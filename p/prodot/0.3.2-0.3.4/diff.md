# Comparing `tmp/prodot-0.3.2.tar.gz` & `tmp/prodot-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodot-0.3.2.tar", max compression
+gzip compressed data, was "prodot-0.3.4.tar", max compression
```

## Comparing `prodot-0.3.2.tar` & `prodot-0.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-06-08 15:23:39.052025 prodot-0.3.2/LICENSE
--rw-r--r--   0        0        0     3615 2023-06-08 15:23:39.052025 prodot-0.3.2/README.md
--rw-r--r--   0        0        0      106 2023-06-08 15:23:39.052025 prodot-0.3.2/prodot/__init__.py
--rw-r--r--   0        0        0     2343 2023-06-08 17:35:21.279970 prodot-0.3.2/prodot/_base_object.py
--rw-r--r--   0        0        0     2350 2023-06-08 15:23:39.052025 prodot-0.3.2/prodot/_dot_object.py
--rw-r--r--   0        0        0     1624 2023-06-08 17:34:44.839979 prodot-0.3.2/prodot/_path_object.py
--rw-r--r--   0        0        0      443 2023-06-08 15:23:39.052025 prodot-0.3.2/prodot/_pro_object.py
--rw-r--r--   0        0        0      105 2023-06-08 15:23:39.052025 prodot-0.3.2/prodot/json_tools/__init__.py
--rw-r--r--   0        0        0       73 2023-06-08 15:23:39.052025 prodot-0.3.2/prodot/json_tools/_filter/__init__.py
--rw-r--r--   0        0        0     1029 2023-06-08 15:23:39.052025 prodot-0.3.2/prodot/json_tools/_filter/__main__.py
--rw-r--r--   0        0        0     1535 2023-06-08 15:23:39.052025 prodot-0.3.2/prodot/json_tools/_filter/_filter_byPath.py
--rw-r--r--   0        0        0     2182 2023-06-08 15:23:39.052025 prodot-0.3.2/prodot/json_tools/_filter/_filter_byValue.py
--rw-r--r--   0        0        0     1169 2023-06-08 15:23:39.062025 prodot-0.3.2/prodot/json_tools/_filter/_filtered_object.py
--rw-r--r--   0        0        0      803 2023-06-08 15:23:39.062025 prodot-0.3.2/prodot/json_tools/_get_all_paths.py
--rw-r--r--   0        0        0      392 2023-06-08 17:36:43.659948 prodot-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4188 1970-01-01 00:00:00.000000 prodot-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-08 15:23:39.052025 prodot-0.3.4/LICENSE
+-rw-r--r--   0        0        0     3615 2023-06-08 15:23:39.052025 prodot-0.3.4/README.md
+-rw-r--r--   0        0        0      106 2023-06-08 15:23:39.052025 prodot-0.3.4/prodot/__init__.py
+-rw-r--r--   0        0        0     2548 2023-06-08 19:07:40.738529 prodot-0.3.4/prodot/_base_object.py
+-rw-r--r--   0        0        0     2477 2023-06-08 19:07:41.408529 prodot-0.3.4/prodot/_dot_object.py
+-rw-r--r--   0        0        0     1624 2023-06-08 17:34:44.839979 prodot-0.3.4/prodot/_path_object.py
+-rw-r--r--   0        0        0      443 2023-06-08 15:23:39.052025 prodot-0.3.4/prodot/_pro_object.py
+-rw-r--r--   0        0        0      105 2023-06-08 15:23:39.052025 prodot-0.3.4/prodot/json_tools/__init__.py
+-rw-r--r--   0        0        0       73 2023-06-08 15:23:39.052025 prodot-0.3.4/prodot/json_tools/_filter/__init__.py
+-rw-r--r--   0        0        0     1029 2023-06-08 15:23:39.052025 prodot-0.3.4/prodot/json_tools/_filter/__main__.py
+-rw-r--r--   0        0        0     1535 2023-06-08 15:23:39.052025 prodot-0.3.4/prodot/json_tools/_filter/_filter_byPath.py
+-rw-r--r--   0        0        0     2182 2023-06-08 15:23:39.052025 prodot-0.3.4/prodot/json_tools/_filter/_filter_byValue.py
+-rw-r--r--   0        0        0     1169 2023-06-08 15:23:39.062025 prodot-0.3.4/prodot/json_tools/_filter/_filtered_object.py
+-rw-r--r--   0        0        0      803 2023-06-08 15:23:39.062025 prodot-0.3.4/prodot/json_tools/_get_all_paths.py
+-rw-r--r--   0        0        0      392 2023-06-08 19:08:03.888523 prodot-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4188 1970-01-01 00:00:00.000000 prodot-0.3.4/PKG-INFO
```

### Comparing `prodot-0.3.2/LICENSE` & `prodot-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prodot-0.3.2/README.md` & `prodot-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `prodot-0.3.2/prodot/_base_object.py` & `prodot-0.3.4/prodot/_base_object.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,46 +35,49 @@
                 return copy.deepcopy(self.caller.__class__(self.main_object))
                 
             def __exit__(self, exc_type, exc_value, traceback):
                 pass
 
         return Scope(self, self.main_object)
 
-    # @abstractmethod
-    def __contains__(self, name: str):
-        try:
-            return self.__getitem__(str(name))
-        except:
-            return False
+    def __contains__(self, value: str)-> t.Any:
+        if value in self.main_object:
+            return True
+        return False
 
     def __init__(self, main_object: t.Union[t.Dict, t.List, None] = dict()):
         '''
-        the init will receive the main object as parameter, 
+        The init will receive the main object as parameter, 
         or will create an initialize with an empty dictionary
         '''
         self.main_object = main_object
 
     def __repr__(self) -> t.Dict:
         return str(self.main_object)
     
-    
-        
-
     def true_repr(self)-> str:
         '''
         returns the original representation of the base
         object.
         '''
         type_ = type(self)
         module = type_.__module__
         qualname = type_.__qualname__
         return f"<{module}.{qualname} object at {hex(id(self))}>"
 
     def __str__(self)-> str:
         return str(self.main_object)
 
+    def __eq__(self, __value: object) -> bool:
+        return __value == self.main_object
+
     def get_value(self):
         '''
-        returns the content inside of the main_object
+        Returns the content inside of the main_object
         '''
         return self.main_object
-    
+    
+    def append(self, value: t.Any):
+        '''
+        Append the value if the main_object is a list
+        '''
+        return self.main_object.append(value)
```

