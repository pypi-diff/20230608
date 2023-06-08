# Comparing `tmp/modular_rl-0.3.1.tar.gz` & `tmp/modular_rl-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modular_rl-0.3.1.tar", last modified: Tue Jun  6 22:51:54 2023, max compression
+gzip compressed data, was "modular_rl-0.3.2.tar", last modified: Thu Jun  8 11:25:20 2023, max compression
```

## Comparing `modular_rl-0.3.1.tar` & `modular_rl-0.3.2.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.852496 modular_rl-0.3.1/
--rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     5670 2023-06-06 22:51:54.852496 modular_rl-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4164 2023-06-06 22:51:16.000000 modular_rl-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.794867 modular_rl-0.3.1/modular_rl/
--rw-rw-rw-   0        0        0       37 2023-05-07 14:51:41.000000 modular_rl-0.3.1/modular_rl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.812342 modular_rl-0.3.1/modular_rl/agents/
--rw-rw-rw-   0        0        0      108 2023-06-06 21:28:14.000000 modular_rl-0.3.1/modular_rl/agents/__init__.py
--rw-rw-rw-   0        0        0     9544 2023-06-06 21:33:56.000000 modular_rl-0.3.1/modular_rl/agents/_agent.py
--rw-rw-rw-   0        0        0     4838 2023-06-06 21:35:21.000000 modular_rl-0.3.1/modular_rl/agents/_custom.py
--rw-rw-rw-   0        0        0    12360 2023-06-06 21:42:41.000000 modular_rl-0.3.1/modular_rl/agents/mcis.py
--rw-rw-rw-   0        0        0    11964 2023-05-07 14:51:41.000000 modular_rl-0.3.1/modular_rl/agents/mcts.py
--rw-rw-rw-   0        0        0    20686 2023-06-06 22:24:07.000000 modular_rl-0.3.1/modular_rl/agents/mim.py
--rw-rw-rw-   0        0        0    14958 2023-06-06 21:36:06.000000 modular_rl-0.3.1/modular_rl/agents/ppo.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.814474 modular_rl-0.3.1/modular_rl/envs/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/envs/__init__.py
--rw-rw-rw-   0        0        0      133 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/envs/_custom.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.817646 modular_rl-0.3.1/modular_rl/envs/mim/
--rw-rw-rw-   0        0        0       25 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/envs/mim/__init__.py
--rw-rw-rw-   0        0        0    15402 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/envs/mim/card_evaluator.py
--rw-rw-rw-   0        0        0     4474 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/envs/mim/mim.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.823543 modular_rl-0.3.1/modular_rl/networks/
--rw-rw-rw-   0        0        0       68 2023-05-07 14:51:41.000000 modular_rl-0.3.1/modular_rl/networks/__init__.py
--rw-rw-rw-   0        0        0     2174 2023-05-07 14:51:41.000000 modular_rl-0.3.1/modular_rl/networks/actor_critic.py
--rw-rw-rw-   0        0        0     2878 2023-05-04 23:35:18.000000 modular_rl-0.3.1/modular_rl/networks/policy.py
--rw-rw-rw-   0        0        0     2688 2023-05-04 23:33:52.000000 modular_rl-0.3.1/modular_rl/networks/value.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.832480 modular_rl-0.3.1/modular_rl/params/
--rw-rw-rw-   0        0        0       85 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/params/__init__.py
--rw-rw-rw-   0        0        0     2161 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/params/mcis.py
--rw-rw-rw-   0        0        0     2345 2023-05-07 14:51:41.000000 modular_rl-0.3.1/modular_rl/params/mcts.py
--rw-rw-rw-   0        0        0     1938 2023-06-06 22:34:44.000000 modular_rl-0.3.1/modular_rl/params/mim.py
--rw-rw-rw-   0        0        0     2053 2023-05-07 14:51:41.000000 modular_rl-0.3.1/modular_rl/params/ppo.py
--rw-rw-rw-   0        0        0     1377 2023-06-06 22:36:03.000000 modular_rl-0.3.1/modular_rl/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.838130 modular_rl-0.3.1/modular_rl/tester/
--rw-rw-rw-   0        0        0       61 2023-05-07 14:51:41.000000 modular_rl-0.3.1/modular_rl/tester/__init__.py
--rw-rw-rw-   0        0        0      978 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/tester/mcis.py
--rw-rw-rw-   0        0        0      366 2023-05-07 14:51:41.000000 modular_rl-0.3.1/modular_rl/tester/mcts.py
--rw-rw-rw-   0        0        0      689 2023-06-06 22:45:16.000000 modular_rl-0.3.1/modular_rl/tester/mim.py
--rw-rw-rw-   0        0        0     1552 2023-05-05 00:05:02.000000 modular_rl-0.3.1/modular_rl/tester/ppo.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.840339 modular_rl-0.3.1/modular_rl/util/
--rw-rw-rw-   0        0        0        0 2023-05-04 23:35:52.000000 modular_rl-0.3.1/modular_rl/util/__init__.py
--rw-rw-rw-   0        0        0     2533 2023-06-04 21:09:01.000000 modular_rl-0.3.1/modular_rl/util/node.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.802163 modular_rl-0.3.1/modular_rl.egg-info/
--rw-rw-rw-   0        0        0     5670 2023-06-06 22:51:54.000000 modular_rl-0.3.1/modular_rl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1193 2023-06-06 22:51:54.000000 modular_rl-0.3.1/modular_rl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 22:51:54.000000 modular_rl-0.3.1/modular_rl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-06 22:51:54.000000 modular_rl-0.3.1/modular_rl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-06 22:51:54.000000 modular_rl-0.3.1/modular_rl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1414 2023-06-06 22:51:47.000000 modular_rl-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 22:51:54.852496 modular_rl-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-06-06 22:51:40.000000 modular_rl-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:51:54.851292 modular_rl-0.3.1/tests/
--rw-rw-rw-   0        0        0       97 2023-06-04 21:09:01.000000 modular_rl-0.3.1/tests/test_mcis.py
--rw-rw-rw-   0        0        0      105 2023-06-04 21:09:01.000000 modular_rl-0.3.1/tests/test_mcis_modular.py
--rw-rw-rw-   0        0        0       97 2023-05-07 14:51:41.000000 modular_rl-0.3.1/tests/test_mcts.py
--rw-rw-rw-   0        0        0      107 2023-06-04 21:09:01.000000 modular_rl-0.3.1/tests/test_mim.py
--rw-rw-rw-   0        0        0      111 2023-06-06 22:42:10.000000 modular_rl-0.3.1/tests/test_mim_modular.py
--rw-rw-rw-   0        0        0       61 2023-05-05 10:03:21.000000 modular_rl-0.3.1/tests/test_ppo.py
--rw-rw-rw-   0        0        0       69 2023-05-05 10:03:28.000000 modular_rl-0.3.1/tests/test_ppo_modular.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.557843 modular_rl-0.3.2/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     5688 2023-06-08 11:25:20.555754 modular_rl-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4182 2023-06-08 11:09:02.000000 modular_rl-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.478416 modular_rl-0.3.2/modular_rl/
+-rw-rw-rw-   0        0        0       37 2023-05-07 14:51:41.000000 modular_rl-0.3.2/modular_rl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.497466 modular_rl-0.3.2/modular_rl/agents/
+-rw-rw-rw-   0        0        0      108 2023-06-06 21:28:14.000000 modular_rl-0.3.2/modular_rl/agents/__init__.py
+-rw-rw-rw-   0        0        0    10432 2023-06-07 12:17:24.000000 modular_rl-0.3.2/modular_rl/agents/_agent.py
+-rw-rw-rw-   0        0        0     4838 2023-06-06 21:35:21.000000 modular_rl-0.3.2/modular_rl/agents/_custom.py
+-rw-rw-rw-   0        0        0    11741 2023-06-08 11:22:46.000000 modular_rl-0.3.2/modular_rl/agents/mcis.py
+-rw-rw-rw-   0        0        0    12121 2023-06-07 22:13:39.000000 modular_rl-0.3.2/modular_rl/agents/mcts.py
+-rw-rw-rw-   0        0        0    20686 2023-06-06 22:24:07.000000 modular_rl-0.3.2/modular_rl/agents/mim.py
+-rw-rw-rw-   0        0        0    14958 2023-06-06 21:36:06.000000 modular_rl-0.3.2/modular_rl/agents/ppo.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.500609 modular_rl-0.3.2/modular_rl/envs/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:09:01.000000 modular_rl-0.3.2/modular_rl/envs/__init__.py
+-rw-rw-rw-   0        0        0      133 2023-06-04 21:09:01.000000 modular_rl-0.3.2/modular_rl/envs/_custom.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.505421 modular_rl-0.3.2/modular_rl/envs/mim/
+-rw-rw-rw-   0        0        0       25 2023-06-04 21:09:01.000000 modular_rl-0.3.2/modular_rl/envs/mim/__init__.py
+-rw-rw-rw-   0        0        0    15402 2023-06-04 21:09:01.000000 modular_rl-0.3.2/modular_rl/envs/mim/card_evaluator.py
+-rw-rw-rw-   0        0        0     4474 2023-06-04 21:09:01.000000 modular_rl-0.3.2/modular_rl/envs/mim/mim.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.510270 modular_rl-0.3.2/modular_rl/networks/
+-rw-rw-rw-   0        0        0       68 2023-05-07 14:51:41.000000 modular_rl-0.3.2/modular_rl/networks/__init__.py
+-rw-rw-rw-   0        0        0     2174 2023-05-07 14:51:41.000000 modular_rl-0.3.2/modular_rl/networks/actor_critic.py
+-rw-rw-rw-   0        0        0     2878 2023-05-04 23:35:18.000000 modular_rl-0.3.2/modular_rl/networks/policy.py
+-rw-rw-rw-   0        0        0     2688 2023-05-04 23:33:52.000000 modular_rl-0.3.2/modular_rl/networks/value.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.519638 modular_rl-0.3.2/modular_rl/params/
+-rw-rw-rw-   0        0        0       85 2023-06-04 21:09:01.000000 modular_rl-0.3.2/modular_rl/params/__init__.py
+-rw-rw-rw-   0        0        0     2161 2023-06-04 21:09:01.000000 modular_rl-0.3.2/modular_rl/params/mcis.py
+-rw-rw-rw-   0        0        0     2294 2023-06-08 11:07:34.000000 modular_rl-0.3.2/modular_rl/params/mcts.py
+-rw-rw-rw-   0        0        0     1938 2023-06-06 22:34:44.000000 modular_rl-0.3.2/modular_rl/params/mim.py
+-rw-rw-rw-   0        0        0     2053 2023-05-07 14:51:41.000000 modular_rl-0.3.2/modular_rl/params/ppo.py
+-rw-rw-rw-   0        0        0     1377 2023-06-06 22:36:03.000000 modular_rl-0.3.2/modular_rl/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.531473 modular_rl-0.3.2/modular_rl/tester/
+-rw-rw-rw-   0        0        0       61 2023-05-07 14:51:41.000000 modular_rl-0.3.2/modular_rl/tester/__init__.py
+-rw-rw-rw-   0        0        0     1036 2023-06-07 12:42:45.000000 modular_rl-0.3.2/modular_rl/tester/mcis.py
+-rw-rw-rw-   0        0        0     1270 2023-06-07 21:24:00.000000 modular_rl-0.3.2/modular_rl/tester/mcts.py
+-rw-rw-rw-   0        0        0      689 2023-06-06 22:45:16.000000 modular_rl-0.3.2/modular_rl/tester/mim.py
+-rw-rw-rw-   0        0        0     1552 2023-05-05 00:05:02.000000 modular_rl-0.3.2/modular_rl/tester/ppo.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.536152 modular_rl-0.3.2/modular_rl/util/
+-rw-rw-rw-   0        0        0        0 2023-05-04 23:35:52.000000 modular_rl-0.3.2/modular_rl/util/__init__.py
+-rw-rw-rw-   0        0        0     2533 2023-06-04 21:09:01.000000 modular_rl-0.3.2/modular_rl/util/node.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.488046 modular_rl-0.3.2/modular_rl.egg-info/
+-rw-rw-rw-   0        0        0     5688 2023-06-08 11:25:20.000000 modular_rl-0.3.2/modular_rl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1220 2023-06-08 11:25:20.000000 modular_rl-0.3.2/modular_rl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 11:25:20.000000 modular_rl-0.3.2/modular_rl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-08 11:25:20.000000 modular_rl-0.3.2/modular_rl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-08 11:25:20.000000 modular_rl-0.3.2/modular_rl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1414 2023-06-08 11:25:03.000000 modular_rl-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-08 11:25:20.557843 modular_rl-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-06-08 11:25:15.000000 modular_rl-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:25:20.554725 modular_rl-0.3.2/tests/
+-rw-rw-rw-   0        0        0       97 2023-06-04 21:09:01.000000 modular_rl-0.3.2/tests/test_mcis.py
+-rw-rw-rw-   0        0        0      105 2023-06-04 21:09:01.000000 modular_rl-0.3.2/tests/test_mcis_modular.py
+-rw-rw-rw-   0        0        0       97 2023-05-07 14:51:41.000000 modular_rl-0.3.2/tests/test_mcts.py
+-rw-rw-rw-   0        0        0      101 2023-06-07 12:43:41.000000 modular_rl-0.3.2/tests/test_mcts_modular.py
+-rw-rw-rw-   0        0        0      107 2023-06-04 21:09:01.000000 modular_rl-0.3.2/tests/test_mim.py
+-rw-rw-rw-   0        0        0      111 2023-06-06 22:42:10.000000 modular_rl-0.3.2/tests/test_mim_modular.py
+-rw-rw-rw-   0        0        0       61 2023-05-05 10:03:21.000000 modular_rl-0.3.2/tests/test_ppo.py
+-rw-rw-rw-   0        0        0       69 2023-05-05 10:03:28.000000 modular_rl-0.3.2/tests/test_ppo_modular.py
```

### Comparing `modular_rl-0.3.1/LICENSE` & `modular_rl-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.1/PKG-INFO` & `modular_rl-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modular_rl
-Version: 0.3.1
+Version: 0.3.2
 Summary: ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
 Home-page: https://github.com/horrible-gh/ModularRL
 Author: sjm
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/ModularRL
 Project-URL: Bug Tracker, https://github.com/horrible-gh/ModularRL/issues
 Keywords: ModularRL,Modular-RL,Modular_RL,Modular RL,modularrl,modular_rl,modular-rl,modular rl,mrl,modular,learn,learning,pytorch learn,pytorch learning
