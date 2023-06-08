# Comparing `tmp/pari-jupyter-1.4.1.tar.gz` & `tmp/pari-jupyter-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pari-jupyter-1.4.1.tar", last modified: Tue Jan 25 09:19:29 2022, max compression
+gzip compressed data, was "pari-jupyter-1.4.2.tar", last modified: Thu Jun  8 09:41:23 2023, max compression
```

## Comparing `pari-jupyter-1.4.1.tar` & `pari-jupyter-1.4.2.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2022-01-25 09:19:29.391049 pari-jupyter-1.4.1/
--rw-r--r--   0 vincent   (1000) vincent   (1000)    35142 2021-12-30 11:04:11.000000 pari-jupyter-1.4.1/LICENSE
--rw-r--r--   0 vincent   (1000) vincent   (1000)       89 2021-12-30 11:04:11.000000 pari-jupyter-1.4.1/MANIFEST.in
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2022-01-25 09:19:29.314383 pari-jupyter-1.4.1/PARIKernel/
--rw-r--r--   0 vincent   (1000) vincent   (1000)       22 2022-01-25 09:18:48.000000 pari-jupyter-1.4.1/PARIKernel/__init__.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)      129 2021-12-30 11:04:11.000000 pari-jupyter-1.4.1/PARIKernel/__main__.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)   204150 2021-12-31 12:26:45.000000 pari-jupyter-1.4.1/PARIKernel/io.c
--rw-r--r--   0 vincent   (1000) vincent   (1000)      164 2021-12-30 11:04:11.000000 pari-jupyter-1.4.1/PARIKernel/io.pxd
--rw-r--r--   0 vincent   (1000) vincent   (1000)     2567 2021-12-31 12:26:01.000000 pari-jupyter-1.4.1/PARIKernel/io.pyx
--rw-r--r--   0 vincent   (1000) vincent   (1000)   351360 2021-12-31 12:26:45.000000 pari-jupyter-1.4.1/PARIKernel/kernel.c
--rw-r--r--   0 vincent   (1000) vincent   (1000)     7751 2021-12-31 12:26:01.000000 pari-jupyter-1.4.1/PARIKernel/kernel.pyx
--rw-r--r--   0 vincent   (1000) vincent   (1000)     1943 2021-12-30 11:04:11.000000 pari-jupyter-1.4.1/PARIKernel/paridecl.pxd
--rw-r--r--   0 vincent   (1000) vincent   (1000)   126360 2021-12-31 12:26:45.000000 pari-jupyter-1.4.1/PARIKernel/svg.c
--rw-r--r--   0 vincent   (1000) vincent   (1000)     1365 2021-12-31 12:26:01.000000 pari-jupyter-1.4.1/PARIKernel/svg.pyx
--rw-r--r--   0 vincent   (1000) vincent   (1000)     1846 2022-01-25 09:19:29.391049 pari-jupyter-1.4.1/PKG-INFO
--rw-r--r--   0 vincent   (1000) vincent   (1000)     1156 2021-12-31 11:36:31.000000 pari-jupyter-1.4.1/README.rst
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2022-01-25 09:19:29.321049 pari-jupyter-1.4.1/gp-mode/
--rw-r--r--   0 vincent   (1000) vincent   (1000)    16637 2021-12-30 11:04:11.000000 pari-jupyter-1.4.1/gp-mode/gp.js
--rw-r--r--   0 vincent   (1000) vincent   (1000)      253 2021-12-30 11:04:11.000000 pari-jupyter-1.4.1/gp-mode/main.js
--rw-r--r--   0 vincent   (1000) vincent   (1000)       56 2021-12-30 11:04:11.000000 pari-jupyter-1.4.1/gp-mode.json
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2022-01-25 09:19:29.351049 pari-jupyter-1.4.1/pari_jupyter.egg-info/
--rw-r--r--   0 vincent   (1000) vincent   (1000)     1846 2022-01-25 09:19:28.000000 pari-jupyter-1.4.1/pari_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 vincent   (1000) vincent   (1000)      561 2022-01-25 09:19:28.000000 pari-jupyter-1.4.1/pari_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)        1 2022-01-25 09:19:28.000000 pari-jupyter-1.4.1/pari_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)       10 2022-01-25 09:19:28.000000 pari-jupyter-1.4.1/pari_jupyter.egg-info/requires.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)       11 2022-01-25 09:19:28.000000 pari-jupyter-1.4.1/pari_jupyter.egg-info/top_level.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)       60 2021-12-31 11:49:24.000000 pari-jupyter-1.4.1/pyproject.toml
--rw-r--r--   0 vincent   (1000) vincent   (1000)       38 2022-01-25 09:19:29.391049 pari-jupyter-1.4.1/setup.cfg
--rwxr-xr-x   0 vincent   (1000) vincent   (1000)     2644 2021-12-30 11:04:11.000000 pari-jupyter-1.4.1/setup.py
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2022-01-25 09:19:29.371049 pari-jupyter-1.4.1/spec/
--rw-r--r--   0 vincent   (1000) vincent   (1000)     1099 2021-12-30 11:04:11.000000 pari-jupyter-1.4.1/spec/kernel.js
--rw-r--r--   0 vincent   (1000) vincent   (1000)      153 2021-12-30 11:04:11.000000 pari-jupyter-1.4.1/spec/kernel.json
--rw-r--r--   0 vincent   (1000) vincent   (1000)     2986 2021-12-30 11:04:11.000000 pari-jupyter-1.4.1/spec/logo-64x64.png
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2022-01-25 09:19:29.371049 pari-jupyter-1.4.1/test/
--rw-r--r--   0 vincent   (1000) vincent   (1000)     4328 2021-12-31 12:13:46.000000 pari-jupyter-1.4.1/test/test_pari_jupyter_kernel.py
+drwxrwxr-x   0 doctorant  (1000) doctorant  (1000)        0 2023-06-08 09:41:23.221112 pari-jupyter-1.4.2/
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)    35142 2023-06-08 08:24:13.000000 pari-jupyter-1.4.2/LICENSE
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)       89 2023-06-08 08:24:13.000000 pari-jupyter-1.4.2/MANIFEST.in
+drwxrwxr-x   0 doctorant  (1000) doctorant  (1000)        0 2023-06-08 09:41:23.221112 pari-jupyter-1.4.2/PARIKernel/
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)       22 2023-06-08 09:40:20.000000 pari-jupyter-1.4.2/PARIKernel/__init__.py
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)      129 2023-06-08 08:24:13.000000 pari-jupyter-1.4.2/PARIKernel/__main__.py
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)   204449 2023-06-08 08:24:26.000000 pari-jupyter-1.4.2/PARIKernel/io.c
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)      164 2023-06-08 08:24:13.000000 pari-jupyter-1.4.2/PARIKernel/io.pxd
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     2567 2023-06-08 08:24:13.000000 pari-jupyter-1.4.2/PARIKernel/io.pyx
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)   354239 2023-06-08 09:35:43.000000 pari-jupyter-1.4.2/PARIKernel/kernel.c
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     8037 2023-06-08 09:38:13.000000 pari-jupyter-1.4.2/PARIKernel/kernel.pyx
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     2147 2023-06-08 08:24:13.000000 pari-jupyter-1.4.2/PARIKernel/paridecl.pxd
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)   126598 2023-06-08 08:24:26.000000 pari-jupyter-1.4.2/PARIKernel/svg.c
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     1365 2023-06-08 08:24:13.000000 pari-jupyter-1.4.2/PARIKernel/svg.pyx
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     1846 2023-06-08 09:41:23.221112 pari-jupyter-1.4.2/PKG-INFO
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     1156 2023-06-08 08:24:13.000000 pari-jupyter-1.4.2/README.rst
+drwxrwxr-x   0 doctorant  (1000) doctorant  (1000)        0 2023-06-08 09:41:23.221112 pari-jupyter-1.4.2/gp-mode/
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)    16637 2023-06-08 08:24:13.000000 pari-jupyter-1.4.2/gp-mode/gp.js
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)      253 2023-06-08 08:24:13.000000 pari-jupyter-1.4.2/gp-mode/main.js
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)       56 2023-06-08 08:24:13.000000 pari-jupyter-1.4.2/gp-mode.json
+drwxrwxr-x   0 doctorant  (1000) doctorant  (1000)        0 2023-06-08 09:41:23.221112 pari-jupyter-1.4.2/pari_jupyter.egg-info/
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     1846 2023-06-08 09:41:23.000000 pari-jupyter-1.4.2/pari_jupyter.egg-info/PKG-INFO
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)      546 2023-06-08 09:41:23.000000 pari-jupyter-1.4.2/pari_jupyter.egg-info/SOURCES.txt
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)        1 2023-06-08 09:41:23.000000 pari-jupyter-1.4.2/pari_jupyter.egg-info/dependency_links.txt
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)       10 2023-06-08 09:41:23.000000 pari-jupyter-1.4.2/pari_jupyter.egg-info/requires.txt
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)       11 2023-06-08 09:41:23.000000 pari-jupyter-1.4.2/pari_jupyter.egg-info/top_level.txt
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)       38 2023-06-08 09:41:23.221112 pari-jupyter-1.4.2/setup.cfg
+-rwxrwxr-x   0 doctorant  (1000) doctorant  (1000)     2644 2023-06-08 08:24:13.000000 pari-jupyter-1.4.2/setup.py
+drwxrwxr-x   0 doctorant  (1000) doctorant  (1000)        0 2023-06-08 09:41:23.221112 pari-jupyter-1.4.2/spec/
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     1099 2023-06-08 08:24:13.000000 pari-jupyter-1.4.2/spec/kernel.js
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)      153 2023-06-08 08:24:13.000000 pari-jupyter-1.4.2/spec/kernel.json
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     2986 2023-06-08 08:24:13.000000 pari-jupyter-1.4.2/spec/logo-64x64.png
+drwxrwxr-x   0 doctorant  (1000) doctorant  (1000)        0 2023-06-08 09:41:23.221112 pari-jupyter-1.4.2/test/
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     4328 2023-06-08 08:24:13.000000 pari-jupyter-1.4.2/test/test_pari_jupyter_kernel.py
```

### Comparing `pari-jupyter-1.4.1/LICENSE` & `pari-jupyter-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pari-jupyter-1.4.1/PARIKernel/io.c` & `pari-jupyter-1.4.2/PARIKernel/io.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.26 */
+/* Generated by Cython 0.29.28 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_26"
-#define CYTHON_HEX_VERSION 0x001D1AF0
+#define CYTHON_ABI "0_29_28"
+#define CYTHON_HEX_VERSION 0x001D1CF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -168,30 +168,36 @@
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
     #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
@@ -2731,21 +2737,21 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
```

### Comparing `pari-jupyter-1.4.1/PARIKernel/io.pyx` & `pari-jupyter-1.4.2/PARIKernel/io.pyx`

 * *Files identical despite different names*

### Comparing `pari-jupyter-1.4.1/PARIKernel/kernel.c` & `pari-jupyter-1.4.2/PARIKernel/kernel.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.26 */
+/* Generated by Cython 0.29.28 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_26"
-#define CYTHON_HEX_VERSION 0x001D1AF0
+#define CYTHON_ABI "0_29_28"
+#define CYTHON_HEX_VERSION 0x001D1CF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -168,30 +168,36 @@
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
     #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
@@ -1249,14 +1255,20 @@
 
 /* BytesEquals.proto */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* UnicodeEquals.proto */
 static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
 
+/* ArgTypeTest.proto */
+#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
+    ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
+        __Pyx__ArgTypeTest(obj, type, name, exact))
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
+
 /* SliceObject.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetSlice(
         PyObject* obj, Py_ssize_t cstart, Py_ssize_t cstop,
         PyObject** py_start, PyObject** py_stop, PyObject** py_slice,
         int has_cstart, int has_cstop, int wraparound);
 
 /* TypeImport.proto */
@@ -1518,14 +1530,15 @@
 static const char __pyx_k_major[] = "major";
 static const char __pyx_k_minor[] = "minor";
 static const char __pyx_k_patch[] = "patch";
 static const char __pyx_k_reply[] = "reply";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_super[] = "super";
 static const char __pyx_k_width[] = "width";
+static const char __pyx_k_wt_ms[] = "wt_ms";
 static const char __pyx_k_Kernel[] = "Kernel";
 static const char __pyx_k_banner[] = "banner";
 static const char __pyx_k_evalue[] = "evalue";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_height[] = "height";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_length[] = "length";
