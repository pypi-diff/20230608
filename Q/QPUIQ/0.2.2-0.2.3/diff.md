# Comparing `tmp/QPUIQ-0.2.2.tar.gz` & `tmp/QPUIQ-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QPUIQ-0.2.2.tar", last modified: Mon Jun  5 21:22:26 2023, max compression
+gzip compressed data, was "QPUIQ-0.2.3.tar", last modified: Thu Jun  8 11:30:04 2023, max compression
```

## Comparing `QPUIQ-0.2.2.tar` & `QPUIQ-0.2.3.tar`

### file list

```diff
@@ -1,77 +1,83 @@
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-05 21:22:26.325611 QPUIQ-0.2.2/
--rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/LICENSE.txt
--rw-r--r--   0 Bug        (504) staff       (20)     6129 2023-06-05 21:22:26.325450 QPUIQ-0.2.2/PKG-INFO
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-05 21:22:26.314389 QPUIQ-0.2.2/PUI/
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-05 21:22:26.318175 QPUIQ-0.2.2/PUI/PySide6/
--rw-r--r--   0 Bug        (504) staff       (20)     1245 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      498 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     5469 2023-06-05 21:20:44.000000 QPUIQ-0.2.2/PUI/PySide6/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      563 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     2696 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      752 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)     2331 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/combobox.py
--rw-r--r--   0 Bug        (504) staff       (20)      710 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      905 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      805 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/mdi.py
--rw-r--r--   0 Bug        (504) staff       (20)     2782 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/menu.py
--rw-r--r--   0 Bug        (504) staff       (20)      481 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      772 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)     3806 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)     1351 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/splitter.py
--rw-r--r--   0 Bug        (504) staff       (20)     1532 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/text.py
--rw-r--r--   0 Bug        (504) staff       (20)     1287 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     2239 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/PySide6/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      488 2023-06-05 21:22:25.000000 QPUIQ-0.2.2/PUI/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      432 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/decorator.py
--rw-r--r--   0 Bug        (504) staff       (20)     3607 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/dom.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-05 21:22:26.319873 QPUIQ-0.2.2/PUI/flet/
--rw-r--r--   0 Bug        (504) staff       (20)      658 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      610 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/application.py
--rw-r--r--   0 Bug        (504) staff       (20)      848 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      487 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      650 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1205 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      592 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)     1636 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)      775 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/text.py
--rw-r--r--   0 Bug        (504) staff       (20)      736 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      751 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/flet/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     5588 2023-06-05 21:20:44.000000 QPUIQ-0.2.2/PUI/node.py
--rw-r--r--   0 Bug        (504) staff       (20)    13532 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/state.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-05 21:22:26.322667 QPUIQ-0.2.2/PUI/textual/
--rw-r--r--   0 Bug        (504) staff       (20)      955 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)     1963 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     2952 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      437 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      519 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)     1300 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1501 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      502 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      622 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)     1612 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)      388 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/text.py
--rw-r--r--   0 Bug        (504) staff       (20)      742 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      381 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/textual/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     1005 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/timeline.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-05 21:22:26.324680 QPUIQ-0.2.2/PUI/tkinter/
--rw-r--r--   0 Bug        (504) staff       (20)      461 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      602 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/application.py
--rw-r--r--   0 Bug        (504) staff       (20)      564 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      450 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     1271 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      510 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     2161 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      456 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      553 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)      854 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1512 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/tkinter/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      505 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/utils.py
--rw-r--r--   0 Bug        (504) staff       (20)     2860 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/PUI/view.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-05 21:22:26.325242 QPUIQ-0.2.2/QPUIQ.egg-info/
--rw-r--r--   0 Bug        (504) staff       (20)     6129 2023-06-05 21:22:26.000000 QPUIQ-0.2.2/QPUIQ.egg-info/PKG-INFO
--rw-r--r--   0 Bug        (504) staff       (20)     1444 2023-06-05 21:22:26.000000 QPUIQ-0.2.2/QPUIQ.egg-info/SOURCES.txt
--rw-r--r--   0 Bug        (504) staff       (20)        1 2023-06-05 21:22:26.000000 QPUIQ-0.2.2/QPUIQ.egg-info/dependency_links.txt
--rw-r--r--   0 Bug        (504) staff       (20)        4 2023-06-05 21:22:26.000000 QPUIQ-0.2.2/QPUIQ.egg-info/top_level.txt
--rw-r--r--   0 Bug        (504) staff       (20)     5869 2023-06-05 21:20:44.000000 QPUIQ-0.2.2/README.md
--rw-r--r--   0 Bug        (504) staff       (20)       38 2023-06-05 21:22:26.325654 QPUIQ-0.2.2/setup.cfg
--rw-r--r--   0 Bug        (504) staff       (20)      539 2023-06-05 21:02:12.000000 QPUIQ-0.2.2/setup.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-08 11:30:04.387673 QPUIQ-0.2.3/
+-rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/LICENSE.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     6129 2023-06-08 11:30:04.387538 QPUIQ-0.2.3/PKG-INFO
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-08 11:30:04.376302 QPUIQ-0.2.3/PUI/
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-08 11:30:04.380125 QPUIQ-0.2.3/PUI/PySide6/
+-rw-r--r--   0 Bug        (504) staff       (20)     1245 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      498 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     5469 2023-06-05 21:20:44.000000 QPUIQ-0.2.3/PUI/PySide6/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      563 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2767 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/PySide6/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      752 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2331 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/combobox.py
+-rw-r--r--   0 Bug        (504) staff       (20)      710 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      905 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      805 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/mdi.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2782 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/menu.py
+-rw-r--r--   0 Bug        (504) staff       (20)      481 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      772 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3806 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1351 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/splitter.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1532 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1287 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2239 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      557 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      432 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/decorator.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3607 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/dom.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-08 11:30:04.382182 QPUIQ-0.2.3/PUI/flet/
+-rw-r--r--   0 Bug        (504) staff       (20)      703 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      588 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)      848 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/flet/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      549 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2067 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      634 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)      679 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1205 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/flet/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      621 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      825 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1665 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1460 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      839 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      751 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/flet/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     5588 2023-06-05 21:20:44.000000 QPUIQ-0.2.3/PUI/node.py
+-rw-r--r--   0 Bug        (504) staff       (20)    13532 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/state.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-08 11:30:04.384901 QPUIQ-0.2.3/PUI/textual/
+-rw-r--r--   0 Bug        (504) staff       (20)      955 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1952 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/textual/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2952 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      437 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      519 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1300 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1501 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      502 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      622 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1612 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)      388 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      742 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      381 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1005 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/timeline.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-08 11:30:04.386847 QPUIQ-0.2.3/PUI/tkinter/
+-rw-r--r--   0 Bug        (504) staff       (20)      692 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      729 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2416 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      469 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1129 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      746 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)      538 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2704 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      490 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      699 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3671 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)      391 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      860 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1550 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      505 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/utils.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2929 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/view.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-08 11:30:04.387348 QPUIQ-0.2.3/QPUIQ.egg-info/
+-rw-r--r--   0 Bug        (504) staff       (20)     6129 2023-06-08 11:30:04.000000 QPUIQ-0.2.3/QPUIQ.egg-info/PKG-INFO
+-rw-r--r--   0 Bug        (504) staff       (20)     1579 2023-06-08 11:30:04.000000 QPUIQ-0.2.3/QPUIQ.egg-info/SOURCES.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        1 2023-06-08 11:30:04.000000 QPUIQ-0.2.3/QPUIQ.egg-info/dependency_links.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        4 2023-06-08 11:30:04.000000 QPUIQ-0.2.3/QPUIQ.egg-info/top_level.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     5869 2023-06-05 21:20:44.000000 QPUIQ-0.2.3/README.md
+-rw-r--r--   0 Bug        (504) staff       (20)       38 2023-06-08 11:30:04.387714 QPUIQ-0.2.3/setup.cfg
+-rw-r--r--   0 Bug        (504) staff       (20)      539 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/setup.py
```

### Comparing `QPUIQ-0.2.2/LICENSE.txt` & `QPUIQ-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PKG-INFO` & `QPUIQ-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.2.2
+Version: 0.2.3
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `QPUIQ-0.2.2/PUI/PySide6/__init__.py` & `QPUIQ-0.2.3/PUI/PySide6/__init__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/PySide6/base.py` & `QPUIQ-0.2.3/PUI/PySide6/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/PySide6/button.py` & `QPUIQ-0.2.3/PUI/PySide6/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/PySide6/canvas.py` & `QPUIQ-0.2.3/PUI/PySide6/canvas.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,38 +17,39 @@
 
     def paintEvent(self, event):
         while self.node.retired_by:
             self.node = self.node.retired_by
         self.node.qpainter = QPainter()
         self.node.qpainter.begin(self)
 
-        if not self.node.bgColor is None:
+        if not self.node.style_bgcolor is None:
             bgBrush = QtGui.QBrush()
-            bgBrush.setColor(QtGui.QColor(self.node.bgColor))
+            bgBrush.setColor(QtGui.QColor(self.node.style_bgcolor))
             bgBrush.setStyle(QtCore.Qt.SolidPattern)
             rect = QtCore.QRect(0, 0, self.node.qpainter.device().width, self.node.qpainter.device().height)
             self.node.qpainter.fillRect(rect, bgBrush)
 
         self.node.painter(self.node, *self.node.args)
 
         self.node.qpainter.end()
         self.node.qpainter = None
 
 class QtCanvas(QtBaseWidget):
-    def __init__(self, painter, *args, bgColor=None):
+    def __init__(self, painter, *args):
         super().__init__()
         self.ui = None
         self.painter = painter
         self.args = args
-        self.bgColor = bgColor
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
             self.ui.puinode = self
+            self.ui.width = self.layout_width or 0
+            self.ui.height = self.layout_height or 0
         else:
             self.ui = PUIQtCanvas(self, self.layout_width or 0, self.layout_height or 0)
         self.ui.update()
         super().update(prev)
 
     def drawText(self, x, y, text):
         self.qpainter.drawText(QPoint(int(x), int(y)), text)
```

