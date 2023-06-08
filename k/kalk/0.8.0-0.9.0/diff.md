# Comparing `tmp/kalk-0.8.0.tar.gz` & `tmp/kalk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kalk-0.8.0.tar", last modified: Sat Sep 26 13:29:42 2020, max compression
+gzip compressed data, was "kalk-0.9.0.tar", last modified: Mon Dec  6 14:32:30 2021, max compression
```

## Comparing `kalk-0.8.0.tar` & `kalk-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2020-09-26 13:29:42.954546 kalk-0.8.0/
--rw-rw-rw-   0        0        0     3705 2020-09-26 13:29:42.954546 kalk-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     2243 2020-09-25 10:45:45.000000 kalk-0.8.0/README.rst
-drwxrwxrwx   0        0        0        0 2020-09-26 13:29:42.938926 kalk-0.8.0/_kalk/
--rw-rw-rw-   0        0        0     5501 2020-09-26 13:29:42.000000 kalk-0.8.0/_kalk/__init__.py
-drwxrwxrwx   0        0        0        0 2020-09-26 13:29:42.938926 kalk-0.8.0/kalk.egg-info/
--rw-rw-rw-   0        0        0     3705 2020-09-26 13:29:42.000000 kalk-0.8.0/kalk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2020-09-26 13:29:42.000000 kalk-0.8.0/kalk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-09-26 13:29:42.000000 kalk-0.8.0/kalk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2020-09-26 13:29:42.000000 kalk-0.8.0/kalk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2020-09-26 13:29:42.000000 kalk-0.8.0/kalk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2020-09-26 13:29:42.000000 kalk-0.8.0/kalk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2020-09-19 09:36:32.000000 kalk-0.8.0/kalk.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2020-09-26 13:29:42.954546 kalk-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0      989 2020-09-26 13:29:42.000000 kalk-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2021-12-06 14:32:30.415134 kalk-0.9.0/
+-rw-rw-rw-   0        0        0    35149 2020-09-16 18:49:33.000000 kalk-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0     2975 2021-12-06 14:32:30.415134 kalk-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2243 2021-03-12 10:17:07.000000 kalk-0.9.0/README.rst
+drwxrwxrwx   0        0        0        0 2021-12-06 14:32:30.399513 kalk-0.9.0/_kalk/
+-rw-rw-rw-   0        0        0     5537 2021-12-06 14:32:28.000000 kalk-0.9.0/_kalk/__init__.py
+drwxrwxrwx   0        0        0        0 2021-12-06 14:32:30.415134 kalk-0.9.0/kalk.egg-info/
+-rw-rw-rw-   0        0        0     2975 2021-12-06 14:32:30.000000 kalk-0.9.0/kalk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2021-12-06 14:32:30.000000 kalk-0.9.0/kalk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-12-06 14:32:30.000000 kalk-0.9.0/kalk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2021-12-06 14:32:30.000000 kalk-0.9.0/kalk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2021-12-06 14:32:30.000000 kalk-0.9.0/kalk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2021-12-06 14:32:30.000000 kalk-0.9.0/kalk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2020-09-19 09:36:32.000000 kalk-0.9.0/kalk.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      248 2021-12-06 14:30:37.000000 kalk-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0      839 2021-12-06 14:32:30.415134 kalk-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     2822 2020-09-26 13:28:56.000000 kalk-0.9.0/test.py
```

### Comparing `kalk-0.8.0/README.rst` & `kalk-0.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 Kalk follows Python syntax for numbers. It even support complex numbers.
 
 .. code-block:: python
 
     >>> 1-.1e2J
     (1-10j)
 
-Therefore ``**`` is the `power operator`_ and ``^`` is `bitwise and`_:
+Therefore ``**`` is the `power operator`_ and ``^`` is `bitwise XOR`_:
 
 .. code-block:: python
 
     >>> 3 3 **
     27
     >>> 3 3 ^
     0
@@ -83,11 +83,11 @@
 * ``rep`` repeats the last result
 * ``s`` prints the stack
 * ``sto`` stores the value before the last in storage using the last stack value as the key.
 * ``rcl`` recalls the value in storage using the last stack value as the key.
 
 .. _RPN: https://en.wikipedia.org/wiki/Reverse_Polish_notation
 .. _power operator: https://docs.python.org/3/reference/expressions.html#the-power-operator
-.. _bitwise and: https://docs.python.org/3/reference/expressions.html#binary-bitwise-operations
+.. _bitwise XOR: https://docs.python.org/3/reference/expressions.html#binary-bitwise-operations
 .. _math: https://docs.python.org/3/library/math.html
 .. _operator: https://docs.python.org/3/library/operator.html
 .. _Euler's number: https://en.wikipedia.org/wiki/E_(mathematical_constant)
```

### Comparing `kalk-0.8.0/_kalk/__init__.py` & `kalk-0.9.0/_kalk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
 
 from math import sin, cos, tan, atan, atan2, atanh, asin, asinh, acos, acosh,\
     factorial, pi, e, ceil, comb, floor, fsum, gcd, lcm, perm, prod, trunc, \
     exp, expm1, log, log10, sqrt, dist, hypot, degrees, radians, erf, erfc,\
     gamma, lgamma, tau, copysign, fabs, fmod, isqrt, ldexp, nextafter,\
     remainder, ulp, log1p, log2, pow as fpow, inf, nan
@@ -133,15 +133,17 @@
 
 def recall():
     APPEND(STORAGE[POP()])
 
 
 BINARY_OPERATORS = {
     '%%': percent,
+    '٪٪': percent,
     '%': mod,
+    '٪': mod,
     '&': and_,
     '*': mul,
     '**': pow,
     '+': add,
     '-': sub,
     'n': neg,
     '/': truediv,
```

