# Comparing `tmp/custom_numbers-1.1.2.tar.gz` & `tmp/custom_numbers-1.1.3.tar.gz`

## Comparing `custom_numbers-1.1.2.tar` & `custom_numbers-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/.bumpversion.cfg
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/i2.sh
--rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/inst.sh
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/mm.sh
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/pytest.ini
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/requirements.txt
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/setup_environment.sh
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/t.sh
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/uninst.sh
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/src/custom_numbers/__init__.py
--rw-r--r--   0        0        0    18322 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/src/custom_numbers/custom_numbers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/src/custom_numbers/py.typed
--rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/tests/test_customnumber.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/tests/test_customnumeralsystem.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/tests/test_geariterator.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/LICENSE
--rw-r--r--   0        0        0     8675 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/README.md
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/pyproject.toml
--rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 custom_numbers-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/.bumpversion.cfg
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/CHANGELOG.md
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/i2.sh
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/inst.sh
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/mm.sh
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/pytest.ini
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/requirements.txt
+-rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/setup_environment.sh
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/t.sh
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/uninst.sh
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/conda/meta.yaml
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/src/custom_numbers/__init__.py
+-rw-r--r--   0        0        0    16943 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/src/custom_numbers/custom_numbers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/src/custom_numbers/py.typed
+-rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/tests/test_customnumber.py
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/tests/test_customnumeralsystem.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/tests/test_geariterator.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/LICENSE
+-rw-r--r--   0        0        0     8675 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/README.md
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/PKG-INFO
```

### Comparing `custom_numbers-1.1.2/.github/ISSUE_TEMPLATE/bug_report.md` & `custom_numbers-1.1.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.2/.github/ISSUE_TEMPLATE/feature_request.md` & `custom_numbers-1.1.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.2/src/custom_numbers/custom_numbers.py` & `custom_numbers-1.1.3/src/custom_numbers/custom_numbers.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,524 +6,511 @@
 
 Project homepage and documentation:
 https://github.com/StrayFeral/custom_numbers
 """
 
 import re
 import math
-from typing import List, Generator
+from typing import List
 
-__version__: str = "1.1.2"
+__version__: str = "1.1.3"
 __author__: str = r"Evgueni Antonov (Evgueni.Antonov@gmail.com)"
 
 
 
 class CustomNumeralSystem:
     r"""Definition of custom numeral systems with basic consistency validation.
-    
+
     Args:
         digits: String of characters to be perceived as digits.
                 The character order is important: 'smallest' is the first on the left!
                 This string length would be the numeral system base.
                 Obviously each "digit" would consist of a single-
                 character.
-                
+
                 Forbidden characters: -, +, *, /, % and space
-    
+
     For the needs of basic validation, the equality and iequality Python
     operators were implemented, so you could compare two objects.
-    
+
     However the comparisson would be by the list (basically the string)
     of the characters representing the digits, rather than standard
     Python object (reference) comparisson.
-                
+
     Example:
         sys1 = CustomNumeralSystem("012ab") # Custom Base5 numeral system
         sys2 = CustomNumeralSystem("mab87")
-        
+
         # Details
         sys3 = CustomNumeralSystem("paf") # Custom Base3 numeral system
         # Example counting from the smallest possible value:
         # "p" # "p" assumes to be the analog of the zero
         # "a"
         # "f"
         # "ap"
         # "aa"
         # and so on. You get the idea.
-        
+
         # COMPARISSON
         sys1 = cn.CustomNumeralSystem("paf")
         sys2 = cn.CustomNumeralSystem("paf")
-        
+
         # The two objects are different, despite being initialized with
         # the same value
         id(sys1) == id(sys2) # False
-        
-        # However the set of characters (the digits) is the same, the 
+
+        # However the set of characters (the digits) is the same, the
         # base is the same, so I accept they are the same numeral systems
         sys1 == sys2 # True
-        
+
         # And you could also test for inequality
         sys1 = cn.CustomNumeralSystem("paf")
         sys2 = cn.CustomNumeralSystem("paz")
         sys1 != sys2 # True
     """
-    
+
     _FORBIDDENCHARACTERS: str = r"+-*/%\s"
-    
+
     
     def __init__(self, digits: str) -> None:
         self._digits: str = digits
         self._base: int = len(digits)
-        
+
         if len(digits) == 0:
             raise ValueError("Empty 'digits' argument given.")
-        
+
         digit_set = set([x for x in digits])
         if len(digits) != len(digit_set):
             raise ValueError("Duplicate characters in the 'digits' argument.")
-        
+
         # I don't think we need to put a limit here. Let the user decide.
-        #if self._base > self._MAXBASE:
+        # if self._base > self._MAXBASE:
         #    raise ValueError(f"Unsupported numeral base given {self._base}. Maximum base supported is {self._MAXBASE}.")
-        
+
     
     def __repr__(self) -> str:
         return self._digits
-    
+
     
     def __eq__(self, other) -> bool:
         """This compare both the digits and the Base."""
         return self._digits == str(other)
-    
+
     
     def __ne__(self, other) -> bool:
         """This compare both the digits and the Base."""
         return self._digits != str(other)
-    
+
     
     @property
     def forbidden_characters(self) -> str:
         return self._FORBIDDENCHARACTERS
-    
+
     
     @property
     def base(self) -> int:
         return self._base
-    
+
     
     def valid_number(self, number: str) -> bool:
         r"""Validation: Is this digit belonging to this numeral system?"""
-        
+
         if len(number) == 0:
             raise ValueError("Passed an empty string as a 'number' argument.")
-        
+
         # Test if string contains forbidden characters.
         # Generally I dislike the + string concatenation, but as an
         # f-string the regexes triggered some warnings, despite I
         # escaped them.
         regex_str = r"[" + re.escape(self._FORBIDDENCHARACTERS) + r"]"
         regex = re.compile(regex_str)
         if regex.search(number):
             return False
-        
+
         # Test if string contains any characters outside the defined set
         regex_str = r"[^" + re.escape(self._digits) + r"]"
         regex = re.compile(regex_str)
         if regex.search(number):
             return False
-        
+
         return True
-    
-    
+
+
 
 class CustomNumber:
     r"""Definition of a number from the CustomNumericalSystem.
