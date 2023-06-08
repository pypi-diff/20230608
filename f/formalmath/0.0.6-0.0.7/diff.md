# Comparing `tmp/formalmath-0.0.6.tar.gz` & `tmp/formalmath-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formalmath-0.0.6.tar", last modified: Thu Jun  8 00:56:33 2023, max compression
+gzip compressed data, was "formalmath-0.0.7.tar", last modified: Thu Jun  8 02:48:46 2023, max compression
```

## Comparing `formalmath-0.0.6.tar` & `formalmath-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 00:56:33.799463 formalmath-0.0.6/
--rw-rw-rw-   0        0        0     2371 2023-06-08 00:56:33.799463 formalmath-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1925 2023-06-08 00:55:49.000000 formalmath-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 00:56:33.796952 formalmath-0.0.6/formalmath/
--rw-rw-rw-   0        0        0       19 2023-06-06 03:06:28.000000 formalmath-0.0.6/formalmath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:56:33.798463 formalmath-0.0.6/formalmath/setmm/
--rw-rw-rw-   0        0        0       28 2023-06-06 03:07:05.000000 formalmath-0.0.6/formalmath/setmm/__init__.py
--rw-rw-rw-   0        0        0     8860 2023-06-08 00:50:46.000000 formalmath-0.0.6/formalmath/setmm/basic_classes.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:56:33.798463 formalmath-0.0.6/formalmath.egg-info/
--rw-rw-rw-   0        0        0     2371 2023-06-08 00:56:33.000000 formalmath-0.0.6/formalmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-06-08 00:56:33.000000 formalmath-0.0.6/formalmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 00:56:33.000000 formalmath-0.0.6/formalmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-08 00:56:33.000000 formalmath-0.0.6/formalmath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 00:56:33.799463 formalmath-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      743 2023-06-08 00:56:09.000000 formalmath-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:48:46.458856 formalmath-0.0.7/
+-rw-rw-rw-   0        0        0     2753 2023-06-08 02:48:46.457857 formalmath-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2307 2023-06-08 02:47:47.000000 formalmath-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 02:48:46.454857 formalmath-0.0.7/formalmath/
+-rw-rw-rw-   0        0        0       19 2023-06-06 03:06:28.000000 formalmath-0.0.7/formalmath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:48:46.457857 formalmath-0.0.7/formalmath/setmm/
+-rw-rw-rw-   0        0        0       28 2023-06-06 03:07:05.000000 formalmath-0.0.7/formalmath/setmm/__init__.py
+-rw-rw-rw-   0        0        0    13037 2023-06-08 02:44:40.000000 formalmath-0.0.7/formalmath/setmm/basic_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:48:46.456857 formalmath-0.0.7/formalmath.egg-info/
+-rw-rw-rw-   0        0        0     2753 2023-06-08 02:48:46.000000 formalmath-0.0.7/formalmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-06-08 02:48:46.000000 formalmath-0.0.7/formalmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 02:48:46.000000 formalmath-0.0.7/formalmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-08 02:48:46.000000 formalmath-0.0.7/formalmath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 02:48:46.458856 formalmath-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-06-08 02:48:17.000000 formalmath-0.0.7/setup.py
```

### Comparing `formalmath-0.0.6/PKG-INFO` & `formalmath-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formalmath
-Version: 0.0.6
+Version: 0.0.7
 Summary: a python port of formal mathematics proof verifier.
 Home-page: https://github.com/lixiang90/formalmath.git
 Author: lixiang90
 Author-email: lixiang90@github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,14 +25,16 @@
 
 `Variable` is the class of variables, corresponding to $v statements in metamath.
 
 `Formula` is the base class of formulas, corresponding to wff in metamath and set.mm.
 
 `FormulaVariable` is the class of formula with only one symbol.
 
