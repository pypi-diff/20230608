# Comparing `tmp/vml-parser-0.0.6.tar.gz` & `tmp/vml-parser-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vml-parser-0.0.6.tar", last modified: Thu Mar 30 08:35:45 2023, max compression
+gzip compressed data, was "vml-parser-0.0.7.tar", last modified: Fri Mar 31 22:45:25 2023, max compression
```

## Comparing `vml-parser-0.0.6.tar` & `vml-parser-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-03-30 08:35:45.181396 vml-parser-0.0.6/
--rw-r--r--   0 valerio   (1000) valerio   (1000)     1073 2023-03-28 14:46:29.000000 vml-parser-0.0.6/LICENSE
--rw-r--r--   0 valerio   (1000) valerio   (1000)     2689 2023-03-30 08:35:45.181396 vml-parser-0.0.6/PKG-INFO
--rw-r--r--   0 valerio   (1000) valerio   (1000)     2232 2023-03-30 08:35:21.000000 vml-parser-0.0.6/README.md
--rw-r--r--   0 valerio   (1000) valerio   (1000)      497 2023-03-30 08:35:39.000000 vml-parser-0.0.6/pyproject.toml
--rw-r--r--   0 valerio   (1000) valerio   (1000)       38 2023-03-30 08:35:45.181396 vml-parser-0.0.6/setup.cfg
-drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-03-30 08:35:45.178396 vml-parser-0.0.6/src/
-drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-03-30 08:35:45.179396 vml-parser-0.0.6/src/vml_parser/
--rw-r--r--   0 valerio   (1000) valerio   (1000)        0 2023-03-28 13:55:01.000000 vml-parser-0.0.6/src/vml_parser/__init__.py
--rwxr-xr-x   0 valerio   (1000) valerio   (1000)     3435 2023-03-29 23:18:52.000000 vml-parser-0.0.6/src/vml_parser/vml.py
-drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-03-30 08:35:45.181396 vml-parser-0.0.6/src/vml_parser.egg-info/
--rw-r--r--   0 valerio   (1000) valerio   (1000)     2689 2023-03-30 08:35:45.000000 vml-parser-0.0.6/src/vml_parser.egg-info/PKG-INFO
--rw-r--r--   0 valerio   (1000) valerio   (1000)      288 2023-03-30 08:35:45.000000 vml-parser-0.0.6/src/vml_parser.egg-info/SOURCES.txt
--rw-r--r--   0 valerio   (1000) valerio   (1000)        1 2023-03-30 08:35:45.000000 vml-parser-0.0.6/src/vml_parser.egg-info/dependency_links.txt
--rw-r--r--   0 valerio   (1000) valerio   (1000)       44 2023-03-30 08:35:45.000000 vml-parser-0.0.6/src/vml_parser.egg-info/entry_points.txt
--rw-r--r--   0 valerio   (1000) valerio   (1000)       11 2023-03-30 08:35:45.000000 vml-parser-0.0.6/src/vml_parser.egg-info/top_level.txt
-drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-03-30 08:35:45.181396 vml-parser-0.0.6/tests/
--rw-r--r--   0 valerio   (1000) valerio   (1000)      221 2023-03-29 23:20:29.000000 vml-parser-0.0.6/tests/test.py
+drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-03-31 22:45:25.360035 vml-parser-0.0.7/
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     1073 2023-03-28 14:46:29.000000 vml-parser-0.0.7/LICENSE
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     3292 2023-03-31 22:45:25.360035 vml-parser-0.0.7/PKG-INFO
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     2835 2023-03-31 22:43:29.000000 vml-parser-0.0.7/README.md
+-rw-r--r--   0 valerio   (1000) valerio   (1000)      497 2023-03-31 22:45:19.000000 vml-parser-0.0.7/pyproject.toml
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       38 2023-03-31 22:45:25.360035 vml-parser-0.0.7/setup.cfg
+drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-03-31 22:45:25.356035 vml-parser-0.0.7/src/
+drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-03-31 22:45:25.358035 vml-parser-0.0.7/src/vml_parser/
+-rw-r--r--   0 valerio   (1000) valerio   (1000)        0 2023-03-28 13:55:01.000000 vml-parser-0.0.7/src/vml_parser/__init__.py
+-rwxr-xr-x   0 valerio   (1000) valerio   (1000)     5177 2023-03-31 22:45:05.000000 vml-parser-0.0.7/src/vml_parser/vml.py
+drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-03-31 22:45:25.359035 vml-parser-0.0.7/src/vml_parser.egg-info/
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     3292 2023-03-31 22:45:25.000000 vml-parser-0.0.7/src/vml_parser.egg-info/PKG-INFO
+-rw-r--r--   0 valerio   (1000) valerio   (1000)      288 2023-03-31 22:45:25.000000 vml-parser-0.0.7/src/vml_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)        1 2023-03-31 22:45:25.000000 vml-parser-0.0.7/src/vml_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       44 2023-03-31 22:45:25.000000 vml-parser-0.0.7/src/vml_parser.egg-info/entry_points.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       11 2023-03-31 22:45:25.000000 vml-parser-0.0.7/src/vml_parser.egg-info/top_level.txt
+drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2023-03-31 22:45:25.360035 vml-parser-0.0.7/tests/
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     2146 2023-03-31 22:26:10.000000 vml-parser-0.0.7/tests/test.py
```

### Comparing `vml-parser-0.0.6/LICENSE` & `vml-parser-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vml-parser-0.0.6/PKG-INFO` & `vml-parser-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 Metadata-Version: 2.1
 Name: vml-parser
