# Comparing `tmp/autoscrum-0.2.0.tar.gz` & `tmp/autoscrum-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoscrum-0.2.0.tar", last modified: Mon Jun  5 17:37:26 2023, max compression
+gzip compressed data, was "autoscrum-0.3.0.tar", last modified: Thu Jun  8 17:33:50 2023, max compression
```

## Comparing `autoscrum-0.2.0.tar` & `autoscrum-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-05 17:37:26.637970 autoscrum-0.2.0/
--rw-rw-r--   0 martin    (1000) martin    (1000)    35149 2023-06-05 14:55:21.000000 autoscrum-0.2.0/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)    43986 2023-06-05 17:37:26.637970 autoscrum-0.2.0/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     2969 2023-06-05 15:41:55.000000 autoscrum-0.2.0/README.md
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-05 17:37:26.637970 autoscrum-0.2.0/autoscrum/
--rw-rw-r--   0 martin    (1000) martin    (1000)      113 2023-06-05 15:22:08.000000 autoscrum-0.2.0/autoscrum/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5205 2023-06-05 15:16:22.000000 autoscrum-0.2.0/autoscrum/__main__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5577 2023-06-05 15:15:15.000000 autoscrum-0.2.0/autoscrum/autoscrum.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1777 2023-06-01 20:12:54.000000 autoscrum-0.2.0/autoscrum/controller.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-05 17:37:26.637970 autoscrum-0.2.0/autoscrum/data/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2274 2023-06-05 14:59:10.000000 autoscrum-0.2.0/autoscrum/data/featurizer.hbs
--rw-rw-r--   0 martin    (1000) martin    (1000)     1032 2023-06-05 15:00:21.000000 autoscrum-0.2.0/autoscrum/data/taskalizer.hbs
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-05 17:37:26.637970 autoscrum-0.2.0/autoscrum.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)    43986 2023-06-05 17:37:26.000000 autoscrum-0.2.0/autoscrum.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      416 2023-06-05 17:37:26.000000 autoscrum-0.2.0/autoscrum.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-05 17:37:26.000000 autoscrum-0.2.0/autoscrum.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       54 2023-06-05 17:37:26.000000 autoscrum-0.2.0/autoscrum.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       80 2023-06-05 17:37:26.000000 autoscrum-0.2.0/autoscrum.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       10 2023-06-05 17:37:26.000000 autoscrum-0.2.0/autoscrum.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     1153 2023-06-05 17:37:10.000000 autoscrum-0.2.0/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-06-05 17:37:26.637970 autoscrum-0.2.0/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)      417 2023-06-05 14:52:02.000000 autoscrum-0.2.0/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-05 17:37:26.637970 autoscrum-0.2.0/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)      195 2023-06-05 15:24:14.000000 autoscrum-0.2.0/tests/test_autoscrum.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-08 17:33:50.201496 autoscrum-0.3.0/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    35149 2023-06-05 17:43:03.000000 autoscrum-0.3.0/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)    44406 2023-06-08 17:33:50.201496 autoscrum-0.3.0/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3389 2023-06-05 18:03:56.000000 autoscrum-0.3.0/README.md
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-08 17:33:50.197496 autoscrum-0.3.0/autoscrum/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      113 2023-06-08 17:32:13.000000 autoscrum-0.3.0/autoscrum/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5351 2023-06-08 17:31:48.000000 autoscrum-0.3.0/autoscrum/__main__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6140 2023-06-08 17:31:48.000000 autoscrum-0.3.0/autoscrum/autoscrum.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1777 2023-06-01 20:12:54.000000 autoscrum-0.3.0/autoscrum/controller.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-08 17:33:50.201496 autoscrum-0.3.0/autoscrum/data/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1218 2023-06-05 17:43:03.000000 autoscrum-0.3.0/autoscrum/data/acceptance.hbs
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3731 2023-06-05 17:43:03.000000 autoscrum-0.3.0/autoscrum/data/clarifier.hbs
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2313 2023-06-08 17:31:48.000000 autoscrum-0.3.0/autoscrum/data/featurizer.hbs
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2126 2023-06-05 17:43:03.000000 autoscrum-0.3.0/autoscrum/data/goalmaker.hbs
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3606 2023-06-05 17:43:03.000000 autoscrum-0.3.0/autoscrum/data/planner.hbs
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2644 2023-06-08 17:31:48.000000 autoscrum-0.3.0/autoscrum/data/requalizer.hbs
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2606 2023-06-08 17:31:48.000000 autoscrum-0.3.0/autoscrum/data/storylizer.hbs
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1032 2023-06-05 17:43:03.000000 autoscrum-0.3.0/autoscrum/data/taskalizer.hbs
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-08 17:33:50.197496 autoscrum-0.3.0/autoscrum.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    44406 2023-06-08 17:33:50.000000 autoscrum-0.3.0/autoscrum.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      591 2023-06-08 17:33:50.000000 autoscrum-0.3.0/autoscrum.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-08 17:33:50.000000 autoscrum-0.3.0/autoscrum.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       54 2023-06-08 17:33:50.000000 autoscrum-0.3.0/autoscrum.egg-info/entry_points.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       80 2023-06-08 17:33:50.000000 autoscrum-0.3.0/autoscrum.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       10 2023-06-08 17:33:50.000000 autoscrum-0.3.0/autoscrum.egg-info/top_level.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1154 2023-06-08 17:32:13.000000 autoscrum-0.3.0/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-06-08 17:33:50.201496 autoscrum-0.3.0/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)      340 2023-06-08 17:33:45.000000 autoscrum-0.3.0/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-08 17:33:50.201496 autoscrum-0.3.0/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      195 2023-06-05 17:43:03.000000 autoscrum-0.3.0/tests/test_autoscrum.py
```

### Comparing `autoscrum-0.2.0/LICENSE` & `autoscrum-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoscrum-0.2.0/PKG-INFO` & `autoscrum-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoscrum
-Version: 0.2.0
+Version: 0.3.0
 Summary: AutoScrum
 Author-email: Martin Schröder <info@swedishembedded.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -688,24 +688,32 @@
 License-File: LICENSE
 
 # AutoScrum
 
 AutoScrum is a python script for automating the Scrum project planning process
 using language models.
 