@@ -1708,14 +1721,15 @@
 static PyObject *__pyx_n_u_traceback;
 static PyObject *__pyx_n_s_user_expressions;
 static PyObject *__pyx_n_u_user_expressions;
 static PyObject *__pyx_n_s_version;
 static PyObject *__pyx_n_s_width;
 static PyObject *__pyx_n_u_width;
 static PyObject *__pyx_n_s_word;
+static PyObject *__pyx_n_s_wt_ms;
 static PyObject *__pyx_pf_10PARIKernel_6kernel_init_svg(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10PARIKernel_6kernel_2pari_short_version(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_10PARIKernel_6kernel_10PARIKernel___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args, PyObject *__pyx_v_kwds); /* proto */
 static PyObject *__pyx_pf_10PARIKernel_6kernel_10PARIKernel_2do_execute(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_code, PyObject *__pyx_v_silent, PyObject *__pyx_v_store_history, CYTHON_UNUSED PyObject *__pyx_v_user_expressions, CYTHON_UNUSED PyObject *__pyx_v_allow_stdin); /* proto */
 static PyObject *__pyx_pf_10PARIKernel_6kernel_10PARIKernel_4do_complete(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_code, PyObject *__pyx_v_cursor_pos); /* proto */
 static PyObject *__pyx_pf_10PARIKernel_6kernel_10PARIKernel_6do_inspect(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_code, PyObject *__pyx_v_cursor_pos, CYTHON_UNUSED PyObject *__pyx_v_detail_level); /* proto */
 static PyObject *__pyx_pf_10PARIKernel_6kernel_10PARIKernel_8publish_svg(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_svg, PyObject *__pyx_v_width, PyObject *__pyx_v_height); /* proto */
@@ -1742,34 +1756,34 @@
 static PyObject *__pyx_codeobj__21;
 /* Late includes */
 
 /* "PARIKernel/kernel.pyx":41
  * cdef sigjmp_buf context
  * 
  * cdef void pari_recover(long numerr) nogil:             # <<<<<<<<<<<<<<
- *     siglongjmp(context, -1)
+ *     siglongjmp(context, numerr)
  * 
  */
 
-static void __pyx_f_10PARIKernel_6kernel_pari_recover(CYTHON_UNUSED long __pyx_v_numerr) {
+static void __pyx_f_10PARIKernel_6kernel_pari_recover(long __pyx_v_numerr) {
 
   /* "PARIKernel/kernel.pyx":42
  * 
  * cdef void pari_recover(long numerr) nogil:
- *     siglongjmp(context, -1)             # <<<<<<<<<<<<<<
+ *     siglongjmp(context, numerr)             # <<<<<<<<<<<<<<
  * 
  * # Global PARI readline interface
  */
-  siglongjmp(__pyx_v_10PARIKernel_6kernel_context, -1);
+  siglongjmp(__pyx_v_10PARIKernel_6kernel_context, __pyx_v_numerr);
 
   /* "PARIKernel/kernel.pyx":41
  * cdef sigjmp_buf context
  * 
  * cdef void pari_recover(long numerr) nogil:             # <<<<<<<<<<<<<<
- *     siglongjmp(context, -1)
+ *     siglongjmp(context, numerr)
  * 
  */
 
   /* function exit code */
 }
 
 /* "PARIKernel/kernel.pyx":51
@@ -2613,14 +2627,15 @@
   pari_sp __pyx_v_av;
   GEN __pyx_v_result;
   char const *__pyx_v_gp_code;
   struct sigaction __pyx_v_sa;
   struct sigaction __pyx_v_old_sa;
   int __pyx_v_err;
   long __pyx_v_t_ms;
+  long __pyx_v_wt_ms;
   char __pyx_v_last;
   PyObject *__pyx_v_content = NULL;
   PyObject *__pyx_v_reply = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   char const *__pyx_t_2;
@@ -2628,14 +2643,15 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
+  pari_sp __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("do_execute", 0);
   __Pyx_INCREF(__pyx_v_code);
 
   /* "PARIKernel/kernel.pyx":113
@@ -2724,106 +2740,124 @@
  *         memset(&sa, 0, sizeof(sa))
  *         sa.sa_handler = pari_sighandler             # <<<<<<<<<<<<<<
  * 
  *         cdef int err
  */
   __pyx_v_sa.sa_handler = pari_sighandler;
 
-  /* "PARIKernel/kernel.pyx":129
- *         cdef long t_ms
+  /* "PARIKernel/kernel.pyx":130
  *         cdef char last
+ * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             err = sigsetjmp(context, 1)
  *             if err == 0:  # Initial sigsetjmp() call
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "PARIKernel/kernel.pyx":130
- *         cdef char last
+        /* "PARIKernel/kernel.pyx":131
+ * 
  *         with nogil:
  *             err = sigsetjmp(context, 1)             # <<<<<<<<<<<<<<
  *             if err == 0:  # Initial sigsetjmp() call
  *                 sigaction(SIGINT, &sa, &old_sa)  # Handle SIGINT by PARI
  */
         __pyx_v_err = sigsetjmp(__pyx_v_10PARIKernel_6kernel_context, 1);
 
-        /* "PARIKernel/kernel.pyx":131
+        /* "PARIKernel/kernel.pyx":132
  *         with nogil:
  *             err = sigsetjmp(context, 1)
  *             if err == 0:  # Initial sigsetjmp() call             # <<<<<<<<<<<<<<
  *                 sigaction(SIGINT, &sa, &old_sa)  # Handle SIGINT by PARI
  *                 timer_start(GP_DATA.T)
  */
         __pyx_t_6 = ((__pyx_v_err == 0) != 0);
         if (__pyx_t_6) {
 
-          /* "PARIKernel/kernel.pyx":132
+          /* "PARIKernel/kernel.pyx":133
  *             err = sigsetjmp(context, 1)
  *             if err == 0:  # Initial sigsetjmp() call
  *                 sigaction(SIGINT, &sa, &old_sa)  # Handle SIGINT by PARI             # <<<<<<<<<<<<<<
  *                 timer_start(GP_DATA.T)
- *                 result = gp_read_str_multiline(gp_code, &last)
+ *                 walltimer_start(GP_DATA.Tw)
  */
           (void)(sigaction(SIGINT, (&__pyx_v_sa), (&__pyx_v_old_sa)));
 
-          /* "PARIKernel/kernel.pyx":133
+          /* "PARIKernel/kernel.pyx":134
  *             if err == 0:  # Initial sigsetjmp() call
  *                 sigaction(SIGINT, &sa, &old_sa)  # Handle SIGINT by PARI
  *                 timer_start(GP_DATA.T)             # <<<<<<<<<<<<<<
+ *                 walltimer_start(GP_DATA.Tw)
  *                 result = gp_read_str_multiline(gp_code, &last)
- *                 t_ms = timer_delay(GP_DATA.T)
  */
           timer_start(GP_DATA->T);
 
-          /* "PARIKernel/kernel.pyx":134
+          /* "PARIKernel/kernel.pyx":135
  *                 sigaction(SIGINT, &sa, &old_sa)  # Handle SIGINT by PARI
  *                 timer_start(GP_DATA.T)
+ *                 walltimer_start(GP_DATA.Tw)             # <<<<<<<<<<<<<<
+ *                 result = gp_read_str_multiline(gp_code, &last)
+ *                 t_ms = timer_delay(GP_DATA.T)
+ */
+          (void)(walltimer_start(GP_DATA->Tw));
+
+          /* "PARIKernel/kernel.pyx":136
+ *                 timer_start(GP_DATA.T)
+ *                 walltimer_start(GP_DATA.Tw)
  *                 result = gp_read_str_multiline(gp_code, &last)             # <<<<<<<<<<<<<<
  *                 t_ms = timer_delay(GP_DATA.T)
- *             sigaction(SIGINT, &old_sa, &sa)      # Restore Python SIGINT handler
+ *                 wt_ms = walltimer_delay(GP_DATA.Tw)
  */
           __pyx_v_result = gp_read_str_multiline(__pyx_v_gp_code, (&__pyx_v_last));
 
-          /* "PARIKernel/kernel.pyx":135
- *                 timer_start(GP_DATA.T)
+          /* "PARIKernel/kernel.pyx":137
+ *                 walltimer_start(GP_DATA.Tw)
  *                 result = gp_read_str_multiline(gp_code, &last)
  *                 t_ms = timer_delay(GP_DATA.T)             # <<<<<<<<<<<<<<
+ *                 wt_ms = walltimer_delay(GP_DATA.Tw)
  *             sigaction(SIGINT, &old_sa, &sa)      # Restore Python SIGINT handler
- * 
  */
           __pyx_v_t_ms = timer_delay(GP_DATA->T);
 
-          /* "PARIKernel/kernel.pyx":131
+          /* "PARIKernel/kernel.pyx":138
+ *                 result = gp_read_str_multiline(gp_code, &last)
+ *                 t_ms = timer_delay(GP_DATA.T)
+ *                 wt_ms = walltimer_delay(GP_DATA.Tw)             # <<<<<<<<<<<<<<
+ *             sigaction(SIGINT, &old_sa, &sa)      # Restore Python SIGINT handler
+ * 
+ */
+          __pyx_v_wt_ms = walltimer_delay(GP_DATA->Tw);
+
+          /* "PARIKernel/kernel.pyx":132
  *         with nogil:
  *             err = sigsetjmp(context, 1)
  *             if err == 0:  # Initial sigsetjmp() call             # <<<<<<<<<<<<<<
  *                 sigaction(SIGINT, &sa, &old_sa)  # Handle SIGINT by PARI
  *                 timer_start(GP_DATA.T)
  */
         }
 
-        /* "PARIKernel/kernel.pyx":136
- *                 result = gp_read_str_multiline(gp_code, &last)
+        /* "PARIKernel/kernel.pyx":139
  *                 t_ms = timer_delay(GP_DATA.T)
+ *                 wt_ms = walltimer_delay(GP_DATA.Tw)
  *             sigaction(SIGINT, &old_sa, &sa)      # Restore Python SIGINT handler             # <<<<<<<<<<<<<<
  * 
- *         if not err:  # success
+ *         if err == 0:  # success
  */
         (void)(sigaction(SIGINT, (&__pyx_v_old_sa), (&__pyx_v_sa)));
       }
 
-      /* "PARIKernel/kernel.pyx":129
- *         cdef long t_ms
+      /* "PARIKernel/kernel.pyx":130
  *         cdef char last
+ * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             err = sigsetjmp(context, 1)
  *             if err == 0:  # Initial sigsetjmp() call
  */
       /*finally:*/ {
         /*normal exit:*/{
           #ifdef WITH_THREAD
@@ -2832,37 +2866,37 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "PARIKernel/kernel.pyx":138
+  /* "PARIKernel/kernel.pyx":141
  *             sigaction(SIGINT, &old_sa, &sa)      # Restore Python SIGINT handler
  * 
- *         if not err:  # success             # <<<<<<<<<<<<<<
+ *         if err == 0:  # success             # <<<<<<<<<<<<<<
  *             if not silent:
  *                 if t_ms and GP_DATA.chrono:
  */
-  __pyx_t_6 = ((!(__pyx_v_err != 0)) != 0);
+  __pyx_t_6 = ((__pyx_v_err == 0) != 0);
   if (__pyx_t_6) {
 
-    /* "PARIKernel/kernel.pyx":139
+    /* "PARIKernel/kernel.pyx":142
  * 
- *         if not err:  # success
+ *         if err == 0:  # success
  *             if not silent:             # <<<<<<<<<<<<<<
  *                 if t_ms and GP_DATA.chrono:
  *                     pari_puts(b"time = ")
  */
-    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_v_silent); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 139, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_v_silent); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 142, __pyx_L1_error)
     __pyx_t_7 = ((!__pyx_t_6) != 0);
     if (__pyx_t_7) {
 
-      /* "PARIKernel/kernel.pyx":140
- *         if not err:  # success
+      /* "PARIKernel/kernel.pyx":143
+ *         if err == 0:  # success
  *             if not silent:
  *                 if t_ms and GP_DATA.chrono:             # <<<<<<<<<<<<<<
  *                     pari_puts(b"time = ")
  *                     pari_puts(gp_format_time(t_ms))
  */
       __pyx_t_6 = (__pyx_v_t_ms != 0);
       if (__pyx_t_6) {
@@ -2871,170 +2905,170 @@
         goto __pyx_L10_bool_binop_done;
       }
       __pyx_t_6 = (GP_DATA->chrono != 0);
       __pyx_t_7 = __pyx_t_6;
       __pyx_L10_bool_binop_done:;
       if (__pyx_t_7) {
 
-        /* "PARIKernel/kernel.pyx":141
+        /* "PARIKernel/kernel.pyx":144
  *             if not silent:
  *                 if t_ms and GP_DATA.chrono:
  *                     pari_puts(b"time = ")             # <<<<<<<<<<<<<<
  *                     pari_puts(gp_format_time(t_ms))
  *                     pari_flush()
  */
         pari_puts(((char *)"time = "));
 
-        /* "PARIKernel/kernel.pyx":142
+        /* "PARIKernel/kernel.pyx":145
  *                 if t_ms and GP_DATA.chrono:
  *                     pari_puts(b"time = ")
  *                     pari_puts(gp_format_time(t_ms))             # <<<<<<<<<<<<<<
  *                     pari_flush()
  * 
  */
         pari_puts(gp_format_time(__pyx_v_t_ms));
 
-        /* "PARIKernel/kernel.pyx":143
+        /* "PARIKernel/kernel.pyx":146
  *                     pari_puts(b"time = ")
  *                     pari_puts(gp_format_time(t_ms))
  *                     pari_flush()             # <<<<<<<<<<<<<<
  * 
  *             # gnil as a result is like Python's None, it should be
  */
         pari_flush();
 
-        /* "PARIKernel/kernel.pyx":140
- *         if not err:  # success
+        /* "PARIKernel/kernel.pyx":143
+ *         if err == 0:  # success
  *             if not silent:
  *                 if t_ms and GP_DATA.chrono:             # <<<<<<<<<<<<<<
  *                     pari_puts(b"time = ")
  *                     pari_puts(gp_format_time(t_ms))
  */
       }
 
-      /* "PARIKernel/kernel.pyx":139
+      /* "PARIKernel/kernel.pyx":142
  * 
- *         if not err:  # success
+ *         if err == 0:  # success
  *             if not silent:             # <<<<<<<<<<<<<<
  *                 if t_ms and GP_DATA.chrono:
  *                     pari_puts(b"time = ")
  */
     }
 
-    /* "PARIKernel/kernel.pyx":147
+    /* "PARIKernel/kernel.pyx":150
  *             # gnil as a result is like Python's None, it should be
  *             # considered as "no result"
  *             if result is not gnil:             # <<<<<<<<<<<<<<
  *                 if store_history:
- *                     pari_add_hist(result, t_ms, t_ms)
+ *                     pari_add_hist(result, t_ms, wt_ms)
  */
     __pyx_t_7 = ((__pyx_v_result != gnil) != 0);
     if (__pyx_t_7) {
 
-      /* "PARIKernel/kernel.pyx":148
+      /* "PARIKernel/kernel.pyx":151
  *             # considered as "no result"
  *             if result is not gnil:
  *                 if store_history:             # <<<<<<<<<<<<<<
- *                     pari_add_hist(result, t_ms, t_ms)
+ *                     pari_add_hist(result, t_ms, wt_ms)
  * 
  */
-      __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_v_store_history); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 148, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_v_store_history); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 151, __pyx_L1_error)
       if (__pyx_t_7) {
 
-        /* "PARIKernel/kernel.pyx":149
+        /* "PARIKernel/kernel.pyx":152
  *             if result is not gnil:
  *                 if store_history:
- *                     pari_add_hist(result, t_ms, t_ms)             # <<<<<<<<<<<<<<
+ *                     pari_add_hist(result, t_ms, wt_ms)             # <<<<<<<<<<<<<<
  * 
  *                 if last != c';' and not silent:
  */
-        pari_add_hist(__pyx_v_result, __pyx_v_t_ms, __pyx_v_t_ms);
+        pari_add_hist(__pyx_v_result, __pyx_v_t_ms, __pyx_v_wt_ms);
 
-        /* "PARIKernel/kernel.pyx":148
+        /* "PARIKernel/kernel.pyx":151
  *             # considered as "no result"
  *             if result is not gnil:
  *                 if store_history:             # <<<<<<<<<<<<<<
- *                     pari_add_hist(result, t_ms, t_ms)
+ *                     pari_add_hist(result, t_ms, wt_ms)
  * 
  */
       }
 
