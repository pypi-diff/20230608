# Comparing `tmp/skymarshal-0.8.0.tar.gz` & `tmp/skymarshal-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skymarshal-0.8.0.tar", last modified: Fri Feb  3 20:53:47 2023, max compression
+gzip compressed data, was "skymarshal-0.9.0.tar", last modified: Wed Jun  7 20:23:05 2023, max compression
```

## Comparing `skymarshal-0.8.0.tar` & `skymarshal-0.9.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:53:47.678574 skymarshal-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26611 2023-02-03 20:53:39.000000 skymarshal-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-03 20:53:39.000000 skymarshal-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-02-03 20:53:47.678574 skymarshal-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-02-03 20:53:39.000000 skymarshal-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-02-03 20:53:47.678574 skymarshal-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-03 20:53:39.000000 skymarshal-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:53:47.674574 skymarshal-0.8.0/skymarshal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/common_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25683 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/emit_cpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/emit_djinni.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/emit_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/emit_java.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/emit_lcmout.py
--rw-r--r--   0 runner    (1001) docker     (123)    27557 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/emit_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/emit_python.py
--rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/emit_typescript.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/language_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/lextab_py2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/lextab_py3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/package_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/regenerate_lextab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/skymarshal.py
--rw-r--r--   0 runner    (1001) docker     (123)    33374 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/syntax_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:53:47.678574 skymarshal-0.8.0/skymarshal/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/aggregate.hpp.template
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/djinni_converter.cc.template
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/djinni_converter.h.template
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/djinni_idl.djinni.template
--rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/enumtype.hpp.template
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/forward.hpp.template
--rw-r--r--   0 runner    (1001) docker     (123)     9034 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/lcmtype.hpp.template
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/lcmtype.java.template
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/proto_enum.proto.template
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/proto_struct.proto.template
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/protolcm.cc.template
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/protolcm.h.template
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/python_enum.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/python_enum_default_wrapper.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/python_init.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/python_struct.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/python_struct_default_wrapper.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/typescript_enum.ts.template
--rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/templates/typescript_struct.ts.template
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-02-03 20:53:39.000000 skymarshal-0.8.0/skymarshal/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:53:47.674574 skymarshal-0.8.0/skymarshal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-02-03 20:53:47.000000 skymarshal-0.8.0/skymarshal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-02-03 20:53:47.000000 skymarshal-0.8.0/skymarshal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 20:53:47.000000 skymarshal-0.8.0/skymarshal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-03 20:53:47.000000 skymarshal-0.8.0/skymarshal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-03 20:53:47.000000 skymarshal-0.8.0/skymarshal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:05.103734 skymarshal-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26611 2023-06-07 20:22:57.000000 skymarshal-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 20:22:57.000000 skymarshal-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-07 20:23:05.103734 skymarshal-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-07 20:22:57.000000 skymarshal-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-07 20:23:05.103734 skymarshal-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-07 20:22:57.000000 skymarshal-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:05.099734 skymarshal-0.9.0/skymarshal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/common_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25677 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/emit_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/emit_djinni.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/emit_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/emit_java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/emit_lcmout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27557 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/emit_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/emit_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/emit_typescript.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/language_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/lextab_py2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/lextab_py3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/package_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/regenerate_lextab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/skymarshal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33481 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/syntax_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:05.103734 skymarshal-0.9.0/skymarshal/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/aggregate.hpp.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/djinni_converter.cc.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/djinni_converter.h.template
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/djinni_idl.djinni.template
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/enumtype.hpp.template
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/forward.hpp.template
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/lcmtype.hpp.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/lcmtype.java.template
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/proto_enum.proto.template
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/proto_struct.proto.template
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/protolcm.cc.template
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/protolcm.h.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/python_enum.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/python_enum_default_wrapper.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/python_init.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/python_struct.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/python_struct_default_wrapper.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/typescript_enum.ts.template
+-rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/templates/typescript_struct.ts.template
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-07 20:22:57.000000 skymarshal-0.9.0/skymarshal/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:05.099734 skymarshal-0.9.0/skymarshal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-07 20:23:05.000000 skymarshal-0.9.0/skymarshal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-07 20:23:05.000000 skymarshal-0.9.0/skymarshal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:23:05.000000 skymarshal-0.9.0/skymarshal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-07 20:23:05.000000 skymarshal-0.9.0/skymarshal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 20:23:05.000000 skymarshal-0.9.0/skymarshal.egg-info/top_level.txt
```

### Comparing `skymarshal-0.8.0/LICENSE` & `skymarshal-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/PKG-INFO` & `skymarshal-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skymarshal
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python implementation of marshalling for LCM messages
 Home-page: https://github.com/symforce-org/symforce/tree/main/third_party/skymarshal
 Author: "Skydio, Inc"
 License: LGPL-2.1-or-later
 Project-URL: Bug Tracker, https://github.com/symforce-org/symforce/issues
 Project-URL: Source, https://github.com/symforce-org/symforce/tree/main/third_party/skymarshal
 Classifier: Intended Audience :: Developers
