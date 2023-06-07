# Comparing `tmp/pyiron_base-0.5.9.tar.gz` & `tmp/pyiron_base-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_base-0.5.9.tar", last modified: Tue Mar 29 12:57:45 2022, max compression
+gzip compressed data, was "pyiron_base-0.6.0.tar", last modified: Wed Jun  7 22:23:35 2023, max compression
```

## Comparing `pyiron_base-0.5.9.tar` & `pyiron_base-0.6.0.tar`

### file list

```diff
@@ -1,119 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4217 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.936418 pyiron_base-0.5.9/pyiron_base/archiving/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/archiving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5075 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/archiving/export_archive.py
--rw-r--r--   0 runner    (1001) docker     (121)     3523 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/archiving/import_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.936418 pyiron_base-0.5.9/pyiron_base/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1543 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (121)     4858 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/cli/ls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/cli/reloadfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/cli/rm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/cli/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.936418 pyiron_base-0.5.9/pyiron_base/database/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12648 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/database/filetable.py
--rw-r--r--   0 runner    (1001) docker     (121)    43659 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/database/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     8823 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/database/jobtable.py
--rw-r--r--   0 runner    (1001) docker     (121)     8397 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/database/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7769 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/database/performance.py
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/database/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.940418 pyiron_base-0.5.9/pyiron_base/generic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31106 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/datacontainer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     6409 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/filedata.py
--rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/fileio.py
--rw-r--r--   0 runner    (1001) docker     (121)    34775 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/flattenedstorage.py
--rw-r--r--   0 runner    (1001) docker     (121)    48981 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/hdfio.py
--rw-r--r--   0 runner    (1001) docker     (121)     3739 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/hdfstub.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/inputlist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/jedi.py
--rw-r--r--   0 runner    (1001) docker     (121)     2314 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/object.py
--rw-r--r--   0 runner    (1001) docker     (121)    32625 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)    14354 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/units.py
--rw-r--r--   0 runner    (1001) docker     (121)    10729 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/generic/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.940418 pyiron_base-0.5.9/pyiron_base/interfaces/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3909 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/interfaces/has_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     8644 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/interfaces/has_hdf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.940418 pyiron_base-0.5.9/pyiron_base/job/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34498 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     8373 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/executable.py
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/external.py
--rw-r--r--   0 runner    (1001) docker     (121)     4515 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)    67494 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)    13242 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)     5152 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/interactivewrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     9527 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/jobstatus.py
--rw-r--r--   0 runner    (1001) docker     (121)     9444 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/jobtype.py
--rw-r--r--   0 runner    (1001) docker     (121)    15129 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/path.py
--rw-r--r--   0 runner    (1001) docker     (121)    16427 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/script.py
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/template.py
--rw-r--r--   0 runner    (1001) docker     (121)    13758 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    14502 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/worker.py
--rw-r--r--   0 runner    (1001) docker     (121)     5763 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/job/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/master/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9885 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/master/flexible.py
--rw-r--r--   0 runner    (1001) docker     (121)    18775 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/master/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)    13510 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/master/list.py
--rw-r--r--   0 runner    (1001) docker     (121)    36271 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/master/parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)    17995 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/master/serial.py
--rw-r--r--   0 runner    (1001) docker     (121)     8090 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/master/submissionstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/project/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/project/data.py
--rw-r--r--   0 runner    (1001) docker     (121)    60215 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/project/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     9360 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/project/gui.py
--rw-r--r--   0 runner    (1001) docker     (121)     7073 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/project/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (121)    12776 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/project/path.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/project/update/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/project/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3577 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/project/update/pyiron_base_03x_to_04x.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/pyio/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/pyio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29090 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/pyio/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/server/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15466 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/server/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)    12794 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/server/queuestatus.py
--rw-r--r--   0 runner    (1001) docker     (121)     3476 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/server/runmode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/state/
--rw-r--r--   0 runner    (1001) docker     (121)     3114 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5839 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/state/install.py
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/state/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     6073 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/state/publications.py
--rw-r--r--   0 runner    (1001) docker     (121)     2954 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/state/queue_adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)    19378 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/state/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/state/update.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/pyiron_base/table/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26892 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/table/datamining.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/pyiron_base/toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.936418 pyiron_base-0.5.9/pyiron_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-03-29 12:57:45.000000 pyiron_base-0.5.9/pyiron_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-03-29 12:57:45.000000 pyiron_base-0.5.9/pyiron_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-29 12:57:45.000000 pyiron_base-0.5.9/pyiron_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-03-29 12:57:45.000000 pyiron_base-0.5.9/pyiron_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-03-29 12:57:45.000000 pyiron_base-0.5.9/pyiron_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-03-29 12:57:45.000000 pyiron_base-0.5.9/pyiron_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-03-29 12:57:44.000000 pyiron_base-0.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/test_benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/test_benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:45.944418 pyiron_base-0.5.9/test_benchmarks/generic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/test_benchmarks/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/test_benchmarks/generic/test_filehdfio.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-03-29 12:57:41.000000 pyiron_base-0.5.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.688014 pyiron_base-0.6.0/pyiron_base/
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-07 22:23:35.688014 pyiron_base-0.6.0/pyiron_base/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.672012 pyiron_base-0.6.0/pyiron_base/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/cli/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/cli/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/cli/reloadfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/cli/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/cli/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.676013 pyiron_base-0.6.0/pyiron_base/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24337 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/database/filetable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45395 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/database/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/database/jobtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/database/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/database/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/database/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.676013 pyiron_base-0.6.0/pyiron_base/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/interfaces/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/interfaces/has_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/interfaces/has_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/interfaces/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/interfaces/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.676013 pyiron_base-0.6.0/pyiron_base/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27613 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/datamining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.676013 pyiron_base-0.6.0/pyiron_base/jobs/job/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.680013 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/jobstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.680013 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16225 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/server/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/server/queuestatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/extension/server/runmode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55900 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/jobtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20133 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/runfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/job/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.680013 pyiron_base-0.6.0/pyiron_base/jobs/master/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/master/flexible.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/master/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/master/interactivewrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/master/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32308 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/master/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/master/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/master/submissionstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/jobs/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.680013 pyiron_base-0.6.0/pyiron_base/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.680013 pyiron_base-0.6.0/pyiron_base/project/archiving/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/archiving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/archiving/export_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/archiving/import_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/archiving/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68931 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12732 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.680013 pyiron_base-0.6.0/pyiron_base/project/update/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/project/update/pyiron_base_03x_to_04x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/pyiron_base/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/state/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/state/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/state/publications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/state/queue_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25086 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/state/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/state/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/state/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/pyiron_base/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32693 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/datacontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/filedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38762 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/flattenedstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/has_stored_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/hdfio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/hdfstub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/inputlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32625 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/storage/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/pyiron_base/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/utils/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/utils/jedi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29090 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/utils/safetar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/pyiron_base/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.672012 pyiron_base-0.6.0/pyiron_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-07 22:23:35.000000 pyiron_base-0.6.0/pyiron_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-06-07 22:23:35.000000 pyiron_base-0.6.0/pyiron_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:23:35.000000 pyiron_base-0.6.0/pyiron_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 22:23:35.000000 pyiron_base-0.6.0/pyiron_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 22:23:35.000000 pyiron_base-0.6.0/pyiron_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 22:23:35.000000 pyiron_base-0.6.0/pyiron_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-07 22:23:35.000000 pyiron_base-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/test_benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/test_benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/test_benchmarks/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/test_benchmarks/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/test_benchmarks/generic/test_filehdfio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:35.684013 pyiron_base-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/tests/test_testwithproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/tests/test_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-07 22:23:32.000000 pyiron_base-0.6.0/versioneer.py
```

### Comparing `pyiron_base-0.5.9/LICENSE` & `pyiron_base-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.9/PKG-INFO` & `pyiron_base-0.6.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pyiron_base
-Version: 0.5.9
+Version: 0.6.0
 Summary: pyiron_base - an integrated development environment (IDE) for computational science.
 Home-page: https://github.com/pyiron/pyiron_base
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
 http://pyiron.org
-
```

### Comparing `pyiron_base-0.5.9/README.rst` & `pyiron_base-0.6.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pyiron
 ======
 
-.. image:: https://coveralls.io/repos/github/pyiron/pyiron_base/badge.svg?branch=master
-    :target: https://coveralls.io/github/pyiron/pyiron_base?branch=master
+.. image:: https://coveralls.io/repos/github/pyiron/pyiron_base/badge.svg?branch=main
+    :target: https://coveralls.io/github/pyiron/pyiron_base?branch=main
     :alt: Coverage Status
 
 .. image:: https://anaconda.org/conda-forge/pyiron_base/badges/latest_release_date.svg
     :target: https://anaconda.org/conda-forge/pyiron_base/
     :alt: Release_Date
 
 .. image:: https://github.com/pyiron/pyiron_base/workflows/Python%20package/badge.svg
@@ -21,20 +21,20 @@
     :target: https://pyiron-base.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 pyiron - an integrated development environment (IDE) for computational materials science. While the general pyiron framework is focused on atomistic simulations, pyiron_base is independent of atomistic simulation. It can be used as a standalone workflow management combining a hierachical storage interface based on HDF5, support for HPC computing clusters and a user interface integrated in the Jupyter environment. 
 
 Installation
 ------------
-You can test pyiron on `Mybinder.org (beta) <https://mybinder.org/v2/gh/pyiron/pyiron_base/master?urlpath=lab>`_.
+You can test pyiron on `Mybinder.org (beta) <https://mybinder.org/v2/gh/pyiron/pyiron_base/main?urlpath=lab>`_.
 For a local installation we recommend to install pyiron inside an `anaconda <https://www.anaconda.com>`_  environment::
 
     conda install -c conda-forge pyiron_base
 
-See the `Documentation-Installation <https://pyiron.github.io/source/installation.html>`_ page for more details.
+See the `Documentation-Installation <https://pyiron.readthedocs.io/en/latest/source/installation.html>`_ page for more details.
 
 Example
 -------
 After the successful configuration you can start your first pyiron calculation. Navigate to the the projects directory and start a jupyter notebook or jupyter lab session correspondingly::
 
     cd ~/pyiron/projects
     jupyter notebook
@@ -47,15 +47,15 @@
 
 
 Getting started:
 ----------------
 Test pyiron with mybinder:
 
 .. image:: https://mybinder.org/badge_logo.svg
-     :target: https://mybinder.org/v2/gh/pyiron/pyiron_base/master
+     :target: https://mybinder.org/v2/gh/pyiron/pyiron_base/main
      :alt: mybinder
 
 
 License and Acknowledgments
 ---------------------------
 ``pyiron_base`` is licensed under the BSD license.
```

### Comparing `pyiron_base-0.5.9/pyiron_base/__init__.py` & `pyiron_base-0.6.0/pyiron_base/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,67 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from pyiron_base.state import state
 
 # API of the pyiron_base module - in alphabetical order
-from pyiron_base.generic.factory import PyironFactory
-from pyiron_base.generic.flattenedstorage import FlattenedStorage
-from pyiron_base.generic.hdfio import FileHDFio, ProjectHDFio
-from pyiron_base.generic.datacontainer import DataContainer
-from pyiron_base.generic.inputlist import InputList
-from pyiron_base.generic.parameters import GenericParameters
-from pyiron_base.generic.util import deprecate, deprecate_soon, ImportAlarm
-from pyiron_base.job.executable import Executable
-from pyiron_base.job.external import Notebook, load, dump
-from pyiron_base.job.generic import GenericJob
-from pyiron_base.job.interactive import InteractiveBase
-from pyiron_base.job.interactivewrapper import InteractiveWrapper
-from pyiron_base.job.jobstatus import (
+from pyiron_base.interfaces.factory import PyironFactory
+from pyiron_base.storage.flattenedstorage import FlattenedStorage
+from pyiron_base.storage.hdfio import FileHDFio, ProjectHDFio
+from pyiron_base.storage.datacontainer import DataContainer
+from pyiron_base.storage.has_stored_traits import HasStoredTraits
+from pyiron_base.storage.inputlist import InputList
+from pyiron_base.storage.parameters import GenericParameters
+from pyiron_base.storage.filedata import load_file, FileDataTemplate, FileData
+from pyiron_base.utils.deprecate import Deprecator, deprecate, deprecate_soon
+from pyiron_base.utils.error import ImportAlarm
+from pyiron_base.jobs.job.extension.executable import Executable
+from pyiron_base.project.external import Notebook, load, dump
+from pyiron_base.jobs.job.generic import GenericJob
+from pyiron_base.jobs.job.interactive import InteractiveBase
+from pyiron_base.jobs.master.interactivewrapper import InteractiveWrapper
+from pyiron_base.jobs.job.extension.jobstatus import (
     JobStatus,
     job_status_successful_lst,
     job_status_finished_lst,
     job_status_lst,
 )
-from pyiron_base.job.jobtype import JOB_CLASS_DICT, JobType, JobTypeChoice
-from pyiron_base.job.template import TemplateJob, PythonTemplateJob
-from pyiron_base.job.factory import JobFactoryCore
-from pyiron_base.master.generic import GenericMaster, get_function_from_string
-from pyiron_base.master.list import ListMaster
-from pyiron_base.master.parallel import ParallelMaster, JobGenerator
-from pyiron_base.master.serial import SerialMasterBase
-from pyiron_base.master.flexible import FlexibleMaster
+from pyiron_base.jobs.job.jobtype import JOB_CLASS_DICT, JobType, JobTypeChoice
+from pyiron_base.jobs.job.template import TemplateJob, PythonTemplateJob
+from pyiron_base.jobs.job.factory import JobFactoryCore
+from pyiron_base.jobs.master.generic import GenericMaster, get_function_from_string
+from pyiron_base.jobs.master.list import ListMaster
+from pyiron_base.jobs.master.parallel import ParallelMaster, JobGenerator
+from pyiron_base.jobs.master.serial import SerialMasterBase
+from pyiron_base.jobs.master.flexible import FlexibleMaster
 from pyiron_base.project.generic import Project, Creator
-from pyiron_base.pyio.parser import Logstatus, extract_data_from_file
-from pyiron_base.server.queuestatus import validate_que_request
+from pyiron_base.utils.parser import Logstatus, extract_data_from_file
+from pyiron_base.jobs.job.extension.server.queuestatus import validate_que_request
 from pyiron_base.state.settings import Settings
 from pyiron_base.state.install import install_dialog
-from pyiron_base.table.datamining import PyironTable, TableJob
-from pyiron_base.generic.object import HasDatabase, HasStorage, PyironObject
+from pyiron_base.jobs.datamining import PyironTable, TableJob
+from pyiron_base.interfaces.object import HasDatabase, HasStorage, PyironObject
 from pyiron_base.database.performance import get_database_statistics
+from pyiron_base.interfaces.has_groups import HasGroups
+from pyiron_base.interfaces.has_hdf import HasHDF
 
-from pyiron_base.toolkit import Toolkit, BaseTools
+from pyiron_base.jobs.job.toolkit import Toolkit, BaseTools
 
 Project.register_tools("base", BaseTools)
 
 # optional API of the pyiron_base module
 try:
     from pyiron_base.project.gui import ProjectGUI
 except (ImportError, TypeError, AttributeError):
     pass
 
 # Internal init
 from ._version import get_versions
-from pyiron_base.generic.jedi import fix_ipython_autocomplete
+from pyiron_base.utils.jedi import fix_ipython_autocomplete
 
 # Set version of pyiron_base
 __version__ = get_versions()["version"]
 del get_versions
 
 # Jedi fix
 fix_ipython_autocomplete()
```

### Comparing `pyiron_base-0.5.9/pyiron_base/_tests.py` & `pyiron_base-0.6.0/pyiron_base/_tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """Classes to help developers avoid code duplication when writing tests for pyiron."""
 
 from contextlib import redirect_stdout
 import doctest
 from io import StringIO
 import unittest
 import os
-from pyiron_base import PythonTemplateJob
+from pyiron_base import PythonTemplateJob, state
 from pyiron_base.project.generic import Project
 from abc import ABC
 from inspect import getfile
 
 
 __author__ = "Liam Huber"
 __copyright__ = (
@@ -31,18 +31,23 @@
 
     """
     Tests that also include testing the docstrings in the specified modules
     """
 
     @classmethod
     def setUpClass(cls):
+        cls._initial_settings_configuration = state.settings.configuration.copy()
         if any([cls is c for c in _TO_SKIP]):
             raise unittest.SkipTest(f"{cls.__name__} tests, it's a base class")
         super().setUpClass()
 
+    @classmethod
+    def tearDownClass(cls) -> None:
+        state.update(cls._initial_settings_configuration)
+
     @property
     def docstring_module(self):
         """
         Define module whose docstrings will be tested
         """
         return None
 
@@ -69,43 +74,53 @@
         print("TestWithProject: Setting up test project")
         cls.project_path = getfile(cls)[:-3].replace("\\", "/")
         cls.file_location, cls.project_name = os.path.split(cls.project_path)
         cls.project = Project(cls.project_path)
 
     @classmethod
     def tearDownClass(cls):
+        super().tearDownClass()
         cls.project.remove(enable=True)
         try:
             os.remove(os.path.join(cls.file_location, "pyiron.log"))
         except FileNotFoundError:
             pass
 
 
 class TestWithCleanProject(TestWithProject, ABC):
     """
     Tests that start and remove a project for their suite, and remove jobs from the project for each test.
     """
 
     def tearDown(self):
+        super().tearDown()
         self.project.remove_jobs(recursive=True, progress=False, silently=True)
 
 
 class ToyJob(PythonTemplateJob):
     def __init__(self, project, job_name):
         """A toyjob to test export/import functionalities."""
         super(ToyJob, self).__init__(project, job_name)
         self.input.data_in = 100
 
     def write_input(self):
+        super().write_input()
         self.input.write(os.path.join(self.working_directory, "input.yml"))
 
     # Allow writing of the input file
     def _check_if_input_should_be_written(self):
         return True
 
+    # Check for valid input
+    def validate_ready_to_run(self):
+        if not isinstance(self.input.data_in, int):
+            raise ValueError(
+                f"data_in in should be of type int, not {type(self.input.data_in)}."
+            )
+
     # This function is executed
     def run_static(self):
         self.status.running = True
         self.output.data_out = self.input.data_in + 1
         self.status.finished = True
         self.to_hdf()
         self.compress()
```

### Comparing `pyiron_base-0.5.9/pyiron_base/archiving/export_archive.py` & `pyiron_base-0.6.0/pyiron_base/project/archiving/export_archive.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 import os
 import numpy as np
 from shutil import copyfile
 from pyfileindex import PyFileIndex
 import tarfile
 from shutil import rmtree
-from pyiron_base.generic.util import static_isinstance
+from pyiron_base.project.archiving.shared import getdir
+from pyiron_base.utils.instance import static_isinstance
 
 
 def new_job_id(job_id, job_translate_dict):
     if isinstance(job_id, float) and not np.isnan(job_id):
         job_id = int(job_id)
     if isinstance(job_id, int):
         return job_translate_dict[job_id]
     else:
         return None
 
 
-def getdir(path):
-    path_base_name = os.path.basename(path)
-    if path_base_name == "":
-        return os.path.basename(os.path.dirname(path))
-    else:
-        return path_base_name
-
-
 def update_project(project_instance, directory_to_transfer, archive_directory, df):
     directory_to_transfer = os.path.basename(directory_to_transfer)
     pr_transfer = project_instance.open(os.curdir)
     dir_name_transfer = getdir(path=directory_to_transfer)
     dir_name_archive = getdir(path=archive_directory)
     path_rel_lst = [
         os.path.relpath(p, pr_transfer.project_path) for p in df["project"].values
@@ -54,34 +47,47 @@
         if p != "."
         else os.path.join(archive_directory, dir_name_transfer)
         for p in path_rel_lst
     ]
 
 
 def compress_dir(archive_directory):
-
     arch_comp_name = archive_directory + ".tar.gz"
     tar = tarfile.open(arch_comp_name, "w:gz")
     tar.add(os.path.relpath(archive_directory, os.getcwd()))
     tar.close()
     rmtree(archive_directory)
 
 
-def copy_files_to_archive(directory_to_transfer, archive_directory, compressed=True):
+def copy_files_to_archive(
+    directory_to_transfer, archive_directory, compressed=True, copy_all_files=False
+):
+    """
+    Create an archive of jobs in directory_to_transfer.
+
+    Args:
+        directory_to_transfer (str): project directory with jobs to export
+        archive_directory (str): name of the final archive; if no file ending is given .tar.gz is added automatically when needed
+        compressed (bool): if True compress archive_directory as a tarball; default True
+        copy_all_files (bool): if True include job output files in archive, otherwise just include .h5 files; default False
+    """
     if archive_directory[-7:] == ".tar.gz":
         archive_directory = archive_directory[:-7]
         if not compressed:
             compressed = True
 
     if directory_to_transfer[-1] != "/":
         directory_to_transfer = os.path.basename(directory_to_transfer)
     else:
         directory_to_transfer = os.path.basename(directory_to_transfer[:-1])
     # print("directory to transfer: "+directory_to_transfer)
-    pfi = PyFileIndex(path=directory_to_transfer, filter_function=filter_function)
+    if not copy_all_files:
+        pfi = PyFileIndex(path=directory_to_transfer, filter_function=filter_function)
+    else:
+        pfi = PyFileIndex(path=directory_to_transfer)
     df_files = pfi.dataframe[~pfi.dataframe.is_directory]
 
     # Create directories
     dir_lst = generate_list_of_directories(
         df_files=df_files,
         directory_to_transfer=directory_to_transfer,
         archive_directory=archive_directory,
```

### Comparing `pyiron_base-0.5.9/pyiron_base/archiving/import_archive.py` & `pyiron_base-0.6.0/pyiron_base/project/archiving/import_archive.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 import os
 import pandas
 import numpy as np
 from shutil import rmtree
 from distutils.dir_util import copy_tree
 import tarfile
-from pyiron_base.generic.util import static_isinstance
+from pyiron_base.project.archiving.shared import getdir
+from pyiron_base.utils.instance import static_isinstance
 from pyiron_base.state import state
 
 
-def getdir(path):
-    path_base_name = os.path.basename(path)
-    if path_base_name == "":
-        return os.path.basename(os.path.dirname(path))
-    else:
-        return path_base_name
-
-
 def update_id_lst(record_lst, job_id_lst):
     masterid_lst = []
     for masterid in record_lst:
         if masterid is None or np.isnan(masterid):
             masterid_lst.append(None)
         elif isinstance(masterid, int) or isinstance(masterid, float):
             masterid = int(masterid)
```

### Comparing `pyiron_base-0.5.9/pyiron_base/cli/__init__.py` & `pyiron_base-0.6.0/pyiron_base/cli/control.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,15 @@
 CLI for various pyiron utilities.
 """
 
 import argparse
 import os
 import warnings
 
-from . import ls
-from . import rm
-from . import install
-from . import reloadfile
-from . import wrapper
+from pyiron_base.cli import ls, rm, install, reloadfile, wrapper
 
 __author__ = "Marvin Poul"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -58,9 +54,9 @@
             warnings.warn(
                 "module '{}' does not define main or register " "function, ignoring"
             )
 
     args = parser.parse_args()
     args.cli(args)
 
-    if not args.dirty:
+    if not args.dirty and os.path.exists("pyiron.log"):
         os.remove("pyiron.log")
```

### Comparing `pyiron_base-0.5.9/pyiron_base/cli/install.py` & `pyiron_base-0.6.0/pyiron_base/cli/install.py`

 * *Files 24% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         "--resources",
         default="~/pyiron/resources",
         help="path where resources should be installed",
     )
     parser.add_argument(
         "-u",
         "--url",
-        default="https://github.com/pyiron/pyiron-resources/releases/download/0.0.3/resources-0.0.3.tar.gz",
+        default="https://github.com/pyiron/pyiron-resources/releases/latest/download/resources.tar.gz",
         help="url to download zipped resources",
     )
     parser.add_argument(
         "-p",
         "--project",
         default="~/pyiron/projects",
         help="path where pyiron should expect projects to run",
```

### Comparing `pyiron_base-0.5.9/pyiron_base/cli/ls.py` & `pyiron_base-0.6.0/pyiron_base/cli/ls.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 import argparse
 import datetime
 import re
 import sys
 import pandas as pd
-import pyiron_base.job.jobstatus
+import pyiron_base.jobs.job.extension.jobstatus
 from pyiron_base import Project
 
 __author__ = "Marvin Poul"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -38,15 +38,14 @@
     Print all jobs that were aborted less than 5 hours ago and match
     "spx.*restart":
         pyiron ls -n "spx.*restart" -i 5h -s aborted
 """
 
 
 def register(parser):
-
     parser.add_argument(
         "project", default=".", nargs="?", help="path to pyiron project"
     )
 
     filter = parser.add_argument_group(
         title="filter",
         description="select which jobs to show, all filters must be true "
@@ -68,18 +67,18 @@
         nargs="+",
         help="chemical elements that must be present in unit cell",
     )
     filter.add_argument(
         "-s",
         "--status",
         nargs="+",
-        choices=pyiron_base.job.jobstatus.job_status_lst,
+        choices=pyiron_base.jobs.job.extension.jobstatus.job_status_lst,
         metavar="status",
         help="job status must be one of the given, one of {}".format(
-            ", ".join(pyiron_base.job.jobstatus.job_status_lst)
+            ", ".join(pyiron_base.jobs.job.extension.jobstatus.job_status_lst)
         ),
     )
     filter.add_argument(
         "-i",
         "--since",
         help="timestop must be less then the given duration before now, "
         "must be an integer and a time unit, i.e. one of d (days), "
@@ -119,15 +118,14 @@
     )
     output.add_argument(
         "-a", "--all", action="store_true", help="show all job attributes"
     )
 
 
 def main(args):
-
     if args.status:
         if "status" not in args.columns:
             args.columns = args.columns + ["status"]
 
     if args.since:
         if "timestop" not in args.columns:
             args.columns = args.columns + ["timestop"]
```

### Comparing `pyiron_base-0.5.9/pyiron_base/cli/reloadfile.py` & `pyiron_base-0.6.0/pyiron_base/cli/reloadfile.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.9/pyiron_base/cli/rm.py` & `pyiron_base-0.6.0/pyiron_base/cli/rm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 Remove jobs from pyiron project or whole project.
 """
 
 import os
-from pyiron_base import Project
+from pyiron_base.project.generic import Project
 
 __author__ = "Marvin Poul"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -28,15 +28,14 @@
     )
     parser.add_argument(
         "-r", "--recursive", action="store_true", help="recurse into subprojects"
     )
 
 
 def main(args):
-
     pr = Project(args.project)
     if args.jobs_only:
         pr.remove_jobs(recursive=args.recursive, silently=True)
     else:
         pr.remove(enable=True)
-        if not os.listdir(args.project):
+        if os.path.exists(args.project) and not os.listdir(args.project):
             os.rmdir(args.project)
```

### Comparing `pyiron_base-0.5.9/pyiron_base/cli/wrapper.py` & `pyiron_base-0.6.0/pyiron_base/cli/wrapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 Run a job from hdf5.
 """
 
-from pyiron_base.job.wrapper import job_wrapper_function
+from pyiron_base.jobs.job.wrapper import job_wrapper_function
 
 
 def register(parser):
     parser.add_argument(
         "-d",
         "--debug",
         action="store_true",
@@ -21,17 +21,24 @@
     parser.add_argument("-f", "--file-path", help="path to the HDF5 file")
     parser.add_argument(
         "-s",
         "--submit",
         action="store_true",
         help="submit to queuing system on remote host",
     )
+    parser.add_argument(
+        "-c",
+        "--collect",
+        action="store_true",
+        help="only collect output of calculation",
+    )
 
 
 def main(args):
     job_wrapper_function(
         working_directory=args.project,
         job_id=args.job_id,
         file_path=args.file_path,
         debug=args.debug,
         submit_on_remote=args.submit,
+        collect=args.collect,
     )
```

### Comparing `pyiron_base-0.5.9/pyiron_base/database/generic.py` & `pyiron_base-0.6.0/pyiron_base/database/generic.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,36 +3,37 @@
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 DatabaseAccess class deals with accessing the database
 """
 
 from pyiron_base.state.logger import logger
 from abc import ABC, abstractmethod
+from collections.abc import Iterable
 import warnings
 import numpy as np
 import re
-import time
 import os
 from datetime import datetime
-from pyiron_base.generic.util import deprecate
+from pyiron_base.utils.deprecate import deprecate
 import pandas
 from sqlalchemy import (
     create_engine,
     MetaData,
     Table,
     text,
     and_,
     or_,
 )
 from sqlalchemy.pool import NullPool
 from sqlalchemy.sql import select
 from sqlalchemy.exc import OperationalError, DatabaseError
 from threading import Thread, Lock
 from queue import SimpleQueue, Empty as QueueEmpty
-from pyiron_base.database.tables import HistoricalTable
+from pyiron_base.database.tables import get_historical_table
+from pyiron_base.utils.error import retry
 
 __author__ = "Murat Han Celik"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH"
     " - Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -109,15 +110,15 @@
         for key in kwargs.keys():
             if key not in list(df.columns):
                 raise ValueError(
                     f"Column name {key} does not exist in the project database!"
                 )
         for key, val in kwargs.items():
             invert = False
-            if val is not None and val[0] == "!":
+            if isinstance(val, str) and val[0] == "!":
                 invert = True
                 val = val[1:]
             if val is None:
                 update = df[key].isnull()
             elif str(val).startswith("*") and str(val).endswith("*"):
                 update = df[key].str.contains(str(val).replace("*", ""))
             elif str(val).endswith("*"):
@@ -217,14 +218,54 @@
             return df.sort_values(by=sort_by)
         return df
 
     @abstractmethod
     def _get_table_headings(self, table_name=None):
         pass
 
+    def item_update(self, par_dict, item_id):
+        if isinstance(item_id, Iterable):
+            return self._items_update(par_dict=par_dict, item_ids=item_id)
+        return self._item_update(par_dict=par_dict, item_id=item_id)
+
+    @abstractmethod
+    def _item_update(self, par_dict, item_id):
+        pass
+
+    def _items_update(self, par_dict, item_ids):
+        """
+        For now simply loops over all item_ids to call item_update,
+        but can be made more efficient.
+        Should be made an asbtract method when defined in inheriting classes
+
+        Args:
+            par_dict (_type_): _description_
+            item_ids (_type_): _description_
+        """
+        for i_id in item_ids:
+            self._item_update(par_dict=par_dict, item_id=i_id)
+
+    def set_job_status(self, status, job_id):
+        """
+        Set status of a job or multiple jobs if job_id is iterable.
+
+        Args:
+            status (str): status
+            job_id (int, Iterable): job id
+        """
+        if isinstance(job_id, Iterable):
+            return self._items_update(
+                par_dict={"status": status},
+                item_ids=job_id,
+            )
+        return self._item_update(
+            par_dict={"status": status},
+            item_id=job_id,
+        )
+
     def get_table_headings(self, table_name=None):
         """
         Get column names; if given table_name can select one of multiple tables defined in the database, but subclasses
         may ignore it
 
         Args:
             table_name (str): simple string of a table_name like: 'jobs_username'
@@ -353,54 +394,55 @@
         self.engine = engine
         self._conn = None
         self._lock = Lock()
         self._watchdog = None
         self._logger = logger
         self._timeout = timeout
 
+    def execute_once(self, *args, **kwargs):
+        with self._lock:
+            if self._conn is None or self._conn.closed:
+                self._conn = self.engine.connect()
+                if self._timeout > 0:
+                    # only log reconnections when we keep the connection alive between requests otherwise we'll spam
+                    # the log
+                    if self._conn is None:
+                        self._logger.info(
+                            "Reconnecting to DB; connection did not exist."
+                        )
+                    else:
+                        self._logger.info("Reconnecting to DB; connection was closed.")
+                    if self._watchdog is not None:
+                        # in case connection is dead, but watchdog is still up, something else killed the connection,
+                        # make the watchdog quit, then making a new one
+                        self._watchdog.kill()
+                    self._watchdog = ConnectionWatchDog(
+                        self._conn, self._lock, timeout=self._timeout
+                    )
+                    self._watchdog.start()
+            if self._timeout > 0:
+                self._watchdog.kick()
+            return self._conn.execute(*args, **kwargs)
+
     def execute(self, *args, **kwargs):
-        while True:
-            try:
-                with self._lock:
-                    if self._conn is None or self._conn.closed:
-                        self._conn = self.engine.connect()
-                        if self._timeout > 0:
-                            # only log reconnections when we keep the connection alive between requests otherwise we'll spam
-                            # the log
-                            if self._conn is None:
-                                self._logger.info(
-                                    "Reconnecting to DB; connection not existing."
-                                )
-                            else:
-                                self._logger.info(
-                                    "Reconnecting to DB; connection closed."
-                                )
-                            if self._watchdog is not None:
-                                # in case connection is dead, but watchdog is still up, something else killed the connection,
-                                # make the watchdog quit, then making a new one
-                                self._watchdog.kill()
-                            self._watchdog = ConnectionWatchDog(
-                                self._conn, self._lock, timeout=self._timeout
-                            )
-                            self._watchdog.start()
-                    if self._timeout > 0:
-                        self._watchdog.kick()
-                    result = self._conn.execute(*args, **kwargs)
-                    break
-            except OperationalError as e:
-                print(
-                    f"Database connection failed with operational error {e}, waiting 5s, then re-trying."
-                )
-                time.sleep(5)
-        return result
+        return retry(
+            lambda: self.execute_once(*args, **kwargs),
+            error=OperationalError,
+            msg="Database connection failed with operational error.",
+            delay=5,
+        )
 
     def close(self):
         if self._conn is not None:
             self._conn.close()
 
+    def commit(self):
+        if self._conn is not None:
+            self._conn.commit()
+
 
 class DatabaseAccess(IsDatabase):
     """
     A core element of PyIron, which generally deals with accessing the database: getting, sending, changing some data
     to the db.
 
     Args:
@@ -429,29 +471,44 @@
         self._sql_lite = "sqlite" in connection_string
         try:
             if not self._sql_lite:
                 self._engine = create_engine(
                     connection_string,
                     connect_args={"connect_timeout": 15},
                     poolclass=NullPool,
+                    future=True,
                 )
                 self.conn = AutorestoredConnection(self._engine, timeout=self._timeout)
                 self._keep_connection = self._timeout > 0
             else:
-                self._engine = create_engine(connection_string)
+                self._engine = create_engine(connection_string, future=True)
                 self.conn = self._engine.connect()
                 self.conn.connection.create_function("like", 2, self.regexp)
                 self._keep_connection = True
         except Exception as except_msg:
             raise ValueError("Connection to database failed: " + str(except_msg))
 
         self._chem_formula_lim_length = 50
-        self.__reload_db()
-        self.simulation_table = HistoricalTable(str(table_name), self.metadata)
-        self.metadata.create_all()
+
+        def _create_table():
+            self.__reload_db()
+            self.simulation_table = get_historical_table(
+                table_name=str(table_name), metadata=self.metadata, extend_existing=True
+            )
+            self.metadata.create_all(bind=self._engine)
+
+        # too many jobs trying to talk to the database can cause this to fail.
+        retry(
+            _create_table,
+            error=OperationalError,
+            msg="Database busy with too many connections.",
+            at_most=10,
+            delay=0.1,
+            delay_factor=2,
+        )
         self._view_mode = False
 
     def _get_view_mode(self):
         return self._view_mode
 
     @IsDatabase.view_mode.setter
     def view_mode(self, value):
@@ -592,16 +649,16 @@
     def __reload_db(self):
         """
         Reload database
 
         Returns:
 
         """
-        self.metadata = MetaData(bind=self._engine)
-        self.metadata.reflect(self._engine)
+        self.metadata = MetaData()
+        self.metadata.reflect(bind=self._engine)
 
     @staticmethod
     def regexp(expr, item):
         """
         Regex function for SQLite
         Args:
             expr: str, regex expression
@@ -649,15 +706,14 @@
         if table_name is None:
             table_name = self.table_name
         self.__reload_db()
         try:
             simulation_list = Table(
                 str(table_name),
                 self.metadata,
-                autoload=True,
                 autoload_with=self._engine,
             )
         except Exception:
             raise ValueError(str(table_name) + " does not exist")
         return [column.name for column in iter(simulation_list.columns)]
 
     def add_column(self, col_name, col_type):
@@ -672,18 +728,21 @@
 
         """
         if not self._view_mode:
             if isinstance(col_name, list):
                 col_name = col_name[-1]
             if isinstance(col_type, list):
                 col_type = col_type[-1]
-            self._engine.execute(
-                "ALTER TABLE %s ADD COLUMN %s %s"
-                % (self.simulation_table.name, col_name, col_type)
+            self.conn.execute(
+                text(
+                    "ALTER TABLE %s ADD COLUMN %s %s"
+                    % (self.simulation_table.name, col_name, col_type)
+                )
             )
+            self.conn.commit()
         else:
             raise PermissionError("Not avilable in viewer mode.")
 
     def change_column_type(self, col_name, col_type):
         """
         Modify data type of an existing column - required for modification on the database
 
@@ -695,18 +754,21 @@
 
         """
         if not self._view_mode:
             if isinstance(col_name, list):
                 col_name = col_name[-1]
             if isinstance(col_type, list):
                 col_type = col_type[-1]
-            self._engine.execute(
-                "ALTER TABLE %s ALTER COLUMN %s TYPE %s"
-                % (self.simulation_table.name, col_name, col_type)
+            self.conn.execute(
+                text(
+                    "ALTER TABLE %s ALTER COLUMN %s TYPE %s"
+                    % (self.simulation_table.name, col_name, col_type)
+                )
             )
+            self.conn.commit()
         else:
             raise PermissionError("Not avilable in viewer mode.")
 
     def get_items_sql(self, where_condition=None, sql_statement=None):
         """
         Submit an SQL query to the database
 
@@ -769,28 +831,26 @@
                 if self._engine.dialect.name == "postgresql"
                 else sql_statement
             )
             # TODO: make it save against SQL injection
             result = self.conn.execute(text(sql_statement))
         else:
             result = self.conn.execute(text("select * from " + self.table_name))
-        row = result.fetchall()
+        row = result.mappings().all()
         if not self._keep_connection:
             self.conn.close()
 
         # change the date of str datatype back into datetime object
         output_list = []
         for col in row:
             # ensures working with db entries, which are camel case
             timestop_index = [item.lower() for item in col.keys()].index("timestop")
             timestart_index = [item.lower() for item in col.keys()].index("timestart")
-            tmp_values = col.values()
-            if (
-                col.values()[timestop_index] and col.values()[timestart_index]
-            ) is not None:
+            tmp_values = list(col.values())
+            if (tmp_values[timestop_index] and tmp_values[timestart_index]) is not None:
                 # changes values
                 try:
                     tmp_values[timestop_index] = datetime.strptime(
                         str(tmp_values[timestop_index]), "%Y-%m-%d %H:%M:%S.%f"
                     )
                     tmp_values[timestart_index] = datetime.strptime(
                         str(tmp_values[timestart_index]), "%Y-%m-%d %H:%M:%S.%f"
@@ -845,16 +905,17 @@
         if not self._view_mode:
             try:
                 par_dict = self._check_chem_formula_length(par_dict)
                 par_dict = dict(
                     (key.lower(), value) for key, value in par_dict.items()
                 )  # make keys lowercase
                 result = self.conn.execute(
-                    self.simulation_table.insert(par_dict)
+                    self.simulation_table.insert().values(**par_dict)
                 ).inserted_primary_key[-1]
+                self.conn.commit()
                 if not self._keep_connection:
                     self.conn.close()
                 return result
             except Exception as except_msg:
                 raise ValueError("Error occurred: " + str(except_msg))
         else:
             raise PermissionError("Not avilable in viewer mode.")
@@ -886,16 +947,16 @@
                       'timestop': datetime.datetime(2016, 5, 2, 11, 31, 4, 371165),
                       'totalcputime': 0.117788,
                       'username': u'Test'}]
         """
         try:
             if type(var) is list:
                 var = var[-1]
-            query = select(
-                [self.simulation_table], self.simulation_table.c[str(col_name)] == var
+            query = select(self.simulation_table).where(
+                self.simulation_table.c[str(col_name)] == var
             )
         except Exception:
             raise ValueError("There is no Column named: " + col_name)
         try:
             result = self.conn.execute(query)
         except (OperationalError, DatabaseError):
             if not self._sql_lite:
@@ -903,50 +964,52 @@
             else:
                 self.conn = self._engine.connect()
                 self.conn.connection.create_function("like", 2, self.regexp)
             result = self.conn.execute(query)
         row = result.fetchall()
         if not self._keep_connection:
             self.conn.close()
-        return [dict(zip(col.keys(), col._mapping.values())) for col in row]
+        return [dict(zip(col._mapping.keys(), col._mapping.values())) for col in row]
 
-    def item_update(self, par_dict, item_id):
+    def _item_update(self, par_dict, item_id):
         """
         Modify Item in database
 
         Args:
             par_dict (dict): Dictionary of the parameters to be modified,, where the key is the column name.
                             {'job' : 'maximize',
                              'subjob' : 'testing',
                              ........}
             item_id (int, list): Database Item ID (Integer) - '38'  can also be [38]
 
         Returns:
 
         """
         if not self._view_mode:
-            if type(item_id) is list:
-                item_id = item_id[-1]  # sometimes a list is given, make it int
             if np.issubdtype(type(item_id), np.integer):
                 item_id = int(item_id)
             # all items must be lower case, ensured here
             par_dict = dict((key.lower(), value) for key, value in par_dict.items())
-            query = self.simulation_table.update(
-                self.simulation_table.c["id"] == item_id
-            ).values()
+            query = (
+                self.simulation_table.update()
+                .where(self.simulation_table.c["id"] == item_id)
+                .values()
+            )
             try:
                 self.conn.execute(query, par_dict)
+                self.conn.commit()
             except (OperationalError, DatabaseError):
                 if not self._sql_lite:
                     self.conn = AutorestoredConnection(self._engine)
                 else:
                     self.conn = self._engine.connect()
                     self.conn.connection.create_function("like", 2, self.regexp)
 
                 self.conn.execute(query, par_dict)
+                self.conn.commit()
             if not self._keep_connection:
                 self.conn.close()
         else:
             raise PermissionError("Not avilable in viewer mode.")
 
     def delete_item(self, item_id):
         """
@@ -956,18 +1019,19 @@
             item_id (int): Databse Item ID (Integer), like: 38
 
         Returns:
 
         """
         if not self._view_mode:
             self.conn.execute(
-                self.simulation_table.delete(
+                self.simulation_table.delete().where(
                     self.simulation_table.c["id"] == int(item_id)
                 )
             )
+            self.conn.commit()
             if not self._keep_connection:
                 self.conn.close()
         else:
             raise PermissionError("Not avilable in viewer mode.")
 
     # Shortcut
     def get_item_by_id(self, item_id):
@@ -1108,44 +1172,40 @@
                 if "%" not in str(value):
                     part_of_statement = [self.simulation_table.c[str(key)] == value]
                 else:
                     part_of_statement = [self.simulation_table.c[str(key)].like(value)]
             # here all statements are wrapped together for the and statement
             and_statement += part_of_statement
         if return_all_columns:
-            query = select([self.simulation_table], and_(*and_statement))
+            query = select(self.simulation_table).where(and_(*and_statement))
         else:
-            query = select([self.simulation_table.columns["id"]], and_(*and_statement))
+            query = select(self.simulation_table.columns["id"]).where(
+                and_(*and_statement)
+            )
         try:
             result = self.conn.execute(query)
         except (OperationalError, DatabaseError):
             if not self._sql_lite:
                 self.conn = AutorestoredConnection(self._engine)
             else:
                 self.conn = self._engine.connect()
                 self.conn.connection.create_function("like", 2, self.regexp)
 
             result = self.conn.execute(query)
         row = result.fetchall()
         if not self._keep_connection:
             self.conn.close()
-        return [dict(zip(col.keys(), col._mapping.values())) for col in row]
+        return [dict(zip(col._mapping.keys(), col._mapping.values())) for col in row]
 
     def get_job_status(self, job_id):
         try:
             return self.get_item_by_id(item_id=job_id)["status"]
         except KeyError:
             return None
 
-    def set_job_status(self, job_id, status):
-        self.item_update(
-            {"status": str(status)},
-            job_id,
-        )
-
     def get_job_working_directory(self, job_id):
         try:
             db_entry = self.get_item_by_id(job_id)
             if db_entry:
                 job_name = db_entry["subjob"][1:]
                 return os.path.join(
                     db_entry["projectpath"],
```

### Comparing `pyiron_base-0.5.9/pyiron_base/database/jobtable.py` & `pyiron_base-0.6.0/pyiron_base/database/jobtable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.9/pyiron_base/database/manager.py` & `pyiron_base-0.6.0/pyiron_base/database/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 A class for mediating connections to SQL databases.
 """
 
 from urllib.parse import quote_plus
 from pyiron_base.state.logger import logger
-from pyiron_base.generic.util import Singleton
+from pyiron_base.interfaces.singleton import Singleton
 from pyiron_base.state.settings import settings as s
 from pyiron_base.database.generic import DatabaseAccess
 import os
 
 __author__ = "Jan Janssen, Liam Huber"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH"
@@ -133,15 +133,15 @@
         Swtich to an local SQLite based database.
 
         Args:
             file_name (str): SQLite database file name
             cwd (str/None): directory where the SQLite database file is located in
         """
         if self.using_local_database:
-            logger.log("Database is already in local mode or disabled!")
+            logger.info("Database is already in local mode or disabled!")
         else:
             if cwd is None and not os.path.isabs(file_name):
                 file_name = os.path.join(os.path.abspath(os.path.curdir), file_name)
             elif cwd is not None:
                 file_name = os.path.join(cwd, file_name)
             self.close_connection()
             self.open_local_sqlite_connection(
@@ -156,26 +156,26 @@
     def switch_to_central_database(self):
         """
         Switch to central database
         """
         if self.using_local_database:
             self.update()
         else:
-            logger.log("Database is already in central mode or disabled!")
+            logger.info("Database is already in central mode or disabled!")
 
     def switch_to_viewer_mode(self):
         """
         Switch from user mode to viewer mode - if view_mode is enable pyiron has read only access to the database.
         """
         if (
             self.sql_view_connection_string is not None
             and not self.database_is_disabled
         ):
             if self._database.view_mode:
-                logger.log("Database is already in viewer mode!")
+                logger.info("Database is already in viewer mode!")
             else:
                 self.close_connection()
                 self._database = DatabaseAccess(
                     self.sql_view_connection_string,
                     self.sql_view_table_name,
                 )
                 self._database.view_mode = True
@@ -194,15 +194,15 @@
                 self.close_connection()
                 self._database = DatabaseAccess(
                     self.sql_connection_string,
                     self.sql_table_name,
                 )
                 self._database.view_mode = False
             else:
-                logger.log("Database is already in user mode!")
+                logger.info("Database is already in user mode!")
         else:
             print("Viewer Mode is not available on this pyiron installation.")
 
     def close_connection(self):
         """
         Internal function to close the connection to the database.
         """
```

### Comparing `pyiron_base-0.5.9/pyiron_base/database/performance.py` & `pyiron_base-0.6.0/pyiron_base/database/performance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.9/pyiron_base/database/tables.py` & `pyiron_base-0.6.0/pyiron_base/database/tables.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,32 +22,30 @@
 __version__ = "0.0"
 __maintainer__ = "Liam Huber"
 __email__ = "huber@mpie.de"
 __status__ = "development"
 __date__ = "Sep, 2021"
 
 
-class HistoricalTable(Table):
+def get_historical_table(table_name, metadata, extend_existing=True):
     """The historical table."""
-
-    def _init(self, table_name, metadata, *args, extend_existing=True, **kwargs):
-        super()._init(
-            table_name,
-            metadata,
-            Column("id", Integer, primary_key=True, autoincrement=True),
-            Column("parentid", Integer),
-            Column("masterid", Integer),
-            Column("projectpath", String(50)),
-            Column("project", String(255)),
-            Column("job", String(50)),
-            Column("subjob", String(255)),
-            Column("chemicalformula", String(50)),
-            Column("status", String(20)),
-            Column("hamilton", String(20)),
-            Column("hamversion", String(50)),
-            Column("username", String(20)),
-            Column("computer", String(100)),
-            Column("timestart", DateTime),
-            Column("timestop", DateTime),
-            Column("totalcputime", Float),
-            extend_existing=extend_existing,
-        )
+    return Table(
+        table_name,
+        metadata,
+        Column("id", Integer, primary_key=True, autoincrement=True),
+        Column("parentid", Integer),
+        Column("masterid", Integer),
+        Column("projectpath", String(50)),
+        Column("project", String(255)),
+        Column("job", String(50)),
+        Column("subjob", String(255)),
+        Column("chemicalformula", String(50)),
+        Column("status", String(20)),
+        Column("hamilton", String(20)),
+        Column("hamversion", String(50)),
+        Column("username", String(20)),
+        Column("computer", String(100)),
+        Column("timestart", DateTime),
+        Column("timestop", DateTime),
+        Column("totalcputime", Float),
+        extend_existing=extend_existing,
+    )
```

### Comparing `pyiron_base-0.5.9/pyiron_base/generic/datacontainer.py` & `pyiron_base-0.6.0/pyiron_base/storage/datacontainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import json
 import warnings
 from collections.abc import Sequence, Set, Mapping, MutableMapping
 
 import numpy as np
 import pandas
 
-from pyiron_base.generic.fileio import read, write
-from pyiron_base.generic.hdfstub import HDFStub
+from pyiron_base.storage.fileio import read, write
+from pyiron_base.storage.hdfstub import HDFStub
 from pyiron_base.interfaces.has_groups import HasGroups
 from pyiron_base.interfaces.has_hdf import HasHDF
 
 __author__ = "Marvin Poul"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
@@ -205,17 +205,28 @@
     ExtendedContainer({'foo': 1, 'bar': 5})
     >>> e.my_fancy_field = 42
     >>> e.my_fancy_field
     42
     >>> e
     ExtendedContainer({'foo': 1, 'bar': 5})
 
-    Or a class that uses a DataContainer for storage, but doesn't derive from it.
+    Be aware the :class:`.DataContainer` and its subclasses are recursive data structures, i.e. your fancy attribute
+    will be available also on sub groups.
 
-    >>> from pyiron_base.generic.object import HasStorage
+    >>> g = e.create_group('sub')
+    >>> g.fnord = 23
+    >>> g.my_fancy_field
+    42
+    >>> e
+    ExtendedContainer({'foo': 1, 'bar': 5, 'sub': ExtendedContainer({'fnord': 23})})
+
+    For that reason most of time you'll actually want a class that uses a DataContainer for storage, but doesn't derive
+    from it.
+
+    >>> from pyiron_base.interfaces.object import HasStorage
     >>> class FancyClass(HasStorage):
     ...     def __init__(self, foo):
     ...         super().__init__()
     ...         self.storage.foo = foo
     ...
     ...     @property
     ...     def foo(self):
@@ -230,15 +241,14 @@
 
     """
 
     __version__ = "0.1.0"
     __hdf_version__ = "0.2.0"
 
     def __new__(cls, *args, **kwargs):
-
         instance = super().__new__(cls)
         # setting these immediately after object creation ensures that they are
         # always defined and attribute access works even before __init__ is
         # called.  This is relevant on deepcopy & pickling.
         object.__setattr__(instance, "_store", [])
         object.__setattr__(instance, "_indices", {})
         object.__setattr__(instance, "table_name", None)
@@ -264,22 +274,20 @@
         if init is not None:
             self.update(init, wrap=True, blacklist=wrap_blacklist)
 
     def __len__(self):
         return len(self._store)
 
     def __iter__(self):
-
         reverse_indices = {i: k for k, i in self._indices.items()}
 
         for i in range(len(self)):
             yield reverse_indices.get(i, i)
 
     def __getitem__(self, key):
-
         key = _normalize(key)
 
         if isinstance(key, tuple):
             if key[0] == "..." and len(key) > 1:
                 res = self.search(key[1], False)
                 return res if (len(key) == 2) else res[key[2:]]
             return self[key[0]][key[1:]]
@@ -306,15 +314,14 @@
             except KeyError:
                 raise KeyError(repr(key)) from None
 
         else:
             raise ValueError("{} is not a valid key, must be str or int".format(key))
 
     def __setitem__(self, key, val):
-
         if self.read_only:
             self._read_only_error()
 
         key = _normalize(key)
 
         if isinstance(key, tuple):
             if key[0] == "..." and len(key) > 1:
@@ -337,15 +344,14 @@
                 self._store.append(val)
             else:
                 self._store[self._indices[key]] = val
         else:
             raise ValueError("{} is not a valid key, must be str or int".format(key))
 
     def __delitem__(self, key):
-
         if self.read_only:
             self._read_only_error()
 
         key = _normalize(key)
 
         if isinstance(key, tuple):
             if key[0] == "..." and len(key) > 1:
@@ -767,55 +773,72 @@
         >>> pl.copy() == pl
         True
         >>> pl.copy() is pl
         False
         >>> all(a is not b for a, b in zip(pl.copy().values(), pl.values()))
         True
         """
+        self._force_load()
         return copy.deepcopy(self)
 
     def _get_hdf_group_name(self):
         return self.table_name
 
     def _to_hdf(self, hdf):
         hdf["READ_ONLY"] = self.read_only
+        written_keys = _internal_hdf_nodes.copy()
         for i, (k, v) in enumerate(self.items()):
             if isinstance(k, str) and "__index_" in k:
                 raise ValueError("Key {} clashes with internal use!".format(k))
 
             k = "{}__index_{}".format(k if isinstance(k, str) else "", i)
+            written_keys.append(k)
 
             # pandas objects also have a to_hdf method that is entirely unrelated to ours
             if hasattr(v, "to_hdf") and not isinstance(
                 v, (pandas.DataFrame, pandas.Series)
             ):
+                # if v will be written as a group, but a node of the same name k exists already in the file, h5py will
+                # complain, so delete it first
+                if k in hdf.list_nodes():
+                    del hdf[k]
                 v.to_hdf(hdf=hdf, group_name=k)
             else:
                 # if the value doesn't know how to serialize itself, assume
                 # that h5py knows how to
                 try:
                     hdf[k] = v
                 except TypeError:
                     raise TypeError(
                         "Error saving {} (key {}): DataContainer doesn't support saving elements "
                         'of type "{}" to HDF!'.format(v, k, type(v))
                     ) from None
+        for n in hdf.list_nodes():
+            if n not in written_keys:
+                del hdf[n]
+        for g in hdf.list_groups():
+            if g not in written_keys:
+                del hdf[g]
 
     def _from_hdf(self, hdf, version=None):
         self.clear()
 
         if version == "0.1.0":
             self.update(hdf["data"], wrap=True)
             self.read_only = bool(hdf.get("read_only", False))
         else:
 
             def normalize_key(name):
                 # split a dataset/group name into the position in the list and
                 # the key
-                k, i = name.split("__index_", maxsplit=1)
+                if "__index_" in name:
+                    k, i = name.split("__index_", maxsplit=1)
+                else:
+                    k = name
+                    i = -1
                 i = int(i)
                 if k == "":
                     return i, i
                 else:
                     return i, k
 
             items = []
@@ -890,14 +913,29 @@
         For supported file types, see :func:`.fileio.write`.
 
         Args:
             file_name(str): the name of the file to be writen to.
         """
         write(self.to_builtin(), file_name)
 
+    def _force_load(self, recursive=True):
+        """
+        Load all HDFStubs present in the data container.
+
+        Args:
+            recursive (bool): force also nested data containers, default True
+        """
+        if not self._lazy and not recursive:
+            return
+
+        # values are loaded from HDF once they are accessed via __getitem__, which is implicitly called by values()
+        for v in self.values():
+            if recursive and isinstance(v, DataContainer):
+                v._force_load()
+
     def __init_subclass__(cls):
         # called whenever a subclass of DataContainer is defined, then register all subclasses with the same function
         # that the DataContainer is registered
         HDFStub.register(cls, lambda h, g: h[g].to_object(lazy=True))
 
 
 HDFStub.register(DataContainer, lambda h, g: h[g].to_object(lazy=True))
```

### Comparing `pyiron_base-0.5.9/pyiron_base/generic/factory.py` & `pyiron_base-0.6.0/pyiron_base/interfaces/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.9/pyiron_base/generic/filedata.py` & `pyiron_base-0.6.0/pyiron_base/storage/filedata.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import json
 import os
 from abc import ABC, abstractmethod
 from functools import lru_cache
 
 import pandas
 
-from pyiron_base import ImportAlarm, FileHDFio, ProjectHDFio
+from pyiron_base.storage.hdfio import FileHDFio, ProjectHDFio
+from pyiron_base.utils.error import ImportAlarm
 
 __author__ = "Niklas Siemer"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "0.1"
@@ -48,26 +49,89 @@
         + str(
             [package for package in _has_imported.keys() if not _has_imported[package]]
         )
         + " could not be imported."
     )
 
 
+def _load_txt(file):
+    if isinstance(file, str):
+        with open(file, encoding="utf8") as f:
+            return f.readlines()
+    else:
+        return file.readlines()
+
+
+def _load_json(file):
+    if isinstance(file, str):
+        with open(file) as f:
+            return json.load(f)
+    else:
+        return json.load(file)
+
+
+class FileLoader:
+    _file_types = {
+        ".json": _load_json,
+        ".txt": _load_txt,
+        ".csv": pandas.read_csv,
+    }
+    default_assumed_file_type = ".txt"
+
+    @classmethod
+    def register(cls, file_type, load_callable):
+        """Register a load function for a specific file type.
+
+        Args:
+            file_type(str): File extension to be registered, e.g. '.txt', '.csv'
+            load_callable(callable): function excepting a file or file-handle, returning an appropriate object for
+                this file type.
+
+        """
+        cls._file_types[file_type] = load_callable
+
+    def load(self, file_type, file, *args, **kwargs):
+        if file_type in self._file_types:
+            return self._file_types[file_type](file, *args, **kwargs)
+        else:
+            return self._load_default(file, *args, **kwargs)
+
+    def _load_default(self, file, *args, **kwargs):
+        try:
+            return self._file_types[self.default_assumed_file_type](
+                file, *args, **kwargs
+            )
+        except Exception as e:
+            raise IOError("File could not be loaded.") from e
+
+
+if _has_imported["PIL"]:
+    for ext in Image.registered_extensions():
+        FileLoader.register(ext, Image.open)
+
+
 if _has_imported["nbformat"]:
 
     class OwnNotebookNode(nbformat.NotebookNode):
 
         """Wrapper for nbformat.NotebookNode with some additional representation based on nbconvert."""
 
         def _repr_html_(self):
             html_exporter = nbconvert.HTMLExporter()
             html_exporter.template_name = "classic"
             (html_output, _) = html_exporter.from_notebook_node(self)
             return html_output
 
+    def _load_ipynb(file):
+        return OwnNotebookNode(nbformat.read(file, as_version=4))
+
+    FileLoader.register(".ipynb", _load_ipynb)
+
+_file_loader = FileLoader()
+
 
 @import_alarm
 def load_file(fp, filetype=None, project=None):
     """
     Load the file and return an appropriate object containing the data.
 
     Args:
@@ -80,50 +144,21 @@
         '.json'
         '.txt'
         '.csv'
         '.ipynb'
         Image extensions supported by PIL
 
     Returns:
-        :class:`FileHDFio`: pointing to the file of filetype = '.h5'
-        dict: containing data from file of filetype = '.json'
+        :class:`FileHDFio`/:class:`ProjectHDFio`: pointing to the file of filetype = '.h5'
+        dict/list: containing data from file of filetype = '.json'
         list: of all lines from file for filetype = '.txt'
         :class:`pandas.DataFrame`: containing data from file of filetype = '.csv'
 
     """
 
-    def _load_txt(file):
-        if isinstance(file, str):
-            with open(file, encoding="utf8") as f:
-                return f.readlines()
-        else:
-            return file.readlines()
-
-    def _load_ipynb(file):
-        return OwnNotebookNode(nbformat.read(file, as_version=4))
-
-    def _load_json(file):
-        if isinstance(file, str):
-            with open(file) as f:
-                return json.load(f)
-        else:
-            return json.load(file)
-
-    def _load_csv(file):
-        return pandas.read_csv(file)
-
-    def _load_img(file):
-        return Image.open(file)
-
-    def _load_default(file):
-        try:
-            return _load_txt(file)
-        except Exception as e:
-            raise IOError("File could not be loaded.") from e
-
     def _resolve_filetype(file, _filetype):
         if _filetype is None and isinstance(file, str):
             _, _filetype = os.path.splitext(file)
         elif _filetype is None and hasattr(file, "name"):
             _, _filetype = os.path.splitext(file.name)
         elif _filetype is None:
             return None
@@ -134,49 +169,43 @@
     filetype = _resolve_filetype(fp, filetype)
 
     if filetype in [".h5", ".hdf"] and isinstance(fp, str):
         if project is None:
             return FileHDFio(file_name=fp)
         else:
             return ProjectHDFio(file_name=fp, project=project)
-    elif filetype in [".json"]:
-        return _load_json(fp)
-    elif filetype in [".txt"]:
-        return _load_txt(fp)
-    elif filetype in [".csv"]:
-        return _load_csv(fp)
-    elif _has_imported["nbformat"] and filetype in [".ipynb"]:
-        return _load_ipynb(fp)
-    elif _has_imported["PIL"] and filetype in Image.registered_extensions():
-        return _load_img(fp)
     else:
-        return _load_default(fp)
+        return _file_loader.load(filetype, fp)
 
 
 class FileDataTemplate(ABC):
     @property
     @abstractmethod
     def data(self):
         """Return the associated data."""
         pass
 
 
 class FileData(FileDataTemplate):
     """FileData stores an instance of a data file, e.g. a single Image from a measurement."""
 
-    def __init__(self, file, data=None, metadata=None, filetype=None):
+    def __init__(
+        self, file, data=None, metadata=None, filetype=None, pyiron_project=None
+    ):
         """FileData class to store data and associated metadata.
 
         Args:
             file (str): path to the data file (if data is None) or filename associated with the data.
             data (object/None): object containing data
             metadata (dict/DataContainer): Dictionary of metadata associated with the data
             filetype (str): File extension associated with the type data,
                             If provided this overwrites the assumption based on the extension of the filename.
+            pyiron_project(Project): Project this file belongs to, if any, used to load files with project awareness.
         """
+        self._project = pyiron_project
         if data is None:
             self.filename = os.path.split(file)[1]
             self.source = file
             self._data = None
         else:
             self.filename = file
             self.source = None
@@ -198,8 +227,8 @@
     @property
     @lru_cache()
     def data(self):
         """Return the associated data."""
         if self._hasdata:
             return self._data
         else:
-            return load_file(self.source, filetype=self.filetype)
+            return load_file(self.source, filetype=self.filetype, project=self._project)
```

### Comparing `pyiron_base-0.5.9/pyiron_base/generic/fileio.py` & `pyiron_base-0.6.0/pyiron_base/storage/fileio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Functions for reading and writing data files.
 """
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
-import ast
 from collections import namedtuple
 import os.path
 import yaml
 import warnings
 
 
 __author__ = "Muhammad Hassani, Marvin Poul"
```

### Comparing `pyiron_base-0.5.9/pyiron_base/generic/flattenedstorage.py` & `pyiron_base-0.6.0/pyiron_base/storage/flattenedstorage.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,39 @@
 __maintainer__ = "Marvin Poul"
 __email__ = "poul@mpie.de"
 __status__ = "production"
 __date__ = "Jul 16, 2020"
 
 
 import copy
-from typing import Callable, Iterable, List
+import warnings
+from typing import Callable, Iterable, List, Tuple, Any
 
 import numpy as np
 import h5py
 from pyiron_base.interfaces.has_hdf import HasHDF
 
 
+def _ensure_str_array_size(array, strlen):
+    """
+    Ensures that the given array can store at least string of length `strlen`.
+
+    Args:
+        array (ndarray): array of dtype <U
+        strlen (int): maximum length that should fit in it
+    Returns:
+        ndarray: either `array` or resized copy
+    """
+    current_length = array.itemsize // np.dtype("1U").itemsize
+    if current_length < strlen:
+        return array.astype(f"{2 * strlen}U")
+    else:
+        return array
+
+
 class FlattenedStorage(HasHDF):
     """
     Efficient storage of ragged arrays in flattened arrays.
 
     This class stores multiple arrays at the same time.  Storage is organized in "chunks" that may be of any size, but
     all arrays within chunk are of the same size, e.g.
 
@@ -176,14 +194,29 @@
     array([ 7,  9, 11])
     >>> len(store)
     3
     """
 
     __version__ = "0.2.0"
     __hdf_version__ = "0.3.0"
+    _default_fill_values = {
+        np.dtype("int8"): -1,
+        np.dtype("int16"): -1,
+        np.dtype("int32"): -1,
+        np.dtype("int64"): -1,
+        np.dtype("float16"): np.nan,
+        np.dtype("float32"): np.nan,
+        np.dtype("float64"): np.nan,
+        np.dtype("object"): None,
+        np.dtype("uint8"): 0,
+        np.dtype("uint16"): 0,
+        np.dtype("uint32"): 0,
+        np.dtype("uint64"): 0,
+        str: "_default",
+    }
 
     def __init__(self, num_chunks=1, num_elements=1, **kwargs):
         """
         Create new flattened storage.
 
         Args:
             num_chunks (int): pre-allocation for per chunk arrays
@@ -222,16 +255,18 @@
                 raise ValueError("Inconsistent chunk length in initializer!")
             self.add_chunk(chunk_length, **{k: c for k, c in zip(keys, chunk_list)})
 
     def _init_arrays(self):
         self._per_element_arrays = {}
 
         self._per_chunk_arrays = {
-            "start_index": np.empty(self._num_chunks_alloc, dtype=np.int32),
-            "length": np.empty(self._num_chunks_alloc, dtype=np.int32),
+            "start_index": np.full(
+                self._num_chunks_alloc, dtype=np.int32, fill_value=0
+            ),
+            "length": np.full(self._num_chunks_alloc, dtype=np.int32, fill_value=0),
             "identifier": np.empty(self._num_chunks_alloc, dtype=np.dtype("U20")),
         }
 
     def __len__(self):
         return self.current_chunk_index
 
     def copy(self):
@@ -374,22 +409,16 @@
             raise ValueError(f'per must "element" or "chunk", not {per}')
 
         if fill is None:
             store[name] = np.empty(shape=shape, dtype=dtype)
         else:
             store[name] = np.full(shape=shape, fill_value=fill, dtype=dtype)
 
-        _default_fill_values = {
-            np.dtype("int32"): -1,
-            np.dtype("int64"): -1,
-            np.dtype("float32"): np.nan,
-            np.dtype("float64"): np.nan,
-        }
-        if fill is None and store[name].dtype in _default_fill_values:
-            fill = _default_fill_values[store[name].dtype]
+        if fill is None and store[name].dtype in self._default_fill_values:
+            fill = self._default_fill_values[store[name].dtype]
         if fill is not None:
             self._fill_values[name] = fill
 
     def get_array(self, name, frame=None):
         """
         Fetch array for given structure.
 
@@ -492,45 +521,29 @@
             frame (int, str): selects structure to set, as in :method:`.get_strucure()`
             value: value (for per chunk) or array of values (for per element); type and shape as per :meth:`.hasarray()`.
 
         Raises:
             `KeyError`: if array with name does not exists
         """
 
-        def ensure_str_array_size(array, strlen):
-            """
-            Ensures that the given array can store at least string of length `strlen`.
-
-            Args:
-                array (ndarray): array of dtype <U
-                strlen (int): maximum length that should fit in it
-            Returns:
-                ndarray: either `array` or resized copy
-            """
-            current_length = array.itemsize // np.dtype("1U").itemsize
-            if current_length < strlen:
-                return array.astype(f"{2 * strlen}U")
-            else:
-                return array
-
         if isinstance(frame, str):
             frame = self.find_chunk(frame)
         if name in self._per_element_arrays:
             if self._per_element_arrays[name].dtype.char == "U":
-                self._per_element_arrays[name] = ensure_str_array_size(
+                self._per_element_arrays[name] = _ensure_str_array_size(
                     self._per_element_arrays[name], max(map(len, value))
                 )
             self._per_element_arrays[name][self._get_per_element_slice(frame)] = value
         elif name in self._per_chunk_arrays:
             if self._per_chunk_arrays[name].dtype.char == "U":
                 if isinstance(value, np.ndarray) and value.ndim == 0:
                     strlen = len(value.item())
                 else:
                     strlen = len(value)
-                self._per_chunk_arrays[name] = ensure_str_array_size(
+                self._per_chunk_arrays[name] = _ensure_str_array_size(
                     self._per_chunk_arrays[name], strlen
                 )
             self._per_chunk_arrays[name][frame] = value
         else:
             raise KeyError(f"no array named {name}")
 
     def __getitem__(self, index):
@@ -761,14 +774,17 @@
         # len of chunk to index into the initialized arrays
         i = self.current_element_index + n
 
         self._per_chunk_arrays["start_index"][
             self.current_chunk_index
         ] = self.current_element_index
         self._per_chunk_arrays["length"][self.current_chunk_index] = n
+        self._per_chunk_arrays["identifier"] = _ensure_str_array_size(
+            self._per_chunk_arrays["identifier"], len(identifier)
+        )
         self._per_chunk_arrays["identifier"][self.current_chunk_index] = identifier
 
         for k, a in arrays.items():
             a = np.asarray(a)
             if k not in self._per_element_arrays and k not in self._per_chunk_arrays:
                 if len(a.shape) > 0 and a.shape[0] == n:
                     self.add_array(k, shape=a.shape[1:], dtype=a.dtype, per="element")
@@ -788,14 +804,77 @@
         self.prev_element_index = self.current_element_index
 
         # Set new current_element_index and increase current_chunk_index
         self.current_chunk_index += 1
         self.current_element_index = i
         # return last_chunk_index, last_element_index
 
+    def extend(self, other: "FlattenedStorage"):
+        self._check_compatible_fill_values(other=other)
+
+        combined_num_chunks = self.num_chunks + other.num_chunks
+        combined_num_elements = self.num_elements + other.num_elements
+        if combined_num_chunks > self._num_chunks_alloc:
+            self._resize_chunks(combined_num_chunks)
+        if combined_num_elements > self._num_elements_alloc:
+            self._resize_elements(combined_num_elements)
+
+        for k, a in other._per_chunk_arrays.items():
+            # add start_index of last chunk to start_index of other for correct mapping
+            if (
+                k == "start_index" and len(self) > 0
+            ):  # Check if len > 0 to ensure that no random values are accessed for length and start_index after empty init
+                last = self.num_chunks - 1
+                len_last = self._per_chunk_arrays["length"][last]
+                a = (
+                    a + self._per_chunk_arrays[k][last] + len_last
+                )  # no += to prevent inplace mutation
+            if k not in self._per_chunk_arrays.keys():
+                dtype, fill = get_dtype_and_fill(storage=other, name=k)
+                self.add_array(
+                    name=k, dtype=dtype, shape=a.shape[1:], fill=fill, per="chunk"
+                )
+            self._per_chunk_arrays[k][self.num_chunks : combined_num_chunks] = a[
+                0 : other.num_chunks
+            ]
+
+        for k, a in other._per_element_arrays.items():
+            if k not in self._per_element_arrays.keys():
+                dtype, fill = get_dtype_and_fill(storage=other, name=k)
+                self.add_array(
+                    name=k, shape=a.shape[1:], dtype=dtype, fill=fill, per="element"
+                )
+            self._per_element_arrays[k][self.num_elements : combined_num_elements] = a[
+                0 : other.num_elements
+            ]
+        self.num_elements = combined_num_elements
+        self.num_chunks = combined_num_chunks
+        self.current_chunk_index = self.num_chunks
+        self.current_element_index = self.num_elements
+
+    def _check_compatible_fill_values(self, other: "FlattenedStorage"):
+        """
+        Check if fill values of 2 FlattenedStorages match to prevent errors due to wrong fill values,
+        f.e. after extending to the storage.
+
+        Args:
+            other (FlattenedStorage): Another FlattenedStorage instance
+
+        Raises:
+            ValueError: Raises when the storages have different fill values for a key
+        """
+        for k in set(self._fill_values).intersection(other._fill_values):
+            if np.isnan(self._fill_values[k]) and np.isnan(other._fill_values[k]):
+                continue
+            else:
+                if self._fill_values[k] != other._fill_values[k]:
+                    raise ValueError(
+                        "Fill values for arrays in storages don't match, can't perform requested operation"
+                    )
+
     def _get_hdf_group_name(self):
         return "flat_storage"
 
     def _to_hdf(self, hdf):
         def write_array(name, array, hdf):
             if array.dtype.char == "U":
                 # numpy stores unicode data in UTF-32/UCS-4, but h5py wants UTF-8, so we manually encode them here
@@ -827,20 +906,20 @@
         for k, a in self._per_chunk_arrays.items():
             write_array(k, a, hdf_arrays)
 
         hdf["_fill_values"] = self._fill_values
 
     def _from_hdf(self, hdf, version=None):
         def read_array(name, hdf):
-            a = np.array(hdf[name])
+            a = np.asarray(hdf[name])
             if a.dtype.char == "S":
                 # if saved as bytes, we wrote this as an encoded unicode string, so manually decode here
                 # TODO: string arrays with shape != () not handled
-                a = np.array(
-                    [s.decode("utf8") for s in a],
+                a = np.fromiter(
+                    (s.decode("utf8") for s in a),
                     # itemsize of original a is four bytes per character, so divide by four to get
                     # length of the orignal stored unicode string; np.dtype('U1').itemsize is just a
                     # platform agnostic way of knowing how wide a unicode charater is for numpy
                     dtype=f"U{a.dtype.itemsize//np.dtype('U1').itemsize}",
                 )
             return a
 
@@ -887,7 +966,27 @@
                 raise RuntimeError(
                     f"per-element array {k} read inconsistently from HDF: "
                     f"shape {a.shape[0]} does not match global allocation {self._num_elements_alloc}!"
                 )
 
         if version >= "0.3.0":
             self._fill_values = hdf["_fill_values"]
+
+
+def get_dtype_and_fill(storage: FlattenedStorage, name: str) -> Tuple[np.generic, Any]:
+    fill = None
+    if name in storage._fill_values.keys():
+        fill = storage._fill_values[name]
+        dtype = type(fill)
+    else:
+        a = storage.get_array(name)
+        if a.dtype.char == "U":
+            dtype = str
+        else:
+            dtype = a.dtype
+        try:
+            fill = FlattenedStorage._default_fill_values[dtype]
+        except KeyError:
+            raise ValueError(
+                f"Could not determine a default fill value for array {name}"
+            )
+    return dtype, fill
```

### Comparing `pyiron_base-0.5.9/pyiron_base/generic/hdfio.py` & `pyiron_base-0.6.0/pyiron_base/storage/hdfio.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 import numbers
 import h5py
 import os
 from collections.abc import MutableMapping
 import importlib
 import pandas
 import posixpath
-import h5io
 import numpy as np
 import sys
 from typing import Union
 
-from pyiron_base.generic.util import deprecate
-
+from pyiron_base.utils.deprecate import deprecate
+from pyiron_base.storage.helper_functions import read_hdf5, write_hdf5
 from pyiron_base.interfaces.has_groups import HasGroups
 from pyiron_base.state import state
-from pyiron_base.generic.dynamic import JOB_DYN_DICT, class_constructor
+from pyiron_base.jobs.dynamic import JOB_DYN_DICT, class_constructor
+from pyiron_base.jobs.job.util import _get_safe_job_name
 import warnings
 
 __author__ = "Joerg Neugebauer, Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -145,19 +145,19 @@
                 # fast path, a good amount of accesses will want to fetch a specific dataset it knows exists in the
                 # file, there's therefor no point in checking whether item is a group or a node or even worse recursing
                 # in case when item contains '/'.  In most cases read_hdf5 will grab the correct data straight away and
                 # if not we will still check thoroughly below.  Since list_nodes()/list_groups() each open the
                 # underlying file once, this reduces the number of file opens in the most-likely case from 2 to 1 (1 to
                 # check whether the data is there and 1 to read it) and increases in the worst case from 1 to 2 (1 to
                 # try to read it here and one more time to verify it's not a group below).
-                obj = h5io.read_hdf5(self.file_name, title=self._get_h5_path(item))
+                obj = read_hdf5(self.file_name, title=self._get_h5_path(item))
                 if self._is_convertable_dtype_object_array(obj):
                     obj = self._convert_dtype_obj_array(obj.copy())
                 return obj
-            except (ValueError, OSError):
+            except (ValueError, OSError, RuntimeError, NotImplementedError):
                 # h5io couldn't find a dataset with name item, but there still might be a group with that name, which we
                 # check in the rest of the method
                 pass
 
             item_lst = item.split("/")
             if len(item_lst) == 1 and item_lst[0] != "..":
                 # if item in self.list_nodes() we would have caught it in the fast path above
@@ -212,15 +212,18 @@
             ):
                 return True
         return False
 
     # TODO: remove this function upon 1.0.0 release
     @staticmethod
     def _convert_dtype_obj_array(obj: np.ndarray):
-        result = np.array(obj.tolist())
+        try:
+            result = np.array(obj.tolist())
+        except ValueError:
+            result = np.array(obj.tolist(), dtype=object)
         if result.dtype != np.dtype(object):
             state.logger.warning(
                 f"Deprecated data structure! "
                 f"Returned array was converted from dtype='O' to dtype={result.dtype} "
                 f"via `np.array(result.tolist())`.\n"
                 f"Please run rewrite_hdf5() (from a job: job.project_hdf5.rewrite_hdf5() ) to update this data! "
                 f"To update all your data run Project.maintenance.update.base_v0_3_to_v0_4('all')."
@@ -233,53 +236,55 @@
         """
         Store data inside the HDF5 file
 
         Args:
             key (str): key to store the data
             value (pandas.DataFrame, pandas.Series, dict, list, float, int): basically any kind of data is supported
         """
-        use_json = True
         if hasattr(value, "to_hdf") & (
             not isinstance(value, (pandas.DataFrame, pandas.Series))
         ):
             value.to_hdf(self, key)
-        elif (
+            return
+
+        use_json = True
+        if (
             isinstance(value, (list, np.ndarray))
             and len(value) > 0
             and isinstance(value[0], (list, np.ndarray))
             and len(value[0]) > 0
             and not isinstance(value[0][0], str)
             and _is_ragged_in_1st_dim_only(value)
         ):
             # if the sub-arrays in value all share shape[1:], h5io comes up with a more efficient storage format than
             # just writing a dataset for each element, by concatenating along the first axis and storing the indices
             # where to break the concatenated array again
             value = np.array([np.asarray(v) for v in value], dtype=object)
             use_json = False
         elif isinstance(value, tuple):
             value = list(value)
-        h5io.write_hdf5(
+        write_hdf5(
             self.file_name,
             value,
-            title=posixpath.join(self.h5_path, key),
+            title=self._get_h5_path(key),
             overwrite="update",
             use_json=use_json,
         )
 
     def __delitem__(self, key):
         """
         Delete item from the HDF5 file
 
         Args:
             key (str): key of the item to delete
         """
         if self.file_exists:
             try:
                 with open_hdf5(self.file_name, mode="a") as store:
-                    del store[key]
+                    del store[self._get_h5_path(key)]
             except (AttributeError, KeyError):
                 pass
 
     @property
     def file_exists(self):
         """
         Check if the HDF5 file exists already
@@ -527,15 +532,15 @@
             name (str): name of the HDF5 group
             track_order (bool): if False this groups tracks its elements in
                 alphanumeric order, if True in insertion order
 
         Returns:
             FileHDFio: FileHDFio object pointing to the new group
         """
-        full_name = posixpath.join(self.h5_path, name)
+        full_name = self._get_h5_path(name)
         with open_hdf5(self.file_name, mode="a") as h:
             try:
                 h.create_group(full_name, track_order=track_order)
             except ValueError:
                 pass
         h_new = self[name].copy()
         return h_new
@@ -566,15 +571,15 @@
             raise ValueError(
                 "Absolute paths are not supported -> replace by relative path name!"
             )
 
         if h5_rel_path.strip() == ".":
             h5_rel_path = ""
         if h5_rel_path.strip() != "":
-            new_h5_path.h5_path = posixpath.join(new_h5_path.h5_path, h5_rel_path)
+            new_h5_path.h5_path = self._get_h5_path(h5_rel_path)
         new_h5_path.history.append(h5_rel_path)
 
         return new_h5_path
 
     def close(self):
         """
         Close the current HDF5 path and return to the path before the last open
@@ -897,15 +902,15 @@
 
         Args:
             item (str): path to the data or key of the data object
 
         Returns:
             dict, list, float, int: data or data object
         """
-        return h5io.read_hdf5(self.file_name, title=self._get_h5_path(item))
+        return read_hdf5(self.file_name, title=self._get_h5_path(item))
 
     # def _open_store(self, mode="r"):
     #     """
     #     Internal function to open the HDF5 file
     #
     #     Args:
     #         mode (str): file mode can be either 'w': write, 'r': read or 'a': append
@@ -1087,16 +1092,15 @@
 
         .. attribute:: working_directory
 
             working directory of the job is executed in - outside the HDF5 file
     """
 
     def __init__(self, project, file_name, h5_path=None, mode=None):
-        file_name += ".h5" if not file_name.endswith(".h5") else ""
-        self._file_name = file_name.replace("\\", "/")
+        self._file_name = _get_safe_filename(file_name)
         if h5_path is None:
             h5_path = "/"
         self._project = project.copy()
         super(ProjectHDFio, self).__init__(
             file_name=os.path.join(self._project.path, self._file_name).replace(
                 "\\", "/"
             ),
@@ -1290,34 +1294,39 @@
         """
         return self._project.create_hdf(path=path, job_name=job_name)
 
     def create_working_directory(self):
         """
         Create the working directory on the file system if it does not exist already.
         """
-        if not os.path.isdir(self.working_directory):
-            os.makedirs(self.working_directory)
+        os.makedirs(self.working_directory, exist_ok=True)
 
     def import_class(self, class_name):
         """
         Import given class from fully qualified name and return class object.
 
         Args:
             class_name (str): fully qualified name of a pyiron class
 
         Returns:
             type: class object of the given name
         """
         internal_class_name = class_name.split(".")[-1][:-2]
+        class_path = class_name.split()[-1].split(".")[:-1]
+        class_path[0] = class_path[0][1:]
+        class_module_path = ".".join(class_path)
         if internal_class_name in self._project.job_type.job_class_dict:
             module_path = self._project.job_type.job_class_dict[internal_class_name]
+            if class_module_path != module_path:
+                state.logger.info(
+                    f'Using registered module "{module_path}" instead of custom/old module "{class_module_path}" to'
+                    f' import job type "{internal_class_name}"!'
+                )
         else:
-            class_path = class_name.split()[-1].split(".")[:-1]
-            class_path[0] = class_path[0][1:]
-            module_path = ".".join(class_path)
+            module_path = class_module_path
         return getattr(
             importlib.import_module(module_path),
             internal_class_name,
         )
 
     def create_instance(self, cls, **kwargs):
         """
@@ -1362,15 +1371,23 @@
             raise ValueError("Objects can be only recovered from hdf5 if TYPE is given")
         elif class_name is not None and class_name != self.get("TYPE"):
             raise ValueError(
                 "Object type in hdf5-file must be identical to input parameter"
             )
         class_name = class_name or self.get("TYPE")
         class_path = class_name.split("<class '")[-1].split("'>")[0]
-        if not class_path.startswith("abc."):
+        class_convert_dict = {  # Fix backwards compatibility
+            "pyiron_base.generic.datacontainer.DataContainer": "pyiron_base.storage.datacontainer.DataContainer",
+            "pyiron_base.generic.inputlist.InputList": "pyiron_base.storage.inputlist.InputList",
+            "pyiron_base.generic.flattenedstorage.FlattenedStorage": "pyiron_base.storage.flattenedstorage.FlattenedStorage",
+        }
+        if class_path in class_convert_dict.keys():
+            class_name_new = "<class '" + class_convert_dict[class_path] + "'>"
+            class_object = self.import_class(class_name_new)
+        elif not class_path.startswith("abc."):
             class_object = self.import_class(class_name)
         else:
             class_object = class_constructor(cp=JOB_DYN_DICT[class_path.split(".")[-1]])
 
         # Backwards compatibility since the format of TYPE changed
         if class_name != str(class_object):
             self["TYPE"] = str(class_object)
@@ -1453,7 +1470,18 @@
         """
         Internal function to create a pyiron project pointing to the directory where the HDF5 file is located.
 
         Returns:
             Project: pyiron project object
         """
         return self._project.__class__(path=self.file_path)
+
+
+def _get_safe_filename(file_name):
+    file_path_no_ext, file_ext = os.path.splitext(file_name)
+    file_path = os.path.dirname(file_path_no_ext)
+    file_name_no_ext = os.path.basename(file_path_no_ext)
+    file_name = os.path.join(
+        file_path, _get_safe_job_name(name=file_name_no_ext) + file_ext
+    )
+    file_name += ".h5" if not file_name.endswith(".h5") else ""
+    return file_name.replace("\\", "/")
```

### Comparing `pyiron_base-0.5.9/pyiron_base/generic/hdfstub.py` & `pyiron_base-0.6.0/pyiron_base/storage/hdfstub.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.9/pyiron_base/generic/jedi.py` & `pyiron_base-0.6.0/pyiron_base/utils/jedi.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.9/pyiron_base/generic/object.py` & `pyiron_base-0.6.0/pyiron_base/interfaces/object.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 """
 The core class in pyiron, linking python to the database to file storage.
 """
 
 from abc import ABC
-from pyiron_base.generic.datacontainer import DataContainer
+from pyiron_base.storage.datacontainer import DataContainer
 from pyiron_base.interfaces.has_hdf import HasHDF
-from pyiron_base.generic.hdfio import ProjectHDFio
+from pyiron_base.storage.hdfio import ProjectHDFio
 from pyiron_base.state import state
 
 __author__ = "Liam Huber"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -23,23 +23,36 @@
 __status__ = "development"
 __date__ = "Mar 23, 2021"
 
 
 class HasStorage(HasHDF, ABC):
     """
     A base class for objects that use HDF5 data serialization via the `DataContainer` class.
+
+    Unless you know what you are doing sub classes should pass the `group_name` argument to :meth:`~.__init__` or
+    override :meth:`~.get_hdf_group_name()` to force a default name for the HDF group the object should write itself to.
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, group_name=None, **kwargs):
+        """
+
+        Args:
+            group_name (str): default name of the HDF group where the whole object should be written to.
+        """
+        super().__init__(*args, **kwargs)
         self._storage = DataContainer(table_name="storage")
+        self._group_name = group_name
 
     @property
     def storage(self) -> DataContainer:
         return self._storage
 
+    def _get_hdf_group_name(self) -> str:
+        return self._group_name
+
     def _to_hdf(self, hdf: ProjectHDFio):
         self.storage.to_hdf(hdf=hdf)
 
     def _from_hdf(self, hdf: ProjectHDFio, version: str = None):
         self.storage.from_hdf(hdf=hdf)
```

### Comparing `pyiron_base-0.5.9/pyiron_base/generic/parameters.py` & `pyiron_base-0.6.0/pyiron_base/storage/parameters.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.9/pyiron_base/generic/units.py` & `pyiron_base-0.6.0/pyiron_base/utils/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     Module to record units for physical quantities within pyiron. This module is used for defining the units
     for different pyiron submodules.
 
     Useage:
 
     >>> import pint
-    >>> from pyiron_base.generic.units import PyironUnitRegistry
+    >>> from pyiron_base.utils.units import PyironUnitRegistry
     >>> pint_registry = pint.UnitRegistry()
 
     After instantiating, the `pint` units for different physical quantities can be registered as follows
 
     >>> base_registry = PyironUnitRegistry()
     >>> base_registry.add_quantity(quantity="energy", unit=pint_registry.eV, data_type=float)
 
@@ -88,15 +88,15 @@
 
         Args:
             quantity (str): The physical quantity
             unit (pint.unit.Unit/pint.quantity.Quantity): `pint` unit or quantity
             data_type (type): Data type in which the quantity has to be stored
 
         """
-        if not isinstance(unit, (pint.unit.Unit, pint.quantity.Quantity)):
+        if not isinstance(unit, (pint.Unit, pint.Quantity)):
             raise ValueError("The unit should be a `pint` unit or quantity")
         self._unit_dict[quantity] = unit
         self._dtype_dict[quantity] = data_type
 
     def add_labels(self, labels, quantity):
         """
         Maps quantities with different labels to quantities already defined in the registry
```

### Comparing `pyiron_base-0.5.9/pyiron_base/interfaces/has_groups.py` & `pyiron_base-0.6.0/pyiron_base/interfaces/has_groups.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.9/pyiron_base/interfaces/has_hdf.py` & `pyiron_base-0.6.0/pyiron_base/interfaces/has_hdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """Interface for classes to serialize to HDF5."""
 
-from pyiron_base.generic.hdfio import ProjectHDFio
+from pyiron_base.storage.hdfio import ProjectHDFio
 
 from abc import ABC, abstractmethod
 
 __author__ = "Marvin Poul"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
@@ -19,14 +19,16 @@
 __date__ = "Sep 1, 2021"
 
 
 class _WithHDF:
     __slots__ = ("_hdf", "_group_name")
 
     def __init__(self, hdf, group_name=None):
+        if group_name in hdf.list_nodes():
+            raise ValueError(f"{group_name} is a node and not a group!")
         self._hdf = hdf
         self._group_name = group_name
 
     def __enter__(self):
         if self._group_name is not None:
             self._hdf = self._hdf.open(self._group_name)
 
@@ -128,16 +130,16 @@
 
     If you're deriving from :class:`GenericJob` it will already take care of
     descending into group_name, so you can pass `""` as the group_name like so
 
     >>> from pyiron_base import GenericJob
     >>> class MyHybridJob(GenericJob, HasHDF):
     ...     def to_hdf(self, hdf, group_name):
-    ...         GenericJob(self, hdf=hdf, group_name=group_name)
-    ...         HasHDF(self, hdf=self.project_hdf5, group_name="")
+    ...         GenericJob.to_hdf(self, hdf=hdf, group_name=group_name)
+    ...         HasHDF.to_hdf(self, hdf=self.project_hdf5, group_name="")
     ...     def from_hdf(self, hdf, group_name):
     ...         MyOldClass.from_hdf(self, hdf=hdf, group_name=group_name)
     ...         HasHDF.to_hdf(self, hdf=self.project_hdf5, group_name="")
 
     .. document private methods
     .. automethod _from_hdf
     .. automethod _to_hdf
@@ -205,15 +207,18 @@
             hdf (:class:`.ProjectHDFio`): HDF group to write to
             group_name (str, optional): name of subgroup
         """
         group_name = (
             group_name if group_name is not None else self._get_hdf_group_name()
         )
         with _WithHDF(hdf, group_name) as hdf:
-            if len(hdf.list_dirs()) > 0 and group_name is None:
+            if (
+                group_name is None
+                and (len(hdf.list_nodes()) > 0 or len(hdf.list_groups())) > 0
+            ):
                 raise ValueError("HDF group must be empty when group_name is not set.")
             self._to_hdf(hdf)
             self._store_type_to_hdf(hdf)
 
     def rewrite_hdf(self, hdf: ProjectHDFio, group_name: str = None):
         """
         Update the HDF representation.
```

### Comparing `pyiron_base-0.5.9/pyiron_base/job/core.py` & `pyiron_base-0.6.0/pyiron_base/jobs/job/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 import math
 import os
 import posixpath
 import shutil
 import warnings
 
 from pyiron_base.interfaces.has_groups import HasGroups
-from pyiron_base.job.util import (
+from pyiron_base.storage.hdfio import ProjectHDFio
+from pyiron_base.jobs.job.util import (
     _get_project_for_copy,
     _copy_database_entry,
     _copy_to_delete_existing,
     _rename_job,
     _get_safe_job_name,
     _job_is_archived,
     _job_archive,
@@ -39,49 +40,46 @@
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 
-class JobCore(HasGroups):
-    """
-    The JobCore the most fundamental pyiron job class. From this class the GenericJob as well as the reduced JobPath
-    class are derived. While JobPath only provides access to the HDF5 file it is about one order faster.
-
-    Implements :class:`.HasGroups`.  Groups are HDF groups in the HDF file associated with the job and any child jobs,
-    nodes are HDF dataset in the HDF file.
-
+# Modular Docstrings
+_doc_str_job_core_args = """\
     Args:
         project (ProjectHDFio): ProjectHDFio instance which points to the HDF5 file the job is stored in
         job_name (str): name of the job, which has to be unique within the project
 
+"""
+
+_doc_str_job_core_attr = """\
     Attributes:
 
         .. attribute:: job_name
 
             name of the job, which has to be unique within the project
 
         .. attribute:: status
 
-            execution status of the job, can be one of the following [initialized, appended, created, submitted, running,
-                                                                      aborted, collect, suspended, refresh, busy, finished]
+            execution status of the job, can be one of the following [initialized, appended, created, submitted, 
+                running, aborted, collect, suspended, refresh, busy, finished]
 
         .. attribute:: job_id
 
             unique id to identify the job in the pyiron database
 
         .. attribute:: parent_id
 
             job id of the predecessor job - the job which was executed before the current one in the current job series
 
         .. attribute:: master_id
 
-            job id of the master job - a meta job which groups a series of jobs, which are executed either in parallel or in
-            serial.
+            job id of the master job - a meta job which groups a series of jobs, which are executed either in parallel 
+                or in serial.
 
         .. attribute:: child_ids
 
             list of child job ids - only meta jobs have child jobs - jobs which list the meta job as their master
 
         .. attribute:: project
 
@@ -98,15 +96,31 @@
         .. attribute:: working_directory
 
             working directory of the job is executed in - outside the HDF5 file
 
         .. attribute:: path
 
             path to the job as a combination of absolute file system path and path within the HDF5 file.
-    """
+"""
+
+
+class JobCore(HasGroups):
+    __doc__ = (
+        """
+    The JobCore the most fundamental pyiron job class. From this class the GenericJob as well as the reduced 
+    JobPath class are derived. While JobPath only provides access to the HDF5 file it is about one order faster.
+    
+    Implements :class:`.HasGroups`.  Groups are HDF groups in the HDF file associated with the job and any 
+    child jobs, nodes are HDF dataset in the HDF file.
+"""
+        + "\n"
+        + _doc_str_job_core_args
+        + "\n"
+        + _doc_str_job_core_attr
+    )
 
     def __init__(self, project, job_name):
         job_name = _get_safe_job_name(job_name)
         self._name = job_name
         self._hdf5 = project.open(self._name)
         self._job_id = None
         self._parent_id = None
@@ -207,78 +221,67 @@
     def parent_id(self):
         """
         Get job id of the predecessor job - the job which was executed before the current one in the current job series
 
         Returns:
             int: parent id
         """
-        if self._parent_id:
-            return self._parent_id
-        elif self.job_id:
+        if self._parent_id is None and self.job_id is not None:
             return self.project.db.get_item_by_id(self.job_id)["parentid"]
-        else:
-            return None
+        return self._parent_id
 
     @parent_id.setter
     def parent_id(self, parent_id):
         """
         Set job id of the predecessor job - the job which was executed before the current one in the current job series
 
         Args:
             parent_id (int): parent id
         """
-        if self.job_id:
+        if self.job_id is not None:
             self.project.db.item_update({"parentid": parent_id}, self.job_id)
         self._parent_id = parent_id
 
     @property
     def master_id(self):
         """
         Get job id of the master job - a meta job which groups a series of jobs, which are executed either in parallel
         or in serial.
 
         Returns:
             int: master id
         """
-        if self._master_id:
-            return self._master_id
-        elif self.job_id:
+        if self._master_id is None and self.job_id is not None:
             return self.project.db.get_item_by_id(self.job_id)["masterid"]
-        else:
-            return None
+        return self._master_id
 
     @master_id.setter
     def master_id(self, master_id):
         """
         Set job id of the master job - a meta job which groups a series of jobs, which are executed either in parallel
         or in serial.
 
         Args:
             master_id (int): master id
         """
-        if self.job_id:
+        if self.job_id is not None:
             self.project.db.item_update({"masterid": master_id}, self.job_id)
         self._master_id = master_id
 
     @property
     def child_ids(self):
         """
         list of child job ids - only meta jobs have child jobs - jobs which list the meta job as their master
 
         Returns:
             list: list of child job ids
         """
-        id_master = self.job_id
-        if id_master is None:
-            return []
-        else:
-            id_l = self.project.db.get_items_dict(
-                {"masterid": str(id_master)}, return_all_columns=False
-            )
-            return sorted([job["id"] for job in id_l])
+        return self.project.get_child_ids(
+            job_specifier=self.job_name, project=self.project.project_path
+        )
 
     @property
     def project_hdf5(self):
         """
         Get the ProjectHDFio instance which points to the HDF5 file the job is stored in
 
         Returns:
@@ -292,14 +295,26 @@
         Set the ProjectHDFio instance which points to the HDF5 file the job is stored in
 
         Args:
             project (ProjectHDFio): HDF5 project
         """
         self._hdf5 = project.copy()
 
+    def relocate_hdf5(self, h5_path=None):
+        """
+        Relocate the hdf file. This function is needed when the child job is
+        spawned by a parent job (cf. pyiron_base.jobs.master.generic)
+        """
+        if h5_path is None:
+            h5_path = "/" + self.job_name
+        self.project_hdf5.remove_group()
+        self.project_hdf5 = self.project_hdf5.__class__(
+            self.project, self.job_name, h5_path=h5_path
+        )
+
     @property
     def project(self):
         """
         Project instance the jobs is located in
 
         Returns:
             Project: project the job is located in
@@ -344,17 +359,17 @@
         Args:
             job_name (str): Job name (optional)
             project (ProjectHDFio, Project): Project path (optional)
 
         Returns:
             (bool): True / False
         """
-        if not job_name:
+        if job_name is None:
             job_name = self.job_name
-        if not project:
+        if project is None:
             project = self._hdf5
 
         where_dict = {
             "job": str(job_name),
             "project": str(project.project_path),
             "subjob": str(project.h5_path),
         }
@@ -458,15 +473,15 @@
                             self.job_name
                         )
                     )
 
         _job_remove_folder(job=self)
 
         # Delete database entry
-        if self.job_id:
+        if self.job_id is not None:
             self.project.db.delete_item(self.job_id)
 
     def to_object(self, object_type=None, **qwargs):
         """
         Load the full pyiron object from an HDF5 file
 
         Args:
@@ -562,31 +577,27 @@
 
         Args:
             job_specifier (str, int): name of the job or job ID
 
         Returns:
             int: job ID of the job
         """
-        if job_specifier:
+        if job_specifier is not None:
             return self.project.get_job_id(
                 job_specifier
             )  # , sub_job_name=self.project_hdf5.h5_path)
-        else:
-            where_dict = {
-                "job": str(self._name),
-                "project": str(self.project_hdf5.project_path),
-                "subjob": str(self.project_hdf5.h5_path),
-            }
-            response = self.project.db.get_items_dict(
-                where_dict, return_all_columns=False
-            )
-            if len(response) > 0:
-                return response[-1]["id"]
-            else:
-                return None
+        where_dict = {
+            "job": str(self._name),
+            "project": str(self.project_hdf5.project_path),
+            "subjob": str(self.project_hdf5.h5_path),
+        }
+        response = self.project.db.get_items_dict(where_dict, return_all_columns=False)
+        if len(response) > 0:
+            return response[-1]["id"]
+        return None
 
     def list_files(self):
         """
         List files inside the working directory
 
         Args:
             extension (str): filter by a specific extension
@@ -693,27 +704,32 @@
         new_job_core._create_working_directory()
         if new_job_name == self.job_name:
             self.project_hdf5.copy_to(destination=hdf5_project.open(".."))
         else:
             self.project_hdf5.copy_to(destination=hdf5_project, maintain_name=False)
 
         # Update the database entry
-        if self.job_id:
-            _copy_database_entry(
-                new_job_core=new_job_core,
-                job_copied_id=self.job_id,
-                new_database_entry=new_database_entry,
-            )
+        if self.job_id is not None:
+            if new_database_entry:
+                _copy_database_entry(
+                    new_job_core=new_job_core,
+                    job_copied_id=self.job_id,
+                )
+            else:
+                new_job_core.reset_job_id(job_id=None)
 
         # Copy files outside the HDF5 file
         if copy_files and os.path.exists(self.working_directory):
-            if len(os.listdir(new_job_core.working_directory)) == 0:
+            wd_content = os.listdir(new_job_core.working_directory)
+            if len(wd_content) == 0:
                 os.rmdir(new_job_core.working_directory)
             else:
-                raise RuntimeError("Target directory for copy not empty!")
+                raise RuntimeError(
+                    f"Target directory for copy not empty! Content = {wd_content}."
+                )
             shutil.copytree(self.working_directory, new_job_core.working_directory)
         return new_job_core, file_project, hdf5_project, False
 
     def copy_to(
         self,
         project,
         new_job_name=None,
@@ -779,15 +795,15 @@
         new_job = self.copy_to(project=project, new_database_entry=False)
         if self.project_hdf5.file_exists:
             if len(self.project_hdf5.h5_path.split("/")) == 2:
                 self.project_hdf5.remove_file()
             else:
                 self.project_hdf5.remove_group()
         self.project_hdf5 = new_job.project_hdf5.copy()
-        if self._job_id:
+        if self._job_id is not None:
             self.project.db.item_update(
                 {
                     "subjob": self.project_hdf5.h5_path,
                     "projectpath": self.project_hdf5.root_path,
                     "project": self.project_hdf5.project_path,
                 },
                 self._job_id,
@@ -814,14 +830,16 @@
         """
         The reset_job_id function has to be implemented by the derived classes - usually the GenericJob class
 
         Args:
             job_id (int/ None):
 
         """
+        if job_id is not None:
+            job_id = int(job_id)
         self._job_id = job_id
 
     def save(self):
         """
         The save function has to be implemented by the derived classes - usually the GenericJob class
         """
         raise NotImplementedError("save() should be implemented in the derived class")
@@ -868,40 +886,84 @@
         If the job is :method:`~.decompress`ed, item can also be a file name to
         access the raw output file of that name of the job.  See available file
         with :method:`~.list_files()`.
 
         `item` is first looked up in this jobs HDF5 file, then in the HDF5 files of any child jobs and finally it is
         matched against any files in the job directory as described above.
 
+        If `item` doesn't match any value (i.e. `None` would be returned), but along its path a `DataContainer` is
+        located, it will be lazily loaded from HDF and then indexed with the remaineder of the path.
+
         Args:
             item (str, slice): path to the data or key of the data object
 
         Returns:
-            dict, list, float, int, None: data or data object; if nothing is found None is returned
+            dict, list, float, int, :class:`.DataContainer`, None: data or data object; if nothing is found None is returned
         """
+
+        if item in self.list_files():
+            file_name = posixpath.join(self.working_directory, "{}".format(item))
+            with open(file_name) as f:
+                return f.readlines()
+
+        # first try to access HDF5 directly to make the common case fast
         try:
-            return self._hdf5[item]
+            group = self._hdf5[item]
+            if (
+                isinstance(group, ProjectHDFio)
+                and "NAME" in group
+                and group["NAME"] == "DataContainer"
+            ):
+                return group.to_object(lazy=True)
+            else:
+                return group
         except ValueError:
             pass
 
         name_lst = item.split("/")
+
+        def successive_path_splits(name_lst):
+            """
+            Yield successive split/joins of a path, i.e.
+            /a/b/c/d
+            gives
+            /a/b/c, d
+            /a/b, c/d
+            /a, b/c/d
+            """
+            for i in range(1, len(name_lst)):
+                # where we are looking for the data container
+                container_path = "/".join(name_lst[:-i])
+                # where we are looking for data in the container
+                data_path = "/".join(name_lst[-1:])
+                yield container_path, data_path
+
+        for container_path, data_path in successive_path_splits(name_lst):
+            try:
+                group = self._hdf5[container_path]
+                if (
+                    isinstance(group, ProjectHDFio)
+                    and "NAME" in group
+                    and group["NAME"] == "DataContainer"
+                ):
+                    return group.to_object(lazy=True)[data_path]
+            except (ValueError, IndexError, KeyError):
+                # either group does not contain a data container or it is does, but it does not have the path we're
+                # looking for
+                pass
+
         item_obj = name_lst[0]
         if item_obj in self._list_ext_childs():
             # ToDo: Murn['strain_0.9'] - sucht im HDF5 file, dort gibt es aber die entsprechenden Gruppen noch nicht.
             child = self._hdf5[self._name + "_hdf5/" + item_obj]
             print("job get: ", self._name + "_jobs")
             if len(name_lst) == 1:
                 return child
             else:
                 return child["/".join(name_lst[1:])]
-
-        if name_lst[0] in self.list_files():
-            file_name = posixpath.join(self.working_directory, "{}".format(item_obj))
-            with open(file_name) as f:
-                return f.readlines()
         return None
 
     def __setitem__(self, key, value):
         """
         Stores data
 
         Args:
@@ -1002,25 +1064,25 @@
 
     def __init__(self, job_dict=None):
         self._job_dict = job_dict
 
     def __bool__(self):
         return self._job_dict is not None
 
-    def __nonzero__(self):  # __bool__() for Python 2.7
-        return self._job_dict is not None
-
     def __dir__(self):
         return list(self._job_dict.keys())
 
     def __getattr__(self, name):
         if name in self._job_dict.keys():
             return self._job_dict[name]
         else:
-            raise AttributeError
+            raise AttributeError(name)
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}({repr(self._job_dict)})"
 
 
 class HDF5Content(object):
     """
     Access the HDF5 file of the job
     """
```

### Comparing `pyiron_base-0.5.9/pyiron_base/job/executable.py` & `pyiron_base-0.6.0/pyiron_base/jobs/job/extension/executable.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import os
+from pyiron_base.interfaces.object import HasStorage
+from pyiron_base.state import state
 
 """
 Executable class loading executables from static/bin/<code>/
 """
 
 __author__ = "Jan Janssen"
 __copyright__ = (
@@ -16,120 +18,125 @@
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 
-class Executable(object):
+class Executable(HasStorage):
     def __init__(
         self,
-        path_binary_codes,
+        path_binary_codes=None,
         codename=None,
         module=None,
         code=None,
         overwrite_nt_flag=False,
     ):
         """
         Handle the path to the executable, as well as the version selection.
 
         Args:
             codename (str): name of the code str
             path_binary_codes (list): path to the binary codes as an absolute path
             overwrite_nt_flag (bool):
         """
-        self.__version__ = None
+        super().__init__()
+        self.storage.table_name = "executable"
+
+        if path_binary_codes is None:
+            path_binary_codes = state.settings.resource_paths
+        self.storage.version = None
         if code is not None:  # Backwards compatibility
             if not isinstance(code.__name__, str):
                 raise TypeError("The codename should be a string.")
             codename = code.__name__
             module = code.__module__.split(".")[1]
         if codename is not None and module is not None:
-            self.__name__ = codename.lower()
+            self.storage.name = codename.lower()
             code_path_lst = [
                 os.path.join(path, module, "bin") for path in path_binary_codes
             ]
             backwards_compatible_path_lst = [
-                os.path.join(path, self.__name__) for path in path_binary_codes
+                os.path.join(path, self.storage.name) for path in path_binary_codes
             ]
-            self._path_bin = [
+            self.path_bin = [
                 exe_path
                 for exe_path in (code_path_lst + backwards_compatible_path_lst)
                 if os.path.exists(exe_path)
             ]
         else:  # Backwards compatibility
-            self.__name__ = codename.lower()
-            self._path_bin = [
-                os.path.join(path, self.__name__)
+            self.storage.name = codename.lower()
+            self.path_bin = [
+                os.path.join(path, self.storage.name)
                 for path in path_binary_codes
-                if os.path.exists(os.path.join(path, self.__name__))
+                if os.path.exists(os.path.join(path, self.storage.name))
             ]
         if overwrite_nt_flag:
-            self._operation_system_nt = False
+            self.storage.operation_system_nt = False
         else:
-            self._operation_system_nt = os.name == "nt"
-        self._executable_lst = self._executable_versions_list()
-        self._executable = None
+            self.storage.operation_system_nt = os.name == "nt"
+        self.executable_lst = self._executable_versions_list()
+        self.storage.executable = None
         self._executable_path = None
-        self._mpi = False
-        if self._executable_lst:
+        self.storage.mpi = False
+        if self.executable_lst:
             self.version = self.default_version
-        self._accepted_return_codes = [0]
+        self.storage.accepted_return_codes = [0]
 
     @property
     def accepted_return_codes(self):
         """
         list of int: accept all of the return codes in this list as the result of a successful run
         """
-        return self._accepted_return_codes
+        return self.storage.accepted_return_codes
 
     @accepted_return_codes.setter
     def accepted_return_codes(self, value):
         if not isinstance(value, list) or any(
             not isinstance(c, int) or c > 255 for c in value
         ):
             raise ValueError("accepted_return_codes must be a list of integers <= 255!")
-        self._accepted_return_codes = value
+        self.storage.accepted_return_codes = value
 
     @property
     def version(self):
         """
         Version of the Executable
 
         Returns:
             str: version
         """
-        return self.__version__
+        return self.storage.version
 
     @property
     def default_version(self):
         """
         Default Version of the Available Executables
         i.e. specifically defined
 
         Returns:
             str: default_version
         """
-        for executable in self._executable_lst.keys():
+        for executable in self.executable_lst.keys():
             if "default" in executable and "mpi" not in executable:
                 return executable
-        return sorted(self._executable_lst.keys())[0]
+        return sorted(self.executable_lst.keys())[0]
 
     @version.setter
     def version(self, new_version):
         """
         Version of the Executable
 
         Args:
             new_version (str): version
         """
-        if new_version in self._executable_lst.keys():
-            self.__version__ = new_version
+        if new_version in self.executable_lst.keys():
+            self.storage.version = new_version
             if "mpi" in new_version:
-                self._mpi = True
+                self.storage.mpi = True
             self._executable_path = None
         else:
             raise ValueError(
                 "Version  [%s] is not supported, please choose one of the following versions: "
                 % new_version,
                 str(self.available_versions),
             )
@@ -138,17 +145,17 @@
     def mpi(self):
         """
         Check if the message processing interface is activated.
 
         Returns:
             bool: [True/False]
         """
-        if not self._mpi and self.version and "_mpi" in self.version:
-            self._mpi = True
-        return self._mpi
+        if not self.storage.mpi and self.version and "_mpi" in self.version:
+            self.storage.mpi = True
+        return self.storage.mpi
 
     @mpi.setter
     def mpi(self, mpi_bool):
         """
         Activate the message processing interface.
 
         Args:
@@ -174,15 +181,15 @@
     def list_executables(self):
         """
         List all available exectuables in the path_binary_codes for the specified codename.
 
         Returns:
             list: list of the available version
         """
-        return sorted(list(self._executable_lst.keys()))
+        return sorted(list(self.executable_lst.keys()))
 
     @property
     def executable_path(self):
         """
         Get the executable path
 
         Returns:
@@ -199,20 +206,49 @@
     def executable_path(self, new_path):
         """
         Set the executable path
 
         Args:
             new_path: absolute path
         """
-        self.__version__ = new_path
+        self.storage.version = new_path
         self._executable_path = new_path
         if new_path and "mpi" in new_path:
-            self._mpi = True
+            self.storage.mpi = True
+        else:
+            self.storage.mpi = False
+
+    def get_input_for_subprocess_call(self, cores, threads):
+        """
+        Get the input parameters for the subprocess call to execute the job
+
+        Args:
+            cores (int): number of cores
+            threads (int): number of threads
+
+        Returns:
+            str/ list, boolean:  executable and shell variables
+        """
+        if cores == 1 or not self.mpi:
+            executable = self.__str__()
+            shell = True
+        elif isinstance(self.executable_path, list):
+            executable = self.executable_path[:] + [
+                str(cores),
+                str(threads),
+            ]
+            shell = False
         else:
-            self._mpi = False
+            executable = [
+                self.executable_path,
+                str(cores),
+                str(threads),
+            ]
+            shell = False
+        return executable, shell
 
     def __repr__(self):
         """
         Executable path
         """
         return repr(self.executable_path)
 
@@ -225,43 +261,48 @@
     def _executable_versions_list(self):
         """
         Internal function to list all available exectuables in the path_binary_codes for the specified codename.
 
         Returns:
             dict: list of the available version
         """
-        if self._operation_system_nt:
+        if self.storage.operation_system_nt:
             extension = ".bat"
         else:
             extension = ".sh"
         try:
             executable_dict = {}
-            for path in self._path_bin:
+            for path in self.path_bin:
                 for executable in os.listdir(path):
                     if (
-                        executable.startswith("run_" + self.__name__ + "_")
+                        executable.startswith("run_" + self.storage.name + "_")
                         & executable.endswith(extension)
                         and executable[
-                            len("run_" + self.__name__) + 1 : -len(extension)
+                            len("run_" + self.storage.name) + 1 : -len(extension)
                         ]
                         not in executable_dict.keys()
                     ):
                         executable_dict[
                             executable[
-                                len("run_" + self.__name__) + 1 : -len(extension)
+                                len("run_" + self.storage.name) + 1 : -len(extension)
                             ]
                         ] = os.path.join(path, executable).replace("\\", "/")
             return executable_dict
-        except OSError:  # No executable exists - This is the case for GenericJob and other abstract job classes.
+        except (
+            OSError
+        ):  # No executable exists - This is the case for GenericJob and other abstract job classes.
             return dict()
 
     def _executable_select(self):
         """
         Internal function to select an executable based on the codename and the version.
 
         Returns:
             str: absolute executable path
         """
         try:
-            return self._executable_lst[self.version]
+            return self.executable_lst[self.version]
         except KeyError:
             return ""
+
+    def _get_hdf_group_name(self):
+        return "executable"
```

### Comparing `pyiron_base-0.5.9/pyiron_base/job/external.py` & `pyiron_base-0.6.0/pyiron_base/project/external.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 """
 Load input parameters for jupyter notebooks from external HDF5 or JSON file
 """
 
 import json
 from pathlib2 import Path
 import warnings
-from pyiron_base.generic.hdfio import FileHDFio
-from pyiron_base.generic.datacontainer import DataContainer
+from pyiron_base.storage.hdfio import FileHDFio
+from pyiron_base.storage.datacontainer import DataContainer
 
 __author__ = "Osamu Waseda"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
```

### Comparing `pyiron_base-0.5.9/pyiron_base/job/factory.py` & `pyiron_base-0.6.0/pyiron_base/jobs/job/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 Factories for creating jobs, which may already exist in the database/storage.
 """
 
 from pyiron_base.project.generic import Project
-from pyiron_base.generic.factory import PyironFactory
+from pyiron_base.interfaces.factory import PyironFactory
 from abc import ABC, abstractmethod
-from pyiron_base.job.jobtype import JobType
-from pyiron_base.job.generic import GenericJob
+from pyiron_base.jobs.job.jobtype import JobType
+from pyiron_base.jobs.job.generic import GenericJob
 from typing import Type, Dict, List, Union
 
-from pyiron_base.master.flexible import FlexibleMaster
-from pyiron_base.job.script import ScriptJob
-from pyiron_base.master.serial import SerialMasterBase
-from pyiron_base.table.datamining import TableJob
-from pyiron_base.generic.hdfio import ProjectHDFio
+from pyiron_base.jobs.master.flexible import FlexibleMaster
+from pyiron_base.jobs.script import ScriptJob
+from pyiron_base.jobs.master.serial import SerialMasterBase
+from pyiron_base.jobs.datamining import TableJob
+from pyiron_base.storage.hdfio import ProjectHDFio
 from pyiron_base.state import state
 
 __author__ = "Liam Huber, Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -62,17 +62,15 @@
                     delete_existing_job (bool): delete an existing job - default false
                     delete_aborted_job (bool): delete an existing and aborted job - default false
 
                 Returns:
                     GenericJob: job object depending on the job_type selected
                 """
                 return JobType(
-                    class_name=self._job_class_dict[
-                        name
-                    ],  # Pass the class directly, JobType can handle that
+                    class_name=name,  # Pass the class directly, JobType can handle that
                     project=ProjectHDFio(
                         project=self._project.copy(), file_name=job_name
                     ),
                     job_name=job_name,
                     job_class_dict=self._job_class_dict,
                     delete_existing_job=delete_existing_job,
                     delete_aborted_job=delete_aborted_job,
```

### Comparing `pyiron_base-0.5.9/pyiron_base/job/generic.py` & `pyiron_base-0.6.0/pyiron_base/jobs/job/generic.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,118 +1,72 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 Generic Job class extends the JobCore class with all the functionality to run the job object.
 """
 
-import signal
 from datetime import datetime
 import os
-
 import posixpath
-import multiprocessing
-import h5io
-from pyiron_base.job.wrapper import JobWrapper
+import signal
+import warnings
+
 from pyiron_base.state import state
-from pyiron_base.job.executable import Executable
-from pyiron_base.job.jobstatus import JobStatus
-from pyiron_base.job.core import JobCore
-from pyiron_base.job.util import (
+from pyiron_base.state.signal import catch_signals
+from pyiron_base.jobs.job.extension.executable import Executable
+from pyiron_base.jobs.job.extension.jobstatus import JobStatus
+from pyiron_base.jobs.job.core import (
+    JobCore,
+    _doc_str_job_core_args,
+    _doc_str_job_core_attr,
+)
+from pyiron_base.jobs.job.runfunction import (
+    run_job_with_parameter_repair,
+    run_job_with_status_initialized,
+    run_job_with_status_created,
+    run_job_with_status_submitted,
+    run_job_with_status_running,
+    run_job_with_status_refresh,
+    run_job_with_status_busy,
+    run_job_with_status_collect,
+    run_job_with_status_suspended,
+    run_job_with_status_finished,
+    run_job_with_runmode_modal,
+    run_job_with_runmode_queue,
+    execute_job_with_external_executable,
+)
+from pyiron_base.jobs.job.util import (
     _copy_restart_files,
     _kill_child,
     _job_store_before_copy,
     _job_reload_after_copy,
 )
-from pyiron_base.generic.util import static_isinstance, deprecate
-from pyiron_base.server.generic import Server
+from pyiron_base.utils.instance import static_isinstance
+from pyiron_base.utils.deprecate import deprecate
+from pyiron_base.jobs.job.extension.server.generic import Server
 from pyiron_base.database.filetable import FileTable
-import subprocess
-import warnings
+from pyiron_base.storage.helper_functions import write_hdf5, read_hdf5
 
 __author__ = "Joerg Neugebauer, Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
-intercepted_signals = [
-    signal.SIGINT,
-    signal.SIGTERM,
-    signal.SIGABRT,
-]  # , signal.SIGQUIT]
-
-
-class GenericJob(JobCore):
-    """
-    Generic Job class extends the JobCore class with all the functionality to run the job object. From this class
-    all specific Hamiltonians are derived. Therefore it should contain the properties/routines common to all jobs.
-    The functions in this module should be as generic as possible.
-
-    Sub classes that need to add special behavior after :method:`.copy_to()` can override
-    :method:`._after_generic_copy_to()`.
-
-    Args:
-        project (ProjectHDFio): ProjectHDFio instance which points to the HDF5 file the job is stored in
-        job_name (str): name of the job, which has to be unique within the project
-
-    Attributes:
-
-        .. attribute:: job_name
-
-            name of the job, which has to be unique within the project
-
-        .. attribute:: status
-
-            execution status of the job, can be one of the following [initialized, appended, created, submitted,
-                                                                      running, aborted, collect, suspended, refresh,
-                                                                      busy, finished]
-
-        .. attribute:: job_id
-
-            unique id to identify the job in the pyiron database
-
-        .. attribute:: parent_id
-
-            job id of the predecessor job - the job which was executed before the current one in the current job series
-
-        .. attribute:: master_id
-
-            job id of the master job - a meta job which groups a series of jobs, which are executed either in parallel
-            or in serial.
-
-        .. attribute:: child_ids
-
-            list of child job ids - only meta jobs have child jobs - jobs which list the meta job as their master
-
-        .. attribute:: project
-
-            Project instance the jobs is located in
-
-        .. attribute:: project_hdf5
-
-            ProjectHDFio instance which points to the HDF5 file the job is stored in
-
-        .. attribute:: job_info_str
-
-            short string to describe the job by it is job_name and job ID - mainly used for logging
-
-        .. attribute:: working_directory
-
-            working directory of the job is executed in - outside the HDF5 file
-
-        .. attribute:: path
-
-            path to the job as a combination of absolute file system path and path within the HDF5 file.
-
+# Modular Docstrings
+_doc_str_generic_job_attr = (
+    _doc_str_job_core_attr
+    + "\n"
+    + """\
         .. attribute:: version
 
             Version of the hamiltonian, which is also the version of the executable unless a custom executable is used.
 
         .. attribute:: executable
 
             Executable used to run the job - usually the path to an external executable.
@@ -146,47 +100,68 @@
 
             list of groups which are excluded from storing in the hdf5 file.
 
         .. attribute:: job_type
 
             Job type object with all the available job types: ['ExampleJob', 'SerialMaster', 'ParallelMaster',
                                                                'ScriptJob', 'ListMaster']
-    """
+"""
+)
+
+
+class GenericJob(JobCore):
+    __doc__ = (
+        """
+    Generic Job class extends the JobCore class with all the functionality to run the job object. From this class
+    all specific job types are derived. Therefore it should contain the properties/routines common to all jobs.
+    The functions in this module should be as generic as possible.
+
+    Sub classes that need to add special behavior after :method:`.copy_to()` can override
+    :method:`._after_generic_copy_to()`.
+"""
+        + "\n"
+        + _doc_str_job_core_args
+        + "\n"
+        + _doc_str_generic_job_attr
+    )
 
     def __init__(self, project, job_name):
         super(GenericJob, self).__init__(project, job_name)
         self.__name__ = type(self).__name__
         self.__version__ = "0.4"
         self.__hdf_version__ = "0.1.0"
         self._server = Server()
         self._logger = state.logger
         self._executable = None
         if not state.database.database_is_disabled:
             self._status = JobStatus(db=project.db, job_id=self.job_id)
             self.refresh_job_status()
         elif os.path.exists(self.project_hdf5.file_name):
-            initial_status = h5io.read_hdf5(
-                self.project_hdf5.file_name, job_name + "/status"
+            initial_status = read_hdf5(
+                self.project_hdf5.file_name, self.job_name + "/status"
             )
             self._status = JobStatus(initial_status=initial_status)
+            if "job_id" in self.list_nodes():
+                self._job_id = read_hdf5(
+                    self.project_hdf5.file_name, self.job_name + "/job_id"
+                )
         else:
             self._status = JobStatus()
         self._restart_file_list = list()
         self._restart_file_dict = dict()
         self._exclude_nodes_hdf = list()
         self._exclude_groups_hdf = list()
         self._process = None
         self._compress_by_default = False
         self._python_only_job = False
+        self._write_work_dir_warnings = True
+        self._flux_executor = None
         self.interactive_cache = None
         self.error = GenericError(job=self)
 
-        for sig in intercepted_signals:
-            signal.signal(sig, self.signal_intercept)
-
     @property
     def version(self):
         """
         Get the version of the hamiltonian, which is also the version of the executable unless a custom executable is
         used.
 
         Returns:
@@ -232,14 +207,23 @@
         Args:
             exe (str): executable path, if no valid path is provided an executable is chosen based on version.
         """
         self._executable_activate()
         self._executable.executable_path = exe
 
     @property
+    def flux_executor(self):
+        return self._flux_executor
+
+    @flux_executor.setter
+    def flux_executor(self, exe):
+        self.server.run_mode.flux = True
+        self._flux_executor = exe
+
+    @property
     def server(self):
         """
         Get the server object to handle the execution environment for the job.
 
         Returns:
             Server: server object
         """
@@ -396,17 +380,31 @@
         pass
 
     def write_input(self):
         """
         Write the input files for the external executable. This method has to be implemented in the individual
         hamiltonians.
         """
-        raise NotImplementedError(
-            "write procedure must be defined for derived Hamilton!"
-        )
+        if (
+            state.settings.configuration["write_work_dir_warnings"]
+            and self._write_work_dir_warnings
+            and not self._python_only_job
+        ):
+            with open(
+                os.path.join(self.working_directory, "WARNING_pyiron_modified_content"),
+                "w",
+            ) as f:
+                f.write(
+                    "Files in this directory are intended to be written and read by pyiron. \n\n"
+                    "pyiron may transform user input to enhance performance, thus, use these files with care!\n"
+                    "Consult the log and/or the documentation to gain further information.\n\n"
+                    "To disable writing these warning files, specify \n"
+                    "WRITE_WORK_DIR_WARNINGS=False in the .pyiron configuration file (or set the "
+                    "PYIRONWRITEWORKDIRWARNINGS environment variable accordingly)."
+                )
 
     def collect_output(self):
         """
         Collect the output files of the external executable and store the information in the HDF5 file. This method has
         to be implemented in the individual hamiltonians.
         """
         raise NotImplementedError(
@@ -434,15 +432,15 @@
             self._status = JobStatus(
                 initial_status=self.project.db.get_job_status(self.job_id),
                 db=self.project.db,
                 job_id=self.job_id,
             )
         elif state.database.database_is_disabled:
             self._status = JobStatus(
-                initial_status=h5io.read_hdf5(
+                initial_status=read_hdf5(
                     self.project_hdf5.file_name, self.job_name + "/status"
                 )
             )
 
     def clear_job(self):
         """
         Convenience function to clear job info after suspend. Mimics deletion of all the job info after suspend in a
@@ -502,15 +500,15 @@
             delete_existing_job=delete_existing_job,
         )
         if reloaded:
             return new_job_core, file_project, hdf5_project, reloaded
 
         # Reload object from HDF5 file
         if not static_isinstance(
-            obj=project.__class__, obj_type="pyiron_base.job.core.JobCore"
+            obj=project.__class__, obj_type="pyiron_base.jobs.job.core.JobCore"
         ):
             _job_reload_after_copy(
                 job=new_job_core, delete_file_after_copy=delete_file_after_copy
             )
         if delete_file_after_copy:
             self.project_hdf5.remove_file()
         return new_job_core, file_project, hdf5_project, reloaded
@@ -617,21 +615,27 @@
         """
         internal function to remove command that removes also child jobs.
         Do never use this command, since it will destroy the integrity of your project.
         """
         _kill_child(job=self)
         super(GenericJob, self).remove_child()
 
-    def kill(self):
-        if self.status.running or self.status.submitted:
+    def remove_and_reset_id(self, _protect_childs=True):
+        if self.job_id is not None:
             master_id, parent_id = self.master_id, self.parent_id
-            self.remove()
+            self.remove(_protect_childs=_protect_childs)
             self.reset_job_id()
             self.master_id, self.parent_id = master_id, parent_id
         else:
+            self.remove(_protect_childs=_protect_childs)
+
+    def kill(self):
+        if self.status.running or self.status.submitted:
+            self.remove_and_reset_id()
+        else:
             raise ValueError(
                 "The kill() function is only available during the execution of the job."
             )
 
     def validate_ready_to_run(self):
         """
         Validate that the calculation is ready to be executed. By default no generic checks are performed, but one could
@@ -650,17 +654,15 @@
         """
         pass
 
     def reset_job_id(self, job_id=None):
         """
         Reset the job id sets the job_id to None in the GenericJob as well as all connected modules like JobStatus.
         """
-        if job_id is not None:
-            job_id = int(job_id)
-        self._job_id = job_id
+        super().reset_job_id(job_id=job_id)
         self._status = JobStatus(db=self.project.db, job_id=self._job_id)
 
     @deprecate(
         run_again="Either delete the job via job.remove() or use delete_existing_job=True.",
         version="0.4.0",
     )
     def run(
@@ -678,156 +680,89 @@
         Args:
             delete_existing_job (bool): Delete the existing job and run the simulation again.
             repair (bool): Set the job status to created and run the simulation again.
             debug (bool): Debug Mode - defines the log level of the subprocess the job is executed in.
             run_mode (str): ['modal', 'non_modal', 'queue', 'manual'] overwrites self.server.run_mode
             run_again (bool): Same as delete_existing_job (deprecated)
         """
-        if run_again:
-            delete_existing_job = True
-        try:
-            self._logger.info(
-                "run {}, status: {}".format(self.job_info_str, self.status)
-            )
-            status = self.status.string
-            if run_mode is not None:
-                self.server.run_mode = run_mode
-            if delete_existing_job and self.job_id:
-                self._logger.info("run repair " + str(self.job_id))
-                status = "initialized"
-                master_id, parent_id = self.master_id, self.parent_id
-                self.remove(_protect_childs=False)
-                self.reset_job_id()
-                self.master_id, self.parent_id = master_id, parent_id
-            if repair and self.job_id and not self.status.finished:
-                self._run_if_repair()
-            elif status == "initialized":
-                self._run_if_new(debug=debug)
-            elif status == "created":
-                self._run_if_created()
-            elif status == "submitted":
-                self._run_if_submitted()
-            elif status == "running":
-                self._run_if_running()
-            elif status == "collect":
-                self._run_if_collect()
-            elif status == "suspend":
-                self._run_if_suspended()
-            elif status == "refresh":
-                self.run_if_refresh()
-            elif status == "busy":
-                self._run_if_busy()
-            elif status == "finished":
-                self._run_if_finished(delete_existing_job=delete_existing_job)
-        except Exception:
-            self.drop_status_to_aborted()
-            raise
-        except KeyboardInterrupt:
-            self.drop_status_to_aborted()
-            raise
-        except SystemExit:
-            self.drop_status_to_aborted()
-            raise
+        with catch_signals(self.signal_intercept):
+            if run_again:
+                delete_existing_job = True
+            try:
+                self._logger.info(
+                    "run {}, status: {}".format(self.job_info_str, self.status)
+                )
+                status = self.status.string
+                if run_mode is not None:
+                    self.server.run_mode = run_mode
+                if delete_existing_job:
+                    status = "initialized"
+                    self.remove_and_reset_id(_protect_childs=False)
+                if repair and self.job_id and not self.status.finished:
+                    self._run_if_repair()
+                elif status == "initialized":
+                    return self._run_if_new(debug=debug)
+                elif status == "created":
+                    return self._run_if_created()
+                elif status == "submitted":
+                    run_job_with_status_submitted(job=self)
+                elif status == "running":
+                    self._run_if_running()
+                elif status == "collect":
+                    self._run_if_collect()
+                elif status == "suspend":
+                    self._run_if_suspended()
+                elif status == "refresh":
+                    self.run_if_refresh()
+                elif status == "busy":
+                    self._run_if_busy()
+                elif status == "finished":
+                    run_job_with_status_finished(job=self)
+                elif status == "aborted":
+                    raise ValueError(
+                        "Running an aborted job with `delete_existing_job=False` is meaningless."
+                    )
+            except Exception:
+                self.drop_status_to_aborted()
+                raise
 
     def run_if_modal(self):
         """
         The run if modal function is called by run to execute the simulation, while waiting for the output. For this we
         use subprocess.check_output()
         """
-        self.run_static()
+        run_job_with_runmode_modal(job=self)
 
     def run_static(self):
         """
         The run static function is called by run to execute the simulation.
         """
-        self._logger.info(
-            "{}, status: {}, run job (modal)".format(self.job_info_str, self.status)
-        )
-        if self.executable.executable_path == "":
-            self.status.aborted = True
-            raise ValueError("No executable set!")
-        self.status.running = True
-        if self.job_id is not None:
-            self.project.db.item_update({"timestart": datetime.now()}, self.job_id)
-        job_crashed, out = False, None
-        if self.server.cores == 1 or not self.executable.mpi:
-            executable = str(self.executable)
-            shell = True
-        elif isinstance(self.executable.executable_path, list):
-            executable = self.executable.executable_path[:] + [
-                str(self.server.cores),
-                str(self.server.threads),
-            ]
-            shell = False
-        else:
-            executable = [
-                self.executable.executable_path,
-                str(self.server.cores),
-                str(self.server.threads),
-            ]
-            shell = False
-        try:
-            out = subprocess.run(
-                executable,
-                cwd=self.project_hdf5.working_directory,
-                shell=shell,
-                stdout=subprocess.PIPE,
-                stderr=subprocess.STDOUT,
-                universal_newlines=True,
-                check=True,
-            ).stdout
-        except subprocess.CalledProcessError as e:
-            out = e.output
-            if e.returncode in self.executable.accepted_return_codes:
-                pass
-            elif not self.server.accept_crash:
-                self._logger.warning("Job aborted")
-                self._logger.warning(e.output)
-                self.status.aborted = True
-                if self.job_id is not None:
-                    self.project.db.item_update(self._runtime(), self.job_id)
-                error_file = posixpath.join(
-                    self.project_hdf5.working_directory, "error.msg"
-                )
-                with open(error_file, "w") as f:
-                    f.write(e.output)
-                if self.server.run_mode.non_modal:
-                    state.database.close_connection()
-                raise RuntimeError("Job aborted")
-            else:
-                job_crashed = True
-
-        with open(
-            posixpath.join(self.project_hdf5.working_directory, "error.out"), mode="w"
-        ) as f_err:
-            f_err.write(out)
+        execute_job_with_external_executable(job=self)
 
-        self.set_input_to_read_only()
-        self.status.collect = True
-        self._logger.info(
-            "{}, status: {}, output: {}".format(self.job_info_str, self.status, out)
-        )
-        self.run()
-        if job_crashed:
-            self.status.aborted = True
+    def run_if_scheduler(self):
+        """
+        The run if queue function is called by run if the user decides to submit the job to and queing system. The job
+        is submitted to the queuing system using subprocess.Popen()
+        Returns:
+            int: Returns the queue ID for the job.
+        """
+        return run_job_with_runmode_queue(job=self)
 
     def transfer_from_remote(self):
         state.queue_adapter.get_job_from_remote(
             working_directory="/".join(self.working_directory.split("/")[:-1]),
-            delete_remote=state.queue_adapter.ssh_delete_file_on_remote,
         )
         state.queue_adapter.transfer_file_to_remote(
             file=self.project_hdf5.file_name,
             transfer_back=True,
-            delete_remote=state.queue_adapter.ssh_delete_file_on_remote,
         )
         if state.database.database_is_disabled:
             self.project.db.update()
         else:
-            ft = FileTable(project=self.project_hdf5.path + "_hdf5/")
+            ft = FileTable(index_from=self.project_hdf5.path + "_hdf5/")
             df = ft.job_table(
                 sql_query=None,
                 user=state.settings.login_user,
                 project_path=None,
                 all_columns=True,
             )
             db_dict_lst = []
@@ -872,14 +807,23 @@
         For jobs which executables are available as Python library, those can also be executed with a library call
         instead of calling an external executable. This is usually faster than a single core python job.
         """
         raise NotImplementedError(
             "This function needs to be implemented in the specific class."
         )
 
+    def run_if_interactive_non_modal(self):
+        """
+        For jobs which executables are available as Python library, those can also be executed with a library call
+        instead of calling an external executable. This is usually faster than a single core python job.
+        """
+        raise NotImplementedError(
+            "This function needs to be implemented in the specific class."
+        )
+
     def interactive_close(self):
         """
         For jobs which executables are available as Python library, those can also be executed with a library call
         instead of calling an external executable. This is usually faster than a single core python job. After the
         interactive execution, the job can be closed using the interactive_close function.
         """
         raise NotImplementedError(
@@ -902,159 +846,14 @@
         instead of calling an external executable. This is usually faster than a single core python job. To write the
         interactive cache to the HDF5 file the interactive flush function is used.
         """
         raise NotImplementedError(
             "This function needs to be implemented in the specific class."
         )
 
-    def run_if_interactive_non_modal(self):
-        """
-        For jobs which executables are available as Python library, those can also be executed with a library call
-        instead of calling an external executable. This is usually faster than a single core python job.
-        """
-        raise NotImplementedError(
-            "This function needs to be implemented in the specific class."
-        )
-
-    def run_if_non_modal(self):
-        """
-        The run if non modal function is called by run to execute the simulation in the background. For this we use
-        multiprocessing.Process()
-        """
-        if not state.database.database_is_disabled:
-            if not state.database.using_local_database:
-                args = (self.job_id, self.project_hdf5.working_directory, False, None)
-            else:
-                args = (
-                    self.job_id,
-                    self.project_hdf5.working_directory,
-                    False,
-                    str(self.project.db.conn.engine.url),
-                )
-
-            p = multiprocessing.Process(
-                target=multiprocess_wrapper,
-                args=args,
-            )
-
-            if self.master_id and self.server.run_mode.non_modal:
-                del self
-                p.start()
-            else:
-                if self.server.run_mode.non_modal:
-                    p.start()
-                else:
-                    self._process = p
-                    self._process.start()
-        else:
-            command = (
-                "python -m pyiron_base.cli wrapper -p "
-                + self.working_directory
-                + " -f "
-                + self.project_hdf5.file_name
-                + self.project_hdf5.h5_path
-            )
-            working_directory = self.project_hdf5.working_directory
-            if not os.path.exists(working_directory):
-                os.makedirs(working_directory)
-            del self
-            subprocess.Popen(
-                command,
-                cwd=working_directory,
-                shell=True,
-                stdout=subprocess.PIPE,
-                stderr=subprocess.STDOUT,
-                universal_newlines=True,
-            )
-
-    def run_if_manually(self, _manually_print=True):
-        """
-        The run if manually function is called by run if the user decides to execute the simulation manually - this
-        might be helpful to debug a new job type or test updated executables.
-
-        Args:
-            _manually_print (bool): Print explanation how to run the simulation manually - default=True.
-        """
-        if _manually_print:
-            abs_working = posixpath.abspath(self.project_hdf5.working_directory)
-            print(
-                "You have selected to start the job manually. "
-                + "To run it, go into the working directory {} and ".format(abs_working)
-                + "call 'python -m pyiron_base.cli wrapper -p {}".format(abs_working)
-                + " -j {} ' ".format(self.job_id)
-            )
-
-    def run_if_scheduler(self):
-        """
-        The run if queue function is called by run if the user decides to submit the job to and queing system. The job
-        is submitted to the queuing system using subprocess.Popen()
-
-        Returns:
-            int: Returns the queue ID for the job.
-        """
-        if state.queue_adapter is None:
-            raise TypeError("No queue adapter defined.")
-        if state.queue_adapter.remote_flag:
-            filename = state.queue_adapter.convert_path_to_remote(
-                path=self.project_hdf5.file_name
-            )
-            working_directory = state.queue_adapter.convert_path_to_remote(
-                path=self.working_directory
-            )
-            command = (
-                "python -m pyiron_base.cli wrapper -p "
-                + working_directory
-                + " -f "
-                + filename
-                + self.project_hdf5.h5_path
-                + " --submit"
-            )
-            state.queue_adapter.transfer_file_to_remote(
-                file=self.project_hdf5.file_name, transfer_back=False
-            )
-        elif state.database.database_is_disabled:
-            command = (
-                "python -m pyiron_base.cli wrapper -p "
-                + self.working_directory
-                + " -f "
-                + self.project_hdf5.file_name
-                + self.project_hdf5.h5_path
-            )
-        else:
-            command = (
-                "python -m pyiron_base.cli wrapper -p "
-                + self.working_directory
-                + " -j "
-                + str(self.job_id)
-            )
-        que_id = state.queue_adapter.submit_job(
-            queue=self.server.queue,
-            job_name="pi_" + str(self.job_id),
-            working_directory=self.project_hdf5.working_directory,
-            cores=self.server.cores,
-            run_time_max=self.server.run_time,
-            memory_max=self.server.memory_limit,
-            command=command,
-        )
-        if que_id is not None:
-            self.server.queue_id = que_id
-            self._server.to_hdf(self._hdf5)
-            print("Queue system id: ", que_id)
-        else:
-            self._logger.warning("Job aborted")
-            self.status.aborted = True
-            raise ValueError("run_queue.sh crashed")
-        state.logger.debug("submitted %s", self.job_name)
-        self._logger.debug("job status: %s", self.status)
-        self._logger.info(
-            "{}, status: {}, submitted: queue id {}".format(
-                self.job_info_str, self.status, que_id
-            )
-        )
-
     def send_to_database(self):
         """
         if the jobs should be store in the external/public database this could be implemented here, but currently it is
         just a placeholder.
         """
         if self.server.send_to_db:
             pass
@@ -1167,36 +966,41 @@
         Args:
             file_name (str): name of the file
             cwd (str): current working directory - this overwrites self.project_hdf5.working_directory - optional
 
         Returns:
             str: absolute path to the file in the current working directory
         """
-        if not cwd:
+        if cwd is None:
             cwd = self.project_hdf5.working_directory
         return posixpath.join(cwd, file_name)
 
+    def _set_hdf(self, hdf=None, group_name=None):
+        if hdf is not None:
+            self._hdf5 = hdf
+        if group_name is not None and self._hdf5 is not None:
+            self._hdf5 = self._hdf5.open(group_name)
+
     def to_hdf(self, hdf=None, group_name=None):
         """
         Store the GenericJob in an HDF5 file
 
         Args:
             hdf (ProjectHDFio): HDF5 group object - optional
             group_name (str): HDF5 subgroup name - optional
         """
-        if hdf is not None:
-            self._hdf5 = hdf
-        if group_name is not None:
-            self._hdf5 = self._hdf5.open(group_name)
+        self._set_hdf(hdf=hdf, group_name=group_name)
         self._executable_activate_mpi()
         self._type_to_hdf()
         self._hdf5["status"] = self.status.string
         if self._import_directory is not None:
             self._hdf5["import_directory"] = self._import_directory
         self._server.to_hdf(self._hdf5)
+        if self._executable is not None:
+            self.executable.to_hdf(self._hdf5)
         with self._hdf5.open("input") as hdf_input:
             generic_dict = {
                 "restart_file_list": self._restart_file_list,
                 "restart_file_dict": self._restart_file_dict,
                 "exclude_nodes_hdf": self._exclude_nodes_hdf,
                 "exclude_groups_hdf": self._exclude_groups_hdf,
             }
@@ -1220,22 +1024,21 @@
         """
         Restore the GenericJob from an HDF5 file
 
         Args:
             hdf (ProjectHDFio): HDF5 group object - optional
             group_name (str): HDF5 subgroup name - optional
         """
-        if hdf is not None:
-            self._hdf5 = hdf
-        if group_name is not None:
-            self._hdf5 = self._hdf5.open(group_name)
+        self._set_hdf(hdf=hdf, group_name=group_name)
         self._type_from_hdf()
         if "import_directory" in self._hdf5.list_nodes():
             self._import_directory = self._hdf5["import_directory"]
         self._server.from_hdf(self._hdf5)
+        if "executable" in self._hdf5.list_groups():
+            self.executable.from_hdf(self._hdf5)
         with self._hdf5.open("input") as hdf_input:
             if "generic_dict" in hdf_input.list_nodes():
                 generic_dict = hdf_input["generic_dict"]
                 self._restart_file_list = generic_dict["restart_file_list"]
                 self._restart_file_dict = generic_dict["restart_file_dict"]
                 self._exclude_nodes_hdf = generic_dict["exclude_nodes_hdf"]
                 self._exclude_groups_hdf = generic_dict["exclude_groups_hdf"]
@@ -1256,14 +1059,20 @@
         Returns:
             (int): Job ID stored in the database
         """
         self.to_hdf()
         if not state.database.database_is_disabled:
             job_id = self.project.db.add_item_dict(self.db_entry())
             self._job_id = job_id
+            write_hdf5(
+                self.project_hdf5.file_name,
+                job_id,
+                title=self.job_name + "/job_id",
+                overwrite="update",
+            )
             self.refresh_job_status()
         else:
             job_id = self.job_name
         if self._check_if_input_should_be_written():
             self.project_hdf5.create_working_directory()
             self.write_input()
             _copy_restart_files(job=self)
@@ -1352,23 +1161,23 @@
             dict: {'groups': [list of groups], 'nodes': [list of nodes]}
         """
         h5_dict = self.project_hdf5.list_all()
         if self.server.new_hdf:
             h5_dict["groups"] += self._list_ext_childs()
         return h5_dict
 
-    def signal_intercept(self, sig, frame):
+    def signal_intercept(self, sig):
         """
+        Abort the job and log signal that caused it.
 
-        Args:
-            sig:
-            frame:
-
-        Returns:
+        Expected to be called from
+        :func:`pyiron_base.state.signal.catch_signals`.
 
+        Args:
+            sig (int): the signal that triggered the abort
         """
         try:
             self._logger.info(
                 "Job {} intercept signal {}, job is shutting down".format(
                     self._job_id, sig
                 )
             )
@@ -1380,236 +1189,117 @@
         """
         Change the job status to aborted when the job was intercepted.
         """
         self.refresh_job_status()
         if not (self.status.finished or self.status.suspended):
             self.status.aborted = True
 
-    def _run_manually(self, _manually_print=True):
-        """
-        Internal helper function to run a job manually.
-
-        Args:
-            _manually_print (bool): [True/False] print command for execution - default=True
-        """
-        if _manually_print:
-            print(
-                "You have selected to start the job manually. "
-                "To run it, go into the working directory {} and "
-                "call 'python run_job.py' ".format(
-                    posixpath.abspath(self.project_hdf5.working_directory)
-                )
-            )
-
     def _run_if_new(self, debug=False):
         """
         Internal helper function the run if new function is called when the job status is 'initialized'. It prepares
         the hdf5 file and the corresponding directory structure.
 
         Args:
             debug (bool): Debug Mode
         """
-        self.validate_ready_to_run()
-        if self.server.run_mode.queue:
-            self.check_setup()
-        if self.check_if_job_exists():
-            print("job exists already and therefore was not created!")
-        else:
-            self.save()
-            self.run()
+        return run_job_with_status_initialized(job=self, debug=debug)
 
     def _run_if_created(self):
         """
         Internal helper function the run if created function is called when the job status is 'created'. It executes
         the simulation, either in modal mode, meaning waiting for the simulation to finish, manually, or submits the
         simulation to the que.
 
         Returns:
             int: Queue ID - if the job was send to the queue
         """
-        self.status.submitted = True
-
-        # Different run modes
-        if self.server.run_mode.manual:
-            self.run_if_manually()
-        elif self.server.run_mode.worker:
-            self.run_if_manually(_manually_print=False)
-        elif self.server.run_mode.modal:
-            self.run_static()
-        elif (
-            self.server.run_mode.non_modal
-            or self.server.run_mode.thread
-            or self.server.run_mode.worker
-        ):
-            self.run_if_non_modal()
-        elif self.server.run_mode.queue:
-            self.run_if_scheduler()
-        elif self.server.run_mode.interactive:
-            self.run_if_interactive()
-        elif self.server.run_mode.interactive_non_modal:
-            self.run_if_interactive_non_modal()
+        return run_job_with_status_created(job=self)
 
     def _run_if_repair(self):
         """
         Internal helper function the run if repair function is called when the run() function is called with the
         'repair' parameter.
         """
-        self._run_if_created()
-
-    def _run_if_submitted(self):  # Submitted jobs are handled by the job wrapper!
-        """
-        Internal helper function the run if submitted function is called when the job status is 'submitted'. It means
-        the job is waiting in the queue. ToDo: Display a list of the users jobs in the queue.
-        """
-        if (
-            self.server.run_mode.queue
-            and not self.project.queue_check_job_is_waiting_or_running(self)
-        ):
-            if not state.queue_adapter.remote_flag:
-                self.run(delete_existing_job=True)
-            else:
-                self.transfer_from_remote()
-        else:
-            print("Job " + str(self.job_id) + " is waiting in the que!")
+        run_job_with_parameter_repair(job=self)
 
     def _run_if_running(self):
         """
         Internal helper function the run if running function is called when the job status is 'running'. It allows the
         user to interact with the simulation while it is running.
         """
-        if (
-            self.server.run_mode.queue
-            and not self.project.queue_check_job_is_waiting_or_running(self)
-        ):
-            self.run(delete_existing_job=True)
-        elif self.server.run_mode.interactive:
-            self.run_if_interactive()
-        elif self.server.run_mode.interactive_non_modal:
-            self.run_if_interactive_non_modal()
-        else:
-            print("Job " + str(self.job_id) + " is running!")
+        run_job_with_status_running(job=self)
 
     def run_if_refresh(self):
         """
         Internal helper function the run if refresh function is called when the job status is 'refresh'. If the job was
         suspended previously, the job is going to be started again, to be continued.
         """
-        raise NotImplementedError(
-            "Refresh is not supported for this job type for job  " + str(self.job_id)
-        )
+        run_job_with_status_refresh(job=self)
 
     def set_input_to_read_only(self):
         """
-        This function enforces read-only mode for the input classes, but it has to be implement in the individual
+        This function enforces read-only mode for the input classes, but it has to be implemented in the individual
         classes.
         """
         pass
 
     def _run_if_busy(self):
         """
         Internal helper function the run if busy function is called when the job status is 'busy'.
         """
-        raise NotImplementedError(
-            "Refresh is not supported for this job type for job  " + str(self.job_id)
-        )
+        run_job_with_status_busy(job=self)
 
     def _run_if_collect(self):
         """
         Internal helper function the run if collect function is called when the job status is 'collect'. It collects
         the simulation output using the standardized functions collect_output() and collect_logfiles(). Afterwards the
         status is set to 'finished'
         """
-        self.collect_output()
-        self.collect_logfiles()
-        if self.job_id is not None:
-            self.project.db.item_update(self._runtime(), self.job_id)
-        if self.status.collect:
-            if not self.convergence_check():
-                self.status.not_converged = True
-            else:
-                if self._compress_by_default:
-                    self.compress()
-                self.status.finished = True
-            self._hdf5["status"] = self.status.string
-        if self.job_id is not None:
-            self._calculate_successor()
-        self.send_to_database()
-        self.update_master()
+        run_job_with_status_collect(job=self)
 
     def _run_if_suspended(self):
         """
         Internal helper function the run if suspended function is called when the job status is 'suspended'. It
         restarts the job by calling the run if refresh function after setting the status to 'refresh'.
         """
-        self.status.refresh = True
-        self.run()
-
-    @deprecate(
-        run_again="Either delete the job via job.remove() or use delete_existing_job=True.",
-        version="0.4.0",
-    )
-    def _run_if_finished(self, delete_existing_job=False, run_again=False):
-        """
-        Internal helper function the run if finished function is called when the job status is 'finished'. It loads
-        the existing job.
-
-        Args:
-            delete_existing_job (bool): Delete the existing job and run the simulation again.
-            run_again (bool): Same as delete_existing_job (deprecated)
-        """
-        if run_again:
-            delete_existing_job = True
-        if delete_existing_job:
-            parent_id = self.parent_id
-            self.parent_id = None
-            self.remove()
-            self._job_id = None
-            self.status.initialized = True
-            self.parent_id = parent_id
-            self.run()
-        else:
-            self.logger.warning(
-                "The job {} is being loaded instead of running. To re-run use the argument "
-                "'delete_existing_job=True in create_job'".format(self.job_name)
-            )
-            self.from_hdf()
+        run_job_with_status_suspended(job=self)
 
     def _executable_activate(self, enforce=False, codename=None):
         """
         Internal helper function to koad the executable object, if it was not loaded already.
 
         Args:
             enforce (bool): Force the executable module to reinitialize
             codename (str): Name of the resource directory and run script.
         """
         if self._executable is None or enforce:
             if codename is not None:
                 self._executable = Executable(
                     codename=codename,
                     module=codename,
-                    path_binary_codes=state.settings.resource_paths,
+                    path_binary_codes=None,
                 )
             elif len(self.__module__.split(".")) > 1:
                 self._executable = Executable(
                     codename=self.__name__,
                     module=self.__module__.split(".")[-2],
-                    path_binary_codes=state.settings.resource_paths,
+                    path_binary_codes=None,
                 )
             elif self.__module__ == "__main__":
                 # Special case when the job classes defined in Jupyter notebooks
                 parent_class = self.__class__.__bases__[0]
                 self._executable = Executable(
                     codename=parent_class.__name__,
                     module=parent_class.__module__.split(".")[-2],
-                    path_binary_codes=state.settings.resource_paths,
+                    path_binary_codes=None,
                 )
             else:
                 self._executable = Executable(
                     codename=self.__name__,
-                    path_binary_codes=state.settings.resource_paths,
+                    path_binary_codes=None,
                 )
 
     def _type_to_hdf(self):
         """
         Internal helper function to save type and version in HDF5 file root
         """
         self._hdf5["NAME"] = self.__name__
@@ -1622,22 +1312,24 @@
             self._hdf5["HDF_VERSION"] = self.__hdf_version__
 
     def _type_from_hdf(self):
         """
         Internal helper function to load type and version from HDF5 file root
         """
         self.__obj_type__ = self._hdf5["TYPE"]
-        if self._executable:
-            try:
-                self.executable.version = self._hdf5["VERSION"]
-            except ValueError:
-                self.executable.executable_path = self._hdf5["VERSION"]
-        else:
+        if self._executable is None:
             self.__obj_version__ = self._hdf5["VERSION"]
 
+    def run_time_to_db(self):
+        """
+        Internal helper function to store the run_time in the database
+        """
+        if not state.database.database_is_disabled and self.job_id is not None:
+            self.project.db.item_update(self._runtime(), self.job_id)
+
     def _runtime(self):
         """
         Internal helper function to calculate runtime by substracting the starttime, from the stoptime.
 
         Returns:
             (dict): Database dictionary db_dict
         """
@@ -1775,17 +1467,7 @@
         return self._print_error(file_name="error.out", string=string)
 
     def _print_error(self, file_name, string="", print_yes=True):
         if self._job[file_name] is None:
             return ""
         elif print_yes:
             return string.join(self._job[file_name])
-
-
-def multiprocess_wrapper(job_id, working_dir, debug=False, connection_string=None):
-    job_wrap = JobWrapper(
-        working_directory=str(working_dir),
-        job_id=int(job_id),
-        debug=debug,
-        connection_string=connection_string,
-    )
-    job_wrap.job.run_static()
```

### Comparing `pyiron_base-0.5.9/pyiron_base/job/interactive.py` & `pyiron_base-0.6.0/pyiron_base/jobs/job/interactive.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 InteractiveBase class extends the Generic Job class with all the functionality to run the job object interactivley.
 """
 
 import numpy as np
-from pyiron_base.job.generic import GenericJob
+from pyiron_base.database.filetable import FileTable
+from pyiron_base.jobs.job.generic import GenericJob
 
 __author__ = "Osamu Waseda, Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -296,17 +297,20 @@
         Sets the job status to :attr:`~.JobStatus.finished`, :meth:`.run()` cannot be called after this.
         """
         if (
             len(list(self.interactive_cache.keys())) > 0
             and len(self.interactive_cache[list(self.interactive_cache.keys())[0]]) != 0
         ):
             self.interactive_flush(path="interactive", include_last_step=True)
-        self.project_hdf5.rewrite_hdf5(job_name=self.job_name, exclude_groups=[])
-        self.project.db.item_update(self._runtime(), self._job_id)
+        self.project_hdf5.rewrite_hdf5()
         self.status.finished = True
+        if not isinstance(self.project.db, FileTable):
+            self.run_time_to_db()
+        else:
+            self._hdf5["status"] = self.status.string
         self._interactive_library = None
         for key in self.interactive_cache.keys():
             self.interactive_cache[key] = []
 
     def interactive_store_in_cache(self, key, value):
         """
```

### Comparing `pyiron_base-0.5.9/pyiron_base/job/interactivewrapper.py` & `pyiron_base-0.6.0/pyiron_base/jobs/master/interactivewrapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from datetime import datetime
 import warnings
-from pyiron_base.generic.parameters import GenericParameters
-from pyiron_base.job.generic import GenericJob
-from pyiron_base.master.generic import GenericMaster
-from pyiron_base.generic.util import deprecate
+
+from pyiron_base.storage.parameters import GenericParameters
+from pyiron_base.jobs.job.generic import GenericJob
+from pyiron_base.jobs.master.generic import GenericMaster
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -132,29 +132,7 @@
         self._db_entry_update_run_time()
         self._logger.info(
             "{}, status: {}, monte carlo master".format(self.job_info_str, self.status)
         )
         self._calculate_successor()
         self.send_to_database()
         self.update_master()
-
-    def __getitem__(self, item):
-        """
-        Get/ read data from the GenericMaster
-
-        Args:
-            item (str, slice): path to the data or key of the data object
-
-        Returns:
-            dict, list, float, int: data or data object
-        """
-        child_id_lst = self.child_ids
-        child_name_lst = [
-            self.project.db.get_item_by_id(child_id)["job"]
-            for child_id in self.child_ids
-        ]
-        if isinstance(item, int):
-            total_lst = child_name_lst + self._job_name_lst
-            item = total_lst[item]
-        return self._get_item_when_str(
-            item=item, child_id_lst=child_id_lst, child_name_lst=child_name_lst
-        )
```

### Comparing `pyiron_base-0.5.9/pyiron_base/job/jobstatus.py` & `pyiron_base-0.6.0/pyiron_base/jobs/job/extension/jobstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.9/pyiron_base/job/jobtype.py` & `pyiron_base-0.6.0/pyiron_base/jobs/job/jobtype.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,78 +4,94 @@
 """
 Jobtype class to create GenericJob type objects
 """
 
 import importlib
 import inspect
 import os
-from pyiron_base.job.util import _get_safe_job_name
-from pyiron_base.generic.hdfio import ProjectHDFio
-from pyiron_base.generic.util import Singleton
-from pyiron_base.generic.factory import PyironFactory
-from pyiron_base.job.jobstatus import job_status_finished_lst
-from pyiron_base.generic.dynamic import JOB_DYN_DICT, class_constructor
+from pyiron_base.jobs.job.util import _get_safe_job_name
+from pyiron_base.storage.hdfio import ProjectHDFio
+from pyiron_base.interfaces.singleton import Singleton
+from pyiron_base.interfaces.factory import PyironFactory
+from pyiron_base.jobs.job.extension.jobstatus import job_status_finished_lst
+from pyiron_base.jobs.dynamic import JOB_DYN_DICT, class_constructor
+from typing import Type, Union
 
 __author__ = "Joerg Neugebauer, Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 
 JOB_CLASS_DICT = {
-    "FlexibleMaster": "pyiron_base.master.flexible",
-    "ScriptJob": "pyiron_base.job.script",
-    "SerialMasterBase": "pyiron_base.master.serial",
-    "TableJob": "pyiron_base.table.datamining",
-    "WorkerJob": "pyiron_base.job.worker",
+    "FlexibleMaster": "pyiron_base.jobs.master.flexible",
+    "ScriptJob": "pyiron_base.jobs.script",
+    "SerialMasterBase": "pyiron_base.jobs.master.serial",
+    "TableJob": "pyiron_base.jobs.datamining",
+    "WorkerJob": "pyiron_base.jobs.worker",
 }
 
 
-class JobType(object):
+class JobType:
     """
     The JobTypeBase class creates a new object of a given class type.
     """
 
+    _job_class_dict = JOB_CLASS_DICT
+
     def __new__(
         cls,
         class_name,
         project,
         job_name,
-        job_class_dict,
+        job_class_dict=None,
         delete_existing_job=False,
         delete_aborted_job=False,
     ):
         """
         The __new__() method allows to create objects from other classes - the class selected by class_name
 
         Args:
-            class_name (str): The specific class name of the class this object belongs to.
+            class_name (str/Type('GenericJob')): The specific class name of the class this object belongs to.
             project (Project): Project object (defines path where job will be created and stored)
             job_name (str): name of the job (must be unique within this project path)
             job_class_dict (dict): dictionary with the jobtypes to choose from.
             delete_existing_job (bool): delete an existing job - default false
             delete_aborted_job (bool): delete an existing and aborted job - default false
 
         Returns:
             GenericJob: object of type class_name
         """
         job_name = _get_safe_job_name(job_name)
-        cls.job_class_dict = job_class_dict
+        cls.job_class_dict = job_class_dict or cls._job_class_dict
         if isinstance(class_name, str):
             job_class = cls.convert_str_to_class(
                 job_class_dict=cls.job_class_dict, class_name=class_name
             )
         elif inspect.isclass(class_name):
-            job_class = class_name
+            if (
+                class_name.__name__ not in cls._job_class_dict
+                or cls._convert_pyiron_to_pyiron_atomistics_module(
+                    class_name.__module__
+                )
+                == cls._job_class_dict[class_name.__name__]
+            ):
+                job_class = class_name
+            else:
+                raise ValueError(
+                    f"You are trying to instantiate a job with the class {class_name} named {class_name.__name__} "
+                    f"from module {class_name.__module__}, however, this name has already been registered with the"
+                    f" module {cls._job_class_dict[class_name.__name__]}."
+                )
         else:
             raise TypeError()
         job = job_class(project, job_name)
         if job.job_id is not None and not os.path.exists(job.project_hdf5.file_name):
             job.logger.warning(
                 "No HDF5 file found - remove database entry and create new job! {}".format(
                     job.job_name
@@ -91,16 +107,93 @@
             )
         if not job.status.initialized:
             job.from_hdf()
         if job.status.string in job_status_finished_lst:
             job.set_input_to_read_only()
         return job
 
+    @classmethod
+    def unregister(cls, job_name_or_class):
+        """Unregister job type from the exposed list of available job types
+
+        Args:
+            job_name_or_class(str/type): name of the job or job class
+
+        Returns:
+            None if a str is provided as job_name_or_class
+            job_name_or_class if a class is provided. Therefore, this method can be used as class decorator.
+        """
+        _cls = None
+        if isinstance(job_name_or_class, type):
+            _cls = job_name_or_class
+            job_name_or_class = job_name_or_class.__name__
+        if job_name_or_class in cls._job_class_dict:
+            del cls._job_class_dict[job_name_or_class]
+        else:
+            raise KeyError(f"No JobType with name '{job_name_or_class}' found.")
+        return _cls
+
     @staticmethod
-    def convert_str_to_class(job_class_dict, class_name):
+    def _convert_pyiron_to_pyiron_atomistics_module(cls_module_str):
+        if cls_module_str.startswith("pyiron."):
+            # Currently, we set all sub-modules of pyiron_atomistics to be sub-modules of pyiron. Thus, any class
+            # pyiron.submodule.PyironClass is identical to pyiron_atomistics_submodule.PyironClass:
+            cls_module_str = cls_module_str.replace("pyiron.", "pyiron_atomistics.")
+        return cls_module_str
+
+    @classmethod
+    def register(
+        cls,
+        job_class_or_module_str: Union[type, str],
+        job_name: str = None,
+        overwrite=False,
+    ):
+        """Register job type from the exposed list of available job types
+
+        Args:
+            job_class_or_module_str(type/str/None): job class itself, string representation of the job class module as
+                provided by cls.__module__, or None for do not register.
+            job_name(str/None): Name of the job to register. Must match cls.__name__. Can be omitted for class input.
+            overwrite(bool): If True, overwrite existing job type.
+        """
+        if job_class_or_module_str is None:
+            return
+        elif isinstance(job_class_or_module_str, type):
+            cls_module_str = cls._convert_pyiron_to_pyiron_atomistics_module(
+                job_class_or_module_str.__module__
+            )
+            if job_name is not None and job_class_or_module_str.__name__ != job_name:
+                raise NotImplementedError(
+                    "Currently, the given name has to match the class name."
+                )
+            else:
+                job_name = job_class_or_module_str.__name__
+        elif job_name is not None:
+            cls_module_str = cls._convert_pyiron_to_pyiron_atomistics_module(
+                job_class_or_module_str
+            )
+        else:
+            raise ValueError(
+                "The job_name needs to be provided if a job_module_string is provided."
+            )
+
+        if (
+            not overwrite
+            and job_name in cls._job_class_dict
+            and cls_module_str != cls._job_class_dict[job_name]
+        ):
+            ValueError(
+                f"A JobType with name '{job_name}' is already defined! New class = '{cls_module_str}', "
+                f"already registered class = '{cls._job_class_dict[job_name]}'."
+            )
+        else:
+            cls._job_class_dict[job_name] = cls_module_str
+
+    @staticmethod
+    def convert_str_to_class(job_class_dict, class_name) -> Type["GenericJob"]:
         """
         convert the name of a class to the corresponding class object - only for pyiron internal classes.
 
         Args:
             job_class_dict (dict):
             class_name (str):
 
@@ -141,15 +234,17 @@
     def __dir__(self):
         """
         Enable autocompletion by overwriting the __dir__() function.
         """
         return list(self._job_class_dict.keys()) + list(self._job_dyn_dict.keys())
 
     def __getattr__(self, name):
-        if name in self._job_class_dict.keys():
+        # FIXME: due to a bug in job registration dynamically created jobs are also present in self._job_class_dict, so
+        # we first have to check whether name is in _job_dyn_dict before we check the general _job_class_dict
+        if name in self._job_dyn_dict:
 
             def wrapper(job_name, delete_existing_job=False, delete_aborted_job=False):
                 """
                 Create one of the following jobs:
                 - 'ExampleJob': example job just generating random number
                 - 'SerialMaster': series of jobs run in serial
                 - 'ParallelMaster': series of jobs run in parallel
@@ -167,59 +262,57 @@
                 job_name = _get_safe_job_name(job_name)
                 return JobType(
                     class_name=name,
                     project=ProjectHDFio(
                         project=self._project.copy(), file_name=job_name
                     ),
                     job_name=job_name,
-                    job_class_dict=self._job_class_dict,
+                    job_class_dict={
+                        name: class_constructor(cp=cp)
+                        for name, cp in self._job_dyn_dict.items()
+                    },
                     delete_existing_job=delete_existing_job,
                     delete_aborted_job=delete_aborted_job,
                 )
 
             return wrapper
-        else:
-            if name in self._job_dyn_dict.keys():
 
-                def wrapper(
-                    job_name, delete_existing_job=False, delete_aborted_job=False
-                ):
-                    """
-                    Create one of the following jobs:
-                    - 'ExampleJob': example job just generating random number
-                    - 'SerialMaster': series of jobs run in serial
-                    - 'ParallelMaster': series of jobs run in parallel
-                    - 'ScriptJob': Python script or jupyter notebook job container
-                    - 'ListMaster': list of jobs
-
-                    Args:
-                        job_name (str): name of the job
-                        delete_existing_job (bool): delete an existing job - default false
-                        delete_aborted_job (bool): delete an existing and aborted job - default false
-
-                    Returns:
-                        GenericJob: job object depending on the job_type selected
-                    """
-                    job_name = _get_safe_job_name(job_name)
-                    return JobType(
-                        class_name=name,
-                        project=ProjectHDFio(
-                            project=self._project.copy(), file_name=job_name
-                        ),
-                        job_name=job_name,
-                        job_class_dict={
-                            name: class_constructor(cp=cp)
-                            for name, cp in self._job_dyn_dict.items()
-                        },
-                        delete_existing_job=delete_existing_job,
-                        delete_aborted_job=delete_aborted_job,
-                    )
+        elif name in self._job_class_dict:
+
+            def wrapper(job_name, delete_existing_job=False, delete_aborted_job=False):
+                """
+                Create one of the following jobs:
+                - 'ExampleJob': example job just generating random number
+                - 'SerialMaster': series of jobs run in serial
+                - 'ParallelMaster': series of jobs run in parallel
+                - 'ScriptJob': Python script or jupyter notebook job container
+                - 'ListMaster': list of jobs
 
-                return wrapper
+                Args:
+                    job_name (str): name of the job
+                    delete_existing_job (bool): delete an existing job - default false
+                    delete_aborted_job (bool): delete an existing and aborted job - default false
 
+                Returns:
+                    GenericJob: job object depending on the job_type selected
+                """
+                job_name = _get_safe_job_name(job_name)
+                return JobType(
+                    class_name=name,
+                    project=ProjectHDFio(
+                        project=self._project.copy(), file_name=job_name
+                    ),
+                    job_name=job_name,
+                    job_class_dict=self._job_class_dict,
+                    delete_existing_job=delete_existing_job,
+                    delete_aborted_job=delete_aborted_job,
+                )
+
+            return wrapper
+        else:
             raise AttributeError("no job class named '{}' defined".format(name))
 
 
 class JobTypeChoice(metaclass=Singleton):
     """
     Helper class to choose the job type directly from the project, autocompletion is enabled by overwriting the
     __dir__() function. This class is only required for pr.job_type.Code which is only used in pr.create_job().
```

### Comparing `pyiron_base-0.5.9/pyiron_base/job/path.py` & `pyiron_base-0.6.0/pyiron_base/jobs/job/path.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,44 +2,36 @@
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 The JobPath class enables quick access to the HDF5 data file without loading the full object
 """
 
 import os
-import posixpath
-from pyiron_base.generic.hdfio import ProjectHDFio
-from pyiron_base.job.core import JobCore
+from pyiron_base.storage.hdfio import ProjectHDFio
+from pyiron_base.jobs.job.core import JobCore
 from pyiron_base.project.generic import Project
 
 __author__ = "Joerg Neugebauer, Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 
-class JobPathBase(JobCore):
+class JobPath(JobCore):
     """
     The JobPath class is derived from the JobCore and is used as a lean version of the GenericJob class. Instead of
     loading the full pyiron object the JobPath class only provides access to the HDF5 file, which should be enough
     for most analysis.
 
-    Args:
-        db (DatabaseAccess): database object
-        job_id (int): Job ID - optional, but either a job ID or a database entry db_entry has to be provided.
-        db_entry (dict): database entry {"job":, "subjob":, "projectpath":, "project":, "hamilton":, "hamversion":,
-                                         "status":} and optional entries are {"id":, "masterid":, "parentid":}
-        user (str): current unix/linux/windows user who is running pyiron
-
     Attributes:
 
         .. attribute:: job_name
 
             name of the job, which has to be unique within the project
 
         .. attribute:: status
@@ -106,14 +98,20 @@
 
         .. attribute:: h5_path
 
             path inside the HDF5 file - also stored as absolute path
     """
 
     def __init__(self, job_path):
+        """
+        Load a job from the given path.
+
+        Args:
+            job_path (str): path to the job, must be of the form /path/to/file.h5/job_name
+        """
         job_path_lst = job_path.replace("\\", "/").split(".h5")
         if len(job_path_lst) != 2:
             raise ValueError
 
         sub_job = job_path_lst[1]
         h5_path = None
         if sub_job is not None:
@@ -122,17 +120,61 @@
 
         hdf_project = ProjectHDFio(
             project=Project(os.path.dirname(job_path_lst[0])),
             file_name=job_path_lst[0].split("/")[-1] + ".h5",
             h5_path=h5_path,
             mode="r",
         )
-        super(JobPathBase, self).__init__(
-            project=hdf_project, job_name=job_path_lst[1].split("/")[-1]
-        )
+        super().__init__(project=hdf_project, job_name=job_path_lst[1].split("/")[-1])
+
+    @classmethod
+    def from_job_id(cls, db, job_id):
+        """
+        Load a job path from a database connection and the job id.
+
+        Args:
+            db (DatabaseAccess): database connection
+            job_id (int): Job ID in the database
+        """
+        db_entry = db.get_item_by_id(job_id)
+        if db_entry is None:
+            raise ValueError("job ID {0} does not exist!".format(job_id))
+
+        return cls.from_db_entry(db_entry)
+
+    @classmethod
+    def from_db_entry(cls, db_entry):
+        """
+        Load a job path from a database entry.
+
+        Args:
+            db_entry (dict): database entry {"job":, "subjob":, "projectpath":, "project":, "hamilton":, "hamversion":,
+                                            "status":} and optional entries are {"id":, "masterid":, "parentid":}
+        """
+        hdf5_file = db_entry["subjob"].split("/")[1] + ".h5"
+        job_path = db_entry["projectpath"]
+        if job_path is None:
+            job_path = ""
+        job_path += db_entry["project"] + hdf5_file + db_entry["subjob"]
+        job = cls(job_path=job_path)
+
+        if "hamilton" in db_entry.keys():
+            job.__name__ = db_entry["hamilton"]
+        if "hamversion" in db_entry.keys():
+            job.__version__ = db_entry["hamversion"]
+
+        if "id" in db_entry.keys():
+            job._job_id = db_entry["id"]
+        if "status" in db_entry.keys():
+            job._status = db_entry["status"]
+        if "masterid" in db_entry.keys():
+            job._master_id = db_entry["masterid"]
+        if "parentid" in db_entry.keys():
+            job._parent_id = db_entry["parentid"]
+        return job
 
     @property
     def is_root(self):
         """
         Check if the current h5_path is pointing to the HDF5 root group.
 
         Returns:
@@ -355,137 +397,7 @@
         """
         When the object is deleted the HDF5 file has to be closed
         """
         try:
             self.project_hdf5._store.close()
         except AttributeError:
             pass
-
-    def __getitem__(self, item):
-        """
-        Get/ read data from the HDF5 file
-
-        Args:
-            item (str, slice): path to the data or key of the data object
-
-        Returns:
-            dict, list, float, int: data or data object
-        """
-        if item in self.list_files():
-            file_name = posixpath.join(self.working_directory, "{}".format(item))
-            with open(file_name) as f:
-                return f.readlines()
-        return self.project_hdf5.__getitem__(item)
-
-
-class JobPath(JobPathBase):
-    """
-    The JobPath class is derived from the JobCore and is used as a lean version of the GenericJob class. Instead of
-    loading the full pyiron object the JobPath class only provides access to the HDF5 file, which should be enough
-    for most analysis.
-
-    Args:
-        db (DatabaseAccess): database object
-        job_id (int): Job ID - optional, but either a job ID or a database entry db_entry has to be provided.
-        db_entry (dict): database entry {"job":, "subjob":, "projectpath":, "project":, "hamilton":, "hamversion":,
-                                         "status":} and optional entries are {"id":, "masterid":, "parentid":}
-        user (str): current unix/linux/windows user who is running pyiron
-
-    Attributes:
-
-        .. attribute:: job_name
-
-            name of the job, which has to be unique within the project
-
-        .. attribute:: status
-
-            execution status of the job, can be one of the following [initialized, appended, created, submitted, running,
-                                                                      aborted, collect, suspended, refresh, busy, finished]
-
-        .. attribute:: job_id
-
-            unique id to identify the job in the pyiron database
-
-        .. attribute:: parent_id
-
-            job id of the predecessor job - the job which was executed before the current one in the current job series
-
-        .. attribute:: master_id
-
-            job id of the master job - a meta job which groups a series of jobs, which are executed either in parallel or in
-            serial.
-
-        .. attribute:: child_ids
-
-            list of child job ids - only meta jobs have child jobs - jobs which list the meta job as their master
-
-        .. attribute:: project
-
-            Project instance the jobs is located in
-
-        .. attribute:: project_hdf5
-
-            ProjectHDFio instance which points to the HDF5 file the job is stored in
-
-        .. attribute:: job_info_str
-
-            short string to describe the job by it is job_name and job ID - mainly used for logging
-
-        .. attribute:: working_directory
-
-            working directory of the job is executed in - outside the HDF5 file
-
-        .. attribute:: path
-
-            path to the job as a combination of absolute file system path and path within the HDF5 file.
-
-        .. attribute:: is_root
-
-            boolean if the HDF5 object is located at the root level of the HDF5 file
-
-        .. attribute:: is_open
-
-            boolean if the HDF5 file is currently opened - if an active file handler exists
-
-        .. attribute:: is_empty
-
-            boolean if the HDF5 file is empty
-
-        .. attribute:: base_name
-
-            name of the HDF5 file but without any file extension
-
-        .. attribute:: file_path
-
-            directory where the HDF5 file is located
-
-        .. attribute:: h5_path
-
-            path inside the HDF5 file - also stored as absolute path
-    """
-
-    def __init__(self, db, job_id=None, db_entry=None, user=None):
-        if db_entry is None and db is not None:
-            db_entry = db.get_item_by_id(job_id)
-        if db_entry is None:
-            raise ValueError("job ID {0} does not exist!".format(job_id))
-        hdf5_file = db_entry["subjob"].split("/")[1] + ".h5"
-        if db_entry["projectpath"] is not None:
-            job_path = db_entry["projectpath"]
-        else:
-            job_path = ""
-        job_path += db_entry["project"] + hdf5_file + db_entry["subjob"]
-        super(JobPath, self).__init__(job_path=job_path)
-
-        if "hamilton" in db_entry.keys():
-            self.__name__ = db_entry["hamilton"]
-        if "hamversion" in db_entry.keys():
-            self.__version__ = db_entry["hamversion"]
-
-        if "id" in db_entry.keys():
-            self._job_id = db_entry["id"]
-        if "status" in db_entry.keys():
-            self._status = db_entry["status"]
-        if "masterid" in db_entry.keys():
-            self._master_id = db_entry["masterid"]
-        if "parentid" in db_entry.keys():
-            self._parent_id = db_entry["parentid"]
```

### Comparing `pyiron_base-0.5.9/pyiron_base/job/script.py` & `pyiron_base-0.6.0/pyiron_base/jobs/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 Jobclass to execute python scripts and jupyter notebooks
 """
 
 import os
 import shutil
-from pyiron_base.job.generic import GenericJob
-from pyiron_base.generic.parameters import GenericParameters
-from pyiron_base.generic.datacontainer import DataContainer
+from pyiron_base.jobs.job.generic import GenericJob
+from pyiron_base.storage.parameters import GenericParameters
+from pyiron_base.storage.datacontainer import DataContainer
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -322,14 +322,15 @@
         else:
             raise ValueError("Cannot handle hdf version: {}".format(version))
 
     def write_input(self):
         """
         Copy the script to the working directory - only python scripts and jupyter notebooks are supported
         """
+        super().write_input()
         if self._script_path is not None:
             file_name = os.path.basename(self._script_path)
             shutil.copyfile(
                 src=self._script_path,
                 dst=os.path.join(self.working_directory, file_name),
             )
             self.executable = self._executable_command(
```

### Comparing `pyiron_base-0.5.9/pyiron_base/job/template.py` & `pyiron_base-0.6.0/pyiron_base/jobs/job/template.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 Template class to define jobs
 """
 
-from pyiron_base.job.generic import GenericJob
-from pyiron_base.generic.object import HasStorage
+from pyiron_base.jobs.job.generic import GenericJob
+from pyiron_base.interfaces.object import HasStorage
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -19,35 +19,33 @@
 __status__ = "development"
 __date__ = "May 15, 2020"
 
 
 class TemplateJob(GenericJob, HasStorage):
     def __init__(self, project, job_name):
         GenericJob.__init__(self, project, job_name)
-        HasStorage.__init__(self)
+        HasStorage.__init__(self, group_name="")
         self.storage.create_group("input")
         self.storage.create_group("output")
 
     @property
     def input(self):
         return self.storage.input
 
     @property
     def output(self):
         return self.storage.output
 
     def to_hdf(self, hdf=None, group_name=None):
         GenericJob.to_hdf(self, hdf=hdf, group_name=group_name)
-        HasStorage.to_hdf(self, hdf=self.project_hdf5, group_name="")
+        HasStorage.to_hdf(self, hdf=self.project_hdf5)
 
     def from_hdf(self, hdf=None, group_name=None):
         GenericJob.from_hdf(self, hdf=hdf, group_name=group_name)
-        HasStorage.from_hdf(self, hdf=self.project_hdf5, group_name="")
+        HasStorage.from_hdf(self, hdf=self.project_hdf5)
 
 
 class PythonTemplateJob(TemplateJob):
     def __init__(self, project, job_name):
         super().__init__(project, job_name)
         self._python_only_job = True
-
-    def _check_if_input_should_be_written(self):
-        return False
+        self._write_work_dir_warnings = False
```

### Comparing `pyiron_base-0.5.9/pyiron_base/job/util.py` & `pyiron_base-0.6.0/pyiron_base/jobs/job/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,52 +3,50 @@
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 Helper functions for the JobCore and GenericJob objects
 """
 import os
 import posixpath
 import psutil
-from pyiron_base.generic.util import static_isinstance
 import tarfile
 import stat
 import shutil
-from typing import Union, Dict
+from typing import Optional, Union
+from pyiron_base.utils.instance import static_isinstance
+from pyiron_base.utils.safetar import safe_extract
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "production"
 __date__ = "Nov 28, 2020"
 
 
-def _copy_database_entry(new_job_core, job_copied_id, new_database_entry=True):
+def _copy_database_entry(new_job_core, job_copied_id):
     """
     Copy database entry from previous job
 
     Args:
         new_job_core (GenericJob): Copy of the job object
         job_copied_id (int): Job id of the copied job
-        new_database_entry (bool): [True/False] to create a new database entry - default True
     """
-    if new_database_entry:
-        db_entry = new_job_core.project.db.get_item_by_id(job_copied_id)
-        if db_entry is not None:
-            db_entry["project"] = new_job_core.project_hdf5.project_path
-            db_entry["projectpath"] = new_job_core.project_hdf5.root_path
-            db_entry["subjob"] = new_job_core.project_hdf5.h5_path
-            del db_entry["id"]
-            job_id = new_job_core.project.db.add_item_dict(db_entry)
-            new_job_core.reset_job_id(job_id=job_id)
-    else:
-        new_job_core.reset_job_id(job_id=None)
+    db_entry = new_job_core.project.db.get_item_by_id(job_copied_id)
+    if db_entry is not None:
+        db_entry["job"] = new_job_core.job_name
+        db_entry["subjob"] = new_job_core.project_hdf5.h5_path
+        db_entry["project"] = new_job_core.project_hdf5.project_path
+        db_entry["projectpath"] = new_job_core.project_hdf5.root_path
+        del db_entry["id"]
+        job_id = new_job_core.project.db.add_item_dict(db_entry)
+        new_job_core.reset_job_id(job_id=job_id)
 
 
 def _copy_to_delete_existing(project_class, job_name, delete_job):
     """
     Check if the job exists already in the project, if that is the case either
     delete it or reload it depending on the setting of delete_job
 
@@ -83,15 +81,15 @@
             project is `None` or the same project as the copied job. (Default is None,
             try to keep the same name.)
 
     Returns:
         Project, ProjectHDFio
     """
     if static_isinstance(
-        obj=project.__class__, obj_type="pyiron_base.job.core.JobCore"
+        obj=project.__class__, obj_type="pyiron_base.jobs.job.core.JobCore"
     ):
         file_project = project.project
         hdf5_project = project.project_hdf5.open(new_job_name)
     elif isinstance(project, job.project.__class__):
         file_project = project
         hdf5_project = job.project_hdf5.__class__(
             project=project, file_name=new_job_name, h5_path="/" + new_job_name
@@ -115,16 +113,33 @@
     "+": "p",
     ",": "c",
     " ": "_",
 }
 
 
 def _get_safe_job_name(
-    name: str, ndigits: Union[int, None] = 8, special_symbols: Union[Dict, None] = None
+    name: Union[str, tuple],
+    ndigits: Optional[int] = 8,
+    special_symbols: Optional[dict] = None,
 ):
+    """
+    Sanitize a job name, optionally appending numeric values.
+
+    Args:
+        name (str|tuple): The name to sanitize, or a tuple of the name and any number
+            of numeric values to append with '_' in between.
+        ndigits (int|None): How many digits to round any floating point values in a
+            `name` tuple to. (Default is 8; to not round at all use None.)
+        special_symbols (dict|None): Conversions of special symbols to apply. This will
+            be applied to the default conversion dict, which contains:
+            DEFAULT_CONV_DICT
+
+    Returns:
+        (str): The sanitized (and possibly rounded) name.
+    """
     d_special_symbols = _special_symbol_replacements.copy()
     if special_symbols is not None:
         d_special_symbols.update(special_symbols)
 
     def round_(value, ndigits=ndigits):
         if isinstance(value, float) and ndigits is not None:
             return round(value, ndigits=ndigits)
@@ -137,14 +152,19 @@
         job_name = name
     for k, v in d_special_symbols.items():
         job_name = job_name.replace(k, v)
     _is_valid_job_name(job_name=job_name)
     return job_name
 
 
+_get_safe_job_name.__doc__ = _get_safe_job_name.__doc__.replace(
+    "DEFAULT_CONV_DICT", f"{_special_symbol_replacements}"
+)
+
+
 def _rename_job(job, new_job_name):
     """ """
     new_job_name = _get_safe_job_name(new_job_name)
     child_ids = job.child_ids
     if child_ids:
         for child_id in child_ids:
             ham = job.project.load(child_id)
@@ -219,15 +239,15 @@
     Internal helper function to kill a child process.
 
     Args:
         job (JobCore): job object to decompress
     """
     if (
         static_isinstance(
-            obj=job.__class__, obj_type="pyiron_base.master.GenericMaster"
+            obj=job.__class__, obj_type="pyiron_base.jobs.master.GenericMaster"
         )
         and not job.server.run_mode.queue
         and (job.status.running or job.status.submitted)
     ):
         for proc in psutil.process_iter():
             try:
                 pinfo = proc.as_dict(attrs=["pid", "cwd"])
@@ -281,15 +301,15 @@
 
     Args:
         job (JobCore): job object to decompress
     """
     try:
         tar_file_name = os.path.join(job.working_directory, job.job_name + ".tar.bz2")
         with tarfile.open(tar_file_name, "r:bz2") as tar:
-            tar.extractall(job.working_directory)
+            safe_extract(tar, job.working_directory)
         os.remove(tar_file_name)
     except IOError:
         pass
 
 
 def _job_is_compressed(job):
     """
@@ -344,15 +364,15 @@
     Args:
         job (JobCore): job object to unarchive
     """
     fpath = job.project_hdf5.file_path
     try:
         tar_name = os.path.join(fpath, job.job_name + ".tar.bz2")
         with tarfile.open(tar_name, "r:bz2") as tar:
-            tar.extractall(fpath)
+            safe_extract(tar, fpath)
         os.remove(tar_name)
     finally:
         pass
 
 
 def _job_is_archived(job):
     """
```

### Comparing `pyiron_base-0.5.9/pyiron_base/job/worker.py` & `pyiron_base-0.6.0/pyiron_base/jobs/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import psutil
 import time
 from datetime import datetime
 from multiprocessing import Pool
 import numpy as np
 from pyiron_base.state import state
-from pyiron_base.job.template import PythonTemplateJob
+from pyiron_base.jobs.job.template import PythonTemplateJob
 
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -131,14 +131,16 @@
             self.input.project = project.path
         else:
             self.input.project = self.working_directory
         self.input.cores_per_job = 1
         self.input.sleep_interval = 10
         self.input.child_runtime = 0
         self.input.queue_limit_factor = 2
+        self.input.maxtasksperchild = 1
+        self._python_only_job = True
 
     @property
     def project_to_watch(self):
         rel_path = os.path.relpath(self.input.project, self.project.path)
         return self.project.open(rel_path)
 
     @project_to_watch.setter
@@ -189,15 +191,17 @@
         master_id = self.job_id
         pr = self.project_to_watch
         self.project_hdf5.create_working_directory()
         log_file = os.path.join(self.working_directory, "worker.log")
         active_job_ids, res_lst = [], []
         process = psutil.Process(os.getpid())
         number_tasks = int(self.server.cores / self.cores_per_job)
-        with Pool(processes=number_tasks) as pool:
+        with Pool(
+            processes=number_tasks, maxtasksperchild=self.input.maxtasksperchild
+        ) as pool:
             while True:
                 # Check the database if there are more calculation to execute
                 df = pr.job_table()
                 df_sub = df[
                     (df["status"] == "submitted")
                     & (df["masterid"] == master_id)
                     & (~df["id"].isin(active_job_ids))
```

### Comparing `pyiron_base-0.5.9/pyiron_base/job/wrapper.py` & `pyiron_base-0.6.0/pyiron_base/jobs/job/wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,17 +45,19 @@
         working_directory,
         job_id=None,
         hdf5_file=None,
         h5_path=None,
         submit_on_remote=False,
         debug=False,
         connection_string=None,
+        collect=False,
     ):
         self.working_directory = working_directory
         self._remote_flag = submit_on_remote
+        self._collect = collect
         if connection_string is not None:
             state.database.open_local_sqlite_connection(
                 connection_string=connection_string
             )
         pr = Project(path=os.path.join(working_directory, "..", ".."))
         if job_id is not None:
             self.job = pr.load(int(job_id))
@@ -116,44 +118,54 @@
     def run(self):
         """
         The job wrapper run command, sets the job status to 'running' and executes run_if_modal().
         """
         if self._remote_flag and self.job.server.queue is not None:
             self.job.run_if_scheduler()
             self.job.status.submitted = True
+        elif self._collect:
+            self.job.status.collect = True
+            self.job.run()
         else:
             self.job.run_static()
 
 
 def job_wrapper_function(
-    working_directory, job_id=None, file_path=None, submit_on_remote=False, debug=False
+    working_directory,
+    job_id=None,
+    file_path=None,
+    submit_on_remote=False,
+    debug=False,
+    collect=False,
 ):
     """
     Job Wrapper function - creates a JobWrapper object and calls run() on that object
 
     Args:
         working_directory (str): directory where the HDF5 file of the job is located
         job_id (int/ None): job id
         file_path (str): path to the HDF5 file
         debug (bool): enable debug mode
         submit_on_remote (bool): submit to queuing system on remote host
+        collect (bool): collect output of calculation
     """
 
     # always close the database connection in calculations on the cluster to avoid high number of concurrent
     # connections.
     state.database.close_connection()
     state.database.connection_timeout = 0
     state.database.open_connection()
 
     if job_id is not None:
         job = JobWrapper(
             working_directory=working_directory,
             job_id=job_id,
             submit_on_remote=submit_on_remote,
             debug=debug,
+            collect=collect,
         )
     elif file_path is not None:
         hdf5_file = (
             ".".join(file_path.split(".")[:-1])
             + "."
             + file_path.split(".")[-1].split("/")[0]
         )
@@ -161,11 +173,12 @@
         job = JobWrapper(
             working_directory,
             job_id=None,
             hdf5_file=hdf5_file,
             h5_path="/" + h5_path,
             submit_on_remote=submit_on_remote,
             debug=debug,
+            collect=collect,
         )
     else:
         raise ValueError("Either job_id or file_path have to be not None.")
     job.run()
```

### Comparing `pyiron_base-0.5.9/pyiron_base/master/flexible.py` & `pyiron_base-0.6.0/pyiron_base/jobs/master/flexible.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,124 +2,40 @@
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 The Flexible master uses a list of functions to connect multiple jobs in a series.
 """
 
 import inspect
-from pyiron_base.master.generic import GenericMaster
-from pyiron_base.job.jobstatus import job_status_finished_lst
+from pyiron_base.jobs.job.core import _doc_str_job_core_args
+from pyiron_base.jobs.master.generic import GenericMaster, _doc_str_generic_master_attr
+from pyiron_base.jobs.job.extension.jobstatus import job_status_finished_lst
 
 __author__ = "Jan Janssen, Liam Huber"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "development"
 __date__ = "Mar 24, 2019"
 
 
 class FlexibleMaster(GenericMaster):
-    """
+    __doc__ = (
+        """
     The FlexibleMaster uses a list of functions to connect multiple jobs in a series.
-
-    Args:
-        project (ProjectHDFio): ProjectHDFio instance which points to the HDF5 file the job is stored in
-        job_name (str): name of the job, which has to be unique within the project
-
-    Attributes:
-
-        .. attribute:: job_name
-
-            name of the job, which has to be unique within the project
-
-        .. attribute:: status
-
-            execution status of the job, can be one of the following [initialized, appended, created, submitted,
-                                                                      running, aborted, collect, suspended, refresh,
-                                                                      busy, finished]
-
-        .. attribute:: job_id
-
-            unique id to identify the job in the pyiron database
-
-        .. attribute:: parent_id
-
-            job id of the predecessor job - the job which was executed before the current one in the current job series
-
-        .. attribute:: master_id
-
-            job id of the master job - a meta job which groups a series of jobs, which are executed either in parallel
-            or in serial.
-
-        .. attribute:: child_ids
-
-            list of child job ids - only meta jobs have child jobs - jobs which list the meta job as their master
-
-        .. attribute:: project
-
-            Project instance the jobs is located in
-
-        .. attribute:: project_hdf5
-
-            ProjectHDFio instance which points to the HDF5 file the job is stored in
-
-        .. attribute:: job_info_str
-
-            short string to describe the job by it is job_name and job ID - mainly used for logging
-
-        .. attribute:: working_directory
-
-            working directory of the job is executed in - outside the HDF5 file
-
-        .. attribute:: path
-
-            path to the job as a combination of absolute file system path and path within the HDF5 file.
-
-        .. attribute:: version
-
-            Version of the hamiltonian, which is also the version of the executable unless a custom executable is used.
-
-        .. attribute:: executable
-
-            Executable used to run the job - usually the path to an external executable.
-
-        .. attribute:: library_activated
-
-            For job types which offer a Python library pyiron can use the python library instead of an external
-            executable.
-
-        .. attribute:: server
-
-            Server object to handle the execution environment for the job.
-
-        .. attribute:: queue_id
-
-            the ID returned from the queuing system - it is most likely not the same as the job ID.
-
-        .. attribute:: logger
-
-            logger object to monitor the external execution and internal pyiron warnings.
-
-        .. attribute:: restart_file_list
-
-            list of files which are used to restart the calculation from these files.
-
-        .. attribute:: job_type
-
-            Job type object with all the available job types: ['ExampleJob', 'SerialMaster', 'ParallelMaster',
-                                                               'ScriptJob', 'ListMaster']
-
-        .. attribute:: child_names
-
-            Dictionary matching the child ID to the child job name.
-    """
+"""
+        + "\n"
+        + _doc_str_job_core_args
+        + "\n"
+        + _doc_str_generic_master_attr
+    )
 
     def __init__(self, project, job_name):
         super(FlexibleMaster, self).__init__(project, job_name=job_name)
         self.__version__ = "0.1"
         self._step_function_lst = []
 
     @property
@@ -168,15 +84,17 @@
         max_steps = len(self.child_ids + self._job_name_lst)
         ind = max_steps - 1
         if self.check_all_childs_finished():
             for ind in range(len(self.child_ids), max_steps):
                 job = self.pop(0)
                 job._master_id = self.job_id
                 if ind != 0:
-                    prev_job = self[ind - 1]
+                    prev_job = self[
+                        self.project.db.get_item_by_id(self.child_ids[-1])["job"]
+                    ]
                     if ind < max_steps:
                         mod_funct = self._step_function_lst[ind - 1]
                         mod_funct(prev_job, job)
                     job._parent_id = prev_job.job_id
                 job.run()
                 if job.server.run_mode.interactive and not isinstance(
                     job, GenericMaster
@@ -184,15 +102,15 @@
                     job.interactive_close()
                 if self.server.run_mode.non_modal and job.server.run_mode.non_modal:
                     break
                 if job.server.run_mode.queue:
                     break
         if ind == max_steps - 1 and self.is_finished():
             self.status.finished = True
-            self.project.db.item_update(self._runtime(), self.job_id)
+            self.run_time_to_db()
         else:
             self.status.suspended = True
 
     def run_if_refresh(self):
         """
         Internal helper function the run if refresh function is called when the job status is 'refresh'. If the job was
         suspended previously, the job is going to be started again, to be continued.
@@ -210,20 +128,14 @@
             self.refresh_job_status()
             if self.status.refresh:
                 self.status.suspended = True
             if self.status.busy:
                 self.status.refresh = True
                 self.run_if_refresh()
 
-    def write_input(self):
-        """
-        write_input is not implemented for FlexibleMaster jobs
-        """
-        pass
-
     def collect_output(self):
         """
         Collect output is not implemented for FlexibleMaster jobs
         """
         pass
 
     def run_if_interactive(self):
@@ -261,20 +173,7 @@
         super(FlexibleMaster, self).from_hdf(hdf=hdf, group_name=group_name)
         with self.project_hdf5.open("input") as hdf5_input:
             if "funct_lst" in hdf5_input.list_nodes() and self._step_function_lst == []:
                 funct_str_lst = hdf5_input["funct_lst"]
                 for funct_str in funct_str_lst:
                     exec(funct_str)
                     self._step_function_lst.append(eval(funct_str.split("(")[0][4:]))
-
-    def __getitem__(self, item):
-        child_id_lst = self.child_ids
-        child_name_lst = [
-            self.project.db.get_item_by_id(child_id)["job"]
-            for child_id in self.child_ids
-        ]
-        if isinstance(item, int):
-            total_lst = child_name_lst + self._job_name_lst
-            item = total_lst[item]
-        return self._get_item_when_str(
-            item=item, child_id_lst=child_id_lst, child_name_lst=child_name_lst
-        )
```

### Comparing `pyiron_base-0.5.9/pyiron_base/master/generic.py` & `pyiron_base-0.6.0/pyiron_base/jobs/master/generic.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,145 +3,82 @@
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 The GenericMaster is the template class for all meta jobs
 """
 
 import inspect
 import textwrap
-from pyiron_base.job.generic import GenericJob
-from pyiron_base.job.jobstatus import job_status_finished_lst
+from functools import wraps
+from typing import Union
+
+from pyiron_base.storage.parameters import GenericParameters
+from pyiron_base.storage.datacontainer import DataContainer
+from pyiron_base.interfaces.object import HasStorage
+from pyiron_base.jobs.job.core import _doc_str_job_core_args
+from pyiron_base.jobs.job.generic import GenericJob, _doc_str_generic_job_attr
+from pyiron_base.jobs.job.extension.jobstatus import job_status_finished_lst
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 
-class GenericMaster(GenericJob):
-    """
-    The GenericMaster is the template class for all meta jobs - meaning all jobs which contain multiple other jobs. It
-    defines the shared functionality of the different kind of job series.
-
-    Args:
-        project (ProjectHDFio): ProjectHDFio instance which points to the HDF5 file the job is stored in
-        job_name (str): name of the job, which has to be unique within the project
-
-    Attributes:
-
-        .. attribute:: job_name
-
-            name of the job, which has to be unique within the project
-
-        .. attribute:: status
-
-            execution status of the job, can be one of the following [initialized, appended, created, submitted,
-                                                                      running, aborted, collect, suspended, refresh,
-                                                                      busy, finished]
-
-        .. attribute:: job_id
-
-            unique id to identify the job in the pyiron database
-
-        .. attribute:: parent_id
-
-            job id of the predecessor job - the job which was executed before the current one in the current job series
-
-        .. attribute:: master_id
-
-            job id of the master job - a meta job which groups a series of jobs, which are executed either in parallel
-            or in serial.
-
-        .. attribute:: child_ids
-
-            list of child job ids - only meta jobs have child jobs - jobs which list the meta job as their master
-
-        .. attribute:: project
-
-            Project instance the jobs is located in
-
-        .. attribute:: project_hdf5
-
-            ProjectHDFio instance which points to the HDF5 file the job is stored in
-
-        .. attribute:: job_info_str
-
-            short string to describe the job by it is job_name and job ID - mainly used for logging
-
-        .. attribute:: working_directory
-
-            working directory of the job is executed in - outside the HDF5 file
-
-        .. attribute:: path
-
-            path to the job as a combination of absolute file system path and path within the HDF5 file.
-
-        .. attribute:: version
-
-            Version of the hamiltonian, which is also the version of the executable unless a custom executable is used.
-
-        .. attribute:: executable
-
-            Executable used to run the job - usually the path to an external executable.
-
-        .. attribute:: library_activated
-
-            For job types which offer a Python library pyiron can use the python library instead of an external
-            executable.
-
-        .. attribute:: server
-
-            Server object to handle the execution environment for the job.
-
-        .. attribute:: queue_id
-
-            the ID returned from the queuing system - it is most likely not the same as the job ID.
-
-        .. attribute:: logger
-
-            logger object to monitor the external execution and internal pyiron warnings.
-
-        .. attribute:: restart_file_list
-
-            list of files which are used to restart the calculation from these files.
+# Modular Docstrings
+_doc_str_generic_master_attr = (
+    _doc_str_generic_job_attr
+    + "\n"
+    + """\
+        .. attribute:: child_names
 
-        .. attribute:: job_type
+            Dictionary matching the child ID to the child job name.
+"""
+)
 
-            Job type object with all the available job types: ['ExampleJob', 'SerialMaster', 'ParallelMaster',
-                                                               'ScriptJob', 'ListMaster']
 
-        .. attribute:: child_names
+class GenericMaster(GenericJob):
+    __doc__ = (
+        """
+    The GenericMaster is the template class for all meta jobs - meaning all jobs which contain multiple other jobs. It
+    defines the shared functionality of the different kind of job series.
 
-            Dictionary matching the child ID to the child job name.
-    """
+"""
+        + "\n"
+        + _doc_str_job_core_args
+        + "\n"
+        + _doc_str_generic_master_attr
+    )
 
     def __init__(self, project, job_name):
         super(GenericMaster, self).__init__(project, job_name=job_name)
+        self._input = GenericParameters("parameters")
         self._job_name_lst = []
         self._job_object_dict = {}
         self._child_id_func = None
         self._child_id_func_str = None
+        self._python_only_job = True
 
     @property
     def child_names(self):
         """
         Dictionary matching the child ID to the child job name
 
         Returns:
             dict: {child_id: child job name }
         """
-        child_dict = {}
-        for child_id in self.child_ids:
-            child_dict[child_id] = self.project.db.get_item_by_id(child_id)["job"]
-        return child_dict
+        return {
+            child_id: self.project.db.get_item_by_id(child_id)["job"]
+            for child_id in self.child_ids
+        }
 
     @property
     def child_ids(self):
         """
         list of child job ids - only meta jobs have child jobs - jobs which list the meta job as their master
 
         Returns:
@@ -158,14 +95,27 @@
         :class:`.Project`: project which holds the created child jobs
         """
         if not self.server.new_hdf:
             return self.project
         else:
             return self.project.open(self.job_name + "_hdf5")
 
+    @property
+    def input(self):
+        return self._input
+
+    @input.setter
+    def input(self, new_input: Union[DataContainer, GenericParameters, HasStorage]):
+        if isinstance(new_input, (DataContainer, GenericParameters, HasStorage)):
+            self._input = new_input
+        else:
+            raise TypeError(
+                f"Expected a DataContainer, GenericParameters or HasStorage object but got {new_input.__class__}"
+            )
+
     def child_hdf(self, job_name):
         """
         Find correct HDF for new children.  Depending on `self.server.new_hdf` this creates a new hdf file or creates
         the group in the file of this job.
 
         Args:
             job_name (str): name of the new job
@@ -187,14 +137,18 @@
         internal cache of currently loaded jobs
 
         Returns:
             dict: Dictionary of currently loaded jobs
         """
         return self._job_object_dict
 
+    @wraps(GenericJob.set_input_to_read_only)
+    def set_input_to_read_only(self):
+        self._input.read_only = True
+
     def first_child_name(self):
         """
         Get the name of the first child job
 
         Returns:
             str: name of the first child job
         """
@@ -231,18 +185,15 @@
         job_name_to_return = self._job_name_lst[i]
         job_to_return = self._load_all_child_jobs(
             self._load_job_from_cache(job_name_to_return)
         )
         del self._job_name_lst[i]
         with self.project_hdf5.open("input") as hdf5_input:
             hdf5_input["job_list"] = self._job_name_lst
-        job_to_return.project_hdf5.remove_group()
-        job_to_return.project_hdf5 = self.project_hdf5.__class__(
-            self.project, job_to_return.job_name, h5_path="/" + job_to_return.job_name
-        )
+        job_to_return.relocate_hdf5()
         if isinstance(job_to_return, GenericMaster):
             for sub_job in job_to_return._job_object_dict.values():
                 self._child_job_update_hdf(parent_job=job_to_return, child_job=sub_job)
         job_to_return.status.initialized = True
         return job_to_return
 
     def move_to(self, project):
@@ -292,14 +243,15 @@
 
         Args:
             hdf (ProjectHDFio): HDF5 group object - optional
             group_name (str): HDF5 subgroup name - optional
         """
         super(GenericMaster, self).to_hdf(hdf=hdf, group_name=group_name)
         with self.project_hdf5.open("input") as hdf5_input:
+            self.input.to_hdf(hdf5_input)
             hdf5_input["job_list"] = self._job_name_lst
             self._to_hdf_child_function(hdf=hdf5_input)
         for job in self._job_object_dict.values():
             job.to_hdf()
 
     def from_hdf(self, hdf=None, group_name=None):
         """
@@ -307,14 +259,15 @@
 
         Args:
             hdf (ProjectHDFio): HDF5 group object - optional
             group_name (str): HDF5 subgroup name - optional
         """
         super(GenericMaster, self).from_hdf(hdf=hdf, group_name=group_name)
         with self.project_hdf5.open("input") as hdf5_input:
+            self.input.from_hdf(hdf5_input)
             job_list_tmp = hdf5_input["job_list"]
             self._from_hdf_child_function(hdf=hdf5_input)
             self._job_name_lst = job_list_tmp
             self._job_object_dict = {
                 job_name: self._load_job_from_cache(job_name=job_name)
                 for job_name in job_list_tmp
             }
@@ -369,15 +322,16 @@
         """
         child_id_lst = self.child_ids
         child_name_lst = [
             self.project.db.get_item_by_id(child_id)["job"]
             for child_id in self.child_ids
         ]
         if isinstance(item, int):
-            item = self._job_name_lst[item]
+            total_lst = self._job_name_lst + child_name_lst
+            item = total_lst[item]
         return self._get_item_when_str(
             item=item, child_id_lst=child_id_lst, child_name_lst=child_name_lst
         )
 
     def __getattr__(self, item):
         """
         CHeck if a job with the specific name exists
```

### Comparing `pyiron_base-0.5.9/pyiron_base/master/list.py` & `pyiron_base-0.6.0/pyiron_base/jobs/master/serial.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,370 +1,387 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
-The ListMaster behaves like a list, just for job objects.
+The serial master class is a metajob consisting of a dynamic list of jobs which are executed in serial mode.
 """
 
-from pyiron_base.generic.parameters import GenericParameters
-from pyiron_base.job.core import JobCore
-from pyiron_base.job.generic import GenericJob
-from pyiron_base.master.generic import GenericMaster
-from pyiron_base.master.submissionstatus import SubmissionStatus
+from collections import OrderedDict
+import inspect
+import time
+import numpy as np
+from pyiron_base.jobs.job.core import _doc_str_job_core_args
+from pyiron_base.jobs.master.generic import (
+    GenericMaster,
+    get_function_from_string,
+    _doc_str_generic_master_attr,
+)
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 
-class ListMaster(GenericMaster):
-    """
-    The ListMaster is the most simple MetaJob derived from the GenericMaster. It behaves like a Python list object. Jobs
-    can be append to the ListMaster just like elements are added to a list and then all jobs can be executed together.
-    This also works for already executed jobs, unless they are already linked to a different MetaJob - meaning they
-    already have a master ID assigned to them.
-
-    Args:
-        project (ProjectHDFio): ProjectHDFio instance which points to the HDF5 file the job is stored in
-        job_name (str): name of the job, which has to be unique within the project
-
-    Attributes:
-
-        .. attribute:: job_name
-
-            name of the job, which has to be unique within the project
-
-        .. attribute:: status
-
-            execution status of the job, can be one of the following [initialized, appended, created, submitted,
-                                                                      running, aborted, collect, suspended, refresh,
-                                                                      busy, finished]
-
-        .. attribute:: job_id
-
-            unique id to identify the job in the pyiron database
-
-        .. attribute:: parent_id
-
-            job id of the predecessor job - the job which was executed before the current one in the current job series
-
-        .. attribute:: master_id
-
-            job id of the master job - a meta job which groups a series of jobs, which are executed either in parallel
-            or in serial.
-
-        .. attribute:: child_ids
-
-            list of child job ids - only meta jobs have child jobs - jobs which list the meta job as their master
-
-        .. attribute:: project
+# Modular Docstrings
+_doc_str_serial_master_base_attr = (
+    _doc_str_generic_master_attr
+    + "\n"
+    + """\
+        .. attribute:: start_job
 
-            Project instance the jobs is located in
+            The first job of the series.
 
-        .. attribute:: project_hdf5
+        .. attribute:: input
 
-            ProjectHDFio instance which points to the HDF5 file the job is stored in
-
-        .. attribute:: job_info_str
-
-            short string to describe the job by it is job_name and job ID - mainly used for logging
-
-        .. attribute:: working_directory
-
-            working directory of the job is executed in - outside the HDF5 file
-
-        .. attribute:: path
-
-            path to the job as a combination of absolute file system path and path within the HDF5 file.
-
-        .. attribute:: version
-
-            Version of the hamiltonian, which is also the version of the executable unless a custom executable is used.
-
-        .. attribute:: executable
-
-            Executable used to run the job - usually the path to an external executable.
-
-        .. attribute:: library_activated
-
-            For job types which offer a Python library pyiron can use the python library instead of an external
-            executable.
-
-        .. attribute:: server
-
-            Server object to handle the execution environment for the job.
+            The input of the start job - the first job of the series.
+"""
+)
 
-        .. attribute:: queue_id
 
-            the ID returned from the queuing system - it is most likely not the same as the job ID.
+class SerialMasterBase(GenericMaster):
+    __doc__ = (
+        """
+    The serial master class is a metajob consisting of a dynamic list of jobs which are executed in serial mode. The job
+    is derived from the GenericMaster.
+"""
+        + "\n"
+        + _doc_str_job_core_args
+        + "\n"
+        + _doc_str_serial_master_base_attr
+    )
 
-        .. attribute:: logger
+    def __init__(self, project, job_name):
+        super(SerialMasterBase, self).__init__(project, job_name=job_name)
+        self.__version__ = "0.3"
+        self._output = GenericOutput()
+        self._max_iterations = 100
+        self._start_job = None
+        self._convergence_goal = None
+        self._convergence_goal_qwargs = {}
+        self._convergence_goal_str = None
 
-            logger object to monitor the external execution and internal pyiron warnings.
+    @property
+    def start_job(self):
+        """
+        Get the first job of the series.
 
-        .. attribute:: restart_file_list
+        Returns:
+            GenericJob: start job
+        """
+        if self._start_job is not None:
+            return self._start_job
+        elif len(self) > 0:
+            self._start_job = self[-1]
+            return self._start_job
+        else:
+            return None
 
-            list of files which are used to restart the calculation from these files.
+    @start_job.setter
+    def start_job(self, job):
+        """
+        Set the first job of the series - that is the same like appending the job.
 
-        .. attribute:: job_type
+        Args:
+            job (GenericJob): start job
+        """
+        self.append(job)
 
-            Job type object with all the available job types: ['ExampleJob', 'SerialMaster', 'ParallelMaster',
-                                                               'ScriptJob', 'ListMaster']
+    @property
+    def ref_job(self):
+        return self.start_job
 
-        .. attribute:: child_names
+    @ref_job.setter
+    def ref_job(self, job):
+        self.append(job)
 
-            Dictionary matching the child ID to the child job name.
+    def get_initial_child_name(self):
+        """
+        Get name of the initial child.
 
-        .. attribute:: submission_status
+        Returns:
+            str: name of the initial child
+        """
+        return self.project.db.get_item_by_id(self.child_ids[0])["job"]
 
-            Monitors how many jobs have been submitted and how many have to be submitted in future.
-    """
+    def create_next(self, job_name=None):
+        """
+        Create the next job in the series by duplicating the previous job.
 
-    def __init__(self, project, job_name):
-        self._input = GenericParameters("parameters")
-        super(ListMaster, self).__init__(project, job_name=job_name)
-        self.__version__ = "0.1"
-        self._input["mode"] = "parallel"
-        self.submission_status = SubmissionStatus(db=project.db, job_id=self.job_id)
-        self.refresh_submission_status()
+        Args:
+            job_name (str): name of the new job - optional - default='job_<index>'
 
-    def set_input_to_read_only(self):
-        """
-        This function enforces read-only mode for the input classes, but it has to be implement in the individual
-        classes.
+        Returns:
+            GenericJob: next job
         """
-        self._input.read_only = True
+        if len(self) == 0:
+            raise ValueError("No job available in job list, please append a job first.")
+        if len(self._job_name_lst) > len(self.child_ids):
+            return self.pop(-1)
+        ham_old = self.project.load(self.child_ids[-1], convert_to_object=True)
+
+        if ham_old.status.aborted:
+            ham_old.status.created = True
+            return ham_old
+        elif not ham_old.status.finished:
+            return None
+        if job_name is None:
+            job_name = "_".join(
+                ham_old.job_name.split("_")[:-1] + [str(len(self.child_ids))]
+            )
+        new_job = ham_old.restart(job_name=job_name)
+        new_job.server.cores = self.server.cores
+        return new_job
 
-    def reset_job_id(self, job_id=None):
+    def collect_output(self):
         """
-        Reset the job id sets the job_id to None as well as all connected modules like JobStatus and SubmissionStatus.
+        Collect the output files of the individual jobs and set the output of the last job to be the output of the
+        SerialMaster - so the SerialMaster contains the same output as its last child.
         """
-        super(ListMaster, self).reset_job_id(job_id=job_id)
-        self.submission_status = SubmissionStatus(db=self.project.db, job_id=job_id)
+        ham_lst = [self.project_hdf5.inspect(child_id) for child_id in self.child_ids]
+        if (
+            "output" in ham_lst[0].list_groups()
+            and "generic" in ham_lst[0]["output"].list_groups()
+        ):
+            nodes = ham_lst[0]["output/generic"].list_nodes()
+            with self.project_hdf5.open("output/generic") as hh:
+                for node in nodes:
+                    if ham_lst[0]["output/generic/{}".format(node)] is not None:
+                        hh[node] = np.concatenate(
+                            [ham["output/generic/{}".format(node)] for ham in ham_lst],
+                            axis=0,
+                        )
+                    else:
+                        hh[node] = None
 
-    def refresh_submission_status(self):
+    def collect_logfiles(self):
         """
-        Refresh the submission status - if a job ID job_id is set then the submission status is loaded from the
-        database.
+        The collect logfiles function is required by the GenericJob class, therefore we use an empty template here.
         """
-        if self.job_id:
-            self.submission_status = SubmissionStatus(
-                db=self._hdf5.db, job_id=self.job_id
-            )
-            self.submission_status.refresh()
+        pass
 
-    def save(self):
+    def copy(self):
         """
-        Save the object, by writing the content to the HDF5 file and storing an entry in the database.
+        Copy the GenericJob object which links to the job and its HDF5 file
 
         Returns:
-            (int): Job ID stored in the database
+            GenericJob: New GenericJob object pointing to the same job
         """
-        job_id = super(ListMaster, self).save()
-        self.refresh_submission_status()
-        return job_id
+        new_job = super(SerialMasterBase, self).copy()
+        new_job.start_job = self.start_job
+        return new_job
 
-    def append(self, job):
+    def from_hdf(self, hdf=None, group_name=None):
         """
-        Append a job to the ListMaster - just like you would append an element to a list.
+        Restore the SerialMaster from an HDF5 file
 
         Args:
-            job (JobCore, GenericJob, int): job to append
+            hdf (ProjectHDFio): HDF5 group object - optional
+            group_name (str): HDF5 subgroup name - optional
         """
-        if isinstance(job, JobCore) and job.job_id:
-            job = job.job_id
-        if isinstance(job, int):
-            job = self._hdf5.project.load(job)
-        if isinstance(job, GenericJob):
-            if job.status.created or job.status.initialized:
-                super(ListMaster, self).append(job=job)
-            elif job.job_id and job.status.finished:
-                if job.master_id is None:
-                    if self.job_id is None:
-                        self._job_id = self.save()
-                    child_db_entry = self.project.db.get_item_by_id(job.job_id)
-                    self.project.db.delete_item(job.job_id)
-                    job._job_id = None
-                    job.master_id = self._job_id
-                    job.save()
-                    del child_db_entry["id"]
-                    del child_db_entry["masterid"]
-                    self.project.db.item_update(child_db_entry, job.job_id)
-                    self.submission_status.submit_next()
-                    if len(self._job_name_lst) == 0:
-                        self.status.finished = True
-                        self.project.db.item_update(self._runtime(), self.job_id)
-                else:
-                    raise ValueError(
-                        "This job ",
-                        job.job_name,
-                        " is already connected to a master ",
-                        job.master_id,
-                        " and can not be appended here.",
-                    )
-        else:
-            raise TypeError(
-                "job has to be either GenericJob, JobCore or int, but it - ",
-                job,
-                " is ",
-                type(job),
-            )
+        super(SerialMasterBase, self).from_hdf(hdf=hdf, group_name=group_name)
+        with self.project_hdf5.open("input") as hdf5_input:
+            convergence_goal_str = hdf5_input["convergence_goal"]
+            if convergence_goal_str == "None":
+                self._convergence_goal = None
+            else:
+                self._convergence_goal_str = convergence_goal_str
+                self._convergence_goal = get_function_from_string(convergence_goal_str)
+                self._convergence_goal_qwargs = hdf5_input["convergence_goal_qwargs"]
 
-    def is_finished(self):
+    def get_from_childs(self, path):
         """
-        Check if the ListMaster job is finished - by checking the job status and the submission status.
+        Extract the output from all child jobs and appending it to a list
+
+        Args:
+            path (str): path inside the HDF5 files of the individual jobs like 'output/generic/volume'
 
         Returns:
-            bool: [True/False]
+            list: list of output from the child jobs
         """
-        if self.status.finished:
-            return True
-        # self.status.busy = True
-        self.submission_status.refresh()
-        if not self.submission_status.finished:
-            return False
-        else:
-            status_set = set(
-                [
-                    self._hdf5.db.get_item_by_id(child_id)["status"]
-                    for child_id in self.child_ids
-                ]
-            )
-            # status_set = set([job.get_status() for job in self.iter_jobs(convert_to_object=False)])
-            if "finished" in status_set:
-                return len(status_set) == 1
-            else:
-                return False
+        var_lst = []
+        for child_id in self.child_ids:
+            ham = self.project.load(child_id, convert_to_object=False)
+            var = ham.__getitem__(path)
+            var_lst.append(var)
+        return np.array(var_lst)
 
-    def run_static(self):
+    def iter_jobs(self, convert_to_object=True):
         """
-        The run static function is called by run to execute the simulation. For the
-        ListMaster this means executing all the childs appened in parallel.
+        Iterate over the jobs within the SerialMaster
+
+        Args:
+            convert_to_object (bool): load the full GenericJob object (default) or just the HDF5 / JobCore object
+
+        Returns:
+            yield: Yield of GenericJob or JobCore
         """
-        self._input["num_points"] = len(self)
-        self._logger.info("{} run parallel master (modal)".format(self.job_info_str))
+        for job_id in self.child_ids:
+            yield self.project.load(job_id, convert_to_object=convert_to_object)
+
+    def run_if_interactive(self):
+        pass
+
+    def _get_job_template(self):
+        self._logger.info("run serial master {}".format(self.job_info_str))
+        job = self.pop(-1)
+        job._master_id = self.job_id
+        job._hdf5 = self.child_hdf(job.job_name)
+        self._logger.info("SerialMaster: run job {}".format(job.job_name))
+        return job
+
+    @staticmethod
+    def _run_child_job(job):
+        job.run()
+
+    def _run_if_master_queue(self, job):
+        job.server.run_mode.modal = True
+        job.run()
+        self.run_if_refresh()
+
+    def _run_if_master_non_modal_child_non_modal(self, job):
+        job.run()
+        if self.master_id is not None:
+            del self
+
+    def _run_if_master_modal_child_modal(self, job):
+        job.run()
+        self.run_if_refresh()
+
+    def _run_if_master_modal_child_non_modal(self, job):
+        job.run()
+        while not job.status.finished and not job.status.aborted:
+            job.refresh_job_status()
+            time.sleep(5)
+        self.run_if_refresh()
+
+    def run_static(self, **qwargs):
         self.status.running = True
-        if len(self._job_name_lst) > 0:
-            job_lst = []
-            for i in range(len(self._job_name_lst)):
-                ham = self.pop(i=0)
-                if (
-                    ham.server.run_mode.non_modal
-                    and self.get_child_cores() + ham.server.cores > self.server.cores
-                ):
-                    break
-                self.submission_status.submit_next()
-                if not ham.status.finished:
-                    ham.run()
-                self._logger.info("ListMaster: finished job {}".format(ham.job_name))
-                if ham.server.run_mode.thread:
-                    job_lst.append(ham._process)
-                else:
-                    self.refresh_job_status()
-            _ = [process.communicate() for process in job_lst if process]
+        if len(self) > len(self.child_ids):
+            job = self._get_job_template()
             self.status.suspended = True
-        if self.server.run_mode.modal or (
-            (self.server.run_mode.non_modal or self.server.run_mode.queue)
-            and self.is_finished()
-        ):
-            self.status.finished = True
+            if self.server.run_mode.queue:
+                self._run_if_master_queue(job)
+            elif self.server.run_mode.non_modal and job.server.run_mode.non_modal:
+                self._run_if_master_non_modal_child_non_modal(job)
+            elif self.server.run_mode.modal and job.server.run_mode.modal:
+                self._run_if_master_modal_child_modal(job)
+            elif self.server.run_mode.modal and job.server.run_mode.non_modal:
+                self._run_if_master_modal_child_non_modal(job)
+            else:
+                raise TypeError()
+        else:
+            self.status.collect = True
+            self.run()
 
-    def write_input(self):
+    def set_goal(self, convergence_goal, **qwargs):
         """
-        Write the input files - for the ListMaster this only contains the execution mode, which is 'parallel' by
-        default.
-        """
-        self._input.write_file(file_name="input.inp", cwd=self.working_directory)
+        Set a convergence goal for the SerialMaster - this is necessary to stop the series.
 
-    def copy(self):
+        Args:
+            convergence_goal (Function): the convergence goal can be any Python function, but if external packages are
+                                         used like numpy they have to be imported within the function.
+            **qwargs: arguments of the convergence goal function.
+        """
+        self._convergence_goal = convergence_goal
+        self._convergence_goal_qwargs = qwargs
+        self._convergence_goal_str = inspect.getsource(convergence_goal)
+        if self.project_hdf5.file_exists:
+            self.to_hdf()
+
+    def show(self):
         """
-        Copy the ListMaster object which links to the job and its HDF5 file
+        list all jobs in the SerialMaster
 
         Returns:
-            ListMaster: New ListMaster object pointing to the same job
+            list: list of jobs ['job', <index>, <GenericJob>]
         """
-        new_job = super(ListMaster, self).copy()
-        new_job._child_ids = self.child_ids[:]
-        return new_job
+        return [["job", str(i), str(job)] for i, job in enumerate(self)]
 
-    def iter_jobs(self, convert_to_object=True):
+    def to_hdf(self, hdf=None, group_name=None):
         """
-        Iterate over the jobs within the ListMaster
+        Store the SerialMaster in an HDF5 file
 
         Args:
-            convert_to_object (bool): load the full GenericJob object (default) or just the HDF5 / JobCore object
+            hdf (ProjectHDFio): HDF5 group object - optional
+            group_name (str): HDF5 subgroup name - optional
+        """
+        super(SerialMasterBase, self).to_hdf(hdf=hdf, group_name=group_name)
+        with self.project_hdf5.open("input") as hdf5_input:
+            if self._convergence_goal is not None:
+                try:
+                    hdf5_input["convergence_goal"] = inspect.getsource(
+                        self._convergence_goal
+                    )
+                except IOError:
+                    hdf5_input["convergence_goal"] = self._convergence_goal_str
+
+                hdf5_input["convergence_goal_qwargs"] = self._convergence_goal_qwargs
+            else:
+                hdf5_input["convergence_goal"] = "None"
+
+    def __len__(self):
+        """
+        Length of the SerialMaster equal the number of childs appended.
 
         Returns:
-            yield: Yield of GenericJob or JobCore
+            int: length of the SerialMaster
         """
-        for job_id in self.child_ids:
-            yield self._hdf5.load(job_id, convert_to_object=convert_to_object)
+        return len(self.child_ids + self._job_name_lst)
 
     def run_if_refresh(self):
         """
         Internal helper function the run if refresh function is called when the job status is 'refresh'. If the job was
         suspended previously, the job is going to be started again, to be continued.
         """
-        self._logger.info(
-            "{}, status: {}, finished: {} parallel master "
-            "refresh".format(self.job_info_str, self.status, self.is_finished())
-        )
-        if self.is_finished() and not self.server.run_mode.modal:
-            self.status.finished = True
-        elif (
-            self.server.run_mode.non_modal or self.server.run_mode.queue
-        ) and not self.submission_status.finished:
-            self.run_static()
+        conv_goal_exists = bool(self._convergence_goal)
+        self._logger.info("Does the convergence goal exit: {}".format(conv_goal_exists))
+        if not conv_goal_exists:
+            self.status.collect = True
+            self.run()
         else:
-            self.refresh_job_status()
-            if self.status.refresh:
-                self.status.suspended = True
-
-    def collect_output(self):
-        """
-        Collect output is not implemented for ListMaster jobs
-        """
-        pass
-
-    def run_if_interactive(self):
-        """
-        run_if_interactive() is not implemented for ListMaster jobs
-        """
-        pass
+            subjobs_statuses = set(
+                [
+                    self.project.db.get_job_status(job_id=child_id)
+                    for child_id in self.child_ids
+                ]
+            )
+            if len(subjobs_statuses) == 0 or subjobs_statuses == {"finished"}:
+                ham = self._convergence_goal(self, **self._convergence_goal_qwargs)
+                if ham is not True:
+                    self.append(ham)
+                    self.to_hdf()
+                    self.run_static()
+                else:
+                    self.status.collect = True
+                    self.run()
 
-    def __getitem__(self, item):
+    def _init_child_job(self, parent):
         """
-        Get/ read data from the HDF5 file
+        Update our reference job and copy their run mode.
 
         Args:
-            item (str, slice): path to the data or key of the data object
-
-        Returns:
-            dict, list, float, int: data or data object
+            parent (:class:`.GenericJob`): job instance that this job was created from
         """
-        child_id_lst = self.child_ids
-        child_name_lst = [
-            self.project.db.get_item_by_id(child_id)["job"]
-            for child_id in self.child_ids
-        ]
-        if isinstance(item, int):
-            total_lst = child_name_lst + self._job_name_lst
-            item = total_lst[item]
-        return self._get_item_when_str(
-            item=item, child_id_lst=child_id_lst, child_name_lst=child_name_lst
-        )
+        super()._init_child_job(parent)
+        if parent.server.run_mode.non_modal:
+            self.server.run_mode.non_modal = True
+        elif (
+            parent.server.run_mode.interactive
+            or parent.server.run_mode.interactive_non_modal
+        ):
+            self.server.run_mode.interactive = True
 
-    def __len__(self):
-        """
-        Length of the ListMaster equal the number of childs appended.
 
-        Returns:
-            int: length of the ListMaster
-        """
-        return len(self.child_ids + self._job_name_lst)
+class GenericOutput(OrderedDict):
+    """
+    Generic Output just a place holder to store the output of the last child directly in the SerialMaster.
+    """
+
+    def __init__(self):
+        super(GenericOutput, self).__init__()
```

### Comparing `pyiron_base-0.5.9/pyiron_base/master/parallel.py` & `pyiron_base-0.6.0/pyiron_base/jobs/master/parallel.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,149 +3,72 @@
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 The parallel master class is a metajob consisting of a list of jobs which are executed in parallel.
 """
 
 from collections import OrderedDict
 from datetime import datetime
+
 import numpy as np
 import pandas
 import multiprocessing
 import importlib
-from pyiron_base.job.generic import GenericJob
-from pyiron_base.master.generic import GenericMaster
-from pyiron_base.master.submissionstatus import SubmissionStatus
-from pyiron_base.generic.parameters import GenericParameters
-from pyiron_base.job.jobstatus import JobStatus
+from pyiron_base.jobs.job.generic import GenericJob
+from pyiron_base.jobs.job.core import _doc_str_job_core_args
+from pyiron_base.jobs.master.generic import GenericMaster, _doc_str_generic_master_attr
+from pyiron_base.jobs.master.submissionstatus import SubmissionStatus
+from pyiron_base.jobs.job.extension.jobstatus import JobStatus
 from pyiron_base.state import state
-from pyiron_base.job.wrapper import job_wrapper_function
-from pyiron_base.generic.util import deprecate
+from pyiron_base.jobs.job.wrapper import job_wrapper_function
+from pyiron_base.utils.deprecate import deprecate
 
 __author__ = "Joerg Neugebauer, Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 
-class ParallelMaster(GenericMaster):
-    """
-    MasterJob that handles the creation and analysis of several parallel jobs (including master and
-    continuation jobs), Examples are Murnaghan or Phonon calculations.
-
-    Subclasses *must* implement :meth:`.collect_output()`.  Additionally :attr:`._job_generator` must be
-    initialized with an instance of :class:`.JobGenerator` in the subclasses' `__init__`.
-
-    Args:
-        project (ProjectHDFio): ProjectHDFio instance which points to the HDF5 file the job is stored in
-        job_name (str): name of the job, which has to be unique within the project
-
-    Attributes:
-
-        .. attribute:: job_name
-
-            name of the job, which has to be unique within the project
-
-        .. attribute:: status
-
-            execution status of the job, can be one of the following [initialized, appended, created, submitted,
-                                                                      running, aborted, collect, suspended, refresh,
-                                                                      busy, finished]
-
-        .. attribute:: job_id
-
-            unique id to identify the job in the pyiron database
-
-        .. attribute:: parent_id
-
-            job id of the predecessor job - the job which was executed before the current one in the current job series
-
-        .. attribute:: master_id
-
-            job id of the master job - a meta job which groups a series of jobs, which are executed either in parallel
-            or in serial.
-
-        .. attribute:: child_ids
-
-            list of child job ids - only meta jobs have child jobs - jobs which list the meta job as their master
-
-        .. attribute:: project
-
-            Project instance the jobs is located in
-
-        .. attribute:: project_hdf5
-
-            ProjectHDFio instance which points to the HDF5 file the job is stored in
-
-        .. attribute:: job_info_str
-
-            short string to describe the job by it is job_name and job ID - mainly used for logging
-
-        .. attribute:: working_directory
-
-            working directory of the job is executed in - outside the HDF5 file
-
-        .. attribute:: path
-
-            path to the job as a combination of absolute file system path and path within the HDF5 file.
-
-        .. attribute:: version
-
-            Version of the hamiltonian, which is also the version of the executable unless a custom executable is used.
-
-        .. attribute:: executable
-
-            Executable used to run the job - usually the path to an external executable.
-
-        .. attribute:: library_activated
-
-            For job types which offer a Python library pyiron can use the python library instead of an external
-            executable.
-
-        .. attribute:: server
-
-            Server object to handle the execution environment for the job.
-
-        .. attribute:: queue_id
-
-            the ID returned from the queuing system - it is most likely not the same as the job ID.
-
-        .. attribute:: logger
-
-            logger object to monitor the external execution and internal pyiron warnings.
-
-        .. attribute:: restart_file_list
-
-            list of files which are used to restart the calculation from these files.
-
-        .. attribute:: job_type
-
-            Job type object with all the available job types: ['ExampleJob', 'SerialMaster', 'ParallelMaster',
-                                                               'ScriptJob', 'ListMaster']
-
-        .. attribute:: child_names
-
-            Dictionary matching the child ID to the child job name.
-
+# Modular Docstrings
+_doc_str_parallel_master_attr = (
+    _doc_str_generic_master_attr
+    + "\n"
+    + """\
         .. attribute:: ref_job
 
             Reference job template from which all jobs within the ParallelMaster are generated.
 
         .. attribute:: number_jobs_total
 
             Total number of jobs
-    """
+"""
+)
+
+
+class ParallelMaster(GenericMaster):
+    __doc__ = (
+        """
+    MasterJob that handles the creation and analysis of several parallel jobs (including master and
+    continuation jobs), Examples are Murnaghan or Phonon calculations.
+
+    Subclasses *must* implement :meth:`.collect_output()`.  Additionally :attr:`._job_generator` must be
+    initialized with an instance of :class:`.JobGenerator` in the subclasses' `__init__`.
+"""
+        + "\n"
+        + _doc_str_job_core_args
+        + "\n"
+        + _doc_str_parallel_master_attr
+    )
 
     def __init__(self, project, job_name):
-        self.input = GenericParameters("parameters")
         super(ParallelMaster, self).__init__(project, job_name=job_name)
         self.__version__ = "0.3"
         self._ref_job = None
         self._output = GenericOutput()
         self._job_generator = None
         self.submission_status = SubmissionStatus(db=project.db, job_id=self.job_id)
         self.refresh_submission_status()
@@ -198,65 +121,26 @@
         Set number of total jobs (optional: default = None)
 
         Args:
             num_jobs (int): number of submitted jobs
         """
         self.submission_status.total_jobs = num_jobs
 
-    def set_input_to_read_only(self):
-        """
-        This function enforces read-only mode for the input classes, but it has to be implement in the individual
-        classes.
-        """
-        self.input.read_only = True
-
     def reset_job_id(self, job_id=None):
         """
         Reset the job id sets the job_id to None as well as all connected modules like JobStatus and SubmissionStatus.
         """
         super(ParallelMaster, self).reset_job_id(job_id=job_id)
         if job_id is not None:
             self.submission_status = SubmissionStatus(db=self.project.db, job_id=job_id)
         else:
             self.submission_status = SubmissionStatus(
                 db=self.project.db, job_id=self.job_id
             )
 
-    def to_hdf(self, hdf=None, group_name=None):
-        """
-        Store the ParallelMaster in an HDF5 file
-
-        Args:
-            hdf (ProjectHDFio): HDF5 group object - optional
-            group_name (str): HDF5 subgroup name - optional
-        """
-        super(ParallelMaster, self).to_hdf(hdf=hdf, group_name=group_name)
-        with self.project_hdf5.open("input") as hdf5_input:
-            self.input.to_hdf(hdf5_input)
-
-    def from_hdf(self, hdf=None, group_name=None):
-        """
-        Restore the ParallelMaster from an HDF5 file
-
-        Args:
-            hdf (ProjectHDFio): HDF5 group object - optional
-            group_name (str): HDF5 subgroup name - optional
-        """
-        super(ParallelMaster, self).from_hdf(hdf=hdf, group_name=group_name)
-        with self.project_hdf5.open("input") as hdf5_input:
-            self.input.from_hdf(hdf5_input)
-
-    def write_input(self):
-        """
-        Write the input files - this contains the GenericInput of the ParallelMaster as well as reseting the submission
-        status.
-        """
-        self.submission_status.submitted_jobs = 0
-        self.input.write_file(file_name="input.inp", cwd=self.working_directory)
-
     def collect_output(self):
         """
         Collect the output files of the external executable and store the information in the HDF5 file. This method has
         to be implemented in the individual meta jobs derived from the ParallelMaster.
         """
         raise NotImplementedError("Implement in derived class")
 
@@ -335,15 +219,17 @@
 
     def interactive_ref_job_initialize(self):
         """
         To execute the reference job in interactive mode it is necessary to initialize it.
         """
         if len(self._job_name_lst) > 0:
             self._ref_job = self.pop(-1)
-            self._ref_job.job_name = self.job_name + "_" + self._ref_job.job_name
+            job_name = self.job_name + "_" + self._ref_job.job_name
+            self._ref_job.job_name = job_name
+            self._ref_job.project_hdf5 = self.child_hdf(job_name)
             if self._job_id is not None and self._ref_job._master_id is None:
                 self._ref_job.master_id = self.job_id
 
     def copy(self):
         """
         Copy the GenericJob object which links to the job and its HDF5 file
 
@@ -399,36 +285,14 @@
             for j in [
                 self._job_generator.job_name(p)
                 for p in self._job_generator.parameter_list
             ]
             if j in job_names
         ]
 
-    def __getitem__(self, item):
-        """
-        Get/ read data from the HDF5 file
-
-        Args:
-            item (str, slice): path to the data or key of the data object
-
-        Returns:
-            dict, list, float, int: data or data object
-        """
-        child_id_lst = self.child_ids
-        child_name_lst = [
-            self.project.db.get_item_by_id(child_id)["job"]
-            for child_id in self.child_ids
-        ]
-        if isinstance(item, int):
-            total_lst = self._job_name_lst + child_name_lst
-            item = total_lst[item]
-        return self._get_item_when_str(
-            item=item, child_id_lst=child_id_lst, child_name_lst=child_name_lst
-        )
-
     def __len__(self):
         """
         Length of the ListMaster equal the number of childs appended.
 
         Returns:
             int: length of the ListMaster
         """
@@ -471,22 +335,49 @@
 
         job_id = self.get_job_id()
         db_dict = {}
         start_time = self.project.db.get_item_by_id(job_id)["timestart"]
         db_dict["timestop"] = datetime.now()
         db_dict["totalcputime"] = (db_dict["timestop"] - start_time).seconds
         self.project.db.item_update(db_dict, job_id)
-        self.status.finished = True
+        if not self.convergence_check():
+            self.status.not_converged = True
+        else:
+            self.status.finished = True
         self._hdf5["status"] = self.status.string
         self._logger.info(
             "{}, status: {}, parallel master".format(self.job_info_str, self.status)
         )
         self.update_master()
         # self.send_to_database()
 
+    def _run_if_new(self, debug=False):
+        """
+        Internal helper function the run if new function is called when the job status is 'initialized'. It prepares
+        the hdf5 file and the corresponding directory structure.
+
+        Args:
+            debug (bool): Debug Mode
+        """
+        self.submission_status.submitted_jobs = 0
+        super()._run_if_new(debug=debug)
+
+    def convergence_check(self) -> bool:
+        """
+        Check if and all child jobs of the calculation are converged. May need be extended in the base classes depending
+        on the specific application
+
+        Returns:
+             (bool): If the calculation is converged
+        """
+        for job in self.iter_jobs(convert_to_object=False):
+            if job.status not in ["finished", "warning"]:
+                return False
+        return True
+
     def _validate_cores(self, job, cores_for_session):
         """
         Check if enough cores are available to start the next child job.
 
         Args:
             job (GenericJob): child job to be started
             cores_for_session (list): list of currently active cores - list of integers
```

### Comparing `pyiron_base-0.5.9/pyiron_base/master/submissionstatus.py` & `pyiron_base-0.6.0/pyiron_base/jobs/master/submissionstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.9/pyiron_base/project/data.py` & `pyiron_base-0.6.0/pyiron_base/project/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
     - Data storage is immediately accessible, i.e. appearing in the project tab-completion module
     - Data stored there should be readable and writeable with a single parameter-free call
     - When instantiated, new projects should automatically read any available data (not *quite* satisfied right now!)
     - The `Project` tab completion menu should not get cluttered (i.e. nest everything under `Project.foo`)
 """
 
-from pyiron_base.generic.datacontainer import DataContainer
-from pyiron_base.generic.hdfio import ProjectHDFio
+from pyiron_base.storage.datacontainer import DataContainer
+from pyiron_base.storage.hdfio import ProjectHDFio
 
 __author__ = "Liam Huber"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "0.1"
@@ -32,22 +32,22 @@
 
 class ProjectData(DataContainer):
     def __new__(cls, *args, **kwargs):
         instance = super().__new__(cls, *args, **kwargs)
         object.__setattr__(instance, "_project", None)
         return instance
 
-    def __init__(self, *args, project=None, **kwargs):
+    def __init__(self, *args, project=None, lazy=True, **kwargs):
         """
         A data storage container which can store itself to/retrieve itself from file at the project level.
 
         Args:
             project (pyiron_base.Project): The project instance the storage is attached to.
         """
-        super().__init__(*args, **kwargs)
+        super().__init__(*args, lazy=lazy, **kwargs)
         self._project = project
 
     def read(self):
         """Read existing data from project-level storage."""
         hdf = ProjectHDFio(self._project, file_name="project_data")
         if self.table_name not in hdf.list_groups():
             raise KeyError(
```

### Comparing `pyiron_base-0.5.9/pyiron_base/project/generic.py` & `pyiron_base-0.6.0/pyiron_base/project/generic.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 """
 The project object is the central import point of pyiron - all other objects can be created from this one
 """
 
 import os
 import posixpath
 import shutil
+import stat
 from tqdm.auto import tqdm
 import pandas
 import pint
-import importlib
 import math
 import numpy as np
 
 from pyiron_base.project.maintenance import Maintenance
 from pyiron_base.project.path import ProjectPath
 from pyiron_base.database.filetable import FileTable
 from pyiron_base.state import state
@@ -24,33 +24,33 @@
     get_job_id,
     get_jobs,
     set_job_status,
     get_child_ids,
     get_job_working_directory,
     get_job_status,
 )
-from pyiron_base.generic.hdfio import ProjectHDFio
-from pyiron_base.generic.filedata import load_file
-from pyiron_base.generic.util import deprecate
-from pyiron_base.job.util import _special_symbol_replacements, _get_safe_job_name
+from pyiron_base.storage.hdfio import ProjectHDFio
+from pyiron_base.storage.filedata import load_file
+from pyiron_base.utils.deprecate import deprecate
+from pyiron_base.jobs.job.util import _special_symbol_replacements, _get_safe_job_name
 from pyiron_base.interfaces.has_groups import HasGroups
-from pyiron_base.job.jobtype import JobType, JobTypeChoice, JobFactory
-from pyiron_base.server.queuestatus import (
+from pyiron_base.jobs.job.jobtype import JobType, JobTypeChoice, JobFactory
+from pyiron_base.jobs.job.extension.server.queuestatus import (
     queue_delete_job,
     queue_is_empty,
     queue_table,
     wait_for_job,
     wait_for_jobs,
     update_from_remote,
     queue_enable_reservation,
     queue_check_job_is_waiting_or_running,
 )
-from pyiron_base.job.external import Notebook
+from pyiron_base.project.external import Notebook
 from pyiron_base.project.data import ProjectData
-from pyiron_base.archiving import import_archive, export_archive
+from pyiron_base.project.archiving import export_archive, import_archive
 from typing import Generator, Union, Dict
 
 __author__ = "Joerg Neugebauer, Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -132,15 +132,15 @@
         return state
 
     @property
     def db(self):
         if not state.database.database_is_disabled:
             return state.database.database
         else:
-            return FileTable(project=self.path)
+            return FileTable(index_from=self.path)
 
     @property
     def maintenance(self):
         if self._maintenance is None:
             self._maintenance = Maintenance(self)
         return self._maintenance
 
@@ -252,23 +252,25 @@
 
         Returns:
             Project: pointing to the new project path
         """
         if not self.view_mode:
             if not isinstance(destination, Project):
                 raise TypeError("A project can only be copied to another project.")
-            for sub_project_name in self.list_groups():
+            for sub_project_name in tqdm(
+                self.list_groups(), desc="Copying sub-projects"
+            ):
                 if "_hdf5" not in sub_project_name:
                     sub_project = self.open(sub_project_name)
                     destination_sub_project = destination.open(sub_project_name)
                     sub_project.copy_to(destination_sub_project)
-            for job_id in self.get_job_ids(recursive=False):
+            for job_id in tqdm(self.get_job_ids(recursive=False), desc="Copying jobs"):
                 ham = self.load(job_id)
                 ham.copy_to(project=destination)
-            for file in self.list_files():
+            for file in tqdm(self.list_files(), desc="Copying files"):
                 if ".h5" not in file:
                     shutil.copy(os.path.join(self.path, file), destination.path)
             return destination
         else:
             raise EnvironmentError("copy_to: is not available in Viewermode !")
 
     def create_from_job(self, job_old, new_job_name):
@@ -557,24 +559,31 @@
         progress: bool = True,
         **kwargs: dict,
     ) -> Generator:
         """
         Iterate over the jobs within the current project and it is sub projects
 
         Args:
-            path (str): HDF5 path inside each job object
-            recursive (bool): search subprojects [True/False] - True by default
-            convert_to_object (bool): load the full GenericJob object (default) or just the HDF5 / JobCore object
-            progress (bool): if True (default), add an interactive progress bar to the iteration
+            path (str): HDF5 path inside each job object. (Default is None, which just uses the top level of the job's
+                HDF5 path.)
+            recursive (bool): search subprojects. (Default is True.)
+            convert_to_object (bool): load the full GenericJob object, else just return the HDF5 / JobCore object.
+                                     (Default is True, convert everything to the full python object.)
+            progress (bool): add an interactive progress bar to the iteration. (Default is True, show the bar.)
             **kwargs (dict): Optional arguments for filtering with keys matching the project database column name
                             (eg. status="finished"). Asterisk can be used to denote a wildcard, for zero or more
                             instances of any character
 
         Returns:
             yield: Yield of GenericJob or JobCore
+
+        Note:
+            The default behavior of converting to object can cause **significant** slowdown in larger projects. In this
+            case, you may seriously wish to consider setting `convert_to_object=False` and access only the HDF5/JobCore
+            representation of the jobs instead.
         """
         job_id_lst = self.job_table(recursive=recursive, **kwargs)["id"]
         if progress:
             job_id_lst = tqdm(job_id_lst)
         for job_id in job_id_lst:
             if path is not None:
                 yield self.load(job_id, convert_to_object=False)[path]
@@ -616,54 +625,94 @@
         All items in the current project - this includes jobs, sub projects/ groups/ folders and any kind of files
 
         Returns:
             list: items in the project
         """
         return [(key, self[key]) for key in self.keys()]
 
-    def update_from_remote(self, recursive=True, ignore_exceptions=False):
+    def update_from_remote(
+        self, recursive=True, ignore_exceptions=False, try_collecting=False
+    ):
         """
         Update jobs from the remote server
 
         Args:
             recursive (bool): search subprojects [True/False] - default=True
             ignore_exceptions (bool): ignore eventual exceptions when retrieving jobs - default=False
 
         Returns:
             returns None if ignore_exceptions is False or when no error occured.
             returns a list with job ids when errors occured, but were ignored
 
         """
         return update_from_remote(
-            project=self, recursive=recursive, ignore_exceptions=ignore_exceptions
+            project=self,
+            recursive=recursive,
+            ignore_exceptions=ignore_exceptions,
+            try_collecting=try_collecting,
         )
 
     def job_table(
         self,
         recursive=True,
         columns=None,
         all_columns=True,
         sort_by="id",
         full_table=False,
         element_lst=None,
         job_name_contains="",
+        auto_refresh_job_status=False,
         **kwargs: dict,
     ):
-        return self.db.job_table(
-            sql_query=self.sql_query,
-            user=self.user,
-            project_path=self.project_path,
-            recursive=recursive,
-            columns=columns,
-            all_columns=all_columns,
-            sort_by=sort_by,
-            full_table=full_table,
-            element_lst=element_lst,
-            **kwargs,
-        )
+        """
+        auto_refresh_job_status (bool): will automatically reload job status by calling refresh_job_status() upon calling job_table
+        """
+        if not isinstance(self.db, FileTable):
+            if auto_refresh_job_status:
+                self.refresh_job_status()
+            return self.db.job_table(
+                sql_query=self.sql_query,
+                user=self.user,
+                project_path=self.project_path,
+                recursive=recursive,
+                columns=columns,
+                all_columns=all_columns,
+                sort_by=sort_by,
+                full_table=full_table,
+                element_lst=element_lst,
+                **kwargs,
+            )
+        elif not auto_refresh_job_status:
+            return self.db.job_table(
+                sql_query=self.sql_query,
+                user=self.user,
+                project_path=self.project_path,
+                recursive=recursive,
+                columns=columns,
+                all_columns=all_columns,
+                sort_by=sort_by,
+                full_table=full_table,
+                element_lst=element_lst,
+                **kwargs,
+            )
+        else:
+            return self._refresh_job_status_file_table(
+                df=self.db.job_table(
+                    sql_query=self.sql_query,
+                    user=self.user,
+                    project_path=self.project_path,
+                    recursive=recursive,
+                    columns=columns,
+                    all_columns=all_columns,
+                    sort_by=sort_by,
+                    full_table=full_table,
+                    element_lst=element_lst,
+                    **kwargs,
+                )
+            )
 
     job_table.__doc__ = "\n".join(
         [
             ll
             for ll in FileTable.job_table.__doc__.split("\n")
             if not any(
                 [
@@ -812,24 +861,25 @@
             convert_to_object (bool): convert the object to an pyiron object or only access the HDF5 file - default=True
                                       accessing only the HDF5 file is about an order of magnitude faster, but only
                                       provides limited functionality. Compare the GenericJob object to JobCore object.
 
         Returns:
             GenericJob, JobCore: Either the full GenericJob object or just a reduced JobCore object
         """
-        jobpath = getattr(importlib.import_module("pyiron_base.job.path"), "JobPath")
+        from pyiron_base.jobs.job.path import JobPath
+
         if job_id is not None:
-            job = jobpath(db=self.db, job_id=job_id, user=self.user)
+            job = JobPath.from_job_id(db=self.db, job_id=job_id)
             if convert_to_object:
                 job = job.to_object()
                 job.reset_job_id(job_id=job_id)
                 job.set_input_to_read_only()
             return job
         elif db_entry is not None:
-            job = jobpath(db=self.db, db_entry=db_entry)
+            job = JobPath.from_db_entry(db_entry)
             if convert_to_object:
                 job = job.to_object()
                 job.set_input_to_read_only()
             return job
         else:
             raise ValueError("Either a job ID or an database entry has to be provided.")
 
@@ -843,23 +893,25 @@
 
         Returns:
             Project: pointing to the new project path
         """
         if not self.view_mode:
             if not isinstance(destination, Project):
                 raise TypeError("A project can only be copied to another project.")
-            for sub_project_name in self.list_groups():
+            for sub_project_name in tqdm(
+                self.list_groups(), desc="Moving sub-projects"
+            ):
                 if "_hdf5" not in sub_project_name:
                     sub_project = self.open(sub_project_name)
                     destination_sub_project = destination.open(sub_project_name)
                     sub_project.move_to(destination_sub_project)
-            for job_id in self.get_job_ids(recursive=False):
+            for job_id in tqdm(self.get_job_ids(recursive=False), desc="Moving jobs"):
                 ham = self.load(job_id)
                 ham.move_to(destination)
-            for file in self.list_files():
+            for file in tqdm(self.list_files(), desc="Moving files"):
                 shutil.move(os.path.join(self.path, file), destination.path)
         else:
             raise EnvironmentError("move_to: is not available in Viewermode !")
 
     def nodes(self):
         """
         Filter project by nodes
@@ -879,55 +931,93 @@
             project_only (bool): Query only for jobs within the current project - True by default
             recursive (bool): Include jobs from sub projects
             full_table (bool): Whether to show the entire pandas table
 
         Returns:
             pandas.DataFrame: Output from the queuing system - optimized for the Sun grid engine
         """
-        return queue_table(
-            job_ids=self.get_job_ids(recursive=recursive),
-            project_only=project_only,
-            full_table=full_table,
-        )
+        if not isinstance(self.db, FileTable):
+            return queue_table(
+                job_ids=self.get_job_ids(recursive=recursive),
+                project_only=project_only,
+                full_table=full_table,
+            )
+        else:
+            return queue_table(
+                project_only=project_only,
+                full_table=full_table,
+                working_directory_lst=[self.path],
+            )
 
     def queue_table_global(self, full_table=False):
         """
         Display the queuing system table as pandas.Dataframe
 
         Args:
             full_table (bool): Whether to show the entire pandas table
 
         Returns:
             pandas.DataFrame: Output from the queuing system - optimized for the Sun grid engine
         """
         df = queue_table(job_ids=[], project_only=False, full_table=full_table)
         if len(df) != 0 and self.db is not None:
-            return pandas.DataFrame(
-                [
-                    self.db.get_item_by_id(
-                        int(str(queue_ID).replace("pi_", "").replace(".sh", ""))
-                    )
-                    for queue_ID in df["jobname"]
-                    if str(queue_ID).startswith("pi_")
-                ]
-            )
+            if not isinstance(self.db, FileTable):
+                return pandas.DataFrame(
+                    [
+                        self.db.get_item_by_id(
+                            int(str(queue_ID).replace("pi_", "").replace(".sh", ""))
+                        )
+                        for queue_ID in df["jobname"]
+                        if str(queue_ID).startswith("pi_")
+                    ]
+                )
+            else:
+
+                def get_id_from_job_table(job_table, job_path):
+                    job_dir = "_hdf5".join(job_path.split("_hdf5")[:-1])
+                    job_name = os.path.basename(job_dir)
+                    project = os.path.dirname(job_dir) + "/"
+                    return job_table[
+                        (job_table.job == job_name) & (job_table.project == project)
+                    ].id.values[0]
+
+                job_table_df = self.job_table()
+
+                return pandas.DataFrame(
+                    [
+                        self.db.get_item_by_id(
+                            int(
+                                get_id_from_job_table(
+                                    job_table=job_table_df, job_path=working_directory
+                                )
+                            )
+                        )
+                        for queue_ID, working_directory in zip(
+                            df["jobname"], df["working_directory"]
+                        )
+                        if str(queue_ID).startswith("pi_")
+                    ]
+                )
         else:
             return None
 
-    def refresh_job_status(self, *jobs):
+    def refresh_job_status(self, *jobs, by_status=["running", "submitted"]):
         """
         Check if job is still running or crashed on the cluster node.
 
         If `jobs` is not given, check for all jobs listed as running in the current project.
 
         Args:
             *jobs (str, int): name of the job or job ID, any number of them
+            by_status (iterable of str): if not jobs are given, select all jobs
+                with the given status in this project
         """
         if len(jobs) == 0:
-            jobs = self.job_table(status="running").id
+            df = self.job_table()
+            jobs = df[df.status.isin(by_status)].id
         if self.db is not None:
             for job_specifier in jobs:
                 if isinstance(job_specifier, str):
                     job_id = get_job_id(
                         database=self.db,
                         sql_query=self.sql_query,
                         user=self.user,
@@ -966,17 +1056,55 @@
             if (
                 not que_mode
                 and self.db.get_item_by_id(job_id)["status"] not in ["finished"]
             ) or (
                 que_mode
                 and self.db.get_item_by_id(job_id)["status"] in ["running", "submitted"]
             ):
-                if not self.queue_check_job_is_waiting_or_running(self.inspect(job_id)):
+                job = self.inspect(job_id)
+                # a job can be in status running or submitted without being on
+                # the queue, if the run mode is worker or non_modal.  In this
+                # case we do not want to check the queue status, so we just
+                # short circuit here.
+                if job["server"]["run_mode"] in ["worker", "non_modal"]:
+                    return
+                if not self.queue_check_job_is_waiting_or_running(job):
                     self.db.set_job_status(job_id=job_id, status="aborted")
 
+    def _refresh_job_status_file_table(self, df):
+        """
+        Internal function to refresh the job table and update the job table with the status from the queuing system.
+
+        Args:
+            df (pandas.DataFrame): job table from the file based database
+
+        Returns:
+            pandas.DataFrame: updated job table with status from the queuing system
+        """
+
+        def convert_queue_status(queue_status):
+            return {"pending": "submitted"}.get(queue_status, default=queue_status)
+
+        df_queue = state.queue_adapter.get_status_of_my_jobs()
+
+        status_lst = df.status.values.tolist()
+        working_dir_lst = df.project + df.job + "_hdf5/" + df.job
+        for i, [working_dir, status] in enumerate(
+            zip(working_dir_lst, status_lst.copy())
+        ):
+            if status == "initialized":
+                df_tmp = df_queue[df_queue.working_directory == working_dir]
+                if len(df_tmp) > 0:
+                    status_lst[i] = convert_queue_status(
+                        queue_status=df_tmp.status.values[0]
+                    )
+        df["status"] = status_lst
+
+        return df
+
     def remove_file(self, file_name):
         """
         Remove a file (same as unlink()) - copied from os.remove()
 
         If dir_fd is not None, it should be a file descriptor open to a directory,
           and path should be relative; path will then be relative to that directory.
         dir_fd may not be implemented on your platform.
@@ -1116,15 +1244,21 @@
                 print("remove directory: {}".format(self.path))
                 shutil.rmtree(self.path, ignore_errors=True)
             else:
                 for root, *_ in os.walk(self.path, topdown=False):
                     # dirs and files return values of the iterator are not updated when removing files, so we need to
                     # manually call listdir
                     if len(os.listdir(root)) == 0:
-                        os.rmdir(root)
+                        root = root.rstrip(os.sep)
+                        # the project was symlinked before being deleted
+                        if os.path.islink(root):
+                            os.rmdir(os.readlink(root))
+                            os.remove(root)
+                        else:
+                            os.rmdir(root)
         else:
             raise EnvironmentError("remove() is not available in view_mode!")
 
     def set_job_status(self, job_specifier, status, project=None):
         """
         Set the status of a particular job
 
@@ -1226,17 +1360,17 @@
             convert_to_object (bool): convert the object to an pyiron object or only access the HDF5 file - default=True
                                       accessing only the HDF5 file is about an order of magnitude faster, but only
                                       provides limited functionality. Compare the GenericJob object to JobCore object.
 
         Returns:
             GenericJob, JobCore: Either the full GenericJob object or just a reduced JobCore object
         """
-        job = getattr(importlib.import_module("pyiron_base.job.path"), "JobPathBase")(
-            job_path=job_path
-        )
+        from pyiron_base.jobs.job.path import JobPath
+
+        job = JobPath(job_path)
         if convert_to_object:
             job = job.to_object()
         job.set_input_to_read_only()
         return job
 
     @staticmethod
     def get_external_input():
@@ -1410,15 +1544,15 @@
         """
         if isinstance(item, slice):
             if not (item.start or item.stop or item.step):
                 return self.values()
             print("slice: ", item)
             raise NotImplementedError("Implement if needed, e.g. for [:]")
         else:
-            item_lst = [sub_item.replace(" ", "") for sub_item in item.split("/")]
+            item_lst = item.split("/")
             if len(item_lst) > 1:
                 try:
                     return self._get_item_helper(
                         item=item_lst[0], convert_to_object=False
                     ).__getitem__("/".join(item_lst[1:]))
                 except ValueError:
                     return self._get_item_helper(
@@ -1448,15 +1582,19 @@
                                       provides limited functionality. Compare the GenericJob object to JobCore object.
 
         Returns:
             Project, GenericJob, JobCore, dict, list, float: basically any kind of item inside the project.
         """
         if item == "..":
             return self.parent_group
-        if item in self.list_nodes():
+        try:
+            item_save = _get_safe_job_name(name=item)
+        except ValueError:
+            item_save = None
+        if item in self.list_nodes() or item_save in self.list_nodes():
             if self._inspect_mode or not convert_to_object:
                 return self.inspect(item)
             return self.load(item)
         if item in self.list_files(extension="h5"):
             file_name = posixpath.join(self.path, "{}.h5".format(item))
             return ProjectHDFio(project=self, file_name=file_name)
         if item in self.list_files():
@@ -1531,27 +1669,40 @@
                 self.db.item_update(
                     {"project": self.project_path}, db_entry_in_old_format[0]["id"]
                 )
             elif db_entry_in_old_format:
                 for entry in db_entry_in_old_format:
                     self.db.item_update({"project": self.project_path}, entry["id"])
 
-    def pack(self, destination_path, csv_file_name="export.csv", compress=True):
+    def pack(
+        self,
+        destination_path,
+        csv_file_name="export.csv",
+        compress=True,
+        copy_all_files=False,
+    ):
         """
-        by this funtion, the job table is exported to a csv file
-        and the project directory is copied and compressed (by default) to a file.
+        Export job table to a csv file and copy (and optionally compress) the project directory.
 
         Args:
-        destination_path (str) gives the ralative path, in which the project folder is copied and the compressed
-        csv_file_name (str) is the name of the csv file used to store the project table.
-        compress (boolian), if true, the function will compress the destination_path to a tar.gz file.
+            destination_path (str): gives the relative path, in which the project folder is copied and compressed
+            csv_file_name (str): is the name of the csv file used to store the project table.
+            compress (bool): if true, the function will compress the destination_path to a tar.gz file.
+            copy_all_files (bool):
         """
         directory_to_transfer = os.path.basename(self.path[:-1])
+        if destination_path == directory_to_transfer:
+            raise ValueError(
+                "The destination_path cannot have the same name as the project to compress."
+            )
         export_archive.copy_files_to_archive(
-            directory_to_transfer, destination_path, compressed=compress
+            directory_to_transfer,
+            destination_path,
+            compressed=compress,
+            copy_all_files=copy_all_files,
         )
         df = export_archive.export_database(
             self, directory_to_transfer, destination_path
         )
         df.to_csv(csv_file_name)
 
     def unpack(self, origin_path, csv_file_name="export.csv", compress=True):
@@ -1599,14 +1750,74 @@
         """
         if hasattr(cls, name):
             raise AttributeError(
                 f"{cls.__name__} already has an attribute {name}. Please use a new name for registration."
             )
         setattr(cls, name, property(lambda self: tools(self)))
 
+    def symlink(self, target_dir):
+        """
+        Move underlying project folder to target and create a symlink to it.
+
+        The project itself does not change and is not updated in the database.  Instead the project folder is moved into
+        a subdirectory of target_dir with the same name as the project and a symlink is placed in the previous project path
+        pointing to the newly created one.
+
+        If self.path is already a symlink pointing inside target_dir, this method will silently return.
+
+        Args:
+            target_dir (str): new parent folder for the project
+
+        Raises:
+            OSError: when calling this method on non-unix systems
+            RuntimeError: the project path is already a symlink to somewhere else
+            RuntimeError: the project path has submitted or running jobs inside it, wait until after they are finished
+            RuntimeError: target already contains a subdirectory with the project name and it is not empty
+        """
+        target = os.path.join(target_dir, self.name)
+        destination = self.path
+        if destination[-1] == "/":
+            destination = destination[:-1]
+        if stat.S_ISLNK(os.lstat(destination).st_mode):
+            if os.readlink(destination) == target:
+                return
+            raise RuntimeError(
+                "Refusing to symlink and move a project that is already symlinked!"
+            )
+        if os.name != "posix":
+            raise OSError("Symlinking projects is only supported on unix systems!")
+        if len(self.job_table().query('status.isin(["submitted", "running"])')) > 0:
+            raise RuntimeError(
+                "Refusing to symlink and move a project that has submitted or running jobs!"
+            )
+        os.makedirs(target_dir, exist_ok=True)
+        if os.path.exists(target):
+            if len(os.listdir(target)) > 0:
+                raise RuntimeError(
+                    "Refusing to symlink and move a project to non-empty directory!"
+                )
+            else:
+                os.rmdir(target)
+        shutil.move(self.path, target_dir)
+        os.symlink(target, destination)
+
+    def unlink(self):
+        """
+        If the project folder is symlinked somewhere else remove the link and restore the original folder.
+
+        If it is not symlinked, silently return.
+        """
+        path = self.path.rstrip(os.sep)
+        if not stat.S_ISLNK(os.lstat(path).st_mode):
+            return
+
+        target = os.readlink(path)
+        os.unlink(path)
+        shutil.move(target, path)
+
 
 class Creator:
     def __init__(self, project):
         self._job_factory = JobFactory(project=project)
         self._project = project
 
     @property
```

### Comparing `pyiron_base-0.5.9/pyiron_base/project/gui.py` & `pyiron_base-0.6.0/pyiron_base/project/gui.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.9/pyiron_base/project/maintenance.py` & `pyiron_base-0.6.0/pyiron_base/project/maintenance.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 
     @property
     def local(self):
         return self._local
 
     @staticmethod
     def get_repository_status():
-
         """
         Finds the hashes and versions for every `pyiron` module available.
 
         Returns:
             pandas.DataFrame: The name of each module and the hash and version for its current git head.
         """
         module_names = [
@@ -56,17 +55,21 @@
         report = pandas.DataFrame(
             columns=["Module", "Git head", "Version"], index=range(len(module_names))
         )
         for i, name in enumerate(module_names):
             module = importlib.import_module(name)
             try:
                 repo = Repo(os.path.dirname(os.path.dirname(module.__file__)))
-                hash_ = repo.head.reference.commit.hexsha
             except InvalidGitRepositoryError:
                 hash_ = "Not a repo"
+            else:
+                try:
+                    hash_ = repo.head.reference.commit.hexsha
+                except (ValueError, TypeError):
+                    hash_ = "Error while resolving sha"
             if hasattr(module, "__version__"):
                 version = module.__version__
             else:
                 version = "not defined"
             report.loc[i] = [name, hash_, version]
 
         return report
```

### Comparing `pyiron_base-0.5.9/pyiron_base/project/path.py` & `pyiron_base-0.6.0/pyiron_base/project/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,18 +387,15 @@
             path (str): absolute path
             rel_path (str): relative path starting from the absolute path (optional)
 
         """
         if rel_path:
             rel_path = self._windows_path_to_unix_path(rel_path)
             path = posixpath.join(path, rel_path)
-        try:
-            os.makedirs(path)
-        except os.error:
-            pass
+        os.makedirs(path, exist_ok=True)
 
     @staticmethod
     def _get_project_from_path(full_path):
         """
         Split the absolute path in root_path and project_path using the top_path function in Settings()
 
         Args:
```

### Comparing `pyiron_base-0.5.9/pyiron_base/project/update/pyiron_base_03x_to_04x.py` & `pyiron_base-0.6.0/pyiron_base/project/update/pyiron_base_03x_to_04x.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.9/pyiron_base/pyio/parser.py` & `pyiron_base-0.6.0/pyiron_base/utils/parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.9/pyiron_base/server/generic.py` & `pyiron_base-0.6.0/pyiron_base/jobs/job/extension/server/generic.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 Server object class which is connected to each job containing the technical details how the job is executed.
 """
 
 from collections import OrderedDict
+import numbers
 from pyiron_base.state import state
-from pyiron_base.server.runmode import Runmode
+from pyiron_base.jobs.job.extension.server.runmode import Runmode
 import socket
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -76,27 +77,28 @@
         self, host=None, queue=None, cores=1, threads=1, run_mode="modal", new_hdf=True
     ):
         self._cores = cores
         self._threads = threads
         self._run_time = None
         self._memory_limit = None
         self._host = self._init_host(host=host)
+        self._run_mode = Runmode()
 
-        self._active_queue = queue
+        self.queue = queue
 
         self._user = state.settings.login_user
-        self._run_mode = Runmode()
         self.run_mode = run_mode
 
         self._queue_id = None
 
         self._new_hdf = new_hdf
         self._send_to_db = False
         self._structure_id = None
         self._accept_crash = False
+        self.additional_arguments = {}
 
     @property
     def send_to_db(self):
         """
         Get the boolean option to decide which jobs should be store in the external/public database
 
         Returns:
@@ -177,25 +179,25 @@
                     memory_max,
                 ) = state.queue_adapter.check_queue_parameters(
                     queue=new_scheduler,
                     cores=self.cores,
                     run_time_max=self.run_time,
                     memory_max=self.memory_limit,
                 )
-                if cores != self.cores:
+                if self.cores is not None and cores != self.cores:
                     self._cores = cores
-                    state.logger.debug("Updated the number of cores to: %i", cores)
-                if run_time_max != self.run_time:
+                    state.logger.warning(f"Updated the number of cores to: {cores}")
+                if self.run_time is not None and run_time_max != self.run_time:
                     self._run_time = run_time_max
-                    state.logger.debug(
-                        "Updated the run time limit to: %i", run_time_max
+                    state.logger.warning(
+                        f"Updated the run time limit to: {run_time_max}"
                     )
-                if memory_max != self.memory_limit:
+                if self.memory_limit is not None and memory_max != self.memory_limit:
                     self._memory_limit = memory_max
-                    state.logger.debug("Updated the memory limit to: %i", memory_max)
+                    state.logger.warning(f"Updated the memory limit to: {memory_max}")
                 self._active_queue = new_scheduler
                 self.run_mode = "queue"
             else:
                 raise TypeError(
                     "No queue adapter defined. Have you "
                     "configured in $PYIRONRESOURCES_PATHS/queues?"
                 )
@@ -242,24 +244,30 @@
     def cores(self, new_cores):
         """
         The number of cores selected for the current simulation
 
         Args:
             new_cores (int): number of cores
         """
+        if not isinstance(new_cores, numbers.Integral):
+            converted = int(new_cores)
+            # if the conversion truncated the number, raise error otherwise silently accept it
+            if new_cores != converted:
+                raise ValueError(f"cores must be an integer number, not {new_cores}!")
+            new_cores = converted
         if state.queue_adapter is not None and self._active_queue is not None:
             cores = state.queue_adapter.check_queue_parameters(
                 queue=self.queue,
                 cores=new_cores,
                 run_time_max=self.run_time,
                 memory_max=self.memory_limit,
             )[0]
             if cores != new_cores:
                 self._cores = cores
-                state.logger.debug("Updated the number of cores to: %i", cores)
+                state.logger.warning(f"Updated the number of cores to: {cores}")
             else:
                 self._cores = new_cores
         else:
             self._cores = new_cores
 
     @property
     def run_time(self):
@@ -288,15 +296,15 @@
                 queue=self.queue,
                 cores=self.cores,
                 run_time_max=new_run_time,
                 memory_max=self.memory_limit,
             )[1]
             if run_time_max != new_run_time:
                 self._run_time = run_time_max
-                state.logger.debug("Updated the run time limit to: %i", run_time_max)
+                state.logger.warning(f"Updated the run time limit to: {run_time_max}")
             else:
                 self._run_time = new_run_time
         else:
             self._run_time = new_run_time
 
     @property
     def memory_limit(self):
@@ -309,15 +317,15 @@
                 queue=self.queue,
                 cores=self.cores,
                 run_time_max=self.run_time,
                 memory_max=limit,
             )[2]
             if memory_max != limit:
                 self._memory_limit = memory_max
-                state.logger.debug("Updated the memory limit to: %i", memory_max)
+                state.logger.warning(f"Updated the memory limit to: {memory_max}")
             else:
                 self._memory_limit = limit
         else:
             self._memory_limit = limit
 
     @property
     def run_mode(self):
@@ -433,14 +441,16 @@
         hdf_dict["cores"] = self.cores
         hdf_dict["threads"] = self.threads
         hdf_dict["new_h5"] = self.new_hdf
         hdf_dict["structure_id"] = self.structure_id
         hdf_dict["run_time"] = self.run_time
         hdf_dict["memory_limit"] = self.memory_limit
         hdf_dict["accept_crash"] = self.accept_crash
+        if len(self.additional_arguments) > 0:
+            hdf_dict["additional_arguments"] = self.additional_arguments
 
         if group_name is not None:
             with hdf.open(group_name) as hdf_group:
                 hdf_group["server"] = hdf_dict
         else:
             hdf["server"] = hdf_dict
 
@@ -474,14 +484,16 @@
             self._run_time = hdf_dict["run_time"]
         if "memory_limit" in hdf_dict.keys():
             self._memory_limit = hdf_dict["memory_limit"]
         if "accept_crash" in hdf_dict.keys():
             self._accept_crash = hdf_dict["accept_crash"] == 1
         if "threads" in hdf_dict.keys():
             self._threads = hdf_dict["threads"]
+        if "additional_arguments" in hdf_dict.keys():
+            self.additional_arguments = hdf_dict["additional_arguments"]
         self._new_hdf = hdf_dict["new_h5"] == 1
 
     def db_entry(self):
         """
         connect all the info regarding the server into a single word that can be used e.g. as entry in a database
 
         Returns:
```

### Comparing `pyiron_base-0.5.9/pyiron_base/server/queuestatus.py` & `pyiron_base-0.6.0/pyiron_base/jobs/job/extension/server/queuestatus.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 Set of functions to interact with the queuing system directly from within pyiron - optimized for the Sun grid engine.
 """
 
 import pandas
 import time
+import numpy as np
 from pyiron_base.state import state
-from pyiron_base.generic.util import static_isinstance
-from pyiron_base.job.jobstatus import job_status_finished_lst
+from pyiron_base.utils.instance import static_isinstance
+from pyiron_base.jobs.job.extension.jobstatus import job_status_finished_lst
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -21,27 +22,34 @@
 __email__ = "janssen@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 QUEUE_SCRIPT_PREFIX = "pi_"
 
 
-def queue_table(job_ids=[], project_only=True, full_table=False):
+def queue_table(
+    job_ids=None, working_directory_lst=None, project_only=True, full_table=False
+):
     """
     Display the queuing system table as pandas.Dataframe
 
     Args:
         job_ids (list): check for a specific list of job IDs - empty list by default
+        working_directory_lst (list): list of working directories to include - empty list by default
         project_only (bool): Query only for jobs within the current project - True by default
         full_table (bool): Return all entries from the queuing system without filtering - False by default
 
     Returns:
         pandas.DataFrame: Output from the queuing system - optimized for the Sun grid engine
     """
-    if project_only and not job_ids:
+    job_ids = [] if job_ids is None else job_ids
+    working_directory_lst = (
+        [] if working_directory_lst is None else working_directory_lst
+    )
+    if project_only and not job_ids and not working_directory_lst:
         return []
     if state.queue_adapter is not None:
         if full_table:
             pandas.set_option("display.max_rows", None)
             pandas.set_option("display.max_columns", None)
         else:
             pandas.reset_option("display.max_rows")
@@ -51,21 +59,37 @@
             return df[
                 [
                     True if QUEUE_SCRIPT_PREFIX in job_name else False
                     for job_name in list(df.jobname)
                 ]
             ]
         else:
-            job_name_lst = [QUEUE_SCRIPT_PREFIX + str(job_id) for job_id in job_ids]
-            return df[
-                [
-                    True if job_name in job_name_lst else False
-                    for job_name in list(df.jobname)
+            if len(job_ids) > len(working_directory_lst):
+                job_name_lst = [QUEUE_SCRIPT_PREFIX + str(job_id) for job_id in job_ids]
+                return df[
+                    [
+                        True if job_name in job_name_lst else False
+                        for job_name in list(df.jobname)
+                    ]
                 ]
-            ]
+            else:
+                if len(df) > 0 and "working_directory" in df.columns:
+                    return df[
+                        [
+                            any(
+                                [
+                                    working_dir.startswith(p)
+                                    for p in working_directory_lst
+                                ]
+                            )
+                            for working_dir in list(df.working_directory)
+                        ]
+                    ]
+                else:
+                    return df
     else:
         return None
 
 
 def queue_check_job_is_waiting_or_running(item):
     """
     Check if a job is still listed in the queue system as either waiting or running.
@@ -88,15 +112,15 @@
 
 def queue_info_by_job_id(job_id):
     """
     Display the queuing system info of job by qstat | grep  shell command
     as dictionary
 
     Args:
-        requested_id (int): query for a specific job_id
+        job_id (int): query for a specific job_id
 
     Returns:
         dict: Dictionary with the output from the queuing system - optimized for the Sun grid engine
     """
     if state.queue_adapter is not None:
         return state.queue_adapter.get_status_of_job(process_id=job_id)
     else:
@@ -117,15 +141,15 @@
 
 
 def queue_delete_job(item):
     """
     Delete a job from the queuing system
 
     Args:
-        item (int, pyiron_base.job.generic.GenericJob): Provide either the job_ID or the full hamiltonian
+        item (int, pyiron_base.jobs.job.generic.GenericJob): Provide either the job_ID or the full hamiltonian
 
     Returns:
         str: Output from the queuing system as string - optimized for the Sun grid engine
     """
     que_id = validate_que_request(item)
     if state.queue_adapter is not None:
         return state.queue_adapter.delete_job(process_id=que_id)
@@ -134,15 +158,15 @@
 
 
 def queue_enable_reservation(item):
     """
     Enable a reservation for a particular job within the queuing system
 
     Args:
-        item (int, pyiron_base.job.generic.GenericJob): Provide either the job_ID or the full hamiltonian
+        item (int, pyiron_base.jobs.job.generic.GenericJob): Provide either the job_ID or the full hamiltonian
 
     Returns:
         str: Output from the queuing system as string - optimized for the Sun grid engine
     """
     que_id = validate_que_request(item)
     if state.queue_adapter is not None:
         if isinstance(que_id, list):
@@ -156,15 +180,15 @@
 
 
 def wait_for_job(job, interval_in_s=5, max_iterations=100):
     """
     Sleep until the job is finished but maximum interval_in_s * max_iterations seconds.
 
     Args:
-        job (pyiron_base.job.generic.GenericJob): Job to wait for
+        job (pyiron_base.job.utils.GenericJob): Job to wait for
         interval_in_s (int): interval when the job status is queried from the database - default 5 sec.
         max_iterations (int): maximum number of iterations - default 100
 
     Raises:
         ValueError: max_iterations reached, job still running
     """
     if job.status.string not in job_status_finished_lst:
@@ -175,15 +199,14 @@
         ):
             finished = False
             for _ in range(max_iterations):
                 if not queue_check_job_is_waiting_or_running(item=job):
                     state.queue_adapter.transfer_file_to_remote(
                         file=job.project_hdf5.file_name,
                         transfer_back=True,
-                        delete_remote=False,
                     )
                     status_hdf5 = job.project_hdf5["status"]
                     job.status.string = status_hdf5
                 else:
                     status_hdf5 = job.status.string
                 if status_hdf5 in job_status_finished_lst:
                     job.transfer_from_remote()
@@ -212,24 +235,26 @@
 
 def wait_for_jobs(
     project,
     interval_in_s=5,
     max_iterations=100,
     recursive=True,
     ignore_exceptions=False,
+    try_collecting=False,
 ):
     """
     Wait for the calculation in the project to be finished
 
     Args:
         project: Project instance the jobs is located in
         interval_in_s (int): interval when the job status is queried from the database - default 5 sec.
         max_iterations (int): maximum number of iterations - default 100
         recursive (bool): search subprojects [True/False] - default=True
         ignore_exceptions (bool): ignore eventual exceptions when retrieving jobs - default=False
+        try_collecting (bool): try to run collect for fetched jobs that don't have a status counting as finished - default=False
 
     Raises:
         ValueError: max_iterations reached, but jobs still running
     """
     finished = False
     for _ in range(max_iterations):
         project.update_from_remote(recursive=True, ignore_exceptions=ignore_exceptions)
@@ -239,108 +264,127 @@
             finished = True
             break
         time.sleep(interval_in_s)
     if not finished:
         raise ValueError("Maximum iterations reached, but the job was not finished.")
 
 
-def update_from_remote(project, recursive=True, ignore_exceptions=False):
+def update_from_remote(
+    project, recursive=True, ignore_exceptions=False, try_collecting=False
+):
     """
     Update jobs from the remote server
 
     Args:
         project: Project instance the jobs is located in
         recursive (bool): search subprojects [True/False] - default=True
         ignore_exceptions (bool): ignore eventual exceptions when retrieving jobs - default=False
+        try_collecting (bool): try to collect jobs that don't have a status counting as finished - default=False
 
     Returns:
         returns None if ignore_exceptions is False or when no error occured.
         returns a list with job ids when errors occured, but were ignored
     """
     if state.queue_adapter is not None and state.queue_adapter.remote_flag:
         df_project = project.job_table(recursive=recursive)
         df_submitted = df_project[df_project.status == "submitted"]
         df_combined = df_project[df_project.status.isin(["running", "submitted"])]
         df_queue = state.queue_adapter.get_status_of_my_jobs()
         if (
             len(df_queue) > 0
-            and len(df_queue[df_queue.jobname.str.startswith("pi_")]) > 0
+            and len(df_queue[df_queue.jobname.str.contains(QUEUE_SCRIPT_PREFIX)]) > 0
         ):
-            df_queue = df_queue[df_queue.jobname.str.startswith("pi_")]
+            df_queue = df_queue[df_queue.jobname.str.contains(QUEUE_SCRIPT_PREFIX)]
             df_queue["pyiron_id"] = df_queue.apply(
-                lambda x: int(x["jobname"].split("pi_")[1]), axis=1
+                lambda x: int(x["jobname"].split(QUEUE_SCRIPT_PREFIX)[-1]), axis=1
             )
-            jobs_now_running_lst = df_queue[
-                df_queue.status == "running"
-            ].pyiron_id.values
-            _ = [
-                project.set_job_status(job_specifier=job_id, status="running")
-                for job_id in df_submitted.id.values
-                if job_id in jobs_now_running_lst
+            queue_running = df_queue[df_queue.status == "running"].pyiron_id.values
+            jobs_now_running_lst = df_submitted.id.values[
+                np.isin(df_submitted.id.values, queue_running)
             ]
-        else:
-            jobs_now_running_lst = []
+            project.db.set_job_status(status="running", job_id=jobs_now_running_lst)
+
+            fetch_ids = df_combined.id.values[
+                np.isin(df_combined.id.values, df_queue.pyiron_id.values, invert=True)
+            ]
+        else:  # handle empty pyiron queue case for fetching
+            fetch_ids = df_combined.id.values
+
         failed_jobs = []
-        for job_id in df_combined.id.values:
-            if job_id not in jobs_now_running_lst:
-                try:
-                    job = project.inspect(job_id)
-                    state.queue_adapter.transfer_file_to_remote(
-                        file=job.project_hdf5.file_name,
-                        transfer_back=True,
-                        delete_remote=False,
+        for job_id in fetch_ids:
+            try:
+                job = project.load(job_id)
+                retrieve_job(job, try_collecting=try_collecting)
+            except Exception as e:
+                if ignore_exceptions:
+                    state.logger.warning(
+                        f"An error occurred while trying to retrieve job {job_id}\n"
+                        f"Error message: \n{e}"
                     )
-                    status_hdf5 = job.project_hdf5["status"]
-                    project.set_job_status(job_specifier=job.job_id, status=status_hdf5)
-                    if status_hdf5 in job_status_finished_lst:
-                        job_object = job.to_object()
-                        job_object.transfer_from_remote()
-                except Exception as e:
-                    if ignore_exceptions:
-                        state.logger.warning(
-                            f"An error occured while trying to retrieve job {job_id}\n"
-                            f"Error message: \n{e}"
-                        )
-                        failed_jobs.append(job_id)
-                    else:
-                        raise e
+                    failed_jobs.append(job_id)
+                else:
+                    raise e
+
         if len(failed_jobs) > 0:
             return failed_jobs
 
 
+def retrieve_job(job, try_collecting=False):
+    """
+    Retrieve a job from remote server and check if it has a "finished status".
+    Optionally try to collect its output.
+
+    Args:
+        job: pyiron job
+        try_collecting (bool): whether to run collect if not finished - default=False
+
+    Returns:
+        returns None
+    """
+    job.transfer_from_remote()
+    if job.status in job_status_finished_lst:
+        return
+
+    if try_collecting:
+        job.status.collect = True
+        job.run()
+
+
 def validate_que_request(item):
     """
     Internal function to convert the job_ID or hamiltonian to the queuing system ID.
 
     Args:
-        item (int, pyiron_base.job.generic.GenericJob): Provide either the job_ID or the full hamiltonian
+        item (int, pyiron_base.jobs.job.generic.GenericJob): Provide either the job_ID or the full hamiltonian
 
     Returns:
         int: queuing system ID
     """
 
     if isinstance(item, int):
         que_id = item
-    elif static_isinstance(item.__class__, "pyiron_base.master.generic.GenericMaster"):
+    elif static_isinstance(
+        item.__class__, "pyiron_base.jobs.master.generic.GenericMaster"
+    ):
         if item.server.queue_id:
             que_id = item.server.queue_id
         else:
             queue_id_lst = [
                 item.project.load(child_id).server.queue_id
                 for child_id in item.child_ids
             ]
             que_id = [queue_id for queue_id in queue_id_lst if queue_id is not None]
             if len(que_id) == 0:
                 raise ValueError("This job does not have a queue ID.")
-    elif static_isinstance(item.__class__, "pyiron_base.job.generic.GenericJob"):
+    elif static_isinstance(item.__class__, "pyiron_base.jobs.job.generic.GenericJob"):
         if item.server.queue_id:
             que_id = item.server.queue_id
         else:
             raise ValueError("This job does not have a queue ID.")
-    elif static_isinstance(item.__class__, "pyiron_base.job.core.JobCore"):
+    elif static_isinstance(item.__class__, "pyiron_base.jobs.job.core.JobCore"):
         if "server" in item.project_hdf5.list_nodes():
             server_hdf_dict = item.project_hdf5["server"]
             if "qid" in server_hdf_dict.keys():
                 que_id = server_hdf_dict["qid"]
             else:
                 raise ValueError("This job does not have a queue ID.")
         else:
```

### Comparing `pyiron_base-0.5.9/pyiron_base/server/runmode.py` & `pyiron_base-0.6.0/pyiron_base/jobs/job/extension/server/runmode.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 run_mode_lst = [
     "modal",
     "non_modal",
     "queue",
     "manual",
     "thread",
     "worker",
+    "srun",
+    "flux",
     "interactive",
     "interactive_non_modal",
 ]
 
 
 class Runmode(object):
     """
```

### Comparing `pyiron_base-0.5.9/pyiron_base/state/__init__.py` & `pyiron_base-0.6.0/pyiron_base/state/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 
 from pyiron_base.state.logger import logger as _logger
 from pyiron_base.database.manager import database as _database
 from pyiron_base.state.publications import publications as _publications
 from pyiron_base.state.queue_adapter import queue_adapters as _queue_adapters
 from pyiron_base.state.settings import settings as _settings
-from pyiron_base.generic.util import Singleton
+from pyiron_base.interfaces.singleton import Singleton
 from typing import Dict, Union
 
 __author__ = "Liam Huber"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
```

### Comparing `pyiron_base-0.5.9/pyiron_base/state/install.py` & `pyiron_base-0.6.0/pyiron_base/state/install.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import os
 import tarfile
 from shutil import copytree, rmtree
 import tempfile
 import stat
 import urllib.request as urllib2
+from pyiron_base.utils.safetar import safe_extract
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -48,15 +49,15 @@
     urllib2.urlretrieve(giturl_for_zip_file, temp_zip_file)
     if os.path.exists(user_directory):
         raise ValueError(
             "The resource directory exists already, therefore it can not be created: ",
             user_directory,
         )
     with tarfile.open(temp_zip_file, "r:gz") as tar:
-        tar.extractall(temp_directory)
+        safe_extract(tar, temp_directory)
     copytree(temp_extract_folder, user_directory)
     if os.name != "nt":  #
         for root, dirs, files in os.walk(user_directory):
             for file in files:
                 if ".sh" in file:
                     st = os.stat(os.path.join(root, file))
                     os.chmod(os.path.join(root, file), st.st_mode | stat.S_IEXEC)
@@ -86,16 +87,15 @@
                     "PROJECT_PATHS = " + project_path + "\n",
                     "RESOURCE_PATHS = " + resource_path + "\n",
                 ]
             )
         project_path = os.path.normpath(
             os.path.abspath(os.path.expanduser(project_path))
         )
-        if not os.path.exists(project_path):
-            os.makedirs(project_path)
+        os.makedirs(project_path, exist_ok=True)
 
 
 def install_dialog(silently=False):
     if not silently:
         user_input = None
     else:
         user_input = "yes"
@@ -114,14 +114,17 @@
             install_pyiron(
                 config_file_name="~/.pyiron",
                 zip_file="resources.tar.gz",
                 resource_directory="~/pyiron/resources",
                 giturl_for_zip_file="https://github.com/pyiron/pyiron-resources/releases/latest/download/resources.tar.gz",
                 git_folder_name="resources",
             )
+            print(
+                "pyiron resources installed - restart your server for the changes to be in effect"
+            )
         else:
             raise ValueError("pyiron was not installed!")
     else:
         print("pyiron is already installed.")
 
 
 def install_pyiron(
@@ -136,21 +139,26 @@
     Function to configure the pyiron installation.
 
     Args:
         config_file_name (str): configuration file name - usually ~/.pyiron
         zip_file (str): name of the compressed file
         project_path (str): the location where pyiron is going to store the pyiron projects
         resource_directory (str): the location where the resouces (executables, potentials, ...) for pyiron are stored.
-        giturl_for_zip_file (str): url for the zipped resources file on github
+        giturl_for_zip_file (str/None): url for the zipped resources file on github.
+            (Default points to pyiron's github resource repository. If None, leaves the
+            resources directory *empty*.)
         git_folder_name (str): name of the extracted folder
     """
     _write_config_file(
         file_name=config_file_name,
         project_path=project_path,
         resource_path=resource_directory,
     )
-    _download_resources(
-        zip_file=zip_file,
-        resource_directory=resource_directory,
-        giturl_for_zip_file=giturl_for_zip_file,
-        git_folder_name=git_folder_name,
-    )
+    if giturl_for_zip_file is not None:
+        _download_resources(
+            zip_file=zip_file,
+            resource_directory=resource_directory,
+            giturl_for_zip_file=giturl_for_zip_file,
+            git_folder_name=git_folder_name,
+        )
+    else:
+        os.makedirs(resource_directory)
```

### Comparing `pyiron_base-0.5.9/pyiron_base/state/logger.py` & `pyiron_base-0.6.0/pyiron_base/state/logger.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.9/pyiron_base/state/publications.py` & `pyiron_base-0.6.0/pyiron_base/state/publications.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Well we can't, but that's the idea behind this alpha-stage feature.
 The idea is that various pyiron submodules and objects will register their relevant publications and you can just ask
 your project for a list of everything you should cite.
 `Publications` is the way we work towards this goal.
 """
 
 import pandas
-from pyiron_base.generic.util import Singleton
+from pyiron_base.interfaces.singleton import Singleton
 from typing import Dict, Union, List
 from typing_extensions import Literal
 
 __author__ = "Joerg Neugebauer, Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
```

### Comparing `pyiron_base-0.5.9/pyiron_base/state/queue_adapter.py` & `pyiron_base-0.6.0/pyiron_base/state/queue_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 This is a central control point for all the queue adapters, i.e. how we talk to remote computing power.
 Before this class was written, we only ever used the first queue adapter we found defined in the resources.
 That behaviour is maintained, but now with `QueueAdapters` we can trivially extend to using multiple resources and
 multiple adapters.
 """
 
-from pyiron_base.generic.util import Singleton
+from pyiron_base.interfaces.singleton import Singleton
 from pysqa import QueueAdapter as PySQAAdpter
 import os
 from pyiron_base.state.settings import settings
 
 __author__ = "Liam Huber"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
```

### Comparing `pyiron_base-0.5.9/pyiron_base/state/settings.py` & `pyiron_base-0.6.0/pyiron_base/state/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,19 +30,20 @@
 
 Finally, :class:`Settings` converts any file paths from your OS to something pyiron-compatible, and does some other
 cleaning and consistency checks.
 """
 
 import ast
 import os
+import warnings
 from configparser import ConfigParser
 from pyiron_base.state.logger import logger
 from pyiron_base.state.publications import publications
 from pathlib import Path
-from pyiron_base.generic.util import deprecate, Singleton
+from pyiron_base.interfaces.singleton import Singleton
 from typing import Union, Dict, List
 from distutils.util import strtobool
 from copy import deepcopy
 
 __author__ = "Jan Janssen, Liam Huber"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
@@ -51,16 +52,20 @@
 __version__ = "1.0"
 __maintainer__ = "Liam Huber"
 __email__ = "huber@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 
+PYIRON_DICT_NAME = "PYIRON"
+
+
 class Settings(metaclass=Singleton):
-    """
+    """The unique settings object (singleton) for the currently running pyiron instance.
+
     The settings object reads configuration data from the following sources in decreasing order of priority: system
     environment values (starting with 'PYIRON'), a configuration file identified in the PYIRONCONFIG system environment
     variable, or a default configuration file in ~/.pyiron. One (or none) of these is used to overwrite default values
     specified in the codebase.
 
     Here are the configuration keys as the appear in the python code/config files/system env variables:
 
@@ -79,14 +84,22 @@
         sql_type / TYPE / PYIRONSQLTYPE ("SQLite"|"Postgres"|"MySQL"): What type of SQL database to use. (Default is
             "SQLite".)
         sql_user_key / PASSWD / PYIRONSQLUSERKEY ():
         sql_database / NAME / PYIRONSQLDATABASE ():
         project_check_enabled / PROJECT_CHECK_ENABLED / PYIRONPROJECTCHECKENABLED (bool):
         disable_database / DISABLE_DATABASE / PYIRONDISABLE (bool): Whether to turn off the database and use a
             file-system-based hierarchy. (Default is False.)
+        credentials_file / CREDENTIALS_FILE / CREDENTIALSFILE (str): Path to an additional credentials file holding
+            credential information. If specified, the values in the credentials_file overwrite the values of other
+            sources.
+        write_work_dir_warnings / WRITE_WORK_DIR_WARNINGS / PYIRONWRITEWORKDIRWARNINGS (bool): Whether to write
+            the working directory warning files to inform users about possibly modified content. (Default is True).
+        config_file_permissions_warning / CONFIG_FILE_PERMISSIONS_WARNING / PYIRONCONFIGFILEPERMISSIONSWARNING (bool):
+            Whether to print a warning message, when the permission of the .pyiron config file, let others access it.
+
 
     Properties:
         configuration (dict): Global variables for configuring the pyiron experience.
         resource_paths (list[str]): A shortcut to the configuration value for locations with pyiron resources.
         login_user (str): A shortcut to the configuration value for the user name.
         default_configuration (dict): Default values for configuration items.
         environment_configuration_map (dict): A map between system environment variable names and the configuration.
@@ -97,20 +110,25 @@
             dictionary (cf keys above) as the primary (overriding) source but otherwise has the same primacy order as
             the initialization.
         convert_path_to_abs_posix: A path converter, since pyiron internally uses posix style regardless of OS.
     """
 
     def __init__(self):
         self._configuration = None
+        self._credentials = None
         self.update()
 
     @property
     def configuration(self) -> Dict:
         return self._configuration
 
+    @property
+    def credentials(self) -> Dict:
+        return self._credentials
+
     def update(self, user_dict: Union[Dict, None] = None) -> None:
         """
         Starting from a clean set of defaults, overwrite with input from exactly one source with the following priority:
         - User input
         - System environment variables
         - A config file at a locations specified in the PYIRONCONFIG system environment variable
         - A config file at ~/.pyiron
@@ -125,14 +143,28 @@
         if user_dict is not None:
             self._update_from_dict(user_dict)
         elif env_dict is not None:
             self._update_from_dict(env_dict)
         elif file_dict is not None:
             self._update_from_dict(file_dict)
 
+        self._credentials = self._add_credentials_from_file()
+        self._update_credentials_from_std_pyiron_config()
+
+        if (
+            self._configuration["config_file_permissions_warning"]
+            and self._configuration["credentials_file"] is not None
+            and os.path.exists(self._configuration["credentials_file"])
+            and oct(os.stat(self._configuration["credentials_file"]).st_mode)[-2:]
+            != "00"
+        ):
+            logger.warning(
+                "Credentials file can be read by other users - check permissions."
+            )
+
         for k in ["CONDA_PREFIX", "CONDA_DIR"]:
             if k in os.environ.keys():
                 res_path = os.path.join(os.environ[k], "share", "pyiron")
                 if os.path.exists(res_path):
                     self._configuration["resource_paths"].append(
                         self.convert_path_to_abs_posix(res_path)
                     )
@@ -155,14 +187,17 @@
                 "sql_file": self.convert_path_to_abs_posix("~/pyiron.db"),
                 "sql_host": None,
                 "sql_type": "SQLite",
                 "sql_user_key": None,
                 "sql_database": None,
                 "project_check_enabled": False,
                 "disable_database": False,
+                "credentials_file": None,
+                "write_work_dir_warnings": True,
+                "config_file_permissions_warning": True,
             }
         )
 
     @property
     def environment_configuration_map(self) -> Dict:
         return {
             "PYIRONUSER": "user",
@@ -178,14 +213,17 @@
             "PYIRONSQLFILE": "sql_file",
             "PYIRONSQHOST": "sql_host",
             "PYIRONSQLTYPE": "sql_type",
             "PYIRONSQLUSERKEY": "sql_user_key",
             "PYIRONSQLDATABASE": "sql_database",
             "PYIRONPROJECTCHECKENABLED": "project_check_enabled",
             "PYIRONDISABLE": "disable_database",
+            "PYIRONCREDENTIALSFILE": "credentials_file",
+            "PYIRONWRITEWORKDIRWARNINGS": "write_work_dir_warnings",
+            "PYIRONCONFIGFILEPERMISSIONSWARNING": "config_file_permissions_warning",
         }
 
     @property
     def file_configuration_map(self) -> Dict:
         return {
             "USER": "user",
             "RESOURCE_PATHS": "resource_paths",
@@ -202,16 +240,37 @@
             "DATABASE_FILE": "sql_file",  # Alternative name
             "HOST": "sql_host",
             "TYPE": "sql_type",
             "PASSWD": "sql_user_key",
             "NAME": "sql_database",
             "PROJECT_CHECK_ENABLED": "project_check_enabled",
             "DISABLE_DATABASE": "disable_database",
+            "CREDENTIALS_FILE": "credentials_file",
+            "WRITE_WORK_DIR_WARNINGS": "write_work_dir_warnings",
+            "CONFIG_FILE_PERMISSIONS_WARNING": "config_file_permissions_warning",
+        }
+
+    @property
+    def file_credential_map(self) -> Dict:
+        return {
+            "PASSWD": "sql_user_key",
+            "VIEWERPASSWD": "sql_view_user_key",
         }
 
+    @property
+    def environment_credential_map(self) -> Dict:
+        return {
+            "PYIRONSQLVIEWUSERKEY": "sql_view_user_key",
+            "PYIRONSQLUSERKEY": "sql_user_key",
+        }
+
+    @property
+    def _credential_keys(self) -> List:
+        return list(self.environment_credential_map.values())
+
     @staticmethod
     def convert_path_to_abs_posix(path: str) -> str:
         """
         Convert path to an absolute POSIX path
 
         Args:
             path (str): input path.
@@ -264,18 +323,16 @@
             elif sql_type == "SQLite":
                 sql_file = config["sql_file"]
                 if sql_file is None:
                     # SQLite is raising ugly error messages when the database directory does not exist.
                     raise ValueError(
                         "For sql_type SQLite, the sql_file must not be None"
                     )
-                elif os.path.dirname(sql_file) != "" and not os.path.exists(
-                    os.path.dirname(sql_file)
-                ):
-                    os.makedirs(os.path.dirname(sql_file))
+                elif os.path.dirname(sql_file) != "":
+                    os.makedirs(os.path.dirname(sql_file), exist_ok=True)
             elif (
                 sql_type == "SQLalchemy"
                 and "sql_connection_string" not in config.keys()
             ):
                 raise ValueError(
                     "sql_type was SQLalchemy but did not find a sql_connection_string setting."
                 )
@@ -285,15 +342,15 @@
                 )
         except KeyError:
             pass
 
     @staticmethod
     def _validate_viewer_configuration(config: Dict) -> None:
         key_group = ["sql_view_table_name", "sql_view_user", "sql_view_user_key"]
-        present = [k in config.keys() for k in key_group]
+        present = [k in config.keys() and config[k] is not None for k in key_group]
         if any(present):
             if not all(present):
                 raise ValueError(
                     f"If any of {key_group} is included they all must be, but got {config.keys()}"
                 )
             if "sql_type" not in config or config["sql_type"] != "Postgres":
                 # Note: This requirement is *implicit* when the sql_view_connection_string is constructed
@@ -317,48 +374,119 @@
                     + "paths list should be empty 'project_paths=[]'. Currently it is: "
                     + str(config["project_paths"])
                 )
 
     def _get_config_from_environment(self) -> Union[Dict, None]:
         config = {}
         for k, v in os.environ.items():
-            try:
+            if k in self.environment_configuration_map:
                 config[self.environment_configuration_map[k]] = v
-            except KeyError:
-                pass
+            elif k in self.environment_credential_map:
+                config[self.environment_credential_map[k]] = v
         config = self._fix_boolean_var_in_config(config=config)
         return config if len(config) > 0 else None
 
+    def _get_remapped_credential_key(self, k):
+        """
+        Converts a key to the known key from the file_credential map or returns a .lower() variant of the unknown key.
+        This allows to stay consistent with the behavior of our current credentials and adds the possibility to add
+        additional credentials to the credentials file without the need to change pyiron_base.
+        """
+        if k.upper() in self.file_credential_map:
+            return self.file_credential_map[k.upper()]
+        elif k.upper() in self.file_configuration_map:
+            warnings.warn(
+                f"pyiron configuration key {k.upper()} used in the credentials file. "
+                "This does not take effect in the pyiron configuration!"
+            )
+
+        return k.lower()
+
+    def _add_credentials_from_file(self) -> Dict:
+        if (
+            "credentials_file" in self._configuration
+            and self._configuration["credentials_file"] is not None
+        ):
+            credential_file = self._configuration["credentials_file"]
+
+            # This gets all the entries in the credential file with the headers
+            # The key-value pairs in the [DEFAULT] section are added everywhere!
+            parser = ConfigParser(inline_comment_prefixes=(";",), interpolation=None)
+            parser.read(credential_file)
+            credentials = {}
+            for sec_name, section in parser.items():
+                credentials_w = {}
+
+                for k, v in section.items():
+                    credentials_w[self._get_remapped_credential_key(k)] = v
+                if len(credentials_w) > 0:
+                    credentials[sec_name.upper()] = credentials_w
+            return credentials
+
+    def _update_credentials_from_std_pyiron_config(self):
+        update_dict = {}
+        for key in self.file_credential_map.values():
+            if key in self._configuration:
+                update_dict[key] = self._configuration[key]
+
+        if len(update_dict) > 0:
+            if self._credentials is None:
+                self._credentials = {PYIRON_DICT_NAME: update_dict}
+            elif PYIRON_DICT_NAME in self._credentials:
+                self._credentials[PYIRON_DICT_NAME].update(update_dict)
+            else:
+                self._credentials[PYIRON_DICT_NAME] = update_dict
+
+    def _get_credentials_from_file(self, config: dict) -> Dict:
+        if "credentials_file" in config and config["credentials_file"] is not None:
+            credential_file = config["credentials_file"]
+
+            if not os.path.isfile(credential_file):
+                raise FileNotFoundError(credential_file)
+            credentials = (
+                self._parse_config_file(credential_file, self.file_credential_map) or {}
+            )
+            config.update(credentials)
+
+        return config
+
     def _get_config_from_file(self) -> Union[Dict, None]:
         if "PYIRONCONFIG" in os.environ.keys():
             config_file = os.environ["PYIRONCONFIG"]
         else:
             config_file = os.path.expanduser(os.path.join("~", ".pyiron"))
 
+        config = self._parse_config_file(config_file, self.file_configuration_map)
+
+        if config is not None:
+            config = self._fix_boolean_var_in_config(config=config)
+
+        return config
+
+    @staticmethod
+    def _parse_config_file(config_file, map_dict):
         if os.path.isfile(config_file):
             parser = ConfigParser(inline_comment_prefixes=(";",), interpolation=None)
             parser.read(config_file)
             config = {}
             for sec_name, section in parser.items():
                 for k, v in section.items():
-                    try:
-                        config[self.file_configuration_map[k.upper()]] = v
-                    except KeyError:
-                        pass
-            config = self._fix_boolean_var_in_config(config=config)
+                    if k.upper() in map_dict:
+                        config[map_dict[k.upper()]] = v
+            return config
         else:
-            config = None
-        return config
+            return None
 
     def _update_from_dict(self, config: Dict, map_: Union[None, Dict] = None) -> None:
         """
         Overwrite values of the configuration dictionary based on a new dictionary.
 
         Non-string non-None items are converted to the expected type and paths are converted to absolute POSIX paths.
         """
+        config = self._get_credentials_from_file(config)
         self._validate_sql_configuration(config=config)
         self._validate_viewer_configuration(config=config)
         self._validate_no_database_configuration(config=config)
 
         for key, value in config.items():
             key = key if map_ is None else map_[key]
 
@@ -370,15 +498,15 @@
                 self._configuration[key] = int(value)
             elif key == "sql_file":
                 self._configuration[key] = self.convert_path_to_abs_posix(value)
             elif key in ["project_check_enabled", "disable_database"]:
                 self._configuration[key] = (
                     value if isinstance(value, bool) else strtobool(value)
                 )
-            elif key not in self._configuration.keys():
+            elif key not in self._configuration and key not in self._credential_keys:
                 raise KeyError(
                     f"Got unexpected configuration key {key}, please choose from among {self._configuration.keys()}"
                 )
             else:
                 self._configuration[key] = value
 
     def _convert_to_list_of_paths(
```

### Comparing `pyiron_base-0.5.9/pyiron_base/state/update.py` & `pyiron_base-0.6.0/pyiron_base/state/update.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.9/pyiron_base/table/datamining.py` & `pyiron_base-0.6.0/pyiron_base/jobs/datamining.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import codecs
-from collections import OrderedDict
 from datetime import datetime
 import dill as pickle
 import json
 import numpy as np
 import os
 import pandas
 from pandas.errors import EmptyDataError
 from tqdm.auto import tqdm
 import types
+from typing import List, Tuple
 
-from pyiron_base.job.generic import GenericJob
-from pyiron_base.generic.datacontainer import DataContainer
-from pyiron_base.generic.hdfio import FileHDFio
-from pyiron_base.interfaces.has_groups import HasGroups
-from pyiron_base.master.generic import get_function_from_string
+from pyiron_base.utils.deprecate import deprecate
+from pyiron_base.jobs.job.generic import GenericJob
+from pyiron_base.jobs.job.extension import jobstatus
+from pyiron_base.storage.hdfio import FileHDFio
+from pyiron_base.jobs.master.generic import get_function_from_string
 
 
 __author__ = "Uday Gajera, Jan Janssen, Joerg Neugebauer"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -121,15 +121,15 @@
     def job_name_contains(job_name_segment):
         def filter_job_name_segment(job):
             return job_name_segment in job.job_name
 
         return filter_job_name_segment
 
 
-class PyironTable(HasGroups):
+class PyironTable:
     """
     Class for easy, efficient, and pythonic analysis of data from pyiron projects
 
     Args:
         project (pyiron.project.Project/None): The project to analyze
         name (str): Name of the pyiron table
         system_function_lst (list/ None): List of built-in functions
@@ -144,39 +144,27 @@
         self._name = name
         self._db_filter_function = always_true_pandas
         self._filter_function = always_true
         self._filter = JobFilters()
         self._system_function_lst = system_function_lst
         self.add = FunctionContainer(system_function_lst=self._system_function_lst)
         self._csv_file = csv_file_name
-        self.EMPTY_STR = "-"
 
     @property
     def filter(self):
         """
         Object containing pre-defined filter functions
 
         Returns:
             pyiron.table.datamining.JobFilters: The object containing the filters
 
         """
         return self._filter
 
     @property
-    def _file_name_csv(self):
-        if self._csv_file is None:
-            return self._project.path + self.name + ".csv"
-        else:
-            return self._csv_file
-
-    @property
-    def _file_name_txt(self):
-        return self._project.path + self.name + ".txt"
-
-    @property
     def name(self):
         """
         Name of the table. Takes the project name if not specified
 
         Returns:
             str: Name of the table
 
@@ -191,213 +179,120 @@
         Function to filter the a project database table before job specific functions are applied.
 
         The function must take a pyiron project table in the pandas.DataFrame format (project.job_table()) and return a
         boolean pandas.DataSeries with the same number of rows as the project table
 
         Example:
 
-            def function(df):
-                return (df["chemicalformula"=="H2"]) & (df["hamilton"=="Vasp"])
+        >>> def job_filter_function(df):
+        >>>    return (df["chemicalformula"=="H2"]) & (df["hamilton"=="Vasp"])
 
+        >>> table.db_filter_function = job_filter_function
         """
         return self._db_filter_function
 
     @db_filter_function.setter
     def db_filter_function(self, funct):
         self._db_filter_function = funct
 
     @property
     def filter_function(self):
         """
         Function to filter each job before more expensive functions are applied
+
+        Example:
+
+        >>> def job_filter_function(job):
+        >>>     return (job.status == "finished") & ("murn" in job.job_name)
+
+        >>> table.filter_function = job_filter_function
         """
         return self._filter_function
 
     @filter_function.setter
     def filter_function(self, funct):
         self._filter_function = funct
 
-    def to_hdf(self):
-        file = FileHDFio(file_name=self._project.path + self.name + ".h5", h5_path="/")
-        self.add._to_hdf(file)
-
-    def from_hdf(self):
-        file = FileHDFio(file_name=self._project.path + self.name + ".h5", h5_path="/")
-        self.add._from_hdf(file)
-
-    def save(self, name=None):
-        self._name = name
-        self.to_hdf()
-        self._save_csv()
-
-    def load(self, name=None):
-        self._name = name
-        self.from_hdf()
-        self._load_csv()
-
-    def create_table(
-        self, enforce_update=False, level=3, file=None, job_status_list=None
-    ):
-        skip_table_update = False
-        filter_funct = self.filter_function
-        if job_status_list is None:
-            job_status_list = ["finished"]
-        if self._is_file():
-            if file is None:
-                file = FileHDFio(
-                    file_name=self._project.path + self.name + ".h5", h5_path="/"
-                )
+    def _get_new_functions(self, file: FileHDFio) -> Tuple[List, List]:
+        try:
             (
                 temp_user_function_dict,
                 temp_system_function_dict,
             ) = self._get_data_from_hdf5(hdf=file)
-            job_update_lst = self._collect_job_update_lst(
-                job_status_list=job_status_list,
-                filter_funct=filter_funct,
-                job_stored_ids=self._get_job_ids(),
-            )
-            keys_update_user_lst = [
+            new_user_functions = [
                 key
                 for key in self.add._user_function_dict.keys()
                 if key not in temp_user_function_dict.keys()
             ]
-            keys_update_system_lst = [
+            new_system_functions = [
                 k
                 for k, v in self.add._system_function_dict.items()
                 if v and not temp_system_function_dict[k]
             ]
-            if (
-                len(job_update_lst) == 0
-                and len(keys_update_user_lst) == 0
-                and keys_update_system_lst == 0
-                and not enforce_update
-            ):
-                skip_table_update = True
-        else:
-            job_update_lst = self._collect_job_update_lst(
-                job_status_list=job_status_list,
-                filter_funct=filter_funct,
-                job_stored_ids=None,
-            )
-            keys_update_user_lst, keys_update_system_lst = [], []
-        if not skip_table_update and len(job_update_lst) != 0:
-            df_new_ids = self._iterate_over_job_lst(
-                job_lst=job_update_lst, function_lst=self.add._function_lst, level=level
-            )
-        else:
-            df_new_ids = pandas.DataFrame({})
-        if not skip_table_update and (
-            len(keys_update_user_lst) != 0 or len(keys_update_system_lst) != 0
-        ):
-            job_update_lst = self._collect_job_update_lst(
-                job_status_list=job_status_list,
-                filter_funct=filter_funct,
-                job_stored_ids=None,
-            )
-            function_lst = [
-                v
-                for k, v in self.add._user_function_dict.items()
-                if k in keys_update_system_lst
-            ] + [
-                funct
-                for funct in self.add._system_function_lst
-                if funct.__name__ in keys_update_system_lst
-            ]
-            df_new_keys = self._iterate_over_job_lst(
-                job_lst=job_update_lst, function_lst=function_lst, level=level
-            )
-        else:
-            df_new_keys = pandas.DataFrame({})
-        if len(self._df) > 0 and len(df_new_keys) > 0:
-            self._df = pandas.concat(
-                [self._df, df_new_keys], axis=1, sort=False
-            ).reset_index(drop=True)
-        if len(self._df) > 0 and len(df_new_ids) > 0:
-            self._df = pandas.concat([self._df, df_new_ids], sort=False).reset_index(
-                drop=True
-            )
-        elif len(df_new_ids) > 0:
-            self._df = df_new_ids
+        except:
+            new_user_functions = []
+            new_system_functions = []
+        return new_user_functions, new_system_functions
 
-    def convert_dict(self, input_dict):
-        return {key: self.str_to_value(value) for key, value in input_dict.items()}
+    def create_table(self, file, job_status_list, enforce_update=False):
+        """
+        Create or update the table.
 
-    def refill_dict(self, diff_dict_lst):
-        total_key_lst = self.total_lst_of_keys(diff_dict_lst)
-        for ind, sub_dict in enumerate(diff_dict_lst):
-            for key in total_key_lst:
-                if key not in sub_dict.keys():
-                    sub_dict[key] = self.EMPTY_STR
-                else:
-                    sub_dict[key] = self.str_to_value(sub_dict[key])
+        If this method has been called before and there are new functions added to :attr:`.add`, apply them on the
+        previously analyzed jobs.
+        If this method has been called before and there are new jobs added to :attr:`.analysis_project`, apply all
+        functions to them.
 
-    def col_to_value(self, col_name):
-        val_lst, key_lst, ind_lst = [], [], []
-        for ind, name in enumerate(self._df[col_name]):
-            #             print ('name: ', ind, name)
-            #             if name == self.EMPTY_STR:
-            #                 continue
-            name = name.split("_")
-            ind_lst.append(ind)
-            key_lst.append(name[0])
-            val_lst.append(eval(".".join(name[1:])))
-        if len(set(key_lst)) == 1:
-            key = key_lst[0]
-            self._df[key] = val_lst
-        else:
-            raise ValueError("key not unique: {}".format(set(key_lst)))
+        The result is available via :meth:`.get_dataframe`.
+
+        Args:
+            file (FileHDFio): HDF were the previous state of the table is stored
+            job_status_list (list of str): only consider jobs with these statuses
+            enforce_update (bool): if True always regenerate the table completely.
+        """
+        # if there's new keys, apply the *new* functions to the old jobs and name the resulting table `df_new_keys`
+        # if there's new jobs, apply *all* functions to them and name the resulting table `df_new_ids`
+
+        # if enforce_update is given we recalculate the whole table below anyway, no need to patch up new keys
+        if not enforce_update:
+            new_user_functions, new_system_functions = self._get_new_functions(file)
+
+            if len(new_user_functions) > 0 or len(new_system_functions) > 0:
+                function_lst = [
+                    self.add._user_function_dict[k] for k in new_user_functions
+                ] + [
+                    funct
+                    for funct in self.add._system_function_lst
+                    if funct.__name__ in new_system_functions
+                ]
+                df_new_keys = self._iterate_over_job_lst(
+                    job_lst=map(self._project.inspect, self._get_job_ids()),
+                    function_lst=function_lst,
+                )
+                if len(df_new_keys) > 0:
+                    self._df = pandas.concat([self._df, df_new_keys], axis="columns")
+
+        new_jobs = self._collect_job_update_lst(
+            job_status_list=job_status_list,
+            job_stored_ids=self._get_job_ids() if not enforce_update else None,
+        )
+        if len(new_jobs) > 0:
+            df_new_ids = self._iterate_over_job_lst(
+                job_lst=new_jobs, function_lst=self.add._function_lst
+            )
+            if len(df_new_ids) > 0:
+                self._df = pandas.concat([self._df, df_new_ids], ignore_index=True)
 
     def get_dataframe(self):
         return self._df
 
     def _list_nodes(self):
         return list(self._df.columns)
 
-    def _list_groups(self):
-        return list(set(self._df["col_0"]))
-
-    @staticmethod
-    def str_to_value(input_val):
-        if not isinstance(input_val, str):
-            return input_val
-        else:
-            try:
-                return eval(input_val)
-            except (TypeError, SyntaxError, NameError):
-                return input_val
-
-    @staticmethod
-    def _apply_function_on_job(funct, job):
-        try:
-            return funct(job)
-        except (ValueError, TypeError):
-            return {}
-
-    @staticmethod
-    def total_lst_of_keys(diff_dict_lst):
-        total_key_lst = []
-        for sub_dict in diff_dict_lst:
-            for key in sub_dict.keys():
-                total_key_lst.append(key)
-        return set(total_key_lst)
-
-    def __getitem__(self, item, max_level=5):
-        rename_dict = OrderedDict()
-        if item in self.list_groups():
-            for i in range(1, max_level):
-                rename_dict["col_{}".format(i)] = "col_{}".format(i - 1)
-
-            new_table = PyironTable(
-                project=self._project[item],
-                system_function_lst=self._system_function_lst,
-                csv_file_name=os.path.join(self.working_directory, "pyirontable.csv"),
-            )
-            new_table._df = self._df.drop("col_0", axis=1)
-            new_table._df.rename(index=str, columns=rename_dict, inplace=True)
-            return new_table
+    def __getitem__(self, item):
         if item in self.list_nodes():
             return np.array(self._df[item])
         return None
 
     def __str__(self):
         return self._df.__str__()
 
@@ -406,30 +301,25 @@
         Human readable string representation
 
         Returns:
             str: pandas Dataframe structure as string
         """
         return self._df.__repr__()
 
-    def _is_file(self):
-        return self._project is not None and os.path.isfile(self._file_name_csv)
-
-    def _save_csv(self):
-        self._df.to_csv(self._file_name_csv, index=False)
+    @property
+    def _file_name_csv(self):
+        if self._csv_file is None:
+            return self._project.path + self.name + ".csv"
+        else:
+            return self._csv_file
 
     def _load_csv(self):
+        # Legacy method to read tables written to csv
         self._df = pandas.read_csv(self._file_name_csv)
 
-    def _get_project_list(self, name, pr_len, level=3):
-        lst = [self.EMPTY_STR for _ in range(level)]
-        for i, p in enumerate(name.split("/")[pr_len - 1 : -1]):
-            if len(lst) > i:
-                lst[i] = p
-        return lst
-
     @staticmethod
     def _get_data_from_hdf5(hdf):
         temp_user_function_dict = _from_pickle(hdf=hdf, key="user_function_dict")
         temp_system_function_dict = _from_pickle(hdf=hdf, key="system_function_dict")
         return temp_user_function_dict, temp_system_function_dict
 
     def _get_job_ids(self):
@@ -439,49 +329,86 @@
             return np.array([])
 
     def _get_filtered_job_ids_from_project(self, recursive=True):
         project_table = self._project.job_table(recursive=recursive)
         filter_funct = self.db_filter_function
         return project_table[filter_funct(project_table)]["id"].tolist()
 
-    def _apply_list_of_functions_on_job(self, job, fucntion_lst):
+    @staticmethod
+    def _apply_function_on_job(funct, job):
+        try:
+            return funct(job)
+        except (ValueError, TypeError):
+            return {}
+
+    def _apply_list_of_functions_on_job(self, job, function_lst):
         diff_dict = {}
-        for funct in fucntion_lst:
+        for funct in function_lst:
             funct_dict = self._apply_function_on_job(funct, job)
             for key, value in funct_dict.items():
                 diff_dict[key] = value
         return diff_dict
 
-    def _iterate_over_job_lst(self, job_lst, function_lst, level):
-        pr_len = len(self._project.project_path.split("/"))
+    def _iterate_over_job_lst(self, job_lst: List, function_lst: List) -> List[dict]:
+        """
+        Apply functions to job.
+
+        Any functions that raise an error are set to `None` in the final list.
+
+        Args:
+            job_lst (list of JobPath): all jobs to analyze
+            function_lst (list of functions): all functions to apply on jobs.  Must return a dictionary.
+
+        Returns:
+            list of dict: a list of the merged dicts from all functions for each job
+        """
         diff_dict_lst = []
         for job_inspect in tqdm(job_lst, desc="Processing jobs"):
             if self.convert_to_object:
                 job = job_inspect.to_object()
             else:
                 job = job_inspect
             diff_dict = self._apply_list_of_functions_on_job(
-                job=job, fucntion_lst=function_lst
+                job=job, function_lst=function_lst
             )
-            pr_lst = self._get_project_list(job.project.project_path, pr_len, level)
-            for ic, col in enumerate(pr_lst):
-                diff_dict["col_{}".format(ic)] = col
             diff_dict_lst.append(diff_dict)
         self.refill_dict(diff_dict_lst)
         return pandas.DataFrame(diff_dict_lst)
 
-    def _collect_job_update_lst(
-        self, job_status_list, filter_funct, job_stored_ids=None
-    ):
+    @staticmethod
+    def total_lst_of_keys(diff_dict_lst):
         """
-        Collect jobs to update the pyiron table
+        Get unique list of all keys occuring in list.
+        """
+        total_key_lst = []
+        for sub_dict in diff_dict_lst:
+            for key in sub_dict.keys():
+                total_key_lst.append(key)
+        return set(total_key_lst)
+
+    def refill_dict(self, diff_dict_lst):
+        """
+        Ensure that all dictionaries in the list have the same keys.
+
+        Keys that are not in a dict are set to `None`.
+        """
+        total_key_lst = self.total_lst_of_keys(diff_dict_lst)
+        for sub_dict in diff_dict_lst:
+            for key in total_key_lst:
+                if key not in sub_dict.keys():
+                    sub_dict[key] = None
+
+    def _collect_job_update_lst(self, job_status_list, job_stored_ids=None):
+        """
+        Collect jobs to update the pyiron table.
+
+        Jobs in `job_stored_ids` are ignored.
 
         Args:
             job_status_list (list): List of job status to consider
-            filter_funct (function): Filter function
             job_stored_ids (list/ None): List of already analysed job ids
 
         Returns:
             list: List of JobCore objects
         """
         if job_stored_ids is not None:
             job_id_lst = [
@@ -492,80 +419,153 @@
         else:
             job_id_lst = self._get_filtered_job_ids_from_project()
 
         job_update_lst = []
         for job_id in tqdm(job_id_lst, desc="Loading and filtering jobs"):
             try:
                 job = self._project.inspect(job_id)
-            except IndexError:  # In case the job was deleted while the pyiron table is running
+            except (
+                IndexError
+            ):  # In case the job was deleted while the pyiron table is running
                 job = None
-            if job is not None and job.status in job_status_list and filter_funct(job):
+            if (
+                job is not None
+                and job.status in job_status_list
+                and self.filter_function(job)
+            ):
                 job_update_lst.append(job)
         return job_update_lst
 
     def _repr_html_(self):
         """
         Internal helper function to represent the GenericParameters object within the Jupyter Framework
 
         Returns:
             HTML: Jupyter HTML object
         """
         return self._df._repr_html_()
 
 
 class TableJob(GenericJob):
+    """
+
+    Since a project can have a large number of jobs, it is often necessary
+    to “filter” the data to extract useful information. PyironTable is a tool
+    that allows the user to do this efficiently.
+
+    Example:
+
+    >>> # Prepare random data
+    >>> for T in T_range:
+    >>>     lmp = pr.create.job.Lammps(('lmp', T))
+    >>>     lmp.structure = pr.create.structure.bulk('Ni', cubic=True).repeat(5)
+    >>>     lmp.calc_md(temperature=T)
+    >>>     lmp.run()
+
+    >>> def db_filter_function(job_table):
+    >>>     return (job_table.status == "finished") & (job_table.hamilton == "Lammps")
+
+    >>> def get_energy(job):
+    >>>     return job["output/generic/energy_pot"][-1]
+
+    >>> def get_temperature(job):
+    >>>     return job['output/generic/temperature'][-1]
+
+    >>> table.db_filter_function = db_filter_function
+
+    >>> table.add["energy"] = get_energy
+    >>> table.add["temperature"] = get_temperature
+    >>> table.run()
+    >>> table.get_dataframe()
+
+    This returns a dataframe containing job-id, energy and temperature.
+
+    Alternatively, the filter function can be applied on the job
+
+    >>> def job_filter_function(job):
+    >>>     return (job.status == "finished") & ("lmp" in job.job_name)
+
+    >>> table.filter_function = job_filter_function
+
+    """
+
+    _system_function_lst = [get_job_id]
+
     def __init__(self, project, job_name):
         super(TableJob, self).__init__(project, job_name)
         self.__version__ = "0.1"
         self.__hdf_version__ = "0.3.0"
-        self.__name__ = "TableJob"
         self._analysis_project = None
-        self._system_function_lst = [get_job_id]
         self._pyiron_table = PyironTable(
             project=None,
             system_function_lst=self._system_function_lst,
             csv_file_name=os.path.join(self.working_directory, "pyirontable.csv"),
         )
         self._enforce_update = False
-        self._project_level = 0
+        self._job_status = ["finished"]
+        self._python_only_job = True
         self.analysis_project = project.project
 
     @property
     def filter(self):
         return self._pyiron_table.filter
 
     @property
-    def project_level(self):
-        return self._project_level
-
-    @project_level.setter
-    def project_level(self, level):
-        self._project_level = level
-
-    @property
     def db_filter_function(self):
+        """
+        function: database level filter function
+
+        The function should accept a dataframe, the job table of :attr:`~.analysis_project` and return a bool index into
+        it.  Jobs where the index is `False` are excluced from the analysis.
+        """
         return self._pyiron_table.db_filter_function
 
     @db_filter_function.setter
     def db_filter_function(self, funct):
         self._pyiron_table.db_filter_function = funct
 
     @property
     def filter_function(self):
+        """
+        function: job level filter function
+
+        The function should accept a GenericJob or JobCore object and return a bool, if it returns `False` the job is
+        excluced from the analysis.
+        """
         return self._pyiron_table.filter_function
 
     @filter_function.setter
     def filter_function(self, funct):
         self._pyiron_table.filter_function = funct
 
     @property
+    def job_status(self):
+        """
+        list of str: only jobs with status in this list are included in the table.
+        """
+        return self._job_status
+
+    @job_status.setter
+    def job_status(self, status):
+        if isinstance(status, str):
+            status = [status]
+        for s in status:
+            valid = jobstatus.job_status_lst
+            if s not in valid:
+                raise ValueError(
+                    f"'{s}' not a valid job status! Must be one of {valid}."
+                )
+        self._job_status = status
+
+    @property
     def pyiron_table(self):
         return self._pyiron_table
 
     @property
+    @deprecate("Use analysis_project instead!")
     def ref_project(self):
         return self.analysis_project
 
     @ref_project.setter
     def ref_project(self, project):
         self.analysis_project = project
 
@@ -585,26 +585,42 @@
             project=self._analysis_project,
             system_function_lst=self._system_function_lst,
             csv_file_name=os.path.join(self.working_directory, "pyirontable.csv"),
         )
 
     @property
     def add(self):
+        """
+        Add a function to analyse job data
+
+        Example:
+
+        >>> def get_energy(job):
+        >>>     return job["output/generic/energy_pot"][-1]
+
+        >>> table.add["energy"] = get_energy
+        """
         return self._pyiron_table.add
 
     @property
     def convert_to_object(self):
+        """
+        bool: if `True` convert fully load jobs before passing them to functions, if `False` use inspect mode.
+        """
         return self._pyiron_table.convert_to_object
 
     @convert_to_object.setter
     def convert_to_object(self, conv_to_obj):
         self._pyiron_table.convert_to_object = conv_to_obj
 
     @property
     def enforce_update(self):
+        """
+        bool: if `True` re-evaluate all function on all jobs when :meth:`.update_table` is called.
+        """
         return self._enforce_update
 
     @enforce_update.setter
     def enforce_update(self, enforce):
         if isinstance(enforce, bool):
             if enforce:
                 self._enforce_update = True
@@ -726,43 +742,46 @@
 
     def run_static(self):
         self._create_working_directory()
         self.status.running = True
         self.update_table()
         self.status.finished = True
 
+    @deprecate(job_status_list="Use TableJob.job_status instead!")
     def update_table(self, job_status_list=None):
         """
-        Update the pyiron table object, add new columns if a new function was added or add new rows for new jobs
+        Update the pyiron table object, add new columns if a new function was added or add new rows for new jobs.
+
+        By default this function does not recompute already evaluated functions on already existing jobs.  To force a
+        complete re-evaluation set :attr:`~.enforce_update` to `True`.
 
         Args:
-            job_status_list (list/None): List of job status which are added to the table by default ["finished"]
+            job_status_list (list/None): List of job status which are added to the table by default ["finished"].
+                                         Deprecated, use :attr:`.job_status` instead!
         """
         if job_status_list is None:
-            job_status_list = ["finished"]
-        self.project.db.item_update({"timestart": datetime.now()}, self.job_id)
+            job_status_list = self.job_status
+        if self.job_id is not None:
+            self.project.db.item_update({"timestart": datetime.now()}, self.job_id)
         with self.project_hdf5.open("input") as hdf5_input:
             self._pyiron_table.create_table(
-                enforce_update=self._enforce_update,
                 file=hdf5_input,
-                level=self._project_level,
                 job_status_list=job_status_list,
+                enforce_update=self._enforce_update,
             )
         self.to_hdf()
         self._pyiron_table._df.to_csv(
             os.path.join(self.working_directory, "pyirontable.csv"), index=False
         )
         self._save_output()
-        self.project.db.item_update(self._runtime(), self.job_id)
-
-    def write_input(self):
-        pass
+        self.run_time_to_db()
 
     def get_dataframe(self):
         """
+        Returns aggregated results over all jobs.
 
         Returns:
             pandas.Dataframe
         """
         return self.pyiron_table._df
```

### Comparing `pyiron_base-0.5.9/pyiron_base/toolkit.py` & `pyiron_base-0.6.0/pyiron_base/jobs/job/toolkit.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 Builtin tools that come with pyiron base.
 """
 
 from abc import ABC
-from pyiron_base.job.factory import JobFactory
+from pyiron_base.jobs.job.factory import JobFactory
 
 __author__ = "Liam Huber"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
```

### Comparing `pyiron_base-0.5.9/pyiron_base.egg-info/PKG-INFO` & `pyiron_base-0.6.0/pyiron_base.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pyiron-base
-Version: 0.5.9
+Version: 0.6.0
 Summary: pyiron_base - an integrated development environment (IDE) for computational science.
 Home-page: https://github.com/pyiron/pyiron_base
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
 http://pyiron.org
-
```

### Comparing `pyiron_base-0.5.9/pyiron_base.egg-info/SOURCES.txt` & `pyiron_base-0.6.0/pyiron_base.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -3,98 +3,111 @@
 README.rst
 setup.cfg
 setup.py
 versioneer.py
 pyiron_base/__init__.py
 pyiron_base/_tests.py
 pyiron_base/_version.py
-pyiron_base/toolkit.py
 pyiron_base.egg-info/PKG-INFO
 pyiron_base.egg-info/SOURCES.txt
 pyiron_base.egg-info/dependency_links.txt
 pyiron_base.egg-info/entry_points.txt
 pyiron_base.egg-info/requires.txt
 pyiron_base.egg-info/top_level.txt
-pyiron_base/archiving/__init__.py
-pyiron_base/archiving/export_archive.py
-pyiron_base/archiving/import_archive.py
 pyiron_base/cli/__init__.py
 pyiron_base/cli/__main__.py
+pyiron_base/cli/control.py
 pyiron_base/cli/install.py
 pyiron_base/cli/ls.py
 pyiron_base/cli/reloadfile.py
 pyiron_base/cli/rm.py
 pyiron_base/cli/wrapper.py
 pyiron_base/database/__init__.py
 pyiron_base/database/filetable.py
 pyiron_base/database/generic.py
 pyiron_base/database/jobtable.py
 pyiron_base/database/manager.py
 pyiron_base/database/performance.py
 pyiron_base/database/tables.py
-pyiron_base/generic/__init__.py
-pyiron_base/generic/datacontainer.py
-pyiron_base/generic/dynamic.py
-pyiron_base/generic/factory.py
-pyiron_base/generic/filedata.py
-pyiron_base/generic/fileio.py
-pyiron_base/generic/flattenedstorage.py
-pyiron_base/generic/hdfio.py
-pyiron_base/generic/hdfstub.py
-pyiron_base/generic/inputlist.py
-pyiron_base/generic/jedi.py
-pyiron_base/generic/object.py
-pyiron_base/generic/parameters.py
-pyiron_base/generic/units.py
-pyiron_base/generic/util.py
 pyiron_base/interfaces/__init__.py
+pyiron_base/interfaces/factory.py
 pyiron_base/interfaces/has_groups.py
 pyiron_base/interfaces/has_hdf.py
-pyiron_base/job/__init__.py
-pyiron_base/job/core.py
-pyiron_base/job/executable.py
-pyiron_base/job/external.py
-pyiron_base/job/factory.py
-pyiron_base/job/generic.py
-pyiron_base/job/interactive.py
-pyiron_base/job/interactivewrapper.py
-pyiron_base/job/jobstatus.py
-pyiron_base/job/jobtype.py
-pyiron_base/job/path.py
-pyiron_base/job/script.py
-pyiron_base/job/template.py
-pyiron_base/job/util.py
-pyiron_base/job/worker.py
-pyiron_base/job/wrapper.py
-pyiron_base/master/__init__.py
-pyiron_base/master/flexible.py
-pyiron_base/master/generic.py
-pyiron_base/master/list.py
-pyiron_base/master/parallel.py
-pyiron_base/master/serial.py
-pyiron_base/master/submissionstatus.py
+pyiron_base/interfaces/object.py
+pyiron_base/interfaces/singleton.py
+pyiron_base/jobs/__init__.py
+pyiron_base/jobs/datamining.py
+pyiron_base/jobs/dynamic.py
+pyiron_base/jobs/script.py
+pyiron_base/jobs/worker.py
+pyiron_base/jobs/job/__init__.py
+pyiron_base/jobs/job/core.py
+pyiron_base/jobs/job/factory.py
+pyiron_base/jobs/job/generic.py
+pyiron_base/jobs/job/interactive.py
+pyiron_base/jobs/job/jobtype.py
+pyiron_base/jobs/job/path.py
+pyiron_base/jobs/job/runfunction.py
+pyiron_base/jobs/job/template.py
+pyiron_base/jobs/job/toolkit.py
+pyiron_base/jobs/job/util.py
+pyiron_base/jobs/job/wrapper.py
+pyiron_base/jobs/job/extension/__init__.py
+pyiron_base/jobs/job/extension/executable.py
+pyiron_base/jobs/job/extension/jobstatus.py
+pyiron_base/jobs/job/extension/server/__init__.py
+pyiron_base/jobs/job/extension/server/generic.py
+pyiron_base/jobs/job/extension/server/queuestatus.py
+pyiron_base/jobs/job/extension/server/runmode.py
+pyiron_base/jobs/master/__init__.py
+pyiron_base/jobs/master/flexible.py
+pyiron_base/jobs/master/generic.py
+pyiron_base/jobs/master/interactivewrapper.py
+pyiron_base/jobs/master/list.py
+pyiron_base/jobs/master/parallel.py
+pyiron_base/jobs/master/serial.py
+pyiron_base/jobs/master/submissionstatus.py
 pyiron_base/project/__init__.py
 pyiron_base/project/data.py
+pyiron_base/project/external.py
 pyiron_base/project/generic.py
 pyiron_base/project/gui.py
 pyiron_base/project/maintenance.py
 pyiron_base/project/path.py
+pyiron_base/project/archiving/__init__.py
+pyiron_base/project/archiving/export_archive.py
+pyiron_base/project/archiving/import_archive.py
+pyiron_base/project/archiving/shared.py
 pyiron_base/project/update/__init__.py
 pyiron_base/project/update/pyiron_base_03x_to_04x.py
-pyiron_base/pyio/__init__.py
-pyiron_base/pyio/parser.py
-pyiron_base/server/__init__.py
-pyiron_base/server/generic.py
-pyiron_base/server/queuestatus.py
-pyiron_base/server/runmode.py
 pyiron_base/state/__init__.py
 pyiron_base/state/install.py
 pyiron_base/state/logger.py
 pyiron_base/state/publications.py
 pyiron_base/state/queue_adapter.py
 pyiron_base/state/settings.py
+pyiron_base/state/signal.py
 pyiron_base/state/update.py
-pyiron_base/table/__init__.py
-pyiron_base/table/datamining.py
+pyiron_base/storage/__init__.py
+pyiron_base/storage/datacontainer.py
+pyiron_base/storage/filedata.py
+pyiron_base/storage/fileio.py
+pyiron_base/storage/flattenedstorage.py
+pyiron_base/storage/has_stored_traits.py
+pyiron_base/storage/hdfio.py
+pyiron_base/storage/hdfstub.py
+pyiron_base/storage/helper_functions.py
+pyiron_base/storage/inputlist.py
+pyiron_base/storage/parameters.py
+pyiron_base/utils/__init__.py
+pyiron_base/utils/deprecate.py
+pyiron_base/utils/error.py
+pyiron_base/utils/instance.py
+pyiron_base/utils/jedi.py
+pyiron_base/utils/parser.py
+pyiron_base/utils/safetar.py
+pyiron_base/utils/units.py
 test_benchmarks/__init__.py
 test_benchmarks/generic/__init__.py
-test_benchmarks/generic/test_filehdfio.py
+test_benchmarks/generic/test_filehdfio.py
+tests/test_testwithproject.py
+tests/test_toolkit.py
```

### Comparing `pyiron_base-0.5.9/setup.py` & `pyiron_base-0.6.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,37 +18,39 @@
     classifiers=['Development Status :: 5 - Production/Stable',
                  'Topic :: Scientific/Engineering :: Physics',
                  'License :: OSI Approved :: BSD License',
                  'Intended Audience :: Science/Research',
                  'Operating System :: OS Independent',
                  'Programming Language :: Python :: 3.8',
                  'Programming Language :: Python :: 3.9',
-                 'Programming Language :: Python :: 3.10'
+                 'Programming Language :: Python :: 3.10',
+                 'Programming Language :: Python :: 3.11'
                 ],
 
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*", "*docs*", "*binder*", "*conda*", "*notebooks*", "*.ci_support*"]),
     install_requires=[
-        'dill>=0.3.4',
-        'future>=0.18.2',
-        'gitpython>=3.1.27',
+        'dill>=0.3.6',
+        'future>=0.18.3',
+        'gitpython>=3.1.31',
         'h5io>=0.1.7',
-        'h5py>=3.6.0',
-        'numpy>=1.22.3',
-        'pandas>=1.4.1',
+        'h5py>=3.8.0',
+        'numpy>=1.24.3',
+        'pandas>=2.0.2',
         'pathlib2>=2.3.7.post1',
-        'pint>=0.18',
-        'psutil>=5.9.0',
-        'pyfileindex>=0.0.6',
-        'pysqa>=0.0.16',
-        'sqlalchemy>=1.4.32',
-        'tables>=3.7.0',
-        'tqdm>=4.63.1'
+        'pint>=0.22',
+        'psutil>=5.9.5',
+        'pyfileindex>=0.0.11',
+        'pysqa>=0.0.25',
+        'sqlalchemy>=2.0.15',
+        'tables>=3.8.0',
+        'tqdm>=4.65.0',
+        'traitlets>=5.9.0',
     ],
     cmdclass=versioneer.get_cmdclass(),
 
-    entry_points = {
+    entry_points={
             "console_scripts": [
                 'pyiron=pyiron_base.cli:main'
             ]
     }
     )
```

### Comparing `pyiron_base-0.5.9/test_benchmarks/generic/test_filehdfio.py` & `pyiron_base-0.6.0/test_benchmarks/generic/test_filehdfio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.5.9/versioneer.py` & `pyiron_base-0.6.0/versioneer.py`

 * *Files identical despite different names*