+`FormulaTemplate` is the class of templates that generate new formula out of old formulas and other symbols.
+
 The port of other concepts in metamath and set.mm is a work in process.
 
 Example code:
 
 ```python
 from formalmath import setmm
 test1 = setmm.MObject("x1")
@@ -54,9 +56,17 @@
 ra = setmm.Constant("->")
 phi = setmm.FormulaVariable("phi")
 psi = setmm.FormulaVariable("psi")
 chi = setmm.FormulaVariable("chi")
 phi_implies_psi = setmm.Formula("phips",list_of_symbols=[lp,phi,ra,psi,rp])
 complex_imply = setmm.Formula("ccimply",list_of_symbols=[lp,phi_implies_psi,ra,chi,rp])
 print(complex_imply) # Formula("(","(","phi","->","psi",")","->","chi",")")
+
+wi = setmm.FormulaTemplate("wi",{"var_types":{"x":Formula,"y":Formula},"template":[lp,"x",ra,"y",rp]})
+print(wi)
+# Template:  (  x  ->  y  )
+# Types:
+# x:Formula
+# y:Formula
+print(wi.generate("newformula",{"x":psi,"y":chi})) # Formula("(","psi","->","chi",")")
 ```
```

### Comparing `formalmath-0.0.6/README.md` & `formalmath-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 `Variable` is the class of variables, corresponding to $v statements in metamath.
 
 `Formula` is the base class of formulas, corresponding to wff in metamath and set.mm.
 
 `FormulaVariable` is the class of formula with only one symbol.
 
+`FormulaTemplate` is the class of templates that generate new formula out of old formulas and other symbols.
+
 The port of other concepts in metamath and set.mm is a work in process.
 
 Example code:
 
 ```python
 from formalmath import setmm
 test1 = setmm.MObject("x1")
@@ -41,9 +43,17 @@
 ra = setmm.Constant("->")
 phi = setmm.FormulaVariable("phi")
 psi = setmm.FormulaVariable("psi")
 chi = setmm.FormulaVariable("chi")
 phi_implies_psi = setmm.Formula("phips",list_of_symbols=[lp,phi,ra,psi,rp])
 complex_imply = setmm.Formula("ccimply",list_of_symbols=[lp,phi_implies_psi,ra,chi,rp])
 print(complex_imply) # Formula("(","(","phi","->","psi",")","->","chi",")")
+
+wi = setmm.FormulaTemplate("wi",{"var_types":{"x":Formula,"y":Formula},"template":[lp,"x",ra,"y",rp]})
+print(wi)
+# Template:  (  x  ->  y  )
+# Types:
+# x:Formula
+# y:Formula
+print(wi.generate("newformula",{"x":psi,"y":chi})) # Formula("(","psi","->","chi",")")
 ```
```

### Comparing `formalmath-0.0.6/formalmath/setmm/basic_classes.py` & `formalmath-0.0.7/formalmath/setmm/basic_classes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 Python port for a slightly extended version of the formal language metamath (us.metamath.org) and the theorem database set.mm written by metamath. This system includes over 40000 theorems in the classic ZFC axiom system.
 
 The basic classes will be defined in this file. That includes:
 0. MObject. The base class for all classes.
 1. Constant. That correspond to $c statement in metamath.
 2. Variable. That correspond to $v statement in metamath.
-3. FormulaTemplate. That correspond to $a statements starting with wff symbol. Basically, it generates new formula from old. But the template can also have Constant, ClassVariable, SetVariable, etc.
+3. FormulaTemplate. That correspond to $a statements starting with wff symbol. Basically, it generates new formula from old. But the template's symbol list can also have Constant, ClassVariable, SetVariable, etc.
 4. Formula. That correspond to wff in metamath and set.mm. It is not a part of the basic metamath language. But it is defined in set.mm to denote well formed formula. There is always new ways to form a wff, when a new term is introduced. But all of them correspond to a conbination of old terms.
 5. ClassVariable. That correspond to class in metamath and set.mm.
 6. SetVariable. That correspond to setvar in metamath and set.mm.
 7. Axiom. That correspond to $a statements that are axioms.
 8. Definition. That correspond to $a statements that are definitions.
 
 Some basic constants will be defined here too, such as left and right parenthesis, well-formed formula symbol and turnstile.
