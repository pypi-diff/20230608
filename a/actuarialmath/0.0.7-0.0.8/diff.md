# Comparing `tmp/actuarialmath-0.0.7.tar.gz` & `tmp/actuarialmath-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actuarialmath-0.0.7.tar", last modified: Mon Jun  5 21:40:58 2023, max compression
+gzip compressed data, was "actuarialmath-0.0.8.tar", last modified: Thu Jun  8 18:51:56 2023, max compression
```

## Comparing `actuarialmath-0.0.7.tar` & `actuarialmath-0.0.8.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-05 21:40:58.475431 actuarialmath-0.0.7/
--rw-rw-r--   0 terence   (1000) terence   (1000)     1073 2023-05-29 19:44:46.000000 actuarialmath-0.0.7/LICENSE
--rw-rw-r--   0 terence   (1000) terence   (1000)     4193 2023-06-05 21:40:58.475431 actuarialmath-0.0.7/PKG-INFO
--rw-rw-r--   0 terence   (1000) terence   (1000)     4674 2023-06-05 17:43:14.000000 actuarialmath-0.0.7/README.md
--rw-rw-r--   0 terence   (1000) terence   (1000)     3695 2023-06-05 17:52:31.000000 actuarialmath-0.0.7/index.rst
--rw-rw-r--   0 terence   (1000) terence   (1000)      573 2023-06-05 21:40:45.000000 actuarialmath-0.0.7/pyproject.toml
--rw-rw-r--   0 terence   (1000) terence   (1000)       38 2023-06-05 21:40:58.475431 actuarialmath-0.0.7/setup.cfg
-drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-05 21:40:58.471431 actuarialmath-0.0.7/src/
-drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-05 21:40:58.475431 actuarialmath-0.0.7/src/actuarialmath/
--rw-rw-r--   0 terence   (1000) terence   (1000)        0 2023-05-25 13:19:02.000000 actuarialmath-0.0.7/src/actuarialmath/__init__.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     4958 2023-06-04 12:06:44.000000 actuarialmath-0.0.7/src/actuarialmath/actuarial.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    15123 2023-06-04 13:28:04.000000 actuarialmath-0.0.7/src/actuarialmath/annuity.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     9333 2023-06-04 14:59:30.000000 actuarialmath-0.0.7/src/actuarialmath/constantforce.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     3638 2023-06-04 15:05:12.000000 actuarialmath-0.0.7/src/actuarialmath/extrarisk.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     9482 2023-06-04 12:58:13.000000 actuarialmath-0.0.7/src/actuarialmath/fractional.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    21112 2023-06-04 13:13:54.000000 actuarialmath-0.0.7/src/actuarialmath/insurance.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     6029 2023-06-04 12:21:48.000000 actuarialmath-0.0.7/src/actuarialmath/interest.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     6906 2023-06-04 12:26:59.000000 actuarialmath-0.0.7/src/actuarialmath/life.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    11663 2023-06-04 14:21:25.000000 actuarialmath-0.0.7/src/actuarialmath/lifetable.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     2706 2023-06-04 12:39:39.000000 actuarialmath-0.0.7/src/actuarialmath/lifetime.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    12048 2023-06-04 14:53:49.000000 actuarialmath-0.0.7/src/actuarialmath/mortalitylaws.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    12454 2023-06-04 15:08:44.000000 actuarialmath-0.0.7/src/actuarialmath/mthly.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    21134 2023-06-04 14:09:48.000000 actuarialmath-0.0.7/src/actuarialmath/policyvalues.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     8833 2023-06-04 13:33:45.000000 actuarialmath-0.0.7/src/actuarialmath/premiums.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    60668 2023-06-04 14:42:14.000000 actuarialmath-0.0.7/src/actuarialmath/recursion.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    11689 2023-06-04 14:13:35.000000 actuarialmath-0.0.7/src/actuarialmath/reserves.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    19575 2023-06-04 14:36:57.000000 actuarialmath-0.0.7/src/actuarialmath/selectlife.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     9499 2023-06-04 14:31:45.000000 actuarialmath-0.0.7/src/actuarialmath/sult.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     8390 2023-06-04 12:50:08.000000 actuarialmath-0.0.7/src/actuarialmath/survival.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     9937 2023-06-04 15:15:45.000000 actuarialmath-0.0.7/src/actuarialmath/udd.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     8112 2023-06-04 15:16:53.000000 actuarialmath-0.0.7/src/actuarialmath/woolhouse.py
-drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-05 21:40:58.475431 actuarialmath-0.0.7/src/actuarialmath.egg-info/
--rw-rw-r--   0 terence   (1000) terence   (1000)     4193 2023-06-05 21:40:58.000000 actuarialmath-0.0.7/src/actuarialmath.egg-info/PKG-INFO
--rw-rw-r--   0 terence   (1000) terence   (1000)      873 2023-06-05 21:40:58.000000 actuarialmath-0.0.7/src/actuarialmath.egg-info/SOURCES.txt
--rw-rw-r--   0 terence   (1000) terence   (1000)        1 2023-06-05 21:40:58.000000 actuarialmath-0.0.7/src/actuarialmath.egg-info/dependency_links.txt
--rw-rw-r--   0 terence   (1000) terence   (1000)       14 2023-06-05 21:40:58.000000 actuarialmath-0.0.7/src/actuarialmath.egg-info/top_level.txt
+drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-08 18:51:56.667060 actuarialmath-0.0.8/
+-rw-rw-r--   0 terence   (1000) terence   (1000)     1073 2023-05-29 19:44:46.000000 actuarialmath-0.0.8/LICENSE
+-rw-rw-r--   0 terence   (1000) terence   (1000)     4370 2023-06-08 18:51:56.667060 actuarialmath-0.0.8/PKG-INFO
+-rw-rw-r--   0 terence   (1000) terence   (1000)     4827 2023-06-08 18:15:03.000000 actuarialmath-0.0.8/README.md
+-rw-rw-r--   0 terence   (1000) terence   (1000)     3845 2023-06-08 18:21:02.000000 actuarialmath-0.0.8/index.rst
+-rw-rw-r--   0 terence   (1000) terence   (1000)      712 2023-06-08 18:51:24.000000 actuarialmath-0.0.8/pyproject.toml
+-rw-rw-r--   0 terence   (1000) terence   (1000)       38 2023-06-08 18:51:56.667060 actuarialmath-0.0.8/setup.cfg
+drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-08 18:51:56.663060 actuarialmath-0.0.8/src/
+drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-08 18:51:56.667060 actuarialmath-0.0.8/src/actuarialmath/
+-rw-rw-r--   0 terence   (1000) terence   (1000)        0 2023-05-25 13:19:02.000000 actuarialmath-0.0.8/src/actuarialmath/__init__.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     4942 2023-06-08 13:33:30.000000 actuarialmath-0.0.8/src/actuarialmath/actuarial.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    14876 2023-06-08 17:49:44.000000 actuarialmath-0.0.8/src/actuarialmath/annuity.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     9400 2023-06-08 15:51:43.000000 actuarialmath-0.0.8/src/actuarialmath/constantforce.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     3638 2023-06-04 15:05:12.000000 actuarialmath-0.0.8/src/actuarialmath/extrarisk.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     9482 2023-06-04 12:58:13.000000 actuarialmath-0.0.8/src/actuarialmath/fractional.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    21113 2023-06-08 18:01:14.000000 actuarialmath-0.0.8/src/actuarialmath/insurance.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     5973 2023-06-06 01:23:38.000000 actuarialmath-0.0.8/src/actuarialmath/interest.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     6906 2023-06-04 12:26:59.000000 actuarialmath-0.0.8/src/actuarialmath/life.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    12187 2023-06-08 17:34:26.000000 actuarialmath-0.0.8/src/actuarialmath/lifetable.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     2706 2023-06-04 12:39:39.000000 actuarialmath-0.0.8/src/actuarialmath/lifetime.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    12048 2023-06-04 14:53:49.000000 actuarialmath-0.0.8/src/actuarialmath/mortalitylaws.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    12454 2023-06-04 15:08:44.000000 actuarialmath-0.0.8/src/actuarialmath/mthly.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    21134 2023-06-04 14:09:48.000000 actuarialmath-0.0.8/src/actuarialmath/policyvalues.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     8833 2023-06-04 13:33:45.000000 actuarialmath-0.0.8/src/actuarialmath/premiums.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    60817 2023-06-08 13:24:50.000000 actuarialmath-0.0.8/src/actuarialmath/recursion.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    11689 2023-06-04 14:13:35.000000 actuarialmath-0.0.8/src/actuarialmath/reserves.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    19575 2023-06-04 14:36:57.000000 actuarialmath-0.0.8/src/actuarialmath/selectlife.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     7296 2023-06-08 13:41:59.000000 actuarialmath-0.0.8/src/actuarialmath/sult.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     8390 2023-06-04 12:50:08.000000 actuarialmath-0.0.8/src/actuarialmath/survival.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     9937 2023-06-04 15:15:45.000000 actuarialmath-0.0.8/src/actuarialmath/udd.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     8112 2023-06-04 15:16:53.000000 actuarialmath-0.0.8/src/actuarialmath/woolhouse.py
+drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-08 18:51:56.667060 actuarialmath-0.0.8/src/actuarialmath.egg-info/
+-rw-rw-r--   0 terence   (1000) terence   (1000)     4370 2023-06-08 18:51:56.000000 actuarialmath-0.0.8/src/actuarialmath.egg-info/PKG-INFO
+-rw-rw-r--   0 terence   (1000) terence   (1000)      913 2023-06-08 18:51:56.000000 actuarialmath-0.0.8/src/actuarialmath.egg-info/SOURCES.txt
+-rw-rw-r--   0 terence   (1000) terence   (1000)        1 2023-06-08 18:51:56.000000 actuarialmath-0.0.8/src/actuarialmath.egg-info/dependency_links.txt
+-rw-rw-r--   0 terence   (1000) terence   (1000)       60 2023-06-08 18:51:56.000000 actuarialmath-0.0.8/src/actuarialmath.egg-info/requires.txt
+-rw-rw-r--   0 terence   (1000) terence   (1000)       14 2023-06-08 18:51:56.000000 actuarialmath-0.0.8/src/actuarialmath.egg-info/top_level.txt
```

### Comparing `actuarialmath-0.0.7/LICENSE` & `actuarialmath-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.7/PKG-INFO` & `actuarialmath-0.0.8/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,74 @@
-Metadata-Version: 2.1
-Name: actuarialmath
-Version: 0.0.7
-Summary: A package for life contingent risks
-Author: Terence Lim
-Project-URL: Homepage, https://github.com/terence-lim/actuarialmath
-Project-URL: Bug Tracker, https://github.com/terence-lim/actuarialmath/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 actuarialmath - Life Contingent Risks with Python
 =================================================
 
-This package implements fundamental methods for modeling life contingent risks, and closely follows traditional topics covered in actuarial exams and standard texts such as the "Fundamentals of Actuarial Math - Long-term" exam syllabus by the Society of Actuaries, and "Actuarial Mathematics for Life Contingent Risks" by Dickson, Hardy and Waters.
+This Python package implements fundamental methods for modeling life contingent risks, and closely follows the coverage of traditional topics in actuarial exams and standard texts such as the "Fundamentals of Actuarial Math - Long-term" exam syllabus by the Society of Actuaries, and "Actuarial Mathematics for Life Contingent Risks" by Dickson, Hardy and Waters.
 
 Overview
 --------
 
 The package comprises three sets of classes, which:
 
-1. Implement general actuarial concepts
-   
-   a. Basic interest theory and probability laws
-   b. Survival functions, future lifetimes and fractional ages
-   c. Insurance, annuity, premiums, policy values, and reserves calculations
-      
-2. Adjust results for
-   
-   a. Extra risks
-   b. 1/mthly payments using UDD or Woolhouse approaches
-      
-3. Specify and load a particular form of assumptions
-   
-   a. Life table, select life table, or standard ultimate life table
-   b. Mortality laws, such as constant force of maturity, beta and uniform distributions, or Makeham's and Gompertz's laws
-   c. Recursion inputs
+1. Implement general actuarial methods
+
+   - Basic interest theory and probability laws
+
+   - Survival functions, expected future lifetimes and fractional ages
+
+   - Insurance, annuity, premiums, policy values, and reserves calculations
+
+
+2. Specify and load a particular form of assumptions
+
+   - Life table, select life table, or standard ultimate life table
+
+   - Mortality laws, such as constant force of maturity, beta and uniform distributions, or Makeham's and Gompertz's laws
+
+   - Recursion inputs
+
+3. Adjust results for
+
+   - Extra mortality risks
+
+   - 1/mthly payment frequency using UDD or Woolhouse approaches
 
 Quick Start
 -----------
 
 1. ``pip install actuarialmath``