```

### Comparing `skymarshal-0.8.0/setup.cfg` & `skymarshal-0.9.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -16,21 +16,26 @@
 license_file = LICENSE
 url = https://github.com/symforce-org/symforce/tree/main/third_party/skymarshal
 project_urls = 
 	Bug Tracker = https://github.com/symforce-org/symforce/issues
 	Source = https://github.com/symforce-org/symforce/tree/main/third_party/skymarshal
 
 [options]
-packages = find:
+packages = find_namespace:
 python_requires = >= 3.8
 include_package_data = True
 install_requires = 
 	argh
 	jinja2
 	numpy
 	ply
 	six
 
+[options.packages.find]
+include = 
+	skymarshal
+	skymarshal.*
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `skymarshal-0.8.0/skymarshal/__main__.py` & `skymarshal-0.9.0/skymarshal/__main__.py`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/common_util.py` & `skymarshal-0.9.0/skymarshal/common_util.py`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/emit_cpp.py` & `skymarshal-0.9.0/skymarshal/emit_cpp.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,15 +406,15 @@
                         " &%s_cstr, 1);",
                         member.name,
                     )
                 else:
                     size_str = ("v_%s" if virtual else "this->%s") % member.name
                     code(
                         1,
-                        "tlen = __%s_encode_array(buf, offset + pos, maxlen - pos," " &%s, 1);",
+                        "tlen = __%s_encode_array(buf, offset + pos, maxlen - pos, &%s, 1);",
                         map_to_functype(member.type_ref),
                         size_str,
                     )
                 code(1, "if(tlen < 0) return tlen; else pos += tlen;")
             else:
                 self.encode_recursive(code, member, 0, 0)
         code(0, "")
@@ -597,15 +597,15 @@
                     member.name,
                 )
                 code(1, "pos += __%s_len__;", member.name)
             else:
                 size_str = ("v_%s" if virtual else "this->%s") % member.name
                 code(
                     1,
-                    "tlen = __%s_decode_array(buf, offset + pos, maxlen - pos, &%s," " 1);",
+                    "tlen = __%s_decode_array(buf, offset + pos, maxlen - pos, &%s, 1);",
                     map_to_functype(member.type_ref),
                     size_str,
                 )
                 code(1, "if(tlen < 0) return tlen; else pos += tlen;")
 
         else:
             self.decode_recursive(code, member, 0)
```

