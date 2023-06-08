# Comparing `tmp/PyXB-CTC-1.3.0.dev0.tar.gz` & `tmp/PyXB-CTC-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyXB-CTC-1.3.0.dev0.tar", last modified: Thu Jun  8 16:33:43 2023, max compression
+gzip compressed data, was "PyXB-CTC-1.3.0rc1.tar", last modified: Thu Jun  8 16:47:47 2023, max compression
```

## Comparing `PyXB-CTC-1.3.0.dev0.tar` & `PyXB-CTC-1.3.0rc1.tar`

### file list

```diff
@@ -1,883 +1,883 @@
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    11358 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/LICENSE
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1104 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/MANIFEST.in
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1014 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/NOTICE
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1983 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/PKG-INFO
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.284035 PyXB-CTC-1.3.0.dev0/PyXB_CTC.egg-info/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1983 2023-06-08 16:33:43.000000 PyXB-CTC-1.3.0.dev0/PyXB_CTC.egg-info/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    23730 2023-06-08 16:33:43.000000 PyXB-CTC-1.3.0.dev0/PyXB_CTC.egg-info/SOURCES.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2023-06-08 16:33:43.000000 PyXB-CTC-1.3.0.dev0/PyXB_CTC.egg-info/dependency_links.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        5 2023-06-08 16:33:43.000000 PyXB-CTC-1.3.0.dev0/PyXB_CTC.egg-info/top_level.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      570 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/README.md
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      712 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/README.txt.in
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.288035 PyXB-CTC-1.3.0.dev0/doc/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       16 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/.gitignore
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.288035 PyXB-CTC-1.3.0.dev0/doc/Images/
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)    93415 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/Images/BindingModel.jpg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)    69824 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/Images/CTDValidationExceptions.jpg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)   104867 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/Images/ComponentModel.jpg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)    94495 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/Images/ContentModel.jpg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)   120680 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/Images/FACAutomaton.jpg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)    80210 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/Images/Namespace.jpg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)    97368 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/Images/NamespaceArchive.jpg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)    92897 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/Images/NamespaceCore.jpg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)    72462 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/Images/RuntimeExceptions.jpg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)    83121 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/Images/ScopedDeclarations.jpg
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1532 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/Makefile
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.288035 PyXB-CTC-1.3.0.dev0/doc/_templates/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      415 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/_templates/layout.html
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    16442 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/arch_binding.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4680 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/arch_component.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     9727 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/arch_content.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    16096 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/arch_namespaces.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      731 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/architecture.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    31515 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/bundles.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6542 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/conf.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6560 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/conf.py.in
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4798 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/documentation.cfg
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      173 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/eltonly.xhtml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     5506 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/examples.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2101 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/extapi.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4511 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/index.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1336 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/legal.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2783 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/limitations.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     8587 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/maintref.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      147 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/overview.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3479 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/overview_how.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1396 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/overview_what.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1267 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/pyxb.binding.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      851 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/pyxb.namespace.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      438 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/pyxb.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1840 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/pyxb.utils.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      365 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/pyxb.xmlschema.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    18100 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/pyxbgen_cli.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1408 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/related.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    35080 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/releases.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      171 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/userref_index.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    15064 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/userref_pyxbgen.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    12129 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/userref_usebind.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4993 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/userref_validating.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     5694 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/doc/vision.txt
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.280035 PyXB-CTC-1.3.0.dev0/examples/
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.288035 PyXB-CTC-1.3.0.dev0/examples/cablelabs/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      524 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/cablelabs/README.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      508 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/cablelabs/custom.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2776 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/cablelabs/demo.py
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)       60 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/cablelabs/disabled-test.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1022 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/cablelabs/genbindings.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.288035 PyXB-CTC-1.3.0.dev0/examples/content/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      625 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/content/content.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      133 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/content/showcontent.out
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      261 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/content/showcontent.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      133 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/content/test.expected
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      283 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/content/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.288035 PyXB-CTC-1.3.0.dev0/examples/customization/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      889 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/customization/README.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2051 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/customization/custom.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3504 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/customization/introspect.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      541 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/customization/normal.py
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      415 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/customization/test.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      420 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/customization/test.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2431 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/customization/tst-introspect.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2575 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/customization/tst-normal.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.288035 PyXB-CTC-1.3.0.dev0/examples/dictionary/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      340 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/dictionary/README.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      684 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/dictionary/define.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      392 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/dictionary/genbindings.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      676 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/dictionary/showdict.expected
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1148 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/dictionary/showdict.py
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      247 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/dictionary/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.288035 PyXB-CTC-1.3.0.dev0/examples/geocoder/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3484 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/geocoder/GeoCoder.wsdl-patch
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      151 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/geocoder/README.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2471 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/geocoder/client.py
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)       41 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/geocoder/disabled-test.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      388 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/geocoder/genbindings.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.288035 PyXB-CTC-1.3.0.dev0/examples/kml/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1047 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/kml/genbindings.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.292035 PyXB-CTC-1.3.0.dev0/examples/manual/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1703 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/address.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      340 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/badcontent.expected
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      340 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/badcontent.out
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      232 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/badcontent.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      846 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/badcontent.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      131 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo.expected
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      608 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      131 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo1.out
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      339 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo1.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       31 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo1.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      329 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo2.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       30 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo2.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      329 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo3.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       30 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo3a.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo3b.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       74 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo3c1.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       53 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo3c2.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      169 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4.expected
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       54 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      169 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4a.out
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      264 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4a.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1063 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4a1.expected
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4a1.out
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      238 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4a1.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      169 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4a2.out
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      264 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4a2.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      234 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4b.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       53 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4b.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      463 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4c.out
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      504 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4c.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      853 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4c1.expected
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      853 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4c1.out
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      543 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4c1.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1032 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4c2.expected
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1032 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4c2.out
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      834 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4c2.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1001 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4c3.expected
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1001 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4c3.out
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1020 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/demo4c3.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      154 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/nsaddress.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2083 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/po.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      844 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/po1.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2083 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/po1.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      926 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/po2.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1705 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/po2.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      844 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/po3.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1772 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/po3.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      812 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/po4.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1900 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/po4.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     2221 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/manual/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.292035 PyXB-CTC-1.3.0.dev0/examples/ndfd/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      768 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/ndfd/README.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2463 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/ndfd/forecast.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1033 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/ndfd/genbindings.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     7119 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/ndfd/latlon.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       23 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/ndfd/ndfd.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2976 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/ndfd/showreq.expected
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2083 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/ndfd/showreq.py
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      512 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/ndfd/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.292035 PyXB-CTC-1.3.0.dev0/examples/tmsxtvd/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       66 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/tmsxtvd/README.md
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)       39 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/tmsxtvd/disabled-test.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2808 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/tmsxtvd/dumpsample.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      379 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/tmsxtvd/genbindings.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.292035 PyXB-CTC-1.3.0.dev0/examples/ucum/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      219 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/ucum/README.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1323 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/ucum/showunits.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    10479 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/ucum/test.expected
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      356 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/ucum/test.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     5365 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/ucum/ucum-essence.xsd
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.292035 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3410 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/README.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2100 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/check.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.292035 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.292035 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/euc-jp/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1863 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/euc-jp/FG-GML-13-RailCL25000-20080331-0001.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    29042 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/euc-jp/FGD_GMLSchema.xsd
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.292035 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/iso-2022-jp/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1898 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/iso-2022-jp/FG-GML-13-RailCL25000-20080331-0001.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    31051 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/iso-2022-jp/FGD_GMLSchema.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/readme.txt
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.292035 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/shift_jis/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1935 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/shift_jis/FG-GML-13-RailCL25000-20080331-0001.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    29854 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/shift_jis/FGD_GMLSchema.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      673 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/shift_jis/readme.txt
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.292035 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/utf-8/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1902 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/utf-8/FG-GML-13-RailCL25000-20080331-0001.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    30642 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/utf-8/FGD_GMLSchema.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     2362 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/pyxbgen_jp
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     1200 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/unicode_jp/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.296035 PyXB-CTC-1.3.0.dev0/examples/weather/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      549 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/weather/README.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1622 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/weather/client.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      845 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/weather/client_get.py
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/weather/disabled-test.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      299 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/weather/genbindings.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.296035 PyXB-CTC-1.3.0.dev0/examples/xhtml/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      553 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/xhtml/README.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      383 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/xhtml/expout.xhtml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      985 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/xhtml/generate.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      359 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/xhtml/rewrite.py
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      731 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/xhtml/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.296035 PyXB-CTC-1.3.0.dev0/examples/xsdprimer/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      680 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/xsdprimer/README.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1738 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/xsdprimer/address.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      201 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/xsdprimer/demo.expected
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      648 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/xsdprimer/demo.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      138 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/xsdprimer/genbindings.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1858 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/xsdprimer/ip.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      431 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/xsdprimer/ipo.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1068 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/xsdprimer/ipo.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1925 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/xsdprimer/ipo.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      683 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/xsdprimer/saxdemo.py
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      240 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/examples/xsdprimer/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.296035 PyXB-CTC-1.3.0.dev0/maintainer/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4092 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/maintainer/analysis-2111.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     5619 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/maintainer/buildUnicode.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2541 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/maintainer/bundlesupport.sh
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      306 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/maintainer/genall
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      867 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/maintainer/genbundles
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     5965 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/maintainer/gendoc
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      460 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/maintainer/genpd.sh
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      877 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/maintainer/getw3c.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      180 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/maintainer/howto-release.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      644 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/maintainer/logging.cfg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      464 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/maintainer/testall
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      180 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/maintainer/usepyxb.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.296035 PyXB-CTC-1.3.0.dev0/pyxb/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    16409 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/__init__.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    16409 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/__init__.py.in
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.296035 PyXB-CTC-1.3.0.dev0/pyxb/binding/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      398 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/binding/__init__.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)   119990 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/binding/basis.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    51781 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/binding/content.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    52599 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/binding/datatypes.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    53439 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/binding/facets.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)   132778 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/binding/generate.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    18006 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/binding/saxer.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3079 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/binding/xml_.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.296035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       14 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/.gitignore
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1037 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/README
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       65 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/__init__.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.296035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/common/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       90 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/common/__init__.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.296035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/common/scripts/
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      887 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/common/scripts/genbind
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1091 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/common/xhtml1.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/common/xlink.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/common/xsd_hfp.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.296035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/dc/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/dc/__init__.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       37 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/dc/dc.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/dc/dcmitype.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       42 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/dc/dcterms.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.296035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/dc/scripts/
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      829 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/dc/scripts/genbind
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.296035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/ecma376/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       25 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/ecma376/.gitignore
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/ecma376/__init__.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.296035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/ecma376/scripts/
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     4087 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/ecma376/scripts/genbind
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.300035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1291 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/README.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/__init__.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/_ogc.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/_sam.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       45 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/_sams.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/atom.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.300035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/citygml/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/citygml/__init__.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       58 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/citygml/appearance.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       52 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/citygml/base.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       56 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/citygml/building.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       61 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/citygml/cityFurniture.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       63 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/citygml/cityObjectGroup.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       56 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/citygml/generics.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       55 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/citygml/landUse.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       54 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/citygml/relief.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       63 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/citygml/texturedSurface.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/citygml/transportation.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       58 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/citygml/vegetation.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       57 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/citygml/waterBody.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       49 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/csw_2_0_2.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/csw_dc.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/csw_dct.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.300035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/examples/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       10 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/examples/.gitignore
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      614 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/examples/check_oseo.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      688 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/examples/check_sos.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      580 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/examples/check_wps.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      172 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/examples/demo.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      686 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/examples/gmlapp.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     1307 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/examples/test.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1235 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/examples/testgml.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/fes_2_0.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/filter.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/gml.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/gml_3_2.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.300035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/gml_3_3/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/gml_3_3/__init__.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       50 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/gml_3_3/ce.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       51 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/gml_3_3/exr.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       50 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/gml_3_3/lr.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       51 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/gml_3_3/lro.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       52 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/gml_3_3/lrov.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       52 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/gml_3_3/lrtr.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       53 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/gml_3_3/rgrid.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       51 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/gml_3_3/tin.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       51 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/gml_3_3/xbt.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       45 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/gmlsf.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       50 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/ic_ism_2_1.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.300035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/iso19139/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/iso19139/__init__.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.300035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/iso19139/v20070417/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/iso19139/v20070417/__init__.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/iso19139/v20070417/gco.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/iso19139/v20070417/gmd.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/iso19139/v20070417/gmx.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/iso19139/v20070417/gsr.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/iso19139/v20070417/gss.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/iso19139/v20070417/gts.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.300035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/misc/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/misc/__init__.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       48 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/misc/xAL.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       51 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/misc/xlinks.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       48 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/ogckml22.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/om_1_0.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/om_2_0.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       72 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/oseo_1_0.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/ows.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/ows_1_1.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/ows_2_0.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       52 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/sampling_1_0.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.300035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/scripts/
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6370 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/scripts/genbind
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       54 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/sensorML_1_0_1.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/smil20.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       50 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/smil20lang.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/sos_1_0.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/sos_2_0.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       49 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/swe_1_0_0.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       49 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/swe_1_0_1.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/swe_2_0.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       48 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/swes_2_0.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/tml.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/waterml.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/wcs_1_1.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/wfs.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       73 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/wps_1_0_0.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.300035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/reqif/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       67 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/reqif/ReqIF.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/reqif/__init__.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       68 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/reqif/_xh11d.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       68 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/reqif/driver.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.300035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/reqif/examples/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      209 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/reqif/examples/process.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       66 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/reqif/examples/test.expected
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      479 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/reqif/examples/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.300035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/reqif/scripts/
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     3007 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/reqif/scripts/genbind
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.304035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/saml20/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/saml20/__init__.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       48 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/saml20/assertion.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       42 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/saml20/dce.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       42 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/saml20/ecp.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/saml20/metadata.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/saml20/protocol.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.304035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/saml20/scripts/
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     1000 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/saml20/scripts/genbind
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/saml20/x500.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/saml20/xacml.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.304035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/__init__.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/bpws.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       42 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/ds.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      679 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/httpbind.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       48 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/mimebind.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       70 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/sawsdl.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.304035 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/scripts/
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     1927 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/scripts/genbind
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/soap11.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/soap12.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      926 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/soapbind11.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      997 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/soapbind12.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/soapenc.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       45 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/whttp.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wsa.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wsam.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wscoor.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    11735 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wsdl11.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      211 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wsdl20.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       45 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wsdli.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       45 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wsdlx.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wsnt.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       45 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wsoap.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wsp.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       49 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wsp200607.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wsrf_bf.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wsrf_br.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wsrm.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wsse.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       45 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wstop.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wsu.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/xenc.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    44301 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/exceptions_.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.304035 PyXB-CTC-1.3.0.dev0/pyxb/namespace/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    45378 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/namespace/__init__.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    42053 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/namespace/archive.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    13985 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/namespace/builtin.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    37710 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/namespace/resolution.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3037 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/namespace/utility.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.304035 PyXB-CTC-1.3.0.dev0/pyxb/utils/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       79 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/utils/__init__.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3595 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/utils/activestate.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    26473 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/utils/domutils.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    75560 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/utils/fac.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    10706 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/utils/saxdom.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    22408 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/utils/saxutils.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    30681 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/utils/six.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4046 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/utils/templates.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    22670 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/utils/unicode.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    88512 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/utils/unicode_data.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    48675 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/utils/utility.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    12909 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/utils/xmlre.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.304035 PyXB-CTC-1.3.0.dev0/pyxb/xmlschema/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      518 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/xmlschema/__init__.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)   228632 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/pyxb/xmlschema/structures.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.304035 PyXB-CTC-1.3.0.dev0/scripts/
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     1516 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/scripts/pyxbdump
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     2670 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/scripts/pyxbgen
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     1892 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/scripts/pyxbwsdl
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/setup.cfg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)    10333 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/setup.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.304035 PyXB-CTC-1.3.0.dev0/tests/
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.304035 PyXB-CTC-1.3.0.dev0/tests/bindings/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    14753 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/bindings/test-constraints.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.304035 PyXB-CTC-1.3.0.dev0/tests/bugs/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4068 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/bugs/test-200907231705.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2065 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/bugs/test-200907231924.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1146 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/bugs/test-200907251353.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2351 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/bugs/test-200907261730.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1765 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/bugs/test-200908021351.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1624 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/bugs/test-200908041708.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3859 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/bugs/test-200908111918.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2260 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/bugs/test-200908161024.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      693 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/bugs/test-200908181430.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1252 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/bugs/test-200908231005.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2480 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/bugs/test-200908271556.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.284035 PyXB-CTC-1.3.0.dev0/tests/complex/
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.308035 PyXB-CTC-1.3.0.dev0/tests/complex/nsaugment/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      446 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsaugment/app.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      333 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsaugment/common.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      330 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsaugment/common4app.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      921 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsaugment/test.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1069 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsaugment/tst-app.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      486 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsaugment/tst-common.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.308035 PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      500 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/a_b.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      465 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/a_c.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      473 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/a_x.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      499 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/b_b.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      570 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/b_c.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      499 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/c_b.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      592 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/c_c.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      869 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/d_c.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      348 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/shared.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      296 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/test.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      740 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/tst-a.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1528 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/tst-b.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.308035 PyXB-CTC-1.3.0.dev0/tests/complex/nsext/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsext/README
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      397 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsext/app.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      332 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsext/base.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      508 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsext/extend.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     1074 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsext/test.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      848 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsext/tst-app.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      485 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsext/tst-base.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      672 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/complex/nsext/tst-extend.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.308035 PyXB-CTC-1.3.0.dev0/tests/datatypes/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      799 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-ENTITIES.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      787 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-ENTITY.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      775 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-ID.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      784 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-IDREF.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      789 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-IDREFS.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4944 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-IntegerTypes.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      787 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-NCName.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      994 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-NMTOKEN.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1090 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-NMTOKENS.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      799 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-Name.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1742 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-QName.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      705 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-anyType.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3252 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-base64Binary.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      906 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-boolean.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2780 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-date.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4183 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-dateTime.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3866 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-decimal.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      351 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-double.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     5228 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-duration.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      350 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-float.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1703 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-gDay.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1720 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-gMonth.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2534 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-gMonthDay.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1582 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-gYear.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2478 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-gYearMonth.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1752 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-hexBinary.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2109 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-integer.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      668 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-language.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      959 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-normalizedString.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      351 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-string.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2509 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-time.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1254 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/test-token.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      356 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/totest-NOTATION.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      366 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/totest-anySimpleType.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      352 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/datatypes/totest-anyURI.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.308035 PyXB-CTC-1.3.0.dev0/tests/documents/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       76 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/documents/qattr1.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      111 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/documents/qattr2.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      146 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/documents/qattr3.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       92 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/documents/substgroup-001.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       90 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/documents/substgroup-002.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      138 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/documents/substgroup-003.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      190 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/documents/test-empty-cstd-001.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      179 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/documents/test-empty-cstd-002.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      355 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/documents/test-mg-choice-001.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       85 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/documents/test-mg-choice-002.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       85 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/documents/test-mg-choice-003.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      112 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/documents/test-namespace-uu-001.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      127 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/documents/test-namespace-uu-002.xml
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.308035 PyXB-CTC-1.3.0.dev0/tests/documents/union/
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      325 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/documents/union/test-union-001.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4445 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/documents/wsdl-001.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2214 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/documents/wsdl-002.xml
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.312035 PyXB-CTC-1.3.0.dev0/tests/drivers/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6863 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-ctd-attr.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4287 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-ctd-extension.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1997 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-ctd-simple.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1224 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-deconflict.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1328 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-empty-cstd.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     5698 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-enumeration.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6638 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-external.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1197 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-facets.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      533 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-generatorGetCommandLineArgs.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1046 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-include-aaq.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      785 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-include-aau.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      600 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-include-ad.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1094 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-include-daq.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1566 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-include-dau.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      601 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-include-dcu.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1094 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-include-ddq.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1424 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-include-ddu.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     7480 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-mg-all.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     7945 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-mg-choice.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     8680 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-mg-sequence.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2257 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-namespace-uu.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     5414 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-particle.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     5975 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-po1.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3606 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-properties.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1384 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-properties2.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3051 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-recursive.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      735 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-simplerange.py
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      477 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-stored.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4159 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-substgroup.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2343 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-time.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1032 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-typeinf.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4878 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-union.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     9927 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-wildcard.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     9790 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-xsi-nil.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4325 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/test-xsi-type.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1509 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/drivers/tst-stored.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.312035 PyXB-CTC-1.3.0.dev0/tests/pyxb/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1574 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/pyxb/test-cdata.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6163 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/pyxb/test-namespace.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      739 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/pyxb/test-reserved.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.316035 PyXB-CTC-1.3.0.dev0/tests/schemas/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      432 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/absentns.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      854 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/alt-po1.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      655 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/anyType.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      390 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/blockfinal.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      722 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/components.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2813 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/enumerations.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      603 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/incl-absent.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      666 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/incl-ad.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      604 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/incl-dau.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      676 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/incl-dcu.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      668 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/incl-ddq.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      668 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/incl-ddu.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      662 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/incl-declared2.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     1169 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/nested-groups.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1735 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/particle.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      848 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/po1.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      779 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/qattr.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2087 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/shared-types.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      709 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/substgroup.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      446 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-ambiguous.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      520 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-collision.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2932 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-ctd-attr.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2081 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-ctd-extension.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1490 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-ctd-simple.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      466 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-deconflict.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      669 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-empty-cstd.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1763 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-external.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      489 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-facets.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      397 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-include-aaq.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      366 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-include-aau.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      435 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-include-ad.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      470 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-include-daq.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      489 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-include-dau.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      542 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-include-dcu.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      470 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-include-ddq.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      489 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-include-ddu.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1069 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-mg-all.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1265 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-mg-choice.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      715 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-mg-sequence.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      622 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-namespace-uu.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1128 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-recursive.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      227 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-simplerange.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2013 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-typeinf.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     2462 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-union.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      666 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/test-wildcard.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      926 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/time.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      619 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/validatable.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      956 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/xsi-nil.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2597 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/schemas/xsi-type.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1628 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/support.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.320035 PyXB-CTC-1.3.0.dev0/tests/trac/
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.320035 PyXB-CTC-1.3.0.dev0/tests/trac/issue-0048/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      376 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/issue-0048/check.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      383 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/issue-0048/profile-base.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      675 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/issue-0048/profile.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)       75 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/issue-0048/test.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1706 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0006.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2309 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0007.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2916 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0013.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2357 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0014.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1537 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0015.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1242 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0019.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1740 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0022.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1252 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0027.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1019 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0031.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1984 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0032.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      877 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0043.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1744 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0047.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1822 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0051.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1121 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0066.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1541 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0069.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2199 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0071.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1700 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0073.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2578 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0078.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2473 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0079.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2173 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0092.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2497 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0094.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1758 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0021.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1550 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0023.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1488 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0023b.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1297 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0023c.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     7270 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0027.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2681 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0027b.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2512 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0027c.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1463 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0029.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4227 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0032.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1530 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0033a.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2512 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0034.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2629 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0034b.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2446 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0036.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3757 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0037.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2719 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0038.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4008 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0039.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2858 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0040.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1240 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0045.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1096 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0046.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4173 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0047.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1422 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0048.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1365 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0051.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1816 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0052.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2222 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0053.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1970 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0056.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4582 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0057.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1181 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0058.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    15006 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0060.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4003 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0061.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3818 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0069.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     7018 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0071.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1996 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0074.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3083 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0075.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1202 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0076.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1796 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0079.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1914 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0087.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1508 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0088.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2957 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0089.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4794 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0091.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      681 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0093.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3571 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0094.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4219 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0099.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1895 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0099a.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2213 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0100.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1467 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0110.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1873 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0111.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2344 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0112.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      834 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0116.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2151 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0117.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      768 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0121.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2629 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0122.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2272 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0123.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1630 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0126.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4064 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0131.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      501 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0132.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1904 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0136.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2366 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0137.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      447 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0138.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6523 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0139.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2116 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0141.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      967 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0148.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6656 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0153.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1737 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0154.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2713 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0155.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1124 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0156a.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1558 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0163.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1992 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0172.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1982 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0175.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1453 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0179.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1998 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0181.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1502 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0182.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1933 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0184.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2459 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0189.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2294 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0190.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1292 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0191.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1286 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0194.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1999 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0195.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2647 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0200.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1172 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0201.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1640 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0203.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1628 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0204.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1251 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0206.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      880 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0207.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1243 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0208.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     7383 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0211.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1805 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0212.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1737 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0213.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1522 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0216.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1347 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0218.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2022 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0219.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3805 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0221.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2146 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0231.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2142 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0232.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.320035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0026/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3119 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0026/check-binding.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    45154 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0026/check-validation.py
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      291 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0026/test.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6244 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0026/trac26.xsd
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.320035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0033/
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      114 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0033/test.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1731 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0033/tread.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.320035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0043/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      579 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0043/a.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      581 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0043/b.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      178 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0043/test.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      638 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0043/tst-1.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      598 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0043/tst-2.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.320035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0065/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      778 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0065/TestSchema.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     2299 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0065/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.320035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0072/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      149 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0072/a.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      149 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0072/b.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      404 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0072/xtest.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.320035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0073/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      365 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0073/base.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      486 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0073/check.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      598 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0073/profile.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      186 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0073/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.320035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0080/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2528 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0080/check.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1700 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0080/multipleRestriction.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)       57 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0080/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.320035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0084/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      503 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0084/example.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      191 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0084/test.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      149 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0084/tryit.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.320035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0088/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      433 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0088/example.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      180 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0088/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.320035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0089/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       15 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0089/bad1.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       17 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0089/bad2.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       23 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0089/bad3.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      892 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0089/example.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       15 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0089/good1.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       17 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0089/good2.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       23 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0089/good3.xml
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      505 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0089/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.320035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0092/
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      528 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0092/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.320035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0104/
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.284035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0104/XSD/
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.320035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0104/XSD/ModelA/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3336 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0104/XSD/ModelA/AA.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1127 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0104/XSD/ModelA/AUXAA.xsd
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0104/XSD/ModelB/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1118 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0104/XSD/ModelB/AUXBB.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3408 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0104/XSD/ModelB/BB.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      316 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0104/test.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      309 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0104/tryload.py
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0108/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      377 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0108/TestPatternRestriction.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      298 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0108/check.py
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      185 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0108/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0114/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1859 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0114/check.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      437 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0114/namespace_other_issue.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      742 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0114/namespace_other_issue.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      288 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0114/namespace_other_issue_support.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      289 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0114/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0119/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      437 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0119/absent.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      365 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0119/base.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     3356 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0119/check.py
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)       78 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0119/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0133/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1415 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0133/poc.xml
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2425 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0133/poc.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      188 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0133/pocSample.py
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      227 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0133/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0169/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      136 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0169/a.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      136 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0169/b.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      181 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0169/base.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      181 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0169/c.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      361 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0169/check.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      632 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0169/logging.cfg
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      215 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0169/root.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      297 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0169/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0183/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      216 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0183/branch1.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      216 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0183/branch2.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      903 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0183/check.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      631 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0183/root.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      341 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0183/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0184/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2540 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0184/check.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1148 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0184/s0add.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      452 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0184/s1core.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      505 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0184/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0186/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    30592 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0186/8_3_2_resource.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      493 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0186/check.py
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      234 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0186/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0193/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1003 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0193/check.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      933 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0193/schema.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      218 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0193/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0196/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2993 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0196/check.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      920 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0196/mix.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1362 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0196/template.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      810 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0196/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0197/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      307 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0197/X.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      320 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0197/s.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      353 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0197/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0198/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1185 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0198/check.py
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      349 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0198/test.sh
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      954 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0198/wsse.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      566 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0198/wsu.xsd
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0199/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      307 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0199/X.xsd
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      662 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0199/check.py
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      215 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0199/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0202/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1553 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0202/check.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1052 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0202/sample.xsd
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      208 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0202/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0230/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      204 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0230/check.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     2214 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0230/sample.xml
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)      613 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/trac/trac-0230/test.sh
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:33:43.324035 PyXB-CTC-1.3.0.dev0/tests/utils/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     5053 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/utils/test-domutils.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    16857 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/utils/test-fac.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     5340 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/utils/test-saxutils.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     4410 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/utils/test-templates.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6228 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/utils/test-unicode.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    32488 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/utils/test-utility.py
--rw-rw-r--   0 niessner  (1000) niessner  (1000)    21323 2023-06-08 16:32:47.000000 PyXB-CTC-1.3.0.dev0/tests/utils/test-xmlre.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.168022 PyXB-CTC-1.3.0rc1/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    11358 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/LICENSE
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1104 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/MANIFEST.in
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1014 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/NOTICE
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2065 2023-06-08 16:47:47.168022 PyXB-CTC-1.3.0rc1/PKG-INFO
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.132022 PyXB-CTC-1.3.0rc1/PyXB_CTC.egg-info/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2065 2023-06-08 16:47:46.000000 PyXB-CTC-1.3.0rc1/PyXB_CTC.egg-info/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    23730 2023-06-08 16:47:47.000000 PyXB-CTC-1.3.0rc1/PyXB_CTC.egg-info/SOURCES.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2023-06-08 16:47:46.000000 PyXB-CTC-1.3.0rc1/PyXB_CTC.egg-info/dependency_links.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        5 2023-06-08 16:47:46.000000 PyXB-CTC-1.3.0rc1/PyXB_CTC.egg-info/top_level.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      570 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/README.md
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      712 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/README.txt.in
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.132022 PyXB-CTC-1.3.0rc1/doc/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       16 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/.gitignore
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.132022 PyXB-CTC-1.3.0rc1/doc/Images/
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)    93415 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/Images/BindingModel.jpg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)    69824 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/Images/CTDValidationExceptions.jpg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)   104867 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/Images/ComponentModel.jpg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)    94495 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/Images/ContentModel.jpg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)   120680 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/Images/FACAutomaton.jpg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)    80210 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/Images/Namespace.jpg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)    97368 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/Images/NamespaceArchive.jpg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)    92897 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/Images/NamespaceCore.jpg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)    72462 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/Images/RuntimeExceptions.jpg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)    83121 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/Images/ScopedDeclarations.jpg
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1532 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/Makefile
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.132022 PyXB-CTC-1.3.0rc1/doc/_templates/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      415 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/_templates/layout.html
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    16442 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/arch_binding.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4680 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/arch_component.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     9727 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/arch_content.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    16096 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/arch_namespaces.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      731 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/architecture.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    31515 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/bundles.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6542 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/conf.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6560 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/conf.py.in
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4798 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/documentation.cfg
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      173 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/eltonly.xhtml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     5506 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/examples.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2101 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/extapi.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4511 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/index.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1336 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/legal.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2783 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/limitations.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     8587 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/maintref.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      147 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/overview.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3479 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/overview_how.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1396 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/overview_what.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1267 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/pyxb.binding.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      851 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/pyxb.namespace.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      438 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/pyxb.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1840 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/pyxb.utils.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      365 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/pyxb.xmlschema.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    18100 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/pyxbgen_cli.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1408 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/related.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    35080 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/releases.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      171 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/userref_index.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    15064 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/userref_pyxbgen.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    12129 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/userref_usebind.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4993 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/userref_validating.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     5694 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/doc/vision.txt
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.128022 PyXB-CTC-1.3.0rc1/examples/
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.132022 PyXB-CTC-1.3.0rc1/examples/cablelabs/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      524 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/cablelabs/README.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      508 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/cablelabs/custom.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2776 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/cablelabs/demo.py
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)       60 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/cablelabs/disabled-test.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1022 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/cablelabs/genbindings.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.132022 PyXB-CTC-1.3.0rc1/examples/content/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      625 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/content/content.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      133 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/content/showcontent.out
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      261 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/content/showcontent.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      133 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/content/test.expected
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      283 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/content/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.132022 PyXB-CTC-1.3.0rc1/examples/customization/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      889 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/customization/README.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2051 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/customization/custom.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3504 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/customization/introspect.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      541 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/customization/normal.py
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      415 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/customization/test.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      420 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/customization/test.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2431 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/customization/tst-introspect.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2575 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/customization/tst-normal.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.132022 PyXB-CTC-1.3.0rc1/examples/dictionary/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      340 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/dictionary/README.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      684 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/dictionary/define.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      392 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/dictionary/genbindings.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      676 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/dictionary/showdict.expected
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1148 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/dictionary/showdict.py
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      247 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/dictionary/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.136022 PyXB-CTC-1.3.0rc1/examples/geocoder/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3484 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/geocoder/GeoCoder.wsdl-patch
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      151 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/geocoder/README.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2471 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/geocoder/client.py
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)       41 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/geocoder/disabled-test.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      388 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/geocoder/genbindings.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.136022 PyXB-CTC-1.3.0rc1/examples/kml/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1047 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/kml/genbindings.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.136022 PyXB-CTC-1.3.0rc1/examples/manual/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1703 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/address.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      340 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/badcontent.expected
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      340 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/badcontent.out
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      232 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/badcontent.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      846 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/badcontent.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      131 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo.expected
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      608 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      131 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo1.out
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      339 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo1.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       31 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo1.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      329 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo2.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       30 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo2.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      329 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo3.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       30 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo3a.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo3b.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       74 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo3c1.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       53 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo3c2.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      169 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4.expected
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       54 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      169 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4a.out
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      264 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4a.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1063 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4a1.expected
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4a1.out
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      238 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4a1.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      169 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4a2.out
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      264 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4a2.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      234 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4b.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       53 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4b.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      463 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4c.out
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      504 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4c.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      853 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4c1.expected
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      853 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4c1.out
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      543 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4c1.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1032 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4c2.expected
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1032 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4c2.out
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      834 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4c2.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1001 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4c3.expected
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1001 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4c3.out
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1020 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/demo4c3.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      154 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/nsaddress.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2083 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/po.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      844 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/po1.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2083 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/po1.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      926 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/po2.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1705 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/po2.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      844 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/po3.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1772 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/po3.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      812 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/po4.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1900 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/po4.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     2221 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/manual/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.136022 PyXB-CTC-1.3.0rc1/examples/ndfd/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      768 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/ndfd/README.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2463 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/ndfd/forecast.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1033 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/ndfd/genbindings.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     7119 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/ndfd/latlon.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       23 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/ndfd/ndfd.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2976 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/ndfd/showreq.expected
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2083 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/ndfd/showreq.py
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      512 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/ndfd/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.136022 PyXB-CTC-1.3.0rc1/examples/tmsxtvd/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       66 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/tmsxtvd/README.md
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)       39 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/tmsxtvd/disabled-test.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2808 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/tmsxtvd/dumpsample.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      379 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/tmsxtvd/genbindings.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.136022 PyXB-CTC-1.3.0rc1/examples/ucum/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      219 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/ucum/README.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1323 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/ucum/showunits.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    10479 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/ucum/test.expected
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      356 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/ucum/test.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     5365 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/ucum/ucum-essence.xsd
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.136022 PyXB-CTC-1.3.0rc1/examples/unicode_jp/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3410 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/unicode_jp/README.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2100 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/unicode_jp/check.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.136022 PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.136022 PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/euc-jp/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1863 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/euc-jp/FG-GML-13-RailCL25000-20080331-0001.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    29042 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/euc-jp/FGD_GMLSchema.xsd
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.136022 PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/iso-2022-jp/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1898 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/iso-2022-jp/FG-GML-13-RailCL25000-20080331-0001.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    31051 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/iso-2022-jp/FGD_GMLSchema.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/readme.txt
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.140022 PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/shift_jis/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1935 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/shift_jis/FG-GML-13-RailCL25000-20080331-0001.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    29854 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/shift_jis/FGD_GMLSchema.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      673 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/shift_jis/readme.txt
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.140022 PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/utf-8/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1902 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/utf-8/FG-GML-13-RailCL25000-20080331-0001.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    30642 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/utf-8/FGD_GMLSchema.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     2362 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/unicode_jp/pyxbgen_jp
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     1200 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/unicode_jp/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.140022 PyXB-CTC-1.3.0rc1/examples/weather/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      549 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/weather/README.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1622 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/weather/client.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      845 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/weather/client_get.py
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/weather/disabled-test.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      299 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/weather/genbindings.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.140022 PyXB-CTC-1.3.0rc1/examples/xhtml/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      553 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/xhtml/README.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      383 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/xhtml/expout.xhtml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      985 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/xhtml/generate.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      359 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/xhtml/rewrite.py
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      731 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/xhtml/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.140022 PyXB-CTC-1.3.0rc1/examples/xsdprimer/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      680 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/xsdprimer/README.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1738 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/xsdprimer/address.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      201 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/xsdprimer/demo.expected
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      648 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/xsdprimer/demo.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      138 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/xsdprimer/genbindings.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1858 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/xsdprimer/ip.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      431 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/xsdprimer/ipo.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1068 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/xsdprimer/ipo.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1925 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/xsdprimer/ipo.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      683 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/xsdprimer/saxdemo.py
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      240 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/examples/xsdprimer/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.140022 PyXB-CTC-1.3.0rc1/maintainer/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4092 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/maintainer/analysis-2111.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     5619 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/maintainer/buildUnicode.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2541 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/maintainer/bundlesupport.sh
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      306 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/maintainer/genall
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      867 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/maintainer/genbundles
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     5965 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/maintainer/gendoc
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      460 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/maintainer/genpd.sh
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      877 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/maintainer/getw3c.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      180 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/maintainer/howto-release.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      644 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/maintainer/logging.cfg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      464 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/maintainer/testall
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      180 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/maintainer/usepyxb.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.140022 PyXB-CTC-1.3.0rc1/pyxb/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    16409 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/__init__.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    16409 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/__init__.py.in
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.140022 PyXB-CTC-1.3.0rc1/pyxb/binding/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      398 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/binding/__init__.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)   119990 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/binding/basis.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    51781 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/binding/content.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    52599 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/binding/datatypes.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    53439 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/binding/facets.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)   132778 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/binding/generate.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    18006 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/binding/saxer.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3079 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/binding/xml_.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.140022 PyXB-CTC-1.3.0rc1/pyxb/bundles/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       14 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/.gitignore
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1037 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/README
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       65 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/__init__.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.140022 PyXB-CTC-1.3.0rc1/pyxb/bundles/common/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       90 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/common/__init__.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.140022 PyXB-CTC-1.3.0rc1/pyxb/bundles/common/scripts/
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      887 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/common/scripts/genbind
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1091 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/common/xhtml1.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/common/xlink.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/common/xsd_hfp.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.140022 PyXB-CTC-1.3.0rc1/pyxb/bundles/dc/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/dc/__init__.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       37 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/dc/dc.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/dc/dcmitype.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       42 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/dc/dcterms.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.140022 PyXB-CTC-1.3.0rc1/pyxb/bundles/dc/scripts/
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      829 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/dc/scripts/genbind
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.140022 PyXB-CTC-1.3.0rc1/pyxb/bundles/ecma376/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       25 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/ecma376/.gitignore
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/ecma376/__init__.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.140022 PyXB-CTC-1.3.0rc1/pyxb/bundles/ecma376/scripts/
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     4087 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/ecma376/scripts/genbind
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.144022 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1291 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/README.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/__init__.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/_ogc.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/_sam.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       45 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/_sams.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/atom.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.144022 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/citygml/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/citygml/__init__.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       58 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/citygml/appearance.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       52 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/citygml/base.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       56 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/citygml/building.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       61 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/citygml/cityFurniture.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       63 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/citygml/cityObjectGroup.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       56 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/citygml/generics.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       55 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/citygml/landUse.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       54 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/citygml/relief.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       63 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/citygml/texturedSurface.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/citygml/transportation.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       58 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/citygml/vegetation.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       57 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/citygml/waterBody.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       49 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/csw_2_0_2.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/csw_dc.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/csw_dct.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.144022 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/examples/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       10 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/examples/.gitignore
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      614 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/examples/check_oseo.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      688 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/examples/check_sos.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      580 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/examples/check_wps.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      172 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/examples/demo.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      686 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/examples/gmlapp.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     1307 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/examples/test.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1235 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/examples/testgml.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/fes_2_0.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/filter.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/gml.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/gml_3_2.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.144022 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/gml_3_3/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/gml_3_3/__init__.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       50 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/gml_3_3/ce.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       51 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/gml_3_3/exr.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       50 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/gml_3_3/lr.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       51 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/gml_3_3/lro.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       52 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/gml_3_3/lrov.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       52 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/gml_3_3/lrtr.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       53 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/gml_3_3/rgrid.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       51 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/gml_3_3/tin.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       51 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/gml_3_3/xbt.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       45 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/gmlsf.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       50 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/ic_ism_2_1.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.144022 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/iso19139/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/iso19139/__init__.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.144022 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/iso19139/v20070417/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/iso19139/v20070417/__init__.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/iso19139/v20070417/gco.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/iso19139/v20070417/gmd.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/iso19139/v20070417/gmx.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/iso19139/v20070417/gsr.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/iso19139/v20070417/gss.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/iso19139/v20070417/gts.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.144022 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/misc/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/misc/__init__.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       48 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/misc/xAL.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       51 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/misc/xlinks.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       48 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/ogckml22.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/om_1_0.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/om_2_0.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       72 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/oseo_1_0.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/ows.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/ows_1_1.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/ows_2_0.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       52 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/sampling_1_0.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.144022 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/scripts/
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6370 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/scripts/genbind
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       54 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/sensorML_1_0_1.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/smil20.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       50 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/smil20lang.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/sos_1_0.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/sos_2_0.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       49 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/swe_1_0_0.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       49 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/swe_1_0_1.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/swe_2_0.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       48 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/swes_2_0.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/tml.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/waterml.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/wcs_1_1.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/wfs.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       73 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/wps_1_0_0.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.144022 PyXB-CTC-1.3.0rc1/pyxb/bundles/reqif/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       67 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/reqif/ReqIF.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/reqif/__init__.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       68 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/reqif/_xh11d.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       68 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/reqif/driver.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.144022 PyXB-CTC-1.3.0rc1/pyxb/bundles/reqif/examples/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      209 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/reqif/examples/process.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       66 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/reqif/examples/test.expected
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      479 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/reqif/examples/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.144022 PyXB-CTC-1.3.0rc1/pyxb/bundles/reqif/scripts/
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     3007 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/reqif/scripts/genbind
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.144022 PyXB-CTC-1.3.0rc1/pyxb/bundles/saml20/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/saml20/__init__.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       48 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/saml20/assertion.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       42 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/saml20/dce.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       42 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/saml20/ecp.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/saml20/metadata.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/saml20/protocol.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.144022 PyXB-CTC-1.3.0rc1/pyxb/bundles/saml20/scripts/
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     1000 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/saml20/scripts/genbind
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/saml20/x500.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/saml20/xacml.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.148022 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/__init__.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/bpws.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       42 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/ds.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      679 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/httpbind.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       48 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/mimebind.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       70 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/sawsdl.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.148022 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/scripts/
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     1927 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/scripts/genbind
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/soap11.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/soap12.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      926 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/soapbind11.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      997 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/soapbind12.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/soapenc.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       45 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/whttp.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wsa.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wsam.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       46 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wscoor.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    11735 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wsdl11.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      211 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wsdl20.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       45 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wsdli.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       45 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wsdlx.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wsnt.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       45 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wsoap.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wsp.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       49 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wsp200607.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wsrf_bf.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       47 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wsrf_br.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wsrm.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wsse.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       45 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wstop.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       43 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wsu.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       44 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/xenc.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    44301 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/exceptions_.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.148022 PyXB-CTC-1.3.0rc1/pyxb/namespace/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    45378 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/namespace/__init__.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    42053 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/namespace/archive.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    13985 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/namespace/builtin.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    37710 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/namespace/resolution.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3037 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/namespace/utility.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.148022 PyXB-CTC-1.3.0rc1/pyxb/utils/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       79 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/utils/__init__.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3595 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/utils/activestate.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    26473 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/utils/domutils.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    75560 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/utils/fac.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    10706 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/utils/saxdom.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    22408 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/utils/saxutils.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    30681 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/utils/six.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4046 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/utils/templates.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    22670 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/utils/unicode.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    88512 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/utils/unicode_data.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    48675 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/utils/utility.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    12909 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/utils/xmlre.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.148022 PyXB-CTC-1.3.0rc1/pyxb/xmlschema/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      518 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/xmlschema/__init__.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)   228632 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/pyxb/xmlschema/structures.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.148022 PyXB-CTC-1.3.0rc1/scripts/
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     1516 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/scripts/pyxbdump
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     2670 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/scripts/pyxbgen
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     1892 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/scripts/pyxbwsdl
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2023-06-08 16:47:47.168022 PyXB-CTC-1.3.0rc1/setup.cfg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)    10720 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/setup.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.148022 PyXB-CTC-1.3.0rc1/tests/
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.148022 PyXB-CTC-1.3.0rc1/tests/bindings/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    14753 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/bindings/test-constraints.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.148022 PyXB-CTC-1.3.0rc1/tests/bugs/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4068 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/bugs/test-200907231705.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2065 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/bugs/test-200907231924.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1146 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/bugs/test-200907251353.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2351 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/bugs/test-200907261730.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1765 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/bugs/test-200908021351.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1624 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/bugs/test-200908041708.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3859 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/bugs/test-200908111918.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2260 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/bugs/test-200908161024.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      693 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/bugs/test-200908181430.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1252 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/bugs/test-200908231005.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2480 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/bugs/test-200908271556.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.128022 PyXB-CTC-1.3.0rc1/tests/complex/
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.148022 PyXB-CTC-1.3.0rc1/tests/complex/nsaugment/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      446 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsaugment/app.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      333 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsaugment/common.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      330 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsaugment/common4app.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      921 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsaugment/test.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1069 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsaugment/tst-app.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      486 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsaugment/tst-common.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.148022 PyXB-CTC-1.3.0rc1/tests/complex/nsdep/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      500 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsdep/a_b.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      465 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsdep/a_c.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      473 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsdep/a_x.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      499 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsdep/b_b.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      570 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsdep/b_c.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      499 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsdep/c_b.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      592 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsdep/c_c.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      869 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsdep/d_c.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      348 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsdep/shared.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      296 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsdep/test.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      740 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsdep/tst-a.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1528 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsdep/tst-b.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.152022 PyXB-CTC-1.3.0rc1/tests/complex/nsext/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       62 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsext/README
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      397 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsext/app.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      332 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsext/base.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      508 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsext/extend.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     1074 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsext/test.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      848 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsext/tst-app.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      485 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsext/tst-base.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      672 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/complex/nsext/tst-extend.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.152022 PyXB-CTC-1.3.0rc1/tests/datatypes/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      799 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-ENTITIES.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      787 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-ENTITY.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      775 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-ID.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      784 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-IDREF.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      789 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-IDREFS.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4944 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-IntegerTypes.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      787 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-NCName.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      994 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-NMTOKEN.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1090 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-NMTOKENS.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      799 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-Name.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1742 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-QName.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      705 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-anyType.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3252 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-base64Binary.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      906 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-boolean.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2780 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-date.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4183 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-dateTime.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3866 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-decimal.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      351 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-double.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     5228 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-duration.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      350 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-float.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1703 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-gDay.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1720 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-gMonth.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2534 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-gMonthDay.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1582 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-gYear.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2478 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-gYearMonth.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1752 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-hexBinary.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2109 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-integer.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      668 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-language.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      959 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-normalizedString.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      351 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-string.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2509 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-time.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1254 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/test-token.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      356 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/totest-NOTATION.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      366 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/totest-anySimpleType.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      352 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/datatypes/totest-anyURI.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.152022 PyXB-CTC-1.3.0rc1/tests/documents/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       76 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/documents/qattr1.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      111 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/documents/qattr2.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      146 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/documents/qattr3.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       92 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/documents/substgroup-001.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       90 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/documents/substgroup-002.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      138 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/documents/substgroup-003.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      190 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/documents/test-empty-cstd-001.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      179 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/documents/test-empty-cstd-002.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      355 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/documents/test-mg-choice-001.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       85 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/documents/test-mg-choice-002.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       85 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/documents/test-mg-choice-003.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      112 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/documents/test-namespace-uu-001.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      127 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/documents/test-namespace-uu-002.xml
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.152022 PyXB-CTC-1.3.0rc1/tests/documents/union/
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      325 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/documents/union/test-union-001.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4445 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/documents/wsdl-001.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2214 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/documents/wsdl-002.xml
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.152022 PyXB-CTC-1.3.0rc1/tests/drivers/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6863 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-ctd-attr.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4287 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-ctd-extension.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1997 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-ctd-simple.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1224 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-deconflict.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1328 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-empty-cstd.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     5698 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-enumeration.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6638 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-external.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1197 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-facets.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      533 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-generatorGetCommandLineArgs.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1046 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-include-aaq.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      785 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-include-aau.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      600 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-include-ad.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1094 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-include-daq.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1566 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-include-dau.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      601 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-include-dcu.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1094 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-include-ddq.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1424 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-include-ddu.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     7480 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-mg-all.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     7945 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-mg-choice.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     8680 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-mg-sequence.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2257 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-namespace-uu.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     5414 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-particle.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     5975 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-po1.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3606 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-properties.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1384 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-properties2.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3051 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-recursive.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      735 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-simplerange.py
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      477 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-stored.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4159 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-substgroup.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2343 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-time.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1032 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-typeinf.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4878 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-union.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     9927 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-wildcard.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     9790 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-xsi-nil.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4325 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/test-xsi-type.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1509 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/drivers/tst-stored.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.152022 PyXB-CTC-1.3.0rc1/tests/pyxb/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1574 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/pyxb/test-cdata.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6163 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/pyxb/test-namespace.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      739 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/pyxb/test-reserved.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.156022 PyXB-CTC-1.3.0rc1/tests/schemas/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      432 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/absentns.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      854 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/alt-po1.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      655 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/anyType.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      390 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/blockfinal.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      722 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/components.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2813 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/enumerations.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      603 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/incl-absent.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      666 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/incl-ad.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      604 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/incl-dau.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      676 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/incl-dcu.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      668 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/incl-ddq.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      668 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/incl-ddu.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      662 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/incl-declared2.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     1169 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/nested-groups.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1735 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/particle.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      848 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/po1.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      779 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/qattr.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2087 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/shared-types.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      709 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/substgroup.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      446 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-ambiguous.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      520 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-collision.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2932 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-ctd-attr.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2081 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-ctd-extension.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1490 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-ctd-simple.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      466 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-deconflict.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      669 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-empty-cstd.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1763 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-external.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      489 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-facets.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      397 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-include-aaq.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      366 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-include-aau.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      435 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-include-ad.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      470 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-include-daq.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      489 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-include-dau.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      542 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-include-dcu.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      470 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-include-ddq.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      489 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-include-ddu.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1069 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-mg-all.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1265 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-mg-choice.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      715 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-mg-sequence.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      622 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-namespace-uu.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1128 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-recursive.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      227 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-simplerange.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2013 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-typeinf.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     2462 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-union.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      666 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/test-wildcard.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      926 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/time.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      619 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/validatable.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      956 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/xsi-nil.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2597 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/schemas/xsi-type.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1628 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/support.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.160022 PyXB-CTC-1.3.0rc1/tests/trac/
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.160022 PyXB-CTC-1.3.0rc1/tests/trac/issue-0048/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      376 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/issue-0048/check.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      383 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/issue-0048/profile-base.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      675 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/issue-0048/profile.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)       75 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/issue-0048/test.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1706 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0006.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2309 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0007.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2916 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0013.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2357 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0014.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1537 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0015.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1242 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0019.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1740 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0022.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1252 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0027.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1019 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0031.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1984 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0032.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      877 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0043.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1744 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0047.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1822 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0051.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1121 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0066.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1541 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0069.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2199 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0071.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1700 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0073.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2578 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0078.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2473 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0079.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2173 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0092.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2497 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0094.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1758 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0021.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1550 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0023.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1488 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0023b.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1297 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0023c.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     7270 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0027.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2681 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0027b.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2512 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0027c.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1463 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0029.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4227 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0032.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1530 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0033a.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2512 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0034.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2629 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0034b.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2446 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0036.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3757 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0037.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2719 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0038.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4008 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0039.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2858 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0040.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1240 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0045.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1096 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0046.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4173 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0047.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1422 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0048.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1365 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0051.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1816 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0052.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2222 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0053.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1970 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0056.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4582 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0057.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1181 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0058.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    15006 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0060.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4003 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0061.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3818 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0069.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     7018 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0071.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1996 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0074.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3083 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0075.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1202 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0076.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1796 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0079.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1914 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0087.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1508 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0088.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2957 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0089.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4794 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0091.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      681 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0093.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3571 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0094.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4219 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0099.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1895 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0099a.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2213 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0100.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1467 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0110.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1873 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0111.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2344 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0112.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      834 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0116.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2151 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0117.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      768 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0121.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2629 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0122.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2272 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0123.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1630 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0126.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4064 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0131.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      501 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0132.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1904 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0136.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2366 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0137.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      447 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0138.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6523 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0139.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2116 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0141.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      967 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0148.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6656 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0153.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1737 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0154.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2713 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0155.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1124 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0156a.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1558 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0163.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1992 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0172.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1982 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0175.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1453 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0179.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1998 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0181.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1502 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0182.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1933 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0184.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2459 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0189.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2294 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0190.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1292 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0191.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1286 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0194.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1999 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0195.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2647 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0200.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1172 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0201.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1640 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0203.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1628 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0204.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1251 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0206.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      880 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0207.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1243 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0208.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     7383 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0211.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1805 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0212.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1737 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0213.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1522 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0216.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1347 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0218.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2022 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0219.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3805 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0221.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2146 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0231.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2142 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0232.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.160022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0026/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3119 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0026/check-binding.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    45154 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0026/check-validation.py
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      291 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0026/test.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6244 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0026/trac26.xsd
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.160022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0033/
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      114 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0033/test.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1731 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0033/tread.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0043/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      579 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0043/a.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      581 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0043/b.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      178 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0043/test.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      638 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0043/tst-1.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      598 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0043/tst-2.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0065/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      778 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0065/TestSchema.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     2299 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0065/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0072/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      149 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0072/a.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      149 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0072/b.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      404 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0072/xtest.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0073/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      365 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0073/base.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      486 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0073/check.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      598 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0073/profile.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      186 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0073/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0080/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2528 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0080/check.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1700 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0080/multipleRestriction.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)       57 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0080/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0084/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      503 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0084/example.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      191 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0084/test.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      149 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0084/tryit.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0088/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      433 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0088/example.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      180 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0088/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0089/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       15 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0089/bad1.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       17 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0089/bad2.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       23 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0089/bad3.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      892 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0089/example.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       15 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0089/good1.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       17 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0089/good2.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       23 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0089/good3.xml
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      505 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0089/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0092/
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      528 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0092/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0104/
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.128022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0104/XSD/
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0104/XSD/ModelA/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3336 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0104/XSD/ModelA/AA.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1127 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0104/XSD/ModelA/AUXAA.xsd
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0104/XSD/ModelB/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1118 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0104/XSD/ModelB/AUXBB.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3408 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0104/XSD/ModelB/BB.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      316 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0104/test.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      309 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0104/tryload.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0108/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      377 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0108/TestPatternRestriction.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      298 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0108/check.py
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      185 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0108/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0114/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1859 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0114/check.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      437 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0114/namespace_other_issue.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      742 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0114/namespace_other_issue.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      288 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0114/namespace_other_issue_support.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      289 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0114/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0119/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      437 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0119/absent.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      365 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0119/base.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     3356 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0119/check.py
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)       78 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0119/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0133/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1415 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0133/poc.xml
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2425 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0133/poc.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      188 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0133/pocSample.py
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      227 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0133/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0169/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      136 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0169/a.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      136 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0169/b.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      181 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0169/base.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      181 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0169/c.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      361 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0169/check.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      632 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0169/logging.cfg
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      215 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0169/root.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      297 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0169/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0183/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      216 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0183/branch1.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      216 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0183/branch2.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      903 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0183/check.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      631 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0183/root.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      341 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0183/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0184/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2540 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0184/check.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1148 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0184/s0add.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      452 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0184/s1core.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      505 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0184/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0186/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    30592 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0186/8_3_2_resource.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      493 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0186/check.py
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      234 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0186/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0193/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1003 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0193/check.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      933 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0193/schema.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      218 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0193/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0196/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2993 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0196/check.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      920 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0196/mix.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1362 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0196/template.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      810 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0196/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0197/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      307 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0197/X.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      320 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0197/s.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      353 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0197/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0198/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1185 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0198/check.py
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      349 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0198/test.sh
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      954 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0198/wsse.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      566 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0198/wsu.xsd
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0199/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      307 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0199/X.xsd
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      662 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0199/check.py
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      215 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0199/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0202/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1553 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0202/check.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1052 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0202/sample.xsd
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      208 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0202/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.164022 PyXB-CTC-1.3.0rc1/tests/trac/trac-0230/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      204 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0230/check.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     2214 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0230/sample.xml
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)      613 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/trac/trac-0230/test.sh
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-06-08 16:47:47.168022 PyXB-CTC-1.3.0rc1/tests/utils/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     5053 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/utils/test-domutils.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    16857 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/utils/test-fac.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     5340 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/utils/test-saxutils.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     4410 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/utils/test-templates.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6228 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/utils/test-unicode.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    32488 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/utils/test-utility.py
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)    21323 2023-06-08 16:45:56.000000 PyXB-CTC-1.3.0rc1/tests/utils/test-xmlre.py
```

### Comparing `PyXB-CTC-1.3.0.dev0/LICENSE` & `PyXB-CTC-1.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/MANIFEST.in` & `PyXB-CTC-1.3.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/NOTICE` & `PyXB-CTC-1.3.0rc1/NOTICE`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/PKG-INFO` & `PyXB-CTC-1.3.0rc1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyXB-CTC
-Version: 1.3.0.dev0
+Version: 1.3.0rc1
 Summary: PyXB ("pixbee") is a pure Python package that generates Python source code for classes that correspond to data structures defined by XMLSchema.
 Home-page: https://github.com/al-niessner/pyxb
 Author: Peter A. Bigot forked by Al Niessner
 Author-email: Via.Repo@github.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,36 +14,36 @@
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Programming Language :: Python :: 3.10
 Provides: PyXB
 License-File: LICENSE
 License-File: NOTICE
 
 PyXB is a pure `Python <http://www.python.org>`_ package that generates
