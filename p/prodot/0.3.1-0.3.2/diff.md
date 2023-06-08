# Comparing `tmp/prodot-0.3.1.tar.gz` & `tmp/prodot-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodot-0.3.1.tar", max compression
+gzip compressed data, was "prodot-0.3.2.tar", max compression
```

## Comparing `prodot-0.3.1.tar` & `prodot-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-02-02 22:57:05.837289 prodot-0.3.1/LICENSE
--rw-r--r--   0        0        0     3615 2023-02-05 17:14:39.595468 prodot-0.3.1/README.md
--rw-r--r--   0        0        0      106 2023-02-05 15:34:07.055460 prodot-0.3.1/prodot/__init__.py
--rw-r--r--   0        0        0     1917 2023-02-25 19:54:30.871506 prodot-0.3.1/prodot/_base_object.py
--rw-r--r--   0        0        0     2350 2023-02-25 16:31:08.591492 prodot-0.3.1/prodot/_dot_object.py
--rw-r--r--   0        0        0     1622 2023-02-25 16:30:58.681492 prodot-0.3.1/prodot/_path_object.py
--rw-r--r--   0        0        0      443 2023-02-09 23:58:42.110378 prodot-0.3.1/prodot/_pro_object.py
--rw-r--r--   0        0        0      105 2023-02-16 13:06:21.052079 prodot-0.3.1/prodot/json_tools/__init__.py
--rw-r--r--   0        0        0       73 2023-02-16 13:07:22.852084 prodot-0.3.1/prodot/json_tools/_filter/__init__.py
--rw-r--r--   0        0        0     1029 2023-02-18 22:34:21.310926 prodot-0.3.1/prodot/json_tools/_filter/__main__.py
--rw-r--r--   0        0        0     1535 2023-02-18 02:10:47.370927 prodot-0.3.1/prodot/json_tools/_filter/_filter_byPath.py
--rw-r--r--   0        0        0     2182 2023-02-18 23:09:46.000914 prodot-0.3.1/prodot/json_tools/_filter/_filter_byValue.py
--rw-r--r--   0        0        0     1169 2023-02-25 16:36:28.891495 prodot-0.3.1/prodot/json_tools/_filter/_filtered_object.py
--rw-r--r--   0        0        0      803 2023-02-15 17:19:20.960887 prodot-0.3.1/prodot/json_tools/_get_all_paths.py
--rw-r--r--   0        0        0      392 2023-02-25 19:54:59.731503 prodot-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4433 1970-01-01 00:00:00.000000 prodot-0.3.1/setup.py
--rw-r--r--   0        0        0     4188 1970-01-01 00:00:00.000000 prodot-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-08 15:23:39.052025 prodot-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3615 2023-06-08 15:23:39.052025 prodot-0.3.2/README.md
+-rw-r--r--   0        0        0      106 2023-06-08 15:23:39.052025 prodot-0.3.2/prodot/__init__.py
+-rw-r--r--   0        0        0     2343 2023-06-08 17:35:21.279970 prodot-0.3.2/prodot/_base_object.py
+-rw-r--r--   0        0        0     2350 2023-06-08 15:23:39.052025 prodot-0.3.2/prodot/_dot_object.py
+-rw-r--r--   0        0        0     1624 2023-06-08 17:34:44.839979 prodot-0.3.2/prodot/_path_object.py
+-rw-r--r--   0        0        0      443 2023-06-08 15:23:39.052025 prodot-0.3.2/prodot/_pro_object.py
+-rw-r--r--   0        0        0      105 2023-06-08 15:23:39.052025 prodot-0.3.2/prodot/json_tools/__init__.py
+-rw-r--r--   0        0        0       73 2023-06-08 15:23:39.052025 prodot-0.3.2/prodot/json_tools/_filter/__init__.py
+-rw-r--r--   0        0        0     1029 2023-06-08 15:23:39.052025 prodot-0.3.2/prodot/json_tools/_filter/__main__.py
+-rw-r--r--   0        0        0     1535 2023-06-08 15:23:39.052025 prodot-0.3.2/prodot/json_tools/_filter/_filter_byPath.py
+-rw-r--r--   0        0        0     2182 2023-06-08 15:23:39.052025 prodot-0.3.2/prodot/json_tools/_filter/_filter_byValue.py
+-rw-r--r--   0        0        0     1169 2023-06-08 15:23:39.062025 prodot-0.3.2/prodot/json_tools/_filter/_filtered_object.py
+-rw-r--r--   0        0        0      803 2023-06-08 15:23:39.062025 prodot-0.3.2/prodot/json_tools/_get_all_paths.py
+-rw-r--r--   0        0        0      392 2023-06-08 17:36:43.659948 prodot-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4188 1970-01-01 00:00:00.000000 prodot-0.3.2/PKG-INFO
```

### Comparing `prodot-0.3.1/LICENSE` & `prodot-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prodot-0.3.1/README.md` & `prodot-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `prodot-0.3.1/prodot/_base_object.py` & `prodot-0.3.2/prodot/_base_object.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import typing as t
-from abc import ABC
+from abc import ABC, abstractmethod
 import copy
 from contextvars import ContextVar
 
 class BaseObject(ABC):
     '''
     ## Description
     A base object to be used by all other object types (like the dot object and the path object). This abstract class has the basic and common configuration for all the future object classes
@@ -15,37 +15,54 @@
     
     
     '''The main object is the object that the class will be representing (most times, it will be a list or a dictionary)'''   
     main_object: t.Any
 
     @property
     def scoped(self):
+        '''
+        Return the Object as a temporary object to be used within a scope. Ex:
+        ```Python
+        >> with my_obj.scoped as temp_object:
+        >> ... print( temp_object.get_value() )
+        ```
+        '''
         class Scope:
             def __init__(self, caller: BaseObject, main_object:t.Any):
                 self.caller = caller
                 self.main_object = main_object
 
             def __enter__(self):
                 return copy.deepcopy(self.caller.__class__(self.main_object))
                 
             def __exit__(self, exc_type, exc_value, traceback):
                 pass
 
         return Scope(self, self.main_object)
 
+    # @abstractmethod
+    def __contains__(self, name: str):
+        try:
+            return self.__getitem__(str(name))
+        except:
+            return False
+
     def __init__(self, main_object: t.Union[t.Dict, t.List, None] = dict()):
         '''
         the init will receive the main object as parameter, 
         or will create an initialize with an empty dictionary
         '''
         self.main_object = main_object
 
     def __repr__(self) -> t.Dict:
         return str(self.main_object)
     
+    
+        
+
     def true_repr(self)-> str:
         '''
         returns the original representation of the base
         object.
         '''
         type_ = type(self)
         module = type_.__module__
@@ -55,8 +72,9 @@
     def __str__(self)-> str:
         return str(self.main_object)
 
     def get_value(self):
         '''
         returns the content inside of the main_object
         '''
-        return self.main_object
+        return self.main_object
+
```