-Version: 0.0.6
+Version: 0.0.7
 Summary: velocitous markup language to JSON parser
 Author-email: Valerio Iacobucci <valerio@valerioiacobucci.com>
 Project-URL: Homepage, https://github.com/iacobucci/vml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # vml
 ## velocitous markup language
 (Totally not related with [VML-SVG](https://en.wikipedia.org/wiki/Vector_Markup_Language)\)  
-This is a JSON parser for a markup language, if you want to call it like that, that i found myself using while jolting notes in the ~~fastest~~ *most velocitous*, and laziest way that i could think of... It goes pretty much like this:
-
+This is a JSON parser for a markup language, if you want to call it like that, that i found myself using while jolting notes in the ~~fastest~~ *most velocitous*, and laziest way that i could think of... It goes pretty much like this:  
 ```
 element 1
 	things
 		dog
 		[x] snacks
 			[ ] apple
 			pear
 		house
 	names
 		james
 		alfred
-
 [ ] element 2
 	foo
 	bar
 	baz
+foobar
 ```
-That translates to this bulky JSON. You see, it makes JSON look bulky!!!
+That translates to this bulky JSON. You see, it makes JSON look bulky!!!  
 ```
 [
-  {
-    "element 1": [
-      {
-        "things": [
-          "dog",
-          {
-            "snacks": [
-              {
-                "apple": [],
-                "checked": false
-              },
-              "pear"
-            ],
-            "checked": true
-          },
-          "house"
-        ]
-      },
-      {
-        "names": [
-          "james",
-          "alfred"
+    {
+        "element 1": [
+            {
+                "things": [
+                    "dog",
+                    {
+                        "snacks": [
+                            {
+                                "apple": [],
+                                "checked": false
+                            },
+                            "pear"
+                        ],
+                        "checked": true
+                    },
+                    "house"
+                ]
+            },
+            {
+                "names": [
+                    "james",
+                    "alfred"
+                ]
+            }
         ]
-      }
-    ]
-  },
-  {
-    "element 2": [
-      "foo",
-      "bar",
-      "baz"
-    ],
-    "checked": false
-  }
+    },
+    {
+        "element 2": [
+            "foo",
+            "bar",
+            "baz"
+        ],
+        "checked": false
+    },
+    "foobar"
 ]
 ```
 vml uses tabs to differentiate the hierarchical level of the current line... i think you got what i mean. Plus, you can also add checkboxes to every line with "[ ]", and you can check it with "[x]", and all this translates to a "checked" property in the JSON representation. It's easy to write vml with vi, for example you might check an empty checkbox with ```rx``` and move around tabulations efficiently with ```>>``` or ```<<```. In fact, this should really have been called tml, as in *tab markup language*, but unfortunately, that resembled too much TOML, dammit you Tom!!  
-Install this with ```pip3 install vml-parser```  
-Import it with ```from vml_parser import vml```, so you that you can access the ```vml.parse(s : list[str]) -> list[Element]``` method. With that you can easily ```json.loads(str(vml.parse(s : list[str]))) -> object```. You now can also dump your python objects to a vml-formatted string with ```vml.dump(obj: object) -> str```, and maybe save it to a file for later use!  
-You will also get the ```vml``` command line script for free! you can pipe it to stdout or you can pass it any number of filenames for it to read.  
+Install this with ```pip3 install vml-parser```.  
+import it with ```from vml_parser import vml```, so you that you can access the ```vml.parse(s : list[str]) -> list[Element]``` method. A list of Elements gives you a middleware representation of what's in your vml. You might, vice versa, build up programmatically your list of Elements, and ```vml.dump(obj: list[Element]) -> list[str]``` for a later use. You now can also dump a list of JSON strings to a vml-formatted list of lines with ```vml.dumps(lines: list[str]) -> list[str]```.  
+You will also get the ```vml``` command line script for free! (it pairs neatly with the ```jq``` cli). You can pipe it to stdout or you can pass it any number of filenames for it to read, and with ```-d``` you can use the included JSON to vml dumper. Have fun with it laying crazy pipes like ```... | vml | vml -d | vml | vml -d | ...```!!
```

### Comparing `vml-parser-0.0.6/README.md` & `vml-parser-0.0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 # vml
 ## velocitous markup language
 (Totally not related with [VML-SVG](https://en.wikipedia.org/wiki/Vector_Markup_Language)\)  
-This is a JSON parser for a markup language, if you want to call it like that, that i found myself using while jolting notes in the ~~fastest~~ *most velocitous*, and laziest way that i could think of... It goes pretty much like this:
-
+This is a JSON parser for a markup language, if you want to call it like that, that i found myself using while jolting notes in the ~~fastest~~ *most velocitous*, and laziest way that i could think of... It goes pretty much like this:  
 ```
 element 1
 	things
 		dog
 		[x] snacks
 			[ ] apple
 			pear
 		house
 	names
 		james
 		alfred
-
 [ ] element 2
 	foo
 	bar
 	baz
+foobar
 ```
-That translates to this bulky JSON. You see, it makes JSON look bulky!!!
+That translates to this bulky JSON. You see, it makes JSON look bulky!!!  
 ```
 [
-  {
-    "element 1": [
-      {
-        "things": [
-          "dog",
-          {
-            "snacks": [
-              {
-                "apple": [],
-                "checked": false
-              },
-              "pear"
-            ],
-            "checked": true
-          },
-          "house"
+    {
+        "element 1": [
+            {
+                "things": [
+                    "dog",
+                    {
+                        "snacks": [
+                            {
+                                "apple": [],
+                                "checked": false
+                            },
+                            "pear"
+                        ],
+                        "checked": true
+                    },
+                    "house"
+                ]
+            },
+            {
+                "names": [
+                    "james",
+                    "alfred"
+                ]
+            }
         ]
-      },
-      {
-        "names": [
-          "james",
-          "alfred"
-        ]
-      }
-    ]
-  },
-  {
-    "element 2": [
-      "foo",
-      "bar",
-      "baz"
-    ],
-    "checked": false
-  }
+    },
+    {
+        "element 2": [
+            "foo",
+            "bar",
+            "baz"
+        ],
+        "checked": false
+    },
+    "foobar"
 ]
 ```
 vml uses tabs to differentiate the hierarchical level of the current line... i think you got what i mean. Plus, you can also add checkboxes to every line with "[ ]", and you can check it with "[x]", and all this translates to a "checked" property in the JSON representation. It's easy to write vml with vi, for example you might check an empty checkbox with ```rx``` and move around tabulations efficiently with ```>>``` or ```<<```. In fact, this should really have been called tml, as in *tab markup language*, but unfortunately, that resembled too much TOML, dammit you Tom!!  
-Install this with ```pip3 install vml-parser```  
-Import it with ```from vml_parser import vml```, so you that you can access the ```vml.parse(s : list[str]) -> list[Element]``` method. With that you can easily ```json.loads(str(vml.parse(s : list[str]))) -> object```. You now can also dump your python objects to a vml-formatted string with ```vml.dump(obj: object) -> str```, and maybe save it to a file for later use!  
-You will also get the ```vml``` command line script for free! you can pipe it to stdout or you can pass it any number of filenames for it to read.  
+Install this with ```pip3 install vml-parser```.  
+import it with ```from vml_parser import vml```, so you that you can access the ```vml.parse(s : list[str]) -> list[Element]``` method. A list of Elements gives you a middleware representation of what's in your vml. You might, vice versa, build up programmatically your list of Elements, and ```vml.dump(obj: list[Element]) -> list[str]``` for a later use. You now can also dump a list of JSON strings to a vml-formatted list of lines with ```vml.dumps(lines: list[str]) -> list[str]```.  
+You will also get the ```vml``` command line script for free! (it pairs neatly with the ```jq``` cli). You can pipe it to stdout or you can pass it any number of filenames for it to read, and with ```-d``` you can use the included JSON to vml dumper. Have fun with it laying crazy pipes like ```... | vml | vml -d | vml | vml -d | ...```!!
```

### Comparing `vml-parser-0.0.6/src/vml_parser.egg-info/PKG-INFO` & `vml-parser-0.0.7/src/vml_parser.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 Metadata-Version: 2.1
 Name: vml-parser
-Version: 0.0.6
+Version: 0.0.7
 Summary: velocitous markup language to JSON parser
 Author-email: Valerio Iacobucci <valerio@valerioiacobucci.com>
 Project-URL: Homepage, https://github.com/iacobucci/vml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # vml
 ## velocitous markup language
 (Totally not related with [VML-SVG](https://en.wikipedia.org/wiki/Vector_Markup_Language)\)  
-This is a JSON parser for a markup language, if you want to call it like that, that i found myself using while jolting notes in the ~~fastest~~ *most velocitous*, and laziest way that i could think of... It goes pretty much like this:
-
+This is a JSON parser for a markup language, if you want to call it like that, that i found myself using while jolting notes in the ~~fastest~~ *most velocitous*, and laziest way that i could think of... It goes pretty much like this:  
 ```
 element 1
 	things
 		dog
 		[x] snacks
 			[ ] apple
 			pear
 		house
 	names
 		james
 		alfred
-
 [ ] element 2
 	foo
 	bar
 	baz
+foobar
 ```
-That translates to this bulky JSON. You see, it makes JSON look bulky!!!
+That translates to this bulky JSON. You see, it makes JSON look bulky!!!  
 ```
 [
-  {
-    "element 1": [
-      {
-        "things": [
-          "dog",
-          {
-            "snacks": [
-              {
-                "apple": [],
-                "checked": false
-              },
-              "pear"
-            ],
-            "checked": true
-          },
-          "house"
-        ]
-      },
-      {
-        "names": [
-          "james",
-          "alfred"
+    {
+        "element 1": [
+            {
+                "things": [
+                    "dog",
+                    {
+                        "snacks": [
+                            {
+                                "apple": [],
+                                "checked": false
+                            },
+                            "pear"
+                        ],
+                        "checked": true
+                    },
+                    "house"
+                ]
+            },
+            {
+                "names": [
+                    "james",
+                    "alfred"
+                ]
+            }
         ]
-      }
-    ]
-  },
-  {
-    "element 2": [
-      "foo",
-      "bar",
-      "baz"
-    ],
-    "checked": false
-  }
+    },
+    {
+        "element 2": [
+            "foo",
+            "bar",
+            "baz"
+        ],
+        "checked": false
+    },
+    "foobar"
 ]
 ```
 vml uses tabs to differentiate the hierarchical level of the current line... i think you got what i mean. Plus, you can also add checkboxes to every line with "[ ]", and you can check it with "[x]", and all this translates to a "checked" property in the JSON representation. It's easy to write vml with vi, for example you might check an empty checkbox with ```rx``` and move around tabulations efficiently with ```>>``` or ```<<```. In fact, this should really have been called tml, as in *tab markup language*, but unfortunately, that resembled too much TOML, dammit you Tom!!  
-Install this with ```pip3 install vml-parser```  
-Import it with ```from vml_parser import vml```, so you that you can access the ```vml.parse(s : list[str]) -> list[Element]``` method. With that you can easily ```json.loads(str(vml.parse(s : list[str]))) -> object```. You now can also dump your python objects to a vml-formatted string with ```vml.dump(obj: object) -> str```, and maybe save it to a file for later use!  
-You will also get the ```vml``` command line script for free! you can pipe it to stdout or you can pass it any number of filenames for it to read.  
+Install this with ```pip3 install vml-parser```.  
+import it with ```from vml_parser import vml```, so you that you can access the ```vml.parse(s : list[str]) -> list[Element]``` method. A list of Elements gives you a middleware representation of what's in your vml. You might, vice versa, build up programmatically your list of Elements, and ```vml.dump(obj: list[Element]) -> list[str]``` for a later use. You now can also dump a list of JSON strings to a vml-formatted list of lines with ```vml.dumps(lines: list[str]) -> list[str]```.  
+You will also get the ```vml``` command line script for free! (it pairs neatly with the ```jq``` cli). You can pipe it to stdout or you can pass it any number of filenames for it to read, and with ```-d``` you can use the included JSON to vml dumper. Have fun with it laying crazy pipes like ```... | vml | vml -d | vml | vml -d | ...```!!
```

