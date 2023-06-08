# Comparing `tmp/formalmath-0.0.7.tar.gz` & `tmp/formalmath-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formalmath-0.0.7.tar", last modified: Thu Jun  8 02:48:46 2023, max compression
+gzip compressed data, was "formalmath-0.0.8.tar", last modified: Thu Jun  8 19:45:07 2023, max compression
```

## Comparing `formalmath-0.0.7.tar` & `formalmath-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 02:48:46.458856 formalmath-0.0.7/
--rw-rw-rw-   0        0        0     2753 2023-06-08 02:48:46.457857 formalmath-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2307 2023-06-08 02:47:47.000000 formalmath-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 02:48:46.454857 formalmath-0.0.7/formalmath/
--rw-rw-rw-   0        0        0       19 2023-06-06 03:06:28.000000 formalmath-0.0.7/formalmath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:48:46.457857 formalmath-0.0.7/formalmath/setmm/
--rw-rw-rw-   0        0        0       28 2023-06-06 03:07:05.000000 formalmath-0.0.7/formalmath/setmm/__init__.py
--rw-rw-rw-   0        0        0    13037 2023-06-08 02:44:40.000000 formalmath-0.0.7/formalmath/setmm/basic_classes.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:48:46.456857 formalmath-0.0.7/formalmath.egg-info/
--rw-rw-rw-   0        0        0     2753 2023-06-08 02:48:46.000000 formalmath-0.0.7/formalmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-06-08 02:48:46.000000 formalmath-0.0.7/formalmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 02:48:46.000000 formalmath-0.0.7/formalmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-08 02:48:46.000000 formalmath-0.0.7/formalmath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 02:48:46.458856 formalmath-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      743 2023-06-08 02:48:17.000000 formalmath-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:45:07.181896 formalmath-0.0.8/
+-rw-rw-rw-   0        0        0     3278 2023-06-08 19:45:07.181896 formalmath-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2832 2023-06-08 19:42:24.000000 formalmath-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 19:45:07.179896 formalmath-0.0.8/formalmath/
+-rw-rw-rw-   0        0        0       19 2023-06-06 03:06:28.000000 formalmath-0.0.8/formalmath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:45:07.181896 formalmath-0.0.8/formalmath/setmm/
+-rw-rw-rw-   0        0        0       28 2023-06-06 03:07:05.000000 formalmath-0.0.8/formalmath/setmm/__init__.py
+-rw-rw-rw-   0        0        0    18579 2023-06-08 19:34:27.000000 formalmath-0.0.8/formalmath/setmm/basic_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:45:07.180895 formalmath-0.0.8/formalmath.egg-info/
+-rw-rw-rw-   0        0        0     3278 2023-06-08 19:45:07.000000 formalmath-0.0.8/formalmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-06-08 19:45:07.000000 formalmath-0.0.8/formalmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 19:45:07.000000 formalmath-0.0.8/formalmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-08 19:45:07.000000 formalmath-0.0.8/formalmath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 19:45:07.181896 formalmath-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-06-08 19:44:26.000000 formalmath-0.0.8/setup.py
```

### Comparing `formalmath-0.0.7/PKG-INFO` & `formalmath-0.0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formalmath
-Version: 0.0.7
+Version: 0.0.8
 Summary: a python port of formal mathematics proof verifier.
 Home-page: https://github.com/lixiang90/formalmath.git
 Author: lixiang90
 Author-email: lixiang90@github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,41 +32,62 @@
 `FormulaTemplate` is the class of templates that generate new formula out of old formulas and other symbols.
 
 The port of other concepts in metamath and set.mm is a work in process.
 
 Example code:
 
 ```python
-from formalmath import setmm
-test1 = setmm.MObject("x1")
-test2 = setmm.MObject("y1")
-# test3 = setmm.MObject("x1")
+from formalmath.setmm import *
+test1 = MObject("x1")
+test2 = MObject("y1")
+# test3 = MObject("x1")
 print(test1) # output: MObject("x1")
-test3 = setmm.MObject.find_MObject_by_label("y1")
+test3 = MObject.find_MObject_by_label("y1")
 print(test3) # output: MObject("y1")
 
-lp1 = setmm.Constant("\\left(")
-rp1 = setmm.Constant("\\right)")
-# lp2 = setmm.Constant("\\left(")
+lp1 = Constant("\\left(")
+rp1 = Constant("\\right)")
+# lp2 = Constant("\\left(")
 print(lp1) # output: Constant("\left(")
-testConst = setmm.Constant.find_MObject_by_label("\\right)")
+testConst = Constant.find_MObject_by_label("\\right)")
 print(testConst) # output: Constant("\right)")
 
-lp = setmm.Constant("(")
-rp = setmm.Constant(")")
-ra = setmm.Constant("->")
-phi = setmm.FormulaVariable("phi")
-psi = setmm.FormulaVariable("psi")
-chi = setmm.FormulaVariable("chi")
-phi_implies_psi = setmm.Formula("phips",list_of_symbols=[lp,phi,ra,psi,rp])
-complex_imply = setmm.Formula("ccimply",list_of_symbols=[lp,phi_implies_psi,ra,chi,rp])
-print(complex_imply) # Formula("(","(","phi","->","psi",")","->","chi",")")
-
-wi = setmm.FormulaTemplate("wi",{"var_types":{"x":Formula,"y":Formula},"template":[lp,"x",ra,"y",rp]})
+lp = Constant("(")
+rp = Constant(")")
+ra = Constant("->")
+phi = FormulaVariable("phi")
+psi = FormulaVariable("psi")
+chi = FormulaVariable("chi")
+phi_implies_psi = Formula("phips",list_of_symbols=[lp,phi,ra,psi,rp])
+complex_imply = Formula("ccimply",list_of_symbols=[lp,phi_implies_psi,ra,chi,rp])
+print(complex_imply) # Formula("( ( phi -> psi ) -> chi )")
+wi = FormulaTemplate({"var_types":{"x":Formula,"y":Formula},"template":[lp,"x",ra,"y",rp]})
 print(wi)
 # Template:  (  x  ->  y  )
 # Types:
-# x:Formula
-# y:Formula
-print(wi.generate("newformula",{"x":psi,"y":chi})) # Formula("(","psi","->","chi",")")
+# x : Formula
+# y : Formula
+nf = wi.generate({"x":psi,"y":chi})
+print(nf) # Formula("( psi -> chi )")
+nf2 = wi.generate({"x":phi,"y":nf})
+nf3 = wi.generate({"x":nf,"y":nf2})
+print(nf3) # Formula("( ( psi -> chi ) -> ( phi -> ( psi -> chi ) ) )")
+
+wi2 = wi.generate_template({"x":"y","y":"z"})
+wiwi = wi.generate_template({"x":wi,"y":wi2})
+print(wiwi)
+# Template:  (  (  x  ->  y  )  ->  (  y  ->  z  )  )
+# Types:
+# x : Formula
+# y : Formula
+# z : Formula
+wi3 = wiwi.generate_template({"x":wi2,"y":wiwi,"z":"w"})
+print(wi3)
+# Template:  (  (  (  y  ->  z  )  ->  (  (  x  ->  y  )  ->  (  y  ->  z  )  )  ) 
+#  ->  (  (  (  x  ->  y  )  ->  (  y  ->  z  )  )  ->  w  )  )
+# Types:
+# y : Formula
+# z : Formula
+# x : Formula
+# w : Formula
 ```
