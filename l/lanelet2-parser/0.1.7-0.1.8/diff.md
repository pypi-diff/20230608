# Comparing `tmp/lanelet2_parser-0.1.7.tar.gz` & `tmp/lanelet2_parser-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lanelet2_parser-0.1.7.tar", last modified: Fri Nov 15 09:25:13 2019, max compression
+gzip compressed data, was "lanelet2_parser-0.1.8.tar", last modified: Thu Jun  8 08:26:03 2023, max compression
```

## Comparing `lanelet2_parser-0.1.7.tar` & `lanelet2_parser-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 autoware  (1000) autoware  (1000)        0 2019-11-15 09:25:13.000000 lanelet2_parser-0.1.7/
--rw-rw-r--   0 autoware  (1000) autoware  (1000)        0 2019-08-01 10:29:02.000000 lanelet2_parser-0.1.7/MANIFEST.in
--rw-rw-r--   0 autoware  (1000) autoware  (1000)     3701 2019-11-15 09:25:13.000000 lanelet2_parser-0.1.7/PKG-INFO
--rw-rw-r--   0 autoware  (1000) autoware  (1000)     1952 2019-08-20 10:06:05.000000 lanelet2_parser-0.1.7/README.md
-drwxrwxr-x   0 autoware  (1000) autoware  (1000)        0 2019-11-15 09:25:13.000000 lanelet2_parser-0.1.7/lanelet2_parser/
--rw-rw-r--   0 autoware  (1000) autoware  (1000)      299 2019-11-15 09:24:52.000000 lanelet2_parser-0.1.7/lanelet2_parser/__init__.py
--rw-rw-r--   0 autoware  (1000) autoware  (1000)      505 2019-08-02 08:40:41.000000 lanelet2_parser-0.1.7/lanelet2_parser/exceptions.py
-drwxrwxr-x   0 autoware  (1000) autoware  (1000)        0 2019-11-15 09:25:13.000000 lanelet2_parser-0.1.7/lanelet2_parser/lanelet2/
--rw-rw-r--   0 autoware  (1000) autoware  (1000)        0 2019-08-20 11:26:31.000000 lanelet2_parser-0.1.7/lanelet2_parser/lanelet2/__init__.py
--rw-rw-r--   0 autoware  (1000) autoware  (1000)      120 2019-08-09 06:22:22.000000 lanelet2_parser-0.1.7/lanelet2_parser/lanelet2/config.py
--rw-rw-r--   0 autoware  (1000) autoware  (1000)     6505 2019-10-28 12:40:55.000000 lanelet2_parser-0.1.7/lanelet2_parser/lanelet2/converter.py
--rw-rw-r--   0 autoware  (1000) autoware  (1000)     6570 2019-11-15 09:23:10.000000 lanelet2_parser-0.1.7/lanelet2_parser/lanelet2/models.py
--rw-rw-r--   0 autoware  (1000) autoware  (1000)     7247 2019-10-28 12:50:43.000000 lanelet2_parser-0.1.7/lanelet2_parser/lanelet2/network.py
-drwxrwxr-x   0 autoware  (1000) autoware  (1000)        0 2019-11-15 09:25:13.000000 lanelet2_parser-0.1.7/lanelet2_parser/osm/
--rw-rw-r--   0 autoware  (1000) autoware  (1000)        0 2019-08-20 11:26:33.000000 lanelet2_parser-0.1.7/lanelet2_parser/osm/__init__.py
--rw-rw-r--   0 autoware  (1000) autoware  (1000)     3369 2019-09-18 02:52:45.000000 lanelet2_parser-0.1.7/lanelet2_parser/osm/models.py
--rw-rw-r--   0 autoware  (1000) autoware  (1000)      866 2019-08-09 06:00:40.000000 lanelet2_parser-0.1.7/lanelet2_parser/osm/validator.py
--rw-rw-r--   0 autoware  (1000) autoware  (1000)     4205 2019-10-28 12:40:45.000000 lanelet2_parser-0.1.7/lanelet2_parser/parser.py
-drwxrwxr-x   0 autoware  (1000) autoware  (1000)        0 2019-11-15 09:25:13.000000 lanelet2_parser-0.1.7/lanelet2_parser.egg-info/
--rw-rw-r--   0 autoware  (1000) autoware  (1000)     3701 2019-11-15 09:25:13.000000 lanelet2_parser-0.1.7/lanelet2_parser.egg-info/PKG-INFO
--rw-rw-r--   0 autoware  (1000) autoware  (1000)      584 2019-11-15 09:25:13.000000 lanelet2_parser-0.1.7/lanelet2_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 autoware  (1000) autoware  (1000)        1 2019-11-15 09:25:13.000000 lanelet2_parser-0.1.7/lanelet2_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 autoware  (1000) autoware  (1000)       18 2019-11-15 09:25:13.000000 lanelet2_parser-0.1.7/lanelet2_parser.egg-info/requires.txt
--rw-rw-r--   0 autoware  (1000) autoware  (1000)       16 2019-11-15 09:25:13.000000 lanelet2_parser-0.1.7/lanelet2_parser.egg-info/top_level.txt
--rw-rw-r--   0 autoware  (1000) autoware  (1000)       38 2019-11-15 09:25:13.000000 lanelet2_parser-0.1.7/setup.cfg
--rw-rw-r--   0 autoware  (1000) autoware  (1000)     1963 2019-08-20 11:41:08.000000 lanelet2_parser-0.1.7/setup.py
+drwxr-xr-x   0 iidayuuki   (501) staff       (20)        0 2023-06-08 08:26:03.977903 lanelet2_parser-0.1.8/
+-rw-r--r--   0 iidayuuki   (501) staff       (20)        0 2023-06-08 07:50:59.000000 lanelet2_parser-0.1.8/MANIFEST.in
+-rw-r--r--   0 iidayuuki   (501) staff       (20)     3695 2023-06-08 08:26:03.976770 lanelet2_parser-0.1.8/PKG-INFO
+-rw-r--r--   0 iidayuuki   (501) staff       (20)     1946 2023-06-08 07:50:59.000000 lanelet2_parser-0.1.8/README.md
+drwxr-xr-x   0 iidayuuki   (501) staff       (20)        0 2023-06-08 08:26:03.947773 lanelet2_parser-0.1.8/lanelet2_parser/
+-rw-r--r--   0 iidayuuki   (501) staff       (20)      299 2023-06-08 08:25:38.000000 lanelet2_parser-0.1.8/lanelet2_parser/__init__.py
+-rw-r--r--   0 iidayuuki   (501) staff       (20)      505 2023-06-08 07:50:59.000000 lanelet2_parser-0.1.8/lanelet2_parser/exceptions.py
+drwxr-xr-x   0 iidayuuki   (501) staff       (20)        0 2023-06-08 08:26:03.968488 lanelet2_parser-0.1.8/lanelet2_parser/lanelet2/
+-rw-r--r--   0 iidayuuki   (501) staff       (20)        0 2023-06-08 07:50:59.000000 lanelet2_parser-0.1.8/lanelet2_parser/lanelet2/__init__.py
+-rw-r--r--   0 iidayuuki   (501) staff       (20)      120 2023-06-08 07:50:59.000000 lanelet2_parser-0.1.8/lanelet2_parser/lanelet2/config.py
+-rw-r--r--   0 iidayuuki   (501) staff       (20)     6749 2023-06-08 08:13:30.000000 lanelet2_parser-0.1.8/lanelet2_parser/lanelet2/converter.py
+-rw-r--r--   0 iidayuuki   (501) staff       (20)     6953 2023-06-08 08:13:27.000000 lanelet2_parser-0.1.8/lanelet2_parser/lanelet2/models.py
+-rw-r--r--   0 iidayuuki   (501) staff       (20)     8210 2023-06-08 07:50:59.000000 lanelet2_parser-0.1.8/lanelet2_parser/lanelet2/network.py
+drwxr-xr-x   0 iidayuuki   (501) staff       (20)        0 2023-06-08 08:26:03.975231 lanelet2_parser-0.1.8/lanelet2_parser/osm/
+-rw-r--r--   0 iidayuuki   (501) staff       (20)        0 2023-06-08 07:50:59.000000 lanelet2_parser-0.1.8/lanelet2_parser/osm/__init__.py
+-rw-r--r--   0 iidayuuki   (501) staff       (20)     3369 2023-06-08 07:50:59.000000 lanelet2_parser-0.1.8/lanelet2_parser/osm/models.py
+-rw-r--r--   0 iidayuuki   (501) staff       (20)      866 2023-06-08 07:50:59.000000 lanelet2_parser-0.1.8/lanelet2_parser/osm/validator.py
+-rw-r--r--   0 iidayuuki   (501) staff       (20)     4205 2023-06-08 07:50:59.000000 lanelet2_parser-0.1.8/lanelet2_parser/parser.py
+drwxr-xr-x   0 iidayuuki   (501) staff       (20)        0 2023-06-08 08:26:03.956751 lanelet2_parser-0.1.8/lanelet2_parser.egg-info/
+-rw-r--r--   0 iidayuuki   (501) staff       (20)     3695 2023-06-08 08:26:03.000000 lanelet2_parser-0.1.8/lanelet2_parser.egg-info/PKG-INFO
+-rw-r--r--   0 iidayuuki   (501) staff       (20)      584 2023-06-08 08:26:03.000000 lanelet2_parser-0.1.8/lanelet2_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 iidayuuki   (501) staff       (20)        1 2023-06-08 08:26:03.000000 lanelet2_parser-0.1.8/lanelet2_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 iidayuuki   (501) staff       (20)       18 2023-06-08 08:26:03.000000 lanelet2_parser-0.1.8/lanelet2_parser.egg-info/requires.txt
+-rw-r--r--   0 iidayuuki   (501) staff       (20)       16 2023-06-08 08:26:03.000000 lanelet2_parser-0.1.8/lanelet2_parser.egg-info/top_level.txt
+-rw-r--r--   0 iidayuuki   (501) staff       (20)       38 2023-06-08 08:26:03.978063 lanelet2_parser-0.1.8/setup.cfg
+-rw-r--r--   0 iidayuuki   (501) staff       (20)     1963 2023-06-08 07:50:59.000000 lanelet2_parser-0.1.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lanelet2_parser-0.1.7/PKG-INFO` & `lanelet2_parser-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanelet2_parser
-Version: 0.1.7
+Version: 0.1.8
 Summary: Parser for Lanelet2
 Home-page: https://github.com/tier4/lanelet2-parser
 Author: Yuki Iida
 Author-email: yuki.iida@tier4.jp
 License: BSD-3-Clause
 Description: # lanelet2-parser: Parser for Lanelet2
         
