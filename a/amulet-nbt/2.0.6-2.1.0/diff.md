# Comparing `tmp/amulet-nbt-2.0.6.tar.gz` & `tmp/amulet-nbt-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amulet-nbt-2.0.6.tar", last modified: Sat Jun  3 09:59:48 2023, max compression
+gzip compressed data, was "amulet-nbt-2.1.0.tar", last modified: Thu Jun  8 12:35:52 2023, max compression
```

## Comparing `amulet-nbt-2.0.6.tar` & `amulet-nbt-2.1.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 09:59:48.572844 amulet-nbt-2.0.6/
--rw-rw-rw-   0        0        0     6954 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/LICENSE
--rw-rw-rw-   0        0        0       53 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1523 2023-06-03 09:59:48.572844 amulet-nbt-2.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1058 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 09:59:48.572844 amulet-nbt-2.0.6/amulet_nbt/
--rw-rw-rw-   0        0        0      690 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/__init__.pxd
--rw-rw-rw-   0        0        0     3569 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 09:59:48.572844 amulet-nbt-2.0.6/amulet_nbt/__pyinstaller/
--rw-rw-rw-   0        0        0       43 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0      192 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/__pyinstaller/hook-amulet_nbt.py
--rw-rw-rw-   0        0        0  1725073 2023-06-03 09:59:44.000000 amulet-nbt-2.0.6/amulet_nbt/_array.c
--rw-rw-rw-   0        0        0      690 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_array.pxd
--rw-rw-rw-   0        0        0      501 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_array.pyi
--rw-rw-rw-   0        0        0    39431 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_array.pyx
--rw-rw-rw-   0        0        0  1231947 2023-06-03 09:59:44.000000 amulet-nbt-2.0.6/amulet_nbt/_compound.c
--rw-rw-rw-   0        0        0     2339 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_compound.pxd
--rw-rw-rw-   0        0        0     2829 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_compound.pyi
--rw-rw-rw-   0        0        0    25306 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_compound.pyx
--rw-rw-rw-   0        0        0   161775 2023-06-03 09:59:44.000000 amulet-nbt-2.0.6/amulet_nbt/_const.c
--rw-rw-rw-   0        0        0      336 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_const.pxd
--rw-rw-rw-   0        0        0      411 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_const.pyx
--rw-rw-rw-   0        0        0     1060 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_dtype.py
--rw-rw-rw-   0        0        0   269156 2023-06-03 09:59:44.000000 amulet-nbt-2.0.6/amulet_nbt/_errors.c
--rw-rw-rw-   0        0        0      583 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_errors.pyx
--rw-rw-rw-   0        0        0  1199885 2023-06-03 09:59:44.000000 amulet-nbt-2.0.6/amulet_nbt/_float.c
--rw-rw-rw-   0        0        0      442 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_float.pxd
--rw-rw-rw-   0        0        0      332 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_float.pyi
--rw-rw-rw-   0        0        0    28250 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_float.pyx
--rw-rw-rw-   0        0        0  1897880 2023-06-03 09:59:45.000000 amulet-nbt-2.0.6/amulet_nbt/_int.c
--rw-rw-rw-   0        0        0      898 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_int.pxd
--rw-rw-rw-   0        0        0      395 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_int.pyi
--rw-rw-rw-   0        0        0    51955 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_int.pyx
--rw-rw-rw-   0        0        0   855724 2023-06-03 09:59:45.000000 amulet-nbt-2.0.6/amulet_nbt/_list.c
--rw-rw-rw-   0        0        0     1383 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_list.pxd
--rw-rw-rw-   0        0        0     1515 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_list.pyi
--rw-rw-rw-   0        0        0    11388 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_list.pyx
--rw-rw-rw-   0        0        0   684400 2023-06-03 09:59:46.000000 amulet-nbt-2.0.6/amulet_nbt/_load_nbt.c
--rw-rw-rw-   0        0        0      378 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_load_nbt.pxd
--rw-rw-rw-   0        0        0      763 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_load_nbt.pyi
--rw-rw-rw-   0        0        0     7233 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_load_nbt.pyx
--rw-rw-rw-   0        0        0   627681 2023-06-03 09:59:46.000000 amulet-nbt-2.0.6/amulet_nbt/_load_snbt.c
--rw-rw-rw-   0        0        0       87 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_load_snbt.pxd
--rw-rw-rw-   0        0        0       71 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_load_snbt.pyi
--rw-rw-rw-   0        0        0     7822 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_load_snbt.pyx
--rw-rw-rw-   0        0        0   849642 2023-06-03 09:59:46.000000 amulet-nbt-2.0.6/amulet_nbt/_named_tag.c
--rw-rw-rw-   0        0        0      155 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_named_tag.pxd
--rw-rw-rw-   0        0        0     1652 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_named_tag.pyi
--rw-rw-rw-   0        0        0     9560 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_named_tag.pyx
--rw-rw-rw-   0        0        0   343411 2023-06-03 09:59:46.000000 amulet-nbt-2.0.6/amulet_nbt/_numeric.c
--rw-rw-rw-   0        0        0      121 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_numeric.pxd
--rw-rw-rw-   0        0        0      309 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_numeric.pyi
--rw-rw-rw-   0        0        0      356 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_numeric.pyx
--rw-rw-rw-   0        0        0   470527 2023-06-03 09:59:46.000000 amulet-nbt-2.0.6/amulet_nbt/_string.c
--rw-rw-rw-   0        0        0      294 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_string.pxd
--rw-rw-rw-   0        0        0      645 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_string.pyi
--rw-rw-rw-   0        0        0     6510 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_string.pyx
--rw-rw-rw-   0        0        0   510600 2023-06-03 09:59:46.000000 amulet-nbt-2.0.6/amulet_nbt/_util.c
--rw-rw-rw-   0        0        0     1498 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_util.pxd
--rw-rw-rw-   0        0        0      174 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_util.pyi
--rw-rw-rw-   0        0        0     5467 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_util.pyx
--rw-rw-rw-   0        0        0   585600 2023-06-03 09:59:47.000000 amulet-nbt-2.0.6/amulet_nbt/_value.c
--rw-rw-rw-   0        0        0      835 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_value.pxd
--rw-rw-rw-   0        0        0     1770 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_value.pyi
--rw-rw-rw-   0        0        0     8646 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/_value.pyx
--rw-rw-rw-   0        0        0      518 2023-06-03 09:59:48.572844 amulet-nbt-2.0.6/amulet_nbt/_version.py
--rw-rw-rw-   0        0        0        0 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/amulet_nbt/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-03 09:59:48.572844 amulet-nbt-2.0.6/amulet_nbt.egg-info/
--rw-rw-rw-   0        0        0     1523 2023-06-03 09:59:48.000000 amulet-nbt-2.0.6/amulet_nbt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2023-06-03 09:59:48.000000 amulet-nbt-2.0.6/amulet_nbt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 09:59:48.000000 amulet-nbt-2.0.6/amulet_nbt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-03 09:59:48.000000 amulet-nbt-2.0.6/amulet_nbt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-03 09:59:47.000000 amulet-nbt-2.0.6/amulet_nbt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      155 2023-06-03 09:59:48.000000 amulet-nbt-2.0.6/amulet_nbt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-03 09:59:48.000000 amulet-nbt-2.0.6/amulet_nbt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      195 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/pyproject.toml
--rw-rw-rw-   0        0        0     1134 2023-06-03 09:59:48.572844 amulet-nbt-2.0.6/setup.cfg
--rw-rw-rw-   0        0        0      382 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 09:59:48.572844 amulet-nbt-2.0.6/tests/
--rw-rw-rw-   0        0        0      980 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/tests/test_legacy.py
--rw-rw-rw-   0        0        0     6522 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/tests/test_massive_nbt.py
--rw-rw-rw-   0        0        0     2246 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/tests/test_nbt.py
--rw-rw-rw-   0        0        0      674 2023-06-03 09:59:03.000000 amulet-nbt-2.0.6/tests/test_tempita.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:35:52.864419 amulet-nbt-2.1.0/
+-rw-rw-rw-   0        0        0     6954 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0       53 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1523 2023-06-08 12:35:52.864419 amulet-nbt-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1058 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 12:35:52.864419 amulet-nbt-2.1.0/amulet_nbt/
+-rw-rw-rw-   0        0        0      690 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/__init__.pxd
+-rw-rw-rw-   0        0        0     3582 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:35:52.848795 amulet-nbt-2.1.0/amulet_nbt/__pyinstaller/
+-rw-rw-rw-   0        0        0       43 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0      192 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/__pyinstaller/hook-amulet_nbt.py
+-rw-rw-rw-   0        0        0  1725073 2023-06-08 12:35:46.000000 amulet-nbt-2.1.0/amulet_nbt/_array.c
+-rw-rw-rw-   0        0        0      690 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_array.pxd
+-rw-rw-rw-   0        0        0      501 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_array.pyi
+-rw-rw-rw-   0        0        0    39431 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_array.pyx
+-rw-rw-rw-   0        0        0  1231947 2023-06-08 12:35:46.000000 amulet-nbt-2.1.0/amulet_nbt/_compound.c
+-rw-rw-rw-   0        0        0     2339 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_compound.pxd
+-rw-rw-rw-   0        0        0     2829 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_compound.pyi
+-rw-rw-rw-   0        0        0    25306 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_compound.pyx
+-rw-rw-rw-   0        0        0   161775 2023-06-08 12:35:46.000000 amulet-nbt-2.1.0/amulet_nbt/_const.c
+-rw-rw-rw-   0        0        0      336 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_const.pxd
+-rw-rw-rw-   0        0        0      411 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_const.pyx
+-rw-rw-rw-   0        0        0     1060 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_dtype.py
+-rw-rw-rw-   0        0        0   269156 2023-06-08 12:35:46.000000 amulet-nbt-2.1.0/amulet_nbt/_errors.c
+-rw-rw-rw-   0        0        0      583 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_errors.pyx
+-rw-rw-rw-   0        0        0  1199885 2023-06-08 12:35:47.000000 amulet-nbt-2.1.0/amulet_nbt/_float.c
+-rw-rw-rw-   0        0        0      442 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_float.pxd
+-rw-rw-rw-   0        0        0      332 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_float.pyi
+-rw-rw-rw-   0        0        0    28250 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_float.pyx
+-rw-rw-rw-   0        0        0  1897880 2023-06-08 12:35:47.000000 amulet-nbt-2.1.0/amulet_nbt/_int.c
+-rw-rw-rw-   0        0        0      898 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_int.pxd
+-rw-rw-rw-   0        0        0      395 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_int.pyi
+-rw-rw-rw-   0        0        0    51955 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_int.pyx
+-rw-rw-rw-   0        0        0   855724 2023-06-08 12:35:48.000000 amulet-nbt-2.1.0/amulet_nbt/_list.c
+-rw-rw-rw-   0        0        0     1383 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_list.pxd
+-rw-rw-rw-   0        0        0     1515 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_list.pyi
+-rw-rw-rw-   0        0        0    11388 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_list.pyx
+-rw-rw-rw-   0        0        0   703719 2023-06-08 12:35:48.000000 amulet-nbt-2.1.0/amulet_nbt/_load_nbt.c
+-rw-rw-rw-   0        0        0      378 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_load_nbt.pxd
+-rw-rw-rw-   0        0        0     2342 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_load_nbt.pyi
+-rw-rw-rw-   0        0        0     7876 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_load_nbt.pyx
+-rw-rw-rw-   0        0        0   627681 2023-06-08 12:35:49.000000 amulet-nbt-2.1.0/amulet_nbt/_load_snbt.c
+-rw-rw-rw-   0        0        0       87 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_load_snbt.pxd
+-rw-rw-rw-   0        0        0       71 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_load_snbt.pyi
+-rw-rw-rw-   0        0        0     7822 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_load_snbt.pyx
+-rw-rw-rw-   0        0        0   849642 2023-06-08 12:35:49.000000 amulet-nbt-2.1.0/amulet_nbt/_named_tag.c
+-rw-rw-rw-   0        0        0      155 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_named_tag.pxd
+-rw-rw-rw-   0        0        0     1652 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_named_tag.pyi
+-rw-rw-rw-   0        0        0     9560 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_named_tag.pyx
+-rw-rw-rw-   0        0        0   343411 2023-06-08 12:35:49.000000 amulet-nbt-2.1.0/amulet_nbt/_numeric.c
+-rw-rw-rw-   0        0        0      121 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_numeric.pxd
+-rw-rw-rw-   0        0        0      309 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_numeric.pyi
+-rw-rw-rw-   0        0        0      356 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_numeric.pyx
+-rw-rw-rw-   0        0        0   470527 2023-06-08 12:35:50.000000 amulet-nbt-2.1.0/amulet_nbt/_string.c
+-rw-rw-rw-   0        0        0      294 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_string.pxd
+-rw-rw-rw-   0        0        0      645 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_string.pyi
+-rw-rw-rw-   0        0        0     6510 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_string.pyx
+-rw-rw-rw-   0        0        0   510600 2023-06-08 12:35:50.000000 amulet-nbt-2.1.0/amulet_nbt/_util.c
+-rw-rw-rw-   0        0        0     1498 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_util.pxd
+-rw-rw-rw-   0        0        0      174 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_util.pyi
+-rw-rw-rw-   0        0        0     5467 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_util.pyx
+-rw-rw-rw-   0        0        0   585600 2023-06-08 12:35:50.000000 amulet-nbt-2.1.0/amulet_nbt/_value.c
+-rw-rw-rw-   0        0        0      835 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_value.pxd
+-rw-rw-rw-   0        0        0     1770 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_value.pyi
+-rw-rw-rw-   0        0        0     8646 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/_value.pyx
+-rw-rw-rw-   0        0        0      518 2023-06-08 12:35:52.864419 amulet-nbt-2.1.0/amulet_nbt/_version.py
+-rw-rw-rw-   0        0        0        0 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/amulet_nbt/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-08 12:35:52.848795 amulet-nbt-2.1.0/amulet_nbt.egg-info/
+-rw-rw-rw-   0        0        0     1523 2023-06-08 12:35:52.000000 amulet-nbt-2.1.0/amulet_nbt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1773 2023-06-08 12:35:52.000000 amulet-nbt-2.1.0/amulet_nbt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 12:35:52.000000 amulet-nbt-2.1.0/amulet_nbt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-08 12:35:52.000000 amulet-nbt-2.1.0/amulet_nbt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-08 12:35:50.000000 amulet-nbt-2.1.0/amulet_nbt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      155 2023-06-08 12:35:52.000000 amulet-nbt-2.1.0/amulet_nbt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-08 12:35:52.000000 amulet-nbt-2.1.0/amulet_nbt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      195 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1134 2023-06-08 12:35:52.864419 amulet-nbt-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      382 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:35:52.864419 amulet-nbt-2.1.0/tests/
+-rw-rw-rw-   0        0        0      980 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/tests/test_legacy.py
+-rw-rw-rw-   0        0        0     6522 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/tests/test_massive_nbt.py
+-rw-rw-rw-   0        0        0     2246 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/tests/test_nbt.py
+-rw-rw-rw-   0        0        0      674 2023-06-08 12:34:41.000000 amulet-nbt-2.1.0/tests/test_tempita.py
```

### Comparing `amulet-nbt-2.0.6/LICENSE` & `amulet-nbt-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/PKG-INFO` & `amulet-nbt-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amulet-nbt
-Version: 2.0.6
+Version: 2.1.0
 Summary: Read and write Minecraft NBT and SNBT data.
 Home-page: https://www.amuletmc.com
 Author: James Clare, Ben Gothard
 Author-email: amuleteditor@gmail.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `amulet-nbt-2.0.6/README.md` & `amulet-nbt-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/__init__.pxd` & `amulet-nbt-2.1.0/amulet_nbt/__init__.pxd`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/__init__.py` & `amulet-nbt-2.1.0/amulet_nbt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     "ListTag",
     "ListTag",
     "TAG_List",
     "CompoundTag",
     "CompoundTag",
     "TAG_Compound",
     "load",
-    "load_many",
+    "load_array",
     "ReadContext",
     "from_snbt",
     "NBTError",
     "NBTLoadError",
     "NBTFormatError",
     "SNBTParseError",
     "SNBTType",
@@ -119,15 +119,15 @@
 )
 from ._compound import (
     CompoundTag,
     CompoundTag as TAG_Compound,
 )
 
 # Load functions
-from ._load_nbt import load, load_many, ReadContext
+from ._load_nbt import load, load_many, load_array, ReadContext
 from ._load_snbt import from_snbt
 
 from ._errors import NBTError, NBTLoadError, NBTFormatError, SNBTParseError
 
 from ._dtype import SNBTType, IntType, FloatType, NumberType, ArrayType, AnyNBT
 
 from ._util import utf8_decoder, utf8_encoder, utf8_escape_decoder, utf8_escape_encoder
```

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_array.c` & `amulet-nbt-2.1.0/amulet_nbt/_array.c`

 * *Files 0% similar despite different names*