### Comparing `QPUIQ-0.2.2/PUI/PySide6/checkbox.py` & `QPUIQ-0.2.3/PUI/PySide6/checkbox.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/PySide6/combobox.py` & `QPUIQ-0.2.3/PUI/PySide6/combobox.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/PySide6/label.py` & `QPUIQ-0.2.3/PUI/PySide6/label.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/PySide6/layout.py` & `QPUIQ-0.2.3/PUI/PySide6/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/PySide6/mdi.py` & `QPUIQ-0.2.3/PUI/PySide6/mdi.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/PySide6/menu.py` & `QPUIQ-0.2.3/PUI/PySide6/menu.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/PySide6/radiobutton.py` & `QPUIQ-0.2.3/PUI/PySide6/radiobutton.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/PySide6/scroll.py` & `QPUIQ-0.2.3/PUI/PySide6/scroll.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/PySide6/splitter.py` & `QPUIQ-0.2.3/PUI/PySide6/splitter.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/PySide6/text.py` & `QPUIQ-0.2.3/PUI/PySide6/text.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/PySide6/textfield.py` & `QPUIQ-0.2.3/PUI/PySide6/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/PySide6/window.py` & `QPUIQ-0.2.3/PUI/PySide6/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/dom.py` & `QPUIQ-0.2.3/PUI/dom.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/flet/__init__.py` & `QPUIQ-0.2.3/PUI/tkinter/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from .application import *
 from .button import *