-Python code for classes that correspond to data structures defined by
-`XMLSchema <http://www.w3.org/XML/Schema>`_.  In concept it is similar to
-`JAXB <http://en.wikipedia.org/wiki/JAXB>`_ for Java and `CodeSynthesis XSD
-<http://www.codesynthesis.com/products/xsd/>`_ for C++.
-
-The major goals of PyXB are:
-
-* Provide a generated Python interface that is "Pythonic", meaning similar
-  to one that would have been hand-written:
-
-  + Attributes and elements are Python properties, with name conflicts
-    resolved in favor of elements
-  + Elements with maxOccurs larger than 1 are stored as Python lists
-  + Bindings for type extensions inherit from the binding for the base type
-  + Enumeration constraints are exposed as class (constant) variables
-
-* Support bi-directional conversion (document to Python and back)
-
-* Allow easy customization of the generated bindings to provide
-  functionality along with content
-
-* Support all XMLSchema features that are in common use, including:
-
-  + complex content models (nested all/choice/sequence)
-  + cross-namespace dependencies
-  + include and import directives
-  + constraints on simple types
-
+    Python code for classes that correspond to data structures defined by
+    `XMLSchema <http://www.w3.org/XML/Schema>`_.  In concept it is similar to
+    `JAXB <http://en.wikipedia.org/wiki/JAXB>`_ for Java and `CodeSynthesis XSD
+    <http://www.codesynthesis.com/products/xsd/>`_ for C++.
+
+    The major goals of PyXB are:
+
+    * Provide a generated Python interface that is "Pythonic", meaning similar
+      to one that would have been hand-written:
+
+      + Attributes and elements are Python properties, with name conflicts
+        resolved in favor of elements
+      + Elements with maxOccurs larger than 1 are stored as Python lists
+      + Bindings for type extensions inherit from the binding for the base type
+      + Enumeration constraints are exposed as class (constant) variables
+
+    * Support bi-directional conversion (document to Python and back)
+
+    * Allow easy customization of the generated bindings to provide
+      functionality along with content
+
+    * Support all XMLSchema features that are in common use, including:
+
+      + complex content models (nested all/choice/sequence)
+      + cross-namespace dependencies
+      + include and import directives
+      + constraints on simple types
+
```

### Comparing `PyXB-CTC-1.3.0.dev0/PyXB_CTC.egg-info/PKG-INFO` & `PyXB-CTC-1.3.0rc1/PyXB_CTC.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyXB-CTC
-Version: 1.3.0.dev0
+Version: 1.3.0rc1
 Summary: PyXB ("pixbee") is a pure Python package that generates Python source code for classes that correspond to data structures defined by XMLSchema.
 Home-page: https://github.com/al-niessner/pyxb
 Author: Peter A. Bigot forked by Al Niessner
 Author-email: Via.Repo@github.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,36 +14,36 @@
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Programming Language :: Python :: 3.10
 Provides: PyXB
 License-File: LICENSE
 License-File: NOTICE
 
 PyXB is a pure `Python <http://www.python.org>`_ package that generates