```diff
@@ -1384,195 +1384,195 @@
   "type.pxd",
   "amulet_nbt\\\\_value.pxd",
   "amulet_nbt\\\\_util.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* #### Code section: numeric_typedefs ### */
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":731
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":731
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":732
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":732
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":733
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":734
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":738
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":738
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":739
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":739
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":740
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":741
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":745
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":745
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":746
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":746
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":755
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":755
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":756
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":756
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":757
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":759
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":759
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":760
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":760
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":761
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":761
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":763
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":764
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":766
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":766
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":767
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":767
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":768
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":768
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1610,42 +1610,42 @@
 struct __pyx_obj_10amulet_nbt_6_value_AbstractBaseMutableTag;
 struct __pyx_obj_10amulet_nbt_5_util_BufferContext;
 struct __pyx_obj_10amulet_nbt_6_array_AbstractBaseArrayTag;
 struct __pyx_obj_10amulet_nbt_6_array_ByteArrayTag;
 struct __pyx_obj_10amulet_nbt_6_array_IntArrayTag;
 struct __pyx_obj_10amulet_nbt_6_array_LongArrayTag;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":770
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":770
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":771
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":772
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":774
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":774
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -4883,261 +4883,261 @@
 #define __pyx_codeobj__125 __pyx_mstate_global->__pyx_codeobj__125
 #define __pyx_codeobj__126 __pyx_mstate_global->__pyx_codeobj__126
 #define __pyx_codeobj__127 __pyx_mstate_global->__pyx_codeobj__127
 #define __pyx_codeobj__128 __pyx_mstate_global->__pyx_codeobj__128
 #define __pyx_codeobj__130 __pyx_mstate_global->__pyx_codeobj__130
 /* #### Code section: module_code ### */
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":245
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":251
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":257
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":263
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":271
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":278
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":284
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":776
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5146,29 +5146,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5179,15 +5179,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":779
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5196,29 +5196,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5229,15 +5229,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":782
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5246,29 +5246,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5279,15 +5279,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":785
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5296,29 +5296,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5329,15 +5329,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":788
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5346,29 +5346,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5379,212 +5379,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":791
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":793
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":792
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":795
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":795
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":791
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":970
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":971
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":972
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":974
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":975
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":977
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":976
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":978
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":978
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":982
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5600,15 +5600,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5616,68 +5616,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":984
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 984, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":985
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":985
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 985, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 986, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 986, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5685,15 +5685,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":982
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5708,15 +5708,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":988
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5732,15 +5732,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5748,68 +5748,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":990
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 990, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":991
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":991
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 991, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 992, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 992, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5817,15 +5817,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":988
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5840,15 +5840,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":994
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5864,15 +5864,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5880,68 +5880,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":996
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 996, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":997
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":997
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 997, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":998
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":998
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 998, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 998, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5949,15 +5949,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":994
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5972,176 +5972,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1001
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1013
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1001
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1016
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1028
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1016
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1031
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1038
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1031
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1041
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1045
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1041
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1048
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1052
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1052
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1048
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -29871,26 +29871,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 986, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 992, __pyx_L1_error)
```

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_array.pxd` & `amulet-nbt-2.1.0/amulet_nbt/_array.pxd`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_array.pyx` & `amulet-nbt-2.1.0/amulet_nbt/_array.pyx`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_compound.c` & `amulet-nbt-2.1.0/amulet_nbt/_compound.c`

 * *Files 1% similar despite different names*

```diff
@@ -1390,195 +1390,195 @@
   "amulet_nbt\\\\_string.pxd",
   "amulet_nbt\\\\_list.pxd",
   "amulet_nbt\\\\_load_nbt.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* #### Code section: numeric_typedefs ### */
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":731
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":731
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":732
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":732
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":733
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":734
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":738
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":738
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":739
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":739
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":740
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":741
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":745
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":745
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":746
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":746
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":755
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":755
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":756
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":756
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":757
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":759
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":759
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":760
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":760
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":761
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":761
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":763
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":764
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":766
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":766
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":767
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":767
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":768
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":768
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1671,42 +1671,42 @@
  * cdef char read_byte(BufferContext buffer) except? -1
  */
 struct __pyx_opt_args_10amulet_nbt_5_util_to_little_endian {
   int __pyx_n;
   int little_endian;
 };
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":770
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":770
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":771
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":772
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":774
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":774
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -5281,261 +5281,261 @@
 #define __pyx_codeobj__50 __pyx_mstate_global->__pyx_codeobj__50
 #define __pyx_codeobj__51 __pyx_mstate_global->__pyx_codeobj__51
 #define __pyx_codeobj__52 __pyx_mstate_global->__pyx_codeobj__52
 #define __pyx_codeobj__53 __pyx_mstate_global->__pyx_codeobj__53
 #define __pyx_codeobj__54 __pyx_mstate_global->__pyx_codeobj__54
 /* #### Code section: module_code ### */
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":245
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":251
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":257
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":263
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":271
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":278
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":284
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":776
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5544,29 +5544,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5577,15 +5577,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":779
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5594,29 +5594,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5627,15 +5627,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":782
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5644,29 +5644,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5677,15 +5677,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":785
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5694,29 +5694,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5727,15 +5727,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":788
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5744,29 +5744,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5777,212 +5777,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":791
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":793
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":792
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":795
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":795
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":791
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":970
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":971
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":972
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":974
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":975
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":977
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":976
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":978
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":978
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":982
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5998,15 +5998,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -6014,68 +6014,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":984
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 984, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":985
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":985
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 985, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 986, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 986, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -6083,15 +6083,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":982
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6106,15 +6106,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":988
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6130,15 +6130,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6146,68 +6146,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":990
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 990, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":991
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":991
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 991, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 992, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 992, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -6215,15 +6215,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":988
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6238,15 +6238,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":994
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6262,15 +6262,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6278,68 +6278,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":996
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 996, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":997
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":997
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 997, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":998
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":998
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 998, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 998, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -6347,15 +6347,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":994
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6370,176 +6370,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1001
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1013
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1001
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1016
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1028
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1016
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1031
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1038
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1031
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1041
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1045
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1041
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1048
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1052
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1052
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1048
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19025,26 +19025,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 986, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 992, __pyx_L1_error)
```

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_compound.pxd` & `amulet-nbt-2.1.0/amulet_nbt/_compound.pxd`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_compound.pyi` & `amulet-nbt-2.1.0/amulet_nbt/_compound.pyi`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_compound.pyx` & `amulet-nbt-2.1.0/amulet_nbt/_compound.pyx`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_const.c` & `amulet-nbt-2.1.0/amulet_nbt/_const.c`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_dtype.py` & `amulet-nbt-2.1.0/amulet_nbt/_dtype.py`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_errors.c` & `amulet-nbt-2.1.0/amulet_nbt/_errors.c`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_errors.pyx` & `amulet-nbt-2.1.0/amulet_nbt/_errors.pyx`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_float.c` & `amulet-nbt-2.1.0/amulet_nbt/_float.c`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_float.pyx` & `amulet-nbt-2.1.0/amulet_nbt/_float.pyx`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_int.c` & `amulet-nbt-2.1.0/amulet_nbt/_int.c`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_int.pxd` & `amulet-nbt-2.1.0/amulet_nbt/_int.pxd`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_int.pyx` & `amulet-nbt-2.1.0/amulet_nbt/_int.pyx`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_list.c` & `amulet-nbt-2.1.0/amulet_nbt/_list.c`

 * *Files 2% similar despite different names*

```diff
@@ -1391,195 +1391,195 @@
   "amulet_nbt\\\\_string.pxd",
   "amulet_nbt\\\\_compound.pxd",
   "amulet_nbt\\\\_load_nbt.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* #### Code section: numeric_typedefs ### */
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":731
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":731
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":732
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":732
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":733
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":734
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":738
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":738
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":739
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":739
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":740
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":741
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":745
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":745
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":746
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":746
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":755
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":755
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":756
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":756
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":757
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":759
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":759
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":760
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":760
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":761
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":761
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":763
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":764
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":766
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":766
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":767
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":767
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":768
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":768
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1671,42 +1671,42 @@
  * cdef char read_byte(BufferContext buffer) except? -1
  */
 struct __pyx_opt_args_10amulet_nbt_5_util_to_little_endian {
   int __pyx_n;
   int little_endian;
 };
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":770
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":770
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":771
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":772
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":774
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":774
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -4783,261 +4783,261 @@
 #define __pyx_codeobj__36 __pyx_mstate_global->__pyx_codeobj__36
 #define __pyx_codeobj__37 __pyx_mstate_global->__pyx_codeobj__37
 #define __pyx_codeobj__38 __pyx_mstate_global->__pyx_codeobj__38
 #define __pyx_codeobj__39 __pyx_mstate_global->__pyx_codeobj__39
 #define __pyx_codeobj__40 __pyx_mstate_global->__pyx_codeobj__40
 /* #### Code section: module_code ### */
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":245
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":251
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":257
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":263
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":271
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":278
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":284
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":776
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5046,29 +5046,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5079,15 +5079,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":779
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5096,29 +5096,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5129,15 +5129,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":782
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5146,29 +5146,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5179,15 +5179,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":785
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5196,29 +5196,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5229,15 +5229,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":788
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5246,29 +5246,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5279,212 +5279,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":791
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":793
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":792
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":795
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":795
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":791
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":970
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":971
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":972
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":974
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":975
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":977
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":976
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":978
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":978
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":982
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5500,15 +5500,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5516,68 +5516,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":984
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 984, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":985
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":985
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 985, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 986, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 986, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5585,15 +5585,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":982
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5608,15 +5608,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":988
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5632,15 +5632,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5648,68 +5648,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":990
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 990, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":991
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":991
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 991, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 992, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 992, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5717,15 +5717,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":988
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5740,15 +5740,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":994
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5764,15 +5764,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5780,68 +5780,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":996
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 996, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":997
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":997
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 997, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":998
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":998
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 998, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 998, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5849,15 +5849,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":994
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5872,176 +5872,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1001
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1013
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1001
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1016
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1028
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1016
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1031
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1038
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1031
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1041
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1045
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1041
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1048
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1052
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1052
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1048
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -12420,26 +12420,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 986, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 992, __pyx_L1_error)
```

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_list.pxd` & `amulet-nbt-2.1.0/amulet_nbt/_list.pxd`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_list.pyi` & `amulet-nbt-2.1.0/amulet_nbt/_list.pyi`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_list.pyx` & `amulet-nbt-2.1.0/amulet_nbt/_list.pyx`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_load_nbt.c` & `amulet-nbt-2.1.0/amulet_nbt/_load_nbt.c`

 * *Files 1% similar despite different names*

