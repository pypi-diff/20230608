# Comparing `tmp/biobb_amber-4.0.0.tar.gz` & `tmp/biobb_amber-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_amber-4.0.0.tar", last modified: Wed Apr 12 08:30:49 2023, max compression
+gzip compressed data, was "dist/biobb_amber-4.0.1.tar", last modified: Thu Jun  8 08:12:34 2023, max compression
```

## Comparing `biobb_amber-4.0.0.tar` & `biobb_amber-4.0.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11357 2022-05-26 11:32:14.000000 biobb_amber-4.0.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      882 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5315 2023-04-12 08:29:08.000000 biobb_amber-4.0.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      155 2023-04-12 08:28:56.000000 biobb_amber-4.0.0/biobb_amber/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/ambpdb/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       43 2022-05-26 11:32:14.000000 biobb_amber-4.0.0/biobb_amber/ambpdb/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7407 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/ambpdb/amber_to_pdb.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1898 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/ambpdb/common.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/cphstats/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       60 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/cphstats/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    17622 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/cphstats/cestats_run.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2327 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/cphstats/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    17574 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/cphstats/cphstats_run.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/cpptraj/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       54 2022-05-26 11:32:14.000000 biobb_amber-4.0.0/biobb_amber/cpptraj/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1968 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/cpptraj/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11027 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/cpptraj/cpptraj_randomize_ions.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/leap/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      105 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/leap/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2144 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/leap/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    26378 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/leap/leap_add_ions.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8046 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/leap/leap_build_linear_structure.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    16671 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/leap/leap_gen_top.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    21736 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/leap/leap_solvate.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/nab/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       51 2022-05-26 11:32:14.000000 biobb_amber-4.0.0/biobb_amber/nab/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1769 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/nab/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8722 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/nab/nab_build_dna_structure.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/parmed/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       73 2022-05-26 11:32:14.000000 biobb_amber-4.0.0/biobb_amber/parmed/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1887 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/parmed/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9081 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/parmed/parmed_cpinutil.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7633 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/parmed/parmed_hmassrepartition.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/pdb4amber/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       47 2022-05-26 11:32:14.000000 biobb_amber-4.0.0/biobb_amber/pdb4amber/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1810 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/pdb4amber/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7603 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/pdb4amber/pdb4amber_run.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/pmemd/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       41 2022-05-26 11:32:14.000000 biobb_amber-4.0.0/biobb_amber/pmemd/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2414 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/pmemd/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    25615 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/pmemd/pmemd_mdrun.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/process/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       63 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/process/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1841 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/process/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9046 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/process/process_mdout.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9149 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/process/process_minout.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/sander/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       43 2022-05-26 11:32:14.000000 biobb_amber-4.0.0/biobb_amber/sander/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2472 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/sander/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    29424 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/sander/sander_mdrun.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber.egg-info/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      882 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1475 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      954 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       12 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2422 2023-04-12 08:28:45.000000 biobb_amber-4.0.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11357 2022-05-26 11:32:14.000000 biobb_amber-4.0.1/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      982 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5315 2023-06-08 08:11:06.000000 biobb_amber-4.0.1/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      155 2023-06-08 08:10:46.000000 biobb_amber-4.0.1/biobb_amber/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber/ambpdb/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       43 2022-05-26 11:32:14.000000 biobb_amber-4.0.1/biobb_amber/ambpdb/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7407 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/ambpdb/amber_to_pdb.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1898 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/ambpdb/common.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber/cphstats/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       60 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/cphstats/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    17622 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/cphstats/cestats_run.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2327 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/cphstats/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    17574 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/cphstats/cphstats_run.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber/cpptraj/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       54 2022-05-26 11:32:14.000000 biobb_amber-4.0.1/biobb_amber/cpptraj/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1968 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/cpptraj/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11027 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/cpptraj/cpptraj_randomize_ions.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber/leap/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      105 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/leap/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2144 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/leap/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    26378 2023-06-08 07:37:01.000000 biobb_amber-4.0.1/biobb_amber/leap/leap_add_ions.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8046 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/leap/leap_build_linear_structure.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    16671 2023-06-08 07:49:29.000000 biobb_amber-4.0.1/biobb_amber/leap/leap_gen_top.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    21736 2023-06-08 07:49:46.000000 biobb_amber-4.0.1/biobb_amber/leap/leap_solvate.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber/nab/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       51 2022-05-26 11:32:14.000000 biobb_amber-4.0.1/biobb_amber/nab/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1769 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/nab/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8722 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/nab/nab_build_dna_structure.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber/parmed/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       73 2022-05-26 11:32:14.000000 biobb_amber-4.0.1/biobb_amber/parmed/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1887 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/parmed/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9081 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/parmed/parmed_cpinutil.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7633 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/parmed/parmed_hmassrepartition.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber/pdb4amber/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       47 2022-05-26 11:32:14.000000 biobb_amber-4.0.1/biobb_amber/pdb4amber/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1810 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/pdb4amber/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7603 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/pdb4amber/pdb4amber_run.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber/pmemd/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       41 2022-05-26 11:32:14.000000 biobb_amber-4.0.1/biobb_amber/pmemd/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2414 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/pmemd/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    25615 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/pmemd/pmemd_mdrun.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber/process/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       63 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/process/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1841 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/process/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9046 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/process/process_mdout.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9149 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/process/process_minout.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber/sander/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       43 2022-05-26 11:32:14.000000 biobb_amber-4.0.1/biobb_amber/sander/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2472 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/sander/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    29424 2023-04-12 08:27:46.000000 biobb_amber-4.0.1/biobb_amber/sander/sander_mdrun.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      982 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1475 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      954 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       12 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/biobb_amber.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-06-08 08:12:34.000000 biobb_amber-4.0.1/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2520 2023-06-08 08:10:35.000000 biobb_amber-4.0.1/setup.py
```

### Comparing `biobb_amber-4.0.0/LICENSE` & `biobb_amber-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/PKG-INFO` & `biobb_amber-4.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: biobb_amber
-Version: 4.0.0
+Version: 4.0.1
 Summary: Biobb_amber is a BioBB category for AMBER MD package.
 Home-page: https://github.com/bioexcel/biobb_amber
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_amber.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility MD Amber
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `biobb_amber-4.0.0/README.md` & `biobb_amber-4.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_amber?label=Version)](https://GitHub.com/bioexcel/biobb_amber/tags/)
 [![](https://img.shields.io/pypi/v/biobb-amber.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-amber/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_amber?label=Conda)](https://anaconda.org/bioconda/biobb_amber)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_amber?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_amber)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_amber?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_amber:4.0.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_amber:4.0.1--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_amber)
 [![](https://img.shields.io/pypi/pyversions/biobb-amber.svg?label=Python%20Versions)](https://pypi.org/project/biobb-amber/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_amber)
 
 [![](https://readthedocs.org/projects/biobb-amber/badge/?version=latest&label=Docs)](https://biobb-amber.readthedocs.io/en/latest/?badge=latest)
@@ -30,61 +30,61 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_amber.readthedocs.io/en/latest/).
 
 ### Version
-v4.0.0 2023.1
+v4.0.1 2023.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_amber>=4.0.0"
+        pip install "biobb_amber>=4.0.1"
 
 
 * Usage: [Python API documentation](https://biobb-amber.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_amber>=4.0.0"
+        conda install -c bioconda "biobb_amber>=4.0.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-amber.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-amber.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_amber:4.0.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_amber:4.0.1--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_amber:4.0.0--pyhdfd78af_0
+        docker run quay.io/biocontainers/biobb_amber:4.0.1--pyhdfd78af_0
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_amber.sif https://depot.galaxyproject.org/singularity/biobb_amber:4.0.0--pyhdfd78af_0
+        singularity pull --name biobb_amber.sif https://depot.galaxyproject.org/singularity/biobb_amber:4.0.1--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_amber.sif <command>
```

