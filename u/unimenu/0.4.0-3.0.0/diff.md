# Comparing `tmp/unimenu-0.4.0.tar.gz` & `tmp/unimenu-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unimenu-0.4.0.tar", last modified: Wed Jun  7 22:07:38 2023, max compression
+gzip compressed data, was "unimenu-3.0.0.tar", last modified: Thu Mar  2 15:01:18 2023, max compression
```

## Comparing `unimenu-0.4.0.tar` & `unimenu-3.0.0.tar`

### file list

```diff
@@ -1,53 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:07:38.304005 unimenu-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:07:38.296005 unimenu-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:07:38.296005 unimenu-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-07 22:07:28.000000 unimenu-0.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-07 22:07:28.000000 unimenu-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-07 22:07:28.000000 unimenu-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-07 22:07:38.304005 unimenu-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-07 22:07:28.000000 unimenu-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:07:38.300005 unimenu-0.4.0/manual_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-07 22:07:28.000000 unimenu-0.4.0/manual_tests/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-07 22:07:28.000000 unimenu-0.4.0/manual_tests/substance_painter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-07 22:07:28.000000 unimenu-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:07:38.300005 unimenu-0.4.0/samples/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-07 22:07:28.000000 unimenu-0.4.0/samples/any_dcc_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-07 22:07:28.000000 unimenu-0.4.0/samples/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-07 22:07:28.000000 unimenu-0.4.0/samples/maya_startup_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-07 22:07:28.000000 unimenu-0.4.0/samples/menu_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-07 22:07:28.000000 unimenu-0.4.0/samples/menu_config_blender.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-07 22:07:28.000000 unimenu-0.4.0/samples/menu_config_unreal.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-07 22:07:28.000000 unimenu-0.4.0/samples/menu_config_unreal_append.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-06-07 22:07:28.000000 unimenu-0.4.0/samples/menu_screen_katana.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    45728 2023-06-07 22:07:28.000000 unimenu-0.4.0/samples/menu_screen_krita.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    25598 2023-06-07 22:07:28.000000 unimenu-0.4.0/samples/menu_screen_mari.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-06-07 22:07:28.000000 unimenu-0.4.0/samples/menu_screen_maya.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-06-07 22:07:28.000000 unimenu-0.4.0/samples/menu_screen_nuke.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    27646 2023-06-07 22:07:28.000000 unimenu-0.4.0/samples/menu_screen_substance_painter.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    45940 2023-06-07 22:07:28.000000 unimenu-0.4.0/samples/menu_screen_unreal5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-07 22:07:28.000000 unimenu-0.4.0/samples/nuke_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-07 22:07:28.000000 unimenu-0.4.0/samples/qt_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 22:07:38.304005 unimenu-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:07:38.300005 unimenu-0.4.0/unimenu/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-07 22:07:28.000000 unimenu-0.4.0/unimenu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:07:38.304005 unimenu-0.4.0/unimenu/apps/
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-07 22:07:28.000000 unimenu-0.4.0/unimenu/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-07 22:07:28.000000 unimenu-0.4.0/unimenu/apps/_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-06-07 22:07:28.000000 unimenu-0.4.0/unimenu/apps/blender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-07 22:07:28.000000 unimenu-0.4.0/unimenu/apps/hiero.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-07 22:07:28.000000 unimenu-0.4.0/unimenu/apps/katana.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-07 22:07:28.000000 unimenu-0.4.0/unimenu/apps/mari.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-07 22:07:28.000000 unimenu-0.4.0/unimenu/apps/marmoset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-07 22:07:28.000000 unimenu-0.4.0/unimenu/apps/max.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-07 22:07:28.000000 unimenu-0.4.0/unimenu/apps/maya.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-07 22:07:28.000000 unimenu-0.4.0/unimenu/apps/nuke.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-07 22:07:28.000000 unimenu-0.4.0/unimenu/apps/qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-07 22:07:28.000000 unimenu-0.4.0/unimenu/apps/unreal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-06-07 22:07:28.000000 unimenu-0.4.0/unimenu/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-07 22:07:28.000000 unimenu-0.4.0/unimenu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:07:38.300005 unimenu-0.4.0/unimenu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-07 22:07:38.000000 unimenu-0.4.0/unimenu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-07 22:07:38.000000 unimenu-0.4.0/unimenu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:07:38.000000 unimenu-0.4.0/unimenu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-07 22:07:38.000000 unimenu-0.4.0/unimenu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 22:07:38.000000 unimenu-0.4.0/unimenu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:01:18.118274 unimenu-3.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:01:18.114274 unimenu-3.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:01:18.114274 unimenu-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-02 15:01:06.000000 unimenu-3.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-03-02 15:01:06.000000 unimenu-3.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-02 15:01:06.000000 unimenu-3.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-03-02 15:01:18.118274 unimenu-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-03-02 15:01:06.000000 unimenu-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:01:18.114274 unimenu-3.0.0/manual_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-02 15:01:06.000000 unimenu-3.0.0/manual_tests/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-02 15:01:06.000000 unimenu-3.0.0/manual_tests/substance_painter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-02 15:01:06.000000 unimenu-3.0.0/openmenu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-02 15:01:06.000000 unimenu-3.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:01:18.118274 unimenu-3.0.0/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/any_dcc_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/maya_startup_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/menu_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/menu_config_blender.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/menu_config_unreal.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/menu_config_unreal_append.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    45728 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/menu_screen_krita.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/menu_screen_maya.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    38386 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/menu_screen_substance_painter.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    45940 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/menu_screen_unreal5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/qt_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 15:01:18.118274 unimenu-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:01:18.118274 unimenu-3.0.0/unimenu/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:01:18.118274 unimenu-3.0.0/unimenu/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/apps/_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/apps/blender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/apps/marmoset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/apps/max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/apps/maya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/apps/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/apps/unreal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:01:18.118274 unimenu-3.0.0/unimenu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-03-02 15:01:18.000000 unimenu-3.0.0/unimenu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-02 15:01:18.000000 unimenu-3.0.0/unimenu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 15:01:18.000000 unimenu-3.0.0/unimenu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-02 15:01:18.000000 unimenu-3.0.0/unimenu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-02 15:01:18.000000 unimenu-3.0.0/unimenu.egg-info/top_level.txt
```

### Comparing `unimenu-0.4.0/.github/workflows/python-publish.yml` & `unimenu-3.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.0/.gitignore` & `unimenu-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.0/.pre-commit-config.yaml` & `unimenu-3.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.0/PKG-INFO` & `unimenu-3.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unimenu
-Version: 0.4.0
+Version: 3.0.0
 Summary: easy menus from a single config across apps
 Author: hannes
 Project-URL: Homepage, https://github.com/hannesdelbeke/unimenu
 Project-URL: Documentation, https://github.com/hannesdelbeke/unimenu/wiki
 Keywords: dcc,pipeline,menu,config
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
@@ -21,55 +21,57 @@
 A pure python module to add python commands to the menu.
 
 Supports Unreal Engine, Blender, Marmoset<br>
 and any app that uses QT: Maya, Krita, Substance Painter, 3ds Max, FreeCAD, CryEngine ...
 
 For more info read the [wiki](https://github.com/hannesdelbeke/unimenu/wiki)
 
-If you use Blender, you can try the [unimenu_addon](https://github.com/hannesdelbeke/unimenu_addon)
-
 <img src="samples/menu_screen_maya.jpg" width="400"/> <img src="samples/menu_screen_unreal5.jpg" width="400"/> <img src="samples/menu_screen_krita.jpg" width="400"/> <img src="samples/menu_screen_substance_painter.jpg" width="400"/>
-<img src="samples/menu_screen_nuke.jpg" width="400"/> <img src="samples/menu_screen_katana.jpg" width="400"/>
-<img src="samples/menu_screen_mari.jpg" width="400"/>
+
 # how to use
 
+you can make your menu(s):
+- from a config
+- from a dict
+- with explicit code
+- from a folder of scripts
+
 ### load from config (YAML & JSON)
 ```yaml
 items:
   - label: my menu
     items:
       - label: my item
         command: print("Hello World")
 ```
 ```python
 import unimenu
 config_path = "path/to/config.yaml"
 unimenu.setup(config_path)
 ```
 
-
-
-### load from a dict
+### load from dynamic dict
 
 ```python
 import unimenu
 data = {"items": [{"label": test,"command": 'print("hello world")'}]}
 unimenu.setup(data)
 ```
 
 
-
 ### with code
 
 ```python
-import unimenu
-menu = unimenu.Node(label="my menu")  # create a menu
-item = unimenu.Node(label="hi", command='print("hi")')  # create a menu item
-menu.items.append(item)  # add the item to the menu
-menu.setup()  # setup the menu in the app, parented by default to the main menu bar
+import unimenu.apps.blender
+
+menu = unimenu.dccs.blender.MenuNodeBlender(label="my submenu")  # create a submenu, parent defaults to the menu bar
+item = unimenu.dccs.blender.MenuNodeBlender(label="hello", command='print("hello world")',
+                                            parent="UNIMENU_MT_my_submenu")  # add menu item to our submenu
+menu.items.append(item)  # add the item to the submenu
+menu.setup()  # setup the menu
 ```
 
 ### from a folder of scripts (module) (experimental, needs updating)
 
 great for a folder full of tools that need launching when clicking a button.
 1. ensure the folder is importable (in the sys.path)
 2. create a menthod in all submodules with the same name, e.g. def show()
@@ -94,18 +96,14 @@
 unimenu was tested in the following versions, and might work in other versions.
 - Unreal 5.0.2
 - Blender 3.2, 2.93, 2.8 (minimum)
 - Maya 2023, 2022 (minimum)
 - Substance Painter 8.2.0
 - Max 2024
 - Marmoset 3.08
-- Nuke 13 (minimum)
-- Hiero 13 (minimum)
-- Katana 5 (minimum)
-- Mari 6.0 (minimum)
 
 python 3.7+ due to f-strings and pathlib
 
 ## Development
 
 main platform is windows, would be interested to hear from mac & linux users.
```

### Comparing `unimenu-0.4.0/README.md` & `unimenu-3.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,55 +8,57 @@
 A pure python module to add python commands to the menu.
 
 Supports Unreal Engine, Blender, Marmoset<br>
 and any app that uses QT: Maya, Krita, Substance Painter, 3ds Max, FreeCAD, CryEngine ...
 
 For more info read the [wiki](https://github.com/hannesdelbeke/unimenu/wiki)
 
-If you use Blender, you can try the [unimenu_addon](https://github.com/hannesdelbeke/unimenu_addon)
-
 <img src="samples/menu_screen_maya.jpg" width="400"/> <img src="samples/menu_screen_unreal5.jpg" width="400"/> <img src="samples/menu_screen_krita.jpg" width="400"/> <img src="samples/menu_screen_substance_painter.jpg" width="400"/>
-<img src="samples/menu_screen_nuke.jpg" width="400"/> <img src="samples/menu_screen_katana.jpg" width="400"/>
-<img src="samples/menu_screen_mari.jpg" width="400"/>
+
 # how to use
 
+you can make your menu(s):
+- from a config
+- from a dict
+- with explicit code
+- from a folder of scripts
+
 ### load from config (YAML & JSON)
 ```yaml
 items:
   - label: my menu
     items:
       - label: my item
         command: print("Hello World")
 ```
 ```python
 import unimenu
 config_path = "path/to/config.yaml"
 unimenu.setup(config_path)
 ```
 
-
-
-### load from a dict
+### load from dynamic dict
 
 ```python
 import unimenu
 data = {"items": [{"label": test,"command": 'print("hello world")'}]}
 unimenu.setup(data)
 ```
 
 
-
 ### with code
 
 ```python
-import unimenu
-menu = unimenu.Node(label="my menu")  # create a menu
-item = unimenu.Node(label="hi", command='print("hi")')  # create a menu item
-menu.items.append(item)  # add the item to the menu
-menu.setup()  # setup the menu in the app, parented by default to the main menu bar
+import unimenu.apps.blender
+
+menu = unimenu.dccs.blender.MenuNodeBlender(label="my submenu")  # create a submenu, parent defaults to the menu bar
+item = unimenu.dccs.blender.MenuNodeBlender(label="hello", command='print("hello world")',
+                                            parent="UNIMENU_MT_my_submenu")  # add menu item to our submenu
+menu.items.append(item)  # add the item to the submenu
+menu.setup()  # setup the menu
 ```
 
 ### from a folder of scripts (module) (experimental, needs updating)
 
 great for a folder full of tools that need launching when clicking a button.
 1. ensure the folder is importable (in the sys.path)
 2. create a menthod in all submodules with the same name, e.g. def show()
@@ -81,18 +83,14 @@
 unimenu was tested in the following versions, and might work in other versions.
 - Unreal 5.0.2
 - Blender 3.2, 2.93, 2.8 (minimum)
 - Maya 2023, 2022 (minimum)
 - Substance Painter 8.2.0
 - Max 2024
 - Marmoset 3.08
-- Nuke 13 (minimum)
-- Hiero 13 (minimum)
-- Katana 5 (minimum)
-- Mari 6.0 (minimum)
 
 python 3.7+ due to f-strings and pathlib
 
 ## Development
 
 main platform is windows, would be interested to hear from mac & linux users.
```

### Comparing `unimenu-0.4.0/manual_tests/generic.py` & `unimenu-3.0.0/manual_tests/generic.py`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.0/pyproject.toml` & `unimenu-3.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 classifiers = [
     "Programming Language :: Python :: 3.7",
 ]
 dependencies = [
     'importlib-metadata; python_version<"3.7"',
 ]
 #dynamic = ["version"]
-version = "0.4.0"
+version = "3.0.0"
 
 [project.optional-dependencies]
 yaml = ["pyyaml"]
 
 #[project.scripts]
 #my-script = "my_package.module:function"
```

### Comparing `unimenu-0.4.0/samples/any_dcc_test.py` & `unimenu-3.0.0/samples/any_dcc_test.py`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.0/samples/config.json` & `unimenu-3.0.0/samples/config.json`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.0/samples/maya_startup_plugin.py` & `unimenu-3.0.0/samples/maya_startup_plugin.py`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.0/samples/menu_screen_krita.jpg` & `unimenu-3.0.0/samples/menu_screen_krita.jpg`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.0/samples/menu_screen_unreal5.jpg` & `unimenu-3.0.0/samples/menu_screen_unreal5.jpg`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.0/samples/qt_sample.py` & `unimenu-3.0.0/samples/qt_sample.py`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.0/unimenu/apps/__init__.py` & `unimenu-3.0.0/unimenu/apps/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,18 +45,14 @@
     MAYA = App(name="maya", module="maya")  # pymel can be slow to import
     UNREAL = App(name="unreal", module="unreal")
     MAX = App(name="max", module="pymxs")
     KRITA = App(name="krita", module="krita")
     SUBSTANCE_DESIGNER = App(name="substance_designer", module="pysbs")
     SUBSTANCE_PAINTER = App(name="substance_painter", module="substance_painter")
     MARMOSET = App(name="marmoset", module="mset")
-    NUKE = App(name="nuke", module="nuke")
-    HIERO = App(name="hiero", module="hiero")
-    KATANA = App(name="katana", module="katana")
-    MARI = App(name="mari", module="mari")
 
     QT = App("qt", None)
 
     # ALL = [BLENDER, MAYA, UNREAL, KRITA, SUBSTANCE_PAINTER, MAX, MARMOSET]
     NON_QT = [BLENDER, UNREAL, SUBSTANCE_PAINTER, MARMOSET]
```

### Comparing `unimenu-0.4.0/unimenu/apps/_abstract.py` & `unimenu-3.0.0/unimenu/apps/_abstract.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from abc import abstractmethod, ABC
 import unimenu.utils
 from pathlib import Path
-import logging
-import re
-import traceback
 
 
 class MenuNode(object):
     """
     data class for menu items, this can be loaded in python in any app
     """
     unigue_names = set()
@@ -37,19 +34,15 @@
         self.separator = separator or False
         items = items or []
         self.items: list[MenuNodeAbstract] = [self.__class__(**item) for item in items]
         self.kwargs = kwargs or {}
         self.data = data or {}
         self.id = id or None
 
-        # only the root node needs parent_path
-        if parent_path:
-            self.parent_path = parent_path.replace(" ", "_")
-        else:
-            self.parent_path = None
+        self.parent_path = parent_path  # only the root node needs this
         # todo get parent path method
 
         # helpers
         self.parent: MenuNode = parent  # some implicit code use, pay attention to parent
         self.config_path = None  # the path to the config file that created this node todo do non root nodes populate this?
         
         # todo move to abstract
@@ -64,26 +57,28 @@
         if self.id:
             return
 
         label = self.label
         if not label:
             label = "TODO"  # todo unique number
 
-
-        label = re.sub('[^0-9a-zA-Z]+', '_', label)  # replace non alphanumeric with _
-
         parent_names = []
         parent = self.parent
         while parent:
-            parent_names.append(parent.id)  # todo, since id includes parent, adding parent id adds root parent multiple times
+            parent_names.append(parent.id)
             parent = parent.parent
         parent_names.reverse()
-        parent_names.append(label)
+        parent_names.append(self.label)
         self.id = "_".join(parent_names)
 
+
+    @property
+    def try_command(self):
+        return f"import unimenu.utils; unimenu.utils.try_command(r'{self.command}')"
+
     @property
     def children(self):
         return self.items
 
     @children.setter
     def children(self, value):
         self.items = value
@@ -131,33 +126,28 @@
         if self.items:
             child_configs = []
             for item in self.items:
                 child_config = item.__dict__()
                 child_config.pop("parent", None)  # we only need to save the parent for the top node
                 child_configs.append(child_config)
             config["items"] = child_configs
-        if self.parent_path and isinstance(self.parent_path, str):
+        if self.parent and isinstance(self.parent, str):
             config["parent_path"] = self.parent_path
         if self.kwargs:
             config["kwargs"] = self.kwargs
         if self.data:
             config["data"] = self.data
         return config
 
-    def run(self, *args):  # some apps pass args to the command. e.g. maya passes False
+    def run(self):
         """execute the command in self.command, which accepts a function or string"""
-        try:
-            if isinstance(self.command, str):
-                # lambda: exec(self.command)
-                exec(self.command)
-            else:  # callable
-                self.command()
-        except Exception as e:
-            traceback.print_exc()
-            return e
+        if isinstance(self.command, str):
+            lambda: exec(self.command)
+        else:  # callable
+            self.command()
 
     @classmethod
     def load(cls, arg):
         # if arg is a Path or string, load from config
         if isinstance(arg, (str, Path)):
             return cls.load_config(arg)
         # if arg is a dict, create a menu node from it
@@ -210,23 +200,22 @@
         elif self.command:  # menu item
             self.app_node = self._setup_menu_item(parent_app_node=parent_app_node)
 
         elif self.items:  # submenu
             self.app_node = self._setup_sub_menu(parent_app_node=parent_app_node)
             for item in self.items:
                 item.setup(parent_app_node=self.app_node)
-        else:
-            logging.warning("Can not create a MenuNode that has no command or children: " + self.label)
 
         # some apps, e.g. unreal, don't allow adding attributes dynamically
         if backlink:
             try:
                 self.app_node.menu_node = self  # todo setproperty qt
             except AttributeError:
-                logging.warning(f"Warning: could not set backlink on {self.app_node} to {self}")
+                print(f"Warning: could not set backlink on {self.app_node} to {self}")
+                pass
 
         return self.app_node
 
     # todo consider moving to abstract, and func isntead of property
     # todo test with parent name in config for all apps
     # todo test with submenu name in config for all apps
     @property
```

### Comparing `unimenu-0.4.0/unimenu/apps/blender.py` & `unimenu-3.0.0/unimenu/apps/blender.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,115 +5,109 @@
 # 4. add operators to menu
 """
 import bpy
 from typing import Union, Callable
 from unimenu.apps._abstract import MenuNodeAbstract
 import unimenu.apps
 
-def unique_operator_name(name) -> str:
-    """ensure unique name for blender operators, adds _number to the end if name not unique"""
-    unique_counter = 1  # start count from 2
-    new_name = name
-    while new_name in dir(bpy.types):
-        unique_counter += 1
-        new_name = f"{name}_{unique_counter}"
-    return new_name
 
+counter = -1
 
 def operator_wrapper(
-    parent: bpy.types.Operator, label: str, id: str, command: Union[str, Callable], icon_name=None, tooltip=None
+    parent: bpy.types.Operator, label: str, command: Union[str, Callable], icon_name=None, tooltip=None
 ) -> bpy.types.Operator:
     """
     Wrap a command in a Blender operator & add it to a parent menu operator.
 
     1 make class
     2 register class
     3 add to (sub)menu (parent operator)
     """
 
+    global counter
+    counter += 1
+
     icon_name = icon_name or "NONE"
     tooltip = tooltip or ""
 
     # handle name
     # class: UNIMENU_OT_my_operator
     # id: unimenu.my_operator
     #  todo add support dupe names
-    name = "UNIMENU_OT_" + id
-    name = unique_operator_name(name)
+    name = "UNIMENU_OT_" + label.replace(" ", "_") + str(counter)
     id_name = name.replace("UNIMENU_OT_", "unimenu.").lower()
 
     # create
     class OperatorWrapper(bpy.types.Operator):
         # blender vars
         bl_label = label
         bl_idname = id_name
 
         # custom vars
         _command = command  # custom var to store string command
         _parent_name = parent.bl_idname
 
         def execute(self, context):
-            self._command()
-            return {"FINISHED"}
+            # data loaded from the config passes strings to eval,
+            # but dynamically created configs support callables
+
+            if isinstance(self._command, str):
+                exec(self._command)
+
+            elif callable(self._command):
+                self._command()
+
+            return {"RUNNING_MODAL"}
 
-    # print("UNI made operator", name, OperatorWrapper.bl_idname)
     OperatorWrapper.__name__ = name
     if tooltip:
         OperatorWrapper.__doc__ = tooltip
 
     # register
     bpy.utils.register_class(OperatorWrapper)
 
     # ensure None was not accidentally passed
     icon_name = icon_name or "NONE"
 
     # add to menu
     def menu_draw(self, context):  # self is the parent menu
-        # todo check if icon exists, if not use NONE, for now dirty try except hack
-        try:
-            self.layout.operator(id_name, icon=icon_name)
-        except TypeError:  # icon not found:
-            self.layout.operator(id_name, icon="NONE")
+        self.layout.operator(id_name, icon=icon_name)
 
     parent.append(menu_draw)
 
     return OperatorWrapper
 
 
 def menu_wrapper(parent: bpy.types.Operator, label: str) -> bpy.types.Menu:
     """
     1 make class
     2 register class
     3 add to (sub)menu (parent operator)
     """
 
-    # global counter
-    # counter += 1
+    global counter
+    counter += 1
     # todo add support dupe names
     # handle name
     # class: UNIMENU_OT_my_operator
     # id: unimenu.my_operator
     # todo we dont need to set both class and bl_idname
 
-    name = "UNIMENU_MT_" + label.replace(" ", "_")
-
-    name = unique_operator_name(name)
-
+    name = "UNIMENU_MT_" + label.replace(" ", "_") + str(counter)
     id_name = name
 
     class MenuWrapper(bpy.types.Menu):
         bl_label = label
         bl_idname = id_name
 
         def draw(self, context):
             layout = self.layout  # layout is needed, even when unused
 
     # rename class
     MenuWrapper.__name__ = name
-    # print("UNI made menu operator", name, MenuWrapper.bl_idname)
 
     # register
     bpy.utils.register_class(MenuWrapper)
 
     # add to menu
     def menu_draw(self, context):  # self is the parent menu
         self.layout.menu(id_name)
@@ -127,33 +121,30 @@
 
 
 class MenuNodeBlender(MenuNodeAbstract):
     app = unimenu.apps.SupportedApps.BLENDER  # helper to get matching App
 
     @property
     def _default_root_parent(self):
-        if self.parent_path:
-            parent_path = f"UNIMENU_MT_{self.parent_path.replace(' ', '_')}"
-        else:
-            parent_path = "TOPBAR_MT_editor_menus"
+        parent_path = self.parent_path or "TOPBAR_MT_editor_menus"
         parent_node = getattr(bpy.types, parent_path)  # get the parent from blender by name
         return parent_node
 
         # # create app menu-nodes
         # operators = cls._setup_menu_items(parent, items=menu_node.items)
         # cls.registered_operators.update(operators)
         # return operators
 
     def _setup_sub_menu(self, parent_app_node=None) -> bpy.types.Menu:
         return menu_wrapper(parent=parent_app_node, label=self.label)
 
     def _setup_menu_item(self, parent_app_node=None) -> bpy.types.Operator:
         icon = self.icon or "NONE"
         tooltip = self.tooltip or ""
-        return operator_wrapper(parent=parent_app_node, label=self.label, id=self.id, command=self.run, icon_name=icon, tooltip=tooltip)
+        return operator_wrapper(parent_app_node, self.label, self.command, icon_name=icon, tooltip=tooltip)
 
     def _setup_separator(self, parent_app_node=None):
         # todo return separator correctly
         parent_app_node.append(lambda self, context: self.layout.separator())
 
     def teardown(self):
         """
```

### Comparing `unimenu-0.4.0/unimenu/apps/marmoset.py` & `unimenu-3.0.0/unimenu/apps/marmoset.py`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.0/unimenu/apps/max.py` & `unimenu-3.0.0/unimenu/apps/max.py`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.0/unimenu/apps/maya.py` & `unimenu-3.0.0/unimenu/apps/maya.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,115 +1,113 @@
 """
 native maya menu support. not needed anymore, use the qt menu instead
-short menu names are the name of the menu node.
-long menu names are the name of the menu, and all its parents, separated by "|"
 """
+
+import pymel.core as pm  # todo replace with cmds because it's faster
 from unimenu.apps._abstract import MenuNodeAbstract
 import maya.mel
-import maya.cmds  # cmds is faster than pymel
-import re
+import maya.cmds
 
 
-def find_menu(long_name):
-    long_name = f"MayaWindow|{long_name}"  # for now we assume the menu is a child of the main window
-    long_menu_names = maya.cmds.lsUI(menus=True, long=True)
-    for long_menu_name in long_menu_names:
-        if long_menu_name == long_name:
-            return long_menu_name
+counter = 0
 
 
-def get_compatible_name(name):
-    name = re.sub('[^0-9a-zA-Z]+', '_', name)  # replace non alpha-numeric with _
-    name = name.strip("_")  # remove leading and trailing underscores
-    return name
+def get_counter():
+    global counter
+    counter += 1
+    return counter
 
 
-def get_unique_name(name, parent):
-    """
-    Guarantee a unique name compatible with maya naming conventions
-    name: str, the short name of the menu
-    parent: str, the long name of the parent menu
-    """
-    name = get_compatible_name(name)
-    long_name = f"{parent}|{name}"
-    long_menu_names = maya.cmds.lsUI(menus=True, long=True)
-    long_menu_item_names = maya.cmds.lsUI(menuItems=True, long=True)
-    if any(long_name == long_menu_name for long_menu_name in long_menu_names + long_menu_item_names):
-        # if the name is already taken, add a number to the end
-        # this could be improved by finding the next available number
-        name = f"{name}_1"
-        name = get_unique_name(name, parent)
-    return name
+def find_menu(name):
+    gMainWindow = maya.mel.eval('$temp=$gMainWindow')
+    # get all the menus that are children of the main menu
+    mainWindowMenus = maya.cmds.window(gMainWindow, query=True, menuArray=True)
+    for menu in mainWindowMenus:
+        if menu.lower() == name.lower():
+            return menu
+
+        # TODO get their children recursively
 
 
-def create_root_menu(label, window_name=None, kwargs=None) -> maya.cmds.menu:
+def create_root_menu(label, window_name=None, kwargs=None) -> pm.menu:
     """
     Create a root menu in Maya
     label: str, the label of the menu
     window_name: str, the name of the window to attach the menu to
     """
-    # todo add support for menus in other windows, e.g. the Script Editor
-    # # lsUI() might be able to replace pymel
-    # import pymel.core as pm
-    # window_name = window_name or "gMainWindow"  # default value
-    # maya_window = pm.language.melGlobals[window_name]  # returns "MayaWindow", type str
-    # same result as this
-    # maya_window = maya.mel.eval('$temp=$gMainWindow')
-    maya_window = "MayaWindow"  # hardcode main window for now
+    window_name = window_name or "gMainWindow"  # default value
+    maya_window = pm.language.melGlobals[window_name]
 
     # support adding custom kwargs from the config
     kwargs = kwargs or {}
     kwargs.setdefault("parent", maya_window)
     kwargs.setdefault("tearOff", True)
 
-    name = label.replace("_", " ")  # maya menu labels should have spaces, not underscores
+    # we require a predictable name to parent menus to from other configs, so no counter
+    # name = f"{label}_{get_counter()}"
+    name = label.replace("_", " ")  # maya menu names can't have underscores
 
-    return maya.cmds.menu(name, **kwargs)
+    return pm.menu(name, **kwargs)
 
 
 class MenuNodeMaya(MenuNodeAbstract):
 
     @property
     def _default_root_parent(self):
+
         # todo parent logic currently is re implemented in every app module
         #  can we move it to the abstract class?
         # if we provide a parent in the config, we might want to parent to a submenu
         if self.parent_path:
-            parent_path = get_compatible_name(self.parent_path)
+            parent_path = self.parent_path.replace(" ", "_")  # maya menu names can't have spaces
             return find_menu(parent_path)
 
     def _setup_sub_menu(self, parent_app_node=None):
-        self.name = get_unique_name(self.label, parent=parent_app_node)
-        kwargs = self.kwargs  # support adding custom kwargs from the config
+        # todo handle unique name, atm label can clash with other menu items
+
+        # support adding custom kwargs from the config
+        kwargs = self.kwargs
         kwargs.setdefault("tearOff", True)
+
         if not parent_app_node:
             return create_root_menu(self.label, kwargs=self.kwargs)
         else:  # make a normal sub menu
             kwargs.setdefault("subMenu", True)
             kwargs.setdefault("label", self.label)
             kwargs.setdefault("parent", parent_app_node)
-            return maya.cmds.menuItem(self.name, **kwargs)
+
+            self.name = f"{self.label}_{get_counter()}"
+            return pm.menuItem(self.name, **kwargs)
 
     def _setup_menu_item(self, parent_app_node=None):
-        self.name = get_unique_name(self.label, parent=parent_app_node)
         icon = self.icon or ""
-        tooltip = self.tooltip or "test"
-        kwargs = self.kwargs  # support adding custom kwargs from the config
+
+        # tooltip = self.tooltip or ""
+        # todo menuItem doesn't support tooltip.
+        #  could use qt instead http://discourse.techart.online/t/is-there-a-way-to-get-tooltips-for-maya-menitem/15385
+
+        # support adding custom kwargs from the config
+        kwargs = self.kwargs
         kwargs.setdefault("label", self.label)
-        kwargs.setdefault("command", self.run)
+        kwargs.setdefault("command", self.try_command)
         kwargs.setdefault("parent", parent_app_node)
         kwargs.setdefault("image", icon)
-        kwargs.setdefault("annotation", tooltip)  # shown on hover in lower left corner
-        return maya.cmds.menuItem(self.name, **kwargs)
+
+        self.name = f"{self.label}_{get_counter()}"
+
+        return pm.menuItem(self.name, **kwargs)
 
     def _setup_separator(self, parent_app_node=None):
-        self.name = get_unique_name(self.label, parent=parent_app_node)
-        kwargs = self.kwargs  # support adding custom kwargs from the config
+        self.name = f"{self.label}_{get_counter()}"
+
+        # support adding custom kwargs from the config
+        kwargs = self.kwargs
         kwargs.setdefault("divider", True)
         kwargs.setdefault("dividerLabel", self.label)
         kwargs.setdefault("parent", parent_app_node)
-        return maya.cmds.menuItem(self.name, **kwargs)
 
-    def teardown(self):
-        """Delete the menu item & its children"""
-        maya.cmds.deleteUI(self.name, menu=True)
+        return pm.menuItem(self.name, **kwargs)
 
+    def teardown(self):
+        # see https://stackoverflow.com/questions/44142119/remove-menu-item-in-maya-using-python
+        # todo can we remove self.name? bit hacky
+        pm.deleteUI(self.name, menu=True)
```

### Comparing `unimenu-0.4.0/unimenu/apps/qt.py` & `unimenu-3.0.0/unimenu/apps/qt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from unimenu.apps._abstract import MenuNodeAbstract
 import contextlib
-import logging
 
 
 with contextlib.suppress(ImportError):
     from PySide6 import QtGui, QtWidgets
     from PySide6.QtGui import QAction
 with contextlib.suppress(ImportError):
     from PyQt6 import QtGui, QtWidgets
@@ -42,26 +41,19 @@
             for widget in QtWidgets.QApplication.topLevelWidgets():
                 if widget.objectName() == "mainWindow":
                     print("FOUND MAIN WINDOW UNIMENU", main_window)
                     main_window = widget
                     break
 
         menu_bar = main_window.findChild(QtWidgets.QMenuBar)
-
-        if self.parent_path:
-            parent_menu = menu_bar.findChild(QtWidgets.QMenu, self.parent_path)
-            if not parent_menu:
-                logging.warning("Parent menu not found, using main menu bar")
-            else:
-                menu_bar = parent_menu
-
         return menu_bar
 
     def _setup_sub_menu(self, parent_app_node=None) -> QtWidgets.QMenu:
-        menu = QtWidgets.QMenu(title=self.label, objectName=self.id, parent=parent_app_node, **self.kwargs)
+        menu = QtWidgets.QMenu(title=self.label, **self.kwargs)  # parent
+        global menu_bar
         if parent_app_node:
             parent_app_node.addMenu(menu)
         return menu
 
     def _setup_menu_item(self, parent_app_node=None):
         """create a QAction from the MenuNode data"""
 
@@ -70,16 +62,21 @@
 
         # todo support:
         #  openAct.setShortcuts(QKeySequence.Open)
         #  openAct.setStatusTip(tr("Open an existing file"))
         #  PySide.QtGui.QAction.setWhatsThis()
         #  PySide.QtGui.QAction.setFont()
 
-        action = QAction(self.label, objectName=self.id, **self.kwargs)
-        action.triggered.connect(self.run)
+        action = QAction(self.label, **self.kwargs)
+
+        # qt accepts callable commands, not just string commands
+        if isinstance(self.command, str):
+            action.triggered.connect(lambda: exec(self.command))
+        else:  # callable
+            action.triggered.connect(lambda: self.command())
 
         if self.tooltip:
             if parent_app_node:
                 parent_app_node.setToolTipsVisible(True)
             action.setToolTip(self.tooltip)
 
         if self.icon:
```

### Comparing `unimenu-0.4.0/unimenu/apps/unreal.py` & `unimenu-3.0.0/unimenu/apps/unreal.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,42 +2,41 @@
 from unimenu.apps._abstract import MenuNodeAbstract
 
 
 class MenuNodeUnreal(MenuNodeAbstract):
 
     @property
     def _default_root_parent(self):
-        if self.parent_path:
-            parent_path = f"LevelEditor.MainMenu.{self.parent_path}"  # todo make this more flexible
-        else:
-            parent_path = "LevelEditor.MainMenu"
+        parent_menu_name = "LevelEditor.MainMenu"
         unreal_menus = unreal.ToolMenus.get()
-        parent_menu = unreal_menus.find_menu(parent_path)
+        parent_menu = unreal_menus.find_menu(parent_menu_name)
         return parent_menu
 
     def setup(self, parent_app_node=None, backlink=True):
-        super().setup(parent_app_node=parent_app_node, backlink=backlink)
+        super().setup(parent_app_node=parent_app_node, backlink=True)
 
         # post setup
         unreal_menus = unreal.ToolMenus.get()
         unreal_menus.refresh_all_widgets()
 
+
     def _setup_sub_menu(self, parent_app_node=None) -> unreal.ToolMenu:
+
         return parent_app_node.add_sub_menu(
             owner=parent_app_node.menu_name,
             section_name="PythonTools",
-            name=self.id,  # todo check if needs to be unique like in add_to_menu
+            name=self.label,  # todo check if needs to be uniqye like in add_to_menu
             label=self.label,  # todo add label support
             tool_tip=self.tooltip
         )
 
     def _setup_menu_item(self, parent_app_node=None) -> unreal.ToolMenuEntry:
         """add a menu item to the script menu"""
         entry = unreal.ToolMenuEntry(
-            name=self.id,  # this needs to be unique! if not set, it's autogenerated
+            # name="Python.MyCoolTool",  # this needs to be unique! if not set, it's autogenerated
             type=unreal.MultiBlockType.MENU_ENTRY,
             insert_position=unreal.ToolMenuInsert("", unreal.ToolMenuInsertType.FIRST),
         )
         if self.label:
             entry.set_label(self.label)
         if self.command:
             entry.set_string_command(
```

### Comparing `unimenu-0.4.0/unimenu/core.py` & `unimenu-3.0.0/unimenu/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import unimenu.apps._abstract
 from unimenu.apps import detect_app, App
 from unimenu.utils import getattr_recursive, load_config
 import os
 from pathlib import Path
 
 
-def load_module(module,
+def setup_module(module,
                  parent_menu: str = None,
                  menu_name: str = None,
                  function_name: str = None,
                  icon: str = None,
                  tooltip: str = None,
                  app=None,
                  smart_spaces=True,
@@ -85,34 +85,18 @@
         if tooltip:
             submodule_dict["tooltip"] = tooltip
         items.append(submodule_dict)
 
     data = {}
     if parent_menu:
         data["parent"] = parent_menu
-
-    parent_menu_label = menu_name or parent_module.__name__
-    parent_menu_label = parent_menu_label.replace('_', ' ').title() if smart_spaces else parent_menu_label
-
-    data["items"] = [{"label": parent_menu_label, "items": items}]
+    data["items"] = [{"label": menu_name or parent_module.__name__, "items": items}]
 
     # use the generated dict to set up the menu
-    return load(data, app)
-
-
-def setup_module(module,
-                    parent_menu: str = None,
-                    menu_name: str = None,
-                    function_name: str = None,
-                    icon: str = None,
-                    tooltip: str = None,
-                    app=None,
-                    smart_spaces=True,
-                    ):
-    return load_module(module, parent_menu, menu_name, function_name, icon, tooltip, app, smart_spaces).setup()
+    return setup(data, app)
 
 
 def load(arg, app: App = None) -> unimenu.apps._abstract.MenuNodeAbstract:
     """
     smart menu load from a dict, config file or module
     arg: a config (dict or str/Path) or a module (to create a menu from a folder)
     """
@@ -155,16 +139,14 @@
 
 def teardown_menu(name, app=None):
     """remove the created menu"""
     # get the top menu with name X, and delete it and all submenus
     app = app or detect_app()
     return app.menu_module.teardown_menu(name)
 
-def teardown_menus(names, app=None):
-    return [teardown_menu(name, app) for name in names]
 
 def config_dir_paths() -> "list[Path]":
     raw_path = os.environ.get("UNIMENU_CONFIG_PATH", "")
     return [Path(x) for x in raw_path.split(os.pathsep) if x]
 
 
 def discover_config_paths() -> "list[Path]":
@@ -173,40 +155,38 @@
     configs = []
     for path in paths:
         configs.extend(path.rglob("*.json"))
         configs.extend(path.rglob("*.yaml"))
     return configs
 
 
-def load_all_configs() -> unimenu.apps._abstract.MenuNodeAbstract:
+def load_all_configs():
     """load all config files in the config paths"""
     nodes = []
     config_paths = discover_config_paths()
     for config_path in config_paths:
         node = load(config_path)
         nodes.append(node)
     return nodes
 
 
-def setup_all_configs() -> unimenu.apps._abstract.MenuNodeAbstract:
+def setup_all_configs():
     """setup all config files in the config paths"""
     config_paths = discover_config_paths()
 
     # register configs without parents first, to avoid creating the child before the parent.
     # note that this is not a perfect solution
 
-    root_nodes = []
-    child_nodes = []
+    configs1 = []
+    configs2 = []
 
     for config_path in config_paths:
         config_node = load(config_path)
         if not config_node.parent_path:
-            root_nodes.append(config_node)
+            configs1.append(config_node)
         else:
-            child_nodes.append(config_node)
+            configs2.append(config_node)
 
-    for node in root_nodes:
+    for node in configs1:
         node.setup()
-    for node in child_nodes:
+    for node in configs2:
         node.setup()
-
-    return root_nodes + child_nodes
```

### Comparing `unimenu-0.4.0/unimenu/utils.py` & `unimenu-3.0.0/unimenu/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,54 @@
 import json
 
 
-def load_json(config_path) -> dict:
+def load_json(config_path):
     """get json data from a file path, return None if not json"""
     path = str(config_path)
     if not path.lower().endswith(".json"):
         return
 
     with open(config_path) as file:
         data = json.load(file)
     return data
 
 
-def load_yaml(config_path) -> dict:
+def load_yaml(config_path):
     """get yaml data from a file path, return None if not yaml"""
     path = str(config_path)
     if not path.lower().endswith(".yaml"):
         return
 
     import yaml
 
     with open(config_path) as file:
         data = yaml.load(file, Loader=yaml.SafeLoader)
     return data
 
 
-def load_config(config_path) -> dict:
+def load_config(config_path):
     """get data from a JSON or YAML config"""
     return load_json(config_path) or load_yaml(config_path)
 
 
-def save_json(data, path):
-    """save data to a json file"""
-    with open(path, "w") as file:
-        json.dump(data, file, indent=4)
-
-
-def save_yaml(data, path):
-    """save data to a yaml file"""
-    with open(path, "w") as file:
-        import yaml
-        yaml.dump(data, file, default_flow_style=False)
-
-
-def save_config(data, path):
-    """save data to a JSON or YAML config"""
-    if path.lower().endswith(".json"):
-        save_json(data, path)
-    elif path.lower().endswith(".yaml"):
-        save_yaml(data, path)
-    else:
-        raise ValueError("Invalid config file extension")
-
-
 def getattr_recursive(obj, attr: str):
     """
-    like getattr from python's std-lib, but recursive, supporting nested attributes
-    e.g. getattr_recursive(object, "mesh.name") is equivalent to object.mesh.name
-
+    getattr but recursive, supports nested attributes
     attr: provide either 1 attribute, or multiple separated by a dot
     """
     attributes = attr.split(".")
     for attribute in attributes:
         obj = getattr(obj, attribute)
     return obj
+
+
+def try_command(command, *args, **kwargs):
+    """try to run a command, return None if it fails & print the traceback"""
+    try:
+        # check if string
+        if isinstance(command, str):
+            return exec(command)
+        else:
+            return command(*args, **kwargs)
+    except Exception:
+        import traceback
+        traceback.print_exc()
```

### Comparing `unimenu-0.4.0/unimenu.egg-info/PKG-INFO` & `unimenu-3.0.0/unimenu.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unimenu
-Version: 0.4.0
+Version: 3.0.0
 Summary: easy menus from a single config across apps
 Author: hannes
 Project-URL: Homepage, https://github.com/hannesdelbeke/unimenu
 Project-URL: Documentation, https://github.com/hannesdelbeke/unimenu/wiki
 Keywords: dcc,pipeline,menu,config
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
@@ -21,55 +21,57 @@
 A pure python module to add python commands to the menu.
 
 Supports Unreal Engine, Blender, Marmoset<br>
 and any app that uses QT: Maya, Krita, Substance Painter, 3ds Max, FreeCAD, CryEngine ...
 
 For more info read the [wiki](https://github.com/hannesdelbeke/unimenu/wiki)
 
-If you use Blender, you can try the [unimenu_addon](https://github.com/hannesdelbeke/unimenu_addon)
-
 <img src="samples/menu_screen_maya.jpg" width="400"/> <img src="samples/menu_screen_unreal5.jpg" width="400"/> <img src="samples/menu_screen_krita.jpg" width="400"/> <img src="samples/menu_screen_substance_painter.jpg" width="400"/>
-<img src="samples/menu_screen_nuke.jpg" width="400"/> <img src="samples/menu_screen_katana.jpg" width="400"/>
-<img src="samples/menu_screen_mari.jpg" width="400"/>
+
 # how to use
 
+you can make your menu(s):
+- from a config
+- from a dict
+- with explicit code
+- from a folder of scripts
+
 ### load from config (YAML & JSON)
 ```yaml
 items:
   - label: my menu
     items:
       - label: my item
         command: print("Hello World")
 ```
 ```python
 import unimenu
 config_path = "path/to/config.yaml"
 unimenu.setup(config_path)
 ```
 
-
-
-### load from a dict
+### load from dynamic dict
 
 ```python
 import unimenu
 data = {"items": [{"label": test,"command": 'print("hello world")'}]}
 unimenu.setup(data)
 ```
 
 
-
 ### with code
 
 ```python
-import unimenu
-menu = unimenu.Node(label="my menu")  # create a menu
-item = unimenu.Node(label="hi", command='print("hi")')  # create a menu item
-menu.items.append(item)  # add the item to the menu
-menu.setup()  # setup the menu in the app, parented by default to the main menu bar
+import unimenu.apps.blender
+
+menu = unimenu.dccs.blender.MenuNodeBlender(label="my submenu")  # create a submenu, parent defaults to the menu bar
+item = unimenu.dccs.blender.MenuNodeBlender(label="hello", command='print("hello world")',
+                                            parent="UNIMENU_MT_my_submenu")  # add menu item to our submenu
+menu.items.append(item)  # add the item to the submenu
+menu.setup()  # setup the menu
 ```
 
 ### from a folder of scripts (module) (experimental, needs updating)
 
 great for a folder full of tools that need launching when clicking a button.
 1. ensure the folder is importable (in the sys.path)
 2. create a menthod in all submodules with the same name, e.g. def show()
@@ -94,18 +96,14 @@
 unimenu was tested in the following versions, and might work in other versions.
 - Unreal 5.0.2
 - Blender 3.2, 2.93, 2.8 (minimum)
 - Maya 2023, 2022 (minimum)
 - Substance Painter 8.2.0
 - Max 2024
 - Marmoset 3.08
-- Nuke 13 (minimum)
-- Hiero 13 (minimum)
-- Katana 5 (minimum)
-- Mari 6.0 (minimum)
 
 python 3.7+ due to f-strings and pathlib
 
 ## Development
 
 main platform is windows, would be interested to hear from mac & linux users.
```

### Comparing `unimenu-0.4.0/unimenu.egg-info/SOURCES.txt` & `unimenu-3.0.0/unimenu.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 .gitignore
 .pre-commit-config.yaml
 README.md
+openmenu.py
 pyproject.toml
 .github/workflows/python-publish.yml
 manual_tests/generic.py
 manual_tests/substance_painter_test.py
 samples/any_dcc_test.py
 samples/config.json
 samples/maya_startup_plugin.py
 samples/menu_config.yaml
 samples/menu_config_blender.yaml
 samples/menu_config_unreal.yaml
 samples/menu_config_unreal_append.yaml
-samples/menu_screen_katana.jpg
 samples/menu_screen_krita.jpg
-samples/menu_screen_mari.jpg
 samples/menu_screen_maya.jpg
-samples/menu_screen_nuke.jpg
 samples/menu_screen_substance_painter.jpg
 samples/menu_screen_unreal5.jpg
-samples/nuke_sample.py
 samples/qt_sample.py
 unimenu/__init__.py
 unimenu/core.py
 unimenu/utils.py
 unimenu.egg-info/PKG-INFO
 unimenu.egg-info/SOURCES.txt
 unimenu.egg-info/dependency_links.txt
 unimenu.egg-info/requires.txt
 unimenu.egg-info/top_level.txt
 unimenu/apps/__init__.py
 unimenu/apps/_abstract.py
 unimenu/apps/blender.py
-unimenu/apps/hiero.py
-unimenu/apps/katana.py
-unimenu/apps/mari.py
 unimenu/apps/marmoset.py
 unimenu/apps/max.py
 unimenu/apps/maya.py
-unimenu/apps/nuke.py
 unimenu/apps/qt.py
 unimenu/apps/unreal.py
```