@@ -113,15 +113,15 @@
         - cancels: Lanelet
         - cancel_line: LineString
         
         LineStringRelation
         - prev_ids: List<Int>
         - next_ids: List<Int>
         
-        LaneletStringRelation
+        LaneletRelation
         - prev_ids: List<Int>
         - next_ids: List<Int>
         ```
         
         
 Keywords: Lanelet2,Parser,Autoware
 Platform: UNKNOWN
```

### Comparing `lanelet2_parser-0.1.7/README.md` & `lanelet2_parser-0.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -105,12 +105,12 @@
 - cancels: Lanelet
 - cancel_line: LineString
 
 LineStringRelation
 - prev_ids: List<Int>
 - next_ids: List<Int>
 
-LaneletStringRelation
+LaneletRelation
 - prev_ids: List<Int>
 - next_ids: List<Int>
 ```
```

### Comparing `lanelet2_parser-0.1.7/lanelet2_parser/lanelet2/converter.py` & `lanelet2_parser-0.1.8/lanelet2_parser/lanelet2/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,14 +113,20 @@
             parameters.right_of_way = ref
         elif member.role == "yield":
             parameters.param_yield = ref
         elif member.role == "cancels":
             parameters.cancels = ref
         elif member.role == "cancel_line":
             parameters.cancel_line = ref