@@ -171,52 +171,144 @@
                     my_list = my_list + symbol.list_of_symbols
                 else:
                     my_list.append(symbol)
             self.list_of_symbols = my_list
     
     def _check_symbol_type(self, list_of_symbols):
         '''
-        Ensure that all symbols in the list_of_symbols are of type Constant or Formula.
+        Ensure that all symbols in the list_of_symbols are of type Constant, Formula ClassVariable and SetVariable.
         Otherwise, raise TypeError.
         '''
         for symbol in list_of_symbols:
-            if not isinstance(symbol, (Constant, Formula)):
-                raise TypeError(f"{symbol}: not in supported type. We support Constant and Formula for symbols in list_of_symbols.")
+            if not isinstance(symbol, (Constant, Formula, ClassVariable, SetVariable)):
+                raise TypeError(f"{symbol}: not in supported type. We support Constant, Formula, ClassVariable and SetVariable for symbols in list_of_symbols.")
     
     def __str__(self):
         '''
         print Formula. will override the __str__ method in MObject.
         '''
         labelstr = ','.join([f"\"{s.label}\"" for s in self.list_of_symbols])
         return f"Formula({labelstr})"
+    
 
 class FormulaVariable(Variable, Formula):
     '''
     $f statement of form $f wff varname $. It means that varname represents a well formed formula.
     This class is the special kind of Formula consisting of only one variable.
     '''
     def __init__(self, label, short_code=None, metamath_code=None):
         super().__init__(label, short_code, metamath_code)
         self.list_of_symbols = [self]
     
     def __str__(self):
         return f"Formula(\"{self.label}\")"
 
+class ClassVariable(Variable):
+    '''
+    $f statement of form $f class varname $. It means that varname represents a class.
+    '''
+    def __init__(self, label, short_code=None, metamath_code=None):
+        super().__init__(label, short_code, metamath_code)
+    
+    def __str__(self):
+        return f"ClassVariable(\"{self.label}\")"
+
+class SetVariable(Variable):
+    '''
+    $f statement of form $f setvar varname $. It means that varname represents a set variable.
+    '''
+    def __init__(self, label, short_code=None, metamath_code=None):
+        super().__init__(label, short_code, metamath_code)
+    
+    def __str__(self):
+        return f"SetVariable(\"{self.label}\")"
+
 class FormulaTemplate(MObject):
     '''
     $a statements that generates new Formula from old by substitution.
     '''
+    def __init__(self, label, template, short_code=None, metamath_code=None):
+        '''
+        template: a dictionary that has keys "var_types" and "template"
+        example: {"var_types":{"x":Formula,"y":Formula},"template":[lp,"x",ra,"y",rp]}
+        this example means in the Template of Formula "( x -> y )", x, y should be replaced with Formulas.
+        '''
+        super().__init__(label, short_code, metamath_code)
+        # check that the template has the right format.
+        self._check_template(template)
+        def generate(mylabel, vars, mycode=None, mymmcode=None):
+            # use the template to define a generator of new Formula from old 
+            mylist = []
+            for symbol in template["template"]:
+                if isinstance(symbol,str):
+                    if template["var_types"][symbol] == Formula:
+                        if len(vars[symbol].list_of_symbols) > 1:
+                            mylist = mylist + vars[symbol].list_of_symbols
+                        else:
+                            mylist.append(vars[symbol])
+                    else:
+                        mylist.append(vars[symbol])
+                else:
+                    mylist.append(symbol)
+            newFormula = Formula(mylabel,mycode,mymmcode,mylist)
+            return newFormula
+            
+        setattr(self, "template", template)
+        setattr(self, "generate", generate)
+    
+    def _check_template(self, template):
+        '''
+        check that the template has the right format.
+        '''
+        if not isinstance(template["template"], list):
+            raise ValueError(f"Template is not a list.")
+        vars = template["var_types"].keys()
+        for symbol in template["template"]:
+            if not isinstance(symbol, Constant):
+                # ensure the variable symbols in the template has not appeared in the labels of MObjects defined before 
+                self._check_unique_label(symbol)
+                if not isinstance(symbol,str):
+                    raise ValueError("Template format error.")
+                if symbol not in vars:
+                    raise ValueError(f"Found undefined symbol in template: {symbol}")
+        
+        for item in vars:
+            # ensure that the type assignings in template["var_types"] are supported (Formula, SetVariable, ClassVariable)
+            if template["var_types"][item] not in [Formula, SetVariable, ClassVariable]:
+                raise ValueError(f"Found unsupported type in template: {item}:{template['var_types'][item]}")
+        
+    def __str__(self):
+        temp_str = ""
+        for symbol in self.template["template"]:
+            if isinstance(symbol, str):
+                temp_str += f" {symbol} "
+            else:
+                temp_str += f" {symbol.label} "
+        vartype_str = ""
+        for v in self.template["var_types"].keys():
+            vartype_str += f"{v}:{self.template['var_types'][v].__name__}\n"
+        return f"Template: {temp_str}\nTypes:\n{vartype_str}"
+
+
+
 
 
 if __name__=='__main__':
     lp = Constant("(")
     rp = Constant(")")
     ra = Constant("->")
     phi = FormulaVariable("phi")
     psi = FormulaVariable("psi")
     chi = FormulaVariable("chi")
     phi_implies_psi = Formula("phips",list_of_symbols=[lp,phi,ra,psi,rp])
     complex_imply = Formula("ccimply",list_of_symbols=[lp,phi_implies_psi,ra,chi,rp])
     print(complex_imply) # Formula("(","(","phi","->","psi",")","->","chi",")")