```

### Comparing `formalmath-0.0.7/README.md` & `formalmath-0.0.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -19,41 +19,62 @@
 `FormulaTemplate` is the class of templates that generate new formula out of old formulas and other symbols.
 
 The port of other concepts in metamath and set.mm is a work in process.
 
 Example code:
 
 ```python
-from formalmath import setmm
-test1 = setmm.MObject("x1")
-test2 = setmm.MObject("y1")
-# test3 = setmm.MObject("x1")
+from formalmath.setmm import *
+test1 = MObject("x1")
+test2 = MObject("y1")
+# test3 = MObject("x1")
 print(test1) # output: MObject("x1")
-test3 = setmm.MObject.find_MObject_by_label("y1")
+test3 = MObject.find_MObject_by_label("y1")
 print(test3) # output: MObject("y1")
 
-lp1 = setmm.Constant("\\left(")
-rp1 = setmm.Constant("\\right)")
-# lp2 = setmm.Constant("\\left(")
+lp1 = Constant("\\left(")
+rp1 = Constant("\\right)")
+# lp2 = Constant("\\left(")
 print(lp1) # output: Constant("\left(")
-testConst = setmm.Constant.find_MObject_by_label("\\right)")
+testConst = Constant.find_MObject_by_label("\\right)")
 print(testConst) # output: Constant("\right)")
 
-lp = setmm.Constant("(")
-rp = setmm.Constant(")")
-ra = setmm.Constant("->")
-phi = setmm.FormulaVariable("phi")
-psi = setmm.FormulaVariable("psi")
-chi = setmm.FormulaVariable("chi")
-phi_implies_psi = setmm.Formula("phips",list_of_symbols=[lp,phi,ra,psi,rp])
-complex_imply = setmm.Formula("ccimply",list_of_symbols=[lp,phi_implies_psi,ra,chi,rp])
-print(complex_imply) # Formula("(","(","phi","->","psi",")","->","chi",")")
-
-wi = setmm.FormulaTemplate("wi",{"var_types":{"x":Formula,"y":Formula},"template":[lp,"x",ra,"y",rp]})
+lp = Constant("(")
+rp = Constant(")")
+ra = Constant("->")
+phi = FormulaVariable("phi")
+psi = FormulaVariable("psi")
+chi = FormulaVariable("chi")
+phi_implies_psi = Formula("phips",list_of_symbols=[lp,phi,ra,psi,rp])
+complex_imply = Formula("ccimply",list_of_symbols=[lp,phi_implies_psi,ra,chi,rp])
+print(complex_imply) # Formula("( ( phi -> psi ) -> chi )")
+wi = FormulaTemplate({"var_types":{"x":Formula,"y":Formula},"template":[lp,"x",ra,"y",rp]})
 print(wi)
 # Template:  (  x  ->  y  )
 # Types:
-# x:Formula
-# y:Formula
-print(wi.generate("newformula",{"x":psi,"y":chi})) # Formula("(","psi","->","chi",")")
+# x : Formula
+# y : Formula
+nf = wi.generate({"x":psi,"y":chi})
+print(nf) # Formula("( psi -> chi )")
+nf2 = wi.generate({"x":phi,"y":nf})
+nf3 = wi.generate({"x":nf,"y":nf2})
+print(nf3) # Formula("( ( psi -> chi ) -> ( phi -> ( psi -> chi ) ) )")
+
+wi2 = wi.generate_template({"x":"y","y":"z"})
+wiwi = wi.generate_template({"x":wi,"y":wi2})
+print(wiwi)
+# Template:  (  (  x  ->  y  )  ->  (  y  ->  z  )  )
+# Types:
+# x : Formula
+# y : Formula
+# z : Formula
+wi3 = wiwi.generate_template({"x":wi2,"y":wiwi,"z":"w"})
+print(wi3)
+# Template:  (  (  (  y  ->  z  )  ->  (  (  x  ->  y  )  ->  (  y  ->  z  )  )  ) 
+#  ->  (  (  (  x  ->  y  )  ->  (  y  ->  z  )  )  ->  w  )  )
+# Types:
+# y : Formula
+# z : Formula
+# x : Formula
+# w : Formula
 ```