### Comparing `biobb_amber-4.0.0/biobb_amber/ambpdb/amber_to_pdb.py` & `biobb_amber-4.0.1/biobb_amber/ambpdb/amber_to_pdb.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/ambpdb/common.py` & `biobb_amber-4.0.1/biobb_amber/ambpdb/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/cphstats/cestats_run.py` & `biobb_amber-4.0.1/biobb_amber/cphstats/cestats_run.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/cphstats/common.py` & `biobb_amber-4.0.1/biobb_amber/cphstats/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/cphstats/cphstats_run.py` & `biobb_amber-4.0.1/biobb_amber/cphstats/cphstats_run.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/cpptraj/common.py` & `biobb_amber-4.0.1/biobb_amber/cpptraj/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/cpptraj/cpptraj_randomize_ions.py` & `biobb_amber-4.0.1/biobb_amber/cpptraj/cpptraj_randomize_ions.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/leap/common.py` & `biobb_amber-4.0.1/biobb_amber/leap/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/leap/leap_add_ions.py` & `biobb_amber-4.0.1/biobb_amber/leap/leap_add_ions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -209,14 +209,25 @@
             if self.negative_ions_number != 0:
                 # ions_command = ions_command + "addions mol " + self.negative_ions_type + " " + str(self.negative_ions_number) + " \n"
                 ions_command = ions_command + "addionsRand mol " + self.negative_ions_type + " " + str(self.negative_ions_number) + " \n"
             if self.positive_ions_number != 0:
                 # ions_command = ions_command + "addions mol " + self.positive_ions_type + " " + str(self.positive_ions_number) + " \n"
                 ions_command = ions_command + "addionsRand mol " + self.positive_ions_type + " " + str(self.positive_ions_number) + " \n"
 
