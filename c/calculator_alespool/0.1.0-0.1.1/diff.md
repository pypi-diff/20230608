# Comparing `tmp/calculator_alespool-0.1.0.tar.gz` & `tmp/calculator_alespool-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculator_alespool-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "calculator_alespool-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `calculator_alespool-0.1.0.tar` & `calculator_alespool-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      180 2023-06-05 19:42:19.997947 calculator_alespool-0.1.0/.idea/.gitignore
--rw-r--r--   0        0        0     7446 2023-06-05 19:39:59.957062 calculator_alespool-0.1.0/115.ipynb
--rw-r--r--   0        0        0     1082 2023-06-05 19:39:59.957062 calculator_alespool-0.1.0/LICENSE
--rw-r--r--   0        0        0    10636 2023-06-05 19:39:59.957062 calculator_alespool-0.1.0/calculator_alespool.py
--rw-r--r--   0        0        0      414 2023-06-05 20:00:01.665092 calculator_alespool-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2569 2023-06-05 20:00:26.226902 calculator_alespool-0.1.0/testing/test_pytest.py
--rw-r--r--   0        0        0     2284 2023-06-05 20:00:26.223902 calculator_alespool-0.1.0/testing/test_unittest.py
--rw-r--r--   0        0        0      433 2023-06-05 20:00:26.218902 calculator_alespool-0.1.0/testing/testing_root.py
--rw-r--r--   0        0        0      362 1970-01-01 00:00:00.000000 calculator_alespool-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      180 2023-06-05 19:42:19.997947 calculator_alespool-0.1.1/.idea/.gitignore
+-rw-r--r--   0        0        0     7446 2023-06-05 19:39:59.957062 calculator_alespool-0.1.1/115.ipynb
+-rw-r--r--   0        0        0     1082 2023-06-05 19:39:59.957062 calculator_alespool-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5911 2023-06-08 09:44:10.684078 calculator_alespool-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 09:23:35.215421 calculator_alespool-0.1.1/__init__.py
+-rw-r--r--   0        0        0    10967 2023-06-08 10:07:42.490453 calculator_alespool-0.1.1/calculator_alespool.py
+-rw-r--r--   0        0        0      697 2023-06-08 10:17:40.938626 calculator_alespool-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 09:24:54.616745 calculator_alespool-0.1.1/testing/__init__.py
+-rw-r--r--   0        0        0     2569 2023-06-06 11:47:24.930423 calculator_alespool-0.1.1/testing/test_pytest.py
+-rw-r--r--   0        0        0     2284 2023-06-05 20:00:26.223902 calculator_alespool-0.1.1/testing/test_unittest.py
+-rw-r--r--   0        0        0     6433 1970-01-01 00:00:00.000000 calculator_alespool-0.1.1/PKG-INFO
```

### Comparing `calculator_alespool-0.1.0/115.ipynb` & `calculator_alespool-0.1.1/115.ipynb`

 * *Files identical despite different names*

### Comparing `calculator_alespool-0.1.0/LICENSE` & `calculator_alespool-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `calculator_alespool-0.1.0/calculator_alespool.py` & `calculator_alespool-0.1.1/calculator_alespool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 'Creating a calculator that can be used to add, subtract, multiply, divide and take (n) root power'
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 from typing import Union, Iterable, Optional
 
 
 class Calculator:
     """An attempt to create a calculator."""
 
@@ -39,15 +39,14 @@
         # Test adding an integer and a float
         result = calculator.add(5, 2.5)
         assert result == -0.5
 
         # Test adding an invalid number
         with pytest.raises(ValueError):
             calculator.add('Ale')
-
         """
 
         if not isinstance(num, (int, float)):
             print("Insert only valid numbers (integers or floats).  Try again...")
             raise ValueError
 
         self.current_value += num
@@ -188,15 +187,14 @@
         calculator.reset()
         with pytest.raises(TypeError):
             calculator.divide()
 
         # Test dividing by 0
         with pytest.raises(ZeroDivisionError):
             calculator.divide(0)
-
         """
 
         if not isinstance(num, (int, float)):
             print("Insert only valid numbers (integers or floats).  Try again...")
             raise ValueError
 
         if num is None:
@@ -223,16 +221,16 @@
                     raise ValueError
 
         if self.current_value % 1 == 0:
             return int(self.current_value)
         else:
             return self.current_value
 
-    def root(self, num: Optional[Union[float, int]] = None, *args: Iterable[Union[int, float]], power: int = 2) -> \
-    Union[int, float]:
+    def root(self, num: Optional[Union[float, int]] = None, power: int = 2, *args: Iterable[Union[int, float]] ) -> \
+            Union[int, float]:
         """
         Returns the closest approximation of the root of the chosen power for the inputted number.
         The default value of the power is 2.
 
         :param power: An `int`. Determines the power of the root operation. Default value: 2 (squared root)
         :param num: Can be `int` or `float`.
         :return: A float value, representing the square power of a number within the epsilon of x
@@ -249,18 +247,25 @@
             calculator.root(-8, power=3)
 
         # Test finding the squared root of a single number
         with pytest.raises(TypeError):
             calculator.root()
         """
 
+        # Check for negative power
+        if power == 0:
+            raise ValueError("Cannot compute root of zero power.")
+        if power < 0:
+            raise ValueError("Cannot compute negative power root.")
+
+        # Not able to write code for negative numbers roots
         if num is None:
             if self.current_value < 0:
-                print("Cannot compute square root of a negative number. Try again...")
-                self.current_value = 0
+                raise ValueError("Cannot compute square root of a negative number. "
+                                 "Please use a calculator that handles complex numbers.")
 
             elif self.current_value == 0:
                 print("You can't get a root of no number.")
                 raise TypeError
 
             else:
                 self.current_value = self.current_value ** (1 / power)
@@ -287,8 +292,7 @@
 
         return self.current_value
 
     def reset(self):
         self.current_value = 0
         print("The memory of the calculator has been erased.")
         return self.current_value
-
```

### Comparing `calculator_alespool-0.1.0/testing/test_pytest.py` & `calculator_alespool-0.1.1/testing/test_pytest.py`

 * *Files identical despite different names*

### Comparing `calculator_alespool-0.1.0/testing/test_unittest.py` & `calculator_alespool-0.1.1/testing/test_unittest.py`

 * *Files identical despite different names*