-    
+
     Args:
         numeral_system: The custom numeral system the number is going to be from.
         number: The number as a string. Signed numbers are supported.
-        
+
     Basic math operations are supported trough standard Python operators.
-    
+
     Comparisson operators are supported as well.
-    
+
     Example:
         sysN = cn.CustomNumeralSystem("paf")
         numN1 = cn.CustomNumber(sysN, "-a") # A negative number
         numN2 = cn.CustomNumber(sysN, "a")  # A positive number
         numN3 = cn.CustomNumber(sysN, "+a") # A positive number
     """
-    
+
     _POSITIVE: str = r"+"
     _NEGATIVE: str = r"-"
+
     
     def __init__(self, numeral_system: CustomNumeralSystem, number: str) -> None:
         self._numeral_system: CustomNumeralSystem = numeral_system
-        self._init_value: str = number # Just in case we will keep the original value
+        self._init_value: str = number  # Just in case we will keep the original value
         self._value: str = number
-        
-        self.absolute() # This will set the sign as well
-        
+
+        self.absolute()  # This will set the sign as well
+
         if not numeral_system.valid_number(self._value):
             raise ValueError("Invalid characters in number, which are not in the chosen numeral system.")
-        
+
     
     def __repr__(self) -> str:
         if self._sign == self._NEGATIVE:
             return f"-{self._value}"
         return self._value
-    
+
     
     @property
     def numeral_system(self) -> CustomNumeralSystem:
         return self._numeral_system
-    
+
     
     @property
     def init_value(self) -> str:
         r"""Return the value the class was initialized with, as it was originally passed to the class."""
         return self._init_value
-    
+
     
     def __eq__(self, other) -> bool:
         if self.numeral_system != other.numeral_system:
             raise ValueError("Numbers must be from the same numeral system.")
         return self.to_decimal() == other.to_decimal()
-    
+
     
     def __ne__(self, other) -> bool:
         if self.numeral_system != other.numeral_system:
             raise ValueError("Numbers must be from the same numeral system.")
         return self.to_decimal() != other.to_decimal()
-    
+
     
     def __ge__(self, other) -> bool:
         if self.numeral_system != other.numeral_system:
             raise ValueError("Numbers must be from the same numeral system.")
         return self.to_decimal() >= other.to_decimal()
-    
+
     
     def __gt__(self, other) -> bool:
         if self.numeral_system != other.numeral_system:
             raise ValueError("Numbers must be from the same numeral system.")
         return self.to_decimal() > other.to_decimal()
-    
+
     
     def __lt__(self, other) -> bool:
         if self.numeral_system != other.numeral_system:
             raise ValueError("Numbers must be from the same numeral system.")
         return self.to_decimal() < other.to_decimal()
-    
+
     
     def __le__(self, other) -> bool:
         if self.numeral_system != other.numeral_system:
             raise ValueError("Numbers must be from the same numeral system.")
         return self.to_decimal() <= other.to_decimal()
-    
+
     
     def __add__(self, other) -> object:
         if self.numeral_system != other.numeral_system:
             raise ValueError("Numbers must be from the same numeral system.")
         result: int = self.to_decimal() + other.to_decimal()
-        num: CustomNumber = CustomNumber(self.numeral_system, str(self.numeral_system)[0]) # Dummy init_value
+        num: CustomNumber = CustomNumber(self.numeral_system, str(self.numeral_system)[0])  # Dummy init_value
         num.from_decimal(result)
         return num
-    
+
     
     def __sub__(self, other) -> object:
         if self.numeral_system != other.numeral_system:
             raise ValueError("Numbers must be from the same numeral system.")
         result: int = self.to_decimal() - other.to_decimal()
-        num: CustomNumber = CustomNumber(self.numeral_system, str(self.numeral_system)[0]) # Dummy init_value
+        num: CustomNumber = CustomNumber(self.numeral_system, str(self.numeral_system)[0])  # Dummy init_value
         num.from_decimal(result)
         return num
-    
+
     
     def __mul__(self, other) -> object:
         if self.numeral_system != other.numeral_system:
             raise ValueError("Numbers must be from the same numeral system.")
         result: int = self.to_decimal() * other.to_decimal()
-        num: CustomNumber = CustomNumber(self.numeral_system, str(self.numeral_system)[0]) # Dummy init_value
+        num: CustomNumber = CustomNumber(self.numeral_system, str(self.numeral_system)[0])  # Dummy init_value
         num.from_decimal(result)
         return num
-    
+
     
     def __floordiv__(self, other) -> object:
         if self.numeral_system != other.numeral_system:
             raise ValueError("Numbers must be from the same numeral system.")
         result: int = self.to_decimal() // other.to_decimal()
-        num: CustomNumber = CustomNumber(self.numeral_system, str(self.numeral_system)[0]) # Dummy init_value
+        num: CustomNumber = CustomNumber(self.numeral_system, str(self.numeral_system)[0])  # Dummy init_value
         num.from_decimal(result)
         return num
-    
+
     
     def __truediv__(self, other) -> object:
         return self.__floordiv__(other)
-    
+
     
     def __div__(self, other) -> object:
         return self.__floordiv__(other)
-    
+
     
     def __pow__(self, other) -> object:
         if self.numeral_system != other.numeral_system:
             raise ValueError("Numbers must be from the same numeral system.")
         result: int = self.to_decimal() ** other.to_decimal()
-        num: CustomNumber = CustomNumber(self.numeral_system, str(self.numeral_system)[0]) # Dummy init_value
+        num: CustomNumber = CustomNumber(self.numeral_system, str(self.numeral_system)[0])  # Dummy init_value
         num.from_decimal(result)
         return num
-    
+
     
     def __mod__(self, other) -> object:
         if self.numeral_system != other.numeral_system:
             raise ValueError("Numbers must be from the same numeral system.")
         result: int = self.to_decimal() % other.to_decimal()
-        num: CustomNumber = CustomNumber(self.numeral_system, str(self.numeral_system)[0]) # Dummy init_value
+        num: CustomNumber = CustomNumber(self.numeral_system, str(self.numeral_system)[0])  # Dummy init_value
         num.from_decimal(result)
         return num
-        
+
     
     def absolute(self, number: str = "") -> str:
         """Returns the absolute value."""
-        
+
         num: str = number
         if len(number) == 0:
             num = self._value
-        
+
         sign: str = self._POSITIVE
         if num[0] == self._NEGATIVE:
             sign = self._NEGATIVE
-        
+
         if num[0] == self._POSITIVE or num[0] == self._NEGATIVE:
-            num = num[1:] # Strip sign
-        
+            num = num[1:]  # Strip sign
+
         if len(number) == 0:
             self._value = num
             self._sign = sign
-        
+
         return num
-    
+
     
     def digit_to_int(self, digit: str) -> int:
         r"""Fastest and simplest possible conversion. Left-most one is the zero."""
-        
+
         if len(digit) != 1:
             raise ValueError("Invalid digit. Must be one character.")
         return str(self._numeral_system).index(digit)
-    
+
     
     def int_to_digit(self, i: int) -> str:
         return str(self.numeral_system)[i]
-    
+
     
     def to_decimal(self) -> int:
         r"""Converts a number of a custom numeral system to a decimal integer."""
-        
+
         power = 0
         int_value = 0
-        
+
         for digit in self._value[::-1]:
-            int_value += self.digit_to_int(digit) * (self._numeral_system.base ** power)
+            int_value += self.digit_to_int(digit) * (self._numeral_system.base**power)
             power += 1
-        
+
         if self._sign == self._NEGATIVE:
             int_value = -abs(int_value)
-        
+
         return int_value
-    
+
     
     def from_decimal(self, number: int) -> None:
         r"""Converts the number to the current numeral system and sets the internal value to it."""
-        
+
         sign: str = self._POSITIVE
         if number < 0:
             sign = self._NEGATIVE
         self._sign = sign
-        
+
         value: str = ""
         num = float(abs(number))
         while int(num) > 0:
             num = num / self.numeral_system.base
             remainder, integr = math.modf(num)
             remainder *= self.numeral_system.base
             value = f"{self.int_to_digit(int(remainder))}{value}"
-        
+
         if number == 0:
             value = f"{self.int_to_digit(0)}"
-        
+
         self._value = value
-        
-        
+
+
 
 class GearIterator:
     r"""GearIterator.