+from .canvas import *
+from .checkbox import *
 from .label import *
 from .layout import *
 from .progressbar import *
+from .radiobutton import *
 from .scroll import *
 from .text import *
 from .textfield import *
 from .window import *
-from .. import NotImplementedNode
 
-Application = FApplication
-Window = FWindow
-HBox = FRow
-VBox = FColumn
-Label = FLabel
-Button = FElevatedButton
-Checkbox = NotImplementedNode
-RadioButton = NotImplementedNode
-Canvas = NotImplementedNode
-TextField = FTextField
-ProgressBar = FProgressBar
-Scroll = FScroll
-Spacer = FSpacer
-Text = FText
-Html = FHtml
-MarkDown = FText
-Combobox = NotImplementedNode
-ComboboxItem = NotImplementedNode
+class DummyWidget(PUINode):
+    supported = False
 
-PUI_BACKEND = "flet"
+Application = TkApplication
+Window = TkWindow
+HBox = TkHBox
+VBox = TkVBox
+Label = TkLabel
+Button = TkButton
+Checkbox = TkCheckbutton
+RadioButton = TkRadiobutton
+Canvas = TkCanvas
+Text = TkLabel
+TextField = TkEntry
+ProgressBar = TkProgressBar
+Scroll = TkScroll
+Spacer = TkSpacer
+Text = TkText
+Html = DummyWidget
+MarkDown = DummyWidget
+
+PUI_BACKEND = "tkinter"
```

### Comparing `QPUIQ-0.2.2/PUI/flet/application.py` & `QPUIQ-0.2.3/PUI/flet/application.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from .base import *
 
 class FApplication(PUIView):
     def __init__(self):
         super().__init__()
         self.ready = False
 