-      /* "PARIKernel/kernel.pyx":151
- *                     pari_add_hist(result, t_ms, t_ms)
+      /* "PARIKernel/kernel.pyx":154
+ *                     pari_add_hist(result, t_ms, wt_ms)
  * 
  *                 if last != c';' and not silent:             # <<<<<<<<<<<<<<
  *                     content = {
  *                         'execution_count': pari_nb_hist(),
  */
       __pyx_t_6 = ((__pyx_v_last != ';') != 0);
       if (__pyx_t_6) {
       } else {
         __pyx_t_7 = __pyx_t_6;
         goto __pyx_L15_bool_binop_done;
       }
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_v_silent); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 151, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_v_silent); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 154, __pyx_L1_error)
       __pyx_t_8 = ((!__pyx_t_6) != 0);
       __pyx_t_7 = __pyx_t_8;
       __pyx_L15_bool_binop_done:;
       if (__pyx_t_7) {
 
-        /* "PARIKernel/kernel.pyx":153
+        /* "PARIKernel/kernel.pyx":156
  *                 if last != c';' and not silent:
  *                     content = {
  *                         'execution_count': pari_nb_hist(),             # <<<<<<<<<<<<<<
  *                         'data': {
  *                             'text/plain': PyUnicode_FromGEN(result),
  */
-        __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_4 = __Pyx_PyInt_From_long(pari_nb_hist()); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 153, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_long(pari_nb_hist()); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 156, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_execution_count, __pyx_t_4) < 0) __PYX_ERR(0, 153, __pyx_L1_error)
+        if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_execution_count, __pyx_t_4) < 0) __PYX_ERR(0, 156, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "PARIKernel/kernel.pyx":155
+        /* "PARIKernel/kernel.pyx":158
  *                         'execution_count': pari_nb_hist(),
  *                         'data': {
  *                             'text/plain': PyUnicode_FromGEN(result),             # <<<<<<<<<<<<<<
  *                         },
  *                         'metadata': {}
  */
-        __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 155, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 158, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_3 = __pyx_f_10PARIKernel_6kernel_PyUnicode_FromGEN(__pyx_v_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
+        __pyx_t_3 = __pyx_f_10PARIKernel_6kernel_PyUnicode_FromGEN(__pyx_v_result); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 158, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (PyDict_SetItem(__pyx_t_4, __pyx_kp_u_text_plain, __pyx_t_3) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
+        if (PyDict_SetItem(__pyx_t_4, __pyx_kp_u_text_plain, __pyx_t_3) < 0) __PYX_ERR(0, 158, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_data, __pyx_t_4) < 0) __PYX_ERR(0, 153, __pyx_L1_error)
+        if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_data, __pyx_t_4) < 0) __PYX_ERR(0, 156, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "PARIKernel/kernel.pyx":157
+        /* "PARIKernel/kernel.pyx":160
  *                             'text/plain': PyUnicode_FromGEN(result),
  *                         },
  *                         'metadata': {}             # <<<<<<<<<<<<<<
  *                     }
  *                     self.send_response(self.iopub_socket, 'execute_result', content)
  */
-        __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 157, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 160, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_metadata, __pyx_t_4) < 0) __PYX_ERR(0, 153, __pyx_L1_error)
+        if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_metadata, __pyx_t_4) < 0) __PYX_ERR(0, 156, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_v_content = ((PyObject*)__pyx_t_1);
         __pyx_t_1 = 0;
 
-        /* "PARIKernel/kernel.pyx":159
+        /* "PARIKernel/kernel.pyx":162
  *                         'metadata': {}
  *                     }
  *                     self.send_response(self.iopub_socket, 'execute_result', content)             # <<<<<<<<<<<<<<
  * 
  *             reply = {'status': 'ok',
  */
-        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_send_response); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 159, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_send_response); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 162, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_iopub_socket); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 159, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_iopub_socket); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_5 = NULL;
         __pyx_t_9 = 0;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_5)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -3043,210 +3077,252 @@
             __Pyx_DECREF_SET(__pyx_t_4, function);
             __pyx_t_9 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_t_3, __pyx_n_u_execute_result, __pyx_v_content};
-          __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
+          __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_t_3, __pyx_n_u_execute_result, __pyx_v_content};
-          __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
+          __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         } else
         #endif
         {
-          __pyx_t_10 = PyTuple_New(3+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 159, __pyx_L1_error)
+          __pyx_t_10 = PyTuple_New(3+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 162, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_10);
           if (__pyx_t_5) {
             __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_5); __pyx_t_5 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_t_3);
           __Pyx_INCREF(__pyx_n_u_execute_result);
           __Pyx_GIVEREF(__pyx_n_u_execute_result);
           PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_n_u_execute_result);
           __Pyx_INCREF(__pyx_v_content);
           __Pyx_GIVEREF(__pyx_v_content);
           PyTuple_SET_ITEM(__pyx_t_10, 2+__pyx_t_9, __pyx_v_content);
           __pyx_t_3 = 0;
-          __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
+          __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "PARIKernel/kernel.pyx":151
- *                     pari_add_hist(result, t_ms, t_ms)
+        /* "PARIKernel/kernel.pyx":154
+ *                     pari_add_hist(result, t_ms, wt_ms)
  * 
  *                 if last != c';' and not silent:             # <<<<<<<<<<<<<<
  *                     content = {
  *                         'execution_count': pari_nb_hist(),
  */
       }
 
-      /* "PARIKernel/kernel.pyx":147
+      /* "PARIKernel/kernel.pyx":150
  *             # gnil as a result is like Python's None, it should be
  *             # considered as "no result"
  *             if result is not gnil:             # <<<<<<<<<<<<<<
  *                 if store_history:
- *                     pari_add_hist(result, t_ms, t_ms)
+ *                     pari_add_hist(result, t_ms, wt_ms)
  */
     }
 
-    /* "PARIKernel/kernel.pyx":161
+    /* "PARIKernel/kernel.pyx":164
  *                     self.send_response(self.iopub_socket, 'execute_result', content)
  * 
  *             reply = {'status': 'ok',             # <<<<<<<<<<<<<<
  *                      'execution_count': pari_nb_hist(),
  *                      'payload': [],
  */
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_status, __pyx_n_u_ok) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_status, __pyx_n_u_ok) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
 
-    /* "PARIKernel/kernel.pyx":162
+    /* "PARIKernel/kernel.pyx":165
  * 
  *             reply = {'status': 'ok',
  *                      'execution_count': pari_nb_hist(),             # <<<<<<<<<<<<<<
  *                      'payload': [],
  *                      'user_expressions': {},
  */
-    __pyx_t_4 = __Pyx_PyInt_From_long(pari_nb_hist()); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_long(pari_nb_hist()); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_execution_count, __pyx_t_4) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_execution_count, __pyx_t_4) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "PARIKernel/kernel.pyx":163
+    /* "PARIKernel/kernel.pyx":166
  *             reply = {'status': 'ok',
  *                      'execution_count': pari_nb_hist(),
  *                      'payload': [],             # <<<<<<<<<<<<<<
  *                      'user_expressions': {},
  *                     }
  */
-    __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_payload, __pyx_t_4) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_payload, __pyx_t_4) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "PARIKernel/kernel.pyx":164
+    /* "PARIKernel/kernel.pyx":167
  *                      'execution_count': pari_nb_hist(),
  *                      'payload': [],
  *                      'user_expressions': {},             # <<<<<<<<<<<<<<
  *                     }
- *         else:  # error (therefore no result)
+ * 
  */
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 167, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_user_expressions, __pyx_t_4) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_user_expressions, __pyx_t_4) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_reply = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "PARIKernel/kernel.pyx":138
+    /* "PARIKernel/kernel.pyx":170
+ *                     }
+ * 
+ *             avma = av             # <<<<<<<<<<<<<<
+ * 
+ *         else:  # error (therefore no result)
+ */
+    avma = __pyx_v_av;
+
+    /* "PARIKernel/kernel.pyx":141
  *             sigaction(SIGINT, &old_sa, &sa)      # Restore Python SIGINT handler
  * 
- *         if not err:  # success             # <<<<<<<<<<<<<<
+ *         if err == 0:  # success             # <<<<<<<<<<<<<<
  *             if not silent:
  *                 if t_ms and GP_DATA.chrono:
  */
     goto __pyx_L7;
   }
 