+        elif member.role == "light_bulbs":
+            parameters.light_bulbs = ref
+        elif member.role == "start_line":
+            parameters.start_line = ref
+        elif member.role == "end_line":
+            parameters.end_line = ref
         else:
             print("Not Support role type. ", member.role)
     parameters.validate()
 
     return is_regulatory_element, subtype, attributes, parameters
 
 def is_lanelet(osm_relation):
```

### Comparing `lanelet2_parser-0.1.7/lanelet2_parser/lanelet2/models.py` & `lanelet2_parser-0.1.8/lanelet2_parser/lanelet2/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -152,28 +152,35 @@
             one_way=True if lanelet_attribute["one_way"] == "yes" else False,
             turn_direction=lanelet_attribute["turn_direction"],
             speed_limit=lanelet_attribute["speed_limit"],
         )
 
 
 class Parameter(Model):
-    refers = BaseType(required=True)
+    refers = BaseType(required=False)
     ref_line = BaseType(required=False)
     right_of_way = BaseType(required=False)
     param_yield = BaseType(required=False)
     cancels = BaseType(required=False)
     cancel_line = BaseType(required=False)
+    light_bulbs = BaseType(required=False)
+    start_line = BaseType(required=False)
+    end_line = BaseType(required=False)
 
     def __init__(self):
         super(Parameter, self).__init__()
         self.refers = None
         self.ref_line = None
         self.param_yield = None
         self.cancels = None
         self.cancel_line = None