```

### Comparing `formalmath-0.0.7/formalmath/setmm/basic_classes.py` & `formalmath-0.0.8/formalmath/setmm/basic_classes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,95 @@
 '''
 Python port for a slightly extended version of the formal language metamath (us.metamath.org) and the theorem database set.mm written by metamath. This system includes over 40000 theorems in the classic ZFC axiom system.
 
 The basic classes will be defined in this file. That includes:
 0. MObject. The base class for all classes.
 1. Constant. That correspond to $c statement in metamath.
 2. Variable. That correspond to $v statement in metamath.
-3. FormulaTemplate. That correspond to $a statements starting with wff symbol. Basically, it generates new formula from old. But the template's symbol list can also have Constant, ClassVariable, SetVariable, etc.
+3. FormulaTemplate. That correspond to $a statements starting with wff symbol. Basically, it generates new formula from old. But the template's symbol list can also have Constant, ClassVariable, ClassType, SetVariable, etc.
 4. Formula. That correspond to wff in metamath and set.mm. It is not a part of the basic metamath language. But it is defined in set.mm to denote well formed formula. There is always new ways to form a wff, when a new term is introduced. But all of them correspond to a conbination of old terms.
-5. ClassVariable. That correspond to class in metamath and set.mm.
-6. SetVariable. That correspond to setvar in metamath and set.mm.
-7. Axiom. That correspond to $a statements that are axioms.
-8. Definition. That correspond to $a statements that are definitions.
+5. ClassType. That correspond to class in metamath and set.mm.
+6. ClassVariable. That correspond to class denoted by a single symbol in metamath and set.mm.
+7. SetVariable. That correspond to setvar in metamath and set.mm.
+8. Axiom. That correspond to $a statements that are axioms.
+9. Definition. That correspond to $a statements that are definitions.
+
+Inherit relation:
+MObject ----- Constant
+          |
+          |-- Variable -- SetVariable
+          |         
+          |-- Formula -- FormulaVariable (also inherit Variable)
+          |
+          |-- FormulaTemplate
+          |
+          |-- ClassType -- ClassVariable (also inherit Variable)
 
 Some basic constants will be defined here too, such as left and right parenthesis, well-formed formula symbol and turnstile.
 '''
 
 class MObject:
     '''
     Base class for all metamath classes.
     Use this to ensure the uniqueness of labels and codes.
     '''
 