-  /* "PARIKernel/kernel.pyx":167
- *                     }
+  /* "PARIKernel/kernel.pyx":173
+ * 
  *         else:  # error (therefore no result)
  *             reply = {'status': 'error',             # <<<<<<<<<<<<<<
  *                      'execution_count': pari_nb_hist(),
  *                      'ename': "",
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_status, __pyx_n_u_error) < 0) __PYX_ERR(0, 167, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_status, __pyx_n_u_error) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
 
-    /* "PARIKernel/kernel.pyx":168
+    /* "PARIKernel/kernel.pyx":174
  *         else:  # error (therefore no result)
  *             reply = {'status': 'error',
  *                      'execution_count': pari_nb_hist(),             # <<<<<<<<<<<<<<
  *                      'ename': "",
  *                      'evalue': "",
  */
-    __pyx_t_4 = __Pyx_PyInt_From_long(pari_nb_hist()); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 168, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_long(pari_nb_hist()); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 174, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_execution_count, __pyx_t_4) < 0) __PYX_ERR(0, 167, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_execution_count, __pyx_t_4) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_ename, __pyx_kp_u__2) < 0) __PYX_ERR(0, 167, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_evalue, __pyx_kp_u__2) < 0) __PYX_ERR(0, 167, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_ename, __pyx_kp_u__2) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_evalue, __pyx_kp_u__2) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
 
-    /* "PARIKernel/kernel.pyx":171
+    /* "PARIKernel/kernel.pyx":177
  *                      'ename': "",
  *                      'evalue': "",
  *                      'traceback': [],             # <<<<<<<<<<<<<<
  *                     }
  * 
  */
-    __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 177, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_traceback, __pyx_t_4) < 0) __PYX_ERR(0, 167, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_traceback, __pyx_t_4) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_reply = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
-  }
-  __pyx_L7:;
 
-  /* "PARIKernel/kernel.pyx":174
+    /* "PARIKernel/kernel.pyx":180
  *                     }
  * 
- *         avma = av             # <<<<<<<<<<<<<<
+ *             if err > 0:             # <<<<<<<<<<<<<<
+ *                 # true error
+ *                 avma = av
+ */
+    __pyx_t_7 = ((__pyx_v_err > 0) != 0);
+    if (__pyx_t_7) {
+
+      /* "PARIKernel/kernel.pyx":182
+ *             if err > 0:
+ *                 # true error
+ *                 avma = av             # <<<<<<<<<<<<<<
+ *             else:
+ *                 # allocatemem
+ */
+      avma = __pyx_v_av;
+
+      /* "PARIKernel/kernel.pyx":180
+ *                     }
+ * 
+ *             if err > 0:             # <<<<<<<<<<<<<<
+ *                 # true error
+ *                 avma = av
+ */
+      goto __pyx_L17;
+    }
+
+    /* "PARIKernel/kernel.pyx":185
+ *             else:
+ *                 # allocatemem
+ *                 avma = pari_mainstack.top             # <<<<<<<<<<<<<<
+ * 
  *         self.io.flush()
- *         return reply
  */
-  avma = __pyx_v_av;
+    /*else*/ {
+      __pyx_t_11 = pari_mainstack->top;
+      avma = __pyx_t_11;
+    }
+    __pyx_L17:;
+  }
+  __pyx_L7:;
 
-  /* "PARIKernel/kernel.pyx":175
+  /* "PARIKernel/kernel.pyx":187
+ *                 avma = pari_mainstack.top
  * 
- *         avma = av
  *         self.io.flush()             # <<<<<<<<<<<<<<
  *         return reply
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_io); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_io); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_flush); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_flush); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_10);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_10, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "PARIKernel/kernel.pyx":176
- *         avma = av
+  /* "PARIKernel/kernel.pyx":188
+ * 
  *         self.io.flush()
  *         return reply             # <<<<<<<<<<<<<<
  * 
  *     def do_complete(self, code, cursor_pos):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_reply);
@@ -3275,15 +3351,15 @@
   __Pyx_XDECREF(__pyx_v_reply);
   __Pyx_XDECREF(__pyx_v_code);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "PARIKernel/kernel.pyx":178
+/* "PARIKernel/kernel.pyx":190
  *         return reply
  * 
  *     def do_complete(self, code, cursor_pos):             # <<<<<<<<<<<<<<
  *         cdef long word
  *         cdef char** m = pari_completion_matches(&pari_rl,
  */
 