```diff
@@ -1393,195 +1393,195 @@
   "amulet_nbt\\\\_compound.pxd",
   "amulet_nbt\\\\_list.pxd",
   "amulet_nbt\\\\_named_tag.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* #### Code section: numeric_typedefs ### */
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":731
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":731
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":732
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":732
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":733
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":734
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":738
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":738
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":739
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":739
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":740
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":741
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":745
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":745
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":746
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":746
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":755
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":755
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":756
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":756
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":757
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":759
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":759
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":760
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":760
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":761
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":761
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":763
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":764
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":766
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":766
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":767
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":767
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":768
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":768
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1674,42 +1674,42 @@
  */
 struct __pyx_opt_args_10amulet_nbt_6_value_15AbstractBaseTag__pretty_to_snbt {
   int __pyx_n;
   int indent_count;
   int leading_indent;
 };
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":770
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":770
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":771
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":772
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":774
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":774
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2038,14 +2038,16 @@
 struct __pyx_opt_args_10amulet_nbt_9_load_nbt_get_buffer;
 struct __pyx_defaults;
 typedef struct __pyx_defaults __pyx_defaults;
 struct __pyx_defaults1;
 typedef struct __pyx_defaults1 __pyx_defaults1;
 struct __pyx_defaults2;
 typedef struct __pyx_defaults2 __pyx_defaults2;
+struct __pyx_defaults3;
+typedef struct __pyx_defaults3 __pyx_defaults3;
 
 /* "amulet_nbt/_load_nbt.pyx":44
  * 
  * 
  * cdef BufferContext get_buffer(             # <<<<<<<<<<<<<<
  *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
  *     bint compressed=True,
@@ -2059,14 +2061,17 @@
 };
 struct __pyx_defaults1 {
   PyObject *__pyx_arg_string_decoder;
 };
 struct __pyx_defaults2 {
   PyObject *__pyx_arg_string_decoder;
 };
+struct __pyx_defaults3 {
+  PyObject *__pyx_arg_string_decoder;
+};
 
 /* "_util.pxd":3
  * from ._dtype import DecoderType, EncoderType
  * 
  * cdef class BufferContext:             # <<<<<<<<<<<<<<
  *     cdef char *buffer
  *     cdef readonly size_t size
@@ -3590,28 +3595,28 @@
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_IOError;
 static PyObject *__pyx_builtin_open;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_EOFError;
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_range;
-static PyObject *__pyx_builtin_FutureWarning;
 static PyObject *__pyx_builtin_DeprecationWarning;
+static PyObject *__pyx_builtin_FutureWarning;
 static PyObject *__pyx_builtin_ImportError;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_i[] = "i";
 static const char __pyx_k__3[] = "\037\213";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_io[] = "io";
 static const char __pyx_k_os[] = "os";
 static const char __pyx_k_rb[] = "rb";
 static const char __pyx_k_Tag[] = "Tag ";
-static const char __pyx_k__10[] = "*";
-static const char __pyx_k__11[] = ".";
-static const char __pyx_k__24[] = "?";
+static const char __pyx_k__11[] = "*";
+static const char __pyx_k__12[] = ".";
+static const char __pyx_k__27[] = "?";
 static const char __pyx_k_int[] = "int";
 static const char __pyx_k_tag[] = "tag";
 static const char __pyx_k_List[] = "List";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_bool[] = "bool";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_exit[] = "__exit__";
@@ -3663,14 +3668,15 @@
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_load_many[] = "load_many";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_compressed[] = "compressed";
+static const char __pyx_k_load_array[] = "load_array";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_DecoderType[] = "DecoderType";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_ReadContext[] = "ReadContext";
 static const char __pyx_k_safe_gunzip[] = "safe_gunzip";
 static const char __pyx_k_NBTLoadError[] = "NBTLoadError";
 static const char __pyx_k_initializing[] = "_initializing";
@@ -3688,40 +3694,43 @@
 static const char __pyx_k_DeprecationWarning[] = "DeprecationWarning";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_filepath_or_buffer[] = "filepath_or_buffer";
 static const char __pyx_k_There_is_no_file_at[] = "There is no file at ";
 static const char __pyx_k_amulet_nbt__load_nbt[] = "amulet_nbt._load_nbt";
 static const char __pyx_k_decode_modified_utf8[] = "decode_modified_utf8";
-static const char __pyx_k_Count_must_be_1_or_more[] = "Count must be 1 or more.";
 static const char __pyx_k_amulet_nbt__load_nbt_pyx[] = "amulet_nbt\\_load_nbt.pyx";
+static const char __pyx_k_Count_must_be_1_or_higher[] = "Count must be -1 or higher";
 static const char __pyx_k_ReadContext___reduce_cython[] = "ReadContext.__reduce_cython__";
 static const char __pyx_k_ReadContext___setstate_cython[] = "ReadContext.__setstate_cython__";
 static const char __pyx_k_buffer_read_must_return_a_bytes[] = "buffer.read() must return a bytes object. Got ";
 static const char __pyx_k_load_with_offset_is_depreciated[] = "load with offset is depreciated. In future versions this function will only return the result. To get the offset pass a ReadContext instance to read_context input.";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_Union_NamedTag_Tuple_Union_Named[] = "Union[NamedTag, Tuple[Union[NamedTag, List[NamedTag]], int]]";
 static const char __pyx_k_Union_str_bytes_BinaryIO_memoryv[] = "Union[str, bytes, BinaryIO, memoryview, None]";
 static const char __pyx_k_buffer_did_not_have_a_read_metho[] = "buffer did not have a read method.";
 static const char __pyx_k_load_arguments_are_going_to_be_k[] = "load arguments are going to be keyword only in the future. This function passes the inputs positionally.";
-static const char __pyx_k_load_with_count_is_depreciated_U[] = "load with count is depreciated. Use load_many";
+static const char __pyx_k_load_many_is_depreciated_Use_loa[] = "load_many is depreciated. Use load_array instead.";
+static const char __pyx_k_load_with_count_is_depreciated_U[] = "load with count is depreciated. Use load_array";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_safe_gunzip(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data); /* proto */
 static int __pyx_pf_10amulet_nbt_9_load_nbt_11ReadContext___cinit__(struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_11ReadContext_6offset___get__(struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_11ReadContext_2__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_11ReadContext_4__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_8__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static struct __pyx_obj_10amulet_nbt_10_named_tag_NamedTag *__pyx_pf_10amulet_nbt_9_load_nbt_2_load_one(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filepath_or_buffer, int __pyx_v_compressed, int __pyx_v_little_endian, struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *__pyx_v_read_context, PyObject *__pyx_v_string_decoder); /* proto */
 static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_10__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_4load_many(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filepath_or_buffer, int __pyx_v_count, int __pyx_v_compressed, int __pyx_v_little_endian, struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *__pyx_v_read_context, PyObject *__pyx_v_string_decoder); /* proto */
+static struct __pyx_obj_10amulet_nbt_10_named_tag_NamedTag *__pyx_pf_10amulet_nbt_9_load_nbt_2_load_one(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filepath_or_buffer, int __pyx_v_compressed, int __pyx_v_little_endian, struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *__pyx_v_read_context, PyObject *__pyx_v_string_decoder); /* proto */
 static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_12__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_6load(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filepath_or_buffer, int __pyx_v_compressed, PyObject *__pyx_v_count, int __pyx_v_offset, int __pyx_v_little_endian, PyObject *__pyx_v_string_decoder, struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *__pyx_v_read_context, PyObject *__pyx_v_args); /* proto */
+static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_4load_array(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filepath_or_buffer, int __pyx_v_count, int __pyx_v_compressed, int __pyx_v_little_endian, struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *__pyx_v_read_context, PyObject *__pyx_v_string_decoder); /* proto */
+static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_14__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_6load_many(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filepath_or_buffer, int __pyx_v_count, int __pyx_v_compressed, int __pyx_v_little_endian, struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *__pyx_v_read_context, PyObject *__pyx_v_string_decoder); /* proto */
+static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_16__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_8load(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filepath_or_buffer, int __pyx_v_compressed, PyObject *__pyx_v_count, int __pyx_v_offset, int __pyx_v_little_endian, PyObject *__pyx_v_string_decoder, struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *__pyx_v_read_context, PyObject *__pyx_v_args); /* proto */
 static PyObject *__pyx_tp_new_10amulet_nbt_9_load_nbt_ReadContext(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
@@ -3824,15 +3833,15 @@
   PyTypeObject *__pyx_ptype_10amulet_nbt_10_named_tag_NamedTag;
   #if CYTHON_USE_MODULE_STATE
   PyObject *__pyx_type_10amulet_nbt_9_load_nbt_ReadContext;
   #endif
   PyTypeObject *__pyx_ptype_10amulet_nbt_9_load_nbt_ReadContext;
   PyObject *__pyx_n_s_BinaryIO;
   PyObject *__pyx_n_s_BytesIO;
-  PyObject *__pyx_kp_u_Count_must_be_1_or_more;
+  PyObject *__pyx_kp_u_Count_must_be_1_or_higher;
   PyObject *__pyx_n_s_DecoderType;
   PyObject *__pyx_n_s_DeprecationWarning;
   PyObject *__pyx_n_s_EOFError;
   PyObject *__pyx_n_s_FutureWarning;
   PyObject *__pyx_n_s_GzipFile;
   PyObject *__pyx_n_s_IOError;
   PyObject *__pyx_n_s_ImportError;
@@ -3847,17 +3856,17 @@
   PyObject *__pyx_kp_u_There_is_no_file_at;
   PyObject *__pyx_n_s_Tuple;
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_n_s_Union;
   PyObject *__pyx_kp_s_Union_NamedTag_Tuple_Union_Named;
   PyObject *__pyx_kp_s_Union_str_bytes_BinaryIO_memoryv;
   PyObject *__pyx_n_s_ValueError;
-  PyObject *__pyx_n_s__10;
-  PyObject *__pyx_kp_u__11;
-  PyObject *__pyx_n_s__24;
+  PyObject *__pyx_n_s__11;
+  PyObject *__pyx_kp_u__12;
+  PyObject *__pyx_n_s__27;
   PyObject *__pyx_kp_b__3;
   PyObject *__pyx_n_s_amulet_nbt__load_nbt;
   PyObject *__pyx_kp_s_amulet_nbt__load_nbt_pyx;
   PyObject *__pyx_n_s_args;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_bool;
   PyObject *__pyx_n_s_buffer;
@@ -3890,15 +3899,17 @@
   PyObject *__pyx_n_s_io;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_n_s_isfile;
   PyObject *__pyx_n_s_little_endian;
   PyObject *__pyx_n_s_load;
   PyObject *__pyx_kp_u_load_arguments_are_going_to_be_k;
+  PyObject *__pyx_n_s_load_array;
   PyObject *__pyx_n_s_load_many;
+  PyObject *__pyx_kp_u_load_many_is_depreciated_Use_loa;
   PyObject *__pyx_n_s_load_one;
   PyObject *__pyx_kp_u_load_with_count_is_depreciated_U;
   PyObject *__pyx_kp_u_load_with_offset_is_depreciated;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_mutf8;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
@@ -3939,26 +3950,29 @@
   PyObject *__pyx_tuple__2;
   PyObject *__pyx_tuple__4;
   PyObject *__pyx_tuple__5;
   PyObject *__pyx_tuple__6;
   PyObject *__pyx_tuple__7;
   PyObject *__pyx_tuple__8;
   PyObject *__pyx_tuple__9;
-  PyObject *__pyx_tuple__12;
-  PyObject *__pyx_tuple__14;
-  PyObject *__pyx_tuple__16;
-  PyObject *__pyx_tuple__18;
-  PyObject *__pyx_tuple__20;
-  PyObject *__pyx_tuple__22;
-  PyObject *__pyx_codeobj__13;
-  PyObject *__pyx_codeobj__15;
-  PyObject *__pyx_codeobj__17;
-  PyObject *__pyx_codeobj__19;
-  PyObject *__pyx_codeobj__21;
-  PyObject *__pyx_codeobj__23;
+  PyObject *__pyx_tuple__10;
+  PyObject *__pyx_tuple__13;
+  PyObject *__pyx_tuple__15;
+  PyObject *__pyx_tuple__17;
+  PyObject *__pyx_tuple__19;
+  PyObject *__pyx_tuple__21;
+  PyObject *__pyx_tuple__23;
+  PyObject *__pyx_tuple__25;
+  PyObject *__pyx_codeobj__14;
+  PyObject *__pyx_codeobj__16;
+  PyObject *__pyx_codeobj__18;
+  PyObject *__pyx_codeobj__20;
+  PyObject *__pyx_codeobj__22;
+  PyObject *__pyx_codeobj__24;
+  PyObject *__pyx_codeobj__26;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -4035,15 +4049,15 @@
   Py_CLEAR(clear_module_state->__pyx_ptype_10amulet_nbt_9_compound_CyCompoundTag);
   Py_CLEAR(clear_module_state->__pyx_ptype_10amulet_nbt_5_list_CyListTag);
   Py_CLEAR(clear_module_state->__pyx_ptype_10amulet_nbt_10_named_tag_NamedTag);
   Py_CLEAR(clear_module_state->__pyx_ptype_10amulet_nbt_9_load_nbt_ReadContext);
   Py_CLEAR(clear_module_state->__pyx_type_10amulet_nbt_9_load_nbt_ReadContext);
   Py_CLEAR(clear_module_state->__pyx_n_s_BinaryIO);
   Py_CLEAR(clear_module_state->__pyx_n_s_BytesIO);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Count_must_be_1_or_more);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Count_must_be_1_or_higher);
   Py_CLEAR(clear_module_state->__pyx_n_s_DecoderType);
   Py_CLEAR(clear_module_state->__pyx_n_s_DeprecationWarning);
   Py_CLEAR(clear_module_state->__pyx_n_s_EOFError);
   Py_CLEAR(clear_module_state->__pyx_n_s_FutureWarning);
   Py_CLEAR(clear_module_state->__pyx_n_s_GzipFile);
   Py_CLEAR(clear_module_state->__pyx_n_s_IOError);
   Py_CLEAR(clear_module_state->__pyx_n_s_ImportError);
@@ -4058,17 +4072,17 @@
   Py_CLEAR(clear_module_state->__pyx_kp_u_There_is_no_file_at);
   Py_CLEAR(clear_module_state->__pyx_n_s_Tuple);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_n_s_Union);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Union_NamedTag_Tuple_Union_Named);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Union_str_bytes_BinaryIO_memoryv);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
-  Py_CLEAR(clear_module_state->__pyx_n_s__10);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__11);
-  Py_CLEAR(clear_module_state->__pyx_n_s__24);
+  Py_CLEAR(clear_module_state->__pyx_n_s__11);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__12);
+  Py_CLEAR(clear_module_state->__pyx_n_s__27);
   Py_CLEAR(clear_module_state->__pyx_kp_b__3);
   Py_CLEAR(clear_module_state->__pyx_n_s_amulet_nbt__load_nbt);
   Py_CLEAR(clear_module_state->__pyx_kp_s_amulet_nbt__load_nbt_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_args);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_bool);
   Py_CLEAR(clear_module_state->__pyx_n_s_buffer);
@@ -4101,15 +4115,17 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_io);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_n_s_isfile);
   Py_CLEAR(clear_module_state->__pyx_n_s_little_endian);
   Py_CLEAR(clear_module_state->__pyx_n_s_load);
   Py_CLEAR(clear_module_state->__pyx_kp_u_load_arguments_are_going_to_be_k);
+  Py_CLEAR(clear_module_state->__pyx_n_s_load_array);
   Py_CLEAR(clear_module_state->__pyx_n_s_load_many);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_load_many_is_depreciated_Use_loa);
   Py_CLEAR(clear_module_state->__pyx_n_s_load_one);
   Py_CLEAR(clear_module_state->__pyx_kp_u_load_with_count_is_depreciated_U);
   Py_CLEAR(clear_module_state->__pyx_kp_u_load_with_offset_is_depreciated);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_mutf8);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
@@ -4150,26 +4166,29 @@
   Py_CLEAR(clear_module_state->__pyx_tuple__2);
   Py_CLEAR(clear_module_state->__pyx_tuple__4);
   Py_CLEAR(clear_module_state->__pyx_tuple__5);
   Py_CLEAR(clear_module_state->__pyx_tuple__6);
   Py_CLEAR(clear_module_state->__pyx_tuple__7);
   Py_CLEAR(clear_module_state->__pyx_tuple__8);
   Py_CLEAR(clear_module_state->__pyx_tuple__9);
-  Py_CLEAR(clear_module_state->__pyx_tuple__12);
-  Py_CLEAR(clear_module_state->__pyx_tuple__14);
-  Py_CLEAR(clear_module_state->__pyx_tuple__16);
-  Py_CLEAR(clear_module_state->__pyx_tuple__18);
-  Py_CLEAR(clear_module_state->__pyx_tuple__20);
-  Py_CLEAR(clear_module_state->__pyx_tuple__22);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__13);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__15);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__17);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__19);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__21);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__23);
+  Py_CLEAR(clear_module_state->__pyx_tuple__10);
+  Py_CLEAR(clear_module_state->__pyx_tuple__13);
+  Py_CLEAR(clear_module_state->__pyx_tuple__15);
+  Py_CLEAR(clear_module_state->__pyx_tuple__17);
+  Py_CLEAR(clear_module_state->__pyx_tuple__19);
+  Py_CLEAR(clear_module_state->__pyx_tuple__21);
+  Py_CLEAR(clear_module_state->__pyx_tuple__23);
+  Py_CLEAR(clear_module_state->__pyx_tuple__25);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__14);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__16);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__18);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__20);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__22);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__24);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__26);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -4224,15 +4243,15 @@
   Py_VISIT(traverse_module_state->__pyx_ptype_10amulet_nbt_9_compound_CyCompoundTag);
   Py_VISIT(traverse_module_state->__pyx_ptype_10amulet_nbt_5_list_CyListTag);
   Py_VISIT(traverse_module_state->__pyx_ptype_10amulet_nbt_10_named_tag_NamedTag);
   Py_VISIT(traverse_module_state->__pyx_ptype_10amulet_nbt_9_load_nbt_ReadContext);
   Py_VISIT(traverse_module_state->__pyx_type_10amulet_nbt_9_load_nbt_ReadContext);
   Py_VISIT(traverse_module_state->__pyx_n_s_BinaryIO);
   Py_VISIT(traverse_module_state->__pyx_n_s_BytesIO);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Count_must_be_1_or_more);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Count_must_be_1_or_higher);
   Py_VISIT(traverse_module_state->__pyx_n_s_DecoderType);
   Py_VISIT(traverse_module_state->__pyx_n_s_DeprecationWarning);
   Py_VISIT(traverse_module_state->__pyx_n_s_EOFError);
   Py_VISIT(traverse_module_state->__pyx_n_s_FutureWarning);
   Py_VISIT(traverse_module_state->__pyx_n_s_GzipFile);
   Py_VISIT(traverse_module_state->__pyx_n_s_IOError);
   Py_VISIT(traverse_module_state->__pyx_n_s_ImportError);
@@ -4247,17 +4266,17 @@
   Py_VISIT(traverse_module_state->__pyx_kp_u_There_is_no_file_at);
   Py_VISIT(traverse_module_state->__pyx_n_s_Tuple);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_n_s_Union);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Union_NamedTag_Tuple_Union_Named);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Union_str_bytes_BinaryIO_memoryv);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
-  Py_VISIT(traverse_module_state->__pyx_n_s__10);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__11);
-  Py_VISIT(traverse_module_state->__pyx_n_s__24);
+  Py_VISIT(traverse_module_state->__pyx_n_s__11);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__12);
+  Py_VISIT(traverse_module_state->__pyx_n_s__27);
   Py_VISIT(traverse_module_state->__pyx_kp_b__3);
   Py_VISIT(traverse_module_state->__pyx_n_s_amulet_nbt__load_nbt);
   Py_VISIT(traverse_module_state->__pyx_kp_s_amulet_nbt__load_nbt_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_args);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_bool);
   Py_VISIT(traverse_module_state->__pyx_n_s_buffer);
@@ -4290,15 +4309,17 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_io);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_n_s_isfile);
   Py_VISIT(traverse_module_state->__pyx_n_s_little_endian);
   Py_VISIT(traverse_module_state->__pyx_n_s_load);
   Py_VISIT(traverse_module_state->__pyx_kp_u_load_arguments_are_going_to_be_k);
+  Py_VISIT(traverse_module_state->__pyx_n_s_load_array);
   Py_VISIT(traverse_module_state->__pyx_n_s_load_many);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_load_many_is_depreciated_Use_loa);
   Py_VISIT(traverse_module_state->__pyx_n_s_load_one);
   Py_VISIT(traverse_module_state->__pyx_kp_u_load_with_count_is_depreciated_U);
   Py_VISIT(traverse_module_state->__pyx_kp_u_load_with_offset_is_depreciated);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_mutf8);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
@@ -4339,26 +4360,29 @@
   Py_VISIT(traverse_module_state->__pyx_tuple__2);
   Py_VISIT(traverse_module_state->__pyx_tuple__4);
   Py_VISIT(traverse_module_state->__pyx_tuple__5);
   Py_VISIT(traverse_module_state->__pyx_tuple__6);
   Py_VISIT(traverse_module_state->__pyx_tuple__7);
   Py_VISIT(traverse_module_state->__pyx_tuple__8);
   Py_VISIT(traverse_module_state->__pyx_tuple__9);
-  Py_VISIT(traverse_module_state->__pyx_tuple__12);
-  Py_VISIT(traverse_module_state->__pyx_tuple__14);
-  Py_VISIT(traverse_module_state->__pyx_tuple__16);
-  Py_VISIT(traverse_module_state->__pyx_tuple__18);
-  Py_VISIT(traverse_module_state->__pyx_tuple__20);
-  Py_VISIT(traverse_module_state->__pyx_tuple__22);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__13);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__15);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__17);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__19);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__21);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__23);
+  Py_VISIT(traverse_module_state->__pyx_tuple__10);
+  Py_VISIT(traverse_module_state->__pyx_tuple__13);
+  Py_VISIT(traverse_module_state->__pyx_tuple__15);
+  Py_VISIT(traverse_module_state->__pyx_tuple__17);
+  Py_VISIT(traverse_module_state->__pyx_tuple__19);
+  Py_VISIT(traverse_module_state->__pyx_tuple__21);
+  Py_VISIT(traverse_module_state->__pyx_tuple__23);
+  Py_VISIT(traverse_module_state->__pyx_tuple__25);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__14);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__16);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__18);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__20);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__22);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__24);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__26);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -4461,15 +4485,15 @@
 #define __pyx_ptype_10amulet_nbt_10_named_tag_NamedTag __pyx_mstate_global->__pyx_ptype_10amulet_nbt_10_named_tag_NamedTag
 #if CYTHON_USE_MODULE_STATE
 #define __pyx_type_10amulet_nbt_9_load_nbt_ReadContext __pyx_mstate_global->__pyx_type_10amulet_nbt_9_load_nbt_ReadContext
 #endif
 #define __pyx_ptype_10amulet_nbt_9_load_nbt_ReadContext __pyx_mstate_global->__pyx_ptype_10amulet_nbt_9_load_nbt_ReadContext
 #define __pyx_n_s_BinaryIO __pyx_mstate_global->__pyx_n_s_BinaryIO
 #define __pyx_n_s_BytesIO __pyx_mstate_global->__pyx_n_s_BytesIO
-#define __pyx_kp_u_Count_must_be_1_or_more __pyx_mstate_global->__pyx_kp_u_Count_must_be_1_or_more
+#define __pyx_kp_u_Count_must_be_1_or_higher __pyx_mstate_global->__pyx_kp_u_Count_must_be_1_or_higher
 #define __pyx_n_s_DecoderType __pyx_mstate_global->__pyx_n_s_DecoderType
 #define __pyx_n_s_DeprecationWarning __pyx_mstate_global->__pyx_n_s_DeprecationWarning
 #define __pyx_n_s_EOFError __pyx_mstate_global->__pyx_n_s_EOFError
 #define __pyx_n_s_FutureWarning __pyx_mstate_global->__pyx_n_s_FutureWarning
 #define __pyx_n_s_GzipFile __pyx_mstate_global->__pyx_n_s_GzipFile
 #define __pyx_n_s_IOError __pyx_mstate_global->__pyx_n_s_IOError
 #define __pyx_n_s_ImportError __pyx_mstate_global->__pyx_n_s_ImportError
@@ -4484,17 +4508,17 @@
 #define __pyx_kp_u_There_is_no_file_at __pyx_mstate_global->__pyx_kp_u_There_is_no_file_at
 #define __pyx_n_s_Tuple __pyx_mstate_global->__pyx_n_s_Tuple
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_n_s_Union __pyx_mstate_global->__pyx_n_s_Union
 #define __pyx_kp_s_Union_NamedTag_Tuple_Union_Named __pyx_mstate_global->__pyx_kp_s_Union_NamedTag_Tuple_Union_Named
 #define __pyx_kp_s_Union_str_bytes_BinaryIO_memoryv __pyx_mstate_global->__pyx_kp_s_Union_str_bytes_BinaryIO_memoryv
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
-#define __pyx_n_s__10 __pyx_mstate_global->__pyx_n_s__10
-#define __pyx_kp_u__11 __pyx_mstate_global->__pyx_kp_u__11
-#define __pyx_n_s__24 __pyx_mstate_global->__pyx_n_s__24
+#define __pyx_n_s__11 __pyx_mstate_global->__pyx_n_s__11
+#define __pyx_kp_u__12 __pyx_mstate_global->__pyx_kp_u__12
+#define __pyx_n_s__27 __pyx_mstate_global->__pyx_n_s__27
 #define __pyx_kp_b__3 __pyx_mstate_global->__pyx_kp_b__3
 #define __pyx_n_s_amulet_nbt__load_nbt __pyx_mstate_global->__pyx_n_s_amulet_nbt__load_nbt
 #define __pyx_kp_s_amulet_nbt__load_nbt_pyx __pyx_mstate_global->__pyx_kp_s_amulet_nbt__load_nbt_pyx
 #define __pyx_n_s_args __pyx_mstate_global->__pyx_n_s_args
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_bool __pyx_mstate_global->__pyx_n_s_bool
 #define __pyx_n_s_buffer __pyx_mstate_global->__pyx_n_s_buffer
@@ -4527,15 +4551,17 @@
 #define __pyx_n_s_io __pyx_mstate_global->__pyx_n_s_io
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_n_s_isfile __pyx_mstate_global->__pyx_n_s_isfile
 #define __pyx_n_s_little_endian __pyx_mstate_global->__pyx_n_s_little_endian
 #define __pyx_n_s_load __pyx_mstate_global->__pyx_n_s_load
 #define __pyx_kp_u_load_arguments_are_going_to_be_k __pyx_mstate_global->__pyx_kp_u_load_arguments_are_going_to_be_k
+#define __pyx_n_s_load_array __pyx_mstate_global->__pyx_n_s_load_array
 #define __pyx_n_s_load_many __pyx_mstate_global->__pyx_n_s_load_many
+#define __pyx_kp_u_load_many_is_depreciated_Use_loa __pyx_mstate_global->__pyx_kp_u_load_many_is_depreciated_Use_loa
 #define __pyx_n_s_load_one __pyx_mstate_global->__pyx_n_s_load_one
 #define __pyx_kp_u_load_with_count_is_depreciated_U __pyx_mstate_global->__pyx_kp_u_load_with_count_is_depreciated_U
 #define __pyx_kp_u_load_with_offset_is_depreciated __pyx_mstate_global->__pyx_kp_u_load_with_offset_is_depreciated
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_mutf8 __pyx_mstate_global->__pyx_n_s_mutf8
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_kp_s_no_default___reduce___due_to_non __pyx_mstate_global->__pyx_kp_s_no_default___reduce___due_to_non
@@ -4576,275 +4602,278 @@
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
 #define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
 #define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
 #define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
 #define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
-#define __pyx_tuple__12 __pyx_mstate_global->__pyx_tuple__12
-#define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
-#define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
-#define __pyx_tuple__18 __pyx_mstate_global->__pyx_tuple__18
-#define __pyx_tuple__20 __pyx_mstate_global->__pyx_tuple__20
-#define __pyx_tuple__22 __pyx_mstate_global->__pyx_tuple__22
-#define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
-#define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
-#define __pyx_codeobj__17 __pyx_mstate_global->__pyx_codeobj__17
-#define __pyx_codeobj__19 __pyx_mstate_global->__pyx_codeobj__19
-#define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
-#define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
+#define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
+#define __pyx_tuple__13 __pyx_mstate_global->__pyx_tuple__13
+#define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
+#define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
+#define __pyx_tuple__19 __pyx_mstate_global->__pyx_tuple__19
+#define __pyx_tuple__21 __pyx_mstate_global->__pyx_tuple__21
+#define __pyx_tuple__23 __pyx_mstate_global->__pyx_tuple__23
+#define __pyx_tuple__25 __pyx_mstate_global->__pyx_tuple__25
+#define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
+#define __pyx_codeobj__16 __pyx_mstate_global->__pyx_codeobj__16
+#define __pyx_codeobj__18 __pyx_mstate_global->__pyx_codeobj__18
+#define __pyx_codeobj__20 __pyx_mstate_global->__pyx_codeobj__20
+#define __pyx_codeobj__22 __pyx_mstate_global->__pyx_codeobj__22
+#define __pyx_codeobj__24 __pyx_mstate_global->__pyx_codeobj__24
+#define __pyx_codeobj__26 __pyx_mstate_global->__pyx_codeobj__26
 /* #### Code section: module_code ### */
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":245
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":251
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":257
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":263
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":271
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":278
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":284
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":776
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4853,29 +4882,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4886,15 +4915,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":779
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4903,29 +4932,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4936,15 +4965,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":782
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4953,29 +4982,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4986,15 +5015,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":785
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5003,29 +5032,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5036,15 +5065,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":788
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5053,29 +5082,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5086,212 +5115,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":791
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":793
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":792
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":795
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":795
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":791
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":970
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":971
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":972
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":974
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":975
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":977
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":976
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":978
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":978
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":982
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5307,15 +5336,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5323,68 +5352,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":984
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 984, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":985
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":985
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 985, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 986, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 986, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5392,15 +5421,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":982
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5415,15 +5444,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":988
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5439,15 +5468,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5455,68 +5484,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":990
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 990, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":991
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":991
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 991, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 992, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 992, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5524,15 +5553,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":988
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5547,15 +5576,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":994
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5571,15 +5600,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5587,68 +5616,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":996
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 996, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":997
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":997
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 997, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":998
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":998
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 998, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 998, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5656,15 +5685,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":994
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5679,176 +5708,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1001
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1013
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1001
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1016
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1028
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1016
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1031
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1038
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1031
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1041
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1045
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1041
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1048
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1052
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1052
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1048
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -7764,15 +7793,15 @@
  * 
  * 
  * def _load_one(             # <<<<<<<<<<<<<<
  *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
  *     *,
  */
 
-static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_8__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_10__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -8082,20 +8111,20 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "amulet_nbt/_load_nbt.pyx":136
  * 
  * 
- * def load_many(             # <<<<<<<<<<<<<<
+ * def load_array(             # <<<<<<<<<<<<<<
  *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
  *     *,
  */
 
-static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_10__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_12__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -8148,15 +8177,15 @@
  * ) -> List[NamedTag]:
  */
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_read_context, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
 
   /* "amulet_nbt/_load_nbt.pyx":136
  * 
  * 
- * def load_many(             # <<<<<<<<<<<<<<
+ * def load_array(             # <<<<<<<<<<<<<<
  *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
  *     *,
  */
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_string_decoder, __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_string_decoder) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
   __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(Py_None);
@@ -8178,23 +8207,23 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10amulet_nbt_9_load_nbt_5load_many(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_10amulet_nbt_9_load_nbt_5load_array(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_10amulet_nbt_9_load_nbt_5load_many = {"load_many", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10amulet_nbt_9_load_nbt_5load_many, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_10amulet_nbt_9_load_nbt_5load_many(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_10amulet_nbt_9_load_nbt_5load_array = {"load_array", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10amulet_nbt_9_load_nbt_5load_array, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_10amulet_nbt_9_load_nbt_5load_array(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_filepath_or_buffer = 0;
@@ -8208,15 +8237,15 @@
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("load_many (wrapper)", 0);
+  __Pyx_RefNannySetupContext("load_array (wrapper)", 0);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_filepath_or_buffer,&__pyx_n_s_count,&__pyx_n_s_compressed,&__pyx_n_s_little_endian,&__pyx_n_s_read_context,&__pyx_n_s_string_decoder,0};
     PyObject* values[6] = {0,0,0,0,0,0};
     __pyx_defaults1 *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self);
     values[4] = (PyObject *)((struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *)((PyObject *)Py_None));
     values[5] = __pyx_dynamic_args->__pyx_arg_string_decoder;
     if (__pyx_kwds) {
@@ -8240,15 +8269,15 @@
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, *__pyx_pyargnames[index]);
           if (value) { values[index] = value; kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "load_many") < 0)) __PYX_ERR(0, 136, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "load_array") < 0)) __PYX_ERR(0, 136, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_filepath_or_buffer = values[0];
@@ -8268,327 +8297,656 @@
       __pyx_v_little_endian = ((int)((int)0));
     }
     __pyx_v_read_context = ((struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *)values[4]);
     __pyx_v_string_decoder = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("load_many", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 136, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("load_array", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 136, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("amulet_nbt._load_nbt.load_many", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("amulet_nbt._load_nbt.load_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_read_context), __pyx_ptype_10amulet_nbt_9_load_nbt_ReadContext, 1, "read_context", 0))) __PYX_ERR(0, 142, __pyx_L1_error)
-  __pyx_r = __pyx_pf_10amulet_nbt_9_load_nbt_4load_many(__pyx_self, __pyx_v_filepath_or_buffer, __pyx_v_count, __pyx_v_compressed, __pyx_v_little_endian, __pyx_v_read_context, __pyx_v_string_decoder);
+  __pyx_r = __pyx_pf_10amulet_nbt_9_load_nbt_4load_array(__pyx_self, __pyx_v_filepath_or_buffer, __pyx_v_count, __pyx_v_compressed, __pyx_v_little_endian, __pyx_v_read_context, __pyx_v_string_decoder);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_4load_many(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filepath_or_buffer, int __pyx_v_count, int __pyx_v_compressed, int __pyx_v_little_endian, struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *__pyx_v_read_context, PyObject *__pyx_v_string_decoder) {
+static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_4load_array(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filepath_or_buffer, int __pyx_v_count, int __pyx_v_compressed, int __pyx_v_little_endian, struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *__pyx_v_read_context, PyObject *__pyx_v_string_decoder) {
   struct __pyx_obj_10amulet_nbt_5_util_BufferContext *__pyx_v_buffer = 0;
   PyObject *__pyx_v_results = 0;
   CYTHON_UNUSED size_t __pyx_v_i;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   struct __pyx_opt_args_10amulet_nbt_9_load_nbt_get_buffer __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
-  size_t __pyx_t_6;
-  int __pyx_t_7;
+  int __pyx_t_6;
+  size_t __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("load_many", 0);
+  __Pyx_RefNannySetupContext("load_array", 0);
 
   /* "amulet_nbt/_load_nbt.pyx":145
  *     string_decoder: DecoderType = decode_modified_utf8
  * ) -> List[NamedTag]:
- *     if count < 1:             # <<<<<<<<<<<<<<
- *         raise ValueError("Count must be 1 or more.")
+ *     if count < -1:             # <<<<<<<<<<<<<<
+ *         raise ValueError("Count must be -1 or higher")
  *     cdef BufferContext buffer = get_buffer(filepath_or_buffer, compressed)
  */
-  __pyx_t_1 = (__pyx_v_count < 1);
+  __pyx_t_1 = (__pyx_v_count < -1L);
   if (unlikely(__pyx_t_1)) {
 
     /* "amulet_nbt/_load_nbt.pyx":146
  * ) -> List[NamedTag]:
- *     if count < 1:
- *         raise ValueError("Count must be 1 or more.")             # <<<<<<<<<<<<<<
+ *     if count < -1:
+ *         raise ValueError("Count must be -1 or higher")             # <<<<<<<<<<<<<<
  *     cdef BufferContext buffer = get_buffer(filepath_or_buffer, compressed)
- *     if buffer.size < 1:
+ *     cdef list results = []
  */
     __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 146, __pyx_L1_error)
 
     /* "amulet_nbt/_load_nbt.pyx":145
  *     string_decoder: DecoderType = decode_modified_utf8
  * ) -> List[NamedTag]:
- *     if count < 1:             # <<<<<<<<<<<<<<
- *         raise ValueError("Count must be 1 or more.")
+ *     if count < -1:             # <<<<<<<<<<<<<<
+ *         raise ValueError("Count must be -1 or higher")
  *     cdef BufferContext buffer = get_buffer(filepath_or_buffer, compressed)
  */
   }
 
   /* "amulet_nbt/_load_nbt.pyx":147
- *     if count < 1:
- *         raise ValueError("Count must be 1 or more.")
+ *     if count < -1:
+ *         raise ValueError("Count must be -1 or higher")
  *     cdef BufferContext buffer = get_buffer(filepath_or_buffer, compressed)             # <<<<<<<<<<<<<<
- *     if buffer.size < 1:
- *         raise EOFError("buffer is empty")
+ *     cdef list results = []
+ *     cdef size_t i
  */
   __pyx_t_3.__pyx_n = 1;
   __pyx_t_3.compressed = __pyx_v_compressed;
   __pyx_t_2 = ((PyObject *)__pyx_f_10amulet_nbt_9_load_nbt_get_buffer(__pyx_v_filepath_or_buffer, &__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_buffer = ((struct __pyx_obj_10amulet_nbt_5_util_BufferContext *)__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "amulet_nbt/_load_nbt.pyx":148
- *         raise ValueError("Count must be 1 or more.")
+ *         raise ValueError("Count must be -1 or higher")
  *     cdef BufferContext buffer = get_buffer(filepath_or_buffer, compressed)
- *     if buffer.size < 1:             # <<<<<<<<<<<<<<
- *         raise EOFError("buffer is empty")
- *     cdef list results = []
+ *     cdef list results = []             # <<<<<<<<<<<<<<
+ *     cdef size_t i
+ *     if count == -1:
  */
-  __pyx_t_1 = (__pyx_v_buffer->size < 1);
-  if (unlikely(__pyx_t_1)) {
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_v_results = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
 
-    /* "amulet_nbt/_load_nbt.pyx":149
- *     cdef BufferContext buffer = get_buffer(filepath_or_buffer, compressed)
- *     if buffer.size < 1:
- *         raise EOFError("buffer is empty")             # <<<<<<<<<<<<<<
+  /* "amulet_nbt/_load_nbt.pyx":150
  *     cdef list results = []
  *     cdef size_t i
+ *     if count == -1:             # <<<<<<<<<<<<<<
+ *         while buffer.offset < buffer.size:
+ *             results.append(
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_EOFError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_1 = (__pyx_v_count == -1L);
+  if (__pyx_t_1) {
 
-    /* "amulet_nbt/_load_nbt.pyx":148
- *         raise ValueError("Count must be 1 or more.")
- *     cdef BufferContext buffer = get_buffer(filepath_or_buffer, compressed)
- *     if buffer.size < 1:             # <<<<<<<<<<<<<<
- *         raise EOFError("buffer is empty")
- *     cdef list results = []
+    /* "amulet_nbt/_load_nbt.pyx":151
+ *     cdef size_t i
+ *     if count == -1:
+ *         while buffer.offset < buffer.size:             # <<<<<<<<<<<<<<
+ *             results.append(
+ *                 load_named_tag(buffer, little_endian, string_decoder)
  */
-  }
+    while (1) {
+      __pyx_t_1 = (__pyx_v_buffer->offset < __pyx_v_buffer->size);
+      if (!__pyx_t_1) break;
 
-  /* "amulet_nbt/_load_nbt.pyx":150
- *     if buffer.size < 1:
- *         raise EOFError("buffer is empty")
- *     cdef list results = []             # <<<<<<<<<<<<<<
- *     cdef size_t i
- *     for i in range(count):
+      /* "amulet_nbt/_load_nbt.pyx":153
+ *         while buffer.offset < buffer.size:
+ *             results.append(
+ *                 load_named_tag(buffer, little_endian, string_decoder)             # <<<<<<<<<<<<<<
+ *             )
+ *     else:
  */
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_v_results = ((PyObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
+      __pyx_t_2 = ((PyObject *)__pyx_f_10amulet_nbt_9_load_nbt_load_named_tag(__pyx_v_buffer, __pyx_v_little_endian, __pyx_v_string_decoder)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
 
-  /* "amulet_nbt/_load_nbt.pyx":152
- *     cdef list results = []
- *     cdef size_t i
- *     for i in range(count):             # <<<<<<<<<<<<<<
- *         results.append(
- *             load_named_tag(buffer, little_endian, string_decoder)
- */
-  __pyx_t_4 = __pyx_v_count;
-  __pyx_t_5 = __pyx_t_4;
-  for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
-    __pyx_v_i = __pyx_t_6;
-
-    /* "amulet_nbt/_load_nbt.pyx":154
- *     for i in range(count):
- *         results.append(
- *             load_named_tag(buffer, little_endian, string_decoder)             # <<<<<<<<<<<<<<
- *         )
- *     if read_context is not None:
+      /* "amulet_nbt/_load_nbt.pyx":152
+ *     if count == -1:
+ *         while buffer.offset < buffer.size:
+ *             results.append(             # <<<<<<<<<<<<<<
+ *                 load_named_tag(buffer, little_endian, string_decoder)
+ *             )
  */
-    __pyx_t_2 = ((PyObject *)__pyx_f_10amulet_nbt_9_load_nbt_load_named_tag(__pyx_v_buffer, __pyx_v_little_endian, __pyx_v_string_decoder)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_4 = __Pyx_PyList_Append(__pyx_v_results, __pyx_t_2); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 152, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    }
 
-    /* "amulet_nbt/_load_nbt.pyx":153
+    /* "amulet_nbt/_load_nbt.pyx":150
+ *     cdef list results = []
  *     cdef size_t i
- *     for i in range(count):
- *         results.append(             # <<<<<<<<<<<<<<
- *             load_named_tag(buffer, little_endian, string_decoder)
- *         )
+ *     if count == -1:             # <<<<<<<<<<<<<<
+ *         while buffer.offset < buffer.size:
+ *             results.append(
  */
-    __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_results, __pyx_t_2); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 153, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    goto __pyx_L4;
   }
 
   /* "amulet_nbt/_load_nbt.pyx":156
- *             load_named_tag(buffer, little_endian, string_decoder)
- *         )
+ *             )
+ *     else:
+ *         for i in range(count):             # <<<<<<<<<<<<<<
+ *             results.append(
+ *                 load_named_tag(buffer, little_endian, string_decoder)
+ */
+  /*else*/ {
+    __pyx_t_5 = __pyx_v_count;
+    __pyx_t_6 = __pyx_t_5;
+    for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
+      __pyx_v_i = __pyx_t_7;
+
+      /* "amulet_nbt/_load_nbt.pyx":158
+ *         for i in range(count):
+ *             results.append(
+ *                 load_named_tag(buffer, little_endian, string_decoder)             # <<<<<<<<<<<<<<
+ *             )
+ * 
+ */
+      __pyx_t_2 = ((PyObject *)__pyx_f_10amulet_nbt_9_load_nbt_load_named_tag(__pyx_v_buffer, __pyx_v_little_endian, __pyx_v_string_decoder)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 158, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+
+      /* "amulet_nbt/_load_nbt.pyx":157
+ *     else:
+ *         for i in range(count):
+ *             results.append(             # <<<<<<<<<<<<<<
+ *                 load_named_tag(buffer, little_endian, string_decoder)
+ *             )
+ */
+      __pyx_t_4 = __Pyx_PyList_Append(__pyx_v_results, __pyx_t_2); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 157, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    }
+  }
+  __pyx_L4:;
+
+  /* "amulet_nbt/_load_nbt.pyx":161
+ *             )
+ * 
  *     if read_context is not None:             # <<<<<<<<<<<<<<
  *         read_context.offset = buffer.offset
  *     return results
  */
   __pyx_t_1 = (((PyObject *)__pyx_v_read_context) != Py_None);
   if (__pyx_t_1) {
 
-    /* "amulet_nbt/_load_nbt.pyx":157
- *         )
+    /* "amulet_nbt/_load_nbt.pyx":162
+ * 
  *     if read_context is not None:
  *         read_context.offset = buffer.offset             # <<<<<<<<<<<<<<
  *     return results
  * 
  */
-    __pyx_t_6 = __pyx_v_buffer->offset;
-    __pyx_v_read_context->offset = __pyx_t_6;
+    __pyx_t_7 = __pyx_v_buffer->offset;
+    __pyx_v_read_context->offset = __pyx_t_7;
 
-    /* "amulet_nbt/_load_nbt.pyx":156
- *             load_named_tag(buffer, little_endian, string_decoder)
- *         )
+    /* "amulet_nbt/_load_nbt.pyx":161
+ *             )
+ * 
  *     if read_context is not None:             # <<<<<<<<<<<<<<
  *         read_context.offset = buffer.offset
  *     return results
  */
   }
 
-  /* "amulet_nbt/_load_nbt.pyx":158
+  /* "amulet_nbt/_load_nbt.pyx":163
  *     if read_context is not None:
  *         read_context.offset = buffer.offset
  *     return results             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_results);
   __pyx_r = __pyx_v_results;
   goto __pyx_L0;
 
   /* "amulet_nbt/_load_nbt.pyx":136
  * 
  * 
- * def load_many(             # <<<<<<<<<<<<<<
+ * def load_array(             # <<<<<<<<<<<<<<
  *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
  *     *,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("amulet_nbt._load_nbt.load_many", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("amulet_nbt._load_nbt.load_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_buffer);
   __Pyx_XDECREF(__pyx_v_results);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "amulet_nbt/_load_nbt.pyx":161
+/* "amulet_nbt/_load_nbt.pyx":166
+ * 
+ * 
+ * def load_many(             # <<<<<<<<<<<<<<
+ *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
+ *     *,
+ */
+
+static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_14__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__defaults__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+
+  /* "amulet_nbt/_load_nbt.pyx":169
+ *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
+ *     *,
+ *     int count = 1,             # <<<<<<<<<<<<<<
+ *     bint compressed: bool=True,
+ *     bint little_endian: bool = False,
+ */
+  __pyx_t_2 = __Pyx_PyInt_From_int(((int)1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_count, __pyx_t_2) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "amulet_nbt/_load_nbt.pyx":170
+ *     *,
+ *     int count = 1,
+ *     bint compressed: bool=True,             # <<<<<<<<<<<<<<
+ *     bint little_endian: bool = False,
+ *     ReadContext read_context = None,
+ */
+  __pyx_t_2 = __Pyx_PyBool_FromLong(((int)1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_compressed, __pyx_t_2) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "amulet_nbt/_load_nbt.pyx":171
+ *     int count = 1,
+ *     bint compressed: bool=True,
+ *     bint little_endian: bool = False,             # <<<<<<<<<<<<<<
+ *     ReadContext read_context = None,
+ *     string_decoder: DecoderType = decode_modified_utf8
+ */
+  __pyx_t_2 = __Pyx_PyBool_FromLong(((int)0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_little_endian, __pyx_t_2) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "amulet_nbt/_load_nbt.pyx":172
+ *     bint compressed: bool=True,
+ *     bint little_endian: bool = False,
+ *     ReadContext read_context = None,             # <<<<<<<<<<<<<<
+ *     string_decoder: DecoderType = decode_modified_utf8
+ * ):
+ */
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_read_context, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
+
+  /* "amulet_nbt/_load_nbt.pyx":166
+ * 
+ * 
+ * def load_many(             # <<<<<<<<<<<<<<
+ *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
+ *     *,
+ */
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_string_decoder, __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_self)->__pyx_arg_string_decoder) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, Py_None);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("amulet_nbt._load_nbt.__defaults__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static PyObject *__pyx_pw_10amulet_nbt_9_load_nbt_7load_many(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_10amulet_nbt_9_load_nbt_7load_many = {"load_many", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10amulet_nbt_9_load_nbt_7load_many, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_10amulet_nbt_9_load_nbt_7load_many(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_filepath_or_buffer = 0;
+  int __pyx_v_count;
+  int __pyx_v_compressed;
+  int __pyx_v_little_endian;
+  struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *__pyx_v_read_context = 0;
+  PyObject *__pyx_v_string_decoder = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("load_many (wrapper)", 0);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_filepath_or_buffer,&__pyx_n_s_count,&__pyx_n_s_compressed,&__pyx_n_s_little_endian,&__pyx_n_s_read_context,&__pyx_n_s_string_decoder,0};
+    PyObject* values[6] = {0,0,0,0,0,0};
+    __pyx_defaults2 *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_self);
+    values[4] = (PyObject *)((struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *)((PyObject *)Py_None));
+    values[5] = __pyx_dynamic_args->__pyx_arg_string_decoder;
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_filepath_or_buffer)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (kw_args > 0 && likely(kw_args <= 5)) {
+        Py_ssize_t index;
+        for (index = 1; index < 6 && kw_args > 0; index++) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, *__pyx_pyargnames[index]);
+          if (value) { values[index] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "load_many") < 0)) __PYX_ERR(0, 166, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_filepath_or_buffer = values[0];
+    if (values[1]) {
+      __pyx_v_count = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_count == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 169, __pyx_L3_error)
+    } else {
+      __pyx_v_count = ((int)((int)1));
+    }
+    if (values[2]) {
+      __pyx_v_compressed = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_compressed == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 170, __pyx_L3_error)
+    } else {
+      __pyx_v_compressed = ((int)((int)1));
+    }
+    if (values[3]) {
+      __pyx_v_little_endian = __Pyx_PyObject_IsTrue(values[3]); if (unlikely((__pyx_v_little_endian == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 171, __pyx_L3_error)
+    } else {
+      __pyx_v_little_endian = ((int)((int)0));
+    }
+    __pyx_v_read_context = ((struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *)values[4]);
+    __pyx_v_string_decoder = values[5];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("load_many", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 166, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("amulet_nbt._load_nbt.load_many", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_read_context), __pyx_ptype_10amulet_nbt_9_load_nbt_ReadContext, 1, "read_context", 0))) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_r = __pyx_pf_10amulet_nbt_9_load_nbt_6load_many(__pyx_self, __pyx_v_filepath_or_buffer, __pyx_v_count, __pyx_v_compressed, __pyx_v_little_endian, __pyx_v_read_context, __pyx_v_string_decoder);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_6load_many(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filepath_or_buffer, int __pyx_v_count, int __pyx_v_compressed, int __pyx_v_little_endian, struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *__pyx_v_read_context, PyObject *__pyx_v_string_decoder) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("load_many", 0);
+
+  /* "amulet_nbt/_load_nbt.pyx":175
+ *     string_decoder: DecoderType = decode_modified_utf8
+ * ):
+ *     warnings.warn("load_many is depreciated. Use load_array instead.", DeprecationWarning)             # <<<<<<<<<<<<<<
+ *     return load_array(filepath_or_buffer, count, compressed, little_endian, read_context, string_decoder)
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_warnings); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "amulet_nbt/_load_nbt.pyx":176
+ * ):
+ *     warnings.warn("load_many is depreciated. Use load_array instead.", DeprecationWarning)
+ *     return load_array(filepath_or_buffer, count, compressed, little_endian, read_context, string_decoder)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_load_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 176, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_count); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 176, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_compressed); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 176, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyBool_FromLong(__pyx_v_little_endian); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 176, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = NULL;
+  __pyx_t_7 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_6)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_6);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_7 = 1;
+    }
+  }
+  {
+    PyObject *__pyx_callargs[7] = {__pyx_t_6, __pyx_v_filepath_or_buffer, __pyx_t_3, __pyx_t_4, __pyx_t_5, ((PyObject *)__pyx_v_read_context), __pyx_v_string_decoder};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_7, 6+__pyx_t_7);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "amulet_nbt/_load_nbt.pyx":166
+ * 
+ * 
+ * def load_many(             # <<<<<<<<<<<<<<
+ *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
+ *     *,
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("amulet_nbt._load_nbt.load_many", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "amulet_nbt/_load_nbt.pyx":179
  * 
  * 
  * def load(             # <<<<<<<<<<<<<<
  *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
  *     *args,
  */
 
-static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_12__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_16__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "amulet_nbt/_load_nbt.pyx":164
+  /* "amulet_nbt/_load_nbt.pyx":182
  *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
  *     *args,
  *     bint compressed: bool=True,             # <<<<<<<<<<<<<<
  *     object count: int = None,
  *     bint offset: bool = False,
  */
-  __pyx_t_2 = __Pyx_PyBool_FromLong(((int)1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(((int)1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_compressed, __pyx_t_2) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_compressed, __pyx_t_2) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "amulet_nbt/_load_nbt.pyx":165
+  /* "amulet_nbt/_load_nbt.pyx":183
  *     *args,
  *     bint compressed: bool=True,
  *     object count: int = None,             # <<<<<<<<<<<<<<
  *     bint offset: bool = False,
  *     bint little_endian: bool = False,
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_count, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_count, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
 
-  /* "amulet_nbt/_load_nbt.pyx":166
+  /* "amulet_nbt/_load_nbt.pyx":184
  *     bint compressed: bool=True,
  *     object count: int = None,
  *     bint offset: bool = False,             # <<<<<<<<<<<<<<
  *     bint little_endian: bool = False,
  *     string_decoder: DecoderType = decode_modified_utf8,
  */
-  __pyx_t_2 = __Pyx_PyBool_FromLong(((int)0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(((int)0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_offset, __pyx_t_2) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_offset, __pyx_t_2) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "amulet_nbt/_load_nbt.pyx":167
+  /* "amulet_nbt/_load_nbt.pyx":185
  *     object count: int = None,
  *     bint offset: bool = False,
  *     bint little_endian: bool = False,             # <<<<<<<<<<<<<<
  *     string_decoder: DecoderType = decode_modified_utf8,
  *     ReadContext read_context = None,
  */
-  __pyx_t_2 = __Pyx_PyBool_FromLong(((int)0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(((int)0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_little_endian, __pyx_t_2) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_little_endian, __pyx_t_2) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "amulet_nbt/_load_nbt.pyx":161
+  /* "amulet_nbt/_load_nbt.pyx":179
  * 
  * 
  * def load(             # <<<<<<<<<<<<<<
  *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
  *     *args,
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_string_decoder, __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_self)->__pyx_arg_string_decoder) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_string_decoder, __Pyx_CyFunction_Defaults(__pyx_defaults3, __pyx_self)->__pyx_arg_string_decoder) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
 
-  /* "amulet_nbt/_load_nbt.pyx":169
+  /* "amulet_nbt/_load_nbt.pyx":187
  *     bint little_endian: bool = False,
  *     string_decoder: DecoderType = decode_modified_utf8,
  *     ReadContext read_context = None,             # <<<<<<<<<<<<<<
  * ) -> Union[NamedTag, Tuple[Union[NamedTag, List[NamedTag]], int]]:
  *     if args:
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_read_context, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_read_context, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
 
-  /* "amulet_nbt/_load_nbt.pyx":161
+  /* "amulet_nbt/_load_nbt.pyx":179
  * 
  * 
  * def load(             # <<<<<<<<<<<<<<
  *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
  *     *args,
  */
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_2, 0, Py_None);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
   __pyx_t_1 = 0;
@@ -8605,23 +8963,23 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10amulet_nbt_9_load_nbt_7load(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_10amulet_nbt_9_load_nbt_9load(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_10amulet_nbt_9_load_nbt_7load = {"load", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10amulet_nbt_9_load_nbt_7load, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_10amulet_nbt_9_load_nbt_7load(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_10amulet_nbt_9_load_nbt_9load = {"load", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10amulet_nbt_9_load_nbt_9load, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_10amulet_nbt_9_load_nbt_9load(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_filepath_or_buffer = 0;
@@ -8647,15 +9005,15 @@
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __Pyx_GOTREF(__pyx_v_args);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_filepath_or_buffer,&__pyx_n_s_compressed,&__pyx_n_s_count,&__pyx_n_s_offset,&__pyx_n_s_little_endian,&__pyx_n_s_string_decoder,&__pyx_n_s_read_context,0};
     PyObject* values[7] = {0,0,0,0,0,0,0};
-    __pyx_defaults2 *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_self);
+    __pyx_defaults3 *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults3, __pyx_self);
     values[2] = ((PyObject*)((PyObject *)Py_None));
     values[5] = __pyx_dynamic_args->__pyx_arg_string_decoder;
     values[6] = (PyObject *)((struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *)((PyObject *)Py_None));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         default:
@@ -8663,79 +9021,79 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_filepath_or_buffer)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 161, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 179, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (kw_args > 0 && likely(kw_args <= 6)) {
         Py_ssize_t index;
         for (index = 1; index < 7 && kw_args > 0; index++) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, *__pyx_pyargnames[index]);
           if (value) { values[index] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 161, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 179, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, used_pos_args, "load") < 0)) __PYX_ERR(0, 161, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, used_pos_args, "load") < 0)) __PYX_ERR(0, 179, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_filepath_or_buffer = values[0];
     if (values[1]) {
-      __pyx_v_compressed = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_compressed == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 164, __pyx_L3_error)
+      __pyx_v_compressed = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_compressed == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L3_error)
     } else {
       __pyx_v_compressed = ((int)((int)1));
     }
     __pyx_v_count = ((PyObject*)values[2]);
     if (values[3]) {
-      __pyx_v_offset = __Pyx_PyObject_IsTrue(values[3]); if (unlikely((__pyx_v_offset == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L3_error)
+      __pyx_v_offset = __Pyx_PyObject_IsTrue(values[3]); if (unlikely((__pyx_v_offset == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 184, __pyx_L3_error)
     } else {
       __pyx_v_offset = ((int)((int)0));
     }
     if (values[4]) {
-      __pyx_v_little_endian = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_little_endian == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 167, __pyx_L3_error)
+      __pyx_v_little_endian = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_little_endian == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 185, __pyx_L3_error)
     } else {
       __pyx_v_little_endian = ((int)((int)0));
     }
     __pyx_v_string_decoder = values[5];
     __pyx_v_read_context = ((struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *)values[6]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("load", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 161, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("load", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 179, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_args); __pyx_v_args = 0;
   __Pyx_AddTraceback("amulet_nbt._load_nbt.load", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_count), (&PyInt_Type), 1, "count", 1))) __PYX_ERR(0, 165, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_read_context), __pyx_ptype_10amulet_nbt_9_load_nbt_ReadContext, 1, "read_context", 0))) __PYX_ERR(0, 169, __pyx_L1_error)
-  __pyx_r = __pyx_pf_10amulet_nbt_9_load_nbt_6load(__pyx_self, __pyx_v_filepath_or_buffer, __pyx_v_compressed, __pyx_v_count, __pyx_v_offset, __pyx_v_little_endian, __pyx_v_string_decoder, __pyx_v_read_context, __pyx_v_args);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_count), (&PyInt_Type), 1, "count", 1))) __PYX_ERR(0, 183, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_read_context), __pyx_ptype_10amulet_nbt_9_load_nbt_ReadContext, 1, "read_context", 0))) __PYX_ERR(0, 187, __pyx_L1_error)
+  __pyx_r = __pyx_pf_10amulet_nbt_9_load_nbt_8load(__pyx_self, __pyx_v_filepath_or_buffer, __pyx_v_compressed, __pyx_v_count, __pyx_v_offset, __pyx_v_little_endian, __pyx_v_string_decoder, __pyx_v_read_context, __pyx_v_args);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_DECREF(__pyx_v_args);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_6load(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filepath_or_buffer, int __pyx_v_compressed, PyObject *__pyx_v_count, int __pyx_v_offset, int __pyx_v_little_endian, PyObject *__pyx_v_string_decoder, struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *__pyx_v_read_context, PyObject *__pyx_v_args) {
+static PyObject *__pyx_pf_10amulet_nbt_9_load_nbt_8load(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filepath_or_buffer, int __pyx_v_compressed, PyObject *__pyx_v_count, int __pyx_v_offset, int __pyx_v_little_endian, PyObject *__pyx_v_string_decoder, struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *__pyx_v_read_context, PyObject *__pyx_v_args) {
   PyObject *__pyx_v_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *(*__pyx_t_4)(PyObject *);
@@ -8746,248 +9104,248 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("load", 0);
   __Pyx_INCREF(__pyx_v_count);
   __Pyx_INCREF((PyObject *)__pyx_v_read_context);
   __Pyx_INCREF(__pyx_v_args);
 
-  /* "amulet_nbt/_load_nbt.pyx":171
+  /* "amulet_nbt/_load_nbt.pyx":189
  *     ReadContext read_context = None,
  * ) -> Union[NamedTag, Tuple[Union[NamedTag, List[NamedTag]], int]]:
  *     if args:             # <<<<<<<<<<<<<<
  *         warnings.warn("load arguments are going to be keyword only in the future. This function passes the inputs positionally.", FutureWarning)
  *         compressed, *args = args
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_args); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 171, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_args); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 189, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "amulet_nbt/_load_nbt.pyx":172
+    /* "amulet_nbt/_load_nbt.pyx":190
  * ) -> Union[NamedTag, Tuple[Union[NamedTag, List[NamedTag]], int]]:
  *     if args:
  *         warnings.warn("load arguments are going to be keyword only in the future. This function passes the inputs positionally.", FutureWarning)             # <<<<<<<<<<<<<<
  *         compressed, *args = args
  *         if args:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_warnings); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_warnings); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 172, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "amulet_nbt/_load_nbt.pyx":173
+    /* "amulet_nbt/_load_nbt.pyx":191
  *     if args:
  *         warnings.warn("load arguments are going to be keyword only in the future. This function passes the inputs positionally.", FutureWarning)
  *         compressed, *args = args             # <<<<<<<<<<<<<<
  *         if args:
  *             count, *args = args
  */
     {
       Py_ssize_t index = -1;
       PyObject** temps[2] = {&__pyx_t_2};
-      __pyx_t_3 = PyObject_GetIter(__pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
+      __pyx_t_3 = PyObject_GetIter(__pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3);
       for (index=0; index < 1; index++) {
         PyObject* item = __pyx_t_4(__pyx_t_3); if (unlikely(!item)) goto __pyx_L4_unpacking_failed;
         __Pyx_GOTREF(item);
         *(temps[index]) = item;
       }
       goto __pyx_L5_unpacking_done;
       __pyx_L4_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_4 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 173, __pyx_L1_error)
+      __PYX_ERR(0, 191, __pyx_L1_error)
       __pyx_L5_unpacking_done:;
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 173, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 191, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
-    __pyx_t_5 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __pyx_t_5 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_compressed = __pyx_t_1;
     __Pyx_DECREF_SET(__pyx_v_args, ((PyObject*)__pyx_t_5));
     __pyx_t_5 = 0;
 
-    /* "amulet_nbt/_load_nbt.pyx":174
+    /* "amulet_nbt/_load_nbt.pyx":192
  *         warnings.warn("load arguments are going to be keyword only in the future. This function passes the inputs positionally.", FutureWarning)
  *         compressed, *args = args
  *         if args:             # <<<<<<<<<<<<<<
  *             count, *args = args
  *         if args:
  */
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_args); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 174, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_args); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 192, __pyx_L1_error)
     if (__pyx_t_1) {
 
-      /* "amulet_nbt/_load_nbt.pyx":175
+      /* "amulet_nbt/_load_nbt.pyx":193
  *         compressed, *args = args
  *         if args:
  *             count, *args = args             # <<<<<<<<<<<<<<
  *         if args:
  *             offset, *args = args
  */
       {
         Py_ssize_t index = -1;
         PyObject** temps[2] = {&__pyx_t_5};
-        __pyx_t_2 = PyObject_GetIter(__pyx_v_args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
+        __pyx_t_2 = PyObject_GetIter(__pyx_v_args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2);
         for (index=0; index < 1; index++) {
           PyObject* item = __pyx_t_4(__pyx_t_2); if (unlikely(!item)) goto __pyx_L7_unpacking_failed;
           __Pyx_GOTREF(item);
           *(temps[index]) = item;
         }
         goto __pyx_L8_unpacking_done;
         __pyx_L7_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_4 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 175, __pyx_L1_error)
+        __PYX_ERR(0, 193, __pyx_L1_error)
         __pyx_L8_unpacking_done:;
-        if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_5))) __PYX_ERR(0, 175, __pyx_L1_error)
+        if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_5))) __PYX_ERR(0, 193, __pyx_L1_error)
       }
-      __pyx_t_3 = PySequence_List(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L1_error)
+      __pyx_t_3 = PySequence_List(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF_SET(__pyx_v_count, ((PyObject*)__pyx_t_5));
       __pyx_t_5 = 0;
       __Pyx_DECREF_SET(__pyx_v_args, ((PyObject*)__pyx_t_3));
       __pyx_t_3 = 0;
 
-      /* "amulet_nbt/_load_nbt.pyx":174
+      /* "amulet_nbt/_load_nbt.pyx":192
  *         warnings.warn("load arguments are going to be keyword only in the future. This function passes the inputs positionally.", FutureWarning)
  *         compressed, *args = args
  *         if args:             # <<<<<<<<<<<<<<
  *             count, *args = args
  *         if args:
  */
     }
 
-    /* "amulet_nbt/_load_nbt.pyx":176
+    /* "amulet_nbt/_load_nbt.pyx":194
  *         if args:
  *             count, *args = args
  *         if args:             # <<<<<<<<<<<<<<
  *             offset, *args = args
  *         if args:
  */
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_args); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_args); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 194, __pyx_L1_error)
     if (__pyx_t_1) {
 
-      /* "amulet_nbt/_load_nbt.pyx":177
+      /* "amulet_nbt/_load_nbt.pyx":195
  *             count, *args = args
  *         if args:
  *             offset, *args = args             # <<<<<<<<<<<<<<
  *         if args:
  *             little_endian, *args = args
  */
       {
         Py_ssize_t index = -1;
         PyObject** temps[2] = {&__pyx_t_3};
-        __pyx_t_5 = PyObject_GetIter(__pyx_v_args); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 177, __pyx_L1_error)
+        __pyx_t_5 = PyObject_GetIter(__pyx_v_args); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5);
         for (index=0; index < 1; index++) {
           PyObject* item = __pyx_t_4(__pyx_t_5); if (unlikely(!item)) goto __pyx_L10_unpacking_failed;
           __Pyx_GOTREF(item);
           *(temps[index]) = item;
         }
         goto __pyx_L11_unpacking_done;
         __pyx_L10_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __pyx_t_4 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 177, __pyx_L1_error)
+        __PYX_ERR(0, 195, __pyx_L1_error)
         __pyx_L11_unpacking_done:;
-        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 177, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 195, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
-      __pyx_t_2 = PySequence_List(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
+      __pyx_t_2 = PySequence_List(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_v_offset = __pyx_t_1;
       __Pyx_DECREF_SET(__pyx_v_args, ((PyObject*)__pyx_t_2));
       __pyx_t_2 = 0;
 
-      /* "amulet_nbt/_load_nbt.pyx":176
+      /* "amulet_nbt/_load_nbt.pyx":194
  *         if args:
  *             count, *args = args
  *         if args:             # <<<<<<<<<<<<<<
  *             offset, *args = args
  *         if args:
  */
     }
 
-    /* "amulet_nbt/_load_nbt.pyx":178
+    /* "amulet_nbt/_load_nbt.pyx":196
  *         if args:
  *             offset, *args = args
  *         if args:             # <<<<<<<<<<<<<<
  *             little_endian, *args = args
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_args); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 178, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_args); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 196, __pyx_L1_error)
     if (__pyx_t_1) {
 
-      /* "amulet_nbt/_load_nbt.pyx":179
+      /* "amulet_nbt/_load_nbt.pyx":197
  *             offset, *args = args
  *         if args:
  *             little_endian, *args = args             # <<<<<<<<<<<<<<
  * 
  *     if offset and read_context is None:
  */
       {
         Py_ssize_t index = -1;
         PyObject** temps[2] = {&__pyx_t_2};
-        __pyx_t_3 = PyObject_GetIter(__pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L1_error)
+        __pyx_t_3 = PyObject_GetIter(__pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3);
         for (index=0; index < 1; index++) {
           PyObject* item = __pyx_t_4(__pyx_t_3); if (unlikely(!item)) goto __pyx_L13_unpacking_failed;
           __Pyx_GOTREF(item);
           *(temps[index]) = item;
         }
         goto __pyx_L14_unpacking_done;
         __pyx_L13_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_t_4 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 179, __pyx_L1_error)
+        __PYX_ERR(0, 197, __pyx_L1_error)
         __pyx_L14_unpacking_done:;
-        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 179, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       }
-      __pyx_t_5 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 179, __pyx_L1_error)
+      __pyx_t_5 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 197, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_v_little_endian = __pyx_t_1;
       __Pyx_DECREF_SET(__pyx_v_args, ((PyObject*)__pyx_t_5));
       __pyx_t_5 = 0;
 
-      /* "amulet_nbt/_load_nbt.pyx":178
+      /* "amulet_nbt/_load_nbt.pyx":196
  *         if args:
  *             offset, *args = args
  *         if args:             # <<<<<<<<<<<<<<
  *             little_endian, *args = args
  * 
  */
     }
 
-    /* "amulet_nbt/_load_nbt.pyx":171
+    /* "amulet_nbt/_load_nbt.pyx":189
  *     ReadContext read_context = None,
  * ) -> Union[NamedTag, Tuple[Union[NamedTag, List[NamedTag]], int]]:
  *     if args:             # <<<<<<<<<<<<<<
  *         warnings.warn("load arguments are going to be keyword only in the future. This function passes the inputs positionally.", FutureWarning)
  *         compressed, *args = args
  */
   }
 
-  /* "amulet_nbt/_load_nbt.pyx":181
+  /* "amulet_nbt/_load_nbt.pyx":199
  *             little_endian, *args = args
  * 
  *     if offset and read_context is None:             # <<<<<<<<<<<<<<
  *         warnings.warn("load with offset is depreciated. In future versions this function will only return the result. To get the offset pass a ReadContext instance to read_context input.", FutureWarning)
  *         read_context = ReadContext()
  */
   if (__pyx_v_offset) {
@@ -8996,318 +9354,318 @@
     goto __pyx_L16_bool_binop_done;
   }
   __pyx_t_6 = (((PyObject *)__pyx_v_read_context) == Py_None);
   __pyx_t_1 = __pyx_t_6;
   __pyx_L16_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "amulet_nbt/_load_nbt.pyx":182
+    /* "amulet_nbt/_load_nbt.pyx":200
  * 
  *     if offset and read_context is None:
  *         warnings.warn("load with offset is depreciated. In future versions this function will only return the result. To get the offset pass a ReadContext instance to read_context input.", FutureWarning)             # <<<<<<<<<<<<<<
  *         read_context = ReadContext()
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_warnings); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_warnings); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_warn); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_warn); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "amulet_nbt/_load_nbt.pyx":183
+    /* "amulet_nbt/_load_nbt.pyx":201
  *     if offset and read_context is None:
  *         warnings.warn("load with offset is depreciated. In future versions this function will only return the result. To get the offset pass a ReadContext instance to read_context input.", FutureWarning)
  *         read_context = ReadContext()             # <<<<<<<<<<<<<<
  * 
  *     cdef object result
  */
-    __pyx_t_5 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_10amulet_nbt_9_load_nbt_ReadContext)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_10amulet_nbt_9_load_nbt_ReadContext)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF_SET(__pyx_v_read_context, ((struct __pyx_obj_10amulet_nbt_9_load_nbt_ReadContext *)__pyx_t_5));
     __pyx_t_5 = 0;
 
-    /* "amulet_nbt/_load_nbt.pyx":181
+    /* "amulet_nbt/_load_nbt.pyx":199
  *             little_endian, *args = args
  * 
  *     if offset and read_context is None:             # <<<<<<<<<<<<<<
  *         warnings.warn("load with offset is depreciated. In future versions this function will only return the result. To get the offset pass a ReadContext instance to read_context input.", FutureWarning)
  *         read_context = ReadContext()
  */
   }
 
-  /* "amulet_nbt/_load_nbt.pyx":187
+  /* "amulet_nbt/_load_nbt.pyx":205
  *     cdef object result
  * 
  *     if count is None:             # <<<<<<<<<<<<<<
  *         result = _load_one(
  *             filepath_or_buffer,
  */
   __pyx_t_1 = (__pyx_v_count == ((PyObject*)Py_None));
   if (__pyx_t_1) {
 
-    /* "amulet_nbt/_load_nbt.pyx":188
+    /* "amulet_nbt/_load_nbt.pyx":206
  * 
  *     if count is None:
  *         result = _load_one(             # <<<<<<<<<<<<<<
  *             filepath_or_buffer,
  *             compressed=compressed,
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_load_one); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_load_one); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 206, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
 
-    /* "amulet_nbt/_load_nbt.pyx":189
+    /* "amulet_nbt/_load_nbt.pyx":207
  *     if count is None:
  *         result = _load_one(
  *             filepath_or_buffer,             # <<<<<<<<<<<<<<
  *             compressed=compressed,
  *             little_endian=little_endian,
  */
-    __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 206, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_v_filepath_or_buffer);
     __Pyx_GIVEREF(__pyx_v_filepath_or_buffer);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_filepath_or_buffer);
 
-    /* "amulet_nbt/_load_nbt.pyx":190
+    /* "amulet_nbt/_load_nbt.pyx":208
  *         result = _load_one(
  *             filepath_or_buffer,
  *             compressed=compressed,             # <<<<<<<<<<<<<<
  *             little_endian=little_endian,
  *             read_context=read_context,
  */
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 208, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_compressed); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_compressed); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 208, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_compressed, __pyx_t_7) < 0) __PYX_ERR(0, 190, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_compressed, __pyx_t_7) < 0) __PYX_ERR(0, 208, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "amulet_nbt/_load_nbt.pyx":191
+    /* "amulet_nbt/_load_nbt.pyx":209
  *             filepath_or_buffer,
  *             compressed=compressed,
  *             little_endian=little_endian,             # <<<<<<<<<<<<<<
  *             read_context=read_context,
  *             string_decoder=string_decoder
  */
-    __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_little_endian); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 191, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_little_endian); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 209, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_little_endian, __pyx_t_7) < 0) __PYX_ERR(0, 190, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_little_endian, __pyx_t_7) < 0) __PYX_ERR(0, 208, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "amulet_nbt/_load_nbt.pyx":192
+    /* "amulet_nbt/_load_nbt.pyx":210
  *             compressed=compressed,
  *             little_endian=little_endian,
  *             read_context=read_context,             # <<<<<<<<<<<<<<
  *             string_decoder=string_decoder
  *         )
  */
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_read_context, ((PyObject *)__pyx_v_read_context)) < 0) __PYX_ERR(0, 190, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_read_context, ((PyObject *)__pyx_v_read_context)) < 0) __PYX_ERR(0, 208, __pyx_L1_error)
 
-    /* "amulet_nbt/_load_nbt.pyx":193
+    /* "amulet_nbt/_load_nbt.pyx":211
  *             little_endian=little_endian,
  *             read_context=read_context,
  *             string_decoder=string_decoder             # <<<<<<<<<<<<<<
  *         )
  *     else:
  */
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_string_decoder, __pyx_v_string_decoder) < 0) __PYX_ERR(0, 190, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_string_decoder, __pyx_v_string_decoder) < 0) __PYX_ERR(0, 208, __pyx_L1_error)
 
-    /* "amulet_nbt/_load_nbt.pyx":188
+    /* "amulet_nbt/_load_nbt.pyx":206
  * 
  *     if count is None:
  *         result = _load_one(             # <<<<<<<<<<<<<<
  *             filepath_or_buffer,
  *             compressed=compressed,
  */
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 206, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_result = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "amulet_nbt/_load_nbt.pyx":187
+    /* "amulet_nbt/_load_nbt.pyx":205
  *     cdef object result
  * 
  *     if count is None:             # <<<<<<<<<<<<<<
  *         result = _load_one(
  *             filepath_or_buffer,
  */
     goto __pyx_L18;
   }
 
-  /* "amulet_nbt/_load_nbt.pyx":196
+  /* "amulet_nbt/_load_nbt.pyx":214
  *         )
  *     else:
- *         warnings.warn("load with count is depreciated. Use load_many", DeprecationWarning)             # <<<<<<<<<<<<<<
- *         result = load_many(
+ *         warnings.warn("load with count is depreciated. Use load_array", DeprecationWarning)             # <<<<<<<<<<<<<<
+ *         result = load_array(
  *             filepath_or_buffer,
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_warnings); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 196, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_warnings); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 214, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 196, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 214, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 196, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 214, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "amulet_nbt/_load_nbt.pyx":197
+    /* "amulet_nbt/_load_nbt.pyx":215
  *     else:
- *         warnings.warn("load with count is depreciated. Use load_many", DeprecationWarning)
- *         result = load_many(             # <<<<<<<<<<<<<<
+ *         warnings.warn("load with count is depreciated. Use load_array", DeprecationWarning)
+ *         result = load_array(             # <<<<<<<<<<<<<<
  *             filepath_or_buffer,
  *             count=count,
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_load_many); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_load_array); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
 
-    /* "amulet_nbt/_load_nbt.pyx":198
- *         warnings.warn("load with count is depreciated. Use load_many", DeprecationWarning)
- *         result = load_many(
+    /* "amulet_nbt/_load_nbt.pyx":216
+ *         warnings.warn("load with count is depreciated. Use load_array", DeprecationWarning)
+ *         result = load_array(
  *             filepath_or_buffer,             # <<<<<<<<<<<<<<
  *             count=count,
  *             compressed=compressed,
  */
-    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_filepath_or_buffer);
     __Pyx_GIVEREF(__pyx_v_filepath_or_buffer);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_filepath_or_buffer);
 
-    /* "amulet_nbt/_load_nbt.pyx":199
- *         result = load_many(
+    /* "amulet_nbt/_load_nbt.pyx":217
+ *         result = load_array(
  *             filepath_or_buffer,
  *             count=count,             # <<<<<<<<<<<<<<
  *             compressed=compressed,
  *             little_endian=little_endian,
  */
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 217, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_count, __pyx_v_count) < 0) __PYX_ERR(0, 199, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_count, __pyx_v_count) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
 
-    /* "amulet_nbt/_load_nbt.pyx":200
+    /* "amulet_nbt/_load_nbt.pyx":218
  *             filepath_or_buffer,
  *             count=count,
  *             compressed=compressed,             # <<<<<<<<<<<<<<
  *             little_endian=little_endian,
  *             read_context=read_context,
  */
-    __pyx_t_5 = __Pyx_PyBool_FromLong(__pyx_v_compressed); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 200, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBool_FromLong(__pyx_v_compressed); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 218, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_compressed, __pyx_t_5) < 0) __PYX_ERR(0, 199, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_compressed, __pyx_t_5) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "amulet_nbt/_load_nbt.pyx":201
+    /* "amulet_nbt/_load_nbt.pyx":219
  *             count=count,
  *             compressed=compressed,
  *             little_endian=little_endian,             # <<<<<<<<<<<<<<
  *             read_context=read_context,
  *             string_decoder=string_decoder
  */
-    __pyx_t_5 = __Pyx_PyBool_FromLong(__pyx_v_little_endian); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBool_FromLong(__pyx_v_little_endian); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_little_endian, __pyx_t_5) < 0) __PYX_ERR(0, 199, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_little_endian, __pyx_t_5) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "amulet_nbt/_load_nbt.pyx":202
+    /* "amulet_nbt/_load_nbt.pyx":220
  *             compressed=compressed,
  *             little_endian=little_endian,
  *             read_context=read_context,             # <<<<<<<<<<<<<<
  *             string_decoder=string_decoder
  *         )
  */
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_read_context, ((PyObject *)__pyx_v_read_context)) < 0) __PYX_ERR(0, 199, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_read_context, ((PyObject *)__pyx_v_read_context)) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
 
-    /* "amulet_nbt/_load_nbt.pyx":203
+    /* "amulet_nbt/_load_nbt.pyx":221
  *             little_endian=little_endian,
  *             read_context=read_context,
  *             string_decoder=string_decoder             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_string_decoder, __pyx_v_string_decoder) < 0) __PYX_ERR(0, 199, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_string_decoder, __pyx_v_string_decoder) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
 
-    /* "amulet_nbt/_load_nbt.pyx":197
+    /* "amulet_nbt/_load_nbt.pyx":215
  *     else:
- *         warnings.warn("load with count is depreciated. Use load_many", DeprecationWarning)
- *         result = load_many(             # <<<<<<<<<<<<<<
+ *         warnings.warn("load with count is depreciated. Use load_array", DeprecationWarning)
+ *         result = load_array(             # <<<<<<<<<<<<<<
  *             filepath_or_buffer,
  *             count=count,
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_result = __pyx_t_5;
     __pyx_t_5 = 0;
   }
   __pyx_L18:;
 
-  /* "amulet_nbt/_load_nbt.pyx":206
+  /* "amulet_nbt/_load_nbt.pyx":224
  *         )
  * 
  *     if offset:             # <<<<<<<<<<<<<<
  *         # depreciated
  *         return result, read_context.offset
  */
   if (__pyx_v_offset) {
 
-    /* "amulet_nbt/_load_nbt.pyx":208
+    /* "amulet_nbt/_load_nbt.pyx":226
  *     if offset:
  *         # depreciated
  *         return result, read_context.offset             # <<<<<<<<<<<<<<
  *     else:
  *         return result
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_read_context->offset); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_read_context->offset); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 226, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 226, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_v_result);
     __Pyx_GIVEREF(__pyx_v_result);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_result);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_5);
     __pyx_t_5 = 0;
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "amulet_nbt/_load_nbt.pyx":206
+    /* "amulet_nbt/_load_nbt.pyx":224
  *         )
  * 
  *     if offset:             # <<<<<<<<<<<<<<
  *         # depreciated
  *         return result, read_context.offset
  */
   }
 
-  /* "amulet_nbt/_load_nbt.pyx":210
+  /* "amulet_nbt/_load_nbt.pyx":228
  *         return result, read_context.offset
  *     else:
  *         return result             # <<<<<<<<<<<<<<
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_result);
     __pyx_r = __pyx_v_result;
     goto __pyx_L0;
   }
 
-  /* "amulet_nbt/_load_nbt.pyx":161
+  /* "amulet_nbt/_load_nbt.pyx":179
  * 
  * 
  * def load(             # <<<<<<<<<<<<<<
  *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
  *     *args,
  */
 
@@ -9487,15 +9845,15 @@
 #endif
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
     {&__pyx_n_s_BinaryIO, __pyx_k_BinaryIO, sizeof(__pyx_k_BinaryIO), 0, 0, 1, 1},
     {&__pyx_n_s_BytesIO, __pyx_k_BytesIO, sizeof(__pyx_k_BytesIO), 0, 0, 1, 1},
-    {&__pyx_kp_u_Count_must_be_1_or_more, __pyx_k_Count_must_be_1_or_more, sizeof(__pyx_k_Count_must_be_1_or_more), 0, 1, 0, 0},
+    {&__pyx_kp_u_Count_must_be_1_or_higher, __pyx_k_Count_must_be_1_or_higher, sizeof(__pyx_k_Count_must_be_1_or_higher), 0, 1, 0, 0},
     {&__pyx_n_s_DecoderType, __pyx_k_DecoderType, sizeof(__pyx_k_DecoderType), 0, 0, 1, 1},
     {&__pyx_n_s_DeprecationWarning, __pyx_k_DeprecationWarning, sizeof(__pyx_k_DeprecationWarning), 0, 0, 1, 1},
     {&__pyx_n_s_EOFError, __pyx_k_EOFError, sizeof(__pyx_k_EOFError), 0, 0, 1, 1},
     {&__pyx_n_s_FutureWarning, __pyx_k_FutureWarning, sizeof(__pyx_k_FutureWarning), 0, 0, 1, 1},
     {&__pyx_n_s_GzipFile, __pyx_k_GzipFile, sizeof(__pyx_k_GzipFile), 0, 0, 1, 1},
     {&__pyx_n_s_IOError, __pyx_k_IOError, sizeof(__pyx_k_IOError), 0, 0, 1, 1},
     {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
@@ -9510,17 +9868,17 @@
     {&__pyx_kp_u_There_is_no_file_at, __pyx_k_There_is_no_file_at, sizeof(__pyx_k_There_is_no_file_at), 0, 1, 0, 0},
     {&__pyx_n_s_Tuple, __pyx_k_Tuple, sizeof(__pyx_k_Tuple), 0, 0, 1, 1},
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_n_s_Union, __pyx_k_Union, sizeof(__pyx_k_Union), 0, 0, 1, 1},
     {&__pyx_kp_s_Union_NamedTag_Tuple_Union_Named, __pyx_k_Union_NamedTag_Tuple_Union_Named, sizeof(__pyx_k_Union_NamedTag_Tuple_Union_Named), 0, 0, 1, 0},
     {&__pyx_kp_s_Union_str_bytes_BinaryIO_memoryv, __pyx_k_Union_str_bytes_BinaryIO_memoryv, sizeof(__pyx_k_Union_str_bytes_BinaryIO_memoryv), 0, 0, 1, 0},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
-    {&__pyx_n_s__10, __pyx_k__10, sizeof(__pyx_k__10), 0, 0, 1, 1},
-    {&__pyx_kp_u__11, __pyx_k__11, sizeof(__pyx_k__11), 0, 1, 0, 0},
-    {&__pyx_n_s__24, __pyx_k__24, sizeof(__pyx_k__24), 0, 0, 1, 1},
+    {&__pyx_n_s__11, __pyx_k__11, sizeof(__pyx_k__11), 0, 0, 1, 1},
+    {&__pyx_kp_u__12, __pyx_k__12, sizeof(__pyx_k__12), 0, 1, 0, 0},
+    {&__pyx_n_s__27, __pyx_k__27, sizeof(__pyx_k__27), 0, 0, 1, 1},
     {&__pyx_kp_b__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 0, 0, 0},
     {&__pyx_n_s_amulet_nbt__load_nbt, __pyx_k_amulet_nbt__load_nbt, sizeof(__pyx_k_amulet_nbt__load_nbt), 0, 0, 1, 1},
     {&__pyx_kp_s_amulet_nbt__load_nbt_pyx, __pyx_k_amulet_nbt__load_nbt_pyx, sizeof(__pyx_k_amulet_nbt__load_nbt_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_bool, __pyx_k_bool, sizeof(__pyx_k_bool), 0, 0, 1, 1},
     {&__pyx_n_s_buffer, __pyx_k_buffer, sizeof(__pyx_k_buffer), 0, 0, 1, 1},
@@ -9553,15 +9911,17 @@
     {&__pyx_n_s_io, __pyx_k_io, sizeof(__pyx_k_io), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
     {&__pyx_n_s_isfile, __pyx_k_isfile, sizeof(__pyx_k_isfile), 0, 0, 1, 1},
     {&__pyx_n_s_little_endian, __pyx_k_little_endian, sizeof(__pyx_k_little_endian), 0, 0, 1, 1},
     {&__pyx_n_s_load, __pyx_k_load, sizeof(__pyx_k_load), 0, 0, 1, 1},
     {&__pyx_kp_u_load_arguments_are_going_to_be_k, __pyx_k_load_arguments_are_going_to_be_k, sizeof(__pyx_k_load_arguments_are_going_to_be_k), 0, 1, 0, 0},
+    {&__pyx_n_s_load_array, __pyx_k_load_array, sizeof(__pyx_k_load_array), 0, 0, 1, 1},
     {&__pyx_n_s_load_many, __pyx_k_load_many, sizeof(__pyx_k_load_many), 0, 0, 1, 1},
+    {&__pyx_kp_u_load_many_is_depreciated_Use_loa, __pyx_k_load_many_is_depreciated_Use_loa, sizeof(__pyx_k_load_many_is_depreciated_Use_loa), 0, 1, 0, 0},
     {&__pyx_n_s_load_one, __pyx_k_load_one, sizeof(__pyx_k_load_one), 0, 0, 1, 1},
     {&__pyx_kp_u_load_with_count_is_depreciated_U, __pyx_k_load_with_count_is_depreciated_U, sizeof(__pyx_k_load_with_count_is_depreciated_U), 0, 1, 0, 0},
     {&__pyx_kp_u_load_with_offset_is_depreciated, __pyx_k_load_with_offset_is_depreciated, sizeof(__pyx_k_load_with_offset_is_depreciated), 0, 1, 0, 0},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_s_mutf8, __pyx_k_mutf8, sizeof(__pyx_k_mutf8), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
@@ -9605,40 +9965,40 @@
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_IOError = __Pyx_GetBuiltinName(__pyx_n_s_IOError); if (!__pyx_builtin_IOError) __PYX_ERR(0, 39, __pyx_L1_error)
   __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 53, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_EOFError = __Pyx_GetBuiltinName(__pyx_n_s_EOFError); if (!__pyx_builtin_EOFError) __PYX_ERR(0, 129, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 146, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 152, __pyx_L1_error)
-  __pyx_builtin_FutureWarning = __Pyx_GetBuiltinName(__pyx_n_s_FutureWarning); if (!__pyx_builtin_FutureWarning) __PYX_ERR(0, 172, __pyx_L1_error)
-  __pyx_builtin_DeprecationWarning = __Pyx_GetBuiltinName(__pyx_n_s_DeprecationWarning); if (!__pyx_builtin_DeprecationWarning) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_builtin_DeprecationWarning = __Pyx_GetBuiltinName(__pyx_n_s_DeprecationWarning); if (!__pyx_builtin_DeprecationWarning) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_builtin_FutureWarning = __Pyx_GetBuiltinName(__pyx_n_s_FutureWarning); if (!__pyx_builtin_FutureWarning) __PYX_ERR(0, 190, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 986, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(2, 986, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(2, 992, __pyx_L1_error)
@@ -9665,124 +10025,147 @@
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_buffer_is_empty); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "amulet_nbt/_load_nbt.pyx":146
  * ) -> List[NamedTag]:
- *     if count < 1:
- *         raise ValueError("Count must be 1 or more.")             # <<<<<<<<<<<<<<
+ *     if count < -1:
+ *         raise ValueError("Count must be -1 or higher")             # <<<<<<<<<<<<<<
  *     cdef BufferContext buffer = get_buffer(filepath_or_buffer, compressed)
- *     if buffer.size < 1:
+ *     cdef list results = []
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_Count_must_be_1_or_more); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_Count_must_be_1_or_higher); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "amulet_nbt/_load_nbt.pyx":172
+  /* "amulet_nbt/_load_nbt.pyx":175
+ *     string_decoder: DecoderType = decode_modified_utf8
+ * ):
+ *     warnings.warn("load_many is depreciated. Use load_array instead.", DeprecationWarning)             # <<<<<<<<<<<<<<
+ *     return load_array(filepath_or_buffer, count, compressed, little_endian, read_context, string_decoder)
+ * 
+ */
+  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_kp_u_load_many_is_depreciated_Use_loa, __pyx_builtin_DeprecationWarning); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+
+  /* "amulet_nbt/_load_nbt.pyx":190
  * ) -> Union[NamedTag, Tuple[Union[NamedTag, List[NamedTag]], int]]:
  *     if args:
  *         warnings.warn("load arguments are going to be keyword only in the future. This function passes the inputs positionally.", FutureWarning)             # <<<<<<<<<<<<<<
  *         compressed, *args = args
  *         if args:
  */
-  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_kp_u_load_arguments_are_going_to_be_k, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 172, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_kp_u_load_arguments_are_going_to_be_k, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "amulet_nbt/_load_nbt.pyx":182
+  /* "amulet_nbt/_load_nbt.pyx":200
  * 
  *     if offset and read_context is None:
  *         warnings.warn("load with offset is depreciated. In future versions this function will only return the result. To get the offset pass a ReadContext instance to read_context input.", FutureWarning)             # <<<<<<<<<<<<<<
  *         read_context = ReadContext()
  * 
  */
-  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_kp_u_load_with_offset_is_depreciated, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 182, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_kp_u_load_with_offset_is_depreciated, __pyx_builtin_FutureWarning); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "amulet_nbt/_load_nbt.pyx":196
+  /* "amulet_nbt/_load_nbt.pyx":214
  *         )
  *     else:
- *         warnings.warn("load with count is depreciated. Use load_many", DeprecationWarning)             # <<<<<<<<<<<<<<
- *         result = load_many(
+ *         warnings.warn("load with count is depreciated. Use load_array", DeprecationWarning)             # <<<<<<<<<<<<<<
+ *         result = load_array(
  *             filepath_or_buffer,
  */
-  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_kp_u_load_with_count_is_depreciated_U, __pyx_builtin_DeprecationWarning); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 196, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__10 = PyTuple_Pack(2, __pyx_kp_u_load_with_count_is_depreciated_U, __pyx_builtin_DeprecationWarning); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 214, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "amulet_nbt/_load_nbt.pyx":35
  * 
  * 
  * cpdef inline bytes safe_gunzip(bytes data):             # <<<<<<<<<<<<<<
  *     if data[:2] == b'\x1f\x8b':  # if the first two bytes are this it should be gzipped
  *         try:
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_n_s_data); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 35, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_amulet_nbt__load_nbt_pyx, __pyx_n_s_safe_gunzip, 35, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_n_s_data); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_amulet_nbt__load_nbt_pyx, __pyx_n_s_safe_gunzip, 35, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 35, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_tuple__16 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(1, 3, __pyx_L1_error)
 
   /* "amulet_nbt/_load_nbt.pyx":119
  * 
  * 
  * def _load_one(             # <<<<<<<<<<<<<<
  *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
  *     *,
  */
-  __pyx_tuple__18 = PyTuple_Pack(7, __pyx_n_s_filepath_or_buffer, __pyx_n_s_compressed, __pyx_n_s_little_endian, __pyx_n_s_read_context, __pyx_n_s_string_decoder, __pyx_n_s_buffer, __pyx_n_s_tag); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 119, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_amulet_nbt__load_nbt_pyx, __pyx_n_s_load_one, 119, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(7, __pyx_n_s_filepath_or_buffer, __pyx_n_s_compressed, __pyx_n_s_little_endian, __pyx_n_s_read_context, __pyx_n_s_string_decoder, __pyx_n_s_buffer, __pyx_n_s_tag); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_amulet_nbt__load_nbt_pyx, __pyx_n_s_load_one, 119, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 119, __pyx_L1_error)
 
   /* "amulet_nbt/_load_nbt.pyx":136
  * 
  * 
+ * def load_array(             # <<<<<<<<<<<<<<
+ *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
+ *     *,
+ */
+  __pyx_tuple__21 = PyTuple_Pack(9, __pyx_n_s_filepath_or_buffer, __pyx_n_s_count, __pyx_n_s_compressed, __pyx_n_s_little_endian, __pyx_n_s_read_context, __pyx_n_s_string_decoder, __pyx_n_s_buffer, __pyx_n_s_results, __pyx_n_s_i); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_amulet_nbt__load_nbt_pyx, __pyx_n_s_load_array, 136, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 136, __pyx_L1_error)
+
+  /* "amulet_nbt/_load_nbt.pyx":166
+ * 
+ * 
  * def load_many(             # <<<<<<<<<<<<<<
  *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
  *     *,
  */
-  __pyx_tuple__20 = PyTuple_Pack(9, __pyx_n_s_filepath_or_buffer, __pyx_n_s_count, __pyx_n_s_compressed, __pyx_n_s_little_endian, __pyx_n_s_read_context, __pyx_n_s_string_decoder, __pyx_n_s_buffer, __pyx_n_s_results, __pyx_n_s_i); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 136, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_amulet_nbt__load_nbt_pyx, __pyx_n_s_load_many, 136, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(6, __pyx_n_s_filepath_or_buffer, __pyx_n_s_count, __pyx_n_s_compressed, __pyx_n_s_little_endian, __pyx_n_s_read_context, __pyx_n_s_string_decoder); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_amulet_nbt__load_nbt_pyx, __pyx_n_s_load_many, 166, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 166, __pyx_L1_error)
 
-  /* "amulet_nbt/_load_nbt.pyx":161
+  /* "amulet_nbt/_load_nbt.pyx":179
  * 
  * 
  * def load(             # <<<<<<<<<<<<<<
  *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
  *     *args,
  */
-  __pyx_tuple__22 = PyTuple_Pack(9, __pyx_n_s_filepath_or_buffer, __pyx_n_s_compressed, __pyx_n_s_count, __pyx_n_s_offset, __pyx_n_s_little_endian, __pyx_n_s_string_decoder, __pyx_n_s_read_context, __pyx_n_s_args, __pyx_n_s_result); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_amulet_nbt__load_nbt_pyx, __pyx_n_s_load, 161, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(9, __pyx_n_s_filepath_or_buffer, __pyx_n_s_compressed, __pyx_n_s_count, __pyx_n_s_offset, __pyx_n_s_little_endian, __pyx_n_s_string_decoder, __pyx_n_s_read_context, __pyx_n_s_args, __pyx_n_s_result); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_amulet_nbt__load_nbt_pyx, __pyx_n_s_load, 179, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -10512,36 +10895,36 @@
   /* "amulet_nbt/_load_nbt.pyx":35
  * 
  * 
  * cpdef inline bytes safe_gunzip(bytes data):             # <<<<<<<<<<<<<<
  *     if data[:2] == b'\x1f\x8b':  # if the first two bytes are this it should be gzipped
  *         try:
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10amulet_nbt_9_load_nbt_1safe_gunzip, 0, __pyx_n_s_safe_gunzip, NULL, __pyx_n_s_amulet_nbt__load_nbt, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10amulet_nbt_9_load_nbt_1safe_gunzip, 0, __pyx_n_s_safe_gunzip, NULL, __pyx_n_s_amulet_nbt__load_nbt, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_safe_gunzip, __pyx_t_3) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10amulet_nbt_9_load_nbt_11ReadContext_3__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ReadContext___reduce_cython, NULL, __pyx_n_s_amulet_nbt__load_nbt, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10amulet_nbt_9_load_nbt_11ReadContext_3__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ReadContext___reduce_cython, NULL, __pyx_n_s_amulet_nbt__load_nbt, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10amulet_nbt_9_load_nbt_11ReadContext_5__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ReadContext___setstate_cython, NULL, __pyx_n_s_amulet_nbt__load_nbt, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10amulet_nbt_9_load_nbt_11ReadContext_5__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ReadContext___setstate_cython, NULL, __pyx_n_s_amulet_nbt__load_nbt, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "amulet_nbt/_load_nbt.pyx":119
  * 
  * 
@@ -10552,15 +10935,15 @@
   __pyx_t_3 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_filepath_or_buffer, __pyx_kp_s_Union_str_bytes_BinaryIO_memoryv) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_compressed, __pyx_n_s_bool) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_little_endian, __pyx_n_s_bool) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_string_decoder, __pyx_n_s_DecoderType) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_NamedTag) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10amulet_nbt_9_load_nbt_3_load_one, 0, __pyx_n_s_load_one, NULL, __pyx_n_s_amulet_nbt__load_nbt, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10amulet_nbt_9_load_nbt_3_load_one, 0, __pyx_n_s_load_one, NULL, __pyx_n_s_amulet_nbt__load_nbt, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults), 1)) __PYX_ERR(0, 119, __pyx_L1_error)
 
   /* "amulet_nbt/_load_nbt.pyx":125
  *     bint little_endian: bool = False,
  *     ReadContext read_context = None,
  *     string_decoder: DecoderType = decode_modified_utf8             # <<<<<<<<<<<<<<
@@ -10568,103 +10951,138 @@
  *     cdef BufferContext buffer = get_buffer(filepath_or_buffer, compressed)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_decode_modified_utf8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_t_2)->__pyx_arg_string_decoder = __pyx_t_4;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_10amulet_nbt_9_load_nbt_8__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_10amulet_nbt_9_load_nbt_10__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_load_one, __pyx_t_2) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "amulet_nbt/_load_nbt.pyx":136
  * 
  * 
- * def load_many(             # <<<<<<<<<<<<<<
+ * def load_array(             # <<<<<<<<<<<<<<
  *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
  *     *,
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_filepath_or_buffer, __pyx_kp_s_Union_str_bytes_BinaryIO_memoryv) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_compressed, __pyx_n_s_bool) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_little_endian, __pyx_n_s_bool) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_string_decoder, __pyx_n_s_DecoderType) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_List_NamedTag) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10amulet_nbt_9_load_nbt_5load_many, 0, __pyx_n_s_load_many, NULL, __pyx_n_s_amulet_nbt__load_nbt, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10amulet_nbt_9_load_nbt_5load_array, 0, __pyx_n_s_load_array, NULL, __pyx_n_s_amulet_nbt__load_nbt, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (!__Pyx_CyFunction_InitDefaults(__pyx_t_3, sizeof(__pyx_defaults1), 1)) __PYX_ERR(0, 136, __pyx_L1_error)
 
   /* "amulet_nbt/_load_nbt.pyx":143
  *     bint little_endian: bool = False,
  *     ReadContext read_context = None,
  *     string_decoder: DecoderType = decode_modified_utf8             # <<<<<<<<<<<<<<
  * ) -> List[NamedTag]:
- *     if count < 1:
+ *     if count < -1:
  */
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_decode_modified_utf8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_t_3)->__pyx_arg_string_decoder = __pyx_t_4;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_3, __pyx_pf_10amulet_nbt_9_load_nbt_10__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_3, __pyx_pf_10amulet_nbt_9_load_nbt_12__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_load_many, __pyx_t_3) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_load_array, __pyx_t_3) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "amulet_nbt/_load_nbt.pyx":161
+  /* "amulet_nbt/_load_nbt.pyx":166
+ * 
+ * 
+ * def load_many(             # <<<<<<<<<<<<<<
+ *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
+ *     *,
+ */
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_filepath_or_buffer, __pyx_kp_s_Union_str_bytes_BinaryIO_memoryv) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_compressed, __pyx_n_s_bool) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_little_endian, __pyx_n_s_bool) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_string_decoder, __pyx_n_s_DecoderType) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10amulet_nbt_9_load_nbt_7load_many, 0, __pyx_n_s_load_many, NULL, __pyx_n_s_amulet_nbt__load_nbt, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults2), 1)) __PYX_ERR(0, 166, __pyx_L1_error)
+
+  /* "amulet_nbt/_load_nbt.pyx":173
+ *     bint little_endian: bool = False,
+ *     ReadContext read_context = None,
+ *     string_decoder: DecoderType = decode_modified_utf8             # <<<<<<<<<<<<<<
+ * ):
+ *     warnings.warn("load_many is depreciated. Use load_array instead.", DeprecationWarning)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_decode_modified_utf8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_t_2)->__pyx_arg_string_decoder = __pyx_t_4;
+  __Pyx_GIVEREF(__pyx_t_4);
+  __pyx_t_4 = 0;
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_10amulet_nbt_9_load_nbt_14__defaults__);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_load_many, __pyx_t_2) < 0) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "amulet_nbt/_load_nbt.pyx":179
  * 
  * 
  * def load(             # <<<<<<<<<<<<<<
  *     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
  *     *args,
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_filepath_or_buffer, __pyx_kp_s_Union_str_bytes_BinaryIO_memoryv) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_compressed, __pyx_n_s_bool) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_count, __pyx_n_s_int) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_offset, __pyx_n_s_bool) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_little_endian, __pyx_n_s_bool) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_string_decoder, __pyx_n_s_DecoderType) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_kp_s_Union_NamedTag_Tuple_Union_Named) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10amulet_nbt_9_load_nbt_7load, 0, __pyx_n_s_load, NULL, __pyx_n_s_amulet_nbt__load_nbt, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults2), 1)) __PYX_ERR(0, 161, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_filepath_or_buffer, __pyx_kp_s_Union_str_bytes_BinaryIO_memoryv) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_compressed, __pyx_n_s_bool) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_count, __pyx_n_s_int) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_offset, __pyx_n_s_bool) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_little_endian, __pyx_n_s_bool) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_string_decoder, __pyx_n_s_DecoderType) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_Union_NamedTag_Tuple_Union_Named) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10amulet_nbt_9_load_nbt_9load, 0, __pyx_n_s_load, NULL, __pyx_n_s_amulet_nbt__load_nbt, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_3, sizeof(__pyx_defaults3), 1)) __PYX_ERR(0, 179, __pyx_L1_error)
 
-  /* "amulet_nbt/_load_nbt.pyx":168
+  /* "amulet_nbt/_load_nbt.pyx":186
  *     bint offset: bool = False,
  *     bint little_endian: bool = False,
  *     string_decoder: DecoderType = decode_modified_utf8,             # <<<<<<<<<<<<<<
  *     ReadContext read_context = None,
  * ) -> Union[NamedTag, Tuple[Union[NamedTag, List[NamedTag]], int]]:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_decode_modified_utf8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_decode_modified_utf8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_t_2)->__pyx_arg_string_decoder = __pyx_t_4;
+  __Pyx_CyFunction_Defaults(__pyx_defaults3, __pyx_t_3)->__pyx_arg_string_decoder = __pyx_t_4;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_10amulet_nbt_9_load_nbt_12__defaults__);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_load, __pyx_t_2) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_3, __pyx_pf_10amulet_nbt_9_load_nbt_16__defaults__);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_load, __pyx_t_3) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "amulet_nbt/_load_nbt.pyx":1
  * import gzip             # <<<<<<<<<<<<<<
  * import warnings
  * import zlib
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -13182,15 +13600,15 @@
         return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
     }
     return module;
 }
 #endif
 static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
 #if PY_MAJOR_VERSION < 3
-    PyObject *module, *from_list, *star = __pyx_n_s__10;
+    PyObject *module, *from_list, *star = __pyx_n_s__11;
     CYTHON_UNUSED_VAR(parts_tuple);
     from_list = PyList_New(1);
     if (unlikely(!from_list))
         return NULL;
     Py_INCREF(star);
     PyList_SET_ITEM(from_list, 0, star);
     module = __Pyx_Import(name, from_list, 0);
@@ -13245,15 +13663,15 @@
         PyObject* module_dot = 0;
         PyObject* full_name = 0;
         PyErr_Clear();
         module_name_str = PyModule_GetName(module);
         if (unlikely(!module_name_str)) { goto modbad; }
         module_name = PyUnicode_FromString(module_name_str);
         if (unlikely(!module_name)) { goto modbad; }
-        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__11);
+        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__12);
         if (unlikely(!module_dot)) { goto modbad; }
         full_name = PyUnicode_Concat(module_dot, name);
         if (unlikely(!full_name)) { goto modbad; }
         #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
         {
             PyObject *modules = PyImport_GetModuleDict();
             if (unlikely(!modules))
@@ -15491,15 +15909,15 @@
 static __Pyx_TypeName
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
-        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__24));
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__27));
     }
     return name;
 }
 #endif
 
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
```

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_load_nbt.pyx` & `amulet-nbt-2.1.0/amulet_nbt/_load_nbt.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -129,39 +129,57 @@
         raise EOFError("buffer is empty")
     cdef NamedTag tag = load_named_tag(buffer, little_endian, string_decoder)
     if read_context is not None:
         read_context.offset = buffer.offset
     return tag
 
 