-    
+
     Briefly simulates old gear counters, like the old cars odometer.
-    
+
     The class is serializable, works with both pickle and dill.
     The class implements the context management protocol.
-    
+
     Args:
         numeral_system: Custom numeral system. Mind the order of symbols!
         min_length: Minimum length, default is zero
         max_length: Maximum length, default is zero - means no limit
         init_value: Value to initialize with
-    
+
     Returns:
         str
     """
+
     
     def __init__(self, numeral_system: CustomNumeralSystem, min_length: int = 0, max_length: int = 0, init_value: str = "") -> None:
         self._numeral_system: CustomNumeralSystem = numeral_system
         self._symbol_list: List[str] = [x for x in str(numeral_system)]
         self._min_length: int = min_length
         self._max_length: int = max_length
         self._init_value: str = init_value
         self._init_value_returned: bool = False
         self._index: int = 0
         self._combinations: int = 0
-        
+
         # Basic validation ...
         if max_length > 0 and min_length > max_length:
             raise ValueError("min_length is greather than max_length.")
-        
+
         if len(init_value) > 0:
             if len(init_value) < min_length or (max_length > 0 and len(init_value) > max_length):
                 raise ValueError("Incorrect init_value length.")
-            
+
             if not numeral_system.valid_number(init_value):
                 raise ValueError("Invalid characters in init_value, which are not in the chosen numeral system.")
-            
+
             if init_value == str(numeral_system)[0] * len(init_value):
                 raise ValueError("Init_value contains only smallest digits (zero-equivalents).")
-        
+
             # Strip the leading "zeroes"
             while init_value[0] == str(numeral_system)[0]:
                 init_value = init_value[1:]
-        
-            self._init_value = init_value[::-1] # Reverse the string
-        
+
+            self._init_value = init_value[::-1]  # Reverse the string
+
         min_len: int = min_length
         if min_len == 0:
             min_len = 1
-        
+
         self._gears: List[list] = []
-        
+
         # Initialization with init_value
         for symbol in self._init_value:
             seq = self._symbol_list.copy()
-            
+
             while seq[0] != symbol:
                 seq.pop(0)
-            
+
             self._gears.append(seq)
-        
+
         # Additional initialization until min_length is reached
         for i in range(len(self._gears), min_len):
             seq = self._symbol_list.copy()
-            
+
             if len(self._init_value) > 0 and i < len(self._init_value):
                 symbol = self._init_value[i]
                 while seq[0] != symbol:
                     seq.pop(0)
-            
+
             self._gears.append(seq)
-    
+
     
     @property
     def combinations(self) -> int:
         """Combinations calculation.