### Comparing `skymarshal-0.8.0/skymarshal/emit_djinni.py` & `skymarshal-0.9.0/skymarshal/emit_djinni.py`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/emit_helpers.py` & `skymarshal-0.9.0/skymarshal/emit_helpers.py`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/emit_java.py` & `skymarshal-0.9.0/skymarshal/emit_java.py`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/emit_lcmout.py` & `skymarshal-0.9.0/skymarshal/emit_lcmout.py`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/emit_proto.py` & `skymarshal-0.9.0/skymarshal/emit_proto.py`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/emit_python.py` & `skymarshal-0.9.0/skymarshal/emit_python.py`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/emit_typescript.py` & `skymarshal-0.9.0/skymarshal/emit_typescript.py`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/language_plugin.py` & `skymarshal-0.9.0/skymarshal/language_plugin.py`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/lextab_py2.py` & `skymarshal-0.9.0/skymarshal/lextab_py2.py`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/lextab_py3.py` & `skymarshal-0.9.0/skymarshal/lextab_py3.py`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/package_map.py` & `skymarshal-0.9.0/skymarshal/package_map.py`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/parser.py` & `skymarshal-0.9.0/skymarshal/parser.py`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/regenerate_lextab.py` & `skymarshal-0.9.0/skymarshal/regenerate_lextab.py`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/skymarshal.py` & `skymarshal-0.9.0/skymarshal/skymarshal.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 """
 Parse lcm defintion files and generate bindings in different languages.
 """
 from __future__ import absolute_import, print_function
 
 import argparse
 import os
+import shlex
+import sys
 import typing as T
 
 import six
 from skymarshal.language_plugin import SkymarshalLanguage  # pylint: disable=unused-import
 from skymarshal.package_map import parse_lcmtypes
 
 
 def parse_args(languages, args=None):
     # type: (T.Sequence[T.Type[SkymarshalLanguage]], T.Optional[T.Sequence[str]]) -> argparse.Namespace
     """Parse the argument list and return an options object."""
-    parser = argparse.ArgumentParser(description=__doc__, fromfile_prefix_chars="@")
+    parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument("source_path", nargs="+")
     parser.add_argument("--debug-tokens", action="store_true")
     parser.add_argument("--print-def", action="store_true")
     parser.add_argument("--verbose", action="store_true")
     parser.add_argument(
         "--excluded-path",
         nargs="+",
@@ -39,15 +41,25 @@
         lang.add_args(parser)
 
     if args:
         # Caller has provided the argument strings explicitly.
         options = parser.parse_args(args)
     else:
         # Use the command-line args.
-        options = parser.parse_args()
+
+        # NOTE(will): Support argfiles, e.g. @argfile as the first argument. argparse supports this
+        # directly with fromfile_prefix_chars="@", but this was causing issues for any arguments
+        # that started with @, even if those arguments were inside the argfile. This approach is
+        # much narrower in only supporting an argfile as the first argument.
+        if len(sys.argv) >= 2 and sys.argv[1].startswith("@"):
+            with open(sys.argv[1][1:]) as argfile:
+                args = shlex.split(argfile.read())
+            options = parser.parse_args(args + sys.argv[2:])
+        else:
+            options = parser.parse_args()
 
     return options
 
 
 def main(
     languages,  # type: T.Sequence[T.Type[SkymarshalLanguage]]
     args=None,  # type: T.Sequence[str]
```

### Comparing `skymarshal-0.8.0/skymarshal/syntax_tree.py` & `skymarshal-0.9.0/skymarshal/syntax_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 for float_type in FLOAT_TYPES:
     CONST_TYPE_MAP[float_type] = float
 
 
 class Hash(object):
     def __init__(self):
+        # type: () -> None
         self.val = int64(0x12345678)
         # TODO(matt): is it possible to remove the int64 dependency?
 
     def update(self, byte):
         """Make the hash dependent on the value of the given character.
         The order that hash_update is called in IS important."""
         self.val = ((self.val << 8) ^ (self.val >> 55)) + byte
@@ -51,14 +52,15 @@
 
         for char in string:
             # NOTE(matt): This restricts the names to be ASCII characters
             self.update(ord(char))
 
     @property
     def int_value(self):
+        # type: () -> int
         # convert to uint64-like number
         # NOTE(matt): this is still a python int, and thus has infinite size
         return int(self.val) & 0xFFFFFFFFFFFFFFFF
 
     def hex_no_padding(self):
         return "0x{0:x}".format(self.int_value)
 
@@ -398,14 +400,15 @@
                         case.int_value,
                         cases_by_id[case.int_value],
                     )
                 )
             cases_by_id[case.int_value] = case.name
 
     def compute_hash(self):
+        # type: () -> Hash
         return self.equivalent_struct.compute_hash()
 
 
 class EnumCase(AstNode):
     """A name/value case of an lcm enum type"""
 
     def __init__(self, name, value_str):
@@ -568,14 +571,15 @@
                         member.field_id,
                     )
                 )
             if member.field_id is not None:
                 field_ids.add(member.field_id)
 
     def compute_hash(self):
+        # type: () -> Hash
         type_hash = Hash()
         for member in self.members:
             if not isinstance(member, ConstMember):
                 member.compute_hash(type_hash)
         return type_hash
```

### Comparing `skymarshal-0.8.0/skymarshal/templates/djinni_converter.cc.template` & `skymarshal-0.9.0/skymarshal/templates/djinni_converter.cc.template`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/templates/djinni_converter.h.template` & `skymarshal-0.9.0/skymarshal/templates/djinni_converter.h.template`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/templates/enumtype.hpp.template` & `skymarshal-0.9.0/skymarshal/templates/enumtype.hpp.template`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,18 @@
          * Retrieve the 64-bit fingerprint identifying the structure of the message.
          * Note that the fingerprint is the same for all instances of the same
          * message type, and is a fingerprint on the message type definition, not on
          * the message contents.
          */
         constexpr static int64_t getHash();
 
+        using type_name_array_t = const char[{{enumtype.name|length + 1}}];
+
+        inline static constexpr type_name_array_t* getTypeNameArrayPtr();
+
         /**
          * Returns "{{enumtype.name}}"
          */
         inline static constexpr const char* getTypeName();
 
         /**
          * Returns "{{enumtype.namespace}}"
@@ -153,17 +157,21 @@
 }
 
 constexpr int64_t {{enumtype.name}}::getHash()
 {
     return _computeHash(NULL);
 }
 
+constexpr {{enumtype.name}}::type_name_array_t* {{enumtype.name}}::getTypeNameArrayPtr() {
+    return &"{{enumtype.name}}";
+}
+
 constexpr const char* {{enumtype.name}}::getTypeName()
 {
-    return "{{enumtype.name}}";
+    return *{{enumtype.name}}::getTypeNameArrayPtr();
 }
 
 constexpr const char * {{enumtype.name}}::getPackageName()
 {
     return "{{enumtype.namespace}}";
 }
```

### Comparing `skymarshal-0.8.0/skymarshal/templates/lcmtype.hpp.template` & `skymarshal-0.9.0/skymarshal/templates/lcmtype.hpp.template`

 * *Files 10% similar despite different names*

```diff
@@ -151,18 +151,14 @@
                 }
             }
             stream << "]"{{comma(loop.last)}};
         {% else %}
             {# Multidimensional arrays will require some complicated stuff #}
             stream << "{{member.name}}=<MULTIDIMENSIONAL ARRAY {{ array_type_str(member) }}>"{{ comma(loop.last) }};
         {% endif %}
-    {% elif "eigen_lcm" in member.type_ref.full_name %}
-            {# We currently don't have operator<< for eigen_lcm types, or a way to regenerate the
-             # bindings :) #}
-            stream << "{{member.name}}=<EIGEN_LCM TYPE {{ member.type_ref.full_name }}>"{{ comma(loop.last) }};
     {% else %}
             stream << "{{member.name}}=" << obj.{{member.name}}{{ comma(loop.last) }};
     {% endif %}
 {% endfor %}
             stream << ")";
 {% if not lcmtype.cpp_display_everywhere %}
 #else
```

### Comparing `skymarshal-0.8.0/skymarshal/templates/lcmtype.java.template` & `skymarshal-0.9.0/skymarshal/templates/lcmtype.java.template`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/templates/proto_enum.proto.template` & `skymarshal-0.9.0/skymarshal/templates/proto_enum.proto.template`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/templates/proto_struct.proto.template` & `skymarshal-0.9.0/skymarshal/templates/proto_struct.proto.template`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/templates/protolcm.cc.template` & `skymarshal-0.9.0/skymarshal/templates/protolcm.cc.template`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/templates/protolcm.h.template` & `skymarshal-0.9.0/skymarshal/templates/protolcm.h.template`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/templates/python_enum.py.template` & `skymarshal-0.9.0/skymarshal/templates/python_enum.py.template`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from io import BytesIO
 import enum
 import struct
-import typing as T  # pylint: disable=unused-import
 
-class {{enumtype.name}}(enum.Enum):  # type: ignore[no-redef]
+class {{enumtype.name}}(enum.Enum):
     {% if enumtype.comment %}
     """{{enumtype.comment}}"""
     {% endif %}
 
 {% for case in enumtype.cases %}
     {{case.name}} = {{case.int_value}}
 {% endfor %}
```

### Comparing `skymarshal-0.8.0/skymarshal/templates/python_struct.py.template` & `skymarshal-0.9.0/skymarshal/templates/python_struct.py.template`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/templates/typescript_enum.ts.template` & `skymarshal-0.9.0/skymarshal/templates/typescript_enum.ts.template`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/templates/typescript_struct.ts.template` & `skymarshal-0.9.0/skymarshal/templates/typescript_struct.ts.template`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal/tokenizer.py` & `skymarshal-0.9.0/skymarshal/tokenizer.py`

 * *Files identical despite different names*

### Comparing `skymarshal-0.8.0/skymarshal.egg-info/PKG-INFO` & `skymarshal-0.9.0/skymarshal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skymarshal
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python implementation of marshalling for LCM messages
 Home-page: https://github.com/symforce-org/symforce/tree/main/third_party/skymarshal
 Author: "Skydio, Inc"
 License: LGPL-2.1-or-later
 Project-URL: Bug Tracker, https://github.com/symforce-org/symforce/issues
 Project-URL: Source, https://github.com/symforce-org/symforce/tree/main/third_party/skymarshal
 Classifier: Intended Audience :: Developers
```

### Comparing `skymarshal-0.8.0/skymarshal.egg-info/SOURCES.txt` & `skymarshal-0.9.0/skymarshal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