+    wi = FormulaTemplate("wi",{"var_types":{"x":Formula,"y":Formula},"template":[lp,"x",ra,"y",rp]})
+    print(wi)
+    # Template:  (  x  ->  y  )
+    # Types:
+    # x:Formula
+    # y:Formula
+    print(wi.generate("newformula",{"x":psi,"y":chi})) # Formula("(","psi","->","chi",")")
```

### Comparing `formalmath-0.0.6/formalmath.egg-info/PKG-INFO` & `formalmath-0.0.7/formalmath.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formalmath
-Version: 0.0.6
+Version: 0.0.7
 Summary: a python port of formal mathematics proof verifier.
 Home-page: https://github.com/lixiang90/formalmath.git
 Author: lixiang90
 Author-email: lixiang90@github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,14 +25,16 @@
 
 `Variable` is the class of variables, corresponding to $v statements in metamath.
 
 `Formula` is the base class of formulas, corresponding to wff in metamath and set.mm.
 
 `FormulaVariable` is the class of formula with only one symbol.
 
+`FormulaTemplate` is the class of templates that generate new formula out of old formulas and other symbols.
+
 The port of other concepts in metamath and set.mm is a work in process.
 
 Example code:
 
 ```python
 from formalmath import setmm
 test1 = setmm.MObject("x1")
@@ -54,9 +56,17 @@
 ra = setmm.Constant("->")
 phi = setmm.FormulaVariable("phi")
 psi = setmm.FormulaVariable("psi")
 chi = setmm.FormulaVariable("chi")
 phi_implies_psi = setmm.Formula("phips",list_of_symbols=[lp,phi,ra,psi,rp])
 complex_imply = setmm.Formula("ccimply",list_of_symbols=[lp,phi_implies_psi,ra,chi,rp])
 print(complex_imply) # Formula("(","(","phi","->","psi",")","->","chi",")")
+
+wi = setmm.FormulaTemplate("wi",{"var_types":{"x":Formula,"y":Formula},"template":[lp,"x",ra,"y",rp]})
+print(wi)
+# Template:  (  x  ->  y  )
+# Types:
+# x:Formula
+# y:Formula
+print(wi.generate("newformula",{"x":psi,"y":chi})) # Formula("(","psi","->","chi",")")
 ```
```

### Comparing `formalmath-0.0.6/setup.py` & `formalmath-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="formalmath",  # Replace with your own username
-    version="0.0.6",
+    version="0.0.7",
     author="lixiang90",
     author_email="lixiang90@github.com",
     description="a python port of formal mathematics proof verifier.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lixiang90/formalmath.git",
     packages=setuptools.find_packages(),
```