-    # global dictionaries that ensures the uniqueness of MObject labels, short_codes and metamath_codes.
-    # these dicts can also be used to search MObjects by labels, short_codes and metamath_codes.
+    # global dictionaries that ensures the uniqueness of MObject labels, latex_codes and metamath_codes.
+    # these dicts can also be used to search MObjects by labels, latex_codes and metamath_codes.
     MObject_labels = {}
-    MObject_short_codes = {}
+    MObject_latex_codes = {}
     MObject_metamath_codes = {}
 
-    def __init__(self, label, short_code=None, metamath_code=None):
+    def __init__(self, label=None, latex_code=None, metamath_code=None):
         '''
         construction function of MObject.
         label: label of the MObject. It is unique.
-        short_code: a shorter code for the MObject. Also unique.
+        latex_code: a latex code for the MObject. Also unique.
         metamath_code: the corresponding original code in set.mm.
         '''
-        # ensure the uniqueness of label
-        self._check_unique_label(label)
-        # define the label of an MObject
-        self.label = label
+        if label:
+            # ensure the uniqueness of label
+            self._check_unique_label(label)
+            # define the label of an MObject
+            self.label = label
         
-        if short_code:
-            # ensure the uniqueness of short_code
-            self._check_unique_short_code(short_code)
-            # define the short_code of an MObject
-            self.short_code = short_code
+        if latex_code:
+            # ensure the uniqueness of latex_code
+            self._check_unique_latex_code(latex_code)
+            # define the latex_code of an MObject
+            self.latex_code = latex_code
 
         if metamath_code:
             # ensure the uniqueness of metamath_code
             self._check_unique_metamath_code(metamath_code)
             # define the metamath_code of an MObject
             self.metamath_code = metamath_code
 
         # add the new MObject into dicts
         MObject.MObject_labels[label] = self
-        if short_code:
-            MObject.MObject_short_codes[short_code] = self
+        if latex_code:
+            MObject.MObject_latex_codes[latex_code] = self
         if metamath_code:
             MObject.MObject_metamath_codes[metamath_code] = self
     
     def _check_unique_label(self, label):
         '''
         ensure label is not seen in MObject_labels
         '''
         # if label is used before, raise ValueError.
         if label in MObject.MObject_labels:
             raise ValueError("Duplicate label: {}".format(label))
         
-    def _check_unique_short_code(self, short_code):
+    def _check_unique_latex_code(self, latex_code):
         '''
-        ensure short_code is not seen in MObject_short_codes
+        ensure latex_code is not seen in MObject_latex_codes
         '''
-        # if short_code is used before, raise ValueError.
-        if short_code in MObject.MObject_short_codes:
-            raise ValueError("Duplicate short_code: {}".format(short_code))
+        # if latex_code is used before, raise ValueError.
+        if latex_code in MObject.MObject_latex_codes:
+            raise ValueError("Duplicate latex_code: {}".format(latex_code))
 
     def _check_unique_metamath_code(self, metamath_code):
         '''
         ensure metamath_code is not seen in MObject_metamath_codes
         '''
         # if metamath_code is used before, raise ValueError.
         if metamath_code in MObject.MObject_metamath_codes:
@@ -95,22 +108,22 @@
         '''
         if label in MObject.MObject_labels:
             return MObject.MObject_labels[label]
         else:
             raise ValueError("MObject label not found: {}".format(label))
 
     @classmethod
-    def find_MObject_by_short_code(cls, short_code):
+    def find_MObject_by_latex_code(cls, latex_code):
         '''
-        Find MObject by short_code. Need exact match. 
+        Find MObject by latex_code. Need exact match. 
         '''
-        if short_code in MObject.MObject_short_codes:
-            return MObject.MObject_short_codes[short_code]
+        if latex_code in MObject.MObject_latex_codes:
+            return MObject.MObject_latex_codes[latex_code]
         else:
-            raise ValueError("MObject short_code not found: {}".format(short_code))
+            raise ValueError("MObject latex_code not found: {}".format(latex_code))
 
     @classmethod
     def find_MObject_by_metamath_code(cls, metamath_code):
         '''
         Find MObject by metamath_code. Need exact match. 
         '''
         if metamath_code in MObject.MObject_metamath_codes:
@@ -119,146 +132,235 @@
             raise ValueError("MObject metamath_code not found: {}".format(metamath_code))
 
 class Constant(MObject):
     '''
     $c statement in metamath, denote constant objects.
     Example: left and right parenthesis, wff symbol
     '''
-    def __init__(self, label, short_code=None, metamath_code=None):
+    def __init__(self, label=None, latex_code=None, metamath_code=None):
         '''
         construction function of Constant.
         just need to inherit from MObject.
         '''
-        super().__init__(label, short_code, metamath_code)
+        super().__init__(label, latex_code, metamath_code)
     
     def __str__(self):
         '''
         print Constant. will override the __str__ method in MObject.
         '''
         return f"Constant(\"{self.label}\")"
 
 class Variable(MObject):
     '''
     $v statement in metamath, denote variable objects.
     '''
-    def __init__(self, label, short_code=None, metamath_code=None):
+    def __init__(self, label=None, latex_code=None, metamath_code=None):
         '''
         construction function of Variable.
         just need to inherit from MObject.
         '''
-        super().__init__(label, short_code, metamath_code)
+        super().__init__(label, latex_code, metamath_code)
     
     def __str__(self):
         '''
         print Variable. will override the __str__ method in MObject.
         '''
         return f"Variable(\"{self.label}\")"
 
 class Formula(MObject):
     '''
     base class for well formed formulas.
     '''
-    def __init__(self, label, short_code=None, metamath_code=None, list_of_symbols=None):
+    def __init__(self, label=None, latex_code=None, metamath_code=None, list_of_symbols=None):
         '''
         construction function for Formula.