+        # Creating temporary folder & Leap configuration (instructions) file
+        if self.container_path:
+            instructions_file = str(PurePath(self.stage_io_dict['unique_dir']).joinpath("leap.in"))
+            instructions_file_path = str(PurePath(self.container_volume_path).joinpath("leap.in"))
+            self.tmp_folder = None
+        else:
+            self.tmp_folder = fu.create_unique_dir()
+            instructions_file = str(PurePath(self.tmp_folder).joinpath("leap.in"))
+            fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
+            instructions_file_path = instructions_file
+
         ligands_lib_list = []
         if self.io_dict['in']['input_lib_path'] is not None:
             if self.io_dict['in']['input_lib_path'].endswith('.zip'):
                 ligands_lib_list = fu.unzip_list(self.stage_io_dict['in']['input_lib_path'], dest_dir=self.tmp_folder, out_log=self.out_log)
             else:
                 ligands_lib_list.append(self.stage_io_dict['in']['input_lib_path'])
 
@@ -237,25 +248,14 @@
         leap_source_list = []
         if self.io_dict['in']['input_source_path'] is not None:
             if self.io_dict['in']['input_source_path'].endswith('.zip'):
                 leap_source_list = fu.unzip_list(self.stage_io_dict['in']['input_source_path'], dest_dir=self.tmp_folder, out_log=self.out_log)
             else:
                 leap_source_list.append(self.stage_io_dict['in']['input_source_path'])
 
-        # Creating temporary folder & Leap configuration (instructions) file
-        if self.container_path:
-            instructions_file = str(PurePath(self.stage_io_dict['unique_dir']).joinpath("leap.in"))
-            instructions_file_path = str(PurePath(self.container_volume_path).joinpath("leap.in"))
-            self.tmp_folder = None
-        else:
-            self.tmp_folder = fu.create_unique_dir()
-            instructions_file = str(PurePath(self.tmp_folder).joinpath("leap.in"))
-            fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
-            instructions_file_path = instructions_file
-
         # instructions_file = str(PurePath(self.tmp_folder).joinpath("leap.in"))
         with open(instructions_file, 'w') as leapin:
             # Forcefields loaded by default:
             # Protein: ff14SB (PARM99 + frcmod.ff99SB + frcmod.parmbsc0 + OL3 for RNA)
             # leapin.write("source leaprc.protein.ff14SB \n")
             # DNA: parmBSC1 (ParmBSC1 (ff99 + bsc0 + bsc1) for DNA. Ivani et al. Nature Methods 13: 55, 2016)
             # leapin.write("source leaprc.DNA.bsc1 \n")
```

### Comparing `biobb_amber-4.0.0/biobb_amber/leap/leap_build_linear_structure.py` & `biobb_amber-4.0.1/biobb_amber/leap/leap_build_linear_structure.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/leap/leap_gen_top.py` & `biobb_amber-4.0.1/biobb_amber/leap/leap_gen_top.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,25 @@
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
         if self.check_restart():
             return 0
         self.stage_files()
 
