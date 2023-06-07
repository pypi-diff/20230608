# Comparing `tmp/myokit-1.33.9.tar.gz` & `tmp/myokit-1.34.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myokit-1.33.9.tar", last modified: Tue Nov  8 12:15:08 2022, max compression
+gzip compressed data, was "myokit-1.34.0.tar", last modified: Wed Jun  7 22:21:18 2023, max compression
```

## Comparing `myokit-1.33.9.tar` & `myokit-1.34.0.tar`

### file list

```diff
@@ -1,466 +1,456 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.773221 myokit-1.33.9/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1833 2022-01-24 10:05:12.000000 myokit-1.33.9/LICENSE.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)      221 2021-02-24 20:23:20.000000 myokit-1.33.9/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     5130 2022-11-08 12:15:08.773221 myokit-1.33.9/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     3845 2022-11-08 11:14:12.000000 myokit-1.33.9/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.409217 myokit-1.33.9/myokit/
--rw-r--r--   0 michael   (1000) michael   (1000)    14908 2022-11-08 11:14:12.000000 myokit-1.33.9/myokit/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    60379 2022-11-08 11:14:12.000000 myokit-1.33.9/myokit/__main__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    22452 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/_aux.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.412217 myokit-1.33.9/myokit/_bin/
--rw-rw-r--   0 michael   (1000) michael   (1000)     6276 2022-06-22 14:03:27.000000 myokit-1.33.9/myokit/_bin/example.mmt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.431217 myokit-1.33.9/myokit/_bin/gui/
--rw-rw-r--   0 michael   (1000) michael   (1000)      784 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/find.png
--rw-rw-r--   0 michael   (1000) michael   (1000)    96412 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer-128.xpm
--rw-rw-r--   0 michael   (1000) michael   (1000)     3528 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer-16.xpm
--rw-rw-r--   0 michael   (1000) michael   (1000)     7752 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer-24.xpm
--rw-rw-r--   0 michael   (1000) michael   (1000)   233500 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer-256.xpm
--rw-rw-r--   0 michael   (1000) michael   (1000)    12232 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer-32.xpm
--rw-rw-r--   0 michael   (1000) michael   (1000)    23817 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer-48.xpm
--rw-rw-r--   0 michael   (1000) michael   (1000)    36761 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer-64.xpm
--rw-rw-r--   0 michael   (1000) michael   (1000)    65257 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer-96.xpm
--rw-rw-r--   0 michael   (1000) michael   (1000)   143766 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer.ico
--rw-rw-r--   0 michael   (1000) michael   (1000)    30396 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer.png
--rw-rw-r--   0 michael   (1000) michael   (1000)    47406 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-ide-128.xpm
--rw-rw-r--   0 michael   (1000) michael   (1000)     2987 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-ide-16.xpm
--rw-rw-r--   0 michael   (1000) michael   (1000)     4971 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-ide-24.xpm
--rw-rw-r--   0 michael   (1000) michael   (1000)   152751 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-ide-256.xpm
--rw-rw-r--   0 michael   (1000) michael   (1000)     7355 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-ide-32.xpm
--rw-rw-r--   0 michael   (1000) michael   (1000)     9835 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-ide-48.xpm
--rw-rw-r--   0 michael   (1000) michael   (1000)    16235 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-ide-64.xpm
--rw-rw-r--   0 michael   (1000) michael   (1000)    30683 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-ide-96.xpm
--rw-rw-r--   0 michael   (1000) michael   (1000)   143766 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-ide.ico
--rw-rw-r--   0 michael   (1000) michael   (1000)    15096 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/icon-ide.png
--rw-rw-r--   0 michael   (1000) michael   (1000)      571 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/new.png
--rw-rw-r--   0 michael   (1000) michael   (1000)      544 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/open.png
--rw-rw-r--   0 michael   (1000) michael   (1000)      273 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/redo.png
--rw-rw-r--   0 michael   (1000) michael   (1000)      320 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/run.png
--rw-rw-r--   0 michael   (1000) michael   (1000)      565 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/save.png
--rw-rw-r--   0 michael   (1000) michael   (1000)      284 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/gui/undo.png
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.435217 myokit-1.33.9/myokit/_bin/install-lin/
--rwxrwxr-x   0 michael   (1000) michael   (1000)      254 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/install-lin/myokit-datablock-viewer.desktop
--rwxrwxr-x   0 michael   (1000) michael   (1000)      266 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/install-lin/myokit-datalog-viewer.desktop
--rwxrwxr-x   0 michael   (1000) michael   (1000)      264 2021-08-03 07:09:27.000000 myokit-1.33.9/myokit/_bin/install-lin/myokit-ide.desktop
--rw-rw-r--   0 michael   (1000) michael   (1000)     4338 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/install-lin/myokit.lang
--rw-rw-r--   0 michael   (1000) michael   (1000)      333 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/install-lin/x-abf.xml
--rw-rw-r--   0 michael   (1000) michael   (1000)      246 2021-08-03 07:09:27.000000 myokit-1.33.9/myokit/_bin/install-lin/x-cellml.xml
--rw-rw-r--   0 michael   (1000) michael   (1000)      247 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/install-lin/x-myokit.xml
--rw-rw-r--   0 michael   (1000) michael   (1000)      275 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_bin/install-lin/x-wcp.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.435217 myokit-1.33.9/myokit/_bin/install-win/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1025 2021-11-10 14:59:29.000000 myokit-1.33.9/myokit/_bin/install-win/menu.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.435217 myokit-1.33.9/myokit/_bin/sundials-win-vs/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1758 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/LICENSE
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.399217 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.437217 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/cvodes/
--rw-rw-r--   0 michael   (1000) michael   (1000)    27506 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h
--rw-rw-r--   0 michael   (1000) michael   (1000)     2427 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h
--rw-rw-r--   0 michael   (1000) michael   (1000)    12344 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.438217 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/nvector/
--rw-rw-r--   0 michael   (1000) michael   (1000)     8934 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.443217 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/
--rw-rw-r--   0 michael   (1000) michael   (1000)     5785 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h
--rw-rw-r--   0 michael   (1000) michael   (1000)     8997 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h
--rw-rw-r--   0 michael   (1000) michael   (1000)    13330 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h
--rw-rw-r--   0 michael   (1000) michael   (1000)     1024 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h
--rw-rw-r--   0 michael   (1000) michael   (1000)    10283 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h
--rw-rw-r--   0 michael   (1000) michael   (1000)     9385 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h
--rw-rw-r--   0 michael   (1000) michael   (1000)     5420 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h
--rw-rw-r--   0 michael   (1000) michael   (1000)     9190 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h
--rw-rw-r--   0 michael   (1000) michael   (1000)    12559 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h
--rw-rw-r--   0 michael   (1000) michael   (1000)     5165 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h
--rw-rw-r--   0 michael   (1000) michael   (1000)     1266 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.444217 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sunlinsol/
--rw-rw-r--   0 michael   (1000) michael   (1000)     2983 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.444217 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sunmatrix/
--rw-rw-r--   0 michael   (1000) michael   (1000)     3647 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.452217 myokit-1.33.9/myokit/_bin/sundials-win-vs/lib/
--rw-rw-r--   0 michael   (1000) michael   (1000)   677888 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll
--rw-rw-r--   0 michael   (1000) michael   (1000)   169196 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib
--rw-rw-r--   0 michael   (1000) michael   (1000)   160768 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll
--rw-rw-r--   0 michael   (1000) michael   (1000)    59576 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib
--rw-r--r--   0 michael   (1000) michael   (1000)    12309 2022-11-08 11:14:12.000000 myokit-1.33.9/myokit/_config.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    68708 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/_datablock.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    68918 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/_datalog.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    11182 2021-08-04 21:14:28.000000 myokit-1.33.9/myokit/_err.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      438 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_exec_new.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      448 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_exec_old.py
--rw-r--r--   0 michael   (1000) michael   (1000)   105002 2022-11-08 11:14:12.000000 myokit-1.33.9/myokit/_expressions.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9390 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/_io.py
--rw-r--r--   0 michael   (1000) michael   (1000)   184074 2022-11-08 11:14:12.000000 myokit-1.33.9/myokit/_model_api.py
--rw-r--r--   0 michael   (1000) michael   (1000)      836 2022-11-08 12:09:23.000000 myokit-1.33.9/myokit/_myokit_version.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    74360 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/_parsing.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4567 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_progress.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    27720 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/_protocol.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.464218 myokit-1.33.9/myokit/_sim/
--rw-r--r--   0 michael   (1000) michael   (1000)    13853 2022-11-08 11:14:12.000000 myokit-1.33.9/myokit/_sim/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    19217 2022-01-10 10:29:37.000000 myokit-1.33.9/myokit/_sim/cable.c
--rw-rw-r--   0 michael   (1000) michael   (1000)    18922 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/_sim/cable.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    37244 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/_sim/cmodel.h
--rw-rw-r--   0 michael   (1000) michael   (1000)    15922 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/_sim/cmodel.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4047 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_sim/compiler.c
--rw-rw-r--   0 michael   (1000) michael   (1000)     2784 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_sim/compiler.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    56941 2022-01-10 10:29:37.000000 myokit-1.33.9/myokit/_sim/cvodesim.c
--rw-rw-r--   0 michael   (1000) michael   (1000)    24851 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/_sim/cvodesim.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    68174 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/_sim/cvodessim.c
--rw-r--r--   0 michael   (1000) michael   (1000)    41208 2022-11-08 11:52:00.000000 myokit-1.33.9/myokit/_sim/cvodessim.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    15451 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/_sim/differential.hpp
--rw-rw-r--   0 michael   (1000) michael   (1000)    47580 2022-01-10 10:29:37.000000 myokit-1.33.9/myokit/_sim/fiber_tissue.c
--rw-rw-r--   0 michael   (1000) michael   (1000)    50786 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/_sim/fiber_tissue.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    18324 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_sim/icsim.cpp
--rw-rw-r--   0 michael   (1000) michael   (1000)    12940 2022-03-10 11:16:58.000000 myokit-1.33.9/myokit/_sim/icsim.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     8014 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_sim/jacobian.cpp
--rw-rw-r--   0 michael   (1000) michael   (1000)    12946 2022-01-10 10:29:37.000000 myokit-1.33.9/myokit/_sim/jacobian.py
--rw-r--r--   0 michael   (1000) michael   (1000)    31548 2022-11-08 11:14:12.000000 myokit-1.33.9/myokit/_sim/mcl.h
--rw-rw-r--   0 michael   (1000) michael   (1000)     5037 2022-01-10 10:29:37.000000 myokit-1.33.9/myokit/_sim/opencl.c
--rw-rw-r--   0 michael   (1000) michael   (1000)    16315 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/_sim/opencl.py
--rw-r--r--   0 michael   (1000) michael   (1000)    46684 2022-11-08 11:14:12.000000 myokit-1.33.9/myokit/_sim/openclsim.c
--rw-rw-r--   0 michael   (1000) michael   (1000)    19363 2021-06-06 21:12:56.000000 myokit-1.33.9/myokit/_sim/openclsim.cl
--rw-rw-r--   0 michael   (1000) michael   (1000)    69035 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/_sim/openclsim.py
--rw-r--r--   0 michael   (1000) michael   (1000)    28789 2022-11-08 11:14:12.000000 myokit-1.33.9/myokit/_sim/pacing.h
--rw-rw-r--   0 michael   (1000) michael   (1000)    22009 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_sim/psim.cpp
--rw-rw-r--   0 michael   (1000) michael   (1000)    17795 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/_sim/psim.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    11122 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_sim/rhs.c
--rw-rw-r--   0 michael   (1000) michael   (1000)     7635 2022-01-10 10:29:37.000000 myokit-1.33.9/myokit/_sim/rhs.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1720 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/_sim/sundials.c
--rw-rw-r--   0 michael   (1000) michael   (1000)     3092 2022-01-10 10:29:37.000000 myokit-1.33.9/myokit/_sim/sundials.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4835 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/_system.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    30096 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/_unit.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3172 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/float.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.464218 myokit-1.33.9/myokit/formats/
--rw-rw-r--   0 michael   (1000) michael   (1000)    20284 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/formats/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.464218 myokit-1.33.9/myokit/formats/ansic/
--rw-rw-r--   0 michael   (1000) michael   (1000)     3453 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/ansic/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3698 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/ansic/_ewriter.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5468 2022-01-10 10:29:37.000000 myokit-1.33.9/myokit/formats/ansic/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.466218 myokit-1.33.9/myokit/formats/ansic/template/
--rw-rw-r--   0 michael   (1000) michael   (1000)    11888 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/ansic/template/cable.c
--rw-rw-r--   0 michael   (1000) michael   (1000)     6035 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/formats/ansic/template/euler.c
--rw-rw-r--   0 michael   (1000) michael   (1000)    14169 2022-01-10 10:29:37.000000 myokit-1.33.9/myokit/formats/ansic/template/sim.c
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.468218 myokit-1.33.9/myokit/formats/axon/
--rw-rw-r--   0 michael   (1000) michael   (1000)      643 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/axon/__init__.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    70267 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/formats/axon/_abf.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    10277 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/formats/axon/_atf.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      939 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/axon/_importer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.470218 myokit-1.33.9/myokit/formats/cellml/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1572 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/cellml/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2909 2022-02-02 09:21:34.000000 myokit-1.33.9/myokit/formats/cellml/_ewriter.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2451 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/cellml/_exporter.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2355 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/cellml/_importer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.472218 myokit-1.33.9/myokit/formats/cellml/v1/
--rw-rw-r--   0 michael   (1000) michael   (1000)      715 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/cellml/v1/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    59230 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/formats/cellml/v1/_api.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    43692 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/formats/cellml/v1/_parser.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    15320 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/formats/cellml/v1/_writer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.475218 myokit-1.33.9/myokit/formats/cellml/v2/
--rw-rw-r--   0 michael   (1000) michael   (1000)      704 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/cellml/v2/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    59297 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/formats/cellml/v2/_api.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    29674 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/formats/cellml/v2/_parser.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12108 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/formats/cellml/v2/_writer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.476218 myokit-1.33.9/myokit/formats/channelml/
--rw-rw-r--   0 michael   (1000) michael   (1000)      549 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/channelml/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    14840 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/channelml/_importer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.477218 myokit-1.33.9/myokit/formats/cpp/
--rw-rw-r--   0 michael   (1000) michael   (1000)      631 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/cpp/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      527 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/cpp/_ewriter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.479218 myokit-1.33.9/myokit/formats/cuda/
--rw-rw-r--   0 michael   (1000) michael   (1000)      922 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/cuda/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4603 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/formats/cuda/_ewriter.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2165 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/cuda/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.479218 myokit-1.33.9/myokit/formats/cuda/template/
--rw-rw-r--   0 michael   (1000) michael   (1000)     8722 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/formats/cuda/template/kernel.cu
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.480218 myokit-1.33.9/myokit/formats/easyml/
--rw-rw-r--   0 michael   (1000) michael   (1000)      942 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/easyml/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3811 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/formats/easyml/_ewriter.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    15871 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/formats/easyml/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.481218 myokit-1.33.9/myokit/formats/html/
--rw-rw-r--   0 michael   (1000) michael   (1000)      563 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/html/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2449 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/html/_exporter.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     7184 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/html/_flatten.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.482218 myokit-1.33.9/myokit/formats/latex/
--rw-rw-r--   0 michael   (1000) michael   (1000)      788 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/latex/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6823 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/formats/latex/_ewriter.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5272 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/latex/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.484218 myokit-1.33.9/myokit/formats/mathml/
--rw-rw-r--   0 michael   (1000) michael   (1000)      743 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/mathml/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12444 2022-02-02 09:21:34.000000 myokit-1.33.9/myokit/formats/mathml/_ewriter.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    34420 2022-02-02 09:21:34.000000 myokit-1.33.9/myokit/formats/mathml/_parser.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.485218 myokit-1.33.9/myokit/formats/matlab/
--rw-rw-r--   0 michael   (1000) michael   (1000)      801 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/matlab/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3306 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/matlab/_ewriter.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2966 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/matlab/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.488218 myokit-1.33.9/myokit/formats/matlab/template/
--rw-rw-r--   0 michael   (1000) michael   (1000)      528 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/matlab/template/constants.m
--rw-rw-r--   0 michael   (1000) michael   (1000)      374 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/matlab/template/ifthenelse.m
--rw-rw-r--   0 michael   (1000) michael   (1000)     2003 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/matlab/template/main.m
--rw-rw-r--   0 michael   (1000) michael   (1000)      861 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/matlab/template/model.m
--rw-rw-r--   0 michael   (1000) michael   (1000)      461 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/matlab/template/model_wrapper.m
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.489218 myokit-1.33.9/myokit/formats/opencl/
--rw-rw-r--   0 michael   (1000) michael   (1000)     7068 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/opencl/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5394 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/formats/opencl/_ewriter.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3994 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/opencl/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.492218 myokit-1.33.9/myokit/formats/opencl/template/
--rw-rw-r--   0 michael   (1000) michael   (1000)    11600 2022-01-10 10:29:37.000000 myokit-1.33.9/myokit/formats/opencl/template/cable.c
--rw-rw-r--   0 michael   (1000) michael   (1000)     8159 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/formats/opencl/template/kernel.cl
--rw-rw-r--   0 michael   (1000) michael   (1000)     9005 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/formats/opencl/template/minilog.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     1042 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/opencl/template/plot.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)      162 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/opencl/template/test
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.493218 myokit-1.33.9/myokit/formats/python/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1155 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/python/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6912 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/formats/python/_ewriter.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1075 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/python/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.494218 myokit-1.33.9/myokit/formats/python/template/
--rw-rw-r--   0 michael   (1000) michael   (1000)    10406 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/python/template/sim.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.496218 myokit-1.33.9/myokit/formats/sbml/
--rw-rw-r--   0 michael   (1000) michael   (1000)      759 2021-08-04 21:14:28.000000 myokit-1.33.9/myokit/formats/sbml/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    59488 2022-01-10 10:29:37.000000 myokit-1.33.9/myokit/formats/sbml/_api.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1111 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/sbml/_importer.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    29317 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/formats/sbml/_parser.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.498218 myokit-1.33.9/myokit/formats/stan/
--rw-rw-r--   0 michael   (1000) michael   (1000)     2983 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/stan/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3233 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/stan/_ewriter.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3860 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/stan/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.499218 myokit-1.33.9/myokit/formats/stan/template/
--rw-rw-r--   0 michael   (1000) michael   (1000)     5306 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/stan/template/cell.stan
--rwxrwxr-x   0 michael   (1000) michael   (1000)       92 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/stan/template/run.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.502218 myokit-1.33.9/myokit/formats/sympy/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1744 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/formats/sympy/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6872 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/sympy/_ereader.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5008 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/formats/sympy/_ewriter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.503218 myokit-1.33.9/myokit/formats/wcp/
--rw-rw-r--   0 michael   (1000) michael   (1000)      360 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/wcp/__init__.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    10511 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/formats/wcp/_wcp.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.506218 myokit-1.33.9/myokit/formats/xml/
--rw-rw-r--   0 michael   (1000) michael   (1000)      551 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/xml/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1600 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/xml/_exporter.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      499 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/formats/xml/_split.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.513218 myokit-1.33.9/myokit/gui/
--rw-rw-r--   0 michael   (1000) michael   (1000)    11993 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/gui/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    46627 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/gui/datablock_viewer.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    28117 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/gui/datalog_viewer.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     8607 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/gui/explorer.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)   106773 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/gui/ide.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2174 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/gui/progress.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    50886 2022-02-06 17:58:38.000000 myokit-1.33.9/myokit/gui/source.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6270 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/gui/vargrapher.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.520218 myokit-1.33.9/myokit/lib/
--rw-rw-r--   0 michael   (1000) michael   (1000)      216 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/lib/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    37373 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/lib/common.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    23949 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/lib/deps.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    28160 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/lib/guess.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    46700 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/lib/hh.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    67906 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/lib/markov.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4513 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/lib/multi.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    13572 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/lib/plots.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4658 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/pacing.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     8504 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/pype.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.637220 myokit-1.33.9/myokit/tests/
--rw-rw-r--   0 michael   (1000) michael   (1000)     7898 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2830 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/ansic_event_based_pacing.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1396 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/ansic_fixed_form_pacing.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.648219 myokit-1.33.9/myokit/tests/data/
--rw-rw-r--   0 michael   (1000) michael   (1000)     3022 2021-05-23 22:45:25.000000 myokit-1.33.9/myokit/tests/data/beeler-1977-model-compare-a.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)     2886 2021-05-23 22:45:25.000000 myokit-1.33.9/myokit/tests/data/beeler-1977-model-compare-b.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)     3137 2021-05-23 22:45:25.000000 myokit-1.33.9/myokit/tests/data/beeler-1977-model.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)       99 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/beeler-1977-protocol.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)      290 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/beeler-1977-script.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)     3287 2021-05-23 22:45:25.000000 myokit-1.33.9/myokit/tests/data/beeler-1977-units.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)     5082 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/clancy-1999-fitting.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)     3128 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/conditional.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)     6067 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/tests/data/cv1d.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)   109483 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/cv1d.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)    23916 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/decker-2009.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)    18350 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/decker.model
--rw-rw-r--   0 michael   (1000) michael   (1000)    10416 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/dn-1985-normalised.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)      800 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/dom-markov.mmt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.651219 myokit-1.33.9/myokit/tests/data/formats/
--rw-rw-r--   0 michael   (1000) michael   (1000)     8192 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/abf-protocol.pro
--rw-rw-r--   0 michael   (1000) michael   (1000)    98376 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/abf-v1.abf
--rw-rw-r--   0 michael   (1000) michael   (1000)    24576 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/abf-v2.abf
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.660220 myokit-1.33.9/myokit/tests/data/formats/cellml/
--rw-rw-r--   0 michael   (1000) michael   (1000)      188 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/cellml/LICENSE
--rw-rw-r--   0 michael   (1000) michael   (1000)    59093 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/cellml/br-1977-dot.cellml
--rw-rw-r--   0 michael   (1000) michael   (1000)    58593 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/cellml/br-1977.cellml
--rw-rw-r--   0 michael   (1000) michael   (1000)   117223 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/cellml/corrias.cellml
--rw-rw-r--   0 michael   (1000) michael   (1000)   221953 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/cellml/decker-2009.cellml
--rw-rw-r--   0 michael   (1000) michael   (1000)     1595 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/cellml/documentation.cellml
--rw-rw-r--   0 michael   (1000) michael   (1000)      118 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/cellml/invalid-file.cellml
--rw-rw-r--   0 michael   (1000) michael   (1000)    44837 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml
--rw-rw-r--   0 michael   (1000) michael   (1000)    44947 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.669220 myokit-1.33.9/myokit/tests/data/formats/channelml/
--rw-rw-r--   0 michael   (1000) michael   (1000)     2648 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)      557 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)      549 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)     2702 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)      549 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)     2369 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)     1258 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)     1539 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)     1402 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)     1402 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)     1338 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)     1338 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)     1290 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)     1289 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)     1374 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)     1373 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)      675 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)     1398 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml
--rw-rw-r--   0 michael   (1000) michael   (1000)     1317 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.670220 myokit-1.33.9/myokit/tests/data/formats/sbml/
--rw-rw-r--   0 michael   (1000) michael   (1000)     8719 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml
--rw-rw-r--   0 michael   (1000) michael   (1000)     9801 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml
--rw-rw-r--   0 michael   (1000) michael   (1000)    31408 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/sbml/HodgkinHuxley.xml
--rw-rw-r--   0 michael   (1000) michael   (1000)      493 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/sbml/LICENSE
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.672220 myokit-1.33.9/myokit/tests/data/formats/sbml/model/
--rw-rw-r--   0 michael   (1000) michael   (1000)     2149 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml
--rw-rw-r--   0 michael   (1000) michael   (1000)     2952 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml
--rw-rw-r--   0 michael   (1000) michael   (1000)     1226 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.673220 myokit-1.33.9/myokit/tests/data/formats/sbml/result/
--rw-rw-r--   0 michael   (1000) michael   (1000)     2457 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/sbml/result/00001-results.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)     2206 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/sbml/result/00004-results.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)     1131 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/sbml/result/01103-results.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)    25600 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/formats/wcp-file.wcp
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.770221 myokit-1.33.9/myokit/tests/data/io/
--rw-rw-r--   0 michael   (1000) michael   (1000)      735 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/bad1d-1-not-enough-files.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)   109429 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/bad1d-2-no-header.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)   104768 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/bad1d-3-no-data.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)     3026 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/bad1d-4-not-a-zip.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)   109458 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/bad1d-5-bad-data-type.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)     1549 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/bad1d-6-time-too-short.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)     1584 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/bad1d-7-0d-too-short.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)   109483 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/bad1d-8-1d-too-short.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)      739 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/bad2d-1-not-enough-files.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)   346240 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/bad2d-2-no-header.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)   333091 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/bad2d-3-no-data.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)     3026 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/bad2d-4-not-a-zip.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)   346257 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/bad2d-5-bad-data-type.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)     1553 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/bad2d-6-time-too-short.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)     1588 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/bad2d-7-0d-too-short.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)   346276 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/bad2d-8-2d-too-short.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)      623 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/badlog-1-no-data.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)     1281 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/badlog-2-no-structure.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)       99 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/badlog-3-not-a-zip.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)     1458 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/badlog-4-invalid-n-fields.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)     1458 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/badlog-5-invalid-data-size.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)     1457 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/badlog-6-bad-data-type.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)     1458 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/badlog-7-not-enough-data.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)     6031 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/tests/data/io/block2d.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)   346276 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/block2d.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)        0 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog-1-empty.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)        5 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog-10-just-spaces.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)        2 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog-11-just-a-semicolon.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)      104 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog-12-bad-header.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)      107 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog-13-header-with-empty-1.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)      105 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog-14-header-with-empty-2.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)      105 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog-15-header-with-empty-3.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)      107 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog-16-wrong-columns-in-data.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)      106 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog-17-non-float-data.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)      112 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog-2-windows.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)      103 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog-3-old-mac.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)      107 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog-4-empty-lines.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)      110 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog-5-semicolons.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)      119 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog-6-open-string.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)      110 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog-7-empty-lines-2.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)      100 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog-8-unquoted-header.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)      114 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog-9-double-quoted-header.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)      109 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/datalog.csv
--rw-rw-r--   0 michael   (1000) michael   (1000)     1421 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/io/goodlog.zip
--rw-rw-r--   0 michael   (1000) michael   (1000)     4992 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/lr-1991-dep.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)     2315 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/lr-1991-fitting.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)     4571 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/lr-1991-testing.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)     6124 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/lr-1991.mmt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.772221 myokit-1.33.9/myokit/tests/data/multi/
--rw-rw-r--   0 michael   (1000) michael   (1000)       99 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/multi/beeler-1977-protocol.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)      290 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/multi/beeler-1977-script.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)     3008 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/multi/beeler-no-name.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)     6013 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/multi/lr-1991.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)      109 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/multi/not-a-model.csv
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.772221 myokit-1.33.9/myokit/tests/data/multi/subdir/
--rw-rw-r--   0 michael   (1000) michael   (1000)     3008 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/multi/subdir/beeler-no-name.mmt
--rw-rw-r--   0 michael   (1000) michael   (1000)     3754 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/data/noble-1962.mmt
--rwxrwxr-x   0 michael   (1000) michael   (1000)    22935 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_aux.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    57357 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_cellml_v1_api.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    42270 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_cellml_v1_parser.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    12819 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_cellml_v1_writer.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    73695 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_cellml_v2_api.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    26746 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_cellml_v2_parser.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    11264 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_cellml_v2_writer.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     4033 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_cmodel.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)      704 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/test_compiler_detection.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    12377 2022-02-06 17:58:38.000000 myokit-1.33.9/myokit/tests/test_component.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    12598 2022-11-08 11:14:12.000000 myokit-1.33.9/myokit/tests/test_config.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    50041 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_datablock.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    82887 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_datalog.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    61106 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_dependency_checking.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)   138795 2022-11-08 11:34:34.000000 myokit-1.33.9/myokit/tests/test_expressions.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     5053 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/tests/test_float.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     4523 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_formats.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    15162 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_formats_axon.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    19483 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_formats_cellml.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     7137 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_formats_channelml.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    11791 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_formats_easyml.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     9610 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_formats_exporters.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    41242 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/tests/test_formats_expression_writers.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     3645 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/test_formats_html.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     1972 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_formats_importers.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    37731 2022-02-02 09:21:34.000000 myokit-1.33.9/myokit/tests/test_formats_mathml_content.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     9013 2022-02-02 09:21:34.000000 myokit-1.33.9/myokit/tests/test_formats_mathml_presentation.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    17615 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/test_formats_opencl.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     5106 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_formats_sbml.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    10611 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_formats_sympy.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     1891 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_formats_wcp.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    14162 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_io.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     2053 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_jacobian_calculator.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     2054 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_jacobian_tracer.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     3639 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_lib_common.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     7763 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/test_lib_deps.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    42620 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_lib_guess.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    30691 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_lib_hh.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    39489 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_lib_markov.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     5432 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_lib_multi.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     5893 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_lib_plots.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     2935 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_meta.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    73487 2022-11-08 11:14:12.000000 myokit-1.33.9/myokit/tests/test_model.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    18841 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/test_model_building.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     4068 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_opencl_info.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     8299 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_pacing_factory.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     5967 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_pacing_system_c.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3235 2021-02-24 20:23:20.000000 myokit-1.33.9/myokit/tests/test_pacing_system_py.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    49048 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_parsing.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     2868 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/tests/test_progress_reporters.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    15379 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_protocol.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    12853 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_protocol_floating_point.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     2689 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_pype.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     7640 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_quantity.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     3738 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_rhs_benchmarker.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    71917 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_sbml_api.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    54976 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_sbml_parser.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    17174 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_simulation_1d.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    21380 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_simulation_cvode.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    33239 2022-06-22 15:17:27.000000 myokit-1.33.9/myokit/tests/test_simulation_cvodes.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     1959 2022-06-22 17:32:44.000000 myokit-1.33.9/myokit/tests/test_simulation_cvodes_from_disk.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    34456 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_simulation_fiber_tissue.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     3284 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_simulation_ic.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    28721 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_simulation_log_interval.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    58505 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_simulation_opencl.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     3110 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_simulation_opencl_log_interval.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    20401 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_simulation_opencl_vs_cvode.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     5503 2022-05-09 14:52:58.000000 myokit-1.33.9/myokit/tests/test_simulation_opencl_vs_sim1d.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     7722 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_simulation_p.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)      790 2021-05-05 18:05:06.000000 myokit-1.33.9/myokit/tests/test_system_info.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    10578 2022-06-22 17:32:44.000000 myokit-1.33.9/myokit/tests/test_tools.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    13923 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_unit.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2009 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_user_functions.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    25859 2022-08-30 00:40:10.000000 myokit-1.33.9/myokit/tests/test_variable.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    17487 2022-06-22 17:32:44.000000 myokit-1.33.9/myokit/tools.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     8522 2021-11-10 14:59:29.000000 myokit-1.33.9/myokit/units.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-08 12:15:08.411217 myokit-1.33.9/myokit.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)     5130 2022-11-08 12:15:08.000000 myokit-1.33.9/myokit.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)    15293 2022-11-08 12:15:08.000000 myokit-1.33.9/myokit.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2022-11-08 12:15:08.000000 myokit-1.33.9/myokit.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       49 2022-11-08 12:15:08.000000 myokit-1.33.9/myokit.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2022-09-23 15:49:28.000000 myokit-1.33.9/myokit.egg-info/not-zip-safe
--rw-rw-r--   0 michael   (1000) michael   (1000)      182 2022-11-08 12:15:08.000000 myokit-1.33.9/myokit.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        7 2022-11-08 12:15:08.000000 myokit-1.33.9/myokit.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2022-11-08 12:15:08.773221 myokit-1.33.9/setup.cfg
--rw-rw-r--   0 michael   (1000) michael   (1000)     3301 2022-08-30 00:40:10.000000 myokit-1.33.9/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.397337 myokit-1.34.0/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1833 2023-06-07 13:48:59.000000 myokit-1.34.0/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      221 2023-06-07 13:48:23.000000 myokit-1.34.0/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     5086 2023-06-07 22:21:18.397337 myokit-1.34.0/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     3821 2023-06-07 13:48:59.000000 myokit-1.34.0/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.361337 myokit-1.34.0/myokit/
+-rw-r--r--   0 michael   (1000) michael   (1000)    14696 2023-06-07 22:09:50.000000 myokit-1.34.0/myokit/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    59821 2023-06-07 22:09:50.000000 myokit-1.34.0/myokit/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23902 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_aux.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.362337 myokit-1.34.0/myokit/_bin/
+-rw-r--r--   0 michael   (1000) michael   (1000)     6226 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/example.mmt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.364337 myokit-1.34.0/myokit/_bin/gui/
+-rw-r--r--   0 michael   (1000) michael   (1000)      784 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/find.png
+-rw-r--r--   0 michael   (1000) michael   (1000)    96412 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-128.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     3528 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-16.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     7752 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-24.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   233500 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-256.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    12232 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-32.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    23817 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-48.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    36761 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-64.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    65257 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-96.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)    30396 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer.png
+-rw-r--r--   0 michael   (1000) michael   (1000)    47406 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide-128.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     2987 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide-16.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     4971 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide-24.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   152751 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide-256.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     7355 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide-32.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     9835 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide-48.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    16235 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide-64.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    30683 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide-96.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)    15096 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/icon-ide.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      571 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/new.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      544 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/open.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/redo.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/run.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      565 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/save.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      284 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/_bin/gui/undo.png
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.364337 myokit-1.34.0/myokit/_bin/install-lin/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      254 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/_bin/install-lin/myokit-datablock-viewer.desktop
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      266 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/_bin/install-lin/myokit-datalog-viewer.desktop
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      264 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/install-lin/myokit-ide.desktop
+-rw-r--r--   0 michael   (1000) michael   (1000)     4338 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/_bin/install-lin/myokit.lang
+-rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-06-07 13:47:50.000000 myokit-1.34.0/myokit/_bin/install-lin/x-abf.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      246 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/install-lin/x-cellml.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      247 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/_bin/install-lin/x-myokit.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      275 2023-06-07 13:47:50.000000 myokit-1.34.0/myokit/_bin/install-lin/x-wcp.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.365337 myokit-1.34.0/myokit/_bin/install-win/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1025 2023-06-07 22:09:55.000000 myokit-1.34.0/myokit/_bin/install-win/menu.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.365337 myokit-1.34.0/myokit/_bin/sundials-win-vs/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1758 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/LICENSE
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.358337 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.365337 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/cvodes/
+-rw-r--r--   0 michael   (1000) michael   (1000)    27506 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     2427 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    12344 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.365337 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/nvector/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8934 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.366337 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5785 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     8997 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    13330 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     1024 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    10283 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     9385 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     5420 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     9190 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    12559 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     5165 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     1266 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.366337 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sunlinsol/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2983 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.366337 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sunmatrix/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3647 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.367337 myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/
+-rw-r--r--   0 michael   (1000) michael   (1000)   677888 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll
+-rw-r--r--   0 michael   (1000) michael   (1000)   169196 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib
+-rw-r--r--   0 michael   (1000) michael   (1000)   160768 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll
+-rw-r--r--   0 michael   (1000) michael   (1000)    59576 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib
+-rw-r--r--   0 michael   (1000) michael   (1000)    12309 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_config.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    68704 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_datablock.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    68982 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_datalog.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11462 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_err.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      438 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/_exec_new.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      448 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/_exec_old.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   105065 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_expressions.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9545 2023-06-07 18:58:09.000000 myokit-1.34.0/myokit/_io.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   193828 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_model_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      836 2023-06-07 22:19:30.000000 myokit-1.34.0/myokit/_myokit_version.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    74425 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_parsing.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4566 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_progress.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    30748 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_protocol.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.369337 myokit-1.34.0/myokit/_sim/
+-rw-r--r--   0 michael   (1000) michael   (1000)    13853 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_sim/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19220 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/cable.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    18933 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/cable.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    38822 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/cmodel.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    15889 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_sim/cmodel.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4047 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_sim/compiler.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     2784 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_sim/compiler.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    71394 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/cvodessim.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    42629 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/cvodessim.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15446 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_sim/differential.hpp
+-rw-r--r--   0 michael   (1000) michael   (1000)    47578 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_sim/fiber_tissue.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    50826 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/fiber_tissue.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8012 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_sim/jacobian.cpp
+-rw-r--r--   0 michael   (1000) michael   (1000)    13105 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_sim/jacobian.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    31548 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/mcl.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     5037 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_sim/opencl.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    16825 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_sim/opencl.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    46683 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_sim/openclsim.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    19360 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_sim/openclsim.cl
+-rw-r--r--   0 michael   (1000) michael   (1000)    69345 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/openclsim.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29825 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_sim/pacing.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    11126 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/_sim/rhs.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     7634 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_sim/rhs.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1720 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_sim/sundials.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     3092 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_sim/sundials.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4835 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/_system.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    30095 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/_unit.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3172 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/float.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.369337 myokit-1.34.0/myokit/formats/
+-rw-r--r--   0 michael   (1000) michael   (1000)    20284 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.369337 myokit-1.34.0/myokit/formats/ansic/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3453 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/ansic/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3698 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/ansic/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5467 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/formats/ansic/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.369337 myokit-1.34.0/myokit/formats/ansic/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11965 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/ansic/template/cable.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     6044 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/formats/ansic/template/euler.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    14244 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/formats/ansic/template/sim.c
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.370337 myokit-1.34.0/myokit/formats/axon/
+-rw-r--r--   0 michael   (1000) michael   (1000)      643 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/axon/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    70187 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/axon/_abf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10277 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/axon/_atf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      939 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/axon/_importer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.370337 myokit-1.34.0/myokit/formats/cellml/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1572 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cellml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2909 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/cellml/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2451 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cellml/_exporter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2355 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cellml/_importer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.370337 myokit-1.34.0/myokit/formats/cellml/v1/
+-rw-r--r--   0 michael   (1000) michael   (1000)      715 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cellml/v1/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    59236 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/cellml/v1/_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    43692 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/cellml/v1/_parser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15320 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/cellml/v1/_writer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.371337 myokit-1.34.0/myokit/formats/cellml/v2/
+-rw-r--r--   0 michael   (1000) michael   (1000)      704 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cellml/v2/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    59303 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/cellml/v2/_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29674 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/cellml/v2/_parser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    12108 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/cellml/v2/_writer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.371337 myokit-1.34.0/myokit/formats/channelml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/channelml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    14840 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/formats/channelml/_importer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.371337 myokit-1.34.0/myokit/formats/cpp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      631 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cpp/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      527 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cpp/_ewriter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.371337 myokit-1.34.0/myokit/formats/cuda/
+-rw-r--r--   0 michael   (1000) michael   (1000)      922 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cuda/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4603 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/cuda/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2165 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/cuda/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.371337 myokit-1.34.0/myokit/formats/cuda/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8863 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/formats/cuda/template/kernel.cu
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.372337 myokit-1.34.0/myokit/formats/easyml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      942 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/easyml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3811 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/easyml/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15877 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/easyml/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.372337 myokit-1.34.0/myokit/formats/html/
+-rw-r--r--   0 michael   (1000) michael   (1000)      563 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/html/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2449 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/html/_exporter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7184 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/html/_flatten.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.372337 myokit-1.34.0/myokit/formats/latex/
+-rw-r--r--   0 michael   (1000) michael   (1000)      788 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/latex/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6823 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/latex/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5259 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/latex/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.372337 myokit-1.34.0/myokit/formats/mathml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      743 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/mathml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    12444 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/mathml/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    34419 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/formats/mathml/_parser.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.373337 myokit-1.34.0/myokit/formats/matlab/
+-rw-r--r--   0 michael   (1000) michael   (1000)      801 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/matlab/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3306 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/matlab/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2974 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/formats/matlab/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.373337 myokit-1.34.0/myokit/formats/matlab/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)      528 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/matlab/template/constants.m
+-rw-r--r--   0 michael   (1000) michael   (1000)      374 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/matlab/template/ifthenelse.m
+-rw-r--r--   0 michael   (1000) michael   (1000)     2095 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/matlab/template/main.m
+-rw-r--r--   0 michael   (1000) michael   (1000)      861 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/matlab/template/model.m
+-rw-r--r--   0 michael   (1000) michael   (1000)      461 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/matlab/template/model_wrapper.m
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.373337 myokit-1.34.0/myokit/formats/opencl/
+-rw-r--r--   0 michael   (1000) michael   (1000)     7068 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/opencl/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5394 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/opencl/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4009 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/opencl/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.374337 myokit-1.34.0/myokit/formats/opencl/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11633 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/opencl/template/cable.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     8158 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/formats/opencl/template/kernel.cl
+-rw-r--r--   0 michael   (1000) michael   (1000)     9018 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/opencl/template/minilog.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1042 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/formats/opencl/template/plot.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      162 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/opencl/template/test.sh
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.374337 myokit-1.34.0/myokit/formats/python/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1155 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/python/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6912 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/python/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1075 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/python/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.374337 myokit-1.34.0/myokit/formats/python/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)    10489 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/python/template/sim.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.375337 myokit-1.34.0/myokit/formats/sbml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      759 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/sbml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    59422 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/formats/sbml/_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1111 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/sbml/_importer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29317 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/sbml/_parser.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.375337 myokit-1.34.0/myokit/formats/stan/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2983 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/stan/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3233 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/stan/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3869 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/stan/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.375337 myokit-1.34.0/myokit/formats/stan/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5305 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/formats/stan/template/cell.stan
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       92 2023-02-05 15:45:10.000000 myokit-1.34.0/myokit/formats/stan/template/run.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.376337 myokit-1.34.0/myokit/formats/sympy/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1744 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/sympy/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6872 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/sympy/_ereader.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5008 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/formats/sympy/_ewriter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.376337 myokit-1.34.0/myokit/formats/wcp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      360 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/wcp/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10510 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/formats/wcp/_wcp.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.376337 myokit-1.34.0/myokit/formats/xml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      551 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/xml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1600 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/xml/_exporter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      499 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/formats/xml/_split.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.377337 myokit-1.34.0/myokit/gui/
+-rw-r--r--   0 michael   (1000) michael   (1000)    12173 2023-06-07 22:09:50.000000 myokit-1.34.0/myokit/gui/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    46626 2023-06-07 22:09:50.000000 myokit-1.34.0/myokit/gui/datablock_viewer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    32941 2023-06-07 22:09:50.000000 myokit-1.34.0/myokit/gui/datalog_viewer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8607 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/gui/explorer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)   108635 2023-06-07 22:09:55.000000 myokit-1.34.0/myokit/gui/ide.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2174 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/gui/progress.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    50887 2023-06-07 22:09:50.000000 myokit-1.34.0/myokit/gui/source.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6270 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/gui/vargrapher.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.378337 myokit-1.34.0/myokit/lib/
+-rw-r--r--   0 michael   (1000) michael   (1000)      216 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/lib/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    24002 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/lib/deps.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    28160 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/lib/guess.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    46838 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/lib/hh.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    67969 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/lib/markov.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4513 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/lib/multi.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    13979 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/lib/plots.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4658 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/pacing.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8504 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/pype.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.385337 myokit-1.34.0/myokit/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)     7898 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2830 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/ansic_event_based_pacing.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1376 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/ansic_fixed_form_pacing.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.387337 myokit-1.34.0/myokit/tests/data/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3022 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/data/beeler-1977-model-compare-a.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2889 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/data/beeler-1977-model-compare-b.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3137 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/data/beeler-1977-model.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/beeler-1977-protocol.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/beeler-1977-script.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3287 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/data/beeler-1977-units.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     5091 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/data/clancy-1999-fitting.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3128 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/conditional.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     6067 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/data/cv1d.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/cv1d.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)    23916 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/decker-2009.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)    18350 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/decker.model
+-rw-r--r--   0 michael   (1000) michael   (1000)    10416 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/dn-1985-normalised.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      800 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/dom-markov.mmt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.388337 myokit-1.34.0/myokit/tests/data/formats/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8192 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/abf-protocol.pro
+-rw-r--r--   0 michael   (1000) michael   (1000)    98376 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/abf-v1.abf
+-rw-r--r--   0 michael   (1000) michael   (1000)    24576 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/abf-v2.abf
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.389337 myokit-1.34.0/myokit/tests/data/formats/cellml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)    59093 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/br-1977-dot.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)    58593 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/br-1977.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)   117223 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/corrias.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)   221953 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/decker-2009.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1595 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/documentation.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/invalid-file.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)    44837 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)    44947 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.391337 myokit-1.34.0/myokit/tests/data/formats/channelml/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2648 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      557 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2702 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2369 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1258 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1539 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1290 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1289 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1374 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1373 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      675 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1398 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1317 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.391337 myokit-1.34.0/myokit/tests/data/formats/sbml/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8719 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)     9801 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)    31408 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/HodgkinHuxley.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/LICENSE
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.391337 myokit-1.34.0/myokit/tests/data/formats/sbml/model/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2149 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2952 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1226 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.391337 myokit-1.34.0/myokit/tests/data/formats/sbml/result/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2457 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/result/00001-results.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)     2206 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/result/00004-results.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)     1131 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/sbml/result/01103-results.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)    25600 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/formats/wcp-file.wcp
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.396337 myokit-1.34.0/myokit/tests/data/io/
+-rw-r--r--   0 michael   (1000) michael   (1000)      735 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad1d-1-not-enough-files.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   109429 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad1d-2-no-header.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   104768 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad1d-3-no-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad1d-4-not-a-zip.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   109458 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad1d-5-bad-data-type.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1549 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad1d-6-time-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1584 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad1d-7-0d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad1d-8-1d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)      739 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad2d-1-not-enough-files.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   346240 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad2d-2-no-header.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   333091 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad2d-3-no-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad2d-4-not-a-zip.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   346257 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad2d-5-bad-data-type.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1553 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad2d-6-time-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1588 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad2d-7-0d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/bad2d-8-2d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)      623 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/badlog-1-no-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1281 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/badlog-2-no-structure.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/badlog-3-not-a-zip.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/badlog-4-invalid-n-fields.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/badlog-5-invalid-data-size.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1457 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/badlog-6-bad-data-type.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/badlog-7-not-enough-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     6031 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/data/io/block2d.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/block2d.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-1-empty.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-10-just-spaces.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)        2 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-11-just-a-semicolon.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      104 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-12-bad-header.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-13-header-with-empty-1.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-14-header-with-empty-2.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-15-header-with-empty-3.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-16-wrong-columns-in-data.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-17-non-float-data.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      112 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-2-windows.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      103 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-3-old-mac.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-4-empty-lines.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-5-semicolons.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      119 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-6-open-string.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-7-empty-lines-2.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      100 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-8-unquoted-header.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      114 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog-9-double-quoted-header.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/datalog.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)     1421 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/io/goodlog.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     4992 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/lr-1991-dep.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2315 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/lr-1991-fitting.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4571 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/lr-1991-testing.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     6124 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/lr-1991.mmt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.397337 myokit-1.34.0/myokit/tests/data/multi/
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/multi/beeler-1977-protocol.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/multi/beeler-1977-script.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/multi/beeler-no-name.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     6013 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/multi/lr-1991.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/multi/not-a-model.csv
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.397337 myokit-1.34.0/myokit/tests/data/multi/subdir/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/multi/subdir/beeler-no-name.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3754 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/data/noble-1962.mmt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    22939 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_aux.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    57389 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_cellml_v1_api.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    42270 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_cellml_v1_parser.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    12819 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_cellml_v1_writer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    73727 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_cellml_v2_api.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    26746 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_cellml_v2_parser.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    11264 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_cellml_v2_writer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4345 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_cmodel.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      704 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/test_compiler_detection.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    14384 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_component.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    12599 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_config.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    50041 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_datablock.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    83227 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_datalog.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    61106 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_dependency_checking.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)   138795 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_expressions.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5053 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_float.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4523 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    15162 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_axon.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    19483 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_cellml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     7137 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_channelml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    11791 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_easyml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     9610 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_exporters.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    41242 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_expression_writers.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3645 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/test_formats_html.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1972 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_importers.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    37731 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_mathml_content.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     9013 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_mathml_presentation.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    17615 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/test_formats_opencl.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5106 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_sbml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10611 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_sympy.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1891 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_formats_wcp.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    14562 2023-06-07 18:58:09.000000 myokit-1.34.0/myokit/tests/test_io.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2107 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_jacobian_calculator.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2054 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_jacobian_tracer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     7763 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/test_lib_deps.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    42620 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_lib_guess.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    31300 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_lib_hh.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    40269 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_lib_markov.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5432 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_lib_multi.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     6168 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/tests/test_lib_plots.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2935 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_meta.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    85260 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/tests/test_model.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    17109 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/tests/test_model_building.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4068 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_opencl_info.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8299 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_pacing_factory.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5448 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_pacing_system_c.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3235 2023-06-07 13:48:23.000000 myokit-1.34.0/myokit/tests/test_pacing_system_py.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    51305 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/tests/test_parsing.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2868 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_progress_reporters.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    15379 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_protocol.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    12852 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/tests/test_protocol_floating_point.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2606 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_protocol_time_series.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2689 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_pype.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     7640 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_quantity.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3738 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_rhs_benchmarker.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    72067 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/tests/test_sbml_api.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    54976 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/tests/test_sbml_parser.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    18000 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_simulation_1d.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    42412 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_simulation_cvodes.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1959 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_simulation_cvodes_from_disk.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    35708 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_simulation_fiber_tissue.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    14320 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_simulation_log_interval.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    59482 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/tests/test_simulation_opencl.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3110 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_simulation_opencl_log_interval.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    20401 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_simulation_opencl_vs_cvode.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5503 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_simulation_opencl_vs_sim1d.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      790 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_system_info.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10578 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_tools.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    13922 2023-06-07 18:43:10.000000 myokit-1.34.0/myokit/tests/test_unit.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2009 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tests/test_user_functions.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    33619 2023-06-07 17:18:23.000000 myokit-1.34.0/myokit/tests/test_variable.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    17487 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/tools.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8609 2023-06-07 13:48:59.000000 myokit-1.34.0/myokit/units.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 22:21:18.362337 myokit-1.34.0/myokit.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5086 2023-06-07 22:21:17.000000 myokit-1.34.0/myokit.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)    15047 2023-06-07 22:21:18.000000 myokit-1.34.0/myokit.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-06-07 22:21:17.000000 myokit-1.34.0/myokit.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       48 2023-06-07 22:21:18.000000 myokit-1.34.0/myokit.egg-info/entry_points.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-01-04 14:18:38.000000 myokit-1.34.0/myokit.egg-info/not-zip-safe
+-rw-rw-r--   0 michael   (1000) michael   (1000)      182 2023-06-07 22:21:18.000000 myokit-1.34.0/myokit.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        7 2023-06-07 22:21:18.000000 myokit-1.34.0/myokit.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-06-07 22:21:18.397337 myokit-1.34.0/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     3290 2023-06-07 22:09:50.000000 myokit-1.34.0/setup.py
```

### Comparing `myokit-1.33.9/LICENSE.txt` & `myokit-1.34.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/PKG-INFO` & `myokit-1.34.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: myokit
-Version: 1.33.9
+Version: 1.34.0
 Summary: A simple interface to cardiac cellular electrophysiology
 Home-page: http://myokit.org
 Author: Michael Clerx
 Author-email: michael@myokit.org
 License: BSD 3-clause license
 Project-URL: Bug Tracker, https://github.com/MichaelClerx/myokit/issues
 Project-URL: Documentation, http://docs.myokit.org
 Project-URL: Source Code, https://github.com/MichaelClerx/myokit
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
@@ -27,18 +26,18 @@
 Provides-Extra: dev
 Provides-Extra: optional
 Provides-Extra: gui
 Provides-Extra: pyqt
 Provides-Extra: pyside
 License-File: LICENSE.txt
 
-[![Ubuntu unit tests](https://github.com/MichaelClerx/myokit/workflows/Ubuntu%20unit%20tests/badge.svg)](https://github.com/MichaelClerx/myokit/actions?query=workflow%3A"Ubuntu+unit+tests")
-[![MacOS unit tests](https://github.com/MichaelClerx/myokit/workflows/MacOS%20unit%20tests/badge.svg)](https://github.com/MichaelClerx/myokit/actions?query=workflow%3A"MacOS+unit+tests")
-[![Windows unit tests](https://github.com/MichaelClerx/myokit/workflows/Windows%20unit%20tests/badge.svg)](https://github.com/MichaelClerx/myokit/actions?query=workflow%3A"Windows+unit+tests")
-[![Windows Miniconda test](https://github.com/MichaelClerx/myokit/workflows/Windows%20Miniconda%20test/badge.svg)](https://github.com/MichaelClerx/myokit/actions?query=workflow%3A"Windows+Miniconda+test")
+[![Ubuntu unit tests](https://github.com/myokit/myokit/actions/workflows/unit-tests-ubuntu.yml/badge.svg)](https://github.com/myokit/myokit/actions/workflows/unit-tests-ubuntu.yml)
+[![MacOS unit tests](https://github.com/myokit/myokit/actions/workflows/unit-tests-macos.yml/badge.svg)](https://github.com/myokit/myokit/actions/workflows/unit-tests-macos.yml)
+[![Windows unit tests](https://github.com/myokit/myokit/actions/workflows/unit-tests-windows.yml/badge.svg)](https://github.com/myokit/myokit/actions/workflows/unit-tests-windows.yml)
+[![Windows Miniconda test](https://github.com/myokit/myokit/actions/workflows/unit-tests-windows-miniconda.yml/badge.svg)](https://github.com/myokit/myokit/actions/workflows/unit-tests-windows-miniconda.yml)
 [![codecov](https://codecov.io/gh/myokit/myokit/branch/main/graph/badge.svg)](https://codecov.io/gh/myokit/myokit)
 [![Documentation Status](https://readthedocs.org/projects/myokit/badge/?version=latest)](https://myokit.readthedocs.io/?badge=latest)
 
 ![Myokit](http://myokit.org/static/img/logo.png)
 
 [Myokit](http://myokit.org) is an [open-source](https://github.com/MichaelClerx/myokit/blob/main/LICENSE.txt) Python-based toolkit that facilitates modeling and simulation of cardiac cellular electrophysiology.
 It's hosted on [GitHub](https://github.com/MichaelClerx/myokit/) and available on [PyPi](https://pypi.org/project/myokit/).
@@ -103,9 +102,7 @@
 
 
 ## Citing Myokit
 
 If you use Myokit in your research, please cite it using the information in our [CITATION file](https://github.com/MichaelClerx/myokit/blob/main/CITATION).
 
 I like to [keep track of who's using Myokit](http://myokit.org/publications/) (for my CV!). If you are using Myokit for teaching, I'd love to hear about it. You can drop me a line at michael[at]myokit.org.
-
-
```

### Comparing `myokit-1.33.9/README.md` & `myokit-1.34.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-[![Ubuntu unit tests](https://github.com/MichaelClerx/myokit/workflows/Ubuntu%20unit%20tests/badge.svg)](https://github.com/MichaelClerx/myokit/actions?query=workflow%3A"Ubuntu+unit+tests")
-[![MacOS unit tests](https://github.com/MichaelClerx/myokit/workflows/MacOS%20unit%20tests/badge.svg)](https://github.com/MichaelClerx/myokit/actions?query=workflow%3A"MacOS+unit+tests")
-[![Windows unit tests](https://github.com/MichaelClerx/myokit/workflows/Windows%20unit%20tests/badge.svg)](https://github.com/MichaelClerx/myokit/actions?query=workflow%3A"Windows+unit+tests")
-[![Windows Miniconda test](https://github.com/MichaelClerx/myokit/workflows/Windows%20Miniconda%20test/badge.svg)](https://github.com/MichaelClerx/myokit/actions?query=workflow%3A"Windows+Miniconda+test")
+[![Ubuntu unit tests](https://github.com/myokit/myokit/actions/workflows/unit-tests-ubuntu.yml/badge.svg)](https://github.com/myokit/myokit/actions/workflows/unit-tests-ubuntu.yml)
+[![MacOS unit tests](https://github.com/myokit/myokit/actions/workflows/unit-tests-macos.yml/badge.svg)](https://github.com/myokit/myokit/actions/workflows/unit-tests-macos.yml)
+[![Windows unit tests](https://github.com/myokit/myokit/actions/workflows/unit-tests-windows.yml/badge.svg)](https://github.com/myokit/myokit/actions/workflows/unit-tests-windows.yml)
+[![Windows Miniconda test](https://github.com/myokit/myokit/actions/workflows/unit-tests-windows-miniconda.yml/badge.svg)](https://github.com/myokit/myokit/actions/workflows/unit-tests-windows-miniconda.yml)
 [![codecov](https://codecov.io/gh/myokit/myokit/branch/main/graph/badge.svg)](https://codecov.io/gh/myokit/myokit)
 [![Documentation Status](https://readthedocs.org/projects/myokit/badge/?version=latest)](https://myokit.readthedocs.io/?badge=latest)
 
 ![Myokit](http://myokit.org/static/img/logo.png)
 
 [Myokit](http://myokit.org) is an [open-source](https://github.com/MichaelClerx/myokit/blob/main/LICENSE.txt) Python-based toolkit that facilitates modeling and simulation of cardiac cellular electrophysiology.
 It's hosted on [GitHub](https://github.com/MichaelClerx/myokit/) and available on [PyPi](https://pypi.org/project/myokit/).
```

### Comparing `myokit-1.33.9/myokit/__init__.py` & `myokit-1.34.0/myokit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,22 +28,14 @@
 # will generate an error.
 #
 from __future__ import absolute_import, division
 from __future__ import print_function, unicode_literals
 
 
 #
-# Configure logging
-#
-import logging  # noqa  (not at top of file)
-logging.basicConfig()
-del logging
-
-
-#
 # Check python version
 #
 # Hexversion guide:
 #  0x   Hex
 #  02   PY_MAJOR_VERSION
 #  07   PY_MINOR_VERSION
 #  0F   PY_MICRO_VERSION, in hex, so 0F is 15, 10 is 16, etc.
@@ -291,15 +283,15 @@
 #
 # Date and time formats to use throughout Myokit
 #
 DATE_FORMAT = '%Y-%m-%d %H:%M:%S'
 TIME_FORMAT = '%H:%M:%S'
 
 #
-# GUI: Favour PySide or PyQt
+# GUI: Favor PySide or PyQt
 #
 FORCE_PYQT5 = False
 FORCE_PYQT4 = False
 FORCE_PYSIDE = False
 FORCE_PYSIDE2 = False
 
 
@@ -337,28 +329,28 @@
     DuplicateFunctionName,
     DuplicateName,
     ExportError,
     FindNanError,
     GenerationError,
     IllegalAliasError,
     IllegalReferenceError,
+    IllegalReferenceInInitialValueError,
     ImportError,
     IncompatibleModelError,
     IncompatibleUnitError,
     IntegrityError,
     InvalidBindingError,
     InvalidDataLogError,
     InvalidFunction,
     InvalidLabelError,
     InvalidMetaDataNameError,
     InvalidNameError,
     MissingRhsError,
     MissingTimeVariableError,
     MyokitError,
-    NonLiteralValueError,
     NumericalError,
     ParseError,
     ProtocolEventError,
     ProtocolParseError,
     SectionNotFoundError,
     SimulationCancelledError,
     SimulationError,
@@ -458,14 +450,15 @@
 )
 
 # Pacing protocol
 from ._protocol import (  # noqa
     PacingSystem,
     Protocol,
     ProtocolEvent,
+    TimeSeriesProtocol,
 )
 from . import pacing  # noqa
 
 # Parser functions
 from ._parsing import (  # noqa
     format_parse_error,
     KEYWORDS,
@@ -501,14 +494,15 @@
 
 # Auxillary functions
 from ._aux import (  # noqa
     default_protocol,
     default_script,
     ModelComparison,
     numpy_writer,
+    _prepare_bindings,
     python_writer,
     run,
     step,
     version,
     # Deprecated and/or moved to myokit.tools
     Benchmarker,
     date,
@@ -560,19 +554,16 @@
     OpenCL,
     OpenCLDeviceInfo,
     OpenCLInfo,
     OpenCLPlatformInfo,
 )
 from ._sim.cmodel import CModel             # noqa
 from ._sim.cvodessim import Simulation      # noqa
-from ._sim.cvodesim import Simulation as LegacySimulation  # noqa
 from ._sim.cable import Simulation1d        # noqa
 from ._sim.rhs import RhsBenchmarker        # noqa
-from ._sim.icsim import ICSimulation        # noqa
-from ._sim.psim import PSimulation          # noqa
 from ._sim.jacobian import JacobianTracer, JacobianCalculator   # noqa
 from ._sim.openclsim import SimulationOpenCL                    # noqa
 from ._sim.fiber_tissue import FiberTissueSimulation            # noqa
 
 
 #
 # Globally shared progress reporter
```

### Comparing `myokit-1.33.9/myokit/__main__.py` & `myokit-1.34.0/myokit/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
 
 #
 # Debug
 #
 
 def debug(source, variable, deps=False):
     """
-    Shows how a single variable is calculated from the initial conditions.
+    Shows how a single variable is calculated from the initial values.
     """
     import myokit
 
     # Load model
     m = myokit.load_model(source)
 
     # Show result
@@ -257,16 +257,16 @@
 def add_debug_parser(subparsers):
     """
     Adds a subcommand parser for the ``debug`` command.
     """
     parser = subparsers.add_parser(
         'debug',
         description='Shows how a single variable is calculated from the '
-                    'initial conditions. The variable\'s equation and value'
-                    ' are displayed, along with the value and formula of any'
+                    ' initial values. The variable\'s equation and value are'
+                    ' displayed, along with the value and formula of any'
                     ' nested variables and the values of all dependencies.',
         help='Shows how a single variable is calculated.',
     )
     parser.add_argument(
         'source',
         metavar='source_file.mmt',
         help='The source file to parse.',
@@ -1286,19 +1286,14 @@
     doc_parser.set_defaults(testfunc=test_documentation)
 
     # Example notebooks
     example_parser = subparsers.add_parser(
         'examples', help='Test example notebooks.')
     example_parser.set_defaults(testfunc=test_examples)
 
-    # Publication examples
-    pub_parser = subparsers.add_parser(
-        'pub', help='Run publication examples.')
-    pub_parser.set_defaults(testfunc=test_examples_pub)
-
     # Style tests
     style_parser = subparsers.add_parser('style', help='Run code style tests.')
     style_parser.set_defaults(testfunc=test_style)
 
     # Unit tests
     unit_parser = subparsers.add_parser('unit', help='Run unit tests')
     unit_parser.set_defaults(testfunc=test_unit)
@@ -1836,31 +1831,14 @@
         for book in failed:
             print('  ' + str(book))
         sys.exit(1)
     else:
         print('ok: Successfully ran all (' + str(len(books)) + ') notebooks.')
 
 
-def test_examples_pub(args):
-    """
-    Runs all publication examples, exits if one of them fails.
-    """
-    import os
-    import sys
-    import myokit
-
-    # Get publications directory
-    path = os.path.join(myokit.DIR_MYOKIT, 'tests', 'publications')
-
-    # PBMB 2016. Myokit: A simple interface to cardiac cellular
-    # electrophysiology
-    if test_mmt_files(os.path.join(path, 'pbmb-2016')):
-        sys.exit(1)
-
-
 def test_examples_web(args):
     """
     Runs all web examples, exits if one of them fails.
     """
     import os
     import sys
     import myokit
@@ -2205,8 +2183,11 @@
         default='traditional',
         choices=myokit.ColorMap.names(),
     )
     parser.set_defaults(func=video)
 
 
 if __name__ == '__main__':
+    import logging
+    logging.basicConfig()
+
     main()
```

### Comparing `myokit-1.33.9/myokit/_aux.py` & `myokit-1.34.0/myokit/_aux.py`

 * *Files 3% similar despite different names*

```diff
@@ -277,32 +277,32 @@
             if key not in seen:
                 self._write(
                     '[1] Missing Meta property' + name + ': "' + str(key)
                     + '"')
 
     def _state(self, m1, m2):
         """
-        Compares two models' states.
+        Compares two models' states and initial values.
         """
         s1 = iter([v.qname() for v in m1.states()])
         s2 = iter([v.qname() for v in m2.states()])
-        c1 = m1.state()
-        c2 = m2.state()
+        c1 = m1.initial_values()
+        c2 = m2.initial_values()
         for k, v1 in enumerate(s1):
             try:
                 v2 = next(s2)
             except StopIteration:
                 self._write('[2] Missing state at position ' + str(k))
                 continue
             if v1 != v2:
                 self._write(
                     '[x] Mismatched State at position ' + str(k) + ': [1]<'
                     + v1 + '> [2]<' + v2 + '>')
                 continue
-            if c1[k] != c2[k]:
+            if c1[k].code() != c2[k].code():
                 self._write('[x] Mismatched Initial value for <' + v1 + '>')
         n = m2.count_states()
         for k, v2 in enumerate(s2):
             self._write('[1] Missing state at position ' + str(n + k))
 
     def text(self):
         """
@@ -430,14 +430,58 @@
             return '_d_' + u if x.is_derivative() else u
 
         _pywriter_.set_lhs_function(name)
 
     return _pywriter_
 
 
+def _prepare_bindings(model, labels):
+    """
+    Takes a mapping of binding labels to internal references and returns a map
+    from variable instances to the same internal references.
+
+    This method also modifies ``model``: All bindings that are not mapped to
+    an internal reference will be removed.
+
+    The argument ``mapping`` should take the form::
+
+        labels = {
+            binding_label_1 : internal_name_1,
+            binding_label_2 : internal_name_2,
+            ...
+            }
+
+    The returned dictionary will have the form::
+
+        variables = {
+            variable_x : internal_name_1,
+            variable_y : internal_name_2,
+            ...
+            }
+
+    Unsupported bindings (i.e. bindings not appearing in ``labels``) will
+    be ignored.
+    """
+    unused = []
+    variables = {}
+    for label, var in model.bindings():
+        try:
+            variables[var] = labels[label]
+        except KeyError:
+            unused.append(var)
+            continue
+        # TODO: Remove this line; https://github.com/myokit/myokit/issues/320
+        var.set_rhs(0)
+
+    for var in unused:
+        var.set_binding(None)
+
+    return variables
+
+
 def run(model, protocol, script, stdout=None, stderr=None, progress=None):
     """
     Runs a python ``script`` using the given ``model`` and ``protocol``.
 
     The following functions are provided to the script:
 
     ``get_model()``
@@ -545,15 +589,15 @@
     (divide-by-zeros, invalid operations and overflows). To run an evaluation
     without error checking, set ``ignore_errors=True``.
 
     Returns a string indicating the results.
     """
     # Get initial state
     if initial is None:
-        initial = model.state()
+        initial = model.initial_values(as_floats=True)
 
     # Get evaluation at initial state
     values = model.evaluate_derivatives(
         state=initial, ignore_errors=ignore_errors)
 
     # Log settings
     fmat = myokit.SFDOUBLE
@@ -616,16 +660,21 @@
                 errors += 1
                 log.append(line + ' exponent')
                 log.append(i + '^^^^')
 
             # Large error, small error, or no error
             else:
                 mark_error = False
-                threshold = 13
-                if xx[:threshold] != yy[:threshold]:
+                abs_err = abs(x - y)
+                if abs_err:
+                    rel_err = abs(x - y) / max(abs(x), abs(y))
+                    n_eps = rel_err / sys.float_info.epsilon
+                else:
+                    n_eps = rel_err = 0
+                if n_eps > 1e6:
                     # "Large" error
                     errors += 1
                     line += ' X'
                     mark_error = True
                 elif xx != yy:
                     # "Small" error, or numerical error
                     rel_err = abs(x - y) / max(abs(x), abs(y))
@@ -660,15 +709,15 @@
         else:
             log.append('Model check completed without errors.')
 
         # Show small mismatches between model and reference
         if warnings > 0:
             log.append('Found (' + str(warnings) + ') small mismatches.')
 
-    # Finalise and return
+    # Finalize and return
     log.append('-' * line_width)
     return '\n'.join(log)
 
 
 def strfloat(number, full=False, precision=myokit.DOUBLE_PRECISION):
     """Deprecated alias of :class:`myokit.float.str`."""
     # Deprecated since 2021-03-24
```

### Comparing `myokit-1.33.9/myokit/_bin/example.mmt` & `myokit-1.34.0/myokit/_bin/example.mmt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [[model]]
 name: Luo-Rudy 1991
 desc: """
 Implementation of the Luo-Rudy model I for the ventricular myocyte.
 Based on an updated formulation downloaded from http://rudylab.wustl.edu
-and licensed under a GNU GPL license version 2.
 """
 # Initial conditions
 membrane.V = -84.5286
 ina.m      = 0.0017
 ina.h      = 0.9832
 ina.j      = 0.995484
 ica.d      = 0.000003
@@ -15,15 +14,15 @@
 ik.x       = 0.0057
 ica.Ca_i   = 0.0002
 
 [membrane]
 desc: """
 Membrane potential and stimulus
 """
-C = 1.0 [uF/cm^2]
+C = 1 [uF/cm^2]
     in [uF/cm^2]
 dot(V) = - (1/C) * (i_ion + i_diff + i_stim) in [mV]
     label membrane_potential
     desc: The membrane potential
 i_ion = ina.INa + ik.IK + ib.Ib + ikp.IKp + ik1.IK1 + ica.ICa
     in [uA/cm^2]
     label cellular_current
```

### Comparing `myokit-1.33.9/myokit/_bin/gui/find.png` & `myokit-1.34.0/myokit/_bin/gui/find.png`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer-128.xpm` & `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-128.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer-16.xpm` & `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-16.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer-24.xpm` & `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-24.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer-256.xpm` & `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-256.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer-32.xpm` & `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-32.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer-48.xpm` & `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-48.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer-64.xpm` & `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-64.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer-96.xpm` & `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer-96.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer.ico` & `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer.ico`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-datablock-viewer.png` & `myokit-1.34.0/myokit/_bin/gui/icon-datablock-viewer.png`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-ide-128.xpm` & `myokit-1.34.0/myokit/_bin/gui/icon-ide-128.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-ide-16.xpm` & `myokit-1.34.0/myokit/_bin/gui/icon-ide-16.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-ide-24.xpm` & `myokit-1.34.0/myokit/_bin/gui/icon-ide-24.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-ide-256.xpm` & `myokit-1.34.0/myokit/_bin/gui/icon-ide-256.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-ide-32.xpm` & `myokit-1.34.0/myokit/_bin/gui/icon-ide-32.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-ide-48.xpm` & `myokit-1.34.0/myokit/_bin/gui/icon-ide-48.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-ide-64.xpm` & `myokit-1.34.0/myokit/_bin/gui/icon-ide-64.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-ide-96.xpm` & `myokit-1.34.0/myokit/_bin/gui/icon-ide-96.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-ide.ico` & `myokit-1.34.0/myokit/_bin/gui/icon-ide.ico`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/icon-ide.png` & `myokit-1.34.0/myokit/_bin/gui/icon-ide.png`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/new.png` & `myokit-1.34.0/myokit/_bin/gui/new.png`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/open.png` & `myokit-1.34.0/myokit/_bin/gui/open.png`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/gui/save.png` & `myokit-1.34.0/myokit/_bin/gui/save.png`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/install-lin/myokit.lang` & `myokit-1.34.0/myokit/_bin/install-lin/myokit.lang`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/install-win/menu.json` & `myokit-1.34.0/myokit/_bin/install-win/menu.json`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 icons = icons.replace('\\', '/')
 ?>
 {
     "menu_name": "Myokit",
     "menu_items":
         [
             {
-                "name": "Myokit IDE",
-                "script": "${PYTHON_SCRIPTS}/myokit.exe",
-                "scriptarguments": ["ide"],
-                "workdir": "${PREFIX}",
-                "icon": "<?=icons?>/icon-ide.ico"
-            },
-            {
                 "name": "DataLog viewer",
                 "script": "${PYTHON_SCRIPTS}/myokit.exe",
                 "scriptarguments": ["log"],
                 "workdir": "${PREFIX}",
                 "icon": "<?=icons?>/icon-ide.ico"
             },
             {
                 "name": "DataBlock viewer",
                 "script": "${PYTHON_SCRIPTS}/myokit.exe",
                 "scriptarguments": ["block"],
                 "workdir": "${PREFIX}",
                 "icon": "<?=icons?>/icon-datablock-viewer.ico"
+            },
+            {
+                "name": "Myokit IDE",
+                "script": "${PYTHON_SCRIPTS}/myokit.exe",
+                "scriptarguments": ["ide"],
+                "workdir": "${PREFIX}",
+                "icon": "<?=icons?>/icon-ide.ico"
             }
         ]
 }
```

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/LICENSE` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/LICENSE`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib` & `myokit-1.34.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_config.py` & `myokit-1.34.0/myokit/_config.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_datablock.py` & `myokit-1.34.0/myokit/_datablock.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,16 +183,16 @@
                 raise ValueError('The argument `border` cannot be negative.')
             elif border >= self._nx // 2:
                 raise ValueError(
                     'The argument `border` must be less than half the number'
                     ' of cells.')
 
         # Get indices of selected cells
-        ilo = border                # First indice
-        ihi = self._nx - border     # Last indice + 1
+        ilo = border                # First index
+        ihi = self._nx - border     # Last index + 1
 
         # Indices of cells with AP
         i1 = None
         i2 = None
 
         # Get Vm, reshaped to get each cell's time-series successively.
         v_series = self._1d[name].reshape(self._nt * self._nx, order='F')
@@ -201,16 +201,16 @@
         v_series = np.split(v_series, self._nx)
 
         # Find first activation time
         have_crossing = False
         t = []
         for i in range(ilo, ihi):
             v = v_series[i]
-            # Get indice of first threshold crossing with positive flank
-            # Don't include crossings at log indice 0
+            # Get index of first threshold crossing with positive flank
+            # Don't include crossings at log index 0
             itime = np.where((v[1:] > -30) & (v[1:] - v[:-1] > 0))[0]
             if len(itime) == 0 or itime[0] == 0:
                 # No crossing found
                 if have_crossing:
                     # CV calculation ends here
                     i2 = i - 1
                     break
```

### Comparing `myokit-1.33.9/myokit/_datalog.py` & `myokit-1.34.0/myokit/_datalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,19 +91,18 @@
     Arguments:
 
     ``other``
         A DataLog to clone or a dictionary to use as basis.
     ``time``
         The log key to use for the time variable. When cloning a log, adding
         the ``time`` argument will overwrite the cloned value.
+
     """
+
     def __init__(self, other=None, time=None):
-        """
-        Creates a new DataLog.
-        """
         if other is None:
             # Create new
             super(DataLog, self).__init__()
             self._time = None
         else:
             # Clone
             super(DataLog, self).__init__(other)
@@ -115,29 +114,25 @@
             self.set_time_key(time)
 
     def apd(self, v='membrane.V', threshold=-70):
         """
         Calculates one or more Action Potential Durations (APDs) in a single
         cell's membrane potential.
 
-        *Note 1: More accuracte apd measurements can be created using the*
+        *Note 1: More accuracte APD measurements can be obtained using the*
         :class:`Simulation` *object's APD tracking functionality. See*
         :meth:`Simulation.run()` *for details.*
 
         *Note 2: This APD is defined by simply checking crossing of a threshold
         potential, and does not look at lowest or highest voltages in a
         signal.*
 
         The membrane potential data should be listed in the log under the key
         given by ``v``.
 
-        The APD is measured as the time that the membrane potential exceeds a
-        certain, fixed, threshold. It does *not* calculate dynamic thresholds
-        like "90% of max(V) - min(V)".
-
         The returned value is a list of tuples (AP_start, APD).
         """
         def crossings(x, y, t):
             """
             Calculates the ``x``-values where ``y`` crosses threshold ``t``.
             Returns a list of tuples ``(xc, sc)`` where ``xc`` is the ``x``
             coordinate of the crossing and ``sc`` is the slope at this point.
@@ -236,26 +231,29 @@
         if other._time != self._time:
             raise ValueError('Both logs must have the same time key.')
         if other[self._time][0] < self[self._time][-1]:
             raise ValueError(
                 'Cannot extend DataLog with data from an earlier time.')
         if set(self.keys()) != set(other.keys()):
             raise ValueError('Both logs must have the same keys.')
+
         # Create new log
         log = DataLog()
         log._time = self._time
+
         # Add data
         for k, v1 in self.items():
             v2 = other[k]
             if isinstance(v1, np.ndarray) or isinstance(v2, np.ndarray):
                 # Concatenation copies data
                 log[k] = np.concatenate((np.asarray(v1), np.asarray(v2)))
             else:
                 log[k] = list(v1)   # Copies v1 data
                 log[k].extend(v2)   # Copies v2 data
+
         # Return
         return log
 
     def find(self, time):
         """
         Deprecated alias of :meth:`find_after()`.
         """
@@ -265,15 +263,15 @@
             'The method `find` is deprecated. Please use `find_after`'
             ' instead.')
 
         return self.find_after(time)
 
     def find_after(self, time):
         """
-        Returns the lowest indice ``i`` such that
+        Returns the lowest index ``i`` such that
 
             times[i] >= time
 
         where ``times`` are the times stored in this ``DataLog``.
 
         If no such value exists in the log, ``len(time)`` is returned.
         """
@@ -284,15 +282,15 @@
         if n == 0 or time <= times[0]:
             return 0
         if time > times[-1]:
             return n
 
         # Find t
         def find(lo, hi):
-            # lo = first indice, hi = last indice + 1
+            # lo = first index, hi = last index + 1
             if (lo + 1 == hi):
                 return lo + 1
             m = int((lo + hi) / 2)
             if time > times[m]:
                 return find(m, hi)
             else:
                 return find(lo, m)
@@ -438,29 +436,29 @@
                 log[k] = np.array(v[a:b], copy=True, dtype=float)
             else:
                 log[k] = v[a:b]
         return log
 
     def itrim_left(self, i):
         """
-        Returns a copy of this log, with all entries before indice ``i``
+        Returns a copy of this log, with all entries before index ``i``
         removed (similar to performing ``x = x[i:]`` on a list).
         """
         log = DataLog()
         log._time = self._time
         for k, v in self.items():
             if isinstance(v, np.ndarray):
                 log[k] = np.array(v[i:], copy=True, dtype=float)
             else:
                 log[k] = v[i:]
         return log
 
     def itrim_right(self, i):
         """
-        Returns a copy of this log, with all entries starting from indice ``i``
+        Returns a copy of this log, with all entries starting from index ``i``
         removed (similar to performing ``x = x[:i]`` on a list).
         """
         log = DataLog()
         log._time = self._time
         for k, v in self.items():
             if isinstance(v, np.ndarray):
                 log[k] = np.array(v[:i], copy=True, dtype=float)
@@ -824,19 +822,24 @@
                 parts = [str(x) for x in key[1]]
             else:
                 parts = [str(x) for x in key[1:]]
             parts.append(str(name))
             key = '.'.join(parts)
         return str(key)
 
-    def regularize(self, dt, tmin=None, tmax=None):
+    def regularize(self, dt, tmin=None, tmax=None):  # pragma: no cover
         """
         Returns a copy of this DataLog with data points at regularly spaced
         times.
 
+        This method is deprecated and will be removed in future versions of
+        Myokit.
+
+        This method requires ``SciPy`` to be installed.
+
         *Note: While regularize() can be used post-simulation to create fixed
         time-step data from variable time-step data, it is usually better to
         re-run a simulation with fixed time step logging. See*
         :meth:`Simulation.run()` *for details.*
 
         The first point will be at ``tmin`` if specified or otherwise the first
         time present in the log. All following points will be spaced ``dt``
@@ -852,34 +855,38 @@
              ``tmin`` and ``tmax`` will be included in the interpolated data
              set (so *only* if there are at least two values before ``tmin`` or
              two values after ``tmax`` in the data respectively).
           3. Evaluating the interpolant at the regularly spaced points.
 
         As a result of the cubic spline interpolation, the function may perform
         poorly on large data sets.
-
-        This method requires ``SciPy`` to be installed.
         """
-        self.validate()
+        # Deprecated since 2023-06-06
+        import warnings
+        warnings.warn(
+            'The method `regularize` is deprecated and will be removed in'
+            ' future versions of Myokit.')
+
         from scipy.interpolate import UnivariateSpline as Spline
+        self.validate()
 
         # Check time variable
         time = self.time()
         n = len(time)
 
-        # Get left indice for splines
+        # Get left index for splines
         imin = 0
         if tmin is None:
             tmin = time[0]
         elif tmin > time[0]:
             # Find position of tmin in time list, then add two points to the
             # left so that the spline has 4 points
             imin = max(0, np.searchsorted(time, tmin) - 2)
 
-        # Get right indice for splines
+        # Get right index for splines
         imax = n
         if tmax is None:
             tmax = time[-1]
         elif tmax < time[-1]:
             imax = min(n, np.searchsorted(time, tmax) + 2)
 
         # Get time steps
@@ -1125,15 +1132,15 @@
 
         The split log files can be returned as-is, or with the time variable's
         value adjusted so that all logs appear to cover the same span. To
         enable this option, set ``adjust`` to ``True``.
 
         By default, the returned intervals are *closed*, so both the left and
         right endpoint are included (if present in the data). This may involve
-        the duplication of some data points. To disable this behaviour and
+        the duplication of some data points. To disable this behavior and
         return half-closed endpoints (containing only the left point), set
         ``closed_intervals`` to ``False``.
         """
         # Validate log before starting
         self.validate()
 
         # Check time variable
```

### Comparing `myokit-1.33.9/myokit/_err.py` & `myokit-1.34.0/myokit/_err.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,16 +165,27 @@
     accessible from the owning variable ``owner``'s scope.
 
     *Extends:* :class:`myokit.IntegrityError`
     """
     def __init__(self, reference, owner):
         super(IllegalReferenceError, self).__init__(
             'Illegal reference: The referenced variable <' + reference.qname()
-            + '> is outside the scope of <' + owner.qname() + '>.'
-        )
+            + '> is outside the scope of <' + owner.qname() + '>.')
+
+
+class IllegalReferenceInInitialValueError(IllegalReferenceError):
+    """
+    Raised when an illegal reference is made in an initial value.
+
+    The only way this can occur is if the reference is to a nested variable.
+    """
+    def __init__(self, reference, owner):
+        super(IllegalReferenceError, self).__init__(
+            'Illegal reference made in initial value: The referenced variable'
+            ' <' + reference.qname() + '> is nested.')
 
 
 class ImportError(MyokitError):
     """
     Raised when an import from another format fails.
 
     *Extends:* :class:`myokit.MyokitError`.
@@ -288,22 +299,14 @@
     """
     def __init__(self):
         msg = 'No variable bound to time. At least one of the model\'s' \
               ' variables must be bound to "time".'
         super(MissingTimeVariableError, self).__init__(msg)
 
 
-class NonLiteralValueError(IntegrityError):
-    """
-    Raised when a literal value is required but not given.
-
-    *Extends:* :class:`myokit.IntegrityError`
-    """
-
-
 class NumericalError(MyokitError):
     """
     Raised when a numerical error occurs during the evaluation of a myokit
     :class:`Expression`.
 
     *Extends:* :class:`myokit.MyokitError`
     """
```

### Comparing `myokit-1.33.9/myokit/_expressions.py` & `myokit-1.34.0/myokit/_expressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -591,29 +591,31 @@
         :class:`myokit.Derivative` instance (and references the variable
         ``var``, if given).
         """
         return False
 
     def is_literal(self):
         """
-        Returns ``True`` if this expression doesn't contain any references.
+        Returns ``True`` if this expression does not contain any references.
         """
         return len(self._references) == 0
 
     def is_name(self, var=None):
         """
         Returns ``True`` only if this expression is a :class:`myokit.Name`
         (and references the variable ``var``, if given).
         """
         return False
 
     def is_number(self, value=None):
         """
-        Returns ``True`` only if this expression is a :class:`myokit.Number`
-        (and has the value ``value``, if given).
+        Returns ``True`` only if this expression is a :class:`myokit.Number`.
+
+        If the optional argument ``value`` is set, it will also return
+        ``False`` if the number does not have the given value.
         """
         return False
 
     def is_state_value(self):
         """
         Returns ``True`` if this expression is a :class:`Name` pointing to the
         current value of a state variable.
@@ -979,15 +981,15 @@
             raise EvalError(self, subst, e)
 
     def is_constant(self):
         """See :meth:`Expression.is_constant()`."""
         return self.var().is_constant()
 
     def is_literal(self):
-        """See :meth:`Expression.is_constant()`."""
+        """See :meth:`Expression.is_literal()`."""
         return False
 
     def rhs(self):
         """
         Returns the RHS expression equal to this LHS expression in the
         associated model.
         """
@@ -1138,15 +1140,15 @@
     def __repr__(self):
         return '<Name(' + repr(self._value) + ')>'
 
     def rhs(self):
         """See :meth:`LhsExpression.rhs()`."""
         if self._proper:
             if self._value.is_state():
-                return Number(self._value.state_value())
+                return self._value.initial_value()
             elif self._value.lhs() == self:
                 return self._value.rhs()
         return None
 
     def _tree_str(self, b, n):
         b.write(' ' * n + str(self._value) + '\n')
 
@@ -1386,15 +1388,15 @@
     def var(self):
         """
         See :meth:`LhsExpression.var()`.
 
         As with time-derivatives, this returns the variable of which a
         derivative is taken (i.e. the dependent variable "y" in "dy/dx").
         """
-        return self._var1._value
+        return self._var1.var()
 
 
 class InitialValue(LhsExpression):
     """
     Represents a reference to the initial value of a state variable.
 
     This class is used when writing out derivatives of equations, but may _not_
@@ -1406,15 +1408,15 @@
     _nargs = [1]    # Allows parsing as a function
     __hash__ = LhsExpression.__hash__   # For Python3, when __eq__ is present
 
     def __init__(self, var):
         super(InitialValue, self).__init__((var, ))
         if not isinstance(var, Name):
             raise IntegrityError(
-                'The first argument to an initial condition must be a variable'
+                'The first argument to an initial value must be a variable'
                 ' name.', self._token)
 
         self._var = var
         self._references = set([self])
         self._has_initials = True
 
     def bracket(self, op=None):
@@ -1432,15 +1434,15 @@
     def _code(self, b, c):
         b.write('init(')
         self._var._code(b, c)
         b.write(')')
 
     def _diff(self, lhs, idstates):
         raise NotImplementedError(
-            'Partial derivatives of initial conditions are not supported.')
+            'Partial derivatives of initial values are not supported.')
 
     def _eval_unit(self, mode):
         return self._var._eval_unit(mode)
 
     def _polishb(self, b):
         b.write('init ')
         self._var._polishb(b)
@@ -1449,15 +1451,15 @@
         return '<InitialValue(' + repr(self._var) + ')>'
 
     def rhs(self):
         """
         See :meth:`LhsExpression.rhs()`.
 
         The RHS returned in this case will be ``None``, as there is no RHS
-        associated with initial conditions in the model.
+        associated with initial values in the model.
         """
         # Note: This _could_ return a Number(init, var unit) instead...
         return None
 
     def _tree_str(self, b, n):
         b.write(' ' * n + 'init(' + str(self._var._value) + ')\n')
 
@@ -1467,15 +1469,15 @@
 
     def _validate(self, trail):
         super(InitialValue, self)._validate(trail)
         # Check if value is the name of a state variable
         var = self._var._value
         if not (isinstance(var, myokit.Variable) and var.is_state()):
             raise IntegrityError(
-                'Initial conditions can only be defined for state variables.',
+                'Initial values can only be defined for state variables.',
                 self._token)
 
 
 class PrefixExpression(Expression):
     """
     Base class for prefix expressions: expressions with a single operand.
 
@@ -1874,15 +1876,15 @@
         # whenever a = k*b (for an integer k). As a result, the derivatives
         # d/da(a//b) and d/db(a//b) are either zero (most of the time) or
         # undefined (at the jumps). Notably, outside of the jump points, the
         # line a//b is flat, so does not depend on a, b, a', or b'!
         #
         # Alternatively, a // b = floor(a / b).
         #
-        # Here we ignore the discontinuities in favour of a left or right
+        # Here we ignore the discontinuities in favor of a left or right
         # derivative, and simply return zero for all points.
         return None
 
     def _eval(self, subst, precision):
         try:
             return (
                 self._op1._eval(subst, precision)
@@ -2862,15 +2864,15 @@
     """
 
     def _diff(self, lhs, idstates):
         raise NotImplementedError(
             'Conditions do not have partial derivatives.')
 
 
-class PrefixCondition(Condition, PrefixExpression):
+class PrefixCondition(PrefixExpression, Condition):
     """
     Interface for prefix conditions.
 
     *Abstract class, extends:* :class:`Condition`, :class:`PrefixExpression`
     """
 
 
@@ -2916,15 +2918,15 @@
         return unit
 
     def _polishb(self, b):
         b.write('not ')
         self._op._polishb(b)
 
 
-class InfixCondition(Condition, InfixExpression):
+class InfixCondition(InfixExpression, Condition):
     """
     Base class for infix expressions.
 
     *Abstract class, extends:* :class:`Condition`, :class:`InfixExpression`
     """
     _rbp = CONDITIONAL
```

### Comparing `myokit-1.33.9/myokit/_io.py` & `myokit-1.34.0/myokit/_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         if not section.strip():
             raise myokit.SectionNotFoundError('Script section not found.')
         return myokit.parse(section.splitlines())[2]
 
 
 def load_state(filename, model=None):
     """
-    Loads an initial state from a file in one of the formats specified by
+    Loads a model state from a file in one of the formats specified by
     :func:`myokit.parse_state()`.
 
     If a :class:`Model` is provided the state will be run through
     :meth:`Model.map_to_state()` and returned as a list of floating point
     numbers.
     """
     filename = os.path.expanduser(filename)
@@ -106,15 +106,16 @@
         if model:
             s = model.map_to_state(s)
         return s
 
 
 def load_state_bin(filename):
     """
-    Loads an initial state from a file in the binary format used by myokit.
+    Loads a model state from a file in the binary format used by Myokit.
+
     See :meth:`save_state_bin` for details.
     """
     filename = os.path.expanduser(filename)
 
     # Load compression modules
     import zipfile
     try:
@@ -171,14 +172,18 @@
 
     The ``model`` argument can be given as plain text or a
     :class:`myokit.Model` object. Similarly, ``protocol`` can be either a
     :class:`myokit.Protocol` or its textual represenation.
 
     If no filename is given the ``mmt`` code is returned as a string.
     """
+    if model is None and protocol is None and script is None:
+        raise ValueError(
+            'At least one of [model, protocol, script] must not be None.')
+
     if filename:
         filename = os.path.expanduser(filename)
         f = open(filename, 'w')
     else:
         f = StringIO()
     out = None
     try:
@@ -240,15 +245,15 @@
     Saves an embedded script to a file
     """
     return save(filename, script=script)
 
 
 def save_state(filename, state, model=None):
     """
-    Stores the given state in the file at ``filename``.
+    Stores a model state to the path ``filename``.
 
     If no ``model`` is specified ``state`` should be given as a list of
     floating point numbers and will be stored by simply placing each number on
     a new line.
 
     If a :class:`Model <myokit.Model>` is provided the state can be in any
     format accepted by :meth:`Model.map_to_state() <myokit.Model.map_to_state>`
@@ -268,16 +273,16 @@
     # Store
     with open(filename, 'w') as f:
         f.write(state)
 
 
 def save_state_bin(filename, state, precision=myokit.DOUBLE_PRECISION):
     """
-    Stores the given state (or any list of floating point numbers) in the file
-    at ``filename``, using a binary format.
+    Stores a model state (or any given list of floating point numbers) to the
+    path ``filename``, using a binary format.
 
     The used format is a zip file, containing a single entry: ``state_x_y``,
     where ``x`` is the used data type (``d`` or ``f``) and ``y`` is the number
     of entries. All entries are stored little-endian.
     """
     # Check filename
     filename = os.path.expanduser(filename)
```

### Comparing `myokit-1.33.9/myokit/_model_api.py` & `myokit-1.34.0/myokit/_model_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -716,17 +716,15 @@
         """
         del self._variables[variable.name()]
 
     def _resolve(self, name):
         """ See :meth:`VarProvider._resolve(). """
         def sa(name):
             # Suggest alternative
-            m = self.model()
-            (var, sug, msg) = m.suggest_variable(name)
-            return msg
+            return self.model().suggest_variable(name)[2]
 
         # Try resolving as an alias
         try:
             return self._component._alias_map[name]
         except KeyError:
             pass
 
@@ -768,43 +766,43 @@
     obtained from a model ``m`` using ``m["x"]``. The number of components in
     ``m`` is given by ``len(m)`` and the presence of "x" in ``m`` can be tested
     using ``if "x" in m:``.
 
     Variables stored inside components can be accessed using :meth:`get()` or
     :meth:`values()`. Values defined through their derivative make up the
     model state and can be accessed using :meth:`states()`. States have
-    initial values accessible through :meth:`inits()`.
+    initial values accessible through :meth:`initial_values()`.
 
     A model's validity can be checked using :meth:`is_valid()`, which returns
     the latest validation status and :meth:`validate()`, which (re)validates
     the model. Warnings can be obtained using :meth:`warnings()`
 
     The optional constructor argument ``name`` can be used to set a meta
     property "name".
 
     Meta-data properties can be accessed via the property ``meta``, for example
     ``model.meta['key']= 'value'``.
 
     For consistency with components, variables, and expressions, models cannot
     be compared with ``==`` (which will only return ``True`` if both operands
     are the same object). Checking if models are the same in other senses can
-    be done with :meth:`is_similar`. Models can be serialised with ``pickle``.
+    be done with :meth:`is_similar`. Models can be serialized with ``pickle``.
     """
 
     def __init__(self, name=None):
         super(Model, self).__init__()
 
         # A dictionary of components
         self._components = {}
 
         # The model's state variables
-        self._state = []
+        self._state_vars = []
 
-        # The model's current state (list of floats)
-        self._current_state = []
+        # The model's initial state, as a list of Expressions
+        self._state_init = []
 
         # A dict mapping binding names to variables
         self._bindings = {}
 
         # A dict mapping label names to variables
         self._labels = {}
 
@@ -1083,17 +1081,19 @@
         # Copy meta data
         self._clone_metadata(clone)
 
         # Clone component/variable structure
         for c in self._components.values():
             c._clone1(clone)
 
-        # Clone state
-        for k, v in enumerate(self._state):
-            clone.get(v.qname()).promote(self._current_state[k])
+        # Create states
+        # Note that the order in which promote() is called determines the
+        # state ordering, so this happens here and not in the Variable class.
+        for k, v in enumerate(self._state_vars):
+            clone.get(v.qname()).promote()
 
         # Create mapping of old var references to new references
         var_map = {}
         lhs_map = {}
         for v in self.variables(deep=True):
             var_map[v] = w = clone.get(v.qname())
             lhs_map[myokit.Name(v)] = myokit.Name(w)
@@ -1106,14 +1106,19 @@
             c._clone2(clone[k], lhs_map, var_map)
 
         # Copy unique names and unique name prefixes
         clone.reserve_unique_names(*iter(self._reserved_unames))
         for prefix, prepend in self._reserved_uname_prefixes.items():
             clone.reserve_unique_name_prefix(prefix, prepend)
 
+        # Copy initial state expressions
+        for k, v in enumerate(self._state_vars):
+            clone.get(v.qname()).set_initial_value(
+                self._state_init[k].clone(subst=lhs_map))
+
         # Return
         return clone
 
     def code(self, line_numbers=False):
         """
         Returns this model in ``mmt`` syntax.
 
@@ -1137,25 +1142,23 @@
         Internal version of Model.code()
         """
         # b = buffer, t = number of tabs
         # Meta properties
         self._code_meta(b, 0)
 
         # Initial state
-        if self._state:
+        if self._state_vars:
             pre = t * TAB
             b.write(pre + '# Initial values\n')
-            names = [eq.lhs.code() for eq in self.inits()]
+            names = [v.qname() for v in self._state_vars]
+            values = [e.code() for e in self._state_init]
             n = max([len(name) for name in names])
-            names = iter(names)
-            for eq in self.inits():
-                name = next(names)
-                b.write(
-                    pre + name + ' ' * (n - len(name)) + ' = ' + eq.rhs.code()
-                    + '\n')
+            for name, value in zip(names, values):
+                b.write(pre + name + ' ' * (n - len(name)) + ' = '
+                        + value + '\n')
             b.write(pre + '\n')
         else:
             # No initial state? Then add newline
             b.write('\n')
 
         # Components
         for c in self.components(sort=True):
@@ -1239,15 +1242,15 @@
         """
         return len(self._components)
 
     def count_states(self):
         """
         Returns the number of state variables in this model.
         """
-        return len(self._state)
+        return len(self._state_vars)
 
     def create_unique_names(self):
         """
         Create a globally unique name for each Component and Variable.
 
         Ideally, the global name equals the variable or component's basic name.
         If a name is disputed the following strategy will be used:
@@ -1353,15 +1356,15 @@
 
         """
         values = {}
 
         # Insert new state (if required)
         if state is not None:
             new_state = self.map_to_state(state)
-            for state, value in zip(self._state, new_state):
+            for state, value in zip(self._state_vars, new_state):
                 values[myokit.Name(state)] = value
             state = None
 
         # Insert values of inputs (if required)
         if inputs is not None:
             for label, value in inputs.items():
                 var = self._bindings.get(label)
@@ -1386,15 +1389,15 @@
             for group in order.values():
                 for eq in group:
                     if eq.lhs in values:
                         continue
                     values[eq.lhs] = eq.rhs.eval(values, precision=precision)
 
         # Return calculated state
-        return [values[state.lhs()] for state in self._state]
+        return [values[state.lhs()] for state in self._state_vars]
 
     def eval_state_derivatives(
             self, state=None, inputs=None, precision=myokit.DOUBLE_PRECISION,
             ignore_errors=False):
         """
         Deprecated alias of :meth:`evaluate_derivatives()`.
         """
@@ -1485,43 +1488,43 @@
         eq_list = myokit.EquationList(eq_list)
 
         return (eq_list, arguments)
 
     def format_state(self, state=None, state2=None,
                      precision=myokit.DOUBLE_PRECISION):
         """
-        Converts the given list of floating point numbers to a string where
-        each line has the format ``<full_qualified_name> = <float_value>``.
+        Converts a sequence of floating point numbers to a string where each
+        line has the format ``<full_qualified_name> = <float_value>``.
 
         Arguments:
 
         ``state=None``
-            The state to show derivatives for. If no state is given the state
-            returned by :meth:`state` is used.
+            The state to display. If no state is given this model's (evaluated)
+            :meth:`<initial_values()>initial values` are used.
         ``state2=None``
             An optional second state, to be shown next to ``state`` for
             comparison.
         ``precision=myokit.DOUBLE_PRECISION``
             An optional precision argument to pass into
             :meth:`myokit.float.str` when formatting the state values.
 
         """
-        n = len(self._state)
-        if state is not None:
+        n = len(self._state_vars)
+        if state is None:
+            state = self.initial_values(as_floats=True)
+        else:
             if len(state) != n:
                 raise ValueError(
-                    'Argument `state` must be a list of (' + str(n)
+                    'Argument `state` must be a sequence of (' + str(n)
                     + ') floating point numbers.')
-        else:
-            state = self.state()
 
         if state2 is not None:
             if len(state2) != n:
                 raise ValueError(
-                    'Argument `state2` must be a list of (' + str(n)
+                    'Argument `state2` must be a sequence of (' + str(n)
                     + ') floating point numbers.')
 
         out = []
         n = max([len(x.qname()) for x in self.states()])
         for k, var in enumerate(self.states()):
             out.append(
                 var.qname() + ' ' * (n - len(var.qname()))
@@ -1537,43 +1540,43 @@
 
     def format_state_derivatives(self, state=None, derivatives=None,
                                  precision=myokit.DOUBLE_PRECISION):
         """
         Like :meth:`format_state` but displays the derivatives along with
         each state's value.
 
-
         Arguments:
 
         ``state=None``
-            The state to display. If no state is given the state returned by
-            :meth:`state` is used.
+            The state to show derivatives for. If no state is given this
+            model's (evaluated) :meth:`<initial_values()>initial values` are
+            used.
         ``derivatives=None``
-            An optional list of evaluated derivatives. If not given, the values
-            will be calculed from ``state`` using :meth:`eval_derivatives()`.
+            An optional list or other sequence of evaluated derivatives. If not
+            given, the values will be calculed from ``state`` using
+            :meth:`eval_derivatives()`.
         ``precision=myokit.DOUBLE_PRECISION``
             An optional precision argument to use when evaluating the state
             derivatives, and to pass into :meth:`myokit.float.str` when
             formatting the state values and derivatives.
 
         """
-        n = len(self._state)
+        n = len(self._state_vars)
         if state is None:
-            state = self.state()
+            state = self.initial_values(as_floats=True)
         elif len(state) != n:
             raise ValueError(
-                'Argument `state` must be a list of (' + str(n)
+                'Argument `state` must be a sequence of (' + str(n)
                 + ') floating point numbers.')
 
         if derivatives is None:
-            derivatives = self.evaluate_derivatives(
-                state, precision=precision)
+            derivatives = self.evaluate_derivatives(state, precision=precision)
         elif len(derivatives) != n:
             raise ValueError(
-                'Argument `deriv` must be a list of (' + str(n)
+                'Argument `derivatives` must be a sequence of (' + str(n)
                 + ') floating point numbers.')
 
         out = []
         n = max([len(x.qname()) for x in self.states()])
         for i, var in enumerate(self.states()):
             s = myokit.float.str(state[i], precision=precision)
             d = myokit.float.str(derivatives[i], precision=precision)
@@ -1798,14 +1801,17 @@
         # Create a list of all external variables that require mapping
         vars_to_map = set()
         for i, comp in enumerate(external_component):
             vars_ref = set()
             for var in comp.variables():
                 vars_ref.update(var.refs_to(state_refs=False))
                 vars_ref.update(var.refs_to(state_refs=True))
+                if var.is_state():
+                    vars_ref.update(
+                        [e.var() for e in var.initial_value().references()])
             vars_ref.update(comp._alias_map.values())
             vars_ref -= set(comp.variables())
             vars_ref = [x for x in vars_ref if not x.is_nested()]
             vars_to_map.update(vars_ref)
         map_to_clone = []
         for comp in external_component:
             map_to_clone.append(vars_to_map.intersection(comp.variables()))
@@ -1873,16 +1879,16 @@
                         + '>.')
                 used_local_vars.add(self_var)
 
                 # Valid mapping: Store, but only if this is a required variable
                 if ext_var in vars_to_map:
                     var_map[ext_var] = self_var
 
-        # add variables to var_map that map to other imported components
-        # but will be reassigned to the clone later
+        # Add variables to var_map that map to other imported components but
+        # will be reassigned to the clone later
         for l in map_to_clone:
             for ext_var in l:
                 if ext_var not in var_map:
                     var_map[ext_var] = None
 
         # Add non user-specified variables that require mapping
         for ext_var in vars_to_map:
@@ -1959,27 +1965,37 @@
                             ext_unit, self_unit)
                     except myokit.IncompatibleUnitError as e:
                         raise myokit.VariableMappingError(
                             'Unable to map time variables due to unit'
                             ' mismatch: ' + str(e))
 
         # Clone component pt 1: create, meta data, empty variables
-        new_component = []
+        new_component = []  # List of components
         for i, comp in enumerate(external_component):
             new_component.append(comp._clone1(self, new_name[i]))
 
-            for var in comp.variables(state=True):
-                # Clone states
-                # TODO: Not sure why clone() code doesn't do this?
-                new_component[i].get(var.qname(comp)).promote(
-                    var.state_value())
             # Now we can add variable to var_map if needed
             for var in map_to_clone[i]:
                 var_map[var] = new_component[i].get(var.qname(comp))
 
+        # Clone states, preserving the state order
+        # Note: The order in which promote() is called determines the order
+        # of the states in the new component. (This is one of the reasons that
+        # the component._clone1 method called above doesn't call promote.)
+        new_states = []     # New states, from all components
+        state_map = {}      # New-state to old state
+        for old_comp, comp in zip(external_component, new_component):
+            for ext_var in old_comp.variables(state=True):
+                var = comp.get(ext_var.name())
+                state_map[var] = ext_var
+                new_states.append(var)
+        new_states.sort(key=lambda var: state_map[var].index())
+        for var in new_states:
+            var.promote()   # Initial value is set later
+
         # Create mapping of old var references to new references
         # This is a mapping from Name(var) and Derivative(Name(var)) objects
         # to new myokit.Expressions referencing the target model's variables
         lhs_map = {}
 
         # Start with all variables (including nested variables) inside the
         # imported component.
@@ -1987,17 +2003,18 @@
             for ext_var in comp.variables(deep=True):
                 self_var = new_component[i].get(ext_var.qname(comp))
                 lhs_map[myokit.Name(ext_var)] = myokit.Name(self_var)
                 if ext_var.is_state():
                     lhs_map[myokit.Derivative(myokit.Name(ext_var))] = \
                         myokit.Derivative(myokit.Name(self_var))
 
-        # Next, add all entries in the var_map. If unit conversion is enabled,
-        # this may include the addition of unit conversion factors
-
+        # Next, add all entries in the var_map to the lhs_map. If unit
+        # conversion is enabled, this may include the addition of unit
+        # conversion factors (so some Names in lhs_map will be mapped onto
+        # Multiply expressions).
         for ext_var, self_var in var_map.items():
             # Substitute in either a reference to self_var, or an expression
             # that converts self_var to the units ext_var's equation expects.
             ex = myokit.Name(self_var)
             factor = factors.get(ext_var, None)
             if factor is not None:
                 ex = myokit.Multiply(ex, myokit.Number(factor))
@@ -2018,32 +2035,54 @@
                     ex = myokit.Multiply(ex, myokit.Number(factor))
                 lhs_map[myokit.Derivative(myokit.Name(ext_var))] = ex
 
         # Clone component/variable contents (equations, references)
         for i, comp in enumerate(external_component):
             comp._clone2(new_component[i], lhs_map, var_map)
 
+        # Clone initial values
+        for var in new_states:
+            var.set_initial_value(
+                state_map[var].initial_value().clone(subst=lhs_map))
+
         # Time unit conversion? Then update all derivatives.
         if time_factor is not None:
             for comp in new_component:
                 for var in comp.variables(state=True):
                     rhs = var.rhs()
                     if rhs is not None:
                         var.set_rhs(
                             myokit.Multiply(rhs, myokit.Number(time_factor)))
 
+    def initial_values(self, as_floats=False):
+        """
+        Returns a list of the model's initial values.
+
+        By default, expressions are returned, but this can be changed to
+        a list of floats by setting ``as_floats=True``.
+        """
+        if as_floats:
+            if any(not e.is_literal() for e in self._state_init):
+                self.validate()  # Check for cycles before evaluating
+            return [float(y) for y in self._state_init]
+        return list(self._state_init)
+
     def inits(self):
         """
-        Returns an iterator over the ``Equation`` objects defining this model's
-        current state.
+        Deprecated method: Returns an iterator over the ``Equation`` objects
+        defining this model's initial values.
         """
+        # Deprecated since 2023-02-22
+        import warnings
+        warnings.warn('The method `inits` is deprecated.')
+
         def StateDefIterator(model):
-            for k, var in enumerate(model._state):
-                yield Equation(
-                    myokit.Name(var), myokit.Number(self._current_state[k]))
+            for var, value in zip(model._state_vars, model._state_init):
+                yield Equation(myokit.Name(var), value)
+
         return StateDefIterator(self)
 
     def is_similar(self, other, check_unames=False):
         """
         Returns ``True`` if this model has the same code as the ``other``
         model.
 
@@ -2130,18 +2169,21 @@
                 'No variable found with label "' + str(label) + '".')
 
     def __len__(self):
         return len(self._components)
 
     def load_state(self, filename):
         """
-        Sets the model state using data from a file formatted in any style
-        accepted by :func:`myokit.parse_state`.
+        Deprecated method: Sets the model's initial values using data from a
+        file formatted in any style accepted by :func:`myokit.map_to_state`.
         """
-        self.set_state(myokit.load_state(filename, self))
+        # Deprecated since 2023-02-22
+        import warnings
+        warnings.warn('The method `load_state` is deprecated.')
+        self.set_initial_values(myokit.load_state(filename, self))
 
     def map_component_dependencies(
             self, omit_states=True, omit_constants=False):
         """
         Scans all equations and creates a map of inter-component dependencies.
 
         The result is an ordered dictionary with the following structure::
@@ -2156,15 +2198,15 @@
         the components they depend upon.
 
         Only direct dependencies are listed: If ``A`` depends on ``B`` and
         ``B`` depends on ``C`` then the returned value for ``A`` is ``[B]``,
         not ``[B,C]``.
 
         By default, dependencies on state variables' current values are
-        omitted. This behaviour can be changed by setting ``omit_states`` to
+        omitted. This behavior can be changed by setting ``omit_states`` to
         ``False``.
 
         To omit all dependencies on constants, set ``omit_constants`` to
         ``True``.
         """
         # Map shallow dependencies
         shallow = self.map_shallow_dependencies(
@@ -2336,15 +2378,15 @@
         references, a :class:`myokit.IntegrityError` is raised.
 
         If the optional parameter ``collapse`` is set to ``True``
         nested variables will not be listed separatly. Instead, their
         dependencies will be added to the dependency lists of their parents.
 
         By default, dependencies on state variables' current values are
-        omitted. This behaviour can be changed by setting ``omit_states`` to
+        omitted. This behavior can be changed by setting ``omit_states`` to
         ``False``.
 
         In case of a dependency such as::
 
             a = f(b)
             b = g(c)
 
@@ -2480,15 +2522,15 @@
         ``b``.
 
         If the optional parameter ``collapse`` is set to ``True``
         nested variables will not be listed separatly. Instead, their
         dependencies will be added to the dependency lists of their parents.
 
         By default, dependencies on state variables' current values are
-        omitted. This behaviour can be changed by setting ``omit_states`` to
+        omitted. This behavior can be changed by setting ``omit_states`` to
         ``False``. Dependencies on constants are included by default, but this
         can be changed by setting ``omit_constants`` to ``True``.
         """
         # Find dependencies for every stored equation
         out = {}
         inc = not omit_states
         const = False if omit_constants else None
@@ -2588,53 +2630,14 @@
         Returns the model meta property ``name``, or ``None`` if it isn't set.
         """
         try:
             return self.meta['name']
         except KeyError:
             return None
 
-    def prepare_bindings(self, labels):
-        """
-        Takes a mapping of binding labels to internal references as input and
-        returns a mapping of variables to internal references. All variables
-        appearing in the map will have their right hand side set to zero. All
-        bindings not mapped to any internal reference will be deleted.
-
-        The argument ``mapping`` should take the form::
-
-            labels = {
-                'binding_label_1' : internal_name_1,
-                'binding_label_2' : internal_name_2,
-                ...
-                }
-
-        The returned dictionary will have the form::
-
-            variables = {
-                variable_x : internal_name_1,
-                variable_y : internal_name_2,
-                ...
-                }
-
-        Unsupported bindings (i.e. bindings not appearing in ``labels``) will
-        be ignored.
-        """
-        unused = []
-        variables = {}
-        for label, var in self._bindings.items():
-            try:
-                variables[var] = labels[label]
-            except KeyError:
-                unused.append(var)
-                continue
-            var.set_rhs(0)
-        for var in unused:
-            var.set_binding(None)
-        return variables
-
     def __reduce__(self):
         """
         Pickles the model.
 
         See: https://docs.python.org/3/library/pickle.html#object.__reduce__
         """
         return (
@@ -2697,15 +2700,15 @@
     def reorder_state(self, order):
         """
         Changes the order of this model's state variables. The argument
         ``order`` must be a list of state variables or their qnames.
 
         This method does not affect the model's validation status.
         """
-        n = len(self._state)
+        n = len(self._state_vars)
         if len(order) != n:
             raise ValueError(
                 'The given list must contain the same number of entries as'
                 ' there are state variables in this model.')
         state = []
         current = []
         for v in order:
@@ -2715,19 +2718,19 @@
                     'The entries of ``order`` must all be state variables or'
                     ' state variable qnames.')
             if v in state:
                 raise ValueError(
                     'Duplicate entry in order specification: "'
                     + str(v.qname()) + '".')
             state.append(v)
-            current.append(self._current_state[v._indice])
-        self._state = state
-        self._current_state = current
+            current.append(self._state_init[v._index])
+        self._state_vars = state
+        self._state_init = current
         for k, v in enumerate(state):
-            v._indice = k
+            v._index = k
 
     def remove_component(self, component):
         """
         Removes a component from the model.
 
         This will reset the model's validation status.
         """
@@ -2767,15 +2770,15 @@
         """
         # Get time unit
         time = self.time()
         if time is not None:
             time_unit = time.unit()
 
         # Scan all states
-        for state in self._state:
+        for state in self._state_vars:
 
             # Search for references to dot(state)
             refs = list(state.refs_by())
 
             if refs:
                 # If found, add a new variable to represent dot(state)
                 var = state.parent().add_variable_allow_renaming(
@@ -2838,26 +2841,30 @@
             raise ValueError('String to prepend cannot start with prefix.')
         self._reserved_uname_prefixes[prefix] = prepend
 
     def _reset_indices(self):
         """
         Resets the indices of this model's state variables.
         """
-        for k, v in enumerate(self._state):
-            v._indice = k
+        for k, v in enumerate(self._state_vars):
+            v._index = k
 
     def _reset_validation(self):
         """
         Will reset the model's validation status to not validated.
         """
         self._valid = None
 
     def _resolve(self, name):
         """ See :meth:`VarProvider._resolve(). """
-        return self.get(name)
+        try:
+            return self.get(name)
+        except KeyError:
+            raise myokit.UnresolvedReferenceError(
+                name, self.suggest_variable(name)[2])
 
     def resolve_interdependent_components(self):
         """
         Checks if the model contains components that each depend on the other.
         If so, variables from these components will be moved to a new component
         called "remaining" until the issue is resolved.
         """
@@ -2883,17 +2890,47 @@
         for eq in remaining:
             var = eq.lhs.var()
             var.parent().move_variable(var, comp, var.uname())
         # Done!
 
     def save_state(self, filename):
         """
-        Saves the model state to a file.
+        Deprecated method: Saves the model state to a file (as floats).
+        """
+        # Deprecated since 2023-02-22
+        import warnings
+        warnings.warn('The method `save_state` is deprecated.')
+
+        return myokit.save_state(
+            filename, self.initial_values(as_floats=True), self)
+
+    def set_initial_values(self, values):
         """
-        return myokit.save_state(filename, self.state(), self)
+        Sets this model's initial values.
+
+        The ``values`` must be specified as either a list of floats,
+        expressions, and/or strings; or as a dict or string in a format
+        accepted by :meth:`map_to_state`.
+        """
+        # Use map to state?
+        if isinstance(values, basestring) or isinstance(values, dict):
+            self._state_init = [
+                myokit.Number(x) for x in self.map_to_state(values)]
+        elif len(values) != len(self._state_vars):
+            raise ValueError('Wrong number of initial values, expecting '
+                             + str(len(self._state_vars)) + '.')
+        else:
+            # Parsing of arguments without making changes, in case it fails.
+            expr = []
+            for var, value in zip(self._state_vars, values):
+                expr.append(var._set_initial_value(value, False))
+
+            # Set all at once, and reset validation status
+            self._state_init = expr
+            self._valid = None
 
     def set_name(self, name=None):
         """
         Changes the value of the meta-property "name".
         """
         if name is None:
             try:
@@ -2910,18 +2947,22 @@
         See: https://docs.python.org/3/library/pickle.html#object.__setstate__
         """
         self._reserved_unames = state[0]
         self._reserved_uname_prefixes = state[1]
 
     def set_state(self, state):
         """
-        Changes this model's state. Accepts any type of input handled by
-        :meth:`map_to_state`.
+        Deprecated method: use :meth:`set_initial_values` instead.
         """
-        self._current_state = self.map_to_state(state)
+        # Deprecated since 2023-02-22
+        import warnings
+        warnings.warn(
+            'The method `set_state` is deprecated. Please use'
+            ' `set_initial_values` instead.')
+        self.set_initial_values(state)
 
     def set_value(self, qname, value):
         """
         Changes a variable's defining expression to the given number or
         :class:`myokit.Expression`.
 
         For state variables, this updates the expression for their derivative.
@@ -2934,28 +2975,34 @@
     def show_evaluation_of(self, var):
         """
         Returns a string representing the evaluation of a single variable.
 
         The variable's equation and value are displayed, along with the value
         and formula of any nested variables and the values of all dependencies.
         """
+        # Model must be valid, or cycles can occur
+        self.validate()
+
         def format_float(number):
             s = str(number)
             if len(s) < 10:
                 return s
             return '%0.17e' % number
 
         # Add basic info
         spacer = '-' * 60
         var, out = self._var_info(var, spacer)
 
         # Add initial value
         rhs = var.rhs()
         if var.is_state():
-            out.append('Initial value = ' + str(var.state_value()))
+            value = var.initial_value()
+            out.append('Initial value = ' + value.code())
+            if not isinstance(value, myokit.Number):
+                out.append('              = ' + format_float(value))
             out.append(spacer)
         varname = var.lhs().code()
 
         # Add references
         deps = list(rhs.references())
         deps.sort(key=lambda x: x.code())
         if deps:
@@ -3233,25 +3280,30 @@
             raise RuntimeError('Equation ordering failed.')
 
         # Return
         return out
 
     def state(self):
         """
-        Returns the current state of the model as a list of floating point
-        numbers.
+        Deprecated method, use
+        :meth:`initial_values(as_floats=True)<initial_values>` instead.
         """
-        return list(self._current_state)
+        # Deprecated since 2023-02-22
+        import warnings
+        warnings.warn(
+            'The method `state` is deprecated. Please use'
+            ' `initial_values(as_floats=True)` instead.')
+        return self.initial_values(as_floats=True)
 
     def states(self):
         """
         Returns an iterator over this model's state :class:`variable
         <myokit.Variable>` objects.
         """
-        return iter(self._state)
+        return iter(self._state_vars)
 
     def suggest_variable(self, name):
         """
         Returns a tuple ``(found, suggested, msg)``.
 
         If the requested variable is found, only the ``found`` part of the
         tuple is set. If not, the second and third argument are set. Here
@@ -3324,18 +3376,15 @@
         """
         Returns this model's time variable.
 
         The time variable is identified by it's binding to the external source
         "time". For a valid model, this method always returns a unique
         variable. If no time variable has been declared ``None`` is returned.
         """
-        try:
-            return self._bindings['time']
-        except KeyError:
-            return None
+        return self._bindings.get('time')
 
     def timex(self):
         """
         Returns this model's time variable, raising a
         :class:`myokit.IncompatibleModelError` if no time variable is found.
 
         See :meth:`Model.time()`.
@@ -3369,15 +3418,15 @@
         :class:`Expression` objects.
         """
         # Names and expressions are immutable, so ok to return
         return dict(self._user_functions)
 
     def validate(self, remove_unused_variables=False):
         """
-        Attempts to check model validity, raises errors if it isn't.
+        Validates this model and raises errors if any issues are found.
 
         Small issues (e.g. unused variables) will generate warnings, which
         can be retrieved using :meth:`Model.warnings()` or
         :meth:`Model.format_warnings()`. Any previously set warnings will be
         erased whenever `validate()` is run.
 
         If ``remove_unused_variables`` is set to True, any unused variables
@@ -3395,14 +3444,23 @@
             # Added cover pragma: This can only happen if there is a bug
             # somewhere!
             self._valid = False
             raise myokit.IntegrityError(
                 'Invalid time variable set. Time variable must be bound to'
                 ' external value "time".')
 
+        # Test initial value expresions
+        n = len(self._state_vars)
+        if n != len(self._state_init):   # pragma: no cover
+            # Cover pragma: This can only happen if there's an API bug
+            self._valid = False
+            raise myokit.IntegrityError(
+                'Initial values list must have same size as state variables'
+                ' list.')
+
         # Validation of components, variables
         for c in self.components():
             if c._parent != self:   # pragma: no cover
                 # Cover pragma: This can only happen if there's an API bug
                 msg = 'Component parent doesn\'t match with enclosing model <'
                 msg += c.name() + '>.'
                 self._valid = False
@@ -3415,23 +3473,14 @@
             if n != c.qname():  # pragma: no cover
                 # Cover pragma: This can only happen if there's an API bug
                 self._valid = False
                 raise myokit.IntegrityError(
                     'Component called <' + c.qname() + '> found at index <'
                     + n + '>.')
 
-        # Test current state values
-        n = len(self._state)
-        if n != len(self._current_state):   # pragma: no cover
-            # Cover pragma: This can only happen if there's an API bug
-            self._valid = False
-            raise myokit.IntegrityError(
-                'Current state values list must have same size as state'
-                ' variables list.')
-
         # Find cycles, warn of unused variables
         self._validate_solvability(remove_unused_variables)
 
         # Create globally unique names
         self.create_unique_names()
 
         # Return
@@ -3477,15 +3526,15 @@
                         follow(d, v, trail, mark_used)
                 trail.pop()
                 if mark_used:
                     var._used = True
 
         # Follow all state variables (unless already visited), all bound
         # variables and all used variables.
-        used = [x for x in self._state]
+        used = [x for x in self._state_vars]
         used += [x for x in self._bindings.values()]
         used += [x for x in self._labels.values()]
 
         # Check for cycles
         trail = []
 
         # Despite its "slow" is-in check, using a list for this purpose is
@@ -3543,15 +3592,15 @@
         uses suggest_variable to find a match) and out is a list of strings
         where each entry is a line of the description.
         """
         out = []
         if not isinstance(var, ModelPart):
             var = self.suggest_variable(var)
             if var[0] is None:
-                if var[1] is None:
+                if var[1] is None:  # pragma: no cover
                     raise Exception(var[2])
                 var = var[1]
                 out.append(
                     'Variable not found, assuming <' + var.qname() + '>.')
             else:
                 var = var[0]
         if var.is_state():
@@ -3822,16 +3871,16 @@
     Meta-data properties can be accessed via the property ``meta``, for example
     ``model.meta['key']= 'value'``.
     """
 
     def __init__(self, parent, name):
         super(Variable, self).__init__(parent, name)
 
-        # Indice, only set if this is a state variable
-        self._indice = None
+        # Index, only set if this is a state variable
+        self._index = None
 
         # This variable's unit, if given, else dimensionless
         self._unit = None
 
         # This variable's label, if given
         self._label = None
 
@@ -3881,15 +3930,19 @@
           ``var.set_rhs(var.eval())``.
         - If this is a state variable, it will be demoted.
         - Any child variables will be removed.
 
         """
         # Set value
         if value is None:
-            value = self.state_value() if self._is_state else self._rhs.eval()
+            self.model().validate()  # Model must be valid before evaluations
+            if self._is_state:
+                value = self.initial_value(True)
+            else:
+                value = self._rhs.eval()
         else:
             value = float(value)
 
         # Demote states (will raise an error if can't)
         if self.is_state():
             self.demote()
 
@@ -3916,15 +3969,15 @@
         """
         Performs step 2 of cloning this variable into ``v``. Adds equations,
         bindings, unit etc.
 
         The argument ``lhs_map`` should be a dictionary mapping old
         :class:`LhsExpression` objects their equivalents in the new model.
         """
-        # _indice is set by promoting (done by model)
+        # _index is set by promoting (done by model)
         # _binding
         if self._binding:
             v.set_binding(self._binding)
 
         # _label
         if self._label:
             v.set_label(self._label)
@@ -3938,14 +3991,18 @@
         if self._rhs:
             v.set_rhs(self._rhs.clone(subst=lhs_map))
 
         # Clone child variables
         for k in self.variables():
             k._clone2(v[k.name()], lhs_map)
 
+        # Note: initial values are stored inside the model, and the state order
+        # depends on the order in which promoting occurs, so states are only
+        # created by Model.clone()
+
     def _code(self, b, t):
         """
         Create the code for this variable and any child variables.
         """
         # Create header line
         c = self.parent(Component)
         lhs = self._lhs.code(c) if self._lhs else 'UNNAMED'
@@ -4077,15 +4134,20 @@
         self.set_unit(new_unit)
 
         # Update the variable's definition
         self.set_rhs(myokit.Multiply(self.rhs(), fw))
 
         # For states, update the current/initial value
         if self._is_state:
-            self.set_state_value(self.state_value() * float(fw))
+            # Number? Then just multiply. Else use expression.
+            value = self.initial_value()
+            if isinstance(value, myokit.Number):
+                self.set_initial_value(float(value) * float(fw))
+            else:
+                self.set_initial_value(myokit.Multiply(value, fw))
 
         # Update all references to the variable
         old_ref = myokit.Name(self)
         new_ref = myokit.Divide(old_ref, fw)
         for var in list(self.refs_by(self._is_state)):
             var.set_rhs(var.rhs().clone(subst={old_ref: new_ref}))
 
@@ -4155,14 +4217,37 @@
 
             if refs:
                 raise myokit.IntegrityError(
                     'Variable <' + self.qname() + '>'
                     ' can not be removed: it is used by ' + ' and '.join(
                         ['<' + v.qname() + '>' for v in refs]) + '.')
 
+        # Third check: Do initial values depend on this variable?
+        # Note that, instead of using a cached set in every variable, this
+        # reference is just checked by scanning all init expressions (which
+        # contain a cached set of references).
+        # Note that we don't optimise by checking if this variable is constant,
+        # as it's possible to create (invalid) models where non-constants are
+        # referenced in initial values (but validate() will pick this up!).
+        refs = set()
+        m = self.model()
+        n = myokit.Name(self)
+        for v, e in zip(m._state_vars, m._state_init):
+            if n in e.references():
+                refs.add(v)
+        if ignore_siblings:
+            # Refs from sibling variables are allowed
+            refs = refs.difference(
+                set([x for x in refs if x.has_ancestor(self._parent)]))
+        if refs:
+            raise myokit.IntegrityError(
+                'Variable <' + self.qname() + '> can not be removed: it is'
+                ' used in the inital value(s) for ' + ' and '.join(
+                    ['<' + v.qname() + '>' for v in refs]) + '.')
+
         # At this point it's OK to delete. Rest of the code makes changes,
         # shouldn't raise errors.
 
         # Tell other variables it no longer depends on them
         for var in self._refs_to:
             var._refs_by.remove(self)
         for var in self._srefs_to:
@@ -4179,15 +4264,14 @@
                 self.demote()
 
             # Remove any bindings or labels
             self.set_binding(None)
             self.set_label(None)
 
             # Remove any aliases
-            m = self.parent(Model)
             for c in m.components():
                 c.remove_aliases_for(self)
 
         # Delete child variables
         if recursive:
             for kid in kids:
                 # Call this method for each kid (and cascade to their kids)
@@ -4201,37 +4285,37 @@
     def demote(self):
         """
         Turns a state variable into an intermediary variable.
 
         This will reset the validation status of the model this variable
         belongs to.
         """
-        if self._indice is None:
+        if self._index is None:
             raise Exception('Variable is not a state variable.')
 
         # Check that nobody has references to this var's derivative
         if self._refs_by:
             refs = ', '.join([r.qname() for r in self._refs_by])
             raise Exception(
                 'Unable to demote variable while references to its derivative'
                 ' are made by (' + refs + ').')
 
         model = self.model()
         try:
             # Remove initial value
-            del model._current_state[self._indice]
+            del model._state_init[self._index]
 
             # Remove this variable from the state
-            del model._state[self._indice]
+            del model._state_vars[self._index]
 
             # Set lhs to name expression
             self._lhs = myokit.Name(self)
 
-            # Remove this variable's indice
-            self._indice = None
+            # Remove this variable's index
+            self._index = None
 
             # Reset other states' indices
             model._reset_indices()
 
             # All state refs to this variable are now considered ordinary refs
             # (And _refs_by is emtpy, see check above)
             for r in self._srefs_by:
@@ -4256,57 +4340,87 @@
 
     def eval(self):
         """
         Evaluates this variable's defining equation and returns the result.
         """
         return self._rhs.eval()
 
-    def indice(self):
+    def index(self):
         """
         For state variables, this will return their index in the state vector.
+
         For all other variables, this will raise an exception.
         """
-        if self._indice is None:
+        if self._index is None:
+            raise Exception('Only state variables have initial values.')
+        return self._index
+
+    def indice(self):
+        """ Deprecated alias of :meth:`index`. """
+
+        # Deprecated on 2023-06-07
+        import warnings
+        warnings.warn(
+            'The method `indice` is deprecated. Please use `index()` instead.')
+        return self.index()
+
+    def initial_value(self, as_float=False):
+        """
+        Returns a state variable's initial value, or raises an exception when
+        called on a non-state variable.
+
+        By default, a :class:`myokit.Expression` is returned. To evaluate and
+        return a float set ``as_float=True``.
+        """
+        if not self._is_state:
             raise Exception('Only state variables have initial values.')
-        return self._indice
+
+        model = self.model()
+        expr = model._state_init[self._index]
+        if not as_float:
+            return expr
+        if not expr.is_literal():
+            model.validate()
+        return expr.eval()
 
     def is_bound(self):
         """
         Returns ``True`` if a binding label has been added to this variable.
         """
         return self._is_bound
 
     def is_constant(self):
         """
-        Returns ``True`` if this variable is constant.
+        Returns ``True`` if this variable has a constant value (even if that
+        value is defined in terms of other constants).
 
         Myokit doesn't discern between mathematical and physical constants,
         parameters etc. Anything that doesn't change during a simulation is
-        termed a constant. Note that this specifically excludes variables bound
-        to external inputs.
+        termed a constant. Note that this specifically excludes variables that
+        define a _binding_ to an external input.
         """
         return self._is_constant
 
     def is_intermediary(self):
         """
         Returns ``True`` if this variable is an intermediary variable, i.e. not
-        a constant or a state variable (and not bound to an external variable).
+        a constant, not a state variable, and not bound to an external input
+        such as time.
         """
         return self._is_intermediary
 
     def is_labelled(self):
         """
         Returns ``True`` if a label has been added to this variable.
         """
         return self._label is not None
 
     def is_literal(self):
         """
-        Returns ``True`` if this variable's expression contains only literal
-        values.
+        Returns ``True`` if this variable does not depend on other variables.
         """
         return self._is_literal
 
     def is_nested(self):
         """
         Returns ``True`` if this variable's parent is another variable.
         """
@@ -4337,50 +4451,76 @@
         Returns the left-hand side of the equation defining this variable.
 
         For state variables this will be a :class:`myokit.Derivative`, for
         all others this should be a :class:`myokit.Name`.
         """
         return self._lhs
 
-    def promote(self, state_value=0):
+    def promote(self, initial_value=0, state_value=None):
         """
-        Turns this variable into a state variable with a current state value
-        given by ``state_value``.
+        Turns this variable into a state variable with an initial value given
+        by ``initial_value``.
 
-        This will reset the validation status of the model this variable
-        belongs to.
+        The new ``initial_value`` should be:
+
+        1. A numerical value.
+        2. A :class:`myokit.Expression`.
+        3. A string which can be parsed to a :class:`myokit.Expression`. Any
+           references to variables must be made using their fully qualified
+           names.
+
+        Note that expressions can contain references to non-nested and
+        constant-valued variables (i.e. their right-hand side is either a
+        literal expression or refers only to constants).
+
+        Calling ``promote`` will reset the validation status of the model this
+        variable belongs to.
         """
-        if self._indice is not None:
+        if self._index is not None:
             raise Exception('Variable is already a state variable')
         if not isinstance(self._parent, Component):
             raise Exception('State variables can only be added to Components.')
         if self._binding is not None:
             raise Exception(
                 'State variables cannot be bound to an external value.')
 
-        # Check state value argument
-        if isinstance(state_value, myokit.Expression):
-            if not state_value.is_literal():
-                raise myokit.NonLiteralValueError(
-                    'Expressions for state values can not contain references'
-                    ' to other variables.')
+        # Deprecated on 2023-02-22
+        if state_value is not None:
+            if initial_value != 0:
+                raise Exception('Deprecated keyword argument `state_value` can'
+                                ' not be used at the same time as its'
+                                ' replacement `initial_value`.')
+            initial_value = state_value
+
+            import warnings
+            warnings.warn('The keyword argument `state_value` is deprecated.'
+                          ' Please use `initial_value` instead.')
 
+        # Handle string and number rhs's
         model = self.model()
+        if not isinstance(initial_value, myokit.Expression):
+            if isinstance(initial_value, basestring):
+                # Expressions are evaluated in model context
+                initial_value = myokit.parse_expression(
+                    initial_value, context=model)
+            elif initial_value is not None:
+                initial_value = myokit.Number(initial_value)
+
         try:
             # Set lhs to derivative expression
             self._lhs = myokit.Derivative(myokit.Name(self))
 
-            # Get new indice
-            self._indice = len(model._state)
+            # Get new index
+            self._index = len(model._state_vars)
 
             # Add to list of states
-            model._state.append(self)
+            model._state_vars.append(self)
 
-            # Add value to list of current values
-            model._current_state.append(float(state_value))
+            # Add initial_value to list of current values
+            model._state_init.append(initial_value)
 
             # All references to this variable are now considered references to
             # its state value
             assert len(self._srefs_by) == 0
             for r in self._refs_by:
                 r._refs_to.remove(self)
                 r._srefs_to.add(self)
@@ -4520,30 +4660,30 @@
 
     def rename(self, new_name):
         """ Renames this variable. """
         assert self._parent is not None
         self._parent.move_variable(self, self._parent, new_name)
 
     def __repr__(self):
-        if self._indice is not None:
+        if self._index is not None:
             return '<State(' + self.qname() + ')>'
         else:
             return '<Var(' + self.qname() + ')>'
 
     def _reset_cache(self, bubble=False):
         """
         Updates this variable's cached attributes. If ``bubble`` is set to
         ``True`` and this variable's cache state changes, a cache reset will be
         triggered in all dependent variables.
         """
         if bubble:
             s_old = (self._is_bound, self._is_state, self._is_intermediary,
                      self._is_literal, self._is_constant, self._is_nested)
         self._is_bound = self._binding is not None
-        self._is_state = self._indice is not None
+        self._is_state = self._index is not None
         self._is_nested = isinstance(self._parent, Variable)
         if self._is_state or self._is_bound or self._rhs is None:
             self._is_constant = False
             self._is_literal = False
             self._is_intermediary = False
         else:
             self._is_constant = self._rhs.is_constant()
@@ -4582,15 +4722,15 @@
             # Check for existing binding
             if self._binding is not None:
                 raise myokit.InvalidBindingError(
                     'The variable <' + self.qname() + '>'
                     ' is already bound to "' + self._binding + '".')
 
             # Check if not a state
-            if self._indice is not None:
+            if self._index is not None:
                 raise myokit.InvalidBindingError(
                     'State variables cannot be bound to an external value.')
 
         # Set binding (model checks uniqueness)
         model = self.model()
         try:
             if binding is None:
@@ -4602,14 +4742,50 @@
         finally:
             # Clear cache and cache of dependent variables
             self._reset_cache(bubble=True)
 
             # Reset model validation
             model._reset_validation()
 
+    def set_initial_value(self, value):
+        """
+        Sets the initial value of a state variable, or raises an exception if
+        called on a non-state variable.
+
+        The new value can be passed in as an expression, number, or a string
+        (in which case it will be parsed as an expression). Expressions can
+        refer to variables as long as they are not nested and are constant in
+        time. Variable references in strings must be made using fully qualified
+        names (``component.variable``).
+        """
+        if not self._is_state:
+            raise Exception('Only state variables have state values.')
+        self._set_initial_value(value, True)
+
+    def _set_initial_value(self, value, make_the_change):
+        """ Internal version of `set_initial_value`. """
+        # Handle strings and floats
+        model = self.model()
+        if not isinstance(value, myokit.Expression):
+            if isinstance(value, basestring):
+                value = myokit.parse_expression(value, context=model)
+            else:
+                value = myokit.Number(value)
+
+        # Allow internal calls to parse `value` without making a change
+        if not make_the_change:
+            return value
+
+        # Update
+        try:
+            model._state_init[self._index] = value
+        finally:
+            # Reset model validation, but not the variable cache
+            model._reset_validation()
+
     def set_label(self, label=None):
         """
         Adds a unique ``label`` for this variable, indicated that its value can
         be read by external users.
 
         To remove a label call ``set_label(None)``.
         """
@@ -4689,27 +4865,22 @@
         # Set rhs
         self._rhs = rhs
         self.model()._reset_validation()
         self._reset_cache(bubble=True)
 
     def set_state_value(self, value):
         """
-        If this variable is a state variable, its current value will be
-        updated. For all other variables this raises an exception.
+        Deprecated method, use :meth:`set_initial_value` instead.
         """
-        if not self._is_state:
-            raise Exception('Only state variables have state values.')
-        model = self.model()
-        if isinstance(value, myokit.Expression):
-            if not value.is_literal():
-                raise myokit.NonLiteralValueError(
-                    'Expressions for state values can not contain references'
-                    ' to other variables.')
-        model._current_state[self._indice] = float(value)
-        # No need to reset validation status or cache here.
+        # Deprecated since 2023-02-22
+        import warnings
+        warnings.warn(
+            'The method `set_state_value` is deprecated. Please use'
+            ' `set_initial_value` instead.')
+        self.set_initial_value(value)
 
     def set_unit(self, unit=None):
         """
         Changes this variable's unit. The unit can be set to any valid Unit
         object, or ``None`` to remove the unit.
         """
         if unit is None or isinstance(unit, myokit.Unit):
@@ -4719,20 +4890,23 @@
         else:
             raise TypeError('Method set_unit() expects a myokit.Unit or None.')
         # No need to reset validation status or cache. Units are checked only
         # by the model.
 
     def state_value(self):
         """
-        For state variables, this will return their current value.
-        For all other variables, this will raise an exception.
+        Deprecated method, use
+        :meth:`initial_value(as_float=True)<initial_value>` instead.
         """
-        if not self._is_state:
-            raise Exception('Only state variables have initial values.')
-        return self.model()._current_state[self._indice]
+        # Deprecated since 2023-02-22
+        import warnings
+        warnings.warn(
+            'The method `state_value` is deprecated. Please use'
+            ' `initial_value(as_float=True)` instead.')
+        return self.initial_value(as_float=True)
 
     def unit(self, mode=myokit.UNIT_TOLERANT):
         """
         Returns the unit specified for this variable.
 
         If no unit was set and ``mode`` is ``myokit.UNIT_TOLERANT``, then None
         is returned. In ``myokit.UNIT_STRICT`` mode the value
@@ -4748,54 +4922,97 @@
             return myokit.units.dimensionless
         return self._unit
 
     def validate(self):
         """
         Attempts to check this variable's validity, raises errors if it isn't.
         """
+        #
         # Validate rhs
+        #
         if self._rhs is None:
             raise myokit.MissingRhsError(self)
         self._rhs.validate()
 
-        # Partial derivatives are not allowed in an RHS
+        # RHS: No PartialDerivative objects
         if self._rhs.contains_type(myokit.PartialDerivative):
             raise myokit.IntegrityError(
                 'Partial derivatives may not appear in expressions set as'
-                ' right-hand side of a variable.')
+                ' right-hand side of a variable: <' + self.qname() + '>.')
 
-        # Initial values are not allowed in an RHS
+        # RHS: No InitialValue objects
         if self._rhs.contains_type(myokit.InitialValue):
             raise myokit.IntegrityError(
                 'Initial value operators may not appear in expressions set as'
-                ' right-hand side of a variable.')
+                ' right-hand side of a variable: <' + self.qname() + '>.')
 
-        # Conditions are not allowed as an RHS
+        # RHS: Can't evaluate to True or False
         if isinstance(self._rhs, myokit.Condition):
             raise myokit.IntegrityError(
                 'The right-hand side expression for a variable can not be a'
-                ' condition.')
+                ' condition: <' + self.qname() + '>.')
 
+        #
         # Check state variables
-        is_state = self._indice is not None
+        #
+        is_state = self._index is not None
         is_deriv = self.lhs().is_derivative()
         if is_state:
+            # Derivative is set
             if not is_deriv:        # pragma: no cover
                 raise myokit.IntegrityError(
                     'Variable <' + self.qname() + '> is listed as a state'
                     ' variable but its lhs is not a derivative.')
+
+            # Not nested
             if self._is_nested:     # pragma: no cover
                 raise myokit.IntegrityError(
                     'State variables should not be nested: <'
                     + str(self.qname()) + '>.')
+
+            # Index matches model
             m = self.model()
-            if not m._state[self._indice] == self:  # pragma: no cover
+            if not m._state_vars[self._index] == self:  # pragma: no cover
                 raise myokit.IntegrityError(
                     'State variable not listed in model state vector at'
-                    ' correct indice: <' + self.qname() + '>.')
+                    ' correct index: <' + self.qname() + '>.')
+
+            # Initial value is an expression
+            i = m._state_init[self._index]
+            if not isinstance(i, myokit.Expression):  # pragma: no cover
+                raise myokit.IntegrityError(
+                    'Initial value for <' + self.qname() + '> is not an'
+                    ' expression.')
+
+            # Init: No PartialDerivative or InitialValue operators
+            if i.contains_type(myokit.PartialDerivative):
+                raise myokit.IntegrityError(
+                    'Partial derivatives may not appear in model expressions:'
+                    ' initial value for <' + self.qname() + '>.')
+            if i.contains_type(myokit.InitialValue):
+                raise myokit.IntegrityError(
+                    'Initial values may not appear in model expressions:'
+                    ' initial value for < ' + self.qname() + '>.')
+
+            # Init: Can't evaluate to True or False
+            if isinstance(i, myokit.Condition):
+                raise myokit.IntegrityError(
+                    'The initial value for a variable can not be a'
+                    ' condition: <' + self.qname() + '>.')
+
+            # Init: No nested variables or non-constants
+            for ref in i.references():
+                var = ref.var()
+                if var.is_nested():
+                    raise myokit.IllegalReferenceInInitialValueError(self, ref)
+                if not var.is_constant():
+                    raise myokit.IntegrityError(
+                        'Initial value for variable <' + self.qname() + '> is'
+                        ' not constant: ' + i.code() + '.')
+
         elif is_deriv:  # pragma: no cover
             raise myokit.IntegrityError(
                 'A derivative was set for <' + self.qname() + '> but this is'
                 ' not a state variable.')
 
         # Check for component as parent
         m = self.parent(Component)
```

### Comparing `myokit-1.33.9/myokit/_myokit_version.py` & `myokit-1.34.0/myokit/_myokit_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # Version as a tuple (major, minor, revision)
 #  - Changes to major are rare
 #  - Changes to minor indicate new features, possible slight backwards
 #    incompatibility
 #  - Changes to revision indicate bugfixes, tiny new features
 #  - There is no significance to odd/even numbers
-__version_tuple__ = 1, 33, 9
+__version_tuple__ = 1, 34, 0
 
 # String version of the version number
 __version__ = '.'.join([str(x) for x in __version_tuple__])
 if not __release__:  # pragma: no cover
     __version_tuple__ += ('dev', )
     __version__ += '.dev'
```

### Comparing `myokit-1.33.9/myokit/_parsing.py` & `myokit-1.34.0/myokit/_parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,14 +348,15 @@
         d[token[3]] = (token, obj)
 
 
 class ParseInfo(object):
     def __init__(self):
         self.model = None
         self.initial_values = OrderedDict()
+        self.initial_value_tokens = {}
         self.alias_map = {}
         self.user_functions = {}
 
 
 def parse_model_from_stream(stream, syntax_only=False):
     """
     Parses a model.
@@ -416,18 +417,18 @@
             t2 = expect(next(stream), NAME)
             name = t0[1] + t1[1] + t2[1]
             if name in info.initial_values:
                 raise ParseError(
                     'Duplicate initial value', t0[2], t0[3],
                     'A value for <' + name + '> was already specified.')
             expect(next(stream), EQUAL)
-            expr = parse_expression_stream(stream)
+            expr = parse_proto_expression(stream)
             expect(next(stream), EOL)
             info.initial_values[name] = expr
-            reg_token(info, t0, expr)
+            info.initial_value_tokens[name] = t0
 
         token = stream.peek()
 
     # Save order of state variables
     state_order = list(info.initial_values.keys())
 
     # Parse components
@@ -435,23 +436,14 @@
         parse_component(stream, info)
     expect(stream.peek(), (EOF, BRACKET_OPEN, SEGMENT_HEADER))
 
     # Syntax checking mode
     if syntax_only:
         return True
 
-    # All initial variables must have been used
-    for qname, e in info.initial_values.items():
-        raise ParseError(
-            'Unused initial value', 0, 0,
-            'An unused initial value was found for "' + str(qname) + '".')
-
-    # Re-order the model state
-    model.reorder_state(state_order)
-
     # Order encountered tokens
     m = model._tokens
     model._tokens = {}
     for line in sorted(m.keys()):
         model._tokens[line] = {}
         for char in sorted(m[line].keys()):
             model._tokens[line][char] = m[line][char]
@@ -464,14 +456,31 @@
     for var in model.variables(deep=True):
         if var._proto_rhs is not None:
             # No need to check for IllegalReferenceErrors here, since these
             # won't have been resolved in the first place.
             var.set_rhs(convert_proto_expression(var._proto_rhs, var, info))
         del var._proto_rhs
 
+    # Resolve variable references in initial values
+    for i, var in enumerate(model.states()):
+        e = info.initial_values[var.qname()]
+        expr = convert_proto_expression(e, model, info)
+        var.set_initial_value(expr)
+        del info.initial_values[var.qname()]
+
+    # All initial variables must have been used
+    for qname, e in info.initial_values.items():
+        t = info.initial_value_tokens[qname]
+        raise ParseError(
+            'Unused initial value', t[2], t[3],
+            'An unused initial value was found for "' + qname + '".')
+
+    # Re-order the model state
+    model.reorder_state(state_order)
+
     # Check the semantics of the model
     try:
         model.validate()
     except myokit.IntegrityError as e:
         t = e.token()
         if t:
             raise ParseError('IntegrityError', t[2], t[3], str(e), cause=e)
@@ -671,22 +680,15 @@
 
     # Set initial value for states
     if is_state:
         if not var.qname() in info.initial_values:
             raise ParseError(
                 'Missing initial value', line, char,
                 'No initial value was found for "' + var.qname() + '"')
-        state_value = info.initial_values[var.qname()]
-        try:
-            var.promote(state_value)
-        except myokit.NonLiteralValueError as e:
-            t = state_value._token
-            raise ParseError(
-                'Illegal state value', t[2], t[3], str(e), cause=e)
-        del info.initial_values[var.qname()]
+        var.promote()
 
     # Parse definition, quick unit, bind, label and description syntax
     # These token must occur in a fixed order!
     unit = None
     token = expect(stream.peek(), (EQUAL, IN, BIND, LABEL, COLON, EOL))
     if token[0] == EQUAL:
         # Parse variable definition
```

### Comparing `myokit-1.33.9/myokit/_progress.py` & `myokit-1.34.0/myokit/_progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     Interface for progress updates in Simulations. Also allows some job types
     to be cancelled by the user.
 
     Many simulation types take an argument ``progress`` that can be used to
     pass in an object implementing this interface. The simulation will use this
     object to report on its progress.
 
-    Note that progress reporters should be re-usable, but the behaviour when
+    Note that progress reporters should be re-usable, but the behavior when
     making calls to a reporter from two different processes (either through
     multi-threading/multi-processing or jobs nested within jobs) is undefined.
 
     An optional description of the job to run can be passed in at construction
     time as ``msg``.
     """
     def enter(self, msg=None):
```

### Comparing `myokit-1.33.9/myokit/_protocol.py` & `myokit-1.34.0/myokit/_protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #
-# Defines the python classes that represent a pacing protocol.
+# Defines the python classes that represent pacing protocols.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
 from __future__ import absolute_import, division
 from __future__ import print_function, unicode_literals
 
 import myokit
 
 import numpy as np
 
+from bisect import bisect_right
+
 
 class Protocol(object):
     """
     Represents a pacing protocol as a sequence of :class:`events
     <ProtocolEvent>`.
 
     Every event represents a time span during which the stimulus is non-zero.
@@ -39,15 +41,15 @@
 
     An event with start time ``a`` and duration ``b`` will be active during
     the interval ``[a, b)``. In other words, time ``a`` will be the first time
     it is active and time ``b`` will be the first time after ``a`` at which it
     is not.
 
     Protocols can be compared with ``==``, which will check if the :meth:`code`
-    for both protocols is the same. Protocols can be serialised with
+    for both protocols is the same. Protocols can be serialized with
     ``pickle``.
     """
     def __init__(self):
         super(Protocol, self).__init__()
         self._head = None
 
     def add(self, e):
@@ -846,7 +848,98 @@
     pass
 
 
 class NotAnUnbrokenSequenceError(myokit.MyokitError):
     """ Error raised exclusively by is_unbroken_sequence_exception(). """
     pass
 
+
+class TimeSeriesProtocol(object):
+    """
+    Represents a pacing protocol as a sequence of time value pairs and an
+    interpolation method (currently only linear interpolation is supported).
+
+    A 1D time-series should be given as input. During the simulation, the value
+    of the pacing variable will be determined by interpolating between the two
+    nearest points in the series. If the simulation time is outside the bounds
+    of the time-series, the first or last value in the series will be used.
+
+    Protocols can be compared with ``==``, which will check if the sequence of
+    time value pairs is the same, and the interpolation method is the same.
+    Protocols can be serialized with ``pickle``.
+
+    """
+
+    def __init__(self, times, values, method=None):
+        super(TimeSeriesProtocol, self).__init__()
+
+        if len(times) != len(values):
+            raise ValueError('Times and values array must have same size.')
+        times_tpl, values_tpl = zip(*[
+            (float(t), float(v)) for t, v in sorted(zip(times, values))
+        ])
+        self._times = list(times_tpl)
+        self._values = list(values_tpl)
+
+        if method is None:
+            self._method = 'linear'
+        else:
+            self._method = str(method).lower()
+            if self._method not in ('linear', ):
+                raise ValueError(
+                    'Unknown interpolation method: ' + self._method)
+
+    def __eq__(self, other):
+        if self is other:
+            return True
+        if not isinstance(other, TimeSeriesProtocol):
+            return False
+        return (
+            self._method == other._method
+            and self._values == other._values
+            and self._times == other._times
+        )
+
+    def __getstate__(self):
+        return {
+            'times': self._times,
+            'values': self._values,
+            'method': self._method,
+        }
+
+    def __setstate__(self, values):
+        self._times = values['times']
+        self._values = values['values']
+        self._method = values['method']
+
+    def clone(self):
+        """
+        Returns a clone of this protocol.
+        """
+        return TimeSeriesProtocol(self._times, self._values, self._method)
+
+    def pace(self, t):
+        """
+        Returns the value of the pacing variable at time ``t``.
+        """
+        if t < self._times[0]:
+            return self._values[0]
+        if t > self._times[-1]:
+            return self._values[-1]
+        i = bisect_right(self._times, t) - 1
+        if i == len(self._times) - 1:
+            return self._values[i]
+        return self._values[i] + (t - self._times[i]) * (
+            self._values[i + 1] - self._values[i]
+        ) / (self._times[i + 1] - self._times[i])
+
+    def times(self):
+        """
+        Returns a list of the times in this protocol.
+        """
+        return self._times
+
+    def values(self):
+        """
+        Returns a list of the values in this protocol.
+        """
+        return self._values
```

### Comparing `myokit-1.33.9/myokit/_sim/__init__.py` & `myokit-1.34.0/myokit/_sim/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_sim/cable.c` & `myokit-1.34.0/myokit/_sim/cable.c`

 * *Files 0% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 model.reserve_unique_names(*ansic.keywords)
 model.create_unique_names()
 
 # Get expression writer
 w = ansic.AnsiCExpressionWriter()
 
 # Process bindings, remove unsupported bindings.
-bound_variables = model.prepare_bindings({
+bound_variables = myokit._prepare_bindings(model, {
     'time'         : 'engine_time',
     'pace'         : 'engine_pace',
     'diffusion_current' : 'diffusion_current',
-    })
+})
 
 # Define var/lhs function
 def v(var, pre='cell->'):
     """
     Accepts a variable or a left-hand-side expression and returns its C
     representation.
     """
@@ -275,15 +275,15 @@
 py_sim_clean()
 {
     sim_clean();
     Py_RETURN_NONE;
 }
 
 /*
- * Initialise a run
+ * Initialize a run
  */
 static PyObject*
 sim_init(PyObject *self, PyObject *args)
 {
     #ifdef MYOKIT_DEBUG_MESSAGES
     printf("Initialising.\n");
     #endif
@@ -437,15 +437,15 @@
 for label, eqs in equations.items():
     for eq in eqs.equations(const=True):
         print(tab*2 + w.eq(eq) + ';')
 ?>
         /* Initial values */
 <?
 for var in model.states():
-    print(tab*2 + v(var) + ' = PyFloat_AsDouble(PyList_GetItem(state_in, icell * N_STATE + ' + str(var.indice()) + '));')
+    print(tab*2 + v(var) + ' = PyFloat_AsDouble(PyList_GetItem(state_in, icell * N_STATE + ' + str(var.index()) + '));')
 ?>
         /* Zeros for pacing and diffusion current */
 <?
 var = model.binding('pace')
 if var is not None:
     print(tab*2 + v(var) + ' = 0;')
 var = model.binding('diffusion_current')
@@ -577,15 +577,15 @@
     #ifdef MYOKIT_DEBUG_MESSAGES
     printf("Setting final state.\n");
     #endif
     cell = cells;
     for(icell=0; icell<ncells; icell++) {
 <?
 for var in model.states():
-    print(tab*2 + 'PyList_SetItem(state_out, icell * N_STATE + ' + str(var.indice()) + ', PyFloat_FromDouble(' + v(var) + '));')
+    print(tab*2 + 'PyList_SetItem(state_out, icell * N_STATE + ' + str(var.index()) + ', PyFloat_FromDouble(' + v(var) + '));')
 ?>
         cell++;
     }
 
     #ifdef MYOKIT_DEBUG_MESSAGES
     printf("Done, tidying up and returning.\n");
     #endif
```

### Comparing `myokit-1.33.9/myokit/_sim/cable.py` & `myokit-1.34.0/myokit/_sim/cable.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     This simulation provides the following inputs variables can bind to:
 
     ``time``
         The simulation time
     ``pace``
         The pacing level, this is set if a protocol was passed in.
     ``diffusion_current``
-        The current flowing from the cell to its neighbours. This will be
+        The current flowing from the cell to its neighbors. This will be
         positive when the cell is acting as a source, negative when it is
         acting as a sink.
 
     The variable ``time`` is set globally, meaning each cell uses the same
     value. The variables ``pace`` and ``diffusion_current`` have different
     values per cell. The number of paced cell can be set with
     :meth:`set_paced_cells`.
@@ -73,15 +73,15 @@
     allows you to pre-pace, run a simulation, reset to the pre-paced state, run
     another simulation etc.
 
     The ``diffusion_current`` is calculated as::
 
         i = sum[g * (V - V_j)]
 
-    Where the sum is taken over all neighbouring cells j (see [1]).
+    Where the sum is taken over all neighboring cells j (see [1]).
 
     The resulting ODE system is solved using a forward Euler (FE) method with
     fixed step sizes. Smaller step sizes lead to more accurate results, and it
     is recommended any important results are double-checked by re-running with
     a reduced step size. Any states written in a Hodgkin-Huxley form can be
     updated using Rush-Larsen steps (see [2]), by setting ``rl=True``. This
     often increases stability (allowing for larger step sizes) but can reduce
@@ -172,15 +172,15 @@
         if self._model.binding('diffusion_current') is None:
             raise ValueError(
                 'This simulation requires a variable to be bound to'
                 ' "diffusion_current" to pass current from one cell to the'
                 ' next')
 
         # Set state and default state
-        self._state = self._model.state() * ncells
+        self._state = self._model.initial_values(True) * ncells
         self._default_state = list(self._state)
 
         # Unique simulation id
         Simulation1d._index += 1
         module_name = 'myokit_sim1d_' + str(Simulation1d._index)
         module_name += '_' + str(myokit.pid_hash())
```

### Comparing `myokit-1.33.9/myokit/_sim/cmodel.h` & `myokit-1.34.0/myokit/_sim/cmodel.h`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 Model variables are divided into several (non-overlapping) groups:
 
 States:
     Independent variables, varied during integration.
 State derivatives:
     Calculated by the model.
 Bound variables:
-    External inputs to the model (e.g. time and pacing).
+    External inputs to the model (e.g. time and pacing). There are an arbitrary
+    number of these, and the model stores the current value of each
 Intermediary variables:
     The remaining variables that depend on state variables.
 Constants:
     The remaining variables that don't.
 
 Constants are further divided into four (non-overlapping) groups:
 
@@ -149,27 +150,27 @@
 =======
 A model can log the value of its variables to a Python dict that maps (fully
 qualified) variable names to sequence types (e.g. lists). Typically, this dict
 will be a myokit.DataLog.
 
 Methods:
 
-Model_InitialiseLogging(Model model, PyObject* log_dict)
+Model_InitializeLogging(Model model, PyObject* log_dict)
     Sets up logging for all variables used as keys in log_dict (assuming fully
     qualified names). Will raise an error if the dict contains keys that do not
     correspond to model variables. The values in the dict should implement the
     sequence interface (and in particular, have an "append" method).
 
 Model_Log(model)
     If logging has been set up, this will log the current values of variables
     to the sequences in the log dict.
 
-Model_DeInitialiseLogging(model)
-    De-initialises logging. This only needs to be called if logging needs to be
-    set up differently, i.e. before a new call to Model_InitialiseLogging.
+Model_DeInitializeLogging(model)
+    De-initializes logging. This only needs to be called if logging needs to be
+    set up differently, i.e. before a new call to Model_InitializeLogging.
 
 Logging sensitivities
 =====================
 Logging of sensitivity outputs is slightly more primitive than variable
 logging, and consists of a single method - no initialisation is needed.
 
 Model_LogSensitivityMatrix(Model model, PyObject* list)
@@ -203,21 +204,23 @@
  */
 typedef int Model_Flag;
 #define Model_OK                             0
 #define Model_OUT_OF_MEMORY                 -1
 /* General */
 #define Model_INVALID_MODEL                 -100
 /* Logging */
-#define Model_LOGGING_ALREADY_INITIALISED   -200
-#define Model_LOGGING_NOT_INITIALISED       -201
+#define Model_LOGGING_ALREADY_INITIALIZED   -200
+#define Model_LOGGING_NOT_INITIALIZED       -201
 #define Model_UNKNOWN_VARIABLES_IN_LOG      -202
 #define Model_LOG_APPEND_FAILED             -203
 /* Logging sensitivities */
 #define Model_NO_SENSITIVITIES_TO_LOG       -300
 #define Model_SENSITIVITY_LOG_APPEND_FAILED -303
+/* Pacing */
+#define Model_INVALID_PACING                -400
 
 /* Caching doesn't help much when running without jacobians etc., so disabled
    for now
 #define Model_CACHING
 */
 
 /*
@@ -236,34 +239,36 @@
     case Model_OUT_OF_MEMORY:
         PyErr_SetString(PyExc_Exception, "CModel error: Memory allocation failed.");
         break;
     case Model_INVALID_MODEL:
         PyErr_SetString(PyExc_Exception, "CModel error: Invalid model pointer provided.");
         break;
     /* Logging */
-    case Model_LOGGING_ALREADY_INITIALISED:
-        PyErr_SetString(PyExc_Exception, "CModel error: Logging initialised twice.");
+    case Model_LOGGING_ALREADY_INITIALIZED:
+        PyErr_SetString(PyExc_Exception, "CModel error: Logging initialized twice.");
         break;
-    case Model_LOGGING_NOT_INITIALISED:
-        PyErr_SetString(PyExc_Exception, "CModel error: Logging not initialised.");
+    case Model_LOGGING_NOT_INITIALIZED:
+        PyErr_SetString(PyExc_Exception, "CModel error: Logging not initialized.");
         break;
     case Model_UNKNOWN_VARIABLES_IN_LOG:
         PyErr_SetString(PyExc_Exception, "CModel error: Unknown variables found in logging dictionary.");
         break;
     case Model_LOG_APPEND_FAILED:
         PyErr_SetString(PyExc_Exception, "CModel error: Call to append() failed on logging list.");
         break;
     /* Logging sensitivities */
     case Model_NO_SENSITIVITIES_TO_LOG:
         PyErr_SetString(PyExc_Exception, "CModel error: Sensivity logging called, but sensitivity calculations were not enabled.");
         break;
     case Model_SENSITIVITY_LOG_APPEND_FAILED:
         PyErr_SetString(PyExc_Exception, "CModel error: Call to append() failed on sensitivity matrix logging list.");
         break;
-
+    case Model_INVALID_PACING:
+        PyErr_SetString(PyExc_Exception, "CModel error: Invalid pacing provided.");
+        break;
     /* Unknown */
     default:
         PyErr_Format(PyExc_Exception, "CModel error: Unlisted error %d", (int)flag);
         break;
     };
 }
 
@@ -273,17 +278,20 @@
 struct Model_Memory {
     /* If this is an ODE model this will be 1, otherwise 0. */
     int is_ode;
 
     /* If this model has sensitivities this will be 1, otherwise 0. */
     int has_sensitivities;
 
+    /* Pacing */
+    realtype *pace_values;
+    int n_pace;
+
     /* Bound variables */
     realtype time;
-    realtype pace;
     realtype realtime;
     realtype evaluations;
 
     /* State variables and derivatives */
     int n_states;
     realtype* states;
     realtype* derivatives;
@@ -322,16 +330,16 @@
     realtype* s_states;
 
     /* Sensitivity of intermediary variables needed to calculate remaining
        sensitivities. */
     int ns_intermediary;
     realtype* s_intermediary;
 
-    /* Logging initialised? */
-    int logging_initialised;
+    /* Logging initialized? */
+    int logging_initialized;
 
     /* Which variables are we logging? */
     int logging_states;
     int logging_derivatives;
     int logging_intermediary;
     int logging_bound;
 
@@ -441,14 +449,49 @@
     if (model == NULL) return Model_INVALID_MODEL;
     Model__InvalidateCache(model);
     #endif
     return Model_OK;
 }
 
 /*
+ * Sets up (i.e. allocates memory for) array of protocol-determined values
+ *
+ * Arguments
+ *  n_pace: the number of pacing values to use.
+ *
+ * Returns a model flag.
+ *
+ */
+Model_Flag
+Model_SetupPacing(Model model, int n_pace)
+{
+    if (model == NULL) return Model_INVALID_MODEL;
+    if (n_pace < 0) return Model_INVALID_PACING;
+
+    /* Free any existing pacing */
+    if (model->n_pace > 0) {
+        free(model->pace_values);
+    }
+
+    /* Allocate new pacing */
+    model->n_pace = n_pace;
+    model->pace_values = (realtype*)malloc((size_t)n_pace * sizeof(realtype));
+    if (model->pace_values == NULL) {
+        return Model_OUT_OF_MEMORY;
+    }
+
+    /* Clear values */
+    for (int i = 0; i < n_pace; i++) {
+        model->pace_values[i] = 0;
+    }
+
+    return Model_OK;
+}
+
+/*
  * (Re)calculates the values of all constants that are derived from other
  * constants.
  *
  * Calling this method does not affect the model cache.
  *
  * Arguments
  *  model : The model to update.
@@ -499,47 +542,47 @@
  *  - the parameter-derived variables are recalculated.
  *
  * Arguments
  *  model : The model whose variables to set
  *  literals : An array of size model->n_literals
  *
  * Returns a model flag.
- */
+ *
 Model_Flag
 Model_SetLiteralVariables(Model model, const realtype* literals)
 {
     int i;
     if (model == NULL) return Model_INVALID_MODEL;
 
-    /* Scan for changes */
+    * Scan for changes *
     i = 0;
     #ifdef Model_CACHING
     if (Model__ValidCache(model)) {
         for (i=0; i<model->n_literals; i++) {
             if (model->literals[i] != literals[i]) {
                 break;
             }
         }
     }
     #endif
 
-    /* Update remaining */
+    * Update remaining *
     if (i < model->n_literals) {
         for (; i<model->n_literals; i++) {
             model->literals[i] = literals[i];
         }
         #ifdef Model_CACHING
         Model__InvalidateCache(model);
         #endif
         Model_EvaluateLiteralDerivedVariables(model);
         Model_EvaluateParameterDerivedVariables(model);
     }
 
     return Model_OK;
-}
+}*/
 
 /*
  * Updates the parameter variables to the values given in `parameters`.
  *
  * If any of the values are changed
  *  - the model caches are cleared.
  *  - the parameter-derived variables are recalculated.
@@ -653,48 +696,58 @@
  * changed.
  *
  * Returns a model flag.
  */
 Model_Flag
 Model_SetBoundVariables(
     Model model,
-    const realtype time, const realtype pace,
-    const realtype realtime, const realtype evaluations)
+    const realtype time,
+    const realtype *pace_values,
+    const realtype realtime,
+    const realtype evaluations)
 {
+    #ifdef Model_CACHING
     int changed;
+    #endif
     if (model == NULL) return Model_INVALID_MODEL;
 
+    #ifdef Model_CACHING
     changed = 0;
+    #endif
     if (time != model->time) {
         model->time = time;
+        #ifdef Model_CACHING
         changed = 1;
+        #endif
+    }
+
+    for (int i = 0; i < model->n_pace; i++) {
+        if (pace_values[i] != model->pace_values[i]) {
+            model->pace_values[i] = pace_values[i];
+            #ifdef Model_CACHING
+            changed = 1;
+            #endif
+        }
     }
 
-<?
-if model.binding('pace') is not None:
-    print(tab + 'if (pace != model->pace) {')
-    print(tab + '    model->pace = pace;')
-    print(tab + '    changed = 1;')
-    print(tab + '}')
-?>
     #ifdef Model_CACHING
     if (changed) {
         Model__InvalidateCache(model);
     }
     #endif
 
     /* Update unchecked variables */
     model->realtime = realtime;
     model->evaluations = evaluations;
 
     return Model_OK;
 }
 
 /*
- * Updates the state variables to the values given in `states`.
+ * Updates the state variables to the float values given in `states`.
  *
  * If any of the values are changed, the model caches are cleared.
  *
  * Arguments
  *  model : The model whose variables to set
  *  states : An array of size model->n_states
  *
@@ -867,15 +920,15 @@
  *
  * Note: The variable names are all ascii compatible. In Python2, the strings
  * inside log_dict are either unicode or bytes, but they can be matched
  * without conversion.
  *
  * Arguments
  *  log_dict : A dictionary mapping variable names to sequences.
- *  i : The next indice to add logs and vars.
+ *  i : The next index to add logs and vars.
  *  name : The name to check.
  *  var : A pointer to the variable.
  *
  * Returns 1 if added, 0 if not.
  */
 int
 Model__AddVariableToLog(
@@ -889,38 +942,38 @@
 
     model->_log_lists[i] = val;
     model->_log_vars[i] = (realtype*)variable;
     return 1;
 }
 
 /*
- * Initialises logging, using the given dict. An error is returned if logging
- * is already initialised.
+ * Initializes logging, using the given dict. An error is returned if logging
+ * is already initialized.
  *
  * Arguments
- *  model : The model whose logging system to initialise.
+ *  model : The model whose logging system to initialize.
  *  log_dict : A Python dict mapping fully qualified variable names to sequence
  *             objects to log in.
  *
  * Returns a model flag
  */
 Model_Flag
-Model_InitialiseLogging(Model model, PyObject* log_dict)
+Model_InitializeLogging(Model model, PyObject* log_dict)
 {
     int i, j;
 
     if (model == NULL) return Model_INVALID_MODEL;
-    if (model->logging_initialised) return Model_LOGGING_ALREADY_INITIALISED;
+    if (model->logging_initialized) return Model_LOGGING_ALREADY_INITIALIZED;
 
     /* Number of variables to log */
-    model->n_logged_variables = PyDict_Size(log_dict);
+    model->n_logged_variables = (int)PyDict_Size(log_dict);
 
     /* Allocate pointer lists */
-    model->_log_lists = (PyObject**)malloc(sizeof(PyObject*) * model->n_logged_variables);
-    model->_log_vars = (realtype**)malloc(sizeof(realtype*) * model->n_logged_variables);
+    model->_log_lists = (PyObject**)malloc((size_t)model->n_logged_variables * sizeof(PyObject*));
+    model->_log_vars = (realtype**)malloc((size_t)model->n_logged_variables * sizeof(realtype*));
 
     /* Check states */
     i = 0;
 <?
 for var in model.states():
     print(tab + 'i += Model__AddVariableToLog(model, log_dict, i, "' + var.qname() + '", &' + v(var)  + ');')
 ?>
@@ -955,57 +1008,57 @@
 
     /* Create "append" string. */
     if (model->_list_update_string == NULL) {
         model->_list_update_string = PyUnicode_FromString("append");
     }
 
     /* All done! */
-    model->logging_initialised = 1;
+    model->logging_initialized = 1;
     return Model_OK;
 }
 
 /*
- * De-initialises logging, undoing the effects of Model_InitialiseLogging() and
- * allowing logging to be initialised again.
+ * De-initializes logging, undoing the effects of Model_InitializeLogging() and
+ * allowing logging to be initialized again.
  *
  * Arguments
- *  model : The model whos logging to deinitialise.
+ *  model : The model whos logging to deinitialize.
  *
  * Returns a model flag.
  */
 Model_Flag
-Model_DeInitialiseLogging(Model model)
+Model_DeInitializeLogging(Model model)
 {
     if (model == NULL) return Model_INVALID_MODEL;
-    if (!model->logging_initialised) return Model_LOGGING_NOT_INITIALISED;
+    if (!model->logging_initialized) return Model_LOGGING_NOT_INITIALIZED;
 
     /* Free memory */
     if (model->_log_vars != NULL) {
         free(model->_log_vars);
         model->_log_vars = NULL;
     }
     if (model->_log_lists != NULL) {
         free(model->_log_lists);
         model->_log_lists = NULL;
     }
 
     /* Reset */
-    model->logging_initialised = 0;
+    model->logging_initialized = 0;
     model->n_logged_variables = 0;
     model->logging_states = 0;
     model->logging_derivatives = 0;
     model->logging_intermediary = 0;
     model->logging_bound = 0;
 
     return Model_OK;
 }
 
 /*
  * Logs the current state of the model to the logging dict passed in to
- * Model_InitialiseLogging.
+ * Model_InitializeLogging.
  *
  * Note: This method does not update the state in any way, e.g. to make sure
  * that what is logged is sensible.
  *
  * Arguments
  *  model : The model whose state to log
  *
@@ -1014,15 +1067,15 @@
 Model_Flag
 Model_Log(Model model)
 {
     int i;
     PyObject *val, *ret;
 
     if (model == NULL) return Model_INVALID_MODEL;
-    if (!model->logging_initialised) return Model_LOGGING_NOT_INITIALISED;
+    if (!model->logging_initialized) return Model_LOGGING_NOT_INITIALIZED;
 
     for (i=0; i<model->n_logged_variables; i++) {
         val = PyFloat_FromDouble(*(model->_log_vars[i]));
         ret = PyObject_CallMethodObjArgs(model->_log_lists[i], model->_list_update_string, val, NULL);
         Py_DECREF(val);
         Py_XDECREF(ret);
         if (ret == NULL) {
@@ -1033,34 +1086,35 @@
     return Model_OK;
 }
 
 /*
  * Creates a matrix of sensitivities and adds it to a Python sequence.
  *
  * The created matrix is a (Python) tuple of tuples, where the first (outer)
- * indice is for the dependent variable (y in dy/dx) and the second (inner)
- * indice is for the independent variable (x in dy/dx).
+ * index is for the dependent variable (y in dy/dx) and the second (inner)
+ * index is for the independent variable (x in dy/dx).
  *
  * model : The model whose sensitivities to log (must have sensitivity
  *         calculations enabled).
  * list : A PyList to add the newly created matrix of sensitivities to.
  *
  * Returns a model flag.
  */
 Model_Flag
 Model_LogSensitivityMatrix(Model model, PyObject* list)
 {
     PyObject *l1, *l2;
-    PyObject *val;
     int flag;
+    <?= 'PyObject *val;' if s_dependents else '' ?>
 
     if (model == NULL) return Model_INVALID_MODEL;
 
     /* Create outer tuple */
     l1 = PyTuple_New(model->ns_dependents);
+    l2 = NULL;  /* Removes "may be unitialized" error */
     if (l1 == NULL) goto nomem;
 
     /* Note that PyTuple_SetItem steals a reference */
 <?
 for i, e1 in enumerate(s_dependents):
     var = e1.var()
     print('')
@@ -1115,70 +1169,74 @@
 
     /*
      * Variables
      */
 
     /* States and derivatives */
     model->n_states = <?= model.count_states() ?>;
-    model->states = (realtype*)malloc(model->n_states * sizeof(realtype));
-    model->derivatives = (realtype*)malloc(model->n_states * sizeof(realtype));
+    model->states = (realtype*)malloc((size_t)model->n_states * sizeof(realtype));
+    model->derivatives = (realtype*)malloc((size_t)model->n_states * sizeof(realtype));
 
     /* Intermediary variables */
     model->n_intermediary = <?= model.count_variables(inter=True, deep=True) ?>;
-    model->intermediary = (realtype*)malloc(model->n_intermediary * sizeof(realtype));
+    model->intermediary = (realtype*)malloc((size_t)model->n_intermediary * sizeof(realtype));
 
     /* Parameters */
     model->n_parameters = <?= len(parameters) ?>;
     model->n_parameter_derived = <?= len(parameter_derived) ?>;
-    model->parameters = (realtype*)malloc(model->n_parameters * sizeof(realtype));
-    model->parameter_derived = (realtype*)malloc(model->n_parameter_derived * sizeof(realtype));
+    model->parameters = (realtype*)malloc((size_t)model->n_parameters * sizeof(realtype));
+    model->parameter_derived = (realtype*)malloc((size_t)model->n_parameter_derived * sizeof(realtype));
+
+    /* Pacing */
+    model->n_pace = 0;
+    model->pace_values = NULL;
 
     /* Literals */
     model->n_literals = <?= len(literals) ?>;
     model->n_literal_derived = <?= len(literal_derived) ?>;
-    model->literals = (realtype*)malloc(model->n_literals * sizeof(realtype));
-    model->literal_derived = (realtype*)malloc(model->n_literal_derived * sizeof(realtype));
+    model->literals = (realtype*)malloc((size_t)model->n_literals * sizeof(realtype));
+    model->literal_derived = (realtype*)malloc((size_t)model->n_literal_derived * sizeof(realtype));
 
     /*
      * Sensitivities
      */
 
     /* Total number of dependents to output sensitivities of */
     model->ns_dependents = <?= len(s_dependents) ?>;
 
     /* Total number of independent to calculate sensitivities w.r.t. */
     model->ns_independents = <?= len(s_independents) ?>;
 
     /* Pointers to independent variables */
     /* Note that, for sensitivities w.r.t. initial values, the entry in this
        list points to the _current_, not the initial value. */
-    model->s_independents = (realtype**)malloc(model->ns_independents * sizeof(realtype));
+    model->s_independents = (realtype**)malloc((size_t)model->ns_independents * sizeof(realtype));
 <?
 for i, expr in enumerate(s_independents):
     print(tab + 'model->s_independents[' + str(i) + '] = &' + v(expr.var()) + ';')
 ?>
     /* Type of independents (1 for parameter, 0 for initial) */
-    model->s_is_parameter = (int*)malloc(model->ns_independents * sizeof(int));
+    model->s_is_parameter = (int*)malloc((size_t)model->ns_independents * sizeof(int));
 <?
 for i, expr in enumerate(s_independents):
     print(tab + 'model->s_is_parameter[' + str(i) + '] = ' + str(1 if isinstance(expr, myokit.Name) else 0) + ';')
 ?>
     /* Sensitivities of state variables */
-    model->s_states = (realtype*)malloc(model->n_states * model->ns_independents * sizeof(realtype));
+    model->s_states = (realtype*)malloc((size_t)(model->n_states * model->ns_independents) * sizeof(realtype));
 
     /* Sensitivities of intermediary variables needed in calculations */
     model->ns_intermediary = <?= sum(len(x) for x in s_output_equations) ?>;
-    model->s_intermediary = (realtype*)malloc(model->ns_intermediary * sizeof(realtype));
+    model->s_intermediary = (realtype*)malloc((size_t)model->ns_intermediary * sizeof(realtype));
 
     /*
      * Logging
      */
 
     /* Logging configured? */
-    model->logging_initialised = 0;
+    model->logging_initialized = 0;
     model->n_logged_variables = 0;
 
     /* Logged variables and logged types */
     model->logging_states = 0;
     model->logging_derivatives = 0;
     model->logging_intermediary = 0;
     model->logging_bound = 0;
@@ -1190,17 +1248,16 @@
     model->_log_lists = NULL;
     model->_log_vars = NULL;
 
     /*
      * Default values
      */
 
-    /* Bound variables */
+    /* Bound variables (except pacing) */
     model->time = 0;
-    model->pace = 0;
     model->realtime = 0;
     model->evaluations = 0;
 
     /* Literal values */
 <?
 for eq in literals.values():
     print(tab + w.eq(eq) + ';')
@@ -1218,31 +1275,31 @@
 ?>
     flag = Model_EvaluateParameterDerivedVariables(model);
     if (flag != Model_OK) {
         if (flagp != NULL) { *flagp = flag; }
         return NULL;
     }
 
-    /* States */
+    /* State values */
 <?
 for var in model.states():
-    print(tab + v(var) + ' = ' + myokit.float.str(var.state_value()) + ';')
+    print(tab + v(var) + ' = ' + myokit.float.str(var.initial_value(True)) + ';')
 ?>
     /*
      * Caching.
      * At this point, we don't have derivatives or sensitivity outputs, so
      * both cache flags are set to invalid.
      */
     #ifdef Model_CACHING
     model->valid_cache_derivatives = 0;
     model->valid_cache_sensitivity_outputs = 0;
     #endif
 
     /*
-     * Finalise
+     * Finalize
      */
 
     /* Set flag to indicate success */
     if (flagp != NULL) { *flagp = Model_OK; }
 
     /* Return newly created model */
     return model;
```

### Comparing `myokit-1.33.9/myokit/_sim/cmodel.py` & `myokit-1.34.0/myokit/_sim/cmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
         cmodel = CModel(model)
         print(cmodel.code)
 
     Arguments:
 
     ``model``
         A :class:`myokit.Model`.
+    ``pacing_labels``
+        A list of ``str`` variable labels, each corresponding to a paced
+        variable.
     ``sensitivities``
         Either ``None`` or a tuple ``(dependents, independents)``. See
         :class:`myokit.Simulation` for details.
 
     The following properties are all public for easy access. But note that they
     do not interact with the compiled header so changing them will have little
     effect.
@@ -72,35 +75,33 @@
     ``literals``
         Constants that do not depend on any other constants (and are not
         parameters).
     ``literal_derived``
         Constants that depend on literals, but not on parameters.
 
     """
-    def __init__(self, model, sensitivities):
+    def __init__(self, model, pacing_labels, sensitivities):
 
         # Parse sensitivity arguments
         has_sensitivities, dependents, independents = \
             self._parse_sensitivities(model, sensitivities)
 
         # Set unique names in model: variable names will be prepended so don't
         # bother with keywords.
         model.create_unique_names()
 
-        # Remove any unused bindings, and get mapping from variables to C
-        # variable names as used in model.h
-        #TODO: Think about best way to do this for model re-use with different
-        # sets of bound variables... Presumably the model would simply support
-        # all bindings used by any of the simulations based on model.h ?
-        bound_variables = model.prepare_bindings({
+        # Get mapping from variables to C variable names as used in model.h
+        labels = {
             'time': 'time',
-            'pace': 'pace',
             'realtime': 'realtime',
             'evaluations': 'evaluations',
-        })
+        }
+        for i, label in enumerate(pacing_labels):
+            labels[label] = 'pace_values[' + str(i) + ']'
+        bound_variables = myokit._prepare_bindings(model, labels)
 
         # Get equations in solvable order (grouped by component)
         equations = model.solvable_order()
 
         # Derive sensitivity equations
         if has_sensitivities:
             output_equations = self._derive_sensitivity_equations(
@@ -397,15 +398,15 @@
     def _generate_code(
             self, model, equations, bound_variables, dependents, independents,
             output_equations, literals, literal_derived, parameters,
             parameter_derived, v, w):
         """ Generates and returns the model code. """
 
         # Get states whose initial value is used in sensivitity calculations
-        initials = [p.var().indice() for p in independents
+        initials = [p.var().index() for p in independents
                     if isinstance(p, myokit.InitialValue)]
 
         # Arguments
         args = {
             'model': model,
             'equations': equations,
             'bound_variables': bound_variables,
```

### Comparing `myokit-1.33.9/myokit/_sim/compiler.c` & `myokit-1.34.0/myokit/_sim/compiler.c`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_sim/compiler.py` & `myokit-1.34.0/myokit/_sim/compiler.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_sim/cvodesim.c` & `myokit-1.34.0/myokit/_sim/cvodessim.c`

 * *Files 20% similar despite different names*

```diff
@@ -1,127 +1,92 @@
 <?
-# cvodesim.c
+# cvodessim.c
 #
-# A pype template for a single cell CVODE-based simulation.
+# A pype template for a single cell CVODES-based simulation that can calculate
+# sensitivities of variables ``v`` w.r.t. parameters or initial conditions and
+# perform root-finding.
+#
+# Note: For compatibility with older Python versions on windows, we need to
+# stick to a slightly outdated C standard (i.e. C90). For a list of which
+# microsoft compilers accept which C standard (and how that matches with python
+# versions), see https://bugs.python.org/issue42380
 #
 # Required variables
 # -----------------------------------------------------------------------------
-# module_name A module name
-# model       A myokit model
-# potential   A variable from the model used to track threshold crossings
+# module_name     A module name
+# model_code      Code for a CModel
 # -----------------------------------------------------------------------------
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
 import myokit
-import myokit.formats.ansic as ansic
-
-# Get model
-model.reserve_unique_names(*ansic.keywords)
-model.create_unique_names()
-
-# Get expression writer
-w = ansic.AnsiCExpressionWriter()
-
-# Define lhs function
-def v(var):
-    # Explicitly asking for derivative?
-    if isinstance(var, myokit.Derivative):
-        return 'NV_Ith_S(ydot, ' + str(var.var().indice()) + ')'
-    # Name given? get variable object from name
-    if isinstance(var, myokit.Name):
-        var = var.var()
-    # Handle states
-    if var.is_state():
-        return 'NV_Ith_S(y, ' + str(var.indice()) + ')'
-    # Handle constants and intermediary variables
-    if var.is_constant():
-        return 'AC_' + var.uname()
-    else:
-        return 'AV_' + var.uname()
-w.set_lhs_function(v)
-
-# Tab
-tab = '    '
-
-# Get mapping of bound variables to internal refs, set the RHS of unbound variables
-# to zero and remove any unsupported bindings.
-bound_variables = model.prepare_bindings({
-    'time'        : 't',
-    'pace'        : 'engine_pace',
-    'realtime'    : 'engine_realtime',
-    'evaluations' : 'engine_evaluations',
-    })
-#
-# About the bindings:
-#
-# Time is bound to "t", the time variable used in the function. This is
-#  required for periodic logging and point-list logging, when "tlog" increases
-#  while engine_time stays fixed at the current solver time.
-# Pace is bound to engine_pace, since the solver always visits the points where
-#  its value changes the same problem as with logging "engine_time" doesn't
-#  occur.
-# Realtime is only useful without variable logging, so again binding to global
-#  is ok.
-# Evaluations may increase during interpolation, but this evaluation will be
-#  taken into account in the global variable "engine_evaluations", so this is
-#  fine.
-#
-
-# Get equations
-equations = model.solvable_order()
 ?>
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 #include <stdio.h>
-#include <math.h>
-#include <string.h>
 
-#include <cvode/cvode.h>
+#include <cvodes/cvodes.h>
 #include <nvector/nvector_serial.h>
 #include <sundials/sundials_types.h>
 #include <sundials/sundials_config.h>
 #ifndef SUNDIALS_VERSION_MAJOR
     #define SUNDIALS_VERSION_MAJOR 2
 #endif
 #if SUNDIALS_VERSION_MAJOR >= 3
     #include <sunmatrix/sunmatrix_dense.h>
     #include <sunlinsol/sunlinsol_dense.h>
-    #include <cvode/cvode_direct.h>
+    #include <cvodes/cvodes_direct.h>
 #else
-    #include <cvode/cvode_dense.h>
+    #include <cvodes/cvodes_dense.h>
 #endif
 
+<?
+if myokit.DEBUG_SM:
+    print('// Show debug output')
+    print('#ifndef MYOKIT_DEBUG_MESSAGES')
+    print('#define MYOKIT_DEBUG_MESSAGES')
+    print('#endif')
+
+# Note: When adding profiling messages, write them in past tense so that we can
+# show time elapsed for an operation **that has just completed**.
+if myokit.DEBUG_SP:
+    print('// Show profiling messages')
+    print('#ifndef MYOKIT_DEBUG_PROFILING')
+    print('#define MYOKIT_DEBUG_PROFILING')
+    print('#endif')
+?>
+
 #include "pacing.h"
 
-#define N_STATE <?= model.count_states() ?>
-#define USE_CVODE <?= 1 if model.count_states() > 0 else 0 ?>
+<?= model_code ?>
 
-/* Pacing */
-ESys epacing;               /* Event-based pacing system */
-FSys fpacing;               /* Fixed-form pacing system */
+/*
+ * Define type for "user data" that will hold parameter values if doing
+ * sensitivity analysis.
+ */
+typedef struct {
+    realtype *p;
+} *UserData;
 
 /*
- * Check sundials flags, set python error
+ * Check sundials flags, set python error.
  *  flagvalue : The value to check
  *  funcname : The name of the function that returned the flag
  *  opt : Mode selector
  *         0 : Error if the flag is null
  *         1 : Error if the flag is < 0
  *         2 : Errir
  */
-static int
+int
 check_cvode_flag(void *flagvalue, char *funcname, int opt)
 {
     if (opt == 0 && flagvalue == NULL) {
         /* Check if sundials function returned null pointer */
-        char str[200];
-        sprintf(str, "%s() failed - returned NULL pointer", funcname);
-        PyErr_SetString(PyExc_Exception, str);
+        PyErr_Format(PyExc_Exception, "%s() failed - returned NULL pointer", funcname);
         return 1;
     } else if (opt == 1) {
         /* Check if flag < 0 */
         int flag = *((int*)flagvalue);
         if (flag < 0) {
             if (strcmp(funcname, "CVode") == 0) {
                 switch (flag) {
@@ -181,406 +146,502 @@
                     break;
                 case -26:
                     PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -26 CV_BAD_DKY: The output derivative vector is NULL.");
                     break;
                 case -27:
                     PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -27 CV_TOO_CLOSE: The output and initial times are too close to each other.");
                     break;
-                default: {
-                     /* Note: Brackets are required here, default: should be followed by
-                        a _statement_ and char str[200]; is technically not a statement... */
-                    char str[200];
-                    sprintf(str, "Function CVode() failed with unknown flag = %d", flag);
-                    PyErr_SetString(PyExc_Exception, str);
-                }}
+                default:
+                    PyErr_Format(PyExc_Exception, "Function CVode() failed with unknown flag = %d", flag);
+                }
             } else {
-                char str[200];
-                sprintf(str, "%s() failed with flag = %d", funcname, flag);
-                PyErr_SetString(PyExc_Exception, str);
+                PyErr_Format(PyExc_Exception, "%s() failed with flag = %d", funcname, flag);
             }
             return 1;
         }
     }
     return 0;
 }
 
 /*
- * Declare intermediary, temporary and system variables
+ * Error and warning message handler for CVODES.
+ * Error messages are already set via check_cvode_flag, so this method
+ * suppresses error messages.
+ * Warnings are passed to Python's warning system, where they can be
+ * caught or suppressed using the warnings module.
  */
-static realtype engine_time = 0;        /* Engine time */
-static realtype engine_time_last = 0;   /* Previous engine time */
-static realtype engine_pace = 0;
-static realtype engine_realtime = 0;
-static realtype engine_starttime = 0;
-static realtype rootfinding_threshold = 0;
-static long engine_evaluations = 0;
-static long engine_steps = 0;
-<?
-for var in model.variables(state=False, deep=True):
-    if var.is_literal():
-        print('static realtype ' + v(var) + ' = ' + myokit.float.str(var.rhs().eval()) + ';')
-    else:
-        print('static realtype ' + v(var) + ';')
-?>
+void
+ErrorHandler(int error_code, const char *module, const char *function,
+             char *msg, void *eh_data)
+{
+    char errstr[1024];
+    if (error_code > 0) {
+        sprintf(errstr, "CVODES: %s", msg);
+        PyErr_WarnEx(PyExc_RuntimeWarning, errstr, 1);
+        /* Python 3.2+: PyErr_WarnFormat(PyExc_RuntimeWarning, 1, "CVODES: %s", msg); */
+    }
+}
+
 /*
- * Set values of calculated constants
+ * Initialisation status.
+ * Proper sequence is init(), repeated step() calls till finished, then clean.
  */
-static void
-updateConstants(void)
-{
-<?
-for label, eqs in equations.items():
-    for eq in eqs.equations(const=True):
-        if not eq.rhs.is_literal():
-            print(tab + w.eq(eq) + ';')
-?>}
+int initialized = 0; /* Has the simulation been initialized */
 
 /*
- * Right-hand-side function of the model ODE
+ * Model
  */
-static int
-rhs(realtype t, N_Vector y, N_Vector ydot, void *f_data)
-{
-    /* Fixed-form pacing? Then look-up correct value of pacing variable! */
-    FSys_Flag flag_fpacing;
-    if (fpacing != NULL) {
-        engine_pace = FSys_GetLevel(fpacing, t, &flag_fpacing);
-        if (flag_fpacing != FSys_OK) { /* This should never happen */
-            FSys_SetPyErr(flag_fpacing);
-            return -1;  /* Negative value signals irrecoverable error to CVODE */
-        }
-    }
-<?
-for label, eqs in equations.items():
-    if eqs.has_equations(const=False):
-        print(tab + '/* ' + label + ' */')
-        for eq in eqs.equations(const=False):
-            var = eq.lhs.var()
-            try:
-                print(tab + v(var) + ' = ' + bound_variables[var] + ';')
-            except KeyError:
-                print(tab + w.eq(eq) + ';')
-        print(tab)
-?>
-    engine_evaluations++;
-    return 0;
-}
+Model model;        /* A model object */
 
 /*
- * Right-hand-side function, bound variables only
+ * Pacing
  */
-static int
-update_bindings(realtype t, N_Vector y, N_Vector ydot, void *f_data)
-{
-<?
-for var, internal in bound_variables.items():
-    print(tab + v(var) + ' = ' + internal + ';')
-?>
-    return 0;
-}
+union PSys {
+    ESys event;
+    FSys fixed;
+};
+enum PSysType {
+    EVENT,
+    FIXED
+};
+union PSys *pacing_systems;   /* Array of pacing system (event or fixed) */
+enum PSysType *pacing_types;  /* Array of pacing system types */
+PyObject *protocols;          /* The protocols used to generate the pacing systems */
+double* pacing;               /* Pacing values, same size as pacing_systems and pacing_types */
+int n_pace;                   /* The number of pacing systems */
 
 /*
- * Update variables bound to engine.realtime
+ * CVODE Memory
  */
-static int
-update_realtime_bindings(realtype t, N_Vector y, N_Vector ydot, void *f_data)
-{
-<?
-var = model.binding('realtime')
-if var is not None:
-    print(tab + v(var) + ' = engine_realtime;')
-?>
-    return 0;
-}
+void *cvode_mem;     /* The memory used by the solver */
+#if SUNDIALS_VERSION_MAJOR >= 3
+SUNMatrix sundense_matrix;          /* Dense matrix for linear solves */
+SUNLinearSolver sundense_solver;    /* Linear solver object */
+#endif
+#if SUNDIALS_VERSION_MAJOR >= 6
+SUNContext sundials_context; /* A sundials context to run in (for profiling etc.) */
+#endif
+
+UserData udata;      /* UserData struct, used to pass in parameters */
+realtype* pbar;      /* Vector of independents in user data */
 
 /*
- * Root finding function
- */<?
-root_finding_indice = potential.indice() if potential is not None else 0
-?>
-static int
-root_finding(realtype t, N_Vector y, realtype *gout, void *f_data)
-{
-    gout[0] = NV_Ith_S(y, <?=root_finding_indice?>) - rootfinding_threshold;
-    return 0;
-}
+ * Solver settings
+ */
+double abs_tol = 1e-6;  /* The absolute tolerance */
+double rel_tol = 1e-4;  /* The relative tolerance */
+double dt_max = 0;      /* The maximum step size (0.0 for none) */
+double dt_min = 0;      /* The minimum step size (0.0 for none) */
 
 /*
- * Settings
+ * Solver stats
  */
-static double abs_tol = 1e-6; /* The absolute tolerance */
-static double rel_tol = 1e-4; /* The relative tolerance */
-static double dt_max = 0;     /* The maximum step size (0.0 for none) */
-static double dt_min = 0;     /* The minimum step size (0.0 for none) */
+double realtime = 0;        /* Time since start */
+long evaluations = 0;       /* Number of evaluations since sim init */
+long steps = 0;             /* Number of steps since sim init */
 
 /*
- * Change the tolerance settings
+ * Checking for repeated size-zero steps
  */
-static PyObject*
-sim_set_tolerance(PyObject *self, PyObject *args)
-{
-    /* Check input arguments */
-    double tabs, trel;
-    if (!PyArg_ParseTuple(args, "dd", &tabs, &trel)) {
-        PyErr_SetString(PyExc_Exception, "Expected input arguments: abs_tol(float), rel_tol(float).");
-        return 0;
-    }
-    abs_tol = tabs;
-    rel_tol = trel;
-    Py_RETURN_NONE;
-}
+int zero_step_count;
+const int max_zero_step_count = 500;
 
 /*
- * Change the maximum step size (0 for none)
+ * State vectors
  */
-static PyObject*
-sim_set_max_step_size(PyObject *self, PyObject *args)
-{
-    /* Check input arguments */
-    double tmax;
-    if (!PyArg_ParseTuple(args, "d", &tmax)) {
-        PyErr_SetString(PyExc_Exception, "Expected input argument: tmax(float).");
-        return 0;
-    }
-    dt_max = tmax;
-    Py_RETURN_NONE;
-}
+N_Vector y;     /* The current position y */
+N_Vector* sy;   /* Current state sensitivities, 1 vector per independent */
+
+/* Intermediary positions for logging: these will only be created if using
+   interpolation to log. Otherwise they will simply point to y and sy */
+N_Vector z;
+N_Vector* sz;
+
+/* Previous position, used for error output, always created */
+N_Vector ylast;
 
 /*
- * Change the minimum step size (0 for none)
+ * Customisable constants, passed in from Python
  */
-static PyObject*
-sim_set_min_step_size(PyObject *self, PyObject *args)
-{
-    /* Check input arguments */
-    double tmin;
-    if (!PyArg_ParseTuple(args, "d", &tmin)) {
-        PyErr_SetString(PyExc_Exception, "Expected input argument: tmin(float).");
-        return 0;
-    }
-    dt_min = tmin;
-    Py_RETURN_NONE;
-}
+PyObject* literals;     /* A list of literal constant values */
+PyObject* parameters;   /* A list of parameter values */
 
 /*
- * Add a variable to the logging lists. Returns 1 if successful
+ * State and bound variable communication
  */
-static int
-log_add(PyObject* log_dict, PyObject** logs, realtype** vars, int i, const char* name, const realtype* var)
+PyObject* state_py;     /* List: The state passed from and to Python */
+PyObject* s_state_py;   /* List: The state sensitivities passed from and to Python */
+PyObject* bound_py;     /* List: The bound variables, passed to Python */
+
+/*
+ * Timing
+ */
+double t;       /* Current simulation time */
+double tlast;   /* Previous simulation time, for error and progress tracking */
+double tnext;   /* Next simulation halting point */
+double tmin;    /* The initial simulation time */
+double tmax;    /* The final simulation time */
+
+/*
+ * Logging
+ */
+int dynamic_logging;    /* True if logging every point. */
+PyObject* log_dict;     /* The log dict (DataLog) */
+PyObject* sens_list;    /* Sensitivity logging list */
+
+/* Periodic and point-list logging */
+double tlog;            /* Next time to log */
+double log_interval;    /* The periodic logging interval */
+Py_ssize_t ilog;        /* Index of next point in the point list */
+PyObject* log_times;    /* The point list (or None if disabled) */
+
+/*
+ * Root finding
+ */
+int rf_index;          /* Index of state variable to use in root finding (ignored if not enabled) */
+double rf_threshold;    /* Threshold to use for root finding (ignored if not enabled) */
+PyObject* rf_list;      /* List to store found roots in (or None if not enabled) */
+int* rf_direction;      /* Direction of root crossings: 1 for up, -1 for down, 0 for no crossing. */
+
+/*
+ * Logging realtime and profiling
+ */
+PyObject* benchmarker;      /* myokit.tools.Benchmarker object */
+PyObject* benchmarker_time_str;
+int log_realtime;           /* 1 iff we're logging real simulation time */
+double realtime_start;      /* time when sim run started */
+
+/*
+ * Returns the current time as given by the benchmarker.
+ */
+double
+benchmarker_realtime(void)
 {
-    /* See first use of log_add for notes on unicode */
-    int added = 0;
-    PyObject* key = PyUnicode_FromString(name);
-    if (PyDict_Contains(log_dict, key)) {
-        logs[i] = PyDict_GetItem(log_dict, key);
-        vars[i] = (realtype*)var;
-        added = 1;
-    }
-    Py_DECREF(key);
-    return added;
+    double val;
+    PyObject* ret = PyObject_CallMethodObjArgs(benchmarker, benchmarker_time_str, NULL);
+    if (!PyFloat_Check(ret)) {
+        Py_XDECREF(ret);
+        return -1.0;
+    }
+    val = PyFloat_AsDouble(ret);
+    Py_DECREF(ret);
+    return val - realtime_start;
 }
 
+#ifdef MYOKIT_DEBUG_PROFILING
+PyObject* benchmarker_print_str;
+
 /*
- * Error and warning message handler for CVODE.
- * Error messages are already set via check_cvode_flag, so this method
- * suppresses error messages.
- * Warnings are passed to Python's warning system, where they can be
- * caught or suppressed using the warnings module.
+ * Prints a message to screen, preceded by the time in ms as given by the benchmarker.
  */
 void
-ErrorHandler(int error_code, const char *module, const char *function,
-             char *msg, void *eh_data)
+benchmarker_print(char* message)
 {
-    char errstr[1024];
-    if (error_code > 0) {
-        sprintf(errstr, "CVODE: %s", msg);
-        PyErr_WarnEx(PyExc_RuntimeWarning, errstr, 1);
-    }
+    PyObject* pymsg = PyUnicode_FromString(message);
+    PyObject_CallMethodObjArgs(benchmarker, benchmarker_print_str, pymsg, NULL);
+    Py_DECREF(pymsg);
 }
+#endif
 
 /*
- * Simulation variables
+ * Right-hand-side function of the model ODE
+ *
+ *  realtype t      Current time
+ *  N_Vector y      The current state values
+ *  N_Vector ydot   Space to store the calculated derivatives in
+ *  void* user_data Extra data (contains the sensitivity parameter values)
+ *
  */
+int
+rhs(realtype t, N_Vector y, N_Vector ydot, void *user_data)
+{
+    FSys_Flag flag_fpacing;
+    UserData fdata;
+    int i;
 
-int running = 0;        /* Running yes or no */
+    /* Fixed-form pacing? Then look-up correct value of pacing variable */
+    for (int i = 0; i < n_pace; i++) {
+        if (pacing_types[i] == FIXED) {
+            pacing[i] = FSys_GetLevel(pacing_systems[i].fixed, t, &flag_fpacing);
+            if (flag_fpacing != FSys_OK) { /* This should never happen */
+                FSys_SetPyErr(flag_fpacing);
+                return -1;  /* Negative value signals irrecoverable error to CVODE */
+            }
+        }
+    }
 
-/* Input arguments */
-double tmin;            /* The initial simulation time */
-double tmax;            /* The final simulation time */
-PyObject* state_in;     /* The initial state */
-PyObject* state_out;    /* The final state */
-PyObject* inputs;       /* A vector used to return the binding inputs` values */
-PyObject* eprotocol;    /* An event-based pacing protocol */
-PyObject* fprotocol;    /* A fixed-form pacing protocol */
-PyObject* log_dict;     /* The log dict */
-double log_interval;    /* Periodic logging: The log interval (0 to disable) */
-PyObject* log_times;    /* Point-list logging: List of points (None to disable) */
-PyObject* root_list;    /* Empty list if root finding should be used */
-double root_threshold;  /* Threshold to use for root finding */
-PyObject* benchtime;    /* Callable time() function or None */
+    /* Update model state */
 
-/* Next simulation halting point */
-double tnext;
+    /* Set time, pace, evaluations and realtime */
+    evaluations++;
+    Model_SetBoundVariables(model, (realtype)t, (realtype*)pacing, (realtype)realtime, (realtype)evaluations);
 
-/* Checking for repeated zero size steps */
-int zero_step_count;
-int max_zero_step_count = 500;   /* Increased this from 50 */
+    /* Set sensitivity parameters */
+    if (model->has_sensitivities) {
+        fdata = (UserData) user_data;
+        Model_SetParametersFromIndependents(model, fdata->p);
+    }
 
-/* CVode objects */
-void *cvode_mem;     /* The memory used by the solver */
-N_Vector y;          /* Stores the current position y */
-N_Vector y_log;      /* Used to store y when logging */
-N_Vector dy_log;     /* Used to store dy when logging */
-N_Vector y_last;     /* Used to store previous value of y for error handling */
-#if SUNDIALS_VERSION_MAJOR >= 3
-SUNMatrix sundense_matrix;          /* Dense matrix for linear solves */
-SUNLinearSolver sundense_solver;    /* Linear solver object */
-#endif
-#if SUNDIALS_VERSION_MAJOR >= 6
-SUNContext sundials_context; /* A sundials context to run in (for profiling etc.) */
-#endif
+    /* Set states */
+    Model_SetStates(model, N_VGetArrayPointer(y));
+
+    /* Calculate state derivatives */
+    Model_EvaluateDerivatives(model);
+
+    /* Fill ydot and return */
+    if (ydot != NULL) {
+        for (i=0; i<model->n_states; i++) {
+            NV_Ith_S(ydot, i) = model->derivatives[i];
+        }
+    }
+
+    return 0;
+}
+
+/*
+ * Utility function to set the state sensitivities and evaluate the sensitivity
+ * outputs.
+ *
+ * Assumes the RHS has been evaluated.
+ */
+void
+shs(N_Vector* sy)
+{
+    int i, j;
+
+    /* Unpack state sensitivities */
+    for (i=0; i<model->ns_independents; i++) {
+        for (j=0; j<model->n_states; j++) {
+            model->s_states[i * model->n_states + j] = NV_Ith_S(sy[i], j);
+        }
+    }
 
-/* Root finding */
-int* rootsfound;     /* Used to store found roots */
+    /* Calculate intermediary variable sensitivities */
+    Model_EvaluateSensitivityOutputs(model);
+}
 
-/* Logging */
-PyObject** logs;            /* An array of pointers to a PyObject */
-realtype** vars;            /* An array of pointers to realtype */
-int n_vars;                 /* Number of logging variables */
-int log_bound;              /* True if logging bound variables */
-int log_inter;              /* True if logging intermediary variables */
-int log_deriv;              /* True if logging derivatives */
-PyObject* list_update_str;  /* PyUnicode, used to call "append" method */
-Py_ssize_t ilog;            /* Periodic/point-list logging: Index of next point */
-double tlog;                /* Periodic/point-list logging: Next point */
-int dynamic_logging;        /* True if logging every point. */
+/*
+ * Root finding function. Can contain several functions for which a root is to
+ * be found, but we only use one.
+ */
+int
+rf_function(realtype t, N_Vector y, realtype *gout, void *user_data)
+{
+    gout[0] = NV_Ith_S(y, rf_index) - rf_threshold;
+    return 0;
+}
 
 /*
  * Cleans up after a simulation
  */
-static PyObject*
-sim_clean()
+PyObject*
+sim_clean(void)
 {
-    if (running != 0) {
-        /* Done with str="append", decref it */
-        Py_XDECREF(list_update_str); list_update_str = NULL;
-
-        /* Free allocated space */
-        free(vars); vars = NULL;
-        free(logs); logs = NULL;
-        free(rootsfound); rootsfound = NULL;
-
-        /* Free CVode space */
-        N_VDestroy_Serial(y); y = NULL;
-        N_VDestroy_Serial(dy_log); dy_log = NULL;
-        if (USE_CVODE && !dynamic_logging) {
-            N_VDestroy_Serial(y_log);
-            y_log = NULL;
+    if (initialized) {
+        #ifdef MYOKIT_DEBUG_PROFILING
+        benchmarker_print("CP Entered sim_clean.");
+        #elif defined MYOKIT_DEBUG_MESSAGES
+        printf("CM Cleaning up.\n");
+        #endif
+
+        /* CVode arrays */
+        if (y != NULL) { N_VDestroy_Serial(y); y = NULL; }
+        if (ylast != NULL) { N_VDestroy_Serial(ylast); ylast = NULL; }
+        if (sy != NULL) { N_VDestroyVectorArray(sy, model->ns_independents); sy = NULL; }
+        if (model != NULL && model->is_ode && !dynamic_logging) {
+            if (z != NULL) { N_VDestroy_Serial(z); z = NULL; }
+            if (sz != NULL) { N_VDestroyVectorArray(sz, model->ns_independents); sz = NULL; }
         }
+
+        /* Root finding results */
+        free(rf_direction); rf_direction = NULL;
+
+        /* Sundials objects */
         CVodeFree(&cvode_mem); cvode_mem = NULL;
         #if SUNDIALS_VERSION_MAJOR >= 3
         SUNLinSolFree(sundense_solver); sundense_solver = NULL;
         SUNMatDestroy(sundense_matrix); sundense_matrix = NULL;
         #endif
         #if SUNDIALS_VERSION_MAJOR >= 6
         SUNContext_Free(&sundials_context); sundials_context = NULL;
         #endif
 
-        /* Free pacing system space */
-        ESys_Destroy(epacing); epacing = NULL;
-        FSys_Destroy(fpacing); fpacing = NULL;
+        /* User data and parameter scale array*/
+        free(pbar);
+        if (udata != NULL) {
+            free(udata->p);
+            free(udata); udata = NULL;
+        }
+
+        /* Pacing systems */
+        for (int i = 0; i < n_pace; i++) {
+            if (pacing_types[i] == FIXED) {
+                FSys_Destroy(pacing_systems[i].fixed);
+            } else if (pacing_types[i] == EVENT) {
+                ESys_Destroy(pacing_systems[i].event);
+            }
+        }
+        free(pacing_systems); pacing_systems = NULL;
+        free(pacing_types); pacing_types = NULL;
+        free(pacing); pacing = NULL;
+
+        /* CModel */
+        Model_Destroy(model); model = NULL;
+
+        /* Benchmarking and profiling */
+        #ifdef MYOKIT_DEBUG_PROFILING
+        benchmarker_print("CP Completed sim_clean.");
+        Py_XDECREF(benchmarker_print_str); benchmarker_print_str = NULL;
+        #endif
+        Py_XDECREF(benchmarker_time_str); benchmarker_time_str = NULL;
 
-        /* No longer running */
-        running = 0;
+        /* Deinitialisation complete */
+        initialized = 0;
     }
 
     /* Return 0, allowing the construct
         PyErr_SetString(PyExc_Exception, "Oh noes!");
         return sim_clean()
        to terminate a python function. */
     return 0;
 }
-static PyObject*
+
+/*
+ * Version of sim_clean that sets a python exception.
+ */
+PyObject*
+sim_cleanx(PyObject* ex_type, const char* msg, ...)
+{
+    va_list argptr;
+    char errstr[1024];
+
+    va_start(argptr, msg);
+    vsprintf(errstr, msg, argptr);
+    va_end(argptr);
+
+    PyErr_SetString(ex_type, errstr);
+    return sim_clean();
+}
+
+/*
+ * Version of sim_clean to be called from Python
+ */
+PyObject*
 py_sim_clean(PyObject *self, PyObject *args)
 {
     sim_clean();
     Py_RETURN_NONE;
 }
 
 /*
- * Initialise a run
+ * Initialize a run.
+ * Called by the Python code's run(), followed by several calls to sim_step().
  */
-static PyObject*
+PyObject*
 sim_init(PyObject *self, PyObject *args)
 {
-    int i, j;
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    printf("CM Entering sim_init.\n");
+    #endif
+
+    /* Error checking flags */
     int flag_cvode;
-    int log_first_point;
+    Model_Flag flag_model;
     ESys_Flag flag_epacing;
     FSys_Flag flag_fpacing;
+
+    /* Pacing systems */
+    ESys epacing;
+    FSys fpacing;
+
+    /* General purpose ints for iterating */
+    int i, j;
+
+    /* Log the first point? Only happens if not continuing from a log */
+    int log_first_point;
+
+    /* Proposed next logging or pacing point */
+    double t_proposed;
+
+    /* Python objects, and a python list index variable */
     Py_ssize_t pos;
-    PyObject *flt;
-    PyObject *key;
-    PyObject* ret;
-    PyObject *value;
+    PyObject *val;
+    PyObject *ret;
 
+    /* Check if already initialized */
+    if (initialized) {
+        PyErr_SetString(PyExc_Exception, "Simulation already initialized.");
+        return 0;
+    }
+
+    /* Check for double precision */
     #ifndef SUNDIALS_DOUBLE_PRECISION
     PyErr_SetString(PyExc_Exception, "Sundials must be compiled with double precision.");
-    /* No memory freeing is needed here, return directly */
     return 0;
     #endif
 
-    /* Check if already running */
-    if (running != 0) {
-        PyErr_SetString(PyExc_Exception, "Simulation already initialized.");
-        return 0;
-    }
-
-    /* Set all pointers used in sim_clean to null */
-    list_update_str = NULL;
-    vars = NULL;
-    logs = NULL;
-    rootsfound = NULL;
+    /* Set all global pointers to null */
+    /* Model and pacing */
+    model = NULL;
+    pacing_types = NULL;
+    pacing_systems = NULL;
+    pacing = NULL;
+    /* User data and parameter scaling */
+    udata = NULL;
+    pbar = NULL;
+    /* State vectors */
     y = NULL;
-    dy_log = NULL;
-    y_log = NULL;
-    cvode_mem = NULL;
-    epacing = NULL;
-    fpacing = NULL;
+    sy = NULL;
+    z = NULL;
+    sz = NULL;
+    ylast = NULL;
+    /* Logging */
     log_times = NULL;
+    /* Benchmarking and profiling */
+    benchmarker_time_str = NULL;
+    #ifdef MYOKIT_DEBUG_PROFILING
+    benchmarker_print_str = NULL;
+    #endif
+
+    /* CVode objects */
+    cvode_mem = NULL;
     #if SUNDIALS_VERSION_MAJOR >= 3
     sundense_matrix = NULL;
     sundense_solver = NULL;
     #endif
     #if SUNDIALS_VERSION_MAJOR >= 6
     sundials_context = NULL;
     #endif
 
-    /* Check input arguments */
-    if (!PyArg_ParseTuple(args, "ddOOOOOOdOOdO",
-            &tmin,
-            &tmax,
-            &state_in,
-            &state_out,
-            &inputs,
-            &eprotocol,
-            &fprotocol,
-            &log_dict,
-            &log_interval,
-            &log_times,
-            &root_list,
-            &root_threshold,
-            &benchtime)) {
+    /* Check input arguments     01234567890123456 */
+    if (!PyArg_ParseTuple(args, "ddOOOOOOOdOOidOOi",
+            &tmin,              /*  0. Float: initial time */
+            &tmax,              /*  1. Float: final time */
+            &state_py,          /*  2. List: initial and final state */
+            &s_state_py,        /*  3. List of lists: state sensitivities */
+            &bound_py,          /*  4. List: store final bound variables here */
+            &literals,          /*  5. List: literal constant values */
+            &parameters,        /*  6. List: parameter values */
+            &protocols,         /*   7. Event-based or fixed protocols */
+            &log_dict,          /*  8. DataLog */
+            &log_interval,      /*  9. Float: log interval, or 0 */
+            &log_times,         /* 10. List of logging times, or None */
+            &sens_list,         /* 11. List to store sensitivities in */
+            &rf_index,          /* 12. Int: root-finding state variable */
+            &rf_threshold,      /* 13. Float: root-finding threshold */
+            &rf_list,           /* 14. List to store roots in or None */
+            &benchmarker,       /* 15. myokit.tools.Benchmarker object */
+            &log_realtime       /* 16. Int: 1 if logging real time */
+    )) {
         PyErr_SetString(PyExc_Exception, "Incorrect input arguments.");
-        /* Nothing allocated yet, no pyobjects _created_, return directly */
         return 0;
     }
 
-    /* Now officialy running :) */
-    running = 1;
+    /* Now officialy initialized */
+    initialized = 1;
 
     /*************************************************************************
     From this point on, no more direct returning! Use sim_clean()
 
     To check if this list is still up to date manually search for cvode
     and python stuff. To find what to free() search for "alloc("
     Initialize all to NULL so that free() will work without errors.
@@ -623,929 +684,1244 @@
        be decref'd after appending.
     C. The time float that is created has refcount 1. It's ownership is passed
        on to the calling function. No need to decref.
     D. The PyFloat objects in this list are added using PyList_SetItem which
        steals ownership: No need to decref.
     */
 
+    /* Set simulation starting time */
+    t = tmin;
+
+    /* Reset solver stats */
+    steps = 0;
+    zero_step_count = 0;
+    evaluations = 0;
+    realtime = 0;
+    if (log_realtime) {
+        realtime_start = 0; /* Updated after init, in first call to run */
+        benchmarker_time_str = PyUnicode_FromString("time");
+    }
+
+    /* Set up profiling */
+    #ifdef MYOKIT_DEBUG_PROFILING
+    benchmarker_print_str = PyUnicode_FromString("print");
+    benchmarker_print("CP Initialisation started (entered sim_init()).");
+    #endif
+
+    /* Print info about simulation to undertake */
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    printf("CM Preparing to simulate from %g to %g.\n", tmin, tmax);
+    #endif
+
+    /*
+     * Create model
+     */
+    model = Model_Create(&flag_model);
+    if (flag_model != Model_OK) { Model_SetPyErr(flag_model); return sim_clean(); }
+    #ifdef MYOKIT_DEBUG_PROFILING
+    benchmarker_print("CP Created C model struct.");
+    #endif
+
     /*
      * Create sundials context
      */
     #if SUNDIALS_VERSION_MAJOR >= 6
     flag_cvode = SUNContext_Create(NULL, &sundials_context);
     if (check_cvode_flag(&flag_cvode, "SUNContext_Create", 1)) {
-        PyErr_SetString(PyExc_Exception, "Failed to create Sundials context.");
-        return sim_clean();
+        return sim_cleanx(PyExc_Exception, "Failed to create Sundials context.");
     }
+    #ifdef MYOKIT_DEBUG_PROFILING
+    benchmarker_print("CP Created sundials context.");
+    #endif
     #endif
 
     /*
      * Create state vectors
      */
 
     /* Create state vector */
     #if SUNDIALS_VERSION_MAJOR >= 6
-    y = N_VNew_Serial(N_STATE, sundials_context);
+    y = N_VNew_Serial(model->n_states, sundials_context);
     #else
-    y = N_VNew_Serial(N_STATE);
+    y = N_VNew_Serial(model->n_states);
     #endif
     if (check_cvode_flag((void*)y, "N_VNew_Serial", 0)) {
-        PyErr_SetString(PyExc_Exception, "Failed to create state vector.");
-        return sim_clean();
+        return sim_cleanx(PyExc_Exception, "Failed to create state vector.");
     }
 
     /* Create state vector copy for error handling */
     #if SUNDIALS_VERSION_MAJOR >= 6
-    y_last = N_VNew_Serial(N_STATE, sundials_context);
+    ylast = N_VNew_Serial(model->n_states, sundials_context);
     #else
-    y_last = N_VNew_Serial(N_STATE);
+    ylast = N_VNew_Serial(model->n_states);
     #endif
-    if (check_cvode_flag((void*)y_last, "N_VNew_Serial", 0)) {
-        PyErr_SetString(PyExc_Exception, "Failed to create last-state vector.");
-        return sim_clean();
+    if (check_cvode_flag((void*)ylast, "N_VNew_Serial", 0)) {
+        return sim_cleanx(PyExc_Exception, "Failed to create last-state vector.");
     }
 
+    /* Create sensitivity vector array */
+    if (model->has_sensitivities) {
+        sy = N_VCloneVectorArray(model->ns_independents, y);
+        if (check_cvode_flag((void*)sy, "N_VCloneVectorArray", 0)) {
+            return sim_cleanx(PyExc_Exception, "Failed to allocate space to store sensitivities.");
+        }
+    }
+
+    /*
+     * Create state vectors for logging
+     */
+
     /* Determine if dynamic logging is being used (or if it's periodic/point-list logging) */
     dynamic_logging = (log_interval <= 0 && log_times == Py_None);
 
-    /* Create state vector for logging */
-    if (dynamic_logging || !USE_CVODE) {
-        /* Dynamic logging or cvode-free mode: don't interpolate,
-           so let y_log point to y */
-        y_log = y;
+    /* When using interpolation logging (periodic or point-list), we need a
+       state and s_state vector to pass to CVODE's interpolation function.
+       When using dynamic logging (or running in CVODE-free mode) we can simply
+       log the current state, so z and sz can point to y and sy. */
+    if (dynamic_logging || !model->is_ode) {
+        z = y;
+        sz = sy;
     } else {
-        /* Logging at fixed points:
-           Keep y_log as a separate N_Vector for cvode interpolation */
         #if SUNDIALS_VERSION_MAJOR >= 6
-        y_log = N_VNew_Serial(N_STATE, sundials_context);
+        z = N_VNew_Serial(model->n_states, sundials_context);
         #else
-        y_log = N_VNew_Serial(N_STATE);
+        z = N_VNew_Serial(model->n_states);
         #endif
-        if (check_cvode_flag((void*)y_log, "N_VNew_Serial", 0)) {
-            PyErr_SetString(PyExc_Exception, "Failed to create logging state vector.");
-            return sim_clean();
+        if (check_cvode_flag((void*)z, "N_VNew_Serial", 0)) {
+            return sim_cleanx(PyExc_Exception, "Failed to create state vector for logging.");
+        }
+        if (model->has_sensitivities) {
+            sz = N_VCloneVectorArray(model->ns_independents, y);
+            if (check_cvode_flag((void*)sz, "N_VCloneVectorArray", 0)) {
+                return sim_cleanx(PyExc_Exception, "Failed to create state sensitivity vector array for logging.");
+            }
         }
     }
 
-    /* Create derivative vector for logging */
-    #if SUNDIALS_VERSION_MAJOR >= 6
-    dy_log = N_VNew_Serial(N_STATE, sundials_context);
-    #else
-    dy_log = N_VNew_Serial(N_STATE);
+    #ifdef MYOKIT_DEBUG_PROFILING
+    benchmarker_print("CP Created sundials state vectors.");
     #endif
-    if (check_cvode_flag((void*)dy_log, "N_VNew_Serial", 0)) {
-        PyErr_SetString(PyExc_Exception, "Failed to create logging state derivatives vector.");
-        return sim_clean();
-    }
 
-    /* Set calculated constants */
-    updateConstants();
+    /*
+     * Set initial state in model and vectors
+     */
 
-    /* Set initial values */
-    if (!PyList_Check(state_in)) {
-        PyErr_SetString(PyExc_Exception, "'state_in' must be a list.");
-        return sim_clean();
-    }
-    for(i=0; i<N_STATE; i++) {
-        flt = PyList_GetItem(state_in, i);    /* Don't decref! */
-        if (!PyFloat_Check(flt)) {
-            char errstr[200];
-            sprintf(errstr, "Item %d in state vector is not a float.", i);
-            PyErr_SetString(PyExc_Exception, errstr);
-            return sim_clean();
+    /* Set initial state values */
+    if (!PyList_Check(state_py)) {
+        return sim_cleanx(PyExc_TypeError, "'state_py' must be a list.");
+    }
+    for (i=0; i<model->n_states; i++) {
+        val = PyList_GetItem(state_py, i);    /* Don't decref! */
+        if (!PyFloat_Check(val)) {
+            return sim_cleanx(PyExc_ValueError, "Item %d in state vector is not a float.", i);
+        }
+        model->states[i] = PyFloat_AsDouble(val);
+        NV_Ith_S(y, i) = model->states[i];
+    }
+
+    /* Print initial state */
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    printf("CM Initial state vector (CVODES):\n");
+    for (i=0; i<model->n_states; i++) {
+        printf("CM   %g\n", NV_Ith_S(y, i));
+    }
+    #endif
+
+    /* Set initial sensitivity state values */
+    if (model->has_sensitivities) {
+        if (!PyList_Check(s_state_py)) {
+            return sim_cleanx(PyExc_TypeError, "'s_state_py' must be a list.");
+        }
+        for (i=0; i<model->ns_independents; i++) {
+            val = PyList_GetItem(s_state_py, i); /* Don't decref */
+            if (!PyList_Check(val)) {
+                return sim_cleanx(PyExc_ValueError, "Item %d in state sensitivity matrix is not a list.", i);
+            }
+            for (j=0; j<model->n_states; j++) {
+                ret = PyList_GetItem(val, j);    /* Don't decref! */
+                if (!PyFloat_Check(ret)) {
+                    return sim_cleanx(PyExc_ValueError, "Item %d, %d in state sensitivity matrix is not a float.", i, j);
+                }
+                NV_Ith_S(sy[i], j) = PyFloat_AsDouble(ret);
+                model->s_states[i * model->n_states + j] = NV_Ith_S(sy[i], j);
+            }
         }
-        NV_Ith_S(y, i) = PyFloat_AsDouble(flt);
-        NV_Ith_S(y_last, i) = NV_Ith_S(y, i);
     }
 
-    /* Periodic or point-list logging? Then set init state in y_log as well */
-    #if USE_CVODE
-    if (!dynamic_logging) {
-        for(i=0; i<N_STATE; i++) {
-            NV_Ith_S(y_log, i) = NV_Ith_S(y, i);
+    /* Print initial sensitivities */
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    if (model->has_sensitivities) {
+        printf("CM Initial state sensitivities (CVODES):\n");
+        for (i=0; i<model->ns_independents; i++) {
+            printf("CM   %d.\n", i);
+            for (j=0; j<model->n_states; j++) {
+                printf("CM     %g\n", NV_Ith_S(sy[i], j));
+            }
         }
     }
     #endif
-    /* In cvode-free mode, y_log points to y, so no need */
 
-    /* Root finding list of integers (only contains 1 int...) */
-    rootsfound = (int*)malloc(sizeof(int)*1);
+    #ifdef MYOKIT_DEBUG_PROFILING
+    benchmarker_print("CP Set initial state.");
+    #endif
 
-    /* Reset evaluation count */
-    engine_evaluations = 0;
+    /*
+     * Set values of constants (literals and parameters)
+     */
+    if (!PyList_Check(literals)) {
+        return sim_cleanx(PyExc_TypeError, "'literals' must be a list.");
+    }
+    for (i=0; i<model->n_literals; i++) {
+        val = PyList_GetItem(literals, i);    /* Don't decref */
+        if (!PyFloat_Check(val)) {
+            return sim_cleanx(PyExc_ValueError, "Item %d in literal vector is not a float.", i);
+        }
+        model->literals[i] = PyFloat_AsDouble(val);
+    }
+
+    /* Print initial sensitivities */
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    printf("CM Literals:\n");
+    for (i=0; i<model->n_literals; i++) {
+        printf("CM   %g\n", model->literals[i]);
+    }
+    #endif
 
-    /* Reset step count */
-    engine_steps = 0;
+    #ifdef MYOKIT_DEBUG_PROFILING
+    benchmarker_print("CP Set values of literal variables.");
+    #endif
 
-    /* Zero step tracking */
-    zero_step_count = 0;
+    /* Evaluate calculated constants */
+    Model_EvaluateLiteralDerivedVariables(model);
 
-    /* Check output list */
-    if (!PyList_Check(state_out)) {
-        PyErr_SetString(PyExc_Exception, "'state_out' must be a list.");
-        return sim_clean();
-    }
+    #ifdef MYOKIT_DEBUG_PROFILING
+    benchmarker_print("CP Set values of calculated constants.");
+    #endif
 
-    /* Check for loss-of-precision issue in periodic logging */
-    if (log_interval > 0) {
-        if (tmax + log_interval == tmax) {
-            PyErr_SetString(PyExc_Exception, "Log interval is too small compared to tmax; issue with numerical precision: float(tmax + log_interval) = float(tmax).");
-            return sim_clean();
+    /* Set model parameters */
+    if (model->has_sensitivities) {
+        if (!PyList_Check(parameters)) {
+            return sim_cleanx(PyExc_TypeError, "'parameters' must be a list.");
+        }
+        for (i=0; i<model->n_parameters; i++) {
+            val = PyList_GetItem(parameters, i);    /* Don't decref */
+            if (!PyFloat_Check(val)) {
+                return sim_cleanx(PyExc_ValueError, "Item %d in parameter vector is not a float.", i);
+            }
+            model->parameters[i] = PyFloat_AsDouble(val);
         }
-    }
 
-    /* Set up logging */
-    log_inter = 0;
-    log_bound = 0;
-    n_vars = PyDict_Size(log_dict);
-    logs = (PyObject**)malloc(sizeof(PyObject*)*n_vars);
-    vars = (realtype**)malloc(sizeof(realtype*)*n_vars);
-    i = 0;
-
-    /* Note: The variable names are all ascii compatible
-       In Python2, they are stored in logs as either unicode or bytes
-       In Python3, they are stored exclusively as unicode
-       However, in Python2 b'name' matches u'name' so this is ok (in Python it
-        does not, but we always use unicode so it's ok).
-       The strategy here will be to convert these C-strings to unicode
-        inside log_add, before the comparison. */
+        /* Evaluate calculated constants */
+        Model_EvaluateParameterDerivedVariables(model);
 
-    /* Check states */
-<?
-for var in model.states():
-    print(tab + 'i += log_add(log_dict, logs, vars, i, "' + var.qname() + '", &NV_Ith_S(y_log, ' + str(var.indice())  + '));')
-?>
+        #ifdef MYOKIT_DEBUG_PROFILING
+        benchmarker_print("CP Setting model sensitivity parameters and calculated derived quantities.");
+        #endif
+    }
 
-    /* Check derivatives */
-    j = i;
-<?
-for var in model.states():
-    print(tab + 'i += log_add(log_dict, logs, vars, i, "dot(' + var.qname() + ')", &NV_Ith_S(dy_log, ' + str(var.indice())  + '));')
-?>
-    log_deriv = (i > j);
+    /* Create UserData with sensitivity vector */
+    if (model->has_sensitivities) {
+        udata = (UserData)malloc(sizeof *udata);
+        if (udata == 0) {
+            return sim_cleanx(PyExc_Exception, "Unable to create user data object to store parameter values.");
+        }
+        udata->p = (realtype*)malloc((size_t)model->ns_independents * sizeof(realtype));
+        if (udata->p == 0) {
+            return sim_cleanx(PyExc_Exception, "Unable to allocate space to store parameter values.");
+        }
 
-    /* Check bound variables */
-    j = i;
-<?
-for var, internal in bound_variables.items():
-    print(tab + 'i += log_add(log_dict, logs, vars, i, "' + var.qname() + '", &' + v(var)  + ');')
-?>
-    log_bound = (i > j);
+        /*
+         * Add in values for parameters and initial values
+         * Note that the initial values in the user data don't have any effect,
+         * so their value isn't important (outside of the scaling set below).
+         */
+        for (i=0; i<model->ns_independents; i++) {
+            udata->p[i] = *model->s_independents[i];
+        }
 
-    /* Remaining variables will require an extra rhs() call to evaluate their
-       values at every log point */
-    j = i;
-<?
-for var in model.variables(deep=True, state=False, bound=False, const=False):
-    print(tab + 'i += log_add(log_dict, logs, vars, i, "' + var.qname() + '", &' + v(var)  + ');')
-?>
-    log_inter = (i > j);
+        /* Create parameter scaling vector, for error control */
+        /* TODO: Get this from the Python code ? */
+        pbar = (realtype*)malloc((size_t)model->ns_independents * sizeof(realtype));
+        if (pbar == NULL) {
+            return sim_cleanx(PyExc_Exception, "Unable to allocate space to store parameter scales.");
+        }
+        for (i=0; i<model->ns_independents; i++) {
+            pbar[i] = (udata->p[i] == 0.0 ? 1.0 : fabs(udata->p[i]));
+        }
 
-    /* Check if log contained extra variables */
-    if (i != n_vars) {
-        PyErr_SetString(PyExc_Exception, "Unknown variables found in logging dictionary.");
-        return sim_clean();
-    }
-
-    /* Set up event-based pacing */
-    if (eprotocol != Py_None) {
-        epacing = ESys_Create(&flag_epacing);
-        if (flag_epacing != ESys_OK) { ESys_SetPyErr(flag_epacing); return sim_clean(); }
-        flag_epacing = ESys_Populate(epacing, eprotocol);
-        if (flag_epacing != ESys_OK) { ESys_SetPyErr(flag_epacing); return sim_clean(); }
-        flag_epacing = ESys_AdvanceTime(epacing, tmin);
-        if (flag_epacing != ESys_OK) { ESys_SetPyErr(flag_epacing); return sim_clean(); }
-        tnext = ESys_GetNextTime(epacing, &flag_epacing);
-        engine_pace = ESys_GetLevel(epacing, &flag_epacing);
-        tnext = (tnext < tmax) ? tnext : tmax;
-    } else {
-        tnext = tmax;
+        #ifdef MYOKIT_DEBUG_PROFILING
+        benchmarker_print("CP Created UserData for sensitivities.");
+        #endif
     }
 
-    /* Set up fixed-form pacing */
-    if (eprotocol == Py_None && fprotocol != Py_None) {
-        /* Check 'protocol' is tuple (times, values) */
-        if (!PyTuple_Check(fprotocol)) {
-            PyErr_SetString(PyExc_Exception, "Fixed-form pacing protocol should be tuple or None.");
-            return sim_clean();
-        }
-        if (PyTuple_Size(fprotocol) != 2) {
-            PyErr_SetString(PyExc_Exception, "Fixed-form pacing protocol tuple should have size 2.");
-            return sim_clean();
+    /*
+     * Set up pacing systems
+     */
+    n_pace = 0;
+    if (protocols != Py_None) {
+        if (!PyList_Check(protocols)) {
+            return sim_cleanx(PyExc_TypeError, "'protocols' must be a list.");
+        }
+        n_pace = (int)PyList_Size(protocols);
+    }
+    pacing_systems = (union PSys*)malloc((size_t)n_pace * sizeof(union PSys));
+    if (pacing_systems == NULL) {
+        return sim_cleanx(PyExc_Exception, "Unable to allocate space to store pacing systems.");
+    }
+    pacing_types = (enum PSysType *)malloc((size_t)n_pace * sizeof(enum PSysType));
+    if (pacing_types == NULL) {
+        return sim_cleanx(PyExc_Exception, "Unable to allocate space to store pacing types.");
+    }
+    pacing = (realtype*)malloc((size_t)n_pace * sizeof(realtype));
+    if (pacing == NULL) {
+        return sim_cleanx(PyExc_Exception, "Unable to allocate space to store pacing values.");
+    }
+    Model_SetupPacing(model, n_pace);
+
+    /*
+     *  Unless set by pacing, tnext is set to tmax
+     */
+    tnext = tmax;
+
+    /*
+     * Set up event-based and/or fixed pacing.
+     */
+    if (protocols != Py_None) {
+        for (int i = 0; i < PyList_Size(protocols); i++) {
+            PyObject *protocol = PyList_GetItem(protocols, i);
+            const char* protocol_type_name = Py_TYPE(protocol)->tp_name;
+            if (strcmp(protocol_type_name, "Protocol") == 0) {
+                pacing_systems[i].event = ESys_Create(&flag_epacing);
+                pacing_types[i] = EVENT;
+                epacing = pacing_systems[i].event;
+                if (flag_epacing != ESys_OK) { ESys_SetPyErr(flag_epacing); return sim_clean(); }
+                flag_epacing = ESys_Populate(epacing, protocol);
+                if (flag_epacing != ESys_OK) { ESys_SetPyErr(flag_epacing); return sim_clean(); }
+                flag_epacing = ESys_AdvanceTime(epacing, tmin);
+                if (flag_epacing != ESys_OK) { ESys_SetPyErr(flag_epacing); return sim_clean(); }
+                t_proposed = ESys_GetNextTime(epacing, &flag_epacing);
+                pacing[i] = ESys_GetLevel(epacing, &flag_epacing);
+                tnext = fmin(t_proposed, tnext);
+
+                #ifdef MYOKIT_DEBUG_PROFILING
+                benchmarker_print("CP Created event-based pacing system.");
+                #endif
+            } else if (strcmp(protocol_type_name, "TimeSeriesProtocol") == 0) {
+                pacing_systems[i].fixed = FSys_Create(&flag_fpacing);
+                pacing_types[i] = FIXED;
+                fpacing = pacing_systems[i].fixed;
+                if (flag_fpacing != FSys_OK) { FSys_SetPyErr(flag_fpacing); return sim_clean(); }
+                flag_fpacing = FSys_Populate(fpacing, protocol);
+                if (flag_fpacing != FSys_OK) { FSys_SetPyErr(flag_fpacing); return sim_clean(); }
+
+
+                #ifdef MYOKIT_DEBUG_PROFILING
+                benchmarker_print("CP Created fixed-form pacing system.");
+                #endif
+            } else {
+                printf("protocol_type_name: %s", protocol_type_name);
+                return sim_cleanx(PyExc_TypeError, "Item %d in 'protocols' is not a myokit.Protocol or myokit.TimeSeriesProtocol object.", i);
+            }
         }
-        /* Create fixed-form pacing object and populate */
-        fpacing = FSys_Create(&flag_fpacing);
-        if (flag_fpacing != FSys_OK) { FSys_SetPyErr(flag_fpacing); return sim_clean(); }
-        flag_fpacing = FSys_Populate(fpacing,
-            PyTuple_GetItem(fprotocol, 0),  /* Borrowed, no decref */
-            PyTuple_GetItem(fprotocol, 1));
-        if (flag_fpacing != FSys_OK) { FSys_SetPyErr(flag_fpacing); return sim_clean(); }
     }
 
-    /* Set simulation starting time */
-    engine_time = tmin;
+    /*
+     * Create solver
+     */
+    if (model->is_ode) {
 
-    /* Check dt_max and dt_min */
-    if (dt_max < 0) dt_max = 0.0;
-    if (dt_min < 0) dt_min = 0.0;
-
-    /* Create solver
-     * Using Backward differentiation and Newton iteration */
-    #if USE_CVODE > 0
-    #if SUNDIALS_VERSION_MAJOR >= 6
+        /* Create, using backwards differentiation and newton iterations */
+        #if SUNDIALS_VERSION_MAJOR >= 6
         cvode_mem = CVodeCreate(CV_BDF, sundials_context);
-    #elif SUNDIALS_VERSION_MAJOR >= 4
-        cvode_mem = CVodeCreate(CV_BDF);
-    #else
+        #elif SUNDIALS_VERSION_MAJOR >= 4
+        cvode_mem = CVodeCreate(CV_BDF);  /* Newton is still default */
+        #else
         cvode_mem = CVodeCreate(CV_BDF, CV_NEWTON);
-    #endif
-    if (check_cvode_flag((void*)cvode_mem, "CVodeCreate", 0)) return sim_clean();
+        #endif
+        if (check_cvode_flag((void*)cvode_mem, "CVodeCreate", 0)) return sim_clean();
 
-    /* Set error and warning-message handler */
-    flag_cvode = CVodeSetErrHandlerFn(cvode_mem, ErrorHandler, NULL);
-    if (check_cvode_flag(&flag_cvode, "CVodeInit", 1)) return sim_clean();
+        /* Set error and warning-message handler */
+        flag_cvode = CVodeSetErrHandlerFn(cvode_mem, ErrorHandler, NULL);
+        if (check_cvode_flag(&flag_cvode, "CVodeInit", 1)) return sim_clean();
+
+        /* Initialize solver memory, specify the rhs */
+        flag_cvode = CVodeInit(cvode_mem, rhs, t, y);
+        if (check_cvode_flag(&flag_cvode, "CVodeInit", 1)) return sim_clean();
+
+        /* Set absolute and relative tolerances */
+        flag_cvode = CVodeSStolerances(cvode_mem, RCONST(rel_tol), RCONST(abs_tol));
+        if (check_cvode_flag(&flag_cvode, "CVodeSStolerances", 1)) return sim_clean();
+
+        /* Set a maximum step size (or 0.0 for none) */
+        flag_cvode = CVodeSetMaxStep(cvode_mem, dt_max < 0 ? 0.0 : dt_max);
+        if (check_cvode_flag(&flag_cvode, "CVodeSetmaxStep", 1)) return sim_clean();
+
+        /* Set a minimum step size (or 0.0 for none) */
+        flag_cvode = CVodeSetMinStep(cvode_mem, dt_min < 0 ? 0.0 : dt_min);
+        if (check_cvode_flag(&flag_cvode, "CVodeSetminStep", 1)) return sim_clean();
 
-    /* Initialise solver memory, specify the rhs */
-    flag_cvode = CVodeInit(cvode_mem, rhs, engine_time, y);
-    if (check_cvode_flag(&flag_cvode, "CVodeInit", 1)) return sim_clean();
+        #if SUNDIALS_VERSION_MAJOR >= 6
+            /* Create dense matrix for use in linear solves */
+            sundense_matrix = SUNDenseMatrix(model->n_states, model->n_states, sundials_context);
+            if (check_cvode_flag((void *)sundense_matrix, "SUNDenseMatrix", 0)) return sim_clean();
+
+            /* Create dense linear solver object with matrix */
+            sundense_solver = SUNLinSol_Dense(y, sundense_matrix, sundials_context);
+            if (check_cvode_flag((void *)sundense_solver, "SUNLinSol_Dense", 0)) return sim_clean();
+
+            /* Attach the matrix and solver to cvode */
+            flag_cvode = CVodeSetLinearSolver(cvode_mem, sundense_solver, sundense_matrix);
+            if (check_cvode_flag(&flag_cvode, "CVodeSetLinearSolver", 1)) return sim_clean();
+        #elif SUNDIALS_VERSION_MAJOR >= 4
+            /* Create dense matrix for use in linear solves */
+            sundense_matrix = SUNDenseMatrix(model->n_states, model->n_states);
+            if (check_cvode_flag((void *)sundense_matrix, "SUNDenseMatrix", 0)) return sim_clean();
+
+            /* Create dense linear solver object with matrix */
+            sundense_solver = SUNLinSol_Dense(y, sundense_matrix);
+            if (check_cvode_flag((void *)sundense_solver, "SUNLinSol_Dense", 0)) return sim_clean();
+
+            /* Attach the matrix and solver to cvode */
+            flag_cvode = CVodeSetLinearSolver(cvode_mem, sundense_solver, sundense_matrix);
+            if (check_cvode_flag(&flag_cvode, "CVodeSetLinearSolver", 1)) return sim_clean();
+        #elif SUNDIALS_VERSION_MAJOR >= 3
+            /* Create dense matrix for use in linear solves */
+            sundense_matrix = SUNDenseMatrix(model->n_states, model->n_states);
+            if (check_cvode_flag((void *)sundense_matrix, "SUNDenseMatrix", 0)) return sim_clean();
+
+            /* Create dense linear solver object with matrix */
+            sundense_solver = SUNDenseLinearSolver(y, sundense_matrix);
+            if (check_cvode_flag((void *)sundense_solver, "SUNDenseLinearSolver", 0)) return sim_clean();
+
+            /* Attach the matrix and solver to cvode */
+            flag_cvode = CVDlsSetLinearSolver(cvode_mem, sundense_solver, sundense_matrix);
+            if (check_cvode_flag(&flag_cvode, "CVDlsSetLinearSolver", 1)) return sim_clean();
+        #else
+            /* Create dense matrix for use in linear solves */
+            flag_cvode = CVDense(cvode_mem, model->n_states);
+            if (check_cvode_flag(&flag_cvode, "CVDense", 1)) return sim_clean();
+        #endif
 
-    /* Set absolute and relative tolerances */
-    flag_cvode = CVodeSStolerances(cvode_mem, RCONST(rel_tol), RCONST(abs_tol));
-    if (check_cvode_flag(&flag_cvode, "CVodeSStolerances", 1)) return sim_clean();
+        #ifdef MYOKIT_DEBUG_PROFILING
+        benchmarker_print("CP CVODES solver initialized.");
+        #endif
 
-    /* Set a maximum step size (or 0.0 for none) */
+        /* Activate forward sensitivity computations */
+        if (model->has_sensitivities) {
+            /* TODO: NULL here is the place to insert a user function to calculate the
+               RHS of the sensitivity ODE */
+            /*flag_cvode = CVodeSensInit(cvode_mem, model->ns_independents, CV_SIMULTANEOUS, rhs1, sy);*/
+            flag_cvode = CVodeSensInit(cvode_mem, model->ns_independents, CV_SIMULTANEOUS, NULL, sy);
+            if (check_cvode_flag(&flag_cvode, "CVodeSensInit", 1)) return sim_clean();
+
+            /* Attach user data */
+            flag_cvode = CVodeSetUserData(cvode_mem, udata);
+            if (check_cvode_flag(&flag_cvode, "CVodeSetUserData", 1)) return sim_clean();
+
+            /* Set parameter scales used in tolerances */
+            flag_cvode = CVodeSetSensParams(cvode_mem, udata->p, pbar, NULL);
+            if (check_cvode_flag(&flag_cvode, "CVodeSetSensParams", 1)) return sim_clean();
+
+            /* Set sensitivity tolerances calculating method (using pbar) */
+            flag_cvode = CVodeSensEEtolerances(cvode_mem);
+            if (check_cvode_flag(&flag_cvode, "CVodeSensEEtolerances", 1)) return sim_clean();
 
-    flag_cvode = CVodeSetMaxStep(cvode_mem, dt_max);
-    if (check_cvode_flag(&flag_cvode, "CVodeSetmaxStep", 1)) return sim_clean();
+            #ifdef MYOKIT_DEBUG_PROFILING
+            benchmarker_print("CP CVODES sensitivity methods initialized.");
+            #endif
+        }
+    }
 
-    /* Set a minimum step size (or 0.0 for none) */
-    flag_cvode = CVodeSetMinStep(cvode_mem, dt_min);
-    if (check_cvode_flag(&flag_cvode, "CVodeSetminStep", 1)) return sim_clean();
+    /*
+     * Root finding
+     * Enabled if rf_list is a PyList
+     */
+    rf_direction = NULL;
 
-    #if SUNDIALS_VERSION_MAJOR >= 6
-        /* Create dense matrix for use in linear solves */
-        sundense_matrix = SUNDenseMatrix(N_STATE, N_STATE, sundials_context);
-        if (check_cvode_flag((void *)sundense_matrix, "SUNDenseMatrix", 0)) return sim_clean();
-
-        /* Create dense linear solver object with matrix */
-        sundense_solver = SUNLinSol_Dense(y, sundense_matrix, sundials_context);
-        if (check_cvode_flag((void *)sundense_solver, "SUNLinSol_Dense", 0)) return sim_clean();
-
-        /* Attach the matrix and solver to cvode */
-        flag_cvode = CVodeSetLinearSolver(cvode_mem, sundense_solver, sundense_matrix);
-        if (check_cvode_flag(&flag_cvode, "CVodeSetLinearSolver", 1)) return sim_clean();
-    #elif SUNDIALS_VERSION_MAJOR >= 4
-        /* Create dense matrix for use in linear solves */
-        sundense_matrix = SUNDenseMatrix(N_STATE, N_STATE);
-        if (check_cvode_flag((void *)sundense_matrix, "SUNDenseMatrix", 0)) return sim_clean();
-
-        /* Create dense linear solver object with matrix */
-        sundense_solver = SUNLinSol_Dense(y, sundense_matrix);
-        if (check_cvode_flag((void *)sundense_solver, "SUNLinSol_Dense", 0)) return sim_clean();
-
-        /* Attach the matrix and solver to cvode */
-        flag_cvode = CVodeSetLinearSolver(cvode_mem, sundense_solver, sundense_matrix);
-        if (check_cvode_flag(&flag_cvode, "CVodeSetLinearSolver", 1)) return sim_clean();
-    #elif SUNDIALS_VERSION_MAJOR >= 3
-        /* Create dense matrix for use in linear solves */
-        sundense_matrix = SUNDenseMatrix(N_STATE, N_STATE);
-        if(check_cvode_flag((void *)sundense_matrix, "SUNDenseMatrix", 0)) return sim_clean();
-
-        /* Create dense linear solver object with matrix */
-        sundense_solver = SUNDenseLinearSolver(y, sundense_matrix);
-        if(check_cvode_flag((void *)sundense_solver, "SUNDenseLinearSolver", 0)) return sim_clean();
-
-        /* Attach the matrix and solver to cvode */
-        flag_cvode = CVDlsSetLinearSolver(cvode_mem, sundense_solver, sundense_matrix);
-        if(check_cvode_flag(&flag_cvode, "CVDlsSetLinearSolver", 1)) return sim_clean();
-    #else
-        /* Create dense matrix for use in linear solves */
-        flag_cvode = CVDense(cvode_mem, N_STATE);
-        if (check_cvode_flag(&flag_cvode, "CVDense", 1)) return sim_clean();
-    #endif
-    #endif
+    if (model->is_ode && PyList_Check(rf_list)) {
+        /* Initialize root function with 1 component */
+        flag_cvode = CVodeRootInit(cvode_mem, 1, rf_function);
+        if (check_cvode_flag(&flag_cvode, "CVodeRootInit", 1)) return sim_clean();
 
-    /* Benchmarking? Then set engine_realtime to 0.0 */
-    if (benchtime != Py_None) {
-        /* Store initial time as 0 */
-        engine_realtime = 0.0;
-        /* Tell sim_step to set engine_starttime */
-        engine_starttime = -1;
+        /* Direction of root crossings, one entry per root function, but we only use 1. */
+        rf_direction = (int*)malloc(sizeof(int));
+
+        #ifdef MYOKIT_DEBUG_PROFILING
+        benchmarker_print("CP CVODES root-finding initialized.");
+        #endif
     }
 
-    /* Set string for updating lists/arrays using Python interface. */
-    list_update_str = PyUnicode_FromString("append");
+    /*
+     * Set up logging, and log first step if needed.
+     */
+
+    /* Check for loss-of-precision issue in periodic logging */
+    if (log_interval > 0) {
+        if (tmax + log_interval == tmax) {
+            return sim_cleanx(PyExc_ValueError, "Log interval is too small compared to tmax; issue with numerical precision: float(tmax + log_interval) = float(tmax).");
+        }
+    }
+
+    /* Set up logging */
+    flag_model = Model_InitializeLogging(model, log_dict);
+    if (flag_model != Model_OK) { Model_SetPyErr(flag_model); return sim_clean(); }
+    #ifdef MYOKIT_DEBUG_PROFILING
+    benchmarker_print("CP Logging initialized.");
+    #endif
+
+    /* Check logging list for sensitivities */
+    if (model->has_sensitivities) {
+        if (!PyList_Check(sens_list)) {
+            return sim_cleanx(PyExc_TypeError, "'sens_list' must be a list.");
+        }
+    }
 
     /* Set logging points */
     if (log_interval > 0) {
 
         /* Periodic logging */
         ilog = 0;
         tlog = tmin;
 
     } else if (log_times != Py_None) {
 
         /* Point-list logging */
 
-        /* Check the log_times list */
-        if (!PyList_Check(log_times)) {
-            PyErr_SetString(PyExc_Exception, "'log_times' must be a list.");
-            return sim_clean();
+        /* Check the log_times sequence */
+        if (!PySequence_Check(log_times)) {
+            return sim_cleanx(PyExc_TypeError, "'log_times' must be a sequence type.");
         }
 
-        /* Read next log point off the list */
+        /* Read next log point off the sequence */
         ilog = 0;
-        tlog = engine_time - 1;
-        while(ilog < PyList_Size(log_times) && tlog < engine_time) {
-            flt = PyList_GetItem(log_times, ilog); /* Borrowed */
-            if (!PyFloat_Check(flt)) {
-                PyErr_SetString(PyExc_Exception, "Entries in 'log_times' must be floats.");
-                return sim_clean();
+        tlog = t - 1;
+        while(ilog < PySequence_Size(log_times) && tlog < t) {
+            val = PySequence_GetItem(log_times, ilog); /* New reference */
+            if (PyFloat_Check(val)) {
+                tlog = PyFloat_AsDouble(val);
+                Py_DECREF(val);
+            } else if (PyNumber_Check(val)) {
+                ret = PyNumber_Float(val); /* New reference */
+                Py_DECREF(val);            /* Done with val */
+                if (ret == NULL) {
+                    return sim_cleanx(PyExc_ValueError, "Unable to cast entry in 'log_times' to float.");
+                } else {
+                    tlog = PyFloat_AsDouble(ret);
+                    Py_DECREF(ret);
+                }
+            } else {
+                Py_DECREF(val);
+                return sim_cleanx(PyExc_ValueError, "Entries in 'log_times' must be floats.");
             }
-            tlog = PyFloat_AsDouble(flt);
+            val = NULL;
             ilog++;
-            flt = NULL;
         }
 
-        /* No points beyond engine_time? Then don't log any future points. */
-        if(tlog < engine_time) {
+        /* No points beyond time? Then don't log any future points. */
+        if (tlog < t) {
             tlog = tmax + 1;
         }
 
     } else {
 
         /*
          * Dynamic logging
          *
          * Log the first entry, but only if not appending to an existing log.
          * This prevents points from appearing twice when a simulation with
          * dynamic logging is stopped and started.
          */
 
-        /*  Check if the log is empty */
+        /* Check if the log is empty */
         log_first_point = 1;
         pos = 0;
-        if(PyDict_Next(log_dict, &pos, &key, &value)) {
-            /* Items found in dict, randomly selected list now in "value" */
-            /* Both key and value are borrowed references, no need to decref */
-            log_first_point = (PyObject_Size(value) <= 0);
+        if (PyDict_Next(log_dict, &pos, &ret, &val)) {
+            /* Items found in dict, randomly selected list now in "val" */
+            /* Both key (ret) and value (val) are borrowed references, no need to decref */
+            log_first_point = (PyObject_Size(val) <= 0);
         }
 
         /* If so, log the first point! */
         if (log_first_point) {
-            rhs(engine_time, y, dy_log, 0);
+            rhs(t, y, NULL, udata);
             /* At this point, we have y(t), inter(t) and dy(t) */
             /* We've also loaded time(t) and pace(t) */
-            for(i=0; i<n_vars; i++) {
-                flt = PyFloat_FromDouble(*vars[i]);
-                ret = PyObject_CallMethodObjArgs(logs[i], list_update_str, flt, NULL);
-                Py_DECREF(flt);
-                Py_XDECREF(ret);
-                if (ret == NULL) {
-                    flt = NULL;
-                    PyErr_SetString(PyExc_Exception, "Call to append() failed on logging list.");
-                    return sim_clean();
-                }
+
+            flag_model = Model_Log(model);
+            if (flag_model != Model_OK) { Model_SetPyErr(flag_model); return sim_clean(); }
+
+            if (model->has_sensitivities) {
+                /* Calculate intermediary variable sensitivities, using
+                   initial state sensitivities */
+                shs(sy);
+
+                /* Write sensitivity matrix to list */
+                flag_model = Model_LogSensitivityMatrix(model, sens_list);
+                if (flag_model != Model_OK) { Model_SetPyErr(flag_model); return sim_clean(); }
             }
-            flt = NULL;
-            ret = NULL;
         }
     }
 
-    /* Root finding enabled? (cvode-mode only) */
-    #if USE_CVODE
-    if (PySequence_Check(root_list)) {
-        /* Set threshold */
-        rootfinding_threshold = root_threshold;
-        /* Initialize root function with 1 component */
-        flag_cvode = CVodeRootInit(cvode_mem, 1, root_finding);
-        if (check_cvode_flag(&flag_cvode, "CVodeRootInit", 1)) return sim_clean();
-    }
+    #ifdef MYOKIT_DEBUG_PROFILING
+    benchmarker_print("CP Logging times and strategy initialized.");
     #endif
 
-    /* Done! */
+    /*
+     * Done!
+     */
+    #ifdef MYOKIT_DEBUG_PROFILING
+    benchmarker_print("CP Initialisation complete (returning from sim_init).");
+    #endif
     Py_RETURN_NONE;
 }
 
 /*
  * Takes the next steps in a simulation run
  */
-static PyObject*
+PyObject*
 sim_step(PyObject *self, PyObject *args)
 {
+    /* Error flags */
+    Model_Flag flag_model;
     ESys_Flag flag_epacing;
-    int i;
-    int steps_taken = 0;    /* Number of integration steps taken in this call */
     int flag_cvode;         /* CVode flag */
     int flag_root;          /* Root finding flag */
     int flag_reinit = 0;    /* Set if CVODE needs to be reset during a simulation step */
-    PyObject *flt, *ret;
+
+    /* Multi-purpose ints for iterating */
+    int i, j;
+
+    /* Number of integration steps taken in this call */
+    int steps_taken = 0;
+
+    /* Proposed next logging or pacing point */
+    double t_proposed;
+
+    /* Multi-purpose Python objects */
+    PyObject *val;
+    PyObject* ret;
 
     /*
-     * Benchmarking? Then make sure start time is set.
+     * Set start time for logging of realtime.
      * This is handled here instead of in sim_init so it only includes time
      * taken performing steps, not time initialising memory etc.
      */
-    if (benchtime != Py_None && engine_starttime < 0) {
-        flt = PyObject_CallFunction(benchtime, "");
-        if (!PyFloat_Check(flt)) {
-            Py_XDECREF(flt); flt = NULL;
-            PyErr_SetString(PyExc_Exception, "Call to benchmark time function didn't return float.");
-            return sim_clean();
+    if (log_realtime && realtime_start == 0) {
+        realtime_start = benchmarker_realtime();
+        if (realtime_start <= 0) {
+            return sim_cleanx(PyExc_Exception, "Failed to set realtime_start.");
         }
-        engine_starttime = PyFloat_AsDouble(flt);
-        Py_DECREF(flt); flt = NULL;
     }
 
     /* Go! */
     while(1) {
 
-        /* Back-up current y (no allocation, this is fast) */
-        for(i=0; i<N_STATE; i++) {
-            NV_Ith_S(y_last, i) = NV_Ith_S(y, i);
+        /* Back-up current y */
+        for (i=0; i<model->n_states; i++) {
+            NV_Ith_S(ylast, i) = NV_Ith_S(y, i);
         }
 
         /* Store engine time before step */
-        engine_time_last = engine_time;
+        tlast = t;
 
-        #if USE_CVODE
+        if (model->is_ode) {
 
-        /* Take a single ODE step */
-        flag_cvode = CVode(cvode_mem, tnext, y, &engine_time, CV_ONE_STEP);
+            /* Take a single ODE step */
+            #ifdef MYOKIT_DEBUG_MESSAGES
+            printf("\nCM Taking CVODE step from time %g to %g.\n", t, tnext);
+            #endif
+            flag_cvode = CVode(cvode_mem, tnext, y, &t, CV_ONE_STEP);
 
-        /* Check for errors */
-        if (check_cvode_flag(&flag_cvode, "CVode", 1)) {
-            /* Something went wrong... Set outputs and return */
-            for(i=0; i<N_STATE; i++) {
-                PyList_SetItem(state_out, i, PyFloat_FromDouble(NV_Ith_S(y_last, i)));
-                /* PyList_SetItem steals a reference: no need to decref the double! */
+            /* Check for errors */
+            if (check_cvode_flag(&flag_cvode, "CVode", 1)) {
+                /* Something went wrong... Set outputs and return */
+                for (i=0; i<model->n_states; i++) {
+                    PyList_SetItem(state_py, i, PyFloat_FromDouble(NV_Ith_S(ylast, i)));
+                    /* PyList_SetItem steals a reference: no need to decref the double! */
+                }
+                PyList_SetItem(bound_py, 0, PyFloat_FromDouble(tlast));
+                PyList_SetItem(bound_py, 1, PyFloat_FromDouble(realtime));
+                PyList_SetItem(bound_py, 2, PyFloat_FromDouble((double)evaluations));
+                for (int i = 0; i < n_pace; i++) {
+                    PyList_SetItem(bound_py, 3 + i, PyFloat_FromDouble(pacing[i]));
+                }
+                return sim_clean();
             }
-            PyList_SetItem(inputs, 0, PyFloat_FromDouble(engine_time));
-            PyList_SetItem(inputs, 1, PyFloat_FromDouble(engine_pace));
-            PyList_SetItem(inputs, 2, PyFloat_FromDouble(engine_realtime));
-            PyList_SetItem(inputs, 3, PyFloat_FromDouble(engine_evaluations));
-            return sim_clean();
-        }
-
-        #else
 
-        /* Just jump to next event */
-        /* Note 1: To stay compatible with cvode-mode, don't jump to the
-           next log time (if tlog < tnext) */
-        /* Note 2: tnext can be infinity, so don't always jump there. */
-        engine_time = (tmax > tnext) ? tnext : tmax;
-        flag_cvode = CV_SUCCESS;
+        } else {
 
-        #endif
+            /* Just jump to next event */
+            /* Note 1: To stay compatible with cvode-mode, don't jump to the
+               next log time (if tlog < tnext) */
+            /* Note 2: tnext can be infinity, so don't always jump there. */
+            t = (tmax > tnext) ? tnext : tmax;
+            flag_cvode = CV_SUCCESS;
+        }
 
         /* Check if progress is being made */
-        if(engine_time == engine_time_last) {
-            if(++zero_step_count >= max_zero_step_count) {
-                char errstr[200];
-                sprintf(errstr, "ZERO_STEP %f", engine_time);
-                PyErr_SetString(PyExc_Exception, errstr);
-                return sim_clean();
+        if (t == tlast) {
+            if (++zero_step_count >= max_zero_step_count) {
+                return sim_cleanx(PyExc_ArithmeticError, "Maximum number of zero-length steps taken at t=%g", t);
             }
         } else {
-            /* Only count consecutive zero steps! */
+            /* Only count consecutive zero steps */
             zero_step_count = 0;
         }
 
         /* Update step count */
-        engine_steps++;
+        steps++;
 
         /* If we got to this point without errors... */
         if ((flag_cvode == CV_SUCCESS) || (flag_cvode == CV_ROOT_RETURN)) {
 
-            /* Next event time exceeded? (Can't happen in cvode-free mode) */
-            #if USE_CVODE
-            if (engine_time > tnext) {
-
-                /* Go back to engine_time=tnext */
-                flag_cvode = CVodeGetDky(cvode_mem, tnext, 0, y);
-                if (check_cvode_flag(&flag_cvode, "CVodeGetDky", 1)) return sim_clean();
-                engine_time = tnext;
-                /* Require reinit (after logging) */
-                flag_reinit = 1;
-
-            } else if (flag_cvode == CV_ROOT_RETURN) {
-
-                /* Store found roots */
-                flag_root = CVodeGetRootInfo(cvode_mem, rootsfound);
-                if (check_cvode_flag(&flag_root, "CVodeGetRootInfo", 1)) return sim_clean();
-                flt = PyTuple_New(2);
-                PyTuple_SetItem(flt, 0, PyFloat_FromDouble(engine_time)); /* Steals reference, so this is ok */
-                PyTuple_SetItem(flt, 1, PyLong_FromLong(rootsfound[0]));
-                ret = PyObject_CallMethodObjArgs(root_list, list_update_str, flt, NULL);
-                Py_DECREF(flt); flt = NULL;
-                Py_XDECREF(ret);
-                if (ret == NULL) {
-                    PyErr_SetString(PyExc_Exception, "Call to append() failed on root finding list.");
-                    return sim_clean();
-                }
-                ret = NULL;
-            }
-            #endif
+            /*
+             * Rewinding to tnext, and root finding
+             */
+            if (model->is_ode) {
+
+                /* Next event time exceeded? */
+                if (t > tnext) {
+                    #ifdef MYOKIT_DEBUG_MESSAGES
+                    printf("CM Event time exceeded, rewinding to %g.\n", tnext);
+                    #endif
+
+                    /* Go back to time=tnext */
+                    flag_cvode = CVodeGetDky(cvode_mem, tnext, 0, y);
+                    if (check_cvode_flag(&flag_cvode, "CVodeGetDky", 1)) return sim_clean();
+                    if (model->has_sensitivities) {
+                        flag_cvode = CVodeGetSensDky(cvode_mem, tnext, 0, sy);
+                        if (check_cvode_flag(&flag_cvode, "CVodeGetSensDky", 1)) return sim_clean();
+                    }
+                    t = tnext;
+                    /* Require reinit (after logging) */
+                    flag_reinit = 1;
+
+                } else {
+
+                    /* Get current sensitivity vector */
+                    if (model->has_sensitivities) {
+                        flag_cvode = CVodeGetSens(cvode_mem, &t, sy);
+                        if (check_cvode_flag(&flag_cvode, "CVodeGetSens", 1)) return sim_clean();
+                    }
 
-            /* Periodic logging or point-list logging */
-            if (!dynamic_logging && engine_time > tlog) {
-                /* Note: For periodic logging, the condition should be
-                   `time > tlog` so that we log half-open intervals (i.e. the
-                   final point should never be included). */
-
-                /* Benchmarking? Then set engine_realtime */
-                if (benchtime != Py_None) {
-                    flt = PyObject_CallFunction(benchtime, "");
-                    if (!PyFloat_Check(flt)) {
-                        Py_XDECREF(flt); flt = NULL;
-                        PyErr_SetString(PyExc_Exception, "Call to benchmark time function didn't return float.");
-                        return sim_clean();
+                    /* Root found */
+                    if (flag_cvode == CV_ROOT_RETURN) {
+
+                        /* Get directions of root crossings (1 per root function) */
+                        flag_root = CVodeGetRootInfo(cvode_mem, rf_direction);
+                        if (check_cvode_flag(&flag_root, "CVodeGetRootInfo", 1)) return sim_clean();
+                        /* We only have one root function, so we know that rf_direction[0] is non-zero at this point. */
+
+                        /* Store tuple (time, direction) for the found root */
+                        val = PyTuple_New(2);
+                        PyTuple_SetItem(val, 0, PyFloat_FromDouble(t)); /* Steals reference, so this is ok */
+                        PyTuple_SetItem(val, 1, PyLong_FromLong(rf_direction[0]));
+                        if (PyList_Append(rf_list, val)) {    /* Doesn't steal, need to decref */
+                            Py_DECREF(val);
+                            return sim_cleanx(PyExc_Exception, "Call to append() failed on root finding list.");
+                        }
+                        Py_DECREF(val); val = NULL;
                     }
-                    engine_realtime = PyFloat_AsDouble(flt) - engine_starttime;
-                    Py_DECREF(flt); flt = NULL;
-                    /* Update any variables bound to realtime */
-                    update_realtime_bindings(engine_time, y, dy_log, 0);
                 }
+            }
+
+            /*
+             * Logging interpolated points (periodic logging or point-list logging)
+             */
+            if (!dynamic_logging && t > tlog) {
+                /* Note: For periodic logging, the condition should be `t > tlog`
+                 * so that we log half-open intervals (i.e. the final point should
+                 * never be included).
+                 */
 
                 /* Log points */
-                while (engine_time > tlog) {
+                while (t > tlog) {
+                    #ifdef MYOKIT_DEBUG_MESSAGES
+                    printf("CM Interpolation-logging for t=%g.\n", t);
+                    #endif
+
+                    /* Benchmarking? Then set realtime */
+                    if (log_realtime) {
+                        realtime = benchmarker_realtime();
+                        if (realtime < 0) return sim_cleanx(PyExc_Exception, "Failed to set realtime during interpolation logging.");
+                    }
 
                     /* Get interpolated y(tlog) */
-                    #if USE_CVODE
-                    flag_cvode = CVodeGetDky(cvode_mem, tlog, 0, y_log);
-                    if (check_cvode_flag(&flag_cvode, "CVodeGetDky", 1)) return sim_clean();
-                    #endif
-                    /* If cvode-free mode, the state can't change so we don't
+                    if (model->is_ode) {
+                        flag_cvode = CVodeGetDky(cvode_mem, tlog, 0, z);
+                        if (check_cvode_flag(&flag_cvode, "CVodeGetDky", 1)) return sim_clean();
+                        if (model->has_sensitivities) {
+                            flag_cvode = CVodeGetSensDky(cvode_mem, tlog, 0, sz);
+                            if (check_cvode_flag(&flag_cvode, "CVodeGetSensDky", 1)) return sim_clean();
+                        }
+                    }
+                    /* If cvode-free mode, the states can't change so we don't
                        need to do anything here */
 
                     /* Calculate intermediate variables & derivatives */
-                    rhs(tlog, y_log, dy_log, 0);
+                    rhs(tlog, z, NULL, udata);
 
                     /* Write to log */
-                    for(i=0; i<n_vars; i++) {
-                        flt = PyFloat_FromDouble(*vars[i]);
-                        ret = PyObject_CallMethodObjArgs(logs[i], list_update_str, flt, NULL);
-                        Py_DECREF(flt);
-                        Py_XDECREF(ret);
-                        if (ret == NULL) {
-                            flt = NULL;
-                            PyErr_SetString(PyExc_Exception, "Call to append() failed on logging list.");
-                            return sim_clean();
-                        }
+                    flag_model = Model_Log(model);
+                    if (flag_model != Model_OK) { Model_SetPyErr(flag_model); return sim_clean(); }
+
+                    if (model->has_sensitivities) {
+                        /* Calculate sensitivities to output */
+                        shs(sz);
+
+                        /* Write sensitivity matrix to list */
+                        flag_model = Model_LogSensitivityMatrix(model, sens_list);
+                        if (flag_model != Model_OK) { Model_SetPyErr(flag_model); return sim_clean(); }
                     }
-                    ret = flt = NULL;
 
                     /* Get next logging point */
                     if (log_interval > 0) {
                         /* Periodic logging */
                         ilog++;
                         tlog = tmin + (double)ilog * log_interval;
                         if (ilog == 0) {
                             /* Unsigned int wraps around instead of overflowing, becomes zero again */
-                            PyErr_SetString(PyExc_Exception, "Overflow in logged step count: Simulation too long!");
-                            return sim_clean();
+                            return sim_cleanx(PyExc_OverflowError, "Overflow in logged step count: Simulation too long!");
                         }
                     } else {
                         /* Point-list logging */
-                        /* Read next log point off the list */
-                        if (ilog < PyList_Size(log_times)) {
-                            flt = PyList_GetItem(log_times, ilog); /* Borrowed */
-                            if (!PyFloat_Check(flt)) {
-                                PyErr_SetString(PyExc_Exception, "Entries in 'log_times' must be floats.");
-                                return sim_clean();
+                        /* Read next log point off the sequence */
+                        if (ilog < PySequence_Size(log_times)) {
+                            val = PySequence_GetItem(log_times, ilog); /* New reference */
+                            if (PyFloat_Check(val)) {
+                                t_proposed = PyFloat_AsDouble(val);
+                                Py_DECREF(val);
+                            } else if (PyNumber_Check(val)) {
+                                ret = PyNumber_Float(val);  /* New reference */
+                                Py_DECREF(val);
+                                if (ret == NULL) {
+                                    return sim_cleanx(PyExc_ValueError, "Unable to cast entry in 'log_times' to float.");
+                                } else {
+                                    t_proposed = PyFloat_AsDouble(ret);
+                                    Py_DECREF(ret);
+                                }
+                            } else {
+                                Py_DECREF(val);
+                                return sim_cleanx(PyExc_ValueError, "Entries in 'log_times' must be floats.");
                             }
-                            tlog = PyFloat_AsDouble(flt);
+                            if (t_proposed < tlog) {
+                                return sim_cleanx(PyExc_ValueError, "Values in log_times must be non-decreasing.");
+                            }
+                            tlog = t_proposed;
                             ilog++;
-                            flt = NULL;
+                            val = NULL;
                         } else {
                             tlog = tmax + 1;
                         }
                     }
                 }
             }
 
-            /* Event-based pacing */
-
-            /* At this point we have logged everything _before_ engine_time, so
-               it's safe to update the pacing mechanism. */
-            if (epacing != NULL) {
-                flag_epacing = ESys_AdvanceTime(epacing, engine_time);
-                if (flag_epacing != ESys_OK) { ESys_SetPyErr(flag_epacing); return sim_clean(); }
-                tnext = ESys_GetNextTime(epacing, NULL);
-                engine_pace = ESys_GetLevel(epacing, NULL);
-                tnext = (tnext < tmax) ? tnext : tmax;
+            /*
+             * Event-based pacing
+             *
+             * At this point we have logged everything _before_ time t, so it
+             * is safe to update the pacing mechanism to time t.
+             */
+            tnext = tmax;
+            for (int i = 0; i < n_pace; i++) {
+                if (pacing_types[i] == EVENT) {
+                    ESys epacing = pacing_systems[i].event;
+                    flag_epacing = ESys_AdvanceTime(epacing, t);
+                    if (flag_epacing != ESys_OK) {
+                        ESys_SetPyErr(flag_epacing); return sim_clean();
+                    }
+                    t_proposed = ESys_GetNextTime(epacing, NULL);
+                    tnext = fmin(tnext, t_proposed);
+                    pacing[i] = ESys_GetLevel(epacing, NULL);
+                }
             }
 
             /* Dynamic logging: Log every visited point */
             if (dynamic_logging) {
 
+                /* Benchmarking? Then set realtime */
+                if (log_realtime) {
+                    realtime = benchmarker_realtime();
+                    if (realtime < 0) return sim_cleanx(PyExc_Exception, "Failed to set realtime during dynamic logging.");
+                }
+
                 /* Ensure the logged values are correct for the new time t */
-                if (log_deriv || log_inter) {
+                if (model->logging_derivatives || model->logging_intermediary || model->has_sensitivities) {
                     /* If logging derivatives or intermediaries, calculate the
-                       values for the current time. */
-                    rhs(engine_time, y, dy_log, 0);
-                } else if (log_bound) {
+                       values for the current time. Similarly, if calculating
+                       sensitivities this is needed. */
+                    #ifdef MYOKIT_DEBUG_MESSAGES
+                    printf("CM Calling RHS to log derivs/inter/sens at time %g.\n", t);
+                    #endif
+                    rhs(t, y, NULL, udata);
+                } else if (model->logging_bound) {
                     /* Logging bounds but not derivs or inters: No need to run
                        full rhs, just update bound variables */
-                    update_bindings(engine_time, y, dy_log, 0);
-                }
-
-                /* Benchmarking? Then set engine_realtime */
-                if (benchtime != Py_None) {
-                    flt = PyObject_CallFunction(benchtime, "");
-                    if (!PyFloat_Check(flt)) {
-                        Py_XDECREF(flt); flt = NULL;
-                        PyErr_SetString(PyExc_Exception, "Call to benchmark time function didn't return float.");
-                        return sim_clean();
-                    }
-                    engine_realtime = PyFloat_AsDouble(flt) - engine_starttime;
-                    Py_DECREF(flt); flt = NULL;
-                    /* Update any variables bound to realtime */
-                    update_realtime_bindings(engine_time, y, dy_log, 0);
+                    Model_SetBoundVariables(model, (realtype)t, (realtype*)pacing, (realtype)realtime, (realtype)evaluations);
                 }
 
                 /* Write to log */
-                for(i=0; i<n_vars; i++) {
-                    flt = PyFloat_FromDouble(*vars[i]);
-                    ret = PyObject_CallMethodObjArgs(logs[i], list_update_str, flt, NULL);
-                    Py_DECREF(flt); flt = NULL;
-                    Py_XDECREF(ret);
-                    if (ret == NULL) {
-                        PyErr_SetString(PyExc_Exception, "Call to append() failed on logging list.");
-                        return sim_clean();
-                    }
-                    ret = NULL;
-                }
+                flag_model = Model_Log(model);
+                if (flag_model != Model_OK) { Model_SetPyErr(flag_model); return sim_clean(); }
 
+                if (model->has_sensitivities) {
+                    /* Calculate sensitivities to output */
+                    shs(sy);
+
+                    /* Write sensitivity matrix to list */
+                    flag_model = Model_LogSensitivityMatrix(model, sens_list);
+                    if (flag_model != Model_OK) { Model_SetPyErr(flag_model); return sim_clean(); }
+                }
             }
 
-            /* Reinitialize if needed (cvode-mode only) */
-            #if USE_CVODE
-            if (flag_reinit) {
-                flag_reinit = 0;
-                /* Re-init */
-                flag_cvode = CVodeReInit(cvode_mem, engine_time, y);
+            /*
+             * Reinitialize CVODE if needed
+             */
+            if (model->is_ode && flag_reinit) {
+                flag_cvode = CVodeReInit(cvode_mem, t, y);
                 if (check_cvode_flag(&flag_cvode, "CVodeReInit", 1)) return sim_clean();
+                if (model->has_sensitivities) {
+                    flag_cvode = CVodeSensReInit(cvode_mem, CV_SIMULTANEOUS, sy);
+                    if (check_cvode_flag(&flag_cvode, "CVodeSensReInit", 1)) return sim_clean();
+                }
+                flag_reinit = 0;
             }
-            #endif
         }
 
-        /* Check if we're finished */
-        if (ESys_eq(engine_time, tmax)) engine_time = tmax;
-        if (engine_time >= tmax) break;
+        /*
+         * Check if we're finished
+         */
+        if (ESys_eq(t, tmax)) t = tmax;
+        if (t >= tmax) break;
 
-        /* Perform any Python signal handling */
+        /*
+         * Perform any Python signal handling
+         */
         if (PyErr_CheckSignals() != 0) {
             /* Exception (e.g. timeout or keyboard interrupt) occurred?
                Then cancel everything! */
             return sim_clean();
         }
 
-        /* Report back to python after every x steps */
+        /*
+         * Report back to python after every x steps
+         */
         steps_taken++;
         if (steps_taken >= 100) {
-            return PyFloat_FromDouble(engine_time);
+            #ifdef MYOKIT_DEBUG_PROFILING
+            benchmarker_print("CP Completed 100 steps, passing control back to Python.");
+            #endif
+            // Return new reference
+            return PyFloat_FromDouble(t);
         }
     }
+    #ifdef MYOKIT_DEBUG_PROFILING
+    benchmarker_print("CP Completed remaining simulation steps.");
+    #endif
+
+    /*
+     * Finished! Set final state
+     */
 
     /* Set final state */
-    for(i=0; i<N_STATE; i++) {
-        PyList_SetItem(state_out, i, PyFloat_FromDouble(NV_Ith_S(y, i)));
-        /* PyList_SetItem steals a reference: no need to decref the double! */
+    for (i=0; i<model->n_states; i++) {
+        PyList_SetItem(state_py, i, PyFloat_FromDouble(NV_Ith_S(y, i)));
+        /* PyList_SetItem steals a reference: no need to decref the PyFloat */
     }
 
-    /* Set state of inputs */
-    PyList_SetItem(inputs, 0, PyFloat_FromDouble(engine_time));
-    PyList_SetItem(inputs, 1, PyFloat_FromDouble(engine_pace));
-    PyList_SetItem(inputs, 2, PyFloat_FromDouble(engine_realtime));
-    PyList_SetItem(inputs, 3, PyFloat_FromDouble(engine_evaluations));
+    /* Set final sensitivities */
+    if (model->has_sensitivities) {
+        for (i=0; i<model->ns_independents; i++) {
+            val = PyList_GetItem(s_state_py, i); /* Borrowed */
+            for (j=0; j<model->n_states; j++) {
+                PyList_SetItem(val, j, PyFloat_FromDouble(NV_Ith_S(sy[i], j)));
+            }
+        }
+    }
+
+    /* Set bound variable values */
+    PyList_SetItem(bound_py, 0, PyFloat_FromDouble(t));
+    PyList_SetItem(bound_py, 1, PyFloat_FromDouble(realtime));
+    PyList_SetItem(bound_py, 2, PyFloat_FromDouble((double)evaluations));
+    for (int i = 0; i < n_pace; i++) {
+        PyList_SetItem(bound_py, 3 + i, PyFloat_FromDouble(pacing[i]));
+    }
+
+    #ifdef MYOKIT_DEBUG_PROFILING
+    benchmarker_print("CP Set final state and bound variable values.");
+    #endif
 
     sim_clean();    /* Ignore return value */
-    return PyFloat_FromDouble(engine_time);
+    return PyFloat_FromDouble(t);  // Return new reference
 }
 
 /*
  * Evaluates the state derivatives at the given state
  */
-static PyObject*
+PyObject*
 sim_eval_derivatives(PyObject *self, PyObject *args)
 {
     /* Declare variables here for C89 compatibility */
     int i;
     int success;
-    int iState;
-    int flag_cvode;
     double time_in;
-    double pace_in;
-    char errstr[200];
+    PyObject *pace_in;
+    double *pacing_in;
+    Model model;
+    Model_Flag flag_model;
     PyObject *state;
     PyObject *deriv;
-    PyObject *flt;
-    N_Vector y;
-    N_Vector dy;
-    #if SUNDIALS_VERSION_MAJOR >= 6
-    SUNContext sundials_context;
-    #endif
+    PyObject *literals;
+    PyObject *parameters;
+    PyObject *val;
 
     /* Start */
     success = 0;
 
     /* Check input arguments */
-    if (!PyArg_ParseTuple(args, "OOdd", &state, &deriv, &time_in, &pace_in)) {
-        PyErr_SetString(PyExc_Exception, "Expecting sequence arguments 'y' and 'dy' followed by floats 'time' and 'pace'.");
+    /* Check input arguments     0123456789ABCDEF*/
+    if (!PyArg_ParseTuple(args, "dOOOOO",
+            &time_in,           /* 0. Float: time */
+            &pace_in,           /* 1. List: pace */
+            &state,             /* 2. List: state */
+            &deriv,             /* 3. List: store derivatives here */
+            &literals,          /* 4. List: literal constant values */
+            &parameters         /* 5. List: parameter values */
+            )) {
+        PyErr_SetString(PyExc_Exception, "Incorrect input arguments in sim_eval_derivatives.");
         /* Nothing allocated yet, no pyobjects _created_, return directly */
         return 0;
     }
-    if (!PySequence_Check(state)) {
-        PyErr_SetString(PyExc_Exception, "First argument must support the sequence interface.");
+
+    /* Check lists are sequences */
+    if (!PyList_Check(pace_in)) {
+        PyErr_SetString(PyExc_Exception, "Pace argument must be a list.");
+        return 0;
+    }
+    if (!PyList_Check(state)) {
+        PyErr_SetString(PyExc_Exception, "State argument must be a list.");
         return 0;
     }
-    if (!PySequence_Check(deriv)) {
-        PyErr_SetString(PyExc_Exception, "Second argument must support the sequence interface.");
+    if (!PyList_Check(deriv)) {
+        PyErr_SetString(PyExc_Exception, "Derivatives argument must be a list.");
+        return 0;
+    }
+    if (!PyList_Check(literals)) {
+        PyErr_SetString(PyExc_Exception, "Literals argument must be a list.");
+        return 0;
+    }
+    if (!PyList_Check(parameters)) {
+        PyErr_SetString(PyExc_Exception, "Parameters argument must be a list.");
         return 0;
     }
 
     /* From this point on, no more direct returning: use goto error */
-    y = NULL;      /* A cvode SERIAL vector */
-    dy = NULL;     /* A cvode SERIAL vector */
-
-    /* Create sundials context */
-    #if SUNDIALS_VERSION_MAJOR >= 6
-    flag_cvode = SUNContext_Create(NULL, &sundials_context);
-    if (check_cvode_flag(&flag_cvode, "SUNContext_Create", 1)) {
-        PyErr_SetString(PyExc_Exception, "Failed to create Sundials context.");
-        goto error;
-    }
-    #endif
+    model = NULL;
 
     /* Temporary object: decref before re-using for another var :) */
     /* (Unless you get them using PyList_GetItem...) */
-    flt = NULL;   /* PyFloat */
+    val = NULL;
 
-    /* Create state vectors */
-    #if SUNDIALS_VERSION_MAJOR >= 6
-    y = N_VNew_Serial(N_STATE, sundials_context);
-    #else
-    y = N_VNew_Serial(N_STATE);
-    #endif
-    if (check_cvode_flag((void*)y, "N_VNew_Serial", 0)) {
-        PyErr_SetString(PyExc_Exception, "Failed to create state vector.");
+    /* Create model */
+    model = Model_Create(&flag_model);
+    if (flag_model != Model_OK) {
+        Model_SetPyErr(flag_model);
         goto error;
     }
-    #if SUNDIALS_VERSION_MAJOR >= 6
-    dy = N_VNew_Serial(N_STATE, sundials_context);
-    #else
-    dy = N_VNew_Serial(N_STATE);
-    #endif
-    if (check_cvode_flag((void*)dy, "N_VNew_Serial", 0)) {
-        PyErr_SetString(PyExc_Exception, "Failed to create state derivatives vector.");
+
+    flag_model = Model_SetupPacing(model, n_pace);
+    if (flag_model != Model_OK) {
+        Model_SetPyErr(flag_model);
         goto error;
     }
 
-    /* Set calculated constants */
-    updateConstants();
+    /* Set pacing values */
+    pacing_in = (double*)malloc((size_t)n_pace * sizeof(double));
+    for (int i = 0; i < n_pace; i++) {
+        val = PyList_GetItem(pace_in, i); /* Don't decref */
+        if (!PyFloat_Check(val)) {
+            PyErr_Format(PyExc_Exception, "Item %d in pace vector is not a float.", i);
+            goto error;
+        }
+        pacing_in[i] = PyFloat_AsDouble(val);
+    }
 
-    /* Set initial values */
-    for (iState = 0; iState < N_STATE; iState++) {
-        flt = PySequence_GetItem(state, iState); /* Remember to decref! */
-        if (!PyFloat_Check(flt)) {
-            Py_XDECREF(flt); flt = NULL;
-            sprintf(errstr, "Item %d in state vector is not a float.", iState);
-            PyErr_SetString(PyExc_Exception, errstr);
+    /* Set bound variables */
+    Model_SetBoundVariables(model, (realtype)time_in, (realtype*)pacing_in, 0, 0);
+
+    /* Set literal values */
+    for (i=0; i<model->n_literals; i++) {
+        val = PyList_GetItem(literals, i);    /* Don't decref */
+        if (!PyFloat_Check(val)) {
+            PyErr_Format(PyExc_Exception, "Item %d in literal vector is not a float.", i);
             goto error;
         }
-        NV_Ith_S(y, iState) = PyFloat_AsDouble(flt);
-        Py_DECREF(flt);
+        model->literals[i] = PyFloat_AsDouble(val);
     }
-    flt = NULL;
 
-    /* Set simulation time and pacing variable */
-    engine_time = time_in;
-    engine_pace = pace_in;
+    /* Evaluate literal-derived variables */
+    Model_EvaluateLiteralDerivedVariables(model);
+
+    /* Set parameter values */
+    for (i=0; i<model->n_parameters; i++) {
+        val = PyList_GetItem(parameters, i);    /* Don't decref */
+        if (!PyFloat_Check(val)) {
+            PyErr_Format(PyExc_Exception, "Item %d in parameter vector is not a float.", i);
+            goto error;
+        }
+        model->parameters[i] = PyFloat_AsDouble(val);
+    }
+
+    /* Evaluate parameter-derived variables */
+    Model_EvaluateParameterDerivedVariables(model);
+
+    /* Set initial values */
+    for (i=0; i < model->n_states; i++) {
+        val = PyList_GetItem(state, i); /* Don't decref */
+        if (!PyFloat_Check(val)) {
+            PyErr_Format(PyExc_Exception, "Item %d in state vector is not a float.", i);
+            goto error;
+        }
+        model->states[i] = PyFloat_AsDouble(val);
+    }
 
     /* Evaluate derivatives */
-    rhs(engine_time, y, dy, 0);
+    Model_EvaluateDerivatives(model);
 
     /* Set output values */
-    for(i=0; i<N_STATE; i++) {
-        flt = PyFloat_FromDouble(NV_Ith_S(dy, i));
-        if (flt == NULL) {
+    for (i=0; i<model->n_states; i++) {
+        val = PyFloat_FromDouble(model->derivatives[i]);
+        if (val == NULL) {
             PyErr_SetString(PyExc_Exception, "Unable to create float.");
             goto error;
         }
-        PySequence_SetItem(deriv, i, flt);
-        Py_DECREF(flt);
+        PyList_SetItem(deriv, i, val);
+        /* PyList_SetItem steals a reference: no need to decref the double! */
     }
-    flt = NULL;
 
     /* Finished succesfully, free memory and return */
     success = 1;
 error:
-    /* Free CVODE space */
-    N_VDestroy_Serial(y);
-    N_VDestroy_Serial(dy);
-    #if SUNDIALS_VERSION_MAJOR >= 6
-    SUNContext_Free(&sundials_context);
-    #endif
+    /* Free model space */
+    Model_Destroy(model);
 
     /* Return */
     if (success) {
         Py_RETURN_NONE;
     } else {
         return 0;
     }
 }
 
 /*
- * Alters the value of a (literal) constant
+ * Change the tolerance settings
  */
-static PyObject*
-sim_set_constant(PyObject *self, PyObject *args)
+PyObject*
+sim_set_tolerance(PyObject *self, PyObject *args)
 {
-    double value;
-    char* name;
-    char errstr[200];
+    /* Check input arguments */
+    double tabs, trel;
+    if (!PyArg_ParseTuple(args, "dd", &tabs, &trel)) {
+        PyErr_SetString(PyExc_Exception, "Expected input arguments: abs_tol(float), rel_tol(float).");
+        return 0;
+    }
+    abs_tol = tabs;
+    rel_tol = trel;
+    Py_RETURN_NONE;
+}
 
+/*
+ * Change the maximum step size (0 for none)
+ */
+PyObject*
+sim_set_max_step_size(PyObject *self, PyObject *args)
+{
     /* Check input arguments */
-    if (!PyArg_ParseTuple(args, "sd", &name, &value)) {
-        PyErr_SetString(PyExc_Exception, "Expected input arguments: name (str), value (Float).");
-        /* Nothing allocated yet, no pyobjects _created_, return directly */
+    double tmax;
+    if (!PyArg_ParseTuple(args, "d", &tmax)) {
+        PyErr_SetString(PyExc_Exception, "Expected input argument: tmax(float).");
         return 0;
     }
+    dt_max = tmax;
+    Py_RETURN_NONE;
+}
 
-<?
-for var in model.variables(const=True, deep=True):
-    if var.is_literal():
-        print(tab + 'if(strcmp("' + var.qname() + '", name) == 0) {')
-        print(tab + tab + v(var) + ' = value;')
-        print(tab + tab + 'Py_RETURN_NONE;')
-        print(tab + '}')
-?>
-    sprintf(errstr, "Constant not found: <%s>", name);
-    PyErr_SetString(PyExc_Exception, errstr);
-    return 0;
+/*
+ * Change the minimum step size (0 for none)
+ */
+PyObject*
+sim_set_min_step_size(PyObject *self, PyObject *args)
+{
+    /* Check input arguments */
+    double tmin;
+    if (!PyArg_ParseTuple(args, "d", &tmin)) {
+        PyErr_SetString(PyExc_Exception, "Expected input argument: tmin(float).");
+        return 0;
+    }
+    dt_min = tmin;
+    Py_RETURN_NONE;
 }
 
 /*
  * Returns the number of steps taken in the last simulation
  */
-static PyObject*
+PyObject*
 sim_steps(PyObject *self, PyObject *args)
 {
-    return PyLong_FromLong(engine_steps);
+    return PyLong_FromLong(steps);
 }
 
 /*
  * Returns the number of rhs evaluations performed during the last simulation
  */
-static PyObject*
+PyObject*
 sim_evals(PyObject *self, PyObject *args)
 {
-    return PyLong_FromLong(engine_evaluations);
+    return PyLong_FromLong(evaluations);
 }
 
 /*
  * Methods in this module
  */
-static PyMethodDef SimMethods[] = {
+PyMethodDef SimMethods[] = {
     {"sim_init", sim_init, METH_VARARGS, "Initialize the simulation."},
     {"sim_step", sim_step, METH_VARARGS, "Perform the next step in the simulation."},
     {"sim_clean", py_sim_clean, METH_VARARGS, "Clean up after an aborted simulation."},
     {"eval_derivatives", sim_eval_derivatives, METH_VARARGS, "Evaluate the state derivatives."},
-    {"set_constant", sim_set_constant, METH_VARARGS, "Change a (literal) constant."},
     {"set_tolerance", sim_set_tolerance, METH_VARARGS, "Set the absolute and relative solver tolerance."},
     {"set_max_step_size", sim_set_max_step_size, METH_VARARGS, "Set the maximum solver step size (0 for none)."},
     {"set_min_step_size", sim_set_min_step_size, METH_VARARGS, "Set the minimum solver step size (0 for none)."},
     {"number_of_steps", sim_steps, METH_VARARGS, "Returns the number of steps taken in the last simulation."},
     {"number_of_evaluations", sim_evals, METH_VARARGS, "Returns the number of rhs evaluations performed during the last simulation."},
     {NULL},
 };
 
 /*
  * Module definition
  */
 #if PY_MAJOR_VERSION >= 3
 
-    static struct PyModuleDef moduledef = {
-        PyModuleDef_HEAD_INIT,
-        "<?= module_name ?>",       /* m_name */
-        "Generated CVODESim module",/* m_doc */
-        -1,                         /* m_size */
-        SimMethods,                 /* m_methods */
-        NULL,                       /* m_reload */
-        NULL,                       /* m_traverse */
-        NULL,                       /* m_clear */
-        NULL,                       /* m_free */
-    };
+struct PyModuleDef moduledef = {
+    PyModuleDef_HEAD_INIT,
+    "<?= module_name ?>",       /* m_name */
+    "Generated CVODESim module",/* m_doc */
+    -1,                         /* m_size */
+    SimMethods,                 /* m_methods */
+    NULL,                       /* m_reload */
+    NULL,                       /* m_traverse */
+    NULL,                       /* m_clear */
+    NULL,                       /* m_free */
+};
 
-    PyMODINIT_FUNC PyInit_<?=module_name?>(void) {
-        return PyModule_Create(&moduledef);
-    }
+PyMODINIT_FUNC PyInit_<?=module_name?>(void) {
+    return PyModule_Create(&moduledef);
+}
 
 #else
 
-    PyMODINIT_FUNC
-    init<?=module_name?>(void) {
-        (void) Py_InitModule("<?= module_name ?>", SimMethods);
-    }
+PyMODINIT_FUNC
+init<?=module_name?>(void) {
+    (void) Py_InitModule("<?= module_name ?>", SimMethods);
+}
 
 #endif
```

### Comparing `myokit-1.33.9/myokit/_sim/cvodessim.py` & `myokit-1.34.0/myokit/_sim/cvodessim.py`

 * *Files 9% similar despite different names*

```diff
@@ -81,30 +81,30 @@
     ``time``
         This input provides the simulation time.
     ``pace``
         This input provides the current value of the pacing variable. This is
         determined using the protocol passed into the Simulation.
     ``evaluations``
         This input provides the number of rhs evaluations used at each point in
-        time and can be used to gain some insight into the solver's behaviour.
+        time and can be used to gain some insight into the solver's behavior.
     ``realtime``
         This input provides the elapsed system time at each logged point.
 
     No variable labels are required for this simulation type.
 
     **Storing and loading simulation objects**
 
     There are two ways to store Simulation objects to the file system: 1.
     using serialisation (the ``pickle`` module), and 2. using the ``path``
     constructor argument.
 
     Each time a simulation is created, a C module is compiled, imported, and
     deleted in the background. This means that part of a ``Simulation`` object
-    is a reference to an imported C extension, and cannot be serialised. When
-    using ``pickle`` to serialise the simulation, this compiled part is not
+    is a reference to an imported C extension, and cannot be serialized. When
+    using ``pickle`` to serialize the simulation, this compiled part is not
     stored. Instead, when the pickled simulation is read from disk the
     compilation is repeated. Unpickling simulations also restores their state:
     variables such as model state, simulation time, and tolerance are preserved
     when pickling.
 
     As an alternative to serialisation, Simulations can be created with a
     ``path`` variable that specifies a location where the generated module can
@@ -118,16 +118,19 @@
     file generated on one machine may not work on another.
 
     **Arguments**
 
     ``model``
         The model to simulate
     ``protocol``
-        An optional :class:`myokit.Protocol` to use as input for variables
-        bound to ``pace``.
+        A :class:`myokit.Protocol` or :class:`myokit.TimeSeriesProtocol` to use
+        for the variable with binding ``pace``. Atlernatively, a dictionary
+        mapping binding labels to :class:`myokit.Protocol` objects can be used
+        to run with multiple protocols. Finally, can be ``None`` to run without
+        a protocol.
     ``sensitivities``
         An optional tuple ``(dependents, independents)`` where ``dependents``
         is a list of variables or expressions to take derivatives of (``y`` in
         ``dy/dx``) and ``independents`` is a list of variables or expressions
         to calculate derivatives to (``x`` in ``dy/dx``).
         Each entry in ``dependents`` must be a :class:`myokit.Variable`, a
         :class:`myokit.Name`, a :class:`myokit.Derivative`, or a string with
@@ -154,23 +157,42 @@
         # Require a valid model
         if not model.is_valid():
             model.validate()
         self._model = model.clone()
         del model
 
         # Set protocol
-        self._protocol = None
-        self._fixed_form_protocol = None
-        self.set_protocol(protocol)
-        del protocol
+        self._protocols = []
+        self._pacing_labels = []
+        if isinstance(protocol, (myokit.Protocol, myokit.TimeSeriesProtocol)):
+            protocol = {'pace': protocol}
+        elif protocol is None:
+            # TODO: This can be an empty dict once #320 is resolved
+            protocol = {'pace': None}
+        for label, protocol in protocol.items():
+            self._pacing_labels.append(label)
+            self._protocols.append(myokit.Protocol())
+            self.set_protocol(protocol, label)
 
         # Generate C Model code, get sensitivity and constants info
-        cmodel = myokit.CModel(self._model, sensitivities)
+        cmodel = myokit.CModel(self._model, self._pacing_labels, sensitivities)
         if cmodel.has_sensitivities:
             self._sensitivities = (cmodel.dependents, cmodel.independents)
+
+            # Check for sensitivities w.r.t. variables used in initial state
+            # expressions. This is not implemented yet.
+            inits = self._model.initial_values()
+            for i in self._sensitivities[1]:  # Expressions
+                if isinstance(i, myokit.Name):
+                    for e in inits:
+                        if e.depends_on(i, deep=True):
+                            raise NotImplementedError(
+                                'Sensitivities with respect to parameters used'
+                                ' in initial conditions is not implemented ('
+                                + e.code() + ' depends on ' + i.code() + ').')
         else:
             self._sensitivities = None
 
         # Ordered dicts mapping Variable objects to float values
         self._literals = OrderedDict()
         self._parameters = OrderedDict()
         for var, eq in cmodel.literals.items():
@@ -182,27 +204,27 @@
         if type(path) == tuple:
             path, self._sim = path
         else:
             self._create_simulation(cmodel.code, path)
         del cmodel
 
         # Get state and default state from model
-        self._state = self._model.state()
+        self._state = self._model.initial_values(as_floats=True)
         self._default_state = list(self._state)
 
         # Set state and default state for sensitivities
         self._s_state = self._s_default_state = None
         if self._sensitivities:
-            # Outer indice: number of independent variables
-            # Inner indice: number of states
+            # Outer index: number of independent variables
+            # Inner index: number of states
             self._s_state = []
             for expr in self._sensitivities[1]:
                 row = [0.0] * len(self._state)
                 if isinstance(expr, myokit.InitialValue):
-                    row[expr.var().indice()] = 1.0
+                    row[expr.var().index()] = 1.0
                 self._s_state.append(row)
             self._s_default_state = [list(x) for x in self._s_state]
 
         # Last state reached before error
         self._error_state = None
 
         # Starting time
@@ -277,21 +299,22 @@
             # Sensitivity constructor argument. Don't pass in expressions, as
             # they will need to pickle the variables as well, which in turn
             # will need a component, model, etc.
             sens_arg = None
             if self._sensitivities:
                 sens_arg = [[x.code() for x in y] for y in self._sensitivities]
 
-            # Store serialised name and constructor args
+            # Store serialized name and constructor args
             fname = os.path.join(d_build, '_simulation.pickle')
             import pickle
             with open(fname, 'wb') as f:
                 pickle.dump(str(name), f)
                 pickle.dump(self._model, f)
-                pickle.dump(self._protocol, f)
+                pickle.dump(self._protocols, f)
+                pickle.dump(self._pacing_labels, f)
                 pickle.dump(sens_arg, f)
 
             # Zip it all in
             with zipfile.ZipFile(path, 'w', zipfile.ZIP_DEFLATED) as f:
                 for root, dirs, files in os.walk(d_build):
                     for fname in files:
                         org = os.path.join(root, fname)
@@ -323,29 +346,35 @@
 
         # Unpack the zipped information
         d_build = tempfile.mkdtemp('myokit_build')
         try:
             with zipfile.ZipFile(path, 'r', zipfile.ZIP_DEFLATED) as f:
                 f.extractall(d_build)
 
-            # Load serialised name and constructor args
+            # Load serialized name and constructor args
             fname = os.path.join(d_build, '_simulation.pickle')
             import pickle
             with open(fname, 'rb') as f:
                 name = pickle.load(f)
                 model = pickle.load(f)
-                protocol = pickle.load(f)
+                protocols = pickle.load(f)
+                pacing_labels = pickle.load(f)
                 sensitivities = pickle.load(f)
 
             # Load module
             from myokit._sim import load_module
             module = load_module(name, d_build)
 
             # Create and return simulation
-            return Simulation(model, protocol, sensitivities, (path, module))
+            labeled_protocols = {
+                k: v for k, v in zip(pacing_labels, protocols)
+            }
+            return Simulation(
+                model, labeled_protocols, sensitivities, (path, module)
+            )
 
         finally:
             myokit.tools.rmtree(d_build, silent=True)
 
     def default_state(self):
         """
         Returns the default state.
@@ -368,36 +397,49 @@
         last state reached during that simulation.
 
         Will return ``None`` if no simulation was run or the simulation did not
         result in an error.
         """
         return list(self._error_state) if self._error_state else None
 
-    def eval_derivatives(self, y=None):
+    def eval_derivatives(self, y=None, pacing=None):
         """
         Evaluates and returns the state derivatives.
 
         The state to evaluate for can be given as ``y``. If no state is given
         the current simulation state is used.
+
+        An optional dict ``pacing`` can be passed in that maps labels to
+        numerical values. If a label is used but not provided in ``pacing``,
+        it's value will be set to 0.
         """
         # Get state
         if y is None:
             y = list(self._state)
         else:
             y = self._model.map_to_state(y)
 
+        pacing_values = [0.0] * len(self._pacing_labels)
+        if pacing is not None:
+            for k, v in pacing.items():
+                try:
+                    ki = self._pacing_labels.index(k)
+                    pacing_values[ki] = float(v)
+                except ValueError:
+                    pass
+
         # Create space to store derivatives
         dy = list(self._state)
 
         # Evaluate and return
         self._sim.eval_derivatives(
             # 0. Time
             0,
             # 1. Pace
-            0,
+            pacing_values,
             # 2. State
             y,
             # 3. Space to store the state derivatives
             dy,
             # 4. Literal values
             list(self._literals.values()),
             # 5. Parameter values
@@ -463,15 +505,15 @@
             msg)
         self._default_state = list(self._state)
         if self._sensitivities:
             # Reset to time 0, so need to reset initial-value sensitivities
             for i, expr in enumerate(self._sensitivities[1]):
                 if isinstance(expr, myokit.InitialValue):
                     self._s_state[i] = [0.0] * len(self._state)
-                    self._s_state[i][expr.var().indice()] = 1.0
+                    self._s_state[i][expr.var().index()] = 1.0
             # Update default state
             self._s_default_state = [list(x) for x in self._s_state]
 
     def __reduce__(self):
         """
         Pickles this Simulation.
 
@@ -480,24 +522,27 @@
         sens_arg = None
         if self._sensitivities:
             # Don't pass in expressions, as they'll need to pickle the
             # variables as well, which in turn will need a component, model,
             # etc.
             sens_arg = [[x.code() for x in y] for y in self._sensitivities]
 
+        protocols = {
+            k: p for k, p in zip(self._pacing_labels, self._protocols)
+        }
+
         return (
             self.__class__,
-            (self._model, self._protocol, sens_arg),
+            (self._model, protocols, sens_arg),
             (
                 self._time,
                 self._state,
                 self._default_state,
                 self._s_state,
                 self._s_default_state,
-                self._fixed_form_protocol,  # Can't be set in constructor
                 self._tolerance,
                 self._dtmin,
                 self._dtmax,
             ),
         )
 
     def reset(self):
@@ -597,16 +642,16 @@
             An optional message to pass to any progress reporter.
 
         By default, this method returns a :class:`myokit.DataLog` containing
         the logged variables.
 
         However, if sensitivity calculations are enabled a tuple is returned,
         where the first entry is the :class:`myokit.DataLog` and the second
-        entry is a matrix of sensitivities ``dy/dx``, where the first indice
-        specifies the dependent variable ``y``, and the second indice specifies
+        entry is a matrix of sensitivities ``dy/dx``, where the first index
+        specifies the dependent variable ``y``, and the second index specifies
         the independent variable ``x``.
 
         Finally, if APD calculation is enabled, the method returns a tuple
         ``(log, apds)`` or ``(log, sensitivities, apds)`` where ``apds`` is a
         :class:`myokit.DataLog` with entries ``start`` and ``duration``,
         representing the start and duration of all measured APDs.
         """
@@ -667,15 +712,15 @@
                     raise ValueError(
                         'The argument `sensitivities` must be None or a list.')
         else:
             sensitivities = None
 
         # APD measuring
         root_list = None
-        root_indice = 0
+        root_index = 0
         root_threshold = 0
         if apd_variable is None:
             if apd_threshold is not None:
                 raise ValueError(
                     'APD Threshold given but no `apd_variable` specified.')
         else:
             # Get apd variable from this model
@@ -684,15 +729,15 @@
             apd_variable = self._model.get(apd_variable)
             if not apd_variable.is_state():
                 raise ValueError(
                     'The `apd_variable` must be a state variable.')
 
             # Set up root finding
             root_list = []
-            root_indice = apd_variable.indice()
+            root_index = apd_variable.index()
             root_threshold = float(apd_threshold)
 
         # Get progress indication function (if any)
         if progress is None:
             progress = myokit._Simulation_progress
         if progress:
             if not isinstance(progress, myokit.ProgressReporter):
@@ -717,15 +762,15 @@
             # Initial state and sensitivities
             state = list(self._state)
             s_state = None
             if self._sensitivities:
                 s_state = [list(x) for x in self._s_state]
 
             # List to store final bound variables in (for debugging)
-            bound = [0, 0, 0, 0]
+            bound = [0, 0, 0] + [0] * len(self._pacing_labels)
 
             # Initialize
             if myokit.DEBUG_SP:
                 b.print('PP Ready to call sim_init.')
             self._sim.sim_init(
                 # 0. Initial time
                 tmin,
@@ -737,38 +782,36 @@
                 s_state,
                 # 4. Space to store the bound variable values
                 bound,
                 # 5. Literal values
                 list(self._literals.values()),
                 # 6. Parameter values
                 list(self._parameters.values()),
-                # 7. An event-based pacing protocol
-                self._protocol,
-                # 8. A fixed-form protocol
-                self._fixed_form_protocol,
-                # 9. A DataLog
+                # 7. Pacing protocols
+                self._protocols,
+                # 8. A DataLog
                 log,
-                # 10. The log interval, or 0
+                # 9. The log interval, or 0
                 log_interval,
-                # 11. A list of predetermind logging times, or None
+                # 10. A list of predetermind logging times, or None
                 log_times,
-                # 12. A list to store calculated sensitivities in
+                # 11. A list to store calculated sensitivities in
                 sensitivities,
-                # 13. The state variable indice for root finding (only used if
+                # 12. The state variable index for root finding (only used if
                 #     root_list is a list)
-                root_indice,
-                # 14. The threshold for root crossing (can be 0 too, only used
+                root_index,
+                # 13. The threshold for root crossing (can be 0 too, only used
                 #     if root_list is a list).
                 root_threshold,
-                # 15. A list to store calculated root crossing times and
+                # 14. A list to store calculated root crossing times and
                 #     directions in, or None
                 root_list,
-                # 16. A myokit.tools.Benchmarker or None (if not used)
+                # 15. A myokit.tools.Benchmarker or None (if not used)
                 b,
-                # 17. Boolean/int: 1 if we are logging realtime
+                # 16. Boolean/int: 1 if we are logging realtime
                 int(self._model.binding('realtime') is not None),
             )
             t = tmin
 
             # Run
             try:
                 if progress:
@@ -796,17 +839,20 @@
                 # Create long error message
                 txt = ['A numerical error occurred during simulation at'
                        ' t = ' + str(t) + '.', 'Last reached state: ']
                 txt.extend(['  ' + x for x
                             in self._model.format_state(state).splitlines()])
                 txt.append('Inputs for binding:')
                 txt.append('  time        = ' + myokit.float.str(bound[0]))
-                txt.append('  pace        = ' + myokit.float.str(bound[1]))
-                txt.append('  realtime    = ' + myokit.float.str(bound[2]))
-                txt.append('  evaluations = ' + myokit.float.str(bound[3]))
+                txt.append('  realtime    = ' + myokit.float.str(bound[1]))
+                txt.append('  evaluations = ' + myokit.float.str(bound[2]))
+                for i, label in enumerate(self._pacing_labels):
+                    txt.append(
+                        '  ' + label + ' = ' + myokit.float.str(bound[3 + i])
+                    )
                 txt.append(str(e))
 
                 # Check if state derivatives can be evaluated in Python, if
                 # not, add the error to the error message.
                 try:
                     self._model.evaluate_derivatives(state)
                 except Exception as en:
@@ -899,15 +945,15 @@
         # Update value in internal model: This is required for error handling,
         # when self._model.evaluate_derivatives is called.
         # It also ensures the modified value is retained when pickling.
         self._model.set_value(var, value)
 
     def set_default_state(self, state):
         """
-        Allows you to manually set the default state.
+        Change the default state to ``state``.
         """
         self._default_state = self._model.map_to_state(state)
 
     def set_max_step_size(self, dtmax=None):
         """
         Sets a maximum step size. To let the solver pick any step size it likes
         use ``dtmax = None``.
@@ -935,94 +981,78 @@
         self._dtmin = dtmin
 
         # Set in simulation
         self._sim.set_min_step_size(dtmin)
 
     def set_fixed_form_protocol(self, times=None, values=None):
         """
-        Configures this simulation to run with a predetermined protocol
-        instead of the usual event-based mechanism.
-
-        A 1D time-series should be given as input. During the simulation, the
-        value of the pacing variable will be determined by linearly
-        interpolating between the two nearest points in the series. If the
-        simulation time is outside the bounds of the time-series, the first or
-        last value in the series will be used.
-
-        Setting a predetermined protocol clears any previously set (event-based
-        or pre-determined) protocol. To clear all protocols, call this method
-        with `times=None`. When a simulation is run without any protocol, the
-        value of any variables bound to `pace` will be set to 0.
-
-        Arguments:
+        Sets a :class:`TimeSeriesProtocol` specified by ``times`` and
+        ``values`` for the label ``pace``.
 
-        ``times``
-            A non-decreasing array of times. If any times appear more than
-            once, only the value at the highest index will be used.
-        ``values``
-            An array of values for the pacing variable. Must have the same size
-            as ``times``.
+        This method is provided for backwards compatibility with older
+        versions, please use :meth:`set_protocol` and the
+        :class:`TimeSeriesProtocol` class instead.
+        """
+        # Deprecated on 2023-06-02
+        import warnings
+        warnings.warn(
+            'The method `myokit.Simulation.set_fixed_form_protocol` is '
+            'deprecated. It will be removed in future versions of Myokit.'
+        )
 
-        """
-        # Check input
+        if times is None and values is None:
+            self.set_protocol(None)
+            return
         if times is None:
-            if values is not None:
-                raise ValueError('Values array given, but no times array.')
-        else:
-            if values is None:
-                raise ValueError('Times array given, but no values array.')
-            if len(times) != len(values):
-                raise ValueError('Times and values array must have same size.')
-
-        # Clear event-based protocol, if set
-        self._protocol = None
+            raise ValueError('No times given.')
+        if values is None:
+            raise ValueError('No values given.')
 
-        # Set new protocol
-        if times is None:
-            # Clear predetermined protocol
-            self._fixed_form_protocol = None
-        else:
-            # Copy data and set
-            self._fixed_form_protocol = (list(times), list(values))
+        self.set_protocol(myokit.TimeSeriesProtocol(times, values))
 
-    def set_protocol(self, protocol=None):
+    def set_protocol(self, protocol, label='pace'):
         """
-        Sets the pacing :class:`Protocol` used by this simulation.
+        Set an event-based pacing :class:`Protocol` or a :class:`FixedProtocol`
+        for the given ``label``.
 
-        To run without pacing call this method with ``protocol = None``. In
-        this case, the value of any variables bound to `pace` will be set to 0.
+        To remove a previously set binding call this method with ``protocol =
+        None``. In this case, the value of any variables bound to ``label``
+        will be set to 0.
+
+        The label must be one of the pacing labels set in the constructor.
         """
-        # Clear predetermined protocol, if set
-        self._fixed_form_protocol = None
+        try:
+            index = self._pacing_labels.index(label)
+        except ValueError:
+            raise ValueError('Unknown pacing label: ' + str(label))
 
         # Set new protocol
         if protocol is None:
-            self._protocol = None
+            self._protocols[index] = myokit.Protocol()
         else:
-            self._protocol = protocol.clone()
+            self._protocols[index] = protocol.clone()
 
     def __setstate__(self, state):
         """
         Called after unpickling, to set any variables not set by the
         constructor.
 
         See: https://docs.python.org/3/library/pickle.html#object.__setstate__
         """
         self._time = state[0]
         self._state = state[1]
         self._default_state = state[2]
         self._s_state = state[3]
         self._s_default_state = state[4]
-        self._fixed_form_protocol = state[5]
 
         # The following properties need to be set on the internal simulation
         # object
-        self.set_tolerance(*state[6])
-        self.set_min_step_size(state[7])
-        self.set_max_step_size(state[8])
+        self.set_tolerance(*state[5])
+        self.set_min_step_size(state[6])
+        self.set_max_step_size(state[7])
 
     def set_state(self, state):
         """
         Sets the current state.
         """
         self._state = self._model.map_to_state(state)
```

### Comparing `myokit-1.33.9/myokit/_sim/differential.hpp` & `myokit-1.34.0/myokit/_sim/differential.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
  * a and b, we can use the FirstDifferential class to calculate them:
  *
  *   // Shortcut to a FirstDifferential object:
  *   typedef FirstDifferential Diff
  *
  *   // Create a and b as differentials. Both have derivative 1 with respect to
  *   // themselves. This can be indicated explicitly or, as in this example,
- *   // using the constructor arguments (value, indice) where indice is the
- *   // indice of this variable in the list of derivatives.
+ *   // using the constructor arguments (value, index) where index is the
+ *   // index of this variable in the list of derivatives.
  *   Diff a = Diff(2, 0);
  *   Diff b = Diff(3, 1);
  *   Diff x = 5 * a + pow(b, 2);
  *
  * Now x->value or (double)x will return 13, while x[0] = 5 and x[1] = b.
  *
  * N.B.: The functions fabs, floor, ceil and fmod are implemented, but will
@@ -63,16 +63,16 @@
 
 /* C89 doesn't have NAN */
 /* https://stackoverflow.com/questions/4399641 */
 #ifndef NAN
     static const unsigned long __nan[2] = {0xffffffff, 0x7fffffff};
     #define NAN (*(const float *) __nan)
 #endif
- 
- 
+
+
 /*
  * Covector. A tiny, fixed size array class that allows addition and scalar
  * multiplication.
  */
 class Covector {
     Real data[N_DIFFS];
 public:
```

### Comparing `myokit-1.33.9/myokit/_sim/fiber_tissue.c` & `myokit-1.34.0/myokit/_sim/fiber_tissue.c`

 * *Files 1% similar despite different names*

```diff
@@ -870,15 +870,15 @@
     /* Logging: States (fiber) */
     logging_states_f = 0;
     for(i=0; i<nfy; i++) {
         for(j=0; j<nfx; j++) {
 <?
 for var in modelf.states():
     print(3*tab + 'sprintf(log_var_name, "%u.%u.' + var.qname() + '", (unsigned int)j, (unsigned int)i);' )
-    print(3*tab + 'if(log_add(log_dict_f, logs_f, vars_f, k_vars, log_var_name, &rvec_state_f[(i*nfx+j)*n_state_f+' + str(var.indice()) + '])) {')
+    print(3*tab + 'if(log_add(log_dict_f, logs_f, vars_f, k_vars, log_var_name, &rvec_state_f[(i*nfx+j)*n_state_f+' + str(var.index()) + '])) {')
     print(4*tab + 'logging_states_f = 1;')
     print(4*tab + 'k_vars++;')
     print(3*tab + '}')
 ?>
         }
     }
 
@@ -941,15 +941,15 @@
     /* Logging: States (tissue) */
     logging_states_t = 0;
     for(i=0; i<nty; i++) {
         for(j=0; j<ntx; j++) {
 <?
 for var in modelt.states():
     print(3*tab + 'sprintf(log_var_name, "%u.%u.' + var.qname() + '", (unsigned int)j, (unsigned int)i);' )
-    print(3*tab + 'if(log_add(log_dict_t, logs_t, vars_t, k_vars, log_var_name, &rvec_state_t[(i*ntx+j)*n_state_t+' + str(var.indice()) + '])) {')
+    print(3*tab + 'if(log_add(log_dict_t, logs_t, vars_t, k_vars, log_var_name, &rvec_state_t[(i*ntx+j)*n_state_t+' + str(var.index()) + '])) {')
     print(4*tab + 'logging_states_t = 1;')
     print(4*tab + 'k_vars++;')
     print(3*tab + '}')
 ?>
         }
     }
```

### Comparing `myokit-1.33.9/myokit/_sim/fiber_tissue.py` & `myokit-1.34.0/myokit/_sim/fiber_tissue.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     The simulation provides the following inputs variables can bind to:
 
     ``time`` (global)
         The simulation time
     ``pace`` (per-cell)
         The pacing level, this is set if a protocol was passed in.
     ``diffusion_current`` (per-cell)
-        The current flowing from the cell to its neighbours. This will be
+        The current flowing from the cell to its neighbors. This will be
         positive when the cell is acting as a source, negative when it is
         acting as a sink.
 
     The variable ``time`` is set globally, meaning each cell uses the same
     value. The variables ``pace`` and ``diffusion_current`` have different
     values per cell.
 
@@ -299,27 +299,27 @@
                              ' diffusion current.')
         if ucf != uct:
             raise ValueError(
                 'The diffusion current must have the same unit in the fiber'
                 ' and the tissue model: ' + str(ucf) + ' vs ' + str(uct) + '.')
 
         # Set state and default state
-        self._statef = self._modelf.state() * self._ntotalf
-        self._statet = self._modelt.state() * self._ntotalt
+        self._statef = self._modelf.initial_values(True) * self._ntotalf
+        self._statet = self._modelt.initial_values(True) * self._ntotalt
         self._default_statef = list(self._statef)
         self._default_statet = list(self._statet)
 
         # Process bindings, remove unsupported bindings, get map of bound
         # variables to internal names.
-        self._bound_variablesf = self._modelf.prepare_bindings({
+        self._bound_variablesf = myokit._prepare_bindings(self._modelf, {
             'time': 'time',
             'pace': 'pace',
             'diffusion_current': 'idiff',
         })
-        self._bound_variablest = self._modelt.prepare_bindings({
+        self._bound_variablest = myokit._prepare_bindings(self._modelt, {
             'time': 'time',
             'pace': 'pace',
             'diffusion_current': 'idiff',
         })
 
         # Create unique names
         self._modelf.create_unique_names()
@@ -672,15 +672,15 @@
             bound.append(b)
 
         # Get variable causing error
         var = model.get('.'.join(kfirst.split('.')[2:]))
 
         # Get value causing error
         if var.is_state():
-            value = states[1 if ifirst > 0 else 0][var.indice()]
+            value = states[1 if ifirst > 0 else 0][var.index()]
         else:
             value = bound[1 if ifirst > 0 else 0][var.qname()]
         var = var.qname()
 
         # Get time error occurred
         time = logf[time_varf][ifirst]
 
@@ -905,16 +905,16 @@
                 device,
                 kernelf,
                 kernelt,
                 self._ncellsf[0],
                 self._ncellsf[1],
                 self._ncellst[0],
                 self._ncellst[1],
-                self._vmf.indice(),
-                self._vmt.indice(),
+                self._vmf.index(),
+                self._vmt.index(),
                 self._gf[0],
                 self._gf[1],
                 self._gt[0],
                 self._gt[1],
                 self._gft,
                 self._cfx,
                 self._ctx,
```

### Comparing `myokit-1.33.9/myokit/_sim/icsim.py` & `myokit-1.34.0/myokit/formats/cellml/v2/_writer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,363 +1,372 @@
 #
-# Simulation that integrates the Jacobian to obtain the partial derivatives of
-# the state vector with respect to the initial conditions.
+# CellML 2.0 Writer: Writes a CellML Model to disk
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
 from __future__ import absolute_import, division
 from __future__ import print_function, unicode_literals
 
-import os
-import myokit
-import numpy as np
-import platform
-import warnings
+from lxml import etree
 
-# Location of C template
-SOURCE_FILE = 'icsim.cpp'
+import myokit
+import myokit.formats.cellml as cellml
 
 
-class ICSimulation(myokit.CppModule):
+def write_file(path, model):
+    """
+    Writes a CellML 2.0 model to the given path.
     """
-    Runs a forward-Euler based simulation and calculates the partial
-    derivatives of the state vector with respect to the initial conditions.
+    return CellMLWriter().write_file(path, model)
 
-    This class is deprecated. Sensitivities with respect to initial conditions
-    can now be calculated with the :class:`Simulation` class.
 
-    The simulation is based on automatic differentiation implemented using a
-    C++ data type that replaces a single scalar float with a float and a list
-    of partial derivatives. Any operations on this pair update both the float
-    and the set of derivatives. A normal simulation starts with a state
-    ``y(tmin)`` and a right-hand side function (RHS) ``f(y) = dy/dt``. It then
-    integrates ``f(y)`` from ``tmin`` to ``tmax`` resulting in an output state
-    ``y(tmax)``. In this simulation the data type of ``f`` is replaced by a
-    ``(f, df/dy)``, where ``df/dy`` is the matrix of partial derivatives of
-    ``f`` with respect to ``y``. By integrating ``f`` from ``tmin`` to ``tmax``
-    we obtain the state at ``tmax``. This can be seen as a function
-    ``F(y(tmin))``, that gives the state at ``tmax`` given ``y(tmin)``. By
-    integrating ``df/dy`` the derivative of ``F`` to ``y(tmin)`` is obtained.
-    This result allows the sensitivity of the system to its initial conditions
-    to be evaluated.
-
-    N.B. The partial derivatives can not be calculated for the following
-    functions: ``floor``, ``ceil``, ``abs``, quotients and remainders. If these
-    are encountered the resulting derivatives will be yielded as ``NaN``.
-    However, in many cases, these functions will only occur as part of a
-    condition in an if statement, so the ``NaN``'s won't propagate to the final
-    result.
-
-    The model passed to the simulation is cloned and stored internally, so
-    changes to the original model object will not affect the simulation.
-
-    A protocol can be passed in as ``protocol`` or set later using
-    :meth:`set_protocol`.
-
-    Simulations maintain an internal state consisting of
-
-    - the current simulation time
-    - the current state
-    - the derivatives of the current state with respect to the initial state
-
-    When a simulation is created, the simulation time is set to 0 and the
-    state is obtained from the given model. The initial derivatives matrix is
-    an identity matrix of size ``(n, n)``, where ``n`` is the number of states
-    in the model.
-    After each call to :meth:`run` the time, state and derivative variables are
-    updated so that each successive call to run continues where the previous
-    one left off. A :meth:`reset` method is provided that will set the
-    time back to 0, revert the current state to the default state and set the
-    derivatives back to ``I``.
-
-    The simulation provides two inputs a variable can bind to:
-
-    ``time``
-        This variable contains the simulation time.
-    ``pace``
-        This variable contains the current value of the pacing variable
-        as given by the protocol passed to the Simulation.
+def write_string(model):
+    """
+    Writes a CellML 2.0 model to a string and returns it.
+    """
+    return CellMLWriter().write_string(model)
+
 
-    No labeled variables are required.
+class CellMLWriter(object):
+    """
+    Writes CellML 2.0 documents.
     """
-    _index = 0  # Simulation id
 
-    def __init__(self, model, protocol=None):
-        super(ICSimulation, self).__init__()
+    # List of si unit names corresponding to myokit.Unit exponents
+    _exp_si = None
+
+    # Note: Most items are sorted, to get closer to a 'canonical form' CellML
+    # document: https://github.com/cellml/libcellml/issues/289
 
-        # Deprecated on 2021-02-25
-        warnings.warn(
-            'The class `ICSimulation` is deprecated. Sensitivities with'
-            ' respect to initial conditions can now be calculated with the'
-            ' single cell myokit.Simulation class.')
-
-        # Require a valid model
-        if not model.is_valid():
-            model.validate()
-        model = model.clone()
-        self._model = model
-
-        # Set protocol
-        self.set_protocol(protocol)
-
-        # Get state and default state from model
-        self._state = self._model.state()
-        self._default_state = list(self._state)
-
-        # Create initial list of derivatives
-        n = len(self._state)
-        self._deriv = [0.0] * n**2
-        for i in range(n):
-            self._deriv[i * (n + 1)] = 1.0
-
-        # Starting time
-        self._time = 0
-
-        # Default time step
-        self._dt = 0
-        self.set_step_size()
-
-        # Unique simulation id
-        ICSimulation._index += 1
-        module_name = 'myokit_ICSimulation_' + str(ICSimulation._index)
-        module_name += '_' + str(myokit.pid_hash())
-
-        # Arguments
-        args = {
-            'module_name': module_name,
-            'model': self._model,
-        }
-        fname = os.path.join(myokit.DIR_CFUNC, SOURCE_FILE)
-
-        # Define libraries
-        libs = []
-        if platform.system() != 'Windows':  # pragma: no windows cover
-            libs.append('m')
-
-        # Create simulation
-        libd = []
-        incd = [myokit.DIR_CFUNC]
-        self._sim = self._compile(module_name, fname, args, libs, libd, incd)
-
-    def block(self, log, derivatives):
+    def _component(self, parent, component, voi):
         """
-        Takes the output of a simulation (a simulation log and a list of
-        derivatives) and combines it into a single :class:`DataBlock2d` object.
+        Adds an etree ``Element`` to a ``parent`` element, representing the
+        given CellML ``component``.
+        """
+
+        # Create component element
+        element = etree.SubElement(parent, 'component')
+        element.attrib['name'] = component.name()
 
-        Each entry in the log is converted to a 0d entry in the log. The
-        calculated derivatives are stored as the 2d field ``derivatives``.
+        # Add variables
+        for variable in sorted(component.variables(), key=_name):
+            self._variable(element, variable)
+
+        # Add maths
+        self._maths(element, component, voi)
+
+    def _connections(self, parent, model):
+        """
+        Adds ``connections`` elements to the given ``parent`` tag for all
+        connections needed in ``model``.
         """
-        # Get time data
-        tvar = self._model.time().qname()
-        try:
-            time = log[tvar]
-        except KeyError:
-            raise ValueError(
-                'The given log must contain an entry for <' + tvar + '>.')
-
-        # Check shape of derivatives array
-        n = self._model.count_states()
-        shape = (len(time), n, n)
-        if derivatives.shape != shape:
-            raise ValueError(
-                'Wrong input: Expecting a derivatives array of shape '
-                + str(shape) + '.')
-
-        # Create datablock
-        block = myokit.DataBlock2d(n, n, time)
-        for k, v in log.items():
-            if k != tvar:
-                block.set0d(k, v)
-        block.set2d('derivatives', derivatives)
-        return block
-
-    def default_state(self):
-        """
-        Returns the default state.
-        """
-        return list(self._default_state)
-
-    def derivatives(self):
-        """
-        Return the partial derivatives of the current state with respect to the
-        initial state.
-        """
-        n = len(self._state)
-        return np.array(self._deriv, copy=True).reshape((n, n))
-
-    def reset(self):
-        """
-        Resets the simulation:
-
-        - The time variable is set to 0
-        - The state is set back to the default state
-
-        """
-        # Reset time
-        self._time = 0
-
-        # Reset state
-        self._state = list(self._default_state)
-
-        # Reset derivatives
-        n = len(self._state)
-        self._deriv = [0.0] * n**2
-        for i in range(n):
-            self._deriv[i * (n + 1)] = 1.0
-
-    def run(self, duration, log=None, log_interval=5, progress=None,
-            msg='Running ICSimulation'):
-        """
-        Runs a simulation and returns the logged results. Running a simulation
-        has the following effects:
-
-        - The internal state is updated to the last state in the simulation.
-        - The simulation's time variable is updated to reflect the time
-          elapsed during the simulation.
-
-        The number of time units to simulate can be set with ``duration``.
-
-        The variables to log can be indicated using the ``log`` argument. There
-        are several options for its value:
-
-        - ``None`` (default), to log all states.
-        - An integer flag or a combination of flags. Options:
-          ``myokit.LOG_NONE``, ``myokit.LOG_STATE``, ``myokit.LOG_INTER``,
-          ``myokit.LOG_BOUND``.
-        - A list of qnames or variable objects
-        - A :class:`myokit.DataLog` obtained from a previous simulation.
-          In this case, the newly logged data will be appended to the existing
-          log.
-
-        For more details on the ``log`` argument, see the function
-        :meth:`myokit.prepare_log`.
-
-        The method returns a :class:`myokit.DataLog` and a 3d numpy
-        array. In the returned array, the first axis represents the time,
-        the second axis is a state x and the third is a state y such that the
-        point ``(t, x, y)`` represents ``dx/dy(0)`` at time t. For example, if
-        ``p`` is the array of derivatives, to get the derivative of state 0
-        with respect to the initial value of state 1, use ``p[:,0,1]``.
-
-        A log entry is created every time *at least* ``log_interval`` time
-        units have passed.
-
-        To obtain feedback on the simulation progress, an object implementing
-        the :class:`myokit.ProgressReporter` interface can be passed in.
-        passed in as ``progress``. An optional description of the current
-        simulation to use in the ProgressReporter can be passed in as `msg`.
-        """
-        # Simulation times
-        if duration < 0:
-            raise ValueError('Simulation time can\'t be negative.')
-        tmin = self._time
-        tmax = tmin + duration
-
-        # Parse log argument
-        log = myokit.prepare_log(
-            log,
-            self._model,
-            if_empty=myokit.LOG_STATE + myokit.LOG_BOUND,
-            allowed_classes=myokit.LOG_STATE + myokit.LOG_BOUND
-            + myokit.LOG_INTER,
-        )
 
-        # Logging period (0 = disabled)
-        log_interval = float(log_interval)
-        if log_interval < 0:
-            log_interval = 0
-
-        # Create empty list for derivative lists
-        derivs = []
-
-        # Get progress indication function (if any)
-        if progress is None:
-            progress = myokit._Simulation_progress
-        if progress:
-            if not isinstance(progress, myokit.ProgressReporter):
-                raise ValueError(
-                    'The argument "progress" must be either a subclass of'
-                    ' myokit.ProgressReporter or None.')
-
-        # Run simulation
-        if duration > 0:
-            # Initialize
-            n = len(self._state)
-            state = [0] * n
-            deriv = [0] * (n ** 2)
-            self._sim.sim_init(
-                tmin,
-                tmax,
-                self._dt,
-                list(self._state),
-                list(self._deriv),
-                state,
-                deriv,
-                self._protocol,
-                log,
-                derivs,
-                log_interval,
-            )
-            t = tmin
+        # Create a dictionary where each key is a pair
+        # ``(component_1, component_2)`` ordered alphabetically by name, and
+        # each value is a (non-empty) list of ``(variable_1, variable_2)``
+        # pairs, such that ``variable_1`` is in ``component_1`` and
+        # ``variable_2`` is in ``component_2``.
+        connections = {}
+
+        # Scan all connections
+        for v1, v2 in model.connections():
+            c1 = v1.component()
+            c2 = v2.component()
+
+            # Order components alphabetically
+            if c2.name() < c1.name():
+                c1, c2 = c2, c1
+                v1, v2 = v2, v1
+
+            # Store the connection
             try:
-                if progress:
-                    # Loop with feedback
-                    with progress.job(msg):
-                        r = 1 / duration
-                        while t < tmax:
-                            t = self._sim.sim_step()
-                            if not progress.update(min((t - tmin) * r, 1)):
-                                raise myokit.SimulationCancelledError()
-                else:
-                    # Loop without feedback
-                    while t < tmax:
-                        t = self._sim.sim_step()
-            finally:
-                # Clean even after KeyboardInterrupt or other Exception
-                self._sim.sim_clean()
-            # Update internal state
-            self._state = list(state)
-            self._deriv = list(deriv)
-            self._time += duration
-            # Convert derivatives to numpy arrays
-            # Using
-            #   derivs = [np.array(x).reshape(n,n) for x in derivs]
-            # will create a list of views of arrays
-            # to avoid the overhead of views, perhaps it's better to copy this
-            # view into a new array explicitly?
-            derivs = np.array([
-                np.array(np.array(x).reshape(n, n), copy=True) for x in derivs
-            ])
-
-        # Return
-        return log, derivs
-
-    def set_protocol(self, protocol=None):
-        """
-        Changes the pacing protocol used by this simulation.
-        """
-        if protocol is None:
-            self._protocol = None
-        else:
-            self._protocol = protocol.clone()
-
-    def set_step_size(self, dt=0.01):
-        """
-        Sets the step size used in the forward Euler solving routine.
-        """
-        dt = float(dt)
-        if dt <= 0:
-            raise ValueError('Step size must be greater than zero.')
-        self._dt = dt
-
-    def state(self):
-        """
-        Returns the current state.
+                vrs = connections[(c1, c2)]
+            except KeyError:
+                connections[(c1, c2)] = vrs = set()
+            vrs.add((v1, v2))
+
+        # Add elements
+        for cs, vs in sorted(connections.items(), key=lambda x: _names(x[0])):
+
+            # Add connection
+            connection = etree.SubElement(parent, 'connection')
+            connection.attrib['component_1'] = cs[0].name()
+            connection.attrib['component_2'] = cs[1].name()
+
+            # Add variables
+            for v1, v2 in sorted(vs, key=_names):
+                map_variables = etree.SubElement(connection, 'map_variables')
+                map_variables.attrib['variable_1'] = v1.name()
+                map_variables.attrib['variable_2'] = v2.name()
+
+    def _encapsulation(self, parent, model):
+        """
+        Adds an ``encapsulation`` element to ``parent`` that contains all
+        encapsulation relationships present in the given ``model``.
+        """
+
+        # Check if this model has encapsulation relationships, if not: return
+        has_encapsulation = False
+        for component in model:
+            if component.parent() is not None:
+                has_encapsulation = True
+                break
+        if not has_encapsulation:
+            return
+
+        # Create element
+        element = etree.SubElement(parent, 'encapsulation')
+
+        # Add all unencapsulated components that have children
+        for component in sorted(model, key=_name):
+            if component.parent() is None and component.has_children():
+                self._encapsulation_component_ref(element, component)
+
+    def _encapsulation_component_ref(self, parent, component):
+        """
+        Adds a ``component_ref`` element for ``component`` to ``parent``, and
+        then recurses to any children of the component.
+        """
+
+        # Create element
+        element = etree.SubElement(parent, 'component_ref')
+        element.attrib['component'] = component.name()
+
+        # Add children
+        for child in sorted(component.children(), key=_name):
+            self._encapsulation_component_ref(element, child)
+
+    def _maths(self, parent, component, voi):
+        """
+        Adds a ``math`` element to the given ``parent`` containing the maths
+        for the variables in ``component``.
+
+        Derivatives will be written with reference to a local variable in the
+        connected variable set of the variable of integration ``voi``.
+        """
+
+        # Test if this component has maths
+        has_maths = False
+        for v in component:
+            if v.rhs() is not None:
+                has_maths = True
+                break
+        if not has_maths:
+            return
+
+        # Find local alias of the variable of integration (in valid models,
+        # this will always be set if states are present in this component).
+        if voi is not None:
+            if voi.component() is not component:
+                for var in voi.connected_variables():
+                    if var.component() is component:
+                        voi = var
+                        break
+
+        # Create expression writer for this component
+        from myokit.formats.cellml import CellMLExpressionWriter
+        model = component.model()
+        ewriter = CellMLExpressionWriter(model.version())
+        ewriter.set_lhs_function(lambda x: x.var().name())
+        ewriter.set_unit_function(lambda x: model.find_units_name(x))
+        if voi is not None:
+            ewriter.set_time_variable(voi)
+
+        # Reset default namespace to MathML namespace
+        nsmap = {None: cellml.NS_MATHML}
+        #if component.model().version() == '2.0':
+        nsmap['cellml'] = cellml.NS_CELLML_2_0
+
+        # Create math elements
+        math = etree.SubElement(parent, 'math', nsmap=nsmap)
+
+        # Add maths for variables
+        for variable in sorted(component, key=_name):
+            if variable.equation_variable() is variable:
+                ewriter.eq(variable.equation(), math)
+
+    def _model(self, model):
+        """
+        Returns an etree ``Element`` representing the given ``model``.
+        """
+
+        # Load correct namespaces
+        version = model.version()
+        # if version == '2.0':
+        namespaces = {None: cellml.NS_CELLML_2_0}
+        namespaces['cellml'] = namespaces[None]
+
+        # Create model element
+        element = etree.Element('model', nsmap=namespaces)
+
+        # Set model name
+        element.attrib['name'] = model.name()
+
+        # Add units
+        for units in sorted(model.units(), key=_name):
+            self._units(element, units)
+
+        # Add components
+        voi = model.variable_of_integration()
+        for component in sorted(model, key=_name):
+            self._component(element, component, voi)
+
+        # Add connections
+        self._connections(element, model)
+
+        # Add encapsulation
+        self._encapsulation(element, model)
+
+        # Return model element
+        return element
+
+    def _units(self, parent, units):
+        """
+        Adds a ``units`` element to ``parent``, for the given CellML units
+        object.
+        """
+        # Get unit exponents on first call
+        if self._exp_si is None:
+            from myokit.formats.cellml import v2
+            self._exp_si = [
+                v2.Units._si_units_r[x] for x in myokit.Unit.list_exponents()]
+
+        # Create units element
+        element = etree.SubElement(parent, 'units')
+        element.attrib['name'] = units.name()
+
+        # Get myokit unit
+        myokit_unit = units.myokit_unit()
+
+        # Add unit row for each of the 7 SI units needed to make up this unit
+        rows = []
+        for k, e in enumerate(myokit_unit.exponents()):
+            if e != 0:
+                row = etree.SubElement(element, 'unit')
+                row.attrib['units'] = self._exp_si[k]
+                if e != 1:
+                    row.attrib['exponent'] = str(e)
+                rows.append(row)
+
+        # Handle dimensionless units with a multiplier
+        if not rows:
+            row = etree.SubElement(element, 'unit')
+            row.attrib['units'] = 'dimensionless'
+            rows.append(row)
+
+        # Add multiplier or prefix to first row
+        multiplier = myokit_unit.multiplier()
+        if multiplier != 1:
+            if myokit.float.eq(multiplier, int(multiplier)):
+                rows[0].attrib['multiplier'] = str(int(multiplier))
+            else:
+                rows[0].attrib['multiplier'] = myokit.float.str(
+                    multiplier).strip()
+
+    def _variable(self, parent, variable):
+        """
+        Adds a ``variable`` element to ``parent`` for the variable represented
+        by :class:`myokit.formats.cellml.v2.Variable` ``variable``.
+        """
+
+        # Create element
+        element = etree.SubElement(parent, 'variable')
+        element.attrib['name'] = variable.name()
+
+        # Add units
+        element.attrib['units'] = variable.units().name()
+
+        # Add interfaces
+        if variable.interface() != 'none':
+            element.attrib['interface'] = variable.interface()
+
+        # Add initial value
+        if variable is variable.initial_value_variable():
+            value = myokit.float.str(variable.initial_value()).strip()
+            if value[-4:] == 'e+00':
+                value = value[:-4]
+            element.attrib['initial_value'] = value
+
+    def write(self, model):
+        """
+        Takes a :class:`myokit.formats.cellml.v2.Model` as input, and
+        creates an ElementTree that represents it.
+
+        If the model contains any variables that have an `oxmeta` meta data
+        property, this will be annotated with RDF tags suitable for use with
+        the Cardiac Electrophysiology Web Lab.
+        """
+        # Validate model
+        model.validate()
+
+        try:
+            # Variables with an oxmeta annotation and a cmeta:id will get an
+            # annotation suitable for use with the web lab. This dict maps
+            # cmeta:id strings to oxmeta annotations.
+            self._oxmeta_variables = {}
+
+            # Temporarily store variable of integration (in valid models, this
+            # is always set if states are used).
+            self._time = model.variable_of_integration()
+
+            # Create model element (with children)
+            element = self._model(model)
+
+            # Wrap in ElementTree and return
+            return etree.ElementTree(element)
+
+        finally:
+            # Delete any temporary properties
+            del self._oxmeta_variables, self._time
+
+    def write_file(self, path, model):
+        """
+        Takes a :class:`myokit.formats.cellml.v2.Model` as input, and writes it
+        to the given ``path``.
+
+        See :meth:`write()` for details.
         """
-        return list(self._state)
 
-    def time(self):
+        # Create ElementTree
+        tree = self.write(model)
+
+        # Write to disk
+        tree.write(
+            path,
+            encoding='utf-8',
+            method='xml',
+            xml_declaration=True,
+            pretty_print=True,
+        )
+        # Note: Can use method='c14n' to get canonical output, but that also
+        # removes the xml declaration, which I quite like having!
+
+    def write_string(self, model):
         """
-        Returns the current simulation time.
+        Takes a :class:`myokit.formats.cellml.v2.Model` as input, and converts
+        it to an XML string.
+
+        See :meth:`write()` for details.
         """
-        return self._time
+
+        # Create ElementTree
+        tree = self.write(model)
+
+        # Write to string
+        return etree.tostring(
+            tree,
+            encoding='utf-8',
+            method='xml',
+            pretty_print=True,
+        )
+
+
+def _name(x):
+    """ Sort by name. """
+    return x.name()
+
+
+def _names(x):
+    """ Sort by names. """
+    return x[0].name(), x[1].name()
+
```

### Comparing `myokit-1.33.9/myokit/_sim/jacobian.cpp` & `myokit-1.34.0/myokit/_sim/jacobian.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -66,20 +66,20 @@
 
 // Define differential type.
 typedef FirstDifferential Diff;
 
 <?
 print('// Aliases of state variable derivatives')
 for var in model.states():
-    print('#define ' + v(var.lhs()) + ' deriv[' + str(var.indice()) + ']')
+    print('#define ' + v(var.lhs()) + ' deriv[' + str(var.index()) + ']')
 print('')
 
 print('// Aliases of state variable values')
 for var in model.states():
-    print('#define ' + v(var) + ' state[' + str(var.indice()) + ']')
+    print('#define ' + v(var) + ' state[' + str(var.index()) + ']')
 print('')
 
 print('// Aliases of input variables')
 for k, label in enumerate(inputs):
     print('#define ' + v(model.binding(label)) + ' inputs[' + str(k) + ']')
 print('')
```

### Comparing `myokit-1.33.9/myokit/_sim/jacobian.py` & `myokit-1.34.0/myokit/_sim/jacobian.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,14 +219,18 @@
         super(JacobianCalculator, self).__init__()
         # Require a valid model
         model.validate()
 
         # Clone model
         self._model = model.clone()
 
+        # Store the initial values (won't be able to access once time binding
+        # is removed).
+        self._state = self._model.initial_values(as_floats=True)
+
         # Unbind all inputs
         for label, var in self._model.bindings():
             var.set_binding(None)
 
         # Extension module id
         JacobianCalculator._index += 1
         module_name = 'myokit_JacobianCalculator_'
@@ -306,15 +310,15 @@
         """
         # Check damping variable
         if damping <= 0 or damping > 1:
             raise ValueError('Damping must be between 0 and 1.')
 
         # Get initial state
         if x is None:
-            x = self._model.state()
+            x = self._state
         x = np.array(x)
 
         # Calculate derivatives & jacobian
         f, j = self.calculate(x)
         e = np.max(np.abs(f))
 
         # Iterations
```

### Comparing `myokit-1.33.9/myokit/_sim/mcl.h` & `myokit-1.34.0/myokit/_sim/mcl.h`

 * *Files 1% similar despite different names*

```diff
@@ -518,15 +518,15 @@
 
 /*
  * Creates and returns a platform information dict, not including a devices
  * entry.
  *
  * Arguments:
  *  cl_platform_id platform_id  The id of the platform to query
- *  char* buffer                An initialised string buffer, that can be used
+ *  char* buffer                An initialized string buffer, that can be used
  *                              to read and write string information.
  *
  * Returns NULL and sets an error message if any exception occurs.
  */
 PyObject* mcl_info_platform_dict(cl_platform_id platform_id, size_t bufsize, char* buffer)
 {
     // Return from OpenCL
@@ -607,15 +607,15 @@
 /*
  * Creates and returns a device information dict, not including a devices
  * entry.
  *
  * Arguments:
  *  cl_device_id device_id  The id of the device to query.
  *  size_t bufsize          Size of the string `buffer`.
- *  char* buffer            An initialised string buffer, that can be used to
+ *  char* buffer            An initialized string buffer, that can be used to
  *                          read and write string information.
  *
  * Returns NULL and sets an error message if any exception occurs.
  */
 PyObject* mcl_info_device_dict(cl_device_id device_id, size_t bufsize, char* buffer)
 {
     // Return from OpenCL
```

### Comparing `myokit-1.33.9/myokit/_sim/opencl.c` & `myokit-1.34.0/myokit/_sim/opencl.c`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_sim/opencl.py` & `myokit-1.34.0/myokit/_sim/opencl.py`

 * *Files 9% similar despite different names*

```diff
@@ -284,18 +284,22 @@
         # mcl_info is a python object returned by mcl_device_info (mcl.h)
         self.platforms = tuple([OpenCLPlatformInfo(x) for x in mcl_info])
 
     def format(self):
         """
         Returns a formatted string version of this object's information.
         """
+        selected_platform, selected_device = myokit.OpenCL.load_selection()
         b = []
         for i, platform in enumerate(self.platforms):
-            b.append('Platform ' + str(i))
-            platform._format(b, pre=' ')
+            pname = 'Platform ' + str(i)
+            if platform.name == selected_platform:  # pragma: no cover
+                pname += '  <-- Selected platform in myokit.ini'
+            b.append(pname)
+            platform._format(b, selected_platform, selected_device, pre=' ')
         return '\n'.join(b)
 
 
 class OpenCLPlatformInfo(object):
     """
     Represents information about an OpenCL platform.
 
@@ -338,31 +342,34 @@
 
     def format(self):
         """
         Returns a formatted string version of this object's information.
         """
         b = []
         b.append('Platform: ' + self.name)
-        self._format(b, ' ', name=False)
+        self._format(b, pre=' ', name=False)
         return '\n'.join(b)
 
-    def _format(self, b, pre='', name=True):
+    def _format(self, b, p_selected=None, d_selected=None, pre='', name=True):
         """
         Formats the information in this object and adds it to the list ``b``.
         """
         if name:
             b.append(pre + 'Name       : ' + self.name)
         b.append(pre + 'Vendor     : ' + self.vendor)
         b.append(pre + 'Version    : ' + self.version)
         b.append(pre + 'Profile    : ' + self.profile)
         b.append(pre + 'Extensions : ' + ' '.join(self.extensions))
         if self.devices is not None:
             b.append(pre + 'Devices:')
             for j, device in enumerate(self.devices):
-                b.append(pre + ' Device ' + str(j))
+                dname = pre + ' Device ' + str(j)
+                if self.name == p_selected and device.name == d_selected:  # pragma: no cover # noqa
+                    dname += '  <-- Selected device in myokit.ini'
+                b.append(dname)
                 device._format(b, pre + '  ')
 
         if self.device is not None:
             b.append(pre[:-1] + 'Device: ' + self.device.name)
             self.device._format(b, pre, name=False)
 
     def has_extension(self, extension):
```

### Comparing `myokit-1.33.9/myokit/_sim/openclsim.c` & `myokit-1.34.0/myokit/_sim/openclsim.c`

 * *Files 0% similar despite different names*

```diff
@@ -971,15 +971,15 @@
         for(j=0; j<nx; j++) {
 <?
 for var in model.states():
     if dims == 1:
         print(3*tab + 'sprintf(log_var_name, "%u.' + var.qname() + '", (unsigned int)j);')
     else:
         print(3*tab + 'sprintf(log_var_name, "%u.%u.' + var.qname() + '", (unsigned int)j, (unsigned int)i);' )
-    print(3*tab + 'if(log_add(log_dict, logs, vars, k_vars, log_var_name, &rvec_state[(i*nx+j)*n_state+' + str(var.indice()) + '])) {')
+    print(3*tab + 'if(log_add(log_dict, logs, vars, k_vars, log_var_name, &rvec_state[(i*nx+j)*n_state+' + str(var.index()) + '])) {')
     print(4*tab + 'logging_states = 1;')
     print(4*tab + 'k_vars++;')
     print(3*tab + '}')
 ?>
         }
     }
```

### Comparing `myokit-1.33.9/myokit/_sim/openclsim.cl` & `myokit-1.34.0/myokit/_sim/openclsim.cl`

 * *Files 0% similar despite different names*

```diff
@@ -148,16 +148,16 @@
 #define n_inter <?=str(len(inter_log))?>
 
 /* Number of scalar fields */
 #define n_field <?=str(len(fields))?>
 
 <?
 if diffusion:
-    print('/* Indice of membrane potential in state vector */')
-    print('#define i_vm ' + str(model.label('membrane_potential').indice()))
+    print('/* Index of membrane potential in state vector */')
+    print('#define i_vm ' + str(model.label('membrane_potential').index()))
 
 if precision == myokit.SINGLE_PRECISION:
     print('/* Using single precision floats */')
     print('typedef float Real;')
     if connections:
         print('typedef unsigned int RealSizedUInt;')
         print('#define Myokit_cmpxchg atomic_cmpxchg')
@@ -184,15 +184,15 @@
         if not isinstance(eq.rhs, myokit.Number):
             if eq.lhs.var() not in fields:
                 print('#define ' + v(eq.lhs) + ' (' + w.ex(eq.rhs) + ')')
 
 print('')
 print('/* Aliases of state variables. */')
 for var in model.states():
-    print('#define ' + v(var) + ' state[of1 + ' + str(var.indice()) + ']')
+    print('#define ' + v(var) + ' state[of1 + ' + str(var.index()) + ']')
 
 print('')
 print('/* Aliases of logged intermediary variables. */')
 for k, var in enumerate(inter_log):
     print('#define ' + v(var) + ' inter_log[of2 + ' + str(k) + ']')
 
 print('')
```

### Comparing `myokit-1.33.9/myokit/_sim/openclsim.py` & `myokit-1.34.0/myokit/_sim/openclsim.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     The simulation provides the following inputs variables can bind to:
 
     ``time``
         The simulation time
     ``pace``
         The pacing level, this is set if a protocol was passed in.
     ``diffusion_current`` (if enabled)
-        The current flowing from the cell to its neighbours. This will be
+        The current flowing from the cell to its neighbors. This will be
         positive when the cell is acting as a source, negative when it is
         acting as a sink.
 
     The input ``time`` is set globally: Any variable bound to ``time`` will
     appear in the logs as single, global variable (for example ``engine.time``
     instead of ``1.2.engine.time``. Variables bound to ``pace`` or
     ``diffusion_current`` are logged per cell. (If diffusion currents are
@@ -99,15 +99,15 @@
     another simulation etc.
 
     To set up a 1d simulation, the argument ``ncells`` should be given as a
     tuple. In this case, any cell ``i`` will be assumed to be connected to
     cells ``i - 1`` and ``i + 1`` (except at the boundaries).
     Similarly, if ``ncells`` is a 2-dimensional tuple ``(nx, ny)`` a grid will
     be assumed so that each (non-boundary) cell is connected to four
-    neighbours.
+    neighbors.
     Finally, arbitrary geometries can be used by passing a scalar to ``ncells``
     and specifying the connections with :meth:`set_connections`.
 
     The ``diffusion_current`` in any cell is calculated as::
 
         i = sum[g * (V - V_j)]
 
@@ -268,26 +268,26 @@
         # Set initial time
         self._time = 0
 
         # Count number of states
         self._nstate = self._model.count_states()
 
         # Set state and default state
-        self._state = self._model.state() * self._ntotal
+        self._state = self._model.initial_values(True) * self._ntotal
         self._default_state = list(self._state)
 
         # List of globally logged inputs
         self._global = ['time', 'pace']
 
         # Process bindings: remove unsupported bindings, get map of bound
         # variables to internal names.
         inputs = {'time': 'time', 'pace': 'pace'}
         if self._diffusion_enabled:
             inputs['diffusion_current'] = 'idiff'
-        self._bound_variables = self._model.prepare_bindings(inputs)
+        self._bound_variables = myokit._prepare_bindings(self._model, inputs)
 
         # Create unique names
         self._model.create_unique_names()
 
         # Create back-end
         SimulationOpenCL._index += 1
         mname = 'myokit_sim_opencl_' + str(SimulationOpenCL._index)
@@ -653,15 +653,15 @@
             bounds.append(b)
 
         # Get variable causing error
         var = self._model.get('.'.join(kfirst.split('.')[ndims:]))
 
         # Get value causing error
         if var.is_state():
-            value = states[1 if ifirst > 0 else 0][var.indice()]
+            value = states[1 if ifirst > 0 else 0][var.index()]
         else:  # pragma: no cover
             value = bounds[1 if ifirst > 0 else 0][var.qname()]
         var = var.qname()
 
         # Get time error occurred
         time = log[time_var][ifirst]
 
@@ -761,17 +761,17 @@
             dV/dt = -1/Cm (I_ion + I_stim + I_diff)
 
         where Cm is membrane capacitance and the diffusion current is defined
         by::
 
             I_diff[i] = sum[g[i,j] * (V[i] - V[j])]
 
-        in which the sum is over all neighbours ``j`` of cell ``i``.
+        in which the sum is over all neighbors ``j`` of cell ``i``.
 
-        Alternatively, with capacitance and currents normalised to membrane
+        Alternatively, with capacitance and currents normalized to membrane
         area, we can write::
 
             dV/dt = -1/cm (i_ion + i_stim + i_diff)
 
         In the monodomain model (see e.g. [4]), this diffusion current per unit
         area is defined as::
 
@@ -783,18 +783,18 @@
         assume **zero-flux boundary conditions**, a **regularly spaced grid**,
         and **no spatial heterogeneity in D** (or g).
 
         With these assumptions, we can use finite differences to find::
 
             g_bar = (1 / chi) * (k / (k + 1)) * D * (1 / dx^2)
 
-        where ``g_bar`` is the cell-to-cell conductance, but normalised with
+        where ``g_bar`` is the cell-to-cell conductance, but normalized with
         respect to unit membrane area.
-        For models with currents normalised to area this is unproblematic, but
-        to convert to models with unnormalised currents this means we have
+        For models with currents normalized to area this is unproblematic, but
+        to convert to models with unnormalized currents this means we have
         added the further assumption that **each node contains some fixed
         amount of membrane**, determined by an area A::
 
             g = (1 / chi) * (k / (k + 1)) * D * (1 / dx^2) * A
 
         This equation can also be applied in two dimensions, but only if
         **we assume that the conductivity matrix is diagonal**, in which case::
@@ -821,17 +821,17 @@
 
         [4] Computer Model of Excitation and Recovery in the Anisotropic
         Myocardium I. Rectangular and Cubic Arrays of Excitable Elements.
         Leon & Horacek (1991) Journal of electrocardiology
         """
         return D * A * k / ((k + 1) * chi * dx * dx)
 
-    def neighbours(self, x, y=None):
+    def neighbors(self, x, y=None):
         """
-        Returns a list of indices specifying the neighbours of the cell at
+        Returns a list of indices specifying the neighbors of the cell at
         index ``x`` (or index ``(x, y)`` for 2d simulations).
 
         Indices are given either as integers (1d or arbitrary geometry) or as
         tuples (2d).
 
         If diffusion is disabled, a call to this method will raise a
         ``RuntimeError``.
@@ -853,37 +853,46 @@
                 raise IndexError('Y-coordinate out of range: ' + str(y) + '.')
         elif not (y is None or y == 0):
             raise ValueError(
                 'Y-coordinate specified for 1-dimensional simulation.')
 
         # User-specified connections (always 1d)
         if self._connections is not None:
-            neighbours = []
+            neighbors = []
             for i, j, c in self._connections:
                 if i == x:
-                    neighbours.append(j)
+                    neighbors.append(j)
                 elif j == x:
-                    neighbours.append(i)
-            return neighbours
+                    neighbors.append(i)
+            return neighbors
 
-        # Left and right neighbours
-        neighbours = []
+        # Left and right neighbors
+        neighbors = []
         if x > 0:
-            neighbours.append(x - 1)
+            neighbors.append(x - 1)
         if x + 1 < self._dims[0]:
-            neighbours.append(x + 1)
+            neighbors.append(x + 1)
 
-        # Top and bottom neighbours
+        # Top and bottom neighbors
         if len(self._dims) == 2:
-            neighbours = [(i, y) for i in neighbours]
+            neighbors = [(i, y) for i in neighbors]
             if y > 0:
-                neighbours.append((x, y - 1))
+                neighbors.append((x, y - 1))
             if y + 1 < self._dims[1]:
-                neighbours.append((x, y + 1))
-        return neighbours
+                neighbors.append((x, y + 1))
+        return neighbors
+
+    def neighbours(self, x, y=None):
+        """ Alias of :meth:`neighbors`. """
+        # Deprecated since 2023-06-07
+        import warnings
+        warnings.warn('The method SimulationOpenCL.neighbours() is deprecated.'
+                      ' Please use neighbors() instead.')
+
+        return self.neighbors(x, y)
 
     def pre(self, duration, report_nan=True, progress=None,
             msg='Pre-pacing SimulationOpenCL'):
         """
         This method can be used to perform an unlogged simulation, typically to
         pre-pace to a (semi-)stable orbit.
 
@@ -1161,22 +1170,22 @@
                 vpace = self._model.binding('pace')
                 vpace = None if vpace is None else vpace.qname()
                 vdiff = None
                 if self._diffusion_enabled:
                     vdiff = self._model.binding('diffusion_current')
                     vdiff = None if vdiff is None else vdiff.qname()
 
-                # List all neighbours for this cell
-                neighbours = self.neighbours(*icell)
+                # List all neighbors for this cell
+                neighbors = self.neighbors(*icell)
                 if len(self._dims) == 2:
-                    neighbours_str = ', '.join(
+                    neighbors_str = ', '.join(
                         ('(' + ','.join([str(i) for i in j]) + ')')
-                        for j in neighbours)
+                        for j in neighbors)
                 else:
-                    neighbours_str = ', '.join(str(j) for j in neighbours)
+                    neighbors_str = ', '.join(str(j) for j in neighbors)
 
                 # Show final state
                 txt.append('State during:')
                 txt.append(self._model.format_state(
                     states[0], precision=self._precision))
 
                 # Show bound variables
@@ -1188,16 +1197,16 @@
                         '  Pacing variable: ' + myokit.float.str(
                             bounds[0][vpace], precision=self._precision)
                         + is_paced_str)
                 if vdiff is not None:
                     txt.append(
                         '  Diffusion current: ' + myokit.float.str(
                             bounds[0][vdiff], precision=self._precision))
-                if neighbours:
-                    txt.append('  Connected cells: ' + neighbours_str)
+                if neighbors:
+                    txt.append('  Connected cells: ' + neighbors_str)
 
                 # Show previous state (and derivatives)
                 n_states = len(states)
                 txt.append('Obtained ' + str(n_states) + ' previous state(s).')
                 if n_states > 1:
                     # Get state and input at previous state
                     state = states[1]
@@ -1235,16 +1244,16 @@
                             '  Pacing variable: ' + myokit.float.str(
                                 bounds[1][vpace], precision=self._precision)
                             + is_paced_str)
                     if vdiff is not None:
                         txt.append(
                             '  Diffusion current: ' + myokit.float.str(
                                 bounds[1][vdiff], precision=self._precision))
-                    if neighbours:
-                        txt.append('  Connected cells: ' + neighbours_str)
+                    if neighbors:
+                        txt.append('  Connected cells: ' + neighbors_str)
 
                     # Show all variables with non-finite values
                     txt.append(
                         'Logged all variables for points: ' + ', '.join(
                             myokit.float.str(t, precision=self._precision)
                             for t in d.time()))
                     txt.append(
```

### Comparing `myokit-1.33.9/myokit/_sim/pacing.h` & `myokit-1.34.0/myokit/_sim/pacing.h`

 * *Files 5% similar despite different names*

```diff
@@ -364,15 +364,15 @@
         n = PyList_Size(list);
 
         // Translate python pacing events
         // Note: A lot of the tests here shouldn't really make a difference,
         // since they are tested by the Python code already!
         if(n > 0) {
             PyObject *item, *attr;
-            events = (ESys_Event)malloc((size_t)n*sizeof(struct ESys_Event_mem));
+            events = (ESys_Event)malloc((size_t)n * sizeof(struct ESys_Event_mem));
             e = events;
             for(i=0; i<n; i++) {
                 item = PyList_GetItem(list, i); // Don't decref!
                 // Level
                 attr = PyObject_GetAttrString(item, "_level");
                 if (attr == NULL) { // Not a string
                     free(events); Py_DECREF(list);
@@ -616,14 +616,15 @@
 #define FSys_POPULATE_INVALID_TIMES         -20
 #define FSys_POPULATE_INVALID_VALUES        -21
 #define FSys_POPULATE_SIZE_MISMATCH         -22
 #define FSys_POPULATE_NOT_ENOUGH_DATA       -23
 #define FSys_POPULATE_INVALID_TIMES_DATA    -24
 #define FSys_POPULATE_INVALID_VALUES_DATA   -25
 #define FSys_POPULATE_DECREASING_TIMES_DATA -26
+#define FSys_POPULATE_INVALID_PROTOCOL      -27
 
 /*
  * Sets a python exception based on a fixed-form pacing error flag.
  *
  * Arguments
  *  flag : The python error flag to base the message on.
  */
@@ -643,14 +644,17 @@
     case FSys_POPULATED_SYSTEM:
         PyErr_SetString(PyExc_Exception, "F-Pacing error: Pacing system already populated.");
         break;
     case FSys_UNPOPULATED_SYSTEM:
         PyErr_SetString(PyExc_Exception, "F-Pacing error: Pacing system not populated.");
         break;
     // Populate
+    case FSys_POPULATE_INVALID_PROTOCOL:
+        PyErr_SetString(PyExc_Exception, "F-Pacing error: Invalid protocol python object passed.");
+        break;
     case FSys_POPULATE_INVALID_TIMES:
         PyErr_SetString(PyExc_Exception, "F-Pacing error: Invalid times array passed.");
         break;
     case FSys_POPULATE_INVALID_VALUES:
         PyErr_SetString(PyExc_Exception, "F-Pacing error: Invalid values array passed.");
         break;
     case FSys_POPULATE_SIZE_MISMATCH:
@@ -746,53 +750,73 @@
  *  sys    : The fixed-form pacing system to add the data to.
  *  times  : A Python list of (non-decreasing) floats.
  *  values : An equally sized Python list of floats.
  *
  * Returns a fixed-form pacing error flag.
  */
 FSys_Flag
-FSys_Populate(FSys sys, PyObject* times_list, PyObject* values_list)
+FSys_Populate(FSys sys, PyObject* protocol)
 {
     int i;
     Py_ssize_t n;
+    PyObject *times_list, *values_list;
 
     // Check ESys
     if(sys == 0) return FSys_INVALID_SYSTEM;
     if (sys->n_points != -1) return FSys_POPULATED_SYSTEM;
+    if (protocol == Py_None) return FSys_POPULATE_INVALID_PROTOCOL;
 
-    // Check input lists
-    if(!PyList_Check(times_list)) return FSys_POPULATE_INVALID_TIMES;
-    if(!PyList_Check(values_list)) return FSys_POPULATE_INVALID_VALUES;
-    n = PyList_Size(times_list);
-    if (n != PyList_Size(values_list)) return FSys_POPULATE_SIZE_MISMATCH;
-    if (n < 2) return FSys_POPULATE_NOT_ENOUGH_DATA;
+    // Get PyList from protocol (will need to decref!)
+    // Cast to (char*) happens because CallMethod accepts a mutable char*
+    // This should have been const char* and has been fixed in python 3
+    times_list = PyObject_CallMethod(protocol, (char*)"times", NULL); // Returns a new reference
+    if(times_list == NULL) return FSys_POPULATE_INVALID_PROTOCOL;
+    if(!PyList_Check(times_list)) {
+        Py_DECREF(times_list);
+        return FSys_POPULATE_INVALID_TIMES;
+    }
 
-    // Convert and check times list
-    sys->times = (double*)malloc((size_t)n*sizeof(double));
+    // Check and convert times list
+    n = PyList_Size(times_list);
+    sys->times = (double*)malloc((size_t)n * sizeof(double));
     for(i=0; i<n; i++) {
         // GetItem and convert --> Borrowed reference so ok not to decref!
         sys->times[i] = PyFloat_AsDouble(PyList_GetItem(times_list, i));
     }
+    Py_DECREF(times_list);  // Finished with the times_list
+
     if (PyErr_Occurred()) {
         free(sys->times); sys->times = NULL;
         return FSys_POPULATE_INVALID_TIMES_DATA;
     }
     for(i=1; i<n; i++) {
         if(sys->times[i] < sys->times[i-1]) {
             free(sys->times); sys->times = NULL;
             return FSys_POPULATE_DECREASING_TIMES_DATA;
         }
     }
 
-    // Convert values list
-    sys->values = (double*)malloc((size_t)n*sizeof(double));
+    // Check and convert values list
+    values_list = PyObject_CallMethod(protocol, (char*)"values", NULL); // Returns a new reference
+    if(values_list == NULL) {
+        free(sys->times); sys->times = NULL;
+        return FSys_POPULATE_INVALID_PROTOCOL;
+    }
+    if(!PyList_Check(values_list) || PyList_Size(values_list) != n) {
+        free(sys->times); sys->times = NULL;
+        Py_DECREF(values_list);
+        return FSys_POPULATE_INVALID_VALUES;
+    }
+    sys->values = (double*)malloc((size_t)n * sizeof(double));
     for(i=0; i<n; i++) {
         // GetItem and convert --> Borrowed reference so ok not to decref!
         sys->values[i] = PyFloat_AsDouble(PyList_GetItem(values_list, i));
     }
+    Py_DECREF(values_list); // Finished with the values list
+
     if (PyErr_Occurred()) {
         free(sys->times); sys->times = NULL;
         free(sys->values); sys->values = NULL;
         return FSys_POPULATE_INVALID_VALUES_DATA;
     }
 
     // Update pacing system and return
@@ -828,15 +852,15 @@
     }
     if(sys->n_points < 0) {
         if(flag != 0) *flag = FSys_UNPOPULATED_SYSTEM;
         return -1;
     }
 
     // Find the highest index `i` of sorted array `times` such that
-    // `times[i] <= time`, or `-1` if no such indice can be found.
+    // `times[i] <= time`, or `-1` if no such index can be found.
     // A guess can be given, which will be used to speed things up
 
     // Get left point, check value
     ileft = 0;
     tleft = sys->times[ileft];
     if (tleft > time) {
         // Out-of-bounds on the left, return left-most value
```

### Comparing `myokit-1.33.9/myokit/_sim/rhs.c` & `myokit-1.34.0/myokit/_sim/rhs.c`

 * *Files 1% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 w.set_lhs_function(v)
 
 # Tab
 tab = '    '
 
 # Process bindings, remove unsupported bindings, get map of bound variables to
 # internal names
-bound_variables = model.prepare_bindings({
+bound_variables = myokit._prepare_bindings(model, {
     'time' : 'engine_time',
-    })
+})
 
 # Get equations
 equations = model.solvable_order()
 ?>
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 #include <stdio.h>
@@ -246,15 +246,15 @@
     // Test given times
     n_positions = stop - start;
     if (n_positions < 1) {
         PyErr_SetString(PyExc_Exception, "Invalid log position selection: At least 1 position in the logs must be checked.");
         return 0;
     }
     if (start < 0) {
-        PyErr_SetString(PyExc_Exception, "Invalid log position selection: Negative list indice given.");
+        PyErr_SetString(PyExc_Exception, "Invalid log position selection: Negative list index given.");
         return 0;
     }
 
     //
     // ALLOCATING MEMORY, FROM THIS POINT ON, USE GOTO ERROR INSTEAD OF RETURN 0
     //
     // Create list for logged results
```

### Comparing `myokit-1.33.9/myokit/_sim/rhs.py` & `myokit-1.34.0/myokit/_sim/rhs.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     To enable partial benchmarking the argument ``variables`` can be used to
     pass in a list of variables whose combined evaluation time can be obtained
     by using :meth:`bench_part()`. Only non-constant, non-bound variables can
     be selected.
 
     By default, the given list of variables are the only variables included in
-    a partial simulation. This behaviour can be inverted by setting
+    a partial simulation. This behavior can be inverted by setting
     ``exclude_selected=True``. With this setting, all variables except those in
     the given list will be tested.
 
     A valid myokit model should be provided as the ``model`` argument.
     """
     _index = 0  # Unique id for the generated module
```

### Comparing `myokit-1.33.9/myokit/_sim/sundials.c` & `myokit-1.34.0/myokit/_sim/sundials.c`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_sim/sundials.py` & `myokit-1.34.0/myokit/_sim/sundials.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_system.py` & `myokit-1.34.0/myokit/_system.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/_unit.py` & `myokit-1.34.0/myokit/_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,15 +512,15 @@
             quantifiable unit. Typically this should only be done for the
             unquantified symbol notation of SI or SI derived units. For example
             m, g, Hz, N but not meter, kg, hertz or forthnight.
         ``output``
             ``True`` if this units name should be used to display this unit in.
             This should be set for all common units (m, kg, nm, Hz) but not for
             more obscure units (furlong, parsec). Having ``output`` set to
-            ``False`` will cause one-way behaviour: Myokit will recognise the
+            ``False`` will cause one-way behavior: Myokit will recognise the
             unit name but never use it in output.
             Setting this to ``True`` will also register the given name as a
             preferred representation format.
 
         """
         if not isinstance(name, basestring):
             raise TypeError('Given name must be a string.')
```

### Comparing `myokit-1.33.9/myokit/float.py` & `myokit-1.34.0/myokit/float.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/__init__.py` & `myokit-1.34.0/myokit/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/ansic/__init__.py` & `myokit-1.34.0/myokit/formats/ansic/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/ansic/_ewriter.py` & `myokit-1.34.0/myokit/formats/ansic/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/ansic/_exporter.py` & `myokit-1.34.0/myokit/formats/ansic/_exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     Provides the following external variables:
 
     ``time``
         The simulation time
     ``pace``
         The value of the pacing variable, implemented using the given protocol.
     ``diffusion_current``
-        The current flowing from each cell to its neighbours. This will be
+        The current flowing from each cell to its neighbors. This will be
         positive if the cell is acting as a source, negative when it's acting
         as a sink.
 
     Requires the following labels to be set in the model:
 
     ``membrane_potential``
         The membrane potential.
```

### Comparing `myokit-1.33.9/myokit/formats/ansic/template/cable.c` & `myokit-1.34.0/myokit/formats/ansic/template/cable.c`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 model.reserve_unique_names(*ansic.keywords)
 model.create_unique_names()
 
 # Get expression writer
 w = ansic.AnsiCExpressionWriter()
 
 # Process bindings, remove unsupported bindings
-bound_variables = model.prepare_bindings({
+bound_variables = myokit._prepare_bindings(model, {
     'time'         : 't',
     'pace'         : 'pace',
     'diffusion_current' : 'current'
-    }).keys()
+}).keys()
 
 if model.binding('diffusion_current') is None:
     raise Exception('This exporter requires a variable to be bound to'
         ' "diffusion_current".')
 
 # Define var/lhs function
 def v(var, pre='cell->'):
@@ -151,16 +151,16 @@
 /*
  * Sets initial state values
  */
 static void
 Cell_set_initial_state(Cell *cell)
 {
 <?
-for eq in model.inits():
-    print(tab + w.eq(eq) + ';')
+for var, init in zip(model.states(), model.initial_values(True)):
+    print(tab + v(var) + ' = ' + myokit.float.str(init) + ';')
 ?>}
 
 /*
  * Calculates derivatives in a cell
  */
 static void
 Cell_calculate_derivatives(Cell *cell)
```

### Comparing `myokit-1.33.9/myokit/formats/ansic/template/euler.c` & `myokit-1.34.0/myokit/formats/ansic/template/euler.c`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 
 # Reserve keywords
 model.reserve_unique_names(*ansic.keywords)
 model.create_unique_names()
 
 # Process bindings, remove unsupported bindings, get map of bound variables to
 # internal names
-bound_variables = model.prepare_bindings({
+bound_variables = myokit._prepare_bindings(model, {
     'time' : 'time',
     'pace' : 'pace',
-    })
+})
 
 # Get equations
 equations = model.solvable_order()
 
 # Get component order
 comp_order = list(equations.keys())
 comp_order = comp_order[:-1] # Strip *remaining*, guaranteed empty
@@ -91,15 +91,15 @@
         # Explicitly asked for derivative
         return pre + 'D_' + var.var().uname()
     if isinstance(var, myokit.Name):
         var = var.var()
     if var in bound_variables:
         return bound_variables[var]
     if var.is_state():
-        return pre + 'state[' + str(var.indice()) + ']'
+        return pre + 'state[' + str(var.index()) + ']'
     elif var.is_constant():
         return pre + 'C_' + var.uname()
     else:
         return pre + 'I_' + var.uname()
 w.set_lhs_function(v)
 
 # Tab
@@ -122,15 +122,15 @@
 #define STIM_OFFSET   <?= stim_offset ?>
 #define STIM_PERIOD   <?= stim_period ?>
 
 /* Define aliases of state variables */
 #define N_STATE <?= model.count_states() ?>
 <?
 for var in model.states():
-    print('#define S_' + var.uname() + ' state[' + str(var.indice()) + ']')
+    print('#define S_' + var.uname() + ' state[' + str(var.index()) + ']')
 ?>
 
 /* Define constants, calculated constants */
 <?
 for group in equations.values():
     for eq in group.equations(const=True):
         if isinstance(eq.rhs, myokit.Number):
@@ -216,15 +216,15 @@
 
 /* Run a simulation */
 int main()
 {
     Real state[N_STATE];
 <?
 for var in model.states():
-    print(tab + v(var) + ' = ' + myokit.float.str(var.state_value()) + ';')
+    print(tab + v(var) + ' = ' + myokit.float.str(var.initial_value(True)) + ';')
 
 ?>
 
     long steps = 0;
     Real dt = 0.01;
     Real time = 0;
     while (time < 1000.0) {
```

### Comparing `myokit-1.33.9/myokit/formats/ansic/template/sim.c` & `myokit-1.34.0/myokit/formats/ansic/template/sim.c`

 * *Files 1% similar despite different names*

```diff
@@ -18,34 +18,34 @@
 # Get model
 model.reserve_unique_names(*ansic.keywords)
 model.create_unique_names()
 
 # Define lhs function
 def v(var):
     if isinstance(var, myokit.Derivative):
-        return 'NV_Ith_S(ydot, ' + str(var.var().indice()) + ')'
+        return 'NV_Ith_S(ydot, ' + str(var.var().index()) + ')'
     elif isinstance(var, myokit.Name):
         var = var.var()
     if var.is_state():
-        return 'NV_Ith_S(y, ' + str(var.indice()) + ')'
+        return 'NV_Ith_S(y, ' + str(var.index()) + ')'
     elif var.is_constant():
         return 'AC_' + var.uname()
     else:
         return 'AV_' + var.uname()
 
 # Create expression writer
 w = ansic.AnsiCExpressionWriter()
 w.set_lhs_function(v)
 
 # Process bindings, remove unsupported bindings, get map of bound variables to
 # internal names
-bound_variables = model.prepare_bindings({
+bound_variables = myokit._prepare_bindings(model, {
     'time' : 't',
     'pace' : 'pace',
-    })
+})
 
 # Tab
 tab = '    '
 
 # Get equations
 equations = model.solvable_order()
 
@@ -127,16 +127,16 @@
 }
 
 /* Set initial values */
 static void
 default_initial_values(N_Vector y)
 {
 <?
-for eq in model.inits():
-    print(tab + w.eq(eq) + ';')
+for var, init in zip(model.states(), model.initial_values(True)):
+    print(tab + v(var) + ' = ' + myokit.float.str(init) + ';')
 ?>
 }
 
 /* Pacing event (non-zero stimulus) */
 struct PacingEventS {
     double level;       /* The stimulus level (dimensionless, normal range [0,1]) */
     double start;       /* The time this stimulus starts */
```

### Comparing `myokit-1.33.9/myokit/formats/axon/__init__.py` & `myokit-1.34.0/myokit/formats/axon/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/axon/_abf.py` & `myokit-1.34.0/myokit/formats/axon/_abf.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,14 @@
         try:
             self._protocol = self._read_protocol()
         except Exception:   # pragma: no cover
             # This is not something we _want_ to happen, so if we have test
             # cases that trigger this error they should be resolved. At the
             # same time, if it happens to a user we want it to "sort-of work"
             # (an experimental rather than a production setting)
-            logging.basicConfig()
             log = logging.getLogger(__name__)
             log.warning('Unable to read protocol from ' + self._filepath)
             log.warning(traceback.format_exc())
             self._protocol = []
 
         # The measured data as a list of sweeps
         if self._is_protocol_file:
@@ -1061,15 +1060,14 @@
                         if i_last > nSam:
                             # The protocol may extend beyond the number of
                             # samples in the recording
                             break
 
                     else:  # pragma: no cover
 
-                        logging.basicConfig()
                         log = logging.getLogger(__name__)
                         log.warning(
                             'Unsupported epoch type: ' + epoch_types(kind))
                         continue
 
             sweeps.append(sweep)
             start += self._sweepStartToStart
```

### Comparing `myokit-1.33.9/myokit/formats/axon/_atf.py` & `myokit-1.34.0/myokit/formats/axon/_atf.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/axon/_importer.py` & `myokit-1.34.0/myokit/formats/axon/_importer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/cellml/__init__.py` & `myokit-1.34.0/myokit/formats/cellml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/cellml/_ewriter.py` & `myokit-1.34.0/myokit/formats/cellml/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/cellml/_exporter.py` & `myokit-1.34.0/myokit/formats/cellml/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/cellml/_importer.py` & `myokit-1.34.0/myokit/formats/cellml/_importer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/cellml/v1/__init__.py` & `myokit-1.34.0/myokit/formats/cellml/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/cellml/v1/_api.py` & `myokit-1.34.0/myokit/formats/cellml/v1/_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -894,15 +894,15 @@
                 # Free variable shouldn't have a value
                 if variable is time:
                     m.set_free_variable(v)
 
                 # Promote states and set rhs and initial value
                 elif variable.is_state():
                     v.set_is_state(True)
-                    v.set_initial_value(variable.state_value())
+                    v.set_initial_value(variable.initial_value(True))
                     v.set_rhs(rhs)
 
                 # Store literals (single number) in initial value
                 elif isinstance(rhs, myokit.Number):
                     v.set_initial_value(rhs.eval())
 
                 # For all other use rhs
```

### Comparing `myokit-1.33.9/myokit/formats/cellml/v1/_parser.py` & `myokit-1.34.0/myokit/formats/cellml/v1/_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/cellml/v1/_writer.py` & `myokit-1.34.0/myokit/formats/cellml/v1/_writer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/cellml/v2/__init__.py` & `myokit-1.34.0/myokit/formats/cellml/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/cellml/v2/_api.py` & `myokit-1.34.0/myokit/formats/cellml/v2/_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -798,15 +798,15 @@
 
                 # Free variable shouldn't have a value
                 if variable is time:
                     m.set_variable_of_integration(v)
 
                 # Promote states and set rhs and initial value
                 elif variable.is_state():
-                    v.set_initial_value(variable.state_value())
+                    v.set_initial_value(variable.initial_value(True))
                     v.set_equation(myokit.Equation(lhs, rhs))
 
                 # Store literals (single number) in initial value
                 elif isinstance(rhs, myokit.Number):
                     v.set_initial_value(rhs.eval())
 
                 # For all other use rhs
```

### Comparing `myokit-1.33.9/myokit/formats/cellml/v2/_parser.py` & `myokit-1.34.0/myokit/formats/cellml/v2/_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/channelml/__init__.py` & `myokit-1.34.0/myokit/formats/channelml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/channelml/_importer.py` & `myokit-1.34.0/myokit/formats/channelml/_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         except IndexError:
             raise ChannelMLError(
                 'No <channel_type> element found inside <channelml> element.'
                 ' Import of <synapse_type> and <ion_concentration> is not'
                 ' supported.')
 
         # Add channel component
-        name = self._sanitise_name(root.getAttribute('name'))
+        name = self._sanitize_name(root.getAttribute('name'))
         if name in model:
             name_root = name
             i = 2
             while name in model:
                 name = name_root + '_' + str(i)
                 i += 1
         component = model.add_component(name)
@@ -196,15 +196,15 @@
         gmaxvar = component.add_variable('gmax')
         gmaxvar.set_rhs(gmax)
         gmaxvar.meta['desc'] = 'Maximum conductance'
 
         # Add gates
         gvars = []
         for gate in cvr.getElementsByTagName('gate'):
-            gname = self._sanitise_name(gate.getAttribute('name'))
+            gname = self._sanitize_name(gate.getAttribute('name'))
             gvar = component.add_variable(gname)
             gvar.promote(0)
             cstate = gate.getElementsByTagName('closed_state')
             cstate = cstate[0].getAttribute('id')
             ostate = gate.getElementsByTagName('open_state')
             ostate = ostate[0].getAttribute('id')
 
@@ -238,28 +238,28 @@
                         break
                 if toc is None:
                     raise ChannelMLError(
                         'Unable to find open-to-closed transition for gate <'
                         + gname + '>')
 
                 # Add closed-to-open transition
-                tname = self._sanitise_name(tco.getAttribute('name'))
+                tname = self._sanitize_name(tco.getAttribute('name'))
                 tcovar = gvar.add_variable(tname)
                 expr = str(tco.getAttribute('expr'))
                 try:
                     tcovar.set_rhs(self._parse_expression(expr, tcovar))
                 except myokit.ParseError as e:
                     warnings.warn(
                         'Error parsing expression for closed-to-open'
                         ' transition in gate <' + gname + '>: '
                         + myokit.format_parse_error(e))
                     tcovar.meta['expression'] = str(expr)
 
                 # Add open-to-closed transition
-                tname = self._sanitise_name(toc.getAttribute('name'))
+                tname = self._sanitize_name(toc.getAttribute('name'))
                 tocvar = gvar.add_variable(tname)
                 expr = str(toc.getAttribute('expr'))
                 try:
                     tocvar.set_rhs(self._parse_expression(expr, tocvar))
                 except myokit.ParseError as e:
                     warnings.warn(
                         'Error parsing expression for open-to-closed'
@@ -280,27 +280,27 @@
                     raise ChannelMLError(
                         'Unable to find transitions or steady state and'
                         ' time course for gate <' + gname + '>.')
                 ss = ss[0]
                 tc = tc[0]
 
                 # Add steady-state variable
-                ssname = self._sanitise_name(ss.getAttribute('name'))
+                ssname = self._sanitize_name(ss.getAttribute('name'))
                 ssvar = gvar.add_variable(ssname)
                 expr = str(ss.getAttribute('expr'))
                 try:
                     ssvar.set_rhs(self._parse_expression(expr, ssvar))
                 except myokit.ParseError as e:
                     warnings.warn(
                         'Error parsing expression for steady state in gate <'
                         + gname + '>: ' + myokit.format_parse_error(e))
                     ssvar.meta['expression'] = str(expr)
 
                 # Add time course variable
-                tcname = self._sanitise_name(tc.getAttribute('name'))
+                tcname = self._sanitize_name(tc.getAttribute('name'))
                 tcvar = gvar.add_variable(tcname)
                 expr = str(tc.getAttribute('expr'))
                 try:
                     tcvar.set_rhs(self._parse_expression(expr, tcvar))
                 except myokit.ParseError as e:
                     warnings.warn(
                         'Error parsing expression for time course in gate <'
@@ -408,15 +408,15 @@
             else:
                 for kid in node.childNodes:
                     text(kid, buff)
             return buff
         return textwrap.fill(
             str('\n'.join(text(node))), 70, replace_whitespace=False)
 
-    def _sanitise_name(self, name):
+    def _sanitize_name(self, name):
         """
         Tests if a name is a valid myokit name. Adapts it if it isn't.
         """
         name = str(name).strip()
         name = name.replace('.', '_')
         name = name.replace(' ', '_')
         name = name.replace('-', '_')
```

### Comparing `myokit-1.33.9/myokit/formats/cpp/__init__.py` & `myokit-1.34.0/myokit/formats/cpp/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/cpp/_ewriter.py` & `myokit-1.34.0/myokit/formats/cpp/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/cuda/__init__.py` & `myokit-1.34.0/myokit/formats/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/cuda/_ewriter.py` & `myokit-1.34.0/myokit/formats/cuda/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/cuda/_exporter.py` & `myokit-1.34.0/myokit/formats/cuda/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/cuda/template/kernel.cu` & `myokit-1.34.0/myokit/formats/cuda/template/kernel.cu`

 * *Files 6% similar despite different names*

```diff
@@ -62,21 +62,24 @@
     'I_diff',
     'dt',
     'parameters',
     'state',
     )
 model.create_unique_names()
 
+# Get initial values (before time binding is removed and model becomes invalid)
+initial_values = model.initial_values(True)
+
 # Process bindings, remove unsupported bindings, get map of bound variables to
 # internal names
-bound_variables = model.prepare_bindings({
+bound_variables = myokit._prepare_bindings(model, {
     #'time' : 'time',
     #'pace' : 'pace',
     'diffusion_current' : 'I_diff',
-    })
+})
 
 # Get equations
 equations = model.solvable_order()
 
 # Delete "*remaning*" group, guaranteed to be empty with independent components
 del(equations['*remaining*'])
 
@@ -186,15 +189,15 @@
     for eq in group.equations(const=True):
         if not isinstance(eq.rhs, myokit.Number):
             print('#define ' + v(eq.lhs) + ' (' + w.ex(eq.rhs) + ')')
 
 print('')
 print('/* Aliases of state variables. */')
 for var in model.states():
-    print('#define ' + var.uname() + ' state[' + str(var.indice()) + ']')
+    print('#define ' + var.uname() + ' state[' + str(var.index()) + ']')
 
 ?>
 
 ////////////////////////////////////////////////////////////////////////////////
 // Local function declarations
 ////////////////////////////////////////////////////////////////////////////////
 
@@ -291,18 +294,18 @@
 
 /* Set the standard initial conditions */
 int get_default_initial_state(Real *state)
 {
     if (state == 0) return(-1);
 
 <?
-for var in model.states():
+for var, val in zip(model.states(), initial_values):
     if 'desc' in var.meta:
         print(tab + '// ' + var.meta['desc'])
-    print(tab + v(var) + ' = ' + myokit.float.str(var.state_value()) + ';')
+    print(tab + v(var) + ' = ' + myokit.float.str(val) + ';')
 ?>
 
     return(0);
 }
 
 /* Function to initialize the parameter array in the model structure. */
 int get_default_parameters(Real *parameters)
```

### Comparing `myokit-1.33.9/myokit/formats/easyml/__init__.py` & `myokit-1.34.0/myokit/formats/easyml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/easyml/_ewriter.py` & `myokit-1.34.0/myokit/formats/easyml/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/easyml/_exporter.py` & `myokit-1.34.0/myokit/formats/easyml/_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,16 +368,16 @@
             f.write(lhs(vm) + '; .nodal(); .external(Vm);' + eol)
 
             # Write current
             f.write('Iion; .nodal(); .external();' + eol + eol)
 
             # Write initial conditions
             for v in model.states():
-                f.write(lhs(v) + '_init = ' + myokit.float.str(v.state_value())
-                        + eos)
+                f.write(lhs(v) + '_init = '
+                        + myokit.float.str(v.initial_value(True)) + eos)
             f.write(eol)
 
             # Write remaining variables
             for c in model.components(sort=True):
                 todo = c.variables(deep=True, sort=True)
                 todo = [v for v in todo if v not in ignore]
                 if todo:
```

### Comparing `myokit-1.33.9/myokit/formats/html/__init__.py` & `myokit-1.34.0/myokit/formats/html/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/html/_exporter.py` & `myokit-1.34.0/myokit/formats/html/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/html/_flatten.py` & `myokit-1.34.0/myokit/formats/html/_flatten.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/latex/__init__.py` & `myokit-1.34.0/myokit/formats/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/latex/_ewriter.py` & `myokit-1.34.0/myokit/formats/latex/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/latex/_exporter.py` & `myokit-1.34.0/myokit/formats/latex/_exporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
             # Initial conditions
             f.write('\\section{Initial conditions}\n')
             for v in model.states():
                 f.write('\\begin{dmath}\n')
                 f.write(e.ex(myokit.Name(v)))
                 f.write(' = ')
-                f.write(e.ex(myokit.Number(v.state_value())))
+                f.write(e.ex(v.initial_value()))
                 f.write('\\end{dmath}\n')
 
             # Write each component
             for c in model.components():
                 f.write('\\section{' + self._clean(c.name()) + '}\n')
                 try:
                     text = c.meta['desc']
```

### Comparing `myokit-1.33.9/myokit/formats/mathml/__init__.py` & `myokit-1.34.0/myokit/formats/mathml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/mathml/_ewriter.py` & `myokit-1.34.0/myokit/formats/mathml/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/mathml/_parser.py` & `myokit-1.34.0/myokit/formats/mathml/_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         :class:`myokit.Number` objects. Note that ``element`` can be ``None``
         for numbers that have no corresponding ``<cn>`` element.
     ``free_variables``
         All :class:`Name` objects for free variables in derivative expressions
         will be added to this set.
 
     This is not a validating parser: if the MathML is invalid the method's
-    behaviour is undefined.
+    behavior is undefined.
 
     The following MathML elements are recognised:
 
     Literals and references
 
     ``<ci>``
         Is converted to a :class:`myokit.Name` by passing the contents of the
```

### Comparing `myokit-1.33.9/myokit/formats/matlab/__init__.py` & `myokit-1.34.0/myokit/formats/matlab/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/matlab/_ewriter.py` & `myokit-1.34.0/myokit/formats/matlab/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/matlab/_exporter.py` & `myokit-1.34.0/myokit/formats/matlab/_exporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,29 +63,29 @@
             'stim_offset'
         )
         model.create_unique_names()
 
         # Variable naming function
         def v(var):
             if isinstance(var, myokit.Derivative):
-                return 'ydot(' + str(1 + var.var().indice()) + ')'
+                return 'ydot(' + str(1 + var.var().index()) + ')'
             if isinstance(var, myokit.Name):
                 var = var.var()
             if var.is_constant():
                 return 'c.' + var.uname()
             else:
                 return var.uname()
 
         # Expression writer
         ew = matlab.MatlabExpressionWriter()
         ew.set_lhs_function(v)
         ew.set_condition_function('ifthenelse')
 
         # Process bound variables
-        bound_variables = model.prepare_bindings({
+        bound_variables = myokit._prepare_bindings(model, {
             'time': 't',
             'pace': 'pace',
         })
 
         # Common variables
         equations = model.solvable_order()
         components = []
```

### Comparing `myokit-1.33.9/myokit/formats/matlab/template/constants.m` & `myokit-1.34.0/myokit/formats/matlab/template/constants.m`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/matlab/template/main.m` & `myokit-1.34.0/myokit/formats/matlab/template/main.m`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 <?
 #
 # main.m :: This will become the driver file
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
+import myokit
 ?>%
 % Driver file for <?= model.name() ?>
 %
 
 % Clear everything up and begin
 close all
 clear all
 
 % Initial values
 <?
-for eq in model.inits():
-    print(e(eq) + ';')
+for var, value in zip(model.states(), model.initial_values(True)):
+    print(v(var) + ' = ' + myokit.float.str(value) + ';')
 ?>
 
 % Vector for initial values
 y0 = [<?= ' '.join([v(var) for var in model.states()]) ?>]';
 
 % Constants
 c = constants();
```

### Comparing `myokit-1.33.9/myokit/formats/matlab/template/model.m` & `myokit-1.34.0/myokit/formats/matlab/template/model.m`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/opencl/__init__.py` & `myokit-1.34.0/myokit/formats/opencl/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/opencl/_ewriter.py` & `myokit-1.34.0/myokit/formats/opencl/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/opencl/_exporter.py` & `myokit-1.34.0/myokit/formats/opencl/_exporter.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     def _dict(self):
         return {
             'cable.c': 'cable.c',
             'kernel.cl': 'kernel.cl',
             'plot.py': 'plot.py',
             'minilog.py': 'minilog.py',
-            'test': 'test',
+            'test.sh': 'test.sh',
         }
 
     def _vars(self, model, protocol):
         from myokit.formats.opencl import keywords
 
         # Check if model has binding to diffusion_current
         if model.binding('diffusion_current') is None:
@@ -76,15 +76,15 @@
             model = model.clone()
 
         # Merge interdependent components
         model.resolve_interdependent_components()
 
         # Process bindings, remove unsupported bindings, get map of bound
         # variables to internal names.
-        bound_variables = model.prepare_bindings({
+        bound_variables = myokit._prepare_bindings(model, {
             'time': 'time',
             'pace': 'pace',
             'diffusion_current': 'idiff',
         })
 
         # Reserve keywords
         model.reserve_unique_names(*keywords)
```

### Comparing `myokit-1.33.9/myokit/formats/opencl/template/cable.c` & `myokit-1.34.0/myokit/formats/opencl/template/cable.c`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,15 @@
  */
 void set_initial_values(int n_cells, Real* s)
 {
     int i;
     for(i=0; i<n_cells; i++) {
 <?
 for v in model.states():
-    print(tab*2 + '*s = ' + myokit.float.str(v.state_value()) + '; s++; // ' + str(v.qname()))
+    print(tab*2 + '*s = ' + myokit.float.str(v.initial_value(True)) + '; s++; // ' + str(v.qname()))
 ?>
     }
 }
 
 /*
  * Runs a simulation
  *
@@ -230,22 +230,22 @@
     Real *state = NULL;
     Real *idiff = NULL;
 
     /* Get device id */
     cl_device_id device_id = get_device_id();
     char buffer[65536];
     ocl(clGetDeviceInfo(device_id, CL_DEVICE_NAME, sizeof(buffer), buffer, NULL));
-    printf("Using device: %s\n", buffer);
+    // printf("Using device: %s\n", buffer);
 
     /* Create a context and command queue */
     cl_int err;
     context = clCreateContext(NULL, 1, &device_id, NULL, NULL, &err);
     ocl_check("clCreateContext", err);
     command_queue = clCreateCommandQueue(context, device_id, 0, &err);
-    printf("Created context and command queue.\n");
+    // printf("Created context and command queue.\n");
 
     /* Create state vector */
     int dsize_state = n_cells * n_state * sizeof(Real);
     state = (Real*)malloc(dsize_state);
     set_initial_values(n_cells, state);
 
     /* Create diffusion current vector and copy to device */
@@ -254,20 +254,20 @@
     for(i=0; i<n_cells; i++) idiff[i] = 0.0;
 
     /* Create memory buffers on the device */
     mbuf_state = clCreateBuffer(context, CL_MEM_READ_WRITE, dsize_state, NULL, &err);
     ocl_check("clCreateBuffer mbuf_state", err);
     mbuf_idiff = clCreateBuffer(context, CL_MEM_READ_ONLY, dsize_idiff, NULL, &err);
     ocl_check("clCreateBuffer mbuf_idiff", err);
-    printf("Created buffers.\n");
+    // printf("Created buffers.\n");
 
     /* Copy data into buffers */
     ocl(clEnqueueWriteBuffer(command_queue, mbuf_state, CL_TRUE, 0, dsize_state, state, 0, NULL, NULL));
     ocl(clEnqueueWriteBuffer(command_queue, mbuf_idiff, CL_TRUE, 0, dsize_idiff, idiff, 0, NULL, NULL));
-    printf("Set initial state.\n");
+    // printf("Set initial state.\n");
 
     /* Load and compile the kernel program(s) */
     char* source = read_kernel("kernel.cl");
     program = clCreateProgramWithSource(context, 1, (const char**)&source, NULL, &err);
     ocl_check("clCreateProgramWithSource", err);
     err = clBuildProgram(program, 1, &device_id, NULL, NULL, NULL);
     if (err == CL_BUILD_PROGRAM_FAILURE) {
@@ -281,34 +281,34 @@
         clGetProgramBuildInfo(program, device_id, CL_PROGRAM_BUILD_LOG, blog_size, blog, NULL);
         fprintf(stderr, "%s\n", blog);
         fprintf(stderr, "----------------------------------------");
         fprintf(stderr, "---------------------------------------\n");
         abort();
     }
     ocl_check("clBuildProgram", err);
-    printf("Program created and built.\n");
+    // printf("Program created and built.\n");
 
     /* Create the kernels */
     kernel_cell = clCreateKernel(program, "cell_step", &err);
     ocl_check("clCreateKernel", err);
     kernel_diff = clCreateKernel(program, "diff_step", &err);
     ocl_check("clCreateKernel", err);
-    printf("Kernels created.\n");
+    // printf("Kernels created.\n");
 
     /* Pass arguments into kernels */
     ocl(clSetKernelArg(kernel_cell, 0, sizeof(n_cells), &n_cells));
     ocl(clSetKernelArg(kernel_diff, 1, sizeof(time), &time));
     ocl(clSetKernelArg(kernel_cell, 2, sizeof(dt), &dt));
     ocl(clSetKernelArg(kernel_cell, 3, sizeof(mbuf_state), &mbuf_state));
     ocl(clSetKernelArg(kernel_cell, 4, sizeof(mbuf_idiff), &mbuf_idiff));
     ocl(clSetKernelArg(kernel_diff, 0, sizeof(n_cells), &n_cells));
     ocl(clSetKernelArg(kernel_diff, 1, sizeof(g), &g));
     ocl(clSetKernelArg(kernel_diff, 2, sizeof(mbuf_state), &mbuf_state));
     ocl(clSetKernelArg(kernel_diff, 3, sizeof(mbuf_idiff), &mbuf_idiff));
-    printf("Arguments passed into kernels.\n");
+    // printf("Arguments passed into kernels.\n");
 
     /* Add log header */
     printf("engine.time");
     for(i=0; i<n_cells; i++) {
 <?
 for v in model.states():
     print(tab*2 + 'printf(",\\"%d.' + v.qname() + '\\"", i);')
@@ -338,29 +338,29 @@
 
         steps++;
         time = time_start + steps * dt;
     }
 
 done:
     /* Tidy up */
-    printf("Tidying up.\n");
+    // printf("Tidying up.\n");
 
     ocl(clFlush(command_queue));
     ocl(clFinish(command_queue));
     ocl(clReleaseMemObject(mbuf_state));
     ocl(clReleaseMemObject(mbuf_idiff));
     ocl(clReleaseKernel(kernel_cell));
     ocl(clReleaseKernel(kernel_diff));
     ocl(clReleaseProgram(program));
     ocl(clReleaseCommandQueue(command_queue));
     ocl(clReleaseContext(context));
     free(state);
     free(idiff);
 
-    printf("Done.\n");
+    // printf("Done.\n");
 }
 
 int main()
 {
     run(
         256,        // n_cells
         0,          // time_start
```

### Comparing `myokit-1.33.9/myokit/formats/opencl/template/kernel.cl` & `myokit-1.34.0/myokit/formats/opencl/template/kernel.cl`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     for eq in group.equations(const=True):
         if not isinstance(eq.rhs, myokit.Number):
             print('#define ' + v(eq.lhs) + ' (' + w.ex(eq.rhs) + ')')
 
 print('')
 print('/* Aliases of state variables. */')
 for var in model.states():
-    print('#define ' + var.uname() + ' state[offset + ' + str(var.indice()) + ']')
+    print('#define ' + var.uname() + ' state[offset + ' + str(var.index()) + ']')
 
 print('')
 for comp, ilist in comp_in.items():
     if comp == last_component:
         continue
     olist = comp_out[comp]
     if len(olist) == 0:
```

### Comparing `myokit-1.33.9/myokit/formats/opencl/template/minilog.py` & `myokit-1.34.0/myokit/formats/opencl/template/minilog.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             raise Exception(
                 'Syntax error on line ' + str(line) + ', character '
                 + str(1 + char) + ': ' + msg)
 
         # Delimiters
         quote = '"'
         delim = ','
-        with open(filename, 'rb') as f:
+        with open(filename, 'r', newline=None) as f:
             # Read header
             keys = []
             try:
                 line = f.readline()
             except EOFError:
                 e(0, 0, 'Empty file, expecting header.')
             # Trim end of line
```

### Comparing `myokit-1.33.9/myokit/formats/opencl/template/plot.py` & `myokit-1.34.0/myokit/formats/opencl/template/plot.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/python/__init__.py` & `myokit-1.34.0/myokit/formats/python/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/python/_ewriter.py` & `myokit-1.34.0/myokit/formats/python/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/python/_exporter.py` & `myokit-1.34.0/myokit/formats/python/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/python/template/sim.py` & `myokit-1.34.0/myokit/formats/python/template/sim.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 # Create python expression writer
 w = python.PythonExpressionWriter()
 w.set_lhs_function(v)
 e = w.eq
 
 # Process bindings
-bound_variables = model.prepare_bindings({
+bound_variables = myokit._prepare_bindings(model, {
     'time' : 'engine.time',
     'pace' : 'engine.pace',
     })
 
 # Get equations
 equations = model.solvable_order()
 components = []
@@ -92,17 +92,17 @@
     for eq in eqs.equations(const=True):
         print(tab2 + e(eq))
     ?>    def init(self):
         """
         Resets the state variables to their initial values
         """
 <?
-    for eq in model.inits():
-        if eq.lhs.var().parent() == comp:
-            print(tab2 + e(eq))
+    for var, value in zip(model.states(), model.initial_values(True)):
+        if var.parent() == comp:
+            print(tab2 + v(var, comp) + ' = ' + myokit.float.str(value))
     ?>    def update(self):
         """
         Re-calculates all values for the current time and state
         """
 <?
     printed = False
     for eq in eqs.equations(const=False):
```

### Comparing `myokit-1.33.9/myokit/formats/sbml/__init__.py` & `myokit-1.34.0/myokit/formats/sbml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/sbml/_api.py` & `myokit-1.34.0/myokit/formats/sbml/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,16 @@
 
     def set_initial_value(self, value):
         """
         Sets a :class:`myokit.Expression` for this quantity's initial value.
         """
         if not isinstance(value, myokit.Expression):
             raise SBMLError(
-                '<' + str(value) + '> needs to be an instance of '
-                'myokit.Expression.')
+                '<' + str(value) + '> needs to be an instance of'
+                ' myokit.Expression.')
 
         self._initial_value = value
 
     def set_value(self, value, is_rate=False):
         """
         Sets a :class:`myokit.Expression` for this quantity's value.
 
@@ -71,16 +71,16 @@
         ``rate``
             Set to ``True`` if the expression gives the rate of change of this
             variable.
 
         """
         if not isinstance(value, myokit.Expression):
             raise SBMLError(
-                '<' + str(value) + '> needs to be an instance of '
-                'myokit.Expression.')
+                '<' + str(value) + '> needs to be an instance of'
+                ' myokit.Expression.')
 
         self._value = value
         self._is_rate = bool(is_rate)
 
     def value(self):
         """
         Returns a :class:`myokit.Expression` for this quantity's value, or
@@ -122,16 +122,16 @@
 
     """
     def __init__(self, model, sid):
         super(Compartment, self).__init__()
 
         if not isinstance(model, Model):
             raise SBMLError(
-                '<' + str(model) + '> needs to be an instance of '
-                'myokit.formats.sbml.Model.')
+                '<' + str(model) + '> needs to be an instance of'
+                ' myokit.formats.sbml.Model.')
 
         self._model = model
         self._sid = str(sid)
 
         self._spatial_dimensions = None
         self._size_units = None
 
@@ -276,15 +276,15 @@
         """
         Adds a :class:`myokit.formats.sbml.Species` to this model (located in
         the given ``compartment``).
         """
         if not isinstance(compartment, Compartment):
             raise SBMLError(
                 '<' + compartment + '> needs to be instance of'
-                'myokit.formats.sbml.Compartment')
+                ' myokit.formats.sbml.Compartment')
 
         sid = str(sid) if sid else sid
         self._register_sid(sid)
         s = Species(compartment, sid, is_amount, is_constant, is_boundary)
         self._species[sid] = s
         self._assignables[sid] = s
 
@@ -423,15 +423,15 @@
         """
         Sets a :class:`Parameter` as global conversion factor for species,
         see :meth:`Species.conversion_factor()`.
         """
         if not isinstance(factor, Parameter):
             raise SBMLError(
                 '<' + str(factor) + '> needs to be instance of'
-                'myokit.formats.sbml.Parameter.')
+                ' myokit.formats.sbml.Parameter.')
 
         self._conversion_factor = factor
 
     def set_extent_units(self, units):
         """
         Sets the default units for "reaction extent", i.e. for the kinetic law
         equations in reactions.
@@ -581,16 +581,16 @@
 
     """
     def __init__(self, model, sid):
         super(Parameter, self).__init__()
 
         if not isinstance(model, Model):
             raise SBMLError(
-                '<' + str(model) + '> needs to be an instance of '
-                'myokit.formats.sbml.Model.')
+                '<' + str(model) + '> needs to be an instance of'
+                ' myokit.formats.sbml.Model.')
 
         self._model = model
         self._sid = str(sid)
         self._units = None
 
     def set_units(self, units):
         """Sets this parameters units to the given ``units``."""
@@ -625,16 +625,16 @@
         This reaction's SId.
 
     """
     def __init__(self, model, sid):
 
         if not isinstance(model, Model):
             raise SBMLError(
-                '<' + str(model) + '> needs to be an instance of '
-                'myokit.formats.sbml.Model.')
+                '<' + str(model) + '> needs to be an instance of'
+                ' myokit.formats.sbml.Model.')
 
         self._model = model
         self._sid = str(sid)
 
         # Reactants, reaction products, and modifiers: all as SpeciesReference
         self._reactants = []
         self._products = []
@@ -646,16 +646,16 @@
         # The kinetic law specifying this reaction's rate (if set)
         self._kinetic_law = None
 
     def add_modifier(self, species, sid=None):
         """Adds a modifier to this reaction and returns the created object."""
         if not isinstance(species, Species):
             raise SBMLError(
-                '<' + str(species) + '> needs to be an instance of '
-                'myokit.formats.sbml.Species')
+                '<' + str(species) + '> needs to be an instance of'
+                ' myokit.formats.sbml.Species')
 
         sid = str(sid) if sid else sid
         if sid is not None:
             self._model._register_sid(sid)
         ref = ModifierSpeciesReference(species, sid)
         self._modifiers.append(ref)
         self._species[species.sid()] = species
@@ -664,16 +664,16 @@
     def add_product(self, species, sid=None):
         """
         Adds a reaction product to this reaction and returns the created
         object.
         """
         if not isinstance(species, Species):
             raise SBMLError(
-                '<' + str(species) + '> needs to be an instance of '
-                'myokit.formats.sbml.Species')
+                '<' + str(species) + '> needs to be an instance of'
+                ' myokit.formats.sbml.Species')
 
         sid = str(sid) if sid else sid
         if sid is not None:
             self._model._register_sid(sid)
         ref = SpeciesReference(species, sid)
         self._products.append(ref)
         self._species[species.sid()] = species
@@ -681,16 +681,16 @@
             self._model._assignables[sid] = ref
         return ref
 
     def add_reactant(self, species, sid=None):
         """Adds a reactant to this reaction and returns the created object."""
         if not isinstance(species, Species):
             raise SBMLError(
-                '<' + str(species) + '> needs to be an instance of '
-                'myokit.formats.sbml.Species')
+                '<' + str(species) + '> needs to be an instance of'
+                ' myokit.formats.sbml.Species')
 
         sid = str(sid) if sid else sid
         if sid is not None:
             self._model._register_sid(sid)
         ref = SpeciesReference(species, sid)
         self._reactants.append(ref)
         self._species[species.sid()] = species
@@ -727,16 +727,16 @@
 
     def set_kinetic_law(self, expression):
         """
         Sets this reaction's kinetic law (as a :class:`myokit.Expression`).
         """
         if not isinstance(expression, myokit.Expression):
             raise SBMLError(
-                '<' + str(expression) + '> needs to be an instance of '
-                'myokit.Expression.')
+                '<' + str(expression) + '> needs to be an instance of'
+                ' myokit.Expression.')
 
         self._kinetic_law = expression
 
     def sid(self):
         """Returns this reaction's sid."""
         return self._sid
 
@@ -773,15 +773,15 @@
     """
     def __init__(self, compartment, sid, is_amount, is_constant, is_boundary):
         super(Species, self).__init__()
 
         if not isinstance(compartment, Compartment):
             raise SBMLError(
                 '<' + compartment + '> needs to be instance of'
-                'myokit.formats.sbml.Compartment')
+                ' myokit.formats.sbml.Compartment')
         if not isinstance(is_amount, bool):
             raise SBMLError(
                 'Is_amount <' + str(is_amount) + '> needs to be a boolean.')
         if not isinstance(is_constant, bool):
             raise SBMLError(
                 'Is_constant <' + str(is_constant) + '> needs to be a boolean.'
             )
@@ -849,30 +849,30 @@
         """
         Sets a :class:`Parameter` as conversion factor for this species,
         see :meth:`conversion_factor()`.
         """
         if not isinstance(factor, Parameter):
             raise SBMLError(
                 '<' + str(factor) + '> needs to be instance of'
-                'myokit.formats.sbml.Parameter.')
+                ' myokit.formats.sbml.Parameter.')
 
         self._conversion_factor = factor
 
     def set_initial_value(self, value, in_amount=None):
         """
         Sets a :class:`myokit.Expression` for this species' initial value.
 
         `in_amount` is a boolean that indicates whether the initial value is
         measured in amount (True) or concentration (False). If set to `None`
         value is treated to have the same units as the species.
         """
         if not isinstance(value, myokit.Expression):
             raise SBMLError(
-                '<' + str(value) + '> needs to be an instance of '
-                'myokit.Expression.')
+                '<' + str(value) + '> needs to be an instance of'
+                ' myokit.Expression.')
         if (in_amount is not None) and (not isinstance(in_amount, bool)):
             raise SBMLError(
                 '<in_amount> needs to be an instance of bool or None.')
 
         self._initial_value = value
         self._initial_value_in_amount = in_amount
 
@@ -915,15 +915,15 @@
 
     def __init__(self, species, sid=None):
         super(SpeciesReference, self).__init__()
 
         if not isinstance(species, Species):
             raise SBMLError(
                 '<' + species + '> needs to be instance of'
-                'myokit.formats.sbml.Species')
+                ' myokit.formats.sbml.Species')
 
         self._species = species
         self._sid = str(sid) if sid else sid
 
     def species(self):
         """Returns the species this object refers to."""
         return self._species
@@ -941,15 +941,15 @@
 
     def __init__(self, species, sid=None):
         super(ModifierSpeciesReference, self).__init__()
 
         if not isinstance(species, Species):
             raise SBMLError(
                 '<' + species + '> needs to be instance of'
-                'myokit.formats.sbml.Species')
+                ' myokit.formats.sbml.Species')
 
         self._species = species
         self._sid = str(sid) if sid else sid
 
     def species(self):
         """Returns the species this object refers to."""
         return self._species
@@ -1054,15 +1054,15 @@
             sbml_model, variable_references, species_amount_references,
             expression_references)
 
         return myokit_model
 
     @staticmethod
     def add_global_component(
-            myokit_model, component_references, name='myokit'):
+            myokit_model, component_references, name='global'):
         """
         Creates a component used to store global parameters and the time
         variable.
 
         An attempt will be made to use the name given by the parameter
         ``name``, but if this is not available another similar name will be
         found (using :meth:`myokit.add_component_allow_renaming`).
@@ -1294,15 +1294,15 @@
                     state_value = 1
                     warnings.warn(
                         'Size of compartment <' + str(compartment) + '> is '
                         'promoted to state variable without being assigned '
                         'with an initial value. Default is set to 1.')
 
                 # Promote size to state variable
-                var.promote(state_value=state_value)
+                var.promote(state_value)
 
             # Set RHS
             # (assignmentRule overwrites initialAssignment)
             expr = compartment.value()
             if expr is not None:
                 expr = expr.clone(subst=expression_references)
                 try:
@@ -1379,15 +1379,15 @@
                     state_value = 0
                     warnings.warn(
                         'Species <' + str(species) + '> is promoted to state '
                         'variable without being assigned with an initial '
                         'value. Default is set to 0.')
 
                 # Promote size to state variable
-                var.promote(state_value=state_value)
+                var.promote(state_value)
                 var.set_rhs(myokit.Number(0))
 
             if (not var.rhs().is_literal()) or var.rhs().eval():
                 # Subtract rate contributions
                 # (Reaction removes species from compartment)
                 expr = myokit.Minus(var.rhs(), expr)
             else:
@@ -1469,15 +1469,15 @@
                     state_value = 0
                     warnings.warn(
                         'Species <' + str(species) + '> is promoted to state '
                         'variable without being assigned with an initial '
                         'value. Default is set to 0.')
 
                 # Promote size to state variable
-                var.promote(state_value=state_value)
+                var.promote(state_value)
                 var.set_rhs(myokit.Number(0))
 
             if (not var.rhs().is_literal()) or var.rhs().eval():
                 # Add rate contributions
                 expr = myokit.Plus(var.rhs(), expr)
 
             # Set RHS
@@ -1542,15 +1542,15 @@
                     state_value = 0
                     warnings.warn(
                         'Species <' + str(species) + '> is promoted to state '
                         'variable without being assigned with an initial '
                         'value. Default is set to 0.')
 
                 # Promote size to state variable
-                var.promote(state_value=state_value)
+                var.promote(state_value)
 
             # Set RHS (reactions are dealt with elsewhere)
             expr = species.value()
             if expr is not None:
                 # Need to convert initial value if species is measured in
                 # concentration (assignments match unit of measurement)
                 if not species.is_amount():
@@ -1603,15 +1603,15 @@
                     state_value = 0
                     warnings.warn(
                         'Parameter ' + str(parameter) + ' is promoted to'
                         ' state variable without being assigned with an'
                         ' initial value. Default is set to 1.')
 
                 # Promote size to state variable
-                var.promote(state_value=state_value)
+                var.promote(state_value)
 
             # Set RHS
             # (assignmentRule overwrites initialAssignment)
             expr = parameter.value()
             if expr is not None:
                 expr = expr.clone(subst=expression_references)
                 try:
@@ -1669,15 +1669,15 @@
                         warnings.warn(
                             'Stoichiometry of <' + str(species_reference) + '>'
                             ' is promoted to state variable without being '
                             'assigned with an initial value. Default is set to'
                             ' 1.')
 
                     # Promote size to state variable
-                    var.promote(state_value=state_value)
+                    var.promote(state_value)
 
                 # Set RHS
                 # (assignmentRule overwrites initialAssignment)
                 expr = species_reference.value()
                 if expr is not None:
                     expr = expr.clone(subst=expression_references)
                     try:
```

### Comparing `myokit-1.33.9/myokit/formats/sbml/_importer.py` & `myokit-1.34.0/myokit/formats/sbml/_importer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/sbml/_parser.py` & `myokit-1.34.0/myokit/formats/sbml/_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/stan/__init__.py` & `myokit-1.34.0/myokit/formats/stan/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/stan/_ewriter.py` & `myokit-1.34.0/myokit/formats/stan/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/stan/_exporter.py` & `myokit-1.34.0/myokit/formats/stan/_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             return var.uname()
 
         # Expression writer
         ew = stan.StanExpressionWriter()
         ew.set_lhs_function(v)
 
         # Process bound variables
-        bound_variables = model.prepare_bindings({
+        bound_variables = myokit._prepare_bindings(model, {
             'time': 'time',
             'pace': 'pace',
         })
 
         # Common variables
         equations = model.solvable_order()
         components = []
```

### Comparing `myokit-1.33.9/myokit/formats/stan/template/cell.stan` & `myokit-1.34.0/myokit/formats/stan/template/cell.stan`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 functions{
 
   /**
    * Uses bisection to find a value `x` in a vector `sorted`.
    *
    * @param x The value to search for.
    * @param sorted A sorted (non-decreasing) vector of values to search in.
-   * @return The greatest array indice `i` such that `sorted[i] <= x`
+   * @return The greatest array index `i` such that `sorted[i] <= x`
    */
   int find_interval_elem(real x, vector sorted) {
 
     int N;
     int iter;
     int max_iter;
     int left_ind;
@@ -79,18 +79,18 @@
   real get_pacing_value(real time, real[] xr, int[] xi) {
 
     // Split real inputs into times and values vector
     int n = xi[1];
     vector[n] times  = to_vector(xr[1:n]);
     vector[n] values = to_vector(xr[(n + 1):(2 * n)]);
 
-    // Find indice for current time
+    // Find index for current time
     int i = find_interval_elem(time, values);
 
-    // Return pacing value
+    // Return pacing valueo
     return (i == 0) ? values[1] : values[i];
   }
 
   /**
    * Calculates the model derivatives
    *
    *
```

### Comparing `myokit-1.33.9/myokit/formats/sympy/__init__.py` & `myokit-1.34.0/myokit/formats/sympy/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/sympy/_ereader.py` & `myokit-1.34.0/myokit/formats/sympy/_ereader.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/sympy/_ewriter.py` & `myokit-1.34.0/myokit/formats/sympy/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/wcp/_wcp.py` & `myokit-1.34.0/myokit/formats/wcp/_wcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         return self._filename
 
     def myokit_log(self):
         """
         Creates and returns a:class:`myokit.DataLog` containing all the
         data from this file.
 
-        Each channel is stored under its own name, with an indice indicating
+        Each channel is stored under its own name, with an index indicating
         the record it was from. Time is stored under ``time``.
         """
         log = myokit.DataLog()
         log.set_time_key('time')
         log['time'] = np.array(self._time)
         for i, record in enumerate(self._records):
             for j, data in enumerate(record):
```

### Comparing `myokit-1.33.9/myokit/formats/xml/__init__.py` & `myokit-1.34.0/myokit/formats/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/formats/xml/_exporter.py` & `myokit-1.34.0/myokit/formats/xml/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/gui/__init__.py` & `myokit-1.34.0/myokit/gui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,14 +298,20 @@
 else:
 
     raise Exception('Selection of qt version failed.')
 
 # Delete temporary variables
 del pyqt4, pyqt5, pyside
 
+# Load Gnome theme on Wayland (for icons)
+if platform == 'Linux':
+    icon = QtGui.QIcon.fromTheme('document-new')
+    if icon.isNull():
+        QtGui.QIcon.setThemeName('gnome')
+
 # Icons with fallback for apple and windows
 ICON_PATH = os.path.join(myokit.DIR_DATA, 'gui')
 ICONS = {
     'document-new': 'new.png',
     'document-open': 'open.png',
     'document-save': 'save.png',
     'edit-undo': 'undo.png',
```

### Comparing `myokit-1.33.9/myokit/gui/datablock_viewer.py` & `myokit-1.34.0/myokit/gui/datablock_viewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1115,15 +1115,15 @@
         self._tmin = 0
         self._tmax = 1
         self._trange = self._tmax - self._tmin
 
         # Current position in time
         self._position = self._tmin
 
-        # Colours for drawing
+        # Colors for drawing
         self._color_temp = Qt.black
         self._color_cycle = [
             Qt.red,
             #Qt.green,
             Qt.blue,
             #Qt.cyan,
             Qt.magenta,
@@ -1132,15 +1132,15 @@
             Qt.darkGreen,
             Qt.darkBlue,
             Qt.darkCyan,
             Qt.darkMagenta,
             Qt.darkYellow,
         ]
 
-        # Scaling factors from pixels to normalised (0, 1) coordinates. Updated
+        # Scaling factors from pixels to normalized (0, 1) coordinates. Updated
         # after every resize.
         self._sw = 1.0
         self._sh = 1.0
 
     def clear(self):
         """
         Removes all graphs from the widget.
@@ -1234,15 +1234,15 @@
     def mouseMoveEvent(self, event):
         """
         Trigger mouse moved event with graph coordinates.
         """
         if self._last_variable is None:
             return
 
-        # Get normalised x, y coordinates ([0, 1])
+        # Get normalized x, y coordinates ([0, 1])
         p = event.pos()
         x = float(p.x()) * self._sw
         y = 1 - float(p.y()) * self._sh
 
         # Scale x-axis according to time
         x = self._tmin + x * self._trange
```

### Comparing `myokit-1.33.9/myokit/gui/datalog_viewer.py` & `myokit-1.34.0/myokit/gui/datalog_viewer.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,14 +28,21 @@
 import matplotlib
 import matplotlib.figure
 from myokit.gui import matplotlib_backend as backend
 
 # NumPy
 import numpy as np
 
+# SciPy: Only used to load matlab files.
+try:
+    import scipy.io
+    has_scipy = True
+except ImportError:
+    has_scipy = False
+
 # ConfigParser in Python 2 and 3
 try:
     import ConfigParser as configparser
 except ImportError:
     import configparser
 
 
@@ -105,53 +112,90 @@
 
 class DataLogViewer(myokit.gui.MyokitApplication):
     """
     Graphical interface for viewing DataLog data.
     """
     def __init__(self, *filenames):
         super(DataLogViewer, self).__init__()
+
         # Set Title, icon
         self.setWindowTitle(TITLE + ' ' + myokit.__version__)
+
         # Set size, center
         self.resize(800, 600)
         qr = self.frameGeometry()
         cp = QtWidgets.QDesktopWidget().availableGeometry().center()
         qr.moveCenter(cp)
         self.move(qr.topLeft())
-        # Add widget for Abf file tabs
-        self._tabs = QtWidgets.QTabWidget()
+
+        # Add widget for file tabs
+        self._tabs = TabWidget()
         self._tabs.setTabsClosable(True)
         self._tabs.tabCloseRequested.connect(self.action_close)
+        self._tabs.currentChanged.connect(self.fileTabChangeEvent)
         self.setCentralWidget(self._tabs)
+
         # Menu bar
         self.create_menu()
+
         # Tool bar
         self.create_toolbar()
+
         # Status bar
         self.statusBar().showMessage('Ready')
+
         # Current path
         self._path = QtCore.QDir.currentPath()
+
         # Load settings from ini file
         self.load_config()
+
+        # File-loading methods
+        self._load_actions = {
+            '.abf': self.load_abf_file,
+            '.atf': self.load_atf_file,
+            '.csv': self.load_datalog,
+            '.pro': self.load_abf_file,
+            '.txt': self.load_txt_file,
+            '.wcp': self.load_wcp_file,
+            '.zip': self.load_datalog,
+        }
+        if has_scipy:
+            self._load_actions['.mat'] = self.load_mat_file
+
         # Load any selected files
         for filename in filenames:
             self.load_file(filename)
+        tc = self._tabs.count()
+        if tc > 0:
+            if tc > 1:
+                self._tool_next_file.setEnabled(True)
+                self._tool_prev_file.setEnabled(True)
+            self._tabs.setCurrentIndex(0)
 
     def action_about(self):
         """
         Displays the about dialog.
         """
         QtWidgets.QMessageBox.about(self, TITLE, ABOUT)
 
     def action_close(self, index):
         """
         Called when a tab should be closed
         """
+        # Remove tab
         tab = self._tabs.widget(index)
         self._tabs.removeTab(index)
+
+        # Update buttons
+        if self._tabs.count() < 2:
+            self._tool_next_file.setEnabled(False)
+            self._tool_prev_file.setEnabled(False)
+
+        # Delete tab
         if tab is not None:
             tab.deleteLater()
         gc.collect()
         del tab
 
     def action_license(self):
         """
@@ -164,21 +208,57 @@
         Let the user select and open a file.
         """
         filenames = QtWidgets.QFileDialog.getOpenFileNames(
             self, 'Open data file', self._path, filter=FILTER_LIST)[0]
         if filenames:
             # Save current number of tabs
             tab_count = self._tabs.count()
+
             # Load files
             for filename in filenames:
                 self.load_file(str(filename))
+
             # If loading went ok, show first of newly loaded files
-            if self._tabs.count() > tab_count:
+            tab_count_new = self._tabs.count()
+            if tab_count_new > tab_count:
                 self._tabs.setCurrentIndex(tab_count)
 
+                # Enable next/previous file menu items
+                if tab_count_new > 1:
+                    self._tool_next_file.setEnabled(True)
+                    self._tool_prev_file.setEnabled(True)
+
+    def action_next_file(self):
+        """
+        Select the next open file.
+        """
+        self._tabs.next()
+
+    def action_next_var(self):
+        """
+        Select the next variable in the selected file.
+        """
+        tab = self._tabs.currentWidget()
+        if tab:
+            tab.next()
+
+    def action_prev_file(self):
+        """
+        Select the previous open file.
+        """
+        self._tabs.previous()
+
+    def action_prev_var(self):
+        """
+        Select the previous variable in the selected file
+        """
+        tab = self._tabs.currentWidget()
+        if tab:
+            tab.previous()
+
     def closeEvent(self, event=None):
         """
         Called when window is closed. To force a close (and trigger this
         function, call self.close())
         """
         # Save configuration
         self.save_config()
@@ -207,14 +287,45 @@
         # File > Quit
         self._tool_exit = QtWidgets.QAction('&Quit', self)
         self._tool_exit.setShortcut('Ctrl+Q')
         self._tool_exit.setStatusTip('Exit application.')
         self._tool_exit.setIcon(QtGui.QIcon.fromTheme('application-exit'))
         self._tool_exit.triggered.connect(self.close)
         self._menu_file.addAction(self._tool_exit)
+        # View menu
+        self._menu_view = self._menu.addMenu('&View')
+        # View > Next file
+        self._tool_next_file = QtWidgets.QAction('Next file', self)
+        self._tool_next_file.setShortcut('Ctrl+PgDown')
+        self._tool_next_file.setStatusTip('Select the next open file')
+        self._tool_next_file.triggered.connect(self.action_next_file)
+        self._tool_next_file.setEnabled(False)
+        self._menu_view.addAction(self._tool_next_file)
+        # View > Previous file
+        self._menu_view.addAction(self._tool_next_file)
+        self._tool_prev_file = QtWidgets.QAction('Previous file', self)
+        self._tool_prev_file.setShortcut('Ctrl+PgUp')
+        self._tool_prev_file.setStatusTip('Select the previous open file')
+        self._tool_prev_file.triggered.connect(self.action_prev_file)
+        self._tool_prev_file.setEnabled(False)
+        self._menu_view.addAction(self._tool_prev_file)
+        # View > Next variable
+        self._tool_next_var = QtWidgets.QAction('Next variable', self)
+        self._tool_next_var.setShortcut('PgDown')
+        self._tool_next_var.setStatusTip('Show the next variable')
+        self._tool_next_var.triggered.connect(self.action_next_var)
+        self._tool_next_var.setEnabled(False)
+        self._menu_view.addAction(self._tool_next_var)
+        # View > Previous var
+        self._tool_prev_var = QtWidgets.QAction('Previous variable', self)
+        self._tool_prev_var.setShortcut('PgUp')
+        self._tool_prev_var.setStatusTip('Show the previous variable')
+        self._tool_prev_var.triggered.connect(self.action_prev_var)
+        self._tool_prev_var.setEnabled(False)
+        self._menu_view.addAction(self._tool_prev_var)
         # Help menu
         self._menu_help = self._menu.addMenu('&Help')
         # Help > About
         self._tool_about = QtWidgets.QAction('&About', self)
         self._tool_about.setStatusTip('View information about this program.')
         self._tool_about.triggered.connect(self.action_about)
         self._menu_help.addAction(self._tool_about)
@@ -270,26 +381,16 @@
                     self._path = path
 
     def load_file(self, filename):
         """
         Loads a data file.
         """
         root, ext = os.path.splitext(os.path.basename(filename))
-        actions = {
-            '.abf': self.load_abf_file,
-            '.atf': self.load_atf_file,
-            '.csv': self.load_datalog,
-            '.mat': self.load_mat_file,
-            '.pro': self.load_abf_file,
-            '.txt': self.load_txt_file,
-            '.wcp': self.load_wcp_file,
-            '.zip': self.load_datalog,
-        }
         try:
-            action = actions[ext.lower()]
+            action = self._load_actions[ext.lower()]
         except KeyError:
             QtWidgets.QMessageBox.critical(
                 self, TITLE, 'File format not recognized: ' + ext)
             return
         action(filename)
 
     def load_abf_file(self, filename):
@@ -340,16 +441,15 @@
     def load_mat_file(self, filename):
         """
         Loads a Matlab file.
 
         This method requires ``SciPy`` to be installed.
         """
         try:
-            from scipy.io import loadmat
-            mat = loadmat(filename)
+            mat = scipy.io.loadmat(filename)
         except Exception:
             e = traceback.format_exc()
             QtWidgets.QMessageBox.critical(self, TITLE, e)
             return
         self._path = os.path.dirname(filename)
         name = os.path.basename(filename)
         self._tabs.addTab(MatTab(self, mat, name), name)
@@ -407,16 +507,54 @@
     def show(self):
         """
         Shows this viewer.
         """
         super(DataLogViewer, self).show()
         QtWidgets.QApplication.processEvents()
 
+    def fileTabChangeEvent(self, index):
+        """
+        Different file tab selected.
+        """
+        if index >= 0:
+            tab = self._tabs.widget(index)
+            if tab.count() > 1:
+                self._tool_prev_var.setEnabled(True)
+                self._tool_next_var.setEnabled(True)
+                return
+        self._tool_prev_var.setEnabled(False)
+        self._tool_next_var.setEnabled(False)
 
-class AbfTab(QtWidgets.QTabWidget):
+
+class TabWidget(QtWidgets.QTabWidget):
+    """
+    Tab widget that can move up and down when asked.
+    """
+    def next(self):
+        """
+        Select the next widget.
+        """
+        n = self.count()
+        if n < 2:
+            return
+        i = self.currentIndex() + 1
+        self.setCurrentIndex(0 if i >= n else i)
+
+    def previous(self):
+        """
+        Select the previous widget.
+        """
+        n = self.count()
+        if n < 2:
+            return
+        i = self.currentIndex() - 1
+        self.setCurrentIndex(n - 1 if i < 0 else i)
+
+
+class AbfTab(TabWidget):
     """
     A widget displaying an ABF file.
     """
     def __init__(self, parent, abf):
         super(AbfTab, self).__init__(parent)
         self.setTabsClosable(False)
         self.setTabPosition(self.East)
@@ -510,15 +648,15 @@
         for axes in self._axes:
             axes.cla()
         del self._figures, self._axes
         gc.collect()
         super(AbfTab, self).deleteLater()
 
 
-class AtfTab(QtWidgets.QTabWidget):
+class AtfTab(TabWidget):
     """
     A widget displaying an AGF file.
     """
     def __init__(self, parent, atf):
         super(AtfTab, self).__init__(parent)
         self._atf = atf
 
@@ -581,15 +719,15 @@
         for axes in self._axes:
             axes.cla()
         del self._figures, self._axes
         gc.collect()
         super(AtfTab, self).deleteLater()
 
 
-class CsvTab(QtWidgets.QTabWidget):
+class CsvTab(TabWidget):
     """
     A widget displaying a CSV file.
 
     The given log must have a time variable set.
     """
     def __init__(self, parent, log, filename):
         super(CsvTab, self).__init__(parent)
@@ -615,35 +753,57 @@
 
         # Check that time series aren't empty
         if log.length() == 0:
             QtWidgets.QMessageBox.critical(
                 self, TITLE, 'Unable to load file: no data found.')
             return
 
-        # Add tab for each column
-        for k, v in log.items():
-            if k == time:
+        # Overlapping sweeps or neighboring cells?
+        keys = []
+        groups = {}
+        for key in log.keys():
+            if key == time:
                 continue
-            self.addTab(self.create_graph_tab(k, v), k)
+            index, var = myokit.split_key(key)
+            if index:
+                group = groups.get(var, None)
+                if group is None:
+                    groups[var] = [index]
+                    keys.append(var)
+                else:
+                    group.append(index)
+            else:
+                keys.append(var)
+
+        # Add tab for each column
+        for k in keys:
+            self.addTab(self.create_graph_tab(k, groups.get(k)), k)
 
-    def create_graph_tab(self, key, data):
+    def create_graph_tab(self, key, indices=None):
         """
-        Creates a widget displaying the ``data`` stored under ``key``.
+        Creates a widget displaying the data stored under ``key``.
         """
         widget = QtWidgets.QWidget(self)
+
         # Create figure
         figure = matplotlib.figure.Figure()
         figure.suptitle(self._filename)
         canvas = backend.FigureCanvasQTAgg(figure)
         canvas.setParent(widget)
         axes = figure.add_subplot(1, 1, 1)
         axes.set_title(key)
         toolbar = backend.NavigationToolbar2QT(canvas, widget)
+
         # Draw lines
-        axes.plot(self._time, data)
+        if indices is None:
+            axes.plot(self._time, self._log[key])
+        else:
+            for i in indices:
+                axes.plot(self._time, self._log[i + key])
+
         # Create a layout
         vbox = QtWidgets.QVBoxLayout()
         vbox.addWidget(canvas)
         vbox.addWidget(toolbar)
         widget.setLayout(vbox)
         self._figures.append(figure)
         self._axes.append(axes)
@@ -658,15 +818,15 @@
         for axes in self._axes:
             axes.cla()
         del self._figures, self._axes
         gc.collect()
         super(CsvTab, self).deleteLater()
 
 
-class MatTab(QtWidgets.QTabWidget):
+class MatTab(TabWidget):
     """
     A widget displaying a MAT file.
     """
     def __init__(self, parent, mat, filename):
         super(MatTab, self).__init__(parent)
         self.setTabsClosable(False)
         self.setTabPosition(self.East)
@@ -746,15 +906,15 @@
         for axes in self._axes:
             axes.cla()
         del self._figures, self._axes
         gc.collect()
         super(MatTab, self).deleteLater()
 
 
-class TxtTab(QtWidgets.QTabWidget):
+class TxtTab(TabWidget):
     """
     A widget displaying a TXT file (with lots of heuristics!).
     """
     def __init__(self, parent, data, filename):
         super(TxtTab, self).__init__(parent)
         self.setTabsClosable(False)
         self.setTabPosition(self.East)
@@ -828,15 +988,15 @@
         for axes in self._axes:
             axes.cla()
         del self._figures, self._axes
         gc.collect()
         super(TxtTab, self).deleteLater()
 
 
-class WcpTab(QtWidgets.QTabWidget):
+class WcpTab(TabWidget):
     """
     A widget displaying a WCP file.
     """
     def __init__(self, parent, wcp):
         super(WcpTab, self).__init__(parent)
         self.setTabsClosable(False)
         self.setTabPosition(self.East)
```

### Comparing `myokit-1.33.9/myokit/gui/explorer.py` & `myokit-1.34.0/myokit/gui/explorer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/gui/ide.py` & `myokit-1.34.0/myokit/gui/ide.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,16 +267,17 @@
         # Load settings from ini file
         self.load_config()
 
         # Cached validated model and protocol
         self._valid_model = None
         self._valid_protocol = None
 
-        # Last-found model error
+        # Last-found model and protocol error
         self._last_model_error = None
+        self._last_protocol_error = None
 
         # React to changes to model and protocol
         # (For example devalidate model and protocol upon any changes)
         self._model_editor.textChanged.connect(self.change_model)
         self._protocol_editor.textChanged.connect(self.change_protocol)
 
         # Starting off on the model tab, so disable actions specific to
@@ -811,26 +812,44 @@
             self.show_exception()
 
     def action_jump_to_error(self):
         """
         Jump to the last error in the model tab.
         """
         try:
-            # Check for error
-            self.model(console=True)
-            if self._last_model_error is None:
-                return
-            # Switch to model tab if required
-            self._editor_tabs.setCurrentWidget(self._model_tab)
-            # Show error
-            line = self._last_model_error.line
-            char = self._last_model_error.char
-            self.statusBar().showMessage(
-                'Jumping to (' + str(line) + ',' + str(char) + ').')
-            self._model_editor.jump_to(line - 1, char)
+            t = self._editor_tabs.currentWidget()
+            if t is self._model_tab:
+
+                # Check for error
+                self.model(console=True)
+                if self._last_model_error is None:
+                    return
+
+                # Show error
+                line = self._last_model_error.line
+                char = self._last_model_error.char
+                self.statusBar().showMessage(
+                    'Jumping to (' + str(line) + ',' + str(char) + ').')
+                self._model_editor.jump_to(line - 1, char)
+
+            elif t is self._protocol_tab:
+
+                # Check for error
+                self.protocol(console=True)
+                if self._last_protocol_error is None:
+                    return
+
+                # Show error
+                line = self._last_protocol_error.line
+                char = self._last_protocol_error.char
+                self.statusBar().showMessage(
+                    'Jumping to (' + str(line) + ',' + str(char) + ').')
+                self._protocol_editor.jump_to(line - 1, char)
+
+            # Can't be called on script tab -- or does nothing
         except Exception:
             self.show_exception()
 
     def action_license(self):
         """
         Displays this program's licensing information.
         """
@@ -1139,19 +1158,23 @@
         """
         Undoes the previous text edit operation.
         """
         self._editor_tabs.currentWidget().editor.undo()
 
     def action_validate(self):
         """
-        Validates the model and, if the model is valid, the protocol.
+        Validates the model or the protocol, depending on the editor tab.
         """
         try:
-            self.model(console=True)
-            self.protocol(console=True)
+            current = self._editor_tabs.currentWidget()
+            if current is self._model_tab:
+                self.model(console=True)
+            elif current is self._protocol_tab:
+                self.protocol(console=True)
+            # Can't be called on script tab -- or does nothing
         except Exception:
             self.show_exception()
 
     def action_variable_definition(self):
         """
         Jump to the variable pointed at by the caret.
         """
@@ -1402,14 +1425,29 @@
         for widget in self._model_widgets:
             widget.setEnabled(index == 0)
         for widget in self._protocol_widgets:
             widget.setEnabled(index == 1)
         for widget in self._script_widgets:
             widget.setEnabled(index == 2)
 
+        # Update "validate" and "jump to last error" tools
+        if t is self._model_tab:
+            self._tool_validate.setText('Validate model')
+            self._tool_validate.setToolTip('Validate the model.')
+            self._tool_validate.setEnabled(True)
+            self._tool_jump_to_error.setEnabled(True)
+        elif t is self._protocol_tab:
+            self._tool_validate.setText('Validate protocol')
+            self._tool_validate.setToolTip('Validate the protocol.')
+            self._tool_validate.setEnabled(True)
+            self._tool_jump_to_error.setEnabled(True)
+        else:
+            self._tool_validate.setEnabled(False)
+            self._tool_jump_to_error.setEnabled(False)
+
     def change_model(self):
         """ Qt slot: Called whenever the model is changed. """
         self._valid_model = None
         # Bundle events in one-shot timer that calls change_model_timeout
         # Successive calls will restart the timer!
         self._model_changed_timer.start(100)    # in ms
 
@@ -2025,17 +2063,17 @@
         self._menu_analysis.addAction(self._tool_component_cycles)
         #
         # Run menu
         #
         self._menu_run = self._menu.addMenu('&Run')
         # Run > Validate
         self._tool_validate = QtWidgets.QAction(
-            '&Validate model and protocol', self)
+            '&Validate model', self)
         self._tool_validate.setShortcut('Ctrl+B')
-        self._tool_validate.setStatusTip('Validate the model and protocol')
+        self._tool_validate.setStatusTip('Validate the model.')
         self._tool_validate.triggered.connect(self.action_validate)
         self._menu_run.addAction(self._tool_validate)
         # Run > Jump to error
         self._tool_jump_to_error = QtWidgets.QAction(
             '&Jump to last error', self)
         self._tool_jump_to_error.setShortcut('Ctrl+Space')
         self._tool_jump_to_error.setStatusTip(
@@ -2234,15 +2272,16 @@
         written to the console. Similarly, the option ``errors_in_console``
         allows errors - but no positive parse results - to be shown in the
         console.
         """
         # Check for cached valid model
         if self._valid_model is not None and not force:
             if console:
-                self._console.write('No changes to model since last build.')
+                self._console.write(
+                    'No changes to model since last build (no errors found).')
             return self._valid_model
 
         # Parse and validate
         model = None
 
         # Reset last model error
         self._last_model_error = None
@@ -2348,20 +2387,25 @@
         written to the console. Similarly, the option ``errors_in_console``
         allows errors - but no positive parse results - to be shown in the
         console.
         """
         # Check for cached valid protocol
         if self._valid_protocol and not force:
             if console:
-                self._console.write('No changes to protocol since last build.')
+                self._console.write(
+                    'No changes to protocol since last build (no errors'
+                    ' found).')
             return self._valid_protocol
 
         # Parse and validate
         protocol = None
 
+        # Reset last protocol error
+        self._last_protocol_error = None
+
         # Check for empty protocol field
         lines = self._protocol_editor.get_text()
         if lines.strip() == '':
             if console:
                 self._console.write('No protocol found.')
             return None
 
@@ -2374,15 +2418,18 @@
             if console:
                 self._console.write('No errors found in protocol.')
             # Cache valid protocol
             self._valid_protocol = protocol
             return protocol
         except myokit.ParseError as e:
             if console or errors_in_console:
+                # Write error to console
                 self._console.write(myokit.format_parse_error(e, lines))
+                # Store error
+                self._last_protocol_error = e
             return False
 
     def save_config(self):
         """
         Saves the user configuration to an ini file.
         """
         config = configparser.RawConfigParser()
```

### Comparing `myokit-1.33.9/myokit/gui/progress.py` & `myokit-1.34.0/myokit/gui/progress.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/gui/source.py` & `myokit-1.34.0/myokit/gui/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 # Selected line is highlighted
 COLOR_SELECTED_LINE = QtGui.QColor(238, 238, 238)
 
 
 def _check_for_dark_mode(palette):
     """
-    Checks the default editor background color, and adjusts the colour scheme
+    Checks the default editor background color, and adjusts the color scheme
     if it looks like dark-mode is enabled.
     """
     c = palette.base().color()
     c = (c.blueF() + c.greenF() + c.redF()) / 3
     dark = c < 0.5
 
     # Don't mess with these directly: Use the SVG in myokit-docs
@@ -969,15 +969,15 @@
 
         # Simple rules
         self._rules = []
 
         # Numbers
         pattern = QtCore.QRegExp(r'\b[+-]?[0-9]*\.?[0-9]+([eE][+-]?[0-9]+)?\b')
         self._rules.append((pattern, STYLE_LITERAL))
-        unit = r'\[[a-zA-Z0-9/^]+\]'
+        unit = r'\[[a-zA-Z0-9/^-*]+\]'
         self._rules.append((QtCore.QRegExp(unit), STYLE_INLINE_UNIT))
 
         # Keywords
         for keyword in self.KEYWORD_1:
             pattern = QtCore.QRegExp(r'\b' + keyword + r'\b')
             self._rules.append((pattern, STYLE_KEYWORD_1))
         for keyword in self.KEYWORD_2:
```

### Comparing `myokit-1.33.9/myokit/gui/vargrapher.py` & `myokit-1.34.0/myokit/gui/vargrapher.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/lib/deps.py` & `myokit-1.34.0/myokit/lib/deps.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,24 +48,24 @@
     iknock = []
     if knockout is not None:
         for v in knockout:
             # Ensure all items in knockout are state variables from this model
             v = model.get(v, class_filter=myokit.Variable)
             if not v.is_state():
                 raise ValueError('Knockout variables must be states.')
-            iknock.append(v.indice())
+            iknock.append(v.index())
 
     # Create matrix of direct dependencies
     m = []
     for i, var in enumerate(states):
         row = [0] * n
         if i not in iknock:
             for dep in deep[var.lhs()]:
                 if dep.var().is_state():
-                    j = dep.var().indice()
+                    j = dep.var().index()
                     if j not in iknock:
                         row[j] = 1
         m.append(row)
 
     # Return directly
     if direct:
         return m
@@ -451,15 +451,15 @@
                     node.x = j * fx
 
         # Iteratively update x coordinates using median rule
         max_runs = 100
         for n_runs in range(max_runs):
             change = False
             for i, layer in enumerate(layers):
-                # Set nodes to median of neighbours
+                # Set nodes to median of neighbors
                 for j, node in enumerate(layer):
                     n = len(node.edgi) + len(node.edgo)
                     if n > 0:
                         nodes = list(node.edgi)
                         nodes.extend(list(node.edgo))
                         nodes.sort(key=lambda snode: snode.x)
                         node.x = nodes[int(n / 2)].x
@@ -489,16 +489,16 @@
                             eq = [last, node]
                             # Get last x
                             x1 = 0.0 if j == 1 else layer[j - 2].x
                             # Get next x
                             x2 = None
                             for k in range(j + 1, n):
                                 if abs(layer[k].x - node.x) >= too_close:
-                                    x2 = layer[k].x
-                                    break
+                                    x2 = layer[k].x     # pragma: no cover
+                                    break               # pragma: no cover
                                 eq.append(layer[k])
                             if x2 is None:
                                 x2 = 1.0
                             # Space nodes between x1 and x2
                             dx = (x2 - x1) / (1.0 + len(eq))
                             for k, enode in enumerate(eq):
                                 enode.x = x1 + dx * (1 + k)
```

### Comparing `myokit-1.33.9/myokit/lib/guess.py` & `myokit-1.34.0/myokit/lib/guess.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,15 +388,15 @@
     for v in model.variables(deep=True):
         if v.meta.get('oxmeta', None) == 'membrane_voltage':
             return v
 
     # Common units for the membrane potential
     common_units = [myokit.units.V]
 
-    # Non-dimensionalised (e.g. Mitchell-Schaeffer) use [1]
+    # Non-dimensionalized (e.g. Mitchell-Schaeffer) use [1]
     # But this causes too many false positives
     # common_units.append(myokit.units.dimensionless)
 
     # Common names for the membrane potential
     common_component_names = [
         'membrane',
         'cell',
@@ -577,15 +577,15 @@
     # Units that current is often expressed in (give or take a multiplier)
     common_units = [
         myokit.units.A,
         myokit.units.A / myokit.units.F,
         myokit.units.A / myokit.units.m**2,
     ]
 
-    # Non-dimensionalised (e.g. Mitchell-Schaeffer) use [mS/uF]
+    # Non-dimensionalized (e.g. Mitchell-Schaeffer) use [mS/uF]
     # But this causes too many false positives
     # common_units.append(myokit.units.S / myokit.units.F)
 
     # Common names for stimulus current variables (lowercase)
     common_names = [
         'istim',
         'i_stim',
```

### Comparing `myokit-1.33.9/myokit/lib/hh.py` & `myokit-1.34.0/myokit/lib/hh.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     constant ``tau_x[i]``, where ``V`` is the membrane potential, ``p`` is a
     set of parameters, ``f`` is an arbitrary function (for example
     ``g_max * (V - E_rev)``).
 
     The model variables to treat as parameter are specified by the user when
     the model is created. Any other variables, for example state variables such
     as intercellular calcium or constants such as temperature, are fixed when
-    the current model is created and can no longer be changed.
+    the current model is created and can no longer be changed. Initial values
+    written as expressions are evaluated when the model is made.
 
     The current variable is optional.
 
     Arguments:
 
     ``model``
         The :class:`myokit.Model` to extract a current model from.
@@ -79,15 +80,15 @@
 
         import myokit
         import myokit.lib.hh as hh
 
         # Load a model from disk
         model = myokit.load_model('some-model.mmt')
 
-        # Extract a markov model
+        # Extract a Hodgkin-Huxley style channel model
         mm = hh.HHModel.from_component(model.get('ina'))
 
     """
     # NOTE: A HHModel must be immutable!
     # This ensures that the simulations don't have to clone it (which would be
     # costly and difficult).
     # A HHModel can return a function to calculate state values, but it never
@@ -179,23 +180,26 @@
                 'The membrane potential should not be included in the list of'
                 ' states.')
         if self._membrane_potential == self._current:
             raise HHModelError(
                 'The membrane potential should not be the current variable.')
         del vm
 
+        # Get values of all states
+        # Note: Do this _before_ changing the model!
+        s = self._model.initial_values(True)
+        self._model.set_initial_values(s)  # Remove expressions
+        self._default_state = np.array(
+            [v.initial_value(True) for v in self._states])
+
         #
         # Demote unnecessary states and remove bindings
         #
-        # Get values of all states
-        # Note: Do this _before_ changing the model!
-        self._default_state = np.array([v.state_value() for v in self._states])
 
         # Freeze remaining, non-current-model states
-        s = self._model.state()   # Get state values before changing anything!
         # Note: list() cast is required so that we iterate over a static list,
         # otherwise we can get issues because the iterator depends on the model
         # (which we're changing).
         for k, state in enumerate(list(self._model.states())):
             if state not in self._states:
                 state.demote()
                 state.set_rhs(s[k])
@@ -342,27 +346,27 @@
         Returns the name of the current variable used by this model, or None if
         no current variable was specified.
         """
         return self._current
 
     def default_membrane_potential(self):
         """
-        Returns this markov model's default membrane potential value.
+        Returns this HH model's default membrane potential value.
         """
         return self._default_inputs[0]
 
     def default_parameters(self):
         """
-        Returns this markov model's default parameter values
+        Returns this HH model's default parameter values
         """
         return list(self._default_inputs[1:])
 
     def default_state(self):
         """
-        Returns this markov model's default state values.
+        Returns this HH model's default state values.
         """
         return list(self._default_state)
 
     @staticmethod
     def from_component(
             component, states=None, parameters=None, current=None, vm=None):
         """
@@ -385,16 +389,16 @@
 
         # Get or check states
         if states is None:
 
             # Get state variables
             states = [x for x in component.variables(state=True)]
 
-            # Sort by state indice
-            states.sort(key=lambda x: x.indice())
+            # Sort by state index
+            states.sort(key=lambda x: x.index())
 
         else:
 
             # Make sure states are variables. This is required to automatically
             # find a current variable.
             states_in = states
             states = []
```

### Comparing `myokit-1.33.9/myokit/lib/markov.py` & `myokit-1.34.0/myokit/lib/markov.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,16 @@
     that for fixed ``p`` and ``V`` this would resolve to
     ``I = (g * (V - E)) * O``, such that ``g * (V - E)`` is a constant that can
     be included in ``B``.
 
     The model variables to treat as parameter are specified by the user when
     the model is created. Any other variables, for example state variables such
     as intercellular calcium or constants such as temperature, are fixed when
-    the markov model is created and can no longer be changed.
+    the markov model is created and can no longer be changed. Initial values
+    written as expressions are evaluated when the model is made.
 
     To create a :class:`Markov`, pass in a :class:`myokit.Model` and select a
     list of states. All other states will be fixed at their current value and
     an attempt will be made to write the remaining state equations as linear
     combinations of the states. If this is not possible, a :class:`ValueError`
     is raised. The membrane potential must be indicated using the label
     ``membrane_potential`` or by passing it in as ``vm``.
@@ -201,23 +202,25 @@
                 'The membrane potential should not be included in the list of'
                 ' states.')
         if self._membrane_potential == self._current:
             raise LinearModelError(
                 'The membrane potential should not be the current variable.')
         del vm
 
+        # Get values of all states
+        # Note: Do this _before_ changing the model!
+        s = self._model.initial_values(True)
+        self._default_state = np.array(
+            [v.initial_value(True) for v in self._states])
+
         #
         # Demote unnecessary states, remove bindings and validate model.
         #
-        # Get values of all states
-        # Note: Do this _before_ changing the model!
-        self._default_state = np.array([v.state_value() for v in self._states])
 
         # Freeze remaining, non-markov-model states
-        s = self._model.state()   # Get state values before changing anything!
         for k, state in enumerate(self._model.states()):
             if state not in self._states:
                 state.demote()
                 state.set_rhs(s[k])
         del s
 
         # Unbind everything except time
@@ -456,16 +459,16 @@
 
         # Get or check states
         if states is None:
 
             # Get state variables
             states = [x for x in component.variables(state=True)]
 
-            # Sort by state indice
-            states.sort(key=lambda x: x.indice())
+            # Sort by state index
+            states.sort(key=lambda x: x.index())
 
         else:
 
             # Make sure states are variables. This is required to automatically
             # find a current variable.
             states_in = states
             states = []
@@ -1221,15 +1224,15 @@
         x = np.array(x, copy=False, dtype=float)
         if (np.abs(1 - np.sum(x))) > 1e-6:
             raise ValueError(
                 'The sum of fractions in the state to be discretized must'
                 ' equal 1.')
         y = np.round(x * self._nchannels)
         # To make sure it always sums to 1, correct the value found at the
-        # indice with the biggest rounding error.
+        # index with the biggest rounding error.
         i = np.argmax(np.abs(x - y))
         y[i] = 0
         y[i] = self._nchannels - np.sum(y)
         return list(y)
 
     def membrane_potential(self):
         """
@@ -1697,15 +1700,15 @@
             raise ValueError(
                 'Expression passed to _split_factor must be a single term.')
         else:
             raise ValueError(
                 'Non-linear function of ' + str(name) + ' found in '
                 + str(term) + '.')
 
-    # Finalise multiplier
+    # Finalize multiplier
     if m is None:
         m = myokit.Number(1)
     if not positive:
         m = myokit.PrefixMinus(m)
 
     # Return
     return name, m
```

### Comparing `myokit-1.33.9/myokit/lib/multi.py` & `myokit-1.34.0/myokit/lib/multi.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/lib/plots.py` & `myokit-1.34.0/myokit/lib/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,15 +261,16 @@
                 size=14,
                 bbox=bbox_props)
     return ax
 
 
 def cumulative_current(
         log, currents, axes=None, labels=None, colors=None, integrate=False,
-        normalise=False, max_currents=None, line_args={}, fill_args={}):
+        normalize=False, max_currents=None, line_args={}, fill_args={},
+        normalise=None):
     """
     Plots a number of currents, one on top of the other, with the positive and
     negative parts of the current plotted separately.
 
     The advantage of this type of plot is that it shows the relative size of
     each current versus the others, and gives an indication of the total
     positive and negative current in a model.
@@ -287,16 +288,16 @@
         Can be used to pass in a list containing the label to set for each
         current.
     ``colors``
         Can be used to pass in a list containing the colors to set for each
         current.
     ``integrate``
         Set this to ``True`` to plot total carried charge instead of currents.
-    ``normalise``
-        Set this to ``True`` to normalise the graph at every point, so that the
+    ``normalize``
+        Set this to ``True`` to normalize the graph at every point, so that the
         relative contribution of each current is shown.
     ``max_currents``
         Set this to any integer n to display only the first n currents, and
         group the rest together in a remainder current.
     ``line_args``
         An optional dict with keyword arguments to pass in when drawing lines.
     ``fill_args``
@@ -306,14 +307,23 @@
     The best results are obtained if relatively constant currents are specified
     early. Another rule of thumb is to specify the currents roughly in the
     order they appear during an AP.
     """
     import matplotlib
     import matplotlib.pyplot as plt
 
+    # Deprecated on 2023-06-7
+    if normalize is not None:
+        import warnings
+        warnings.warn(
+            'The keyword argument `normalise` is deprecated. Please use'
+            ' `normalize` instead.')
+        normalize = normalise
+    del normalise
+
     # Get axes
     if axes is None:
         axes = plt.gca()
 
     # Get numpy version of log
     log = log.npview()
 
@@ -326,16 +336,16 @@
     else:
         pos = np.array([log[c] for c in currents])
 
     # Split positive and negative
     neg = np.minimum(pos, 0)
     pos = np.maximum(pos, 0)
 
-    # Normalise
-    if normalise:
+    # Normalize
+    if normalize:
         pos /= np.maximum(np.sum(pos, axis=0), 1e-99)
         neg /= -np.minimum(np.sum(neg, axis=0), -1e-99)
 
     # Number of currents to show
     nc = len(currents)
     if max_currents is None or max_currents + 1 >= nc:
         show_remainder = False
@@ -346,15 +356,18 @@
 
     # Colors
     if colors:
         while len(colors) < nc:
             colors.extend(colors)
     else:
         # Colormap
-        cmap = matplotlib.cm.get_cmap(name='tab20')
+        try:
+            cmap = matplotlib.colormaps['tab20']
+        except AttributeError:  # pragma: no cover
+            cmap = matplotlib.cm.get_cmap(name='tab20')
         colors = [cmap(i) for i in range(nc)]
 
     # Line drawing keyword arguments
     if 'color' not in line_args:
         line_args['color'] = 'k'
     if 'lw' not in line_args:
         line_args['lw'] = 1
```

### Comparing `myokit-1.33.9/myokit/pacing.py` & `myokit-1.34.0/myokit/pacing.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/pype.py` & `myokit-1.34.0/myokit/pype.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/__init__.py` & `myokit-1.34.0/myokit/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/ansic_event_based_pacing.py` & `myokit-1.34.0/myokit/tests/ansic_event_based_pacing.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/ansic_fixed_form_pacing.py` & `myokit-1.34.0/myokit/tests/ansic_fixed_form_pacing.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 class AnsicFixedFormPacing(myokit.CModule):
     """
     Class for testing the fixed-form pacing system.
     """
     _index = 0
 
-    def __init__(self, times=None, values=None):
+    def __init__(self, protocol):
         super(AnsicFixedFormPacing, self).__init__()
 
         # Unique id
         AnsicFixedFormPacing._index += 1
         module_name = \
             'myokit_ansic_fpacing_' + str(AnsicFixedFormPacing._index)
 
@@ -39,15 +39,15 @@
         args = {'module_name': module_name}
         libs = []
         libd = []
         incd = [DIR_TEST, myokit.DIR_CFUNC]
         self._sys = self._compile(module_name, fname, args, libs, libd, incd)
 
         # Initialize
-        self._sys.init(times, values)
+        self._sys.init(protocol)
 
     def pace(self, time):
         return self._sys.pace(time)
 
     def __del__(self):
         # Free the memory used by the pacing system
         try:
```

### Comparing `myokit-1.33.9/myokit/tests/data/beeler-1977-model-compare-a.mmt` & `myokit-1.34.0/myokit/tests/data/beeler-1977-model-compare-a.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/beeler-1977-model-compare-b.mmt` & `myokit-1.34.0/myokit/tests/data/beeler-1977-model-compare-b.mmt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [[model]]
 name: beeler-1977-with-differences
 desc: """
     The 1997 Beeler Reuter model of the AP in ventricular myocytes.
-    
+
     This test version has some differences
 
     Reference:
 
     Beeler, Reuter (1976) Reconstruction of the action potential of ventricular
     myocardial fibres
     """
@@ -14,15 +14,15 @@
 f(x) = 5 * x
 g(x) = 3 * x
 # Initial values:
 membrane.V  = -84.622
 calcium.Cai = 2e-7
 ina.m       = 0.01
 ina.h       = 1.0
-ina.j       = 0.98
+ina.j       = 0.97 + 0.01
 isiz.d       = 0.003
 isiz.f       = 1.0
 
 
 [engine]
 toim = 0 in [ms] bind time
 pace = 0 bind pace
```

### Comparing `myokit-1.33.9/myokit/tests/data/beeler-1977-model.mmt` & `myokit-1.34.0/myokit/tests/data/beeler-1977-model.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/beeler-1977-units.mmt` & `myokit-1.34.0/myokit/tests/data/beeler-1977-units.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/clancy-1999-fitting.mmt` & `myokit-1.34.0/myokit/tests/data/clancy-1999-fitting.mmt`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
 dot(C3) = -C3 * (a11           ) + C2 * b11
 dot(C2) = -C2 * (a12 + b11     ) + C1 * b12 + C3 * a11
 dot(C1) = -C1 * (a13 + b12 + b3) + O  * b13 + C2 * a12 + IF * a3
 dot(O)  = -O  * (a2  + b13     ) + C1 * a13 + IF * b2
 dot(IF) = -IF * (a4  + b2  + a3) + IS * b4  + O  * a2  + C1 * b3
 dot(IS) = -IS * (b4            ) + IF * a4
 i = gmax * O * (V - E)
+p = 1e-4
 
 [[protocol]]
 # Level  Start    Length   Period   Multiplier
 1.0      10.0      0.5      1000.0   0
 
 [[script]]
 #
```

### Comparing `myokit-1.33.9/myokit/tests/data/conditional.mmt` & `myokit-1.34.0/myokit/tests/data/conditional.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/cv1d.mmt` & `myokit-1.34.0/myokit/tests/data/cv1d.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/cv1d.zip` & `myokit-1.34.0/myokit/tests/data/cv1d.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/decker-2009.mmt` & `myokit-1.34.0/myokit/tests/data/decker-2009.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/decker.model` & `myokit-1.34.0/myokit/tests/data/decker.model`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/dn-1985-normalised.mmt` & `myokit-1.34.0/myokit/tests/data/dn-1985-normalised.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/dom-markov.mmt` & `myokit-1.34.0/myokit/tests/data/dom-markov.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/abf-protocol.pro` & `myokit-1.34.0/myokit/tests/data/formats/abf-protocol.pro`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/abf-v1.abf` & `myokit-1.34.0/myokit/tests/data/formats/abf-v1.abf`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/abf-v2.abf` & `myokit-1.34.0/myokit/tests/data/formats/abf-v2.abf`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/cellml/br-1977-dot.cellml` & `myokit-1.34.0/myokit/tests/data/formats/cellml/br-1977-dot.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/cellml/br-1977.cellml` & `myokit-1.34.0/myokit/tests/data/formats/cellml/br-1977.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/cellml/corrias.cellml` & `myokit-1.34.0/myokit/tests/data/formats/cellml/corrias.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/cellml/decker-2009.cellml` & `myokit-1.34.0/myokit/tests/data/formats/cellml/decker-2009.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/cellml/documentation.cellml` & `myokit-1.34.0/myokit/tests/data/formats/cellml/documentation.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml` & `myokit-1.34.0/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml` & `myokit-1.34.0/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml` & `myokit-1.34.0/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml` & `myokit-1.34.0/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml` & `myokit-1.34.0/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/sbml/HodgkinHuxley.xml` & `myokit-1.34.0/myokit/tests/data/formats/sbml/HodgkinHuxley.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml` & `myokit-1.34.0/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml` & `myokit-1.34.0/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml` & `myokit-1.34.0/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/sbml/result/00001-results.csv` & `myokit-1.34.0/myokit/tests/data/formats/sbml/result/00001-results.csv`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/sbml/result/00004-results.csv` & `myokit-1.34.0/myokit/tests/data/formats/sbml/result/00004-results.csv`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/sbml/result/01103-results.csv` & `myokit-1.34.0/myokit/tests/data/formats/sbml/result/01103-results.csv`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/formats/wcp-file.wcp` & `myokit-1.34.0/myokit/tests/data/formats/wcp-file.wcp`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/bad1d-1-not-enough-files.zip` & `myokit-1.34.0/myokit/tests/data/io/bad1d-1-not-enough-files.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/bad1d-2-no-header.zip` & `myokit-1.34.0/myokit/tests/data/io/bad1d-2-no-header.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/bad1d-3-no-data.zip` & `myokit-1.34.0/myokit/tests/data/io/bad1d-3-no-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/bad1d-4-not-a-zip.zip` & `myokit-1.34.0/myokit/tests/data/io/bad1d-4-not-a-zip.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/bad1d-5-bad-data-type.zip` & `myokit-1.34.0/myokit/tests/data/io/bad1d-5-bad-data-type.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/bad1d-6-time-too-short.zip` & `myokit-1.34.0/myokit/tests/data/io/bad1d-6-time-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/bad1d-7-0d-too-short.zip` & `myokit-1.34.0/myokit/tests/data/io/bad1d-7-0d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/bad1d-8-1d-too-short.zip` & `myokit-1.34.0/myokit/tests/data/io/bad1d-8-1d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/bad2d-1-not-enough-files.zip` & `myokit-1.34.0/myokit/tests/data/io/bad2d-1-not-enough-files.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/bad2d-2-no-header.zip` & `myokit-1.34.0/myokit/tests/data/io/bad2d-2-no-header.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/bad2d-3-no-data.zip` & `myokit-1.34.0/myokit/tests/data/io/bad2d-3-no-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/bad2d-4-not-a-zip.zip` & `myokit-1.34.0/myokit/tests/data/io/bad2d-4-not-a-zip.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/bad2d-5-bad-data-type.zip` & `myokit-1.34.0/myokit/tests/data/io/bad2d-5-bad-data-type.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/bad2d-6-time-too-short.zip` & `myokit-1.34.0/myokit/tests/data/io/bad2d-6-time-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/bad2d-7-0d-too-short.zip` & `myokit-1.34.0/myokit/tests/data/io/bad2d-7-0d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/bad2d-8-2d-too-short.zip` & `myokit-1.34.0/myokit/tests/data/io/bad2d-8-2d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/badlog-1-no-data.zip` & `myokit-1.34.0/myokit/tests/data/io/badlog-1-no-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/badlog-2-no-structure.zip` & `myokit-1.34.0/myokit/tests/data/io/badlog-2-no-structure.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/badlog-4-invalid-n-fields.zip` & `myokit-1.34.0/myokit/tests/data/io/badlog-4-invalid-n-fields.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/badlog-5-invalid-data-size.zip` & `myokit-1.34.0/myokit/tests/data/io/badlog-5-invalid-data-size.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/badlog-6-bad-data-type.zip` & `myokit-1.34.0/myokit/tests/data/io/badlog-6-bad-data-type.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/badlog-7-not-enough-data.zip` & `myokit-1.34.0/myokit/tests/data/io/badlog-7-not-enough-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/block2d.mmt` & `myokit-1.34.0/myokit/tests/data/io/block2d.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/block2d.zip` & `myokit-1.34.0/myokit/tests/data/io/block2d.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/io/goodlog.zip` & `myokit-1.34.0/myokit/tests/data/io/goodlog.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/lr-1991-dep.mmt` & `myokit-1.34.0/myokit/tests/data/lr-1991-dep.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/lr-1991-fitting.mmt` & `myokit-1.34.0/myokit/tests/data/lr-1991-fitting.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/lr-1991-testing.mmt` & `myokit-1.34.0/myokit/tests/data/lr-1991-testing.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/lr-1991.mmt` & `myokit-1.34.0/myokit/tests/data/lr-1991.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/multi/beeler-no-name.mmt` & `myokit-1.34.0/myokit/tests/data/multi/beeler-no-name.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/multi/lr-1991.mmt` & `myokit-1.34.0/myokit/tests/data/multi/lr-1991.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/multi/subdir/beeler-no-name.mmt` & `myokit-1.34.0/myokit/tests/data/multi/subdir/beeler-no-name.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/data/noble-1962.mmt` & `myokit-1.34.0/myokit/tests/data/noble-1962.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_aux.py` & `myokit-1.34.0/myokit/tests/test_aux.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,15 @@
             '[x] Mismatched Meta property in model: "name"',
             '[2] Missing Meta property in model: "author"',
             '[1] Missing Meta property in model: "extra"',
             '[x] Mismatched User function <f(1)>',
             '[1] Missing User function <g(1)>.',
             '[x] Mismatched Time variable: [1]<engine.time> [2]<engine.toim>',
             '[x] Mismatched Initial value for <ina.h>',
+            '[x] Mismatched Initial value for <ina.j>',
             '[x] Mismatched State at position 5: [1]<isi.d> [2]<isiz.d>',
             '[x] Mismatched State at position 6: [1]<isi.f> [2]<isiz.f>',
             '[2] Missing state at position 7',
             '[x] Mismatched RHS <calcium.Cai>',
             '[2] Missing Variable <engine.time>',
             '[1] Missing Variable <engine.toim>',
             '[x] Mismatched RHS <ina.h.alpha>',
@@ -189,17 +190,14 @@
             '  [1] beeler-1977',
             '  [2] beeler-1977-with-differences',
         ] + differences + [
             'Done',
             '  ' + str(len(differences)) + ' differences found',
         ]
 
-        # Show massive diff messages
-        self.maxDiff = None
-
         caught_differences = set(capture.text().splitlines())
         live = set(live)
         self.assertEqual(live, caught_differences)
         differences = set(differences)
         caught_differences = set(c.text().splitlines())
         self.assertEqual(differences, caught_differences)
 
@@ -272,16 +270,14 @@
         # Test run() method.
 
         m, p, _ = myokit.load('example')
         x = '\n'.join([
             'import myokit',
             'm = get_model()',  # Test magic methods
             'p = get_protocol()',
-            's = myokit.Simulation(m, p)',
-            's.run(200)',
         ])
         with myokit.tools.capture():
             myokit.run(m, p, x)
         with myokit.tools.capture():
             myokit.run(m, p, '[[script]]\n' + x)
         self.assertRaises(ZeroDivisionError, myokit.run, m, p, 'print(1 / 0)')
 
@@ -509,14 +505,17 @@
         for a, b in zip(x, y):
             self.assertTrue(almost_equal(a, b))
         self.assertEqual(len(x), len(y))
 
         # Test positive/negative zero comparison
         m1 = myokit.Model()
         c = m1.add_component('c')
+        t = c.add_variable('t')
+        t.set_binding('time')
+        t.set_rhs(0)
         x = c.add_variable('x')
         x.promote(1)
         x.set_rhs('-0.0')
         y = c.add_variable('y')
         y.promote(1)
         y.set_rhs('0.0')
         m2 = m1.clone()
```

### Comparing `myokit-1.33.9/myokit/tests/test_cellml_v1_api.py` & `myokit-1.34.0/myokit/tests/test_cellml_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -726,16 +726,16 @@
         with WarningCollector() as w:
             cm.validate()
         self.assertFalse(w.has_warnings())
 
         # Recreate myokit model and test states
         mm = cm.myokit_model()
         mm.validate()
-        state_1 = m.state()
-        state_2 = mm.state()
+        state_1 = m.initial_values(True)
+        state_2 = mm.initial_values(True)
         states_1 = [x.name() for x in m.states()]
         states_2 = [x.name() for x in mm.states()]
         state_2 = [state_2[states_2.index(x)] for x in states_1]
         self.assertEqual(state_1[0], state_2[0])
         self.assertEqual(state_1[1], state_2[1])
         self.assertEqual(state_1[2], state_2[2])
         self.assertEqual(state_1[3], state_2[3])
@@ -826,15 +826,15 @@
         self.assertEqual(
             mz.rhs(),
             myokit.Plus(myokit.Number(3, myokit.units.volt), myokit.Name(mx)))
         self.assertEqual(mz2.rhs(), myokit.Number(4, myokit.units.meter))
 
         # Check state
         self.assertTrue(mx.is_state())
-        self.assertEqual(mx.state_value(), 0.123)
+        self.assertEqual(mx.initial_value(True), 0.123)
 
         # Check binding
         self.assertEqual(mt.binding(), 'time')
 
     def test_c2m_pass_through_variables(self):
         # Test support for variables used only to pass a value through a
         # hierarchical CellML structure.
```

### Comparing `myokit-1.33.9/myokit/tests/test_cellml_v1_parser.py` & `myokit-1.34.0/myokit/tests/test_cellml_v1_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_cellml_v1_writer.py` & `myokit-1.34.0/myokit/tests/test_cellml_v1_writer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_cellml_v2_api.py` & `myokit-1.34.0/myokit/tests/test_cellml_v2_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -905,16 +905,16 @@
         with WarningCollector() as w:
             cm.validate()
         self.assertFalse(w.has_warnings())
 
         # Recreate myokit model and test states
         mm = cm.myokit_model()
         mm.validate()
-        state_1 = m.state()
-        state_2 = mm.state()
+        state_1 = m.initial_values(True)
+        state_2 = mm.initial_values(True)
         states_1 = [x.name() for x in m.states()]
         states_2 = [x.name() for x in mm.states()]
         state_2 = [state_2[states_2.index(x)] for x in states_1]
         self.assertEqual(state_1[0], state_2[0])
         self.assertEqual(state_1[1], state_2[1])
         self.assertEqual(state_1[2], state_2[2])
         self.assertEqual(state_1[3], state_2[3])
@@ -1009,15 +1009,15 @@
         self.assertEqual(
             mz.rhs(),
             myokit.Plus(myokit.Number(3, myokit.units.volt), myokit.Name(mx)))
         self.assertEqual(mz2.rhs(), myokit.Number(4, myokit.units.meter))
 
         # Check state
         self.assertTrue(mx.is_state())
-        self.assertEqual(mx.state_value(), 0.123)
+        self.assertEqual(mx.initial_value(True), 0.123)
 
         # Check binding
         self.assertEqual(mt.binding(), 'time')
 
     def test_c2m_no_voi(self):
         # Test creating a myokit model from a model where there's no variable
         # of integration
```

### Comparing `myokit-1.33.9/myokit/tests/test_cellml_v2_parser.py` & `myokit-1.34.0/myokit/tests/test_cellml_v2_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_cellml_v2_writer.py` & `myokit-1.34.0/myokit/tests/test_cellml_v2_writer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_cmodel.py` & `myokit-1.34.0/myokit/tests/test_cmodel.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,94 +29,97 @@
 
     @classmethod
     def setUpClass(cls):
         # Test cmodel instantiation.
         m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
         cls.model = m
         cls.sensitivities = (['ik1.gK1', 'ikp.IKp'], ['cell.K_o', 'ikp.gKp'])
-        cls.cmodel = myokit.CModel(cls.model, cls.sensitivities)
+        cls.pacing_labels = {}
+        cls.cmodel = myokit.CModel(
+            cls.model, cls.pacing_labels, cls.sensitivities
+        )
 
     def test_sensitivities(self):
         # Test instantiation of cmodel with sensitivities
 
         # Bad type
         sens = 'Bad type'
         with self.assertRaisesRegex(ValueError, 'The argument `sensitivities'):
-            myokit.CModel(self.model, sens)
+            myokit.CModel(self.model, self.pacing_labels, sens)
 
         # Empty deps or indeps
         sens = ([], ['some parameter'])
-        m = myokit.CModel(self.model, sens)
+        m = myokit.CModel(self.model, self.pacing_labels, sens)
         self.assertFalse(m.has_sensitivities)
         sens = (['some state'], [])
-        m = myokit.CModel(self.model, sens)
+        m = myokit.CModel(self.model, self.pacing_labels, sens)
         self.assertFalse(m.has_sensitivities)
 
         # Provide sensitivies as Variables
         s1 = self.model.get('ik1.gK1')
         s2 = self.model.get('ikp.IKp')
         p1 = self.model.get('cell.K_o')
         p2 = self.model.get('ikp.gKp')
         sens = ([s1, s2], [p1, p2])
-        m = myokit.CModel(self.model, sens)
+        m = myokit.CModel(self.model, self.pacing_labels, sens)
         self.assertTrue(m.has_sensitivities)
 
         # Provide sensitivities as Names
         sens = (
             [myokit.Name(s1), myokit.Name(s2)],
             [myokit.Name(p1), myokit.Name(p2)])
-        m = myokit.CModel(self.model, sens)
+        m = myokit.CModel(self.model, self.pacing_labels, sens)
         self.assertTrue(m.has_sensitivities)
 
         # Sensitivity of derivative
         s3 = self.model.get('ik.x')
         sens = (
             [myokit.Derivative(myokit.Name(s3)), myokit.Name(s2)],
             [myokit.Name(p1), myokit.Name(p2)])
-        m = myokit.CModel(self.model, sens)
+        m = myokit.CModel(self.model, self.pacing_labels, sens)
         self.assertTrue(m.has_sensitivities)
         s3 = 'dot(ik.x)'
         sens = (
             [s3, myokit.Name(s2)],
             [myokit.Name(p1), myokit.Name(p2)])
-        m = myokit.CModel(self.model, sens)
+        m = myokit.CModel(self.model, self.pacing_labels, sens)
         self.assertTrue(m.has_sensitivities)
 
         # Sensitivity of derivative of non-state
         sens = (
             [myokit.Derivative(myokit.Name(s1)), myokit.Name(s2)],
             [myokit.Name(p1), myokit.Name(p2)])
         with self.assertRaisesRegex(ValueError, 'Sensitivity of '):
-            myokit.CModel(self.model, sens)
+            myokit.CModel(self.model, self.pacing_labels, sens)
 
         # Sensitivity of bound variable
         sens = (
             ['engine.time', myokit.Name(s2)],
             [myokit.Name(p1), myokit.Name(p2)])
         with self.assertRaisesRegex(ValueError, 'Sensitivities cannot'):
-            myokit.CModel(self.model, sens)
+            myokit.CModel(self.model, self.pacing_labels, sens)
 
         # Sensitivity w.r.t. Initial value
         s3 = self.model.get('ik.x')
         sens = (
             [s3, myokit.Name(s2)],
             [myokit.Name(p1), myokit.InitialValue(myokit.Name(s3))])
-        m = myokit.CModel(self.model, sens)
+        m = myokit.CModel(self.model, self.pacing_labels, sens)
         self.assertTrue(m.has_sensitivities)
 
         # Sensitivity w.r.t. initial value of non-state
         sens = (
             [myokit.Name(s1), myokit.Name(s2)],
             [myokit.Name(p1), myokit.InitialValue(myokit.Name(p2))])
         with self.assertRaisesRegex(ValueError, 'Sensitivity with respect to'):
-            myokit.CModel(self.model, sens)
+            myokit.CModel(self.model, self.pacing_labels, sens)
 
         # Sensitivity w.r.t. non-literal
         sens = (
             [myokit.Name(s1), myokit.Name(s2)],
             [myokit.Name(p1), 'ik.E'])
         with self.assertRaisesRegex(ValueError, 'Sensitivity with respect to'):
-            myokit.CModel(self.model, sens)
+            myokit.CModel(self.model, self.pacing_labels, sens)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `myokit-1.33.9/myokit/tests/test_compiler_detection.py` & `myokit-1.34.0/myokit/tests/test_compiler_detection.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_component.py` & `myokit-1.34.0/myokit/tests/test_component.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,24 +54,24 @@
         x.set_rhs(myokit.Minus(
             myokit.Multiply(myokit.Name(a), myokit.Name(x)),
             myokit.Multiply(
                 myokit.Multiply(myokit.Name(b), myokit.Name(x)),
                 myokit.Name(y)
             )
         ))
-        x.set_state_value(10)
+        x.set_initial_value(10)
         y.set_rhs(myokit.Plus(
             myokit.Multiply(
                 myokit.PrefixMinus(myokit.Name(c)), myokit.Name(y)
             ),
             myokit.Multiply(
                 myokit.Multiply(myokit.Name(d), myokit.Name(x)), myokit.Name(y)
             )
         ))
-        y.set_state_value(5)
+        y.set_initial_value(5)
         Z = m.add_component('Z')
         t = Z.add_variable('total')
         t.set_rhs(myokit.Plus(myokit.Name(x), myokit.Name(y)))
         E = m.add_component('engine')
         time = E.add_variable('time')
         time.set_rhs(0)
         time.set_binding('time')
@@ -113,114 +113,114 @@
     def test_remove_variable(self):
         # Test the removal of a variable.
 
         # Create a model
         m = myokit.Model('LotkaVolterra')
 
         # Add a variable 'a'
-        X = m.add_component('X')
+        z = m.add_component('z')
 
         # Simplest case
-        a = X.add_variable('a')
-        self.assertEqual(X.count_variables(), 1)
-        X.remove_variable(a)
-        self.assertEqual(X.count_variables(), 0)
-        self.assertRaises(Exception, X.remove_variable, a)
+        a = z.add_variable('a')
+        self.assertEqual(z.count_variables(), 1)
+        z.remove_variable(a)
+        self.assertEqual(z.count_variables(), 0)
+        self.assertRaises(Exception, z.remove_variable, a)
 
         # Test re-adding
-        a = X.add_variable('a')
+        a = z.add_variable('a')
         a.set_rhs(myokit.Number(5))
-        self.assertEqual(X.count_variables(), 1)
+        self.assertEqual(z.count_variables(), 1)
 
         # Test deleting dependent variables
-        b = X.add_variable('b')
-        self.assertEqual(X.count_variables(), 2)
+        b = z.add_variable('b')
+        self.assertEqual(z.count_variables(), 2)
         b.set_rhs(myokit.Plus(myokit.Number(3), myokit.Name(a)))
 
         # Test blocking of removal
-        self.assertRaises(myokit.IntegrityError, X.remove_variable, a)
-        self.assertEqual(X.count_variables(), 2)
+        self.assertRaises(myokit.IntegrityError, z.remove_variable, a)
+        self.assertEqual(z.count_variables(), 2)
 
         # Test removal in the right order
-        X.remove_variable(b)
-        self.assertEqual(X.count_variables(), 1)
-        X.remove_variable(a)
-        self.assertEqual(X.count_variables(), 0)
+        z.remove_variable(b)
+        self.assertEqual(z.count_variables(), 1)
+        z.remove_variable(a)
+        self.assertEqual(z.count_variables(), 0)
 
         # Test reference to current state variable values
-        a = X.add_variable('a')
+        a = z.add_variable('a')
         a.set_rhs(myokit.Number(5))
         a.promote()
-        b = X.add_variable('b')
+        b = z.add_variable('b')
         b.set_rhs(myokit.Plus(myokit.Number(3), myokit.Name(a)))
-        self.assertRaises(myokit.IntegrityError, X.remove_variable, a)
-        X.remove_variable(b)
-        X.remove_variable(a)
-        self.assertEqual(X.count_variables(), 0)
+        self.assertRaises(myokit.IntegrityError, z.remove_variable, a)
+        z.remove_variable(b)
+        z.remove_variable(a)
+        self.assertEqual(z.count_variables(), 0)
 
         # Test reference to current state variable values with "self"-ref
-        a = X.add_variable('a')
+        a = z.add_variable('a')
         a.promote()
         a.set_rhs(myokit.Name(a))
-        X.remove_variable(a)
+        z.remove_variable(a)
 
         # Test it doesn't interfere with normal workings
-        a = X.add_variable('a')
+        a = z.add_variable('a')
         a.promote()
         a.set_rhs(myokit.Name(a))
-        b = X.add_variable('b')
+        b = z.add_variable('b')
         b.set_rhs(myokit.Name(a))
-        self.assertRaises(myokit.IntegrityError, X.remove_variable, a)
-        X.remove_variable(b)
-        X.remove_variable(a)
+        self.assertRaises(myokit.IntegrityError, z.remove_variable, a)
+        z.remove_variable(b)
+        z.remove_variable(a)
 
         # Test reference to dot
-        a = X.add_variable('a')
+        a = z.add_variable('a')
         a.set_rhs(myokit.Number(5))
         a.promote()
-        b = X.add_variable('b')
+        b = z.add_variable('b')
         b.set_rhs(myokit.Derivative(myokit.Name(a)))
-        self.assertRaises(myokit.IntegrityError, X.remove_variable, a)
-        X.remove_variable(b)
-        X.remove_variable(a)
+        self.assertRaises(myokit.IntegrityError, z.remove_variable, a)
+        z.remove_variable(b)
+        z.remove_variable(a)
 
         # Test if orphaned
         self.assertIsNone(b.parent())
 
         # Test deleting variable with nested variables
-        a = X.add_variable('a')
+        a = z.add_variable('a')
         b = a.add_variable('b')
         b.set_rhs(myokit.Plus(myokit.Number(2), myokit.Number(2)))
         a.set_rhs(myokit.Multiply(myokit.Number(3), myokit.Name(b)))
-        self.assertRaises(myokit.IntegrityError, X.remove_variable, a)
+        self.assertRaises(myokit.IntegrityError, z.remove_variable, a)
         self.assertEqual(a.count_variables(), 1)
-        self.assertEqual(X.count_variables(), 1)
+        self.assertEqual(z.count_variables(), 1)
 
         # Test recursive deleting
-        X.remove_variable(a, recursive=True)
+        z.remove_variable(a, recursive=True)
         self.assertEqual(a.count_variables(), 0)
-        self.assertEqual(X.count_variables(), 0)
+        self.assertEqual(z.count_variables(), 0)
 
         # Test deleting variable with nested variables that depend on each
         # other
-        a = X.add_variable('a')
+        a = z.add_variable('a')
         b = a.add_variable('b')
         c = a.add_variable('c')
         d = a.add_variable('d')
         a.set_rhs('b + c - d')
         a.promote(0.1)
         b.set_rhs('2 * a - d')
         c.set_rhs('a + b + d')
         d.set_rhs('3 * a')
-        self.assertRaises(myokit.IntegrityError, X.remove_variable, a)
+        self.assertRaises(myokit.IntegrityError, z.remove_variable, a)
         self.assertEqual(a.count_variables(), 3)
-        self.assertEqual(X.count_variables(), 1)
-        X.remove_variable(a, recursive=True)
+        self.assertEqual(z.count_variables(), 1)
+        z.remove_variable(a, recursive=True)
         self.assertEqual(a.count_variables(), 0)
-        self.assertEqual(X.count_variables(), 0)
+        self.assertEqual(z.count_variables(), 0)
 
         # Test if removed from model's label and binding lists
         m = myokit.Model()
         c = m.add_component('c')
         x = c.add_variable('x')
         y = c.add_variable('y')
         x.set_rhs(0)
@@ -232,14 +232,76 @@
         c.remove_variable(x)
         self.assertIs(m.binding('time'), None)
         self.assertIs(m.label('membrane_potential'), y)
         c.remove_variable(y)
         self.assertIs(m.binding('time'), None)
         self.assertIs(m.label('membrane_potential'), None)
 
+        # Test variable can't be removed if used in initial expression
+        m = myokit.Model()
+        c = m.add_component('c')
+        p = c.add_variable('p')
+        p.set_rhs(2)
+        x = c.add_variable('x')
+        x.set_rhs(1)
+        x.promote('1 + c.p')
+        self.assertRaises(myokit.IntegrityError, c.remove_variable, p)
+        q = c.add_variable('q')
+        q.set_rhs(10)
+        x.set_initial_value('1 / c.q')
+        c.remove_variable(p)
+        self.assertRaises(myokit.IntegrityError, c.remove_variable, q)
+        x.set_initial_value('sqrt(2)')
+        c.remove_variable(q)
+
+        # But it's OK if we're deleting a whole component
+        m = myokit.Model()
+        c = m.add_component('c')
+        p = c.add_variable('p')
+        p.set_rhs(2)
+        x = c.add_variable('x')
+        x.set_rhs(1)
+        x.promote('1 + c.p')
+        m.remove_component('c')
+
+    def test_remove_variable_with_alias(self):
+        # Test cloning of a variable with an alias after an add / remove event.
+
+        m = myokit.Model('AddRemoveClone')
+        c = m.add_component('c')
+        p = c.add_variable('p')
+        p.set_binding('time')
+        p.set_rhs(0)
+        q = c.add_variable('q')
+        q.set_rhs(12)
+        m.validate()    # Raises error if not ok
+        m.clone()       # Raises error if not ok
+        d = m.add_component('d')
+        d.add_alias('bert', p)
+        e = d.add_variable('e')
+        e.set_rhs('10 * bert')
+        m.validate()
+        m.clone()
+        d.add_alias('ernie', q)
+        m.validate()
+        m.clone()
+        c.remove_variable(q)
+        m.validate()
+        m.clone()   # Will raise error if alias isn't deleted
+
+    def test_resolve(self):
+        # Test if an error is raised when a variable can't be resolved.
+
+        m = myokit.Model('Resolve')
+        c = m.add_component('c')
+        p = c.add_variable('p')
+        q = c.add_variable('q')
+        p.set_rhs('10 * q')
+        self.assertRaises(myokit.ParseError, q.set_rhs, '10 * r')
+
     def test_sequence_interface(self):
         # Test the sequence interface implementation
 
         model = myokit.load_model('example')
         c = model['membrane']
 
         vs = [v for v in c]
```

### Comparing `myokit-1.33.9/myokit/tests/test_config.py` & `myokit-1.34.0/myokit/tests/test_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import unittest
 
 import myokit
 
 from myokit.tests import TemporaryDirectory, WarningCollector
 
 
-debug = True
+debug = False
 
 
 # Simple test
 config_basic = """
 [myokit]
 [time]
 date_format = TEST_DATE_FORMAT
```

### Comparing `myokit-1.33.9/myokit/tests/test_datablock.py` & `myokit-1.34.0/myokit/tests/test_datablock.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_datalog.py` & `myokit-1.34.0/myokit/tests/test_datalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,16 +122,18 @@
     def test_find(self):
         # Tests the deprecated find() function
 
         d = myokit.DataLog({
             'engine.time': [0, 5, 10, 15, 20],
             'membrane.V': [0, 50, 100, 150, 200]})
         d.set_time_key('engine.time')
-        with WarningCollector():
+        with WarningCollector() as w:
             self.assertEqual(d.find(-5), d.find_after(-5))
+        self.assertIn('eprecated', w.text())
+        with WarningCollector():
             self.assertEqual(d.find(0), d.find_after(0))
             self.assertEqual(d.find(2), d.find_after(2))
             self.assertEqual(d.find(5), d.find_after(5))
             self.assertEqual(d.find(7), d.find_after(7))
             self.assertEqual(d.find(20), d.find_after(20))
             self.assertEqual(d.find(22), d.find_after(22))
 
@@ -2177,20 +2179,30 @@
         self.assertEqual(d.length(), 0)
         d['time'] = list(np.arange(100) * 3)
         self.assertEqual(d.length(), 100)
         d['x'] = list(np.arange(100) * 3)
         self.assertEqual(d.length(), 100)
 
     def test_regularize(self):
-        # Test the regularize() method.
+        # Test the deprecated regularize() method.
 
         d = myokit.DataLog(time='time')
         d['time'] = np.log(np.linspace(1, 25, 100))
         d['values'] = np.linspace(1, 25, 100)
-        e = d.regularize(dt=0.5)
+
+        has_scipy = True
+        with WarningCollector() as w:
+            try:
+                e = d.regularize(dt=0.5)
+            except ImportError:
+                has_scipy = False
+        self.assertIn('eprecated', w.text())
+        if not has_scipy:
+            return
+
         self.assertEqual(len(e['time']), 7)
         x = np.array([0, 0.5, 1, 1.5, 2, 2.5, 3])
         self.assertTrue(np.all(e['time'] == x))
         for i, y in enumerate(x):
             self.assertTrue(np.abs(np.exp(y) - e['values'][i]) < 0.02)
 
         # test setting tmin and tmax
```

### Comparing `myokit-1.33.9/myokit/tests/test_dependency_checking.py` & `myokit-1.34.0/myokit/tests/test_dependency_checking.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_expressions.py` & `myokit-1.34.0/myokit/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_float.py` & `myokit-1.34.0/myokit/tests/test_float.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_formats.py` & `myokit-1.34.0/myokit/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_formats_axon.py` & `myokit-1.34.0/myokit/tests/test_formats_axon.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_formats_cellml.py` & `myokit-1.34.0/myokit/tests/test_formats_cellml.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_formats_channelml.py` & `myokit-1.34.0/myokit/tests/test_formats_channelml.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_formats_easyml.py` & `myokit-1.34.0/myokit/tests/test_formats_easyml.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_formats_exporters.py` & `myokit-1.34.0/myokit/tests/test_formats_exporters.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_formats_expression_writers.py` & `myokit-1.34.0/myokit/tests/test_formats_expression_writers.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_formats_html.py` & `myokit-1.34.0/myokit/tests/test_formats_html.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_formats_importers.py` & `myokit-1.34.0/myokit/tests/test_formats_importers.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_formats_mathml_content.py` & `myokit-1.34.0/myokit/tests/test_formats_mathml_content.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_formats_mathml_presentation.py` & `myokit-1.34.0/myokit/tests/test_formats_mathml_presentation.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_formats_opencl.py` & `myokit-1.34.0/myokit/tests/test_formats_opencl.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_formats_sbml.py` & `myokit-1.34.0/myokit/tests/test_formats_sbml.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_formats_sympy.py` & `myokit-1.34.0/myokit/tests/test_formats_sympy.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_formats_wcp.py` & `myokit-1.34.0/myokit/tests/test_formats_wcp.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_io.py` & `myokit-1.34.0/myokit/tests/test_io.py`

 * *Files 8% similar despite different names*

```diff
@@ -251,14 +251,20 @@
         with TemporaryDirectory() as d:
             opath = d.path('test.mmt')
             myokit.save(opath, model=m, protocol=p, script=x)
             with open(opath, 'r') as f:
                 text = f.read()
             self.assertEqual(text, myokit.save(model=m, protocol=p, script=x))
 
+        # Save nothing
+        with TemporaryDirectory() as d:
+            opath = d.path('test.mmt')
+            self.assertRaises(ValueError, myokit.save, opath)
+            self.assertFalse(os.path.exists(opath))
+
     def test_save_model(self):
         # Test if the correct parts are saved/loaded from disk using the
         # ``save_model()`` method.
 
         ipath = os.path.join(DIR_DATA, 'lr-1991.mmt')
         # Test example loading
         m = myokit.load_model('example')
@@ -336,43 +342,45 @@
 
     def test_load_save_state(self):
         # Test loading/saving state.
         m, p, x = myokit.load('example')
         with TemporaryDirectory() as d:
             # Test save and load without model
             f = d.path('state.txt')
-            myokit.save_state(f, m.state())
-            self.assertEqual(myokit.load_state(f), m.state())
+            myokit.save_state(f, m.initial_values(True))
+            self.assertEqual(myokit.load_state(f), m.initial_values(True))
 
             # Test save and load with model argument
-            myokit.save_state(f, m.state(), m)
-            self.assertEqual(myokit.load_state(f, m), m.state())
+            myokit.save_state(f, m.initial_values(True), m)
+            self.assertEqual(myokit.load_state(f, m), m.initial_values(True))
 
             # Save without, load with model
-            myokit.save_state(f, m.state())
-            self.assertEqual(myokit.load_state(f, m), m.state())
+            myokit.save_state(f, m.initial_values(True))
+            self.assertEqual(myokit.load_state(f, m), m.initial_values(True))
 
             # Save with model, load without
             # Loaded version is dict!
-            myokit.save_state(f, m.state(), m)
-            dct = dict(zip([v.qname() for v in m.states()], m.state()))
-            self.assertEqual(myokit.load_state(f), dct)
+            myokit.save_state(f, m.initial_values(True), m)
+            self.assertEqual(myokit.load_state(f), dict(zip(
+                [v.qname() for v in m.states()], m.initial_values(True))))
 
     def test_load_save_state_bin(self):
         # Test loading/saving state in binary format.
         m, p, x = myokit.load('example')
         with TemporaryDirectory() as d:
 
             # Test save and load with double precision
             f = d.path('state.bin')
-            myokit.save_state_bin(f, m.state())
-            self.assertEqual(myokit.load_state_bin(f), m.state())
+            myokit.save_state_bin(f, m.initial_values(True))
+            self.assertEqual(myokit.load_state_bin(f), m.initial_values(True))
 
             # Test save and load with single precision
             f = d.path('state.bin')
-            myokit.save_state_bin(f, m.state(), myokit.SINGLE_PRECISION)
-            d = np.array(myokit.load_state_bin(f)) - np.array(m.state())
+            myokit.save_state_bin(
+                f, m.initial_values(True), myokit.SINGLE_PRECISION)
+            d = np.array(myokit.load_state_bin(f))
+            d -= np.array(m.initial_values(True))
             self.assertTrue(np.all(np.abs(d) < 1e-5))   # Not very precise!
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `myokit-1.33.9/myokit/tests/test_jacobian_calculator.py` & `myokit-1.34.0/myokit/tests/test_jacobian_calculator.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,41 +33,41 @@
 
         # Run a simple simulation
         c = myokit.JacobianCalculator(m)
         x, f, j, e = c.newton_root(damping=0.01, max_iter=50)
 
         # Test if still runs with initial x all zero
         # (But does cause a linear algebra issue in this case)
-        x = np.zeros(len(m.state()))
+        x = np.zeros(m.count_states())
         c.newton_root(x, damping=0.01, max_iter=50)
 
         # Test if still works with a single zero (Enno's bug)
-        x = np.array(m.state())
+        x = np.array(m.initial_values(True))
         x[1] = 0
         x, f, j, e = c.newton_root(x, damping=0.01, max_iter=50)
 
         # Test quick return
-        x = np.array(m.state())
+        x = np.array(m.initial_values(True))
         x[0] = 0
         x2, f, j, e = c.newton_root(damping=0.01, max_iter=1)
         self.assertTrue(np.sum((x2 - x)**2) > 10)
 
         # Invalid damping value
         self.assertRaisesRegex(
             ValueError, 'Damping', c.newton_root, damping=0)
         self.assertRaisesRegex(
             ValueError, 'Damping', c.newton_root, damping=1.1)
 
         # Missing a state
-        x = m.state()[:-1]
+        x = m.initial_values(True)[:-1]
         self.assertRaisesRegex(
             ValueError, 'must have length', c.calculate, x)
 
         # Non-numbers in state
-        x = m.state()
+        x = m.initial_values(True)
         x[0] = 'Hello'
         self.assertRaisesRegex(
             ValueError, 'floats', c.calculate, x)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `myokit-1.33.9/myokit/tests/test_jacobian_tracer.py` & `myokit-1.34.0/myokit/tests/test_jacobian_tracer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_lib_deps.py` & `myokit-1.34.0/myokit/tests/test_lib_deps.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_lib_guess.py` & `myokit-1.34.0/myokit/tests/test_lib_guess.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_lib_hh.py` & `myokit-1.34.0/myokit/tests/test_lib_hh.py`

 * *Files 2% similar despite different names*

```diff
@@ -361,21 +361,21 @@
         ikr = m2.get('ikr')
         dt = ikr.add_variable('dt')
         dt.set_rhs(1e-6)
         # Test for a
         a = m2.get('ikr.a')
         rl = hh.get_rl_expression(a, myokit.Name(dt))
         a1 = rl.eval()
-        a2 = a.state_value() + dt.eval() * a.rhs().eval()
+        a2 = a.initial_value(True) + dt.eval() * a.rhs().eval()
         self.assertAlmostEqual(a1, a2)
         # And for r
         r = m2.get('ikr.r')
         rl = hh.get_rl_expression(r, myokit.Name(dt))
         r1 = rl.eval()
-        r2 = r.state_value() + dt.eval() * r.rhs().eval()
+        r2 = r.initial_value(True) + dt.eval() * r.rhs().eval()
         self.assertAlmostEqual(r1, r2)
 
         # Dt must be an expression
         self.assertRaisesRegex(
             ValueError, 'must be a myokit.Expression',
             hh.get_rl_expression, a, 'dt')
 
@@ -604,15 +604,15 @@
         # Check that this is a valid steady state
         self.assertTrue(np.all(ss >= 0))
         self.assertTrue(np.all(ss <= 1))
 
         # Test if derivatives are zero
         for k, x in enumerate(['ina.m', 'ina.h', 'ina.j']):
             x = model.get(x)
-            x.set_state_value(ss[k])
+            x.set_initial_value(ss[k])
             self.assertAlmostEqual(x.eval(), 0)
 
         # Test arguments
         m.steady_state(-20, m.default_parameters())
         self.assertRaisesRegex(
             ValueError, 'parameter vector size',
             m.steady_state, -20, [1])
@@ -641,14 +641,28 @@
         # Test with the v-independent states
 
         model = myokit.parse_model(MODEL)
         m = hh.HHModel.from_component(model.get('binding'))
 
         self.assertEqual(len(m.states()), 3)
 
+    def test_initial_value_conversion(self):
+        # Tests that initial value expressions are converted to floats
+
+        model = myokit.parse_model(MODEL)
+        model.get('ikr.a').set_initial_value('1 / sqrt(7)')
+        model.get('ikr.r').set_initial_value('log(binding.koff, 10)')
+        m = hh.HHModel.from_component(model.get('ikr'))
+        x0 = m.default_state()
+        self.assertEqual(len(x0), 2)
+        self.assertIsInstance(x0[0], float)
+        self.assertIsInstance(x0[1], float)
+        self.assertAlmostEqual(x0[0], 0.377964473)
+        self.assertAlmostEqual(x0[1], -5)
+
 
 class AnalyticalSimulationTest(unittest.TestCase):
     """
     Tests :class:`myokit.lib.hh.AnalyticalSimulation`.
     """
 
     def test_create_and_run(self):
```

### Comparing `myokit-1.33.9/myokit/tests/test_lib_markov.py` & `myokit-1.34.0/myokit/tests/test_lib_markov.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,16 +151,16 @@
         x.set_rhs(str(x.rhs()) + ' - ina.C1')
         self.assertRaisesRegex(
             markov.LinearModelError, 'not vice versa',
             markov.LinearModel, m2, states, parameters, current)
 
         # States must sum to 1
         m2 = model.clone()
-        m2.get(states[0]).set_state_value(0.6)
-        m2.get(states[1]).set_state_value(0.6)
+        m2.get(states[0]).set_initial_value(0.6)
+        m2.get(states[1]).set_initial_value(0.6)
         self.assertRaisesRegex(
             markov.LinearModelError, 'sum of states',
             markov.LinearModel, m2, states, parameters, current)
 
         # Derivatives per column don't sum to zero
         m2 = model.clone()
         x = m2.get(states[0])
@@ -279,15 +279,15 @@
 
         # Check that this is a valid steady state
         self.assertTrue(np.all(ss >= 0))
         self.assertTrue(np.all(ss <= 1))
 
         # Check that derivatives with ss are close to zero
         ss = list(ss)
-        model.set_state(ss + ss)    # Model has 2 ina's
+        model.set_initial_values(ss + ss)    # Model has 2 ina's
         derivs = model.evaluate_derivatives()
         for i in range(len(ss)):
             self.assertAlmostEqual(0, derivs[i])
 
         # Try with awful parameters
         self.assertRaisesRegex(
             markov.LinearModelError, 'positive eigenvalues',
@@ -306,15 +306,15 @@
         ss = np.array(m.steady_state())
 
         # Check that this is a valid steady state
         self.assertTrue(np.all(ss >= 0))
         self.assertTrue(np.all(ss <= 1))
 
         # Check that derivatives with ss are close to zero
-        model.set_state(ss)
+        model.set_initial_values(ss)
         derivs = model.evaluate_derivatives()
         for i in range(len(ss)):
             self.assertAlmostEqual(0, derivs[i])
 
     def test_rates(self):
 
         # Load model
@@ -327,14 +327,30 @@
         # Test rates method runs
         self.assertEqual(len(m.rates()), 12)
         m.rates(parameters=[0.01] * 21)
         self.assertRaisesRegex(
             ValueError, 'Illegal parameter vector size',
             m.rates, parameters=[0.01] * 22)
 
+    def test_initial_value_conversion(self):
+        # Tests that initial value expressions are converted to floats
+
+        fname = os.path.join(DIR_DATA, 'clancy-1999-fitting.mmt')
+        model = myokit.load_model(fname)
+        model.get('ina.C3').set_initial_value('1 / sqrt(7)')
+        model.get('ina.C2').set_initial_value('-1 / log(ina_ref.p)')
+        model.get('ina.C1').set_initial_value(0.5134619065149598)
+        m = markov.LinearModel.from_component(model.get('ina'))
+        x0 = m.default_state()
+        self.assertEqual(len(x0), 6)
+        self.assertIsInstance(x0[0], float)
+        self.assertIsInstance(x0[1], float)
+        self.assertAlmostEqual(x0[0], 0.3779644730092272)
+        self.assertAlmostEqual(x0[1], 0.10857362047581297)
+
 
 class AnalyticalSimulationTest(unittest.TestCase):
     """
     Tests :class:`myokit.lib.markov.AnalyticalSimulation`.
     """
 
     def test_create_and_run(self):
```

### Comparing `myokit-1.33.9/myokit/tests/test_lib_multi.py` & `myokit-1.34.0/myokit/tests/test_lib_multi.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_lib_plots.py` & `myokit-1.34.0/myokit/tests/test_lib_plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import os
 import unittest
 
 import myokit
 import myokit.lib.plots as plots
 
-from myokit.tests import DIR_DATA
+from myokit.tests import DIR_DATA, WarningCollector
 
 
 class LibPlotTest(unittest.TestCase):
     """
     Tests if the myokit.lib.plots module runs without exceptions, doesn't
     inspect the output.
     """
@@ -172,24 +172,32 @@
         # Integrate currents to charges
         fig = plt.figure()
         plots.cumulative_current(d, currents, integrate=True)
         plt.legend()
         plt.close(fig)
         plt.show()
 
-        # Normalise currents
+        # Normalize currents
         fig = plt.figure()
-        plots.cumulative_current(d, currents, normalise=True)
+        plots.cumulative_current(d, currents, normalize=True)
         plt.legend()
         plt.close(fig)
         plt.show()
 
-        # Normalise currents and set maximum number of currents shown
+        # Normalize currents and set maximum number of currents shown
         fig = plt.figure()
-        plots.cumulative_current(d, currents, normalise=True, max_currents=3)
+        plots.cumulative_current(d, currents, normalize=True, max_currents=3)
         plt.legend()
         plt.close(fig)
         plt.show()
 
+        with WarningCollector() as w:
+            fig = plt.figure()
+            plots.cumulative_current(d, currents, normalise=True)
+            plt.legend()
+            plt.close(fig)
+            plt.show()
+        self.assertIn('deprecated', w.text())
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `myokit-1.33.9/myokit/tests/test_meta.py` & `myokit-1.34.0/myokit/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_model.py` & `myokit-1.34.0/myokit/tests/test_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -297,14 +297,34 @@
         m2 = m1.clone()
         self.assertTrue(m1.is_similar(m2, True))
 
         # Test tokens are not cloned
         self.assertTrue(m1.has_parse_info())
         self.assertFalse(m2.has_parse_info())
 
+        # Test initial value expressions are maintained
+        m1 = myokit.Model('moo')
+        component = m1.add_component('c')
+        p = component.add_variable('p')
+        q = component.add_variable('q')
+        r = component.add_variable('r')
+        s = component.add_variable('s')
+        z = component.add_variable('z')
+        z.set_rhs(123)
+        p.promote(1)
+        q.promote('1 + exp(3)')
+        r.promote('c.z')
+        s.promote('1 [g] + c.z / 2 [1/g]')
+        m2 = m1.clone()
+        self.assertEqual(m2.get('c.p').initial_value(), myokit.Number(1))
+        self.assertEqual(m2.get('c.q').initial_value().code(), '1 + exp(3)')
+        self.assertEqual(m2.get('c.r').initial_value(), m2.get('c.z').lhs())
+        self.assertEqual(m2.get('c.s').initial_value().code(),
+                         '1 [g] + c.z / 2 [1/g]')
+
     def test_code(self):
         # Test :meth:`Model.code()`.
 
         model = myokit.Model('m')
         component = model.add_component('comp1')
         a = component.add_variable('a')
         b = component.add_variable('b')
@@ -351,52 +371,49 @@
             ' 9 c = a * b\n'
             '10     in [J]\n'
             '11 \n'
             '12 [comp2]\n'
             '13 d = comp1.a\n'
         )
 
-    def test_is_similar(self):
-        # Check that equality takes both code() and unames into account
-
-        # Test without custom reserved names
-        m1 = myokit.load_model('example')
-        m2 = m1.clone()
-        self.assertIsInstance(m2, myokit.Model)
-        self.assertFalse(m1 is m2)
-        self.assertNotEqual(m1, m2)
-        self.assertNotEqual(m2, m1)
-        self.assertTrue(m1.is_similar(m2, False))
-        self.assertTrue(m1.is_similar(m2, True))
-        self.assertTrue(m2.is_similar(m1, False))
-        self.assertTrue(m2.is_similar(m1, True))
-        self.assertTrue(m1.is_similar(m1, True))
-        self.assertTrue(m2.is_similar(m2, False))
-
-        # Test with none-model
-        self.assertFalse(m1.is_similar(None))
-        self.assertFalse(m1.is_similar(m1.code()))
-
-        # Add reserved names
-        m1.reserve_unique_names('bertie')
-        self.assertFalse(m1.is_similar(m2))
-        m1.reserve_unique_names('clair')
-        self.assertFalse(m1.is_similar(m2))
-        m2.reserve_unique_names('clair', 'bertie')
-        self.assertTrue(m1.is_similar(m2))
-
-        # Add reserved name prefixes
-        m1.reserve_unique_name_prefix('aa', 'bb')
-        m1.reserve_unique_name_prefix('cc', 'dd')
-        self.assertFalse(m1.is_similar(m2))
-        m2.reserve_unique_name_prefix('aa', 'bb')
-        m2.reserve_unique_name_prefix('cc', 'ee')
-        self.assertFalse(m1.is_similar(m2))
-        m2.reserve_unique_name_prefix('cc', 'dd')
-        self.assertTrue(m1.is_similar(m2))
+        # Test initial value expressions are maintained
+        model = myokit.Model('moo')
+        component = model.add_component('c')
+        p = component.add_variable('p')
+        q = component.add_variable('q')
+        r = component.add_variable('r')
+        s = component.add_variable('s')
+        z = component.add_variable('z')
+        z.set_rhs(123)
+        p.promote(1)
+        q.promote('1 + exp(3)')
+        r.promote('c.z')
+        s.promote('1 [g] + c.z / 2 [1/g]')
+
+        p.set_rhs(1)
+        q.set_rhs(2)
+        r.set_rhs(3)
+        s.set_rhs('4 [g/s]')
+
+        self.assertEqual(model.code(line_numbers=False), '\n'.join([
+            '[[model]]',
+            'name: moo',
+            '# Initial values',
+            'c.p = 1',
+            'c.q = 1 + exp(3)',
+            'c.r = c.z',
+            'c.s = 1 [g] + c.z / 2 [1/g]',
+            '',
+            '[c]',
+            'dot(p) = 1',
+            'dot(q) = 2',
+            'dot(r) = 3',
+            'dot(s) = 4 [g/s]',
+            'z = 123\n\n',
+        ]))
 
     def test_evaluate_derivatives(self):
         # Test Model.evaluate_derivatives().
         model = myokit.Model('m')
         component = model.add_component('comp1')
         t = component.add_variable('time')
         t.set_binding('time')
@@ -490,15 +507,15 @@
             'ica.f      = 6\n'
             'ik.x       = 7\n'
             'ica.Ca_i   = 8'
         )
 
         # Test with invalid state argument
         self.assertRaisesRegex(
-            ValueError, r'list of \(8\)', m.format_state, [1, 2, 3])
+            ValueError, r'sequence of \(8\)', m.format_state, [1, 2, 3])
 
         # Test with precision argument
         state1 = [1, 2, 3, 4, 5, 6, 7, 8]
         state1[3] = 124.35624574537437
         self.assertEqual(
             m.format_state(state1, precision=myokit.SINGLE_PRECISION),
             'membrane.V = 1\n'
@@ -522,17 +539,34 @@
             'ica.f      = 6    3\n'
             'ik.x       = 7    2\n'
             'ica.Ca_i   = 8    1'
         )
 
         # Test with invalid second state argument
         self.assertRaisesRegex(
-            ValueError, r'list of \(8\)', m.format_state,
+            ValueError, r'sequence of \(8\)', m.format_state,
             [1, 2, 3, 4, 5, 6, 7, 8], [1, 2, 3])
 
+        # Test with model that has expressions in its initial state.
+        # These will be evaluated (the method handles states, not initial state
+        # expressions).
+        m.get('ina.m').set_initial_value('sqrt(4) / 4')
+        m.get('ina.h').set_initial_value('ina.gNa / 20')
+        self.assertEqual(
+            m.format_state(),
+            'membrane.V = -84.5286\n'
+            'ina.m      = 0.5\n'
+            'ina.h      = 0.8\n'
+            'ina.j      = 0.995484\n'
+            'ica.d      = 3e-06\n'
+            'ica.f      = 1.0\n'
+            'ik.x       = 0.0057\n'
+            'ica.Ca_i   = 0.0002'
+        )
+
     def test_format_state_derivatives(self):
         # Test Model.format_state_derivatives().
 
         self.maxDiff = None
         m = myokit.load_model('example')
 
         # For whatever reason, CI gives slightly different final digits some
@@ -581,15 +615,15 @@
         ]
         for a, b in zip(x, y):
             self.assertTrue(almost_equal(a, b))
         self.assertEqual(len(x), len(y))
 
         # Test with invalid state argument
         self.assertRaisesRegex(
-            ValueError, r'list of \(8\)',
+            ValueError, r'sequence of \(8\)',
             m.format_state_derivatives, [1, 2, 3])
 
         # Test with state and precision argument
         # Ignoring some of the middle digits, as they differ on some (but not
         # all!) CI builds.
         out = m.format_state_derivatives(
             state1, precision=myokit.SINGLE_PRECISION).splitlines()
@@ -632,17 +666,36 @@
             'ica.f      = 6                          dot = 3\n'
             'ik.x       = 7                          dot = 2\n'
             'ica.Ca_i   = 8                          dot = 1'
         )
 
         # Test with invalid derivs argument
         self.assertRaisesRegex(
-            ValueError, r'list of \(8\)', m.format_state_derivatives,
+            ValueError, r'sequence of \(8\)', m.format_state_derivatives,
             [1, 2, 3, 4, 5, 6, 7, 8], [1, 2, 3])
 
+        # Test without expressions in the initial state (these will be
+        # evaluated)
+        m.get('ina.m').set_initial_value('sqrt(0.25)')
+        m.get('ina.h').set_initial_value('ina.gNa / 20')
+        x = m.format_state_derivatives().splitlines()
+        y = [
+'membrane.V = -84.5286                   dot =  2.46843981754470434e+02', # noqa
+'ina.m      = 0.5                        dot = -8.68225658924664856e+01', # noqa
+'ina.h      = 0.8                        dot =  4.89677127030544446e-02', # noqa
+'ina.j      = 0.995484                   dot = -3.70409866928434243e-04', # noqa
+'ica.d      = 3e-06                      dot =  3.68067721821794798e-04', # noqa
+'ica.f      = 1.0                        dot = -3.55010150519739432e-07', # noqa
+'ik.x       = 0.0057                     dot = -2.04613933160084307e-07', # noqa
+'ica.Ca_i   = 0.0002                     dot = -6.99430692442154227e-06'  # noqa
+        ]
+        for a, b in zip(x, y):
+            self.assertTrue(almost_equal(a, b))
+        self.assertEqual(len(x), len(y))
+
     def test_get(self):
         # Test Model.get().
 
         m = myokit.load_model('example')
 
         # Get by name
         v = m.get('membrane.V')
@@ -721,18 +774,20 @@
 
     def test_import_component(self):
         # Test :meth: 'import_component()'.
 
         # Source model, to import stuff from
         ms = myokit.parse_model('''
             [[model]]
+            n.c = 1 + n.p
+            n.b = sqrt(0.25)
             p.b = 0.2
             q.e = 0.2
-            x.a = 0.2
             y.e = 0.2
+            x.a = 0.2
 
             [e]
             t = 0 [s] bind time
                 in [s]
             g = 0
                 label this_is_g
             h = 4
@@ -774,22 +829,28 @@
             [y]
             use x.d
             dot(e) = d * sub_e
                 in [m]
                 sub_e = 2 * e
                     in [m]
 
-            # another group component but this isn't independant
+            # Another group component but this isn't independent
             [z]
             use x.d
             use y.e
             use e.h
-
             f = d * e * h
                 in [m/s]
+
+            # A component with expressions in initial states
+            [n]
+            a = 1
+            dot(b) = 1 [1/s]
+            dot(c) = 2 [1/s]
+            p = 0.1
         ''')
         ms.validate()
         ms.check_units(myokit.UNIT_STRICT)
 
         # Make copy of ms, to ensure nothing is altered in original model
         ms_unaltered = ms.clone()
 
@@ -912,25 +973,58 @@
         self.assertTrue(m1.has_component('x'))
         self.assertTrue(m1.has_component('y'))
         self.assertFalse(m1['x'] is ms['x'])
         self.assertFalse(m1['y'] is ms['y'])
         self.assertEqual(m1['x'].code(), ms['x'].code())
         self.assertEqual(m1['y'].code(), ms['y'].code())
         self.assertTrue(ms.is_similar(ms_unaltered, True))
+        # Check that state order is preserved
+        self.assertLess(m1.get('y.e').index(), m1.get('x.a').index())
+
+        # Import multiple components and rename
+        component_list = [ms['x'], ms['y']]
+        m1.import_component(component_list, new_name=['xx', 'yy'])
+        self.assertTrue(m1.has_component('xx'))
+        self.assertTrue(m1.has_component('yy'))
+        self.assertFalse(m1['xx'] is ms['x'])
+        self.assertFalse(m1['yy'] is ms['y'])
+        self.assertTrue(ms.is_similar(ms_unaltered, True))
+        # Check that state order is preserved
+        self.assertLess(m1.get('yy.e').index(), m1.get('xx.a').index())
 
         # Import 1 component in list
         m1.import_component([ms['p']], new_name='p3')
         self.assertTrue(m1.has_component('p3'))
         self.assertFalse(m1['p3'] is ms['p'])
         self.assertFalse(m1['p3'] is m1['p'])
         cs = '\n'.join((ms['p'].code().splitlines())[1:])
         c1 = '\n'.join((m1['p3'].code().splitlines())[1:])
         self.assertEqual(cs, c1)
         self.assertTrue(ms.is_similar(ms_unaltered, True))
 
+        # Import state variables with expressions in their initial values
+        m1_unaltered = m1.clone()
+        m1.import_component(ms['n'])
+        self.assertEqual(m1.get('n.b').initial_value().code(), 'sqrt(0.25)')
+        self.assertEqual(
+            m1.get('n.c').initial_value(),
+            myokit.Plus(myokit.Number(1), myokit.Name(m1.get('n.p'))))
+        # Check that state order is preserved
+        self.assertLess(m1.get('n.c').index(), m1.get('n.b').index())
+        m1 = m1_unaltered
+
+        # ...including references to parameters in other components
+        ms2 = ms.clone()
+        ms2.get('n.c').set_initial_value('1 + e.h')
+        ms2_unaltered = ms2.clone()
+        self.assertRaises(
+            myokit.VariableMappingError, m1.import_component, ms2['n'])
+        self.assertTrue(m1.is_similar(m1_unaltered, True))
+        self.assertTrue(ms2.is_similar(ms2_unaltered, True))
+
         # Try and fail to import r without a mapping
         m1_unaltered = m1.clone()
         self.assertRaises(
             myokit.VariableMappingError,
             m1.import_component, ms['q'], new_name='q9')
         self.assertTrue(m1.is_similar(m1_unaltered, True))
         self.assertTrue(ms.is_similar(ms_unaltered, True))
@@ -1150,33 +1244,33 @@
         self.assertTrue(ms.is_similar(ms_unaltered, True))
         self.assertIn('r', m1)
         self.assertEqual(len(m1['r']), 1)
         self.assertIn('f', m1['r'])
         self.assertTrue(m1.get('r.f').is_state())
         self.assertEqual(m1.get('r.f').unit(), ms.get('r.f').unit())
         self.assertEqual(
-            m1.get('r.f').state_value(), ms.get('r.f').state_value())
+            m1.get('r.f').initial_value(), ms.get('r.f').initial_value())
         self.assertEqual(
             m1.get('r.f').rhs().code(),
             myokit.Multiply(ms.get('r.f').rhs(), s2ms).code())
 
         # Import multiple components
         m1.import_component([ms['x'], ms['y']], convert_units=True)
         self.assertTrue(m1.has_component('x'))
         self.assertTrue(m1.has_component('y'))
         self.assertFalse(m1['x'] is ms['x'])
         self.assertFalse(m1['y'] is ms['y'])
         self.assertEqual(m1.get('x.a').unit(), ms.get('x.a').unit())
         self.assertEqual(
-            m1.get('x.a').state_value(), ms.get('x.a').state_value())
+            m1.get('x.a').initial_value(), ms.get('x.a').initial_value())
         self.assertEqual(
             m1.get('x.a').rhs().code(),
             myokit.Multiply(ms.get('x.a').rhs(), s2ms).code())
         self.assertEqual(
-            m1.get('y.e').state_value(), ms.get('y.e').state_value())
+            m1.get('y.e').initial_value(), ms.get('y.e').initial_value())
         self.assertEqual(
             m1.get('y.e').rhs().code(),
             myokit.Multiply(ms.get('y.e').rhs(), s2ms).code())
 
         # Target model with different space units
         m1 = myokit.parse_model('''
             [[model]]
@@ -1312,14 +1406,121 @@
         m1.check_units(myokit.UNIT_STRICT)
         vm = {'p.a': 'p.a', 'p.b': 'p.b', 'p.c': 'p.c'}
         self.assertRaisesRegex(
             myokit.VariableMappingError, 'Unable to convert',
             m1.import_component, ms['q'], var_map=vm, convert_units=True)
         self.assertTrue(ms.is_similar(ms_unaltered, True))
 
+    def test_initial_values(self):
+        # Tests :meth:`Model.initial_values`.
+
+        m = myokit.parse_model('''
+            [[model]]
+            c.x = 2
+            c.y = 1 + 2
+            c.z = 2 * c.p
+
+            [c]
+            t = 0 bind time
+            dot(x) = 0
+            dot(y) = 0
+            dot(z) = 0
+            p = 3
+            q = 4
+        ''')
+
+        # Test expression version
+        p = m.get('c.p')
+        x0 = m.initial_values()
+        self.assertEqual(x0[0], myokit.Number(2))
+        self.assertEqual(
+            x0[1], myokit.Plus(myokit.Number(1), myokit.Number(2)))
+        self.assertEqual(x0[2], myokit.Multiply(myokit.Number(2), p.lhs()))
+
+        # Test float version
+        self.assertEqual(m.initial_values(True), [2, 3, 6])
+
+        # Test deprecated alias
+        with WarningCollector() as w:
+            self.assertEqual(m.state(), m.initial_values(True))
+        self.assertIn('deprecated', w.text())
+
+        # Test cycles are detected before evaluation
+        p.set_rhs('1 / q')
+        m.get('c.q').set_rhs('1 + p')
+        m.initial_values()  # No evaluation, so no error
+        self.assertRaises(
+            myokit.CyclicalDependencyError, m.initial_values, as_floats=True)
+
+    def test_inits(self):
+        # Tests :meth:`Model.inits`
+
+        m = myokit.parse_model('''
+            [[model]]
+            c.x = 2
+            c.y = 1 + 2
+            c.z = 2 * c.p
+
+            [c]
+            t = 0 bind time
+            dot(x) = 0
+            dot(y) = 0
+            dot(z) = 0
+            p = 3
+        ''')
+        with WarningCollector() as w:
+            eqs = m.inits()
+        self.assertIn('deprecated', w.text())
+
+        E, N, M = myokit.Equation, myokit.Number, myokit.Multiply
+        self.assertEqual(list(eqs), [
+            E(myokit.Name(m.get('c.x')), N(2)),
+            E(myokit.Name(m.get('c.y')), myokit.Plus(N(1), N(2))),
+            E(myokit.Name(m.get('c.z')), M(N(2), m.get('c.p').lhs()))
+        ])
+
+    def test_is_similar(self):
+        # Check that equality takes both code() and unames into account
+
+        # Test without custom reserved names
+        m1 = myokit.load_model('example')
+        m2 = m1.clone()
+        self.assertIsInstance(m2, myokit.Model)
+        self.assertFalse(m1 is m2)
+        self.assertNotEqual(m1, m2)
+        self.assertNotEqual(m2, m1)
+        self.assertTrue(m1.is_similar(m2, False))
+        self.assertTrue(m1.is_similar(m2, True))
+        self.assertTrue(m2.is_similar(m1, False))
+        self.assertTrue(m2.is_similar(m1, True))
+        self.assertTrue(m1.is_similar(m1, True))
+        self.assertTrue(m2.is_similar(m2, False))
+
+        # Test with none-model
+        self.assertFalse(m1.is_similar(None))
+        self.assertFalse(m1.is_similar(m1.code()))
+
+        # Add reserved names
+        m1.reserve_unique_names('bertie')
+        self.assertFalse(m1.is_similar(m2))
+        m1.reserve_unique_names('clair')
+        self.assertFalse(m1.is_similar(m2))
+        m2.reserve_unique_names('clair', 'bertie')
+        self.assertTrue(m1.is_similar(m2))
+
+        # Add reserved name prefixes
+        m1.reserve_unique_name_prefix('aa', 'bb')
+        m1.reserve_unique_name_prefix('cc', 'dd')
+        self.assertFalse(m1.is_similar(m2))
+        m2.reserve_unique_name_prefix('aa', 'bb')
+        m2.reserve_unique_name_prefix('cc', 'ee')
+        self.assertFalse(m1.is_similar(m2))
+        m2.reserve_unique_name_prefix('cc', 'dd')
+        self.assertTrue(m1.is_similar(m2))
+
     def test_item_at_text_position(self):
         # Test :meth:`Model.item_at_text_position()`.
 
         text = [
             '[[model]]',        # 1
             'c.x = 0',          # 2
             '',                 # 3
@@ -1450,25 +1651,29 @@
             myokit.InvalidLabelError, 'in use as a binding', w.set_label,
             'time')
 
     def test_load_save_state(self):
         # Test :meth:`Model.save_state()` and :meth:`Model.load_state()`.
 
         m = myokit.load_model('example')
-        s1 = m.state()
+        s1 = m.initial_values(True)
         with TemporaryDirectory() as d:
             path = d.path('state.csv')
-            m.save_state(path)
-            self.assertEqual(m.state(), s1)
+            with WarningCollector() as w:
+                m.save_state(path)
+            self.assertIn('deprecated', w.text())
+            self.assertEqual(m.initial_values(True), s1)
             sx = list(s1)
             sx[0] = 10
-            m.set_state(sx)
-            self.assertNotEqual(m.state(), s1)
-            m.load_state(path)
-            self.assertEqual(m.state(), s1)
+            m.set_initial_values(sx)
+            self.assertNotEqual(m.initial_values(True), s1)
+            with WarningCollector() as w:
+                m.load_state(path)
+            self.assertIn('deprecated', w.text())
+            self.assertEqual(m.initial_values(True), s1)
 
     def test_map_to_state(self):
         # Test :meth:`Model.map_to_state()`.
 
         # Create test model
         m = myokit.Model()
         c = m.add_component('c')
@@ -1620,15 +1825,15 @@
         self.assertEqual(m.count_components(), 1)
         m.remove_component(X)
         self.assertEqual(m.count_components(), 0)
 
     def test_remove_derivative_references(self):
         # Test the remove_derivative_references() method.
 
-        m0 = myokit.parse_model("""
+        m0 = myokit.parse_model('''
             [[model]]
             c.x = 0
             c.y = 1
 
             [e]
             t = 0 bind time
 
@@ -1639,16 +1844,16 @@
                     cc = 1.23
                 dot_x = 3
             dot(y) = (12 - y) / 7
             z = 3 * dot(y)
 
             [d]
             z = 3 * dot(c.x) / dot(c.y)
-            """)
-        m2 = myokit.parse_model("""
+            ''')
+        m2 = myokit.parse_model('''
             [[model]]
             c.x = 0
             c.y = 1
 
             [e]
             t = 0 bind time
 
@@ -1661,15 +1866,15 @@
                 dot_x = 3
             dot(y) = dot_y
             dot_y = (12 - y) / 7
             z = 3 * dot_y
 
             [d]
             z = 3 * c.dot_x_1 / c.dot_y
-            """)
+            ''')
 
         # Remove derivatives from m1
         m1 = m0.clone()
         m1.remove_derivative_references()
 
         # Assert model matches expected code
         self.assertEqual(m1.code(), m2.code())
@@ -1696,39 +1901,14 @@
         # Both units set? Then unit is division of two
         m1 = m0.clone()
         m1.get('e.t').set_unit('ms')
         m1.get('c.y').set_unit('mV')
         m1.remove_derivative_references()
         self.assertEqual(m1.get('c.dot_y').unit(), myokit.parse_unit('mV/ms'))
 
-    def test_remove_variable_with_alias(self):
-        # Test cloning of a variable with an alias after an add / remove event.
-
-        m = myokit.Model('AddRemoveClone')
-        c = m.add_component('c')
-        p = c.add_variable('p')
-        p.set_binding('time')
-        p.set_rhs(0)
-        q = c.add_variable('q')
-        q.set_rhs(12)
-        m.validate()    # Raises error if not ok
-        m.clone()       # Raises error if not ok
-        d = m.add_component('d')
-        d.add_alias('bert', p)
-        e = d.add_variable('e')
-        e.set_rhs('10 * bert')
-        m.validate()
-        m.clone()
-        d.add_alias('ernie', q)
-        m.validate()
-        m.clone()
-        c.remove_variable(q)
-        m.validate()
-        m.clone()   # Will raise error if alias isn't deleted
-
     def test_reorder_state(self):
         # Test :meth:`Model.reorder_state()`.
 
         m = myokit.Model()
         c = m.add_component('c')
         t = c.add_variable('time')
         t.set_binding('time')
@@ -1826,14 +2006,78 @@
 
         cs = [c for c in model]
         self.assertEqual(cs, list(model.components()))
         self.assertEqual(len(cs), len(model))
         c = model['membrane']
         self.assertEqual(c.name(), 'membrane')
 
+    def test_set_initial_values(self):
+        # Tests :meth:`Model.set_initial_values()`.
+        m = myokit.load_model('example')
+        states = [v.qname() for v in m.states()]
+        values = m.initial_values(as_floats=True)
+
+        # Set with floats
+        values[0] += 2
+        m.set_initial_values(values)
+        for val, ref in zip(m.initial_values(True), values):
+            self.assertEqual(val, ref)
+
+        # Set with expressions
+        values[1] -= 3
+        m.set_initial_values([myokit.Number(v) for v in values])
+        for val, ref in zip(m.initial_values(True), values):
+            self.assertEqual(val, ref)
+
+        # Set with mix, including strings and expressions
+        values[2] += 10
+        mixed = list(values)
+        mixed[2] = myokit.Number(mixed[2])
+        mixed[3] = str(values[3])
+        m.set_initial_values(mixed)
+        for val, ref in zip(m.initial_values(True), values):
+            self.assertEqual(val, ref)
+
+        # Set with dict of floats
+        values = m.initial_values(as_floats=True)
+        s = dict(zip(states, values))
+        m.set_initial_values(s)
+        for val, ref in zip(m.initial_values(True), values):
+            self.assertEqual(val, ref)
+
+        # Set with one big string
+        values[0] += 5
+        s = dict(zip(states, values))
+        s = '\n'.join([str(a) + '=' + str(b) for a, b in s.items()])
+        m.set_initial_values(s)
+        for val, ref in zip(m.initial_values(True), values):
+            self.assertEqual(val, ref)
+
+        # Test that errors are detected in validation
+        values[0] = myokit.Name(m.get('membrane.V'))
+        m.set_initial_values(values)
+        self.assertRaisesRegex(myokit.IntegrityError, 'not const', m.validate)
+        values[0] = 'sqrt(3)'
+        m.set_initial_values(values)
+        m.validate()
+
+        # Deprecated alias
+        values = m.initial_values(as_floats=True)
+        values[0] += 10
+        with WarningCollector() as w:
+            m.set_state(values)
+        self.assertIn('deprecated', w.text())
+        for val, ref in zip(m.initial_values(True), values):
+            self.assertEqual(val, ref)
+
+        # Wrong number of elements
+        self.assertRaisesRegex(
+            ValueError, 'Wrong number of initial values',
+            m.set_initial_values, [1, 2, 3])
+
     def test_show_evaluation_of(self):
         # Test :meth:`Model.show_evaluation_of(variable)`.
         # Depends mostly on `references()`, and `code()` methods.
 
         m = myokit.load_model('example')
 
         # Test for literal
@@ -1863,14 +2107,24 @@
         # Test with guessing of similar
         e = m.show_evaluation_of('ina.Na_o')
         self.assertIn('not found', e)
         self.assertIn('cell.Na_o = ', e)
         self.assertIn('Literal constant', e)
         self.assertEqual(len(e.splitlines()), 7)
 
+        # Test with expressions in initial values
+        m.get('ina.m').set_initial_value('1 / sqrt(4)')
+        e = m.show_evaluation_of('ina.m')
+        self.assertIn('Initial value = 1 / sqrt(4)', e)
+        self.assertEqual(len(e.splitlines()), 16)
+        m.get('ina.m').set_initial_value('1 / sqrt(ina.gNa)')
+        e = m.show_evaluation_of('ina.m')
+        self.assertIn('Initial value = 1 / sqrt(ina.gNa)', e)
+        self.assertIn('              = 2.5000000', e)
+
         # Test with nothing similar
         m = myokit.Model()
         self.assertRaises(Exception, m.show_evaluation_of, 'Hello')
 
     def test_show_expressions_for(self):
         # Test :meth:`Model.show_expressions_for(variable)`.
 
@@ -1882,28 +2136,28 @@
     def test_show_line_of(self):
         # Test :meth:`Model.show_line_of(variable)`.
 
         # Check string with info
         m = myokit.load_model('example')
         v = m.get('ina.INa')
         e = m.show_line_of(v)
-        self.assertIn('Defined on line 91', e)
+        self.assertIn('Defined on line 90', e)
         self.assertIn('Intermediary variable', e)
         self.assertEqual(len(e.splitlines()), 4)
 
         # Check with freshly made model
         m2 = m.clone()
         v2 = m2.get('ina.INa')
         e = m2.show_line_of(v2)
         self.assertNotIn('Defined on line', e)
         self.assertIn('Intermediary variable', e)
         self.assertEqual(len(e.splitlines()), 3)
 
         # 'raw' version
-        self.assertEqual(m.show_line_of(v, raw=True), 91)
+        self.assertEqual(m.show_line_of(v, raw=True), 90)
         self.assertIsNone(m2.show_line_of(v2, raw=True))
 
     def test_str(self):
         # Test conversion to string
 
         m = myokit.Model()
         self.assertEqual(str(m), '<Unnamed Model>')
@@ -2047,14 +2301,64 @@
         self.assertRaisesRegex(
             ValueError, 'prepend cannot be empty',
             m.reserve_unique_name_prefix, 'x', '')
         self.assertRaisesRegex(
             ValueError, 'prepend cannot start with prefix',
             m.reserve_unique_name_prefix, 'x', 'x')
 
+    def test_unused_and_cycles(self):
+        # Test unused variable and cycle detection.
+
+        m = myokit.Model('LotkaVolterra')
+        c0 = m.add_component('c0')
+        t = c0.add_variable('time')
+        t.set_rhs(myokit.Number(0))
+        t.set_binding('time')
+        c1 = m.add_component('c1')
+        m.add_component('c2')
+        c1_a = c1.add_variable('a')
+        c1_b = c1.add_variable('b')
+        c1_a.promote(1.0)
+        c1_a.set_rhs(myokit.Multiply(myokit.Name(c1_a), myokit.Number(0.5)))
+        c1_b.set_rhs(myokit.Multiply(myokit.Name(c1_a), myokit.Number(1.0)))
+        # b is unused, test if found
+        m.validate()
+        w = m.warnings()
+        self.assertEqual(len(w), 1)
+        self.assertEqual(type(w[0]), myokit.UnusedVariableError)
+        # b is used by c, c is unused, test if found
+        c1_c = c1.add_variable('c')
+        c1_c.set_rhs(myokit.Name(c1_b))
+        m.validate()
+        w = m.warnings()
+        self.assertEqual(len(w), 2)
+        self.assertEqual(type(w[0]), myokit.UnusedVariableError)
+        self.assertEqual(type(w[1]), myokit.UnusedVariableError)
+        # Test 1:1 cycle
+        c1_b.set_rhs(myokit.Name(c1_b))
+        self.assertRaises(myokit.CyclicalDependencyError, m.validate)
+        # Test longer cycles
+        c1_b.set_rhs(myokit.Multiply(myokit.Number(10), myokit.Name(c1_c)))
+        self.assertRaises(myokit.CyclicalDependencyError, m.validate)
+        # Reset
+        c1_b.set_rhs(myokit.Multiply(myokit.Name(c1_a), myokit.Number(1.0)))
+        m.validate()
+        # Test cycle involving state variable
+        c1_a.set_rhs(myokit.Name(c1_b))
+        m.validate()
+        c1_b.set_rhs(myokit.Multiply(myokit.Name(c1_a), myokit.Name(c1_b)))
+        self.assertRaises(myokit.CyclicalDependencyError, m.validate)
+        c1_b.set_rhs(myokit.Multiply(myokit.Name(c1_a), myokit.Name(c1_c)))
+        c1_c.set_rhs(myokit.Multiply(myokit.Name(c1_a), myokit.Number(3)))
+        m.validate()
+        w = m.warnings()
+        self.assertEqual(len(w), 0)
+        c1_c.set_rhs(myokit.Multiply(myokit.Name(c1_a), myokit.Name(c1_b)))
+        self.assertRaises(myokit.CyclicalDependencyError, m.validate)
+
     def test_validate_and_remove_unused_variables(self):
         # Test :class:`Model.validate` with ``remove_unused_variables=True``.
 
         m = myokit.Model()
         c = m.add_component('c')
         t = c.add_variable('time')
         t.set_binding('time')
```

### Comparing `myokit-1.33.9/myokit/tests/test_model_building.py` & `myokit-1.34.0/myokit/tests/test_model_building.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #!/usr/bin/env python3
 #
 # Tests the model building API.
 #
+# NOTE: THESE TESTS SHOULD SLOWLY BE MERGED INTO test_model, test_variable, etc
+#
+#
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
 from __future__ import absolute_import, division
 from __future__ import print_function, unicode_literals
 
 import myokit
@@ -29,21 +32,31 @@
 
 class ModelBuildTest(unittest.TestCase):
 
     def test_model_creation(self):
         # Create a model
         m = myokit.Model('LotkaVolterra')
 
-        # Add the first component
+        # Add engine component
+        E = m.add_component('engine')
+        self.assertEqual(len(m), 1)
+        time = E.add_variable('time')
+        time.set_rhs(0)
+        self.assertIsNone(time.binding())
+        time.set_binding('time')
+        self.assertIsNotNone(time.binding())
+
+        # Add the first test component
         X = m.add_component('X')
+        self.assertNotEqual(E, X)
         self.assertEqual(X.qname(), 'X')
         self.assertEqual(X.parent(), m)
         self.assertIsInstance(X, myokit.Component)
         self.assertIn(X.qname(), m)
-        self.assertEqual(len(m), 1)
+        self.assertEqual(len(m), 2)
 
         # Add variable a
         self.assertFalse(X.has_variable('a'))
         a = X.add_variable('a')
         self.assertTrue(X.has_variable('a'))
         self.assertEqual(a, a)
         self.assertIsInstance(a, myokit.Variable)
@@ -107,15 +120,15 @@
         self.assertIsInstance(x, myokit.Variable)
         self.assertEqual(len(X), 3)
         self.assertIn(x.name(), X)
         self.assertTrue(x.is_state())
         self.assertFalse(x.is_intermediary())
         self.assertFalse(x.is_constant())
         self.assertEqual(x.lhs(), myokit.Derivative(myokit.Name(x)))
-        self.assertEqual(x.indice(), 0)
+        self.assertEqual(x.index(), 0)
 
         # Test demoting, promoting
         x.demote()
         self.assertFalse(x.is_state())
         self.assertFalse(x.is_intermediary())
         self.assertTrue(x.is_constant())
         self.assertEqual(x.lhs(), myokit.Name(x))
@@ -129,18 +142,40 @@
         x.demote()
         x.promote()
         self.assertTrue(x.is_state())
         self.assertFalse(x.is_intermediary())
         self.assertFalse(x.is_constant())
         self.assertEqual(x.lhs(), myokit.Derivative(myokit.Name(x)))
 
+        # Set number initial value
+        x.demote()
+        x.promote(1)
+        self.assertEqual(x.initial_value(as_float=True), 1)
+
+        # Set constant expression initial value
+        x.set_initial_value(myokit.Name(b))
+        self.assertEqual(x.initial_value(as_float=True), 2)
+        self.assertEqual(x.initial_value(), myokit.Name(b))
+
+        # Non-constant expression initial value can be set, but isn't valid
+        m.validate()
+        b.promote()
+        self.assertRaisesRegex(
+            myokit.IntegrityError, 'not constant', m.validate)
+        b.demote()
+
+        # Set literal valued expression initial value
+        x.demote()
+        x.promote('1 + 2')
+        self.assertEqual(x.initial_value(as_float=True), 3)
+
         # Add second component, variables
         Y = m.add_component('Y')
         self.assertNotEqual(X, Y)
-        self.assertEqual(len(m), 2)
+        self.assertEqual(len(m), 3)
         c = Y.add_variable('c')
         c.set_rhs(myokit.Minus(myokit.Name(a), myokit.Number(1)))
         d = Y.add_variable('d')
         d.set_rhs(2)
         y = Y.add_variable('y')
         y.promote()
 
@@ -148,59 +183,47 @@
         x.set_rhs(myokit.Minus(
             myokit.Multiply(myokit.Name(a), myokit.Name(x)),
             myokit.Multiply(
                 myokit.Multiply(myokit.Name(b), myokit.Name(x)),
                 myokit.Name(y)
             )
         ))
-        x.set_state_value(10)
+        x.set_initial_value(10)
         self.assertEqual(x.rhs().code(), 'X.a * X.x - X.b * X.x * Y.y')
         y.set_rhs(myokit.Plus(
             myokit.Multiply(
                 myokit.PrefixMinus(myokit.Name(c)), myokit.Name(y)
             ),
             myokit.Multiply(
                 myokit.Multiply(myokit.Name(d), myokit.Name(x)),
                 myokit.Name(y)
             )
         ))
-        y.set_state_value(5)
+        y.set_initial_value(5)
         self.assertEqual(y.rhs().code(), '-Y.c * Y.y + Y.d * X.x * Y.y')
 
         # Add ano component, variables
         Z = m.add_component('Z')
         self.assertNotEqual(X, Z)
         self.assertNotEqual(Y, Z)
-        self.assertEqual(len(m), 3)
+        self.assertEqual(len(m), 4)
         t = Z.add_variable('total')
         self.assertEqual(t.name(), 'total')
         self.assertEqual(t.qname(), 'Z.total')
         self.assertEqual(t.qname(X), 'Z.total')
         self.assertEqual(t.qname(Z), 'total')
         t.set_rhs(myokit.Plus(myokit.Name(x), myokit.Name(y)))
         self.assertFalse(t.is_state())
         self.assertFalse(t.is_constant())
         self.assertTrue(t.is_intermediary())
         self.assertEqual(t.rhs().code(), 'X.x + Y.y')
         self.assertEqual(t.rhs().code(X), 'x + Y.y')
         self.assertEqual(t.rhs().code(Y), 'X.x + y')
         self.assertEqual(t.rhs().code(Z), 'X.x + Y.y')
 
-        # Add engine component
-        E = m.add_component('engine')
-        self.assertNotEqual(X, E)
-        self.assertNotEqual(Y, E)
-        self.assertNotEqual(Z, E)
-        self.assertEqual(len(m), 4)
-        time = E.add_variable('time')
-        time.set_rhs(0)
-        self.assertIsNone(time.binding())
-        time.set_binding('time')
-        self.assertIsNotNone(time.binding())
-
         # Check state
         state = [i for i in m.states()]
         self.assertEqual(len(state), 2)
         self.assertIn(x, state)
         self.assertIn(y, state)
 
         # Test variable iterators
@@ -351,24 +374,14 @@
         self.assertEqual(eqs[3].code(), 'X.b = b1 + b2')
 
         # Test model export and cloning
         code1 = m.code()
         code2 = m.clone().code()
         self.assertEqual(code1, code2)
 
-    def test_resolve(self):
-        # Test if an error is raised when a variable can't be resolved.
-
-        m = myokit.Model('Resolve')
-        c = m.add_component('c')
-        p = c.add_variable('p')
-        q = c.add_variable('q')
-        p.set_rhs('10 * q')
-        self.assertRaises(myokit.ParseError, q.set_rhs, '10 * r')
-
     def test_scope(self):
         # Test if illegal references are detected.
 
         m = myokit.Model('Scope')
         c = m.add_component('c')
         p = c.add_variable('p')
         q = p.add_variable('q')
@@ -432,60 +445,10 @@
         self.assertRaises(myokit.InvalidNameError, v1.add_variable, 'ab.cd')
         self.assertRaises(myokit.InvalidNameError, v1.add_variable, 'ab!cd')
         self.assertRaises(myokit.InvalidNameError, v1.add_variable, '5*x')
         # Keywords
         self.assertRaises(myokit.InvalidNameError, v1.add_variable, 'not')
         self.assertRaises(myokit.InvalidNameError, v1.add_variable, 'in')
 
-    def test_unused_and_cycles(self):
-        # Test unused variable and cycle detection.
-
-        m = myokit.Model('LotkaVolterra')
-        c0 = m.add_component('c0')
-        t = c0.add_variable('time')
-        t.set_rhs(myokit.Number(0))
-        t.set_binding('time')
-        c1 = m.add_component('c1')
-        m.add_component('c2')
-        c1_a = c1.add_variable('a')
-        c1_b = c1.add_variable('b')
-        c1_a.promote(1.0)
-        c1_a.set_rhs(myokit.Multiply(myokit.Name(c1_a), myokit.Number(0.5)))
-        c1_b.set_rhs(myokit.Multiply(myokit.Name(c1_a), myokit.Number(1.0)))
-        # b is unused, test if found
-        m.validate()
-        w = m.warnings()
-        self.assertEqual(len(w), 1)
-        self.assertEqual(type(w[0]), myokit.UnusedVariableError)
-        # b is used by c, c is unused, test if found
-        c1_c = c1.add_variable('c')
-        c1_c.set_rhs(myokit.Name(c1_b))
-        m.validate()
-        w = m.warnings()
-        self.assertEqual(len(w), 2)
-        self.assertEqual(type(w[0]), myokit.UnusedVariableError)
-        self.assertEqual(type(w[1]), myokit.UnusedVariableError)
-        # Test 1:1 cycle
-        c1_b.set_rhs(myokit.Name(c1_b))
-        self.assertRaises(myokit.CyclicalDependencyError, m.validate)
-        # Test longer cycles
-        c1_b.set_rhs(myokit.Multiply(myokit.Number(10), myokit.Name(c1_c)))
-        self.assertRaises(myokit.CyclicalDependencyError, m.validate)
-        # Reset
-        c1_b.set_rhs(myokit.Multiply(myokit.Name(c1_a), myokit.Number(1.0)))
-        m.validate()
-        # Test cycle involving state variable
-        c1_a.set_rhs(myokit.Name(c1_b))
-        m.validate()
-        c1_b.set_rhs(myokit.Multiply(myokit.Name(c1_a), myokit.Name(c1_b)))
-        self.assertRaises(myokit.CyclicalDependencyError, m.validate)
-        c1_b.set_rhs(myokit.Multiply(myokit.Name(c1_a), myokit.Name(c1_c)))
-        c1_c.set_rhs(myokit.Multiply(myokit.Name(c1_a), myokit.Number(3)))
-        m.validate()
-        w = m.warnings()
-        self.assertEqual(len(w), 0)
-        c1_c.set_rhs(myokit.Multiply(myokit.Name(c1_a), myokit.Name(c1_b)))
-        self.assertRaises(myokit.CyclicalDependencyError, m.validate)
-
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `myokit-1.33.9/myokit/tests/test_opencl_info.py` & `myokit-1.34.0/myokit/tests/test_opencl_info.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_pacing_factory.py` & `myokit-1.34.0/myokit/tests/test_pacing_factory.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_pacing_system_c.py` & `myokit-1.34.0/myokit/tests/test_pacing_system_c.py`

 * *Files 10% similar despite different names*

```diff
@@ -140,32 +140,19 @@
             # Plot the new points
             plt.plot(t2, v2, '.', color='green')
             plt.show()
             # Quite
             import sys
             sys.exit(1)
 
-        # Test input checking
-        times = 1
-        values = [1, 2]
-        self.assertRaises(Exception, AnsicFixedFormPacing)
-        self.assertRaises(Exception, AnsicFixedFormPacing, 1)
-        self.assertRaises(Exception, AnsicFixedFormPacing, 1, 2)
-        self.assertRaises(Exception, AnsicFixedFormPacing, [1], [2])
-        self.assertRaises(
-            Exception, AnsicFixedFormPacing, [1, 2], [2])
-        self.assertRaises(
-            Exception, AnsicFixedFormPacing, [2, 1], [2, 2])
-        AnsicFixedFormPacing([1, 2], [1, 2])
-
         # Test with small lists
         values = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]
         times = [0, 0, 1, 1, 1, 2, 2, 2, 3, 4, 5, 7]
         values = list(range(len(times)))
-        pacing = AnsicFixedFormPacing(times, values)
+        pacing = AnsicFixedFormPacing(myokit.TimeSeriesProtocol(times, values))
 
         def test(value, index):
             self.assertEqual(pacing.pace(value), index)
 
         test(-1, 0)
         test(0, 1)
         test(1, 2)
```

### Comparing `myokit-1.33.9/myokit/tests/test_pacing_system_py.py` & `myokit-1.34.0/myokit/tests/test_pacing_system_py.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_parsing.py` & `myokit-1.34.0/myokit/tests/test_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,14 +219,15 @@
         self.assertEqual(next(s)[0], p.EOL)
 
 
 class PhasedParseTest(unittest.TestCase):
     """
     Tests several phases of parsing.
     """
+
     def test_segment_parsing(self):
         # Test :meth:`parse_model()`.
         from myokit._parsing import parse
 
         # Empty code --> error
         code = ''
         self.assertRaisesRegex(
@@ -1225,15 +1226,20 @@
         try:
             myokit.parse_expression(b)
         except myokit.ParseError as e:
             self.assertEqual(myokit.format_parse_error(e, source=[b]), error)
 
 
 class ModelParseTest(unittest.TestCase):
+    """
+    Test parsing models.
+    """
+
     def test_model_creation(self):
+        # Basic model creation via the parser
         m = myokit.load_model(os.path.join(DIR_DATA, 'lr-1991.mmt'))
 
         # Test components
         self.assertEqual(len(m), 9)
         self.assertIn('engine', m)
         self.assertIn('membrane', m)
         self.assertIn('cell', m)
@@ -1259,44 +1265,22 @@
             0.0017,
             0.9832,
             0.995484,
             0.000003,
             1,
             0.0057,
             0.0002]
+        self.assertEqual(len(values), m.count_states())
+
+        # Test initial value parsing
         out = ', '.join([str(x) for x in m.states()])
         ref = ', '.join(states)
         self.assertEqual(ref, out)
-        for k, eq in enumerate(m.inits()):
-            self.assertEqual(eq.rhs.eval(), values[k])
-
-        # Test state parsing / setting
-        m.set_state(values)
-        for k, eq in enumerate(m.inits()):
-            self.assertEqual(eq.rhs.eval(), values[k])
-        s = dict(zip(states, values))
-        m.set_state(s)
-        for k, eq in enumerate(m.inits()):
-            self.assertEqual(eq.rhs.eval(), values[k])
-        s = '\n'.join([str(a) + '=' + str(b) for a, b in s.items()])
-        m.set_state(s)
-        for k, eq in enumerate(m.inits()):
-            self.assertEqual(eq.rhs.eval(), values[k])
-
-        # Test cloning
-        try:
-            m2 = m.clone()
-        except Exception as e:
-            s = m.code(line_numbers=True)
-            print('\n')
-            print(s)
-            print('-' * 80)
-            print(myokit.format_parse_error(e, s.splitlines()))
-            raise e
-        self.assertEqual(m.code(), m2.code())
+        for val, ref in zip(m.initial_values(as_floats=True), values):
+            self.assertEqual(val, ref)
 
     def test_unresolved_reference_error(self):
         # Test unresolved reference errors.
         code = """
             [[model]]
 
             [engine]
@@ -1350,27 +1334,29 @@
         # Test a model with a piecewise statement
 
         m = myokit.load_model(
             os.path.join(DIR_DATA, 'conditional.mmt'))
         # Test evaluation
         x = m.get('test.x')
         y = m.get('test.y')
-        s = m.state()
-        i = m.get('membrane.V').indice()
+        s = m.initial_values(as_floats=True)
+        i = m.get('membrane.V').index()
         # Test x, xo, y, yo
+
+        v = myokit.Name(m.get('membrane.V'))
         s[i] = -80
-        m.set_state(s)
+        m.set_initial_values(s)
         self.assertEqual(x.rhs().eval(), 3)
         self.assertEqual(y.rhs().eval(), 2)
         s[i] = -10
-        m.set_state(s)
+        m.set_initial_values(s)
         self.assertEqual(x.rhs().eval(), 2)
         self.assertEqual(y.rhs().eval(), 2)
         s[i] = 30
-        m.set_state(s)
+        m.set_initial_values(s)
         self.assertEqual(x.rhs().eval(), 1)
         self.assertEqual(y.rhs().eval(), 1)
         # Test code() output by cloning
         m.clone()
 
     def test_initial_values(self):
         # Test if expressions for initial values are handled correctly.
@@ -1383,30 +1369,142 @@
             [engine]
             time = 0 bind time
 
             [c]
             dot(p) = 1
             dot(q) = 2
             """
-        myokit.parse(code)
+        m = myokit.parse_model(code)
+        self.assertEqual(m.get('c.p').initial_value(), myokit.Number(1))
+        self.assertEqual(m.get('c.q').initial_value().code(), '10 * 2')
+
+        # initial expression
+        code = """
+            [[model]]
+            c.q = 10 * 2 + c.p
+            c.r = c.p + c.a
+
+            [engine]
+            time = 0 bind time
+
+            [c]
+            p = 0.5
+            dot(q) = 2
+            dot(r) = 1
+            a = p + 1
+            """
+        m = myokit.parse_model(code)
+        self.assertEqual(
+            m.get('c.q').initial_value().code(), '10 * 2 + c.p')
+
+        # initial expression with just literals
+        code = """
+            [[model]]
+            c.q = 10 * exp(2)
+
+            [engine]
+            time = 0 bind time
+
+            [c]
+            p = 0.5
+            dot(q) = 2
+            """
+        m = myokit.parse_model(code)
+        self.assertEqual(
+            m.get('c.q').initial_value().code(), '10 * exp(2)')
 
-        # Non-literal value
+        # non-existent variable in initial value
         code = """
             [[model]]
             c.p = 1.0
-            c.q = 10 * 2 + b
+            c.q = 10 * 2 + c.b
 
             [engine]
             time = 0 bind time
 
             [c]
             dot(p) = 1
             dot(q) = 2
             """
-        self.assertRaises(myokit.ParseError, myokit.parse, code)
+        self.assertRaisesRegex(
+            myokit.ParseError, 'Unresolved reference', myokit.parse, code)
+
+        # initial expression using child variables should fail
+        code = """
+            [[model]]
+            c.q = a
+
+            [engine]
+            time = 0 bind time
+
+            [c]
+            p = 0.5
+            dot(q) = 2
+                a = 10 * 2 + p
+            """
+        self.assertRaisesRegex(
+            myokit.ParseError, 'Unresolved reference', myokit.parse, code)
+
+        # non-constant initial value
+        code = """
+            [[model]]
+            c.p = engine.time
+
+            [engine]
+            time = 0 bind time
+
+            [c]
+            dot(p) = 1
+            """
+        self.assertRaisesRegex(
+            myokit.ParseError, 'is not constant', myokit.parse, code)
+
+        # indirect non-constant initial value
+        code = """
+            [[model]]
+            c.p = c.r
+            c.q = 1
+
+            [engine]
+            time = 0 bind time
+
+            [c]
+            dot(p) = 1
+            dot(q) = 2
+            r = 2 * q
+            """
+        self.assertRaisesRegex(
+            myokit.ParseError, 'is not constant', myokit.parse, code)
+
+        # looks like it shouldn't be constant, but it is!
+        code = """
+            [[model]]
+            c.p = dot(c.p)
+
+            [engine]
+            time = 0 bind time
+
+            [c]
+            dot(p) = 0
+            """
+        # Treat all state variables as non-constant
+        self.assertRaisesRegex(
+            myokit.ParseError, 'is not constant', myokit.parse, code)
+
+        # Initial value cycles are caught in validation
+        code = """
+            [[model]]
+            x.x = x.x
+
+            [x]
+            dot(x) = x
+            t = 0 bind time
+            """
+        self.assertRaisesRegex(
+            myokit.ParseError, 'is not constant', myokit.parse, code)
 
     def test_aliases(self):
         code = """
             [[model]]
 
             [engine]
             time = 0 bind time
```

### Comparing `myokit-1.33.9/myokit/tests/test_progress_reporters.py` & `myokit-1.34.0/myokit/tests/test_progress_reporters.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_protocol.py` & `myokit-1.34.0/myokit/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_protocol_floating_point.py` & `myokit-1.34.0/myokit/tests/test_protocol_floating_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         self.assertEqual(p.characteristic_time(), 30000)
         self.assertTrue(p.is_sequence())
         self.assertTrue(p.is_unbroken_sequence())
 
 
 class PacingSystemFloatingPointTest(unittest.TestCase):
     """
-    Test float behaviour in the Python PacingSystem implementation, using the
+    Test float behavior in the Python PacingSystem implementation, using the
     log_for_interval method.
     """
 
     def test_python_pacing_floats_1(self):
 
         # Test fixes for event start/end touching
         p = myokit.Protocol()
```

### Comparing `myokit-1.33.9/myokit/tests/test_pype.py` & `myokit-1.34.0/myokit/tests/test_pype.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_quantity.py` & `myokit-1.34.0/myokit/tests/test_quantity.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_rhs_benchmarker.py` & `myokit-1.34.0/myokit/tests/test_rhs_benchmarker.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_sbml_api.py` & `myokit-1.34.0/myokit/tests/test_sbml_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1210,15 +1210,15 @@
         # Check setting referenced initial value parameter for size
         sm = sbml.Model()
         p = sm.add_parameter('parameter')
         c = sm.add_compartment('comp')
         c.set_initial_value(myokit.Name(p))
         mm = sm.myokit_model()
         self.assertTrue(mm.has_component('comp'))
-        self.assertEqual(mm.get('comp.size').rhs().code(), 'myokit.parameter')
+        self.assertEqual(mm.get('comp.size').rhs().code(), 'global.parameter')
         self.assertFalse(mm.get('comp.size').is_state())
 
         # Check setting size as value
         sm = sbml.Model()
         c = sm.add_compartment('comp')
         c.set_value(myokit.Number(3))
         mm = sm.myokit_model()
@@ -1237,15 +1237,15 @@
         # Check setting referenced value parameter for size
         sm = sbml.Model()
         p = sm.add_parameter('parameter')
         c = sm.add_compartment('comp')
         c.set_value(myokit.Name(p))
         mm = sm.myokit_model()
         self.assertTrue(mm.has_component('comp'))
-        self.assertEqual(mm.get('comp.size').rhs().code(), 'myokit.parameter')
+        self.assertEqual(mm.get('comp.size').rhs().code(), 'global.parameter')
         self.assertFalse(mm.get('comp.size').is_state())
 
         # Check setting size as rate
         sm = sbml.Model()
         c = sm.add_compartment('comp')
         c.set_value(myokit.Number(1.5), is_rate=True)
         with WarningCollector():
@@ -1285,37 +1285,37 @@
         m = sbml.Model()
         m.add_parameter('z')
         m.add_parameter('boat')
         m.add_parameter('c')
         m = m.myokit_model()
 
         # Check that model created parameters in 'global' component
-        self.assertTrue(m.has_variable('myokit.z'))
-        self.assertTrue(m.has_variable('myokit.boat'))
-        self.assertTrue(m.has_variable('myokit.c'))
+        self.assertTrue(m.has_variable('global.z'))
+        self.assertTrue(m.has_variable('global.boat'))
+        self.assertTrue(m.has_variable('global.c'))
 
         # Check that total number of parameters is 4 (3 parameters and time)
         self.assertEqual(m.count_variables(), 4)
 
     def test_parameters_initial_value(self):
         # Tests adding parameters set with initial values
 
         m = sbml.Model()
         p = m.add_parameter('param')
         p.set_initial_value(myokit.Number(7))
         mm = m.myokit_model()
-        pp = mm.get('myokit.param')
+        pp = mm.get('global.param')
         self.assertFalse(pp.is_state())
         self.assertEqual(pp.rhs(), myokit.Number(7))
 
         # Test units
         self.assertIsNone(pp.unit())
         p.set_units(myokit.units.pF)
         mm = m.myokit_model()
-        pp = mm.get('myokit.param')
+        pp = mm.get('global.param')
         self.assertFalse(pp.is_state())
         self.assertEqual(pp.rhs(), myokit.Number(7))
         self.assertEqual(pp.unit(), myokit.units.pF)
 
         # Unreferenced parameter
         m = sbml.Model()
         p_bad = sbml.Parameter(m, 'p_bad')
@@ -1327,24 +1327,24 @@
     def test_parameters_values(self):
         # Tests adding parameters set with a value (non-state)
 
         m = sbml.Model()
         p = m.add_parameter('param')
         p.set_value(myokit.Plus(myokit.Number(7), myokit.Number(3)))
         mm = m.myokit_model()
-        pp = mm.get('myokit.param')
+        pp = mm.get('global.param')
         self.assertFalse(pp.is_state())
         self.assertEqual(
             pp.rhs(), myokit.Plus(myokit.Number(7), myokit.Number(3)))
 
         # Test units
         self.assertIsNone(pp.unit())
         p.set_units(myokit.units.pF)
         mm = m.myokit_model()
-        pp = mm.get('myokit.param')
+        pp = mm.get('global.param')
         self.assertFalse(pp.is_state())
         self.assertEqual(pp.rhs().code(), '7 + 3')
         self.assertEqual(pp.unit(), myokit.units.pF)
 
         # Unreferenced parameter
         m = sbml.Model()
         p_bad = sbml.Parameter(m, 'p_bad')
@@ -1357,32 +1357,32 @@
         # Tests adding parameters set with a value (state)
 
         m = sbml.Model()
         p = m.add_parameter('param')
         p.set_value(myokit.Number(3.2), is_rate=True)
         with WarningCollector():
             mm = m.myokit_model()
-        pp = mm.get('myokit.param')
+        pp = mm.get('global.param')
         self.assertTrue(pp.is_state())
         self.assertEqual(pp.rhs(), myokit.Number(3.2))
-        self.assertEqual(pp.state_value(), 0)
+        self.assertEqual(pp.initial_value(as_float=True), 0)
 
         # With initial value
         p.set_initial_value(myokit.Number(1))
         mm = m.myokit_model()
-        pp = mm.get('myokit.param')
+        pp = mm.get('global.param')
         self.assertTrue(pp.is_state())
         self.assertEqual(pp.rhs(), myokit.Number(3.2))
-        self.assertEqual(pp.state_value(), 1)
+        self.assertEqual(pp.initial_value(as_float=True), 1)
 
         # Test units
         self.assertIsNone(pp.unit())
         p.set_units(myokit.units.pF)
         mm = m.myokit_model()
-        pp = mm.get('myokit.param')
+        pp = mm.get('global.param')
         self.assertTrue(pp.is_state())
         self.assertEqual(pp.rhs(), myokit.Number(3.2))
         self.assertEqual(pp.unit(), myokit.units.pF)
 
         # Unreferenced parameter
         m = sbml.Model()
         p_bad = sbml.Parameter(m, 'p_bad')
@@ -1474,15 +1474,15 @@
 
         # Species in amount: referenced parameter
         p1 = m.add_parameter('p1')
         s1.set_initial_value(value=myokit.Name(p1), in_amount=True)
         mm = m.myokit_model()
         ms = mm.get('comp.spec_1_amount')
         self.assertFalse(ms.is_state())
-        self.assertEqual(ms.rhs().code(), 'myokit.p1')
+        self.assertEqual(ms.rhs().code(), 'global.p1')
 
         # Species in concentration: unreferenced parameter
         p2 = sbml.Parameter(m, 'p2')
         s2.set_initial_value(value=myokit.Name(p2), in_amount=False)
         self.assertRaisesRegex(
             sbml.SBMLError, 'Initial value of <', m.myokit_model)
 
@@ -1538,56 +1538,56 @@
         s1 = m.add_species(c, 'spec_1', is_amount=True)
         s1.set_value(myokit.Number(3), is_rate=True)
         with WarningCollector():
             mm = m.myokit_model()
         ms = mm.get('comp.spec_1_amount')
         self.assertTrue(ms.is_state())
         self.assertEqual(ms.rhs(), myokit.Number(3))
-        self.assertEqual(ms.state_value(), 0)
+        self.assertEqual(ms.initial_value(as_float=True), 0)
         s1.set_initial_value(myokit.Number(7))
         mm = m.myokit_model()
         ms = mm.get('comp.spec_1_amount')
         self.assertTrue(ms.is_state())
         self.assertEqual(ms.rhs(), myokit.Number(3))
-        self.assertEqual(ms.state_value(), 7)
+        self.assertEqual(ms.initial_value(as_float=True), 7)
 
         # Species in concentration
         s2 = m.add_species(c, 'spec_2', is_amount=False)
         s2.set_value(myokit.Number(4), is_rate=True)
         with WarningCollector():
             mm = m.myokit_model()
         sc = mm.get('comp.spec_2_concentration')
         self.assertFalse(sc.is_state())
         self.assertEqual(
             sc.rhs().code(), 'comp.spec_2_amount / comp.size')
         sa = mm.get('comp.spec_2_amount')
         self.assertTrue(sa.is_state())
         self.assertEqual(sa.rhs().code(), '4 * comp.size')
-        self.assertEqual(sa.state_value(), 0)
+        self.assertEqual(sa.initial_value(as_float=True), 0)
 
         # I: Set compartment size
         m = sbml.Model()
         c = m.add_compartment('comp')
         c.set_initial_value(myokit.Number(2))
 
         # Species in amount
         s1 = m.add_species(c, 'spec_1', is_amount=True)
         s1.set_value(myokit.Number(3), is_rate=True)
         with WarningCollector():
             mm = m.myokit_model()
         ms = mm.get('comp.spec_1_amount')
         self.assertTrue(ms.is_state())
         self.assertEqual(ms.rhs(), myokit.Number(3))
-        self.assertEqual(ms.state_value(), 0)
+        self.assertEqual(ms.initial_value(as_float=True), 0)
         s1.set_initial_value(myokit.Number(7))
         mm = m.myokit_model()
         ms = mm.get('comp.spec_1_amount')
         self.assertTrue(ms.is_state())
         self.assertEqual(ms.rhs(), myokit.Number(3))
-        self.assertEqual(ms.state_value(), 7)
+        self.assertEqual(ms.initial_value(as_float=True), 7)
 
         # Species in concentration
         s2 = m.add_species(c, 'spec_2', is_amount=False)
         s2.set_value(myokit.Number(4), is_rate=True)
         with WarningCollector():
             mm = m.myokit_model()
         sc = mm.get('comp.spec_2_concentration')
@@ -1595,15 +1595,15 @@
         self.assertEqual(
             sc.rhs().code(), 'comp.spec_2_amount / comp.size')
         s2.set_initial_value(myokit.Number(6))
         mm = m.myokit_model()
         sa = mm.get('comp.spec_2_amount')
         self.assertTrue(sa.is_state())
         self.assertEqual(sa.rhs().code(), '4 * comp.size')
-        self.assertEqual(sa.state_value(), 6 * 2)
+        self.assertEqual(sa.initial_value(as_float=True), 6 * 2)
 
     def test_species_units(self):
         # Tests whether species units are set properly.
 
         # Test I: No substance nor size units provided
         m = sbml.Model()
         c = m.add_compartment('c')
@@ -1964,15 +1964,15 @@
         self.assertEqual(var.eval(), 0 * (2 / 1.2 + 1.5))
 
         # Check values for stoichiometries
         var = mm.get('c.sr1')
         self.assertEqual(var.eval(), 5)
 
         var = mm.get('c.sr2')
-        self.assertEqual(var.state_value(), 0)
+        self.assertEqual(var.initial_value(as_float=True), 0)
         self.assertEqual(var.eval(), 3.82)
 
     def test_reaction_stoichiometries_exist(self):
         # Tests whether stoichiometries are created properly.
 
         m = sbml.Model()
         c = m.add_compartment('c')
@@ -2057,15 +2057,15 @@
         self.assertTrue(var.is_state())
 
         # Check value of stoichiometries
         var = mm.get('c.sr1')
         self.assertEqual(var.eval(), 15.23)
 
         var = mm.get('c.sr2')
-        self.assertEqual(var.state_value(), 3.5)
+        self.assertEqual(var.initial_value(as_float=True), 3.5)
         self.assertEqual(var.eval(), 9.23)
 
         # Bad value
         m = sbml.Model()
         p = sbml.Parameter(m, 'parameter')
         c = m.add_compartment('c')
         s1 = m.add_species(c, 's1')
@@ -2164,18 +2164,18 @@
         # Tests whether time variable is created.
 
         m = sbml.Model()
         m.set_time_units(myokit.units.ampere)
         m = m.myokit_model()
 
         # Check that time variable exists
-        self.assertTrue(m.has_variable('myokit.time'))
+        self.assertTrue(m.has_variable('global.time'))
 
         # Check that unit is set
-        var = m.get('myokit.time')
+        var = m.get('global.time')
         self.assertEqual(var.unit(), myokit.units.ampere)
 
         # Check that initial value is set
         self.assertEqual(var.rhs(), myokit.Number(0, myokit.units.ampere))
 
         # Chet that variable is time bound
         self.assertTrue(var.binding(), 'time')
@@ -2185,18 +2185,18 @@
 
         # Create SBML model
         s = sbml.Model()
         s.set_time_units(myokit.units.ms)
         p = s.add_parameter('param')
         p.set_value(myokit.Plus(myokit.Number(1), myokit.Name(s.time())))
         m = s.myokit_model()
-        t = m.get('myokit.time')
+        t = m.get('global.time')
         self.assertEqual(t.unit(), myokit.units.ms)
         self.assertEqual(
-            m.get('myokit.param').rhs(),
+            m.get('global.param').rhs(),
             myokit.Plus(myokit.Number(1), myokit.Name(m.time())))
 
 
 if __name__ == '__main__':
     import warnings
     warnings.simplefilter('always')
     unittest.main()
```

### Comparing `myokit-1.33.9/myokit/tests/test_sbml_parser.py` & `myokit-1.34.0/myokit/tests/test_sbml_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -909,20 +909,20 @@
         self.assertEqual(
             r.kinetic_law().code(),
             '<Compartment c> * <Parameter k1> * <Species S1>')
 
         # Check species reactions (no unecessary zeros and all terms present)
         model_mmt = m.myokit_model().code()
         S1_rhs = \
-            'dot(S1_amount) = -(r1 * (size * myokit.k1 * S1_concentration)) ' \
-            + '- size * myokit.k1 * S1_concentration'
+            'dot(S1_amount) = -(r1 * (size * global.k1 * S1_concentration)) ' \
+            + '- size * global.k1 * S1_concentration'
         self.assertTrue(S1_rhs in model_mmt)
-        S2_rhs = 'dot(S2_amount) = r2 * (size * myokit.k1 * S1_concentration)'
+        S2_rhs = 'dot(S2_amount) = r2 * (size * global.k1 * S1_concentration)'
         self.assertTrue(S2_rhs in model_mmt)
-        S3_rhs = 'dot(S3_amount) = size * myokit.k1 * S1_concentration'
+        S3_rhs = 'dot(S3_amount) = size * global.k1 * S1_concentration'
         self.assertTrue(S3_rhs in model_mmt)
 
     def test_parse_rule(self):
         # Tests parsing assignment rules and rate rules
 
         # Set a parameter value
         a = ('<model name="mathml">'
```

### Comparing `myokit-1.33.9/myokit/tests/test_simulation_1d.py` & `myokit-1.34.0/myokit/tests/test_simulation_1d.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,42 +27,44 @@
 debug = False
 
 
 class Simulation1dTest(unittest.TestCase):
     """
     Test the non-parallel 1d simulation.
     """
+
     def test_basic(self):
         # Test basic usage.
 
         # Load model
         m, p, _ = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
 
         # Run a simulation
         ncells = 5
         s = myokit.Simulation1d(m, p, ncells=ncells)
         s.set_step_size(0.05)
 
+        x0 = m.initial_values(True)
         self.assertEqual(s.time(), 0)
-        self.assertEqual(s.state(0), m.state())
-        self.assertEqual(s.default_state(0), m.state())
+        self.assertEqual(s.state(0), x0)
+        self.assertEqual(s.default_state(0), x0)
         d = s.run(5, log_interval=1)
         self.assertEqual(s.time(), 5)
-        self.assertNotEqual(s.state(0), m.state())
-        self.assertEqual(s.default_state(0), m.state())
+        self.assertNotEqual(s.state(0), x0)
+        self.assertEqual(s.default_state(0), x0)
 
         # Test full state getting and reset
-        self.assertEqual(s.default_state(), m.state() * ncells)
-        self.assertNotEqual(s.state(), m.state() * ncells)
+        self.assertEqual(s.default_state(), x0 * ncells)
+        self.assertNotEqual(s.state(), x0 * ncells)
         s.reset()
         self.assertEqual(s.state(), s.default_state())
 
         # Test pre updates the default state.
         s.pre(1)
-        self.assertNotEqual(s.default_state(0), m.state())
+        self.assertNotEqual(s.default_state(0), x0)
 
         # Test running without a protocol
         s.set_protocol(None)
         s.run(1)
 
         # Simulation time can't be negative
         self.assertRaises(ValueError, s.run, -1)
@@ -99,14 +101,39 @@
         self.assertRaises(ValueError, s.set_step_size, 0)
 
         # Test setting time
         self.assertNotEqual(s.time(), 100)
         s.set_time(100)
         self.assertEqual(s.time(), 100)
 
+    def test_initial_value_expressions(self):
+        # Test if initial value expressions are converted to floats
+        m = myokit.parse_model('''
+            [[model]]
+            c.x = 1 + sqrt(3)
+            c.y = 1 / c.p
+            c.z = 3
+
+            [c]
+            t = 0 bind time
+            dot(x) = 1 label membrane_potential
+            dot(y) = 2
+            dot(z) = 3
+            p = log(3)
+            q = 0 bind diffusion_current
+        ''')
+        s = myokit.Simulation1d(m, ncells=2)
+        x = s.state()
+        self.assertIsInstance(x[0], float)
+        self.assertIsInstance(x[1], float)
+        self.assertIsInstance(x[2], float)
+        self.assertEqual(x[:3], x[3:])
+        self.assertEqual(x, m.initial_values(True) * 2)
+        self.assertEqual(x, s.default_state())
+
     def test_with_progress_reporter(self):
         # Test running with a progress reporter.
         m, p, _ = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
 
         # Test using a progress reporter
         s = myokit.Simulation1d(m, p, ncells=5)
         s.set_step_size(0.05)
@@ -126,74 +153,76 @@
 
     def test_set_state(self):
         # Test :meth:`Simulation1d.set_state()`.
         m, p, _ = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
         n = 4
 
         s = myokit.Simulation1d(m, p, n)
-        self.assertEqual(s.state(), m.state() * n)
+        x0 = m.initial_values(True)
+        self.assertEqual(s.state(), x0 * n)
 
         # Test setting a full state
         sx = [0] * 8 * n
         self.assertNotEqual(sx, s.state())
         s.set_state(sx)
         self.assertEqual(sx, s.state())
 
         # Test setting a single, global state
         sx = [0] * 8
         s.set_state(sx)
         self.assertEqual(s.state(), sx * n)
-        s.set_state(m.state())
-        self.assertEqual(s.state(), m.state() * n)
+        s.set_state(x0)
+        self.assertEqual(s.state(), x0 * n)
 
         # Test setting a single state
         j = 1
         s.set_state(sx, j)
         for i in range(n):
             if i == j:
                 self.assertEqual(s.state(i), sx)
             else:
-                self.assertEqual(s.state(i), m.state())
+                self.assertEqual(s.state(i), x0)
 
         # Invalid cell index
         s.set_state(sx, 0)
         self.assertRaises(ValueError, s.set_state, sx, -1)
         self.assertRaises(ValueError, s.set_state, sx, n)
         self.assertRaises(ValueError, s.state, -1)
         self.assertRaises(ValueError, s.state, n)
 
     def test_set_default_state(self):
         # Test :meth:`Simulation1d.set_default_state()`.
         m, p, _ = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
         n = 4
 
         s = myokit.Simulation1d(m, p, n)
-        self.assertEqual(s.state(), m.state() * n)
+        self.assertEqual(s.state(), m.initial_values(True) * n)
 
         # Test setting a full state
         sx = [0] * 8 * n
         self.assertNotEqual(sx, s.default_state())
         s.set_default_state(sx)
         self.assertEqual(sx, s.default_state())
 
         # Test setting a single, global state
         sx = [0] * 8
         s.set_default_state(sx)
         self.assertEqual(s.default_state(), sx * n)
-        s.set_default_state(m.state())
-        self.assertEqual(s.default_state(), m.state() * n)
+        sy = m.initial_values(True)
+        s.set_default_state(sy)
+        self.assertEqual(s.default_state(), sy * n)
 
         # Test setting a single state
         j = 1
         s.set_default_state(sx, j)
         for i in range(n):
             if i == j:
                 self.assertEqual(s.default_state(i), sx)
             else:
-                self.assertEqual(s.default_state(i), m.state())
+                self.assertEqual(s.default_state(i), sy)
 
         # Invalid cell index
         s.set_default_state(sx, 0)
         self.assertRaises(ValueError, s.set_default_state, sx, -1)
         self.assertRaises(ValueError, s.set_default_state, sx, n)
         self.assertRaises(ValueError, s.default_state, -1)
         self.assertRaises(ValueError, s.default_state, n)
```

### Comparing `myokit-1.33.9/myokit/tests/test_simulation_cvodes.py` & `myokit-1.34.0/myokit/tests/test_simulation_cvodes.py`

 * *Files 18% similar despite different names*

```diff
@@ -76,69 +76,248 @@
         # Negative log interval is set to zero
         self.sim.reset()
         d1 = self.sim.run(5)
         self.sim.reset()
         d2 = self.sim.run(5, log_interval=-5)
         self.assertEqual(d1.time(), d2.time())
 
+    def test_multiple_protocols(self):
+        # Test using multiple protocols
+
+        # Set up a model
+        model = myokit.Model()
+        c = model.add_component('c')
+        t = c.add_variable('t')
+        t.set_binding('time')
+        t.set_rhs(0)
+
+        a = c.add_variable('a')
+        a.set_binding('a')
+        a.set_rhs(0)
+        b = c.add_variable('b')
+        b.set_binding('b')
+        b.set_rhs(0)
+        y = c.add_variable('y')
+        y.promote(1)
+        y.set_rhs('-a * y - b * y')
+
+        # Create two overlapping protocols
+        pa = myokit.Protocol()
+        pa.schedule(level=1, start=0.2, duration=0.5)
+
+        pb = myokit.Protocol()
+        pb.schedule(level=2, start=0.5, duration=0.6)
+
+        # Run a simulation with both
+        s = myokit.Simulation(model, {'a': pa, 'b': pb})
+        s.set_tolerance(1e-8)
+        d = s.run(2).npview()
+        times = d[t]
+
+        # Check that the changing points are in the log
+        self.assertIn(0, times)
+        self.assertIn(0.2, times)
+        self.assertIn(0.5, times)
+        self.assertIn(0.7, times)
+        self.assertIn(1.1, times)
+        self.assertIn(2, times)
+
+        # Check that a, b, and y have the expected values
+        a_up = (times >= 0.2) & (times < 0.7)
+        np.testing.assert_array_equal(d[a], np.where(a_up, 1, 0))
+
+        b_up = (times >= 0.5) & (times < 1.1)
+        np.testing.assert_array_equal(d[b], np.where(b_up, 2, 0))
+
+        # Check that dy/dt has the expected values
+        # dy/dt =
+        #   0   from 0 to 0.2
+        #   -y  from 0.2 to 0.5
+        #   -3y from 0.5 to 0.7
+        #   -2y from 0.7 to 1.1
+        #   0   after 1.1
+        #
+        dy_expect = 0 * times
+        dy_expect[a_up] -= 1 * d[y][a_up]
+        dy_expect[b_up] -= 2 * d[y][b_up]
+        np.testing.assert_array_equal(d['dot(c.y)'], dy_expect)
+
+        # Check that y has the expected values
+        # The solution for dy/dt = -a*y is y(t) = c * exp(-at), so
+        # y =
+        #   1
+        #   exp(-(t - 0.5))
+        #   exp(-0.3) * exp(-3 * (t - 0.5))
+        #   exp(-0.9) * exp(-2 * (t - 0.7))
+        #   exp(-1.7)
+        #
+        y_expect = np.ones(times.shape)
+        i = (times >= 0.2) & (times < 0.5)
+        y_expect[i] = np.exp(-(times[i] - 0.2))
+        i = (times >= 0.5) & (times < 0.7)
+        y_expect[i] = np.exp(-0.3) * np.exp(-3 * (times[i] - 0.5))
+        i = (times >= 0.7) & (times < 1.1)
+        y_expect[i] = np.exp(-0.9) * np.exp(-2 * (times[i] - 0.7))
+        y_expect[times >= 1.1] = np.exp(-1.7)
+        np.testing.assert_array_almost_equal(d[y], y_expect, decimal=3)
+
+        # Test unsetting
+        s.set_protocol(None, label='a')
+        s.reset()
+        d = s.run(2).npview()
+        np.testing.assert_array_equal(d[a], np.zeros(d[a].shape))
+        times = d[t]
+        b_up = (times >= 0.5) & (times < 1.1)
+        np.testing.assert_array_equal(d[b], np.where(b_up, 2, 0))
+        y_expect = np.ones(times.shape)
+        i = (times >= 0.5) & (times < 1.1)
+        y_expect[i] = np.exp(-2 * (times[i] - 0.5))
+        y_expect[times >= 1.1] = np.exp(-1.2)
+        np.testing.assert_array_almost_equal(d[y], y_expect, decimal=3)
+
+        # Test unsetting
+        s.set_protocol(None, label='b')
+        s.reset()
+        d = s.run(2).npview()
+        np.testing.assert_array_equal(d[a], np.zeros(d[a].shape))
+        np.testing.assert_array_equal(d[a], np.zeros(d[a].shape))
+        np.testing.assert_array_equal(d[y], np.ones(d[a].shape))
+
+    def test_mixed_protocols(self):
+        # Test using a step and a time series protocol at the same time
+
+        # Set up a model
+        model = myokit.Model()
+        c = model.add_component('c')
+        t = c.add_variable('t')
+        t.set_binding('time')
+        t.set_rhs(0)
+        a = c.add_variable('a')
+        a.set_binding('a')
+        a.set_rhs(0)
+        b = c.add_variable('b')
+        b.set_binding('b')
+        b.set_rhs(0)
+        y = c.add_variable('y')  # Just to log more points
+        y.promote(1)
+        y.set_rhs('a + b')
+
+        # Set up protocols
+        pa = myokit.pacing.blocktrain(level=2, offset=1, duration=2, period=5)
+        x = np.linspace(0, 10, 100)
+        y = 0.1 + 0.2 * np.sin(x)
+        pb = myokit.TimeSeriesProtocol(x, y)
+
+        # Run a simulation with both
+        s = myokit.Simulation(model, {'a': pa, 'b': pb})
+        s.set_tolerance(1e-8)
+        d = s.run(12).npview()
+        t = d[t]
+
+        # Start, end, and change points visited exactly
+        self.assertIn(0, t)
+        self.assertIn(1, t)
+        self.assertIn(3, t)
+        self.assertIn(6, t)
+        self.assertIn(8, t)
+        self.assertIn(11, t)
+        self.assertIn(12, t)
+
+        # Test a
+        a_e = np.zeros(t.shape)
+        a_e[(t >= 1) & (t < 3)] = 2
+        a_e[(t >= 6) & (t < 8)] = 2
+        a_e[(t >= 11) & (t < 13)] = 2
+        np.testing.assert_array_equal(d[a], a_e)
+
+        # Test b
+        b_e = 0.1 + 0.2 * np.sin(t)
+        b_e[t > 10] = y[-1]
+        # Note: We don't expect a super good match here, as b_e is an exact
+        #       sine value, while the solver will be interpolating y
+        np.testing.assert_array_almost_equal(d[b], b_e, decimal=3)
+
     def test_no_protocol(self):
         # Test running without a protocol.
 
         self.sim.reset()
         self.sim.pre(50)
         self.sim.set_protocol(None)
         d = self.sim.run(50).npview()
 
         # Check if pace was set to zero (see prop 651 / technical docs).
         self.assertTrue(np.all(d['engine.pace'] == 0.0))
 
-    def test_fixed_form_protocol(self):
-        # Test running with a fixed form protocol.
+    def test_wrong_label_set_pacing(self):
+        # Test set_pacing with incorrect label
+        self.sim.reset()
+        self.sim.pre(50)
+        with self.assertRaisesRegex(ValueError, 'Unknown pacing label'):
+            self.sim.set_protocol(None, label='does not exist')
+
+    def test_time_series_protocol(self):
+        # Test running with a time series protocol
 
         n = 10
-        time = list(range(n))
-        pace = [0] * n
-        pace[2:4] = [0.5, 0.5]
+        times = list(range(n))
+        values = [0] * n
+        values[2:4] = [0.5, 0.5]
+        p = myokit.TimeSeriesProtocol(times, values)
 
-        self.sim.set_fixed_form_protocol(time, pace)
+        self.sim.set_protocol(p)
         self.sim.reset()
         d = self.sim.run(n, log_interval=1)
-        self.assertEqual(list(d.time()), time)
-        self.assertEqual(list(d['engine.pace']), pace)
+        self.assertEqual(list(d.time()), times)
+        self.assertEqual(list(d['engine.pace']), values)
 
         # Unset
-        self.sim.set_fixed_form_protocol(None)
+        self.sim.set_protocol(None)
         self.sim.reset()
         d = self.sim.run(n, log_interval=1)
         self.assertEqual(list(d['engine.pace']), [0] * n)
 
         # Reset
-        self.sim.set_fixed_form_protocol(time, pace)
+        self.sim.set_protocol(p)
         self.sim.reset()
         d = self.sim.run(n, log_interval=1)
-        self.assertEqual(list(d.time()), time)
-        self.assertEqual(list(d['engine.pace']), pace)
+        self.assertEqual(list(d.time()), times)
+        self.assertEqual(list(d['engine.pace']), values)
 
         # Unset, replace with original protocol
         self.sim.set_protocol(self.protocol)
         self.sim.reset()
         d = self.sim.run(n, log_interval=1)
-        self.assertNotEqual(list(d['engine.pace']), pace)
+        self.assertNotEqual(list(d['engine.pace']), values)
         self.assertNotEqual(list(d['engine.pace']), [0] * n)
 
-        # Invalid protocols
-        self.assertRaisesRegex(
-            ValueError, 'no times', self.sim.set_fixed_form_protocol,
-            values=pace)
+        # Deprecated version
+        with WarningCollector() as w:
+            self.sim.set_fixed_form_protocol(times, values)
+        self.assertIn('eprecated', w.text())
+        self.sim.reset()
+        d = self.sim.run(n, log_interval=1)
+        self.assertEqual(list(d.time()), times)
+        self.assertEqual(list(d['engine.pace']), values)
         self.assertRaisesRegex(
-            ValueError, 'no values', self.sim.set_fixed_form_protocol,
-            times=time)
+            ValueError, 'No times',
+            self.sim.set_fixed_form_protocol, values=values)
         self.assertRaisesRegex(
-            ValueError, 'same size', self.sim.set_fixed_form_protocol,
-            time, pace[:-1])
+            ValueError, 'No values',
+            self.sim.set_fixed_form_protocol, times=times)
+        self.sim.set_fixed_form_protocol(None)
+        self.sim.reset()
+        d = self.sim.run(n, log_interval=1)
+        self.assertEqual(list(d['engine.pace']), [0] * n)
+
+        # Reset original protocol
+        self.sim.set_protocol(self.protocol)
+        self.sim.reset()
+        d = self.sim.run(n, log_interval=1)
+        self.assertNotEqual(list(d['engine.pace']), values)
+        self.assertNotEqual(list(d['engine.pace']), [0] * n)
 
     def test_in_parts(self):
         # Test running the simulation in parts.
 
         self.sim.reset()
         # New logs should start with first state, finish with final
         d = self.sim.run(150)
@@ -150,14 +329,38 @@
         self.assertEqual(d['membrane.V'][-1], e['membrane.V'][0])
         # Re-used logs shouldn't re-log their first state
         n = len(e['engine.time'])
         e = self.sim.run(50, log=e)
         self.assertNotEqual(e['engine.time'][n - 1], e['engine.time'][n])
         self.assertGreater(e['engine.time'][n], e['engine.time'][n - 1])
 
+    def test_initial_value_expressions(self):
+        # Test if initial value expressions are converted to floats
+
+        m = myokit.parse_model('''
+            [[model]]
+            c.x = 1 + sqrt(3)
+            c.y = 1 / c.p
+            c.z = 3
+
+            [c]
+            t = 0 bind time
+            dot(x) = 1
+            dot(y) = 2
+            dot(z) = 3
+            p = log(3)
+        ''')
+        s = myokit.Simulation(m)
+        x = s.state()
+        self.assertIsInstance(x[0], float)
+        self.assertIsInstance(x[1], float)
+        self.assertIsInstance(x[2], float)
+        self.assertEqual(x, m.initial_values(True))
+        self.assertEqual(x, s.default_state())
+
     def test_pacing_values_at_event_transitions(self):
         # Tests the value of the pacing signal at event transitions
 
         # Create a simple model
         m = myokit.Model()
         c = m.add_component('c')
         t = c.add_variable('t')
@@ -235,17 +438,42 @@
 
         # Cancel from reporter
         self.assertRaises(
             myokit.SimulationCancelledError, self.sim.run, 1,
             progress=CancellingReporter(0))
 
     def test_apd_tracking(self):
-        # Test the APD calculation method.
+        # Test the APD / rootfinding method.
+        # Tested against offline method in test_datalog.py
+
+        # Test that it works
+        self.sim.reset()
+        res = self.sim.run(
+            1800, log=['engine.time', 'membrane.V'],
+            apd_variable='membrane.V', apd_threshold=-70)
 
-        # More testing is done in test_datalog.py!
+        self.assertIsInstance(res, tuple)
+        self.assertEqual(len(res), 2)
+        d, apds = res
+        self.assertIsInstance(d, myokit.DataLog)
+        self.assertIsInstance(apds, myokit.DataLog)
+        self.assertEqual(len(apds), 2)
+        self.assertEqual(apds.length(), 2)
+        self.assertIn('start', apds)
+        self.assertAlmostEqual(apds['start'][0], 1, places=0)
+        self.assertAlmostEqual(apds['start'][1], 1001, places=0)
+        self.assertIn('start', apds)
+        self.assertAlmostEqual(apds['duration'][0], 383.877194, places=1)
+        self.assertAlmostEqual(apds['duration'][1], 378.315915, places=1)
+
+        # Works with variable objects too
+        self.sim.reset()
+        res = self.sim.run(
+            1000, log=['engine.time', 'membrane.V'],
+            apd_variable=self.model.get('membrane.V'), apd_threshold=-70)
 
         # Apd var is not a state
         self.assertRaisesRegex(
             ValueError, 'must be a state',
             self.sim.run, 1000, apd_variable='ina.INa')
 
         # No apd var given, but threshold provided
@@ -331,31 +559,92 @@
         self.sim.run(1)
         d2 = self.sim.eval_derivatives()
         self.assertNotEqual(d1, d2)
         self.assertEqual(d1, self.sim.eval_derivatives(s1))
         self.sim.set_state(s1)
         self.assertEqual(d1, self.sim.eval_derivatives())
 
-    def test_sensitivites_initial(self):
+    def test_eval_derivatives_with_pacing(self):
+        # Test :meth:`Simulation.eval_derivatives()`.
+
+        model = myokit.Model()
+        c = model.add_component('c')
+
+        a = c.add_variable('a')
+        a.set_binding('a')
+        a.set_rhs(0)
+        b = c.add_variable('b')
+        b.set_binding('b')
+        b.set_rhs(0)
+
+        y = c.add_variable('y')
+        t = c.add_variable('t')
+        t.set_binding('time')
+        t.set_rhs(0)
+        y.promote(1)
+        y.set_rhs('- a * y - b * y')
+
+        pa = myokit.Protocol()
+        pa.schedule(1, 0, 0.5)
+
+        pb = myokit.Protocol()
+        pb.schedule(2, 1.0, 0.5)
+
+        sim = myokit.Simulation(model, {'a': pa, 'b': pb})
+        sim.run(1)
+        d1 = sim.eval_derivatives(pacing={'a': 0.5, 'b': 0.5})
+        d2 = sim.eval_derivatives(pacing={'a': 1.5, 'b': 0.5})
+        self.assertNotEqual(d1, d2)
+        d1 = sim.eval_derivatives(pacing={'b': 0.5})
+        d2 = sim.eval_derivatives(pacing={'a': 0.0, 'b': 0.5})
+        self.assertEqual(d1, d2)
+        d1 = sim.eval_derivatives()
+        d2 = sim.eval_derivatives(pacing={'a': 0.0, 'b': 0.0})
+        self.assertEqual(d1, d2)
+        d1 = sim.eval_derivatives(pacing={'a': 0.0, 'b': 0.5})
+        d2 = sim.eval_derivatives(pacing={'aaaaa': 1.0, 'b': 0.5})
+        self.assertEqual(d1, d2)
+
+    def test_sensitivities_initial(self):
         # Test setting initial sensitivity values.
 
         m = myokit.parse_model('''
             [[model]]
-            e.y = 2.3
+            e.y = 1 + 1.3
 
             [e]
             t = 0 bind time
             p = 1 / 100
             dot(y) = 2 * p - y
             ''')
         m.validate()
 
         #TODO: Test results
         s = myokit.Simulation(m, sensitivities=(['e.y'], ['e.p', 'init(e.y)']))
 
+        # Warn if a parameter sensitivity won't be picked up.
+        m = myokit.parse_model('''
+            [[model]]
+            c.x = 1 / c.p
+
+            [c]
+            t = 0 bind time
+            p = 1 / q
+            q = 5
+            r = 3
+            dot(x) = 2 + r
+            ''')
+        m.validate()
+        s = (['c.x'], ['c.q'])
+        self.assertRaisesRegex(
+            NotImplementedError, 'respect to parameters used in initial',
+            myokit.Simulation, m, sensitivities=s)
+        s = (['c.x'], ['c.r'])
+        s = myokit.Simulation(m, sensitivities=s)
+
         # Test bad initial matrix
         self.assertRaisesRegex(
             ValueError, 'None or a list',
             s.run, 10, sensitivities='hello')
 
     def test_sensitivity_ordering(self):
         # Tests that sensitivities are returned in the correct order
@@ -535,16 +824,16 @@
             dot(x) = p * q
             dot(y) = 2 * p - y
             fx = x^2
             fy = r + p^2 + dot(y)
             ''')
         m.validate()
 
-        x0 = m.get('e.x').state_value()
-        y0 = m.get('e.y').state_value()
+        x0 = m.get('e.x').initial_value(True)
+        y0 = m.get('e.y').initial_value(True)
         p = m.get('e.p').eval()
         q = m.get('e.q').eval()
         r = m.get('e.r').eval()
 
         # Dependents is a list of y in dy/dx.
         # Must refer to state, derivative, or intermediary, given as:
         #  - Variable
@@ -689,14 +978,15 @@
         self.assertEqual(self.sim.default_state(), default_state)
 
     def test_set_constant(self):
         # Test :meth:`Simulation.set_constant()`.
 
         # Literal
         self.sim.set_constant('cell.Na_i', 11)
+        self.sim.set_constant(self.model.get('cell.Na_i'), 11)
         self.assertRaises(KeyError, self.sim.set_constant, 'cell.Bert', 11)
 
         # Parameter (needs sensitivies set)
         m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
         sim = myokit.Simulation(m, p, (['ib.Ib'], ['ib.gb']))
         sim.set_constant('ib.gb', 20)
 
@@ -782,14 +1072,15 @@
         # Create a model with a state
         m2 = m1.clone()
         z = m2.get('c').add_variable('z')
         z.set_rhs(0.1)
         z.promote(0)
 
         # Test without protocol and dynamic logging
+        #myokit.DEBUG_WG = True
         s1 = myokit.Simulation(m1)
         d1 = s1.run(5)
         self.assertEqual(len(d1.time()), 2)
         self.assertEqual(list(d1.time()), [0, 5])
         self.assertEqual(list(d1['c.w']), [0, 0])
         s2 = myokit.Simulation(m2)
         d2 = s2.run(6, log_times=d1.time())
@@ -882,31 +1173,14 @@
         self.assertEqual(len(d.time()), len(rt))
         self.assertEqual(len(d.time()), len(ev))
         self.assertTrue(np.all(rt >= 0))
         self.assertTrue(np.all(ev >= 0))
         self.assertTrue(np.all(rt[1:] >= rt[:-1]))
         self.assertTrue(np.all(ev[1:] >= ev[:-1]))
 
-    def test_apd(self):
-        # Test the apd rootfinding routine
-
-        s = myokit.Simulation(self.model, self.protocol)
-        s.set_tolerance(1e-8, 1e-8)
-        d, apds = s.run(
-            1800, log=myokit.LOG_NONE,
-            apd_variable='membrane.V', apd_threshold=-70)
-
-        # Check with threshold equal to V
-        self.assertEqual(len(apds['start']), 2)
-        self.assertEqual(len(apds['duration']), 2)
-        self.assertAlmostEqual(apds['start'][0], 1.19, places=1)
-        self.assertAlmostEqual(apds['start'][1], 1001.19, places=1)
-        self.assertAlmostEqual(apds['duration'][0], 383.88262, places=1)
-        self.assertAlmostEqual(apds['duration'][1], 378.31448, places=1)
-
     def test_derivatives(self):
         # Tests logging of derivatives by comparing with a finite difference
         # approximation
 
         # Run past the upstroke, where finite diff approx is worst
         self.sim.reset()
         self.sim.run(52)
```

### Comparing `myokit-1.33.9/myokit/tests/test_simulation_cvodes_from_disk.py` & `myokit-1.34.0/myokit/tests/test_simulation_cvodes_from_disk.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_simulation_fiber_tissue.py` & `myokit-1.34.0/myokit/tests/test_simulation_fiber_tissue.py`

 * *Files 2% similar despite different names*

```diff
@@ -531,15 +531,15 @@
     def test_fiber_state(self):
         # Test the fiber_state related methods.
 
         # Check simulation state equals model state
         m = self.mf.count_states()
         nx, ny = self.nfx, self.nfy
 
-        sm = self.mf.state()
+        sm = self.mf.initial_values(True)
         for i in range(nx):
             for j in range(ny):
                 self.assertEqual(sm, self.s1.fiber_state(i, j))
 
         try:
             # Test setting a full-sized state
             sx = list(range(nx * ny * m))
@@ -618,22 +618,58 @@
             self.assertRaisesRegex(IndexError, 'y-index out of range',
                                    self.s1.default_fiber_state, 0, ny)
             self.assertRaisesRegex(ValueError, 'both an x and y',
                                    self.s1.default_fiber_state, 0)
         finally:
             self.s1.reset()
 
+    def test_initial_value_expressions(self):
+        # Test if initial value expressions are converted to floats
+        m = myokit.parse_model('''
+            [[model]]
+            c.x = 1 + sqrt(3)
+            c.y = 1 / c.p
+            c.z = 3
+
+            [c]
+            t = 0 bind time
+            dot(x) = 1 label membrane_potential
+                in [mV]
+            dot(y) = 2
+            dot(z) = 3
+            p = log(3)
+            q = 0 bind diffusion_current
+                in [A/F]
+        ''')
+        s = myokit.FiberTissueSimulation(
+            m, m, ncells_fiber=(1, 1), ncells_tissue=(3, 1))
+        x = s.fiber_state()
+        self.assertIsInstance(x[0], float)
+        self.assertIsInstance(x[1], float)
+        self.assertIsInstance(x[2], float)
+        self.assertEqual(x, m.initial_values(True))
+        self.assertEqual(x, s.default_fiber_state())
+
+        x = s.tissue_state()
+        self.assertIsInstance(x[0], float)
+        self.assertIsInstance(x[1], float)
+        self.assertIsInstance(x[2], float)
+        self.assertEqual(x[:3], x[3:6])
+        self.assertEqual(x[:3], x[6:])
+        self.assertEqual(x, m.initial_values(True) * 3)
+        self.assertEqual(x, s.default_tissue_state())
+
     def test_tissue_state(self):
         # Test the set_tissue_state and set_default_tissue_state methods
 
         # Check simulation state equals model state
         m = self.mt.count_states()
         nx, ny = self.ntx, self.nty
 
-        sm = self.mt.state()
+        sm = self.mt.initial_values(True)
         for i in range(nx):
             for j in range(ny):
                 self.assertEqual(sm, self.s1.tissue_state(i, j))
 
         try:
             # Test setting a full-sized state
             sx = list(range(nx * ny * m))
```

### Comparing `myokit-1.33.9/myokit/tests/test_simulation_ic.py` & `myokit-1.34.0/myokit/tests/test_simulation_opencl_log_interval.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,108 +1,101 @@
 #!/usr/bin/env python3
 #
-# Tests the ICSimulation class.
+# Tests the OpenCL simulation classes' interpretation of log_interval
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
 from __future__ import absolute_import, division
 from __future__ import print_function, unicode_literals
 
 import os
 import unittest
 import numpy as np
 
 import myokit
 
-from myokit.tests import DIR_DATA, CancellingReporter, WarningCollector
+from myokit.tests import OpenCL_FOUND, DIR_DATA, WarningCollector
+from myokit.tests.test_simulation_log_interval import PeriodicTest
 
-# Unit testing in Python 2 and 3
-try:
-    unittest.TestCase.assertRaisesRegex
-except AttributeError:
-    unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
+debug = False
 
 
-class ICSimulationTest(unittest.TestCase):
+@unittest.skipIf(not OpenCL_FOUND, 'OpenCL not found on this system.')
+class SimulationOpenCLTest(PeriodicTest):
     """
-    Tests the :class:`ICSimulation`.
+    Tests myokit.SimulationOpenCL for consistent log entry timing.
     """
-    def test_basic(self):
-        # Test basic usage.
-        # Load model
-        m, p, _ = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
-        n = m.count_states()
-
-        # Run a simulation
-        with WarningCollector() as c:
-            s = myokit.ICSimulation(m, p)
-        self.assertIn('`ICSimulation` is deprecated', c.text())
-
-        self.assertEqual(s.time(), 0)
-        self.assertEqual(s.state(), m.state())
-        self.assertEqual(s.default_state(), m.state())
-        self.assertTrue(np.all(s.derivatives() == np.eye(n)))
-        d, e = s.run(20, log_interval=5)
-        self.assertEqual(s.time(), 20)
-        self.assertNotEqual(s.state(), m.state())
-        self.assertEqual(s.default_state(), m.state())
-        self.assertFalse(np.all(s.derivatives() == np.eye(n)))
-
-        # Create a datablock from the simulation log
-        b = s.block(d, e)
-
-        # Calculate eigenvalues
-        b.eigenvalues('derivatives')
-
-        # Log with missing time value
-        d2 = d.clone()
-        del d2['engine.time']
-        self.assertRaisesRegex(ValueError, 'time', s.block, d2, e)
-
-        # Wrong size derivatives array
-        self.assertRaisesRegex(ValueError, 'shape', s.block, d, e[:-1])
-
-        # Time can't be negative
-        self.assertRaises(ValueError, s.run, -1)
-
-        # Test running without a protocol
-        s.set_protocol(None)
-        s.run(1)
+    def test_periodic(self):
+        # Test periodic logging.
 
-        # Test step size is > 0
-        self.assertRaises(ValueError, s.set_step_size, 0)
+        m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
+        s = myokit.SimulationOpenCL(m, p, ncells=1)
+        self.periodic(s)
 
-        # Test negative log interval is ignored
-        s.run(1, log_interval=-1)
 
-    def test_progress_reporter(self):
-        # Test running with a progress reporter.
-        m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
+@unittest.skipIf(not OpenCL_FOUND, 'OpenCL not found on this system.')
+class FiberTissueSimulationTest(unittest.TestCase):
+    """
+    Tests myokit.FiberTissueSimulation for consistent log entry timing.
+    """
+    def test_periodic(self):
+        # Test periodic logging.
 
-        # Test using a progress reporter
-        with WarningCollector() as c:
-            s = myokit.ICSimulation(m, p)
-        with myokit.tools.capture() as c:
-            s.run(110, progress=myokit.ProgressPrinter())
-        c = c.text().splitlines()
-        self.assertTrue(len(c) > 0)
-
-        # Not a progress reporter
-        self.assertRaisesRegex(
-            ValueError, 'ProgressReporter', s.run, 5, progress=12)
-
-        # Cancel from reporter
-        self.assertRaises(
-            myokit.SimulationCancelledError, s.run, 1,
-            progress=CancellingReporter(0))
-
-    def test_invalid_model(self):
-        # Test running with an invalid model.
-        m = myokit.Model()
-        with WarningCollector() as c:
-            self.assertRaises(
-                myokit.MissingTimeVariableError, myokit.ICSimulation, m)
+        m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
+        with WarningCollector():
+            s = myokit.FiberTissueSimulation(
+                m, m, p, ncells_fiber=(1, 1), ncells_tissue=(1, 1))
+
+        # Set tolerance for equality testing
+        emax = 1e-2  # Time steps for logging are approximate
+
+        # Test 1: Simple 5 ms simulation, log_interval 0.5 ms
+        d, e = s.run(
+            5, logf=['engine.time'], logt=myokit.LOG_NONE, log_interval=0.5)
+        d = d.npview()
+        t = d['engine.time']
+        q = np.arange(0, 5, 0.5)
+        if debug:
+            print(t)
+            print(q)
+            print('- ' * 10)
+        self.assertEqual(len(t), len(q))
+        self.assertTrue(np.max(np.abs(t - q)) < emax)
+
+        # Test 2: Very short simulation
+        s.reset()
+        d, e = s.run(
+            1, logf=['engine.time'], logt=myokit.LOG_NONE, log_interval=0.5)
+        d = d.npview()
+        t = d['engine.time']
+        q = np.arange(0, 1, 0.5)
+        if debug:
+            print(t)
+            print(q)
+            print('- ' * 10)
+        self.assertEqual(len(t), len(q))
+        self.assertTrue(np.max(np.abs(t - q)) < emax)
+
+        # Test 3: Stop and start a simulation
+        s.reset()
+        d, e = s.run(
+            1, logf=['engine.time'], logt=myokit.LOG_NONE, log_interval=0.5)
+        d, e = s.run(2, logf=d, logt=myokit.LOG_NONE, log_interval=0.5)
+        d, e = s.run(2, logf=d, logt=myokit.LOG_NONE, log_interval=0.5)
+        d = d.npview()
+        t = d['engine.time']
+        q = np.arange(0, 5, 0.5)
+        if debug:
+            print(t)
+            print(q)
+            print('- ' * 10)
+        self.assertEqual(len(t), len(q))
+        self.assertTrue(np.max(np.abs(t - q)) < emax)
 
 
 if __name__ == '__main__':
+    print('Add -v for more debug output')
+    import sys
+    if '-v' in sys.argv:
+        debug = True
     unittest.main()
```

### Comparing `myokit-1.33.9/myokit/tests/test_simulation_log_interval.py` & `myokit-1.34.0/myokit/tests/test_simulation_log_interval.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
 from __future__ import absolute_import, division
 from __future__ import print_function, unicode_literals
 
 import os
-import platform
 import unittest
 
 import numpy as np
 
 import myokit
 
-from myokit.tests import DIR_DATA, WarningCollector
+from myokit.tests import DIR_DATA
 
 # Unit testing in Python 2 and 3
 try:
     unittest.TestCase.assertRaisesRegex
 except AttributeError:
     unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
 
@@ -406,445 +405,25 @@
         offset = 0
         for v, t in steps[:-1]:
             offset += t
             e = d.trim(offset - dt, offset + 2 * dt)
             self.assertNotEqual(e['membrane.V'][0], e['membrane.V'][1])
 
 
-@unittest.skipIf(platform.system() != 'Linux', 'Legacy CVODE tests')
-class LegacySimulationTest(PeriodicTest):
-    """
-    Tests myokit.LegacySimulation (which has dynamic, periodic and point-list
-    logging) for consistent log entry timing.
-    """
-    def test_dynamic(self):
-        # Test dynamic logging.
-
-        emax = 1e-6     # Used for equality testing
-        if debug:
-            print('= Simulation :: Dynamic logging =')
-        # Load model & protocol
-        m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
-        # Create simulation
-        s = myokit.LegacySimulation(m, p)
-
-        #
-        # Test 1: Simple 5 ms simulation, log_interval 0.5 ms
-        #
-        d = s.run(50, log=['engine.time'])
-        t = d['engine.time']
-        if debug:
-            print(t[:2])
-            print(t[-2:])
-            print('- ' * 10)
-        # Test first point not double
-        self.assertGreater(t[1], t[0])
-        # Test last point not double
-        self.assertGreater(t[-1], t[-2])
-        # Test first point is 0
-        self.assertTrue(np.abs(t[0] - 0) < emax)
-        # Test last point is 50
-        self.assertTrue(np.abs(t[-1] - 50) < emax)
-
-        #
-        # Test 2: Very short simulation
-        #
-        s.reset()
-        d = s.run(1, log=['engine.time'])
-        t = d['engine.time']
-        if debug:
-            print(t[:2])
-            print(t[-2:])
-            print('- ' * 10)
-        # Test first point not double
-        self.assertGreater(t[1], t[0])
-        # Test last point not double
-        self.assertGreater(t[-1], t[-2])
-        # Test first point is 0
-        self.assertTrue(np.abs(t[0] - 0) < emax)
-        # Test last point is 50
-        self.assertTrue(np.abs(t[-1] - 1) < emax)
-
-        #
-        # Test 3: Stop and start a simulation
-        #
-        s.reset()
-        d = s.run(2, log=['engine.time'])
-        t = d['engine.time']
-        n = len(d['engine.time'])
-        if debug:
-            print(d['engine.time'][:2])
-        # Test first point not double
-        self.assertGreater(t[1], t[0])
-        # Test last point not double
-        self.assertGreater(t[-1], t[-2])
-        # Test first point is 0
-        self.assertTrue(np.abs(t[0] - 0) < emax)
-        # Test last point is 2
-        self.assertTrue(np.abs(t[-1] - 2) < emax)
-        d = s.run(13, log=d)
-        t = d['engine.time']
-        if debug:
-            print(t[n - 2:n + 2])
-        # Test last point not double
-        self.assertGreater(t[-1], t[-2])
-        # Test last point is 2+13
-        self.assertTrue(np.abs(t[-1] - 15) < emax)
-        # Test intermediary points are different
-        self.assertGreater(t[n], t[n - 1])
-        n = len(d['engine.time'])
-        d = s.run(15, log=d)
-        t = d['engine.time']
-        if debug:
-            print(t[n - 2:n + 2])
-        # Test last point not double
-        self.assertGreater(t[-1], t[-2])
-        # Test last point is 2 + 13 + 15
-        self.assertTrue(np.abs(t[-1] - 30) < emax)
-        # Test intermediary points are different
-        self.assertGreater(t[n], t[n - 1])
-        n = len(d['engine.time'])
-        d = s.run(20, log=d)
-        t = d['engine.time']
-        if debug:
-            print(t[n - 2:n + 2])
-            print(t[-2:])
-            print('- ' * 10)
-        # Test last point not double
-        self.assertGreater(t[-1], t[-2])
-        # Test last point is 2 + 13 + 15 + 20
-        self.assertTrue(np.abs(t[-1] - 50) < emax)
-        # Test intermediary points are different
-        self.assertGreater(t[n], t[n - 1])
-
-    def test_periodic(self):
-        # Test periodic logging
-
-        m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
-        s = myokit.LegacySimulation(m, p)
-        self.periodic(s)
-
-    def test_interpolation_and_pacing(self):
-        # Test if interpolation results in correct pacing values.
-
-        # When logging with discontinuous steps, in the adaptive time
-        # CVODE sim, the value of pace must be
-        #  1. The old value *before* the time of the event
-        #  2. The new value *at and after* the time of the event
-        #  3. Back to zero *at and after* the end of the event
-        #     (Unless it ends sooner due to a new event arriving)
-        # Load model
-        m = myokit.load_model('example')
-
-        # Voltage-clamp V (but don't bind it directly)
-        v = m.label('membrane_potential')
-        v.demote()
-        v.set_rhs('-80 + 10 * engine.pace')
-
-        # Create protocol
-        p = myokit.Protocol()
-        p.schedule(level=1, start=0, duration=5, period=10)
-
-        # Create simulation
-        s = myokit.LegacySimulation(m, p)
-
-        # Test if this would result in multiple interpolation steps for logging
-        # i.e. test if the step before each transition was at least 2 log steps
-        # long
-        e = s.run(30).npview()
-        t = e.time()
-        for x in [5, 10, 15, 20, 25]:
-            i = e.find_after(x)
-            if not t[i] - t[i - 1] > 0.2:
-                raise Exception('Issue with test: use longer intervals!')
-        del e, t, x, i
-
-        # Now test if correct interpolated values are returned by periodic
-        # logging.
-        d = s.run(30, log_interval=0.1).npview()
-
-        # Test bound variable
-        p = d['engine.pace']
-        self.assertTrue(np.all(p[0:50] == 1))
-        self.assertTrue(np.all(p[50:100] == 0))
-        self.assertTrue(np.all(p[100:150] == 1))
-        self.assertTrue(np.all(p[150:200] == 0))
-        self.assertTrue(np.all(p[200:250] == 1))
-        self.assertTrue(np.all(p[250:300] == 0))
-
-        # Test variable dependent on bound variable
-        p = d['membrane.V']
-        self.assertTrue(np.all(p[0:50] == -70))
-        self.assertTrue(np.all(p[50:100] == -80))
-        self.assertTrue(np.all(p[100:150] == -70))
-        self.assertTrue(np.all(p[150:200] == -80))
-        self.assertTrue(np.all(p[200:250] == -70))
-        self.assertTrue(np.all(p[250:300] == -80))
-
-    def test_point_list(self):
-        # Test logging with a preset list of points.
-
-        # Load model
-        m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
-        # Create simulation
-        s = myokit.LegacySimulation(m, p)
-
-        # Don't allow decreasing values
-        times = [1, 2, 1]
-        self.assertRaisesRegex(
-            ValueError, 'non-decreasing', s.run, 5, log_times=times)
-
-        # Can't use together with a log interval
-        self.assertRaisesRegex(
-            ValueError, 'simultaneously', s.run, 5, log_interval=1,
-            log_times=[1, 2, 3])
-
-        # Get some odd times
-        times = np.linspace(0, 90, 999)
-
-        # Test!
-        s.reset()
-        d = s.run(100, log_times=times).npview()
-        self.assertTrue(np.all(d.time() == times))
-
-        # Reset and run again
-        s.reset()
-        d = s.run(100, log_times=times).npview()
-        self.assertTrue(np.all(d.time() == times))
-
-        # Run in parts
-        s.reset()
-        d = s.run(50, log_times=times)
-        self.assertEqual(len(d.time()), np.where(times >= 50)[0][0])
-        d = s.run(50, log=d, log_times=times).npview()
-        self.assertTrue(np.all(d.time() == times))
-
-        # Pre-pacing
-        s.reset()
-        s.pre(50)
-        s.run(100, log_times=times)
-        self.assertTrue(np.all(d.time() == times))
-
-        # Partial logging
-        s.reset()
-        s.run(10)
-        d = s.run(10, log_times=times)
-        imin = np.where(times >= 10)[0][0]
-        imax = np.where(times >= 20)[0][0]
-        self.assertEqual(len(d.time()), imax - imin)
-        self.assertTrue(np.all(d.time() == times[imin:imax]))
-        s.run(20)
-        d = s.run(15, log_times=times)
-        imin = np.where(times >= 40)[0][0]
-        imax = np.where(times >= 55)[0][0]
-        self.assertEqual(len(d.time()), imax - imin)
-        self.assertTrue(np.all(d.time() == times[imin:imax]))
-
-        # Get some regular times
-        times = [0, 1, 2, 3, 4, 5]
-        s.reset()
-        d = s.run(6, log_times=times).npview()
-        self.assertEqual(len(d.time()), len(times))
-        self.assertTrue(np.all(d.time() == times))
-
-        # Repeated points
-        times = [0, 0, 0, 5, 5, 5]
-        s.reset()
-        d = s.run(6, log_times=times).npview()
-        self.assertEqual(len(d.time()), len(times))
-        self.assertTrue(np.all(d.time() == times))
-
-        # End points not included, unless also visited!
-        s.reset()
-        s.run(5)
-        d = s.run(5, log_times=times).npview()
-        self.assertEqual(len(d.time()), 3)
-        self.assertTrue(np.all(d.time() == times[3:]))
-        d = s.run(5, log_times=times).npview()
-        self.assertEqual(len(d.time()), 0)
-
-        # Empty list is same as none
-        s.reset()
-        d = s.run(1, log_times=[])
-        self.assertNotEqual(len(d.time()), 0)
-
-    def test_point_list_2(self):
-        # Test how the point-list logging performs when some of the logging
-        # points overlap with protocol change points.
-
-        # Load model
-        m = myokit.load_model(os.path.join(DIR_DATA, 'lr-1991.mmt'))
-        # Voltage clamp
-        m.binding('pace').set_binding(None)
-        v = m.get('membrane.V')
-        v.demote()
-        v.set_rhs(0)
-        v.set_binding('pace')
-        #TODO: Implement chaining like this?
-        #m.get('membrane.V').demote().set_rhs(0).set_binding('pace')
-        # Create step protocol
-        dt = 0.1
-        steps = [
-            [-80, 250.1],
-            [-120, 50],
-            [-80, 200],
-            [40, 1000],
-            [-120, 500],
-            [-80, 1000],
-            [-30, 3500],
-            [-120, 500],
-            [-80, 1000],
-        ]
-        p = myokit.Protocol()
-        for f, t in steps:
-            p.add_step(f, t)
-        # Create set of times that overlap with change points
-        times = np.arange(80000) * dt
-        # Create simulation
-        s = myokit.LegacySimulation(m, p)
-        # Run
-        d = s.run(8000, log_times=times).npview()
-        # Check if logging points show correct pacing value
-        # In an earlier implementation, rounding errors and a difference in the
-        # implementation of passing logpoints and passing protocol points could
-        # cause the log point to be just before the protocol change.
-        # In this case, a change at t=120.0 would only be picked up at t=120.1
-        # (but not consistently!)
-        # The below code checks for this
-        offset = 0
-        for v, t in steps[:-1]:
-            offset += t
-            e = d.trim(offset - dt, offset + 2 * dt)
-            self.assertNotEqual(e['membrane.V'][0], e['membrane.V'][1])
-
-
 class Simulation1dTest(PeriodicTest):
     """
     Tests myokit.Simulation1d for consistent log entry timing.
     """
     def test_periodic(self):
         # Test periodic logging.
 
         m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
         s = myokit.Simulation1d(m, p, ncells=1)
         self.periodic(s)
 
 
-class PSimulationTest(unittest.TestCase):
-    """
-    Tests myokit.PSimulation for consistent log entry timing.
-    """
-    def test_periodic(self):
-        # Test periodic logging.
-
-        m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
-        with WarningCollector():
-            s = myokit.PSimulation(
-                m, p, variables=['membrane.V'], parameters=['ina.gNa'])
-        # Set tolerance for equality testing
-        emax = 1e-2     # Time steps for logging are approximate
-
-        # Test 1: Simple 5 ms simulation, log_interval 0.5 ms
-        d, e = s.run(5, log=['engine.time'], log_interval=0.5)
-        d = d.npview()
-        t = d['engine.time']
-        q = np.arange(0, 5, 0.5)
-        if debug:
-            print(t)
-            print(q)
-            print('- ' * 10)
-        self.assertEqual(len(t), len(q))
-        self.assertTrue(np.max(np.abs(t - q)) < emax)
-
-        # Test 2: Very short simulation
-        s.reset()
-        d, e = s.run(1, log=['engine.time'], log_interval=0.5)
-        d = d.npview()
-        t = d['engine.time']
-        q = np.arange(0, 1, 0.5)
-        if debug:
-            print(t)
-            print(q)
-            print('- ' * 10)
-        self.assertEqual(len(t), len(q))
-        self.assertTrue(np.max(np.abs(t - q)) < emax)
-
-        # Test 3: Stop and start a simulation
-        s.reset()
-        d, e = s.run(1, log=['engine.time'], log_interval=0.5)
-        d, e = s.run(2, log=d, log_interval=0.5)
-        d, e = s.run(2, log=d, log_interval=0.5)
-        d = d.npview()
-        t = d['engine.time']
-        q = np.arange(0, 5, 0.5)
-        if debug:
-            print(t)
-            print(q)
-            print('- ' * 10)
-        self.assertEqual(len(t), len(q))
-        self.assertTrue(np.max(np.abs(t - q)) < emax)
-
-        # Negative or 0 log interval --> Log every step
-        s.set_step_size(0.01)
-        d, dp = s.run(1, log_interval=0)
-        self.assertEqual(len(d.time()), 101)
-        d, dp = s.run(1, log_interval=-1)
-        self.assertEqual(len(d.time()), 101)
-
-
-class ICSimulationTest(unittest.TestCase):
-    """
-    Tests myokit.ICSimulation for consistent log entry timing.
-    """
-    def test_periodic(self):
-        # Test periodic logging.
-
-        m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
-        with WarningCollector():
-            s = myokit.ICSimulation(m, p)
-        # Set tolerance for equality testing
-        emax = 1e-2     # Time steps for logging are approximate
-        # Test 1: Simple 5 ms simulation, log_interval 0.5 ms
-        d, e = s.run(5, log=['engine.time'], log_interval=0.5)
-        d = d.npview()
-        t = d['engine.time']
-        q = np.arange(0, 5, 0.5)
-        if debug:
-            print(t)
-            print(q)
-            print('- ' * 10)
-        self.assertEqual(len(t), len(q))
-        self.assertTrue(np.max(np.abs(t - q)) < emax)
-        # Test 2: Very short simulation
-        s.reset()
-        d, e = s.run(1, log=['engine.time'], log_interval=0.5)
-        d = d.npview()
-        t = d['engine.time']
-        q = np.arange(0, 1, 0.5)
-        if debug:
-            print(t)
-            print(q)
-            print('- ' * 10)
-        self.assertEqual(len(t), len(q))
-        self.assertTrue(np.max(np.abs(t - q)) < emax)
-        # Test 3: Stop and start a simulation
-        s.reset()
-        d, e = s.run(1, log=['engine.time'], log_interval=0.5)
-        d, e = s.run(2, log=d, log_interval=0.5)
-        d, e = s.run(2, log=d, log_interval=0.5)
-        d = d.npview()
-        t = d['engine.time']
-        q = np.arange(0, 5, 0.5)
-        if debug:
-            print(t)
-            print(q)
-            print('- ' * 10)
-        self.assertEqual(len(t), len(q))
-        self.assertTrue(np.max(np.abs(t - q)) < emax)
-
-
 if __name__ == '__main__':
     print('Add -v for more debug output')
     import sys
     if '-v' in sys.argv:
         debug = True
     unittest.main()
```

### Comparing `myokit-1.33.9/myokit/tests/test_simulation_opencl.py` & `myokit-1.34.0/myokit/tests/test_simulation_opencl.py`

 * *Files 2% similar despite different names*

```diff
@@ -617,15 +617,15 @@
 
         # Check that various methods are now unavailable
         self.assertRaisesRegex(
             RuntimeError, 'method is unavailable', s.conductance)
         self.assertRaisesRegex(
             RuntimeError, 'method is unavailable', s.is_paced, 0)
         self.assertRaisesRegex(
-            RuntimeError, 'method is unavailable', s.neighbours, 0)
+            RuntimeError, 'method is unavailable', s.neighbors, 0)
         self.assertRaisesRegex(
             RuntimeError, 'method is unavailable', s.set_conductance)
         self.assertRaisesRegex(
             RuntimeError, 'method is unavailable', s.set_connections, [])
         self.assertRaisesRegex(
             RuntimeError, 'method is unavailable', s.set_paced_cells)
         self.assertRaisesRegex(
@@ -662,130 +662,160 @@
         d = s.run(10, log=['membrane.V']).npview()
         self.assertGreater(np.max(d['membrane.V', 0]), 0)
         self.assertGreater(np.max(d['membrane.V', 1]), 0)
         self.assertGreater(np.max(d['membrane.V', 2]), 0)
         self.assertTrue(np.all(d['membrane.V', 0] == d['membrane.V', 1]))
         self.assertTrue(np.all(d['membrane.V', 0] == d['membrane.V', 2]))
 
-    def test_neighbours_0d(self):
-        # Test listing neighbours in a 0d simulation
+    def test_initial_value_expressions(self):
+        # Test if initial value expressions are converted to floats
+        m = myokit.parse_model('''
+            [[model]]
+            c.x = 1 + sqrt(3)
+            c.y = 1 / c.p
+            c.z = 3
+
+            [c]
+            t = 0 bind time
+            dot(x) = 1 label membrane_potential
+            dot(y) = 2
+            dot(z) = 3
+            p = log(3)
+            q = 0 bind diffusion_current
+        ''')
+        s = myokit.SimulationOpenCL(m, ncells=2)
+        x = s.state()
+        self.assertIsInstance(x[0], float)
+        self.assertIsInstance(x[1], float)
+        self.assertIsInstance(x[2], float)
+        self.assertEqual(x[:3], x[3:])
+        self.assertEqual(x, m.initial_values(True) * 2)
+        self.assertEqual(x, s.default_state())
 
-        x = self.s0.neighbours(0)
+    def test_neighbors_0d(self):
+        # Test listing neighbors in a 0d simulation
+
+        x = self.s0.neighbors(0)
         self.assertEqual(len(x), 0)
         self.assertRaisesRegex(
-            IndexError, 'out of range', self.s0.neighbours, -1)
+            IndexError, 'out of range', self.s0.neighbors, -1)
         self.assertRaisesRegex(
-            IndexError, 'out of range', self.s0.neighbours, 1)
+            IndexError, 'out of range', self.s0.neighbors, 1)
         self.assertRaisesRegex(
-            ValueError, '1-dimensional', self.s0.neighbours, 0, 1)
+            ValueError, '1-dimensional', self.s0.neighbors, 0, 1)
+
+        # Test alias
+        with WarningCollector() as w:
+            self.assertEqual(self.s0.neighbours(0), self.s0.neighbors(0))
+        self.assertIn('deprecated', w.text())
 
-    def test_neighbours_1d(self):
-        # Test listing neighbours in a 1d simulation
+    def test_neighbors_1d(self):
+        # Test listing neighbors in a 1d simulation
 
         # Left edge
-        x = self.s1.neighbours(0)
+        x = self.s1.neighbors(0)
         self.assertEqual(len(x), 1)
         self.assertIn(1, x)
         # Middle
-        x = self.s1.neighbours(1)
+        x = self.s1.neighbors(1)
         self.assertEqual(len(x), 2)
         self.assertIn(0, x)
         self.assertIn(2, x)
         # Right edge
-        x = self.s1.neighbours(9)
+        x = self.s1.neighbors(9)
         self.assertEqual(len(x), 1)
         self.assertIn(8, x)
 
         # Out of range
         self.assertRaisesRegex(
-            IndexError, 'out of range', self.s1.neighbours, -1)
+            IndexError, 'out of range', self.s1.neighbors, -1)
         self.assertRaisesRegex(
-            IndexError, 'out of range', self.s1.neighbours, 10)
+            IndexError, 'out of range', self.s1.neighbors, 10)
         self.assertRaisesRegex(
-            ValueError, '1-dimensional', self.s1.neighbours, 0, 1)
+            ValueError, '1-dimensional', self.s1.neighbors, 0, 1)
 
-    def test_neighbours_1d_connections(self):
-        # Test listing neighbours in a 1d simulation with arbitrary geometry
+    def test_neighbors_1d_connections(self):
+        # Test listing neighbors in a 1d simulation with arbitrary geometry
 
         try:
             g = 1
             self.s1.set_connections(
                 [(0, 1, g), (0, 2, g), (3, 0, g), (3, 2, g)])
-            x = self.s1.neighbours(0)
+            x = self.s1.neighbors(0)
             self.assertEqual(len(x), 3)
             self.assertIn(1, x)
             self.assertIn(2, x)
             self.assertIn(3, x)
-            x = self.s1.neighbours(1)
+            x = self.s1.neighbors(1)
             self.assertEqual(len(x), 1)
             self.assertIn(0, x)
-            x = self.s1.neighbours(2)
+            x = self.s1.neighbors(2)
             self.assertEqual(len(x), 2)
             self.assertIn(0, x)
             self.assertIn(3, x)
-            x = self.s1.neighbours(3)
+            x = self.s1.neighbors(3)
             self.assertEqual(len(x), 2)
             self.assertIn(0, x)
             self.assertIn(2, x)
-            x = self.s1.neighbours(4)
+            x = self.s1.neighbors(4)
             self.assertEqual(len(x), 0)
         finally:
             # Restore defaults
             self.s1.set_conductance()
 
-    def test_neighbours_2d(self):
-        # Test listing neighbours in a 2d simulation
+    def test_neighbors_2d(self):
+        # Test listing neighbors in a 2d simulation
 
         # Corners
-        x = self.s2.neighbours(0, 0)
+        x = self.s2.neighbors(0, 0)
         self.assertEqual(len(x), 2)
         self.assertIn((1, 0), x)
         self.assertIn((0, 1), x)
-        x = self.s2.neighbours(3, 2)
+        x = self.s2.neighbors(3, 2)
         self.assertEqual(len(x), 2)
         self.assertIn((3, 1), x)
         self.assertIn((2, 2), x)
 
         # Edges
-        x = self.s2.neighbours(1, 0)
+        x = self.s2.neighbors(1, 0)
         self.assertEqual(len(x), 3)
         self.assertIn((0, 0), x)
         self.assertIn((2, 0), x)
         self.assertIn((1, 1), x)
-        x = self.s2.neighbours(3, 1)
+        x = self.s2.neighbors(3, 1)
         self.assertEqual(len(x), 3)
         self.assertIn((2, 1), x)
         self.assertIn((3, 0), x)
         self.assertIn((3, 2), x)
 
         # Middle
-        x = self.s2.neighbours(1, 1)
+        x = self.s2.neighbors(1, 1)
         self.assertEqual(len(x), 4)
         self.assertIn((0, 1), x)
         self.assertIn((2, 1), x)
         self.assertIn((1, 0), x)
         self.assertIn((1, 2), x)
-        x = self.s2.neighbours(2, 1)
+        x = self.s2.neighbors(2, 1)
         self.assertEqual(len(x), 4)
         self.assertIn((1, 1), x)
         self.assertIn((3, 1), x)
         self.assertIn((2, 0), x)
         self.assertIn((2, 2), x)
 
         # Out of range
         self.assertRaisesRegex(
-            IndexError, 'out of range', self.s2.neighbours, -1, 0)
+            IndexError, 'out of range', self.s2.neighbors, -1, 0)
         self.assertRaisesRegex(
-            IndexError, 'out of range', self.s2.neighbours, 0, -1)
+            IndexError, 'out of range', self.s2.neighbors, 0, -1)
         self.assertRaisesRegex(
-            IndexError, 'out of range', self.s2.neighbours, 4, 0)
+            IndexError, 'out of range', self.s2.neighbors, 4, 0)
         self.assertRaisesRegex(
-            IndexError, 'out of range', self.s2.neighbours, 0, 3)
+            IndexError, 'out of range', self.s2.neighbors, 0, 3)
         self.assertRaisesRegex(
-            ValueError, '2-dimensional', self.s2.neighbours, 0)
+            ValueError, '2-dimensional', self.s2.neighbors, 0)
 
     def test_protocol(self):
         # Tests changing the protocol
 
         # Run with protocol, check for depolarisation
         self.s0.reset()
         d0 = self.s0.run(3, log=['engine.pace']).npview()
@@ -1176,15 +1206,15 @@
     def test_set_state_1d(self):
         # Test the set_state methods on a 1d simulation (interface only)
 
         # Check simulation state equals model state
         m = 8
         n = 10
         self.s1.reset()
-        sm = self.m.state()
+        sm = self.m.initial_values(True)
         ss = [self.s1.state(x) for x in range(n)]
         for si in ss:
             self.assertEqual(sm, si)
 
         # Test setting a full-sized state
         sx = list(range(n * m))
         self.s1.set_state(sx)
@@ -1273,15 +1303,15 @@
     def test_set_state_2d(self):
         # Test the set_state methods on a 2d simulation (interface only)
 
         # Check simulation state equals model state
         m = 8
         nx, ny = 4, 3
         self.s2.reset()
-        sm = self.m.state()
+        sm = self.m.initial_values(True)
         for i in range(nx):
             for j in range(ny):
                 self.assertEqual(sm, self.s2.state(i, j))
 
         # Test setting a full-sized state
         sx = list(range(nx * ny * m))
         self.s2.set_state(sx)
```

### Comparing `myokit-1.33.9/myokit/tests/test_simulation_opencl_vs_cvode.py` & `myokit-1.34.0/myokit/tests/test_simulation_opencl_vs_cvode.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_simulation_opencl_vs_sim1d.py` & `myokit-1.34.0/myokit/tests/test_simulation_opencl_vs_sim1d.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_system_info.py` & `myokit-1.34.0/myokit/tests/test_system_info.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_tools.py` & `myokit-1.34.0/myokit/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_unit.py` & `myokit-1.34.0/myokit/tests/test_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         pF2 = myokit.units.pF**2
         not_pF2 = pF2 * 1.0001
         self.assertTrue(myokit.Unit.close(pF2, pF2))
         self.assertTrue(myokit.Unit.close(not_pF2, not_pF2))
         self.assertFalse(myokit.Unit.close(not_pF2, pF2))
         self.assertFalse(myokit.Unit.close(pF2, not_pF2))
 
-        # The next test is not a requirement, but tests the current behaviour:
+        # The next test is not a requirement, but tests the current behavior:
         u = myokit.units.m * 1.000000001
         self.assertTrue(myokit.Unit.close(u, myokit.units.m))
 
     def test_conversion_factor(self):
         # Test :meth:`Unit.conversion_factor()`.
 
         cf = myokit.Unit.conversion_factor
```

### Comparing `myokit-1.33.9/myokit/tests/test_user_functions.py` & `myokit-1.34.0/myokit/tests/test_user_functions.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/tests/test_variable.py` & `myokit-1.34.0/myokit/tests/test_variable.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,30 +4,35 @@
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
 from __future__ import absolute_import, division
 from __future__ import print_function, unicode_literals
 
-import myokit
-import numpy as np
 import unittest
 
+import numpy as np
+
+import myokit
+
+from myokit.tests import WarningCollector
+
 
 # Unit testing in Python 2 and 3
 try:
     unittest.TestCase.assertRaisesRegex
 except AttributeError:
     unittest.TestCase.assertRaisesRegex = unittest.TestCase.assertRaisesRegexp
 
 
 class VariableTest(unittest.TestCase):
     """
     Tests parts of :class:`myokit.Variable`.
     """
+
     def test_clamp(self):
         # Tests clamping a variable to a fixed value
         m = myokit.parse_model("""
             [[model]]
             z.g = 2
             z.h = 6.123
             z.p = 1.5
@@ -88,15 +93,15 @@
         self.assertRaises(KeyError, m.get, 'z.d.e')
         self.assertRaises(KeyError, m.get, 'z.d.f')
         del d
 
         # Clamp simple state
         g = m.get('z.g')
         self.assertTrue(g.is_state())
-        self.assertTrue(g.state_value() != 10)
+        self.assertNotEqual(g.initial_value(True), 10)
         self.assertEqual(g.unit(), myokit.units.m)
         self.assertEqual(g.rhs().unit(), myokit.units.m / myokit.units.s)
         self.assertEqual(m.count_states(), 3)
         g.clamp(10)
         self.assertTrue(g.is_literal())
         self.assertFalse(g.is_state())
         self.assertEqual(g.rhs(), myokit.Number(10, myokit.units.m))
@@ -154,24 +159,27 @@
 
     def test_convert_unit(self):
         # Test changing variable units
 
         m = myokit.parse_model("""
             [[model]]
             membrane.V = -83
+            membrane.w = 10
 
             [env]
             t = 0 [ms] bind time
                 in [ms]
 
             [membrane]
             dot(V) = - (ikr.i + ina.i * 1 [cm^2/uF])
                 in [mV]
             dotv = 5 [mV/ms] + dot(V)
                 in [mV/ms]
+            dot(w) = 0.1 [mg/ms]
+                in [mg]
 
             [cell]
             Cm = 0.123 [uF]
                 in [uF]
 
             [ina]
             i = 12 [uA/cm^2]
@@ -190,25 +198,47 @@
 
         # Convert to same
         code = m.code()
         v = m.get('membrane.V')
         v.convert_unit('mV')
         self.assertEqual(code, m.code())
 
-        # Convert state
+        # Convert state (note: initial value is treated as PrefixMinus expr!)
         vdot = v.rhs().eval()
         self.assertNotEqual(v.unit(), myokit.units.V)
         v.convert_unit('V')
         self.assertEqual(v.unit(), myokit.units.V)
 
         # Check dot(v) is the same, and all units are compatible
         vdot /= 1000
         self.assertEqual(vdot, v.rhs().eval())
         m.check_units(myokit.UNIT_STRICT)
 
+        # Check units of the initial value have been converted
+        self.assertEqual(v.initial_value(True), -0.083)
+        # Not sure if this one is desirable, but -83 is parsed as the
+        # expression -(83)
+        self.assertEqual(
+            v.initial_value(),
+            myokit.Multiply(
+                myokit.PrefixMinus(myokit.Number(83)),
+                myokit.Number(0.001, myokit.units.V / myokit.units.mV)))
+
+        # Convert state with number initial value
+        w = m.get('membrane.w')
+        wdot = w.rhs().eval()
+        w.convert_unit('ug')
+        self.assertEqual(w.unit(), myokit.units.g / 1e6)
+        self.assertEqual(wdot * 1000, w.rhs().eval())
+        m.check_units(myokit.UNIT_STRICT)
+        self.assertEqual(w.initial_value(True), 10000)
+        self.assertEqual(w.initial_value(), myokit.Number(10000))
+        #self.assertEqual(
+        #    w.initial_value(), myokit.Number(10000, myokit.units.g / 1e6))
+
         # Convert non-state
         i = m.get('ina.i')
         self.assertNotEqual(i.unit(), myokit.parse_unit('uA/uF'))
         i.convert_unit('uA/uF', ['1 [uF/cm^2]'])
         self.assertEqual(i.unit(), myokit.parse_unit('uA/uF'))
 
         # Check dot(v) is the same, and all units are compatible
@@ -222,14 +252,80 @@
         self.assertEqual(t.unit(), myokit.units.s)
 
         # Check dot(v) is the same, and all units are compatible
         vdot *= 1000
         self.assertEqual(vdot, v.rhs().eval())
         m.check_units(myokit.UNIT_STRICT)
 
+    def test_index(self):
+        # Tests the index() method
+
+        m = myokit.Model()
+        c = m.add_component('c')
+        a = c.add_variable('a')
+        a.set_rhs(0)
+        a.promote(0)
+        b = c.add_variable('b')
+        b.set_rhs(0)
+        b.promote(0)
+
+        self.assertEqual(a.index(), 0)
+        self.assertEqual(b.index(), 1)
+        m.reorder_state((b, a))
+        self.assertEqual(a.index(), 1)
+        self.assertEqual(b.index(), 0)
+
+        # Test deprecated alias
+        with WarningCollector() as w:
+            self.assertEqual(a.indice(), 1)
+        self.assertIn('deprecated', w.text())
+
+    def test_initial_value(self):
+        # Tests :meth:`Variable.initial_value`.
+
+        m = myokit.parse_model('''
+            [[model]]
+            c.x = 2
+
+            [c]
+            t = 0 bind time
+            dot(x) = 0
+            p = 3
+            q = 4
+        ''')
+
+        # Test expression version
+        x, p = m.get('c.x'), m.get('c.p')
+        p = m.get('c.p')
+        self.assertEqual(x.initial_value(), myokit.Number(2))
+        x.set_initial_value(3)
+        self.assertEqual(x.initial_value(), myokit.Number(3))
+        x.set_initial_value('3 [kg]')
+        self.assertEqual(x.initial_value(), myokit.Number(3, myokit.units.kg))
+        x.set_initial_value('sqrt(c.p) / log(c.p)')
+        self.assertEqual(x.initial_value(), myokit.Divide(
+            myokit.Sqrt(p.lhs()), myokit.Log(p.lhs())))
+
+        # Test float version
+        p.set_rhs(9)
+        x.set_initial_value('1 + sqrt(c.p)')
+        self.assertEqual(x.initial_value(True), 4)
+
+        # Test deprecated alias
+        with WarningCollector() as w:
+            self.assertEqual(x.state_value(), x.initial_value(True))
+        self.assertIn('deprecated', w.text())
+
+        # Test cycles are detected
+        p.set_rhs('1 - 2 * q')
+        m.get('c.q').set_rhs('7 * sqrt(p)')
+        x.initial_value()  # No evaluation, so no error
+        self.assertRaises(
+            myokit.CyclicalDependencyError, x.initial_value, as_float=True)
+
     def test_is_referenced(self):
         # Test :meth:`Variable.is_referenced().
 
         m = myokit.Model()
         c = m.add_component('c')
         v = c.add_variable('v')
         v.set_rhs(3)
@@ -272,68 +368,92 @@
         self.assertIsNone(v.label())
 
     def test_promote_demote(self):
         # Test variable promotion and demotion.
 
         m = myokit.Model()
         c = m.add_component('c')
+        p = c.add_variable('p')
+        p.set_rhs(1)
         v = c.add_variable('v')
         v.set_rhs(3)
 
         self.assertTrue(v.is_literal())
         self.assertTrue(v.is_constant())
         self.assertFalse(v.is_intermediary())
         self.assertFalse(v.is_state())
         self.assertEqual(v.lhs(), myokit.Name(v))
         self.assertRaises(Exception, v.demote)
-        self.assertRaises(Exception, v.indice)
-        self.assertRaises(Exception, v.state_value)
+        self.assertRaises(Exception, v.index)
+        self.assertRaises(Exception, v.initial_value)
 
         v.promote(3)
         self.assertFalse(v.is_literal())
         self.assertFalse(v.is_constant())
         self.assertFalse(v.is_intermediary())
         self.assertTrue(v.is_state())
         self.assertEqual(v.lhs(), myokit.Derivative(myokit.Name(v)))
-        self.assertEqual(v.indice(), 0)
-        self.assertEqual(v.state_value(), 3)
+        self.assertEqual(v.index(), 0)
+        self.assertEqual(v.initial_value(), myokit.Number(3))
 
         v.demote()
         self.assertTrue(v.is_literal())
         self.assertTrue(v.is_constant())
         self.assertFalse(v.is_intermediary())
         self.assertFalse(v.is_state())
         self.assertEqual(v.lhs(), myokit.Name(v))
         self.assertRaises(Exception, v.demote)
-        self.assertRaises(Exception, v.indice)
-        self.assertRaises(Exception, v.state_value)
+        self.assertRaises(Exception, v.index)
+        self.assertRaises(Exception, v.initial_value)
 
         # Test errors
         v.promote(3)
         self.assertRaisesRegex(Exception, 'already', v.promote, 4)
         v.demote()
         v.set_binding('time')
         self.assertRaisesRegex(Exception, 'cannot be bound', v.promote, 4)
         w = v.add_variable('w')
         self.assertRaisesRegex(
             Exception, 'only be added to Components', w.promote, 4)
 
+        # Test that promote accepts expressions and strings
+        v.set_binding(None)
+        v.remove_variable(w)
+        v.promote(myokit.Number(3, myokit.units.kg))
+        self.assertEqual(v.initial_value(), myokit.Number(3, myokit.units.kg))
+        v.demote()
+        v.promote('1 + c.p')
+        self.assertEqual(v.initial_value().code(), '1 + c.p')
+        v.demote()
+
+        # Test that promote only works with global syntax references
+        self.assertRaisesRegex(myokit.ParseError, 'Unresolved', v.promote, 'p')
+
         # Test we can't demote a variable with references to its derivative
         m = myokit.Model()
         c = m.add_component('c')
         x = c.add_variable('x')
         x.set_rhs(3)
         x.promote()
         y = c.add_variable('y')
         y.set_rhs('1 + dot(x)')
         self.assertRaisesRegex(
             Exception, 'references to its derivative', x.demote)
         y.set_rhs('1 + x')
         x.demote()
 
+        # Test deprecated keyword argument
+        with WarningCollector() as w:
+            x.promote(state_value=3)
+        self.assertIn('deprecated', w.text())
+        self.assertEqual(x.initial_value(), myokit.Number(3))
+        x.demote()
+        self.assertRaisesRegex(
+            Exception, 'at the same time as', x.promote, 3, state_value=3)
+
     def test_pyfunc(self):
         # Test :meth:`Variable.pyfunc().
 
         m = myokit.Model()
         c = m.add_component('c')
         x = c.add_variable('x')
         x.set_rhs(3)
@@ -634,39 +754,80 @@
         m = myokit.Model()
         c = m.add_component('c')
         v = c.add_variable('v')
         v.rename('w')
         self.assertEqual(v.name(), 'w')
         self.assertEqual(v.qname(), 'c.w')
 
-    def test_set_state_value(self):
-        # Test :meth:`Variable.set_state_value()`.
+    def test_set_initial_value(self):
+        # Test :meth:`Variable.set_initial_value()`.
 
         m = myokit.Model()
         c = m.add_component('c')
+        t = c.add_variable('t')
+        t.set_rhs(0)
+        t.set_binding('time')
         v = c.add_variable('v')
+        v.set_rhs(3)
         w = c.add_variable('w')
+        w.set_rhs('1 + 2')
+        m.validate()
 
         # Test basic functionality
         v.promote(10)
-        self.assertEqual(v.state_value(), 10)
-        v.set_state_value(12)
-        self.assertEqual(v.state_value(), 12)
+        self.assertEqual(v.initial_value(), myokit.Number(10))
+        v.set_initial_value(myokit.Number(12, myokit.units.g))
+        self.assertEqual(v.initial_value(), myokit.Number(12, myokit.units.g))
+
+        # Test setting expressions
+        v.set_initial_value('1 + 11')
+        #self.assertEqual(v.initial_value(),
+        #                 myokit.Plus(myokit.Number(1), myokit.Number(11)))
+        v.set_initial_value('1 + c.w')
+        self.assertEqual(v.initial_value(),
+                         myokit.Plus(myokit.Number(1), myokit.Name(w)))
+
+        # Strings must use global context
+        self.assertRaisesRegex(myokit.ParseError, 'No component specified for',
+                               v.set_initial_value, '1 / w')
 
         # Only states have this option
         v.demote()
         self.assertRaisesRegex(
-            Exception, 'Only state variables', v.set_state_value, 3)
+            Exception, 'Only state variables', v.set_initial_value, 3)
         self.assertRaisesRegex(
-            Exception, 'Only state variables', w.set_state_value, 3)
-
-        # State values must be literals
+            Exception, 'Only state variables', w.set_initial_value, 3)
         v.promote(3)
+        m.validate()
+
+        # Initial values must be constant, but this is only picked up in
+        # validation
+        w.promote(1)
+        v.set_initial_value(myokit.Name(w))
+        self.assertRaises(myokit.IntegrityError, m.validate)
+        w.demote()
+        m.validate()
+
+        # Nested variables may not be used, but this is only picked up when
+        # validating
+        x = v.add_variable('x')
+        x.set_rhs(1)
+        v.set_initial_value(x.lhs())
         self.assertRaises(
-            myokit.NonLiteralValueError, v.set_state_value, w.lhs())
+            myokit.IllegalReferenceInInitialValueError, m.validate)
+        v.set_initial_value(x)
+
+        # InitialValue and PartialDerivative can not be used
+        v.set_initial_value(myokit.PartialDerivative(v.lhs(), x.lhs()))
+
+        # Deprecated alias
+        with WarningCollector() as w:
+            v.set_state_value(1)
+        self.assertIn('deprecated', w.text())
+        self.assertEqual(v.initial_value(), myokit.Number(1))
 
     def test_set_unit(self):
         # Test :meth:`Variable.set_unit()`.
         m = myokit.Model()
         c = m.add_component('c')
         v = c.add_variable('v')
 
@@ -741,14 +902,67 @@
         p.promote(1)
         p.set_rhs(myokit.InitialValue(myokit.Name(p)))
         self.assertRaisesRegex(
             myokit.IntegrityError, 'Initial value', p.validate)
         p.set_rhs('q == 3')
         self.assertRaisesRegex(
             myokit.IntegrityError, 'can not be a condition', p.validate)
+        p.set_rhs(3)
+        p.validate()
+
+        # Initial value can not reference nested variables
+        r = c.add_variable('r')
+        r1 = r.add_variable('r1')
+        r1.set_rhs(1)
+        r.set_rhs('1 + r1')
+        p.validate()
+        p.set_initial_value(myokit.Plus(myokit.Number(1), myokit.Name(r1)))
+        self.assertRaises(
+            myokit.IllegalReferenceInInitialValueError, p.validate)
+
+        # Initial value must be constant
+        p.set_initial_value('1 / c.q')
+        q.promote(3)
+        self.assertRaisesRegex(myokit.IntegrityError, 'not const', p.validate)
+        q.demote()
+        p.validate()
+        q.set_rhs('1 + c.p')
+        self.assertRaisesRegex(myokit.IntegrityError, 'not const', p.validate)
+        q.set_rhs(10)
+        p.validate()
+        q.set_binding('hello')
+        self.assertRaisesRegex(myokit.IntegrityError, 'not const', p.validate)
+        # Don't test everything, is_const() should work!
+
+        # Initial value cannot be a partial, init, or condition
+        p.set_initial_value(myokit.PartialDerivative(p.lhs(), q.lhs()))
+        self.assertRaisesRegex(
+            myokit.IntegrityError, 'Partial derivatives', p.validate)
+        p.set_initial_value(myokit.InitialValue(myokit.Name(p)))
+        self.assertRaisesRegex(
+            myokit.IntegrityError, 'Initial value', p.validate)
+        p.set_initial_value('c.q == 3')
+        self.assertRaisesRegex(
+            myokit.IntegrityError, 'can not be a condition', p.validate)
+
+        # Initial value cycles are caught in validation, don't cause loops
+        m = myokit.parse_model('''
+            [[model]]
+            x.x = 0
+            [x]
+            dot(x) = x
+            t = 0 bind time
+            ''')
+        x = m.get('x.x')
+        x.set_initial_value('x.x')
+        self.assertRaisesRegex(myokit.IntegrityError, 'not const', m.validate)
+        x.set_initial_value(1)
+        m.validate()
+        x.set_initial_value('1 + 1 / x.x')
+        self.assertRaisesRegex(myokit.IntegrityError, 'not const', m.validate)
 
     def test_value(self):
         # Test :meth:`Variable.value()`.
 
         m = myokit.Model()
         c = m.add_component('c')
         v = c.add_variable('v')
```

### Comparing `myokit-1.33.9/myokit/tools.py` & `myokit-1.34.0/myokit/tools.py`

 * *Files identical despite different names*

### Comparing `myokit-1.33.9/myokit/units.py` & `myokit-1.34.0/myokit/units.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,14 +259,15 @@
 _rep('nL')
 _rep('pL')
 # Concentrations
 _rep('M')
 _rep('mM')
 _rep('mM^2')
 _rep('mM^3')
+_rep('mM^4')
 _rep('uM')
 _rep('1/mM/ms')
 _rep('1/mM^2/ms')
 _rep('mM/ms')
 _rep('mM/mV/ms')
 # Voltages
 _rep('1/mV')
@@ -280,19 +281,23 @@
 _rep('uA/cm^2')
 _rep('pA/cm^2')
 # Conductances and permeability
 _rep('S/F')
 _rep('mS/uF')
 _rep('mS/cm^2')
 _rep('mS/mm^2')
+_rep('L/F/s')
 _rep('L/F/ms')
 _rep('mA/cm^2')
 # Capacitance
 _rep('cm^2/uF')
 _rep('uF/cm^2')
 _rep('uF/mm^2')
 _rep('uF*mol/C')
 # Various
 _rep('J/mol/K')
 _rep('mJ/mol/K')
 _rep('C/mol')
 _rep('C/mmol')
+_rep('J/K')  # Boltzmann
+_rep('J*s')  # Planck
+_rep('J*ms')
```

### Comparing `myokit-1.33.9/myokit.egg-info/PKG-INFO` & `myokit-1.34.0/myokit.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: myokit
-Version: 1.33.9
+Version: 1.34.0
 Summary: A simple interface to cardiac cellular electrophysiology
 Home-page: http://myokit.org
 Author: Michael Clerx
 Author-email: michael@myokit.org
 License: BSD 3-clause license
 Project-URL: Bug Tracker, https://github.com/MichaelClerx/myokit/issues
 Project-URL: Documentation, http://docs.myokit.org
 Project-URL: Source Code, https://github.com/MichaelClerx/myokit
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
@@ -27,18 +26,18 @@
 Provides-Extra: dev
 Provides-Extra: optional
 Provides-Extra: gui
 Provides-Extra: pyqt
 Provides-Extra: pyside
 License-File: LICENSE.txt
 
-[![Ubuntu unit tests](https://github.com/MichaelClerx/myokit/workflows/Ubuntu%20unit%20tests/badge.svg)](https://github.com/MichaelClerx/myokit/actions?query=workflow%3A"Ubuntu+unit+tests")
-[![MacOS unit tests](https://github.com/MichaelClerx/myokit/workflows/MacOS%20unit%20tests/badge.svg)](https://github.com/MichaelClerx/myokit/actions?query=workflow%3A"MacOS+unit+tests")
-[![Windows unit tests](https://github.com/MichaelClerx/myokit/workflows/Windows%20unit%20tests/badge.svg)](https://github.com/MichaelClerx/myokit/actions?query=workflow%3A"Windows+unit+tests")
-[![Windows Miniconda test](https://github.com/MichaelClerx/myokit/workflows/Windows%20Miniconda%20test/badge.svg)](https://github.com/MichaelClerx/myokit/actions?query=workflow%3A"Windows+Miniconda+test")
+[![Ubuntu unit tests](https://github.com/myokit/myokit/actions/workflows/unit-tests-ubuntu.yml/badge.svg)](https://github.com/myokit/myokit/actions/workflows/unit-tests-ubuntu.yml)
+[![MacOS unit tests](https://github.com/myokit/myokit/actions/workflows/unit-tests-macos.yml/badge.svg)](https://github.com/myokit/myokit/actions/workflows/unit-tests-macos.yml)
+[![Windows unit tests](https://github.com/myokit/myokit/actions/workflows/unit-tests-windows.yml/badge.svg)](https://github.com/myokit/myokit/actions/workflows/unit-tests-windows.yml)
+[![Windows Miniconda test](https://github.com/myokit/myokit/actions/workflows/unit-tests-windows-miniconda.yml/badge.svg)](https://github.com/myokit/myokit/actions/workflows/unit-tests-windows-miniconda.yml)
 [![codecov](https://codecov.io/gh/myokit/myokit/branch/main/graph/badge.svg)](https://codecov.io/gh/myokit/myokit)
 [![Documentation Status](https://readthedocs.org/projects/myokit/badge/?version=latest)](https://myokit.readthedocs.io/?badge=latest)
 
 ![Myokit](http://myokit.org/static/img/logo.png)
 
 [Myokit](http://myokit.org) is an [open-source](https://github.com/MichaelClerx/myokit/blob/main/LICENSE.txt) Python-based toolkit that facilitates modeling and simulation of cardiac cellular electrophysiology.
 It's hosted on [GitHub](https://github.com/MichaelClerx/myokit/) and available on [PyPi](https://pypi.org/project/myokit/).
@@ -103,9 +102,7 @@
 
 
 ## Citing Myokit
 
 If you use Myokit in your research, please cite it using the information in our [CITATION file](https://github.com/MichaelClerx/myokit/blob/main/CITATION).
 
 I like to [keep track of who's using Myokit](http://myokit.org/publications/) (for my CV!). If you are using Myokit for teaching, I'd love to hear about it. You can drop me a line at michael[at]myokit.org.
-
-
```

### Comparing `myokit-1.33.9/myokit.egg-info/SOURCES.txt` & `myokit-1.34.0/myokit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -94,34 +94,28 @@
 myokit/_sim/__init__.py
 myokit/_sim/cable.c
 myokit/_sim/cable.py
 myokit/_sim/cmodel.h
 myokit/_sim/cmodel.py
 myokit/_sim/compiler.c
 myokit/_sim/compiler.py
-myokit/_sim/cvodesim.c
-myokit/_sim/cvodesim.py
 myokit/_sim/cvodessim.c
 myokit/_sim/cvodessim.py
 myokit/_sim/differential.hpp
 myokit/_sim/fiber_tissue.c
 myokit/_sim/fiber_tissue.py
-myokit/_sim/icsim.cpp
-myokit/_sim/icsim.py
 myokit/_sim/jacobian.cpp
 myokit/_sim/jacobian.py
 myokit/_sim/mcl.h
 myokit/_sim/opencl.c
 myokit/_sim/opencl.py
 myokit/_sim/openclsim.c
 myokit/_sim/openclsim.cl
 myokit/_sim/openclsim.py
 myokit/_sim/pacing.h
-myokit/_sim/psim.cpp
-myokit/_sim/psim.py
 myokit/_sim/rhs.c
 myokit/_sim/rhs.py
 myokit/_sim/sundials.c
 myokit/_sim/sundials.py
 myokit/formats/__init__.py
 myokit/formats/ansic/__init__.py
 myokit/formats/ansic/_ewriter.py
@@ -176,15 +170,15 @@
 myokit/formats/opencl/__init__.py
 myokit/formats/opencl/_ewriter.py
 myokit/formats/opencl/_exporter.py
 myokit/formats/opencl/template/cable.c
 myokit/formats/opencl/template/kernel.cl
 myokit/formats/opencl/template/minilog.py
 myokit/formats/opencl/template/plot.py
-myokit/formats/opencl/template/test
+myokit/formats/opencl/template/test.sh
 myokit/formats/python/__init__.py
 myokit/formats/python/_ewriter.py
 myokit/formats/python/_exporter.py
 myokit/formats/python/template/sim.py
 myokit/formats/sbml/__init__.py
 myokit/formats/sbml/_api.py
 myokit/formats/sbml/_importer.py
@@ -207,15 +201,14 @@
 myokit/gui/datalog_viewer.py
 myokit/gui/explorer.py
 myokit/gui/ide.py
 myokit/gui/progress.py
 myokit/gui/source.py
 myokit/gui/vargrapher.py
 myokit/lib/__init__.py
-myokit/lib/common.py
 myokit/lib/deps.py
 myokit/lib/guess.py
 myokit/lib/hh.py
 myokit/lib/markov.py
 myokit/lib/multi.py
 myokit/lib/plots.py
 myokit/tests/__init__.py
@@ -251,15 +244,14 @@
 myokit/tests/test_formats_opencl.py
 myokit/tests/test_formats_sbml.py
 myokit/tests/test_formats_sympy.py
 myokit/tests/test_formats_wcp.py
 myokit/tests/test_io.py
 myokit/tests/test_jacobian_calculator.py
 myokit/tests/test_jacobian_tracer.py
-myokit/tests/test_lib_common.py
 myokit/tests/test_lib_deps.py
 myokit/tests/test_lib_guess.py
 myokit/tests/test_lib_hh.py
 myokit/tests/test_lib_markov.py
 myokit/tests/test_lib_multi.py
 myokit/tests/test_lib_plots.py
 myokit/tests/test_meta.py
@@ -269,31 +261,29 @@
 myokit/tests/test_pacing_factory.py
 myokit/tests/test_pacing_system_c.py
 myokit/tests/test_pacing_system_py.py
 myokit/tests/test_parsing.py
 myokit/tests/test_progress_reporters.py
 myokit/tests/test_protocol.py
 myokit/tests/test_protocol_floating_point.py
+myokit/tests/test_protocol_time_series.py
 myokit/tests/test_pype.py
 myokit/tests/test_quantity.py
 myokit/tests/test_rhs_benchmarker.py
 myokit/tests/test_sbml_api.py
 myokit/tests/test_sbml_parser.py
 myokit/tests/test_simulation_1d.py
-myokit/tests/test_simulation_cvode.py
 myokit/tests/test_simulation_cvodes.py
 myokit/tests/test_simulation_cvodes_from_disk.py
 myokit/tests/test_simulation_fiber_tissue.py
-myokit/tests/test_simulation_ic.py
 myokit/tests/test_simulation_log_interval.py
 myokit/tests/test_simulation_opencl.py
 myokit/tests/test_simulation_opencl_log_interval.py
 myokit/tests/test_simulation_opencl_vs_cvode.py
 myokit/tests/test_simulation_opencl_vs_sim1d.py
-myokit/tests/test_simulation_p.py
 myokit/tests/test_system_info.py
 myokit/tests/test_tools.py
 myokit/tests/test_unit.py
 myokit/tests/test_user_functions.py
 myokit/tests/test_variable.py
 myokit/tests/data/beeler-1977-model-compare-a.mmt
 myokit/tests/data/beeler-1977-model-compare-b.mmt
```

### Comparing `myokit-1.33.9/setup.py` & `myokit-1.34.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,31 +81,31 @@
 
     # List of dependencies
     install_requires=[
         'configparser',
         'lxml',
         'matplotlib>=1.5',
         'numpy',
-        'scipy',            # Used in data log, and data log viewer
         'setuptools',
         # PyQT or PySide?
-        # (PySide is pip installable, Travis can get PyQt from apt)
+        # (PySide is pip installable, Actions can get PyQt from apt)
     ],
 
     # Optional extras
     extras_require={
         'docs': [
             'sphinx>=1.5, !=1.7.3',     # Doc generation
         ],
         'dev': [
-            'coverage',                 # Coverage checking
-            'flake8>=3',                # Style checking
+            'coverage',             # Coverage checking
+            'flake8>=3',            # Style checking
         ],
         'optional': [
-            'sympy',                    # Used in formats.sympy
+            'scipy',            # Used in data log, and data log viewer
+            'sympy',            # Used in formats.sympy
         ],
         'gui': ['pyqt5', 'sip'],
         'pyqt': ['pyqt5', 'sip'],
         'pyside': ['pyside2'],
     },
 
     # Unit tests
```