-        list_of_symbols: a list of constants and formulas, making the symbols of the new formula 
+        list_of_symbols: a list of constants and formulas and classes and setvars, making the symbols of the new formula 
         '''
-        super().__init__(label, short_code, metamath_code)
+        super().__init__(label, latex_code, metamath_code)
         if list_of_symbols:
             self._check_symbol_type(list_of_symbols)
             my_list = []
             for symbol in list_of_symbols:
-                if isinstance(symbol, Formula):
+                if isinstance(symbol, (Formula, ClassType)):
                     my_list = my_list + symbol.list_of_symbols
                 else:
                     my_list.append(symbol)
             self.list_of_symbols = my_list
     
     def _check_symbol_type(self, list_of_symbols):
         '''
-        Ensure that all symbols in the list_of_symbols are of type Constant, Formula ClassVariable and SetVariable.
+        Ensure that all symbols in the list_of_symbols are of type Constant, Formula ClassType and SetVariable.
         Otherwise, raise TypeError.
         '''
         for symbol in list_of_symbols:
-            if not isinstance(symbol, (Constant, Formula, ClassVariable, SetVariable)):
-                raise TypeError(f"{symbol}: not in supported type. We support Constant, Formula, ClassVariable and SetVariable for symbols in list_of_symbols.")
+            if not isinstance(symbol, (Constant, Formula, ClassType, SetVariable)):
+                raise TypeError(f"{symbol}: not in supported type. We support Constant, Formula, ClassType and SetVariable for symbols in list_of_symbols.")
     
     def __str__(self):
         '''
         print Formula. will override the __str__ method in MObject.
         '''
-        labelstr = ','.join([f"\"{s.label}\"" for s in self.list_of_symbols])
-        return f"Formula({labelstr})"
+        labelstr = ' '.join([f"{s.label}" for s in self.list_of_symbols])
+        return f"Formula(\"{labelstr}\")"
     
-
 class FormulaVariable(Variable, Formula):
     '''
     $f statement of form $f wff varname $. It means that varname represents a well formed formula.
     This class is the special kind of Formula consisting of only one variable.
     '''
-    def __init__(self, label, short_code=None, metamath_code=None):
-        super().__init__(label, short_code, metamath_code)
+    def __init__(self, label=None, latex_code=None, metamath_code=None):
+        super().__init__(label, latex_code, metamath_code)
         self.list_of_symbols = [self]
     
     def __str__(self):
         return f"Formula(\"{self.label}\")"
 
-class ClassVariable(Variable):
+class ClassType(MObject):
+    '''
+    base class for classes of set.mm.
+    '''
+    def __init__(self, label=None, latex_code=None, metamath_code=None, list_of_symbols=None):
+        '''
+        construction function for ClassType.
+        list_of_symbols: a list of constants and formulas and classes and setvars, making the symbols of the new class
+        '''
+        super().__init__(label, latex_code, metamath_code)
+        if list_of_symbols:
+            self._check_symbol_type(list_of_symbols)
+            my_list = []
+            for symbol in list_of_symbols:
+                if isinstance(symbol, (Formula, ClassType)):
+                    my_list = my_list + symbol.list_of_symbols
+                else:
+                    my_list.append(symbol)
+            self.list_of_symbols = my_list
+    
+    def _check_symbol_type(self, list_of_symbols):
+        '''
+        Ensure that all symbols in the list_of_symbols are of type Constant, Formula, ClassType and SetVariable.
+        Otherwise, raise TypeError.
+        '''
+        for symbol in list_of_symbols:
+            if not isinstance(symbol, (Constant, Formula, ClassType, SetVariable)):
+                raise TypeError(f"{symbol}: not in supported type. We support Constant, Formula, ClassType and SetVariable for symbols in list_of_symbols.")
+    
+    def __str__(self):
+        '''
+        print ClaaType. will override the __str__ method in MObject.
+        '''
+        labelstr = ' '.join([f"{s.label}" for s in self.list_of_symbols])
+        return f"Formula(\"{labelstr}\")"
+
+class ClassVariable(Variable, ClassType):
     '''
     $f statement of form $f class varname $. It means that varname represents a class.
     '''
-    def __init__(self, label, short_code=None, metamath_code=None):
-        super().__init__(label, short_code, metamath_code)
+    def __init__(self, label=None, latex_code=None, metamath_code=None):
+        super().__init__(label, latex_code, metamath_code)
+        self.list_of_symbols = [self]
     
     def __str__(self):
         return f"ClassVariable(\"{self.label}\")"
 
 class SetVariable(Variable):
     '''
     $f statement of form $f setvar varname $. It means that varname represents a set variable.
     '''
-    def __init__(self, label, short_code=None, metamath_code=None):
-        super().__init__(label, short_code, metamath_code)
+    def __init__(self, label=None, latex_code=None, metamath_code=None):
+        super().__init__(label, latex_code, metamath_code)
     
     def __str__(self):
         return f"SetVariable(\"{self.label}\")"
 
 class FormulaTemplate(MObject):
     '''
     $a statements that generates new Formula from old by substitution.
     '''
-    def __init__(self, label, template, short_code=None, metamath_code=None):
+    def __init__(self, template=None, label=None, latex_code=None, metamath_code=None):
         '''
         template: a dictionary that has keys "var_types" and "template"
         example: {"var_types":{"x":Formula,"y":Formula},"template":[lp,"x",ra,"y",rp]}
         this example means in the Template of Formula "( x -> y )", x, y should be replaced with Formulas.
         '''
-        super().__init__(label, short_code, metamath_code)
+        super().__init__(label, latex_code, metamath_code)
         # check that the template has the right format.
-        self._check_template(template)
-        def generate(mylabel, vars, mycode=None, mymmcode=None):
-            # use the template to define a generator of new Formula from old 
-            mylist = []
-            for symbol in template["template"]:
-                if isinstance(symbol,str):
-                    if template["var_types"][symbol] == Formula:
-                        if len(vars[symbol].list_of_symbols) > 1:
-                            mylist = mylist + vars[symbol].list_of_symbols
-                        else:
-                            mylist.append(vars[symbol])
+        self._check_template(template)            
+        setattr(self, "template", template)
+        
+    def generate(self, vars, mylabel=None, mycode=None, mymmcode=None):
+        '''
+        use the template to define a generator of new Formula from old
+        '''
+        mylist = []
+        for symbol in self.template["template"]:
+            if isinstance(symbol,str):
+                if self.template["var_types"][symbol] in [Formula,ClassType]:
+                    if len(vars[symbol].list_of_symbols) > 1:
+                        mylist = mylist + vars[symbol].list_of_symbols
                     else:
                         mylist.append(vars[symbol])
                 else:
-                    mylist.append(symbol)
-            newFormula = Formula(mylabel,mycode,mymmcode,mylist)
-            return newFormula
-            
-        setattr(self, "template", template)
-        setattr(self, "generate", generate)
-    
+                    mylist.append(vars[symbol])
+            else:
+                mylist.append(symbol)
+        newFormula = Formula(mylabel,mycode,mymmcode,mylist)
+        return newFormula
+    
+    def generate_template(self, vars, mylabel=None, mycode=None, mymmcode=None):
+        '''
+        use the template to define a generator of new FormulaTemplate from old 
+        '''
+        new_var_types = {}
+        new_template = []
+        var_types = self.template["var_types"]
+        temp = self.template["template"]
+
+        # example 1. temp is (x->y), var_types={"x":Formula,"y":Formula}, vars={"x":"z","y":"w"}
+        # then new_var_types should be {"z":Formula,"w":Formula}
+        # and, new_template should be (z->w)
+
+        # example 2. temp is (x->y), var_types={"x":Formula,"y":Formula}, vars={"x":f1,"y":f2}
+        # where f1 is a template: temp is (z->w), var_types={"z":Formula,"w":Formula},
+        # f2 is also a template: temp is (z->t), var_types={"z":Formula,"t":Formula},
+        # then new_var_types should be {"z":Formula,"w":Formula,"t":Formula}
+        # and, new_template should be ((z->w)->(z->t))
+
+        for item in vars.keys():
+            if isinstance(vars[item], str):
+                if vars[item] not in new_var_types.keys():
+                    new_var_types[vars[item]] = var_types[item]
+                else:
+                    if new_var_types[vars[item]] != var_types[item]:
+                        raise ValueError(f"Conflict types: {new_var_types[vars[item]]} and {var_types[item]}")
+            elif isinstance(vars[item], FormulaTemplate):
+                for symbol in vars[item].template["var_types"].keys():
+                    if symbol not in new_var_types.keys():
+                        new_var_types[symbol] = vars[item].template["var_types"][symbol]
+                    else:
+                        if new_var_types[symbol] != vars[item].template["var_types"][symbol]:
+                            raise ValueError(f"Conflict types: {new_var_types[symbol]} and {vars[item].template['var_types'][symbol]}")
+            else:
+                pass
+        
+        for symbol in temp:
+            if isinstance(symbol, str):
+                if isinstance(vars[symbol],str):
+                    new_template.append(vars[symbol])
+                else:
+                    if symbol not in vars.keys():
+                        raise ValueError(f"Undefined symbol : {symbol}")
+                    if not isinstance(vars[symbol],FormulaTemplate):
+                        raise ValueError(f"Unsupported type : {vars[symbol]}")
+                    new_template = new_template + vars[symbol].template["template"]
+            else:
+                new_template.append(symbol)
+        
+        new_formula_temp = FormulaTemplate({"var_types":new_var_types,"template":new_template},mylabel,mycode,mymmcode)
+        return new_formula_temp
+
     def _check_template(self, template):
         '''
         check that the template has the right format.
         '''
         if not isinstance(template["template"], list):
             raise ValueError(f"Template is not a list.")
         vars = template["var_types"].keys()
@@ -281,15 +383,15 @@
         for symbol in self.template["template"]:
             if isinstance(symbol, str):
                 temp_str += f" {symbol} "
             else:
                 temp_str += f" {symbol.label} "
         vartype_str = ""
         for v in self.template["var_types"].keys():
-            vartype_str += f"{v}:{self.template['var_types'][v].__name__}\n"
+            vartype_str += f"{v} : {self.template['var_types'][v].__name__}\n"
         return f"Template: {temp_str}\nTypes:\n{vartype_str}"
 
 
 
 
 
 if __name__=='__main__':
@@ -297,18 +399,37 @@
     rp = Constant(")")
     ra = Constant("->")
     phi = FormulaVariable("phi")
     psi = FormulaVariable("psi")
     chi = FormulaVariable("chi")
     phi_implies_psi = Formula("phips",list_of_symbols=[lp,phi,ra,psi,rp])
     complex_imply = Formula("ccimply",list_of_symbols=[lp,phi_implies_psi,ra,chi,rp])
-    print(complex_imply) # Formula("(","(","phi","->","psi",")","->","chi",")")
-    wi = FormulaTemplate("wi",{"var_types":{"x":Formula,"y":Formula},"template":[lp,"x",ra,"y",rp]})
+    print(complex_imply) # Formula("( ( phi -> psi ) -> chi )")
+    wi = FormulaTemplate({"var_types":{"x":Formula,"y":Formula},"template":[lp,"x",ra,"y",rp]})
     print(wi)
     # Template:  (  x  ->  y  )
     # Types:
-    # x:Formula
-    # y:Formula
-    print(wi.generate("newformula",{"x":psi,"y":chi})) # Formula("(","psi","->","chi",")")
-
-    
-    
+    # x : Formula
+    # y : Formula
+    nf = wi.generate({"x":psi,"y":chi})
+    print(nf) # Formula("( psi -> chi )")
+    nf2 = wi.generate({"x":phi,"y":nf})
+    nf3 = wi.generate({"x":nf,"y":nf2})
+    print(nf3) # Formula("( ( psi -> chi ) -> ( phi -> ( psi -> chi ) ) )")
+
+    wi2 = wi.generate_template({"x":"y","y":"z"})
+    wiwi = wi.generate_template({"x":wi,"y":wi2})
+    print(wiwi)
+    # Template:  (  (  x  ->  y  )  ->  (  y  ->  z  )  )
+    # Types:
+    # x : Formula
+    # y : Formula
+    # z : Formula
+    wi3 = wiwi.generate_template({"x":wi2,"y":wiwi,"z":"w"})
+    print(wi3)
+    # Template:  (  (  (  y  ->  z  )  ->  (  (  x  ->  y  )  ->  (  y  ->  z  )  )  ) 
+    #  ->  (  (  (  x  ->  y  )  ->  (  y  ->  z  )  )  ->  w  )  )
+    # Types:
+    # y : Formula
+    # z : Formula
+    # x : Formula
+    # w : Formula
```

### Comparing `formalmath-0.0.7/formalmath.egg-info/PKG-INFO` & `formalmath-0.0.8/formalmath.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formalmath
-Version: 0.0.7
+Version: 0.0.8
 Summary: a python port of formal mathematics proof verifier.
 Home-page: https://github.com/lixiang90/formalmath.git
 Author: lixiang90
 Author-email: lixiang90@github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,41 +32,62 @@
 `FormulaTemplate` is the class of templates that generate new formula out of old formulas and other symbols.
 
 The port of other concepts in metamath and set.mm is a work in process.
 
 Example code:
 
 ```python
-from formalmath import setmm
-test1 = setmm.MObject("x1")
-test2 = setmm.MObject("y1")
-# test3 = setmm.MObject("x1")
+from formalmath.setmm import *
+test1 = MObject("x1")
+test2 = MObject("y1")
+# test3 = MObject("x1")
 print(test1) # output: MObject("x1")
-test3 = setmm.MObject.find_MObject_by_label("y1")
+test3 = MObject.find_MObject_by_label("y1")
 print(test3) # output: MObject("y1")
 
-lp1 = setmm.Constant("\\left(")
-rp1 = setmm.Constant("\\right)")
-# lp2 = setmm.Constant("\\left(")
+lp1 = Constant("\\left(")
+rp1 = Constant("\\right)")
+# lp2 = Constant("\\left(")
 print(lp1) # output: Constant("\left(")
-testConst = setmm.Constant.find_MObject_by_label("\\right)")
+testConst = Constant.find_MObject_by_label("\\right)")
 print(testConst) # output: Constant("\right)")
 
-lp = setmm.Constant("(")
-rp = setmm.Constant(")")
-ra = setmm.Constant("->")
-phi = setmm.FormulaVariable("phi")
-psi = setmm.FormulaVariable("psi")
-chi = setmm.FormulaVariable("chi")
-phi_implies_psi = setmm.Formula("phips",list_of_symbols=[lp,phi,ra,psi,rp])
-complex_imply = setmm.Formula("ccimply",list_of_symbols=[lp,phi_implies_psi,ra,chi,rp])
-print(complex_imply) # Formula("(","(","phi","->","psi",")","->","chi",")")
-
-wi = setmm.FormulaTemplate("wi",{"var_types":{"x":Formula,"y":Formula},"template":[lp,"x",ra,"y",rp]})
+lp = Constant("(")
+rp = Constant(")")
+ra = Constant("->")
+phi = FormulaVariable("phi")
+psi = FormulaVariable("psi")
+chi = FormulaVariable("chi")
+phi_implies_psi = Formula("phips",list_of_symbols=[lp,phi,ra,psi,rp])
+complex_imply = Formula("ccimply",list_of_symbols=[lp,phi_implies_psi,ra,chi,rp])
+print(complex_imply) # Formula("( ( phi -> psi ) -> chi )")
+wi = FormulaTemplate({"var_types":{"x":Formula,"y":Formula},"template":[lp,"x",ra,"y",rp]})
 print(wi)
 # Template:  (  x  ->  y  )
 # Types:
-# x:Formula
-# y:Formula
-print(wi.generate("newformula",{"x":psi,"y":chi})) # Formula("(","psi","->","chi",")")
+# x : Formula
+# y : Formula
+nf = wi.generate({"x":psi,"y":chi})
+print(nf) # Formula("( psi -> chi )")
+nf2 = wi.generate({"x":phi,"y":nf})
+nf3 = wi.generate({"x":nf,"y":nf2})
+print(nf3) # Formula("( ( psi -> chi ) -> ( phi -> ( psi -> chi ) ) )")
+
+wi2 = wi.generate_template({"x":"y","y":"z"})
+wiwi = wi.generate_template({"x":wi,"y":wi2})
+print(wiwi)
+# Template:  (  (  x  ->  y  )  ->  (  y  ->  z  )  )
+# Types:
+# x : Formula
+# y : Formula
+# z : Formula
+wi3 = wiwi.generate_template({"x":wi2,"y":wiwi,"z":"w"})
+print(wi3)
+# Template:  (  (  (  y  ->  z  )  ->  (  (  x  ->  y  )  ->  (  y  ->  z  )  )  ) 
+#  ->  (  (  (  x  ->  y  )  ->  (  y  ->  z  )  )  ->  w  )  )
+# Types:
+# y : Formula
+# z : Formula
+# x : Formula
+# w : Formula
 ```
```

### Comparing `formalmath-0.0.7/setup.py` & `formalmath-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="formalmath",  # Replace with your own username
-    version="0.0.7",
+    version="0.0.8",
     author="lixiang90",
     author_email="lixiang90@github.com",
     description="a python port of formal mathematics proof verifier.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lixiang90/formalmath.git",
     packages=setuptools.find_packages(),
```

