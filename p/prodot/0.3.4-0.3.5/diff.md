# Comparing `tmp/prodot-0.3.4.tar.gz` & `tmp/prodot-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodot-0.3.4.tar", max compression
+gzip compressed data, was "prodot-0.3.5.tar", max compression
```

## Comparing `prodot-0.3.4.tar` & `prodot-0.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-06-08 15:23:39.052025 prodot-0.3.4/LICENSE
--rw-r--r--   0        0        0     3615 2023-06-08 15:23:39.052025 prodot-0.3.4/README.md
--rw-r--r--   0        0        0      106 2023-06-08 15:23:39.052025 prodot-0.3.4/prodot/__init__.py
--rw-r--r--   0        0        0     2548 2023-06-08 19:07:40.738529 prodot-0.3.4/prodot/_base_object.py
--rw-r--r--   0        0        0     2477 2023-06-08 19:07:41.408529 prodot-0.3.4/prodot/_dot_object.py
--rw-r--r--   0        0        0     1624 2023-06-08 17:34:44.839979 prodot-0.3.4/prodot/_path_object.py
--rw-r--r--   0        0        0      443 2023-06-08 15:23:39.052025 prodot-0.3.4/prodot/_pro_object.py
--rw-r--r--   0        0        0      105 2023-06-08 15:23:39.052025 prodot-0.3.4/prodot/json_tools/__init__.py
--rw-r--r--   0        0        0       73 2023-06-08 15:23:39.052025 prodot-0.3.4/prodot/json_tools/_filter/__init__.py
--rw-r--r--   0        0        0     1029 2023-06-08 15:23:39.052025 prodot-0.3.4/prodot/json_tools/_filter/__main__.py
--rw-r--r--   0        0        0     1535 2023-06-08 15:23:39.052025 prodot-0.3.4/prodot/json_tools/_filter/_filter_byPath.py
--rw-r--r--   0        0        0     2182 2023-06-08 15:23:39.052025 prodot-0.3.4/prodot/json_tools/_filter/_filter_byValue.py
--rw-r--r--   0        0        0     1169 2023-06-08 15:23:39.062025 prodot-0.3.4/prodot/json_tools/_filter/_filtered_object.py
--rw-r--r--   0        0        0      803 2023-06-08 15:23:39.062025 prodot-0.3.4/prodot/json_tools/_get_all_paths.py
--rw-r--r--   0        0        0      392 2023-06-08 19:08:03.888523 prodot-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     4188 1970-01-01 00:00:00.000000 prodot-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-08 15:23:39.052025 prodot-0.3.5/LICENSE
+-rw-r--r--   0        0        0     3615 2023-06-08 15:23:39.052025 prodot-0.3.5/README.md
+-rw-r--r--   0        0        0      106 2023-06-08 15:23:39.052025 prodot-0.3.5/prodot/__init__.py
+-rw-r--r--   0        0        0     2615 2023-06-08 19:51:16.247848 prodot-0.3.5/prodot/_base_object.py
+-rw-r--r--   0        0        0     2510 2023-06-08 19:34:38.298107 prodot-0.3.5/prodot/_dot_object.py
+-rw-r--r--   0        0        0     1741 2023-06-08 19:34:10.768114 prodot-0.3.5/prodot/_path_object.py
+-rw-r--r--   0        0        0      443 2023-06-08 15:23:39.052025 prodot-0.3.5/prodot/_pro_object.py
+-rw-r--r--   0        0        0      105 2023-06-08 15:23:39.052025 prodot-0.3.5/prodot/json_tools/__init__.py
+-rw-r--r--   0        0        0       73 2023-06-08 15:23:39.052025 prodot-0.3.5/prodot/json_tools/_filter/__init__.py
+-rw-r--r--   0        0        0     1029 2023-06-08 15:23:39.052025 prodot-0.3.5/prodot/json_tools/_filter/__main__.py
+-rw-r--r--   0        0        0     1535 2023-06-08 15:23:39.052025 prodot-0.3.5/prodot/json_tools/_filter/_filter_byPath.py
+-rw-r--r--   0        0        0     2158 2023-06-08 19:36:47.368074 prodot-0.3.5/prodot/json_tools/_filter/_filter_byValue.py
+-rw-r--r--   0        0        0     1169 2023-06-08 15:23:39.062025 prodot-0.3.5/prodot/json_tools/_filter/_filtered_object.py
+-rw-r--r--   0        0        0      803 2023-06-08 15:23:39.062025 prodot-0.3.5/prodot/json_tools/_get_all_paths.py
+-rw-r--r--   0        0        0      392 2023-06-08 19:52:37.417827 prodot-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     4188 1970-01-01 00:00:00.000000 prodot-0.3.5/PKG-INFO
```

### Comparing `prodot-0.3.4/LICENSE` & `prodot-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prodot-0.3.4/README.md` & `prodot-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `prodot-0.3.4/prodot/_base_object.py` & `prodot-0.3.5/prodot/_base_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,8 +76,11 @@
         '''
         return self.main_object
     
     def append(self, value: t.Any):
         '''
         Append the value if the main_object is a list
         '''
-        return self.main_object.append(value)
+        return self.main_object.append(value)
+    
+    def __iter__(self):
+        return iter(self.main_object)
```