-        
+
         People may argue with me here, but in a set of only two values,
         like {0, 1}, if we make two gears out of these and rotate them,
         the values would be:
         # 0
         # 1
         # 10
         # 11
         And while for mathematicians "01" == "10", for me they are not
         the same.
         """
-        
+
         if self._combinations == 0:
-            ## C(n, r) = (n + r - 1)! / (r!(n - 1)!)
             n: int = len(self._symbol_list)
             r: int = self._max_length
-            #c: int = math.factorial(n + r - 1) // math.factorial(r) * math.factorial(n - 1)
             c: int = n * r
-            
+
             self._combinations = c
-        
+
         return self._combinations
-        
+
     
     def __repr__(self) -> str:
         result: str = ""
         for gear in self._gears:
             result += gear[0]
-        return result[::-1] # Reverse the string
-    
+        return result[::-1]  # Reverse the string
+
     
     def __iter__(self) -> object:
         return self
-        
+
     
     # l = list(generator) # internally call next() until exhaustion
     def __next__(self) -> str:
         if not self._init_value_returned:
             self._init_value_returned = True
             return repr(self)
-        
+
         spin_wheels: bool = True
         i = 0
         while spin_wheels:
             self._gears[i].pop(0)
-            
+
             # Reset gear
             if len(self._gears[i]) == 0:
                 self._gears[i] = self._symbol_list.copy()
                 i += 1
-                
+
                 # Add a new gear
                 if i == len(self._gears) and i < self._max_length:
                     self._gears.append(self._symbol_list.copy())
-                    self._gears[i].pop(0) # Remove the "zero"
+                    self._gears[i].pop(0)  # Remove the "zero"
                     spin_wheels = False
-                
+
                 if i == self._max_length:
                     raise StopIteration
-            else: # Wheel not yet reached the final set value
+            else:  # Wheel not yet reached the final set value
                 spin_wheels = False
-        
+
         return repr(self)
-    
+
     
     def __enter__(self) -> object:
         r"""Context management protocol.
-        
+
         Not sure we would need this, but it's there.
         """
         return self
-    
+
     
     def __exit__(self, exc_type: object, exc_value: object, exc_tb: object) -> bool:
         r"""Context management protocol.
-        
+
         StopIteration exception will not be propagated.
-        
+
         Not sure we would need this, but it's there.
         """
-        return True # We won't propagate the StopIteration exception
-
-
-
-#class GearGenerator:
-#    r"""The GearIterator in a generator form.
-#    
-#    I wrote this class as part of an exercise. Not sure if anyone would need it,
-#    but would leave it here.
-#    """
-#    
-#    def generate(self, numeral_system: CustomNumeralSystem, min_length: int = 0, max_length: int = 0, init_value: str = "") -> Generator[str, None, None]:
-#        for gear_value in GearIterator(numeral_system, min_length, max_length, init_value):
-#            yield gear_value
+        return True  # We won't propagate the StopIteration exception
```

### Comparing `custom_numbers-1.1.2/tests/test_customnumber.py` & `custom_numbers-1.1.3/tests/test_customnumber.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,330 +1,332 @@
 import pytest
 from custom_numbers import custom_numbers as cn
 
 
-class TestCustomNumber():
+
+class TestCustomNumber:
     r"""CustomNumber test class."""
+
     
     def test_invalid_number(self):
         sysN = cn.CustomNumeralSystem("paf")
         with pytest.raises(Exception):
-            num = cn.CustomNumber(sysN, "x") # Invalid
-    
+            num = cn.CustomNumber(sysN, "x")  # Invalid
+
     
     def test_repr(self):
         expected = "1100101"
         sysN = cn.CustomNumeralSystem("01")
         num = cn.CustomNumber(sysN, "1100101")
         result = str(num)
         assert result == expected
-    
+
     
     def test_init_value(self):
         expected = "1100101"
         sysN = cn.CustomNumeralSystem("01")
         num = cn.CustomNumber(sysN, "1100101")
         result = str(num.init_value)
         assert result == expected
-    
+
     
     def test_digit_to_int(self):
         expected = 1
-        sysN = cn.CustomNumeralSystem("paf") # 0 1 2
+        sysN = cn.CustomNumeralSystem("paf")  # 0 1 2
         num = cn.CustomNumber(sysN, "aaa")
         result = num.digit_to_int("a")
         assert result == expected
-    
+
     
     def test_digit_to_int_hex(self):
         """Just in case"""
-        
+
         expected = 15
