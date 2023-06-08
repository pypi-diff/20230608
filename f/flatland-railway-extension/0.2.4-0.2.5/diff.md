# Comparing `tmp/flatland-railway-extension-0.2.4.tar.gz` & `tmp/flatland-railway-extension-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatland-railway-extension-0.2.4.tar", last modified: Wed Jun  7 04:57:12 2023, max compression
+gzip compressed data, was "dist\flatland-railway-extension-0.2.5.tar", last modified: Thu Jun  8 07:40:50 2023, max compression
```

## Comparing `flatland-railway-extension-0.2.4.tar` & `flatland-railway-extension-0.2.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 04:57:12.736353 flatland-railway-extension-0.2.4/
--rw-rw-rw-   0        0        0     1214 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      405 2023-06-07 04:57:12.736353 flatland-railway-extension-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    14346 2023-05-09 20:30:03.000000 flatland-railway-extension-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 04:57:12.688912 flatland-railway-extension-0.2.4/flatland_railway_extension/
--rw-rw-rw-   0        0        0     3133 2023-06-01 07:54:21.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/FlatlandEnvironmentHelper.py
--rw-rw-rw-   0        0        0    17639 2023-06-07 04:54:43.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/FlatlandGraphBuilder.py
--rw-rw-rw-   0        0        0     7805 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/RailroadSwitchAnalyser.py
--rw-rw-rw-   0        0        0     9991 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/RailroadSwitchCluster.py
--rw-rw-rw-   0        0        0       25 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 04:57:12.705095 flatland-railway-extension-0.2.4/flatland_railway_extension/environments/
--rw-rw-rw-   0        0        0    21375 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/environments/DynamicAgent.py
--rw-rw-rw-   0        0        0      686 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/environments/DynamicsResourceData.py
--rw-rw-rw-   0        0        0    10121 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/environments/FlatlandDynamics.py
--rw-rw-rw-   0        0        0     4829 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/environments/FlatlandDynamicsDistanceMap.py
--rw-rw-rw-   0        0        0     8950 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/environments/FlatlandResourceAllocator.py
--rw-rw-rw-   0        0        0     1682 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/environments/InfrastructureData.py
--rw-rw-rw-   0        0        0     1511 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/environments/MultiResourcesAllocationAgent.py
--rw-rw-rw-   0        0        0     8028 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/environments/MultiResourcesAllocationRailEnv.py
--rw-rw-rw-   0        0        0     5009 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/environments/RollingStock.py
--rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/environments/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 04:57:12.720727 flatland-railway-extension-0.2.4/flatland_railway_extension/examples/
--rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 04:57:12.720727 flatland-railway-extension-0.2.4/flatland_railway_extension/examples/data_exports/
--rw-rw-rw-   0        0        0     6857 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/examples/data_exports/FlatlandRecifeExporter.py
--rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/examples/data_exports/__init__.py
--rw-rw-rw-   0        0        0     7031 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/examples/demo_flatland_dynamics.py
--rw-rw-rw-   0        0        0     4913 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/examples/demo_flatland_extensions.py
--rw-rw-rw-   0        0        0     3981 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/examples/demo_flatland_graph.py
--rw-rw-rw-   0        0        0     2857 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/examples/demo_flatland_railroad_cluster.py
--rw-rw-rw-   0        0        0     6927 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/examples/demo_simple_flatland_navigation.py
-drwxrwxrwx   0        0        0        0 2023-06-07 04:57:12.736353 flatland-railway-extension-0.2.4/flatland_railway_extension/utils/
--rw-rw-rw-   0        0        0     5982 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/utils/FlatlandDynamicsRenderer.py
--rw-rw-rw-   0        0        0     6048 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/utils/FlatlandRenderer.py
--rw-rw-rw-   0        0        0     2200 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/utils/ShortestPathNextStepObservation.py
--rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/utils/__init__.py
--rw-rw-rw-   0        0        0      248 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.4/flatland_railway_extension/utils/cached_methods.py
-drwxrwxrwx   0        0        0        0 2023-06-07 04:57:12.688912 flatland-railway-extension-0.2.4/flatland_railway_extension.egg-info/
--rw-rw-rw-   0        0        0      405 2023-06-07 04:57:12.000000 flatland-railway-extension-0.2.4/flatland_railway_extension.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1952 2023-06-07 04:57:12.000000 flatland-railway-extension-0.2.4/flatland_railway_extension.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 04:57:12.000000 flatland-railway-extension-0.2.4/flatland_railway_extension.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-07 04:57:12.000000 flatland-railway-extension-0.2.4/flatland_railway_extension.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-06-07 04:57:12.000000 flatland-railway-extension-0.2.4/flatland_railway_extension.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 04:57:12.736353 flatland-railway-extension-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-06-07 04:56:49.000000 flatland-railway-extension-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:40:50.000000 flatland-railway-extension-0.2.5/
+-rw-rw-rw-   0        0        0     1214 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-06-08 07:40:50.000000 flatland-railway-extension-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    14346 2023-05-09 20:30:03.000000 flatland-railway-extension-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 07:40:50.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/
+-rw-rw-rw-   0        0        0     3133 2023-06-01 07:54:21.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/FlatlandEnvironmentHelper.py
+-rw-rw-rw-   0        0        0    18414 2023-06-08 07:39:10.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/FlatlandGraphBuilder.py
+-rw-rw-rw-   0        0        0     7805 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/RailroadSwitchAnalyser.py
+-rw-rw-rw-   0        0        0     9991 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/RailroadSwitchCluster.py
+-rw-rw-rw-   0        0        0       25 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:40:50.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/environments/
+-rw-rw-rw-   0        0        0    21375 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/environments/DynamicAgent.py
+-rw-rw-rw-   0        0        0      686 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/environments/DynamicsResourceData.py
+-rw-rw-rw-   0        0        0    10121 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/environments/FlatlandDynamics.py
+-rw-rw-rw-   0        0        0     4829 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/environments/FlatlandDynamicsDistanceMap.py
+-rw-rw-rw-   0        0        0     8950 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/environments/FlatlandResourceAllocator.py
+-rw-rw-rw-   0        0        0     1682 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/environments/InfrastructureData.py
+-rw-rw-rw-   0        0        0     1511 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/environments/MultiResourcesAllocationAgent.py
+-rw-rw-rw-   0        0        0     8028 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/environments/MultiResourcesAllocationRailEnv.py
+-rw-rw-rw-   0        0        0     5009 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/environments/RollingStock.py
+-rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/environments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:40:50.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/examples/
+-rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:40:50.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/examples/data_exports/
+-rw-rw-rw-   0        0        0     6857 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/examples/data_exports/FlatlandRecifeExporter.py
+-rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/examples/data_exports/__init__.py
+-rw-rw-rw-   0        0        0     7031 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/examples/demo_flatland_dynamics.py
+-rw-rw-rw-   0        0        0     4913 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/examples/demo_flatland_extensions.py
+-rw-rw-rw-   0        0        0     3981 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/examples/demo_flatland_graph.py
+-rw-rw-rw-   0        0        0     2857 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/examples/demo_flatland_railroad_cluster.py
+-rw-rw-rw-   0        0        0     6927 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/examples/demo_simple_flatland_navigation.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:40:50.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/utils/
+-rw-rw-rw-   0        0        0     5982 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/utils/FlatlandDynamicsRenderer.py
+-rw-rw-rw-   0        0        0     6048 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/utils/FlatlandRenderer.py
+-rw-rw-rw-   0        0        0     2200 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/utils/ShortestPathNextStepObservation.py
+-rw-rw-rw-   0        0        0        0 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/utils/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-04-22 06:40:26.000000 flatland-railway-extension-0.2.5/flatland_railway_extension/utils/cached_methods.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:40:50.000000 flatland-railway-extension-0.2.5/flatland_railway_extension.egg-info/
+-rw-rw-rw-   0        0        0      405 2023-06-08 07:40:50.000000 flatland-railway-extension-0.2.5/flatland_railway_extension.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1952 2023-06-08 07:40:50.000000 flatland-railway-extension-0.2.5/flatland_railway_extension.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 07:40:50.000000 flatland-railway-extension-0.2.5/flatland_railway_extension.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-08 07:40:50.000000 flatland-railway-extension-0.2.5/flatland_railway_extension.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-08 07:40:50.000000 flatland-railway-extension-0.2.5/flatland_railway_extension.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 07:40:50.000000 flatland-railway-extension-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      762 2023-06-08 07:40:38.000000 flatland-railway-extension-0.2.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `flatland-railway-extension-0.2.4/LICENSE` & `flatland-railway-extension-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/README.md` & `flatland-railway-extension-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/FlatlandEnvironmentHelper.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/FlatlandEnvironmentHelper.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/FlatlandGraphBuilder.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/FlatlandGraphBuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Dict, Tuple, List
 from typing import Union
 
 import networkx as nx
 import numpy as np
 # import all flatland dependance
 from flatland.core.grid.grid4_utils import get_new_position
-from flatland.envs.fast_methods import fast_position_equal, fast_argmax
+from flatland.envs.fast_methods import fast_position_equal, fast_argmax, fast_count_nonzero
 from matplotlib import pyplot as plt
 from networkx.classes.reportviews import OutEdgeView
 
 from flatland_railway_extension.RailroadSwitchAnalyser import RailroadSwitchAnalyser
 from flatland_railway_extension.environments.InfrastructureData import InfrastructureData
 
 
@@ -65,32 +65,43 @@
     def _create_full_graph(self):
         graph = nx.DiGraph()
         env = self.railroad_switch_analyser.get_rail_env()
         nodes = {}
         from_vertex_edge_map = {}
         for h in range(env.height):
             for w in range(env.width):
-                pos = (h, w)
+                from_position = (h, w)
                 for from_direction in range(4):
-                    possible_transitions = env.rail.get_transitions(*pos, from_direction)
-                    for to_direction in range(4):
-                        if possible_transitions[to_direction] == 1:
-                            new_position = get_new_position(pos, to_direction)
-                            from_vertex_name = '{}_{}_{}'.format(pos[0], pos[1], from_direction)
-                            to_vertex_name = '{}_{}_{}'.format(new_position[0], new_position[1], to_direction)
-                            graph.add_edge(from_vertex_name,
-                                           to_vertex_name,
-                                           length=self.estimate_edge_len(pos),
-                                           from_nodes=[from_vertex_name],
-                                           resources=[pos],
-                                           resource_id='{}_{}'.format(pos[0], pos[1])
-                                           )
-                            nodes.update({from_vertex_name: (pos[0], pos[1], from_direction)})
-                            nodes.update({to_vertex_name: (new_position[0], new_position[1], to_direction)})
-                            from_vertex_edge_map.update({from_vertex_name: (from_vertex_name, to_vertex_name)})
+                    possible_transitions = env.rail.get_transitions(*from_position, from_direction)
+                    if fast_count_nonzero(possible_transitions):
+                        actions = {}
+                        idx = 0
+                        for direction in [(from_direction + i) % 4 for i in range(-1, 2)]:
+                            if possible_transitions[direction]:
+                                actions.update({direction: idx})
+                            else:
+                                actions.update({direction: idx})
+                            idx += 1
+
+                        for to_direction in range(4):
+                            if possible_transitions[to_direction] == 1:
+                                new_position = get_new_position(from_position, to_direction)
+                                from_vertex_name = '{}_{}_{}'.format(from_position[0], from_position[1], from_direction)
+                                to_vertex_name = '{}_{}_{}'.format(new_position[0], new_position[1], to_direction)
+                                graph.add_edge(from_vertex_name,
+                                               to_vertex_name,
+                                               length=self.estimate_edge_len(from_position),
+                                               from_nodes=[from_vertex_name],
+                                               resources=[from_position],
+                                               action=[actions.get(to_direction)],
+                                               resource_id='{}_{}'.format(from_position[0], from_position[1])
+                                               )
+                                nodes.update({from_vertex_name: (from_position[0], from_position[1], from_direction)})
+                                nodes.update({to_vertex_name: (new_position[0], new_position[1], to_direction)})
+                                from_vertex_edge_map.update({from_vertex_name: (from_vertex_name, to_vertex_name)})
 
         return graph, nodes, from_vertex_edge_map
 
     def _create_simplified_graph(self):
         self._graph, self._nodes, self._from_vertex_edge_map = self._create_full_graph()
         graph, nodes, from_vertex_edge_map = self._graph, self._nodes, self._from_vertex_edge_map
         # loop as long as the graph changes (gets updated)
```

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/RailroadSwitchAnalyser.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/RailroadSwitchAnalyser.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/RailroadSwitchCluster.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/RailroadSwitchCluster.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/environments/DynamicAgent.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/environments/DynamicAgent.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/environments/DynamicsResourceData.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/environments/DynamicsResourceData.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/environments/FlatlandDynamics.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/environments/FlatlandDynamics.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/environments/FlatlandDynamicsDistanceMap.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/environments/FlatlandDynamicsDistanceMap.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/environments/FlatlandResourceAllocator.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/environments/FlatlandResourceAllocator.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/environments/InfrastructureData.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/environments/InfrastructureData.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/environments/MultiResourcesAllocationAgent.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/environments/MultiResourcesAllocationAgent.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/environments/MultiResourcesAllocationRailEnv.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/environments/MultiResourcesAllocationRailEnv.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/environments/RollingStock.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/environments/RollingStock.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/examples/data_exports/FlatlandRecifeExporter.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/examples/data_exports/FlatlandRecifeExporter.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/examples/demo_flatland_dynamics.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/examples/demo_flatland_dynamics.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/examples/demo_flatland_extensions.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/examples/demo_flatland_extensions.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/examples/demo_flatland_graph.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/examples/demo_flatland_graph.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/examples/demo_flatland_railroad_cluster.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/examples/demo_flatland_railroad_cluster.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/examples/demo_simple_flatland_navigation.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/examples/demo_simple_flatland_navigation.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/utils/FlatlandDynamicsRenderer.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/utils/FlatlandDynamicsRenderer.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/utils/FlatlandRenderer.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/utils/FlatlandRenderer.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension/utils/ShortestPathNextStepObservation.py` & `flatland-railway-extension-0.2.5/flatland_railway_extension/utils/ShortestPathNextStepObservation.py`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/flatland_railway_extension.egg-info/SOURCES.txt` & `flatland-railway-extension-0.2.5/flatland_railway_extension.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatland-railway-extension-0.2.4/setup.py` & `flatland-railway-extension-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # twine upload dist/*
 
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name='flatland-railway-extension',
-    version='0.2.4',
+    version='0.2.5',
     author='Adrian Egli',
     author_email="3dhelp@gmail.com",
     description='Extends Flatland Railway Simulator with helpful features.',
     url='https://github.com/aiAdrian/flatland_railway_extension',
     keywords='flatland, railway, extension, dynamics, simulation, multi-agent, reinforcement learning',
     python_requires='>=3.6, <4',
     packages=find_packages('.'),
```