### Comparing `prodot-0.3.4/prodot/_dot_object.py` & `prodot-0.3.5/prodot/_dot_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,18 +15,23 @@
     `main_object:` a Dict or List object that will be interpreted
     by the children objects
     '''
     arrayTypes = [list]
     numberIndexKey = 'n'
     _temp_path = '$'
 
-    def __getattr__(self, name: str) -> DotObject:
+    def __getattr__(self, name: str) -> t.Self:
         if type(self.main_object) in self.arrayTypes:
-            return self._get_array(name)
-        return self._get_map(name)
+            res = self._get_array(name)
+        else:
+            res = self._get_map(name)
+
+        if isinstance(res, list) or isinstance(res, dict):
+            return self.__class__(res)
+        return res
         
     def __setattr__(self, name: str, value: t.Any) -> None:
         if name in dir(self):
             return super().__setattr__(name, value)
 
         if name == 'main_object':
             self.__dict__[name] = value
@@ -40,27 +45,25 @@
             return
         
         if type(self.main_object) in self.arrayTypes:
             self._set_array(name, value)
             return
         self._set_map(name, value)
             
-    def _get_map(self, name:str) -> DotObject:
+    def _get_map(self, name:str) -> t.Any:
         if name in self.main_object:
-            return DotObject(self.main_object[name])
+            return self.main_object[name]
 
-        raise ValueError(f"path <<{name}>> not found in  the main_object")
-        # self._temp_path += f'.{name}'
-        # return self
+        raise ValueError(f"Key <<{name}>> not found in  the main_object")
 
-    def _get_array(self, name:str) -> DotObject:         
+    def _get_array(self, name:str) -> t.Any:    
         if name.startswith(self.numberIndexKey):
             name = name.replace(self.numberIndexKey,'')
         try:
-            return DotObject(self.main_object[int(name)])
+            return self.main_object[int(name)]
         except IndexError:
             raise Exception(f"Array index doesn't exist in DotObject {self.true_repr()}")
     
     def _set_map(self, name:str, value:t.Any):
         self.main_object[name] = value
 
     def _set_array(self, name:str, value:t.Any):
```

### Comparing `prodot-0.3.4/prodot/_path_object.py` & `prodot-0.3.5/prodot/_path_object.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,17 +30,21 @@
     def filter(self)->Filter:
         '''
         returns a filter instance responsible to extract data
         from the main_object
         '''
         return self.__filter_object(self.main_object, self)
         
-    def __getitem__(self, name:str)->PathObject:
+    def __getitem__(self, name:str)->t.Self:
         try:
-            return PathObject(parse('$.'+name).find(self.main_object)[0].value)
+            res = parse('$.'+name).find(self.main_object)[0].value
+            if isinstance(res, list) or isinstance(res, dict):
+                return self.__class__(res)
+            return res
+    
         except IndexError:
             raise IndexError(f"path <<{name}>> not found in  the main_object")
 
     def __setitem__(self, name:str, value:t.Any):
         path = parse('$.'+name)
         path.update_or_create(self.main_object, value)
```

### Comparing `prodot-0.3.4/prodot/json_tools/_filter/__main__.py` & `prodot-0.3.5/prodot/json_tools/_filter/__main__.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.4/prodot/json_tools/_filter/_filter_byPath.py` & `prodot-0.3.5/prodot/json_tools/_filter/_filter_byPath.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.4/prodot/json_tools/_filter/_filter_byValue.py` & `prodot-0.3.5/prodot/json_tools/_filter/_filter_byValue.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Check for each possible json path in the received json object,
         compare each value from each path, and returns a FilteredObject
         containing all the possible json paths that contains the data
         parameter anywhere in the value
         '''
         
         for path in get_all_paths(self.json):
-            value = self.pathObject(self.json)[path].get_value()
+            value = self.pathObject(self.json)[path]
             
             try: str_to_search in value
             except Exception: value = str(value)
             if str(str_to_search) in value:
                 self.filtered_paths.append(path)
                 path = parse(path)
                 path.update_or_create(self.filtered_json, path.find(self.json)[0].value)
@@ -36,15 +36,15 @@
     def matches(self, data_to_search:any):
         '''
         Check for each possible json path in the received json object,
         compare each value from each path, and returns a FilteredObject
         containing all the possible json paths that the data_to_search matches exactly the value
         '''
         for path in get_all_paths(self.json):
-            value = self.pathObject(self.json)[path].get_value()
+            value = self.pathObject(self.json)[path]
             try: data_to_search in value
             except Exception: value = str(value)
             if str(data_to_search) == value:
                 self.filtered_paths.append(path)
                 path = parse(path)
                 path.update_or_create(self.filtered_json, path.find(self.json)[0].value)
```

### Comparing `prodot-0.3.4/prodot/json_tools/_filter/_filtered_object.py` & `prodot-0.3.5/prodot/json_tools/_filter/_filtered_object.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.4/prodot/json_tools/_get_all_paths.py` & `prodot-0.3.5/prodot/json_tools/_get_all_paths.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.4/PKG-INFO` & `prodot-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodot
-Version: 0.3.4
+Version: 0.3.5
 Summary: 
 License: GNU GENERAL PUBLIC LICENSE
 Author: Matheus Menezes Almeida
 Author-email: mrotame@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