-        sysN = cn.CustomNumeralSystem("0123456789abcdef") # Common hex system
+        sysN = cn.CustomNumeralSystem("0123456789abcdef")  # Common hex system
         num = cn.CustomNumber(sysN, "aaa")
         result = num.digit_to_int("f")
         assert result == expected
-    
+
     
     def test_digit_to_int_negative_more_characters(self):
-        sysN = cn.CustomNumeralSystem("paf") # 0 1 2
+        sysN = cn.CustomNumeralSystem("paf")  # 0 1 2
         num = cn.CustomNumber(sysN, "aaa")
         with pytest.raises(Exception):
             result = num.digit_to_int("aa")
-    
+
     
     def test_digit_to_int_negative_empty(self):
-        sysN = cn.CustomNumeralSystem("paf") # 0 1 2
+        sysN = cn.CustomNumeralSystem("paf")  # 0 1 2
         num = cn.CustomNumber(sysN, "aaa")
         with pytest.raises(Exception):
             result = num.digit_to_int("")
-    
+
     
     def test_hex_to_decimal(self):
         expected = 240
-        sysN = cn.CustomNumeralSystem("0123456789abcdef") # Common hex system
+        sysN = cn.CustomNumeralSystem("0123456789abcdef")  # Common hex system
         num = cn.CustomNumber(sysN, "f0")
         result = num.to_decimal()
         assert result == expected
-    
+
     
     def test_bin_to_decimal(self):
         expected = 101
-        sysN = cn.CustomNumeralSystem("01") # Common bin system
+        sysN = cn.CustomNumeralSystem("01")  # Common bin system
         num = cn.CustomNumber(sysN, "1100101")
         result = num.to_decimal()
         assert result == expected
-    
+
     
     def test_ternary_to_decimal(self):
         expected = 4
         sysN = cn.CustomNumeralSystem("paf")
         num = cn.CustomNumber(sysN, "aa")
         result = num.to_decimal()
         assert result == expected
-    
+
     
     def test_full_equality(self):
         expected = True
         sysN1 = cn.CustomNumeralSystem("paf")
         numN1 = cn.CustomNumber(sysN1, "aa")
         sysN2 = cn.CustomNumeralSystem("paf")
         numN2 = cn.CustomNumber(sysN2, "aa")
-        result = (numN1 == numN2)
+        result = numN1 == numN2
         assert result == expected
-    
+
     
     def test_equality_different_numbers(self):
         expected = False
         sysN1 = cn.CustomNumeralSystem("paf")
         numN1 = cn.CustomNumber(sysN1, "aa")
         sysN2 = cn.CustomNumeralSystem("paf")
         numN2 = cn.CustomNumber(sysN2, "aaa")
-        result = (numN1 == numN2)
+        result = numN1 == numN2
         assert result == expected
-    
+
     
     def test_equality_different_systems(self):
-        expected = False
         sysN1 = cn.CustomNumeralSystem("paf")
         numN1 = cn.CustomNumber(sysN1, "aa")
         sysN2 = cn.CustomNumeralSystem("paft")
         numN2 = cn.CustomNumber(sysN2, "aa")
         with pytest.raises(Exception):
-            result = (numN1 == numN2)
-    
+            result = numN1 == numN2
+
     
     def test_inequality(self):
         expected = True
         sysN1 = cn.CustomNumeralSystem("paf")
         numN1 = cn.CustomNumber(sysN1, "aa")
         sysN2 = cn.CustomNumeralSystem("paf")
         numN2 = cn.CustomNumber(sysN2, "a")
-        result = (numN1 != numN2)
+        result = numN1 != numN2
         assert result == expected
-    
+
     
     def test_gt(self):
         expected = True
         sysN1 = cn.CustomNumeralSystem("paf")
         numN1 = cn.CustomNumber(sysN1, "f")
         sysN2 = cn.CustomNumeralSystem("paf")
         numN2 = cn.CustomNumber(sysN2, "a")
-        result = (numN1 > numN2)
+        result = numN1 > numN2
         assert result == expected
-    
+
     
     def test_ge(self):
         expected = True
         sysN1 = cn.CustomNumeralSystem("paf")
         numN1 = cn.CustomNumber(sysN1, "f")
         sysN2 = cn.CustomNumeralSystem("paf")
         numN2 = cn.CustomNumber(sysN2, "p")
-        result = (numN1 >= numN2)
+        result = numN1 >= numN2
         assert result == expected
-    
+
     
     def test_lt(self):
         expected = True
         sysN1 = cn.CustomNumeralSystem("paf")
         numN1 = cn.CustomNumber(sysN1, "p")
         sysN2 = cn.CustomNumeralSystem("paf")
         numN2 = cn.CustomNumber(sysN2, "a")
-        result = (numN1 < numN2)
+        result = numN1 < numN2
         assert result == expected
-    
+
     
     def test_le(self):
         expected = True
         sysN1 = cn.CustomNumeralSystem("paf")
         numN1 = cn.CustomNumber(sysN1, "p")
         sysN2 = cn.CustomNumeralSystem("paf")
         numN2 = cn.CustomNumber(sysN2, "a")
-        result = (numN1 <= numN2)
+        result = numN1 <= numN2
         assert result == expected
-    
+
     
     def test_addition(self):
         expected = "a"
-        sysN1 = cn.CustomNumeralSystem("paf") # 0 1 2
+        sysN1 = cn.CustomNumeralSystem("paf")  # 0 1 2
         numN1 = cn.CustomNumber(sysN1, "p")
         sysN2 = cn.CustomNumeralSystem("paf")
         numN2 = cn.CustomNumber(sysN2, "a")
         result = numN1 + numN2
         assert str(result) == expected