-    def update(self, prev=None, redraw=False):
+    def update(self, prev=None):
         if not self.ready:
             return
-        super().update(redraw=False)
+        super().update(prev)
 
     def flet_app(self, page: ft.Page):
         self.ui = page
         self.ready = True
         self.update()
 
     def addChild(self, idx, child):
```

### Comparing `QPUIQ-0.2.2/PUI/flet/base.py` & `QPUIQ-0.2.3/PUI/flet/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/flet/label.py` & `QPUIQ-0.2.3/PUI/flet/label.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,9 @@
         else:
             self.ui.spans = [
                 ft.TextSpan(self.text)
             ]
         try:
             self.ui.update()
         except:
-            pass
+            pass
+        super().update(prev)
```

### Comparing `QPUIQ-0.2.2/PUI/flet/layout.py` & `QPUIQ-0.2.3/PUI/flet/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/flet/progressbar.py` & `QPUIQ-0.2.3/PUI/flet/button.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from .. import *
 from .base import *
 
-class FProgressBar(FBase):
-    def __init__(self, progress, maximum=100):
+class FElevatedButton(FBase):
+    def __init__(self, text):
         super().__init__()
-        self.progress = progress
-        self.maximum = maximum
+        self.text = text
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
-            self.ui.value = self.progress / self.maximum
+            self.ui.text = self.text
+            self.ui.on_click = self._clicked
+            try:
+                self.ui.update()
+            except:
+                pass
         else:
-            self.ui = ft.ProgressBar(width=300) # XXX
-            self.ui.value = self.progress / self.maximum
+            self.ui = ft.ElevatedButton(text=self.text, on_click=self._clicked)
         self.ui.expand = self.layout_weight
-        try:
-            self.ui.update()
-        except:
-            pass
```

### Comparing `QPUIQ-0.2.2/PUI/flet/scroll.py` & `QPUIQ-0.2.3/PUI/flet/scroll.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
             self.hframe.scroll = ft.ScrollMode.ADAPTIVE
         else:
             self.hframe.scroll = None
         try:
             self.vframe.update()
         except:
             pass
+        super().update(prev)
 
     def addChild(self, idx, child):
         if idx != 0:
             return
         self.hframe.controls.insert(idx, child.outer)
         try:
             self.hframe.update()
```

### Comparing `QPUIQ-0.2.2/PUI/flet/text.py` & `QPUIQ-0.2.3/PUI/flet/checkbox.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 from .. import *
 from .base import *
 
-class FText(FBase):
-    def __init__(self, text, **kwargs):
-        super().__init__(**kwargs)
+class FCheckbox(FBase):
+    def __init__(self, text, model):
+        super().__init__()
         self.text = text
+        self.model = model
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
-            self.ui.value = self.text
+            self.ui.value = self.model.value
+            self.ui.on_change = self._changed
             self.ui.update()
         else:
-            self.ui = ft.Text(self.text, expand=self.layout_weight)
+            self.ui = ft.Checkbox(label=self.text, value=self.model.value, on_change=self._changed)
 
-class FHtml(FBase):
-    supported = False
-    def __init__(self, text, **kwargs):
-        super().__init__(**kwargs)
-        self.text = text
+        super().update(prev)
 
-    def update(self, prev):
-        if prev and prev.ui:
-            self.ui = prev.ui
-            self.ui.value = self.text
-            self.ui.update()
-        else:
-            self.ui = ft.Text(self.text, expand=self.layout_weight)
+    def _changed(self, event):
+        node = self.get_node()
+        self.model.value = node.ui.value
```

### Comparing `QPUIQ-0.2.2/PUI/flet/textfield.py` & `QPUIQ-0.2.3/PUI/flet/textfield.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 
     def update(self, prev):
         value = self.model.value
         if prev and prev.ui:
             self.ui = prev.ui
             if prev.last_value != value:
                 self.ui.value = str(value)
-                self.ui.update()
+                try:
+                    self.ui.update()
+                except:
+                    pass
             self.last_value = value
         else:
             self.last_value = value
             self.ui = ft.TextField(label=self.label, value=value, on_change=self.on_textbox_changed, expand=self.layout_weight)
+        super().update(prev)
 
     def on_textbox_changed(self, e):
         self.model.value = e.control.value
```

### Comparing `QPUIQ-0.2.2/PUI/flet/window.py` & `QPUIQ-0.2.3/PUI/flet/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/node.py` & `QPUIQ-0.2.3/PUI/node.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/state.py` & `QPUIQ-0.2.3/PUI/state.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/textual/__init__.py` & `QPUIQ-0.2.3/PUI/textual/__init__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/textual/application.py` & `QPUIQ-0.2.3/PUI/textual/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         if self.updating:
             return
         self.updating = True
         self.ui.call_next(self._redraw)
 
     def _redraw(self):
         with self.ui.batch_update():
-            self.update(redraw=True)
+            self.update()
         self.updating = False
 
     def run(self):
         # self.redraw() # need to be after on_mount
         self.start()
 
     def start(self):
```

### Comparing `QPUIQ-0.2.2/PUI/textual/base.py` & `QPUIQ-0.2.3/PUI/textual/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/textual/checkbox.py` & `QPUIQ-0.2.3/PUI/textual/checkbox.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/textual/label.py` & `QPUIQ-0.2.3/PUI/textual/label.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/textual/layout.py` & `QPUIQ-0.2.3/PUI/textual/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/textual/radiobutton.py` & `QPUIQ-0.2.3/PUI/textual/radiobutton.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/textual/scroll.py` & `QPUIQ-0.2.3/PUI/textual/scroll.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/textual/textfield.py` & `QPUIQ-0.2.3/PUI/textual/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/timeline.py` & `QPUIQ-0.2.3/PUI/timeline.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/PUI/tkinter/application.py` & `QPUIQ-0.2.3/PUI/tkinter/application.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from .. import *
 from .base import *
 import functools
 
 class TkApplication(PUIView):
     def redraw(self):
         if self.ui:
-            self.ui.after(0, functools.partial(self.update, redraw=True))
+            self.ui.after(0, functools.partial(self.update))
         else:
-            self.update(redraw=True)
+            self.update()
 
     def update(self, prev=None):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = tk.Tk()
+            ttkStyle = ttk.Style(self.ui)
+            ttkStyle.theme_use('classic') # macOS's aqua doesn't respect background setting for some widgets
             self.ui.withdraw()
 
         super().update(prev)
 
     def addChild(self, idx, child):
         pass
```

### Comparing `QPUIQ-0.2.2/PUI/tkinter/canvas.py` & `QPUIQ-0.2.3/PUI/tkinter/canvas.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 from .. import *
 from .base import *
 import itertools
 class TkCanvas(TkBaseWidget):
     terminal = True
