# Comparing `tmp/pyiron-atomistics-0.2.9.tar.gz` & `tmp/pyiron-atomistics-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron-atomistics-0.2.9.tar", last modified: Mon Mar 22 13:30:45 2021, max compression
+gzip compressed data, was "pyiron-atomistics-0.3.0.tar", last modified: Thu Jun  8 01:10:49 2023, max compression
```

## Comparing `pyiron-atomistics-0.2.9.tar` & `pyiron-atomistics-0.3.0.tar`

### file list

```diff
@@ -1,134 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      933 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5773 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/pyiron_atomistics/
--rw-r--r--   0 runner    (1001) docker     (121)     3285 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/pyiron_atomistics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.487854 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.487854 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/generic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2436 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/generic/object_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.487854 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32123 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/atomistic.py
--rw-r--r--   0 runner    (1001) docker     (121)    21935 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)     3380 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/interactivewrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     7749 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/potentials.py
--rw-r--r--   0 runner    (1001) docker     (121)    10845 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/sqs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6058 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/structurecontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.487854 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/convergence_volume.py
--rw-r--r--   0 runner    (1001) docker     (121)    22931 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/elastic.py
--rw-r--r--   0 runner    (1001) docker     (121)    28767 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/murnaghan.py
--rw-r--r--   0 runner    (1001) docker     (121)     6823 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)    18408 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (121)     6233 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/quasi.py
--rw-r--r--   0 runner    (1001) docker     (121)     5131 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/serial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1898 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/sqsmaster.py
--rw-r--r--   0 runner    (1001) docker     (121)     7416 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32530 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/_visualize.py
--rw-r--r--   0 runner    (1001) docker     (121)    11003 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/analyse.py
--rw-r--r--   0 runner    (1001) docker     (121)     5249 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/atom.py
--rw-r--r--   0 runner    (1001) docker     (121)   126343 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/atoms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/factories/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3903 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/factories/aimsgb.py
--rw-r--r--   0 runner    (1001) docker     (121)     2094 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/factories/ase.py
--rw-r--r--   0 runner    (1001) docker     (121)    13586 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)    42984 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (121)    15375 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/periodic_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/pyironase.py
--rw-r--r--   0 runner    (1001) docker     (121)     8528 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/pyscal.py
--rw-r--r--   0 runner    (1001) docker     (121)    18221 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/sparse_list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/thermodynamics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/thermodynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12234 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/volumetric/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/volumetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16570 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/volumetric/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/job/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18069 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/job/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3133 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/convergence_encut_parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/convergence_encut_serial.py
--rw-r--r--   0 runner    (1001) docker     (121)     3372 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2246 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/murnaghan_dft.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/waves/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/waves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10607 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/waves/bandstructure.py
--rw-r--r--   0 runner    (1001) docker     (121)    12121 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/waves/dos.py
--rw-r--r--   0 runner    (1001) docker     (121)    29289 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/waves/electronic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/gpaw/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/gpaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5083 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/gpaw/gpaw.py
--rw-r--r--   0 runner    (1001) docker     (121)    18327 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/gpaw/pyiron_ase.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/interactive/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6694 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/interactive/activation_relaxation_technique.py
--rw-r--r--   0 runner    (1001) docker     (121)    11731 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/interactive/scipy_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)    15264 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/interactive/sxextoptint.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    52747 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    42436 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/control.py
--rw-r--r--   0 runner    (1001) docker     (121)    26001 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)     1462 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/lammps.py
--rw-r--r--   0 runner    (1001) docker     (121)    10635 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/potential.py
--rw-r--r--   0 runner    (1001) docker     (121)    22815 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/structure.py
--rw-r--r--   0 runner    (1001) docker     (121)    25329 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    96079 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    16251 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)     3480 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/potential.py
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/sphinx.py
--rw-r--r--   0 runner    (1001) docker     (121)     3794 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/structure.py
--rw-r--r--   0 runner    (1001) docker     (121)     5885 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/volumetric_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/pyiron_atomistics/table/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4119 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/table/datamining.py
--rw-r--r--   0 runner    (1001) docker     (121)     9045 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/table/funct.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/pyiron_atomistics/testing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6854 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/testing/executable.py
--rw-r--r--   0 runner    (1001) docker     (121)    16911 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/testing/randomatomistic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/pyiron_atomistics/thermodynamics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/thermodynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8641 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/thermodynamics/hessian.py
--rw-r--r--   0 runner    (1001) docker     (121)    49541 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/thermodynamics/interfacemethod.py
--rw-r--r--   0 runner    (1001) docker     (121)    18446 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/thermodynamics/sxphonons.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    97442 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    14804 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)    13087 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/metadyn.py
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/oszicar.py
--rw-r--r--   0 runner    (1001) docker     (121)    36265 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/outcar.py
--rw-r--r--   0 runner    (1001) docker     (121)    18519 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/potential.py
--rw-r--r--   0 runner    (1001) docker     (121)     3899 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/procar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1607 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/report.py
--rw-r--r--   0 runner    (1001) docker     (121)    15337 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/structure.py
--rw-r--r--   0 runner    (1001) docker     (121)     2399 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/vasp.py
--rw-r--r--   0 runner    (1001) docker     (121)    33024 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/vasprun.py
--rw-r--r--   0 runner    (1001) docker     (121)      880 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/vaspsol.py
--rw-r--r--   0 runner    (1001) docker     (121)    12462 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/volumetric_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.487854 pyiron-atomistics-0.2.9/pyiron_atomistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      933 2021-03-22 13:30:45.000000 pyiron-atomistics-0.2.9/pyiron_atomistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4588 2021-03-22 13:30:45.000000 pyiron-atomistics-0.2.9/pyiron_atomistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-22 13:30:45.000000 pyiron-atomistics-0.2.9/pyiron_atomistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      278 2021-03-22 13:30:45.000000 pyiron-atomistics-0.2.9/pyiron_atomistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-03-22 13:30:45.000000 pyiron-atomistics-0.2.9/pyiron_atomistics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      201 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2021-03-22 13:30:44.000000 pyiron-atomistics-0.2.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.546330 pyiron-atomistics-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-08 01:10:49.546330 pyiron-atomistics-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.546330 pyiron-atomistics-0.3.0/pyiron_atomistics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-08 01:10:49.546330 pyiron-atomistics-0.3.0/pyiron_atomistics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.530330 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.530330 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/generic/object_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.530330 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41928 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/atomistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/interactivewrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/potentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/structurecontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.530330 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/convergence_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32931 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/murnaghan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/quasi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/sqsmaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.534330 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16778 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)   128325 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/atoms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.534330 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/aimsgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/ase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/atomsk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/materialsproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20288 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/has_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16196 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/periodic_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/pyironase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/sparse_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20264 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/structurestorage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.534330 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/thermodynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/thermodynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.534330 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/volumetric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/volumetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/volumetric/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.534330 pyiron-atomistics-0.3.0/pyiron_atomistics/calphy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/calphy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34986 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/calphy/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.538330 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/bader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.538330 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/job/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18570 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/job/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.538330 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/convergence_encut_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/convergence_encut_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/murnaghan_dft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.538330 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/waves/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/waves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/waves/bandstructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/waves/dos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29606 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/waves/electronic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.538330 pyiron-atomistics-0.3.0/pyiron_atomistics/gpaw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/gpaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/gpaw/gpaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/gpaw/pyiron_ase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.538330 pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/activation_relaxation_technique.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/quasi_newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/scipy_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/sxextoptint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.538330 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44523 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41465 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33649 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25776 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26176 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.542330 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99408 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/volumetric_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.542330 pyiron-atomistics-0.3.0/pyiron_atomistics/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/table/datamining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/table/funct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.542330 pyiron-atomistics-0.3.0/pyiron_atomistics/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/testing/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/testing/randomatomistic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.542330 pyiron-atomistics-0.3.0/pyiron_atomistics/thermodynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/thermodynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/thermodynamics/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51129 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/thermodynamics/interfacemethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/thermodynamics/sxphonons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.546330 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101289 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14988 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13769 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/metadyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/oszicar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45257 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/outcar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/procar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15487 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34363 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/vasprun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/vaspsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/volumetric_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.530330 pyiron-atomistics-0.3.0/pyiron_atomistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-08 01:10:49.000000 pyiron-atomistics-0.3.0/pyiron_atomistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-08 01:10:49.000000 pyiron-atomistics-0.3.0/pyiron_atomistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 01:10:49.000000 pyiron-atomistics-0.3.0/pyiron_atomistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-08 01:10:49.000000 pyiron-atomistics-0.3.0/pyiron_atomistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 01:10:49.000000 pyiron-atomistics-0.3.0/pyiron_atomistics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-08 01:10:49.546330 pyiron-atomistics-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-08 01:10:49.000000 pyiron-atomistics-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.546330 pyiron-atomistics-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/tests/test_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/versioneer.py
```

### Comparing `pyiron-atomistics-0.2.9/LICENSE` & `pyiron-atomistics-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.9/PKG-INFO` & `pyiron-atomistics-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyiron-atomistics
-Version: 0.2.9
+Version: 0.3.0
 Summary: pyiron - an integrated development environment (IDE) for computational materials science.
 Home-page: https://github.com/pyiron/pyiron_atomistics
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
-Description: http://pyiron.org
 Keywords: pyiron
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+
+http://pyiron.org
```

### Comparing `pyiron-atomistics-0.2.9/README.rst` & `pyiron-atomistics-0.3.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pyiron
 ======
 
-.. image:: https://coveralls.io/repos/github/pyiron/pyiron_atomistics/badge.svg?branch=master
-    :target: https://coveralls.io/github/pyiron/pyiron_atomistics?branch=master
+.. image:: https://coveralls.io/repos/github/pyiron/pyiron_atomistics/badge.svg?branch=main
+    :target: https://coveralls.io/github/pyiron/pyiron_atomistics?branch=main
     :alt: Coverage Status
 
 .. image:: https://api.codacy.com/project/badge/Grade/c513254f10004df5a1f5c76425c6584b
     :target: https://app.codacy.com/app/pyiron-runner/pyiron?utm_source=github.com&utm_medium=referral&utm_content=pyiron/pyiron&utm_campaign=Badge_Grade_Settings
     :alt: Codacy Badge
 
 .. image:: https://anaconda.org/conda-forge/pyiron_atomistics/badges/latest_release_date.svg
@@ -43,15 +43,15 @@
 
 pyiron (called pyron) is developed in the `Computational Materials Design department <https://www.mpie.de/CM>`_ of `Joerg Neugebauer <https://www.mpie.de/person/43010/2763386>`_ at the `Max Planck Institut für Eisenforschung (Max Planck Institute for iron research) <https://www.mpie.de/2281/en>`_. While its original focus was to provide a framework to develop and run complex simulation protocols as needed for ab initio thermodynamics it quickly evolved into a versatile tool to manage a wide variety of simulation tasks. In 2016 the `Interdisciplinary Centre for Advanced Materials Simulation (ICAMS) <http://www.icams.de>`_ joined the development of the framework with a specific focus on high throughput applications. In 2018 pyiron was released as open-source project.
 See the `Documentation <http://pyiron.org>`_ page for more details.
 
 
 Installation
 ------------
-You can test pyiron on `Mybinder.org (beta) <https://mybinder.org/v2/gh/pyiron/pyiron_atomistics/master?urlpath=lab>`_.
+You can test pyiron on `Mybinder.org (beta) <https://mybinder.org/v2/gh/pyiron/pyiron_atomistics/main?urlpath=lab>`_.
 For a local installation we recommend to install pyiron inside an `anaconda <https://www.anaconda.com>`_  environment::
 
     conda install -c conda-forge pyiron
 
 
 After the installation of pyiron you need to configure pyiron. The default configuration can be generated automatically. Start a new Python session and import pyiron::
 
@@ -63,15 +63,15 @@
 
 
 See the `Documentation-Installation <https://pyiron.readthedocs.io/en/latest/source/installation.html>`_ page for more details.
 
 
 Example
 -------
-After the successful configuration you can start your first pyiron calculation. Navigate to the the projects directory and start a jupyter notebook or jupyter lab session correspondingly::
+After the successful configuration you can start your first pyiron calculation. Navigate to the projects directory and start a jupyter notebook or jupyter lab session correspondingly::
 
     cd ~/pyiron/projects
     jupyter notebook
 
 Open a new jupyter notebook and inside the notebook you can now validate your pyiron calculation by creating a test project, setting up an initial structure of bcc Fe and visualize it using NGLview::
 
     from pyiron_atomistics import Project
@@ -88,15 +88,15 @@
 
 
 Getting started:
 ----------------
 Test pyiron with mybinder:
 
 .. image:: https://mybinder.org/badge_logo.svg
-     :target: https://mybinder.org/v2/gh/pyiron/pyiron_atomistics/master
+     :target: https://mybinder.org/v2/gh/pyiron/pyiron_atomistics/main
      :alt: mybinder
 
 
 License and Acknowledgments
 ---------------------------
 ``pyiron`` is licensed under the BSD license.
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/generic/object_type.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/generic/object_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from __future__ import print_function
 import importlib
-from pyiron_base import Settings
 
 __author__ = "Joerg Neugebauer, Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 
-s = Settings()
-
-OBJECT_CLASS_DICT = {"ThermoBulk": "pyiron_atomistics.atomistics.thermodynamics.thermo_bulk"}
+OBJECT_CLASS_DICT = {
+    "ThermoBulk": "pyiron_atomistics.atomistics.thermodynamics.thermo_bulk"
+}
 
 
 class ObjectTypeChoice(object):
     def __init__(self):
         for item in list(OBJECT_CLASS_DICT.keys()):
             self.__setattr__(item, item)
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/atomistic.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/atomistic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
-from ase.io import write as ase_write
 import copy
-
-import numpy as np
 import warnings
-
+import numpy as np
+import numbers
+import os
+from typing import Callable, Union, Tuple
+from ase.io import write as ase_write
+import posixpath
 from pyiron_atomistics.atomistics.structure.atoms import Atoms
-from pyiron_base import GenericParameters, GenericMaster, GenericJob as GenericJobCore, deprecate
+from pyiron_atomistics.atomistics.structure.neighbors import NeighborsTrajectory
+from pyiron_atomistics.atomistics.structure.has_structure import HasStructure
+from pyiron_base import (
+    GenericParameters,
+    GenericMaster,
+    GenericJob as GenericJobCore,
+    deprecate,
+)
 
 try:
     from pyiron_base import ProjectGUI
 except (ImportError, TypeError, AttributeError):
     pass
 
 __author__ = "Jan Janssen"
@@ -24,15 +33,15 @@
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 
-class AtomisticGenericJob(GenericJobCore):
+class AtomisticGenericJob(GenericJobCore, HasStructure):
     """
     Atomistic Generic Job class extends the Generic Job class with all the functionality to run jobs containing
     atomistic structures. From this class all specific atomistic Hamiltonians are derived. Therefore it should contain
     the properties/routines common to all atomistic jobs. The functions in this module should be as generic as possible.
 
     Args:
         project (ProjectHDFio): ProjectHDFio instance which points to the HDF5 file the job is stored in
@@ -153,40 +162,41 @@
     def set_input_to_read_only(self):
         """
         This function enforces read-only mode for the input classes, but it has to be implement in the individual
         classes.
         """
         self._generic_input.read_only = True
 
-    def copy_to(
-        self, project=None, new_job_name=None, input_only=False, new_database_entry=True
-    ):
+    def create_pipeline(self, step_lst, delete_existing_job=False):
         """
+        Create a job pipeline
 
         Args:
-            destination:
-            new_job_name:
-            input_only:
-            new_database_entry:
+            step_lst (list): List of functions which create calculations
 
         Returns:
-
+            FlexibleMaster:
         """
-        new_generic_job = super(AtomisticGenericJob, self).copy_to(
-            project=project,
-            new_job_name=new_job_name,
-            input_only=input_only,
-            new_database_entry=new_database_entry,
+        return self.project.create_pipeline(
+            job=self, step_lst=step_lst, delete_existing_job=delete_existing_job
         )
-        if not new_generic_job._structure:
-            new_generic_job._structure = copy.copy(self._structure)
-        return new_generic_job
+
+    def _after_generic_copy_to(self, original, new_database_entry, reloaded):
+        if self._structure is None:
+            self._structure = copy.copy(original._structure)
 
     def calc_minimize(
-        self, ionic_energy_tolerance=0, ionic_force_tolerance=1e-4, e_tol=None, f_tol=None, max_iter=1000, pressure=None, n_print=1
+        self,
+        ionic_energy_tolerance=0,
+        ionic_force_tolerance=1e-4,
+        e_tol=None,
+        f_tol=None,
+        max_iter=1000,
+        pressure=None,
+        n_print=1,
     ):
         """
 
         Args:
             ionic_energy_tolerance (float): Maximum energy difference between 2 steps
             ionic_force_tolerance (float): Maximum force magnitude that each of atoms is allowed to have
             e_tol (float): same as ionic_energy_tolerance (deprecated)
@@ -245,15 +255,26 @@
         initial_temperature=True,
         langevin=False,
     ):
         self._generic_input["calc_mode"] = "md"
         self._generic_input["temperature"] = temperature
         self._generic_input["n_ionic_steps"] = n_ionic_steps
         self._generic_input["n_print"] = n_print
-        self._generic_input.remove_keys(["max_iter", "pressure"])
+        self._generic_input[
+            "temperature_damping_timescale"
+        ] = temperature_damping_timescale
+        if pressure is not None:
+            self._generic_input["pressure"] = pressure
+        if pressure_damping_timescale is not None:
+            self._generic_input[
+                "pressure_damping_timescale"
+            ] = pressure_damping_timescale
+        if time_step is not None:
+            self._generic_input["time_step"] = time_step
+        self._generic_input.remove_keys(["max_iter"])
 
     def from_hdf(self, hdf=None, group_name=None):
         """
         Recreates instance from the hdf5 file
         Args:
             hdf (str): Path to the hdf5 file
             group_name (str): Name of the group which contains the object
@@ -293,59 +314,71 @@
             )
             structure_container.structure = self.structure
             self.parent_id = structure_container.job_id
             return structure_container
         else:
             ValueError("There is no structure attached to the current Job.")
 
+    @deprecate(
+        "Call animate_structures() instead.  Arguments stride/center_of_mass/atom_indices/snapshot_indices/repeat "
+        "can be emulated by calling trajectory() first."
+    )
     def animate_structure(
         self,
-        spacefill=True,
-        show_cell=True,
-        stride=1,
-        center_of_mass=False,
-        particle_size=0.5,
-        camera="orthographic",
+        spacefill: bool = True,
+        show_cell: bool = True,
+        stride: int = 1,
+        center_of_mass: bool = False,
+        particle_size: float = 0.5,
+        camera: str = "orthographic",
+        atom_indices: Union[list, np.ndarray] = None,
+        snapshot_indices: Union[list, np.ndarray] = None,
+        repeat: Union[int, Tuple[int, int, int]] = None,
     ):
         """
         Animates the job if a trajectory is present
 
         Args:
-            spacefill (bool):
-            show_cell (bool):
+            spacefill (bool): If True, then atoms are visualized in spacefill stype
+            show_cell (bool): True if the cell boundaries of the structure is to be shown
             stride (int): show animation every stride [::stride]
                           use value >1 to make animation faster
                            default=1
-            center_of_mass (bool):
+            particle_size (float): Scaling factor for the spheres representing the atoms.
+                                    (The radius is determined by the atomic number)
+            center_of_mass (bool): False (default) if the specified positions are w.r.t. the origin
             camera (str):
                 camera perspective, choose from "orthographic" or "perspective"
+            atom_indices (list/numpy.ndarray): The atom indices for which the trajectory should be generated
+            snapshot_indices (list/numpy.ndarray): The snapshots for which the trajectory should be generated
+            repeat (int/3-tuple of int): Repeat the structures by this before animating
 
         Returns:
             animation: nglview IPython widget
 
         """
-        try:
-            import nglview
-        except ImportError:
-            raise ImportError(
-                "The animate() function requires the package nglview to be installed"
-            )
 
-        animation = nglview.show_asetraj(
-            self.trajectory(stride=stride, center_of_mass=center_of_mass)
+        if self.number_of_structures <= 1:
+            raise ValueError("job must have more than one structure to animate!")
+
+        traj = self.trajectory(
+            stride=stride,
+            center_of_mass=center_of_mass,
+            atom_indices=atom_indices,
+            snapshot_indices=snapshot_indices,
+        )
+        if repeat is not None:
+            traj = traj.transform_structures(lambda s: s.repeat(repeat))
+
+        if self.structure.cell is None:
+            show_cell = False
+
+        animation = traj.animate_structures(
+            spacefill, show_cell, center_of_mass, particle_size, camera
         )
-        if spacefill:
-            animation.add_spacefill(radius_type="vdw", scale=0.5, radius=particle_size)
-            animation.remove_ball_and_stick()
-        else:
-            animation.add_ball_and_stick()
-        if show_cell:
-            if self.structure.cell is not None:
-                animation.add_unitcell()
-        animation.camera = camera
         return animation
 
     def view_structure(self, snapshot=-1, spacefill=True, show_cell=True):
         """
 
         Args:
             snapshot (int): Snapshot of the trajectory one wants
@@ -410,20 +443,43 @@
         """
         new_ham = super(AtomisticGenericJob, self).restart(
             job_name=job_name, job_type=job_type
         )
         if isinstance(new_ham, GenericMaster) and not isinstance(self, GenericMaster):
             new_child = self.restart(job_name=None, job_type=None)
             new_ham.append(new_child)
-        new_ham.structure = self.get_structure(iteration_step=-1)
-        if new_ham.structure is None:
+        if self.number_of_structures > 0:
+            new_ham.structure = self.get_structure(frame=-1)
+        else:
             new_ham.structure = self.structure.copy()
-        new_ham._generic_input['structure'] = 'atoms'
+        new_ham._generic_input["structure"] = "atoms"
         return new_ham
 
+    def get_workdir_file(self, filename: str) -> None:
+        """
+        Checks if a given file exists within the job's working directory and returns the absolute path to it.
+
+        ToDo: Move this to pyiron_base since this is more generic.
+
+        Args:
+            filename (str): The name of the file
+
+        Returns:
+            str: The name absolute path of the file in the working directory
+
+        Raises:
+            FileNotFoundError: Raised if the given file does not exist.
+        """
+        appended_path = posixpath.join(self.working_directory, filename)
+        if not os.path.isfile(appended_path):
+            raise FileNotFoundError(
+                f"File {filename} not found in working directory: {self.working_directory}"
+            )
+        return appended_path
+
     # Required functions
     def continue_with_restart_files(self, job_type=None, job_name=None):
         """
 
         Args:
             job_type:
             job_name:
@@ -462,46 +518,57 @@
             new_ham.structure = self.get_structure(iteration_step=-1)
             new_ham._generic_input["structure"] = "atoms"
         else:
             new_ham._generic_input["structure"] = "continue_final"
         return new_ham
 
     def trajectory(
-        self, stride=1, center_of_mass=False, atom_indices=None,
-            snapshot_indices=None, overwrite_positions=None, overwrite_cells=None
+        self,
+        stride=1,
+        center_of_mass=False,
+        atom_indices=None,
+        snapshot_indices=None,
+        overwrite_positions=None,
+        overwrite_cells=None,
     ):
         """
+        Returns a `Trajectory` instance containing the necessary information to describe the evolution of the atomic
+        structure during the atomistic simulation.
 
         Args:
             stride (int): The trajectories are generated with every 'stride' steps
-            center_of_mass (list/numpy.ndarray): The center of mass
-            atom_indices (list/numpy.ndarray): The atom indices for which the trajectory should be generated
-            snapshot_indices (list/numpy.ndarray): The snapshots for which the trajectory should be generated
-            overwrite_positions (list/numpy.ndarray): List of positions that are meant to overwrite the existing
+            center_of_mass (bool): False (default) if the specified positions are w.r.t. the origin
+            atom_indices (list/ndarray): The atom indices for which the trajectory should be generated
+            snapshot_indices (list/ndarray): The snapshots for which the trajectory should be generated
+            overwrite_positions (list/ndarray): List of positions that are meant to overwrite the existing
                                                       trajectory. Useful to wrap coordinates for example
-            overwrite_cells(list/numpy.ndarray): List of cells that are meant to overwrite the existing
+            overwrite_cells(list/ndarray): List of cells that are meant to overwrite the existing
                                                  trajectory. Only used when `overwrite_positions` is defined. This must
                                                  have the same length of `overwrite_positions`
 
         Returns:
-            pyiron.atomistics.job.atomistic.Trajectory: Trajectory instance
+            pyiron_atomistics.atomistics.job.atomistic.Trajectory: Trajectory instance
 
         """
         cells = self.output.cells
         if len(self.output.indices) != 0:
             indices = self.output.indices
         else:
-            indices = [self.structure.indices] * len(cells)  # Use the same indices throughout
+            indices = [self.structure.indices] * len(
+                cells
+            )  # Use the same indices throughout
         if overwrite_positions is not None:
             positions = np.array(overwrite_positions).copy()
             if overwrite_cells is not None:
                 if overwrite_cells.shape == (len(positions), 3, 3):
                     cells = np.array(overwrite_cells).copy()
                 else:
-                    raise ValueError("overwrite_cells must be compatible with the positions!")
+                    raise ValueError(
+                        "overwrite_cells must be compatible with the positions!"
+                    )
         else:
             positions = self.output.positions.copy()
         conditions = list()
         if isinstance(cells, (list, np.ndarray)):
             if len(cells) == 0:
                 conditions.append(True)
             else:
@@ -521,53 +588,61 @@
             indices = indices[snapshot_indices]
         if atom_indices is None:
             return Trajectory(
                 positions[::stride],
                 self.structure.get_parent_basis(),
                 center_of_mass=center_of_mass,
                 cells=cells[::stride],
-                indices=indices[::stride]
+                indices=indices[::stride],
             )
         else:
             sub_struct = self.structure.get_parent_basis()[atom_indices]
             if len(sub_struct.species) < len(self.structure.species):
                 # Then `sub_struct` has had its indices remapped so they run from 0 to the number of species - 1
                 # But the `indices` array is unaware of this and needs to be remapped to this new space
-                original_symbols = np.array([el.Abbreviation for el in self.structure.species])
+                original_symbols = np.array(
+                    [el.Abbreviation for el in self.structure.species]
+                )
                 sub_symbols = np.array([el.Abbreviation for el in sub_struct.species])
 
-                map_ = np.array([np.argwhere(original_symbols == symbol)[0, 0] for symbol in sub_symbols], dtype=int)
+                map_ = np.array(
+                    [
+                        np.argwhere(original_symbols == symbol)[0, 0]
+                        for symbol in sub_symbols
+                    ],
+                    dtype=int,
+                )
 
                 remapped_indices = np.array(indices)
                 for i_sub, i_original in enumerate(map_):
                     np.place(remapped_indices, indices == i_original, i_sub)
             else:
                 remapped_indices = indices
 
             return Trajectory(
                 positions[::stride, atom_indices, :],
                 sub_struct,
                 center_of_mass=center_of_mass,
                 cells=cells[::stride],
-                indices=remapped_indices[::stride, atom_indices]
+                indices=np.asarray(remapped_indices)[::stride, atom_indices],
             )
 
     def write_traj(
         self,
         filename,
         file_format=None,
         parallel=True,
         append=False,
         stride=1,
         center_of_mass=False,
         atom_indices=None,
         snapshot_indices=None,
         overwrite_positions=None,
         overwrite_cells=None,
-        **kwargs
+        **kwargs,
     ):
         """
         Writes the trajectory in a given file file_format based on the `ase.io.write`_ function.
 
         Args:
             filename (str): Filename of the output
             file_format (str): The specific file_format of the output
@@ -588,75 +663,133 @@
         """
         traj = self.trajectory(
             stride=stride,
             center_of_mass=center_of_mass,
             atom_indices=atom_indices,
             snapshot_indices=snapshot_indices,
             overwrite_positions=overwrite_positions,
-            overwrite_cells=overwrite_cells
+            overwrite_cells=overwrite_cells,
         )
         # Using thr ASE output writer
         ase_write(
             filename=filename,
             images=traj,
             format=file_format,
             parallel=parallel,
             append=append,
-            **kwargs
+            **kwargs,
         )
 
-    # Compatibility functions
-    @deprecate("Use get_structure()")
-    def get_final_structure(self):
+    def get_neighbors_snapshots(
+        self, snapshot_indices=None, num_neighbors=12, **kwargs
+    ):
         """
-        Get the final structure calculated from the job.
+        Get the neighbors only for the required snapshots from the trajectory
+
+        Args:
+            snapshot_indices (list/numpy.ndarray): Snapshots for which the the neighbors need to be computed
+                                                   (eg. [1, 5, 10,..., 100]
+            num_neighbors (int): The cutoff for the number of neighbors
+            **kwargs (dict): Additional arguments to be passed to the `get_neighbors()` routine
+                             (eg. cutoff_radius, norm_order , etc.)
 
         Returns:
-            :class:`.Atoms`
+            pyiron_atomistics.atomistics.structure.neighbors.NeighborsTrajectory: `NeighborsTraj` instances
+                                                                             containing the neighbor information.
         """
-        return self.get_structure(iteration_step=-1)
+        return self.trajectory().get_neighbors_snapshots(
+            snapshot_indices=snapshot_indices, num_neighbors=num_neighbors, **kwargs
+        )
 
-    def get_structure(self, iteration_step=-1, wrap_atoms=True):
+    def get_neighbors(self, start=0, stop=-1, stride=1, num_neighbors=12, **kwargs):
         """
-        Gets the structure from a given iteration step of the simulation (MD/ionic relaxation). For static calculations
-        there is only one ionic iteration step
+        Get the neighbors for a given section of the trajectory
 
         Args:
-            iteration_step (int): Step for which the structure is requested
-            wrap_atoms (bool): True if the atoms are to be wrapped back into the unit cell
+            start (int): Start point of the slice of the trajectory to be sampled
+            stop (int): End point of of the slice of the trajectory to be sampled
+            stride (int): Samples the snapshots evert `stride` steps
+            num_neighbors (int): The cutoff for the number of neighbors
+            **kwargs (dict): Additional arguments to be passed to the `get_neighbors()` routine
+                             (eg. cutoff_radius, norm_order , etc.)
+
+        Returns:
+            pyiron_atomistics.atomistics.structure.neighbors.NeighborsTrajectory: `NeighborsTraj` instances
+                                                                             containing the neighbor information.
+        """
+        return self.trajectory().get_neighbors(
+            start=start, stop=stop, stride=stride, num_neighbors=num_neighbors, **kwargs
+        )
+
+    # Compatibility functions
+    @deprecate("Use get_structure()")
+    def get_final_structure(self):
+        """
+        Get the final structure calculated from the job.
 
         Returns:
-            pyiron.atomistics.structure.atoms.Atoms: The required structure
+            :class:`.Atoms`
         """
+        return self.get_structure(iteration_step=-1)
+
+    def _get_structure(self, frame=-1, wrap_atoms=True):
         if self.structure is None:
-            raise AssertionError('Structure not set')
-        snapshot = self.structure.copy()
+            raise AssertionError("Structure not set")
         if self.output.cells is not None:
             try:
-                snapshot.cell = self.output.cells[iteration_step]
+                cell = self.output.cells[frame]
             except IndexError:
                 if wrap_atoms:
-                    raise IndexError('cell at step ', iteration_step, ' not found')
-                snapshot.cell = None
+                    raise IndexError("cell at step ", frame, " not found") from None
+                cell = None
         if self.output.indices is not None:
             try:
-                snapshot.indices = self.output.indices[iteration_step]
+                indices = self.output.indices[frame]
             except IndexError:
-                pass
+                indices = None
+        if indices is not None and len(indices) != len(self.structure):
+            snapshot = Atoms(
+                species=self.structure.species,
+                indices=indices,
+                positions=np.zeros(indices.shape + (3,)),
+                cell=cell,
+                pbc=self.structure.pbc,
+            )
+        else:
+            snapshot = self.structure.copy()
+            if cell is not None:
+                snapshot.cell = cell
+            if indices is not None:
+                snapshot.indices = indices
         if self.output.positions is not None:
             if wrap_atoms:
-                snapshot.positions = self.output.positions[iteration_step]
+                snapshot.positions = self.output.positions[frame]
                 snapshot.center_coordinates_in_unit_cell()
-            elif len(self.output.unwrapped_positions) > max([iteration_step, 0]):
-                snapshot.positions = self.output.unwrapped_positions[iteration_step]
+            elif len(self.output.unwrapped_positions) > max([frame, 0]):
+                snapshot.positions = self.output.unwrapped_positions[frame]
             else:
-                snapshot.positions += self.output.total_displacements[iteration_step]
+                snapshot.positions += self.output.total_displacements[frame]
         return snapshot
 
+    def _number_of_structures(self):
+        return self.output.positions.shape[0]
+
     def map(self, function, parameter_lst):
+        """
+        Create :class:`.MapMaster` with the current job as reference job.
+
+        The job name is created as 'map_{self.name}'
+
+        Args:
+            function (callable): passed as `modify_function` to the map master
+            parameter_list (list): passed as `parameter_list` to the map master
+
+        Returns:
+            :class:`.MapMaster`: newly created master job
+        """
         master = self.create_job(
             job_type=self.project.job_type.MapMaster, job_name="map_" + self.job_name
         )
         master.modify_function = function
         master.parameter_list = parameter_lst
         return master
 
@@ -701,55 +834,136 @@
 
 
 class MapFunctions(object):
     def __init__(self):
         self.set_structure = set_structure
 
 
-class Trajectory(object):
+class Trajectory(HasStructure):
     """
     A trajectory instance compatible with the ase.io class
-
-    Args:
-        positions (numpy.ndarray): The array of the trajectory in cartesian coordinates
-        structure (pyiron.atomistics.structure.atoms.Atoms): The initial structure instance from which the species info
-                                                             is derived
-        center_of_mass (bool): False (default) if the specified positions are w.r.t. the origin
-        cells (numpy.ndarray): Optional argument of the cell shape at every time step (Nx3x3 array) when the volume
-                                varies
     """
 
-    def __init__(self, positions, structure, center_of_mass=False, cells=None, indices=None):
+    def __init__(
+        self, positions, structure, center_of_mass=False, cells=None, indices=None
+    ):
+        """
+
+        Args:
+            positions (ndarray): The array of the trajectory in cartesian coordinates
+            structure (pyiron.atomistics.structure.atoms.Atoms): The initial structure instance from which the species
+                                                                 info is derived
+            center_of_mass (bool): False (default) if the specified positions are w.r.t. the origin
+            cells (None/ndarray): Optional argument of the cell shape at every time step (Nx3x3 array) when the volume
+                                  varies
+            indices (None/ndarray): Indices for the species in the structure
+        """
+
         if center_of_mass:
             pos = np.copy(positions)
             pos[:, :, 0] = (pos[:, :, 0].T - np.mean(pos[:, :, 0], axis=1)).T
             pos[:, :, 1] = (pos[:, :, 1].T - np.mean(pos[:, :, 1], axis=1)).T
             pos[:, :, 2] = (pos[:, :, 2].T - np.mean(pos[:, :, 2], axis=1)).T
             self._positions = pos
         else:
             self._positions = positions
         self._structure = structure
         self._cells = cells
         self._indices = indices
+        # If the indices don't exist, we construct the indices based on the indices of the initial structure
+        if self._indices is None:
+            self._indices = np.broadcast_to(
+                self._structure.indices,
+                (len(self._positions), len(self._structure.indices)),
+            )
 
     def __getitem__(self, item):
-        new_structure = self._structure.copy()
-        if self._cells is not None:
-            new_structure.cell = self._cells[item]
-        if self._indices is not None:
-            new_structure.indices = self._indices[item]
-        new_structure.positions = self._positions[item]
-        # This step is necessary for using ase.io.write for trajectories
-        new_structure.arrays["positions"] = new_structure.positions
-        # new_structure.arrays['cells'] = new_structure.cell
-        return new_structure
+        if isinstance(item, numbers.Integral):
+            new_structure = self._structure.copy()
+            if self._cells is not None:
+                new_structure.cell = self._cells[item]
+            if self._indices is not None:
+                new_structure.indices = self._indices[item]
+            new_structure.positions = self._positions[item]
+            # This step is necessary for using ase.io.write for trajectories
+            new_structure.arrays["positions"] = new_structure.positions
+            # new_structure.arrays['cells'] = new_structure.cell
+            return new_structure
+        elif isinstance(item, (list, np.ndarray, slice)):
+            snapshots = np.arange(len(self), dtype=int)[item]
+            if self._cells is not None:
+                return Trajectory(
+                    positions=self._positions[snapshots],
+                    cells=self._cells[snapshots],
+                    structure=self[snapshots[0]],
+                    indices=self._indices[snapshots],
+                )
+            else:
+                return Trajectory(
+                    positions=self._positions[snapshots],
+                    cells=self._cells,
+                    structure=self[snapshots[0]],
+                    indices=self._indices[snapshots],
+                )
+
+    def _get_structure(self, frame=-1, wrap_atoms=True):
+        return self[frame]
 
     def __len__(self):
         return len(self._positions)
 
+    _number_of_structures = __len__
+
+    def get_neighbors_snapshots(
+        self, snapshot_indices=None, num_neighbors=12, **kwargs
+    ):
+        """
+        Get the neighbors only for the required snapshots from the trajectory
+
+        Args:
+            snapshot_indices (list/numpy.ndarray): Snapshots for which the the neighbors need to be computed
+                                                   (eg. [1, 5, 10,..., 100]
+            num_neighbors (int): The cutoff for the number of neighbors
+            **kwargs (dict): Additional arguments to be passed to the `get_neighbors()` routine
+                             (eg. cutoff_radius, norm_order , etc.)
+
+        Returns:
+            pyiron_atomistics.atomistics.structure.neighbors.NeighborsTrajectory: `NeighborsTraj` instances
+                                                                             containing the neighbor information.
+        """
+        if snapshot_indices is None:
+            snapshot_indices = np.arange(len(self), dtype=int)
+
+        n_obj = NeighborsTrajectory(
+            has_structure=self[snapshot_indices], num_neighbors=num_neighbors, **kwargs
+        )
+        n_obj.compute_neighbors()
+        return n_obj
+
+    def get_neighbors(self, start=0, stop=-1, stride=1, num_neighbors=12, **kwargs):
+        """
+        Get the neighbors for a given section of the trajectory
+
+        Args:
+            start (int): Start point of the slice of the trajectory to be sampled
+            stop (int): End point of of the slice of the trajectory to be sampled
+            stride (int): Samples the snapshots evert `stride` steps
+            num_neighbors (int): The cutoff for the number of neighbors
+            **kwargs (dict): Additional arguments to be passed to the `get_neighbors()` routine
+                             (eg. cutoff_radius, norm_order , etc.)
+
+        Returns:
+            pyiron_atomistics.atomistics.structure.neighbors.NeighborsTrajectory: `NeighborsTraj` instances
+                                                                             containing the neighbor information.
+        """
+        snapshot_indices = np.arange(len(self))[start:stop:stride]
+        return self.get_neighbors_snapshots(
+            snapshot_indices=snapshot_indices, num_neighbors=num_neighbors, **kwargs
+        )
+
 
 class GenericInput(GenericParameters):
     def __init__(self, input_file_name=None, table_name="generic"):
         super(GenericInput, self).__init__(
             input_file_name=input_file_name,
             table_name=table_name,
             comment_char="#",
@@ -786,16 +1000,16 @@
     @property
     def forces(self):
         return self._job["output/generic/forces"]
 
     @property
     def force_max(self):
         """
-            maximum force magnitude of each step which is used for
-            convergence criterion of structure optimizations
+        maximum force magnitude of each step which is used for
+        convergence criterion of structure optimizations
         """
         return np.linalg.norm(self.forces, axis=-1).max(axis=-1)
 
     @property
     def positions(self):
         return self._job["output/generic/positions"]
 
@@ -817,34 +1031,40 @@
 
     @property
     def unwrapped_positions(self):
         unwrapped_positions = self._job["output/generic/unwrapped_positions"]
         if unwrapped_positions is not None:
             return unwrapped_positions
         else:
-            return self._job.structure.positions+self.total_displacements
+            return self._job.structure.positions + self.total_displacements
 
     @property
     def volume(self):
         return self._job["output/generic/volume"]
 
     @property
     def indices(self):
         return self._job["output/generic/indices"]
 
     @property
     def displacements(self):
         """
         Output for 3-d displacements between successive snapshots, with minimum image convention.
         For the total displacements from the initial configuration, use total_displacements
-        This algorithm collapses if:
-        - the ID's are not consistent (i.e. you can also not change the number of atoms)
-        - there are atoms which move by more than half a box length in any direction within two snapshots (due to
-        periodic boundary conditions)
+        This algorithm collapses if (if `unwrapped_positions` is not available in output):
+            - the ID's are not consistent (i.e. you can also not change the number of atoms)
+            - there are atoms which move by more than half a box length in any direction within
+                two snapshots (due to periodic boundary conditions)
         """
+        unwrapped_positions = self._job["output/generic/unwrapped_positions"]
+        if unwrapped_positions is not None:
+            return np.diff(
+                np.append([self._job.structure.positions], unwrapped_positions, axis=0),
+                axis=0,
+            )
         return self.get_displacements(self._job.structure, self.positions, self.cells)
 
     @staticmethod
     def get_displacements(structure, positions, cells):
         """
         Output for 3-d displacements between successive snapshots, with minimum image convention.
         For the total displacements from the initial configuration, use total_displacements
@@ -860,33 +1080,39 @@
 
         Returns:
             numpy.ndarray: Displacements (N_steps x N_atoms x 3)
 
         """
         # Check if the cell changes in any snapshot
         c = cells.reshape(-1, 9)
-        if np.max(c.max(axis=0)-c.min(axis=0)) > 1e-5:
-            warnings.warn("You are computing displacements in a simulation with periodic boundary conditions \n"
-                          "and a varying cell shape.")
-        displacement = np.einsum('nki,nij->nkj', positions, np.linalg.inv(cells))
+        if np.max(c.max(axis=0) - c.min(axis=0)) > 1e-5:
+            warnings.warn(
+                "You are computing displacements in a simulation with periodic boundary conditions \n"
+                "and a varying cell shape."
+            )
+        displacement = np.einsum("nki,nij->nkj", positions, np.linalg.inv(cells))
         displacement[1:] -= displacement[:-1]
         displacement[0] -= structure.get_scaled_positions()
-        displacement[:,:,structure.pbc] -= np.rint(displacement)[:,:,structure.pbc]
-        displacement = np.einsum('nki,nij->nkj', displacement, cells)
+        displacement[:, :, structure.pbc] -= np.rint(displacement)[:, :, structure.pbc]
+        displacement = np.einsum("nki,nij->nkj", displacement, cells)
         return displacement
 
     @property
     def total_displacements(self):
         """
         Output for 3-d total displacements from the initial configuration, with minimum image convention.
-        For the diplacements for the successive snapshots, use displacements
-        This algorithm collapses if:
-        - the ID's are not consistent (i.e. you can also not change the number of atoms)
-        - there are atoms which move by more than half a box length in any direction within two snapshots (due to periodic boundary conditions)
+        For the displacements for the successive snapshots, use displacements
+        This algorithm collapses if (if `unwrapped_positions` is not available in the output):
+            - the ID's are not consistent (i.e. you can also not change the number of atoms)
+            - there are atoms which move by more than half a box length in any direction within
+                two snapshots (due to periodic boundary conditions)
         """
+        unwrapped_positions = self._job["output/generic/unwrapped_positions"]
+        if unwrapped_positions is not None:
+            return unwrapped_positions - self._job.structure.positions
         return np.cumsum(self.displacements, axis=0)
 
     def __dir__(self):
         hdf5_path = self._job["output/generic"]
         if hdf5_path is not None:
             return hdf5_path.list_nodes()
         else:
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/interactive.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/interactive.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
-from pyiron_base import Settings, InteractiveBase
-from pyiron_atomistics.atomistics.structure.atoms import Atoms
+from pyiron_base import state, InteractiveBase
 from pyiron_atomistics.atomistics.structure.periodic_table import PeriodicTable
-from pyiron_atomistics.atomistics.job.atomistic import AtomisticGenericJob, GenericOutput
+from pyiron_atomistics.atomistics.job.atomistic import (
+    AtomisticGenericJob,
+    GenericOutput,
+)
 from collections import defaultdict
 
 __author__ = "Osamu Waseda, Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "development"
 __date__ = "Sep 1, 2017"
 
-s = Settings()
-
 
 class GenericInteractive(AtomisticGenericJob, InteractiveBase):
     def __init__(self, project, job_name):
         super(GenericInteractive, self).__init__(project, job_name)
         self.output = GenericInteractiveOutput(job=self)
         self._structure_previous = None
         self._structure_current = None
         self._interactive_enforce_structure_reset = False
         self._interactive_grand_canonical = False
         self._interactive_fetch_completed = True
         self._interactive_species_lst = np.array([])
         self._periodic_table = PeriodicTable()
-        self.interactive_input_functions = {'index': self.interactive_index_organizer,
-                                            'cell': self.interactive_cell_organizer,
-                                            'positions': self.interactive_positions_organizer,
-                                            'magnetic_moments': self.interactive_magmom_organizer}
-        self.interactive_output_functions =  {'cells': self.interactive_cells_getter,
-                                              'energy_pot': self.interactive_energy_pot_getter,
-                                              'energy_tot': self.interactive_energy_tot_getter,
-                                              'forces': self.interactive_forces_getter,
-                                              'positions': self.interactive_positions_getter,
-                                              'pressures': self.interactive_pressures_getter,
-                                              'stress': self.interactive_stress_getter,
-                                              'steps': self.interactive_steps_getter,
-                                              'temperature': self.interactive_temperatures_getter,
-                                              'indices': self.interactive_indices_getter,
-                                              'computation_time': self.interactive_computation_time_getter,
-                                              'unwrapped_positions': self.interactive_unwrapped_positions_getter,
-                                              'atom_spin_constraints': self.interactive_atom_spin_constraints_getter,
-                                              'atom_spins': self.interactive_atom_spins_getter,
-                                              'magnetic_forces': self.interactive_magnetic_forces_getter,
-                                              'volume': self.interactive_volume_getter}
+        self.interactive_input_functions = {
+            "index": self.interactive_index_organizer,
+            "cell": self.interactive_cell_organizer,
+            "positions": self.interactive_positions_organizer,
+            "magnetic_moments": self.interactive_magmom_organizer,
+        }
+        self.interactive_output_functions = {
+            "cells": self.interactive_cells_getter,
+            "energy_pot": self.interactive_energy_pot_getter,
+            "energy_tot": self.interactive_energy_tot_getter,
+            "forces": self.interactive_forces_getter,
+            "positions": self.interactive_positions_getter,
+            "pressures": self.interactive_pressures_getter,
+            "stress": self.interactive_stress_getter,
+            "steps": self.interactive_steps_getter,
+            "temperature": self.interactive_temperatures_getter,
+            "indices": self.interactive_indices_getter,
+            "computation_time": self.interactive_computation_time_getter,
+            "unwrapped_positions": self.interactive_unwrapped_positions_getter,
+            "atom_spin_constraints": self.interactive_atom_spin_constraints_getter,
+            "atom_spins": self.interactive_atom_spins_getter,
+            "magnetic_forces": self.interactive_magnetic_forces_getter,
+            "volume": self.interactive_volume_getter,
+        }
         self.interactive_cache = defaultdict(list)
 
     @property
     def interactive_enforce_structure_reset(self):
         return self._interactive_enforce_structure_reset
 
     @interactive_enforce_structure_reset.setter
@@ -117,15 +121,14 @@
         self.status.running = True
         if self.structure is None:
             raise ValueError("Input structure not set. Use method set_structure()")
         if not self.interactive_is_activated():
             self.interactive_initialize_interface()
         if self._structure_previous is None:
             self._structure_previous = self.structure.copy()
-        self._update_previous_structure()
         if self._structure_current is not None:
             if (
                 len(self._structure_current) != len(self._structure_previous)
                 and not self._interactive_grand_canonical
             ):
                 raise ValueError(
                     "The number of atoms changed, this is currently not supported!"
@@ -133,80 +136,83 @@
             if not self._interactive_enforce_structure_reset:
                 functions_to_execute = list(self.interactive_input_functions.values())
                 for v in functions_to_execute:
                     v()
             else:
                 self._logger.debug("Generic library: structure changed!")
                 self.interactive_structure_setter(self._structure_current)
+        self._update_previous_structure()
 
     def interactive_index_organizer(self):
         index_merge_lst = self._interactive_species_lst.tolist() + list(
             self._structure_current.get_species_symbols()
         )
         el_lst = sorted(set(index_merge_lst), key=index_merge_lst.index)
         current_structure_index = [
-            el_lst.index(el)
-            for el in self._structure_current.get_chemical_symbols()
+            el_lst.index(el) for el in self._structure_current.get_chemical_symbols()
         ]
         previous_structure_index = [
-            el_lst.index(el)
-            for el in self._structure_previous.get_chemical_symbols()
+            el_lst.index(el) for el in self._structure_previous.get_chemical_symbols()
         ]
         if not np.array_equal(
             np.array(current_structure_index),
             np.array(previous_structure_index),
         ):
             self._logger.debug("Generic library: indices changed!")
             self.interactive_indices_setter(self._structure_current.indices)
 
     def interactive_cell_organizer(self):
-        if not np.allclose(
+        if self._generic_input["calc_mode"] != "static" or not np.allclose(
             self._structure_current.cell,
             self._structure_previous.cell,
-            rtol=1e-15, atol=1e-15,
+            rtol=1e-15,
+            atol=1e-15,
         ):
             self._logger.debug("Generic library: cell changed!")
             try:
                 self.interactive_cells_setter(self._structure_current.cell)
             except NotImplementedError:
-                del self.interactive_input_functions['cell']
+                del self.interactive_input_functions["cell"]
 
     def interactive_positions_organizer(self):
-        if not np.allclose(
+        if self._generic_input["calc_mode"] != "static" or not np.allclose(
             self._structure_current.positions,
             self._structure_previous.positions,
             rtol=1e-15,
             atol=1e-15,
         ):
             self._logger.debug("Generic library: positions changed!")
             self.interactive_positions_setter(self._structure_current.positions)
 
     def interactive_magmom_organizer(self):
-        if all(mm is None for mm in self._structure_current.get_initial_magnetic_moments()):
-            del self.interactive_input_functions['magnetic_moments']
-        elif (None in self._structure_previous.get_initial_magnetic_moments()
+        if all(
+            mm is None for mm in self._structure_current.get_initial_magnetic_moments()
+        ):
+            del self.interactive_input_functions["magnetic_moments"]
+        elif (
+            None in self._structure_previous.get_initial_magnetic_moments()
             or not np.allclose(
                 self._structure_current.get_initial_magnetic_moments(),
                 self._structure_previous.get_initial_magnetic_moments(),
             )
         ):
             self._logger.debug("Generic library: magnetic moments changed!")
             try:
                 self.interactive_spin_constraints_setter(
                     self._structure_current.get_initial_magnetic_moments()
                 )
             except NotImplementedError:
-                del self.interactive_input_functions['magnetic_moments']
+                del self.interactive_input_functions["magnetic_moments"]
 
     def interactive_cells_getter(self):
         return self.initial_structure.cell
 
     def interactive_collect(self):
         del_key_lst = []
-        for k,v in self.interactive_output_functions.items():
+        for k, v in self.interactive_output_functions.items():
             try:
                 value = v()
                 if value is not None:
                     self.interactive_cache[k].append(value)
                 else:
                     del_key_lst.append(k)
             except NotImplementedError:
@@ -265,35 +271,16 @@
     def interactive_time_getter(self):
         return self.interactive_steps_getter()
 
     def interactive_volume_getter(self):
         return self.initial_structure.get_volume()
 
     def _update_previous_structure(self):
-        """
-        Update the previous structure to the last step configuration
-        Args:
-            wrap_atoms (bool):
-        """
-        try:
-            indices = self.output.indices[-1]
-            positions = self.output.positions[-1]
-            cell = self.output.cells[-1]
-        except IndexError:
-            return
-        if len(self._interactive_species_lst) == 0:
-            el_lst = [el.Abbreviation for el in self.structure.species]
-        else:
-            el_lst = self._interactive_species_lst.tolist()
-        self._structure_previous = self._structure_previous.__class__(
-            positions=positions,
-            cell=cell,
-            indices=indices,
-            species=[self._periodic_table.element(el) for el in el_lst],
-        )
+        """Update the previous structure to the last step configuration."""
+        self._structure_previous = self.structure.copy()
 
     @staticmethod
     def _extend_species_elements(struct_species, species_array):
         if not all(np.isin(struct_species, species_array)):
             new_elements_index = np.invert(np.isin(struct_species, species_array))
             species_array = np.append(species_array, struct_species[new_elements_index])
         return species_array
@@ -324,17 +311,15 @@
 
     def interactive_atom_spin_constraints_getter(self):
         raise NotImplementedError(
             "interactive_atom_spin_constraints_getter() is not implemented!"
         )
 
     def interactive_atom_spins_getter(self):
-        raise NotImplementedError(
-            "interactive_atom_spins_getter() is not implemented!"
-        )
+        raise NotImplementedError("interactive_atom_spins_getter() is not implemented!")
 
     def interactive_magnetic_forces_getter(self):
         raise NotImplementedError(
             "interactive_magnetic_forces_getter() is not implemented!"
         )
 
     def interactive_spin_constraints_setter(self, spins):
@@ -356,15 +341,17 @@
     def interactive_stress_getter(self):
         raise NotImplementedError("interactive_stress_getter() is not implemented!")
 
     def interactive_structure_setter(self, structure):
         raise NotImplementedError("interactive_structure_setter() is not implemented!")
 
     def interactive_computation_time_getter(self):
-        raise NotImplementedError("interactive_computation_time_getter() is not implemented!")
+        raise NotImplementedError(
+            "interactive_computation_time_getter() is not implemented!"
+        )
 
     def interactive_temperatures_getter(self):
         raise NotImplementedError(
             "interactive_temperatures_getter() is not implemented!"
         )
 
     def interactive_unwrapped_positions_getter(self):
@@ -441,20 +428,21 @@
 
         Returns:
 
         """
         return_lst = self._key_from_cache(key)
         hdf5_output = self._key_from_hdf(key)
         if hdf5_output is not None:
-            return_lst = hdf5_output.tolist() + return_lst
+            return np.concatenate([hdf5_output, *return_lst])
         else:
             prop_result = prop(self)
             if prop_result is not None:
-                return_lst = prop(self).tolist() + return_lst
-        return np.array(return_lst)
+                return np.concatenate([prop_result, *return_lst])
+            else:
+                return np.asarray(return_lst)
 
     def _lst_from_property(self, key):
         """
         Fetch latest values for the given property.
 
         Values are first looked up in the interactive cache, then in the interactive group in the HDF5 file
         ('output/interactive/<key>') and if not found there via approriate getter from our super class (GenericOutput).
@@ -540,15 +528,15 @@
                 + super(GenericOutput).__dir__()
             )
         )
 
 
 class InteractiveInterface(object):
     def __init__(self):
-        self._logger = s.logger
+        self._logger = state.logger
 
     def get_cell(self):
         raise NotImplementedError
 
     def set_cell(self, cell):
         raise NotImplementedError
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/interactivewrapper.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/interactivewrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 
 class InteractiveWrapper(InteractiveWrapperBase):
     def __init__(self, project, job_name):
         super(InteractiveWrapper, self).__init__(project, job_name)
 
     @property
     def structure(self):
-        if self.ref_job:
+        if self.ref_job is not None:
             return self._ref_job.structure
         else:
             return None
 
     @structure.setter
     def structure(self, basis):
-        if self.ref_job:
+        if self.ref_job is not None:
             self._ref_job.structure = basis
         else:
             raise ValueError(
                 "A structure can only be set after a start job has been assinged."
             )
 
     @deprecate("use get_structure() instead")
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/potentials.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/potentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,29 +4,27 @@
 
 """
 An abstract Potential class to provide an easy access for the available potentials. Currently implemented for the
 OpenKim https://openkim.org database.
 """
 import pandas
 import os
-from pyiron_base import Settings
+from pyiron_base import state
 
 __author__ = "Martin Boeckmann, Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "development"
 __date__ = "Sep 1, 2017"
 
-s = Settings()
-
 
 class PotentialAbstract(object):
     """
     The PotentialAbstract class loads a list of available potentials and sorts them. Afterwards the potentials can be
     accessed through:
         PotentialAbstract.<Element>.<Element> or PotentialAbstract.find_potentials_set({<Element>, <Element>}
 
@@ -67,18 +65,19 @@
             [
                 True if set(element).issubset(species) else False
                 for species in self._potential_df["Species"].values
             ]
         ]
 
     def find_by_name(self, potential_name):
-        mask = (self._potential_df["Name"] == potential_name)
+        mask = self._potential_df["Name"] == potential_name
         if not mask.any():
-            raise ValueError("Potential '{}' not found in database.".format(
-                             potential_name))
+            raise ValueError(
+                "Potential '{}' not found in database.".format(potential_name)
+            )
         return self._potential_df[mask]
 
     def list(self):
         """
         List the available potentials
 
         Returns:
@@ -110,15 +109,15 @@
             file_name_lst (set):
             backward_compatibility_name (str):
 
         Returns:
             pandas.DataFrame:
         """
         env = os.environ
-        resource_path_lst = s.resource_paths
+        resource_path_lst = state.settings.resource_paths
         for conda_var in ["CONDA_PREFIX", "CONDA_DIR"]:
             if conda_var in env.keys():  # support iprpy-data package
                 path_to_add = os.path.join(env[conda_var], "share", "iprpy")
                 if path_to_add not in resource_path_lst:
                     resource_path_lst += [path_to_add]
         df_lst = []
         for resource_path in resource_path_lst:
@@ -127,30 +126,32 @@
             if "potentials" in resource_path or "iprpy" in resource_path:
                 for path, folder_lst, file_lst in os.walk(resource_path):
                     for periodic_table_file_name in file_name_lst:
                         if (
                             periodic_table_file_name in file_lst
                             and periodic_table_file_name.endswith(".csv")
                         ):
-                            df_lst.append(pandas.read_csv(
-                                os.path.join(path, periodic_table_file_name),
-                                index_col=0,
-                                converters={
-                                    "Species": lambda x: x.replace("'", "")
-                                    .strip("[]")
-                                    .split(", "),
-                                    "Config": lambda x: x.replace("'", "")
-                                    .replace("\\n", "\n")
-                                    .strip("[]")
-                                    .split(", "),
-                                    "Filename": lambda x: x.replace("'", "")
-                                    .strip("[]")
-                                    .split(", "),
-                                },
-                            ))
+                            df_lst.append(
+                                pandas.read_csv(
+                                    os.path.join(path, periodic_table_file_name),
+                                    index_col=0,
+                                    converters={
+                                        "Species": lambda x: x.replace("'", "")
+                                        .strip("[]")
+                                        .split(", "),
+                                        "Config": lambda x: x.replace("'", "")
+                                        .replace("\\n", "\n")
+                                        .strip("[]")
+                                        .split(", "),
+                                        "Filename": lambda x: x.replace("'", "")
+                                        .strip("[]")
+                                        .split(", "),
+                                    },
+                                )
+                            )
         if len(df_lst) > 0:
             return pandas.concat(df_lst)
         else:
             raise ValueError("Was not able to locate the potential files.")
 
     @staticmethod
     def _get_potential_default_df(
@@ -164,15 +165,15 @@
             plugin_name (str):
             file_name_lst (set):
             backward_compatibility_name (str):
 
         Returns:
             pandas.DataFrame:
         """
-        for resource_path in s.resource_paths:
+        for resource_path in state.settings.resource_paths:
             pot_path = os.path.join(resource_path, plugin_name, "potentials")
             if os.path.exists(pot_path):
                 resource_path = pot_path
             if "potentials" in resource_path:
                 for path, folder_lst, file_lst in os.walk(resource_path):
                     for periodic_table_file_name in file_name_lst:
                         if (
@@ -198,9 +199,12 @@
         for resource_path in resource_path_lst:
             path_direct = os.path.join(resource_path, path)
             path_indirect = os.path.join(resource_path, rel_path, path)
             if os.path.exists(path_direct):
                 return path_direct
             elif os.path.exists(path_indirect):
                 return path_indirect
-    raise ValueError("Either the filename or the functional has to be defined.",
-                     path, resource_path_lst)
+    raise ValueError(
+        "Either the filename or the functional has to be defined.",
+        path,
+        resource_path_lst,
+    )
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/sqs.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/sqs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,115 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
-from multiprocessing import cpu_count
+import random
+import warnings
+import itertools
+from structuretoolkit.build import sqs_structures
 from pyiron_atomistics.atomistics.job.atomistic import AtomisticGenericJob
-from pyiron_base import DataContainer, GenericParameters, Settings, ImportAlarm
-from pyiron_atomistics.atomistics.structure.atoms import Atoms, ase_to_pyiron, pyiron_to_ase
-from pymatgen.io.ase import AseAtomsAdaptor
+from pyiron_base import state, DataContainer, GenericParameters, ImportAlarm
+from pyiron_atomistics.atomistics.structure.atoms import Atoms, ase_to_pyiron
 import numpy as np
 
+
 try:
-    from sqsgenerator.core.sqs import ParallelSqsIterator
+    from sqsgenerator.settings import BadSettings
+    from sqsgenerator import sqs_optimize, process_settings, IterationMode
+
     import_alarm = ImportAlarm()
 except ImportError:
     import_alarm = ImportAlarm(
-        "SQSJob relies on sqsgenerator.core.sqs.ParallelSqsIterator, but this is unavailable. Please ensure your "
+        "SQSJob relies on the sqsgenerator module, but this is unavailable. Please ensure your "
         "python environment contains the [sqsgenerator module](https://github.com/dgehringer/sqsgenerator), e.g. with "
         "`conda install -c conda-forge sqsgenerator`."
     )
 
+
+from typing import Dict
+
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "0.1"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "development"
 __date__ = "Aug 14, 2020"
 
 
-s = Settings()
-
-
-def pyiron_to_pymatgen(structure):
-    return AseAtomsAdaptor.get_structure(pyiron_to_ase(structure))
-
+def chemical_formula(atoms: Atoms) -> str:
+    def group_symbols():
+        for species, same in itertools.groupby(atoms.get_chemical_symbols()):
+            num_same = len(list(same))
+            yield species if num_same == 1 else f"{species}{num_same}"
+
+    return "".join(group_symbols())
+
+
+def map_dict(f, d: Dict) -> Dict:
+    return {k: f(v) for k, v in d.items()}
+
+
+def mole_fractions_to_composition(
+    mole_fractions: Dict[str, float], num_atoms: int
+) -> Dict[str, int]:
+    # if the sum of x is less than 1 - 1/n then we are missing at least one atoms
+    if not (1.0 - 1 / num_atoms) < sum(mole_fractions.values()) < (1.0 + 1 / num_atoms):
+        raise ValueError(
+            "mole-fractions must sum up to one: {}".format(sum(mole_fractions.values()))
+        )
 
-def pymatgen_to_pyiron(structure):
-    return ase_to_pyiron(AseAtomsAdaptor.get_atoms(structure))
+    composition = map_dict(lambda x: x * num_atoms, mole_fractions)
+    # check to avoid partial occupation -> x_i * num_atoms is not an integer number
+    if any(
+        map(
+            lambda occupation: not float.is_integer(round(occupation, 1)),
+            composition.values(),
+        )
+    ):
+        # at least one of the specified species exhibits fractional occupation, we try to fix it by rounding
+        composition_ = map_dict(lambda occ: int(round(occ)), composition)
+        warnings.warn(
+            "The current mole-fraction specification cannot be applied to {} atoms, "
+            "as it would lead to fractional occupation. Hence, I have changed it from "
+            '"{}" -> "{}"'.format(
+                num_atoms,
+                mole_fractions,
+                map_dict(lambda n: n / num_atoms, composition_),
+            )
+        )
+        composition = composition_
 
+    # due to rounding errors there might be a difference of one atom
+    actual_atoms = sum(composition.values())
+    diff = actual_atoms - num_atoms
+    if abs(diff) == 1:
+        # it is not possible to distribute atoms equally e.g x_a = x_b = x_c = 1/3 on 32 atoms
+        # we remove one randomly bet we inform the user
+        removed_species = random.choice(tuple(composition))
+        composition[removed_species] -= 1
+        warnings.warn(
+            'It is not possible to distribute the species properly. Therefore one "{}" atom was removed. '
+            "This changes the input mole-fraction specification. "
+            '"{}" -> "{}"'.format(
+                removed_species,
+                mole_fractions,
+                map_dict(lambda n: n / num_atoms, composition),
+            )
+        )
+    elif abs(diff) > 1:
+        # something else is wrong with the mole-fractions input
+        raise ValueError(
+            "Cannot interpret mole-fraction dict {}".format(mole_fractions)
+        )
 
-def get_sqs_structures(structure, mole_fractions, weights=None, objective=0.0, iterations=1e6, output_structures=10,
-                       num_threads=None):
-    structure = pyiron_to_pymatgen(structure)
-    if not weights:
-        weights = {i: 1.0/i for i in range(1, 7)}
-    if not num_threads:
-        # Thats default behaviour
-        num_threads = cpu_count()
-    iterator = ParallelSqsIterator(structure, mole_fractions, weights, num_threads=num_threads)
-    structures, decmp, iter_, cycle_time = iterator.iteration(
-        iterations=iterations, output_structures=output_structures, objective=objective
-    )
-    return [pymatgen_to_pyiron(s) for s in structures], decmp, iter_, cycle_time
+    return composition
 
 
 class SQSJob(AtomisticGenericJob):
     """
     Produces special quasirandom structures designed to duplicate truly random chemical distributions as well as
     possible while using finite periodic cells.
 
@@ -91,29 +142,34 @@
     Example:
         Case I: Get SQS for a given mole fraction:
 
         >>> job = SQSJob(job_name='sqs')
         >>> job.structure = structure
         >>> job.input.mole_fractions = {'Al': 0.8, 'Ni':0.2}
         >>> job.run()
-        
+
         Case II: Get SQS for a given structure already containing at least 2 elements:
 
         >>> job = SQSJob(job_name='sqs')
         >>> job.structure = structure
         >>> job.run()
 
         In Case II, if the mole fractions will be overwritten if you specify the values (like in Case I)
     """
 
     publication = {
         "sqs": {
             "method": {
                 "title": "Special quasirandom structures",
-                "author": ["Zunger, A.", "Wei, S.-H.", "Ferreira, L.G.", "Bernard, J.E."],
+                "author": [
+                    "Zunger, A.",
+                    "Wei, S.-H.",
+                    "Ferreira, L.G.",
+                    "Bernard, J.E.",
+                ],
                 "journal": "Phys. Rev. Lett.",
                 "volume": "65",
                 "issue": "3",
                 "pages": "353",
                 "numpages": "0",
                 "month": "July",
                 "publisher": "American Physical Society",
@@ -123,117 +179,98 @@
         }
     }
 
     @import_alarm
     def __init__(self, project, job_name):
         super(SQSJob, self).__init__(project, job_name)
         # self.input = InputList(table_name='input')
-        self.input = DataContainer(table_name='custom_dict')
+        self.input = DataContainer(table_name="custom_dict")
         self.input.mole_fractions = dict()
         self.input.weights = None
         self.input.objective = 0.0
         self.input.iterations = 1e6
         self.input.n_output_structures = 1
         self._python_only_job = True
         self._lst_of_struct = []
         self.__hdf_version__ = "0.2.0"
-        self.__name__ = "SQSJob"
-        s.publication_add(self.publication)
+
+        state.publications.add(self.publication)
 
     @property
     def list_of_structures(self):
         return self._lst_of_struct
 
     def validate_ready_to_run(self):
         super(SQSJob, self).validate_ready_to_run()
         if len(self.input.mole_fractions) == 0:
             chem = np.unique(self.structure.get_chemical_symbols(), return_counts=True)
-            self.input.mole_fractions = dict(zip(chem[0], chem[1]/np.sum(chem[1])))
+            self.input.mole_fractions = dict(zip(chem[0], chem[1] / np.sum(chem[1])))
         if len(self.input.mole_fractions) == 1:
-            raise ValueError('There must be at least two chemical elements')
+            raise ValueError("There must be at least two chemical elements")
 
     def db_entry(self):
         """
         Generate the initial database entry
 
         Returns:
             (dict): db_dict
         """
         db_dict = super(SQSJob, self).db_entry()
         if self.structure:
             struct_len = len(self.structure)
-            mole_fractions = {
-                k: v for k, v in self.input.mole_fractions.items()
-            }
+            mole_fractions = {k: v for k, v in self.input.mole_fractions.items()}
             el_lst = sorted(mole_fractions.keys())
             atom_number_lst = [
-                int(np.round(mole_fractions[el]*struct_len))
-                for el in el_lst
+                int(np.round(mole_fractions[el] * struct_len)) for el in el_lst
             ]
-            db_dict["ChemicalFormula"] = "".join([
-                e + str(n)
-                for e, n in zip(el_lst, atom_number_lst)
-            ])
+            db_dict["ChemicalFormula"] = "".join(
+                [e + str(n) for e, n in zip(el_lst, atom_number_lst)]
+            )
         return db_dict
 
     def list_structures(self):
-        if self.status.finished:
-            return self._lst_of_struct
-        else:
-            return []
-    
-    def get_structure(self, iteration_step=-1, wrap_atoms=True):
-        """
-        Gets the structure from a given iteration step of the simulation (MD/ionic relaxation). For static calculations
-        there is only one ionic iteration step
-        Args:
-            iteration_step (int): Step for which the structure is requested
-            wrap_atoms (bool): True if the atoms are to be wrapped back into the unit cell
-        Returns:
-            pyiron.atomistics.structure.atoms.Atoms: The required structure
-        """
-        return self.list_structures()[iteration_step]
-    
-    # This function is executed 
+        return self._lst_of_struct if self.status.finished else []
+
+    def _get_structure(self, frame=-1, wrap_atoms=True):
+        return self.list_structures()[frame]
+
+    def _number_of_structures(self):
+        return len(self.list_structures())
+
+    # This function is executed
     def run_static(self):
-        self._lst_of_struct, decmp, iterations, cycle_time = get_sqs_structures(
-            structure=self.structure, 
-            mole_fractions={
-                k:v for k,v in self.input.mole_fractions.items()
-            },
+        structure_lst, decmp, iterations, cycle_time = sqs_structures(
+            structure=self.structure,
+            mole_fractions={k: v for k, v in self.input.mole_fractions.items()},
             weights=self.input.weights,
             objective=self.input.objective,
             iterations=self.input.iterations,
             output_structures=self.input.n_output_structures,
-            num_threads=self.server.cores
+            num_threads=self.server.cores,
+            return_statistics=True,
         )
+        self._lst_of_struct = [ase_to_pyiron(s) for s in structure_lst]
         for i, structure in enumerate(self._lst_of_struct):
             with self.project_hdf5.open("output/structures/structure_" + str(i)) as h5:
                 structure.to_hdf(h5)
         with self.project_hdf5.open("output") as h5:
             h5["decmp"] = decmp
             h5["cycle_time"] = cycle_time
             h5["iterations"] = iterations
         self.status.finished = True
         self.project.db.item_update(self._runtime(), self.job_id)
-        
+
     def to_hdf(self, hdf=None, group_name=None):
-        super().to_hdf(
-            hdf=hdf,
-            group_name=group_name
-        )
+        super().to_hdf(hdf=hdf, group_name=group_name)
         self._structure_to_hdf()
         with self.project_hdf5.open("input") as h5in:
             self.input.to_hdf(h5in)
 
     def from_hdf(self, hdf=None, group_name=None):
-        super().from_hdf(
-            hdf=hdf,
-            group_name=group_name
-        )
+        super().from_hdf(hdf=hdf, group_name=group_name)
         self._structure_from_hdf()
         self._backwards_compatible_input_from_hdf()
         with self.project_hdf5.open("output/structures") as hdf5_output:
             structure_names = hdf5_output.list_groups()
         for group in structure_names:
             with self.project_hdf5.open("output/structures/" + group) as hdf5_output:
                 self._lst_of_struct.append(Atoms().from_hdf(hdf5_output))
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/structurecontainer.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/structurecontainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,94 +9,77 @@
 )
 __version__ = "0.1"
 __maintainer__ = "Marvin Poul"
 __email__ = "poul@mpie.de"
 __status__ = "development"
 __date__ = "Aug 12, 2020"
 
-from pyiron_base import DataContainer, GenericJob
+from pyiron_base import DataContainer, GenericJob, deprecate
 from pyiron_atomistics.atomistics.job.atomistic import AtomisticGenericJob
 from pyiron_atomistics.atomistics.structure.atoms import Atoms
+from pyiron_atomistics.atomistics.structure.has_structure import HasStructure
+from pyiron_atomistics.atomistics.structure.structurestorage import StructureStorage
 
 
-class StructureContainer(AtomisticGenericJob):
+class StructureContainer(GenericJob, HasStructure):
     """
     Container to save a list of structures in HDF5 together with tags.
 
     Add new structures with :meth:`.append`, they are added to
     :attr:`.structure_lst`.  The HDF5 is written when :meth:`.run` is called.
     """
 
     def __init__(self, project, job_name):
         super().__init__(project, job_name)
         self.__version__ = "0.2.0"
-        self.__hdf_version__ = "0.2.0"
-        self._structure_lst = DataContainer(table_name = "structures")
+        self.__hdf_version__ = "0.3.0"
+        self._structure_lst = DataContainer(table_name="structures")
+        self._container = StructureStorage()
         self.server.run_mode.interactive = True
 
     @property
     def structure_lst(self):
         """
         :class:`.DataContainer`: list of :class:`~.Atoms`
         """
+        if len(self._structure_lst) != len(self._container):
+            self._structure_lst = DataContainer(list(self._container.iter_structures()))
         return self._structure_lst
 
     @staticmethod
     def _to_structure(structure_or_job):
         """
         Return structure from structure or atomic job.
 
         Args:
             structure_or_job (:class:`~.AtomisticGenericJob`, :class:`~.Atoms`):
                 if :class:`~.AtomisticGenericJob` try to get most recent structure,
         copy it and set the job_id in :attr:`~.Atoms.info`
-        
+
         Returns:
             :class:`~.Atoms`: structure from the job or given structure
-            
+
         Raises:
             ValueError: if given :class:`~.AtomisticGenericJob` has no structure set
             TypeError: if structure_or_job is of invalid type
         """
         if isinstance(structure_or_job, AtomisticGenericJob):
             if structure_or_job.structure:
                 s = structure_or_job.get_structure(-1).copy()
                 s.info["jobid"] = structure_or_job.job_id
                 return s
             else:
-                raise ValueError(
-                        "The job does not contain any structure to import."
-                )
+                raise ValueError("The job does not contain any structure to import.")
         elif isinstance(structure_or_job, Atoms):
             return structure_or_job
         else:
             raise TypeError(
-                "You can only use a structure object or an "
-                "AtomisticGenericJob object."
+                f"structure_or_job must be of type {Atoms} or {AtomisticGenericJob}, not {type(structure_or_job)}"
             )
 
-    @property
-    def structure(self):
-        """
-        :class:`~.Atoms`: first (or only) structure set in the container
-
-        :setter:  :class:`~.Atoms`, :class:`~.AtomisticGenericJob`
-            if a job is given take the last structure and add the job id to its
-            :attr:`pyiron_atomistics.atomistics.structure.Atoms.info`
-        """
-        return self.structure_lst.get(0, None)
-
-    @structure.setter
-    def structure(self, structure_or_job):
-        item = self._to_structure(structure_or_job)
-        if len(self.structure_lst) >= 1:
-            self.structure_lst[0] = item
-        else:
-            self.structure_lst.append(item)
-
     def append(self, structure_or_job):
         """
         Add new structure to structure list.
 
         The added structure will available in :attr:`~.structure_lst`.  If the
         structure is added via a job, retrieve the latest structure and add its
         id to :attr:`pyiron_atomistics.atomistics.generic.Atoms.info`.
@@ -106,59 +89,86 @@
                 if :class:`~.AtomisticGenericJob` add from
                 :meth:`~.AtomisticGenericJob.get_structure`,
                 otherwise add just the given :class:`~.Atoms`
 
         Returns:
             dict: item added to :attr:`~.structure_lst`
         """
-        self.structure_lst.append(self._to_structure(structure_or_job))
-        return self.structure_lst[0]
+        struct = self._to_structure(structure_or_job)
+        self._container.add_structure(struct)
+        return struct
+
+    def add_structure(self, structure: Atoms, identifier: str = None, **kwargs):
+        """
+        Add a new structure.
+
+        Args:
+            structure (:class:`~.Atoms`): structure to add
+            identifier (str, optional): optional identifier for the structure
+            **kwargs: passed through to the underlying :meth:`.StructureStorage.add_structure`
+        """
+        self._container.add_structure(structure, identifier=identifier, **kwargs)
 
     def run_static(self):
         self.status.finished = True
 
     def run_if_interactive(self):
         self.to_hdf()
         self.status.finished = True
 
     def write_input(self):
         pass
 
     def collect_output(self):
         pass
 
-    def to_hdf(self, hdf = None, group_name = None):
-        # skip any of the AtomisticGenericJob specific serialization, since we
-        # handle the structures on our own and that method might just confuse
-        # self.structure and self.structure_lst
-        GenericJob.to_hdf(self, hdf = hdf, group_name = group_name)
+    @property
+    @deprecate("use get_structure()")
+    def structure(self):
+        return self._get_structure(frame=0)
 
-        hdf = self.project_hdf5.create_group("structures")
+    @structure.setter
+    @deprecate("use append()")
+    def structure(self, struct):
+        self.append(struct)
 
-        for i, structure in enumerate(self.structure_lst.values()):
-            structure.to_hdf(hdf, group_name = "structure_{}".format(i))
+    def _number_of_structures(self):
+        return len(self._container)
 
-    def from_hdf(self, hdf = None, group_name = None):
+    def _get_structure(self, frame=-1, wrap_atoms=True):
+        return self._container._get_structure(frame=frame, wrap_atoms=wrap_atoms)
+
+    def to_hdf(self, hdf=None, group_name=None):
+        super().to_hdf(hdf=hdf, group_name=group_name)
+        self._container.to_hdf(hdf=self.project_hdf5, group_name="structures")
+
+    def from_hdf(self, hdf=None, group_name=None):
         # keep hdf structure for version peeking in separate variable, so that
         # the inherited from_hdf() can properly deal with it
         h5 = hdf or self.project_hdf5
         if group_name:
             h5 = h5[group_name]
         if "HDF_VERSION" in h5.list_nodes():
             hdf_version = h5["HDF_VERSION"]
         else:
             # old versions didn't use to set a HDF version
             hdf_version = "0.1.0"
         if hdf_version == "0.1.0":
             super().from_hdf(hdf=hdf, group_name=group_name)
             with self.project_hdf5.open("input") as hdf5_input:
-                self.structure = Atoms().from_hdf(hdf5_input)
-        else:
-            GenericJob.from_hdf(self, hdf = hdf, group_name = group_name)
-
-            self.structure_lst.clear()
+                self.append(Atoms().from_hdf(hdf5_input))
+        elif hdf_version == "0.2.0":
+            GenericJob.from_hdf(self, hdf=hdf, group_name=group_name)
 
             hdf = self.project_hdf5["structures"]
             for group in sorted(hdf.list_groups()):
-                structure = Atoms()
-                structure.from_hdf(hdf, group_name = group)
-                self.structure_lst.append(structure)
+                self.append(Atoms().from_hdf(hdf=hdf, group_name=group))
+        else:
+            super().from_hdf(hdf=hdf, group_name=group_name)
+            self._container.from_hdf(hdf=self.project_hdf5, group_name="structures")
+
+    @property
+    def plot(self):
+        """
+        Accessor for :class:`~.StructurePlots` instance using these structures.
+        """
+        return self._container.plot
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/convergence_volume.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/convergence_volume.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     Args:
         project:
         job_name:
     """
 
     def __init__(self, project, job_name):
         super(ConvergenceVolume, self).__init__(project, job_name=job_name)
-        self.__name__ = "ConvergenceVolume"
+
         self.__version__ = "0.0.2"
         if not self["input/convergence_goal"]:
             self.set_goal(convergence_goal, eps=0.005)
 
     def create_next(self, job_name=None):
         """
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/elastic.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/elastic.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,79 +25,91 @@
 __date__ = "Oct 21, 2020"
 
 
 eV_div_A3_to_GPa = (
     1e21 / scipy.constants.physical_constants["joule-electron volt relationship"][0]
 )
 
+
 def get_elastic_tensor_by_orientation(orientation, elastic_tensor):
     """
     Get elastic tensor in a given orientation
     Args:
         orientation (numpy.ndarray): 3x3 orthogonal orientation (no need to be orthonormal)
         elastic_tensor (numpy.ndarray): 6x6 elastic tensor
     Returns:
         (numpy.ndarray) 6x6 elastic_tensor in a given orientation
     """
-    orientation = np.einsum('ij,i->ij', orientation, 1/np.linalg.norm(orientation, axis=-1))
+    orientation = np.einsum(
+        "ij,i->ij", orientation, 1 / np.linalg.norm(orientation, axis=-1)
+    )
     if not np.isclose(np.linalg.det(orientation), 1):
-        raise ValueError('orientation must be an orthogonal 3x3 tensor')
-    C = np.zeros((3,3,3,3))
+        raise ValueError("orientation must be an orthogonal 3x3 tensor")
+    C = np.zeros((3, 3, 3, 3))
     r = np.arange(3)
     for i, j, k, l in itertools.product(r, r, r, r):
-        C[i,j,k,l] = elastic_tensor[i+(i!=j)*(6-2*i-j), k+(k!=l)*(6-2*k-l)]
-    C = np.einsum('Ii,Jj,ijkl,Kk,Ll->IJKL',
-                  orientation, orientation, C, orientation, orientation)
+        C[i, j, k, l] = elastic_tensor[
+            i + (i != j) * (6 - 2 * i - j), k + (k != l) * (6 - 2 * k - l)
+        ]
+    C = np.einsum(
+        "Ii,Jj,ijkl,Kk,Ll->IJKL", orientation, orientation, C, orientation, orientation
+    )
     elastic_tensor_to_return = np.zeros_like(elastic_tensor)
     for i, j, k, l in itertools.product(r, r, r, r):
-        elastic_tensor_to_return[i+(i!=j)*(6-2*i-j), k+(k!=l)*(6-2*k-l)] = C[i,j,k,l]
+        elastic_tensor_to_return[
+            i + (i != j) * (6 - 2 * i - j), k + (k != l) * (6 - 2 * k - l)
+        ] = C[i, j, k, l]
     return elastic_tensor_to_return
 
 
 def calc_elastic_constants(elastic_tensor):
     """
     Calculate elastic constants from the elastic tensor.
     For anistropic material (i.e. zener_ratio!=1), the values may or may not make
     sense -> don't trust the results straightforwardly
     Args:
         elastic_tensor (numpy.ndarray): 6x6 tensor
     """
     output = {}
-    output['elastic_tensor'] = elastic_tensor
-    output['lame_coefficient'] = np.mean(elastic_tensor[:3, :3].diagonal())
-    output['shear_modulus'] = np.mean(elastic_tensor[3:, 3:].diagonal())
-    output['bulk_modulus'] = np.mean(elastic_tensor[:3,:3])
-    output['youngs_modulus'] = 1/np.mean(np.linalg.inv(elastic_tensor[:3,:3]).diagonal())
-    output['poissons_ratio'] = -output['youngs_modulus']*np.sum(
-        np.linalg.inv(elastic_tensor[:3,:3])
-    )/6+0.5
-    output['zener_ratio'] = 12*np.mean(elastic_tensor[3:,3:].diagonal())
-    output['zener_ratio'] /= (3*np.trace(elastic_tensor[:3,:3])-np.sum(elastic_tensor[:3,:3]))
+    output["elastic_tensor"] = elastic_tensor
+    output["lame_coefficient"] = np.mean(elastic_tensor[:3, :3].diagonal())
+    output["shear_modulus"] = np.mean(elastic_tensor[3:, 3:].diagonal())
+    output["bulk_modulus"] = np.mean(elastic_tensor[:3, :3])
+    output["youngs_modulus"] = 1 / np.mean(
+        np.linalg.inv(elastic_tensor[:3, :3]).diagonal()
+    )
+    output["poissons_ratio"] = (
+        -output["youngs_modulus"] * np.sum(np.linalg.inv(elastic_tensor[:3, :3])) / 6
+        + 0.5
+    )
+    output["zener_ratio"] = 12 * np.mean(elastic_tensor[3:, 3:].diagonal())
+    output["zener_ratio"] /= 3 * np.trace(elastic_tensor[:3, :3]) - np.sum(
+        elastic_tensor[:3, :3]
+    )
     return output
 
+
 def _convert_to_voigt(s, rotations=None, strain=False):
     if rotations is not None:
-        s_tmp = np.einsum('nik,mkl,njl->nmij',
-            rotations, s, rotations
-        ).reshape(-1, 9)
+        s_tmp = np.einsum("nik,mkl,njl->nmij", rotations, s, rotations).reshape(-1, 9)
     else:
         s_tmp = s.reshape(-1, 9)
     s_tmp = s_tmp[:, [0, 4, 8, 5, 2, 1]]
     if strain:
         s_tmp[:, 3:] *= 2
     return s_tmp
 
 
 def _fit_coeffs_with_stress(
-        strain,
-        stress,
-        rotations,
-        max_polynomial_order=None,
-        fit_first_order=False,
-    ):
+    strain,
+    stress,
+    rotations,
+    max_polynomial_order=None,
+    fit_first_order=False,
+):
     higher_strains = _get_higher_order_strains(
         strain,
         max_polynomial_order=max_polynomial_order,
         rotations=rotations,
         derivative=True,
     )
     strain = _convert_to_voigt(strain, rotations=rotations, strain=True)
@@ -105,149 +117,149 @@
         strain = np.concatenate((strain, higher_strains), axis=-1)
     stress = _convert_to_voigt(stress, rotations=rotations, strain=False)
     score = []
     coeff = []
     for ii in range(6):
         strain_tmp = strain.copy()
         strain_tmp[:, 6:] *= strain[:, ii, np.newaxis]
-        reg = LinearRegression(
-            fit_intercept=fit_first_order
-        ).fit(strain_tmp, stress[:,ii])
+        reg = LinearRegression(fit_intercept=fit_first_order).fit(
+            strain_tmp, stress[:, ii]
+        )
         coeff.append(reg.coef_)
-        score.append(reg.score(strain_tmp, stress[:,ii]))
+        score.append(reg.score(strain_tmp, stress[:, ii]))
     return np.array(coeff), np.array(score)
 
+
 def _fit_coeffs_with_energies(
-        strain,
-        energy,
-        volume,
-        rotations,
-        max_polynomial_order=None,
-        fit_first_order=False,
-    ):
+    strain,
+    energy,
+    volume,
+    rotations,
+    max_polynomial_order=None,
+    fit_first_order=False,
+):
     higher_strains = _get_higher_order_strains(
         strain,
         max_polynomial_order=max_polynomial_order,
         rotations=rotations,
         derivative=False,
     )
     strain_voigt = _convert_to_voigt(strain, rotations=rotations, strain=True)
     energy = np.tile(energy, len(rotations))
     volume = np.tile(volume, len(rotations))
     # Create symmetric tensor for elastic tensor
-    strain = 0.5*np.einsum('ni,nj->nij', strain_voigt, strain_voigt)
-    # Set lower triangle to 0 (which is the same as the upper triangle)
-    strain = np.triu(strain).reshape(-1, 36)
+    strain = 0.5 * np.einsum("ni,nj->nij", *2 * [strain_voigt])
     # Remove lower triangle
-    strain = strain[:,np.sum(strain, axis=0)!=0]
+    strain = np.array([s[np.triu_indices(6)] for s in strain])
     if higher_strains is not None:
         strain = np.concatenate((strain, higher_strains), axis=-1)
     if fit_first_order:
         strain = np.concatenate((strain, strain_voigt), axis=-1)
-    strain = np.einsum('n,ni->ni', volume, strain)
+    strain = np.einsum("n,ni->ni", volume, strain)
     reg = LinearRegression().fit(strain, energy)
     score = reg.score(strain, energy)
     # Create base tensor for elastic tensor
-    coeff = np.triu(np.ones((6,6))).flatten()
+    coeff = np.zeros((6, 6))
     # Multiply upper triangle with upper triangle coeffs (v.s.)
-    coeff[coeff!=0] *= reg.coef_[:21]*eV_div_A3_to_GPa
-    coeff = coeff.reshape(6,6)
-    coeff = 0.5*(coeff+coeff.T)
+    coeff[np.triu_indices(6)] = reg.coef_[:21] * eV_div_A3_to_GPa
+    coeff = coeff.reshape(6, 6)
+    coeff = 0.5 * (coeff + coeff.T)
     return coeff, score
 
+
 def _get_linear_dependent_indices(strain_lst):
     """
 
     This function returns an array of booleans, which shows linearly dependent
     strain matrices. Strain matrices which have True along axis=0 are linearly
     dependent. Axis=1 should contain the total number of strain matrices.
 
     """
     s = np.array(strain_lst).reshape(-1, 9)
     norm = np.linalg.norm(s, axis=-1)
     sign = np.sign(np.sum(s, axis=-1))
     indices = np.round(
-        np.einsum('ni,n->ni', s, sign/(norm+np.isclose(norm, 0))),
-        decimals=8
+        np.einsum("ni,n->ni", s, sign / (norm + np.isclose(norm, 0))), decimals=8
     )
     indices = np.unique(indices, axis=0, return_inverse=True)[1]
     na = np.newaxis
-    indices = np.unique(indices[~np.isclose(norm, 0)])[:,na]==indices[na,:]
+    indices = np.unique(indices[~np.isclose(norm, 0)])[:, na] == indices[na, :]
     # 0-tensor gets a special treatment, since it's linearly dependent on all
     # strains (even though it virtually changes nothing)
     indices[:, np.isclose(norm, 0)] = True
     return indices
 
+
 def _get_higher_order_strains(
-        strain_lst,
-        max_polynomial_order=None,
-        rotations=None,
-        derivative=False,
-    ):
+    strain_lst,
+    max_polynomial_order=None,
+    rotations=None,
+    derivative=False,
+):
     """
     Returns a matrix containing higher order strains. axis=0 corresponds to the
     elastic tensors and axis=1 the higher order strains. From the number of
     linearly dependent strains the polynomial order is calculated internally
     -> up to 3: harmonic; 4 and 5: third degree etc.
     """
     strain_lst = np.array(strain_lst)
     indices = _get_linear_dependent_indices(strain_lst)
     # counts stands for the polynomial degree, starting from 1 meaning first
     # anharmonic contribution
     counts = np.sum(indices, axis=1)
-    counts = np.floor(counts/2-0.75).astype(int)
+    counts = np.floor(counts / 2 - 0.75).astype(int)
     if max_polynomial_order is not None:
-        counts[counts>max_polynomial_order-2] = max_polynomial_order-2
-    counts[counts<0] = 0
-    if sum(counts)==0: # No term gets more than harmonic part
+        counts[counts > max_polynomial_order - 2] = max_polynomial_order - 2
+    counts[counts < 0] = 0
+    if sum(counts) == 0:  # No term gets more than harmonic part
         return None
     strain_higher_order = np.zeros((len(strain_lst), np.sum(counts)))
     na = np.newaxis
     for cc, ind in zip(counts, indices):
         # Take strain with the highest magnitude among linearly dependent ones
         # It does not have to be the highest magnitude, but it's important that
         # it does not choose the zero strain vector (which is with all the
         # strains linearly dependent)
         E = strain_lst[ind][
-            np.linalg.norm(strain_lst[ind].reshape(-1, 9), axis=-1).argmax()]
+            np.linalg.norm(strain_lst[ind].reshape(-1, 9), axis=-1).argmax()
+        ]
         # Normalize strain
         E /= np.linalg.norm(E)
         # Take inner product (Instead of taking the inner product, it is also
         # possible to take the magnitude of each strain, in which case there
         # must be a well defined convention on the sign so that the odd
         # exponent terms can take asymmetry around strain=0 into account).
-        E = np.sum((E*strain_lst[ind]).reshape(-1, 9), axis=-1)
+        E = np.sum((E * strain_lst[ind]).reshape(-1, 9), axis=-1)
         # Take polynomial development
         if derivative:
-            E = E[:,na]**(np.arange(cc)+1)[na,:]*np.sign(E)[:,na]
+            E = E[:, na] ** (np.arange(cc) + 1)[na, :] * np.sign(E)[:, na]
         else:
-            E = E[:,na]**(np.arange(cc)+3)[na,:]
+            E = E[:, na] ** (np.arange(cc) + 3)[na, :]
         # Check starting column
-        starting_index = np.sum(np.any(strain_higher_order!=0, axis=0))
-        strain_higher_order[ind, starting_index:starting_index+E.shape[1]] = E
+        starting_index = np.sum(np.any(strain_higher_order != 0, axis=0))
+        strain_higher_order[ind, starting_index : starting_index + E.shape[1]] = E
     # Repeat by the number of rotations (nothing to do with real rotations)
     if rotations is not None:
-        strain_higher_order = np.einsum('n,ij->nij',
-                                          np.ones(len(rotations)),
-                                          strain_higher_order)
-    strain_higher_order = strain_higher_order.reshape(
-        -1, strain_higher_order.shape[-1]
-    )
+        strain_higher_order = np.einsum(
+            "n,ij->nij", np.ones(len(rotations)), strain_higher_order
+        )
+    strain_higher_order = strain_higher_order.reshape(-1, strain_higher_order.shape[-1])
     return strain_higher_order
 
+
 def calc_elastic_tensor(
-        strain,
-        stress=None,
-        energy=None,
-        volume=None,
-        rotations=None,
-        return_score=False,
-        max_polynomial_order=None,
-        fit_first_order=False,
-    ):
+    strain,
+    stress=None,
+    energy=None,
+    volume=None,
+    rotations=None,
+    return_score=False,
+    max_polynomial_order=None,
+    fit_first_order=False,
+):
     """
     Calculate 6x6-elastic tensor from the strain and stress or strain and
     energy+volume.
 
     Rotations matrices can be added to take box symmetries into account (unit
     matrix can be added but does not have to be included in the list)
 
@@ -256,107 +268,111 @@
         stress (numpy.ndarray): nx3x3 stress tensors
         energy (numpy.ndarray): n energy values
         volume (numpy.ndarray): n volume values
         rotations (numpy.ndarray): mx3x3 rotation matrices
         return_score (numpy.ndarray): return regression score
             (cf. sklearn.linear_mode.LinearRegression)
     """
-    if len(strain)==0:
-        raise ValueError('Not enough points')
+    if len(strain) == 0:
+        raise ValueError("Not enough points")
     if rotations is not None:
         rotations = np.append(np.eye(3), rotations).reshape(-1, 3, 3)
-        _, indices = np.unique(
-            np.round(rotations, 6), axis=0, return_inverse=True
-        )
+        _, indices = np.unique(np.round(rotations, 6), axis=0, return_inverse=True)
         rotations = rotations[np.unique(indices)]
     else:
         rotations = np.eye(3).reshape(1, 3, 3)
-    if stress is not None and len(stress)==len(strain):
+    if stress is not None and np.asarray(stress).shape == np.asarray(strain).shape:
         coeff, score = _fit_coeffs_with_stress(
             strain=strain,
             stress=stress,
             rotations=rotations,
             max_polynomial_order=max_polynomial_order,
             fit_first_order=fit_first_order,
         )
-    elif (energy is not None
-          and volume is not None
-          and len(energy)==len(strain)
-          and len(energy)==len(volume)):
+    elif (
+        energy is not None
+        and volume is not None
+        and len(energy) == len(strain)
+        and len(energy) == len(volume)
+    ):
         coeff, score = _fit_coeffs_with_energies(
             strain=strain,
             energy=energy,
             volume=volume,
             rotations=rotations,
             max_polynomial_order=max_polynomial_order,
             fit_first_order=fit_first_order,
         )
     else:
-        raise ValueError('Provide either strain and stress, or strain, energy '
-                         + 'and volume of same length.')
+        raise ValueError(
+            "Provide either strain and stress, or strain, energy "
+            + "and volume of same length."
+        )
     if return_score:
-        return np.array(coeff)[:,:6], score
+        return np.array(coeff)[:, :6], score
     else:
-        return np.array(coeff)[:,:6]
+        return np.array(coeff)[:, :6]
+
 
 def _get_random_symmetric_matrices(n):
-    matrices = np.random.random((n, 3, 3))-0.5
-    return matrices + np.einsum('nij->nji', matrices)
+    matrices = np.random.random((n, 3, 3)) - 0.5
+    return matrices + np.einsum("nij->nji", matrices)
 
 
-def get_strain(max_strain=0.05, n_set=10, polynomial_order=2,
-               additional_points=0, normalize=False):
+def get_strain(
+    max_strain=0.05, n_set=10, polynomial_order=2, additional_points=0, normalize=False
+):
     """
-        Args:
-            max_strain (float): Maximum strain (for each component)
-            n_set (int): Number of strain values to return
-            polynomial_order (int): This value determines the number of
-                linear-dependent strain values. For a polynomial order of two,
-                there will be +-strain and for 3, there will be +-strain and
-                +-0.5*strain etc.
-            additional_points (int): Additional linear-dependent points
-            normalize (bool): Whether to normalize the strain values. If True,
-                the norm (Frobenius norm) of all outer most strain (i.e. the
-                greatest strain within the linear-dependent strains) will be
-                equal to max_strain
+    Args:
+        max_strain (float): Maximum strain (for each component)
+        n_set (int): Number of strain values to return
+        polynomial_order (int): This value determines the number of
+            linear-dependent strain values. For a polynomial order of two,
+            there will be +-strain and for 3, there will be +-strain and
+            +-0.5*strain etc.
+        additional_points (int): Additional linear-dependent points
+        normalize (bool): Whether to normalize the strain values. If True,
+            the norm (Frobenius norm) of all outer most strain (i.e. the
+            greatest strain within the linear-dependent strains) will be
+            equal to max_strain
 
-        Returns: numpy.ndarray of strains (n, 3, 3)
+    Returns: numpy.ndarray of strains (n, 3, 3)
     """
     strain_lst = _get_random_symmetric_matrices(n_set)
     if normalize:
         strain_lst = np.einsum(
-            'nij,n->nij',
+            "nij,n->nij",
             strain_lst,
-            1/np.linalg.norm(strain_lst.reshape(-1, 9), axis=-1)
+            1 / np.linalg.norm(strain_lst.reshape(-1, 9), axis=-1),
         )
     strain_lst *= max_strain
-    m = np.linspace(-1, 1, int(2*polynomial_order+2*additional_points-1))
-    strain_lst = np.einsum('k,nij->nkij', m, strain_lst).reshape(-1, 9)
+    m = np.linspace(-1, 1, int(2 * polynomial_order + 2 * additional_points - 1))
+    strain_lst = np.einsum("k,nij->nkij", m, strain_lst).reshape(-1, 9)
     return np.unique(strain_lst, axis=0).reshape(-1, 3, 3)
 
+
 class _ElasticJobGenerator(JobGenerator):
     @property
     def parameter_list(self):
         parameter_lst = []
-        for ii, epsilon in enumerate(self._master.input['strain_matrices']):
+        for ii, epsilon in enumerate(self._master.input["strain_matrices"]):
             basis = self._master.ref_job.structure.copy()
             basis.apply_strain(np.array(epsilon))
             parameter_lst.append([ii, basis])
         return parameter_lst
 
     def job_name(self, parameter):
-        return "{}_{}".format(
-            self._master.job_name, parameter[0]
-        ).replace(".", "_")
+        return "{}_{}".format(self._master.job_name, parameter[0]).replace(".", "_")
 
     @staticmethod
     def modify_job(job, parameter):
         job.structure = parameter[1]
         return job
 
+
 class ElasticTensor(AtomisticParallelMaster):
     """
     Class to calculate the elastic tensor and isotropic elastic constants.
 
     Example:
 
     >>> job = pr.create_job('SomeAtomisticJob', 'atomistic')
@@ -398,152 +414,176 @@
     time, make sure to choose an orientation which maximizes the number
     symmetry operations. Also if the child job does not support pressure,
     better increase the number of measurements - without pressure the constants
     must be fit to total cell energies, which contain only a fraction of the
     data that the pressure matrix does. This lack can be compensated by
     sampling more rotations.
     """
+
     def __init__(self, project, job_name):
         """
 
         Args:
             project: project
             job_name: job_name
         """
         super().__init__(project, job_name)
-        self.__name__ = "ElasticTensor"
-        self.__version__ = "0.1.0"
 
+        self.__version__ = "0.1.0"
         self.input["min_num_measurements"] = (
-            11, "minimum number of samples to be taken"
+            11,
+            "minimum number of samples to be taken",
+        )
+        self.input["min_num_points"] = (
+            105,
+            "minimum number of data points"
+            + "(number of measurements will be min_num_points/len(rotations))",
         )
-        self.input["min_num_points"] = (105, "minimum number of data points"
-            + "(number of measurements will be min_num_points/len(rotations))")
         self.input["max_strain"] = (
             0.01,
             "relative volume variation around volume defined by ref_ham",
         )
-        self.input['polynomial_order'] = 2
-        self.input['additional_points'] = (
+        self.input["polynomial_order"] = 2
+        self.input["additional_points"] = (
             0,
-            'number of additional linear-dependent points to make anharmonic'
-             + ' contribution more stable. It should not be larger than 0 if'
-             + ' polynomial_order=2'
+            "number of additional linear-dependent points to make anharmonic"
+            + " contribution more stable. It should not be larger than 0 if"
+            + " polynomial_order=2",
         )
-        self.input['strain_matrices'] = (
+        self.input["strain_matrices"] = (
             [],
-            'List of strain matrices (generated automatically if not set)'
+            "List of strain matrices (generated automatically if not set)",
         )
-        self.input['use_symmetry'] = (True, 'Whether to consider box symmetries')
-        self.input['rotations'] = (
+        self.input["use_symmetry"] = (True, "Whether to consider box symmetries")
+        self.input["rotations"] = (
             [],
-            'List of rotation matrices (generated automatically if not set)'
+            "List of rotation matrices (generated automatically if not set)",
         )
-        self.input['normalize_magnitude'] = (
+        self.input["normalize_magnitude"] = (
             False,
-            'Whether or normalize magnitude, so that the Frobenius norm is '
-            + 'always max_strain'
+            "Whether or normalize magnitude, so that the Frobenius norm is "
+            + "always max_strain",
         )
-        self.input['use_elements'] = (
+        self.input["use_elements"] = (
             True,
-            'Whether or not consider chemical elements for the symmetry'
-            + ' analysis. Could be useful for SQS'
+            "Whether or not consider chemical elements for the symmetry"
+            + " analysis. Could be useful for SQS",
         )
-        self.input['fit_first_order'] = (
+        self.input["fit_first_order"] = (
             False,
-            'Whether or not fit first order strains. In principle it should not'
-            + ' be necessary, but might stabilize the calculation if the'
-            + ' reference structure is not exactly in the zero pressure state.'
-            + ' Setting this to True does not correct the second order strains'
+            "Whether or not fit first order strains. In principle it should not"
+            + " be necessary, but might stabilize the calculation if the"
+            + " reference structure is not exactly in the zero pressure state."
+            + " Setting this to True does not correct the second order strains",
+        )
+        self.input["use_pressure"] = (
+            True,
+            "Whether to use the pressure values instead of energy or not. Ignored if pressure"
+            + "values are not available",
         )
         self._job_generator = _ElasticJobGenerator(self)
 
     @property
     def _number_of_measurements(self):
-        return int(max(
-            self.input['min_num_measurements'],
-            np.ceil(self.input['min_num_points']/max(len(self.input['rotations']), 1))
-        ))
+        return int(
+            max(
+                self.input["min_num_measurements"],
+                np.ceil(
+                    self.input["min_num_points"] / max(len(self.input["rotations"]), 1)
+                ),
+            )
+        )
 
     def _get_rotation_matrices(self):
         rotations = self.ref_job.structure.get_symmetry(
-            use_elements=self.input['use_elements']
-        )['rotations']
+            use_elements=self.input["use_elements"]
+        )["rotations"]
         _, indices = np.unique(np.round(rotations, 6), axis=0, return_inverse=True)
         rotations = rotations[np.unique(indices)]
-        self.input['rotations'] = rotations.tolist()
+        self.input["rotations"] = rotations.tolist()
 
     def _create_strain_matrices(self):
-        self.input['strain_matrices'] = get_strain(
-            max_strain=self.input['max_strain'],
+        self.input["strain_matrices"] = get_strain(
+            max_strain=self.input["max_strain"],
             n_set=self._number_of_measurements,
-            polynomial_order=self.input['polynomial_order'],
-            additional_points=self.input['additional_points'],
-            normalize=self.input['normalize_magnitude']
+            polynomial_order=self.input["polynomial_order"],
+            additional_points=self.input["additional_points"],
+            normalize=self.input["normalize_magnitude"],
         ).tolist()
 
+    def save(self):
+        self.validate_ready_to_run()
+        super().save()
+
     def validate_ready_to_run(self):
         super().validate_ready_to_run()
-        if self.input['use_symmetry'] and len(self.input['rotations'])==0:
+        if self.input["use_symmetry"] and len(self.input["rotations"]) == 0:
             self._get_rotation_matrices()
-        if len(self.input['strain_matrices'])==0:
+        if len(self.input["strain_matrices"]) == 0:
             self._create_strain_matrices()
-        if self.input['polynomial_order']<2:
-            raise ValueError('Minimum polynomial order: 2')
-        if (self.input['polynomial_order']==2
-            and self.input['additional_points']>0):
-            warnings.warn('Setting additional points in harmonic calculations'
-                + ' only increases the number of calculations')
-        if (self.input['polynomial_order']==2
-            and self.input['normalize_magnitude']):
-            warnings.warn('Magnitude normalization could reduce accuracy in'
-                + ' harmonic calculations')
-        if (self.input['polynomial_order']>2
-            and not self.input['normalize_magnitude']):
-            warnings.warn('Not normalizing magnitude could destabilise fit')
-        if self.input['fit_first_order']:
-            warnings.warn('First order fit does not correct the second order'
-                          + ' coefficients in the current implementation')
+        if self.input["polynomial_order"] < 2:
+            raise ValueError("Minimum polynomial order: 2")
+        if self.input["polynomial_order"] == 2 and self.input["additional_points"] > 0:
+            warnings.warn(
+                "Setting additional points in harmonic calculations"
+                + " only increases the number of calculations"
+            )
+        if self.input["polynomial_order"] == 2 and self.input["normalize_magnitude"]:
+            warnings.warn(
+                "Magnitude normalization could reduce accuracy in"
+                + " harmonic calculations"
+            )
+        if self.input["polynomial_order"] > 2 and not self.input["normalize_magnitude"]:
+            warnings.warn("Not normalizing magnitude could destabilise fit")
+        if self.input["fit_first_order"]:
+            warnings.warn(
+                "First order fit does not correct the second order"
+                + " coefficients in the current implementation"
+            )
 
     def collect_output(self):
         output_data = defaultdict(list)
         if self.ref_job.server.run_mode.interactive:
             job = self.project_hdf5.inspect(self.child_ids[0])
-            for key in ['energy_tot', 'energy_pot', 'pressures', 'volume']:
+            for key in ["energy_tot", "energy_pot", "pressures", "volume"]:
                 if key in job["output/generic"].list_nodes():
                     output_data[key] = job["output/generic/{}".format(key)]
         else:
             job_list = [self.project_hdf5.inspect(job_id) for job_id in self.child_ids]
-            output_data['id'] = self.child_ids
-            for key in ['energy_tot', 'energy_pot', 'pressures', 'volume']:
+            output_data["id"] = self.child_ids
+            for key in ["energy_tot", "energy_pot", "pressures", "volume"]:
                 if all(key in job["output/generic"].list_nodes() for job in job_list):
-                    output_data[key] = np.array([
-                        job["output/generic/{}".format(key)][-1] for job in job_list
-                    ])
-        energy = output_data['energy_tot']
-        if len(output_data['energy_pot'])==len(output_data['volume']):
-            energy = output_data['energy_pot']
+                    output_data[key] = np.array(
+                        [job["output/generic/{}".format(key)][-1] for job in job_list]
+                    )
+        energy = output_data["energy_tot"]
+        if len(output_data["energy_pot"]) == len(output_data["volume"]):
+            energy = output_data["energy_pot"]
+        if not self.input["use_pressure"]:
+            output_data["pressures"] = []
         elastic_tensor, score = calc_elastic_tensor(
-            strain=self.input['strain_matrices'],
-            stress=-np.array(output_data['pressures']),
-            rotations=self.input['rotations'],
+            strain=self.input["strain_matrices"],
+            stress=-np.array(output_data["pressures"]),
+            rotations=self.input["rotations"],
             energy=energy,
-            volume=output_data['volume'],
+            volume=output_data["volume"],
             return_score=True,
-            fit_first_order=self.input['fit_first_order'],
-            max_polynomial_order=self.input['polynomial_order'],
+            fit_first_order=self.input["fit_first_order"],
+            max_polynomial_order=self.input["polynomial_order"],
         )
-        output_data['fit_score'] = score
-        output_data['elastic_tensor'] = elastic_tensor
+        output_data["fit_score"] = score
+        output_data["elastic_tensor"] = elastic_tensor
         with self.project_hdf5.open("output") as hdf5_out:
             for key, val in output_data.items():
                 hdf5_out[key] = val
 
     def get_elastic_tensor_by_orientation(self, orientation):
         """
         Get elastic tensor in given orientation.
         Args:
             orientation (numpy.ndarray): 3x3 orientation tensor (e.g. [[1,1,1],[-1,0,1],[1,-2,1]])
         Returns:
             elastic tensor in the given orientation
         """
-        return get_elastic_tensor_by_orientation(orientation, self['output/elastic_tensor'])
+        return get_elastic_tensor_by_orientation(
+            orientation, self["output/elastic_tensor"]
+        )
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/murnaghan.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/murnaghan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from __future__ import print_function
+from typing import Optional, Literal
 
+import matplotlib.pyplot as plt
 import numpy as np
+import scipy.constants
 import scipy.integrate
 import scipy.optimize as spy
-import scipy.constants
-import warnings
-from pyiron_atomistics.atomistics.structure.atoms import Atoms, ase_to_pyiron
+
 from pyiron_atomistics.atomistics.master.parallel import AtomisticParallelMaster
+from pyiron_atomistics.atomistics.structure.atoms import Atoms, ase_to_pyiron
 from pyiron_base import JobGenerator
 
 __author__ = "Joerg Neugebauer, Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -27,33 +29,33 @@
 
 eV_div_A3_to_GPa = (
     1e21 / scipy.constants.physical_constants["joule-electron volt relationship"][0]
 )
 
 
 def _debye_kernel(xi):
-    return xi ** 3 / (np.exp(xi) - 1)
+    return xi**3 / (np.exp(xi) - 1)
 
 
 def debye_integral(x):
     return scipy.integrate.quad(_debye_kernel, 0, x)[0]
 
 
 def debye_function(x):
     if hasattr(x, "__len__"):
-        return np.array([3 / xx ** 3 * debye_integral(xx) for xx in x])
-    return 3 / x ** 3 * debye_integral(x)
+        return np.array([3 / xx**3 * debye_integral(xx) for xx in x])
+    return 3 / x**3 * debye_integral(x)
 
 
 # https://gitlab.com/ase/ase/blob/master/ase/eos.py
 def birchmurnaghan_energy(V, E0, B0, BP, V0):
     "BirchMurnaghan equation from PRB 70, 224107"
     eta = (V0 / V) ** (1 / 3)
-    return E0 + 9 * B0 * V0 / 16 * (eta ** 2 - 1) ** 2 * (
-        6 + BP * (eta ** 2 - 1) - 4 * eta ** 2
+    return E0 + 9 * B0 * V0 / 16 * (eta**2 - 1) ** 2 * (
+        6 + BP * (eta**2 - 1) - 4 * eta**2
     )
 
 
 def vinet_energy(V, E0, B0, BP, V0):
     "Vinet equation from PRB 70, 224107"
     eta = (V / V0) ** (1 / 3)
     return E0 + 2 * B0 * V0 / (BP - 1) ** 2 * (
@@ -84,15 +86,15 @@
 
 
 def pouriertarantola(V, E0, B0, BP, V0):
     "Pourier-Tarantola equation from PRB 70, 224107"
     eta = (V / V0) ** (1 / 3)
     squiggle = -3 * np.log(eta)
 
-    E = E0 + B0 * V0 * squiggle ** 2 / 6 * (3 + squiggle * (BP - 2))
+    E = E0 + B0 * V0 * squiggle**2 / 6 * (3 + squiggle * (BP - 2))
     return E
 
 
 def fitfunction(parameters, vol, fittype="vinet"):
     """
     Fit the energy volume curve
 
@@ -231,15 +233,15 @@
     @property
     def debye_temperature(self):
         if self._debye_T is not None:
             return self._debye_T
 
         GPaTokBar = 10
         Ang3_to_Bohr3 = (
-            scipy.constants.angstrom ** 3
+            scipy.constants.angstrom**3
             / scipy.constants.physical_constants["Bohr radius"][0] ** 3
         )
         convert = 67.48  # conversion factor, Moruzzi Eq. (4)
         empirical = 0.617  # empirical factor, Moruzzi Eq. (6)
         gamma_low, gamma_high = 1, 2 / 3  # low/high T gamma
 
         out = self._murnaghan["output"]
@@ -287,37 +289,76 @@
         else:
             val = 9.0 / 8.0 * kB * debye_T + T * kB * (
                 3 * np.log(1 - np.exp(-debye_T / T)) - debye_function(debye_T / T)
             )
         atoms_per_cell = len(self._murnaghan.structure)
         return atoms_per_cell * val
 
+    @property
+    def publication(self):
+        return {
+            "debye_model": {
+                "Moruzzi1988": {
+                    "title": "Calculated thermal properties of metals",
+                    "author": ["Moruzzi, V. L.", "Janak, J. F.", "Schwarz, K"],
+                    "journal": "Phys. Rev. B",
+                    "volume": "37",
+                    "issue": "2",
+                    "pages": "790--799",
+                    "numpages": "0",
+                    "month": "jan",
+                    "publisher": "American Physical Society",
+                    "doi": "10.1103/PhysRevB.37.790",
+                    "url": "https://link.aps.org/doi/10.1103/PhysRevB.37.790",
+                }
+            }
+        }
+
+
+def _strain_axes(
+    structure: Atoms, axes: Literal["x", "y", "z"], volume_strain: float
+) -> Atoms:
+    """
+    Strain box along given axes to achieve given *volumetric* strain.
+
+    Returns a copy.
+    """
+    axes = np.array([a in axes for a in ("x", "y", "z")])
+    num_axes = sum(axes)
+    # formula calculates the strain along each axis to achieve the overall volumetric strain
+    # beware that: (1+e)**x - 1 != e**x
+    strains = axes * ((1 + volume_strain) ** (1.0 / num_axes) - 1)
+    return structure.apply_strain(strains, return_box=True)
+
 
 class MurnaghanJobGenerator(JobGenerator):
     @property
     def parameter_list(self):
         """
 
         Returns:
             (list)
         """
         parameter_lst = []
-        for strain in np.linspace(
-            1 - self._master.input["vol_range"],
-            1 + self._master.input["vol_range"],
-            int(self._master.input["num_points"]),
-        ):
-            basis = self._master.ref_job.structure.copy()
-            basis.set_cell(basis.cell * strain ** (1.0 / 3.0), scale_atoms=True)
-            parameter_lst.append([np.round(strain, 7), basis])
+        strains = self._master.input.get("strains")
+        if strains is None:
+            strains = np.linspace(
+                -self._master.input["vol_range"],
+                self._master.input["vol_range"],
+                int(self._master.input["num_points"]),
+            )
+        for strain in strains:
+            basis = _strain_axes(
+                self._master.structure, self._master.input["axes"], strain
+            )
+            parameter_lst.append([1 + np.round(strain, 7), basis])
         return parameter_lst
 
-    @staticmethod
-    def job_name(parameter):
-        return "strain_" + str(parameter[0]).replace(".", "_")
+    def job_name(self, parameter):
+        return "{}_{}".format(self._master.job_name, parameter[0]).replace(".", "_")
 
     def modify_job(self, job, parameter):
         job.structure = parameter[1]
         return job
 
 
 class EnergyVolumeFit(object):
@@ -502,15 +543,15 @@
             list: [E0, B0, BP, V0], [E0_err, B0_err, BP_err, V0_err]
         """
         vol_lst = np.array(volume_lst).flatten()
         eng_lst = np.array(energy_lst).flatten()
         a, b, c = np.polyfit(vol_lst, eng_lst, 2)
         v0 = -b / (2 * a)
         pfit_leastsq, perr_leastsq = fit_leastsq(
-            [a * v0 ** 2 + b * v0 + c, 2 * a * v0 * eV_div_A3_to_GPa, 4, v0],
+            [a * v0**2 + b * v0 + c, 2 * a * v0 * eV_div_A3_to_GPa, 4, v0],
             vol_lst,
             eng_lst,
             fittype,
         )
         return pfit_leastsq, perr_leastsq  # [e0, b0, bP, v0]
 
     @staticmethod
@@ -601,23 +642,24 @@
     >>> ref_job.structure = structure_of_your_choice
     >>> murn = ref_job.create_job('Murnaghan', 'murn')
     >>> murn.run()
 
     The minimum energy volume and bulk modulus are stored in `ref_job['output/equilibrium_volume']`
     and `ref_job['output/equilibrium_bulk_modulus/']`.
     """
-    def __init__(self, project, job_name="murnaghan"):
+
+    def __init__(self, project, job_name):
         """
 
         Args:
             project:
             job_name:
         """
         super(Murnaghan, self).__init__(project, job_name)
-        self.__name__ = "Murnaghan"
+
         self.__version__ = "0.3.0"
 
         # print ("h5_path: ", self.project_hdf5._h5_path)
 
         # define default input
         self.input["num_points"] = (11, "number of sample points")
         self.input["fit_type"] = (
@@ -625,22 +667,45 @@
             "['polynomial', 'birch', 'birchmurnaghan', 'murnaghan', 'pouriertarantola', 'vinet']",
         )
         self.input["fit_order"] = (3, "order of the fit polynom")
         self.input["vol_range"] = (
             0.1,
             "relative volume variation around volume defined by ref_ham",
         )
+        self.input["axes"] = (
+            ["x", "y", "z"],
+            "Axes along which the strain will be applied",
+        )
+        self.input["strains"] = (
+            None,
+            "List of strains that should be calculated.  If given vol_range and num_points take no effect.",
+        )
 
         self.debye_model = DebyeModel(self)
         self.fit_module = EnergyVolumeFit()
 
         self.fit_dict = None
         self._debye_T = None
         self._job_generator = MurnaghanJobGenerator(self)
 
+    def convergence_check(self) -> bool:
+        """
+        Checks if the Murnaghan job has cnverged or not
+
+        Note: Currently, a 3rd order polynomial is fit to check if there is any convergence
+
+        Returns:
+            bool: True if the calculation is converged
+        """
+        if super().convergence_check():
+            e_vol = self["output/equilibrium_volume"]
+            return e_vol is not None
+        else:
+            return False
+
     @property
     def fit(self):
         return self.debye_model
 
     @property
     def equilibrium_volume(self):
         return self.fit_dict["volume_eq"]
@@ -659,33 +724,35 @@
         return self._fit_eos_general(vol_erg_dic=vol_erg_dic, fittype="birchmurnaghan")
 
     def fit_vinet(self, vol_erg_dic=None):
         return self._fit_eos_general(vol_erg_dic=vol_erg_dic, fittype="vinet")
 
     def _final_struct_to_hdf(self):
         with self._hdf5.open("output") as hdf5:
-            structure = self.get_structure(iteration_step=-1)
+            structure = self.get_structure(frame=-1)
             if not isinstance(structure, Atoms):
                 structure = ase_to_pyiron(structure)
             structure.to_hdf(hdf5)
 
-    def _fit_eos_general(self, vol_erg_dic=None, fittype="birchmurnaghan"):
-        self._set_fit_module(vol_erg_dic=vol_erg_dic)
-        fit_dict = self.fit_module.fit_eos_general(fittype=fittype)
-        self.input["fit_type"] = fit_dict["fit_type"]
-        self.input["fit_order"] = 0
+    def _store_fit_in_hdf(self, fit_dict):
         with self.project_hdf5.open("input") as hdf5_input:
             self.input.to_hdf(hdf5_input)
         with self.project_hdf5.open("output") as hdf5:
             hdf5["equilibrium_energy"] = fit_dict["energy_eq"]
             hdf5["equilibrium_volume"] = fit_dict["volume_eq"]
             hdf5["equilibrium_bulk_modulus"] = fit_dict["bulkmodul_eq"]
             hdf5["equilibrium_b_prime"] = fit_dict["b_prime_eq"]
         self._final_struct_to_hdf()
 
+    def _fit_eos_general(self, vol_erg_dic=None, fittype="birchmurnaghan"):
+        self._set_fit_module(vol_erg_dic=vol_erg_dic)
+        fit_dict = self.fit_module.fit_eos_general(fittype=fittype)
+        self.input["fit_type"] = fit_dict["fit_type"]
+        self.input["fit_order"] = 0
+        self._store_fit_in_hdf(fit_dict=fit_dict)
         self.fit_dict = fit_dict
         return fit_dict
 
     def _fit_leastsq(self, volume_lst, energy_lst, fittype="birchmurnaghan"):
         return self.fit_module._fit_leastsq(
             volume_lst=volume_lst, energy_lst=energy_lst, fittype=fittype
         )
@@ -708,52 +775,52 @@
         self._set_fit_module(vol_erg_dic=vol_erg_dic)
         fit_dict = self.fit_module.fit_polynomial(fit_order=fit_order)
         if fit_dict is None:
             self._logger.warning("Minimum could not be found!")
         else:
             self.input["fit_type"] = fit_dict["fit_type"]
             self.input["fit_order"] = fit_dict["fit_order"]
-            with self.project_hdf5.open("input") as hdf5_input:
-                self.input.to_hdf(hdf5_input)
-            with self.project_hdf5.open("output") as hdf5:
-                hdf5["equilibrium_energy"] = fit_dict["energy_eq"]
-                hdf5["equilibrium_volume"] = fit_dict["volume_eq"]
-                hdf5["equilibrium_bulk_modulus"] = fit_dict["bulkmodul_eq"]
-                hdf5["equilibrium_b_prime"] = fit_dict["b_prime_eq"]
-            self._final_struct_to_hdf()
-
+            self._store_fit_in_hdf(fit_dict=fit_dict)
             self.fit_dict = fit_dict
         return fit_dict
 
     def list_structures(self):
         if self.ref_job.structure is not None:
             return [parameter[1] for parameter in self._job_generator.parameter_list]
         else:
             return []
 
+    def validate_ready_to_run(self):
+        axes = self.input["axes"]
+        if len(set(axes)) != len(axes):
+            raise ValueError('input["axes"] may not contain duplicate entries!')
+        if not (1 <= len(axes) <= 3):
+            raise ValueError('input["axes"] must contain one to three entries!')
+        if set(axes).union(["x", "y", "z"]) != {"x", "y", "z"}:
+            raise ValueError('input["axes"] entries must be one of "x", "y" or "z"!')
+
     def collect_output(self):
         if self.ref_job.server.run_mode.interactive:
             ham = self.project_hdf5.inspect(self.child_ids[0])
             erg_lst = ham["output/generic/energy_tot"]
             vol_lst = ham["output/generic/volume"]
             arg_lst = np.argsort(vol_lst)
 
             self._output["volume"] = vol_lst[arg_lst]
             self._output["energy"] = erg_lst[arg_lst]
         else:
             erg_lst, vol_lst, err_lst, id_lst = [], [], [], []
             for job_id in self.child_ids:
                 ham = self.project_hdf5.inspect(job_id)
-                print("job_id: ", job_id, ham.status)
                 if "energy_tot" in ham["output/generic"].list_nodes():
                     energy = ham["output/generic/energy_tot"][-1]
                 elif "energy_pot" in ham["output/generic"].list_nodes():
                     energy = ham["output/generic/energy_pot"][-1]
                 else:
-                    raise ValueError('Neither energy_pot or energy_tot was found.')
+                    raise ValueError("Neither energy_pot or energy_tot was found.")
                 volume = ham["output/generic/volume"][-1]
                 erg_lst.append(np.mean(energy))
                 err_lst.append(np.var(energy))
                 vol_lst.append(volume)
                 id_lst.append(job_id)
             vol_lst = np.array(vol_lst)
             erg_lst = np.array(erg_lst)
@@ -770,79 +837,140 @@
             for key, val in self._output.items():
                 hdf5_out[key] = val
         if self.input["fit_type"] == "polynomial":
             self.fit_polynomial(fit_order=self.input["fit_order"])
         else:
             self._fit_eos_general(fittype=self.input["fit_type"])
 
-    def plot(self, num_steps=100, plt_show=True):
-        try:
-            import matplotlib.pylab as plt
-        except ImportError:
-            import matplotlib.pyplot as plt
+    def plot(
+        self,
+        per_atom: bool = False,
+        num_steps: int = 100,
+        plt_show: bool = True,
+        ax=None,
+        plot_kwargs: Optional[dict] = None,
+    ):
+        """
+        Plot E-V curve.
+
+        Args:
+            per_atom (optional, bool): normalize energy and volume by number of atoms in structure before plotting
+            num_steps (optional, int): number of sample points to interpolate the calculated values on
+            plt_show (optional, bool): call `matplotlib.pyplot.show()` after plotting (only necessary when running pyiron from scripts)
+            ax (optional, plt.Axes): if given plot onto this axis, otherwise create new figure for the plot
+            plot_kwargs (optional, dict): arguments passed verbatim to `matplotlib.pyplot.plot()`
+
+        Returns:
+            ax: The axis plotted onto
+
+        Raises:
+            ValueError: if job is not finished when calling this method
+        """
+        if not self.status.finished:
+            raise ValueError(
+                "Job must be successfully run, before calling this method."
+            )
+
+        if ax is None:
+            ax = plt.subplot(111)
+        else:
+            plt_show = False
         if not self.fit_dict:
             if self.input["fit_type"] == "polynomial":
                 self.fit_polynomial(fit_order=self.input["fit_order"])
             else:
                 self._fit_eos_general(fittype=self.input["fit_type"])
         df = self.output_to_pandas()
         vol_lst, erg_lst = df["volume"].values, df["energy"].values
         x_i = np.linspace(np.min(vol_lst), np.max(vol_lst), num_steps)
-        color = "blue"
 
+        if plot_kwargs is None:
+            plot_kwargs = {}
+
+        if "color" in plot_kwargs.keys():
+            color = plot_kwargs["color"]
+            del plot_kwargs["color"]
+        else:
+            color = "blue"
+
+        if "marker" in plot_kwargs.keys():
+            del plot_kwargs["marker"]
+
+        if "label" in plot_kwargs.keys():
+            label = plot_kwargs["label"]
+            del plot_kwargs["label"]
+        else:
+            label = self.input["fit_type"]
+
+        normalization = 1 if not per_atom else len(self.structure)
         if self.fit_dict is not None:
             if self.input["fit_type"] == "polynomial":
                 p_fit = np.poly1d(self.fit_dict["poly_fit"])
                 least_square_error = self.fit_module.get_error(vol_lst, erg_lst, p_fit)
-                plt.title("Murnaghan: error: " + str(least_square_error))
-                plt.plot(
-                    x_i,
-                    p_fit(x_i),
+                ax.set_title("Murnaghan: error: " + str(least_square_error))
+                ax.plot(
+                    x_i / normalization,
+                    p_fit(x_i) / normalization,
                     "-",
-                    label=self.input["fit_type"],
+                    label=label,
                     color=color,
                     linewidth=3,
+                    **plot_kwargs,
                 )
             else:
                 V0 = self.fit_dict["volume_eq"]
                 E0 = self.fit_dict["energy_eq"]
                 B0 = self.fit_dict["bulkmodul_eq"]
                 BP = self.fit_dict["b_prime_eq"]
-                eng_fit_lst = fitfunction(parameters=[E0, B0, BP, V0],
-                                          vol=x_i,
-                                          fittype=self.input["fit_type"])
-                plt.plot(
-                    x_i,
-                    eng_fit_lst,
+                eng_fit_lst = fitfunction(
+                    parameters=[E0, B0, BP, V0], vol=x_i, fittype=self.input["fit_type"]
+                )
+                ax.plot(
+                    x_i / normalization,
+                    eng_fit_lst / normalization,
                     "-",
-                    label=self.input["fit_type"],
+                    label=label,
                     color=color,
                     linewidth=3,
+                    **plot_kwargs,
                 )
 
-        plt.plot(vol_lst, erg_lst, "x", color=color, markersize=20)
-        plt.legend()
-        plt.xlabel("Volume ($\AA^3$)")
-        plt.ylabel("energy (eV)")
+        ax.plot(
+            vol_lst / normalization,
+            erg_lst / normalization,
+            "x",
+            color=color,
+            markersize=20,
+            **plot_kwargs,
+        )
+        ax.legend()
+        ax.set_xlabel("Volume ($\AA^3$)")
+        ax.set_ylabel("energy (eV)")
         if plt_show:
             plt.show()
+        return ax
 
-    def get_structure(self, iteration_step=-1):
+    def _get_structure(self, frame=-1, wrap_atoms=True):
         """
+        Gives original structure or final one with equilibrium volume.
 
-        Returns: Structure with equilibrium volume
+        Args:
+            iteration_step (int): if 0 return original structure; if 1/-1 structure with equilibrium volume
 
+        Returns:
+            :class:`pyiron_atomistics.atomistics.structure.atoms.Atoms`: requested structure
         """
-        if not (self.structure is not None):
-            raise AssertionError()
-        if iteration_step == -1:
-            snapshot = self.structure.copy()
-            old_vol = snapshot.get_volume()
+        if frame == 1:
+            old_vol = self.structure.get_volume()
             new_vol = self["output/equilibrium_volume"]
-            k = (new_vol / old_vol) ** (1.0 / 3.0)
-            new_cell = snapshot.cell * k
-            snapshot.set_cell(new_cell, scale_atoms=True)
-            return snapshot
-        elif iteration_step == 0:
+            vol_strain = new_vol / old_vol - 1
+            return _strain_axes(self.structure, self.input["axes"], vol_strain)
+        elif frame == 0:
             return self.structure
+
+    def _number_of_structures(self):
+        if self.structure is None:
+            return 0
+        elif not self.status.finished:
+            return 1
         else:
-            raise ValueError("iteration_step should be either 0 or -1.")
+            return 2
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/parallel.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/parallel.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,36 +37,54 @@
         if self.ref_job is not None:
             self._ref_job.structure = basis
         else:
             raise ValueError(
                 "A structure can only be set after a reference job has been assinged."
             )
 
-    def get_structure(self, iteration_step=-1):
-        if iteration_step == 0:
-            return self.structure
-        else:
-            raise ValueError("iteration_step should be either 0.")
+    def _get_structure(self, frame=0, wrap_atoms=True):
+        return self.structure
+
+    def _number_of_structures(self):
+        return 1
 
 
 class GenericOutput(OrderedDict):
     def __init__(self):
         super(GenericOutput, self).__init__()
 
 
 class MapMaster(AtomisticParallelMaster):
+    """
+    Atomistic parallel master job that computes a given function in the given arguments in parallel.
+
+    Example usage:
+
+    >>> master = self.create_job(
+    ...     job_type=self.project.job_type.MapMaster, job_name="map_" + self.job_name
+    ... )
+    >>> master.modify_function = function
+    >>> master.parameter_list = parameter_lst
+
+    or simpler
+
+    >>> master = job.map(function, parameter_lst)
+
+
+    """
+
     def __init__(self, project, job_name):
         """
 
         Args:
             project:
             job_name:
         """
         super(MapMaster, self).__init__(project, job_name)
-        self.__name__ = "MapMaster"
+
         self.__version__ = "0.0.1"
         self._job_generator = MapJobGenerator(self)
         self._map_function = None
         self.parameter_list = []
 
     @property
     def modify_function(self):
@@ -158,21 +176,25 @@
         project (pyiron.Project): Project to calculate pipeline in
         job (AtomisticGenericJob): Template for the calculation
         step_lst (list): List of functions which create calculations
 
     Returns:
         FlexibleMaster:
     """
-    job_lst_master = project.create_job(project.job_type.FlexibleMaster, job.job_name + '_lstmaster', delete_existing_job=delete_existing_job)
+    job_lst_master = project.create_job(
+        project.job_type.FlexibleMaster,
+        job.job_name + "_lstmaster",
+        delete_existing_job=delete_existing_job,
+    )
     if job_lst_master.status.finished:
         return job_lst_master
     else:
         for i, step_funct in enumerate(step_lst):
             job_lst_master.append(step_funct(job))
-            if i > 0 and 'for_each_structure' in step_funct.__name__:
+            if i > 0 and "for_each_structure" in step_funct.__name__:
                 job_lst_master.function_lst.append(_structure_many_to_many)
             elif i > 0:
                 job_lst_master.function_lst.append(_structure_one_to_one)
         return job_lst_master
 
 
 def _structure_one_to_one(job_prev, job_next):
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/phonopy.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/phonopy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import codecs
 import pickle
+from typing import Optional
 
 import numpy as np
 import posixpath
 import scipy.constants
 from phonopy import Phonopy
 from phonopy.structure.atoms import PhonopyAtoms
 from phonopy.units import VaspToTHz
 from phonopy.file_IO import write_FORCE_CONSTANTS
 
 from pyiron_atomistics.atomistics.structure.atoms import Atoms
 from pyiron_atomistics.atomistics.master.parallel import AtomisticParallelMaster
-from pyiron_atomistics.atomistics.structure.phonopy import publication as phonopy_publication
-from pyiron_base import JobGenerator, Settings
+from pyiron_atomistics.atomistics.structure.phonopy import (
+    publication as phonopy_publication,
+)
+from pyiron_base import state, JobGenerator, ImportAlarm, deprecate
 
 __author__ = "Jan Janssen, Yury Lysogorskiy"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "development"
 __date__ = "Sep 1, 2017"
 
-s = Settings()
-
 
 class Thermal:
     """
     Holds thermal properties that are the results of the phonopy calculation.
 
     Args:
         temperatures (ndarray): temperatures at which the other quantities are evaluated, units of Kelvin
         free_energies (ndarray): free energies in the quasi-harmonic approximation from phonon contributions, units of
                                  electron volts
         entropy (ndarray): vibrational entropy calculated from the above free energy
         cv (ndarray): heat capacity at constant volume, units of kJ/K/mol
     """
 
     def __init__(self, temperatures, free_energies, entropy, cv):
-
         self.temperatures = temperatures
         self.free_energies = free_energies
         self.entropy = entropy
         self.cv = cv
 
 
 def phonopy_to_atoms(ph_atoms):
@@ -60,15 +60,16 @@
 
     Returns: ASE-like Atoms object
 
     """
     return Atoms(
         symbols=list(ph_atoms.get_chemical_symbols()),
         positions=list(ph_atoms.get_positions()),
-        cell=list(ph_atoms.get_cell()), pbc=True
+        cell=list(ph_atoms.get_cell()),
+        pbc=True,
     )
 
 
 def atoms_to_phonopy(atom):
     """
     Convert ASE-like Atoms to Phonopy Atoms
     Args:
@@ -91,29 +92,37 @@
         """
 
         Returns:
             (list)
         """
         supercells = self._master.phonopy.get_supercells_with_displacements()
         return [
-            ["{}_{}".format(self._master.ref_job.job_name, ind), self._restore_magmoms(phonopy_to_atoms(sc))]
+            [
+                "{}_{}".format(self._master.ref_job.job_name, ind),
+                self._restore_magmoms(phonopy_to_atoms(sc)),
+            ]
             for ind, sc in enumerate(supercells)
         ]
 
     def _restore_magmoms(self, structure):
         """
         Args:
             structure (pyiron.atomistics.structure.atoms): input structure
 
         Returns:
             structure (pyiron_atomistics.atomistics.structure.atoms): output structure with magnetic moments
         """
         if any(self._master.structure.get_initial_magnetic_moments() != None):
             magmoms = self._master.structure.get_initial_magnetic_moments()
-            magmoms = np.tile(magmoms, np.prod(np.diagonal(self._master._phonopy_supercell_matrix())).astype(int))
+            magmoms = np.tile(
+                magmoms,
+                np.prod(np.diagonal(self._master._phonopy_supercell_matrix())).astype(
+                    int
+                ),
+            )
             structure.set_initial_magnetic_moments(magmoms)
         return structure
 
     @staticmethod
     def job_name(parameter):
         return parameter[0]
 
@@ -146,29 +155,36 @@
         for DFT instead of setting k-points directly).
     - The structure used in the reference job should be a relaxed structure.
     - Theory behind it: https://en.wikipedia.org/wiki/Quasi-harmonic_approximation
     """
 
     def __init__(self, project, job_name):
         super(PhonopyJob, self).__init__(project, job_name)
-        self.__name__ = "PhonopyJob"
+
         self.__version__ = "0.0.1"
         self.input["interaction_range"] = (10.0, "Minimal size of supercell, Ang")
         self.input["factor"] = (
             VaspToTHz,
             "Frequency unit conversion factor (default for VASP)",
         )
         self.input["displacement"] = (0.01, "atoms displacement, Ang")
         self.input["dos_mesh"] = (20, "mesh size for DOS calculation")
         self.input["primitive_matrix"] = None
+        self.input["number_of_snapshots"] = (
+            None,
+            "int or None, optional. Number of snapshots of supercells with random displacements. Random displacements "
+            "are generated displacing all atoms in random directions with a fixed displacement distance specified by "
+            "'distance' parameter, i.e., all atoms in supercell are displaced with the same displacement distance in "
+            "direct space. (Copied directly from phonopy docs. Requires the alm package to work.)",
+        )
 
         self.phonopy = None
         self._job_generator = PhonopyJobGenerator(self)
         self._disable_phonopy_pickle = False
-        s.publication_add(phonopy_publication())
+        state.publications.add(phonopy_publication())
 
     @property
     def phonopy_pickling_disabled(self):
         return self._disable_phonopy_pickle
 
     @phonopy_pickling_disabled.setter
     def phonopy_pickling_disabled(self, disable):
@@ -186,15 +202,18 @@
             if self.structure is not None:
                 self.phonopy = Phonopy(
                     unitcell=self._phonopy_unit_cell,
                     supercell_matrix=self._phonopy_supercell_matrix(),
                     primitive_matrix=self.input["primitive_matrix"],
                     factor=self.input["factor"],
                 )
-                self.phonopy.generate_displacements(distance=self.input["displacement"])
+                self.phonopy.generate_displacements(
+                    distance=self.input["displacement"],
+                    number_of_snapshots=self.input["number_of_snapshots"],
+                )
                 self.to_hdf()
             else:
                 raise ValueError("No reference job/ No reference structure found.")
 
     def list_structures(self):
         if self.structure is not None:
             self._enable_phonopy()
@@ -270,26 +289,28 @@
         else:
             pr_job = self.project_hdf5.project.open(self.job_name + "_hdf5")
             forces_lst = [
                 pr_job.inspect(job_name)["output/generic/forces"][-1]
                 for job_name in self._get_jobs_sorted()
             ]
         self.phonopy.set_forces(forces_lst)
-        self.phonopy.produce_force_constants()
+        self.phonopy.produce_force_constants(
+            fc_calculator=None if self.input["number_of_snapshots"] is None else "alm"
+        )
         self.phonopy.run_mesh(mesh=[self.input["dos_mesh"]] * 3)
         mesh_dict = self.phonopy.get_mesh_dict()
         self.phonopy.run_total_dos()
         dos_dict = self.phonopy.get_total_dos_dict()
 
         self.to_hdf()
 
         with self.project_hdf5.open("output") as hdf5_out:
-            hdf5_out["dos_total"] = dos_dict['total_dos']
-            hdf5_out["dos_energies"] = dos_dict['frequency_points']
-            hdf5_out["qpoints"] = mesh_dict['qpoints']
+            hdf5_out["dos_total"] = dos_dict["total_dos"]
+            hdf5_out["dos_energies"] = dos_dict["frequency_points"]
+            hdf5_out["qpoints"] = mesh_dict["qpoints"]
             hdf5_out["supercell_matrix"] = self._phonopy_supercell_matrix()
             hdf5_out["displacement_dataset"] = self.phonopy.get_displacement_dataset()
             hdf5_out[
                 "dynamical_matrix"
             ] = self.phonopy.dynamical_matrix.get_dynamical_matrix()
             hdf5_out["force_constants"] = self.phonopy.force_constants
 
@@ -314,15 +335,15 @@
 
         Returns:
 
         """
         unit_conversion = (
             scipy.constants.physical_constants["Hartree energy in eV"][0]
             / scipy.constants.physical_constants["Bohr radius"][0] ** 2
-            * scipy.constants.angstrom ** 2
+            * scipy.constants.angstrom**2
         )
         force_shape = np.shape(self.phonopy.force_constants)
         force_reshape = force_shape[0] * force_shape[2]
         return (
             np.transpose(self.phonopy.force_constants, (0, 2, 1, 3)).reshape(
                 (force_reshape, force_reshape)
             )
@@ -344,35 +365,33 @@
         Returns:
             :class:`Thermal`: thermal properties as returned by Phonopy
         """
         self.phonopy.run_thermal_properties(
             t_step=t_step, t_max=t_max, t_min=t_min, temperatures=temperatures
         )
         tp_dict = self.phonopy.get_thermal_properties_dict()
-        kJ_mol_to_eV = 1000/scipy.constants.Avogadro/scipy.constants.electron_volt
-        return Thermal(tp_dict['temperatures'],
-                       tp_dict['free_energy'] * kJ_mol_to_eV,
-                       tp_dict['entropy'],
-                       tp_dict['heat_capacity'])
+        kJ_mol_to_eV = 1000 / scipy.constants.Avogadro / scipy.constants.electron_volt
+        return Thermal(
+            tp_dict["temperatures"],
+            tp_dict["free_energy"] * kJ_mol_to_eV,
+            tp_dict["entropy"],
+            tp_dict["heat_capacity"],
+        )
 
     @property
     def dos_total(self):
         """
-
-        Returns:
-
+        ndarray of float: Value of the DOS.
         """
         return self["output/dos_total"]
 
     @property
     def dos_energies(self):
         """
-
-        Returns:
-
+        ndarray of float: Energies at which the DOS is sampled.
         """
         return self["output/dos_energies"]
 
     @property
     def dynamical_matrix(self):
         """
 
@@ -390,38 +409,51 @@
             q:
 
         Returns:
 
         """
         return np.real_if_close(self.phonopy.get_dynamical_matrix_at_q(q))
 
-    def plot_dos(self, ax=None, *args, **qwargs):
+    @deprecate(ax="Use axis instead")
+    def plot_dos(self, ax=None, *args, axis=None, **kwargs):
         """
+        Plot the DOS.
+
+        If "label" is present in `kwargs` a legend is added to the plot automatically.
 
         Args:
-            *args:
-            ax:
-            **qwargs:
+            axis (optional): matplotlib axis to use, if None create a new one
+            ax: deprecated alias for axis
+            *args: passed to `axis.plot`
+            **kwargs: passed to `axis.plot`
 
         Returns:
-
+            matplotlib.axes._subplots.AxesSubplot: axis with the plot
         """
         try:
             import pylab as plt
         except ImportError:
             import matplotlib.pyplot as plt
-        if ax is None:
-            fig, ax = plt.subplots(1, 1)
-        ax.plot(self["output/dos_energies"], self["output/dos_total"], *args, **qwargs)
-        ax.set_xlabel("Frequency [THz]")
-        ax.set_ylabel("DOS")
-        ax.set_title("Phonon DOS vs Energy")
+        if ax is not None and axis is None:
+            axis = ax
+        if axis is None:
+            _, axis = plt.subplots(1, 1)
+        axis.plot(
+            self["output/dos_energies"], self["output/dos_total"], *args, **kwargs
+        )
+        axis.set_xlabel("Frequency [THz]")
+        axis.set_ylabel("DOS")
+        axis.set_title("Phonon DOS vs Energy")
+        if "label" in kwargs:
+            axis.legend()
         return ax
 
-    def get_band_structure(self, npoints=101, with_eigenvectors=False, with_group_velocities=False):
+    def get_band_structure(
+        self, npoints=101, with_eigenvectors=False, with_group_velocities=False
+    ):
         """
         Calculate band structure with automatic path through reciprocal space.
 
         Can only be called after job is finished.
 
         Args:
             npoints (int, optional):  Number of sample points between high symmetry points.
@@ -440,38 +472,54 @@
             different length than other paths.  As compared to the phonopy output this method also reshapes the
             eigenvectors so that they directly have the same shape as the underlying structure.
 
         Raises:
             :exception:`ValueError`: method is called on a job that is not finished or aborted
         """
         if not self.status.finished:
-            raise ValueError("Job must be successfully run, before calling this method.")
+            raise ValueError(
+                "Job must be successfully run, before calling this method."
+            )
 
-        self.phonopy.auto_band_structure(npoints,
-                                        with_eigenvectors=with_eigenvectors,
-                                        with_group_velocities=with_group_velocities)
+        self.phonopy.auto_band_structure(
+            npoints,
+            with_eigenvectors=with_eigenvectors,
+            with_group_velocities=with_group_velocities,
+        )
         results = self.phonopy.get_band_structure_dict()
         if results["eigenvectors"] is not None:
             # see https://phonopy.github.io/phonopy/phonopy-module.html#eigenvectors for the way phonopy stores the
             # eigenvectors
-            results["eigenvectors"] = [e.transpose(0, 2, 1).reshape(*e.shape[:2], -1, 3) for e in results["eigenvectors"]]
+            results["eigenvectors"] = [
+                e.transpose(0, 2, 1).reshape(*e.shape[:2], -1, 3)
+                for e in results["eigenvectors"]
+            ]
         return results
 
-    def plot_band_structure(self, axis=None):
+    def plot_band_structure(
+        self, axis=None, *args, label: Optional[str] = None, **kwargs
+    ):
         """
-        Plot bandstructure calculated with :method:`.get_bandstructure`.
+        Plot bandstructure calculated with :meth:`.get_bandstructure`.
+
+        If :meth:`.get_bandstructure` hasn't been called before, it is automatically called with the default arguments.
 
-        If :method:`.get_bandstructure` hasn't been called before, it is automatically called with the default arguments.
+        If `label` is passed a legend is added automatically.
 
         Args:
             axis (matplotlib axis, optional): plot to this axis, if not given a new one is created.
+            *args: passed through to matplotlib.pyplot.plot when plotting the dispersion
+            label (str, optional): label for dispersion line
+            **kwargs: passed through to matplotlib.pyplot.plot when plotting the dispersion
 
         Returns:
             matplib axis: the axis the figure has been drawn to, if axis is given the same object is returned
         """
+        # label is it's own argument because if you try to pass it via **kwargs every line would get the label giving a
+        # messy legend
         try:
             import pylab as plt
         except ImportError:
             import matplotlib.pyplot as plt
 
         if axis is None:
             _, axis = plt.subplots(1, 1)
@@ -484,30 +532,50 @@
         distances = results["distances"]
         frequencies = results["frequencies"]
 
         # HACK: strictly speaking this breaks phonopy API and could bite us
         path_connections = self.phonopy._band_structure.path_connections
         labels = self.phonopy._band_structure.labels
 
+        if "color" not in kwargs:
+            kwargs["color"] = "black"
+
         offset = 0
         tick_positions = [distances[0][0]]
         for di, fi, ci in zip(distances, frequencies, path_connections):
-            axis.axvline(tick_positions[-1], color="black", linestyle="--")
-            axis.plot(offset + di, fi, color="black")
+            axis.axvline(
+                tick_positions[-1], color="black", linestyle="dotted", alpha=0.5
+            )
+            line, *_ = axis.plot(offset + di, fi, *args, **kwargs)
             tick_positions.append(di[-1] + offset)
             if not ci:
-                offset+=.05
-                plt.axvline(tick_positions[-1], color="black", linestyle="--")
+                offset += 0.05
+                axis.axvline(
+                    tick_positions[-1], color="black", linestyle="dotted", alpha=0.5
+                )
                 tick_positions.append(di[-1] + offset)
+        if label is not None:
+            line.set_label(label)
+            axis.legend()
         axis.set_xticks(tick_positions[:-1])
         axis.set_xticklabels(labels)
         axis.set_xlabel("Bandpath")
         axis.set_ylabel("Frequency [THz]")
         axis.set_title("Bandstructure")
         return axis
 
     def validate_ready_to_run(self):
         if self.ref_job._generic_input["calc_mode"] != "static":
-            raise ValueError("Phonopy reference jobs should be static calculations, but got {}".format(
-                self.ref_job._generic_input["calc_mode"]
-            ))
+            raise ValueError(
+                "Phonopy reference jobs should be static calculations, but got {}".format(
+                    self.ref_job._generic_input["calc_mode"]
+                )
+            )
+        if self.input["number_of_snapshots"] is not None:
+            with ImportAlarm(
+                "Phonopy with random snapshot displacement relies on the alm module but this unavailable. Please "
+                "ensure your python environment contains alm, e.g. by running `conda install -c conda-forge alm`."
+                "Note: at time of writing alm is only available for Linux and OSX systems."
+            ) as import_alarm:
+                import alm
+            import_alarm.warn_if_failed()
         super().validate_ready_to_run()
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/sqsmaster.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/convergence_encut_parallel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,99 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
-import numpy as np
+from __future__ import print_function
 from pyiron_atomistics.atomistics.master.parallel import AtomisticParallelMaster
 from pyiron_base import JobGenerator
+import numpy as np
+
+try:
+    import pylab as plt
+except (ImportError, RuntimeError):
+    try:
+        import matplotlib.pyplot as plt
+    except (ImportError, RuntimeError):
+        pass
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
-__version__ = "0.0.1"
+__version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "development"
-__date__ = "Oct 29, 2020"
-
-
-class SQSMaster(AtomisticParallelMaster):
-    def __init__(self, project, job_name):
-        super(SQSMaster, self).__init__(project, job_name)
-        self.__name__ = "SQSMaster"
-        self.__version__ = "0.0.1"
-        self.input["fraction_lst"] = []
-        self.input["species_one"] = ""
-        self.input["species_two"] = ""
-        self._job_generator = SQSJobGenerator(self)
-
-    def collect_output(self):
-        pass
-
-    @property
-    def list_of_structures(self):
-        return [self.project_hdf5.load(job_id).list_of_structures[0] for job_id in self.child_ids]
+__date__ = "Sep 1, 2017"
 
-    def list_structures(self):
-        return self.list_of_structures
 
-
-class SQSJobGenerator(JobGenerator):
+class EncutConvergenceJobGenerator(JobGenerator):
     @property
     def parameter_list(self):
         """
 
         Returns:
             (list)
         """
         return [
-            [
-                "sqs_" + str(np.round(f, 4)).replace(".", "_"),
-                {self._master.input["species_one"]: f, self._master.input["species_two"]: 1-f}
-            ]
-            for f in self._master.input["fraction_lst"]
+            np.round(encut, 7)
+            for encut in np.linspace(
+                self._master.input["min"],
+                self._master.input["max"],
+                self._master.input["num_points"],
+            )
         ]
 
     @staticmethod
     def job_name(parameter):
-        return parameter[0]
+        return "encut_" + str(parameter).replace(".", "_")
 
-    def modify_job(self, job, parameter):
-        job.input['mole_fractions'] = parameter[1]
+    @staticmethod
+    def modify_job(job, parameter):
+        job.set_encut(encut=parameter)
         return job
+
+
+# ToDo: not all abstract methods implemented
+class ConvEncutParallel(AtomisticParallelMaster):
+    def __init__(self, project, job_name="encut_conv"):
+        """
+
+        Args:
+            project:
+            job_name:
+        """
+        super(ConvEncutParallel, self).__init__(project, job_name)
+
+        self.__version__ = "0.0.1"
+
+        # define default input
+        self.input["num_points"] = (11, "number of sample points")
+        self.input["min"] = (200, "EnCut Minimum")
+        self.input["max"] = (800, "EnCut Maximum")
+        self._job_generator = EncutConvergenceJobGenerator(self)
+
+    def collect_output(self):
+        eng_lst, encut_lst = [], []
+        for job_id in self.child_ids:  # add iter_jobs (should behave like a project)
+            ham = self.project_hdf5.inspect(job_id)
+            print("job_id: ", job_id, ham.status)
+            eng_lst.append(ham["output/generic/energy_tot"][-1])
+            encut = ham.job_name.split("_")[1:]
+            encut_lst.append(float(encut[0] + "." + encut[1]))
+        arg_lst = np.argsort(encut_lst)
+        self._output["energy"] = eng_lst[arg_lst]
+        self._output["encut"] = encut_lst[arg_lst]
+
+        with self.project_hdf5.open("output") as hdf5_out:
+            for key, val in self._output.items():
+                hdf5_out[key] = val
+
+    def plot(self, plt_show=True):
+        df = self.output_to_pandas()
+        encut_lst, eng_lst = df["encut"], df["energy"]
+        plt.plot(encut_lst, eng_lst, "x-", markersize=20)
+        plt.xlabel("EnCut (eV)")
+        plt.ylabel("energy (eV)")
+        if plt_show:
+            plt.show()
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/structure.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/atom.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/atom.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
-from pyiron_atomistics.atomistics.structure.periodic_table import PeriodicTable, ChemicalElement
+from pyiron_atomistics.atomistics.structure.periodic_table import (
+    PeriodicTable,
+    ChemicalElement,
+)
 from pyiron_atomistics.atomistics.structure.sparse_list import SparseArrayElement
-from six import string_types
 from ase.atom import Atom as ASEAtom
 
 __author__ = "Sudarsan Surendralal"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -34,14 +36,15 @@
         charge (float): Charge in e
         atoms (ase.atoms.Atoms): Assigned atoms
         index (int): Assigned index
 
     .. _ASE atom class: https://wiki.fysik.dtu.dk/ase/ase/atom.html
 
     """
+
     def __init__(
         self,
         symbol="X",
         position=(0, 0, 0),
         tag=None,
         momentum=None,
         mass=None,
@@ -63,18 +66,15 @@
             pse = PeriodicTable()
 
         if element is None or element == "X":
             if "Z" in qwargs:
                 el_symbol = pse.atomic_number_to_abbreviation(qwargs["Z"])
                 self._lists["element"] = pse.element(el_symbol)
         else:
-            if isinstance(element, string_types):
-                el_symbol = element
-                self._lists["element"] = pse.element(el_symbol)
-            elif isinstance(element, str):
+            if isinstance(element, str):
                 el_symbol = element
                 self._lists["element"] = pse.element(el_symbol)
             elif isinstance(element, ChemicalElement):
                 self._lists["element"] = element
             else:
                 raise ValueError("Unknown element type")
 
@@ -86,28 +86,30 @@
                 position=position,
                 tag=tag,
                 momentum=momentum,
                 mass=mass,
                 magmom=magmom,
                 charge=charge,
                 atoms=atoms,
-                index=index)
+                index=index,
+            )
         except KeyError:
             symbol = pse.Parent[symbol]
             ASEAtom.__init__(
                 self,
                 symbol=symbol,
                 position=position,
                 tag=tag,
                 momentum=momentum,
                 mass=mass,
                 magmom=magmom,
                 charge=charge,
                 atoms=atoms,
-                index=index)
+                index=index,
+            )
 
         # ASE compatibility for tags
         for key, val in qwargs.items():
             self.data[key] = val
 
     @property
     def mass(self):
@@ -159,16 +161,18 @@
     Args:
         ase_obj(ase.atom.Atom): The ase atoms instance to convert
 
     Returns:
         pyiron.atomistics.structure.atom.Atom: The equivalent pyiron Atom
 
     """
-    return Atom(symbol=ase_obj.symbol,
-                position=ase_obj.position,
-                tag=ase_obj.tag,
-                momentum=ase_obj.momentum,
-                mass=ase_obj.mass,
-                magmom=ase_obj.magmom,
-                charge=ase_obj.charge,
-                atoms=ase_obj.atoms,
-                index=ase_obj.index)
+    return Atom(
+        symbol=ase_obj.symbol,
+        position=ase_obj.position,
+        tag=ase_obj.tag,
+        momentum=ase_obj.momentum,
+        mass=ase_obj.mass,
+        magmom=ase_obj.magmom,
+        charge=ase_obj.charge,
+        atoms=ase_obj.atoms,
+        index=ase_obj.index,
+    )
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/atoms.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/atoms.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,56 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from __future__ import division, print_function
 from ase.atoms import Atoms as ASEAtoms, Atom as ASEAtom
+from ase.symbols import Symbols as ASESymbols
 import ast
 from copy import copy
 from collections import OrderedDict
 import numpy as np
-from six import string_types
 import warnings
 import seekpath
-from pyiron_atomistics.atomistics.structure.atom import Atom, ase_to_pyiron as ase_to_pyiron_atom
-from pyiron_atomistics.atomistics.structure.neighbors import Neighbors, Tree
-from pyiron_atomistics.atomistics.structure._visualize import Visualize
+import importlib
+from structuretoolkit.analyse import (
+    get_symmetry,
+    get_neighbors,
+    get_neighborhood,
+    get_distances_array,
+    find_mic,
+)
+from structuretoolkit.common import center_coordinates_in_unit_cell
+from structuretoolkit.visualize import plot3d
+from pyiron_atomistics.atomistics.structure.atom import (
+    Atom,
+    ase_to_pyiron as ase_to_pyiron_atom,
+)
+from pyiron_atomistics.atomistics.structure.pyscal import pyiron_to_pyscal_system
 from pyiron_atomistics.atomistics.structure.analyse import Analyse
 from pyiron_atomistics.atomistics.structure.sparse_list import SparseArray, SparseList
 from pyiron_atomistics.atomistics.structure.periodic_table import (
     PeriodicTable,
-    ChemicalElement
+    ChemicalElement,
 )
-from pyiron_base import Settings, deprecate, deprecate_soon
-
-from scipy.spatial import cKDTree, Voronoi
-import spglib
+from pyiron_base import state, deprecate
+from pymatgen.io.ase import AseAtomsAdaptor
+from collections.abc import Sequence
 
 __author__ = "Joerg Neugebauer, Sudarsan Surendralal"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Sudarsan Surendralal"
 __email__ = "surendralal@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
-s = Settings()
-
 
 class Atoms(ASEAtoms):
     """
     The Atoms class represents all the information required to describe a structure at the atomic scale. This class is
     derived from the `ASE atoms class`_.
 
     Args:
@@ -81,15 +90,15 @@
         constraint=None,
         calculator=None,
         info=None,
         indices=None,
         elements=None,
         dimension=None,
         species=None,
-        **qwargs
+        **qwargs,
     ):
         if symbols is not None:
             if elements is None:
                 elements = symbols
             else:
                 raise ValueError("Only elements OR symbols should be given.")
         if (
@@ -98,18 +107,16 @@
             or masses is not None
             or charges is not None
             or celldisp is not None
             or constraint is not None
             or calculator is not None
             or info is not None
         ):
-            s.logger.debug("Not supported parameter used!")
+            state.logger.debug("Not supported parameter used!")
 
-        self._store_elements = dict()
-        self._species_to_index_dict = None
         self._is_scaled = False
 
         self._species = list()
         self.indices = np.array([])
         self.constraints = None
         self._pse = PeriodicTable()
         self._tag_list = SparseArray()
@@ -140,15 +147,15 @@
                         el_object_list = object_list
 
                 if len(elements) == 0:
                     element_list = elements
                 else:
                     if isinstance(elements[0], (list, tuple, np.ndarray)):
                         elements = np.array(elements).flatten()
-                    if isinstance(elements[0], string_types):
+                    if isinstance(elements[0], str):
                         element_list = elements
                     elif isinstance(elements[0], ChemicalElement):
                         el_object_list = elements
                     elif isinstance(elements[0], Atom):
                         el_object_list = [el.element for el in elements]
                         positions = [el.position for el in elements]
                     elif elements.dtype in [int, np.integer]:
@@ -158,83 +165,105 @@
                             "Unknown static type for element in list: "
                             + str(type(elements[0]))
                         )
 
             if el_object_list is None:
                 el_object_list = [self.convert_element(el) for el in element_list]
 
-            self.set_species(list(set(el_object_list)))
-            # species_to_index_dict = {el: i for i, el in enumerate(self.species)}
+            # Create a list from a set but always preserve order
+            self.set_species(list(dict.fromkeys(el_object_list)))
             el_index_lst = [self._species_to_index_dict[el] for el in el_object_list]
 
         elif indices is not None:
             el_index_lst = indices
+            if species is None:
+                raise ValueError(
+                    "species must be given if indices is given, but is None."
+                )
             self.set_species(species)
 
         self.indices = np.array(el_index_lst, dtype=int)
 
-        el_lst = [el.Abbreviation if el.Parent is None else el.Parent for el in self.species]
+        el_lst = [
+            el.Abbreviation if el.Parent is None else el.Parent for el in self.species
+        ]
         symbols = np.array([el_lst[el] for el in self.indices])
         self._tag_list._length = len(symbols)
-        super(Atoms, self).__init__(symbols=symbols, positions=positions, numbers=None,
-                                    tags=tags, momenta=momenta, masses=masses,
-                                    magmoms=magmoms, charges=charges,
-                                    scaled_positions=scaled_positions, cell=cell,
-                                    pbc=pbc, celldisp=celldisp, constraint=constraint,
-                                    calculator=calculator, info=info)
+        super(Atoms, self).__init__(
+            symbols=symbols,
+            positions=positions,
+            numbers=None,
+            tags=tags,
+            momenta=momenta,
+            masses=masses,
+            magmoms=magmoms,
+            charges=charges,
+            scaled_positions=scaled_positions,
+            cell=cell,
+            pbc=pbc,
+            celldisp=celldisp,
+            constraint=constraint,
+            calculator=calculator,
+            info=info,
+        )
 
         self.bonds = None
         self.units = {"length": "A", "mass": "u"}
-        self._symmetry_dataset = None
         self.set_initial_magnetic_moments(magmoms)
         self._high_symmetry_points = None
         self._high_symmetry_path = None
         self.dimension = dimension
         if len(self.positions) > 0:
             self.dimension = len(self.positions[0])
         else:
             self.dimension = 0
-        self._visualize = Visualize(self)
         self._analyse = Analyse(self)
+        # Velocities were not handled at all during file writing
+        self._velocities = None
+
+    def __setstate__(self, state):
+        self.__dict__.update(state)
+
+    def __getstate__(self):
+        # Only necessary to support pickling in python <3.11
+        # https://docs.python.org/release/3.11.2/library/pickle.html#object.__getstate__
+        return self.__dict__
+
+    @property
+    def velocities(self):
+        return self._velocities
+
+    @velocities.setter
+    def velocities(self, val):
+        if self.positions.shape == val.shape:
+            self._velocities = val
+        else:
+            raise ValueError(
+                f"Shape of velocities and positions has to match. Velocities shape: {val.shape}, positions shape: {self.positions.shape}"
+            )
 
     @property
     def spins(self):
         """
         Magnetic spins for each atom in the structure
 
         Returns:
             numpy.ndarray/list: The magnetic moments for reach atom as a single value or a vector (non-collinear spins)
 
         """
         if self.has("initial_magmoms"):
             return self.arrays["initial_magmoms"]
         else:
-            return
+            raise AttributeError("'Atoms' object has no attribute 'spins'")
 
     @spins.setter
     def spins(self, val):
+        self.set_array("initial_magmoms", None)
         if val is not None:
-            val = np.asarray(val)
-            if self.has("initial_magmoms"):
-                try:
-                    self.arrays["initial_magmoms"][:] = val
-                except ValueError as err:
-                    if len(self.arrays["initial_magmoms"]) == len(val):
-                        self.set_array('initial_magmoms', None)
-                        self.arrays["initial_magmoms"] = val
-                    else:
-                        raise err
-            else:
-                self.new_array("initial_magmoms", val)
-        else:
-            self.set_array('initial_magmoms', None)
-
-    @property
-    def visualize(self):
-        return self._visualize
+            self.set_array("initial_magmoms", np.asarray(val))
 
     @property
     def analyse(self):
         return self._analyse
 
     @property
     def species(self):
@@ -249,20 +278,41 @@
         """
         Setting the species list
 
         Args:
             value (list): A list atomistics.structure.periodic_table.ChemicalElement instances
 
         """
-        if value is None:
-            return
-        value = list(value)
-        self._species_to_index_dict = {el: i for i, el in enumerate(value)}
-        self._species = value[:]
-        self._store_elements = {el.Abbreviation: el for el in value}
+        if value is not None:
+            self._species = list(value)[:]
+
+    @property
+    def _store_elements(self) -> dict:
+        return {el.Abbreviation: el for el in self.species}
+
+    @property
+    def _species_to_index_dict(self) -> dict:
+        return {el: i for i, el in enumerate(self.species)}
+
+    @property
+    def symbols(self):
+        """
+        Get chemical symbols as a :class:`ase.symbols.Symbols` object.
+
+        The object works like ``atoms.numbers`` except its values
+        are strings.  It supports in-place editing.
+        """
+        sym_obj = Symbols(self.numbers)
+        sym_obj.structure = self
+        return sym_obj
+
+    @symbols.setter
+    def symbols(self, obj):
+        new_symbols = Symbols.fromsymbols(obj)
+        self.numbers[:] = new_symbols.numbers
 
     @property
     def elements(self):
         """
         numpy.ndarray: A size N list of atomistics.structure.periodic_table.ChemicalElement instances according
                        to the ordering of the atoms in the instance
 
@@ -293,15 +343,17 @@
         """
         Adds new points to the dict of existing high symmetry points.
 
         Args:
             new_points (dict): Points to add
         """
         if self.get_high_symmetry_points() is None:
-            raise AssertionError("Construct high symmetry points first. Use self.create_line_mode_structure().")
+            raise AssertionError(
+                "Construct high symmetry points first. Use self.create_line_mode_structure()."
+            )
         else:
             self._high_symmetry_points.update(new_points)
 
     def get_high_symmetry_path(self):
         """
         Path used for band structure calculations
 
@@ -326,40 +378,46 @@
         Adds a new path to the dictionary of pathes for band structure calculations.
 
         Args:
             path (dict): dictionary of lists of tuples with start and end point.
                 E.G. {"my_path": [('Gamma', 'X'), ('X', 'Y')]}
         """
         if self.get_high_symmetry_path() is None:
-            raise AssertionError("Construct high symmetry path first. Use self.create_line_mode_structure().")
+            raise AssertionError(
+                "Construct high symmetry path first. Use self.create_line_mode_structure()."
+            )
 
         for values_all in path.values():
             for values in values_all:
                 if not len(values) == 2:
                     raise ValueError(
                         "'{}' is not a propper trace! It has to contain exactly 2 values! (start and end point)".format(
-                            values))
+                            values
+                        )
+                    )
                 for v in values:
                     if v not in self.get_high_symmetry_points().keys():
-                        raise ValueError("'{}' is not a valid high symmetry point".format(v))
+                        raise ValueError(
+                            "'{}' is not a valid high symmetry point".format(v)
+                        )
 
         self._high_symmetry_path.update(path)
 
-    def add_tag(self, *args, **qwargs):
+    def add_tag(self, **qwargs):
         """
         Add tags to the atoms object.
 
         Examples:
 
             For selective dynamics::
 
             >>> self.add_tag(selective_dynamics=[False, False, False])
 
         """
-        self._tag_list.add_tag(*args, **qwargs)
+        self._tag_list.add_tag(**qwargs)
 
     # @staticmethod
     def numbers_to_elements(self, numbers):
         """
         Convert atomic numbers in element objects (needed for compatibility with ASE)
 
         Args:
@@ -394,15 +452,14 @@
             hdf (pyiron_base.generic.hdfio.FileHDFio): HDF path to which the object is to be saved
             group_name (str):
                 Group name with which the object should be stored. This same name should be used to retrieve the object
 
         """
         # import time
         with hdf.open(group_name) as hdf_structure:
-            # time_start = time.time()
             hdf_structure["TYPE"] = str(type(self))
             for el in self.species:
                 if isinstance(el.tags, dict):
                     with hdf_structure.open("new_species") as hdf_species:
                         el.to_hdf(hdf_species)
             hdf_structure["species"] = [el.Abbreviation for el in self.species]
             hdf_structure["indices"] = self.indices
@@ -419,29 +476,36 @@
                 with hdf_structure.open("cell") as hdf_cell:
                     # Convert ASE cell object to numpy array before storing
                     hdf_cell["cell"] = np.array(self.cell)
                     hdf_cell["pbc"] = self.pbc
 
             # hdf_structure["coordinates"] = self.positions  # "Atomic coordinates"
             hdf_structure["positions"] = self.positions  # "Atomic coordinates"
-            hdf_structure["spins"] = self.spins
+            if self.has("initial_magmoms"):
+                hdf_structure["spins"] = self.spins
             # potentials with explicit bonds (TIP3P, harmonic, etc.)
             if self.bonds is not None:
                 hdf_structure["explicit_bonds"] = self.bonds
 
-            # print ('time in atoms.to_hdf: ', time.time() - time_start)
-
             if self._high_symmetry_points is not None:
                 hdf_structure["high_symmetry_points"] = self._high_symmetry_points
 
             if self._high_symmetry_path is not None:
                 hdf_structure["high_symmetry_path"] = self._high_symmetry_path
 
             hdf_structure["info"] = self.info
 
+            if self.calc is not None:
+                calc_dict = self.calc.todict()
+                calc_dict["label"] = self.calc.label
+                calc_dict["class"] = (
+                    self.calc.__class__.__module__ + "." + self.calc.__class__.__name__
+                )
+                hdf_structure["calculator"] = calc_dict
+
     def from_hdf(self, hdf, group_name="structure"):
         """
         Retrieve the object from a HDF5 file
 
         Args:
             hdf (pyiron_base.generic.hdfio.FileHDFio): HDF path to which the object is to be saved
             group_name (str): Group name from which the Atoms object is retreived.
@@ -474,23 +538,22 @@
                         self.cell = hdf_cell["cell"]
                         self.pbc = hdf_cell["pbc"]
 
                 # Backward compatibility
                 position_tag = "positions"
                 if position_tag not in hdf_atoms.list_nodes():
                     position_tag = "coordinates"
-                if "is_absolute" in hdf_atoms.list_nodes():
-                    if not tr_dict[hdf_atoms["is_absolute"]]:
-                        self.set_scaled_positions(hdf_atoms[position_tag])
-                    else:
-                        self.arrays['positions'] = hdf_atoms[position_tag]
-                else:
-                    self.arrays['positions'] = hdf_atoms[position_tag]
+                self.arrays["positions"] = hdf_atoms[position_tag]
+                if (
+                    "is_absolute" in hdf_atoms.list_nodes()
+                    and not tr_dict[hdf_atoms["is_absolute"]]
+                ):
+                    self.set_scaled_positions(self.arrays["positions"])
 
-                self.arrays['numbers'] = self.get_atomic_numbers()
+                self.arrays["numbers"] = self.get_atomic_numbers()
 
                 if "explicit_bonds" in hdf_atoms.list_nodes():
                     # print "bonds: "
                     self.bonds = hdf_atoms["explicit_bonds"]
                 if "spins" in hdf_atoms.list_nodes():
                     self.spins = hdf_atoms["spins"]
                 if "tags" in hdf_atoms.list_groups():
@@ -524,14 +587,22 @@
                     self._high_symmetry_points = hdf_atoms["high_symmetry_points"]
 
                 self._high_symmetry_path = None
                 if "high_symmetry_path" in hdf_atoms.list_nodes():
                     self._high_symmetry_path = hdf_atoms["high_symmetry_path"]
                 if "info" in hdf_atoms.list_nodes():
                     self.info = hdf_atoms["info"]
+                if "calculator" in hdf_atoms:
+                    calc_dict = hdf_atoms["calculator"]
+                    class_path = calc_dict.pop("class")
+                    calc_module = importlib.import_module(
+                        ".".join(class_path.split(".")[:-1])
+                    )
+                    calc_class = getattr(calc_module, class_path.split(".")[-1])
+                    self.calc = calc_class(**calc_dict)
                 return self
 
         else:
             return self._from_hdf_old(hdf, group_name)
 
     def _from_hdf_old(self, hdf, group_name="structure"):
         """
@@ -652,26 +723,25 @@
 
             atomistics.structure.periodictable.ChemicalElement: The required chemical element
 
         """
         if el in list(self._store_elements.keys()):
             return self._store_elements[el]
 
-        if isinstance(el, string_types):  # as symbol
+        if isinstance(el, str):  # as symbol
             element = Atom(el, pse=pse).element
         elif isinstance(el, Atom):
             element = el.element
             el = el.element.Abbreviation
         elif isinstance(el, ChemicalElement):
             element = el
             el = el.Abbreviation
         else:
             raise ValueError("Unknown static type to specify a element")
 
-        self._store_elements[el] = element
         if hasattr(self, "species"):
             if element not in self.species:
                 self._species.append(element)
                 self.set_species(self._species)
         return element
 
     def get_chemical_formula(self):
@@ -695,15 +765,15 @@
         """
         Returns the list of chemical indices as ordered in self.species
 
         Returns:
             numpy.ndarray: A list of chemical indices
 
         """
-        return self.indices
+        return self.indices.copy()
 
     def get_atomic_numbers(self):
         """
         Returns the atomic numbers of all the atoms in the structure
 
         Returns:
             numpy.ndarray: A list of atomic numbers
@@ -918,47 +988,46 @@
 
         Returns:
 
             numpy.ndarray: Wrapped positions
 
         """
         scaled_positions = np.einsum(
-            'ji,nj->ni', np.linalg.inv(self.cell), np.asarray(positions).reshape(-1, 3)
+            "ji,nj->ni", np.linalg.inv(self.cell), np.asarray(positions).reshape(-1, 3)
         )
         if any(self.pbc):
-            scaled_positions[:, self.pbc] -= np.floor(scaled_positions[:, self.pbc]+epsilon)
-        new_positions = np.einsum('ji,nj->ni', self.cell, scaled_positions)
+            scaled_positions[:, self.pbc] -= np.floor(
+                scaled_positions[:, self.pbc] + epsilon
+            )
+        new_positions = np.einsum("ji,nj->ni", self.cell, scaled_positions)
         return new_positions.reshape(np.asarray(positions).shape)
 
     def center_coordinates_in_unit_cell(self, origin=0, eps=1e-4):
         """
-        Wrap atomic coordinates within the supercell as given by a1, a2., a3
+        Wrap atomic coordinates within the supercell.
+
+        Modifies object in place and returns itself.
 
         Args:
             origin (float):  0 to confine between 0 and 1, -0.5 to confine between -0.5 and 0.5
             eps (float): Tolerance to detect atoms at cell edges
 
         Returns:
-
-            pyiron.atomistics.structure.atoms.Atoms: Wrapped structure
-
+            :class:`pyiron_atomistics.atomistics.structure.atoms.Atoms`: reference to this structure
         """
-        if any(self.pbc):
-            self.set_scaled_positions(
-                np.mod(self.get_scaled_positions(wrap=False) + eps, 1) - eps + origin
-            )
-        return self
+        return center_coordinates_in_unit_cell(structure=self, origin=origin, eps=eps)
 
-    def create_line_mode_structure(self,
-                                   with_time_reversal=True,
-                                   recipe='hpkot',
-                                   threshold=1e-07,
-                                   symprec=1e-05,
-                                   angle_tolerance=-1.0,
-                                   ):
+    def create_line_mode_structure(
+        self,
+        with_time_reversal=True,
+        recipe="hpkot",
+        threshold=1e-07,
+        symprec=1e-05,
+        angle_tolerance=-1.0,
+    ):
         """
         Uses 'seekpath' to create a new structure with high symmetry points and path for band structure calculations.
 
         Args:
             with_time_reversal (bool): if False, and the group has no inversion symmetry,
                 additional lines are returned as described in the HPKOT paper.
             recipe (str): choose the reference publication that defines the special points and paths.
@@ -970,46 +1039,38 @@
             symprec (float): the symmetry precision used internally by SPGLIB
             angle_tolerance (float): the angle_tolerance used internally by SPGLIB
 
         Returns:
             pyiron.atomistics.structure.atoms.Atoms: new structure
         """
         input_structure = (self.cell, self.get_scaled_positions(), self.indices)
-        sp_dict = seekpath.get_path(structure=input_structure,
-                                    with_time_reversal=with_time_reversal,
-                                    recipe=recipe,
-                                    threshold=threshold,
-                                    symprec=symprec,
-                                    angle_tolerance=angle_tolerance,
-                                    )
+        sp_dict = seekpath.get_path(
+            structure=input_structure,
+            with_time_reversal=with_time_reversal,
+            recipe=recipe,
+            threshold=threshold,
+            symprec=symprec,
+            angle_tolerance=angle_tolerance,
+        )
 
         original_element_list = [el.Abbreviation for el in self.species]
         element_list = [original_element_list[l] for l in sp_dict["primitive_types"]]
         positions = sp_dict["primitive_positions"]
         pbc = self.pbc
         cell = sp_dict["primitive_lattice"]
 
-        struc_new = Atoms(elements=element_list, scaled_positions=positions, pbc=pbc, cell=cell)
+        struc_new = Atoms(
+            elements=element_list, scaled_positions=positions, pbc=pbc, cell=cell
+        )
 
         struc_new._set_high_symmetry_points(sp_dict["point_coords"])
         struc_new._set_high_symmetry_path({"full": sp_dict["path"]})
 
         return struc_new
 
-    def repeat(self, rep):
-        """Create new repeated atoms object.
-
-        The *rep* argument should be a sequence of three positive
-        integers like *(2,3,1)* or a single integer (*r*) equivalent
-        to *(r,r,r)*."""
-
-        atoms = self.copy()
-        atoms *= rep
-        return atoms
-
     def set_repeat(self, vec):
         self *= vec
 
     def repeat_points(self, points, rep, centered=False):
         """
         Return points with repetition given according to periodic boundary conditions
 
@@ -1021,90 +1082,124 @@
             centered (bool): Whether the original points should be in the center of
                              repeated points.
 
         Returns:
             (np.ndarray) repeated points
         """
         n = np.array([rep]).flatten()
-        if len(n)==1:
+        if len(n) == 1:
             n = np.tile(n, 3)
-        if len(n)!=3:
-            raise ValueError('rep must be an integer or a list of 3 integers')
+        if len(n) != 3:
+            raise ValueError("rep must be an integer or a list of 3 integers")
         vector = np.array(points)
-        if vector.shape[-1]!=3:
-            raise ValueError('points must be an xyz vector or a list/array of xyz vectors')
-        if centered and np.mod(n, 2).sum()!=3:
-            warnings.warn('When centered, only odd number of repetition should be used')
+        if vector.shape[-1] != 3:
+            raise ValueError(
+                "points must be an xyz vector or a list/array of xyz vectors"
+            )
+        if centered and np.mod(n, 2).sum() != 3:
+            warnings.warn("When centered, only odd number of repetition should be used")
         v = vector.reshape(-1, 3)
         n_lst = []
         for nn in n:
             if centered:
-                n_lst.append(np.arange(nn)-int(nn/2))
+                n_lst.append(np.arange(nn) - int(nn / 2))
             else:
                 n_lst.append(np.arange(nn))
         meshgrid = np.meshgrid(n_lst[0], n_lst[1], n_lst[2])
-        v_repeated = np.einsum('ni,ij->nj', np.stack(meshgrid, axis=-1).reshape(-1, 3), self.cell)
-        v_repeated = v_repeated[:, np.newaxis, :]+v[np.newaxis, :, :]
-        return v_repeated.reshape((-1,)+vector.shape)
+        v_repeated = np.einsum(
+            "ni,ij->nj", np.stack(meshgrid, axis=-1).reshape(-1, 3), self.cell
+        )
+        v_repeated = v_repeated[:, np.newaxis, :] + v[np.newaxis, :, :]
+        return v_repeated.reshape((-1,) + vector.shape)
 
     def reset_absolute(self, is_absolute):
         raise NotImplementedError("This function was removed!")
 
-    @deprecate("Use Atoms.analyse.pyscal_cna_adaptive() with ovito_compatibility=True instead")
+    @deprecate(
+        "Use Atoms.analyse.pyscal_cna_adaptive() with ovito_compatibility=True instead"
+    )
     def analyse_ovito_cna_adaptive(self, mode="total"):
         return self._analyse.pyscal_cna_adaptive(mode=mode, ovito_compatibility=True)
+
     analyse_ovito_cna_adaptive.__doc__ = Analyse.pyscal_cna_adaptive.__doc__
 
-    @deprecate('Use Atoms.analyse.pyscal_centro_symmetry() instead')
+    @deprecate("Use Atoms.analyse.pyscal_centro_symmetry() instead")
     def analyse_ovito_centro_symmetry(self, num_neighbors=12):
         return self._analyse.pyscal_centro_symmetry(num_neighbors=num_neighbors)
+
     analyse_ovito_centro_symmetry.__doc__ = Analyse.pyscal_centro_symmetry.__doc__
 
     @deprecate("Use Atoms.analyse.pyscal_voronoi_volume() instead")
     def analyse_ovito_voronoi_volume(self):
         return self._analyse.pyscal_voronoi_volume()
+
     analyse_ovito_voronoi_volume.__doc__ = Analyse.pyscal_voronoi_volume.__doc__
 
     @deprecate("Use Atoms.analyse.pyscal_steinhardt_parameter() instead")
-    def analyse_pyscal_steinhardt_parameter(self, neighbor_method="cutoff", cutoff=0, n_clusters=2,
-                                            q=(4, 6), averaged=False, clustering=True):
+    def analyse_pyscal_steinhardt_parameter(
+        self,
+        neighbor_method="cutoff",
+        cutoff=0,
+        n_clusters=2,
+        q=(4, 6),
+        averaged=False,
+        clustering=True,
+    ):
         return self._analyse.pyscal_steinhardt_parameter(
-            neighbor_method=neighbor_method, cutoff=cutoff, n_clusters=n_clusters,
-            q=q, averaged=averaged, clustering=clustering
+            neighbor_method=neighbor_method,
+            cutoff=cutoff,
+            n_clusters=n_clusters,
+            q=q,
+            averaged=averaged,
+            clustering=clustering,
         )
-    analyse_pyscal_steinhardt_parameter.__doc__ = Analyse.pyscal_steinhardt_parameter.__doc__
+
+    analyse_pyscal_steinhardt_parameter.__doc__ = (
+        Analyse.pyscal_steinhardt_parameter.__doc__
+    )
 
     @deprecate("Use Atoms.analyse.pyscal_cna_adaptive() instead")
     def analyse_pyscal_cna_adaptive(self, mode="total", ovito_compatibility=False):
-        return self._analyse.pyscal_cna_adaptive(mode=mode, ovito_compatibility=ovito_compatibility)
+        return self._analyse.pyscal_cna_adaptive(
+            mode=mode, ovito_compatibility=ovito_compatibility
+        )
+
     analyse_pyscal_cna_adaptive.__doc__ = Analyse.pyscal_cna_adaptive.__doc__
 
     @deprecate("Use Atoms.analyse.pyscal_centro_symmetry() instead")
     def analyse_pyscal_centro_symmetry(self, num_neighbors=12):
         return self._analyse.pyscal_centro_symmetry(num_neighbors=num_neighbors)
+
     analyse_pyscal_centro_symmetry.__doc__ = Analyse.pyscal_centro_symmetry.__doc__
 
     @deprecate("Use Atoms.analyse.pyscal_diamond_structure() instead")
     def analyse_pyscal_diamond_structure(self, mode="total", ovito_compatibility=False):
-        return self._analyse.pyscal_diamond_structure(mode=mode, ovito_compatibility=ovito_compatibility)
+        return self._analyse.pyscal_diamond_structure(
+            mode=mode, ovito_compatibility=ovito_compatibility
+        )
+
     analyse_pyscal_diamond_structure.__doc__ = Analyse.pyscal_diamond_structure.__doc__
 
     @deprecate("Use Atoms.analyse.pyscal_voronoi_volume() instead")
     def analyse_pyscal_voronoi_volume(self):
         return self._analyse.pyscal_voronoi_volume()
+
     analyse_pyscal_voronoi_volume.__doc__ = Analyse.pyscal_voronoi_volume.__doc__
 
     @deprecate("Use get_symmetry()['equivalent_atoms'] instead")
     def analyse_phonopy_equivalent_atoms(self):
-        from pyiron_atomistics.atomistics.structure.phonopy import analyse_phonopy_equivalent_atoms
+        from pyiron_atomistics.atomistics.structure.phonopy import (
+            analyse_phonopy_equivalent_atoms,
+        )
+
         return analyse_phonopy_equivalent_atoms(atoms=self)
 
     def plot3d(
         self,
-        mode='NGLview',
+        mode="NGLview",
         show_cell=True,
         show_axes=True,
         camera="orthographic",
         spacefill=True,
         particle_size=1.0,
         select_atoms=None,
         background="white",
@@ -1115,17 +1210,71 @@
         scalar_end=None,
         scalar_cmap=None,
         vector_field=None,
         vector_color=None,
         magnetic_moments=False,
         view_plane=np.array([0, 0, 1]),
         distance_from_camera=1.0,
-        opacity=1.0
+        opacity=1.0,
     ):
-        return self.visualize.plot3d(
+        """
+        Plot3d relies on NGLView or plotly to visualize atomic structures. Here, we construct a string in the "protein database"
+
+        The final widget is returned. If it is assigned to a variable, the visualization is suppressed until that
+        variable is evaluated, and in the meantime more NGL operations can be applied to it to modify the visualization.
+
+        Args:
+            mode (str): `NGLView`, `plotly` or `ase`
+            show_cell (bool): Whether or not to show the frame. (Default is True.)
+            show_axes (bool): Whether or not to show xyz axes. (Default is True.)
+            camera (str): 'perspective' or 'orthographic'. (Default is 'perspective'.)
+            spacefill (bool): Whether to use a space-filling or ball-and-stick representation. (Default is True, use
+                space-filling atoms.)
+            particle_size (float): Size of the particles. (Default is 1.)
+            select_atoms (numpy.ndarray): Indices of atoms to show, either as integers or a boolean array mask.
+                (Default is None, show all atoms.)
+            background (str): Background color. (Default is 'white'.)
+            color_scheme (str): NGLView color scheme to use. (Default is None, color by element.)
+            colors (numpy.ndarray): A per-atom array of HTML color names or hex color codes to use for atomic colors.
+                (Default is None, use coloring scheme.)
+            scalar_field (numpy.ndarray): Color each atom according to the array value (Default is None, use coloring
+                scheme.)
+            scalar_start (float): The scalar value to be mapped onto the low end of the color map (lower values are
+                clipped). (Default is None, use the minimum value in `scalar_field`.)
+            scalar_end (float): The scalar value to be mapped onto the high end of the color map (higher values are
+                clipped). (Default is None, use the maximum value in `scalar_field`.)
+            scalar_cmap (matplotlib.cm): The colormap to use. (Default is None, giving a blue-red divergent map.)
+            vector_field (numpy.ndarray): Add vectors (3 values) originating at each atom. (Default is None, no
+                vectors.)
+            vector_color (numpy.ndarray): Colors for the vectors (only available with vector_field). (Default is None,
+                vectors are colored by their direction.)
+            magnetic_moments (bool): Plot magnetic moments as 'scalar_field' or 'vector_field'.
+            view_plane (numpy.ndarray): A Nx3-array (N = 1,2,3); the first 3d-component of the array specifies
+                which plane of the system to view (for example, [1, 0, 0], [1, 1, 0] or the [1, 1, 1] planes), the
+                second 3d-component (if specified, otherwise [1, 0, 0]) gives the horizontal direction, and the third
+                component (if specified) is the vertical component, which is ignored and calculated internally. The
+                orthonormality of the orientation is internally ensured, and therefore is not required in the function
+                call. (Default is np.array([0, 0, 1]), which is view normal to the x-y plane.)
+            distance_from_camera (float): Distance of the camera from the structure. Higher = farther away.
+                (Default is 14, which also seems to be the NGLView default value.)
+
+            Possible NGLView color schemes:
+              " ", "picking", "random", "uniform", "atomindex", "residueindex",
+              "chainindex", "modelindex", "sstruc", "element", "resname", "bfactor",
+              "hydrophobicity", "value", "volume", "occupancy"
+
+        Returns:
+            (nglview.NGLWidget): The NGLView widget itself, which can be operated on further or viewed as-is.
+
+        Warnings:
+            * Many features only work with space-filling atoms (e.g. coloring by a scalar field).
+            * The colour interpretation of some hex codes is weird, e.g. 'green'.
+        """
+        return plot3d(
+            structure=pyiron_to_ase(self),
             mode=mode,
             show_cell=show_cell,
             show_axes=show_axes,
             camera=camera,
             spacefill=spacefill,
             particle_size=particle_size,
             select_atoms=select_atoms,
@@ -1139,15 +1288,14 @@
             vector_field=vector_field,
             vector_color=vector_color,
             magnetic_moments=magnetic_moments,
             view_plane=view_plane,
             distance_from_camera=distance_from_camera,
             opacity=opacity,
         )
-    plot3d.__doc__ = Visualize.plot3d.__doc__
 
     def pos_xyz(self):
         """
 
         Returns:
 
         """
@@ -1161,327 +1309,291 @@
 
         Returns:
 
         """
         xyz = self.get_scaled_positions(wrap=False)
         return xyz[:, 0], xyz[:, 1], xyz[:, 2]
 
-    def get_extended_positions(self, width, return_indices=False, norm_order=2):
+    def get_vertical_length(self, norm_order=2):
+        """
+        Return the length of the cell in each direction projected on the vector vertical to the
+        plane.
+
+        Example:
+
+        For a cell `[[1, 1, 0], [0, 1, 0], [0, 0, 1]]`, this function returns
+        `[1., 0.70710678, 1.]` because the first cell vector is projected on the vector vertical
+        to the yz-plane (as well as the y component on the xz-plane).
+
+        Args:
+            norm_order (int): Norm order (cf. numpy.linalg.norm)
+        """
+        return np.linalg.det(self.cell) / np.linalg.norm(
+            np.cross(np.roll(self.cell, -1, axis=0), np.roll(self.cell, 1, axis=0)),
+            axis=-1,
+            ord=norm_order,
+        )
+
+    def get_extended_positions(
+        self, width, return_indices=False, norm_order=2, positions=None
+    ):
         """
         Get all atoms in the boundary around the supercell which have a distance
         to the supercell boundary of less than dist
 
         Args:
             width (float): width of the buffer layer on every periodic box side within which all
                 atoms across periodic boundaries are chosen.
             return_indices (bool): Whether or not return the original indices of the appended
                 atoms.
             norm_order (float): Order of Lp-norm.
+            positions (numpy.ndarray): Positions for which the extended positions are returned.
+                If None, the atom positions of the structure are used.
 
         Returns:
             numpy.ndarray: Positions of all atoms in the extended box, indices of atoms in
                 their original option (if return_indices=True)
 
         """
-        if width<0:
-            raise ValueError('Invalid width')
-        if width==0:
+        if width < 0:
+            raise ValueError("Invalid width")
+        if positions is None:
+            positions = self.positions
+        if width == 0:
             if return_indices:
-                return self.positions, np.arange(len(self))
-            return self.positions
-        width /= np.linalg.det(self.cell)
-        width *= np.linalg.norm(
-            np.cross(np.roll(self.cell, -1, axis=0), np.roll(self.cell, 1, axis=0)),
-            axis=-1,
-            ord=norm_order,
-        )
-        rep = 2*np.ceil(width).astype(int)*self.pbc+1
-        rep = [np.arange(r)-int(r/2) for r in rep]
+                return positions, np.arange(len(positions))
+            return positions
+        width /= self.get_vertical_length(norm_order=norm_order)
+        rep = 2 * np.ceil(width).astype(int) * self.pbc + 1
+        rep = [np.arange(r) - int(r / 2) for r in rep]
         meshgrid = np.meshgrid(rep[0], rep[1], rep[2])
         meshgrid = np.stack(meshgrid, axis=-1).reshape(-1, 3)
-        v_repeated = np.einsum('ni,ij->nj', meshgrid, self.cell)
-        v_repeated = v_repeated[:,np.newaxis,:]+self.positions[np.newaxis,:,:]
+        v_repeated = np.einsum("ni,ij->nj", meshgrid, self.cell)
+        v_repeated = v_repeated[:, np.newaxis, :] + positions[np.newaxis, :, :]
         v_repeated = v_repeated.reshape(-1, 3)
-        indices = np.tile(np.arange(len(self)), len(meshgrid))
-        dist = v_repeated-np.sum(self.cell*0.5, axis=0)
-        dist = np.absolute(np.einsum('ni,ij->nj', dist+1e-8, np.linalg.inv(self.cell)))-0.5
-        check_dist = np.all(dist-width<0, axis=-1)
-        indices = indices[check_dist]%len(self)
+        indices = np.tile(np.arange(len(positions)), len(meshgrid))
+        dist = v_repeated - np.sum(self.cell * 0.5, axis=0)
+        dist = (
+            np.absolute(np.einsum("ni,ij->nj", dist + 1e-8, np.linalg.inv(self.cell)))
+            - 0.5
+        )
+        check_dist = np.all(dist - width < 0, axis=-1)
+        indices = indices[check_dist] % len(positions)
         v_repeated = v_repeated[check_dist]
         if return_indices:
             return v_repeated, indices
         return v_repeated
 
+    @deprecate("Use get_neighbors and call numbers_of_neighbors")
     def get_numbers_of_neighbors_in_sphere(
-            self,
-            cutoff_radius=10,
-            num_neighbors=None,
-            id_list=None,
-            width_buffer=1.2,
-    ):
-        """
-        Function to compute the maximum number of neighbors in a sphere around each atom.
-        Args:
-            cutoff_radius (float): Upper bound of the distance to which the search must be done
-            num_neighbors (int/None): maximum number of neighbors found
-            id_list (list): list of atoms the neighbors are to be looked for
-            width_buffer (float): width of the layer to be added to account for pbc.
-
-        Returns:
-            (np.ndarray) : for each atom the number of neighbors found in the sphere of radius
-                           cutoff_radius (<= num_neighbors if specified)
-        """
-        if num_neighbors is not None:
-            neigh = self._get_neighbors(
-                num_neighbors=num_neighbors,
-                t_vec=False,
-                id_list=id_list,
-                cutoff_radius=cutoff_radius,
-                width_buffer=width_buffer,
-            )
-            num_neighbors_per_atom = np.sum(neigh.distances < np.inf, axis=-1)
-        else:
-            volume_per_atom = self.get_volume(per_atom=True)
-            if id_list is not None:
-                volume_per_atom = self.get_volume() / len(id_list)
-            num_neighbors = int((1 + width_buffer) *
-                                4. / 3. * np.pi * cutoff_radius ** 3 / volume_per_atom)
-            num_neighbors_old = num_neighbors - 1
-            while num_neighbors_old < num_neighbors:
-                neigh = self._get_neighbors(
-                    num_neighbors=num_neighbors,
-                    t_vec=False,
-                    id_list=id_list,
-                    cutoff_radius=cutoff_radius,
-                    width_buffer=width_buffer,
-                )
-                num_neighbors_old = num_neighbors
-                num_neighbors_per_atom = np.sum(neigh.distances < np.inf, axis=-1)
-                num_neighbors = num_neighbors_per_atom.max()
-                if num_neighbors == num_neighbors_old:
-                    num_neighbors = 2 * num_neighbors
-        return num_neighbors_per_atom
-
-    def get_neighbors_by_distance(
         self,
-        cutoff_radius=5,
+        cutoff_radius=10,
         num_neighbors=None,
-        t_vec=True,
-        tolerance=2,
         id_list=None,
         width_buffer=1.2,
-        allow_ragged=True,
-        norm_order=2,
     ):
         """
-
+        Function to compute the maximum number of neighbors in a sphere around each atom.
         Args:
             cutoff_radius (float): Upper bound of the distance to which the search must be done
-            num_neighbors (int/None): maximum number of neighbors found; if None this is estimated based on the density.
-            t_vec (bool): True: compute distance vectors
-                        (pbc are automatically taken into account)
-            tolerance (int): tolerance (round decimal points) used for computing neighbor shells
+            num_neighbors (int/None): maximum number of neighbors found
             id_list (list): list of atoms the neighbors are to be looked for
             width_buffer (float): width of the layer to be added to account for pbc.
-            allow_ragged (bool): Whether to allow ragged list of arrays or rectangular
-                numpy.ndarray filled with np.inf for values outside cutoff_radius
-            norm_order (int): Norm to use for the neighborhood search and shell recognition. The
-                definition follows the conventional Lp norm (cf.
-                https://en.wikipedia.org/wiki/Lp_space). This is an feature and for anything
-                other than norm_order=2, there is no guarantee that this works flawlessly.
 
         Returns:
-
-            pyiron.atomistics.structure.atoms.Neighbors: Neighbors instances with the neighbor
-                indices, distances and vectors
-
+            (np.ndarray) : for each atom the number of neighbors found in the sphere of radius
+                           cutoff_radius (<= num_neighbors if specified)
         """
         return self.get_neighbors(
             cutoff_radius=cutoff_radius,
             num_neighbors=num_neighbors,
-            t_vec=t_vec,
-            tolerance=tolerance,
             id_list=id_list,
             width_buffer=width_buffer,
-            allow_ragged=allow_ragged,
-            norm_order=norm_order,
-        )
+        ).numbers_of_neighbors
 
+    @deprecate(allow_ragged="use `mode='ragged'` instead.")
     def get_neighbors(
         self,
         num_neighbors=12,
-        t_vec=True,
         tolerance=2,
         id_list=None,
         cutoff_radius=np.inf,
         width_buffer=1.2,
-        allow_ragged=False,
+        allow_ragged=None,
+        mode="filled",
         norm_order=2,
     ):
         """
 
         Args:
             num_neighbors (int): number of neighbors
-            t_vec (bool): True: compute distance vectors
-                        (pbc are automatically taken into account)
             tolerance (int): tolerance (round decimal points) used for computing neighbor shells
             id_list (list): list of atoms the neighbors are to be looked for
             cutoff_radius (float): Upper bound of the distance to which the search must be done
             width_buffer (float): width of the layer to be added to account for pbc.
-            allow_ragged (bool): Whether to allow ragged list of arrays or rectangular
-                numpy.ndarray filled with np.inf for values outside cutoff_radius
+            allow_ragged (bool): (Deprecated; use mode) Whether to allow ragged list of arrays or
+                rectangular numpy.ndarray filled with np.inf for values outside cutoff_radius
+            mode (str): Representation of per-atom quantities (distances etc.). Choose from
+                'filled', 'ragged' and 'flattened'.
             norm_order (int): Norm to use for the neighborhood search and shell recognition. The
                 definition follows the conventional Lp norm (cf.
                 https://en.wikipedia.org/wiki/Lp_space). This is an feature and for anything
                 other than norm_order=2, there is no guarantee that this works flawlessly.
 
         Returns:
 
-            pyiron.atomistics.structure.atoms.Neighbors: Neighbors instances with the neighbor
+            structuretoolkit.analyse.neighbors.Neighbors: Neighbors instances with the neighbor
                 indices, distances and vectors
 
         """
-        neigh = self._get_neighbors(
+        return get_neighbors(
+            structure=self,
             num_neighbors=num_neighbors,
-            t_vec=t_vec,
             tolerance=tolerance,
             id_list=id_list,
             cutoff_radius=cutoff_radius,
             width_buffer=width_buffer,
+            mode=mode,
             norm_order=norm_order,
         )
-        neigh.allow_ragged = allow_ragged
-        return neigh
 
-    def _get_neighbors(
+    @deprecate(allow_ragged="use `mode='ragged'` instead.")
+    @deprecate("Use get_neighbors", version="1.0.0")
+    def get_neighbors_by_distance(
         self,
-        num_neighbors=12,
-        t_vec=True,
+        cutoff_radius=5,
+        num_neighbors=None,
         tolerance=2,
         id_list=None,
-        cutoff_radius=np.inf,
         width_buffer=1.2,
-        get_tree=False,
+        allow_ragged=None,
+        mode="ragged",
         norm_order=2,
     ):
-        if num_neighbors is not None and num_neighbors<=0:
-            raise ValueError('invalid number of neighbors')
-        if width_buffer<0:
-            raise ValueError('width_buffer must be a positive float')
-        if get_tree:
-            neigh = Tree(ref_structure=self)
-        else:
-            neigh = Neighbors(ref_structure=self, tolerance=tolerance)
-        neigh._norm_order = norm_order
-        width = neigh._estimate_width(
-            num_neighbors=num_neighbors,
+        return self.get_neighbors(
             cutoff_radius=cutoff_radius,
-            width_buffer=width_buffer,
-        )
-        if (width<0.5*np.min(self.cell.diagonal())
-                and np.isclose(np.linalg.norm(self.cell-np.eye(3)*self.cell.diagonal()), 0)
-                and np.all(self.pbc)
-                and cutoff_radius==np.inf):
-            neigh._cell = self.cell.diagonal()
-            extended_positions = self.get_extended_positions(
-                0,
-                return_indices=False,
-                norm_order=norm_order
-            ).copy()
-            extended_positions -= neigh._cell*np.floor(extended_positions/neigh._cell)
-        else:
-            extended_positions, neigh._wrapped_indices = self.get_extended_positions(
-                width, return_indices=True, norm_order=norm_order
-            )
-            neigh._extended_positions = extended_positions
-        neigh._tree = cKDTree(extended_positions, boxsize=neigh._cell)
-        if get_tree:
-            return neigh
-        positions = self.positions
-        if id_list is not None:
-            positions = positions[np.array(id_list)]
-        neigh._get_neighborhood(
-            positions=positions,
             num_neighbors=num_neighbors,
-            t_vec=t_vec,
-            cutoff_radius=cutoff_radius,
-            exclude_self=True,
+            tolerance=tolerance,
+            id_list=id_list,
             width_buffer=width_buffer,
+            allow_ragged=allow_ragged,
+            mode=mode,
+            norm_order=norm_order,
         )
-        if neigh._check_width(width=width, pbc=self.pbc):
-            warnings.warn('width_buffer may have been too small - '
-                          'most likely not all neighbors properly assigned')
-        return neigh
+
+    get_neighbors_by_distance.__doc__ = get_neighbors.__doc__
 
     def get_neighborhood(
         self,
         positions,
         num_neighbors=12,
-        t_vec=True,
         cutoff_radius=np.inf,
         width_buffer=1.2,
+        mode="filled",
         norm_order=2,
     ):
         """
 
         Args:
             position: Position in a box whose neighborhood information is analysed
             num_neighbors (int): Number of nearest neighbors
-            t_vec (bool): True: compute distance vectors (pbc are taken into account)
             cutoff_radius (float): Upper bound of the distance to which the search is to be done
             width_buffer (float): Width of the layer to be added to account for pbc.
+            mode (str): Representation of per-atom quantities (distances etc.). Choose from
+                'filled', 'ragged' and 'flattened'.
             norm_order (int): Norm to use for the neighborhood search and shell recognition. The
                 definition follows the conventional Lp norm (cf.
                 https://en.wikipedia.org/wiki/Lp_space). This is an feature and for anything
                 other than norm_order=2, there is no guarantee that this works flawlessly.
 
         Returns:
 
             pyiron.atomistics.structure.atoms.Tree: Neighbors instances with the neighbor
                 indices, distances and vectors
 
         """
-
-        neigh = self._get_neighbors(
+        return get_neighborhood(
+            structure=self,
+            positions=positions,
             num_neighbors=num_neighbors,
             cutoff_radius=cutoff_radius,
             width_buffer=width_buffer,
-            t_vec=t_vec,
-            get_tree=True,
+            mode=mode,
             norm_order=norm_order,
         )
-        return neigh._get_neighborhood(
-            positions=positions,
-            num_neighbors=num_neighbors,
-            t_vec=t_vec,
-            cutoff_radius=cutoff_radius,
-        )
 
-    @deprecate("Use neigh.find_neighbors_by_vector() instead (after calling neigh = structure.get_neighbors())",
-               version="1.0.0")
-    def find_neighbors_by_vector(self, vector, return_deviation=False, num_neighbors=96):
+    @deprecate(
+        "Use neigh.find_neighbors_by_vector() instead (after calling neigh = structure.get_neighbors())",
+        version="1.0.0",
+    )
+    def find_neighbors_by_vector(
+        self, vector, return_deviation=False, num_neighbors=96
+    ):
+        """
+        Args:
+            vector (list/np.ndarray): vector by which positions are translated (and neighbors are searched)
+            return_deviation (bool): whether to return distance between the expect positions and real positions
+
+        Returns:
+            np.ndarray: list of id's for the specified translation
+
+        Example:
+            a_0 = 2.832
+            structure = pr.create_structure('Fe', 'bcc', a_0)
+            id_list = structure.find_neighbors_by_vector([0, 0, a_0])
+            # In this example, you get a list of neighbor atom id's at z+=a_0 for each atom.
+            # This is particularly powerful for SSA when the magnetic structure has to be translated
+            # in each direction.
+        """
         neighbors = self.get_neighbors(num_neighbors=num_neighbors)
-        return neighbors.find_neighbors_by_vector(vector=vector, return_deviation=return_deviation)
-    find_neighbors_by_vector.__doc__ = Neighbors.find_neighbors_by_vector.__doc__
+        return neighbors.find_neighbors_by_vector(
+            vector=vector, return_deviation=return_deviation
+        )
 
-    @deprecate("Use neigh.get_shell_matrix() instead (after calling neigh = structure.get_neighbors())",
-               version="1.0.0")
+    @deprecate(
+        "Use neigh.get_shell_matrix() instead (after calling neigh = structure.get_neighbors())",
+        version="1.0.0",
+    )
     def get_shell_matrix(
-        self, id_list=None, chemical_pair=None, num_neighbors=100, tolerance=2,
-        cluster_by_distances=False, cluster_by_vecs=False
+        self,
+        id_list=None,
+        chemical_pair=None,
+        num_neighbors=100,
+        tolerance=2,
+        cluster_by_distances=False,
+        cluster_by_vecs=False,
     ):
+        """
+        Shell matrices for pairwise interaction. Note: The matrices are always symmetric, meaning if you
+        use them as bilinear operators, you have to divide the results by 2.
+
+        Args:
+            chemical_pair (list): pair of chemical symbols (e.g. ['Fe', 'Ni'])
+
+        Returns:
+            list of sparse matrices for different shells
+
+
+        Example:
+            from pyiron_atomistics import Project
+            structure = Project('.').create_structure('Fe', 'bcc', 2.83).repeat(2)
+            J = -0.1 # Ising parameter
+            magmoms = 2*np.random.random((len(structure)), 3)-1 # Random magnetic moments between -1 and 1
+            neigh = structure.get_neighbors(num_neighbors=8) # Iron first shell
+            shell_matrices = neigh.get_shell_matrix()
+            print('Energy =', 0.5*J*magmoms.dot(shell_matrices[0].dot(matmoms)))
+        """
         neigh_list = self.get_neighbors(
             num_neighbors=num_neighbors, id_list=id_list, tolerance=tolerance
         )
         return neigh_list.get_shell_matrix(
             chemical_pair=chemical_pair,
             cluster_by_distances=cluster_by_distances,
-            cluster_by_vecs=cluster_by_vecs
+            cluster_by_vecs=cluster_by_vecs,
         )
-    get_shell_matrix.__doc__ = Neighbors.get_shell_matrix.__doc__
 
     def occupy_lattice(self, **qwargs):
         """
         Replaces specified indices with a given species
         """
         new_species = list(np.array(self.species).copy())
         new_indices = np.array(self.indices.copy())
@@ -1502,16 +1614,18 @@
                 retain_species_indices.append(i)
         for i in delete_species_indices:
             new_indices[new_indices >= i] += -1
         new_species = np.array(new_species)[retain_species_indices]
         self.set_species(new_species)
         self.indices = new_indices
 
-    @deprecate("Use neigh.cluster_analysis() instead (after calling neigh = structure.get_neighbors())",
-               version="1.0.0")
+    @deprecate(
+        "Use neigh.cluster_analysis() instead (after calling neigh = structure.get_neighbors())",
+        version="1.0.0",
+    )
     def cluster_analysis(
         self, id_list, neighbors=None, radius=None, return_cluster_sizes=False
     ):
         """
 
         Args:
             id_list:
@@ -1521,24 +1635,30 @@
 
         Returns:
 
         """
         if neighbors is None:
             if radius is None:
                 neigh = self.get_neighbors(num_neighbors=100)
-                indices = np.unique(neigh.shells[0][neigh.shells[0]<=2], return_index=True)[1]
+                indices = np.unique(
+                    neigh.shells[0][neigh.shells[0] <= 2], return_index=True
+                )[1]
                 radius = neigh.distances[0][indices]
                 radius = np.mean(radius)
                 # print "radius: ", radius
-            neighbors = self.get_neighbors_by_distance(cutoff_radius=radius, t_vec=False)
-        return neighbors.cluster_analysis(id_list=id_list, return_cluster_sizes=return_cluster_sizes)
+            neighbors = self.get_neighbors_by_distance(cutoff_radius=radius)
+        return neighbors.cluster_analysis(
+            id_list=id_list, return_cluster_sizes=return_cluster_sizes
+        )
 
     # TODO: combine with corresponding routine in plot3d
-    @deprecate("Use neigh.get_bonds() instead (after calling neigh = structure.get_neighbors())",
-               version="1.0.0")
+    @deprecate(
+        "Use neigh.get_bonds() instead (after calling neigh = structure.get_neighbors())",
+        version="1.0.0",
+    )
     def get_bonds(self, radius=np.inf, max_shells=None, prec=0.1, num_neighbors=20):
         """
 
         Args:
             radius:
             max_shells:
             prec: minimum distance between any two clusters (if smaller considered to be single cluster)
@@ -1548,353 +1668,193 @@
 
         """
         neighbors = self.get_neighbors_by_distance(
             cutoff_radius=radius, num_neighbors=num_neighbors
         )
         return neighbors.get_bonds(radius=radius, max_shells=max_shells, prec=prec)
 
-    # spglib calls
-    @deprecate_soon
     def get_symmetry(
         self, use_magmoms=False, use_elements=True, symprec=1e-5, angle_tolerance=-1.0
     ):
         """
 
         Args:
-            use_magmoms:
-            use_elements: True or False. If False, chemical elements will be ignored
-            symprec:
-            angle_tolerance:
+            use_magmoms (bool): Whether to consider magnetic moments (cf.
+            get_initial_magnetic_moments())
+            use_elements (bool): If False, chemical elements will be ignored
+            symprec (float): Symmetry search precision
+            angle_tolerance (float): Angle search tolerance
 
         Returns:
+            symmetry (:class:`pyiron.atomistics.structure.symmetry.Symmetry`): Symmetry class
 
 
         """
-        lattice = np.array(self.get_cell().T, dtype="double", order="C")
-        positions = np.array(
-            self.get_scaled_positions(wrap=False), dtype="double", order="C"
-        )
-        if use_elements:
-            numbers = np.array(self.get_atomic_numbers(), dtype="intc")
-        else:
-            numbers = np.ones_like(self.get_atomic_numbers(), dtype="intc")
-        if use_magmoms:
-            magmoms = self.get_initial_magnetic_moments()
-            return spglib.get_symmetry(
-                cell=(lattice, positions, numbers, magmoms),
-                symprec=symprec,
-                angle_tolerance=angle_tolerance,
-            )
-        else:
-            return spglib.get_symmetry(
-                cell=(lattice, positions, numbers),
-                symprec=symprec,
-                angle_tolerance=angle_tolerance,
-            )
+        return get_symmetry(
+            structure=self,
+            use_magmoms=use_magmoms,
+            use_elements=use_elements,
+            symprec=symprec,
+            angle_tolerance=angle_tolerance,
+        )
 
-    @deprecate_soon
+    @deprecate("Use structure.get_symmetry().symmetrize_vectors()")
     def symmetrize_vectors(
-        self, vectors, force_update=False, use_magmoms=False, use_elements=True, symprec=1e-5, angle_tolerance=-1.0
+        self,
+        vectors,
+        use_magmoms=False,
+        use_elements=True,
+        symprec=1e-5,
+        angle_tolerance=-1.0,
     ):
         """
         Symmetrization of natom x 3 vectors according to box symmetries
 
         Args:
             vectors (ndarray/list): natom x 3 array to symmetrize
-            force_update (bool): whether to update the symmetry info
             use_magmoms (bool): cf. get_symmetry
             use_elements (bool): cf. get_symmetry
             symprec (float): cf. get_symmetry
             angle_tolerance (float): cf. get_symmetry
 
         Returns:
             (np.ndarray) symmetrized vectors
         """
-        vectors = np.array(vectors).reshape(-1, 3)
-        if vectors.shape != self.positions.shape:
-            print(vectors.shape, self.positions.shape)
-            raise ValueError('Vector must be a natom x 3 array: {} != {}'.format(vectors.shape, self.positions.shape))
-        if self._symmetry_dataset is None or force_update:
-            symmetry = self.get_symmetry(use_magmoms=use_magmoms, use_elements=use_elements,
-                                         symprec=symprec, angle_tolerance=angle_tolerance)
-            scaled_positions = self.get_scaled_positions(wrap=False)
-            symmetry['indices'] = []
-            for rot,tra in zip(symmetry['rotations'], symmetry['translations']):
-                positions = np.einsum('ij,nj->ni', rot, scaled_positions)+tra
-                positions -= np.floor(positions+1.0e-2)
-                vec = np.where(np.linalg.norm(positions[np.newaxis, :, :]-scaled_positions[:, np.newaxis, :], axis=-1)<=1.0e-4)
-                symmetry['indices'].append(vec[1])
-            symmetry['indices'] = np.array(symmetry['indices'])
-            self._symmetry_dataset = symmetry
-        return np.einsum('ijk,ink->nj', self._symmetry_dataset['rotations'],
-                         vectors[self._symmetry_dataset['indices']])/len(self._symmetry_dataset['rotations'])
-
-    @deprecate_soon
-    def group_points_by_symmetry(self, points):
-        """
-            This function classifies the points into groups according to the box symmetry given by spglib.
-
-            Args:
-                points: (np.array/list) nx3 array which contains positions
-
-            Returns: list of arrays containing geometrically equivalent positions
-
-            It is possible that the original points are not found in the returned list, as the positions outsie
-            the box will be projected back to the box.
-        """
-        struct_copy = self.copy()
-        points = np.array(points).reshape(-1, 3)
-        struct_copy += Atoms(elements=len(points) * ["Hs"], positions=points)
-        struct_copy.center_coordinates_in_unit_cell()
-        group_IDs = struct_copy.get_symmetry()["equivalent_atoms"][
-            struct_copy.select_index("Hs")
-        ]
-        return [
-            np.round(points[group_IDs == ID], decimals=8) for ID in np.unique(group_IDs)
-        ]
-
-    def _get_voronoi_vertices(self, minimum_dist=0.1):
-        """
-            This function gives the positions of Voronoi vertices
-            This function does not work if there are Hs atoms in the box
-
-            Args:
-                minimum_dist: Minimum distance between two Voronoi vertices to be considered as one
-
-            Returns: Positions of Voronoi vertices, box
-
-        """
-        vor = Voronoi(
-            self.repeat(3 * [2]).positions
-        )  # Voronoi package does not have periodic boundary conditions
-        b_cell_inv = np.linalg.inv(self.cell)
-        voro_vert = vor.vertices
-        for ind, v in enumerate(voro_vert):
-            pos = np.mean(
-                voro_vert[(np.linalg.norm(voro_vert - v, axis=-1) < minimum_dist)],
-                axis=0,
-            )  # Find all points which are within minimum_dist
-            voro_vert[(np.linalg.norm(voro_vert - v, axis=-1) < 0.5)] = np.array(
-                3 * [-10]
-            )  # Mark atoms to be deleted afterwards
-            voro_vert[ind] = pos
-        voro_vert = voro_vert[np.min(voro_vert, axis=-1) > -5]
-
-        voro_vert = np.dot(b_cell_inv.T, voro_vert.T).T  # get scaled positions
-        voro_vert = voro_vert[
-            (np.min(voro_vert, axis=-1) > 0.499) & (np.max(voro_vert, axis=-1) < 1.501)
-        ]
-        voro_vert = np.dot(self.cell.T, voro_vert.T).T  # get true positions
-
-        box_copy = self.copy()
-        new_atoms = Atoms(cell=self.cell, symbols=["Hs"]).repeat([len(voro_vert), 1, 1])
-        box_copy += new_atoms
-
-        pos_total = np.append(self.positions, voro_vert)
-        pos_total = pos_total.reshape(-1, 3)
-        box_copy.positions = pos_total
-
-        box_copy.center_coordinates_in_unit_cell()
-
-        neigh = (
-            box_copy.get_neighbors()
-        )  # delete all atoms which lie within minimum_dist (including periodic boundary conditions)
-        while (
-            len(
-                np.array(neigh.indices).flatten()[
-                    np.array(neigh.distances).flatten() < minimum_dist
-                ]
-            )
-            != 0
-        ):
-            del box_copy[
-                np.array(neigh.indices).flatten()[
-                    np.array(neigh.distances).flatten() < minimum_dist
-                ][0]
-            ]
-            neigh = box_copy.get_neighbors()
-        return pos_total, box_copy
+        return self.get_symmetry(
+            use_magmoms=use_magmoms,
+            use_elements=use_elements,
+            symprec=symprec,
+            angle_tolerance=angle_tolerance,
+        ).symmetrize_vectors(vectors=vectors)
 
-    @deprecate_soon
-    def get_equivalent_voronoi_vertices(
-        self, return_box=False, minimum_dist=0.1, symprec=1e-5, angle_tolerance=-1.0
+    @deprecate("Use structure.get_symmetry().get_arg_equivalent_sites() instead")
+    def group_points_by_symmetry(
+        self,
+        points,
+        use_magmoms=False,
+        use_elements=True,
+        symprec=1e-5,
+        angle_tolerance=-1.0,
     ):
         """
-            This function gives the positions of spatially equivalent Voronoi vertices in lists, which
-            most likely represent interstitial points or vacancies (along with other high symmetry points)
-            Each list item contains an array of positions which are spacially equivalent.
-            This function does not work if there are Hs atoms in the box
+        This function classifies the points into groups according to the box symmetry given by
+        spglib.
 
-            Args:
-                return_box: True, if the box containing atoms on the positions of Voronoi vertices
-                            should be returned (which are represented by Hs atoms)
-                minimum_dist: Minimum distance between two Voronoi vertices to be considered as one
+        Args:
+            points: (np.array/list) nx3 array which contains positions
+            use_magmoms (bool): Whether to consider magnetic moments (cf.
+            get_initial_magnetic_moments())
+            use_elements (bool): If False, chemical elements will be ignored
+            symprec (float): Symmetry search precision
+            angle_tolerance (float): Angle search tolerance
 
-            Returns: List of numpy array positions of spacially equivalent Voronoi vertices
+        Returns: list of arrays containing geometrically equivalent positions
 
+        It is possible that the original points are not found in the returned list, as the
+        positions outsie the box will be projected back to the box.
         """
+        return self.get_symmetry(
+            use_magmoms=use_magmoms,
+            use_elements=use_elements,
+            symprec=symprec,
+            angle_tolerance=angle_tolerance,
+        ).get_arg_equivalent_sites(points)
 
-        _, box_copy = self._get_voronoi_vertices(minimum_dist=minimum_dist)
-        list_positions = []
-        sym = box_copy.get_symmetry(symprec=symprec, angle_tolerance=angle_tolerance)
-        for ind in set(sym["equivalent_atoms"][box_copy.select_index("Hs")]):
-            list_positions.append(box_copy.positions[sym["equivalent_atoms"] == ind])
-        if return_box:
-            return list_positions, box_copy
-        else:
-            return list_positions
-
-    @deprecate_soon
-    def get_equivalent_points(self, points, use_magmoms=False, use_elements=True, symprec=1e-5, angle_tolerance=-1.0):
+    @deprecate("Use structure.get_symmetry().get_arg_equivalent_sites() instead")
+    def get_equivalent_points(
+        self,
+        points,
+        use_magmoms=False,
+        use_elements=True,
+        symprec=1e-5,
+        angle_tolerance=-1.0,
+    ):
         """
 
         Args:
             points (list/ndarray): 3d vector
             use_magmoms (bool): cf. get_symmetry()
             use_elements (bool): cf. get_symmetry()
             symprec (float): cf. get_symmetry()
             angle_tolerance (float): cf. get_symmetry()
 
         Returns:
             (ndarray): array of equivalent points with respect to box symmetries
         """
-        symmetry_operations = self.get_symmetry(use_magmoms=use_magmoms,
-                                                use_elements=use_elements,
-                                                symprec=symprec,
-                                                angle_tolerance=angle_tolerance)
-        R = symmetry_operations['rotations']
-        t = symmetry_operations['translations']
-        x = np.einsum('jk,j->k', np.linalg.inv(self.cell), points)
-        x = np.einsum('nxy,y->nx', R, x)+t
-        x -= np.floor(x)
-        dist = x[:,np.newaxis]-x[np.newaxis,:]
-        w, v = np.where(np.linalg.norm(dist-np.rint(dist), axis=-1)<symprec)
-        x = np.delete(x, w[v<w], axis=0)
-        x = np.einsum('ji,mj->mi', self.cell, x)
-        return x
+        return self.get_symmetry(
+            use_magmoms=use_magmoms,
+            use_elements=use_elements,
+            symprec=symprec,
+            angle_tolerance=angle_tolerance,
+        ).get_arg_equivalent_sites(points)
 
-    @deprecate_soon
+    @deprecate("Use structure.get_symmetry().info instead")
     def get_symmetry_dataset(self, symprec=1e-5, angle_tolerance=-1.0):
         """
 
         Args:
             symprec:
             angle_tolerance:
 
         Returns:
 
         https://atztogo.github.io/spglib/python-spglib.html
         """
-        lattice = np.array(self.get_cell().T, dtype="double", order="C")
-        positions = np.array(
-            self.get_scaled_positions(wrap=False), dtype="double", order="C"
-        )
-        numbers = np.array(self.get_atomic_numbers(), dtype="intc")
-        return spglib.get_symmetry_dataset(
-            cell=(lattice, positions, numbers),
-            symprec=symprec,
-            angle_tolerance=angle_tolerance,
-        )
+        return self.get_symmetry(symprec=symprec, angle_tolerance=angle_tolerance).info
 
-    @deprecate_soon
+    @deprecate("Use structure.get_symmetry().spacegroup instead")
     def get_spacegroup(self, symprec=1e-5, angle_tolerance=-1.0):
         """
 
         Args:
             symprec:
             angle_tolerance:
 
         Returns:
 
         https://atztogo.github.io/spglib/python-spglib.html
         """
-        lattice = np.array(self.get_cell(), dtype="double", order="C")
-        positions = np.array(
-            self.get_scaled_positions(wrap=False), dtype="double", order="C"
-        )
-        numbers = np.array(self.get_atomic_numbers(), dtype="intc")
-        space_group = spglib.get_spacegroup(
-            cell=(lattice, positions, numbers),
-            symprec=symprec,
-            angle_tolerance=angle_tolerance,
-        ).split()
-        if len(space_group) == 1:
-            return {"Number": ast.literal_eval(space_group[0])}
-        else:
-            return {
-                "InternationalTableSymbol": space_group[0],
-                "Number": ast.literal_eval(space_group[1]),
-            }
+        return self.get_symmetry(
+            symprec=symprec, angle_tolerance=angle_tolerance
+        ).spacegroup
 
-    @deprecate_soon
+    @deprecate("Use structure.get_symmetry().refine_cell() instead")
     def refine_cell(self, symprec=1e-5, angle_tolerance=-1.0):
         """
 
         Args:
             symprec:
             angle_tolerance:
 
         Returns:
 
         https://atztogo.github.io/spglib/python-spglib.html
         """
-        lattice = np.array(self.get_cell().T, dtype="double", order="C")
-        positions = np.array(
-            self.get_scaled_positions(wrap=False), dtype="double", order="C"
-        )
-        numbers = np.array(self.get_atomic_numbers(), dtype="intc")
-        cell, coords, el = spglib.refine_cell(
-            cell=(lattice, positions, numbers),
-            symprec=symprec,
-            angle_tolerance=angle_tolerance,
-        )
-
-        return Atoms(
-            symbols=list(self.get_chemical_symbols()), positions=coords, cell=cell, pbc=self.pbc
-        )
-
-    @deprecate_soon
+        return self.get_symmetry(
+            symprec=symprec, angle_tolerance=angle_tolerance
+        ).refine_cell()
+
+    @deprecate(
+        "Use structure.get_symmetry().get_primitive_cell(standardize=False) instead"
+    )
     def get_primitive_cell(self, symprec=1e-5, angle_tolerance=-1.0):
         """
 
         Args:
             symprec:
             angle_tolerance:
 
         Returns:
 
         """
-        el_dict = {}
-        for el in set(self.get_chemical_elements()):
-            el_dict[el.AtomicNumber] = el
-        lattice = np.array(self.get_cell().T, dtype="double", order="C")
-        positions = np.array(
-            self.get_scaled_positions(wrap=False), dtype="double", order="C"
-        )
-        numbers = np.array(self.get_atomic_numbers(), dtype="intc")
-        cell, coords, atomic_numbers = spglib.find_primitive(
-            cell=(lattice, positions, numbers),
-            symprec=symprec,
-            angle_tolerance=angle_tolerance,
-        )
-        # print atomic_numbers, type(atomic_numbers)
-        el_lst = [el_dict[i_a] for i_a in atomic_numbers]
-
-        # convert lattice vectors to standard (experimental feature!) TODO:
-        red_structure = Atoms(elements=el_lst, scaled_positions=coords, cell=cell, pbc=self.pbc)
-        space_group = red_structure.get_spacegroup(symprec)["Number"]
-        # print "space group: ", space_group
-        if space_group == 225:  # fcc
-            alat = np.max(cell[0])
-            amat_fcc = alat * np.array([[1, 0, 1], [1, 1, 0], [0, 1, 1]])
+        return self.get_symmetry(
+            symprec=symprec, angle_tolerance=angle_tolerance
+        ).get_primitive_cell(standardize=False)
 
-            red_structure.cell = amat_fcc
-        return red_structure
-
-    @deprecate_soon
+    @deprecate("Use structure.get_symmetry().get_ir_reciprocal_mesh() instead")
     def get_ir_reciprocal_mesh(
         self,
         mesh,
         is_shift=np.zeros(3, dtype="intc"),
         is_time_reversal=True,
         symprec=1e-5,
     ):
@@ -1905,22 +1865,19 @@
             is_shift:
             is_time_reversal:
             symprec:
 
         Returns:
 
         """
-        mapping, mesh_points = spglib.get_ir_reciprocal_mesh(
+        return self.get_symmetry(symprec=symprec).get_ir_reciprocal_mesh(
             mesh=mesh,
-            cell=self,
             is_shift=is_shift,
             is_time_reversal=is_time_reversal,
-            symprec=symprec,
         )
-        return mapping, mesh_points
 
     def get_majority_species(self, return_count=False):
         """
         This function returns the majority species and their number in the box
 
         Returns:
             number of atoms of the majority species, chemical symbol and chemical index
@@ -1944,14 +1901,15 @@
     def close(self):
         # TODO: implement
         pass
 
     @deprecate("Use Atoms.analyse.pyscal_voronoi_volume() instead")
     def get_voronoi_volume(self):
         return self._analyse.pyscal_voronoi_volume()
+
     get_voronoi_volume.__doc__ = Analyse.pyscal_voronoi_volume.__doc__
 
     def is_skewed(self, tolerance=1.0e-8):
         """
         Check whether the simulation box is skewed/sheared. The algorithm compares the box volume
         and the product of the box length in each direction. If these numbers do not match, the box
         is considered to be skewed and the function returns True
@@ -1961,37 +1919,30 @@
 
         Returns:
             (bool): Whether the box is skewed or not.
         """
         volume = self.get_volume()
         prod = np.linalg.norm(self.cell, axis=-1).prod()
         if volume > 0:
-            if abs(volume-prod)/volume < tolerance:
+            if abs(volume - prod) / volume < tolerance:
                 return False
         return True
 
     def find_mic(self, v, vectors=True):
         """
         Find vectors following minimum image convention (mic). In principle this
         function does the same as ase.geometry.find_mic
 
         Args:
             v (list/numpy.ndarray): 3d vector or a list/array of 3d vectors
             vectors (bool): Whether to return vectors (distances are returned if False)
 
         Returns: numpy.ndarray of the same shape as input with mic
         """
-        vecs = np.asarray(v).reshape(-1, 3)
-        if any(self.pbc):
-            vecs = np.einsum('ji,nj->ni', np.linalg.inv(self.cell), vecs)
-            vecs[:,self.pbc] -= np.rint(vecs)[:,self.pbc]
-            vecs = np.einsum('ji,nj->ni', self.cell, vecs)
-        if vectors:
-            return vecs.reshape(np.asarray(v).shape)
-        return np.linalg.norm(vecs, axis=-1).reshape(np.asarray(v).shape[:-1])
+        return find_mic(structure=self, v=v, vectors=vectors)
 
     def get_distance(self, a0, a1, mic=True, vector=False):
         """
         Return distance between two atoms.
         Use mic=True to use the Minimum Image Convention.
         vector=True gives the distance vector (from a0 to a1).
 
@@ -2019,15 +1970,15 @@
             a1 = np.array(a1)
         else:
             a1 = positions[a1]
         distance = np.array([a1 - a0])
         if mic:
             distance, d_len = find_mic(distance, self.cell, self.pbc)
         else:
-            d_len = np.array([np.sqrt((distance ** 2).sum())])
+            d_len = np.array([np.sqrt((distance**2).sum())])
         if vector:
             return distance[0]
 
         return d_len[0]
 
     def get_distances_array(self, p1=None, p2=None, mic=True, vectors=False):
         """
@@ -2042,31 +1993,17 @@
             p2 (numpy.ndarray/list): Nx3 array of positions
             mic (bool): minimum image convention
             vectors (bool): return vectors instead of distances
         Returns:
             numpy.ndarray: NxN if vector=False and NxNx3 if vector=True
 
         """
-        if p1 is None and p2 is not None:
-            p1 = p2
-            p2 = None
-        if p1 is None:
-            p1 = self.positions
-        if p2 is None:
-            p2 = self.positions
-        p1 = np.asarray(p1)
-        p2 = np.asarray(p2)
-        diff_relative = p2.reshape(-1,3)[np.newaxis,:,:]-p1.reshape(-1,3)[:,np.newaxis,:]
-        diff_relative = diff_relative.reshape(p1.shape[:-1]+p2.shape[:-1]+(3,))
-        if not mic:
-            if vectors:
-                return diff_relative
-            else:
-                return np.linalg.norm(diff_relative, axis=-1)
-        return self.find_mic(diff_relative, vectors=vectors)
+        return get_distances_array(
+            structure=self, p1=p1, p2=p2, mic=mic, vectors=vectors
+        )
 
     def append(self, atom):
         if isinstance(atom, ASEAtom):
             super(Atoms, self).append(atom=atom)
         else:
             new_atoms = atom.copy()
             if new_atoms.pbc.all() and np.isclose(new_atoms.get_volume(), 0):
@@ -2087,47 +2024,56 @@
         """
         old_indices = self.indices
         if isinstance(other, Atom):
             other = self.__class__([other])
         elif isinstance(other, ASEAtom):
             other = self.__class__([ase_to_pyiron_atom(other)])
         if not isinstance(other, Atoms) and isinstance(other, ASEAtoms):
-            warnings.warn("Converting ase structure to pyiron before appending the structure")
+            warnings.warn(
+                "Converting ase structure to pyiron before appending the structure"
+            )
             other = ase_to_pyiron(other)
 
         new_indices = other.indices.copy()
         super(Atoms, self).extend(other=other)
         if isinstance(other, Atoms):
             if not np.allclose(self.cell, other.cell):
-                warnings.warn("You are adding structures with different cell shapes. "
-                              "Taking the cell and pbc of the first structure:{}".format(self.cell))
+                warnings.warn(
+                    "You are adding structures with different cell shapes. "
+                    "Taking the cell and pbc of the first structure:{}".format(
+                        self.cell
+                    )
+                )
             if not np.array_equal(self.pbc, other.pbc):
-                warnings.warn("You are adding structures with different periodic boundary conditions. "
-                              "Taking the cell and pbc of the first structure:{}".format(self.cell))
+                warnings.warn(
+                    "You are adding structures with different periodic boundary conditions. "
+                    "Taking the cell and pbc of the first structure:{}".format(
+                        self.cell
+                    )
+                )
             sum_atoms = self
             # sum_atoms = copy(self)
             sum_atoms._tag_list = sum_atoms._tag_list + other._tag_list
             sum_atoms.indices = np.append(sum_atoms.indices, other.indices)
             new_species_lst = copy(sum_atoms.species)
             ind_conv = {}
             for ind_old, el in enumerate(other.species):
                 if el.Abbreviation in sum_atoms._store_elements.keys():
                     ind_new = sum_atoms._species_to_index_dict[
                         sum_atoms._store_elements[el.Abbreviation]
                     ]
                     ind_conv[ind_old] = ind_new
                 else:
                     new_species_lst.append(el)
-                    sum_atoms._store_elements[el.Abbreviation] = el
                     ind_conv[ind_old] = len(new_species_lst) - 1
 
             for key, val in ind_conv.items():
                 new_indices[new_indices == key] = val + 1000
             new_indices = np.mod(new_indices, 1000)
-            sum_atoms.indices[len(old_indices):] = new_indices
+            sum_atoms.indices[len(old_indices) :] = new_indices
             sum_atoms.set_species(new_species_lst)
             if not len(set(sum_atoms.indices)) == len(sum_atoms.species):
                 raise ValueError("Adding the atom instances went wrong!")
         return self
 
     __iadd__ = extend
 
@@ -2143,15 +2089,14 @@
         atoms_new = super(Atoms, self).copy()
         ase_keys = list(ASEAtoms().__dict__.keys())
         ase_keys.append("_pse")
         # Only copy the non ASE keys
         for key, val in self.__dict__.items():
             if key not in ase_keys:
                 atoms_new.__dict__[key] = copy(val)
-        atoms_new._visualize = Visualize(atoms_new)
         atoms_new._analyse = Analyse(atoms_new)
         return atoms_new
 
     def __delitem__(self, key):
         if isinstance(key, (int, np.integer)):
             key = [key]
         key = np.array(key).flatten()
@@ -2170,16 +2115,17 @@
             else:
                 retain_species_indices.append(i)
         new_species = np.array(self.species).copy()[retain_species_indices]
         self.set_species(new_species)
         self.indices = new_indices
 
     def __eq__(self, other):
-        return super(Atoms, self).__eq__(other) and \
-               np.array_equal(self.get_chemical_symbols(), other.get_chemical_symbols())
+        return super(Atoms, self).__eq__(other) and np.array_equal(
+            self.get_chemical_symbols(), other.get_chemical_symbols()
+        )
 
     def __ne__(self, other):
         return not self == other
 
     def __getitem__(self, item):
         new_dict = dict()
         if isinstance(item, int):
@@ -2192,15 +2138,15 @@
             position = self.positions[item]
             return Atom(
                 element=element,
                 position=position,
                 pse=self._pse,
                 index=index,
                 atoms=self,
-                **new_dict
+                **new_dict,
             )
 
         new_array = super(Atoms, self).__getitem__(item)
         new_array.dimension = self.dimension
         if isinstance(item, tuple):
             item = list(item)
         new_indices = self.indices[item].copy()
@@ -2231,17 +2177,14 @@
             new_dir.append(key)
         return new_dir
 
     # def __len__(self):
     #     return len(self.indices)
 
     def __repr__(self):
-        return self.__str__()
-
-    def __str__(self):
         if len(self) == 0:
             return "[]"
         out_str = ""
         for el, pos in zip(self.get_chemical_symbols(), self.positions):
             out_str += el + ": " + str(pos) + "\n"
         if len(self.get_tags()) > 0:
             tags = self.get_tags()
@@ -2252,14 +2195,17 @@
                 )
         if self.cell is not None:
             out_str += "pbc: " + str(self.pbc) + "\n"
             out_str += "cell: \n"
             out_str += str(self.cell) + "\n"
         return out_str
 
+    def __str__(self):
+        return self.get_chemical_formula()
+
     def __setitem__(self, key, value):
         if isinstance(key, (int, np.integer)):
             old_el = self.species[self.indices[key]]
             if isinstance(value, str):
                 el = PeriodicTable().element(value)
             elif isinstance(value, ChemicalElement):
                 el = value
@@ -2367,26 +2313,34 @@
                     self.indices = new_indices.copy()
                     new_species = np.array(new_species)[
                         np.setdiff1d(np.arange(len(new_species)), delete_indices)
                     ].tolist()
                     self.set_species(new_species)
         else:
             raise NotImplementedError()
-
-    __mul__ = repeat
+        # For ASE compatibility
+        self.numbers = self.get_atomic_numbers()
 
     def __imul__(self, vec):
         if isinstance(vec, (int, np.integer)):
             vec = [vec] * self.dimension
         initial_length = len(self)
-        if not hasattr(vec, '__len__'):
-            raise ValueError('Box repetition must be an integer or a list/ndarray of integers and not', type(vec))
+        if not hasattr(vec, "__len__"):
+            raise ValueError(
+                "Box repetition must be an integer or a list/ndarray of integers and not",
+                type(vec),
+            )
 
         if len(vec) != self.dimension:
-            raise AssertionError('Dimension of box repetition not consistent: ', len(vec), '!=', self.dimension)
+            raise AssertionError(
+                "Dimension of box repetition not consistent: ",
+                len(vec),
+                "!=",
+                self.dimension,
+            )
 
         i_vec = np.array([vec[0], 1, 1])
         if self.dimension > 1:
             i_vec[1] = vec[1]
         if self.dimension > 2:
             i_vec[2] = vec[2]
 
@@ -2399,15 +2353,17 @@
         lat = np.array(np.meshgrid(nx_lst, ny_lst, nz_lst)).T.reshape(-1, 3)
         lat_new = np.repeat(lat, len(positions), axis=0)
         new_positions = np.tile(positions, (len(lat), 1)) + lat_new
         new_positions /= np.array(i_vec)
         self.set_cell((self.cell.T * np.array(vec)).T, scale_atoms=True)
         # ASE compatibility
         for name, a in self.arrays.items():
-            self.arrays[name] = np.tile(a, (np.product(vec),) + (1, ) * (len(a.shape) - 1))
+            self.arrays[name] = np.tile(
+                a, (np.product(vec),) + (1,) * (len(a.shape) - 1)
+            )
         self.arrays["positions"] = np.dot(new_positions, self.cell)
         self.indices = np.tile(self.indices, len(lat))
         self._tag_list._length = len(self)
         scale = i_vec[0] * i_vec[1] * i_vec[2]
         for tag in self._tag_list.keys():
             self._tag_list[tag] *= scale
         # Repeating ASE constraints
@@ -2456,74 +2412,97 @@
 
         return el_list
 
     def get_constraint(self):
         if "selective_dynamics" in self._tag_list._lists.keys():
             from ase.constraints import FixAtoms
 
-            return FixAtoms(indices=[atom_ind for atom_ind in
-                                     range(len(self)) if not any(self.selective_dynamics[atom_ind])])
+            return FixAtoms(
+                indices=[
+                    atom_ind
+                    for atom_ind in range(len(self))
+                    if not any(self.selective_dynamics[atom_ind])
+                ]
+            )
         else:
             return None
 
     def set_constraint(self, constraint=None):
         super(Atoms, self).set_constraint(constraint)
         if constraint is not None:
             if constraint.todict()["name"] != "FixAtoms":
-                raise ValueError("Only FixAtoms is supported as ASE compatible constraint.")
+                raise ValueError(
+                    "Only FixAtoms is supported as ASE compatible constraint."
+                )
             if "selective_dynamics" not in self._tag_list._lists.keys():
                 self.add_tag(selective_dynamics=None)
             for atom_ind in range(len(self)):
                 if atom_ind in constraint.index:
                     self.selective_dynamics[atom_ind] = [False, False, False]
                 else:
                     self.selective_dynamics[atom_ind] = [True, True, True]
 
-    def apply_strain(self, epsilon, return_box=False):
+    def apply_strain(self, epsilon, return_box=False, mode="linear"):
         """
-        Apply a given strain on the structure
+        Apply a given strain on the structure. It applies the matrix `F` in the manner:
+
+        ```
+            new_cell = F @ current_cell
+        ```
 
         Args:
-            epsilon (float/list/ndarray): epsilon matrix. If a single number is set, the same strain
-                                          is applied in each direction. If a 3-dim vector is set, it
-                                          will be multiplied by a unit matrix.
+            epsilon (float/list/ndarray): epsilon matrix. If a single number is set, the same
+                strain is applied in each direction. If a 3-dim vector is set, it will be
+                multiplied by a unit matrix.
             return_box (bool): whether to return a box. If set to True, only the returned box will
-                               have the desired strain and the original box will stay unchanged.
+                have the desired strain and the original box will stay unchanged.
+            mode (str): `linear` or `lagrangian`. If `linear`, `F` is equal to the epsilon - 1.
+                If `lagrangian`, epsilon is given by `(F^T * F - 1) / 2`. It raises an error if
+                the strain is not symmetric (if the shear components are given).
         """
         epsilon = np.array([epsilon]).flatten()
         if len(epsilon) == 3 or len(epsilon) == 1:
-            epsilon = epsilon*np.eye(3)
+            epsilon = epsilon * np.eye(3)
         epsilon = epsilon.reshape(3, 3)
         if epsilon.min() < -1.0:
             raise ValueError("Strain value too negative")
         if return_box:
             structure_copy = self.copy()
         else:
             structure_copy = self
         cell = structure_copy.cell.copy()
-        cell = np.matmul(epsilon + np.eye(3), cell)
+        if mode == "linear":
+            F = epsilon + np.eye(3)
+        elif mode == "lagrangian":
+            if not np.allclose(epsilon, epsilon.T):
+                raise ValueError("Strain must be symmetric if `mode = 'lagrangian'`")
+            E, V = np.linalg.eigh(2 * epsilon + np.eye(3))
+            F = np.einsum("ik,k,jk->ij", V, np.sqrt(E), V)
+        else:
+            raise ValueError("mode must be `linear` or `lagrangian`")
+        cell = np.matmul(F, cell)
         structure_copy.set_cell(cell, scale_atoms=True)
         if return_box:
             return structure_copy
 
     def get_spherical_coordinates(self, x=None):
         """
-            Args:
-                x (list/ndarray): coordinates to transform. If not set, the positions
-                                  in structure will be returned.
+        Args:
+            x (list/ndarray): coordinates to transform. If not set, the positions
+                              in structure will be returned.
 
-            Returns:
-                array in spherical coordinates
+        Returns:
+            array in spherical coordinates
         """
         if x is None:
             x = self.positions.copy()
         x = np.array(x).reshape(-1, 3)
         r = np.linalg.norm(x, axis=-1)
-        phi = np.arctan2(x[:,2], x[:,1])
-        theta = np.arctan2(np.linalg.norm(x[:,:2], axis=-1), x[:,2])
+        phi = np.arctan2(x[:, 2], x[:, 1])
+        theta = np.arctan2(np.linalg.norm(x[:, :2], axis=-1), x[:, 2])
         return np.stack((r, theta, phi), axis=-1)
 
     def get_initial_magnetic_moments(self):
         """
         Get array of initial magnetic moments.
 
         Returns:
@@ -2534,20 +2513,24 @@
         else:
             spin_lst = [
                 element.tags["spin"] if "spin" in element.tags.keys() else None
                 for element in self.get_chemical_elements()
             ]
             if any(spin_lst):
                 if (
-                    isinstance(spin_lst, str)
-                    or (
-                        isinstance(spin_lst, (list, np.ndarray))
-                        and isinstance(spin_lst[0], str)
+                    (
+                        isinstance(spin_lst, str)
+                        or (
+                            isinstance(spin_lst, (list, np.ndarray))
+                            and isinstance(spin_lst[0], str)
+                        )
                     )
-                ) and "[" in list(set(spin_lst))[0]:
+                    and list(set(spin_lst))[0] is not None
+                    and "[" in list(set(spin_lst))[0]
+                ):
                     return np.array(
                         [
                             [
                                 float(spin_dir)
                                 for spin_dir in spin.replace("[", "")
                                 .replace("]", "")
                                 .replace(",", "")
@@ -2555,41 +2538,109 @@
                             ]
                             if spin
                             else [0.0, 0.0, 0.0]
                             for spin in spin_lst
                         ]
                     )
                 elif isinstance(spin_lst, (list, np.ndarray)):
-                    return np.array(spin_lst)
+                    return np.array([float(s) if s else 0.0 for s in spin_lst])
                 else:
                     return np.array([float(spin) if spin else 0.0 for spin in spin_lst])
             else:
-                return np.array([None] * len(self))
+                return np.zeros(len(self))
 
     def set_initial_magnetic_moments(self, magmoms=None):
         """
         Set array of initial magnetic moments.
 
         Args:
-            magmoms (numpy.ndarray/list): List of magneric moments
+            magmoms (None/numpy.ndarray/list/dict/float): Default value is
+                None (non magnetic calc). List, dict or single value assigning
+                magnetic moments to the structure object.
+
+        Non-collinear calculations may be specified through using a dict/list
+        (see last example)
+
+        If you want to make it non-magnetic, set `None`
+        >>> structure.set_initial_magnetic_moments(None)
+
+        Example I input: np.ndarray / List
+        Assigns site moments via corresponding list of same length as number
+        of sites in structure
+        >>> from pyiron_atomistics import Project
+        >>> structure = Project('.').create.structure.bulk('Ni', cubic=True)
+        >>> structure[-1] = 'Fe'
+        >>> spin_list = [1, 2, 3, 4]
+        >>> structure.set_initial_magnetic_moments(spin_list)
+        >>> structure.get_initial_magnetic_moments()
+        array([1, 2, 3, 4])
+
+        Example II input: dict
+        Assigns species-specific magnetic moments
+        >>> from pyiron_atomistics import Project
+        >>> structure = Project('.').create.structure.bulk('Ni', cubic=True)
+        >>> structure[-1] = 'Fe'
+        >>> spin_dict = {'Fe': 1, 'Ni': 2}
+        >>> structure.set_initial_magnetic_moments(spin_dict)
+        >>> structure.get_initial_magnetic_moments()
+        array([2, 2, 2, 1])
+
+        Example III input: float
+        Assigns the same magnetic moment to all sites in the structure
+        >>> from pyiron_atomistics import Project
+        >>> structure = Project('.').create.structure.bulk('Ni', cubic=True)
+        >>> structure[-1] = 'Fe'
+        >>> structure.set_initial_magnetic_moments(1)
+        >>> print(structure.get_initial_magnetic_moments())
+        array([1, 1, 1, 1])
+
+        Example IV input: dict/list for non-collinear magmoms.
+        Assigns non-collinear magnetic moments to the sites in structure
+        >>> from pyiron_atomistics import Project
+        >>> structure = Project('.').create.structure.bulk('Ni', cubic=True)
+        >>> structure[-1] = 'Fe'
+
+        Option 1: List input sets vectors for each individual site
+        >>> non_coll_magmom_vect = [[1, 2, 3]
+                                    [2, 3, 4],
+                                    [3, 4, 5],
+                                    [4, 5, 6]]
+        >>> structure.set_initial_magnetic_moments(non_coll_magmom_vect)
+        >>> print(structure.get_initial_magnetic_moments())
+        array([[1, 2, 3], [2, 3, 4], [3, 4, 5], [4, 5, 6]])
+
+        Option 2: Dict input sets magmom vectors for individual species:
+        >>> print(structure.get_initial_magnetic_moments())
+        >>> non_coll_spin_dict = {'Fe': [2, 3, 4], 'Ni': [1, 2, 3]}
+        >>> structure.set_initial_magnetic_moments(non_coll_spin_dict)
+        >>> print(structure.get_initial_magnetic_moments())
+        array([[1, 2, 3], [1, 2, 3], [1, 2, 3], [2, 3, 4]])
         """
         # pyiron part
         if magmoms is not None:
+            if isinstance(magmoms, dict):
+                if set(self.get_species_symbols()) != set(magmoms.keys()):
+                    raise ValueError(
+                        "Elements in structure {} not found in dict {}".format(
+                            set(self.get_chemical_symbols()), set(magmoms.keys())
+                        )
+                    )
+                magmoms = [magmoms[c] for c in self.get_chemical_symbols()]
+            elif not isinstance(magmoms, (np.ndarray, Sequence)):
+                magmoms = len(self) * [magmoms]
             if len(magmoms) != len(self):
-                raise ValueError("magmons can be collinear or non-collinear.")
-            for ind, element in enumerate(self.get_chemical_elements()):
-                if "spin" in element.tags.keys():
-                    self[ind] = element.Parent
+                raise ValueError("magmoms can be collinear or non-collinear.")
             if "spin" not in self._tag_list._lists.keys():
                 self.add_tag(spin=None)
             for ind, spin in enumerate(magmoms):
-                self.spin[ind] = spin
-        self.spins = magmoms
+                self.spin[ind] = spin  # For self._tag_list.spin
+        self.spins = magmoms  # For self.array['initial_magmoms']
 
-    def rotate(self, a=0.0, v=None, center=(0, 0, 0), rotate_cell=False, index_list=None
+    def rotate(
+        self, a=0.0, v=None, center=(0, 0, 0), rotate_cell=False, index_list=None
     ):
         """
         Rotate atoms based on a vector and an angle, or two vectors. This function is completely adopted from ASE code
         (https://wiki.fysik.dtu.dk/ase/_modules/ase/atoms.html#Atoms.rotate)
 
         Args:
 
@@ -2628,14 +2679,26 @@
         if index_list is None:
             super(Atoms, self).rotate(a=a, v=v, center=center, rotate_cell=rotate_cell)
         else:
             dummy_basis = copy(self)
             dummy_basis.rotate(a=a, v=v, center=center, rotate_cell=rotate_cell)
             self.positions[index_list] = dummy_basis.positions[index_list]
 
+    def to_ase(self):
+        return pyiron_to_ase(self)
+
+    def to_pymatgen(self):
+        return pyiron_to_pymatgen(self)
+
+    def to_ovito(self):
+        return pyiron_to_ovito(self)
+
+    def to_pyscal_system(self):
+        return pyiron_to_pyscal_system(self)
+
 
 class _CrystalStructure(Atoms):
     """
     only for historical reasons
 
     Args:
         element:
@@ -2653,17 +2716,16 @@
         element="Fe",
         bravais_lattice="cubic",
         bravais_basis="primitive",
         lattice_constants=None,  # depending on symmetry length and angles
         dimension=3,
         rel_coords=True,
         pse=None,
-        **kwargs
+        **kwargs,
     ):
-
         # print "basis0"
         # allow also for scalar input for LatticeConstants (for a cubic system)
         if lattice_constants is None:
             lattice_constants = [1.0]
         try:
             test = lattice_constants[0]
         except (TypeError, IndexError):
@@ -2868,17 +2930,15 @@
                 raise ValueError(
                     "Only centered and primitive cells are supported for 2D."
                 )
         elif self.dimension == 1:
             if self.bravais_basis == "primitive":
                 basis = np.array([[0.0]])
             else:
-                raise ValueError(
-                    "Only primitive cells are supported for 1D."
-                )
+                raise ValueError("Only primitive cells are supported for 1D.")
         self.coordinates = basis
 
     # ########################### get commmands ########################
     def get_lattice_types(self):
         """
 
         Returns:
@@ -3123,18 +3183,14 @@
     Args:
         ase_obj(ase.atoms.Atoms): The ase atoms instance to convert
 
     Returns:
         pyiron.atomistics.structure.atoms.Atoms: The equivalent pyiron structure
 
     """
-    try:
-        import ase
-    except ImportError:
-        raise ValueError("ASE package not yet installed")
     element_list = ase_obj.get_chemical_symbols()
     cell = ase_obj.cell
     positions = ase_obj.get_positions()
     pbc = ase_obj.get_pbc()
     spins = ase_obj.get_initial_magnetic_moments()
     if all(spins == np.array(None)) or sum(np.abs(spins)) == 0.0:
         pyiron_atoms = Atoms(
@@ -3167,18 +3223,14 @@
                 ] = constraint_dict["kwargs"]["mask"]
             else:
                 warnings.warn("Unsupported ASE constraint: " + constraint_dict["name"])
     return pyiron_atoms
 
 
 def pyiron_to_ase(pyiron_obj):
-    try:
-        from pyiron_atomistics.atomistics.structure.pyironase import ASEAtoms
-    except ImportError:
-        raise ValueError("ASE package not yet installed")
     element_list = pyiron_obj.get_parent_symbols()
     cell = pyiron_obj.cell
     positions = pyiron_obj.positions
     pbc = pyiron_obj.get_pbc()
     spins = pyiron_obj.get_initial_magnetic_moments()
     if all(spins == np.array(None)) or sum(np.abs(spins)) == 0.0:
         atoms = ASEAtoms(symbols=element_list, positions=positions, pbc=pbc, cell=cell)
@@ -3219,48 +3271,68 @@
         warnings.warn("Cell is not periodic: " + str(atoms.__dict__["_pbc"]))
     if not len(array_keys) == 0:
         warnings.warn("Found unknown flags: " + str(array_keys))
     if not atoms.__dict__["info"] == dict():
         warnings.warn("Info is not empty: " + str(atoms.__dict__["info"]))
 
 
-def pymatgen_to_pyiron(pymatgen_obj):
+def pymatgen_to_pyiron(structure):
     """
-    Convert pymatgen atoms object to pyiron atoms object (pymatgen->ASE->pyiron)
+        Convert pymatgen Structure object to pyiron atoms object (pymatgen->ASE->pyiron)
 
     Args:
-        pymatgen_obj: pymatgen atoms object
+        pymatgen_obj: pymatgen Structure object
 
     Returns:
         pyiron atoms object
     """
-    try:
-        from pymatgen.io.ase import AseAtomsAdaptor
-    except ImportError:
-        raise ValueError("PyMatGen package not yet installed")
-    return ase_to_pyiron(AseAtomsAdaptor().get_atoms(structure=pymatgen_obj))
+    # This workaround is necessary because ASE refuses to accept limited degrees of freedom in their atoms object
+    # e.g. only accepts [T T T] or [F F F] but rejects [T, T, F] etc.
+    # Have to check for the property explicitly otherwise it just straight crashes
+    # Let's just implement this workaround if any selective dynamics are present
+    if "selective_dynamics" in structure.site_properties.keys():
+        sel_dyn_list = structure.site_properties["selective_dynamics"]
+        struct = structure.copy()
+        struct.remove_site_property("selective_dynamics")
+        pyiron_atoms = ase_to_pyiron(AseAtomsAdaptor().get_atoms(structure=struct))
+        pyiron_atoms.add_tag(selective_dynamics=[True, True, True])
+        for i, _ in enumerate(pyiron_atoms):
+            pyiron_atoms.selective_dynamics[i] = sel_dyn_list[i]
+    else:
+        pyiron_atoms = ase_to_pyiron(AseAtomsAdaptor().get_atoms(structure=structure))
+    return pyiron_atoms
 
 
 def pyiron_to_pymatgen(pyiron_obj):
     """
-    Convert pyiron atoms object to pymatgen atoms object
+    Convert pyiron atoms object to pymatgen Structure object
 
     Args:
         pyiron_obj: pyiron atoms object
 
     Returns:
-        pymatgen atoms object
+        pymatgen Structure object
     """
-    try:
-        from pymatgen.io.ase import AseAtomsAdaptor
-    except ImportError:
-        raise ValueError("PyMatGen package not yet installed")
-    ase_atoms = pyiron_to_ase(pyiron_obj)
-    _check_if_simple_atoms(atoms=ase_atoms)
-    return AseAtomsAdaptor().get_structure(atoms=ase_atoms, cls=None)
+    pyiron_obj_conv = pyiron_obj.copy()  # necessary to avoid changing original object
+    # This workaround is necessary because ASE refuses to accept limited degrees of freedom in their atoms object
+    # e.g. only accepts [T T T] or [F F F] but rejects [T, T, F] etc.
+    # Let's just implement this workaround if any selective dynamics are present
+    if hasattr(pyiron_obj, "selective_dynamics"):
+        sel_dyn_list = pyiron_obj.selective_dynamics
+        pyiron_obj_conv.selective_dynamics = [True, True, True]
+        ase_obj = pyiron_to_ase(pyiron_obj_conv)
+        pymatgen_obj_conv = AseAtomsAdaptor().get_structure(atoms=ase_obj)
+        new_site_properties = pymatgen_obj_conv.site_properties
+        new_site_properties["selective_dynamics"] = sel_dyn_list
+        pymatgen_obj = pymatgen_obj_conv.copy(site_properties=new_site_properties)
+    else:
+        ase_obj = pyiron_to_ase(pyiron_obj_conv)
+        _check_if_simple_atoms(atoms=ase_obj)
+        pymatgen_obj = AseAtomsAdaptor().get_structure(atoms=ase_obj)
+    return pymatgen_obj
 
 
 def ovito_to_pyiron(ovito_obj):
     """
 
     Args:
         ovito_obj:
@@ -3358,15 +3430,15 @@
     """
     pse = PeriodicTable()
     df = pse.dataframe.T
     if isinstance(symbols, str):
         symbols = string2symbols(symbols)
     numbers = list()
     for sym in symbols:
-        if isinstance(sym, string_types):
+        if isinstance(sym, str):
             numbers.append(df[sym]["AtomicNumber"])
         else:
             numbers.append(sym)
     return numbers
 
 
 def string2vector(v):
@@ -3411,7 +3483,47 @@
                 allnone = False
         if allnone:
             return None
         return newdata
     else:
         return data
 
+
+class Symbols(ASESymbols):
+
+    """
+    Derived from the ase symbols class which has the following docs:
+
+    Args:
+        numbers list/numpy.ndarray): List of atomic numbers
+    """
+
+    def __init__(self, numbers):
+        self.__doc__ = self.__doc__ + "\n" + super().__doc__
+        super().__init__(numbers)
+        self._structure = None
+
+    @property
+    def structure(self):
+        """
+        The structure to which the symbol is assigned to
+
+        Returns:
+            pyiron_atomistics.atomistics.structure.atoms.Atoms: The required structure
+        """
+        return self._structure
+
+    @structure.setter
+    def structure(self, val):
+        self._structure = val
+
+    def __setitem__(self, key, value):
+        super().__setitem__(key, value)
+        if self._structure is not None:
+            index_array = np.argwhere(
+                self.numbers != self._structure.get_atomic_numbers()
+            ).flatten()
+            replace_elements = self.structure.numbers_to_elements(
+                self.numbers[index_array]
+            )
+            for i, el in enumerate(replace_elements):
+                self._structure[index_array[i]] = el
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/factories/aimsgb.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/aimsgb.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
-from aimsgb import GrainBoundary, Grain, GBInformation
-from pyiron_base import Settings
-from pyiron_atomistics.atomistics.structure.atoms import pyiron_to_pymatgen, pymatgen_to_pyiron
+from structuretoolkit.build import grainboundary, get_grainboundary_info
+from pyiron_atomistics.atomistics.structure.atoms import ase_to_pyiron
 
 __author__ = "Ujjal Saikia"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Liam Huber"
 __email__ = "huber@mpie.de"
 __status__ = "production"
 __date__ = "Feb 26, 2021"
 
-s = Settings()
-
 
 class AimsgbFactory:
     @staticmethod
     def info(axis, max_sigma):
         """
         Provides a list of possible GB structures for a given rotational axis and upto the given maximum sigma value.
 
@@ -38,25 +35,27 @@
                 'plane': the GB planes")
                 'rot_matrix': array([the rotational matrix]),
                 'csl': [array([the csl matrix])]}}
 
         To construct the grain boundary select a GB plane and sigma value from the list and pass it to the
         GBBuilder.gb_build() function along with the rotational axis and initial bulk structure.
         """
-        return GBInformation(axis=axis, max_sigma=max_sigma)
+        return get_grainboundary_info(axis=axis, max_sigma=max_sigma)
 
     @staticmethod
     def build(
-            axis,
-            sigma,
-            plane,
-            initial_struct,
-            to_primitive=False,
-            delete_layer='0b0t0b0t',
-            add_if_dist=0.0
+        axis,
+        sigma,
+        plane,
+        initial_struct,
+        to_primitive=False,
+        delete_layer="0b0t0b0t",
+        add_if_dist=0.0,
+        uc_a=1,
+        uc_b=1,
     ):
         """
         Generate a grain boundary structure based on the aimsgb.GrainBoundary module.
 
         Args:
             axis : Rotational axis for the GB you want to construct (for example, axis=[1,0,0])
             sigma (int) : The sigma value of the GB you want to construct (for example, sigma=5)
@@ -69,17 +68,26 @@
                            to be deleted. The first t and second b from the left hand side represents
                            the layers at the GB interface. Default value is delete_layer='0b0t0b0t', which
                            means no deletion of layers.
             add_if_dist : If you want to add extra interface distance, you can specify add_if_dist.
                            Default value is add_if_dist=0.0
             to_primitive : To generate primitive or non-primitive GB structure. Default value is
                             to_primitive=False
+            uc_a (int): Number of unit cell of grain A. Default to 1.
+            uc_b (int): Number of unit cell of grain B. Default to 1.
 
         Returns:
             :class:`.Atoms`: final grain boundary structure
         """
-        basis_pymatgen = pyiron_to_pymatgen(initial_struct)
-        grain_init = Grain(basis_pymatgen.lattice, basis_pymatgen.species, basis_pymatgen.frac_coords)
-        gb_obj = GrainBoundary(axis=axis, sigma=sigma, plane=plane, initial_struct=grain_init)
-
-        return pymatgen_to_pyiron(gb_obj.build_gb(to_primitive=to_primitive, delete_layer=delete_layer,
-                                                  add_if_dist=add_if_dist))
+        return ase_to_pyiron(
+            grainboundary(
+                axis=axis,
+                sigma=sigma,
+                plane=plane,
+                initial_struct=initial_struct,
+                to_primitive=to_primitive,
+                delete_layer=delete_layer,
+                add_if_dist=add_if_dist,
+                uc_a=uc_a,
+                uc_b=uc_b,
+            )
+        )
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/factories/ase.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/ase.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from functools import wraps
 from inspect import getmodule
-from ase.build import cut as ase_cut, stack as ase_stack, bulk as ase_bulk
+from ase.build import (
+    cut as ase_cut,
+    stack as ase_stack,
+    bulk as ase_bulk,
+    molecule as ase_molecule,
+)
 from ase.io import read as ase_read
 from ase.spacegroup import crystal as ase_crystal
 from pyiron_atomistics.atomistics.structure.atoms import ase_to_pyiron
-from pyiron_atomistics.atomistics.structure.pyironase import publication as publication_ase
-from pyiron_base import Settings
+from pyiron_atomistics.atomistics.structure.pyironase import (
+    publication as publication_ase,
+)
+from pyiron_base import state
 
 __author__ = "Ali Zendegani"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0.1"
 __maintainer__ = "Liam Huber"
 __email__ = "huber@mpie.de"
 __status__ = "production"
 __date__ = "Feb 26, 2021"
 
-s = Settings()
-
 
 def _ase_header(ase_func):
     chain = getmodule(ase_func).__name__
-    name = chain.split('.')[-1]
+    name = chain.split(".")[-1]
     return f"""
     Returns an ASE's {name} result as a `pyiron_atomistics.atomstic.structure.atoms.Atoms`.
 
     {chain} docstring:
 
     """
 
 
 def _ase_wraps(ase_func):
     def decorator(func):
         @wraps(ase_func)
         def wrapper(*args, **kwargs):
-            s.publication_add(publication_ase())
+            state.publications.add(publication_ase())
             return func(*args, **kwargs)
+
         wrapper.__doc__ = _ase_header(ase_func) + wrapper.__doc__
         return wrapper
+
     return decorator
 
 
 class AseFactory:
     @_ase_wraps(ase_bulk)
     def bulk(self, *args, **kwargs):
         return ase_to_pyiron(ase_bulk(*args, **kwargs))
@@ -63,7 +70,11 @@
     @_ase_wraps(ase_crystal)
     def crystal(self, *args, **kwargs):
         return ase_to_pyiron(ase_crystal(*args, **kwargs))
 
     @_ase_wraps(ase_read)
     def read(self, *args, **kwargs):
         return ase_to_pyiron(ase_read(*args, **kwargs))
+
+    @_ase_wraps(ase_molecule)
+    def molecule(self, *args, **kwargs):
+        return ase_to_pyiron(ase_molecule(*args, **kwargs))
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/factory.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,155 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from ase.build import (
-        add_adsorbate,
-        add_vacuum,
-        bcc100,
-        bcc110,
-        bcc111,
-        diamond100,
-        diamond111,
-        fcc100,
-        fcc110,
-        fcc111,
-        fcc211,
-        hcp0001,
-        hcp10m10,
-        mx2,
-        hcp0001_root,
-        fcc111_root,
-        bcc111_root,
-        root_surface,
-        root_surface_analysis,
-        surface as ase_surf
+    add_adsorbate,
+    add_vacuum,
+    bcc100,
+    bcc110,
+    bcc111,
+    diamond100,
+    diamond111,
+    fcc100,
+    fcc110,
+    fcc111,
+    fcc211,
+    hcp0001,
+    hcp10m10,
+    mx2,
+    hcp0001_root,
+    fcc111_root,
+    bcc111_root,
+    root_surface,
+    root_surface_analysis,
+    surface as ase_surf,
 )
 import numpy as np
+from structuretoolkit.build import (
+    high_index_surface,
+    get_high_index_surface_info,
+)
 from pyiron_atomistics.atomistics.structure.factories.ase import AseFactory
+from pyiron_atomistics.atomistics.structure.factories.atomsk import (
+    AtomskFactory,
+    _ATOMSK_EXISTS,
+)
 from pyiron_atomistics.atomistics.structure.factories.aimsgb import AimsgbFactory
-from pyiron_atomistics.atomistics.structure.pyironase import publication as publication_ase
-from pyiron_atomistics.atomistics.structure.atoms import CrystalStructure, ase_to_pyiron, Atoms
+from pyiron_atomistics.atomistics.structure.factories.compound import CompoundFactory
+from pyiron_atomistics.atomistics.structure.factories.materialsproject import (
+    MaterialsProjectFactory,
+)
+from pyiron_atomistics.atomistics.structure.pyironase import (
+    publication as publication_ase,
+)
+from pyiron_atomistics.atomistics.structure.atoms import (
+    CrystalStructure,
+    Atoms,
+    ase_to_pyiron,
+    pymatgen_to_pyiron,
+    ovito_to_pyiron,
+)
+from pymatgen.core import Structure
 from pyiron_atomistics.atomistics.structure.periodic_table import PeriodicTable
-from pyiron_base import Settings, PyironFactory, deprecate
+from pyiron_base import state, PyironFactory, deprecate
 import types
+from functools import wraps
 
 __author__ = "Sudarsan Surendralal"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Sudarsan Surendralal"
 __email__ = "surendralal@mpie.de"
 __status__ = "production"
 __date__ = "May 1, 2020"
 
-s = Settings()
-
 
 class StructureFactory(PyironFactory):
     def __init__(self):
         self._ase = AseFactory()
+        if _ATOMSK_EXISTS:
+            self._atomsk = AtomskFactory()
         self._aimsgb = AimsgbFactory()
+        self._materialsproject = MaterialsProjectFactory()
+        self._compound = CompoundFactory()
 
     @property
     def ase(self):
         return self._ase
 
+    if _ATOMSK_EXISTS:
+
+        @property
+        def atomsk(self):
+            return self._atomsk
+
     @property
     def aimsgb(self):
         return self._aimsgb
 
+    @property
+    def compound(self):
+        return self._compound
+
     def cut(self, *args, **kwargs):
         return self.ase.cut(*args, **kwargs)
+
     cut.__doc__ = AseFactory.cut.__doc__
 
     def stack(self, *args, **kwargs):
         return self.ase.stack(*args, **kwargs)
+
     stack.__doc__ = AseFactory.stack.__doc__
 
     def read(self, *args, **kwargs):
-        return self.ase.read(*args, **kwargs)
+        # This looks weird, but it's because ASE doesn't handle selective dynamics properly, so we replace it with the pymatgen read equivalent.
+        try:
+            structure = self.read_using_pymatgen(*args, **kwargs)
+        except (ValueError, TypeError):
+            # For stuff that pymatgen can't read it raises
+            # ValueError: Unrecognized file extension!
+            # backwards compatibility for notebooks.
+            # TypeError: IStructure.from_file() got an unexpected keyword argument 'format'
+            structure = self.read_using_ase(*args, **kwargs)
+        return structure
+
     read.__doc__ = AseFactory.read.__doc__
 
+    def read_using_pymatgen(self, *args, **kwargs):
+        return pymatgen_to_pyiron(Structure.from_file(*args, **kwargs))
+
+    def read_using_ase(self, *args, **kwargs):
+        return self.ase.read(*args, **kwargs)
+
     @deprecate(message="Please use .read or .ase.read", version="0.2.2")
     def ase_read(self, *args, **kwargs):
         return self.ase.read(*args, **kwargs)
+
     ase_read.__doc__ = AseFactory.read.__doc__
 
     @deprecate(message="Please use .bulk or .ase.bulk", version="0.2.2")
     def ase_bulk(self, *args, **kwargs):
         return self.ase.bulk(*args, **kwargs)
+
     ase_bulk.__doc__ = AseFactory.bulk.__doc__
 
     def bulk(
-            self,
-            name,
-            crystalstructure=None,
-            a=None,
-            c=None,
-            covera=None,
-            u=None,
-            orthorhombic=False,
-            cubic=False,
+        self,
+        name,
+        crystalstructure=None,
+        a=None,
+        c=None,
+        covera=None,
+        u=None,
+        orthorhombic=False,
+        cubic=False,
     ):
         """
         Creating bulk systems (using ASE bulk module). Crystal structure and lattice constant(s) will be guessed if not
         provided.
 
         name (str): Chemical symbol or symbols as in 'MgO' or 'NaCl'.
         crystalstructure (str): Must be one of sc, fcc, bcc, hcp, diamond, zincblende,
@@ -119,15 +173,21 @@
             u=u,
             orthorhombic=orthorhombic,
             cubic=cubic,
         )
 
     @staticmethod
     def surface(
-        element, surface_type, size=(1, 1, 1), vacuum=1.0, center=False, pbc=True, **kwargs
+        element,
+        surface_type,
+        size=(1, 1, 1),
+        vacuum=1.0,
+        center=False,
+        pbc=True,
+        **kwargs,
     ):
         """
         Generate a surface based on the ase.build.surface module.
 
         Args:
             element (str): Element name
             surface_type (str): The string specifying the surface type generators available through ase (fcc111,
@@ -143,15 +203,15 @@
         Returns:
             pyiron_atomistics.atomistics.structure.atoms.Atoms instance: Required surface
 
         """
         # https://gitlab.com/ase/ase/blob/master/ase/lattice/surface.py
         if pbc is None:
             pbc = True
-        s.publication_add(publication_ase())
+        state.publications.add(publication_ase())
         for surface_class in [
             add_adsorbate,
             add_vacuum,
             bcc100,
             bcc110,
             bcc111,
             diamond100,
@@ -201,21 +261,21 @@
             center (bool): shift all positions to center the surface
                 in the cell
 
         Returns:
             pyiron_atomistics.atomistics.structure.atoms.Atoms instance: Required surface
         """
         # https://gitlab.com/ase/ase/blob/master/ase/lattice/surface.py
-        s.publication_add(publication_ase())
+        state.publications.add(publication_ase())
 
         surface = ase_surf(lattice, hkl, layers)
         z_max = np.max(surface.positions[:, 2])
         surface.cell[2, 2] = z_max + vacuum
         if center:
-            surface.positions += 0.5 * surface.cell[2] - [0, 0, z_max/2]
+            surface.positions += 0.5 * surface.cell[2] - [0, 0, z_max / 2]
         surface.pbc = pbc
         return ase_to_pyiron(surface)
 
     @staticmethod
     def crystal(element, bravais_basis, lattice_constant):
         """
         Create a crystal structure using pyiron's native crystal structure generator
@@ -232,34 +292,34 @@
             element=element,
             bravais_basis=bravais_basis,
             lattice_constants=[lattice_constant],
         )
 
     @staticmethod
     def atoms(
-            symbols=None,
-            positions=None,
-            numbers=None,
-            tags=None,
-            momenta=None,
-            masses=None,
-            magmoms=None,
-            charges=None,
-            scaled_positions=None,
-            cell=None,
-            pbc=None,
-            celldisp=None,
-            constraint=None,
-            calculator=None,
-            info=None,
-            indices=None,
-            elements=None,
-            dimension=None,
-            species=None,
-            **qwargs
+        symbols=None,
+        positions=None,
+        numbers=None,
+        tags=None,
+        momenta=None,
+        masses=None,
+        magmoms=None,
+        charges=None,
+        scaled_positions=None,
+        cell=None,
+        pbc=None,
+        celldisp=None,
+        constraint=None,
+        calculator=None,
+        info=None,
+        indices=None,
+        elements=None,
+        dimension=None,
+        species=None,
+        **qwargs,
     ):
         """
         Creates a atomistics.structure.atoms.Atoms instance.
 
         Args:
             elements (list/numpy.ndarray): List of strings containing the elements or a list of
                                 atomistics.structure.periodic_table.ChemicalElement instances
@@ -303,15 +363,15 @@
             constraint=constraint,
             calculator=calculator,
             info=info,
             indices=indices,
             elements=elements,
             dimension=dimension,
             species=species,
-            **qwargs
+            **qwargs,
         )
 
     @staticmethod
     def element(parent_element, new_element_name=None, spin=None, potential_file=None):
         """
 
         Args:
@@ -323,15 +383,15 @@
         Returns:
             atomistics.structure.periodic_table.ChemicalElement instance
         """
         periodic_table = PeriodicTable()
         if new_element_name is None:
             if spin is not None:
                 new_element_name = (
-                        parent_element + "_spin_" + str(spin).replace(".", "_")
+                    parent_element + "_spin_" + str(spin).replace(".", "_")
                 )
             else:
                 new_element_name = parent_element + "_1"
         if potential_file is not None:
             if spin is not None:
                 periodic_table.add_element(
                     parent_element=parent_element,
@@ -355,31 +415,155 @@
             periodic_table.add_element(
                 parent_element=parent_element, new_element=new_element_name
             )
         return periodic_table.element(new_element_name)
 
     @deprecate(message="Use .aimsgb.info", version="0.2.2")
     def aimsgb_info(self, axis, max_sigma):
-        self.aimsgb.info(axis=axis, max_sigma=max_sigma)
+        return self.aimsgb.info(axis=axis, max_sigma=max_sigma)
+
     aimsgb_info.__doc__ = AimsgbFactory.info.__doc__
 
     @deprecate(message="Use .aimsgb.build", version="0.2.2")
     def aimsgb_build(
-            self,
-            axis,
-            sigma,
-            plane,
-            initial_struct,
-            to_primitive=False,
-            delete_layer='0b0t0b0t',
-            add_if_dist=0.0
+        self,
+        axis,
+        sigma,
+        plane,
+        initial_struct,
+        to_primitive=False,
+        delete_layer="0b0t0b0t",
+        add_if_dist=0.0,
     ):
         return self.aimsgb.build(
             axis=axis,
             sigma=sigma,
             plane=plane,
             initial_struct=initial_struct,
             to_primitive=to_primitive,
             delete_layer=delete_layer,
-            add_if_dist=add_if_dist
+            add_if_dist=add_if_dist,
         )
+
     aimsgb_build.__doc__ = AimsgbFactory.build.__doc__
+
+    @staticmethod
+    @wraps(ase_to_pyiron)
+    def from_ase(ase_atoms):
+        return ase_to_pyiron(ase_atoms)
+
+    @staticmethod
+    @wraps(pymatgen_to_pyiron)
+    def from_pymatgen(pymatgen_obj):
+        return pymatgen_to_pyiron(pymatgen_obj)
+
+    @staticmethod
+    @wraps(ovito_to_pyiron)
+    def from_ovito(ovito_obj):
+        return ovito_to_pyiron(ovito_obj)
+
+    def high_index_surface_info(
+        self,
+        element,
+        crystal_structure,
+        lattice_constant,
+        terrace_orientation=None,
+        step_orientation=None,
+        kink_orientation=None,
+        step_down_vector=None,
+        length_step=3,
+        length_terrace=3,
+        length_kink=1,
+    ):
+        """
+        Gives the miller indices of high index surface required to create a stepped and kink surface, based
+        on the general orientation and length of terrace, step and kinks respectively. The microfacet notation used is
+        based on the work of Van Hove et al.,[1].
+
+        [1] Van Hove, M. A., and G. A. Somorjai. "A new microfacet notation for high-Miller-index surfaces of cubic
+        materials with terrace, step and kink structures." Surface Science 92.2-3 (1980): 489-518.
+
+        Args:
+            element (str): The parent element eq. "N", "O", "Mg" etc.
+            crystal_structure (str): The crystal structure of the lattice
+            lattice_constant (float): The lattice constant
+            terrace_orientation (list): The miller index of the terrace eg., [1,1,1]
+            step_orientation (list): The miller index of the step eg., [1,1,0]
+            kink_orientation (list): The miller index of the kink eg., [1,1,1]
+            step_down_vector (list): The direction for stepping down from the step to next terrace eg., [1,1,0]
+            length_terrace (int): The length of the terrace along the kink direction in atoms eg., 3
+            length_step (int): The length of the step along the step direction in atoms eg., 3
+            length_kink (int): The length of the kink along the kink direction in atoms eg., 1
+
+
+        Returns:
+            high_index_surface: The high miller index surface which can be used to create slabs
+            fin_kink_orientation: The kink orientation lying in the terrace
+            fin_step_orientation: The step orientation lying in the terrace
+        """
+        return get_high_index_surface_info(
+            element=element,
+            crystal_structure=crystal_structure,
+            lattice_constant=lattice_constant,
+            terrace_orientation=terrace_orientation,
+            step_orientation=step_orientation,
+            kink_orientation=kink_orientation,
+            step_down_vector=step_down_vector,
+            length_step=length_step,
+            length_terrace=length_terrace,
+            length_kink=length_kink,
+        )
+
+    def high_index_surface(
+        self,
+        element,
+        crystal_structure,
+        lattice_constant,
+        terrace_orientation=None,
+        step_orientation=None,
+        kink_orientation=None,
+        step_down_vector=None,
+        length_step=3,
+        length_terrace=3,
+        length_kink=1,
+        layers=60,
+        vacuum=10,
+    ):
+        """
+        Gives a slab positioned at the bottom with the high index surface computed by high_index_surface_info().
+        Args:
+            element (str): The parent element eq. "N", "O", "Mg" etc.
+            crystal_structure (str): The crystal structure of the lattice
+            lattice_constant (float): The lattice constant
+            terrace_orientation (list): The miller index of the terrace. default: [1,1,1]
+            step_orientation (list): The miller index of the step. default: [1,1,0]
+            kink_orientation (list): The miller index of the kink. default: [1,1,1]
+            step_down_vector (list): The direction for stepping down from the step to next terrace. default: [1,1,0]
+            length_terrace (int): The length of the terrace along the kink direction in atoms. default: 3
+            length_step (int): The length of the step along the step direction in atoms. default: 3
+            length_kink (int): The length of the kink along the kink direction in atoms. default: 1
+            layers (int): Number of layers of the high_index_surface. default: 60
+            vacuum (float): Thickness of vacuum on the top of the slab. default:10
+
+        Returns:
+            slab: pyiron_atomistics.atomistics.structure.atoms.Atoms instance Required surface
+        """
+        return ase_to_pyiron(
+            high_index_surface(
+                element=element,
+                crystal_structure=crystal_structure,
+                lattice_constant=lattice_constant,
+                terrace_orientation=terrace_orientation,
+                step_orientation=step_orientation,
+                kink_orientation=kink_orientation,
+                step_down_vector=step_down_vector,
+                length_step=length_step,
+                length_terrace=length_terrace,
+                length_kink=length_kink,
+                layers=layers,
+                vacuum=vacuum,
+            )
+        )
+
+    @property
+    def materialsproject(self):
+        return self._materialsproject
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/periodic_table.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/periodic_table.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from __future__ import print_function, unicode_literals
 import numpy as np
 import os
-from pyiron_base import Settings
-from mendeleev import element
-import sys
+from pyiron_base import state
+import mendeleev
 import pandas
+from functools import lru_cache
 
 __author__ = "Joerg Neugebauer, Sudarsan Surendralal, Martin Boeckmann"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Sudarsan Surendralal"
 __email__ = "surendralal@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
-s = Settings()
 pandas.options.mode.chained_assignment = None
 
 
+@lru_cache(maxsize=118)
+def element(*args):
+    return mendeleev.element(*args)
+
+
 class ChemicalElement(object):
     """
     An Object which contains the element specific parameters
     """
 
     def __init__(self, sub):
         """
@@ -43,52 +47,64 @@
             self._init_mendeleev(self.sub)
         elif "Parent" in self.sub.index and isinstance(self.sub.Parent, stringtypes):
             self._init_mendeleev(self.sub.Parent)
         elif len(self.sub) > 0:
             self._init_mendeleev(self.sub.Abbreviation)
 
         self._mendeleev_translation_dict = {
-            'AtomicNumber': 'atomic_number',
-            'AtomicRadius': 'covalent_radius_cordero',
-            'AtomicMass': 'mass',
-            'Color': 'cpk_color',
-            'CovalentRadius': 'covalent_radius',
-            'CrystalStructure': 'lattice_structure',
-            'Density': 'density',
-            'DiscoveryYear': 'discovery_year',
-            'ElectronAffinity': 'electron_affinity',
-            'Electronegativity': 'electronegativity',
-            'Group': 'group_id',
-            'Name': 'name',
-            'Period': 'period',
-            'StandardName': 'name',
-            'VanDerWaalsRadius': 'vdw_radius',
-            'MeltingPoint': 'melting_point'
+            "AtomicNumber": "atomic_number",
+            "AtomicRadius": "covalent_radius_cordero",
+            "AtomicMass": "mass",
+            "Color": "cpk_color",
+            "CovalentRadius": "covalent_radius",
+            "CrystalStructure": "lattice_structure",
+            "Density": "density",
+            "DiscoveryYear": "discovery_year",
+            "ElectronAffinity": "electron_affinity",
+            "Electronegativity": "electronegativity",
+            "Group": "group_id",
+            "Name": "name",
+            "Period": "period",
+            "StandardName": "name",
+            "VanDerWaalsRadius": "vdw_radius",
+            "MeltingPoint": "melting_point",
         }
         self.el = None
 
     def _init_mendeleev(self, element_str):
         self._mendeleev_element = element(str(element_str))
-        self._mendeleev_property_lst = [s for s in dir(self._mendeleev_element) if not s.startswith('_')]
+        self._mendeleev_property_lst = [
+            s for s in dir(self._mendeleev_element) if not s.startswith("_")
+        ]
 
     def __getattr__(self, item):
         if item in ["__array_struct__", "__array_interface__", "__array__"]:
             raise AttributeError
         return self[item]
 
     def __getitem__(self, item):
         if item in self._mendeleev_translation_dict.keys():
             item = self._mendeleev_translation_dict[item]
         if item in self._mendeleev_property_lst:
             return getattr(self._mendeleev_element, item)
         if item in self.sub.index:
             return self.sub[item]
 
+    def __setstate__(self, state):
+        self.__dict__.update(state)
+
+    def __getstate__(self):
+        # Only necessary to support pickling in python <3.11
+        # https://docs.python.org/release/3.11.2/library/pickle.html#object.__getstate__
+        return self.__dict__
+
     def __eq__(self, other):
-        if isinstance(other, self.__class__):
+        if self is other:
+            return True
+        elif isinstance(other, self.__class__):
             conditions = list()
             conditions.append(self.sub.to_dict() == other.sub.to_dict())
             return all(conditions)
         elif isinstance(other, (np.ndarray, list)):
             conditions = list()
             for sp in other:
                 conditions.append(self.sub.to_dict() == sp.sub.to_dict())
@@ -211,29 +227,40 @@
 
     def __getitem__(self, item):
         if item in self.dataframe.columns.values:
             return self.dataframe[item]
         if item in self.dataframe.index.values:
             return self.dataframe.loc[item]
 
+    def __setstate__(self, state):
+        """
+        Used by (cloud)pickle; force the state update to avoid recursion pickling Atoms
+        """
+        self.__dict__.update(state)
+
+    def __getstate__(self):
+        # Only necessary to support pickling in python <3.11
+        # https://docs.python.org/release/3.11.2/library/pickle.html#object.__getstate__
+        return self.__dict__
+
     def from_hdf(self, hdf):
         """
         loads an element with his parameters from the hdf5 job file by creating an Object of the ChemicalElement type.
         The new element will be stored in the current periodic table.
         Changes in the tags will also be modified inside the periodic table.
 
         Args:
             hdf (Hdfio): Hdfio object which will be used to read the data from a hdf5 file
 
         Returns:
 
         """
         elements = hdf.list_groups()  # ["elements"]
         for el in elements:
-            sub = pandas.Series()
+            sub = pandas.Series(dtype=object)
             new_element = ChemicalElement(sub)
             new_element.sub.name = el
             new_element.from_hdf(hdf)
             new_element.sub["Abbreviation"] = el
 
             if "sub_tags" in new_element.tags:
                 if not new_element.tags["sub_tags"]:
@@ -244,15 +271,17 @@
                     raise AssertionError()
                 if len(new_element.sub["tags"]) > 0:
                     raise ValueError("Element cannot get tag-assignment twice")
                 if "tags" not in self.dataframe.keys():
                     self.dataframe["tags"] = None
                 self.dataframe["tags"][el] = new_element.tags
             else:
-                self.dataframe = self.dataframe.append(new_element.sub)
+                self.dataframe = pandas.concat(
+                    [self.dataframe, new_element.sub.to_frame().T]
+                )
                 self.dataframe["tags"] = self.dataframe["tags"].apply(
                     lambda x: None if pandas.isnull(x) else x
                 )
                 self.dataframe["Parent"] = self.dataframe["Parent"].apply(
                     lambda x: None if pandas.isnull(x) else x
                 )
 
@@ -264,33 +293,30 @@
         Args:
             arg (str, ChemicalElement): sort of element
             **qwargs: e.g. a dictionary of tags
 
         Returns element (ChemicalElement): a element with all its properties (Abbreviation, AtomicMass, Weight, ...)
 
         """
-
         stringtypes = str
         if isinstance(arg, stringtypes):
             if arg in self.dataframe.index.values:
                 self.el = arg
             else:
                 raise KeyError(arg)
         elif isinstance(arg, int):
-
             if arg in list(self.dataframe["AtomicNumber"]):
                 index = list(self.dataframe["AtomicNumber"]).index(arg)
                 self.el = self.dataframe.iloc[index].name
         else:
             raise ValueError("type not defined: " + str(type(arg)))
-
-        if qwargs is not None and "tags" not in self.dataframe.columns.values:
-            self.dataframe["tags"] = None
+        if len(qwargs.values()) > 0:
+            if "tags" not in self.dataframe.columns.values:
+                self.dataframe["tags"] = None
             self.dataframe["tags"][self.el] = qwargs
-
         element = self.dataframe.loc[self.el]
         # element['CovalentRadius'] /= 100
         return ChemicalElement(element)
 
     def is_element(self, symbol):
         """
         Compares the Symbol with the Abbreviations of elements inside the periodic table
@@ -342,37 +368,36 @@
 
         pandas.options.mode.chained_assignment = None
         parent_element_data_series = self.dataframe.loc[parent_element]
         parent_element_data_series["Abbreviation"] = new_element
         parent_element_data_series["Parent"] = parent_element
         parent_element_data_series.name = new_element
         if new_element not in self.dataframe.T.columns:
-            self.dataframe = self.dataframe.append(parent_element_data_series)
+            self.dataframe = pandas.concat(
+                [self.dataframe, parent_element_data_series.to_frame().T],
+            )
         else:
             self.dataframe.loc[new_element] = parent_element_data_series
-        if len(qwargs) != 0:
-            if "tags" not in self.dataframe.columns.values:
-                self.dataframe["tags"] = None
-            self.dataframe["tags"][new_element] = qwargs
         if use_parent_potential:
             self._parent_element = parent_element
-        return self.element(new_element)
+        return self.element(new_element, **qwargs)
 
     @staticmethod
+    @lru_cache(maxsize=1)
     def _get_periodic_table_df(file_name):
         """
 
         Args:
             file_name:
 
         Returns:
 
         """
         if not file_name:
-            for resource_path in s.resource_paths:
+            for resource_path in state.settings.resource_paths:
                 if os.path.exists(os.path.join(resource_path, "atomistics")):
                     resource_path = os.path.join(resource_path, "atomistics")
                 for path, folder_lst, file_lst in os.walk(resource_path):
                     for periodic_table_file_name in {"periodic_table.csv"}:
                         if (
                             periodic_table_file_name in file_lst
                             and periodic_table_file_name.endswith(".csv")
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/pyironase.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/pyironase.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,11 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
-import sys
-
-try:
-    from ase.atoms import Atoms as ASEAtoms
-except ImportError:
-    pass
-
 __author__ = "Joerg Neugebauer"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/sparse_list.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/sparse_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 from __future__ import print_function
 
 # import os
 import sys
 import copy
 import numpy as np
-from collections import OrderedDict, Sequence
+from numbers import Integral
+from collections import OrderedDict
+from collections.abc import Sequence
 
 __author__ = "Joerg Neugebauer"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -106,15 +108,15 @@
         elif len(self.values()) > 0:
             print("sparse array: ", key, len(self.values()))
             data_type = self._val_data_type()
             my_dict = OrderedDict()
             my_dict["index"] = self.keys()
             if data_type == "list_bool":
                 my_dict["values"] = [
-                    sum([2 ** i * int(v) for i, v in enumerate(val)])
+                    sum([2**i * int(v) for i, v in enumerate(val)])
                     for val in self.values()
                 ]
             else:
                 my_dict["values"] = self.values()
             print("values: ", self.values())
             hdf[key] = my_dict
 
@@ -167,53 +169,65 @@
             for i, val in self._dict.items():
                 yield SparseListElement(i, val)
         else:
             for i, val in enumerate(self.list()):
                 yield val
 
     def __getitem__(self, item):
-        if isinstance(item, (int, np.integer)):
+        if isinstance(item, Integral):
+            if item > len(self):
+                raise IndexError
+            item = item % len(self)
             if item in self._dict:
                 return self._dict[item]
             return self._default
 
         if isinstance(item, slice):
             ind_list = range(len(self))[item]
         elif isinstance(item, (list, tuple, np.ndarray)):
             if len(item) == 0:
                 ind_list = []
             else:
-                if isinstance(item[0], (int, np.integer)):
+                # for some reason isinstance(True, int) == True, so check for bools first explicitly
+                if isinstance(item[0], (bool, np.bool_)):
+                    if len(item) != len(self):
+                        raise IndexError(
+                            "Length of boolean index does not match indexed list!"
+                        )
+                    ind_list = np.argwhere(item).flatten()
+                elif isinstance(item[0], Integral):
                     ind_list = item
-                elif isinstance(item[0], (bool, np.bool_)):
-                    ind_list = []
-                    for i, bo in enumerate(item):
-                        if bo:
-                            ind_list.append(i)
         else:
             raise ValueError("Unknown item type: " + str(type(item)))
         sliced_dict = {
             j: self._dict[ind] for j, ind in enumerate(ind_list) if ind in self._dict
         }
 
         return self.__class__(sliced_dict, default=self._default, length=len(ind_list))
 
     def __setitem__(self, key, value):
-        if isinstance(key, (int, np.integer)):
+        if isinstance(key, Integral):
             if key > len(self):
                 raise IndexError
+            key = key % len(self)
             self._dict[key] = value
             return
         elif isinstance(key, slice):
             key = range(len(self))[key]
 
         if max(key) > self._length:
             raise IndexError
-        for i in key:
-            self._dict[i] = value
+
+        keys = list(key)
+        if isinstance(keys[0], (bool, np.bool_)):
+            for i in np.argwhere(keys).flatten():
+                self._dict[i] = value
+        else:
+            for i in key:
+                self._dict[i] = value
 
     def __delitem__(self, key):
         # programmed for simplicity, not for performance
         ind_list = list(range(len(self)))
         if isinstance(key, (list, np.ndarray, tuple)):
             indexes = sorted(list(key), reverse=True)
             for index in indexes:
@@ -233,25 +247,26 @@
         new_list = self.__copy__()
         shifted_dict = {i + self._length: val for i, val in other._dict.items()}
         new_list._dict.update(shifted_dict)
         new_list._length += len(other)
         return new_list
 
     def __mul__(self, other):
-        if not isinstance(other, (int, np.integer)):
+        if not isinstance(other, Integral):
             raise ValueError("Multiplication defined only for SparseArray*integers")
-        overall_list = other * np.arange(len(self)).tolist()
-        new_dic = dict()
-        for k in self.keys():
-            for val in np.argwhere(np.array(overall_list) == k).flatten():
-                new_dic[val] = self[k]
-        return self.__class__(new_dic, default=self._default, length=other * len(self))
+        new_dict = {}
+        length = len(self)
+        for rep in range(other):
+            offset = rep * length
+            for k in self.keys():
+                new_dict[k + offset] = self[k]
+        return self.__class__(new_dict, default=self._default, length=other * length)
 
     def __rmul__(self, other):
-        if isinstance(other, int):
+        if isinstance(other, Integral):
             return self * other
 
     def __str__(self):
         if self._default is None:
             return "[" + " ".join([str(el) for el in self]) + "]"
         else:
             # return "[" + " ".join([str(el) + os.sep for el in self.list()]) + "]"
@@ -416,15 +431,15 @@
         if hasattr(self, "_length"):
             return self._length
         else:
             return 0
 
     def __getitem__(self, item):
         new_dict = {}
-        if isinstance(item, int):
+        if isinstance(item, Integral):
             for key, value in self._lists.items():
                 if value[item] is not None:
                     new_dict[key] = value[item]
             return SparseArrayElement(**new_dict)
         elif isinstance(item, str):
             return self._lists[item]
 
@@ -519,55 +534,45 @@
                 else:
                     raise ValueError(
                         "Type not implemented " + str(type(new_array._lists[key]))
                     )
             elif isinstance(val, SparseList):
                 new_array._lists[
                     key
-                ]._length = (
-                    new_length
-                )  # TODO: default extends to all elements (may be undesired)
+                ]._length = new_length  # TODO: default extends to all elements (may be undesired)
             else:
                 print("non-matching key: ", key)
                 raise ValueError(
                     "Incompatible lists (for non-sparse lists keys must be identical (2)"
                 )
         new_array._length += len(other)
         return new_array
 
     def __mul__(self, other):
-        if not isinstance(other, int):
+        if not isinstance(other, Integral):
             raise ValueError(
                 "Multiplication with SparseMatrix only implemented for integers"
             )
         new_array = self.__copy__()
         for key, value in self.items():
             new_array._lists[key] *= other
 
         new_array._length *= other
         return new_array
 
     def __rmul__(self, other):
-        if isinstance(other, int):
+        if isinstance(other, Integral):
             return self * other
 
-    def add_tag(self, *args, **qwargs):
-        for key in args:
-            self._lists[key] = SparseList({}, length=len(self))
-
+    def add_tag(self, **qwargs):
         for key, default in qwargs.items():
             self._lists[key] = SparseList({}, default=default, length=len(self))
 
-    def remove_tag(self, *args, **qwargs):
+    def remove_tag(self, key):
         """
+        Remove tags to the atoms object.
 
         Args:
-            *args:
-            **qwargs:
-
-        Returns:
+            tag (str): tag to remove
 
         """
-        for key in args:
-            del self._lists[key]
-        for key, default in qwargs.items():
-            del self._lists[key]
+        del self._lists[key]
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/volumetric/generic.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/volumetric/generic.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,40 +81,48 @@
 
         Returns:
             float: Gaussian reduction constant
 
         """
         sigma = fwhm / (2 * np.sqrt(2 * np.log(2)))
         d2 = d * d
-        return np.exp(-1 / (2 * sigma ** 2) * d2)
+        return np.exp(-1 / (2 * sigma**2) * d2)
 
     @staticmethod
-    def dist_between_two_grid_points(target_grid_point, n_grid_at_center, lattice, grid_shape):
+    def dist_between_two_grid_points(
+        target_grid_point, n_grid_at_center, lattice, grid_shape
+    ):
         """
         Calculates the distance between a target grid point and another grid point
 
         Args:
             target_grid_point (numpy.ndarray/list): Target grid point
             n_grid_at_center (numpy.ndarray/list): coordinate of center of sphere
             lattice (numpy.ndarray/list): lattice vector
             grid_shape (tuple/list/numpy.ndarray): size of grid
 
         Returns:
 
             float: Distance between target grid and center of sphere in angstrom
 
         """
-        unit_dist_in_grid = [np.sqrt(np.dot(lattice[0], lattice[0])) / grid_shape[0],
-                             np.sqrt(np.dot(lattice[1], lattice[1])) / grid_shape[1],
-                             np.sqrt(np.dot(lattice[2], lattice[2])) / grid_shape[2]]
-        dn = np.multiply(np.subtract(target_grid_point, n_grid_at_center), unit_dist_in_grid)
+        unit_dist_in_grid = [
+            np.sqrt(np.dot(lattice[0], lattice[0])) / grid_shape[0],
+            np.sqrt(np.dot(lattice[1], lattice[1])) / grid_shape[1],
+            np.sqrt(np.dot(lattice[2], lattice[2])) / grid_shape[2],
+        ]
+        dn = np.multiply(
+            np.subtract(target_grid_point, n_grid_at_center), unit_dist_in_grid
+        )
         dist = np.linalg.norm(dn)
         return dist
 
-    def spherical_average_potential(self, structure, spherical_center, rad=2, fwhm=0.529177):
+    def spherical_average_potential(
+        self, structure, spherical_center, rad=2, fwhm=0.529177
+    ):
         """
         Calculates the spherical average about a given point in space
 
         Args:
             structure (pyiron_atomistics.atomistics.structure.Atoms): Input structure
             spherical_center (list/numpy.ndarray): position of spherical_center in direct coordinate
             rad (float): radius of sphere to be considered in Angstrom (recommended value: 2)
@@ -123,80 +131,96 @@
         Returns:
             float: Spherical average at the target center
 
         """
         grid_shape = self._total_data.shape
 
         # Position of center of sphere at grid coordinates
-        n_grid_at_center = [int(np.ceil(spherical_center[0] * grid_shape[0])),
-                            int(np.ceil(spherical_center[1] * grid_shape[1])),
-                            int(np.ceil(spherical_center[2] * grid_shape[2]))]
+        n_grid_at_center = [
+            int(np.ceil(spherical_center[0] * grid_shape[0])),
+            int(np.ceil(spherical_center[1] * grid_shape[1])),
+            int(np.ceil(spherical_center[2] * grid_shape[2])),
+        ]
 
         # Unit distance between grids
-        dist_in_grid = [np.linalg.norm(structure.cell[0]) / grid_shape[0],
-                        np.linalg.norm(structure.cell[1]) / grid_shape[1],
-                        np.linalg.norm(structure.cell[2]) / grid_shape[2]]
+        dist_in_grid = [
+            np.linalg.norm(structure.cell[0]) / grid_shape[0],
+            np.linalg.norm(structure.cell[1]) / grid_shape[1],
+            np.linalg.norm(structure.cell[2]) / grid_shape[2],
+        ]
 
         # Range of grids to be considered within the provided radius w.r.t. center of sphere
         num_grid_in_sph = [[], []]
         for i, dist in enumerate(dist_in_grid):
             num_grid_in_sph[0].append(n_grid_at_center[i] - int(np.ceil(rad / dist)))
             num_grid_in_sph[1].append(n_grid_at_center[i] + int(np.ceil(rad / dist)))
 
         sph_avg_tmp = []
         weight = 0
         for k in range(num_grid_in_sph[0][0], num_grid_in_sph[1][0]):
             for l in range(num_grid_in_sph[0][1], num_grid_in_sph[1][1]):
                 for m in range(num_grid_in_sph[0][2], num_grid_in_sph[1][2]):
                     target_grid_point = [k, l, m]
-                    dist = self.dist_between_two_grid_points(target_grid_point,
-                                                             n_grid_at_center, structure.cell, grid_shape)
+                    dist = self.dist_between_two_grid_points(
+                        target_grid_point, n_grid_at_center, structure.cell, grid_shape
+                    )
                     if dist <= rad:
                         sph_avg_tmp.append(
-                            self._total_data[k % grid_shape[0], l % grid_shape[1], m % grid_shape[2]]
-                            * self.gauss_f(dist, fwhm))
+                            self._total_data[
+                                k % grid_shape[0], l % grid_shape[1], m % grid_shape[2]
+                            ]
+                            * self.gauss_f(dist, fwhm)
+                        )
                         weight += self.gauss_f(dist, fwhm)
                     else:
                         pass
         sum_list = np.sum(sph_avg_tmp)
         sph_avg = sum_list / weight
         return sph_avg
 
     @staticmethod
-    def dist_between_two_grid_points_cyl(target_grid_point, n_grid_at_center, lattice, grid_shape, direction_of_cyl):
+    def dist_between_two_grid_points_cyl(
+        target_grid_point, n_grid_at_center, lattice, grid_shape, direction_of_cyl
+    ):
         """
         Distance between a target grid point and the center of a cylinder
 
         Args:
             target_grid_point (numpy.ndarray/list): Target grid point
             n_grid_at_center (numpy.ndarray/list): coordinate of center of sphere
             lattice (numpy.ndarray/list): lattice vector
             grid_shape (tuple/list/numpy.ndarray): size of grid
             direction_of_cyl (int): Axis of cylinder (0 (x) or 1 (y) or 2 (z))
 
         Returns:
             float: Distance between target grid and in-plane center of cylinder
 
         """
-        unit_dist_in_grid = [np.sqrt(np.dot(lattice[0], lattice[0])) / grid_shape[0],
-                             np.sqrt(np.dot(lattice[1], lattice[1])) / grid_shape[1],
-                             np.sqrt(np.dot(lattice[2], lattice[2])) / grid_shape[2]]
-        dn = np.multiply(np.subtract(target_grid_point, n_grid_at_center), unit_dist_in_grid)
+        unit_dist_in_grid = [
+            np.sqrt(np.dot(lattice[0], lattice[0])) / grid_shape[0],
+            np.sqrt(np.dot(lattice[1], lattice[1])) / grid_shape[1],
+            np.sqrt(np.dot(lattice[2], lattice[2])) / grid_shape[2],
+        ]
+        dn = np.multiply(
+            np.subtract(target_grid_point, n_grid_at_center), unit_dist_in_grid
+        )
         if direction_of_cyl == 0:
             dn[0] = 0
         elif direction_of_cyl == 1:
             dn[1] = 0
         elif direction_of_cyl == 2:
             dn[2] = 0
         else:
             print("check the direction of cylindrical axis")
         dist = np.linalg.norm(dn)
         return dist
 
-    def cylindrical_average_potential(self, structure, spherical_center, axis_of_cyl, rad=2, fwhm=0.529177):
+    def cylindrical_average_potential(
+        self, structure, spherical_center, axis_of_cyl, rad=2, fwhm=0.529177
+    ):
         """
         Calculates the cylindrical average about a given point in space
 
         Args:
             structure (pyiron_atomistics.atomistics.structure.Atoms): Input structure
             spherical_center (list/numpy.ndarray): position of spherical_center in direct coordinate
             rad (float): radius of sphere to be considered in Angstrom (recommended value: 2)
@@ -206,46 +230,62 @@
         Returns:
             float: Cylindrical average at the target center
 
         """
         grid_shape = self._total_data.shape
 
         # Position of center of sphere at grid coordinates
-        n_grid_at_center = [int(np.ceil(spherical_center[0] * grid_shape[0])),
-                            int(np.ceil(spherical_center[1] * grid_shape[1])),
-                            int(np.ceil(spherical_center[2] * grid_shape[2]))]
+        n_grid_at_center = [
+            int(np.ceil(spherical_center[0] * grid_shape[0])),
+            int(np.ceil(spherical_center[1] * grid_shape[1])),
+            int(np.ceil(spherical_center[2] * grid_shape[2])),
+        ]
 
         # Unit distance between grids
-        dist_in_grid = [np.linalg.norm(structure.cell[0]) / grid_shape[0],
-                        np.linalg.norm(structure.cell[1]) / grid_shape[1],
-                        np.linalg.norm(structure.cell[2]) / grid_shape[2]]
+        dist_in_grid = [
+            np.linalg.norm(structure.cell[0]) / grid_shape[0],
+            np.linalg.norm(structure.cell[1]) / grid_shape[1],
+            np.linalg.norm(structure.cell[2]) / grid_shape[2],
+        ]
 
         # Range of grids to be considered within the provided radius w.r.t. center of sphere
         num_grid_in_cyl = [[], []]
 
         for i, dist in enumerate(dist_in_grid):
             if i == axis_of_cyl:
                 num_grid_in_cyl[0].append(0)
                 num_grid_in_cyl[1].append(grid_shape[i])
             else:
-                num_grid_in_cyl[0].append(n_grid_at_center[i] - int(np.ceil(rad / dist)))
-                num_grid_in_cyl[1].append(n_grid_at_center[i] + int(np.ceil(rad / dist)))
+                num_grid_in_cyl[0].append(
+                    n_grid_at_center[i] - int(np.ceil(rad / dist))
+                )
+                num_grid_in_cyl[1].append(
+                    n_grid_at_center[i] + int(np.ceil(rad / dist))
+                )
 
         cyl_avg_tmp = []
         weight = 0
         for k in range(num_grid_in_cyl[0][0], num_grid_in_cyl[1][0]):
             for l in range(num_grid_in_cyl[0][1], num_grid_in_cyl[1][1]):
                 for m in range(num_grid_in_cyl[0][2], num_grid_in_cyl[1][2]):
                     target_grid_point = [k, l, m]
-                    dist = self.dist_between_two_grid_points_cyl(target_grid_point, n_grid_at_center, structure.cell,
-                                                                 grid_shape, axis_of_cyl)
+                    dist = self.dist_between_two_grid_points_cyl(
+                        target_grid_point,
+                        n_grid_at_center,
+                        structure.cell,
+                        grid_shape,
+                        axis_of_cyl,
+                    )
                     if dist <= rad:
                         cyl_avg_tmp.append(
-                            self._total_data[k % grid_shape[0], l % grid_shape[1], m % grid_shape[2]]
-                            * self.gauss_f(dist, fwhm))
+                            self._total_data[
+                                k % grid_shape[0], l % grid_shape[1], m % grid_shape[2]
+                            ]
+                            * self.gauss_f(dist, fwhm)
+                        )
                         weight += self.gauss_f(dist, fwhm)
                     else:
                         pass
         sum_list = np.sum(cyl_avg_tmp)
         cyl_avg = sum_list / weight
 
         return cyl_avg
@@ -349,22 +389,25 @@
             lines = f.readlines()
             n_atoms = int(lines[2].strip().split()[0])
             cell_data = np.genfromtxt(lines[3:6])
             cell_grid = cell_data[:, 1:]
             grid_shape = np.array(cell_data[:, 0], dtype=int)
             # total_data = np.zeros(grid_shape)
             cell = np.array([val * grid_shape[i] for i, val in enumerate(cell_grid)])
-            pos_data = np.genfromtxt(lines[6: n_atoms + 6])
-            if n_atoms == 1:
-                pos_data = np.array([pos_data])
-            atomic_numbers = np.array(pos_data[:, 0], dtype=int)
-            positions = pos_data[:, 2:]
-            self._atoms = Atoms(numbers=atomic_numbers, positions=positions, cell=cell)
+            if n_atoms > 0:
+                pos_data = np.genfromtxt(lines[6 : n_atoms + 6])
+                if n_atoms == 1:
+                    pos_data = np.array([pos_data])
+                atomic_numbers = np.array(pos_data[:, 0], dtype=int)
+                positions = pos_data[:, 2:]
+                self._atoms = Atoms(
+                    numbers=atomic_numbers, positions=positions, cell=cell
+                )
             end_int = n_atoms + 6 + int(np.prod(grid_shape) / 6)
-            data = np.genfromtxt(lines[n_atoms+6: end_int])
+            data = np.genfromtxt(lines[n_atoms + 6 : end_int])
             data_flatten = np.hstack(data)
             if np.prod(grid_shape) % 6 > 0:
                 data_flatten = np.append(
                     data_flatten, [float(val) for val in lines[end_int].split()]
                 )
             n_x, n_y, n_z = grid_shape
             self._total_data = data_flatten.reshape((n_x, n_y, n_z))
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/dft/job/generic.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/dft/job/generic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
-from pyiron_atomistics.atomistics.job.atomistic import AtomisticGenericJob, MapFunctions as AtomisticMapFunctions
+from pyiron_atomistics.atomistics.job.atomistic import (
+    AtomisticGenericJob,
+    MapFunctions as AtomisticMapFunctions,
+)
 from pyiron_atomistics.dft.waves.electronic import ElectronicStructure
 import warnings
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
@@ -146,29 +149,19 @@
 
     @fix_symmetry.setter
     def fix_symmetry(self, boolean):
         if not isinstance(boolean, bool):
             raise AssertionError()
         self._generic_input["fix_symmetry"] = boolean
 
-    def get_structure(self, iteration_step=-1, wrap_atoms=True):
-        """
-        Gets the structure from a given iteration step of the simulation (MD/ionic relaxation). For static calculations
-        there is only one ionic iteration step
-        Args:
-            iteration_step (int): Step for which the structure is requested
-            wrap_atoms (bool): True if the atoms are to be wrapped back into the unit cell
-
-        Returns:
-            pyiron.atomistics.structure.atoms.Atoms: The required structure
-        """
-        snapshot = super(GenericDFTJob, self).get_structure(
-            iteration_step=iteration_step, wrap_atoms=wrap_atoms
+    def _get_structure(self, frame=-1, wrap_atoms=True):
+        snapshot = super(GenericDFTJob, self)._get_structure(
+            frame=frame, wrap_atoms=wrap_atoms
         )
-        spins = self.get_magnetic_moments(iteration_step=iteration_step)
+        spins = self.get_magnetic_moments(iteration_step=frame)
         if spins is not None:
             snapshot.set_initial_magnetic_moments(spins)
         return snapshot
 
     def set_mixing_parameters(
         self,
         method=None,
@@ -239,14 +232,19 @@
             return None
 
     def get_kpoints(self):
         raise NotImplementedError(
             "The get_kpoints() function is not implemented for this code."
         )
 
+    def get_valence_and_total_charge_density(self):
+        raise NotImplementedError(
+            "The get_valence_and_total_charge_density() function is not implemented for this code."
+        )
+
     def get_k_mesh_by_cell(self, k_mesh_spacing, cell=None):
         """
         Get k-mesh density according to the box size.
 
         Args:
             k_mesh_spacing (float): K-point spacing in units of 2 * pi reciprocal Angstrom.
                                 (smaller values result in a denser mesh for a given structure).
@@ -254,15 +252,17 @@
 
         Returns:
             list/numpy.ndarray: Mesh size
 
         """
         if cell is None:
             if self.structure is None:
-                raise ValueError("Can't generate k-points without structure being set and if cell is not specified")
+                raise ValueError(
+                    "Can't generate k-points without structure being set and if cell is not specified"
+                )
             cell = self.structure.cell
         return get_k_mesh_by_density(cell=cell, k_mesh_spacing=k_mesh_spacing)
 
     def set_kpoints(
         self,
         mesh=None,
         scheme="MP",
@@ -368,16 +368,18 @@
         """
         Function to check if there are a sufficient number of empty bands in the calculation to ensure electronic convergence.
 
         Returns:
 
             bool : True if the highest band is unoccupied, False if the highest band is occupied
         """
-        return np.all(np.isclose(self["output/electronic_structure/occ_matrix"][:,:,-1], 0)) #shape is n_spin x n_kpoints x n_bands
-    
+        return np.all(
+            np.isclose(self["output/electronic_structure/occ_matrix"][:, :, -1], 0)
+        )  # shape is n_spin x n_kpoints x n_bands
+
     # Backward compatibility
     def get_encut(self):
         return self.encut
 
     def set_encut(self, encut):
         """
         Sets the plane-wave energy cutoff
@@ -390,14 +392,34 @@
         self.exchange_correlation_functional = exchange_correlation_functional
 
     def set_empty_states(self, n_empty_states=None):
         raise NotImplementedError(
             "The set_empty_states function is not implemented for this code."
         )
 
+    def get_bader_charges(self):
+        """
+        Returns the total charge on every atom determined by the Bader charge partitioning scheme.
+
+        Returns:
+            numpy.ndarray: The Bader charges for each atom
+
+        """
+        return self["output/generic/dft/bader_charges"]
+
+    def get_bader_volumes(self):
+        """
+        Returns the integration volume around every atom from the Bader charge partitioning scheme.
+
+        Returns:
+            numpy.ndarray: The Bader charges for each atom
+
+        """
+        return self["output/generic/dft/bader_volumes"]
+
     def _set_kpoints(
         self,
         mesh=None,
         scheme="MP",
         center_shift=None,
         symmetry_reduction=True,
         manual_kpoints=None,
@@ -423,17 +445,19 @@
             with self.project_hdf5.open("output") as ho:
                 es_obj = ElectronicStructure()
                 es_obj.from_hdf(ho)
             return es_obj
 
     def modify_kpoints(self):
         if self.k_mesh_spacing is not None:
-            self.set_kpoints(center_shift=self.k_mesh_center_shift,
-                             k_mesh_spacing=self.k_mesh_spacing,
-                             symmetry_reduction=self.reduce_kpoint_symmetry)
+            self.set_kpoints(
+                center_shift=self.k_mesh_center_shift,
+                k_mesh_spacing=self.k_mesh_spacing,
+                symmetry_reduction=self.reduce_kpoint_symmetry,
+            )
 
     def save(self):
         self.modify_kpoints()
         super(GenericDFTJob, self).save()
 
     def get_density_of_states(self, sigma=0.1, shift_by_fermi_energy=True, grid=None):
         """
@@ -448,30 +472,38 @@
             grid (list/numpy.ndarray): Energy grid. If None, the interval between maximum and
                 minimum eigenvalues plus 5 x sigma with a step length of sigma will be taken.
 
         Returns:
             (dict): grid and density of states (n_spin x energy_grid)
         """
         if sigma <= 0:
-            raise ValueError('Sigma must be a positive float')
-        k_weights = self['output/electronic_structure/k_weights']
+            raise ValueError("Sigma must be a positive float")
+        k_weights = self["output/electronic_structure/k_weights"]
         if k_weights is None:
-            raise ValueError('k-point weighting not found')
+            raise ValueError("k-point weighting not found")
         e_fermi = 0
         if shift_by_fermi_energy:
-            e_fermi = self['output/electronic_structure/efermi']
-        eigen_values = self['output/electronic_structure/eig_matrix']
-        eigen_values = eigen_values-e_fermi
+            e_fermi = self["output/electronic_structure/efermi"]
+        eigen_values = self["output/electronic_structure/eig_matrix"]
+        eigen_values = eigen_values - e_fermi
         if grid is None:
-            grid = np.arange(eigen_values.min()-5*sigma, eigen_values.max()+5*sigma, sigma)
-        hist = eigen_values[:,:,:,np.newaxis]-grid[np.newaxis,np.newaxis,np.newaxis,:]
-        hist = np.exp(-(hist)**2/(2*sigma**2))*k_weights[np.newaxis,:,np.newaxis,np.newaxis]
-        hist = np.sum(hist, axis=(1,2))
-        hist *= 2/len(eigen_values)/np.sqrt(2*np.pi*sigma**2)
-        return {'grid': grid, 'dos': hist}
+            grid = np.arange(
+                eigen_values.min() - 5 * sigma, eigen_values.max() + 5 * sigma, sigma
+            )
+        hist = (
+            eigen_values[:, :, :, np.newaxis]
+            - grid[np.newaxis, np.newaxis, np.newaxis, :]
+        )
+        hist = (
+            np.exp(-((hist) ** 2) / (2 * sigma**2))
+            * k_weights[np.newaxis, :, np.newaxis, np.newaxis]
+        )
+        hist = np.sum(hist, axis=(1, 2))
+        hist *= 2 / len(eigen_values) / np.sqrt(2 * np.pi * sigma**2)
+        return {"grid": grid, "dos": hist}
 
 
 def get_k_mesh_by_density(cell, k_mesh_spacing=0.5):
     """
     Get k-mesh density according to the box size.
 
     Args:
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/convergence_encut_parallel.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/sqsmaster.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,99 +1,91 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
-from __future__ import print_function
+import numpy as np
 from pyiron_atomistics.atomistics.master.parallel import AtomisticParallelMaster
 from pyiron_base import JobGenerator
-import numpy as np
-
-try:
-    import pylab as plt
-except (ImportError, RuntimeError):
-    try:
-        import matplotlib.pyplot as plt
-    except (ImportError, RuntimeError):
-        pass
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
-__version__ = "1.0"
+__version__ = "0.0.1"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "development"
-__date__ = "Sep 1, 2017"
+__date__ = "Oct 29, 2020"
+
+
+class SQSMaster(AtomisticParallelMaster):
+    """
+    Master job to compute SQS structures for a list of concentrations.
+
+    The input keys "species_one", "species_two" and "fraction_lst" are combined into dictionaries that are then passed
+    to the input "mole_fractions" as defined on :class:`.SQSJob` according to the pseudo code
+
+    >>> for f in fraction_lst:
+    ...     {species_one: f, species_two: 1-f}
+
+    The other options to :class:`.SQSJob` must be set on the reference job.
+    """
 
+    def __init__(self, project, job_name):
+        super(SQSMaster, self).__init__(project, job_name)
+
+        self.__version__ = "0.0.1"
+        self.input["fraction_lst"] = []
+        self.input["species_one"] = ""
+        self.input["species_two"] = ""
+        self._job_generator = SQSJobGenerator(self)
+
+    def collect_output(self):
+        pass
 
-class EncutConvergenceJobGenerator(JobGenerator):
     @property
-    def parameter_list(self):
+    def list_of_structures(self):
         """
-
-        Returns:
-            (list)
+        list: `len(self.input["fraction_lst"])` with the top-scoring structure from each sub job
         """
         return [
-            np.round(encut, 7)
-            for encut in np.linspace(
-                self._master.input["min"],
-                self._master.input["max"],
-                self._master.input["num_points"],
-            )
+            self.project_hdf5.load(job_id).list_of_structures[0]
+            for job_id in self.child_ids
         ]
 
-    @staticmethod
-    def job_name(parameter):
-        return "encut_" + str(parameter).replace(".", "_")
+    def list_structures(self):
+        """
+        List of top-scoring structures from each sub job.
 
-    @staticmethod
-    def modify_job(job, parameter):
-        job.set_encut(encut=parameter)
-        return job
+        Returns:
+            list: value of :attribute:`.list_of_structures`
+        """
+        return self.list_of_structures
 
 
-# ToDo: not all abstract methods implemented
-class ConvEncutParallel(AtomisticParallelMaster):
-    def __init__(self, project, job_name="encut_conv"):
+class SQSJobGenerator(JobGenerator):
+    @property
+    def parameter_list(self):
         """
 
-        Args:
-            project:
-            job_name:
+        Returns:
+            (list)
         """
-        super(ConvEncutParallel, self).__init__(project, job_name)
-        self.__name__ = "ConvEncutParallel"
-        self.__version__ = "0.0.1"
+        return [
+            [
+                "sqs_" + str(np.round(f, 4)).replace(".", "_"),
+                {
+                    self._master.input["species_one"]: f,
+                    self._master.input["species_two"]: 1 - f,
+                },
+            ]
+            for f in self._master.input["fraction_lst"]
+        ]
 
-        # define default input
-        self.input["num_points"] = (11, "number of sample points")
-        self.input["min"] = (200, "EnCut Minimum")
-        self.input["max"] = (800, "EnCut Maximum")
-        self._job_generator = EncutConvergenceJobGenerator(self)
+    @staticmethod
+    def job_name(parameter):
+        return parameter[0]
 
-    def collect_output(self):
-        eng_lst, encut_lst = [], []
-        for job_id in self.child_ids:  # add iter_jobs (should behave like a project)
-            ham = self.project_hdf5.inspect(job_id)
-            print("job_id: ", job_id, ham.status)
-            eng_lst.append(ham["output/generic/energy_tot"][-1])
-            encut = ham.job_name.split("_")[1:]
-            encut_lst.append(float(encut[0] + "." + encut[1]))
-        arg_lst = np.argsort(encut_lst)
-        self._output["energy"] = eng_lst[arg_lst]
-        self._output["encut"] = encut_lst[arg_lst]
-
-        with self.project_hdf5.open("output") as hdf5_out:
-            for key, val in self._output.items():
-                hdf5_out[key] = val
-
-    def plot(self, plt_show=True):
-        df = self.output_to_pandas()
-        encut_lst, eng_lst = df["encut"], df["energy"]
-        plt.plot(encut_lst, eng_lst, "x-", markersize=20)
-        plt.xlabel("EnCut (eV)")
-        plt.ylabel("energy (eV)")
-        if plt_show:
-            plt.show()
+    def modify_job(self, job, parameter):
+        job.input["mole_fractions"] = parameter[1]
+        return job
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/convergence_encut_serial.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/convergence_encut_serial.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     Args:
         project:
         job_name:
     """
 
     def __init__(self, project, job_name):
         super(ConvEncutSerial, self).__init__(project, job_name=job_name)
-        self.__name__ = "ConvEncutSerial"
+
         self.__version__ = "0.0.2"
         if (
             not self["input/convergence_goal"]
             or self["input/convergence_goal"] == "None"
         ):
             self.set_goal(convergence_goal, eps=0.005)
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         """
 
         Args:
             project:
             job_name:
         """
         super(ConvKpointParallel, self).__init__(project, job_name)
-        self.__name__ = "ConvKpointParallel"
+
         self.__version__ = "0.0.1"
 
         # define default input
         self.input["steps"] = (2, "increase of kpoints")
         self.input["min"] = (4, "Kpoint Minimum")
         self.input["max"] = (8, "Kpoint Maximum")
         self._job_generator = KpointConvergenceJobGenerator(self)
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/murnaghan_dft.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/murnaghan_dft.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from __future__ import print_function
 from pyiron_atomistics.atomistics.master.murnaghan import Murnaghan, DebyeModel
+from pyiron_base import deprecate
 
 __author__ = "Joerg Neugebauer, Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 
 class MurnaghanDFT(Murnaghan):
+    @deprecate("use standard Murnaghan instead")
     def __init__(self, project, job_name="murnaghan"):
         super(MurnaghanDFT, self).__init__(project, job_name)
-        self.__name__ = "MurnaghanDFT"
+
         self.__version__ = "0.3.0"
 
     def set_kpoints(
         self,
         mesh=None,
         scheme="MP",
         center_shift=None,
@@ -50,24 +52,18 @@
 
     def get_encut(self):
         if self.ref_job:
             return self._ref_job.get_encut()
         else:
             return None
 
-    def get_structure(self, iteration_step=-1):
-        """
-
-        Returns: Structure with equilibrium volume
-
-        """
-        if not (iteration_step == -1):
-            raise AssertionError()
-        if not (self.structure is not None):
-            raise AssertionError()
+    def _get_structure(self, frame=-1, wrap_atoms=True):
+        # base class makes sure we only get called when self.structure is set already
         snapshot = self.structure.copy()
         old_vol = snapshot.get_volume()
         new_vol = self["output/equilibrium_volume"]
         k = (new_vol / old_vol) ** (1.0 / 3.0)
         new_cell = snapshot.cell * k
         snapshot.set_cell(new_cell, scale_atoms=True)
+        if wrap_atoms:
+            snapshot.center_coordinates_in_unit_cell()
         return snapshot
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/dft/waves/bandstructure.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/dft/waves/bandstructure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/dft/waves/dos.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/dft/waves/dos.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,20 +44,21 @@
         for eig_val in eig_vals:
             dos_min = np.min(eig_val)
             dos_max = np.max(eig_val)
             if bin_density is not None:
                 n_bins = int((dos_max - dos_min) * bin_density)
             else:
                 n_bins = self.n_bins
-            t_dos, energies = np.histogram(
-                eig_val, bins=int(n_bins), density=True
-            )
+            t_dos, energies = np.histogram(eig_val, bins=int(n_bins), density=True)
             self.t_dos.append(t_dos)
             self.energies.append(energies)
-        self.energies = [energies[1:] - ((energies[1] - energies[0]) / 2.0) for energies in self.energies]
+        self.energies = [
+            energies[1:] - ((energies[1] - energies[0]) / 2.0)
+            for energies in self.energies
+        ]
 
     def plot_total_dos(self, **kwargs):
         """
         Plots the total DOS
 
         Args:
             **kwargs: Variables for matplotlib.pylab.plot customization (linewidth, linestyle, etc.)
@@ -70,15 +71,17 @@
         except ImportError:
             import matplotlib.pyplot as plt
         fig = plt.figure(1, figsize=(6, 4))
         ax1 = fig.add_subplot(111)
         ax1.set_xlabel("E (eV)", fontsize=14)
         ax1.set_ylabel("DOS", fontsize=14)
         for i, energies in enumerate(self.energies):
-            plt.fill_between(energies, self.t_dos[i], label="spin {}".format(i), **kwargs)
+            plt.fill_between(
+                energies, self.t_dos[i], label="spin {}".format(i), **kwargs
+            )
         plt.legend()
         return plt
 
     def plot_orbital_resolved_dos(self, **kwargs):
         """
         Plots the orbital resolved DOS
 
@@ -97,15 +100,17 @@
                 "Can not plot the orbital resolved dos since resolved dos values are not"
                 " available"
             )
         plot = self.plot_total_dos()
         for spin in range(len(self.energies)):
             for key, val in self.orbital_dict.items():
                 r_dos = self.get_orbital_resolved_dos(val)
-                plt.plot(self.energies, r_dos, label=key + "spin {}".format(spin), **kwargs)
+                plt.plot(
+                    self.energies, r_dos, label=key + "spin {}".format(spin), **kwargs
+                )
         plot.legend()
         return plot
 
     def get_spin_resolved_dos(self, spin_indices):
         """
         Gives the dos contribution of a given indices of spin as arranged in the
         pyiron_atomistics.objects.waves.ElectronicStructure instance.
@@ -135,15 +140,17 @@
             weight = np.sum(tot_val[spin_indices, k, b, :, :])
             weight_sum = np.sum(tot_val[:, k, b, :, :])
             if b < n_bands - 1:
                 b += 1
             else:
                 b = 0
                 k += 1
-            index = len(self.energies[spin_indices][self.energies[spin_indices] < e]) - 1
+            index = (
+                len(self.energies[spin_indices][self.energies[spin_indices] < e]) - 1
+            )
             if index >= 0:
                 r_dos[index] = r_dos[index] + weight
                 w_dos[index] = w_dos[index] + weight_sum
             else:
                 r_dos[0] = r_dos[0] + weight
                 w_dos[0] = w_dos[0] + weight_sum
         ind_0 = np.argwhere(w_dos < 1e-8).flatten()
@@ -182,15 +189,17 @@
             weight = np.sum(tot_val[spin_indices, k, b, atom_indices, :])
             weight_sum = np.sum(tot_val[spin_indices, k, b, :, :])
             if b < n_bands - 1:
                 b += 1
             else:
                 b = 0
                 k += 1
-            index = len(self.energies[spin_indices][self.energies[spin_indices] < e]) - 1
+            index = (
+                len(self.energies[spin_indices][self.energies[spin_indices] < e]) - 1
+            )
             if index >= 0:
                 r_dos[index] = r_dos[index] + weight
                 w_dos[index] = w_dos[index] + weight_sum
             else:
                 r_dos[0] = r_dos[0] + weight
                 w_dos[0] = w_dos[0] + weight_sum
         ind_0 = np.argwhere(w_dos < 1e-8).flatten()
@@ -229,15 +238,17 @@
             weight = np.sum(tot_val[spin_indices, k, b, :, orbital_indices])
             weight_sum = np.sum(tot_val[spin_indices, k, b, :, :])
             if b < n_bands - 1:
                 b += 1
             else:
                 b = 0
                 k += 1
-            index = len(self.energies[spin_indices][self.energies[spin_indices] < e]) - 1
+            index = (
+                len(self.energies[spin_indices][self.energies[spin_indices] < e]) - 1
+            )
             if index >= 0:
                 r_dos[index] = r_dos[index] + weight
                 w_dos[index] = w_dos[index] + weight_sum
             else:
                 r_dos[0] = r_dos[0] + weight
                 w_dos[0] = w_dos[0] + weight_sum
         ind_0 = np.argwhere(w_dos < 1e-8).flatten()
@@ -284,15 +295,17 @@
             )
             weight_sum = np.sum(tot_val[spin_indices, k, b, :, :])
             if b < n_bands - 1:
                 b += 1
             else:
                 b = 0
                 k += 1
-            index = len(self.energies[spin_indices][self.energies[spin_indices] < e]) - 1
+            index = (
+                len(self.energies[spin_indices][self.energies[spin_indices] < e]) - 1
+            )
             if index >= 0:
                 r_dos[index] = r_dos[index] + weight
                 w_dos[index] = w_dos[index] + weight_sum
             else:
                 r_dos[0] = r_dos[0] + weight
                 w_dos[0] = w_dos[0] + weight_sum
         ind_0 = np.argwhere(w_dos < 1e-8).flatten()
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/dft/waves/electronic.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/dft/waves/electronic.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         self._grand_dos_matrix = None
         self._resolved_densities = None
         self._kpoint_list = list()
         self._kpoint_weights = list()
         self.n_spins = 1
         self._structure = None
         self._orbital_dict = None
+        self._output_dict = {}
 
     def add_kpoint(self, value, weight):
         """
         Appends a Kpoint() instance to the kpoints attribute
 
         Args:
             value (list/numpy.ndarray): Value of the k-point in cartesian reciprocal coordinates
@@ -465,14 +466,17 @@
     @grand_dos_matrix.setter
     def grand_dos_matrix(self, val):
         """
         Setter for grand_dos_matrix
         """
         self._grand_dos_matrix = val
 
+    def __getitem__(self, item):
+        return self._output_dict[item]
+
     def to_hdf(self, hdf, group_name="electronic_structure"):
         """
         Store the object to hdf5 file
 
         Args:
             hdf: Path to the hdf5 file/group in the file
             group_name: Name of the group under which the attributes are o be stored
@@ -529,14 +533,15 @@
                     self.dos_energies = h_dos["energies"]
                     self.dos_densities = h_dos["tot_densities"]
                     self.dos_idensities = h_dos["int_densities"]
                     if "grand_dos_matrix" in nodes:
                         self.grand_dos_matrix = h_dos["grand_dos_matrix"]
                     if "resolved_densities" in nodes:
                         self.resolved_densities = h_dos["resolved_densities"]
+                self._output_dict = h_es.copy()
             self.generate_from_matrices()
 
     def to_hdf_old(self, hdf, group_name="electronic_structure"):
         """
         Store the object to hdf5 file
 
         Args:
@@ -585,14 +590,15 @@
                 pass
             if "fermi_level" in nodes:
                 self.efermi = h_es["fermi_level"]
             if "grand_dos_matrix" in nodes:
                 self.grand_dos_matrix = h_es["grand_dos_matrix"]
             if "resolved_densities" in nodes:
                 self.resolved_densities = h_es["resolved_densities"]
+            self._output_dict = h_es.copy()
         self.generate_from_matrices()
 
     def generate_from_matrices(self):
         """
         Generate the Kpoints and Bands from the kpoint lists and sometimes grand_dos_matrix
 
         """
@@ -668,15 +674,21 @@
         """
         try:
             import matplotlib.pylab as plt
         except ModuleNotFoundError:
             import matplotlib.pyplot as plt
         for spin, eigenvalues in enumerate(self.eigenvalues):
             arg = np.argsort(eigenvalues)
-            plt.plot(eigenvalues[arg], self.occupancies[spin][arg], "-o", label="spin:{}".format(spin), linewidth=2)
+            plt.plot(
+                eigenvalues[arg],
+                self.occupancies[spin][arg],
+                "-o",
+                label="spin:{}".format(spin),
+                linewidth=2,
+            )
         plt.legend()
         plt.axvline(self.efermi, linewidth=2.0, linestyle="dashed", color="black")
         plt.xlabel("Eigen value (eV)")
         plt.ylabel("Occupancy")
         return plt
 
     def __del__(self):
@@ -694,25 +706,33 @@
         del self._kpoint_weights
         del self.n_spins
 
     def __str__(self):
         output_string = list()
         output_string.append("ElectronicStructure Instance")
         output_string.append("----------------------------")
-        output_string.append("Number of spin channels: {}".format(len(self.eigenvalue_matrix)))
+        output_string.append(
+            "Number of spin channels: {}".format(len(self.eigenvalue_matrix))
+        )
         output_string.append("Number of k-points: {}".format(len(self.kpoints)))
-        output_string.append("Number of bands: {}".format(len(self.kpoints[0].bands[0])))
+        output_string.append(
+            "Number of bands: {}".format(len(self.kpoints[0].bands[0]))
+        )
         try:
             for spin, is_metal in enumerate(self.is_metal):
                 if is_metal:
-                    output_string.append("spin {}:".format(spin) + " Is a metal: {}".format(is_metal))
+                    output_string.append(
+                        "spin {}:".format(spin) + " Is a metal: {}".format(is_metal)
+                    )
                 else:
-                    output_string.append("spin {}:".format(spin) + " Is a metal: "
-                                                                   "{}".format(is_metal) + " Band gap (ev) "
-                                                                                           "{}".format(self.eg[spin]))
+                    output_string.append(
+                        "spin {}:".format(spin) + " Is a metal: "
+                        "{}".format(is_metal) + " Band gap (ev) "
+                        "{}".format(self.eg[spin])
+                    )
         except ValueError:
             pass
         return "\n".join(output_string)
 
     def __repr__(self):
         return self.__str__()
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/gpaw/gpaw.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/gpaw/gpaw.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from pyiron_atomistics.gpaw.pyiron_ase import AseJob
 from pyiron_atomistics.dft.job.generic import GenericDFTJob
-from pyiron_base import GenericParameters, Settings, ImportAlarm
+from pyiron_base import GenericParameters, ImportAlarm
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "development"
 __date__ = "Sep 1, 2018"
 
-s = Settings()
-
-try:
+with ImportAlarm(
+    "Gpaw relies on the gpaw module but this is unavailable. Please ensure your python environment contains gpaw, "
+    "e.g. by running `conda install -c conda-forge gpaw`."
+) as import_alarm:
     from gpaw import GPAW as GPAWcode, PW, MethfesselPaxton
-    import_alarm = ImportAlarm()
-except ImportError:
-    import_alarm = ImportAlarm(
-        "Gpaw relies on the gpaw module but th is unavailable. Please ensure your python environment contains gpaw, "
-        "e.g. by running `conda install -c conda-forge gpaw`."
-    )
 
 
 class Gpaw(AseJob, GenericDFTJob):
     @import_alarm
     def __init__(self, project, job_name):
         super(Gpaw, self).__init__(project, job_name)
-        self.__name__ = "GpawJob"
+
         self.input = GpawInput()
 
     @property
     def plane_wave_cutoff(self):
         return self.input["encut"]
 
     @plane_wave_cutoff.setter
@@ -56,62 +51,48 @@
         manual_kpoints=None,
         weights=None,
         reciprocal=True,
         n_path=None,
         path_name=None,
     ):
         if scheme != "MP":
-            raise ValueError(
-                "Currently only MP is supported in the pyiron wrapper."
-            )
+            raise ValueError("Currently only MP is supported in the pyiron wrapper.")
         if center_shift is not None:
-            raise ValueError(
-                "centershift is not implemented in the pyiron wrapper."
-            )
+            raise ValueError("centershift is not implemented in the pyiron wrapper.")
         if not symmetry_reduction:
             raise ValueError(
                 "symmetry_reduction is not implemented in the pyiron wrapper."
             )
         if manual_kpoints is not None:
             raise ValueError(
                 "manual_kpoints are not implemented in the pyiron wrapper."
             )
         if weights is not None:
-            raise ValueError(
-                "weights are not implemented in the pyiron wrapper."
-            )
+            raise ValueError("weights are not implemented in the pyiron wrapper.")
         if not reciprocal:
-            raise ValueError(
-                "reciprocal is not implemented in the pyiron wrapper."
-            )
+            raise ValueError("reciprocal is not implemented in the pyiron wrapper.")
         if n_path is not None:
-            raise ValueError(
-                "n_path is not implemented in the pyiron wrapper."
-            )
+            raise ValueError("n_path is not implemented in the pyiron wrapper.")
         if path_name is not None:
-            raise ValueError(
-                "path_name is not implemented in the pyiron wrapper."
-            )
+            raise ValueError("path_name is not implemented in the pyiron wrapper.")
         self.input["kpoints"] = mesh
 
     def set_calculator(self):
         kpoints = self.input["kpoints"]
         if isinstance(kpoints, str):
-            kpoints = (
-                self.input["kpoints"].replace("[", "").replace("]", "").split()
-            )
+            kpoints = self.input["kpoints"].replace("[", "").replace("]", "").split()
         self._create_working_directory()
         calc = GPAWcode(
             mode=PW(float(self.input["encut"])),
             xc=self.input["potential"],
             occupations=MethfesselPaxton(width=float(self.input["sigma"])),
             kpts=kpoints,
             txt=self.working_directory + "/" + self.job_name + ".txt",
         )
-        self.structure.set_calculator(calc)
+        self.structure.calc = calc
 
     def to_hdf(self, hdf=None, group_name=None):
         """
         Store the ExampleJob object in the HDF5 File
 
         Args:
             hdf (ProjectHDFio): HDF5 group object - optional
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/interactive/activation_relaxation_technique.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/activation_relaxation_technique.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
-from pyiron_atomistics.atomistics.job.interactivewrapper import InteractiveWrapper, ReferenceJobOutput
-from pyiron_base import DataContainer, Settings
+from pyiron_atomistics.atomistics.job.interactivewrapper import (
+    InteractiveWrapper,
+    ReferenceJobOutput,
+)
+from pyiron_base import DataContainer
 
 __author__ = "Osamu Waseda"
-__copyright__ = "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH " \
-                "- Computational Materials Design (CM) Department"
+__copyright__ = (
+    "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH "
+    "- Computational Materials Design (CM) Department"
+)
 __version__ = "1.0"
 __maintainer__ = "Osamu Waseda"
 __email__ = "waseda@mpie.de"
 __status__ = "development"
 __date__ = "Sep 1, 2018"
 
-s = Settings()
-
 
 class ARTInteractive(object):
     def __init__(self, art_id, direction, gamma=0.1, fix_layer=False, non_art_id=None):
         if int(art_id) != art_id or art_id < 0:
-            raise ValueError('art_id must be a posive integer')
+            raise ValueError("art_id must be a posive integer")
         if len(direction) != 3 or np.isclose(np.linalg.norm(direction), 0):
-            raise ValueError('direction must be a finite 3d vector')
+            raise ValueError("direction must be a finite 3d vector")
         if gamma < 0:
-            raise ValueError('gamma must be a positive float')
+            raise ValueError("gamma must be a positive float")
         if fix_layer and non_art_id is not None:
-            raise ValueError('fix_layer and non_art_id cannot be set at the same time')
+            raise ValueError("fix_layer and non_art_id cannot be set at the same time")
         self.art_id = art_id
         self.direction = direction
         self.gamma = gamma
         self.non_art_id = non_art_id
         if non_art_id is not None:
             self.non_art_id = np.array([non_art_id]).flatten()
         self.fix_layer = fix_layer
@@ -44,22 +47,27 @@
 
     def get_forces(self, f_in):
         f = np.array(f_in)
         if len(f.shape) == 2:
             f = np.array([f])
         if self.non_art_id is None:
             self.non_art_id = np.arange(len(f[0])) != self.art_id
-        f_art = (1.0+self.gamma)*np.einsum('ij,nj->ni', self._R, f[:, self.art_id])
+        f_art = (1.0 + self.gamma) * np.einsum("ij,nj->ni", self._R, f[:, self.art_id])
         if self.fix_layer:
-            f[:, self.non_art_id] = np.einsum('nmj,ij->nmi', f[:, self.non_art_id], np.identity(3)-self._R)
+            f[:, self.non_art_id] = np.einsum(
+                "nmj,ij->nmi", f[:, self.non_art_id], np.identity(3) - self._R
+            )
         else:
-            f[:, self.non_art_id] += f_art[:, np.newaxis, :] / np.sum(self.non_art_id != False)
+            f[:, self.non_art_id] += f_art[:, np.newaxis, :] / np.sum(
+                self.non_art_id != False
+            )
         f[:, self.art_id] -= f_art
         return f.reshape(np.array(f_in).shape)
 
+
 class ART(InteractiveWrapper):
     """
     Apply an artificial force according to the Activation Relaxation Technique (ART)
     DOI:https://doi.org/10.1103/PhysRevE.57.2419
 
     The applied force f_art is calculated from the original force f by:
 
@@ -98,18 +106,19 @@
         >>> art.input.art_id = art_id
         >>> art.input.direction = direction
         >>> some_minimizer.ref_job = art
         >>> some_minimizer.run()
 
 
     """
+
     def __init__(self, project, job_name):
         super(ART, self).__init__(project, job_name)
-        self.__name__ = "ART"
-        self.input = DataContainer(table_name='custom_dict')
+
+        self.input = DataContainer(table_name="custom_dict")
         self.input.gamma = 0.1
         self.input.fix_layer = False
         self.input.non_art_id = None
         self.input.art_id = None
         self.input.direction = None
         self.output = ARTIntOutput(job=self)
         self.server.run_mode.interactive = True
@@ -127,38 +136,38 @@
     def art(self):
         if self._art is None:
             self._art = ARTInteractive(
                 art_id=self.input.art_id,
                 direction=self.input.direction,
                 gamma=self.input.gamma,
                 fix_layer=self.input.fix_layer,
-                non_art_id=self.input.non_art_id
+                non_art_id=self.input.non_art_id,
             )
         return self._art
 
     def run_if_interactive(self):
-        self._logger.debug('art status: ' + str(self.status))
+        self._logger.debug("art status: " + str(self.status))
         if not self.status.running:
             self.ref_job_initialize()
         self.status.running = True
         if self.ref_job.server.run_mode.interactive:
             self.ref_job.run()
         else:
             self.ref_job.run(run_again=True)
-        self._logger.debug('art status: ' + str(self.status))
+        self._logger.debug("art status: " + str(self.status))
 
     def interactive_forces_getter(self):
         return self.art.get_forces(self.ref_job.output.forces[-1])
 
     def validate_ready_to_run(self):
         """
-            check whether art_id and direction are set
+        check whether art_id and direction are set
         """
         if self.input.art_id is None or self.input.direction is None:
-            raise AssertionError('art_id and/or direction not set')
+            raise AssertionError("art_id and/or direction not set")
 
     def interactive_close(self):
         self.status.collect = True
         if self.ref_job.server.run_mode.interactive:
             self.ref_job.interactive_close()
         self.status.finished = True
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/interactive/scipy_minimizer.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/scipy_minimizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
 from pyiron_atomistics.atomistics.job.interactivewrapper import InteractiveWrapper
-from pyiron_base import DataContainer
+from pyiron_base import HasStorage
 from pyiron_atomistics.atomistics.job.interactive import GenericInteractiveOutput
 from scipy.optimize import minimize
 import scipy
+from typing import List, Iterable
 import warnings
 
 __author__ = "Osamu Waseda"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -63,19 +64,20 @@
     mathematically ill-defined problem and therefore it might end up in a
     physically undefined state. For this reason, it is strongly recommended to
     launch several jobs using the Murnaghan class (cf. `Murnaghan`).
 
     In order to perform volume optimization, the child job must have
     3x3-pressure output.
     """
+
     def __init__(self, project, job_name):
         super(ScipyMinimizer, self).__init__(project, job_name)
-        self.__name__ = "ScipyMinimizer"
+
         self._ref_job = None
-        self.input = Input()
+        self.input = ScipyMinimizerInput()
         self.output = ScipyMinimizerOutput(job=self)
         self.interactive_cache = {}
         self._delete_existing_job = True
 
     def set_input_to_read_only(self):
         """
         This function enforces read-only mode for the input classes, but it
@@ -96,40 +98,41 @@
         self._logger.debug("cg status: " + str(self.status))
         self._initialize_structure()
         if self.ref_job.server.run_mode.interactive:
             self._delete_existing_job = False
         self.ref_job.run(delete_existing_job=self._delete_existing_job)
         self.status.running = True
         if self.input.pressure is not None:
-            x0 = np.zeros(sum(self.input.pressure!=None))
+            x0 = np.zeros(sum(self.input.pressure != None))
             if not self.input.volume_only:
-                x0 = np.append(x0, self.ref_job.structure.get_scaled_positions().flatten())
+                x0 = np.append(
+                    x0, self.ref_job.structure.get_scaled_positions().flatten()
+                )
         else:
             x0 = self.ref_job.structure.positions.flatten()
         self.output._result = minimize(
             method=self.input.minimizer,
             fun=self._get_value,
             x0=x0,
-            jac=self._get_gradient,
-            tol=1.0e-20,
-            options={'maxiter': self.input.ionic_steps,
-                     'return_all': True }
+            jac=self._get_gradient if self.input.use_pressure else None,
+            tol=self.input.ionic_energy_tolerance,
+            options={"maxiter": self.input.ionic_steps, "return_all": True},
         )
         self.status.collect = True
         self.collect_output()
         if self.ref_job.server.run_mode.interactive:
             self.ref_job.interactive_close()
         if self["output/convergence"] > 0:
             self.status.finished = True
         else:
             self.status.not_converged = True
 
     @staticmethod
     def _tensor_to_voigt(s, strain=False):
-        ss = 0.5*(s+s.T)
+        ss = 0.5 * (s + s.T)
         ss = ss.flatten()[[0, 4, 8, 5, 2, 1]]
         if strain:
             ss[3:] *= 2
         return ss
 
     @staticmethod
     def _voigt_to_tensor(s, strain=False):
@@ -139,104 +142,121 @@
         ss = np.array([[ss[0], ss[5], ss[4]], [0, ss[1], ss[3]], [0, 0, ss[2]]])
         ss += ss.T
         return ss
 
     def _update(self, x):
         rerun = False
         if self.input.pressure is not None:
-            if not np.allclose(x[:len(self.input.pressure)], self._current_strain):
-                if len(self.input.pressure)==1:
+            if not np.allclose(x[: len(self.input.pressure)], self._current_strain):
+                if len(self.input.pressure) == 1:
                     self._current_strain[:3] = x[0]
                 else:
-                    self._current_strain[self.input.pressure!=None] = x[:len(self.input.pressure)]
+                    self._current_strain[self.input.pressure != None] = x[
+                        : len(self.input.pressure)
+                    ]
                 cell = np.matmul(
-                    self._voigt_to_tensor(self._current_strain, strain=True)+np.eye(3),
-                    self._original_cell
+                    self._voigt_to_tensor(self._current_strain, strain=True)
+                    + np.eye(3),
+                    self._original_cell,
                 )
                 self.ref_job.structure.set_cell(cell, scale_atoms=True)
                 rerun = True
-            if (not self.input.volume_only
-                and not np.allclose(
-                    x[len(self.input.pressure):], self.ref_job.structure.get_scaled_positions().flatten()
-                )):
-                self.ref_job.structure.set_scaled_positions(x[len(self.input.pressure):].reshape(-1, 3))
+            if not self.input.volume_only and not np.allclose(
+                x[len(self.input.pressure) :],
+                self.ref_job.structure.get_scaled_positions().flatten(),
+            ):
+                self.ref_job.structure.set_scaled_positions(
+                    x[len(self.input.pressure) :].reshape(-1, 3)
+                )
                 rerun = True
         elif not np.allclose(x, self.ref_job.structure.positions.flatten()):
             self.ref_job.structure.positions = x.reshape(-1, 3)
             rerun = True
         if rerun:
             self.ref_job.run(delete_existing_job=self._delete_existing_job)
 
     def check_convergence(self):
         if self.input.ionic_energy_tolerance > 0:
             if len(self.ref_job.output.energy_pot) < 2:
                 return False
-            elif np.absolute(np.diff(self.ref_job.output.energy_pot)[-1]) > self.input.ionic_energy_tolerance:
+            elif (
+                np.absolute(np.diff(self.ref_job.output.energy_pot)[-1])
+                > self.input.ionic_energy_tolerance
+            ):
                 return False
-            if self.input.ionic_force_tolerance==0:
+            if self.input.ionic_force_tolerance == 0:
                 return True
         max_force = np.linalg.norm(self.ref_job.output.forces[-1], axis=-1).max()
         if self.input.pressure is None:
             if max_force > self.input.ionic_force_tolerance:
                 return False
         elif self.input.volume_only:
-            if np.absolute(self._get_pressure()-self.input.pressure).max() > self.input.pressure_tolerance:
+            if self.input.use_pressure and (
+                np.absolute(self._get_pressure() - self.input.pressure).max()
+                > self.input.pressure_tolerance
+            ):
                 return False
         else:
             if max_force > self.input.ionic_force_tolerance:
                 return False
-            if np.absolute(self._get_pressure()-self.input.pressure).max() > self.input.pressure_tolerance:
+            if self.input.use_pressure and (
+                np.absolute(self._get_pressure() - self.input.pressure).max()
+                > self.input.pressure_tolerance
+            ):
                 return False
         return True
 
     def _get_pressure(self):
-        if len(self.input.pressure)==1:
+        if len(self.input.pressure) == 1:
             return [np.mean(np.diagonal(self.ref_job.output.pressures[-1]))]
         else:
-            return self._tensor_to_voigt(self.ref_job.output.pressures[-1])[self.input.pressure!=None]
+            return self._tensor_to_voigt(self.ref_job.output.pressures[-1])[
+                self.input.pressure != None
+            ]
 
     def _get_gradient(self, x):
         self._update(x)
         prefactor = 1.0e-1
         if self.check_convergence():
             prefactor = 0
         if self.input.pressure is not None:
-            pressure = -(
-                self._get_pressure()-self.input.pressure
-            )
+            pressure = -(self._get_pressure() - self.input.pressure)
             if self.input.volume_only:
-                return pressure*prefactor
+                return pressure * prefactor
             else:
-                return np.append(
-                    pressure,
-                    -np.einsum(
-                        'ij,ni->nj',
-                        np.linalg.inv(self.ref_job.structure.cell),
-                        self.ref_job.output.forces[-1]
+                return (
+                    np.append(
+                        pressure,
+                        -np.einsum(
+                            "ij,ni->nj",
+                            np.linalg.inv(self.ref_job.structure.cell),
+                            self.ref_job.output.forces[-1],
+                        ).flatten(),
                     ).flatten()
-                ).flatten()*prefactor
+                    * prefactor
+                )
         else:
-            return -self.ref_job.output.forces[-1].flatten()*prefactor
+            return -self.ref_job.output.forces[-1].flatten() * prefactor
 
     def _get_value(self, x):
         self._update(x)
         return self.ref_job.output.energy_pot[-1]
 
     def collect_output(self):
         self.output.to_hdf(self._hdf5)
 
     def to_hdf(self, hdf=None, group_name=None):
         super(ScipyMinimizer, self).to_hdf(hdf=hdf, group_name=group_name)
-        self.output.to_hdf(self._hdf5)
+        self.output.to_hdf(self.project_hdf5)
 
     def calc_minimize(
         self,
         max_iter=100,
         pressure=None,
-        algorithm='CG',
+        algorithm="CG",
         ionic_energy_tolerance=0,
         ionic_force_tolerance=1.0e-2,
         pressure_tolerance=1.0e-3,
         volume_only=False,
     ):
         """
         Args:
@@ -246,61 +266,133 @@
             ionic_energy_tolerance (float): convergence goal in terms of
                                   energy (optional)
             ionic_force_tolerance (float): convergence goal in terms of
                                   forces (optional)
             volume_only (bool): Only pressure minimization
         """
         if pressure is None and volume_only:
-            raise ValueError('pressure must be specified if volume_only')
+            raise ValueError("pressure must be specified if volume_only")
         if pressure is not None and not volume_only:
             warnings.warn(
-                'Simultaneous optimization of pressures and positions is a'
-                + ' mathematically ill posed problem - there is no guarantee'
-                + ' that it converges to the desired structure'
+                "Simultaneous optimization of pressures and positions is a"
+                + " mathematically ill posed problem - there is no guarantee"
+                + " that it converges to the desired structure"
             )
         if pressure is not None:
             pressure = np.array([pressure]).flatten()
-            if len(pressure)==9:
-                pressure = self._tensor_to_voigt(pressure.reshape(3,3))
-            if len(pressure)==3:
-                pressure = np.append(pressure, 3*[None])
+            if len(pressure) == 9:
+                pressure = self._tensor_to_voigt(pressure.reshape(3, 3))
+            if len(pressure) == 3:
+                pressure = np.append(pressure, 3 * [None])
         self.input.minimizer = algorithm
         self.input.ionic_steps = max_iter
         self.input.pressure = pressure
         self.input.volume_only = volume_only
         self.input.ionic_force_tolerance = ionic_force_tolerance
         self.input.ionic_energy_tolerance = ionic_energy_tolerance
         self.input.pressure_tolerance = pressure_tolerance
 
 
-class Input(DataContainer):
-    """
-    Args:
-        minimizer (str): minimizer to use (currently only 'CG' and 'BFGS' run
-            reliably)
-        ionic_steps (int): max number of steps
-        ionic_force_tolerance (float): maximum force tolerance
-    """
+class ScipyMinimizerInput(HasStorage):
+    def __init__(self):
+        super().__init__()
+        self.storage.minimizer = "CG"
+        self.storage.ionic_steps = 100
+        self.storage.ionic_energy_tolerance = 0
+        self.storage.ionic_force_tolerance = 1.0e-2
+        self.storage.pressure_tolerance = 1.0e-3
+        self.storage.pressure = None
+        self.storage.use_pressure = True
+        self.storage.volume_only = False
+
+    def _get_hdf_group_name(self) -> str:
+        return "parameters"
+
+    @property
+    def minimizer(self) -> str:
+        """str: name of minimizer to use"""
+        return self.storage.minimizer
+
+    @minimizer.setter
+    def minimizer(self, value: str):
+        self.storage.minimizer = value
+
+    @property
+    def ionic_steps(self) -> int:
+        """int: maximum number of minimization steps"""
+        return self.storage.ionic_steps
+
+    @ionic_steps.setter
+    def ionic_steps(self, value: int):
+        self.storage.ionic_steps = value
+
+    @property
+    def ionic_force_tolerance(self) -> float:
+        """float: convergence goal in terms of forces"""
+        return self.storage.ionic_force_tolerance
+
+    @ionic_force_tolerance.setter
+    def ionic_force_tolerance(self, value: float):
+        self.storage.ionic_force_tolerance = value
+
+    @property
+    def ionic_energy_tolerance(self) -> float:
+        """float: convergence goal in terms of energye"""
+        return self.storage.ionic_energy_tolerance
+
+    @ionic_energy_tolerance.setter
+    def ionic_energy_tolerance(self, value: float):
+        self.storage.ionic_energy_tolerance = value
+
+    @property
+    def pressure_tolerance(self) -> float:
+        """float: convergence goal in terms of energye"""
+        return self.storage.pressure_tolerance
+
+    @pressure_tolerance.setter
+    def pressure_tolerance(self, value: float):
+        self.storage.pressure_tolerance = value
+
+    @property
+    def pressure(self):
+        """float: target pressure"""
+        if isinstance(self.storage.pressure, Iterable):
+            return np.asarray(self.storage.pressure)
+        else:
+            return self.storage.pressure
 
-    def __init__(self, input_file_name=None, table_name="input"):
-        self.minimizer = 'CG'
-        self.ionic_steps = 100
-        self.ionic_force_tolerance = 1.0e-2
-        self.pressure = None
-        self.volume_only = False
-        self.ionic_energy_tolerance = 0
-        self.pressure_tolerance = 1.0e-3
+    @pressure.setter
+    def pressure(self, value: Iterable[float]):
+        value = list(value)
+        self.storage.pressure = value
+
+    @property
+    def use_pressure(self) -> bool:
+        """bool: rely on pressures computed by reference job or not"""
+        return self.storage.use_pressure
+
+    @use_pressure.setter
+    def use_pressure(self, value: bool):
+        self.storage.use_pressure = value
+
+    @property
+    def volume_only(self) -> bool:
+        """bool: only pressure minimization"""
+        return self.storage.volume_only
+
+    @volume_only.setter
+    def volume_only(self, value: bool):
+        self.storage.volume_only = value
 
 
 class ScipyMinimizerOutput(GenericInteractiveOutput):
     def __init__(self, job):
         super(ScipyMinimizerOutput, self).__init__(job=job)
         self._result = None
 
     def to_hdf(self, hdf, group_name="output"):
         if self._result is None:
             return
         with hdf.open(group_name) as hdf_output:
-            hdf_output["convergence"] = self._result['success']
-            if 'hess_inv' in self._result.keys():
-                hdf_output["hessian"] = self._result['hess_inv']
-
+            hdf_output["convergence"] = self._result["success"]
+            if "hess_inv" in self._result.keys():
+                hdf_output["hessian"] = self._result["hess_inv"]
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/interactive/sxextoptint.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/sxextoptint.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import numpy as np
 import subprocess
 import os
 import time
 import posixpath
 import warnings
-from pyiron_base import Settings, GenericParameters, Executable, deprecate
+from pyiron_base import state, GenericParameters, Executable, deprecate
 from pyiron_atomistics.atomistics.job.interactivewrapper import (
     InteractiveWrapper,
     ReferenceJobOutput,
 )
 from pyiron_atomistics.atomistics.job.interactive import InteractiveInterface
 from pyiron_atomistics.sphinx.base import InputWriter
 
@@ -24,20 +24,19 @@
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "development"
 __date__ = "Sep 1, 2018"
 
 
-s = Settings()
-
-
 class SxExtOpt(InteractiveInterface):
-    @deprecate(ionic_forces="Use ionic_force_tolerance",
-               ionic_energy="use ionic_energy_tolerance")
+    @deprecate(
+        ionic_forces="Use ionic_force_tolerance",
+        ionic_energy="use ionic_energy_tolerance",
+    )
     def __init__(
         self,
         structure,
         working_directory=None,
         maxDist=5,
         ionic_steps=1000,
         ionic_energy=None,
@@ -50,24 +49,24 @@
         ssa=False,
     ):
         if ionic_forces is not None:
             ionic_force_tolerance = ionic_forces
         if ionic_energy is not None:
             ionic_energy_tolerance = ionic_energy
         super().__init__()
-        self.__name__ = "SxExtOpt"
+
         if working_directory is None:
             warnings.warn("WARNING: working_directory not set; current folder is used")
             working_directory = os.getcwd()
         self._interactive_library = None
         self._interactive_library_read = None
         self.working_directory = working_directory
         if executable is None:
             executable = Executable(
-                path_binary_codes=s.resource_paths,
+                path_binary_codes=state.settings.resource_paths,
                 codename="SxExtOptInteractive",
                 module=self.__module__.split(".")[1],
                 overwrite_nt_flag=False,
             ).executable_path
         self._start_process(
             structure=structure,
             executable=executable,
@@ -81,19 +80,19 @@
             ssa=ssa,
         )
         self._cell = structure.cell
         if ssa:
             self._elements = structure.get_parent_symbols()
         else:
             magmom = structure.get_initial_magnetic_moments()
-            magmom[magmom!=None] = np.round(magmom[magmom!=None], decimals=1)
-            magmom = np.char.mod('%s', magmom)
+            magmom[magmom != None] = np.round(magmom[magmom != None], decimals=1)
+            magmom = np.char.mod("%s", magmom)
             self._elements = np.char.add(structure.get_parent_symbols(), magmom)
-            self._elements = np.char.replace(self._elements, '-', 'm')
-            self._elements = np.char.replace(self._elements, '.', 'p')
+            self._elements = np.char.replace(self._elements, "-", "m")
+            self._elements = np.char.replace(self._elements, ".", "p")
         self._positions = structure.positions
         self._converged = False
 
     def _start_process(
         self,
         structure,
         executable,
@@ -106,15 +105,17 @@
         selective_dynamics=False,
         ssa=False,
     ):
         if selective_dynamics:
             input_writer_obj = InputWriter()
             input_writer_obj.structure = structure
             if ssa:
-                input_writer_obj.structure.set_initial_magnetic_moments(len(structure)*[None])
+                input_writer_obj.structure.set_initial_magnetic_moments(
+                    len(structure) * [None]
+                )
             input_writer_obj.write_structure(
                 file_name="structure.sx",
                 cwd=self.working_directory,
                 structure_str=None,
                 symmetry_enabled=True,
                 keep_angstrom=True,
             )
@@ -198,15 +199,15 @@
 
     def interactive_close(self):
         if self.interactive_is_activated():
             self._interactive_library.close()
             self._interactive_library_read.close()
             self._delete_named_pipes(working_directory=self.working_directory)
 
-    @staticmethod 
+    @staticmethod
     def _delete_named_pipes(working_directory):
         for file in ["control", "response"]:
             file_path = posixpath.join(working_directory, file)
             if os.path.exists(file_path):
                 os.remove(file_path)
 
     def interactive_is_activated(self):
@@ -290,18 +291,18 @@
         else:
             self._delete_named_pipes(working_directory=self.working_directory)
 
 
 class SxExtOptInteractive(InteractiveWrapper):
     def __init__(self, project, job_name):
         super(SxExtOptInteractive, self).__init__(project, job_name)
-        self.__name__ = "SxExtOptInteractive"
+
         self.__version__ = (
-            None
-        )  # Reset the version number to the executable is set automatically
+            None  # Reset the version number to the executable is set automatically
+        )
         self._executable_activate()
         self.input = Input()
         self.output = SxExtOptOutput(job=self)
         self._interactive_interface = None
         self._interactive_number_of_steps = 0
 
     def set_input_to_read_only(self):
@@ -313,29 +314,29 @@
         self.input.read_only = True
 
     def write_input(self):
         pass
 
     def run_static(self):
         """
-        The run if modal function is called by run to execute the simulation, while waiting for the output. For this we
-        use subprocess.check_output()
+        The run if modal function is called by run to execute the simulation,
+        while waiting for the output. For this we use subprocess.check_output()
         """
         self._create_working_directory()
         self._interactive_interface = SxExtOpt(
             structure=self.ref_job.structure,
             working_directory=self.working_directory,
             maxDist=int(self.input["maxDist"]),
             ionic_steps=int(self.input["ionic_steps"]),
             ionic_energy_tolerance=float(self.input["ionic_energy_tolerance"]),
             ionic_force_tolerance=float(self.input["ionic_force_tolerance"]),
             max_step_length=float(self.input["max_step_length"]),
             soft_mode_damping=float(self.input["soft_mode_damping"]),
             executable=self.executable.executable_path,
-            ssa=self.input['ssa'],
+            ssa=self.input["ssa"],
         )
         self.status.running = True
         self._logger.info("job status: %s", self.status)
         new_positions = self.ref_job.structure.positions
         self.ref_job_initialize()
         while (
             self._interactive_number_of_steps < self.input["ionic_steps"]
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/base.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,55 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from __future__ import print_function, unicode_literals
 import os
-import posixpath
 
 import ast
-import h5py
 import numpy as np
 import pandas as pd
 import warnings
-from io import StringIO
 
-from pyiron_atomistics.lammps.potential import LammpsPotentialFile, PotentialAvailable
+from pyiron_base import state, deprecate
+from pyiron_atomistics.lammps.potential import (
+    LammpsPotentialFile,
+    PotentialAvailable,
+    view_potentials,
+    list_potentials,
+)
 from pyiron_atomistics.atomistics.job.atomistic import AtomisticGenericJob
-from pyiron_base import Settings, extract_data_from_file, deprecate
 from pyiron_atomistics.lammps.control import LammpsControl
 from pyiron_atomistics.lammps.potential import LammpsPotential
-from pyiron_atomistics.lammps.structure import LammpsStructure, UnfoldingPrism
+from pyiron_atomistics.lammps.structure import (
+    LammpsStructure,
+    UnfoldingPrism,
+    structure_to_lammps,
+)
+from pyiron_atomistics.lammps.units import UnitConverter, LAMMPS_UNIT_CONVERSIONS
+from pyiron_atomistics.lammps.output import (
+    collect_output_log,
+    collect_h5md_file,
+    collect_dump_file,
+    collect_errors,
+    remap_indices,
+)
 
 __author__ = "Joerg Neugebauer, Sudarsan Surendralal, Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH "
     "- Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Sudarsan Surendralal"
 __email__ = "surendralal@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 
-s = Settings()
-
-
 class LammpsBase(AtomisticGenericJob):
     """
     Class to setup and run and analyze LAMMPS simulations which is a derivative of
     atomistics.job.generic.GenericJob. The functions in these modules are written in such the function names and
     attributes are very generic (get_structure(), molecular_dynamics(), version) but the functions are written to handle
     LAMMPS specific input/output.
 
@@ -53,29 +64,65 @@
     def __init__(self, project, job_name):
         super(LammpsBase, self).__init__(project, job_name)
         self.input = Input()
         self._cutoff_radius = None
         self._is_continuation = None
         self._compress_by_default = True
         self._prism = None
-        s.publication_add(self.publication)
+        state.publications.add(self.publication)
+
+    @property
+    def units(self):
+        """
+        Type of LAMMPS units used in the calculations. Can be either of 'metal', 'real', 'si', 'cgs', and 'lj'
+
+        Returns:
+            str: Type of LAMMPS unit
+        """
+        if self.input.control["units"] is not None:
+            return self.input.control["units"]
+        else:
+            # Default to metal units
+            return "metal"
+
+    @units.setter
+    def units(self, val):
+        allowed_types = LAMMPS_UNIT_CONVERSIONS.keys()
+        if val in allowed_types:
+            self.input.control["units"] = val
+        else:
+            raise ValueError("'{}' is not a valid LAMMPS unit")
 
     @property
     def bond_dict(self):
         """
         A dictionary which defines the nature of LAMMPS bonds that are to be drawn between atoms. To set the values, use
         the function `define_bonds`.
 
         Returns:
             dict: Dictionary of the bond properties for every species
 
         """
         return self.input.bond_dict
 
-    def define_bonds(self, species, element_list, cutoff_list, max_bond_list, bond_type_list, angle_type_list=None):
+    def clear_bonds(self) -> None:
+        """
+        Clears all pre-defined bonds
+        """
+        self.input.bond_dict = {}
+
+    def define_bonds(
+        self,
+        species,
+        element_list,
+        cutoff_list,
+        max_bond_list,
+        bond_type_list,
+        angle_type_list=None,
+    ):
         """
         Define the nature of bonds between different species. Make sure that the bonds between two species are defined
         only once (no double counting).
 
         Args:
             species (str): Species for which the bonds are to be drawn (e.g. O, H, C ..)
             element_list (list): List of species to which the bonds are to be made (e.g. O, H, C, ..)
@@ -100,16 +147,18 @@
                 self.input.bond_dict[species]["bond_type_list"] = bond_type_list
                 self.input.bond_dict[species]["max_bond_list"] = max_bond_list
                 if angle_type_list is not None:
                     self.input.bond_dict[species]["angle_type_list"] = angle_type_list
                 else:
                     self.input.bond_dict[species]["angle_type_list"] = [None]
             else:
-                raise ValueError("The element list, cutoff list, max bond list, and the bond type list"
-                                 " must have the same length")
+                raise ValueError(
+                    "The element list, cutoff list, max bond list, and the bond type list"
+                    " must have the same length"
+                )
 
     @property
     def cutoff_radius(self):
         """
 
         Returns:
 
@@ -153,34 +202,35 @@
         if isinstance(potential_filename, stringtypes):
             if ".lmp" in potential_filename:
                 potential_filename = potential_filename.split(".lmp")[0]
             potential_db = LammpsPotentialFile()
             potential = potential_db.find_by_name(potential_filename)
         elif isinstance(potential_filename, pd.DataFrame):
             potential = potential_filename
+        elif hasattr(potential_filename, "get_df"):
+            potential = potential_filename.get_df()
         else:
             raise TypeError("Potentials have to be strings or pandas dataframes.")
         if self.structure:
             structure_elements = self.structure.get_species_symbols()
             potential_elements = list(potential["Species"])[0]
             if not set(structure_elements).issubset(potential_elements):
-                raise ValueError("Potential {} does not support elements "
-                                 "in structure {}.".format(
-                                     potential_elements,
-                                     structure_elements
-                                ))
+                raise ValueError(
+                    "Potential {} does not support elements "
+                    "in structure {}.".format(potential_elements, structure_elements)
+                )
         self.input.potential.df = potential
         if "Citations" in potential.columns.values:
             pot_pub_dict = {}
             pub_lst = potential["Citations"].values[0]
-            if isinstance(pub_lst, str):
+            if isinstance(pub_lst, str) and len(pub_lst) > 0:
                 for p in ast.literal_eval(pub_lst):
                     for k in p.keys():
                         pot_pub_dict[k] = p[k]
-            s.publication_add({"lammps_potential": pot_pub_dict})
+            state.publications.add({"lammps_potential": pot_pub_dict})
         for val in ["units", "atom_style", "dimension"]:
             v = self.input.potential[val]
             if v is not None:
                 self.input.control[val] = v
                 if val == "units" and v != "metal":
                     warnings.warn(
                         "WARNING: Non-'metal' units are not fully supported. Your calculation should run OK, but "
@@ -231,26 +281,39 @@
         Validating input parameters before LAMMPS run
         """
         super(LammpsBase, self).validate_ready_to_run()
         if self.potential is None:
             lst_of_potentials = self.list_potentials()
             if len(lst_of_potentials) > 0:
                 self.potential = lst_of_potentials[0]
-                warnings.warn("No potential set via job.potential - use default potential, " + lst_of_potentials[0])
+                warnings.warn(
+                    "No potential set via job.potential - use default potential, "
+                    + lst_of_potentials[0]
+                )
             else:
                 raise ValueError(
-                    "This job does not contain a valid potential: {}".format(self.job_name)
+                    "This job does not contain a valid potential: {}".format(
+                        self.job_name
+                    )
                 )
         scaled_positions = self.structure.get_scaled_positions(wrap=False)
         # Check if atoms located outside of non periodic box
-        conditions = [(np.min(scaled_positions[:, i]) < 0.0 or
-                       np.max(scaled_positions[:, i]) > 1.0) and not self.structure.pbc[i] for i in range(3)]
+        conditions = [
+            (
+                np.min(scaled_positions[:, i]) < 0.0
+                or np.max(scaled_positions[:, i]) > 1.0
+            )
+            and not self.structure.pbc[i]
+            for i in range(3)
+        ]
         if any(conditions):
-            raise ValueError("You have atoms located outside the non-periodic boundaries "
-                             "of the defined simulation box")
+            raise ValueError(
+                "You have atoms located outside the non-periodic boundaries "
+                "of the defined simulation box"
+            )
 
     def get_potentials_for_structure(self):
         """
 
         Returns:
 
         """
@@ -263,45 +326,35 @@
         Returns:
 
         """
         return self.get_structure(iteration_step=-1)
 
     def view_potentials(self):
         """
-        List all interatomic potentials for the current atomistic sturcture including all potential parameters.
+        List all interatomic potentials for the current atomistic structure including all potential parameters.
 
-        To quickly get only the names of the potentials you can use: self.potentials_list()
+        To quickly get only the names of the potentials you can use: self.list_potentials()
 
         Returns:
             pandas.Dataframe: Dataframe including all potential parameters.
         """
-        from pyiron_atomistics.lammps.potential import LammpsPotentialFile
-
         if not self.structure:
             raise ValueError("No structure set.")
-        list_of_elements = set(self.structure.get_chemical_symbols())
-        list_of_potentials = LammpsPotentialFile().find(list_of_elements)
-        if list_of_potentials is not None:
-            return list_of_potentials
-        else:
-            raise TypeError(
-                "No potentials found for this kind of structure: ",
-                str(list_of_elements),
-            )
+        return view_potentials(self.structure)
 
     def list_potentials(self):
         """
         List of interatomic potentials suitable for the current atomic structure.
 
-        use self.potentials_view() to get more details.
+        use self.view_potentials() to get more details.
 
         Returns:
             list: potential names
         """
-        return list(self.view_potentials()["Name"].values)
+        return list_potentials(self.structure)
 
     def enable_h5md(self):
         """
 
         Returns:
 
         """
@@ -443,36 +496,30 @@
         Args:
             file_name:
             cwd:
 
         Returns:
 
         """
-        prism = UnfoldingPrism(self.structure.cell, digits=15)
-        if np.matrix.trace(prism.R) != 3:
-            raise RuntimeError("The Lammps output will not be mapped back to pyiron correctly.")
-        file_name = self.job_file_name(file_name=file_name, cwd=cwd)
-        with h5py.File(file_name, mode="r", libver="latest", swmr=True) as h5md:
-            positions = [
-                pos_i.tolist() for pos_i in h5md["/particles/all/position/value"]
-            ]
-            steps = [steps_i.tolist() for steps_i in h5md["/particles/all/position/step"]]
-            forces = [for_i.tolist() for for_i in h5md["/particles/all/force/value"]]
-            # following the explanation at: http://nongnu.org/h5md/h5md.html
-            cell = [
-                np.eye(3) * np.array(cell_i.tolist())
-                for cell_i in h5md["/particles/all/box/edges/value"]
-            ]
-            indices = [indices_i.tolist() for indices_i in h5md["/particles/all/indices/value"]]
+        uc = UnitConverter(self.units)
+        forces, positions, steps, cell = collect_h5md_file(
+            file_name=self.job_file_name(file_name=file_name, cwd=cwd),
+            prism=self._prism,
+        )
         with self.project_hdf5.open("output/generic") as h5_file:
-            h5_file["forces"] = np.array(forces)
-            h5_file["positions"] = np.array(positions)
-            h5_file["steps"] = np.array(steps)
-            h5_file["cells"] = cell
-            h5_file["indices"] = self.remap_indices(indices)
+            h5_file["forces"] = uc.convert_array_to_pyiron_units(
+                np.array(forces), "forces"
+            )
+            h5_file["positions"] = uc.convert_array_to_pyiron_units(
+                np.array(positions), "positions"
+            )
+            h5_file["steps"] = uc.convert_array_to_pyiron_units(
+                np.array(steps), "steps"
+            )
+            h5_file["cells"] = uc.convert_array_to_pyiron_units(np.array(cell), "cells")
 
     def remap_indices(self, lammps_indices):
         """
         Give the Lammps-dumped indices, re-maps these back onto the structure's indices to preserve the species.
 
         The issue is that for an N-element potential, Lammps dumps the chemical index from 1 to N based on the order
         that these species are written in the Lammps input file. But the indices for a given structure are based on the
@@ -481,149 +528,70 @@
 
         Args:
             indices (numpy.ndarray/list): The Lammps-dumped integers.
 
         Returns:
             numpy.ndarray: Those integers mapped onto the structure.
         """
-        lammps_symbol_order = np.array(self.input.potential.get_element_lst())
-
-        # If new Lammps indices are present for which we have no species, extend the species list
-        unique_lammps_indices = np.unique(lammps_indices)
-        if len(unique_lammps_indices) > len(np.unique(self.structure.indices)):
-            unique_lammps_indices -= 1  # Convert from Lammps start counting at 1 to python start counting at 0
-            new_lammps_symbols = lammps_symbol_order[unique_lammps_indices]
-            self.structure.set_species([self.structure.convert_element(el) for el in new_lammps_symbols])
-
-        # Create a map between the lammps indices and structure indices to preserve species
-        structure_symbol_order = np.array([el.Abbreviation for el in self.structure.species])
-        map_ = np.array([int(np.argwhere(lammps_symbol_order == symbol)[0]) + 1 for symbol in structure_symbol_order])
-
-        structure_indices = np.array(lammps_indices)
-        for i_struct, i_lammps in enumerate(map_):
-            np.place(structure_indices, lammps_indices == i_lammps, i_struct)
-        # TODO: Vectorize this for-loop for computational efficiency
-
-        return structure_indices
-
-    def collect_errors(self, file_name, cwd=None):
-        """
-
-        Args:
-            file_name:
-            cwd:
-
-        Returns:
-
-        """
-        file_name = self.job_file_name(file_name=file_name, cwd=cwd)
-        error = extract_data_from_file(file_name, tag="ERROR", num_args=1000)
-        if len(error) > 0:
-            error = " ".join(error[0])
-            raise RuntimeError("Run time error occurred: " + str(error))
-        else:
-            return True
+        return remap_indices(
+            lammps_indices=lammps_indices,
+            potential_elements=self.input.potential.get_element_lst(),
+            structure=self.structure,
+        )
 
     def collect_output_log(self, file_name="log.lammps", cwd=None):
         """
         general purpose routine to extract static from a lammps log file
 
         Args:
             file_name:
             cwd:
 
         Returns:
 
         """
-        self.collect_errors(file_name=file_name, cwd=cwd)
         file_name = self.job_file_name(file_name=file_name, cwd=cwd)
+        collect_errors(file_name=file_name)
         if os.path.exists(file_name):
-            with open(file_name, "r") as f:
-                f = f.readlines()
-                l_start = np.where([line.startswith("Step") for line in f])[0]
-                l_end = np.where([line.startswith("Loop") for line in f])[0]
-                if len(l_start) > len(l_end):
-                    l_end = np.append(l_end, [None])
-                df = [
-                    pd.read_csv(
-                        StringIO("\n".join(f[llst:llen])), delim_whitespace=True
-                    )
-                    for llst, llen in zip(l_start, l_end)
-                ]
-            if len(df) == 1:
-                df = df[-1]
-            else:
-                df = pd.concat(df)
-
-            h5_dict = {
-                "Step": "steps",
-                "Temp": "temperature",
-                "PotEng": "energy_pot",
-                "TotEng": "energy_tot",
-                "Volume": "volume",
-            }
-
-            for key in df.columns[df.columns.str.startswith('f_mean')]:
-                h5_dict[key] = key.replace('f_', '')
-
-            df = df.rename(index=str, columns=h5_dict)
-            if all([x in df.columns.values for x in ["Pxx", "Pxy", "Pxz", "Pxy", "Pyy", "Pyz", "Pxz", "Pyz", "Pzz"]]):
-                pressures = np.stack(
-                    (df.Pxx, df.Pxy, df.Pxz, df.Pxy, df.Pyy, df.Pyz, df.Pxz, df.Pyz, df.Pzz),
-                    axis=-1,
-                ).reshape(-1, 3, 3).astype('float64')
-                pressures *= 0.0001  # bar -> GPa
-
-                # Rotate pressures from Lammps frame to pyiron frame if necessary
-                rotation_matrix = self._prism.R.T
-                if np.matrix.trace(rotation_matrix) != 3:
-                    pressures = rotation_matrix.T @ pressures @ rotation_matrix
-
-                df = df.drop(
-                    columns=df.columns[
-                        ((df.columns.str.len() == 3) & df.columns.str.startswith("P"))
-                    ]
-                )
-                df["pressures"] = pressures.tolist()
-            else:
-                warnings.warn("LAMMPS warning: log.lammps does not contain the required pressure values.")
-            if 'mean_pressure[1]' in df.columns:
-                pressures = np.stack(
-                    (df['mean_pressure[1]'], df['mean_pressure[4]'], df['mean_pressure[5]'],
-                     df['mean_pressure[4]'], df['mean_pressure[2]'], df['mean_pressure[6]'],
-                     df['mean_pressure[5]'], df['mean_pressure[6]'], df['mean_pressure[3]']),
-                    axis=-1,
-                ).reshape(-1, 3, 3).astype('float64')
-                pressures *= 0.0001  # bar -> GPa
-                if np.matrix.trace(rotation_matrix) != 3:
-                    pressures = rotation_matrix.T @ pressures @ rotation_matrix
-                df = df.drop(
-                    columns=df.columns[
-                        (df.columns.str.startswith("mean_pressure") & df.columns.str.endswith(']'))
-                    ]
-                )
-                df["mean_pressures"] = pressures.tolist()
-
+            generic_keys_lst, pressure_dict, df = collect_output_log(
+                file_name=file_name,
+                prism=self._prism,
+            )
+            uc = UnitConverter(self.units)
             with self.project_hdf5.open("output/generic") as hdf_output:
                 # This is a hack for backward comparability
                 for k, v in df.items():
-                    hdf_output[k] = np.array(v)
+                    if k in generic_keys_lst:
+                        hdf_output[k] = uc.convert_array_to_pyiron_units(
+                            np.array(v), label=k
+                        )
+                # Store pressures as numpy arrays
+                for key, val in pressure_dict.items():
+                    hdf_output[key] = uc.convert_array_to_pyiron_units(val, label=key)
+
+            with self.project_hdf5.open("output/lammps") as hdf_output:
+                # This is a hack for backward comparability
+                for k, v in df.items():
+                    if k not in generic_keys_lst:
+                        hdf_output[k] = uc.convert_array_to_pyiron_units(
+                            np.array(v), label=k
+                        )
         else:
             warnings.warn("LAMMPS warning: No log.lammps output file found.")
 
     def calc_minimize(
-            self,
-            ionic_energy_tolerance=0.0,
-            ionic_force_tolerance=1e-4,
-            e_tol=None,
-            f_tol=None,
-            max_iter=1000000,
-            pressure=None,
-            n_print=100,
-            style='cg'
+        self,
+        ionic_energy_tolerance=0.0,
+        ionic_force_tolerance=1e-4,
+        e_tol=None,
+        f_tol=None,
+        max_iter=1000000,
+        pressure=None,
+        n_print=100,
+        style="cg",
     ):
         rotation_matrix = self._get_rotation_matrix(pressure=pressure)
         # Docstring set programmatically -- Ensure that changes to signature or defaults stay consistent!
         if e_tol is not None:
             ionic_energy_tolerance = e_tol
         if f_tol is not None:
             ionic_force_tolerance = f_tol
@@ -639,16 +607,17 @@
         self.input.control.calc_minimize(
             ionic_energy_tolerance=ionic_energy_tolerance,
             ionic_force_tolerance=ionic_force_tolerance,
             max_iter=max_iter,
             pressure=pressure,
             n_print=n_print,
             style=style,
-            rotation_matrix=rotation_matrix
+            rotation_matrix=rotation_matrix,
         )
+
     calc_minimize.__doc__ = LammpsControl.calc_minimize.__doc__
 
     def calc_static(self):
         """
 
         Returns:
 
@@ -702,38 +671,39 @@
             seed=seed,
             tloop=tloop,
             initial_temperature=initial_temperature,
             langevin=langevin,
             delta_temp=delta_temp,
             delta_press=delta_press,
             job_name=self.job_name,
-            rotation_matrix=rotation_matrix
+            rotation_matrix=rotation_matrix,
         )
+
     calc_md.__doc__ = LammpsControl.calc_md.__doc__
 
     def calc_vcsgc(
         self,
         mu=None,
         target_concentration=None,
-        kappa=1000.,
+        kappa=1000.0,
         mc_step_interval=100,
         swap_fraction=0.1,
         temperature_mc=None,
         window_size=None,
         window_moves=None,
         temperature=None,
         pressure=None,
         n_ionic_steps=1000,
         time_step=1.0,
         n_print=100,
         temperature_damping_timescale=100.0,
         pressure_damping_timescale=1000.0,
         seed=None,
         initial_temperature=None,
-        langevin=False
+        langevin=False,
     ):
         """
         Run variance-constrained semi-grand-canonical MD/MC for a binary system. In addition to VC-SGC arguments, all
         arguments for a regular MD calculation are also accepted.
 
         https://vcsgc-lammps.materialsmodeling.org
 
@@ -767,18 +737,29 @@
             window_moves (int): The number of times the sampling window is moved during one MC cycle. (Default is None,
                 number of moves is determined automatically.)
         """
         rotation_matrix = self._get_rotation_matrix(pressure=pressure)
         if mu is None:
             mu = {}
             for el in self.input.potential.get_element_lst():
-                mu[el] = 0.
+                mu[el] = 0.0
 
         self._generic_input["calc_mode"] = "vcsgc"
+        self._generic_input["mu"] = mu
+        if target_concentration is not None:
+            self._generic_input["target_concentration"] = target_concentration
+            self._generic_input["kappa"] = kappa
+        self._generic_input["mc_step_interval"] = mc_step_interval
+        self._generic_input["swap_fraction"] = swap_fraction
         self._generic_input["temperature"] = temperature
+        self._generic_input["temperature_mc"] = temperature_mc
+        if window_size is not None:
+            self._generic_input["window_size"] = window_size
+        if window_moves is not None:
+            self._generic_input["window_moves"] = window_moves
         self._generic_input["n_ionic_steps"] = n_ionic_steps
         self._generic_input["n_print"] = n_print
         self._generic_input.remove_keys(["max_iter"])
         self.input.control.calc_vcsgc(
             mu=mu,
             ordered_element_list=self.input.potential.get_element_lst(),
             target_concentration=target_concentration,
@@ -795,15 +776,15 @@
             n_print=n_print,
             temperature_damping_timescale=temperature_damping_timescale,
             pressure_damping_timescale=pressure_damping_timescale,
             seed=seed,
             initial_temperature=initial_temperature,
             langevin=langevin,
             job_name=self.job_name,
-            rotation_matrix=rotation_matrix
+            rotation_matrix=rotation_matrix,
         )
 
     # define hdf5 input and output
     def to_hdf(self, hdf=None, group_name=None):
         """
 
         Args:
@@ -878,130 +859,41 @@
         Args:
             file_name:
             cwd:
 
         Returns:
 
         """
+        uc = UnitConverter(self.units)
         file_name = self.job_file_name(file_name=file_name, cwd=cwd)
-        if os.path.exists(file_name):
-            output = {}
-            with open(file_name, "r") as ff:
-                dump = ff.readlines()
-
-            steps = np.genfromtxt(
-                [
-                    dump[nn]
-                    for nn in np.where([ll.startswith("ITEM: TIMESTEP") for ll in dump])[0]
-                    + 1
-                ],
-                dtype=int,
-            )
-            steps = np.array([steps]).flatten()
-            output["steps"] = steps
 
-            natoms = np.genfromtxt(
-                [
-                    dump[nn]
-                    for nn in np.where(
-                        [ll.startswith("ITEM: NUMBER OF ATOMS") for ll in dump]
-                    )[0]
-                    + 1
-                ],
-                dtype=int,
+        if os.path.exists(file_name):
+            dump_dict = collect_dump_file(
+                file_name=file_name,
+                prism=self._prism,
+                structure=self.structure,
+                potential_elements=self.input.potential.get_element_lst(),
             )
-            natoms = np.array([natoms]).flatten()
-
-            prism = self._prism
-            rotation_lammps2orig = self._prism.R.T
-            cells = np.genfromtxt(
-                " ".join(
-                    (
-                        [
-                            " ".join(dump[nn:nn + 3])
-                            for nn in np.where(
-                                [ll.startswith("ITEM: BOX BOUNDS") for ll in dump]
-                            )[0]
-                            + 1
-                        ]
+            # Write to hdf
+            with self.project_hdf5.open("output/generic") as hdf_output:
+                for k, v in dump_dict.pop("computes").items():
+                    hdf_output[k] = uc.convert_array_to_pyiron_units(
+                        np.array(v), label=k
                     )
-                ).split()
-            ).reshape(len(natoms), -1)
-            lammps_cells = np.array([to_amat(cc) for cc in cells])
-            unfolded_cells = np.array([prism.unfold_cell(cell) for cell in lammps_cells])
-            output["cells"] = unfolded_cells
-
-
-            l_start = np.where([ll.startswith("ITEM: ATOMS") for ll in dump])[0]
-            l_end = l_start + natoms + 1
-            content = [
-                pd.read_csv(
-                    StringIO("\n".join(dump[llst:llen]).replace("ITEM: ATOMS ", "")),
-                    delim_whitespace=True,
-                )
-                for llst, llen in zip(l_start, l_end)
-            ]
-
-            indices = np.array([cc["type"] for cc in content], dtype=int)
-            output["indices"] = self.remap_indices(indices)
-
-            forces = np.array(
-                [np.stack((cc["fx"], cc["fy"], cc["fz"]), axis=-1) for cc in content]
-            )
-            output["forces"] = np.matmul(forces, rotation_lammps2orig)
-
-            if 'f_mean_forces[1]' in content[0].keys():
-                forces = np.array(
-                    [np.stack((cc["f_mean_forces[1]"],
-                               cc["f_mean_forces[2]"],
-                               cc["f_mean_forces[3]"]),
-                              axis=-1) for cc in content]
-                )
-                output["mean_forces"] = np.matmul(forces, rotation_lammps2orig)
-
-            if np.all([flag in content[0].columns.values for flag in ["vx", "vy", "vz"]]):
-                velocities = np.array(
-                    [np.stack((cc["vx"], cc["vy"], cc["vz"]), axis=-1) for cc in content]
-                )
-                output["velocities"] = np.matmul(velocities, rotation_lammps2orig)
 
-            if 'f_mean_velocities[1]' in content[0].keys():
-                velocities = np.array(
-                    [np.stack((cc["f_mean_velocities[1]"],
-                               cc["f_mean_velocities[2]"],
-                               cc["f_mean_velocities[3]"]),
-                              axis=-1) for cc in content]
+                hdf_output["steps"] = uc.convert_array_to_pyiron_units(
+                    np.array(dump_dict.pop("steps"), dtype=int), label="steps"
                 )
-                output["mean_velocities"] = np.matmul(velocities, rotation_lammps2orig)
-            direct_unwrapped_positions = np.array(
-                [np.stack((cc["xsu"], cc["ysu"], cc["zsu"]), axis=-1) for cc in content]
-            )
-            unwrapped_positions = np.matmul(direct_unwrapped_positions, lammps_cells)
-            output["unwrapped_positions"] = np.matmul(unwrapped_positions, rotation_lammps2orig)
-            if 'f_mean_positions[1]' in content[0].keys():
-                direct_unwrapped_positions = np.array(
-                    [np.stack((cc["f_mean_positions[1]"],
-                               cc["f_mean_positions[2]"],
-                               cc["f_mean_positions[3]"]),
-                              axis=-1) for cc in content]
-                )
-                unwrapped_positions = np.matmul(direct_unwrapped_positions, lammps_cells)
-                output["mean_unwrapped_positions"] = np.matmul(unwrapped_positions, rotation_lammps2orig)
 
-            direct_positions = direct_unwrapped_positions - np.floor(direct_unwrapped_positions)
-            positions = np.matmul(direct_positions, lammps_cells)
-            output["positions"] = np.matmul(positions, rotation_lammps2orig)
-
-            keys = content[0].keys()
-            for kk in keys[keys.str.startswith('c_')]:
-                output[kk.replace('c_', '')] = np.array([cc[kk] for cc in content], dtype=float)
+                for k, v in dump_dict.items():
+                    if len(v) > 0:
+                        hdf_output[k] = uc.convert_array_to_pyiron_units(
+                            np.array(v), label=k
+                        )
 
-            with self.project_hdf5.open("output/generic") as hdf_output:
-                for k, v in output.items():
-                    hdf_output[k] = v
         else:
             warnings.warn("LAMMPS warning: No dump.out output file found.")
 
     # Outdated functions:
     def set_potential(self, file_name):
         """
 
@@ -1021,68 +913,57 @@
             project (pyiron_atomistics.project.Project instance): Project instance at which the new job should be created
             job_name (str): Job name
             job_type (str): Job type. If not specified a Lammps job type is assumed
 
         Returns:
             new_ham (lammps.lammps.Lammps instance): New job
         """
-        return super(LammpsBase, self).restart(
-            job_name=job_name, job_type=job_type
-        )
+        return super(LammpsBase, self).restart(job_name=job_name, job_type=job_type)
 
     def restart(self, job_name=None, job_type=None):
         """
         Restart a new job created from an existing Lammps calculation.
         Args:
             project (pyiron_atomistics.project.Project instance): Project instance at which the new job should be created
             job_name (str): Job name
             job_type (str): Job type. If not specified a Lammps job type is assumed
 
         Returns:
-            new_ham (lammps.lammps.Lammps instance): New job
+            lammps.lammps.Lammps instance: New job
         """
-        new_ham = super(LammpsBase, self).restart(
-            job_name=job_name, job_type=job_type
-        )
+        new_ham = super(LammpsBase, self).restart(job_name=job_name, job_type=job_type)
         if new_ham.__name__ == self.__name__:
             new_ham.potential = self.potential
-            if os.path.isfile(os.path.join(self.working_directory, "restart.out")):
-                new_ham.read_restart_file(filename="restart.out")
-                new_ham.restart_file_list.append(
-                    posixpath.join(self.working_directory, "restart.out")
-                )
+            new_ham.read_restart_file(filename="restart.out")
+            new_ham.restart_file_list.append(self.get_workdir_file("restart.out"))
         return new_ham
 
+    @staticmethod
+    def _structure_to_lammps(structure):
+        """
+        Convert structure to LAMMPS compatible lower triangle format
+        Args:
+            structure (pyiron_atomistics.atomistics.structure.atoms.Atoms): Current structure
+
+        Returns:
+            pyiron_atomistics.atomistics.structure.atoms.Atoms: Converted structure
+        """
+        return structure_to_lammps(structure=structure)
+
     def _get_lammps_structure(self, structure=None, cutoff_radius=None):
-        lmp_structure = LammpsStructure(bond_dict=self.input.bond_dict)
+        lmp_structure = LammpsStructure(bond_dict=self.input.bond_dict, job=self)
         lmp_structure._force_skewed = self.input.control._force_skewed
         lmp_structure.potential = self.input.potential
         lmp_structure.atom_type = self.input.control["atom_style"]
         if cutoff_radius is not None:
             lmp_structure.cutoff_radius = cutoff_radius
         else:
             lmp_structure.cutoff_radius = self.cutoff_radius
         lmp_structure.el_eam_lst = self.input.potential.get_element_lst()
 
-        def structure_to_lammps(structure):
-            """
-            Converts a structure to the Lammps coordinate frame
-
-            Args:
-                structure (pyiron.atomistics.structure.atoms.Atoms): Structure to convert.
-
-            Returns:
-                pyiron.atomistics.structure.atoms.Atoms: Structure with the LAMMPS coordinate frame.
-            """
-            prism = UnfoldingPrism(structure.cell)
-            lammps_structure = structure.copy()
-            lammps_structure.set_cell(prism.A)
-            lammps_structure.positions = np.matmul(structure.positions, prism.R)
-            return lammps_structure
-
         if structure is not None:
             lmp_structure.structure = structure_to_lammps(structure)
         else:
             lmp_structure.structure = structure_to_lammps(self.structure)
         if not set(lmp_structure.structure.get_species_symbols()).issubset(
             set(lmp_structure.el_eam_lst)
         ):
@@ -1196,42 +1077,44 @@
                     ] = "constraintz setforce NULL NULL 0.0"
                     if self._generic_input["calc_mode"] == "md":
                         self.input.control[
                             "velocity___constraintz"
                         ] = "set NULL NULL 0.0"
 
     @staticmethod
-    def _modify_structure_to_allow_requested_deformation(structure, pressure, prism=None):
+    def _modify_structure_to_allow_requested_deformation(
+        structure, pressure, prism=None
+    ):
         """
         Lammps will not allow xy/xz/yz cell deformations in minimization or MD for non-triclinic cells. In case the
         requested pressure for a calculation has these non-diagonal entries, we need to make sure it will run. One way
         to do this is by invoking the lammps `change_box` command, but it is easier to just force our box to to be
         triclinic by adding a very small cell perturbation (in the case where it isn't triclinic already).
 
         Args:
             pressure (float/int/list/numpy.ndarray/tuple): Between three and six pressures for the x, y, z, xy, xz, and
                 yz directions, in that order, or a single value.
         """
-        if hasattr(pressure, '__len__'):
+        if hasattr(pressure, "__len__"):
             non_diagonal_pressures = np.any([p is not None for p in pressure[3:]])
 
             if prism is None:
                 prism = UnfoldingPrism(structure.cell)
 
             if non_diagonal_pressures:
                 try:
                     if not prism.is_skewed():
                         skew_structure = structure.copy()
                         skew_structure.cell[0, 1] += 2 * prism.acc
                         return skew_structure
                 except AttributeError:
                     warnings.warn(
-                        "WARNING: Setting a calculation type which uses pressure before setting the structure risks " +
-                        "constraining your cell shape evolution if non-diagonal pressures are used but the structure " +
-                        "is not triclinic from the start of the calculation."
+                        "WARNING: Setting a calculation type which uses pressure before setting the structure risks "
+                        + "constraining your cell shape evolution if non-diagonal pressures are used but the structure "
+                        + "is not triclinic from the start of the calculation."
                     )
         return structure
 
     def _get_rotation_matrix(self, pressure):
         """
 
         Args:
@@ -1241,23 +1124,19 @@
 
         """
         if self.structure is not None:
             if self._prism is None:
                 self._prism = UnfoldingPrism(self.structure.cell)
 
             self.structure = self._modify_structure_to_allow_requested_deformation(
-                pressure=pressure,
-                structure=self.structure,
-                prism=self._prism
+                pressure=pressure, structure=self.structure, prism=self._prism
             )
             rotation_matrix = self._prism.R
         else:
-            warnings.warn(
-                "No structure set, can not validate the simulation cell!"
-            )
+            warnings.warn("No structure set, can not validate the simulation cell!")
             rotation_matrix = None
         return rotation_matrix
 
 
 class Input:
     def __init__(self):
         self.control = LammpsControl()
@@ -1302,46 +1181,7 @@
 
         """
         with hdf5.open("input") as hdf5_input:
             self.control.from_hdf(hdf5_input)
             self.potential.from_hdf(hdf5_input)
             if "bond_dict" in hdf5_input.list_nodes():
                 self.bond_dict = hdf5_input["bond_dict"]
-
-
-def to_amat(l_list):
-    """
-
-    Args:
-        l_list:
-
-    Returns:
-
-    """
-    lst = np.reshape(l_list, -1)
-    if len(lst) == 9:
-        xlo_bound, xhi_bound, xy, ylo_bound, yhi_bound, xz, zlo_bound, zhi_bound, yz = (
-            lst
-        )
-
-    elif len(lst) == 6:
-        xlo_bound, xhi_bound, ylo_bound, yhi_bound, zlo_bound, zhi_bound = lst
-        xy, xz, yz = 0.0, 0.0, 0.0
-    else:
-        raise ValueError("This format for amat not yet implemented: " + str(len(lst)))
-
-    # > xhi_bound - xlo_bound = xhi -xlo  + MAX(0.0, xy, xz, xy + xz) - MIN(0.0, xy, xz, xy + xz)
-    # > xhili = xhi -xlo   = xhi_bound - xlo_bound - MAX(0.0, xy, xz, xy + xz) + MIN(0.0, xy, xz, xy + xz)
-    xhilo = (
-        (xhi_bound - xlo_bound)
-        - max([0.0, xy, xz, xy + xz])
-        + min([0.0, xy, xz, xy + xz])
-    )
-
-    # > yhilo = yhi -ylo = yhi_bound -ylo_bound - MAX(0.0, yz) + MIN(0.0, yz)
-    yhilo = (yhi_bound - ylo_bound) - max([0.0, yz]) + min([0.0, yz])
-
-    # > zhi - zlo = zhi_bound- zlo_bound
-    zhilo = zhi_bound - zlo_bound
-
-    cell = [[xhilo, 0, 0], [xy, yhilo, 0], [xz, yz, zhilo]]
-    return cell
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/control.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/control.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,119 +3,29 @@
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from __future__ import print_function
 from collections import OrderedDict
 import hashlib
 import numpy as np
 import warnings
-from pyiron_base import GenericParameters
-import scipy.constants as spc
+from pyiron_base import GenericParameters, state
+from pyiron_atomistics.lammps.units import LAMMPS_UNIT_CONVERSIONS
 
 __author__ = "Joerg Neugebauer, Sudarsan Surendralal, Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Sudarsan Surendralal"
 __email__ = "surendralal@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 
-# Conversion factors for transfroming pyiron units to Lammps units (alphabetical)
-AMU_TO_G = spc.atomic_mass * spc.kilo
-AMU_TO_KG = spc.atomic_mass
-ANG_PER_FS_TO_ANG_PER_PS = spc.pico / spc.femto
-ANG_PER_FS_TO_BOHR_PER_FS = spc.angstrom / spc.physical_constants['Bohr radius'][0]
-ANG_PER_FS_TO_CM_PER_S = (spc.angstrom / spc.femto) / spc.centi
-ANG_PER_FS_TO_M_PER_S = spc.angstrom / spc.femto
-ANG_TO_BOHR = spc.angstrom / spc.physical_constants['Bohr radius'][0]
-ANG_TO_CM = spc.angstrom / spc.centi
-ANG_TO_M = spc.angstrom
-EL_TO_COUL = spc.elementary_charge
-EV_PER_ANG_TO_DYNE = (spc.electron_volt / spc.angstrom) / spc.dyne
-EV_PER_ANG_TO_HA_PER_BOHR = spc.physical_constants["electron volt-hartree relationship"][0] * \
-                            spc.physical_constants['Bohr radius'][0] / spc.angstrom
-EV_PER_ANG_TO_KCAL_PER_MOL_ANG = spc.eV / (spc.kilo * spc.calorie / spc.N_A)
-EV_PER_ANG_TO_N = spc.electron_volt / spc.angstrom
-EV_TO_ERG = spc.electron_volt / spc.erg
-EV_TO_HA = spc.physical_constants["electron volt-hartree relationship"][0]
-EV_TO_J = spc.electron_volt
-EV_TO_KCAL_PER_MOL = spc.eV / (spc.kilo * spc.calorie / spc.N_A)
-FS_TO_PS = spc.femto / spc.pico
-FS_TO_S = spc.femto
-GPA_TO_ATM = spc.giga / spc.atm
-GPA_TO_BAR = spc.giga / spc.bar
-GPA_TO_BARYE = spc.giga / (spc.micro * spc.bar)  # "barye" = 1e-6 bar
-GPA_TO_PA = spc.giga
-
-# Conversions for most of the Lammps units to Pyiron units
-# Lammps units source doc: https://lammps.sandia.gov/doc/units.html
-# Pyrion units source doc: https://pyiron.readthedocs.io/en/latest/source/faq.html
-# At time of writing, not all these conversion factors are used, but may be helpful later.
-LAMMPS_UNIT_CONVERSIONS = {
-    "metal": {
-        "mass": 1.,
-        "distance": 1.,
-        "time": FS_TO_PS,
-        "energy": 1.,
-        "velocity": ANG_PER_FS_TO_ANG_PER_PS,
-        "force": 1.,
-        "temperature": 1.,
-        "pressure": GPA_TO_BAR,
-        "charge": 1.
-    },
-    "si": {
-        "mass": AMU_TO_KG,
-        "distance": ANG_TO_M,
-        "time": FS_TO_S,
-        "energy": EV_TO_J,
-        "velocity": ANG_PER_FS_TO_M_PER_S,
-        "force": EV_PER_ANG_TO_N,
-        "temperature": 1.,
-        "pressure": GPA_TO_PA,
-        "charge": EL_TO_COUL
-    },
-    "cgs": {
-        "mass": AMU_TO_G,
-        "distance": ANG_TO_CM,
-        "time": FS_TO_S,
-        "energy": EV_TO_ERG,
-        "velocity": ANG_PER_FS_TO_CM_PER_S,
-        "force": EV_PER_ANG_TO_DYNE,
-        "temperature": 1.,
-        "pressure": GPA_TO_BARYE,
-        "charge": 4.8032044e-10  # In statCoulombs, but these are deprecated and thus not in scipt.constants
-    },
-    "real": {
-        "mass": 1.,
-        "distance": 1.,
-        "time": 1.,
-        "energy": EV_TO_KCAL_PER_MOL,
-        "velocity": 1.,
-        "force": EV_PER_ANG_TO_KCAL_PER_MOL_ANG,
-        "temperature": 1.,
-        "pressure": GPA_TO_ATM,
-        "charge": 1.
-    },
-    "electron": {
-        "mass": 1.,
-        "distance": ANG_TO_BOHR,
-        "time": 1.,
-        "energy": EV_TO_HA,
-        "velocity": ANG_PER_FS_TO_BOHR_PER_FS,
-        "force": EV_PER_ANG_TO_HA_PER_BOHR,
-        "temperature": 1.,
-        "pressure": GPA_TO_PA,
-        "charge": 1.
-    },
-}
-
-
 class LammpsControl(GenericParameters):
     def __init__(self, input_file_name=None, **qwargs):
         super(LammpsControl, self).__init__(
             input_file_name=input_file_name, table_name="control_inp", comment_char="#"
         )
         self._init_block_dict()
         self._force_skewed = False
@@ -185,15 +95,15 @@
                 + "atom_style            atomic\n"
                 + "read_data             structure.inp\n"
                 + "include               potential.inp\n"
                 + "fix___ensemble        all nve\n"
                 + "variable___dumptime   equal 100\n"
                 + "variable___thermotime equal 100\n"
                 + "dump___1              all custom ${dumptime} dump.out id type xsu ysu zsu fx fy fz vx vy vz\n"
-                + "dump_modify___1       sort id format line \"%d %d %20.15g %20.15g %20.15g %20.15g %20.15g %20.15g %20.15g %20.15g %20.15g\"\n"
+                + 'dump_modify___1       sort id format line "%d %d %20.15g %20.15g %20.15g %20.15g %20.15g %20.15g %20.15g %20.15g %20.15g"\n'
                 + "thermo_style          custom step temp pe etotal pxx pxy pxz pyy pyz pzz vol\n"
                 + "thermo_modify         format float %20.15g\n"
                 + "thermo                ${thermotime}\n"
                 + "run                   0\n"
             )
         self.load_string(file_content)
 
@@ -224,63 +134,76 @@
 
         # If pressure is a scalar, only unit conversion is needed.
         if np.isscalar(pressure):
             return float(pressure) * LAMMPS_UNIT_CONVERSIONS[self["units"]]["pressure"]
 
         # Normalize pressure to a list of 6 entries of either float or NoneType type.
         if len(pressure) > 6:
-            raise ValueError("Pressure can have a maximum of 6 values, (x, y, z, xy, xz, and yz), but got " +
-                             "{}".format(len(pressure)))
-        pressure = [float(p) if p is not None else None
-                    for p in pressure]
+            raise ValueError(
+                "Pressure can have a maximum of 6 values, (x, y, z, xy, xz, and yz), but got "
+                + "{}".format(len(pressure))
+            )
+        pressure = [float(p) if p is not None else None for p in pressure]
         pressure += (6 - len(pressure)) * [None]
 
         if all(p is None for p in pressure):
             raise ValueError("Pressure cannot have a length but all be None")
 
         # If necessary, rotate the pressure tensor to the Lammps coordinate frame.
         # Isotropic, hydrostatic pressures are rotation invariant.
-        if not np.isclose(np.matrix.trace(rotation_matrix), 3) and not self._is_isotropic_hydrostatic(pressure):
+        if not np.isclose(
+            np.matrix.trace(rotation_matrix), 3
+        ) and not self._is_isotropic_hydrostatic(pressure):
             if any(p is None for p in pressure):
-                raise ValueError("Cells which are not orthorhombic or an upper-triangular cell are incompatible with Lammps "
-                                 "constant pressure calculations unless the entire pressure tensor is defined. "
-                                 "The reason is that Lammps demands such cells be represented with an "
-                                 "upper-triangular unit cell, thus a rotation between Lammps and pyiron coordinate "
-                                 "frames is required; it is not possible to rotate the pressure tensor if any of "
-                                 "its components is None.")
+                raise ValueError(
+                    "Cells which are not orthorhombic or an upper-triangular cell are incompatible with Lammps "
+                    "constant pressure calculations unless the entire pressure tensor is defined. "
+                    "The reason is that Lammps demands such cells be represented with an "
+                    "upper-triangular unit cell, thus a rotation between Lammps and pyiron coordinate "
+                    "frames is required; it is not possible to rotate the pressure tensor if any of "
+                    "its components is None."
+                )
             pxx, pyy, pzz, pxy, pxz, pyz = pressure
             pressure_tensor = np.array(
-                [[pxx, pxy, pxz],
-                 [pxy, pyy, pyz],
-                 [pxz, pyz, pzz]]
-            )
-            lammps_pressure_tensor = rotation_matrix.T @ pressure_tensor @ rotation_matrix
-            pressure = list(lammps_pressure_tensor[[0, 1, 2, 0, 0, 1], [0, 1, 2, 1, 2, 2]])
-
-        return [(p * LAMMPS_UNIT_CONVERSIONS[self["units"]]["pressure"]
-                 if p is not None
-                 else p)
-                for p in pressure]
+                [[pxx, pxy, pxz], [pxy, pyy, pyz], [pxz, pyz, pzz]]
+            )
+            lammps_pressure_tensor = (
+                rotation_matrix.T @ pressure_tensor @ rotation_matrix
+            )
+            pressure = list(
+                lammps_pressure_tensor[[0, 1, 2, 0, 0, 1], [0, 1, 2, 1, 2, 2]]
+            )
+
+        return [
+            (
+                p * LAMMPS_UNIT_CONVERSIONS[self["units"]]["pressure"]
+                if p is not None
+                else p
+            )
+            for p in pressure
+        ]
 
     @staticmethod
     def _is_isotropic_hydrostatic(pressure):
-        axial_all_alike = None not in pressure[:3] and np.allclose(pressure[:3], pressure[0])
+        axial_all_alike = None not in pressure[:3] and np.allclose(
+            pressure[:3], pressure[0]
+        )
         shear_all_none = all(p is None for p in pressure[3:])
         shear_all_zero = None not in pressure[3:] and np.allclose(pressure[3:], 0)
         return axial_all_alike and (shear_all_none or shear_all_zero)
 
     def calc_minimize(
         self,
         ionic_energy_tolerance=0.0,
         ionic_force_tolerance=1e-4,
         max_iter=100000,
         pressure=None,
         n_print=100,
-        style='cg',
-        rotation_matrix=None
+        style="cg",
+        rotation_matrix=None,
     ):
         """
         Sets parameters required for minimization.
 
         Args:
             ionic_energy_tolerance (float): If the magnitude of difference between energies of two consecutive steps is
                 lower than or equal to `ionic_energy_tolerance`, the minimisation terminates. (Default is 0.0 eV.)
@@ -304,34 +227,46 @@
             rotation_matrix (numpy.ndarray): The rotation matrix from the pyiron to Lammps coordinate frame.
         """
         # This docstring is a source for the calc_minimize method in pyiron_atomistics.lammps.base.LammpsBase.calc_minimize and
         # pyiron_atomistics.lammps.interactive.LammpsInteractive.calc_minimize -- Please ensure that changes to signature or
         # defaults stay consistent!
 
         max_evaluations = 100 * max_iter
+        if n_print > max_iter:
+            state.logger.warning(
+                "n_print larger than max_iter, adjusting to n_print=max_iter"
+            )
+            n_print = max_iter
 
         if self["units"] not in LAMMPS_UNIT_CONVERSIONS.keys():
             raise NotImplementedError
         energy_units = LAMMPS_UNIT_CONVERSIONS[self["units"]]["energy"]
         force_units = LAMMPS_UNIT_CONVERSIONS[self["units"]]["force"]
 
         ionic_energy_tolerance *= energy_units
         ionic_force_tolerance *= force_units
 
         if pressure is not None:
+            if rotation_matrix is None:
+                raise ValueError(
+                    "No rotation matrix given while trying to convert pressure. "
+                    "This is most likely due to no structure being defined."
+                )
             self._force_skewed = False
             pressure = self.pressure_to_lammps(pressure, rotation_matrix)
             if np.isscalar(pressure):
                 str_press = " iso {}".format(pressure)
             else:
                 str_press = ""
-                for ii, (press, str_axis) in enumerate(zip(pressure, ["x","y","z","xy","xz","yz"])):
+                for ii, (press, str_axis) in enumerate(
+                    zip(pressure, ["x", "y", "z", "xy", "xz", "yz"])
+                ):
                     if press is not None:
-                        str_press += ' {} {}'.format(str_axis, press)
-                        if ii>2:
+                        str_press += " {} {}".format(str_axis, press)
+                        if ii > 2:
                             self._force_skewed = True
                 if len(str_press) > 1:
                     str_press += " couple none"
             self.set(fix___ensemble=r"all box/relax" + str_press)
         self.remove_keys(["fix___nve"])
         self.set(min_style=style)
         self.set(
@@ -342,15 +277,15 @@
             + str(int(max_iter))
             + " "
             + str(int(max_evaluations))
         )
         self.remove_keys(["run", "velocity"])
         self.modify(
             variable___dumptime="equal " + str(n_print),
-            variable___thermotime="equal " + str(n_print)
+            variable___thermotime="equal " + str(n_print),
         )
 
     def calc_static(self):
         self.set(run="0")
         self.remove_keys(["minimize", "velocity"])
 
     def set_initial_velocity(
@@ -423,15 +358,15 @@
         seed=None,
         tloop=None,
         initial_temperature=None,
         langevin=False,
         delta_temp=None,
         delta_press=None,
         job_name="",
-        rotation_matrix=None
+        rotation_matrix=None,
     ):
         """
         Set an MD calculation within LAMMPS. Nosé Hoover is used by default.
 
         Args:
             temperature (None/float/list): Target temperature value(-s). If set to None, an NVE
                 calculation is performed. It is required when the pressure is set or langevin is set
@@ -501,50 +436,58 @@
             pressure_damping_timescale = delta_press
         else:
             pressure_damping_timescale *= time_units
 
         # Transform temperature
         if temperature is not None:
             temperature = np.array([temperature], dtype=float).flatten()
-            if len(temperature)==1:
-                temperature = np.array(2*temperature.tolist())
+            if len(temperature) == 1:
+                temperature = np.array(2 * temperature.tolist())
             elif len(temperature) != 2:
-                raise ValueError("At most two temperatures can be provided "
-                                 "(for a linearly ramping target temperature), "
-                                 "but got {}".format(len(temperature)))
+                raise ValueError(
+                    "At most two temperatures can be provided "
+                    "(for a linearly ramping target temperature), "
+                    "but got {}".format(len(temperature))
+                )
             temperature *= temperature_units
 
         # Apply initial overheating (default uses the theorem of equipartition of energy between KE and PE)
         if initial_temperature is None and temperature is not None:
             initial_temperature = 2 * temperature[0]
 
         if seed is None:
             seed = self.generate_seed_from_job(job_name=job_name)
         if seed <= 0:
             raise ValueError("Seed must be a positive integer larger than 0")
-            
+
         # Set thermodynamic ensemble
         if pressure is not None:  # NPT
             if temperature is None or temperature.min() <= 0:
-                raise ValueError("Target temperature for fix nvt/npt/nph cannot be 0 or negative")
+                raise ValueError(
+                    "Target temperature for fix nvt/npt/nph cannot be 0 or negative"
+                )
 
             self._force_skewed = False
             pressure = self.pressure_to_lammps(pressure, rotation_matrix)
 
             if np.isscalar(pressure):
-                pressure_string = " iso {0} {0} {1}".format(pressure, pressure_damping_timescale)
+                pressure_string = " iso {0} {0} {1}".format(
+                    pressure, pressure_damping_timescale
+                )
             else:
                 pressure_string = ""
-                for ii, (coord, value) in enumerate(zip(["x", "y", "z", "xy", "xz", "yz"], pressure)):
+                for ii, (coord, value) in enumerate(
+                    zip(["x", "y", "z", "xy", "xz", "yz"], pressure)
+                ):
                     if value is not None:
                         pressure_string += " {0} {1} {1} {2}".format(
                             coord, value, pressure_damping_timescale
                         )
-                    if ii > 2:
-                        self._force_skewed = True
+                        if ii > 2:
+                            self._force_skewed = True
 
             if langevin:  # NPT(Langevin)
                 fix_ensemble_str = "all nph" + pressure_string
                 self.modify(
                     fix___langevin="all langevin {0} {1} {2} {3} zero yes".format(
                         str(temperature[0]),
                         str(temperature[1]),
@@ -558,15 +501,17 @@
                     str(temperature[0]),
                     str(temperature[1]),
                     str(temperature_damping_timescale),
                 )
                 fix_ensemble_str += pressure_string
         elif temperature is not None:  # NVT
             if temperature.min() <= 0:
-                raise ValueError("Target temperature for fix nvt/npt/nph cannot be 0 or negative")
+                raise ValueError(
+                    "Target temperature for fix nvt/npt/nph cannot be 0 or negative"
+                )
 
             if langevin:  # NVT(Langevin)
                 fix_ensemble_str = "all nve"
                 self.modify(
                     fix___langevin="all langevin {0} {1} {2} {3} zero yes".format(
                         str(temperature[0]),
                         str(temperature[1]),
@@ -581,42 +526,41 @@
                     str(temperature[1]),
                     str(temperature_damping_timescale),
                 )
         else:  # NVE
             if langevin:
                 warnings.warn("Temperature not set; Langevin ignored.")
             fix_ensemble_str = "all nve"
-            initial_temperature = 0
 
         if tloop is not None:
             fix_ensemble_str += " tloop " + str(tloop)
 
         self.remove_keys(["minimize"])
         self.modify(
             fix___ensemble=fix_ensemble_str,
             variable___dumptime=" equal {} ".format(n_print),
             variable___thermotime=" equal {} ".format(n_print),
             run=int(n_ionic_steps),
             append_if_not_present=True,
         )
 
-        if initial_temperature > 0:
+        if initial_temperature is not None and initial_temperature > 0:
             self.set_initial_velocity(
                 temperature=initial_temperature,
                 seed=seed,
                 gaussian=True,
-                job_name=job_name
+                job_name=job_name,
             )
 
     def calc_vcsgc(
         self,
         mu,
         ordered_element_list,
         target_concentration=None,
-        kappa=1000.,
+        kappa=1000.0,
         mc_step_interval=100,
         swap_fraction=0.1,
         temperature_mc=None,
         window_size=None,
         window_moves=None,
         temperature=None,
         pressure=None,
@@ -625,15 +569,15 @@
         n_print=100,
         temperature_damping_timescale=100.0,
         pressure_damping_timescale=1000.0,
         seed=None,
         initial_temperature=None,
         langevin=False,
         job_name="",
-        rotation_matrix=None
+        rotation_matrix=None,
     ):
         """
         Run variance-constrained semi-grand-canonical MD/MC for a binary system. In addition to VC-SGC arguments, all
         arguments for a regular MD calculation are also accepted.
 
         https://vcsgc-lammps.materialsmodeling.org
 
@@ -678,15 +622,15 @@
             temperature_damping_timescale=temperature_damping_timescale,
             pressure_damping_timescale=pressure_damping_timescale,
             seed=seed,
             tloop=None,
             initial_temperature=initial_temperature,
             langevin=langevin,
             job_name=job_name,
-            rotation_matrix=rotation_matrix
+            rotation_matrix=rotation_matrix,
         )
 
         if self["units"] not in LAMMPS_UNIT_CONVERSIONS.keys():
             raise NotImplementedError
         temperature_units = LAMMPS_UNIT_CONVERSIONS[self["units"]]["temperature"]
         energy_units = LAMMPS_UNIT_CONVERSIONS[self["units"]]["energy"]
 
@@ -695,137 +639,181 @@
                 raise ValueError("If temperature is not given, temperature_mc must be.")
             temperature_mc = temperature * temperature_units
 
         if seed is None:
             seed = self.generate_seed_from_job(job_name=job_name)
 
         if set(mu.keys()) != set(ordered_element_list):
-            raise ValueError("Exactly one chemical potential must be given for each element treated by the potential.")
+            raise ValueError(
+                "Exactly one chemical potential must be given for each element treated by the potential."
+            )
 
         calibrating_el = ordered_element_list[0]
         # Apply the actual SGC string
         fix_vcsgc_str = "all sgcmc {0} {1} {2} {3} randseed {4}".format(
             str(mc_step_interval),
             str(swap_fraction),
             str(temperature_mc),
-            str(" ".join(str((mu[el] - mu[calibrating_el]) * energy_units) for el in ordered_element_list[1:])),
+            str(
+                " ".join(
+                    str((mu[el] - mu[calibrating_el]) * energy_units)
+                    for el in ordered_element_list[1:]
+                )
+            ),
             str(seed),
         )
 
         # Add VC to the SGC if target concentrations were provided
         if target_concentration is not None:
             if set(target_concentration.keys()) != set(ordered_element_list):
-                raise ValueError("Exactly one target concentration must be given for each element treated by the "
-                                 "potential.")
+                raise ValueError(
+                    "Exactly one target concentration must be given for each element treated by the "
+                    "potential."
+                )
 
             if not np.isclose(np.sum([v for _, v in target_concentration.items()]), 1):
-                raise ValueError("Target concentrations must sum to 1 but were {}.".format(
-                    np.sum([v for _, v in target_concentration.items()])
-                ))
+                raise ValueError(
+                    "Target concentrations must sum to 1 but were {}.".format(
+                        np.sum([v for _, v in target_concentration.items()])
+                    )
+                )
 
             fix_vcsgc_str += " variance {0} {1}".format(
                 str(kappa),
-                str(" ".join([str(target_concentration[el]) for el in ordered_element_list[1:]]))
+                str(
+                    " ".join(
+                        [
+                            str(target_concentration[el])
+                            for el in ordered_element_list[1:]
+                        ]
+                    )
+                ),
             )
 
         # Set optional windowing parameters
         if window_moves is not None:
             if int(window_moves) != window_moves or window_moves < 0:
                 raise ValueError("Window moves must be a non-negative integer.")
             fix_vcsgc_str += " window_moves {0}".format(window_moves)
         if window_size is not None:
             if not 0.5 <= window_size <= 1.0:
                 raise ValueError("Window size must be a fraction between 0.5 and 1")
             fix_vcsgc_str += " window_size {0}".format(window_size)
 
-        self.modify(
-            fix___vcsgc=fix_vcsgc_str,
-            append_if_not_present=True
-        )
+        self.modify(fix___vcsgc=fix_vcsgc_str, append_if_not_present=True)
 
     def measure_mean_value(self, key, every=1, repeat=None, name=None, atom=False):
         """
-            Args:
-                key (str): property to take an average value of (e.g. 'energy_pot' v.i.)
-                every (int): number of steps there should be between two measurements
-                repeat (int): number of measurements for each output (default: n_print/every)
-                name (str): name to give in the output string (ignored if a pyiron predefined tag is used)
-
-            Comments:
-                Currently available keys: 'energy_pot', 'energy_tot', 'temperature', 'volume',
-                                          'pressures', 'positions', 'forces, 'velocities'
-                Future keys: 'cells'
+        Args:
+            key (str): property to take an average value of (e.g. 'energy_pot' v.i.)
+            every (int): number of steps there should be between two measurements
+            repeat (int): number of measurements for each output (default: n_print/every)
+            name (str): name to give in the output string (ignored if a pyiron predefined tag is used)
+
+        Comments:
+            Currently available keys: 'energy_pot', 'energy_tot', 'temperature', 'volume',
+                                      'pressures', 'positions', 'forces, 'velocities'
+            Future keys: 'cells'
         """
 
-        if every<=0:
-            raise AssertionError('every must be a positive integer')
+        if every <= 0:
+            raise AssertionError("every must be a positive integer")
         if repeat is None:
-            self['variable___mean_repeat_times'] = 'equal round(${thermotime}/'+str(every)+')'
+            self["variable___mean_repeat_times"] = (
+                "equal round(${thermotime}/" + str(every) + ")"
+            )
         else:
-            self['variable___mean_repeat_times'] = 'equal {}'.format(repeat)
-        if key=='energy_pot':
-            self._measure_mean_value('energy_pot', 'pe', every)
-        elif key=='energy_tot':
-            self._measure_mean_value('energy_tot', 'etotal', every)
-        elif key=='temperature':
-            self._measure_mean_value('temperature', 'temp', every)
-        elif key=='volume':
-            self._measure_mean_value('volume', 'vol', every)
-        elif key=='pressures':
-            self._measure_mean_value('pressure', ['pxx', 'pyy', 'pzz', 'pxy', 'pxz', 'pyz'], every)
-        elif key=='positions':
-            self['compute___unwrap'] = 'all property/atom xu yu zu'
-            self['fix___mean_positions'] = ('all ave/atom '
-                                            +str(every)
-                                            +' ${mean_repeat_times} ${thermotime} c_unwrap[*]'
-                                           )
-            self['dump___1'] = self['dump___1']+' '+' '.join(['f_mean_positions[{}]'.format(ii+1) for ii in range(3)])
-            self['dump_modify___1'] = self['dump_modify___1'][:-1]+' '+' '.join(['%20.15g']*3)+'"'
-        elif key=='forces':
-            self._measure_mean_value('forces', ['fx', 'fy', 'fz'], every, atom=True)
-        elif key=='velocities':
-            self._measure_mean_value('velocities', ['vx', 'vy', 'vz'], every, atom=True)
+            self["variable___mean_repeat_times"] = "equal {}".format(repeat)
+        if key == "energy_pot":
+            self._measure_mean_value("energy_pot", "pe", every)
+        elif key == "energy_tot":
+            self._measure_mean_value("energy_tot", "etotal", every)
+        elif key == "temperature":
+            self._measure_mean_value("temperature", "temp", every)
+        elif key == "volume":
+            self._measure_mean_value("volume", "vol", every)
+        elif key == "pressures":
+            self._measure_mean_value(
+                "pressure", ["pxx", "pyy", "pzz", "pxy", "pxz", "pyz"], every
+            )
+        elif key == "positions":
+            self["compute___unwrap"] = "all property/atom xu yu zu"
+            self["fix___mean_positions"] = (
+                "all ave/atom "
+                + str(every)
+                + " ${mean_repeat_times} ${thermotime} c_unwrap[*]"
+            )
+            self["dump___1"] = (
+                self["dump___1"]
+                + " "
+                + " ".join(["f_mean_positions[{}]".format(ii + 1) for ii in range(3)])
+            )
+            self["dump_modify___1"] = (
+                self["dump_modify___1"][:-1] + " " + " ".join(["%20.15g"] * 3) + '"'
+            )
+        elif key == "forces":
+            self._measure_mean_value("forces", ["fx", "fy", "fz"], every, atom=True)
+        elif key == "velocities":
+            self._measure_mean_value("velocities", ["vx", "vy", "vz"], every, atom=True)
         elif name is not None:
-            if '**' in key:
-                warnings.warn('** is replaced by ^ (as it is understood by LAMMPS)')
-                key = key.replace('**', '^')
+            if "**" in key:
+                warnings.warn("** is replaced by ^ (as it is understood by LAMMPS)")
+                key = key.replace("**", "^")
             self._measure_mean_value(name, key, every, atom)
         else:
-            raise NotImplementedError(key+' is not implemented')
+            raise NotImplementedError(key + " is not implemented")
 
     def energy_pot_per_atom(self):
-        if self['compute___energy_pot_per_atom'] is None:
-            self['compute___energy_pot_per_atom'] = 'all pe/atom'
-            self['dump___1'] += ' c_energy_pot_per_atom'
-            self['dump_modify___1'] = self['dump_modify___1'][:-1] + ' %20.15g"'
+        """
+        Enable the output of atomic energies.  This will add an additional key 'energy_pot_per_atom' to the HDF output.
+        """
+        if self["compute___energy_pot_per_atom"] is None:
+            self["compute___energy_pot_per_atom"] = "all pe/atom"
+            self["dump___1"] += " c_energy_pot_per_atom"
+            self["dump_modify___1"] = self["dump_modify___1"][:-1] + ' %20.15g"'
 
     def _set_group_by_id(self, group_name, ids):
         if len(ids) < 1:
-            raise ValueError('Group ids must have at least length one, but got {}'.format(ids))
-        if np.any([isinstance(id_, bool) or not isinstance(id_, (int, np.integer)) for id_ in ids]):
+            raise ValueError(
+                "Group ids must have at least length one, but got {}".format(ids)
+            )
+        if np.any(
+            [
+                isinstance(id_, bool) or not isinstance(id_, (int, np.integer))
+                for id_ in ids
+            ]
+        ):
             # Note: it turns out bool is a subclass of int. Weird, eh.
-            raise TypeError('Group ids must be integers, but got {}'.format(ids))
+            raise TypeError("Group ids must be integers, but got {}".format(ids))
         if np.any(np.array(ids) < 0):
-            raise ValueError('Group ids must be non-negative to be parsed by Lammps, but got {}'.format(ids))
-        self['group___{}'.format(group_name)] = 'id {}'.format(' '.join(np.array(ids).astype(int).astype(str)))
+            raise ValueError(
+                "Group ids must be non-negative to be parsed by Lammps, but got {}".format(
+                    ids
+                )
+            )
+        self["group___{}".format(group_name)] = "id {}".format(
+            " ".join(np.array(ids).astype(int).astype(str))
+        )
 
     def _fix_with_three_vector(self, ids, vector, fix_string, conversion):
         if len(vector) != 3:
-            raise ValueError('{} must have three components, but got {}'.format(fix_string, vector))
+            raise ValueError(
+                "{} must have three components, but got {}".format(fix_string, vector)
+            )
         vector = list(vector)
         for i, v in enumerate(vector):
             if v is None:
-                vector[i] = 'NULL'
+                vector[i] = "NULL"
             else:
                 vector[i] = str(v * conversion)
-        name = str(hash(tuple(ids))).replace('-', 'm')  # A unique name for the group
+        name = str(hash(tuple(ids))).replace("-", "m")  # A unique name for the group
         self._set_group_by_id(name, ids)
-        self['fix___{}_{}'.format(fix_string.replace(' ', '_'), name)] = '{} {} {}'.format(
-            name, fix_string, ' '.join(vector)
-        )
+        self[
+            "fix___{}_{}".format(fix_string.replace(" ", "_"), name)
+        ] = "{} {} {}".format(name, fix_string, " ".join(vector))
 
     def fix_move_linear_by_id(self, ids, velocity):
         """
         Displace atoms at each timestep. Creates a new group with a unique name based off the hash of the ids.
 
         Args:
             ids (list/numpy.ndarray): Integer ids of the atoms to move in the job's structure.
@@ -834,68 +822,124 @@
 
         Warning: This fix does not exclude these atoms from [other fixes](https://lammps.sandia.gov/doc/fix_move.html).
             You may wish to combine this call with `selective_dynamics` on your corresponding structure. Future
             developers can find a more complete discussion [here](https://github.com/pyiron/pyiron/pull/1212) when
             further modifying this capability. Further, it will malfunction if the Lammps coordinate frame and pyiron
             coordinate frame differ.
         """
-        warnings.warn('This fix does not exclude these atoms from other fixes. You may wish to combine this call with '
-                      '`selective_dynamics` on your corresponding structure. Further, it will malfunction if the '
-                      'Lammps coordinate frame and pyiron coordinate frame differ.')
-        self._fix_with_three_vector(ids, velocity, 'move linear', LAMMPS_UNIT_CONVERSIONS[self["units"]]["velocity"])
+        warnings.warn(
+            "This fix does not exclude these atoms from other fixes. You may wish to combine this call with "
+            "`selective_dynamics` on your corresponding structure. Further, it will malfunction if the "
+            "Lammps coordinate frame and pyiron coordinate frame differ."
+        )
+        self._fix_with_three_vector(
+            ids,
+            velocity,
+            "move linear",
+            LAMMPS_UNIT_CONVERSIONS[self["units"]]["velocity"],
+        )
 
     def fix_setforce_by_id(self, ids, force):
         """
         Set the force on a collection of atoms to a specified value.
 
         ids (list/numpy.ndarray): Integer ids of the atoms to move in the job's structure.
         force (list/numpy.ndarray/tuple): The force in x-y-z-direction for the group. `None` arguments are
             converted to Lammps 'NULL' values and the force in this direction is left unchanged.
 
         Warning: This fix will malfunction (silently) if the Lammps coordinate frame and pyiron coordinate frame differ.
         """
-        warnings.warn('This fix will malfunction (silently) if the Lammps coordinate frame and pyiron coordinate frame '
-                      'differ.')
-        self._fix_with_three_vector(ids, force, 'setforce', LAMMPS_UNIT_CONVERSIONS[self["units"]]["force"])
+        warnings.warn(
+            "This fix will malfunction (silently) if the Lammps coordinate frame and pyiron coordinate frame "
+            "differ."
+        )
+        self._fix_with_three_vector(
+            ids, force, "setforce", LAMMPS_UNIT_CONVERSIONS[self["units"]]["force"]
+        )
 
     def _measure_mean_value(self, key_pyiron, key_lmp, every, atom=False):
         """
-            Args:
-                key (str): property to take an average value of (e.g. 'energy_pot' v.i.)
-                every (int): number of steps there should be between two measurements
-                repeat (int): number of measurements for each output (default: n_print/every)
-                freq (int): output frequency (default: n_print)
-
-            Comments:
-                Currently available keys: 'energy_pot', 'energy_tot', 'temperature', 'volume',
-                                          'pressures', 'psitions', 'forces, 'velocities'
-                Future keys: 'cells'
+        Args:
+            key (str): property to take an average value of (e.g. 'energy_pot' v.i.)
+            every (int): number of steps there should be between two measurements
+            repeat (int): number of measurements for each output (default: n_print/every)
+            freq (int): output frequency (default: n_print)
+
+        Comments:
+            Currently available keys: 'energy_pot', 'energy_tot', 'temperature', 'volume',
+                                      'pressures', 'psitions', 'forces, 'velocities'
+            Future keys: 'cells'
         """
         if isinstance(key_lmp, str):
-            self['variable___{}'.format(key_pyiron)] = 'equal {}'.format(key_lmp)
-            self['fix___mean_{}'.format(key_pyiron)] = ('all ave/time '
-                                                        +str(every)
-                                                        +' ${mean_repeat_times} ${thermotime} v_'
-                                                        +str(key_pyiron))
-            self['thermo_style'] = self['thermo_style']+' f_mean_{}'.format(key_pyiron)
+            self["variable___{}".format(key_pyiron)] = "equal {}".format(key_lmp)
+            self["fix___mean_{}".format(key_pyiron)] = (
+                "all ave/time "
+                + str(every)
+                + " ${mean_repeat_times} ${thermotime} v_"
+                + str(key_pyiron)
+            )
+            self["thermo_style"] = self["thermo_style"] + " f_mean_{}".format(
+                key_pyiron
+            )
         else:
             if atom is True:
                 for ii, _ in enumerate(key_lmp):
-                    self['variable___{}_{}'.format(key_pyiron, ii)] = 'atom {}'.format(key_lmp[ii])
-                self['fix___mean_{}'.format(key_pyiron)] = ('all ave/atom '
-                                                            +str(every)+
-                                                            ' ${mean_repeat_times} ${thermotime} '
-                                                            +str(' '.join(['v_{}_{}'.format(key_pyiron, ii) for ii in range(len(key_lmp))]))
-                                                           )
-                self['dump___1'] = self['dump___1']+' '+' '.join(['f_mean_{}[{}]'.format(key_pyiron, ii+1) for ii in range(len(key_lmp))])
-                self['dump_modify___1'] = self['dump_modify___1'][:-1]+' '+' '.join(['%20.15g']*len(key_lmp))+'"'
+                    self["variable___{}_{}".format(key_pyiron, ii)] = "atom {}".format(
+                        key_lmp[ii]
+                    )
+                self["fix___mean_{}".format(key_pyiron)] = (
+                    "all ave/atom "
+                    + str(every)
+                    + " ${mean_repeat_times} ${thermotime} "
+                    + str(
+                        " ".join(
+                            [
+                                "v_{}_{}".format(key_pyiron, ii)
+                                for ii in range(len(key_lmp))
+                            ]
+                        )
+                    )
+                )
+                self["dump___1"] = (
+                    self["dump___1"]
+                    + " "
+                    + " ".join(
+                        [
+                            "f_mean_{}[{}]".format(key_pyiron, ii + 1)
+                            for ii in range(len(key_lmp))
+                        ]
+                    )
+                )
+                self["dump_modify___1"] = (
+                    self["dump_modify___1"][:-1]
+                    + " "
+                    + " ".join(["%20.15g"] * len(key_lmp))
+                    + '"'
+                )
             else:
                 for ii, _ in enumerate(key_lmp):
-                    self['variable___{}_{}'.format(key_pyiron, ii)] = 'equal {}'.format(key_lmp[ii])
-                self['fix___mean_{}'.format(key_pyiron)] = ('all ave/time '
-                                                            +str(every)
-                                                            +' ${mean_repeat_times} ${thermotime} '
-                                                            +str(' '.join(['v_{}_{}'.format(key_pyiron, ii) for ii in range(len(key_lmp))]))
-                                                           )
-                self['thermo_style'] = (self['thermo_style']
-                                        +' '
-                                        +' '.join(['f_mean_{}[{}]'.format(key_pyiron, ii+1) for ii in range(len(key_lmp))]))
+                    self["variable___{}_{}".format(key_pyiron, ii)] = "equal {}".format(
+                        key_lmp[ii]
+                    )
+                self["fix___mean_{}".format(key_pyiron)] = (
+                    "all ave/time "
+                    + str(every)
+                    + " ${mean_repeat_times} ${thermotime} "
+                    + str(
+                        " ".join(
+                            [
+                                "v_{}_{}".format(key_pyiron, ii)
+                                for ii in range(len(key_lmp))
+                            ]
+                        )
+                    )
+                )
+                self["thermo_style"] = (
+                    self["thermo_style"]
+                    + " "
+                    + " ".join(
+                        [
+                            "f_mean_{}[{}]".format(key_pyiron, ii + 1)
+                            for ii in range(len(key_lmp))
+                        ]
+                    )
+                )
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/lammps.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/sphinx.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
-from pyiron_atomistics.lammps.interactive import LammpsInteractive
+import warnings
+from pyiron_atomistics.sphinx.interactive import SphinxInteractive
 
-__author__ = "Joerg Neugebauer, Sudarsan Surendralal, Jan Janssen"
+__author__ = "Osamu Waseda, Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
-    "- Computational Materials Design (CM) Department"
+    "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
-__maintainer__ = "Sudarsan Surendralal"
-__email__ = "surendralal@mpie.de"
-__status__ = "production"
+__maintainer__ = "Jan Janssen"
+__email__ = "janssen@mpie.de"
+__status__ = "development"
 __date__ = "Sep 1, 2017"
 
 
-class Lammps(LammpsInteractive):
+class Sphinx(SphinxInteractive):
     """
-    Class to setup and run and analyze LAMMPS simulations which is a derivative of
-    atomistics.job.generic.GenericJob. The functions in these modules are written in such the function names and
-    attributes are very generic (get_structure(), molecular_dynamics(), version) but the functions are written to handle
-    LAMMPS specific input/output.
+    Class to setup and run Sphinx simulations which is a derivative of pyiron_atomistics.job.generic.GenericJob.
+    The functions in these modules are written in such the function names and attributes are very generic
+    (get_structure(), molecular_dynamics(), version) but the functions are written to handle Sphinx specific input and
+    output.
 
     Args:
-        project (pyiron_atomistics.project.Project instance):  Specifies the project path among other attributes
-        job_name (str): Name of the job
-
-    Attributes:
-        input (lammps.Input instance): Instance which handles the input
+        project: Project object (defines path where job will be created and stored)
+        job_name (str): name of the job (must be unique within this project path)
     """
 
     def __init__(self, project, job_name):
-        super(Lammps, self).__init__(project, job_name)
-        self.__name__ = "Lammps"
+        super(Sphinx, self).__init__(project, job_name)
+
+        self.__version__ = (
+            None  # Reset the version number to the executable is set automatically
+        )
         self._executable_activate(enforce=True)
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/potential.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/potential.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
-from __future__ import print_function
-from ast import literal_eval
-import numpy as np
 import pandas as pd
 import shutil
 import os
-from pyiron_base import Settings, GenericParameters
-from pyiron_atomistics.atomistics.job.potentials import PotentialAbstract, find_potential_file_base
+from pyiron_base import state, GenericParameters
+from pyiron_atomistics.atomistics.job.potentials import (
+    PotentialAbstract,
+    find_potential_file_base,
+)
+from pyiron_atomistics.atomistics.structure.atoms import Atoms
+from typing import List
 
 __author__ = "Joerg Neugebauer, Sudarsan Surendralal, Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Sudarsan Surendralal"
 __email__ = "surendralal@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
-s = Settings()
-
 
 class LammpsPotential(GenericParameters):
 
     """
     This module helps write commands which help in the control of parameters related to the potential used in LAMMPS
     simulations
     """
@@ -61,34 +61,42 @@
     def remove_structure_block(self):
         self.remove_keys(["units"])
         self.remove_keys(["atom_style"])
         self.remove_keys(["dimension"])
 
     @property
     def files(self):
-        if len(self._df["Filename"].values[0]) > 0 and self._df["Filename"].values[0] != ['']:
+        if len(self._df["Filename"].values[0]) > 0 and self._df["Filename"].values[
+            0
+        ] != [""]:
             absolute_file_paths = [
                 files for files in list(self._df["Filename"])[0] if os.path.isabs(files)
             ]
             relative_file_paths = [
                 files
                 for files in list(self._df["Filename"])[0]
                 if not os.path.isabs(files)
             ]
             env = os.environ
-            resource_path_lst = s.resource_paths
+            resource_path_lst = state.settings.resource_paths
             for conda_var in ["CONDA_PREFIX", "CONDA_DIR"]:
                 if conda_var in env.keys():  # support iprpy-data package
-                    resource_path_lst += [os.path.join(env[conda_var], "share", "iprpy")]
+                    path_to_add = state.settings.convert_path_to_abs_posix(
+                        os.path.join(env[conda_var], "share", "iprpy")
+                    )
+                    if path_to_add not in resource_path_lst:
+                        resource_path_lst.append(path_to_add)
             for path in relative_file_paths:
-                absolute_file_paths.append(find_potential_file_base(
-                    path=path,
-                    resource_path_lst=resource_path_lst,
-                    rel_path=os.path.join("lammps", "potentials")
-                ))
+                absolute_file_paths.append(
+                    find_potential_file_base(
+                        path=path,
+                        resource_path_lst=resource_path_lst,
+                        rel_path=os.path.join("lammps", "potentials"),
+                    )
+                )
             if len(absolute_file_paths) != len(list(self._df["Filename"])[0]):
                 raise ValueError("Was not able to locate the potentials.")
             else:
                 return absolute_file_paths
 
     def copy_pot_files(self, working_directory):
         if self.files is not None:
@@ -109,28 +117,27 @@
             list: words of the matching line
 
         Raises:
             ValueError: if not matching line was found
         """
 
         def isprefix(prefix, lst):
-            if len(prefix) > len(lst): return False
+            if len(prefix) > len(lst):
+                return False
             return all(n == l for n, l in zip(prefix, lst))
 
         # compare the line word by word to also match lines that differ only in
         # whitespace
         prefix = prefix.split()
-        for parameter, value in zip(self._dataset["Parameter"],
-                                    self._dataset["Value"]):
+        for parameter, value in zip(self._dataset["Parameter"], self._dataset["Value"]):
             words = (parameter + " " + value).strip().split()
             if isprefix(prefix, words):
                 return words
 
-        raise ValueError("No line with prefix \"{}\" found.".format(
-                            " ".join(prefix)))
+        raise ValueError('No line with prefix "{}" found.'.format(" ".join(prefix)))
 
     def get_element_id(self, element_symbol):
         """
         Return numeric element id for element. If potential does not contain
         the element raise a :class:NameError.  Only makes sense for potentials
         with pair_style "full".
 
@@ -145,16 +152,15 @@
         """
 
         try:
             line = "group {} type".format(element_symbol)
             return int(self._find_line_by_prefix(line)[3])
 
         except ValueError:
-            msg = "potential does not contain element {}".format(
-                    element_symbol)
+            msg = "potential does not contain element {}".format(element_symbol)
             raise NameError(msg) from None
 
     def get_charge(self, element_symbol):
         """
         Return charge for element. If potential does not specify a charge,
         raise a :class:NameError.  Only makes sense for potentials
         with pair_style "full".
@@ -171,15 +177,16 @@
 
         try:
             line = "set group {} charge".format(element_symbol)
             return float(self._find_line_by_prefix(line)[4])
 
         except ValueError:
             msg = "potential does not specify charge for element {}".format(
-                    element_symbol)
+                element_symbol
+            )
             raise NameError(msg) from None
 
     def to_hdf(self, hdf, group_name=None):
         if self._df is not None:
             with hdf.open("potential") as hdf_pot:
                 hdf_pot["Config"] = self._df["Config"].values[0]
                 hdf_pot["Filename"] = self._df["Filename"].values[0]
@@ -278,21 +285,53 @@
             selected_atoms=selected_atoms,
         )
 
 
 class PotentialAvailable(object):
     def __init__(self, list_of_potentials):
         self._list_of_potentials = {
-            "pot_" + v.replace("-", "_").replace('.', '_'): v for v in list_of_potentials
+            "pot_" + v.replace("-", "_").replace(".", "_"): v
+            for v in list_of_potentials
         }
 
     def __getattr__(self, name):
         if name in self._list_of_potentials.keys():
             return self._list_of_potentials[name]
         else:
             raise AttributeError
 
     def __dir__(self):
         return list(self._list_of_potentials.keys())
 
     def __repr__(self):
         return str(dir(self))
+
+
+def view_potentials(structure: Atoms) -> pd.DataFrame:
+    """
+    List all interatomic potentials for the given atomistic structure including all potential parameters.
+
+    To quickly get only the names of the potentials you can use `list_potentials()` instead.
+
+    Args:
+        structure (Atoms): The structure for which to get potentials.
+
+    Returns:
+        pandas.Dataframe: Dataframe including all potential parameters.
+    """
+    list_of_elements = set(structure.get_chemical_symbols())
+    return LammpsPotentialFile().find(list_of_elements)
+
+
+def list_potentials(structure: Atoms) -> List[str]:
+    """
+    List of interatomic potentials suitable for the given atomic structure.
+
+    See `view_potentials` to get more details.
+
+    Args:
+        structure (Atoms): The structure for which to get potentials.
+
+    Returns:
+        list: potential names
+    """
+    return list(view_potentials(structure)["Name"].values)
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/structure.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/structure.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from __future__ import print_function
 from collections import OrderedDict
 import numpy as np
-from pyiron_base import GenericParameters
+import posixpath
 import decimal as dec
 import warnings
+from pyiron_atomistics.lammps.units import UnitConverter
 
 try:
     from ase.calculators.lammps import Prism
-
 except ImportError:
     try:
         from ase.calculators.lammpsrun import Prism
     except ImportError:
         from ase.calculators.lammpsrun import prism as Prism
 
 __author__ = "Joerg Neugebauer, Sudarsan Surendralal, Yury Lysogorskiy, Jan Janssen, Markus Tautschnig"
@@ -66,15 +66,15 @@
         gamma = np.arccos(np.dot(a, b) / (an * bn))
 
         xhi = an
         xyp = np.cos(gamma) * bn
         yhi = np.sin(gamma) * bn
         xzp = np.cos(beta) * cn
         yzp = (bn * cn * np.cos(alpha) - xyp * xzp) / yhi
-        zhi = np.sqrt(cn ** 2 - xzp ** 2 - yzp ** 2)
+        zhi = np.sqrt(cn**2 - xzp**2 - yzp**2)
 
         # Set precision
         self.car_prec = dec.Decimal("10.0") ** int(
             np.floor(np.log10(max((xhi, yhi, zhi)))) - digits
         )
         self.dir_prec = dec.Decimal("10.0") ** (-digits)
         self.acc = float(self.car_prec)
@@ -113,15 +113,17 @@
                 print("debug: apply shift")
                 apre[1, 0] += 2 * d_a
                 apre[2, 0] += 2 * d_a
 
         self.A = apre
 
         if self.is_skewed() and (not (pbc[0] and pbc[1] and pbc[2])):
-            warnings.warn( "Skewed lammps cells should have PBC == True in all directions!")
+            warnings.warn(
+                "Skewed lammps cells should have PBC == True in all directions!"
+            )
 
     def unfold_cell(self, cell):
         """
         Unfold LAMMPS cell to original
 
         Let C be the pyiron_atomistics cell and A be the Lammps cell, then define (in init) the rotation matrix between them as
             R := C^inv.A
@@ -171,36 +173,32 @@
 
     def get_lammps_prism_str(self):
         """Return a tuple of strings"""
         p = self.get_lammps_prism()
         return tuple([self.f2s(x) for x in p])
 
 
-class LammpsStructure(GenericParameters):
+class LammpsStructure(object):
     """
 
     Args:
         input_file_name:
     """
 
-    def __init__(self, input_file_name=None, bond_dict=None):
-        super(LammpsStructure, self).__init__(
-            input_file_name=input_file_name,
-            table_name="structure_inp",
-            comment_char="#",
-            val_only=True,
-        )
+    def __init__(self, bond_dict=None, job=None):
+        self._string_input = ""
         self._structure = None
         self._potential = None
         self._el_eam_lst = []
         self.atom_type = None
         self.cutoff_radius = None
         self.digits = 10
         self._bond_dict = bond_dict
         self._force_skewed = False
+        self._job = job
 
     @property
     def potential(self):
         return self._potential
 
     @potential.setter
     def potential(self, val):
@@ -230,15 +228,29 @@
             input_str = self.structure_full()
         elif self.atom_type == "bond":
             input_str = self.structure_bond()
         elif self.atom_type == "charge":
             input_str = self.structure_charge()
         else:  # self.atom_type == 'atomic'
             input_str = self.structure_atomic()
-        self.load_string(input_str)
+
+        if self._structure.velocities is not None:
+            uc = UnitConverter(self._job.units)
+            self._structure.velocities *= uc.pyiron_to_lammps("velocity")
+            vels = self.rotate_velocities(self._structure)
+            input_str += "Velocities\n\n"
+            if self._structure.dimension == 3:
+                format_str = "{0:d} {1:f} {2:f} {3:f}\n"
+                for id_atom, (x, y, z) in enumerate(vels, start=1):
+                    input_str += format_str.format(id_atom, x, y, z)
+            if self._structure.dimension == 2:
+                format_str = "{0:d} {1:f} {2:f}\n"
+                for id_atom, (x, y) in enumerate(vels, start=1):
+                    input_str += format_str.format(id_atom, x, y)
+        self._string_input = input_str
 
     @property
     def el_eam_lst(self):
         """
 
         Returns:
 
@@ -253,23 +265,14 @@
             el_eam_lst:
 
         Returns:
 
         """
         self._el_eam_lst = el_eam_lst
 
-    def load_default(self):
-        """
-
-        Returns:
-
-        """
-        input_str = ""
-        self.load_string(input_str)
-
     def simulation_cell(self):
         """
 
         Returns:
 
         """
 
@@ -335,15 +338,15 @@
             " Start File for LAMMPS \n"
             + "{0:d} atoms".format(len(self._structure))
             + " \n"
             + "{0:d} bonds".format(len(bonds))
             + " \n"
             + "{0} atom types".format(self._structure.get_number_of_species())
             + " \n"
-            + "{0} bond types".format(np.max(bond_type))
+            + "{0} bond types".format(np.max(np.array(bonds)[:, 2]))
             + " \n"
         )
 
         cell_dimesions = self.simulation_cell()
 
         masses = "Masses \n\n"
         el_obj_list = self._structure.get_species_objects()
@@ -407,65 +410,79 @@
             species_name = species.Abbreviation
             q_dict[species_name] = self.potential.get_charge(species_name)
             species_translate_list.append(self.potential.get_element_id(species_name))
         sorted_species_list = np.array(self._potential.get_element_lst())
         molecule_lst, bonds_lst, angles_lst = [], [], []
         bond_type_lst, angle_type_lst = [], []
         # Using a cutoff distance to draw the bonds instead of the number of neighbors
-        cutoff_list = list()
-        for val in self._bond_dict.values():
-            cutoff_list.append(np.max(val["cutoff_list"]))
-        max_cutoff = np.max(cutoff_list)
-        # Calculate neighbors only once
-        neighbors = self._structure.get_neighbors_by_distance(cutoff_radius=max_cutoff)
-        id_mol = 0
-        indices = self._structure.indices
-        for id_el, id_species in enumerate(indices):
-            id_mol += 1
-            molecule_lst.append([id_el, id_mol, species_translate_list[id_species]])
-        # Draw bonds between atoms is defined in self._bond_dict
-        # Go through all elements for which bonds are defined
-        for element, val in self._bond_dict.items():
-            el_1_list = self._structure.select_index(element)
-            if el_1_list is not None:
-                if len(el_1_list) > 0:
-                    for i, v in enumerate(val["element_list"]):
-                        el_2_list = self._structure.select_index(v)
-                        cutoff_dist = val["cutoff_list"][i]
-                        for j, ind in enumerate(np.array(neighbors.indices)[el_1_list]):
-                            # Only chose those indices within the cutoff distance and which belong
-                            # to the species defined in the element_list
-                            # i is the index of each bond type, and j is the element index
-                            id_el = el_1_list[j]
-                            bool_1 = np.array(neighbors.distances)[id_el] <= cutoff_dist
-                            act_ind = ind[bool_1]
-                            bool_2 = np.in1d(act_ind, el_2_list)
-                            final_ind = act_ind[bool_2]
-                            # Get the bond and angle type
-                            bond_type = val["bond_type_list"][i]
-                            angle_type = val["angle_type_list"][i]
-                            # Draw only maximum allowed bonds
-                            final_ind = final_ind[:val["max_bond_list"][i]]
-                            for fi in final_ind:
-                                bonds_lst.append([id_el + 1, fi + 1])
-                                bond_type_lst.append(bond_type)
-                            # Draw angles if at least 2 bonds are present and if an angle type is defined for this
-                            # particular set of bonds
-                            if len(final_ind) >= 2 and val["angle_type_list"][i] is not None:
-                                angles_lst.append([final_ind[0] + 1, id_el + 1, final_ind[1] + 1])
-                                angle_type_lst.append(angle_type)
-        m_lst = np.array(molecule_lst)
-        molecule_lst = m_lst[m_lst[:, 0].argsort()]
+        # Only if any bonds are defined
+        if len(self._bond_dict.keys()) > 0:
+            cutoff_list = list()
+            for val in self._bond_dict.values():
+                cutoff_list.append(np.max(val["cutoff_list"]))
+            max_cutoff = np.max(cutoff_list)
+            # Calculate neighbors only once
+            neighbors = self._structure.get_neighbors_by_distance(
+                cutoff_radius=max_cutoff
+            )
+            id_mol = 0
+            indices = self._structure.indices
+            for id_el, id_species in enumerate(indices):
+                id_mol += 1
+                molecule_lst.append([id_el, id_mol, species_translate_list[id_species]])
+            # Draw bonds between atoms is defined in self._bond_dict
+            # Go through all elements for which bonds are defined
+            for element, val in self._bond_dict.items():
+                el_1_list = self._structure.select_index(element)
+                if el_1_list is not None:
+                    if len(el_1_list) > 0:
+                        for i, v in enumerate(val["element_list"]):
+                            el_2_list = self._structure.select_index(v)
+                            cutoff_dist = val["cutoff_list"][i]
+                            for j, ind in enumerate(
+                                np.array(neighbors.indices, dtype=object)[el_1_list]
+                            ):
+                                # Only chose those indices within the cutoff distance and which belong
+                                # to the species defined in the element_list
+                                # i is the index of each bond type, and j is the element index
+                                id_el = el_1_list[j]
+                                bool_1 = (
+                                    np.array(neighbors.distances, dtype=object)[id_el]
+                                    <= cutoff_dist
+                                )
+                                act_ind = ind[bool_1]
+                                bool_2 = np.in1d(act_ind, el_2_list)
+                                final_ind = act_ind[bool_2]
+                                # Get the bond and angle type
+                                bond_type = val["bond_type_list"][i]
+                                angle_type = val["angle_type_list"][i]
+                                # Draw only maximum allowed bonds
+                                final_ind = final_ind[: val["max_bond_list"][i]]
+                                for fi in final_ind:
+                                    bonds_lst.append([id_el + 1, fi + 1])
+                                    bond_type_lst.append(bond_type)
+                                # Draw angles if at least 2 bonds are present and if an angle type is defined for this
+                                # particular set of bonds
+                                if (
+                                    len(final_ind) >= 2
+                                    and val["angle_type_list"][i] is not None
+                                ):
+                                    angles_lst.append(
+                                        [final_ind[0] + 1, id_el + 1, final_ind[1] + 1]
+                                    )
+                                    angle_type_lst.append(angle_type)
+            m_lst = np.array(molecule_lst)
+            molecule_lst = m_lst[m_lst[:, 0].argsort()]
 
         if len(bond_type_lst) == 0:
-            num_bond_types = 1
+            num_bond_types = 0
         else:
             num_bond_types = int(np.max(bond_type_lst))
         if len(angle_type_lst) == 0:
-            num_angle_types = 1
+            num_angle_types = 0
         else:
             num_angle_types = int(np.max(angle_type_lst))
 
         atomtypes = (
             " Start File for LAMMPS \n"
             + "{0:d} atoms".format(len(self._structure))
             + " \n"
@@ -491,15 +508,17 @@
         atoms = "Atoms \n\n"
 
         # format: atom-ID, molecule-ID, atom_type, q, x, y, z
         format_str = "{0:d} {1:d} {2:d} {3:f} {4:f} {5:f} {6:f}"
         for atom in molecule_lst:
             id_atom, id_mol, id_species = atom
             x, y, z = coords[id_atom]
-            ind = np.argwhere(np.array(species_translate_list) == id_species).flatten()[0]
+            ind = np.argwhere(np.array(species_translate_list) == id_species).flatten()[
+                0
+            ]
             el_id = self._structure.species[ind].Abbreviation
             atoms += (
                 format_str.format(
                     id_atom + 1, id_mol, id_species, q_dict[el_id], x, y, z
                 )
                 + "\n"
             )
@@ -517,15 +536,19 @@
             bonds_str = "\n"
 
         if len(angles_lst) > 0:
             angles_str = "Angles \n\n"
             for i_angle, id_vec in enumerate(angles_lst):
                 angles_str += (
                     "{0:d} {1:d} {2:d} {3:d} {4:d}".format(
-                        i_angle + 1, angle_type_lst[i_angle], id_vec[0], id_vec[1], id_vec[2]
+                        i_angle + 1,
+                        angle_type_lst[i_angle],
+                        id_vec[0],
+                        id_vec[1],
+                        id_vec[2],
                     )
                     + "\n"
                 )
         else:
             angles_str = "\n"
         return (
             atomtypes
@@ -565,16 +588,15 @@
 
         for ind, obj in enumerate(self._structure.get_species_objects()):
             masses += "{0:3d} {1:f}".format(ind + 1, obj.AtomicMass) + "\n"
 
         atoms = "Atoms\n\n"
 
         coords = self.rotate_positions(self._structure)
-
-        el_charge_lst = self._structure.charge
+        el_charge_lst = self._structure.get_initial_charges()
         el_lst = self._structure.get_chemical_symbols()
         el_alphabet_dict = {}
         for ind, el in enumerate(self._structure.get_species_symbols()):
             el_alphabet_dict[el] = ind + 1
         for id_atom, (el, coord) in enumerate(zip(el_lst, coords)):
             id_el = el_alphabet_dict[el]
             dim = self._structure.dimension
@@ -625,15 +647,17 @@
         coords = self.rotate_positions(self._structure)
 
         el_lst = self._structure.get_chemical_elements()
         for id_atom, (el, coord) in enumerate(zip(el_lst, coords)):
             if el in el_dict.keys():
                 id_el = el_dict[el]
             else:
-                raise ValueError("Selected potential does not support the existing chemical composition")
+                raise ValueError(
+                    "Selected potential does not support the existing chemical composition"
+                )
             dim = self._structure.dimension
             c = np.zeros(3)
             c[:dim] = coord
             atoms += (
                 "{0:d} {1:d} {2:.15f} {3:.15f} {4:.15f}".format(
                     id_atom + 1, id_el, c[0], c[1], c[2]
                 )
@@ -651,13 +675,61 @@
         Returns:
             (list): List of rotated coordinates
         """
         prism = UnfoldingPrism(self._structure.cell)
         coords = [prism.pos_to_lammps(position) for position in structure.positions]
         return coords
 
+    def rotate_velocities(self, structure):
+        """
+        Rotate all atomic velocities in given structure according to new Prism cell
+
+        Args:
+            structure: Atoms-like object. Should have .velocities attribute.
+
+        Returns:
+            (list): List of rotated velocities
+        """
+        prism = UnfoldingPrism(self._structure.cell)
+        vels = [prism.pos_to_lammps(vel) for vel in structure.velocities]
+        return vels
+
+    def write_file(self, file_name, cwd=None):
+        """
+        Write GenericParameters to input file
+
+        Args:
+            file_name (str): name of the file, either absolute (then cwd must be None) or relative
+            cwd (str): path name (default: None)
+        """
+        if cwd is not None:
+            file_name = posixpath.join(cwd, file_name)
+
+        with open(file_name, "w") as f:
+            for line in self._string_input:
+                f.write(line)
+
 
 def write_lammps_datafile(structure, file_name="lammps.data", cwd=None):
     lammps_str = LammpsStructure()
     lammps_str.el_eam_lst = structure.get_species_symbols()
     lammps_str.structure = structure
     lammps_str.write_file(file_name=file_name, cwd=cwd)
+
+
+def structure_to_lammps(structure):
+    """
+    Converts a structure to the Lammps coordinate frame
+
+    Args:
+        structure (pyiron.atomistics.structure.atoms.Atoms): Structure to convert.
+
+    Returns:
+        pyiron.atomistics.structure.atoms.Atoms: Structure with the LAMMPS coordinate frame.
+    """
+    prism = UnfoldingPrism(structure.cell)
+    lammps_structure = structure.copy()
+    lammps_structure.set_cell(prism.A)
+    lammps_structure.positions = np.matmul(structure.positions, prism.R)
+    if structure.velocities is not None:
+        lammps_structure.velocities = np.matmul(structure.velocities, prism.R)
+    return lammps_structure
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/project.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from __future__ import print_function
 import os
 import posixpath
+
 # import warnings
 from string import punctuation
 from shutil import copyfile
-from pyiron_base import Settings, ProjectHDFio, JobType, JobTypeChoice, Project as ProjectCore, Creator as CreatorCore
+from pyiron_base import (
+    ProjectHDFio,
+    JobType,
+    JobTypeChoice,
+    Project as ProjectCore,
+    Creator as CreatorCore,
+    deprecate,
+)
+
 try:
     from pyiron_base import ProjectGUI
 except (ImportError, TypeError, AttributeError):
     pass
-from pyiron_atomistics.atomistics.generic.object_type import ObjectType, ObjectTypeChoice
+from pyiron_atomistics.atomistics.generic.object_type import (
+    ObjectType,
+    ObjectTypeChoice,
+)
 from pyiron_atomistics.atomistics.structure.periodic_table import PeriodicTable
 from pyiron_atomistics.lammps.potential import LammpsPotentialFile
 from pyiron_atomistics.vasp.potential import VaspPotential
 import pyiron_atomistics.atomistics.structure.pyironase as ase
 from pyiron_atomistics.atomistics.structure.atoms import Atoms
 from pyiron_atomistics.atomistics.structure.factory import StructureFactory
 from pyiron_atomistics.atomistics.master.parallel import pipe
@@ -33,20 +45,28 @@
 __email__ = "janssen@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 if not (isinstance(ase.__file__, str)):
     raise AssertionError()
 
-s = Settings()
-
 
 class Project(ProjectCore):
     """
-    The project is the central class in pyiron, all other objects can be created from the project object.
+    Welcome to pyiron! The project is the central class in pyiron, all other objects can be
+    created from the project object.
+
+    Your first steps in pyiron:
+
+    >>> pr = Project("EXAMPLE")
+    >>> job = pr.create.job.Lammps(job_name="lmp_example")
+
+    Replace `Lammps` by the job type of your choice - you can look at the list of all available
+    jobs in the list of auto-complete in `pr.create.job`. After you create a job, look up the
+    DocString of your job by `job?` to find out what are the next steps!
 
     Args:
         path (GenericPath, str): path of the project defined by GenericPath, absolute or relative (with respect to
                                      current working directory) path
         user (str): current pyiron user
         sql_query (str): SQL query to only select a subset of the existing jobs within the current project
         default_working_directory (bool): Access default working directory, for ScriptJobs this equals the project
@@ -101,20 +121,22 @@
                                              ‘MinimizeMurnaghan’, ‘ElasticMatrix’, ‘ConvergenceVolume’,
                                              ‘ConvergenceEncutParallel’, ‘ConvergenceKpointParallel’, ’PhonopyMaster’,
                                              ‘DefectFormationEnergy’, ‘LammpsASE’, ‘PipelineMaster’,
                                              ’TransformationPath’, ‘ThermoIntEamQh’, ‘ThermoIntDftEam’, ‘ScriptJob’,
                                              ‘ListMaster']
     """
 
-    def __init__(self, path="", user=None, sql_query=None, default_working_directory=False):
+    def __init__(
+        self, path="", user=None, sql_query=None, default_working_directory=False
+    ):
         super(Project, self).__init__(
             path=path,
             user=user,
             sql_query=sql_query,
-            default_working_directory=default_working_directory
+            default_working_directory=default_working_directory,
         )
         self.job_type = JobTypeChoice()
         self.object_type = ObjectTypeChoice()
         self._creator = Creator(self)
         # TODO: instead of re-initialzing, auto-update pyiron_base creator with factories, like we update job class
         #  creation
 
@@ -228,15 +250,19 @@
         job = super(Project, self).load_from_jobpath_string(
             job_path=job_path, convert_to_object=convert_to_object
         )
         job.project_hdf5._project = Project(path=job.project_hdf5.file_path)
         return job
 
     def import_single_calculation(
-        self, project_to_import_from, rel_path=None, job_type="Vasp", copy_raw_files=False
+        self,
+        project_to_import_from,
+        rel_path=None,
+        job_type="Vasp",
+        copy_raw_files=False,
     ):
         """
         A method to import a single calculation jobs into pyiron. Currently, it suppor
         ts VASP and KMC calculations.
         Args:
             rel_path:
             project_to_import_from:
@@ -272,23 +298,22 @@
                 project_to_import_from = os.path.join(self.path, project_to_import_from)
             try:
                 ham.from_directory(project_to_import_from.replace("\\", "/"))
             except:
                 ham.status.aborted = True
             else:
                 ham._import_directory = None
-                del ham['import_directory']
+                del ham["import_directory"]
                 if copy_raw_files:
                     os.makedirs(ham.working_directory, exist_ok=True)
                     for f in os.listdir(project_to_import_from):
                         src = os.path.join(project_to_import_from, f)
                         if os.path.isfile(src):
                             copyfile(
-                                src=src,
-                                dst=os.path.join(ham.working_directory, f)
+                                src=src, dst=os.path.join(ham.working_directory, f)
                             )
                     ham.compress()
 
     def import_from_path(self, path, recursive=True, copy_raw_files=False):
         """
         A method to import jobs into pyiron. Currently, it supports VASP and
         KMC calculations.
@@ -304,21 +329,27 @@
         else:
             search_path = posixpath.normpath(
                 posixpath.join(self.path, path.replace("//", "/"))
             )
         if recursive:
             for x in os.walk(search_path):
                 self._calculation_validation(
-                    x[0], x[2], rel_path=posixpath.relpath(x[0], search_path), copy_raw_files=copy_raw_files
+                    x[0],
+                    x[2],
+                    rel_path=posixpath.relpath(x[0], search_path),
+                    copy_raw_files=copy_raw_files,
                 )
         else:
             abs_path = "/".join(search_path.replace("\\", "/").split("/")[:-1])
             rel_path = posixpath.relpath(abs_path, self.path)
             self._calculation_validation(
-                search_path, os.listdir(search_path), rel_path=rel_path, copy_raw_files=copy_raw_files
+                search_path,
+                os.listdir(search_path),
+                rel_path=rel_path,
+                copy_raw_files=copy_raw_files,
             )
 
     def get_structure(self, job_specifier, iteration_step=-1, wrap_atoms=True):
         """
         Gets the structure from a given iteration step of the simulation (MD/ionic relaxation). For static calculations
         there is only one ionic iteration step
         Args:
@@ -344,15 +375,17 @@
                     job.get("output/generic/dft/atom_spins")[iteration_step]
                 )
         if wrap_atoms:
             return snapshot.center_coordinates_in_unit_cell()
         else:
             return snapshot
 
-    def _calculation_validation(self, path, files_available, rel_path=None, copy_raw_files=False):
+    def _calculation_validation(
+        self, path, files_available, rel_path=None, copy_raw_files=False
+    ):
         """
 
         Args:
             path:
             files_available:
             rel_path:
             copy_raw_files (bool):
@@ -360,21 +393,25 @@
         if (
             "OUTCAR" in files_available
             or "vasprun.xml" in files_available
             or "OUTCAR.gz" in files_available
             or "vasprun.xml.bz2" in files_available
             or "vasprun.xml.gz" in files_available
         ):
-            self.import_single_calculation(path, rel_path=rel_path, job_type="Vasp", copy_raw_files=copy_raw_files)
+            self.import_single_calculation(
+                path, rel_path=rel_path, job_type="Vasp", copy_raw_files=copy_raw_files
+            )
         if (
             "incontrol.dat" in files_available
             and "lattice.out" in files_available
             and "lattice.inp" in files_available
         ):
-            self.import_single_calculation(path, rel_path=rel_path, job_type="KMC", copy_raw_files=copy_raw_files)
+            self.import_single_calculation(
+                path, rel_path=rel_path, job_type="KMC", copy_raw_files=copy_raw_files
+            )
 
     @staticmethod
     def inspect_periodic_table():
         return PeriodicTable()
 
     @staticmethod
     def inspect_emperical_potentials():
@@ -400,28 +437,34 @@
         Args:
             job (AtomisticGenericJob): Template for the calculation
             step_lst (list): List of functions which create calculations
 
         Returns:
             FlexibleMaster:
         """
-        return pipe(project=self, job=job, step_lst=step_lst, delete_existing_job=delete_existing_job)
+        return pipe(
+            project=self,
+            job=job,
+            step_lst=step_lst,
+            delete_existing_job=delete_existing_job,
+        )
 
     # Deprecated methods
 
+    @deprecate("Use create.structure.bulk instead")
     def create_ase_bulk(
-            self,
-            name,
-            crystalstructure=None,
-            a=None,
-            c=None,
-            covera=None,
-            u=None,
-            orthorhombic=False,
-            cubic=False,
+        self,
+        name,
+        crystalstructure=None,
+        a=None,
+        c=None,
+        covera=None,
+        u=None,
+        orthorhombic=False,
+        cubic=False,
     ):
         """
         Creating bulk systems using ASE bulk module. Crystal structure and lattice constant(s) will be guessed if not
         provided.
 
         name (str): Chemical symbol or symbols as in 'MgO' or 'NaCl'.
         crystalstructure (str): Must be one of sc, fcc, bcc, hcp, diamond, zincblende,
@@ -433,21 +476,26 @@
         orthorhombic (bool): Construct orthorhombic unit cell instead of primitive cell which is the default.
         cubic (bool): Construct cubic unit cell if possible.
 
         Returns:
 
             pyiron.atomistics.structure.atoms.Atoms: Required bulk structure
         """
-        # warnings.warn(
-        #     "Project.create_ase_bulk is deprecated as of v0.3. Please use Project.create.structure.ase_bulk.",
-        #     DeprecationWarning
-        # )
-        return self.create.structure.ase.bulk(name=name, crystalstructure=crystalstructure, a=a, c=c,
-                                              covera=covera, u=u, orthorhombic=orthorhombic, cubic=cubic)
+        return self.create.structure.ase.bulk(
+            name=name,
+            crystalstructure=crystalstructure,
+            a=a,
+            c=c,
+            covera=covera,
+            u=u,
+            orthorhombic=orthorhombic,
+            cubic=cubic,
+        )
 
+    @deprecate("Use create.structure.* methods instead")
     def create_structure(self, element, bravais_basis, lattice_constant):
         """
         Create a crystal structure using pyiron's native crystal structure generator
 
         Args:
             element (str): Element name
             bravais_basis (str): Basis type
@@ -457,19 +505,30 @@
             pyiron.atomistics.structure.atoms.Atoms: The required crystal structure
 
         """
         # warnings.warn(
         #     "Project.create_structure is deprecated as of v0.3. Please use Project.create.structure.structure.",
         #     DeprecationWarning
         # )
-        return self.create.structure.crystal(element=element, bravais_basis=bravais_basis,
-                                             lattice_constant=lattice_constant)
+        return self.create.structure.crystal(
+            element=element,
+            bravais_basis=bravais_basis,
+            lattice_constant=lattice_constant,
+        )
 
+    @deprecate("Use create.structure.surface instead")
     def create_surface(
-            self, element, surface_type, size=(1, 1, 1), vacuum=1.0, center=False, pbc=None, **kwargs
+        self,
+        element,
+        surface_type,
+        size=(1, 1, 1),
+        vacuum=1.0,
+        center=False,
+        pbc=None,
+        **kwargs
     ):
         """
         Generate a surface based on the ase.build.surface module.
 
         Args:
             element (str): Element name
             surface_type (str): The string specifying the surface type generators available through ase (fcc111,
@@ -486,39 +545,47 @@
             pyiron_atomistics.atomistics.structure.atoms.Atoms instance: Required surface
 
         """
         # warnings.warn(
         #     "Project.create_surface is deprecated as of v0.3. Please use Project.create.structure.surface.",
         #     DeprecationWarning
         # )
-        return self.create.structure.surface(element=element, surface_type=surface_type, size=size,
-                                             vacuum=vacuum, center=center, pbc=pbc, **kwargs)
+        return self.create.structure.surface(
+            element=element,
+            surface_type=surface_type,
+            size=size,
+            vacuum=vacuum,
+            center=center,
+            pbc=pbc,
+            **kwargs
+        )
 
+    @deprecate("Use create.structure.atoms instead")
     def create_atoms(
-            self,
-            symbols=None,
-            positions=None,
-            numbers=None,
-            tags=None,
-            momenta=None,
-            masses=None,
-            magmoms=None,
-            charges=None,
-            scaled_positions=None,
-            cell=None,
-            pbc=None,
-            celldisp=None,
-            constraint=None,
-            calculator=None,
-            info=None,
-            indices=None,
-            elements=None,
-            dimension=None,
-            species=None,
-            **qwargs
+        self,
+        symbols=None,
+        positions=None,
+        numbers=None,
+        tags=None,
+        momenta=None,
+        masses=None,
+        magmoms=None,
+        charges=None,
+        scaled_positions=None,
+        cell=None,
+        pbc=None,
+        celldisp=None,
+        constraint=None,
+        calculator=None,
+        info=None,
+        indices=None,
+        elements=None,
+        dimension=None,
+        species=None,
+        **qwargs
     ):
         """
         Creates a atomistics.structure.atoms.Atoms instance.
 
         Args:
             elements (list/numpy.ndarray): List of strings containing the elements or a list of
                                 atomistics.structure.periodic_table.ChemicalElement instances
@@ -567,15 +634,18 @@
             indices=indices,
             elements=elements,
             dimension=dimension,
             species=species,
             **qwargs
         )
 
-    def create_element(self, parent_element, new_element_name=None, spin=None, potential_file=None):
+    @deprecate("Use create.structure.element instead")
+    def create_element(
+        self, parent_element, new_element_name=None, spin=None, potential_file=None
+    ):
         """
         Args:
             parent_element (str, int): The parent element eq. "N", "O", "Mg" etc.
             new_element_name (str): The name of the new parent element (can be arbitrary)
             spin (float): Value of the magnetic moment (with sign)
             potential_file (str): Location of the new potential file if necessary
 
@@ -586,20 +656,19 @@
         #     "Project.create_element is deprecated as of v0.3. Please use Project.create.structure.element.",
         #     DeprecationWarning
         # )
         return self.create.structure.element(
             parent_element=parent_element,
             new_element_name=new_element_name,
             spin=spin,
-            potential_file=potential_file
+            potential_file=potential_file,
         )
 
 
 class Creator(CreatorCore):
-
     def __init__(self, project):
         super().__init__(project)
         self._structure = StructureFactory()
 
     @property
     def structure(self):
         return self._structure
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/base.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,50 +5,54 @@
 from __future__ import print_function, division
 
 import numpy as np
 import os
 import posixpath
 import re
 import stat
-from shutil import copyfile
+from shutil import copyfile, move as movefile
 import scipy.constants
 import warnings
 import json
-from collections import defaultdict
 import spglib
+import subprocess
+from subprocess import PIPE
+import tarfile
+from tempfile import TemporaryDirectory
 
 from pyiron_atomistics.dft.job.generic import GenericDFTJob
 from pyiron_atomistics.dft.waves.electronic import ElectronicStructure
-from pyiron_atomistics.vasp.potential import VaspPotentialFile, \
-    strip_xc_from_potential_name, \
-    find_potential_file as find_potential_file_vasp, \
-    VaspPotentialSetter
+from pyiron_atomistics.vasp.potential import (
+    VaspPotentialFile,
+    strip_xc_from_potential_name,
+    find_potential_file as find_potential_file_vasp,
+    VaspPotentialSetter,
+)
 from pyiron_atomistics.sphinx.structure import read_atoms
 from pyiron_atomistics.sphinx.potential import SphinxJTHPotentialFile
-from pyiron_atomistics.sphinx.potential import find_potential_file \
-    as find_potential_file_jth
+from pyiron_atomistics.sphinx.potential import (
+    find_potential_file as find_potential_file_jth,
+)
+from pyiron_atomistics.sphinx.util import sxversions
 from pyiron_atomistics.sphinx.volumetric_data import SphinxVolumetricData
-from pyiron_base import Settings, DataContainer, job_status_successful_lst, deprecate
+from pyiron_base import state, DataContainer, job_status_successful_lst, deprecate
 
 __author__ = "Osamu Waseda, Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "development"
 __date__ = "Sep 1, 2017"
 
-s = Settings()
-
 BOHR_TO_ANGSTROM = (
-    scipy.constants.physical_constants["Bohr radius"][0] /
-    scipy.constants.angstrom
+    scipy.constants.physical_constants["Bohr radius"][0] / scipy.constants.angstrom
 )
 HARTREE_TO_EV = scipy.constants.physical_constants["Hartree energy in eV"][0]
 RYDBERG_TO_EV = HARTREE_TO_EV / 2
 HARTREE_OVER_BOHR_TO_EV_OVER_ANGSTROM = HARTREE_TO_EV / BOHR_TO_ANGSTROM
 
 
 class SphinxBase(GenericDFTJob):
@@ -62,23 +66,23 @@
 
     Alternatively, because SPHInX inputs are built on a group-based
     format, users have the option to set specific groups and parameters
     directly, e.g.
 
     ```python
     # Modify/add a new parameter via
-    job.input.PAWHamiltonian.nEmptyStates = 15
-    job.input.PAWHamiltonian.dipoleCorrection = True
+    job.input.sphinx.PAWHamiltonian.nEmptyStates = 15
+    job.input.sphinx.PAWHamiltonian.dipoleCorrection = True
     # or
-    job.input.PAWHamiltonian.set("nEmptyStates", 15)
-    job.input.PAWHamiltonian.set("dipoleCorrection", True)
+    job.input.sphinx.PAWHamiltonian.set("nEmptyStates", 15)
+    job.input.sphinx.PAWHamiltonian.set("dipoleCorrection", True)
     # Modify/add a sub-group via
-    job.input.initialGuess.rho.charged = {"charge": 2, "z": 25}
+    job.input.sphinx.initialGuess.rho.charged = {"charge": 2, "z": 25}
     # or
-    job.input.initialGuess.rho.set("charged", {"charge": 2, "z": 25})
+    job.input.sphinx.initialGuess.rho.set("charged", {"charge": 2, "z": 25})
     ```
 
     Args:
         project: Project object (defines path where job will be
                  created and stored)
         job_name (str): name of the job (must be unique within
                         this project path)
@@ -88,25 +92,47 @@
     __hdf_version__ = "0.1.0"
 
     def __init__(self, project, job_name):
         super(SphinxBase, self).__init__(project, job_name)
 
         # keeps both the generic parameters as well as the sphinx specific
         # input groups
-        self.input = Group(table_name = "parameters")
+        self.input = Group(table_name="parameters", lazy=True)
         self.load_default_input()
-        self._save_memory = False
-        self._output_parser = Output(self)
+        self.output = Output(job=self)
         self.input_writer = InputWriter()
         self._potential = VaspPotentialSetter([])
         if self.check_vasp_potentials():
             self.input["VaspPot"] = True  # use VASP potentials if available
         self._generic_input["restart_for_band_structure"] = False
         self._generic_input["path_name"] = None
         self._generic_input["n_path"] = None
+        self._generic_input["fix_spin_constraint"] = False
+
+    def update_sphinx(self):
+        if self.output.old_version:
+            _update_datacontainer(self)
+
+    def __getitem__(self, item):
+        if not isinstance(item, str):
+            return super().__getitem__(item)
+        result = None
+        if item[-1] == "/":
+            item = item[:-1]
+        for tag in item.split("/"):
+            try:  # horrible workaround to be removed when hdf output becomes consistent
+                if result is None:
+                    result = super().__getitem__(tag)
+                else:
+                    result = result[tag]
+                if hasattr(result, "list_nodes") and "TYPE" in result.list_nodes():
+                    result = result.to_object()
+            except (ValueError, KeyError):
+                return None
+        return result
 
     @property
     def structure(self):
         """
 
         Returns:
 
@@ -209,15 +235,17 @@
         else:
             if self.input["VaspPot"]:
                 potentials = VaspPotentialFile(xc=self.input["Xcorr"])
             else:
                 potentials = SphinxJTHPotentialFile(xc=self.input["Xcorr"])
             df = potentials.find(self.structure.get_species_symbols().tolist())
             if len(df) > 0:
-                df["Name"] = [strip_xc_from_potential_name(n) for n in df["Name"].values]
+                df["Name"] = [
+                    strip_xc_from_potential_name(n) for n in df["Name"].values
+                ]
             return df
 
     @property
     def potential_list(self):
         return list(self.potential_view["Name"].values)
 
     @property
@@ -225,34 +253,29 @@
         return self._potential
 
     def get_kpoints(self):
         return self.input.KpointFolding
 
     def get_version_float(self):
         version_str = self.executable.version.split("_")[0]
-        version_float = float(
-            version_str.split(".")[0]
-        )
+        version_float = float(version_str.split(".")[0])
         if len(version_str.split(".")) > 1:
-            version_float += float(
-                "0." + "".join(version_str.split(".")[1:])
-                )
+            version_float += float("0." + "".join(version_str.split(".")[1:]))
         return version_float
 
     def set_input_to_read_only(self):
         """
         This function enforces read-only mode for the input classes,
         but it has to be implemented in the individual classes.
         """
         super(SphinxBase, self).set_input_to_read_only()
         self.input.read_only = True
 
     def get_scf_group(
-        self, maxSteps=None, keepRhoFixed=False, dEnergy=None,
-        algorithm="blockCCG"
+        self, maxSteps=None, keepRhoFixed=False, dEnergy=None, algorithm="blockCCG"
     ):
         """
         SCF group setting for SPHInX
         for all args refer to calc_static or calc_minimize
         """
 
         scf_group = Group()
@@ -277,20 +300,26 @@
             scf_group["dEnergy"] = self.input["Ediff"] / HARTREE_TO_EV
         else:
             scf_group["dEnergy"] = str(dEnergy)
         if maxSteps is None:
             scf_group["maxSteps"] = str(self.input["Estep"])
         else:
             scf_group["maxSteps"] = str(maxSteps)
-        if 'preconditioner' in self.input and self.input['preconditioner'] != 'KERKER':
-            scf_group.create_group("preconditioner")["type"] = self.input['preconditioner']
+        if "preconditioner" in self.input and self.input["preconditioner"] != "KERKER":
+            scf_group.create_group("preconditioner")["type"] = self.input[
+                "preconditioner"
+            ]
         else:
-            scf_group.create_group("preconditioner")["type"] = 'KERKER'
-            scf_group.preconditioner.set_parameter('scaling', self.input["rhoResidualScaling"])
-            scf_group.preconditioner.set_parameter('spinScaling', self.input["spinResidualScaling"])
+            scf_group.create_group("preconditioner")["type"] = "KERKER"
+            scf_group.preconditioner.set_parameter(
+                "scaling", self.input["rhoResidualScaling"]
+            )
+            scf_group.preconditioner.set_parameter(
+                "spinScaling", self.input["spinResidualScaling"]
+            )
         scf_group.create_group(algorithm)
         if "maxStepsCCG" in self.input:
             scf_group[algorithm]["maxStepsCCG"] = self.input["maxStepsCCG"]
         if "blockSize" in self.input and algorithm == "blockCCG":
             scf_group[algorithm]["blockSize"] = self.input["blockSize"]
         if "nSloppy" in self.input and algorithm == "blockCCG":
             scf_group[algorithm]["nSloppy"] = self.input["nSloppy"]
@@ -302,84 +331,78 @@
         """
         create a SPHInX Group object based on self.structure
 
         Args:
             keep_angstrom (bool): Store distances in Angstroms or Bohr
         """
         if keep_angstrom:
-            structure_group = Group( {"cell": np.array(self.structure.cell)} )
+            structure_group = Group({"cell": np.array(self.structure.cell)})
         else:
-            structure_group = Group( {
+            structure_group = Group(
+                {
                     "cell": np.array(self.structure.cell * 1 / BOHR_TO_ANGSTROM),
-            })
+                }
+            )
         if "selective_dynamics" in self.structure._tag_list.keys():
-            selective_dynamics_list = \
-                self.structure.selective_dynamics.list()
+            selective_dynamics_list = self.structure.selective_dynamics.list()
         else:
-            selective_dynamics_list = [3 * [False]] * len(
-                self.structure.positions)
+            selective_dynamics_list = [3 * [False]] * len(self.structure.positions)
         species = structure_group.create_group("species")
         for elm_species in self.structure.get_species_objects():
             if elm_species.Parent:
                 element = elm_species.Parent
             else:
                 element = elm_species.Abbreviation
-            species.append(
-                Group({"element": '"' + str(element) + '"'})
-            )
+            species.append(Group({"element": '"' + str(element) + '"'}))
             elm_list = np.array(
-                self.structure.get_chemical_symbols() ==
-                elm_species.Abbreviation
+                self.structure.get_chemical_symbols() == elm_species.Abbreviation
             )
             atom_group = species[-1].create_group("atom")
             for elm_pos, elm_magmon, selective in zip(
                 self.structure.positions[elm_list],
-                np.array(self.structure.get_initial_magnetic_moments())[
-                    elm_list],
+                np.array(self.structure.get_initial_magnetic_moments())[elm_list],
                 np.array(selective_dynamics_list)[elm_list],
             ):
                 atom_group.append(Group())
                 if self._spin_enabled:
-                    atom_group[-1]["label"] \
-                        = '"spin_' + str(elm_magmon) + '"'
+                    atom_group[-1]["label"] = '"spin_' + str(elm_magmon) + '"'
                 if keep_angstrom:
                     atom_group[-1]["coords"] = np.array(elm_pos)
                 else:
-                    atom_group[-1]["coords"] = \
-                        np.array(elm_pos * 1 / BOHR_TO_ANGSTROM)
+                    atom_group[-1]["coords"] = np.array(elm_pos * 1 / BOHR_TO_ANGSTROM)
                 if all(selective):
                     atom_group[-1]["movable"] = True
                 elif any(selective):
                     for ss, xx in zip(selective, ["X", "Y", "Z"]):
                         if ss:
                             atom_group[-1]["movable" + xx] = True
         if not self.fix_symmetry:
-            structure_group.symmetry = Group({
-                "operator": {
-                    "S": "[[1,0,0],[0,1,0],[0,0,1]]"
-            }})
+            structure_group.symmetry = Group(
+                {"operator": {"S": "[[1,0,0],[0,1,0],[0,0,1]]"}}
+            )
         return structure_group
 
     def load_default_input(self):
         """
         Set defaults for generic parameters and create SPHInX input groups.
         """
 
-        sph = self.input.create_group('sphinx')
-        sph.create_group('pawPot')
-        sph.create_group('structure')
-        sph.create_group('basis')
-        sph.create_group('PAWHamiltonian')
-        sph.create_group('initialGuess')
-        sph.create_group('main')
+        sph = self.input.create_group("sphinx")
+        sph.create_group("pawPot")
+        sph.create_group("structure")
+        sph.create_group("basis")
+        sph.create_group("PAWHamiltonian")
+        sph.create_group("initialGuess")
+        sph.create_group("main")
 
         self.input.EnCut = 340
         self.input.KpointCoords = [0.5, 0.5, 0.5]
         self.input.KpointFolding = [4, 4, 4]
         self.input.EmptyStates = "auto"
+        self.input.MethfesselPaxton = 1
         self.input.Sigma = 0.2
         self.input.Xcorr = "PBE"
         self.input.VaspPot = False
         self.input.Estep = 100
         self.input.Ediff = 1.0e-4
         self.input.WriteWaves = True
         self.input.KJxc = False
@@ -397,17 +420,17 @@
         Build + load the structure group based on self.structure
 
         Args:
             keep_angstrom (bool): Store distances in Angstroms or Bohr
         """
         self.input.sphinx.structure = self.get_structure_group(
             keep_angstrom=keep_angstrom
-            )
+        )
 
-    def load_species_group(self, check_overlap=True, potformat='VASP'):
+    def load_species_group(self, check_overlap=True, potformat="VASP"):
         """
         Build the species Group object based on self.structure
 
         Args:
             check_overlap (bool): Whether to check overlap
                 (see set_check_overlap)
             potformat (str): type of pseudopotentials that will be
@@ -417,122 +440,130 @@
         self.input.sphinx.pawPot = Group({"species": []})
         for species_obj in self.structure.get_species_objects():
             if species_obj.Parent is not None:
                 elem = species_obj.Parent
             else:
                 elem = species_obj.Abbreviation
             if potformat == "JTH":
-                self.input.sphinx.pawPot["species"].append(Group({
+                self.input.sphinx.pawPot["species"].append(
+                    Group(
+                        {
                             "name": '"' + elem + '"',
                             "potType": '"AtomPAW"',
                             "element": '"' + elem + '"',
                             "potential": f'"{elem}_GGA.atomicdata"',
-                }))
+                        }
+                    )
+                )
             elif potformat == "VASP":
-                self.input.sphinx.pawPot["species"].append(Group({
+                self.input.sphinx.pawPot["species"].append(
+                    Group(
+                        {
                             "name": '"' + elem + '"',
                             "potType": '"VASP"',
                             "element": '"' + elem + '"',
                             "potential": '"' + elem + "_POTCAR" + '"',
-                }))
+                        }
+                    )
+                )
             else:
-                raise ValueError('Potential must be JTH or VASP')
+                raise ValueError("Potential must be JTH or VASP")
         if not check_overlap:
             self.input.sphinx.pawPot["species"][-1]["checkOverlap"] = "false"
         if self.input["KJxc"]:
             self.input.sphinx.pawPot["kjxc"] = True
 
     def load_main_group(self):
         """
         Load the main Group.
 
         The group is populated based on the type of calculation and settings in
         the self.input.
         """
 
-        if len(self.restart_file_list) != 0 \
-        and not self._generic_input["restart_for_band_structure"]:
-            self.input.sphinx.main.get("scfDiag", create = True).append(
-                self.get_scf_group(
-                    maxSteps=10, keepRhoFixed=True, dEnergy=1.0e-4
-                )
+        if (
+            len(self.restart_file_list) != 0
+            and not self._generic_input["restart_for_band_structure"]
+        ):
+            self.input.sphinx.main.get("scfDiag", create=True).append(
+                self.get_scf_group(maxSteps=10, keepRhoFixed=True, dEnergy=1.0e-4)
             )
         if "Istep" in self.input:
-            optimizer = 'linQN'
+            optimizer = "linQN"
             if self.input.use_on_the_fly_cg_optimization:
-                optimizer = 'ricQN'
-            self.input.sphinx.main[optimizer] = Group(table_name = "input")
+                optimizer = "ricQN"
+            self.input.sphinx.main[optimizer] = Group(table_name="input")
             self.input.sphinx.main[optimizer]["maxSteps"] = str(self.input["Istep"])
-            self.input.sphinx.main[optimizer]["maxStepLength"] = str(0.1/BOHR_TO_ANGSTROM)
-            if "dE" in self.input and "dF" in self.input:
-                self.input["dE"] = 1e-3
+            self.input.sphinx.main[optimizer]["maxStepLength"] = str(
+                0.1 / BOHR_TO_ANGSTROM
+            )
             if "dE" in self.input:
                 self.input.sphinx.main[optimizer]["dEnergy"] = str(
                     self.input["dE"] / HARTREE_TO_EV
-                    )
+                )
             if "dF" in self.input:
                 self.input.sphinx.main[optimizer]["dF"] = str(
                     self.input["dF"] / HARTREE_OVER_BOHR_TO_EV_OVER_ANGSTROM
                 )
             self.input.sphinx.main[optimizer].create_group("bornOppenheimer")
-            self.input.sphinx.main[optimizer]['bornOppenheimer']["scfDiag"] = self.get_scf_group()
+            self.input.sphinx.main[optimizer]["bornOppenheimer"][
+                "scfDiag"
+            ] = self.get_scf_group()
         else:
-            scf = self.input.sphinx.main.get("scfDiag", create = True)
+            scf = self.input.sphinx.main.get("scfDiag", create=True)
             if self._generic_input["restart_for_band_structure"]:
                 scf.append(self.get_scf_group(keepRhoFixed=True))
             else:
                 scf.append(self.get_scf_group())
             if self.executable.version is not None:
                 if self.get_version_float() > 2.5:
-                    self.input.sphinx.main.create_group("evalForces")["file"] = \
-                            '"relaxHist.sx"'
+                    self.input.sphinx.main.create_group("evalForces")[
+                        "file"
+                    ] = '"relaxHist.sx"'
             else:
                 warnings.warn("executable version could not be identified")
 
     def load_basis_group(self):
         """
         Load the basis Group.
 
         The group is populated using setdefault to avoid
         overwriting values that were previously (intentionally)
         modified.
         """
-        self.input.sphinx.basis.setdefault("eCut", self.input["EnCut"]/RYDBERG_TO_EV)
+        self.input.sphinx.basis.setdefault("eCut", self.input["EnCut"] / RYDBERG_TO_EV)
         self.input.sphinx.basis.get("kPoint", create=True)
         if "KpointCoords" in self.input:
             self.input.sphinx.basis.kPoint.setdefault(
-                "coords",
-                np.array(self.input["KpointCoords"])
+                "coords", np.array(self.input["KpointCoords"])
             )
         self.input.sphinx.basis.kPoint.setdefault("weight", 1)
         self.input.sphinx.basis.kPoint.setdefault("relative", True)
         if "KpointFolding" in self.input:
             self.input.sphinx.basis.setdefault(
-                "folding",
-                np.array(self.input["KpointFolding"])
+                "folding", np.array(self.input["KpointFolding"])
             )
-        self.input.sphinx.basis.setdefault(
-            "saveMemory",
-            self.input["SaveMemory"]
-        )
+        self.input.sphinx.basis.setdefault("saveMemory", self.input["SaveMemory"])
 
     def load_hamilton_group(self):
         """
         Load the PAWHamiltonian Group.
 
         The group is populated using setdefault to avoid
         overwriting values that were previously (intentionally)
         modified.
         """
         self.input.sphinx.PAWHamiltonian.setdefault(
             "nEmptyStates", self.input["EmptyStates"]
-            )
-        self.input.sphinx.PAWHamiltonian.setdefault(
-            "ekt", self.input["Sigma"]
-            )
+        )
+        self.input.sphinx.PAWHamiltonian.setdefault("ekt", self.input["Sigma"])
+        for k in ["MethfesselPaxton", "FermiDirac"]:
+            if k in self.input.list_nodes():
+                self.input.sphinx.PAWHamiltonian.setdefault(k, self.input[k])
+                break
         self.input.sphinx.PAWHamiltonian.setdefault("xc", self.input["Xcorr"])
         self.input.sphinx.PAWHamiltonian["spinPolarized"] = self._spin_enabled
 
     def load_guess_group(self, update_spins=True):
         """
         Load the initialGuess Group.
 
@@ -551,57 +582,60 @@
             if "rho.sxb" in ff.split("/")[-1]:
                 charge_density_file = ff
         wave_function_file = None
         for ff in self.restart_file_list:
             if "waves.sxb" in ff.split("/")[-1]:
                 wave_function_file = ff
 
-        self.input.sphinx.initialGuess.setdefault("waves", Group())
-        self.input.sphinx.initialGuess.waves.setdefault("lcao", Group())
-        self.input.sphinx.initialGuess.waves.setdefault("pawBasis", True)
-        if wave_function_file is not None:
-            self.input.sphinx.initialGuess.setdefault("exchange", Group())
-            self.input.sphinx.initialGuess.exchange.setdefault(
-                "file", '"' + wave_function_file + '"'
-            )
+        # introduce short alias for initialGuess group
+        guess = self.input.sphinx.initialGuess
+
+        guess.setdefault("waves", Group())
+        guess.waves.setdefault("pawBasis", True)
+        if wave_function_file is None:
+            guess.waves.setdefault("lcao", Group())
+        else:
+            guess.waves.setdefault("file", '"' + wave_function_file + '"')
+            # TODO: only for hybrid functionals
+            guess.setdefault("exchange", Group())
+            guess.exchange.setdefault("file", '"' + wave_function_file + '"')
+
+        guess.setdefault("rho", Group())
         if charge_density_file is None:
-            self.input.sphinx.initialGuess.setdefault("rho", Group({"atomicOrbitals": True}))
-        else:
-            self.input.sphinx.initialGuess.setdefault(
-                "rho", Group({"file": '"' + charge_density_file + '"'})
-                )
-        if self._spin_enabled:
-            if any(
-                [
-                    True
-                    if isinstance(spin, list) or isinstance(spin, np.ndarray)
-                    else False
-                    for spin in self.structure.get_initial_magnetic_moments()
-                ]
-            ):
-                raise ValueError("SPHInX only supports collinear spins.")
+            if wave_function_file is None:
+                guess.rho.setdefault("atomicOrbitals", True)
+                if self._spin_enabled:
+                    init_spins = self.structure.get_initial_magnetic_moments()
+                    # --- validate that initial spin moments are scalar
+                    for spin in init_spins:
+                        if isinstance(spin, list) or isinstance(spin, np.ndarray):
+                            raise ValueError("SPHInX only supports collinear spins.")
+                    guess.rho.get("atomicSpin", create=True)
+                    if update_spins:
+                        guess.rho.atomicSpin.clear()
+                    # --- create initial spins if needed
+                    if len(guess.rho.atomicSpin) == 0:
+                        # set initial spin via label for each unique value of spin
+                        # dict.from_keys (...).keys () deduplicates
+                        for spin in dict.fromkeys(init_spins).keys():
+                            guess.rho["atomicSpin"].append(
+                                Group(
+                                    {
+                                        "label": '"spin_' + str(spin) + '"',
+                                        "spin": str(spin),
+                                    }
+                                )
+                            )
             else:
-                rho = self.input.sphinx.initialGuess.rho
-                rho.get("atomicSpin", create = True)
-                if update_spins:
-                    rho.atomicSpin.clear()
-                if len(rho.atomicSpin) == 0:
-                    for spin in self.structure.get_initial_magnetic_moments()[
-                        self.id_pyi_to_spx
-                    ]:
-                        rho["atomicSpin"].append(
-                            Group({
-                                "label": '"spin_' + str(spin) + '"',
-                                "spin": str(spin)
-                            })
-                        )
+                guess.rho.setdefault("fromWaves", True)
+        else:
+            guess.rho.setdefault("file", '"' + charge_density_file + '"')
 
-        if "noWavesStorage" not in self.input.sphinx.initialGuess:
-            self.input.sphinx.initialGuess["noWavesStorage"] = \
-                    not self.input["WriteWaves"]
+        if "noWavesStorage" not in guess:
+            guess["noWavesStorage"] = not self.input["WriteWaves"]
 
     def calc_static(
         self,
         electronic_steps=100,
         algorithm=None,
         retain_charge_density=False,
         retain_electrostatic_potential=False,
@@ -640,28 +674,32 @@
         max_iter=None,
         pressure=None,
         algorithm=None,
         retain_charge_density=False,
         retain_electrostatic_potential=False,
         ionic_energy=None,
         ionic_forces=None,
-        ionic_energy_tolerance=0.0,
-        ionic_force_tolerance=1.0e-2,
+        ionic_energy_tolerance=None,
+        ionic_force_tolerance=None,
         volume_only=False,
     ):
         """
         Setup the hamiltonian to perform ionic relaxations.
 
         The convergence goal can be set using either the
         ionic_energy_tolerance as a limit for fluctuations in energy or the
         ionic_force_tolerance.
 
         Loads defaults for all SPHInX input groups, including a
         ricQN-based main Group.
 
+        .. warning::
+            Sphinx does not support volume minimizations!  Calling this method with `pressure` or `volume_only` results
+            in an error.
+
         Args:
             retain_electrostatic_potential:
             retain_charge_density:
             algorithm:
             pressure:
             max_iter:
             electronic_steps (int): maximum number of electronic steps
@@ -673,15 +711,15 @@
                                   energy (optional)
             ionic_forces (float): convergence goal in terms of
                                   forces (depreciated use ionic_force_tolerance instead)
             ionic_force_tolerance (float): convergence goal in terms of
                                   forces (optional)
             volume_only (bool):
         """
-        if pressure is not None:
+        if pressure is not None or volume_only:
             raise NotImplementedError(
                 "pressure minimization is not implemented in SPHInX"
             )
         if electronic_steps is not None:
             self.input["Estep"] = electronic_steps
         if ionic_steps is not None:
             self.input["Istep"] = ionic_steps
@@ -713,15 +751,15 @@
         self,
         temperature=None,
         n_ionic_steps=1000,
         n_print=1,
         time_step=1.0,
         retain_charge_density=False,
         retain_electrostatic_potential=False,
-        **kwargs
+        **kwargs,
     ):
         raise NotImplementedError("calc_md() not implemented in SPHInX.")
 
     def restart_for_band_structure_calculations(self, job_name=None):
         """
         Restart a new job created from an existing calculation
         by reading the charge density for band structures.
@@ -729,24 +767,19 @@
         Args:
             job_name (str/None): Job name
 
         Returns:
             pyiron_atomistics.sphinx.sphinx.sphinx: new job instance
         """
         return self.restart_from_charge_density(
-            job_name=job_name,
-            job_type=None,
-            band_structure_calc=True
+            job_name=job_name, band_structure_calc=True
         )
 
     def restart_from_charge_density(
-            self,
-            job_name=None,
-            job_type="Sphinx",
-            band_structure_calc=False
+        self, job_name=None, job_type="Sphinx", band_structure_calc=False
     ):
         """
         Restart a new job created from an existing calculation
         by reading the charge density.
 
         Args:
             job_name (str/None): Job name
@@ -757,24 +790,34 @@
         Returns:
             pyiron_atomistics.sphinx.sphinx.sphinx: new job instance
         """
         ham_new = self.restart(
             job_name=job_name,
             job_type=job_type,
             from_wave_functions=False,
-            from_charge_density=True
+            from_charge_density=True,
         )
         if band_structure_calc:
             ham_new._generic_input["restart_for_band_structure"] = True
+            # --- clean up minimization related settings
+            for setting in ["Istep", "dF", "dE"]:
+                if setting in ham_new.input:
+                    del ham_new.input[setting]
+            # remove optimization-related stuff from GenericDFTJob
+            super(SphinxBase, self).calc_static()
+            # --- recreate main group
+            del ham_new.input.sphinx["main"]
+            ham_new.input.sphinx.create_group("main")
+            ham_new.load_main_group()
         return ham_new
 
     def restart_from_wave_functions(
-            self,
-            job_name=None,
-            job_type="Sphinx",
+        self,
+        job_name=None,
+        job_type="Sphinx",
     ):
         """
         Restart a new job created from an existing calculation
         by reading the wave functions.
 
         Args:
             job_name (str): Job name
@@ -784,118 +827,137 @@
         Returns:
             pyiron_atomistics.sphinx.sphinx.sphinx: new job instance
         """
         return self.restart(
             job_name=job_name,
             job_type=job_type,
             from_wave_functions=True,
-            from_charge_density=False
+            from_charge_density=False,
         )
 
     def restart(
         self,
         job_name=None,
         job_type=None,
         from_charge_density=True,
         from_wave_functions=True,
     ):
         if not self.status.finished and not self.is_compressed():
             # self.decompress()
             with warnings.catch_warnings(record=True) as w:
                 try:
                     self.collect_output()
-                except AssertionError:
-                    from_charge_density=False
-                    from_wave_functions=False
+                except AssertionError as orig_error:
+                    if from_charge_density or from_wave_functions:
+                        raise AssertionError(
+                            orig_error.message
+                            + "\nCowardly refusing to use density or wavefunctions for restart.\n"
+                            + "Solution: set from_charge_density and from_wave_functions to False."
+                        )
                 if len(w) > 0:
                     self.status.not_converged = True
-        new_job = super(SphinxBase, self).restart(
-            job_name=job_name, job_type=job_type
-        )
+        new_job = super(SphinxBase, self).restart(job_name=job_name, job_type=job_type)
 
-        new_job.input = self.input
+        new_job.input = self.input.copy()
 
+        recreate_guess = False
         if from_charge_density and os.path.isfile(
             posixpath.join(self.working_directory, "rho.sxb")
         ):
-            new_job.restart_file_list.append(posixpath.join(self.working_directory, "rho.sxb"))
+            new_job.restart_file_list.append(
+                posixpath.join(self.working_directory, "rho.sxb")
+            )
+            del new_job.input.sphinx.initialGuess["rho"]
+            recreate_guess = True
 
         elif from_charge_density:
             self._logger.warning(
                 msg=f"A charge density from job: {self.job_name} "
                 + "is not generated and therefore it can't be read."
             )
         if from_wave_functions and os.path.isfile(
             posixpath.join(self.working_directory, "waves.sxb")
         ):
-            new_job.restart_file_list.append(posixpath.join(self.working_directory, "waves.sxb"))
+            new_job.restart_file_list.append(
+                posixpath.join(self.working_directory, "waves.sxb")
+            )
+            try:
+                del new_job.input.sphinx.initialGuess["rho"]
+            except KeyError:
+                pass
+            del new_job.input.sphinx.initialGuess["waves"]
+            recreate_guess = True
+
         elif from_wave_functions:
             self._logger.warning(
                 msg="No wavefunction file (waves.sxb) was found for "
                 + f"job {self.job_name} in {self.working_directory}."
             )
+        if recreate_guess:
+            new_job.load_guess_group()
         return new_job
 
+    def relocate_hdf5(self, h5_path=None):
+        self.input._force_load()
+        super().relocate_hdf5(h5_path=h5_path)
+
     def to_hdf(self, hdf=None, group_name=None):
         """
         Stores the instance attributes into the hdf5 file
 
         Args:
             hdf (str): Path to the hdf5 file
             group_name (str): Name of the group which contains the object
         """
         super(SphinxBase, self).to_hdf(hdf=hdf, group_name=group_name)
         self._structure_to_hdf()
         with self._hdf5.open("input") as hdf:
             self.input.to_hdf(hdf)
-        self._output_parser.to_hdf(self._hdf5)
+        self.output.to_hdf(self._hdf5)
 
     def from_hdf(self, hdf=None, group_name=None):
         """
         Recreates instance from the hdf5 file
 
         Args:
             hdf (str): Path to the hdf5 file
             group_name (str): Name of the group which contains the object
         """
         if "HDF_VERSION" not in self._hdf5.keys():
             from pyiron_base import GenericParameters
+
             super(SphinxBase, self).from_hdf(hdf=hdf, group_name=group_name)
             self._structure_from_hdf()
-            gp = GenericParameters(table_name = "input")
+            gp = GenericParameters(table_name="input")
             gp.from_hdf(self._hdf5)
             for k in gp.keys():
                 self.input[k] = gp[k]
-            if self.status.finished:
-                self._output_parser.from_hdf(self._hdf5)
         elif self._hdf5["HDF_VERSION"] == "0.1.0":
             super(SphinxBase, self).from_hdf(hdf=hdf, group_name=group_name)
             self._structure_from_hdf()
             with self._hdf5.open("input") as hdf:
-                self.input.from_hdf(hdf, group_name = "parameters")
-            if self.status.finished:
-                self._output_parser.from_hdf(self._hdf5)
+                self.input.from_hdf(hdf, group_name="parameters")
+        self.output.from_hdf(self._hdf5)
 
     def from_directory(self, directory, file_name="structure.sx"):
         try:
             if not self.status.finished:
-
                 file_path = posixpath.join(directory, file_name)
                 if os.path.isfile(file_path):
                     self.structure = read_atoms(file_path)
                 else:
                     raise ValueError(
                         f"File {file_path} not found. "
                         "Please double check the directory and file name."
                     )
 
-                self._output_parser.collect(directory=directory)
+                self.output.collect(directory=directory)
                 self.to_hdf(self._hdf5)
             else:
-                self._output_parser.from_hdf(self._hdf5)
+                self.output.from_hdf(self._hdf5)
             self.status.finished = True
         except Exception as err:
             print(err)
             self.status.aborted = True
 
     def set_check_overlap(self, check_overlap=True):
         """
@@ -927,79 +989,88 @@
         n_pulay_steps=None,
         density_mixing_parameter=None,
         spin_mixing_parameter=None,
         density_residual_scaling=None,
         spin_residual_scaling=None,
     ):
         """
-            Further information can be found on the website:
-            https://sxrepo.mpie.de
+        Further information can be found on the website:
+        https://sxrepo.mpie.de
         """
         method_list = ["PULAY", "KERKER", "LINEAR"]
         if method is not None and method.upper() not in method_list:
             raise ValueError("Mixing method has to be PULAY or KERKER")
         if method is not None:
-            self.input["mixingMethod"] = method.upper().replace('KERKER', 'LINEAR')
+            self.input["mixingMethod"] = method.upper().replace("KERKER", "LINEAR")
         if n_pulay_steps is not None:
             self.input["nPulaySteps"] = int(n_pulay_steps)
         if density_mixing_parameter is not None:
             if density_mixing_parameter > 1.0 or density_mixing_parameter < 0:
                 raise ValueError(
-                    "density_mixing_parameter has to be between 0 and 1 "+
-                    "(default value is 1)"
+                    "density_mixing_parameter has to be between 0 and 1 "
+                    + "(default value is 1)"
                 )
             self.input["rhoMixing"] = density_mixing_parameter
         if spin_mixing_parameter is not None:
             if spin_mixing_parameter > 1.0 or spin_mixing_parameter < 0:
                 raise ValueError(
-                    "spin_mixing_parameter has to be between 0 and 1 "+
-                    "(default value is 1)"
+                    "spin_mixing_parameter has to be between 0 and 1 "
+                    + "(default value is 1)"
                 )
             self.input["spinMixing"] = spin_mixing_parameter
         if density_residual_scaling is not None:
             if density_residual_scaling <= 0:
-                raise ValueError('density_residual_scaling must be a positive value')
+                raise ValueError("density_residual_scaling must be a positive value")
             self.input["rhoResidualScaling"] = density_residual_scaling
         if spin_residual_scaling is not None:
             if spin_residual_scaling <= 0:
-                raise ValueError('spin_residual_scaling   must be a positive value')
+                raise ValueError("spin_residual_scaling   must be a positive value")
             self.input["spinResidualScaling"] = spin_residual_scaling
+
     set_mixing_parameters.__doc__ = (
-        GenericDFTJob.set_mixing_parameters.__doc__
-        + set_mixing_parameters.__doc__
+        GenericDFTJob.set_mixing_parameters.__doc__ + set_mixing_parameters.__doc__
     )
 
-    def set_occupancy_smearing(self, smearing=None, width=None):
+    def set_occupancy_smearing(self, smearing=None, width=None, order=1):
         """
         Set how the finite temperature smearing is applied in
         determining partial occupancies
 
         Args:
-            smearing (str): Type of smearing (only fermi is
-                            implemented anything else will be ignored)
+            smearing (str): Type of smearing, 'FermiDirac' or 'MethfesselPaxton'
             width (float): Smearing width (eV) (default: 0.2)
+            order (int): Smearing order
         """
-        if smearing is not None and not isinstance(smearing, str):
-            raise ValueError(
-                "Smearing must be a string"
-            )
+        if smearing is not None:
+            if not isinstance(smearing, str):
+                raise ValueError("Smearing must be a string")
+            if smearing.lower().startswith("meth"):
+                self.input.MethfesselPaxton = order
+                if "FermiDirac" in self.input.list_nodes():
+                    del self.input["FermiDirac"]
+            elif smearing.lower().startswith("fermi"):
+                self.input.FermiDirac = order
+                if "MethfesselPaxton" in self.input.list_nodes():
+                    del self.input["MethfesselPaxton"]
         if width is not None and width < 0:
             raise ValueError("Smearing value must be a float >= 0")
         if width is not None:
             self.input["Sigma"] = width
 
-    @deprecate(ionic_forces="Use ionic_force_tolerance",
-               ionic_energy="use ionic_energy_tolerance")
+    @deprecate(
+        ionic_forces="Use ionic_force_tolerance",
+        ionic_energy="use ionic_energy_tolerance",
+    )
     def set_convergence_precision(
-            self,
-            ionic_energy_tolerance=None,
-            ionic_force_tolerance=None,
-            ionic_energy=None,
-            electronic_energy=None,
-            ionic_forces=None
+        self,
+        ionic_energy_tolerance=None,
+        ionic_force_tolerance=None,
+        ionic_energy=None,
+        electronic_energy=None,
+        ionic_forces=None,
     ):
         """
         Sets the electronic and ionic convergence precision.
 
         For ionic convergence either the energy or the force
         precision is required.
 
@@ -1012,28 +1083,32 @@
             ionic_forces (float): Ionic force convergence precision
                                   (depreciated use ionic_force_tolerance instead)
             ionic_force_tolerance (float): Ionic force convergence precision
         """
         if ionic_forces is not None:
             ionic_force_tolerance = ionic_forces
         if ionic_energy is not None:
-            ionic_energy_tolerance =ionic_energy
+            ionic_energy_tolerance = ionic_energy
         assert (
             ionic_energy_tolerance is None or ionic_energy_tolerance > 0
         ), "ionic_energy_tolerance must be a positive float"
         assert (
             ionic_force_tolerance is None or ionic_force_tolerance > 0
         ), "ionic_force_tolerance must be a positive float"
         assert (
             electronic_energy is None or electronic_energy > 0
         ), "electronic_energy must be a positive float"
         if ionic_energy_tolerance is not None or ionic_force_tolerance is not None:
+            # self.input["dE"] = ionic_energy_tolerance
+            # self.input["dF"] = ionic_force_tolerance
             print("Setting calc_minimize")
-            self.calc_minimize(ionic_energy_tolerance=ionic_energy_tolerance,
-                               ionic_force_tolerance=ionic_force_tolerance)
+            self.calc_minimize(
+                ionic_energy_tolerance=ionic_energy_tolerance,
+                ionic_force_tolerance=ionic_force_tolerance,
+            )
         if electronic_energy is not None:
             self.input["Ediff"] = electronic_energy
 
     def set_empty_states(self, n_empty_states=None):
         """
         Function to set the number of empty states.
 
@@ -1055,17 +1130,15 @@
             and 1.5*NIONS+3 for magnetic systems
         """
         if n_empty_states is None:
             # will be converted later; see load_default_groups
             self.input["EmptyStates"] = "auto"
         else:
             if n_empty_states < 0:
-                raise ValueError(
-                    "Number of empty states must be greater than 0"
-                    )
+                raise ValueError("Number of empty states must be greater than 0")
             self.input["EmptyStates"] = n_empty_states
         self.input.sphinx.PAWHamiltonian.nEmptyStates = self.input["EmptyStates"]
 
     def _set_kpoints(
         self,
         mesh=None,
         scheme="MP",
@@ -1096,102 +1169,105 @@
             n_path (int): Number of points per trace part for line mode
             path_name (str): Name of high symmetry path used for band
                              structure calculations.
         """
         if not isinstance(symmetry_reduction, bool):
             raise ValueError("symmetry_reduction has to be a boolean")
         if manual_kpoints is not None:
-            raise ValueError("manual_kpoints is not yet implemented in "
-                + "Pyiron for SPHInX")
+            raise ValueError(
+                "manual_kpoints is not yet implemented in pyiron for SPHInX"
+            )
         if weights is not None:
             raise ValueError(
-                "manual weights are not yet implmented in Pyiron for "
-                + "SPHInX"
-                )
+                "manual weights are not yet implmented in Pyiron for " + "SPHInX"
+            )
 
         if scheme == "MP":
             # Remove kPoints and set kPoint
             if "kPoints" in self.input.sphinx.basis:
                 del self.input.sphinx.basis.kPoints
             self.input.sphinx.basis.get("kPoint", create=True)
             if mesh is not None:
                 self.input["KpointFolding"] = list(mesh)
-                self.input.sphinx.basis["folding"] = np.array(self.input["KpointFolding"])
+                self.input.sphinx.basis["folding"] = np.array(
+                    self.input["KpointFolding"]
+                )
             if center_shift is not None:
                 self.input["KpointCoords"] = list(center_shift)
-                self.input.sphinx.basis["kPoint"]["coords"] = \
-                    np.array(self.input["KpointCoords"])
+                self.input.sphinx.basis["kPoint"]["coords"] = np.array(
+                    self.input["KpointCoords"]
+                )
                 self.input.sphinx.basis.kPoint["weight"] = 1
                 self.input.sphinx.basis.kPoint["relative"] = True
 
         elif scheme == "Line":
             # Remove Kpoint and set Kpoints
 
             if "kPoint" in self.input.sphinx.basis:
                 del self.input.sphinx.basis["kPoint"]
                 del self.input["KpointFolding"]
                 del self.input["KpointCoords"]
                 if "folding" in self.input.sphinx.basis:
-                    del self.input.sphinx.basis['folding']
+                    del self.input.sphinx.basis["folding"]
             if n_path is None and self._generic_input["n_path"] is None:
                 raise ValueError("'n_path' has to be defined")
             if n_path is None:
                 n_path = self._generic_input["n_path"]
             else:
                 self._generic_input["n_path"] = n_path
 
             if self.structure.get_high_symmetry_points() is None:
-                raise ValueError(
-                    "no 'high_symmetry_points' defined for 'structure'."
-                )
+                raise ValueError("no 'high_symmetry_points' defined for 'structure'.")
 
             if path_name is None and self._generic_input["path_name"] is None:
                 raise ValueError("'path_name' has to be defined")
             if path_name is None:
                 path_name = self._generic_input["path_name"]
             else:
                 self._generic_input["path_name"] = path_name
 
             try:
                 path = self.structure.get_high_symmetry_path()[path_name]
             except KeyError:
-                raise AssertionError(
-                    "'{}' is not a valid path!".format(path_name)
-                    )
+                raise AssertionError("'{}' is not a valid path!".format(path_name))
 
             def make_point(point, n_path):
-                return Group({
-                    "coords": np.array(self.structure.get_high_symmetry_points()[point]),
-                    "nPoints": n_path,
-                    "label": "\"{}\"".format(point.replace("'", "p"))
-                })
+                return Group(
+                    {
+                        "coords": np.array(
+                            self.structure.get_high_symmetry_points()[point]
+                        ),
+                        "nPoints": n_path,
+                        "label": '"{}"'.format(point.replace("'", "p")),
+                    }
+                )
 
             kpoints = Group({"relative": True})
             kpoints["from"] = make_point(path[0][0], None)
             # from nodes are not supposed to have a nPoints attribute
             del kpoints["from/nPoints"]
 
             kpoints.create_group("to").append(make_point(path[0][1], n_path))
 
             for segment in path[1:]:
                 # if the last node on the so far is not the same as the first
                 # node of this path segment, then we need to insert another
                 # node into the path to alert sphinx that we want a cut in our
                 # band structure (n_path = 0)
                 if '"{}"'.format(segment[0]) != kpoints.to[-1].label:
-                    kpoints["to"].append(
-                            make_point(segment[0], 0)
-                    )
+                    kpoints["to"].append(make_point(segment[0], 0))
 
                 kpoints["to"].append(make_point(segment[1], n_path))
 
             self.input.sphinx.basis["kPoints"] = kpoints
         else:
-            raise ValueError("only Monkhorst-Pack mesh and Line mode\
-                are currently implemented in Pyiron for SPHInX")
+            raise ValueError(
+                "only Monkhorst-Pack mesh and Line mode\
+                are currently implemented in Pyiron for SPHInX"
+            )
 
     def load_default_groups(self):
         """
         Populates input groups with the default values.
 
         Nearly every default simply points to a variable stored in
         self.input.
@@ -1202,35 +1278,37 @@
         the job is run. These groups can be synced to job.structure
         at any time using job.load_structure_group() and
         job.load_species_group().
         """
 
         if self.structure is None:
             raise AssertionError(
-                f"{self.job_name} has not been assigned " +\
-                "a structure. Please load one first (e.g. " +\
-                f"{self.job_name}.structure = ...)")
+                f"{self.job_name} has not been assigned "
+                + "a structure. Please load one first (e.g. "
+                + f"{self.job_name}.structure = ...)"
+            )
 
         if self.input["EmptyStates"] == "auto":
             if self._spin_enabled:
-                self.input["EmptyStates"] = int(
-                    1.5 * len(self.structure) + 3)
+                self.input["EmptyStates"] = int(1.5 * len(self.structure) + 3)
             else:
                 self.input["EmptyStates"] = int(len(self.structure) + 3)
 
         if not self.input.sphinx.basis.read_only:
             self.load_basis_group()
         if not self.input.sphinx.structure.read_only:
             self.load_structure_group()
         if self.input["VaspPot"]:
             potformat = "VASP"
         else:
             potformat = "JTH"
         if not self.input.sphinx.pawPot.read_only:
-            self.load_species_group(check_overlap=self.input.CheckOverlap, potformat=potformat)
+            self.load_species_group(
+                check_overlap=self.input.CheckOverlap, potformat=potformat
+            )
         if not self.input.sphinx.initialGuess.read_only:
             self.load_guess_group()
         if not self.input.sphinx.PAWHamiltonian.read_only:
             self.load_hamilton_group()
         if not self.input.sphinx.main.read_only:
             self.load_main_group()
 
@@ -1255,60 +1333,61 @@
 
         Automatically called by job.run()
         """
 
         # If the structure group was not modified directly by the
         # user, via job.input.structure (which is likely True),
         # load it based on job.structure.
-        structure_sync = (str(self.input.sphinx.structure)
-                          == str(self.get_structure_group()))
+        structure_sync = str(self.input.sphinx.structure) == str(
+            self.get_structure_group()
+        )
         if not structure_sync and not self.input.sphinx.structure.read_only:
             self.load_structure_group()
 
         # copy potential files to working directory
         if self.input["VaspPot"]:
             potformat = "VASP"
         else:
             potformat = "JTH"
         # If the species group was not modified directly by the user,
         # via job.input.pawPot (which is likely True),
         # load it based on job.structure.
         if not structure_sync and not self.input.sphinx.pawPot.read_only:
-            self.load_species_group(check_overlap=self.input.CheckOverlap, potformat=potformat)
+            self.load_species_group(
+                check_overlap=self.input.CheckOverlap, potformat=potformat
+            )
 
         modified_elements = {
             key: value
             for key, value in self._potential.to_dict().items()
             if value is not None
         }
 
         self.input_writer.structure = self.structure
         self.input_writer.copy_potentials(
             potformat=potformat,
             xc=self.input["Xcorr"],
             cwd=self.working_directory,
-            modified_elements=modified_elements
+            modified_elements=modified_elements,
         )
 
         # Write spin constraints, if set via _generic_input.
         all_groups = [
             self.input.sphinx.pawPot,
             self.input.sphinx.structure,
             self.input.sphinx.basis,
             self.input.sphinx.PAWHamiltonian,
             self.input.sphinx.initialGuess,
-            self.input.sphinx.main
+            self.input.sphinx.main,
         ]
 
         if self._generic_input["fix_spin_constraint"]:
             self.input.sphinx.spinConstraint = Group()
             all_groups.append(self.input.sphinx.spinConstraint)
-            self.input_writer.write_spin_constraints(
-                cwd=self.working_directory
-                )
+            self.input_writer.write_spin_constraints(cwd=self.working_directory)
             self.input.sphinx.spinConstraint.setdefault("file", '"spins.in"')
 
         # In case the entire group was
         # set/overwritten as a normal dict.
         for group in all_groups:
             group = Group(group)
 
@@ -1319,17 +1398,15 @@
             f.write("//SPHInX input file generated by pyiron\n\n")
             f.write("format paw;\n")
             f.write("include <parameters.sx>;\n\n")
             f.write(self.input.sphinx.to_sphinx(indent=0))
 
     @property
     def _spin_enabled(self):
-        if np.any(self.structure.get_initial_magnetic_moments().flatten() != None):
-            return True
-        return False
+        return self.structure.has("initial_magmoms")
 
     def get_charge_density(self):
         """
         Gets the charge density from the hdf5 file. This value is normalized by the volume
 
         Returns:
             pyiron_atomistics.atomistics.volumetric.generic.VolumetricData
@@ -1359,16 +1436,19 @@
             es_obj.atoms = self.get_structure(-1)
             return es_obj
 
     def collect_output(self, force_update=False, compress_files=True):
         """
         Collects the outputs and stores them to the hdf file
         """
-        self._output_parser.collect(directory=self.working_directory)
-        self._output_parser.to_hdf(self._hdf5, force_update=force_update)
+        if self.is_compressed():
+            warnings.warn("Job already compressed - output not collected")
+            return
+        self.output.collect(directory=self.working_directory)
+        self.output.to_hdf(self._hdf5, force_update=force_update)
         if compress_files:
             self.compress()
 
     def convergence_check(self):
         """
         Checks for electronic and ionic convergence according to the user specified tolerance
 
@@ -1376,154 +1456,136 @@
 
             bool: True if converged
 
         """
         # Checks if sufficient empty states are present
         if not self.nbands_convergence_check():
             return False
-        if (
-            self._generic_input["calc_mode"] == "minimize"
-            and self._output_parser._parse_dict["scf_convergence"][-1]
-        ):
-            return True
-        elif self._generic_input["calc_mode"] == "static" and np.all(
-            self._output_parser._parse_dict["scf_convergence"]
-        ):
-            return True
-        else:
-            return False
+        return self.output.generic.dft.scf_convergence[-1]
 
     def collect_logfiles(self):
         """
         Collect errors and warnings.
         """
         self.collect_errors()
         self.collect_warnings()
 
     def collect_warnings(self):
         """
         Collects warnings from the SPHInX run
         """
-        self._logger.info("collect_warnings() is not yet \
-            implemented for SPHInX")
+        self._logger.info(
+            "collect_warnings() is not yet \
+            implemented for SPHInX"
+        )
 
     def collect_errors(self):
         """
         Collects errors from the SPHInX run
         """
         self._logger.info("collect_errors() is not yet implemented for SPHInX")
 
     def get_n_ir_reciprocal_points(
         self, is_time_reversal=True, symprec=1e-5, ignore_magmoms=False
     ):
         lattice = self.structure.cell
         positions = self.structure.get_scaled_positions()
         numbers = self.structure.get_atomic_numbers()
-        magmoms = self.structure.get_initial_magnetic_moments()
-        if np.all(magmoms==None) or ignore_magmoms:
-            magmoms = np.zeros(len(magmoms))
+        if ignore_magmoms:
+            magmoms = np.zeros(len(positions))
+        else:
+            magmoms = self.structure.get_initial_magnetic_moments()
         mag_num = np.array(list(zip(magmoms, numbers)))
         satz = np.unique(mag_num, axis=0)
         numbers = []
         for nn in np.all(satz == mag_num[:, np.newaxis], axis=-1):
             numbers.append(np.arange(len(satz))[nn][0])
         mapping, _ = spglib.get_ir_reciprocal_mesh(
             mesh=[int(self.input["KpointFolding"][k]) for k in range(3)],
             cell=(lattice, positions, numbers),
-            is_shift=np.dot(
-                self.structure.cell,
-                np.array(self.input["KpointCoords"])
-            ),
+            is_shift=np.dot(self.structure.cell, np.array(self.input["KpointCoords"])),
             is_time_reversal=is_time_reversal,
             symprec=symprec,
         )
         return len(np.unique(mapping))
 
     def check_setup(self):
-
         with warnings.catch_warnings(record=True) as w:
-
             # Check for parameters that were not modified but
             # possibly should have (encut, kpoints, smearing, etc.),
             # or were set to nonsensical values.
 
             if (
                 not (
                     isinstance(self.input.sphinx.basis["eCut"], int)
                     or isinstance(self.input.sphinx.basis["eCut"], float)
                 )
-                or round(self.input.sphinx.basis["eCut"]*RYDBERG_TO_EV, 0) == 340
+                or round(self.input.sphinx.basis["eCut"] * RYDBERG_TO_EV, 0) == 340
             ):
                 warnings.warn(
-                    "Energy cut-off value wrong or not modified from default "+
-                    "340 eV; change it via job.set_encut()"
+                    "Energy cut-off value wrong or not modified from default "
+                    + "340 eV; change it via job.set_encut()"
                 )
             if not (
                 isinstance(self.input.sphinx.basis["kPoint"]["coords"], np.ndarray)
                 or len(self.input.sphinx.basis["kPoint"]["coords"]) != 3
             ):
                 warnings.warn("K point coordinates seem to be inappropriate")
             if (
                 not (
                     isinstance(self.input.sphinx.PAWHamiltonian["ekt"], int)
                     or isinstance(self.input.sphinx.PAWHamiltonian["ekt"], float)
                 )
                 or round(self.input.sphinx.PAWHamiltonian["ekt"], 1) == 0.2
             ):
                 warnings.warn(
-                    "Fermi smearing value wrong or not modified from default "+
-                    "0.2 eV; change it via job.set_occupancy_smearing()"
+                    "Fermi smearing value wrong or not modified from default "
+                    + "0.2 eV; change it via job.set_occupancy_smearing()"
                 )
             if not (
                 isinstance(self.input.sphinx.basis["folding"], np.ndarray)
                 or len(self.input.sphinx.basis["folding"]) != 3
-            ) or self.input.sphinx.basis["folding"].tolist() == [4,4,4]:
+            ) or self.input.sphinx.basis["folding"].tolist() == [4, 4, 4]:
                 warnings.warn(
-                    "K point folding wrong or not modified from default "+
-                    "[4,4,4]; change it via job.set_kpoints()"
+                    "K point folding wrong or not modified from default "
+                    + "[4,4,4]; change it via job.set_kpoints()"
                 )
             if self.get_n_ir_reciprocal_points() < self.server.cores:
                 warnings.warn(
                     "Number of cores exceed number of irreducible "
                     + "reciprocal points: "
                     + str(self.get_n_ir_reciprocal_points())
                 )
             if self.input["EmptyStates"] == "auto":
-                if any(self.structure.get_initial_magnetic_moments() != None):
+                if self._spin_enabled:
                     warnings.warn(
                         "Number of empty states was not specified. Default: "
                         + "3+NIONS*1.5 for magnetic systems. "
                     )
                 else:
                     warnings.warn(
                         "Number of empty states was not specified. Default: "
                         + "3+NIONS for non-magnetic systems"
                     )
 
-            if len(w) > 0:
-                print("WARNING:")
-                for ww in w:
-                    print(ww.message)
-                return False
-            else:
-                return True
+            return len(w) == 0
 
     def validate_ready_to_run(self):
         """
         Checks whether parameters are set appropriately. It does not
         mean the simulation won't run if it returns False.
         """
 
         all_groups = {
             "job.input.pawPot": self.input.sphinx.pawPot,
             "job.input.structure": self.input.sphinx.structure,
             "job.input.basis": self.input.sphinx.basis,
             "job.input.PAWHamiltonian": self.input.sphinx.PAWHamiltonian,
             "job.input.initialGuess": self.input.sphinx.initialGuess,
-            "job.input.main": self.input.sphinx.main
+            "job.input.main": self.input.sphinx.main,
         }
 
         if np.any([len(all_groups[group]) == 0 for group in all_groups]):
             self.load_default_groups()
 
         if self.structure is None:
             raise AssertionError(
@@ -1535,62 +1597,66 @@
                 "Number of cores cannot be smaller than the number "
                 + "of OpenMP threads"
             )
         with warnings.catch_warnings(record=True) as w:
             # Warn about discrepancies between values in
             # self.input and individual groups, in case
             # a user modified them directly
-            if round(self.input["EnCut"], 0) != \
-                    round(self.input.sphinx.basis.eCut * RYDBERG_TO_EV, 0):
+            if round(self.input["EnCut"], 0) != round(
+                self.input.sphinx.basis.eCut * RYDBERG_TO_EV, 0
+            ):
                 warnings.warn(
                     "job.input.basis.eCut was modified directly. "
                     "It is recommended to set it via job.set_encut()"
                 )
 
-            if round(self.input["Sigma"], 1) != \
-                    round(self.input.sphinx.PAWHamiltonian.ekt, 1):
+            if round(self.input["Sigma"], 1) != round(
+                self.input.sphinx.PAWHamiltonian.ekt, 1
+            ):
                 warnings.warn(
                     "job.input.PAWHamiltonian.ekt was modified directly. "
                     "It is recommended to set it via "
                     "job.set_occupancy_smearing()"
                 )
 
             if self.input["Xcorr"] != self.input.sphinx.PAWHamiltonian.xc:
                 warnings.warn(
                     "job.input.PAWHamiltonian.xc was modified directly. "
                     "It is recommended to set it via "
                     "job.exchange_correlation_functional()"
                 )
 
-            if self.input["EmptyStates"] != self.input.sphinx.PAWHamiltonian.nEmptyStates:
+            if (
+                self.input["EmptyStates"]
+                != self.input.sphinx.PAWHamiltonian.nEmptyStates
+            ):
                 warnings.warn(
                     "job.input.PAWHamiltonian.nEmptyStates was modified "
                     "directly. It is recommended to set it via "
                     "job.set_empty_states()"
                 )
 
             if (
                 "KpointCoords" in self.input
                 and np.array(self.input.KpointCoords).tolist()
-                    != np.array(self.input.sphinx.basis.kPoint.coords).tolist()
-                ) \
-            or (
+                != np.array(self.input.sphinx.basis.kPoint.coords).tolist()
+            ) or (
                 "KpointFolding" in self.input
                 and np.array(self.input.KpointFolding).tolist()
-                    != np.array(self.input.sphinx.basis.folding).tolist()
-                ):
-
+                != np.array(self.input.sphinx.basis.folding).tolist()
+            ):
                 warnings.warn(
                     "job.input.basis.kPoint was modified directly. "
                     "It is recommended to set all k-point settings via "
                     "job.set_kpoints()"
                 )
 
-            structure_sync = (str(self.input.sphinx.structure)
-                              == str(self.get_structure_group()))
+            structure_sync = str(self.input.sphinx.structure) == str(
+                self.get_structure_group()
+            )
             if not structure_sync and not self.input.sphinx.structure.read_only:
                 warnings.warn(
                     "job.input.structure != job.structure. "
                     "The current job.structure will overwrite "
                     "any changes you may might have made to "
                     "job.input.structure in the meantime. "
                     "To disable this overwrite, "
@@ -1614,124 +1680,267 @@
 
         Args:
             files_to_compress (list): A list of files to compress (optional)
         """
         # delete empty files
         if files_to_compress is None:
             files_to_compress = [
-                f for f in list(self.list_files())
-                if (f not in ["rho.sxb", "waves.sxb"]
-                    and not stat.S_ISFIFO(os.stat(os.path.join(
-                            self.working_directory,
-                            f
-                        )).st_mode))
+                f
+                for f in list(self.list_files())
+                if (
+                    f not in ["rho.sxb", "waves.sxb"]
+                    and not stat.S_ISFIFO(
+                        os.stat(os.path.join(self.working_directory, f)).st_mode
+                    )
+                )
             ]
         for f in list(self.list_files()):
             filename = os.path.join(self.working_directory, f)
             if (
                 f not in files_to_compress
                 and os.path.exists(filename)
                 and os.stat(filename).st_size == 0
             ):
                 os.remove(filename)
         super(SphinxBase, self).compress(files_to_compress=files_to_compress)
 
     @staticmethod
     def check_vasp_potentials():
         return any(
-            [os.path.exists(
-                os.path.join(p, 'vasp', 'potentials', 'potpaw', 'Fe', 'POTCAR')
+            [
+                os.path.exists(
+                    os.path.join(p, "vasp", "potentials", "potpaw", "Fe", "POTCAR")
                 )
-            for p in s.resource_paths]
+                for p in state.settings.resource_paths
+            ]
         )
 
+    def run_addon(
+        self,
+        addon,
+        args=None,
+        from_tar=None,
+        silent=False,
+        log=True,
+        version=None,
+        debug=False,
+    ):
+        """Run a SPHInX addon
+
+        addon          - name of addon (str)
+        args           - arguments (str or list)
+        from_tar       - if job is compressed, extract these files (list)
+        silent         - do not print output for successful runs?
+        log            - produce log file?
+        version        - which sphinx version to load (str or None)
+        debug          - return subprocess.CompletedProcess ?
+
+        """
+        if self.is_compressed() and from_tar is None:
+            raise FileNotFoundError(
+                "Cannot run add-on on compressed job without 'from_tar' parameter.\n"
+                + "   Solution 1: Run .decompress () first.\n"
+                + "   Solution 2: specify from_tar list to run in temporary directory\n"
+                + "   Solution 3: run with from_tar=[] if no files from tar are needed\n"
+            )
+
+        # prepare argument list
+        if args is None:
+            args = ""
+        elif isinstance(args, list):
+            args = " ".join(args)
+        if log:
+            args += " --log"
+
+        cmd = addon + " " + args
+
+        # --- handle versions
+        sxv = sxversions()
+        if (
+            version is None
+            and self.executable.version is not None
+            and self.executable.version in sxv.keys()
+        ):
+            version = self.executable.version
+            if not silent:
+                print("Taking version '" + version + "' from job._executable version")
+        if isinstance(version, str):
+            if version in sxv.keys():
+                cmd = sxv[version] + " && " + cmd
+            elif version != "":
+                raise KeyError(
+                    "version '"
+                    + version
+                    + "' not found. Available versions are: '"
+                    + "', '".join(sxv.keys())
+                    + "'."
+                )
+            # version="" overrides job.executable_version
+        elif version is not None:
+            raise TypeError("version must be str or None")
+
+        if isinstance(from_tar, str):
+            from_tar = [from_tar]
+        if self.is_compressed() and isinstance(from_tar, list):
+            # run addon in temporary directory
+            with TemporaryDirectory() as tempd:
+                if not silent:
+                    print("Running {} in temporary directory {}".format(addon, tempd))
+
+                # --- extract files from list
+                # note: tf should be obtained from JobCore to ensure encapsulation
+                tarfilename = os.path.join(
+                    self.working_directory, self.job_name + ".tar.bz2"
+                )
+                with tarfile.open(tarfilename, "r:bz2") as tf:
+                    for file in from_tar:
+                        try:
+                            tf.extract(file, path=tempd)
+                        except:
+                            print("Cannot extract " + file + " from " + tarfilename)
+
+                # --- link other files
+                linkfiles = []
+                for file in self.list_files():
+                    linkfile = os.path.join(tempd, file)
+                    if not os.path.isfile(linkfile):
+                        os.symlink(
+                            os.path.join(self.working_directory, file),
+                            linkfile,
+                            target_is_directory=True,
+                        )
+                        linkfiles.append(linkfile)
+                # now run
+                out = subprocess.run(
+                    cmd, cwd=tempd, shell=True, stdout=PIPE, stderr=PIPE, text=True
+                )
+
+                # now clean tempdir
+                for file in from_tar:
+                    try:
+                        os.remove(os.path.join(tempd, file))
+                    except FileNotFoundError:
+                        pass
+                for linkfile in linkfiles:
+                    if os.path.islink:
+                        os.remove(linkfile)
+
+                # move output to working directory for successful runs
+                if out.returncode == 0:
+                    for file in os.listdir(tempd):
+                        movefile(os.path.join(tempd, file), self.working_directory)
+                        if not silent:
+                            print("Copying " + file + " to " + self.working_directory)
+                else:
+                    print(addon + " crashed - potential output files are not kept.")
+
+        else:
+            out = subprocess.run(
+                cmd,
+                cwd=self.working_directory,
+                shell=True,
+                stdout=PIPE,
+                stderr=PIPE,
+                text=True,
+            )
+            if out.returncode != 0:
+                print(addon + " crashed.")
+
+        # print output
+        if not silent or out.returncode != 0:
+            if out.returncode != 0:
+                print(addon + " output:\n\n")
+            print(out.stdout)
+            if out.returncode != 0:
+                print(out.stderr)
+        return out if debug else None
+
 
 class InputWriter(object):
     """
     The SPHInX Input writer is called to write the
     SPHInX specific input files.
     """
 
     def __init__(self):
         self.structure = None
         self._id_pyi_to_spx = []
         self._id_spx_to_pyi = []
         self.file_dict = {}
 
-    def copy_potentials(self, potformat="JTH", xc=None, cwd=None,
-                        pot_path_dict=None, modified_elements=None):
+    def copy_potentials(
+        self,
+        potformat="JTH",
+        xc=None,
+        cwd=None,
+        pot_path_dict=None,
+        modified_elements=None,
+    ):
         """
         Copy potential files
 
         Args:
             potformat (str):
             xc (str/None):
             cwd (str/None):
             pot_path_dict (dict):
             modified_elements (dict):
         """
 
         if pot_path_dict is None:
             pot_path_dict = {}
 
-        if potformat == 'JTH':
+        if potformat == "JTH":
             potentials = SphinxJTHPotentialFile(xc=xc)
             find_potential_file = find_potential_file_jth
             pot_path_dict.setdefault("PBE", "jth-gga-pbe")
-        elif potformat == 'VASP':
+        elif potformat == "VASP":
             potentials = VaspPotentialFile(xc=xc)
             find_potential_file = find_potential_file_vasp
             pot_path_dict.setdefault("PBE", "paw-gga-pbe")
             pot_path_dict.setdefault("LDA", "paw-lda")
         else:
-            raise ValueError('Only JTH and VASP potentials are supported!')
+            raise ValueError("Only JTH and VASP potentials are supported!")
 
         for species_obj in self.structure.get_species_objects():
             if species_obj.Parent is not None:
                 elem = species_obj.Parent
             else:
                 elem = species_obj.Abbreviation
 
             if "pseudo_potcar_file" in species_obj.tags.keys():
                 new_element = species_obj.tags["pseudo_potcar_file"]
-                potentials.add_new_element(
-                    parent_element=elem, new_element=new_element
-                )
+                potentials.add_new_element(parent_element=elem, new_element=new_element)
                 potential_path = find_potential_file(
-                    path=potentials.find_default(new_element)[
-                        "Filename"].values[0][0]
+                    path=potentials.find_default(new_element)["Filename"].values[0][0]
                 )
                 assert os.path.isfile(
                     potential_path
                 ), "such a file does not exist in the pp directory"
             elif elem in modified_elements.keys():
                 new_element = modified_elements[elem]
                 if os.path.isabs(new_element):
                     potential_path = new_element
                 else:
                     potentials.add_new_element(
                         parent_element=elem, new_element=new_element
                     )
                     potential_path = find_potential_file(
-                        path=potentials.find_default(new_element)[
-                            "Filename"].values[0][0]
+                        path=potentials.find_default(new_element)["Filename"].values[0][
+                            0
+                        ]
                     )
             else:
                 potential_path = find_potential_file(
-                    path=potentials.find_default(elem)[
-                        "Filename"].values[0][0]
+                    path=potentials.find_default(elem)["Filename"].values[0][0]
                 )
             if potformat == "JTH":
-                copyfile(potential_path, posixpath.join(
-                    cwd, elem + "_GGA.atomicdata"
-                ))
+                copyfile(potential_path, posixpath.join(cwd, elem + "_GGA.atomicdata"))
             else:
-                copyfile(potential_path, posixpath.join(
-                    cwd, elem + "_POTCAR"
-                ))
+                copyfile(potential_path, posixpath.join(cwd, elem + "_POTCAR"))
 
     @property
     def id_spx_to_pyi(self):
         if self.structure is None:
             return None
         if len(self._id_spx_to_pyi) == 0:
             self._initialize_order()
@@ -1745,72 +1954,63 @@
             self._initialize_order()
         return self._id_pyi_to_spx
 
     def _initialize_order(self):
         for elm_species in self.structure.get_species_objects():
             self._id_pyi_to_spx.append(
                 np.arange(len(self.structure))[
-                    self.structure.get_chemical_symbols()
-                    == elm_species.Abbreviation
+                    self.structure.get_chemical_symbols() == elm_species.Abbreviation
                 ]
             )
         self._id_pyi_to_spx = np.array(
             [ooo for oo in self._id_pyi_to_spx for ooo in oo]
         )
         self._id_spx_to_pyi = np.array([0] * len(self._id_pyi_to_spx))
         for i, p in enumerate(self._id_pyi_to_spx):
             self._id_spx_to_pyi[p] = i
 
-    def write_spin_constraints(
-            self, file_name="spins.in", cwd=None, spins_list=None
-    ):
+    def write_spin_constraints(self, file_name="spins.in", cwd=None, spins_list=None):
         """
         Write a text file containing a list of all spins named spins.in -
         which is used for the external control scripts.
 
         Args:
             file_name (str): name of the file to be written (optional)
             cwd (str): the current working directory (optinal)
             spins_list (list): the input to write, if no input is
                 given the default input will be written. (optional)
         """
-        s.logger.debug(f"Writing {file_name}")
-        if spins_list is None or len(spins_list) == 0:
-            spins_list = []
-            s.logger.debug("Getting magnetic moments via \
-                get_initial_magnetic_moments")
-            if any(self.structure.get_initial_magnetic_moments().flatten() != None):
-                if any([
+        state.logger.debug(f"Writing {file_name}")
+        state.logger.debug(
+            "Getting magnetic moments via \
+            get_initial_magnetic_moments"
+        )
+        if self.structure.has("initial_magmoms"):
+            if any(
+                [
                     True
                     if isinstance(spin, list) or isinstance(spin, np.ndarray)
                     else False
                     for spin in self.structure.get_initial_magnetic_moments()
-                ]):
-                    raise ValueError(
-                        "SPHInX only supports collinear spins at the moment."
-                    )
-                else:
-                    for spin, value in zip(
-                        self.structure.spin_constraint[self.id_pyi_to_spx],
-                        self.structure.get_initial_magnetic_moments()[
-                            self.id_pyi_to_spx
-                        ],
-                    ):
-                        if spin:
-                            spins_list.append(str(value))
-                        else:
-                            spins_list.append("X")
-                    spins_str = "\n".join(spins_list)+'\n'
-        if spins_str is not None:
-            if cwd is not None:
-                file_name = posixpath.join(cwd, file_name)
-            with open(file_name, "w") as f:
-                f.write(spins_str)
+                ]
+            ):
+                raise ValueError("SPHInX only supports collinear spins at the moment.")
+            else:
+                constraint = self.structure.spin_constraint[self.id_pyi_to_spx]
+                if spins_list is None or len(spins_list) == 0:
+                    spins_list = self.structure.get_initial_magnetic_moments()
+                spins = spins_list[self.id_pyi_to_spx].astype(str)
+                spins[~np.asarray(constraint)] = "X"
+                spins_str = "\n".join(spins) + "\n"
+                if cwd is not None:
+                    file_name = posixpath.join(cwd, file_name)
+                with open(file_name, "w") as f:
+                    f.write(spins_str)
         else:
-            s.logger.debug("No magnetic moments")
+            state.logger.debug("No magnetic moments")
 
 
 class Group(DataContainer):
     """
     Dictionary-like object to store SPHInX inputs.
 
     Attributes (sub-groups, parameters, & flags) can be set
@@ -1864,34 +2064,28 @@
         self.set(parameter, val)
 
     def remove(self, name):
         if name in self.keys():
             del self[name]
 
     def to_sphinx(self, content="__self__", indent=0):
-
         if content == "__self__":
             content = self
 
         def format_value(v):
             if isinstance(v, bool):
                 if v:
                     return ";"
                 else:
                     return " = false;"
             elif isinstance(v, Group):
                 if len(v) == 0:
                     return " {}"
                 else:
-                    return (
-                        " {\n"
-                        + self.to_sphinx(v, indent+1)
-                        + indent * "\t"
-                        + "}"
-                    )
+                    return " {\n" + self.to_sphinx(v, indent + 1) + indent * "\t" + "}"
             else:
                 if isinstance(v, np.ndarray):
                     v = v.tolist()
                 return " = {!s};".format(v)
 
         line = ""
         for k, v in content.items():
@@ -1900,52 +2094,240 @@
                     line += indent * "\t" + str(k) + format_value(vv) + "\n"
             else:
                 line += indent * "\t" + str(k) + format_value(v) + "\n"
 
         return line
 
 
-class Output(object):
+def splitter(arr, counter):
+    if len(arr) == 0 or len(counter) == 0:
+        return []
+    arr_new = []
+    spl_loc = list(np.where(np.array(counter) == min(counter))[0])
+    spl_loc.append(None)
+    for ii, ll in enumerate(spl_loc[:-1]):
+        arr_new.append(np.array(arr[ll : spl_loc[ii + 1]]).tolist())
+    return arr_new
+
+
+class _SphinxLogParser:
+    def __init__(self, log_file):
+        self.log_file = log_file
+        self._check_enter_scf()
+        self._log_main = None
+        self._counter = None
+        self._n_atoms = None
+        self._n_steps = None
+        self._spin_enabled = None
+
+    @property
+    def spin_enabled(self):
+        return len(re.findall("The spin for the label", self.log_file)) > 0
+
+    @property
+    def log_main(self):
+        if self._log_main is None:
+            match = re.search("Enter Main Loop", self.log_file)
+            self._log_main = match.end() + 1
+        return self.log_file[self._log_main :]
+
+    @property
+    def job_finished(self):
+        if (
+            len(re.findall("Program exited normally.", self.log_file, re.MULTILINE))
+            == 0
+        ):
+            warnings.warn("scf loops did not converge")
+            return False
+        return True
+
+    def _check_enter_scf(self):
+        if len(re.findall("Enter Main Loop", self.log_file, re.MULTILINE)) == 0:
+            raise AssertionError("Log file created but first scf loop not reached")
+
+    def get_n_valence(self):
+        log = self.log_file.split("\n")
+        return {
+            log[ii - 1].split()[1]: int(ll.split("=")[-1])
+            for ii, ll in enumerate(log)
+            if ll.startswith("| Z=")
+        }
+
+    @property
+    def log_k_points(self):
+        start_match = re.search(
+            "-ik-     -x-      -y-       -z-    \|  -weight-    -nG-    -label-",
+            self.log_file,
+        )
+        log_part = self.log_file[start_match.end() + 1 :]
+        log_part = log_part[: re.search("^\n", log_part, re.MULTILINE).start()]
+        return log_part.split("\n")[:-2]
+
+    def get_bands_k_weights(self):
+        return np.array([float(kk.split()[6]) for kk in self.log_k_points])
+
+    @property
+    def _rec_cell(self):
+        log_extract = re.findall("b[1-3]:.*$", self.log_file, re.MULTILINE)
+        return (
+            np.array([ll.split()[1:4] for ll in log_extract]).astype(float)
+            / BOHR_TO_ANGSTROM
+        )[:3]
+
+    def get_kpoints_cartesian(self):
+        return np.einsum("ni,ij->nj", self.k_points, self._rec_cell)
+
+    @property
+    def k_points(self):
+        return np.array(
+            [[float(kk.split()[i]) for i in range(2, 5)] for kk in self.log_k_points]
+        )
+
+    def get_volume(self):
+        volume = re.findall("Omega:.*$", self.log_file, re.MULTILINE)
+        if len(volume) > 0:
+            volume = float(volume[0].split()[1])
+            volume *= BOHR_TO_ANGSTROM**3
+        else:
+            volume = 0
+        return np.array(self.n_steps * [volume])
+
+    @property
+    def counter(self):
+        if self._counter is None:
+            self._counter = [
+                int(re.sub("[^0-9]", "", line.split("=")[0]))
+                for line in re.findall("F\(.*$", self.log_main, re.MULTILINE)
+            ]
+        return self._counter
+
+    def get_energy_free(self):
+        return splitter(
+            [
+                float(line.split("=")[1]) * HARTREE_TO_EV
+                for line in re.findall("F\(.*$", self.log_main, re.MULTILINE)
+            ],
+            self.counter,
+        )
+
+    def get_energy_int(self):
+        return splitter(
+            [
+                float(line.replace("=", " ").replace(",", " ").split()[1])
+                * HARTREE_TO_EV
+                for line in re.findall("^eTot\([0-9].*$", self.log_main, re.MULTILINE)
+            ],
+            self.counter,
+        )
+
+    @property
+    def n_atoms(self):
+        if self._n_atoms is None:
+            self._n_atoms = len(
+                np.unique(re.findall("^Species.*\{", self.log_main, re.MULTILINE))
+            )
+        return self._n_atoms
+
+    def get_forces(self, spx_to_pyi=None):
+        forces = [
+            float(re.split("{|}", line)[1].split(",")[i])
+            * HARTREE_OVER_BOHR_TO_EV_OVER_ANGSTROM
+            for line in re.findall("^Species.*$", self.log_main, re.MULTILINE)
+            for i in range(3)
+        ]
+        if len(forces) != 0:
+            forces = np.array(forces).reshape(-1, self.n_atoms, 3)
+            if spx_to_pyi is not None:
+                for ii, ff in enumerate(forces):
+                    forces[ii] = ff[spx_to_pyi]
+        return forces
+
+    def get_magnetic_forces(self, spx_to_pyi=None):
+        magnetic_forces = [
+            HARTREE_TO_EV * float(line.split()[-1])
+            for line in re.findall("^nu\(.*$", self.log_main, re.MULTILINE)
+        ]
+        if len(magnetic_forces) != 0:
+            magnetic_forces = np.array(magnetic_forces).reshape(-1, self.n_atoms)
+            if spx_to_pyi is not None:
+                for ii, mm in enumerate(magnetic_forces):
+                    magnetic_forces[ii] = mm[spx_to_pyi]
+        return splitter(magnetic_forces, self.counter)
+
+    @property
+    def n_steps(self):
+        if self._n_steps is None:
+            self._n_steps = len(
+                re.findall("\| SCF calculation", self.log_file, re.MULTILINE)
+            )
+        return self._n_steps
+
+    def _parse_band(self, term):
+        arr = np.loadtxt(re.findall(term, self.log_main, re.MULTILINE))
+        shape = (-1, len(self.k_points), arr.shape[-1])
+        if self.spin_enabled:
+            shape = (-1, 2, len(self.k_points), shape[-1])
+        return arr.reshape(shape)
+
+    def get_band_energy(self):
+        return self._parse_band("final eig \[eV\]:(.*)$")
+
+    def get_occupancy(self):
+        return self._parse_band("final focc:(.*)$")
+
+    def get_convergence(self):
+        conv_dict = {
+            "WARNING: Maximum number of steps exceeded": False,
+            "Convergence reached.": True,
+        }
+        key = "|".join(list(conv_dict.keys())).replace(".", "\.")
+        items = re.findall(key, self.log_main, re.MULTILINE)
+        convergence = [conv_dict[k] for k in items]
+        diff = self.n_steps - len(convergence)
+        for _ in range(diff):
+            convergence.append(False)
+        return convergence
+
+    def get_fermi(self):
+        return np.array(
+            [
+                float(line.split()[2])
+                for line in re.findall("Fermi energy:.*$", self.log_main, re.MULTILINE)
+            ]
+        )
+
+
+class Output:
     """
     Handles the output from a SPHInX simulation.
     """
 
     def __init__(self, job):
         self._job = job
-        self._parse_dict = defaultdict(list)
+        self.generic = DataContainer(table_name="output/generic")
         self.charge_density = SphinxVolumetricData()
         self.electrostatic_potential = SphinxVolumetricData()
-
-    @staticmethod
-    def splitter(arr, counter):
-        if len(arr) == 0 or len(counter) == 0:
-            return []
-        arr_new = []
-        spl_loc = list(np.where(np.array(counter) == min(counter))[0])
-        spl_loc.append(None)
-        for ii, ll in enumerate(spl_loc[:-1]):
-            arr_new.append(np.array(arr[ll : spl_loc[ii + 1]]).tolist())
-        return arr_new
+        self.generic.create_group("dft")
+        self.old_version = False
 
     def collect_spins_dat(self, file_name="spins.dat", cwd=None):
         """
 
         Args:
             file_name:
             cwd:
 
         Returns:
 
         """
         if not os.path.isfile(posixpath.join(cwd, file_name)):
             return None
         spins = np.loadtxt(posixpath.join(cwd, file_name))
-        self._parse_dict["atom_scf_spins"] = self.splitter(
-            np.array([ss[self._job.id_spx_to_pyi] for ss in spins[:, 1:]]),
-            spins[:, 0]
+        self.generic.dft.atom_scf_spins = splitter(
+            np.array([ss[self._job.id_spx_to_pyi] for ss in spins[:, 1:]]), spins[:, 0]
         )
 
     def collect_energy_dat(self, file_name="energy.dat", cwd=None):
         """
 
         Args:
             file_name:
@@ -1953,37 +2335,29 @@
 
         Returns:
 
         """
         if not os.path.isfile(posixpath.join(cwd, file_name)):
             return None
         energies = np.loadtxt(posixpath.join(cwd, file_name))
-        self._parse_dict["scf_computation_time"] = self.splitter(
-            energies[:, 1], energies[:, 0]
-        )
-        self._parse_dict["scf_energy_int"] = self.splitter(
+        self.generic.dft.scf_computation_time = splitter(energies[:, 1], energies[:, 0])
+        self.generic.dft.scf_energy_int = splitter(
             energies[:, 2] * HARTREE_TO_EV, energies[:, 0]
         )
+
+        def en_split(e, counter=energies[:, 0]):
+            return splitter(e * HARTREE_TO_EV, counter)
+
         if len(energies[0]) == 7:
-            self._parse_dict["scf_energy_free"] = self.splitter(
-                energies[:, 3] * HARTREE_TO_EV, energies[:, 0]
-            )
-            self._parse_dict["scf_energy_zero"] = self.splitter(
-                energies[:, 4] * HARTREE_TO_EV, energies[:, 0]
-            )
-            self._parse_dict["scf_energy_band"] = self.splitter(
-                energies[:, 5] * HARTREE_TO_EV, energies[:, 0]
-            )
-            self._parse_dict["scf_electronic_entropy"] = self.splitter(
-                energies[:, 6] * HARTREE_TO_EV, energies[:, 0]
-            )
+            self.generic.dft.scf_energy_free = en_split(energies[:, 3])
+            self.generic.dft.scf_energy_zero = en_split(energies[:, 4])
+            self.generic.dft.scf_energy_band = en_split(energies[:, 5])
+            self.generic.dft.scf_electronic_entropy = en_split(energies[:, 6])
         else:
-            self._parse_dict["scf_energy_band"] = self.splitter(
-                energies[:, 3] * HARTREE_TO_EV, energies[:, 0]
-            )
+            self.generic.dft.scf_energy_band = en_split(energies[:, 3])
 
     def collect_residue_dat(self, file_name="residue.dat", cwd=None):
         """
 
         Args:
             file_name:
             cwd:
@@ -1993,498 +2367,265 @@
         """
         if not os.path.isfile(posixpath.join(cwd, file_name)):
             return None
         residue = np.loadtxt(posixpath.join(cwd, file_name))
         if len(residue) == 0:
             return None
         if len(residue[0]) == 2:
-            self._parse_dict["scf_residue"] = self.splitter(
-                residue[:, 1] * HARTREE_TO_EV, residue[:, 0]
-            )
+            self.generic.dft.scf_residue = splitter(residue[:, 1], residue[:, 0])
         else:
-            self._parse_dict["scf_residue"] = self.splitter(
-                residue[:, 1:] * HARTREE_TO_EV, residue[:, 0]
-            )
+            self.generic.dft.scf_residue = splitter(residue[:, 1:], residue[:, 0])
 
     def collect_eps_dat(self, file_name="eps.dat", cwd=None):
         """
 
         Args:
             file_name:
             cwd:
 
         Returns:
 
         """
-        file_name = posixpath.join(cwd, file_name)
-        if os.path.isfile(file_name):
-            try:
-                value = np.loadtxt(file_name)[:, 1:]
-            except IndexError:
-                value = np.loadtxt(file_name)[1:]
-        elif os.path.isfile(posixpath.join(
-                cwd, "eps.0.dat")) and os.path.isfile(
-                posixpath.join(cwd, "eps.1.dat")
-        ):
-            eps_up = np.loadtxt(posixpath.join(cwd, "eps.0.dat"))
-            eps_down = np.loadtxt(posixpath.join(cwd, "eps.1.dat"))
-            if len(eps_up.shape) == 2:
-                eps_up = eps_up[:, 1:]
-                eps_down = eps_down[:, 1:]
-            else:
-                eps_up = eps_up[1:]
-                eps_down = eps_down[1:]
-            value = np.vstack((eps_up, eps_down)).reshape((2,)+eps_up.shape)
-        else:
-            return
-        shape = np.asarray(self._parse_dict["bands_eigen_values"]).shape
-        if shape[1:] == value.shape:
-            self._parse_dict["bands_eigen_values"][-1] = value
-        else:
-            self._parse_dict["bands_eigen_values"] = value.reshape((-1,)+value.shape)
-        return None
+        if isinstance(file_name, str):
+            file_name = [file_name]
+        values = []
+        for f in file_name:
+            file_tmp = posixpath.join(cwd, f)
+            if not os.path.isfile(file_tmp):
+                return
+            values.append(np.loadtxt(file_tmp)[..., 1:])
+        values = np.stack(values, axis=0)
+        if "bands_eigen_values" not in self.generic.dft.list_nodes():
+            self.generic.dft.bands_eigen_values = values.reshape((-1,) + values.shape)
 
-    def collect_energy_struct(self, file_name="energy-structOpt.dat",
-                              cwd=None):
+    def collect_energy_struct(self, file_name="energy-structOpt.dat", cwd=None):
         """
 
         Args:
             file_name:
             cwd:
 
         Returns:
 
         """
-        energy_free_lst = []
         file_name = posixpath.join(cwd, file_name)
         if os.path.isfile(file_name):
-            with open(file_name, "r") as f:
-                for line in f.readlines():
-                    line = line.split()
-                    energy_free_lst.append(float(line[1]) * HARTREE_TO_EV)
-        self._energy_free_struct_lst = energy_free_lst
+            self.generic.dft.energy_free = (
+                np.loadtxt(file_name).reshape(-1, 2)[:, 1] * HARTREE_TO_EV
+            )
 
-    def collect_sphinx_log(
-        self, file_name="sphinx.log", cwd=None, check_consistency=True
-    ):
+    def collect_sphinx_log(self, file_name="sphinx.log", cwd=None):
         """
 
         Args:
             file_name:
             cwd:
-            check_consistency (bool):
 
         Returns:
 
         """
 
         if not os.path.isfile(posixpath.join(cwd, file_name)):
             return None
 
-        def check_conv(line):
-            if line.startswith("WARNING: Maximum number of steps exceeded"):
-                return False
-            elif line.startswith("Convergence reached"):
-                return True
-            else:
-                return None
-
         with open(posixpath.join(cwd, file_name), "r") as sphinx_log_file:
-            log_file = sphinx_log_file.readlines()
-            if not np.any(["Enter Main Loop" in line for line in log_file]):
-                self._job.status.aborted = True
-                raise AssertionError("SPHInX did not enter the main loop; \
-                    output not collected")
-            if not np.any(["Program exited normally." in line
-                           for line in log_file]):
-                self._job.status.aborted = True
-                warnings.warn("SPHInX parsing failed; most likely \
-                    SPHInX crashed.")
-            main_start = np.where([
-                "Enter Main Loop" in line
-                for line in log_file]
-            )[0][0]
-            log_main = log_file[main_start:]
-
-            self._parse_dict["n_valence"] = {
-                log_file[ii-1].split()[1]:int(ll.split('=')[-1])
-                for ii, ll in enumerate(log_file)
-                if ll.startswith('| Z=')
-            }
-
-            def get_partial_log(file_content, start_line, end_line):
-                start_line = np.where([
-                    line == start_line
-                    for line in file_content]
-                )[0][0]
-                end_line = np.where(
-                    [line == end_line for line in file_content[start_line:]]
-                )[0][0]
-                return file_content[start_line : start_line + end_line]
-            k_points = get_partial_log(
-                log_file,
-                "| Symmetrized k-points:               "
-                + "in cartesian coordinates\n",
-                "\n",
-            )[2:-1]
-            self._parse_dict["bands_k_weights"] = np.array([float(kk.split()[6]) for kk in k_points])
-            k_points = np.array([[float(kk.split()[i]) for i in range(2, 5)] for kk in k_points])
-            rec_cell = np.linalg.inv(self._job.structure.cell.T / BOHR_TO_ANGSTROM) * 2 * np.pi
-            self._parse_dict["kpoints_cartesian"] = np.einsum('ni,ij->nj', k_points, np.linalg.inv(rec_cell))
-            counter = [
-                int(line.replace("F(", "").replace(")", " ").split()[0])
-                for line in log_main
-                if line.startswith("F(")
-            ]
-            energy_free = [
-                float(line.replace("=", " ").replace(",", " ").split()[1])
-                * HARTREE_TO_EV
-                for line in log_main
-                if line.startswith("F(")
-            ]
-            energy_int = [
-                float(line.replace("=", " ").replace(",", " ").split()[1])
-                * HARTREE_TO_EV
-                for line in log_main
-                if line.startswith("eTot(") and not line.startswith(
-                    "eTot(Val)")
-            ]
-            energy_zero = 0.5 * (np.array(energy_free) + np.array(energy_int))
-            energy_band = [
-                float(line.split()[2]) * HARTREE_TO_EV
-                for line in log_main
-                if line.startswith("eBand")
-            ]
-
-            forces = [
-                float(re.split("{|}", line)[1].split(",")[i])
-                * HARTREE_OVER_BOHR_TO_EV_OVER_ANGSTROM
-                for line in log_main
-                for i in range(3)
-                if line.startswith("Species: ")
-            ]
-            magnetic_forces = [
-                HARTREE_TO_EV * float(line.split()[-1])
-                for line in log_main
-                if line.startswith("nu(")
-            ]
-            convergence = [
-                check_conv(line) for line in log_main
-                if check_conv(line) is not None
-            ]
-            self._parse_dict["bands_e_fermi"] = np.array([float(line.split()[3])
-                                                          for line in log_main if line.startswith("| Fermi energy:")])
-            line_vol = np.where(["Omega:" in line for line in log_file])[0][0]
-            volume = float(log_file[line_vol].split()[2]) \
-                * BOHR_TO_ANGSTROM ** 3
-            self._parse_dict["bands_occ"] = [
-                line.split()[3:]
-                for line in log_main
-                if line.startswith("| final focc:")
-            ]
-            self._parse_dict["bands_eigen_values"] = [
-                line.split()[4:]
-                for line in log_main
-                if line.startswith("| final eig [eV]:")
-            ]
-
-            def eig_converter(
-                arr,
-                magnetic=np.any(
-                    self._job.structure.get_initial_magnetic_moments() != None
-                ),
-                len_k_points=len(k_points),
-            ):
-                if len(arr) == 0:
-                    return np.array([])
-                elif magnetic:
-                    return np.array(
-                        [float(ff) for f in arr for ff in f]
-                    ).reshape(
-                        -1, 2, len_k_points, len(arr[0])
-                    )
-                else:
-                    return np.array(
-                        [float(ff) for f in arr for ff in f]
-                    ).reshape(
-                        -1, len_k_points, len(arr[0])
-                    )
-
-            self._parse_dict["bands_occ"] = eig_converter(
-                self._parse_dict["bands_occ"])
-            self._parse_dict["bands_eigen_values"] = eig_converter(
-                self._parse_dict["bands_eigen_values"]
-            )
-            energy_free_lst = self.splitter(energy_free, counter)
-            energy_int_lst = self.splitter(energy_int, counter)
-            energy_zero_lst = self.splitter(energy_zero, counter)
-            energy_band_lst = self.splitter(energy_band, counter)
-            if len(forces) != 0:
-                forces = np.array(forces).reshape(
-                    -1, len(self._job.structure), 3)
-                for ii, ff in enumerate(forces):
-                    forces[ii] = ff[self._job.id_spx_to_pyi]
-            if len(magnetic_forces) != 0:
-                magnetic_forces = np.array(magnetic_forces).reshape(
-                    -1, len(self._job.structure)
-                )
-                for ii, mm in enumerate(magnetic_forces):
-                    magnetic_forces[ii] = mm[self._job.id_spx_to_pyi]
-                magnetic_forces = self.splitter(magnetic_forces, counter)
-        if len(convergence) == len(energy_free_lst) - 1:
-            convergence.append(False)
-        self._parse_dict["scf_convergence"] = convergence
-        self._parse_dict["volume"] = np.array(len(convergence) * [volume])
-        if len(self._parse_dict["scf_energy_int"]) == 0 and \
-            len(energy_int_lst) != 0:
-            self._parse_dict["scf_energy_int"] = energy_int_lst
-        if len(self._parse_dict["scf_energy_free"]) == 0 and \
-            len(energy_free_lst) != 0:
-            self._parse_dict["scf_energy_free"] = energy_free_lst
-        if len(self._parse_dict["forces"]) == 0 and len(forces) != 0:
-            self._parse_dict["forces"] = forces
-        if len(self._parse_dict["scf_magnetic_forces"]) == 0 and \
-                len(magnetic_forces) != 0:
-            self._parse_dict["scf_magnetic_forces"] = magnetic_forces
+            log_file = "".join(sphinx_log_file.readlines())
+        try:
+            self._spx_log_parser = _SphinxLogParser(log_file)
+        except AssertionError as e:
+            self._job.status.aborted = True
+            raise AssertionError(e)
+        if not self._spx_log_parser.job_finished:
+            self._job.status.aborted = True
+        self.generic.dft.n_valence = self._spx_log_parser.get_n_valence()
+        self.generic.dft.bands_k_weights = self._spx_log_parser.get_bands_k_weights()
+        self.generic.dft.kpoints_cartesian = (
+            self._spx_log_parser.get_kpoints_cartesian()
+        )
+        self.generic.volume = self._spx_log_parser.get_volume()
+        self.generic.dft.bands_e_fermi = self._spx_log_parser.get_fermi()
+        self.generic.dft.bands_occ = self._spx_log_parser.get_occupancy()
+        self.generic.dft.bands_eigen_values = self._spx_log_parser.get_band_energy()
+        self.generic.dft.scf_convergence = self._spx_log_parser.get_convergence()
+        if "scf_energy_int" not in self.generic.dft.list_nodes():
+            self.generic.dft.scf_energy_int = self._spx_log_parser.get_energy_int()
+        if "scf_energy_free" not in self.generic.dft.list_nodes():
+            self.generic.dft.scf_energy_free = self._spx_log_parser.get_energy_free()
+        if "forces" in self.generic.list_nodes():
+            self.generic.forces = self._spx_log_parser.get_forces(
+                self._job.id_spx_to_pyi
+            )
+        if "scf_magnetic_forces" not in self.generic.dft.list_nodes():
+            self.generic.dft.scf_magnetic_forces = (
+                self._spx_log_parser.get_magnetic_forces(self._job.id_spx_to_pyi)
+            )
 
     def collect_relaxed_hist(self, file_name="relaxHist.sx", cwd=None):
         """
 
         Args:
             file_name:
             cwd:
 
         Returns:
 
         """
         file_name = posixpath.join(cwd, file_name)
         if not os.path.isfile(file_name):
             return None
-        with open(file_name, "r") as file_content:
-            file_content = file_content.readlines()
-            natoms = len(self._job.id_spx_to_pyi)
-            coords = np.array(
-                [
-                    json.loads(line.split("=")[1].split(";")[0])
-                    for line in file_content
-                    if "coords" in line
-                ]
-            )
-            self._parse_dict["positions"] = (
-                coords.reshape(-1, natoms, 3) * BOHR_TO_ANGSTROM
-            )
-            self._parse_dict["positions"] = np.array(
-                [ff[self._job.id_spx_to_pyi]
-                for ff in self._parse_dict["positions"]]
-            )
-            force = np.array(
-                [
-                    json.loads(line.split("=")[1].split(";")[0])
-                    for line in file_content
-                    if "force" in line
-                ]
-            )
-            self._parse_dict["forces"] = (
-                force.reshape(-1, natoms, 3) *
-                HARTREE_OVER_BOHR_TO_EV_OVER_ANGSTROM
-            )
-            self._parse_dict["forces"] = np.array(
-                [ff[self._job.id_spx_to_pyi]
-                for ff in self._parse_dict["forces"]]
-            )
-            self._parse_dict["cell"] = (
+        with open(file_name, "r") as f:
+            file_content = "".join(f.readlines())
+        natoms = len(self._job.id_spx_to_pyi)
+
+        def get_value(term, file_content=file_content, natoms=natoms):
+            value = (
                 np.array(
                     [
-                        json.loads(
-                            "".join(file_content[i_line : i_line + 3])
-                            .split("=")[1]
-                            .split(";")[0]
-                        )
-                        for i_line, line in enumerate(file_content)
-                        if "cell" in line
+                        re.split("\[|\]", line)[1].split(",")
+                        for line in re.findall(term, file_content, re.MULTILINE)
                     ]
                 )
-                * BOHR_TO_ANGSTROM
+                .astype(float)
+                .reshape(-1, natoms, 3)
+            )
+            return np.array([ff[self._job.id_spx_to_pyi] for ff in value])
+
+        self.generic.positions = get_value("coords.*$") * BOHR_TO_ANGSTROM
+        self.generic.forces = (
+            get_value("force.*$") * HARTREE_OVER_BOHR_TO_EV_OVER_ANGSTROM
+        )
+        self.generic.cells = (
+            np.array(
+                [
+                    json.loads(line)
+                    for line in re.findall(
+                        "cell =(.*?);", file_content.replace("\n", ""), re.MULTILINE
+                    )
+                ]
             )
+            * BOHR_TO_ANGSTROM
+        )
 
     def collect_charge_density(self, file_name, cwd):
         if (
             file_name in os.listdir(cwd)
             and os.stat(posixpath.join(cwd, file_name)).st_size != 0
         ):
             self.charge_density.from_file(
-                filename=posixpath.join(cwd, file_name),
-                normalize=True
+                filename=posixpath.join(cwd, file_name), normalize=True
             )
 
     def collect_electrostatic_potential(self, file_name, cwd):
         if (
-            file_name in os.listdir(cwd) and
-            os.stat(posixpath.join(cwd, file_name)).st_size != 0
+            file_name in os.listdir(cwd)
+            and os.stat(posixpath.join(cwd, file_name)).st_size != 0
         ):
             self.electrostatic_potential.from_file(
-                filename=posixpath.join(cwd, file_name),
-                normalize=False
+                filename=posixpath.join(cwd, file_name), normalize=False
             )
 
     def _get_electronic_structure_object(self):
         es = ElectronicStructure()
-        if len(self._parse_dict["bands_eigen_values"]) > 0:
-            eig_mat = self._parse_dict["bands_eigen_values"][-1]
-            occ_mat = self._parse_dict["bands_occ"][-1]
+        if "bands_eigen_values" in self.generic.dft.list_nodes():
+            eig_mat = self.generic.dft.bands_eigen_values[-1]
+            occ_mat = self.generic.dft.bands_occ[-1]
             if len(eig_mat.shape) == 3:
                 es.eigenvalue_matrix = eig_mat
                 es.occupancy_matrix = occ_mat
             else:
                 es.eigenvalue_matrix = np.array([eig_mat])
                 es.occupancy_matrix = np.array([occ_mat])
-            es.efermi = self._parse_dict["bands_e_fermi"][-1]
+            es.efermi = self.generic.dft.bands_e_fermi[-1]
             es.n_spins = len(es.occupancy_matrix)
-            es.kpoint_list = self._parse_dict["kpoints_cartesian"]
-            es.kpoint_weights = self._parse_dict["bands_k_weights"]
+            es.kpoint_list = self.generic.dft.kpoints_cartesian
+            es.kpoint_weights = self.generic.dft.bands_k_weights
             es.generate_from_matrices()
         return es
 
     def collect(self, directory=os.getcwd()):
         """
         The collect function, collects all the output from a SPHInX simulation.
 
         Args:
             directory (str): the directory to collect the output from.
         """
+        self.collect_energy_struct(file_name="energy-structOpt.dat", cwd=directory)
         self.collect_sphinx_log(file_name="sphinx.log", cwd=directory)
         self.collect_energy_dat(file_name="energy.dat", cwd=directory)
         self.collect_residue_dat(file_name="residue.dat", cwd=directory)
-        self.collect_eps_dat(file_name="eps.dat", cwd=directory)
+        if self._job._spin_enabled:
+            self.collect_eps_dat(file_name="eps.dat", cwd=directory)
+        else:
+            self.collect_eps_dat(
+                file_name=[f"eps.{i}.dat" for i in [0, 1]], cwd=directory
+            )
         self.collect_spins_dat(file_name="spins.dat", cwd=directory)
-        self.collect_energy_struct(file_name="energy-structOpt.dat",
-                                   cwd=directory)
         self.collect_relaxed_hist(file_name="relaxHist.sx", cwd=directory)
-        self.collect_electrostatic_potential(file_name="vElStat-eV.sxb",
-                                             cwd=directory)
-        self.collect_charge_density(file_name="rho.sxb",
-                                    cwd=directory)
+        self.collect_electrostatic_potential(file_name="vElStat-eV.sxb", cwd=directory)
+        self.collect_charge_density(file_name="rho.sxb", cwd=directory)
 
     def to_hdf(self, hdf, force_update=False):
         """
         Store output in an HDF5 file
 
         Args:
             hdf: HDF5 group
             force_update(bool):
         """
 
-        if len(self._parse_dict["scf_energy_zero"]) == 0:
-            self._parse_dict["scf_energy_zero"] = [
-                (0.5 * (np.array(fr) + np.array(en))).tolist()
-                for fr, en in zip(
-                    self._parse_dict["scf_energy_free"],
-                    self._parse_dict["scf_energy_int"],
-                )
-            ]
-        with hdf.open("input") as hdf5_input:
-            with hdf5_input.open("generic") as hdf5_generic:
-                if "dft" not in hdf5_generic.list_groups():
-                    hdf5_generic.create_group("dft")
-                with hdf5_generic.open("dft") as hdf5_dft:
-                    if (
-                        len(self._parse_dict["atom_spin_constrains"]) > 0
-                        and "atom_spin_constraints" not in
-                        hdf5_dft.list_nodes()
-                    ):
-                        hdf5_dft["atom_spin_constraints"] = [
-                            self._parse_dict["atom_spin_constrains"]
-                        ]
+        def get_last(arr):
+            return np.array([vv[-1] for vv in arr])
+
+        for k in self.generic.dft.list_nodes():
+            if "scf" in k and k != "scf_convergence":
+                self.generic.dft[k.replace("scf_", "")] = get_last(self.generic.dft[k])
+        if "energy_free" in self.generic.dft.list_nodes():
+            self.generic.energy_tot = self.generic.dft.energy_free
+            self.generic.energy_pot = self.generic.dft.energy_free
+        if "positions" not in self.generic.list_nodes():
+            self.generic.positions = np.array([self._job.structure.positions])
+        if "cells" not in self.generic.list_nodes():
+            self.generic.cells = np.array([self._job.structure.cell.tolist()])
+        self.generic.to_hdf(hdf=hdf)
 
         with hdf.open("output") as hdf5_output:
             if self.electrostatic_potential.total_data is not None:
                 self.electrostatic_potential.to_hdf(
                     hdf5_output, group_name="electrostatic_potential"
                 )
             if self.charge_density.total_data is not None:
-                self.charge_density.to_hdf(
-                    hdf5_output, group_name="charge_density"
-                )
-            if "bands_eigen_values" in self._parse_dict.keys():
+                self.charge_density.to_hdf(hdf5_output, group_name="charge_density")
+            if "bands_eigen_values" in self.generic.dft.list_nodes():
                 es = self._get_electronic_structure_object()
                 if len(es.kpoint_list) > 0:
                     es.to_hdf(hdf5_output)
             with hdf5_output.open("electronic_structure") as hdf5_es:
                 if "dos" not in hdf5_es.list_groups():
                     hdf5_es.create_group("dos")
                 with hdf5_es.open("dos") as hdf5_dos:
-                    warning_message = (
-                        ' is not stored in SPHInX; use job.get_density_of_states instead'
-                    )
-                    for k in ['energies', 'int_densities', 'tot_densities']:
-                        hdf5_dos[k] = k+warning_message
-            with hdf5_output.open("generic") as hdf5_generic:
-                if "dft" not in hdf5_generic.list_groups():
-                    hdf5_generic.create_group("dft")
-                with hdf5_generic.open("dft") as hdf5_dft:
-                    hdf5_dft["scf_convergence"] = \
-                        self._parse_dict["scf_convergence"]
-                    for k in [
-                        "scf_residue",
-                        "scf_energy_free",
-                        "scf_energy_zero",
-                        "scf_energy_int",
-                        "scf_electronic_entropy",
-                        "scf_energy_band",
-                        "scf_magnetic_forces",
-                        "scf_computation_time",
-                        "bands_occ",
-                        "bands_e_fermi",
-                        "bands_k_weights",
-                        "bands_eigen_values",
-                        "atom_scf_spins",
-                        "n_valence",
-                    ]:
-                        if len(self._parse_dict[k]) > 0:
-                            hdf5_dft[k] = self._parse_dict[k]
-                            if "scf_" in k:
-                                hdf5_dft[k.replace("scf_", "")] = np.array(
-                                    [vv[-1] for vv in self._parse_dict[k]]
-                                )
-                if len(self._parse_dict["scf_computation_time"]) > 0:
-                    hdf5_generic["computation_time"] = np.array(
-                        [tt[-1] for tt in
-                         self._parse_dict["scf_computation_time"]]
-                    )
-                if len([en[-1] for en in
-                    self._parse_dict["scf_energy_free"]]) > 0:
-                    hdf5_generic["energy_tot"] = np.array(
-                        [en[-1] for en in self._parse_dict["scf_energy_free"]]
-                    )
-                    hdf5_generic["energy_pot"] = np.array(
-                        [en[-1] for en in self._parse_dict["scf_energy_free"]]
-                    )
-                hdf5_generic["volume"] = self._parse_dict["volume"]
-                if "positions" not in hdf5_generic.list_nodes() or \
-                    force_update:
-                    if len(self._parse_dict["positions"]) > 0:
-                        hdf5_generic["positions"] = np.array(
-                            self._parse_dict["positions"]
-                        )
-                    elif len(self._parse_dict["scf_convergence"]) == 1:
-                        hdf5_generic["positions"] = np.array(
-                            [self._job.structure.positions]
-                        )
-                if ("forces" not in hdf5_generic.list_nodes() or force_update)\
-                    and len(
-                    self._parse_dict["forces"]
-                ) > 0:
-                    hdf5_generic["forces"] = \
-                        np.array(self._parse_dict["forces"])
-                if "cells" not in hdf5_generic.list_nodes() or force_update:
-                    if len(self._parse_dict["cell"]) > 0:
-                        hdf5_generic["cells"] = np.array(
-                            self._parse_dict["cell"])
-                    elif len(self._parse_dict["scf_convergence"]) == 1:
-                        hdf5_generic["cells"] = np.array(
-                            [self._job.structure.cell])
+                    warning_message = " is not stored in SPHInX; use job.get_density_of_states instead"
+                    for k in ["energies", "int_densities", "tot_densities"]:
+                        hdf5_dos[k] = k + warning_message
 
     def from_hdf(self, hdf):
         """
         Load output from an HDF5 file
         """
-        pass
+        try:
+            self.generic.from_hdf(hdf=hdf)
+        except ValueError:
+            warnings.warn(
+                "You are using an old version of SPHInX output - update via job.update_sphinx()"
+            )
+            self.old_version = True
+            pass
+
+
+def _update_datacontainer(job):
+    job.output.generic.create_group("dft")
+    for node in job["output/generic/dft"].list_nodes():
+        job.output.generic.dft[node] = job["output/generic/dft"][node]
+    for node in job["output/generic"].list_nodes():
+        job.output.generic[node] = job["output/generic"][node]
+    job["output/generic"].remove_group()
+    job.output.generic.to_hdf(hdf=job.project_hdf5)
+    job.output.old_version = False
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/interactive.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/interactive.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 
 import numpy as np
 import os
 import scipy.constants
 import subprocess
 import warnings
 import time
-from pyiron_atomistics.sphinx.base import SphinxBase, Group
-from pyiron_atomistics.atomistics.job.interactive import GenericInteractive, GenericInteractiveOutput
+from pyiron_atomistics.sphinx.base import SphinxBase, Group, Output
+from pyiron_atomistics.atomistics.job.interactive import (
+    GenericInteractive,
+    GenericInteractiveOutput,
+)
 from pyiron_atomistics.vasp.potential import VaspPotentialSetter
 
 BOHR_TO_ANGSTROM = (
     scipy.constants.physical_constants["Bohr radius"][0] / scipy.constants.angstrom
 )
 HARTREE_TO_EV = scipy.constants.physical_constants["Hartree energy in eV"][0]
 HARTREE_OVER_BOHR_TO_EV_OVER_ANGSTROM = HARTREE_TO_EV / BOHR_TO_ANGSTROM
@@ -29,35 +32,35 @@
 __status__ = "development"
 __date__ = "Sep 1, 2017"
 
 
 class SphinxInteractive(SphinxBase, GenericInteractive):
     def __init__(self, project, job_name):
         super(SphinxInteractive, self).__init__(project, job_name)
-        self.output = SphinxOutput(job=self)
         self._interactive_write_input_files = True
         self._interactive_library_read = None
         self._interactive_fetch_completed = True
         self.interactive_flush_frequency = 1
+        self.output = SphinxOutput(job=self)
 
     @property
     def structure(self):
         return GenericInteractive.structure.fget(self)
 
     @structure.setter
     def structure(self, structure):
         GenericInteractive.structure.fset(self, structure)
         if structure is not None:
             self._potential = VaspPotentialSetter(
                 element_lst=structure.get_species_symbols().tolist()
             )
 
-    def get_structure(self, iteration_step=-1, wrap_atoms=True):
-        return GenericInteractive.get_structure(
-            self, iteration_step=iteration_step, wrap_atoms=wrap_atoms
+    def _get_structure(self, frame=-1, wrap_atoms=True):
+        return GenericInteractive._get_structure(
+            self, frame=frame, wrap_atoms=wrap_atoms
         )
 
     def interactive_energy_tot_getter(self):
         return self.interactive_energy_pot_getter()
 
     def interactive_energy_pot_getter(self):
         self._interactive_pipe_write("get energy")
@@ -173,15 +176,15 @@
             os.path.join(self.working_directory, "sxctrl"), "w"
         )
         self._interactive_library_read = open(
             os.path.join(self.working_directory, "sxres"), "r"
         )
         self._logger.debug("interactive interface is opened!")
         if (
-            np.all(self.structure.get_initial_magnetic_moments() == None)
+            not self.structure.has("initial_magmoms")
             and "atom_spins" in self.interactive_cache.keys()
         ):
             del self.interactive_cache["atom_spins"]
         if self._generic_input["fix_spin_constraint"]:
             self.interactive_spin_constraints_setter(
                 self._structure_current.get_initial_magnetic_moments()
             )
@@ -195,30 +198,25 @@
             self._interactive_pipe_write("run restart")
             self.interactive_fetch()
 
     def _output_interactive_to_generic(self):
         with self.project_hdf5.open("output") as h5:
             if "interactive" in h5.list_groups():
                 for key in ["positions", "cells", "indices", "cells", "forces"]:
-                    h5["generic/" + key] = h5["interactive/" + key]
-                with self.project_hdf5.open("input") as hdf5_input:
-                    with hdf5_input.open("generic") as hdf5_generic:
-                        if "dft" not in hdf5_generic.list_groups():
-                            hdf5_generic.create_group("dft")
-                        with hdf5_generic.open("dft") as hdf5_dft:
-                            if (
-                                "atom_spin_constraints"
-                                in h5["interactive"].list_nodes()
-                            ):
-                                hdf5_dft["atom_spin_constraints"] = h5[
-                                    "interactive/atom_spin_constraints"
-                                ]
+                    self.output.generic[key] = h5["interactive/" + key]
+                if "atom_spin_constraints" in h5["interactive"].list_nodes():
+                    self.output.generic.dft.atom_spin_constraints = h5[
+                        "interactive/atom_spin_constraints"
+                    ]
+                self.output.generic.to_hdf(hdf=self.project_hdf5)
 
     def collect_output(self, force_update=False, compress_files=True):
-        super(SphinxInteractive, self).collect_output(force_update=force_update, compress_files=compress_files)
+        super(SphinxInteractive, self).collect_output(
+            force_update=force_update, compress_files=compress_files
+        )
         self._output_interactive_to_generic()
 
     def interactive_close(self):
         if self.interactive_is_activated():
             self._interactive_pipe_write("end")
             self._interactive_library.close()
             self._interactive_library_read.close()
@@ -233,16 +231,16 @@
         electronic_steps=None,
         ionic_steps=None,
         max_iter=None,
         pressure=None,
         algorithm=None,
         retain_charge_density=False,
         retain_electrostatic_potential=False,
-        ionic_energy_tolerance=0.0,
-        ionic_force_tolerance=1.0e-2,
+        ionic_energy_tolerance=None,
+        ionic_force_tolerance=None,
         ionic_energy=None,
         ionic_forces=None,
         volume_only=False,
     ):
         if (
             self.server.run_mode.interactive
             or self.server.run_mode.interactive_non_modal
@@ -335,70 +333,75 @@
 
     def load_main_group(self):
         main_group = Group()
         if (
             self.server.run_mode.interactive
             or self.server.run_mode.interactive_non_modal
         ):
-            commands = Group([
-                {
-                    "id": '"restart"',
-                    "scfDiag":
-                        self.get_scf_group(
+            commands = Group(
+                [
+                    {
+                        "id": '"restart"',
+                        "scfDiag": self.get_scf_group(
                             maxSteps=10, keepRhoFixed=True, dEnergy=1.0e-4
-                        )
-                }, {
-                    "id": '"electronicminimization"',
-                    "scfDiag": self.get_scf_group(),
-                }
-            ])
+                        ),
+                    },
+                    {
+                        "id": '"electronicminimization"',
+                        "scfDiag": self.get_scf_group(),
+                    },
+                ]
+            )
             self.input.sphinx.main.extControl = Group()
-            self.input.sphinx.main.extControl.set_group('bornOppenheimer')
+            self.input.sphinx.main.extControl.set_group("bornOppenheimer")
             self.input.sphinx.main.extControl.bornOppenheimer = commands
         else:
             super(SphinxInteractive, self).load_main_group()
 
 
-class SphinxOutput(GenericInteractiveOutput):
-    def __init__(self, job):
-        super(SphinxOutput, self).__init__(job)
+class SphinxOutput(Output, GenericInteractiveOutput):
+    """
+    Handles the output from a SPHInX simulation.
+    """
 
     def check_band_occupancy(self, plot=True):
         """
-            Check whether there are still empty bands available.
+        Check whether there are still empty bands available.
 
-            args:
-                plot (bool): plots occupancy of the last step
+        args:
+            plot (bool): plots occupancy of the last step
 
-            returns:
-                True if there are still empty bands
+        returns:
+            True if there are still empty bands
         """
         import matplotlib.pylab as plt
-        elec_dict = self._job['output/generic/dft']['n_valence']
+
+        elec_dict = self._job["output/generic/dft"]["n_valence"]
         if elec_dict is None:
-            raise AssertionError('Number of electrons not parsed')
-        n_elec = np.sum([elec_dict[k]
-                         for k in self._job.structure.get_chemical_symbols()])
-        n_elec = int(np.ceil(n_elec/2))
-        bands = self._job['output/generic/dft/bands_occ'][-1]
+            raise AssertionError("Number of electrons not parsed")
+        n_elec = np.sum(
+            [elec_dict[k] for k in self._job.structure.get_chemical_symbols()]
+        )
+        n_elec = int(np.ceil(n_elec / 2))
+        bands = self._job["output/generic/dft/bands_occ"][-1]
         bands = bands.reshape(-1, bands.shape[-1])
-        max_occ = np.sum(bands>0, axis=-1).max()
+        max_occ = np.sum(~np.isclose(bands, 0), axis=-1).max()
         n_bands = bands.shape[-1]
         if plot:
-            xticks = np.arange(1, n_bands+1)
-            plt.xlabel('Electron number')
-            plt.ylabel('Occupancy')
-            if n_bands<20:
+            xticks = np.arange(1, n_bands + 1)
+            plt.xlabel("Electron number")
+            plt.ylabel("Occupancy")
+            if n_bands < 20:
                 plt.xticks(xticks)
-            plt.axvline(n_elec, label='#electrons: {}'.format(n_elec))
-            plt.axvline(max_occ, color='red',
-                label='Max occupancy: {}'.format(max_occ))
-            plt.axvline(n_bands, color='green',
-                label='Number of bands: {}'.format(n_bands))
-            plt.plot(xticks, bands.T, 'x', color='black')
+            plt.axvline(n_elec, label="#electrons: {}".format(n_elec))
+            plt.axvline(max_occ, color="red", label="Max occupancy: {}".format(max_occ))
+            plt.axvline(
+                n_bands, color="green", label="Number of bands: {}".format(n_bands)
+            )
+            plt.plot(xticks, bands.T, "x", color="black")
             plt.legend()
         if max_occ < n_bands:
             return True
         else:
             return False
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/potential.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/potential.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import os
 import pandas
-from pyiron_base import Settings
-from pyiron_atomistics.vasp.potential import VaspPotentialAbstract, find_potential_file_base
+from pyiron_base import state
+from pyiron_atomistics.vasp.potential import (
+    VaspPotentialAbstract,
+    find_potential_file_base,
+)
 
 __author__ = "Osamu Waseda"
 __copyright__ = (
     "Copyright 2019, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Osamu Waseda"
 __email__ = "waseda@mpie.de"
 __status__ = "development"
 __date__ = "Sep 20, 2019"
 
-s = Settings()
-
 
 class SphinxJTHPotentialFile(VaspPotentialAbstract):
     """
     The Potential class is derived from the PotentialAbstract class, but instead of loading the potentials from a list,
     the potentials are loaded from a file.
 
     Args:
         xc (str): Exchange correlation functional ['PBE', 'LDA']
     """
+
     def __init__(self, xc=None, selected_atoms=None):
         potential_df = self._get_potential_df(
             plugin_name="sphinx",
             file_name_lst={"potentials_sphinx.csv"},
             backward_compatibility_name="sphinxpotentials",
         )
         if xc == "PBE":
@@ -74,18 +76,18 @@
         ds.name = new_element
         ds["Name"] = "-".join(name_list)
         self._default_df = self._default_df.append(ds)
 
 
 def find_potential_file(path):
     env = os.environ
-    resource_path_lst = s.resource_paths
+    resource_path_lst = state.settings.resource_paths
     for conda_var in ["CONDA_PREFIX", "CONDA_DIR"]:
         if conda_var in env.keys():  # support sphinx-data package
             path_to_add = os.path.join(env[conda_var], "share", "sphinxdft")
             if path_to_add not in resource_path_lst:
                 resource_path_lst += [path_to_add]
     return find_potential_file_base(
         path=path,
         resource_path_lst=resource_path_lst,
-        rel_path=os.path.join("sphinx", "potentials")
+        rel_path=os.path.join("sphinx", "potentials"),
     )
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/structure.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,15 @@
                 k = 0
                 if "atom" in line_str:
                     break_loop = False
                     while not break_loop:
                         position_string = " ".join(
                             file_string[i + j + k].split("=")[-1]
                         )
-                        replace_list = ["[", "]", ";", "}",
-                            "movable", "X", "Y", "Z"]
+                        replace_list = ["[", "]", ";", "}", "movable", "X", "Y", "Z"]
                         for rep in replace_list:
                             position_string = (
                                 "".join(position_string).replace(rep, " ").split()
                             )
                         positions.append(
                             np.array(position_string[0].split(","), dtype=float)
                         )
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/volumetric_data.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/volumetric_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
 import scipy
 from scipy.io.netcdf import netcdf_file
 import os
-from pyiron_base import Settings
+from pyiron_base import state
 from pyiron_atomistics.atomistics.volumetric.generic import VolumetricData
 
 __author__ = "Sudarsan Surendralal"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -18,59 +18,52 @@
 __maintainer__ = "Sudarsan Surendralal"
 __email__ = "surendralal@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 
 BOHR_TO_ANGSTROM = (
-    scipy.constants.physical_constants["Bohr radius"][0] /
-    scipy.constants.angstrom
+    scipy.constants.physical_constants["Bohr radius"][0] / scipy.constants.angstrom
 )
 
 
 class SphinxVolumetricData(VolumetricData):
     """
     General class for parsing and manipulating volumetric static within Sphinx.
 
     The basic idea of the Base class is adapted from the pymatgen vasp
     VolumetricData class:
 
     http://pymatgen.org/_modules/pymatgen/io/vasp/outputs.html#VolumetricData
 
     """
 
-
     def __init__(self):
         super(SphinxVolumetricData, self).__init__()
         self.atoms = None
         self._diff_data = None
         self._total_data = None
 
-
     def from_file(self, filename, normalize=True):
         """
         Parses volumetric data from a sphinx binary (.sxb) file.
 
         Args:
             filename (str): Path of file to parse
             normalize (boolean): Flag to normalize by the volume of the cell
         """
         try:
-            vol_data_list = self._read_vol_data(
-                filename=filename,
-                normalize=normalize
-            )
+            vol_data_list = self._read_vol_data(filename=filename, normalize=normalize)
         except (ValueError, IndexError, TypeError):
             raise ValueError("Unable to parse file: {}".format(filename))
         self._total_data = vol_data_list[0]
         if len(vol_data_list) == 2:
             self._total_data = vol_data_list[0] + vol_data_list[1]
             self._diff_data = vol_data_list[0] - vol_data_list[1]
 
-
     @staticmethod
     def _read_vol_data(filename, normalize=True):
         """
         Parses the Sphinx volumetric data files (rho.sxb and vElStat-eV.sxb).
 
         Args:
             filename (str): File to be parsed
@@ -79,16 +72,15 @@
 
         Returns:
             list: A list of the volumetric data (length >1 for density
                 files with spin)
 
         """
         if not os.path.getsize(filename) > 0:
-            s = Settings()
-            s.logger.warning("File:" + filename + "seems to be empty! ")
+            state.logger.warning("File:" + filename + "seems to be empty! ")
             return None, None
 
         with netcdf_file(filename, mmap=False) as f:
             dim = [int(d) for d in f.variables["dim"]]
             volume = 1.0
             if normalize:
                 cell = f.variables["cell"].data * BOHR_TO_ANGSTROM
@@ -98,55 +90,48 @@
                 total_data_list = [
                     np.array(f.variables["mesh"][:]).reshape(dim) / volume
                 ]
             elif "mesh-0" in f.variables and "mesh-1" in f.variables:
                 # spin-polarized
                 total_data_list = [
                     np.array(f.variables["mesh-0"][:]).reshape(dim) / volume,
-                    np.array(f.variables["mesh-1"][:]).reshape(dim) / volume
+                    np.array(f.variables["mesh-1"][:]).reshape(dim) / volume,
                 ]
             else:
                 raise ValueError(
                     "Unexpected keys in the netcdf file's variables: neither "
                     f"'mesh' nor 'mesh-0' and 'mesh-1' found in {f.variables}."
                 )
 
         if len(total_data_list) == 0:
-            s = Settings()
-            s.logger.warning(
-                "File:"
-                + filename
-                + "seems to be corrupted/empty even after parsing!"
+            state.logger.warning(
+                "File:" + filename + "seems to be corrupted/empty even after parsing!"
             )
             return None
 
         return total_data_list
 
-
     @property
     def total_data(self):
         """
         numpy.ndarray: Total volumtric data (3D)
         """
         return self._total_data
 
-
     @total_data.setter
     def total_data(self, val):
         self._total_data = val
 
-
     @property
     def diff_data(self):
         """
         numpy.ndarray: Volumtric difference data (3D)
         """
         return self._diff_data
 
-
     @diff_data.setter
     def diff_data(self, val):
         self._diff_data = val
 
     def to_hdf(self, hdf, group_name="volumetric_data"):
         """
         Writes the data as a group to a HDF5 file
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/table/funct.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/table/funct.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from pyiron_atomistics.atomistics.structure.atoms import Atoms, pyiron_to_ase
 
 
 def _get_value_from_incar(job, key):
     value = job["input/incar/data_dict"]["Value"][
         job["input/incar/data_dict"]["Parameter"].index(key)
-    ]   
+    ]
     if isinstance(value, str):
         return ast.literal_eval(value)
     else:
         return value
 
 
 def get_majority(lst, minority=False):
@@ -54,50 +54,54 @@
 
 
 def get_n_kpts(job):
     return {"n_kpts": eval(job["input/kpoints/data_dict"]["Value"][3].split()[0])}
 
 
 def get_n_equ_kpts(job):
-    return {"n_equ_kpts": len(job['output/generic/dft/bands/k_points'])}
+    return {"n_equ_kpts": len(job["output/generic/dft/bands/k_points"])}
 
 
 def get_total_number_of_atoms(job):
     return {"Number_of_atoms": len(job["input/structure/indices"])}
 
 
 def get_average_waves(job):
-    _, weights, planewaves = job["output/outcar/irreducible_kpoints"]
+    weights = job["output/outcar/irreducible_kpoint_weights"]
+    planewaves = job["output/outcar/number_plane_waves"]
     return {"avg. plane waves": sum(weights * planewaves) / sum(weights)}
 
 
 def get_plane_waves(job):
     _, weights, planewaves = job["output/outcar/irreducible_kpoints"]
     return {"plane waves": sum(weights * planewaves)}
 
 
 def get_ekin_error(job):
-    return {"energy_tot_wo_kin_corr": job["output/outcar/kin_energy_error"] + job["output/generic/energy_tot"][-1]}
+    return {
+        "energy_tot_wo_kin_corr": job["output/outcar/kin_energy_error"]
+        + job["output/generic/energy_tot"][-1]
+    }
 
 
 def get_volume(job):
     return {"volume": job["output/generic/volume"][-1]}
 
 
 def get_volume_per_atom(job):
-    return {"volume": job["output/generic/volume"][-1] / get_total_number_of_atoms(job=job)["Number_of_atoms"]}
+    return {
+        "volume": job["output/generic/volume"][-1]
+        / get_total_number_of_atoms(job=job)["Number_of_atoms"]
+    }
 
 
 def get_elements(job):
     species = job["input/structure/species"]
-    indices_lst = job["input/structure/indices"]
-    indices_set = set(indices_lst)
-    count_lst = [indices_lst.tolist().count(ind) for ind in indices_set]
-    main_element = species[count_lst.index(np.max(count_lst))]
-    return {species[ind]: count_lst[ind] for ind in indices_set}
+    indices = job["input/structure/indices"]
+    return {s: sum(indices == i) for i, s in enumerate(species)}
 
 
 def get_convergence_check(job):
     try:
         conv = job.project.load(job.job_id).convergence_check()
     except:
         conv = None
@@ -131,55 +135,64 @@
 
 def get_majority_crystal_structure(job):
     basis = Atoms().from_hdf(job["input"])
     majority_element = basis.get_majority_species()["symbol"]
     majority_index = [
         ind for ind, el in enumerate(basis) if el.symbol == majority_element
     ]
-    type_list = list(basis[majority_index].analyse.pyscal_cna_adaptive(
-        mode="str",
-        ovito_compatibility=True
-    ))
+    type_list = list(
+        basis[majority_index].analyse.pyscal_cna_adaptive(
+            mode="str", ovito_compatibility=True
+        )
+    )
     return {"crystal_structure": get_majority(type_list, minority=False)}
 
 
 def get_job_name(job):
     return {"job_name": job.job_name}
 
 
-def get_job_id(job):
-    return {"job_id": job.job_id}
-
-
 def get_energy_tot_per_atom(job):
-    return {"energy_tot": job["output/generic/energy_tot"][-1] / get_total_number_of_atoms(job=job)["Number_of_atoms"]}
+    return {
+        "energy_tot": job["output/generic/energy_tot"][-1]
+        / get_total_number_of_atoms(job=job)["Number_of_atoms"]
+    }
 
 
 def get_energy_tot(job):
     return {"energy_tot": job["output/generic/energy_tot"][-1]}
 
 
 def get_energy_pot_per_atom(job):
-    return {"energy_pot": job["output/generic/energy_pot"][-1] / get_total_number_of_atoms(job=job)["Number_of_atoms"]}
+    return {
+        "energy_pot": job["output/generic/energy_pot"][-1]
+        / get_total_number_of_atoms(job=job)["Number_of_atoms"]
+    }
 
 
 def get_energy_pot(job):
     return {"energy_pot": job["output/generic/energy_pot"][-1]}
 
 
 def get_energy_free_per_atom(job):
-    return {"energy_free": job["output/generic/dft/energy_free"][-1] / get_total_number_of_atoms(job=job)["Number_of_atoms"]}
+    return {
+        "energy_free": job["output/generic/dft/energy_free"][-1]
+        / get_total_number_of_atoms(job=job)["Number_of_atoms"]
+    }
 
 
 def get_energy_free(job):
     return {"energy_free": job["output/generic/dft/energy_free"][-1]}
 
 
 def get_energy_int_per_atom(job):
-    return {"energy_int": job["output/generic/dft/energy_int"][-1] / get_total_number_of_atoms(job=job)["Number_of_atoms"]}
+    return {
+        "energy_int": job["output/generic/dft/energy_int"][-1]
+        / get_total_number_of_atoms(job=job)["Number_of_atoms"]
+    }
 
 
 def get_energy_int(job):
     return {"energy_int": job["output/generic/dft/energy_int"][-1]}
 
 
 def get_f_states(job):
@@ -221,15 +234,15 @@
             "equilibrium_bulk_modulus",
             "equilibrium_volume",
         ]
     }
 
 
 def get_structure(job):
-    atoms = pyiron_to_ase(job.load_object().get_structure())
+    atoms = pyiron_to_ase(job.to_object().get_structure())
     atoms_dict = {
         "symbols": atoms.get_chemical_symbols(),
         "positions": atoms.get_positions().tolist(),
         "cell": atoms.get_cell().tolist(),
         "pbc": atoms.get_pbc().tolist(),
         "celldisp": atoms.get_celldisp().tolist(),
     }
@@ -269,11 +282,15 @@
         elif abs_sum_mag > 0 and sum_mag == 0:
             return {"magnetic_structure": "para-magnetic"}
         else:
             return {"magnetic_structure": "unknown"}
 
 
 def get_e_conv_level(job):
-    return {'el_conv': np.max(np.abs(
-        job['output/generic/dft/scf_energy_free'][0] -
-        job['output/generic/dft/scf_energy_free'][0][-1]
-    )[-10:])}
+    return {
+        "el_conv": np.max(
+            np.abs(
+                job["output/generic/dft/scf_energy_free"][0]
+                - job["output/generic/dft/scf_energy_free"][0][-1]
+            )[-10:]
+        )
+    }
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/testing/executable.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/testing/executable.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/testing/randomatomistic.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/testing/randomatomistic.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from __future__ import print_function
 import numpy as np
 import posixpath
 from pyiron_base import GenericParameters, GenericJob, Logstatus
 from pyiron_atomistics.atomistics.job.interactive import GenericInteractive
 from pyiron_atomistics.testing.executable import ExampleExecutable
 from collections import defaultdict
+import pint
+
 
 """
 Example Job class for testing the pyiron classes
 """
 
 __author__ = "Joerg Neugebauer, Jan Janssen"
 __copyright__ = (
@@ -115,15 +117,15 @@
             Job type object with all the available job types: ['ExampleJob', 'SerialMaster', 'ParallelMaster', 'ScriptJob',
                                                                'ListMaster']
     """
 
     def __init__(self, project, job_name):
         super(ExampleJob, self).__init__(project, job_name)
         self.__version__ = "0.3"
-        self.__name__ = "ExampleJob"
+
         self.input = ExampleInput()
         self.executable = "python -m pyiron_atomistics.testing.executable"
         self.interactive_cache = {"alat": [], "count": [], "energy": []}
 
     def set_input_to_read_only(self):
         """
         This function enforces read-only mode for the input classes, but it has to be implement in the individual
@@ -263,22 +265,25 @@
         )
 
     def load_default(self):
         """
         Loading the default settings for the input file.
         """
         input_str = """\
-alat  3.2     # lattice constant (would be in a more realistic example in the structure file)
-alpha 0.1     # noise amplitude
-a_0   3       # equilibrium lattice constant
-a_1   0
-a_2   1.0     # 2nd order in energy (corresponds to bulk modulus)
-a_3   0.0     # 3rd order
-a_4   0.0     # 4th order
-count 10      # number of calls (dummy)
+alat    3.2     # lattice constant (would be in a more realistic example in the structure file)
+alpha   0.1     # noise amplitude
+a_0     3       # equilibrium lattice constant
+a_1     0
+a_2     1.0     # 2nd order in energy (corresponds to bulk modulus)
+a_3     0.0     # 3rd order
+a_4     0.0     # 4th order
+count   10      # number of calls (dummy)
+epsilon 0.2     # energy prefactor of lennard jones
+sigma   2.4     # distance unit of lennard jones
+cutoff  4.0     # cutoff length (relative to sigma)
 write_restart True
 read_restart False
 """
         self.load_string(input_str)
 
 
 class AtomisticExampleJob(ExampleJob, GenericInteractive):
@@ -370,37 +375,49 @@
             Job type object with all the available job types: ['ExampleJob', 'SerialMaster', 'ParallelMaster', 'ScriptJob',
                                                                'ListMaster']
     """
 
     def __init__(self, project, job_name):
         super(AtomisticExampleJob, self).__init__(project, job_name)
         self.__version__ = "0.3"
-        self.__name__ = "AtomisticExampleJob"
+
         self.input = ExampleInput()
         self.executable = "python -m pyiron_atomistics.testing.executable"
-        self._internal_energy = None
         self.interactive_cache = defaultdict(list)
+        self._velocity = None
+        self._neigh = None
+        self._unit = pint.UnitRegistry()
+
+    @property
+    def neigh(self):
+        if self._neigh is None:
+            self._neigh = self.structure.get_neighbors(
+                num_neighbors=None,
+                cutoff_radius=self.input["cutoff"] * self.input["sigma"],
+            )
+        return self._neigh
 
     @property
     def structure(self):
         """
 
         Returns:
 
         """
         return self._structure
 
-    def get_structure(self, iteration_step=-1, wrap_atoms=True):
+    def _get_structure(self, frame=-1, wrap_atoms=True):
         try:
-            return super(AtomisticExampleJob, self).get_structure(
-                iteration_step=iteration_step, wrap_atoms=wrap_atoms
-            )
+            return super()._get_structure(frame=frame, wrap_atoms=wrap_atoms)
         except IndexError:
             return self.structure
 
+    def _number_of_structures(self):
+        return max(1, super()._number_of_structures())
+
     @structure.setter
     def structure(self, structure):
         """
 
         Args:
             structure:
 
@@ -441,59 +458,122 @@
         """
         super(AtomisticExampleJob, self).from_hdf(hdf=hdf, group_name=group_name)
         self._structure_from_hdf()
 
     def interactive_cells_getter(self):
         return self._structure.cell.copy()
 
+    @property
+    def _s_r(self):
+        return self.input["sigma"] / self.neigh.flattened.distances
+
     def interactive_energy_pot_getter(self):
-        return self._internal_energy
+        return self.input["epsilon"] * (
+            np.sum(self._s_r**12) - np.sum(self._s_r**6)
+        )
 
     def interactive_energy_tot_getter(self):
-        return self._internal_energy
+        return (
+            self.interactive_energy_pot_getter() + self.interadtive_energy_kin_getter()
+        )
+
+    def interadtive_energy_kin_getter(self):
+        v = np.einsum("ni,n->", self._velocity**2, self.structure.get_masses()) / 2
+        return (
+            (
+                v
+                * self._unit.angstrom**2
+                / self._unit.second**2
+                / 1e-30
+                * self._unit.amu
+            )
+            .to("eV")
+            .magnitude
+        )
 
     def interactive_forces_getter(self):
-        return np.random.random((len(self._structure), 3))
+        all_values = self.input["epsilon"] * np.einsum(
+            "ni,n,n->ni",
+            self.neigh.flattened.vecs,
+            1 / self.neigh.flattened.distances**2,
+            12 * self._s_r**12 - 6 * self._s_r**6,
+        )
+        forces = np.zeros_like(self.structure.positions)
+        np.add.at(forces, self.neigh.flattened.atom_numbers, all_values)
+        return forces
 
     def interactive_positions_getter(self):
         return self._structure.positions
 
     def interactive_pressures_getter(self):
-        return np.random.random((3, 3))
+        pot_part = (
+            self.input["epsilon"]
+            * np.einsum(
+                "ni,nj,n,n->ij",
+                self.neigh.flattened.vecs,
+                self.neigh.flattened.vecs,
+                1 / self.neigh.flattened.distances**2,
+                12 * self._s_r**12 - 6 * self._s_r**6,
+            )
+            * self._unit.electron_volt
+        )
+        kin_part = (
+            np.einsum(
+                "ni,nj,n->ij",
+                self._velocity,
+                self._velocity,
+                self.structure.get_masses(),
+            )
+            * self._unit.angstrom**2
+            / self._unit.second**2
+            / 1e-30
+            * self._unit.amu
+        )
+        return (
+            (pot_part + kin_part)
+            / self.structure.get_volume()
+            / self._unit.angstrom**3
+        ).to(self._unit.pascal).magnitude / 1e9
 
     def interactive_stress_getter(self):
         return np.random.random((len(self._structure), 3, 3))
 
     def interactive_steps_getter(self):
         return len(self.interactive_cache["steps"])
 
     def interactive_temperatures_getter(self):
-        return np.random.random()
+        value = self.interadtive_energy_kin_getter() / len(self.structure)
+        return (
+            (value / self._unit.boltzmann_constant * self._unit.electron_volt)
+            .to("kelvin")
+            .magnitude
+        )
 
     def interactive_indices_getter(self):
         return self._structure.indices
 
     def interactive_computation_time_getter(self):
         return np.random.random()
 
     def interactive_unwrapped_positions_getter(self):
         return self._structure.positions
 
     def interactive_volume_getter(self):
         return self._structure.get_volume()
 
-    def interactive_execute(self):
-        _, _, self._internal_energy = ExampleExecutable().run_lib(self.input)
-
     def interactive_initialize_interface(self):
         self._interactive_library = True
 
     def run_if_interactive(self):
         """
         Run the job as Python library and store the result in the HDF5 File.
 
         Returns:
             int: job ID
         """
+        self._neigh = None
+        if self._generic_input["calc_mode"] == "md":
+            self._velocity = np.random.randn(len(self._structure), 3) / 1000
+        elif self._velocity is None:
+            self._velocity = np.zeros((len(self._structure), 3))
         GenericInteractive.run_if_interactive(self)
-        self.interactive_execute()
         self.interactive_collect()
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/thermodynamics/hessian.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/thermodynamics/hessian.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
 from pyiron_atomistics.atomistics.structure.atoms import Atoms
 from pyiron_atomistics.atomistics.job.interactive import GenericInteractive
 
 __author__ = "Jan Janssen"
-__copyright__ = "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH " \
-                "- Computational Materials Design (CM) Department"
+__copyright__ = (
+    "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH "
+    "- Computational Materials Design (CM) Department"
+)
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "development"
 __date__ = "Feb 20, 2020"
 
 
 class HessianJob(GenericInteractive):
     def __init__(self, project, job_name):
         super(HessianJob, self).__init__(project, job_name)
         self.__version__ = "0.0.1"
-        self.__name__ = "HessianJob"
+
         self._python_only_job = True
         self._force_constants = None
         self._reference_structure = None
         self._energy_pot = 0
         self._forces = np.zeros(3)
         self._pressure = np.zeros((3, 3))
         self._stiffness_tensor = np.zeros((6, 6))
@@ -46,55 +48,64 @@
         self.interactive_open()
         self.run_if_interactive()
         self.interactive_close()
         self.server.run_mode = run_mode
 
     def set_elastic_moduli(self, bulk_modulus=0, shear_modulus=0):
         self._stiffness_tensor = np.zeros((6, 6))
-        self._stiffness_tensor[:3, :3] = bulk_modulus-2*shear_modulus/3
-        self._stiffness_tensor[:3, :3] += np.eye(3)*2*shear_modulus
-        self._stiffness_tensor[3:, 3:] = np.eye(3)*shear_modulus
+        self._stiffness_tensor[:3, :3] = bulk_modulus - 2 * shear_modulus / 3
+        self._stiffness_tensor[:3, :3] += np.eye(3) * 2 * shear_modulus
+        self._stiffness_tensor[3:, 3:] = np.eye(3) * shear_modulus
 
     def set_force_constants(self, force_constants):
         if self.structure is None:
-            raise ValueError('Set reference structure via set_reference_structure() first')
+            raise ValueError(
+                "Set reference structure via set_reference_structure() first"
+            )
         n_atom = len(self.structure.positions)
         if len(np.array([force_constants]).flatten()) == 1:
-            self._force_constants = force_constants*np.eye(3*n_atom)
-        elif np.array(force_constants).shape == (3*n_atom, 3*n_atom):
+            self._force_constants = force_constants * np.eye(3 * n_atom)
+        elif np.array(force_constants).shape == (3 * n_atom, 3 * n_atom):
             self._force_constants = force_constants
         elif np.array(force_constants).shape == (n_atom, n_atom):
             na = np.newaxis
-            self._force_constants = (np.array(force_constants)[:, na, :, na]*np.eye(3)[na, :, na, :]).flatten()
+            self._force_constants = (
+                np.array(force_constants)[:, na, :, na] * np.eye(3)[na, :, na, :]
+            ).flatten()
         elif len(np.shape(force_constants)) == 4:
             force_shape = np.shape(force_constants)
             if force_shape[2] == 3 and force_shape[3] == 3:
                 force_reshape = force_shape[0] * force_shape[2]
                 self._force_constants = np.transpose(
-                    force_constants,
-                    (0, 2, 1, 3)
+                    force_constants, (0, 2, 1, 3)
                 ).reshape((force_reshape, force_reshape))
             elif force_shape[1] == 3 and force_shape[3] == 3:
-                self._force_constants = np.array(force_constants).reshape(3*n_atom, 3*n_atom)
+                self._force_constants = np.array(force_constants).reshape(
+                    3 * n_atom, 3 * n_atom
+                )
             else:
-                raise AssertionError('force constant shape not recognized')
+                raise AssertionError("force constant shape not recognized")
         else:
-            raise AssertionError('force constant shape not recognized')
+            raise AssertionError("force constant shape not recognized")
 
     def set_reference_structure(self, structure):
         self._reference_structure = structure.copy()
         if self.structure is None:
             self.structure = structure.copy()
 
     def validate_ready_to_run(self):
         super(HessianJob, self).validate_ready_to_run()
         if self._force_constants is None:
-            raise AssertionError('set force constants by set_force_constants before run')
+            raise AssertionError(
+                "set force constants by set_force_constants before run"
+            )
         if self._reference_structure is None:
-            raise AssertionError('set reference structure by set_reference_structure before run')
+            raise AssertionError(
+                "set reference structure by set_reference_structure before run"
+            )
 
     def interactive_forces_getter(self):
         return self._forces
 
     def interactive_energy_pot_getter(self):
         return self._energy_pot
 
@@ -112,37 +123,39 @@
 
     def interactive_pressures_getter(self):
         return self._pressure
 
     def interactive_cells_setter(self, cell):
         if np.sum(self._stiffness_tensor) != 0:
             epsilon = np.einsum(
-                'ij,jk->ik',
+                "ij,jk->ik",
                 self.structure.cell,
-                np.linalg.inv(self._reference_structure.cell)
-            )-np.eye(3)
-            epsilon = (epsilon+epsilon.T)*0.5
+                np.linalg.inv(self._reference_structure.cell),
+            ) - np.eye(3)
+            epsilon = (epsilon + epsilon.T) * 0.5
             epsilon = np.append(
-                epsilon.diagonal(),
-                np.roll(epsilon, -1, axis=0).diagonal()
+                epsilon.diagonal(), np.roll(epsilon, -1, axis=0).diagonal()
+            )
+            pressure = -np.einsum("ij,j->i", self._stiffness_tensor, epsilon)
+            self._pressure = pressure[3:] * np.roll(np.eye(3), -1, axis=1)
+            self._pressure += self._pressure.T + np.eye(3) * pressure[:3]
+            self._pressure_times_volume = (
+                -np.sum(epsilon * pressure) * self.structure.get_volume()
             )
-            pressure = -np.einsum('ij,j->i', self._stiffness_tensor, epsilon)
-            self._pressure = pressure[3:]*np.roll(np.eye(3), -1, axis=1)
-            self._pressure += self._pressure.T+np.eye(3)*pressure[:3]
-            self._pressure_times_volume = -np.sum(epsilon*pressure)*self.structure.get_volume()
 
     def interactive_positions_setter(self, positions):
         displacements = self.structure.get_scaled_positions()
         displacements -= self._reference_structure.get_scaled_positions()
         displacements -= np.rint(displacements)
-        self._displacements = np.einsum('ji,ni->nj', self.structure.cell, displacements)
+        self._displacements = np.einsum("ji,ni->nj", self.structure.cell, displacements)
 
     def calculate_forces(self):
         position_transformed = self._displacements.reshape(
-            self._displacements.shape[0] * self._displacements.shape[1])
+            self._displacements.shape[0] * self._displacements.shape[1]
+        )
         forces_transformed = -np.dot(self._force_constants, position_transformed)
         self._forces = forces_transformed.reshape(self._displacements.shape)
         self._energy_pot = -1 / 2 * np.dot(position_transformed, forces_transformed)
         self._energy_pot += self._pressure_times_volume
 
     def interactive_collect(self):
         super(HessianJob, self).interactive_collect()
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/thermodynamics/interfacemethod.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/thermodynamics/interfacemethod.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 import operator
 import os
 import matplotlib.pylab as plt
 import random
 from sklearn.neighbors import KernelDensity
 
 __author__ = "Lifang Zhu, Jan Janssen"
-__copyright__ = "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH " \
-                "- Computational Materials Design (CM) Department"
+__copyright__ = (
+    "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH "
+    "- Computational Materials Design (CM) Department"
+)
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "development"
 __date__ = "Apr 24, 2020"
 
 
@@ -53,15 +55,15 @@
 
     Args:
         basis (pyiron_atomistics.structure.atoms.Atoms): Atomistic structure object
 
     Returns:
         Atoms: Atomistic structure object with selective dynamics set to True
     """
-    if 'selective_dynamics' in basis._tag_list.keys():
+    if "selective_dynamics" in basis._tag_list.keys():
         for ind in range(len(basis)):
             basis.selective_dynamics[ind] = [True, True, True]
     return basis
 
 
 def set_server(job, project_parameter):
     """
@@ -70,18 +72,18 @@
     Args:
         job (GenericJob): Job object
         project_parameter (dict): Dictionary with the keys potential and cpu_cores and optionally queue
 
     Returns:
         GenericJob: Updated job object
     """
-    job.potential = project_parameter['potential']
-    if 'queue' in project_parameter.keys():
-        job.server.queue = project_parameter['queue']
-    job.server.cores = project_parameter['cpu_cores']
+    job.potential = project_parameter["potential"]
+    if "queue" in project_parameter.keys():
+        job.server.queue = project_parameter["queue"]
+    job.server.cores = project_parameter["cpu_cores"]
     return job
 
 
 def create_job_template(job_name, structure, project_parameter):
     """
     Create a job template using the project_parameter dictionary. The dictionary has to contain the following keys:
     - job_type: Type of Simulation code to be used
@@ -93,46 +95,49 @@
         job_name (str): Name of the job object
         structure (pyiron_atomistics.structure.atoms.Atoms): Atomistic Structure object to be set to the job as input sturcture
         project_parameter (dict): Dictionary with the project parameters
 
     Returns:
         GenericJob: New job object
     """
-    pr = project_parameter['project']
-    job = pr.create_job(project_parameter['job_type'], job_name)
+    pr = project_parameter["project"]
+    job = pr.create_job(project_parameter["job_type"], job_name)
     job.structure = structure
     return set_server(job=job, project_parameter=project_parameter)
 
 
 def fix_iso(job):
     """
     Add couple xyz to the fix_ensemble inside LAMMPS
 
     Args:
         job (LAMMPS): Lammps job object
 
     Returns:
         LAMMPS: Return updated job object
     """
-    job.input.control['fix___ensemble'] = job.input.control['fix___ensemble'] + ' couple xyz'
+    job.input.control["fix___ensemble"] = (
+        job.input.control["fix___ensemble"] + " couple xyz"
+    )
     return job
 
 
 def fix_z_dir(job):
     """
     Rather than fixing all directions only fix the z-direction during an NPT simulation
 
     Args:
         job (LAMMPS): Lammps job object
 
     Returns:
         LAMMPS: Return updated job object
     """
-    job.input.control['fix___ensemble'] = \
-        job.input.control['fix___ensemble'].replace('x 0.0 0.0 1.0 y 0.0 0.0 1.0 z 0.0 0.0 1.0', 'z 0.0 0.0 1.0')
+    job.input.control["fix___ensemble"] = job.input.control["fix___ensemble"].replace(
+        "x 0.0 0.0 1.0 y 0.0 0.0 1.0 z 0.0 0.0 1.0", "z 0.0 0.0 1.0"
+    )
     return job
 
 
 def half_velocity(job, temperature):
     """
     Rather than setting twice the kinetic energy at the beginning of a molecular dynamics simulation reduce the
     velocity to half the initial velocity. This is required to continue MD claculation.
@@ -140,15 +145,17 @@
     Args:
         job (LAMMPS): Lammps job object
         temperature (float): Temperature of the molecular dynamics calculation in K
 
     Returns:
         LAMMPS: Return updated job object
     """
-    job.input.control['velocity'] = job.input.control['velocity'].replace(str(temperature * 2), str(temperature))
+    job.input.control["velocity"] = job.input.control["velocity"].replace(
+        str(temperature * 2), str(temperature)
+    )
     return job
 
 
 def minimize_pos(structure, project_parameter, max_iter=1000):
     """
     Minimize the positions in a given structure using the job type defined in the project_parameters, which
     contains the following keys:
@@ -162,29 +169,24 @@
         project_parameter (dict): Dictionary wtih the project parameters
         max_iter (int): Maximum number of steps during minimization
 
     Returns:
         job object used to execute the calculation
     """
     ham_minimize_pos = create_job_template(
-        job_name='minimize_pos',
+        job_name="minimize_pos",
         structure=structure,
-        project_parameter=project_parameter
+        project_parameter=project_parameter,
     )
     ham_minimize_pos.calc_minimize(
-        max_iter=max_iter,
-        e_tol=1.0e-9,
-        f_tol=1.0e-8,
-        n_print=max_iter
+        max_iter=max_iter, e_tol=1.0e-9, f_tol=1.0e-8, n_print=max_iter
     )
     ham_minimize_pos.run()
     ham_minimize_pos.project.wait_for_job(
-        ham_minimize_pos,
-        interval_in_s=100,
-        max_iterations=100000
+        ham_minimize_pos, interval_in_s=100, max_iterations=100000
     )
     return ham_minimize_pos
 
 
 def minimize_vol(structure, project_parameter, max_iter=1000):
     """
     Minimize the volume for a given structure using the job type defined in the project_parameters, which
@@ -199,31 +201,25 @@
         project_parameter (dict): Dictionary with the project parameters
         max_iter (int): Maximum number of steps during minimization
 
     Returns:
         job object used to execute the calculation
     """
     ham_minimize_vol = create_job_template(
-        job_name='minimize_vol',
+        job_name="minimize_vol",
         structure=structure,
-        project_parameter=project_parameter
+        project_parameter=project_parameter,
     )
     ham_minimize_vol.calc_minimize(
-        max_iter=max_iter,
-        e_tol=1.0e-9,
-        f_tol=1.0e-8,
-        pressure=0.0,
-        n_print=max_iter
+        max_iter=max_iter, e_tol=1.0e-9, f_tol=1.0e-8, pressure=0.0, n_print=max_iter
     )
-    ham_minimize_vol.input.control['fix___ensemble'] += ' vmax 0.001'
+    ham_minimize_vol.input.control["fix___ensemble"] += " vmax 0.001"
     ham_minimize_vol.run()
     ham_minimize_vol.project.wait_for_job(
-        ham_minimize_vol,
-        interval_in_s=100,
-        max_iterations=100000
+        ham_minimize_vol, interval_in_s=100, max_iterations=100000
     )
     return ham_minimize_vol
 
 
 def next_calc(structure, temperature, project_parameter, run_time_steps=10000):
     """
     Calculate NPT ensemble at a given temperature using the job defined in the project parameters:
@@ -238,38 +234,31 @@
         project_parameter (dict): Dictionary with the project parameters
         run_time_steps (int): Number of Molecular dynamics steps
 
     Returns:
         Final Atomistic Structure object
     """
     ham_temp = create_job_template(
-        job_name='temp_heating_' + str(temperature).replace('.', '_'),
+        job_name="temp_heating_" + str(temperature).replace(".", "_"),
         structure=structure,
-        project_parameter=project_parameter
+        project_parameter=project_parameter,
     )
     ham_temp.calc_md(
         temperature=temperature,
         temperature_damping_timescale=100.0,
         pressure=0.0,
         pressure_damping_timescale=1000.0,
         n_print=run_time_steps,
         n_ionic_steps=run_time_steps,
-        seed=project_parameter['seed'],
+        seed=project_parameter["seed"],
     )
     ham_temp = fix_iso(job=ham_temp)
-    ham_temp = half_velocity(
-        job=ham_temp,
-        temperature=temperature
-    )
+    ham_temp = half_velocity(job=ham_temp, temperature=temperature)
     ham_temp.run()
-    ham_temp.project.wait_for_job(
-        ham_temp,
-        interval_in_s=100,
-        max_iterations=100000
-    )
+    ham_temp.project.wait_for_job(ham_temp, interval_in_s=100, max_iterations=100000)
     return ham_temp.get_structure()
 
 
 def npt_solid(temperature, basis, project_parameter, timestep=1.0):
     """
     Calculate NPT ensemble at a given temperature using the job defined in the project parameters:
     - job_type: Type of Simulation code to be used
@@ -283,38 +272,33 @@
         project_parameter (dict): Dictionary with the project parameters
         timestep (float): Molecular dynamics time step
 
     Returns:
         job object used to execute the calculation
     """
     ham_npt_solid = create_job_template(
-        job_name='ham_npt_solid_' + str(temperature).replace('.', '_'),
+        job_name="ham_npt_solid_" + str(temperature).replace(".", "_"),
         structure=basis,
-        project_parameter=project_parameter
+        project_parameter=project_parameter,
     )
     ham_npt_solid.calc_md(
         temperature=temperature,
         temperature_damping_timescale=100.0,
         time_step=timestep,
         pressure=0.0,
         pressure_damping_timescale=1000.0,
-        n_print=project_parameter['run_time_steps'],
-        n_ionic_steps=project_parameter['run_time_steps'],
-        seed=project_parameter['seed'],
-    )
-    ham_npt_solid = half_velocity(
-        job=ham_npt_solid,
-        temperature=temperature
+        n_print=project_parameter["run_time_steps"],
+        n_ionic_steps=project_parameter["run_time_steps"],
+        seed=project_parameter["seed"],
     )
+    ham_npt_solid = half_velocity(job=ham_npt_solid, temperature=temperature)
     ham_npt_solid = fix_iso(job=ham_npt_solid)
     ham_npt_solid.run()
     ham_npt_solid.project.wait_for_job(
-        ham_npt_solid,
-        interval_in_s=100,
-        max_iterations=100000
+        ham_npt_solid, interval_in_s=100, max_iterations=100000
     )
     return ham_npt_solid
 
 
 def setup_liquid_job(job_name, basis, temperature, project_parameter, timestep=1.0):
     """
     Calculate NPT ensemble at a given temperature while freezing the position of the atoms
@@ -333,43 +317,40 @@
 
     Returns:
         job object used to execute the calculation
     """
     ham_npt_liquid_high = create_job_template(
         job_name=job_name,
         structure=freeze_one_half(basis),
-        project_parameter=project_parameter
+        project_parameter=project_parameter,
     )
     ham_npt_liquid_high.calc_md(
         temperature=temperature,
         temperature_damping_timescale=100.0,
         time_step=timestep,
         pressure=[0.0, 0.0, 0.0],
         pressure_damping_timescale=1000.0,
-        n_print=project_parameter['run_time_steps'],
-        n_ionic_steps=project_parameter['run_time_steps'],
-        seed=project_parameter['seed'],
+        n_print=project_parameter["run_time_steps"],
+        n_ionic_steps=project_parameter["run_time_steps"],
+        seed=project_parameter["seed"],
     )
     ham_npt_liquid_high = half_velocity(
-        job=ham_npt_liquid_high,
-        temperature=temperature
-    )
-    ham_npt_liquid_high = fix_z_dir(
-        job=ham_npt_liquid_high
+        job=ham_npt_liquid_high, temperature=temperature
     )
+    ham_npt_liquid_high = fix_z_dir(job=ham_npt_liquid_high)
     ham_npt_liquid_high.run()
     ham_npt_liquid_high.project.wait_for_job(
-        ham_npt_liquid_high,
-        interval_in_s=100,
-        max_iterations=100000
+        ham_npt_liquid_high, interval_in_s=100, max_iterations=100000
     )
     return ham_npt_liquid_high
 
 
-def npt_liquid(temperature_solid, temperature_liquid, basis, project_parameter, timestep=1.0):
+def npt_liquid(
+    temperature_solid, temperature_liquid, basis, project_parameter, timestep=1.0
+):
     """
     Calculate NPT ensemble at a given temperature while initally freezing the position of the atoms
     of the upper part (z>0.5) and afterwards calculating the full sample at a lower temperature.
     These steps are used to construct the solid liquid interface as part of the coexistence approach.
     For the calculations the job object is defined in the project parameters:
     - job_type: Type of Simulation code to be used
     - project: Project object used to create the job
@@ -383,26 +364,26 @@
         project_parameter (dict): Dictionary with the project parameters
         timestep (float): Molecular dynamics time step
 
     Returns:
         job object used to execute the calculation
     """
     ham_npt_liquid_high = setup_liquid_job(
-        job_name='ham_npt_liquid_high_' + str(temperature_liquid).replace('.', '_'),
+        job_name="ham_npt_liquid_high_" + str(temperature_liquid).replace(".", "_"),
         basis=basis,
         temperature=temperature_liquid,
         project_parameter=project_parameter,
-        timestep=timestep
+        timestep=timestep,
     )
     ham_npt_liquid_low = setup_liquid_job(
-        job_name='ham_npt_liquid_low_' + str(temperature_solid).replace('.', '_'),
+        job_name="ham_npt_liquid_low_" + str(temperature_solid).replace(".", "_"),
         basis=ham_npt_liquid_high.get_structure(iteration_step=-1),
         temperature=temperature_solid,
         project_parameter=project_parameter,
-        timestep=timestep
+        timestep=timestep,
     )
     return ham_npt_liquid_low
 
 
 def check_diamond(structure):
     """
     Utility function to check if the structure is fcc, bcc, hcp or diamond
@@ -410,22 +391,23 @@
     Args:
         structure (pyiron_atomistics.structure.atoms.Atoms): Atomistic Structure object to check
 
     Returns:
         bool: true if diamond else false
     """
     cna_dict = structure.analyse.pyscal_cna_adaptive(
-        mode="total",
-        ovito_compatibility=True
+        mode="total", ovito_compatibility=True
     )
     dia_dict = structure.analyse.pyscal_diamond_structure(
-        mode="total",
-        ovito_compatibility=True
+        mode="total", ovito_compatibility=True
+    )
+    return (
+        cna_dict["CommonNeighborAnalysis.counts.OTHER"]
+        > dia_dict["IdentifyDiamond.counts.OTHER"]
     )
-    return cna_dict['CommonNeighborAnalysis.counts.OTHER'] > dia_dict['IdentifyDiamond.counts.OTHER']
 
 
 def analyse_structure(structure, mode="total", diamond=False):
     """
     Use either common neighbor analysis or the diamond structure detector
 
     Args:
@@ -440,34 +422,34 @@
             the common neighbor analysis.
 
     Returns:
         (depends on `mode`)
     """
     if not diamond:
         return structure.analyse.pyscal_cna_adaptive(
-            mode=mode,
-            ovito_compatibility=True
+            mode=mode, ovito_compatibility=True
         )
     else:
         return structure.analyse.pyscal_diamond_structure(
-            mode=mode,
-            ovito_compatibility=True
+            mode=mode, ovito_compatibility=True
         )
 
 
-def next_step_funct(number_of_atoms,
-                    key_max,
-                    structure_left,
-                    structure_right,
-                    temperature_left,
-                    temperature_right,
-                    distribution_initial_half,
-                    structure_after_minimization,
-                    run_time_steps,
-                    project_parameter):
+def next_step_funct(
+    number_of_atoms,
+    key_max,
+    structure_left,
+    structure_right,
+    temperature_left,
+    temperature_right,
+    distribution_initial_half,
+    structure_after_minimization,
+    run_time_steps,
+    project_parameter,
+):
     """
 
     Args:
         number_of_atoms:
         key_max:
         structure_left:
         structure_right:
@@ -480,57 +462,64 @@
 
     Returns:
 
     """
     structure_left_dict = analyse_structure(
         structure=structure_left,
         mode="total",
-        diamond=project_parameter['crystalstructure'].lower() == 'diamond'
+        diamond=project_parameter["crystalstructure"].lower() == "diamond",
     )
     structure_right_dict = analyse_structure(
         structure=structure_right,
         mode="total",
-        diamond=project_parameter['crystalstructure'].lower() == 'diamond'
+        diamond=project_parameter["crystalstructure"].lower() == "diamond",
     )
     temperature_diff = temperature_right - temperature_left
-    if structure_left_dict[key_max] / number_of_atoms > distribution_initial_half and \
-            structure_right_dict[key_max] / number_of_atoms > distribution_initial_half:
+    if (
+        structure_left_dict[key_max] / number_of_atoms > distribution_initial_half
+        and structure_right_dict[key_max] / number_of_atoms > distribution_initial_half
+    ):
         structure_left = structure_right.copy()
         temperature_left = temperature_right
         temperature_right += temperature_diff
         structure_right = next_calc(
             structure=structure_after_minimization,
             temperature=temperature_right,
             project_parameter=project_parameter,
-            run_time_steps=run_time_steps
+            run_time_steps=run_time_steps,
         )
-    elif structure_left_dict[key_max] / number_of_atoms > distribution_initial_half > \
-            structure_right_dict[key_max] / number_of_atoms:
+    elif (
+        structure_left_dict[key_max] / number_of_atoms
+        > distribution_initial_half
+        > structure_right_dict[key_max] / number_of_atoms
+    ):
         temperature_diff /= 2
         temperature_left += temperature_diff
         structure_left = next_calc(
             structure=structure_after_minimization,
             temperature=temperature_left,
             project_parameter=project_parameter,
-            run_time_steps=run_time_steps
+            run_time_steps=run_time_steps,
         )
-    elif structure_left_dict[key_max] / number_of_atoms < distribution_initial_half and \
-            structure_right_dict[key_max] / number_of_atoms < distribution_initial_half:
+    elif (
+        structure_left_dict[key_max] / number_of_atoms < distribution_initial_half
+        and structure_right_dict[key_max] / number_of_atoms < distribution_initial_half
+    ):
         temperature_diff /= 2
         temperature_right = temperature_left
         temperature_left -= temperature_diff
         structure_right = structure_left.copy()
         structure_left = next_calc(
             structure=structure_after_minimization,
             temperature=temperature_left,
             project_parameter=project_parameter,
-            run_time_steps=run_time_steps
+            run_time_steps=run_time_steps,
         )
     else:
-        raise ValueError('We should never reach this point!')
+        raise ValueError("We should never reach this point!")
     return structure_left, structure_right, temperature_left, temperature_right
 
 
 def round_temperature_next(temperature_next):
     """
     Round temperature to the last two dicits
 
@@ -539,16 +528,25 @@
 
     Returns:
         float: rounded temperature
     """
     return np.round(temperature_next, 2)
 
 
-def strain_circle(basis_relative, temperature_next, nve_run_time_steps, project_parameter, timestep=1.0,
-                  strain_result_lst=None, pressure_result_lst=None, center=None, fit_range=0.02):
+def strain_circle(
+    basis_relative,
+    temperature_next,
+    nve_run_time_steps,
+    project_parameter,
+    timestep=1.0,
+    strain_result_lst=None,
+    pressure_result_lst=None,
+    center=None,
+    fit_range=0.02,
+):
     """
 
     Args:
         basis_relative:
         temperature_next:
         nve_run_time_steps:
         project_parameter:
@@ -557,172 +555,188 @@
         pressure_result_lst:
         center:
         fit_range:
 
     Returns:
 
     """
-    strain_lst, pressure_lst, temperature_lst, pressure_std_lst, temperature_std_lst = [], [], [], [], []
+    strain_lst, pressure_lst, temperature_lst, pressure_std_lst, temperature_std_lst = (
+        [],
+        [],
+        [],
+        [],
+        [],
+    )
     ovito_dict_lst, ham_nvt_lst, ham_nve_lst = [], [], []
     strain_value_lst = get_strain_lst(
         fit_range=fit_range,
-        points=project_parameter['points'],
+        points=project_parameter["points"],
         strain_result_lst=strain_result_lst,
         pressure_result_lst=pressure_result_lst,
-        center=center
+        center=center,
     )
     temperature_next = round_temperature_next(temperature_next)
     for strain in strain_value_lst:
         job_name = get_nve_job_name(
             temperature_next=temperature_next,
             strain=strain,
-            steps_lst=project_parameter['nve_run_time_steps_lst'],
-            nve_run_time_steps=nve_run_time_steps
+            steps_lst=project_parameter["nve_run_time_steps_lst"],
+            nve_run_time_steps=nve_run_time_steps,
         )
-        ham_nve = project_parameter['project'].load(job_name)
+        ham_nve = project_parameter["project"].load(job_name)
         if ham_nve is None:
             basis_strain = basis_relative.copy()
             cell = basis_strain.cell.copy()
             cell[2, 2] *= strain
             basis_strain.set_cell(cell=cell, scale_atoms=True)
-            ham_nvt = create_job_template(job_name=job_name.replace('nve', 'nvt'),
-                                          structure=basis_strain,
-                                          project_parameter=project_parameter)
+            ham_nvt = create_job_template(
+                job_name=job_name.replace("nve", "nvt"),
+                structure=basis_strain,
+                project_parameter=project_parameter,
+            )
             ham_nvt.calc_md(
                 temperature=temperature_next,
                 time_step=timestep,
                 temperature_damping_timescale=100.0,
-                n_print=project_parameter['nvt_run_time_steps'],
-                n_ionic_steps=project_parameter['nvt_run_time_steps'],
-                seed=project_parameter['seed'],
-            )
-            ham_nvt.input.control['fix___ensemble'] += ' drag 1'
-            ham_nvt = half_velocity(
-                job=ham_nvt,
-                temperature=temperature_next
+                n_print=project_parameter["nvt_run_time_steps"],
+                n_ionic_steps=project_parameter["nvt_run_time_steps"],
+                seed=project_parameter["seed"],
             )
+            ham_nvt.input.control["fix___ensemble"] += " drag 1"
+            ham_nvt = half_velocity(job=ham_nvt, temperature=temperature_next)
             ham_nvt.write_restart_file()
             ham_nvt.run()
             ham_nvt_lst.append(ham_nvt)
     for ham_nvt in ham_nvt_lst:
-        ham_nvt.project.wait_for_job(
-            ham_nvt,
-            interval_in_s=100,
-            max_iterations=100000
-        )
+        ham_nvt.project.wait_for_job(ham_nvt, interval_in_s=100, max_iterations=100000)
         ham_nve = ham_nvt.restart()
-        ham_nve.job_name = ham_nvt.job_name.replace('nvt', 'nve')
+        ham_nve.job_name = ham_nvt.job_name.replace("nvt", "nve")
         ham_nve.calc_md(
             n_ionic_steps=nve_run_time_steps,
             time_step=timestep,
             n_print=nve_run_time_steps / 100,
-            seed=project_parameter['seed'],
+            seed=project_parameter["seed"],
         )
-        ham_nve = set_server(
-            job=ham_nve,
-            project_parameter=project_parameter
+        ham_nve = set_server(job=ham_nve, project_parameter=project_parameter)
+        ham_nve.input.control["dump___1"] = ham_nve.input.control["dump___1"].replace(
+            "${dumptime}", str(nve_run_time_steps)
         )
-        ham_nve.input.control['dump___1'] = \
-            ham_nve.input.control['dump___1'].replace('${dumptime}', str(nve_run_time_steps))
         ham_nve.run()
         ham_nve_lst.append(ham_nve)
     for ham_nve in ham_nve_lst:
-        ham_nve.project.wait_for_job(
-            ham_nve,
-            interval_in_s=100,
-            max_iterations=100000
-        )
+        ham_nve.project.wait_for_job(ham_nve, interval_in_s=100, max_iterations=100000)
     for strain in strain_value_lst:
         job_name = get_nve_job_name(
             temperature_next=temperature_next,
             strain=strain,
-            steps_lst=project_parameter['nve_run_time_steps_lst'],
-            nve_run_time_steps=nve_run_time_steps
+            steps_lst=project_parameter["nve_run_time_steps_lst"],
+            nve_run_time_steps=nve_run_time_steps,
         )
-        ham_nve = project_parameter['project'].load(job_name)
+        ham_nve = project_parameter["project"].load(job_name)
         press, temperature, press_std, temperature_std, ovito_dict = [
             np.mean(get_press(ham=ham_nve, step=-20)),
-            np.mean(ham_nve['output/generic/temperature'][-20:]),
+            np.mean(ham_nve["output/generic/temperature"][-20:]),
             np.std(get_press(ham=ham_nve, step=-20)),
-            np.std(ham_nve['output/generic/temperature'][-20:]),
+            np.std(ham_nve["output/generic/temperature"][-20:]),
             analyse_structure(
                 structure=ham_nve.get_structure(iteration_step=-1),
                 mode="total",
-                diamond=project_parameter['crystalstructure'].lower() == 'diamond'
-            )
+                diamond=project_parameter["crystalstructure"].lower() == "diamond",
+            ),
         ]
         strain_lst.append(strain)
         pressure_lst.append(press)
         temperature_lst.append(temperature)
         pressure_std_lst.append(press_std)
         temperature_std_lst.append(temperature_std)
         ovito_dict_lst.append(ovito_dict)
-    return strain_lst, pressure_lst, temperature_lst, pressure_std_lst, temperature_std_lst, ovito_dict_lst
+    return (
+        strain_lst,
+        pressure_lst,
+        temperature_lst,
+        pressure_std_lst,
+        temperature_std_lst,
+        ovito_dict_lst,
+    )
 
 
 def analyse_minimized_structure(ham):
     """
 
     Args:
         ham (GenericJob):
 
     Returns:
 
     """
-    final_structure = ham.get_structure(
-        iteration_step=-1
-    )
+    final_structure = ham.get_structure(iteration_step=-1)
     diamond_flag = check_diamond(structure=final_structure)
     final_structure_dict = analyse_structure(
-        structure=final_structure,
-        mode="total",
-        diamond=diamond_flag
+        structure=final_structure, mode="total", diamond=diamond_flag
     )
     key_max = max(final_structure_dict.items(), key=operator.itemgetter(1))[0]
     number_of_atoms = len(final_structure)
     distribution_initial = final_structure_dict[key_max] / number_of_atoms
     distribution_initial_half = distribution_initial / 2
-    return final_structure, key_max, number_of_atoms, distribution_initial_half, final_structure_dict
+    return (
+        final_structure,
+        key_max,
+        number_of_atoms,
+        distribution_initial_half,
+        final_structure_dict,
+    )
 
 
 def get_press(ham, step=20):
     """
 
     Args:
         ham:
         step:
 
     Returns:
 
     """
-    return np.mean(ham['output/generic/pressures'][step:, :, :].diagonal(0, 2), axis=1)
+    return np.mean(ham["output/generic/pressures"][step:, :, :].diagonal(0, 2), axis=1)
 
 
 def get_center_point(strain_result_lst=None, pressure_result_lst=None, center=None):
     """
 
     Args:
         strain_result_lst:
         pressure_result_lst:
         center:
 
     Returns:
 
     """
-    if strain_result_lst is not None and len(strain_result_lst) != 0 and \
-            pressure_result_lst is not None and len(pressure_result_lst) != 0:
-        center_point = np.round(np.roots(np.polyfit(strain_result_lst, pressure_result_lst, 1))[0], 2)
+    if (
+        strain_result_lst is not None
+        and len(strain_result_lst) != 0
+        and pressure_result_lst is not None
+        and len(pressure_result_lst) != 0
+    ):
+        center_point = np.round(
+            np.roots(np.polyfit(strain_result_lst, pressure_result_lst, 1))[0], 2
+        )
     elif center is not None:
         center_point = center
     else:
         center_point = 1.0
     return center_point
 
 
-def get_strain_lst(fit_range=0.02, points=21, strain_result_lst=None, pressure_result_lst=None, center=None):
+def get_strain_lst(
+    fit_range=0.02,
+    points=21,
+    strain_result_lst=None,
+    pressure_result_lst=None,
+    center=None,
+):
     """
 
     Args:
         fit_range:
         points:
         strain_result_lst:
         pressure_result_lst:
@@ -730,17 +744,20 @@
 
     Returns:
 
     """
     center_point = get_center_point(
         strain_result_lst=strain_result_lst,
         pressure_result_lst=pressure_result_lst,
-        center=center
+        center=center,
     )
-    return [np.round(s, 3) for s in np.linspace(center_point-fit_range, center_point+fit_range, points)]
+    return [
+        np.round(s, 3)
+        for s in np.linspace(center_point - fit_range, center_point + fit_range, points)
+    ]
 
 
 def get_nve_job_name(temperature_next, strain, steps_lst, nve_run_time_steps):
     """
 
     Args:
         temperature_next:
@@ -748,77 +765,90 @@
         steps_lst:
         nve_run_time_steps:
 
     Returns:
 
     """
     temperature_next = round_temperature_next(temperature_next)
-    temp_str = str(temperature_next).replace('.', '_')
-    strain_str = str(strain).replace('.', '_')
+    temp_str = str(temperature_next).replace(".", "_")
+    strain_str = str(strain).replace(".", "_")
     steps_str = str(steps_lst.index(nve_run_time_steps))
-    return 'ham_nve_' + strain_str + '_' + temp_str + '_' + steps_str
+    return "ham_nve_" + strain_str + "_" + temp_str + "_" + steps_str
 
 
-def plot_solid_liquid_ratio(temperature_next, strain_lst, nve_run_time_steps, project_parameter, debug_plot=True):
+def plot_solid_liquid_ratio(
+    temperature_next, strain_lst, nve_run_time_steps, project_parameter, debug_plot=True
+):
     """
 
     Args:
         temperature_next:
         strain_lst:
         nve_run_time_steps:
         project_parameter:
         debug_plot:
 
     Returns:
 
     """
-    cna_str = project_parameter['crystalstructure'].upper()
+    cna_str = project_parameter["crystalstructure"].upper()
     ratio_lst = []
     for strain in strain_lst:
         job_name = get_nve_job_name(
             temperature_next=temperature_next,
             strain=strain,
-            steps_lst=project_parameter['nve_run_time_steps_lst'],
-            nve_run_time_steps=nve_run_time_steps
+            steps_lst=project_parameter["nve_run_time_steps_lst"],
+            nve_run_time_steps=nve_run_time_steps,
         )
-        ham_nve = project_parameter['project'].load(job_name)
+        ham_nve = project_parameter["project"].load(job_name)
         struct = ham_nve.get_structure().center_coordinates_in_unit_cell()
         cna = analyse_structure(
             structure=struct,
             mode="str",
-            diamond=project_parameter['crystalstructure'].lower() == 'diamond'
+            diamond=project_parameter["crystalstructure"].lower() == "diamond",
         )
-        if not project_parameter['crystalstructure'].lower() == 'diamond':
-            bcc_count = sum(cna == 'BCC')
-            fcc_count = sum(cna == 'FCC')
-            hcp_count = sum(cna == 'HCP')
-            cond = (cna_str == 'BCC' and bcc_count > fcc_count and bcc_count > hcp_count) or \
-                (cna_str == 'FCC' and fcc_count > bcc_count and fcc_count > hcp_count) or \
-                (cna_str == 'HCP' and hcp_count > bcc_count and hcp_count > fcc_count)
+        if not project_parameter["crystalstructure"].lower() == "diamond":
+            bcc_count = sum(cna == "BCC")
+            fcc_count = sum(cna == "FCC")
+            hcp_count = sum(cna == "HCP")
+            cond = (
+                (cna_str == "BCC" and bcc_count > fcc_count and bcc_count > hcp_count)
+                or (
+                    cna_str == "FCC" and fcc_count > bcc_count and fcc_count > hcp_count
+                )
+                or (
+                    cna_str == "HCP" and hcp_count > bcc_count and hcp_count > fcc_count
+                )
+            )
         else:
-            cna_str = 'Cubic diamond'
+            cna_str = "Cubic diamond"
             cond = sum(cna == cna_str) > 0.05 * len(struct)
         if cond:
             # plt.figure(figsize=(16,12))
-            bandwidth = (struct.get_volume()/len(struct))**(1.0/3.0)
-            kde = KernelDensity(kernel='gaussian',
-                                bandwidth=bandwidth).fit(struct.positions[:, 2][cna == cna_str].reshape(-1, 1))
-            z_range = np.linspace(struct.positions[:, 2].min(), struct.positions[:, 2].max(), 1000)
+            bandwidth = (struct.get_volume() / len(struct)) ** (1.0 / 3.0)
+            kde = KernelDensity(kernel="gaussian", bandwidth=bandwidth).fit(
+                struct.positions[:, 2][cna == cna_str].reshape(-1, 1)
+            )
+            z_range = np.linspace(
+                struct.positions[:, 2].min(), struct.positions[:, 2].max(), 1000
+            )
             sample = kde.score_samples(z_range.reshape(-1, 1))
-            gaussian_funct = np.exp(sample)/np.exp(sample).max()
+            gaussian_funct = np.exp(sample) / np.exp(sample).max()
             z_range_above_limit = z_range[np.where(gaussian_funct > 0.1)]
             z_range_below_limit = z_range[np.where(gaussian_funct < 0.1)]
             if len(z_range_above_limit) != 0:
-                ratio_above = (np.max(z_range_above_limit)-np.min(z_range_above_limit)) / \
-                              (np.max(z_range)-np.min(z_range))
+                ratio_above = (
+                    np.max(z_range_above_limit) - np.min(z_range_above_limit)
+                ) / (np.max(z_range) - np.min(z_range))
             else:
                 ratio_above = 1.0
             if len(z_range_below_limit) != 0:
-                ratio_below = 1 - (np.max(z_range_below_limit)-np.min(z_range_below_limit)) / \
-                              (np.max(z_range)-np.min(z_range))
+                ratio_below = 1 - (
+                    np.max(z_range_below_limit) - np.min(z_range_below_limit)
+                ) / (np.max(z_range) - np.min(z_range))
             else:
                 ratio_below = 0.0
             if ratio_below == 0.0:
                 ratio = ratio_above
             elif ratio_above == 1.0:
                 ratio = ratio_below
             else:
@@ -827,79 +857,106 @@
         else:
             z_range = None
             gaussian_funct = None
             z_range_above_limit = None
             ratio = None
             ratio_lst.append(0.0)
         if debug_plot:
-            plt.title('strain: ' + str(strain))
-            plt.xlabel('position z')
-            plt.ylabel('position x')
-            plt.plot(struct.positions[:, 2], struct.positions[:, 0], 'o', label='all')
-            if not project_parameter['crystalstructure'].lower() == 'diamond':
-                plt.plot(struct.positions[:, 2][cna == 'BCC'], struct.positions[:, 0][cna == 'BCC'], 'x', label='BCC')
-                plt.plot(struct.positions[:, 2][cna == 'FCC'], struct.positions[:, 0][cna == 'FCC'], 'x', label='FCC')
-                plt.plot(struct.positions[:, 2][cna == 'HCP'], struct.positions[:, 0][cna == 'HCP'], 'x', label='HCP')
+            plt.title("strain: " + str(strain))
+            plt.xlabel("position z")
+            plt.ylabel("position x")
+            plt.plot(struct.positions[:, 2], struct.positions[:, 0], "o", label="all")
+            if not project_parameter["crystalstructure"].lower() == "diamond":
+                plt.plot(
+                    struct.positions[:, 2][cna == "BCC"],
+                    struct.positions[:, 0][cna == "BCC"],
+                    "x",
+                    label="BCC",
+                )
+                plt.plot(
+                    struct.positions[:, 2][cna == "FCC"],
+                    struct.positions[:, 0][cna == "FCC"],
+                    "x",
+                    label="FCC",
+                )
+                plt.plot(
+                    struct.positions[:, 2][cna == "HCP"],
+                    struct.positions[:, 0][cna == "HCP"],
+                    "x",
+                    label="HCP",
+                )
             else:
                 plt.plot(
-                    struct.positions[:, 2][cna == 'Cubic diamond'],
-                    struct.positions[:, 0][cna == 'Cubic diamond'],
-                    'x',
-                    label='Cubic diamond'
+                    struct.positions[:, 2][cna == "Cubic diamond"],
+                    struct.positions[:, 0][cna == "Cubic diamond"],
+                    "x",
+                    label="Cubic diamond",
                 )
                 plt.plot(
-                    struct.positions[:, 2][cna == 'Cubic diamond (1st neighbor)'],
-                    struct.positions[:, 0][cna == 'Cubic diamond (1st neighbor)'],
-                    'x',
-                    label='Cubic diamond (1st neighbor)'
+                    struct.positions[:, 2][cna == "Cubic diamond (1st neighbor)"],
+                    struct.positions[:, 0][cna == "Cubic diamond (1st neighbor)"],
+                    "x",
+                    label="Cubic diamond (1st neighbor)",
                 )
                 plt.plot(
-                    struct.positions[:, 2][cna == 'Cubic diamond (2nd neighbor)'],
-                    struct.positions[:, 0][cna == 'Cubic diamond (2nd neighbor)'],
-                    'x',
-                    label='Cubic diamond (2nd neighbor)'
+                    struct.positions[:, 2][cna == "Cubic diamond (2nd neighbor)"],
+                    struct.positions[:, 0][cna == "Cubic diamond (2nd neighbor)"],
+                    "x",
+                    label="Cubic diamond (2nd neighbor)",
                 )
                 plt.plot(
-                    struct.positions[:, 2][cna == 'Hexagonal diamond'],
-                    struct.positions[:, 0][cna == 'Hexagonal diamond'],
-                    'x',
-                    label='Hexagonal diamond'
+                    struct.positions[:, 2][cna == "Hexagonal diamond"],
+                    struct.positions[:, 0][cna == "Hexagonal diamond"],
+                    "x",
+                    label="Hexagonal diamond",
                 )
                 plt.plot(
-                    struct.positions[:, 2][cna == 'Hexagonal diamond (1st neighbor)'],
-                    struct.positions[:, 0][cna == 'Hexagonal diamond (1st neighbor)'],
-                    'x',
-                    label='Hexagonal diamond (1st neighbor)'
+                    struct.positions[:, 2][cna == "Hexagonal diamond (1st neighbor)"],
+                    struct.positions[:, 0][cna == "Hexagonal diamond (1st neighbor)"],
+                    "x",
+                    label="Hexagonal diamond (1st neighbor)",
                 )
                 plt.plot(
-                    struct.positions[:, 2][cna == 'Hexagonal diamond (2nd neighbor)'],
-                    struct.positions[:, 0][cna == 'Hexagonal diamond (2nd neighbor)'],
-                    'x',
-                    label='Hexagonal diamond (2nd neighbor)'
+                    struct.positions[:, 2][cna == "Hexagonal diamond (2nd neighbor)"],
+                    struct.positions[:, 0][cna == "Hexagonal diamond (2nd neighbor)"],
+                    "x",
+                    label="Hexagonal diamond (2nd neighbor)",
                 )
             cna_str_lst = struct.positions[:, 2][cna == cna_str]
             if len(cna_str_lst) != 0:
-                plt.axvline(cna_str_lst.max(), color='red')
-                plt.axvline(cna_str_lst.min(), color='red')
+                plt.axvline(cna_str_lst.max(), color="red")
+                plt.axvline(cna_str_lst.min(), color="red")
             plt.legend()
             plt.show()
-            plt.xlabel('Position in z')
-            plt.ylabel('kernel density score')
-            plt.title('strain: ' + str(strain))
+            plt.xlabel("Position in z")
+            plt.ylabel("kernel density score")
+            plt.title("strain: " + str(strain))
             if z_range is not None:
                 plt.plot(z_range, gaussian_funct, label=cna_str)
-                plt.axvline(np.min(z_range_above_limit), color='black', linestyle='--', label='ratio: ' + str(ratio))
-                plt.axvline(np.max(z_range_above_limit), color='black', linestyle='--')
-            plt.axhline(0.1, color='red')
+                plt.axvline(
+                    np.min(z_range_above_limit),
+                    color="black",
+                    linestyle="--",
+                    label="ratio: " + str(ratio),
+                )
+                plt.axvline(np.max(z_range_above_limit), color="black", linestyle="--")
+            plt.axhline(0.1, color="red")
             plt.legend()
             plt.show()
     return ratio_lst
 
 
-def ratio_selection(strain_lst, ratio_lst, pressure_lst, temperature_lst, ratio_boundary, debug_plot=True):
+def ratio_selection(
+    strain_lst,
+    ratio_lst,
+    pressure_lst,
+    temperature_lst,
+    ratio_boundary,
+    debug_plot=True,
+):
     """
 
     Args:
         strain_lst:
         ratio_lst:
         pressure_lst:
         temperature_lst:
@@ -907,19 +964,19 @@
         debug_plot:
 
     Returns:
 
     """
     if debug_plot:
         plt.plot(strain_lst, ratio_lst)
-        plt.axhline(0.5 + ratio_boundary, color='red', linestyle='--')
-        plt.axhline(0.5, color='black', linestyle='--')
-        plt.axhline(0.5 - ratio_boundary, color='red', linestyle='--')
-        plt.xlabel('Strain')
-        plt.ylabel('ratio solid vs. liquid')
+        plt.axhline(0.5 + ratio_boundary, color="red", linestyle="--")
+        plt.axhline(0.5, color="black", linestyle="--")
+        plt.axhline(0.5 - ratio_boundary, color="red", linestyle="--")
+        plt.xlabel("Strain")
+        plt.ylabel("ratio solid vs. liquid")
     rat_lst, rat_col_lst = [], []
     for rat in ratio_lst:
         if (0.5 - ratio_boundary) < rat < (0.5 + ratio_boundary):
             rat_lst.append(rat)
         elif len(rat_lst) != 0:
             rat_col_lst.append(rat_lst)
             rat_lst = []
@@ -929,29 +986,43 @@
         rat_max_ind = np.argmax([len(lst) for lst in rat_col_lst])
         ratio_ind = [r in rat_col_lst[rat_max_ind] for r in ratio_lst]
         strain_value_lst = np.array(strain_lst)[ratio_ind]
         ratio_value_lst = np.array(ratio_lst)[ratio_ind]
         pressure_value_lst = np.array(pressure_lst)[ratio_ind]
         temperature_value_lst = np.array(temperature_lst)[ratio_ind]
         if debug_plot:
-            plt.axvline(np.min(strain_value_lst), color='blue', linestyle='--')
-            plt.axvline(np.max(strain_value_lst), color='blue', linestyle='--')
+            plt.axvline(np.min(strain_value_lst), color="blue", linestyle="--")
+            plt.axvline(np.max(strain_value_lst), color="blue", linestyle="--")
             plt.show()
         if np.mean(ratio_value_lst) > 0.5:
-            return strain_value_lst, ratio_value_lst, pressure_value_lst, temperature_value_lst, 1
+            return (
+                strain_value_lst,
+                ratio_value_lst,
+                pressure_value_lst,
+                temperature_value_lst,
+                1,
+            )
         else:
-            return strain_value_lst, ratio_value_lst, pressure_value_lst, temperature_value_lst, -1
+            return (
+                strain_value_lst,
+                ratio_value_lst,
+                pressure_value_lst,
+                temperature_value_lst,
+                -1,
+            )
     else:
         if np.mean(ratio_lst) > 0.5:
             return [], [], [], [], 1
         else:
             return [], [], [], [], -1
 
 
-def plot_equilibration(temperature_next, strain_lst, nve_run_time_steps, project_parameter, debug_plot=True):
+def plot_equilibration(
+    temperature_next, strain_lst, nve_run_time_steps, project_parameter, debug_plot=True
+):
     """
 
     Args:
         temperature_next:
         strain_lst:
         nve_run_time_steps:
         project_parameter:
@@ -961,79 +1032,125 @@
 
     """
     if debug_plot:
         for strain in strain_lst:
             job_name = get_nve_job_name(
                 temperature_next=temperature_next,
                 strain=strain,
-                steps_lst=project_parameter['nve_run_time_steps_lst'],
-                nve_run_time_steps=nve_run_time_steps
+                steps_lst=project_parameter["nve_run_time_steps_lst"],
+                nve_run_time_steps=nve_run_time_steps,
+            )
+            ham_nve = project_parameter["project"].load(job_name)
+            plt.plot(
+                ham_nve["output/generic/temperature"], label="strain: " + str(strain)
+            )
+            plt.axhline(
+                np.mean(ham_nve["output/generic/temperature"][-20:]),
+                linestyle="--",
+                color="red",
+            )
+            plt.axvline(
+                range(len(ham_nve["output/generic/temperature"]))[-20],
+                linestyle="--",
+                color="black",
             )
-            ham_nve = project_parameter['project'].load(job_name)
-            plt.plot(ham_nve['output/generic/temperature'], label='strain: ' + str(strain))
-            plt.axhline(np.mean(ham_nve['output/generic/temperature'][-20:]), linestyle='--', color='red')
-            plt.axvline(range(len(ham_nve['output/generic/temperature']))[-20], linestyle='--', color='black')
             plt.legend()
-            plt.xlabel('timestep')
-            plt.ylabel('Temperature K')
+            plt.xlabel("timestep")
+            plt.ylabel("Temperature K")
             plt.legend()
             plt.show()
 
 
-def plot_melting_point_prediction(strain_value_lst, pressure_value_lst, temperature_value_lst, boundary_value=0.25,
-                                  debug_plot=True):
+def plot_melting_point_prediction(
+    strain_value_lst,
+    pressure_value_lst,
+    temperature_value_lst,
+    boundary_value=0.25,
+    debug_plot=True,
+):
     """
 
     Args:
         strain_value_lst:
         pressure_value_lst:
         temperature_value_lst:
         boundary_value:
         debug_plot:
 
     Returns:
 
     """
     fit_press = np.poly1d(np.polyfit(strain_value_lst, pressure_value_lst, 1))
     fit_temp = np.poly1d(np.polyfit(strain_value_lst, temperature_value_lst, 1))
-    fit_temp_from_press = np.poly1d(np.polyfit(pressure_value_lst, temperature_value_lst, 1))
-    fit_combined = np.poly1d(np.polyfit(fit_press(strain_value_lst), fit_temp(strain_value_lst), 1))
+    fit_temp_from_press = np.poly1d(
+        np.polyfit(pressure_value_lst, temperature_value_lst, 1)
+    )
+    fit_combined = np.poly1d(
+        np.polyfit(fit_press(strain_value_lst), fit_temp(strain_value_lst), 1)
+    )
     if debug_plot:
-        plt.plot(strain_value_lst, pressure_value_lst, 'o', label='pressure (strain)')
-        plt.plot(strain_value_lst, fit_press(strain_value_lst), label='fit')
-        plt.xlabel('Strain')
-        plt.ylabel('Pressure GPa')
+        plt.plot(strain_value_lst, pressure_value_lst, "o", label="pressure (strain)")
+        plt.plot(strain_value_lst, fit_press(strain_value_lst), label="fit")
+        plt.xlabel("Strain")
+        plt.ylabel("Pressure GPa")
         plt.legend()
         plt.show()
-        plt.plot(strain_value_lst, temperature_value_lst, 'o', label='temperature (strain)')
-        plt.plot(strain_value_lst, fit_temp(strain_value_lst), label='fit')
-        plt.xlabel('Strain')
-        plt.ylabel('Temperature K')
+        plt.plot(
+            strain_value_lst, temperature_value_lst, "o", label="temperature (strain)"
+        )
+        plt.plot(strain_value_lst, fit_temp(strain_value_lst), label="fit")
+        plt.xlabel("Strain")
+        plt.ylabel("Temperature K")
         plt.legend()
         plt.show()
-        plt.plot(pressure_value_lst, temperature_value_lst, 'o', label='temperature (pressure)')
-        plt.plot(pressure_value_lst, fit_temp_from_press(pressure_value_lst), label='fit direct')
-        plt.plot(fit_press(strain_value_lst), fit_temp(strain_value_lst), label='combined fits')
-        plt.xlabel('Pressure GPa')
-        plt.ylabel('Temperature K')
+        plt.plot(
+            pressure_value_lst,
+            temperature_value_lst,
+            "o",
+            label="temperature (pressure)",
+        )
+        plt.plot(
+            pressure_value_lst,
+            fit_temp_from_press(pressure_value_lst),
+            label="fit direct",
+        )
+        plt.plot(
+            fit_press(strain_value_lst),
+            fit_temp(strain_value_lst),
+            label="combined fits",
+        )
+        plt.xlabel("Pressure GPa")
+        plt.ylabel("Temperature K")
         plt.legend()
         plt.show()
     print(fit_temp_from_press(0.0), fit_combined(0.0))
-    temperature_mean = np.min(temperature_value_lst) + \
-        (np.max(temperature_value_lst) - np.min(temperature_value_lst)) * 1 / 2
-    temperature_left = np.min(temperature_value_lst) + \
-        (np.max(temperature_value_lst) - np.min(temperature_value_lst)) * (1 / 2 - boundary_value)
-    temperature_right = np.min(temperature_value_lst) + \
-        (np.max(temperature_value_lst) - np.min(temperature_value_lst)) * (1 / 2 + boundary_value)
+    temperature_mean = (
+        np.min(temperature_value_lst)
+        + (np.max(temperature_value_lst) - np.min(temperature_value_lst)) * 1 / 2
+    )
+    temperature_left = np.min(temperature_value_lst) + (
+        np.max(temperature_value_lst) - np.min(temperature_value_lst)
+    ) * (1 / 2 - boundary_value)
+    temperature_right = np.min(temperature_value_lst) + (
+        np.max(temperature_value_lst) - np.min(temperature_value_lst)
+    ) * (1 / 2 + boundary_value)
     temperature_next = fit_temp_from_press(0.0)
     return temperature_next, temperature_mean, temperature_left, temperature_right
 
 
-def calc_temp_iteration(basis, temperature_next, project_parameter, timestep, nve_run_time_steps, fit_range, center,
-                        debug_plot=True):
+def calc_temp_iteration(
+    basis,
+    temperature_next,
+    project_parameter,
+    timestep,
+    nve_run_time_steps,
+    fit_range,
+    center,
+    debug_plot=True,
+):
     """
 
     Args:
         basis:
         temperature_next:
         project_parameter:
         timestep:
@@ -1046,135 +1163,192 @@
 
     """
     temperature_next = round_temperature_next(temperature_next)
     ham_npt_solid = npt_solid(
         temperature=temperature_next,
         basis=basis,
         project_parameter=project_parameter,
-        timestep=timestep
+        timestep=timestep,
     )
     ham_npt_liquid_low = npt_liquid(
         temperature_solid=temperature_next,
         temperature_liquid=temperature_next + 1000,
         basis=ham_npt_solid.get_structure(),
         project_parameter=project_parameter,
-        timestep=timestep
+        timestep=timestep,
     )
     basis = ham_npt_liquid_low.get_structure()
     basis_no_selective = remove_selective_dynamics(basis)
     basis_relative = basis_no_selective.copy()
     strain_lst, pressure_lst, temperature_lst, _, _, _ = strain_circle(
         basis_relative=basis_relative,
         temperature_next=temperature_next,
         nve_run_time_steps=nve_run_time_steps,
         project_parameter=project_parameter,
         timestep=timestep,
         strain_result_lst=None,
         pressure_result_lst=None,
         center=center,
-        fit_range=fit_range
+        fit_range=fit_range,
     )
     ratio_lst = plot_solid_liquid_ratio(
         temperature_next=temperature_next,
         strain_lst=strain_lst,
         nve_run_time_steps=nve_run_time_steps,
         project_parameter=project_parameter,
-        debug_plot=debug_plot
+        debug_plot=debug_plot,
     )
-    strain_value_lst, _, pressure_value_lst, temperature_value_lst, sl_flag = ratio_selection(
+    (
+        strain_value_lst,
+        _,
+        pressure_value_lst,
+        temperature_value_lst,
+        sl_flag,
+    ) = ratio_selection(
         strain_lst=strain_lst,
         ratio_lst=ratio_lst,
         pressure_lst=pressure_lst,
         temperature_lst=temperature_lst,
-        ratio_boundary=project_parameter['ratio_boundary'],
-        debug_plot=debug_plot
+        ratio_boundary=project_parameter["ratio_boundary"],
+        debug_plot=debug_plot,
     )
     if len(strain_value_lst) > 2:
         plot_equilibration(
             temperature_next=temperature_next,
             strain_lst=strain_lst,
             nve_run_time_steps=nve_run_time_steps,
             project_parameter=project_parameter,
-            debug_plot=debug_plot
+            debug_plot=debug_plot,
         )
         ind = check_for_holes(
             temperature_next=temperature_next,
             strain_value_lst=strain_value_lst,
             nve_run_time_steps=nve_run_time_steps,
-            project_parameter=project_parameter
+            project_parameter=project_parameter,
         )
         strain_value_lst = np.array(strain_value_lst)[ind].tolist()
         pressure_value_lst = np.array(pressure_value_lst)[ind].tolist()
         temperature_value_lst = np.array(temperature_value_lst)[ind].tolist()
-        temperature_next, temperature_mean, temperature_left, temperature_right = plot_melting_point_prediction(
+        (
+            temperature_next,
+            temperature_mean,
+            temperature_left,
+            temperature_right,
+        ) = plot_melting_point_prediction(
             strain_value_lst=strain_value_lst,
             pressure_value_lst=pressure_value_lst,
             temperature_value_lst=temperature_value_lst,
-            boundary_value=project_parameter['boundary_value'],
-            debug_plot=True
+            boundary_value=project_parameter["boundary_value"],
+            debug_plot=True,
         )
     else:
         if sl_flag < 0:
-            temperature_next, temperature_mean, temperature_left, temperature_right = \
-                temperature_next * 0.90, 0.0, 0.0, 0.0
+            temperature_next, temperature_mean, temperature_left, temperature_right = (
+                temperature_next * 0.90,
+                0.0,
+                0.0,
+                0.0,
+            )
         else:
-            temperature_next, temperature_mean, temperature_left, temperature_right = \
-                temperature_next * 1.10, 0.0, 0.0, 0.0
-    return temperature_next, temperature_mean, temperature_left, temperature_right, strain_value_lst, pressure_value_lst
+            temperature_next, temperature_mean, temperature_left, temperature_right = (
+                temperature_next * 1.10,
+                0.0,
+                0.0,
+                0.0,
+            )
+    return (
+        temperature_next,
+        temperature_mean,
+        temperature_left,
+        temperature_right,
+        strain_value_lst,
+        pressure_value_lst,
+    )
 
 
-def get_initial_melting_temperature_guess(project_parameter, ham_minimize_vol, temperature_next=None):
+def get_initial_melting_temperature_guess(
+    project_parameter, ham_minimize_vol, temperature_next=None
+):
     """
 
     Args:
         project_parameter:
         ham_minimize_vol:
         temperature_next:
 
     Returns:
 
     """
-    structure_after_minimization, key_max, number_of_atoms, distribution_initial_half, _ = analyse_minimized_structure(
-        ham_minimize_vol
-    )
-    temperature_left = project_parameter['temperature_left']
-    temperature_right = project_parameter['temperature_right']
+    (
+        structure_after_minimization,
+        key_max,
+        number_of_atoms,
+        distribution_initial_half,
+        _,
+    ) = analyse_minimized_structure(ham_minimize_vol)
+    temperature_left = project_parameter["temperature_left"]
+    temperature_right = project_parameter["temperature_right"]
     if temperature_next is None:
         structure_left = structure_after_minimization
         structure_right = next_calc(
             structure=structure_after_minimization,
             temperature=temperature_right,
             project_parameter=project_parameter,
-            run_time_steps=project_parameter['strain_run_time_steps']
+            run_time_steps=project_parameter["strain_run_time_steps"],
         )
         temperature_step = temperature_right - temperature_left
         while temperature_step > 10:
-            structure_left, structure_right, temperature_left, temperature_right = next_step_funct(
+            (
+                structure_left,
+                structure_right,
+                temperature_left,
+                temperature_right,
+            ) = next_step_funct(
                 number_of_atoms=number_of_atoms,
                 key_max=key_max,
                 structure_left=structure_left,
                 structure_right=structure_right,
                 temperature_left=temperature_left,
                 temperature_right=temperature_right,
                 distribution_initial_half=distribution_initial_half,
                 structure_after_minimization=structure_after_minimization,
-                run_time_steps=project_parameter['strain_run_time_steps'],
-                project_parameter=project_parameter)
+                run_time_steps=project_parameter["strain_run_time_steps"],
+                project_parameter=project_parameter,
+            )
             temperature_step = temperature_right - temperature_left
         temperature_next = int(round(temperature_left))
         return temperature_next, structure_left
     else:
         return temperature_next, ham_minimize_vol.get_structure()
 
 
-def validate_convergence(pr, temperature_left, temperature_next, temperature_right, enable_iteration,
-                         timestep_iter, timestep_lst, timestep, fit_range_iter, fit_range_lst, fit_range,
-                         nve_run_time_steps_iter, nve_run_time_steps_lst, nve_run_time_steps,
-                         strain_result_lst, pressure_result_lst, step_count, step_dict, boundary_value, ratio_boundary,
-                         convergence_goal, output_file='melting.json'):
+def validate_convergence(
+    pr,
+    temperature_left,
+    temperature_next,
+    temperature_right,
+    enable_iteration,
+    timestep_iter,
+    timestep_lst,
+    timestep,
+    fit_range_iter,
+    fit_range_lst,
+    fit_range,
+    nve_run_time_steps_iter,
+    nve_run_time_steps_lst,
+    nve_run_time_steps,
+    strain_result_lst,
+    pressure_result_lst,
+    step_count,
+    step_dict,
+    boundary_value,
+    ratio_boundary,
+    convergence_goal,
+    output_file="melting.json",
+):
     """
 
     Args:
         pr:
         temperature_left:
         temperature_next:
         temperature_right:
@@ -1200,61 +1374,90 @@
     Returns:
 
     """
     if temperature_left < temperature_next < temperature_right and enable_iteration:
         timestep = next(timestep_iter)
         fit_range = next(fit_range_iter)
         nve_run_time_steps = next(nve_run_time_steps_iter)
-    if timestep == timestep_lst[-1] and fit_range == fit_range_lst[-1] and nve_run_time_steps == nve_run_time_steps_lst[-1]:
+    if (
+        timestep == timestep_lst[-1]
+        and fit_range == fit_range_lst[-1]
+        and nve_run_time_steps == nve_run_time_steps_lst[-1]
+    ):
         enable_iteration = False
-    center = np.abs(get_center_point(
-        strain_result_lst=strain_result_lst,
-        pressure_result_lst=pressure_result_lst
-    ))
+    center = np.abs(
+        get_center_point(
+            strain_result_lst=strain_result_lst, pressure_result_lst=pressure_result_lst
+        )
+    )
     step_count += 1
     if step_count not in step_dict.keys():
-        step_dict[step_count] = {'timestep': timestep,
-                                 'fit_range': fit_range,
-                                 'nve_run_time_steps': nve_run_time_steps,
-                                 'boundary_value': boundary_value,
-                                 'ratio_boundary': ratio_boundary,
-                                 'temperature_next': temperature_next,
-                                 'center': center}
-        with open(output_file, 'w') as f:
+        step_dict[step_count] = {
+            "timestep": timestep,
+            "fit_range": fit_range,
+            "nve_run_time_steps": nve_run_time_steps,
+            "boundary_value": boundary_value,
+            "ratio_boundary": ratio_boundary,
+            "temperature_next": temperature_next,
+            "center": center,
+        }
+        with open(output_file, "w") as f:
             json.dump(step_dict, f)
     else:
-        timestep = step_dict[step_count]['timestep']
-        fit_range = step_dict[step_count]['fit_range']
-        nve_run_time_steps = step_dict[step_count]['nve_run_time_steps']
-        boundary_value = step_dict[step_count]['boundary_value']
-        ratio_boundary = step_dict[step_count]['ratio_boundary']
-        temperature_next = step_dict[step_count]['temperature_next']
-        center = step_dict[step_count]['center']
-    if np.abs(step_dict[step_count]['temperature_next'] - step_dict[step_count - 1][
-            'temperature_next']) <= convergence_goal:
+        timestep = step_dict[step_count]["timestep"]
+        fit_range = step_dict[step_count]["fit_range"]
+        nve_run_time_steps = step_dict[step_count]["nve_run_time_steps"]
+        boundary_value = step_dict[step_count]["boundary_value"]
+        ratio_boundary = step_dict[step_count]["ratio_boundary"]
+        temperature_next = step_dict[step_count]["temperature_next"]
+        center = step_dict[step_count]["center"]
+    if (
+        np.abs(
+            step_dict[step_count]["temperature_next"]
+            - step_dict[step_count - 1]["temperature_next"]
+        )
+        <= convergence_goal
+    ):
         convergence_goal_achieved = True
     else:
         convergence_goal_achieved = False
-    return convergence_goal_achieved, enable_iteration, step_count, step_dict, timestep, \
-        fit_range, nve_run_time_steps, boundary_value, ratio_boundary, temperature_next, center
+    return (
+        convergence_goal_achieved,
+        enable_iteration,
+        step_count,
+        step_dict,
+        timestep,
+        fit_range,
+        nve_run_time_steps,
+        boundary_value,
+        ratio_boundary,
+        temperature_next,
+        center,
+    )
 
 
 def initialise_iterators(project_parameter):
     """
 
     Args:
         project_parameter:
 
     Returns:
 
     """
-    return iter(project_parameter['timestep_lst']), iter(project_parameter['fit_range_lst']), iter(project_parameter['nve_run_time_steps_lst'])
+    return (
+        iter(project_parameter["timestep_lst"]),
+        iter(project_parameter["fit_range_lst"]),
+        iter(project_parameter["nve_run_time_steps_lst"]),
+    )
 
 
-def get_voronoi_volume(temperature_next, strain_lst, nve_run_time_steps, project_parameter):
+def get_voronoi_volume(
+    temperature_next, strain_lst, nve_run_time_steps, project_parameter
+):
     """
 
     Args:
         temperature_next:
         strain_lst:
         nve_run_time_steps:
         project_parameter:
@@ -1263,25 +1466,31 @@
 
     """
     max_lst, mean_lst = [], []
     for strain in strain_lst:
         job_name = get_nve_job_name(
             temperature_next=temperature_next,
             strain=strain,
-            steps_lst=project_parameter['nve_run_time_steps_lst'],
-            nve_run_time_steps=nve_run_time_steps
+            steps_lst=project_parameter["nve_run_time_steps_lst"],
+            nve_run_time_steps=nve_run_time_steps,
         )
-        ham_nve = project_parameter['project'].load(job_name)
+        ham_nve = project_parameter["project"].load(job_name)
         structure_voronoi_lst = ham_nve.get_structure().analyse.pyscal_voronoi_volume()
         max_lst.append(np.max(structure_voronoi_lst))
         mean_lst.append(np.mean(structure_voronoi_lst))
     return max_lst, mean_lst
 
 
-def check_for_holes(temperature_next, strain_value_lst, nve_run_time_steps, project_parameter, debug_plot=True):
+def check_for_holes(
+    temperature_next,
+    strain_value_lst,
+    nve_run_time_steps,
+    project_parameter,
+    debug_plot=True,
+):
     """
 
     Args:
         temperature_next:
         strain_value_lst:
         nve_run_time_steps:
         project_parameter:
@@ -1290,62 +1499,66 @@
     Returns:
 
     """
     max_lst, mean_lst = get_voronoi_volume(
         temperature_next=temperature_next,
         strain_lst=strain_value_lst,
         nve_run_time_steps=nve_run_time_steps,
-        project_parameter=project_parameter
+        project_parameter=project_parameter,
     )
     if debug_plot:
-        plt.plot(strain_value_lst, mean_lst, label='mean')
-        plt.plot(strain_value_lst, max_lst, label='max')
-        plt.axhline(np.mean(mean_lst) * 2, color='black', linestyle='--')
+        plt.plot(strain_value_lst, mean_lst, label="mean")
+        plt.plot(strain_value_lst, max_lst, label="max")
+        plt.axhline(np.mean(mean_lst) * 2, color="black", linestyle="--")
         plt.legend()
-        plt.xlabel('Strain')
-        plt.ylabel('Voronoi Volume')
+        plt.xlabel("Strain")
+        plt.ylabel("Voronoi Volume")
         plt.show()
     return np.array(max_lst) < np.mean(mean_lst) * 2
 
 
 def generate_structure(project_parameter):
     """
 
     Args:
         project_parameter:
 
     Returns:
 
     """
-    if 'lattice_constant' in project_parameter.keys():
-        basis = project_parameter['project'].create_structure(
-            project_parameter['element'],
-            project_parameter['crystalstructure'].lower(),
-            project_parameter['lattice_constant']
+    if "lattice_constant" in project_parameter.keys():
+        basis = project_parameter["project"].create_structure(
+            project_parameter["element"],
+            project_parameter["crystalstructure"].lower(),
+            project_parameter["lattice_constant"],
         )
     else:
-        basis = project_parameter['project'].create_ase_bulk(
-            project_parameter['element'],
-            project_parameter['crystalstructure'].lower(),
-            cubic=True
+        basis = project_parameter["project"].create_ase_bulk(
+            project_parameter["element"],
+            project_parameter["crystalstructure"].lower(),
+            cubic=True,
         )
     basis_lst = [basis.repeat([i, i, i]) for i in range(5, 30)]
-    basis = basis_lst[np.argmin([
-        np.abs(len(b) - project_parameter['number_of_atoms'] / 2)
-        for b in basis_lst
-    ])]
+    basis = basis_lst[
+        np.argmin(
+            [
+                np.abs(len(b) - project_parameter["number_of_atoms"] / 2)
+                for b in basis_lst
+            ]
+        )
+    ]
     return basis
 
 
 def generate_random_seed(project_parameter):
     """
     Generate random seed for project parameters
 
     Args:
         project_parameter (dict):
 
     Returns:
         dict: The project parameters dictionary including the key 'seed'
     """
-    if 'seed' not in project_parameter.keys():
-        project_parameter['seed'] = random.randint(0, 99999)
+    if "seed" not in project_parameter.keys():
+        project_parameter["seed"] = random.randint(0, 99999)
     return project_parameter
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/thermodynamics/sxphonons.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/thermodynamics/sxphonons.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 HARTREE_OVER_BOHR_TO_EV_OVER_ANGSTROM = HARTREE_TO_EV / BOHR_TO_ANGSTROM
 
 
 class SxUniqDispl(AtomisticGenericJob):
     def __init__(self, project, job_name):
         super(SxUniqDispl, self).__init__(project, job_name)
         self.__version__ = "0.1"
-        self.__name__ = "SxUniqDispl"
+
         self.input = GenericParameters(table_name="displacement")
         self.input["displacement"] = 0.01
         self.structure_lst = []
         self._id_pyi_to_spx = []
         self._id_spx_to_pyi = []
 
     @property
@@ -158,15 +158,15 @@
                 ]
 
 
 class SxDynMat(GenericJob):
     def __init__(self, project, job_name):
         super(SxDynMat, self).__init__(project, job_name)
         self.__version__ = "0.1"
-        self.__name__ = "SxDynMat"
+
         self._child_lst = []
         self._child_id_lst = []
 
     @property
     def child_id_lst(self):
         return self._child_id_lst
 
@@ -320,15 +320,15 @@
         return job
 
 
 class SxPhonons(AtomisticParallelMaster):
     def __init__(self, project, job_name):
         super(SxPhonons, self).__init__(project, job_name)
         self.__version__ = "0.1"
-        self.__name__ = "SxPhonons"
+
         self.input["displacement"] = (0.01, "atoms displacement, Ang")
         self._displacement_job = None
         self._dynmat_job = None
         self._job_generator = SxPhononsJobGenerator(self)
 
     def run_static(self):
         if self._displacement_job is None:
@@ -359,15 +359,15 @@
             return self.project_hdf5["output/hesse"]
 
 
 class SxHarmPotTst(AtomisticGenericJob):
     def __init__(self, project, job_name):
         super(SxHarmPotTst, self).__init__(project, job_name)
         self.__version__ = "0.1"
-        self.__name__ = "SxHarmPotTst"
+
         self.input = GenericParameters(table_name="interaction")
         self.input["interaction_radius"] = 4.0
         self.input["maximum_noise"] = 0.26
         self._positions_lst = []
         self._forces_lst = []
         self._md_job_id = None
         self._md_job = None
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/base.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,43 +5,47 @@
 from __future__ import print_function
 import os
 import posixpath
 import subprocess
 import numpy as np
 
 from pyiron_atomistics.dft.job.generic import GenericDFTJob
-from pyiron_atomistics.vasp.potential import VaspPotential, VaspPotentialFile, VaspPotentialSetter, Potcar, \
-    strip_xc_from_potential_name
+from pyiron_atomistics.vasp.potential import (
+    VaspPotential,
+    VaspPotentialFile,
+    VaspPotentialSetter,
+    Potcar,
+    strip_xc_from_potential_name,
+)
 from pyiron_atomistics.atomistics.structure.atoms import Atoms, CrystalStructure
-from pyiron_base import Settings, GenericParameters, deprecate
+from pyiron_base import state, GenericParameters, deprecate
 from pyiron_atomistics.vasp.outcar import Outcar
 from pyiron_atomistics.vasp.oszicar import Oszicar
 from pyiron_atomistics.vasp.procar import Procar
 from pyiron_atomistics.vasp.structure import read_atoms, write_poscar, vasp_sorter
 from pyiron_atomistics.vasp.vasprun import Vasprun as Vr
 from pyiron_atomistics.vasp.vasprun import VasprunError, VasprunWarning
 from pyiron_atomistics.vasp.volumetric_data import VaspVolumetricData
 from pyiron_atomistics.vasp.potential import get_enmax_among_potentials
 from pyiron_atomistics.dft.waves.electronic import ElectronicStructure
 from pyiron_atomistics.dft.waves.bandstructure import Bandstructure
+from pyiron_atomistics.dft.bader import Bader
 import warnings
 
 __author__ = "Sudarsan Surendralal, Felix Lochner"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Sudarsan Surendralal"
 __email__ = "surendralal@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
-s = Settings()
-
 
 class VaspBase(GenericDFTJob):
     """
     Class to setup and run and analyze VASP simulations which is a derivative of pyiron_atomistics.objects.job.generic.GenericJob.
     The functions in these modules are written in such the function names and attributes are very generic
     (get_structure(), molecular_dynamics(), version) but the functions are written to handle VASP specific input/output.
 
@@ -78,15 +82,15 @@
         self._sorted_indices = None
         self.input = Input()
         self.input.incar["SYSTEM"] = self.job_name
         self._output_parser = Output()
         self._potential = VaspPotentialSetter([])
         self._compress_by_default = True
         self.get_enmax_among_species = get_enmax_among_potentials
-        s.publication_add(self.publication)
+        state.publications.add(self.publication)
 
     @property
     def structure(self):
         """
 
         Returns:
 
@@ -142,15 +146,15 @@
 
     @property
     def spin_constraints(self):
         """
         Returns True if the calculation is spin constrained
         """
         if "I_CONSTRAINED_M" in self.input.incar._dataset["Parameter"]:
-            return (self.input.incar["I_CONSTRAINED_M"] >= 1)
+            return self.input.incar["I_CONSTRAINED_M"] >= 1
         else:
             return False
 
     @spin_constraints.setter
     def spin_constraints(self, val):
         self.input.incar["I_CONSTRAINED_M"] = val
 
@@ -268,15 +272,17 @@
         if self.structure is None:
             raise ValueError("Can't list potentials unless a structure is set")
         else:
             df = VaspPotentialFile(xc=self.input.potcar["xc"]).find(
                 self.structure.get_species_symbols().tolist()
             )
             if len(df) > 0:
-                df["Name"] = [strip_xc_from_potential_name(n) for n in df["Name"].values]
+                df["Name"] = [
+                    strip_xc_from_potential_name(n) for n in df["Name"].values
+                ]
             return df
 
     @property
     def potential_list(self):
         return list(self.potential_view["Name"].values)
 
     @property
@@ -387,25 +393,51 @@
                 directory=self.working_directory, sorted_indices=self.sorted_indices
             )
         except VaspCollectError:
             self.status.aborted = True
             return
         # Try getting high precision positions from CONTCAR
         try:
-            self._output_parser.structure = self.get_final_structure_from_file(filename="CONTCAR")
+            self._output_parser.structure = self.get_final_structure_from_file(
+                filename="CONTCAR"
+            )
         except (IOError, ValueError, FileNotFoundError):
             pass
 
+        # Bader analysis
+        if os.path.isfile(
+            os.path.join(self.working_directory, "AECCAR0")
+        ) and os.path.isfile(os.path.join(self.working_directory, "AECCAR2")):
+            bader = Bader(self)
+            try:
+                charges_orig, volumes_orig = bader.compute_bader_charges()
+            except ValueError:
+                warnings.warn("Invoking Bader charge analysis failed")
+                self.logger.warning("Invoking Bader charge analysis failed")
+            else:
+                charges, volumes = charges_orig.copy(), volumes_orig.copy()
+                charges[self.sorted_indices] = charges_orig
+                volumes[self.sorted_indices] = volumes_orig
+                if (
+                    "valence_charges"
+                    in self._output_parser.generic_output.dft_log_dict.keys()
+                ):
+                    valence_charges = self._output_parser.generic_output.dft_log_dict[
+                        "valence_charges"
+                    ]
+                    # Positive values indicate electron depletion
+                    self._output_parser.generic_output.dft_log_dict["bader_charges"] = (
+                        valence_charges - charges
+                    )
+                self._output_parser.generic_output.dft_log_dict[
+                    "bader_volumes"
+                ] = volumes
         self._output_parser.to_hdf(self._hdf5)
         if len(self._exclude_groups_hdf) > 0 or len(self._exclude_nodes_hdf) > 0:
-            self.project_hdf5.rewrite_hdf5(
-                job_name=self.job_name,
-                exclude_groups=self._exclude_groups_hdf,
-                exclude_nodes=self._exclude_nodes_hdf,
-            )
+            self.project_hdf5.rewrite_hdf5()
 
     def convergence_check(self):
         """
         Checks for electronic and ionic convergence according to the user specified tolerance
 
         Returns:
 
@@ -505,18 +537,24 @@
         if os.path.exists(file_name):
             with open(file_name, "r") as f:
                 lines = f.readlines()
 
             # EDDRMM
             # If the wrong convergence algorithm is chosen, we get the following error.
             # https://cms.mpi.univie.ac.at/vasp-forum/viewtopic.php?f=4&t=17071
-            lines_where_eddrmm = np.argwhere([eddrmm_error_str in l for l in lines]).flatten()
+            lines_where_eddrmm = np.argwhere(
+                [eddrmm_error_str in l for l in lines]
+            ).flatten()
             num_eddrmm = len(lines_where_eddrmm)
             if num_eddrmm > 0:
-                snap_eddrmm = len(np.argwhere(["E0=" in l for l in lines[:lines_where_eddrmm[0]]]).flatten())
+                snap_eddrmm = len(
+                    np.argwhere(
+                        ["E0=" in l for l in lines[: lines_where_eddrmm[0]]]
+                    ).flatten()
+                )
 
             # ZBRENT
             for l in lines:
                 if zbrent_error_str in l:
                     zbrent_status = True
                     break
 
@@ -525,24 +563,32 @@
             self.status.aborted = True
             self._logger.warning(zbrent_warning_str + aborted_status_str)
         elif snap_eddrmm is not None:
             if self.get_eddrmm_handling() == "ignore":
                 self._logger.warning(eddrmm_warning_str.format(num_eddrmm, snap_eddrmm))
             elif self.get_eddrmm_handling() == "warn":
                 self.status.warning = True
-                self._logger.warning(eddrmm_warning_str.format(num_eddrmm, snap_eddrmm) + warning_status_str)
+                self._logger.warning(
+                    eddrmm_warning_str.format(num_eddrmm, snap_eddrmm)
+                    + warning_status_str
+                )
             elif self.get_eddrmm_handling() == "restart":
                 self.status.warning = True
-                self._logger.warning(eddrmm_warning_str.format(num_eddrmm, snap_eddrmm) + warning_status_str)
+                self._logger.warning(
+                    eddrmm_warning_str.format(num_eddrmm, snap_eddrmm)
+                    + warning_status_str
+                )
                 if not self.input.incar["ALGO"].lower() == "normal":
                     ham_new = self.copy_hamiltonian(self.name + "_normal")
                     ham_new.input.incar["ALGO"] = "Normal"
                     ham_new.set_eddrmm_handling()
                     ham_new.run()
-                    self._logger.info("Job was restarted with 'ALGO' = 'Normal' to avoid EDDRMM warning.")
+                    self._logger.info(
+                        "Job was restarted with 'ALGO' = 'Normal' to avoid EDDRMM warning."
+                    )
 
     def copy_hamiltonian(self, job_name):
         """
         Copies a job to new one with a different name.
 
         Args:
             job_name (str): Job name
@@ -605,16 +651,22 @@
                     self.input.kpoints.read_input(
                         posixpath.join(directory, "KPOINTS"), ignore_trigger="!"
                     )
                 except (IndexError, TypeError, ValueError):
                     pass
             if "POSCAR" in files:
                 if "POTCAR" in files:
-                    structure = read_atoms(posixpath.join(directory, "POSCAR"),
-                                           species_from_potcar=True)
+                    try:
+                        structure = read_atoms(
+                            posixpath.join(directory, "POSCAR"),
+                            species_from_potcar=True,
+                        )
+                    # In order to handle cases where the species info. is corrputed in POTCAR files
+                    except KeyError:
+                        structure = read_atoms(posixpath.join(directory, "POSCAR"))
                 else:
                     structure = read_atoms(posixpath.join(directory, "POSCAR"))
             elif "CONTCAR" in files:
                 structure = read_atoms(posixpath.join(directory, "CONTCAR"))
             elif "vasprun.xml" in files:
                 structure = vp_new.get_initial_structure()
             else:
@@ -760,20 +812,21 @@
                         if isinstance(spin, (list, np.ndarray))
                         else str(spin)
                         for spin in self.structure.get_initial_magnetic_moments()[
                             self.sorted_indices
                         ]
                     ]
                 )
-                s.logger.debug("Magnetic Moments are: {0}".format(final_cmd))
+                state.logger.debug("Magnetic Moments are: {0}".format(final_cmd))
                 if "MAGMOM" not in self.input.incar._dataset["Parameter"]:
                     self.input.incar["MAGMOM"] = final_cmd
                 if any(
                     [
-                        isinstance(spin, (list, np.ndarray)) for spin in self.structure.get_initial_magnetic_moments()
+                        isinstance(spin, (list, np.ndarray))
+                        for spin in self.structure.get_initial_magnetic_moments()
                     ]
                 ):
                     self.input.incar["LNONCOLLINEAR"] = True
                     if (
                         self.spin_constraints
                         and "M_CONSTR" not in self.input.incar._dataset["Parameter"]
                     ):
@@ -799,19 +852,19 @@
                             "Parameter RWIGS has to be set for spin constraint calculations"
                         )
                 if self.spin_constraints and not self.input.incar["LNONCOLLINEAR"]:
                     raise ValueError(
                         "Spin constraints are only avilable for non collinear calculations."
                     )
             else:
-                s.logger.debug(
+                state.logger.debug(
                     "Spin polarized calculation is switched off by the user. No magnetic moments are written."
                 )
         else:
-            s.logger.debug("No magnetic moments")
+            state.logger.debug("No magnetic moments")
 
     def set_eddrmm_handling(self, status="warn"):
         """
         Sets the way, how EDDRMM warning is handled.
 
         Args:
             status (str): new status of EDDRMM handling (can be 'warn', 'ignore', or 'restart')
@@ -866,15 +919,15 @@
             self.input.incar["LDAUTYPE"] = interaction_type
             self.input.incar["LDAUL"] = " ".join(ldaul)
             self.input.incar["LDAUU"] = " ".join(ldauu)
             self.input.incar["LDAUJ"] = " ".join(ldauj)
             if ldau_print:
                 self.input.incar["LDAUPRINT"] = 2
         else:
-            s.logger.debug("No on site coulomb interactions")
+            state.logger.debug("No on site coulomb interactions")
 
     def set_algorithm(self, algorithm="Fast", ialgo=None):
         """
         Sets the type of electronic minimization algorithm
 
         Args:
             algorithm (str): Algorithm defined by VASP (Fast, Normal etc.)
@@ -882,15 +935,15 @@
         """
         algorithm_list = ["Fast", "Accurate", "Normal", "Very Fast"]
         if ialgo is not None:
             self.input.incar["IALGO"] = int(ialgo)
         else:
             self.input.incar["ALGO"] = str(algorithm)
             if algorithm not in algorithm_list:
-                s.logger.warning(
+                state.logger.warning(
                     msg="Algorithm {} is unusual for VASP. "
                     "I hope you know what you are up to".format(algorithm)
                 )
 
     def calc_minimize(
         self,
         electronic_steps=60,
@@ -901,14 +954,15 @@
         retain_charge_density=False,
         retain_electrostatic_potential=False,
         ionic_energy=None,
         ionic_forces=None,
         ionic_energy_tolerance=None,
         ionic_force_tolerance=None,
         volume_only=False,
+        cell_only=False,
     ):
         """
         Function to setup the hamiltonian to perform ionic relaxations using DFT. The ISIF tag has to be supplied
         separately.
 
         Args:
             electronic_steps (int): Maximum number of electronic steps
@@ -918,15 +972,16 @@
             algorithm (str): Type of VASP algorithm to be used "Fast"/"Accurate"
             retain_charge_density (bool): True if the charge density should be written
             retain_electrostatic_potential (boolean): True if the electrostatic potential should be written
             ionic_energy_tolerance (float): Ionic energy convergence criteria (eV)
             ionic_force_tolerance (float): Ionic forces convergence criteria (overwrites ionic energy) (ev/A)
             ionic_energy (float): Same as ionic_energy_tolerance (deprecated)
             ionic_forces (float): Same as ionic_force_tolerance (deprecated)
-            volume_only (bool): Option to relax only the volume (keeping the relative coordinates fixed
+            volume_only (bool): Option to relax only the volume (keeping the relative coordinates fixed)
+            cell_only (bool): Option to relax only the cell parameters (keeping the relative coordinates fixed)
         """
         super(VaspBase, self).calc_minimize(
             electronic_steps=electronic_steps,
             ionic_steps=ionic_steps,
             max_iter=max_iter,
             pressure=pressure,
             algorithm=algorithm,
@@ -934,37 +989,44 @@
             retain_electrostatic_potential=retain_electrostatic_potential,
             ionic_energy_tolerance=ionic_energy_tolerance,
             ionic_force_tolerance=ionic_force_tolerance,
             volume_only=volume_only,
         )
         if volume_only:
             self.input.incar["ISIF"] = 7
+        elif cell_only:
+            self.input.incar["ISIF"] = 6
         else:
             if pressure == 0.0:
                 self.input.incar["ISIF"] = 3
-            else:
+            elif pressure is None:
                 self.input.incar["ISIF"] = 2
+            else:
+                raise ValueError("Non-zero pressure not supported!")
 
         if max_iter:
             electronic_steps = max_iter
             ionic_steps = max_iter
 
         self.input.incar["IBRION"] = 2
         self.input.incar["NELM"] = electronic_steps
         self.input.incar["NSW"] = ionic_steps
         if algorithm is not None:
             self.set_algorithm(algorithm=algorithm)
         if retain_charge_density:
             self.write_charge_density = retain_charge_density
         if retain_electrostatic_potential:
             self.write_electrostatic_potential = retain_electrostatic_potential
-        self.set_convergence_precision(ionic_force_tolerance=ionic_force_tolerance,
-                                       ionic_energy_tolerance=ionic_energy_tolerance,
-                                       ionic_energy=ionic_energy, ionic_forces=ionic_forces,
-                                       electronic_energy=None)
+        self.set_convergence_precision(
+            ionic_force_tolerance=ionic_force_tolerance,
+            ionic_energy_tolerance=ionic_energy_tolerance,
+            ionic_energy=ionic_energy,
+            ionic_forces=ionic_forces,
+            electronic_energy=None,
+        )
 
     def calc_static(
         self,
         electronic_steps=100,
         algorithm=None,
         retain_charge_density=False,
         retain_electrostatic_potential=False,
@@ -1000,15 +1062,15 @@
         self,
         temperature=None,
         n_ionic_steps=1000,
         n_print=1,
         time_step=1.0,
         retain_charge_density=False,
         retain_electrostatic_potential=False,
-        **kwargs
+        **kwargs,
     ):
         """
         Sets appropriate tags for molecular dynamics in VASP
 
         Args:
             temperature (int/float/list): Temperature/ range of temperatures in Kelvin
             n_ionic_steps (int): Maximum number of ionic steps
@@ -1020,15 +1082,15 @@
         super(VaspBase, self).calc_md(
             temperature=temperature,
             n_ionic_steps=n_ionic_steps,
             n_print=n_print,
             time_step=time_step,
             retain_charge_density=retain_charge_density,
             retain_electrostatic_potential=retain_electrostatic_potential,
-            **kwargs
+            **kwargs,
         )
         if temperature is not None:
             # NVT ensemble
             self.input.incar["SMASS"] = 3
             if isinstance(temperature, (int, float)):
                 self.input.incar["TEBEG"] = temperature
             else:
@@ -1084,17 +1146,21 @@
         if scheme == "MP":
             if mesh is None:
                 mesh = [int(val) for val in self.input.kpoints[3].split()]
             self.input.kpoints.set_kpoints_file(size_of_mesh=mesh, shift=center_shift)
         if scheme == "GC":
             if mesh is None:
                 mesh = [int(val) for val in self.input.kpoints[3].split()]
-            self.input.kpoints.set_kpoints_file(size_of_mesh=mesh, shift=center_shift, method="Gamma centered")
+            self.input.kpoints.set_kpoints_file(
+                size_of_mesh=mesh, shift=center_shift, method="Gamma centered"
+            )
         if scheme == "GP":
-            self.input.kpoints.set_kpoints_file(size_of_mesh=[1, 1, 1], method="Gamma Point")
+            self.input.kpoints.set_kpoints_file(
+                size_of_mesh=[1, 1, 1], method="Gamma Point"
+            )
         if scheme == "Line":
             if n_path is None and self.input.kpoints._n_path is None:
                 raise ValueError("n_path has to be defined")
             high_symmetry_points = self.structure.get_high_symmetry_points()
             if high_symmetry_points is None:
                 raise ValueError("high_symmetry_points has to be defined")
 
@@ -1107,15 +1173,15 @@
                 self.input.kpoints._path_name = path_name
             if n_path is not None:
                 self.input.kpoints._n_path = n_path
 
             self.input.kpoints.set_kpoints_file(
                 method="Line",
                 n_path=self.input.kpoints._n_path,
-                path=self._get_path_for_kpoints(self.input.kpoints._path_name)
+                path=self._get_path_for_kpoints(self.input.kpoints._path_name),
             )
         if scheme == "Manual":
             if manual_kpoints is None:
                 raise ValueError(
                     "For the manual mode, the kpoints list should be specified"
                 )
             else:
@@ -1183,19 +1249,25 @@
             scheme="Manual",
             symmetry_reduction=False,
             manual_kpoints=q_point_list,
             weights=None,
             reciprocal=False,
         )
 
-    @deprecate(ionic_forces="Use ionic_force_tolerance",
-               ionic_energy="use ionic_energy_tolerance")
+    @deprecate(
+        ionic_forces="Use ionic_force_tolerance",
+        ionic_energy="use ionic_energy_tolerance",
+    )
     def set_convergence_precision(
-        self, ionic_energy_tolerance=1.0e-3, electronic_energy=1.0e-7, ionic_force_tolerance=1.0e-2,
-        ionic_energy=None, ionic_forces=None
+        self,
+        ionic_energy_tolerance=1.0e-3,
+        electronic_energy=1.0e-7,
+        ionic_force_tolerance=1.0e-2,
+        ionic_energy=None,
+        ionic_forces=None,
     ):
         """
         Sets the electronic and ionic convergence precision. For ionic convergence either the energy or the force
         precision is required
 
         Args:
             ionic_energy_tolerance (float): Ionic energy convergence precision (eV)
@@ -1212,15 +1284,17 @@
                 ionic_energy_tolerance = ionic_energy
         if ionic_force_tolerance is not None:
             self.input.incar["EDIFFG"] = -1.0 * abs(ionic_force_tolerance)
         elif ionic_energy_tolerance is not None:
             self.input.incar["EDIFFG"] = abs(ionic_energy_tolerance)
         else:
             # Using default convergence criterion
-            self.input.incar["EDIFFG"] = -0.01
+            self.input.incar["EDIFFG"] = (
+                -0.01 if self.input.incar["ISIF"] not in (5, 6, 7) else 0.01
+            )
         if electronic_energy is not None:
             self.input.incar["EDIFF"] = electronic_energy
 
     def set_dipole_correction(self, direction=2, dipole_center=None):
         """
         Apply a dipole correction using the dipole layer method proposed by `Neugebauer & Scheffler`_
 
@@ -1254,29 +1328,49 @@
         self.input.incar["LORBIT"] = 11
         self.input.incar["IDIPOL"] = direction + 1
         self.input.incar["LDIPOL"] = True
         self.input.incar["EFIELD"] = e_field
         if dipole_center is not None:
             self.input.incar["DIPOL"] = " ".join(str(val) for val in dipole_center)
 
-    def set_occupancy_smearing(self, smearing="fermi", width=0.2, ismear=None):
+    @deprecate(
+        ismear="Preferably use parameters `smearing` and `order` "
+        "to set the type of smearing you want"
+    )
+    def set_occupancy_smearing(
+        self,
+        smearing: str = None,
+        width: float = None,
+        order: int = 1,
+        ismear: int = None,
+    ) -> None:
         """
         Set how the finite temperature smearing is applied in determining partial occupancies
 
         Args:
-            smearing (str): Type of smearing (fermi/gaussian etc.)
+            smearing (str): Type of smearing (Fermi, Gaussian, or Methfessel-Paxton)
             width (float): Smearing width (eV)
-            ismear (int): Directly sets the ISMEAR tag. Overwrites the smearing tag
+            order (int): order (int): Smearing order (only for Methfessel-Paxton)
+            ismear (int): (Deprecated) Directly sets the ISMEAR tag. Overwrites the smearing tag
         """
-        ismear_dict = {"fermi": -1, "gaussian": 0, "MP": 1}
         if ismear is not None:
             self.input.incar["ISMEAR"] = int(ismear)
+        elif smearing.lower().startswith("meth") or smearing.lower().startswith("mp"):
+            self.input.incar["ISMEAR"] = int(order)
+        elif smearing.lower().startswith("fermi"):
+            self.input.incar["ISMEAR"] = -1
+        elif smearing.lower().startswith("gauss"):
+            self.input.incar["ISMEAR"] = 0
         else:
-            self.input.incar["ISMEAR"] = ismear_dict[smearing]
-        self.input.incar["SIGMA"] = width
+            raise ValueError(
+                f"Smearing scheme {smearing} is not available. Only types 'Fermi', 'Gaussian', "
+                f"and 'Methfessel-Paxton'"
+            )
+        if width is not None:
+            self.input.incar["SIGMA"] = width
 
     def set_fft_mesh(self, nx=None, ny=None, nz=None):
         """
         Set the number of points in the respective directions for the 3D FFT mesh used for computing the charge density
         or electrostatic potentials. In VASP, using PAW potentials, this refers to the "finer fft mesh". If no values
         are set, the default settings from Vasp are used to set the number of grid points.
 
@@ -1298,25 +1392,26 @@
         n_pulay_steps=None,
         density_mixing_parameter=None,
         spin_mixing_parameter=None,
         density_residual_scaling=None,
         spin_residual_scaling=None,
     ):
         if density_residual_scaling is not None or spin_residual_scaling is not None:
-            raise NotImplementedError('Residual scaling is not implemented in VASP')
+            raise NotImplementedError("Residual scaling is not implemented in VASP")
         if method is None:
             method = "PULAY"
         if method.upper() == "PULAY":
             self.input.incar["IMIX"] = 4
         if method.upper() == "KERKER":
             self.input.incar["IMIX"] = 1
         if n_pulay_steps is not None:
             self.input.incar["MAXMIX"] = n_pulay_steps
         if density_mixing_parameter is not None:
             self.input.incar["AMIX"] = density_mixing_parameter
+
     set_mixing_parameters.__doc__ = GenericDFTJob.set_mixing_parameters.__doc__
 
     def set_empty_states(self, n_empty_states=None):
         """
         Sets the number of empty states in the calculation
         Args:
             n_empty_states (int): Required number of empty states
@@ -1374,14 +1469,32 @@
             return
         else:
             with self.project_hdf5.open("output") as ho:
                 cd_obj = VaspVolumetricData()
                 cd_obj.from_hdf(ho, "charge_density")
             return cd_obj
 
+    def get_valence_and_total_charge_density(self):
+        """
+        Gives the valence and total charge densities
+
+        Returns:
+            tuple: The required charge densities
+        """
+        cd_core = VaspVolumetricData()
+        cd_total = VaspVolumetricData()
+        cd_val = VaspVolumetricData()
+        if os.path.isfile(self.working_directory + "/AECCAR0"):
+            cd_core.from_file(self.working_directory + "/AECCAR0")
+            cd_val.from_file(self.working_directory + "/AECCAR2")
+            cd_val.atoms = cd_val.atoms
+            cd_total.total_data = cd_core.total_data + cd_val.total_data
+            cd_total.atoms = cd_val.atoms
+        return cd_val, cd_total
+
     def get_electrostatic_potential(self):
         """
         Gets the electrostatic potential from the hdf5 file.
 
         Returns:
                 atomistics.volumetric.generic.VolumetricData instance
         """
@@ -1391,26 +1504,27 @@
             with self.project_hdf5.open("output") as ho:
                 es_obj = VaspVolumetricData()
                 es_obj.from_hdf(ho, "electrostatic_potential")
             return es_obj
 
     def restart(self, job_name=None, job_type=None):
         """
-        Restart a new job created from an existing Vasp calculation.
+        Creates a "restart" job from an existing Vasp calculation.
+        (Default behaviour is to copy CONTCAR -> POSCAR, all other job inputs are copied from original job)
+
+        Usage: job.restart().run() restarts the job with job_name: "$(original_job_name)_restart"
 
         Args:
             job_name (str): Job name
             job_type (str): Job type. If not specified a Vasp job type is assumed
 
         Returns:
             new_ham (vasp.vasp.Vasp instance): New job
         """
-        new_ham = super(VaspBase, self).restart(
-            job_name=job_name, job_type=job_type
-        )
+        new_ham = super(VaspBase, self).restart(job_name=job_name, job_type=job_type)
         if new_ham.__name__ == self.__name__:
             new_ham.input.potcar["xc"] = self.input.potcar["xc"]
         if new_ham.input.incar["MAGMOM"] is not None:
             del new_ham.input.incar["MAGMOM"]
         if new_ham.input.incar["M_CONSTR"] is not None:
             del new_ham.input.incar["M_CONSTR"]
         if new_ham.input.incar["LNONCOLLINEAR"] is not None:
@@ -1425,18 +1539,15 @@
         Args:
             job_name (str/None): Job name
 
         Returns:
             new_ham (vasp.vasp.Vasp instance): New job
         """
         return self.restart_from_charge_density(
-            job_name=job_name,
-            job_type=None,
-            icharg=11,
-            self_consistent_calc=None
+            job_name=job_name, job_type=None, icharg=11, self_consistent_calc=None
         )
 
     def get_icharg_value(self, icharg=None, self_consistent_calc=None):
         """
         Gives the correct ICHARG value for the restart calculation.
 
         Args:
@@ -1449,20 +1560,25 @@
 
         """
         if icharg is None:
             if self_consistent_calc is True:
                 return 1
             if self_consistent_calc is False:
                 return 11
-            if ("ICHARG" in self.input.incar.keys() and int(self.input.incar["ICHARG"]) > 9):
+            if (
+                "ICHARG" in self.input.incar.keys()
+                and int(self.input.incar["ICHARG"]) > 9
+            ):
                 return 11
             return 1
         if icharg not in [0, 1, 2, 4, 10, 11, 12]:
             raise ValueError(
-                "The value '{}' is not a proper input for 'icharg'. Look at VASP manual.".format(icharg)
+                "The value '{}' is not a proper input for 'icharg'. Look at VASP manual.".format(
+                    icharg
+                )
             )
         return icharg
 
     def restart_from_charge_density(
         self,
         job_name=None,
         job_type=None,
@@ -1479,25 +1595,17 @@
             self_consistent_calc (bool/None): If 'True' returns 1, if 'False' returns 11,
                 if 'None' returns based on the job either 1 or 11.
 
         Returns:
             new_ham (vasp.vasp.Vasp instance): New job
         """
         new_ham = self.restart(job_name=job_name, job_type=job_type)
+
         if new_ham.__name__ == self.__name__:
-            try:
-                new_ham.restart_file_list.append(
-                    posixpath.join(self.working_directory, "CHGCAR")
-                )
-            except IOError:
-                self.logger.warning(
-                    msg="A CHGCAR from job: {} is not generated and therefore it can't be read.".format(
-                        self.job_name
-                    )
-                )
+            new_ham.restart_file_list.append(self.get_workdir_file("CHGCAR"))
             new_ham.input.incar["ICHARG"] = self.get_icharg_value(
                 icharg=icharg,
                 self_consistent_calc=self_consistent_calc,
             )
         return new_ham
 
     def append_charge_density(self, job_specifier=None, path=None):
@@ -1538,36 +1646,17 @@
             istart (int): Vasp ISTART tag
 
         Returns:
             new_ham (vasp.vasp.Vasp instance): New job
         """
         new_ham = self.restart(job_name=job_name, job_type=job_type)
         if new_ham.__name__ == self.__name__:
-            try:
-                new_ham.restart_file_list.append(
-                    posixpath.join(self.working_directory, "CHGCAR")
-                )
-            except IOError:
-                self.logger.warning(
-                    msg="A CHGCAR from job: {} is not generated and therefore it can't be read.".format(
-                        self.job_name
-                    )
-                )
-            try:
-                new_ham.restart_file_list.append(
-                    posixpath.join(self.working_directory, "WAVECAR")
-                )
-            except IOError:
-                self.logger.warning(
-                    msg="A WAVECAR from job: {} is not generated and therefore it can't be read.".format(
-                        self.job_name
-                    )
-                )
+            new_ham.restart_file_list.append(self.get_workdir_file("CHGCAR"))
+            new_ham.restart_file_list.append(self.get_workdir_file("WAVECAR"))
             new_ham.input.incar["ISTART"] = istart
-
             new_ham.input.incar["ICHARG"] = self.get_icharg_value(
                 icharg=icharg,
                 self_consistent_calc=self_consistent_calc,
             )
         return new_ham
 
     def compress(self, files_to_compress=None):
@@ -1577,54 +1666,51 @@
         Args:
             files_to_compress (list): A list of files to compress (optional)
         """
         if files_to_compress is None:
             files_to_compress = [
                 f
                 for f in list(self.list_files())
-                if f not in ["CHGCAR", "CONTCAR", "WAVECAR", "STOPCAR"]
+                if f
+                not in [
+                    "CHGCAR",
+                    "CONTCAR",
+                    "WAVECAR",
+                    "STOPCAR",
+                    "AECCAR0",
+                    "AECCAR1",
+                    "AECCAR2",
+                ]
             ]
         # delete empty files
         for f in list(self.list_files()):
             filename = os.path.join(self.working_directory, f)
             if (
                 f not in files_to_compress
                 and os.path.exists(filename)
                 and os.stat(filename).st_size == 0
             ):
                 os.remove(filename)
         super(VaspBase, self).compress(files_to_compress=files_to_compress)
 
-    def restart_from_wave_functions(
-        self, job_name=None, job_type=None, istart=1
-    ):
-
+    def restart_from_wave_functions(self, job_name=None, job_type=None, istart=1):
         """
         Restart a new job created from an existing Vasp calculation by reading the wave functions.
 
         Args:
             job_name (str/None): Job name
             job_type (str/None): Job type. If not specified a Vasp job type is assumed
             istart (int): Vasp ISTART tag
 
         Returns:
             new_ham (vasp.vasp.Vasp instance): New job
         """
         new_ham = self.restart(job_name=job_name, job_type=job_type)
         if new_ham.__name__ == self.__name__:
-            try:
-                new_ham.restart_file_list.append(
-                    posixpath.join(self.working_directory, "WAVECAR")
-                )
-            except IOError:
-                self.logger.warning(
-                    msg="A WAVECAR from job: {} is not generated and therefore it can't be read.".format(
-                        self.job_name
-                    )
-                )
+            new_ham.restart_file_list.append(self.get_workdir_file("WAVECAR"))
             new_ham.input.incar["ISTART"] = istart
         return new_ham
 
     def append_wave_function(self, job_specifier=None, path=None):
         """
         Append wave function file (WAVECAR)
 
@@ -1699,15 +1785,17 @@
         if direction and norm:
             self.input.incar["I_CONSTRAINED_M"] = 2
         elif direction:
             self.input.incar["I_CONSTRAINED_M"] = 1
         elif norm:
             raise ValueError("Constraining norm only is not possible.")
         else:
-            raise ValueError("You have to constrain either direction or norm and direction.")
+            raise ValueError(
+                "You have to constrain either direction or norm and direction."
+            )
 
         self.input.incar["LAMBDA"] = lamb
         self.set_rwigs(rwigs_dict)
 
     def validate_ready_to_run(self):
         super(VaspBase, self).validate_ready_to_run()
         if "spin_constraint" in self.structure._tag_list.keys():
@@ -1762,15 +1850,18 @@
         Writes all the input files to a specified directory
 
         Args:
             structure (atomistics.structure.atoms.Atoms instance): Structure to be written
             directory (str): The working directory for the VASP run
         """
         self.incar.write_file(file_name="INCAR", cwd=directory)
-        self.kpoints.write_file(file_name="KPOINTS", cwd=directory)
+        if "KSPACING" in self.incar.keys():
+            warnings.warn("'KSPACING' found in INCAR, no KPOINTS file written")
+        else:
+            self.kpoints.write_file(file_name="KPOINTS", cwd=directory)
         self.potcar.potcar_set_structure(structure, modified_elements)
         self.potcar.write_file(file_name="POTCAR", cwd=directory)
         # Write the species info in the POSCAR file only if there are no user defined species
         is_user_defined = list()
         for species in structure.get_species_objects():
             is_user_defined.append(species.Parent is not None)
         do_not_write_species = any(is_user_defined)
@@ -1814,21 +1905,23 @@
             self.kpoints.from_hdf(hdf5_input)
             self.potcar.from_hdf(hdf5_input)
 
             self._eddrmm = "ignore"
             if "vasp_dict" in hdf5_input.list_nodes():
                 vasp_dict = hdf5_input["vasp_dict"]
                 if "eddrmm_handling" in vasp_dict.keys():
-                    self._eddrmm = self._eddrmm_backwards_compatibility(vasp_dict["eddrmm_handling"])
+                    self._eddrmm = self._eddrmm_backwards_compatibility(
+                        vasp_dict["eddrmm_handling"]
+                    )
 
     @staticmethod
     def _eddrmm_backwards_compatibility(eddrmm_value):
         """On 9-03-2020, the EDDRMM flag 'not_converged' was switched to 'warn'."""
-        if eddrmm_value == 'not_converged':
-            return 'warn'
+        if eddrmm_value == "not_converged":
+            return "warn"
         else:
             return eddrmm_value
 
 
 class Output:
     """
     Handles the output from a VASP simulation.
@@ -1887,27 +1980,37 @@
         if "OUTCAR" in files_present:
             self.outcar.from_file(filename=posixpath.join(directory, "OUTCAR"))
             outcar_working = True
         if "vasprun.xml" in files_present:
             try:
                 with warnings.catch_warnings(record=True) as w:
                     warnings.simplefilter("always")
-                    self.vp_new.from_file(filename=posixpath.join(directory, "vasprun.xml"))
+                    self.vp_new.from_file(
+                        filename=posixpath.join(directory, "vasprun.xml")
+                    )
                     if any([isinstance(warn.category, VasprunWarning) for warn in w]):
-                        s.logger.warning("vasprun.xml parsed but with some inconsistencies. "
-                                         "Check vasp output to be sure")
-                        warnings.warn("vasprun.xml parsed but with some inconsistencies. "
-                                      "Check vasp output to be sure", VasprunWarning)
+                        state.logger.warning(
+                            "vasprun.xml parsed but with some inconsistencies. "
+                            "Check vasp output to be sure"
+                        )
+                        warnings.warn(
+                            "vasprun.xml parsed but with some inconsistencies. "
+                            "Check vasp output to be sure",
+                            VasprunWarning,
+                        )
             except VasprunError:
-                s.logger.warning("Unable to parse the vasprun.xml file. Will attempt to get data from OUTCAR")
+                state.logger.warning(
+                    "Unable to parse the vasprun.xml file. Will attempt to get data from OUTCAR"
+                )
             else:
                 # If parsing the vasprun file does not throw an error, then set to True
                 vasprun_working = True
         if outcar_working:
             log_dict["temperature"] = self.outcar.parse_dict["temperatures"]
+            log_dict["stresses"] = self.outcar.parse_dict["stresses"]
             log_dict["pressures"] = self.outcar.parse_dict["pressures"]
             log_dict["elastic_constants"] = self.outcar.parse_dict["elastic_constants"]
             self.generic_output.dft_log_dict["n_elect"] = self.outcar.parse_dict[
                 "n_elect"
             ]
             if len(self.outcar.parse_dict["magnetization"]) > 0:
                 magnetization = np.array(self.outcar.parse_dict["magnetization"]).copy()
@@ -1920,61 +2023,72 @@
                         final_magmoms[:, sorted_indices] = final_magmoms.copy()
                 self.generic_output.dft_log_dict[
                     "magnetization"
                 ] = magnetization.tolist()
                 self.generic_output.dft_log_dict[
                     "final_magmoms"
                 ] = final_magmoms.tolist()
-            self.generic_output.dft_log_dict["e_fermi_list"] = self.outcar.parse_dict["e_fermi_list"]
-            self.generic_output.dft_log_dict["vbm_list"] = self.outcar.parse_dict["vbm_list"]
-            self.generic_output.dft_log_dict["cbm_list"] = self.outcar.parse_dict["cbm_list"]
+            self.generic_output.dft_log_dict["e_fermi_list"] = self.outcar.parse_dict[
+                "e_fermi_list"
+            ]
+            self.generic_output.dft_log_dict["vbm_list"] = self.outcar.parse_dict[
+                "vbm_list"
+            ]
+            self.generic_output.dft_log_dict["cbm_list"] = self.outcar.parse_dict[
+                "cbm_list"
+            ]
 
         if vasprun_working:
             log_dict["forces"] = self.vp_new.vasprun_dict["forces"]
             log_dict["cells"] = self.vp_new.vasprun_dict["cells"]
-            log_dict["volume"] = [
-                np.linalg.det(cell) for cell in self.vp_new.vasprun_dict["cells"]
-            ]
+            log_dict["volume"] = np.linalg.det(self.vp_new.vasprun_dict["cells"])
             # log_dict["total_energies"] = self.vp_new.vasprun_dict["total_energies"]
             log_dict["energy_tot"] = self.vp_new.vasprun_dict["total_energies"]
             if "kinetic_energies" in self.vp_new.vasprun_dict.keys():
                 log_dict["energy_pot"] = (
                     log_dict["energy_tot"]
                     - self.vp_new.vasprun_dict["kinetic_energies"]
                 )
             else:
                 log_dict["energy_pot"] = log_dict["energy_tot"]
             log_dict["steps"] = np.arange(len(log_dict["energy_tot"]))
             log_dict["positions"] = self.vp_new.vasprun_dict["positions"]
             log_dict["forces"][:, sorted_indices] = log_dict["forces"].copy()
             log_dict["positions"][:, sorted_indices] = log_dict["positions"].copy()
-            log_dict["positions"] = np.einsum('nij,njk->nik',
-                                              log_dict["positions"],
-                                              log_dict["cells"])
+            log_dict["positions"] = np.einsum(
+                "nij,njk->nik", log_dict["positions"], log_dict["cells"]
+            )
             # log_dict["scf_energies"] = self.vp_new.vasprun_dict["scf_energies"]
             # log_dict["scf_dipole_moments"] = self.vp_new.vasprun_dict["scf_dipole_moments"]
             self.electronic_structure = self.vp_new.get_electronic_structure()
             if self.electronic_structure.grand_dos_matrix is not None:
                 self.electronic_structure.grand_dos_matrix[
                     :, :, :, sorted_indices, :
                 ] = self.electronic_structure.grand_dos_matrix[:, :, :, :, :].copy()
             if self.electronic_structure.resolved_densities is not None:
                 self.electronic_structure.resolved_densities[
                     :, sorted_indices, :, :
                 ] = self.electronic_structure.resolved_densities[:, :, :, :].copy()
             self.structure.positions = log_dict["positions"][-1]
             self.structure.set_cell(log_dict["cells"][-1])
-            self.generic_output.dft_log_dict["potentiostat_output"] = self.vp_new.get_potentiostat_output()
+            self.generic_output.dft_log_dict[
+                "potentiostat_output"
+            ] = self.vp_new.get_potentiostat_output()
+            valence_charges_orig = self.vp_new.get_valence_electrons_per_atom()
+            valence_charges = valence_charges_orig.copy()
+            valence_charges[sorted_indices] = valence_charges_orig
+            self.generic_output.dft_log_dict["valence_charges"] = valence_charges
 
         elif outcar_working:
             # log_dict = self.outcar.parse_dict.copy()
             if len(self.outcar.parse_dict["energies"]) == 0:
                 raise VaspCollectError("Error in parsing OUTCAR")
             log_dict["energy_tot"] = self.outcar.parse_dict["energies"]
             log_dict["temperature"] = self.outcar.parse_dict["temperatures"]
+            log_dict["stresses"] = self.outcar.parse_dict["stresses"]
             log_dict["pressures"] = self.outcar.parse_dict["pressures"]
             log_dict["forces"] = self.outcar.parse_dict["forces"]
             log_dict["positions"] = self.outcar.parse_dict["positions"]
             log_dict["forces"][:, sorted_indices] = log_dict["forces"].copy()
             log_dict["positions"][:, sorted_indices] = log_dict["positions"].copy()
             if len(log_dict["positions"].shape) != 3:
                 raise VaspCollectError("Improper OUTCAR parsing")
@@ -2064,17 +2178,21 @@
                 [
                     e_free[-1]
                     for e_free in self.generic_output.dft_log_dict["scf_energy_free"]
                 ]
             )
             # Overwrite energy_free with much better precision from the OSZICAR file
             if "energy_pot" in self.oszicar.parse_dict.keys():
-                if np.array_equal(self.generic_output.dft_log_dict["energy_free"],
-                                  np.round(self.oszicar.parse_dict["energy_pot"], 8)):
-                    self.generic_output.dft_log_dict["energy_free"] = self.oszicar.parse_dict["energy_pot"]
+                if np.array_equal(
+                    self.generic_output.dft_log_dict["energy_free"],
+                    np.round(self.oszicar.parse_dict["energy_pot"], 8),
+                ):
+                    self.generic_output.dft_log_dict[
+                        "energy_free"
+                    ] = self.oszicar.parse_dict["energy_pot"]
             self.generic_output.dft_log_dict["energy_zero"] = np.array(
                 [
                     e_zero[-1]
                     for e_zero in self.generic_output.dft_log_dict["scf_energy_zero"]
                 ]
             )
             self.generic_output.dft_log_dict["n_elect"] = float(
@@ -2131,15 +2249,15 @@
                 self.charge_density.to_hdf(hdf5_output, group_name="charge_density")
 
             if len(self.electronic_structure.kpoint_list) > 0:
                 self.electronic_structure.to_hdf(
                     hdf=hdf5_output, group_name="electronic_structure"
                 )
 
-            if self.outcar.parse_dict:
+            if len(self.outcar.parse_dict.keys()) > 0:
                 self.outcar.to_hdf_minimal(hdf=hdf5_output, group_name="outcar")
 
     def from_hdf(self, hdf):
         """
         Reads the attributes and reconstructs the object from a hdf file
         Args:
             hdf: The hdf5 instance
@@ -2160,15 +2278,15 @@
                         hdf5_output, group_name="charge_density"
                     )
                 if "electronic_structure" in hdf5_output.list_groups():
                     self.electronic_structure.from_hdf(hdf=hdf5_output)
                 if "outcar" in hdf5_output.list_groups():
                     self.outcar.from_hdf(hdf=hdf5_output, group_name="outcar")
             except (TypeError, IOError, ValueError):
-                s.logger.warning("Routine from_hdf() not completely successful")
+                state.logger.warning("Routine from_hdf() not completely successful")
 
 
 class GenericOutput:
     """
 
     This class stores the generic output like different structures, energies and forces from a simulation in a highly
     generic format. Usually the user does not have to access this class.
@@ -2322,15 +2440,17 @@
             table_name=table_name,
             val_only=True,
             comment_char="!",
         )
         self._path_name = None
         self._n_path = None
 
-    def set_kpoints_file(self, method=None, size_of_mesh=None, shift=None, n_path=None, path=None):
+    def set_kpoints_file(
+        self, method=None, size_of_mesh=None, shift=None, n_path=None, path=None
+    ):
         """
         Sets appropriate tags and values in the KPOINTS file
         Args:
             method (str): Type of meshing scheme (Gamma, MP, Manual or Line)
             size_of_mesh (list/numpy.ndarray): List of size 1x3 specifying the required mesh size
             shift (list): List of size 1x3 specifying the user defined shift from the Gamma point
             n_path (int): Number of points per trace for line mode
@@ -2385,36 +2505,29 @@
         """
         Store the GenericParameters in an HDF5 file
 
         Args:
             hdf (ProjectHDFio): HDF5 group object
             group_name (str): HDF5 subgroup name - optional
         """
-        super(Kpoints, self).to_hdf(
-            hdf=hdf,
-            group_name=group_name
-        )
+        super(Kpoints, self).to_hdf(hdf=hdf, group_name=group_name)
         if self._path_name is not None:
-            line_dict = {"path_name": self._path_name,
-                         "n_path": self._n_path}
+            line_dict = {"path_name": self._path_name, "n_path": self._n_path}
             with hdf.open("kpoints") as hdf_kpoints:
                 hdf_kpoints["line_dict"] = line_dict
 
     def from_hdf(self, hdf, group_name=None):
         """
         Restore the GenericParameters from an HDF5 file
 
         Args:
             hdf (ProjectHDFio): HDF5 group object
             group_name (str): HDF5 subgroup name - optional
         """
-        super(Kpoints, self).from_hdf(
-            hdf=hdf,
-            group_name=group_name
-        )
+        super(Kpoints, self).from_hdf(hdf=hdf, group_name=group_name)
         self._path_name = None
         self._n_path = None
         with hdf.open("kpoints") as hdf_kpoints:
             if "line_dict" in hdf_kpoints.list_nodes():
                 self._path_name = hdf_kpoints["line_dict"]["path_name"]
                 self._n_path = hdf_kpoints["line_dict"]["n_path"]
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/interactive.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/interactive.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,34 +53,26 @@
 
     @interactive_enforce_structure_reset.setter
     def interactive_enforce_structure_reset(self, reset):
         raise NotImplementedError(
             "interactive_enforce_structure_reset() is not implemented!"
         )
 
-    def get_structure(self, iteration_step=-1, wrap_atoms=True):
-        """
-        Gets the structure from a given iteration step of the simulation (MD/ionic relaxation). For static calculations
-        there is only one ionic iteration step
-        Args:
-            iteration_step (int): Step for which the structure is requested
-            wrap_atoms (bool): True if the atoms are to be wrapped back into the unit cell
-
-        Returns:
-            pyiron.atomistics.structure.atoms.Atoms: The required structure
-        """
+    def _get_structure(self, frame=-1, wrap_atoms=True):
         if (
             self.server.run_mode.interactive
             or self.server.run_mode.interactive_non_modal
         ):
-            structure = GenericInteractive.get_structure(self, iteration_step=iteration_step, wrap_atoms=wrap_atoms)
+            return super(GenericInteractive, self)._get_structure(
+                frame=frame, wrap_atoms=wrap_atoms
+            )
         else:
-            structure = VaspBase.get_structure(self, iteration_step=iteration_step, wrap_atoms=wrap_atoms)
-
-        return structure
+            return super(VaspBase, self)._get_structure(
+                frame=frame, wrap_atoms=wrap_atoms
+            )
 
     def interactive_close(self):
         if self.interactive_is_activated():
             with open(os.path.join(self.working_directory, "STOPCAR"), "w") as stopcar:
                 stopcar.write("LABORT = .TRUE.")  # stopcar.write('LSTOP = .TRUE.')
             try:
                 self.run_if_interactive_non_modal()
@@ -285,33 +277,55 @@
 
     def interactive_positions_setter(self, positions):
         pass
 
     def _check_incar_parameter(self, parameter, value):
         if parameter not in self.input.incar._dataset["Parameter"]:
             self.input.incar[parameter] = value
+        if parameter == "NSW":
+            self._logger.debug("setting NSW to {}".format(value))
+            self.input.incar["NSW"] = value
 
     def _interactive_check_output(self):
         while self._interactive_library.poll() is None:
             text = self._interactive_library.stdout.readline()
             if "POSITIONS: reading from stdin" in text:
                 return
 
     def _run_if_new(self, debug=False):
         if (
             self.server.run_mode.interactive
             or self.server.run_mode.interactive_non_modal
         ):
-            self._check_incar_parameter(parameter="INTERACTIVE", value=True)
-            self._check_incar_parameter(parameter="IBRION", value=-1)
-            self._check_incar_parameter(parameter="POTIM", value=0.0)
-            self._check_incar_parameter(parameter="NSW", value=1000)
-            self._check_incar_parameter(parameter="ISYM", value=0)
+            self.interactive_prepare()
         super(VaspInteractive, self)._run_if_new(debug=debug)
 
+    def interactive_prepare(self):
+        """
+        Modifies/adds tags in the INCAR file that make it possible to run VASP interactively
+        """
+        self._check_incar_parameter(parameter="INTERACTIVE", value=True)
+        self._check_incar_parameter(parameter="IBRION", value=-1)
+        self._check_incar_parameter(parameter="POTIM", value=0.0)
+        self._check_incar_parameter(parameter="NSW", value=np.iinfo(np.int32).max - 1)
+        self._check_incar_parameter(parameter="ISYM", value=0)
+
+    def convergence_check(self):
+        """
+        We don't care about convergence for interactive jobs! Always returns True
+
+        Returns:
+            bool: Always True
+
+        """
+        if self.server.run_mode.interactive:
+            return True
+        else:
+            return super().convergence_check()
+
 
 class Output(OutputBase):
     """
     Handles the output from a VASP simulation.
 
     Attributes:
         electronic_structure: Gives the electronic structure of the system
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/metadyn.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/metadyn.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,131 +55,188 @@
         The exact same tags as in the first examples are set automatically.
 
     .. _VASP documentation: https://cms.mpi.univie.ac.at/vasp/vasp/Advanced_MD_techniques.html
     """
 
     def __init__(self, project, job_name):
         super(VaspMetadyn, self).__init__(project, job_name)
-        self.__name__ = "VaspMetadyn"
+
         self.input = MetadynInput()
         self._output_parser = MetadynOutput()
-        self.supported_primitive_constraints = ["bond", "angle", "torsion", "x_pos", "y_pos", "z_pos"]
-        self.supported_complex_constraints = ["linear_combination", "norm", "coordination_number"]
+        self.supported_primitive_constraints = [
+            "bond",
+            "angle",
+            "torsion",
+            "x_pos",
+            "y_pos",
+            "z_pos",
+        ]
+        self.supported_complex_constraints = [
+            "linear_combination",
+            "norm",
+            "coordination_number",
+        ]
         self._constraint_dict = dict()
         self._complex_constraints = dict()
         # This is necessary to write the constrained dynamics output to the REPORT file
         self.input.incar["LBLUEOUT"] = True
 
-    def set_primitive_constraint(self, name, constraint_type, atom_indices, biased=False, increment=0.0):
+    def set_primitive_constraint(
+        self, name, constraint_type, atom_indices, biased=False, increment=0.0
+    ):
         """
         Function to set primitive geometric constraints  in VASP.
 
         Args:
             name (str): Name of the constraint
             constraint_type (str): Type of the constraint  (has to be part of `supported_primitive_constraints`
             atom_indices (int/list/numpy.ndarray): Indices of the atoms for which the constraint should be applied
             biased (bool): True if potential bias is to be applied (biased MD and metadynamics calculations)
             increment (float): Increment in the constraint variable at every time step
 
         """
         if self.structure is None:
-            raise ValueError("The structure has to be set before a dynamic constraint is assigned")
+            raise ValueError(
+                "The structure has to be set before a dynamic constraint is assigned"
+            )
         self._constraint_dict[name] = dict()
         if constraint_type in self.supported_primitive_constraints:
             self._constraint_dict[name]["constraint_type"] = constraint_type
         else:
-            raise ValueError("The constraint type '{}' is not supported".format(constraint_type))
+            raise ValueError(
+                "The constraint type '{}' is not supported".format(constraint_type)
+            )
         self._constraint_dict[name]["atom_indices"] = atom_indices
         self._constraint_dict[name]["biased"] = biased
         self._constraint_dict[name]["increment"] = increment
 
-    def _set_primitive_constraint_iconst(self, constraint_type, atom_indices, biased=False):
+    def _set_primitive_constraint_iconst(
+        self, constraint_type, atom_indices, biased=False
+    ):
         if self.structure is None:
-            raise ValueError("The structure has to be set before a dynamic constraint is assigned")
-        constraint_dict = {"bond": "R", "angle": "A", "torsion": "T",
-                           "x_pos": "X", "y_pos": "Y", "z_pos": "Z"}
+            raise ValueError(
+                "The structure has to be set before a dynamic constraint is assigned"
+            )
+        constraint_dict = {
+            "bond": "R",
+            "angle": "A",
+            "torsion": "T",
+            "x_pos": "X",
+            "y_pos": "Y",
+            "z_pos": "Z",
+        }
         if constraint_type not in list(constraint_dict.keys()):
             raise ValueError("Use a compatible constraint type")
         line = len(self.input.iconst._dataset["Value"])
         status = 0
         if biased:
             status = 7
         if constraint_type in ["x_pos", "y_pos", "z_pos"]:
             if isinstance(atom_indices, (list, np.ndarray)):
                 a_ind = str(self.sorted_indices[atom_indices[0]] + 1)
             else:
                 a_ind = str(self.sorted_indices[atom_indices] + 1)
         elif constraint_type in ["bond"]:
             if len(atom_indices) != 2:
-                raise ValueError("For this constraint the atom_indices must be a list or numpy array with 2 values")
-            a_ind = ' '.join(map(str, self.sorted_indices[atom_indices] + 1))
+                raise ValueError(
+                    "For this constraint the atom_indices must be a list or numpy array with 2 values"
+                )
+            a_ind = " ".join(map(str, self.sorted_indices[atom_indices] + 1))
         elif constraint_type in ["angle"]:
             if len(atom_indices) != 3:
-                raise ValueError("For this constraint the atom_indices must be a list or numpy array with 3 values")
-            a_ind = ' '.join(map(str, self.sorted_indices[atom_indices] + 1))
+                raise ValueError(
+                    "For this constraint the atom_indices must be a list or numpy array with 3 values"
+                )
+            a_ind = " ".join(map(str, self.sorted_indices[atom_indices] + 1))
         else:
-            raise ValueError("The constraint {} is not implemented!".format(constraint_type))
-        constraint_string = "{} {} {}".format(constraint_dict[constraint_type], a_ind, status)
+            raise ValueError(
+                "The constraint {} is not implemented!".format(constraint_type)
+            )
+        constraint_string = "{} {} {}".format(
+            constraint_dict[constraint_type], a_ind, status
+        )
         self.input.iconst.set_value(line, constraint_string)
 
-    def set_complex_constraint(self, name, constraint_type, coefficient_dict, biased=False, increment=0.0):
+    def set_complex_constraint(
+        self, name, constraint_type, coefficient_dict, biased=False, increment=0.0
+    ):
         """
         Set complex constraints based on defined primitive constraints.
 
         Args:
             name (str): Name of the complex constraint
             constraint_type (str): Type of the constraint  (has to be part of `supported_complex_constraints`
             coefficient_dict (dict): Dictionary containing the primitive constraint name as the key and the
                                      constraint coefficient as the values
             biased (bool): True if potential bias is to be applied (biased MD and metadynamics calculations)
             increment (float): Increment in the constraint variable at every time step
 
         """
         if self.structure is None:
-            raise ValueError("The structure has to be set before a dynamic constraint is assigned")
+            raise ValueError(
+                "The structure has to be set before a dynamic constraint is assigned"
+            )
         if constraint_type not in self.supported_complex_constraints:
             raise ValueError("Use a compatible complex constraint type")
         self._complex_constraints[name] = dict()
         self._complex_constraints[name]["constraint_type"] = constraint_type
-        if len(list(coefficient_dict.keys())) != len(list(self._constraint_dict.keys())):
-            raise ValueError("The number of coefficients should match the number of primitive contstraints")
+        if len(list(coefficient_dict.keys())) != len(
+            list(self._constraint_dict.keys())
+        ):
+            raise ValueError(
+                "The number of coefficients should match the number of primitive contstraints"
+            )
         self._complex_constraints[name]["coefficient_dict"] = coefficient_dict
         self._complex_constraints[name]["biased"] = biased
         self._complex_constraints[name]["increment"] = increment
 
     def _set_complex_constraint(self, constraint_type, coefficients, biased=False):
-        constraint_dict = {"linear_combination": "S", "norm": "C", "coordination_number": "D"}
+        constraint_dict = {
+            "linear_combination": "S",
+            "norm": "C",
+            "coordination_number": "D",
+        }
         if constraint_type not in list(constraint_dict.keys()):
             raise ValueError("Use a compatible constraint type")
         status = 0
         if biased:
             status = 5
         coeffs = " ".join(map(str, coefficients))
-        constraint_string = "{} {} {}".format(constraint_dict[constraint_type], coeffs, status)
+        constraint_string = "{} {} {}".format(
+            constraint_dict[constraint_type], coeffs, status
+        )
         line = len(self.input.iconst._dataset["Value"])
         self.input.iconst.set_value(line, constraint_string)
 
     def write_constraints(self):
         """
         Function to write constraint parameters in the INCAR and ICONST files
         """
         increment_list = list()
         linear_constraint_order = list()
         # Clear the existing ICONST file
         self.input.iconst.clear_all()
         for key, constraint in self._constraint_dict.items():
             linear_constraint_order.append(key)
-            self._set_primitive_constraint_iconst(constraint_type=constraint["constraint_type"],
-                                                  atom_indices=constraint["atom_indices"], biased=constraint["biased"])
+            self._set_primitive_constraint_iconst(
+                constraint_type=constraint["constraint_type"],
+                atom_indices=constraint["atom_indices"],
+                biased=constraint["biased"],
+            )
             increment_list.append(constraint["increment"])
 
         for constraint in self._complex_constraints.values():
-            coefficients = [constraint["coefficient_dict"][val] for val in linear_constraint_order]
-            self._set_complex_constraint(constraint_type=constraint["constraint_type"],
-                                         coefficients=coefficients, biased=constraint["biased"])
+            coefficients = [
+                constraint["coefficient_dict"][val] for val in linear_constraint_order
+            ]
+            self._set_complex_constraint(
+                constraint_type=constraint["constraint_type"],
+                coefficients=coefficients,
+                biased=constraint["biased"],
+            )
             increment_list.append(constraint["increment"])
         self.input.incar["INCREM"] = " ".join(map(str, increment_list))
 
     def write_input(self):
         """
         Call routines that generate the INCAR, POTCAR, KPOINTS and POSCAR input files
         """
@@ -195,20 +252,25 @@
     def from_hdf(self, hdf=None, group_name=None):
         super(VaspMetadyn, self).from_hdf(hdf=hdf, group_name=group_name)
         self._constraint_dict = self.input._constraint_dict
         self._complex_constraints = self.input._complex_constraints
 
 
 class MetadynInput(Input):
-
     def __init__(self):
         super(MetadynInput, self).__init__()
-        self.iconst = GenericParameters(input_file_name=None, table_name="iconst", val_only=True, comment_char="!")
-        self.penaltypot = GenericParameters(input_file_name=None, table_name="penaltypot", val_only=True,
-                                            comment_char="!")
+        self.iconst = GenericParameters(
+            input_file_name=None, table_name="iconst", val_only=True, comment_char="!"
+        )
+        self.penaltypot = GenericParameters(
+            input_file_name=None,
+            table_name="penaltypot",
+            val_only=True,
+            comment_char="!",
+        )
         self._constraint_dict = dict()
         self._complex_constraints = dict()
 
     def write(self, structure, modified_elements, directory=None):
         """
         Writes all the input files to a specified directory
 
@@ -237,21 +299,22 @@
             if "constraint_dict" in hdf5_input.list_nodes():
                 self._constraint_dict = hdf5_input["constraint_dict"]
             if "complex_constraint_dict" in hdf5_input.list_nodes():
                 self._complex_constraints = hdf5_input["complex_constraint_dict"]
 
 
 class MetadynOutput(Output):
-
     def __init__(self):
         super(MetadynOutput, self).__init__()
         self.report_file = Report()
 
     def collect(self, directory=os.getcwd(), sorted_indices=None):
-        super(MetadynOutput, self).collect(directory=directory, sorted_indices=sorted_indices)
+        super(MetadynOutput, self).collect(
+            directory=directory, sorted_indices=sorted_indices
+        )
         files_present = os.listdir(directory)
         if "REPORT" in files_present:
             self.report_file.from_file(filename=posixpath.join(directory, "REPORT"))
 
     def to_hdf(self, hdf):
         """
         Save the object in a HDF5 file
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/oszicar.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/oszicar.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,9 +38,9 @@
     @staticmethod
     def get_energy_pot(lines):
         trigger = "F="
         energy_list = list()
         for i, line in enumerate(lines):
             line = line.strip()
             if trigger in line:
-                energy_list.append(float(lines[i-1].strip().split()[2]))
+                energy_list.append(float(lines[i - 1].strip().split()[2]))
         return np.array(energy_list)
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/outcar.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/outcar.py`

 * *Files 15% similar despite different names*

```diff
@@ -60,51 +60,75 @@
         temperatures = self.get_temperatures(filename=filename, lines=lines)
         time = self.get_time(filename=filename, lines=lines)
         fermi_level = self.get_fermi_level(filename=filename, lines=lines)
         scf_moments = self.get_dipole_moments(filename=filename, lines=lines)
         kin_energy_error = self.get_kinetic_energy_error(filename=filename, lines=lines)
         stresses = self.get_stresses(filename=filename, si_unit=False, lines=lines)
         n_elect = self.get_nelect(filename=filename, lines=lines)
-        e_fermi_list, vbm_list, cbm_list = self.get_band_properties(filename=filename, lines=lines)
+        e_fermi_list, vbm_list, cbm_list = self.get_band_properties(
+            filename=filename, lines=lines
+        )
         elastic_constants = self.get_elastic_constants(filename=filename, lines=lines)
+        energy_components = self.get_energy_components(filename=filename, lines=lines)
+        cpu_time = self.get_cpu_time(filename=filename, lines=lines)
+        user_time = self.get_user_time(filename=filename, lines=lines)
+        system_time = self.get_system_time(filename=filename, lines=lines)
+        elapsed_time = self.get_elapsed_time(filename=filename, lines=lines)
+        memory_used = self.get_memory_used(filename=filename, lines=lines)
+        vasp_version = self.get_vasp_version(filename=filename, lines=lines)
+
         try:
-            irreducible_kpoints = self.get_irreducible_kpoints(
-                filename=filename, lines=lines
-            )
+            (
+                irreducible_kpoints,
+                ir_kpt_weights,
+                plane_waves,
+            ) = self.get_irreducible_kpoints(filename=filename, lines=lines)
         except ValueError:
             print("irreducible kpoints not parsed !")
             irreducible_kpoints = None
+            ir_kpt_weights = None
+            plane_waves = None
         magnetization, final_magmom_lst = self.get_magnetization(
             filename=filename, lines=lines
         )
         broyden_mixing = self.get_broyden_mixing_mesh(filename=filename, lines=lines)
-
+        self.parse_dict["vasp_version"] = vasp_version
         self.parse_dict["energies"] = energies
         self.parse_dict["energies_int"] = energies_int
         self.parse_dict["energies_zero"] = energies_zero
         self.parse_dict["scf_energies"] = scf_energies
         self.parse_dict["forces"] = forces
         self.parse_dict["positions"] = positions
         self.parse_dict["cells"] = cells
         self.parse_dict["steps"] = steps
         self.parse_dict["temperatures"] = temperatures
         self.parse_dict["time"] = time
         self.parse_dict["fermi_level"] = fermi_level
         self.parse_dict["scf_dipole_moments"] = scf_moments
         self.parse_dict["kin_energy_error"] = kin_energy_error
-        self.parse_dict["stresses"] = stresses
+        self.parse_dict["stresses"] = stresses * KBAR_TO_EVA
         self.parse_dict["irreducible_kpoints"] = irreducible_kpoints
+        self.parse_dict["irreducible_kpoint_weights"] = ir_kpt_weights
+        self.parse_dict["number_plane_waves"] = plane_waves
         self.parse_dict["magnetization"] = magnetization
         self.parse_dict["final_magmoms"] = final_magmom_lst
         self.parse_dict["broyden_mixing"] = broyden_mixing
         self.parse_dict["n_elect"] = n_elect
         self.parse_dict["e_fermi_list"] = e_fermi_list
         self.parse_dict["vbm_list"] = vbm_list
         self.parse_dict["cbm_list"] = cbm_list
         self.parse_dict["elastic_constants"] = elastic_constants
+        self.parse_dict["energy_components"] = energy_components
+        self.parse_dict["resources"] = {
+            "cpu_time": cpu_time,
+            "user_time": user_time,
+            "system_time": system_time,
+            "elapsed_time": elapsed_time,
+            "memory_used": memory_used,
+        }
         try:
             self.parse_dict["pressures"] = (
                 np.average(stresses[:, 0:3], axis=1) * KBAR_TO_EVA
             )
         except IndexError:
             self.parse_dict["pressures"] = np.zeros(len(steps))
 
@@ -129,14 +153,18 @@
             group_name (str): Name of the HDF5 group
         """
         unique_quantities = [
             "kin_energy_error",
             "broyden_mixing",
             "stresses",
             "irreducible_kpoints",
+            "irreducible_kpoint_weights",
+            "number_plane_waves",
+            "energy_components",
+            "resources",
         ]
         with hdf.open(group_name) as hdf5_output:
             for key in self.parse_dict.keys():
                 if key in unique_quantities:
                     hdf5_output[key] = self.parse_dict[key]
 
     def from_hdf(self, hdf, group_name="outcar"):
@@ -147,14 +175,17 @@
             hdf (pyiron_base.generic.hdfio.FileHDFio): HDF5 group or file
             group_name (str): Name of the HDF5 group
         """
         with hdf.open(group_name) as hdf5_output:
             for key in hdf5_output.list_nodes():
                 self.parse_dict[key] = hdf5_output[key]
 
+    def get_vasp_version(self, filename="OUTCAR", lines=None):
+        return lines[0].lstrip().split(sep=" ")[0]
+
     def get_positions_and_forces(self, filename="OUTCAR", lines=None, n_atoms=None):
         """
         Gets the forces and positions for every ionic step from the OUTCAR file
 
         Args:
             filename (str): Filename of the OUTCAR file to parse
             lines (list/None): lines read from the file
@@ -177,15 +208,14 @@
             trigger_indices=trigger_indices,
             n_atoms=n_atoms,
             pos_flag=True,
             force_flag=True,
         )
 
     def get_positions(self, filename="OUTCAR", lines=None, n_atoms=None):
-
         """
         Gets the positions for every ionic step from the OUTCAR file
 
         Args:
             filename (str): Filename of the OUTCAR file to parse
             lines (list/None): lines read from the file
             n_atoms (int/None): number of ions in OUTCAR
@@ -268,31 +298,41 @@
 
         """
         trigger_indices, lines = _get_trigger(
             lines=lines,
             filename=filename,
             trigger="FORCE on cell =-STRESS in cart. coord.  units (eV):",
         )
-        pullay_stress_lst = []
+        stress_lst = []
         for j in trigger_indices:
+            # search for '------...' delimiters of the stress table
+            # setting a constant offset into `lines` does not work, because the number of stress contributions may vary
+            # depending on the VASP configuration (e.g. with or without van der Waals interactions)
+            jj = j
+            while set(lines[jj].strip()) != {"-"}:
+                jj += 1
+            jj += 1
+            # there's two delimiters, so search again
+            while set(lines[jj].strip()) != {"-"}:
+                jj += 1
             try:
                 if si_unit:
-                    pullay_stress_lst.append(
-                        [float(l) for l in lines[j + 13].split()[1:7]]
-                    )
+                    stress = [float(l) for l in lines[jj + 1].split()[1:7]]
                 else:
-                    pullay_stress_lst.append(
-                        [float(l) for l in lines[j + 14].split()[2:8]]
-                    )
+                    stress = [float(l) for l in lines[jj + 2].split()[2:8]]
             except ValueError:
-                if si_unit:
-                    pullay_stress_lst.append([float("NaN")] * 6)
-                else:
-                    pullay_stress_lst.append([float("NaN")] * 6)
-        return np.array(pullay_stress_lst)
+                stress = [float("NaN")] * 6
+            # VASP outputs the stresses in XX, YY, ZZ, XY, YZ, ZX order
+            #                               0,  1,  2,  3,  4,  5
+            stressm = np.diag(stress[:3])
+            stressm[0, 1] = stressm[1, 0] = stress[3]
+            stressm[1, 2] = stressm[2, 1] = stress[4]
+            stressm[0, 2] = stressm[2, 0] = stress[5]
+            stress_lst.append(stressm)
+        return np.array(stress_lst)
 
     @staticmethod
     def get_irreducible_kpoints(
         filename="OUTCAR", reciprocal=True, weight=True, planewaves=True, lines=None
     ):
         """
         Function to extract the irreducible kpoints from the OUTCAR file
@@ -335,15 +375,15 @@
                 weight_lst.append(float(line.split()[3]))
         if planewaves and trigger_plane_waves != 0:
             for line in lines[
                 trigger_plane_waves : trigger_plane_waves + number_irr_kpoints
             ]:
                 line = line.strip()
                 line = _clean_line(line)
-                planewaves_lst.append(float(line.split()[-1]))
+                planewaves_lst.append(int(line.split()[-1]))
         if weight and planewaves:
             return np.array(kpoint_lst), np.array(weight_lst), np.array(planewaves_lst)
         elif weight:
             return np.array(kpoint_lst), np.array(weight_lst)
         elif planewaves:
             return np.array(kpoint_lst), np.array(planewaves_lst)
         else:
@@ -441,29 +481,35 @@
         Args:
             filename (str): Filename of the OUTCAR file to parse
             lines (list/None): lines read from the file
 
         Returns:
             list: A list of energie for every electronic step at every ionic step
         """
-        ionic_trigger = "FREE ENERGIE OF THE ION-ELECTRON SYSTEM (eV)"
-        electronic_trigger = "free energy    TOTEN  ="
-        scf_energies = list()
-        lines = _get_lines_from_file(filename=filename, lines=lines)
-        istep_energies = list()
-        for i, line in enumerate(lines):
-            line = line.strip()
-            if ionic_trigger in line:
-                scf_energies.append(np.array(istep_energies))
-                istep_energies = list()
-            if electronic_trigger in line:
-                line = _clean_line(line)
-                ene = float(line.split()[-2])
-                istep_energies.append(ene)
-        return scf_energies
+        ind_ionic_lst, lines = _get_trigger(
+            trigger="FREE ENERGIE OF THE ION-ELECTRON SYSTEM (eV)",
+            filename=filename,
+            lines=lines,
+            return_lines=True,
+        )
+        ind_elec_lst = _get_trigger(
+            trigger="free energy    TOTEN  =",
+            filename=None,
+            lines=lines,
+            return_lines=False,
+        )
+        ind_combo_lst = _split_indices(
+            ind_ionic_lst=ind_ionic_lst, ind_elec_lst=ind_elec_lst
+        )
+        return [
+            np.array(
+                [float(_clean_line(lines[ind].strip()).split()[-2]) for ind in ind_lst]
+            )
+            for ind_lst in ind_combo_lst
+        ]
 
     @staticmethod
     def get_magnetization(filename="OUTCAR", lines=None):
         """
         Gets the magnetization
 
         Args:
@@ -611,52 +657,51 @@
         Args:
             filename (str): Filename of the OUTCAR file to parse
             lines (list/None): lines read from the file
 
         Returns:
             numpy.ndarray: Steps during the simulation
         """
-        nblock_trigger = "NBLOCK ="
+        nblock_regex = re.compile(r"NBLOCK =\s+(\d+);")
         trigger = "FREE ENERGIE OF THE ION-ELECTRON SYSTEM (eV)"
-        trigger_indices = list()
-        read_nblock = True
-        n_block = 1
+        steps = 0
+        nblock = None
         lines = _get_lines_from_file(filename=filename, lines=lines)
-        for i, line in enumerate(lines):
-            line = line.strip()
+        for line in lines:
             if trigger in line:
-                trigger_indices.append(i)
-            if read_nblock is None:
-                if nblock_trigger in line:
-                    line = _clean_line(line)
-                    n_block = int(line.split(nblock_trigger)[-1])
-        return n_block * np.linspace(0, len(trigger_indices))
+                steps += 1
+            if nblock is None and "NBLOCK" in line:
+                line = line.strip()
+                line = _clean_line(line)
+                nblock = int(nblock_regex.findall(line)[0])
+        if nblock is None:
+            nblock = 1
+        return np.arange(0, steps * nblock, nblock)
 
     def get_time(self, filename="OUTCAR", lines=None):
         """
         Time after each simulation step (for MD)
 
         Args:
             filename (str): Filename of the OUTCAR file to parse
             lines (list/None): lines read from the file
 
         Returns:
             numpy.ndarray: An array of time values in fs
 
         """
         potim_trigger = "POTIM  ="
-        read_potim = True
         potim = 1.0
         lines = _get_lines_from_file(filename=filename, lines=lines)
         for i, line in enumerate(lines):
-            line = line.strip()
-            if read_potim is None:
-                if potim_trigger in line:
-                    line = _clean_line(line)
-                    potim = float(line.split(potim_trigger)[0])
+            if potim_trigger in line:
+                line = line.strip()
+                line = _clean_line(line)
+                potim = float(line.split(potim_trigger)[1].strip().split()[0])
+                break
         return potim * self.get_steps(filename)
 
     @staticmethod
     def get_kinetic_energy_error(filename="OUTCAR", lines=None):
         """
         Get the kinetic energy error
 
@@ -755,14 +800,114 @@
         lines = _get_lines_from_file(filename=filename, lines=lines)
         for i, line in enumerate(lines):
             line = line.strip()
             if nelect_trigger in line:
                 return float(line.split()[2])
 
     @staticmethod
+    def get_cpu_time(filename="OUTCAR", lines=None):
+        """
+        Returns the total CPU time in seconds
+
+        Args:
+            filename (str): OUTCAR filename
+            lines (list/None): lines read from the file
+
+        Returns:
+            float: CPU time in seconds
+
+        """
+        nelect_trigger = "Total CPU time used (sec):"
+        lines = _get_lines_from_file(filename=filename, lines=lines)
+        for i, line in enumerate(lines):
+            line = line.strip()
+            if nelect_trigger in line:
+                return float(line.split()[-1])
+
+    @staticmethod
+    def get_user_time(filename="OUTCAR", lines=None):
+        """
+        Returns the User time in seconds
+
+        Args:
+            filename (str): OUTCAR filename
+            lines (list/None): lines read from the file
+
+        Returns:
+            float: User time in seconds
+
+        """
+        nelect_trigger = "User time (sec):"
+        lines = _get_lines_from_file(filename=filename, lines=lines)
+        for i, line in enumerate(lines):
+            line = line.strip()
+            if nelect_trigger in line:
+                return float(line.split()[-1])
+
+    @staticmethod
+    def get_system_time(filename="OUTCAR", lines=None):
+        """
+        Returns the system time in seconds
+
+        Args:
+            filename (str): OUTCAR filename
+            lines (list/None): lines read from the file
+
+        Returns:
+            float: system time in seconds
+
+        """
+        nelect_trigger = "System time (sec):"
+        lines = _get_lines_from_file(filename=filename, lines=lines)
+        for i, line in enumerate(lines):
+            line = line.strip()
+            if nelect_trigger in line:
+                return float(line.split()[-1])
+
+    @staticmethod
+    def get_elapsed_time(filename="OUTCAR", lines=None):
+        """
+        Returns the elapsed time in seconds
+
+        Args:
+            filename (str): OUTCAR filename
+            lines (list/None): lines read from the file
+
+        Returns:
+            float: elapsed time in seconds
+
+        """
+        nelect_trigger = "Elapsed time (sec):"
+        lines = _get_lines_from_file(filename=filename, lines=lines)
+        for i, line in enumerate(lines):
+            line = line.strip()
+            if nelect_trigger in line:
+                return float(line.split()[-1])
+
+    @staticmethod
+    def get_memory_used(filename="OUTCAR", lines=None):
+        """
+        Returns the maximum memory used during the simulation in kB
+
+        Args:
+            filename (str): OUTCAR filename
+            lines (list/None): lines read from the file
+
+        Returns:
+            float: Maximum memory used in kB
+
+        """
+        nelect_trigger = "Maximum memory used (kb):"
+        lines = _get_lines_from_file(filename=filename, lines=lines)
+        for i, line in enumerate(lines):
+            line = line.strip()
+            if nelect_trigger in line:
+                return float(line.split()[-1])
+
+    @staticmethod
     def get_number_of_atoms(filename="OUTCAR", lines=None):
         """
         Returns the number of ions in the simulation
 
         Args:
             filename (str): OUTCAR filename
             lines (list/None): lines read from the file
@@ -796,59 +941,85 @@
         for n, ind in enumerate(fermi_trigger_indices):
             if n == len(fermi_trigger_indices) - 1:
                 trigger_indices, lines_new = _get_trigger(
                     lines=lines[ind:-1], filename=filename, trigger=band_trigger
                 )
             else:
                 trigger_indices, lines_new = _get_trigger(
-                    lines=lines[ind:fermi_trigger_indices[n+1]], filename=filename, trigger=band_trigger
+                    lines=lines[ind : fermi_trigger_indices[n + 1]],
+                    filename=filename,
+                    trigger=band_trigger,
                 )
             band_data = list()
             for ind in trigger_indices:
-                if "spin component" in lines_new[ind-3]:
+                if "spin component" in lines_new[ind - 3]:
                     is_spin_polarized = True
-                for line in lines_new[ind+1:]:
+                for line in lines_new[ind + 1 :]:
                     data = line.strip().split()
+                    # This if "Fermi" bypass needs to exist because of VASP changing it's OUTCAR format after 6.1.0
+                    # In all versions prior, searching "Fermi" will only yield 2 mentions in the OUTCAR
+                    # In the new versions, a Fermi energy is printed immediately after each spin-component k-point text block:
+                    # i.e. Fermi energy: XXXXX
+                    # This breaks the (old) parser, and thus this bypass is necessary to skip this last line at each spin component block
+                    # Ugly and hacky, but parsing the OUTCAR is a ugly and hacky endeavour in general
+                    if "Fermi" in data:
+                        continue
                     if len(data) != 3:
                         break
                     band_data.append([float(d) for d in data[1:]])
             if is_spin_polarized:
-                band_data_per_spin = [np.array(band_data[0:int(len(band_data)/2)]).tolist(),
-                                      np.array(band_data[int(len(band_data)/2):]).tolist()]
+                band_data_per_spin = [
+                    np.array(band_data[0 : int(len(band_data) / 2)]).tolist(),
+                    np.array(band_data[int(len(band_data) / 2) :]).tolist(),
+                ]
             else:
                 band_data_per_spin = [band_data]
             for spin, band_data in enumerate(band_data_per_spin):
                 if spin in cbm_level_dict.keys():
                     pass
                 else:
                     cbm_level_dict[spin] = list()
                 if spin in vbm_level_dict.keys():
                     pass
                 else:
                     vbm_level_dict[spin] = list()
                 if len(band_data) > 0:
-                    band_energy, band_occ = [np.array(band_data)[:, i] for i in range(2)]
+                    band_energy, band_occ = [
+                        np.array(band_data)[:, i] for i in range(2)
+                    ]
                     args = np.argsort(band_energy)
                     band_occ = band_occ[args]
                     band_energy = band_energy[args]
                     cbm_bool = np.abs(band_occ) < 1e-6
                     if any(cbm_bool):
-                        cbm_level_dict[spin].append(band_energy[np.abs(band_occ) < 1e-6][0])
+                        cbm_level_dict[spin].append(
+                            band_energy[np.abs(band_occ) < 1e-6][0]
+                        )
                     else:
                         cbm_level_dict[spin].append(band_energy[-1])
-                    vbm_level_dict[spin].append(band_energy[np.abs(band_occ) >= 1e-6][-1])
-        return np.array(fermi_level_list), np.array([val for val
-                                                     in vbm_level_dict.values()]), np.array([val
-                                                                                             for val in
-                                                                                             cbm_level_dict.values()])
+                    # If spin channel is completely empty, setting vbm=cbm
+                    if all(cbm_bool):
+                        vbm_level_dict[spin].append(cbm_level_dict[spin][-1])
+                    else:
+                        vbm_level_dict[spin].append(band_energy[~cbm_bool][-1])
+        return (
+            np.array(fermi_level_list),
+            np.array([val for val in vbm_level_dict.values()]),
+            np.array([val for val in cbm_level_dict.values()]),
+        )
 
     @staticmethod
     def get_elastic_constants(filename="OUTCAR", lines=None):
         lines = _get_lines_from_file(filename=filename, lines=lines)
-        trigger_indices = _get_trigger(lines=lines, filename=filename, trigger="TOTAL ELASTIC MODULI (kBar)", return_lines=False)
+        trigger_indices = _get_trigger(
+            lines=lines,
+            filename=filename,
+            trigger="TOTAL ELASTIC MODULI (kBar)",
+            return_lines=False,
+        )
         if len(trigger_indices) != 1:
             return None
         else:
             start_index = trigger_indices[0] + 3
             end_index = start_index + 6
             elastic_constants = []
             for line in lines[start_index:end_index]:
@@ -915,24 +1086,85 @@
             where M is the number of time steps
 
         """
         cells = []
         try:
             for j in trigger_indices:
                 cell = []
-                for line in lines[j + 5: j + 8]:
+                for line in lines[j + 5 : j + 8]:
                     line = line.strip()
                     line = _clean_line(line)
                     cell.append([float(l) for l in line.split()[0:3]])
                 cells.append(cell)
             return np.array(cells)
         except ValueError:
             warnings.warn("Unable to parse the cells from the OUTCAR file")
             return
 
+    @staticmethod
+    def get_energy_components(filename="OUTCAR", lines=None):
+        """
+        Gets the individual components of the free energy energy for every electronic step from the OUTCAR file
+
+        alpha Z        PSCENC =        -0.19957337
+        Ewald energy   TEWEN  =       -73.03212173
+        -Hartree energ DENC   =        -0.10933240
+        -exchange      EXHF   =         0.00000000
+        -V(xc)+E(xc)   XCENC  =       -26.17018410
+        PAW double counting   =       168.82497547     -136.88269783
+        entropy T*S    EENTRO =        -0.00827174
+        eigenvalues    EBANDS =        10.35379785
+        atomic energy  EATOM  =        53.53616173
+        Solvation  Ediel_sol  =         0.00000000
+
+        Args:
+            filename (str): Filename of the OUTCAR file to parse
+            lines (list/None): lines read from the file
+        Returns:
+            numpy.ndarray: A 1xM array of the total energies in $eV$
+            where M is the number of time steps
+        """
+        ind_ionic_lst, lines = _get_trigger(
+            trigger="FREE ENERGIE OF THE ION-ELECTRON SYSTEM (eV)",
+            filename=filename,
+            lines=lines,
+            return_lines=True,
+        )
+        ind_elec_lst = _get_trigger(
+            trigger="Free energy of the ion-electron system (eV)",
+            filename=None,
+            lines=lines,
+            return_lines=False,
+        )
+        ind_combo_lst = _split_indices(
+            ind_ionic_lst=ind_ionic_lst, ind_elec_lst=ind_elec_lst
+        )
+        try:
+            return [
+                np.array(
+                    [
+                        np.hstack(
+                            [
+                                float(lines[ind + i].split()[-1])
+                                if i != 7
+                                else [
+                                    float(lines[ind_lst[-1] + 7].split()[-2]),
+                                    float(lines[ind_lst[-1] + 7].split()[-1]),
+                                ]
+                                for i in range(2, 12)
+                            ]
+                        )
+                        for ind in ind_lst
+                    ]
+                ).T
+                for ind_lst in ind_combo_lst
+            ]
+        except ValueError:
+            return []
+
 
 def _clean_line(line):
     return line.replace("-", " -")
 
 
 def _get_trigger(trigger, filename=None, lines=None, return_lines=True):
     """
@@ -950,14 +1182,34 @@
     trigger_indicies = [i for i, line in enumerate(lines) if trigger in line.strip()]
     if return_lines:
         return trigger_indicies, lines
     else:
         return trigger_indicies
 
 
+def _split_indices(ind_ionic_lst, ind_elec_lst):
+    """
+    Combine ionic pattern matches and electronic pattern matches
+
+    Args:
+        ind_ionic_lst (list): indices of lines which matched the iconic pattern
+        ind_elec_lst (list): indices of lines which matched the electronic pattern
+
+    Returns:
+        list: nested list of electronic pattern matches within an ionic pattern match
+    """
+    ind_elec_array = np.array(ind_elec_lst)
+    return [
+        ind_elec_array[(ind_elec_array < j2) & (j1 < ind_elec_array)]
+        if j1 < j2
+        else ind_elec_array[(ind_elec_array < j2)]
+        for j1, j2 in zip(np.roll(ind_ionic_lst, 1), ind_ionic_lst)
+    ]
+
+
 def _get_lines_from_file(filename, lines=None):
     """
     If lines is None read the lines from the file with the filename filename.
 
     Args:
         filename (str): file to read lines from
         lines (list/ None): list of lines
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/potential.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/potential.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,31 @@
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import os
 import posixpath
 
 import numpy as np
 import pandas
-import tables
-import warnings
-from pyiron_base import GenericParameters, Settings, deprecate
-from pyiron_atomistics.atomistics.job.potentials import PotentialAbstract, find_potential_file_base
+from pyiron_base import state, GenericParameters, deprecate
+from pyiron_atomistics.atomistics.job.potentials import (
+    PotentialAbstract,
+    find_potential_file_base,
+)
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "development"
 __date__ = "Sep 1, 2017"
 
-s = Settings()
-
 
 class VaspPotentialAbstract(PotentialAbstract):
     """
 
     Args:
         potential_df:
         default_df:
@@ -119,15 +118,15 @@
         if len(df) != 0:
             return list(self.list()["Name"])
         else:
             return []
 
     @staticmethod
     def _return_potential_file(file_name):
-        for resource_path in s.resource_paths:
+        for resource_path in state.settings.resource_paths:
             resource_path_potcar = os.path.join(
                 resource_path, "vasp", "potentials", file_name
             )
             if os.path.exists(resource_path_potcar):
                 return resource_path_potcar
         return None
 
@@ -200,28 +199,31 @@
         Adding a new user defined element with a different POTCAR file. It is assumed that the file exists
 
         Args:
             parent_element (str): Parent element
             new_element (str): Name of the new element (the name of the folder where the new POTCAR file exists
 
         """
-        ds = self.find_default(element=parent_element)
-        ds["Species"].values[0][0] = new_element
-        path_list = ds["Filename"].values[0][0].split("/")
+        df = self.find_default(element=parent_element)
+        df["Species"].values[0][0] = new_element
+        path_list = df["Filename"].values[0][0].split("/")
         path_list[-2] = new_element
-        name_list = ds["Name"].values[0].split("-")
+        name_list = df["Name"].values[0].split("-")
         name_list[0] = new_element
-        ds["Name"].values[0] = "-".join(name_list)
-        ds["Filename"].values[0][0] = "/".join(path_list)
-        self._potential_df = self._potential_df.append(ds)
+        df["Name"].values[0] = "-".join(name_list)
+        df["Filename"].values[0][0] = "/".join(path_list)
+        self._potential_df = pandas.concat([self._potential_df, df])
         if new_element not in self._default_df.index.values:
-            ds = pandas.Series()
-            ds.name = new_element
-            ds["Name"] = "-".join(name_list)
-            self._default_df = self._default_df.append(ds)
+            ds = pandas.Series(
+                ["-".join(name_list), "/".join(path_list)],
+                index=["Name", "Filename"],
+                dtype=str,
+                name=new_element,
+            )
+            self._default_df = pandas.concat([self._default_df, ds.to_frame().T])
         else:
             self._default_df.loc[new_element] = "-".join(name_list)
 
 
 class VaspPotential(object):
     """
     The Potential class is derived from the PotentialAbstract class, but instead of loading the potentials from a list,
@@ -264,20 +266,22 @@
     def __repr__(self):
         return self._potential_dict.__repr__()
 
 
 def find_potential_file(path):
     return find_potential_file_base(
         path=path,
-        resource_path_lst=s.resource_paths,
-        rel_path=os.path.join("vasp", "potentials")
+        resource_path_lst=state.settings.resource_paths,
+        rel_path=os.path.join("vasp", "potentials"),
     )
 
 
-@deprecate("use get_enmax_among_potentials and note the adjustment to the signature (*args instead of list)")
+@deprecate(
+    "use get_enmax_among_potentials and note the adjustment to the signature (*args instead of list)"
+)
 def get_enmax_among_species(symbol_lst, return_list=False, xc="PBE"):
     """
     DEPRECATED: Please use `get_enmax_among_potentials`.
 
     Given a list of species symbols, finds the largest applicable encut.
 
     Args:
@@ -307,28 +311,36 @@
         xc ("GGA"/"PBE"/"LDA"): The exchange correlation functional for which the POTCARs were generated.
             (Default is "PBE".)
 
     Returns:
         (float): The largest ENMAX among the POTCAR files for all the requested names.
         [optional](list): The ENMAX value corresponding to each species.
     """
+
     def _get_just_element_from_name(name):
-        return name.split('_')[0]
+        return name.split("_")[0]
 
     def _get_index_of_exact_match(name, potential_names):
         try:
-            return np.argwhere([name == strip_xc_from_potential_name(pn) for pn in potential_names])[0, 0]
+            return np.argwhere(
+                [name == strip_xc_from_potential_name(pn) for pn in potential_names]
+            )[0, 0]
         except IndexError:
-            raise ValueError("Couldn't find {} among potential names for {}".format(name,
-                                                                                    _get_just_element_from_name(name)))
+            raise ValueError(
+                "Couldn't find {} among potential names for {}".format(
+                    name, _get_just_element_from_name(name)
+                )
+            )
 
     def _get_potcar_filename(name, exch_corr):
-        potcar_table = VaspPotentialFile(xc=exch_corr).find(_get_just_element_from_name(name))
-        return potcar_table['Filename'].values[
-            _get_index_of_exact_match(name, potcar_table['Name'].values)
+        potcar_table = VaspPotentialFile(xc=exch_corr).find(
+            _get_just_element_from_name(name)
+        )
+        return potcar_table["Filename"].values[
+            _get_index_of_exact_match(name, potcar_table["Name"].values)
         ][0]
 
     enmax_lst = []
     for n in names:
         with open(find_potential_file(path=_get_potcar_filename(n, xc))) as pf:
             for i, line in enumerate(pf):
                 if i == 14:
@@ -339,15 +351,15 @@
     if return_list:
         return max(enmax_lst), enmax_lst
     else:
         return max(enmax_lst)
 
 
 def strip_xc_from_potential_name(name):
-    return name.split('-')[0]
+    return name.split("-")[0]
 
 
 class Potcar(GenericParameters):
     pot_path_dict = {"GGA": "paw-gga-pbe", "PBE": "paw-gga-pbe", "LDA": "paw-lda"}
 
     def __init__(self, input_file_name=None, table_name="potcar"):
         GenericParameters.__init__(
@@ -359,14 +371,21 @@
         )
         self._structure = None
         self.electrons_per_atom_lst = list()
         self.max_cutoff_lst = list()
         self.el_path_lst = list()
         self.el_path_dict = dict()
         self.modified_elements = dict()
+        self._vasp_potentials = None
+
+    @property
+    def vasp_potentials(self):
+        if self._vasp_potentials is None:
+            self._vasp_potentials = VaspPotentialFile(self.get("xc"))
+        return self._vasp_potentials
 
     def potcar_set_structure(self, structure, modified_elements):
         self._structure = structure
         self._set_default_path_dict()
         self._set_potential_paths()
         self.modified_elements = modified_elements
 
@@ -379,79 +398,74 @@
         GenericParameters.modify(self, **modify)
         if self._structure is not None:
             self._set_potential_paths()
 
     def _set_default_path_dict(self):
         if self._structure is None:
             return
-        vasp_potentials = VaspPotentialFile(xc=self.get("xc"))
         for i, el_obj in enumerate(self._structure.get_species_objects()):
             if isinstance(el_obj.Parent, str):
                 el = el_obj.Parent
             else:
                 el = el_obj.Abbreviation
             if isinstance(el_obj.tags, dict):
                 if "pseudo_potcar_file" in el_obj.tags.keys():
                     new_element = el_obj.tags["pseudo_potcar_file"]
-                    vasp_potentials.add_new_element(
+                    self.vasp_potentials.add_new_element(
                         parent_element=el, new_element=new_element
                     )
-            key = vasp_potentials.find_default(el).Species.values[0][0]
-            val = vasp_potentials.find_default(el).Name.values[0]
+            key = self.vasp_potentials.find_default(el).Species.values[0][0]
+            val = self.vasp_potentials.find_default(el).Name.values[0]
             self[key] = val
 
     def _set_potential_paths(self):
         element_list = (
             self._structure.get_species_symbols()
         )  # .ElementList.getSpecies()
         object_list = self._structure.get_species_objects()
-        s.logger.debug("element list: {0}".format(element_list))
+        state.logger.debug("element list: {0}".format(element_list))
         self.el_path_lst = list()
-        try:
-            xc = self.get("xc")
-        except tables.exceptions.NoSuchNodeError:
-            xc = self.get("xc")
-        s.logger.debug("XC: {0}".format(xc))
-        vasp_potentials = VaspPotentialFile(xc=xc)
+        xc = self.get("xc")
+        state.logger.debug("XC: {0}".format(xc))
         for i, el_obj in enumerate(object_list):
             if isinstance(el_obj.Parent, str):
                 el = el_obj.Parent
             else:
                 el = el_obj.Abbreviation
             if (
                 isinstance(el_obj.tags, dict)
                 and "pseudo_potcar_file" in el_obj.tags.keys()
             ):
                 new_element = el_obj.tags["pseudo_potcar_file"]
-                vasp_potentials.add_new_element(
+                self.vasp_potentials.add_new_element(
                     parent_element=el, new_element=new_element
                 )
                 el_path = find_potential_file(
-                    path=vasp_potentials.find_default(new_element)["Filename"].values[
-                        0
-                    ][0]
+                    path=self.vasp_potentials.find_default(new_element)[
+                        "Filename"
+                    ].values[0][0]
                 )
                 if not (os.path.isfile(el_path)):
                     raise ValueError("such a file does not exist in the pp directory")
             elif el in self.modified_elements.keys():
                 new_element = self.modified_elements[el]
                 if os.path.isabs(new_element):
                     el_path = new_element
                 else:
-                    vasp_potentials.add_new_element(
+                    self.vasp_potentials.add_new_element(
                         parent_element=el, new_element=new_element
                     )
                     el_path = find_potential_file(
-                        path=vasp_potentials.find_default(new_element)["Filename"].values[
-                            0
-                        ][0]
+                        path=self.vasp_potentials.find_default(new_element)[
+                            "Filename"
+                        ].values[0][0]
                     )
             else:
                 el_path = find_potential_file(
-                    path=vasp_potentials.find_default(el)["Filename"].values[0][0]
+                    path=self.vasp_potentials.find_default(el)["Filename"].values[0][0]
                 )
 
             if not (os.path.isfile(el_path)):
                 raise AssertionError()
             pot_name = "pot_" + str(i)
 
             if pot_name in self._dataset["Parameter"]:
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/procar.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/procar.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,17 +50,19 @@
 
                     if band_trigger in line.split():
                         eigenvalue, occupancy = self._get_band_details(line)
                         es_obj.kpoints[-1].add_band(
                             eigenvalue=eigenvalue, occupancy=occupancy
                         )
                         band_obj = es_obj.kpoints[-1].bands[-1]
-                        band_obj.resolved_dos_matrix, band_obj.orbital_resolved_dos, band_obj.atom_resolved_dos = self._get_dos_matrix(
-                            lines[i + 2 : i + num_atoms + 4]
-                        )
+                        (
+                            band_obj.resolved_dos_matrix,
+                            band_obj.orbital_resolved_dos,
+                            band_obj.atom_resolved_dos,
+                        ) = self._get_dos_matrix(lines[i + 2 : i + num_atoms + 4])
         return es_obj
 
     @staticmethod
     def _check_if_spin_polarized(line):
         pass
 
     @staticmethod
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/report.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/report.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,17 +30,21 @@
         Reads values from files and stores it in the `parse_dict` attribute
 
         Args:
             filename (str): Path to the file that needs to be parsed
         """
         with open(filename, "r") as f:
             lines = f.readlines()
-        rel_lines = [lines[i + 2] for i, line in enumerate(lines) if "Blue_moon" in line]
+        rel_lines = [
+            lines[i + 2] for i, line in enumerate(lines) if "Blue_moon" in line
+        ]
         if len(rel_lines) > 0:
-            [lam, _, _, _] = [val for val in np.genfromtxt(rel_lines, usecols=[1, 2, 3, 4]).T]
+            [lam, _, _, _] = [
+                val for val in np.genfromtxt(rel_lines, usecols=[1, 2, 3, 4]).T
+            ]
             rel_lines = [lines[i] for i, line in enumerate(lines) if "cc>" in line]
             cv = np.genfromtxt(rel_lines, usecols=[2])
             fe = cumtrapz(lam, cv)
             self.parse_dict["cv_full"] = cv
             self.parse_dict["derivative"] = lam
             self.parse_dict["cv"] = cv[:-1]
             self.parse_dict["free_energy"] = fe
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/structure.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,16 @@
         pyiron.atomistics.structure.atoms.Atoms: The generated structure object
 
     """
     directory = "/".join(filename.split("/")[0:-1])
     potcar_file = "/".join([directory, "POTCAR"])
     if (species_list is None) and species_from_potcar:
         species_list = get_species_list_from_potcar(potcar_file)
+        if len(species_list) == 0:
+            warnings.warn("Warning! Unable to read species information from POTCAR")
     file_string = list()
     with open(filename) as f:
         for line in f:
             line = line.strip()
             file_string.append(line)
     return atoms_from_string(
         file_string, read_velocities=return_velocities, species_list=species_list
@@ -100,14 +102,15 @@
         if write_species:
             f.write(" ".join(atom_numbers.keys()) + endline)
         num_str = [str(val) for val in atom_numbers.values()]
         f.write(" ".join(num_str))
         f.write(endline)
         if "selective_dynamics" in structure.get_tags():
             selec_dyn = True
+            cartesian = False
             f.write("Selective dynamics" + endline)
         sorted_coords = list()
         selec_dyn_lst = list()
         for species in atom_numbers.keys():
             indices = structure.select_index(species)
             for i in indices:
                 if cartesian:
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/vasp.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/vasp.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,12 +45,12 @@
         >>> ham.set_kpoints(mesh=[6, 6, 6])
         The exact same tags as in the first examples are set automatically.
 
     """
 
     def __init__(self, project, job_name):
         super(Vasp, self).__init__(project, job_name)
-        self.__name__ = "Vasp"
+
         self.__version__ = (
-            None
-        )  # Reset the version number to the executable is set automatically
+            None  # Reset the version number to the executable is set automatically
+        )
         self._executable_activate(enforce=True)
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/vasprun.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/vasprun.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 # import xml.etree.cElementTree as ETree
 import numpy as np
 from collections import OrderedDict
 from pyiron_atomistics.atomistics.structure.atoms import Atoms
 from pyiron_atomistics.atomistics.structure.periodic_table import PeriodicTable
-from pyiron_base import Settings
+from pyiron_base import state
 from pyiron_atomistics.dft.waves.electronic import ElectronicStructure
 import defusedxml.cElementTree as ETree
 from defusedxml.ElementTree import ParseError
 import warnings
 
 
 __author__ = "Sudarsan Surendralal"
@@ -43,68 +43,65 @@
                 'cell' (numpy.ndarray): Mx3x3 array containing all the size and shape of cells at every iteration point
                 'forces' (numpy.ndarray): MxNx3 array containing all the forces in eV/A
                 'total_energies' (numpy.ndarray): 1xM array containing all the total energies in eV
     """
 
     def __init__(self):
         self.vasprun_dict = dict()
-        self.root = None
 
     def from_file(self, filename="vasprun.xml"):
         """
         Parsing vasprun.xml from the working directory
 
         Args:
             filename (str): Path to the vasprun file
         """
         if not (os.path.isfile(filename)):
             raise AssertionError()
         try:
-            self.root = ETree.parse(filename).getroot()
+            self.parse_root_to_dict(filename)
         except ParseError:
             raise VasprunError(
                 "The vasprun.xml file is either corrupted or the simulation has failed"
             )
 
-        self.parse_root_to_dict()
-
-    def parse_root_to_dict(self):
+    def parse_root_to_dict(self, filename):
         """
         Parses from the main xml root.
         """
-        node = self.root
         d = self.vasprun_dict
         d["scf_energies"] = list()
         d["scf_fr_energies"] = list()
         d["scf_0_energies"] = list()
         d["scf_dipole_moments"] = list()
         d["positions"] = list()
         d["cells"] = list()
         d["forces"] = list()
         d["total_energies"] = list()
         d["total_fr_energies"] = list()
         d["total_0_energies"] = list()
         d["stress_tensors"] = list()
-        for leaf in node:
+        for _, leaf in ETree.iterparse(filename):
             if leaf.tag in ["generator", "incar"]:
                 d[leaf.tag] = dict()
                 for items in leaf:
                     d[leaf.tag] = self.parse_item_to_dict(items, d[leaf.tag])
             if leaf.tag in ["kpoints"]:
                 d[leaf.tag] = dict()
                 self.parse_kpoints_to_dict(leaf, d[leaf.tag])
             if leaf.tag in ["atominfo"]:
                 d[leaf.tag] = dict()
                 self.parse_atom_information_to_dict(leaf, d[leaf.tag])
-            if leaf.tag in ["structure"] and leaf.attrib["name"] == "initialpos":
-                d["init_structure"] = dict()
-                self.parse_structure_to_dict(leaf, d["init_structure"])
-            if leaf.tag in ["structure"] and leaf.attrib["name"] == "finalpos":
-                d["final_structure"] = dict()
-                self.parse_structure_to_dict(leaf, d["final_structure"])
+            if leaf.tag in ["structure"] and "name" in leaf.keys():
+                if "initialpos" in leaf.attrib["name"]:
+                    d["init_structure"] = dict()
+                    self.parse_structure_to_dict(leaf, d["init_structure"])
+                elif "finalpos" in leaf.attrib["name"]:
+                    d["final_structure"] = dict()
+                    self.parse_structure_to_dict(leaf, d["final_structure"])
             if leaf.tag in ["calculation"]:
                 self.parse_calc_to_dict(leaf, d)
             if leaf.tag in ["parameters"]:
                 pass
                 self.parse_parameters(leaf, d)
         d["cells"] = np.array(d["cells"])
         d["positions"] = np.array(d["positions"])
@@ -214,24 +211,35 @@
                                             [elements[1].text, str(count)]
                                         )
                                         if species_key not in species_dict.keys():
                                             not_unique = False
                                         else:
                                             count += 1
                                     if species_key is not None:
-                                        pse.add_element(clean_character(elements[1].text), species_key)
+                                        pse.add_element(
+                                            clean_character(elements[1].text),
+                                            species_key,
+                                        )
                                         special_element = pse.element(species_key)
                                         species_dict[special_element] = dict()
-                                        species_dict[special_element]["n_atoms"] = int(elements[0].text)
-                                        species_dict[special_element]["valence"] = float(elements[3].text)
+                                        species_dict[special_element]["n_atoms"] = int(
+                                            elements[0].text
+                                        )
+                                        species_dict[special_element][
+                                            "valence"
+                                        ] = float(elements[3].text)
                                 else:
                                     species_key = elements[1].text
                                     species_dict[species_key] = dict()
-                                    species_dict[species_key]["n_atoms"] = int(elements[0].text)
-                                    species_dict[species_key]["valence"] = float(elements[3].text)
+                                    species_dict[species_key]["n_atoms"] = int(
+                                        elements[0].text
+                                    )
+                                    species_dict[species_key]["valence"] = float(
+                                        elements[3].text
+                                    )
         d["species_dict"] = species_dict
         species_list = list()
         for key, val in species_dict.items():
             for sp in np.tile([key], species_dict[key]["n_atoms"]):
                 species_list.append(clean_character(sp))
         d["species_list"] = species_list
 
@@ -459,19 +467,20 @@
                 self.parse_cce_to_dict(item, d)
 
         d["scf_energies"].append(scf_energies)
         d["scf_fr_energies"].append(scf_fr_energies)
         d["scf_0_energies"].append(scf_0_energies)
         d["scf_dipole_moments"].append(scf_moments)
 
-    def parse_cce_to_dict(self, node, d):
+    @staticmethod
+    def parse_cce_to_dict(node, d):
         for item in node:
-            if item.attrib['name'] not in list(d.keys()):
-                d[item.attrib['name']] = list()
-            d[item.attrib['name']].append(float(item.text))
+            if item.attrib["name"] not in list(d.keys()):
+                d[item.attrib["name"]] = list()
+            d[item.attrib["name"]].append(float(item.text))
 
     def parse_eigenvalues_to_dict(self, node, d):
         """
         Parses eigenvalue and occupancy data from a node to a dictionary
 
         Args:
             node (xml.etree.Element instance): The node to parse
@@ -651,16 +660,15 @@
                 basis.add_tag(selective_dynamics=[True, True, True])
                 for i, val in enumerate(
                     self.vasprun_dict["init_structure"]["selective_dynamics"]
                 ):
                     basis[i].selective_dynamics = val
             return basis
         except KeyError:
-            s = Settings()
-            s.logger.warning(
+            state.logger.warning(
                 "The initial structure could not be extracted from vasprun properly"
             )
             return
 
     def get_final_structure(self):
         """
         Gets the final structure from the simulation
@@ -706,26 +714,62 @@
         if "resolved_dos_matrix" in self.vasprun_dict.keys():
             es_obj.resolved_densities = self.vasprun_dict["resolved_dos_matrix"]
             es_obj.orbital_dict = self.vasprun_dict["orbital_dict"]
         es_obj.generate_from_matrices()
         return es_obj
 
     def get_potentiostat_output(self):
+        """
+        Gets the input from the vasp potentiostat output and stores it using intuitive names
+
+        Returns:
+            dict/None: Dictionary with potentiostat output
+
+        """
+        potstat_dict = dict()
         if "dftnw_pot" not in self.vasprun_dict.keys():
             return
         try:
-            vasprun_dict_keys = ["dftnw_pot", "dftnw_zval", "dftnw_electrodecharge", "dftnw_vaclevel_upperside_surf", "dftnw_vaclevel_lowerside_surf", "dftnw_efermi"]
-            potstat_dict_keys = ["potential_drop", "Ne_charge", "electrode_charge", "vac_level_upper", "vac_level_lower", "fermi_level"]
-            return {k: np.array(self.vasprun_dict[vk]) for k, vk in zip(potstat_dict_keys, vasprun_dict_keys) if vk in self.vasprun_dict.keys()}
+            vasprun_dict_keys = [
+                "dftnw_pot",
+                "dftnw_zval",
+                "dftnw_electrodecharge",
+                "dftnw_vaclevel_upperside_surf",
+                "dftnw_vaclevel_lowerside_surf",
+                "dftnw_efermi",
+            ]
+            potstat_dict_keys = [
+                "potential_drop",
+                "Ne_charge",
+                "electrode_charge",
+                "vac_level_upper",
+                "vac_level_lower",
+                "fermi_level",
+            ]
+            for k, vk in zip(potstat_dict_keys, vasprun_dict_keys):
+                if vk in self.vasprun_dict.keys():
+                    potstat_dict[k] = np.array(self.vasprun_dict[vk])
+            return potstat_dict
         except KeyError:
             if len(potstat_dict.keys()) > 0:
                 return potstat_dict
             else:
                 return
 
+    def get_valence_electrons_per_atom(self):
+        """
+        Gets the number of valence electrons for each atom in the final structure
+
+        Returns:
+            numpy.ndarray: Array of valence charges
+        """
+        sp_dict = self.vasprun_dict["atominfo"]["species_dict"]
+        return np.hstack(
+            [[val["valence"]] * val["n_atoms"] for val in sp_dict.values()]
+        )
 
 
 def clean_character(a, remove_char=" "):
     """
     Args:
         a (str): String to be cleaned
         remove_char (str): Character to be replaced
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/vaspsol.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/vaspsol.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from pyiron_atomistics.vasp.vasp import Vasp
 
 __author__ = "Jan Janssen"
-__copyright__ = "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - " \
-                "Computational Materials Design (CM) Department"
+__copyright__ = (
+    "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
+    "Computational Materials Design (CM) Department"
+)
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "development"
 __date__ = "Sep 1, 2018"
 
 
 class VaspSol(Vasp):
     def __init__(self, project, job_name):
         super(VaspSol, self).__init__(project, job_name)
-        self.__name__ = "VaspSol"
-        self.__version__ = None  # Reset the version number to the executable is set automatically
+
+        self.__version__ = (
+            None  # Reset the version number to the executable is set automatically
+        )
         self._executable = None
         self._executable_activate()
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/volumetric_data.py` & `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/volumetric_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import math
 
 import numpy as np
 import os
-from pyiron_base import Settings
-from pyiron_atomistics.vasp.structure import atoms_from_string, get_species_list_from_potcar
+from pyiron_base import state
+from pyiron_atomistics.vasp.structure import (
+    atoms_from_string,
+    get_species_list_from_potcar,
+)
 from pyiron_atomistics.atomistics.volumetric.generic import VolumetricData
 
 __author__ = "Sudarsan Surendralal"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -72,16 +75,15 @@
 
         Args:
             filename (str): Path of file to parse
             normalize (boolean): Flag to normalize by the volume of the cell
 
         """
         if os.stat(filename).st_size == 0:
-            s = Settings()
-            s.logger.warning("File:" + filename + "seems to be corrupted/empty")
+            state.logger.warning("File:" + filename + "seems to be corrupted/empty")
             return None, None
         poscar_read = False
         poscar_string = list()
         dataset = list()
         all_dataset = list()
         dim = None
         dimline = None
@@ -133,16 +135,15 @@
                     dataset = np.zeros(dim)
                 elif line == dimline:
                     read_dataset = True
                     dataset = np.zeros(dim)
             if not normalize:
                 volume = 1.0
             if len(all_dataset) == 0:
-                s = Settings()
-                s.logger.warning("File:" + filename + "seems to be corrupted/empty")
+                state.logger.warning("File:" + filename + "seems to be corrupted/empty")
                 return None, None
             if len(all_dataset) == 2:
                 data = {
                     "total": all_dataset[0] / volume,
                     "diff": all_dataset[1] / volume,
                 }
                 return atoms, [data["total"], data["diff"]]
@@ -161,16 +162,15 @@
 
         Returns:
             pyiron.atomistics.structure.atoms.Atoms: The structure of the volumetric snapshot
             list: A list of the volumetric data (length >1 for CHGCAR files with spin)
 
         """
         if not os.path.getsize(filename) > 0:
-            s = Settings()
-            s.logger.warning("File:" + filename + "seems to be empty! ")
+            state.logger.warning("File:" + filename + "seems to be empty! ")
             return None, None
         with open(filename, "r") as f:
             struct_lines = list()
             get_grid = False
             n_x = 0
             n_y = 0
             n_z = 0
@@ -218,16 +218,15 @@
                         total_data = self._fastest_index_reshape(
                             load_txt, [n_x, n_y, n_z]
                         )
                         if normalize:
                             total_data /= atoms.get_volume()
                         total_data_list.append(total_data)
             if len(total_data_list) == 0:
-                s = Settings()
-                s.logger.warning(
+                state.logger.warning(
                     "File:"
                     + filename
                     + "seems to be corrupted/empty even after parsing!"
                 )
                 return None, None
             return atoms, total_data_list
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics.egg-info/PKG-INFO` & `pyiron-atomistics-0.3.0/pyiron_atomistics.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyiron-atomistics
-Version: 0.2.9
+Version: 0.3.0
 Summary: pyiron - an integrated development environment (IDE) for computational materials science.
 Home-page: https://github.com/pyiron/pyiron_atomistics
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
-Description: http://pyiron.org
 Keywords: pyiron
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+
+http://pyiron.org
```

### Comparing `pyiron-atomistics-0.2.9/pyiron_atomistics.egg-info/SOURCES.txt` & `pyiron-atomistics-0.3.0/pyiron_atomistics.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 versioneer.py
 pyiron_atomistics/__init__.py
+pyiron_atomistics/_tests.py
 pyiron_atomistics/_version.py
 pyiron_atomistics/project.py
+pyiron_atomistics/toolkit.py
 pyiron_atomistics.egg-info/PKG-INFO
 pyiron_atomistics.egg-info/SOURCES.txt
 pyiron_atomistics.egg-info/dependency_links.txt
 pyiron_atomistics.egg-info/requires.txt
 pyiron_atomistics.egg-info/top_level.txt
 pyiron_atomistics/atomistics/__init__.py
 pyiron_atomistics/atomistics/generic/__init__.py
@@ -29,33 +31,40 @@
 pyiron_atomistics/atomistics/master/parallel.py
 pyiron_atomistics/atomistics/master/phonopy.py
 pyiron_atomistics/atomistics/master/quasi.py
 pyiron_atomistics/atomistics/master/serial.py
 pyiron_atomistics/atomistics/master/sqsmaster.py
 pyiron_atomistics/atomistics/master/structure.py
 pyiron_atomistics/atomistics/structure/__init__.py
-pyiron_atomistics/atomistics/structure/_visualize.py
 pyiron_atomistics/atomistics/structure/analyse.py
 pyiron_atomistics/atomistics/structure/atom.py
 pyiron_atomistics/atomistics/structure/atoms.py
 pyiron_atomistics/atomistics/structure/factory.py
+pyiron_atomistics/atomistics/structure/has_structure.py
 pyiron_atomistics/atomistics/structure/neighbors.py
 pyiron_atomistics/atomistics/structure/periodic_table.py
 pyiron_atomistics/atomistics/structure/phonopy.py
 pyiron_atomistics/atomistics/structure/pyironase.py
 pyiron_atomistics/atomistics/structure/pyscal.py
 pyiron_atomistics/atomistics/structure/sparse_list.py
+pyiron_atomistics/atomistics/structure/structurestorage.py
 pyiron_atomistics/atomistics/structure/factories/__init__.py
 pyiron_atomistics/atomistics/structure/factories/aimsgb.py
 pyiron_atomistics/atomistics/structure/factories/ase.py
+pyiron_atomistics/atomistics/structure/factories/atomsk.py
+pyiron_atomistics/atomistics/structure/factories/compound.py
+pyiron_atomistics/atomistics/structure/factories/materialsproject.py
 pyiron_atomistics/atomistics/thermodynamics/__init__.py
 pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py
 pyiron_atomistics/atomistics/volumetric/__init__.py
 pyiron_atomistics/atomistics/volumetric/generic.py
+pyiron_atomistics/calphy/__init__.py
+pyiron_atomistics/calphy/job.py
 pyiron_atomistics/dft/__init__.py
+pyiron_atomistics/dft/bader.py
 pyiron_atomistics/dft/job/__init__.py
 pyiron_atomistics/dft/job/generic.py
 pyiron_atomistics/dft/master/__init__.py
 pyiron_atomistics/dft/master/convergence_encut_parallel.py
 pyiron_atomistics/dft/master/convergence_encut_serial.py
 pyiron_atomistics/dft/master/convergence_kpoint_parallel.py
 pyiron_atomistics/dft/master/murnaghan_dft.py
@@ -64,29 +73,33 @@
 pyiron_atomistics/dft/waves/dos.py
 pyiron_atomistics/dft/waves/electronic.py
 pyiron_atomistics/gpaw/__init__.py
 pyiron_atomistics/gpaw/gpaw.py
 pyiron_atomistics/gpaw/pyiron_ase.py
 pyiron_atomistics/interactive/__init__.py
 pyiron_atomistics/interactive/activation_relaxation_technique.py
+pyiron_atomistics/interactive/quasi_newton.py
 pyiron_atomistics/interactive/scipy_minimizer.py
 pyiron_atomistics/interactive/sxextoptint.py
 pyiron_atomistics/lammps/__init__.py
 pyiron_atomistics/lammps/base.py
 pyiron_atomistics/lammps/control.py
 pyiron_atomistics/lammps/interactive.py
 pyiron_atomistics/lammps/lammps.py
+pyiron_atomistics/lammps/output.py
 pyiron_atomistics/lammps/potential.py
 pyiron_atomistics/lammps/structure.py
+pyiron_atomistics/lammps/units.py
 pyiron_atomistics/sphinx/__init__.py
 pyiron_atomistics/sphinx/base.py
 pyiron_atomistics/sphinx/interactive.py
 pyiron_atomistics/sphinx/potential.py
 pyiron_atomistics/sphinx/sphinx.py
 pyiron_atomistics/sphinx/structure.py
+pyiron_atomistics/sphinx/util.py
 pyiron_atomistics/sphinx/volumetric_data.py
 pyiron_atomistics/table/__init__.py
 pyiron_atomistics/table/datamining.py
 pyiron_atomistics/table/funct.py
 pyiron_atomistics/testing/__init__.py
 pyiron_atomistics/testing/executable.py
 pyiron_atomistics/testing/randomatomistic.py
@@ -103,8 +116,10 @@
 pyiron_atomistics/vasp/potential.py
 pyiron_atomistics/vasp/procar.py
 pyiron_atomistics/vasp/report.py
 pyiron_atomistics/vasp/structure.py
 pyiron_atomistics/vasp/vasp.py
 pyiron_atomistics/vasp/vasprun.py
 pyiron_atomistics/vasp/vaspsol.py
-pyiron_atomistics/vasp/volumetric_data.py
+pyiron_atomistics/vasp/volumetric_data.py
+tests/test_project.py
+tests/test_toolkit.py
```

### Comparing `pyiron-atomistics-0.2.9/setup.py` & `pyiron-atomistics-0.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,65 @@
 """
 Setuptools based setup module
 """
 from setuptools import setup, find_packages
+
 import versioneer
 
 setup(
     name='pyiron-atomistics',
     version=versioneer.get_version(),
     description='pyiron - an integrated development environment (IDE) for computational materials science.',
     long_description='http://pyiron.org',
 
     url='https://github.com/pyiron/pyiron_atomistics',
     author='Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department',
     author_email='janssen@mpie.de',
     license='BSD',
 
-    classifiers=['Development Status :: 5 - Production/Stable',
-                 'Topic :: Scientific/Engineering :: Physics',
-                 'License :: OSI Approved :: BSD License',
-                 'Intended Audience :: Science/Research',
-                 'Operating System :: OS Independent',
-                 'Programming Language :: Python :: 3',
-                 'Programming Language :: Python :: 3.6',
-                 'Programming Language :: Python :: 3.7',
-                 'Programming Language :: Python :: 3.8',
-                 'Programming Language :: Python :: 3.9'],
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Topic :: Scientific/Engineering :: Physics',
+        'License :: OSI Approved :: BSD License',
+        'Intended Audience :: Science/Research',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
+    ],
 
     keywords='pyiron',
-    packages=find_packages(exclude=["*tests*", "*docs*", "*binder*", "*conda*", "*notebooks*", "*.ci_support*"]),
+    packages=find_packages(exclude=[
+        "*tests*", 
+        "*docs*", 
+        "*binder*", 
+        "*.devcontainer*", 
+        "*notebooks*",
+        "*.ci_support*", 
+        "*test_benchmarks*", 
+        "*test_integration*", 
+        "*.github*"
+    ]),
     install_requires=[
-        'aimsgb>=0.1.0',
-        'ase>=3.21.1',
+        'ase>=3.22.1',
         'defusedxml>=0.7.1',
-        'future>=0.18.2',
-        'h5py>=3.1.0',
-        'matplotlib>=3.3.4',
-        'mendeleev>=0.7.0',
-        'numpy>=1.20.1',
-        'pandas>=1.2.3',
-        'phonopy>=2.9.3',
-        'pyiron_base>=0.2.7',
-        'pymatgen>=2022.0.5',
-        'scipy>=1.6.1',
-        'seekpath>=2.0.1',
-        'six>=1.15.0',
-        'scikit-learn>=0.24.1',
-        'spglib>=1.16.1',
-        'tables>=3.6.1'
+        'h5py>=3.8.0',
+        'matplotlib>=3.7.1',
+        'mendeleev>=0.13.1',
+        'mp-api>=0.33.3',
+        'numpy>=1.24.3',
+        'pandas>=2.0.2',
+        'phonopy>=2.19.1',
+        'pint>=0.22',
+        'pyiron_base>=0.6.0',
+        'pymatgen>=2023.5.31',
+        'scipy>=1.10.1',
+        'seekpath>=2.1.0',
+        'scikit-learn>=1.2.2',
+        'spglib>=2.0.2',
+        'structuretoolkit>=0.0.3'
     ],
     cmdclass=versioneer.get_cmdclass(),
 
     )
```

### Comparing `pyiron-atomistics-0.2.9/versioneer.py` & `pyiron-atomistics-0.3.0/versioneer.py`

 * *Files identical despite different names*