-    
+
     
     def test_subtraction(self):
         expected = "a"
-        sysN1 = cn.CustomNumeralSystem("paf") # 0 1 2
+        sysN1 = cn.CustomNumeralSystem("paf")  # 0 1 2
         numN1 = cn.CustomNumber(sysN1, "f")
         sysN2 = cn.CustomNumeralSystem("paf")
         numN2 = cn.CustomNumber(sysN2, "a")
         result = numN1 - numN2
         assert str(result) == expected
-    
+
     
     def test_augmented_addition(self):
         expected1 = "f"
         expected2 = "a"
-        sysN1 = cn.CustomNumeralSystem("paf") # 0 1 2
+        sysN1 = cn.CustomNumeralSystem("paf")  # 0 1 2
         numN1 = cn.CustomNumber(sysN1, "a")
         sysN2 = cn.CustomNumeralSystem("paf")
         numN2 = cn.CustomNumber(sysN2, "a")
         numN1 += numN2
         assert str(numN1) == expected1
         assert str(numN2) == expected2
-    
+
     
     def test_augmented_subtraction(self):
         expected1 = "p"
         expected2 = "a"
-        sysN1 = cn.CustomNumeralSystem("paf") # 0 1 2
+        sysN1 = cn.CustomNumeralSystem("paf")  # 0 1 2
         numN1 = cn.CustomNumber(sysN1, "a")
         sysN2 = cn.CustomNumeralSystem("paf")
         numN2 = cn.CustomNumber(sysN2, "a")
         numN1 -= numN2
         assert str(numN1) == expected1
         assert str(numN2) == expected2
-    
+
     
     def test_int_to_digit(self):
         expected = "a"
-        sysN = cn.CustomNumeralSystem("paf") # 0 1 2
+        sysN = cn.CustomNumeralSystem("paf")  # 0 1 2
         num = cn.CustomNumber(sysN, "aaa")
         result = num.int_to_digit(1)
         assert result == expected
-    
+
     
     def test_decimal_to_hex(self):
         expected = "1df"
-        sysN = cn.CustomNumeralSystem("0123456789abcdef") # Common hex system
-        num = cn.CustomNumber(sysN, "f0") # The value is irrelevant here, we just want to instantiate
+        sysN = cn.CustomNumeralSystem("0123456789abcdef")  # Common hex system
+        num = cn.CustomNumber(sysN, "f0")  # The value is irrelevant here, we just want to instantiate
         num.from_decimal(479)
         result = str(num)
         assert result == expected
-        
+
     
     def test_subtraction_negative_number_result(self):
-        expected = "-a" # -1
-        sysN1 = cn.CustomNumeralSystem("paf") # 0 1 2
+        expected = "-a"  # -1
+        sysN1 = cn.CustomNumeralSystem("paf")  # 0 1 2
         numN1 = cn.CustomNumber(sysN1, "a")
         numN2 = cn.CustomNumber(sysN1, "f")
         result = numN1 - numN2
         assert str(result) == expected
-    
+
     
     def test_absolute_value_positive_signed(self):
         expected = "a"
-        sysN = cn.CustomNumeralSystem("paf") # 0 1 2
+        sysN = cn.CustomNumeralSystem("paf")  # 0 1 2
         num = cn.CustomNumber(sysN, "+a")
         result = num.absolute()
         assert str(result) == expected
-    
+
     
     def test_absolute_value_negative_number(self):
         expected = "a"
-        sysN = cn.CustomNumeralSystem("paf") # 0 1 2
+        sysN = cn.CustomNumeralSystem("paf")  # 0 1 2
         num = cn.CustomNumber(sysN, "-a")
         result = num.absolute()
         assert str(result) == expected
-    
+
     
     def test_negative_number_subtraction1(self):
-        expected = "p" # 0
-        sysN1 = cn.CustomNumeralSystem("paf") # 0 1 2
+        expected = "p"  # 0
+        sysN1 = cn.CustomNumeralSystem("paf")  # 0 1 2
         numN1 = cn.CustomNumber(sysN1, "-a")
         numN2 = cn.CustomNumber(sysN1, "-a")
         result = numN1 - numN2
         assert str(result) == expected
-    
+
     
     def test_negative_number_subtraction2(self):
-        expected = "-f" # -2
-        sysN1 = cn.CustomNumeralSystem("paf") # 0 1 2
+        expected = "-f"  # -2
+        sysN1 = cn.CustomNumeralSystem("paf")  # 0 1 2
         numN1 = cn.CustomNumber(sysN1, "-a")
         numN2 = cn.CustomNumber(sysN1, "a")
         result = numN1 - numN2
         assert str(result) == expected
-    
+
     
     def test_negative_number_addition1(self):
-        expected = "-f" # -2
-        sysN1 = cn.CustomNumeralSystem("paf") # 0 1 2
+        expected = "-f"  # -2
+        sysN1 = cn.CustomNumeralSystem("paf")  # 0 1 2
         numN1 = cn.CustomNumber(sysN1, "-a")
         numN2 = cn.CustomNumber(sysN1, "-a")
         result = numN1 + numN2
         assert str(result) == expected
-    
+
     
     def test_negative_number_addition2(self):
