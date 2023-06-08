# Comparing `tmp/formalmath-0.0.4.tar.gz` & `tmp/formalmath-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formalmath-0.0.4.tar", last modified: Wed Jun  7 05:37:03 2023, max compression
+gzip compressed data, was "formalmath-0.0.5.tar", last modified: Wed Jun  7 06:54:06 2023, max compression
```

## Comparing `formalmath-0.0.4.tar` & `formalmath-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 05:37:03.346152 formalmath-0.0.4/
--rw-rw-rw-   0        0        0     1695 2023-06-07 05:37:03.346152 formalmath-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1249 2023-06-07 05:34:30.000000 formalmath-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 05:37:03.344153 formalmath-0.0.4/formalmath/
--rw-rw-rw-   0        0        0       19 2023-06-06 03:06:28.000000 formalmath-0.0.4/formalmath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:37:03.346152 formalmath-0.0.4/formalmath/setmm/
--rw-rw-rw-   0        0        0       28 2023-06-06 03:07:05.000000 formalmath-0.0.4/formalmath/setmm/__init__.py
--rw-rw-rw-   0        0        0     5539 2023-06-07 05:14:32.000000 formalmath-0.0.4/formalmath/setmm/basic_classes.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:37:03.345152 formalmath-0.0.4/formalmath.egg-info/
--rw-rw-rw-   0        0        0     1695 2023-06-07 05:37:03.000000 formalmath-0.0.4/formalmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-06-07 05:37:03.000000 formalmath-0.0.4/formalmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 05:37:03.000000 formalmath-0.0.4/formalmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-07 05:37:03.000000 formalmath-0.0.4/formalmath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 05:37:03.346152 formalmath-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      743 2023-06-07 05:36:45.000000 formalmath-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:54:06.517477 formalmath-0.0.5/
+-rw-rw-rw-   0        0        0     1780 2023-06-07 06:54:06.517477 formalmath-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1334 2023-06-07 06:52:55.000000 formalmath-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 06:54:06.514478 formalmath-0.0.5/formalmath/
+-rw-rw-rw-   0        0        0       19 2023-06-06 03:06:28.000000 formalmath-0.0.5/formalmath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:54:06.517477 formalmath-0.0.5/formalmath/setmm/
+-rw-rw-rw-   0        0        0       28 2023-06-06 03:07:05.000000 formalmath-0.0.5/formalmath/setmm/__init__.py
+-rw-rw-rw-   0        0        0     6056 2023-06-07 06:20:42.000000 formalmath-0.0.5/formalmath/setmm/basic_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:54:06.516477 formalmath-0.0.5/formalmath.egg-info/
+-rw-rw-rw-   0        0        0     1780 2023-06-07 06:54:06.000000 formalmath-0.0.5/formalmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-06-07 06:54:06.000000 formalmath-0.0.5/formalmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 06:54:06.000000 formalmath-0.0.5/formalmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-07 06:54:06.000000 formalmath-0.0.5/formalmath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 06:54:06.517477 formalmath-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-06-07 06:51:55.000000 formalmath-0.0.5/setup.py
```

### Comparing `formalmath-0.0.4/PKG-INFO` & `formalmath-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formalmath
-Version: 0.0.4
+Version: 0.0.5
 Summary: a python port of formal mathematics proof verifier.
 Home-page: https://github.com/lixiang90/formalmath.git
 Author: lixiang90
 Author-email: lixiang90@github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,16 @@
 
 A port for [metamath](https://us.metamath.org) and `set.mm`. The language `metamath` is a math proof verifying language. And, `set.mm` is its main database of theorems, based on the classical ZFC axiom system.
 
 `MObject` is the basic class. Any `MObject` have a label. Some of them have short_code or metamath_code. The label system is unique (if you create a new MObject with the same label with existing one, the program will raise ValueError). So does the short_code and metamath_code.
 
  `Constant` is the class of constants, corresponding to $c statements in metamath.
 
+`Variable` is the class of variables, corresponding to $v statements in metamath.
+
 The port of other concepts in metamath and set.mm is a work in process.
 
 Example code:
 
 ```python
 from formalmath import setmm
 test1 = setmm.MObject("x1")
```

### Comparing `formalmath-0.0.4/README.md` & `formalmath-0.0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 A port for [metamath](https://us.metamath.org) and `set.mm`. The language `metamath` is a math proof verifying language. And, `set.mm` is its main database of theorems, based on the classical ZFC axiom system.
 
 `MObject` is the basic class. Any `MObject` have a label. Some of them have short_code or metamath_code. The label system is unique (if you create a new MObject with the same label with existing one, the program will raise ValueError). So does the short_code and metamath_code.
 
  `Constant` is the class of constants, corresponding to $c statements in metamath.
 
+`Variable` is the class of variables, corresponding to $v statements in metamath.
+
 The port of other concepts in metamath and set.mm is a work in process.
 
 Example code:
 
 ```python
 from formalmath import setmm
 test1 = setmm.MObject("x1")
```

### Comparing `formalmath-0.0.4/formalmath/setmm/basic_classes.py` & `formalmath-0.0.5/formalmath/setmm/basic_classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,14 +112,31 @@
     
     def __str__(self):
         '''
         print Constant. will override the __str__ method in MObject.
         '''
         return f"Constant(\"{self.label}\")"
 
+class Variable(MObject):
+    '''
+    $v statement in metamath, denote variable objects.
+    '''
+    def __init__(self, label, short_code=None, metamath_code=None):
+        '''
+        construction function of Variable.
+        just need to inherit from MObject.
+        '''
+        super().__init__(label, short_code, metamath_code)
+    
+    def __str__(self):
+        '''
+        print Variable. will override the __str__ method in MObject.
+        '''
+        return f"Variable(\"{self.label}\")"
+
 if __name__=='__main__':
     test1 = MObject("x1")
     test2 = MObject("y1")
     # test3 = MObject("x1")
     print(test1) # output: MObject("x1")
     test3 = MObject.find_MObject_by_label("y1")
     print(test3) # output: MObject("y1")
```

### Comparing `formalmath-0.0.4/formalmath.egg-info/PKG-INFO` & `formalmath-0.0.5/formalmath.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formalmath
-Version: 0.0.4
+Version: 0.0.5
 Summary: a python port of formal mathematics proof verifier.
 Home-page: https://github.com/lixiang90/formalmath.git
 Author: lixiang90
 Author-email: lixiang90@github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,16 @@
 
 A port for [metamath](https://us.metamath.org) and `set.mm`. The language `metamath` is a math proof verifying language. And, `set.mm` is its main database of theorems, based on the classical ZFC axiom system.
 
 `MObject` is the basic class. Any `MObject` have a label. Some of them have short_code or metamath_code. The label system is unique (if you create a new MObject with the same label with existing one, the program will raise ValueError). So does the short_code and metamath_code.
 
  `Constant` is the class of constants, corresponding to $c statements in metamath.
 
+`Variable` is the class of variables, corresponding to $v statements in metamath.
+
 The port of other concepts in metamath and set.mm is a work in process.
 
 Example code:
 
 ```python
 from formalmath import setmm
 test1 = setmm.MObject("x1")
```

### Comparing `formalmath-0.0.4/setup.py` & `formalmath-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="formalmath",  # Replace with your own username
-    version="0.0.4",
+    version="0.0.5",
     author="lixiang90",
     author_email="lixiang90@github.com",
     description="a python port of formal mathematics proof verifier.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lixiang90/formalmath.git",
     packages=setuptools.find_packages(),
```