+        # Creating temporary folder & Leap configuration (instructions) file
+        if self.container_path:
+            instructions_file = str(PurePath(self.stage_io_dict['unique_dir']).joinpath("leap.in"))
+            instructions_file_path = str(PurePath(self.container_volume_path).joinpath("leap.in"))
+            self.tmp_folder = None
+        else:
+            self.tmp_folder = fu.create_unique_dir()
+            instructions_file = str(PurePath(self.tmp_folder).joinpath("leap.in"))
+            fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
+            instructions_file_path = instructions_file
+
         ligands_lib_list = []
         if self.io_dict['in']['input_lib_path'] is not None:
             if self.io_dict['in']['input_lib_path'].endswith('.zip'):
                 ligands_lib_list = fu.unzip_list(self.stage_io_dict['in']['input_lib_path'], dest_dir=self.tmp_folder, out_log=self.out_log)
             else:
                 ligands_lib_list.append(self.stage_io_dict['in']['input_lib_path'])
 
@@ -154,25 +165,14 @@
         leap_source_list = []
         if self.io_dict['in']['input_source_path'] is not None:
             if self.io_dict['in']['input_source_path'].endswith('.zip'):
                 leap_source_list = fu.unzip_list(self.stage_io_dict['in']['input_source_path'], dest_dir=self.tmp_folder, out_log=self.out_log)
             else:
                 leap_source_list.append(self.stage_io_dict['in']['input_source_path'])
 
-        # Creating temporary folder & Leap configuration (instructions) file
-        if self.container_path:
-            instructions_file = str(PurePath(self.stage_io_dict['unique_dir']).joinpath("leap.in"))
-            instructions_file_path = str(PurePath(self.container_volume_path).joinpath("leap.in"))
-            self.tmp_folder = None
-        else:
-            self.tmp_folder = fu.create_unique_dir()
-            instructions_file = str(PurePath(self.tmp_folder).joinpath("leap.in"))
-            fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
-            instructions_file_path = instructions_file
-
         with open(instructions_file, 'w') as leapin:
             # Forcefields loaded by default:
             # Protein: ff14SB (PARM99 + frcmod.ff99SB + frcmod.parmbsc0 + OL3 for RNA)
             # leapin.write("source leaprc.protein.ff14SB \n")
             # DNA: parmBSC1 (ParmBSC1 (ff99 + bsc0 + bsc1) for DNA. Ivani et al. Nature Methods 13: 55, 2016)
             # leapin.write("source leaprc.DNA.bsc1 \n")
             # Ligands: GAFF (General Amber Force field, J. Comput. Chem. 2004 Jul 15;25(9):1157-74)
```

### Comparing `biobb_amber-4.0.0/biobb_amber/leap/leap_solvate.py` & `biobb_amber-4.0.1/biobb_amber/leap/leap_solvate.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -182,14 +182,25 @@
             ions_command = ions_command + "addions mol " + self.positive_ions_type + " 0 \n"
 
         if self.negative_ions_number != 0:
             ions_command = ions_command + "addions mol " + self.negative_ions_type + " " + str(self.negative_ions_number) + " \n"
         if self.positive_ions_number != 0:
             ions_command = ions_command + "addions mol " + self.positive_ions_type + " " + str(self.positive_ions_number) + " \n"
 
+        # Creating temporary folder & Leap configuration (instructions) file
+        if self.container_path:
+            instructions_file = str(PurePath(self.stage_io_dict['unique_dir']).joinpath("leap.in"))
+            instructions_file_path = str(PurePath(self.container_volume_path).joinpath("leap.in"))
+            self.tmp_folder = None
+        else:
+            self.tmp_folder = fu.create_unique_dir()
+            instructions_file = str(PurePath(self.tmp_folder).joinpath("leap.in"))
+            fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
+            instructions_file_path = instructions_file
+
         ligands_lib_list = []
         if self.io_dict['in']['input_lib_path'] is not None:
             if self.io_dict['in']['input_lib_path'].endswith('.zip'):
                 ligands_lib_list = fu.unzip_list(self.stage_io_dict['in']['input_lib_path'], dest_dir=self.tmp_folder, out_log=self.out_log)
             else:
                 ligands_lib_list.append(self.stage_io_dict['in']['input_lib_path'])
 
@@ -210,25 +221,14 @@
         leap_source_list = []
         if self.io_dict['in']['input_source_path'] is not None:
             if self.io_dict['in']['input_source_path'].endswith('.zip'):
                 leap_source_list = fu.unzip_list(self.stage_io_dict['in']['input_source_path'], dest_dir=self.tmp_folder, out_log=self.out_log)
             else:
                 leap_source_list.append(self.stage_io_dict['in']['input_source_path'])
 