-[Download Research Paper](https://github.com/autoscrum/autoscrum/raw/main/paper.pdf)
+[Download Research Paper](https://github.com/autoscrum/autoscrum/raw/main/Martin-Schroder-AutoScrum-Paper.pdf)
 
 You provide it with your product name, current customer situation and desired
 customer situation and the script does the rest.
 
 ![overview](images/overview.png "What is autoscrum?")
 
 AutoScrum is designed to assist users with the automatic generation of detailed
 scrum plans using language models.
 
+![detail](images/detail.png "AutoScrum details")
+
+AutoScrum also supports shortcut mode where a single language program is used to generate the next
+most urgent task to bridge the gap between current and desired situation. The shortcut mode does not
+create any user stories or features. Instead it simply iteratively creates a plan.
+
+![shortcut](images/shortcut.png "AutoScrum shortcut mode")
+
 By using AutoScrum, you can generate stories, features, goals, requirements,
 tasks, acceptance criteria, and clarifications for your scrum planning. 
 
 ## Installing
 
 You can install dependencies using pip:
```

### Comparing `autoscrum-0.2.0/README.md` & `autoscrum-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 # AutoScrum
 
 AutoScrum is a python script for automating the Scrum project planning process
 using language models.
 
-[Download Research Paper](https://github.com/autoscrum/autoscrum/raw/main/paper.pdf)
+[Download Research Paper](https://github.com/autoscrum/autoscrum/raw/main/Martin-Schroder-AutoScrum-Paper.pdf)
 
 You provide it with your product name, current customer situation and desired
 customer situation and the script does the rest.
 
 ![overview](images/overview.png "What is autoscrum?")
 
 AutoScrum is designed to assist users with the automatic generation of detailed
 scrum plans using language models.
 
+![detail](images/detail.png "AutoScrum details")
+
+AutoScrum also supports shortcut mode where a single language program is used to generate the next
+most urgent task to bridge the gap between current and desired situation. The shortcut mode does not
+create any user stories or features. Instead it simply iteratively creates a plan.
+
+![shortcut](images/shortcut.png "AutoScrum shortcut mode")
+
 By using AutoScrum, you can generate stories, features, goals, requirements,
 tasks, acceptance criteria, and clarifications for your scrum planning. 
 
 ## Installing
 
 You can install dependencies using pip:
```

### Comparing `autoscrum-0.2.0/autoscrum/__main__.py` & `autoscrum-0.3.0/autoscrum/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,21 +36,27 @@
 
     subparser = subparsers.add_parser("requirements")
     subparser.add_argument("-n", "--count", type=int, default=3)
 
     subparser = subparsers.add_parser("plan")
     subparser.add_argument("-n", "--count", type=int, default=1)
 
+    subparser = subparsers.add_parser("init")
+
     args = parser.parse_args()
 
     print(f"Using datafile: {args.data_file}")
     autoscrum = AutoScrum(args.data_file)
 
 
-    if args.command == "plan":
+    if args.command == "init":
+        autoscrum.reset()
+        autoscrum.save(args.data_file)
+
+    elif args.command == "plan":
         print("Existing plan: ")
         for i,f in enumerate(autoscrum.plan):
             print(f"{i}: {f['task']}")
 
         res = autoscrum.gen_plan(count=args.count)
 
         print("Identified new steps: ")
```

### Comparing `autoscrum-0.2.0/autoscrum/autoscrum.py` & `autoscrum-0.3.0/autoscrum/autoscrum.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,34 @@
         self.storylizer = self.load_program("storylizer")
         self.goalmaker = self.load_program("goalmaker")
         self.clarifier = self.load_program("clarifier")
         self.acceptance = self.load_program("acceptance")
         self.taskalizer = self.load_program("taskalizer")
         self.requalizer = self.load_program("requalizer")
         self.planner = self.load_program("planner")
+        if not Path(path).exists():
+            self.reset()
+            self.save(path)
         self.data = self.load_data(path)
 
+    def reset(self):
+        self.data = {
+            "product": "Your product name",
+            "vision": "Your product vision",
+            "niche": "Your product niche",
+            "current_state": {},
+            "desired_state": {},
+            "plan": [],
+            "requirements": [],
+            "sprint_duration": "2 weeks",
+            "features": [],
+            "stories": [],
+            "avoid": []
+        }
+
     def load_data(self, path):
         """
         Loads data json file
         """
         return json.loads(Path(path).read_text())
 
     def load_program(self, name: str):
@@ -63,18 +81,19 @@
     def gen_requirements(self, count:int):
         prog = self.requalizer(
             product=self.data["product"],
             vision=self.data["vision"],
             niche=self.data["niche"],
             current_state=self.data["current_state"],
             desired_state=self.data["desired_state"],
-            requirements=self.data["requirements"],
+            requirements=[f["name"] for f in self.data["requirements"]],
             count=count
         )
         try:
+            print(prog)
             obj = json.loads(prog["response"])
             return obj
         except:
             print(prog)
             print("Error: JSON conversion failed")
         return []
```

### Comparing `autoscrum-0.2.0/autoscrum/controller.py` & `autoscrum-0.3.0/autoscrum/controller.py`

 * *Files identical despite different names*

### Comparing `autoscrum-0.2.0/autoscrum/data/featurizer.hbs` & `autoscrum-0.3.0/autoscrum/data/featurizer.hbs`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,16 @@
   {
     "name": "Another feature",
     "explanation": "explanation of the second feature",
     "reasoning": "Reasoning for why we should develop this feature",
     "goal": "name of product goal"
   }
 ]
+
+Only output valid JSON list of items.
 {{~/system}}
 {{#user~}}
 Product: {{product}}
 Product Vision: {{vision}}
 Requirements: {{requirements}}
 Story Features: {{story_features}}
 Existing Features: {{features}}
```

### Comparing `autoscrum-0.2.0/autoscrum/data/taskalizer.hbs` & `autoscrum-0.3.0/autoscrum/data/taskalizer.hbs`

 * *Files identical despite different names*

### Comparing `autoscrum-0.2.0/autoscrum.egg-info/PKG-INFO` & `autoscrum-0.3.0/autoscrum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoscrum
-Version: 0.2.0
+Version: 0.3.0
 Summary: AutoScrum
 Author-email: Martin Schröder <info@swedishembedded.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -688,24 +688,32 @@
 License-File: LICENSE
 
 # AutoScrum
 
 AutoScrum is a python script for automating the Scrum project planning process
 using language models.
 
-[Download Research Paper](https://github.com/autoscrum/autoscrum/raw/main/paper.pdf)
+[Download Research Paper](https://github.com/autoscrum/autoscrum/raw/main/Martin-Schroder-AutoScrum-Paper.pdf)
 
 You provide it with your product name, current customer situation and desired
 customer situation and the script does the rest.
 
 ![overview](images/overview.png "What is autoscrum?")
 
 AutoScrum is designed to assist users with the automatic generation of detailed
 scrum plans using language models.
 
+![detail](images/detail.png "AutoScrum details")
+
+AutoScrum also supports shortcut mode where a single language program is used to generate the next
+most urgent task to bridge the gap between current and desired situation. The shortcut mode does not
+create any user stories or features. Instead it simply iteratively creates a plan.
+
+![shortcut](images/shortcut.png "AutoScrum shortcut mode")
+
 By using AutoScrum, you can generate stories, features, goals, requirements,
 tasks, acceptance criteria, and clarifications for your scrum planning. 
 
 ## Installing
 
 You can install dependencies using pip:
```

### Comparing `autoscrum-0.2.0/pyproject.toml` & `autoscrum-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autoscrum"
-version = "0.2.0"
+version = "0.3.0"
 description = "AutoScrum"
 readme = "README.md"
 authors = [{ name = "Martin Schröder", email = "info@swedishembedded.com" }]
 license = { file = "LICENSE" }
 classifiers = [
 	"License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 	"Programming Language :: Python",
@@ -35,19 +35,19 @@
 [project.urls]
 Homepage = "https://github.com/autoscrum/autoscrum"
 
 [project.scripts]
 autoscrum = "autoscrum.__main__:main"
 
 [tool.bumpver]
-current_version = "0.2.0"
+current_version = "0.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
-tag = true
+tag = false
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
 	'current_version = "{version}"',
 	'version = "{version}"',
 ]
```