-2. Select a suitable subclass to initialize with your actuarial assumptions, such as `MortalityLaws` (or a special law like `ConstantForce`), `LifeTable`, `SULT`, `SelectTable` or `Recursion`.
-3. Call appropriate methods to compute intermediate or final results, or to `solve` parameter values implicitly.
-4. If needed, adjust the answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes.
+   
+   - also requires `numpy`, `scipy`, `matplotlib` and `pandas`.
+     
+2. Start Python (version >= 3.10) or Jupyter-notebook
+
+   - Select a suitable subclass to initialize with your actuarial assumptions, such as `MortalityLaws` (or a special law like `ConstantForce`), `LifeTable`, `SULT`, `SelectLife` or `Recursion`.
+      
+   - Call appropriate methods to compute intermediate or final results, or to `solve` parameter values implicitly.
+
+   - If needed, adjust the answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes.
 
 Examples
 --------
 
 ::
 
   # SOA FAM-L sample question 5.7
   from actuarialmath.recursion import Recursion
   from actuarialmath.woolhouse import Woolhouse
   # initialize Recursion class with actuarial inputs
-  life = Recursion().set_interest(i=0.04)\\
-                    .set_A(0.188, x=35)\\
-                    .set_A(0.498, x=65)\\
+  life = Recursion().set_interest(i=0.04)\
+                    .set_A(0.188, x=35)\
+                    .set_A(0.498, x=65)\
                     .set_p(0.883, x=35, t=30)
   # modfy the standard results with Woolhouse mthly approximation
   mthly = Woolhouse(m=2, life=life, three_term=False)
   # compute the desired temporary annuity value
   print(1000 * mthly.temporary_annuity(35, t=30)) #   solution = 17376.7
 
-::  
+::
 
   # SOA FAM-L sample question 7.20
   from actuarialmath.sult import SULT   # use Standard Ultimate Life Table
   from actuarialmath.policyvalues import Contract
   life = SULT()
   # compute the required FPT policy value
   S = life.FPT_policy_value(35, t=1, b=1000)  # is always 0 in year 1!
@@ -80,20 +79,19 @@
                       renewal_premium=.04,
                       renewal_policy=30)
   # compute gross premium using the equivalence principle
   G = life.gross_premium(A=life.whole_life_insurance(35), **contract.premium_terms)
   # compute the required policy value
   R = life.gross_policy_value(35, t=1, contract=contract.set_contract(premium=G))
   print(R-S)   # solution = -277.19
-   
 
 Resources
 ---------
 
 1. `Colab <https://colab.research.google.com/drive/1TcNr1x5HbT2fF3iFMYGXdN_cvRKiSua4?usp=sharing>`_ or `Jupyter notebook <https://terence-lim.github.io/notes/faml.ipynb>`_, to solve all sample SOA FAM-L exam questions
 
 2. `Online tutorial <https://terence-lim.github.io/actuarialmath-tutorial/>`_, or `download pdf <https://terence-lim.github.io/notes/actuarialmath-tutorial.pdf>`_
 
-3. `Code documentation <https://terence-lim.github.io/actuarialmath-docs/>`_
+3. `Code documentation <https://actuarialmath.readthedocs.io/en/latest/>`_
 
 4. `Github repo <https://github.com/terence-lim/actuarialmath.git>`_ and `issues <https://github.com/terence-lim/actuarialmath/issues>`_
```

### Comparing `actuarialmath-0.0.7/README.md` & `actuarialmath-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 # Introduction
 
 __actuarialmath -- Life Contingent Risks with Python__
 