-Python code for classes that correspond to data structures defined by
-`XMLSchema <http://www.w3.org/XML/Schema>`_.  In concept it is similar to
-`JAXB <http://en.wikipedia.org/wiki/JAXB>`_ for Java and `CodeSynthesis XSD
-<http://www.codesynthesis.com/products/xsd/>`_ for C++.
-
-The major goals of PyXB are:
-
-* Provide a generated Python interface that is "Pythonic", meaning similar
-  to one that would have been hand-written:
-
-  + Attributes and elements are Python properties, with name conflicts
-    resolved in favor of elements
-  + Elements with maxOccurs larger than 1 are stored as Python lists
-  + Bindings for type extensions inherit from the binding for the base type
-  + Enumeration constraints are exposed as class (constant) variables
-
-* Support bi-directional conversion (document to Python and back)
-
-* Allow easy customization of the generated bindings to provide
-  functionality along with content
-
-* Support all XMLSchema features that are in common use, including:
-
-  + complex content models (nested all/choice/sequence)
-  + cross-namespace dependencies
-  + include and import directives
-  + constraints on simple types
-
+    Python code for classes that correspond to data structures defined by
+    `XMLSchema <http://www.w3.org/XML/Schema>`_.  In concept it is similar to
+    `JAXB <http://en.wikipedia.org/wiki/JAXB>`_ for Java and `CodeSynthesis XSD
+    <http://www.codesynthesis.com/products/xsd/>`_ for C++.
+
+    The major goals of PyXB are:
+
+    * Provide a generated Python interface that is "Pythonic", meaning similar
+      to one that would have been hand-written:
+
+      + Attributes and elements are Python properties, with name conflicts
+        resolved in favor of elements
+      + Elements with maxOccurs larger than 1 are stored as Python lists
+      + Bindings for type extensions inherit from the binding for the base type
+      + Enumeration constraints are exposed as class (constant) variables
+
+    * Support bi-directional conversion (document to Python and back)
+
+    * Allow easy customization of the generated bindings to provide
+      functionality along with content
+
+    * Support all XMLSchema features that are in common use, including:
+
+      + complex content models (nested all/choice/sequence)
+      + cross-namespace dependencies
+      + include and import directives
+      + constraints on simple types
+
```

### Comparing `PyXB-CTC-1.3.0.dev0/PyXB_CTC.egg-info/SOURCES.txt` & `PyXB-CTC-1.3.0rc1/PyXB_CTC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/README.md` & `PyXB-CTC-1.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/README.txt.in` & `PyXB-CTC-1.3.0rc1/README.txt.in`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/Images/BindingModel.jpg` & `PyXB-CTC-1.3.0rc1/doc/Images/BindingModel.jpg`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/Images/CTDValidationExceptions.jpg` & `PyXB-CTC-1.3.0rc1/doc/Images/CTDValidationExceptions.jpg`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/Images/ComponentModel.jpg` & `PyXB-CTC-1.3.0rc1/doc/Images/ComponentModel.jpg`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/Images/ContentModel.jpg` & `PyXB-CTC-1.3.0rc1/doc/Images/ContentModel.jpg`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/Images/FACAutomaton.jpg` & `PyXB-CTC-1.3.0rc1/doc/Images/FACAutomaton.jpg`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/Images/Namespace.jpg` & `PyXB-CTC-1.3.0rc1/doc/Images/Namespace.jpg`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/Images/NamespaceArchive.jpg` & `PyXB-CTC-1.3.0rc1/doc/Images/NamespaceArchive.jpg`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/Images/NamespaceCore.jpg` & `PyXB-CTC-1.3.0rc1/doc/Images/NamespaceCore.jpg`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/Images/RuntimeExceptions.jpg` & `PyXB-CTC-1.3.0rc1/doc/Images/RuntimeExceptions.jpg`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/Images/ScopedDeclarations.jpg` & `PyXB-CTC-1.3.0rc1/doc/Images/ScopedDeclarations.jpg`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/Makefile` & `PyXB-CTC-1.3.0rc1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/arch_binding.txt` & `PyXB-CTC-1.3.0rc1/doc/arch_binding.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/arch_component.txt` & `PyXB-CTC-1.3.0rc1/doc/arch_component.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/arch_content.txt` & `PyXB-CTC-1.3.0rc1/doc/arch_content.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/arch_namespaces.txt` & `PyXB-CTC-1.3.0rc1/doc/arch_namespaces.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/architecture.txt` & `PyXB-CTC-1.3.0rc1/doc/architecture.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/bundles.txt` & `PyXB-CTC-1.3.0rc1/doc/bundles.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/conf.py` & `PyXB-CTC-1.3.0rc1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/conf.py.in` & `PyXB-CTC-1.3.0rc1/doc/conf.py.in`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/documentation.cfg` & `PyXB-CTC-1.3.0rc1/doc/documentation.cfg`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/examples.txt` & `PyXB-CTC-1.3.0rc1/doc/examples.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/extapi.py` & `PyXB-CTC-1.3.0rc1/doc/extapi.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/index.txt` & `PyXB-CTC-1.3.0rc1/doc/index.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/legal.txt` & `PyXB-CTC-1.3.0rc1/doc/legal.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/limitations.txt` & `PyXB-CTC-1.3.0rc1/doc/limitations.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/maintref.txt` & `PyXB-CTC-1.3.0rc1/doc/maintref.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/overview_how.txt` & `PyXB-CTC-1.3.0rc1/doc/overview_how.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/overview_what.txt` & `PyXB-CTC-1.3.0rc1/doc/overview_what.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/pyxb.binding.txt` & `PyXB-CTC-1.3.0rc1/doc/pyxb.binding.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/pyxb.namespace.txt` & `PyXB-CTC-1.3.0rc1/doc/pyxb.namespace.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/pyxb.utils.txt` & `PyXB-CTC-1.3.0rc1/doc/pyxb.utils.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/pyxbgen_cli.txt` & `PyXB-CTC-1.3.0rc1/doc/pyxbgen_cli.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/related.txt` & `PyXB-CTC-1.3.0rc1/doc/related.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/releases.txt` & `PyXB-CTC-1.3.0rc1/doc/releases.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/userref_pyxbgen.txt` & `PyXB-CTC-1.3.0rc1/doc/userref_pyxbgen.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/userref_usebind.txt` & `PyXB-CTC-1.3.0rc1/doc/userref_usebind.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/userref_validating.txt` & `PyXB-CTC-1.3.0rc1/doc/userref_validating.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/doc/vision.txt` & `PyXB-CTC-1.3.0rc1/doc/vision.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/cablelabs/README.txt` & `PyXB-CTC-1.3.0rc1/examples/cablelabs/README.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/cablelabs/demo.py` & `PyXB-CTC-1.3.0rc1/examples/cablelabs/demo.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/cablelabs/genbindings.sh` & `PyXB-CTC-1.3.0rc1/examples/cablelabs/genbindings.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/content/content.xsd` & `PyXB-CTC-1.3.0rc1/examples/content/content.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/customization/README.txt` & `PyXB-CTC-1.3.0rc1/examples/customization/README.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/customization/custom.xsd` & `PyXB-CTC-1.3.0rc1/examples/customization/custom.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/customization/introspect.py` & `PyXB-CTC-1.3.0rc1/examples/customization/introspect.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/customization/normal.py` & `PyXB-CTC-1.3.0rc1/examples/customization/normal.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/customization/tst-introspect.py` & `PyXB-CTC-1.3.0rc1/examples/customization/tst-introspect.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/customization/tst-normal.py` & `PyXB-CTC-1.3.0rc1/examples/customization/tst-normal.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/dictionary/define.py` & `PyXB-CTC-1.3.0rc1/examples/dictionary/define.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/dictionary/showdict.expected` & `PyXB-CTC-1.3.0rc1/examples/dictionary/showdict.expected`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/dictionary/showdict.py` & `PyXB-CTC-1.3.0rc1/examples/dictionary/showdict.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/geocoder/GeoCoder.wsdl-patch` & `PyXB-CTC-1.3.0rc1/examples/geocoder/GeoCoder.wsdl-patch`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/geocoder/client.py` & `PyXB-CTC-1.3.0rc1/examples/geocoder/client.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/kml/genbindings.sh` & `PyXB-CTC-1.3.0rc1/examples/kml/genbindings.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/address.xsd` & `PyXB-CTC-1.3.0rc1/examples/manual/address.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/badcontent.xml` & `PyXB-CTC-1.3.0rc1/examples/manual/badcontent.xml`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/demo.sh` & `PyXB-CTC-1.3.0rc1/examples/manual/demo.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/demo4a1.expected` & `PyXB-CTC-1.3.0rc1/examples/manual/demo4a1.expected`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/demo4c1.expected` & `PyXB-CTC-1.3.0rc1/examples/manual/demo4c1.expected`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/demo4c1.out` & `PyXB-CTC-1.3.0rc1/examples/manual/demo4c1.out`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/demo4c1.py` & `PyXB-CTC-1.3.0rc1/examples/manual/demo4c1.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/demo4c2.expected` & `PyXB-CTC-1.3.0rc1/examples/manual/demo4c2.expected`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/demo4c2.out` & `PyXB-CTC-1.3.0rc1/examples/manual/demo4c2.out`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/demo4c2.py` & `PyXB-CTC-1.3.0rc1/examples/manual/demo4c2.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/demo4c3.expected` & `PyXB-CTC-1.3.0rc1/examples/manual/demo4c3.expected`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/demo4c3.out` & `PyXB-CTC-1.3.0rc1/examples/manual/demo4c3.out`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/demo4c3.py` & `PyXB-CTC-1.3.0rc1/examples/manual/demo4c3.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/po.xsd` & `PyXB-CTC-1.3.0rc1/examples/manual/po.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/po1.xml` & `PyXB-CTC-1.3.0rc1/examples/manual/po1.xml`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/po1.xsd` & `PyXB-CTC-1.3.0rc1/examples/manual/po1.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/po2.xml` & `PyXB-CTC-1.3.0rc1/examples/manual/po2.xml`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/po2.xsd` & `PyXB-CTC-1.3.0rc1/examples/manual/po2.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/po3.xml` & `PyXB-CTC-1.3.0rc1/examples/manual/po3.xml`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/po3.xsd` & `PyXB-CTC-1.3.0rc1/examples/manual/po3.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/po4.xml` & `PyXB-CTC-1.3.0rc1/examples/manual/po4.xml`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/po4.xsd` & `PyXB-CTC-1.3.0rc1/examples/manual/po4.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/manual/test.sh` & `PyXB-CTC-1.3.0rc1/examples/manual/test.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/ndfd/README.txt` & `PyXB-CTC-1.3.0rc1/examples/ndfd/README.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/ndfd/forecast.py` & `PyXB-CTC-1.3.0rc1/examples/ndfd/forecast.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/ndfd/genbindings.sh` & `PyXB-CTC-1.3.0rc1/examples/ndfd/genbindings.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/ndfd/latlon.py` & `PyXB-CTC-1.3.0rc1/examples/ndfd/latlon.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/ndfd/showreq.expected` & `PyXB-CTC-1.3.0rc1/examples/ndfd/showreq.expected`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/ndfd/showreq.py` & `PyXB-CTC-1.3.0rc1/examples/ndfd/showreq.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/ndfd/test.sh` & `PyXB-CTC-1.3.0rc1/examples/ndfd/test.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/tmsxtvd/dumpsample.py` & `PyXB-CTC-1.3.0rc1/examples/tmsxtvd/dumpsample.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/ucum/showunits.py` & `PyXB-CTC-1.3.0rc1/examples/ucum/showunits.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/ucum/test.expected` & `PyXB-CTC-1.3.0rc1/examples/ucum/test.expected`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/ucum/ucum-essence.xsd` & `PyXB-CTC-1.3.0rc1/examples/ucum/ucum-essence.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/unicode_jp/README.txt` & `PyXB-CTC-1.3.0rc1/examples/unicode_jp/README.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/unicode_jp/check.py` & `PyXB-CTC-1.3.0rc1/examples/unicode_jp/check.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/euc-jp/FG-GML-13-RailCL25000-20080331-0001.xml` & `PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/euc-jp/FG-GML-13-RailCL25000-20080331-0001.xml`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/euc-jp/FGD_GMLSchema.xsd` & `PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/euc-jp/FGD_GMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/iso-2022-jp/FG-GML-13-RailCL25000-20080331-0001.xml` & `PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/iso-2022-jp/FG-GML-13-RailCL25000-20080331-0001.xml`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/iso-2022-jp/FGD_GMLSchema.xsd` & `PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/iso-2022-jp/FGD_GMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/shift_jis/FG-GML-13-RailCL25000-20080331-0001.xml` & `PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/shift_jis/FG-GML-13-RailCL25000-20080331-0001.xml`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/shift_jis/FGD_GMLSchema.xsd` & `PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/shift_jis/FGD_GMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/shift_jis/readme.txt` & `PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/shift_jis/readme.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/utf-8/FG-GML-13-RailCL25000-20080331-0001.xml` & `PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/utf-8/FG-GML-13-RailCL25000-20080331-0001.xml`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/unicode_jp/data/utf-8/FGD_GMLSchema.xsd` & `PyXB-CTC-1.3.0rc1/examples/unicode_jp/data/utf-8/FGD_GMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/unicode_jp/pyxbgen_jp` & `PyXB-CTC-1.3.0rc1/examples/unicode_jp/pyxbgen_jp`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/unicode_jp/test.sh` & `PyXB-CTC-1.3.0rc1/examples/unicode_jp/test.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/weather/README.txt` & `PyXB-CTC-1.3.0rc1/examples/weather/README.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/weather/client.py` & `PyXB-CTC-1.3.0rc1/examples/weather/client.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/weather/client_get.py` & `PyXB-CTC-1.3.0rc1/examples/weather/client_get.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/xhtml/README.txt` & `PyXB-CTC-1.3.0rc1/examples/xhtml/README.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/xhtml/generate.py` & `PyXB-CTC-1.3.0rc1/examples/xhtml/generate.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/xhtml/test.sh` & `PyXB-CTC-1.3.0rc1/examples/xhtml/test.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/xsdprimer/README.txt` & `PyXB-CTC-1.3.0rc1/examples/xsdprimer/README.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/xsdprimer/address.xsd` & `PyXB-CTC-1.3.0rc1/examples/xsdprimer/address.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/xsdprimer/demo.py` & `PyXB-CTC-1.3.0rc1/examples/xsdprimer/demo.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/xsdprimer/ip.xsd` & `PyXB-CTC-1.3.0rc1/examples/xsdprimer/ip.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/xsdprimer/ipo.xml` & `PyXB-CTC-1.3.0rc1/examples/xsdprimer/ipo.xml`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/xsdprimer/ipo.xsd` & `PyXB-CTC-1.3.0rc1/examples/xsdprimer/ipo.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/examples/xsdprimer/saxdemo.py` & `PyXB-CTC-1.3.0rc1/examples/xsdprimer/saxdemo.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/maintainer/analysis-2111.txt` & `PyXB-CTC-1.3.0rc1/maintainer/analysis-2111.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/maintainer/buildUnicode.py` & `PyXB-CTC-1.3.0rc1/maintainer/buildUnicode.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/maintainer/bundlesupport.sh` & `PyXB-CTC-1.3.0rc1/maintainer/bundlesupport.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/maintainer/genbundles` & `PyXB-CTC-1.3.0rc1/maintainer/genbundles`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/maintainer/gendoc` & `PyXB-CTC-1.3.0rc1/maintainer/gendoc`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/maintainer/getw3c.sh` & `PyXB-CTC-1.3.0rc1/maintainer/getw3c.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/maintainer/logging.cfg` & `PyXB-CTC-1.3.0rc1/maintainer/logging.cfg`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/__init__.py` & `PyXB-CTC-1.3.0rc1/pyxb/__init__.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/__init__.py.in` & `PyXB-CTC-1.3.0rc1/pyxb/__init__.py.in`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/binding/basis.py` & `PyXB-CTC-1.3.0rc1/pyxb/binding/basis.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/binding/content.py` & `PyXB-CTC-1.3.0rc1/pyxb/binding/content.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/binding/datatypes.py` & `PyXB-CTC-1.3.0rc1/pyxb/binding/datatypes.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/binding/facets.py` & `PyXB-CTC-1.3.0rc1/pyxb/binding/facets.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/binding/generate.py` & `PyXB-CTC-1.3.0rc1/pyxb/binding/generate.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/binding/saxer.py` & `PyXB-CTC-1.3.0rc1/pyxb/binding/saxer.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/binding/xml_.py` & `PyXB-CTC-1.3.0rc1/pyxb/binding/xml_.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/README` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/README`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/common/scripts/genbind` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/common/scripts/genbind`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/common/xhtml1.py` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/common/xhtml1.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/dc/scripts/genbind` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/dc/scripts/genbind`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/ecma376/scripts/genbind` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/ecma376/scripts/genbind`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/README.txt` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/README.txt`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/examples/check_oseo.py` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/examples/check_oseo.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/examples/check_sos.py` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/examples/check_sos.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/examples/check_wps.py` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/examples/check_wps.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/examples/gmlapp.xsd` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/examples/gmlapp.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/examples/test.sh` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/examples/test.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/examples/testgml.py` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/examples/testgml.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/opengis/scripts/genbind` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/opengis/scripts/genbind`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/reqif/scripts/genbind` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/reqif/scripts/genbind`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/saml20/scripts/genbind` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/saml20/scripts/genbind`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/httpbind.py` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/httpbind.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/scripts/genbind` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/scripts/genbind`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/soapbind11.py` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/soapbind11.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/soapbind12.py` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/soapbind12.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/bundles/wssplat/wsdl11.py` & `PyXB-CTC-1.3.0rc1/pyxb/bundles/wssplat/wsdl11.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/exceptions_.py` & `PyXB-CTC-1.3.0rc1/pyxb/exceptions_.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/namespace/__init__.py` & `PyXB-CTC-1.3.0rc1/pyxb/namespace/__init__.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/namespace/archive.py` & `PyXB-CTC-1.3.0rc1/pyxb/namespace/archive.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/namespace/builtin.py` & `PyXB-CTC-1.3.0rc1/pyxb/namespace/builtin.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/namespace/resolution.py` & `PyXB-CTC-1.3.0rc1/pyxb/namespace/resolution.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/namespace/utility.py` & `PyXB-CTC-1.3.0rc1/pyxb/namespace/utility.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/utils/activestate.py` & `PyXB-CTC-1.3.0rc1/pyxb/utils/activestate.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/utils/domutils.py` & `PyXB-CTC-1.3.0rc1/pyxb/utils/domutils.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/utils/fac.py` & `PyXB-CTC-1.3.0rc1/pyxb/utils/fac.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/utils/saxdom.py` & `PyXB-CTC-1.3.0rc1/pyxb/utils/saxdom.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/utils/saxutils.py` & `PyXB-CTC-1.3.0rc1/pyxb/utils/saxutils.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/utils/six.py` & `PyXB-CTC-1.3.0rc1/pyxb/utils/six.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/utils/templates.py` & `PyXB-CTC-1.3.0rc1/pyxb/utils/templates.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/utils/unicode.py` & `PyXB-CTC-1.3.0rc1/pyxb/utils/unicode.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/utils/unicode_data.py` & `PyXB-CTC-1.3.0rc1/pyxb/utils/unicode_data.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/utils/utility.py` & `PyXB-CTC-1.3.0rc1/pyxb/utils/utility.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/utils/xmlre.py` & `PyXB-CTC-1.3.0rc1/pyxb/utils/xmlre.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/xmlschema/__init__.py` & `PyXB-CTC-1.3.0rc1/pyxb/xmlschema/__init__.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/pyxb/xmlschema/structures.py` & `PyXB-CTC-1.3.0rc1/pyxb/xmlschema/structures.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/scripts/pyxbdump` & `PyXB-CTC-1.3.0rc1/scripts/pyxbdump`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/scripts/pyxbgen` & `PyXB-CTC-1.3.0rc1/scripts/pyxbgen`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/scripts/pyxbwsdl` & `PyXB-CTC-1.3.0rc1/scripts/pyxbwsdl`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/setup.py` & `PyXB-CTC-1.3.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from __future__ import print_function
 import sys
 
 # The current version of the system.  Format is #.#.#[-DEV].