-        # Creating temporary folder & Leap configuration (instructions) file
-        if self.container_path:
-            instructions_file = str(PurePath(self.stage_io_dict['unique_dir']).joinpath("leap.in"))
-            instructions_file_path = str(PurePath(self.container_volume_path).joinpath("leap.in"))
-            self.tmp_folder = None
-        else:
-            self.tmp_folder = fu.create_unique_dir()
-            instructions_file = str(PurePath(self.tmp_folder).joinpath("leap.in"))
-            fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
-            instructions_file_path = instructions_file
-
         with open(instructions_file, 'w') as leapin:
             # Forcefields loaded by default:
             # Protein: ff14SB (PARM99 + frcmod.ff99SB + frcmod.parmbsc0 + OL3 for RNA)
             # leapin.write("source leaprc.protein.ff14SB \n")
             # DNA: parmBSC1 (ParmBSC1 (ff99 + bsc0 + bsc1) for DNA. Ivani et al. Nature Methods 13: 55, 2016)
             # leapin.write("source leaprc.DNA.bsc1 \n")
             # Ligands: GAFF (General Amber Force field, J. Comput. Chem. 2004 Jul 15;25(9):1157-74)
```

### Comparing `biobb_amber-4.0.0/biobb_amber/nab/common.py` & `biobb_amber-4.0.1/biobb_amber/nab/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/nab/nab_build_dna_structure.py` & `biobb_amber-4.0.1/biobb_amber/nab/nab_build_dna_structure.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/parmed/common.py` & `biobb_amber-4.0.1/biobb_amber/parmed/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/parmed/parmed_cpinutil.py` & `biobb_amber-4.0.1/biobb_amber/parmed/parmed_cpinutil.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/parmed/parmed_hmassrepartition.py` & `biobb_amber-4.0.1/biobb_amber/parmed/parmed_hmassrepartition.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/pdb4amber/common.py` & `biobb_amber-4.0.1/biobb_amber/pdb4amber/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/pdb4amber/pdb4amber_run.py` & `biobb_amber-4.0.1/biobb_amber/pdb4amber/pdb4amber_run.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/pmemd/common.py` & `biobb_amber-4.0.1/biobb_amber/pmemd/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/pmemd/pmemd_mdrun.py` & `biobb_amber-4.0.1/biobb_amber/pmemd/pmemd_mdrun.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/process/common.py` & `biobb_amber-4.0.1/biobb_amber/process/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/process/process_mdout.py` & `biobb_amber-4.0.1/biobb_amber/process/process_mdout.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/process/process_minout.py` & `biobb_amber-4.0.1/biobb_amber/process/process_minout.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/sander/common.py` & `biobb_amber-4.0.1/biobb_amber/sander/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber/sander/sander_mdrun.py` & `biobb_amber-4.0.1/biobb_amber/sander/sander_mdrun.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber.egg-info/PKG-INFO` & `biobb_amber-4.0.1/biobb_amber.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: biobb-amber
-Version: 4.0.0
+Version: 4.0.1
 Summary: Biobb_amber is a BioBB category for AMBER MD package.
 Home-page: https://github.com/bioexcel/biobb_amber
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_amber.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility MD Amber
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `biobb_amber-4.0.0/biobb_amber.egg-info/SOURCES.txt` & `biobb_amber-4.0.1/biobb_amber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/biobb_amber.egg-info/entry_points.txt` & `biobb_amber-4.0.1/biobb_amber.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.0.0/setup.py` & `biobb_amber-4.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_amber",
-    version="4.0.0",
+    version="4.0.1",
     author="Biobb developers",
     author_email="adam.hospital@irbbarcelona.org",
     description="Biobb_amber is a BioBB category for AMBER MD package.",
     long_description="Biobb_amber allows setup and simulation of atomistic MD simulations using AMBER MD package and its associated AMBER tools.",
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility MD Amber",
     url="https://github.com/bioexcel/biobb_amber",
@@ -39,12 +39,14 @@
             "process_minout = biobb_amber.process.process_minout:main",
             "sander_mdrun = biobb_amber.sander.sander_mdrun:main"
         ]
     },
     classifiers=(
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX",
     ),
 )
```