-    def __init__(self, painter, *args, size=None, bgColor=None):
+    def __init__(self, painter, *args):
         super().__init__()
         self.painter = painter
         self.args = args
-        self.size = size
-        self.bgColor = bgColor
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
-            self.ui = tk.Canvas(self.parent.ui, **self.kwargs)
+            self.ui = tk.Canvas(self.tkparent.inner)
         self.ui.delete("all")
 
-        if self.bgColor:
-            self.ui.config(bg=f"#{self.bgColor:06X}")
-
         self.painter(self, *self.args)
+        super().update(prev)
 
     def drawText(self, x, y, text):
         self.ui.create_text(x, y, text=text)
 
     def drawLine(self, x1, y1, x2, y2, color=None, width=None):
         params = {}
         if not color is None:
```

### Comparing `QPUIQ-0.2.2/PUI/tkinter/layout.py` & `QPUIQ-0.2.3/PUI/tkinter/layout.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,82 @@
 from .. import *
 from .base import *
 
 class TkHBox(TkBaseWidget):
+    use_ttk = "TFrame"
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
-            self.ui = tk.Frame(self.tkparent.inner)
+            self.ui = ttk.Frame(self.tkparent.inner)
             self.ui.grid_rowconfigure(0, weight=1)
+        super().update(prev)
 
-    def addChild(self, idx, child):
+    def putChild(self, idx, child):
         if isinstance(child, TkBaseWidget):
-            child.ui.grid(row=0, column=idx, sticky='nsew')
+            child.outer.grid(row=0, column=idx, sticky='nsew')
             if child.layout_weight is None:
                 self.ui.grid_columnconfigure(idx, weight=0)
             else:
-                self.ui.grid_columnconfigure(idx, weight=child.layout_weight)
+                self.ui.grid_columnconfigure(idx, weight=child.layout_weight, uniform=".")
         elif child.children:
-            self.addChild(idx, child.children[0])
+            self.putChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         self.ui.grid_columnconfigure(idx, weight=0)
         if isinstance(child, TkBaseWidget):
-            child.ui.grid_forget()
+            child_outer = child.outer
+            if child_outer:
+                child_outer.grid_forget()
         elif child.children:
             self.removeChild(idx, child.children[0])
 
+    def postSync(self):
+        for i,child in enumerate(self.children):
+            self.putChild(i, child)
+        super().postSync()
+
 class TkVBox(TkBaseWidget):
+    use_ttk = "TFrame"
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
-            self.ui = tk.Frame(self.tkparent.inner)
-            self.ui.config(bg="white")
+            self.ui = ttk.Frame(self.tkparent.inner)
             self.ui.grid_columnconfigure(0, weight=1)
+        super().update(prev)
 
-    def addChild(self, idx, child):
+    def putChild(self, idx, child):
         if isinstance(child, TkBaseWidget):
-            child.ui.grid(row=idx, column=0, sticky='nsew')
+            child.outer.grid(row=idx, column=0, sticky='nsew')
             if child.layout_weight is None:
                 self.ui.grid_rowconfigure(idx, weight=0)
             else:
-                self.ui.grid_rowconfigure(idx, weight=child.layout_weight)
+                self.ui.grid_rowconfigure(idx, weight=child.layout_weight, uniform=".")
         elif child.children:
-            self.addChild(idx, child.children[0])
+            self.putChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         self.ui.grid_rowconfigure(idx, weight=0)
         if isinstance(child, TkBaseWidget):
-            child.ui.grid_forget()
+            child_outer = child.outer
+            if child_outer:
+                child_outer.grid_forget()
         elif child.children:
             self.removeChild(idx, child.children[0])
 
+    def postSync(self):
+        for i,child in enumerate(self.children):
+            self.putChild(i, child)
+        super().postSync()
+
 class TkSpacer(TkBaseWidget):
+    use_ttk = "TFrame"
     def __init__(self, *args):
         super().__init__(*args)
         self.layout_weight = 1
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
-            self.ui = tk.Frame(self.tkparent.inner)
+            self.ui = ttk.Frame(self.tkparent.inner)
```

### Comparing `QPUIQ-0.2.2/PUI/tkinter/window.py` & `QPUIQ-0.2.3/PUI/tkinter/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
             self.curr_size = prev.curr_size
             self.curr_maximize = prev.curr_maximize
             self.curr_fullscreen = prev.curr_fullscreen
         else:
-            self.ui = tk.Toplevel(self.parent.ui)
+            self.ui = tk.Toplevel(self.parent.inner)
 
         if self.curr_size != self.size:
             self.curr_size = self.size
             self.ui.geometry("x".join([str(v) for v in self.size]))
         if self.curr_maximize !=  self.maximize:
             self.curr_maximize =  self.maximize
 
@@ -36,11 +36,13 @@
         if self.curr_fullscreen != self.fullscreen:
             self.curr_fullscreen = self.fullscreen
             self.ui.attributes('-fullscreen', True)
         if not self.title is None:
             self.ui.title(self.title)
 
     def addChild(self, idx, child):
+        if idx:
+            return
         child.ui.pack(fill=tk.BOTH, expand=True)
 
     def removeChild(self, idx, child):
         child.ui.pack_forget()
```

### Comparing `QPUIQ-0.2.2/PUI/view.py` & `QPUIQ-0.2.3/PUI/view.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,23 +48,27 @@
         return scope
 
     def destroy(self, direct):
         PUIView.__ALLVIEWS__.remove(self)
         return super().destroy(direct)
 
     def redraw(self):
-        self.update(redraw=True)
+        self.update()
 
-    def update(self, prev=None, redraw=False):
+    def update(self, prev=None):
         if self.retired_by:
             return
         if self.destroyed:
             return
-        if not prev and not redraw:
-            self.setup()
+        if not prev:
+            if self.setup:
+                self.setup()
+                self.setup = None
+        else:
+            self.setup = None
         update_start = time.time()
         dprint("update()", self.key)
         if prev:
             self.children = prev.children
             prev.retired_by = self
             PUIView.__ALLVIEWS__.remove(prev)
```

### Comparing `QPUIQ-0.2.2/QPUIQ.egg-info/PKG-INFO` & `QPUIQ-0.2.3/QPUIQ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.2.2
+Version: 0.2.3
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `QPUIQ-0.2.2/QPUIQ.egg-info/SOURCES.txt` & `QPUIQ-0.2.3/QPUIQ.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,20 @@
 PUI/PySide6/text.py
 PUI/PySide6/textfield.py
 PUI/PySide6/window.py
 PUI/flet/__init__.py
 PUI/flet/application.py
 PUI/flet/base.py
 PUI/flet/button.py
+PUI/flet/canvas.py
+PUI/flet/checkbox.py
 PUI/flet/label.py
 PUI/flet/layout.py
 PUI/flet/progressbar.py
+PUI/flet/radiobutton.py
 PUI/flet/scroll.py
 PUI/flet/text.py
 PUI/flet/textfield.py
 PUI/flet/window.py
 PUI/textual/__init__.py
 PUI/textual/application.py
 PUI/textual/base.py
@@ -52,17 +55,20 @@
 PUI/textual/textfield.py
 PUI/textual/window.py
 PUI/tkinter/__init__.py
 PUI/tkinter/application.py
 PUI/tkinter/base.py
 PUI/tkinter/button.py
 PUI/tkinter/canvas.py
+PUI/tkinter/checkbox.py
 PUI/tkinter/label.py
 PUI/tkinter/layout.py
 PUI/tkinter/progressbar.py
+PUI/tkinter/radiobutton.py
 PUI/tkinter/scroll.py
+PUI/tkinter/text.py
 PUI/tkinter/textfield.py
 PUI/tkinter/window.py
 QPUIQ.egg-info/PKG-INFO
 QPUIQ.egg-info/SOURCES.txt
 QPUIQ.egg-info/dependency_links.txt
 QPUIQ.egg-info/top_level.txt
```

### Comparing `QPUIQ-0.2.2/README.md` & `QPUIQ-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.2/setup.py` & `QPUIQ-0.2.3/setup.py`

 * *Files identical despite different names*