-version = '1.3.0-DEV'
+version = '1.3.0-rc1'
 
 # Require Python 3.10 or higher
 if (sys.version_info[:2] < (3, 10)):
     raise ValueError('''PyXB requires:
   Python3 version 3.10 or later
 (You have %s.)''' % (sys.version,))
 
@@ -162,108 +162,109 @@
             verbosity = 2
         elif self.inhibit_output:
             # Don't know how to do this for real
             verbosity = 0
         runner = unittest.TextTestRunner(verbosity=verbosity)
         runner.run(suite)
 
-import glob
-import sys
-import pyxb.utils.utility
-
-packages = [
-        'pyxb', 'pyxb.namespace', 'pyxb.binding', 'pyxb.utils', 'pyxb.xmlschema',
-        "pyxb.bundles"
-        ]
-package_data = {}
-
-init_re = re.compile('^__init__\.py$')
-wxs_re = re.compile('^.*\.wxs$')
-
-setup_path = os.path.dirname(__file__)
-bundle_base = os.path.join(setup_path, 'pyxb', 'bundles')
-possible_bundles = []
-try:
-    possible_bundles.extend(os.listdir(bundle_base))
-except OSError as e:
-    print("Directory %s bundle search failed: %s" % (bundle_base, e))
-for possible_bundle in possible_bundles:
-    bundle_root = os.path.join(bundle_base, possible_bundle)
-    if not os.path.isdir(bundle_root):
-        continue
-    b_packages = []
-    b_data = { }
-    for fp in pyxb.utils.utility.GetMatchingFiles('%s//' % (bundle_root,), init_re):
-        bundle_path = os.path.dirname(os.path.normpath(fp))
-        try:
-            package_relpath = os.path.relpath(bundle_path, setup_path)
-        except AttributeError as e:
-            package_relpath = bundle_path
-            if setup_path and '.' != setup_path:
-                prefix_path = setup_path + os.path.sep
-                if not package_relpath.startswith(prefix_path):
-                    print("Unable to determine relative path from %s to %s installation" % (setup_path, bundle_path))
-                    sys.exit(1)
-                package_relpath = package_relpath[len(prefix_path):]
-        package = package_relpath.replace(os.path.sep, '.')
-        b_packages.append(package)
-        wxs_files = [os.path.basename(_f) for _f in pyxb.utils.utility.GetMatchingFiles(bundle_path, wxs_re) ]
-        if wxs_files:
-            b_data[package] = wxs_files
-    if 0 < len(b_data):
-        print('Found bundle in %s' % (bundle_root,))
-        packages.extend(b_packages)
-        package_data.update(b_data)
-
-setup(name='PyXB-CTC',
-      description = 'PyXB ("pixbee") is a pure Python package that generates Python source code for classes that correspond to data structures defined by XMLSchema.',
-      author='Peter A. Bigot forked by Al Niessner',
-      author_email='Via.Repo@github.com',
-      url='https://github.com/al-niessner/pyxb',
-      # Also change in README.TXT, pyxb/__init__.py, and doc/conf.py
-      version=version,
-      license='Apache License 2.0',
-      long_description='''PyXB is a pure `Python <http://www.python.org>`_ package that generates
-Python code for classes that correspond to data structures defined by
-`XMLSchema <http://www.w3.org/XML/Schema>`_.  In concept it is similar to
-`JAXB <http://en.wikipedia.org/wiki/JAXB>`_ for Java and `CodeSynthesis XSD
-<http://www.codesynthesis.com/products/xsd/>`_ for C++.
-
-The major goals of PyXB are:
-
-* Provide a generated Python interface that is "Pythonic", meaning similar
-  to one that would have been hand-written:
-
-  + Attributes and elements are Python properties, with name conflicts
-    resolved in favor of elements
-  + Elements with maxOccurs larger than 1 are stored as Python lists
-  + Bindings for type extensions inherit from the binding for the base type
-  + Enumeration constraints are exposed as class (constant) variables
-
-* Support bi-directional conversion (document to Python and back)
-
-* Allow easy customization of the generated bindings to provide
-  functionality along with content
-
-* Support all XMLSchema features that are in common use, including:
-
-  + complex content models (nested all/choice/sequence)
-  + cross-namespace dependencies
-  + include and import directives
-  + constraints on simple types
-''',
-      provides=[ 'PyXB' ],
-      packages=packages,
-      package_data=package_data,
-      # I normally keep these in $purelib, but distutils won't tell me where that is.
-      # We don't need them in the installation anyway.
-      #data_files= [ ('pyxb/standard/schemas', glob.glob(os.path.join(*'pyxb/standard/schemas/*.xsd'.split('/'))) ) ],
-      scripts=[ 'scripts/pyxbgen', 'scripts/pyxbwsdl', 'scripts/pyxbdump' ],
-      cmdclass = { 'test' : test,
-                   'update_version' : update_version },
-      classifiers = [ 'Development Status :: 5 - Production/Stable'
-                      , 'Intended Audience :: Developers'
-                      , 'License :: OSI Approved :: Apache Software License'
-                      , 'Topic :: Software Development :: Code Generators'
-                      , 'Topic :: Text Processing :: Markup :: XML'
-                      , 'Programming Language :: Python :: 3.10'
-                      ] )
+if __name__ == '__main__':
+    import glob
+    import sys
+    import pyxb.utils.utility
+
+    packages = [
+            'pyxb', 'pyxb.namespace', 'pyxb.binding', 'pyxb.utils', 'pyxb.xmlschema',
+            "pyxb.bundles"
+            ]
+    package_data = {}
+
+    init_re = re.compile('^__init__\.py$')
+    wxs_re = re.compile('^.*\.wxs$')
+
+    setup_path = os.path.dirname(__file__)
+    bundle_base = os.path.join(setup_path, 'pyxb', 'bundles')
+    possible_bundles = []
+    try:
+        possible_bundles.extend(os.listdir(bundle_base))
+    except OSError as e:
+        print("Directory %s bundle search failed: %s" % (bundle_base, e))
+    for possible_bundle in possible_bundles:
+        bundle_root = os.path.join(bundle_base, possible_bundle)
+        if not os.path.isdir(bundle_root):
+            continue
+        b_packages = []
+        b_data = { }
+        for fp in pyxb.utils.utility.GetMatchingFiles('%s//' % (bundle_root,), init_re):
+            bundle_path = os.path.dirname(os.path.normpath(fp))
+            try:
+                package_relpath = os.path.relpath(bundle_path, setup_path)
+            except AttributeError as e:
+                package_relpath = bundle_path
+                if setup_path and '.' != setup_path:
+                    prefix_path = setup_path + os.path.sep
+                    if not package_relpath.startswith(prefix_path):
+                        print("Unable to determine relative path from %s to %s installation" % (setup_path, bundle_path))
+                        sys.exit(1)
+                    package_relpath = package_relpath[len(prefix_path):]
+            package = package_relpath.replace(os.path.sep, '.')
+            b_packages.append(package)
+            wxs_files = [os.path.basename(_f) for _f in pyxb.utils.utility.GetMatchingFiles(bundle_path, wxs_re) ]
+            if wxs_files:
+                b_data[package] = wxs_files
+        if 0 < len(b_data):
+            print('Found bundle in %s' % (bundle_root,))
+            packages.extend(b_packages)
+            package_data.update(b_data)
+
+    setup(name='PyXB-CTC',
+          description = 'PyXB ("pixbee") is a pure Python package that generates Python source code for classes that correspond to data structures defined by XMLSchema.',
+          author='Peter A. Bigot forked by Al Niessner',
+          author_email='Via.Repo@github.com',
+          url='https://github.com/al-niessner/pyxb',
+          # Also change in README.TXT, pyxb/__init__.py, and doc/conf.py
+          version=version,
+          license='Apache License 2.0',
+          long_description='''PyXB is a pure `Python <http://www.python.org>`_ package that generates
+    Python code for classes that correspond to data structures defined by
+    `XMLSchema <http://www.w3.org/XML/Schema>`_.  In concept it is similar to
+    `JAXB <http://en.wikipedia.org/wiki/JAXB>`_ for Java and `CodeSynthesis XSD
+    <http://www.codesynthesis.com/products/xsd/>`_ for C++.
+
+    The major goals of PyXB are:
+
+    * Provide a generated Python interface that is "Pythonic", meaning similar
+      to one that would have been hand-written:
+
+      + Attributes and elements are Python properties, with name conflicts
+        resolved in favor of elements
+      + Elements with maxOccurs larger than 1 are stored as Python lists
+      + Bindings for type extensions inherit from the binding for the base type
+      + Enumeration constraints are exposed as class (constant) variables
+
+    * Support bi-directional conversion (document to Python and back)
+
+    * Allow easy customization of the generated bindings to provide
+      functionality along with content
+
+    * Support all XMLSchema features that are in common use, including:
+
+      + complex content models (nested all/choice/sequence)
+      + cross-namespace dependencies
+      + include and import directives
+      + constraints on simple types
+    ''',
+          provides=[ 'PyXB' ],
+          packages=packages,
+          package_data=package_data,
+          # I normally keep these in $purelib, but distutils won't tell me where that is.
+          # We don't need them in the installation anyway.
+          #data_files= [ ('pyxb/standard/schemas', glob.glob(os.path.join(*'pyxb/standard/schemas/*.xsd'.split('/'))) ) ],
+          scripts=[ 'scripts/pyxbgen', 'scripts/pyxbwsdl', 'scripts/pyxbdump' ],
+          cmdclass = { 'test' : test,
+                       'update_version' : update_version },
+          classifiers = [ 'Development Status :: 5 - Production/Stable'
+                          , 'Intended Audience :: Developers'
+                          , 'License :: OSI Approved :: Apache Software License'
+                          , 'Topic :: Software Development :: Code Generators'
+                          , 'Topic :: Text Processing :: Markup :: XML'
+                          , 'Programming Language :: Python :: 3.10'
+                          ] )
```

### Comparing `PyXB-CTC-1.3.0.dev0/tests/bindings/test-constraints.py` & `PyXB-CTC-1.3.0rc1/tests/bindings/test-constraints.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/bugs/test-200907231705.py` & `PyXB-CTC-1.3.0rc1/tests/bugs/test-200907231705.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/bugs/test-200907231924.py` & `PyXB-CTC-1.3.0rc1/tests/bugs/test-200907231924.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/bugs/test-200907251353.py` & `PyXB-CTC-1.3.0rc1/tests/bugs/test-200907251353.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/bugs/test-200907261730.py` & `PyXB-CTC-1.3.0rc1/tests/bugs/test-200907261730.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/bugs/test-200908021351.py` & `PyXB-CTC-1.3.0rc1/tests/bugs/test-200908021351.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/bugs/test-200908041708.py` & `PyXB-CTC-1.3.0rc1/tests/bugs/test-200908041708.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/bugs/test-200908111918.py` & `PyXB-CTC-1.3.0rc1/tests/bugs/test-200908111918.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/bugs/test-200908161024.py` & `PyXB-CTC-1.3.0rc1/tests/bugs/test-200908161024.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/bugs/test-200908181430.py` & `PyXB-CTC-1.3.0rc1/tests/bugs/test-200908181430.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/bugs/test-200908231005.py` & `PyXB-CTC-1.3.0rc1/tests/bugs/test-200908231005.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/bugs/test-200908271556.py` & `PyXB-CTC-1.3.0rc1/tests/bugs/test-200908271556.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/complex/nsaugment/test.sh` & `PyXB-CTC-1.3.0rc1/tests/complex/nsaugment/test.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/complex/nsaugment/tst-app.py` & `PyXB-CTC-1.3.0rc1/tests/complex/nsaugment/tst-app.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/b_c.xsd` & `PyXB-CTC-1.3.0rc1/tests/complex/nsdep/b_c.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/c_c.xsd` & `PyXB-CTC-1.3.0rc1/tests/complex/nsdep/c_c.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/d_c.xsd` & `PyXB-CTC-1.3.0rc1/tests/complex/nsdep/d_c.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/tst-a.py` & `PyXB-CTC-1.3.0rc1/tests/complex/nsdep/tst-a.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/complex/nsdep/tst-b.py` & `PyXB-CTC-1.3.0rc1/tests/complex/nsdep/tst-b.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/complex/nsext/test.sh` & `PyXB-CTC-1.3.0rc1/tests/complex/nsext/test.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/complex/nsext/tst-app.py` & `PyXB-CTC-1.3.0rc1/tests/complex/nsext/tst-app.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/complex/nsext/tst-extend.py` & `PyXB-CTC-1.3.0rc1/tests/complex/nsext/tst-extend.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-ENTITIES.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-ENTITIES.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-ENTITY.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-ENTITY.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-ID.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-ID.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-IDREF.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-IDREF.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-IDREFS.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-IDREFS.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-IntegerTypes.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-IntegerTypes.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-NCName.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-NCName.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-NMTOKEN.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-NMTOKEN.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-NMTOKENS.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-NMTOKENS.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-Name.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-Name.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-QName.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-QName.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-anyType.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-anyType.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-base64Binary.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-base64Binary.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-boolean.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-boolean.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-date.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-date.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-dateTime.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-dateTime.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-decimal.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-decimal.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-duration.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-duration.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-gDay.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-gDay.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-gMonth.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-gMonth.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-gMonthDay.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-gMonthDay.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-gYear.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-gYear.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-gYearMonth.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-gYearMonth.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-hexBinary.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-hexBinary.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-integer.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-integer.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-language.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-language.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-normalizedString.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-normalizedString.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-time.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-time.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/datatypes/test-token.py` & `PyXB-CTC-1.3.0rc1/tests/datatypes/test-token.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/documents/wsdl-001.xml` & `PyXB-CTC-1.3.0rc1/tests/documents/wsdl-001.xml`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/documents/wsdl-002.xml` & `PyXB-CTC-1.3.0rc1/tests/documents/wsdl-002.xml`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-ctd-attr.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-ctd-attr.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-ctd-extension.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-ctd-extension.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-ctd-simple.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-ctd-simple.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-deconflict.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-deconflict.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-empty-cstd.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-empty-cstd.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-enumeration.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-enumeration.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-external.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-external.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-facets.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-facets.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-generatorGetCommandLineArgs.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-generatorGetCommandLineArgs.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-include-aaq.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-include-aaq.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-include-aau.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-include-aau.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-include-ad.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-include-ad.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-include-daq.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-include-daq.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-include-dau.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-include-dau.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-include-dcu.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-include-dcu.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-include-ddq.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-include-ddq.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-include-ddu.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-include-ddu.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-mg-all.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-mg-all.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-mg-choice.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-mg-choice.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-mg-sequence.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-mg-sequence.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-namespace-uu.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-namespace-uu.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-particle.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-particle.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-po1.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-po1.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-properties.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-properties.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-properties2.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-properties2.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-recursive.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-recursive.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-simplerange.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-simplerange.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-substgroup.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-substgroup.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-time.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-time.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-typeinf.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-typeinf.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-union.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-union.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-wildcard.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-wildcard.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-xsi-nil.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-xsi-nil.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/test-xsi-type.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/test-xsi-type.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/drivers/tst-stored.py` & `PyXB-CTC-1.3.0rc1/tests/drivers/tst-stored.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/pyxb/test-cdata.py` & `PyXB-CTC-1.3.0rc1/tests/pyxb/test-cdata.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/pyxb/test-namespace.py` & `PyXB-CTC-1.3.0rc1/tests/pyxb/test-namespace.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/pyxb/test-reserved.py` & `PyXB-CTC-1.3.0rc1/tests/pyxb/test-reserved.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/alt-po1.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/alt-po1.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/anyType.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/anyType.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/components.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/components.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/enumerations.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/enumerations.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/incl-absent.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/incl-absent.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/incl-ad.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/incl-ad.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/incl-dau.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/incl-dau.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/incl-dcu.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/incl-dcu.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/incl-ddq.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/incl-ddq.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/incl-ddu.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/incl-ddu.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/incl-declared2.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/incl-declared2.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/nested-groups.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/nested-groups.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/particle.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/particle.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/po1.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/po1.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/qattr.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/qattr.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/shared-types.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/shared-types.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/substgroup.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/substgroup.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/test-collision.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/test-collision.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/test-ctd-attr.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/test-ctd-attr.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/test-ctd-extension.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/test-ctd-extension.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/test-ctd-simple.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/test-ctd-simple.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/test-empty-cstd.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/test-empty-cstd.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/test-external.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/test-external.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/test-include-dcu.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/test-include-dcu.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/test-mg-all.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/test-mg-all.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/test-mg-choice.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/test-mg-choice.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/test-mg-sequence.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/test-mg-sequence.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/test-namespace-uu.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/test-namespace-uu.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/test-recursive.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/test-recursive.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/test-typeinf.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/test-typeinf.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/test-union.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/test-union.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/test-wildcard.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/test-wildcard.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/time.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/time.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/validatable.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/validatable.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/xsi-nil.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/xsi-nil.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/schemas/xsi-type.xsd` & `PyXB-CTC-1.3.0rc1/tests/schemas/xsi-type.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/support.sh` & `PyXB-CTC-1.3.0rc1/tests/support.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/issue-0048/profile.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/issue-0048/profile.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0006.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0006.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0007.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0007.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0013.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0013.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0014.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0014.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0015.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0015.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0019.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0019.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0022.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0022.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0027.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0027.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0031.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0031.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0032.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0032.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0043.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0043.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0047.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0047.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0051.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0051.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0066.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0066.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0069.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0069.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0071.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0071.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0073.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0073.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0078.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0078.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0079.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0079.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0092.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0092.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-issue-0094.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-issue-0094.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0021.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0021.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0023.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0023.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0023b.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0023b.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0023c.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0023c.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0027.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0027.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0027b.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0027b.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0027c.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0027c.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0029.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0029.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0032.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0032.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0033a.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0033a.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0034.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0034.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0034b.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0034b.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0036.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0036.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0037.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0037.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0038.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0038.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0039.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0039.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0040.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0040.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0045.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0045.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0046.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0046.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0047.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0047.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0048.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0048.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0051.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0051.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0052.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0052.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0053.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0053.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0056.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0056.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0057.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0057.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0058.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0058.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0060.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0060.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0061.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0061.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0069.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0069.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0071.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0071.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0074.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0074.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0075.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0075.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0076.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0076.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0079.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0079.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0087.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0087.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0088.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0088.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0089.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0089.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0091.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0091.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0093.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0093.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0094.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0094.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0099.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0099.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0099a.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0099a.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0100.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0100.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0110.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0110.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0111.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0111.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0112.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0112.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0116.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0116.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0117.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0117.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0121.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0121.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0122.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0122.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0123.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0123.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0126.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0126.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0131.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0131.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0136.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0136.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0137.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0137.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0139.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0139.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0141.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0141.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0148.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0148.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0153.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0153.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0154.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0154.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0155.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0155.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0156a.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0156a.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0163.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0163.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0172.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0172.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0175.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0175.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0179.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0179.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0181.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0181.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0182.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0182.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0184.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0184.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0189.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0189.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0190.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0190.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0191.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0191.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0194.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0194.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0195.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0195.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0200.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0200.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0201.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0201.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0203.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0203.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0204.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0204.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0206.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0206.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0207.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0207.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0208.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0208.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0211.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0211.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0212.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0212.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0213.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0213.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0216.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0216.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0218.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0218.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0219.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0219.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0221.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0221.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0231.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0231.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/test-trac-0232.py` & `PyXB-CTC-1.3.0rc1/tests/trac/test-trac-0232.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0026/check-binding.py` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0026/check-binding.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0026/check-validation.py` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0026/check-validation.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0026/trac26.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0026/trac26.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0033/tread.py` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0033/tread.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0043/a.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0043/a.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0043/b.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0043/b.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0043/tst-1.py` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0043/tst-1.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0043/tst-2.py` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0043/tst-2.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0065/TestSchema.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0065/TestSchema.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0065/test.sh` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0065/test.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0073/profile.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0073/profile.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0080/check.py` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0080/check.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0080/multipleRestriction.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0080/multipleRestriction.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0089/example.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0089/example.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0092/test.sh` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0092/test.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0104/XSD/ModelA/AA.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0104/XSD/ModelA/AA.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0104/XSD/ModelA/AUXAA.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0104/XSD/ModelA/AUXAA.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0104/XSD/ModelB/AUXBB.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0104/XSD/ModelB/AUXBB.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0104/XSD/ModelB/BB.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0104/XSD/ModelB/BB.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0114/check.py` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0114/check.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0114/namespace_other_issue.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0114/namespace_other_issue.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0119/check.py` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0119/check.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0133/poc.xml` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0133/poc.xml`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0133/poc.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0133/poc.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0169/logging.cfg` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0169/logging.cfg`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0183/check.py` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0183/check.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0183/root.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0183/root.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0184/check.py` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0184/check.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0184/s0add.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0184/s0add.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0186/8_3_2_resource.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0186/8_3_2_resource.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0193/check.py` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0193/check.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0193/schema.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0193/schema.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0196/check.py` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0196/check.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0196/mix.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0196/mix.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0196/template.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0196/template.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0196/test.sh` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0196/test.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0198/check.py` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0198/check.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0198/wsse.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0198/wsse.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0198/wsu.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0198/wsu.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0199/check.py` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0199/check.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0202/check.py` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0202/check.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0202/sample.xsd` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0202/sample.xsd`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0230/sample.xml` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0230/sample.xml`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/trac/trac-0230/test.sh` & `PyXB-CTC-1.3.0rc1/tests/trac/trac-0230/test.sh`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/utils/test-domutils.py` & `PyXB-CTC-1.3.0rc1/tests/utils/test-domutils.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/utils/test-fac.py` & `PyXB-CTC-1.3.0rc1/tests/utils/test-fac.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/utils/test-saxutils.py` & `PyXB-CTC-1.3.0rc1/tests/utils/test-saxutils.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/utils/test-templates.py` & `PyXB-CTC-1.3.0rc1/tests/utils/test-templates.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/utils/test-unicode.py` & `PyXB-CTC-1.3.0rc1/tests/utils/test-unicode.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/utils/test-utility.py` & `PyXB-CTC-1.3.0rc1/tests/utils/test-utility.py`

 * *Files identical despite different names*

### Comparing `PyXB-CTC-1.3.0.dev0/tests/utils/test-xmlre.py` & `PyXB-CTC-1.3.0rc1/tests/utils/test-xmlre.py`

 * *Files identical despite different names*