@@ -3321,40 +3397,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_code)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("do_complete", 1, 3, 3, 1); __PYX_ERR(0, 178, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("do_complete", 1, 3, 3, 1); __PYX_ERR(0, 190, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cursor_pos)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("do_complete", 1, 3, 3, 2); __PYX_ERR(0, 178, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("do_complete", 1, 3, 3, 2); __PYX_ERR(0, 190, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "do_complete") < 0)) __PYX_ERR(0, 178, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "do_complete") < 0)) __PYX_ERR(0, 190, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_code = values[1];
     __pyx_v_cursor_pos = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("do_complete", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 178, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("do_complete", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 190, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("PARIKernel.kernel.PARIKernel.do_complete", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10PARIKernel_6kernel_10PARIKernel_4do_complete(__pyx_self, __pyx_v_self, __pyx_v_code, __pyx_v_cursor_pos);
 
@@ -3378,191 +3454,191 @@
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("do_complete", 0);
 
-  /* "PARIKernel/kernel.pyx":181
+  /* "PARIKernel/kernel.pyx":193
  *         cdef long word
  *         cdef char** m = pari_completion_matches(&pari_rl,
  *                 (<unicode?>code).encode("utf-8"), cursor_pos, &word)             # <<<<<<<<<<<<<<
  * 
  *         cdef list matches = []
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_code))||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_code)->tp_name), 0))) __PYX_ERR(0, 181, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_code))||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_code)->tp_name), 0))) __PYX_ERR(0, 193, __pyx_L1_error)
   if (unlikely(__pyx_v_code == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 181, __pyx_L1_error)
+    __PYX_ERR(0, 193, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_AsUTF8String(((PyObject*)__pyx_v_code)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_AsUTF8String(((PyObject*)__pyx_v_code)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBytes_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyInt_As_long(__pyx_v_cursor_pos); if (unlikely((__pyx_t_3 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_long(__pyx_v_cursor_pos); if (unlikely((__pyx_t_3 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 193, __pyx_L1_error)
 
-  /* "PARIKernel/kernel.pyx":180
+  /* "PARIKernel/kernel.pyx":192
  *     def do_complete(self, code, cursor_pos):
  *         cdef long word
  *         cdef char** m = pari_completion_matches(&pari_rl,             # <<<<<<<<<<<<<<
  *                 (<unicode?>code).encode("utf-8"), cursor_pos, &word)
  * 
  */
   __pyx_v_m = pari_completion_matches((&__pyx_v_10PARIKernel_6kernel_pari_rl), __pyx_t_2, __pyx_t_3, (&__pyx_v_word));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "PARIKernel/kernel.pyx":183
+  /* "PARIKernel/kernel.pyx":195
  *                 (<unicode?>code).encode("utf-8"), cursor_pos, &word)
  * 
  *         cdef list matches = []             # <<<<<<<<<<<<<<
  *         if m != NULL:
  *             if m[1] == NULL:  # Unique match
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_matches = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "PARIKernel/kernel.pyx":184
+  /* "PARIKernel/kernel.pyx":196
  * 
  *         cdef list matches = []
  *         if m != NULL:             # <<<<<<<<<<<<<<
  *             if m[1] == NULL:  # Unique match
  *                 matches = [PyUnicode_FromString(m[0])]
  */
   __pyx_t_4 = ((__pyx_v_m != NULL) != 0);
   if (__pyx_t_4) {
 
-    /* "PARIKernel/kernel.pyx":185
+    /* "PARIKernel/kernel.pyx":197
  *         cdef list matches = []
  *         if m != NULL:
  *             if m[1] == NULL:  # Unique match             # <<<<<<<<<<<<<<
  *                 matches = [PyUnicode_FromString(m[0])]
  *             else:             # Non-unique match
  */
     __pyx_t_4 = (((__pyx_v_m[1]) == NULL) != 0);
     if (__pyx_t_4) {
 
-      /* "PARIKernel/kernel.pyx":186
+      /* "PARIKernel/kernel.pyx":198
  *         if m != NULL:
  *             if m[1] == NULL:  # Unique match
  *                 matches = [PyUnicode_FromString(m[0])]             # <<<<<<<<<<<<<<
  *             else:             # Non-unique match
  *                 while m[1] != NULL:
  */
-      __pyx_t_1 = PyUnicode_FromString((__pyx_v_m[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+      __pyx_t_1 = PyUnicode_FromString((__pyx_v_m[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_5 = PyList_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 186, __pyx_L1_error)
+      __pyx_t_5 = PyList_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_1);
       PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
       __pyx_t_1 = 0;
       __Pyx_DECREF_SET(__pyx_v_matches, ((PyObject*)__pyx_t_5));
       __pyx_t_5 = 0;
 
-      /* "PARIKernel/kernel.pyx":185
+      /* "PARIKernel/kernel.pyx":197
  *         cdef list matches = []
  *         if m != NULL:
  *             if m[1] == NULL:  # Unique match             # <<<<<<<<<<<<<<
  *                 matches = [PyUnicode_FromString(m[0])]
  *             else:             # Non-unique match
  */
       goto __pyx_L4;
     }
 
-    /* "PARIKernel/kernel.pyx":188
+    /* "PARIKernel/kernel.pyx":200
  *                 matches = [PyUnicode_FromString(m[0])]
  *             else:             # Non-unique match
  *                 while m[1] != NULL:             # <<<<<<<<<<<<<<
  *                     matches.append(PyUnicode_FromString(m[1]))
  *                     m += 1
  */
     /*else*/ {
       while (1) {
         __pyx_t_4 = (((__pyx_v_m[1]) != NULL) != 0);
         if (!__pyx_t_4) break;
 
-        /* "PARIKernel/kernel.pyx":189
+        /* "PARIKernel/kernel.pyx":201
  *             else:             # Non-unique match
  *                 while m[1] != NULL:
  *                     matches.append(PyUnicode_FromString(m[1]))             # <<<<<<<<<<<<<<
  *                     m += 1
  * 
  */
-        __pyx_t_5 = PyUnicode_FromString((__pyx_v_m[1])); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 189, __pyx_L1_error)
+        __pyx_t_5 = PyUnicode_FromString((__pyx_v_m[1])); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
-        __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_matches, __pyx_t_5); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 189, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_matches, __pyx_t_5); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-        /* "PARIKernel/kernel.pyx":190
+        /* "PARIKernel/kernel.pyx":202
  *                 while m[1] != NULL:
  *                     matches.append(PyUnicode_FromString(m[1]))
  *                     m += 1             # <<<<<<<<<<<<<<
  * 
  *         reply = dict(status="ok", matches=sorted(matches),
  */
         __pyx_v_m = (__pyx_v_m + 1);
       }
     }
     __pyx_L4:;
 
-    /* "PARIKernel/kernel.pyx":184
+    /* "PARIKernel/kernel.pyx":196
  * 
  *         cdef list matches = []
  *         if m != NULL:             # <<<<<<<<<<<<<<
  *             if m[1] == NULL:  # Unique match
  *                 matches = [PyUnicode_FromString(m[0])]
  */
   }
 
-  /* "PARIKernel/kernel.pyx":192
+  /* "PARIKernel/kernel.pyx":204
  *                     m += 1
  * 
  *         reply = dict(status="ok", matches=sorted(matches),             # <<<<<<<<<<<<<<
  *                 cursor_start=word, cursor_end=cursor_pos)
  *         return reply
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_status, __pyx_n_u_ok) < 0) __PYX_ERR(0, 192, __pyx_L1_error)
-  __pyx_t_7 = PySequence_List(__pyx_v_matches); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 192, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_status, __pyx_n_u_ok) < 0) __PYX_ERR(0, 204, __pyx_L1_error)
+  __pyx_t_7 = PySequence_List(__pyx_v_matches); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_1 = ((PyObject*)__pyx_t_7);
   __pyx_t_7 = 0;
-  __pyx_t_6 = PyList_Sort(__pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 192, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_matches, __pyx_t_1) < 0) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_6 = PyList_Sort(__pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 204, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_matches, __pyx_t_1) < 0) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "PARIKernel/kernel.pyx":193
+  /* "PARIKernel/kernel.pyx":205
  * 
  *         reply = dict(status="ok", matches=sorted(matches),
  *                 cursor_start=word, cursor_end=cursor_pos)             # <<<<<<<<<<<<<<
  *         return reply
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_word); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_word); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_cursor_start, __pyx_t_1) < 0) __PYX_ERR(0, 192, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_cursor_start, __pyx_t_1) < 0) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_cursor_end, __pyx_v_cursor_pos) < 0) __PYX_ERR(0, 192, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_cursor_end, __pyx_v_cursor_pos) < 0) __PYX_ERR(0, 204, __pyx_L1_error)
   __pyx_v_reply = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "PARIKernel/kernel.pyx":194
+  /* "PARIKernel/kernel.pyx":206
  *         reply = dict(status="ok", matches=sorted(matches),
  *                 cursor_start=word, cursor_end=cursor_pos)
  *         return reply             # <<<<<<<<<<<<<<
  * 
  *     def do_inspect(self, code, cursor_pos, detail_level=0):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_reply);
   __pyx_r = __pyx_v_reply;
   goto __pyx_L0;
 
-  /* "PARIKernel/kernel.pyx":178
+  /* "PARIKernel/kernel.pyx":190
  *         return reply
  * 
  *     def do_complete(self, code, cursor_pos):             # <<<<<<<<<<<<<<
  *         cdef long word
  *         cdef char** m = pari_completion_matches(&pari_rl,
  */
 
@@ -3577,15 +3653,15 @@
   __Pyx_XDECREF(__pyx_v_matches);
   __Pyx_XDECREF(__pyx_v_reply);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "PARIKernel/kernel.pyx":196
+/* "PARIKernel/kernel.pyx":208
  *         return reply
  * 
  *     def do_inspect(self, code, cursor_pos, detail_level=0):             # <<<<<<<<<<<<<<
  *         word = self.__get_keyword(code, cursor_pos)[0]
  *         # Possibly rewind if we are right after a "("
  */
 
@@ -3627,31 +3703,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_code)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("do_inspect", 0, 3, 4, 1); __PYX_ERR(0, 196, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("do_inspect", 0, 3, 4, 1); __PYX_ERR(0, 208, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cursor_pos)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("do_inspect", 0, 3, 4, 2); __PYX_ERR(0, 196, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("do_inspect", 0, 3, 4, 2); __PYX_ERR(0, 208, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_detail_level);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "do_inspect") < 0)) __PYX_ERR(0, 196, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "do_inspect") < 0)) __PYX_ERR(0, 208, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -3663,15 +3739,15 @@
     __pyx_v_self = values[0];
     __pyx_v_code = values[1];
     __pyx_v_cursor_pos = values[2];
     __pyx_v_detail_level = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("do_inspect", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 196, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("do_inspect", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 208, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("PARIKernel.kernel.PARIKernel.do_inspect", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10PARIKernel_6kernel_10PARIKernel_6do_inspect(__pyx_self, __pyx_v_self, __pyx_v_code, __pyx_v_cursor_pos, __pyx_v_detail_level);
 
@@ -3697,22 +3773,22 @@
   PyObject *__pyx_t_9 = NULL;
   char *__pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("do_inspect", 0);
 
-  /* "PARIKernel/kernel.pyx":197
+  /* "PARIKernel/kernel.pyx":209
  * 
  *     def do_inspect(self, code, cursor_pos, detail_level=0):
  *         word = self.__get_keyword(code, cursor_pos)[0]             # <<<<<<<<<<<<<<
  *         # Possibly rewind if we are right after a "("
  *         if not word and cursor_pos > 0 and code[cursor_pos-1] == u"(":
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_PARIKernel__get_keyword); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_PARIKernel__get_keyword); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 209, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -3721,93 +3797,93 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_code, __pyx_v_cursor_pos};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 209, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_code, __pyx_v_cursor_pos};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 209, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 209, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_code);
     __Pyx_GIVEREF(__pyx_v_code);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_code);
     __Pyx_INCREF(__pyx_v_cursor_pos);
     __Pyx_GIVEREF(__pyx_v_cursor_pos);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_cursor_pos);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 209, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 209, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_word = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "PARIKernel/kernel.pyx":199
+  /* "PARIKernel/kernel.pyx":211
  *         word = self.__get_keyword(code, cursor_pos)[0]
  *         # Possibly rewind if we are right after a "("
  *         if not word and cursor_pos > 0 and code[cursor_pos-1] == u"(":             # <<<<<<<<<<<<<<
  *             word = self.__get_keyword(code, cursor_pos-1)[0]
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_v_word); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_v_word); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 211, __pyx_L1_error)
   __pyx_t_8 = ((!__pyx_t_7) != 0);
   if (__pyx_t_8) {
   } else {
     __pyx_t_6 = __pyx_t_8;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_2 = PyObject_RichCompare(__pyx_v_cursor_pos, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_v_cursor_pos, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_8) {
   } else {
     __pyx_t_6 = __pyx_t_8;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_PyInt_SubtractObjC(__pyx_v_cursor_pos, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_SubtractObjC(__pyx_v_cursor_pos, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_code, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_code, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_kp_u__3, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_kp_u__3, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_6 = __pyx_t_8;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_6) {
 
-    /* "PARIKernel/kernel.pyx":200
+    /* "PARIKernel/kernel.pyx":212
  *         # Possibly rewind if we are right after a "("
  *         if not word and cursor_pos > 0 and code[cursor_pos-1] == u"(":
  *             word = self.__get_keyword(code, cursor_pos-1)[0]             # <<<<<<<<<<<<<<
  * 
  *         reply = dict(status="ok", found=False, data={}, metadata={})
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_PARIKernel__get_keyword); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 200, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_PARIKernel__get_keyword); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = __Pyx_PyInt_SubtractObjC(__pyx_v_cursor_pos, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 200, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_SubtractObjC(__pyx_v_cursor_pos, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_3 = NULL;
     __pyx_t_4 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -3816,134 +3892,134 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_4 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_code, __pyx_t_5};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_code, __pyx_t_5};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else
     #endif
     {
-      __pyx_t_9 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 200, __pyx_L1_error)
+      __pyx_t_9 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 212, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       if (__pyx_t_3) {
         __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_3); __pyx_t_3 = NULL;
       }
       __Pyx_INCREF(__pyx_v_code);
       __Pyx_GIVEREF(__pyx_v_code);
       PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_4, __pyx_v_code);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_4, __pyx_t_5);
       __pyx_t_5 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 200, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_word, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "PARIKernel/kernel.pyx":199
+    /* "PARIKernel/kernel.pyx":211
  *         word = self.__get_keyword(code, cursor_pos)[0]
  *         # Possibly rewind if we are right after a "("
  *         if not word and cursor_pos > 0 and code[cursor_pos-1] == u"(":             # <<<<<<<<<<<<<<
  *             word = self.__get_keyword(code, cursor_pos-1)[0]
  * 
  */
   }
 
-  /* "PARIKernel/kernel.pyx":202
+  /* "PARIKernel/kernel.pyx":214
  *             word = self.__get_keyword(code, cursor_pos-1)[0]
  * 
  *         reply = dict(status="ok", found=False, data={}, metadata={})             # <<<<<<<<<<<<<<
  *         if not word:
  *             return reply
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 202, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_status, __pyx_n_u_ok) < 0) __PYX_ERR(0, 202, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_found, Py_False) < 0) __PYX_ERR(0, 202, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 202, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_status, __pyx_n_u_ok) < 0) __PYX_ERR(0, 214, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_found, Py_False) < 0) __PYX_ERR(0, 214, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_data, __pyx_t_1) < 0) __PYX_ERR(0, 202, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_data, __pyx_t_1) < 0) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 202, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_metadata, __pyx_t_1) < 0) __PYX_ERR(0, 202, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_metadata, __pyx_t_1) < 0) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_reply = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "PARIKernel/kernel.pyx":203
+  /* "PARIKernel/kernel.pyx":215
  * 
  *         reply = dict(status="ok", found=False, data={}, metadata={})
  *         if not word:             # <<<<<<<<<<<<<<
  *             return reply
  * 
  */
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_v_word); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_v_word); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 215, __pyx_L1_error)
   __pyx_t_8 = ((!__pyx_t_6) != 0);
   if (__pyx_t_8) {
 
-    /* "PARIKernel/kernel.pyx":204
+    /* "PARIKernel/kernel.pyx":216
  *         reply = dict(status="ok", found=False, data={}, metadata={})
  *         if not word:
  *             return reply             # <<<<<<<<<<<<<<
  * 
  *         cdef entree* ep = is_entry((<unicode?>word).encode("utf-8"))
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_reply);
     __pyx_r = __pyx_v_reply;
     goto __pyx_L0;
 
-    /* "PARIKernel/kernel.pyx":203
+    /* "PARIKernel/kernel.pyx":215
  * 
  *         reply = dict(status="ok", found=False, data={}, metadata={})
  *         if not word:             # <<<<<<<<<<<<<<
  *             return reply
  * 
  */
   }
 
-  /* "PARIKernel/kernel.pyx":206
+  /* "PARIKernel/kernel.pyx":218
  *             return reply
  * 
  *         cdef entree* ep = is_entry((<unicode?>word).encode("utf-8"))             # <<<<<<<<<<<<<<
  *         if ep == NULL or ep.help == NULL:
  *             return reply
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_word))||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_word)->tp_name), 0))) __PYX_ERR(0, 206, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_word))||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_word)->tp_name), 0))) __PYX_ERR(0, 218, __pyx_L1_error)
   if (unlikely(__pyx_v_word == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 206, __pyx_L1_error)
+    __PYX_ERR(0, 218, __pyx_L1_error)
   }
-  __pyx_t_2 = PyUnicode_AsUTF8String(((PyObject*)__pyx_v_word)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_t_2 = PyUnicode_AsUTF8String(((PyObject*)__pyx_v_word)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 218, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_10 = __Pyx_PyBytes_AsWritableString(__pyx_t_2); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyBytes_AsWritableString(__pyx_t_2); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 218, __pyx_L1_error)
   __pyx_v_ep = is_entry(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "PARIKernel/kernel.pyx":207
+  /* "PARIKernel/kernel.pyx":219
  * 
  *         cdef entree* ep = is_entry((<unicode?>word).encode("utf-8"))
  *         if ep == NULL or ep.help == NULL:             # <<<<<<<<<<<<<<
  *             return reply
  * 
  */
   __pyx_t_6 = ((__pyx_v_ep == NULL) != 0);
@@ -3953,73 +4029,73 @@
     goto __pyx_L9_bool_binop_done;
   }
   __pyx_t_6 = ((__pyx_v_ep->help == NULL) != 0);
   __pyx_t_8 = __pyx_t_6;
   __pyx_L9_bool_binop_done:;
   if (__pyx_t_8) {
 
-    /* "PARIKernel/kernel.pyx":208
+    /* "PARIKernel/kernel.pyx":220
  *         cdef entree* ep = is_entry((<unicode?>word).encode("utf-8"))
  *         if ep == NULL or ep.help == NULL:
  *             return reply             # <<<<<<<<<<<<<<
  * 
  *         reply["found"] = True
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_reply);
     __pyx_r = __pyx_v_reply;
     goto __pyx_L0;
 
-    /* "PARIKernel/kernel.pyx":207
+    /* "PARIKernel/kernel.pyx":219
  * 
  *         cdef entree* ep = is_entry((<unicode?>word).encode("utf-8"))
  *         if ep == NULL or ep.help == NULL:             # <<<<<<<<<<<<<<
  *             return reply
  * 
  */
   }
 
-  /* "PARIKernel/kernel.pyx":210
+  /* "PARIKernel/kernel.pyx":222
  *             return reply
  * 
  *         reply["found"] = True             # <<<<<<<<<<<<<<
  *         reply["data"] = {"text/plain": PyUnicode_FromString(ep.help)}
  *         return reply
  */
-  if (unlikely(PyDict_SetItem(__pyx_v_reply, __pyx_n_u_found, Py_True) < 0)) __PYX_ERR(0, 210, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_reply, __pyx_n_u_found, Py_True) < 0)) __PYX_ERR(0, 222, __pyx_L1_error)
 