-def load_many(
+def load_array(
     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
     *,
     int count = 1,
     bint compressed: bool=True,
     bint little_endian: bool = False,
     ReadContext read_context = None,
     string_decoder: DecoderType = decode_modified_utf8
 ) -> List[NamedTag]:
-    if count < 1:
-        raise ValueError("Count must be 1 or more.")
+    if count < -1:
+        raise ValueError("Count must be -1 or higher")
     cdef BufferContext buffer = get_buffer(filepath_or_buffer, compressed)
-    if buffer.size < 1:
-        raise EOFError("buffer is empty")
     cdef list results = []
     cdef size_t i
-    for i in range(count):
-        results.append(
-            load_named_tag(buffer, little_endian, string_decoder)
-        )
+    if count == -1:
+        while buffer.offset < buffer.size:
+            results.append(
+                load_named_tag(buffer, little_endian, string_decoder)
+            )
+    else:
+        for i in range(count):
+            results.append(
+                load_named_tag(buffer, little_endian, string_decoder)
+            )
+
     if read_context is not None:
         read_context.offset = buffer.offset
     return results
 
 
+def load_many(
+    object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
+    *,
+    int count = 1,
+    bint compressed: bool=True,
+    bint little_endian: bool = False,
+    ReadContext read_context = None,
+    string_decoder: DecoderType = decode_modified_utf8
+):
+    warnings.warn("load_many is depreciated. Use load_array instead.", DeprecationWarning)
+    return load_array(filepath_or_buffer, count, compressed, little_endian, read_context, string_decoder)
+
+
 def load(
     object filepath_or_buffer: Union[str, bytes, BinaryIO, memoryview, None],
     *args,
     bint compressed: bool=True,
     object count: int = None,
     bint offset: bool = False,
     bint little_endian: bool = False,
@@ -189,16 +207,16 @@
             filepath_or_buffer,
             compressed=compressed,
             little_endian=little_endian,
             read_context=read_context,
             string_decoder=string_decoder
         )
     else:
-        warnings.warn("load with count is depreciated. Use load_many", DeprecationWarning)
-        result = load_many(
+        warnings.warn("load with count is depreciated. Use load_array", DeprecationWarning)
+        result = load_array(
             filepath_or_buffer,
             count=count,
             compressed=compressed,
             little_endian=little_endian,
             read_context=read_context,
             string_decoder=string_decoder
         )
```

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_load_snbt.c` & `amulet-nbt-2.1.0/amulet_nbt/_load_snbt.c`

 * *Files 0% similar despite different names*

```diff
@@ -1390,195 +1390,195 @@
   "amulet_nbt\\\\_string.pxd",
   "amulet_nbt\\\\_compound.pxd",
   "amulet_nbt\\\\_list.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* #### Code section: numeric_typedefs ### */
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":731
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":731
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":732
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":732
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":733
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":734
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":738
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":738
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":739
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":739
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":740
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":741
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":745
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":745
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":746
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":746
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":755
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":755
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":756
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":756
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":757
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":759
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":759
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":760
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":760
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":761
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":761
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":763
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":764
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":766
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":766
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":767
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":767
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":768
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":768
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1669,42 +1669,42 @@
  * cdef char read_byte(BufferContext buffer) except? -1
  */
 struct __pyx_opt_args_10amulet_nbt_5_util_to_little_endian {
   int __pyx_n;
   int little_endian;
 };
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":770
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":770
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":771
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":772
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":774
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":774
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -4313,261 +4313,261 @@
 #define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
 #define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
 #define __pyx_tuple__18 __pyx_mstate_global->__pyx_tuple__18
 #define __pyx_tuple__19 __pyx_mstate_global->__pyx_tuple__19
 #define __pyx_codeobj__20 __pyx_mstate_global->__pyx_codeobj__20
 /* #### Code section: module_code ### */
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":245
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":251
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":257
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":263
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":271
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":278
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":284
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":776
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4576,29 +4576,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4609,15 +4609,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":779
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4626,29 +4626,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4659,15 +4659,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":782
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4676,29 +4676,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4709,15 +4709,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":785
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4726,29 +4726,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4759,15 +4759,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":788
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4776,29 +4776,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4809,212 +4809,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":791
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":793
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":792
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":795
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":795
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":791
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":970
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":971
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":972
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":974
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":975
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":977
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":976
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":978
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":978
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":982
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5030,15 +5030,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5046,68 +5046,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":984
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 984, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":985
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":985
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 985, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 986, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 986, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5115,15 +5115,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":982
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5138,15 +5138,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":988
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5162,15 +5162,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5178,68 +5178,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":990
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 990, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":991
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":991
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 991, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 992, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 992, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5247,15 +5247,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":988
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5270,15 +5270,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":994
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5294,15 +5294,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5310,68 +5310,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":996
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 996, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":997
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":997
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 997, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":998
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":998
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 998, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 998, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5379,15 +5379,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":994
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5402,176 +5402,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1001
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1013
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1001
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1016
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1028
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1016
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1031
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1038
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1031
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1041
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1045
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1041
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1048
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1052
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1052
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1048
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -9282,26 +9282,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 986, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 992, __pyx_L1_error)
```

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_load_snbt.pyx` & `amulet-nbt-2.1.0/amulet_nbt/_load_snbt.pyx`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_named_tag.c` & `amulet-nbt-2.1.0/amulet_nbt/_named_tag.c`

 * *Files 1% similar despite different names*

```diff
@@ -1392,195 +1392,195 @@
   "amulet_nbt\\\\_string.pxd",
   "amulet_nbt\\\\_compound.pxd",
   "amulet_nbt\\\\_list.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* #### Code section: numeric_typedefs ### */
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":731
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":731
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":732
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":732
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":733
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":734
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":738
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":738
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":739
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":739
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":740
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":741
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":745
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":745
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":746
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":746
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":755
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":755
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":756
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":756
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":757
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":759
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":759
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":760
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":760
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":761
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":761
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":763
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":764
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":766
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":766
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":767
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":767
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":768
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":768
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1674,42 +1674,42 @@
  * cdef char read_byte(BufferContext buffer) except? -1
  */
 struct __pyx_opt_args_10amulet_nbt_5_util_to_little_endian {
   int __pyx_n;
   int little_endian;
 };
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":770
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":770
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":771
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":772
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":774
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":774
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -4900,261 +4900,261 @@
 #define __pyx_codeobj__40 __pyx_mstate_global->__pyx_codeobj__40
 #define __pyx_codeobj__41 __pyx_mstate_global->__pyx_codeobj__41
 #define __pyx_codeobj__43 __pyx_mstate_global->__pyx_codeobj__43
 #define __pyx_codeobj__45 __pyx_mstate_global->__pyx_codeobj__45
 #define __pyx_codeobj__47 __pyx_mstate_global->__pyx_codeobj__47
 /* #### Code section: module_code ### */
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":245
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":251
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":257
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":263
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":271
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":278
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":284
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":776
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5163,29 +5163,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5196,15 +5196,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":779
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5213,29 +5213,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5246,15 +5246,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":782
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5263,29 +5263,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5296,15 +5296,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":785
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5313,29 +5313,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5346,15 +5346,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":788
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5363,29 +5363,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5396,212 +5396,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":791
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":793
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":792
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":795
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":795
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":791
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":970
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":971
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":972
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":974
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":975
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":977
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":976
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":978
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":978
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":982
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5617,15 +5617,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5633,68 +5633,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":984
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 984, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":985
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":985
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 985, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 986, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 986, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5702,15 +5702,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":982
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5725,15 +5725,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":988
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5749,15 +5749,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5765,68 +5765,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":990
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 990, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":991
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":991
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 991, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 992, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 992, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5834,15 +5834,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":988
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5857,15 +5857,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":994
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5881,15 +5881,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5897,68 +5897,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":996
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 996, __pyx_L3_error)
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":997
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":997
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 997, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":998
+      /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":998
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 998, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 998, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5966,15 +5966,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":994
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5989,176 +5989,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1001
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1013
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1001
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1016
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1028
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1016
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1031
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1038
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1031
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1041
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1045
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1041
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1048
+/* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1052
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1052
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":1048
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -12022,26 +12022,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 986, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-2tr6m1by/lib/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "C:/Users/runneradmin/AppData/Local/Temp/build-env-uof8g4pm/lib/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 992, __pyx_L1_error)
```

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_named_tag.pyi` & `amulet-nbt-2.1.0/amulet_nbt/_named_tag.pyi`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_named_tag.pyx` & `amulet-nbt-2.1.0/amulet_nbt/_named_tag.pyx`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_numeric.c` & `amulet-nbt-2.1.0/amulet_nbt/_numeric.c`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_string.c` & `amulet-nbt-2.1.0/amulet_nbt/_string.c`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_string.pyi` & `amulet-nbt-2.1.0/amulet_nbt/_string.pyi`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_string.pyx` & `amulet-nbt-2.1.0/amulet_nbt/_string.pyx`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_util.c` & `amulet-nbt-2.1.0/amulet_nbt/_util.c`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_util.pxd` & `amulet-nbt-2.1.0/amulet_nbt/_util.pxd`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_util.pyx` & `amulet-nbt-2.1.0/amulet_nbt/_util.pyx`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_value.c` & `amulet-nbt-2.1.0/amulet_nbt/_value.c`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_value.pxd` & `amulet-nbt-2.1.0/amulet_nbt/_value.pxd`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_value.pyi` & `amulet-nbt-2.1.0/amulet_nbt/_value.pyi`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt/_value.pyx` & `amulet-nbt-2.1.0/amulet_nbt/_value.pyx`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/amulet_nbt.egg-info/PKG-INFO` & `amulet-nbt-2.1.0/amulet_nbt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amulet-nbt
-Version: 2.0.6
+Version: 2.1.0
 Summary: Read and write Minecraft NBT and SNBT data.
 Home-page: https://www.amuletmc.com
 Author: James Clare, Ben Gothard
 Author-email: amuleteditor@gmail.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `amulet-nbt-2.0.6/amulet_nbt.egg-info/SOURCES.txt` & `amulet-nbt-2.1.0/amulet_nbt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/setup.cfg` & `amulet-nbt-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/tests/test_legacy.py` & `amulet-nbt-2.1.0/tests/test_legacy.py`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/tests/test_massive_nbt.py` & `amulet-nbt-2.1.0/tests/test_massive_nbt.py`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/tests/test_nbt.py` & `amulet-nbt-2.1.0/tests/test_nbt.py`

 * *Files identical despite different names*

### Comparing `amulet-nbt-2.0.6/tests/test_tempita.py` & `amulet-nbt-2.1.0/tests/test_tempita.py`

 * *Files identical despite different names*