### Comparing `prodot-0.3.1/prodot/_dot_object.py` & `prodot-0.3.2/prodot/_dot_object.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.1/prodot/_path_object.py` & `prodot-0.3.2/prodot/_path_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         '''
         return self.__filter_object(self.main_object, self)
         
     def __getitem__(self, name:str)->PathObject:
         try:
             return PathObject(parse('$.'+name).find(self.main_object)[0].value)
         except IndexError:
-            raise Exception(f"path <<{name}>> not found at the main_object")
+            raise IndexError(f"path <<{name}>> not found in  the main_object")
 
     def __setitem__(self, name:str, value:t.Any):
         path = parse('$.'+name)
         path.update_or_create(self.main_object, value)
 
     def get_all_paths(self, **kwargs)->t.Iterable:
         '''
```

### Comparing `prodot-0.3.1/prodot/json_tools/_filter/__main__.py` & `prodot-0.3.2/prodot/json_tools/_filter/__main__.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.1/prodot/json_tools/_filter/_filter_byPath.py` & `prodot-0.3.2/prodot/json_tools/_filter/_filter_byPath.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.1/prodot/json_tools/_filter/_filter_byValue.py` & `prodot-0.3.2/prodot/json_tools/_filter/_filter_byValue.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.1/prodot/json_tools/_filter/_filtered_object.py` & `prodot-0.3.2/prodot/json_tools/_filter/_filtered_object.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.1/prodot/json_tools/_get_all_paths.py` & `prodot-0.3.2/prodot/json_tools/_get_all_paths.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.1/setup.py` & `prodot-0.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,131 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: prodot
+Version: 0.3.2
+Summary: 
+License: GNU GENERAL PUBLIC LICENSE
+Author: Matheus Menezes Almeida
+Author-email: mrotame@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0)
+Description-Content-Type: text/markdown
+
+# Prodot
+
+A new way to deal with dictionaries and lists in python.
+Treat data like classes, or by reading/writing data with json paths
+```Python
+>>> from prodot import ProObject
+>>> my_obj = ProObject({'foo':{'bar':['eggs']}})
+
+>>> my_obj.foo.bar.n1.get_value()
+'eggs'
+
+>>> my_obj['$.foo.bar.[0]'].get_value()
+'eggs
+```
+
+# Getting started
+
+## install
+```
+pip install prodot
+```
+
+## Usage
+
+Import the pro object from the prodot library. You can create a new empty dictionary, or start with a filled one
+
+```Python
+# No parameters instances an empty dictionary
+>>> my_new_obj = ProObject() 
+
+# The pro object can be initialized with a dictionary
+>>> my_dict_obj = ProObject({"foo":["bar","eggs"]})
+
+# The pro object can also initialize with a list
+>>> my_list_obj = ProObject([ [1,2,3], ["a","b","c"], [{"foo":"bar"}, {"bar":"eggs"}] ])
+
+```
+
+### Dot notation usage
+By using the pro-object you can use the dictionary as a class
+
+```Python
+>>> my_json = {
+...     "userData": {
+...         "name": "John",
+...         "age": "38",
+...         "shoppingCart":[
+...             {"cellphone": 999.99},
+...             {"notebook": 2999.99},
+...             {"wireless keyboard": 299.99}
+...         ]
+...     }
+... }
+
+>>> my_new_obj = ProObject(my_json)
+
+>>> shoppingCart = my_new_obj.userData.shoppingCart
+```
+
+The ProObject will return another instance of the ProObject with the main_object attribute as being the selected path.
+
+```Python
+>>> type(shoppingCart)
+<class 'prodot.pro_object.ProObject'>
+```
+
+To get the raw value of the object, you can use the `.get_value()` function.
+
+```Python
+>>> shoppingCart.get_value()
+[{"cellphone": 999.99}, {"notebook": 2999.99}, {"wireless keyboard": 299.99}]
+
+# or by using the get_value directly at the path
+>>> my_new_obj.userData.shoppingCart.get_value()
+[{"cellphone": 999.99}, {"notebook": 2999.99}, {"wireless keyboard": 299.99}]
+
+>>> type(shoppingCart.get_value())
+<class 'dict'>
+```
+
+You can also add new information to the instancied object
+
+```Python
+# n3 means list index 3 (will be added as 4th item)
+>>> my_new_obj.userData.shoppingCart.n3 = {"monitor": 699.99}
+>>> my_new_obj.userData.shoppingCart.get_value()
+[{"cellphone": 999.99}, {"notebook": 2999.99}, {"wireless keyboard": 299.99}, {"monitor": 399.99}]
+```
+Python doesn't accept list indexes to be used as a class attribute. For solve this problem, list indexes start with the `n` letter (like n0, n1, ...)
+
+### Json path usage
+
+If you prefere or need to use json paths, it is possible to write and retrieve information using json path strings.
+
+```Python
+>>> my_new_obj['$.userData.shoppingCart[4]'] = {'FunStation 6 Series T':'699,99'}
+
+>>> my_new_obj['$.userData.shoppingCart'].get_value()
+[{"cellphone": 999.99}, {"notebook": 2999.99}, {"wireless keyboard": 299.99}, {"monitor": 399.99}, {'FunStation 6 Series T':'699,99'}]
+```
+
+Note that by using a json path string, list indexes must not have `n` as their first value.
+
+You can view all possible json_paths from object by using the `get_all_paths` attribute.
+
+```Python
+>>> my_new_obj.get_all_paths()
+<generator object PathObject.all_paths_from_main_object at 0x7f6a012b5c80>
+
+>>> list(my_new_obj.get_all_paths())
+['.userData', '.userData.name', '.userData.age', '.userData.shoppingCart', '.userData.shoppingCart[0]', '.userData.shoppingCart[0].cellphone', '.userData.shoppingCart[1]', '.userData.shoppingCart[1].notebook', '.userData.shoppingCart[2]', '.userData.shoppingCart[2].wireless keyboard', '.userData.shoppingCart[3]', '.userData.shoppingCart[3].monitor', '.userData.shoppingCart[4]', '.userData.shoppingCart[4].FunStation 6 Series T']
+```
 
-packages = \
-['prodot', 'prodot.json_tools', 'prodot.json_tools._filter']
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['jsonpath-ng>=1.5.3,<2.0.0']
-
-setup_kwargs = {
-    'name': 'prodot',
-    'version': '0.3.1',
-    'description': '',
-    'long_description': '# Prodot\n\nA new way to deal with dictionaries and lists in python.\nTreat data like classes, or by reading/writing data with json paths\n```Python\n>>> from prodot import ProObject\n>>> my_obj = ProObject({\'foo\':{\'bar\':[\'eggs\']}})\n\n>>> my_obj.foo.bar.n1.get_value()\n\'eggs\'\n\n>>> my_obj[\'$.foo.bar.[0]\'].get_value()\n\'eggs\n```\n\n# Getting started\n\n## install\n```\npip install prodot\n```\n\n## Usage\n\nImport the pro object from the prodot library. You can create a new empty dictionary, or start with a filled one\n\n```Python\n# No parameters instances an empty dictionary\n>>> my_new_obj = ProObject() \n\n# The pro object can be initialized with a dictionary\n>>> my_dict_obj = ProObject({"foo":["bar","eggs"]})\n\n# The pro object can also initialize with a list\n>>> my_list_obj = ProObject([ [1,2,3], ["a","b","c"], [{"foo":"bar"}, {"bar":"eggs"}] ])\n\n```\n\n### Dot notation usage\nBy using the pro-object you can use the dictionary as a class\n\n```Python\n>>> my_json = {\n...     "userData": {\n...         "name": "John",\n...         "age": "38",\n...         "shoppingCart":[\n...             {"cellphone": 999.99},\n...             {"notebook": 2999.99},\n...             {"wireless keyboard": 299.99}\n...         ]\n...     }\n... }\n\n>>> my_new_obj = ProObject(my_json)\n\n>>> shoppingCart = my_new_obj.userData.shoppingCart\n```\n\nThe ProObject will return another instance of the ProObject with the main_object attribute as being the selected path.\n\n```Python\n>>> type(shoppingCart)\n<class \'prodot.pro_object.ProObject\'>\n```\n\nTo get the raw value of the object, you can use the `.get_value()` function.\n\n```Python\n>>> shoppingCart.get_value()\n[{"cellphone": 999.99}, {"notebook": 2999.99}, {"wireless keyboard": 299.99}]\n\n# or by using the get_value directly at the path\n>>> my_new_obj.userData.shoppingCart.get_value()\n[{"cellphone": 999.99}, {"notebook": 2999.99}, {"wireless keyboard": 299.99}]\n\n>>> type(shoppingCart.get_value())\n<class \'dict\'>\n```\n\nYou can also add new information to the instancied object\n\n```Python\n# n3 means list index 3 (will be added as 4th item)\n>>> my_new_obj.userData.shoppingCart.n3 = {"monitor": 699.99}\n>>> my_new_obj.userData.shoppingCart.get_value()\n[{"cellphone": 999.99}, {"notebook": 2999.99}, {"wireless keyboard": 299.99}, {"monitor": 399.99}]\n```\nPython doesn\'t accept list indexes to be used as a class attribute. For solve this problem, list indexes start with the `n` letter (like n0, n1, ...)\n\n### Json path usage\n\nIf you prefere or need to use json paths, it is possible to write and retrieve information using json path strings.\n\n```Python\n>>> my_new_obj[\'$.userData.shoppingCart[4]\'] = {\'FunStation 6 Series T\':\'699,99\'}\n\n>>> my_new_obj[\'$.userData.shoppingCart\'].get_value()\n[{"cellphone": 999.99}, {"notebook": 2999.99}, {"wireless keyboard": 299.99}, {"monitor": 399.99}, {\'FunStation 6 Series T\':\'699,99\'}]\n```\n\nNote that by using a json path string, list indexes must not have `n` as their first value.\n\nYou can view all possible json_paths from object by using the `get_all_paths` attribute.\n\n```Python\n>>> my_new_obj.get_all_paths()\n<generator object PathObject.all_paths_from_main_object at 0x7f6a012b5c80>\n\n>>> list(my_new_obj.get_all_paths())\n[\'.userData\', \'.userData.name\', \'.userData.age\', \'.userData.shoppingCart\', \'.userData.shoppingCart[0]\', \'.userData.shoppingCart[0].cellphone\', \'.userData.shoppingCart[1]\', \'.userData.shoppingCart[1].notebook\', \'.userData.shoppingCart[2]\', \'.userData.shoppingCart[2].wireless keyboard\', \'.userData.shoppingCart[3]\', \'.userData.shoppingCart[3].monitor\', \'.userData.shoppingCart[4]\', \'.userData.shoppingCart[4].FunStation 6 Series T\']\n```\n\n',
-    'author': 'Matheus Menezes Almeida',
-    'author_email': 'mrotame@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