-  /* "PARIKernel/kernel.pyx":211
+  /* "PARIKernel/kernel.pyx":223
  * 
  *         reply["found"] = True
  *         reply["data"] = {"text/plain": PyUnicode_FromString(ep.help)}             # <<<<<<<<<<<<<<
  *         return reply
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyUnicode_FromString(__pyx_v_ep->help); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_FromString(__pyx_v_ep->help); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_text_plain, __pyx_t_1) < 0) __PYX_ERR(0, 211, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_text_plain, __pyx_t_1) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(PyDict_SetItem(__pyx_v_reply, __pyx_n_u_data, __pyx_t_2) < 0)) __PYX_ERR(0, 211, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_reply, __pyx_n_u_data, __pyx_t_2) < 0)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "PARIKernel/kernel.pyx":212
+  /* "PARIKernel/kernel.pyx":224
  *         reply["found"] = True
  *         reply["data"] = {"text/plain": PyUnicode_FromString(ep.help)}
  *         return reply             # <<<<<<<<<<<<<<
  * 
- *     def publish_svg(self, svg, width, height):
+ *     def publish_svg(self, bytes svg, width, height):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_reply);
   __pyx_r = __pyx_v_reply;
   goto __pyx_L0;
 
-  /* "PARIKernel/kernel.pyx":196
+  /* "PARIKernel/kernel.pyx":208
  *         return reply
  * 
  *     def do_inspect(self, code, cursor_pos, detail_level=0):             # <<<<<<<<<<<<<<
  *         word = self.__get_keyword(code, cursor_pos)[0]
  *         # Possibly rewind if we are right after a "("
  */
 
@@ -4036,20 +4112,20 @@
   __Pyx_XDECREF(__pyx_v_word);
   __Pyx_XDECREF(__pyx_v_reply);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "PARIKernel/kernel.pyx":214
+/* "PARIKernel/kernel.pyx":226
  *         return reply
  * 
- *     def publish_svg(self, svg, width, height):             # <<<<<<<<<<<<<<
- *         # For some reason, the payload must be str, not bytes
- *         if not isinstance(svg, str):
+ *     def publish_svg(self, bytes svg, width, height):             # <<<<<<<<<<<<<<
+ *         content = {
+ *             'data': {
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10PARIKernel_6kernel_10PARIKernel_9publish_svg(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_10PARIKernel_6kernel_10PARIKernel_9publish_svg = {"publish_svg", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10PARIKernel_6kernel_10PARIKernel_9publish_svg, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_10PARIKernel_6kernel_10PARIKernel_9publish_svg(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
@@ -4085,259 +4161,247 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_svg)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("publish_svg", 1, 4, 4, 1); __PYX_ERR(0, 214, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("publish_svg", 1, 4, 4, 1); __PYX_ERR(0, 226, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_width)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("publish_svg", 1, 4, 4, 2); __PYX_ERR(0, 214, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("publish_svg", 1, 4, 4, 2); __PYX_ERR(0, 226, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_height)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("publish_svg", 1, 4, 4, 3); __PYX_ERR(0, 214, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("publish_svg", 1, 4, 4, 3); __PYX_ERR(0, 226, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "publish_svg") < 0)) __PYX_ERR(0, 214, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "publish_svg") < 0)) __PYX_ERR(0, 226, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
     __pyx_v_self = values[0];
-    __pyx_v_svg = values[1];
+    __pyx_v_svg = ((PyObject*)values[1]);
     __pyx_v_width = values[2];
     __pyx_v_height = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("publish_svg", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 214, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("publish_svg", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 226, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("PARIKernel.kernel.PARIKernel.publish_svg", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_svg), (&PyBytes_Type), 1, "svg", 1))) __PYX_ERR(0, 226, __pyx_L1_error)
   __pyx_r = __pyx_pf_10PARIKernel_6kernel_10PARIKernel_8publish_svg(__pyx_self, __pyx_v_self, __pyx_v_svg, __pyx_v_width, __pyx_v_height);
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_10PARIKernel_6kernel_10PARIKernel_8publish_svg(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_svg, PyObject *__pyx_v_width, PyObject *__pyx_v_height) {
   PyObject *__pyx_v_content = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  int __pyx_t_2;
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
   char const *__pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
-  PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("publish_svg", 0);
-  __Pyx_INCREF(__pyx_v_svg);
 
-  /* "PARIKernel/kernel.pyx":216
- *     def publish_svg(self, svg, width, height):
- *         # For some reason, the payload must be str, not bytes
- *         if not isinstance(svg, str):             # <<<<<<<<<<<<<<
- *             svg = PyUnicode_FromString(svg)
- *         content = {
- */
-  __pyx_t_1 = PyUnicode_Check(__pyx_v_svg); 
-  __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
-  if (__pyx_t_2) {
-
-    /* "PARIKernel/kernel.pyx":217
- *         # For some reason, the payload must be str, not bytes
- *         if not isinstance(svg, str):
- *             svg = PyUnicode_FromString(svg)             # <<<<<<<<<<<<<<
- *         content = {
- *             'data': {
- */
-    __pyx_t_3 = __Pyx_PyObject_AsString(__pyx_v_svg); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 217, __pyx_L1_error)
-    __pyx_t_4 = PyUnicode_FromString(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 217, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF_SET(__pyx_v_svg, __pyx_t_4);
-    __pyx_t_4 = 0;
-
-    /* "PARIKernel/kernel.pyx":216
- *     def publish_svg(self, svg, width, height):
- *         # For some reason, the payload must be str, not bytes
- *         if not isinstance(svg, str):             # <<<<<<<<<<<<<<
- *             svg = PyUnicode_FromString(svg)
- *         content = {
- */
-  }
-
-  /* "PARIKernel/kernel.pyx":219
- *             svg = PyUnicode_FromString(svg)
+  /* "PARIKernel/kernel.pyx":228
+ *     def publish_svg(self, bytes svg, width, height):
  *         content = {
  *             'data': {             # <<<<<<<<<<<<<<
  *                 "text/plain": "SVG plot",
- *                 "image/svg+xml": svg,
+ *                 "image/svg+xml": PyUnicode_FromString(svg),
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 219, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
 
-  /* "PARIKernel/kernel.pyx":220
+  /* "PARIKernel/kernel.pyx":229
  *         content = {
  *             'data': {
  *                 "text/plain": "SVG plot",             # <<<<<<<<<<<<<<
- *                 "image/svg+xml": svg,
+ *                 "image/svg+xml": PyUnicode_FromString(svg),
  *             },
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 220, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_kp_u_text_plain, __pyx_kp_u_SVG_plot) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_text_plain, __pyx_kp_u_SVG_plot) < 0) __PYX_ERR(0, 229, __pyx_L1_error)
 
-  /* "PARIKernel/kernel.pyx":221
+  /* "PARIKernel/kernel.pyx":230
  *             'data': {
  *                 "text/plain": "SVG plot",
- *                 "image/svg+xml": svg,             # <<<<<<<<<<<<<<
+ *                 "image/svg+xml": PyUnicode_FromString(svg),             # <<<<<<<<<<<<<<
  *             },
  *             'metadata': {
  */
-  if (PyDict_SetItem(__pyx_t_5, __pyx_kp_u_image_svg_xml, __pyx_v_svg) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_data, __pyx_t_5) < 0) __PYX_ERR(0, 219, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(__pyx_v_svg == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
+    __PYX_ERR(0, 230, __pyx_L1_error)
+  }
+  __pyx_t_3 = __Pyx_PyBytes_AsString(__pyx_v_svg); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 230, __pyx_L1_error)
+  __pyx_t_4 = PyUnicode_FromString(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 230, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_image_svg_xml, __pyx_t_4) < 0) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_data, __pyx_t_2) < 0) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "PARIKernel/kernel.pyx":224
+  /* "PARIKernel/kernel.pyx":233
  *             },
  *             'metadata': {
- *                 "width": width,             # <<<<<<<<<<<<<<
- *                 "height": height,
- *             }
+ *                 "image/svg+xml": {             # <<<<<<<<<<<<<<
+ *                     "width": width,
+ *                     "height": height
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 224, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_width, __pyx_v_width) < 0) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
 
-  /* "PARIKernel/kernel.pyx":225
+  /* "PARIKernel/kernel.pyx":234
  *             'metadata': {
- *                 "width": width,
- *                 "height": height,             # <<<<<<<<<<<<<<
+ *                 "image/svg+xml": {
+ *                     "width": width,             # <<<<<<<<<<<<<<
+ *                     "height": height
+ *                 }
+ */
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_width, __pyx_v_width) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
+
+  /* "PARIKernel/kernel.pyx":235
+ *                 "image/svg+xml": {
+ *                     "width": width,
+ *                     "height": height             # <<<<<<<<<<<<<<
+ *                 }
  *             }
- *         }
  */
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_height, __pyx_v_height) < 0) __PYX_ERR(0, 224, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_metadata, __pyx_t_5) < 0) __PYX_ERR(0, 219, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_v_content = ((PyObject*)__pyx_t_4);
-  __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_height, __pyx_v_height) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_image_svg_xml, __pyx_t_4) < 0) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_metadata, __pyx_t_2) < 0) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v_content = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
 
-  /* "PARIKernel/kernel.pyx":228
+  /* "PARIKernel/kernel.pyx":239
  *             }
  *         }
  *         self.send_response(self.iopub_socket, 'display_data', content)             # <<<<<<<<<<<<<<
  * 
  *     def __get_keyword(self, code, pos):
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_send_response); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 228, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_iopub_socket); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 228, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = NULL;
-  __pyx_t_8 = 0;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_7)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_7);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_send_response); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_iopub_socket); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = NULL;
+  __pyx_t_6 = 0;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
-      __pyx_t_8 = 1;
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_5)) {
-    PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_6, __pyx_n_u_display_data, __pyx_v_content};
-    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 228, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyFunction_Check(__pyx_t_2)) {
+    PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_t_4, __pyx_n_u_display_data, __pyx_v_content};
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
-    PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_6, __pyx_n_u_display_data, __pyx_v_content};
-    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 228, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
+    PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_t_4, __pyx_n_u_display_data, __pyx_v_content};
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
-    __pyx_t_9 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 228, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    if (__pyx_t_7) {
-      __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
+    __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 239, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    if (__pyx_t_5) {
+      __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_t_4);
     __Pyx_INCREF(__pyx_n_u_display_data);
     __Pyx_GIVEREF(__pyx_n_u_display_data);
-    PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_n_u_display_data);
+    PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_n_u_display_data);
     __Pyx_INCREF(__pyx_v_content);
     __Pyx_GIVEREF(__pyx_v_content);
-    PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_8, __pyx_v_content);
-    __pyx_t_6 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 228, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_6, __pyx_v_content);
+    __pyx_t_4 = 0;
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "PARIKernel/kernel.pyx":214
+  /* "PARIKernel/kernel.pyx":226
  *         return reply
  * 
- *     def publish_svg(self, svg, width, height):             # <<<<<<<<<<<<<<
- *         # For some reason, the payload must be str, not bytes
- *         if not isinstance(svg, str):
+ *     def publish_svg(self, bytes svg, width, height):             # <<<<<<<<<<<<<<
+ *         content = {
+ *             'data': {
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("PARIKernel.kernel.PARIKernel.publish_svg", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_content);
-  __Pyx_XDECREF(__pyx_v_svg);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "PARIKernel/kernel.pyx":230
+/* "PARIKernel/kernel.pyx":241
  *         self.send_response(self.iopub_socket, 'display_data', content)
  * 
  *     def __get_keyword(self, code, pos):             # <<<<<<<<<<<<<<
  *         """
  *         Return a tuple ``(word, start, end)`` such that ``word`` is a
  */
 
@@ -4376,40 +4440,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_code)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__get_keyword", 1, 3, 3, 1); __PYX_ERR(0, 230, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__get_keyword", 1, 3, 3, 1); __PYX_ERR(0, 241, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pos)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__get_keyword", 1, 3, 3, 2); __PYX_ERR(0, 230, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__get_keyword", 1, 3, 3, 2); __PYX_ERR(0, 241, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__get_keyword") < 0)) __PYX_ERR(0, 230, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__get_keyword") < 0)) __PYX_ERR(0, 241, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_code = values[1];
     __pyx_v_pos = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__get_keyword", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 230, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__get_keyword", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 241, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("PARIKernel.kernel.PARIKernel.__get_keyword", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10PARIKernel_6kernel_10PARIKernel_10__get_keyword(__pyx_self, __pyx_v_self, __pyx_v_code, __pyx_v_pos);
 
@@ -4433,139 +4497,139 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get_keyword", 0);
 
-  /* "PARIKernel/kernel.pyx":236
+  /* "PARIKernel/kernel.pyx":247
  *         such that ``start <= pos <= end``.
  *         """
  *         cdef Py_ssize_t start, end, length = len(code)             # <<<<<<<<<<<<<<
  *         start = end = pos
  *         while start > 0 and is_keyword_char_python(code[start-1]):
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_code); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_code); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 247, __pyx_L1_error)
   __pyx_v_length = __pyx_t_1;
 
-  /* "PARIKernel/kernel.pyx":237
+  /* "PARIKernel/kernel.pyx":248
  *         """
  *         cdef Py_ssize_t start, end, length = len(code)
  *         start = end = pos             # <<<<<<<<<<<<<<
  *         while start > 0 and is_keyword_char_python(code[start-1]):
  *             start -= 1
  */
-  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_pos); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 237, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_pos); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 248, __pyx_L1_error)
   __pyx_v_start = __pyx_t_1;
   __pyx_v_end = __pyx_t_1;
 