@@ -45,18 +45,18 @@
 -   Proximal Policy Optimization (PPO)
 -   Monte Carlo Tree Search (MCTS)
 -   Monte Carlo Information Set (MCIS)
 -   Modular's sIMulator (MIM)
 
 Refer to the respective agent classes for each algorithm:
 
--   AgentPPO (Modular)
--   AgentMCTS
--   AgentMCIS (Modular)
--   AgentMIM (Modular)
+-   AgentPPO (+ Modular)
+-   AgentMCTS (+ Modular)
+-   AgentMCIS (+ Modular)
+-   AgentMIM (+ Modular)
 
 ## Example Usage
 
 You can use the tester.py script provided in the library to create and train an instance of an agent with default or modified settings:
 
 ```python
 import modular_rl.tester as tester
```

### Comparing `modular_rl-0.3.1/README.md` & `modular_rl-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 -   Proximal Policy Optimization (PPO)
 -   Monte Carlo Tree Search (MCTS)
 -   Monte Carlo Information Set (MCIS)
 -   Modular's sIMulator (MIM)
 
 Refer to the respective agent classes for each algorithm:
 
--   AgentPPO (Modular)
--   AgentMCTS
--   AgentMCIS (Modular)
--   AgentMIM (Modular)
+-   AgentPPO (+ Modular)
+-   AgentMCTS (+ Modular)
+-   AgentMCIS (+ Modular)
+-   AgentMIM (+ Modular)
 
 ## Example Usage
 
 You can use the tester.py script provided in the library to create and train an instance of an agent with default or modified settings:
 
 ```python
 import modular_rl.tester as tester
```