-        expected = "-a" # -1
-        sysN1 = cn.CustomNumeralSystem("paf") # 0 1 2
+        expected = "-a"  # -1
+        sysN1 = cn.CustomNumeralSystem("paf")  # 0 1 2
         numN1 = cn.CustomNumber(sysN1, "-f")
         numN2 = cn.CustomNumber(sysN1, "a")
         result = numN1 + numN2
         assert str(result) == expected
-    
+
     
     def test_multiplication(self):
         expected = "25"
-        sysN1 = cn.CustomNumeralSystem("0123456789") # Common decimal system
+        sysN1 = cn.CustomNumeralSystem("0123456789")  # Common decimal system
         numN1 = cn.CustomNumber(sysN1, "5")
         numN2 = cn.CustomNumber(sysN1, "5")
         result = numN1 * numN2
         assert str(result) == expected
-    
+
     
     def test_division(self):
         expected = "1"
-        sysN1 = cn.CustomNumeralSystem("0123456789") # Common decimal system
+        sysN1 = cn.CustomNumeralSystem("0123456789")  # Common decimal system
         numN1 = cn.CustomNumber(sysN1, "5")
         numN2 = cn.CustomNumber(sysN1, "5")
         result = numN1 / numN2
         assert str(result) == expected
-    
+
     
     def test_power(self):
         expected = "25"
-        sysN1 = cn.CustomNumeralSystem("0123456789") # Common decimal system
+        sysN1 = cn.CustomNumeralSystem("0123456789")  # Common decimal system
         numN1 = cn.CustomNumber(sysN1, "5")
         numN2 = cn.CustomNumber(sysN1, "2")
-        result = numN1 ** numN2
+        result = numN1**numN2
         assert str(result) == expected
-    
+
     
     def test_modulo1(self):
         expected = "1"
-        sysN1 = cn.CustomNumeralSystem("0123456789") # Common decimal system
+        sysN1 = cn.CustomNumeralSystem("0123456789")  # Common decimal system
         numN1 = cn.CustomNumber(sysN1, "5")
         numN2 = cn.CustomNumber(sysN1, "2")
         result = numN1 % numN2
         assert str(result) == expected
-    
+
     
     def test_modulo2(self):
         expected = "0"
-        sysN1 = cn.CustomNumeralSystem("0123456789") # Common decimal system
+        sysN1 = cn.CustomNumeralSystem("0123456789")  # Common decimal system
         numN1 = cn.CustomNumber(sysN1, "5")
         numN2 = cn.CustomNumber(sysN1, "5")
         result = numN1 % numN2
         assert str(result) == expected
+
```

### Comparing `custom_numbers-1.1.2/tests/test_customnumeralsystem.py` & `custom_numbers-1.1.3/tests/test_customnumeralsystem.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,75 @@
 import pytest
 from custom_numbers import custom_numbers as cn
 
 
-class TestCustomNumeralSystem():
+class TestCustomNumeralSystem:
     r"""CustomNumeralSystem test class."""
+
     
     def test_empty_argument(self):
         with pytest.raises(Exception):
             sysN = cn.CustomNumeralSystem("")
-    
+
     
     def test_duplicates_in_argument(self):
         with pytest.raises(Exception):
             sysN = cn.CustomNumeralSystem("abcc")
-    
+
     
     def test_repr(self):
         expected = "012"
         sysN = cn.CustomNumeralSystem("012")
         result = str(sysN)
         assert result == expected
-    
+
     
     def test_base(self):
         expected = 3
-        sysN = cn.CustomNumeralSystem("012") # Base 3
+        sysN = cn.CustomNumeralSystem("012")  # Base 3
         result = sysN.base
         assert result == expected
-    
+
     
     def test_number_validation(self):
         expected = True
         sysN = cn.CustomNumeralSystem("paf")
-        result = sysN.valid_number("ff") # Valid
+        result = sysN.valid_number("ff")  # Valid
         assert result == expected
-    
+
     
     def test_number_validation_negative(self):
         expected = False
         sysN = cn.CustomNumeralSystem("paf")
-        result = sysN.valid_number("xx") # Invalid
+        result = sysN.valid_number("xx")  # Invalid
         assert result == expected
-    
+
     
     def test_number_validation_negative_empty_string(self):
         sysN = cn.CustomNumeralSystem("paf")
         with pytest.raises(Exception):
-            result = sysN.valid_number("") # Invalid
-    
+            result = sysN.valid_number("")  # Invalid
+
     
     def test_equality(self):
         expected = True
         sysN1 = cn.CustomNumeralSystem("paf")
         sysN2 = cn.CustomNumeralSystem("paf")
-        result = (sysN1 == sysN2)
+        result = sysN1 == sysN2
         assert result == expected
-    
+
     
     def test_equality_negative(self):
         expected = False
         sysN1 = cn.CustomNumeralSystem("paf")
         sysN2 = cn.CustomNumeralSystem("pa")
-        result = (sysN1 == sysN2)
+        result = sysN1 == sysN2
         assert result == expected
-    
+
     
     def test_inequality(self):
         expected = True
         sysN1 = cn.CustomNumeralSystem("paf")
         sysN2 = cn.CustomNumeralSystem("pa")
-        result = (sysN1 != sysN2)
+        result = sysN1 != sysN2
         assert result == expected
+
```

### Comparing `custom_numbers-1.1.2/tests/test_geariterator.py` & `custom_numbers-1.1.3/tests/test_geariterator.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from custom_numbers import custom_numbers as cn
 
 
 # Common parameter
 sys3 = cn.CustomNumeralSystem("pba")
 
 # Scenario 0) Invalid parameters exception test