-  /* "PARIKernel/kernel.pyx":238
+  /* "PARIKernel/kernel.pyx":249
  *         cdef Py_ssize_t start, end, length = len(code)
  *         start = end = pos
  *         while start > 0 and is_keyword_char_python(code[start-1]):             # <<<<<<<<<<<<<<
  *             start -= 1
  *         while end < length and is_keyword_char_python(code[end]):
  */
   while (1) {
     __pyx_t_3 = ((__pyx_v_start > 0) != 0);
     if (__pyx_t_3) {
     } else {
       __pyx_t_2 = __pyx_t_3;
       goto __pyx_L5_bool_binop_done;
     }
     __pyx_t_1 = (__pyx_v_start - 1);
-    __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_code, __pyx_t_1, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 238, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_code, __pyx_t_1, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 249, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __pyx_f_10PARIKernel_6kernel_is_keyword_char_python(__pyx_t_4); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 238, __pyx_L1_error)
+    __pyx_t_3 = __pyx_f_10PARIKernel_6kernel_is_keyword_char_python(__pyx_t_4); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 249, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_5 = (__pyx_t_3 != 0);
     __pyx_t_2 = __pyx_t_5;
     __pyx_L5_bool_binop_done:;
     if (!__pyx_t_2) break;
 
-    /* "PARIKernel/kernel.pyx":239
+    /* "PARIKernel/kernel.pyx":250
  *         start = end = pos
  *         while start > 0 and is_keyword_char_python(code[start-1]):
  *             start -= 1             # <<<<<<<<<<<<<<
  *         while end < length and is_keyword_char_python(code[end]):
  *             end += 1
  */
     __pyx_v_start = (__pyx_v_start - 1);
   }
 
-  /* "PARIKernel/kernel.pyx":240
+  /* "PARIKernel/kernel.pyx":251
  *         while start > 0 and is_keyword_char_python(code[start-1]):
  *             start -= 1
  *         while end < length and is_keyword_char_python(code[end]):             # <<<<<<<<<<<<<<
  *             end += 1
  *         word = code[start:end]
  */
   while (1) {
     __pyx_t_5 = ((__pyx_v_end < __pyx_v_length) != 0);
     if (__pyx_t_5) {
     } else {
       __pyx_t_2 = __pyx_t_5;
       goto __pyx_L9_bool_binop_done;
     }
-    __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_code, __pyx_v_end, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 240, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_code, __pyx_v_end, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 251, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __pyx_f_10PARIKernel_6kernel_is_keyword_char_python(__pyx_t_4); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 240, __pyx_L1_error)
+    __pyx_t_5 = __pyx_f_10PARIKernel_6kernel_is_keyword_char_python(__pyx_t_4); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 251, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_3 = (__pyx_t_5 != 0);
     __pyx_t_2 = __pyx_t_3;
     __pyx_L9_bool_binop_done:;
     if (!__pyx_t_2) break;
 
-    /* "PARIKernel/kernel.pyx":241
+    /* "PARIKernel/kernel.pyx":252
  *             start -= 1
  *         while end < length and is_keyword_char_python(code[end]):
  *             end += 1             # <<<<<<<<<<<<<<
  *         word = code[start:end]
  *         return (word, start, end)
  */
     __pyx_v_end = (__pyx_v_end + 1);
   }
 
-  /* "PARIKernel/kernel.pyx":242
+  /* "PARIKernel/kernel.pyx":253
  *         while end < length and is_keyword_char_python(code[end]):
  *             end += 1
  *         word = code[start:end]             # <<<<<<<<<<<<<<
  *         return (word, start, end)
  */
-  __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_v_code, __pyx_v_start, __pyx_v_end, NULL, NULL, NULL, 1, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_v_code, __pyx_v_start, __pyx_v_end, NULL, NULL, NULL, 1, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_v_word = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "PARIKernel/kernel.pyx":243
+  /* "PARIKernel/kernel.pyx":254
  *             end += 1
  *         word = code[start:end]
  *         return (word, start, end)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_end); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_end); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(__pyx_v_word);
   __Pyx_GIVEREF(__pyx_v_word);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_word);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_t_6);
   __pyx_t_4 = 0;
   __pyx_t_6 = 0;
   __pyx_r = __pyx_t_7;
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
-  /* "PARIKernel/kernel.pyx":230
+  /* "PARIKernel/kernel.pyx":241
  *         self.send_response(self.iopub_socket, 'display_data', content)
  * 
  *     def __get_keyword(self, code, pos):             # <<<<<<<<<<<<<<
  *         """
  *         Return a tuple ``(word, start, end)`` such that ``word`` is a
  */
 
@@ -4745,14 +4809,15 @@
   {&__pyx_n_u_traceback, __pyx_k_traceback, sizeof(__pyx_k_traceback), 0, 1, 0, 1},
   {&__pyx_n_s_user_expressions, __pyx_k_user_expressions, sizeof(__pyx_k_user_expressions), 0, 0, 1, 1},
   {&__pyx_n_u_user_expressions, __pyx_k_user_expressions, sizeof(__pyx_k_user_expressions), 0, 1, 0, 1},
   {&__pyx_n_s_version, __pyx_k_version, sizeof(__pyx_k_version), 0, 0, 1, 1},
   {&__pyx_n_s_width, __pyx_k_width, sizeof(__pyx_k_width), 0, 0, 1, 1},
   {&__pyx_n_u_width, __pyx_k_width, sizeof(__pyx_k_width), 0, 1, 0, 1},
   {&__pyx_n_s_word, __pyx_k_word, sizeof(__pyx_k_word), 0, 0, 1, 1},
+  {&__pyx_n_s_wt_ms, __pyx_k_wt_ms, sizeof(__pyx_k_wt_ms), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(0, 50, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 87, __pyx_L1_error)
   __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 101, __pyx_L1_error)
   return 0;
@@ -4803,72 +4868,72 @@
   /* "PARIKernel/kernel.pyx":110
  *         init_svg(self)
  * 
  *     def do_execute(self, code, silent, store_history=True, user_expressions=None,             # <<<<<<<<<<<<<<
  *                    allow_stdin=False):
  *         global avma
  */
-  __pyx_tuple__10 = PyTuple_Pack(16, __pyx_n_s_self, __pyx_n_s_code, __pyx_n_s_silent, __pyx_n_s_store_history, __pyx_n_s_user_expressions, __pyx_n_s_allow_stdin, __pyx_n_s_av, __pyx_n_s_result, __pyx_n_s_gp_code, __pyx_n_s_sa, __pyx_n_s_old_sa, __pyx_n_s_err, __pyx_n_s_t_ms, __pyx_n_s_last, __pyx_n_s_content, __pyx_n_s_reply); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(17, __pyx_n_s_self, __pyx_n_s_code, __pyx_n_s_silent, __pyx_n_s_store_history, __pyx_n_s_user_expressions, __pyx_n_s_allow_stdin, __pyx_n_s_av, __pyx_n_s_result, __pyx_n_s_gp_code, __pyx_n_s_sa, __pyx_n_s_old_sa, __pyx_n_s_err, __pyx_n_s_t_ms, __pyx_n_s_wt_ms, __pyx_n_s_last, __pyx_n_s_content, __pyx_n_s_reply); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(6, 0, 16, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_PARIKernel_kernel_pyx, __pyx_n_s_do_execute, 110, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(6, 0, 17, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_PARIKernel_kernel_pyx, __pyx_n_s_do_execute, 110, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 110, __pyx_L1_error)
   __pyx_tuple__12 = PyTuple_Pack(3, ((PyObject *)Py_True), ((PyObject *)Py_None), ((PyObject *)Py_False)); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "PARIKernel/kernel.pyx":178
+  /* "PARIKernel/kernel.pyx":190
  *         return reply
  * 
  *     def do_complete(self, code, cursor_pos):             # <<<<<<<<<<<<<<
  *         cdef long word
  *         cdef char** m = pari_completion_matches(&pari_rl,
  */
-  __pyx_tuple__13 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_code, __pyx_n_s_cursor_pos, __pyx_n_s_word, __pyx_n_s_m, __pyx_n_s_matches, __pyx_n_s_reply); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_code, __pyx_n_s_cursor_pos, __pyx_n_s_word, __pyx_n_s_m, __pyx_n_s_matches, __pyx_n_s_reply); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(3, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_PARIKernel_kernel_pyx, __pyx_n_s_do_complete, 178, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(3, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_PARIKernel_kernel_pyx, __pyx_n_s_do_complete, 190, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 190, __pyx_L1_error)
 
-  /* "PARIKernel/kernel.pyx":196
+  /* "PARIKernel/kernel.pyx":208
  *         return reply
  * 
  *     def do_inspect(self, code, cursor_pos, detail_level=0):             # <<<<<<<<<<<<<<
  *         word = self.__get_keyword(code, cursor_pos)[0]
  *         # Possibly rewind if we are right after a "("
  */
-  __pyx_tuple__15 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_code, __pyx_n_s_cursor_pos, __pyx_n_s_detail_level, __pyx_n_s_word, __pyx_n_s_reply, __pyx_n_s_ep); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_code, __pyx_n_s_cursor_pos, __pyx_n_s_detail_level, __pyx_n_s_word, __pyx_n_s_reply, __pyx_n_s_ep); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 208, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(4, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_PARIKernel_kernel_pyx, __pyx_n_s_do_inspect, 196, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 196, __pyx_L1_error)
-  __pyx_tuple__17 = PyTuple_Pack(1, ((PyObject *)__pyx_int_0)); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(4, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_PARIKernel_kernel_pyx, __pyx_n_s_do_inspect, 208, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 208, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, ((PyObject *)__pyx_int_0)); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 208, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
-  /* "PARIKernel/kernel.pyx":214
+  /* "PARIKernel/kernel.pyx":226
  *         return reply
  * 
- *     def publish_svg(self, svg, width, height):             # <<<<<<<<<<<<<<
- *         # For some reason, the payload must be str, not bytes
- *         if not isinstance(svg, str):
+ *     def publish_svg(self, bytes svg, width, height):             # <<<<<<<<<<<<<<
+ *         content = {
+ *             'data': {
  */
-  __pyx_tuple__18 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_svg, __pyx_n_s_width, __pyx_n_s_height, __pyx_n_s_content); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 214, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_svg, __pyx_n_s_width, __pyx_n_s_height, __pyx_n_s_content); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(4, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_PARIKernel_kernel_pyx, __pyx_n_s_publish_svg, 214, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 214, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(4, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_PARIKernel_kernel_pyx, __pyx_n_s_publish_svg, 226, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 226, __pyx_L1_error)
 
-  /* "PARIKernel/kernel.pyx":230
+  /* "PARIKernel/kernel.pyx":241
  *         self.send_response(self.iopub_socket, 'display_data', content)
  * 
  *     def __get_keyword(self, code, pos):             # <<<<<<<<<<<<<<
  *         """
  *         Return a tuple ``(word, start, end)`` such that ``word`` is a
  */
-  __pyx_tuple__20 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_code, __pyx_n_s_pos, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_length, __pyx_n_s_word); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 230, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_code, __pyx_n_s_pos, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_length, __pyx_n_s_word); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_PARIKernel_kernel_pyx, __pyx_n_s_get_keyword, 230, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 230, __pyx_L1_error)
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_PARIKernel_kernel_pyx, __pyx_n_s_get_keyword, 241, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -5449,61 +5514,61 @@
  */
   __pyx_t_10 = __Pyx_CyFunction_New(&__pyx_mdef_10PARIKernel_6kernel_10PARIKernel_3do_execute, 0, __pyx_n_s_PARIKernel_do_execute, NULL, __pyx_n_s_PARIKernel_kernel, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_10, __pyx_tuple__12);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_do_execute, __pyx_t_10) < 0) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "PARIKernel/kernel.pyx":178
+  /* "PARIKernel/kernel.pyx":190
  *         return reply
  * 
  *     def do_complete(self, code, cursor_pos):             # <<<<<<<<<<<<<<
  *         cdef long word
  *         cdef char** m = pari_completion_matches(&pari_rl,
  */