### Comparing `modular_rl-0.3.1/modular_rl/agents/_agent.py` & `modular_rl-0.3.2/modular_rl/agents/_agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -175,14 +175,41 @@
 
         update() function is a placeholder that needs to be implemented in the child class that extends the Agent class. This function is responsible for updating the agent's state, action, and policy based on the new state and reward received from the environment.
 
         No parameters are passed into this function and it does not return anything.
         '''
         pass
 
+    def update_step(self, state, action, reward, done, next_state):
+        """
+        Updates the provided state, action, reward, done, and next_state.
+
+        :param state: The current state of the environment.
+        :type state: numpy.ndarray
+        :param action: The action taken by the agent.
+        :type action: int
+        :param reward: The reward for the current step.
+        :type reward: float
+        :param done: Flag to mark if the episode is done or not.
+        :type done: bool
+        :param next_state: The next state after the current action.
+        :type next_state: numpy.ndarray
+        """
+
+        self.update_reward(reward)
+
+        self.states.append(state)
+        self.actions.append(action)
+        self.rewards.append(reward)
+        self.dones.append(done)
+        self.next_states.append(next_state)
+
+        if done:
+            self.update()
+
     def save_policy_value(self, file_name):
         """
         Save the policy and value networks and their optimizer states in a file.
 
         :param file_name: The name of the file to save the networks and optimizer states.
         :type file_name: str
         """
```

### Comparing `modular_rl-0.3.1/modular_rl/agents/_custom.py` & `modular_rl-0.3.2/modular_rl/agents/_custom.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.1/modular_rl/agents/mcis.py` & `modular_rl-0.3.2/modular_rl/agents/mcis.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,44 +49,14 @@
         self.temperature = setting.get('temperature', 1.0)
 
         self.device = setting.get('device', None)
         if self.device == None:
             self.device = torch.device(
                 "cuda" if torch.cuda.is_available() else "cpu")
 
-        # Save selected learning data separately
-        # self.state_tensor
-
-    def update_step(self, state, action, reward, done, next_state):
-        """
-        Updates the provided state, action, reward, done, and next_state.
-
-        :param state: The current state of the environment.
-        :type state: numpy.ndarray
-        :param action: The action taken by the agent.
-        :type action: int
-        :param reward: The reward for the current step.
-        :type reward: float
-        :param done: Flag to mark if the episode is done or not.
-        :type done: bool
-        :param next_state: The next state after the current action.
-        :type next_state: numpy.ndarray
-        """
-
-        self.update_reward(reward)
-
-        self.states.append(state)
-        self.actions.append(action)
-        self.rewards.append(reward)
-        self.dones.append(done)
-        self.next_states.append(next_state)
-
-        if done:
-            self.update()
-
     def select_action(self, state):
         """
         Select an action using mcis.
 
         :param state: The current state.
         :type state: numpy.ndarray
         :return: The selected action.
@@ -132,15 +102,22 @@
         :type reward: float
         :param done: Whether the episode has ended.
         :type done: bool
         """
         for node in reversed(search_path):
             node.update_stats(reward)
             if not done:
-                state_tensor = self.check_tensor(node.state).to(self.device)
+                if isinstance(node.state, np.ndarray):
+                    state_tensor = torch.from_numpy(
+                        node.state).float().to(self.device)
+                elif torch.is_tensor(node.state):
+                    state_tensor = node.state.float().to(self.device)
+                else:
+                    raise ValueError(
+                        "node.state must be a numpy array or torch tensor")
                 _, reward = self.actor_critic_net(state_tensor)
                 reward = reward.item()
 
     def learn(self):
         """
         Train the agent.
         """
```

### Comparing `modular_rl-0.3.1/modular_rl/agents/mcts.py` & `modular_rl-0.3.2/modular_rl/agents/mcts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,309 +1,323 @@
-
-# -*- coding: utf-8 -*-
-"""
-ModularRL project
-
-Copyright (c) 2023 horrible-gh
-
-Class AgentMCTS is an implementation of the Monte Carlo Tree Search (MCTS) algorithm.
-It takes an environment and a setting configuration as inputs, initializes neural network instances and optimizers,
-and sets various learning parameters.
-It has methods to predict an action given a state, perform a learning step, update the neural network parameters,
-save and load a checkpoint, and reset learning parameters.
-The class also has instance variables to keep track of episode and total rewards, previous reward, and average reward.
-
-This software includes the following third-party libraries:
-Gym (MIT License): https://github.com/openai/gym - Copyright (c) OpenAI.
-NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
-PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
-"""
-
-import gym
-import torch
-import torch.optim as optim
-from torch.distributions import Categorical
-import torch.nn.functional as F
-from modular_rl.networks.actor_critic import ActorCriticNetwork
-from modular_rl.util.node import Node
-from modular_rl.agents._agent import Agent
-from LogAssist.log import Logger
-
-
-class AgentMCTS(Agent):
-    def __init__(self, env, setting):
-        """
-        Initialize the AgentMCTS class with the specified environment and settings.
-
-        :param env: The environment to use for training.
-        :type env: gym.Env or None
-        :param setting: The settings for the MCTS algorithm.
-        :type setting: AgentSettings
-        """
-
-        super().__init__(env, setting)
-        super().init_actor_critic()
-
-        # MCTS parameters
-        self.num_simulations = setting.get('num_simulations', 800)
-        self.cpuct = setting.get('cpuct', 1.0)
-        self.temperature = setting.get('temperature', 1.0)
-
-        self.device = setting.get('device', None)
-        if self.device == None:
-            self.device = torch.device(
-                "cuda" if torch.cuda.is_available() else "cpu")
-
-        # Save selected learning data separately
-        # self.state_tensor
-
-    def select_action(self, state):
-        """
-        Select an action using MCTS.
-
-        :param state: The current state.
-        :type state: numpy.ndarray
-        :return: The selected action.
-        :rtype: int
-        """
-
-        state_tensor = self.check_tensor(self._check_state(state))
-        action_probs, _ = self.actor_critic_net(state_tensor)
-        action_probs = action_probs.detach().numpy().flatten()
-        root = Node(state, action_probs)
-        Logger.verb(
-            'agents:mcts:select_action:self.num_simulations', self.num_simulations)
-        Logger.verb(
-            'agents:mcts:select_action:root', root)
-        Logger.verb(
-            'agents:mcts:select_action:action_probs', action_probs)
-        Logger.verb('agents:mcts:select_action:node', f'Root node: {root}')
-        for _ in range(self.num_simulations):
-            node = root
-            search_path = [node]
-            # Logger.verb(
-            #    'agents:mcts:select_action:search_path', search_path)
-            # Selection
-            while node.expanded():
-                action, node = node.select_child(self.cpuct)
-                search_path.append(node)
-            Logger.verb('agents:mcts:select_action:After selection',
-                        f' {search_path[-1]}')
-
-            # Expansion
-            if len(search_path) > 1:
-                parent, action = search_path[-2], search_path[-1].action
-            else:
-                # or some other suitable defaults
-                parent, action = search_path[0], None
-
-            # Logger.verb('mcts:select_action:action', action)
-            step_output = self.env.step(action) if action is not None else (
-                parent.state, 0, False, None)
-            step_output_num = len(step_output)
-
-            if step_output_num == 4:
-                state, reward, done, _ = step_output
-            elif step_output_num == 5:
-                state, reward, done, _, _ = step_output
-
-            if not done:
-                # Logger.verb(
-                #    'agents:mcts:select_action:state', state)
-                if not torch.is_tensor(state):
-                    state_tensor = torch.from_numpy(
-                        state).float().to(self.device)
-                else:
-                    state_tensor = state.to(self.device)
-
-                action_probs, value = self.actor_critic_net(state_tensor)
-                action_space = self.env.action_space.n
-                node.expand(action_space, action_probs)
-
-            # Backpropagation
-            self.backpropagate(search_path, reward, done)
-
-        chosen_action = root.select_action(self.temperature)
-        chosen_action_reward = root.children[chosen_action].total_value
-        chosen_action_state = root.children[chosen_action].state
-        # Assuming that a non-zero reward indicates a terminal state
-        done = (chosen_action_reward != 0)
-
-        # Save selected learning data separately
-        self.state = chosen_action_state
-        self.action = chosen_action
-        self.reward = chosen_action_reward
-        self.done = done
-
-        self.total_reward += reward
-        self.prev_reward = reward
-
-        return chosen_action_state, chosen_action, chosen_action_reward, done
-
-    def backpropagate(self, search_path, reward, done):
-        """
-        Backpropagate the value estimates back to the root node.
-
-        :param search_path: The nodes visited during the search.
-        :type search_path: list of Node
-        :param reward: The reward obtained after the search.
-        :type reward: float
-        :param done: Whether the episode has ended.
-        :type done: bool
-        """
-        for node in reversed(search_path):
-            node.update_stats(reward)
-            if not done:
-                _, reward = self.actor_critic_net(node.state)
-                reward = reward.item()
-
-    def learn(self):
-        """
-        Train the agent.
-        """
-        self.train()
-
-    def train(self):
-        """
-        Train the agent.
-        """
-        self.total_reward = 0
-        for episode in range(self.max_episodes):
-            self.episode = episode
-            state = self.learn_reset()
-            # state = self.env.reset()
-
-            for t in range(self.max_timesteps):
-                state = self._check_state(state)
-                self.state_tensor = self.check_tensor(state).squeeze(0)
-                self.next_state, self.action, self.reward, self.done = self.select_action(
-                    self.state_tensor)
-
-                self.learn_check()
-
-                if self.done:
-                    # self.update()
-                    break
-
-                self.update()
-
-                state = self.next_state
-
-            self.episode += 1
-            # print(f"Episode: {self.episode}, Reward: {self.total_reward}")
-
-    def compute_loss(self, state, action, reward, next_state, done):
-        '''
-        This function computes the actor and critic loss using the provided state, action, reward, next_state, and done variables.
-        The actor loss is computed based on the policy gradient algorithm,
-        and the critic loss is computed as the mean squared error between the estimated value of the current state and the target value of the next state.
-
-        compute_loss() function computes the actor and critic loss values for the provided state, action, reward, next_state, and done variables.
-
-        The state parameter is the current state of the environment.
-        The action parameter is the action taken in the current state.
-        The reward parameter is the reward received for taking the action in the current state.
-        The next_state parameter is the state resulting from taking the action in the current state.
-        The done parameter is a flag indicating whether the episode has ended.
-
-        :param state: The current state of the environment.
-        :param action: The action taken in the current state.
-        :param reward: The reward received for taking the action in the current state.
-        :param next_state: The state resulting from taking the action in the current state.
-        :param done: A flag indicating whether the episode has ended.
-        :return: The computed actor and critic loss values.
-        '''
-
-        # Predict action probabilities and values
-        action_probs, values = self.actor_critic_net(state)
-
-        # Compute the value loss
-        target_values = reward + self.gamma * \
-            self.actor_critic_net(next_state)[1] * (1 - done)
-        critic_loss = F.mse_loss(values, target_values.detach())
-
-        # Compute the policy loss
-        m = Categorical(action_probs)
-        logprobs = m.log_prob(self.check_tensor(action))
-        actor_loss = -logprobs * (target_values - values).detach()
-
-        return actor_loss, critic_loss
-
-    def update(self):
-        '''
-        This function updates the network parameters using the optimizer and computed loss values.
-
-        update() function updates the network parameters using the optimizer and computed loss values.
-        It uses the compute_loss() function to compute the loss and the optimizer object to perform the optimization step.
-
-        This function does not take any parameters and does not return anything.
-
-        :return: None
-        '''
-
-        # Update the network
-        self.actor_critic_optimizer.zero_grad()
-        actor_loss, critic_loss = self.compute_loss(
-            self.state_tensor, self.action, self.reward, self.next_state, self.done)
-        loss = actor_loss + critic_loss
-        loss.backward()
-        self.actor_critic_optimizer.step()
-
-    def check_tensor(self, obj):
-        '''
-        This function checks if the provided object is a PyTorch tensor, and if not, converts it to a tensor.
-
-        check_tensor() function checks if the provided obj parameter is a PyTorch tensor.
-        If it is not a tensor, it converts it to a tensor using torch.FloatTensor().
-        If it is already a tensor, it simply returns the tensor.
-
-        The obj parameter is the object to check/convert to a PyTorch tensor.
-
-        The function returns the input object as a PyTorch tensor.
-
-        :param obj: The object to check/convert to a PyTorch tensor.
-        :return: The input object as a PyTorch tensor.
-        '''
-
-        if not torch.is_tensor(obj):
-            obj_tensor = torch.FloatTensor(obj)
-        else:
-            obj_tensor = obj
-        return obj_tensor
-
-    def save_model(self, file_name):
-        """
-        This function saves the model to the specified file.
-
-        :param file_name: The name of the file to save the model to.
-        :return: None
-        """
-        self.save(file_name)
-
-    def save(self, file_name):
-        """
-        This function saves the actor critic network to the specified file.
-
-        :param file_name: The name of the file to save the actor critic network to.
-        :return: None
-        """
-
-        self.save_actor_critic(file_name)
-
-    def load_model(self, file_name):
-        """
-        This function loads the model from the specified file.
-
-        :param file_name: The name of the file to load the model from.
-        :return: None
-        """
-        self.load(file_name)
-
-    def load(self, file_name):
-        """
-        This function loads the actor critic network from the specified file.
-
-        :param file_name: The name of the file to load the actor critic network from.
-        :return: None
-        """
-
-        self.load_actor_critic(file_name)
+
+# -*- coding: utf-8 -*-
+"""
+ModularRL project
+
+Copyright (c) 2023 horrible-gh
+
+Class AgentMCTS is an implementation of the Monte Carlo Tree Search (MCTS) algorithm.
+It takes an environment and a setting configuration as inputs, initializes neural network instances and optimizers,
+and sets various learning parameters.
+It has methods to predict an action given a state, perform a learning step, update the neural network parameters,
+save and load a checkpoint, and reset learning parameters.
+The class also has instance variables to keep track of episode and total rewards, previous reward, and average reward.
+
+This software includes the following third-party libraries:
+Gym (MIT License): https://github.com/openai/gym - Copyright (c) OpenAI.
+NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
+PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
+"""
+
+import torch
+import numpy as np
+from torch.distributions import Categorical
+import torch.nn.functional as F
+from modular_rl.util.node import Node
+from modular_rl.agents._agent import Agent
+from LogAssist.log import Logger
+
+
+class AgentMCTS(Agent):
+    def __init__(self, env, setting):
+        """
+        Initialize the AgentMCTS class with the specified environment and settings.
+
+        :param env: The environment to use for training.
+        :type env: gym.Env or None
+        :param setting: The settings for the MCTS algorithm.
+        :type setting: AgentSettings
+        """
+
+        super().__init__(env, setting)
+        super().init_actor_critic()
+
+        # MCTS parameters
+        self.num_simulations = setting.get('num_simulations', 800)
+        self.cpuct = setting.get('cpuct', 1.0)
+        self.temperature = setting.get('temperature', 1.0)
+        self.gamma = 0.95
+        self.total_value = 0
+
+        self.device = setting.get('device', None)
+        if self.device == None:
+            self.device = torch.device(
+                "cuda" if torch.cuda.is_available() else "cpu")
+        self.reset()
+
+    def reset(self):
+        self.state = None
+        self.action = None
+        self.reward = None
+        self.done = None
+        self.total_reward = 0
+
+    def select_action(self, state):
+        """
+        Select an action using MCTS.
+
+        :param state: The current state.
+        :type state: numpy.ndarray
+        :return: The selected action.
+        :rtype: int
+        """
+
+        state_tensor = self.check_tensor(self._check_state(state))
+        action_probs, _ = self.actor_critic_net(state_tensor)
+        action_probs = action_probs.detach()
+        m = Categorical(action_probs)
+        chosen_action = m.sample().item()
+
+        # Use uniform prior for root node.
+        root = Node(state, [1 / self.env.action_space.n]
+                    * self.env.action_space.n)
+
+        for _ in range(self.num_simulations):
+            node, search_path = root, [root]
+
+            while node.expanded():
+                action, node = node.select_child(self.cpuct)
+                if action is None:
+                    action = chosen_action
+                search_path.append(node)
+
+            parent, action = (search_path[-2], search_path[-1].action) if len(
+                search_path) > 1 else (search_path[0], None)
+            step_output = self.env.step(action) if action is not None else (
+                parent.state, 0, False, None)
+            state, reward, done, *_ = step_output
+            Logger.verb('mcts:select_action', f"Step Output Reward: {reward}")
+
+            if not done:
+                state_tensor = self.check_tensor(state).to(self.device)
+                action_probs, _ = self.actor_critic_net(state_tensor)
+                node.expand(self.env.action_space.n,
+                            action_probs.detach().cpu().numpy().flatten(), False)
+
+            self.backpropagate(search_path, reward, done)
+
+        chosen_action_node = root.children[chosen_action]
+
+        self.state = chosen_action_node.state
+        self.action = chosen_action
+        self.reward = chosen_action_node.total_value
+        self.done = self.reward != 0
+
+        self.total_reward += self.reward
+
+        return self.state, self.action, self.reward, self.done
+
+    def backpropagate(self, search_path, reward, done):
+        """
+        Backpropagate the value estimates back to the root node.
+
+        :param search_path: The nodes visited during the search.
+        :type search_path: list of Node
+        :param reward: The reward obtained after the search.
+        :type reward: float
+        :param done: Whether the episode has ended.
+        :type done: bool
+        """
+        for node in reversed(search_path):
+            # Logger.verb('mcts:backpropagate',
+            #            f"Node Reward({reward}) after Update Stats: {node.total_value}")
+            node.update_stats(reward)
+
+    def learn(self):
+        """
+        Train the agent.
+        """
+        self.train()
+
+    def train(self):
+        """
+        Train the agent.
+        """
+        self.total_reward = 0
+        for episode in range(self.max_episodes):
+            self.episode = episode
+            state = self.learn_reset()
+            # state = self.env.reset()
+
+            for t in range(self.max_timesteps):
+                state = self._check_state(state)
+                self.state_tensor = self.check_tensor(state).squeeze(0)
+                self.next_state, self.action, self.reward, self.done = self.select_action(
+                    self.state_tensor)
+
+                self.learn_check()
+
+                if self.done:
+                    # self.update()
+                    break
+
+                self.update()
+
+                state = self.next_state
+
+            self.episode += 1
+            # print(f"Episode: {self.episode}, Reward: {self.total_reward}")
+
+    def compute_loss(self, state, action, reward, done):
+        '''
+        This function computes the actor and critic loss using the provided state, action, reward, next_state, and done variables.
+        The actor loss is computed based on the policy gradient algorithm,
+        and the critic loss is computed as the mean squared error between the estimated value of the current state and the target value of the next state.
+
+        compute_loss() function computes the actor and critic loss values for the provided state, action, reward, next_state, and done variables.
+
+        The state parameter is the current state of the environment.
+        The action parameter is the action taken in the current state.
+        The reward parameter is the reward received for taking the action in the current state.
+        The next_state parameter is the state resulting from taking the action in the current state.
+        The done parameter is a flag indicating whether the episode has ended.
+
+        :param state: The current state of the environment.
+        :param action: The action taken in the current state.
+        :param reward: The reward received for taking the action in the current state.
+        :param next_state: The state resulting from taking the action in the current state.
+        :param done: A flag indicating whether the episode has ended.
+        :return: The computed actor and critic loss values.
+        '''
+        # Predict action probabilities and values
+        action_probs, values = self.actor_critic_net(state)
+
+        # Compute the value loss
+        # Convert reward to tensor
+        reward = torch.tensor(reward, device=self.device)
+        # Convert total_value to tensor
+        total_value = torch.tensor(self.total_value, device=self.device)
+        target_values = reward + self.gamma * total_value * (1 - done)
+        target_values = target_values.unsqueeze(0)
+        critic_loss = F.mse_loss(values, target_values.detach())
+
+        # If action is not a list or tuple or its length is zero, initialize it with zeros
+        if not isinstance(action, (list, tuple)) or len(action) == 0:
+            action = torch.zeros_like(action_probs)
+
+        # Compute the policy loss
+        m = Categorical(action_probs)
+        logprobs = m.log_prob(self.check_tensor(action))
+        actor_loss = -logprobs * (target_values - values).detach()
+
+        # Average the actor and critic loss
+        loss = (actor_loss.mean() + critic_loss.mean()) / 2
+
+        return loss
+
+    def update(self):
+        '''
+        This function updates the network parameters using the optimizer and computed loss values.
+
+        update() function updates the network parameters using the optimizer and computed loss values.
+        It uses the compute_loss() function to compute the loss and the optimizer object to perform the optimization step.
+
+        This function does not take any parameters and does not return anything.
+
+        :return: None
+        '''
+
+        # Update the network
+        # Convert state to tensor
+        state_tensor = torch.tensor(self.state, device=self.device)
+
+        # Update the network
+        self.actor_critic_optimizer.zero_grad()
+        loss = self.compute_loss(
+            state_tensor, self.action, self.reward, self.done)
+        Logger.verb('mcts:update',
+                    f"Loss: {loss.item()}, Reward: {self.reward}")
+        loss.backward()
+        self.actor_critic_optimizer.step()
+
+        self.reset()
+
+    def check_tensor(self, obj):
+        '''
+        This function checks if the provided object is a PyTorch tensor, and if not, converts it to a tensor.
+
+        check_tensor() function checks if the provided obj parameter is a PyTorch tensor.
+        If it is not a tensor, it converts it to a tensor using torch.FloatTensor().
+        If it is already a tensor, it simply returns the tensor.
+
+        The obj parameter is the object to check/convert to a PyTorch tensor.
+
+        The function returns the input object as a PyTorch tensor.
+
+        :param obj: The object to check/convert to a PyTorch tensor.
+        :return: The input object as a PyTorch tensor.
+        '''
+
+        if not torch.is_tensor(obj):
+            obj_tensor = torch.FloatTensor(obj)
+        else:
+            obj_tensor = obj
+
+        Logger.verb('mcts:check_tensor', f"Before remapping: {obj_tensor}")
+        obj_tensor = obj_tensor % self.env.action_space.n
+        obj_tensor = torch.where(
+            obj_tensor >= self.env.action_space.n, self.env.action_space.n - 1, obj_tensor)
+        obj_tensor = torch.round(obj_tensor)
+        Logger.verb('mcts:check_tensor', f"After remapping: {obj_tensor}")
+        return obj_tensor
+
+    def save_model(self, file_name):
+        """
+        This function saves the model to the specified file.
+
+        :param file_name: The name of the file to save the model to.
+        :return: None
+        """
+        self.save(file_name)
+
+    def save(self, file_name):
+        """
+        This function saves the actor critic network to the specified file.
+
+        :param file_name: The name of the file to save the actor critic network to.
+        :return: None
+        """
+
+        self.save_actor_critic(file_name)
+
+    def load_model(self, file_name):
+        """
+        This function loads the model from the specified file.
+
+        :param file_name: The name of the file to load the model from.
+        :return: None
+        """
+        self.load(file_name)
+
+    def load(self, file_name):
+        """
+        This function loads the actor critic network from the specified file.
+
+        :param file_name: The name of the file to load the actor critic network from.
+        :return: None
+        """
+
+        self.load_actor_critic(file_name)
+
+    def update_step(self, state, action, reward, done, next_state):
+        """
+        In MCTS, update_step is not necessary as the agent is updated
+        after every simulation (or a batch of simulations), each of which
+        represents an entire episode. Thus, this method can be left blank or removed.
+        """
+        self.state = state
+        self.action = action
+        self.reward = reward
+        self.done = done
+        self.next_state = next_state
+        self.update_reward(reward)
+        self.update_episode()
```

### Comparing `modular_rl-0.3.1/modular_rl/agents/mim.py` & `modular_rl-0.3.2/modular_rl/agents/mim.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.1/modular_rl/agents/ppo.py` & `modular_rl-0.3.2/modular_rl/agents/ppo.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.1/modular_rl/envs/mim/card_evaluator.py` & `modular_rl-0.3.2/modular_rl/envs/mim/card_evaluator.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.1/modular_rl/envs/mim/mim.py` & `modular_rl-0.3.2/modular_rl/envs/mim/mim.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.1/modular_rl/networks/actor_critic.py` & `modular_rl-0.3.2/modular_rl/networks/actor_critic.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.1/modular_rl/networks/policy.py` & `modular_rl-0.3.2/modular_rl/networks/policy.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.1/modular_rl/networks/value.py` & `modular_rl-0.3.2/modular_rl/networks/value.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.1/modular_rl/params/mcis.py` & `modular_rl-0.3.2/modular_rl/params/mcis.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.1/modular_rl/params/mcts.py` & `modular_rl-0.3.2/modular_rl/params/mcts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-class ParamMCTS:
-    default = {
-        'max_episodes': 10,  # Maximum number of episodes for training
-        'max_timesteps': 200,  # Maximum number of timesteps for each episode
-        'update_timestep': 2000,  # Update the policy every specified timestep
-        'networks': 'medium',  # Size of the hidden layer in neural networks
-        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
-        'num_simulations': 10,  # Number of MCTS simulations per move
-        'cpuct': 1.0,  # Exploration constant for MCTS
-        'temperature': 1.0,  # Temperature for action selection during MCTS
-        'gamma': 0.99,  # Discount factor
-        # If the average reward is greater than or equal to this value, training is stopped early
-        'early_stop_threshold': -1,
-        'done_loop_end': False,  # If True, end the episode when the done flag is set
-        'reward_print': True,  # If True, print the reward during training
-        'device': None,  # Device to run the model on, None for automatic selection
-        'log_level': 'debug',  # Log level for the logger
-        'log_init_pass': False,  # If True, skip logger initialization
-    }
-
-    default_modular = {
-        # Maximum number of episodes for training (-1 for no limit)
-        'max_episodes': -1,
-        # Maximum number of timesteps for each episode (-1 for no limit)
-        'max_timesteps': -1,
-        # Update the policy every specified timestep (-1 for no limit)
-        'update_timestep': -1,
-        'networks': 'medium',  # Size of the hidden layer in neural networks
-        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
-        'num_simulations': 800,  # Number of MCTS simulations per move
-        'cpuct': 1.0,  # Exploration constant for MCTS
-        'temperature': 1.0,  # Temperature for action selection during MCTS
-        'gamma': 0.99,  # Discount factor
-        # If the average reward is greater than or equal to this value, training is stopped early
-        'early_stop_threshold': -1,
-        'reward_print': True,  # If True, print the reward during training
-        'device': None,  # Device to run the model on, None for automatic selection
-        'log_level': 'debug',  # Log level for the logger
-        'log_init_pass': False,  # If True, skip logger initialization
-    }
+class ParamMCTS:
+    default = {
+        'max_episodes': 10,  # Maximum number of episodes for training
+        'max_timesteps': 200,  # Maximum number of timesteps for each episode
+        'update_timestep': 2000,  # Update the policy every specified timestep
+        'num_simulations': 10,  # Number of MCTS simulations per move
+        'networks': 'medium',  # Size of the hidden layer in neural networks
+        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
+        'cpuct': 1.0,  # Exploration constant for MCTS
+        'temperature': 1.0,  # Temperature for action selection during MCTS
+        'gamma': 0.99,  # Discount factor
+        # If the average reward is greater than or equal to this value, training is stopped early
+        'early_stop_threshold': -1,
+        'done_loop_end': False,  # If True, end the episode when the done flag is set
+        'reward_print': True,  # If True, print the reward during training
+        'device': None,  # Device to run the model on, None for automatic selection
+        'log_level': 'debug',  # Log level for the logger
+        'log_init_pass': False,  # If True, skip logger initialization
+    }
+
+    default_modular = {
+        # Maximum number of episodes for training (1 for modular)
+        'max_episodes': 1,
+        # Maximum number of timesteps for each episode (1 for modular)
+        'max_timesteps': 1,
+        # Update the policy every specified timestep (1 for modular)
+        'update_timestep': 1,
+        'num_simulations': 1,  # Number of MCTS simulations per move
+        'networks': 'medium',  # Size of the hidden layer in neural networks
+        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
+        'cpuct': 1.0,  # Exploration constant for MCTS
+        'temperature': 1.0,  # Temperature for action selection during MCTS
+        'gamma': 0.99,  # Discount factor
+        # If the average reward is greater than or equal to this value, training is stopped early
+        'early_stop_threshold': -1,
+        'reward_print': True,  # If True, print the reward during training
+        'device': None,  # Device to run the model on, None for automatic selection
+        'log_level': 'debug',  # Log level for the logger
+        'log_init_pass': False,  # If True, skip logger initialization
+    }
```

### Comparing `modular_rl-0.3.1/modular_rl/params/mim.py` & `modular_rl-0.3.2/modular_rl/params/mim.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.1/modular_rl/params/ppo.py` & `modular_rl-0.3.2/modular_rl/params/ppo.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.1/modular_rl/settings.py` & `modular_rl-0.3.2/modular_rl/settings.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.1/modular_rl/tester/mim.py` & `modular_rl-0.3.2/modular_rl/tester/mim.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.1/modular_rl/tester/ppo.py` & `modular_rl-0.3.2/modular_rl/tester/ppo.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.1/modular_rl/util/node.py` & `modular_rl-0.3.2/modular_rl/util/node.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.3.1/modular_rl.egg-info/PKG-INFO` & `modular_rl-0.3.2/modular_rl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modular-rl
-Version: 0.3.1
+Version: 0.3.2
 Summary: ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
 Home-page: https://github.com/horrible-gh/ModularRL
 Author: sjm
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/ModularRL
 Project-URL: Bug Tracker, https://github.com/horrible-gh/ModularRL/issues
 Keywords: ModularRL,Modular-RL,Modular_RL,Modular RL,modularrl,modular_rl,modular-rl,modular rl,mrl,modular,learn,learning,pytorch learn,pytorch learning
@@ -45,18 +45,18 @@
 -   Proximal Policy Optimization (PPO)
 -   Monte Carlo Tree Search (MCTS)
 -   Monte Carlo Information Set (MCIS)
 -   Modular's sIMulator (MIM)
 
 Refer to the respective agent classes for each algorithm:
 
--   AgentPPO (Modular)
--   AgentMCTS
--   AgentMCIS (Modular)
--   AgentMIM (Modular)
+-   AgentPPO (+ Modular)
+-   AgentMCTS (+ Modular)
+-   AgentMCIS (+ Modular)
+-   AgentMIM (+ Modular)
 
 ## Example Usage
 
 You can use the tester.py script provided in the library to create and train an instance of an agent with default or modified settings:
 
 ```python
 import modular_rl.tester as tester
```

### Comparing `modular_rl-0.3.1/modular_rl.egg-info/SOURCES.txt` & `modular_rl-0.3.2/modular_rl.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -36,11 +36,12 @@
 modular_rl/tester/mim.py
 modular_rl/tester/ppo.py
 modular_rl/util/__init__.py
 modular_rl/util/node.py
 tests/test_mcis.py
 tests/test_mcis_modular.py
 tests/test_mcts.py
+tests/test_mcts_modular.py
 tests/test_mim.py
 tests/test_mim_modular.py
 tests/test_ppo.py
 tests/test_ppo_modular.py
```

### Comparing `modular_rl-0.3.1/pyproject.toml` & `modular_rl-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "modular_rl"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="horrible", email="shinjpn1@gmail.com" },
 ]
 description = "ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `modular_rl-0.3.1/setup.py` & `modular_rl-0.3.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modular_rl',
-    version='0.3.1',
+    version='0.3.2',
     description='ModularRL package',
     author='sjm',
     author_email='shinjpn1@gmail.com',
     url='https://github.com/horrible-gh/ModularRL',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