-This package implements fundamental methods for modeling life contingent risks, and closely follows traditional topics covered in actuarial exams and standard texts such as the "Fundamentals of Actuarial Math - Long-term" exam syllabus by the Society of Actuaries, and "Actuarial Mathematics for Life Contingent Risks" by Dickson, Hardy and Waters.
+This Python package implements fundamental methods for modeling life contingent risks, and closely follows the coverage of traditional topics in actuarial exams and standard texts such as the "Fundamentals of Actuarial Math - Long-term" exam syllabus by the Society of Actuaries, and "Actuarial Mathematics for Life Contingent Risks" by Dickson, Hardy and Waters.
 The resources listed below should be helpful for getting started. The code chunks in this complete [Colab](https://colab.research.google.com/drive/1TcNr1x5HbT2fF3iFMYGXdN_cvRKiSua4?usp=sharing), or [Jupyter notebook](https://terence-lim.github.io/notes/faml.ipynb), demonstrate how to solve each of the sample FAM-L exam questions released by the SOA.
 
-The actuarial concepts, as shown in this graphic, are introduced and modeled hierarchically, and realized by corresponding derivations of Python classes. 
+The actuarial concepts, as shown in this graphic, are introduced and modeled hierarchically, and realized by corresponding derivations of Python classes.
 
 ![classes](FAM-L.png)
 
 ## Quick Start
 
 1. `pip install actuarialmath`
-2. Select a suitable subclass to initialize with your actuarial assumptions, such as `MortalityLaws` (or a special law like `ConstantForce`), `LifeTable`, `SULT`, `SelectTable` or `Recursion`.
-3. Call appropriate methods to compute intermediate or final results, or to `solve` parameter values implicitly.
-4. If needed, adjust the answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes.
+
+   - also requires `numpy`, `scipy`, `matplotlib` and `pandas`.
+
+
+2. Start Python (version >= 3.10) or Jupyter-notebook
+
+
+   - Select and import a suitable subclass to initialize with your actuarial assumptions, such as `MortalityLaws` (or a special law like `ConstantForce`), `LifeTable`, `SULT`, `SelectLife` or `Recursion`.
+
+   - Call appropriate methods to compute intermediate or final results, or to `solve` parameter values implicitly.
+
+   - If needed, adjust the answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes.
 
 ## Examples
 
 __SOA FAM-L sample question 5.7__: 
 
 Given $A_{35} = 0.188$, $A_{65} = 0.498$, $S_{35}(30) = 0.883$, calculate the EPV of a temporary annuity $\ddot{a}^{(2)}_{35:\overline{30|}}$ paid half-yearly using the Woolhouse approximation.
 
@@ -71,15 +80,15 @@
 
 ## Resources
 
 1. [Colab](https://colab.research.google.com/drive/1TcNr1x5HbT2fF3iFMYGXdN_cvRKiSua4?usp=sharing) or [Jupyter notebook](https://terence-lim.github.io/notes/faml.ipynb), to solve all sample SOA FAM-L exam questions
 
 2. [Online tutorial](https://terence-lim.github.io/actuarialmath-tutorial/), or [download pdf](https://terence-lim.github.io/notes/actuarialmath-tutorial.pdf)
 
-3. [Code documentation](https://terence-lim.github.io/actuarialmath-docs/)
+3. [Code documentation](https://actuarialmath.readthedocs.io/en/latest/)
 
 4. [Github repo](https://github.com/terence-lim/actuarialmath.git) and [issues](https://github.com/terence-lim/actuarialmath/issues)
 
 
 
 ## Sources
```

### Comparing `actuarialmath-0.0.7/index.rst` & `actuarialmath-0.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,88 @@
+Metadata-Version: 2.1
+Name: actuarialmath
+Version: 0.0.8
+Summary: A package for actuarial math and life contingent risks
+Author: Terence Lim
+Project-URL: Homepage, https://terence-lim.github.io/actuarialmath-tutorial
+Project-URL: Bug Tracker, https://github.com/terence-lim/actuarialmath/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 actuarialmath - Life Contingent Risks with Python
 =================================================
 
-This package implements fundamental methods for modeling life contingent risks, and closely follows traditional topics covered in actuarial exams and standard texts such as the "Fundamentals of Actuarial Math - Long-term" exam syllabus by the Society of Actuaries, and "Actuarial Mathematics for Life Contingent Risks" by Dickson, Hardy and Waters.
+This Python package implements fundamental methods for modeling life contingent risks, and closely follows the coverage of traditional topics in actuarial exams and standard texts such as the "Fundamentals of Actuarial Math - Long-term" exam syllabus by the Society of Actuaries, and "Actuarial Mathematics for Life Contingent Risks" by Dickson, Hardy and Waters.
 
 Overview
 --------
 
 The package comprises three sets of classes, which:
 
-1. Implement general actuarial concepts
-   
-   a. Basic interest theory and probability laws
-   b. Survival functions, future lifetimes and fractional ages
-   c. Insurance, annuity, premiums, policy values, and reserves calculations
-      
-2. Adjust results for
-   
-   a. Extra risks
-   b. 1/mthly payments using UDD or Woolhouse approaches
-      
-3. Specify and load a particular form of assumptions
-   
-   a. Life table, select life table, or standard ultimate life table
-   b. Mortality laws, such as constant force of maturity, beta and uniform distributions, or Makeham's and Gompertz's laws
-   c. Recursion inputs
+1. Implement general actuarial methods
+
+   - Basic interest theory and probability laws
+
+   - Survival functions, expected future lifetimes and fractional ages
+
+   - Insurance, annuity, premiums, policy values, and reserves calculations
+
+
+2. Specify and load a particular form of assumptions
+
+   - Life table, select life table, or standard ultimate life table
+
+   - Mortality laws, such as constant force of maturity, beta and uniform distributions, or Makeham's and Gompertz's laws
+
+   - Recursion inputs
+
+3. Adjust results for
+
+   - Extra mortality risks
+
+   - 1/mthly payment frequency using UDD or Woolhouse approaches
 
 Quick Start
 -----------
 
 1. ``pip install actuarialmath``
-2. Select a suitable subclass to initialize with your actuarial assumptions, such as `MortalityLaws` (or a special law like `ConstantForce`), `LifeTable`, `SULT`, `SelectTable` or `Recursion`.
-3. Call appropriate methods to compute intermediate or final results, or to `solve` parameter values implicitly.
-4. If needed, adjust the answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes.
+   
+   - also requires `numpy`, `scipy`, `matplotlib` and `pandas`.
+     
+2. Start Python (version >= 3.10) or Jupyter-notebook
+
+   - Select a suitable subclass to initialize with your actuarial assumptions, such as `MortalityLaws` (or a special law like `ConstantForce`), `LifeTable`, `SULT`, `SelectLife` or `Recursion`.
+      
+   - Call appropriate methods to compute intermediate or final results, or to `solve` parameter values implicitly.
+
+   - If needed, adjust the answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes.
 
 Examples
 --------
 
 ::
 
   # SOA FAM-L sample question 5.7
   from actuarialmath.recursion import Recursion
   from actuarialmath.woolhouse import Woolhouse
   # initialize Recursion class with actuarial inputs
-  life = Recursion().set_interest(i=0.04)\\
-                    .set_A(0.188, x=35)\\
-                    .set_A(0.498, x=65)\\
+  life = Recursion().set_interest(i=0.04)\
+                    .set_A(0.188, x=35)\
+                    .set_A(0.498, x=65)\
                     .set_p(0.883, x=35, t=30)
   # modfy the standard results with Woolhouse mthly approximation
   mthly = Woolhouse(m=2, life=life, three_term=False)
   # compute the desired temporary annuity value
   print(1000 * mthly.temporary_annuity(35, t=30)) #   solution = 17376.7
 
-::  
+::
 
   # SOA FAM-L sample question 7.20
   from actuarialmath.sult import SULT   # use Standard Ultimate Life Table
   from actuarialmath.policyvalues import Contract
   life = SULT()
   # compute the required FPT policy value
   S = life.FPT_policy_value(35, t=1, b=1000)  # is always 0 in year 1!
@@ -66,20 +93,19 @@
                       renewal_premium=.04,
                       renewal_policy=30)
   # compute gross premium using the equivalence principle
   G = life.gross_premium(A=life.whole_life_insurance(35), **contract.premium_terms)
   # compute the required policy value
   R = life.gross_policy_value(35, t=1, contract=contract.set_contract(premium=G))
   print(R-S)   # solution = -277.19
-   
 
 Resources
 ---------
 
 1. `Colab <https://colab.research.google.com/drive/1TcNr1x5HbT2fF3iFMYGXdN_cvRKiSua4?usp=sharing>`_ or `Jupyter notebook <https://terence-lim.github.io/notes/faml.ipynb>`_, to solve all sample SOA FAM-L exam questions
 
 2. `Online tutorial <https://terence-lim.github.io/actuarialmath-tutorial/>`_, or `download pdf <https://terence-lim.github.io/notes/actuarialmath-tutorial.pdf>`_
 
-3. `Code documentation <https://terence-lim.github.io/actuarialmath-docs/>`_
+3. `Code documentation <https://actuarialmath.readthedocs.io/en/latest/>`_
 
 4. `Github repo <https://github.com/terence-lim/actuarialmath.git>`_ and `issues <https://github.com/terence-lim/actuarialmath/issues>`_
```

### Comparing `actuarialmath-0.0.7/pyproject.toml` & `actuarialmath-0.0.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "actuarialmath"
-version = "0.0.7"
+version = "0.0.8" # "0.0.98" 
 authors = [
   { name="Terence Lim"},
 ]
-description = "A package for life contingent risks"
+description = "A package for actuarial math and life contingent risks"
 readme = "index.rst"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+dependencies = [
+  "matplotlib==3.7.1",
+  "numpy==1.24.3",
+  "pandas==2.0.2",
+  "scipy==1.10.1",
+]
+
 [project.urls]
-"Homepage" = "https://github.com/terence-lim/actuarialmath"
+"Homepage" = "https://terence-lim.github.io/actuarialmath-tutorial"
 "Bug Tracker" = "https://github.com/terence-lim/actuarialmath/issues"
```

### Comparing `actuarialmath-0.0.7/src/actuarialmath/actuarial.py` & `actuarialmath-0.0.8/src/actuarialmath/actuarial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Base class for actuarial math, with common utility functions and constants
+"""Define base class for actuarial math, with utility helpers and constants
 
 MIT License. Copyright (c) 2022-2023 Terence Lim
 """
 import math
 import numpy as np
 import scipy
 from typing import Callable, Any, Tuple, List
@@ -73,58 +73,58 @@
           x : value to compute derivative at
         """
         return scipy.misc.derivative(fun, x0=x, dx=1)
 
     @staticmethod
     def solve(fun: Callable[[float], float], target: float, 
               grid: float | Tuple | List, mad: bool = False) -> float:
-        """Solve for the root of, or parameter value that minimizes, an equation
+        """Solve for the root of, or parameter value that minimizes, a function
 
         Args:
           fun : function to compute output given input values
           target : target value of function output
-          grid : initial guesses or bounds
-          root : whether solve root, or minimize absolute difference (False)
+          grid : initial range of guesses
+          root : whether solve root (True), or minimize absolute deviation (False)
 
         Returns:
           value s.t. output of function fun(value) ~ target
         """
         if mad:   # minimize absolute difference
             f = lambda t: abs(fun(t) - target)
             return scipy.optimize.minimize_scalar(f, grid).x    
         else:     # solve root
             f = lambda x: fun(x) - target
             if isinstance(grid, (list, tuple)):
                 grid = min([(abs(f(x)), x)    # guess can be list of guesses
                             for x in np.linspace(min(grid), max(grid), 5)])[1]
             output = scipy.optimize.fsolve(f, [grid], full_output=True)
-            fun(output[0][0])  # execute with final answer in case want side effects
+            fun(output[0][0])   # call again with final in case want side effect
             return output[0][0]
 
     def add_term(self, t: int, n: int) -> int:
         """Add two terms, either term may be Whole Life
 
         Args:
           t : first term to add
           n : second term to add
         """
         if t == self.WHOLE or n == self.WHOLE:
             return self.WHOLE  # adding any term to WHOLE is still WHOLE
         return t + n
 
     def max_term(self, x: int, t: int, u: int = 0) -> int:
-        """Adjust term if adding term and deferral periods to (x) exceeds maxage
+        """Decrease term t if deferral period u to (x) exceeds maxage
 
         Args:
           x : age
           t : term of insurance or annuity, after deferral period
           u : term deferred
 
         Returns:
-          value of term t adjusted by deferral and maxage s.t. does not exceed maxage
+          value of term t adjusted by deferral and maxage s.t. maxage not exceeded
         """
         if t < 0 or x + t + u > self._MAXAGE:
             return self._MAXAGE - (x + u)
         return t
 
 if __name__ == "__main__":
     actuarial = Actuarial()
```

### Comparing `actuarialmath-0.0.7/src/actuarialmath/annuity.py` & `actuarialmath-0.0.8/src/actuarialmath/annuity.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
           benefit : benefit as a function of age and year
           discrete : annuity due (True) or continuous (False)
         """
         t = self.max_term(x+s+u, t=t)
         if discrete:
             a = sum([benefit(x+s, k) * self.interest.v_t(k) 
                      * self.p_x(x, s=s, t=k) for k in range(u, t+u)])
-        else:   # use continous first principles
+        else:   # use continuous first principles
             Y = lambda t: (benefit(x+s, t+u) * self.interest.v_t(t+u) 
                            * self.S(x, 0, t=t+u))
             a = self.integral(Y, 0, t)
         return a
 
 
     def immediate_annuity(self, x: int, s: int = 0, t: int = Insurance.WHOLE, 
@@ -52,43 +52,47 @@
                 - 1 + self.E_x(x, s=s, t=t)) * b
     
     def annuity_twin(self, A: float, discrete: bool = True) -> float:
         """Returns annuity from its WL or Endowment Insurance twin"
 
         Args:
           A : cost of insurance
-          discrete : discrete/annuity due (True) or continous (False)
+          discrete : discrete/annuity due (True) or continuous (False)
         """
         interest = (self.interest.d if discrete else self.interest.delta)
-        return ((1-A) / interest) if interest else 0 # undefined for 0 interest
+        return ((1 - A) / interest) if interest else 1 - A
 
     def insurance_twin(self, a: float, moment: int = 1, 
                        discrete: bool = True) -> float:
         """Returns WL or Endowment Insurance twin from annuity
 
         Args:
           a : cost of annuity
-          discrete : discrete/annuity due (True) or continous (False)
+          discrete : discrete/annuity due (True) or continuous (False)
         """
         assert moment in [1]
-        return 1 - a*(self.interest.d if discrete else self.interest.delta)
+        interest = (self.interest.d if discrete else self.interest.delta)
+        return 1 - a*interest
   
     def annuity_variance(self, A2: float, A1: float, b: float = 1.,
                          discrete: bool = True) -> float:
         """Compute variance from WL or endowment insurance twin
 
         Args:
           A2 : second moment of insurance factor
           A1 : first moment of insurance factor
           b : annuity benefit amount
-          discrete : discrete/annuity due (True) or continous (False)
+          discrete : discrete/annuity due (True) or continuous (False)
         """
-        return (b**2 * self.insurance_variance(A2=A2, A1=A1)
-                / (self.interest.d if discrete else self.interest.delta)**2)
-        
+        interest = (self.interest.d if discrete else self.interest.delta)
+        if interest == 0:
+            return b**2 * self.insurance_variance(A2=A2, A1=A1)
+        else:
+            return (b**2 * self.insurance_variance(A2=A2, A1=A1) / interest**2)
+
     def whole_life_annuity(self, x: int, s: int = 0, b: int = 1, 
                            variance: bool = False, 
                            discrete: bool = True) -> float:
         """Whole life annuity: a_x
 
         Args:
           x : age of selection
@@ -98,16 +102,20 @@
           discrete : annuity due (True) or continuous (False)
         """
         interest = self.interest.d if discrete else self.interest.delta
         if variance:  # short cut for variance of whole life
             A1 = self.whole_life_insurance(x, s=s, moment=1, discrete=discrete)
             A2 = self.whole_life_insurance(x, s=s, moment=2, discrete=discrete)
             return self.annuity_variance(A2=A2, A1=A1, discrete=discrete, b=b)
-        A = self.whole_life_insurance(x, s=s, discrete=discrete)
-        return b * (1 - A) / interest
+        if interest > 0:
+            A = self.whole_life_insurance(x, s=s, discrete=discrete)
+            return b * (1 - A) / interest if interest > 0 else b * (1 - A)
+        else:  # when interest=1, annuity is expected life time (+1 if discrete)
+            return discrete + self.e_x(x=x, s=s, curtate=discrete)
+
             
     def temporary_annuity(self, x: int, s: int = 0, t: int = Insurance.WHOLE, 
                           b: int = 1, variance: bool = False, 
                           discrete: bool = True) -> float:
         """Temporary life annuity: a_x:t
 
         Args:
@@ -206,37 +214,42 @@
 
         Args:
           x : age of selection
           prob : desired probability threshold
           discrete : annuity due (True) or continuous (False)
         """
         assert prob < 1.0
-        t = Insurance.solve(lambda t: self.S(x, 0, t), target=1-prob, grid=25)
+        t = self.solve(lambda t: self.S(x, 0, t), target=1-prob, grid=25)
         return math.floor(t) if discrete else t   # opposite of insurance
 
     def Y_from_t(self, t: float, discrete: bool = True) -> float:
         """PV of insurance payment Y(t), given T_x (or K_x if discrete)
 
         Args:
           t : year of death
           discrete : annuity due (True) or continuous (False)
         """
+        if self.interest.delta == 0.:  # return number of payments if interest=0
+            return math.floor(t) + 1 if discrete else t
         if discrete:
             return (1 - self.interest.v_t(math.floor(t) + 1)) / self.interest.d
         else:
             return (1 - self.interest.v_t(t)) / self.interest.delta
 
     def Y_to_t(self, Y: float) -> float:
         """T_x  s.t. PV of annuity payments is Y
 
         Args:
           Y : Present value of benefits paid
         """
-        t = math.log(1 - self.interest.delta * Y) / math.log(self.interest.v)
-        return t
+        if self.interest.v == 0.:
+            return Y
+        else:
+            return math.log(1 - self.interest.delta*Y) / math.log(self.interest.v)
+
 
     def Y_from_prob(self, x: int, prob: float, discrete: bool = True) -> float:
         """Percentile of annuity PV r.v. Y, given probability
 
         Args:
           x : age initially insured
           prob : desired probability threshold
@@ -327,57 +340,40 @@
                      if title is None else title)
         ax.set_ylabel(f"$Y({K}_x)$", color=color)
         ax.set_xlabel(f"${K}_x$")
         plt.tight_layout()
         return Y
 
 if __name__ == "__main__":
+    from actuarialmath.policyvalues import Contract
     from actuarialmath.sult import SULT
-    life = SULT()
-    life.Y_plot(x=65, T=life.Y_t(x=65, prob=0.5))
+    contract = Contract(premium=0, benefit=10000)  # premiums=0 after t=10
+    L = SULT().gross_policy_value(35, contract=contract)
+    V = SULT().set_interest(i=0).gross_policy_value(35, contract=contract) # 10000
 
+if False:
     
+    from actuarialmath.sult import SULT
+    life = SULT()
+    x = 20
+    life.Y_plot(x=x, T=life.Y_t(x=x, prob=0.5))
+
     life = Annuity().set_interest(delta=0.06)\
                     .set_survival(mu=lambda *x: 0.04)
-    prob = 0.8
+    prob = 0.5
     x = 0
     discrete = False
     t = life.Y_t(0, prob, discrete=discrete)
+    life.Y_plot(x=20, T=t, discrete=discrete)
     Y = life.Y_from_prob(x, prob=prob, discrete=discrete)
     print(t, life.Y_to_t(Y))
     print(Y, life.Y_from_t(t, discrete=discrete))
     print(prob, life.Y_to_prob(x, Y=Y))
-    life.Y_plot(x=0, T=t, discrete=discrete)
-
+    
+if False:
     print("SOA Question 5.6:  (D) 1200")
     life = Annuity().set_interest(i=0.05)
     var = life.annuity_variance(A2=0.22, A1=0.45)
     mean = life.annuity_twin(A=0.45)
     print(life.portfolio_percentile(mean=mean, variance=var, prob=.95, N=100))
     print()
     
-    print("Other usage")
-    mu = 0.04
-    delta = 0.06
-    life = Annuity().set_interest(delta=delta)\
-                    .set_survival(mu=lambda *x: mu)
-    print(life.temporary_annuity(50, t=20, b=10000, discrete=False))
-    print(life.endowment_insurance(50, t=20, b=10000, discrete=False))
-    print(life.E_x(50, t=20))
-    print(life.whole_life_annuity(50, b=10000, discrete=False))
-    print(life.whole_life_annuity(70, b=10000, discrete=False))
-
-    mu = 0.07
-    delta = 0.02
-    life = Annuity().set_interest(delta=delta)\
-                    .set_survival(mu=lambda *x: mu)
-    print(life.whole_life_annuity(0, discrete=False) * 30)   # 333.33
-    print(life.temporary_annuity(0, t=10, discrete=False) * 30)  # 197.81
-    print(life.interest.annuity(5, m=0))  # 4.7581
-    print(life.deferred_annuity(0, u=5, discrete=False)) # 7.0848
-    print(life.certain_life_annuity(0, u=5, discrete=False))  # 11.842
-
-    mu = 0.02
-    delta = 0.05
-    life = Annuity().set_interest(delta=delta)\
-                    .set_survival(mu=lambda *x: mu)
-    print(life.decreasing_annuity(0, t=5, discrete=False))  # 6.94
```

### Comparing `actuarialmath-0.0.7/src/actuarialmath/constantforce.py` & `actuarialmath-0.0.8/src/actuarialmath/constantforce.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,16 @@
         """
         if variance:  # short cut for variance of temporary life annuity
             A1 = self.whole_life_insurance(x, s=s, discrete=discrete)
             A2 = self.whole_life_insurance(x, s=s, moment=2, discrete=discrete)
             return (b**2 * (A2 - A1**2) /
                     (self.interest.d if discrete else self.interest.delta)**2)
         if not discrete:
-            return (1. / (self.mu_ + self.interest.delta)) * b
+            den = self.mu_ + self.interest.delta
+            return (1. / den) * b if den > 0 else math.inf
         return super().whole_life_annuity(x, s=s, b=b, discrete=discrete)
 
     def temporary_annuity(self, x: int, s: int = 0, t: int = MortalityLaws.WHOLE,
                           b: int = 1, variance: bool = False,
                           discrete: bool = True) -> float:
         """Shortcut for temporary life annuity: does not depend on age x
 
@@ -125,15 +126,15 @@
           s : years after selection
           b : amount of benefit
           moment : compute first or second moment
           discrete : benefit paid year-end (True) or moment of death (False)
         """
         if moment > 0 and not discrete:
             delta = moment * self.interest.delta   # multiply force of interest
-            return (self.mu_ / (self.mu_ + delta))
+            return self.mu_ / (self.mu_ + delta) if self.mu_ > 0 else 0.
         return super().whole_life_insurance(x, s=s, moment=moment, b=b,
                                             discrete=discrete)
 
     def term_insurance(self, x: int, s: int = 0, t: int = 1, b: int = 1,
                        moment: int = 1, discrete: bool = True) -> float:
         """Shortcut for APV of term life: does not depend on age x
```

### Comparing `actuarialmath-0.0.7/src/actuarialmath/extrarisk.py` & `actuarialmath-0.0.8/src/actuarialmath/extrarisk.py`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.7/src/actuarialmath/fractional.py` & `actuarialmath-0.0.8/src/actuarialmath/fractional.py`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.7/src/actuarialmath/insurance.py` & `actuarialmath-0.0.8/src/actuarialmath/insurance.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         """Compute variance of insurance given moments and benefit
 
         Args:
           A2 : second moment of insurance r.v.
           A1 : first moment of insurance r.v.
           b : benefit amount
         """
-        return b**2 * (A2 - A1**2)
+        return b**2 * max(0, A2 - A1**2)
 
     def whole_life_insurance(self, x: int, s: int = 0, moment: int = 1, 
                              b: int = 1, discrete: bool = True) -> float:
         """Whole life insurance: A_x
 
         Args:
           x : age of selection
@@ -207,15 +207,15 @@
 
         Args:
           x : age initially insured
           prob : desired probability threshold
           discrete : benefit paid year-end (True) or moment of death (False)
         """
         assert prob < 1.0
-        t = Insurance.solve(lambda t: self.S(x, 0, t), target=prob, grid=50)
+        t = self.solve(lambda t: self.S(x, 0, t), target=prob, grid=50)
         return math.floor(t) if discrete else t    # opposite of annuity
 
     def Z_from_t(self, t: float, discrete: bool = True) -> float:
         """PV of insurance payment Z(t), given T_x (or K_x if discrete)
 
         Args:
           t : year of death
```

### Comparing `actuarialmath-0.0.7/src/actuarialmath/interest.py` & `actuarialmath-0.0.8/src/actuarialmath/interest.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 import math
 import numpy as np
 import pandas as pd
 from typing import Callable
 from actuarialmath.actuarial import Actuarial
 
 class Interest(Actuarial):
-    """Convert between nominal, discount, continously-compounded and 1/m'thly rates,
-    and compute value of annuity certain
+    """Converts interest rates, and computes value of annuity certain
     
     Args:
       i : assumed annual interest rate
       d : or assumed discount rate
       v : or assumed discount factor
       delta : or assumed continuously compounded interest rate
       v_t : or assumed discount rate as a function of time
```

### Comparing `actuarialmath-0.0.7/src/actuarialmath/life.py` & `actuarialmath-0.0.8/src/actuarialmath/life.py`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.7/src/actuarialmath/lifetable.py` & `actuarialmath-0.0.8/src/actuarialmath/lifetable.py`

 * *Files 3% similar despite different names*

```diff
@@ -220,26 +220,35 @@
         """
         denom = self.l_x(x, s=s)
         if denom and x+s+t <= self._MAXAGE:
             return self.d_x(x, s=s+u, t=t) / self.l_x(x, s=s)
         else:
             return 1     # the only certainty in life
 
-    def e_x(self, x: int, s: int = 0, n: int = Reserves.WHOLE) -> float:
+    def e_x(self, x: int, s: int = 0, n: int = Reserves.WHOLE,
+            curtate: bool = True, moment: int = 1) -> float:
         """Expected curtate lifetime from sum of lives in table
 
         Args:
           x : age of selection
           s : years after selection
           n : future lifetime limited at n years
+          curtate : whether curtate (True) or complete (False) expectations
+          moment : whether to compute first (1) or second (2) moment
+
         """
-        # E[K_x] = sum([self.p(x, k+1) for k in range(n)])
-        n = min(self._MAXAGE - x, n)
-        e = sum([self.l(x+1+s) for s in range(n)]) # since s_p_x = l_x+s / l_x
-        return e
+        if moment == 1:
+            # E[K_x] = sum([self.p(x, k+1) for k in range(n)])
+            n = min(self._MAXAGE - x, n) if n > 0 else self._MAXAGE
+            # approximate complete by UDD between integer age recursion
+            e = sum([(1 - curtate)*(self.l(x, s=s+t) - self.l(x, s=s+t+1))*0.5
+                     + self.l(x, s=s+t+1) for t in range(n)])  # s_p_x = l_x+s/l_x
+            return e / self.l(x, s=0)
+        else:
+            return super().e_x(x=x, s=s, n=n, curtate=curtate, moment=moment)
 
     def E_x(self, x: int, s: int = 0, t: int = 1, moment: int = 1) -> float:
         """Pure Endowment from life table and interest rate
 
         Args:
           x : age of selection
           s : years after selection
```

### Comparing `actuarialmath-0.0.7/src/actuarialmath/lifetime.py` & `actuarialmath-0.0.8/src/actuarialmath/lifetime.py`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.7/src/actuarialmath/mortalitylaws.py` & `actuarialmath-0.0.8/src/actuarialmath/mortalitylaws.py`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.7/src/actuarialmath/mthly.py` & `actuarialmath-0.0.8/src/actuarialmath/mthly.py`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.7/src/actuarialmath/policyvalues.py` & `actuarialmath-0.0.8/src/actuarialmath/policyvalues.py`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.7/src/actuarialmath/premiums.py` & `actuarialmath-0.0.8/src/actuarialmath/premiums.py`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.7/src/actuarialmath/recursion.py` & `actuarialmath-0.0.8/src/actuarialmath/recursion.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
       - 'a' : deferred, temporary or whole life annuity of t years, and moments
     """
 
     def __init__(self, depth: int = 3, verbose: bool = True, **kwargs):
         super().__init__(**kwargs)
         self.db = {}
         self.maxdepth = depth
-        Blog._verbose = verbose
+        _Blog._verbose = verbose
 
     #
     # helpers to store given input values
     #
     def db_key(self, *args, **kwargs) -> Tuple:
         """Generate a unique key representing values of given arguments"""
         assert args and kwargs
@@ -94,39 +94,39 @@
             return 0
         if t < 0:
             return 1
         if u > 0:
             pu = self._p_x(x, s=s, t=u, depth=depth-1) #1-abs(depth))
             qt = self.get_q(x, s=s+u, t=t)
             if pu is not None and qt is not None:
-                self.blog(Blog.q(x=x, s=s, t=t, u=u), '=',
-                          Blog.p(x=x, s=s, t=u), '*', Blog.q(x=x, s=s+u, t=t),
+                self.blog(_Blog.q(x=x, s=s, t=t, u=u), '=',
+                          _Blog.p(x=x, s=s, t=u), '*', _Blog.q(x=x, s=s+u, t=t),
                           depth=depth, rule="defer mortality")
                 return pu * qt        # (1) u_p_x * t_q_x+u
             qu = self.get_q(x, s=s, t=u)
             qt = self.get_q(x, s=s, t=u+t)
             if qu is not None and qt is not None:
-                self.blog(Blog.q(x=x, s=s, t=t, u=u), '=',
-                          Blog.q(x=x, s=s, t=t+u), '-', Blog.q(x=x, s=s, t=u),
+                self.blog(_Blog.q(x=x, s=s, t=t, u=u), '=',
+                          _Blog.q(x=x, s=s, t=t+u), '-', _Blog.q(x=x, s=s, t=u),
                           depth=depth, rule="limit mortality")
                 return qt - qu        # (2) u+t_q_x - u_q_x
         if depth <= 0:
             return None
         pu = self._p_x(x, s=s, t=u, depth=depth-1)
         pt = self._p_x(x, s=s, t=u+t, depth=depth-1)
         if pu is not None and pt is not None:
-            self.blog(Blog.q(x=x, s=s, t=t, u=u), '=',
-                      Blog.p(x=x, s=s, t=u), '-', Blog.p(x=x, s=s, t=t+u),
+            self.blog(_Blog.q(x=x, s=s, t=t, u=u), '=',
+                      _Blog.p(x=x, s=s, t=u), '-', _Blog.p(x=x, s=s, t=t+u),
                       depth=depth, rule="complement survival")
             return pu - pt            # (3) u_p_x - u+t_p_x
 
 
     def q_x(self, x: int, s: int = 0, t: int = 1, u: int = 0) -> float:
-        self.blog = Blog("Mortality",
-                         Blog.q(x=x, s=s, t=t, u=u),
+        self.blog = _Blog("Mortality",
+                         _Blog.q(x=x, s=s, t=t, u=u),
                          levels=self.maxdepth)
         """Compute mortality rate by calling recursion helper"""
         q = self._q_x(x, s=s, t=t, u=u, depth=self.maxdepth)
         if q is not None:
             print(self.blog, end='')
         return q
 
@@ -162,97 +162,97 @@
     def _p_x(self, x: int, s: int = 0, t: int = 1, depth: int = 1) -> float:
         """Helper to compute survival from recursive and alternate formulas"""
         found = self.get_p(x, s=s, t=t)
         if found is not None:
             return found
         found = self.get_q(x, s=s, t=t)  
         if found is not None:
-            self.blog(Blog.p(x=x, s=s, t=t), '= 1 -', Blog.q(x=x, s=s, t=t),
+            self.blog(_Blog.p(x=x, s=s, t=t), '= 1 -', _Blog.q(x=x, s=s, t=t),
                       depth=depth, rule='complement of mortality')
             return 1 - found  # (1) complement of q_x
         if depth <= 0:
             return None
         
         # (2a) inverse chain rule: p_x(t) = p_x-1(t+1) / p_x-1 
         found = self._p_x(x, s=s-1, t=t+1, depth=depth-1)
         p = self._p_x(x, s=s-1, t=1, depth=1-abs(depth))
         if found is not None and p is not None:
-            self.blog(Blog.p(x=x, s=s, t=t), '=',
-                      Blog.p(x=x, s=s-1, t=t+1), '/', Blog.p(x=x, s=s-1, t=1),
+            self.blog(_Blog.p(x=x, s=s, t=t), '=',
+                      _Blog.p(x=x, s=s-1, t=t+1), '/', _Blog.p(x=x, s=s-1, t=1),
                       depth=depth, rule="survival chain rule")
             return found / p
         
         # (2b) inverse chain rule: p_x(t) = p_x(t+1) / p_x+t 
         found = self._p_x(x, s=s, t=t+1, depth=depth-1)
         p = self._p_x(x, s=s+t, t=1, depth=1-abs(depth))
         if found is not None and p is not None:
-            self.blog(Blog.p(x=x, s=s, t=t), '=',
-                      Blog.p(x=x, s=s, t=t+1), '/', Blog.p(x=x, s=s+t, t=1),
+            self.blog(_Blog.p(x=x, s=s, t=t), '=',
+                      _Blog.p(x=x, s=s, t=t+1), '/', _Blog.p(x=x, s=s+t, t=1),
                       depth=depth, rule="survival chain rule")
             return found / p
         if t > 1:
             # (3a) chain rule: p_x(t) = p_x * p_x+1(t-1)
             found = self._p_x(x, s=s+1, t=t-1, depth=depth-1)
             p = self._p_x(x, s=s, t=1, depth=1-abs(depth))
             if found is not None and p is not None:
-                self.blog(Blog.p(x=x, s=s, t=t), '=',
-                          Blog.p(x=x, s=s+1, t=t-1), '*', Blog.p(x=x, s=s, t=1),
+                self.blog(_Blog.p(x=x, s=s, t=t), '=',
+                          _Blog.p(x=x, s=s+1, t=t-1), '*', _Blog.p(x=x, s=s, t=1),
                           depth=depth, rule="survival chain rule")
                 return found * p
 
             # (3b) chain rule: p_x(t) = p_x+t-1 * p_x(t-1)
             found = self._p_x(x, s=s, t=t-1, depth=depth-1)
             p = self._p_x(x, s=s+t-1, t=1, depth=1-abs(depth))
             if found is not None and p is not None:
-                self.blog(Blog.p(x=x, s=s, t=t), '=',
-                          Blog.p(x=x, s=s, t=t-1), '*', Blog.p(x=x, s=s+t-1, t=1),
+                self.blog(_Blog.p(x=x, s=s, t=t), '=',
+                          _Blog.p(x=x, s=s, t=t-1), '*', _Blog.p(x=x, s=s+t-1, t=1),
                           depth=depth, rule="survival chain rule")
                 return found * p
 
         if t == 1:
             E = self._E_x(x, s=s, t=1, depth=depth-1)
             if E is not None:
-                self.blog(Blog.p(x=x, s=s, t=1), '=',
-                          Blog.E(x=x, s=s, t=1), "/v",
+                self.blog(_Blog.p(x=x, s=s, t=1), '=',
+                          _Blog.E(x=x, s=s, t=1), "/v",
                           depth=depth, rule="one-year endowment")
                 return E / self.interest.v
 
             # (4a) annuity recursion: p_x = [a_x(t) - 1] / [v a_x+1(t-1)
             for _t in [self.WHOLE, 2]:  # consider only WL and 2-term
                 a = self._a_x(x, s=s, t=_t, depth=depth-1)
                 a1 = self._a_x(x, s=s+1, t=self.add_term(_t, -1), depth=depth-1)
                 if a is not None and a1 is not None:
-                    self.blog(Blog.p(x=x, s=s, t=1), '= [',
-                              Blog.a(x=x, s=s, t=_t), '- 1 ] / [ v *',
-                              Blog.a(x=x, s=s+1, t=_t-1), ']',
+                    self.blog(_Blog.p(x=x, s=s, t=1), '= [',
+                              _Blog.a(x=x, s=s, t=_t), '- 1 ] / [ v *',
+                              _Blog.a(x=x, s=s+1, t=_t-1), ']',
                               depth=depth, rule="annuity recursion")
                     return (a - 1) / (self.interest.v * a1)
 
             
             # (4b) insurance recursion: p_x = [v - A_x(t)] / [v (1 - A_x+1(t-1))]
             for _t in [self.WHOLE, 2]:  # consider only WL and 2-term
                 A = self._A_x(x, s=s, t=_t, depth=depth-1)
                 A1 = self._A_x(x, s=s+1, t=self.add_term(_t, -1), depth=depth-1)
                 if A is not None and A1 is not None:
-                    self.blog(Blog.p(x=x, s=s, t=1), '= [ v -',
-                              Blog.A(x=x, s=s, t=_t), '] / [v * [ 1 -',
-                              Blog.A(x=x, s=s+1, t=_t-1), ']]',
+                    self.blog(_Blog.p(x=x, s=s, t=1), '= [ v -',
+                              _Blog.A(x=x, s=s, t=_t), '] / [v * [ 1 -',
+                              _Blog.A(x=x, s=s+1, t=_t-1), ']]',
                               depth=depth, rule="insurance recursion")
                     return (self.interest.v - A)/(self.interest.v * (1 - A1))
 
     def p_x(self, x: int, s: int = 0, t: int = 1) -> float:
         """Compute survival probability by calling recursion helper
 
         Args:
           x : age of selection
           s : years after selection
           t : survives at least t years
         """
-        self.blog = Blog("Survival",
-                         Blog.p(x=x, s=s, t=t),
+        self.blog = _Blog("Survival",
+                         _Blog.p(x=x, s=s, t=t),
                          levels=self.maxdepth)
         p = self._p_x(x, s=s, t=t, depth=self.maxdepth)
         if p is not None:
             print(self.blog, end='')
         return p
 
     #
@@ -296,50 +296,50 @@
             return found
         if depth <= 0:
             return None
         if moment == 1:
             if t > 0:  
                 p_t = self._p_x(x, s=s, t=t)
                 if t == 1 and curtate:
-                    self.blog(Blog.e(x=x, s=s, t=1, curtate=curtate), '=',
-                              Blog.p(x=x, s=s, t=1),
+                    self.blog(_Blog.e(x=x, s=s, t=1, curtate=curtate), '=',
+                              _Blog.p(x=x, s=s, t=1),
                               #f"e_{x+s}:1",
                               depth=depth, rule='1-year curtate shortcut')
                     return p_t   # (1) if curtate and t=1: e_x:1 = p_x 
                 if t > 1:
                     e = self._e_x(x, s=s, t=Reserves._WHOLE, curtate=curtate, 
                                   moment=1, depth=depth-1)
                     e_t = self._e_x(x, s=s+t, t=Reserves._WHOLE, curtate=curtate,
                                     moment=1, depth=depth-1)
                     if e is not None and e_t is not None and p_t is not None:
-                        self.blog(Blog.e(x=x, s=s, t=t), '=', Blog.e(x=x, s=s), '-',
-                                  Blog.p(x=x, s=s), '*', Blog.e(x=x, s=s+t),
+                        self.blog(_Blog.e(x=x, s=s, t=t), '=', _Blog.e(x=x, s=s), '-',
+                                  _Blog.p(x=x, s=s), '*', _Blog.e(x=x, s=s+t),
                                   #"e_{x+s}:{t}: e_x - p_x e_x+t",
                                   depth=depth, rule="temporary lifetime")
                         return e - p_t*e_t  # (2) temporary = e_x - t_p_x e_x+t
             e = self._e_x(x, s=s-1, t=self.add_term(t, 1), curtate=curtate,
                           moment=1, depth=depth-1)
             e1 = self._e_x(x, s=s-1, t=1, curtate=curtate, moment=1,
                           depth=depth-1)
             p = self._p_x(x, s=s-1)
             if e is not None and e1 is not None and p is not None:
                 #_t = "" if t < 0 else ":" + str(t)
                 #msg = f"forward e_{x+s}{_t} = e_{x+s}:1 + p_{x+s} e_{x+s+1}"
-                self.blog(Blog.e(x=x, s=s, t=t), '=', Blog.e(x=x, s=s, t=t), '+',
-                          Blog.p(x=x, s=s), '*', Blog.e(x=x, s=s+t),
+                self.blog(_Blog.e(x=x, s=s, t=t), '=', _Blog.e(x=x, s=s, t=t), '+',
+                          _Blog.p(x=x, s=s), '*', _Blog.e(x=x, s=s+t),
                           depth=depth, rule='lifetime forward recursion')
                 return (e - e1) / p # (3) forward: (e_x-1 - e_x-1:1) / p_x-1
             e = self._e_x(x, s=s, t=1, curtate=curtate,
                           moment=1, depth=depth-1)
             e_t = self._e_x(x, s=s+1, t=self.add_term(t, -1), curtate=curtate,
                             moment=1, depth=depth-1)
             p = self._p_x(x, s=s)
             if e is not None and e_t is not None and p is not None:
-                self.blog(Blog.e(x=x, s=s, t=t), '=', Blog.e(x=x ,s=s, t=1), '+',
-                          Blog.p(x=x, s=s), '*', Blog.e(x=x, s=s+1, t=t-1),
+                self.blog(_Blog.e(x=x, s=s, t=t), '=', _Blog.e(x=x ,s=s, t=1), '+',
+                          _Blog.p(x=x, s=s), '*', _Blog.e(x=x, s=s+1, t=t-1),
                           #f"backward: e_x:1 + p_x e_x+1:{t}",
                           depth=depth, rule='lifetime backward recursion')
                 return e + p * e_t # (4) backward: e_x:1 + p_x e_x+1:t-1
 
 
     def e_x(self, x: int, s: int = 0, t: int = Reserves._WHOLE, 
             curtate: bool = False, moment: int = 1) -> float:
@@ -348,16 +348,16 @@
         Args:
           x : age of selection
           s : years after selection
           t : limited at t years
           curtate : whether curtate (True) or complete (False) lifetime
           moment : whether to compute first (1) or second (2) moment
         """
-        self.blog = Blog("Lifetime",
-                         Blog.e(x=x, s=s, t=t, moment=moment, curtate=curtate),
+        self.blog = _Blog("Lifetime",
+                         _Blog.e(x=x, s=s, t=t, moment=moment, curtate=curtate),
                          levels=self.maxdepth)
         e = self._e_x(x, s=s, t=t, curtate=curtate, moment=moment,
                       depth=self.maxdepth)
         if e is not None:
             print(self.blog, end='')
             return e
 
@@ -404,64 +404,64 @@
         if t < 0:     # t infinite => EPV(t) = 0
             return 0
         if t == 0:    # t = 0 => EPV(0) = endowment**moment
             return endowment**moment
         if moment > 1:
             E = self._E_x(x, s=s, endowment=endowment, depth=depth)
             if E:  # (1) Shortcut: 2E_x = v E_x
-                self.blog(Blog.E(x=x, s=s, t=t, moment=moment),
-                          f"= v(t={t})"+Blog.m(moment), '*', Blog.E(x=x, s=s, t=t),
+                self.blog(_Blog.E(x=x, s=s, t=t, moment=moment),
+                          f"= v(t={t})"+_Blog.m(moment), '*', _Blog.E(x=x, s=s, t=t),
                           depth=depth, rule='moments of pure endowment')
                 return E * self.interest.v**(moment-1) 
         p = self._p_x(x, s=s, t=t, depth=depth-1)  # 1-abs(depth))
         if p is not None:   # (2) E_x = p_x * v
             #msg = f"pure endowment {t}_E_{x+s} = {t}_p_{x+s} * v^{t}"
-            self.blog(Blog.E(x=x, s=s, t=t), '=', Blog.p(x=x, s=s, t=t),
-                      f"* v(t={t})"+Blog.m(moment),
+            self.blog(_Blog.E(x=x, s=s, t=t), '=', _Blog.p(x=x, s=s, t=t),
+                      f"* v(t={t})"+_Blog.m(moment),
                       depth=depth, rule='pure endowment')
             return p * (endowment * self.interest.v_t(t))**moment
         if depth <= 0:
             return None
 
         At = self._A_x(x, s=s, t=t, moment=moment, b=endowment, endowment=0,
                        depth=depth-1)  #1-abs(depth))
         A = self._A_x(x, s=s, t=t, b=endowment, endowment=endowment, 
                       moment=moment, depth=1-abs(depth))        
         if A is not None and At is not None:
-            self.blog(Blog.E(x=x, s=s, t=t), '=',
-                      Blog.A(x=x, s=s, t=t, endowment=endowment), '-',
-                      Blog.A(x=x, s=s, t=t, endowment=0),
+            self.blog(_Blog.E(x=x, s=s, t=t), '=',
+                      _Blog.A(x=x, s=s, t=t, endowment=endowment), '-',
+                      _Blog.A(x=x, s=s, t=t, endowment=0),
                       #f"endowment - term insurance = {t}_E_{x+s}",
                       depth=depth, rule='endowment insurance minus term')
             return A - At  # (3) endowment insurance - term (helpful SULT)
 
         E = self._E_x(x, s=s, moment=moment, depth=1-abs(depth))
         Et = self._E_x(x, s=s+1, t=t-1, moment=moment, depth=depth-1)
         if E is not None and Et is not None:
             msg = f"chain Rule: {t}_E_{x+s} = E_{x+s} * {t-1}_E_{x+s+1}"
-            self.blog(Blog.E(x=x, s=s, t=t, moment=moment), '=',
-                      Blog.E(x=x, s=s, t=1, moment=moment), '*',
-                      Blog.E(x=x, s=s+1, t=t-1, moment=moment), '*',
-                      Blog.m(moment, endow=endowment),
+            self.blog(_Blog.E(x=x, s=s, t=t, moment=moment), '=',
+                      _Blog.E(x=x, s=s, t=1, moment=moment), '*',
+                      _Blog.E(x=x, s=s+1, t=t-1, moment=moment), '*',
+                      _Blog.m(moment, endow=endowment),
                       depth=depth, rule='pure endowment chain rule')
             return E * Et * endowment**moment # (4) chain rule
 
     def E_x(self, x: int, s: int = 0, t: int = 1, 
             endowment: int = 1, moment: int = 1) -> float:
         """Compute pure endowment by calling recursion helper
 
         Args:
           x : age of selection
           s : years after selection
           t : term of pure endowment
           endowment : amount of pure endowment
           moment : compute first or second moment
         """
-        self.blog = Blog("Pure Endowment",
-                         Blog.E(x=x, s=s, t=t, moment=moment, endowment=endowment),
+        self.blog = _Blog("Pure Endowment",
+                         _Blog.E(x=x, s=s, t=t, moment=moment, endowment=endowment),
                          levels=self.maxdepth)
         if moment == self._VARIANCE:  # Bernoulli shortcut for variance
             found = self.get_E(x, s=s, t=t, endowment=endowment, moment=moment)
             if found is not None:
                 return found
             t_p_x = self.p_x(x, s=s, t=t)
             return (endowment * self.interest.v_t(t))**2 * t_p_x * (1-t_p_x)
@@ -518,26 +518,26 @@
             return None
 
         if t > 0:  # decreasing must be term insurance
             A = self._A_x(x=x, s=s, t=t, b=b, discrete=discrete, depth=depth-1)
             n = t + int(discrete)
             DA = self._DA_x(x=x, s=s, t=t, b=b, discrete=discrete, depth=depth-1)
             if A is not None and DA is not None:
-                self.blog(Blog.IA(x=x, s=s, t=t), f'= {n}',
-                          Blog.A(x=x, s=s, t=t), '-', Blog.DA(x=x, s=s, t=t),
+                self.blog(_Blog.IA(x=x, s=s, t=t), f'= {n}',
+                          _Blog.A(x=x, s=s, t=t), '-', _Blog.DA(x=x, s=s, t=t),
                     #f"identity IA_{x+s}:{t}: ({n})A - DA",
                           depth=depth, rule='varying insurance identity')
                 return A * n - DA  # (1) Identity with term and decreasing
 
         A = self._A_x(x=x, s=s, t=1, b=b, discrete=discrete, depth=depth-1)
         IA = self._IA_x(x=x, s=s+1, t=self.add_term(t, -1), b=b, depth=depth-1)
         p = self._p_x(x, s=s, t=1, depth=1-abs(depth))   # FIXED t=1
         if A is not None and IA is not None and p is not None:
-            self.blog(Blog.IA(x=x, s=s, t=t), '=', Blog.A(x=x, s=s, t=t), '+',
-                      Blog.p(x=x, s=s), f"* v(t={t}) *", Blog.IA(x=x, s=s+1, t=t-1),
+            self.blog(_Blog.IA(x=x, s=s, t=t), '=', _Blog.A(x=x, s=s, t=t), '+',
+                      _Blog.p(x=x, s=s), f"* v(t={t}) *", _Blog.IA(x=x, s=s+1, t=t-1),
                       #f"backward IA_{x+s}:{t}: A + IA_{x+s+1}:{t-1}",
                       depth=depth, rule='backward recursion')
             return A + p * self.interest.v * IA  # (2) backward recursion
 
     def increasing_insurance(self, x: int, s: int = 0, t: int = Reserves._WHOLE,
                              b: int = 1, discrete: bool = True) -> float:
         """Compute increasing insurance with recursive helper
@@ -545,16 +545,16 @@
         Args:
           x : age of selection
           s : years after selection
           t : term of insurance
           b : amount of benefit in first year
           discrete : benefit paid year-end (True) or moment of death (False)
         """
-        self.blog = Blog("Increasing Insurance",
-                         Blog.IA(x=x, s=s, t=t, b=b, discrete=discrete),
+        self.blog = _Blog("Increasing Insurance",
+                         _Blog.IA(x=x, s=s, t=t, b=b, discrete=discrete),
                          levels=self.maxdepth)
         IA = self._IA_x(x, s=s, b=b, t=t, discrete=discrete, depth=self.maxdepth)
         if IA is not None:
             print(self.blog, end='')
             return IA
         IA = super().increasing_insurance(x, s=s, b=b, t=t, discrete=discrete)
         if IA is not None:
@@ -609,41 +609,41 @@
         if t < 0:  # decreasing must be term insurance
             return None
     
         A = self._A_x(x=x, s=s, t=t, b=b, discrete=discrete, depth=depth-1)
         n = t + int(discrete)
         IA = self._DA_x(x=x, s=s, t=t, b=b, discrete=discrete, depth=depth-1)
         if A is not None and IA is not None:
-            self.blog(Blog.DA(x=x, s=s, t=t), f'= {n}',
-                      Blog.A(x=x, s=s, t=t), '-', Blog.IA(x=x, s=s, t=t),
+            self.blog(_Blog.DA(x=x, s=s, t=t), f'= {n}',
+                      _Blog.A(x=x, s=s, t=t), '-', _Blog.IA(x=x, s=s, t=t),
                       depth=depth, rule='varying insurance identity')
             return A * n - IA  # (1) identity with term and decreasing
 
         DA = self._IA_x(x=x, s=s+1, t=self.add_term(t, -1), b=b, depth=depth-1)
         p = self._p_x(x, s=s, depth=1-abs(depth))
         if DA is not None and p is not None:
             #msg = f"backward DA_{x+s}:{t}: v(t q_{x+s} + p_{x+s} DA_{x+s+1}:{t-1})"
-            self.blog(Blog.DA(x=x, s=s, t=t), f"= v(t={t}) * t *", Blog.q(x=x, s=s),
-                      '+', Blog.p(x=x, s=s), '*', Blog.DA(x=x, s=s+1, t=t-1),
+            self.blog(_Blog.DA(x=x, s=s, t=t), f"= v(t={t}) * t *", _Blog.q(x=x, s=s),
+                      '+', _Blog.p(x=x, s=s), '*', _Blog.DA(x=x, s=s+1, t=t-1),
                       depth=depth, rule='backward recursion')
             return self.interest.v * ((1-p)*t + p*DA)  # (2) backward recursion
 
     def decreasing_insurance(self, x: int, s: int = 0, t: int = Reserves._WHOLE,
                              b: int = 1, discrete: bool = True) -> float:
         """Compute decreasing insurance by calling recursive helper first
 
         Args:
           x : age of selection
           s : years after selection
           t : term of insurance
           b : amount of benefit in first year
           discrete : benefit paid year-end (True) or moment of death (False)
         """
-        self.blog = Blog("Increasing Insurance",
-                         Blog.DA(x=x, s=s, t=t, b=b, discrete=discrete),
+        self.blog = _Blog("Increasing Insurance",
+                         _Blog.DA(x=x, s=s, t=t, b=b, discrete=discrete),
                          levels=self.maxdepth)
         if t == 0:
             return 0
         A = self._DA_x(x=x, s=s, t=t, b=b, discrete=discrete, depth=self.maxdepth)
         if A is not None:
             print(self.blog, end='')
             return A
@@ -731,101 +731,101 @@
 
         if u > 0:  # (1) deferred insurance  
             A = self._A_x(x=x, s=s+1, t=t, b=b, u=u-1, discrete=discrete, 
                               moment=moment, endowment=endowment, depth=depth-1)
             E = self._E_x(x, s=s, t=1, moment=moment, depth=depth-1)
             if A is not None and p is not None:  # (1a) backward E_x * A
                 #msg = f"backward deferred {u}_A_{x+s}: {u}_E * A_{x+s+u}"
-                self.blog(Blog.A(x=x, s=s, t=t, u=u, b=b, moment=moment), '=',
-                          Blog.E(x=x, s=s, moment=moment), '*',
-                          Blog.A(x=x, s=s+1, t=t, u=u-1, moment=moment),
+                self.blog(_Blog.A(x=x, s=s, t=t, u=u, b=b, moment=moment), '=',
+                          _Blog.E(x=x, s=s, moment=moment), '*',
+                          _Blog.A(x=x, s=s+1, t=t, u=u-1, moment=moment),
                           depth=depth, rule='backward recursion')
                 return E * A
 
             A = self._A_x(x, s=s-1, t=t, b=b, u=u+1, discrete=discrete, 
                           moment=moment, endowment=endowment, depth=depth-1)
             E = self._E_x(x, s=s-1, t=1, moment=moment, depth=depth-1)
             if A is not None and E is not None: # (1b) forward recursion
                 msg = f"forward deferred {u}_A_{x+s}: {u+1}A_{x+s-1} / E"
-                self.blog(Blog.A(x=x, s=s, t=t, u=u, b=b, moment=moment), '=',
-                          Blog.A(x=x, s=s-1, t=t, u=u+1, moment=moment), '/',
-                          Blog.E(x=x, s=s-1, moment=moment),
+                self.blog(_Blog.A(x=x, s=s, t=t, u=u, b=b, moment=moment), '=',
+                          _Blog.A(x=x, s=s-1, t=t, u=u+1, moment=moment), '/',
+                          _Blog.E(x=x, s=s-1, moment=moment),
                           depth=depth, rule='forward recursion')
                 return A / E
             return None
 
         if endowment > 0: # (2a) endowment = term + E_x * endowment
             A = self._A_x(x=x, s=s, t=t, b=b, discrete=discrete, 
                           moment=moment, depth=1-abs(depth))
             E_x = self._E_x(x=x, s=s, t=t, moment=moment, 
                             endowment=endowment, depth=1-abs(depth))
             if A is not None and E_x is not None:
                 # f"term + pure insurance = A_{x+s}:{t}",
-                self.blog(Blog.A(x=x, s=s, t=t, endowment=endowment, moment=moment),
-                          '=', Blog.A(x=x, s=s, t=t, moment=moment), '+',
-                          Blog.E(x=x, s=s, t=t, endowment=endowment, moment=moment),
+                self.blog(_Blog.A(x=x, s=s, t=t, endowment=endowment, moment=moment),
+                          '=', _Blog.A(x=x, s=s, t=t, moment=moment), '+',
+                          _Blog.E(x=x, s=s, t=t, endowment=endowment, moment=moment),
                           depth=depth, rule='term plus pure endowment')
                 return A + E_x
         else:             # (2b) term = endowment insurance - E_x * endowment
             A = self._A_x(x=x, s=s, t=t, b=b, discrete=discrete, 
                           moment=moment, endowment=b, depth=1-abs(depth))
             E_x = self._E_x(x=x, s=s, t=t, moment=moment, endowment=b, 
                             depth=1-abs(depth))
             if A is not None and E_x is not None:
                 #msg = f"endowment insurance - pure endowment = A_{x+s}^1:{t}"
-                self.blog(Blog.A(x=x, s=s, t=t, moment=moment), '=',
-                          Blog.A(x=x, s=s, t=t, moment=moment, endowment=b), '-',
-                          Blog.E(x=x, s=s, t=t, endowment=b, moment=moment),
+                self.blog(_Blog.A(x=x, s=s, t=t, moment=moment), '=',
+                          _Blog.A(x=x, s=s, t=t, moment=moment, endowment=b), '-',
+                          _Blog.E(x=x, s=s, t=t, endowment=b, moment=moment),
                           depth=depth, rule='endowment insurance - pure')
                 return A - E_x
 
         if not discrete:  # recursions for discrete insurance
             return None
         if t == 1:  # special cases for discrete one-year insurance
             if endowment == b:  # (3a) discrete one-year endowment insurance
-                self.blog(Blog.A(x=x, s=s, t=1, endowment=endowment,
-                                 moment=moment), f"= v"+Blog.m(moment),
-                          "*", Blog.m(moment, endow=endowment),
+                self.blog(_Blog.A(x=x, s=s, t=1, endowment=endowment,
+                                 moment=moment), f"= v"+_Blog.m(moment),
+                          "*", _Blog.m(moment, endow=endowment),
                           depth=depth, rule='one-year endowment insurance')
                 return (self.interest.v * endowment)**moment
             p = self._p_x(x, s=s, t=1)
             if p is not None:  # (3b) one-year discrete insurance
-                self.blog(Blog.A(x=x, s=s, t=t, moment=moment, endowment=endowment),
-                          f"= v"+Blog.m(moment), "*",
-                          Blog.q(x=x, s=s), f"*", "v"*Blog.m(moment), "+",
-                          Blog.p(x=x, s=s), f"*".
-                          Blog.m(moment, endow=endowment),
+                self.blog(_Blog.A(x=x, s=s, t=t, moment=moment, endowment=endowment),
+                          f"= v"+_Blog.m(moment), "*",
+                          _Blog.q(x=x, s=s), f"*", "v"*_Blog.m(moment), "+",
+                          _Blog.p(x=x, s=s), f"*".
+                          _Blog.m(moment, endow=endowment),
                           #f"discrete 1-year insurance: A_{x+s}:1 = qv",
                           depth=depth, rule='one-year discrete insurance')
                 return (self.interest.v**moment 
                         * ((1 - p) * b**moment + p * endowment**moment))
     
         A = self._A_x(x=x, s=s+1, t=self.add_term(t, -1), b=b, 
                       discrete=discrete, moment=moment,
                       endowment=endowment, depth=depth-1)
         p = self._p_x(x, s=s, t=1, depth=1-abs(depth)) # (4) backward recursion
         if A is not None and p is not None:
-            self.blog(Blog.A(x=x, s=s, t=t, b=b, moment=moment),
-                      f"= v"+Blog.m(moment), "* [",
-                      Blog.q(x=x,s=s), f"* b"+Blog.m(moment), "+",
-                      Blog.p(x=x, s=s), '*',
-                      Blog.A(x=x, s=s+1, t=t-1, b=b, moment=moment), ']',
+            self.blog(_Blog.A(x=x, s=s, t=t, b=b, moment=moment),
+                      f"= v"+_Blog.m(moment), "* [",
+                      _Blog.q(x=x,s=s), f"* b"+_Blog.m(moment), "+",
+                      _Blog.p(x=x, s=s), '*',
+                      _Blog.A(x=x, s=s+1, t=t-1, b=b, moment=moment), ']',
                       #f"backward: A_{x+s} = qv + pvA_{x+s+1}",
                       depth=depth, rule='backward recursion')
             return self.interest.v_t(1)**moment * ((1 - p)*b**moment + p*A)
 
         A = self._A_x(x=x, s=s-1, t=self.add_term(t, 1), b=b, u=u, 
                       discrete=discrete, moment=moment, 
                       endowment=endowment, depth=depth-1)
         p = self._p_x(x, s=s-1, t=1, depth=1-abs(depth))
         if A is not None and p is not None:  # (5) forward recursion
-            self.blog(Blog.A(x=x, s=s, t=t, b=b, moment=moment), '= [',
-                      Blog.A(x=x, s=s-1, t=t+1, b=b, moment=moment),
-                      f"/v"+Blog.m(moment), "-", Blog.q(x=x,s=s),
-                      f"* b"+Blog.m(moment), "] /", Blog.p(x=x, s=s),
+            self.blog(_Blog.A(x=x, s=s, t=t, b=b, moment=moment), '= [',
+                      _Blog.A(x=x, s=s-1, t=t+1, b=b, moment=moment),
+                      f"/v"+_Blog.m(moment), "-", _Blog.q(x=x,s=s),
+                      f"* b"+_Blog.m(moment), "] /", _Blog.p(x=x, s=s),
                       #f"forward: A_{x+s} = (A_{x+s-1}/v - q) / p",
                       depth=depth, rule='forward recursion')
             return (A/self.interest.v_t(1)**moment - (1-p)*b**moment) / p
 
     def whole_life_insurance(self, x: int, s: int = 0, b: int = 1, 
                              discrete: bool = True, moment: int = 1) -> float:
         """Compute whole life insurance A_x by calling recursion helper and twin
@@ -833,16 +833,16 @@
         Args:
           x : age of selection
           s : years after selection
           b : amount of benefit
           moment : compute first or second moment
           discrete : benefit paid year-end (True) or moment of death (False)
         """
-        self.blog = Blog("Whole Life Insurance",
-                         Blog.A(x=x, s=s, t=Reserves._WHOLE, b=b, u=0,
+        self.blog = _Blog("Whole Life Insurance",
+                         _Blog.A(x=x, s=s, t=Reserves._WHOLE, b=b, u=0,
                                 endowment=0, moment=moment, discrete=discrete),
                          levels=self.maxdepth)
         found = self._A_x(x, s=s, b=b, moment=moment, discrete=discrete,
                           depth=self.maxdepth)
         if found is not None:
             print(self.blog, end='')
             return found
@@ -867,16 +867,16 @@
           x : age of selection
           s : years after selection
           t : term of insurance
           b : amount of benefit
           moment : compute first or second moment
           discrete : benefit paid year-end (True) or moment of death (False)
         """
-        self.blog = Blog("Term Insurance",
-                         Blog.A(x=x, s=s, t=t, b=b, u=0, discrete=discrete,
+        self.blog = _Blog("Term Insurance",
+                         _Blog.A(x=x, s=s, t=t, b=b, u=0, discrete=discrete,
                                 endowment=0, moment=moment),
                          levels=self.maxdepth)
         found = self._A_x(x, s=s, b=b, t=t, moment=moment, discrete=discrete,
                           depth=self.maxdepth)
         if found is not None:
             print(self.blog, end='')
             return found
@@ -886,16 +886,16 @@
             print(self.blog, end='')
             return A
 
     def deferred_insurance(self, x: int, s: int = 0, b: int = 1, u: int = 0, 
                            t: int = Reserves._WHOLE, moment: int = 1, 
                            discrete: bool = True) -> float:
         """Compute deferred life insurance u|A_x:t^1 by calling recursion helper: """
-        self.blog = Blog("Deferred Insurance",
-                         Blog.A(x=x, s=s, t=t, b=b, u=u, discrete=discrete,
+        self.blog = _Blog("Deferred Insurance",
+                         _Blog.A(x=x, s=s, t=t, b=b, u=u, discrete=discrete,
                                 endowment=0, moment=moment),
                          levels=self.maxdepth)
         A = self.get_A(x=x, s=s, t=t, b=b, u=u, discrete=discrete, 
                        moment=moment)
         if A is not None:
             print(self.blog, end='')
             return A
@@ -905,16 +905,16 @@
             print(self.blog, end='')
             return A
     
     def endowment_insurance(self, x: int, s: int = 0, t: int = 1, b: int = 1,
                             endowment: int = -1, moment: int = 1,
                             discrete: bool = True) -> float:
         """Compute endowment insurance u|A_x:t by calling recursion helper: """
-        self.blog = Blog("Endowment Insurance",
-                         Blog.A(x=x, s=s, t=t, b=b, u=0, discrete=discrete,
+        self.blog = _Blog("Endowment Insurance",
+                         _Blog.A(x=x, s=s, t=t, b=b, u=0, discrete=discrete,
                                 endowment=endowment, moment=moment),
                          levels=self.maxdepth)
         assert t >= 0
         if endowment < 0:
             endowment = b
         found = self._A_x(x, s=s, b=b, t=t, moment=moment, discrete=discrete,
                           endowment=endowment, depth=self.maxdepth)
@@ -976,15 +976,15 @@
                            variance=variance, discrete=discrete), val)
 
     def _a_x(self, x: int, s: int = 0, t: int = Reserves._WHOLE, 
              u: int = 0, b: int = 1, discrete: bool = True, 
              variance: bool = False, depth: int = 1) -> float | None:
         """Helper to compute from recursive and alternate formulas"""
         if t == 1 and not u and discrete:
-            self.blog(Blog.a(x=x, s=s, t=1, discrete=discrete), '= 1',
+            self.blog(_Blog.a(x=x, s=s, t=1, discrete=discrete), '= 1',
                       depth=depth, rule='one-year discrete annuity')
             return b 
         if t == 0:
             return 0
         found = self.get_a(x=x, s=s, t=t, b=b, u=u, discrete=discrete,
                            variance=variance)
         if found is not None:
@@ -996,51 +996,51 @@
 
         if u > 0:  # (1) deferred annuity
             found = self._a_x(x=x, s=s+1, t=t, b=b, u=u-1, discrete=discrete, 
                               variance=variance, depth=depth-1)
             E = self._E_x(x, s=s, t=1, depth=depth-1)
             if found is not None and E is not None:
                 #msg = f"backward {u}_a_{x+s} = {u}_E * a_{x+s+u}"
-                self.blog(Blog.a(x=x, s=s, u=u, t=t), '=',
-                          Blog.a(x=x, s=s+1, t=t, u=u-1), '/', Blog.E(x=x, s=s),
+                self.blog(_Blog.a(x=x, s=s, u=u, t=t), '=',
+                          _Blog.a(x=x, s=s+1, t=t, u=u-1), '/', _Blog.E(x=x, s=s),
                           depth=depth, rule='backward deferred annuity')
                 return E * found  # (1a) backward recusion
 
             found = self._a_x(x=x, s=s-1, t=t, b=b, u=u+1, discrete=discrete, 
                               depth=depth-1)         # FIXED u=u+1
             E = self._E_x(x, s=s-1, t=1, depth=depth-1)
             if found is not None and E is not None:  # (1b) forward
                 #msg = f"forward: {u}_a_{x+s} = {u+1}_a_{x+s-1}/E_{x+s-1}"
-                self.blog(Blog.a(x=x, s=s, u=u, t=t), '=',
-                          Blog.a(x=x, s=s-1, t=t, u=u+1), '/', Blog.E(x=x, s=s-1),
+                self.blog(_Blog.a(x=x, s=s, u=u, t=t), '=',
+                          _Blog.a(x=x, s=s-1, t=t, u=u+1), '/', _Blog.E(x=x, s=s-1),
                           depth=depth, rule='forward deferred annuity')
                 return found / E
 
         else:  # (2) Temporary and whole annuity
             found = self._a_x(x=x, s=s+1, t=self.add_term(t, -1), b=b, u=u, 
                               discrete=discrete, 
                               variance=variance, depth=depth-1)
             E = self._E_x(x, s=s, t=1, depth=depth-1)
             if found is not None and E is not None:  # (2a) backward
                 #msg = (f"backward: a_{x+s}{'' if t < 0 else (':'+str(t))} = 1 + "
                 #       + f"E_{x+s} a_{x+s+1}{'' if t < 0 else (':'+str(t-1))}")
                 #_t = "" if t < 0 else f":{t-1}"
-                self.blog(Blog.a(x=x, s=s, t=t), '= 1 +',
-                          Blog.E(x=x, s=s, t=1), '*', Blog.a(x=x, s=s+1, t=t-1),
+                self.blog(_Blog.a(x=x, s=s, t=t), '= 1 +',
+                          _Blog.E(x=x, s=s, t=1), '*', _Blog.a(x=x, s=s+1, t=t-1),
                           depth=depth, rule='backward recursion')
                 return b + E * found
 
             found = self._a_x(x=x, s=s-1, t=self.add_term(t, 1), b=b, u=u, 
                               discrete=discrete, depth=depth-1)
             E = self._E_x(x, s=s-1, t=1, depth=depth-1)
             if found is not None and E is not None:  # (2b) forward
                 _t = "" if t < 0 else f":{t-1}"
-                self.blog(Blog.a(x=x, s=s, t=t), '= [',
-                          Blog.a(x=x, s=s-1), '- 1 ] /',
-                          Blog.E(x=x, s=s-1, t=1),
+                self.blog(_Blog.a(x=x, s=s, t=t), '= [',
+                          _Blog.a(x=x, s=s-1), '- 1 ] /',
+                          _Blog.E(x=x, s=s-1, t=1),
                     #f"forward: a_{x+s}{_t} = (a_{x+s-1} - 1)/E",
                           depth=depth, rule='forward recursion')
                 return (found - b) / E
 
     def whole_life_annuity(self, x: int, s: int = 0, b: int = 1, 
                            variance: bool = False,
                            discrete: bool = True) -> float:
@@ -1049,16 +1049,16 @@
         Args:
           x : age of selection
           s : years after selection
           b : annuity benefit amount
           variance (bool): return EPV (True) or variance (False)
           discrete : annuity due (True) or continuous (False)
         """
-        self.blog = Blog("Whole Life Annuity",
-                         Blog.a(x=x, s=s, t=Reserves._WHOLE, b=b, u=0,
+        self.blog = _Blog("Whole Life Annuity",
+                         _Blog.a(x=x, s=s, t=Reserves._WHOLE, b=b, u=0,
                                 discrete=discrete, variance=False),
                          levels=self.maxdepth)
         found = self._a_x(x, s=s, b=b, variance=variance, 
                           discrete=discrete, depth=self.maxdepth)
         if found is not None:
             print(self.blog, end='')
             return found
@@ -1084,29 +1084,29 @@
           x : age of selection
           s : years after selection
           t : term of annuity in years
           b : annuity benefit amount
           variance (bool): return EPV (True) or variance (False)
           discrete : annuity due (True) or continuous (False)
         """
-        self.blog = Blog("Temporary Annuity",
-                         Blog.a(x=x, s=s, t=t, b=b, u=0,
+        self.blog = _Blog("Temporary Annuity",
+                         _Blog.a(x=x, s=s, t=t, b=b, u=0,
                                 discrete=discrete, variance=variance),
                          levels=self.maxdepth)
         found = self._a_x(x, s=s, b=b, t=t, variance=variance, 
                           discrete=discrete, depth=self.maxdepth)
         if found is not None:
             print(self.blog, end='')
             return found
         if not variance and self.interest.i > 0: # (1) twin insurance shortcut
             A = self._A_x(x, s=s, b=b, t=t, endowment=b, discrete=discrete, 
                           depth=self.maxdepth)
             if A is not None:
-                self.blog(Blog.a(x=x, s=s, t=t), '= [ 1 -',
-                          Blog.A(x=x, s=s, t=t), f"] / d(t={t})",
+                self.blog(_Blog.a(x=x, s=s, t=t), '= [ 1 -',
+                          _Blog.A(x=x, s=s, t=t), f"] / d(t={t})",
                           #"Annuity twin: a = (1 - A) / d",
                           depth=self.maxdepth, rule='annuity twin')
                 print(self.blog, end='')
                 return self.annuity_twin(A=A, discrete=discrete)
         a = super().temporary_annuity(x, s=s, b=b, t=t, discrete=discrete,
                                       variance=variance)
         if a is not None:
@@ -1121,16 +1121,16 @@
           x : age of selection
           s : years after selection
           u : years deferred
           t : term of annuity in years
           b : annuity benefit amount
           discrete : annuity due (True) or continuous (False)
         """
-        self.blog = Blog("Deferred Annuity",
-                         Blog.a(x=x, s=s, t=t, b=b, u=u,
+        self.blog = _Blog("Deferred Annuity",
+                         _Blog.a(x=x, s=s, t=t, b=b, u=u,
                                 discrete=discrete, variance=False),
                          levels=self.maxdepth)
         a = self._a_x(x, s=s, b=b, t=t, u=u, 
                           discrete=discrete, depth=self.maxdepth)
         if a is not None:
             print(self.blog, end='')
             return a
@@ -1140,15 +1140,15 @@
                         discrete=discrete, depth=self.maxdepth)
         if a is not None and a_t is not None:
             print(self.blog, end='')
             return a - a_t
         return super().deferred_annuity(x, s=s, b=b, t=t, discrete=discrete)
 
 
-class Blog:
+class _Blog:
     """Helper to track and display recursion progress"""
     _verbose : bool = True
     def __init__(self, *args, levels: int = 3, width: int = 80):
         self.title = ' *' + " ".join(args) + " <--"  # to identify this stack
         self.levels = levels                         # maximum levels to indent
         self.width = width - 3                       # display line width
         self._history = []
@@ -1161,15 +1161,15 @@
         msg = " ".join([a for a in args]) 
         if msg not in self._history:
             self._history.insert(0, msg)
             self._depths.insert(0, depth)
             self._rules.insert(0, rule)
 
     def __len__(self) -> int:
-        return int(Blog._verbose and bool(self._history))
+        return int(_Blog._verbose and bool(self._history))
 
     def __str__(self):
         """Display message history"""
         if not len(self):
             return ''
         _str = self.title + '\n'
         for msg, depth, rule in zip(self._history, self._depths, self._rules):
```

### Comparing `actuarialmath-0.0.7/src/actuarialmath/reserves.py` & `actuarialmath-0.0.8/src/actuarialmath/reserves.py`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.7/src/actuarialmath/selectlife.py` & `actuarialmath-0.0.8/src/actuarialmath/selectlife.py`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.7/src/actuarialmath/sult.py` & `actuarialmath-0.0.8/src/actuarialmath/sult.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 """
 import math
 import numpy as np
 import pandas as pd
 from typing import Dict, Callable
 from actuarialmath.lifetable import LifeTable
 
-def faml_survival(x, t, A = 0.00022, B = 0.0000027, c = 1.124):
-    """SULT default survival function from SOA's `Excel Workbook for FAM-L Tables`"""
-    A, B, c = 0.00022, 0.0000027, 1.124
-    return math.exp(-A*t - (B*c**x*(c**t - 1))/math.log(c))
+# Makeham's Law parameters from SOA’s Excel Workbook for FAM-L Tables
+_A, _B, _c = 0.00022, 0.0000027, 1.124
+def _faml_sult(x, t: float) -> float:
+    return math.exp(-_A*t - (_B*_c**x*(_c**t - 1)) / math.log(_c))
 
 class SULT(LifeTable):
     """Generates and uses a standard ultimate life table
 
     Args:
       i : interest rate
       radix : initial number of lives
       minage : minimum age
       maxage : maximum age
       S : survival function, default is Makeham with SOA FAM-L parameters
     """
-    
+
+
     def __init__(self, i: float = 0.05, radix: int = 100000, 
-                 S: Callable[[float, float], float] = faml_survival,
+                 S: Callable[[float, float], float] = _faml_sult,
                  minage: int = 20, maxage: int = 130, **kwargs):
         """Construct SULT"""
         super().__init__(**kwargs)
         l = {t+minage: radix * S(minage, t) for t in range(1+maxage-minage)}
         self.set_interest(i=i).set_table(l=l, minage=minage, maxage=maxage)
 
     def __getitem__(self, col: str) -> Dict[int, float]:
@@ -197,59 +198,10 @@
     print("SOA Question 3.4:  (B) 815")
     sult = SULT()
     mean = sult.p_x(25, t=95-25)
     var = sult.bernoulli(mean, variance=True)
     print(sult.portfolio_percentile(N=4000, mean=mean, variance=var, prob=.1))
     print()
     
-    print("Other usage examples")
-    print(sult.temporary_annuity(80, t=10)*20000) # ~130770
-
-    E = sult.E_x(60, t=5)
-    print(E, E*sult.a_x(65, benefit=(lambda x,t: 1000 + .05*t)))
-
-    print(sult.whole_life_annuity(60))  # 14.9041
-    print(sult.whole_life_annuity(60, discrete=False))  # ~13.9041
-    print(sult.deferred_annuity(60, u=10))  #6.9485
-    print(sult.temporary_annuity(60, t=10))  # 7.9555
-    print(sult.temporary_annuity(60, t=15))  # 10.5282
-    print(sult.temporary_annuity(60, t=10))
-    print(sult.E_x(60, t=10))  #
-    print(sult.temporary_annuity(60, t=10, discrete=False))  # ~7.5341
-    print(sult.certain_life_annuity(60, u=10))  # 15.0563
-    print(sult.whole_life_annuity(60, variance=True, discrete=False)) # ~10.6182
-    print(sult.endowment_insurance(60, t=10)) # .62116
-    print(sult.whole_life_insurance(60, moment=2)) # .10834
-    print(sult.whole_life_insurance(70, moment=2)) # .21467
-    print(sult.endowment_insurance(60, t=10, moment=2)) # .38732
-    print(sult.temporary_annuity(60, t=10, variance=True)) #.6513
-
-
-    print(sult.p_x(70)) # 0.989587
-    print(math.log(sult.p_x(70, t=2)) / -2)  # 0.011103
-
-    A1 = sult.whole_life_insurance(20, discrete=False)
-    #print(A1, sult.whole_life(20))
-    A2 = sult.whole_life_insurance(50, discrete=False)
-    #print(A2, sult.whole_life(50))
-    A3 = sult.whole_life_insurance(70, discrete=False)
-    E2 = sult.E_x(20, t=30)
-    E3 = sult.E_x(20, t=50)
-    print(A1, E2, A2, E3, A3, 125*A1 + E2*175*A2 - E3*250*A3)  # 5,335
-
-    print(sult.whole_life_insurance(50)) # .18931
-    print(sult.term_insurance(50, t=20)) # .0402
-    print(sult.endowment_insurance(50, t=20))  # ~.31471
-    print(sult.E_x(50, t=20), 
-          sult.whole_life_insurance(70),
-          sult.deferred_insurance(50, u=20)) # .14911
-
-    print(sult.whole_life_insurance(50, discrete=False)) # .19400
-    print(sult.term_insurance(50, t=20, discrete=False)) # .0412
-    print(sult.endowment_insurance(50, t=20, discrete=False))  #.38944
-    print(sult.E_x(50, t=20), 
-          sult.whole_life_insurance(70, discrete=False),
-          sult.deferred_insurance(50, u=20, discrete=False)) # .15281
-  
     print("Standard Ultimate Life Table at i=0.05")
     print(sult.frame())
     print()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `actuarialmath-0.0.7/src/actuarialmath/survival.py` & `actuarialmath-0.0.8/src/actuarialmath/survival.py`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.7/src/actuarialmath/udd.py` & `actuarialmath-0.0.8/src/actuarialmath/udd.py`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.7/src/actuarialmath/woolhouse.py` & `actuarialmath-0.0.8/src/actuarialmath/woolhouse.py`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.7/src/actuarialmath.egg-info/PKG-INFO` & `actuarialmath-0.0.8/src/actuarialmath.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,88 @@
 Metadata-Version: 2.1
 Name: actuarialmath
-Version: 0.0.7
-Summary: A package for life contingent risks
+Version: 0.0.8
+Summary: A package for actuarial math and life contingent risks
 Author: Terence Lim
-Project-URL: Homepage, https://github.com/terence-lim/actuarialmath
+Project-URL: Homepage, https://terence-lim.github.io/actuarialmath-tutorial
 Project-URL: Bug Tracker, https://github.com/terence-lim/actuarialmath/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 actuarialmath - Life Contingent Risks with Python
 =================================================
 
-This package implements fundamental methods for modeling life contingent risks, and closely follows traditional topics covered in actuarial exams and standard texts such as the "Fundamentals of Actuarial Math - Long-term" exam syllabus by the Society of Actuaries, and "Actuarial Mathematics for Life Contingent Risks" by Dickson, Hardy and Waters.
+This Python package implements fundamental methods for modeling life contingent risks, and closely follows the coverage of traditional topics in actuarial exams and standard texts such as the "Fundamentals of Actuarial Math - Long-term" exam syllabus by the Society of Actuaries, and "Actuarial Mathematics for Life Contingent Risks" by Dickson, Hardy and Waters.
 
 Overview
 --------
 
 The package comprises three sets of classes, which:
 
-1. Implement general actuarial concepts
-   
-   a. Basic interest theory and probability laws
-   b. Survival functions, future lifetimes and fractional ages
-   c. Insurance, annuity, premiums, policy values, and reserves calculations
-      
-2. Adjust results for
-   
-   a. Extra risks
-   b. 1/mthly payments using UDD or Woolhouse approaches
-      
-3. Specify and load a particular form of assumptions
-   
-   a. Life table, select life table, or standard ultimate life table
-   b. Mortality laws, such as constant force of maturity, beta and uniform distributions, or Makeham's and Gompertz's laws
-   c. Recursion inputs
+1. Implement general actuarial methods
+
+   - Basic interest theory and probability laws
+
+   - Survival functions, expected future lifetimes and fractional ages
+
+   - Insurance, annuity, premiums, policy values, and reserves calculations
+
+
+2. Specify and load a particular form of assumptions
+
+   - Life table, select life table, or standard ultimate life table
+
+   - Mortality laws, such as constant force of maturity, beta and uniform distributions, or Makeham's and Gompertz's laws
+
+   - Recursion inputs
+
+3. Adjust results for
+
+   - Extra mortality risks
+
+   - 1/mthly payment frequency using UDD or Woolhouse approaches
 
 Quick Start
 -----------
 
 1. ``pip install actuarialmath``
-2. Select a suitable subclass to initialize with your actuarial assumptions, such as `MortalityLaws` (or a special law like `ConstantForce`), `LifeTable`, `SULT`, `SelectTable` or `Recursion`.
-3. Call appropriate methods to compute intermediate or final results, or to `solve` parameter values implicitly.
-4. If needed, adjust the answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes.
+   
+   - also requires `numpy`, `scipy`, `matplotlib` and `pandas`.
+     
+2. Start Python (version >= 3.10) or Jupyter-notebook
+
+   - Select a suitable subclass to initialize with your actuarial assumptions, such as `MortalityLaws` (or a special law like `ConstantForce`), `LifeTable`, `SULT`, `SelectLife` or `Recursion`.
+      
+   - Call appropriate methods to compute intermediate or final results, or to `solve` parameter values implicitly.
+
+   - If needed, adjust the answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes.
 
 Examples
 --------
 
 ::
 
   # SOA FAM-L sample question 5.7
   from actuarialmath.recursion import Recursion
   from actuarialmath.woolhouse import Woolhouse
   # initialize Recursion class with actuarial inputs
-  life = Recursion().set_interest(i=0.04)\\
-                    .set_A(0.188, x=35)\\
-                    .set_A(0.498, x=65)\\
+  life = Recursion().set_interest(i=0.04)\
+                    .set_A(0.188, x=35)\
+                    .set_A(0.498, x=65)\
                     .set_p(0.883, x=35, t=30)
   # modfy the standard results with Woolhouse mthly approximation
   mthly = Woolhouse(m=2, life=life, three_term=False)
   # compute the desired temporary annuity value
   print(1000 * mthly.temporary_annuity(35, t=30)) #   solution = 17376.7
 
-::  
+::
 
   # SOA FAM-L sample question 7.20
   from actuarialmath.sult import SULT   # use Standard Ultimate Life Table
   from actuarialmath.policyvalues import Contract
   life = SULT()
   # compute the required FPT policy value
   S = life.FPT_policy_value(35, t=1, b=1000)  # is always 0 in year 1!
@@ -80,20 +93,19 @@
                       renewal_premium=.04,
                       renewal_policy=30)
   # compute gross premium using the equivalence principle
   G = life.gross_premium(A=life.whole_life_insurance(35), **contract.premium_terms)
   # compute the required policy value
   R = life.gross_policy_value(35, t=1, contract=contract.set_contract(premium=G))
   print(R-S)   # solution = -277.19
-   
 
 Resources
 ---------
 
 1. `Colab <https://colab.research.google.com/drive/1TcNr1x5HbT2fF3iFMYGXdN_cvRKiSua4?usp=sharing>`_ or `Jupyter notebook <https://terence-lim.github.io/notes/faml.ipynb>`_, to solve all sample SOA FAM-L exam questions
 
 2. `Online tutorial <https://terence-lim.github.io/actuarialmath-tutorial/>`_, or `download pdf <https://terence-lim.github.io/notes/actuarialmath-tutorial.pdf>`_
 
-3. `Code documentation <https://terence-lim.github.io/actuarialmath-docs/>`_
+3. `Code documentation <https://actuarialmath.readthedocs.io/en/latest/>`_
 
 4. `Github repo <https://github.com/terence-lim/actuarialmath.git>`_ and `issues <https://github.com/terence-lim/actuarialmath/issues>`_
```

### Comparing `actuarialmath-0.0.7/src/actuarialmath.egg-info/SOURCES.txt` & `actuarialmath-0.0.8/src/actuarialmath.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 src/actuarialmath/sult.py
 src/actuarialmath/survival.py
 src/actuarialmath/udd.py
 src/actuarialmath/woolhouse.py
 src/actuarialmath.egg-info/PKG-INFO
 src/actuarialmath.egg-info/SOURCES.txt
 src/actuarialmath.egg-info/dependency_links.txt
+src/actuarialmath.egg-info/requires.txt
 src/actuarialmath.egg-info/top_level.txt
```