-#params0_1 = [cn.CustomNumeralSystem(""), 0, 2]              # Empty set
-params0_2 = [sys3, 3, 2]            # min_length > max_length
-params0_3 = [sys3, 5, 10, "ppp"]    # len(init_value) < min_length
-params0_4 = [sys3, 5, 10, "ppppppppppppppp"] # len(init_value) > max_length
-params0_5 = [sys3, 3, 10, "pbz"]    # Invalid symbol in init_value
+# params0_1 = [cn.CustomNumeralSystem(""), 0, 2]              # Empty set
+params0_2 = [sys3, 3, 2]  # min_length > max_length
+params0_3 = [sys3, 5, 10, "ppp"]  # len(init_value) < min_length
+params0_4 = [sys3, 5, 10, "ppppppppppppppp"]  # len(init_value) > max_length
+params0_5 = [sys3, 3, 10, "pbz"]  # Invalid symbol in init_value
 
 # Scenario 1) no init_value, max_length=2, full test
 params1 = [sys3, 0, 2, ""]
 expected1 = [
     ("p"),
     ("b"),
     ("a"),
@@ -36,94 +36,85 @@
     ("aa"),
     ("bpp"),
     ("bpb"),
 ]
 
 
 
-class TestGearIterator():
+class TestGearIterator:
     r"""GearIterator test class."""
+
     
     @classmethod
     def setup_class(cls):
         cls.scenario1 = cn.GearIterator(*params1)
         cls.scenario2 = cn.GearIterator(*params2)
-    
-    
-    ## Test no longer needed
-    #def test_scenario0_1(self):
-    #    with pytest.raises(Exception):
-    #        i = cn.GearIterator(*params0_1)
-    
+
     
     def test_scenario0_2(self):
         with pytest.raises(Exception):
             i = cn.GearIterator(*params0_2)
-    
+
     
     def test_scenario0_3(self):
         with pytest.raises(Exception):
             i = cn.GearIterator(*params0_3)
-    
+
     
     def test_scenario0_4(self):
         with pytest.raises(Exception):
             i = cn.GearIterator(*params0_4)
-    
+
     
     def test_scenario0_5(self):
         with pytest.raises(Exception):
             i = cn.GearIterator(*params0_5)
-    
+
     
     @pytest.mark.parametrize("expected", expected1)
     def test_scenario1(self, expected):
         result = self.scenario1
         assert next(result) == expected
-    
+
     
     def test_scenario1_expected_exception(self):
         result = self.scenario1
         with pytest.raises(StopIteration):
             assert next(result)
-    
+
     
     @pytest.mark.parametrize("expected", expected2)
     def test_scenario2(self, expected):
         result = self.scenario2
         assert next(result) == expected
-    
+
     
     def test_scenario3(self):
         """Testing serialization"""
-        
+
         our_iterator = self.scenario2
         assert next(our_iterator) == "bpa"
         serialized = pickle.dumps(our_iterator)
         print("\n-----")
-        print("Serialized length: {0}".format(len(serialized))) # 302
-        print("Serialized size: {0}".format(sys.getsizeof(serialized))) # 335
-        
+        print("Serialized length: {0}".format(len(serialized)))  # 302
+        print("Serialized size: {0}".format(sys.getsizeof(serialized)))  # 335
+
         assert next(our_iterator) == "bbp"
         assert next(our_iterator) == "bbb"
-        
+
         our_iterator = pickle.loads(serialized)
         assert next(our_iterator) == "bbp"
-    
-    
-    #def test_scenario4_thread_safe(self):
-    #    """Testing thread safe"""
-    #    pass
-    
+
     
     def test_combinations_calculation(self):
         expected = 4
         sysN = cn.CustomNumeralSystem("01")
         it = cn.GearIterator(sysN, 0, 2)
         result = it.combinations
         assert result == expected
-    
+
     
     @classmethod
     def teardown_class(cls):
         del cls.scenario1
         del cls.scenario2
+
```

### Comparing `custom_numbers-1.1.2/.gitignore` & `custom_numbers-1.1.3/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -154,7 +154,11 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+# EVG: My backups
+old_builds/
+
```

### Comparing `custom_numbers-1.1.2/LICENSE` & `custom_numbers-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.2/README.md` & `custom_numbers-1.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# custom_numbers 1.1.2
+# custom_numbers 1.1.3
 
 ## DESCRIPTION
 
 A Swiss-army knife for numbers of custom numeral systems.
 
 ## AUTHOR
```

### Comparing `custom_numbers-1.1.2/pyproject.toml` & `custom_numbers-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "custom_numbers"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
     { name = "Evgueni Antonov", email = "Evgueni.Antonov@gmail.com" },
 ]
 description = "Swiss-army knife for numbers of custom numeral systems."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `custom_numbers-1.1.2/PKG-INFO` & `custom_numbers-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom_numbers
-Version: 1.1.2
+Version: 1.1.3
 Summary: Swiss-army knife for numbers of custom numeral systems.
 Project-URL: Homepage, https://github.com/StrayFeral/custom_numbers
 Project-URL: Bug Tracker, https://github.com/StrayFeral/custom_numbers/issues
 Author-email: Evgueni Antonov <Evgueni.Antonov@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Evgueni Antonov
@@ -32,15 +32,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# custom_numbers 1.1.2
+# custom_numbers 1.1.3
 
 ## DESCRIPTION
 
 A Swiss-army knife for numbers of custom numeral systems.
 
 ## AUTHOR
```