+        self.light_bulbs = None
+        self.start_line = None
+        self.end_line = None
+        
 
 class RegulatoryElement(Model):
     '''
     RegulatoryElement
     '''
     id = IntType(required=True)
     subtype = StringType(required=True)
@@ -209,13 +216,17 @@
 
 class LaneletRelation(Model):
     '''
     Lanelet Relation
     '''
     prev_ids = ListType(IntType)
     next_ids = ListType(IntType)
+    left_ids = ListType(IntType)
+    right_ids = ListType(IntType)
 
-    def __init__(self, prev_ids, next_ids):
+    def __init__(self, prev_ids, next_ids, left_ids, right_ids):
         super(LaneletRelation, self).__init__()
         self.prev_ids = prev_ids
         self.next_ids = next_ids
+        self.left_ids = left_ids
+        self.right_ids = right_ids
         self.validate()
```

### Comparing `lanelet2_parser-0.1.7/lanelet2_parser/lanelet2/network.py` & `lanelet2_parser-0.1.8/lanelet2_parser/lanelet2/network.py`

 * *Files 26% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     :param osm_data:
     :param line_string_relations:
     :return lanelet_relations:
     '''
     lanelet_relations = {}
     lanelet_way_relation = {}  # {lanelet_id: {"left_way_id": way_id, "right_way_id": way_id}}
     way_lanelet_relation = {}  # {(left_way_id or right_way_id): lanelet_id}
+    way_LR_lanelet_relation = {}  # {way_id: {"left_lanelet_id": [lanelet_id], "right_lanelet_id": [lanelet_id]}}
 
     # (way_id) => lanelet_id の関係を算出
     for relation_id, relation in osm_data.relations.items():
         is_lanelet = False
         # check type of relations
         for tag in relation.tags:
             if tag.key == "type" and tag.value == "lanelet":
@@ -76,18 +77,22 @@
         # create lanelet_way_relation
         if relation_id not in lanelet_way_relation:
             lanelet_way_relation[relation_id] = {
                 "left_way_id": None,
                 "right_way_id": None
             }
         for member in relation.members:
+            if member.ref not in way_LR_lanelet_relation:
+                way_LR_lanelet_relation[member.ref] = {"right_lanelet_id": [], "left_lanelet_id": []}
             if member.role == "left" and member.type == "way":
                 lanelet_way_relation[relation_id]["left_way_id"] = member.ref
+                way_LR_lanelet_relation[member.ref]["right_lanelet_id"].append(relation_id)
             elif member.role == "right" and member.type == "way":
                 lanelet_way_relation[relation_id]["right_way_id"] = member.ref
+                way_LR_lanelet_relation[member.ref]["left_lanelet_id"].append(relation_id)
         # raise error if left/right way id is none
         if lanelet_way_relation[relation_id]["left_way_id"] == None or \
                 lanelet_way_relation[relation_id]["right_way_id"] == None:
             raise InvalidMapDateError("Lanelet's left, right way are not found.")
 
         # create way lanelet relation
         if left_hand_traffic is True:
@@ -99,27 +104,35 @@
     for lanelet_id, lanelet_way_id in lanelet_way_relation.items():
         if lanelet_way_id["left_way_id"] not in line_string_relations or lanelet_way_id["right_way_id"] not in line_string_relations:
             raise MissingResourceError("Way is not found.")
 
         target_line_string_relations = line_string_relations[lanelet_way_id["left_way_id"]] if left_hand_traffic is True else line_string_relations[lanelet_way_id["right_way_id"]]
         prev_ids = []
         next_ids = []
-
+        left_ids = []
+        right_ids = []
         # prev lanelet
         for prev_way_id in target_line_string_relations["prev_ids"]:
             if prev_way_id in way_lanelet_relation:
                 prev_ids.append(way_lanelet_relation[prev_way_id])
         # next lanelet
         for next_way_id in target_line_string_relations["next_ids"]:
             if next_way_id in way_lanelet_relation:
                 next_ids.append(way_lanelet_relation[next_way_id])
+        # left lanelet
+        if "right_lanelet_id" in way_LR_lanelet_relation[lanelet_way_id["left_way_id"]]:
+            left_ids = way_LR_lanelet_relation[lanelet_way_id["left_way_id"]]["left_lanelet_id"]
+        if "left_lanelet_id" in way_LR_lanelet_relation[lanelet_way_id["right_way_id"]]:
+            right_ids = way_LR_lanelet_relation[lanelet_way_id["right_way_id"]]["right_lanelet_id"]
         # set lanelet relation
         lanelet_relations[lanelet_id] = LaneletRelation(
             prev_ids=prev_ids,
-            next_ids=next_ids
+            next_ids=next_ids,
+            left_ids=left_ids,
+            right_ids=right_ids
         )
     return lanelet_relations
 
 
 def validate_line_string_network(line_string_relations, osm_data):
     # check size
     # if len(line_string_relations.keys()) != len(osm_data.ways.keys()):
```