-  __pyx_t_10 = __Pyx_CyFunction_New(&__pyx_mdef_10PARIKernel_6kernel_10PARIKernel_5do_complete, 0, __pyx_n_s_PARIKernel_do_complete, NULL, __pyx_n_s_PARIKernel_kernel, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_CyFunction_New(&__pyx_mdef_10PARIKernel_6kernel_10PARIKernel_5do_complete, 0, __pyx_n_s_PARIKernel_do_complete, NULL, __pyx_n_s_PARIKernel_kernel, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_do_complete, __pyx_t_10) < 0) __PYX_ERR(0, 178, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_do_complete, __pyx_t_10) < 0) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "PARIKernel/kernel.pyx":196
+  /* "PARIKernel/kernel.pyx":208
  *         return reply
  * 
  *     def do_inspect(self, code, cursor_pos, detail_level=0):             # <<<<<<<<<<<<<<
  *         word = self.__get_keyword(code, cursor_pos)[0]
  *         # Possibly rewind if we are right after a "("
  */
-  __pyx_t_10 = __Pyx_CyFunction_New(&__pyx_mdef_10PARIKernel_6kernel_10PARIKernel_7do_inspect, 0, __pyx_n_s_PARIKernel_do_inspect, NULL, __pyx_n_s_PARIKernel_kernel, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_CyFunction_New(&__pyx_mdef_10PARIKernel_6kernel_10PARIKernel_7do_inspect, 0, __pyx_n_s_PARIKernel_do_inspect, NULL, __pyx_n_s_PARIKernel_kernel, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 208, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_10, __pyx_tuple__17);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_do_inspect, __pyx_t_10) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_do_inspect, __pyx_t_10) < 0) __PYX_ERR(0, 208, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "PARIKernel/kernel.pyx":214
+  /* "PARIKernel/kernel.pyx":226
  *         return reply
  * 
- *     def publish_svg(self, svg, width, height):             # <<<<<<<<<<<<<<
- *         # For some reason, the payload must be str, not bytes
- *         if not isinstance(svg, str):
+ *     def publish_svg(self, bytes svg, width, height):             # <<<<<<<<<<<<<<
+ *         content = {
+ *             'data': {
  */
-  __pyx_t_10 = __Pyx_CyFunction_New(&__pyx_mdef_10PARIKernel_6kernel_10PARIKernel_9publish_svg, 0, __pyx_n_s_PARIKernel_publish_svg, NULL, __pyx_n_s_PARIKernel_kernel, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 214, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_CyFunction_New(&__pyx_mdef_10PARIKernel_6kernel_10PARIKernel_9publish_svg, 0, __pyx_n_s_PARIKernel_publish_svg, NULL, __pyx_n_s_PARIKernel_kernel, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_publish_svg, __pyx_t_10) < 0) __PYX_ERR(0, 214, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_publish_svg, __pyx_t_10) < 0) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "PARIKernel/kernel.pyx":230
+  /* "PARIKernel/kernel.pyx":241
  *         self.send_response(self.iopub_socket, 'display_data', content)
  * 
  *     def __get_keyword(self, code, pos):             # <<<<<<<<<<<<<<
  *         """
  *         Return a tuple ``(word, start, end)`` such that ``word`` is a
  */
-  __pyx_t_10 = __Pyx_CyFunction_New(&__pyx_mdef_10PARIKernel_6kernel_10PARIKernel_11__get_keyword, 0, __pyx_n_s_PARIKernel___get_keyword, NULL, __pyx_n_s_PARIKernel_kernel, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 230, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_CyFunction_New(&__pyx_mdef_10PARIKernel_6kernel_10PARIKernel_11__get_keyword, 0, __pyx_n_s_PARIKernel___get_keyword, NULL, __pyx_n_s_PARIKernel_kernel, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_PARIKernel__get_keyword, __pyx_t_10) < 0) __PYX_ERR(0, 230, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_PARIKernel__get_keyword, __pyx_t_10) < 0) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
   /* "PARIKernel/kernel.pyx":92
  * 
  * 
  * class PARIKernel(Kernel):             # <<<<<<<<<<<<<<
  *     implementation = 'PARI'
@@ -6695,14 +6760,35 @@
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(owned_ref);
     #endif
     return (equals == Py_NE);
 #endif
 }
 
+/* ArgTypeTest */
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
+{
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
+    }
+    else if (exact) {
+        #if PY_MAJOR_VERSION == 2
+        if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
+        #endif
+    }
+    else {
+        if (likely(__Pyx_TypeCheck(obj, type))) return 1;
+    }
+    PyErr_Format(PyExc_TypeError,
+        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
+        name, type->tp_name, Py_TYPE(obj)->tp_name);
+    return 0;
+}
+
 /* SliceObject */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetSlice(PyObject* obj,
         Py_ssize_t cstart, Py_ssize_t cstop,
         PyObject** _py_start, PyObject** _py_stop, PyObject** _py_slice,
         int has_cstart, int has_cstop, CYTHON_UNUSED int wraparound) {
 #if CYTHON_USE_TYPE_SLOTS
     PyMappingMethods* mp;
@@ -7575,21 +7661,21 @@
     0,
     0,
     0,
     0,
 #if PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b1
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
```

### Comparing `pari-jupyter-1.4.1/PARIKernel/kernel.pyx` & `pari-jupyter-1.4.2/PARIKernel/kernel.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 DEF PRIMELIMIT = 500000
 
 
 # Global setjmp() context for error handling
 cdef sigjmp_buf context
 
 cdef void pari_recover(long numerr) nogil:
-    siglongjmp(context, -1)
+    siglongjmp(context, numerr)
 
 # Global PARI readline interface
 cdef pari_rl_interface pari_rl
 
 # Support for SVG plotting (if compiled in)
 try:
     from .svg import init_svg
@@ -120,37 +120,40 @@
 
         cdef sigaction_t sa
         cdef sigaction_t old_sa
         memset(&sa, 0, sizeof(sa))
         sa.sa_handler = pari_sighandler
 
         cdef int err
-        cdef long t_ms
+        cdef long t_ms, wt_ms
         cdef char last
+
         with nogil:
             err = sigsetjmp(context, 1)
             if err == 0:  # Initial sigsetjmp() call
                 sigaction(SIGINT, &sa, &old_sa)  # Handle SIGINT by PARI
                 timer_start(GP_DATA.T)
+                walltimer_start(GP_DATA.Tw)
                 result = gp_read_str_multiline(gp_code, &last)
                 t_ms = timer_delay(GP_DATA.T)
+                wt_ms = walltimer_delay(GP_DATA.Tw)
             sigaction(SIGINT, &old_sa, &sa)      # Restore Python SIGINT handler
 
-        if not err:  # success
+        if err == 0:  # success
             if not silent:
                 if t_ms and GP_DATA.chrono:
                     pari_puts(b"time = ")
                     pari_puts(gp_format_time(t_ms))
                     pari_flush()
 
             # gnil as a result is like Python's None, it should be
             # considered as "no result"
             if result is not gnil:
                 if store_history:
-                    pari_add_hist(result, t_ms, t_ms)
+                    pari_add_hist(result, t_ms, wt_ms)
 
                 if last != c';' and not silent:
                     content = {
                         'execution_count': pari_nb_hist(),
                         'data': {
                             'text/plain': PyUnicode_FromGEN(result),
                         },
@@ -159,23 +162,32 @@
                     self.send_response(self.iopub_socket, 'execute_result', content)
 
             reply = {'status': 'ok',
                      'execution_count': pari_nb_hist(),
                      'payload': [],
                      'user_expressions': {},
                     }
+
+            avma = av
+
         else:  # error (therefore no result)
             reply = {'status': 'error',
                      'execution_count': pari_nb_hist(),
                      'ename': "",
                      'evalue': "",
                      'traceback': [],
                     }
 
-        avma = av
+            if err > 0:
+                # true error
+                avma = av
+            else:
+                # allocatemem
+                avma = pari_mainstack.top
+
         self.io.flush()
         return reply
 
     def do_complete(self, code, cursor_pos):
         cdef long word
         cdef char** m = pari_completion_matches(&pari_rl,
                 (<unicode?>code).encode("utf-8"), cursor_pos, &word)
```

### Comparing `pari-jupyter-1.4.1/PARIKernel/paridecl.pxd` & `pari-jupyter-1.4.2/PARIKernel/paridecl.pxd`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,19 @@
         entree* next
         char* name
         const char* help
 
     long    paricfg_version_code
     long    PARI_VERSION_SHIFT
 
+    ctypedef struct pari_mainstack:
+        pari_sp top
+
     pari_sp avma
+    pari_mainstack * pari_mainstack
     GEN     gnil
 
     int     INIT_JMPm, INIT_SIGm, INIT_DFTm, INIT_noPRIMEm, INIT_noIMTm
     void    pari_init_opts(size_t parisize, ulong maxprime, ulong init_opts)
     void    pari_init(size_t parisize, ulong maxprime)
     void    pari_sighandler(int sig)
 
@@ -28,14 +32,18 @@
     char*   GENtostr(GEN x)
     void    pari_add_hist(GEN z, long t, long r)
     long    pari_nb_hist()
 
     long    timer_delay(pari_timer *T)
     long    timer_get(pari_timer *T)
     void    timer_start(pari_timer *T)
+
+    long    walltimer_start(pari_timer *T)
+    long    walltimer_delay(pari_timer *T)
+
     char*   gp_format_time(long delay)
 
     void    pari_puts(char*)
     void    pari_flush()
 
     struct PariOUT:
         void (*putch)(char)
@@ -62,14 +70,15 @@
 
 cdef extern from "pari/paripriv.h" nogil:
     long    is_keyword_char(char c)
 
     ctypedef struct gp_data:
         int chrono
         pari_timer* T
+        pari_timer* Tw
 
     gp_data* GP_DATA
 
     ctypedef struct pari_rl_interface:
         pass
 
     void    pari_use_readline(pari_rl_interface)
```

### Comparing `pari-jupyter-1.4.1/PARIKernel/svg.c` & `pari-jupyter-1.4.2/PARIKernel/svg.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.26 */
+/* Generated by Cython 0.29.28 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_26"
-#define CYTHON_HEX_VERSION 0x001D1AF0
+#define CYTHON_ABI "0_29_28"
+#define CYTHON_HEX_VERSION 0x001D1CF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -168,30 +168,36 @@
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
     #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
```

### Comparing `pari-jupyter-1.4.1/PARIKernel/svg.pyx` & `pari-jupyter-1.4.2/PARIKernel/svg.pyx`

 * *Files identical despite different names*

### Comparing `pari-jupyter-1.4.1/PKG-INFO` & `pari-jupyter-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pari-jupyter
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Jupyter kernel for PARI/GP
 Home-page: https://github.com/sagemath/pari-jupyter
 Author: Jeroen Demeyer
 Author-email: pari-users@pari.math.u-bordeaux.fr
 License: GNU General Public License (GPL) version 3 or later
 Platform: POSIX
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pari-jupyter-1.4.1/README.rst` & `pari-jupyter-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `pari-jupyter-1.4.1/gp-mode/gp.js` & `pari-jupyter-1.4.2/gp-mode/gp.js`

 * *Files identical despite different names*

### Comparing `pari-jupyter-1.4.1/pari_jupyter.egg-info/PKG-INFO` & `pari-jupyter-1.4.2/pari_jupyter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pari-jupyter
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Jupyter kernel for PARI/GP
 Home-page: https://github.com/sagemath/pari-jupyter
 Author: Jeroen Demeyer
 Author-email: pari-users@pari.math.u-bordeaux.fr
 License: GNU General Public License (GPL) version 3 or later
 Platform: POSIX
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pari-jupyter-1.4.1/pari_jupyter.egg-info/SOURCES.txt` & `pari-jupyter-1.4.2/pari_jupyter.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
 gp-mode.json
-pyproject.toml
 setup.py
 PARIKernel/__init__.py
 PARIKernel/__main__.py
 PARIKernel/io.c
 PARIKernel/io.pxd
 PARIKernel/io.pyx
 PARIKernel/kernel.c
```

### Comparing `pari-jupyter-1.4.1/setup.py` & `pari-jupyter-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `pari-jupyter-1.4.1/spec/kernel.js` & `pari-jupyter-1.4.2/spec/kernel.js`

 * *Files identical despite different names*

### Comparing `pari-jupyter-1.4.1/spec/logo-64x64.png` & `pari-jupyter-1.4.2/spec/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `pari-jupyter-1.4.1/test/test_pari_jupyter_kernel.py` & `pari-jupyter-1.4.2/test/test_pari_jupyter_kernel.py`

 * *Files identical despite different names*

