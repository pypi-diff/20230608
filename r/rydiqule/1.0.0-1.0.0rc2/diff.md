# Comparing `tmp/rydiqule-1.0.0.tar.gz` & `tmp/rydiqule-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rydiqule-1.0.0.tar", last modified: Thu Jun  8 18:26:47 2023, max compression
+gzip compressed data, was "rydiqule-1.0.0rc2.tar", last modified: Wed May 24 20:39:55 2023, max compression
```

## Comparing `rydiqule-1.0.0.tar` & `rydiqule-1.0.0rc2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:26:47.170641 rydiqule-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-06-08 18:26:30.000000 rydiqule-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-06-08 18:26:47.170641 rydiqule-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-08 18:26:30.000000 rydiqule-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 18:26:30.000000 rydiqule-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-08 18:26:47.170641 rydiqule-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 18:26:30.000000 rydiqule-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:26:47.162641 rydiqule-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:26:47.166641 rydiqule-1.0.0/src/rydiqule/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/atom_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24078 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)    15257 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/doppler_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/energy_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/rydiqule_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    74697 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/sensor_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    23386 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/sensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:26:47.166641 rydiqule-1.0.0/src/rydiqule/slicing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/slicing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/slicing/slicing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:26:47.170641 rydiqule-1.0.0/src/rydiqule/stack_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/stack_solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/stack_solvers/cyrk_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/stack_solvers/nbkode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/stack_solvers/nbrk_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/stack_solvers/scipy_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    18945 2023-06-08 18:26:30.000000 rydiqule-1.0.0/src/rydiqule/timesolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:26:47.166641 rydiqule-1.0.0/src/rydiqule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-06-08 18:26:47.000000 rydiqule-1.0.0/src/rydiqule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-08 18:26:47.000000 rydiqule-1.0.0/src/rydiqule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:26:47.000000 rydiqule-1.0.0/src/rydiqule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:26:46.000000 rydiqule-1.0.0/src/rydiqule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-08 18:26:47.000000 rydiqule-1.0.0/src/rydiqule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 18:26:47.000000 rydiqule-1.0.0/src/rydiqule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:26:47.170641 rydiqule-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-08 18:26:30.000000 rydiqule-1.0.0/tests/test_EOMs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-08 18:26:30.000000 rydiqule-1.0.0/tests/test_calculate_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-08 18:26:30.000000 rydiqule-1.0.0/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-08 18:26:30.000000 rydiqule-1.0.0/tests/test_level_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-08 18:26:30.000000 rydiqule-1.0.0/tests/test_numbakitode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-08 18:26:30.000000 rydiqule-1.0.0/tests/test_parameter_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-06-08 18:26:30.000000 rydiqule-1.0.0/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-06-08 18:26:30.000000 rydiqule-1.0.0/tests/test_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-08 18:26:30.000000 rydiqule-1.0.0/tests/test_steady_state_ham_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-06-08 18:26:30.000000 rydiqule-1.0.0/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-08 18:26:30.000000 rydiqule-1.0.0/tests/test_time_cyrk.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-08 18:26:30.000000 rydiqule-1.0.0/tests/test_time_ham_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-06-08 18:26:30.000000 rydiqule-1.0.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:39:55.035320 rydiqule-1.0.0rc2/
+-rw-rw-rw-   0        0        0    11584 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/LICENSE
+-rw-rw-rw-   0        0        0     5535 2023-05-24 20:39:55.035320 rydiqule-1.0.0rc2/PKG-INFO
+-rw-rw-rw-   0        0        0     4784 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/README.md
+-rw-rw-rw-   0        0        0       91 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/pyproject.toml
+-rw-rw-rw-   0        0        0     1197 2023-05-24 20:39:55.035320 rydiqule-1.0.0rc2/setup.cfg
+-rw-rw-rw-   0        0        0      100 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:39:54.457389 rydiqule-1.0.0rc2/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 20:39:54.676030 rydiqule-1.0.0rc2/src/rydiqule/
+-rw-rw-rw-   0        0        0      816 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/__init__.py
+-rw-rw-rw-   0        0        0     2838 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/atom_utils.py
+-rw-rw-rw-   0        0        0    24444 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/cell.py
+-rw-rw-rw-   0        0        0    15657 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/doppler_utils.py
+-rw-rw-rw-   0        0        0    18590 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/energy_diagram.py
+-rw-rw-rw-   0        0        0    14820 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/experiments.py
+-rw-rw-rw-   0        0        0     2124 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/rydiqule_utils.py
+-rw-rw-rw-   0        0        0    76355 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/sensor.py
+-rw-rw-rw-   0        0        0     2886 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/sensor_solution.py
+-rw-rw-rw-   0        0        0    23896 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/sensor_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:39:54.722963 rydiqule-1.0.0rc2/src/rydiqule/slicing/
+-rw-rw-rw-   0        0        0        0 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/slicing/__init__.py
+-rw-rw-rw-   0        0        0    20282 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/slicing/slicing.py
+-rw-rw-rw-   0        0        0    11373 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/solvers.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:39:54.801070 rydiqule-1.0.0rc2/src/rydiqule/stack_solvers/
+-rw-rw-rw-   0        0        0        0 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/stack_solvers/__init__.py
+-rw-rw-rw-   0        0        0     7078 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/stack_solvers/cyrk_solver.py
+-rw-rw-rw-   0        0        0     6472 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/stack_solvers/nbkode_solver.py
+-rw-rw-rw-   0        0        0     6431 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/stack_solvers/nbrk_solver.py
+-rw-rw-rw-   0        0        0     5258 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/stack_solvers/scipy_solver.py
+-rw-rw-rw-   0        0        0    18887 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/src/rydiqule/timesolvers.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:39:54.707275 rydiqule-1.0.0rc2/src/rydiqule.egg-info/
+-rw-rw-rw-   0        0        0     5535 2023-05-24 20:39:54.000000 rydiqule-1.0.0rc2/src/rydiqule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1185 2023-05-24 20:39:54.000000 rydiqule-1.0.0rc2/src/rydiqule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 20:39:54.000000 rydiqule-1.0.0rc2/src/rydiqule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-24 20:37:26.000000 rydiqule-1.0.0rc2/src/rydiqule.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      262 2023-05-24 20:39:54.000000 rydiqule-1.0.0rc2/src/rydiqule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-24 20:39:54.000000 rydiqule-1.0.0rc2/src/rydiqule.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 20:39:55.019702 rydiqule-1.0.0rc2/tests/
+-rw-rw-rw-   0        0        0     2283 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/tests/test_EOMs.py
+-rw-rw-rw-   0        0        0     2638 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/tests/test_calculate_snr.py
+-rw-rw-rw-   0        0        0     4289 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/tests/test_cell.py
+-rw-rw-rw-   0        0        0     2553 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/tests/test_level_diagram.py
+-rw-rw-rw-   0        0        0     5489 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/tests/test_numbakitode.py
+-rw-rw-rw-   0        0        0     5162 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/tests/test_parameter_zip.py
+-rw-rw-rw-   0        0        0     4821 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/tests/test_sensor.py
+-rw-rw-rw-   0        0        0    10418 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/tests/test_solvers.py
+-rw-rw-rw-   0        0        0     2612 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/tests/test_steady_state_ham_gen.py
+-rw-rw-rw-   0        0        0     9564 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/tests/test_time.py
+-rw-rw-rw-   0        0        0     2992 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/tests/test_time_cyrk.py
+-rw-rw-rw-   0        0        0      952 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/tests/test_time_ham_gen.py
+-rw-rw-rw-   0        0        0     2377 2023-05-24 20:36:18.000000 rydiqule-1.0.0rc2/tests/test_utils.py
```

### Comparing `rydiqule-1.0.0/LICENSE` & `rydiqule-1.0.0rc2/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2023 Quantum Technology Center at the University of Maryland
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2023 Quantum Technology Center at the University of Maryland
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
    limitations under the License.
```

### Comparing `rydiqule-1.0.0/PKG-INFO` & `rydiqule-1.0.0rc2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,152 +1,148 @@
-Metadata-Version: 2.1
-Name: rydiqule
-Version: 1.0.0
-Summary: Rydberg Sensor Interactive Quantum Physics Module
-Author: ARL and NAWCWD
-License: Apache
-Keywords: rydberg,atomic-physics,quantum-optics,atomic-sensors,electrometry
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: tests
-Provides-Extra: mypy
-Provides-Extra: linter
-License-File: LICENSE
-
-<img src="https://raw.githubusercontent.com/QTC-UMD/rydiqule/main/docs/source/img/Rydiqule_Logo_Transparent_300.png" alt="rydiqule" style="max-width: 100%;">
-
-The Rydberg Interactive Quantum module is a modelling library designed to simulate
-the response of a Rydberg atoms to arbitrary input RF waveforms.
-It also functions as a general master equation solver based on the semi-classical density matrix method.
-
-[![PyPI](https://img.shields.io/pypi/v/rydiqule.svg)](https://pypi.org/project/rydiqule)
-[![Python Version](https://img.shields.io/pypi/pyversions/rydiqule.svg)](https://python.org)
-[![License](https://img.shields.io/pypi/l/rydiqule.svg)](https://github.com/QTC-UMD/rydiqule/raw/main/LICENSE)
-[![Docs](https://readthedocs.org/projects/rydiqule/badge/?version=latest)](https://rydiqule.readthedocs.io/en/latest)
-
-## Installation
-
-Presently, installation is done via pip.
-See below for detailed instructions.
-
-In all cases, it is highly recommended to install rydiqule in a virtual environment.
-
-### Conda/pip installation
-
-If using a conda to provide the virtual environmnet,
-it can often be advantageous to install as many packages as possible via conda before running the pip installation command.
-
-Assuming you have not already created a separate environment for RydIQule (recommended), run the following to create a new environment:
-```shell
-(base) ~/> conda create -n rydiqule python=3.9
-(base) ~/> conda activate rydiqule
-```
-RydIQule currently requires python >3.8.
-
-Now install dependencies that are available via conda.
-To capture as many dependencies as possible,
-we will add the `conda-forge` channel at a lower priority.
-```shell
-(rydiqule) ~/> conda config --append channels conda-forge
-(rydiqule) ~/> conda config --set channel_priority strict
-(rydiqule) ~/> conda install numpy scipy matplotlib networkx numba psutil
-# ARC specific dependencies available via conda
-(rydiqule) ~/> conda install sympy asteval lmfit uncertainties
-```
-
-Now use pip to install rydiqule and remaining dependencies.
-```shell
-# for normal installation
-(rydiqule) ~/> pip install rydiqule
-# for editable installation, so source can be modified locally
-(rydiqule) ~/> pip install -e rydiqule
-```
-
-### Pure pip installation
-
-To install normally, run:
-```shell
-pip install rydiqule
-```
-This command will use pip to install all necessary dependencies.
-
-To install in an editable way (which allows edits of the source code), run:
-```shell
-pip install -e rydiqule
-```
-
-### Confirm installation
-
-Proper installation can be confirmed by executing the following commands in a python terminal.
-```shell
->>> import rydiqule as rq
->>> rq.about()
-
-        Rydiqule
-    ================
-
-Rydiqule Version:     1.0.0
-Installation Path:    C:\Users\naqsL\Miniconda3\envs\rydiqule\lib\site-packages\rydiqule
-
-      Dependencies
-    ================
-
-NumPy Version:        1.24.3
-SciPy Version:        1.10.1
-Matplotlib Version:   3.7.1
-ARC Version:          3.3.0
-Python Version:       3.9.16
-Python Install Path:  C:\Users\naqsL\Miniconda3\envs\rydiqule
-Platform Info:        Windows (AMD64)
-CPU Count:            12
-Total System Memory:  128 GB
-```
-
-### Updating an existing installation
-
-Upgrading an existing installation is simple.
-Simply run the pip installation commands described above with the update flag.
-```shell
-pip install -U rydiqule
-```
-This command will also install any new dependencies that are required.
-
-If using an editable install, simply replacing the files in the same directory is sufficient.
-Though it is recommended to also run the appropriate pip update command as well.
-```shell
-pip install -U -e rydiqule
-```
-
-### Dependencies
-
-This package requires installation of the excellent [ARC](https://github.com/nikolasibalic/ARC-Alkali-Rydberg-Calculator) package, which is used to get Rydberg atomic properties.
-It also requires other standard computation dependenices, such as `numpy`, `scipy`, `matplotlib`, etc.
-These dependencies will be automatically installed by pip if not already present.
-
-The timesolver backend dependencies include the [numbakit-ode](https://github.com/hgrecco/numbakit-ode)
-and [CyRK](https://github.com/jrenaud90/CyRK) packages.
-Both are available via `pip`.
-
-## Documentation
-
-Documentation is available online at [readthedocs](https://rydiqule.readthedocs.io/en/latest).
-PDF or EPUB formats of the documentation can be downloaded from the online documentation.
-
-### Examples
-
-Example jupyter notebooks that demonstrate RydIQule can be found in the `examples` subdirectory.
-Printouts of these notebooks are available in the documentation as well.
-
-## Support
-
-Creation of this software was supported in part by the Defense Advanced Research Projects Agency (DARPA) Quantum Apertures program, DEVCOM Army Research Laboratory, and the Quantum Technology Center at the University of Maryland.
-
-## Disclaimer
-
-The views, opinions and/or findings expressed are those of the authors and should not be interpreted as representing the official views or policies of the Department of Defense or the U.S. Government.
+Metadata-Version: 2.1
+Name: rydiqule
+Version: 1.0.0rc2
+Summary: Rydberg Sensor Interactive Quantum Physics Module
+Author: ARL and NAWCWD
+License: Apache
+Keywords: rydberg,atomic-physics,quantum-optics,atomic-sensors,electrometry
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: tests
+Provides-Extra: mypy
+Provides-Extra: linter
+License-File: LICENSE
+
+![Rydiqule Logo](docs/source/img/Rydiqule_Logo_Transparent_300.png)
+
+The Rydberg Interactive Quantum module is a modelling library designed to simulate
+the response of a Rydberg atoms to arbitrary input RF waveforms.
+It also functions as a general master equation solver based on the semi-classical density matrix method.
+
+[![Docs](https://readthedocs.org/projects/rydiqule/badge/?version=latest)](https://rydiqule.readthedocs.io/en/latest)
+
+## Installation
+
+Presently, installation must be done manually using a copy of the repository.
+After downloading or cloning this repository,
+follow the directions below for installation.
+
+### Pure pip installation
+
+To install in an editable way (which allows edits of the source code), run:
+```shell
+pip install -e .
+```
+from within the top level `rydiqule` directory (i.e. where the `setup.cfg` file resides).
+This command will use pip to install all necessary dependencies.
+
+To install normally, run:
+```shell
+pip install .
+```
+from the same directory.
+
+### Conda/pip installation
+
+If using a conda environment, it can often be advantageous to install as many packages via conda before running the pip installation command.
+
+Assuming you have not already created a separate environment for RydIQule (recommended), run the following to create a new environment:
+```shell
+(base) ~/Rydiqule> conda create -n rydiqule python=3.9
+(base) ~/Rydiqule> conda activate rydiqule
+```
+RydIQule currently requires python >3.8.
+
+Now install dependencies that are available via conda.
+To capture as many dependencies as possible,
+we will add the `conda-forge` channel at a lower priority.
+```shell
+(rydiqule) ~/Rydiqule> conda config --append channels conda-forge
+(rydiqule) ~/Rydiqule> conda config --set channel_priority strict
+(rydiqule) ~/Rydiqule> conda install numpy scipy matplotlib networkx psutil
+# ARC specific dependencies available via conda
+(rydiqule) ~/Rydiqule> conda install sympy asteval lmfit uncertainties
+```
+
+Now use pip to install rydiqule and remaining dependencies.
+```shell
+# for editable installation, so source can be modified locally
+(rydiqule) ~/Rydiqule> pip install -e .
+# for normal installation
+(rydiqule) ~/Rydiqule> pip install .
+```
+
+### Confirm installation
+
+Proper installation can be confirmed by executing the following commands in a python terminal.
+```shell
+>>> import rydiqule as rq
+>>> rq.about()
+
+        Rydiqule
+    ================
+
+Rydiqule Version:     0.3.0
+Installation Path:    c:\users\naqsl\src\rydiqule\src\rydiqule
+
+      Dependencies
+    ================
+
+NumPy Version:        1.20.3
+SciPy Version:        1.7.1
+Matplotlib Version:   3.5.0
+ARC Version:          3.2.0
+Python Version:       3.8.12
+Python Install Path:  C:\Users\naqsL\Miniconda3\envs\arc
+Platform Info:        Windows (AMD64)
+CPU Count:            12
+Total System Memory:  128 GB
+```
+
+### Updating an existing installation
+
+Upgrading an existing installation is simple.
+Simply run the pip installation commands described above with the update flag.
+```shell
+pip install -U .
+```
+This command will also install any new dependencies that are required.
+
+If using an editable install, simply replacing the files in the same directory is sufficient.
+Though it is recommended to also run the appropriate pip update command as well.
+```shell
+pip install -U -e .
+```
+
+### Dependencies
+
+This package requires installation of the excellent [ARC](https://github.com/nikolasibalic/ARC-Alkali-Rydberg-Calculator) package, which is used to get Rydberg atomic properties.
+It also requires other standard computation dependenices, such as `numpy`, `scipy`, `matplotlib`, etc.
+These dependencies will be automatically installed by pip if not already present.
+
+The timesolver backend dependencies include the `numbakit-ode` and `CyRK` packages.
+Both are available via `pip`.
+
+## Documentation
+
+Documentation is available online at [readthedocs](https://rydiqule.readthedocs.io/en/latest).
+PDF or EPUB formats of the documentation can be downloaded from the online documentation.
+
+### Examples
+
+Example jupyter notebooks that demonstrate RydIQule can be found in the `examples` subdirectory.
+Printouts of these notebooks are available in the documentation as well.
+
+## Support
+
+Creation of this software was supported in part by the Defense Advanced Research Projects Agency (DARPA) Quantum Apertures program, DEVCOM Army Research Laboratory, and the Quantum Technology Center at the University of Maryland.
+
+## Disclaimer
+
+The views, opinions and/or findings expressed are those of the authors and should not be interpreted as representing the official views or policies of the Department of Defense or the U.S. Government.
```

### Comparing `rydiqule-1.0.0/README.md` & `rydiqule-1.0.0rc2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,131 +1,127 @@
-<img src="https://raw.githubusercontent.com/QTC-UMD/rydiqule/main/docs/source/img/Rydiqule_Logo_Transparent_300.png" alt="rydiqule" style="max-width: 100%;">
-
-The Rydberg Interactive Quantum module is a modelling library designed to simulate
-the response of a Rydberg atoms to arbitrary input RF waveforms.
-It also functions as a general master equation solver based on the semi-classical density matrix method.
-
-[![PyPI](https://img.shields.io/pypi/v/rydiqule.svg)](https://pypi.org/project/rydiqule)
-[![Python Version](https://img.shields.io/pypi/pyversions/rydiqule.svg)](https://python.org)
-[![License](https://img.shields.io/pypi/l/rydiqule.svg)](https://github.com/QTC-UMD/rydiqule/raw/main/LICENSE)
-[![Docs](https://readthedocs.org/projects/rydiqule/badge/?version=latest)](https://rydiqule.readthedocs.io/en/latest)
-
-## Installation
-
-Presently, installation is done via pip.
-See below for detailed instructions.
-
-In all cases, it is highly recommended to install rydiqule in a virtual environment.
-
-### Conda/pip installation
-
-If using a conda to provide the virtual environmnet,
-it can often be advantageous to install as many packages as possible via conda before running the pip installation command.
-
-Assuming you have not already created a separate environment for RydIQule (recommended), run the following to create a new environment:
-```shell
-(base) ~/> conda create -n rydiqule python=3.9
-(base) ~/> conda activate rydiqule
-```
-RydIQule currently requires python >3.8.
-
-Now install dependencies that are available via conda.
-To capture as many dependencies as possible,
-we will add the `conda-forge` channel at a lower priority.
-```shell
-(rydiqule) ~/> conda config --append channels conda-forge
-(rydiqule) ~/> conda config --set channel_priority strict
-(rydiqule) ~/> conda install numpy scipy matplotlib networkx numba psutil
-# ARC specific dependencies available via conda
-(rydiqule) ~/> conda install sympy asteval lmfit uncertainties
-```
-
-Now use pip to install rydiqule and remaining dependencies.
-```shell
-# for normal installation
-(rydiqule) ~/> pip install rydiqule
-# for editable installation, so source can be modified locally
-(rydiqule) ~/> pip install -e rydiqule
-```
-
-### Pure pip installation
-
-To install normally, run:
-```shell
-pip install rydiqule
-```
-This command will use pip to install all necessary dependencies.
-
-To install in an editable way (which allows edits of the source code), run:
-```shell
-pip install -e rydiqule
-```
-
-### Confirm installation
-
-Proper installation can be confirmed by executing the following commands in a python terminal.
-```shell
->>> import rydiqule as rq
->>> rq.about()
-
-        Rydiqule
-    ================
-
-Rydiqule Version:     1.0.0
-Installation Path:    C:\Users\naqsL\Miniconda3\envs\rydiqule\lib\site-packages\rydiqule
-
-      Dependencies
-    ================
-
-NumPy Version:        1.24.3
-SciPy Version:        1.10.1
-Matplotlib Version:   3.7.1
-ARC Version:          3.3.0
-Python Version:       3.9.16
-Python Install Path:  C:\Users\naqsL\Miniconda3\envs\rydiqule
-Platform Info:        Windows (AMD64)
-CPU Count:            12
-Total System Memory:  128 GB
-```
-
-### Updating an existing installation
-
-Upgrading an existing installation is simple.
-Simply run the pip installation commands described above with the update flag.
-```shell
-pip install -U rydiqule
-```
-This command will also install any new dependencies that are required.
-
-If using an editable install, simply replacing the files in the same directory is sufficient.
-Though it is recommended to also run the appropriate pip update command as well.
-```shell
-pip install -U -e rydiqule
-```
-
-### Dependencies
-
-This package requires installation of the excellent [ARC](https://github.com/nikolasibalic/ARC-Alkali-Rydberg-Calculator) package, which is used to get Rydberg atomic properties.
-It also requires other standard computation dependenices, such as `numpy`, `scipy`, `matplotlib`, etc.
-These dependencies will be automatically installed by pip if not already present.
-
-The timesolver backend dependencies include the [numbakit-ode](https://github.com/hgrecco/numbakit-ode)
-and [CyRK](https://github.com/jrenaud90/CyRK) packages.
-Both are available via `pip`.
-
-## Documentation
-
-Documentation is available online at [readthedocs](https://rydiqule.readthedocs.io/en/latest).
-PDF or EPUB formats of the documentation can be downloaded from the online documentation.
-
-### Examples
-
-Example jupyter notebooks that demonstrate RydIQule can be found in the `examples` subdirectory.
-Printouts of these notebooks are available in the documentation as well.
-
-## Support
-
-Creation of this software was supported in part by the Defense Advanced Research Projects Agency (DARPA) Quantum Apertures program, DEVCOM Army Research Laboratory, and the Quantum Technology Center at the University of Maryland.
-
-## Disclaimer
-
+![Rydiqule Logo](docs/source/img/Rydiqule_Logo_Transparent_300.png)
+
+The Rydberg Interactive Quantum module is a modelling library designed to simulate
+the response of a Rydberg atoms to arbitrary input RF waveforms.
+It also functions as a general master equation solver based on the semi-classical density matrix method.
+
+[![Docs](https://readthedocs.org/projects/rydiqule/badge/?version=latest)](https://rydiqule.readthedocs.io/en/latest)
+
+## Installation
+
+Presently, installation must be done manually using a copy of the repository.
+After downloading or cloning this repository,
+follow the directions below for installation.
+
+### Pure pip installation
+
+To install in an editable way (which allows edits of the source code), run:
+```shell
+pip install -e .
+```
+from within the top level `rydiqule` directory (i.e. where the `setup.cfg` file resides).
+This command will use pip to install all necessary dependencies.
+
+To install normally, run:
+```shell
+pip install .
+```
+from the same directory.
+
+### Conda/pip installation
+
+If using a conda environment, it can often be advantageous to install as many packages via conda before running the pip installation command.
+
+Assuming you have not already created a separate environment for RydIQule (recommended), run the following to create a new environment:
+```shell
+(base) ~/Rydiqule> conda create -n rydiqule python=3.9
+(base) ~/Rydiqule> conda activate rydiqule
+```
+RydIQule currently requires python >3.8.
+
+Now install dependencies that are available via conda.
+To capture as many dependencies as possible,
+we will add the `conda-forge` channel at a lower priority.
+```shell
+(rydiqule) ~/Rydiqule> conda config --append channels conda-forge
+(rydiqule) ~/Rydiqule> conda config --set channel_priority strict
+(rydiqule) ~/Rydiqule> conda install numpy scipy matplotlib networkx psutil
+# ARC specific dependencies available via conda
+(rydiqule) ~/Rydiqule> conda install sympy asteval lmfit uncertainties
+```
+
+Now use pip to install rydiqule and remaining dependencies.
+```shell
+# for editable installation, so source can be modified locally
+(rydiqule) ~/Rydiqule> pip install -e .
+# for normal installation
+(rydiqule) ~/Rydiqule> pip install .
+```
+
+### Confirm installation
+
+Proper installation can be confirmed by executing the following commands in a python terminal.
+```shell
+>>> import rydiqule as rq
+>>> rq.about()
+
+        Rydiqule
+    ================
+
+Rydiqule Version:     0.3.0
+Installation Path:    c:\users\naqsl\src\rydiqule\src\rydiqule
+
+      Dependencies
+    ================
+
+NumPy Version:        1.20.3
+SciPy Version:        1.7.1
+Matplotlib Version:   3.5.0
+ARC Version:          3.2.0
+Python Version:       3.8.12
+Python Install Path:  C:\Users\naqsL\Miniconda3\envs\arc
+Platform Info:        Windows (AMD64)
+CPU Count:            12
+Total System Memory:  128 GB
+```
+
+### Updating an existing installation
+
+Upgrading an existing installation is simple.
+Simply run the pip installation commands described above with the update flag.
+```shell
+pip install -U .
+```
+This command will also install any new dependencies that are required.
+
+If using an editable install, simply replacing the files in the same directory is sufficient.
+Though it is recommended to also run the appropriate pip update command as well.
+```shell
+pip install -U -e .
+```
+
+### Dependencies
+
+This package requires installation of the excellent [ARC](https://github.com/nikolasibalic/ARC-Alkali-Rydberg-Calculator) package, which is used to get Rydberg atomic properties.
+It also requires other standard computation dependenices, such as `numpy`, `scipy`, `matplotlib`, etc.
+These dependencies will be automatically installed by pip if not already present.
+
+The timesolver backend dependencies include the `numbakit-ode` and `CyRK` packages.
+Both are available via `pip`.
+
+## Documentation
+
+Documentation is available online at [readthedocs](https://rydiqule.readthedocs.io/en/latest).
+PDF or EPUB formats of the documentation can be downloaded from the online documentation.
+
+### Examples
+
+Example jupyter notebooks that demonstrate RydIQule can be found in the `examples` subdirectory.
+Printouts of these notebooks are available in the documentation as well.
+
+## Support
+
+Creation of this software was supported in part by the Defense Advanced Research Projects Agency (DARPA) Quantum Apertures program, DEVCOM Army Research Laboratory, and the Quantum Technology Center at the University of Maryland.
+
+## Disclaimer
+
 The views, opinions and/or findings expressed are those of the authors and should not be interpreted as representing the official views or policies of the Department of Defense or the U.S. Government.
```

### Comparing `rydiqule-1.0.0/setup.cfg` & `rydiqule-1.0.0rc2/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,75 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 7279 6469 7175 6c65 0a76 6572 7369  = rydiqule.versi
-00000020: 6f6e 203d 2061 7474 723a 2072 7964 6971  on = attr: rydiq
-00000030: 756c 652e 5f5f 7665 7273 696f 6e5f 5f0a  ule.__version__.
-00000040: 6465 7363 7269 7074 696f 6e20 3d20 5279  description = Ry
-00000050: 6462 6572 6720 5365 6e73 6f72 2049 6e74  dberg Sensor Int
-00000060: 6572 6163 7469 7665 2051 7561 6e74 756d  eractive Quantum
-00000070: 2050 6879 7369 6373 204d 6f64 756c 650a   Physics Module.
-00000080: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000090: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-000000a0: 6d64 0a6c 6f6e 675f 6465 7363 7269 7074  md.long_descript
-000000b0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-000000c0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-000000d0: 0a61 7574 686f 7220 3d20 4152 4c20 616e  .author = ARL an
-000000e0: 6420 4e41 5743 5744 0a6b 6579 776f 7264  d NAWCWD.keyword
-000000f0: 7320 3d20 0a09 7279 6462 6572 670a 0961  s = ..rydberg..a
-00000100: 746f 6d69 632d 7068 7973 6963 730a 0971  tomic-physics..q
-00000110: 7561 6e74 756d 2d6f 7074 6963 730a 0961  uantum-optics..a
-00000120: 746f 6d69 632d 7365 6e73 6f72 730a 0965  tomic-sensors..e
-00000130: 6c65 6374 726f 6d65 7472 790a 6c69 6365  lectrometry.lice
-00000140: 6e73 6520 3d20 4170 6163 6865 0a63 6c61  nse = Apache.cla
-00000150: 7373 6966 6965 7273 203d 200a 0944 6576  ssifiers = ..Dev
-00000160: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
-00000170: 3a3a 2035 202d 2050 726f 6475 6374 696f  :: 5 - Productio
-00000180: 6e2f 5374 6162 6c65 0a09 4c69 6365 6e73  n/Stable..Licens
-00000190: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-000001a0: 6420 3a3a 2041 7061 6368 6520 536f 6674  d :: Apache Soft
-000001b0: 7761 7265 204c 6963 656e 7365 0a09 5072  ware License..Pr
-000001c0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001d0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001e0: 3320 3a3a 204f 6e6c 790a 0950 726f 6772  3 :: Only..Progr
-000001f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000200: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
-00000210: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000220: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000230: 203a 3a20 332e 390a 0950 726f 6772 616d   :: 3.9..Program
-00000240: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000250: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
-00000260: 0a5b 6f70 7469 6f6e 735d 0a7a 6970 5f73  .[options].zip_s
-00000270: 6166 6520 3d20 4661 6c73 650a 696e 636c  afe = False.incl
-00000280: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
-00000290: 203d 2054 7275 650a 7061 636b 6167 655f   = True.package_
-000002a0: 6469 7220 3d20 0a09 3d73 7263 0a70 6163  dir = ..=src.pac
-000002b0: 6b61 6765 7320 3d20 6669 6e64 3a0a 7079  kages = find:.py
-000002c0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-000002d0: 3e3d 2033 2e38 0a69 6e73 7461 6c6c 5f72  >= 3.8.install_r
-000002e0: 6571 7569 7265 7320 3d20 0a09 6172 632d  equires = ..arc-
-000002f0: 616c 6b61 6c69 2d72 7964 6265 7267 2d63  alkali-rydberg-c
-00000300: 616c 6375 6c61 746f 720a 096e 756d 7079  alculator..numpy
-00000310: 0a09 7363 6970 793e 3d30 2e31 392e 310a  ..scipy>=0.19.1.
-00000320: 096d 6174 706c 6f74 6c69 620a 096e 756d  .matplotlib..num
-00000330: 6261 6b69 742d 6f64 650a 096e 756d 6261  bakit-ode..numba
-00000340: 0a09 6379 726b 3e3d 302e 352e 330a 096e  ..cyrk>=0.5.3..n
-00000350: 6574 776f 726b 780a 0970 7375 7469 6c0a  etworkx..psutil.
-00000360: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-00000370: 6573 2e66 696e 645d 0a77 6865 7265 203d  es.find].where =
-00000380: 2073 7263 0a0a 5b6f 7074 696f 6e73 2e65   src..[options.e
-00000390: 7874 7261 735f 7265 7175 6972 655d 0a64  xtras_require].d
-000003a0: 6f63 7320 3d20 0a09 5370 6869 6e78 3d3d  ocs = ..Sphinx==
-000003b0: 352e 302e 320a 0973 7068 696e 782d 7274  5.0.2..sphinx-rt
-000003c0: 642d 7468 656d 653d 3d31 2e31 2e31 0a09  d-theme==1.1.1..
-000003d0: 6e62 636f 6e76 6572 740a 0970 616e 646f  nbconvert..pando
-000003e0: 630a 0969 7079 7468 6f6e 0a74 6573 7473  c..ipython.tests
-000003f0: 203d 200a 0970 7974 6573 740a 0963 6f76   = ..pytest..cov
-00000400: 6572 6167 650a 0970 7974 6573 742d 636f  erage..pytest-co
-00000410: 760a 6d79 7079 203d 200a 096d 7970 790a  v.mypy = ..mypy.
-00000420: 096e 756d 7079 3e3d 312e 3231 0a09 6c78  .numpy>=1.21..lx
-00000430: 6d6c 0a6c 696e 7465 7220 3d20 0a09 7275  ml.linter = ..ru
-00000440: 6666 0a0a 5b65 6767 5f69 6e66 6f5d 0a74  ff..[egg_info].t
-00000450: 6167 5f62 7569 6c64 203d 200a 7461 675f  ag_build = .tag_
-00000460: 6461 7465 203d 2030 0a0a                 date = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2072 7964 6971 756c 650d 0a76 6572   = rydiqule..ver
+00000020: 7369 6f6e 203d 2061 7474 723a 2072 7964  sion = attr: ryd
+00000030: 6971 756c 652e 5f5f 7665 7273 696f 6e5f  iqule.__version_
+00000040: 5f0d 0a64 6573 6372 6970 7469 6f6e 203d  _..description =
+00000050: 2052 7964 6265 7267 2053 656e 736f 7220   Rydberg Sensor 
+00000060: 496e 7465 7261 6374 6976 6520 5175 616e  Interactive Quan
+00000070: 7475 6d20 5068 7973 6963 7320 4d6f 6475  tum Physics Modu
+00000080: 6c65 0d0a 6c6f 6e67 5f64 6573 6372 6970  le..long_descrip
+00000090: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
+000000a0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
+000000b0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
+000000c0: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
+000000d0: 6b64 6f77 6e0d 0a61 7574 686f 7220 3d20  kdown..author = 
+000000e0: 4152 4c20 616e 6420 4e41 5743 5744 0d0a  ARL and NAWCWD..
+000000f0: 6b65 7977 6f72 6473 203d 200d 0a09 7279  keywords = ...ry
+00000100: 6462 6572 670d 0a09 6174 6f6d 6963 2d70  dberg...atomic-p
+00000110: 6879 7369 6373 0d0a 0971 7561 6e74 756d  hysics...quantum
+00000120: 2d6f 7074 6963 730d 0a09 6174 6f6d 6963  -optics...atomic
+00000130: 2d73 656e 736f 7273 0d0a 0965 6c65 6374  -sensors...elect
+00000140: 726f 6d65 7472 790d 0a6c 6963 656e 7365  rometry..license
+00000150: 203d 2041 7061 6368 650d 0a63 6c61 7373   = Apache..class
+00000160: 6966 6965 7273 203d 200d 0a09 4465 7665  ifiers = ...Deve
+00000170: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
+00000180: 3a20 3520 2d20 5072 6f64 7563 7469 6f6e  : 5 - Production
+00000190: 2f53 7461 626c 650d 0a09 4c69 6365 6e73  /Stable...Licens
+000001a0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+000001b0: 6420 3a3a 2041 7061 6368 6520 536f 6674  d :: Apache Soft
+000001c0: 7761 7265 204c 6963 656e 7365 0d0a 0950  ware License...P
+000001d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000001e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000001f0: 2033 203a 3a20 4f6e 6c79 0d0a 0950 726f   3 :: Only...Pro
+00000200: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000210: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000220: 2e38 0d0a 0950 726f 6772 616d 6d69 6e67  .8...Programming
+00000230: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000240: 686f 6e20 3a3a 2033 2e39 0d0a 0950 726f  hon :: 3.9...Pro
+00000250: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000260: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000270: 2e31 300d 0a0d 0a5b 6f70 7469 6f6e 735d  .10....[options]
+00000280: 0d0a 7a69 705f 7361 6665 203d 2046 616c  ..zip_safe = Fal
+00000290: 7365 0d0a 696e 636c 7564 655f 7061 636b  se..include_pack
+000002a0: 6167 655f 6461 7461 203d 2054 7275 650d  age_data = True.
+000002b0: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
+000002c0: 0a09 3d73 7263 0d0a 7061 636b 6167 6573  ..=src..packages
+000002d0: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
+000002e0: 5f72 6571 7569 7265 7320 3d20 3e3d 2033  _requires = >= 3
+000002f0: 2e38 0d0a 696e 7374 616c 6c5f 7265 7175  .8..install_requ
+00000300: 6972 6573 203d 200d 0a09 6172 632d 616c  ires = ...arc-al
+00000310: 6b61 6c69 2d72 7964 6265 7267 2d63 616c  kali-rydberg-cal
+00000320: 6375 6c61 746f 720d 0a09 6e75 6d70 790d  culator...numpy.
+00000330: 0a09 7363 6970 793e 3d30 2e31 392e 310d  ..scipy>=0.19.1.
+00000340: 0a09 6d61 7470 6c6f 746c 6962 0d0a 096e  ..matplotlib...n
+00000350: 756d 6261 6b69 742d 6f64 650d 0a09 6e75  umbakit-ode...nu
+00000360: 6d62 610d 0a09 6379 726b 3e3d 302e 352e  mba...cyrk>=0.5.
+00000370: 330d 0a09 6e65 7477 6f72 6b78 0d0a 0970  3...networkx...p
+00000380: 7375 7469 6c0d 0a0d 0a5b 6f70 7469 6f6e  sutil....[option
+00000390: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+000003a0: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
+000003b0: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
+000003c0: 5f72 6571 7569 7265 5d0d 0a64 6f63 7320  _require]..docs 
+000003d0: 3d20 0d0a 0953 7068 696e 783d 3d35 2e30  = ...Sphinx==5.0
+000003e0: 2e32 0d0a 0973 7068 696e 782d 7274 642d  .2...sphinx-rtd-
+000003f0: 7468 656d 653d 3d31 2e31 2e31 0d0a 096e  theme==1.1.1...n
+00000400: 6263 6f6e 7665 7274 0d0a 0970 616e 646f  bconvert...pando
+00000410: 630d 0a09 6970 7974 686f 6e0d 0a74 6573  c...ipython..tes
+00000420: 7473 203d 200d 0a09 7079 7465 7374 0d0a  ts = ...pytest..
+00000430: 0963 6f76 6572 6167 650d 0a09 7079 7465  .coverage...pyte
+00000440: 7374 2d63 6f76 0d0a 6d79 7079 203d 200d  st-cov..mypy = .
+00000450: 0a09 6d79 7079 0d0a 096e 756d 7079 3e3d  ..mypy...numpy>=
+00000460: 312e 3231 0d0a 096c 786d 6c0d 0a6c 696e  1.21...lxml..lin
+00000470: 7465 7220 3d20 0d0a 0966 6c61 6b65 380d  ter = ...flake8.
+00000480: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000490: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+000004a0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `rydiqule-1.0.0/src/rydiqule/__init__.py` & `rydiqule-1.0.0rc2/src/rydiqule/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-'''
-Parent computational module.
-'''
-
-from .experiments import get_transmission_coef, get_susceptibility, get_phase_shift, get_solution_element, get_snr
-
-from .cell import Cell
-from .sensor import Sensor
-from .sensor_utils import generate_eom, get_basis_transform, get_rho_ij, get_rho_populations, scale_dipole, draw_diagram,  calc_kappa, calc_eta
-from .atom_utils import D1_states, D2_states
-from .solvers import solve_steady_state
-from .timesolvers import solve_time, solve_eom_stack, generate_eom_time
-from .doppler_utils import get_doppler_equations, generate_doppler_shift_eom, doppler_classes, doppler_mesh, apply_doppler_weights
-from .rydiqule_utils import about
-
-from .slicing.slicing import compute_grid, matrix_slice, memory_size, get_slice_num, get_slice_num_t
-
-__version__ = '1.0.0'
+'''
+Parent computational module.
+'''
+
+from .experiments import get_transmission_coef, get_susceptibility, get_phase_shift, get_solution_element, get_snr
+
+from .cell import Cell
+from .sensor import Sensor
+from .sensor_utils import generate_eom, get_basis_transform, get_rho_ij, get_rho_populations, scale_dipole, draw_diagram,  calc_kappa, calc_eta
+from .atom_utils import D1_states, D2_states
+from .solvers import solve_steady_state
+from .timesolvers import solve_time, solve_eom_stack, generate_eom_time
+from .doppler_utils import get_doppler_equations, generate_doppler_shift_eom, doppler_classes, doppler_mesh, apply_doppler_weights
+from .rydiqule_utils import about
+
+from .slicing.slicing import compute_grid, matrix_slice, memory_size, get_slice_num, get_slice_num_t
+
+__version__ = '1.0.0rc2'
```

### Comparing `rydiqule-1.0.0/src/rydiqule/atom_utils.py` & `rydiqule-1.0.0rc2/src/rydiqule/atom_utils.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-"""
-Utilities for interacting with atomic parameters and ARC.
-"""
-
-import arc.alkali_atom_data as arc_atoms
-
-from typing import Union
-
-ATOMS = {
-    'H': arc_atoms.Hydrogen,
-    'Li6': arc_atoms.Lithium6, 'Li7': arc_atoms.Lithium7,
-    'Na': arc_atoms.Sodium,
-    'K39': arc_atoms.Potassium39, 'K40': arc_atoms.Potassium40, 'K41': arc_atoms.Potassium41,
-    'Rb85': arc_atoms.Rubidium85, 'Rb87': arc_atoms.Rubidium87,
-    'Cs': arc_atoms.Caesium
-}
-"""
-Alkali atoms defined by ARC that can be used with :class:`~.Cell`.
-"""
-
-ground_n = {
-    "H": 1,
-    "Li": 2, "Li6": 2, "Li7": 2,
-    "Na": 3,
-    "K": 4, "K39": 4, "K40": 4, "K41": 4,
-    "Rb": 5, "Rb85": 5, "Rb87": 5,
-    "Cs": 6
-}
-
-
-def D1_states(n: Union[int, str]):
-    """
-    Retrieve the quantum numbers for the states corresponding to
-    the D1 line for a given Rydberg atom or principle quantum number.
-
-    Parameters
-    ----------
-    n: int or str
-        Either the string flag of the atom or the principle quantum number n of
-        an atom. If string, must be one of ['H', 'Li', 'Li6', 'Li7', 'Na', 'K', 'K39', 'K40',
-        'K41', 'Rb', 'Rb85', 'Rb87', 'Cs'].
-
-    Returns
-    -------
-    list
-        Quantum numbers [n, l, j, m] of the atoms ground state.
-    list
-        Quantum numbers [n, l, j, m] of the first excited state corresponding
-        to the D1 line of the Rydberg atom.
-    """
-
-    if type(n) is str:
-
-        if n in ground_n.keys():
-            n = ground_n[n]
-        else:
-            raise ValueError(f"For string value of n, must use one of {list(ground_n.keys())}")
-
-    if type(n) != int:
-        raise ValueError(f"n must be int or str, but found type {type(n)}.")
-
-    return [n, 0, 1/2, 1/2], [n, 1, 1/2, 1/2]
-
-
-def D2_states(n: Union[int, str]):
-    """
-    Retrieve the quantum numbers for the states corresponding to the D2 line for a
-    given Rydberg atom or principle quantum number.
-
-    Parameters
-    ----------
-    n: int or str
-        Either the string flag of the atom or the principle quantum number n of
-        an atom. If string, must be one of ['H', 'Li', 'Li6', 'Li7', 'Na', 'K', 'K39', 'K40',
-        'K41', 'Rb', 'Rb85', 'Rb87', 'Cs'].
-
-    Returns
-    -------
-    list
-        Quantum numbers [n, l, j, m] of the atoms ground state.
-    list
-        Quantum numbers [n, l, j, m] of the first excited state corresponding
-        to the D2 line of the Rydberg atom.
-    """
-
-    if type(n) is str:
-
-        if n in ground_n.keys():
-            n = ground_n[n]
-        else:
-            raise ValueError(f"For string value of n, must use one of {list(ground_n.keys())}")
-
-    if type(n) != int:
-        raise ValueError(f"n must be int or str, but found type {type(n)}.")
-
-    return [n, 0, 1/2, 1/2], [n, 1, 3/2, 1/2]
+"""
+Utilities for interacting with atomic parameters and ARC.
+"""
+
+import arc.alkali_atom_data as arc_atoms
+
+from typing import Union
+
+ATOMS = {
+    'H': arc_atoms.Hydrogen,
+    'Li6': arc_atoms.Lithium6, 'Li7': arc_atoms.Lithium7,
+    'Na': arc_atoms.Sodium,
+    'K39': arc_atoms.Potassium39, 'K40': arc_atoms.Potassium40, 'K41': arc_atoms.Potassium41,
+    'Rb85': arc_atoms.Rubidium85, 'Rb87': arc_atoms.Rubidium87,
+    'Cs': arc_atoms.Caesium
+}
+"""
+Alkali atoms defined by ARC that can be used with :class:`~.Cell`.
+"""
+
+ground_n = {
+    "H": 1,
+    "Li": 2, "Li6": 2, "Li7": 2,
+    "Na": 3,
+    "K": 4, "K39": 4, "K40": 4, "K41": 4,
+    "Rb": 5, "Rb85": 5, "Rb87": 5,
+    "Cs": 6
+}
+
+
+def D1_states(n: Union[int, str]):
+    """
+    Retrieve the quantum numbers for the states corresponding to
+    the D1 line for a given Rydberg atom or principle quantum number.
+
+    Parameters
+    ----------
+    n: int or str
+        Either the string flag of the atom or the principle quantum number n of
+        an atom. If string, must be one of ['H', 'Li', 'Li6', 'Li7', 'Na', 'K', 'K39', 'K40',
+        'K41', 'Rb', 'Rb85', 'Rb87', 'Cs'].
+
+    Returns
+    -------
+    list
+        Quantum numbers [n, l, j, m] of the atoms ground state.
+    list
+        Quantum numbers [n, l, j, m] of the first excited state corresponding
+        to the D1 line of the Rydberg atom.
+    """
+
+    if type(n) is str:
+
+        if n in ground_n.keys():
+            n = ground_n[n]
+        else:
+            raise ValueError(f"For string value of n, must use one of {list(ground_n.keys())}")
+
+    if type(n) != int:
+        raise ValueError(f"n must be int or str, but found type {type(n)}.")
+
+    return [n, 0, 1/2, 1/2], [n, 1, 1/2, 1/2]
+
+
+def D2_states(n: Union[int, str]):
+    """
+    Retrieve the quantum numbers for the states corresponding to the D2 line for a
+    given Rydberg atom or principle quantum number.
+
+    Parameters
+    ----------
+    n: int or str
+        Either the string flag of the atom or the principle quantum number n of
+        an atom. If string, must be one of ['H', 'Li', 'Li6', 'Li7', 'Na', 'K', 'K39', 'K40',
+        'K41', 'Rb', 'Rb85', 'Rb87', 'Cs'].
+
+    Returns
+    -------
+    list
+        Quantum numbers [n, l, j, m] of the atoms ground state.
+    list
+        Quantum numbers [n, l, j, m] of the first excited state corresponding
+        to the D2 line of the Rydberg atom.
+    """
+
+    if type(n) is str:
+
+        if n in ground_n.keys():
+            n = ground_n[n]
+        else:
+            raise ValueError(f"For string value of n, must use one of {list(ground_n.keys())}")
+
+    if type(n) != int:
+        raise ValueError(f"n must be int or str, but found type {type(n)}.")
+
+    return [n, 0, 1/2, 1/2], [n, 1, 3/2, 1/2]
```

### Comparing `rydiqule-1.0.0/src/rydiqule/cell.py` & `rydiqule-1.0.0rc2/src/rydiqule/cell.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,546 +1,531 @@
-"""
-Physical Cell objects for use in solvers.
-"""
-
-import scipy
-import numpy as np
-import warnings
-
-import scipy.constants
-from scipy.constants import Boltzmann
-
-# rydiqule imports
-from .sensor import Sensor, ScannableParameter
-from .sensor_utils import scale_dipole, calc_eta, calc_kappa
-from .atom_utils import ATOMS
-
-from typing import Literal, Optional, Sequence, List, Tuple, Callable
-
-a0 = scipy.constants.physical_constants["Bohr radius"][0]
-
-AtomFlags = Literal['H', 'Li6', 'Li7', 'Na', 'K39', 'K40', 'K41', 'Rb85', 'Rb87', 'Cs']
-QState = Sequence  # TODO: consider using named tuples here
-States = Tuple[int, ...]
-
-
-class Cell(Sensor):
-    """
-    Subclass of :class:`~.Sensor` that creates a Sensor with additional physical properties
-    corresponding to a specific Rydberg atom.
-
-    In addition to the core functionality of `~.Sensor`, this class allows for labelling of states
-    with quantum numbers, calculating of state lifetimes and decoherences and tracking of
-    of some physical laser parameters.
-    A key distictinction between a :class:`~.Cell` and a :class:`~.Sensor` is that
-    a cell supports (and requires) and absolute ordering of energy between states,
-    which allows for implicit calculation of decay rates an transition frequencies.
-
-    """
-
-    # these are not optional for a Cell
-    eta: float
-    kappa: float
-
-    def __init__(self, atom_flag: AtomFlags, *atomic_states: QState,
-                 gamma_transit: Optional[float] = None, cell_length: float = 0,
-                 beam_area: float = 1e-6, beam_diam: Optional[float] = None,
-                 temp: float = 300.0) -> None:
-        """
-        Initialize the Rydberg cell from the given parameters. 
-
-        Parameters
-        ----------
-        atom_flag : str 
-            Which atom is used in the cell for calculating physical properties with ARC Rydberg.
-            One of ['H', 'Li6', 'Li7', 'Na', 'K39', 'K40', 'K41', 'Rb85', 'Rb87', 'Cs'].
-        atomic_states : list[list]
-            List of states to be added to the cell. Each state is 
-            an iterable whose elements are each a list of the form [n, l, j, m], represnting the 
-            Rydberg atomic quantum numbers of the state. At least two states must be added so 
-            that the system is nontrivial. The number of states will determine the basis size
-            of the system. 
-        gamma_transit : float, optional
-            Decoherence due to atom transit through the optical
-            beams. Specified in units of Mrad/s. If `None`, will calculate based
-            on value of `beam_area`. See :meth:`~.Sensor.add_transit_broadening` for
-            details on how transit broadening is treated. Default is None.
-        beam_area : float, optional
-            Area of probing field cross-section in m^2.
-            Used to calculate `kappa` and `gamma_transit`. Default is 1e-6.
-        beam_diam : float, optonal 
-            Diameter of the probing field cross section in meters.
-            Used to calculate `gamma_transit`. If `None`, it is calculated from
-            `beam_area` assuming the beam cross-section is a circle. Default is `None`.
-        temp : float, optional
-            Temperature of the gas in Kelvin.
-            Used in calculations of enery level lifetime. Default is 300 K.
-
-        Raises
-        ------
-        ValueError
-            If at least two atomic states are not provided.
-        ValueError
-            If atom_flag is not one of ARC's supported alkali atoms.
-
-        """
-        if atom_flag not in ATOMS.keys():
-            raise ValueError(f"Atom flag must be one of {ATOMS.keys()}")
-
-        if len(atomic_states) < 2:
-            raise ValueError(("No states added to system. "
-                             "Specify at least two states of the form [n, l, j, m]"))
-
-        self.atom_flag = atom_flag
-        self.atom = ATOMS[atom_flag]()
-
-        self.cell_length = cell_length  # Default 0 to do optically thin sample
-        self.temp = temp  # K
-        self.beam_area = beam_area
-        self.density = self.atom.getNumberDensity(self.temp)
-        self.atom_mass = self.atom.mass
-
-        if beam_diam is None:
-            beam_diam = 2.0*np.sqrt(beam_area/np.pi)
-
-        self.beam_diameter = beam_diam
-
-        if gamma_transit is None:
-            gamma_transit = 1E-6*np.sqrt(8*Boltzmann*self.temp/(self.atom_mass*np.pi)
-                                         )/(self.beam_diameter/2*np.sqrt(2*np.log(2)))
-
-        super().__init__(0)
-
-        self._add_states(*atomic_states)
-
-        self.add_transit_broadening(gamma_transit)
-
-
-    def add_states(self):
-        """
-        Deprecated.
-        
-        Use \"atomic_state\" keyword argument of the constructor instead.
-        """
-        raise NotImplementedError(("Adding states after a cell has been created is "
-                                   "no longer supported. Please specify states with "
-                                   "the \"atomic_states\" keyword argument in the constructor."))
-
-
-    def _add_states(self, *states: QState) -> None:
-        """
-        Internal method to add states to the system and update internal variables
-        for energy and decay rates. 
-        
-        Quantum numbers and other states information are stored on the couplings graph nodes.
-        The first state added to the system is treated as the ground state,
-        and all "absolute energies" are calculated as a difference from ground.
-        Should only be called in :meth:`~.Cell.__init__`.
-
-        Parameters
-        ----------
-        *states : list[list[int or float]]
-            States that are added to the list of atomic states of interest for the cell.
-            Arguments should be lists of the form `[n, l, j, m]`, where n, l, j, and m
-            are the ususal quantum numbers describing the state: principal,
-            orbital, total angular momentum, and magnetic quantum numbers respectively.
-
-        """
-        for state in states:
-            node_info: dict = {"qnums": state}
-
-            # add energy to node
-            if self.basis_size == 0:
-                node_info["energy"] = 0
-            else:
-                ground_state = self.couplings.nodes[0]["qnums"]
-                # Mrad/s
-                node_info["energy"] = self.atom.getTransitionFrequency(*ground_state[:3],
-                                                                       *state[:3])*1e-6*2.0*np.pi
-
-            # add state lifetime to node
-            if self.basis_size == 0:
-                gamma_lifetime = 0
-            else:
-                gamma_lifetime = 1E-6/self.atom.getStateLifetime(*state[0:3])
-            node_info['gamma_lifetime'] = gamma_lifetime
-
-            self.couplings.add_node(self.basis_size, **node_info)
-
-            self.basis_size += 1
-
-        self._add_decay_to_graph()
-        self._get_probe_info()
-
-
-    def states_list(self) -> List[QState]:
-        """
-        Returns a list of quantum numbers for all states in the cell.
-
-        States position in the list will be in the order they were added,
-        and correspond to the density matrix values numbered with the same index.
-
-        Returns
-        -------
-        list[list]
-            List of quantum states of the form [n, l, j, m] that are stored
-            on graph nodes in the cell.
-
-        Examples
-        --------
-        >>> state1 = [50, 2, 2.5, 2.5] # states are written with quantum numbers [n, l, j, m] 
-        >>> state2 = [51, 2, 2.5, 2.5]
-        >>> cell = rq.Cell("Rb85", *rq.D2_states(5), state1, state2) #D2 states gets the states for the Rubidium 85 D2 line
-        >>> print(cell.states_list())
-        [[5, 0, 0.5, 0.5], [5, 1, 1.5, 0.5], [50, 2, 2.5, 2.5], [51, 2, 2.5, 2.5]]
-
-        """ # noqa
-        return [state[1] for state in self.couplings.nodes("qnums")]
-
-
-    def level_ordering(self) -> List[int]:
-        """
-        Return a list of the integer numbers of each state (*not* the quantum numbers) 
-        in descending order by energy order.
-
-        All energies are calculated with respect to the ground state energy, which is defined as 0.
-        Ground state is determined by the first state added to the system (state 0). Thus, state 0 
-        will always be last in the list.
-
-        Returns
-        -------
-        list[int]
-            The level numbers of the states in order of decending energy
-            relative to the ground state (state 0).
-
-        Examples
-        --------
-        For the following example, states are added to the cell in ascending
-        energy order, so the return reflects that, with the highest-energy state first.
-
-        >>> state1 = [50, 2, 2.5, 2.5]
-        >>> state2 = [51, 2, 2.5, 2.5]
-        >>> cell = rq.Cell("Rb85", *rq.D2_states("Rb85"), state1, state2) #uses the D2 line of Rb85
-        >>> print(cell.states_list())
-        >>> print(cell.level_ordering())
-        [[5, 0, 0.5, 0.5], [5, 1, 1.5, 0.5], [50, 2, 2.5, 2.5], [51, 2, 2.5, 2.5]]
-        [3, 2, 1, 0]
-
-        If we add `state1` and `state2` in the opposite order (thus switching
-        their positions in the states list), the level ordering will change since
-        `state2` is still a higher energy.
-
-        >>> state1 = [50, 2, 2.5, 2.5]
-        >>> state2 = [51, 2, 2.5, 2.5]
-        >>> cell = rq.Cell("Rb85", *rq.D2_states("Rb85"), state2, state1) #uses the D2 line of Rb85
-        >>> print(cell.states_list())
-        >>> print(cell.level_ordering())
-        [[5, 0, 0.5, 0.5], [5, 1, 1.5, 0.5], [51, 2, 2.5, 2.5], [50, 2, 2.5, 2.5]]
-        [2, 3, 1, 0]
-
-        """
-        energies = list(self.couplings.nodes("energy")).copy()
-        energies.sort(key=lambda val:val[1],reverse=True)
-        return [s[0] for s in energies]
-
-
-    def _get_probe_info(self, q_optical: Literal[-1,0,1] = 0) -> None:
-        """
-        Internal helper method to get information about the probing transition.
-
-        For this function, the probe transition is defined as the transition between
-        the ground state and first excited state.
-
-        Parameters
-        ----------
-        q_optical : int, optional
-            polarization of probing optical field in spherical basis. Must be -1, 0, 1.
-            Defaults to 0 for linear polarization.
-
-        """
-        gState = self.states_list()[0]
-        iState = self.states_list()[1]
-
-        self.probe_elem = self.atom.getDipoleMatrixElement(*gState, *iState, q_optical)
-        self.probe_freq = np.abs(self.atom.getTransitionFrequency(*gState[:3], *iState[:3]))
-
-        self.density = self.atom.getNumberDensity(self.temp)
-        self.kappa = calc_kappa(self.probe_freq, self.probe_elem, self.density)
-        self.eta = calc_eta(self.probe_freq, self.probe_elem, self.beam_area)
-
-
-    def decoherence_matrix(self) -> np.ndarray:
-        """
-        Get the decoherence matrix for a system.
-
-        This overload differs from :meth:`~Sensor.decoherence_matrix`
-        by including state lifetimes and decay rates calculated from arc rydberg without any
-        explicit definition of decoherence terms. In other words, it ensures that the
-        calculated decoherence terms match what is expected for a particular
-        real-world atom. 
-        
-        Returns
-        -------
-        numpy.ndarray
-            The decoherence matrix stack of the system.
-
-        """
-        # start with base gamma matrix from the transitions on graph
-        gamma = super().decoherence_matrix()
-
-        for state, lifetime in list(self.couplings.nodes(data="gamma_lifetime"))[1:]:
-
-            decay_sum = 0.0
-
-            for edge in self.couplings.out_edges(state):
-                decay_sum += self.couplings.edges[edge].get("gamma_transition", 0)
-
-            gamma[..., state, 0] += lifetime - decay_sum
-
-        return gamma
-
-
-    def _add_decay_to_graph(self) -> None:
-        """
-        Internal helper method to add population decay rates to the nodes to calculate gamma matrix.
-
-        1. add the state lifetime to each node
-        2. add the transition rate to each edge
-        
-        """
-        # First going to get absolute lifetimes of each state
-        states = self.level_ordering()
-
-        for index,state in enumerate(states):
-
-            qnum = self.couplings.nodes[state]["qnums"]
-
-            # Starts at 1, for the ground state, we want to avoid calculating decay
-            # loop over all couplings to get transition rates
-            for lower_state in states[index+1:]:
-                qnum_lower = self.couplings.nodes[lower_state]["qnums"]
-                try:
-                    gamma_transition = 1E-6*self.atom.getTransitionRate(*qnum[0:3],
-                                                                        *qnum_lower[0:3])
-                except ValueError:
-                    gamma_transition = 0
-
-                if gamma_transition != 0:
-                    self.add_decoherence((state, lower_state), gamma_transition, label="transition")
-
-
-    def add_coupling(
-            self, states: States, rabi_frequency: Optional[ScannableParameter] = None,
-            detuning: Optional[ScannableParameter] = None,
-            transition_frequency: Optional[float] = None,
-            phase: Optional[ScannableParameter] = 0, kvec: Tuple[float,float,float] = (0,0,0),
-            time_dependence: Optional[Callable[[float],float]] = None, label: Optional[str] = None,
-            e_field: Optional[ScannableParameter] = None, beam_power: Optional[float] = None,
-            beam_waist: Optional[float] = None,
-            q: Literal[-1, 0, 1] = 0,
-            **extra_kwargs) -> None:
-        """
-        Overload of :meth:`~.Sensor.add_coupling` which allows for different specification of
-        coupling fields which are more reflective of real experimental setups.
-
-        Rabi frequency is a mandatory argument in :class:`~.Sensor` but in :class:`~.Cell`, 
-        there are 3 options for laser power specification:
-
-        1. Explicit rabi-frequency definition identical to :class:`~.Sensor`.
-        2. Electric field strength, in V/m.
-        3. Specification of both beam power and beam waist.
-
-        Any one of these options can be used in place of the standard`rabi_frequency` argument
-        of :meth:`~.Sensor.add_coupling`.
-
-        As in :class:`~.Sensor`, if `detuning` is specified, the coupling is assumed
-        to act under the rotating-wave approximation (RWA), and `transition_frequency`
-        can not be specified. However, unlike in a :class:`~.Sensor`, if `detuning`
-        is not specified, in a :class:`~.cell.Cell`, `transition_frequency` will be 
-        calculated automatically based on atomic properties rather than taken as an argument.
-
-        Parameters
-        ----------
-        states: sequence
-            Length-2 list-like object (list or tuple) of integers
-            corresponding to the numbered states of the cell.
-        rabi_frequency: float, optional
-            The rabi frequency, in Mrad/s, of the coupling
-            field. If specified, `e_field`, `beam_power`, and `beam_waist` cannot
-            be specified.
-        detuning: float, optional
-            Field detuning, in Mrad/s, of a coupling
-            in the RWA. If specified, RWA is assumed, otherwise RWA not assumed,
-            and transition frequency will be calculated based on atomic properties.
-        phase: float, optional
-            The relative phase of the field in radians.
-            Defaults to zero.
-        kvec: sequence, optional
-            A three-element iterable that defines the
-            atomic doppler shift on a particular coupling field.
-            It should have magntiude equal to the doppler shift (in the units of Mrad/s)
-            of an atom moving at the Maxwell-Boltzmann distribution most probable
-            speed, `vP=np.sqrt(2*kB*T/m)`. I.E. `np.linalg.norm(kvec)=2*np.pi/lambda*vP`.
-            If equal to `(0,0,0)`, solvers will ignore doppler shifts
-            on this field.  Defaults to `(0,0,0)`.
-        time_dependence: scalar function, optional
-            A scalar function that
-            specifies a time-dependent field. The time dependence function
-            is defined as a funtion that returns a unitless value as a function
-            of time that is multiplied by the `rabi_frequency` parameter.
-        label: str, optional
-            The user-defined name of the coupling. This does not change
-            any calculations, but can be used to track individual couplings, and
-            will be reflected in the output of :meth:`~.Sensor.axis_labels`
-            Default None results in using the states tuple as the label.
-        e_field: float, optional
-            Electric field strenth of the coupling in Volts/meter.
-            If specified, `rabi_frequency`, `beam_power`, and `beam_waist` cannot
-            be specified.
-        beam_power: float, optional
-            Beam power in Watts.  If specified, `beam_waist`
-            must also be supplied, and `rabi_frequency` and `e_field` cannot
-            be specified. `beam_power` and `beam_waist` cannot be scanned simultaneously.
-        beam_waist: float, optional
-            1/e^2 Beam waist (radius) in units of
-            meters.  Only necessary when specifying `beam_power`.
-        q: int, optional
-            Coupling polarization in spherical basis.
-            Valid values are -1, 0, 1 for :math:`-\\sigma`, linear, :math:`+\\sigma`.
-            Default is 0 for linear.
-
-        Raises
-        ------
-        ValueError
-            If `states` is not a list-like of 2 integers.
-        ValueError
-            If an invalid combination of `rabi_frequency`, `e_field`,
-            `beam_power`, and `beam_waist` is provided.
-        ValueError
-            If `tranistion_frequency` is passed as an argument (it is
-            calculated from atomic properties).
-        ValueError
-            If `beam_power` and `beam_waist` are both sequences.
-
-        Notes
-        -----
-        .. note::
-            Note that while this function can be used directly just as in :class:`~.sensor.Sensor`,
-            it will often be called implicitly via :meth:`~.Sensor.add_couplings` which `Cell`
-            inherits. While they are equivalent, the second of these options is
-            often the more clear approach.
-            
-        .. note::
-            Specifying the beam power by beam parameters or electric field still computes
-            the `rabi_frequency` and adds that quantity to the `Cell` to maintain consistency across
-            `rydiqule`'s other calculations.
-            In other words, `beam_power`, `beam_waist`, and `e_field` will never appear
-            as quantities on the graph of a `Cell`.
-        
-        Examples
-        --------
-        In the simplest case, physical properties are calculated automatically in a `Cell`
-        All the familiar quantities are present, as well as many more.
-
-        >>> cell = rq.Cell("Rb85", *rq.D2_states("Rb85"))
-        >>> cell.add_coupling(states=(0,1), detuning=1, rabi_frequency=2)
-        >>> print(dict(cell.couplings.edges))
-        {(0, 0): {'gamma_transit': 0.41172855461658464, 'label': '(0,0)'}, (0, 1): {'rabi_frequency': 2, 'detuning': 1, 
-        'phase': 0, 'kvec': (0, 0, 0), 'label': '(0,1)'}, (1, 0): {'gamma_transition': 37.829349995476726, 
-        'label': '(1,0)', 'gamma_transit': 0.41172855461658464}}
-        
-        Here we see implicitly calling this overloaded function through :meth:`~.Sensor.add_couplings`.
-        
-        >>> cell = rq.Cell("Rb85", *rq.D2_states("Rb85"))
-        >>> c = {"states":(0,1), "detuning":1, "rabi_frequency":2}
-        >>> cell.add_couplings(c)
-        >>> print(dict(cell.couplings.edges))
-        {(0, 0): {'gamma_transit': 0.41172855461658464, 'label': '(0,0)'}, (0, 1): {'rabi_frequency': 2, 'detuning': 1, 
-        'phase': 0, 'kvec': (0, 0, 0), 'label': '(0,1)'}, (1, 0): {'gamma_transition': 37.829349995476726, 
-        'label': '(1,0)', 'gamma_transit': 0.41172855461658464}}
-
-        `e_field` can be specified in stead of `rabi_frequency`,
-        but a `rabi_frequency` will still be added to the system based on the `e_field`,
-        rather than `e_field` directly.
-        
-        >>> cell = rq.Cell("Rb85", *rq.D2_states("Rb85"))
-        >>> c = {"states":(0,1), "detuning":1, "e_field":6}
-        >>> cell.add_couplings(c)
-        >>> print(cell.couplings.edges(data='e_field'))
-        >>> print(cell.couplings.edges(data='rabi_frequency'))
-        [(0, 0, None), (0, 1, None), (1, 0, None)]
-        [(0, 0, None), (0, 1, -1.172912676105507), (1, 0, None)]
-        
-        As can `beam_power` and `beam_waist`,
-        with similar behavior regarding how information is stored.
-
-        >>> cell = rq.Cell("Rb85", *rq.D2_states("Rb85"))
-        >>> c = {"states":(0,1), "detuning":1, "beam_power":1, "beam_waist":1}
-        >>> cell.add_couplings(c)
-        >>> print(cell.couplings.edges(data='beam_power'))
-        >>> print(cell.couplings.edges(data='rabi_frequency'))
-        [(0, 0, None), (0, 1, None), (1, 0, None)]
-        [(0, 0, None), (0, 1, 4.28138982322625), (1, 0, None)]
-
-        """ # noqa
-        states = self._states_valid(states)
-        state1 = self.states_list()[states[0]]
-        state2 = self.states_list()[states[1]]
-        
-        suppress_dipole_warn = extra_kwargs.pop("suppress_dipole_warn", False)
-        
-        try:
-            dipole_moment = self.atom.getDipoleMatrixElement(*state1,*state2, q)
-        except ValueError:
-            msg = f"Transition between states {state1} and {state2} not electric-dipole allowed."\
-                "Solutions may be innacurate. "\
-                "Suppress this by passing \"suppress_dipole_warn=True\" to Cell.add_coupling"
-            dipole_moment = 0
-            if not suppress_dipole_warn:
-                warnings.warn(msg)
-        
-        if isinstance(e_field, list):
-            e_field = np.array(e_field)
-
-        if (e_field is not None
-            and beam_power is None
-            and beam_waist is None
-            and rabi_frequency is None
-            ):
-            passed_rabi = e_field*scale_dipole(dipole_moment)
-
-        elif (e_field is None
-              and beam_power is not None
-              and rabi_frequency is None
-              and beam_waist is not None
-              ):
-            if isinstance(beam_power, Sequence) and isinstance(beam_waist, Sequence):
-                raise ValueError('beam_power and beam_waist cannot be scanned simultaneously')
-            else:
-                passed_rabi = np.array([[1e-6*self.atom.getRabiFrequency(*state1, *state2[:-1],
-                                                                         q, bp, bw)
-                                        for bp in np.array(beam_power, ndmin=1)]
-                                        for bw in np.array(beam_waist, ndmin=1)]).squeeze()
-                if passed_rabi.shape == tuple():
-                    passed_rabi = float(passed_rabi)
-
-        elif (e_field is None and beam_power is None and rabi_frequency is not None):
-            passed_rabi = rabi_frequency
-
-        else:
-            msg = ("Please only define one of: 1) rabi_frequency or "
-                   "2) e_field or 3) beam_power and beam_waist.")
-            raise ValueError(msg)
-
-        if detuning is None:
-            if transition_frequency is not None:
-                msg = """Cell does not support explicit definietion of transition_frequency,
-                it is calculated based on atomic properties."""
-                raise ValueError(msg)
-            else:
-                transition_frequency = self.atom.getTransitionFrequency(*state2[:3],
-                                                                        *state1[:3])*1e-6*2.0*np.pi
-
-        super().add_coupling(states=states, rabi_frequency=passed_rabi,
-                             detuning=detuning, transition_frequency=transition_frequency,
-                             phase=phase, kvec=kvec, time_dependence=time_dependence, label=label,
-                             **extra_kwargs)
+"""
+Physical Cell objects for use in solvers.
+"""
+
+import scipy
+import numpy as np
+import warnings
+
+import scipy.constants
+from scipy.constants import Boltzmann
+
+# rydiqule imports
+from .sensor import Sensor, ScannableParameter
+from .sensor_utils import scale_dipole, calc_eta, calc_kappa
+from .atom_utils import ATOMS
+
+from typing import Literal, Optional, Sequence, List, Tuple, Union, Callable
+
+a0 = scipy.constants.physical_constants["Bohr radius"][0]
+
+AtomFlags = Literal['H', 'Li6', 'Li7', 'Na', 'K39', 'K40', 'K41', 'Rb85', 'Rb87', 'Cs']
+QState = Sequence  # TODO: consider using named tuples here
+States = Tuple[int, ...]
+
+
+class Cell(Sensor):
+    """
+    Subclass of :class:`~.Sensor` that creates a Sensor with additional physical properties
+    corresponding to a specific Rydberg atom.
+
+    In addition to the core functionality of `~.Sensor`, this class allows for labelling of states
+    with quantum numbers, calculating of state lifetimes and decoherences and tracking of
+    of some physical laser parameters. A key distictinction between a :class:`~.Cell` and a :class:`~.Sensor` is that
+    a cell supports (and requires) and absolute ordering of energy between states,
+    which allows for implicit calculation of decay rates an transition frequencies.
+
+    """
+
+    # these are not optional for a Cell
+    eta: float
+    kappa: float
+
+    def __init__(self, atom_flag: AtomFlags, *atomic_states: QState,
+                 gamma_transit: Optional[float] = None, cell_length: float = 0,
+                 beam_area: float = 1e-6, beam_diam: Optional[float] = None,
+                 temp: float = 300.0) -> None:
+        """
+        Initialize the Rydberg cell from the given parameters. 
+
+        Parameters
+        ----------
+        atom_flag : str 
+            Which atom is used in the cell for calculating physical properties with ARC Rydberg.
+            One of ['H', 'Li6', 'Li7', 'Na', 'K39', 'K40', 'K41', 'Rb85', 'Rb87', 'Cs'].
+        atomic_states : list[list]
+            List of states to be added to the cell. Each state is 
+            an iterable whose elements are each a list of the form [n, l, j, m], represnting the 
+            Rydberg atomic quantum numbers of the state. At least two states must be added so 
+            that the system is nontrivial. The number of states will determine the basis size
+            of the system. 
+        gamma_transit : float, optional
+            Decoherence due to atom transit through the optical
+            beams. Specified in units of Mrad/s. If `None`, will calculate based
+            on value of `beam_area`. See :meth:`~.Sensor.add_transit_broadening` for
+            details on how transit broadening is treated. Default is None.
+        beam_area : float, optional
+            Area of probing field cross-section in m^2.
+            Used to calculate `kappa` and `gamma_transit`. Default is 1e-6.
+        beam_diam : float, optonal 
+            Diameter of the probing field cross section in meters.
+            Used to calculate `gamma_transit`. If `None`, it is calculated from
+            `beam_area` assuming the beam cross-section is a circle. Default is `None`.
+        temp : float, optional
+            Temperature of the gas in Kelvin.
+            Used in calculations of enery level lifetime. Default is 300 K.
+
+        Raises
+        ------
+        ValueError
+            If at least two atomic states are not provided.
+        ValueError
+            If atom_flag is not one of ARC's supported alkali atoms.
+
+        """ #noqa
+        if atom_flag not in ATOMS.keys():
+            raise ValueError(f"Atom flag must be one of {ATOMS.keys()}")
+
+        if len(atomic_states) < 2:
+            raise ValueError(("No states added to system. "
+                             "Specify at least two states of the form [n, l, j, m]"))
+
+        self.atom_flag = atom_flag
+        self.atom = ATOMS[atom_flag]()
+
+        self.cell_length = cell_length  # Default 0 to do optically thin sample
+        self.temp = temp  # K
+        self.beam_area = beam_area
+        self.density = self.atom.getNumberDensity(self.temp)
+        self.atom_mass = self.atom.mass
+
+        if beam_diam is None:
+            beam_diam = 2.0*np.sqrt(beam_area/np.pi)
+
+        self.beam_diameter = beam_diam
+
+        if gamma_transit is None:
+            gamma_transit = 1E-6*np.sqrt(8*Boltzmann*self.temp/(self.atom_mass*np.pi)
+                                         )/(self.beam_diameter/2*np.sqrt(2*np.log(2)))
+
+        super().__init__(0)
+
+        self._add_states(*atomic_states)
+
+        self.add_transit_broadening(gamma_transit)
+
+
+    def add_states(self):
+        """
+        Deprecated.
+        
+        Use \"atomic_state\" keyword argument of the constructor instead.
+        """
+        raise NotImplementedError(("Adding states after a cell has been created is "
+                                   "no longer supported. Please specify states with "
+                                   "the \"atomic_states\" keyword argument in the constructor."))
+
+
+    def _add_states(self, *states: QState) -> None:
+        """
+        Internal method to add states to the system and update internal variables
+        for energy and decay rates. 
+        
+        Quantum numbers and other states information are stored on the couplings graph nodes.
+        The first state added to the system is treated as the ground state, and all "absolute energies"
+        are calculated as a difference from ground. Should only be called in :meth:`~.Cell.__init__`.
+
+        Parameters
+        ----------
+        *states : list[list[int or float]]
+            States that are added to the list of atomic states of interest for the cell.
+            Arguments should be lists of the form `[n, l, j, m]`, where n, l, j, and m
+            are the ususal quantum numbers describing the state: principal,
+            orbital, total angular momentum, and magnetic quantum numbers respectively.
+
+        """ #noqa
+        for state in states:
+            node_info: dict = {"qnums": state}
+
+            # add energy to node
+            if self.basis_size == 0:
+                node_info["energy"] = 0
+            else:
+                ground_state = self.couplings.nodes[0]["qnums"]
+                # Mrad/s
+                node_info["energy"] = self.atom.getTransitionFrequency(*ground_state[:3],
+                                                                       *state[:3])*1e-6*2.0*np.pi
+
+            # add state lifetime to node
+            if self.basis_size == 0:
+                gamma_lifetime = 0
+            else:
+                gamma_lifetime = 1E-6/self.atom.getStateLifetime(*state[0:3])
+            node_info['gamma_lifetime'] = gamma_lifetime
+
+            self.couplings.add_node(self.basis_size, **node_info)
+
+            self.basis_size += 1
+
+        self._add_decay_to_graph()
+        self._get_probe_info()
+
+
+    def states_list(self) -> List[QState]:
+        """
+        Returns a list of quantum numbers for all states in the cell.
+
+        States position in the list will be in the order they were added,
+        and correspond to the density matrix values numbered with the same index.
+
+        Returns
+        -------
+        list[list]
+            List of quantum states of the form [n, l, j, m] that are stored
+            on graph nodes in the cell.
+
+        Examples
+        --------
+        >>> state1 = [50, 2, 2.5, 2.5] # states are written with quantum numbers [n, l, j, m] 
+        >>> state2 = [51, 2, 2.5, 2.5]
+        >>> cell = rq.Cell("Rb85", *rq.D2_states(5), state1, state2) #D2 states gets the states for the Rubidium 85 D2 line
+        >>> print(cell.states_list())
+        [[5, 0, 0.5, 0.5], [5, 1, 1.5, 0.5], [50, 2, 2.5, 2.5], [51, 2, 2.5, 2.5]]
+
+        """ #noqa
+        return [state[1] for state in self.couplings.nodes("qnums")]
+
+
+    def level_ordering(self) -> List[int]:
+        """
+        Return a list of the integer numbers of each state (*not* the quantum numbers) 
+        in descending order by energy order.
+
+        All energies are calculated with respect to the ground state energy, which is defined as 0.
+        Ground state is determined by the first state added to the system (state 0). Thus, state 0 
+        will always be last in the list.
+
+        Returns
+        -------
+        list[int]
+            The level numbers of the states in order of decending energy
+            relative to the ground state (state 0).
+
+        Examples
+        --------
+        For the following example, states are added to the cell in ascending
+        energy order, so the return reflects that, with the highest-energy state first.
+
+        >>> state1 = [50, 2, 2.5, 2.5]
+        >>> state2 = [51, 2, 2.5, 2.5]
+        >>> cell = rq.Cell("Rb85", *rq.D2_states("Rb85"), state1, state2) #uses the D2 line of Rb85
+        >>> print(cell.states_list())
+        >>> print(cell.level_ordering())
+        [[5, 0, 0.5, 0.5], [5, 1, 1.5, 0.5], [50, 2, 2.5, 2.5], [51, 2, 2.5, 2.5]]
+        [3, 2, 1, 0]
+
+        If we add `state1` and `state2` in the opposite order (thus switching
+        their positions in the states list), the level ordering will change since
+        `state2` is still a higher energy.
+
+        >>> state1 = [50, 2, 2.5, 2.5]
+        >>> state2 = [51, 2, 2.5, 2.5]
+        >>> cell = rq.Cell("Rb85", *rq.D2_states("Rb85"), state2, state1) #uses the D2 line of Rb85
+        >>> print(cell.states_list())
+        >>> print(cell.level_ordering())
+        [[5, 0, 0.5, 0.5], [5, 1, 1.5, 0.5], [51, 2, 2.5, 2.5], [50, 2, 2.5, 2.5]]
+        [2, 3, 1, 0]
+
+        """ # noqa
+        energies = list(self.couplings.nodes("energy")).copy()
+        energies.sort(key=lambda val:val[1],reverse=True)
+        return [s[0] for s in energies]
+
+
+    def _get_probe_info(self, q_optical: Literal[-1,0,1] = 0) -> None:
+        """
+        Internal helper method to get information about the probing transition.
+
+        For this function, the probe transition is defined as the transition between
+        the ground state and first excited state.
+
+        Parameters
+        ----------
+        q_optical : int, optional
+            polarization of probing optical field in spherical basis. Must be -1, 0, 1.
+            Defaults to 0 for linear polarization.
+
+        """ #noqa
+        gState = self.states_list()[0]
+        iState = self.states_list()[1]
+
+        self.probe_elem = self.atom.getDipoleMatrixElement(*gState, *iState, q_optical)
+        self.probe_freq = np.abs(self.atom.getTransitionFrequency(*gState[:3], *iState[:3]))
+
+        self.density = self.atom.getNumberDensity(self.temp)
+        self.kappa = calc_kappa(self.probe_freq, self.probe_elem, self.density)
+        self.eta = calc_eta(self.probe_freq, self.probe_elem, self.beam_area)
+
+
+    def decoherence_matrix(self) -> np.ndarray:
+        """
+        Get the decoherence matrix for a system.
+
+        This overload differs from :meth:`~Sensor.decoherence_matrix`
+        by including state lifetimes and decay rates calculated from arc rydberg without any
+        explicit definition of decoherence terms. In other words, it ensures that the
+        calculated decoherence terms match what is expected for a particular
+        real-world atom. 
+        
+        Returns
+        -------
+        numpy.ndarray
+            The decoherence matrix stack of the system.
+
+        """
+        # start with base gamma matrix from the transitions on graph
+        gamma = super().decoherence_matrix()
+
+        for state, lifetime in list(self.couplings.nodes(data="gamma_lifetime"))[1:]:
+
+            decay_sum = 0.0
+
+            for edge in self.couplings.out_edges(state):
+                decay_sum += self.couplings.edges[edge].get("gamma_transition", 0)
+
+            gamma[..., state, 0] += lifetime - decay_sum
+
+        return gamma
+
+
+    def _add_decay_to_graph(self) -> None:
+        """
+        Internal helper method to add population decay rates to the nodes in order to calculate gamma matrix.
+
+        1. add the state lifetime to each node
+        2. add the transition rate to each edge
+        
+        """ #noqa
+        # First going to get absolute lifetimes of each state
+        states = self.level_ordering()
+
+        for index,state in enumerate(states):
+
+            qnum = self.couplings.nodes[state]["qnums"]
+
+            # Starts at 1, for the ground state, we want to avoid calculating decay
+            # loop over all couplings to get transition rates
+            for lower_state in states[index+1:]:
+                qnum_lower = self.couplings.nodes[lower_state]["qnums"]
+                try:
+                    gamma_transition = 1E-6*self.atom.getTransitionRate(*qnum[0:3],
+                                                                        *qnum_lower[0:3])
+                except ValueError:
+                    gamma_transition = 0
+
+                if gamma_transition != 0:
+                    self.add_decoherence((state, lower_state), gamma_transition, label="transition")
+
+
+    def add_coupling(
+            self, states: States, rabi_frequency: Optional[ScannableParameter] = None,
+            detuning: Optional[ScannableParameter] = None,
+            transition_frequency: Optional[float] = None,
+            phase: Optional[ScannableParameter] = 0, kvec: Tuple[float,float,float] = (0,0,0),
+            time_dependence: Optional[Callable[[float],float]] = None, label: Optional[str] = None,
+            e_field: Optional[ScannableParameter] = None, beam_power: Optional[float] = None,
+            beam_waist: Optional[float] = None,
+            q: Literal[-1, 0, 1] = 0,
+            **extra_kwargs) -> None:
+        """
+        Overload of :meth:`~.Sensor.add_coupling` which allows for different specification of
+        coupling fields which are more reflective of real experimental setups.
+
+        Rabi frequency is a mandatory argument in :class:`~.Sensor` but in :class:`~.Cell`, 
+        there are 3 options for laser power specification:
+
+        1. Explicit rabi-frequency definition identical to :class:`~.Sensor`.
+        2. Electric field strength, in V/m.
+        3. Specification of both beam power and beam waist.
+
+        Any one of these options can be used in place of the standard`rabi_frequency` argument
+        of :meth:`~.Sensor.add_coupling`.
+
+        As in :class:`~.Sensor`, if `detuning` is specified, the coupling is assumed
+        to act under the rotating-wave approximation (RWA), and `transition_frequency`
+        can not be specified. However, unlike in a :class:`~.Sensor`, if `detuning`
+        is not specified, in a :class:`~.cell.Cell`, `transition_frequency` will be 
+        calculated automatically based on atomic properties rather than taken as an argument.
+
+        Parameters
+        ----------
+        states: sequence
+            Length-2 list-like object (list or tuple) of integers
+            corresponding to the numbered states of the cell.
+        rabi_frequency: float, optional
+            The rabi frequency, in Mrad/s, of the coupling
+            field. If specified, `e_field`, `beam_power`, and `beam_waist` cannot
+            be specified.
+        detuning: float, optional
+            Field detuning, in Mrad/s, of a coupling
+            in the RWA. If specified, RWA is assumed, otherwise RWA not assumed,
+            and transition frequency will be calculated based on atomic properties.
+        phase: float, optional
+            The relative phase of the field in radians.
+            Defaults to zero.
+        kvec: sequence, optional
+            A three-element iterable that defines the
+            atomic doppler shift on a particular coupling field.
+            It should have magntiude equal to the doppler shift (in the units of Mrad/s)
+            of an atom moving at the Maxwell-Boltzmann distribution most probable
+            speed, `vP=np.sqrt(2*kB*T/m)`. I.E. `np.linalg.norm(kvec)=2*np.pi/lambda*vP`.
+            If equal to `(0,0,0)`, solvers will ignore doppler shifts
+            on this field.  Defaults to `(0,0,0)`.
+        time_dependence: scalar function, optional
+            A scalar function that
+            specifies a time-dependent field. The time dependence function
+            is defined as a funtion that returns a unitless value as a function
+            of time that is multiplied by the `rabi_frequency` parameter.
+        label: str, optional
+            The user-defined name of the coupling. This does not change
+            any calculations, but can be used to track individual couplings, and
+            will be reflected in the output of :meth:`~.Sensor.axis_labels`
+            Default None results in using the states tuple as the label.
+        e_field: float, optional
+            Electric field strenth of the coupling in Volts/meter.
+            If specified, `rabi_frequency`, `beam_power`, and `beam_waist` cannot
+            be specified.
+        beam_power: float, optional
+            Beam power in Watts.  If specified, `beam_waist`
+            must also be supplied, and `rabi_frequency` and `e_field` cannot
+            be specified. `beam_power` and `beam_waist` cannot be scanned simultaneously.
+        beam_waist: float, optional
+            1/e^2 Beam waist (radius) in units of
+            meters.  Only necessary when specifying `beam_power`.
+        q: int, optional
+            Coupling polarization in spherical basis.
+            Valid values are -1, 0, 1 for :math:`-\\sigma`, linear, :math:`+\\sigma`.
+            Default is 0 for linear.
+
+        Raises
+        ------
+        ValueError
+            If `states` is not a list-like of 2 integers.
+        ValueError
+            If an invalid combination of `rabi_frequency`, `e_field`,
+            `beam_power`, and `beam_waist` is provided.
+        ValueError
+            If `tranistion_frequency` is passed as an argument (it is
+            calculated from atomic properties).
+        ValueError
+            If `beam_power` and `beam_waist` are both sequences.
+
+        Notes
+        -----
+        .. note::
+            Note that while this function can be used directly just as in :class:`~.sensor.Sensor`, it will often
+            be called implicitly via :meth:`~.Sensor.add_couplings` which `Cell`
+            inherits. While they are equivalent, the second of these options is
+            often the more clear approach.
+            
+        .. note::
+            Specifying the beam power by beam parameters or electric field still computes the `rabi_frequency` and
+            adds that quantity to the `Cell` to maintain consistency across `rydiqule`'s other calculations. In other
+            words, `beam_power`, `beam_waist`, and `e_field` will never appear as quantities on the graph of a `Cell`.
+        
+        Examples
+        --------
+        In the simplest case, it is clear physical properties are calculated automatically in a `Cell`
+        All the familiar quantities are present, as well as many more.
+
+        >>> cell = rq.Cell("Rb85", *rq.D2_states("Rb85"))
+        >>> cell.add_coupling(states=(0,1), detuning=1, rabi_frequency=2)
+        >>> print(dict(cell.couplings.edges))
+        {(0, 0): {'gamma_transit': 0.41172855461658464, 'label': '(0,0)'}, (0, 1): {'rabi_frequency': 2, 'detuning': 1, 
+        'phase': 0, 'kvec': (0, 0, 0), 'label': '(0,1)'}, (1, 0): {'gamma_transition': 37.829349995476726, 
+        'label': '(1,0)', 'gamma_transit': 0.41172855461658464}}
+        
+        Here we see implicitly calling this overloaded function through :meth:`~.Sensor.add_couplings`.
+        
+        >>> cell = rq.Cell("Rb85", *rq.D2_states("Rb85"))
+        >>> c = {"states":(0,1), "detuning":1, "rabi_frequency":2}
+        >>> cell.add_couplings(c)
+        >>> print(dict(cell.couplings.edges))
+        {(0, 0): {'gamma_transit': 0.41172855461658464, 'label': '(0,0)'}, (0, 1): {'rabi_frequency': 2, 'detuning': 1, 
+        'phase': 0, 'kvec': (0, 0, 0), 'label': '(0,1)'}, (1, 0): {'gamma_transition': 37.829349995476726, 
+        'label': '(1,0)', 'gamma_transit': 0.41172855461658464}}
+
+        `e_field` can be specified in stead of `rabi_frequency`, but a `rabi_frequency` will still be added
+        to the system based on the `e_field`, rather than `e_field` directly.
+        
+        >>> cell = rq.Cell("Rb85", *rq.D2_states("Rb85"))
+        >>> c = {"states":(0,1), "detuning":1, "e_field":6}
+        >>> cell.add_couplings(c)
+        >>> print(cell.couplings.edges(data='e_field'))
+        >>> print(cell.couplings.edges(data='rabi_frequency'))
+        [(0, 0, None), (0, 1, None), (1, 0, None)]
+        [(0, 0, None), (0, 1, -1.172912676105507), (1, 0, None)]
+        
+        As can `beam_power` and `beam_waist`, with similar behavior regarding how information is stored.
+
+        >>> cell = rq.Cell("Rb85", *rq.D2_states("Rb85"))
+        >>> c = {"states":(0,1), "detuning":1, "beam_power":1, "beam_waist":1}
+        >>> cell.add_couplings(c)
+        >>> print(cell.couplings.edges(data='beam_power'))
+        >>> print(cell.couplings.edges(data='rabi_frequency'))
+        [(0, 0, None), (0, 1, None), (1, 0, None)]
+        [(0, 0, None), (0, 1, 4.28138982322625), (1, 0, None)]
+
+        """ # noqa
+        states = self._states_valid(states)
+        state1 = self.states_list()[states[0]]
+        state2 = self.states_list()[states[1]]
+        
+        suppress_dipole_warn = extra_kwargs.pop("suppress_dipole_warn", False)
+        
+        try:
+            dipole_moment = self.atom.getDipoleMatrixElement(*state1,*state2, q)
+        except ValueError:
+            msg = f"Transition between states {state1} and {state2} not electric-dipole allowed."\
+                "Solutions may be innacurate. "\
+                "Suppress this by passing \"suppress_dipole_warn=True\" to Cell.add_coupling"
+            dipole_moment = 0
+            if not suppress_dipole_warn:
+                warnings.warn(msg)
+        
+        if isinstance(e_field, list):
+            e_field = np.array(e_field)
+
+        if (e_field is not None and beam_power is None and beam_waist is None and rabi_frequency is None):
+            passed_rabi = e_field*scale_dipole(dipole_moment)
+
+        elif (e_field is None and beam_power is not None and rabi_frequency is None and beam_waist is not None):  # noqa
+            if isinstance(beam_power, Sequence) and isinstance(beam_waist, Sequence):
+                raise ValueError('beam_power and beam_waist cannot be scanned simultaneously')
+            else:
+                passed_rabi = np.array([[1e-6*self.atom.getRabiFrequency(*state1, *state2[:-1], q, bp, bw)
+                                        for bp in np.array(beam_power, ndmin=1)]
+                                        for bw in np.array(beam_waist, ndmin=1)]).squeeze()
+                if passed_rabi.shape == tuple():
+                    passed_rabi = float(passed_rabi)
+
+        elif (e_field is None and beam_power is None and rabi_frequency is not None):
+            passed_rabi = rabi_frequency
+
+        else:
+            msg = ("Please only define one of: 1) rabi_frequency or "
+                   "2) e_field or 3) beam_power and beam_waist.")
+            raise ValueError(msg)
+
+        if detuning is None:
+            if transition_frequency is not None:
+                msg = """Cell does not support explicit definietion of transition_frequency,
+                it is calculated based on atomic properties."""
+                raise ValueError(msg)
+            else:
+                transition_frequency = self.atom.getTransitionFrequency(*state2[:3],
+                                                                        *state1[:3])*1e-6*2.0*np.pi
+
+        super().add_coupling(states=states, rabi_frequency=passed_rabi,
+                             detuning=detuning, transition_frequency=transition_frequency,
+                             phase=phase, kvec=kvec, time_dependence=time_dependence, label=label,
+                             **extra_kwargs)
```

### Comparing `rydiqule-1.0.0/src/rydiqule/doppler_utils.py` & `rydiqule-1.0.0rc2/src/rydiqule/doppler_utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,400 +1,400 @@
-"""
-Utilities for implementing Doppler averaging
-"""
-
-import numpy as np
-from scipy import special
-
-from .sensor_utils import _hamiltonian_term, make_real, remove_ground
-
-from typing import Tuple, Optional, TypedDict, Union, Literal, Sequence
-
-
-class UniformMethod(TypedDict, total=False):
-    method: Literal['uniform']
-    width_doppler: float
-    n_uniform: int
-
-
-class IsoPopMethod(TypedDict, total=False):
-    method: Literal['isopop']
-    n_isopop: int
-
-
-class SplitMethod(TypedDict, total=False):
-    method: Literal['split']
-    width_doppler: float
-    n_doppler: int
-    width_coherent: float
-    n_coherent: int
-
-
-class DirectMethod(TypedDict, total=False):
-    method: Literal['direct']
-    doppler_velocities: Union[np.ndarray, Sequence]
-
-
-MeshMethod = Union[UniformMethod, SplitMethod, DirectMethod]
-
-
-def get_doppler_equations(base_eoms: np.ndarray,
-                          doppler_hamiltonians: np.ndarray, Vs: np.ndarray) -> np.ndarray:
-    """
-    Returns the equations for each slice of the doppler profile.
-
-    A new axes corresponding to these slices are appended to the beginning.
-    For example, if equations are of shape `(m,m)`
-    and there are `n_doppler` doppler values being sampled,
-    the return will be of shape `(n_doppler, m, m)`.
-
-    Parameters
-    ----------
-    base_eoms : numpy.ndarray
-        Stacked square arrays representing the unshifted equations,
-        i.e. the theoretical equations for an ensemble of atoms with zero momentum.
-    doppler_hamiltonians : numpy.ndarray
-        Arrays of hamiltonians with only doppler shifts present.
-        One for each spatial dimension needed.
-        See :meth:`~.Sensor.get_doppler_shifts` for details.
-    Vs : numpy.ndarray
-        Mesh of velocity classes to sample,
-        with same spatial dimensions as `dop_ham`.
-        See :func:`~.doppler_mesh` for details.
-
-    Returns
-    -------
-    numpy.ndarray
-        An array of shape `(*Vs.shape[1:], *base_eoms.shape)` which is a,
-        potentially multi-dimensional, stack of individual equations of shape `(m, m)`.
-        Each slice of this stack is an equation of shape `(m, m)`
-        with the corresponding doppler shifts applied.
-
-    Note
-    ----
-    Each doppler shift is equal to `k_i*vP*det_i`, in units of Mrad/s,
-    where `i` denotes the einstein summation along the spatial dimensions.
-    `det` is the normalized velocity class, with `vP*det_i=v_i` giving the velocity.
-    `vP` is the most probable speed from the Maxwell-Boltzmann distribution:
-    sqrt(2*kB*T/m).
-    `k_i` is the k-vector of the field along the same axis as `det_i`.
-    `doppler_hamiltonians` provides `k_i*vP`, `Vs` provides `det_i`.
-
-    """
-    base_doppler_shift_eoms = generate_doppler_shift_eom(doppler_hamiltonians)
-    # take outer product of velocities and base kvec eoms to get detunings.
-    # Add shifts from each spatial dimension to each detuning
-    doppler_shift_eoms = np.tensordot(Vs, base_doppler_shift_eoms, ((0),(0)))
-    # broadcast up base_eom to add doppler shift dims
-    # broadcast up doppler_shift_eoms to add base_eom stack dimensions
-    n_stacks = len(base_eoms.shape[:-2])
-    spatial_dim = base_doppler_shift_eoms.shape[0]
-    exp_dims = tuple(range(spatial_dim, spatial_dim+n_stacks))
-    doppler_eqns = np.expand_dims(base_eoms, 0) + np.expand_dims(doppler_shift_eoms, exp_dims)
-
-    return doppler_eqns
-
-
-def generate_doppler_shift_eom(doppler_hamiltonians: np.ndarray) -> np.ndarray:
-    """doppler_mesh_method
-    Generates the EOMs for the supplied doppler shifts.
-
-    Multiply the output by the velocity in each dimension,
-    then add to the normal EOMs to get the full Doppler shifted EOMs.
-
-    Parameters
-    ----------
-    doppler_hamiltonians : numpy.ndarray
-        Hamiltonians of only the doppler shifts,
-        one for each spatial dimension to be averaged over.
-
-    Returns
-    -------
-    numpy.ndarray
-        Corresponding LHS EOMs with ground removed and in the real basis.
-
-    """
-    obes = _hamiltonian_term(doppler_hamiltonians)
-    obes, const = remove_ground(obes)
-    doppler_shift_obes = make_real(obes, const)[0]
-
-    return doppler_shift_obes
-
-
-def gaussian3d(Vs: np.ndarray) -> np.ndarray:
-    """
-    Evaluate a multi-dimensional gaussian, with sigma=1, for the given detunings.
-
-    Parameters
-    ----------
-    Vs : numpy.ndarray
-        Array of normalized velocity classes for which to get
-        the gaussian weighting.
-
-    Returns
-    -------
-    numpy.ndarray
-        Gaussian weights for the velocity classes.
-        Has same shape as `Vs`.
-
-    """
-    spatial_dim = Vs.shape[0]
-    if spatial_dim > 3:
-        raise ValueError(f"Too many axes supplied: {spatial_dim}")
-
-    prefactor = np.power(1/(np.pi),spatial_dim*0.5)
-
-    return prefactor*np.exp(-np.square(Vs).sum(axis=0))
-
-
-def doppler_classes(method: Optional[MeshMethod] = None
-                    ) -> np.ndarray:
-    """
-    Defines which velocity classes to sample for doppler averaging.
-
-    These are defined in units of the gaussian width sigma of the Maxwell-Boltzmann
-    distribution.
-
-    Note: To avoid issues, optical detunings should not leave densely sampled velocity classes.
-    To avoid artifacts, the density of points should provide >~10 points over the
-    narrowest absorptive feature. The default is a decent first guess, but for many
-    problems the sampling mesh should be adjusted.
-
-    Parameters
-    ----------
-    method : dict
-        Specifies method to use and any control parameters.
-        Must contain the key `"method"` with one of the following options.
-        Each method has suboptions that also need to be specified.
-        Valid options are:
-
-            - `"uniform"`: Defines a uniformly spaced, dense grid.
-              Configuration parameters include:
-
-                - `"width_doppler"`: Float that specifies one-sided width of gaussian
-                  distributionto average over, in units of sigma. Defaults to 2.0.
-                - `"n_uniform"`: Int that specifies how many points to use. Defaults to 1601.
-
-            - `"isopop"`: Defines a grid with uniform population in each interval.
-              This method highly emphasises physics happening near the 0 velocity class.
-              If stuff is happening for non-zero velocity classes,
-              it is likely to alias it unless `n_isopop` is large.
-              See Ref [1]_ for details.
-              Configuration parameters include:
-
-                - `"n_isopop"`: Int that specifies how many points to use. Defaults to 400.
-
-            - `"split"`: Defines a grid with a dense central spacing and wide spacing wings.
-              This method provides a decent compromise between uniform and isopop.
-              It uses fewer points than uniform, but also works well for non-zero velocity class
-              models (like Autler-Townes splittings).
-              This is the default meshing method.
-              Configuration parameters include:
-
-              - `"width_doppler"`: Float that specifies one-sided width of coarse grided portion
-                of the gaussian distribution.
-                Units are in sigma. Defaults to 2.0.
-              - `"width_coherent"`: Float that specifies one-sided width of fine grided portion
-                of gaussian distribution. Units are in sigma. Defaults to 0.4.
-              - `"n_doppler"`: Int that specifies how many points to use for the coarse grid.
-                Note that points of the coarse grid that fall within the fine grid are
-                dropped. Default is 201.
-              - `"n_coherent"`: Int that specifies how many points to use for the fine grid.
-                Default is 401.
-
-              .. note::
-                Note that for the "split" method, a union of 2 samplings is taken,
-                so the number of total points will not necessary be equal to the sum
-                of `"n_coherent"` and `"n_doppler"`.
-
-            - `"direct"`: Use the supplied 1-D numpy array to build the mesh.
-
-              - `"doppler_velocities"`: Mandatory parameter that holds the 1-D numpy array
-                to use when building the mesh grids.
-
-    Returns
-    -------
-    numpy.ndarray
-        1-D array of velocities to be sampled.
-
-    Examples
-    --------
-    The defaults will sample more densely near the center of the distribution,
-    (the "split" method) with a total of 561 classes.
-
-    >>> classes = rq.doppler_classes() #use the default values
-    >>> print(classes.shape)
-    (561,)
-
-    Specifying "uniform" with no additional arguments produces 1601 evenly spaced
-    classes by default.
-
-    >>> m = {"method":"uniform"}
-    >>> classes = rq.doppler_classes(method=m)
-    >>> print(classes.shape)
-    (1601,)
-
-    Further specifying the number of points allows more dense or sparse sampling
-    of the velocity distribution.
-
-    >>> m = {"method":"uniform", "n_uniform":801}
-    >>> classes = rq.doppler_classes(method=m)
-    >>> print(classes.shape)
-    (801,)
-
-    The "split" method also has further specifications
-
-    >>> m = {"method":"split", "n_coherent":301, "n_doppler":501}
-    >>> classes = rq.doppler_classes(method=m)
-    >>> print(classes.shape)
-    (701,)
-
-    References
-    ----------
-    .. [1] Andrew P. Rotunno, et. al.
-        Inverse Transform Sampling for Efficient Doppler-Averaged Spectroscopy Simulation,
-        arXiv:2304.12468 (2023)
-        http://arxiv.org/abs/2304.12468
-
-    """
-    if method is None:
-        method = SplitMethod(method="split")
-
-    assert method is not None
-    implemented_methods = ["uniform","isopop","split","direct"]
-    try:
-        if method["method"] not in implemented_methods:
-            raise ValueError(f"Method {method['method']} is not a recognized meshing method.")
-    except KeyError:
-        raise KeyError("Meshing method must be a dictionary with at least key 'method'")
-
-    if method["method"] == "uniform":
-        # use default options if not provided
-        width_doppler = method.get("width_doppler",2.0)
-        n_uniform = method.get("n_uniform",1601)
-        doppler_velocities = np.linspace(-width_doppler,width_doppler,n_uniform)
-    elif method["method"] == "isopop":
-        # define such that each slice has equal population distribution
-        n_isopop = method.get("n_isopop", 400)
-        bin_edges = np.linspace(0, 1.0, n_isopop+1)
-        bin_centers = (bin_edges - bin_edges[1]/2)[1:]
-        doppler_velocities = special.erfinv(2*bin_centers-1)*np.sqrt(2)
-    elif method["method"] == "split":
-        # use default options if not provided
-        width_doppler = method.get("width_doppler",2.0)
-        width_coherent = method.get("width_coherent",0.4)
-        n_doppler = method.get("n_doppler",201)
-        n_coherent = method.get("n_coherent",401)
-        # Doppler shifts to sample
-        range_doppler = np.linspace(-width_doppler,width_doppler,n_doppler)
-        # Finer mesh near zero velocity class where coherent stuff is happening
-        range_coherent = np.linspace(-width_coherent,width_coherent,n_coherent)
-        # Combine and get deltas for calculating the lazy integral
-        # mask out points from course grid where fine grid is, avoids aliasing artifacts
-        doppler_velocities = np.union1d(range_doppler[np.abs(range_doppler) > width_coherent],
-                                        range_coherent)
-    elif method["method"] == "direct":
-        try:
-            doppler_velocities = method["doppler_velocities"]  # type: ignore[assignment]
-        except KeyError:
-            raise KeyError("Method 'direct' must specify a 'doppler_velocities' config parameter")
-        if not isinstance(doppler_velocities,np.ndarray):
-            doppler_velocities = np.array(doppler_velocities)  # type: ignore[unreachable]
-        # ensure numpy array, then assert shape is 1-D
-        assert len(doppler_velocities.shape) == 1, "doppler_velocities must be 1-D"
-
-    return doppler_velocities
-
-
-def doppler_mesh(doppler_velocities: np.ndarray, spatial_dim: int) -> Tuple[np.ndarray, np.ndarray]:
-    """
-    Creates meshgrids of evaluation points and point "volumes" for doppler averaging.
-
-    Parameters
-    ----------
-    dop_velocities : numpy.ndarray
-        A 1-D array of velocities to evaluate over.
-        These should be normalized to the most probable velocity used by
-        :func:`gaussian3d`.
-    spatial_dim : int
-        Number of spatial dimensions to grid over.
-
-    Returns
-    -------
-    Vs : numpy.ndarray
-        Velocity evaluation points array of shape `(spatial_dim,spatial_dim*[len(dop_vel)])`.
-    Vols : numpy.ndarray
-        "Volume" of each meshpoint. Has same shape as `Vs`.
-
-    Examples
-    --------
-    >>> m = {"method":"uniform", "n_uniform":801}
-    >>> classes = rq.doppler_classes(method=m)
-    >>> mesh, vols = rq.doppler_mesh(classes, 2)
-    >>> print(type(mesh), type(vols))
-    >>> mesh_np = np.array(mesh)
-    >>> vols_np = np.array(vols)
-    >>> print(mesh_np.shape, vols_np.shape)
-    <class 'numpy.ndarray'> <class 'numpy.ndarray'>
-    (2, 801, 801) (2, 801, 801)
-
-    """
-    dop_volumes = np.gradient(doppler_velocities)  # smoothly handles irregular arrays
-    # generate the velocity meshgrids
-    dets = [doppler_velocities for _ in range(spatial_dim)]
-    diffs = [dop_volumes for _ in range(spatial_dim)]
-    Vs = np.array(np.meshgrid(*dets,indexing="ij"))
-    Vols = np.array(np.meshgrid(*diffs,indexing="ij"))
-
-    return Vs, Vols
-
-
-def apply_doppler_weights(sols: np.ndarray,
-                          velocities: np.ndarray, volumes: np.ndarray) -> np.ndarray:
-    """
-    Calculates and applies the weight for each doppler class given unweighted solutions
-    to doppler-shifted equations.
-
-    Works for both time-domain and stead-states solutions.
-
-    Parameters
-    ----------
-    sols : numpy.ndarray
-        The array of solutions over which to calculate weights.
-    velocities : numpy.ndarray
-        Array of shape `(n_dim, *n_dop)` where n_dim
-        is the number of dimensions over which doppler shifts are being considered
-        and `*n_dop` is a number of axes equal to n_dim with length equal to the number
-        of doppler velocity classes which are being considered. The values correspond
-        the velocity class in units of sigma.
-    volumes : numpy.ndarray
-        Array of shape equal to `velocities`.
-        The values correspond to the spacings between doppler classes on each axis.
-
-    Returns
-    -------
-    numpy.ndarray
-        The weighted solution array of shape equal to that of `sols`.
-
-    Raises
-    ------
-    ValueError
-        If the shapes of `velocities` and `volumes` do not match.
-
-    """
-    spatial_dim = volumes.shape[0]
-
-    if volumes.shape != velocities.shape:
-        raise ValueError((f"velocity shape {velocities.shape} does not match "
-                         f"volume shape {volumes.shape}"))
-
-    weights = gaussian3d(velocities)
-    volumes = np.prod(volumes, axis=0)
-
-    # calculate axes to append for array broadcasting to work in return
-    solution_dim = len(sols.shape) - spatial_dim
-    expand_axes = tuple(-1*np.arange(solution_dim)-1)
-
-    weights = np.expand_dims(weights, expand_axes)
-    volumes = np.expand_dims(volumes, expand_axes)
-
-    return weights*volumes*sols
+"""
+Utilities for implementing Doppler averaging
+"""
+
+import numpy as np
+from scipy import special
+
+from .sensor_utils import _hamiltonian_term, make_real, remove_ground
+
+from typing import Tuple, Optional, TypedDict, Union, Literal, Sequence
+
+
+class UniformMethod(TypedDict, total=False):
+    method: Literal['uniform']
+    width_doppler: float
+    n_uniform: int
+
+
+class IsoPopMethod(TypedDict, total=False):
+    method: Literal['isopop']
+    n_isopop: int
+
+
+class SplitMethod(TypedDict, total=False):
+    method: Literal['split']
+    width_doppler: float
+    n_doppler: int
+    width_coherent: float
+    n_coherent: int
+
+
+class DirectMethod(TypedDict, total=False):
+    method: Literal['direct']
+    doppler_velocities: Union[np.ndarray, Sequence]
+
+
+MeshMethod = Union[UniformMethod, SplitMethod, DirectMethod]
+
+
+def get_doppler_equations(base_eoms: np.ndarray,
+                          doppler_hamiltonians: np.ndarray, Vs: np.ndarray) -> np.ndarray:
+    """
+    Returns the equations for each slice of the doppler profile.
+
+    A new axes corresponding to these slices are appended to the beginning.
+    For example, if equations are of shape `(m,m)`
+    and there are `n_doppler` doppler values being sampled,
+    the return will be of shape `(n_doppler, m, m)`.
+
+    Parameters
+    ----------
+    base_eoms : numpy.ndarray
+        Stacked square arrays representing the unshifted equations,
+        i.e. the theoretical equations for an ensemble of atoms with zero momentum.
+    doppler_hamiltonians : numpy.ndarray
+        Arrays of hamiltonians with only doppler shifts present.
+        One for each spatial dimension needed.
+        See :meth:`~.Sensor.get_doppler_shifts` for details.
+    Vs : numpy.ndarray
+        Mesh of velocity classes to sample,
+        with same spatial dimensions as `dop_ham`.
+        See :func:`~.doppler_mesh` for details.
+
+    Returns
+    -------
+    numpy.ndarray
+        An array of shape `(*Vs.shape[1:], *base_eoms.shape)` which is a,
+        potentially multi-dimensional, stack of individual equations of shape `(m, m)`.
+        Each slice of this stack is an equation of shape `(m, m)`
+        with the corresponding doppler shifts applied.
+
+    Note
+    ----
+    Each doppler shift is equal to `k_i*vP*det_i`, in units of Mrad/s,
+    where `i` denotes the einstein summation along the spatial dimensions.
+    `det` is the normalized velocity class, with `vP*det_i=v_i` giving the velocity.
+    `vP` is the most probable speed from the Maxwell-Boltzmann distribution:
+    sqrt(2*kB*T/m).
+    `k_i` is the k-vector of the field along the same axis as `det_i`.
+    `doppler_hamiltonians` provides `k_i*vP`, `Vs` provides `det_i`.
+
+    """
+    base_doppler_shift_eoms = generate_doppler_shift_eom(doppler_hamiltonians)
+    # take outer product of velocities and base kvec eoms to get detunings.
+    # Add shifts from each spatial dimension to each detuning
+    doppler_shift_eoms = np.tensordot(Vs, base_doppler_shift_eoms, ((0),(0)))
+    # broadcast up base_eom to add doppler shift dims
+    # broadcast up doppler_shift_eoms to add base_eom stack dimensions
+    n_stacks = len(base_eoms.shape[:-2])
+    spatial_dim = base_doppler_shift_eoms.shape[0]
+    exp_dims = tuple(range(spatial_dim, spatial_dim+n_stacks))
+    doppler_eqns = np.expand_dims(base_eoms, 0) + np.expand_dims(doppler_shift_eoms, exp_dims)
+
+    return doppler_eqns
+
+
+def generate_doppler_shift_eom(doppler_hamiltonians: np.ndarray) -> np.ndarray:
+    """doppler_mesh_method
+    Generates the EOMs for the supplied doppler shifts.
+
+    Multiply the output by the velocity in each dimension,
+    then add to the normal EOMs to get the full Doppler shifted EOMs.
+
+    Parameters
+    ----------
+    doppler_hamiltonians : numpy.ndarray
+        Hamiltonians of only the doppler shifts,
+        one for each spatial dimension to be averaged over.
+
+    Returns
+    -------
+    numpy.ndarray
+        Corresponding LHS EOMs with ground removed and in the real basis.
+
+    """
+    obes = _hamiltonian_term(doppler_hamiltonians)
+    obes, const = remove_ground(obes)
+    doppler_shift_obes = make_real(obes, const)[0]
+
+    return doppler_shift_obes
+
+
+def gaussian3d(Vs: np.ndarray) -> np.ndarray:
+    """
+    Evaluate a multi-dimensional gaussian, with sigma=1, for the given detunings.
+
+    Parameters
+    ----------
+    Vs : numpy.ndarray
+        Array of normalized velocity classes for which to get
+        the gaussian weighting.
+
+    Returns
+    -------
+    numpy.ndarray
+        Gaussian weights for the velocity classes.
+        Has same shape as `Vs`.
+
+    """
+    spatial_dim = Vs.shape[0]
+    if spatial_dim > 3:
+        raise ValueError(f"Too many axes supplied: {spatial_dim}")
+
+    prefactor = np.power(1/(np.pi),spatial_dim*0.5)
+
+    return prefactor*np.exp(-np.square(Vs).sum(axis=0))
+
+
+def doppler_classes(method: Optional[MeshMethod] = None
+                    ) -> np.ndarray:
+    """
+    Defines which velocity classes to sample for doppler averaging.
+
+    These are defined in units of the gaussian width sigma of the Maxwell-Boltzmann
+    distribution.
+
+    Note: To avoid issues, optical detunings should not leave densely sampled velocity classes.
+    To avoid artifacts, the density of points should provide >~10 points over the
+    narrowest absorptive feature. The default is a decent first guess, but for many
+    problems the sampling mesh should be adjusted.
+
+    Parameters
+    ----------
+    method : dict
+        Specifies method to use and any control parameters.
+        Must contain the key `"method"` with one of the following options.
+        Each method has suboptions that also need to be specified.
+        Valid options are:
+
+            - `"uniform"`: Defines a uniformly spaced, dense grid.
+              Configuration parameters include:
+
+                - `"width_doppler"`: Float that specifies one-sided width of gaussian
+                  distributionto average over, in units of sigma. Defaults to 2.0.
+                - `"n_uniform"`: Int that specifies how many points to use. Defaults to 1601.
+
+            - `"isopop"`: Defines a grid with uniform population in each interval.
+              This method highly emphasises physics happening near the 0 velocity class.
+              If stuff is happening for non-zero velocity classes,
+              it is likely to alias it unless `n_isopop` is large.
+              See Ref [1]_ for details.
+              Configuration parameters include:
+
+                - `"n_isopop"`: Int that specifies how many points to use. Defaults to 400.
+
+            - `"split"`: Defines a grid with a dense central spacing and wide spacing wings.
+              This method provides a decent compromise between uniform and isopop.
+              It uses fewer points than uniform, but also works well for non-zero velocity class
+              models (like Autler-Townes splittings).
+              This is the default meshing method.
+              Configuration parameters include:
+
+              - `"width_doppler"`: Float that specifies one-sided width of coarse grided portion
+                of the gaussian distribution.
+                Units are in sigma. Defaults to 2.0.
+              - `"width_coherent"`: Float that specifies one-sided width of fine grided portion
+                of gaussian distribution. Units are in sigma. Defaults to 0.4.
+              - `"n_doppler"`: Int that specifies how many points to use for the coarse grid.
+                Note that points of the coarse grid that fall within the fine grid are
+                dropped. Default is 201.
+              - `"n_coherent"`: Int that specifies how many points to use for the fine grid.
+                Default is 401.
+
+              .. note::
+                Note that for the "split" method, a union of 2 samplings is taken,
+                so the number of total points will not necessary be equal to the sum
+                of `"n_coherent"` and `"n_doppler"`.
+
+            - `"direct"`: Use the supplied 1-D numpy array to build the mesh.
+
+              - `"doppler_velocities"`: Mandatory parameter that holds the 1-D numpy array
+                to use when building the mesh grids.
+
+    Returns
+    -------
+    numpy.ndarray
+        1-D array of velocities to be sampled.
+
+    Examples
+    --------
+    The defaults will sample more densely near the center of the distribution,
+    (the "split" method) with a total of 561 classes.
+
+    >>> classes = rq.doppler_classes() #use the default values
+    >>> print(classes.shape)
+    (561,)
+
+    Specifying "uniform" with no additional arguments produces 1601 evenly spaced
+    classes by default.
+
+    >>> m = {"method":"uniform"}
+    >>> classes = rq.doppler_classes(method=m)
+    >>> print(classes.shape)
+    (1601,)
+
+    Further specifying the number of points allows more dense or sparse sampling
+    of the velocity distribution.
+
+    >>> m = {"method":"uniform", "n_uniform":801}
+    >>> classes = rq.doppler_classes(method=m)
+    >>> print(classes.shape)
+    (801,)
+
+    The "split" method also has further specifications
+
+    >>> m = {"method":"split", "n_coherent":301, "n_doppler":501}
+    >>> classes = rq.doppler_classes(method=m)
+    >>> print(classes.shape)
+    (701,)
+
+    References
+    ----------
+    .. [1] Andrew P. Rotunno, et. al.
+        Inverse Transform Sampling for Efficient Doppler-Averaged Spectroscopy Simulation,
+        arXiv:2304.12468 (2023)
+        http://arxiv.org/abs/2304.12468
+
+    """
+    if method is None:
+        method = SplitMethod(method="split")
+
+    assert method is not None
+    implemented_methods = ["uniform","isopop","split","direct"]
+    try:
+        if method["method"] not in implemented_methods:
+            raise ValueError(f"Method {method['method']} is not a recognized meshing method.")
+    except KeyError:
+        raise KeyError("Meshing method must be a dictionary with at least key 'method'")
+
+    if method["method"] == "uniform":
+        # use default options if not provided
+        width_doppler = method.get("width_doppler",2.0)
+        n_uniform = method.get("n_uniform",1601)
+        doppler_velocities = np.linspace(-width_doppler,width_doppler,n_uniform)
+    elif method["method"] == "isopop":
+        # define such that each slice has equal population distribution
+        n_isopop = method.get("n_isopop", 400)
+        bin_edges = np.linspace(0, 1.0, n_isopop+1)
+        bin_centers = (bin_edges - bin_edges[1]/2)[1:]
+        doppler_velocities = special.erfinv(2*bin_centers-1)*np.sqrt(2)
+    elif method["method"] == "split":
+        # use default options if not provided
+        width_doppler = method.get("width_doppler",2.0)
+        width_coherent = method.get("width_coherent",0.4)
+        n_doppler = method.get("n_doppler",201)
+        n_coherent = method.get("n_coherent",401)
+        # Doppler shifts to sample
+        range_doppler = np.linspace(-width_doppler,width_doppler,n_doppler)
+        # Finer mesh near zero velocity class where coherent stuff is happening
+        range_coherent = np.linspace(-width_coherent,width_coherent,n_coherent)
+        # Combine and get deltas for calculating the lazy integral
+        # mask out points from course grid where fine grid is, avoids aliasing artifacts
+        doppler_velocities = np.union1d(range_doppler[np.abs(range_doppler) > width_coherent],
+                                        range_coherent)
+    elif method["method"] == "direct":
+        try:
+            doppler_velocities = method["doppler_velocities"]  # type: ignore[assignment]
+        except KeyError:
+            raise KeyError("Method 'direct' must specify a 'doppler_velocities' config parameter")
+        if not isinstance(doppler_velocities,np.ndarray):
+            doppler_velocities = np.array(doppler_velocities)  # type: ignore[unreachable]
+        # ensure numpy array, then assert shape is 1-D
+        assert len(doppler_velocities.shape) == 1, "doppler_velocities must be 1-D"
+
+    return doppler_velocities
+
+
+def doppler_mesh(doppler_velocities: np.ndarray, spatial_dim: int) -> Tuple[np.ndarray, np.ndarray]:
+    """
+    Creates meshgrids of evaluation points and point "volumes" for doppler averaging.
+
+    Parameters
+    ----------
+    dop_velocities : numpy.ndarray
+        A 1-D array of velocities to evaluate over.
+        These should be normalized to the most probable velocity used by
+        :func:`gaussian3d`.
+    spatial_dim : int
+        Number of spatial dimensions to grid over.
+
+    Returns
+    -------
+    Vs : numpy.ndarray
+        Velocity evaluation points array of shape `(spatial_dim,spatial_dim*[len(dop_vel)])`.
+    Vols : numpy.ndarray
+        "Volume" of each meshpoint. Has same shape as `Vs`.
+
+    Examples
+    --------
+    >>> m = {"method":"uniform", "n_uniform":801}
+    >>> classes = rq.doppler_classes(method=m)
+    >>> mesh, vols = rq.doppler_mesh(classes, 2)
+    >>> print(type(mesh), type(vols))
+    >>> mesh_np = np.array(mesh)
+    >>> vols_np = np.array(vols)
+    >>> print(mesh_np.shape, vols_np.shape)
+    <class 'numpy.ndarray'> <class 'numpy.ndarray'>
+    (2, 801, 801) (2, 801, 801)
+
+    """
+    dop_volumes = np.gradient(doppler_velocities)  # smoothly handles irregular arrays
+    # generate the velocity meshgrids
+    dets = [doppler_velocities for _ in range(spatial_dim)]
+    diffs = [dop_volumes for _ in range(spatial_dim)]
+    Vs = np.array(np.meshgrid(*dets,indexing="ij"))
+    Vols = np.array(np.meshgrid(*diffs,indexing="ij"))
+
+    return Vs, Vols
+
+
+def apply_doppler_weights(sols: np.ndarray,
+                          velocities: np.ndarray, volumes: np.ndarray) -> np.ndarray:
+    """
+    Calculates and applies the weight for each doppler class given unweighted solutions
+    to doppler-shifted equations.
+
+    Works for both time-domain and stead-states solutions.
+
+    Parameters
+    ----------
+    sols : numpy.ndarray
+        The array of solutions over which to calculate weights.
+    velocities : numpy.ndarray
+        Array of shape `(n_dim, *n_dop)` where n_dim
+        is the number of dimensions over which doppler shifts are being considered
+        and `*n_dop` is a number of axes equal to n_dim with length equal to the number
+        of doppler velocity classes which are being considered. The values correspond
+        the velocity class in units of sigma.
+    volumes : numpy.ndarray
+        Array of shape equal to `velocities`.
+        The values correspond to the spacings between doppler classes on each axis.
+
+    Returns
+    -------
+    numpy.ndarray
+        The weighted solution array of shape equal to that of `sols`.
+
+    Raises
+    ------
+    ValueError
+        If the shapes of `velocities` and `volumes` do not match.
+
+    """
+    spatial_dim = volumes.shape[0]
+
+    if volumes.shape != velocities.shape:
+        raise ValueError((f"velocity shape {velocities.shape} does not match "
+                         f"volume shape {volumes.shape}"))
+
+    weights = gaussian3d(velocities)
+    volumes = np.prod(volumes, axis=0)
+
+    # calculate axes to append for array broadcasting to work in return
+    solution_dim = len(sols.shape) - spatial_dim
+    expand_axes = tuple(-1*np.arange(solution_dim)-1)
+
+    weights = np.expand_dims(weights, expand_axes)
+    volumes = np.expand_dims(volumes, expand_axes)
+
+    return weights*volumes*sols
```

### Comparing `rydiqule-1.0.0/src/rydiqule/energy_diagram.py` & `rydiqule-1.0.0rc2/src/rydiqule/energy_diagram.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,486 +1,486 @@
-# MIT License
-#
-# Original Copyright (c) 2017 Giacomo Marchioro
-# Modified by Duy Nguyen and David Meyer
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-"""
-Energy profile diagram
-
-This is a simple script to plot energy profile diagram using matplotlib.
-
-.. code-block:: text
-
-    E|          4__
-    n|   2__    /  \\
-    e|1__/  \__/5   \\
-    r|  3\__/       6\__
-    g|
-    y|
-
-Original author is Giacomo Marchioro.
-The following is modified from https://github.com/giacomomarchioro/PyEnergyDiagrams
-"""
-import matplotlib.pyplot as plt
-from matplotlib.lines import Line2D
-import matplotlib as mpl
-import numpy as np
-
-from collections.abc import Collection
-from typing import Tuple, List, Dict, Optional, Union
-
-COLORS = [
-    '#0173b2', '#de8f05', '#029e73', '#d55e00', '#cc78bc',
-    '#ca9161', '#fbafe4', '#949494', '#ece133', '#56b4e9'
-]
-"Seaborn colorblind palette, for use with coupling arrows."
-
-COLORS_W = [
-    '#006374', '#b8850a', '#3c3c3c', '#a23582', '#592f0d',
-    '#591e71', '#8c0800', '#12711c', '#b1400d', '#001c7f'
-]
-"""Reversed Seaborn colorblind palette, for use with wavy arrows.
-
-Reversing the order helps limit color overlap when using default ordering.
-"""
-
-
-def draw_wiggly_arrow(ax: plt.Axes, start: Collection, stop: Collection,
-                      amp: float = 0.07, nhalfwaves: int = 8, arrow_size: float = 0.06,
-                      linestyle: str = 'solid', color: str = 'k', alpha: float = 1.0) -> None:
-    """
-    Helper funtion that draws a wavy arrow between two points on a plot.
-
-    Parameters
-    ----------
-    ax: :class:`matplotlib:matplotlib.axes.Axes`
-        Axes to add the wiggly arrow to.
-    start: tuple
-        Arrow start point in axes units
-    stop: tuple
-        Arrow stop point in axes units
-    amp: float, optional
-        Amplitude of the wave in axes units.
-        Default is 0.07.
-    nhalfwaves: int, optional
-        Number of half-waves to wave the arrow.
-        Default is 8.
-    arrow_size: float, optional
-        Size of the arrow in axes units.
-        Default is 0.06.
-    linestyle: str, optional
-        Matplotlib linestyle definition.
-        Default is `'solid'`.
-    color: str, optional
-        Matplotlib color specification.
-        Default is `'k'`.
-    alpha: float, optional
-        Matplotlib alpha specification.
-        Default is 1.
-    """
-    start = np.array(start)
-    stop = np.array(stop)
-    vec = stop-start
-    dist = np.sqrt(vec.dot(vec)) - 2*arrow_size  # accounts for arrow head
-    ang = np.arctan2(*vec[::-1])
-
-    # define wiggly line
-    omega = np.pi*nhalfwaves
-    phi = 0
-    x0 = np.linspace(0,dist,151) + start[0]
-    y0 = amp*np.sin(omega*x0 + phi) + start[1]
-    line = mpl.lines.Line2D(x0,y0,color=color,alpha=alpha,linestyle=linestyle)
-    # rotate it to the correct angle
-    line.set_transform(mpl.transforms.Affine2D().rotate_around(*start,ang) + ax.transData)
-
-    # define the arrowhead
-    verts = np.array([[-2,1],[-2,-1],[0,0],[-2,1]]).astype(float) * arrow_size
-    verts[:,1] += stop[1]
-    verts[:,0] += stop[0]
-    path = mpl.path.Path(verts)
-    patch = mpl.patches.PathPatch(path,fc=color,ec=color,alpha=alpha)
-    # rotate it
-    patch.set_transform(mpl.transforms.Affine2D().rotate_around(*stop, ang) + ax.transData)
-    # plot them
-    ax.add_line(line)
-    ax.add_patch(patch)
-
-
-class ED(object):
-    "Energy diagram class"
-
-    def __init__(self, aspect: str = 'equal') -> None:
-        """
-        Constructor for an energy diagram.
-
-        This class contains methods to add energy levels and connections between them.
-        It uses matplotlib to generate the figure, so standard manipulations via
-        matplotlib function calls (including saving of the figure) can be done.
-
-        Call :meth:`~.plot` to actually create the plot.
-
-        Parameters
-        ----------
-        aspect: str,optional
-            Kwarg passed to `fig.add_subplot()`. Default is `'equal'`.
-
-        Note
-        ----
-        Calling :meth:`~.plot` in a jupyter notebook will automatically show
-        the generated figure thanks to jupyter notebook magic in handling
-        matplotlib figures.
-        If you wish to see the plot outside a jupyter notebook, you will need
-        to call `plt.show()` just like any other matplotlib figure.
-        """
-        # plot parameters
-        self.ratio = 1.6181
-        self.auto_adjust = ('dimension', 'space', 'offset')
-        self.dimension: float
-        self.space: float
-        self.offset: float
-        self.offset_ratio = 0.02
-        self.color_bottom_text = 'blue'
-        self.aspect = aspect
-        self.round_energies_at_digit: Union[str,int] = "keep all digits"
-        # data
-        self.pos_number = 0
-        self.energies: List[float] = []
-        self.positions: List[float] = []
-        self.colors: List[str] = []
-        self.top_texts: List[str] = []
-        self.bottom_texts: List[str] = []
-        self.left_texts: List[str] = []
-        self.right_texts: List[str] = []
-        self.links: List = []
-        self.arrows: List = []
-        self.wiggly_arrows: List = []
-        self.arrows_linestyles: Dict = {}
-        self.level_linestyles: List[str] = []
-        self.wiggly_linestyles: Dict = {}
-        # matplotlib fiugre handlers
-        self.fig: Optional[plt.Figure] = None
-        self.ax: Optional[plt.Axes] = None
-
-    def add_level(self, energy: float, bottom_text: str = '',
-                  position: Optional[Union[str, float]] = None, color: str = 'k',
-                  top_text: str = 'Energy', right_text: str = '',
-                  left_text: str = '', linestyle: str = 'solid') -> None:
-        '''
-        This method add a new energy level to the plot.
-
-        Parameters
-        ----------
-        energy : int
-                 The energy of the level in Kcal mol-1
-        bottom_text  : str
-                The text on the bottom of the level (label of the level)
-                (default '')
-        position  : str
-                The position of the level in the plot. Keep it empty to add
-                the level on the right of the previous level use 'last' as
-                argument for adding the level to the last position used
-                for the level before.
-                An integer can be used for adding the level to an arbitrary
-                position.
-                (default  None)
-        color  : str
-                matplotlib color specification of the level  (default  'k')
-        top_text  : str
-                Text on the top of the level. By default it will print the
-                energy of the level. (default  'Energy')
-        right_text  : str
-                Text at the right of the level. (default  '')
-        left_text  : str
-                Text at the left of the level. (default  '')
-        linestyle  : str
-                The linestyle of the level, one of the following values:
-                'solid', 'dashed', 'dashdot', 'dotted' (default  'solid')
-        '''
-
-        if position is None:
-            position = self.pos_number + 1
-            self.pos_number += 1
-        elif isinstance(position, (int, float)):
-            pass
-        elif position == 'last' or position == 'l':
-            position = self.pos_number
-        else:
-            raise ValueError(("Position must be None or 'last' (abrv. 'l') or "
-                              "in case an integer or float specifing the position. "
-                              "It was: %s" % position))
-        if top_text == 'Energy':
-            if self.round_energies_at_digit == "keep all digits":
-                top_text = str(energy)
-            else:
-                assert isinstance(self.round_energies_at_digit, int)
-                top_text = str(round(energy,self.round_energies_at_digit))
-
-        link: List[Tuple[int, str, float, str]] = []
-        self.colors.append(color)
-        self.energies.append(energy)
-        self.positions.append(position)
-        self.top_texts.append(top_text)
-        self.bottom_texts.append(bottom_text)
-        self.left_texts.append(left_text)
-        self.right_texts.append(right_text)
-        self.links.append(link)
-        self.level_linestyles.append(linestyle)
-        self.arrows.append([])
-        self.wiggly_arrows.append([])
-
-    def add_arrow(self, start_level_id: int, end_level_id: int, linestyle: str) -> None:
-        '''
-        Add a arrow between two energy levels using IDs of the level.
-
-        Use self.plot(show_index=True) to show the IDs of the levels.
-
-        Parameters
-        ----------
-        start_level_id : int
-                 Starting level ID
-        end_level_id : int
-                 Ending level ID
-        linestyle: str
-                 matplotlib linestyle string
-        '''
-        self.arrows[start_level_id].append(end_level_id)
-        self.arrows_linestyles[(start_level_id,end_level_id)] = linestyle
-
-    def add_wiggly_arrow(self, start_level_id: int, end_level_id: int, ls_dict: dict) -> None:
-        '''
-        Add a wiggly arrow between two energy levels using IDs of the level.
-
-        Use self.plot(show_index=True) to show the IDs of the levels.
-
-        Parameters
-        ----------
-        start_level_id : int
-                 Starting level ID
-        end_level_id : int
-                 Ending level ID
-        ls_dict: dict
-                 Dictionary of linestyle parameters.
-                 Passed as kwargs to :func:`~.draw_wiggly_arrow`.
-        '''
-        self.wiggly_arrows[start_level_id].append(end_level_id)
-        self.wiggly_linestyles[(start_level_id,end_level_id)] = ls_dict
-
-    def add_link(self, start_level_id: int, end_level_id: int,
-                 color: str = 'k',
-                 ls: str = '--',
-                 linewidth: float = 1,
-                 ) -> None:
-        '''
-        Add a link between two energy levels using IDs of the level.
-
-        Use self.plot(show_index=True) to show the IDs of the levels.
-
-        Parameters
-        ----------
-        start_level_id : int
-                 Starting level ID
-        end_level_id : int
-                 Ending level ID
-        color : str
-                matplotlib color specification of the line
-        ls : str
-                matplotlib line style e.g. -- , ..
-        linewidth : float
-                line width
-        '''
-        self.links[start_level_id].append((end_level_id, ls, linewidth, color))
-
-    def plot(self, show_IDs: bool = False, ylabel: str = "Energy / $kcal$ $mol^{-1}$",
-             ax: Optional[plt.Axes] = None) -> Tuple[plt.Figure, plt.Axes]:
-        '''
-        Plot the energy diagram.
-
-        Use show_IDs=True for showing the IDs of the
-        energy levels and allowing an easy linking.
-
-        .. code-block:: text
-
-            E|          4__
-            n|   2__    /  \\
-            e|1__/  \__/5   \\
-            r|  3\__/       6\__
-            g|
-            y|
-
-        Parameters
-        ----------
-        show_IDs : bool
-            show the IDs of the energy levels
-        ylabel : str
-            The label to use on the left-side axis. "Energy / $kcal$
-            $mol^{-1}$" by default.
-        ax : :class:`matplotlib:matplotlib.axes.Axes`
-            The axes to plot onto. If not specified, a Figure and Axes will be
-            created for you.
-
-        Returns
-        -------
-        fig: :class:`matplotlib:matplotlib.figure.Figure`
-            Figure handle for the generated figure.
-        ax: :class:`matplotlib:matplotlib.axes.Axes`
-            Axes handle for the generated figure.
-        '''
-
-        # Create a figure and axis if the user didn't specify them.
-        if ax is None:
-            self.fig = plt.figure()
-            self.ax = self.fig.add_subplot(111, aspect=self.aspect)
-        # Otherwise register the axes and figure the user passed.
-        else:
-            self.ax = ax
-            self.fig = ax.figure
-            # Constrain the target axis to have the proper aspect ratio
-            self.ax.set_aspect(self.aspect)
-        self.ax.set_ylabel(ylabel)
-        self.ax.axes.get_xaxis().set_visible(False)
-        self.ax.spines['top'].set_visible(False)
-        self.ax.spines['right'].set_visible(False)
-        self.ax.spines['bottom'].set_visible(False)
-        self.ax.axis('off')
-        self.__auto_adjust()
-
-        data = list(
-            zip(
-                self.energies,  # 0
-                self.positions,  # 1
-                self.bottom_texts,  # 2
-                self.top_texts,  # 3
-                self.colors,  # 4
-                self.right_texts,  # 5
-                self.left_texts,  # 6
-                self.level_linestyles
-            )
-        )
-        # plot energy levels
-        level_coords = {}
-        for level in data:
-            start = level[1]*(self.dimension+self.space)
-            self.ax.hlines(
-                level[0],
-                start,
-                start + self.dimension,
-                color=level[4],
-                linestyles=level[7]
-            )
-            level_coords[level[0]] = start
-            self.ax.text(
-                start + self.dimension,  # X
-                level[0] - self.offset,  # Y
-                level[2],  # self.bottom_text
-                horizontalalignment='left',
-                verticalalignment='top',
-                color=self.color_bottom_text
-            )
-        self.level_counter = len(level_coords)
-        if show_IDs:
-            # for showing the ID allowing the user to identify the level
-            for ind, level in enumerate(data):
-                start = level[1]*(self.dimension+self.space)
-                self.ax.text(
-                    start,
-                    level[0]+self.offset,
-                    str(ind),
-                    horizontalalignment='right',
-                    color='black'
-                )
-
-        # draw coupling arrows between levels
-        for idx, arrow in enumerate(self.arrows):
-            diff = 0.0
-            coupling_color = COLORS[idx]
-            for i in arrow:
-                linestyle = self.arrows_linestyles.get((idx, i))
-                start = self.positions[idx]*(self.dimension+self.space)
-                x1 = start + 0.5*self.dimension  # arrow base
-                x2 = start + 0.5*self.dimension
-                y1 = self.energies[idx]
-                y2 = self.energies[i]
-                self.ax.annotate(
-                    "",
-                    xy=(level_coords[i] + diff, y2),  # arrow tip
-                    xytext=(x1, y1),  # arrow base
-                    arrowprops=dict(
-                        color=coupling_color,
-                        linewidth=2.5,
-                        arrowstyle='->',
-                        linestyle=linestyle,
-                        shrinkA=0,
-                        shrinkB=0,
-                    )
-                )
-                diff += 0.4
-
-        # draw wiggly coupling arrows between levels
-        for idx, warrow in enumerate(self.wiggly_arrows):
-            diff = 0.0
-            coupling_color = COLORS_W[idx]
-            for i in warrow:
-                ls_dict = self.wiggly_linestyles.get((idx, i),{})
-                start = self.positions[idx]*(self.dimension+self.space)
-                x1 = start + 0.9*self.dimension  # arrow base
-                x2 = level_coords[i] + 0.9*self.dimension - diff*np.abs(idx-i)
-                y1 = self.energies[idx]
-                y2 = self.energies[i]
-                draw_wiggly_arrow(self.ax, (x1,y1),
-                                  (x2, y2),
-                                  color=coupling_color,
-                                  **ls_dict)
-                diff += 0.1
-
-        # draw links between levels
-        for idx, link in enumerate(self.links):
-            # here we connect the levels with the links
-            # x1, x2   y1, y2
-            for i in link:
-                start = self.positions[idx]*(self.dimension+self.space)
-                x1 = start + self.dimension
-                x2 = self.positions[i[0]]*(self.dimension+self.space)
-                y1 = self.energies[idx]
-                y2 = self.energies[i[0]]
-                line = Line2D(
-                    [x1, x2],
-                    [y1, y2],
-                    ls=i[1],
-                    linewidth=i[2],
-                    color=i[3]
-                )
-                self.ax.add_line(line)
-
-        return self.fig, self.ax
-
-    def __auto_adjust(self) -> None:
-        '''
-        Sets the ratio to the best dimension and space between
-        the levels.
-        '''
-        # Max range between the energy
-        Energy_variation = abs(max(self.energies) - min(self.energies))
-        if 'dimension' in self.auto_adjust or 'space' in self.auto_adjust:
-            # Unique positions of the levels
-            unique_positions = float(len(set(self.positions)))
-            space_for_level = Energy_variation*self.ratio/unique_positions
-            self.dimension = space_for_level*0.7
-            self.space = space_for_level*0.3
-        if 'offset' in self.auto_adjust:
-            self.offset = Energy_variation*self.offset_ratio
+# MIT License
+#
+# Original Copyright (c) 2017 Giacomo Marchioro
+# Modified by Duy Nguyen and David Meyer
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+"""
+Energy profile diagram
+
+This is a simple script to plot energy profile diagram using matplotlib.
+
+.. code-block:: text
+
+    E|          4__
+    n|   2__    /  \\
+    e|1__/  \__/5   \\
+    r|  3\__/       6\__
+    g|
+    y|
+
+Original author is Giacomo Marchioro.
+The following is modified from https://github.com/giacomomarchioro/PyEnergyDiagrams
+"""  # noqa
+import matplotlib.pyplot as plt
+from matplotlib.lines import Line2D
+import matplotlib as mpl
+import numpy as np
+
+from collections.abc import Collection
+from typing import Tuple, List, Dict, Optional, Union
+
+COLORS = [
+    '#0173b2', '#de8f05', '#029e73', '#d55e00', '#cc78bc',
+    '#ca9161', '#fbafe4', '#949494', '#ece133', '#56b4e9'
+]
+"Seaborn colorblind palette, for use with coupling arrows."
+
+COLORS_W = [
+    '#006374', '#b8850a', '#3c3c3c', '#a23582', '#592f0d',
+    '#591e71', '#8c0800', '#12711c', '#b1400d', '#001c7f'
+]
+"""Reversed Seaborn colorblind palette, for use with wavy arrows.
+
+Reversing the order helps limit color overlap when using default ordering.
+"""
+
+
+def draw_wiggly_arrow(ax: plt.Axes, start: Collection, stop: Collection,
+                      amp: float = 0.07, nhalfwaves: int = 8, arrow_size: float = 0.06,
+                      linestyle: str = 'solid', color: str = 'k', alpha: float = 1.0) -> None:
+    """
+    Helper funtion that draws a wavy arrow between two points on a plot.
+
+    Parameters
+    ----------
+    ax: :class:`matplotlib:matplotlib.axes.Axes`
+        Axes to add the wiggly arrow to.
+    start: tuple
+        Arrow start point in axes units
+    stop: tuple
+        Arrow stop point in axes units
+    amp: float, optional
+        Amplitude of the wave in axes units.
+        Default is 0.07.
+    nhalfwaves: int, optional
+        Number of half-waves to wave the arrow.
+        Default is 8.
+    arrow_size: float, optional
+        Size of the arrow in axes units.
+        Default is 0.06.
+    linestyle: str, optional
+        Matplotlib linestyle definition.
+        Default is `'solid'`.
+    color: str, optional
+        Matplotlib color specification.
+        Default is `'k'`.
+    alpha: float, optional
+        Matplotlib alpha specification.
+        Default is 1.
+    """
+    start = np.array(start)
+    stop = np.array(stop)
+    vec = stop-start
+    dist = np.sqrt(vec.dot(vec)) - 2*arrow_size  # accounts for arrow head
+    ang = np.arctan2(*vec[::-1])
+
+    # define wiggly line
+    omega = np.pi*nhalfwaves
+    phi = 0
+    x0 = np.linspace(0,dist,151) + start[0]
+    y0 = amp*np.sin(omega*x0 + phi) + start[1]
+    line = mpl.lines.Line2D(x0,y0,color=color,alpha=alpha,linestyle=linestyle)
+    # rotate it to the correct angle
+    line.set_transform(mpl.transforms.Affine2D().rotate_around(*start,ang) + ax.transData)
+
+    # define the arrowhead
+    verts = np.array([[-2,1],[-2,-1],[0,0],[-2,1]]).astype(float) * arrow_size
+    verts[:,1] += stop[1]
+    verts[:,0] += stop[0]
+    path = mpl.path.Path(verts)
+    patch = mpl.patches.PathPatch(path,fc=color,ec=color,alpha=alpha)
+    # rotate it
+    patch.set_transform(mpl.transforms.Affine2D().rotate_around(*stop, ang) + ax.transData)
+    # plot them
+    ax.add_line(line)
+    ax.add_patch(patch)
+
+
+class ED(object):
+    "Energy diagram class"
+
+    def __init__(self, aspect: str = 'equal') -> None:
+        """
+        Constructor for an energy diagram.
+
+        This class contains methods to add energy levels and connections between them.
+        It uses matplotlib to generate the figure, so standard manipulations via
+        matplotlib function calls (including saving of the figure) can be done.
+
+        Call :meth:`~.plot` to actually create the plot.
+
+        Parameters
+        ----------
+        aspect: str,optional
+            Kwarg passed to `fig.add_subplot()`. Default is `'equal'`.
+
+        Note
+        ----
+        Calling :meth:`~.plot` in a jupyter notebook will automatically show
+        the generated figure thanks to jupyter notebook magic in handling
+        matplotlib figures.
+        If you wish to see the plot outside a jupyter notebook, you will need
+        to call `plt.show()` just like any other matplotlib figure.
+        """
+        # plot parameters
+        self.ratio = 1.6181
+        self.auto_adjust = ('dimension', 'space', 'offset')
+        self.dimension: float
+        self.space: float
+        self.offset: float
+        self.offset_ratio = 0.02
+        self.color_bottom_text = 'blue'
+        self.aspect = aspect
+        self.round_energies_at_digit: Union[str,int] = "keep all digits"
+        # data
+        self.pos_number = 0
+        self.energies: List[float] = []
+        self.positions: List[float] = []
+        self.colors: List[str] = []
+        self.top_texts: List[str] = []
+        self.bottom_texts: List[str] = []
+        self.left_texts: List[str] = []
+        self.right_texts: List[str] = []
+        self.links: List = []
+        self.arrows: List = []
+        self.wiggly_arrows: List = []
+        self.arrows_linestyles: Dict = {}
+        self.level_linestyles: List[str] = []
+        self.wiggly_linestyles: Dict = {}
+        # matplotlib fiugre handlers
+        self.fig: Optional[plt.Figure] = None
+        self.ax: Optional[plt.Axes] = None
+
+    def add_level(self, energy: float, bottom_text: str = '',
+                  position: Optional[Union[str, float]] = None, color: str = 'k',
+                  top_text: str = 'Energy', right_text: str = '',
+                  left_text: str = '', linestyle: str = 'solid') -> None:
+        '''
+        This method add a new energy level to the plot.
+
+        Parameters
+        ----------
+        energy : int
+                 The energy of the level in Kcal mol-1
+        bottom_text  : str
+                The text on the bottom of the level (label of the level)
+                (default '')
+        position  : str
+                The position of the level in the plot. Keep it empty to add
+                the level on the right of the previous level use 'last' as
+                argument for adding the level to the last position used
+                for the level before.
+                An integer can be used for adding the level to an arbitrary
+                position.
+                (default  None)
+        color  : str
+                matplotlib color specification of the level  (default  'k')
+        top_text  : str
+                Text on the top of the level. By default it will print the
+                energy of the level. (default  'Energy')
+        right_text  : str
+                Text at the right of the level. (default  '')
+        left_text  : str
+                Text at the left of the level. (default  '')
+        linestyle  : str
+                The linestyle of the level, one of the following values:
+                'solid', 'dashed', 'dashdot', 'dotted' (default  'solid')
+        '''
+
+        if position is None:
+            position = self.pos_number + 1
+            self.pos_number += 1
+        elif isinstance(position, (int, float)):
+            pass
+        elif position == 'last' or position == 'l':
+            position = self.pos_number
+        else:
+            raise ValueError(("Position must be None or 'last' (abrv. 'l') or "
+                              "in case an integer or float specifing the position. "
+                              "It was: %s" % position))
+        if top_text == 'Energy':
+            if self.round_energies_at_digit == "keep all digits":
+                top_text = str(energy)
+            else:
+                assert isinstance(self.round_energies_at_digit, int)
+                top_text = str(round(energy,self.round_energies_at_digit))
+
+        link: List[Tuple[int, str, float, str]] = []
+        self.colors.append(color)
+        self.energies.append(energy)
+        self.positions.append(position)
+        self.top_texts.append(top_text)
+        self.bottom_texts.append(bottom_text)
+        self.left_texts.append(left_text)
+        self.right_texts.append(right_text)
+        self.links.append(link)
+        self.level_linestyles.append(linestyle)
+        self.arrows.append([])
+        self.wiggly_arrows.append([])
+
+    def add_arrow(self, start_level_id: int, end_level_id: int, linestyle: str) -> None:
+        '''
+        Add a arrow between two energy levels using IDs of the level.
+
+        Use self.plot(show_index=True) to show the IDs of the levels.
+
+        Parameters
+        ----------
+        start_level_id : int
+                 Starting level ID
+        end_level_id : int
+                 Ending level ID
+        linestyle: str
+                 matplotlib linestyle string
+        '''
+        self.arrows[start_level_id].append(end_level_id)
+        self.arrows_linestyles[(start_level_id,end_level_id)] = linestyle
+
+    def add_wiggly_arrow(self, start_level_id: int, end_level_id: int, ls_dict: dict) -> None:
+        '''
+        Add a wiggly arrow between two energy levels using IDs of the level.
+
+        Use self.plot(show_index=True) to show the IDs of the levels.
+
+        Parameters
+        ----------
+        start_level_id : int
+                 Starting level ID
+        end_level_id : int
+                 Ending level ID
+        ls_dict: dict
+                 Dictionary of linestyle parameters.
+                 Passed as kwargs to :func:`~.draw_wiggly_arrow`.
+        '''
+        self.wiggly_arrows[start_level_id].append(end_level_id)
+        self.wiggly_linestyles[(start_level_id,end_level_id)] = ls_dict
+
+    def add_link(self, start_level_id: int, end_level_id: int,
+                 color: str = 'k',
+                 ls: str = '--',
+                 linewidth: float = 1,
+                 ) -> None:
+        '''
+        Add a link between two energy levels using IDs of the level.
+
+        Use self.plot(show_index=True) to show the IDs of the levels.
+
+        Parameters
+        ----------
+        start_level_id : int
+                 Starting level ID
+        end_level_id : int
+                 Ending level ID
+        color : str
+                matplotlib color specification of the line
+        ls : str
+                matplotlib line style e.g. -- , ..
+        linewidth : float
+                line width
+        '''
+        self.links[start_level_id].append((end_level_id, ls, linewidth, color))
+
+    def plot(self, show_IDs: bool = False, ylabel: str = "Energy / $kcal$ $mol^{-1}$",
+             ax: Optional[plt.Axes] = None) -> Tuple[plt.Figure, plt.Axes]:
+        '''
+        Plot the energy diagram.
+
+        Use show_IDs=True for showing the IDs of the
+        energy levels and allowing an easy linking.
+
+        .. code-block:: text
+
+            E|          4__
+            n|   2__    /  \\
+            e|1__/  \__/5   \\
+            r|  3\__/       6\__
+            g|
+            y|
+
+        Parameters
+        ----------
+        show_IDs : bool
+            show the IDs of the energy levels
+        ylabel : str
+            The label to use on the left-side axis. "Energy / $kcal$
+            $mol^{-1}$" by default.
+        ax : :class:`matplotlib:matplotlib.axes.Axes`
+            The axes to plot onto. If not specified, a Figure and Axes will be
+            created for you.
+
+        Returns
+        -------
+        fig: :class:`matplotlib:matplotlib.figure.Figure`
+            Figure handle for the generated figure.
+        ax: :class:`matplotlib:matplotlib.axes.Axes`
+            Axes handle for the generated figure.
+        '''  # noqa
+
+        # Create a figure and axis if the user didn't specify them.
+        if ax is None:
+            self.fig = plt.figure()
+            self.ax = self.fig.add_subplot(111, aspect=self.aspect)
+        # Otherwise register the axes and figure the user passed.
+        else:
+            self.ax = ax
+            self.fig = ax.figure
+            # Constrain the target axis to have the proper aspect ratio
+            self.ax.set_aspect(self.aspect)
+        self.ax.set_ylabel(ylabel)
+        self.ax.axes.get_xaxis().set_visible(False)
+        self.ax.spines['top'].set_visible(False)
+        self.ax.spines['right'].set_visible(False)
+        self.ax.spines['bottom'].set_visible(False)
+        self.ax.axis('off')
+        self.__auto_adjust()
+
+        data = list(
+            zip(
+                self.energies,  # 0
+                self.positions,  # 1
+                self.bottom_texts,  # 2
+                self.top_texts,  # 3
+                self.colors,  # 4
+                self.right_texts,  # 5
+                self.left_texts,  # 6
+                self.level_linestyles
+            )
+        )
+        # plot energy levels
+        level_coords = {}
+        for level in data:
+            start = level[1]*(self.dimension+self.space)
+            self.ax.hlines(
+                level[0],
+                start,
+                start + self.dimension,
+                color=level[4],
+                linestyles=level[7]
+            )
+            level_coords[level[0]] = start
+            self.ax.text(
+                start + self.dimension,  # X
+                level[0] - self.offset,  # Y
+                level[2],  # self.bottom_text
+                horizontalalignment='left',
+                verticalalignment='top',
+                color=self.color_bottom_text
+            )
+        self.level_counter = len(level_coords)
+        if show_IDs:
+            # for showing the ID allowing the user to identify the level
+            for ind, level in enumerate(data):
+                start = level[1]*(self.dimension+self.space)
+                self.ax.text(
+                    start,
+                    level[0]+self.offset,
+                    str(ind),
+                    horizontalalignment='right',
+                    color='black'
+                )
+
+        # draw coupling arrows between levels
+        for idx, arrow in enumerate(self.arrows):
+            diff = 0.0
+            coupling_color = COLORS[idx]
+            for i in arrow:
+                linestyle = self.arrows_linestyles.get((idx, i))
+                start = self.positions[idx]*(self.dimension+self.space)
+                x1 = start + 0.5*self.dimension  # arrow base
+                x2 = start + 0.5*self.dimension
+                y1 = self.energies[idx]
+                y2 = self.energies[i]
+                self.ax.annotate(
+                    "",
+                    xy=(level_coords[i] + diff, y2),  # arrow tip
+                    xytext=(x1, y1),  # arrow base
+                    arrowprops=dict(
+                        color=coupling_color,
+                        linewidth=2.5,
+                        arrowstyle='->',
+                        linestyle=linestyle,
+                        shrinkA=0,
+                        shrinkB=0,
+                    )
+                )
+                diff += 0.4
+
+        # draw wiggly coupling arrows between levels
+        for idx, warrow in enumerate(self.wiggly_arrows):
+            diff = 0.0
+            coupling_color = COLORS_W[idx]
+            for i in warrow:
+                ls_dict = self.wiggly_linestyles.get((idx, i),{})
+                start = self.positions[idx]*(self.dimension+self.space)
+                x1 = start + 0.9*self.dimension  # arrow base
+                x2 = level_coords[i] + 0.9*self.dimension - diff*np.abs(idx-i)
+                y1 = self.energies[idx]
+                y2 = self.energies[i]
+                draw_wiggly_arrow(self.ax, (x1,y1),
+                                  (x2, y2),
+                                  color=coupling_color,
+                                  **ls_dict)
+                diff += 0.1
+
+        # draw links between levels
+        for idx, link in enumerate(self.links):
+            # here we connect the levels with the links
+            # x1, x2   y1, y2
+            for i in link:
+                start = self.positions[idx]*(self.dimension+self.space)
+                x1 = start + self.dimension
+                x2 = self.positions[i[0]]*(self.dimension+self.space)
+                y1 = self.energies[idx]
+                y2 = self.energies[i[0]]
+                line = Line2D(
+                    [x1, x2],
+                    [y1, y2],
+                    ls=i[1],
+                    linewidth=i[2],
+                    color=i[3]
+                )
+                self.ax.add_line(line)
+
+        return self.fig, self.ax
+
+    def __auto_adjust(self) -> None:
+        '''
+        Sets the ratio to the best dimension and space between
+        the levels.
+        '''
+        # Max range between the energy
+        Energy_variation = abs(max(self.energies) - min(self.energies))
+        if 'dimension' in self.auto_adjust or 'space' in self.auto_adjust:
+            # Unique positions of the levels
+            unique_positions = float(len(set(self.positions)))
+            space_for_level = Energy_variation*self.ratio/unique_positions
+            self.dimension = space_for_level*0.7
+            self.space = space_for_level*0.3
+        if 'offset' in self.auto_adjust:
+            self.offset = Energy_variation*self.offset_ratio
```

### Comparing `rydiqule-1.0.0/src/rydiqule/experiments.py` & `rydiqule-1.0.0rc2/src/rydiqule/experiments.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,425 +1,423 @@
-"""
-Standard methods for converting results to physical values.
-"""
-
-from .sensor import Sensor
-from .cell import Cell
-from .sensor_solution import Solution
-from .sensor_utils import get_rho_ij
-from .solvers import solve_steady_state
-
-import numpy as np
-import warnings
-
-from scipy.constants import c
-
-from typing import Tuple, Optional, Union
-
-
-def get_transmission_coef(sol: Solution, cell: Cell, cell_length: float,
-                          probe_tuple: Tuple[int, ...] = (0, 1)) -> np.ndarray:
-    """
-    Extract the transmission term from a solution.
-
-    Assumes the optically-thin approximation is valid.
-
-    Parameters
-    ----------
-    sol: :class:`~.Solution`
-        A Solution object containing at least the `rho`
-        attribute. Typically created as the return of :meth:`~.solve_steady_state`
-        or `~.solve_time`.
-    cell: :class:`~.Cell`
-        The cell used to generate the solution. Used to get
-        physical information needed for the calculation.
-    cell_length: float
-        Optical path length of the cell, in meters.
-    probe_tuple: tuple of int, optional
-        Tuple of probing coupling.
-        Defaults to `(0,1)`.
-
-    Returns
-    -------
-    numpy.ndarray
-        Numerical value of the probe absorption in fractional units
-        (P_out/P_in).
-
-    Examples
-    --------
-    >>> c = rq.Cell('Rb85', *rq.D2_states('Rb85'))
-    >>> c.add_coupling(states=(0,1), rabi_frequency=1, detuning=1)
-    >>> sols = rq.solve_steady_state(c)
-    >>> print(sols.rho.shape)
-    >>> t = rq.get_transmission_coef(sols, c, 1e-3)
-    >>> print(t)
-    (3,)
-    0.47653638415943955
-
-    """
-    probe_rabi = _get_probe_rabi(cell, probe_tuple)
-    # reverse probe tuple order to get correct sign of imag
-    rho_probe = get_rho_ij(sol.rho, *probe_tuple[::-1])
-    OD = get_OD(rho_probe, cell_length, probe_rabi, cell.kappa)
-
-    return np.exp(-OD)
-
-
-def get_OD(rho_probe: np.ndarray, cell_length: float,
-           probe_rabi: Union[float, np.ndarray], kappa: float,) -> np.ndarray:
-    """
-    Calculates the optical depth from the solution.
-
-    Assumes the optically-thin approximation is valid.
-    If a calculated OD for a solution exceeds 1,
-    this approximation is likely invalid.
-
-    Parameters
-    ----------
-    rho_probe: numpy.ndarray
-        Array of matrix elements for the probing transition.
-    cell_length: float
-        Optical path length of the cell, in meters.
-    probe_rabi: float or numpy.ndarray
-        Probe Rabi frequency, in Mrad/s
-    kappa: float
-        kappa constant, in units of MHz/m
-
-    Returns
-    -------
-    OD: numpy.ndarray
-        Optical depth of the sample
-
-    Warns
-    -----
-    UserWarning
-        If any OD exceeds 1, which indicates the optically-thin approximation
-        is likely invalid.
-
-    Examples
-    --------
-    >>> c = rq.Cell('Rb85', *rq.D2_states('Rb85'))
-    >>> c.add_coupling(states=(0,1), rabi_frequency=1, detuning=1)
-    >>> sols = rq.solve_steady_state(c)
-    >>> print(sols.rho.shape)
-    >>> OD = rq.experiments.get_OD(rq.get_rho_ij(sols, 1, 0), 1e-3, 1, c.kappa)
-    >>> print(OD)
-    >>> OD2 = rq.experiments.get_OD(rq.get_rho_ij(sols, 1, 0), 1e-2, 1, c.kappa)
-    >>> print(OD2)
-    (3,)
-    0.7412112017002291
-    7.412112017002292
-    ~/src/Rydiqule/src/rydiqule/experiments.py:103: UserWarning:
-    At least one solution has optical depth greater than 1.
-    Integrated results are likely invalid.
-
-    """
-    # calculate optical-depth assuming optically-then approximation is valid
-    OD = kappa*rho_probe.imag*cell_length/probe_rabi
-    if np.any(OD > 1.0):
-        # optically-thin approximation probably violated
-        warnings.warn(('At least one solution has optical depth '
-                       'greater than 1. Integrated results are '
-                       'likely invalid.'))
-
-    return OD
-
-
-def get_phase_shift(sol: Solution, cell: Cell, cell_length: float,
-                    probe_tuple: Tuple[int, ...] = (0, 1)) -> np.ndarray:
-    """
-    Extract the phase shift from a solution.
-
-    Assumes the optically-thin approximation is valid.
-
-    Parameters
-    ----------
-    sol: :class:`~.Solution`
-        Solution object to extract phase shift from.
-    cell: :class:`~.Cell`
-        The cell used to generate the solution. Used to get
-        physical information needed for the calculation.
-    cell_length: float
-        Optical path length of the cell, in meters.
-    probe_tuple: tuple of int, optional
-        Tuple of probing coupling.
-        Defaults to `(0,1)`.
-
-    Returns
-    -------
-    numpy.ndarray
-        Probe phase in radians.
-
-    Examples
-    --------
-    >>> c = rq.Cell('Rb85', *rq.D2_states('Rb85'))
-    >>> c.add_coupling(states=(0,1), rabi_frequency=1, detuning=1)
-    >>> sols = rq.solve_steady_state(c)
-    >>> print(sols.rho.shape)
-    >>> phase_shift = rq.get_phase_shift(sols, c, 1e-3)
-    >>> print(phase_shift)
-    (3,)
-    -0.03807271078849609
-
-    """
-    probe_rabi = _get_probe_rabi(cell, probe_tuple)
-    # reverse probe tuple order to get correct sign of imag
-    # not actually necessary for this function since only need real part
-    rho_probe = get_rho_ij(sol.rho, *probe_tuple[::-1])
-
-    return (cell.kappa/probe_rabi)*rho_probe.real*cell_length
-
-
-def get_susceptibility(sol: Solution, cell: Cell,
-                       probe_tuple: Tuple[int, ...] = (0, 1)) -> np.ndarray:
-    """
-    For a given density matrix solution and cell,
-    return the atomic susceptibility on the probe transition.
-
-    Parameters
-    ----------
-    sol: :class:`~.Solution`
-        Solution object to extract susceptibility from.
-    cell: :class:`~.Cell`
-        The cell used to generate the solution. Used to get
-        physical information needed for the calculation.
-    probe_tuple: tuple of int, optional
-        Tuple of probing coupling.
-        Defaults to `(0,1)`.
-
-    Returns
-    -------
-    numpy.ndarray
-        Susceptibility of the density matrix solution.
-
-    Examples
-    --------
-    >>> c = rq.Cell('Rb85', *rq.D2_states('Rb85'))
-    >>> c.add_coupling(states=(0,1), rabi_frequency=1, detuning=1)
-    >>> sols = rq.solve_steady_state(c)
-    >>> print(sols.rho.shape)
-    >>> sus = rq.get_susceptibility(sols, c)
-    >>> print(f"{sus:.2f}")
-    (3,)
-    -24.40+474.99j
-
-    """
-    probe_rabi = _get_probe_rabi(cell, probe_tuple)
-    # reverse probe tuple order to get correct sign of imag
-    rho_probe = get_rho_ij(sol.rho, *probe_tuple[::-1])
-
-    return 1e-6*(cell.kappa/probe_rabi)*rho_probe*cell.probe_freq/(2*c)
-
-
-def get_solution_element(sols: Solution, idx: int) -> np.ndarray:
-    """
-    Return a slice of an n_dimensional matrix of solutions of shape (...,n^2-1),
-    where n is the basis size of the quantum system.
-
-    Parameters
-    ----------
-    sols: numpy.ndarray
-        An N-Dimensional numpy array representing the final
-        density matrix, with ground state removed, and written in the totally
-        real equations basis. Can have arbitrary axes preceding density matrix
-        axis.
-    idx: int
-        Solution index to slice.
-
-    Returns
-    -------
-    numpy.ndarray
-        Slice of solutions corresponding to index idx. For example,
-        if sols has shape (..., n^2-1), sol_slice will have shape (...).
-
-    Raises
-    ------
-    IndexError
-        If `idx` in not within the shape determined by basis size.
-
-    Examples
-    --------
-    >>> c = rq.Cell('Rb85', *rq.D2_states('Rb85'))
-    >>> c.add_coupling(states=(0,1), rabi_frequency=1, detuning=1)
-    >>> sols = rq.solve_steady_state(c)
-    >>> print(sols.rho.shape)
-    >>> rho_01 = rq.get_solution_element(sols, 0)
-    >>> print(rho_01)
-    (3,)
-    -0.0013139903428765695
-
-    """
-    basis_size = np.sqrt(sols.rho.shape[-1] + 1)
-    try:
-        sol_slice = sols.rho.take(indices=idx, axis=-1)
-    except IndexError:
-        raise IndexError(f"No element with given index for {basis_size}-level system")
-
-    return sol_slice
-
-
-def get_snr(sensor: Sensor, optical_path_length: float, param_label: str,
-            probe_tuple: Tuple[int, int] = (0, 1),
-            phase_quadrature: bool = False,
-            kappa: Optional[float] = None, eta: Optional[float] = None
-            ) -> Tuple[np.ndarray, Tuple[np.ndarray, ...]]:
-    """
-    Calculate a Sensor's signal-to-noise ratio, in a 1Hz bandwidth,
-    to a specified signal parameter.
-
-    SNR is calculated with respect to the signal parameter,
-    relative to the inital value of the signal parameter.
-    The returned mesh is similarly transformed from the typical sensor mesh,
-    by replacing the total value of the signal parameter
-    with the deviation in the signal parameter (relative
-    to it's initial array value).
-
-    The conventions used follow that of [1]_.
-
-    Parameters
-    ----------
-    sensor : :class:`Sensor`
-        sensor for which SNR should be calculated. The definition
-        of sensor.couplings should contain at least one coupling with a list-like
-        parameter. For the list-like parameter, the first array element is the
-        "base" against which SNR for each other value is calculated.
-    optical_path_length : int
-        Sensor optical path length in meters.
-    param_label : str
-        Label of the axis with respect to which SNR is calculated.
-        See :meth:`Sensor.axis_labels` for more details on axis labeling. The
-        value corresponding to this label should be the list-like parameter
-        with respect to which SNR should be calculated.
-        This parameter list must have at least two elements,
-        and SNR is calculated relative to the first element in the list
-        for all other elements in the list.
-    probe_tuple : tuple
-        Two-integer tuple specifying the probing transition.
-    phase_quadrature : :obj:`bool`, optional
-        Whether the sensor is measured in the
-        phase quadrature of the probe laser. False denotes measurement in the
-        amplitude quadrature.  Default is False.
-    kappa: float, optional
-        Differential prefactor, in units of (Mrad/s)/m.
-        Must be specified when using :class:`Sensor`.
-    eta: float, optional
-        Noise density prefactor, in units of root(Hz)
-        Must be specified when using :class:`Sensor`.
-
-    Returns
-    -------
-        snrs : numpy.ndarray
-            Array of SNRs for the sensor with respect to the change
-            in the signal parameter.  Calculated in units of amplitude relative
-            to noise standard deviation.
-        mesh : tuple(numpy.ndarray)
-            Numpy meshgrid of the coupling parameters that yield each
-            snr.  The signal parameter axis now shows the signal change.
-
-    Raises
-    ------
-    ValueError
-        If the specified param_label is not in `Sensor.axis_labels()`
-
-    Examples
-    --------
-    >>> c = rq.Sensor()
-    >>> c.add_coupling(states=(0,1), rabi_frequency=np.linspace(0, 1, 5), detuning=1)
-    >>> snr, mesh = rq.get_snr(c, 0.01, '(0, 1)_rabi_frequency')
-    >>> print(snr)
-    >>> print(mesh)
-    [     0. 137024. 273980. 410796. 547405.]
-    [array([0., 0., 0., 1., 1.])]
-
-    References
-    ----------
-    .. [1] D. H. Meyer, C. O'Brien, D. P. Fahey, K. C. Cox, and P. D. Kunz,
-       "Optimal atomic quantum sensing using
-       electromagnetically-induced-transparency readout,"
-       Phys. Rev. A, vol. 104, p. 043103, 2021.
-    """
-    if (sensor.eta is not None or sensor.kappa is not None) and (eta is not None
-                                                                 or kappa is not None):
-        raise ValueError('Cannot provide alternate eta/kappa values from Sensor class')
-    elif eta is None or kappa is None:
-        if sensor.eta is None or sensor.kappa is None:
-            raise ValueError(('Must specify both eta/kappa via arguments '
-                              'to get_snr OR attributes of sensor.'))
-        eta = sensor.eta
-        kappa = sensor.kappa
-
-    labels = sensor.axis_labels()
-    try:
-        sensitivity_axis = labels.index(param_label)
-    except ValueError:
-        raise ValueError(f"{param_label} label is not in sensor.axis_labels()")
-
-    full_sols = solve_steady_state(sensor)
-    rhos_ij = get_rho_ij(full_sols.rho, *probe_tuple[::-1])
-
-    # check that OD isn't high so optically-thin approximation is valid
-    probe_rabi = _get_probe_rabi(sensor, probe_tuple)
-    _ = get_OD(rhos_ij, optical_path_length, probe_rabi, kappa)
-
-    rho_diffs = rhos_ij - np.take(rhos_ij, [0], sensitivity_axis)
-
-    if phase_quadrature:
-        rho_diffs_quadrature = np.abs(np.real(rho_diffs))
-    else:
-        rho_diffs_quadrature = np.abs(np.imag(rho_diffs))
-
-    rho_ij_noise = eta/kappa  # follows directly from eqns 4 and 6 of 2105.10494
-    snrs: np.ndarray = rho_diffs_quadrature/rho_ij_noise*optical_path_length
-
-    mesh = sensor.get_parameter_mesh(sparse=False)
-    mesh[sensitivity_axis] -= np.take(mesh[sensitivity_axis], [0], sensitivity_axis)
-
-    return snrs, mesh
-
-
-def _get_probe_rabi(sensor: Sensor,
-                    probe_tuple: Tuple[int, ...] = (0, 1)) -> Union[float, np.ndarray]:
-    """
-    Helper function that returns the correct probe Rabi frequency
-    from a Sensor for use in functions that return experimental values.
-
-    Parameters
-    ----------
-    sensor: :class:`~.Sensor`
-        Sensor object that has the probe coupling defined
-    probe_tuple: tuple of int
-        The tuple that defines the probing coupling to extract
-
-    Returns
-    -------
-    probe_rabi: float of numpy.ndarray
-        Probe Rabi frequency defined in the Sensor
-
-    Warns
-    -----
-    UserWarning
-        If the probe coupling has time dependence.
-        In this case, the returned Rabi frequency may not be well defined.
-    
-    """
-    probe_coupling = sensor.couplings.edges[probe_tuple]
-
-    if probe_coupling.get('time_dependence', False):
-        warnings.warn(('Probe is time dependent.  Output of _get_probe_rabi '
-                       'is not guaranteed to be well defined.'))
-
-    rabi = probe_coupling.get('rabi_frequency', None)
-    if isinstance(rabi, (list, np.ndarray)):
-
-        # get Rabi from parameter mesh so broadcasting works
-        probe_label = probe_coupling['label']
-
-        # get index in mesh for the scanned Rabi frequency
-        labels = sensor.axis_labels()
-        mesh_index = labels.index(probe_label+'_rabi_frequency')
-        parameter_mesh = sensor.get_parameter_mesh()
-
-        return parameter_mesh[mesh_index]
-
-    else:
-        # it's just a number
-        return rabi
+"""
+Standard methods for converting results to physical values.
+"""
+
+from .sensor import Sensor
+from .cell import Cell
+from .sensor_solution import Solution
+from .sensor_utils import get_rho_ij
+from .solvers import solve_steady_state
+
+import numpy as np
+import warnings
+
+from scipy.constants import c
+
+from typing import Tuple, Optional, Union
+
+
+def get_transmission_coef(sol: Solution, cell: Cell, cell_length: float,
+                          probe_tuple: Tuple[int, ...] = (0, 1)) -> np.ndarray:
+    """
+    Extract the transmission term from a solution.
+
+    Assumes the optically-thin approximation is valid.
+
+    Parameters
+    ----------
+    sol: :class:`~.Solution`
+        A Solution object containing at least the `rho`
+        attribute. Typically created as the return of :meth:`~.solve_steady_state`
+        or `~.solve_time`.
+    cell: :class:`~.Cell`
+        The cell used to generate the solution. Used to get
+        physical information needed for the calculation.
+    cell_length: float
+        Optical path length of the cell, in meters.
+    probe_tuple: tuple of int, optional
+        Tuple of probing coupling.
+        Defaults to `(0,1)`.
+
+    Returns
+    -------
+    numpy.ndarray
+        Numerical value of the probe absorption in fractional units
+        (P_out/P_in).
+
+    Examples
+    --------
+    >>> c = rq.Cell('Rb85', *rq.D2_states('Rb85'))
+    >>> c.add_coupling(states=(0,1), rabi_frequency=1, detuning=1)
+    >>> sols = rq.solve_steady_state(c)
+    >>> print(sols.rho.shape)
+    >>> t = rq.get_transmission_coef(sols, c, 1e-3)
+    >>> print(t)
+    (3,)
+    0.47653638415943955
+
+    """
+    probe_rabi = _get_probe_rabi(cell, probe_tuple)
+    # reverse probe tuple order to get correct sign of imag
+    rho_probe = get_rho_ij(sol.rho, *probe_tuple[::-1])
+    OD = get_OD(rho_probe, cell_length, probe_rabi, cell.kappa)
+
+    return np.exp(-OD)
+
+
+def get_OD(rho_probe: np.ndarray, cell_length: float,
+           probe_rabi: Union[float, np.ndarray], kappa: float,) -> np.ndarray:
+    """
+    Calculates the optical depth from the solution.
+
+    Assumes the optically-thin approximation is valid.
+    If a calculated OD for a solution exceeds 1,
+    this approximation is likely invalid.
+
+    Parameters
+    ----------
+    rho_probe: numpy.ndarray
+        Array of matrix elements for the probing transition.
+    cell_length: float
+        Optical path length of the cell, in meters.
+    probe_rabi: float or numpy.ndarray
+        Probe Rabi frequency, in Mrad/s
+    kappa: float
+        kappa constant, in units of MHz/m
+
+    Returns
+    -------
+    OD: numpy.ndarray
+        Optical depth of the sample
+
+    Warns
+    -----
+    UserWarning
+        If any OD exceeds 1, which indicates the optically-thin approximation
+        is likely invalid.
+
+    Examples
+    --------
+    >>> c = rq.Cell('Rb85', *rq.D2_states('Rb85'))
+    >>> c.add_coupling(states=(0,1), rabi_frequency=1, detuning=1)
+    >>> sols = rq.solve_steady_state(c)
+    >>> print(sols.rho.shape)
+    >>> OD = rq.experiments.get_OD(rq.get_rho_ij(sols, 1, 0), 1e-3, 1, c.kappa)
+    >>> print(OD)
+    >>> OD2 = rq.experiments.get_OD(rq.get_rho_ij(sols, 1, 0), 1e-2, 1, c.kappa)
+    >>> print(OD2)
+    (3,)
+    0.7412112017002291
+    7.412112017002292
+    ~/src/Rydiqule/src/rydiqule/experiments.py:103: UserWarning: At least one solution has optical depth greater than 1.
+    Integrated results are likely invalid.
+
+    """
+    # calculate optical-depth assuming optically-then approximation is valid
+    OD = kappa*rho_probe.imag*cell_length/probe_rabi
+    if np.any(OD > 1.0):
+        # optically-thin approximation probably violated
+        warnings.warn(('At least one solution has optical depth '
+                       'greater than 1. Integrated results are '
+                       'likely invalid.'))
+
+    return OD
+
+
+def get_phase_shift(sol: Solution, cell: Cell, cell_length: float,
+                    probe_tuple: Tuple[int, ...] = (0, 1)) -> np.ndarray:
+    """
+    Extract the phase shift from a solution.
+
+    Assumes the optically-thin approximation is valid.
+
+    Parameters
+    ----------
+    sol: :class:`~.Solution`
+        Solution object to extract phase shift from.
+    cell: :class:`~.Cell`
+        The cell used to generate the solution. Used to get
+        physical information needed for the calculation.
+    cell_length: float
+        Optical path length of the cell, in meters.
+    probe_tuple: tuple of int, optional
+        Tuple of probing coupling.
+        Defaults to `(0,1)`.
+
+    Returns
+    -------
+    numpy.ndarray
+        Probe phase in radians.
+
+    Examples
+    --------
+    >>> c = rq.Cell('Rb85', *rq.D2_states('Rb85'))
+    >>> c.add_coupling(states=(0,1), rabi_frequency=1, detuning=1)
+    >>> sols = rq.solve_steady_state(c)
+    >>> print(sols.rho.shape)
+    >>> phase_shift = rq.get_phase_shift(sols, c, 1e-3)
+    >>> print(phase_shift)
+    (3,)
+    -0.03807271078849609
+
+    """
+    probe_rabi = _get_probe_rabi(cell, probe_tuple)
+    # reverse probe tuple order to get correct sign of imag
+    # not actually necessary for this function since only need real part
+    rho_probe = get_rho_ij(sol.rho, *probe_tuple[::-1])
+
+    return (cell.kappa/probe_rabi)*rho_probe.real*cell_length
+
+
+def get_susceptibility(sol: Solution, cell: Cell,
+                       probe_tuple: Tuple[int, ...] = (0, 1)) -> np.ndarray:
+    """
+    For a given density matrix solution and cell,
+    return the atomic susceptibility on the probe transition.
+
+    Parameters
+    ----------
+    sol: :class:`~.Solution`
+        Solution object to extract susceptibility from.
+    cell: :class:`~.Cell`
+        The cell used to generate the solution. Used to get
+        physical information needed for the calculation.
+    probe_tuple: tuple of int, optional
+        Tuple of probing coupling.
+        Defaults to `(0,1)`.
+
+    Returns
+    -------
+    numpy.ndarray
+        Susceptibility of the density matrix solution.
+
+    Examples
+    --------
+    >>> c = rq.Cell('Rb85', *rq.D2_states('Rb85'))
+    >>> c.add_coupling(states=(0,1), rabi_frequency=1, detuning=1)
+    >>> sols = rq.solve_steady_state(c)
+    >>> print(sols.rho.shape)
+    >>> sus = rq.get_susceptibility(sols, c)
+    >>> print(f"{sus:.2f}")
+    (3,)
+    -24.40+474.99j
+
+    """
+    probe_rabi = _get_probe_rabi(cell, probe_tuple)
+    # reverse probe tuple order to get correct sign of imag
+    rho_probe = get_rho_ij(sol.rho, *probe_tuple[::-1])
+
+    return 1e-6*(cell.kappa/probe_rabi)*rho_probe*cell.probe_freq/(2*c)
+
+
+def get_solution_element(sols: Solution, idx: int) -> np.ndarray:
+    """
+    Return a slice of an n_dimensional matrix of solutions of shape (...,n^2-1),
+    where n is the basis size of the quantum system.
+
+    Parameters
+    ----------
+    sols: numpy.ndarray
+        An N-Dimensional numpy array representing the final
+        density matrix, with ground state removed, and written in the totally
+        real equations basis. Can have arbitrary axes preceding density matrix
+        axis.
+    idx: int
+        Solution index to slice.
+
+    Returns
+    -------
+    numpy.ndarray
+        Slice of solutions corresponding to index idx. For example,
+        if sols has shape (..., n^2-1), sol_slice will have shape (...).
+
+    Raises
+    ------
+    IndexError
+        If `idx` in not within the shape determined by basis size.
+
+    Examples
+    --------
+    >>> c = rq.Cell('Rb85', *rq.D2_states('Rb85'))
+    >>> c.add_coupling(states=(0,1), rabi_frequency=1, detuning=1)
+    >>> sols = rq.solve_steady_state(c)
+    >>> print(sols.rho.shape)
+    >>> rho_01 = rq.get_solution_element(sols, 0)
+    >>> print(rho_01)
+    (3,)
+    -0.0013139903428765695
+
+    """
+    basis_size = np.sqrt(sols.rho.shape[-1] + 1)
+    try:
+        sol_slice = sols.rho.take(indices=idx, axis=-1)
+    except IndexError:
+        raise IndexError(f"No element with given index for {basis_size}-level system")
+
+    return sol_slice
+
+
+def get_snr(sensor: Sensor, optical_path_length: float, param_label: str,
+            probe_tuple: Tuple[int, int] = (0, 1),
+            phase_quadrature: bool = False,
+            kappa: Optional[float] = None, eta: Optional[float] = None
+            ) -> Tuple[np.ndarray, Tuple[np.ndarray, ...]]:
+    """
+    Calculate a Sensor's signal-to-noise ratio, in a 1Hz bandwidth,
+    to a specified signal parameter.
+
+    SNR is calculated with respect to the signal parameter,
+    relative to the inital value of the signal parameter.
+    The returned mesh is similarly transformed from the typical sensor mesh,
+    by replacing the total value of the signal parameter
+    with the deviation in the signal parameter (relative
+    to it's initial array value).
+
+    The conventions used follow that of [1]_.
+
+    Parameters
+    ----------
+    sensor : :class:`Sensor`
+        sensor for which SNR should be calculated. The definition
+        of sensor.couplings should contain at least one coupling with a list-like
+        parameter. For the list-like parameter, the first array element is the
+        "base" against which SNR for each other value is calculated.
+    optical_path_length : int
+        Sensor optical path length in meters.
+    param_label : str
+        Label of the axis with respect to which SNR is calculated.
+        See :meth:`Sensor.axis_labels` for more details on axis labeling. The
+        value corresponding to this label should be the list-like parameter
+        with respect to which SNR should be calculated.
+        This parameter list must have at least two elements,
+        and SNR is calculated relative to the first element in the list
+        for all other elements in the list.
+    probe_tuple : tuple
+        Two-integer tuple specifying the probing transition.
+    phase_quadrature : :obj:`bool`, optional
+        Whether the sensor is measured in the
+        phase quadrature of the probe laser. False denotes measurement in the
+        amplitude quadrature.  Default is False.
+    kappa: float, optional
+        Differential prefactor, in units of (Mrad/s)/m.
+        Must be specified when using :class:`Sensor`.
+    eta: float, optional
+        Noise density prefactor, in units of root(Hz)
+        Must be specified when using :class:`Sensor`.
+
+    Returns
+    -------
+        snrs : numpy.ndarray
+            Array of SNRs for the sensor with respect to the change
+            in the signal parameter.  Calculated in units of amplitude relative
+            to noise standard deviation.
+        mesh : tuple(numpy.ndarray)
+            Numpy meshgrid of the coupling parameters that yield each
+            snr.  The signal parameter axis now shows the signal change.
+
+    Raises
+    ------
+    ValueError
+        If the specified param_label is not in `Sensor.axis_labels()`
+
+    Examples
+    --------
+    >>> c = rq.Sensor()
+    >>> c.add_coupling(states=(0,1), rabi_frequency=np.linspace(0, 1, 5), detuning=1)
+    >>> snr, mesh = rq.get_snr(c, 0.01, '(0, 1)_rabi_frequency')
+    >>> print(snr)
+    >>> print(mesh)
+    [     0. 137024. 273980. 410796. 547405.]
+    [array([0., 0., 0., 1., 1.])]
+
+    References
+    ----------
+    .. [1] D. H. Meyer, C. O'Brien, D. P. Fahey, K. C. Cox, and P. D. Kunz,
+       "Optimal atomic quantum sensing using
+       electromagnetically-induced-transparency readout,"
+       Phys. Rev. A, vol. 104, p. 043103, 2021.
+    """
+    if (sensor.eta is not None or sensor.kappa is not None) and (eta is not None or kappa is not None):  # noqa
+        raise ValueError('Cannot provide alternate eta/kappa values from Sensor class')
+    elif eta is None or kappa is None:
+        if sensor.eta is None or sensor.kappa is None:
+            raise ValueError(('Must specify both eta/kappa via arguments '
+                              'to get_snr OR attributes of sensor.'))
+        eta = sensor.eta
+        kappa = sensor.kappa
+
+    labels = sensor.axis_labels()
+    try:
+        sensitivity_axis = labels.index(param_label)
+    except ValueError:
+        raise ValueError(f"{param_label} label is not in sensor.axis_labels()")
+
+    full_sols = solve_steady_state(sensor)
+    rhos_ij = get_rho_ij(full_sols.rho, *probe_tuple[::-1])
+
+    # check that OD isn't high so optically-thin approximation is valid
+    probe_rabi = _get_probe_rabi(sensor, probe_tuple)
+    _ = get_OD(rhos_ij, optical_path_length, probe_rabi, kappa)
+
+    rho_diffs = rhos_ij - np.take(rhos_ij, [0], sensitivity_axis)
+
+    if phase_quadrature:
+        rho_diffs_quadrature = np.abs(np.real(rho_diffs))
+    else:
+        rho_diffs_quadrature = np.abs(np.imag(rho_diffs))
+
+    rho_ij_noise = eta/kappa  # follows directly from eqns 4 and 6 of 2105.10494
+    snrs: np.ndarray = rho_diffs_quadrature/rho_ij_noise*optical_path_length
+
+    mesh = sensor.get_parameter_mesh(sparse=False)
+    mesh[sensitivity_axis] -= np.take(mesh[sensitivity_axis], [0], sensitivity_axis)
+
+    return snrs, mesh
+
+
+def _get_probe_rabi(sensor: Sensor,
+                    probe_tuple: Tuple[int, ...] = (0, 1)) -> Union[float, np.ndarray]:
+    """
+    Helper function that returns the correct probe Rabi frequency
+    from a Sensor for use in functions that return experimental values.
+
+    Parameters
+    ----------
+    sensor: :class:`~.Sensor`
+        Sensor object that has the probe coupling defined
+    probe_tuple: tuple of int
+        The tuple that defines the probing coupling to extract
+
+    Returns
+    -------
+    probe_rabi: float of numpy.ndarray
+        Probe Rabi frequency defined in the Sensor
+
+    Warns
+    -----
+    UserWarning
+        If the probe coupling has time dependence.
+        In this case, the returned Rabi frequency may not be well defined.
+    
+    """
+    probe_coupling = sensor.couplings.edges[probe_tuple]
+
+    if probe_coupling.get('time_dependence', False):
+        warnings.warn(('Probe is time dependent.  Output of _get_probe_rabi '
+                       'is not guaranteed to be well defined.'))
+
+    rabi = probe_coupling.get('rabi_frequency', None)
+    if isinstance(rabi, (list, np.ndarray)):
+
+        # get Rabi from parameter mesh so broadcasting works
+        probe_label = probe_coupling['label']
+
+        # get index in mesh for the scanned Rabi frequency
+        labels = sensor.axis_labels()
+        mesh_index = labels.index(probe_label+'_rabi_frequency')
+        parameter_mesh = sensor.get_parameter_mesh()
+
+        return parameter_mesh[mesh_index]
+
+    else:
+        # it's just a number
+        return rabi
```

### Comparing `rydiqule-1.0.0/src/rydiqule/sensor.py` & `rydiqule-1.0.0rc2/src/rydiqule/sensor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1793 +1,1777 @@
-"""
-Sensor objects that control solvers.
-"""
-
-import numpy as np
-import networkx as nx  # type: ignore
-import warnings
-
-from .sensor_utils import _get_collapse_str, _combine_parameter_labels
-
-from typing import List, Tuple, Dict, Literal, Callable, Optional, Union
-
-ScannableParameter = Union[float, List[float], np.ndarray]
-
-CouplingDict = Dict
-States = Tuple[int, ...]
-
-BASE_SCANNABLE_KEYS = ["detuning", 
-                       "rabi_frequency", 
-                       "phase", 
-                       "transition_frequency"]
-"""Reference list of all coherent coupling keys that support rydiqules stacking convention.
-Note that all decoherence keys (keys beginning with `gamma_`) are supported, but handled separately.
-"""
-
-BASE_EDGE_KEYS = ["states",
-                   "detuning", 
-                   "rabi_frequency",
-                   "transition_frequency",
-                   "phase",
-                   "kvec",
-                   "time_dependence",
-                   "label",
-                   "dipole_moment"]
-"""Reference list of all keys that can be specified with values in a coherenct coupling.
-Subclasses which inherit from :class:`~.Sensor` should override the `valid_parameters` attribute,
-NOT this list. The `valid_parameters` attribute is initialized as a copy of `BASE_EDGE_KEYS`."""
-
-class Sensor():
-    """
-    Class that contains minimum information necessary to run the solvers.
-
-    Consider this class the theorist's interface to the solvers.
-    It requires nearly complete, explicit specification of inputs.
-    This allows for very fine control of the solvers,
-    including the ability to solve systems that are not entirely physical.
-    
-    """
-
-    eta: Optional[float] = None
-    """Noise density prefactor, in units of root(Hz).
-    Must be specified when using :class:`Sensor`.
-    Automatically calculated when using :class:`Cell`."""
-
-    kappa: Optional[float] = None
-    """Differential prefactor, in units of (Mrad/s)/m.
-    Must be specified when using :class:`Sensor`.
-    Automatically calculated when using :class:`Cell`."""
-
-    def __init__(self, basis_size: int, *couplings: CouplingDict) -> None:
-        """
-        Initializes the Sensor of the specified basis size.
-
-        Parameters
-        ----
-        basis_size : int 
-            Number of states in the basis.
-        *couplings : tuple(dict) 
-            Couplings dictionaries to pass to :meth:`~.add_couplings` on sensor construction.
-        
-        Raises
-        ------
-        TypeError
-            If `basis_size` is not an integer.
-        
-        """
-        if type(basis_size) != int:
-            raise TypeError("basis_size must be an integer")
-        
-        self.basis_size = basis_size
-
-        self.couplings = nx.DiGraph()
-        self.couplings.add_nodes_from(range(self.basis_size))
-
-        if len(couplings) > 0:
-            self.add_couplings(*couplings)
-
-        self._zipped_parameters: List[List[str]] = []
-        self.valid_parameters = BASE_EDGE_KEYS.copy()
-
-
-    def add_coupling(
-            self, states: States, rabi_frequency: Optional[ScannableParameter] = None,
-            detuning: Optional[ScannableParameter] = None,
-            transition_frequency: Optional[float] = None,
-            phase: Optional[ScannableParameter] = 0,
-            kvec: Tuple[float,float,float] = (0,0,0),
-            time_dependence: Optional[Callable[[float],float]] = None,
-            label: Optional[str] = None,
-            **extra_kwargs) -> None:
-        """
-        Adds a single coupling of states to the system.
-
-        One or more of these paramters can be a list or array-like of values to represent
-        a laser that can take on a set of discrete values during a field scan.
-        Designed to be a user-facing wrapper for :meth:`~._add_coupling` with arguments
-        for states and coupling parameters.
-
-        Parameters
-        ----------
-        states : tuple of ints of length 2
-            The pair of states of the sensor which the state couples
-            Must be a tuple of intergers of length 2, and the integers must
-            be unique indicies within the basis.
-        rabi_frequency : float or complex, or list-like of float or complex
-            The rabi frequency of the field being added. Defined in units of Mrad/s. List-like
-            values will invoke Rydiqule's stacking convention when relevant quantities are calculated.
-        detuning : float or list-like of floats or  None, optional 
-            The frequency difference between the transition frequency and the field frequency in 
-            units of Mrad/s. List-like values will invoke Rydiqule's stacking convention when relevant 
-            quantities are calculated. If specified, the coupling is treated with the rotating-wave 
-            approximation rather than in the lab frame, and `transition_frequency` is ignored if present.
-        transition_frequency : float or list-like of floats or None, optional 
-            The transition frequency between a particular pair of states. List-like
-            values will invoke Rydiqule's stacking convention when relevant quantities are calculated. 
-            Only used directly in calculations if `detuning` is `None`, ignored otherwise. 
-            Note that on its own, it only defines the spacing between two energy levels and not the
-            field itsself. To define a field, the `time_dependence` argument must be specified, or else 
-            the off-diagonal terms to drive transitions will not be generated in the Hamiltonian matrix.
-        phase : float, optional
-            The relative phase of the field in radians. Defaults to zero.
-        kvec : iterable, optional 
-            A three-element iterable that defines the atomic doppler shift on a particular coupling
-            field. It should have magntiude equal to the doppler shift (in the units of Mrad/s) of a
-            n atom moving at the Maxwell-Boltzmann distribution most probable speed, `vP=np.sqrt(2*kB*T/m)`. 
-            I.E. `np.linalg.norm(kvec)=2*np.pi/lambda*vP`. If equal to `(0,0,0)`, solvers will ignore 
-            doppler shifts on this field.  Defaults to `(0,0,0)`.
-        time_dependence : scalar function, optional
-            A scalar function specifying a time-dependent field. The time dependence function is defined 
-            as a python funtion that returns a unitless value as a function of time (in microseconds) 
-            that is multiplied by the `rabi_frequency` parameter to get a  field strength scaled to units 
-            of Mrad/s.
-        label : str or None, optional
-            Name of the coupling. This does not change any calculations, but can be used 
-            to help track individual couplings, and will be reflected in the output of 
-            :meth:`~.Sensor.axis_labels`, and to specify zipping for :meth:`~.Sensor.zip_couplings`. 
-            If `None`, the label is generated as the value of `states` cast to a string with 
-            whitespace removed. Defaults to `None`.
-
-        Raises
-        ------
-        ValueError
-            If `states` cannot be interpreted as a tuple.
-        ValueError
-            If `states` does not have a length of 2.
-        ValueError
-            If the state numbers specified by `states` are beyond the basis size.
-            For example, calling this function with `states=(3,4)`
-            will raise this error if the basis size is equal to 3.
-        ValueError
-            If both `rabi_frequency` and `dipole_moment` are specified or if
-            neither are specified.
-        ValueError
-            If both detuning and transition_frequency are specified or if
-            neither are specified.
-
-        Examples
-        --------
-        >>> s = rq.Sensor(2)
-        >>> s.add_coupling(states=(0,1), detuning=1, rabi_frequency=2)
-
-        >>> s = rq.Sensor(2)
-        >>> s.add_coupling(states=(0,1), detuning=np.linspace(-10, 10, 101), rabi_frequency=2, label="laser")
-
-        >>> s = rq.Sensor(2)
-        >>> step = lambda t: 1 if t>=1 else 0
-        >>> s.add_coupling(states=(0,1), transition_frequency=1000, rabi_frequency=2, time_dependence=step)
-
-        >>> s = rq.Sensor(2)
-        >>> kp = 250*np.array([1,0,0])
-        >>> s.add_coupling(states=(0,1), detuning=1, rabi_frequency=2, kvec=kp)
-
-        """ # noqa
-
-        if states[0] == states[1]:
-            raise ValueError('Coherent coupling must couple different states.')
-
-        suppress_rwa = extra_kwargs.pop("suppress_rwa_warn", False)
-
-        field_params = {k:v for k,v in locals().items()
-                        if k in self.valid_parameters
-                        and v is not None}
-        
-        if not (detuning is not None) ^ (transition_frequency is not None):
-            msg = """Please specify \'detuning\' for a field under the RWA or
-                \'transition_frequency\' for a coupling without the approximation,
-                but not both."""
-            raise ValueError(msg)
-
-        if detuning is None and np.abs(transition_frequency) > 5000 and not suppress_rwa:
-            msg = "Not using the rotating wave approximation for large transition frequencies "\
-                "can result in prohibitively long computation times. Specify detuning to use the"\
-                " rotating wave approximation or passing \"suppress_rwa_warn=True\" to"\
-                " add_coupling() to suppress this warning."
-
-            with warnings.catch_warnings():
-                warnings.simplefilter("always")
-                warnings.warn(msg, stacklevel=2)
-
-        self._add_coupling(**field_params, **extra_kwargs)
-
-
-    def add_couplings(self, *couplings: CouplingDict,
-                        **extra_kwargs) -> None:
-        """
-        Add any number of couplings between pairs of states.
-        
-        Acts as an alternative to calling :meth:`~.Sensor.add_coupling`
-        individually for each pair of states.
-        Can be used interchangably up to preference,
-        and all of keyword :meth:`~.Sensor.add_coupling` are supported dictionary
-        keys for dictionaries passed to this function.
-
-        Parameters
-        ----------
-        couplings : tuple of dicts
-            Any number of dictionaries, each specifying the parameters of a single field 
-            coupling 2 states. For more details on the keys of each dictionry see the arguments 
-            for :meth:`~.Sensor.add_coupling`. Equivalent to passing each dictiories keys and 
-            values to :meth:`~.Sensor.add_coupling` individually.
-        **extra_kwargs : dict
-            Additional keyword-only arguments to pass to the relevant `add_coupling` method.
-            The same arguments will be passed to each call of :meth:`~.Sensor.add_coupling`.
-            Often used for warning suppression.
-
-        Raises
-        ------
-        ValueError
-            If the `states` parameter is missing.
-
-        Examples
-        --------
-        >>> s = rq.Sensor(3)
-        >>> blue = {"states":(0,1), "rabi_frequency":1, "detuning":2}
-        >>> red = {"states":(1,2), "rabi_frequency":3, "detuning":4}
-        >>> s.add_couplings(blue, red)
-        >>> print(s.couplings.edges(data=True))
-        [(0, 1, {'rabi_frequency': 1, 'detuning': 2, 'phase': 0, 'kvec': (0, 0, 0)}),
-        (1, 2, {'rabi_frequency': 3, 'detuning': 4, 'phase': 0, 'kvec': (0, 0, 0)})]
-
-        """
-        for c in couplings:
-            c_copy = c.copy()
-            try:
-                states = self._states_valid(c_copy.pop('states'))
-            except KeyError:
-                raise ValueError("\'states\' parameter must be specified for any field")
-
-            self.add_coupling(states=states, **c_copy, **extra_kwargs)
-
-
-    def _add_coupling(self, states: States, **field_params) -> None:
-        """
-        Function for internal use which will ensure the supplied couplings is valid,
-        add the field to self.couplings. 
-        
-        Exists to abstract away some of the internally necessary bookkeeping functionality from
-        user-facing classes. 
-
-        Parameters
-        ----------
-            states : tuple
-                The integer pair of states to be coupled.
-            **field_params : dict
-                The dictionry of couplings parameters. For details
-                on the keys of the dictionry see :meth:`~.Sensor.add_coupling`.
-
-        """
-        states = self._states_valid(states)
-
-        # if label not provided, set to default value of states tuple as a str
-        if field_params.get("label") is None:
-            field_params["label"] = str(states).replace(" ","")
-
-        # remove all coherent data in both directions on the graph
-        # this prevents adding coherent couplings in both directions between 2 nodes
-        self._remove_edge_data(states, 'coherent')
-        self._remove_edge_data(states[::-1], 'coherent')
-
-        self.couplings.add_edge(*states, **field_params)
-
-
-    def zip_parameters(self, *labels: str) -> None:
-        """
-        Define 2 scannable parameters as "zipped" so they are scanned in parallel.
-
-        Zipped parameters will share an axis when quantities relevant to the equations of
-        motion, such as the `gamma_matrix` and `hamiltonian` are generated. Note that calling
-        this function does not affect internal quanties directly, but adds their labels together
-        in the internal `self._zipped_parameters` list, and they are zipped at calculation time
-        for `hamiltonian` and `decoherence_matrix`.
-
-        Parameters
-        ----------
-        labels : str
-            Parameter labels to scan together. Parameter labels are strings of the form 
-            `"<coupling_label>_<parameter_name>"`, such as `"(0,1)_detuning"`.
-            Must be at least 2 labels to zip.
-
-        Raises
-        ------
-        ValueError
-            If fewer than 2 labels are provided.
-        ValueError
-            If any of the 2 labels are the same.
-        ValueError
-            If any elements of `labels` are not labels of couplings in the sensor.
-        ValueError
-            If any of the parameters specified by labels are already zipped.
-        ValueError
-            If any of the parameters specified are not list-like.
-        ValueError
-            If all list-like parameters are not the same length.
-
-        Notes
-        -----
-        .. note::
-            This function should be called last after all Sensor couplings and dephasings
-            have been added. Changing a coupling that has already been zipped removes it from
-            the `self.zipped_parameters` list.
-            
-        .. note::
-            Modifying the `Sensor.zipped_parameters` attribute directly can break some functionality
-            and should be avoided. Use this function or :meth:`~.Sensor.unzip_parameters` instead. 
-
-        Examples
-        --------
-        >>> s = rq.Sensor(3)
-        >>> det = np.linspace(-1,1,11)
-        >>> s.add_coupling(states=(0,1), detuning=det, rabi_frequency=1, label="probe")
-        >>> s.add_coupling(states=(1,2), detuning=det, rabi_frequency=1)
-        >>> s.zip_parameters("probe_detuning", "(1,2)_detuning")
-        >>> print(s._zipped_parameters) #NOT modifying directly
-        [['(1,2)_detuning', 'probe_detuning']]
-
-        """
-        # check for at least 2 labels
-        if len(labels) < 2:
-            raise ValueError(("Please provide at least 2 parameter labels "
-                              f"to zip (only provided {len(labels)})"))
-            
-        #check that all labels are unique
-        if len(labels) != len(set(labels)): #set will be shorter if there are duplicates
-            raise ValueError("parameters cannot be zipped to themselves")
-        
-        #check if any labels are already zipped
-        new_label_array = np.expand_dims(labels, (-1,-2))
-        current_zipped_params = np.expand_dims(self._zipped_parameters, 0)
-        
-        # see if ANY provided label is currently zipped
-        if len(self._zipped_parameters)>0 and np.any(new_label_array==current_zipped_params):
-
-            for l in labels: #if so, find which label for error reporting
-                if l in current_zipped_params:
-                    raise ValueError(f"Label {l} has already been zipped with another parameter")
-
-        #ensure provided labels are valid for zipping
-        previous_len = 0
-        for l in labels:
-            
-            coupling, param = l.split("_", 1)
-            #make sure the label exists
-            try:
-                states = self._coupling_with_label(coupling)
-            except ValueError:
-                raise ValueError(f"{coupling} is not a label of any coupling in this sensor")
-            
-            #make sure parameter exists and is an array
-            try:
-                _ = self.couplings.edges[states][param]
-            except KeyError:
-                raise ValueError(f"Coupling {coupling} has no parameter {param}")
-            if not hasattr(param, "__len__"):
-                raise ValueError(f"Parameter {l} is not list-like and cannot be zipped")
-            
-            #make sure parameters are the same length
-            current_len = len(self.couplings.edges[states][param])
-            if previous_len > 0 and current_len != previous_len:
-                raise ValueError(
-                    f"Got length {current_len} for parameter \"{l}\", "
-                    f"but \"{labels[0]}\" is length {previous_len}")
-            
-            previous_len = current_len
-                        
-        labels = list(labels)
-        labels.sort()
-        self._zipped_parameters.append(labels)
-
-
-    def unzip_parameters(self, *labels: str, **extra_kwargs):
-        
-        """
-        Remove a set of zipped parameters from the internal zipped_parameters list.
-
-        If an element of the internal `_zipped_parameters` array matches ALL labels provided,
-        removes it from the internal `zipped_parameters` method. If no such element is
-        in `_zipped_parameters`, does nothing.
-
-        Parameters
-        ----------
-        labels : str 
-            Any number of string labels matching ALL the names of a set of parameters
-            that has already been zipped.
-        **extra_kwargs: dict
-            Optional Extra keyword-only arguments. Supported argument is
-              - verbose (str): Whether to print if there are no parameters matching `labels`
-                in `_zipped_parameters`. Defaults to `True`.
-        
-        Notes
-        -----
-        .. note::
-            This function should always be used rather than modifying the `_zipped_parameters`
-            attribute directly.
-            
-        Examples
-        --------
-        >>> s = rq.Sensor(3)
-        >>> det = np.linspace(-1,1,11)
-        >>> s.add_coupling(states=(0,1), detuning=det, rabi_frequency=1, label="probe")
-        >>> s.add_coupling(states=(1,2), detuning=det, rabi_frequency=1)
-        >>> s.zip_parameters("probe_detuning", "(1,2)_detuning")
-        >>> print(s._zipped_parameters) #NOT modifying directly
-        >>> s.unzip_parameters('(1,2)_detuning', 'probe_detuning')
-        >>> print(s._zipped_parameters) #NOT modifying directly
-        [['(1,2)_detuning', 'probe_detuning']]
-        []
-        
-        If the labels provided are not a match, a message is printed and nothing is altered. 
-        
-        >>> s = rq.Sensor(3)
-        >>> det = np.linspace(-1,1,11)
-        >>> s.add_coupling(states=(0,1), detuning=det, rabi_frequency=1, label="probe")
-        >>> s.add_coupling(states=(1,2), detuning=det, rabi_frequency=1)
-        >>> s.zip_parameters("probe_detuning", "(1,2)_detuning")
-        >>> print(s._zipped_parameters) #NOT modifying directly
-        >>> s.unzip_parameters('green_detuning', 'probe_detuning')
-        >>> print(s._zipped_parameters) #NOT modifying directly
-        [['(1,2)_detuning', 'probe_detuning']]
-        No zipped parameters matching ['green_detuning', 'probe_detuning']
-        [['(1,2)_detuning', 'probe_detuning']]
-        
-        """
-        labels = list(labels)
-        labels.sort()
-        
-        verbose = extra_kwargs.get("verbose", True)
-
-        for i, param_list in enumerate(self._zipped_parameters):
-            if labels == param_list:
-                del self._zipped_parameters[i]
-                return
-        
-        if verbose:
-            print(f"No zipped parameters matching {labels}")
-
-
-    def add_decoherence(self, states: Tuple[int, ...], gamma: ScannableParameter,
-                        label: Optional[str] = None) -> None:
-        """
-        Add decoherent coupling to the graph between two states.
-
-        If `gamma` is list-like, the sensor will scan over the values,
-        solving the system for each different gamma.
-
-        Parameters
-        ----------
-        states : tuple of ints
-            Length-2 tuple of integers corresponding to the two states. The first
-            value is the number of state out of which population decays, and the 
-            second is the number of the state into which population decays.
-        gamma : float or sequence
-            The decay rate, in Mrad/s.
-        label : str or None, optional
-            Optional label for the decay. If `None`, decay will be stored on
-            the graph edge as `"gamma"`. Otherwise, will cast as a string and decay will be stored
-            on the graph edge as `"gamma_"+label`.
-
-        Notes
-        -----
-        .. note::
-            Adding a decoherece with a particular label (including `None`) will override an existing
-            decoherent transition with that label.
-            
-        Examples
-        --------
-        s = rq.Sensor(3)
-        >>> s.add_coupling(states=(0,1), detuning=1, rabi_frequency=1)
-        >>> s.add_coupling(states=(1,2), detuning=1, rabi_frequency=1)
-        >>> s.add_decoherence((2,0), 0.1, label="misc")
-        >>> print(s.decoherence_matrix())
-        [[0.  0.  0. ]
-        [0.  0.  0. ]
-        [0.1 0.  0. ]]
-        
-        Decoherence values can also be scanned. Here decoherece from states 2->0 is scanned
-        between 0 and 0.5 for 11 values. We can also see how the Hamiltonian shape accounts
-        for this to allow for clean broadcasting, indicating that the hamiltonian is identical
-        accross all decoherence values.
-        
-        >>> s = rq.Sensor(3)
-        >>> gamma = np.linspace(0,0.5,11)
-        >>> s.add_coupling(states=(0,1), detuning=1, rabi_frequency=1)
-        >>> s.add_coupling(states=(1,2), detuning=1, rabi_frequency=1)
-        >>> s.add_decoherence((2,0), gamma)
-        >>> print(s.decoherence_matrix().shape)
-        (11, 3, 3)
-        >>> print(s.get_hamiltonian().shape)
-        (11, 3, 3)
-
-        """
-        if label is None:
-            label_full = "gamma"
-        else:
-            label_full = "gamma_" + str(label)
-
-        states = self._states_valid(states)
-        # invalidate existing decoherence data if already exists
-        self._remove_edge_data(states, kind=label_full)
-        self.couplings.add_edge(*states, **{label_full:gamma})
-
-        # if edge doesn't have a label (ie decoherence only), add a default label
-        if self.couplings.edges[states].get("label") is None:
-            self.couplings.edges[states]["label"] = str(states).replace(" ", "")
-
-
-    def add_transit_broadening(self, gamma_transit: ScannableParameter,
-                               repop: Dict[int, float] = {0: 1.0}) -> None:
-        """
-        Adds transit broadening by adding a decoherence from each node to ground.
-        
-        For each graph node n, adds a decoherent transition from n the specified state
-        (0 by default) using the :meth:`~.Sensor.add_decoherence` method with the `"transit"` label.
-        See :meth:`~.Sensor.add_decoherence` for more details on labeling.
-
-        If an array of transit values are provided, they will be automatically zipped together
-        into a single scanning element.
-
-        Parameters
-        ----------
-        gamma_transit: float or sequence
-            The transit broadening rate in Mrad/s.
-        repop: dict, optional
-            Dictionary of states for transit to repopulate in to.
-            The keys represent the state labels. The values represent
-            the fractional amount that goes to that state.
-            If the sum of values does not equal 1, population will not be conserved.
-            Default is to repopulate everything into state 0.
-
-        Warns
-        -----
-        If the values of the `repop` parameter do not sum to 1, thus meaning
-        population will not be conserved.
-        
-        Examples
-        --------
-        >>> s = rq.Sensor(3)
-        >>> s.add_transit_broadening(0.1)
-        >>> print(s.couplings.edges(data=True))
-        >>> print(s.decoherence_matrix())
-        [(0, 0, {'gamma_transit': 0.1}), (1, 0, {'gamma_transit': 0.1}), (2, 0, {'gamma_transit': 0.1})]
-        [[0.1 0.  0. ]
-        [0.1 0.  0. ]
-        [0.1 0.  0. ]]
-
-        """  # noqa
-        if isinstance(gamma_transit, list):
-            # needed for multiplying branching ratios
-            gamma_transit = np.array(gamma_transit)
-
-        if not np.isclose(sum(repop.values()), 1.0):
-            warnings.warn(('Repopulation branching ratios do not sum to 1!'
-                           ' Population will not be conserved.'))
-
-        for t, br in repop.items():
-            for i in range(self.basis_size):
-                self.add_decoherence((i, t), gamma=gamma_transit*br, label="transit")
-
-        if isinstance(gamma_transit, (list,np.ndarray)):
-            # need to zip together all the transit rates
-            axes = self.axis_labels()
-            transit_axes = [s for s in axes if s.endswith('gamma_transit')]
-            self.zip_parameters(*transit_axes)
-
-
-    def add_self_broadening(self, node: int, gamma: ScannableParameter,
-                            label: Optional[str] = "self") -> None:
-        """
-        Specify self-broadening (such as collisional broadening) of a level.
-
-        Equivalent to calling :meth:`~.Sensor.add_decoherence` and specifying both
-        states to be the same, with the "self" label. For more complicated systems,
-        it may be useful to further specify the source of self-broadening as, for
-        example, "collisional" for easier bookkeeping and to ensure no values
-        are overwritten.
-
-        Parameters
-        ----------
-        node: int
-            The integer number of the state node to which the broadening
-            will be added. The integer corresponds to the state's position in
-            the graph.
-        gamma: float or sequence
-            The broadening width to be added in Mrad/s.
-        label: str, optional
-            Optional label for the state. If `None`, decay will be stored on
-            the graph edge as `"gamma"`. Otherwise, will cast as a string
-            and decay will be stored on the graph edge as `"gamma_"+label`
-
-        Notes
-        -----
-        .. note::
-            Just as with the :meth:`~.Sensor.add_decoherence` function, adding a decoherence
-            value with a label that already exists will overwrite an existing decoherent
-            transition with that label. The "self" label is applied to this function
-            automatically to help avoid an unwanted overwrite.
-            
-        Examples
-        --------
-        >>> s = rq.Sensor(3)
-        >>> s.add_self_broadening(1, 0.1)
-        >>> print(s.couplings.edges(data=True))
-        >>> print(s.decoherence_matrix())
-        [(1, 1, {'gamma_self': 0.1, 'label': '(1,1)'})]
-        [[0.  0.  0. ]
-        [0.  0.1 0. ]
-        [0.  0.  0. ]]
-
-        """
-        self.add_decoherence((node, node), gamma, label=label)
-
-
-    def decoherence_matrix(self) -> np.ndarray:
-        """
-        Build a decoherence matrix out of the decoherence terms of the graph.
-
-        For each edge, sums all parameters with a key that begins with "gamma",
-        and places it on the appropriate location in an adjacency matrix for the
-        `couplings` graph.
-        
-        Returns
-        -------
-        numpy.ndarray
-            The decoherence matrix stack of the system.
-
-        Examples
-        --------
-        >>> s = rq.Sensor(3)
-        >>> s.add_decoherence((1,0), 0.2, label="foo")
-        >>> s.add_decoherence((1,0), 0.1, label="bar")
-        >>> s.add_decoherence((2,0), 0.05)
-        >>> s.add_decoherence((2,1), 0.05)
-        >>> print(s.couplings.edges(data=True))
-        >>> print(s.decoherence_matrix())
-        [(1, 0, {'gamma_foo': 0.2, 'label': '(1,0)', 'gamma_bar': 0.1}), (2, 0, {'gamma': 0.05, 'label': '(2,0)'}), (2, 1, {'gamma': 0.05, 'label': '(2,1)'})]
-        [[0.   0.   0.  ]
-        [0.3  0.   0.  ]
-        [0.05 0.05 0.  ]]
-        
-        Decoherences can be stacked just like any parameters of the Hamiltonian:
-        
-        >>> s = rq.Sensor(3)
-        >>> gamma = np.linspace(0,0.5, 11)
-        >>> s.add_decoherence((1,0), gamma)
-        >>> print(s.decoherence_matrix().shape)
-        (11,3,3)   
-             
-        """  # noqa
-        base_couplings = self.couplings.copy()
-
-        stack_shape = self._stack_shape(collapse=False)
-        for states, param, arr in self.variable_parameters(apply_mesh=True):
-            self.couplings.edges[states][param] = arr
-
-        gamma_shape = (*stack_shape, self.basis_size, self.basis_size)
-        gamma_matrix = np.zeros(gamma_shape, np.float64)
-
-        # get a list of all unique parameter labels containing "gamma"
-        labels_lists = [list(d.keys()) for _,_,d in self.couplings.edges(data=True)]
-        all_labels = list(set(sum(labels_lists, start=[])))
-        decoherence_labels = [l for l in all_labels if "gamma" in l]
-
-        # for each unique decoherence name,
-        for label in decoherence_labels:
-            for states, f in self.couplings_with(label).items():
-
-                idx = (..., *states)
-                gamma_matrix[idx] += f[label]
-
-        if len(self._zipped_parameters) > 0:
-            gamma_matrix = self.collapse_dims(gamma_matrix)
-
-        self.couplings = base_couplings
-        return gamma_matrix
-
-
-    def axis_labels(self, collapse: bool = True) -> List[str]:
-        """
-        Get a list of axis labels for stacked hamiltonians. 
-        
-        The axes of a hamiltonian
-        stack are defined as the axes preceding the usual hamiltonian, which are always
-        the last 2. These axes only exist if one of the parametes used to define
-        a Hamiltonian are lists.
-
-        Be default, labels which have been zipped using :meth:`~.Sensor.zip_parameters`
-        will be combined into a single label, as this is how :meth:`~.Sensor.get_hamiltonian`
-        treats these axes.
-
-        Returns
-        -------
-        list of str 
-            Strings corresponding to the label of each axis on a stack
-            of multiple hamiltonians.
-
-        Examples
-        --------
-        There are no preceding axes if there are no list-like parameters.
-
-        >>> s = rq.Sensor(3)
-        >>> blue = {"states":(0,1), "rabi_frequency":1, "detuning":2}
-        >>> red = {"states":(1,2), "rabi_frequency":3, "detuning":4}
-        >>> s.add_couplings(blue, red)
-        >>> print(s.get_hamiltonian().shape())
-        >>> print(s.axis_labels())
-        (3,3)
-        []
-
-        Adding list-like parameters expands the hamiltonian
-
-        >>> s = rq.Sensor(3)
-        >>> det = np.linspace(-10, 10, 11)
-        >>> blue = {"states":(0,1), "rabi_frequency":1, "detuning":det, "label":"blue"}
-        >>> red = {"states":(1,2), "rabi_frequency":3, "detuning":det}
-        >>> s.add_couplings(blue, red)
-        >>> print(s.get_hamiltonian().shape)
-        >>> print(s.axis_labels())
-        (11, 11, 3, 3)
-        ['blue_detuning', '(1, 2)_detuning']
-
-        Zipping parameters combines their corresponding labels, since their Hamiltonians now 
-        lie on a single axis of the stack. Here the axis of length 7 (axis 0) corresponds to the
-        rabi frequencies and the axis of shape 11 (axis 1) corresponds to the zipped detunings
-        
-        >>> s = rq.Sensor(3)
-        >>> s.add_coupling(states=(0,1), detuning=np.arange(11), rabi_frequency=np.linspace(-3, 3, 7))
-        >>> s.add_coupling(states=(1,2), detuning=0.5*np.arange(11), rabi_frequency=1)
-        >>> s.zip_parameters("(0,1)_detuning", "(1,2)_detuning")
-        >>> print(s.get_hamiltonian().shape)
-        >>> print(s.axis_labels())
-        (7, 11, 3, 3)
-        ['(0,1)_rabi_frequency', '(0,1)_detuning|(1,2)_detuning']
-        
-        """  # noqa
-        axis_labels = []
-
-        # build the base list of axis labels based just on couplings
-        for states, param, _ in self.variable_parameters():
-            if 'label' in self.couplings.edges[states].keys():
-                label = str(self.couplings.edges[states]['label']) + '_' + str(param)
-            else:
-                label = str(states) + "_" + str(param)
-            axis_labels.append(label)
-
-        # combine labels for parameters that have been zipped and move to the end of stack
-        if collapse:
-            for params in self._zipped_parameters:
-                new_label = _combine_parameter_labels(*params)
-
-                for p in params:
-                    axis_labels.remove(p)
-
-                axis_labels.append(new_label)
-
-        return axis_labels
-
-
-    def variable_parameters(self, apply_mesh=False):
-        """
-        Property to retrieve the values of parameters that were stored on the graph as arrays.
-
-        Values are returned as a list of tuples in the standard order of pythons default sorting,
-        applied first to the tuple indicating states and then to the key of the parameter itself. 
-        This means that couplings are sorted first by lower state, then by upper state, then 
-        alphabetically by the name of the parameter. 
-
-        Returns
-        -------
-        list of tuples
-            A list of tuples corresponding to the parameters of the systems that are variable 
-            (i.e. stored as an array). They are ordered accordning to states,
-            then according to variable name.
-            Tuple entries of the list take the form `(states, param_name, value)`
-
-        Examples
-        --------
-        >>> s = rq.Sensor(3)
-        >>> vals = np.linspace(-1,2,3)
-        >>> s.add_coupling(states=(1,2), rabi_frequency=vals, detuning=1)
-        >>> s.add_coupling(states=(0,1), rabi_frequency=vals, detuning=vals)
-        >>> for states, key, value in s.variable_parameters():
-        ...     print(f"{states}: {key}={value}")
-        (0, 1): detuning=[-1.   0.5  2. ]
-        (0, 1): rabi_frequency=[-1.   0.5  2. ]
-        (1, 2): rabi_frequency=[-1.   0.5  2. ]
-        
-        """
-        l=[]
-        for states in sorted(self.couplings.edges):
-            
-            edge_data = self.couplings.edges.get(states)
-            
-            for key, value in sorted(edge_data.items()):
-                if not key.startswith("gamma") and key not in BASE_SCANNABLE_KEYS:
-                    continue
-
-                if isinstance(value, (list,np.ndarray)):
-                    l.append((states, key, value))
-        
-        if apply_mesh:
-            vals = [val for _,_,val in l]
-            mesh_vals = np.meshgrid(*vals, indexing='ij', sparse=True)
-            l = [(*l[i][:2], mesh_vals[i].copy()) for i in range(len(l))]
-
-        return l
-
-
-    def get_parameter_mesh(self, sparse:bool=True, **kwargs) -> Tuple[np.ndarray, ...]:
-        """
-        Returns the parameter mesh of the sensor.
-
-        The parameter mesh is the flattened grid of variable parameters
-        in all the couplings of a sensor.
-        Wraps `numpy.meshgrid` by passing arguments as the variable parameters in a
-        sensor. The `indexing` argument is always `"ij"` for matrix indexing. 
-        For full documention of all arguments, see `numpy.meshgrid` documentation.
-        Argument documentation copied from `numpy.meshgrid`.
-
-        Parameters
-        ----------
-        sparse : bool, optional
-            If `True`, the shape of the returned coordinate array for dimension i is 
-            reduced from `(N1, ..., Ni, ... Nn)` to `(1, ..., 1, Ni, 1, ..., 1)`. 
-            These sparse coordinate grids are intended to be used in a way consistent 
-            with numpy's broadcasting conventions. When all coordinates are used in an 
-            expression, broadcasting still leads to a fully-dimensonal result array. 
-            Recommended to keep as `True`. Default is `True`.
-        kwargs : dict, optional
-            Additional keyword arguments to pass to `numpy.meshgrid`. All arguments are 
-            passed directly to `numpy.meshgrid` with the exception of `indexing`, which 
-            is fixed to `"ij"` and cannot be specified.
-            
-        Examples
-        --------
-        >>> s = rq.Sensor(3)
-        >>> rabi1 = np.linspace(-1,1,11)
-        >>> rabi2 = np.linspace(-2,2,21)
-        >>> s.add_coupling(states=(0,1), rabi_frequency=rabi1, detuning=1)
-        >>> s.add_coupling(states=(1,2), rabi_frequency=rabi2, detuning=1)
-        >>> for p in s.get_parameter_mesh():
-        ...     print(p.shape)
-        (11, 1)
-        (1, 21)
-        
-        """
-        if "indexing" in kwargs.keys():
-            raise TypeError("get_parameter_mesh() got an unexpected keyword argument \'indexing\'")
-
-        vals = [v for _,_,v in self.variable_parameters()]
-
-        parameter_mesh = np.meshgrid(*vals, indexing='ij', sparse=sparse, **kwargs)
-        return parameter_mesh
-
-
-    def get_hamiltonian(self) -> np.ndarray:
-        """
-        Creates the Hamiltonians from the couplings defined by the fields.
-
-        They will only be the steady state hamiltonians, i.e. will only contain
-        terms which do not vary with time. Implicitly creates hamiltonians in "stacks"
-        by creating a grid of all supported coupling parameters which are lists.
-        This grid of parameters will not contain rabi-frequency parameters which
-        vary with time and are defined as list-like. Rather, the associated axis
-        will be of length 1, with the scanning over this value handled by the
-        :meth:`~Sensor.get_time_couplings` function.
-
-        For m list-like parameters x1,x2,...,xm with shapes N1,N2,...,Nm, and basis
-        size n, the output will be shape `(N1,N2,...,Nm, n, n)`. The dimensions
-        N1,N2,...Nm are labeled by the output of :meth:`~.Sensor.axis_labels`.
-
-        If any parameters have been zipped with the :meth:`~.Sensor._zip_parameters`
-        method, those parameters will share an axis in the final hamiltonian stack.
-        In this case, if axis N1 and N2 above are the same shape and zipped, the final
-        Hamiltonian will be of shape `(N1,...,Nm, n, n)`
-        
-        See rydiqule's conventions for matrix stacking for more details.
-
-        Returns
-        -------
-        np.ndarray
-            The complex hamiltonian stack for the sensor.
-
-        Examples
-        --------
-        >>> s = rq.Sensor(3)
-        >>> det = np.linspace(-1,1,11)
-        >>> blue = {"states":(0,1), "rabi_frequency":1, "detuning":det}
-        >>> red = {"states":(1,2), "rabi_frequency":3, "detuning":det}
-        >>> s.add_couplings(red, blue)
-        >>> print(s.get_hamiltonian().shape)
-        (11, 11, 3, 3)
-        
-        Time dependent couplings are handled separately. The axis that contains array-like
-        parameters with time dependence is length 1 in the steady-state Hamiltonian.
-        
-        >>> s = rq.Sensor(3)
-        >>> rabi = np.linspace(-1,1,11)
-        >>> step = lambda t: 0 if t<1 else 1
-        >>> blue = {"states":(0,1), "rabi_frequency":rabi, "detuning":1}
-        >>> red = {"states":(1,2), "rabi_frequency":rabi, "detuning":0, 'time_dependence': step}
-        >>> s.add_couplings(red, blue)
-        >>> print(s.get_hamiltonian().shape)
-        (11, 1, 3, 3)
-
-        Zipping parameters means they share an axis in the Hamiltonian.
-
-        >>> s = rq.Sensor(3)
-        >>> s.add_coupling(states=(0,1), detuning=np.arange(11), rabi_frequency=2)
-        >>> s.add_coupling(states=(1,2), detuning=0.5*np.arange(11), rabi_frequency=1)
-        >>> s.zip_parameters("(0,1)_detuning", "(1,2)_detuning")
-        >>> H = s.get_hamiltonian()
-        >>> print(H.shape)
-        (11, 3, 3)
-
-        """
-        base_couplings = self.couplings.copy()
-
-        stack_shape = self._stack_shape(collapse=False, time_dependence='steady')
-
-        for states, param, arr in self.variable_parameters(apply_mesh=True):
-            # print(states, param, arr.shape)
-            self.couplings.edges[states][param] = arr
-
-        hamiltonian_shape = (*stack_shape, self.basis_size, self.basis_size)
-        # returns diagonal elements of Hamiltonian
-        transition_frequencies = self.get_transition_frequencies()
-        #define hamiltonian and place terms from above on diagonal
-        hamiltonian = np.zeros(hamiltonian_shape, np.complex128)
-        np.einsum("...ii->...i", hamiltonian)[:] = transition_frequencies
-
-        for states, f in self.couplings_with('time_dependence', method='not any').items():
-
-            if 'rabi_frequency' not in f:
-                continue
-
-            idx = (...,*states)
-            conj_idx = (...,*states[::-1])
-
-            # factor of 1/2 accounts for implicit rotating wave approximation
-
-            hamiltonian[idx] = (f['rabi_frequency']*np.cos(f['phase'])
-                                + 1j*f['rabi_frequency']*np.sin(f['phase']))/2
-            hamiltonian[conj_idx] = np.conj(hamiltonian[idx])
-
-        if len(self._zipped_parameters) > 0:
-            hamiltonian = self.collapse_dims(hamiltonian)
-
-        self.couplings = base_couplings
-        return hamiltonian
-
-
-    def collapse_dims(self, stack: np.ndarray) -> np.ndarray:
-        """
-        Collapse dimensions of a stack accoring to the `_zipped_parameters` attribute.
-       
-        Designed primarily for internal use, but can be called externally or
-        in custom overloads of :meth:`~.Sensor.get_hamiltonian`. Effectively performs
-        a `numpy.einsum` operation to replicate `numpy.diag` along the appropriate
-        dimensions. 
-
-        Parameters
-        ----------
-        stack : numpy.ndarray
-            Array with shape matching uncollapsed system hamiltonians. 
-
-        Returns
-        -------
-        numpy.ndarray
-            Input array with appropriate dimensions removed via a numpy.diag-like operation.
-
-        """
-        axis_labels = self.axis_labels(collapse=False)
-
-        paired_axes = []
-
-        for couplings in self._zipped_parameters:
-            paired_axes.append([axis_labels.index(c) for c in couplings])
-
-        einsum_str = _get_collapse_str(len(axis_labels), *paired_axes)
-        collapsed_stack = np.einsum(einsum_str, stack)
-
-        return collapsed_stack
-
-
-    def get_time_hamiltonians(self) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
-        """
-        Get the hamiltonians for the time solver.
-
-        Get both the steady state hamiltonian (as returned by :meth:`~.Sensor.get_hamiltonian`)
-        and the time_dependent hamiltonians (as returned by :meth:`~.Sensor.get_time_couplings`).
-        The time dependent hamiltonians give 2 terms, the hamiltonian corresponding
-        to the real part of the coupling and the hamiltonian corresponding to the imaginary part.
-
-        Returns
-        -------
-        hamiltonian_base : np.ndarray
-            The `(*l,n,n)` shape base hamiltonian of the system containing
-            all elements that do not depend on time, where `n` is the basis size
-            of the sensor.
-
-        dipole_matrix_real : np.ndarray
-            The `(M,n,n)` shape array of matrices representing the real
-            time-dependent portion of the hamiltonian. For `0 <= i <= M`,
-            the ith value along the first axis is the portion of the matrix which
-            will be multiplied by the output of the ith `time_dependence` function.
-
-        dipole_matrix_imag: nd.ndarray
-            The `(M,n,n)` shape array of matrices representing the imaginary
-            time-dependent portion of the hamiltonian. For `0 <= i <= M`,
-            the ith value along the first axis is the portion of the matrix which
-            will be multiplied by the output of the ith `time_dependence` function.
-
-        Examples
-        --------
-        >>> s = rq.Sensor(2)
-        >>> step = lambda t: 0. if t<1 else 1.
-        >>> s.add_coupling(states=(0,1), detuning=1, rabi_frequency=1, time_dependence=step)
-        >>> H_base, H_time_real, H_time_imaginary = s.get_time_hamiltonians()
-        >>> print(H_base)
-        >>> print(H_time_real)
-        >>> print(H_time_imaginary)
-        [[0.+0.j 0.+0.j]
-        [0.+0.j 1.+0.j]]
-        [array([[0. +0.j, 0.5+0.j],
-            [0.5+0.j, 0. +0.j]])]
-        [array([[0.+0.j , 0.+0.5j],
-            [0.-0.5j, 0.+0.j ]])]
-
-        """
-        hamiltonian_base = self.get_hamiltonian()
-        dipole_matrices = self.get_time_couplings()
-
-        return hamiltonian_base, *dipole_matrices
-
-
-    def get_time_couplings(self) -> Tuple[np.ndarray, np.ndarray]:
-        """
-        Returns the list of matrices of all couplings in the system defined with
-        a `time_dependence` key.
-
-        The ouput will be two lists of matricies representing which terms of the hamiltonian
-        are dependent on each time-dependent coupling.
-        The lists will be of length M and shape `(*l_time, n, n)`,
-        where M is the number of time-dependent couplings, `l_time` is time-dependent stack shape
-        (possibly all ones), and `n` is the basis size. Each matrix will have terms equal to the rabi frequency
-        (or half the rabi frequency under RWA) in positions that correspond to the associated transition.
-        For example, in the case where there is a `time_dependence` function defined for the `(2,3)` transition
-        with a rabi frequency of 1, the associated time coupling matrix will be all zeros,
-        with a 1 in the `(2,3)` and `(3,2)` positions.
-
-        Typically, this function is called internally and multiplied by the output
-        of the :meth:`~.Sensor.get_time_dependence` function.
-
-        Returns
-        -------
-        list of numpy.ndarray
-            The list of M `(*l,n,n)` matrices representing the
-            real-valued time-dependent portion of the hamiltonian. For `0 <= i <= M`,
-            the ith value along the first axis is the portion of the matrix which
-            will be multiplied by the output of the ith `time_dependence` function.
-            
-        list of numpy.ndarray
-            The list of M `(*l,n,n)` matrices representing the
-            imaginary-valued time-dependent portion of the hamiltonian. For `0 <= i <= M`,
-            the ith value along the first axis is the portion of the matrix which
-            will be multiplied by the output of the ith `time_dependence` function.
-
-        Examples
-        --------
-        >>> s = rq.Sensor(3)
-        >>> step = lambda t: 0 if t<1 else 1
-        >>> wave = lambda t: np.sin(2000*np.pi*t)
-        >>> f1 = {"states": (0,1), "transition_frequency":10, "rabi_frequency": 1, "time_dependence":wave}
-        >>> f2 = {"states": (1,2), "transition_frequency":10, "rabi_frequency": 2, "time_dependence":step}
-        >>> s.add_couplings(f1, f2)
-        >>> time_hams, time_hams_i = s.get_time_couplings()
-        >>> for H in time_hams:
-        ...     print(H)
-        [[0.+0.j 1.+0.j 0.+0.j]
-        [1.+0.j 0.+0.j 0.+0.j]
-        [0.+0.j 0.+0.j 0.+0.j]]
-        [[0.+0.j 0.+0.j 0.+0.j]
-        [0.+0.j 0.+0.j 2.+0.j]
-        [0.+0.j 2.+0.j 0.+0.j]]
-            
-        To handle stacking across the steady-state and time hamiltonians, the dimensions are 
-        matched in a way that broadcasting works in a numpy-friendly way
-        
-        >>> s = rq.Sensor(3)
-        >>> rabi = np.linspace(-1,1,11)
-        >>> step = lambda t: 0 if t<1 else 1
-        >>> blue = {"states":(0,1), "rabi_frequency":rabi, "detuning":1}
-        >>> red = {"states":(1,2), "rabi_frequency":rabi, "detuning":0, 'time_dependence': step}
-        >>> s.add_couplings(red, blue)
-        >>> time_hams, time_hams_i = s.get_time_couplings()
-        >>> print(s.get_hamiltonian().shape)
-        >>> print(time_hams[0].shape)
-        >>> print(time_hams_i[0].shape)
-        (1, 11, 3, 3)
-        (11, 1, 3, 3)
-        (11, 1, 3, 3)
-
-        """  # noqa
-        #save to re-add later
-        base_couplings = self.couplings.copy()
-
-        stack_shape = self._stack_shape(collapse=False, time_dependence='time')
-
-        for states, param, arr in self.variable_parameters(apply_mesh=True):
-            self.couplings.edges[states][param] = arr
-
-        hamiltonian_shape = (*stack_shape, self.basis_size, self.basis_size)
-
-        matrix_list = []
-        matrix_list_i = []
-
-        #loop over time-dependent couplings
-        for states, f in self.couplings_with("time_dependence").items():
-            
-            if 'rabi_frequency' not in f:
-                continue
-            
-            time_hamiltonian = np.zeros(hamiltonian_shape, dtype='complex')
-            time_hamiltonian_i = np.zeros(hamiltonian_shape, dtype='complex')
-
-            idx = (...,*states)
-            conj_idx = (...,*states[::-1])
-            
-            #ignores numpy casting to real warning that we already account for
-            with warnings.catch_warnings():
-                warnings.simplefilter("ignore")
-                if 'transition_frequency' in f:
-                    time_hamiltonian[idx] = f['rabi_frequency']
-                    time_hamiltonian[conj_idx] = np.conj(f["rabi_frequency"])
-                    time_hamiltonian_i[idx] = 1j*f["rabi_frequency"]
-                    time_hamiltonian_i[conj_idx] = np.conj(f["rabi_frequency"]*1j)
-                
-                #factor of 1/2 for rwa
-                else:
-                    time_hamiltonian[idx] = f['rabi_frequency']/2
-                    time_hamiltonian[conj_idx] = np.conj(f["rabi_frequency"])/2
-                    time_hamiltonian_i[idx] = 1j*f["rabi_frequency"]/2
-                    time_hamiltonian_i[conj_idx] = np.conj(f["rabi_frequency"]*1j)/2
-
-            matrix_list.append(time_hamiltonian)
-            matrix_list_i.append(time_hamiltonian_i)
-            
-        self.couplings = base_couplings
-
-        return matrix_list, matrix_list_i
-
-
-    def get_time_dependence(self) -> List[Callable[[float], float]]:
-        """
-        Function which returns a list of the `time_dependence` functions.
-        
-        The list is returned with in the order that matches with the time hamiltonians from 
-        :meth:`~.Sensor.get_time_couplings` such that the ith element of of the return of this
-        functions corresponds with the ith Hamiltonian terms returned by that function. 
-
-        Returns
-        -------
-        list
-            List of scalar functions, representing all couplings specified with a `time_dependence`.
-            
-
-        Examples:
-            >>> s = rq.Sensor(3)
-            >>> step = lambda t: 0 if t<1 else 1
-            >>> wave = lambda t: np.sin(2000*np.pi*t)
-            >>> f1 = {"states": (0,1), "transition_frequency":10, "rabi_frequency": 1, "time_dependence":wave}
-            >>> f2 = {"states": (1,2), "transition_frequency":10, "rabi_frequency": 2, "time_dependence":step}
-            >>> s.add_couplings(f1, f2)
-            >>> print(s.get_time_dependence())
-            [<function <lambda> at 0x7fb310edd9d0>, <function <lambda> at 0x7fb37c0c81f0>]
-
-        """  # noqa
-        time_dependence = []
-        for (i,j),f in self.couplings_with("time_dependence").items():
-            time_dependence.append(f['time_dependence'])
-        return time_dependence
-
-
-    def get_hamiltonian_diagonal(self, values: dict, no_stack: bool=False) -> np.ndarray:
-        """
-        Apply addition and subtraction logic corresponding to the direction of the couplings.
-
-        For a given state `n`, the path from ground will be traced to `n`. For each edge along this
-        path, values will be added where the path direction and coupling direction match,
-        and subtracting values where they do not.
-        The sum of all such values along the path is the `n` th term in the output array. 
-
-        Primarily for internal functions which help generate hamiltonians. Most commonly used
-        to calculate total detunings for ranges of couplings under the RWA
-
-        Parameters
-        ----------
-        values : dict
-            Key-value pairs where the keys correspond to transitions
-            (agnostic to ordering of states) and values corresponding to the values
-            to which the logic will be applied.
-        no_stack : bool, optional
-            Whether to ignore variable parameters in the system and
-            use only basic math operations rather than reshape the output. Typically
-            only `True` for calculating doppler shifts.
-
-        Returns
-        -------
-        numpy.ndarray
-            The digonal of the hamiltonian of the system of shape `(*l,n)`,
-            where `l` is the shape of the hamiltonian stack for the sensor.
-
-        """
-        coherent_edges = [
-            states for states in self.couplings.edges
-            if "rabi_frequency" in self.couplings.edges[states]
-            ]
-
-        coherent_graph = self.couplings.edge_subgraph(coherent_edges)
-
-        if no_stack:
-            diag = np.zeros(self.basis_size)
-        else:
-            diag = np.zeros((*self._stack_shape(collapse=False, time_dependence="steady"),
-                             self.basis_size),
-                             dtype=np.complex128)
-
-        connected_levels = nx.weakly_connected_components(coherent_graph)
-        subgraphs = [coherent_graph.subgraph(ls) for ls in connected_levels]
-
-        for g in subgraphs:
-
-            # min sets lowest state in graph as "ground"
-            paths = nx.shortest_path(nx.to_undirected(g), source=min(g.nodes))
-            paths_np = {k:np.array(v) for k,v in paths.items()}  # convert to numpy arrays
-
-            for i, path in paths_np.items():
-
-                term = 0
-
-                for j in range(1, len(path)):
-
-                    # get the jth couplings along the path and initialize the sign as positive
-                    field = tuple(np.copy(path[j-1:j+1]))
-                    sign = 1
-
-                    if field not in self.couplings.edges:
-                        # switch the sign if the arrow points in the opposite direction
-                        # This corresponds to moving to a lower energy state
-                        # Since it is getting an existing edge from the undirected graph,
-                        # we are guaranteed either field or field[::-1] being on the graph
-                        field = field[::-1]
-                        sign = -1
-
-                    # sum to the cumulative term along the path from ground
-                    term = term + values.get(field,0)*sign
-
-                diag[..., i] = term
-
-        return diag
-
-
-    def get_transition_frequencies(self) -> np.ndarray:
-        """
-        Gets an array of the diagonal elements of the Hamiltonian from the field detunings.
-
-        Wraps the :meth:`~.Sensor.get_hamiltonian_diagonal` function using both
-        transition frequencies and detunings. Primarily for internal use. 
-
-        Returns
-        -------
-        numpy.ndarray
-            N-D array of the hamiltonian diagonal. For an n-level system with stack shape `*l`,
-            will be shape `(*l, n)`
-            
-        """
-        detuning_dict = self.get_value_dictionary("detuning")
-        transition_frequency_dict = self.get_value_dictionary("transition_frequency")
-        freq_dict = {**detuning_dict, **transition_frequency_dict}
-        return self.get_hamiltonian_diagonal(freq_dict)
-
-
-    def get_value_dictionary(self, key: str) -> dict:
-        """
-        Get subset of dictionary coupling parameters.
-
-        Return a dictionary of key value pairs where the keys are couplings added
-        to the system and the values are the value of the parameter specified by key.
-        Produces an output that can be passed directly to :meth:`~.get_hamiltonian_diagonal`.
-        Only couplings whose parameter dictionaries contain "key" will be in the
-        returned dictionary.
-
-        Parameters
-        ----------
-        key : str
-            String value of the parameter name to build the dictionary.
-            For example, `get_value_dictionary("detuning")` will return a dictionary with keys
-            corresponding to transitions and values corresponding to detuning
-            for each transition which has a detuning.
-
-        Returns
-        -------
-        dict
-            Coupling dictionary with couplings as keys and corresponding
-            values set by input key.
-
-        Examples
-        --------
-        >>> s = rq.Sensor(4)
-        >>> f1 = {"states": (0,1), "detuning": 2, "rabi_frequency": 1}
-        >>> f2 = {"states": (1,2), "detuning": 3, "rabi_frequency": 2}
-        >>> f3 = {"states": (2,3), "rabi_frequency": 3, "transition_frequency": 3}
-        >>> s.add_couplings(f1, f2, f3)
-        >>> print(s.get_value_dictionary("detuning"))
-        {(0,1): 2, (1,2): 3}
-
-        """
-        couplings_with_key = self.couplings_with(key)
-        return {states:params[key] for states, params in couplings_with_key.items()}
-
-
-    def set_gamma_matrix(self, gamma_matrix: np.ndarray) -> None:
-        """
-        Set the decoherence matrix for the system. 
-        
-        Works by first removing all existing decoherent data from graph edges, then individually
-        adding all nonzero terms of a provided gamma matrix to the corresponding graph edges.
-        Can be used to set all decoherence attributes to edges simultaneously,
-        but :meth:`~.add_decoherence` is preferred.
-        
-        Unlike :meth:`~.add_decoherence`, does not support scanning multiple decoherence values,
-        rather should be used to set the decoherences of the system to individual static values.
-
-        Parameters
-        ----------
-        gamma_matrix : numpy.ndarray
-            Array of shape `(basis_size, basis_size)`.
-            Element `(i,j)` describes the decoherence rate, in Mrad/s,
-            from state `i` to state `j`.
-
-        Raises
-        ------
-        TypeError
-            If `gamma_matrix` is not a numpy array.
-        ValueError
-            If `gamma_matrix` is not a square matrix of the appropriate size
-        ValueError
-            If the shape of `gamma_matrix` is not compatible with `self.basis_size`.
-
-        Examples
-        --------
-        >>> s = rq.Sensor(2)
-        >>> f1 = {"states": (0,1), "transition_frequency":10, "rabi_frequency": 1}
-        >>> s.add_couplings(f1)
-        >>> gamma = np.array([[.1,0],[.1,0]])
-        >>> s.set_gamma_matrix(gamma)
-        >>> print(s.decoherence_matrix())
-        [[0.1 0. ]
-        [0.1 0. ]]
-
-        """
-        if not isinstance(gamma_matrix, np.ndarray):
-            raise TypeError(f'gamma_matrix must be a numpy array, not type {type(gamma_matrix)}')
-
-        if gamma_matrix.shape != (self.basis_size,self.basis_size):
-            raise ValueError((f'gamma_matrix has shape {gamma_matrix.shape}, '
-                              f'must be {(self.basis_size,self.basis_size)}'))
-
-        for states, gamma in np.ndenumerate(gamma_matrix):
-            
-            #remove existing decoherence data
-            if self.couplings.has_edge(*states):
-                
-                remove_keys = []
-                for key in self.couplings.edges[states].keys():
-                    if key.startswith("gamma_"):
-                        remove_keys.append(key)
-                        
-                for key in remove_keys:
-                    del self.couplings.edges[states][key]
-            
-            #add new decoherence
-            if gamma != 0: 
-                #exclude gamma==0; its implicitly put there in decoherence_matrix()
-                self.add_decoherence(states, gamma)
-
-
-    def get_doppler_shifts(self) -> np.ndarray:
-        """
-        Returns the Hamiltonian with only detunings set to the kvector values for
-        each spatial dimension.
-
-        Determining if a float should be treated as zero is done using :obj:`numpy.isclose`,
-        which has default absolute tolerance of `1e-08`.
-
-        Returns
-        -------
-        numpy.ndarray
-            Array of shape (used_spatial_dim,n,n), Hamiltonians
-            with only the doppler shifts present along each non-zero spatial dimension
-            specified by the fields' "kvec" parameter.
-
-        """
-        spatial_dim = 3
-
-        kvecs = self.get_value_dictionary('kvec')
-        # collect shifts for each spatial dimension that is non-zero
-        s_kvecs = [{k:v[i] for k,v in kvecs.items() if ~np.isclose(v[i],0)}
-                   for i in range(spatial_dim)]
-        if not any(s_kvecs):
-            raise ValueError(('You must specify at least one non-zero '
-                              'kvector to do doppler averaging.'))
-        # get hamiltonian diagonal for each non-zero spatial dimension
-        frequencies = np.array([self.get_hamiltonian_diagonal(s_kvec, no_stack=True)
-                                for s_kvec in s_kvecs if s_kvec])
-        # expand to full hamiltonians
-        doppler_hamiltonians = np.eye(self.basis_size) * frequencies[:,np.newaxis,:]
-
-        assert self.spatial_dim() == doppler_hamiltonians.shape[0], \
-            'Spatial dimension inconsistency'
-
-        return doppler_hamiltonians
-
-
-    def couplings_with(self, *keys: str,
-                       method: Literal['all','any', 'not any'] = "all"
-                       ) -> Dict[States, CouplingDict]:
-        """
-        Returns a version of self.couplings with only the keys specified.
-        
-        Can be specified with a several criteria, including all, none, or any of the keys
-        specified.
-
-        Parameters
-        ----------
-        keys(tuple of str): tuple of strings which should be one the valid
-            parameter names for a state. See :meth:`~.add_coupling` for which
-            names are valid for a Sensor object.
-        method : {'all','any', 'not any'} 
-            Method to see if a given field matches the keys
-            given. Choosing "all" will return couplings
-            which have keys matching all of the values provided in the keys
-            argument, while coosing "any", will return all couplings with keys
-            matching at least one of the values specified by keys. For example,
-            `sensor.couplings_with("rabi_frequency")` returns a dictionary of
-            all couplings for which a rabi_frequency was specified.
-            `sensor.couplings_with("rabi_frequency", "detuning", method="all")`
-            returns all couplings for which both rabi_frequency and detuning
-            are specified.
-            'sensor.couplings_with("rabi_frequency", "detuning", method="any")`
-            returns all couplings for which either rabi_frequency or detuning
-            are specified.
-            Defaults to "all".
-
-        Returns
-        -------
-        dict
-            A copy of the `sensor.couplings` dictionary with only couplings containing
-            the specified parameter keys.
-
-        Examples
-        --------
-        Can be used, for example, to return couplings in the roating wave approximation.
-        
-        >>> s = rq.Sensor(3)
-        >>> sinusoid = lambda t: 0 if t<1 else sin(100*t)
-        >>> f2 = {"states": (0,1), "detuning": 1, "rabi_frequency":2}
-        >>> f1 = {"states": (1,2), "transition_frequency":100, "rabi_frequency":1, "time_dependence": sinusoid}
-        >>> s.add_couplings(f1, f2)
-        >>> gamma = np.array([[.2,0,0],
-        ...                  [.1,0,0],
-        ...                  [0.05,0,0]])
-        >>> s.set_gamma_matrix(gamma)
-        >>> print(s.couplings_with("detuning"))
-        {(0, 1): {'rabi_frequency': 2, 'detuning': 1, 'phase': 0, 'kvec': (0, 0, 0), 'no_rwa_warning': False, 'label': '(0,1)'}}
-        """  # noqa
-        def notAll(x):
-            return not all(x)
-
-        def notAny(x):
-            return not any(x)
-
-        methods = {"any":any, "all":all, "not any": notAny, "not all": notAll}
-
-        return {s:p
-                for s,p in self.couplings.edges.items()
-                if methods[method]([k in p for k in keys])
-                }
-
-
-    def get_couplings(self) -> Dict[States, CouplingDict]:
-        """
-        Returns the couplings of the system as a dictionary
-        
-        Deprecating in favor of calling the couplings.edges attribute directly. 
-
-        Returns
-        -------
-        dict
-            A dictionary of key-value pairs with the keys corresponding to levels of
-            transition, and the values being dictionaries of coupling attributes.
-
-        """
-        return {s:p for s,p in self.couplings.edges.items()}
-
-
-    def spatial_dim(self) -> int:
-        """
-        Returns the number of spatial dimensions doppler averaging will occur over.
-
-        Determining if a float should be treated as zero is done using :obj:`numpy.isclose`,
-        which has default absolute tolerance of `1e-08`.
-
-        Returns
-        -------
-        int
-            Number of dimensions, between 0 and 3,
-            where 0 means no doppler averaging kvectors have been specified
-            or are too small to be calculates. 
-            
-        Examples
-        --------
-        No spatial dimesions specified
-        
-        >>> s = rq.Sensor(2)
-        >>> s.add_coupling((0,1), detuning = 1, rabi_freqency=1)
-        >>> print(s.spatial_dim())
-        0
-        
-        One spatial dimension specified
-        
-        >>> s = rq.Sensor(2)
-        >>> s.add_coupling((0,1), detuning = 1, rabi_freqency=1, kvec=(0,0,1))
-        >>> print(s.spatial_dim())
-        1
-        
-        Multiple spatial dimensions can exist in a single coupling or 
-        across multiple couplings
-        
-        >>> s = rq.Sensor(2)
-        >>> s.add_coupling((0,1), detuning = 1, rabi_freqency=1, kvec=(1,0,1))
-        >>> print(s.spatial_dim())
-        2
-        
-        >>> s = rq.Sensor(3)
-        >>> s.add_coupling((0,1), detuning = 1, rabi_freqency=1, kvec=(1,0,1))
-        >>> s.add_coupling((1,2), detuning = 2, rabi_freqency=2, kvec=(0,1,0))
-        >>> print(s.spatial_dim())
-        3
-        """
-        k_vector_dim = np.zeros(3,dtype=bool)
-
-        for key, field in self.couplings.edges.items():
-            if 'kvec' in field:
-                k_vector_dim = k_vector_dim | ~np.isclose(field['kvec'],0)
-
-        return np.sum(k_vector_dim)
-
-
-    def _states_valid(self, states: States) -> States:
-        """
-        Confirms that the provided states are in a valid format.
-        
-        Typically used internally to validate states added. If provided as 
-        a form other than a tuple, first casts to a tuple for consistent
-        indexing.
-        
-        Checks that `states` contains 2 elements, can be interpreted as a tuple,
-        and that both states lie inside the basis.
-
-        Parameters
-        ----------
-        states : iterable
-            iterable of to validate. Should be a pair of integers that can
-            be cast to a tuple.
-
-        Returns
-        -------
-        tuple
-            Length 2 tuple of validated state labels.
-
-        Raises
-        ------
-        ValueError
-            If `states` has more than two elements.
-        TypeError
-            If `states` cannot be converted to a tuple.
-        ValueError
-            If either state in `states` is outside the basis.
-        """
-        try:
-            tpl = tuple(states)
-        except TypeError:
-            raise ValueError(
-                f'states argument of type {type(states)} cannot be interpreted as a tuple')
-        if len(tpl) != 2:
-            raise ValueError(
-                f'A field must couple exactly 2 states, but {len(tpl)} are specified in {states}')
-        for i in tpl:
-            if not isinstance(i, int):
-                raise TypeError('State specifications must be an integer')
-            if i >= self.basis_size:
-                raise ValueError((f'State specification {i} is outside '
-                                  f'the basis size {self.basis_size:d}'))
-
-        return tpl
-
-
-    def _stack_shape(self, collapse=True, time_dependence="all") -> Tuple[int, ...]:
-        """
-        Internal function to get the shape of the tuple preceding the two hamiltonian
-        axes in :meth:`~.get_hamiltonian()`
-
-        """
-        # generate the uncollapsed stack
-        stack_shape = []
-
-        #case where we ignore time dependence in the stack shape
-        if time_dependence == 'all':
-            for _, _, arr in self.variable_parameters():
-                stack_shape.append(len(np.squeeze(arr)))
-
-        #case where we only want time-dependant stack shape
-        elif time_dependence == "time":
-            time_couplings = self.couplings_with("time_dependence")
-            for states, param, arr in self.variable_parameters():
-                if states in time_couplings and param == "rabi_frequency":
-                    stack_shape.append(len(np.squeeze(arr)))
-                else:
-                    stack_shape.append(1)
-
-        #case where we only want non-time-dependant stack shape
-        elif time_dependence == "steady":
-            time_couplings = self.couplings_with("time_dependence")
-            for states, param, arr in self.variable_parameters():
-                if states not in time_couplings or param != "rabi_frequency":
-                    stack_shape.append(len(np.squeeze(arr)))
-                else:
-                    stack_shape.append(1)
-        
-        else:
-            raise ValueError("time_dependence must be one of \"time\", \"steady\", or \"all\"")
-
-
-        # if collapsing, figure out the einsum logic
-        if collapse and len(self._zipped_parameters) > 0:
-            # list logic direct lifted from Sensor.collapse_dims()
-            axis_labels = self.axis_labels(collapse=False)
-            
-            paired_axes = []
-            for couplings in self._zipped_parameters:
-                paired_axes.append([axis_labels.index(c) for c in couplings])
-                
-            col_str = _get_collapse_str(len(axis_labels), *paired_axes)
-            
-            # this logic adapted from
-            # https://stackoverflow.com/questions/58380445/output-shape-of-numpy-einsum
-            insubs, outsubs = col_str.replace('.','').split('->')
-            insubs_array = np.array(list(insubs))
-            outshape = []
-            for o in outsubs:
-                indices, = np.where(insubs_array == o)
-                outshape.append(max([stack_shape[idx] for idx in indices]))
-                
-            stack_shape = tuple(outshape)
-
-        return stack_shape
-
-
-    def basis(self) -> np.ndarray:
-        """
-        Generate basis labels of density matrix components. 
-        
-        The basis corresponds to the elements in the solution.
-        This is not the complex basis of the sensor class, but rather the real basis
-        of a solution after calling one of `rydiqule`'s solvers. This means that the
-        ground state population has been removed and it has been transformed to the real basis.
-
-        Returns
-        -------
-        numpy.ndarray
-            Array of string labels corresponding to the solving basis.
-            Is a 1-D array of length `n**2-1`.
-
-        Examples
-        --------
-        >>> s = rq.Sensor(3)
-        >>> print(s.basis())
-        ['01_real' '02_real' '01_imag' '11_real' '12_real' '02_imag' '12_imag'
-        '22_real']
-
-        """
-        basis = [f'{j:d}{i:d}_imag' if i > j else f'{i:d}{j:d}_real'
-                 for i in range(self.basis_size)
-                 for j in range(self.basis_size)][1:]  # indexing removes ground state label
-        return np.array(basis)
-
-
-    def _remove_edge_data(self, states: States, kind: str):
-        """
-        Helper function to remove all data that was added with a :meth:`~.Sensor.add_coupling`
-        call or :meth:`~.Sensor.add_decoherence` call.
-        Needed to ensure that two nodes do not have coherent couplings pointing both ways
-        and to invalidate existing zip parameter couplings.
-
-        Parameters
-        ----------
-        states : tuple
-            Edge from which to remove data.
-        kind : str
-            What type of data to remove. Valid options are `coherent` coherent couplings
-            or the incoherent key to be cleared (must start with `gamma`).
-
-        Raises
-        ------
-        ValueError
-            If `kind` is not `'coherent'` and doesn't begin with `'gamma'`
-        """
-
-        if states not in self.couplings.edges:
-            return
-
-        if kind != 'coherent' and not kind.startswith('gamma'):
-            msg = ("If clearing incoherent data,"
-                   " must provide key to clear that starts with `gamma`, not {}")
-            raise ValueError(msg.format(kind))
-
-        #get rid of zipped couplings containing
-        label = self.couplings.edges[states]["label"]
-        zipped_idxs = []
-        for idx, zip_strs in enumerate(self._zipped_parameters):
-            zip_labels = [l.split("_",1)[0] for l in zip_strs]
-            if label in zip_labels:
-                zipped_idxs.append(idx)
-
-        for idx in zipped_idxs[::-1]:
-            del self._zipped_parameters[idx]
-        
-        # delete undesired keys from the edge
-        for key in list(self.couplings.edges[states]):  # prevent generator
-            if key == 'label':
-                pass
-            elif kind == 'coherent' and not key.startswith('gamma'):
-                del self.couplings.edges[states][key]
-            elif kind == key:
-                del self.couplings.edges[states][key]
-                
-        # delete edge outright if it only has a label
-        if not sum(k != 'label' for k in self.couplings.edges[states].keys()):
-            self.couplings.remove_edge(*states)
-
-
-    def _coupling_with_label(self, label: str) -> dict:
-        """
-        Helper function to return the pair of states corresponding to a particular label string.
-        For internal use.
-        """
-        label_map = {key:(state1, state2)
-                     for state1, state2, key in self.couplings.edges(data="label")}
-        if label in label_map.keys():
-            return label_map[label]
-        else:
-            raise ValueError(f"No coupling with label {label}")
+"""
+Sensor objects that control solvers.
+"""
+
+import numpy as np
+import networkx as nx  # type: ignore
+import warnings
+
+from .sensor_utils import _get_collapse_str, _combine_parameter_labels
+
+from typing import List, Tuple, Dict, Literal, Callable, Optional, Union
+
+ScannableParameter = Union[float, List[float], np.ndarray]
+
+CouplingDict = Dict
+States = Tuple[int, ...]
+
+#this includes only parameters for coherent couplings. "gamma" parameters are handled separately in the relevant places.
+BASE_SCANNABLE_KEYS = ["detuning", 
+                       "rabi_frequency", 
+                       "phase", 
+                       "transition_frequency"]
+"""Reference list of all coherent coupling keys that support rydiqules stacking convention.
+Note that all decoherence keys (keys beginning with `gamma_`) are supported, but handled separately."""
+
+BASE_EDGE_KEYS = ["states",
+                   "detuning", 
+                   "rabi_frequency",
+                   "transition_frequency",
+                   "phase",
+                   "kvec",
+                   "time_dependence",
+                   "label",
+                   "dipole_moment"]
+"""Reference list of all keys that can be specified with values in a coherenct coupling.
+Subclasses which inherit the :class:`~.Sensor` class should override the `valid_parameters` attribute,
+NOT this list. The `valid_parameters` attribute is initialized as a copy of `BASE_EDGE_KEYS`."""
+
+class Sensor():
+    """
+    Class that contains minimum information necessary to run the solvers.
+
+    Consider this class the theorist's interface to the solvers.
+    It requires nearly complete, explicit specification of inputs.
+    This allows for very fine control of the solvers,
+    including the ability to solve systems that are not entirely physical.
+    
+    """
+
+    eta: Optional[float] = None
+    """Noise density prefactor, in units of root(Hz).
+    Must be specified when using :class:`Sensor`.
+    Automatically calculated when using :class:`Cell`."""
+
+    kappa: Optional[float] = None
+    """Differential prefactor, in units of (Mrad/s)/m.
+    Must be specified when using :class:`Sensor`.
+    Automatically calculated when using :class:`Cell`."""
+
+    def __init__(self, basis_size: int, *couplings: CouplingDict) -> None:
+        """
+        Initializes the Sensor of the specified basis size.
+
+        Parameters
+        ----
+        basis_size : int 
+            Number of states in the basis.
+        *couplings : tuple(dict) 
+            Couplings dictionaries to pass to :meth:`~.add_couplings` on sensor construction.
+        
+        Raises
+        ------
+        TypeError
+            If `basis_size` is not an integer.
+        
+        """
+        if type(basis_size) != int:
+            raise TypeError("basis_size must be an integer")
+        
+        self.basis_size = basis_size
+
+        self.couplings = nx.DiGraph()
+        self.couplings.add_nodes_from(range(self.basis_size))
+
+        if len(couplings) > 0:
+            self.add_couplings(*couplings)
+
+        self._zipped_parameters: List[List[str]] = []
+        self.valid_parameters = BASE_EDGE_KEYS.copy()
+
+
+    def add_coupling(
+            self, states: States, rabi_frequency: Optional[ScannableParameter] = None,
+            detuning: Optional[ScannableParameter] = None,
+            transition_frequency: Optional[float] = None,
+            phase: Optional[ScannableParameter] = 0,
+            kvec: Tuple[float,float,float] = (0,0,0),
+            time_dependence: Optional[Callable[[float],float]] = None,
+            label: Optional[str] = None,
+            **extra_kwargs) -> None:
+        """
+        Adds a single coupling of states to the system.
+
+        One or more of these paramters can be a list or array-like of values to represent
+        a laser that can take on a set of discrete values during a field scan.
+        Designed to be a user-facing wrapper for :meth:`~._add_coupling` with arguments
+        for states and coupling parameters.
+
+        Parameters
+        ----------
+        states : tuple of ints of length 2
+            The pair of states of the sensor which the state couples
+            Must be a tuple of intergers of length 2, and the integers must
+            be unique indicies within the basis.
+        rabi_frequency : float or complex, or list-like of float or complex
+            The rabi frequency of the field being added. Defined in units of Mrad/s. List-like
+            values will invoke Rydiqule's stacking convention when relevant quantities are calculated.
+        detuning : float or list-like of floats or  None, optional 
+            The frequency difference between the transition frequency and the field frequency in 
+            units of Mrad/s. List-like values will invoke Rydiqule's stacking convention when relevant 
+            quantities are calculated. If specified, the coupling is treated with the rotating-wave 
+            approximation rather than in the lab frame, and `transition_frequency` is ignored if present.
+        transition_frequency : float or list-like of floats or None, optional 
+            The transition frequency between a particular pair of states. List-like
+            values will invoke Rydiqule's stacking convention when relevant quantities are calculated. 
+            Only used directly in calculations if `detuning` is `None`, ignored otherwise. 
+            Note that on its own, it only defines the spacing between two energy levels and not the
+            field itsself. To define a field, the `time_dependence` argument must be specified, or else 
+            the off-diagonal terms to drive transitions will not be generated in the Hamiltonian matrix.
+        phase : float, optional
+            The relative phase of the field in radians. Defaults to zero.
+        kvec : iterable, optional 
+            A three-element iterable that defines the atomic doppler shift on a particular coupling
+            field. It should have magntiude equal to the doppler shift (in the units of Mrad/s) of a
+            n atom moving at the Maxwell-Boltzmann distribution most probable speed, `vP=np.sqrt(2*kB*T/m)`. 
+            I.E. `np.linalg.norm(kvec)=2*np.pi/lambda*vP`. If equal to `(0,0,0)`, solvers will ignore 
+            doppler shifts on this field.  Defaults to `(0,0,0)`.
+        time_dependence : scalar function, optional
+            A scalar function specifying a time-dependent field. The time dependence function is defined 
+            as a python funtion that returns a unitless value as a function of time (in microseconds) 
+            that is multiplied by the `rabi_frequency` parameter to get a  field strength scaled to units 
+            of Mrad/s.
+        label : str or None, optional
+            Name of the coupling. This does not change any calculations, but can be used 
+            to help track individual couplings, and will be reflected in the output of 
+            :meth:`~.Sensor.axis_labels`, and to specify zipping for :meth:`~.Sensor.zip_couplings`. 
+            If `None`, the label is generated as the value of `states` cast to a string with 
+            whitespace removed. Defaults to `None`.
+
+        Raises
+        ------
+        ValueError
+            If `states` cannot be interpreted as a tuple.
+        ValueError
+            If `states` does not have a length of 2.
+        ValueError
+            If the state numbers specified by `states` are beyond the basis size.
+            For example, calling this function with `states=(3,4)`
+            will raise this error if the basis size is equal to 3.
+        ValueError
+            If both `rabi_frequency` and `dipole_moment` are specified or if
+            neither are specified.
+        ValueError
+            If both detuning and transition_frequency are specified or if
+            neither are specified.
+
+        Examples
+        --------
+        >>> s = rq.Sensor(2)
+        >>> s.add_coupling(states=(0,1), detuning=1, rabi_frequency=2)
+
+        >>> s = rq.Sensor(2)
+        >>> s.add_coupling(states=(0,1), detuning=np.linspace(-10, 10, 101), rabi_frequency=2, label="laser")
+
+        >>> s = rq.Sensor(2)
+        >>> step = lambda t: 1 if t>=1 else 0
+        >>> s.add_coupling(states=(0,1), transition_frequency=1000, rabi_frequency=2, time_dependence=step)
+
+        >>> s = rq.Sensor(2)
+        >>> kp = 250*np.array([1,0,0])
+        >>> s.add_coupling(states=(0,1), detuning=1, rabi_frequency=2, kvec=kp)
+
+        """ 
+
+        if states[0] == states[1]:
+            raise ValueError('Coherent coupling must couple different states.')
+
+        suppress_rwa = extra_kwargs.pop("suppress_rwa_warn", False)
+
+        field_params = {k:v for k,v in locals().items()
+                        if k in self.valid_parameters
+                        and v is not None}
+        
+        if not (detuning is not None) ^ (transition_frequency is not None):
+            msg = """Please specify \'detuning\' for a field under the RWA or
+                \'transition_frequency\' for a coupling without the approximation,
+                but not both."""
+            raise ValueError(msg)
+
+        if detuning is None and np.abs(transition_frequency) > 5000 and not suppress_rwa:  # type: ignore[operator]
+            msg = "Not using the rotating wave approximation for large transition frequencies "\
+                "can result in prohibitively long computation times. Specify detuning to use the"\
+                " rotating wave approximation or set the \"suppress_rwa_warn\" to \"True\" to"\
+                " suppress this warning."
+
+            with warnings.catch_warnings():
+                warnings.simplefilter("always")
+                warnings.warn(msg, stacklevel=2)
+
+        self._add_coupling(**field_params, **extra_kwargs)
+
+
+    def add_couplings(self, *couplings: CouplingDict,
+                        **extra_kwargs) -> None:
+        """
+        Add any number of couplings between pairs of states.
+        
+        Acts as an alternative to calling :meth:`~.Sensor.add_coupling` individually for each pair of states.
+        Can be used interchangably up to preference, and all of keyword :meth:`~.Sensor.add_coupling` are supported dictionary
+        keys for dictionaries passed to this function.
+
+        Parameters
+        ----------
+        couplings : tuple of dicts
+            Any number of dictionaries, each specifying the parameters of a single field 
+            coupling 2 states. For more details on the keys of each dictionry see the arguments 
+            for :meth:`~.Sensor.add_coupling`. Equivalent to passing each dictiories keys and 
+            values to :meth:`~.Sensor.add_coupling` individually.
+        **extra_kwargs : dict
+            Additional keyword-only arguments to pass to the relevant `add_coupling` method.
+            The same arguments will be passed to each call of :meth:`~.Sensor.add_coupling`.
+            Often used for warning suppression.
+
+        Raises
+        ------
+        ValueError
+            If the `states` parameter is missing.
+
+        Examples
+        --------
+        >>> s = rq.Sensor(3)
+        >>> blue = {"states":(0,1), "rabi_frequency":1, "detuning":2}
+        >>> red = {"states":(1,2), "rabi_frequency":3, "detuning":4}
+        >>> s.add_couplings(blue, red)
+        >>> print(s.couplings.edges(data=True))
+        [(0, 1, {'rabi_frequency': 1, 'detuning': 2, 'phase': 0, 'kvec': (0, 0, 0)}), (1, 2, {'rabi_frequency': 3, 'detuning': 4, 'phase': 0, 'kvec': (0, 0, 0)})]
+
+        """ # noqa
+        for c in couplings:
+            c_copy = c.copy()
+            try:
+                states = self._states_valid(c_copy.pop('states'))
+            except KeyError:
+                raise ValueError("\'states\' parameter must be specified for any field")
+
+            self.add_coupling(states=states, **c_copy, **extra_kwargs)
+
+
+    def _add_coupling(self, states: States, **field_params) -> None:
+        """
+        Function for internal use which will ensure the supplied couplings is valid,
+        add the field to self.couplings. 
+        
+        Exists to abstract away some of the internally necessary bookkeeping functionality from
+        user-facing classes. 
+
+        Parameters
+        ----------
+            states : tuple
+                The integer pair of states to be coupled.
+            **field_params : dict
+                The dictionry of couplings parameters. For details
+                on the keys of the dictionry see :meth:`~.Sensor.add_coupling`.
+
+        """
+        states = self._states_valid(states)
+
+        # if label not provided, set to default value of states tuple as a str
+        if field_params.get("label") is None:
+            field_params["label"] = str(states).replace(" ","")
+
+        # remove all coherent data in both directions on the graph
+        # this prevents adding coherent couplings in both directions between 2 nodes
+        self._remove_edge_data(states, 'coherent')
+        self._remove_edge_data(states[::-1], 'coherent')
+
+        self.couplings.add_edge(*states, **field_params)
+
+
+    def zip_parameters(self, *labels: str) -> None:
+        """
+        Define 2 scannable parameters as "zipped" so they are scanned in parallel.
+
+        Zipped parameters will share an axis when quantities relevant to the equations of
+        motion, such as the `gamma_matrix` and `hamiltonian` are generated. Note that calling
+        this function does not affect internal quanties directly, but adds their labels together
+        in the internal `self._zipped_parameters` list, and they are zipped at calculation time
+        for `hamiltonian` and `decoherence_matrix`.
+
+        Parameters
+        ----------
+        labels : str
+            Parameter labels to scan together. Parameter labels are strings of the form 
+            `"<coupling_label>_<parameter_name>"`, such as `"(0,1)_detuning"`. Must be at least 2 labels to zip.
+
+        Raises
+        ------
+        ValueError
+            If fewer than 2 labels are provided.
+        ValueError
+            If any of the 2 labels are the same.
+        ValueError
+            If any elements of `labels` are not labels of couplings in the sensor.
+        ValueError
+            If any of the parameters specified by labels are already zipped.
+        ValueError
+            If any of the parameters specified are not list-like.
+        ValueError
+            If all list-like parameters are not the same length.
+
+        Notes
+        -----
+        .. note::
+            This function should be called last after all Sensor couplings and dephasings
+            have been added. Changing a coupling that has already been zipped removes it from
+            the `self.zipped_parameters` list.
+            
+        .. note::
+            Modifying the `Sensor.zipped_parameters` attribute directly can break some functionality
+            and should be avoided. Use this function or :meth:`~.Sensor.unzip_parameters` instead. 
+
+        Examples
+        --------
+        >>> s = rq.Sensor(3)
+        >>> det = np.linspace(-1,1,11)
+        >>> s.add_coupling(states=(0,1), detuning=det, rabi_frequency=1, label="probe")
+        >>> s.add_coupling(states=(1,2), detuning=det, rabi_frequency=1)
+        >>> s.zip_parameters("probe_detuning", "(1,2)_detuning")
+        >>> print(s._zipped_parameters) #NOT modifying directly
+        [['(1,2)_detuning', 'probe_detuning']]
+
+        """
+        # check for at least 2 labels
+        if len(labels) < 2:
+            raise ValueError(("Please provide at least 2 parameter labels "
+                              f"to zip (only provided {len(labels)})"))
+            
+        #check that all labels are unique
+        if len(labels) != len(set(labels)): #set will be shorter if there are duplicates
+            raise ValueError("parameters cannot be zipped to themselves")
+        
+        #check if any labels are already zipped
+        new_label_array = np.expand_dims(labels, (-1,-2))
+        current_zipped_params = np.expand_dims(self._zipped_parameters, 0)
+        
+        if len(self._zipped_parameters)>0 and np.any(new_label_array==current_zipped_params):  #see if ANY provided label is currently zipped
+
+            for l in labels: #if so, find which label for error reporting
+                if l in current_zipped_params:
+                    raise ValueError(f"Label {l} has already been zipped with another parameter")
+
+        #ensure provided labels are valid for zipping
+        previous_len = 0
+        for l in labels:
+            
+            coupling, param = l.split("_", 1)
+            #make sure the label exists
+            try:
+                states = self._coupling_with_label(coupling)
+            except ValueError:
+                raise ValueError(f"{coupling} is not a label of any coupling in this sensor")
+            
+            #make sure parameter exists and is an array
+            try:
+                param_value = self.couplings.edges[states][param]
+            except KeyError:
+                raise ValueError(f"Coupling {coupling} has no parameter {param}")
+            if not hasattr(param, "__len__"):
+                raise ValueError(f"Parameter {l} is not list-like and cannot be zipped")
+            
+            #make sure parameters are the same length
+            current_len = len(self.couplings.edges[states][param])
+            if previous_len > 0 and current_len != previous_len:
+                raise ValueError(f"Got length {current_len} for parameter \"{l}\", but \"{labels[0]}\" is length {previous_len}")
+            
+            previous_len = current_len
+                        
+        labels = list(labels)
+        labels.sort()
+        self._zipped_parameters.append(labels)
+
+
+    def unzip_parameters(self, *labels: str, **extra_kwargs):
+        
+        """
+        Remove a set of zipped parameters from the internal zipped_parameters list.
+
+        If an element of the internal `_zipped_parameters` array matches ALL labels provided,
+        removes it from the internal `zipped_parameters` method. If no such element is
+        in `_zipped_parameters`, does nothing.
+
+        Parameters
+        ----------
+        labels : str 
+            Any number of string labels matching ALL the names of a set of parameters
+            that has already been zipped.
+        **extra_kwargs: dict
+            Optional Extra keyword-only arguments. Supported argument is
+              - verbose (str): Whether to print if there are no parameters matching `labels`
+                in `_zipped_parameters`. Defaults to `True`.
+        
+        Notes
+        -----
+        .. note::
+            This function should always be used rather than modifying the `_zipped_parameters` attribute
+            directly.
+            
+        Examples
+        --------
+        >>> s = rq.Sensor(3)
+        >>> det = np.linspace(-1,1,11)
+        >>> s.add_coupling(states=(0,1), detuning=det, rabi_frequency=1, label="probe")
+        >>> s.add_coupling(states=(1,2), detuning=det, rabi_frequency=1)
+        >>> s.zip_parameters("probe_detuning", "(1,2)_detuning")
+        >>> print(s._zipped_parameters) #NOT modifying directly
+        >>> s.unzip_parameters('(1,2)_detuning', 'probe_detuning')
+        >>> print(s._zipped_parameters) #NOT modifying directly
+        [['(1,2)_detuning', 'probe_detuning']]
+        []
+        
+        If the labels provided are not a match, a message is printed and nothing is altered. 
+        
+        >>> s = rq.Sensor(3)
+        >>> det = np.linspace(-1,1,11)
+        >>> s.add_coupling(states=(0,1), detuning=det, rabi_frequency=1, label="probe")
+        >>> s.add_coupling(states=(1,2), detuning=det, rabi_frequency=1)
+        >>> s.zip_parameters("probe_detuning", "(1,2)_detuning")
+        >>> print(s._zipped_parameters) #NOT modifying directly
+        >>> s.unzip_parameters('green_detuning', 'probe_detuning')
+        >>> print(s._zipped_parameters) #NOT modifying directly
+        [['(1,2)_detuning', 'probe_detuning']]
+        No zipped parameters matching ['green_detuning', 'probe_detuning']
+        [['(1,2)_detuning', 'probe_detuning']]
+        
+        """
+        labels = list(labels)
+        labels.sort()
+        
+        verbose = extra_kwargs.get("verbose", True)
+
+        for i, param_list in enumerate(self._zipped_parameters):
+            if labels == param_list:
+                del self._zipped_parameters[i]
+                return
+        
+        if verbose:
+            print(f"No zipped parameters matching {labels}")
+
+
+    def add_decoherence(self, states: Tuple[int, ...], gamma: ScannableParameter,
+                        label: Optional[str] = None) -> None:
+        """
+        Add decoherent coupling to the graph between two states.
+
+        If `gamma` is list-like, the sensor will scan over the values,
+        solving the system for each different gamma.
+
+        Parameters
+        ----------
+        states : tuple of ints
+            Length-2 tuple of integers corresponding to the two states. The first
+            value is the number of state out of which population decays, and the 
+            second is the number of the state into which population decays.
+        gamma : float or sequence
+            The decay rate, in Mrad/s.
+        label : str or None, optional
+            Optional label for the decay. If `None`, decay will be stored on
+            the graph edge as `"gamma"`. Otherwise, will cast as a string and decay will be stored
+            on the graph edge as `"gamma_"+label`.
+
+        Notes
+        -----
+        .. note::
+            Adding a decoherece with a particular label (including `None`) will override an existing
+            decoherent transition with that label.
+            
+        Examples
+        --------
+        s = rq.Sensor(3)
+        >>> s.add_coupling(states=(0,1), detuning=1, rabi_frequency=1)
+        >>> s.add_coupling(states=(1,2), detuning=1, rabi_frequency=1)
+        >>> s.add_decoherence((2,0), 0.1, label="misc")
+        >>> print(s.decoherence_matrix())
+        [[0.  0.  0. ]
+        [0.  0.  0. ]
+        [0.1 0.  0. ]]
+        
+        Decoherence values can also be scanned. Here decoherece from states 2->0 is scanned
+        between 0 and 0.5 for 11 values. We can also see how the Hamiltonian shape accounts
+        for this to allow for clean broadcasting, indicating that the hamiltonian is identical
+        accross all decoherence values.
+        
+        >>> s = rq.Sensor(3)
+        >>> gamma = np.linspace(0,0.5,11)
+        >>> s.add_coupling(states=(0,1), detuning=1, rabi_frequency=1)
+        >>> s.add_coupling(states=(1,2), detuning=1, rabi_frequency=1)
+        >>> s.add_decoherence((2,0), gamma)
+        >>> print(s.decoherence_matrix().shape)
+        (11, 3, 3)
+        >>> print(s.get_hamiltonian().shape)
+        (11, 3, 3)
+
+        """
+        if label is None:
+            label_full = "gamma"
+        else:
+            label_full = "gamma_" + str(label)
+
+        states = self._states_valid(states)
+        # invalidate existing decoherence data if already exists
+        self._remove_edge_data(states, kind=label_full)
+        self.couplings.add_edge(*states, **{label_full:gamma})
+
+        # if edge doesn't have a label (ie decoherence only), add a default label
+        if self.couplings.edges[states].get("label") is None:
+            self.couplings.edges[states]["label"] = str(states).replace(" ", "")
+
+
+    def add_transit_broadening(self, gamma_transit: ScannableParameter,
+                               repop: Dict[int, float] = {0: 1.0}) -> None:
+        """
+        Adds transit broadening by adding a decoherence from each node to ground.
+        
+        For each graph node n, adds a decoherent transition from n the specified state (0 by default)
+        using the :meth:`~.Sensor.add_decoherence` method with the `"transit"` label. 
+        See :meth:`~.Sensor.add_decoherence` for more details on labeling.
+
+        If an array of transit values are provided, they will be automatically zipped together
+        into a single scanning element.
+
+        Parameters
+        ----------
+        gamma_transit: float or sequence
+            The transit broadening rate in Mrad/s.
+        repop: dict, optional
+            Dictionary of states for transit to repopulate in to.
+            The keys represent the state labels. The values represent
+            the fractional amount that goes to that state.
+            If the sum of values does not equal 1, population will not be conserved.
+            Default is to repopulate everything into state 0.
+
+        Warns
+        -----
+        If the values of the `repop` parameter do not sum to 1, thus meaning
+        population will not be conserved.
+        
+        Examples
+        --------
+        >>> s = rq.Sensor(3)
+        >>> s.add_transit_broadening(0.1)
+        >>> print(s.couplings.edges(data=True))
+        >>> print(s.decoherence_matrix())
+        [(0, 0, {'gamma_transit': 0.1}), (1, 0, {'gamma_transit': 0.1}), (2, 0, {'gamma_transit': 0.1})]
+        [[0.1 0.  0. ]
+        [0.1 0.  0. ]
+        [0.1 0.  0. ]]
+
+        """  # noqa
+        if isinstance(gamma_transit, list):
+            # needed for multiplying branching ratios
+            gamma_transit = np.array(gamma_transit)
+
+        if not np.isclose(sum(repop.values()), 1.0):
+            warnings.warn(('Repopulation branching ratios do not sum to 1!'
+                           ' Population will not be conserved.'))
+
+        for t, br in repop.items():
+            for i in range(self.basis_size):
+                self.add_decoherence((i, t), gamma=gamma_transit*br, label="transit")
+
+        if isinstance(gamma_transit, (list,np.ndarray)):
+            # need to zip together all the transit rates
+            axes = self.axis_labels()
+            transit_axes = [s for s in axes if s.endswith('gamma_transit')]
+            self.zip_parameters(*transit_axes)
+
+
+    def add_self_broadening(self, node: int, gamma: ScannableParameter,
+                            label: Optional[str] = "self") -> None:
+        """
+        Specify self-broadening (such as collisional broadening) of a level.
+
+        Equivalent to calling :meth:`~.Sensor.add_decoherence` and specifying both
+        states to be the same, with the "self" label. For more complicated systems,
+        it may be useful to further specify the source of self-broadening as, for
+        example, "collisional" for easier bookkeeping and to ensure no values
+        are overwritten.
+
+        Parameters
+        ----------
+        node: int
+            The integer number of the state node to which the broadening
+            will be added. The integer corresponds to the state's position in
+            the graph.
+        gamma: float or sequence
+            The broadening width to be added in Mrad/s.
+        label: str, optional
+            Optional label for the state. If `None`, decay will be stored on
+            the graph edge as `"gamma"`. Otherwise, will cast as a string
+            and decay will be stored on the graph edge as `"gamma_"+label`
+
+        Notes
+        -----
+        .. note::
+            Just as with the :meth:`~.Sensor.add_decoherence` function, adding a decoherence
+            value with a label that already exists will overwrite an existing decoherent
+            transition with that label. The "self" label is applied to this function
+            automatically to help avoid an unwanted overwrite.
+            
+        Examples
+        --------
+        >>> s = rq.Sensor(3)
+        >>> s.add_self_broadening(1, 0.1)
+        >>> print(s.couplings.edges(data=True))
+        >>> print(s.decoherence_matrix())
+        [(1, 1, {'gamma_self': 0.1, 'label': '(1,1)'})]
+        [[0.  0.  0. ]
+        [0.  0.1 0. ]
+        [0.  0.  0. ]]
+
+        """
+        self.add_decoherence((node, node), gamma, label=label)
+
+
+    def decoherence_matrix(self) -> np.ndarray:
+        """
+        Build a decoherence matrix out of the decoherence terms of the graph.
+
+        For each edge, sums all parameters with a key that begins with "gamma",
+        and places it on the appropriate location in an adjacency matrix for the
+        `couplings` graph.
+        
+        Returns
+        -------
+        numpy.ndarray
+            The decoherence matrix stack of the system.
+
+        Examples
+        --------
+        >>> s = rq.Sensor(3)
+        >>> s.add_decoherence((1,0), 0.2, label="foo")
+        >>> s.add_decoherence((1,0), 0.1, label="bar")
+        >>> s.add_decoherence((2,0), 0.05)
+        >>> s.add_decoherence((2,1), 0.05)
+        >>> print(s.couplings.edges(data=True))
+        >>> print(s.decoherence_matrix())
+        [(1, 0, {'gamma_foo': 0.2, 'label': '(1,0)', 'gamma_bar': 0.1}), (2, 0, {'gamma': 0.05, 'label': '(2,0)'}), (2, 1, {'gamma': 0.05, 'label': '(2,1)'})]
+        [[0.   0.   0.  ]
+        [0.3  0.   0.  ]
+        [0.05 0.05 0.  ]]
+        
+        Decoherences can be stacked just like any parameters of the Hamiltonian:
+        
+        >>> s = rq.Sensor(3)
+        >>> gamma = np.linspace(0,0.5, 11)
+        >>> s.add_decoherence((1,0), gamma)
+        >>> print(s.decoherence_matrix().shape)
+        (11,3,3)   
+             
+        """
+        base_couplings = self.couplings.copy()
+
+        stack_shape = self._stack_shape(collapse=False)
+        for states, param, arr in self.variable_parameters(apply_mesh=True):
+            self.couplings.edges[states][param] = arr
+
+        gamma_shape = (*stack_shape, self.basis_size, self.basis_size)
+        gamma_matrix = np.zeros(gamma_shape, np.float64)
+
+        # get a list of all unique parameter labels containing "gamma"
+        labels_lists = [list(d.keys()) for _,_,d in self.couplings.edges(data=True)]
+        all_labels = list(set(sum(labels_lists, start=[])))
+        decoherence_labels = [l for l in all_labels if "gamma" in l]
+
+        # for each unique decoherence name,
+        for label in decoherence_labels:
+            for states, f in self.couplings_with(label).items():
+
+                idx = (..., *states)
+                gamma_matrix[idx] += f[label]
+
+        if len(self._zipped_parameters) > 0:
+            gamma_matrix = self.collapse_dims(gamma_matrix)
+
+        self.couplings = base_couplings
+        return gamma_matrix
+
+
+    def axis_labels(self, collapse: bool = True) -> List[str]:
+        """
+        Get a list of axis labels for stacked hamiltonians. 
+        
+        The axes of a hamiltonian
+        stack are defined as the axes preceding the usual hamiltonian, which are always
+        the last 2. These axes only exist if one of the parametes used to define
+        a Hamiltonian are lists.
+
+        Be default, labels which have been zipped using :meth:`~.Sensor.zip_parameters`
+        will be combined into a single label, as this is how :meth:`~.Sensor.get_hamiltonian`
+        treats these axes.
+
+        Returns
+        -------
+        list of str 
+            Strings corresponding to the label of each axis on a stack
+            of multiple hamiltonians.
+
+        Examples
+        --------
+        There are no preceding axes if there are no list-like parameters.
+
+        >>> s = rq.Sensor(3)
+        >>> blue = {"states":(0,1), "rabi_frequency":1, "detuning":2}
+        >>> red = {"states":(1,2), "rabi_frequency":3, "detuning":4}
+        >>> s.add_couplings(blue, red)
+        >>> print(s.get_hamiltonian().shape())
+        >>> print(s.axis_labels())
+        (3,3)
+        []
+
+        Adding list-like parameters expands the hamiltonian
+
+        >>> s = rq.Sensor(3)
+        >>> det = np.linspace(-10, 10, 11)
+        >>> blue = {"states":(0,1), "rabi_frequency":1, "detuning":det, "label":"blue"}
+        >>> red = {"states":(1,2), "rabi_frequency":3, "detuning":det}
+        >>> s.add_couplings(blue, red)
+        >>> print(s.get_hamiltonian().shape)
+        >>> print(s.axis_labels())
+        (11, 11, 3, 3)
+        ['blue_detuning', '(1, 2)_detuning']
+
+        Zipping parameters combines their corresponding labels, since their Hamiltonians now 
+        lie on a single axis of the stack. Here the axis of length 7 (axis 0) corresponds to the
+        rabi frequencies and the axis of shape 11 (axis 1) corresponds to the zipped detunings
+        
+        >>> s = rq.Sensor(3)
+        >>> s.add_coupling(states=(0,1), detuning=np.arange(11), rabi_frequency=np.linspace(-3, 3, 7))
+        >>> s.add_coupling(states=(1,2), detuning=0.5*np.arange(11), rabi_frequency=1)
+        >>> s.zip_parameters("(0,1)_detuning", "(1,2)_detuning")
+        >>> print(s.get_hamiltonian().shape)
+        >>> print(s.axis_labels())
+        (7, 11, 3, 3)
+        ['(0,1)_rabi_frequency', '(0,1)_detuning|(1,2)_detuning']
+        
+        """ # noqa
+        axis_labels = []
+
+        # build the base list of axis labels based just on couplings
+        for states, param, _ in self.variable_parameters():
+            if 'label' in self.couplings.edges[states].keys():
+                label = str(self.couplings.edges[states]['label']) + '_' + str(param)
+            else:
+                label = str(states) + "_" + str(param)
+            axis_labels.append(label)
+
+        # combine labels for parameters that have been zipped and move to the end of stack
+        if collapse:
+            for params in self._zipped_parameters:
+                new_label = _combine_parameter_labels(*params)
+
+                for p in params:
+                    axis_labels.remove(p)
+
+                axis_labels.append(new_label)
+
+        return axis_labels
+
+
+    def variable_parameters(self, apply_mesh=False):
+        """
+        Property to retrieve the values of parameters that were stored on the graph as arrays.
+
+        Values are returned as a list of tuples in the standard order of pythons default sorting,
+        applied first to the tuple indicating states and then to the key of the parameter itself. 
+        This means that couplings are sorted first by lower state, then by upper state, then 
+        alphabetically by the name of the parameter. 
+
+        Returns
+        -------
+        list of tuples
+            A list of tuples corresponding to the parameters of the systems that are variable 
+            (i.e. stored as an array). They are ordered accordning to states, then according to variable 
+            name. Tuple entries of the list take the form `(states, param_name, value)`
+
+        Examples
+        --------
+        >>> s = rq.Sensor(3)
+        >>> vals = np.linspace(-1,2,3)
+        >>> s.add_coupling(states=(1,2), rabi_frequency=vals, detuning=1)
+        >>> s.add_coupling(states=(0,1), rabi_frequency=vals, detuning=vals)
+        >>> for states, key, value in s.variable_parameters():
+        ...     print(f"{states}: {key}={value}")
+        (0, 1): detuning=[-1.   0.5  2. ]
+        (0, 1): rabi_frequency=[-1.   0.5  2. ]
+        (1, 2): rabi_frequency=[-1.   0.5  2. ]
+        
+        """
+        l=[]
+        for states in sorted(self.couplings.edges):
+            
+            edge_data = self.couplings.edges.get(states)
+            
+            for key, value in sorted(edge_data.items()):
+                if not key.startswith("gamma") and key not in BASE_SCANNABLE_KEYS:
+                    continue
+
+                if isinstance(value, (list,np.ndarray)):
+                    l.append((states, key, value))
+        
+        if apply_mesh:
+            vals = [val for _,_,val in l]
+            mesh_vals = np.meshgrid(*vals, indexing='ij', sparse=True)
+            l = [(*l[i][:2], mesh_vals[i].copy()) for i in range(len(l))]
+
+        return l
+
+
+    def get_parameter_mesh(self, sparse:bool=True, **kwargs) -> Tuple[np.ndarray, ...]:
+        """
+        Returns the parameter mesh of the sensor.
+
+        The parameter mesh is the flattened grid of variable parameters in all the couplings of a sensor.
+        Wraps `numpy.meshgrid` by passing arguments as the variable parameters in a
+        sensor. The `indexing` argument is always `"ij"` for matrix indexing. 
+        For full documention of all arguments, see `numpy.meshgrid` documentation.
+        Argument documentation copied from `numpy.meshgrid`.
+
+        Parameters
+        ----------
+        sparse : bool, optional
+            If `True`, the shape of the returned coordinate array for dimension i is 
+            reduced from `(N1, ..., Ni, ... Nn)` to `(1, ..., 1, Ni, 1, ..., 1)`. 
+            These sparse coordinate grids are intended to be used in a way consistent 
+            with numpy's broadcasting conventions. When all coordinates are used in an 
+            expression, broadcasting still leads to a fully-dimensonal result array. 
+            Recommended to keep as `True`. Default is `True`.
+        kwargs : dict, optional
+            Additional keyword arguments to pass to `numpy.meshgrid`. All arguments are 
+            passed directly to `numpy.meshgrid` with the exception of `indexing`, which 
+            is fixed to `"ij"` and cannot be specified.
+            
+        Examples
+        --------
+        >>> s = rq.Sensor(3)
+        >>> rabi1 = np.linspace(-1,1,11)
+        >>> rabi2 = np.linspace(-2,2,21)
+        >>> s.add_coupling(states=(0,1), rabi_frequency=rabi1, detuning=1)
+        >>> s.add_coupling(states=(1,2), rabi_frequency=rabi2, detuning=1)
+        >>> for p in s.get_parameter_mesh():
+        ...     print(p.shape)
+        (11, 1)
+        (1, 21)
+        
+        """
+        if "indexing" in kwargs.keys():
+            raise TypeError("get_parameter_mesh() got an unexpected keyword argument \'indexing\'")
+
+        vals = [v for _,_,v in self.variable_parameters()]
+
+        parameter_mesh = np.meshgrid(*vals, indexing='ij', sparse=sparse, **kwargs)
+        return parameter_mesh
+
+
+    def get_hamiltonian(self) -> np.ndarray:
+        """
+        Creates the Hamiltonians from the couplings defined by the fields.
+
+        They will only be the steady state hamiltonians, i.e. will only contain
+        terms which do not vary with time. Implicitly creates hamiltonians in "stacks"
+        by creating a grid of all supported coupling parameters which are lists.
+        This grid of parameters will not contain rabi-frequency parameters which
+        vary with time and are defined as list-like. Rather, the associated axis
+        will be of length 1, with the scanning over this value handled by the
+        :meth:`~Sensor.get_time_couplings` function.
+
+        For m list-like parameters x1,x2,...,xm with shapes N1,N2,...,Nm, and basis
+        size n, the output will be shape `(N1,N2,...,Nm, n, n)`. The dimensions
+        N1,N2,...Nm are labeled by the output of :meth:`~.Sensor.axis_labels`.
+
+        If any parameters have been zipped with the :meth:`~.Sensor._zip_parameters`
+        method, those parameters will share an axis in the final hamiltonian stack.
+        In this case, if axis N1 and N2 above are the same shape and zipped, the final
+        Hamiltonian will be of shape `(N1,...,Nm, n, n)`
+        
+        See rydiqule's conventions for matrix stacking for more details.
+
+        Returns
+        -------
+        np.ndarray
+            The complex hamiltonian stack for the sensor.
+
+        Examples
+        --------
+        >>> s = rq.Sensor(3)
+        >>> det = np.linspace(-1,1,11)
+        >>> blue = {"states":(0,1), "rabi_frequency":1, "detuning":det}
+        >>> red = {"states":(1,2), "rabi_frequency":3, "detuning":det}
+        >>> s.add_couplings(red, blue)
+        >>> print(s.get_hamiltonian().shape)
+        (11, 11, 3, 3)
+        
+        Time dependent couplings are handled separately. The axis that contains array-like
+        parameters with time dependence is length 1 in the steady-state Hamiltonian.
+        
+        >>> s = rq.Sensor(3)
+        >>> rabi = np.linspace(-1,1,11)
+        >>> step = lambda t: 0 if t<1 else 1
+        >>> blue = {"states":(0,1), "rabi_frequency":rabi, "detuning":1}
+        >>> red = {"states":(1,2), "rabi_frequency":rabi, "detuning":0, 'time_dependence': step}
+        >>> s.add_couplings(red, blue)
+        >>> print(s.get_hamiltonian().shape)
+        (11, 1, 3, 3)
+
+        Zipping parameters means they share an axis in the Hamiltonian.
+
+        >>> s = rq.Sensor(3)
+        >>> s.add_coupling(states=(0,1), detuning=np.arange(11), rabi_frequency=2)
+        >>> s.add_coupling(states=(1,2), detuning=0.5*np.arange(11), rabi_frequency=1)
+        >>> s.zip_parameters("(0,1)_detuning", "(1,2)_detuning")
+        >>> H = s.get_hamiltonian()
+        >>> print(H.shape)
+        (11, 3, 3)
+
+        """
+        base_couplings = self.couplings.copy()
+
+        stack_shape = self._stack_shape(collapse=False, time_dependence='steady')
+
+        for states, param, arr in self.variable_parameters(apply_mesh=True):
+            # print(states, param, arr.shape)
+            self.couplings.edges[states][param] = arr
+
+        hamiltonian_shape = (*stack_shape, self.basis_size, self.basis_size)
+        # returns diagonal elements of Hamiltonian
+        transition_frequencies = self.get_transition_frequencies()
+        #define hamiltonian and place terms from above on diagonal
+        hamiltonian = np.zeros(hamiltonian_shape, np.complex128)
+        np.einsum("...ii->...i", hamiltonian)[:] = transition_frequencies
+
+        for states, f in self.couplings_with('time_dependence', method='not any').items():
+
+            if 'rabi_frequency' not in f:
+                continue
+
+            idx = (...,*states)
+            conj_idx = (...,*states[::-1])
+
+            # factor of 1/2 accounts for implicit rotating wave approximation
+
+            hamiltonian[idx] = (f['rabi_frequency']*np.cos(f['phase'])
+                                + 1j*f['rabi_frequency']*np.sin(f['phase']))/2
+            hamiltonian[conj_idx] = np.conj(hamiltonian[idx])
+
+        if len(self._zipped_parameters) > 0:
+            hamiltonian = self.collapse_dims(hamiltonian)
+
+        self.couplings = base_couplings
+        return hamiltonian
+
+
+    def collapse_dims(self, stack: np.ndarray) -> np.ndarray:
+        """
+        Collapse dimensions of a stack accoring to the `_zipped_parameters` attribute.
+       
+        Designed primarily for internal use, but can be called externally or
+        in custom overloads of :meth:`~.Sensor.get_hamiltonian`. Effectively performs
+        a `numpy.einsum` operation to replicate `numpy.diag` along the appropriate
+        dimensions. 
+
+        Parameters
+        ----------
+        stack : numpy.ndarray
+            Array with shape matching uncollapsed system hamiltonians. 
+
+        Returns
+        -------
+        numpy.ndarray
+            Input array with appropriate dimensions removed via a numpy.diag-like operation.
+
+        """
+        axis_labels = self.axis_labels(collapse=False)
+
+        paired_axes = []
+
+        for couplings in self._zipped_parameters:
+            paired_axes.append([axis_labels.index(c) for c in couplings])
+
+        einsum_str = _get_collapse_str(len(axis_labels), *paired_axes)
+        collapsed_stack = np.einsum(einsum_str, stack)
+
+        return collapsed_stack
+
+
+    def get_time_hamiltonians(self) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """
+        Get the hamiltonians for the time solver.
+
+        Get both the steady state hamiltonian (as returned by :meth:`~.Sensor.get_hamiltonian`)
+        and the time_dependent hamiltonians (as returned by :meth:`~.Sensor.get_time_couplings`).
+        The time dependent hamiltonians give 2 terms, the hamiltonian corresponding
+        to the real part of the coupling and the hamiltonian corresponding to the imaginary part.
+
+        Returns
+        -------
+        hamiltonian_base : np.ndarray
+            The `(*l,n,n)` shape base hamiltonian of the system containing
+            all elements that do not depend on time, where `n` is the basis size
+            of the sensor.
+
+        dipole_matrix_real : np.ndarray
+            The `(M,n,n)` shape array of matrices representing the real
+            time-dependent portion of the hamiltonian. For `0 <= i <= M`,
+            the ith value along the first axis is the portion of the matrix which
+            will be multiplied by the output of the ith `time_dependence` function.
+
+        dipole_matrix_imag: nd.ndarray
+            The `(M,n,n)` shape array of matrices representing the imaginary
+            time-dependent portion of the hamiltonian. For `0 <= i <= M`,
+            the ith value along the first axis is the portion of the matrix which
+            will be multiplied by the output of the ith `time_dependence` function.
+
+        Examples
+        --------
+        >>> s = rq.Sensor(2)
+        >>> step = lambda t: 0. if t<1 else 1.
+        >>> s.add_coupling(states=(0,1), detuning=1, rabi_frequency=1, time_dependence=step)
+        >>> H_base, H_time_real, H_time_imaginary = s.get_time_hamiltonians()
+        >>> print(H_base)
+        >>> print(H_time_real)
+        >>> print(H_time_imaginary)
+        [[0.+0.j 0.+0.j]
+        [0.+0.j 1.+0.j]]
+        [array([[0. +0.j, 0.5+0.j],
+            [0.5+0.j, 0. +0.j]])]
+        [array([[0.+0.j , 0.+0.5j],
+            [0.-0.5j, 0.+0.j ]])]
+
+        """
+        hamiltonian_base = self.get_hamiltonian()
+        dipole_matrices = self.get_time_couplings()
+
+        return hamiltonian_base, *dipole_matrices
+
+
+    def get_time_couplings(self) -> Tuple[np.ndarray, np.ndarray]:
+        """
+        Returns the list of matrices of all couplings in the system defined with
+        a `time_dependence` key.
+
+        The ouput will be two lists of matricies representing which terms of the hamiltonian
+        are dependent on each time-dependent coupling. The lists will be of length M and shape `(*l_time, n, n)`,
+        where M is the number of time-dependent couplings, `l_time` is time-dependent stack shape
+        (possibly all ones), and `n` is the basis size. Each matrix will have terms equal to the rabi frequency
+        (or half the rabi frequency under RWA) in positions that correspond to the associated transition.
+        For example, in the case where there is a `time_dependence` function defined for the `(2,3)` transition
+        with a rabi frequency of 1, the associated time coupling matrix will be all zeros, with a 1 in the `(2,3)`
+        and `(3,2)` positions.
+
+        Typically, this function is called internally and multiplied by the output of the :meth:`~.Sensor.get_time_dependence`
+        function.
+
+        Returns
+        -------
+        list of numpy.ndarray
+            The list of M `(*l,n,n)` matrices representing the
+            real-valued time-dependent portion of the hamiltonian. For `0 <= i <= M`,
+            the ith value along the first axis is the portion of the matrix which
+            will be multiplied by the output of the ith `time_dependence` function.
+            
+        list of numpy.ndarray
+            The list of M `(*l,n,n)` matrices representing the
+            imaginary-valued time-dependent portion of the hamiltonian. For `0 <= i <= M`,
+            the ith value along the first axis is the portion of the matrix which
+            will be multiplied by the output of the ith `time_dependence` function.
+
+        Examples
+        --------
+        >>> s = rq.Sensor(3)
+        >>> step = lambda t: 0 if t<1 else 1
+        >>> wave = lambda t: np.sin(2000*np.pi*t)
+        >>> f1 = {"states": (0,1), "transition_frequency":10, "rabi_frequency": 1, "time_dependence":wave}
+        >>> f2 = {"states": (1,2), "transition_frequency":10, "rabi_frequency": 2, "time_dependence":step}
+        >>> s.add_couplings(f1, f2)
+        >>> time_hams, time_hams_i = s.get_time_couplings()
+        >>> for H in time_hams:
+        ...     print(H)
+        [[0.+0.j 1.+0.j 0.+0.j]
+        [1.+0.j 0.+0.j 0.+0.j]
+        [0.+0.j 0.+0.j 0.+0.j]]
+        [[0.+0.j 0.+0.j 0.+0.j]
+        [0.+0.j 0.+0.j 2.+0.j]
+        [0.+0.j 2.+0.j 0.+0.j]]
+            
+        To handle stacking across the steady-state and time hamiltonians, the dimensions are 
+        matched in a way that broadcasting works in a numpy-friendly way
+        
+        >>> s = rq.Sensor(3)
+        >>> rabi = np.linspace(-1,1,11)
+        >>> step = lambda t: 0 if t<1 else 1
+        >>> blue = {"states":(0,1), "rabi_frequency":rabi, "detuning":1}
+        >>> red = {"states":(1,2), "rabi_frequency":rabi, "detuning":0, 'time_dependence': step}
+        >>> s.add_couplings(red, blue)
+        >>> time_hams, time_hams_i = s.get_time_couplings()
+        >>> print(s.get_hamiltonian().shape)
+        >>> print(time_hams[0].shape)
+        >>> print(time_hams_i[0].shape)
+        (1, 11, 3, 3)
+        (11, 1, 3, 3)
+        (11, 1, 3, 3)
+
+        """ # noqa
+        #save to re-add later
+        base_couplings = self.couplings.copy()
+
+        stack_shape = self._stack_shape(collapse=False, time_dependence='time')
+
+        for states, param, arr in self.variable_parameters(apply_mesh=True):
+            self.couplings.edges[states][param] = arr
+
+        hamiltonian_shape = (*stack_shape, self.basis_size, self.basis_size)
+
+        matrix_list = []
+        matrix_list_i = []
+
+        #loop over time-dependent couplings
+        for states, f in self.couplings_with("time_dependence").items():
+            
+            if 'rabi_frequency' not in f:
+                continue
+            
+            time_hamiltonian = np.zeros(hamiltonian_shape, dtype='complex')
+            time_hamiltonian_i = np.zeros(hamiltonian_shape, dtype='complex')
+
+            idx = (...,*states)
+            conj_idx = (...,*states[::-1])
+            
+            #ignores numpy casting to real warning that we already account for
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")
+                if 'transition_frequency' in f:
+                    time_hamiltonian[idx] = f['rabi_frequency']
+                    time_hamiltonian[conj_idx] = np.conj(f["rabi_frequency"])
+                    time_hamiltonian_i[idx] = 1j*f["rabi_frequency"]
+                    time_hamiltonian_i[conj_idx] = np.conj(f["rabi_frequency"]*1j)
+                
+                #factor of 1/2 for rwa
+                else:
+                    time_hamiltonian[idx] = f['rabi_frequency']/2
+                    time_hamiltonian[conj_idx] = np.conj(f["rabi_frequency"])/2
+                    time_hamiltonian_i[idx] = 1j*f["rabi_frequency"]/2
+                    time_hamiltonian_i[conj_idx] = np.conj(f["rabi_frequency"]*1j)/2
+
+            matrix_list.append(time_hamiltonian)
+            matrix_list_i.append(time_hamiltonian_i)
+            
+        self.couplings = base_couplings
+
+        return matrix_list, matrix_list_i
+
+
+    def get_time_dependence(self) -> List[Callable[[float], float]]:
+        """
+        Function which returns a list of the `time_dependence` functions.
+        
+        The list is returned with in the order that matches with the time hamiltonians from 
+        :meth:`~.Sensor.get_time_couplings` such that the ith element of of the return of this
+        functions corresponds with the ith Hamiltonian terms returned by that function. 
+
+        Returns
+        -------
+        list
+            List of scalar functions, representing all couplings specified with a `time_dependence`.
+            
+
+        Examples:
+            >>> s = rq.Sensor(3)
+            >>> step = lambda t: 0 if t<1 else 1
+            >>> wave = lambda t: np.sin(2000*np.pi*t)
+            >>> f1 = {"states": (0,1), "transition_frequency":10, "rabi_frequency": 1, "time_dependence":wave}
+            >>> f2 = {"states": (1,2), "transition_frequency":10, "rabi_frequency": 2, "time_dependence":step}
+            >>> s.add_couplings(f1, f2)
+            >>> print(s.get_time_dependence())
+            [<function <lambda> at 0x7fb310edd9d0>, <function <lambda> at 0x7fb37c0c81f0>]
+
+        """ # noqa
+        time_dependence = []
+        for (i,j),f in self.couplings_with("time_dependence").items():
+            time_dependence.append(f['time_dependence'])
+        return time_dependence
+
+
+    def get_hamiltonian_diagonal(self, values: dict, no_stack: bool=False) -> np.ndarray:
+        """
+        Apply addition and subtraction logic corresponding to the direction of the couplings.
+
+        For a given state `n`, the path from ground will be traced to `n`. For each edge along this
+        path, values will be added where the path direction and coupling direction match, and subtracting
+        values where they do not. The sum of all such values along the path is the `n` th term in
+        the output array. 
+
+        Primarily for internal functions which help generate hamiltonians. Most commonly used
+        to calculate total detunings for ranges of couplings under the RWA
+
+        Parameters
+        ----------
+        values : dict
+            Key-value pairs where the keys correspond to transitions
+            (agnostic to ordering of states) and values corresponding to the values
+            to which the logic will be applied.
+        no_stack : bool, optional
+            Whether to ignore variable parameters in the system and
+            use only basic math operations rather than reshape the output. Typically
+            only `True` for calculating doppler shifts.
+
+        Returns
+        -------
+        numpy.ndarray
+            The digonal of the hamiltonian of the system of shape `(*l,n)`,
+            where `l` is the shape of the hamiltonian stack for the sensor.
+
+        """
+        coherent_edges = [
+            states for states in self.couplings.edges
+            if "rabi_frequency" in self.couplings.edges[states]
+            ]
+
+        coherent_graph = self.couplings.edge_subgraph(coherent_edges)
+
+        if no_stack:
+            diag = np.zeros(self.basis_size)
+        else:
+            diag = np.zeros((*self._stack_shape(collapse=False, time_dependence="steady"), self.basis_size), dtype=np.complex128)
+
+        connected_levels = nx.weakly_connected_components(coherent_graph)
+        subgraphs = [coherent_graph.subgraph(ls) for ls in connected_levels]
+
+        for g in subgraphs:
+
+            # min sets lowest state in graph as "ground"
+            paths = nx.shortest_path(nx.to_undirected(g), source=min(g.nodes))
+            paths_np = {k:np.array(v) for k,v in paths.items()}  # convert to numpy arrays
+
+            for i, path in paths_np.items():
+
+                term = 0
+
+                for j in range(1, len(path)):
+
+                    # get the jth couplings along the path and initialize the sign as positive
+                    field = tuple(np.copy(path[j-1:j+1]))
+                    sign = 1
+
+                    if field not in self.couplings.edges:
+                        # switch the sign if the arrow points in the opposite direction
+                        # This corresponds to moving to a lower energy state
+                        # Since it is getting an existing edge from the undirected graph,
+                        # we are guaranteed either field or field[::-1] being on the graph
+                        field = field[::-1]
+                        sign = -1
+
+                    # sum to the cumulative term along the path from ground
+                    term = term + values.get(field,0)*sign
+
+                diag[..., i] = term
+
+        return diag
+
+
+    def get_transition_frequencies(self) -> np.ndarray:
+        """
+        Gets an array of the diagonal elements of the Hamiltonian from the field detunings.
+
+        Wraps the :meth:`~.Sensor.get_hamiltonian_diagonal` function using both transition frequencies and detunings.
+        Primarily for internal use. 
+
+        Returns
+        -------
+        numpy.ndarray
+            N-D array of the hamiltonian diagonal. For an n-level system with stack shape `*l`,
+            will be shape `(*l, n)`
+            
+        """
+        detuning_dict = self.get_value_dictionary("detuning")
+        transition_frequency_dict = self.get_value_dictionary("transition_frequency")
+        freq_dict = {**detuning_dict, **transition_frequency_dict}
+        return self.get_hamiltonian_diagonal(freq_dict)
+
+
+    def get_value_dictionary(self, key: str) -> dict:
+        """
+        Get subset of dictionary coupling parameters.
+
+        Return a dictionary of key value pairs where the keys are couplings added
+        to the system and the values are the value of the parameter specified by key.
+        Produces an output that can be passed directly to :meth:`~.get_hamiltonian_diagonal`.
+        Only couplings whose parameter dictionaries contain "key" will be in the
+        returned dictionary.
+
+        Parameters
+        ----------
+        key : str
+            String value of the parameter name to build the dictionary.
+            For example, `get_value_dictionary("detuning")` will return a dictionary with keys
+            corresponding to transitions and values corresponding to detuning
+            for each transition which has a detuning.
+
+        Returns
+        -------
+        dict
+            Coupling dictionary with couplings as keys and corresponding
+            values set by input key.
+
+        Examples
+        --------
+        >>> s = rq.Sensor(4)
+        >>> f1 = {"states": (0,1), "detuning": 2, "rabi_frequency": 1}
+        >>> f2 = {"states": (1,2), "detuning": 3, "rabi_frequency": 2}
+        >>> f3 = {"states": (2,3), "rabi_frequency": 3, "transition_frequency": 3}
+        >>> s.add_couplings(f1, f2, f3)
+        >>> print(s.get_value_dictionary("detuning"))
+        {(0,1): 2, (1,2): 3}
+
+        """
+        couplings_with_key = self.couplings_with(key)
+        return {states:params[key] for states, params in couplings_with_key.items()}
+
+
+    def set_gamma_matrix(self, gamma_matrix: np.ndarray) -> None:
+        """
+        Set the decoherence matrix for the system. 
+        
+        Works by first removing all existing decoherent data from graph edges, then 
+        individually adding all nonzero terms of a provided gamma matrix to the corresponding graph edges.
+        Can be used to set all decoherence attributes to edges simultaneously, but :meth:`~.add_decoherence`
+        is preferred.
+        
+        Unlike :meth:`~.add_decoherence`, does not support scanning multiple decoherence values,
+        rather should be used to set the decoherences of the system to individual static values.
+
+        Parameters
+        ----------
+        gamma_matrix : numpy.ndarray
+            Array of shape `(basis_size, basis_size)`.
+            Element `(i,j)` describes the decoherence rate, in Mrad/s,
+            from state `i` to state `j`.
+
+        Raises
+        ------
+        TypeError
+            If `gamma_matrix` is not a numpy array.
+        ValueError
+            If `gamma_matrix` is not a square matrix of the appropriate size
+        ValueError
+            If the shape of `gamma_matrix` is not compatible with `self.basis_size`.
+
+        Examples
+        --------
+        >>> s = rq.Sensor(2)
+        >>> f1 = {"states": (0,1), "transition_frequency":10, "rabi_frequency": 1}
+        >>> s.add_couplings(f1)
+        >>> gamma = np.array([[.1,0],[.1,0]])
+        >>> s.set_gamma_matrix(gamma)
+        >>> print(s.decoherence_matrix())
+        [[0.1 0. ]
+        [0.1 0. ]]
+
+        """
+        if not isinstance(gamma_matrix, np.ndarray):
+            raise TypeError(f'gamma_matrix must be a numpy array, not type {type(gamma_matrix)}')
+
+        if gamma_matrix.shape != (self.basis_size,self.basis_size):
+            raise ValueError((f'gamma_matrix has shape {gamma_matrix.shape}, '
+                              f'must be {(self.basis_size,self.basis_size)}'))
+
+        for states, gamma in np.ndenumerate(gamma_matrix):
+            
+            #remove existing decoherence data
+            if self.couplings.has_edge(*states):
+                
+                remove_keys = []
+                for key in self.couplings.edges[states].keys():
+                    if key.startswith("gamma_"):
+                        remove_keys.append(key)
+                        
+                for key in remove_keys:
+                    del self.couplings.edges[states][key]
+            
+            #add new decoherence
+            if gamma != 0: 
+                #exclude gamma==0; its implicitly put there in decoherence_matrix()
+                self.add_decoherence(states, gamma)
+
+
+    def get_doppler_shifts(self) -> np.ndarray:
+        """
+        Returns the Hamiltonian with only detunings set to the kvector values for
+        each spatial dimension.
+
+        Determining if a float should be treated as zero is done using :obj:`numpy.isclose`,
+        which has default absolute tolerance of `1e-08`.
+
+        Returns
+        -------
+        numpy.ndarray
+            Array of shape (used_spatial_dim,n,n), Hamiltonians
+            with only the doppler shifts present along each non-zero spatial dimension
+            specified by the fields' "kvec" parameter.
+
+        """
+        spatial_dim = 3
+
+        kvecs = self.get_value_dictionary('kvec')
+        # collect shifts for each spatial dimension that is non-zero
+        s_kvecs = [{k:v[i] for k,v in kvecs.items() if ~np.isclose(v[i],0)}
+                   for i in range(spatial_dim)]
+        if not any(s_kvecs):
+            raise ValueError(('You must specify at least one non-zero '
+                              'kvector to do doppler averaging.'))
+        # get hamiltonian diagonal for each non-zero spatial dimension
+        frequencies = np.array([self.get_hamiltonian_diagonal(s_kvec, no_stack=True)
+                                for s_kvec in s_kvecs if s_kvec])
+        # expand to full hamiltonians
+        doppler_hamiltonians = np.eye(self.basis_size) * frequencies[:,np.newaxis,:]
+
+        assert self.spatial_dim() == doppler_hamiltonians.shape[0], \
+            'Spatial dimension inconsistency'
+
+        return doppler_hamiltonians
+
+
+    def couplings_with(self, *keys: str,
+                       method: Literal['all','any', 'not any'] = "all"
+                       ) -> Dict[States, CouplingDict]:
+        """
+        Returns a version of self.couplings with only the keys specified.
+        
+        Can be specified with a several criteria, including all, none, or any of the keys
+        specified.
+
+        Parameters
+        ----------
+        keys(tuple of str): tuple of strings which should be one the valid
+            parameter names for a state. See :meth:`~.add_coupling` for which
+            names are valid for a Sensor object.
+        method : {'all','any', 'not any'} 
+            Method to see if a given field matches the keys
+            given. Choosing "all" will return couplings
+            which have keys matching all of the values provided in the keys
+            argument, while coosing "any", will return all couplings with keys
+            matching at least one of the values specified by keys. For example,
+            `sensor.couplings_with("rabi_frequency")` returns a dictionary of
+            all couplings for which a rabi_frequency was specified.
+            `sensor.couplings_with("rabi_frequency", "detuning", method="all")`
+            returns all couplings for which both rabi_frequency and detuning
+            are specified.
+            'sensor.couplings_with("rabi_frequency", "detuning", method="any")`
+            returns all couplings for which either rabi_frequency or detuning
+            are specified.
+            Defaults to "all".
+
+        Returns
+        -------
+        dict
+            A copy of the `sensor.couplings` dictionary with only couplings containing
+            the specified parameter keys.
+
+        Examples
+        --------
+        Can be used, for example, to return couplings in the roating wave approximation.
+        
+        >>> s = rq.Sensor(3)
+        >>> sinusoid = lambda t: 0 if t<1 else sin(100*t)
+        >>> f2 = {"states": (0,1), "detuning": 1, "rabi_frequency":2}
+        >>> f1 = {"states": (1,2), "transition_frequency":100, "rabi_frequency":1, "time_dependence": sinusoid}
+        >>> s.add_couplings(f1, f2)
+        >>> gamma = np.array([[.2,0,0],
+        ...                  [.1,0,0],
+        ...                  [0.05,0,0]])
+        >>> s.set_gamma_matrix(gamma)
+        >>> print(s.couplings_with("detuning"))
+        {(0, 1): {'rabi_frequency': 2, 'detuning': 1, 'phase': 0, 'kvec': (0, 0, 0), 'no_rwa_warning': False, 'label': '(0,1)'}}
+        """
+        def notAll(x):
+            return not all(x)
+
+        def notAny(x):
+            return not any(x)
+
+        methods = {"any":any, "all":all, "not any": notAny, "not all": notAll}
+
+        return {s:p
+                for s,p in self.couplings.edges.items()
+                if methods[method]([k in p for k in keys])
+                }
+
+
+    def get_couplings(self) -> Dict[States, CouplingDict]:
+        """
+        Returns the couplings of the system as a dictionary
+        
+        Deprecating in favor of calling the couplings.edges attribute directly. 
+
+        Returns
+        -------
+        dict
+            A dictionary of key-value pairs with the keys corresponding to levels of
+            transition, and the values being dictionaries of coupling attributes.
+
+        """
+        return {s:p for s,p in self.couplings.edges.items()}
+
+
+    def spatial_dim(self) -> int:
+        """
+        Returns the number of spatial dimensions doppler averaging will occur over.
+
+        Determining if a float should be treated as zero is done using :obj:`numpy.isclose`,
+        which has default absolute tolerance of `1e-08`.
+
+        Returns
+        -------
+        int
+            Number of dimensions, between 0 and 3,
+            where 0 means no doppler averaging kvectors have been specified
+            or are too small to be calculates. 
+            
+        Examples
+        --------
+        No spatial dimesions specified
+        
+        >>> s = rq.Sensor(2)
+        >>> s.add_coupling((0,1), detuning = 1, rabi_freqency=1)
+        >>> print(s.spatial_dim())
+        0
+        
+        One spatial dimension specified
+        
+        >>> s = rq.Sensor(2)
+        >>> s.add_coupling((0,1), detuning = 1, rabi_freqency=1, kvec=(0,0,1))
+        >>> print(s.spatial_dim())
+        1
+        
+        Multiple spatial dimensions can exist in a single coupling or 
+        across multiple couplings
+        
+        >>> s = rq.Sensor(2)
+        >>> s.add_coupling((0,1), detuning = 1, rabi_freqency=1, kvec=(1,0,1))
+        >>> print(s.spatial_dim())
+        2
+        
+        >>> s = rq.Sensor(3)
+        >>> s.add_coupling((0,1), detuning = 1, rabi_freqency=1, kvec=(1,0,1))
+        >>> s.add_coupling((1,2), detuning = 2, rabi_freqency=2, kvec=(0,1,0))
+        >>> print(s.spatial_dim())
+        3
+        """
+        k_vector_dim = np.zeros(3,dtype=bool)
+
+        for key, field in self.couplings.edges.items():
+            if 'kvec' in field:
+                k_vector_dim = k_vector_dim | ~np.isclose(field['kvec'],0)
+
+        return np.sum(k_vector_dim)
+
+
+    def _states_valid(self, states: States) -> States:
+        """
+        Confirms that the provided states are in a valid format.
+        
+        Typically used internally to validate states added. If provided as 
+        a form other than a tuple, first casts to a tuple for consistent
+        indexing.
+        
+        Checks that `states` contains 2 elements, can be interpreted as a tuple,
+        and that both states lie inside the basis.
+
+        Parameters
+        ----------
+        states : iterable
+            iterable of to validate. Should be a pair of integers that can
+            be cast to a tuple.
+
+        Returns
+        -------
+        tuple
+            Length 2 tuple of validated state labels.
+
+        Raises
+        ------
+        ValueError
+            If `states` has more than two elements.
+        TypeError
+            If `states` cannot be converted to a tuple.
+        ValueError
+            If either state in `states` is outside the basis.
+        """
+        try:
+            tpl = tuple(states)
+        except TypeError:
+            raise ValueError(f'states argument of type {type(states)} cannot be interpreted as a tuple')
+        if len(tpl) != 2:
+            raise ValueError(f'A field must couple exactly 2 states, but {len(tpl)} are specified in {states}')
+        for i in tpl:
+            if not isinstance(i, int):
+                raise TypeError(f'State specifications must be an integer')
+            if i >= self.basis_size:
+                raise ValueError((f'State specification {i} is outside '
+                                  f'the basis size {self.basis_size:d}'))
+
+        return tpl
+
+
+    def _stack_shape(self, collapse=True, time_dependence="all") -> Tuple[int, ...]:
+        """
+        Internal function to get the shape of the tuple preceding the two hamiltonian
+        axes in :meth:`~.get_hamiltonian()`
+
+        """
+        # generate the uncollapsed stack
+        stack_shape = []
+
+        #case where we ignore time dependence in the stack shape
+        if time_dependence == 'all':
+            for _, _, arr in self.variable_parameters():
+                stack_shape.append(len(np.squeeze(arr)))
+
+        #case where we only want time-dependant stack shape
+        elif time_dependence == "time":
+            time_couplings = self.couplings_with("time_dependence")
+            for states, param, arr in self.variable_parameters():
+                if states in time_couplings and param == "rabi_frequency":
+                    stack_shape.append(len(np.squeeze(arr)))
+                else:
+                    stack_shape.append(1)
+
+        #case where we only want non-time-dependant stack shape
+        elif time_dependence == "steady":
+            time_couplings = self.couplings_with("time_dependence")
+            for states, param, arr in self.variable_parameters():
+                if states not in time_couplings or param != "rabi_frequency":
+                    stack_shape.append(len(np.squeeze(arr)))
+                else:
+                    stack_shape.append(1)
+        
+        else:
+            raise ValueError("time_dependence must be one of \"time\", \"steady\", or \"all\"")
+
+
+        # if collapsing, figure out the einsum logic
+        if collapse and len(self._zipped_parameters) > 0:
+            # list logic direct lifted from Sensor.collapse_dims()
+            axis_labels = self.axis_labels(collapse=False)
+            
+            paired_axes = []
+            for couplings in self._zipped_parameters:
+                paired_axes.append([axis_labels.index(c) for c in couplings])
+                
+            col_str = _get_collapse_str(len(axis_labels), *paired_axes)
+            
+            # this logic adapted from
+            # https://stackoverflow.com/questions/58380445/output-shape-of-numpy-einsum
+            insubs, outsubs = col_str.replace('.','').split('->')
+            insubs_array = np.array(list(insubs))
+            outshape = []
+            for o in outsubs:
+                indices, = np.where(insubs_array == o)
+                outshape.append(max([stack_shape[idx] for idx in indices]))
+                
+            stack_shape = tuple(outshape)
+
+        return stack_shape
+
+
+    def basis(self) -> np.ndarray:
+        """
+        Generate basis labels of density matrix components. 
+        
+        The basis corresponds to the elements in the solution.
+        This is not the complex basis of the sensor class, but rather the real basis
+        of a solution after calling one of `rydiqule`'s solvers. This means that the
+        ground state population has been removed and it has been transformed to the real basis.
+
+        Returns
+        -------
+        numpy.ndarray
+            Array of string labels corresponding to the solving basis.
+            Is a 1-D array of length `n**2-1`.
+
+        Examples
+        --------
+        >>> s = rq.Sensor(3)
+        >>> print(s.basis())
+        ['01_real' '02_real' '01_imag' '11_real' '12_real' '02_imag' '12_imag'
+        '22_real']
+
+        """
+        basis = [f'{j:d}{i:d}_imag' if i > j else f'{i:d}{j:d}_real'
+                 for i in range(self.basis_size)
+                 for j in range(self.basis_size)][1:]  # indexing removes ground state label
+        return np.array(basis)
+
+
+    def _remove_edge_data(self, states: States, kind: str):
+        """
+        Helper function to remove all data that was added with a :meth:`~.Sensor.add_coupling`
+        call or :meth:`~.Sensor.add_decoherence` call.
+        Needed to ensure that two nodes do not have coherent couplings pointing both ways
+        and to invalidate existing zip parameter couplings.
+
+        Parameters
+        ----------
+        states : tuple
+            Edge from which to remove data.
+        kind : str
+            What type of data to remove. Valid options are `coherent` coherent couplings
+            or the incoherent key to be cleared (must start with `gamma`).
+
+        Raises
+        ------
+        ValueError
+            If `kind` is not `'coherent'` and doesn't begin with `'gamma'`
+        """
+
+        if states not in self.couplings.edges:
+            return
+
+        if kind != 'coherent' and not kind.startswith('gamma'):
+            msg = 'If clearing incoherent data, must provide key to clear that starts with `gamma`, not {}'
+            raise ValueError(msg.format(kind))
+
+        #get rid of zipped couplings containing
+        label = self.couplings.edges[states]["label"]
+        zipped_idxs = []
+        for idx, zip_strs in enumerate(self._zipped_parameters):
+            zip_labels = [l.split("_",1)[0] for l in zip_strs]
+            if label in zip_labels:
+                zipped_idxs.append(idx)
+
+        for idx in zipped_idxs[::-1]:
+            del self._zipped_parameters[idx]
+        
+        # delete undesired keys from the edge
+        for key in list(self.couplings.edges[states]):  # prevent generator
+            if key == 'label':
+                pass
+            elif kind == 'coherent' and not key.startswith('gamma'):
+                del self.couplings.edges[states][key]
+            elif kind == key:
+                del self.couplings.edges[states][key]
+                
+        # delete edge outright if it only has a label
+        if not sum(k != 'label' for k in self.couplings.edges[states].keys()):
+            self.couplings.remove_edge(*states)
+
+
+    def _coupling_with_label(self, label: str) -> dict:
+        """
+        Helper function to return the pair of states corresponding to a particular label string.
+        For internal use.
+        """
+        label_map = {key:(state1, state2) for state1, state2, key in self.couplings.edges(data="label")}
+        if label in label_map.keys():
+            return label_map[label]
+        else:
+            raise ValueError(f"No coupling with label {label}")
```

### Comparing `rydiqule-1.0.0/src/rydiqule/sensor_solution.py` & `rydiqule-1.0.0rc2/src/rydiqule/sensor_solution.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-"""
-Bunch-like object use to store aspects of a solution when calling rydiule.solve()
-Adds essential keys with "None" entries
-"""
-from __future__ import annotations
-from typing import Optional
-
-import copy
-
-import numpy as np
-
-# have to import this way to prevent circular imports
-from rydiqule import sensor_utils
-
-
-class Solution(dict):
-    """
-    Manual implementation of a bunch object which fuctions as a dictionary with
-    the ability to access elements.
-
-    For now, little additional funcitonality exists
-    on top of this, but some may be added in the future.
-    """
-    # common attributes
-    rho: np.ndarray
-    """numpy.ndarray : Solutions returned by the solver."""
-    eta: Optional[float]
-    """float, optional : Eta constant from the Cell.
-    Not generally defined when using a Sensor."""
-    kappa: Optional[float]
-    """float, optional : Kappa constant from the Cell.
-    Not generally defined when using a Sensor."""
-    couplings: dict
-    """dict : Dictionary of the couplings."""
-    axis_labels: list[str]
-    """list of str : Labels for the axes of scanned parameters.
-    If doppler averaging but not summing, doppler dimensions are prepended."""
-    axis_values: list
-    """list : Value arrays corresponding to each axis.
-    If doppler averaging but not summing, doppler classes in internal units are added."""
-    rq_version: str
-    """str : Version of rydiqule that created the Solution."""
-    basis: list[str]
-    """list of str: The list of density matrix elements in the order they appear in the solution.
-    See :meth:`Sensor.basis` for details."""
-
-    # doppler specific
-    doppler_classes: Optional[np.ndarray]
-    """numpy.ndarray, optional : Doppler classes used to perform the doppler average.
-    Will be None if doppler averaging was not used."""
-
-    # time_solver specific
-    t: np.ndarray
-    """numpy.ndarray : Times the solution is returned at, when using the time solver.
-    Undefined otherwise."""
-    init_cond: np.ndarray
-    """numpy.ndarray : Initial conditions, when using the time solver.
-    Undefined otherwise."""
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.__dict__ = self
-
-    def rho_ij(self, i: int, j: int) -> np.ndarray:
-        """
-        Gets the i,j element(s) of the density matrix solutions.
-
-        See :func:`~.get_rho_ij` for details.
-
-        Parameters
-        ----------
-        i: int
-            density matrix element `i`
-        j: int
-            density matrix element `j`
-
-        Returns
-        -------
-        numpy.ndarray
-            `[i,j]` elments of the density matrix
-        """
-
-        return sensor_utils.get_rho_ij(self.rho, i, j)
-
-    def copy(self):
-        return copy.copy(self)
-    
-    def deepcopy(self):
+"""
+Bunch-like object use to store aspects of a solution when calling rydiule.solve()
+Adds essential keys with "None" entries
+"""
+from __future__ import annotations
+from typing import Optional
+
+import copy
+
+import numpy as np
+
+# have to import this way to prevent circular imports
+from rydiqule import sensor_utils
+
+
+class Solution(dict):
+    """
+    Manual implementation of a bunch object which fuctions as a dictionary with
+    the ability to access elements.
+
+    For now, little additional funcitonality exists
+    on top of this, but some may be added in the future.
+    """
+    # common attributes
+    rho: np.ndarray
+    """numpy.ndarray : Solutions returned by the solver."""
+    eta: Optional[float]
+    """float, optional : Eta constant from the Cell.
+    Not generally defined when using a Sensor."""
+    kappa: Optional[float]
+    """float, optional : Kappa constant from the Cell.
+    Not generally defined when using a Sensor."""
+    couplings: dict
+    """dict : Dictionary of the couplings."""
+    axis_labels: list[str]
+    """list of str : Labels for the axes of scanned parameters.
+    If doppler averaging but not summing, doppler dimensions are prepended."""
+    axis_values: list
+    """list : Value arrays corresponding to each axis.
+    If doppler averaging but not summing, doppler classes in internal units are added."""
+    rq_version: str
+    """str : Version of rydiqule that created the Solution."""
+    basis: list[str]
+    """list of str: The list of density matrix elements in the order they appear in the solution.
+    See :meth:`Sensor.basis` for details."""
+
+    # doppler specific
+    doppler_classes: Optional[np.ndarray]
+    """numpy.ndarray, optional : Doppler classes used to perform the doppler average.
+    Will be None if doppler averaging was not used."""
+
+    # time_solver specific
+    t: np.ndarray
+    """numpy.ndarray : Times the solution is returned at, when using the time solver.
+    Undefined otherwise."""
+    init_cond: np.ndarray
+    """numpy.ndarray : Initial conditions, when using the time solver.
+    Undefined otherwise."""
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.__dict__ = self
+
+    def rho_ij(self, i: int, j: int) -> np.ndarray:
+        """
+        Gets the i,j element(s) of the density matrix solutions.
+
+        See :func:`~.get_rho_ij` for details.
+
+        Parameters
+        ----------
+        i: int
+            density matrix element `i`
+        j: int
+            density matrix element `j`
+
+        Returns
+        -------
+        numpy.ndarray
+            `[i,j]` elments of the density matrix
+        """
+
+        return sensor_utils.get_rho_ij(self.rho, i, j)
+
+    def copy(self):
+        return copy.copy(self)
+    
+    def deepcopy(self):
         return copy.deepcopy(self)
```

### Comparing `rydiqule-1.0.0/src/rydiqule/sensor_utils.py` & `rydiqule-1.0.0rc2/src/rydiqule/sensor_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,736 +1,728 @@
-"""
-Utilities used by the Sensor classes.
-"""
-import string
-import math
-
-import numpy as np
-from .energy_diagram import ED
-from .sensor_solution import Solution
-import scipy.constants
-from scipy.constants import hbar, c, e, epsilon_0
-
-from typing import Dict, Tuple, Union, TYPE_CHECKING
-if TYPE_CHECKING:
-    # only import when type checking, avoid circular import
-    from .sensor import Sensor
-
-a0 = scipy.constants.physical_constants["Bohr radius"][0]
-
-RHO: Dict[int, np.ndarray] = {}
-U: Dict[int, np.ndarray] = {}
-B: Dict[int, int] = {}
-
-
-def generate_eom(hamiltonian: np.ndarray, gamma_matrix: np.ndarray,
-                 remove_ground_state: bool = True,
-                 real_eom: bool = True) -> Tuple[np.ndarray, np.ndarray]:
-    """
-    Create the optical bloch equations for a hamiltonian and decoherence matrix
-    using the Lindblad master equation.
-
-    Parameters
-    ----------
-    hamiltonian : numpy.ndarray
-        Complex array representing the Hamiltonian matrix
-        of the system, the matrix should be of shape `(*l, n, n)`, where n is
-        the basis size and l is the shape of the stack of hamiltonians. For
-        example, if the hamiltonian varies in 2 parameters l might be `(10, 10)`.
-    gamma_matrix : numpy.ndarray
-        Complex array representing the decoherence matrix
-        of the system, the matrix should be of size `(n, n)`, where n is the basis size.
-    remove_ground_state : bool, optional
-        Remove the ground state from the equations
-        of motion using population conservation. Setting to `False` is intended
-        for internal use only and is not officially supported.
-        See :func:`~.remove_ground` for details.
-    real_eom : bool, optional
-        Transform the equations of motion from the complex basis
-        to the real basis. Setting to `False` is intended for internal use only
-        and is not officially supported
-        Seee :func:`~.make_real` for details.
-
-    Returns
-    -------
-    equations : numpy.ndarray
-        The array representing the Optical
-        Bloch Equations (OBEs) of the system. The shape will be `(*l, n^2-1, n^2-1)`
-        if `remove_ground_state` is `True` and `(*l, n^2, n^2)` otherwise. The
-        datatype will be `np.float64` if `real_eom` is `True` and `np.complex128`
-        otherwise.
-    const : numpy.ndarray
-        Array of which defines the constant
-        term in the linear OBEs. The shape will be `(*l, n^2-1)` if
-        `remove_ground_state` is `True` and `(*l, n^2)` otherwise. The
-        datatype will be `np.float64` if `real_eom` is `True` and `np.complex128`
-        otherwise.
-
-    Raises
-    ------
-    ValueError: If the shapes of gamma_matrix and hamiltonian are not matching
-        or not square in the last 2 dimensions
-
-    Examples
-    --------
-    >>> ham = np.diag([1,-1])
-    >>> gamma = np.array([[.1, 0],[.1,0]])
-    >>> print(ham.shape)
-    >>> eom, const = rq.generate_eom(ham, gamma)
-    >>> print(eom)
-    >>> print(const.shape)
-    (2, 2)
-    [[-0.1  2.   0. ]
-     [-2.  -0.1  0. ]
-     [ 0.   0.  -0.1]]
-    (3,)
-
-    This also works with a "stack" of multiple hamiltonians:
-
-    >>> ham_base = np.diag([1,-1])
-    >>> ham_full = np.array([ham_base for _ in range(10)])
-    >>> gamma = np.array([[.1, 0],[.1,0]])
-    >>> print(ham_full.shape)
-    >>> eom, const = rq.generate_eom(ham_full, gamma)
-    >>> print(eom.shape)
-    >>> print(const.shape)
-    (10, 2, 2)
-    (10, 3, 3)
-    (10, 3)
-
-    """
-    if not hamiltonian.shape[-2:] == gamma_matrix.shape[-2:]:
-        raise ValueError("hamiltonian and gamma matrix must have matching shape")
-    if not hamiltonian.shape[-1] == hamiltonian.shape[-2]:
-        raise ValueError("hamiltonian and gamma matrix must be square")
-
-    basis_size = hamiltonian.shape[-1]
-    basis = np.array([[[m,n] for m in range(basis_size)] for n in range(basis_size)])
-    basis = basis.reshape((basis_size)**2,2)
-
-    # create optical bloch equations
-    obes = _hamiltonian_term(hamiltonian) + _decoherence_term(gamma_matrix)
-    stack_shape = obes.shape[:-2]
-    const_shape = (*tuple(np.ones_like(stack_shape)), basis_size**2)
-    const = np.zeros(const_shape)
-
-    if remove_ground_state:
-        obes, const = remove_ground(obes)
-
-    # transform to real basis
-    if real_eom:
-        obes, const = make_real(obes, const)
-
-    return obes, const
-
-
-def _hamiltonian_term(ham: np.ndarray) -> np.ndarray:
-    """
-    Helper function to calculate the first term of the Lindblad master equation.
-
-    Parameters
-    ----------
-    ham : numpy.ndarray
-        Complex Hamiltonian of shape `(*l, n, n)`
-        the describes the couplings between states and detunings.
-
-    Returns
-    -------
-    numpy.ndarray
-        Coherent Hamiltonian portion of the EOMs of shape `(*l, n^2, n^2)`
-        of dtype np.complex128
-
-    """
-    n: int = ham.shape[-1]
-    stack_shape = ham.shape[:-2]
-    ham = ham.reshape(stack_shape+(1,1,n,n))
-    rho = _get_rho(n)
-
-    term: np.ndarray = -1j*((ham @ rho) - (rho @ ham))
-
-    return term.reshape(stack_shape+(n*n, n*n))
-
-
-def _decoherence_term(gamma: np.ndarray) -> np.ndarray:
-    """
-    Helper function to determine the second term of the Lindblad master equation.
-
-    Parameters
-    ----------
-    gamma : numpy.ndarray
-        Square decoherence matrix of shape `(*l, n, n)`
-
-    Returns
-    -------
-    numpy.ndarray
-        The decoherence portion of the EOMs of shape `(*l, n^2, n^2)`.
-
-    """
-    n = gamma.shape[-1]
-    rho = _get_rho(n)
-    stack_shape = gamma.shape[:-2]
-    gamma_exp = gamma.reshape(stack_shape+(1,1,n,n))
-    g = gamma.sum(axis=-1).reshape(stack_shape+(1,1,1,n)) * rho
-
-    # equivalent to g_T = np.einsum('...ijkl->...lkji', g)
-    g_axes = np.arange(len(g.shape))
-    gT_axes = np.concatenate([g_axes[:-4], g_axes[-4:][::-1]])
-    g_T = np.transpose(g, axes=gT_axes)
-
-    term: np.ndarray = np.swapaxes((rho @ gamma_exp @ rho), -2, -3) - (g_T + g)/2
-    return term.reshape(stack_shape+(n*n, n*n))
-
-
-def remove_ground(equations: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
-    """
-    Remove the ground state from the equations of motion using population conservation.
-
-    Population conservation enforces
-
-    .. math:: \\rho_{(0,0)} = 1 - \\sum_{i=1}^{n-1} \\rho_{(i,i)}
-
-    We use this equation to remove the EOM for rho_00 and
-    enforce population conservation in the steady state.
-
-    Parameters
-    ----------
-    equations : numpy.ndarray
-        array of shape (n^2, n^2) representing the equations
-        of motion of the system, where n is the number of basis states.
-
-    Returns
-    -------
-    numpy.ndarray
-        The modified equations of shape (n^2-1, n^2-1)
-
-    """
-    if equations.shape[-1] != math.isqrt(equations.shape[-1])**2:
-        # full equations shape should be perfect square
-        raise ValueError("Ground state already removed")
-
-    basis_size = int(np.sqrt(equations.shape[-1]))
-    eqn_size = equations.shape[-1]
-
-    # get the constant term
-    eqns_column1 = equations[...,0]
-    constant_term = equations[...,1:,0]
-
-    # find the indices where populations need to be subtracted
-    plocations = np.array([(basis_size+1)*x for x in range(basis_size)])
-    pvector = np.array([int(i in plocations) for i in range(eqn_size)])
-
-    # make a matrix to subtract populations
-    pop_subtract = np.einsum('...i,j', eqns_column1, pvector)
-
-    # subtract populations
-    equation_new = equations - pop_subtract
-
-    # remove the ground state
-    equations_reduced = equation_new[..., 1:, 1:]
-
-    return equations_reduced, constant_term
-
-
-def make_real(equations: np.ndarray, constant: np.ndarray,
-              ground_removed: bool = True) -> Tuple[np.ndarray, np.ndarray]:
-    """
-    Converts equations of motion from complex basis to real basis.
-
-    Changes the density vector equation for p_ij into the Re[p_ij] equation
-    and changing the density vector equation for p_ji into the equation for Im[p_ij].
-
-    Parameters
-    ----------
-    equations : numpy.ndarray
-        Complex equations of motion.
-    constant : numpy.ndarray
-        RHS of the equations of motion.
-    ground_removed : bool, optional
-        Indicates if `equations` has had the ground state removed.
-        Default is `True`.
-
-    Returns
-    -------
-    real_eqns : numpy.ndarray
-        EOMs in real basis.
-    real_const : numpy.ndarray
-        RHS of EOMs in real basis.
-
-    """
-    # Define the basis for printout purposes for ground removed or not removed
-    if np.sqrt(equations.shape[-1]) % 1 == 0:  # ground is not removed
-
-        basis_size = int(np.sqrt(equations.shape[-1]))
-
-    elif np.sqrt(equations.shape[-1]+1) % 1 == 0:  # ground is removed
-
-        basis_size = int(np.sqrt(equations.shape[-1]+1))
-
-    else:
-        raise ValueError("unsupported equation shape")
-
-    u, u_inv = get_basis_transform(basis_size)  # unitary transformation matrix
-
-    if ground_removed:
-        u = u[1:,1:]
-        u_inv = u_inv[1:,1:]
-
-    # transform to the real basis
-    new_eqns = u@(equations@u_inv)
-    new_const = 0
-
-    if ground_removed:
-        new_const = np.einsum('ij,...j', u, constant)
-
-    # copies allow complex base arrays to be GC
-    return new_eqns.real.copy(), new_const.real.copy()
-
-
-def get_basis_transform(basis_size: int) -> Tuple[np.ndarray, np.ndarray]:
-    """
-    Function that defines the basis transformation matrix u and its inverse u_i,
-    between the real and complex basis.
-
-    This matrix u implements that the :math:`\\rho[j,i] \\rightarrow Re(\\rho[j,i])`
-    and :math:`\\rho[i,j] \\rightarrow Im(\\rho[j,i])`.
-
-    The transformation is not quite unitary, due to the asymmetry of the factors of 1/2.
-
-    Parameters
-    ----------
-    basis_size : int
-        Size of the basis to generate transformations for.
-
-    Returns
-    -------
-    u : numpy.ndarray
-        Forward transformation matrix.
-    u_inv : numpy.ndarray
-        Inverse transformation matrix.
-
-    Raises
-    ------
-    ValueError
-        If `basis_size` does not match current basis.
-
-    """
-    try:
-        u = U[0]
-        u_inv = U[1]
-        basis = B[0]
-        if basis != basis_size:
-            raise ValueError("new basis size")
-        return u, u_inv
-
-    except (KeyError, ValueError):
-        eqn_size = basis_size**2
-        u = np.zeros((eqn_size, eqn_size), dtype=complex)
-        u_inv = np.zeros((eqn_size, eqn_size), dtype=complex)
-        ipairs = np.array([[i for i in range(basis_size)] for j in range(basis_size)]).flatten()
-        jpairs = np.array([[j for i in range(basis_size)] for j in range(basis_size)]).flatten()
-        index = np.array(range(eqn_size))
-
-        for i,j,a in zip(ipairs,jpairs, index):
-            for k,l,b in zip(ipairs, jpairs, index):
-
-                # population equations dont change
-                if i == j and j == k and k == l:
-                    u[a,b] = 1
-                    u_inv[a,b] = 1
-                # define the  2x2 transformation between real and imaginary
-                elif i == k and j == l and i > j:
-                    u[a,b] = 1/2
-                    u_inv[a,b] = 1
-                elif i == k and j == l and i < j:
-                    u[a,b] = 1j/2
-                    u_inv[a,b] = -1j
-                elif i == l and j == k and i > j:
-                    u[a,b] = 1/2
-                    u_inv[a,b] = 1j
-                elif i == l and j == k and i < j:
-                    u[a,b] = -1j/2
-                    u_inv[a,b] = 1
-
-        U[0] = u
-        U[1] = u_inv
-        B[0] = basis_size
-        return u, u_inv
-
-
-def _get_rho(n: int) -> np.ndarray:
-    """
-    Helper function which gets the projectors for calculating the EOMs.
-
-    Uses a gobal dictionary to cache results and avoid recalculating.
-
-    Parameters
-    ----------
-    n : int
-        Basis size to get projectors for.
-
-    Returns
-    -------
-    numpy.ndarray
-        Projector matrices for the basis.
-
-    """
-    try:
-        return RHO[n]
-    except KeyError:
-        rho = np.zeros((n,n,n,n))
-        for i in range(n):
-            for k in range(n):
-                rho[i,k,i,k] = 1
-
-        RHO[n] = rho
-        return rho
-
-
-def get_rho_ij(sols: Union[np.ndarray, Solution], i: int, j: int) -> np.ndarray:
-    """
-    For a given density matrix solution, retrieve a specific element of the density matrix.
-
-    Assumes the ground state of the solution is eliminated (as per :func:`~.remove_ground`),
-    and assumes Rydiqule's nominal state ordering of the Density Vector (per :func:`~.make_real`).
-
-    Parameters
-    ----------
-    sols : numpy.ndarray or :class:`~.Solution`
-        Solutions to extract the matrix element for.
-        Can be either the solution object returned by the solve or
-        an N-D array representing density vectors, with ground state removed,
-        and written in the totally real equations.
-    i : int
-        density matrix index i
-    j : int
-        density matrix index j
-
-    Returns
-    -------
-    numpy.ndarray
-        Array of rho_ij values.
-        Will be of type float when `i==j`.
-        Will be of type complex128 when `i!=j`.
-
-    Examples
-    --------
-    >>> sols = np.arange(180).reshape((4,5,3,3))
-    >>> print(sols.shape)
-    >>> rho_01 = rq.get_rho_ij(sols, 0,1)
-    >>> print(rho_01.shape)
-    >>> print(rho_01[0,0])
-    (4, 5, 3, 3)
-    (4, 5, 3)
-    [0.-1.j 3.-4.j 6.-7.j]
-
-    """
-    rhos = _validate_sols(sols)
-
-    b = int(np.sqrt(rhos.shape[-1]+1))  # basis size
-    if i == 0 and j == 0:
-        zero_state_pop = 1.0
-        for k in range(1,b):
-            zero_state_pop -= rhos[...,b*k+k-1]
-        return zero_state_pop
-
-    elif i == j:
-        return rhos[...,b*j+i-1]
-
-    elif i > j:
-        realpart = rhos[...,b*j+i-1]
-        imagpart = rhos[...,b*i+j-1]
-        return realpart + 1j*imagpart
-    else:
-        realpart = rhos[...,b*i+j-1]
-        imagpart = rhos[...,b*j+i-1]
-        return realpart - 1j*imagpart
-
-
-def get_rho_populations(sols: Union[np.ndarray, Solution]) -> np.ndarray:
-    """
-    For a given density matrix solution, return the diagonal populations.
-
-    Note that rydiqule's convention for removing the ground state forces population conservation,
-    ie the sum of these populations will be 1.
-
-    Parameters
-    ----------
-    sols: numpy.ndarray or :class:`~.Solution`
-        Solutions to extract the matrix element for.
-        Can be either the solution object returned by the solve or
-        an N-D array representing density vectors, with ground state removed,
-        and written in the totally real equations.
-
-    Returns
-    -------
-    numpy.ndarray
-        Populations of the density matrices.
-        Will have same shape as input solutions, with the last dimension
-        reduced to the basis size.
-    """
-
-    rhos = _validate_sols(sols)
-
-    b = int(np.sqrt(rhos.shape[-1]+1))  # basis size
-    nonzero_state_pops = rhos[...,b::b+1]
-    zero_state_pop = 1.0 - nonzero_state_pops.sum(axis=-1)
-
-    return np.concatenate((zero_state_pop[...,np.newaxis], nonzero_state_pops), axis=-1)
-
-
-def scale_dipole(dipole: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
-    """
-    Scale a dipole matrix from units of a0*e to Mrad/s when multiplied by a field in V/m.
-
-    Parameters
-    ----------
-    dipole : float or numpy.ndarray
-        Array of dipole moments in units of a0*e.
-        These are the default units used by ARC.
-
-    Returns
-    -------
-    numpy.ndarray
-        Scaled array in units of (Mrad/s)/(V/m)
-
-    """
-    scale_factor = (a0*e)/hbar*1e-6
-    dipole = dipole * scale_factor
-    return dipole
-
-
-def draw_diagram(sensor: "Sensor", include_dephasing: bool = True) -> ED:
-    """
-    Draw a matplotlib plot that shows the energy level diagram, couplings, and dephasing paths.
-
-    To show the plot, call `plt.show()`.
-    If in a jupyter notebook, this is handled automatically.
-
-    Diagram has horizontal lines for the energy levels (spacing not to scale).
-    Integer labels refer to the internal indexing for each state.
-    If sensor is of type :class:`~.Cell`, will also add text labels to each state of the
-    quantum numbers.
-
-    Solid arrows between states are couplings defined with a non-zero Rabi frequency.
-    Dashed arrows between states are couplings defined with a dipole moment.
-
-    Wiggly arrows between states denote a dephasing pathway.
-    Opacity represents strength of dephasing relative to the largest specified dephasing,
-    where fully opaque is the largest dephasing.
-
-    Parameters
-    ----------
-    sensor : :class:`~.Sensor`
-        Sensor object to diagram.
-    include_dephasing : bool, optional
-        Whether to plot dephasing paths. Default is `True`.
-
-    Returns
-    -------
-    :class:`~.ED`
-        Diagram handle
-
-    """
-    from .cell import Cell
-    diagram = ED()
-    if isinstance(sensor, Cell):
-        for index, state_info in enumerate(sensor.states_list()):
-            diagram.add_level(index, str(state_info))
-    else:
-        for i in range(0, sensor.basis_size):
-            diagram.add_level(i, '')
-
-
-    for item in sensor.couplings.edges:
-        #draw coherent couplings
-        if 'dipole_moment' in sensor.couplings.edges[item].keys():
-            linestyle = 'dashed'  # loosely dashdotted
-            diagram.add_arrow(*item, linestyle)
-
-        elif 'rabi_frequency' in sensor.couplings.edges[item].keys():
-            if np.all(sensor.couplings.edges[item].get('rabi_frequency')) != 0:
-                linestyle = 'solid'  # solid
-                diagram.add_arrow(*item, linestyle)
-
-    gamma_matrix = sensor.decoherence_matrix()
-    # we get the biggest possible decoherence value for each term
-    # by doing a max reduction along stack axes
-    stack_axes = tuple(np.arange(0,gamma_matrix.ndim-2))
-    gamma_matrix = gamma_matrix.max(axis=stack_axes)
-
-    if include_dephasing and gamma_matrix.any():
-        max_dephase = gamma_matrix.max()
-        min_dephase = gamma_matrix[gamma_matrix != 0.0].min()
-        if np.isclose(min_dephase, max_dephase):
-            # all non-zero dephasings are the same, prevent /0 error in normalization
-            min_dephase = max_dephase*1e-1
-        idxs = np.argwhere(gamma_matrix != 0.0)[::-1,:]  # reverse order so transits don't all align
-        for idx in idxs:
-            # ensure alpha doesn't get too small to not be seen
-            # also uses a log scale for the full range of non-zero dephasings
-            alph = 1-(0.95*np.log10(gamma_matrix[tuple(idx)]/max_dephase
-                                    )/np.log10(min_dephase/max_dephase))
-            ls = {'linestyle':'solid','alpha':alph}
-            diagram.add_wiggly_arrow(*idx,ls)  # type: ignore[call-arg]
-
-    fig, ax = diagram.plot(show_IDs=True)
-    return diagram
-
-
-def calc_kappa(probe_freq: float, probe_elem: float, density: float) -> float:
-    """
-    Calculate kappa according to Eq. 5 of
-    Meyer et. al. PRA 104, 043103 (2021)
-
-    Parameters
-    ----------
-    probe_freq: float
-        Frequency of the probing field, in Hz
-    probe_elem: float
-        Dipole moment of the probing transition, in units of a_0*e
-    density: float
-        Atomic density, in m^(-3)
-
-    Returns
-    -------
-    kappa: float
-        in units of MHz/m
-
-    """
-    kappa = 2.0*np.pi*(probe_freq *
-                       density *
-                       probe_elem**2 *
-                       a0**2 *
-                       e**2)/(2.0*c*epsilon_0*hbar*1.0E6)
-
-    return kappa
-
-
-def calc_eta(probe_freq: float, probe_elem: float, beam_area: float) -> float:
-    """
-    Calculate eta according to Eq. 7 of
-    Meyer et. al. PRA 104, 043103 (2021)
-
-    Parameters
-    ----------
-    probe_freq: float
-        Frequency of the probing field, in Hz
-    probe_elem: float
-        Dipole moment of the probing transition, in units of a_0*e
-    beam_area: float
-        Area of the probing field, in m^2
-
-    Returns
-    -------
-    eta: float
-        in units of sqrt(MHz)
-
-    """
-    eta = np.sqrt((2.0*np.pi *
-                   probe_freq *
-                   probe_elem**2 *
-                   a0**2 *
-                   e**2)/(2.0*c*epsilon_0*hbar*beam_area*1.0E6))
-
-    return eta
-
-
-def _get_collapse_str(len: int, *matched_dims) -> str:
-    """
-    Internal helper function to build the string argument of `numpy.einsum`
-    when dimensions are collapsed.
-
-    Creates a string of the appropriate number of ascii characters
-    (the first n for an n-dimensional stack).
-    Then swaps in new characters in the appropriate place to produce a string that can be passed
-    to `numpy`'s `einsum` function.
-    """
-    # left-hand side and right-hand side of equation in einstein summation convention
-    idxs_rhs = string.ascii_lowercase[:len]
-    idxs_lhs = string.ascii_lowercase[:len]
-
-    for i, dims in enumerate(matched_dims):
-        new_idx = string.ascii_lowercase[-(i+1)]
-
-        for d in dims:
-            old_idx = idxs_rhs[d]
-            idxs_rhs = idxs_rhs.replace(old_idx, new_idx)
-            idxs_lhs = idxs_lhs.replace(old_idx, "")
-
-        idxs_lhs += new_idx
-
-    full_expression = idxs_rhs + "...->" + idxs_lhs + "..."
-    return full_expression
-
-
-def _validate_sols(sols):
-    """Helper function to validate that solutions are of an appropriate type.
-    There are 3 outcomes:
-    
-      - `sols` is a np.ndarray, returns `sols`.
-      - `sols` is an object with a `rho` attribute that is a `numpy.ndarray`,
-        in which case returns `rho`.
-      - `sols` does not meet either of the above criteria, in which case raises an exception.
-
-    Parameters
-    ----------
-    sols : any
-        The value to validate, should be a np.ndarray or an object
-        (like a :class:`~.sensor_solution.Solution`)
-        with a `rho` attribute which is a numpy array.
-        
-    Raises
-    ------
-    ValueError:
-        If `sols` is not an array or object with a `rho` attribute that is an array.
-    """
-    if hasattr(sols, "rho"):
-        rho = sols.rho
-    else:
-        rho = sols
-        
-    if not isinstance(rho, np.ndarray):
-        raise TypeError(
-            "sols must be a numpy array or have an attribute \"rho\" which is a numpy array.")
-    
-    return rho
-    
-
-def _combine_parameter_labels(*labels: str) -> str:
-    """
-    Combine 2 or more parameter label strings into a single label.
-
-    Labels are grouped by parameter type (detuning, rabi_freq, etc),
-    separated by a |
-
-    """
-
-    return "|".join(labels)
-
-
-    ## LEAVING IN CASE WE WANT TO USE THIS
-
-    # new_label = []
-
-    # couplings = []
-    # params = []
-
-    # #get lists of all the coupling labels and param types
-    # for label in labels:
-    #     coupling, param = label.split("_", 1)
-    #     couplings.append(coupling)
-    #     params.append(param)
-
-    # #build the full label from the lists
-    # #under this convention, couplings will be grouped in the label
-    # #by parameter type, with parameter types separated by a pipe
-    # for p_base in params: #loop over parameter types, skipping those that have already been done
-    #     if (p_base + "|") in new_label:
-    #         continue
-
-    #     for c, p_test in zip(couplings, params): #for each parameter type, get all labels
-    #         if p_test == p_base:
-    #             new_label.append(c + "_")
-    #     new_label.append(p_base + "|") #add a pipe to separate parameter types
-
-    # #turn the full label array into a string, get rid of pipe on the end
-    # return "".join(new_label)[:-1]
+"""
+Utilities used by the Sensor classes.
+"""
+import string
+import math
+
+import numpy as np
+from .energy_diagram import ED
+from .sensor_solution import Solution
+import scipy.constants
+from scipy.constants import hbar, c, e, epsilon_0
+
+from typing import Dict, Tuple, Union, TYPE_CHECKING
+if TYPE_CHECKING:
+    # only import when type checking, avoid circular import
+    from .sensor import Sensor
+
+a0 = scipy.constants.physical_constants["Bohr radius"][0]
+
+RHO: Dict[int, np.ndarray] = {}
+U: Dict[int, np.ndarray] = {}
+B: Dict[int, int] = {}
+
+
+def generate_eom(hamiltonian: np.ndarray, gamma_matrix: np.ndarray,
+                 remove_ground_state: bool = True,
+                 real_eom: bool = True) -> Tuple[np.ndarray, np.ndarray]:
+    """
+    Create the optical bloch equations for a hamiltonian and decoherence matrix
+    using the Lindblad master equation.
+
+    Parameters
+    ----------
+    hamiltonian : numpy.ndarray
+        Complex array representing the Hamiltonian matrix
+        of the system, the matrix should be of shape `(*l, n, n)`, where n is
+        the basis size and l is the shape of the stack of hamiltonians. For
+        example, if the hamiltonian varies in 2 parameters l might be `(10, 10)`.
+    gamma_matrix : numpy.ndarray
+        Complex array representing the decoherence matrix
+        of the system, the matrix should be of size `(n, n)`, where n is the basis size.
+    remove_ground_state : bool, optional
+        Remove the ground state from the equations
+        of motion using population conservation. Setting to `False` is intended
+        for internal use only and is not officially supported.
+        See :func:`~.remove_ground` for details.
+    real_eom : bool, optional
+        Transform the equations of motion from the complex basis
+        to the real basis. Setting to `False` is intended for internal use only
+        and is not officially supported
+        Seee :func:`~.make_real` for details.
+
+    Returns
+    -------
+    equations : numpy.ndarray
+        The array representing the Optical
+        Bloch Equations (OBEs) of the system. The shape will be `(*l, n^2-1, n^2-1)`
+        if `remove_ground_state` is `True` and `(*l, n^2, n^2)` otherwise. The
+        datatype will be `np.float64` if `real_eom` is `True` and `np.complex128`
+        otherwise.
+    const : numpy.ndarray
+        Array of which defines the constant
+        term in the linear OBEs. The shape will be `(*l, n^2-1)` if
+        `remove_ground_state` is `True` and `(*l, n^2)` otherwise. The
+        datatype will be `np.float64` if `real_eom` is `True` and `np.complex128`
+        otherwise.
+
+    Raises
+    ------
+    ValueError: If the shapes of gamma_matrix and hamiltonian are not matching
+        or not square in the last 2 dimensions
+
+    Examples
+    --------
+    >>> ham = np.diag([1,-1])
+    >>> gamma = np.array([[.1, 0],[.1,0]])
+    >>> print(ham.shape)
+    >>> eom, const = rq.generate_eom(ham, gamma)
+    >>> print(eom)
+    >>> print(const.shape)
+    (2, 2)
+    [[-0.1  2.   0. ]
+     [-2.  -0.1  0. ]
+     [ 0.   0.  -0.1]]
+    (3,)
+
+    This also works with a "stack" of multiple hamiltonians:
+
+    >>> ham_base = np.diag([1,-1])
+    >>> ham_full = np.array([ham_base for _ in range(10)])
+    >>> gamma = np.array([[.1, 0],[.1,0]])
+    >>> print(ham_full.shape)
+    >>> eom, const = rq.generate_eom(ham_full, gamma)
+    >>> print(eom.shape)
+    >>> print(const.shape)
+    (10, 2, 2)
+    (10, 3, 3)
+    (10, 3)
+
+    """
+    if not hamiltonian.shape[-2:] == gamma_matrix.shape[-2:]:
+        raise ValueError("hamiltonian and gamma matrix must have matching shape")
+    if not hamiltonian.shape[-1] == hamiltonian.shape[-2]:
+        raise ValueError("hamiltonian and gamma matrix must be square")
+
+    basis_size = hamiltonian.shape[-1]
+    basis = np.array([[[m,n] for m in range(basis_size)] for n in range(basis_size)])
+    basis = basis.reshape((basis_size)**2,2)
+
+    # create optical bloch equations
+    obes = _hamiltonian_term(hamiltonian) + _decoherence_term(gamma_matrix)
+    stack_shape = obes.shape[:-2]
+    const_shape = (*tuple(np.ones_like(stack_shape)), basis_size**2)
+    const = np.zeros(const_shape)
+
+    if remove_ground_state:
+        obes, const = remove_ground(obes)
+
+    # transform to real basis
+    if real_eom:
+        obes, const = make_real(obes, const)
+
+    return obes, const
+
+
+def _hamiltonian_term(ham: np.ndarray) -> np.ndarray:
+    """
+    Helper function to calculate the first term of the Lindblad master equation.
+
+    Parameters
+    ----------
+    ham : numpy.ndarray
+        Complex Hamiltonian of shape `(*l, n, n)`
+        the describes the couplings between states and detunings.
+
+    Returns
+    -------
+    numpy.ndarray
+        Coherent Hamiltonian portion of the EOMs of shape `(*l, n^2, n^2)`
+        of dtype np.complex128
+
+    """
+    n: int = ham.shape[-1]
+    stack_shape = ham.shape[:-2]
+    ham = ham.reshape(stack_shape+(1,1,n,n))
+    rho = _get_rho(n)
+
+    term: np.ndarray = -1j*((ham @ rho) - (rho @ ham))
+
+    return term.reshape(stack_shape+(n*n, n*n))
+
+
+def _decoherence_term(gamma: np.ndarray) -> np.ndarray:
+    """
+    Helper function to determine the second term of the Lindblad master equation.
+
+    Parameters
+    ----------
+    gamma : numpy.ndarray
+        Square decoherence matrix of shape `(*l, n, n)`
+
+    Returns
+    -------
+    numpy.ndarray
+        The decoherence portion of the EOMs of shape `(*l, n^2, n^2)`.
+
+    """
+    n = gamma.shape[-1]
+    rho = _get_rho(n)
+    stack_shape = gamma.shape[:-2]
+    gamma_exp = gamma.reshape(stack_shape+(1,1,n,n))
+    g = gamma.sum(axis=-1).reshape(stack_shape+(1,1,1,n)) * rho
+
+    # equivalent to g_T = np.einsum('...ijkl->...lkji', g)
+    g_axes = np.arange(len(g.shape))
+    gT_axes = np.concatenate([g_axes[:-4], g_axes[-4:][::-1]])
+    g_T = np.transpose(g, axes=gT_axes)
+
+    term: np.ndarray = np.swapaxes((rho @ gamma_exp @ rho), -2, -3) - (g_T + g)/2
+    return term.reshape(stack_shape+(n*n, n*n))
+
+
+def remove_ground(equations: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
+    """
+    Remove the ground state from the equations of motion using population conservation.
+
+    Population conservation enforces
+
+    .. math:: \\rho_{(0,0)} = 1 - \\sum_{i=1}^{n-1} \\rho_{(i,i)}
+
+    We use this equation to remove the EOM for rho_00 and
+    enforce population conservation in the steady state.
+
+    Parameters
+    ----------
+    equations : numpy.ndarray
+        array of shape (n^2, n^2) representing the equations
+        of motion of the system, where n is the number of basis states.
+
+    Returns
+    -------
+    numpy.ndarray
+        The modified equations of shape (n^2-1, n^2-1)
+
+    """
+    if equations.shape[-1] != math.isqrt(equations.shape[-1])**2:
+        # full equations shape should be perfect square
+        raise ValueError("Ground state already removed")
+
+    basis_size = int(np.sqrt(equations.shape[-1]))
+    eqn_size = equations.shape[-1]
+
+    # get the constant term
+    eqns_column1 = equations[...,0]
+    constant_term = equations[...,1:,0]
+
+    # find the indices where populations need to be subtracted
+    plocations = np.array([(basis_size+1)*x for x in range(basis_size)])
+    pvector = np.array([int(i in plocations) for i in range(eqn_size)])
+
+    # make a matrix to subtract populations
+    pop_subtract = np.einsum('...i,j', eqns_column1, pvector)
+
+    # subtract populations
+    equation_new = equations - pop_subtract
+
+    # remove the ground state
+    equations_reduced = equation_new[..., 1:, 1:]
+
+    return equations_reduced, constant_term
+
+
+def make_real(equations: np.ndarray, constant: np.ndarray,
+              ground_removed: bool = True) -> Tuple[np.ndarray, np.ndarray]:
+    """
+    Converts equations of motion from complex basis to real basis.
+
+    Changes the density vector equation for p_ij into the Re[p_ij] equation
+    and changing the density vector equation for p_ji into the equation for Im[p_ij].
+
+    Parameters
+    ----------
+    equations : numpy.ndarray
+        Complex equations of motion.
+    constant : numpy.ndarray
+        RHS of the equations of motion.
+    ground_removed : bool, optional
+        Indicates if `equations` has had the ground state removed.
+        Default is `True`.
+
+    Returns
+    -------
+    real_eqns : numpy.ndarray
+        EOMs in real basis.
+    real_const : numpy.ndarray
+        RHS of EOMs in real basis.
+
+    """
+    # Define the basis for printout purposes for ground removed or not removed
+    if np.sqrt(equations.shape[-1]) % 1 == 0:  # ground is not removed
+
+        basis_size = int(np.sqrt(equations.shape[-1]))
+
+    elif np.sqrt(equations.shape[-1]+1) % 1 == 0:  # ground is removed
+
+        basis_size = int(np.sqrt(equations.shape[-1]+1))
+
+    else:
+        raise ValueError("unsupported equation shape")
+
+    u, u_inv = get_basis_transform(basis_size)  # unitary transformation matrix
+
+    if ground_removed:
+        u = u[1:,1:]
+        u_inv = u_inv[1:,1:]
+
+    # transform to the real basis
+    new_eqns = u@(equations@u_inv)
+    new_const = 0
+
+    if ground_removed:
+        new_const = np.einsum('ij,...j', u, constant)
+
+    # copies allow complex base arrays to be GC
+    return new_eqns.real.copy(), new_const.real.copy()
+
+
+def get_basis_transform(basis_size: int) -> Tuple[np.ndarray, np.ndarray]:
+    """
+    Function that defines the basis transformation matrix u and its inverse u_i,
+    between the real and complex basis.
+
+    This matrix u implements that the :math:`\\rho[j,i] \\rightarrow Re(\\rho[j,i])`
+    and :math:`\\rho[i,j] \\rightarrow Im(\\rho[j,i])`.
+
+    The transformation is not quite unitary, due to the asymmetry of the factors of 1/2.
+
+    Parameters
+    ----------
+    basis_size : int
+        Size of the basis to generate transformations for.
+
+    Returns
+    -------
+    u : numpy.ndarray
+        Forward transformation matrix.
+    u_inv : numpy.ndarray
+        Inverse transformation matrix.
+
+    Raises
+    ------
+    ValueError
+        If `basis_size` does not match current basis.
+
+    """
+    try:
+        u = U[0]
+        u_inv = U[1]
+        basis = B[0]
+        if basis != basis_size:
+            raise ValueError("new basis size")
+        return u, u_inv
+
+    except (KeyError, ValueError):
+        eqn_size = basis_size**2
+        u = np.zeros((eqn_size, eqn_size), dtype=complex)
+        u_inv = np.zeros((eqn_size, eqn_size), dtype=complex)
+        ipairs = np.array([[i for i in range(basis_size)] for j in range(basis_size)]).flatten()
+        jpairs = np.array([[j for i in range(basis_size)] for j in range(basis_size)]).flatten()
+        index = np.array(range(eqn_size))
+
+        for i,j,a in zip(ipairs,jpairs, index):
+            for k,l,b in zip(ipairs, jpairs, index):
+
+                # population equations dont change
+                if i == j and j == k and k == l:
+                    u[a,b] = 1
+                    u_inv[a,b] = 1
+                # define the  2x2 transformation between real and imaginary
+                elif i == k and j == l and i > j:
+                    u[a,b] = 1/2
+                    u_inv[a,b] = 1
+                elif i == k and j == l and i < j:
+                    u[a,b] = 1j/2
+                    u_inv[a,b] = -1j
+                elif i == l and j == k and i > j:
+                    u[a,b] = 1/2
+                    u_inv[a,b] = 1j
+                elif i == l and j == k and i < j:
+                    u[a,b] = -1j/2
+                    u_inv[a,b] = 1
+
+        U[0] = u
+        U[1] = u_inv
+        B[0] = basis_size
+        return u, u_inv
+
+
+def _get_rho(n: int) -> np.ndarray:
+    """
+    Helper function which gets the projectors for calculating the EOMs.
+
+    Uses a gobal dictionary to cache results and avoid recalculating.
+
+    Parameters
+    ----------
+    n : int
+        Basis size to get projectors for.
+
+    Returns
+    -------
+    numpy.ndarray
+        Projector matrices for the basis.
+
+    """
+    try:
+        return RHO[n]
+    except KeyError:
+        rho = np.zeros((n,n,n,n))
+        for i in range(n):
+            for k in range(n):
+                rho[i,k,i,k] = 1
+
+        RHO[n] = rho
+        return rho
+
+
+def get_rho_ij(sols: Union[np.ndarray, Solution], i: int, j: int) -> np.ndarray:
+    """
+    For a given density matrix solution, retrieve a specific element of the density matrix.
+
+    Assumes the ground state of the solution is eliminated (as per :func:`~.remove_ground`),
+    and assumes Rydiqule's nominal state ordering of the Density Vector (per :func:`~.make_real`).
+
+    Parameters
+    ----------
+    sols : numpy.ndarray or :class:`~.Solution`
+        Solutions to extract the matrix element for.
+        Can be either the solution object returned by the solve or
+        an N-D array representing density vectors, with ground state removed,
+        and written in the totally real equations.
+    i : int
+        density matrix index i
+    j : int
+        density matrix index j
+
+    Returns
+    -------
+    numpy.ndarray
+        Array of rho_ij values.
+        Will be of type float when `i==j`.
+        Will be of type complex128 when `i!=j`.
+
+    Examples
+    --------
+    >>> sols = np.arange(180).reshape((4,5,3,3))
+    >>> print(sols.shape)
+    >>> rho_01 = rq.get_rho_ij(sols, 0,1)
+    >>> print(rho_01.shape)
+    >>> print(rho_01[0,0])
+    (4, 5, 3, 3)
+    (4, 5, 3)
+    [0.-1.j 3.-4.j 6.-7.j]
+
+    """
+    rhos = _validate_sols(sols)
+
+    b = int(np.sqrt(rhos.shape[-1]+1))  # basis size
+    if i == 0 and j == 0:
+        zero_state_pop = 1.0
+        for k in range(1,b):
+            zero_state_pop -= rhos[...,b*k+k-1]
+        return zero_state_pop
+
+    elif i == j:
+        return rhos[...,b*j+i-1]
+
+    elif i > j:
+        realpart = rhos[...,b*j+i-1]
+        imagpart = rhos[...,b*i+j-1]
+        return realpart + 1j*imagpart
+    else:
+        realpart = rhos[...,b*i+j-1]
+        imagpart = rhos[...,b*j+i-1]
+        return realpart - 1j*imagpart
+
+
+def get_rho_populations(sols: Union[np.ndarray, Solution]) -> np.ndarray:
+    """
+    For a given density matrix solution, return the diagonal populations.
+
+    Note that rydiqule's convention for removing the ground state forces population conservation,
+    ie the sum of these populations will be 1.
+
+    Parameters
+    ----------
+    sols: numpy.ndarray or :class:`~.Solution`
+        Solutions to extract the matrix element for.
+        Can be either the solution object returned by the solve or
+        an N-D array representing density vectors, with ground state removed,
+        and written in the totally real equations.
+
+    Returns
+    -------
+    numpy.ndarray
+        Populations of the density matrices.
+        Will have same shape as input solutions, with the last dimension
+        reduced to the basis size.
+    """
+
+    rhos = _validate_sols(sols)
+
+    b = int(np.sqrt(rhos.shape[-1]+1))  # basis size
+    nonzero_state_pops = rhos[...,b::b+1]
+    zero_state_pop = 1.0 - nonzero_state_pops.sum(axis=-1)
+
+    return np.concatenate((zero_state_pop[...,np.newaxis], nonzero_state_pops), axis=-1)
+
+
+def scale_dipole(dipole: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
+    """
+    Scale a dipole matrix from units of a0*e to Mrad/s when multiplied by a field in V/m.
+
+    Parameters
+    ----------
+    dipole : float or numpy.ndarray
+        Array of dipole moments in units of a0*e.
+        These are the default units used by ARC.
+
+    Returns
+    -------
+    numpy.ndarray
+        Scaled array in units of (Mrad/s)/(V/m)
+
+    """
+    scale_factor = (a0*e)/hbar*1e-6
+    dipole = dipole * scale_factor
+    return dipole
+
+
+def draw_diagram(sensor: "Sensor", include_dephasing: bool = True) -> ED:
+    """
+    Draw a matplotlib plot that shows the energy level diagram, couplings, and dephasing paths.
+
+    To show the plot, call `plt.show()`.
+    If in a jupyter notebook, this is handled automatically.
+
+    Diagram has horizontal lines for the energy levels (spacing not to scale).
+    Integer labels refer to the internal indexing for each state.
+    If sensor is of type :class:`~.Cell`, will also add text labels to each state of the
+    quantum numbers.
+
+    Solid arrows between states are couplings defined with a non-zero Rabi frequency.
+    Dashed arrows between states are couplings defined with a dipole moment.
+
+    Wiggly arrows between states denote a dephasing pathway.
+    Opacity represents strength of dephasing relative to the largest specified dephasing,
+    where fully opaque is the largest dephasing.
+
+    Parameters
+    ----------
+    sensor : :class:`~.Sensor`
+        Sensor object to diagram.
+    include_dephasing : bool, optional
+        Whether to plot dephasing paths. Default is `True`.
+
+    Returns
+    -------
+    :class:`~.ED`
+        Diagram handle
+
+    """
+    from .cell import Cell
+    diagram = ED()
+    if isinstance(sensor, Cell):
+        for index, state_info in enumerate(sensor.states_list()):
+            diagram.add_level(index, str(state_info))
+    else:
+        for i in range(0, sensor.basis_size):
+            diagram.add_level(i, '')
+
+
+    for item in sensor.couplings.edges:
+        #draw coherent couplings
+        if 'dipole_moment' in sensor.couplings.edges[item].keys():
+            linestyle = 'dashed'  # loosely dashdotted
+            diagram.add_arrow(*item, linestyle)
+
+        elif 'rabi_frequency' in sensor.couplings.edges[item].keys():
+            if np.all(sensor.couplings.edges[item].get('rabi_frequency')) != 0:
+                linestyle = 'solid'  # solid
+                diagram.add_arrow(*item, linestyle)
+
+    gamma_matrix = sensor.decoherence_matrix()
+    #we get the biggest possible decoherence value for each term by doing a max reduction along stack axes
+    stack_axes = tuple(np.arange(0,gamma_matrix.ndim-2))
+    gamma_matrix = gamma_matrix.max(axis=stack_axes)
+
+    if include_dephasing and gamma_matrix.any():
+        max_dephase = gamma_matrix.max()
+        min_dephase = gamma_matrix[gamma_matrix != 0.0].min()
+        idxs = np.argwhere(gamma_matrix != 0.0)[::-1,:]  # reverse order so transits don't all align
+        for idx in idxs:
+            # ensure alpha doesn't get too small to not be seen
+            # also uses a log scale for the full range of non-zero dephasings
+            alph = 1-(0.95*np.log10(gamma_matrix[tuple(idx)]/max_dephase
+                                    )/np.log10(min_dephase/max_dephase))
+            ls = {'linestyle':'solid','alpha':alph}
+            diagram.add_wiggly_arrow(*idx,ls)  # type: ignore[call-arg]
+
+    fig, ax = diagram.plot(show_IDs=True)
+    return diagram
+
+
+def calc_kappa(probe_freq: float, probe_elem: float, density: float) -> float:
+    """
+    Calculate kappa according to Eq. 5 of
+    Meyer et. al. PRA 104, 043103 (2021)
+
+    Parameters
+    ----------
+    probe_freq: float
+        Frequency of the probing field, in Hz
+    probe_elem: float
+        Dipole moment of the probing transition, in units of a_0*e
+    density: float
+        Atomic density, in m^(-3)
+
+    Returns
+    -------
+    kappa: float
+        in units of MHz/m
+
+    """
+    kappa = 2.0*np.pi*(probe_freq *
+                       density *
+                       probe_elem**2 *
+                       a0**2 *
+                       e**2)/(2.0*c*epsilon_0*hbar*1.0E6)
+
+    return kappa
+
+
+def calc_eta(probe_freq: float, probe_elem: float, beam_area: float) -> float:
+    """
+    Calculate eta according to Eq. 7 of
+    Meyer et. al. PRA 104, 043103 (2021)
+
+    Parameters
+    ----------
+    probe_freq: float
+        Frequency of the probing field, in Hz
+    probe_elem: float
+        Dipole moment of the probing transition, in units of a_0*e
+    beam_area: float
+        Area of the probing field, in m^2
+
+    Returns
+    -------
+    eta: float
+        in units of sqrt(MHz)
+
+    """
+    eta = np.sqrt((2.0*np.pi *
+                   probe_freq *
+                   probe_elem**2 *
+                   a0**2 *
+                   e**2)/(2.0*c*epsilon_0*hbar*beam_area*1.0E6))
+
+    return eta
+
+
+def _get_collapse_str(len: int, *matched_dims) -> str:
+    """
+    Internal helper function to build the string argument of `numpy.einsum`
+    when dimensions are collapsed.
+
+    Creates a string of the appropriate number of ascii characters (the first n for an n-dimensional stack).
+    Then swaps in new characters in the appropriate place to produce a string that can be passed
+    to `numpy`'s `einsum` function.
+    """
+    # left-hand side and right-hand side of equation in einstein summation convention
+    idxs_rhs = string.ascii_lowercase[:len]
+    idxs_lhs = string.ascii_lowercase[:len]
+
+    for i, dims in enumerate(matched_dims):
+        new_idx = string.ascii_lowercase[-(i+1)]
+
+        for d in dims:
+            old_idx = idxs_rhs[d]
+            idxs_rhs = idxs_rhs.replace(old_idx, new_idx)
+            idxs_lhs = idxs_lhs.replace(old_idx, "")
+
+        idxs_lhs += new_idx
+
+    full_expression = idxs_rhs + "...->" + idxs_lhs + "..."
+    return full_expression
+
+
+def _validate_sols(sols):
+    """Helper function to validate that solutions are of an appropriate type.
+    There are 3 outcomes:
+    
+      - `sols` is a np.ndarray, returns `sols`.
+      - `sols` is an object with a `rho` attribute that is a `numpy.ndarray`, in which case returns `rho`.
+      - `sols` does not meet either of the above criteria, in which case raises an exception.
+
+    Parameters
+    ----------
+    sols : any
+        The value to validate, should be a np.ndarray or an object (like a :class:`~.sensor_solution.Solution`)
+        with a `rho` attribute which is a numpy array.
+        
+    Raises
+    ------
+    ValueError:
+        If `sols` is not an array or object with a `rho` attribute that is an array.
+    """
+    if hasattr(sols, "rho"):
+        rho = sols.rho
+    else:
+        rho = sols
+        
+    if not isinstance(rho, np.ndarray):
+        raise TypeError("sols must be a numpy array or have an attribute \"rho\" which is a numpy array.")
+    
+    return rho
+    
+
+def _combine_parameter_labels(*labels: str) -> str:
+    """
+    Combine 2 or more parameter label strings into a single label.
+
+    Labels are grouped by parameter type (detuning, rabi_freq, etc),
+    separated by a |
+
+    """
+
+    return "|".join(labels)
+
+
+    ## LEAVING IN CASE WE WANT TO USE THIS
+
+    # new_label = []
+
+    # couplings = []
+    # params = []
+
+    # #get lists of all the coupling labels and param types
+    # for label in labels:
+    #     coupling, param = label.split("_", 1)
+    #     couplings.append(coupling)
+    #     params.append(param)
+
+    # #build the full label from the lists
+    # #under this convention, couplings will be grouped in the label
+    # #by parameter type, with parameter types separated by a pipe
+    # for p_base in params: #loop over parameter types, skipping those that have already been done
+    #     if (p_base + "|") in new_label:
+    #         continue
+
+    #     for c, p_test in zip(couplings, params): #for each parameter type, get all labels
+    #         if p_test == p_base:
+    #             new_label.append(c + "_")
+    #     new_label.append(p_base + "|") #add a pipe to separate parameter types
+
+    # #turn the full label array into a string, get rid of pipe on the end
+    # return "".join(new_label)[:-1]
```

### Comparing `rydiqule-1.0.0/src/rydiqule/slicing/slicing.py` & `rydiqule-1.0.0rc2/src/rydiqule/slicing/slicing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,496 +1,484 @@
-"""
-A handful of tools that solvers use to interface with slicing matrix stacks
-"""
-
-import psutil
-import warnings
-import itertools
-
-import numpy as np
-
-from typing import Tuple, Iterator, Union, List
-
-
-def compute_grid(stack_shape: np.ndarray, n_slices: int):
-    """Calculate the bin edges to break a given stack shape into at least a certain number of pieces
-
-    Works by iterating first over a number of slices per axis (N=1,2,3),
-    then over each in the stack shape, splitting the axis into N slices,
-    and comparing the total number of slices to the number specified.
-    In a sense, the algorithm factors a number greater than or equal to n_slices,
-    then breaks the stack along each axis according to this factorization.
-    If the axis lengths do not break evenly into the appropriate number of pieces,
-    the bin edges are truncated to an integer.
-    This means that the slices are not guaranteed to be `(1/n_slices)`,
-    but they will be close enough for most cases. 
-
-    Parameters
-    ----------
-    stack_shape : np.ndarray
-        The shape of the stack to be sliced.
-        Does not include Hamiltonian or matrix equation dimensions,
-        so for a hamiltonain stack of shape `(*l,n,n)`, `stack_shape` will be `*l`.
-    n_slices : int
-        The number of slices into which to break the hamiltonian. Lower bound on the number of 
-        slices there will actually be.
-
-    Returns
-    -------
-    list(np.ndarray)
-        The list of bin edges axis by axis. Can be passed to :func:`matrix_slice` as the `edges` 
-        argument.
-        
-    Examples
-    --------
-    >>> stack_shape=(10,10)
-    >>> print(compute_grid(stack_shape, 4))
-    [array([ 0,  5, 10]), array([ 0,  5, 10])]
-    >>> print(compute_grid(stack_shape, 6))
-    [array([ 0,  3,  6, 10]), array([ 0,  5, 10])]
-    """
-    
-    if n_slices > np.prod(stack_shape):
-        raise ValueError(f"Too many slices ({n_slices}) for stack of shape {stack_shape}")
-    
-    n_ax_slices = np.ones_like(stack_shape)
-    
-    current_slices = 1
-    current_axis = 0
-    
-    while current_slices < n_slices:
-        n_ax_slices[current_axis]+= 1
-        current_slices = np.prod(n_ax_slices)
-        current_axis += 1
-        
-        if current_axis ==len(stack_shape):
-            current_axis=0
-    total_axes = sum([1 for a in n_ax_slices if a>1])
-    
-    return [np.linspace(0,stack_shape[i], n_ax_slices[i]+1, dtype=int) for i in range(total_axes)]
-
-
-def matrix_slice(*matrices: np.ndarray,
-                 edges:Union[List, None]=None,
-                 n_slices:Union[int, None]=None) -> Iterator[Tuple[tuple, np.ndarray]]:
-    """
-    Generator that returns parts of a stack of matrices.
-
-    Given a stack of n by n matrices, produces a genererator which returns the given matrices
-    in the specified number of smaller stacks. For example, given a stack of matrices of shape
-    `(10,10,4,4)` with 4 slices, generates 4 stacks of shape `(5,4,4)`. Due to the nature
-    of the slicing, the number of slices might be slightly greater that the number specified.
-    Output matrices will be broadcastable by numpy's broadcasting rules.
-    Input arrays are interpreted as a stack, with the last 2 dimensions staying intact.
-
-    Args
-    ----
-    matrices: np.ndarray 
-        matrix stacks to be sliced. All matrices must be of shapes that can be
-        broadcast by numpy's broadcasting rules, with the additional restriction that all matrices
-        must have the same number of dimensions, even if some dimensions are of size 1. For example,
-        matrices of sizes `(10,1,4,4)` and `(1,20,4,4)` can be sliced together. 
-    edges: list(iterable)
-        The values along each axis that define the edges of bins on an n-dimensional grid.
-        For example, to slice a grid of hamiltonians with stack_shape `(10,10)` into 4 pieces,
-        `edges` could be defined as `[0,5,10]` for each of the 2 stack axes. 
-    n_slices : int or None 
-        The number of slices into which to break the matrix stack. Ignored if the
-        `edges` parameter is not `None`. Must be specified as an integer value if `edges` is `None`,
-        ignored otherwise. Defaults to None. 
-
-    Yields
-    ------
-    numpy.ndarray
-        Slice of hamiltonian stack
-        
-    Examples
-    --------
-    >>> import numpy as np
-    >>> import rydiqule as rq
-
-    >>> M1 = np.ones((1,20,4,4))
-    >>> M2 = np.ones((20,1,4,4))
-    >>> M3 = np.ones((20,20,4,4))
-    
-    >>> axis0_edges = np.array([0,10,20])
-    >>> axis1_edges = np.array([0,10,20])
-    
-    >>> for idx,m1,m2, m3 in rq.matrix_slice(M1, M2, M3, edges=[axis0_edges, axis1_edges]):
-    >>>     print(m1.shape, m2.shape, m3.shape)
-    
-    (1, 10, 4, 4) (10, 1, 4, 4) (10, 10, 4, 4)
-    (1, 10, 4, 4) (10, 1, 4, 4) (10, 10, 4, 4)
-    (1, 10, 4, 4) (10, 1, 4, 4) (10, 10, 4, 4)
-    (1, 10, 4, 4) (10, 1, 4, 4) (10, 10, 4, 4)
-    """
-    #catch input shape errors and raise more useful errors
-    shapes = [m.shape for m in matrices]
-    if len(matrices) == 0:
-        raise ValueError("Must provide at least 1 matrix for slicing")
-    if matrices[0].ndim < 2:
-        raise ValueError("Must have at least 2d matrices to slice")
-
-    try:
-        stack_shape = np.broadcast_shapes(*shapes)[:-2]
-    except ValueError:
-        raise ValueError(f"Incompatiple input shapes {shapes}")
-    
-    # handle the trivial case of a single hamiltonian
-    if len(stack_shape) == 0:
-        yield (), *matrices
-        return
-    #Build the grid if only the number of slices is specified. 
-    if edges is None:
-        if n_slices in (1,None):
-            yield (), *matrices
-            return
-        elif n_slices>1:
-            edges = compute_grid(stack_shape, n_slices)
-
-    #check that the bins slice each axis appropriately
-    for i,e in enumerate(edges):
-        if e[0] != 0 or e[-1] != stack_shape[i]:
-            raise ValueError(
-                f"slices must start at 0 and end at the axis length ({stack_shape[i]} for axis {i})"
-                )
-
-    start_edges = [e[:-1] for e in edges] # "left" edge
-    end_edges = [e[1:] for e in edges] #"right" edge
-
-    #loop over each box, defined by 2 opposite corners p_start and p_end. 
-    #eg consider the 3-box from (4,4,4) to (6,6,6)
-    #in this case p_start will be (4,4,4) and p_end will be (6,6,6)
-    for p_start, p_end in zip(itertools.product(*start_edges), itertools.product(*end_edges)):
-
-        #loop over dimensions for each box and get the box bounds as slices
-        slices = []
-        for i in range(len(p_start)):
-            slices.append(slice(p_start[i], p_end[i]))
-        slices = tuple(slices)
-        
-        m_idx = [] #actual matrix indeces, accounting for broadcasting support
-        for m in matrices:
-            m_idx.append(tuple(idx
-                if m.shape[j] !=1
-                else slice(0,None)
-                for j, idx in enumerate(slices)
-            ))
-        
-        yield slices, *[m[idx] for m, idx in zip(matrices, m_idx)]
-    
-
-def memory_size(shape: Tuple[int, ...], item_size: int) -> int:
-    """
-    Calculate the memory size, in bytes of an array with the given size and shape. Does not
-    calculate the actual array, just theoretical size since this function is intended
-    to be used before attempting allocate an array that is too large.
-
-    Args:
-        shape (list-like): Shape of the array in question.
-        item_size(int): Size of an array element in bytes.
-
-    Returns:
-        int: Expected memory size of array in bytes
-    
-    """
-    size: int = np.prod(shape,dtype=np.ulonglong)*item_size
-    return size
-
-
-def get_slice_num(n: int, stack_shape: Tuple[int, ...], doppler_shape: Tuple[int, ...],
-                  sum_doppler: bool, weight_doppler: bool,
-                  n_slices: Union[int,None] = None,
-                  debug: bool = False) -> Tuple[int, Tuple[int, ...]]:
-    """
-    Estimates the memory required for the desired steady state solve.
-
-    Estimates are fairly accurate, but not guaranteed.
-    Goal is to err on allowing edge case solves to proceed.
-
-    Parameters
-    ----------
-    n: int
-        Size of the system basis
-    stack_shape: tuple of int
-        Tuple of sizes for the hamiltonian stack to be solved
-    doppler_shape: tuple of int
-        Tuple of sizes for the doppler axes.
-        Pass an empty tuple if no doppler averaging.
-    sum_doppler: bool
-        Whether solution will be summing the doppler average
-    weight_doppler: bool
-        Whether the solution will apply weights to the doppler averaging
-    n_slices: int, default=1
-        Manually override the minimum number of hamiltonian slices to use.
-    debug: bool, default=False
-        Print debug information about the memory calculations.
-
-    Returns
-    -------
-    n_ham_slices: int
-        Number of slices to use when solving the stacked hamiltonian
-    out_sol_shape: tuple of int
-        Shape of the resulting solution for this calculation.
-
-    Raises
-    ------
-    MemoryError: If there isn't enough memory to solve the system
-    MemoryError: If `sum_doppler=False` and full solution does not fit in memory.
-
-    """
-    # set the initial number of slices to 1 if None are specified
-    #This is primarily to handle the fact that n_slices defaults to None
-    # in matrix_slice
-    if n_slices is None:
-        n_slices=1
-    # get total avaialable memory for the system
-    total_mem = psutil.virtual_memory().available
-    # total number of EOM systems to solve for the stack
-    stack_factor = np.prod(stack_shape, dtype=np.ulonglong)
-    # track memory to solve a single set of EOMs
-    single_eom_mem = 0
-    # track mandatory memory per solve
-    mand_sol_mem = 0
-
-    # determine minimum memory requirements for a solve
-    # 16 bytes for complex128 arrays, 8 bytes for float64 arrays
-    ham_shape = (*stack_shape, n, n)
-    ham_size = memory_size(ham_shape, 16)
-    sol_shape = (*stack_shape, n**2-1)
-    sol_size = memory_size(sol_shape, 8)
-    # all solves need to make full sized hamiltonians and solutions
-    # happens in solve_steady_state
-    mand_sol_mem += (ham_size + sol_size)
-    # rest of these memory allocations happen in _solve_hamiltonian_stack
-
-    eom_shape = (n**2, n**2)
-    const_shape = eom_shape[:-1]
-    eom_size = memory_size(eom_shape, 16) + memory_size(const_shape,16)
-    # minimum solve must be able to make at least one set of EOMs
-    # note that you have to times 2 for remove_ground
-    # make_real now deallocates at the end, but keeping 1.5 factor for buffer
-    # round factor up to 3 to keep types as int and give buffer
-    # happens in generate_eom
-    single_eom_mem += eom_size * 3
-
-    if doppler_shape:
-        dop_eom_shape = (*doppler_shape, n**2-1, n**2-1)
-        dop_eom_size = memory_size(dop_eom_shape,8)
-        # all doppler solves must allocate the dop EOMs in addition to bare
-        single_eom_mem += dop_eom_size
-
-        # to solve doppler, need to allocate full dop sol size
-        dop_sol_shape = dop_eom_shape[:-1]
-        dop_sol_size = memory_size(dop_sol_shape,8)
-        if weight_doppler:
-            # weighting adds extra dop sol allocation
-            dop_sol_size *= 2
-        else:
-            # not summing or weighting only leaves dop_sol_size
-            pass
-
-        single_eom_mem += dop_sol_size
-
-    # minimum required memory to solve a single set of EOMs in the stack
-    min_sol_mem = mand_sol_mem + single_eom_mem
-    # required memory to solve the entire stack at once
-    full_sol_mem = mand_sol_mem + single_eom_mem*stack_factor
-    # get memory available for solving hamiltonian slices
-    available_mem = total_mem - mand_sol_mem
-    if doppler_shape and not sum_doppler:
-        # not summing doppler, don't allocate summed solutiion
-        available_mem -= sol_size
-        full_sol_mem -= sol_size
-        min_sol_mem -= sol_size
-
-    if doppler_shape and not sum_doppler:
-        out_sol_shape = (*doppler_shape, *stack_shape, n**2-1)
-    else:
-        out_sol_shape = sol_shape
-    output_sol_size = memory_size(out_sol_shape, 8)
-
-    if debug:
-        print(f'Total available memory: {total_mem/1024**3:.5g} GiB')
-        print(f'Min Req memory to solve: {min_sol_mem/1024**3:.5g} GiB')
-        print(f'Req memory per EOM: {single_eom_mem/1024**3:.5g} GiB')
-        print(f'Req memory for full solve: {full_sol_mem/1024**3:.5g} GiB')
-        print(f'\tMandatory memory use: {mand_sol_mem/1024**3:.5g} GiB')
-        print(f'\tMemory use for all EOMs: {single_eom_mem*stack_factor/1024**3:.5g} GiB')
-        print(f'\tFull output solution size: {output_sol_size/1024**3:.5g} GiB')
-        print(f'Available memory for sliced solves: {available_mem/1024**3:.5g} GiB')
-
-    if (total_mem - min_sol_mem) <= 0:
-        raise MemoryError(f'System is too large to solve. Need at least {min_sol_mem/1024**3} GiB')
-    
-    compare_vals = np.array([np.ceil(single_eom_mem*stack_factor / available_mem), n_slices],
-                            dtype=float)
-    n_ham_slices = int(np.nanmax(compare_vals))
-
-    if doppler_shape:
-        if not sum_doppler and n_ham_slices > 1:
-            msg = ("Setting 'sum_doppler=False' if full equations of motion"
-                   " do not fit in memory is unsupported.")
-            raise MemoryError(msg)
-
-    if debug:
-        print(f'Number of stack slices to be used: {n_ham_slices:d}')
-
-    return n_ham_slices, out_sol_shape
-
-
-def get_slice_num_t(n: int, stack_shape: Tuple[int, ...],
-                    doppler_shape: Tuple[int, ...], time_points: int,
-                    sum_doppler: bool,
-                    n_slices: Union[int,None], debug: bool = False) -> Tuple[int, Tuple[int, ...]]:
-    """
-    Estimates the memory required for the desired time solve.
-
-    Note that the time solver used (scipy.solve_ivp) is an adaptive
-    solver, so the internal number of time steps used is
-    problem dependent and not controlled by the requested number
-    of time points. Generally, the number of points is proportional
-    to the highest frequency in the problem and the length of the time
-    to solve.
-    To estimate a lower bound on the memory
-    needed to time solve, we use a fudge factor of 4 on the
-    requested time points. This is unlikely to be accurate
-    even in a general case.
-
-    Parameters
-    ----------
-    n: int
-        Size of the system basis
-    stack_shape: tuple of int
-        Tuple of sizes for the hamiltonian stack to be solved
-    doppler_shape: tuple of int
-        Tuple of sizes for the doppler axes.
-        Pass an empty tuple if no doppler averaging.
-    time_points: int
-        Number of time steps requested from the time solver.
-        This sets the output solution shape.
-        An internal fudge factor of 4 is applied for memory estimation purposes.
-    sum_doppler: bool
-        Whether solution will be summing the doppler average
-    n_slices: int, default=1
-        Manually override the minimum number of hamiltonian slices to use.
-    debug: bool, default=False
-        Print debug information about the memory calculations.
-
-    Returns
-    -------
-    n_ham_slices: int
-        Number of slices to use when solving the stacked hamiltonian
-    out_sol_shape: tuple of int
-        Shape of the resulting solution for this calculation.
-
-    Raises
-    ------
-    MemoryError: If `sum_doppler=False` and full solution does not fit in memory.
-
-    Warns
-    -----
-    UserWarning: If there is unlikely to be enough memory to solve the system.
-
-    """
-    # get total avaialable memory for the system
-    total_mem = psutil.virtual_memory().available
-    # total number of EOM systems to solve for the stack
-    stack_factor = np.prod(stack_shape, dtype=np.ulonglong)
-    # track memory to solve a single set of EOMs
-    single_eom_mem = 0
-    # track mandatory memory per solve
-    mand_sol_mem = 0
-
-    # determine minimum memory requirements for a solve
-    # 16 bytes for complex128 arrays, 8 bytes for float64 arrays
-    ham_shape = (*stack_shape, n, n)
-    ham_size = memory_size(ham_shape, 16)
-    sol_shape = (*stack_shape, time_points, n**2-1)
-    sol_size = memory_size(sol_shape, 8)
-    # all solves need to make 3 full sized hamiltonians and solutions
-    # happens in solve_time
-    mand_sol_mem += (3*ham_size + sol_size)
-    # rest of these memory allocations happen in _solve_hamiltonian_stack
-
-    eom_shape = (n**2, n**2)
-    const_shape = eom_shape[:-1]
-    eom_size = memory_size(eom_shape, 16) + memory_size(const_shape,16)
-    # minimum solve must be able to make at least one set of EOMs
-    # note that you have to times 2 for remove_ground
-    # make_real now deallocates at the end, but keeping 1.5 factor for buffer
-    # round factor up to 3 to keep types as int and give buffer
-    # happens in generate_eom
-    # have to make two copies for the real/imag time dependent eoms too
-    single_eom_mem += eom_size * 3 * 3
-
-    # time solver is adaptive, so number of solve points
-    # will almost always exceed requested, so fudging a bit
-    # note that unused intermediate steps will be GC once solve_ivp result
-    # object is dumped, however these points must fit in memory during the solve
-    time_fudge = 4
-
-    if doppler_shape:
-        dop_eom_shape = (*doppler_shape, n**2-1, n**2-1)
-        dop_eom_size = memory_size(dop_eom_shape,8)
-        # all doppler solves must allocate the dop EOMs in addition to bare
-        single_eom_mem += dop_eom_size
-
-        # to solve doppler, need to allocate full dop sol size
-        dop_sol_shape = (*doppler_shape, time_points, n**2-1)
-        dop_sol_size = memory_size(dop_sol_shape,8)
-
-        single_eom_mem += dop_sol_size * time_fudge
-        if sum_doppler:
-            # weighting adds extra dop sol allocation
-            single_eom_mem += dop_sol_size
-
-    else:
-        single_eom_mem *= time_fudge
-
-    # minimum required memory to solve a single set of EOMs in the stack
-    min_sol_mem = mand_sol_mem + single_eom_mem
-    # required memory to solve the entire stack at once
-    full_sol_mem = mand_sol_mem + single_eom_mem*stack_factor
-    # get memory available for solving hamiltonian slices
-    available_mem = total_mem - mand_sol_mem
-    if doppler_shape and not sum_doppler:
-        # not summing doppler, don't allocate summed solutiion
-        available_mem -= sol_size
-        full_sol_mem -= sol_size
-        min_sol_mem -= sol_size
-
-    if doppler_shape and not sum_doppler:
-        out_sol_shape = (*doppler_shape, *stack_shape, time_points, n**2-1)
-    else:
-        out_sol_shape = sol_shape
-    output_sol_size = memory_size(out_sol_shape, 8)
-
-    if debug:
-        print(f'Total available memory: {total_mem/1024**3:.5g} GiB')
-        print(f'Min Req memory to solve: {min_sol_mem/1024**3:.5g} GiB')
-        print(f'Req memory per EOM: {single_eom_mem/1024**3:.5g} GiB')
-        print(f'Req memory for full solve: {full_sol_mem/1024**3:.5g} GiB')
-        print(f'\tMandatory memory use: {mand_sol_mem/1024**3:.5g} GiB')
-        print(f'\tMemory use for all EOMs: {single_eom_mem*stack_factor/1024**3:.5g} GiB')
-        print(f'\tFull output solution size: {output_sol_size/1024**3:.5g} GiB')
-        print(f'Available memory for sliced solves: {available_mem/1024**3:.5g} GiB')
-
-    if (total_mem - min_sol_mem) <= 0:
-        warnings.warn(
-            f'System is likely too large to solve. Need at least {min_sol_mem/1024**3} GiB')
-
-    #array of the minimum necessary slices and the specified number of slices
-    compare_vals = np.array([np.ceil(single_eom_mem*stack_factor / available_mem), n_slices],
-                            dtype=float)
-    n_ham_slices = int(np.nanmax(compare_vals))
-
-    if doppler_shape:
-        if not sum_doppler and n_ham_slices > 1:
-            msg = ("Setting 'sum_doppler=False' if full equations of motion"
-                   " do not fit in memory is unsupported.")
-            raise MemoryError(msg)
-
-    if debug:
-        print(f'Number of stack slices to be used: {n_ham_slices:d}')
-
-    return n_ham_slices, out_sol_shape
+"""
+A handful of tools that solvers use to interface with slicing matrix stacks
+"""
+
+import psutil
+import warnings
+import itertools
+
+import numpy as np
+
+from typing import Dict, Tuple, Iterator, Union, List
+
+
+def compute_grid(stack_shape: np.ndarray, n_slices: int):
+    """Calculate the bin edges to break a given stack shape into at least a certain number of pieces
+
+    Works by iterating first over a number of slices per axis (N=1,2,3), then over each in the stack shape,
+    splitting the axis into N slices, and comparing the total number of slices to the number specified. In a
+    sense, the algorithm factors a number greater than or equal to n_slices, then breaks the stack along each
+    axis according to this factorization. If the axis lengths do not break evenly into the appropriate number
+    of pieces, the bin edges are truncated to an integer. This means that the slices are not guaranteed to be
+    `(1/n_slices)`, but they will be close enough for most cases. 
+
+    Parameters
+    ----------
+    stack_shape : np.ndarray
+        The shape of the stack to be sliced. Does not include Hamiltonian or matrix equation dimensions,
+        so for a hamiltonain stack of shape `(*l,n,n)`, `stack_shape` will be `*l`.
+    n_slices : int
+        The number of slices into which to break the hamiltonian. Lower bound on the number of 
+        slices there will actually be.
+
+    Returns
+    -------
+    list(np.ndarray)
+        The list of bin edges axis by axis. Can be passed to :func:`matrix_slice` as the `edges` 
+        argument.
+        
+    Examples
+    --------
+    >>> stack_shape=(10,10)
+    >>> print(compute_grid(stack_shape, 4))
+    [array([ 0,  5, 10]), array([ 0,  5, 10])]
+    >>> print(compute_grid(stack_shape, 6))
+    [array([ 0,  3,  6, 10]), array([ 0,  5, 10])]
+    """
+    
+    if n_slices > np.prod(stack_shape):
+        raise ValueError(f"Too many slices ({n_slices}) for stack of shape {stack_shape}")
+    
+    n_ax_slices = np.ones_like(stack_shape)
+    
+    current_slices = 1
+    current_axis = 0
+    
+    while current_slices < n_slices:
+        n_ax_slices[current_axis]+= 1
+        current_slices = np.prod(n_ax_slices)
+        current_axis += 1
+        
+        if current_axis ==len(stack_shape):
+            current_axis=0
+    total_axes = sum([1 for a in n_ax_slices if a>1])
+    
+    return [np.linspace(0,stack_shape[i], n_ax_slices[i]+1, dtype=int) for i in range(total_axes)]
+
+
+def matrix_slice(*matrices: np.ndarray, edges:Union[List, None]=None, n_slices:Union[int, None]=None) -> Iterator[Tuple[tuple, np.ndarray]]:
+    """
+    Generator that returns parts of a stack of matrices.
+
+    Given a stack of n by n matrices, produces a genererator which returns the given matrices
+    in the specified number of smaller stacks. For example, given a stack of matrices of shape
+    `(10,10,4,4)` with 4 slices, generates 4 stacks of shape `(5,4,4)`. Due to the nature
+    of the slicing, the number of slices might be slightly greater that the number specified.
+    Output matrices will be broadcastable by numpy's broadcasting rules. Input arrays are interpreted as
+    a stack, with the last 2 dimensions staying intact.
+
+    Args
+    ----
+    matrices: np.ndarray 
+        matrix stacks to be sliced. All matrices must be of shapes that can be
+        broadcast by numpy's broadcasting rules, with the additional restriction that all matrices
+        must have the same number of dimensions, even if some dimensions are of size 1. For example,
+        matrices of sizes `(10,1,4,4)` and `(1,20,4,4)` can be sliced together. 
+    edges: list(iterable)
+        The values along each axis that define the edges of bins on an n-dimensional grid. For example,
+        to slice a grid of hamiltonians with stack_shape `(10,10)` into 4 pieces, `edges` could be defined as
+        `[0,5,10]` for each of the 2 stack axes. 
+    n_slices : int or None 
+        The number of slices into which to break the matrix stack. Ignored if the
+        `edges` parameter is not `None`. Must be specified as an integer value if `edges` is `None`, 
+        ignored otherwise. Defaults to None. 
+
+    Yields
+    ------
+    numpy.ndarray
+        Slice of hamiltonian stack
+        
+    Examples
+    --------
+    >>> import numpy as np
+    >>> import rydiqule as rq
+
+    >>> M1 = np.ones((1,20,4,4))
+    >>> M2 = np.ones((20,1,4,4))
+    >>> M3 = np.ones((20,20,4,4))
+    
+    >>> axis0_edges = np.array([0,10,20])
+    >>> axis1_edges = np.array([0,10,20])
+    
+    >>> for idx,m1,m2, m3 in rq.matrix_slice(M1, M2, M3, edges=[axis0_edges, axis1_edges]):
+    >>>     print(m1.shape, m2.shape, m3.shape)
+    
+    (1, 10, 4, 4) (10, 1, 4, 4) (10, 10, 4, 4)
+    (1, 10, 4, 4) (10, 1, 4, 4) (10, 10, 4, 4)
+    (1, 10, 4, 4) (10, 1, 4, 4) (10, 10, 4, 4)
+    (1, 10, 4, 4) (10, 1, 4, 4) (10, 10, 4, 4)
+    """
+    #catch input shape errors and raise more useful errors
+    shapes = [m.shape for m in matrices]
+    if len(matrices) == 0:
+        raise ValueError("Must provide at least 1 matrix for slicing")
+    if matrices[0].ndim < 2:
+        raise ValueError("Must have at least 2d matrices to slice")
+
+    try:
+        stack_shape = np.broadcast_shapes(*shapes)[:-2]
+    except ValueError:
+        raise ValueError(f"Incompatiple input shapes {shapes}")
+    
+    # handle the trivial case of a single hamiltonian
+    if len(stack_shape) == 0:
+        yield (), *matrices
+        return
+    #Build the grid if only the number of slices is specified. 
+    if edges==None:
+        if n_slices in (1,None):
+            yield (), *matrices
+            return
+        elif n_slices>1:
+            edges = compute_grid(stack_shape, n_slices)
+
+    #check that the bins slice each axis appropriately
+    for i,e in enumerate(edges):
+        if e[0] != 0 or e[-1] != stack_shape[i]:
+            raise ValueError(f"slices must start at 0 and end at the axis length ({stack_shape[i]} for axis {i})")
+
+    start_edges = [e[:-1] for e in edges] # "left" edge
+    end_edges = [e[1:] for e in edges] #"right" edge
+
+    #loop over each box, defined by 2 opposite corners p_start and p_end. 
+    #eg consider the 3-box from (4,4,4) to (6,6,6)
+    #in this case p_start will be (4,4,4) and p_end will be (6,6,6)
+    for p_start, p_end in zip(itertools.product(*start_edges), itertools.product(*end_edges)):
+
+        #loop over dimensions for each box and get the box bounds as slices
+        slices = []
+        for i in range(len(p_start)):
+            slices.append(slice(p_start[i], p_end[i]))
+        slices = tuple(slices)
+        
+        m_idx = [] #actual matrix indeces, accounting for broadcasting support
+        for m in matrices:
+            m_idx.append(tuple(idx
+                if m.shape[j] !=1
+                else slice(0,None)
+                for j, idx in enumerate(slices)
+            ))
+        
+        yield slices, *[m[idx] for m, idx in zip(matrices, m_idx)]
+    
+
+def memory_size(shape: Tuple[int, ...], item_size: int) -> int:
+    """
+    Calculate the memory size, in bytes of an array with the given size and shape. Does not
+    calculate the actual array, just theoretical size since this function is intended
+    to be used before attempting allocate an array that is too large.
+
+    Args:
+        shape (list-like): Shape of the array in question.
+        item_size(int): Size of an array element in bytes.
+
+    Returns:
+        int: Expected memory size of array in bytes
+    
+    """
+    size: int = np.prod(shape,dtype=np.ulonglong)*item_size
+    return size
+
+
+def get_slice_num(n: int, stack_shape: Tuple[int, ...], doppler_shape: Tuple[int, ...],
+                  sum_doppler: bool, weight_doppler: bool,
+                  n_slices: Union[int,None] = None, debug: bool = False) -> Tuple[int, Tuple[int, ...]]:
+    """
+    Estimates the memory required for the desired steady state solve.
+
+    Estimates are fairly accurate, but not guaranteed.
+    Goal is to err on allowing edge case solves to proceed.
+
+    Parameters
+    ----------
+    n: int
+        Size of the system basis
+    stack_shape: tuple of int
+        Tuple of sizes for the hamiltonian stack to be solved
+    doppler_shape: tuple of int
+        Tuple of sizes for the doppler axes.
+        Pass an empty tuple if no doppler averaging.
+    sum_doppler: bool
+        Whether solution will be summing the doppler average
+    weight_doppler: bool
+        Whether the solution will apply weights to the doppler averaging
+    n_slices: int, default=1
+        Manually override the minimum number of hamiltonian slices to use.
+    debug: bool, default=False
+        Print debug information about the memory calculations.
+
+    Returns
+    -------
+    n_ham_slices: int
+        Number of slices to use when solving the stacked hamiltonian
+    out_sol_shape: tuple of int
+        Shape of the resulting solution for this calculation.
+
+    Raises
+    ------
+    MemoryError: If there isn't enough memory to solve the system
+    MemoryError: If `sum_doppler=False` and full solution does not fit in memory.
+
+    """
+    # set the initial number of slices to 1 if None are specified
+    #This is primarily to handle the fact that n_slices defaults to None
+    # in matrix_slice
+    if n_slices==None:
+        n_slices=1
+    # get total avaialable memory for the system
+    total_mem = psutil.virtual_memory().available
+    # total number of EOM systems to solve for the stack
+    stack_factor = np.prod(stack_shape, dtype=np.ulonglong)
+    # track memory to solve a single set of EOMs
+    single_eom_mem = 0
+    # track mandatory memory per solve
+    mand_sol_mem = 0
+
+    # determine minimum memory requirements for a solve
+    # 16 bytes for complex128 arrays, 8 bytes for float64 arrays
+    ham_shape = (*stack_shape, n, n)
+    ham_size = memory_size(ham_shape, 16)
+    sol_shape = (*stack_shape, n**2-1)
+    sol_size = memory_size(sol_shape, 8)
+    # all solves need to make full sized hamiltonians and solutions
+    # happens in solve_steady_state
+    mand_sol_mem += (ham_size + sol_size)
+    # rest of these memory allocations happen in _solve_hamiltonian_stack
+
+    eom_shape = (n**2, n**2)
+    const_shape = eom_shape[:-1]
+    eom_size = memory_size(eom_shape, 16) + memory_size(const_shape,16)
+    # minimum solve must be able to make at least one set of EOMs
+    # note that you have to times 2 for remove_ground
+    # make_real now deallocates at the end, but keeping 1.5 factor for buffer
+    # round factor up to 3 to keep types as int and give buffer
+    # happens in generate_eom
+    single_eom_mem += eom_size * 3
+
+    if doppler_shape:
+        dop_eom_shape = (*doppler_shape, n**2-1, n**2-1)
+        dop_eom_size = memory_size(dop_eom_shape,8)
+        # all doppler solves must allocate the dop EOMs in addition to bare
+        single_eom_mem += dop_eom_size
+
+        # to solve doppler, need to allocate full dop sol size
+        dop_sol_shape = dop_eom_shape[:-1]
+        dop_sol_size = memory_size(dop_sol_shape,8)
+        if weight_doppler:
+            # weighting adds extra dop sol allocation
+            dop_sol_size *= 2
+        else:
+            # not summing or weighting only leaves dop_sol_size
+            pass
+
+        single_eom_mem += dop_sol_size
+
+    # minimum required memory to solve a single set of EOMs in the stack
+    min_sol_mem = mand_sol_mem + single_eom_mem
+    # required memory to solve the entire stack at once
+    full_sol_mem = mand_sol_mem + single_eom_mem*stack_factor
+    # get memory available for solving hamiltonian slices
+    available_mem = total_mem - mand_sol_mem
+    if doppler_shape and not sum_doppler:
+        # not summing doppler, don't allocate summed solutiion
+        available_mem -= sol_size
+        full_sol_mem -= sol_size
+        min_sol_mem -= sol_size
+
+    if doppler_shape and not sum_doppler:
+        out_sol_shape = (*doppler_shape, *stack_shape, n**2-1)
+    else:
+        out_sol_shape = sol_shape
+    output_sol_size = memory_size(out_sol_shape, 8)
+
+    if debug:
+        print(f'Total available memory: {total_mem/1024**3:.5g} GiB')
+        print(f'Min Req memory to solve: {min_sol_mem/1024**3:.5g} GiB')
+        print(f'Req memory per EOM: {single_eom_mem/1024**3:.5g} GiB')
+        print(f'Req memory for full solve: {full_sol_mem/1024**3:.5g} GiB')
+        print(f'\tMandatory memory use: {mand_sol_mem/1024**3:.5g} GiB')
+        print(f'\tMemory use for all EOMs: {single_eom_mem*stack_factor/1024**3:.5g} GiB')
+        print(f'\tFull output solution size: {output_sol_size/1024**3:.5g} GiB')
+        print(f'Available memory for sliced solves: {available_mem/1024**3:.5g} GiB')
+
+    if (total_mem - min_sol_mem) <= 0:
+        raise MemoryError(f'System is too large to solve. Need at least {min_sol_mem/1024**3} GiB')
+    
+    compare_vals = np.array([np.ceil(single_eom_mem*stack_factor / available_mem), n_slices], dtype=float)
+    n_ham_slices = int(np.nanmax(compare_vals))
+
+    if doppler_shape:
+        if not sum_doppler and n_ham_slices > 1:
+            msg = ("Setting 'sum_doppler=False' if full equations of motion"
+                   " do not fit in memory is unsupported.")
+            raise MemoryError(msg)
+
+    if debug:
+        print(f'Number of stack slices to be used: {n_ham_slices:d}')
+
+    return n_ham_slices, out_sol_shape
+
+
+def get_slice_num_t(n: int, stack_shape: Tuple[int, ...],
+                    doppler_shape: Tuple[int, ...], time_points: int,
+                    sum_doppler: bool,
+                    n_slices: Union[int,None], debug: bool = False) -> Tuple[int, Tuple[int, ...]]:
+    """
+    Estimates the memory required for the desired time solve.
+
+    Note that the time solver used (scipy.solve_ivp) is an adaptive
+    solver, so the internal number of time steps used is
+    problem dependent and not controlled by the requested number
+    of time points. Generally, the number of points is proportional
+    to the highest frequency in the problem and the length of the time
+    to solve.
+    To estimate a lower bound on the memory
+    needed to time solve, we use a fudge factor of 4 on the
+    requested time points. This is unlikely to be accurate
+    even in a general case.
+
+    Parameters
+    ----------
+    n: int
+        Size of the system basis
+    stack_shape: tuple of int
+        Tuple of sizes for the hamiltonian stack to be solved
+    doppler_shape: tuple of int
+        Tuple of sizes for the doppler axes.
+        Pass an empty tuple if no doppler averaging.
+    time_points: int
+        Number of time steps requested from the time solver.
+        This sets the output solution shape.
+        An internal fudge factor of 4 is applied for memory estimation purposes.
+    sum_doppler: bool
+        Whether solution will be summing the doppler average
+    n_slices: int, default=1
+        Manually override the minimum number of hamiltonian slices to use.
+    debug: bool, default=False
+        Print debug information about the memory calculations.
+
+    Returns
+    -------
+    n_ham_slices: int
+        Number of slices to use when solving the stacked hamiltonian
+    out_sol_shape: tuple of int
+        Shape of the resulting solution for this calculation.
+
+    Raises
+    ------
+    MemoryError: If `sum_doppler=False` and full solution does not fit in memory.
+
+    Warns
+    -----
+    UserWarning: If there is unlikely to be enough memory to solve the system.
+
+    """
+    # get total avaialable memory for the system
+    total_mem = psutil.virtual_memory().available
+    # total number of EOM systems to solve for the stack
+    stack_factor = np.prod(stack_shape, dtype=np.ulonglong)
+    # track memory to solve a single set of EOMs
+    single_eom_mem = 0
+    # track mandatory memory per solve
+    mand_sol_mem = 0
+
+    # determine minimum memory requirements for a solve
+    # 16 bytes for complex128 arrays, 8 bytes for float64 arrays
+    ham_shape = (*stack_shape, n, n)
+    ham_size = memory_size(ham_shape, 16)
+    sol_shape = (*stack_shape, time_points, n**2-1)
+    sol_size = memory_size(sol_shape, 8)
+    # all solves need to make 3 full sized hamiltonians and solutions
+    # happens in solve_time
+    mand_sol_mem += (3*ham_size + sol_size)
+    # rest of these memory allocations happen in _solve_hamiltonian_stack
+
+    eom_shape = (n**2, n**2)
+    const_shape = eom_shape[:-1]
+    eom_size = memory_size(eom_shape, 16) + memory_size(const_shape,16)
+    # minimum solve must be able to make at least one set of EOMs
+    # note that you have to times 2 for remove_ground
+    # make_real now deallocates at the end, but keeping 1.5 factor for buffer
+    # round factor up to 3 to keep types as int and give buffer
+    # happens in generate_eom
+    # have to make two copies for the real/imag time dependent eoms too
+    single_eom_mem += eom_size * 3 * 3
+
+    # time solver is adaptive, so number of solve points
+    # will almost always exceed requested, so fudging a bit
+    # note that unused intermediate steps will be GC once solve_ivp result
+    # object is dumped, however these points must fit in memory during the solve
+    time_fudge = 4
+
+    if doppler_shape:
+        dop_eom_shape = (*doppler_shape, n**2-1, n**2-1)
+        dop_eom_size = memory_size(dop_eom_shape,8)
+        # all doppler solves must allocate the dop EOMs in addition to bare
+        single_eom_mem += dop_eom_size
+
+        # to solve doppler, need to allocate full dop sol size
+        dop_sol_shape = (*doppler_shape, time_points, n**2-1)
+        dop_sol_size = memory_size(dop_sol_shape,8)
+
+        single_eom_mem += dop_sol_size * time_fudge
+        if sum_doppler:
+            # weighting adds extra dop sol allocation
+            single_eom_mem += dop_sol_size
+
+    else:
+        single_eom_mem *= time_fudge
+
+    # minimum required memory to solve a single set of EOMs in the stack
+    min_sol_mem = mand_sol_mem + single_eom_mem
+    # required memory to solve the entire stack at once
+    full_sol_mem = mand_sol_mem + single_eom_mem*stack_factor
+    # get memory available for solving hamiltonian slices
+    available_mem = total_mem - mand_sol_mem
+    if doppler_shape and not sum_doppler:
+        # not summing doppler, don't allocate summed solutiion
+        available_mem -= sol_size
+        full_sol_mem -= sol_size
+        min_sol_mem -= sol_size
+
+    if doppler_shape and not sum_doppler:
+        out_sol_shape = (*doppler_shape, *stack_shape, time_points, n**2-1)
+    else:
+        out_sol_shape = sol_shape
+    output_sol_size = memory_size(out_sol_shape, 8)
+
+    if debug:
+        print(f'Total available memory: {total_mem/1024**3:.5g} GiB')
+        print(f'Min Req memory to solve: {min_sol_mem/1024**3:.5g} GiB')
+        print(f'Req memory per EOM: {single_eom_mem/1024**3:.5g} GiB')
+        print(f'Req memory for full solve: {full_sol_mem/1024**3:.5g} GiB')
+        print(f'\tMandatory memory use: {mand_sol_mem/1024**3:.5g} GiB')
+        print(f'\tMemory use for all EOMs: {single_eom_mem*stack_factor/1024**3:.5g} GiB')
+        print(f'\tFull output solution size: {output_sol_size/1024**3:.5g} GiB')
+        print(f'Available memory for sliced solves: {available_mem/1024**3:.5g} GiB')
+
+    if (total_mem - min_sol_mem) <= 0:
+        warnings.warn(f'System is likely too large to solve. Need at least {min_sol_mem/1024**3} GiB')
+
+    #array of the minimum necessary slices and the specified number of slices
+    compare_vals = np.array([np.ceil(single_eom_mem*stack_factor / available_mem), n_slices], dtype=float)
+    n_ham_slices = int(np.nanmax(compare_vals))
+
+    if doppler_shape:
+        if not sum_doppler and n_ham_slices > 1:
+            msg = ("Setting 'sum_doppler=False' if full equations of motion"
+                   " do not fit in memory is unsupported.")
+            raise MemoryError(msg)
+
+    if debug:
+        print(f'Number of stack slices to be used: {n_ham_slices:d}')
+
+    return n_ham_slices, out_sol_shape
```

### Comparing `rydiqule-1.0.0/src/rydiqule/solvers.py` & `rydiqule-1.0.0rc2/src/rydiqule/solvers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,275 +1,268 @@
-"""
-Steady-state solvers of the Optical Bloch Equations.
-"""
-import numpy as np
-from importlib.metadata import version
-
-from .sensor import Sensor
-from .sensor_utils import *
-from .doppler_utils import *
-from .slicing.slicing import *
-from .sensor_solution import Solution
-
-from typing import Optional, Iterable, Union
-
-
-def solve_steady_state(
-        sensor: Sensor, doppler: bool = False, doppler_mesh_method: Optional[MeshMethod] = None,
-        sum_doppler: bool = True, weight_doppler: bool = True, 
-        n_slices: Union[int, None] = None,
-        ) -> Solution:
-    """
-    Finds the steady state solution for a system characterized by a sensor.
-
-    If insuffucent system memory is available to solve the system in a single call, 
-    system is broken into "slices" of manageable memory footprint which are solved indivudually.
-    This slicing behavior does not affect the result.
-    Can be performed with or without doppler averging.
-
-    Parameters
-    ----------
-    sensor : :class:`~.Sensor`
-        The sensor for which the solution will be calculated.
-    doppler : bool, optional
-        Whether to calculate the solution for a doppler-broadened
-        gas. If `True`, only uses dopper brodening defined by `kvec` parameters
-        for couplings in the `sensoe`, so setting this `True` without `kvec` definitions 
-        will have no effect. Default is `False`.
-    doppler_mesh_method (dict,optional): 
-        If not `None`, should be a dictionary of meshing parameters to be passed 
-        to :func:`~.doppler_classes`. See :func:`~.doppler_classes` for more 
-        information on supported methods and arguments. If `None, uses the 
-        default doppler meshing. Default is `None`.
-    sum_doppler : bool
-        Whether to average over doppler classes after the solve
-        is complete. Setting to `False` will not perform the sum, allowing viewing
-        of the weighted results of the solve for each doppler class. In this case,
-        an axis will be prepended to the solution for each axis along which doppler
-        broadening is computed. Ignored if `doppler=False`. Default is `True`.
-    weight_doppler : bool
-        Whether to apply weights to doppler solution to perform
-        averaging. If `False`, will **not** apply weights or perform a doppler_average,
-        regardless of the value of `sum_doppler`. Changing from default intended
-        only for internal use. Ignored if `doppler=False` or `sum_doppler=False`. 
-        Default is `True`.
-    n_slices : int or None, optional
-        How many sets of equations to break the full equations into.
-        The actual number of slices will be the largest between this value and the minumum
-        number of slices to solve the system without a memory error. If `None`, uses the minimum
-        number of slices to solve the system without a memory error. Detailed information about 
-        slicing behavior can be found in :func:`~.slicing.slicing.matrix_slice`. Default is `None`.
-
-    Notes
-    -----
-    .. note::
-        If decoherence values are not sufficiently populated in the sensor, the resulting
-        equations may be singular, resulting in an error in `numpy.linalg`. This error is not
-        caught for flexibility, but is likely the culprit for `numpy.linalg` errors encountered
-        in steady-state solves.
-    
-    .. note::
-        The solution produced by this function will be expressed using rydiqule's convention
-        of converting a density matrix into the real basis and removing the ground state to
-        improve numerical stability.
-
-    Returns
-    -------
-    :class:`~.Solution`
-        A bunch-type object contining information about the
-        solution. Presently, only attribute "rho" is added to the solution, corresponding
-        to the density matrix of the steady state solution. Will include solutions
-        to all parameter value combinations if array-like parameters are specified.
-        
-    Examples
-    --------
-    A basic solve for a 3-level system would have a "density matrix" solution of size 8 (3^2-1)
-    
-    >>> s = rq.Sensor(3)
-    >>> s.add_coupling((0,1), detuning = 1, rabi_freqency=1)
-    >>> s.add_coupling((1,2), detuning = 2, rabi_freqency=2)
-    >>> s.add_transit_broadening(0.1)
-    >>> sol = rq.solve_steady_state(s)
-    >>> print(type(sol))
-    >>> print(type(sol.rho))
-    >>> print(sol.rho.shape)
-    <class 'rydiqule.sensor_solution.Solution'>
-    <class 'numpy.ndarray'>
-    (8,)
-    
-    Defining an array-like parameter will automatically calculate the density matrix solution
-    for every value. Here we use 11 values, resulting in 11 density matrices. The `axis_labels`
-    attribute of the solution can clarify which axes are which.
-    
-    >>> s = rq.Sensor(3)
-    >>> det = np.linspace(-1,1,11)
-    >>> s.add_coupling((0,1), detuning = det, rabi_freqency=1)
-    >>> s.add_coupling((1,2), detuning = 2, rabi_freqency=2)
-    >>> s.add_transit_broadening(0.1)
-    >>> sol = rq.solve_steady_state(s)
-    >>> print(sol.rho.shape)
-    >>> print(sol.axis_labels)
-    (11, 8)
-    ['(0,1)_detuning']
-    
-    >>> s = rq.Sensor(3)
-    >>> det = np.linspace(-1,1,11)
-    >>> s.add_coupling((0,1), detuning = det, rabi_freqency=1)
-    >>> s.add_coupling((1,2), detuning = det, rabi_freqency=2)
-    >>> s.add_transit_broadening(0.1)
-    >>> sol = rq.solve_steady_state(s)
-    >>> print(sol.rho.shape)
-    >>> print(sol.axis_labels)
-    (11, 11, 8)
-    ['(0,1)_detuning', '(1,2)_detuning']
-    
-    If the solve uses doppler broadening, but not averaging for doppler is specified,
-    there will be a solution axis corresponding to doppler classes.
-    
-    >>> s = rq.Sensor(3)
-    >>> det = np.linspace(-1,1,11)
-    >>> s.add_coupling((0,1), detuning = det, rabi_freqency=1)
-    >>> s.add_coupling((1,2), detuning = 2, rabi_freqency=2, kvec=(1,0,0))
-    >>> s.add_transit_broadening(0.1)
-    >>> sol = rq.solve_steady_state(s, doppler=True, sum_doppler=False)
-    >>> print(sol.rho.shape)
-    >>> print(sol.axis_labels)
-    (561, 11, 8)
-    ['doppler_0', '(0,1)_detuning']
-    
-    """
-    solution = Solution()
-
-    # relevant sensor-related quantities
-    stack_shape = sensor._stack_shape()
-    basis_size = sensor.basis_size
-    spatial_dim = sensor.spatial_dim()
-
-    # initialize doppler-related quantities
-    doppler_axis_shape: Iterable[int] = ()
-    dop_classes = None
-    doppler_shifts = None
-    doppler_axes: Iterable[slice] = ()
-
-    # update doppler-related values
-    if doppler:
-        dop_classes = doppler_classes(method=doppler_mesh_method)
-        doppler_shifts = sensor.get_doppler_shifts()
-        doppler_axis_shape = tuple(len(dop_classes) for _ in range(spatial_dim))
-
-        if not sum_doppler:
-            doppler_axes = tuple(slice(None) for _ in range(spatial_dim))
-
-    n_slices, out_sol_shape = get_slice_num(basis_size, stack_shape, doppler_axis_shape,
-                                                sum_doppler, weight_doppler, n_slices)
-
-    if n_slices > 1:
-        print(f"Breaking equations of motion into {n_slices} sets of equations...")
-        
-    # allocate arrays
-    hamiltonians = sensor.get_hamiltonian()
-    hamiltonians_time, _ = sensor.get_time_couplings()
-    hamiltonians_total = hamiltonians + np.sum(hamiltonians_time, axis=0)
-    gamma = sensor.decoherence_matrix()
-    sols = np.zeros(out_sol_shape)
-    
-    # loop over individual slices of hamiltonian
-    n_slices_true = sum(1 for _ in matrix_slice(gamma, n_slices=n_slices))
-
-    for i, (idx, H, G) in enumerate(matrix_slice(hamiltonians_total, gamma, n_slices=n_slices)):
-    
-        if n_slices_true > 1:
-            print(f"Solving equation slice {i+1}/{n_slices_true}", end='\r')
-        
-        full_idx = (*doppler_axes, *idx)
-        sols[full_idx] = _solve_hamiltonian_stack(
-            H, G, doppler=doppler, dop_classes=dop_classes, sum_doppler=sum_doppler,
-            weight_doppler=weight_doppler, doppler_shifts=doppler_shifts,
-            spatial_dim=spatial_dim
-            )
-
-    # save results to Solution object
-    solution.rho = sols
-    solution.eta = sensor.eta
-    solution.kappa = sensor.kappa
-    solution.couplings = sensor.get_couplings()
-    solution.axis_labels = ([f'doppler_{i:d}' for i in range(spatial_dim) if not sum_doppler]
-                            + sensor.axis_labels()
-                            + ["density_matrix"])
-    solution.axis_values = ([dop_classes for i in range(spatial_dim) if not sum_doppler]
-                            + [val for _,_,val in sensor.variable_parameters()]
-                            + [sensor.basis()])
-    solution.basis = sensor.basis()
-    solution.rq_version = version("rydiqule")
-    solution.doppler_classes = dop_classes
-
-    return solution
-
-
-def _solve_hamiltonian_stack(
-        hamiltonians: np.ndarray, gamma_matrix: np.ndarray,
-        doppler: bool = False, dop_classes: Optional[np.ndarray] = None,
-        sum_doppler: bool = True, weight_doppler: bool = True,
-        doppler_shifts: Optional[np.ndarray] = None, spatial_dim: int = 0
-        ) -> np.ndarray:
-    """
-    Solves a the equations of motion corresponding to the given set of hamiltonians.
-    
-    Typically used as an auxillary function for :meth:`~.solve_steady_state`. Hamiltonian and
-    gamma matrices must be of broadcastable shapes. 
-    """
-    eom, const = generate_eom(hamiltonians, gamma_matrix)
-
-    if doppler:
-        assert dop_classes is not None and doppler_shifts is not None
-        dop_velocities, dop_volumes = doppler_mesh(dop_classes, spatial_dim)
-
-        eom = get_doppler_equations(eom, doppler_shifts, dop_velocities)
-
-        # this is required for linalg.solve boadcasting to work
-        const = np.expand_dims(const, tuple(np.arange(spatial_dim)))
-        sols_full = steady_state_solve_stack(eom, const)
-
-        if weight_doppler:
-            sols_weighted = apply_doppler_weights(sols_full, dop_velocities, dop_volumes)
-            if sum_doppler:
-                sum_axes = tuple(np.arange(spatial_dim))
-                sols = np.sum(sols_weighted, axis=sum_axes)
-            else:
-                sols = sols_weighted
-        else:
-            sols = sols_full
-
-    else:
-        sols = steady_state_solve_stack(eom, const)
-
-    return sols
-
-
-def steady_state_solve_stack(eom: np.ndarray, const: np.ndarray) -> np.ndarray:
-    """
-    Helper function which returns the solution to the given equations of motion
-
-    Solves an equation of the form :math:`\dot{x} = Ax + b`, or a set of such equations
-    arranged into stacks. 
-    Essentially just wraps numpy.linalg.solve(), but included as its own 
-    function for modularity if another solver is found to be worth invesitigating. 
-
-    Parameters
-    ----------
-    eom : numpy.ndarray
-        An square array of shape `(*l,n,n)` representing the differential
-        equations to be solved. The matrix (or matrices) A in the above formula.
-    const : numpy.ndarray
-        An array or shape `(*l,n)` representing the constant in the matrix form
-        of the differential equation. The constant b in the above formula. Stack shape
-        `*l` must be consistent with that in the `eom` argument
-
-    Returns
-    -------
-    numpy.ndarray
-        A 1xn array representing the steady-state solution
-        of the differential equation
-    """
-    
-    sol = np.linalg.solve(eom, -const)
-    return sol
+"""
+Steady-state solvers of the Optical Bloch Equations.
+"""
+import numpy as np
+from importlib.metadata import version
+
+from .sensor import Sensor
+from .sensor_utils import *
+from .doppler_utils import *
+from .slicing.slicing import *
+from .sensor_solution import Solution
+
+from typing import Optional, Iterable, Union
+
+
+def solve_steady_state(
+        sensor: Sensor, doppler: bool = False, doppler_mesh_method: Optional[MeshMethod] = None,
+        sum_doppler: bool = True, weight_doppler: bool = True, 
+        n_slices: Union[int, None] = None,
+        ) -> Solution:
+    """
+    Finds the steady state solution for a system characterized by a sensor.
+
+    If insuffucent system memory is available to solve the system in a single call, 
+    system is broken into "slices" of manageable memory footprint which are solved indivudually.
+    This slicing behavior does not affect the result. Can be performed with or without doppler averging.
+
+    Parameters
+    ----------
+    sensor : :class:`~.Sensor`
+        The sensor for which the solution will be calculated.
+    doppler : bool, optional
+        Whether to calculate the solution for a doppler-broadened
+        gas. If `True`, only uses dopper brodening defined by `kvec` parameters
+        for couplings in the `sensoe`, so setting this `True` without `kvec` definitions 
+        will have no effect. Default is `False`.
+    doppler_mesh_method (dict,optional): 
+        If not `None`, should be a dictionary of meshing parameters to be passed 
+        to :func:`~.doppler_classes`. See :func:`~.doppler_classes` for more 
+        information on supported methods and arguments. If `None, uses the 
+        default doppler meshing. Default is `None`.
+    sum_doppler : bool
+        Whether to average over doppler classes after the solve
+        is complete. Setting to `False` will not perform the sum, allowing viewing
+        of the weighted results of the solve for each doppler class. In this case,
+        an axis will be prepended to the solution for each axis along which doppler
+        broadening is computed. Ignored if `doppler=False`. Default is `True`.
+    weight_doppler : bool
+        Whether to apply weights to doppler solution to perform
+        averaging. If `False`, will **not** apply weights or perform a doppler_average,
+        regardless of the value of `sum_doppler`. Changing from default intended
+        only for internal use. Ignored if `doppler=False` or `sum_doppler=False`. 
+        Default is `True`.
+    n_slices : int or None, optional
+        How many sets of equations to break the full equations into.
+        The actual number of slices will be the largest between this value and the minumum
+        number of slices to solve the system without a memory error. If `None`, uses the minimum
+        number of slices to solve the system without a memory error. Detailed information about 
+        slicing behavior can be found in :func:`~.slicing.slicing.matrix_slice`. Default is `None`.
+
+    Notes
+    -----
+    .. note::
+        If decoherence values are not sufficiently populated in the sensor, the resulting
+        equations may be singular, resulting in an error in `numpy.linalg`. This error is not
+        caught for flexibility, but is likely the culprit for `numpy.linalg` errors encountered
+        in steady-state solves.
+    
+    .. note::
+        The solution produced by this function will be expressed using rydiqule's convention
+        of converting a density matrix into the real basis and removing the ground state to
+        improve numerical stability.
+
+    Returns
+    -------
+    :class:`~.Solution`
+        A bunch-type object contining information about the
+        solution. Presently, only attribute "rho" is added to the solution, corresponding
+        to the density matrix of the steady state solution. Will include solutions
+        to all parameter value combinations if array-like parameters are specified.
+        
+    Examples
+    --------
+    A basic solve for a 3-level system would have a "density matrix" solution of size 8 (3^2-1)
+    
+    >>> s = rq.Sensor(3)
+    >>> s.add_coupling((0,1), detuning = 1, rabi_freqency=1)
+    >>> s.add_coupling((1,2), detuning = 2, rabi_freqency=2)
+    >>> s.add_transit_broadening(0.1)
+    >>> sol = rq.solve_steady_state(s)
+    >>> print(type(sol))
+    >>> print(type(sol.rho))
+    >>> print(sol.rho.shape)
+    <class 'rydiqule.sensor_solution.Solution'>
+    <class 'numpy.ndarray'>
+    (8,)
+    
+    Defining an array-like parameter will automatically calculate the density matrix solution
+    for every value. Here we use 11 values, resulting in 11 density matrices. The `axis_labels`
+    attribute of the solution can clarify which axes are which.
+    
+    >>> s = rq.Sensor(3)
+    >>> det = np.linspace(-1,1,11)
+    >>> s.add_coupling((0,1), detuning = det, rabi_freqency=1)
+    >>> s.add_coupling((1,2), detuning = 2, rabi_freqency=2)
+    >>> s.add_transit_broadening(0.1)
+    >>> sol = rq.solve_steady_state(s)
+    >>> print(sol.rho.shape)
+    >>> print(sol.axis_labels)
+    (11, 8)
+    ['(0,1)_detuning']
+    
+    >>> s = rq.Sensor(3)
+    >>> det = np.linspace(-1,1,11)
+    >>> s.add_coupling((0,1), detuning = det, rabi_freqency=1)
+    >>> s.add_coupling((1,2), detuning = det, rabi_freqency=2)
+    >>> s.add_transit_broadening(0.1)
+    >>> sol = rq.solve_steady_state(s)
+    >>> print(sol.rho.shape)
+    >>> print(sol.axis_labels)
+    (11, 11, 8)
+    ['(0,1)_detuning', '(1,2)_detuning']
+    
+    If the solve uses doppler broadening, but not averaging for doppler is specified,
+    there will be a solution axis corresponding to doppler classes.
+    
+    >>> s = rq.Sensor(3)
+    >>> det = np.linspace(-1,1,11)
+    >>> s.add_coupling((0,1), detuning = det, rabi_freqency=1)
+    >>> s.add_coupling((1,2), detuning = 2, rabi_freqency=2, kvec=(1,0,0))
+    >>> s.add_transit_broadening(0.1)
+    >>> sol = rq.solve_steady_state(s, doppler=True, sum_doppler=False)
+    >>> print(sol.rho.shape)
+    >>> print(sol.axis_labels)
+    (561, 11, 8)
+    ['doppler_0', '(0,1)_detuning']
+    
+    """
+    solution = Solution()
+
+    # relevant sensor-related quantities
+    stack_shape = sensor._stack_shape()
+    basis_size = sensor.basis_size
+    spatial_dim = sensor.spatial_dim()
+
+    # initialize doppler-related quantities
+    doppler_axis_shape: Iterable[int] = ()
+    dop_classes = None
+    doppler_shifts = None
+    doppler_axes: Iterable[slice] = ()
+
+    # update doppler-related values
+    if doppler:
+        dop_classes = doppler_classes(method=doppler_mesh_method)
+        doppler_shifts = sensor.get_doppler_shifts()
+        doppler_axis_shape = tuple(len(dop_classes) for _ in range(spatial_dim))
+
+        if not sum_doppler:
+            doppler_axes = tuple(slice(None) for _ in range(spatial_dim))
+
+    n_slices, out_sol_shape = get_slice_num(basis_size, stack_shape, doppler_axis_shape,
+                                                sum_doppler, weight_doppler, n_slices)
+
+    if n_slices > 1:
+        print(f"Breaking equations of motion into {n_slices} sets of equations...")
+        
+    # allocate arrays
+    hamiltonians = sensor.get_hamiltonian()
+    gamma = sensor.decoherence_matrix()
+    sols = np.zeros(out_sol_shape)
+    
+    # loop over individual slices of hamiltonian
+    n_slices_true = sum(1 for _ in matrix_slice(gamma, n_slices=n_slices))
+
+    for i, (idx, H, G) in enumerate(matrix_slice(hamiltonians, gamma, n_slices=n_slices)):
+    
+        if n_slices_true > 1:
+            print(f"Solving equation slice {i+1}/{n_slices_true}", end='\r')
+        
+        full_idx = (*doppler_axes, *idx)
+        sols[full_idx] = _solve_hamiltonian_stack(
+            H, G, doppler=doppler, dop_classes=dop_classes, sum_doppler=sum_doppler,
+            weight_doppler=weight_doppler, doppler_shifts=doppler_shifts,
+            spatial_dim=spatial_dim
+            )
+
+    # save results to Solution object
+    solution.rho = sols
+    solution.eta = sensor.eta
+    solution.kappa = sensor.kappa
+    solution.couplings = sensor.get_couplings()
+    solution.axis_labels = [f'doppler_{i:d}' for i in range(spatial_dim) if not sum_doppler] + sensor.axis_labels() + ["density_matrix"]
+    solution.axis_values = [dop_classes for i in range(spatial_dim) if not sum_doppler] + [val for _,_,val in sensor.variable_parameters()] + [sensor.basis()]
+    solution.basis = sensor.basis()
+    solution.rq_version = version("rydiqule")
+    solution.doppler_classes = dop_classes
+
+    return solution
+
+
+def _solve_hamiltonian_stack(
+        hamiltonians: np.ndarray, gamma_matrix: np.ndarray,
+        doppler: bool = False, dop_classes: Optional[np.ndarray] = None,
+        sum_doppler: bool = True, weight_doppler: bool = True,
+        doppler_shifts: Optional[np.ndarray] = None, spatial_dim: int = 0
+        ) -> np.ndarray:
+    """
+    Solves a the equations of motion corresponding to the given set of hamiltonians.
+    
+    Typically used as an auxillary function for :meth:`~.solve_steady_state`. Hamiltonian and
+    gamma matrices must be of broadcastable shapes. 
+    """
+    eom, const = generate_eom(hamiltonians, gamma_matrix)
+
+    if doppler:
+        assert dop_classes is not None and doppler_shifts is not None
+        dop_velocities, dop_volumes = doppler_mesh(dop_classes, spatial_dim)
+
+        eom = get_doppler_equations(eom, doppler_shifts, dop_velocities)
+
+        # this is required for linalg.solve boadcasting to work
+        const = np.expand_dims(const, tuple(np.arange(spatial_dim)))
+        sols_full = steady_state_solve_stack(eom, const)
+
+        if weight_doppler:
+            sols_weighted = apply_doppler_weights(sols_full, dop_velocities, dop_volumes)
+            if sum_doppler:
+                sum_axes = tuple(np.arange(spatial_dim))
+                sols = np.sum(sols_weighted, axis=sum_axes)
+            else:
+                sols = sols_weighted
+        else:
+            sols = sols_full
+
+    else:
+        sols = steady_state_solve_stack(eom, const)
+
+    return sols
+
+
+def steady_state_solve_stack(eom: np.ndarray, const: np.ndarray) -> np.ndarray:
+    """
+    Helper function which returns the solution to the given equations of motion
+
+    Solves an equation of the form :math:`\dot{x} = Ax + b`, or a set of such equations
+    arranged into stacks. 
+    Essentially just wraps numpy.linalg.solve(), but included as its own 
+    function for modularity if another solver is found to be worth invesitigating. 
+
+    Parameters
+    ----------
+    eom : numpy.ndarray
+        An square array of shape `(*l,n,n)` representing the differential
+        equations to be solved. The matrix (or matrices) A in the above formula.
+    const : numpy.ndarray
+        An array or shape `(*l,n)` representing the constant in the matrix form
+        of the differential equation. The constant b in the above formula. Stack shape
+        `*l` must be consistent with that in the `eom` argument
+
+    Returns
+    -------
+    numpy.ndarray
+        A 1xn array representing the steady-state solution
+        of the differential equation
+    """
+    
+    sol = np.linalg.solve(eom, -const)
+    return sol
```

### Comparing `rydiqule-1.0.0/src/rydiqule/stack_solvers/cyrk_solver.py` & `rydiqule-1.0.0rc2/src/rydiqule/stack_solvers/cyrk_solver.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,156 +1,154 @@
-import warnings
-
-import numpy as np
-import numba as nb
-
-from CyRK import cyrk_ode
-
-from typing import Sequence, Callable, Union, Tuple
-
-
-def cyrk_solve(eoms_base: np.ndarray, const_base: np.ndarray,
-               eom_time_r: np.ndarray, const_r: np.ndarray,
-               eom_time_i: np.ndarray, const_i: np.ndarray,
-               time_inputs: Sequence[Callable[[float], Union[float, complex]]],
-               t_eval: np.ndarray, init_cond: np.ndarray,
-               **kwargs
-               ) -> np.ndarray:
-    """
-    Solve a set of Optical Bloch Equations (OBEs) with rydiqule's time solving convention
-    using CyRK's `cyrk_ode`.
-
-    Uses matrix components of the equations of motion provided by the methods of a :meth:`~.Sensor`.
-    Designed to be used as a wrapped function within :func:`~.timesolvers.solve_time`.
-    Builds and solves equations of motion according rydiqule's time solving conventions.
-    Sets up and solves dx/dt = A(t)x + b(t)
-
-    Args
-    ----
-    eoms_base: numpy.ndarray
-        The matrix of shape `(*l,n,n)` representing the non time-varying portion of the matrix A
-        in the equations of motion.
-    const_base: numpy.ndarray
-        The array of shape `(*l, n)` representing the non time-varying portion of the vector b in the
-        equations of motion.
-    eoms_time_r: numpy.ndarraynumpy
-        The matrix of shape `(n_t, *l, n, n)` representing the real time-varying portion of the matrix A,
-        where n_t is the length of `time_inputs`.
-        The ith slice along the first axis should be multiplied by the real part
-        of the ith entry in `time_inputs`.
-    const_r: numpy.nd_array
-        The matrix of shape `(n_t, *l, n)` representing the real time-varying portion of the vector b,
-        where n_t is the length of `time_inputs`.
-        The ith slice along the first axis should be multiplied by the real part
-        of the ith entry in `time_inputs`.
-    eoms_time_i: numpy.ndarray
-        The matrix of shape `(n_t, *l, n, n)` representing the imaginary time-varying portion of the matrix A,
-        where n_t is the length of `time_inputs`.
-        The ith slice along the first axis should be multiplied by the imaginary part
-        of the ith entry in `time_inputs`.
-    const_i: numpy.nd_array
-        The matrix of shape `(n_t, *l, n)` representing the imaginary time-varying portion of the vector b,
-        where n_t is the length of `time_inputs`.
-        The ith slice along the first axis should be multiplied by the imaginary part
-        of the ith entry in `time_inputs`.
-    time_inputs: list(callable)
-        List of callable functions of length `n_t`.
-        The functions should take a single floating point
-        as an input representing the time in microseconds,
-        and return a real or complex floating point value represent an
-        electric field in V/m at that time.
-        Return type of each function must be the same for all inputs t.
-    t_eval: numpy.ndarray
-        Array of times to sample the integration at.
-        This array must have dtype of float64.
-    init_cond: numpy.ndarray
-        Matrix of shape `(*l, n)` representing the initial state of the system.
-    **kwargs: dict:
-        Additional keyword arguments passed to the cyrk_ode.
-
-    Returns
-    -------
-    numpy.ndarray
-        The matrix solution of shape `(*l,n,n_t)`
-        representing the density matrix of the system at each time t.
-
-    Raises
-    ------
-    OverflowError: If system size exceeds cyrk backend limit of 65535 equations.
-        If we see this error a lot, consider getting CyRK project to increase it
-        by changing type of `y_size` from unisgned short.
-    """  # noqa
-
-    if init_cond.size > np.iinfo(np.ushort).max:
-        raise OverflowError(f'Max system size exceeded for cyrk backend. '
-                            f'({init_cond.size:d}>{np.iinfo(np.ushort).max:d}) '
-                            'Use n_slices to break system into smaller chunks.')
-
-    to_compile = [not nb.extending.is_jitted(f) for f in time_inputs]
-    complex_out = [isinstance(f(0.0), complex) for f in time_inputs]
-    time_inputs_compiled = tuple(nb.njit("c16(f8)", cache=True)(f) if t
-                                 else nb.njit("f8(f8)", cache=True)(f)
-                                 if c else f
-                                 for c,t,f in zip(to_compile,complex_out,time_inputs))
-
-    equations = _derEqns(eoms_base, const_base,
-                         eom_time_r, const_r,
-                         eom_time_i, const_i,
-                         time_inputs_compiled
-                         )
-
-    sol_shape = eoms_base.shape[:-1]
-    with warnings.catch_warnings():
-        # ignore first-class function warning
-        warnings.simplefilter("ignore", category=nb.NumbaExperimentalFeatureWarning)
-        cy_times, cy_sols, cy_success, cy_message = cyrk_ode(equations, (t_eval[0], t_eval[-1]),
-                                                             init_cond.ravel(),
-                                                             t_eval=t_eval,
-                                                             **kwargs)
-
-    return cy_sols.reshape(sol_shape+(cy_sols.shape[-1],))
-
-
-def _derEqns(obes_base: np.ndarray, const_base: np.ndarray,
-             obes_time_r: np.ndarray, const_r: np.ndarray,
-             obes_time_i: np.ndarray, const_i: np.ndarray,
-             time_inputs: Tuple[Callable[[float], Union[float, complex]]]
-             ) -> Callable[[float, np.ndarray, np.ndarray], None]:
-    """
-    Function to build the callable passed to CyRK's cyrk_ode cython solver.
-
-    Note that `time_inputs` functions must be njit compiled.
-
-    Uses the base and time matrix components of the eoms to build
-    a function of vector and scalar time
-    that has the expected input/output of functions passed to `cyrk.cyrk_ode()`
-    """
-
-    t_func_num = obes_time_r.shape[0]
-    input_shape = obes_base.shape[:-1]
-    stack_shape = obes_base.shape[:-2]
-
-    @nb.njit
-    def func(t: float, A_flat: np.ndarray, result_out: np.ndarray):
-
-        # create OBEs at time t
-        obe_total = obes_base.copy()
-        const_total = const_base.copy()
-
-        for idx in range(t_func_num):
-            ti = time_inputs[idx](t)
-            obe_total += ti.real*obes_time_r[idx] + ti.imag*obes_time_i[idx]
-            const_total += ti.real*const_r[idx] + ti.imag*const_i[idx]
-
-        # reshape input to stack shape
-        A_stack = A_flat.reshape(input_shape)
-        result = np.empty_like(A_stack)
-        # matrix multiply obes with input for each parameter of stack
-        for sidx in np.ndindex(stack_shape):
-            result[sidx] = np.dot(obe_total[sidx], A_stack[sidx])
-        # add const values, note: uses broadcasting to handle doppler axis
-        result += const_total
-        # load stacked result into flat output array
-        for i, v in enumerate(result.flat):
-            result_out[i] = v
-
-    return func
+import warnings
+
+import numpy as np
+import numba as nb
+
+from CyRK import cyrk_ode
+
+from typing import Sequence, Callable, Union, Tuple
+
+
+def cyrk_solve(eoms_base: np.ndarray, const_base: np.ndarray,
+               eom_time_r: np.ndarray, const_r: np.ndarray,
+               eom_time_i: np.ndarray, const_i: np.ndarray,
+               time_inputs: Sequence[Callable[[float], Union[float, complex]]],
+               t_eval: np.ndarray, init_cond: np.ndarray,
+               **kwargs
+               ) -> np.ndarray:
+    """
+    Solve a set of Optical Bloch Equations (OBEs) with rydiqule's time solving convention using CyRK's `cyrk_ode`.
+
+    Uses matrix components of the equations of motion provided by the methods of a :meth:`~.Sensor`.
+    Designed to be used as a wrapped function within :func:`~.timesolvers.solve_time`.
+    Builds and solves equations of motion according rydiqule's time solving conventions.
+    Sets up and solves dx/dt = A(t)x + b(t)
+
+    Args
+    ----
+    eoms_base: numpy.ndarray
+        The matrix of shape `(*l,n,n)` representing the non time-varying portion of the matrix A
+        in the equations of motion.
+    const_base: numpy.ndarray
+        The array of shape `(*l, n)` representing the non time-varying portion of the vector b in the
+        equations of motion.
+    eoms_time_r: numpy.ndarraynumpy
+        The matrix of shape `(n_t, *l, n, n)` representing the real time-varying portion of the matrix A,
+        where n_t is the length of `time_inputs`.
+        The ith slice along the first axis should be multiplied by the real part
+        of the ith entry in `time_inputs`.
+    const_r: numpy.nd_array
+        The matrix of shape `(n_t, *l, n)` representing the real time-varying portion of the vector b,
+        where n_t is the length of `time_inputs`.
+        The ith slice along the first axis should be multiplied by the real part
+        of the ith entry in `time_inputs`.
+    eoms_time_i: numpy.ndarray
+        The matrix of shape `(n_t, *l, n, n)` representing the imaginary time-varying portion of the matrix A,
+        where n_t is the length of `time_inputs`.
+        The ith slice along the first axis should be multiplied by the imaginary part
+        of the ith entry in `time_inputs`.
+    const_i: numpy.nd_array
+        The matrix of shape `(n_t, *l, n)` representing the imaginary time-varying portion of the vector b,
+        where n_t is the length of `time_inputs`.
+        The ith slice along the first axis should be multiplied by the imaginary part
+        of the ith entry in `time_inputs`.
+    time_inputs: list(callable)
+        List of callable functions of length `n_t`. The functions should take a single floating point
+        as an input representing the time in microseconds,
+        and return a real or complex floating point value represent an
+        electric field in V/m at that time.
+        Return type of each function must be the same for all inputs t.
+    t_eval: numpy.ndarray
+        Array of times to sample the integration at.
+        This array must have dtype of float64.
+    init_cond: numpy.ndarray
+        Matrix of shape `(*l, n)` representing the initial state of the system.
+    **kwargs: dict:
+        Additional keyword arguments passed to the cyrk_ode.
+
+    Returns
+    -------
+    numpy.ndarray
+        The matrix solution of shape `(*l,n,n_t)`
+        representing the density matrix of the system at each time t.
+
+    Raises
+    ------
+    OverflowError: If system size exceeds cyrk backend limit of 65535 equations.
+        If we see this error a lot, consider getting CyRK project to increase it
+        by changing type of `y_size` from unisgned short.
+    """
+
+    if init_cond.size > np.iinfo(np.ushort).max:
+        raise OverflowError(f'Max system size exceeded for cyrk backend. '
+                            f'({init_cond.size:d}>{np.iinfo(np.ushort).max:d}) '
+                            'Use n_slices to break system into smaller chunks.')
+
+    to_compile = [not nb.extending.is_jitted(f) for f in time_inputs]
+    complex_out = [isinstance(f(0.0), complex) for f in time_inputs]
+    time_inputs_compiled = tuple(nb.njit("c16(f8)", cache=True)(f) if t
+                                 else nb.njit("f8(f8)", cache=True)(f)
+                                 if c else f
+                                 for c,t,f in zip(to_compile,complex_out,time_inputs))
+
+    equations = _derEqns(eoms_base, const_base,
+                         eom_time_r, const_r,
+                         eom_time_i, const_i,
+                         time_inputs_compiled
+                         )
+
+    sol_shape = eoms_base.shape[:-1]
+    with warnings.catch_warnings():
+        # ignore first-class function warning
+        warnings.simplefilter("ignore", category=nb.NumbaExperimentalFeatureWarning)
+        cy_times, cy_sols, cy_success, cy_message = cyrk_ode(equations, (t_eval[0], t_eval[-1]),
+                                                             init_cond.ravel(),
+                                                             t_eval=t_eval,
+                                                             **kwargs)
+
+    return cy_sols.reshape(sol_shape+(cy_sols.shape[-1],))
+
+
+def _derEqns(obes_base: np.ndarray, const_base: np.ndarray,
+             obes_time_r: np.ndarray, const_r: np.ndarray,
+             obes_time_i: np.ndarray, const_i: np.ndarray,
+             time_inputs: Tuple[Callable[[float], Union[float, complex]]]
+             ) -> Callable[[float, np.ndarray, np.ndarray], None]:
+    """
+    Function to build the callable passed to CyRK's cyrk_ode cython solver.
+
+    Note that `time_inputs` functions must be njit compiled.
+
+    Uses the base and time matrix components of the eoms to build
+    a function of vector and scalar time
+    that has the expected input/output of functions passed to `cyrk.cyrk_ode()`
+    """
+
+    t_func_num = obes_time_r.shape[0]
+    input_shape = obes_base.shape[:-1]
+    stack_shape = obes_base.shape[:-2]
+
+    @nb.njit
+    def func(t: float, A_flat: np.ndarray, result_out: np.ndarray):
+
+        # create OBEs at time t
+        obe_total = obes_base.copy()
+        const_total = const_base.copy()
+
+        for idx in range(t_func_num):
+            ti = time_inputs[idx](t)
+            obe_total += ti.real*obes_time_r[idx] + ti.imag*obes_time_i[idx]
+            const_total += ti.real*const_r[idx] + ti.imag*const_i[idx]
+
+        # reshape input to stack shape
+        A_stack = A_flat.reshape(input_shape)
+        result = np.empty_like(A_stack)
+        # matrix multiply obes with input for each parameter of stack
+        for sidx in np.ndindex(stack_shape):
+            result[sidx] = np.dot(obe_total[sidx], A_stack[sidx])
+        # add const values, note: uses broadcasting to handle doppler axis
+        result += const_total
+        # load stacked result into flat output array
+        for i, v in enumerate(result.flat):
+            result_out[i] = v
+
+    return func
```

### Comparing `rydiqule-1.0.0/src/rydiqule/stack_solvers/nbkode_solver.py` & `rydiqule-1.0.0rc2/src/rydiqule/stack_solvers/nbkode_solver.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,146 +1,144 @@
-import warnings
-
-import numpy as np
-import numba as nb
-import nbkode
-from numba import NumbaExperimentalFeatureWarning
-
-from typing import Sequence, Tuple, Callable, Union
-
-
-def nbkode_solve(eoms_base: np.ndarray, const_base: np.ndarray,
-                 eom_time_r: np.ndarray, const_r: np.ndarray,
-                 eom_time_i: np.ndarray, const_i: np.ndarray,
-                 time_inputs: Sequence[Callable[[float], Union[float, complex]]],
-                 t_eval: np.ndarray, init_cond: np.ndarray, **kwargs
-                 ) -> np.ndarray:
-    """
-    Solve a set of Optical Bloch Equations (OBEs) using rydiqule's time solving convention using
-    :doc:`numbakit-ode <numbakitode:index>`.
-
-    Uses matrix components of the equations of motion provided by the methods of a :meth:`~.Sensor`.
-    Designed to be used as a wrapped function within :func:`~.timesolvers.solve_time`.
-    Builds and solves equations of motion according rydiqule's time solving conventions.
-    Sets up and solves dx/dt = A(t)x + b(t)
-
-    Args
-    ----
-    eoms_base: numpy.ndarray
-        The matrix of shape `(*l,n,n)` representing the non time-varying portion of the matrix A
-        in the equations of motion.
-    const: numpy.ndarray
-        The array of shape `(*l, n)` representing the non time-varying portion of the vector b in the
-        equations of motion.
-    eoms_time_r: numpy.ndarraynumpy
-        The matrix of shape `(n_t, *l, n, n)` representing the real time-varying portion of the matrix A,
-        where n_t is the length of `time_inputs`.
-        The ith slice along the first axis should be multiplied by the real part
-        of the ith entry in `time_inputs`.
-    const_r: numpy.nd_array
-        The matrix of shape `(n_t, *l, n)` representing the real time-varying portion of the vector b,
-        where n_t is the length of `time_inputs`.
-        The ith slice along the first axis should be multiplied by the real part
-        of the ith entry in `time_inputs`.
-    eoms_time_i: numpy.ndarray
-        The matrix of shape `(n_t, *l, n, n)` representing the imaginary time-varying portion of the matrix A,
-        where n_t is the length of `time_inputs`.
-        The ith slice along the first axis should be multiplied by the imaginary part
-        of the ith entry in `time_inputs`.
-    const_i: numpy.nd_array
-        The matrix of shape `(n_t, *l, n)` representing the imaginary time-varying portion of the vector b,
-        where n_t is the length of `time_inputs`.
-        The ith slice along the first axis should be multiplied by the imaginary part
-        of the ith entry in `time_inputs`.
-    time_inputs: list(callable)
-        List of callable functions of length `n_t`.
-        The functions should take a single floating point
-        as an input representing the time in microseconds,
-        and return a real or complex floating point value represent an
-        electric field in V/m at that time.
-        Return type of each function must be the same for all inputs t.
-    t_eval: numpy.ndarray
-        Array of times to sample the integration at.
-        This array must have dtype of float64.
-    init_cond: (numpy.ndarray)
-        Matrix of shape `(*l, n)` representing the initial state of the system.
-    **kwargs: dict
-        Additional keyword arguments passed to the nbkode solver constructor.
-
-    Returns
-    -------
-    numpy.ndarray
-        The matrix solution of shape `(*l,n,n_t)`
-        representing the density matrix of the system at each time t.
-    """  # noqa
-
-    # numbakit-ode requires all functions to be of same type
-    to_compile = [not nb.extending.is_jitted(f) for f in time_inputs]
-    complex_out = any([isinstance(f(0.0), complex) for f in time_inputs])
-
-    time_inputs_compiled = tuple(nb.njit("c16(f8)", cache=True)(f) if complex_out
-                                 else nb.njit("f8(f8)", cache=True)(f)
-                                 if c else f
-                                 for c,f in zip(to_compile,time_inputs))
-
-    equations = _derEqns(eoms_base, const_base,
-                         eom_time_r, const_r,
-                         eom_time_i, const_i,
-                         time_inputs_compiled
-                         )
-
-    sol_shape = eoms_base.shape[:-1]
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore", category=NumbaExperimentalFeatureWarning)
-        solver = nbkode.RungeKutta45(equations, t_eval[0],
-                                     init_cond.ravel(),
-                                     rtol=kwargs.pop("rtol",1e-6), **kwargs)
-        _, ys = solver.run(t_eval)
-        sol_flat = np.transpose(ys)
-
-    return sol_flat.reshape(sol_shape+(sol_flat.shape[-1],))
-
-
-def _derEqns(obes_base: np.ndarray, const_base: np.ndarray,
-             obes_time_r: np.ndarray, const_r: np.ndarray,
-             obes_time_i: np.ndarray,  const_i: np.ndarray,
-             time_inputs: Tuple[Callable[[float], Union[float, complex]]]
-             ) -> Callable[[float, np.ndarray], np.ndarray]:
-    """
-    Function to build the callable passed to nbkode numba solver.
-
-    Note that `time_inputs` functions must be njit compiled.
-
-    Uses the base and time matrix components of the eoms to build
-    a function of vector and scalar time
-    that has the expected input/output of functions passed to `nbkode.solver()`
-    """
-
-    t_func_num = obes_time_r.shape[0]
-    input_shape = obes_base.shape[:-1]
-    stack_shape = obes_base.shape[:-2]
-
-    @nb.njit
-    def func(t: float, A_flat: np.ndarray):
-
-        # create OBEs at time t
-        obe_total = obes_base.copy()
-        const_total = const_base.copy()
-
-        for idx in range(t_func_num):
-            ti = time_inputs[idx](t)
-            obe_total += ti.real*obes_time_r[idx] + ti.imag*obes_time_i[idx]
-            const_total += ti.real*const_r[idx] + ti.imag*const_i[idx]
-
-        # reshape input to stack shape
-        A_stack = A_flat.reshape(input_shape)
-        result = np.empty_like(A_stack)
-        # matrix multiply obes with input for each parameter of stack
-        for sidx in np.ndindex(stack_shape):
-            A = A_stack[sidx]
-            result[sidx] = np.dot(obe_total[sidx], A)
-        # add const values, note: uses broadcasting to handle doppler axis
-        result += const_total
-        # flatten output
-        return np.ravel(result)
-
-    return func
+import warnings
+
+import numpy as np
+import numba as nb
+import nbkode
+from numba import NumbaExperimentalFeatureWarning
+
+from typing import Sequence, Tuple, Callable, Union
+
+
+def nbkode_solve(eoms_base: np.ndarray, const_base: np.ndarray,
+                 eom_time_r: np.ndarray, const_r: np.ndarray,
+                 eom_time_i: np.ndarray, const_i: np.ndarray,
+                 time_inputs: Sequence[Callable[[float], Union[float, complex]]],
+                 t_eval: np.ndarray, init_cond: np.ndarray, **kwargs
+                 ) -> np.ndarray:
+    """
+    Solve a set of Optical Bloch Equations (OBEs) using rydiqule's time solving convention using :doc:`numbakit-ode <numbakitode:index>`.
+
+    Uses matrix components of the equations of motion provided by the methods of a :meth:`~.Sensor`.
+    Designed to be used as a wrapped function within :func:`~.timesolvers.solve_time`.
+    Builds and solves equations of motion according rydiqule's time solving conventions.
+    Sets up and solves dx/dt = A(t)x + b(t)
+
+    Args
+    ----
+    eoms_base: numpy.ndarray
+        The matrix of shape `(*l,n,n)` representing the non time-varying portion of the matrix A
+        in the equations of motion.
+    const: numpy.ndarray
+        The array of shape `(*l, n)` representing the non time-varying portion of the vector b in the
+        equations of motion.
+    eoms_time_r: numpy.ndarraynumpy
+        The matrix of shape `(n_t, *l, n, n)` representing the real time-varying portion of the matrix A,
+        where n_t is the length of `time_inputs`.
+        The ith slice along the first axis should be multiplied by the real part
+        of the ith entry in `time_inputs`.
+    const_r: numpy.nd_array
+        The matrix of shape `(n_t, *l, n)` representing the real time-varying portion of the vector b,
+        where n_t is the length of `time_inputs`.
+        The ith slice along the first axis should be multiplied by the real part
+        of the ith entry in `time_inputs`.
+    eoms_time_i: numpy.ndarray
+        The matrix of shape `(n_t, *l, n, n)` representing the imaginary time-varying portion of the matrix A,
+        where n_t is the length of `time_inputs`.
+        The ith slice along the first axis should be multiplied by the imaginary part
+        of the ith entry in `time_inputs`.
+    const_i: numpy.nd_array
+        The matrix of shape `(n_t, *l, n)` representing the imaginary time-varying portion of the vector b,
+        where n_t is the length of `time_inputs`.
+        The ith slice along the first axis should be multiplied by the imaginary part
+        of the ith entry in `time_inputs`.
+    time_inputs: list(callable)
+        List of callable functions of length `n_t`. The functions should take a single floating point
+        as an input representing the time in microseconds,
+        and return a real or complex floating point value represent an
+        electric field in V/m at that time.
+        Return type of each function must be the same for all inputs t.
+    t_eval: numpy.ndarray
+        Array of times to sample the integration at.
+        This array must have dtype of float64.
+    init_cond: (numpy.ndarray)
+        Matrix of shape `(*l, n)` representing the initial state of the system.
+    **kwargs: dict
+        Additional keyword arguments passed to the nbkode solver constructor.
+
+    Returns
+    -------
+    numpy.ndarray
+        The matrix solution of shape `(*l,n,n_t)`
+        representing the density matrix of the system at each time t.
+    """
+
+    # numbakit-ode requires all functions to be of same type
+    to_compile = [not nb.extending.is_jitted(f) for f in time_inputs]
+    complex_out = any([isinstance(f(0.0), complex) for f in time_inputs])
+
+    time_inputs_compiled = tuple(nb.njit("c16(f8)", cache=True)(f) if complex_out
+                                 else nb.njit("f8(f8)", cache=True)(f)
+                                 if c else f
+                                 for c,f in zip(to_compile,time_inputs))
+
+    equations = _derEqns(eoms_base, const_base,
+                         eom_time_r, const_r,
+                         eom_time_i, const_i,
+                         time_inputs_compiled
+                         )
+
+    sol_shape = eoms_base.shape[:-1]
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", category=NumbaExperimentalFeatureWarning)
+        solver = nbkode.RungeKutta45(equations, t_eval[0],
+                                     init_cond.ravel(),
+                                     rtol=kwargs.pop("rtol",1e-6), **kwargs)
+        _, ys = solver.run(t_eval)
+        sol_flat = np.transpose(ys)
+
+    return sol_flat.reshape(sol_shape+(sol_flat.shape[-1],))
+
+
+def _derEqns(obes_base: np.ndarray, const_base: np.ndarray,
+             obes_time_r: np.ndarray, const_r: np.ndarray,
+             obes_time_i: np.ndarray,  const_i: np.ndarray,
+             time_inputs: Tuple[Callable[[float], Union[float, complex]]]
+             ) -> Callable[[float, np.ndarray], np.ndarray]:
+    """
+    Function to build the callable passed to nbkode numba solver.
+
+    Note that `time_inputs` functions must be njit compiled.
+
+    Uses the base and time matrix components of the eoms to build
+    a function of vector and scalar time
+    that has the expected input/output of functions passed to `nbkode.solver()`
+    """
+
+    t_func_num = obes_time_r.shape[0]
+    input_shape = obes_base.shape[:-1]
+    stack_shape = obes_base.shape[:-2]
+
+    @nb.njit
+    def func(t: float, A_flat: np.ndarray):
+
+        # create OBEs at time t
+        obe_total = obes_base.copy()
+        const_total = const_base.copy()
+
+        for idx in range(t_func_num):
+            ti = time_inputs[idx](t)
+            obe_total += ti.real*obes_time_r[idx] + ti.imag*obes_time_i[idx]
+            const_total += ti.real*const_r[idx] + ti.imag*const_i[idx]
+
+        # reshape input to stack shape
+        A_stack = A_flat.reshape(input_shape)
+        result = np.empty_like(A_stack)
+        # matrix multiply obes with input for each parameter of stack
+        for sidx in np.ndindex(stack_shape):
+            A = A_stack[sidx]
+            result[sidx] = np.dot(obe_total[sidx], A)
+        # add const values, note: uses broadcasting to handle doppler axis
+        result += const_total
+        # flatten output
+        return np.ravel(result)
+
+    return func
```

### Comparing `rydiqule-1.0.0/src/rydiqule/stack_solvers/nbrk_solver.py` & `rydiqule-1.0.0rc2/src/rydiqule/stack_solvers/nbrk_solver.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,144 +1,142 @@
-import warnings
-
-import numpy as np
-import numba as nb
-
-from CyRK import nbrk_ode
-
-from typing import Sequence, Callable, Union, Tuple
-
-
-def nbrk_solve(eoms_base: np.ndarray, const_base: np.ndarray,
-               eom_time_r: np.ndarray, const_r: np.ndarray,
-               eom_time_i: np.ndarray, const_i: np.ndarray,
-               time_inputs: Sequence[Callable[[float], Union[float, complex]]],
-               t_eval: np.ndarray, init_cond: np.ndarray, **kwargs
-               ) -> np.ndarray:
-    """
-    Solve a set of Optical Bloch Equations (OBEs) with rydiqule's time solving convention
-    using CyRK's `nbrk_ode`.
-
-    Uses matrix components of the equations of motion provided by the methods of a :meth:`~.Sensor`.
-    Designed to be used as a wrapped function within :func:`~.timesolvers.solve_time`.
-    Builds and solves equations of motion according rydiqule's time solving conventions.
-    Sets up and solves dx/dt = A(t)x + b(t)
-
-    Args
-    ----
-    eoms_base: numpy.ndarray
-        The matrix of shape `(*l,n,n)` representing the non time-varying portion of the matrix A
-        in the equations of motion.
-    const: numpy.ndarray
-        The array of shape `(*l, n)` representing the non time-varying portion of the vector b in the
-        equations of motion.
-    eoms_time_r: numpy.ndarraynumpy
-        The matrix of shape `(n_t, *l, n, n)` representing the real time-varying portion of the matrix A,
-        where n_t is the length of `time_inputs`.
-        The ith slice along the first axis should be multiplied by the real part
-        of the ith entry in `time_inputs`.
-    const_r: numpy.nd_array
-        The matrix of shape `(n_t, *l, n)` representing the real time-varying portion of the vector b,
-        where n_t is the length of `time_inputs`.
-        The ith slice along the first axis should be multiplied by the real part
-        of the ith entry in `time_inputs`.
-    eoms_time_i: numpy.ndarray
-        The matrix of shape `(n_t, *l, n, n)` representing the imaginary time-varying portion of the matrix A,
-        where n_t is the length of `time_inputs`.
-        The ith slice along the first axis should be multiplied by the imaginary part
-        of the ith entry in `time_inputs`.
-    const_i: numpy.nd_array
-        The matrix of shape `(n_t, *l, n)` representing the imaginary time-varying portion of the vector b,
-        where n_t is the length of `time_inputs`.
-        The ith slice along the first axis should be multiplied by the imaginary part
-        of the ith entry in `time_inputs`.
-    time_inputs: list(callable)
-        List of callable functions of length `n_t`.
-        The functions should take a single floating point
-        as an input representing the time in microseconds,
-        and return a real or complex floating point value represent an
-        electric field in V/m at that time.
-        Return type of each function must be the same for all inputs t.
-    t_eval: numpy.ndarray
-        Array of times to sample the integration at.
-        This array must have dtype of float64.
-    init_cond: (numpy.ndarray)
-        Matrix of shape `(*l, n)` representing the initial state of the system.
-    **kwargs: dict
-        Additional keyword arguments passed to nbrk_ode.
-
-    Returns
-    -------
-    numpy.ndarray
-        The matrix solution of shape `(*l,n,n_t)`
-        representing the density matrix of the system at each time t.
-    """  # noqa
-
-    to_compile = [not nb.extending.is_jitted(f) for f in time_inputs]
-    complex_out = [isinstance(f(0.0), complex) for f in time_inputs]
-    time_inputs_compiled = tuple(nb.njit("c16(f8)", cache=True)(f) if t
-                                 else nb.njit("f8(f8)", cache=True)(f)
-                                 if c else f
-                                 for c,t,f in zip(to_compile,complex_out,time_inputs))
-
-    equations = _derEqns(eoms_base, const_base,
-                         eom_time_r, const_r,
-                         eom_time_i, const_i,
-                         time_inputs_compiled
-                         )
-
-    sol_shape = eoms_base.shape[:-1]
-    with warnings.catch_warnings():
-        # ignore first-class function warning
-        warnings.simplefilter("ignore", category=nb.NumbaExperimentalFeatureWarning)
-        nb_times, nb_sols, nb_success, nb_message = nbrk_ode(equations, (t_eval[0], t_eval[-1]),
-                                                             init_cond.ravel(),
-                                                             t_eval=t_eval,
-                                                             **kwargs)
-
-    return nb_sols.reshape(sol_shape+(nb_sols.shape[-1],))
-
-
-def _derEqns(obes_base: np.ndarray, const_base: np.ndarray,
-             obes_time_r: np.ndarray, const_r: np.ndarray,
-             obes_time_i: np.ndarray,  const_i: np.ndarray,
-             time_inputs: Tuple[Callable[[float], Union[float, complex]]]
-             ) -> Callable[[float, np.ndarray], np.ndarray]:
-    """
-    Function to build the callable passed to CyRK's nbrk_ode numba solver.
-
-    Note that `time_inputs` functions must be njit compiled.
-
-    Uses the base and time matrix components of the eoms to build
-    a function of vector and scalar time
-    that has the expected input/output of functions passed to `cyrk.nbrk_ode()`
-    """
-
-    t_func_num = obes_time_r.shape[0]
-    input_shape = obes_base.shape[:-1]
-    stack_shape = obes_base.shape[:-2]
-
-    @nb.njit
-    def func(t: float, A_flat: np.ndarray):
-
-        # create OBEs at time t
-        obe_total = obes_base.copy()
-        const_total = const_base.copy()
-
-        for idx in range(t_func_num):
-            ti = time_inputs[idx](t)
-            obe_total += ti.real*obes_time_r[idx] + ti.imag*obes_time_i[idx]
-            const_total += ti.real*const_r[idx] + ti.imag*const_i[idx]
-
-        # reshape input to stack shape
-        A_stack = A_flat.reshape(input_shape)
-        result = np.empty_like(A_stack)
-        # matrix multiply obes with input for each parameter of stack
-        for sidx in np.ndindex(stack_shape):
-            A = A_stack[sidx]
-            result[sidx] = np.dot(obe_total[sidx], A)
-        # add const values, note: uses broadcasting to handle doppler axis
-        result += const_total
-        # flatten output
-        return np.ravel(result)
-
-    return func
+import warnings
+
+import numpy as np
+import numba as nb
+
+from CyRK import nbrk_ode
+
+from typing import Sequence, Callable, Union, Tuple
+
+
+def nbrk_solve(eoms_base: np.ndarray, const_base: np.ndarray,
+               eom_time_r: np.ndarray, const_r: np.ndarray,
+               eom_time_i: np.ndarray, const_i: np.ndarray,
+               time_inputs: Sequence[Callable[[float], Union[float, complex]]],
+               t_eval: np.ndarray, init_cond: np.ndarray, **kwargs
+               ) -> np.ndarray:
+    """
+    Solve a set of Optical Bloch Equations (OBEs) with rydiqule's time solving convention using CyRK's `nbrk_ode`.
+
+    Uses matrix components of the equations of motion provided by the methods of a :meth:`~.Sensor`.
+    Designed to be used as a wrapped function within :func:`~.timesolvers.solve_time`.
+    Builds and solves equations of motion according rydiqule's time solving conventions.
+    Sets up and solves dx/dt = A(t)x + b(t)
+
+    Args
+    ----
+    eoms_base: numpy.ndarray
+        The matrix of shape `(*l,n,n)` representing the non time-varying portion of the matrix A
+        in the equations of motion.
+    const: numpy.ndarray
+        The array of shape `(*l, n)` representing the non time-varying portion of the vector b in the
+        equations of motion.
+    eoms_time_r: numpy.ndarraynumpy
+        The matrix of shape `(n_t, *l, n, n)` representing the real time-varying portion of the matrix A,
+        where n_t is the length of `time_inputs`.
+        The ith slice along the first axis should be multiplied by the real part
+        of the ith entry in `time_inputs`.
+    const_r: numpy.nd_array
+        The matrix of shape `(n_t, *l, n)` representing the real time-varying portion of the vector b,
+        where n_t is the length of `time_inputs`.
+        The ith slice along the first axis should be multiplied by the real part
+        of the ith entry in `time_inputs`.
+    eoms_time_i: numpy.ndarray
+        The matrix of shape `(n_t, *l, n, n)` representing the imaginary time-varying portion of the matrix A,
+        where n_t is the length of `time_inputs`.
+        The ith slice along the first axis should be multiplied by the imaginary part
+        of the ith entry in `time_inputs`.
+    const_i: numpy.nd_array
+        The matrix of shape `(n_t, *l, n)` representing the imaginary time-varying portion of the vector b,
+        where n_t is the length of `time_inputs`.
+        The ith slice along the first axis should be multiplied by the imaginary part
+        of the ith entry in `time_inputs`.
+    time_inputs: list(callable)
+        List of callable functions of length `n_t`. The functions should take a single floating point
+        as an input representing the time in microseconds,
+        and return a real or complex floating point value represent an
+        electric field in V/m at that time.
+        Return type of each function must be the same for all inputs t.
+    t_eval: numpy.ndarray
+        Array of times to sample the integration at.
+        This array must have dtype of float64.
+    init_cond: (numpy.ndarray)
+        Matrix of shape `(*l, n)` representing the initial state of the system.
+    **kwargs: dict
+        Additional keyword arguments passed to nbrk_ode.
+
+    Returns
+    -------
+    numpy.ndarray
+        The matrix solution of shape `(*l,n,n_t)`
+        representing the density matrix of the system at each time t.
+    """
+
+    to_compile = [not nb.extending.is_jitted(f) for f in time_inputs]
+    complex_out = [isinstance(f(0.0), complex) for f in time_inputs]
+    time_inputs_compiled = tuple(nb.njit("c16(f8)", cache=True)(f) if t
+                                 else nb.njit("f8(f8)", cache=True)(f)
+                                 if c else f
+                                 for c,t,f in zip(to_compile,complex_out,time_inputs))
+
+    equations = _derEqns(eoms_base, const_base,
+                         eom_time_r, const_r,
+                         eom_time_i, const_i,
+                         time_inputs_compiled
+                         )
+
+    sol_shape = eoms_base.shape[:-1]
+    with warnings.catch_warnings():
+        # ignore first-class function warning
+        warnings.simplefilter("ignore", category=nb.NumbaExperimentalFeatureWarning)
+        nb_times, nb_sols, nb_success, nb_message = nbrk_ode(equations, (t_eval[0], t_eval[-1]),
+                                                             init_cond.ravel(),
+                                                             t_eval=t_eval,
+                                                             **kwargs)
+
+    return nb_sols.reshape(sol_shape+(nb_sols.shape[-1],))
+
+
+def _derEqns(obes_base: np.ndarray, const_base: np.ndarray,
+             obes_time_r: np.ndarray, const_r: np.ndarray,
+             obes_time_i: np.ndarray,  const_i: np.ndarray,
+             time_inputs: Tuple[Callable[[float], Union[float, complex]]]
+             ) -> Callable[[float, np.ndarray], np.ndarray]:
+    """
+    Function to build the callable passed to CyRK's nbrk_ode numba solver.
+
+    Note that `time_inputs` functions must be njit compiled.
+
+    Uses the base and time matrix components of the eoms to build
+    a function of vector and scalar time
+    that has the expected input/output of functions passed to `cyrk.nbrk_ode()`
+    """
+
+    t_func_num = obes_time_r.shape[0]
+    input_shape = obes_base.shape[:-1]
+    stack_shape = obes_base.shape[:-2]
+
+    @nb.njit
+    def func(t: float, A_flat: np.ndarray):
+
+        # create OBEs at time t
+        obe_total = obes_base.copy()
+        const_total = const_base.copy()
+
+        for idx in range(t_func_num):
+            ti = time_inputs[idx](t)
+            obe_total += ti.real*obes_time_r[idx] + ti.imag*obes_time_i[idx]
+            const_total += ti.real*const_r[idx] + ti.imag*const_i[idx]
+
+        # reshape input to stack shape
+        A_stack = A_flat.reshape(input_shape)
+        result = np.empty_like(A_stack)
+        # matrix multiply obes with input for each parameter of stack
+        for sidx in np.ndindex(stack_shape):
+            A = A_stack[sidx]
+            result[sidx] = np.dot(obe_total[sidx], A)
+        # add const values, note: uses broadcasting to handle doppler axis
+        result += const_total
+        # flatten output
+        return np.ravel(result)
+
+    return func
```

### Comparing `rydiqule-1.0.0/src/rydiqule/timesolvers.py` & `rydiqule-1.0.0rc2/src/rydiqule/timesolvers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,384 +1,368 @@
-"""
-Solvers for time domain analysis with an arbitrary RF field
-"""
-
-import numpy as np
-from importlib.metadata import version
-
-from .sensor_utils import _hamiltonian_term, generate_eom, make_real
-from .sensor_solution import Solution
-from .sensor import Sensor  # only needing for type hinting
-from .slicing.slicing import matrix_slice, get_slice_num_t
-
-from rydiqule.solvers import solve_steady_state
-from rydiqule.doppler_utils import *
-from rydiqule.stack_solvers.scipy_solver import scipy_solve
-from rydiqule.stack_solvers.nbkode_solver import nbkode_solve
-from rydiqule.stack_solvers.cyrk_solver import cyrk_solve
-from rydiqule.stack_solvers.nbrk_solver import nbrk_solve
-
-from typing import Optional, Tuple, Iterable, List, Callable, Literal, Union
-
-stack_solvers = {"scipy": scipy_solve,
-                 "nbkode": nbkode_solve,
-                 "cyrk": cyrk_solve,
-                 "nbrk": nbrk_solve}
-
-solver_type = Union[Callable, Literal['scipy', 'nbkode', 'cyrk', 'nbrk']]
-
-def solve_time(sensor: Sensor, end_time: float, num_pts: int,
-               init_cond: Optional[np.ndarray] = None, doppler: bool = False,
-               doppler_mesh_method: Optional[MeshMethod] = None, sum_doppler: bool = True,
-               n_slices: Union[int, None] = None, solver: solver_type = "scipy",
-               **kwargs) -> Solution:
-    """
-    Solves the response of the optical sensor in the time domain given the its time-dependent inputs
-    
-    If insuffucent system memory is available to solve the system all at once, 
-    system is broken into "slices" of manageable memory footprint which are solved indivudually. 
-    This slicing behavior does not affect the result.
-    All couplings that include a "time_dependence" argument will be solved in the time domain. 
-    
-    A number of solver backends work with rydiqule, but the default `"scipy"` ivp solver is the
-    is recommended backend in almost all cases, as it is the most fully-featured and
-    documented. Advanced users have the ablity to define their own solver backends
-    by creating a function that follows the call signature for rydiqule timesolver
-    backends. Additional arguments to the solver backend can be supplied with `**kwargs`.
-    
-    Parameters
-    -----------
-    sensor : :class:`~.Sensor`
-        The sensor object representing the atomic/laser arrangement of the system.
-    end_time : float  
-        Amount of time, in microseconds, for which to simulate the system
-    num_pts : int
-        The number of points along the range `(0, end_time)` for which
-        the solution is evaluated. This does not affect the number of funtion
-        evaluations during the solve, rather the spacing of the points in 
-        the reported solution.
-    init_cond : numpy.ndarray or `None`, optional 
-        Density matrix representing the initial state of the system. 
-        If specified, the shape should be either `(n)` in the case of a single
-        initial condition for all parameter values, or should be of shape `(*l, n)`
-        matching the output shape of a steady state solve if the initial condition
-        may be different for different combinations of parameters. 
-        If `None`, will solve the problem in the steady state with all time-dependent fields
-        "off" and use the solution as the initial condition for the time behavior. Other
-        possible manual options might include a matrix populated by zeros representing the
-        entire population in the ground state. Defaults to `None`.
-    doppler : bool, optional
-        Whether to account for doppler shift among moving atoms in
-        the gas. If True, the solver will implicitly define a velocity distribution
-        for particles in the cell, solve the problem for each velocity class,
-        and return a weighted average of the results. Note that solving in this
-        manner carries a substantial performance penalty, as each doppler velocity class
-        is solved as its own problem. If solved with doppler, only axis specified by a `"kvec"'
-        argument in one of the sensor couplings will be average over. The time solver currently 
-        supports doppler averaging in any number of spatial dimensions, up to the limit of 
-        3 imposed by the macroscopic physical world. Defaults to `False`.
-    doppler_mesh_method : dict, optional
-        Dictionary that controls the doppler meshing method. Exact details of this are
-        found in the documentation of :func:`~doppler_classes`. Ignored if 
-        `doppler=False`. Default is `None`.
-    sum_doppler : bool, optional
-        Whether to average over doppler classes after the solve
-        is complete. Setting to false will not perform the sum, allowing viewing
-        of the weighted results of the solve for each doppler class. Ignored
-        if `doppler=False`. Default is `True`.
-    n_slices : int or None, optional
-        How many sets of equations to break the full equations into.
-        The actual number of slices will be the largest between this value and the minumum
-        number of slices to solve the system without a memory error. If `None`, solver uses the
-        minimum number of slices required to solve without a `memoryError`. Defaults to None.
-    solver : {"scipy", "nbkode", "cyrk", "nbrk"} or callable
-        The backend solver used to solve the ivp generated by the sensor.
-        All string values correspond to backend solvers built in to rydiqule.
-        Valid string values are:
-
-            - "scipy": Solves equations with :func:`scipy:scipy.integrate.solve_ivp`.
-              The default, most stable, and well-supported option.
-            - "nbkode": Solves equations with the jit-compiled Runge-Kutta-45 solver in
-              :doc:`numbakit-ode <numbakitode:index>`.
-              May be faster for very long time solves with many timesteps.
-            - "cyrk": Solves jit-compiled equations with a cython compiled RK solver from `CyRK`.
-              Due to some jit compilation, only faster for moderate length problems
-              (ie problems with a moderate number of required time steps).
-            - "nbrk": Solves equations with the jit-compiled RK solver from `CyRK`.
-              Due to extensive jit compilation, only faster for very long solves
-              (ie problems with a large number of required time steps).
-
-        Additionally, can be specified with a callable that matches
-        rydiqule's time-solver convention,
-        enabling using a custom solver backend.
-
-        .. note::
-
-            Unless otherwise noted, backends other than scipy are considered experimental.
-            Issues with their use are considered features not fully implemented rather than
-            bugs.
-
-    **kwargs: Additional keyword arguments passed to the backend solver.
-        See documentation of the relevant solver (i.e. :func:`scipy:scipy.integrate.solve_ivp`)
-        for details and supported arguments.
-
-    Returns
-    -------
-    :class:`~.Solution`
-        A bunch-type object contining information about the
-        solution. Timesolver specific attributes are `t`  and `init_cond`,
-        corresponding respectively to the times at which the solution is sampled and
-        the initial conditions used for the solve.
-        
-    """
-    if type(solver) == str:
-        try:
-            solver = stack_solvers[solver]
-        except KeyError:
-            raise ValueError(
-                f"{solver} is not a built-in solver."
-                f" Supported built-in solvers are {list(stack_solvers.keys())}")
-    
-    if not isinstance(solver, Callable):
-        raise ValueError("Solvers must be callable functions")
-    
-    solution = Solution()
-
-    # relevant sensor-related quantities
-    stack_shape = sensor._stack_shape()
-    basis_size = sensor.basis_size
-    spatial_dim = sensor.spatial_dim()
-
-    # set up time parameters
-    time_range = (0.0, end_time)
-    t_eval = np.linspace(*time_range, num=num_pts, dtype=np.float64)
-
-    # initialize doppler-related quantities
-    doppler_axis_shape: Iterable[int] = ()
-    dop_classes = None
-    doppler_shifts = None
-    out_doppler_axes: Iterable[slice] = ()
-    doppler_axes: Iterable[slice] = ()
-
-    # update doppler-related values
-    if doppler:
-        dop_classes = doppler_classes(method=doppler_mesh_method)
-        doppler_shifts = sensor.get_doppler_shifts()
-        doppler_axis_shape = tuple(len(dop_classes) for _ in range(spatial_dim))
-        doppler_axes = tuple(slice(None) for _ in range(spatial_dim))
-
-        if not sum_doppler:
-            out_doppler_axes = doppler_axes
-
-    if init_cond is None:
-        init_cond = solve_steady_state(
-            sensor, doppler=doppler, weight_doppler=False, sum_doppler=False,
-            doppler_mesh_method=doppler_mesh_method
-            ).rho
-
-    # use available memory to figure out how to slice the hamiltonian
-    n_slices, out_sol_shape = get_slice_num_t(basis_size, stack_shape, doppler_axis_shape,
-                                                  num_pts, sum_doppler, n_slices)
-
-    if n_slices > 1:
-        print(f"Breaking equations of motion into {n_slices} sets of equations...")
-
-    # allocate arrays
-    hamiltonians, hamiltonians_time, hamiltonians_time_i = sensor.get_time_hamiltonians()
-    n_time = len(hamiltonians_time)
-    time_functions = sensor.get_time_dependence()
-    gamma = sensor.decoherence_matrix()
-    sols = np.zeros(out_sol_shape, dtype="float64")
-    
-    n_slices_true = sum(1 for _ in matrix_slice(gamma, n_slices=n_slices))
-
-    for i, (idx, H, G, *time_hams), in enumerate(matrix_slice(hamiltonians, gamma,
-                                                              *hamiltonians_time,
-                                                              *hamiltonians_time_i,
-                                                              n_slices=n_slices)):
-        
-        if n_slices_true > 1:
-            print(f"Solving equation slice {i+1}/{n_slices_true}", end='\r')
-            
-        Ht = np.array(time_hams[:n_time])
-        Ht_i = np.array(time_hams[n_time:])
-        
-        full_idx = (*out_doppler_axes, *idx, slice(None))
-        sols[full_idx] = _solve_hamiltonian_stack(H, Ht, Ht_i,
-                                                  G, time_functions, t_eval,
-                                                  init_cond[(*doppler_axes, *idx)], solver,
-                                                  doppler=doppler,
-                                                  dop_classes=dop_classes, sum_doppler=sum_doppler,
-                                                  doppler_shifts=doppler_shifts,
-                                                  spatial_dim=spatial_dim, **kwargs)
-
-    # save results to the Solution
-    solution.rho = sols
-    solution.eta = sensor.eta
-    solution.kappa = sensor.kappa
-    solution.axis_labels = ([f'doppler_{i:d}' for i in range(spatial_dim) if not sum_doppler]
-                            + sensor.axis_labels()
-                            + ["time", "density_matrix"])
-    solution.axis_values = ([dop_classes for i in range(spatial_dim) if not sum_doppler]
-                            + [val for _,_,val in sensor.variable_parameters()]
-                            + [t_eval, sensor.basis()])
-    solution.basis = sensor.basis()
-    solution.rq_version = version("rydiqule")
-    solution.doppler_classes = dop_classes
-    # time solver specific
-    solution.t = t_eval
-    solution.init_cond = init_cond
-
-    return solution
-
-
-def _solve_hamiltonian_stack(hamiltonians_base: np.ndarray, hamiltonians_time: np.ndarray,
-                             hamiltonians_time_i: np.ndarray, gamma_matrix: np.ndarray,
-                             time_functions: List[Callable[[float], float]], t_eval: np.ndarray,
-                             init_cond: np.ndarray, solver, doppler: bool = False,
-                             dop_classes: Optional[np.ndarray] = None, sum_doppler: bool = True,
-                             weight_doppler: bool = True,
-                             doppler_shifts: Optional[np.ndarray] = None,
-                             spatial_dim: int = 0, **kwargs
-                             ) -> np.ndarray:
-
-    """
-    Internal funtions which solve the equations of a given hamiltonian stack 
-    with the given parameters.
-    """
-    eom_base, const = generate_eom(hamiltonians_base, gamma_matrix,
-                                   remove_ground_state=True, real_eom=True)
-    eom_time_r, const_r = generate_eom_time(hamiltonians_time)
-    eom_time_i, const_i = generate_eom_time(hamiltonians_time_i)
-
-    if doppler:
-        assert dop_classes is not None and doppler_shifts is not None
-        dop_velocities, dop_volumes = doppler_mesh(dop_classes, spatial_dim)
-        eom_base = get_doppler_equations(eom_base, doppler_shifts, dop_velocities)
-
-        sols = solve_eom_stack(eom_base, const, eom_time_r, const_r,
-                               eom_time_i, const_i, time_functions,
-                               t_eval, init_cond, solver, **kwargs)
-
-        sols_weighted = apply_doppler_weights(sols, dop_velocities, dop_volumes)
-        if sum_doppler:
-            sum_axes = tuple(np.arange(spatial_dim))
-            sols_final = np.sum(sols_weighted, axis=sum_axes)
-        else:
-            sols_final = sols_weighted
-
-    else:
-        sols_final = solve_eom_stack(eom_base, const, eom_time_r, const_r,
-                                     eom_time_i, const_i, time_functions, t_eval,
-                                     init_cond, solver, **kwargs)
-
-    return sols_final.swapaxes(-1,-2)
-
-
-def solve_eom_stack(eoms_base: np.ndarray, const: np.ndarray,
-                    eom_time_r: np.ndarray, const_r: np.ndarray,
-                    eom_time_i: np.ndarray, const_i: np.ndarray,
-                    time_inputs: List[Callable[[float],float]],
-                    t_eval: np.ndarray, init_cond: np.ndarray, solver, **kwargs
-                    ) -> np.ndarray:
-
-    """
-    Solve a stack of equations of motion with shape `(*l, n, n)` in the time domain.
-    
-    Companion function to :func:`~.timesolvers.solve_time`, but can be invoked on its
-    for equations already formatted. 
-
-    Parameters
-    ----------
-    eoms_base : numpy.ndarray
-        Array of shape `(*l, n, n)` represnting the part of
-        equations of motion of the system which do not respond to external fields.
-    const : numpy.ndarray
-        constant term of shape (n,) added in differential equations. Typically
-        generated by :func:`~.sensor_utils.generate_eom`.
-    eoms_time_r : list[numpy.ndarray]
-        list of arrays of shape `(basis_size^2-1, basis_size^2-1)`
-        representing the parts of the OBEs with a real-valued time-dependence. In the solver,
-        this array will be multiplied by a time-dependent rabi frequency. Typically a matrix of
-        mostly zeros, with non-zero terms corresponding to a particular time-dependent coupling
-    const_r : numpy.ndarray
-        Constant term of shape (n,) added in a real time-dependent portion of
-        differential equations. Typically generated by :func:`~.sensor_utils.generate_eom_time`.
-    eoms_time_i : numpy.ndarray
-        list of arrays of shape `(basis_size^2-1, basis_size^2-1)`
-        representing the parts of the OBEs with an imaginary-valued time-dependence. In the solver,
-        this array will be multiplied by a time-dependent rabi frequency.
-    const_i : numpy.ndarray
-        constant term of shape (n,) added in an imaginary time-dependent portion of
-        differential equations. Typically generated by :func:`~.sensor_utils.generate_eom_time`.
-    t_eval : numpy.ndarray
-        1-D array of times, in microseconds, at which to
-        evaluate the solution. Does not affect evaluations in the solve.
-    time_inputs : list[function float->float]
-        List of functions which represent
-        the rabi frequency of a field as a function of time. list length should
-        be identical to the length of obes_time. In the solver, the *i* th time
-        input will be evaluated at time *t* and multiplied by the *i* th entry of
-        obes_time.
-    time_range tuple(float):
-        Pair of values represent the start and end time, in microseconds, of the simulation.
-    init_cond : numpy.ndarray or `None`, optional 
-        Density matrix representing the initial state of the system. 
-        If specified, the shape should be either `(n)` in the case of a single
-        initial condition for all parameter values, or should be of shape `(*l, n)`
-        matching the output shape of a steady state solve if the initial condition
-        may be different for different combinations of parameters. 
-        If `None`, will solve the problem in the steady state with all time-dependent fields
-        "off" and use the solution as the initial condition for the time behavior. Other
-        possible manual options might include a matrix populated by zeros representing the
-        entire population in the ground state. Defaults to `None`.
-
-    Returns
-    -------
-    numpy.ndarray
-        Flattened solution array corresponding to time points.
-        
-    """
-    stack_shape = eoms_base.shape[:-2]
-    solution_shape = stack_shape + (eoms_base.shape[-1], len(t_eval))
-
-    if init_cond.shape == eoms_base.shape[-1:]:
-        init_cond = np.broadcast_to(init_cond, solution_shape[:-1])
-
-    elif init_cond.shape != solution_shape[:-1]:
-        msg = f"""Inital condition shape {init_cond.shape} does not match expected
-        soulution shape {solution_shape[:-1]}"""
-        raise ValueError(msg)
-    
-    solutions = solver(eoms_base, const, eom_time_r, const_r, eom_time_i, const_i,
-                       time_inputs, t_eval, init_cond, **kwargs)
-
-    return solutions
-
-
-def generate_eom_time(hamiltonians_time: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
-    """
-    Generates the Optical Bloch Equations for just the rf terms. 
-    Uses the convention of the hamiltonian_rf return of the get_time_hamiltonian function.
-    The equations of motion returned are assumed to be used in conjunction with an electric field.
-
-    Parameters
-    ----------
-    hamiltonians_time : numpy.ndarray
-        A matrix of shape (basis_size, basis_size), where the off-diagonal
-        terms (i,j) are the dipole matrix elements in e a_b of the transition
-        coupling state i to state j.
-
-    Returns
-    -------
-    numpy.ndarray: Part of the Optical Bloch Equations corresponding to time_dependent couplings.
-        To produce equations to solve, these values must be multiplied by an electric
-        field in V/m.
-    numpy.ndarray: Constant term of the time-dependent portion of the equations
-        of motion. Same units as the equations themselves.
-        
-    """
-    eom_time = _hamiltonian_term(hamiltonians_time)
-    eqns, const = remove_ground(eom_time)
-    eom_time, const = make_real(eqns,const)
-
-    return eom_time.real, const
+"""
+Solvers for time domain analysis with an arbitrary RF field
+"""
+
+import numpy as np
+from importlib.metadata import version
+
+from .sensor_utils import _hamiltonian_term, generate_eom, make_real
+from .sensor_solution import Solution
+from .sensor import Sensor  # only needing for type hinting
+from .slicing.slicing import matrix_slice, get_slice_num_t
+
+from rydiqule.solvers import solve_steady_state
+from rydiqule.doppler_utils import *
+from rydiqule.stack_solvers.scipy_solver import scipy_solve
+from rydiqule.stack_solvers.nbkode_solver import nbkode_solve
+from rydiqule.stack_solvers.cyrk_solver import cyrk_solve
+from rydiqule.stack_solvers.nbrk_solver import nbrk_solve
+
+from typing import Optional, Tuple, Iterable, List, Callable, Sequence, Literal, Union
+
+stack_solvers = {"scipy": scipy_solve,
+                 "nbkode": nbkode_solve,
+                 "cyrk": cyrk_solve,
+                 "nbrk": nbrk_solve}
+
+solver_type = Union[Callable, Literal['scipy', 'nbkode', 'cyrk', 'nbrk']]
+
+def solve_time(sensor: Sensor, end_time: float, num_pts: int,
+               init_cond: Optional[np.ndarray] = None, doppler: bool = False,
+               doppler_mesh_method: Optional[MeshMethod] = None, sum_doppler: bool = True,
+               n_slices: Union[int, None] = None, solver: solver_type = "scipy", **kwargs) -> Solution:
+    """
+    Solves the response of the optical sensor in the time domain given the its time-dependent inputs
+    
+    If insuffucent system memory is available to solve the system all at once, 
+    system is broken into "slices" of manageable memory footprint which are solved indivudually. 
+    This slicing behavior does not affect the result. All couplings that include a "time_dependence" argument
+    will be solved in the time domain. 
+    
+    A number of solver backends work with rydiqule, but the default `"scipy"` ivp solver is the
+    is recommended backend in almost all cases, as it is the most fully-featured and
+    documented. Advanced users have the ablity to define their own solver backends
+    by creating a function that follows the call signature for rydiqule timesolver
+    backends. Additional arguments to the solver backend can be supplied with `**kwargs`.
+    
+    Parameters
+    -----------
+    sensor : :class:`~.Sensor`
+        The sensor object representing the atomic/laser arrangement of the system.
+    end_time : float  
+        Amount of time, in microseconds, for which to simulate the system
+    num_pts : int
+        The number of points along the range `(0, end_time)` for which
+        the solution is evaluated. This does not affect the number of funtion
+        evaluations during the solve, rather the spacing of the points in 
+        the reported solution.
+    init_cond : numpy.ndarray or `None`, optional 
+        Density matrix representing the initial state of the system. 
+        If specified, the shape should be either `(n)` in the case of a single
+        initial condition for all parameter values, or should be of shape `(*l, n)`
+        matching the output shape of a steady state solve if the initial condition
+        may be different for different combinations of parameters. 
+        If `None`, will solve the problem in the steady state with all time-dependent fields
+        "off" and use the solution as the initial condition for the time behavior. Other
+        possible manual options might include a matrix populated by zeros representing the
+        entire population in the ground state. Defaults to `None`.
+    doppler : bool, optional
+        Whether to account for doppler shift among moving atoms in
+        the gas. If True, the solver will implicitly define a velocity distribution
+        for particles in the cell, solve the problem for each velocity class,
+        and return a weighted average of the results. Note that solving in this
+        manner carries a substantial performance penalty, as each doppler velocity class
+        is solved as its own problem. If solved with doppler, only axis specified by a `"kvec"'
+        argument in one of the sensor couplings will be average over. The time solver currently 
+        supports doppler averaging in any number of spatial dimensions, up to the limit of 
+        3 imposed by the macroscopic physical world. Defaults to `False`.
+    doppler_mesh_method : dict, optional
+        Dictionary that controls the doppler meshing method. Exact details of this are
+        found in the documentation of :func:`~doppler_classes`. Ignored if 
+        `doppler=False`. Default is `None`.
+    sum_doppler : bool, optional
+        Whether to average over doppler classes after the solve
+        is complete. Setting to false will not perform the sum, allowing viewing
+        of the weighted results of the solve for each doppler class. Ignored
+        if `doppler=False`. Default is `True`.
+    n_slices : int or None, optional
+        How many sets of equations to break the full equations into.
+        The actual number of slices will be the largest between this value and the minumum
+        number of slices to solve the system without a memory error. If `None`, solver uses the
+        minimum number of slices required to solve without a `memoryError`. Defaults to None.
+    solver : {"scipy", "nbkode", "cyrk", "nbrk"} or callable
+        The backend solver used to solve the ivp generated by the sensor. All string values correspond
+        to backend solvers built in to rydiqule. Valid string values are:
+
+            - "scipy": Solves equations with :func:`scipy:scipy.integrate.solve_ivp`.
+                The default, most stable, and well-supported option.
+            - "nbkode": Solves equations with the jit-compiled Runge-Kutta-45 solver in :doc:`numbakit-ode <numbakitode:index>`.
+                May be faster for very long time solves with many timesteps.
+            - "cyrk": Solves jit-compiled equations with a cython compiled RK solver from `CyRK`.
+                Due to some jit compilation, only faster for moderate length problems
+                (ie problems with a moderate number of required time steps).
+            - "nbrk": Solves equations with the jit-compiled RK solver from `CyRK`.
+                Due to extensive jit compilation, only faster for very long solves
+                (ie problems with a large number of required time steps).
+
+        Additionally, can be specified with a callable that matches rydiqule's time-solver convention,
+        enabling using a custom solver backend.
+
+        .. note::
+
+            Unless otherwise noted, backends other than scipy are considered experimental.
+            Issues with their use are considered features not fully implemented rather than
+            bugs.
+
+    **kwargs: Additional keyword arguments passed to the backend solver. See documentation of the
+        relevant solver (i.e. :func:`scipy:scipy.integrate.solve_ivp`) for details and supported arguments.
+
+    Returns
+    -------
+    :class:`~.Solution`
+        A bunch-type object contining information about the
+        solution. Timesolver specific attributes are `t`  and `init_cond`,
+        corresponding respectively to the times at which the solution is sampled and
+        the initial conditions used for the solve.
+        
+    """
+    if type(solver) == str:
+        try:
+            solver = stack_solvers[solver]
+        except KeyError:
+            raise ValueError(f"{solver} is not a built-in solver. Supported built-in solvers are {list(stack_solvers.keys())}")
+    
+    if not isinstance(solver, Callable):
+        raise ValueError(f"Solvers must be callable functions")
+    
+    solution = Solution()
+
+    # relevant sensor-related quantities
+    stack_shape = sensor._stack_shape()
+    basis_size = sensor.basis_size
+    spatial_dim = sensor.spatial_dim()
+
+    # set up time parameters
+    time_range = (0.0, end_time)
+    t_eval = np.linspace(*time_range, num=num_pts, dtype=np.float64)
+
+    # initialize doppler-related quantities
+    doppler_axis_shape: Iterable[int] = ()
+    dop_classes = None
+    doppler_shifts = None
+    out_doppler_axes: Iterable[slice] = ()
+    doppler_axes: Iterable[slice] = ()
+
+    # update doppler-related values
+    if doppler:
+        dop_classes = doppler_classes(method=doppler_mesh_method)
+        doppler_shifts = sensor.get_doppler_shifts()
+        doppler_axis_shape = tuple(len(dop_classes) for _ in range(spatial_dim))
+        doppler_axes = tuple(slice(None) for _ in range(spatial_dim))
+
+        if not sum_doppler:
+            out_doppler_axes = doppler_axes
+
+    if init_cond is None:
+        init_cond = solve_steady_state(
+            sensor, doppler=doppler, weight_doppler=False, sum_doppler=False,
+            doppler_mesh_method=doppler_mesh_method
+            ).rho
+
+    # use available memory to figure out how to slice the hamiltonian
+    n_slices, out_sol_shape = get_slice_num_t(basis_size, stack_shape, doppler_axis_shape,
+                                                  num_pts, sum_doppler, n_slices)
+
+    if n_slices > 1:
+        print(f"Breaking equations of motion into {n_slices} sets of equations...")
+
+    # allocate arrays
+    hamiltonians, hamiltonians_time, hamiltonians_time_i = sensor.get_time_hamiltonians()
+    n_time = len(hamiltonians_time)
+    time_functions = sensor.get_time_dependence()
+    gamma = sensor.decoherence_matrix()
+    sols = np.zeros(out_sol_shape, dtype="float64")
+    
+    n_slices_true = sum(1 for _ in matrix_slice(gamma, n_slices=n_slices))
+
+    for i, (idx, H, G, *time_hams), in enumerate(matrix_slice(hamiltonians, gamma, *hamiltonians_time, *hamiltonians_time_i, n_slices=n_slices)):
+        
+        if n_slices_true > 1:
+            print(f"Solving equation slice {i+1}/{n_slices_true}", end='\r')
+            
+        Ht = np.array(time_hams[:n_time])
+        Ht_i = np.array(time_hams[n_time:])
+        
+        full_idx = (*out_doppler_axes, *idx, slice(None))
+        sols[full_idx] = _solve_hamiltonian_stack(H, Ht, Ht_i,
+                                                  G, time_functions, t_eval,
+                                                  init_cond[(*doppler_axes, *idx)], solver, doppler=doppler,
+                                                  dop_classes=dop_classes, sum_doppler=sum_doppler,
+                                                  doppler_shifts=doppler_shifts,
+                                                  spatial_dim=spatial_dim, **kwargs)
+
+    # save results to the Solution
+    solution.rho = sols
+    solution.eta = sensor.eta
+    solution.kappa = sensor.kappa
+    solution.axis_labels = [f'doppler_{i:d}' for i in range(spatial_dim) if not sum_doppler] + sensor.axis_labels() + ["time", "density_matrix"]
+    solution.axis_values = [dop_classes for i in range(spatial_dim) if not sum_doppler] + [val for _,_,val in sensor.variable_parameters()] + [t_eval, sensor.basis()]
+    solution.basis = sensor.basis()
+    solution.rq_version = version("rydiqule")
+    solution.doppler_classes = dop_classes
+    # time solver specific
+    solution.t = t_eval
+    solution.init_cond = init_cond
+
+    return solution
+
+
+def _solve_hamiltonian_stack(hamiltonians_base: np.ndarray, hamiltonians_time: np.ndarray,
+                             hamiltonians_time_i: np.ndarray, gamma_matrix: np.ndarray,
+                             time_functions: List[Callable[[float], float]], t_eval: np.ndarray,
+                             init_cond: np.ndarray, solver, doppler: bool = False,
+                             dop_classes: Optional[np.ndarray] = None, sum_doppler: bool = True,
+                             weight_doppler: bool = True,
+                             doppler_shifts: Optional[np.ndarray] = None,
+                             spatial_dim: int = 0, **kwargs
+                             ) -> np.ndarray:
+
+    """
+    Internal funtions which solve the equations of a given hamiltonian stack 
+    with the given parameters.
+    """
+    eom_base, const = generate_eom(hamiltonians_base, gamma_matrix,
+                                   remove_ground_state=True, real_eom=True)
+    eom_time_r, const_r = generate_eom_time(hamiltonians_time)
+    eom_time_i, const_i = generate_eom_time(hamiltonians_time_i)
+
+    if doppler:
+        assert dop_classes is not None and doppler_shifts is not None
+        dop_velocities, dop_volumes = doppler_mesh(dop_classes, spatial_dim)
+        eom_base = get_doppler_equations(eom_base, doppler_shifts, dop_velocities)
+
+        sols = solve_eom_stack(eom_base, const, eom_time_r, const_r,
+                               eom_time_i, const_i, time_functions,
+                               t_eval, init_cond, solver, **kwargs)
+
+        sols_weighted = apply_doppler_weights(sols, dop_velocities, dop_volumes)
+        if sum_doppler:
+            sum_axes = tuple(np.arange(spatial_dim))
+            sols_final = np.sum(sols_weighted, axis=sum_axes)
+        else:
+            sols_final = sols_weighted
+
+    else:
+        sols_final = solve_eom_stack(eom_base, const, eom_time_r, const_r,
+                                     eom_time_i, const_i, time_functions, t_eval,
+                                     init_cond, solver, **kwargs)
+
+    return sols_final.swapaxes(-1,-2)
+
+
+def solve_eom_stack(eoms_base: np.ndarray, const: np.ndarray,
+                    eom_time_r: np.ndarray, const_r: np.ndarray,
+                    eom_time_i: np.ndarray, const_i: np.ndarray,
+                    time_inputs: List[Callable[[float],float]],
+                    t_eval: np.ndarray, init_cond: np.ndarray, solver, **kwargs
+                    ) -> np.ndarray:
+
+    """
+    Solve a stack of equations of motion with shape `(*l, n, n)` in the time domain.
+    
+    Companion function to :func:`~.timesolvers.solve_time`, but can be invoked on its
+    for equations already formatted. 
+
+    Parameters
+    ----------
+    eoms_base : numpy.ndarray
+        Array of shape `(*l, n, n)` represnting the part of
+        equations of motion of the system which do not respond to external fields.
+    const : numpy.ndarray
+        constant term of shape (n,) added in differential equations. Typically
+        generated by :func:`~.sensor_utils.generate_eom`.
+    eoms_time_r : list[numpy.ndarray]
+        list of arrays of shape `(basis_size^2-1, basis_size^2-1)`
+        representing the parts of the OBEs with a real-valued time-dependence. In the solver,
+        this array will be multiplied by a time-dependent rabi frequency. Typically a matrix of
+        mostly zeros, with non-zero terms corresponding to a particular time-dependent coupling
+    const_r : numpy.ndarray
+        Constant term of shape (n,) added in a real time-dependent portion of
+        differential equations. Typically generated by :func:`~.sensor_utils.generate_eom_time`.
+    eoms_time_i : numpy.ndarray
+        list of arrays of shape `(basis_size^2-1, basis_size^2-1)`
+        representing the parts of the OBEs with an imaginary-valued time-dependence. In the solver,
+        this array will be multiplied by a time-dependent rabi frequency.
+    const_i : numpy.ndarray
+        constant term of shape (n,) added in an imaginary time-dependent portion of
+        differential equations. Typically generated by :func:`~.sensor_utils.generate_eom_time`.
+    t_eval : numpy.ndarray
+        1-D array of times, in microseconds, at which to
+        evaluate the solution. Does not affect evaluations in the solve.
+    time_inputs : list[function float->float]
+        List of functions which represent
+        the rabi frequency of a field as a function of time. list length should
+        be identical to the length of obes_time. In the solver, the *i* th time
+        input will be evaluated at time *t* and multiplied by the *i* th entry of
+        obes_time.
+    time_range tuple(float):
+        Pair of values represent the start and end time, in microseconds, of the simulation.
+    init_cond : numpy.ndarray or `None`, optional 
+        Density matrix representing the initial state of the system. 
+        If specified, the shape should be either `(n)` in the case of a single
+        initial condition for all parameter values, or should be of shape `(*l, n)`
+        matching the output shape of a steady state solve if the initial condition
+        may be different for different combinations of parameters. 
+        If `None`, will solve the problem in the steady state with all time-dependent fields
+        "off" and use the solution as the initial condition for the time behavior. Other
+        possible manual options might include a matrix populated by zeros representing the
+        entire population in the ground state. Defaults to `None`.
+
+    Returns
+    -------
+    numpy.ndarray
+        Flattened solution array corresponding to time points.
+        
+    """  # noqa
+    stack_shape = eoms_base.shape[:-2]
+    solution_shape = stack_shape + (eoms_base.shape[-1], len(t_eval))
+
+    if init_cond.shape == eoms_base.shape[-1:]:
+        init_cond = np.broadcast_to(init_cond, solution_shape[:-1])
+
+    elif init_cond.shape != solution_shape[:-1]:
+        msg = f"""Inital condition shape {init_cond.shape} does not match expected
+        soulution shape {solution_shape[:-1]}"""
+        raise ValueError(msg)
+    
+    solutions = solver(eoms_base, const, eom_time_r, const_r, eom_time_i, const_i, time_inputs, t_eval, init_cond, **kwargs)
+
+    return solutions
+
+
+def generate_eom_time(hamiltonians_time: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
+    """
+    Generates the Optical Bloch Equations for just the rf terms. 
+    Uses the convention of the hamiltonian_rf return of the get_time_hamiltonian function.
+    The equations of motion returned are assumed to be used in conjunction with an electric field.
+
+    Parameters
+    ----------
+    hamiltonians_time : numpy.ndarray
+        A matrix of shape (basis_size, basis_size), where the off-diagonal
+        terms (i,j) are the dipole matrix elements in e a_b of the transition
+        coupling state i to state j.
+
+    Returns
+    -------
+    numpy.ndarray: Part of the Optical Bloch Equations corresponding to time_dependent couplings.
+        To produce equations to solve, these values must be multiplied by an electric
+        field in V/m.
+    numpy.ndarray: Constant term of the time-dependent portion of the equations
+        of motion. Same units as the equations themselves.
+        
+    """  # noqa
+    eom_time = _hamiltonian_term(hamiltonians_time)
+    eqns, const = remove_ground(eom_time)
+    eom_time, const = make_real(eqns,const)
+
+    return eom_time.real, const
```

### Comparing `rydiqule-1.0.0/src/rydiqule.egg-info/PKG-INFO` & `rydiqule-1.0.0rc2/src/rydiqule.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,152 +1,148 @@
-Metadata-Version: 2.1
-Name: rydiqule
-Version: 1.0.0
-Summary: Rydberg Sensor Interactive Quantum Physics Module
-Author: ARL and NAWCWD
-License: Apache
-Keywords: rydberg,atomic-physics,quantum-optics,atomic-sensors,electrometry
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: tests
-Provides-Extra: mypy
-Provides-Extra: linter
-License-File: LICENSE
-
-<img src="https://raw.githubusercontent.com/QTC-UMD/rydiqule/main/docs/source/img/Rydiqule_Logo_Transparent_300.png" alt="rydiqule" style="max-width: 100%;">
-
-The Rydberg Interactive Quantum module is a modelling library designed to simulate
-the response of a Rydberg atoms to arbitrary input RF waveforms.
-It also functions as a general master equation solver based on the semi-classical density matrix method.
-
-[![PyPI](https://img.shields.io/pypi/v/rydiqule.svg)](https://pypi.org/project/rydiqule)
-[![Python Version](https://img.shields.io/pypi/pyversions/rydiqule.svg)](https://python.org)
-[![License](https://img.shields.io/pypi/l/rydiqule.svg)](https://github.com/QTC-UMD/rydiqule/raw/main/LICENSE)
-[![Docs](https://readthedocs.org/projects/rydiqule/badge/?version=latest)](https://rydiqule.readthedocs.io/en/latest)
-
-## Installation
-
-Presently, installation is done via pip.
-See below for detailed instructions.
-
-In all cases, it is highly recommended to install rydiqule in a virtual environment.
-
-### Conda/pip installation
-
-If using a conda to provide the virtual environmnet,
-it can often be advantageous to install as many packages as possible via conda before running the pip installation command.
-
-Assuming you have not already created a separate environment for RydIQule (recommended), run the following to create a new environment:
-```shell
-(base) ~/> conda create -n rydiqule python=3.9
-(base) ~/> conda activate rydiqule
-```
-RydIQule currently requires python >3.8.
-
-Now install dependencies that are available via conda.
-To capture as many dependencies as possible,
-we will add the `conda-forge` channel at a lower priority.
-```shell
-(rydiqule) ~/> conda config --append channels conda-forge
-(rydiqule) ~/> conda config --set channel_priority strict
-(rydiqule) ~/> conda install numpy scipy matplotlib networkx numba psutil
-# ARC specific dependencies available via conda
-(rydiqule) ~/> conda install sympy asteval lmfit uncertainties
-```
-
-Now use pip to install rydiqule and remaining dependencies.
-```shell
-# for normal installation
-(rydiqule) ~/> pip install rydiqule
-# for editable installation, so source can be modified locally
-(rydiqule) ~/> pip install -e rydiqule
-```
-
-### Pure pip installation
-
-To install normally, run:
-```shell
-pip install rydiqule
-```
-This command will use pip to install all necessary dependencies.
-
-To install in an editable way (which allows edits of the source code), run:
-```shell
-pip install -e rydiqule
-```
-
-### Confirm installation
-
-Proper installation can be confirmed by executing the following commands in a python terminal.
-```shell
->>> import rydiqule as rq
->>> rq.about()
-
-        Rydiqule
-    ================
-
-Rydiqule Version:     1.0.0
-Installation Path:    C:\Users\naqsL\Miniconda3\envs\rydiqule\lib\site-packages\rydiqule
-
-      Dependencies
-    ================
-
-NumPy Version:        1.24.3
-SciPy Version:        1.10.1
-Matplotlib Version:   3.7.1
-ARC Version:          3.3.0
-Python Version:       3.9.16
-Python Install Path:  C:\Users\naqsL\Miniconda3\envs\rydiqule
-Platform Info:        Windows (AMD64)
-CPU Count:            12
-Total System Memory:  128 GB
-```
-
-### Updating an existing installation
-
-Upgrading an existing installation is simple.
-Simply run the pip installation commands described above with the update flag.
-```shell
-pip install -U rydiqule
-```
-This command will also install any new dependencies that are required.
-
-If using an editable install, simply replacing the files in the same directory is sufficient.
-Though it is recommended to also run the appropriate pip update command as well.
-```shell
-pip install -U -e rydiqule
-```
-
-### Dependencies
-
-This package requires installation of the excellent [ARC](https://github.com/nikolasibalic/ARC-Alkali-Rydberg-Calculator) package, which is used to get Rydberg atomic properties.
-It also requires other standard computation dependenices, such as `numpy`, `scipy`, `matplotlib`, etc.
-These dependencies will be automatically installed by pip if not already present.
-
-The timesolver backend dependencies include the [numbakit-ode](https://github.com/hgrecco/numbakit-ode)
-and [CyRK](https://github.com/jrenaud90/CyRK) packages.
-Both are available via `pip`.
-
-## Documentation
-
-Documentation is available online at [readthedocs](https://rydiqule.readthedocs.io/en/latest).
-PDF or EPUB formats of the documentation can be downloaded from the online documentation.
-
-### Examples
-
-Example jupyter notebooks that demonstrate RydIQule can be found in the `examples` subdirectory.
-Printouts of these notebooks are available in the documentation as well.
-
-## Support
-
-Creation of this software was supported in part by the Defense Advanced Research Projects Agency (DARPA) Quantum Apertures program, DEVCOM Army Research Laboratory, and the Quantum Technology Center at the University of Maryland.
-
-## Disclaimer
-
-The views, opinions and/or findings expressed are those of the authors and should not be interpreted as representing the official views or policies of the Department of Defense or the U.S. Government.
+Metadata-Version: 2.1
+Name: rydiqule
+Version: 1.0.0rc2
+Summary: Rydberg Sensor Interactive Quantum Physics Module
+Author: ARL and NAWCWD
+License: Apache
+Keywords: rydberg,atomic-physics,quantum-optics,atomic-sensors,electrometry
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: tests
+Provides-Extra: mypy
+Provides-Extra: linter
+License-File: LICENSE
+
+![Rydiqule Logo](docs/source/img/Rydiqule_Logo_Transparent_300.png)
+
+The Rydberg Interactive Quantum module is a modelling library designed to simulate
+the response of a Rydberg atoms to arbitrary input RF waveforms.
+It also functions as a general master equation solver based on the semi-classical density matrix method.
+
+[![Docs](https://readthedocs.org/projects/rydiqule/badge/?version=latest)](https://rydiqule.readthedocs.io/en/latest)
+
+## Installation
+
+Presently, installation must be done manually using a copy of the repository.
+After downloading or cloning this repository,
+follow the directions below for installation.
+
+### Pure pip installation
+
+To install in an editable way (which allows edits of the source code), run:
+```shell
+pip install -e .
+```
+from within the top level `rydiqule` directory (i.e. where the `setup.cfg` file resides).
+This command will use pip to install all necessary dependencies.
+
+To install normally, run:
+```shell
+pip install .
+```
+from the same directory.
+
+### Conda/pip installation
+
+If using a conda environment, it can often be advantageous to install as many packages via conda before running the pip installation command.
+
+Assuming you have not already created a separate environment for RydIQule (recommended), run the following to create a new environment:
+```shell
+(base) ~/Rydiqule> conda create -n rydiqule python=3.9
+(base) ~/Rydiqule> conda activate rydiqule
+```
+RydIQule currently requires python >3.8.
+
+Now install dependencies that are available via conda.
+To capture as many dependencies as possible,
+we will add the `conda-forge` channel at a lower priority.
+```shell
+(rydiqule) ~/Rydiqule> conda config --append channels conda-forge
+(rydiqule) ~/Rydiqule> conda config --set channel_priority strict
+(rydiqule) ~/Rydiqule> conda install numpy scipy matplotlib networkx psutil
+# ARC specific dependencies available via conda
+(rydiqule) ~/Rydiqule> conda install sympy asteval lmfit uncertainties
+```
+
+Now use pip to install rydiqule and remaining dependencies.
+```shell
+# for editable installation, so source can be modified locally
+(rydiqule) ~/Rydiqule> pip install -e .
+# for normal installation
+(rydiqule) ~/Rydiqule> pip install .
+```
+
+### Confirm installation
+
+Proper installation can be confirmed by executing the following commands in a python terminal.
+```shell
+>>> import rydiqule as rq
+>>> rq.about()
+
+        Rydiqule
+    ================
+
+Rydiqule Version:     0.3.0
+Installation Path:    c:\users\naqsl\src\rydiqule\src\rydiqule
+
+      Dependencies
+    ================
+
+NumPy Version:        1.20.3
+SciPy Version:        1.7.1
+Matplotlib Version:   3.5.0
+ARC Version:          3.2.0
+Python Version:       3.8.12
+Python Install Path:  C:\Users\naqsL\Miniconda3\envs\arc
+Platform Info:        Windows (AMD64)
+CPU Count:            12
+Total System Memory:  128 GB
+```
+
+### Updating an existing installation
+
+Upgrading an existing installation is simple.
+Simply run the pip installation commands described above with the update flag.
+```shell
+pip install -U .
+```
+This command will also install any new dependencies that are required.
+
+If using an editable install, simply replacing the files in the same directory is sufficient.
+Though it is recommended to also run the appropriate pip update command as well.
+```shell
+pip install -U -e .
+```
+
+### Dependencies
+
+This package requires installation of the excellent [ARC](https://github.com/nikolasibalic/ARC-Alkali-Rydberg-Calculator) package, which is used to get Rydberg atomic properties.
+It also requires other standard computation dependenices, such as `numpy`, `scipy`, `matplotlib`, etc.
+These dependencies will be automatically installed by pip if not already present.
+
+The timesolver backend dependencies include the `numbakit-ode` and `CyRK` packages.
+Both are available via `pip`.
+
+## Documentation
+
+Documentation is available online at [readthedocs](https://rydiqule.readthedocs.io/en/latest).
+PDF or EPUB formats of the documentation can be downloaded from the online documentation.
+
+### Examples
+
+Example jupyter notebooks that demonstrate RydIQule can be found in the `examples` subdirectory.
+Printouts of these notebooks are available in the documentation as well.
+
+## Support
+
+Creation of this software was supported in part by the Defense Advanced Research Projects Agency (DARPA) Quantum Apertures program, DEVCOM Army Research Laboratory, and the Quantum Technology Center at the University of Maryland.
+
+## Disclaimer
+
+The views, opinions and/or findings expressed are those of the authors and should not be interpreted as representing the official views or policies of the Department of Defense or the U.S. Government.
```

### Comparing `rydiqule-1.0.0/src/rydiqule.egg-info/SOURCES.txt` & `rydiqule-1.0.0rc2/src/rydiqule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rydiqule-1.0.0/tests/test_EOMs.py` & `rydiqule-1.0.0rc2/tests/test_EOMs.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-import numpy as np
-import pytest
-from rydiqule.sensor_utils import generate_eom
-from rydiqule.solvers import steady_state_solve_stack
-
-
-@pytest.mark.util
-def test_2level_EOM():
-    """Tests that EOMs are generated correctly using a simple two-level
-    system with a far detuned coupling field.
-    """
-
-    omega1 = 1
-    natLifetime = 0.01
-    delta1 = 10
-
-    # expected EOM arrays
-    # basis is rho01_real, rho01_imag, rho11_real
-    rhs = -np.array([0,-omega1/2,0])
-    lhs = -np.array([[natLifetime/2,delta1,0],
-                    [-delta1,natLifetime/2,omega1],
-                    [0,-omega1,natLifetime]])
-
-    ham = np.array([[0,omega1/2],[omega1/2,delta1]])
-    decoh = np.zeros((2,2),dtype=np.double)
-    decoh[1,0] = natLifetime
-
-    eom, constant_term = generate_eom(ham, decoh)
-
-    np.testing.assert_allclose(rhs, constant_term,
-                               err_msg='Constant terms do not match for 2-level EOMs')
-    np.testing.assert_allclose(lhs, eom, err_msg='EOM terms do not match for 2-level EOMs')
-
-
-@pytest.mark.util
-def test_simple_Ham():
-    """Tests that EOMs are generated correctly using a simple three-level
-    system with far detuned fields.
-    """
-
-    omega1 = 0.55555+1.3333j
-    decayRate = .01
-    delta1 = 10
-    delta2 = 10
-    omega2 = .5
-
-    rho_01_pred = -omega1.real/delta1
-    rho_10_pred = -omega1.imag/delta1
-    # rho_21_pred = -omega2/delta1
-    # rho_12_pred = -omega2/delta2
-    # these predictions come from analytically solving the master eqn.
-    # see simple mathematica notebook that can be supplied by KCC
-
-    ham = np.array([[0,np.conj(omega1),0],[omega1,delta1,omega2],[0,omega2,delta2]])
-    decoh = np.array([[decayRate,0,0],[decayRate,0,0],[decayRate,0,0]])
-    # redrabi = omega1
-    # redphase = 0
-    eom, constant_term = generate_eom(ham, decoh, real_eom=True)
-    rho = steady_state_solve_stack(eom, constant_term)
-    np.testing.assert_allclose([rho_01_pred,rho_10_pred], [rho[0],rho[2]],atol=0.1,
-                               err_msg='did not correctly solve large-detuning test Hamiltonian')
-    # note: I do not currently know what the basis is after make_real.
-    # But the code asserts that Re(rho_01) is rho[0], so start with that one.
+import numpy as np
+import pytest
+from rydiqule.sensor_utils import generate_eom
+from rydiqule.solvers import steady_state_solve_stack
+
+
+@pytest.mark.util
+def test_2level_EOM():
+    """Tests that EOMs are generated correctly using a simple two-level
+    system with a far detuned coupling field.
+    """
+
+    omega1 = 1
+    natLifetime = 0.01
+    delta1 = 10
+
+    # expected EOM arrays
+    # basis is rho01_real, rho01_imag, rho11_real
+    rhs = -np.array([0,-omega1/2,0])
+    lhs = -np.array([[natLifetime/2,delta1,0],
+                    [-delta1,natLifetime/2,omega1],
+                    [0,-omega1,natLifetime]])
+
+    ham = np.array([[0,omega1/2],[omega1/2,delta1]])
+    decoh = np.zeros((2,2),dtype=np.double)
+    decoh[1,0] = natLifetime
+
+    eom, constant_term = generate_eom(ham, decoh)
+
+    np.testing.assert_allclose(rhs, constant_term,
+                               err_msg='Constant terms do not match for 2-level EOMs')
+    np.testing.assert_allclose(lhs, eom, err_msg='EOM terms do not match for 2-level EOMs')
+
+
+@pytest.mark.util
+def test_simple_Ham():
+    """Tests that EOMs are generated correctly using a simple three-level
+    system with far detuned fields.
+    """
+
+    omega1 = 0.55555+1.3333j
+    decayRate = .01
+    delta1 = 10
+    delta2 = 10
+    omega2 = .5
+
+    rho_01_pred = -omega1.real/delta1
+    rho_10_pred = -omega1.imag/delta1
+    # rho_21_pred = -omega2/delta1
+    # rho_12_pred = -omega2/delta2
+    # these predictions come from analytically solving the master eqn.
+    # see simple mathematica notebook that can be supplied by KCC
+
+    ham = np.array([[0,np.conj(omega1),0],[omega1,delta1,omega2],[0,omega2,delta2]])
+    decoh = np.array([[decayRate,0,0],[decayRate,0,0],[decayRate,0,0]])
+    # redrabi = omega1
+    # redphase = 0
+    eom, constant_term = generate_eom(ham, decoh, real_eom=True)
+    rho = steady_state_solve_stack(eom, constant_term)
+    np.testing.assert_allclose([rho_01_pred,rho_10_pred], [rho[0],rho[2]],atol=0.1,
+                               err_msg='did not correctly solve large-detuning test Hamiltonian')
+    # note: I do not currently know what the basis is after make_real.
+    # But the code asserts that Re(rho_01) is rho[0], so start with that one.
```

### Comparing `rydiqule-1.0.0/tests/test_calculate_snr.py` & `rydiqule-1.0.0rc2/tests/test_calculate_snr.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-import numpy as np
-import pytest
-import rydiqule as rq
-
-
-@pytest.mark.exp
-def test_calculate_snr():
-    """
-    Check the SNR calculation agains a basic result from https://arxiv.org/pdf/2105.10494.pdf.
-    Show that for a weak off-resonant E-field, in the phase quadrature, with small decoherence,
-    and in the limit of small Rabi frequencies, that the optimum probe Rabis is sqrt(2) lower
-    than the coupling.  Note that this test does not check the overal scalling of the SNR.
-    """
-
-    Rb_sensor = rq.Sensor(4)
-
-    kappa = 28759.120135025692
-    eta = 0.0013537502717366691
-
-    red_rabi = np.linspace(0.1,4,100)
-    blue_rabi = 1
-
-    rf_rabi_step = np.array([0.1, 0.101])
-    probe = {'states': (0,1), 'rabi_frequency': red_rabi, 'detuning': 0, 'label': 'probe'}
-    couple = {'states': (1,2), 'rabi_frequency': blue_rabi, 'detuning': 0, 'label':'couple'}
-    rf = {'states': (2,3), 'rabi_frequency': rf_rabi_step, 'detuning':30, 'label': 'rf'}
-
-    gamma_matrix = np.array(
-                          [[0, 0, 0, 0],
-                           [37.82675, 0, 0, 0],
-                           [0.02, 0, 0, 0],
-                           [0, 0, 0, 0]]
-                          )
-
-    Rb_sensor.add_couplings(probe, couple, rf)
-
-    Rb_sensor.set_gamma_matrix(gamma_matrix)
-
-    snrs, param_mesh = rq.get_snr(
-        Rb_sensor, 100e-6, param_label='rf_rabi_frequency', probe_tuple=(0,1),
-        phase_quadrature=True, kappa=kappa, eta=eta
-        )
-
-    snrs_final = snrs[:,1]
-    max_idx = np.argmax(snrs_final)
-    param_mesh_final = np.array(param_mesh)[:,:,1]
-
-    optimum_rabi_result = param_mesh_final[0,max_idx]
-    prediction = blue_rabi/np.sqrt(2)
-
-    assert optimum_rabi_result == pytest.approx(prediction, abs=0, rel=0.1), \
-        'SNR with sensor does not match theory approximation'
-
-    # Now check with a Cell to confirm general operation
-    r1 = [50, 2, 2.5, 0.5]
-    r2 = [51, 1, 1.5, 0.5]
-
-    Rb_cell = rq.Cell('Rb85', *rq.D2_states("Rb85"), r1, r2, gamma_transit=0, beam_area=1e-6)
-
-    Rb_cell.add_couplings(probe, couple, rf)
-
-    snrs, param_mesh = rq.get_snr(
-        Rb_cell, 100e-6, param_label='rf_rabi_frequency', probe_tuple=(0,1),
-        phase_quadrature=True,
-    )
-
-    snrs_final = snrs[:,1]
-    max_idx = np.argmax(snrs_final)
-    param_mesh_final = np.array(param_mesh)[:,:,1]
-
-    optimum_rabi_result = param_mesh_final[0,max_idx]
-    prediction = blue_rabi/np.sqrt(2)
-
-    assert optimum_rabi_result == pytest.approx(prediction, abs=0, rel=0.1), \
-        'SNR with cell does not match theory approximation'
+import numpy as np
+import pytest
+import rydiqule as rq
+
+
+@pytest.mark.exp
+def test_calculate_snr():
+    """
+    Check the SNR calculation agains a basic result from https://arxiv.org/pdf/2105.10494.pdf.
+    Show that for a weak off-resonant E-field, in the phase quadrature, with small decoherence,
+    and in the limit of small Rabi frequencies, that the optimum probe Rabis is sqrt(2) lower
+    than the coupling.  Note that this test does not check the overal scalling of the SNR.
+    """
+
+    Rb_sensor = rq.Sensor(4)
+
+    kappa = 28759.120135025692
+    eta = 0.0013537502717366691
+
+    red_rabi = np.linspace(0.1,4,100)
+    blue_rabi = 1
+
+    rf_rabi_step = np.array([0.1, 0.101])
+    probe = {'states': (0,1), 'rabi_frequency': red_rabi, 'detuning': 0, 'label': 'probe'}
+    couple = {'states': (1,2), 'rabi_frequency': blue_rabi, 'detuning': 0, 'label':'couple'}
+    rf = {'states': (2,3), 'rabi_frequency': rf_rabi_step, 'detuning':30, 'label': 'rf'}
+
+    gamma_matrix = np.array(
+                          [[0, 0, 0, 0],
+                           [37.82675, 0, 0, 0],
+                           [0.02, 0, 0, 0],
+                           [0, 0, 0, 0]]
+                          )
+
+    Rb_sensor.add_couplings(probe, couple, rf)
+
+    Rb_sensor.set_gamma_matrix(gamma_matrix)
+
+    snrs, param_mesh = rq.get_snr(
+        Rb_sensor, 100e-6, param_label='rf_rabi_frequency', probe_tuple=(0,1),
+        phase_quadrature=True, kappa=kappa, eta=eta
+        )
+
+    snrs_final = snrs[:,1]
+    max_idx = np.argmax(snrs_final)
+    param_mesh_final = np.array(param_mesh)[:,:,1]
+
+    optimum_rabi_result = param_mesh_final[0,max_idx]
+    prediction = blue_rabi/np.sqrt(2)
+
+    assert optimum_rabi_result == pytest.approx(prediction, abs=0, rel=0.1), \
+        'SNR with sensor does not match theory approximation'
+
+    # Now check with a Cell to confirm general operation
+    r1 = [50, 2, 2.5, 0.5]
+    r2 = [51, 1, 1.5, 0.5]
+
+    Rb_cell = rq.Cell('Rb85', *rq.D2_states("Rb85"), r1, r2, gamma_transit=0, beam_area=1e-6)
+
+    Rb_cell.add_couplings(probe, couple, rf)
+
+    snrs, param_mesh = rq.get_snr(
+        Rb_cell, 100e-6, param_label='rf_rabi_frequency', probe_tuple=(0,1),
+        phase_quadrature=True,
+    )
+
+    snrs_final = snrs[:,1]
+    max_idx = np.argmax(snrs_final)
+    param_mesh_final = np.array(param_mesh)[:,:,1]
+
+    optimum_rabi_result = param_mesh_final[0,max_idx]
+    prediction = blue_rabi/np.sqrt(2)
+
+    assert optimum_rabi_result == pytest.approx(prediction, abs=0, rel=0.1), \
+        'SNR with cell does not match theory approximation'
```

### Comparing `rydiqule-1.0.0/tests/test_cell.py` & `rydiqule-1.0.0rc2/tests/test_cell.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-import numpy as np
-from arc import Rubidium85
-import rydiqule as rq
-import pytest
-
-
-@pytest.mark.exception
-def test_cell_coupling_exceptions(Rb85_sensor_kwargs):
-    '''Test that Cell-specific checks for couplings fail appropriately.'''
-
-    c = rq.Cell('Rb85', *rq.D2_states(50), **Rb85_sensor_kwargs)
-
-    with pytest.raises(ValueError, match='only define one'):
-        f1 = {'states':(0,1), 'rabi_frequency':10, 'e_field':5}
-        c.add_coupling(**f1)
-
-    with pytest.raises(ValueError, match='only define one'):
-        f1 = {'states':(0,1), 'rabi_frequency':10, 'beam_power':5}
-        c.add_coupling(**f1)
-
-    with pytest.raises(ValueError, match='only define one'):
-        f1 = {'states':(0,1), 'e_field':5, 'beam_waist':1.5}
-        c.add_coupling(**f1)
-
-    with pytest.raises(ValueError, match='only define one'):
-        f1 = {'states':(0,1), 'beam_power':5}
-        c.add_coupling(**f1)
-
-    with pytest.raises(ValueError, match='scanned simultaneously'):
-        f1 = {'states':(0,1), 'beam_power':[1e-6, 2e-6], 'beam_waist':[100e-6,200e-6]}
-        c.add_coupling(**f1)
-
-    with pytest.raises(ValueError, match='Cell does not support explicit'):
-        f2 = {'states':(0,1), 'rabi_frequency':2, 'transition_frequency':5}
-        c.add_coupling(**f2)
-
-
-@pytest.mark.structure
-def test_dipole_scaling(Rb85_sensor_kwargs):
-    """Tests that fields specified by dipole moment are scaled correctly."""
-
-    rt = [50,2,2.5,0.5]
-    re = [49,3,3.5,0.5]
-    c = rq.Cell('Rb85', *rq.D2_states(50), rt, re, **Rb85_sensor_kwargs)
-
-    def func(t):
-        return 1
-    c.add_couplings({'states':(2,3), 'e_field':1, 'detuning':0,'time_dependence':func})
-
-    # diff between c.rf_dipole_matrix is scale_factor
-    base, dipole_mat, dipole_mat_i = c.get_time_hamiltonians()
-    rf_dipole_moment = dipole_mat[0][2,3]
-    desired_rabi = 5  # Mrad/s
-    # rf_dipole_moment is defined to have units of (Mrad/s)/(V/m)
-    field = desired_rabi/rf_dipole_moment
-
-    atom = Rubidium85()
-    arc_rabi = 0.5*atom.getRabiFrequency2(*rt, *re[:3], 0, field)*1e-6  # Mrad/s
-
-    assert desired_rabi == pytest.approx(arc_rabi), 'Internal dipole moments not scaled correctly'
-
-
-@pytest.mark.structure
-def test_decoherences(Rb85_sensor_kwargs):
-    """Confirms that the decoherence matrix is building correctly.
-    """
-    gState = [5, 0, 0.5, 0.5]
-    iState = [5, 1, 1.5, 0.5]
-    rState = [50, 2, 2.5, 0.5]
-    rcState = [51, 1, 1.5, 0.5]
-
-    atom = Rubidium85()
-
-    # all rates are in MHz
-    gamma = 1/atom.getStateLifetime(*iState[0:3])*1e-6
-    rState_lifetime = 1/atom.getStateLifetime(*rState[0:3])*1e-6
-    rcState_lifetime = 1/atom.getStateLifetime(*rcState[0:3])*1e-6
-
-    riDecay = atom.getTransitionRate(*rState[:3], *iState[:3])*1e-6
-    rrcDecay = atom.getTransitionRate(*rState[:3], *rcState[:3])*1e-6
-    rcgDecay = atom.getTransitionRate(*rcState[:3], *gState[:3])*1e-6
-    transit = 2*np.pi*65.5286e-3*0
-
-    # calculates all dipole allowed dephasings
-    # any dephasing not accounted for from the natural lifetime
-    # is assumed to decay to the ground state
-    gamma_expected = np.zeros((4, 4))
-    gamma_expected[1, 0] = gamma
-    gamma_expected[2, 1] = riDecay
-    gamma_expected[2, 3] = rrcDecay
-    gamma_expected[3, 0] = rcgDecay
-
-    gamma_expected[2, 0] += rState_lifetime - riDecay - rrcDecay
-    gamma_expected[3, 0] += rcState_lifetime - rcgDecay
-
-    gamma_expected[:, 0] += transit
-
-    cell = rq.Cell('Rb85', gState, iState,
-                   rState, rcState, **Rb85_sensor_kwargs)
-    cell.add_transit_broadening(transit)
-
-    np.testing.assert_allclose(cell.decoherence_matrix(), gamma_expected,
-                               atol=2*np.pi*1e-4, rtol=0,
-                               err_msg='gamma matrix for 2-photon;1 RF not equal')
-
-@pytest.mark.exception
-def test_warns_dipole(Rb85_sensor_kwargs):
-    """Test that cell raises an error when a non dipole-allowed transition is added"""
-    c = rq.Cell('Rb85', *rq.D2_states(5), [50,2,2.5,0.5], **Rb85_sensor_kwargs)
-    
-    with pytest.warns(UserWarning, match='not electric-dipole allowed'):
-        f1 = {'states':(0,2), 'rabi_frequency':1, 'detuning':0}
+import numpy as np
+from arc import Rubidium85
+import rydiqule as rq
+import pytest
+
+
+@pytest.mark.exception
+def test_cell_coupling_exceptions(Rb85_sensor_kwargs):
+    '''Test that Cell-specific checks for couplings fail appropriately.'''
+
+    c = rq.Cell('Rb85', *rq.D2_states(50), **Rb85_sensor_kwargs)
+
+    with pytest.raises(ValueError, match='only define one'):
+        f1 = {'states':(0,1), 'rabi_frequency':10, 'e_field':5}
+        c.add_coupling(**f1)
+
+    with pytest.raises(ValueError, match='only define one'):
+        f1 = {'states':(0,1), 'rabi_frequency':10, 'beam_power':5}
+        c.add_coupling(**f1)
+
+    with pytest.raises(ValueError, match='only define one'):
+        f1 = {'states':(0,1), 'e_field':5, 'beam_waist':1.5}
+        c.add_coupling(**f1)
+
+    with pytest.raises(ValueError, match='only define one'):
+        f1 = {'states':(0,1), 'beam_power':5}
+        c.add_coupling(**f1)
+
+    with pytest.raises(ValueError, match='scanned simultaneously'):
+        f1 = {'states':(0,1), 'beam_power':[1e-6, 2e-6], 'beam_waist':[100e-6,200e-6]}
+        c.add_coupling(**f1)
+
+    with pytest.raises(ValueError, match='Cell does not support explicit'):
+        f2 = {'states':(0,1), 'rabi_frequency':2, 'transition_frequency':5}
+        c.add_coupling(**f2)
+
+
+@pytest.mark.structure
+def test_dipole_scaling(Rb85_sensor_kwargs):
+    """Tests that fields specified by dipole moment are scaled correctly."""
+
+    rt = [50,2,2.5,0.5]
+    re = [49,3,3.5,0.5]
+    c = rq.Cell('Rb85', *rq.D2_states(50), rt, re, **Rb85_sensor_kwargs)
+
+    def func(t):
+        return 1
+    c.add_couplings({'states':(2,3), 'e_field':1, 'detuning':0,'time_dependence':func})
+
+    # diff between c.rf_dipole_matrix is scale_factor
+    base, dipole_mat, dipole_mat_i = c.get_time_hamiltonians()
+    rf_dipole_moment = dipole_mat[0][2,3]
+    desired_rabi = 5  # Mrad/s
+    # rf_dipole_moment is defined to have units of (Mrad/s)/(V/m)
+    field = desired_rabi/rf_dipole_moment
+
+    atom = Rubidium85()
+    arc_rabi = 0.5*atom.getRabiFrequency2(*rt, *re[:3], 0, field)*1e-6  # Mrad/s
+
+    assert desired_rabi == pytest.approx(arc_rabi), 'Internal dipole moments not scaled correctly'
+
+
+@pytest.mark.structure
+def test_decoherences(Rb85_sensor_kwargs):
+    """Confirms that the decoherence matrix is building correctly.
+    """
+    gState = [5, 0, 0.5, 0.5]
+    iState = [5, 1, 1.5, 0.5]
+    rState = [50, 2, 2.5, 0.5]
+    rcState = [51, 1, 1.5, 0.5]
+
+    atom = Rubidium85()
+
+    # all rates are in MHz
+    gamma = 1/atom.getStateLifetime(*iState[0:3])*1e-6
+    rState_lifetime = 1/atom.getStateLifetime(*rState[0:3])*1e-6
+    rcState_lifetime = 1/atom.getStateLifetime(*rcState[0:3])*1e-6
+
+    riDecay = atom.getTransitionRate(*rState[:3], *iState[:3])*1e-6
+    rrcDecay = atom.getTransitionRate(*rState[:3], *rcState[:3])*1e-6
+    rcgDecay = atom.getTransitionRate(*rcState[:3], *gState[:3])*1e-6
+    transit = 2*np.pi*65.5286e-3*0
+
+    # calculates all dipole allowed dephasings
+    # any dephasing not accounted for from the natural lifetime
+    # is assumed to decay to the ground state
+    gamma_expected = np.zeros((4, 4))
+    gamma_expected[1, 0] = gamma
+    gamma_expected[2, 1] = riDecay
+    gamma_expected[2, 3] = rrcDecay
+    gamma_expected[3, 0] = rcgDecay
+
+    gamma_expected[2, 0] += rState_lifetime - riDecay - rrcDecay
+    gamma_expected[3, 0] += rcState_lifetime - rcgDecay
+
+    gamma_expected[:, 0] += transit
+
+    cell = rq.Cell('Rb85', gState, iState,
+                   rState, rcState, **Rb85_sensor_kwargs)
+    cell.add_transit_broadening(transit)
+
+    np.testing.assert_allclose(cell.decoherence_matrix(), gamma_expected,
+                               atol=2*np.pi*1e-4, rtol=0,
+                               err_msg='gamma matrix for 2-photon;1 RF not equal')
+
+@pytest.mark.exception
+def test_warns_dipole(Rb85_sensor_kwargs):
+    """Test that cell raises an error when a non dipole-allowed transition is added"""
+    c = rq.Cell('Rb85', *rq.D2_states(5), [50,2,2.5,0.5], **Rb85_sensor_kwargs)
+    
+    with pytest.warns(UserWarning, match='not electric-dipole allowed'):
+        f1 = {'states':(0,2), 'rabi_frequency':1, 'detuning':0}
         c.add_coupling(**f1)
```

### Comparing `rydiqule-1.0.0/tests/test_level_diagram.py` & `rydiqule-1.0.0rc2/tests/test_level_diagram.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,58 @@
-import numpy as np
-import pytest
-import rydiqule as rq
-
-
-@pytest.mark.util
-def test_lv_diagram():
-    """Confirms that level diagram plotting runs without major errors."""
-    # Generate 3 states
-    RydbergState_1 = [50, 2, 2.5, 0.5]  # states labeled n, l, j, m_j
-    RydbergState_2 = [51, 3, 3.5, 0.5]
-    RydbergState_3 = [52, 4, 3.5, 0.5]
-
-    # Initialize Cell
-    RbSensor_ss = rq.Cell("Rb85", *rq.D2_states(5),
-                          RydbergState_1, RydbergState_2, RydbergState_3,
-                          gamma_transit=2*np.pi*1)
-
-    # Couplings specified by rabi_frequency
-    test_laser_1 = {'states': (0,2), 'rabi_frequency': 1, 'detuning': 2}
-    # Not suppose to show up since Rabi_Frequency = 0
-    test_laser_2 = {'states': (1,3), 'rabi_frequency': 0, 'detuning': 3}
-
-    def testfun(a):
-        return 0
-
-    # Couplings specified by dipole moment
-    test_laser_3 = {'states': (0,3), 'rabi_frequency': 7,
-                    'beam_waist': 1, 'time_dependence': testfun}
-    test_laser_4 = {'states': (2,3), 'rabi_frequency': 8,
-                    'beam_waist': 1, 'time_dependence': testfun}
-    test_laser_5 = {'states': (3,4), 'rabi_frequency': 8,
-                    'beam_waist': 1, 'time_dependence': testfun}
-
-    RbSensor_ss.add_couplings(test_laser_1, test_laser_2, test_laser_3, test_laser_4, test_laser_5,
-                              suppress_dipole_warn=True, suppress_rwa_warn=True)
-    RbSensor_ss.add_transit_broadening([0,1,2,3])
-
-    # Draw the level diagram
-    level_diagram = rq.draw_diagram(RbSensor_ss)
-
-    # Remove the couplings defined by rabi_frequency of 0.
-    coupling_list = [test_laser_1, test_laser_2, test_laser_3, test_laser_4, test_laser_5]
-    coupling_list = [x for x in coupling_list
-                     if "rabi_frequency" in x.keys() and x.get('rabi_frequency') != 0]\
-        + [x for x in coupling_list if "beam_power" in x.keys()]
-        
-    gamma_list = [x for x in coupling_list
-                     if "gamma_transit" in x.keys()]
-
-    total_arrows = len([item for sublist in level_diagram.arrows for item in sublist])
-    total_levels = len(level_diagram.energies)
-
-    # Verify that the function gets the correct number of arrows
-    # (representing the couplings) and horizontal lines (representing the levels)
-    assert total_levels == 5, \
-        "Number of horizontal lines in the plot is not equal to number of states defined"
-    assert total_arrows == len(coupling_list) + len(gamma_list), \
-        "Number of arrows in the plot is not equal to number of couplings and dephasings defined"
+import numpy as np
+import pytest
+import rydiqule as rq
+
+
+@pytest.mark.util
+def test_lv_diagram():
+    """Confirms that level diagram plotting runs without major errors."""
+    # Generate 3 states
+    RydbergState_1 = [50, 2, 2.5, 0.5]  # states labeled n, l, j, m_j
+    RydbergState_2 = [51, 3, 3.5, 0.5]
+    RydbergState_3 = [52, 4, 3.5, 0.5]
+
+    # Initialize Cell
+    RbSensor_ss = rq.Cell("Rb85", *rq.D2_states(5),
+                          RydbergState_1, RydbergState_2, RydbergState_3,
+                          gamma_transit=2*np.pi*1)
+
+    # Couplings specified by rabi_frequency
+    test_laser_1 = {'states': (0,2), 'rabi_frequency': 1, 'detuning': 2}
+    # Not suppose to show up since Rabi_Frequency = 0
+    test_laser_2 = {'states': (1,3), 'rabi_frequency': 0, 'detuning': 3}
+
+    def testfun(a):
+        return 0
+
+    # Couplings specified by dipole moment
+    test_laser_3 = {'states': (0,3), 'rabi_frequency': 7,
+                    'beam_waist': 1, 'time_dependence': testfun}
+    test_laser_4 = {'states': (2,3), 'rabi_frequency': 8,
+                    'beam_waist': 1, 'time_dependence': testfun}
+    test_laser_5 = {'states': (3,4), 'rabi_frequency': 8,
+                    'beam_waist': 1, 'time_dependence': testfun}
+
+    RbSensor_ss.add_couplings(test_laser_1, test_laser_2, test_laser_3, test_laser_4, test_laser_5)
+    RbSensor_ss.add_transit_broadening([0,1,2,3])
+
+    # Draw the level diagram
+    level_diagram = rq.draw_diagram(RbSensor_ss)
+
+    # Remove the couplings defined by rabi_frequency of 0.
+    coupling_list = [test_laser_1, test_laser_2, test_laser_3, test_laser_4, test_laser_5]
+    coupling_list = [x for x in coupling_list
+                     if "rabi_frequency" in x.keys() and x.get('rabi_frequency') != 0]\
+        + [x for x in coupling_list if "beam_power" in x.keys()]
+        
+    gamma_list = [x for x in coupling_list
+                     if "gamma_transit" in x.keys()]
+
+    total_arrows = len([item for sublist in level_diagram.arrows for item in sublist])
+    total_levels = len(level_diagram.energies)
+
+    # Verify that the function gets the correct number of arrows
+    # (representing the couplings) and horizontal lines (representing the levels)
+    assert total_levels == 5, \
+        "Number of horizontal lines in the plot is not equal to number of states defined"
+    assert total_arrows == len(coupling_list) + len(gamma_list), \
+        "Number of arrows in the plot is not equal to number of couplings and dephasings defined"
```

### Comparing `rydiqule-1.0.0/tests/test_numbakitode.py` & `rydiqule-1.0.0rc2/tests/test_numbakitode.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,140 +1,139 @@
-import numpy as np
-import pytest
-
-import rydiqule as rq
-
-
-@pytest.mark.time
-@pytest.mark.slow
-def test_nbkit():
-    """Tests that time solver functions with Doppler broadening
-    """
-    red_laser = {'states':(0,1), 'rabi_frequency':2*np.pi*0.6, 'detuning':0}
-
-    RydbergTargetState = [150, 2, 2.5, 0.5]  # states labeled n, l, j, m_j
-    RydbergExcitedState = [149, 3, 3.5, 0.5]
-
-    RbSensor_time = rq.Cell("Rb85", *rq.D2_states(5),
-                            RydbergTargetState, RydbergExcitedState,
-                            gamma_transit=2*np.pi*.1)
-
-    def rf_carrier(t):
-        return np.sin(2*np.pi*10.0*t)
-
-    sampleNum = 20
-    endTime = 2
-
-    blue_laser = {'states':(1,2), 'rabi_frequency':6.0, 'detuning': 0}
-    rf = {'states':(2,3), 'rabi_frequency':1.0, 'detuning': 0, 'time_dependence': rf_carrier}
-    RbSensor_time.add_couplings(blue_laser, red_laser, rf)
-
-    sols_solve_ivp = rq.solve_time(RbSensor_time, endTime, sampleNum, solver='scipy', rtol=1e-6, atol=1e-6)
-    sols_nbkode = rq.solve_time(RbSensor_time, endTime, sampleNum,  solver='nbkode', rtol=1e-6, atol=1e-6)
-
-    np.testing.assert_allclose(sols_solve_ivp.rho[-1,:], sols_nbkode.rho[-1,:], atol=0.005, err_msg='The difference between two solutions is too big')
-
-
-@pytest.mark.time
-@pytest.mark.slow
-def test_time_complex_match_steady_numbakit():
-    """Tests the time solver vs steady state
-    with aribtrary (complex) and time-dependent rabi frequencies
-    using the numbakitode backend
-    """
-
-    def fun(t):
-        if t < 1:
-            return 0
-        else:
-            return 1
-
-    def fun2(t):
-        if t < 1:
-            return 0j
-        else:
-            return 1j
-
-    end_time = 100
-    sample_num = 20
-
-    probe_t = {'states':(0,1), 'rabi_frequency':4+9j,'detuning':0.3, 'time_dependence': fun}
-    probe_s = {'states':(0,1), 'rabi_frequency':4+9j,'detuning':0.3}
-    dress = {'states':(1,2), 'rabi_frequency':3+2j,'detuning': .7}
-    couple_t = {'states':(2,3), 'rabi_frequency':-9j+1, 'detuning':0.3, 'time_dependence': fun2}
-    couple_s = {'states':(2,3), 'rabi_frequency':9+1j, 'detuning':0.3}
-
-    gam = np.zeros((4,4),dtype=np.float64)
-    gam[1,0] = 0.5
-    gam[2,1] = 0.4
-    gam[3,2] = 0.6
-    gamma_matrix = gam
-
-    sensor_t = rq.Sensor(4)
-    sensor_s = rq.Sensor(4)
-
-    sensor_t.add_couplings(probe_t, dress, couple_t)
-    sensor_t.set_gamma_matrix(gamma_matrix)
-    sensor_s.add_couplings(probe_s, dress, couple_s)
-    sensor_s.set_gamma_matrix(gamma_matrix)
-
-    sols_s = rq.solve_steady_state(sensor_s)
-    sol_t_numba = rq.solve_time(sensor_t, end_time, sample_num, rtol=1E-6, atol=1e-6,
-                                solver='nbkode')
-    np.testing.assert_allclose(sols_s.rho,sol_t_numba.rho[-1,:],atol=0.005,
-           err_msg='Complex time and steady state solutions do not match using numbakit.')
-
-# @pytest.mark.time
-# @pytest.mark.doppler
-# def test_numba_with_doppler():
-#     """Tests that time solver functions with Doppler broadening
-#     """
-#     rf_rabi = 25 #Mrad/s
-#     red_laser = {'states':(0,1), 'rabi_frequency':2*np.pi*0.6}  #fields are stored as dictioniaries
-#     blue_laser = {'states':(1,2), 'rabi_frequency':2*np.pi*2.0, 'detuning': 0}
-#
-#     RbSensor_ss = rq.Cell(gamma_transit=2*np.pi*1, gamma_exc=2*np.pi*6, gamma_Ryd = 2*np.pi*.1)
-#     RbSensor_time = rq.Cell(gamma_transit=2*np.pi*1, gamma_exc=2*np.pi*6, gamma_Ryd = 2*np.pi*.1)
-#
-#     RydbergTargetState = [350, 2, 2.5, 0.5]  #states labeled n, l, j, m_j
-#     RydbergExcitedState = [349, 3, 3.5, 0.5]
-#
-#     RbSensor_ss.add_states(RydbergTargetState,RydbergExcitedState)
-#     RbSensor_time.add_states(RydbergTargetState,RydbergExcitedState)
-#
-#     rf_freq = RbSensor_time.atom.getTransitionFrequency(*RydbergTargetState[:3],*RydbergExcitedState[:3])*1E-6
-#
-#     RbSensor_ss.add_couplings({'states':(2,3), "dipole_moment":"auto", "transition_frequency":"auto"})
-#     rf_dipole_matrix = RbSensor_ss.rf_dipole_matrix()
-#
-#     rf_dipole_moment = rf_dipole_matrix[2,3]
-#     field = 2*rf_rabi/rf_dipole_moment
-#
-#     def sig_and_LO(omega_0, delta, beta):
-#         def fun(t):
-#             return field*np.sin(omega_0*t)+field*beta*np.sin((omega_0+delta)*t)
-#         return fun
-#
-#     sampleNum = 20
-#     endTime = 1 # microseconds
-#     rf = sig_and_LO(2*np.pi*rf_freq, 5, .1)
-#
-#     kpmag = 2*np.pi/780.241e-3 # sets end units correctly to Mrad/s
-#     kcmag = 2*np.pi/480e-3
-#     kp = kpmag*np.array([1,0,0])
-#     kc = kcmag*np.array([-1,0,0])
-#     vP = 242.387
-#     wPp = kp*vP
-#     wPc = kc*vP
-#
-#     d_meth = {"method":"uniform", "n_uniform":50}
-#
-#     red_laser = {'states':(0,1), 'rabi_frequency':2*np.pi*1.0, 'detuning':0, 'kvec':wPp}
-#     blue_laser = {'states':(1,2), 'rabi_frequency':2*np.pi*6.0, 'detuning': 0, 'kvec':wPc}
-#
-#     RbSensor_time.add_fields(blue_laser, red_laser)
-#     RbSensor_time.add_fields({"states":(2,3), "dipole_moment":"auto", "transition_frequency":"auto"})
-#
-#     time, time_sol_ivp = rq.solve_time(RbSensor_time, endTime, sampleNum, rf_input=rf, doppler=True, doppler_mesh_method=d_meth, use_nkode=False)
-#     time, time_sol_nbkode = rq.solve_time(RbSensor_time, endTime, sampleNum, rf_input=rf, doppler=True, doppler_mesh_method=d_meth, use_nkode=True)
-#
-#     np.testing.assert_allclose(time_sol_ivp, time_sol_nbkode, rtol=0.1, err_msg='The difference between two solutions is too big')
+import numpy as np
+import pytest
+
+import rydiqule as rq
+
+
+@pytest.mark.time
+@pytest.mark.slow
+def test_nbkit():
+    """Tests that time solver functions with Doppler broadening
+    """
+    red_laser = {'states':(0,1), 'rabi_frequency':2*np.pi*0.6, 'detuning':0}
+
+    RydbergTargetState = [150, 2, 2.5, 0.5]  # states labeled n, l, j, m_j
+    RydbergExcitedState = [149, 3, 3.5, 0.5]
+
+    RbSensor_time = rq.Cell("Rb85", *rq.D2_states(5),
+                            RydbergTargetState, RydbergExcitedState,
+                            gamma_transit=2*np.pi*.1)
+
+    def rf_carrier(t):
+        return np.sin(2*np.pi*10.0*t)
+
+    sampleNum = 20
+    endTime = 2
+
+    blue_laser = {'states':(1,2), 'rabi_frequency':6.0, 'detuning': 0}
+    rf = {'states':(2,3), 'rabi_frequency':1.0, 'detuning': 0, 'time_dependence': rf_carrier}
+    RbSensor_time.add_couplings(blue_laser, red_laser, rf)
+
+    sols_solve_ivp = rq.solve_time(RbSensor_time, endTime, sampleNum, solver='scipy', rtol=1e-6, atol=1e-6)
+    sols_nbkode = rq.solve_time(RbSensor_time, endTime, sampleNum,  solver='nbkode', rtol=1e-6, atol=1e-6)
+
+    np.testing.assert_allclose(sols_solve_ivp.rho[-1,:], sols_nbkode.rho[-1,:], atol=0.005, err_msg='The difference between two solutions is too big')
+
+
+@pytest.mark.time
+def test_time_complex_match_steady_numbakit():
+    """Tests the time solver vs steady state
+    with aribtrary (complex) and time-dependent rabi frequencies
+    using the numbakitode backend
+    """
+
+    def fun(t):
+        if t < 1:
+            return 0
+        else:
+            return 1
+
+    def fun2(t):
+        if t < 1:
+            return 0j
+        else:
+            return 1j
+
+    end_time = 100
+    sample_num = 20
+
+    probe_t = {'states':(0,1), 'rabi_frequency':4+9j,'detuning':0.3, 'time_dependence': fun}
+    probe_s = {'states':(0,1), 'rabi_frequency':4+9j,'detuning':0.3}
+    dress = {'states':(1,2), 'rabi_frequency':3+2j,'detuning': .7}
+    couple_t = {'states':(2,3), 'rabi_frequency':-9j+1, 'detuning':0.3, 'time_dependence': fun2}
+    couple_s = {'states':(2,3), 'rabi_frequency':9+1j, 'detuning':0.3}
+
+    gam = np.zeros((4,4),dtype=np.float64)
+    gam[1,0] = 0.5
+    gam[2,1] = 0.4
+    gam[3,2] = 0.6
+    gamma_matrix = gam
+
+    sensor_t = rq.Sensor(4)
+    sensor_s = rq.Sensor(4)
+
+    sensor_t.add_couplings(probe_t, dress, couple_t)
+    sensor_t.set_gamma_matrix(gamma_matrix)
+    sensor_s.add_couplings(probe_s, dress, couple_s)
+    sensor_s.set_gamma_matrix(gamma_matrix)
+
+    sols_s = rq.solve_steady_state(sensor_s)
+    sol_t_numba = rq.solve_time(sensor_t, end_time, sample_num, rtol=1E-6, atol=1e-6,
+                                solver='nbkode')
+    np.testing.assert_allclose(sols_s.rho,sol_t_numba.rho[-1,:],atol=0.005,
+           err_msg='Complex time and steady state solutions do not match using numbakit.')
+
+# @pytest.mark.time
+# @pytest.mark.doppler
+# def test_numba_with_doppler():
+#     """Tests that time solver functions with Doppler broadening
+#     """
+#     rf_rabi = 25 #Mrad/s
+#     red_laser = {'states':(0,1), 'rabi_frequency':2*np.pi*0.6}  #fields are stored as dictioniaries
+#     blue_laser = {'states':(1,2), 'rabi_frequency':2*np.pi*2.0, 'detuning': 0}
+#
+#     RbSensor_ss = rq.Cell(gamma_transit=2*np.pi*1, gamma_exc=2*np.pi*6, gamma_Ryd = 2*np.pi*.1)
+#     RbSensor_time = rq.Cell(gamma_transit=2*np.pi*1, gamma_exc=2*np.pi*6, gamma_Ryd = 2*np.pi*.1)
+#
+#     RydbergTargetState = [350, 2, 2.5, 0.5]  #states labeled n, l, j, m_j
+#     RydbergExcitedState = [349, 3, 3.5, 0.5]
+#
+#     RbSensor_ss.add_states(RydbergTargetState,RydbergExcitedState)
+#     RbSensor_time.add_states(RydbergTargetState,RydbergExcitedState)
+#
+#     rf_freq = RbSensor_time.atom.getTransitionFrequency(*RydbergTargetState[:3],*RydbergExcitedState[:3])*1E-6
+#
+#     RbSensor_ss.add_couplings({'states':(2,3), "dipole_moment":"auto", "transition_frequency":"auto"})
+#     rf_dipole_matrix = RbSensor_ss.rf_dipole_matrix()
+#
+#     rf_dipole_moment = rf_dipole_matrix[2,3]
+#     field = 2*rf_rabi/rf_dipole_moment
+#
+#     def sig_and_LO(omega_0, delta, beta):
+#         def fun(t):
+#             return field*np.sin(omega_0*t)+field*beta*np.sin((omega_0+delta)*t)
+#         return fun
+#
+#     sampleNum = 20
+#     endTime = 1 # microseconds
+#     rf = sig_and_LO(2*np.pi*rf_freq, 5, .1)
+#
+#     kpmag = 2*np.pi/780.241e-3 # sets end units correctly to Mrad/s
+#     kcmag = 2*np.pi/480e-3
+#     kp = kpmag*np.array([1,0,0])
+#     kc = kcmag*np.array([-1,0,0])
+#     vP = 242.387
+#     wPp = kp*vP
+#     wPc = kc*vP
+#
+#     d_meth = {"method":"uniform", "n_uniform":50}
+#
+#     red_laser = {'states':(0,1), 'rabi_frequency':2*np.pi*1.0, 'detuning':0, 'kvec':wPp}
+#     blue_laser = {'states':(1,2), 'rabi_frequency':2*np.pi*6.0, 'detuning': 0, 'kvec':wPc}
+#
+#     RbSensor_time.add_fields(blue_laser, red_laser)
+#     RbSensor_time.add_fields({"states":(2,3), "dipole_moment":"auto", "transition_frequency":"auto"})
+#
+#     time, time_sol_ivp = rq.solve_time(RbSensor_time, endTime, sampleNum, rf_input=rf, doppler=True, doppler_mesh_method=d_meth, use_nkode=False)
+#     time, time_sol_nbkode = rq.solve_time(RbSensor_time, endTime, sampleNum, rf_input=rf, doppler=True, doppler_mesh_method=d_meth, use_nkode=True)
+#
+#     np.testing.assert_allclose(time_sol_ivp, time_sol_nbkode, rtol=0.1, err_msg='The difference between two solutions is too big')
```

### Comparing `rydiqule-1.0.0/tests/test_parameter_zip.py` & `rydiqule-1.0.0rc2/tests/test_parameter_zip.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-import numpy as np
-import rydiqule as rq
-import pytest
-
-
-@pytest.mark.structure
-def test_zip_detunings():
-    """
-    Tests that zipping parameters works properly for a simple
-    variable detuning case where red and blue detuning are scanned
-    in parallel for a simple 3-level system.
-    """
-
-    # what the correct hamiltonian will be for this system
-    expected_ham = np.array([[[0. + 0.j,  0.5+0.j,  0. + 0.j],
-                              [0.5-0.j, -2. + 0.j,  1. + 0.j],
-                              [0. + 0.j,  1. - 0.j, -2. + 0.j]],
-
-                             [[0. + 0.j,  0.5+0.j,  0. + 0.j],
-                              [0.5-0.j, -1. + 0.j,  1. + 0.j],
-                              [0. + 0.j,  1. - 0.j,  0. + 0.j]],
-
-                             [[0. + 0.j,  0.5+0.j,  0. + 0.j],
-                              [0.5-0.j,  0. + 0.j,  1. + 0.j],
-                              [0. + 0.j,  1. - 0.j,  2. + 0.j]],
-
-                             [[0. + 0.j,  0.5+0.j,  0. + 0.j],
-                              [0.5-0.j,  1. + 0.j,  1. + 0.j],
-                              [0. + 0.j,  1. - 0.j,  4. + 0.j]],
-
-                             [[0. + 0.j,  0.5+0.j,  0. + 0.j],
-                              [0.5-0.j,  2. + 0.j,  1. + 0.j],
-                              [0. + 0.j,  1. - 0.j,  6. + 0.j]]])
-
-    s = rq.Sensor(3)
-    detunings_red = np.linspace(-2, 2, 5)
-    detunings_blue = 2 + detunings_red
-
-    red = {"states": (0,1), "detuning": detunings_red, "rabi_frequency": 1, "label": "red"}
-    blue = {"states": (1,2), "detuning": detunings_blue, "rabi_frequency": 2, "label": "blue"}
-
-    s.add_couplings(red, blue)
-    s.zip_parameters("red_detuning", "blue_detuning")
-
-    test_ham = s.get_hamiltonian()
-
-    np.testing.assert_equal(test_ham, expected_ham)
-
-
-@pytest.mark.structure
-def test_zip_rabi():
-    """
-    Tests that zipping parameters works properly for a simple
-    variable rabi case where red and blue rabi_frequency are scanned
-    in parallel for a simple 3-level system.
-    """
-
-    expected_ham = np.array([[[0. + 0.j, 0.5+0.j, 0. + 0.j],
-                              [0.5-0.j, 0. + 0.j, 1. + 0.j],
-                              [0. + 0.j, 1. - 0.j, 0. + 0.j]],
-
-                             [[0. + 0.j, 1. + 0.j, 0. + 0.j],
-                              [1. - 0.j, 0. + 0.j, 2. + 0.j],
-                              [0. + 0.j, 2. - 0.j, 0. + 0.j]],
-
-                             [[0. + 0.j, 1.5+0.j, 0. + 0.j],
-                              [1.5-0.j, 0. + 0.j, 3. + 0.j],
-                              [0. + 0.j, 3. - 0.j, 0. + 0.j]],
-
-                             [[0. + 0.j, 2. + 0.j, 0. + 0.j],
-                              [2. - 0.j, 0. + 0.j, 4. + 0.j],
-                              [0. + 0.j, 4. - 0.j, 0. + 0.j]],
-
-                             [[0. + 0.j, 2.5+0.j, 0. + 0.j],
-                              [2.5-0.j, 0. + 0.j, 5. + 0.j],
-                              [0. + 0.j, 5. - 0.j, 0. + 0.j]]])
-
-    s = rq.Sensor(3)
-    rabi_red = np.linspace(1, 5, 5)
-    rabi_blue = 2 * rabi_red
-
-    red = {"states": (0,1), "detuning": 0, "rabi_frequency": rabi_red}
-    blue = {"states": (1,2), "detuning": 0, "rabi_frequency": rabi_blue}
-
-    s.add_couplings(red, blue)
-    s.zip_parameters("(0,1)_rabi_frequency", "(1,2)_rabi_frequency")
-
-    test_ham = s.get_hamiltonian()
-    np.testing.assert_equal(test_ham, expected_ham)
-
-
-@pytest.mark.structure
-def test_zip_phase():
-    """
-    Tests that zipping parameters works properly for a simple
-    variable phase case where red and blue phase are scanned
-    in parallel for a simple 3-level system.
-    """
-    expected_ham = np.array([[[0. + 0.j, 0. - 0.5j, 0. + 0.j],
-                              [0. + 0.5j, 0. + 0.j, 0. - 1.j],
-                              [0. + 0.j, 0. + 1.j, 0. + 0.j]],
-
-                             [[0. + 0.j, 0.35355-0.35355j, 0. + 0.j],
-                              [0.35355+0.35355j, 0. + 0.j, 0.70711-0.70711j],
-                              [0. + 0.j, 0.70711+0.70711j, 0. + 0.j]],
-
-                             [[0. + 0.j, 0.5 + 0.j, 0. + 0.j],
-                              [0.5 - 0.j, 0. + 0.j, 1. + 0.j],
-                              [0. + 0.j, 1. - 0.j, 0. + 0.j]],
-
-                             [[0. + 0.j, 0.35355+0.35355j, 0. + 0.j],
-                              [0.35355-0.35355j, 0. + 0.j, 0.70711+0.70711j],
-                              [0. + 0.j, 0.70711-0.70711j, 0. + 0.j]],
-
-                             [[0. + 0.j, 0. + 0.5j, 0. + 0.j],
-                              [0. - 0.5j, 0. + 0.j, 0. + 1.j],
-                              [0. + 0.j, 0. - 1.j, 0. + 0.j]]])
-
-    s = rq.Sensor(3)
-    phases = np.pi/2 * np.linspace(-1, 1, 5)
-
-    red = {"states": (0,1), "detuning": 0, "rabi_frequency": 1, "phase": phases}
-    blue = {"states": (1,2), "detuning": 0, "rabi_frequency": 2, "phase": phases}
-
-    s.add_couplings(red, blue)
-    s.zip_parameters("(0,1)_phase", "(1,2)_phase")
-
-    test_ham = s.get_hamiltonian()
-    np.testing.assert_allclose(expected_ham, test_ham, atol=1e-4)
+import numpy as np
+import rydiqule as rq
+import pytest
+
+
+@pytest.mark.structure
+def test_zip_detunings():
+    """
+    Tests that zipping parameters works properly for a simple
+    variable detuning case where red and blue detuning are scanned
+    in parallel for a simple 3-level system.
+    """
+
+    # what the correct hamiltonian will be for this system
+    expected_ham = np.array([[[0. + 0.j,  0.5+0.j,  0. + 0.j],
+                              [0.5-0.j, -2. + 0.j,  1. + 0.j],
+                              [0. + 0.j,  1. - 0.j, -2. + 0.j]],
+
+                             [[0. + 0.j,  0.5+0.j,  0. + 0.j],
+                              [0.5-0.j, -1. + 0.j,  1. + 0.j],
+                              [0. + 0.j,  1. - 0.j,  0. + 0.j]],
+
+                             [[0. + 0.j,  0.5+0.j,  0. + 0.j],
+                              [0.5-0.j,  0. + 0.j,  1. + 0.j],
+                              [0. + 0.j,  1. - 0.j,  2. + 0.j]],
+
+                             [[0. + 0.j,  0.5+0.j,  0. + 0.j],
+                              [0.5-0.j,  1. + 0.j,  1. + 0.j],
+                              [0. + 0.j,  1. - 0.j,  4. + 0.j]],
+
+                             [[0. + 0.j,  0.5+0.j,  0. + 0.j],
+                              [0.5-0.j,  2. + 0.j,  1. + 0.j],
+                              [0. + 0.j,  1. - 0.j,  6. + 0.j]]])
+
+    s = rq.Sensor(3)
+    detunings_red = np.linspace(-2, 2, 5)
+    detunings_blue = 2 + detunings_red
+
+    red = {"states": (0,1), "detuning": detunings_red, "rabi_frequency": 1, "label": "red"}
+    blue = {"states": (1,2), "detuning": detunings_blue, "rabi_frequency": 2, "label": "blue"}
+
+    s.add_couplings(red, blue)
+    s.zip_parameters("red_detuning", "blue_detuning")
+
+    test_ham = s.get_hamiltonian()
+
+    np.testing.assert_equal(test_ham, expected_ham)
+
+
+@pytest.mark.structure
+def test_zip_rabi():
+    """
+    Tests that zipping parameters works properly for a simple
+    variable rabi case where red and blue rabi_frequency are scanned
+    in parallel for a simple 3-level system.
+    """
+
+    expected_ham = np.array([[[0. + 0.j, 0.5+0.j, 0. + 0.j],
+                              [0.5-0.j, 0. + 0.j, 1. + 0.j],
+                              [0. + 0.j, 1. - 0.j, 0. + 0.j]],
+
+                             [[0. + 0.j, 1. + 0.j, 0. + 0.j],
+                              [1. - 0.j, 0. + 0.j, 2. + 0.j],
+                              [0. + 0.j, 2. - 0.j, 0. + 0.j]],
+
+                             [[0. + 0.j, 1.5+0.j, 0. + 0.j],
+                              [1.5-0.j, 0. + 0.j, 3. + 0.j],
+                              [0. + 0.j, 3. - 0.j, 0. + 0.j]],
+
+                             [[0. + 0.j, 2. + 0.j, 0. + 0.j],
+                              [2. - 0.j, 0. + 0.j, 4. + 0.j],
+                              [0. + 0.j, 4. - 0.j, 0. + 0.j]],
+
+                             [[0. + 0.j, 2.5+0.j, 0. + 0.j],
+                              [2.5-0.j, 0. + 0.j, 5. + 0.j],
+                              [0. + 0.j, 5. - 0.j, 0. + 0.j]]])
+
+    s = rq.Sensor(3)
+    rabi_red = np.linspace(1, 5, 5)
+    rabi_blue = 2 * rabi_red
+
+    red = {"states": (0,1), "detuning": 0, "rabi_frequency": rabi_red}
+    blue = {"states": (1,2), "detuning": 0, "rabi_frequency": rabi_blue}
+
+    s.add_couplings(red, blue)
+    s.zip_parameters("(0,1)_rabi_frequency", "(1,2)_rabi_frequency")
+
+    test_ham = s.get_hamiltonian()
+    np.testing.assert_equal(test_ham, expected_ham)
+
+
+@pytest.mark.structure
+def test_zip_phase():
+    """
+    Tests that zipping parameters works properly for a simple
+    variable phase case where red and blue phase are scanned
+    in parallel for a simple 3-level system.
+    """
+    expected_ham = np.array([[[0. + 0.j, 0. - 0.5j, 0. + 0.j],
+                              [0. + 0.5j, 0. + 0.j, 0. - 1.j],
+                              [0. + 0.j, 0. + 1.j, 0. + 0.j]],
+
+                             [[0. + 0.j, 0.35355-0.35355j, 0. + 0.j],
+                              [0.35355+0.35355j, 0. + 0.j, 0.70711-0.70711j],
+                              [0. + 0.j, 0.70711+0.70711j, 0. + 0.j]],
+
+                             [[0. + 0.j, 0.5 + 0.j, 0. + 0.j],
+                              [0.5 - 0.j, 0. + 0.j, 1. + 0.j],
+                              [0. + 0.j, 1. - 0.j, 0. + 0.j]],
+
+                             [[0. + 0.j, 0.35355+0.35355j, 0. + 0.j],
+                              [0.35355-0.35355j, 0. + 0.j, 0.70711+0.70711j],
+                              [0. + 0.j, 0.70711-0.70711j, 0. + 0.j]],
+
+                             [[0. + 0.j, 0. + 0.5j, 0. + 0.j],
+                              [0. - 0.5j, 0. + 0.j, 0. + 1.j],
+                              [0. + 0.j, 0. - 1.j, 0. + 0.j]]])
+
+    s = rq.Sensor(3)
+    phases = np.pi/2 * np.linspace(-1, 1, 5)
+
+    red = {"states": (0,1), "detuning": 0, "rabi_frequency": 1, "phase": phases}
+    blue = {"states": (1,2), "detuning": 0, "rabi_frequency": 2, "phase": phases}
+
+    s.add_couplings(red, blue)
+    s.zip_parameters("(0,1)_phase", "(1,2)_phase")
+
+    test_ham = s.get_hamiltonian()
+    np.testing.assert_allclose(expected_ham, test_ham, atol=1e-4)
```

### Comparing `rydiqule-1.0.0/tests/test_sensor.py` & `rydiqule-1.0.0rc2/tests/test_sensor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-import numpy as np
-import rydiqule as rq
-import pytest
-import warnings
-
-
-@pytest.mark.structure
-def test_detunings():
-    """Tests that detunings are properly accounted for."""
-
-    s = rq.Sensor(4)
-    f1 = {'states':(0,1), 'rabi_frequency':0, 'detuning':1}
-    f2 = {'states':(1,2), 'rabi_frequency':0, 'detuning':2}
-    f3 = {'states':(2,3), 'rabi_frequency':0, 'detuning':4}
-    s.add_couplings(f1,f2,f3)
-    ham = s.get_hamiltonian()
-
-    expected_ham = np.diag([0,1,1+2,1+2+4]).astype(np.complex128)
-
-    np.testing.assert_allclose(ham, expected_ham, err_msg='4-level ladder detunings not correct')
-
-
-@pytest.mark.structure
-def test_dephasings():
-    """Tests that decoherence matrix is made correctly, with higher dimensions."""
-
-    b = 4
-    g10 = 1
-    g21 = np.array([0.1, 0.2, 0.5, 1.0])
-    g22 = 5
-    g32 = 0.01
-    g13 = 0.7
-    gt = [4, 6, 8]
-
-    gam_exp = np.zeros((len(g21), len(gt), b,b),dtype=float)
-    gam_exp[...,1,0] = g10
-    gam_exp[...,2,2] = g22
-    gam_exp[...,3,2] = g32
-    gam_exp[...,1,3] = g13
-    gam_exp[...,2,1] = g21[:,np.newaxis]
-    gam_exp[...,0] += np.array(gt)[np.newaxis,:,np.newaxis]*0.6
-    gam_exp[...,1] += np.array(gt)[np.newaxis,:,np.newaxis]*0.4
-
-    s = rq.Sensor(b)
-    s.add_decoherence((1,0), g10)
-    s.add_decoherence((2,1), g21)
-    s.add_self_broadening(2, g22)
-    s.add_decoherence((3,2), g32)
-    s.add_decoherence((1,3), g13)
-    s.add_transit_broadening(gt, {0:0.6, 1:0.4})
-    s_gam = s.decoherence_matrix()
-
-    np.testing.assert_allclose(s_gam, gam_exp, err_msg='Sensor decoherence matrix incorrect')
-
-
-@pytest.mark.exception
-def test_coupling_exceptions():
-    '''Confirms the bad input fields to add_coupling raise correct exceptions.
-    '''
-
-    s = rq.Sensor(2)
-
-    with pytest.raises(ValueError):
-        # specify both detuning and transition frequency
-        f1 = {'states':(0,1), 'detuning':0, 'transition_frequency':1}
-        s.add_coupling(**f1)
-
-    with pytest.warns(UserWarning):
-        # checks for warning about likely accidental RWA violation
-        f2 = {'states':(0,1), 'transition_frequency': 5001}
-        s.add_coupling(**f2)
-
-    # RWA violation should not be shown
-    with warnings.catch_warnings(record=True) as record:
-        f3 = {'states':(0,1), 'transition_frequency': 5001, 'suppress_rwa_warn':True}
-        s.add_coupling(**f3)
-
-        assert len(record) == 0, 'RWA warning not supressed'
-
-    with pytest.raises(ValueError, match="\'states\' parameter must be specified for any field"):
-        f4 = {'detuning':0, 'rabi_frequency':20}
-        s.add_couplings(f4)
-
-    with pytest.raises(ValueError, match='non-zero kvector'):
-        f5 = {'states':(0,1), 'detuning':0}
-        s.add_couplings(f5)
-        s.get_doppler_shifts()
-
-    with pytest.raises(ValueError):
-        f6 = {'states': (0,0), 'detuning':0, 'rabi_frequency':1}
-        s.add_couplings(f6)
-
-
-@pytest.mark.exception
-def test_states_validation():
-    '''Assures that bad state specifications a caught.'''
-
-    s = rq.Sensor(2)
-
-    with pytest.raises(ValueError, match='cannot be interpreted as a tuple'):
-        # bad input type
-        s._states_valid(1.0)
-
-    with pytest.raises(ValueError, match='must couple exactly 2 states'):
-        # too many labels passed
-        s._states_valid((0,1,2))
-
-    with pytest.raises(TypeError, match='must be an integer'):
-        # non-integer inputs
-        s._states_valid('01')
-
-    with pytest.raises(ValueError, match='outside the basis size'):
-        # outside basis
-        s._states_valid((0,2))
-
-
-@pytest.mark.exception
-def test_zip_param_validation():
-    '''Assures that incorrect usage of Sensor.zip_parameters is caught.'''
-
-    s = rq.Sensor(3)
-
-    f1 = {'states':(0,1), 'detuning': [1,2,3], 'rabi_frequency':10, 'label':'f1'}
-    f2 = {'states':(1,2), 'detuning': [1,2,3], 'rabi_frequency':[10,11,12, 13], 'label':'f2'}
-    s.add_couplings(f1,f2)
-
-    with pytest.raises(ValueError, match='provide at least 2'):
-        s.zip_parameters('f1_detuning')
-
-    with pytest.raises(ValueError, match='not a label of any coupling'):
-        s.zip_parameters('f1_detuning', 'f3_detuning')
-
-    with pytest.raises(ValueError, match='Got length'):
-        s.zip_parameters('f1_detuning', 'f2_rabi_frequency')
-
-@pytest.mark.exception
-def test_gamma_matrix_validation():
-    '''Confirms that validation checks trigger for bad gamma matrices.'''
-
-    s = rq.Sensor(2)
-
-    with pytest.raises(TypeError, match='must be a numpy array'):
-        gam = [[0,1], [1,0]]
-        s.set_gamma_matrix(gam)
-
-    with pytest.raises(ValueError, match='gamma_matrix has shape'):
-        gam = np.array([[0,1,2],[1,0,2],[2,1,0]])
-        s.set_gamma_matrix(gam)
+import numpy as np
+import rydiqule as rq
+import pytest
+import warnings
+
+
+@pytest.mark.structure
+def test_detunings():
+    """Tests that detunings are properly accounted for."""
+
+    s = rq.Sensor(4)
+    f1 = {'states':(0,1), 'rabi_frequency':0, 'detuning':1}
+    f2 = {'states':(1,2), 'rabi_frequency':0, 'detuning':2}
+    f3 = {'states':(2,3), 'rabi_frequency':0, 'detuning':4}
+    s.add_couplings(f1,f2,f3)
+    ham = s.get_hamiltonian()
+
+    expected_ham = np.diag([0,1,1+2,1+2+4]).astype(np.complex128)
+
+    np.testing.assert_allclose(ham, expected_ham, err_msg='4-level ladder detunings not correct')
+
+
+@pytest.mark.structure
+def test_dephasings():
+    """Tests that decoherence matrix is made correctly, with higher dimensions."""
+
+    b = 4
+    g10 = 1
+    g21 = np.array([0.1, 0.2, 0.5, 1.0])
+    g22 = 5
+    g32 = 0.01
+    g13 = 0.7
+    gt = [4, 6, 8]
+
+    gam_exp = np.zeros((len(g21), len(gt), b,b),dtype=float)
+    gam_exp[...,1,0] = g10
+    gam_exp[...,2,2] = g22
+    gam_exp[...,3,2] = g32
+    gam_exp[...,1,3] = g13
+    gam_exp[...,2,1] = g21[:,np.newaxis]
+    gam_exp[...,0] += np.array(gt)[np.newaxis,:,np.newaxis]*0.6
+    gam_exp[...,1] += np.array(gt)[np.newaxis,:,np.newaxis]*0.4
+
+    s = rq.Sensor(b)
+    s.add_decoherence((1,0), g10)
+    s.add_decoherence((2,1), g21)
+    s.add_self_broadening(2, g22)
+    s.add_decoherence((3,2), g32)
+    s.add_decoherence((1,3), g13)
+    s.add_transit_broadening(gt, {0:0.6, 1:0.4})
+    s_gam = s.decoherence_matrix()
+
+    np.testing.assert_allclose(s_gam, gam_exp, err_msg='Sensor decoherence matrix incorrect')
+
+
+@pytest.mark.exception
+def test_coupling_exceptions():
+    '''Confirms the bad input fields to add_coupling raise correct exceptions.
+    '''
+
+    s = rq.Sensor(2)
+
+    with pytest.raises(ValueError):
+        # specify both detuning and transition frequency
+        f1 = {'states':(0,1), 'detuning':0, 'transition_frequency':1}
+        s.add_coupling(**f1)
+
+    with pytest.warns(UserWarning):
+        # checks for warning about likely accidental RWA violation
+        f2 = {'states':(0,1), 'transition_frequency': 5001}
+        s.add_coupling(**f2)
+
+    # RWA violation should not be shown
+    with warnings.catch_warnings(record=True) as record:
+        f3 = {'states':(0,1), 'transition_frequency': 5001, 'supress_rwa_warning':True}
+        s.add_coupling(**f3)
+
+        assert len(record) == 0, 'RWA warning not supressed'
+
+    with pytest.raises(ValueError, match="\'states\' parameter must be specified for any field"):
+        f4 = {'detuning':0, 'rabi_frequency':20}
+        s.add_couplings(f4)
+
+    with pytest.raises(ValueError, match='non-zero kvector'):
+        f5 = {'states':(0,1), 'detuning':0}
+        s.add_couplings(f5)
+        s.get_doppler_shifts()
+
+    with pytest.raises(ValueError):
+        f6 = {'states': (0,0), 'detuning':0, 'rabi_frequency':1}
+        s.add_couplings(f6)
+
+
+@pytest.mark.exception
+def test_states_validation():
+    '''Assures that bad state specifications a caught.'''
+
+    s = rq.Sensor(2)
+
+    with pytest.raises(ValueError, match='cannot be interpreted as a tuple'):
+        # bad input type
+        s._states_valid(1.0)
+
+    with pytest.raises(ValueError, match='must couple exactly 2 states'):
+        # too many labels passed
+        s._states_valid((0,1,2))
+
+    with pytest.raises(TypeError, match='must be an integer'):
+        # non-integer inputs
+        s._states_valid('01')
+
+    with pytest.raises(ValueError, match='outside the basis size'):
+        # outside basis
+        s._states_valid((0,2))
+
+
+@pytest.mark.exception
+def test_zip_param_validation():
+    '''Assures that incorrect usage of Sensor.zip_parameters is caught.'''
+
+    s = rq.Sensor(3)
+
+    f1 = {'states':(0,1), 'detuning': [1,2,3], 'rabi_frequency':10, 'label':'f1'}
+    f2 = {'states':(1,2), 'detuning': [1,2,3], 'rabi_frequency':[10,11,12, 13], 'label':'f2'}
+    s.add_couplings(f1,f2)
+
+    with pytest.raises(ValueError, match='provide at least 2'):
+        s.zip_parameters('f1_detuning')
+
+    with pytest.raises(ValueError, match='not a label of any coupling'):
+        s.zip_parameters('f1_detuning', 'f3_detuning')
+
+    with pytest.raises(ValueError, match='Got length'):
+        s.zip_parameters('f1_detuning', 'f2_rabi_frequency')
+
+@pytest.mark.exception
+def test_gamma_matrix_validation():
+    '''Confirms that validation checks trigger for bad gamma matrices.'''
+
+    s = rq.Sensor(2)
+
+    with pytest.raises(TypeError, match='must be a numpy array'):
+        gam = [[0,1], [1,0]]
+        s.set_gamma_matrix(gam)
+
+    with pytest.raises(ValueError, match='gamma_matrix has shape'):
+        gam = np.array([[0,1,2],[1,0,2],[2,1,0]])
+        s.set_gamma_matrix(gam)
```

### Comparing `rydiqule-1.0.0/tests/test_solvers.py` & `rydiqule-1.0.0rc2/tests/test_solvers.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,285 +1,285 @@
-import numpy as np
-import rydiqule as rq
-from rydiqule.sensor_utils import get_rho_ij
-import pytest
-
-
-@pytest.mark.steady_state
-def test_linewidths():
-    """Confirms that doppler-free linewidths are correct
-    and that dephasing broadcasting is working.
-    """
-
-    gammas = np.array([1.0, 4.28, 9.17, 12.0])
-    s = rq.Sensor(2)
-
-    detunings = np.linspace(-10,10,201)
-
-    probe = {'states':(0,1), 'rabi_frequency': 0.01, 'detuning':2*np.pi*detunings}
-
-    s.add_decoherence((1,0), 2*np.pi*gammas)
-    s.add_couplings(probe)
-
-    sols = rq.solve_steady_state(s).rho
-    isols = rq.get_rho_ij(sols, 1, 0).imag
-
-    sol_ind = s.axis_labels().index('(0,1)_detuning')
-    meas_gammas = np.abs(detunings[np.abs(isols - np.expand_dims(isols.max(axis=sol_ind),sol_ind)/2).argmin(axis=sol_ind)])*2
-    # use relatively loose abstol since width finding is so crude
-    np.testing.assert_allclose(meas_gammas, gammas, rtol=0, atol=0.1,
-                               err_msg='2-level absorption linewidths do not match')
-
-
-@pytest.mark.steady_state
-@pytest.mark.util
-def test_ham_slicing():
-    """Confirms that breaking up the system during solves norminally works"""
-
-    s = rq.Sensor(3)
-    s.add_decoherence((1,0), 2*np.pi*6.0666)
-    s.add_decoherence((2,1), 2*np.pi*10e-3)
-    s.add_transit_broadening(2*np.pi*100e-3)
-
-    detunings = np.linspace(-10,10,41)
-    probe = {'states':(0,1), 'rabi_frequency':2*np.pi*0.1, 'detuning':2*np.pi*detunings, 'label':'probe'}
-    couple = {'states':(1,2), 'rabi_frequency':2*np.pi*1, 'detuning':0, 'label':'couple'}
-
-    s.add_couplings(probe,couple)
-
-    # if slicing is broken, error will occur here
-    sols = rq.solve_steady_state(s,n_slices=4)
-    disp = sols.rho_ij(1,0).real
-
-    # do a couple simple checks to roughly confirm output is dispersive
-    zero_cross_ind = np.where(disp == 0)[0].squeeze()
-    zero_cross = detunings[zero_cross_ind]
-
-    assert zero_cross == pytest.approx(0.0), 'Resonance not resonant!'
-    assert disp.max() == pytest.approx(-disp.min()), 'Resonance not symmetric!'
-
-
-@pytest.mark.steady_state
-@pytest.mark.parametrize("rf_rabi", np.linspace(1.0, 20.0, 5))  # in MHz
-def test_DopFree_AT(find_zero_crossings, rf_rabi):
-    """Confirms that the expected Autler-Townes splitting is generated
-    in steady state without Doppler averaging or optical depth.
-    """
-
-    basis_size = 4
-    s = rq.Sensor(basis_size)
-    transit = 100e-3
-    gamma = 5.75
-    ryd_lifetime = 1e-3
-    gam = np.zeros((s.basis_size,s.basis_size),dtype=np.float64)
-    gam[1,0] = gamma
-    gam[2,1] = ryd_lifetime
-    gam[3,1] = ryd_lifetime
-    gam[:,0] += transit
-    s.set_gamma_matrix(2*np.pi*gam)
-
-    detunings = np.linspace(-15, 15, 301)
-    probe = {'states':(0,1), 'rabi_frequency':2*np.pi*0.1, 'detuning':0}
-    coupling = {'states':(1,2), 'rabi_frequency': 2*np.pi*0.6, 'detuning':2*np.pi*detunings}
-    rf = {'states':(2,3), 'rabi_frequency': 2*np.pi*rf_rabi, 'detuning':0}
-
-    s.add_couplings(probe,coupling,rf)
-    sols = rq.solve_steady_state(s).rho
-    rsols = get_rho_ij(sols, 1,0).real
-
-    # detect expected zero crossings in phase shift vs detuning
-    # this will give us the AT splitting
-    det_crossings = find_zero_crossings(rsols,detunings)
-
-    # ensure we got the right number of crossings
-    assert len(det_crossings) == 2
-
-    AT_splitting = det_crossings[-1] - det_crossings[0]
-
-    # tolerances set conservatively at 1% relative and 0.1 MHz absolute
-    assert AT_splitting == pytest.approx(rf_rabi, rel=1e-2, abs=1e-1), \
-        f'Expected AT={rf_rabi:.2f}, got {AT_splitting:.2f}'
-
-
-@pytest.mark.steady_state
-@pytest.mark.doppler
-@pytest.mark.parametrize("rf_rabi", np.linspace(8.0, 20.0, 5))  # in MHz
-def test_Dop_AT_couple(find_zero_crossings, rf_rabi):
-    """Confirms that the expected Autler-Townes splitting is generated
-    in steady state with Doppler averaging. For a coupling sweep, AT = rf_rabi
-    """
-
-    basis_size = 4
-    s = rq.Sensor(basis_size)
-    transit = 100e-3
-    gamma = 6.0666
-    ryd_lifetime = 1e-3
-    gam = np.zeros((s.basis_size,s.basis_size),dtype=np.float64)
-    gam[1,0] = gamma
-    gam[2,1] = ryd_lifetime
-    gam[3,1] = ryd_lifetime
-    gam[:,0] += transit
-    s.set_gamma_matrix(2*np.pi*gam)
-
-    # values correspond to Rb D2 scheme
-    kpmag = 2*np.pi/780.241e-3  # sets end units correctly to Mrad/s
-    kcmag = 2*np.pi/480e-3
-    kp = kpmag*np.array([1,0,0])
-    kc = kcmag*np.array([-1,0,0])
-    vP = 242.387  # Rb85
-    wPp = kp*vP
-    wPc = kc*vP
-
-    detunings = np.linspace(-15, 15, 301)
-    probe = {'states':(0,1), 'rabi_frequency':2*np.pi*1.5, 'detuning':0, 'kvec':wPp}
-    coupling = {'states':(1,2), 'rabi_frequency': 2*np.pi*4.0, 'detuning':2*np.pi*detunings,
-                'kvec':wPc}
-    rf = {'states':(2,3), 'rabi_frequency': 2*np.pi*rf_rabi, 'detuning':0}
-
-    s.add_couplings(probe,coupling,rf)
-    sols = rq.solve_steady_state(s,doppler=True).rho
-    rsols = get_rho_ij(sols, 1,0).real
-
-    # detect expected zero crossings in phase shift vs detuning
-    # this will give us the AT splitting
-    det_crossings = find_zero_crossings(rsols,detunings)
-
-    # ensure splitting is actually symmetric
-    assert det_crossings[-1] == pytest.approx(-det_crossings[0],rel=1e-2), \
-        'Assymetric AT splitting detected'
-
-    AT_splitting = det_crossings[-1] - det_crossings[0]
-
-    # tolerances set conservatively at 1% relative and 0.1 MHz absolute
-    assert AT_splitting == pytest.approx(rf_rabi, rel=1e-2, abs=1e-1), \
-        f'Expected AT={rf_rabi:.2f}, got {AT_splitting:.2f}'
-
-
-@pytest.mark.steady_state
-@pytest.mark.doppler
-@pytest.mark.parametrize("rf_rabi", np.linspace(8.0, 20.0, 5))  # in MHz
-def test_Dop_AT_probe(find_zero_crossings, rf_rabi):
-    """Confirms that the expected Autler-Townes splitting is generated
-    in steady state with Doppler averaging. For a coupling sweep, AT = kp/kc*rf_rabi
-    """
-
-    basis_size = 4
-    s = rq.Sensor(basis_size)
-    transit = 100e-3
-    gamma = 6.0666
-    ryd_lifetime = 1e-3
-    gam = np.zeros((s.basis_size,s.basis_size),dtype=np.float64)
-    gam[1,0] = gamma
-    gam[2,1] = ryd_lifetime
-    gam[3,1] = ryd_lifetime
-    gam[:,0] += transit
-    s.set_gamma_matrix(2*np.pi*gam)
-
-    # values correspond to Rb D2 scheme
-    kpmag = 2*np.pi/780.241e-3  # sets end units correctly to Mrad/s
-    kcmag = 2*np.pi/480e-3
-    kp = kpmag*np.array([1,0,0])
-    kc = kcmag*np.array([-1,0,0])
-    vP = 242.387
-    wPp = kp*vP
-    wPc = kc*vP
-
-    detunings = np.linspace(-15, 15, 301)
-    probe = {'states':(0,1), 'rabi_frequency':2*np.pi*1.5,'detuning':2*np.pi*detunings, 'kvec':wPp}
-    coupling = {'states':(1,2), 'rabi_frequency': 2*np.pi*4.0, 'detuning':0, 'kvec':wPc}
-    rf = {'states':(2,3), 'rabi_frequency': 2*np.pi*rf_rabi, 'detuning':0}
-
-    s.add_couplings(probe,coupling,rf)
-    sols = rq.solve_steady_state(s, doppler=True).rho
-    rsols = get_rho_ij(sols, 1,0).real
-
-    # detect expected zero crossings in phase shift vs detuning
-    # this will give us the AT splitting
-    det_crossings = find_zero_crossings(rsols,detunings)
-
-    # ensure splitting is actually symmetric
-    assert det_crossings[-1] == pytest.approx(-det_crossings[0],rel=1e-2), \
-        'Assymetric AT splitting detected'
-
-    AT_splitting = det_crossings[-1] - det_crossings[0]
-
-    # tolerances set conservatively at 1% relative and 0.25 MHz absolute
-    expAT = kpmag/kcmag*rf_rabi
-    assert AT_splitting == pytest.approx(expAT, rel=1e-2, abs=2.5e-1), \
-        f'Expected AT={expAT:.2f}, got {AT_splitting:.2f}'
-
-
-@pytest.mark.steady_state
-@pytest.mark.doppler
-def test_Dop_2level():
-    """Checks that simple doppler broadening of the probing transition
-    is correctly calculated by the doppler averaging.
-    """
-
-    from scipy.optimize import curve_fit
-    from scipy.constants import k,c
-    from arc import Rubidium85
-
-    # get actual atom parameters to compare against
-    atom = Rubidium85()
-    gState = [5,0,0.5]
-    iState = [5,1,1.5]
-    f0 = atom.getTransitionFrequency(*gState,*iState)
-    gamma = atom.getTransitionRate(*iState,*gState)/2/np.pi*1e-6
-    mRb85 = atom.mass
-    T = 300
-
-    # define out 2-level system
-    basis_size = 2
-    s = rq.Sensor(basis_size)
-    gam = np.zeros((s.basis_size,s.basis_size),dtype=np.float64)
-    gam[1,0] = gamma
-    s.set_gamma_matrix(2*np.pi*gam)
-
-    kpmag = 2*np.pi/780.241e-3  # sets end units correctly to Mrad/s
-    kp = kpmag*np.array([1,0,0])
-    vP = np.sqrt(2*k*T/mRb85)
-    wPp = kp*vP
-
-    # calculate the theoretical doppler width for this transition, in MHz
-    actualWidth = vP*np.sqrt(4*np.log(2)/c**2)*f0*1e-6
-
-    # calculate the doppler absorption profile
-    detunings = np.linspace(-750, 750, 301)
-    probe = {'states':(0,1), 'rabi_frequency':2*np.pi*1.5,'detuning':2*np.pi*detunings,'kvec':wPp}
-
-    s.add_couplings(probe)
-    sols = rq.solve_steady_state(s,doppler=True,
-                                 doppler_mesh_method={'method':'uniform','wDop':2.5}).rho
-
-    def gaussFit(f,A,w):
-        return A*np.exp(-f**2/(2*w**2))
-
-    rho10imag = get_rho_ij(sols, 1,0).imag
-    maxval_init = rho10imag.max()
-    p0 = [maxval_init,200]
-    popt,pcov = curve_fit(gaussFit,detunings,rho10imag,p0=p0)
-
-    measuredWidth = popt[1]*2*np.sqrt(2*np.log(2))
-
-    # confirm measured width is within 2% of theorectical
-    assert measuredWidth == pytest.approx(actualWidth,rel=2e-2), \
-        f'Doppler width of Rb85 D2 transition not correct'
-
-
-@pytest.mark.exception
-def test_solve_memory_fits():
-    '''Confirms that checks for EOMs fitting in memory fail when appropriate.'''
-
-    with pytest.raises(MemoryError, match='sum_doppler=False'):
-        # We do not support sum_doppler=False when full solve does not fit in memory
-        n = 4
-        stack = (101, 101)
-        doppler_stack = (561, 561)
-        rq.get_slice_num(n, stack, doppler_stack, sum_doppler=False, weight_doppler=True)
-
-    with pytest.raises(MemoryError, match='System is too large'):
-        # this system requires 335.4 GiB
-        n = 4
-        stack = (101, 101)
-        doppler_stack = (561, 561, 561)
-        rq.get_slice_num(n, stack, doppler_stack, sum_doppler=True, weight_doppler=True)
+import numpy as np
+import rydiqule as rq
+from rydiqule.sensor_utils import get_rho_ij
+import pytest
+
+
+@pytest.mark.steady_state
+def test_linewidths():
+    """Confirms that doppler-free linewidths are correct
+    and that dephasing broadcasting is working.
+    """
+
+    gammas = np.array([1.0, 4.28, 9.17, 12.0])
+    s = rq.Sensor(2)
+
+    detunings = np.linspace(-10,10,201)
+
+    probe = {'states':(0,1), 'rabi_frequency': 0.01, 'detuning':2*np.pi*detunings}
+
+    s.add_decoherence((1,0), 2*np.pi*gammas)
+    s.add_couplings(probe)
+
+    sols = rq.solve_steady_state(s).rho
+    isols = rq.get_rho_ij(sols, 1, 0).imag
+
+    sol_ind = s.axis_labels().index('(0,1)_detuning')
+    meas_gammas = np.abs(detunings[np.abs(isols - np.expand_dims(isols.max(axis=sol_ind),sol_ind)/2).argmin(axis=sol_ind)])*2
+    # use relatively loose abstol since width finding is so crude
+    np.testing.assert_allclose(meas_gammas, gammas, rtol=0, atol=0.1,
+                               err_msg='2-level absorption linewidths do not match')
+
+
+@pytest.mark.steady_state
+@pytest.mark.util
+def test_ham_slicing():
+    """Confirms that breaking up the system during solves norminally works"""
+
+    s = rq.Sensor(3)
+    s.add_decoherence((1,0), 2*np.pi*6.0666)
+    s.add_decoherence((2,1), 2*np.pi*10e-3)
+    s.add_transit_broadening(2*np.pi*100e-3)
+
+    detunings = np.linspace(-10,10,41)
+    probe = {'states':(0,1), 'rabi_frequency':2*np.pi*0.1, 'detuning':2*np.pi*detunings, 'label':'probe'}
+    couple = {'states':(1,2), 'rabi_frequency':2*np.pi*1, 'detuning':0, 'label':'couple'}
+
+    s.add_couplings(probe,couple)
+
+    # if slicing is broken, error will occur here
+    sols = rq.solve_steady_state(s,n_slices=4)
+    disp = sols.rho_ij(1,0).real
+
+    # do a couple simple checks to roughly confirm output is dispersive
+    zero_cross_ind = np.where(disp == 0)[0].squeeze()
+    zero_cross = detunings[zero_cross_ind]
+
+    assert zero_cross == pytest.approx(0.0), 'Resonance not resonant!'
+    assert disp.max() == pytest.approx(-disp.min()), 'Resonance not symmetric!'
+
+
+@pytest.mark.steady_state
+@pytest.mark.parametrize("rf_rabi", np.linspace(1.0, 20.0, 5))  # in MHz
+def test_DopFree_AT(find_zero_crossings, rf_rabi):
+    """Confirms that the expected Autler-Townes splitting is generated
+    in steady state without Doppler averaging or optical depth.
+    """
+
+    basis_size = 4
+    s = rq.Sensor(basis_size)
+    transit = 100e-3
+    gamma = 5.75
+    ryd_lifetime = 1e-3
+    gam = np.zeros((s.basis_size,s.basis_size),dtype=np.float64)
+    gam[1,0] = gamma
+    gam[2,1] = ryd_lifetime
+    gam[3,1] = ryd_lifetime
+    gam[:,0] += transit
+    s.set_gamma_matrix(2*np.pi*gam)
+
+    detunings = np.linspace(-15, 15, 301)
+    probe = {'states':(0,1), 'rabi_frequency':2*np.pi*0.1, 'detuning':0}
+    coupling = {'states':(1,2), 'rabi_frequency': 2*np.pi*0.6, 'detuning':2*np.pi*detunings}
+    rf = {'states':(2,3), 'rabi_frequency': 2*np.pi*rf_rabi, 'detuning':0}
+
+    s.add_couplings(probe,coupling,rf)
+    sols = rq.solve_steady_state(s).rho
+    rsols = get_rho_ij(sols, 1,0).real
+
+    # detect expected zero crossings in phase shift vs detuning
+    # this will give us the AT splitting
+    det_crossings = find_zero_crossings(rsols,detunings)
+
+    # ensure we got the right number of crossings
+    assert len(det_crossings) == 2
+
+    AT_splitting = det_crossings[-1] - det_crossings[0]
+
+    # tolerances set conservatively at 1% relative and 0.1 MHz absolute
+    assert AT_splitting == pytest.approx(rf_rabi, rel=1e-2, abs=1e-1), \
+        f'Expected AT={rf_rabi:.2f}, got {AT_splitting:.2f}'
+
+
+@pytest.mark.steady_state
+@pytest.mark.doppler
+@pytest.mark.parametrize("rf_rabi", np.linspace(8.0, 20.0, 5))  # in MHz
+def test_Dop_AT_couple(find_zero_crossings, rf_rabi):
+    """Confirms that the expected Autler-Townes splitting is generated
+    in steady state with Doppler averaging. For a coupling sweep, AT = rf_rabi
+    """
+
+    basis_size = 4
+    s = rq.Sensor(basis_size)
+    transit = 100e-3
+    gamma = 6.0666
+    ryd_lifetime = 1e-3
+    gam = np.zeros((s.basis_size,s.basis_size),dtype=np.float64)
+    gam[1,0] = gamma
+    gam[2,1] = ryd_lifetime
+    gam[3,1] = ryd_lifetime
+    gam[:,0] += transit
+    s.set_gamma_matrix(2*np.pi*gam)
+
+    # values correspond to Rb D2 scheme
+    kpmag = 2*np.pi/780.241e-3  # sets end units correctly to Mrad/s
+    kcmag = 2*np.pi/480e-3
+    kp = kpmag*np.array([1,0,0])
+    kc = kcmag*np.array([-1,0,0])
+    vP = 242.387  # Rb85
+    wPp = kp*vP
+    wPc = kc*vP
+
+    detunings = np.linspace(-15, 15, 301)
+    probe = {'states':(0,1), 'rabi_frequency':2*np.pi*1.5, 'detuning':0, 'kvec':wPp}
+    coupling = {'states':(1,2), 'rabi_frequency': 2*np.pi*4.0, 'detuning':2*np.pi*detunings,
+                'kvec':wPc}
+    rf = {'states':(2,3), 'rabi_frequency': 2*np.pi*rf_rabi, 'detuning':0}
+
+    s.add_couplings(probe,coupling,rf)
+    sols = rq.solve_steady_state(s,doppler=True).rho
+    rsols = get_rho_ij(sols, 1,0).real
+
+    # detect expected zero crossings in phase shift vs detuning
+    # this will give us the AT splitting
+    det_crossings = find_zero_crossings(rsols,detunings)
+
+    # ensure splitting is actually symmetric
+    assert det_crossings[-1] == pytest.approx(-det_crossings[0],rel=1e-2), \
+        'Assymetric AT splitting detected'
+
+    AT_splitting = det_crossings[-1] - det_crossings[0]
+
+    # tolerances set conservatively at 1% relative and 0.1 MHz absolute
+    assert AT_splitting == pytest.approx(rf_rabi, rel=1e-2, abs=1e-1), \
+        f'Expected AT={rf_rabi:.2f}, got {AT_splitting:.2f}'
+
+
+@pytest.mark.steady_state
+@pytest.mark.doppler
+@pytest.mark.parametrize("rf_rabi", np.linspace(8.0, 20.0, 5))  # in MHz
+def test_Dop_AT_probe(find_zero_crossings, rf_rabi):
+    """Confirms that the expected Autler-Townes splitting is generated
+    in steady state with Doppler averaging. For a coupling sweep, AT = kp/kc*rf_rabi
+    """
+
+    basis_size = 4
+    s = rq.Sensor(basis_size)
+    transit = 100e-3
+    gamma = 6.0666
+    ryd_lifetime = 1e-3
+    gam = np.zeros((s.basis_size,s.basis_size),dtype=np.float64)
+    gam[1,0] = gamma
+    gam[2,1] = ryd_lifetime
+    gam[3,1] = ryd_lifetime
+    gam[:,0] += transit
+    s.set_gamma_matrix(2*np.pi*gam)
+
+    # values correspond to Rb D2 scheme
+    kpmag = 2*np.pi/780.241e-3  # sets end units correctly to Mrad/s
+    kcmag = 2*np.pi/480e-3
+    kp = kpmag*np.array([1,0,0])
+    kc = kcmag*np.array([-1,0,0])
+    vP = 242.387
+    wPp = kp*vP
+    wPc = kc*vP
+
+    detunings = np.linspace(-15, 15, 301)
+    probe = {'states':(0,1), 'rabi_frequency':2*np.pi*1.5,'detuning':2*np.pi*detunings, 'kvec':wPp}
+    coupling = {'states':(1,2), 'rabi_frequency': 2*np.pi*4.0, 'detuning':0, 'kvec':wPc}
+    rf = {'states':(2,3), 'rabi_frequency': 2*np.pi*rf_rabi, 'detuning':0}
+
+    s.add_couplings(probe,coupling,rf)
+    sols = rq.solve_steady_state(s, doppler=True).rho
+    rsols = get_rho_ij(sols, 1,0).real
+
+    # detect expected zero crossings in phase shift vs detuning
+    # this will give us the AT splitting
+    det_crossings = find_zero_crossings(rsols,detunings)
+
+    # ensure splitting is actually symmetric
+    assert det_crossings[-1] == pytest.approx(-det_crossings[0],rel=1e-2), \
+        'Assymetric AT splitting detected'
+
+    AT_splitting = det_crossings[-1] - det_crossings[0]
+
+    # tolerances set conservatively at 1% relative and 0.25 MHz absolute
+    expAT = kpmag/kcmag*rf_rabi
+    assert AT_splitting == pytest.approx(expAT, rel=1e-2, abs=2.5e-1), \
+        f'Expected AT={expAT:.2f}, got {AT_splitting:.2f}'
+
+
+@pytest.mark.steady_state
+@pytest.mark.doppler
+def test_Dop_2level():
+    """Checks that simple doppler broadening of the probing transition
+    is correctly calculated by the doppler averaging.
+    """
+
+    from scipy.optimize import curve_fit
+    from scipy.constants import k,c
+    from arc import Rubidium85
+
+    # get actual atom parameters to compare against
+    atom = Rubidium85()
+    gState = [5,0,0.5]
+    iState = [5,1,1.5]
+    f0 = atom.getTransitionFrequency(*gState,*iState)
+    gamma = atom.getTransitionRate(*iState,*gState)/2/np.pi*1e-6
+    mRb85 = atom.mass
+    T = 300
+
+    # define out 2-level system
+    basis_size = 2
+    s = rq.Sensor(basis_size)
+    gam = np.zeros((s.basis_size,s.basis_size),dtype=np.float64)
+    gam[1,0] = gamma
+    s.set_gamma_matrix(2*np.pi*gam)
+
+    kpmag = 2*np.pi/780.241e-3  # sets end units correctly to Mrad/s
+    kp = kpmag*np.array([1,0,0])
+    vP = np.sqrt(2*k*T/mRb85)
+    wPp = kp*vP
+
+    # calculate the theoretical doppler width for this transition, in MHz
+    actualWidth = vP*np.sqrt(4*np.log(2)/c**2)*f0*1e-6
+
+    # calculate the doppler absorption profile
+    detunings = np.linspace(-750, 750, 301)
+    probe = {'states':(0,1), 'rabi_frequency':2*np.pi*1.5,'detuning':2*np.pi*detunings,'kvec':wPp}
+
+    s.add_couplings(probe)
+    sols = rq.solve_steady_state(s,doppler=True,
+                                 doppler_mesh_method={'method':'uniform','wDop':2.5}).rho
+
+    def gaussFit(f,A,w):
+        return A*np.exp(-f**2/(2*w**2))
+
+    rho10imag = get_rho_ij(sols, 1,0).imag
+    maxval_init = rho10imag.max()
+    p0 = [maxval_init,200]
+    popt,pcov = curve_fit(gaussFit,detunings,rho10imag,p0=p0)
+
+    measuredWidth = popt[1]*2*np.sqrt(2*np.log(2))
+
+    # confirm measured width is within 2% of theorectical
+    assert measuredWidth == pytest.approx(actualWidth,rel=2e-2), \
+        f'Doppler width of Rb85 D2 transition not correct'
+
+
+@pytest.mark.exception
+def test_solve_memory_fits():
+    '''Confirms that checks for EOMs fitting in memory fail when appropriate.'''
+
+    with pytest.raises(MemoryError, match='sum_doppler=False'):
+        # We do not support sum_doppler=False when full solve does not fit in memory
+        n = 4
+        stack = (101, 101)
+        doppler_stack = (561, 561)
+        rq.get_slice_num(n, stack, doppler_stack, sum_doppler=False, weight_doppler=True)
+
+    with pytest.raises(MemoryError, match='System is too large'):
+        # this system requires 335.4 GiB
+        n = 4
+        stack = (101, 101)
+        doppler_stack = (561, 561, 561)
+        rq.get_slice_num(n, stack, doppler_stack, sum_doppler=True, weight_doppler=True)
```

### Comparing `rydiqule-1.0.0/tests/test_steady_state_ham_gen.py` & `rydiqule-1.0.0rc2/tests/test_steady_state_ham_gen.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import numpy as np
-import pytest
-from rydiqule import Sensor
-from rydiqule import Cell
-from rydiqule import D2_states
-
-
-@pytest.mark.steady_state
-def test_ladder_5_level():
-
-    f1 = {'states':(0,1), 'rabi_frequency':0, 'detuning':1}
-    f2 = {'states':(1,2), 'rabi_frequency':0, 'detuning':2}
-    f3 = {'states':(2,3), 'rabi_frequency':0, 'detuning':4}
-    f4 = {'states':(3,4), 'rabi_frequency':0, 'detuning':8}
-
-    sensor = Sensor(5)
-    sensor.add_couplings(f1, f2, f3, f4)
-
-    expected_ham = np.diag([0, 1, 1+2, 1+2+4, 1+2+4+8])
-    ham = sensor.get_hamiltonian()
-
-    np.testing.assert_allclose(ham, expected_ham,
-                               err_msg="5 Level ladder failed hamilonian generation")
-
-
-@pytest.mark.steady_state
-def test_lambda_4_level():
-
-    f1 = {'states':(0,1), 'rabi_frequency':0, 'detuning':1}
-    f2 = {'states':(1,3), 'rabi_frequency':0, 'detuning':2}
-    f3 = {'states':(2,3), 'rabi_frequency':0, 'detuning':4}
-
-    sensor = Sensor(4)
-    sensor.add_couplings(f1, f2, f3)
-
-    expected_ham = np.diag([0, 1, 1+2-4, 1+2])
-    ham = sensor.get_hamiltonian()
-
-    np.testing.assert_allclose(ham, expected_ham,
-                               err_msg="4 Level lambda failed hamilonian generation")
-
-
-@pytest.mark.steady_state
-def test_v_5_level():
-
-    f1 = {'states':(0,1), 'rabi_frequency':0, 'detuning':1}
-    f2 = {'states':(1,2), 'rabi_frequency':0, 'detuning':2}
-    f3 = {'states':(2,3), 'rabi_frequency':0, 'detuning':4}
-    f4 = {'states':(2,4), 'rabi_frequency':0, 'detuning':8}
-
-    sensor = Sensor(5)
-    sensor.add_couplings(f1, f2, f3, f4)
-
-    expected_ham = np.diag([0, 1, 1+2, 1+2+4, 1+2+8])
-    ham = sensor.get_hamiltonian()
-
-    np.testing.assert_allclose(ham, expected_ham,
-                               err_msg="5 Level V failed hamilonian generation")
-
-
-@pytest.mark.steady_state
-def test_v_5_cell():
-
-    f1 = {'states':(0,1), 'rabi_frequency':0, 'detuning':1}
-    f2 = {'states':(1,2), 'rabi_frequency':0, 'detuning':2}
-    f3 = {'states':(2,3), 'rabi_frequency':0, 'detuning':4}
-    f4 = {'states':(2,4), 'rabi_frequency':0, 'detuning':8}
-
-    state1 = [10, 2, 2.5, 0.5]
-    state2 = [11, 3, 3.5, 0.5]
-    state3 = [9, 3, 3.5, 0.5]
-
-    RbSensor_ss = Cell('Rb85', *D2_states(5), state1, state2, state3)
-
-    RbSensor_ss.add_couplings(f1, f2, f3, f4)
-
-    expected_ham = np.diag([0, 1, 1+2, 1+2+4, 1+2+8])
-    ham = RbSensor_ss.get_hamiltonian()
-
-    np.testing.assert_allclose(ham, expected_ham,
-                               err_msg="5 Level V failed hamilonian generation")
+import numpy as np
+import pytest
+from rydiqule import Sensor
+from rydiqule import Cell
+from rydiqule import D2_states
+
+
+@pytest.mark.steady_state
+def test_ladder_5_level():
+
+    f1 = {'states':(0,1), 'rabi_frequency':0, 'detuning':1}
+    f2 = {'states':(1,2), 'rabi_frequency':0, 'detuning':2}
+    f3 = {'states':(2,3), 'rabi_frequency':0, 'detuning':4}
+    f4 = {'states':(3,4), 'rabi_frequency':0, 'detuning':8}
+
+    sensor = Sensor(5)
+    sensor.add_couplings(f1, f2, f3, f4)
+
+    expected_ham = np.diag([0, 1, 1+2, 1+2+4, 1+2+4+8])
+    ham = sensor.get_hamiltonian()
+
+    np.testing.assert_allclose(ham, expected_ham,
+                               err_msg="5 Level ladder failed hamilonian generation")
+
+
+@pytest.mark.steady_state
+def test_lambda_4_level():
+
+    f1 = {'states':(0,1), 'rabi_frequency':0, 'detuning':1}
+    f2 = {'states':(1,3), 'rabi_frequency':0, 'detuning':2}
+    f3 = {'states':(2,3), 'rabi_frequency':0, 'detuning':4}
+
+    sensor = Sensor(4)
+    sensor.add_couplings(f1, f2, f3)
+
+    expected_ham = np.diag([0, 1, 1+2-4, 1+2])
+    ham = sensor.get_hamiltonian()
+
+    np.testing.assert_allclose(ham, expected_ham,
+                               err_msg="4 Level lambda failed hamilonian generation")
+
+
+@pytest.mark.steady_state
+def test_v_5_level():
+
+    f1 = {'states':(0,1), 'rabi_frequency':0, 'detuning':1}
+    f2 = {'states':(1,2), 'rabi_frequency':0, 'detuning':2}
+    f3 = {'states':(2,3), 'rabi_frequency':0, 'detuning':4}
+    f4 = {'states':(2,4), 'rabi_frequency':0, 'detuning':8}
+
+    sensor = Sensor(5)
+    sensor.add_couplings(f1, f2, f3, f4)
+
+    expected_ham = np.diag([0, 1, 1+2, 1+2+4, 1+2+8])
+    ham = sensor.get_hamiltonian()
+
+    np.testing.assert_allclose(ham, expected_ham,
+                               err_msg="5 Level V failed hamilonian generation")
+
+
+@pytest.mark.steady_state
+def test_v_5_cell():
+
+    f1 = {'states':(0,1), 'rabi_frequency':0, 'detuning':1}
+    f2 = {'states':(1,2), 'rabi_frequency':0, 'detuning':2}
+    f3 = {'states':(2,3), 'rabi_frequency':0, 'detuning':4}
+    f4 = {'states':(2,4), 'rabi_frequency':0, 'detuning':8}
+
+    state1 = [10, 2, 2.5, 0.5]
+    state2 = [11, 3, 3.5, 0.5]
+    state3 = [9, 3, 3.5, 0.5]
+
+    RbSensor_ss = Cell('Rb85', *D2_states(5), state1, state2, state3)
+
+    RbSensor_ss.add_couplings(f1, f2, f3, f4)
+
+    expected_ham = np.diag([0, 1, 1+2, 1+2+4, 1+2+8])
+    ham = RbSensor_ss.get_hamiltonian()
+
+    np.testing.assert_allclose(ham, expected_ham,
+                               err_msg="5 Level V failed hamilonian generation")
```

### Comparing `rydiqule-1.0.0/tests/test_time.py` & `rydiqule-1.0.0rc2/tests/test_time.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,255 +1,255 @@
-import numpy as np
-import pytest
-
-import rydiqule as rq
-
-
-@pytest.mark.time
-@pytest.mark.slow
-@pytest.mark.doppler
-def test_rabi_flop_doppler():
-    """Tests that time solver functions with Doppler broadening
-    """
-    def const(t):
-        return 1
-    kp = 0.001*np.array([1,0,0])
-
-    red_rabi_freq = 4.4444
-    red_laser = {'states':(0,1), 'rabi_frequency':red_rabi_freq,
-                 'detuning':0, 'kvec':kp, 'time_dependence': const}
-
-    sensor = rq.Sensor(3)
-
-    sensor.add_couplings(red_laser)
-    gamma = np.zeros((3,3))
-    gamma[0,1] = 0.1
-    sensor.set_gamma_matrix(gamma)
-
-    # RF field does not matter, just including one to test functionality
-    solSize = sensor.basis_size * sensor.basis_size-1
-    initCond = np.zeros(solSize)
-
-    dop_meth = {"method":"split", "n_doppler":20, "n_coherent":40}
-
-    sampleNum = 4000
-    endTime = 20.0
-    solution = rq.solve_time(sensor, endTime, sampleNum,
-                             init_cond=initCond, doppler_mesh_method=dop_meth,
-                             doppler=True)
-    fft1 = np.fft.fft(solution.rho[:,3])  # Checking if the main frequency is the Rabi frequency
-    fft1 = fft1[1:round(len(solution.t)/2)]
-    fft1 = np.abs(fft1)
-
-    freq = np.linspace(np.pi/endTime, np.pi*sampleNum/endTime, len(fft1))
-    freq_loc = np.argmax(fft1)
-
-    val = freq[freq_loc]  # The strongest frequency value
-
-    np.testing.assert_allclose(red_rabi_freq, val, rtol=0.05,
-                               err_msg='Two level time solution not working with Doppler')
-
-
-@pytest.mark.time
-def test_rabi_flop():
-    """Tests that time solver functions without Doppler broadening
-    """
-
-    def const(t):
-        return 1
-
-    blue_laser = {'states':(1,2), 'rabi_frequency':0.0, 'detuning':0, 'time_dependence': const}
-    red_rabi_freq = 2*np.pi*4.4444
-    red_laser = {'states':(0,1), 'rabi_frequency':red_rabi_freq, 'detuning':0}
-
-    RbSensor = rq.Sensor(3)
-    RbSensor.add_couplings(red_laser,blue_laser)
-    gamma_matrix = np.zeros((3,3),dtype='double')
-    gamma_matrix[0,1] = 0.1
-    gamma_matrix[0,2] = 0.1
-    gamma_matrix[1,2] = 0.1
-    RbSensor.set_gamma_matrix(gamma_matrix)
-
-    # RF field does not matter, just including one to test functionality
-    solSize = RbSensor.basis_size * RbSensor.basis_size-1
-    initCond = np.zeros(solSize)
-
-    sampleNum = 1000
-    endTime = 10.0
-    solution = rq.solve_time(RbSensor, endTime, sampleNum, init_cond=initCond,rtol=1e-6)
-    fft1 = np.fft.fft(solution.rho[:,3])  # Checking if the main frequency is the Rabi frequency
-    fft1 = fft1[:round(len(solution.t)/2)]
-    fft1 = np.abs(fft1)
-
-    freq_loc = np.argmax(fft1[1:])
-
-    freq = np.linspace(np.pi/endTime, np.pi*sampleNum/endTime, len(fft1))
-    val = freq[freq_loc]  # The strongest frequency value
-
-    np.testing.assert_allclose(red_rabi_freq, val, rtol=0.05,
-                               err_msg='Two level time solution not working without Doppler')
-
-
-@pytest.mark.time
-@pytest.mark.slow
-def test_time_match_steady():
-    """Uses a single tone RF field to check if the time solver starting at zero reached steady state
-    """
-    red_laser = {'states':(0,1), 'rabi_frequency':2*np.pi*4.0, 'detuning':2.0}
-    blue_laser = {'states':(1,2), 'rabi_frequency':2*np.pi*6.0, 'detuning':-1.0}
-    rf_coupling_ss = {'states': (2,3), 'rabi_frequency':2*np.pi*5.0, 'detuning': 0}
-
-    rydberg_target_state = [150, 2, 2.5, 0.5]
-    rydberg_excited_state = [149, 3, 3.5, 0.5]
-
-    RbSensor_ss = rq.Cell("Rb85", *rq.D2_states(5),
-                          rydberg_target_state, rydberg_excited_state,
-                          gamma_transit=0.1)
-    RbSensor_t = rq.Cell("Rb85", *rq.D2_states(5),
-                         rydberg_target_state, rydberg_excited_state,
-                         gamma_transit=0.1)
-
-    RbSensor_ss.add_couplings(red_laser, blue_laser, rf_coupling_ss)
-
-    solSize = RbSensor_ss.basis_size * RbSensor_ss.basis_size-1
-    initCond = np.zeros(solSize)
-
-    [n,l,j,m] = RbSensor_ss.states_list()[2]
-    [n2, l2, j2, m2] = RbSensor_ss.states_list()[3]
-
-    rf_freq = RbSensor_ss.atom.getTransitionFrequency(n2,l2,j2,n,l,j)*1E-6
-
-    def rf_carrier(t):
-        return np.cos(2*np.pi*rf_freq*t)
-
-    rf_coupling_t = {'states': (2,3), 'rabi_frequency':2*np.pi*5.0, 'time_dependence': rf_carrier}
-    RbSensor_t.add_couplings(red_laser, blue_laser, rf_coupling_t)
-
-    sampleNum = 10000
-    endTime = 5
-
-    # currently passes with end time 25 and Rtol = atol = 1e-4
-    time_sol = rq.solve_time(RbSensor_t, endTime, sampleNum, initCond, rtol=1e-6, atol=1e-6)
-    steady_sol = rq.solve_steady_state(RbSensor_ss)
-
-    # certain off-diagonal elements will not match.
-    # For now, test 1 diagonal and one off-diagonal element.
-    np.testing.assert_allclose(steady_sol.rho[:2], time_sol.rho[-1][:2], rtol=0.1,
-                               err_msg='Time solution does not converge to steady state')
-
-
-@pytest.mark.time
-def test_time_complex_match_steady():
-    """Tests the time solver vs steady state
-    with aribtrary (complex) and time-dependent rabi frequencies
-    """
-
-    def fun(t):
-        if t < 1:
-            return 0
-        else:
-            return 1
-
-    def fun2(t):
-        if t < 1:
-            return 0
-        else:
-            return 1j
-
-    end_time = 100
-    sample_num = 20
-
-    probe_t = {'states':(0,1), 'rabi_frequency':4+9j,'detuning':0.3, 'time_dependence': fun}
-    probe_s = {'states':(0,1), 'rabi_frequency':4+9j,'detuning':0.3}
-    dress = {'states':(1,2), 'rabi_frequency':3+2j,'detuning': .7}
-    couple_t = {'states':(2,3), 'rabi_frequency':-9j+1, 'detuning':0.3, 'time_dependence': fun2}
-    couple_s = {'states':(2,3), 'rabi_frequency':9+1j, 'detuning':0.3}
-
-    gam = np.zeros((4,4),dtype=np.float64)
-    gam[1,0] = 0.5
-    gam[2,1] = 0.4
-    gam[3,2] = 0.6
-    gamma_matrix = gam
-
-    sensor_t = rq.Sensor(4)
-    sensor_s = rq.Sensor(4)
-
-    sensor_t.add_couplings(probe_t, dress, couple_t)
-    sensor_t.set_gamma_matrix(gamma_matrix)
-    sensor_s.add_couplings(probe_s, dress, couple_s)
-    sensor_s.set_gamma_matrix(gamma_matrix)
-
-    sols_s = rq.solve_steady_state(sensor_s)
-    sol_t = rq.solve_time(sensor_t, end_time, sample_num, rtol=1E-6, atol=1e-6)
-    # sol_t_numba = rq.solve_time(sensor_t, end_time, sample_num, rtol=1E-6, atol=1e-6,
-    #                             use_nkode = True, complex_numba = True)
-    np.testing.assert_allclose(sols_s.rho,sol_t.rho[-1,:],atol=0.005,
-            err_msg='Complex time and steady state solutions do not match.  non-compiled.')  # noqa
-    # np.testing.assert_allclose(sols_s.rho,sol_t_numba.rho[-1,:],atol=0.005,
-    #       err_msg='Complex time and steady state solutions do not match.  numbakit.')
-
-
-@pytest.mark.time
-@pytest.mark.slow
-def test_time_rwa():
-
-    n = 159
-    RydbergTargetState = [n+1, 2, 2.5, 0.5]  # states labeled n, l, j, m_j
-    RydbergExcitedState = [n, 3, 3.5, 0.5]
-
-    RbSensor_rwa = rq.Cell("Rb85", *rq.D2_states(5),
-                           RydbergTargetState, RydbergExcitedState,
-                           gamma_transit=2*np.pi*1)
-    RbSensor_norwa = rq.Cell("Rb85", *rq.D2_states(5),
-                             RydbergTargetState, RydbergExcitedState,
-                             gamma_transit=2*np.pi*1)
-
-    rf_freq = RbSensor_norwa.atom.getTransitionFrequency(n+1, 2, 2.5, n, 3, 3.5)*1E-6
-    field = 0.0006  # V/m
-
-    def rf_fun(omega_0, omega_mod,factor):
-        def fun(t):
-            return factor*field*np.cos(omega_0*t)*np.sin(omega_mod*t)
-        return fun
-
-    rf_norwa = rf_fun(2*np.pi*rf_freq, 2*np.pi*5,2)
-    rf_rwa = rf_fun(0, 2*np.pi*5,1)
-
-    red_laser = {'states':(0,1), 'rabi_frequency':2*np.pi*0.6, 'detuning':0}
-    blue_laser = {'states':(1,2), 'rabi_frequency':2*np.pi*1.0, 'detuning':0}
-    RFrwa = {'states': (2,3), 'rabi_frequency':2*np.pi*0.6, "detuning":0, 'time_dependence': rf_rwa}
-    RFno = {'states': (2,3), 'rabi_frequency':2*np.pi*0.6, 'time_dependence': rf_norwa}
-
-    RbSensor_rwa.add_couplings(red_laser, blue_laser,RFrwa)
-    RbSensor_norwa.add_couplings(red_laser, blue_laser,RFno)
-
-    endTime = 5
-    sampleNum = 1000000
-
-    time_sol_rwa = rq.solve_time(RbSensor_rwa, endTime, sampleNum, rtol=1E-6)
-    time_sol_norwa = rq.solve_time(RbSensor_norwa, endTime, sampleNum, rtol=1E-6)
-
-    transNO = np.imag(rq.get_susceptibility(time_sol_norwa, RbSensor_norwa))
-    transRWA = np.imag(rq.get_susceptibility(time_sol_rwa, RbSensor_rwa))
-    np.testing.assert_allclose(transNO,transRWA,rtol=0.01,
-            err_msg='Non-RWA and RWA give different results when they should match')  # noqa
-    
-    
-@pytest.mark.time
-def test_time_scan_rabi():
-    step = lambda t: 0 if t<1 else 1
-    rabi = np.linspace(-5,5,11)
-    f1 = {"states":(0,1), "detuning":1, "rabi_frequency":1}
-    f2_s = {"states": (1,2), "detuning":2, "rabi_frequency":rabi}
-    f2_t = {"states": (1,2), "detuning":2, "rabi_frequency":rabi, "time_dependence":step}
-    
-    s_steady = rq.Sensor(3)
-    s_time = rq.Sensor(3)
-    s_steady.add_couplings(f1, f2_s)
-    s_time.add_couplings(f1, f2_t)
-    s_steady.add_transit_broadening(0.5)
-    s_time.add_transit_broadening(0.5)
-    
-    sol_steady = rq.solve_steady_state(s_steady).rho
-    sol_time = rq.solve_time(s_time, 500, 10, rtol=1e-3).rho
-    
-    np.testing.assert_allclose(sol_steady, sol_time[...,-1,:], atol=0.005)
+import numpy as np
+import pytest
+
+import rydiqule as rq
+
+
+@pytest.mark.time
+@pytest.mark.slow
+@pytest.mark.doppler
+def test_rabi_flop_doppler():
+    """Tests that time solver functions with Doppler broadening
+    """
+    def const(t):
+        return 1
+    kp = 0.001*np.array([1,0,0])
+
+    red_rabi_freq = 4.4444
+    red_laser = {'states':(0,1), 'rabi_frequency':red_rabi_freq,
+                 'detuning':0, 'kvec':kp, 'time_dependence': const}
+
+    sensor = rq.Sensor(3)
+
+    sensor.add_couplings(red_laser)
+    gamma = np.zeros((3,3))
+    gamma[0,1] = 0.1
+    sensor.set_gamma_matrix(gamma)
+
+    # RF field does not matter, just including one to test functionality
+    solSize = sensor.basis_size * sensor.basis_size-1
+    initCond = np.zeros(solSize)
+
+    dop_meth = {"method":"split", "n_doppler":20, "n_coherent":40}
+
+    sampleNum = 4000
+    endTime = 20.0
+    solution = rq.solve_time(sensor, endTime, sampleNum,
+                             init_cond=initCond, doppler_mesh_method=dop_meth,
+                             doppler=True)
+    fft1 = np.fft.fft(solution.rho[:,3])  # Checking if the main frequency is the Rabi frequency
+    fft1 = fft1[1:round(len(solution.t)/2)]
+    fft1 = np.abs(fft1)
+
+    freq = np.linspace(np.pi/endTime, np.pi*sampleNum/endTime, len(fft1))
+    freq_loc = np.argmax(fft1)
+
+    val = freq[freq_loc]  # The strongest frequency value
+
+    np.testing.assert_allclose(red_rabi_freq, val, rtol=0.05,
+                               err_msg='Two level time solution not working with Doppler')
+
+
+@pytest.mark.time
+def test_rabi_flop():
+    """Tests that time solver functions without Doppler broadening
+    """
+
+    def const(t):
+        return 1
+
+    blue_laser = {'states':(1,2), 'rabi_frequency':0.0, 'detuning':0, 'time_dependence': const}
+    red_rabi_freq = 2*np.pi*4.4444
+    red_laser = {'states':(0,1), 'rabi_frequency':red_rabi_freq, 'detuning':0}
+
+    RbSensor = rq.Sensor(3)
+    RbSensor.add_couplings(red_laser,blue_laser)
+    gamma_matrix = np.zeros((3,3),dtype='double')
+    gamma_matrix[0,1] = 0.1
+    gamma_matrix[0,2] = 0.1
+    gamma_matrix[1,2] = 0.1
+    RbSensor.set_gamma_matrix(gamma_matrix)
+
+    # RF field does not matter, just including one to test functionality
+    solSize = RbSensor.basis_size * RbSensor.basis_size-1
+    initCond = np.zeros(solSize)
+
+    sampleNum = 1000
+    endTime = 10.0
+    solution = rq.solve_time(RbSensor, endTime, sampleNum, init_cond=initCond,rtol=1e-6)
+    fft1 = np.fft.fft(solution.rho[:,3])  # Checking if the main frequency is the Rabi frequency
+    fft1 = fft1[:round(len(solution.t)/2)]
+    fft1 = np.abs(fft1)
+
+    freq_loc = np.argmax(fft1[1:])
+
+    freq = np.linspace(np.pi/endTime, np.pi*sampleNum/endTime, len(fft1))
+    val = freq[freq_loc]  # The strongest frequency value
+
+    np.testing.assert_allclose(red_rabi_freq, val, rtol=0.05,
+                               err_msg='Two level time solution not working without Doppler')
+
+
+@pytest.mark.time
+@pytest.mark.slow
+def test_time_match_steady():
+    """Uses a single tone RF field to check if the time solver starting at zero reached steady state
+    """
+    red_laser = {'states':(0,1), 'rabi_frequency':2*np.pi*4.0, 'detuning':2.0}
+    blue_laser = {'states':(1,2), 'rabi_frequency':2*np.pi*6.0, 'detuning':-1.0}
+    rf_coupling_ss = {'states': (2,3), 'rabi_frequency':2*np.pi*5.0, 'detuning': 0}
+
+    rydberg_target_state = [150, 2, 2.5, 0.5]
+    rydberg_excited_state = [149, 3, 3.5, 0.5]
+
+    RbSensor_ss = rq.Cell("Rb85", *rq.D2_states(5),
+                          rydberg_target_state, rydberg_excited_state,
+                          gamma_transit=0.1)
+    RbSensor_t = rq.Cell("Rb85", *rq.D2_states(5),
+                         rydberg_target_state, rydberg_excited_state,
+                         gamma_transit=0.1)
+
+    RbSensor_ss.add_couplings(red_laser, blue_laser, rf_coupling_ss)
+
+    solSize = RbSensor_ss.basis_size * RbSensor_ss.basis_size-1
+    initCond = np.zeros(solSize)
+
+    [n,l,j,m] = RbSensor_ss.states_list()[2]
+    [n2, l2, j2, m2] = RbSensor_ss.states_list()[3]
+
+    rf_freq = RbSensor_ss.atom.getTransitionFrequency(n2,l2,j2,n,l,j)*1E-6
+
+    def rf_carrier(t):
+        return np.cos(2*np.pi*rf_freq*t)
+
+    rf_coupling_t = {'states': (2,3), 'rabi_frequency':2*np.pi*5.0, 'time_dependence': rf_carrier}
+    RbSensor_t.add_couplings(red_laser, blue_laser, rf_coupling_t)
+
+    sampleNum = 10000
+    endTime = 5
+
+    # currently passes with end time 25 and Rtol = atol = 1e-4
+    time_sol = rq.solve_time(RbSensor_t, endTime, sampleNum, initCond, rtol=1e-6, atol=1e-6)
+    steady_sol = rq.solve_steady_state(RbSensor_ss)
+
+    # certain off-diagonal elements will not match.
+    # For now, test 1 diagonal and one off-diagonal element.
+    np.testing.assert_allclose(steady_sol.rho[:2], time_sol.rho[-1][:2], rtol=0.1,
+                               err_msg='Time solution does not converge to steady state')
+
+
+@pytest.mark.time
+def test_time_complex_match_steady():
+    """Tests the time solver vs steady state
+    with aribtrary (complex) and time-dependent rabi frequencies
+    """
+
+    def fun(t):
+        if t < 1:
+            return 0
+        else:
+            return 1
+
+    def fun2(t):
+        if t < 1:
+            return 0
+        else:
+            return 1j
+
+    end_time = 100
+    sample_num = 20
+
+    probe_t = {'states':(0,1), 'rabi_frequency':4+9j,'detuning':0.3, 'time_dependence': fun}
+    probe_s = {'states':(0,1), 'rabi_frequency':4+9j,'detuning':0.3}
+    dress = {'states':(1,2), 'rabi_frequency':3+2j,'detuning': .7}
+    couple_t = {'states':(2,3), 'rabi_frequency':-9j+1, 'detuning':0.3, 'time_dependence': fun2}
+    couple_s = {'states':(2,3), 'rabi_frequency':9+1j, 'detuning':0.3}
+
+    gam = np.zeros((4,4),dtype=np.float64)
+    gam[1,0] = 0.5
+    gam[2,1] = 0.4
+    gam[3,2] = 0.6
+    gamma_matrix = gam
+
+    sensor_t = rq.Sensor(4)
+    sensor_s = rq.Sensor(4)
+
+    sensor_t.add_couplings(probe_t, dress, couple_t)
+    sensor_t.set_gamma_matrix(gamma_matrix)
+    sensor_s.add_couplings(probe_s, dress, couple_s)
+    sensor_s.set_gamma_matrix(gamma_matrix)
+
+    sols_s = rq.solve_steady_state(sensor_s)
+    sol_t = rq.solve_time(sensor_t, end_time, sample_num, rtol=1E-6, atol=1e-6)
+    # sol_t_numba = rq.solve_time(sensor_t, end_time, sample_num, rtol=1E-6, atol=1e-6,
+    #                             use_nkode = True, complex_numba = True)
+    np.testing.assert_allclose(sols_s.rho,sol_t.rho[-1,:],atol=0.005,
+            err_msg='Complex time and steady state solutions do not match.  non-compiled.')  # noqa
+    # np.testing.assert_allclose(sols_s.rho,sol_t_numba.rho[-1,:],atol=0.005,
+    #       err_msg='Complex time and steady state solutions do not match.  numbakit.')
+
+
+@pytest.mark.time
+@pytest.mark.slow
+def test_time_rwa():
+
+    n = 159
+    RydbergTargetState = [n+1, 2, 2.5, 0.5]  # states labeled n, l, j, m_j
+    RydbergExcitedState = [n, 3, 3.5, 0.5]
+
+    RbSensor_rwa = rq.Cell("Rb85", *rq.D2_states(5),
+                           RydbergTargetState, RydbergExcitedState,
+                           gamma_transit=2*np.pi*1)
+    RbSensor_norwa = rq.Cell("Rb85", *rq.D2_states(5),
+                             RydbergTargetState, RydbergExcitedState,
+                             gamma_transit=2*np.pi*1)
+
+    rf_freq = RbSensor_norwa.atom.getTransitionFrequency(n+1, 2, 2.5, n, 3, 3.5)*1E-6
+    field = 0.0006  # V/m
+
+    def rf_fun(omega_0, omega_mod,factor):
+        def fun(t):
+            return factor*field*np.cos(omega_0*t)*np.sin(omega_mod*t)
+        return fun
+
+    rf_norwa = rf_fun(2*np.pi*rf_freq, 2*np.pi*5,2)
+    rf_rwa = rf_fun(0, 2*np.pi*5,1)
+
+    red_laser = {'states':(0,1), 'rabi_frequency':2*np.pi*0.6, 'detuning':0}
+    blue_laser = {'states':(1,2), 'rabi_frequency':2*np.pi*1.0, 'detuning':0}
+    RFrwa = {'states': (2,3), 'rabi_frequency':2*np.pi*0.6, "detuning":0, 'time_dependence': rf_rwa}
+    RFno = {'states': (2,3), 'rabi_frequency':2*np.pi*0.6, 'time_dependence': rf_norwa}
+
+    RbSensor_rwa.add_couplings(red_laser, blue_laser,RFrwa)
+    RbSensor_norwa.add_couplings(red_laser, blue_laser,RFno)
+
+    endTime = 5
+    sampleNum = 1000000
+
+    time_sol_rwa = rq.solve_time(RbSensor_rwa, endTime, sampleNum, rtol=1E-6)
+    time_sol_norwa = rq.solve_time(RbSensor_norwa, endTime, sampleNum, rtol=1E-6)
+
+    transNO = np.imag(rq.get_susceptibility(time_sol_norwa, RbSensor_norwa))
+    transRWA = np.imag(rq.get_susceptibility(time_sol_rwa, RbSensor_rwa))
+    np.testing.assert_allclose(transNO,transRWA,rtol=0.01,
+            err_msg='Non-RWA and RWA give different results when they should match')  # noqa
+    
+    
+@pytest.mark.time
+def test_time_scan_rabi():
+    step = lambda t: 0 if t<1 else 1
+    rabi = np.linspace(-5,5,11)
+    f1 = {"states":(0,1), "detuning":1, "rabi_frequency":1}
+    f2_s = {"states": (1,2), "detuning":2, "rabi_frequency":rabi}
+    f2_t = {"states": (1,2), "detuning":2, "rabi_frequency":rabi, "time_dependence":step}
+    
+    s_steady = rq.Sensor(3)
+    s_time = rq.Sensor(3)
+    s_steady.add_couplings(f1, f2_s)
+    s_time.add_couplings(f1, f2_t)
+    s_steady.add_transit_broadening(0.5)
+    s_time.add_transit_broadening(0.5)
+    
+    sol_steady = rq.solve_steady_state(s_steady).rho
+    sol_time = rq.solve_time(s_time, 500, 10, rtol=1e-3).rho
+    
+    np.testing.assert_allclose(sol_steady, sol_time[...,-1,:], atol=0.005)
```

### Comparing `rydiqule-1.0.0/tests/test_time_cyrk.py` & `rydiqule-1.0.0rc2/tests/test_time_cyrk.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,83 @@
-import numpy as np
-import pytest
-
-import rydiqule as rq
-
-@pytest.mark.time
-def test_rabi_flop_cyrk():
-    """Tests that the cyrk.cyrk_ode backend runs"""
-
-    def const(t):
-        return 1
-    
-    blue_laser = {'states':(1,2), 'rabi_frequency':0.0, 'detuning':0, 'time_dependence': const}
-    red_rabi_freq = 2*np.pi*4.4444
-    red_laser = {'states':(0,1), 'rabi_frequency':red_rabi_freq, 'detuning':0}
-
-    RbSensor = rq.Sensor(3)
-    RbSensor.add_couplings(red_laser,blue_laser)
-    gamma_matrix = np.zeros((3,3),dtype='double')
-    gamma_matrix[0,1] = 0.1
-    gamma_matrix[0,2] = 0.1
-    gamma_matrix[1,2] = 0.1
-    RbSensor.set_gamma_matrix(gamma_matrix)
-
-    # RF field does not matter, just including one to test functionality
-    solSize = RbSensor.basis_size * RbSensor.basis_size-1
-    initCond = np.zeros(solSize)
-
-    sampleNum = 1000
-    endTime = 10.0
-    solution = rq.solve_time(RbSensor, endTime, sampleNum, init_cond=initCond,rtol=1e-6,
-                             solver='cyrk')
-    fft1 = np.fft.fft(solution.rho[:,3])  # Checking if the main frequency is the Rabi frequency
-    fft1 = fft1[:round(len(solution.t)/2)]
-    fft1 = np.abs(fft1)
-
-    freq_loc = np.argmax(fft1[1:])
-
-    freq = np.linspace(np.pi/endTime, np.pi*sampleNum/endTime, len(fft1))
-    val = freq[freq_loc]  # The strongest frequency value
-
-    np.testing.assert_allclose(red_rabi_freq, val, rtol=0.05,
-                               err_msg='cyrk_doe two level time solution not working')
-
-
-@pytest.mark.time
-@pytest.mark.slow
-def test_rabi_flop_nbrk():
-    """Tests that the cyrk.nbrk_ode backend runs"""
-
-    def const(t):
-        return 1
-    
-    blue_laser = {'states':(1,2), 'rabi_frequency':0.0, 'detuning':0, 'time_dependence': const}
-    red_rabi_freq = 2*np.pi*4.4444
-    red_laser = {'states':(0,1), 'rabi_frequency':red_rabi_freq, 'detuning':0}
-
-    RbSensor = rq.Sensor(3)
-    RbSensor.add_couplings(red_laser,blue_laser)
-    gamma_matrix = np.zeros((3,3),dtype='double')
-    gamma_matrix[0,1] = 0.1
-    gamma_matrix[0,2] = 0.1
-    gamma_matrix[1,2] = 0.1
-    RbSensor.set_gamma_matrix(gamma_matrix)
-
-    # RF field does not matter, just including one to test functionality
-    solSize = RbSensor.basis_size * RbSensor.basis_size-1
-    initCond = np.zeros(solSize)
-
-    sampleNum = 1000
-    endTime = 10.0
-    solution = rq.solve_time(RbSensor, endTime, sampleNum, init_cond=initCond,rtol=1e-6,
-                             solver='nbrk')
-    fft1 = np.fft.fft(solution.rho[:,3])  # Checking if the main frequency is the Rabi frequency
-    fft1 = fft1[:round(len(solution.t)/2)]
-    fft1 = np.abs(fft1)
-
-    freq_loc = np.argmax(fft1[1:])
-
-    freq = np.linspace(np.pi/endTime, np.pi*sampleNum/endTime, len(fft1))
-    val = freq[freq_loc]  # The strongest frequency value
-
-    np.testing.assert_allclose(red_rabi_freq, val, rtol=0.05,
+import numpy as np
+import pytest
+
+import rydiqule as rq
+
+@pytest.mark.time
+def test_rabi_flop_cyrk():
+    """Tests that the cyrk.cyrk_ode backend runs"""
+
+    def const(t):
+        return 1
+    
+    blue_laser = {'states':(1,2), 'rabi_frequency':0.0, 'detuning':0, 'time_dependence': const}
+    red_rabi_freq = 2*np.pi*4.4444
+    red_laser = {'states':(0,1), 'rabi_frequency':red_rabi_freq, 'detuning':0}
+
+    RbSensor = rq.Sensor(3)
+    RbSensor.add_couplings(red_laser,blue_laser)
+    gamma_matrix = np.zeros((3,3),dtype='double')
+    gamma_matrix[0,1] = 0.1
+    gamma_matrix[0,2] = 0.1
+    gamma_matrix[1,2] = 0.1
+    RbSensor.set_gamma_matrix(gamma_matrix)
+
+    # RF field does not matter, just including one to test functionality
+    solSize = RbSensor.basis_size * RbSensor.basis_size-1
+    initCond = np.zeros(solSize)
+
+    sampleNum = 1000
+    endTime = 10.0
+    solution = rq.solve_time(RbSensor, endTime, sampleNum, init_cond=initCond,rtol=1e-6,
+                             solver='cyrk')
+    fft1 = np.fft.fft(solution.rho[:,3])  # Checking if the main frequency is the Rabi frequency
+    fft1 = fft1[:round(len(solution.t)/2)]
+    fft1 = np.abs(fft1)
+
+    freq_loc = np.argmax(fft1[1:])
+
+    freq = np.linspace(np.pi/endTime, np.pi*sampleNum/endTime, len(fft1))
+    val = freq[freq_loc]  # The strongest frequency value
+
+    np.testing.assert_allclose(red_rabi_freq, val, rtol=0.05,
+                               err_msg='cyrk_doe two level time solution not working')
+
+
+@pytest.mark.time
+def test_rabi_flop_nbrk():
+    """Tests that the cyrk.nbrk_ode backend runs"""
+
+    def const(t):
+        return 1
+    
+    blue_laser = {'states':(1,2), 'rabi_frequency':0.0, 'detuning':0, 'time_dependence': const}
+    red_rabi_freq = 2*np.pi*4.4444
+    red_laser = {'states':(0,1), 'rabi_frequency':red_rabi_freq, 'detuning':0}
+
+    RbSensor = rq.Sensor(3)
+    RbSensor.add_couplings(red_laser,blue_laser)
+    gamma_matrix = np.zeros((3,3),dtype='double')
+    gamma_matrix[0,1] = 0.1
+    gamma_matrix[0,2] = 0.1
+    gamma_matrix[1,2] = 0.1
+    RbSensor.set_gamma_matrix(gamma_matrix)
+
+    # RF field does not matter, just including one to test functionality
+    solSize = RbSensor.basis_size * RbSensor.basis_size-1
+    initCond = np.zeros(solSize)
+
+    sampleNum = 1000
+    endTime = 10.0
+    solution = rq.solve_time(RbSensor, endTime, sampleNum, init_cond=initCond,rtol=1e-6,
+                             solver='nbrk')
+    fft1 = np.fft.fft(solution.rho[:,3])  # Checking if the main frequency is the Rabi frequency
+    fft1 = fft1[:round(len(solution.t)/2)]
+    fft1 = np.abs(fft1)
+
+    freq_loc = np.argmax(fft1[1:])
+
+    freq = np.linspace(np.pi/endTime, np.pi*sampleNum/endTime, len(fft1))
+    val = freq[freq_loc]  # The strongest frequency value
+
+    np.testing.assert_allclose(red_rabi_freq, val, rtol=0.05,
                                err_msg='cyrk_doe two level time solution not working')
```

### Comparing `rydiqule-1.0.0/tests/test_time_ham_gen.py` & `rydiqule-1.0.0rc2/tests/test_time_ham_gen.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import numpy as np
-import rydiqule as rq
-import pytest
-from rydiqule import Sensor
-
-@pytest.mark.time
-def test_time_ham_gen():
-    s = rq.Sensor(3)
-    step = lambda t: 0 if t<1 else 1
-    s.add_coupling(states=(0,1),detuning=1, rabi_frequency=2+2j)
-    s.add_coupling(states=(1,2), detuning=2, rabi_frequency=[-1,0,1], time_dependence=step)
-    calc_ham = s.get_hamiltonian()
-    calc_ham_t = s.get_time_couplings()[0][0]
-    
-    h_true = np.zeros((1,3,3), dtype=np.complex128)
-    h_true += np.diag([0,1,3])
-    h_true[:,0,1]=(2+2j)/2
-    h_true[:,1,0]=(2-2j)/2
-    
-    h_t_true = np.zeros((3,3,3),dtype=np.complex128)
-    h_t_true[:,1,2] += np.array([-1,0,1])/2
-    h_t_true[:,2,1] = np.array([-1,0,1])/2
-    
-    np.testing.assert_array_equal(calc_ham, h_true, err_msg="Steady-hamiltonian does not match theory")
-    np.testing.assert_array_equal(calc_ham_t, h_t_true, err_msg="Time Hamiltonian does not match theory")
-
+import numpy as np
+import rydiqule as rq
+import pytest
+from rydiqule import Sensor
+
+@pytest.mark.time
+def test_time_ham_gen():
+    s = rq.Sensor(3)
+    step = lambda t: 0 if t<1 else 1
+    s.add_coupling(states=(0,1),detuning=1, rabi_frequency=2+2j)
+    s.add_coupling(states=(1,2), detuning=2, rabi_frequency=[-1,0,1], time_dependence=step)
+    calc_ham = s.get_hamiltonian()
+    calc_ham_t = s.get_time_couplings()[0][0]
+    
+    h_true = np.zeros((1,3,3), dtype=np.complex128)
+    h_true += np.diag([0,1,3])
+    h_true[:,0,1]=(2+2j)/2
+    h_true[:,1,0]=(2-2j)/2
+    
+    h_t_true = np.zeros((3,3,3),dtype=np.complex128)
+    h_t_true[:,1,2] += np.array([-1,0,1])/2
+    h_t_true[:,2,1] = np.array([-1,0,1])/2
+    
+    np.testing.assert_array_equal(calc_ham, h_true, err_msg="Steady-hamiltonian does not match theory")
+    np.testing.assert_array_equal(calc_ham_t, h_t_true, err_msg="Time Hamiltonian does not match theory")
+
```

### Comparing `rydiqule-1.0.0/tests/test_utils.py` & `rydiqule-1.0.0rc2/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-import numpy as np
-from rydiqule.doppler_utils import gaussian3d, doppler_classes, doppler_mesh
-from rydiqule import matrix_slice
-import pytest
-
-
-@pytest.mark.doppler
-@pytest.mark.high_memory
-@pytest.mark.parametrize("spatial_dim", [1,2,3])
-def test_gaussian(spatial_dim):
-    """Confirms that the gaussian averaging function integrates to 1 in multiple dimensions"""
-
-    if spatial_dim == 3:
-        # for 3D, lower the meshing density to avoid RAM overflows
-        dop_vels = doppler_classes({'method':'split','n_doppler':51,'n_coherent':201})
-    else:
-        dop_vels = doppler_classes({'method':'split'})
-
-    Vs, Diffs = doppler_mesh(dop_vels,spatial_dim)
-
-    weighting = Diffs.prod(axis=0)*gaussian3d(Vs)
-
-    total = weighting.sum(axis=None)
-
-    # confirm the integration is within 3%
-    print(f'{spatial_dim:d}-D gaussian integration: {total:.2f}')
-    assert total == pytest.approx(1.0, abs=3e-2), \
-        f'{spatial_dim:d}-D gaussian integration not normalized'
-
-
-@pytest.mark.doppler
-@pytest.mark.util
-def test_doppler_classes_assertion():
-    """Confirms that doppler_classes correctly screens direct array inputs as 1-D"""
-
-    # python list input
-    l = [i for i in range(-10,11)]
-    l_out = doppler_classes({'method':'direct','doppler_velocities':l})
-    assert l_out == pytest.approx(l), 'Python list input mangled'
-
-    # numpy 1-D array input
-    arr = np.linspace(-1,1,100)
-    arr_out = doppler_classes({'method':'direct','doppler_velocities':arr})
-    assert arr_out == pytest.approx(arr), 'Numpy 1-D array input mangled'
-
-    # numpy 2-D array input
-    with pytest.raises(AssertionError,match='doppler_velocities must be 1-D'):
-        arr2 = arr.reshape(20,5)
-        _ = doppler_classes({'method':'direct','doppler_velocities':arr2})
-        
-        
-@pytest.mark.util
-def test_matrix_slice():
-    """Uses a test set of matrices to ensure they slice correctly"""
-    M1 = np.ones((1,15,5,5))
-    M2 = np.ones((10,1,5,5))
-    M3 = np.ones((10,15,5,5))
-
-    shapes = [M.shape for M in [M1,M2,M3]]
-
-    total_size_true = np.prod(np.broadcast_shapes(*shapes))
-    total_size_calc = 0
-
-    for _, m1, m2, m3 in matrix_slice(M1, M2, M3, n_slices=3):
-        total_size_calc += np.prod(np.broadcast_shapes(m1.shape,m2.shape,m3.shape))
-
+import numpy as np
+from rydiqule.doppler_utils import gaussian3d, doppler_classes, doppler_mesh
+from rydiqule import matrix_slice
+import pytest
+
+
+@pytest.mark.doppler
+@pytest.mark.high_memory
+@pytest.mark.parametrize("spatial_dim", [1,2,3])
+def test_gaussian(spatial_dim):
+    """Confirms that the gaussian averaging function integrates to 1 in multiple dimensions"""
+
+    if spatial_dim == 3:
+        # for 3D, lower the meshing density to avoid RAM overflows
+        dop_vels = doppler_classes({'method':'split','n_doppler':51,'n_coherent':201})
+    else:
+        dop_vels = doppler_classes({'method':'split'})
+
+    Vs, Diffs = doppler_mesh(dop_vels,spatial_dim)
+
+    weighting = Diffs.prod(axis=0)*gaussian3d(Vs)
+
+    total = weighting.sum(axis=None)
+
+    # confirm the integration is within 3%
+    print(f'{spatial_dim:d}-D gaussian integration: {total:.2f}')
+    assert total == pytest.approx(1.0, abs=3e-2), \
+        f'{spatial_dim:d}-D gaussian integration not normalized'
+
+
+@pytest.mark.doppler
+@pytest.mark.util
+def test_doppler_classes_assertion():
+    """Confirms that doppler_classes correctly screens direct array inputs as 1-D"""
+
+    # python list input
+    l = [i for i in range(-10,11)]
+    l_out = doppler_classes({'method':'direct','doppler_velocities':l})
+    assert l_out == pytest.approx(l), 'Python list input mangled'
+
+    # numpy 1-D array input
+    arr = np.linspace(-1,1,100)
+    arr_out = doppler_classes({'method':'direct','doppler_velocities':arr})
+    assert arr_out == pytest.approx(arr), 'Numpy 1-D array input mangled'
+
+    # numpy 2-D array input
+    with pytest.raises(AssertionError,match='doppler_velocities must be 1-D'):
+        arr2 = arr.reshape(20,5)
+        _ = doppler_classes({'method':'direct','doppler_velocities':arr2})
+        
+        
+@pytest.mark.util
+def test_matrix_slice():
+    """Uses a test set of matrices to ensure they slice correctly"""
+    M1 = np.ones((1,15,5,5))
+    M2 = np.ones((10,1,5,5))
+    M3 = np.ones((10,15,5,5))
+
+    shapes = [M.shape for M in [M1,M2,M3]]
+
+    total_size_true = np.prod(np.broadcast_shapes(*shapes))
+    total_size_calc = 0
+
+    for _, m1, m2, m3 in matrix_slice(M1, M2, M3, n_slices=3):
+        total_size_calc += np.prod(np.broadcast_shapes(m1.shape,m2.shape,m3.shape))
+
     assert total_size_calc == total_size_true
```