### Comparing `lanelet2_parser-0.1.7/lanelet2_parser/osm/models.py` & `lanelet2_parser-0.1.8/lanelet2_parser/osm/models.py`

 * *Files identical despite different names*

### Comparing `lanelet2_parser-0.1.7/lanelet2_parser/osm/validator.py` & `lanelet2_parser-0.1.8/lanelet2_parser/osm/validator.py`

 * *Files identical despite different names*

### Comparing `lanelet2_parser-0.1.7/lanelet2_parser/parser.py` & `lanelet2_parser-0.1.8/lanelet2_parser/parser.py`

 * *Files identical despite different names*

### Comparing `lanelet2_parser-0.1.7/lanelet2_parser.egg-info/PKG-INFO` & `lanelet2_parser-0.1.8/lanelet2_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanelet2-parser
-Version: 0.1.7
+Version: 0.1.8
 Summary: Parser for Lanelet2
 Home-page: https://github.com/tier4/lanelet2-parser
 Author: Yuki Iida
 Author-email: yuki.iida@tier4.jp
 License: BSD-3-Clause
 Description: # lanelet2-parser: Parser for Lanelet2
         
@@ -113,15 +113,15 @@
         - cancels: Lanelet
         - cancel_line: LineString
         
         LineStringRelation
         - prev_ids: List<Int>
         - next_ids: List<Int>
         
-        LaneletStringRelation
+        LaneletRelation
         - prev_ids: List<Int>
         - next_ids: List<Int>
         ```
         
         
 Keywords: Lanelet2,Parser,Autoware
 Platform: UNKNOWN
```

### Comparing `lanelet2_parser-0.1.7/lanelet2_parser.egg-info/SOURCES.txt` & `lanelet2_parser-0.1.8/lanelet2_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lanelet2_parser-0.1.7/setup.py` & `lanelet2_parser-0.1.8/setup.py`

 * *Files identical despite different names*

