# Comparing `tmp/nunavut-2.0.9.tar.gz` & `tmp/nunavut-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nunavut-2.0.9.tar", last modified: Thu Mar  9 14:02:54 2023, max compression
+gzip compressed data, was "nunavut-2.1.0.tar", last modified: Wed Jun  7 23:18:20 2023, max compression
```

## Comparing `nunavut-2.0.9.tar` & `nunavut-2.1.0.tar`

### file list

```diff
@@ -1,132 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.147617 nunavut-2.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-03-09 13:59:31.000000 nunavut-2.0.9/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-03-09 14:02:54.151617 nunavut-2.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-03-09 13:59:31.000000 nunavut-2.0.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-03-09 14:02:54.151617 nunavut-2.0.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      680 2023-03-09 13:59:31.000000 nunavut-2.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.131615 nunavut-2.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.135615 nunavut-2.0.9/src/nunavut/
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    15294 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/_postprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.135615 nunavut-2.0.9/src/nunavut/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    17322 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/cli/runners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.135615 nunavut-2.0.9/src/nunavut/jinja/
--rw-r--r--   0 runner    (1001) docker     (123)    38251 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21298 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.139616 nunavut-2.0.9/src/nunavut/jinja/jinja2/
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/asyncfilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/asyncsupport.py
--rw-r--r--   0 runner    (1001) docker     (123)    12822 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/bccache.py
--rw-r--r--   0 runner    (1001) docker     (123)    65539 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12101 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    51122 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24611 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    37431 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9225 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/idtracking.py
--rw-r--r--   0 runner    (1001) docker     (123)    28746 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17438 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/nativetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    30882 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    36955 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    27700 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    20614 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/jinja2/visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.143616 nunavut-2.0.9/src/nunavut/jinja/markupsafe/
--rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/markupsafe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/markupsafe/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/markupsafe/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/jinja/markupsafe/_native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.143616 nunavut-2.0.9/src/nunavut/lang/
--rw-r--r--   0 runner    (1001) docker     (123)    19108 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27417 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    23941 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    28263 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/_language.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.143616 nunavut-2.0.9/src/nunavut/lang/c/
--rw-r--r--   0 runner    (1001) docker     (123)    35190 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/c/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.143616 nunavut-2.0.9/src/nunavut/lang/c/support/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/c/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32649 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/c/support/serialization.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.143616 nunavut-2.0.9/src/nunavut/lang/c/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/c/templates/DelimitedType.j2
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/c/templates/ServiceType.j2
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/c/templates/StructureType.j2
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/c/templates/UnionType.j2
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/c/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/c/templates/base.j2
--rw-r--r--   0 runner    (1001) docker     (123)    12715 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/c/templates/definitions.j2
--rw-r--r--   0 runner    (1001) docker     (123)    13900 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/c/templates/deserialization.j2
--rw-r--r--   0 runner    (1001) docker     (123)    21356 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/c/templates/serialization.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.143616 nunavut-2.0.9/src/nunavut/lang/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)    54149 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/cpp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.143616 nunavut-2.0.9/src/nunavut/lang/cpp/support/
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/cpp/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42399 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/cpp/support/serialization.j2
--rw-r--r--   0 runner    (1001) docker     (123)    54053 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/cpp/support/variable_length_array.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.147617 nunavut-2.0.9/src/nunavut/lang/cpp/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/cpp/templates/DelimitedType.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/cpp/templates/ServiceType.j2
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/cpp/templates/StructureType.j2
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/cpp/templates/UnionType.j2
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/cpp/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/cpp/templates/_composite_type.j2
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/cpp/templates/_definitions.j2
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/cpp/templates/_fields.j2
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/cpp/templates/_fields_as_union.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/cpp/templates/_fields_as_variant.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/cpp/templates/base.j2
--rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/cpp/templates/deserialization.j2
--rw-r--r--   0 runner    (1001) docker     (123)    17133 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/cpp/templates/serialization.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.147617 nunavut-2.0.9/src/nunavut/lang/html/
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/html/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.147617 nunavut-2.0.9/src/nunavut/lang/html/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/html/templates/DelimitedType.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/html/templates/Namespace.j2
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/html/templates/ServiceType.j2
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/html/templates/StructureType.j2
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/html/templates/UnionType.j2
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/html/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.147617 nunavut-2.0.9/src/nunavut/lang/html/templates/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    80427 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/html/templates/assets/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   154875 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/html/templates/assets/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/html/templates/namespace_base.js
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/html/templates/namespace_info.j2
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/html/templates/sidebar.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/html/templates/type_base.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/html/templates/type_info.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.147617 nunavut-2.0.9/src/nunavut/lang/js/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/js/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/properties.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.147617 nunavut-2.0.9/src/nunavut/lang/py/
--rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.147617 nunavut-2.0.9/src/nunavut/lang/py/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/py/templates/Any.j2
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-09 13:59:31.000000 nunavut-2.0.9/src/nunavut/lang/py/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:02:54.135615 nunavut-2.0.9/src/nunavut.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-03-09 14:02:54.000000 nunavut-2.0.9/src/nunavut.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-03-09 14:02:54.000000 nunavut-2.0.9/src/nunavut.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 14:02:54.000000 nunavut-2.0.9/src/nunavut.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-09 14:02:54.000000 nunavut-2.0.9/src/nunavut.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 14:00:03.000000 nunavut-2.0.9/src/nunavut.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-09 14:02:54.000000 nunavut-2.0.9/src/nunavut.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-09 14:02:54.000000 nunavut-2.0.9/src/nunavut.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.058654 nunavut-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-06-07 23:16:12.000000 nunavut-2.1.0/LICENSE.rst
+-rw-r--r--   0 root         (0) root         (0)    10747 2023-06-07 23:18:20.058654 nunavut-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9343 2023-06-07 23:16:12.000000 nunavut-2.1.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-06-07 23:18:20.058654 nunavut-2.1.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      680 2023-06-07 23:16:12.000000 nunavut-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.038653 nunavut-2.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.042654 nunavut-2.1.0/src/nunavut/
+-rw-r--r--   0 root         (0) root         (0)     4236 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      308 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6127 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/_dependencies.py
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     8097 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/_generators.py
+-rw-r--r--   0 root         (0) root         (0)    15294 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/_namespace.py
+-rw-r--r--   0 root         (0) root         (0)     8744 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/_postprocessors.py
+-rw-r--r--   0 root         (0) root         (0)    11922 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/_templates.py
+-rw-r--r--   0 root         (0) root         (0)     6584 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/_utilities.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.042654 nunavut-2.1.0/src/nunavut/cli/
+-rw-r--r--   0 root         (0) root         (0)    17182 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9778 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/cli/runners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.042654 nunavut-2.1.0/src/nunavut/jinja/
+-rw-r--r--   0 root         (0) root         (0)    38251 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21298 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/environment.py
+-rw-r--r--   0 root         (0) root         (0)     8937 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/extensions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.046654 nunavut-2.1.0/src/nunavut/jinja/jinja2/
+-rw-r--r--   0 root         (0) root         (0)     2523 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2685 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/_compat.py
+-rw-r--r--   0 root         (0) root         (0)     1726 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/_identifier.py
+-rw-r--r--   0 root         (0) root         (0)     4202 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/asyncfilters.py
+-rw-r--r--   0 root         (0) root         (0)     7990 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/asyncsupport.py
+-rw-r--r--   0 root         (0) root         (0)    12822 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/bccache.py
+-rw-r--r--   0 root         (0) root         (0)    65539 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/constants.py
+-rw-r--r--   0 root         (0) root         (0)    12101 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/debug.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/defaults.py
+-rw-r--r--   0 root         (0) root         (0)    51122 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/environment.py
+-rw-r--r--   0 root         (0) root         (0)     4442 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    24611 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/ext.py
+-rw-r--r--   0 root         (0) root         (0)    37431 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/filters.py
+-rw-r--r--   0 root         (0) root         (0)     9225 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/idtracking.py
+-rw-r--r--   0 root         (0) root         (0)    28746 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/lexer.py
+-rw-r--r--   0 root         (0) root         (0)    23098 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/loaders.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/meta.py
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/nativetypes.py
+-rw-r--r--   0 root         (0) root         (0)    30882 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/nodes.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)    36955 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/parser.py
+-rw-r--r--   0 root         (0) root         (0)    27700 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/runtime.py
+-rw-r--r--   0 root         (0) root         (0)    16714 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/sandbox.py
+-rw-r--r--   0 root         (0) root         (0)     4242 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/tests.py
+-rw-r--r--   0 root         (0) root         (0)    20614 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3330 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/jinja2/visitor.py
+-rw-r--r--   0 root         (0) root         (0)    11838 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/loaders.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.046654 nunavut-2.1.0/src/nunavut/jinja/markupsafe/
+-rw-r--r--   0 root         (0) root         (0)    10126 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/markupsafe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/markupsafe/_compat.py
+-rw-r--r--   0 root         (0) root         (0)     4690 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/markupsafe/_constants.py
+-rw-r--r--   0 root         (0) root         (0)     1873 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/jinja/markupsafe/_native.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.050654 nunavut-2.1.0/src/nunavut/lang/
+-rw-r--r--   0 root         (0) root         (0)    19108 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27417 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/_common.py
+-rw-r--r--   0 root         (0) root         (0)    23941 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/_config.py
+-rw-r--r--   0 root         (0) root         (0)    28263 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/_language.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.050654 nunavut-2.1.0/src/nunavut/lang/c/
+-rw-r--r--   0 root         (0) root         (0)    35190 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/c/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.050654 nunavut-2.1.0/src/nunavut/lang/c/support/
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/c/support/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32649 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/c/support/serialization.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.050654 nunavut-2.1.0/src/nunavut/lang/c/templates/
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/c/templates/DelimitedType.j2
+-rw-r--r--   0 root         (0) root         (0)      629 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/c/templates/ServiceType.j2
+-rw-r--r--   0 root         (0) root         (0)      525 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/c/templates/StructureType.j2
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/c/templates/UnionType.j2
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/c/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3460 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/c/templates/base.j2
+-rw-r--r--   0 root         (0) root         (0)    12715 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/c/templates/definitions.j2
+-rw-r--r--   0 root         (0) root         (0)    13900 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/c/templates/deserialization.j2
+-rw-r--r--   0 root         (0) root         (0)    21356 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/c/templates/serialization.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.050654 nunavut-2.1.0/src/nunavut/lang/cpp/
+-rw-r--r--   0 root         (0) root         (0)    54149 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/cpp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.050654 nunavut-2.1.0/src/nunavut/lang/cpp/support/
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/cpp/support/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42399 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/cpp/support/serialization.j2
+-rw-r--r--   0 root         (0) root         (0)    54053 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/cpp/support/variable_length_array.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.054654 nunavut-2.1.0/src/nunavut/lang/cpp/templates/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/cpp/templates/DelimitedType.j2
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/cpp/templates/ServiceType.j2
+-rw-r--r--   0 root         (0) root         (0)      346 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/cpp/templates/StructureType.j2
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/cpp/templates/UnionType.j2
+-rw-r--r--   0 root         (0) root         (0)      342 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/cpp/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8079 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/cpp/templates/_composite_type.j2
+-rw-r--r--   0 root         (0) root         (0)      373 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/cpp/templates/_definitions.j2
+-rw-r--r--   0 root         (0) root         (0)      675 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/cpp/templates/_fields.j2
+-rw-r--r--   0 root         (0) root         (0)     7094 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/cpp/templates/_fields_as_union.j2
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/cpp/templates/_fields_as_variant.j2
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/cpp/templates/base.j2
+-rw-r--r--   0 root         (0) root         (0)    12326 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/cpp/templates/deserialization.j2
+-rw-r--r--   0 root         (0) root         (0)    17133 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/cpp/templates/serialization.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.054654 nunavut-2.1.0/src/nunavut/lang/html/
+-rw-r--r--   0 root         (0) root         (0)     6336 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/html/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.054654 nunavut-2.1.0/src/nunavut/lang/html/support/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/html/support/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.054654 nunavut-2.1.0/src/nunavut/lang/html/templates/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/html/templates/DelimitedType.j2
+-rw-r--r--   0 root         (0) root         (0)     4071 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/html/templates/Namespace.j2
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/html/templates/ServiceType.j2
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/html/templates/StructureType.j2
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/html/templates/UnionType.j2
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/html/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.054654 nunavut-2.1.0/src/nunavut/lang/html/templates/assets/
+-rw-r--r--   0 root         (0) root         (0)    80427 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/html/templates/assets/bootstrap.bundle.min.js
+-rw-r--r--   0 root         (0) root         (0)   154875 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/html/templates/assets/bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)     3257 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/html/templates/namespace_base.js
+-rw-r--r--   0 root         (0) root         (0)      999 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/html/templates/namespace_info.j2
+-rw-r--r--   0 root         (0) root         (0)     5548 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/html/templates/sidebar.j2
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/html/templates/type_base.j2
+-rw-r--r--   0 root         (0) root         (0)     3040 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/html/templates/type_info.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.054654 nunavut-2.1.0/src/nunavut/lang/js/
+-rw-r--r--   0 root         (0) root         (0)      868 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/js/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.054654 nunavut-2.1.0/src/nunavut/lang/js/support/
+-rw-r--r--   0 root         (0) root         (0)      618 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/js/support/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8279 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/properties.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.054654 nunavut-2.1.0/src/nunavut/lang/py/
+-rw-r--r--   0 root         (0) root         (0)    10384 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/py/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.054654 nunavut-2.1.0/src/nunavut/lang/py/support/
+-rw-r--r--   0 root         (0) root         (0)      618 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/py/support/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.058654 nunavut-2.1.0/src/nunavut/lang/py/templates/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/py/templates/Any.j2
+-rw-r--r--   0 root         (0) root         (0)      340 2023-06-07 23:16:12.000000 nunavut-2.1.0/src/nunavut/lang/py/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:18:20.042654 nunavut-2.1.0/src/nunavut.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10747 2023-06-07 23:18:19.000000 nunavut-2.1.0/src/nunavut.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4254 2023-06-07 23:18:20.000000 nunavut-2.1.0/src/nunavut.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 23:18:19.000000 nunavut-2.1.0/src/nunavut.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-07 23:18:19.000000 nunavut-2.1.0/src/nunavut.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 23:16:30.000000 nunavut-2.1.0/src/nunavut.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-07 23:18:19.000000 nunavut-2.1.0/src/nunavut.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-07 23:18:19.000000 nunavut-2.1.0/src/nunavut.egg-info/top_level.txt
```

### Comparing `nunavut-2.0.9/LICENSE.rst` & `nunavut-2.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/PKG-INFO` & `nunavut-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nunavut
-Version: 2.0.9
+Version: 2.1.0
 Summary: Generate code from DSDL using Jinja2 templates.
 Home-page: https://opencyphal.org
 Author: OpenCyphal Development Team
 Author-email: maintainers@opencyphal.org
 License: MIT
 Keywords: uavcan,dsdl,can,can-bus,codegen,cyphal,opencyphal
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nunavut-2.0.9/README.rst` & `nunavut-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/setup.cfg` & `nunavut-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/setup.py` & `nunavut-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/__init__.py` & `nunavut-2.1.0/src/nunavut/__init__.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/_dependencies.py` & `nunavut-2.1.0/src/nunavut/_dependencies.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/_exceptions.py` & `nunavut-2.1.0/src/nunavut/_exceptions.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/_generators.py` & `nunavut-2.1.0/src/nunavut/_generators.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/_namespace.py` & `nunavut-2.1.0/src/nunavut/_namespace.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/_postprocessors.py` & `nunavut-2.1.0/src/nunavut/_postprocessors.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/_templates.py` & `nunavut-2.1.0/src/nunavut/_templates.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/_utilities.py` & `nunavut-2.1.0/src/nunavut/_utilities.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/cli/__init__.py` & `nunavut-2.1.0/src/nunavut/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,17 +104,17 @@
         List of other namespace directories containing data type definitions that are
         referred to from the target root namespace. For example, if you are reading a
         vendor-specific namespace, the list of lookup directories should always include
         a path to the standard root namespace "uavcan", otherwise the types defined in
         the vendor-specific namespace won't be able to use data types from the standard
         namespace.
 