### Comparing `prodot-0.3.2/prodot/_dot_object.py` & `prodot-0.3.4/prodot/_dot_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     by the children objects
     '''
     arrayTypes = [list]
     numberIndexKey = 'n'
     _temp_path = '$'
 
     def __getattr__(self, name: str) -> DotObject:
-            if type(self.main_object) in self.arrayTypes:
-                return self._get_array(name)
-            return self._get_map(name)
+        if type(self.main_object) in self.arrayTypes:
+            return self._get_array(name)
+        return self._get_map(name)
         
     def __setattr__(self, name: str, value: t.Any) -> None:
         if name in dir(self):
             return super().__setattr__(name, value)
 
         if name == 'main_object':
             self.__dict__[name] = value
@@ -40,25 +40,25 @@
             return
         
         if type(self.main_object) in self.arrayTypes:
             self._set_array(name, value)
             return
         self._set_map(name, value)
             
-
     def _get_map(self, name:str) -> DotObject:
         if name in self.main_object:
             return DotObject(self.main_object[name])
 
-        self._temp_path += f'.{name}'
-        return self
-
-    def _get_array(self, name:str) -> DotObject:
-
-        name = name.replace(self.numberIndexKey,'')
+        raise ValueError(f"path <<{name}>> not found in  the main_object")
+        # self._temp_path += f'.{name}'
+        # return self
+
+    def _get_array(self, name:str) -> DotObject:         
+        if name.startswith(self.numberIndexKey):
+            name = name.replace(self.numberIndexKey,'')
         try:
             return DotObject(self.main_object[int(name)])
         except IndexError:
             raise Exception(f"Array index doesn't exist in DotObject {self.true_repr()}")
     
     def _set_map(self, name:str, value:t.Any):
         self.main_object[name] = value
```

### Comparing `prodot-0.3.2/prodot/_path_object.py` & `prodot-0.3.4/prodot/_path_object.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.2/prodot/json_tools/_filter/__main__.py` & `prodot-0.3.4/prodot/json_tools/_filter/__main__.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.2/prodot/json_tools/_filter/_filter_byPath.py` & `prodot-0.3.4/prodot/json_tools/_filter/_filter_byPath.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.2/prodot/json_tools/_filter/_filter_byValue.py` & `prodot-0.3.4/prodot/json_tools/_filter/_filter_byValue.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.2/prodot/json_tools/_filter/_filtered_object.py` & `prodot-0.3.4/prodot/json_tools/_filter/_filtered_object.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.2/prodot/json_tools/_get_all_paths.py` & `prodot-0.3.4/prodot/json_tools/_get_all_paths.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.2/PKG-INFO` & `prodot-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodot
-Version: 0.3.2
+Version: 0.3.4
 Summary: 
 License: GNU GENERAL PUBLIC LICENSE
 Author: Matheus Menezes Almeida
 Author-email: mrotame@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