-        Additional directories can also be specified through the environment variable
-        DSDL_INCLUDE_PATH, where the path entries are separated by colons ":" on posix
-        systems and ";" on Windows.
+        Additional directories can also be specified through an environment variable
+        DSDL_INCLUDE_PATH where the path entries are separated by colons ":" on
+        posix systems and ";" on Windows.
 
     """
         ).lstrip(),
     )
 
     parser.add_argument("--verbose", "-v", action="count", help="verbosity level (-v, -vv)")
 
@@ -558,17 +558,15 @@
     logging.info("Running %s using sys.prefix: %s", pathlib.Path(__file__).name, sys.prefix)
 
     #
     # Parse DSDL_INCLUDE_PATH
     #
     extra_includes = args.lookup_dir
 
-    # legacy variable. We'll support this for a time.
-    extra_includes_from_env = _extra_includes_from_env("UAVCAN_DSDL_INCLUDE_PATH")
-    extra_includes_from_env += _extra_includes_from_env("DSDL_INCLUDE_PATH")
+    extra_includes_from_env = _extra_includes_from_env("DSDL_INCLUDE_PATH")
     extra_includes += sorted(extra_includes_from_env)
 
     from nunavut.cli.runners import ArgparseRunner
 
     runner = ArgparseRunner(args, extra_includes)
     runner.run()
     return 0
```

### Comparing `nunavut-2.0.9/src/nunavut/cli/runners.py` & `nunavut-2.1.0/src/nunavut/cli/runners.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/__init__.py` & `nunavut-2.1.0/src/nunavut/jinja/__init__.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/environment.py` & `nunavut-2.1.0/src/nunavut/jinja/environment.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/extensions.py` & `nunavut-2.1.0/src/nunavut/jinja/extensions.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/__init__.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/_compat.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/_identifier.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/asyncfilters.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/asyncfilters.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/asyncsupport.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/asyncsupport.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/bccache.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/compiler.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/constants.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/debug.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/defaults.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/environment.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/exceptions.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/ext.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/filters.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/idtracking.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/lexer.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/meta.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/nativetypes.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/nodes.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/optimizer.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/parser.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/runtime.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/sandbox.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/tests.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/utils.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/jinja2/visitor.py` & `nunavut-2.1.0/src/nunavut/jinja/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/loaders.py` & `nunavut-2.1.0/src/nunavut/jinja/loaders.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/markupsafe/__init__.py` & `nunavut-2.1.0/src/nunavut/jinja/markupsafe/__init__.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/markupsafe/_compat.py` & `nunavut-2.1.0/src/nunavut/jinja/markupsafe/_compat.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/markupsafe/_constants.py` & `nunavut-2.1.0/src/nunavut/jinja/markupsafe/_constants.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/jinja/markupsafe/_native.py` & `nunavut-2.1.0/src/nunavut/jinja/markupsafe/_native.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/__init__.py` & `nunavut-2.1.0/src/nunavut/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/_common.py` & `nunavut-2.1.0/src/nunavut/lang/_common.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/_config.py` & `nunavut-2.1.0/src/nunavut/lang/_config.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/_language.py` & `nunavut-2.1.0/src/nunavut/lang/_language.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/c/__init__.py` & `nunavut-2.1.0/src/nunavut/lang/c/__init__.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/c/support/__init__.py` & `nunavut-2.1.0/src/nunavut/lang/c/support/__init__.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/c/support/serialization.j2` & `nunavut-2.1.0/src/nunavut/lang/c/support/serialization.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/c/templates/ServiceType.j2` & `nunavut-2.1.0/src/nunavut/lang/c/templates/ServiceType.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/c/templates/StructureType.j2` & `nunavut-2.1.0/src/nunavut/lang/c/templates/StructureType.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/c/templates/base.j2` & `nunavut-2.1.0/src/nunavut/lang/c/templates/base.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/c/templates/definitions.j2` & `nunavut-2.1.0/src/nunavut/lang/c/templates/definitions.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/c/templates/deserialization.j2` & `nunavut-2.1.0/src/nunavut/lang/c/templates/deserialization.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/c/templates/serialization.j2` & `nunavut-2.1.0/src/nunavut/lang/c/templates/serialization.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/cpp/__init__.py` & `nunavut-2.1.0/src/nunavut/lang/cpp/__init__.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/cpp/support/__init__.py` & `nunavut-2.1.0/src/nunavut/lang/cpp/support/__init__.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/cpp/support/serialization.j2` & `nunavut-2.1.0/src/nunavut/lang/cpp/support/serialization.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/cpp/support/variable_length_array.hpp` & `nunavut-2.1.0/src/nunavut/lang/cpp/support/variable_length_array.hpp`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/cpp/templates/ServiceType.j2` & `nunavut-2.1.0/src/nunavut/lang/cpp/templates/ServiceType.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/cpp/templates/_composite_type.j2` & `nunavut-2.1.0/src/nunavut/lang/cpp/templates/_composite_type.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/cpp/templates/_fields.j2` & `nunavut-2.1.0/src/nunavut/lang/cpp/templates/_fields.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/cpp/templates/_fields_as_union.j2` & `nunavut-2.1.0/src/nunavut/lang/cpp/templates/_fields_as_union.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/cpp/templates/_fields_as_variant.j2` & `nunavut-2.1.0/src/nunavut/lang/cpp/templates/_fields_as_variant.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/cpp/templates/base.j2` & `nunavut-2.1.0/src/nunavut/lang/cpp/templates/base.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/cpp/templates/deserialization.j2` & `nunavut-2.1.0/src/nunavut/lang/cpp/templates/deserialization.j2`

 * *Files 2% similar despite different names*

```diff
@@ -197,23 +197,23 @@
 {% set first_element_offset = offset + t.length_field_type.bit_length %}
 {% assert (element_offset.min) == (first_element_offset.min) %}
 {% if first_element_offset.is_aligned_at_byte() %}
     {{ assert('in_buffer.offset_alings_to_byte()') }}
 {% endif %}
     {# GENERAL CASE #}
     {% set ref_index = 'index'|to_template_unique_name %}
+    {% set tmp_element = 'tmp'|to_template_unique_name %}
         for ({{ typename_unsigned_length }} {{ ref_index }} = 0U; {{ ref_index }} < {{ ref_size }}; ++{{ ref_index }})
         {
-            // TODO This is terribly inefficient. We need to completely refactor this template to use C++ emplace and
-            // move semantics instead of assuming C-style containers
-            {{ reference }}.push_back();
+            {{ t.element_type | declaration }} {{ tmp_element }} = {{ t.element_type | declaration }}();
             {{
-                _deserialize_any(t.element_type, reference + ('[%s]'|format(ref_index)), element_offset)
+                _deserialize_any(t.element_type, tmp_element, element_offset)
             |trim|indent
             }}
+            {{ reference }}.push_back(std::move({{ tmp_element }}));
         }
 
     }
 {% endmacro %}
 
 
 {# ----------------------------------------------------------------------------------------------------------------- #}
```

### Comparing `nunavut-2.0.9/src/nunavut/lang/cpp/templates/serialization.j2` & `nunavut-2.1.0/src/nunavut/lang/cpp/templates/serialization.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/html/__init__.py` & `nunavut-2.1.0/src/nunavut/lang/html/__init__.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/html/templates/Namespace.j2` & `nunavut-2.1.0/src/nunavut/lang/html/templates/Namespace.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/html/templates/assets/bootstrap.bundle.min.js` & `nunavut-2.1.0/src/nunavut/lang/html/templates/assets/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/html/templates/assets/bootstrap.min.css` & `nunavut-2.1.0/src/nunavut/lang/html/templates/assets/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/html/templates/namespace_base.js` & `nunavut-2.1.0/src/nunavut/lang/html/templates/namespace_base.js`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/html/templates/namespace_info.j2` & `nunavut-2.1.0/src/nunavut/lang/html/templates/namespace_info.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/html/templates/sidebar.j2` & `nunavut-2.1.0/src/nunavut/lang/html/templates/sidebar.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/html/templates/type_base.j2` & `nunavut-2.1.0/src/nunavut/lang/html/templates/type_base.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/html/templates/type_info.j2` & `nunavut-2.1.0/src/nunavut/lang/html/templates/type_info.j2`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/js/__init__.py` & `nunavut-2.1.0/src/nunavut/lang/js/__init__.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/properties.yaml` & `nunavut-2.1.0/src/nunavut/lang/properties.yaml`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut/lang/py/__init__.py` & `nunavut-2.1.0/src/nunavut/lang/py/__init__.py`

 * *Files identical despite different names*

### Comparing `nunavut-2.0.9/src/nunavut.egg-info/PKG-INFO` & `nunavut-2.1.0/src/nunavut.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nunavut
-Version: 2.0.9
+Version: 2.1.0
 Summary: Generate code from DSDL using Jinja2 templates.
 Home-page: https://opencyphal.org
 Author: OpenCyphal Development Team
 Author-email: maintainers@opencyphal.org
 License: MIT
 Keywords: uavcan,dsdl,can,can-bus,codegen,cyphal,opencyphal
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nunavut-2.0.9/src/nunavut.egg-info/SOURCES.txt` & `nunavut-2.1.0/src/nunavut.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -87,24 +87,27 @@
 src/nunavut/lang/cpp/templates/_fields.j2
 src/nunavut/lang/cpp/templates/_fields_as_union.j2
 src/nunavut/lang/cpp/templates/_fields_as_variant.j2
 src/nunavut/lang/cpp/templates/base.j2
 src/nunavut/lang/cpp/templates/deserialization.j2
 src/nunavut/lang/cpp/templates/serialization.j2
 src/nunavut/lang/html/__init__.py
+src/nunavut/lang/html/support/__init__.py
 src/nunavut/lang/html/templates/DelimitedType.j2
 src/nunavut/lang/html/templates/Namespace.j2
 src/nunavut/lang/html/templates/ServiceType.j2
 src/nunavut/lang/html/templates/StructureType.j2
 src/nunavut/lang/html/templates/UnionType.j2
 src/nunavut/lang/html/templates/__init__.py
 src/nunavut/lang/html/templates/namespace_base.js
 src/nunavut/lang/html/templates/namespace_info.j2
 src/nunavut/lang/html/templates/sidebar.j2
 src/nunavut/lang/html/templates/type_base.j2
 src/nunavut/lang/html/templates/type_info.j2
 src/nunavut/lang/html/templates/assets/bootstrap.bundle.min.js
 src/nunavut/lang/html/templates/assets/bootstrap.min.css
 src/nunavut/lang/js/__init__.py
+src/nunavut/lang/js/support/__init__.py
 src/nunavut/lang/py/__init__.py
+src/nunavut/lang/py/support/__init__.py
 src/nunavut/lang/py/templates/Any.j2
 src/nunavut/lang/py/templates/__init__.py
```

