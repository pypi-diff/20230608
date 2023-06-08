# Comparing `tmp/pufferlib-0.2.1.tar.gz` & `tmp/pufferlib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pufferlib-0.2.1.tar", last modified: Mon Mar 20 03:20:22 2023, max compression
+gzip compressed data, was "pufferlib-0.3.0.tar", last modified: Thu Jun  8 02:41:45 2023, max compression
```

## Comparing `pufferlib-0.2.1.tar` & `pufferlib-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:20:22.781782 pufferlib-0.2.1/
--rw-r--r--   0 root         (0) root         (0)     1065 2022-10-14 23:33:16.000000 pufferlib-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      866 2023-03-20 03:20:22.781782 pufferlib-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1076 2023-03-20 03:17:38.000000 pufferlib-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:20:22.771782 pufferlib-0.2.1/pufferlib/
--rw-r--r--   0 root         (0) root         (0)       67 2023-03-08 02:05:50.000000 pufferlib-0.2.1/pufferlib/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22066 2023-03-20 03:17:38.000000 pufferlib-0.2.1/pufferlib/emulation.py
--rw-r--r--   0 root         (0) root         (0)     6143 2023-03-07 04:48:58.000000 pufferlib-0.2.1/pufferlib/evaluation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:20:22.771782 pufferlib-0.2.1/pufferlib/frameworks/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-20 19:21:46.000000 pufferlib-0.2.1/pufferlib/frameworks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-03-07 02:14:15.000000 pufferlib-0.2.1/pufferlib/frameworks/base.py
--rw-r--r--   0 root         (0) root         (0)     2709 2023-03-12 22:50:55.000000 pufferlib-0.2.1/pufferlib/frameworks/cleanrl.py
--rw-r--r--   0 root         (0) root         (0)     4758 2023-03-12 22:52:48.000000 pufferlib-0.2.1/pufferlib/frameworks/rllib.py
--rw-r--r--   0 root         (0) root         (0)     4412 2023-03-12 22:35:10.000000 pufferlib-0.2.1/pufferlib/models.py
--rw-r--r--   0 root         (0) root         (0)     3808 2022-12-20 03:08:05.000000 pufferlib-0.2.1/pufferlib/rating.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:20:22.781782 pufferlib-0.2.1/pufferlib/registry/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-07 03:34:29.000000 pufferlib-0.2.1/pufferlib/registry/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4592 2023-03-12 23:07:09.000000 pufferlib-0.2.1/pufferlib/registry/atari.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-03-12 22:08:21.000000 pufferlib-0.2.1/pufferlib/registry/butterfly.py
--rw-r--r--   0 root         (0) root         (0)      521 2023-03-12 22:11:26.000000 pufferlib-0.2.1/pufferlib/registry/classic_control.py
--rw-r--r--   0 root         (0) root         (0)      591 2023-03-12 22:11:31.000000 pufferlib-0.2.1/pufferlib/registry/griddly.py
--rw-r--r--   0 root         (0) root         (0)      521 2023-03-12 22:11:35.000000 pufferlib-0.2.1/pufferlib/registry/magent.py
--rw-r--r--   0 root         (0) root         (0)      545 2023-03-12 22:11:41.000000 pufferlib-0.2.1/pufferlib/registry/microrts.py
--rw-r--r--   0 root         (0) root         (0)     7036 2023-03-12 22:12:36.000000 pufferlib-0.2.1/pufferlib/registry/nethack.py
--rw-r--r--   0 root         (0) root         (0)     1845 2023-03-12 22:14:06.000000 pufferlib-0.2.1/pufferlib/registry/nmmo.py
--rw-r--r--   0 root         (0) root         (0)      575 2023-03-12 22:16:25.000000 pufferlib-0.2.1/pufferlib/registry/smac.py
--rw-r--r--   0 root         (0) root         (0)      578 2022-12-20 03:08:05.000000 pufferlib-0.2.1/pufferlib/torch.py
--rw-r--r--   0 root         (0) root         (0)     4372 2023-03-07 04:02:00.000000 pufferlib-0.2.1/pufferlib/utils.py
--rw-r--r--   0 root         (0) root         (0)     6069 2023-03-12 22:47:23.000000 pufferlib-0.2.1/pufferlib/vectorization.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-03-20 03:18:11.000000 pufferlib-0.2.1/pufferlib/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:20:22.771782 pufferlib-0.2.1/pufferlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      866 2023-03-20 03:20:22.000000 pufferlib-0.2.1/pufferlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      812 2023-03-20 03:20:22.000000 pufferlib-0.2.1/pufferlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 03:20:22.000000 pufferlib-0.2.1/pufferlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      865 2023-03-20 03:20:22.000000 pufferlib-0.2.1/pufferlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-20 03:20:22.000000 pufferlib-0.2.1/pufferlib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-20 03:20:22.781782 pufferlib-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2537 2023-03-20 03:17:51.000000 pufferlib-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:41:45.075120 pufferlib-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-26 00:26:04.000000 pufferlib-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      966 2023-06-08 02:41:45.075120 pufferlib-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-05-26 00:26:04.000000 pufferlib-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:41:45.075120 pufferlib-0.3.0/pufferlib/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30790 2023-06-08 02:01:34.000000 pufferlib-0.3.0/pufferlib/emulation.py
+-rw-r--r--   0 root         (0) root         (0)     6143 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/evaluation.py
+-rw-r--r--   0 root         (0) root         (0)      535 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:41:45.075120 pufferlib-0.3.0/pufferlib/frameworks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/frameworks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-06-02 03:36:02.000000 pufferlib-0.3.0/pufferlib/frameworks/base.py
+-rw-r--r--   0 root         (0) root         (0)     3328 2023-06-08 02:24:57.000000 pufferlib-0.3.0/pufferlib/frameworks/cleanrl.py
+-rw-r--r--   0 root         (0) root         (0)     4758 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/frameworks/rllib.py
+-rw-r--r--   0 root         (0) root         (0)     4148 2023-06-08 01:53:23.000000 pufferlib-0.3.0/pufferlib/models.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/rating.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:41:45.075120 pufferlib-0.3.0/pufferlib/registry/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/registry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4733 2023-06-08 02:38:25.000000 pufferlib-0.3.0/pufferlib/registry/atari.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/registry/butterfly.py
+-rw-r--r--   0 root         (0) root         (0)      521 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/registry/classic_control.py
+-rw-r--r--   0 root         (0) root         (0)      467 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/registry/crafter.py
+-rw-r--r--   0 root         (0) root         (0)      515 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/registry/dm_lab.py
+-rw-r--r--   0 root         (0) root         (0)      452 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/registry/dmc.py
+-rw-r--r--   0 root         (0) root         (0)      591 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/registry/griddly.py
+-rw-r--r--   0 root         (0) root         (0)      521 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/registry/magent.py
+-rw-r--r--   0 root         (0) root         (0)      545 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/registry/microrts.py
+-rw-r--r--   0 root         (0) root         (0)      448 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/registry/minecraft.py
+-rw-r--r--   0 root         (0) root         (0)     6967 2023-06-08 02:39:31.000000 pufferlib-0.3.0/pufferlib/registry/nethack.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-06-08 02:36:09.000000 pufferlib-0.3.0/pufferlib/registry/nmmo.py
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/registry/smac.py
+-rw-r--r--   0 root         (0) root         (0)      578 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/torch.py
+-rw-r--r--   0 root         (0) root         (0)     7670 2023-05-31 04:55:22.000000 pufferlib-0.3.0/pufferlib/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:41:45.075120 pufferlib-0.3.0/pufferlib/vectorization/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/vectorization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/vectorization/multiprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     7984 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/vectorization/multiprocessing_shared.py
+-rw-r--r--   0 root         (0) root         (0)     6158 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/vectorization/ray.py
+-rw-r--r--   0 root         (0) root         (0)     6347 2023-05-26 00:26:04.000000 pufferlib-0.3.0/pufferlib/vectorization/ray_shared.py
+-rw-r--r--   0 root         (0) root         (0)     4238 2023-06-01 19:06:46.000000 pufferlib-0.3.0/pufferlib/vectorization/serial.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 02:41:30.000000 pufferlib-0.3.0/pufferlib/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:41:45.075120 pufferlib-0.3.0/pufferlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      966 2023-06-08 02:41:45.000000 pufferlib-0.3.0/pufferlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1158 2023-06-08 02:41:45.000000 pufferlib-0.3.0/pufferlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 02:41:45.000000 pufferlib-0.3.0/pufferlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-06-08 02:41:45.000000 pufferlib-0.3.0/pufferlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-08 02:41:45.000000 pufferlib-0.3.0/pufferlib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 02:41:45.075120 pufferlib-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2900 2023-05-26 00:26:04.000000 pufferlib-0.3.0/setup.py
```

### Comparing `pufferlib-0.2.1/LICENSE` & `pufferlib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pufferlib-0.2.1/PKG-INFO` & `pufferlib-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pufferlib
-Version: 0.2.1
+Version: 0.3.0
 Summary: PufferAI LibraryPufferAI's library of RL tools and utilities
 Home-page: https://github.com/PufferAI/PufferLib
 Author: Joseph Suarez
 Author-email: jsuarez@mit.edu
 License: MIT
 Keywords: Puffer,AI,RL
 Platform: UNKNOWN
@@ -13,20 +13,24 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: rllib
+Provides-Extra: cleanrl
 Provides-Extra: tests
 Provides-Extra: all
 Provides-Extra: atari
 Provides-Extra: box2d
 Provides-Extra: butterfly
+Provides-Extra: crafter
+Provides-Extra: dm_control
+Provides-Extra: dm_lab
 Provides-Extra: magent
 Provides-Extra: microrts
+Provides-Extra: minerl
 Provides-Extra: nethack
-Provides-Extra: nmmo
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `pufferlib-0.2.1/README.md` & `pufferlib-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pufferlib-0.2.1/pufferlib/emulation.py` & `pufferlib-0.3.0/pufferlib/emulation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,549 @@
 from pdb import set_trace as T
-
+import itertools
 import numpy as np
 from contextlib import nullcontext
-from collections import defaultdict
-from collections import OrderedDict
+from collections import defaultdict, OrderedDict, Mapping
 
 import gym
 from pettingzoo.utils.env import ParallelEnv
 
 from pufferlib import utils
+from pufferlib import exceptions
 
 
-class Binding:
-    @property
-    def raw_env_cls(self):
-        '''Returns the original, unwrapped environment class used to create this binding, if available'''
-        if self._raw_env_cls is None:
-            raise ValueError('raw_env_cls not available when binding is not passed an env_cls')
-        return self._raw_env_cls
+class Postprocessor:
+    def __init__(self, env, teams, team_id):
+        if not isinstance(teams, Mapping):
+            raise ValueError(f'Teams is not a valid dict or mapping: {teams}')
 
-    def raw_env_creator(self):
-        '''Returns the original, unwrapped env_creator function used to create this binding'''
-        with utils.Suppress() if self._suppress_env_prints else nullcontext():
-            if self._raw_env_cls is None:
-                return self._raw_env_creator(*self._default_args, **self._default_kwargs)
+        if team_id not in teams:
+            raise ValueError(f'Team {team_id} not in teams {teams}')
+
+        self.env = env
+        self.teams = teams
+        self.team_id = team_id
+
+        self.num_teams = len(teams)
+        self.team_size = len(teams[team_id])
+        self.max_team_size = max([len(v) for v in self.teams.values()])
+
+        self.dummy_ob = None
+
+    def reset(self, team_obs):
+        return
+
+    def features(self, obs, step):
+        '''Default featurizer pads observations to max team size'''
+        if len(obs) == 0:
+            raise ValueError('Observation is empty')
+
+        if self.dummy_ob is None:
+            self.dummy_ob = utils.make_zeros_like(list(obs.values())[0])
+
+        team_id = [k for k, v in self.teams.items() if list(obs.keys())[0] in v][0]
+
+        ret = []
+        for agent in self.teams[team_id]:
+            if agent in obs:
+                ret.append(obs[agent])
             else:
-                return self._raw_env_cls(*self._default_args, **self._default_kwargs)
+                ret.append(self.dummy_ob)
 
-    @property
-    def env_cls(self):
-        '''Returns wrapped PufferEnv class created by this binding'''
-        return self._env_cls
+        return ret
 
-    def env_creator(self):
-        '''Returns the wrapped PufferEnv env_creator function created by this binding'''
-        return self._env_cls(*self._default_args, **self._default_kwargs)
+    def actions(self, actions, step):
+        return actions
 
-    @property
-    def single_observation_space(self):
-        '''Returns the wrapped, flat observation space of a single agent.
-        
-        PufferLib currently assumes that all agents share the same observation space'''
-        return self._single_observation_space
+    def rewards(self, team_rewards, team_dones, team_infos, step):
+        '''Default reward shaper sums team rewards'''
+        return sum(team_rewards.values()), team_infos
+
+
+class GymToPettingZooParallelWrapper(ParallelEnv):
+    def __init__(self, env: gym.Env):
+        self.env = env
+        self.possible_agents = [1]
+
+    def reset(self):
+        self.agents = [1]
+        return {1: self.env.reset()}
+
+    def step(self, actions):
+        ob, reward, done, info = self.env.step(actions[1])
+
+        if done:
+            self.agents = []
+
+        return {1: ob}, {1: reward}, {1: done}, info
+
+    def observation_space(self, agent):
+        return self.env.observation_space
+
+    def action_space(self, agent):
+        return self.env.action_space
+
+    def render(self, mode="human"):
+        return self.env.render(mode)
+
+    def close(self):
+        return self.env.close()
+
+    def seed(self, seed=None):
+        return self.env.seed(seed)
+
+def make_puffer_env_cls(scope, raw_obs):
+    class PufferEnv(ParallelEnv):
+        @utils.profile
+        def __init__(self, *args, env=None, **kwargs):
+            self.raw_env = self._create_env(env, *args, **kwargs)
+            self.env = self.raw_env if utils.is_multiagent(self.raw_env) else GymToPettingZooParallelWrapper(self.raw_env)
+
+            self.initialized = False
+            self._step = 0
+
+            self._obs_min, self._obs_max = utils._get_dtype_bounds(scope.obs_dtype)
+
+            # Assign valid teams. Autogen 1 team per agent if not provided
+            self._teams = {a:[a] for a in self.env.possible_agents} if scope.teams is None else scope.teams
+
+            if set(self.env.possible_agents) != {item for team in self._teams.values() for item in team}:
+                raise ValueError(f'Invalid teams: {self._teams} for possible_agents: {self.env.possible_agents}')
+
+            self.possible_agents = list(self._teams.keys())
+            self.default_team = self.possible_agents[0]
+
+            # Initialize postprocessors
+            self.postprocessors = {
+                team_id: scope.postprocessor_cls(
+                    self.env, self._teams, team_id,
+                    *scope.postprocessor_args,
+                    **scope.postprocessor_kwargs
+                ) for team_id in self._teams
+            }
+
+            # Manual LRU since functools.lru_cache is not pickleable
+            self._raw_observation_space = {}
+            self._flat_observation_space = {}
+            self._flat_action_space = {}
+            self._agent_action_space = {}
+
+            self.obs_space_cache, self.atn_space_cache = {}, {}
+            self.obs_space_cache = {team_id: self.observation_space(team_id) for team_id in self._teams}
+            self.atn_space_cache = {team_id: self.action_space(team_id) for team_id in self._teams}
+
+            # Set env metadata
+            self.metadata = self.env.metadata if hasattr(self.env, 'metadata') else {}
+
+        def _group_by_team(self, agent_data):
+            team_data = {}
+            for team_id, team in self._teams.items():
+                team_data[team_id] = {}
+                for agent_id in team:
+                    if agent_id in agent_data:
+                        team_data[team_id][agent_id] = agent_data[agent_id]
+            return team_data
+
+        @utils.profile
+        def _create_env(self, env, *args, **kwargs):
+            if env is not None:
+                return env
+
+            with utils.Suppress() if scope.suppress_env_prints else nullcontext():
+                if scope.env_cls:
+                    return scope.env_cls(*args, **kwargs)
+                return scope.env_creator(*args, **kwargs)
+
+        @utils.profile
+        def _reset_env(self, seed):
+            with utils.Suppress() if scope.suppress_env_prints else nullcontext():
+                # Handle seeding with different gym versions
+                try:
+                    return self.env.reset(seed=seed)
+                except:
+                    if seed is not None:
+                        self.env.seed(seed)
+                    return self.env.reset()
 
-    @property
-    def single_action_space(self):
-        '''Returns the wrapped, flat action space of a single agent.
-        
-        PufferLib currently assumes that all agents share the same action space'''
-        return self._single_action_space
+        @utils.profile
+        def _prestep(self, team_actions):
+            # Agent key check
+            if __debug__:
+                for team, atns in team_actions.items():
+                    if team not in self._teams:
+                        raise exceptions.InvalidAgentError(team, self._teams)
+
+            for team_id in self._teams:
+                team_actions[team_id] = self._handle_actions(
+                    team_actions[team_id], team_id)
+
+            # Action shape test
+            if __debug__:
+                for team, atns in team_actions.items():
+                    if not self.action_space(team).contains(atns):
+                        raise ValueError(
+                            f'action:\n{atns}\n for agent/team {team} not in '
+                            f'action space:\n{self.action_space(team)}')
+
+            # Unpack actions from teams
+            actions = {}
+            for team_id, team in self._teams.items():
+                # TODO: Assert all keys present since actions are padded
+                team_atns = np.split(team_actions[team_id], len(team))
+                for agent_id, atns in zip(team, team_atns):
+                    actions[agent_id] = atns
+
+            # TODO: Do we want to support structured actions?
+            if not scope.emulate_flat_atn:
+                return actions
+
+            # Unpack actions
+            for k in list(actions):
+                if k not in self.agents:
+                    del(actions[k])
+                    continue
+
+                flat = actions[k]
+                flat_space = self._agent_action_space[k]
+
+                if not isinstance(flat_space, dict):
+                    actions[k] = flat.reshape(flat_space.shape)
+                elif () in flat_space:
+                    actions[k] = flat[0]
+                else:
+                    nested_data = {}
 
-    @property
-    def raw_single_observation_space(self):
-        '''Returns the unwrapped, structured observation space of a single agent.
-        
-        PufferLib currently assumes that all agents share the same observation space'''
-        return self._raw_single_observation_space
+                    for key_list, space in flat_space.items():
+                        current_dict = nested_data
 
-    @property
-    def raw_single_action_space(self):
-        '''Returns the unwrapped, structured action space of a single agent.
-        
-        PufferLib currently assumes that all agents share the same action space'''
-        return self._raw_single_action_space
+                        for key in key_list[:-1]:
+                            if key not in current_dict:
+                                current_dict[key] = {}
+                            current_dict = current_dict[key]
+
+                        last_key = key_list[-1]
+
+                        if space.shape:
+                            size = np.prod(space.shape)
+                            current_dict[last_key] = flat[:size].reshape(space.shape)
+                            flat = flat[size:]
+                        else:
+                            current_dict[last_key] = flat[0]
+                            flat = flat[1:]
+
+                    actions[k] = nested_data
+
+            return actions
+
+        @utils.profile
+        def _step_env(self, actions):
+            with utils.Suppress() if scope.suppress_env_prints else nullcontext():
+                return self.env.step(actions)
+
+        @utils.profile
+        def _featurize(self, team_ob, team_id):
+            # Featurize observations for teams with at least 1 living agent
+            team_ob = self.postprocessors[team_id].features(team_ob, self._step)
+
+            if __debug__:
+                space = self._raw_observation_space[team_id]
+                if not space.contains(team_ob):
+                    raise ValueError(
+                        f'Featurized observation:\n{team_ob}\n not in observation space:\n'
+                        f'{space}\n for agent/team {team_id}'
+                    )
+
+            return team_ob
+
+        def _handle_actions(self, team_atns, team_id):
+            return self.postprocessors[team_id].actions(team_atns, self._step)
+
+        @utils.profile
+        def _shape_rewards(self, team_reward, team_dones, team_infos, team_id):
+            # Shape rewards for teams with at least 1 living agent
+            team_reward, team_infos = self.postprocessors[team_id].rewards(
+                team_reward, team_dones, team_infos, self._step)
+
+            if not isinstance(team_reward, (float, int)):
+                raise ValueError(
+                    f'Shaped reward {team_reward} of type '
+                    f'{type(team_reward)} is not a float or int'
+                )
 
-    @property
-    def max_agents(self):
-        '''Returns the maximum number of agents in the environment'''
-        return self._max_agents
+            return team_reward, team_infos
 
-    @property
-    def env_name(self):
-        '''Returns the environment name'''
-        return self._env_name
+        @utils.profile
+        def _poststep(self, obs, rewards, dones, infos):
+            # Terminate episode at horizon or if all agents are done
+            if scope.emulate_const_horizon is not None:
+                assert self._step <= scope.emulate_const_horizon
+                if self._step == scope.emulate_const_horizon:
+                    self.done = True
+
+            # Group by teams
+            obs = self._group_by_team(obs)
+            rewards = self._group_by_team(rewards)
+            dones = self._group_by_team(dones)
+
+            # Featurize and shape rewards; pad data
+            for team in self._teams:
+                if obs[team]:
+                    obs[team] = self._featurize(obs[team], team)
+                    obs[team] = _flatten_to_array(obs[team], self._flat_observation_space[team], scope.obs_dtype)
+                elif scope.emulate_flat_obs:
+                    obs[team] = self.pad_obs
+                else:
+                    del obs[team]
+
+                if rewards[team]:
+                    team_infos = {}
+                    if team in infos:
+                        team_infos = infos[team]
+
+                    # TODO: Handle team infos better
+                    rewards[team], infos[team] = self._shape_rewards(
+                        rewards[team], dones[team], team_infos, team)
+                elif scope.emulate_const_num_agents:
+                    rewards[team] = 0
+                else:
+                    del rewards[team]
 
+                if dones[team]:
+                    # TODO: Should dones per team be true on the first tick
+                    # or all subsequent ticks as well?
+                    dones[team] = self.done or \
+                        not any([e in self.agents for e in self._teams[team]])
+
+                elif scope.emulate_const_num_agents:
+                    dones[team] = self.done
+                else:
+                    del dones[team]
+
+            # Record episode statistics
+            for agent in self._teams:
+                self._epoch_lengths[agent] += 1
+                self._epoch_returns[agent] += rewards[agent]
+
+                if scope.record_episode_statistics and dones[agent]:
+                    #TODO: Resolve this with global infos
+                    if 'episode' not in infos:
+                        infos['episode'] = {}
+                        infos['episode']['r'] = []
+                        infos['episode']['l'] = []
+
+                    infos['episode']['r'].append(self._epoch_returns[agent])
+                    infos['episode']['l'].append(self._epoch_lengths[agent])
+
+                    self._epoch_lengths[agent] = 0
+                    self._epoch_returns[agent] = 0
+
+            # Observation shape test
+            if __debug__:
+                for team, ob in obs.items():
+                    if not self.observation_space(agent).contains(ob):
+                        raise ValueError(
+                            f'observation:\n{ob}\n for agent/team {team} not in '
+                            f'observation space:\n{self.observation_space(team)}'
+                        )
+
+            return obs, rewards, dones, infos
+
+        @property
+        def timers(self):
+            return self._timers
+
+        @property
+        def max_agents(self):
+            return len(self._teams)
+
+        @property
+        def raw_single_observation_space(self):
+            '''The observation space of a single agent after featurization but before flattening
+
+            Used by _unpack_batched_obs at the start of the network forward pass
+            '''
+            return self._raw_observation_space[self.default_team]
+
+        @property
+        def single_observation_space(self):
+            '''The observation space of a single agent after featurization and flattening'''
+            return self._flat_observation_space[self.default_team]
+
+        @property
+        def single_action_space(self):
+            '''The action space of a single agent after flattening'''
+            return self._flat_action_space[self.default_team]
+
+        def close(self):
+            if not self.initialized:
+                raise exceptions.APIUsageError('close() called before reset()')
+
+            self.env.close()
+
+        @utils.profile
+        def observation_space(self, team):
+            if team not in self._teams:
+                raise exceptions.InvalidAgentError(team, self._teams)
+
+            #Flattened (Box) and cached observation space
+            if team in self.obs_space_cache:
+                return self.obs_space_cache[team]
+
+            team_obs = self._group_by_team(raw_obs)[team]
+
+            # Initialize obs with dummy postprocessor
+            postprocessor = scope.postprocessor_cls(
+                self.env, self._teams, team, *scope.postprocessor_args, **scope.postprocessor_kwargs
+            )
+            postprocessor.reset(team_obs)
+            obs = postprocessor.features(team_obs, self._step)
+
+            # Flatten and cache observation space
+            self._raw_observation_space[team] = _make_space_like(obs)
+            self._flat_observation_space[team] = _flatten_space(self._raw_observation_space[team])
+
+            # TODO: Add checks on return dtype etc... this should not trigger
+            if not self._raw_observation_space[team].contains(obs):
+                print({e: self._raw_observation_space[team][0][e].contains(obs[0][e]) for e in obs[0].keys()})
+            assert self._raw_observation_space[team].contains(obs)
+
+            # Flatten obs to arrays
+            if scope.emulate_flat_obs:
+                obs = _flatten_to_array(obs, self._flat_observation_space[team], scope.obs_dtype)
+
+            self.pad_obs = 0 * obs
+            obs_space = gym.spaces.Box(
+                low=self._obs_min, high=self._obs_max,
+                shape=obs.shape, dtype=scope.obs_dtype
+            )
+
+            return obs_space
+
+        @utils.profile
+        def action_space(self, team):
+            if team not in self._teams:
+                raise exceptions.InvalidAgentError(team, self._teams)
+
+            #Flattened (MultiDiscrete) and cached action space
+            if team in self.atn_space_cache:
+                return self.atn_space_cache[team]
+
+            atn_space = gym.spaces.Dict({a: self.env.action_space(a) for a in self._teams[team]})
+
+            self._flat_action_space[team] = _flatten_space(atn_space)
+            for agent in self._teams[team]:
+                self._agent_action_space[agent] = _flatten_space(atn_space[agent])
+
+            if scope.emulate_flat_atn:
+                assert(isinstance(atn_space, gym.Space)), 'Arg must be a gym space'
+
+                if isinstance(atn_space, (gym.spaces.Discrete, gym.spaces.MultiDiscrete)):
+                    return atn_space
+
+                flat = _flatten_space(atn_space)
+
+                lens = []
+                for e in flat.values():
+                    if isinstance(e, gym.spaces.Discrete):
+                        lens.append(e.n)
+                    elif isinstance(e, gym.spaces.MultiDiscrete):
+                        lens += e.nvec.tolist()
+                    else:
+                        raise ValueError(f'Invalid action space: {e}')
+
+                atn_space = gym.spaces.MultiDiscrete(lens)
+
+            return atn_space
+
+        @utils.profile
+        def reset(self, seed=None):
+            #Reset the environment and return observations
+            self._epoch_returns = defaultdict(float)
+            self._epoch_lengths = defaultdict(int)
+
+            obs = self._reset_env(seed)
+            obs = self._group_by_team(obs)
+            for team_id, team_ob in obs.items():
+                self.postprocessors[team_id].reset(team_ob)
+                obs[team_id] = self._featurize(team_ob, team_id)
+
+            self.agents = self.env.agents
+            self.initialized = True
+            self.done = False
+
+            # Sort observations according to possible_agents
+            # All keys must be present in possible_agents on reset
+            obs = {a: obs[a] for a in self.possible_agents}
+
+            orig_obs = obs
+            if scope.emulate_flat_obs:
+                obs = {team_id: _flatten_to_array(
+                    team_ob, self._flat_observation_space[team_id], scope.obs_dtype)
+                    for team_id, team_ob in obs.items()}
+
+            if __debug__:
+                for agent, ob in obs.items():
+                    assert self.observation_space(agent).contains(ob)
+
+                packed_obs = np.stack(list(obs.values()))
+                unpacked = unpack_batched_obs(self._flat_observation_space[self.default_team], packed_obs)
+                ret = utils._compare_observations(orig_obs, unpacked)
+                assert ret, 'Observation packing/unpacking mismatch'
+
+            self._step = 0
+            return obs
+
+        @utils.profile
+        def step(self, team_actions, **kwargs):
+            #Step the environment and return (observations, rewards, dones, infos)
+            if not self.initialized:
+                raise exceptions.APIUsageError('step() called before reset()')
+
+            if self.done:
+                raise exceptions.APIUsageError('step() called after environment is done')
+
+            actions = self._prestep(team_actions)
+            obs, rewards, dones, infos = self._step_env(actions)
+
+            self.agents = self.env.agents
+            num_agents = len(self.agents)
+            self.done = num_agents == 0
+            self._step += 1
+
+            # Inject number of agent steps into timer logs
+            if not hasattr(self._timers['step'], 'total_agent_steps'):
+                self._timers['step'].total_agent_steps = 0
+            self._timers['step'].total_agent_steps += num_agents
+
+            obs, rewards, dones, infos = self._poststep(obs, rewards, dones, infos)
+            return obs, rewards, dones, infos
+
+    return PufferEnv
+
+
+class Binding:
     def __init__(self,
-            env_cls=None, 
+            env_cls=None,
             env_creator=None,
             default_args=[],
             default_kwargs={},
             env_name=None,
-            feature_parser=None,
-            reward_shaper=None,
+            postprocessor_cls=Postprocessor,
+            postprocessor_args=[],
+            postprocessor_kwargs={},
+            teams=None,
             emulate_flat_obs=True,
             emulate_flat_atn=True,
             emulate_const_horizon=None,
             emulate_const_num_agents=True,
-            suppress_env_prints=True,
+            suppress_env_prints=__debug__,
             record_episode_statistics=True,
             obs_dtype=np.float32):
         '''PufferLib's core Binding class.
-        
+
         Wraps the provided Gym or PettingZoo environment in a PufferEnv that
         behaves like a normal PettingZoo environment with several simplifications:
             - The observation space is flattened to a single vector
             - The action space is flattened to a single vector
             - The environment caches observation and action spaces for improved performance
             - The environment is reset to a fixed horizon
             - The environment is padded to a fixed number of agents in sorted order
@@ -102,495 +551,259 @@
             - The environment records additional statistics
             - The environment has suppressed stdout and stderr to avoid poluting the console
             - The environment contains additional error checking
 
         The Binding class additionally provides utility functions for interacting with complex
         observation and action spaces.
 
-        Args: 
+        Args:
             env_cls: Environment class to wrap. Specify this or env_creator
             env_creator: Environment creation function to wrap. Specify this or env_cls
             default_args: Default arguments for binding.env_creator and binding.raw_env_creator
             default_kwargs: Default keyword arguments for binding.env_creator and binding.raw_env_creator
             env_name: Name of the environment
-            feature_parser: Feature parser to use
-            reward_shaper: Reward shaper to use
+            postprocessor_cls: Postprocessor subclass to use
             emulate_flat_obs: Whether the observation space requires flattening
             emulate_flat_atn: Whether the action space requires flattening
             emulate_const_horizon: Fixed max horizon for resets, None if not applicable
             emulate_const_num_agents: Whether to pad to len(env.possible_agents) observations
             suppress_env_prints: Whether to consume all environment prints
             record_episode_statistics: Whether to record additional episode statistics
             obs_dtype: Observation data type
         '''
-        assert (env_cls is None) != (env_creator is None), \
-            'Specify only one of env_cls (preferred) or env_creator'
+        if (env_cls is None) == (env_creator is None):
+            raise ValueError(
+                f'Invalid combination of env_cls={env_cls} and env_creator={env_creator}.'
+                ' Specify exactly one one of env_cls (preferred) or env_creator'
+            )
 
         self._env_name = env_name
         self._default_args = default_args
         self._default_kwargs = default_kwargs
+        self._obs_dtype = obs_dtype
 
         self._raw_env_cls = env_cls
         self._raw_env_creator = env_creator
         self._suppress_env_prints = suppress_env_prints
 
-        raw_local_env = self.raw_env_creator()
-
-        # TODO: Consider integrating these?
-        # env = wrappers.AssertOutOfBoundsWrapper(env)
-        # env = wrappers.OrderEnforcingWrapper(env)
-
-        class PufferEnv(ParallelEnv):
-            @utils.profile
-            def _create_env(self, *args, **kwargs):
-                with utils.Suppress() if suppress_env_prints else nullcontext():
-                    if env_cls is None:
-                        return env_creator(*args, **kwargs)
-                    else:
-                        return env_cls(*args, **kwargs) 
-
-            @utils.profile
-            def _reset_env(self):
-                with utils.Suppress() if suppress_env_prints else nullcontext():
-                    return self.env.reset()
+        scope = utils.dotdict(locals())
+        del scope['self']
 
-            @utils.profile
-            def _step_env(self, actions):
-                with utils.Suppress() if suppress_env_prints else nullcontext():
-                    return self.env.step(actions)
-
-            @utils.profile
-            def __init__(self, *args, env=None, **kwargs):
-                # Populated by utils.profile decorator
-                self.timers = {}
-                self.prestep_timer = utils.Profiler()
-                self.poststep_timer = utils.Profiler()
-                self.timers['prestep_timer'] = self.prestep_timer
-                self.timers['poststep_timer'] = self.poststep_timer
+        raw_local_env = self.pz_env_creator()
 
-                if env is None:
-                    self.env = self._create_env(*args, **kwargs)
-                else:
-                    self.env = env
+        try:
+            raw_local_env.seed(42)
+            old_seed=True
+        except:
+            old_seed=False
 
-                self.dummy_obs = {}
-                self._step = 0
-                self.done = False
-                self.obs_dtype = obs_dtype
-
-                self.feature_parser = feature_parser
-                self.reward_shaper = reward_shaper
-
-                self.emulate_flat_obs = emulate_flat_obs
-                self.emulate_flat_atn = emulate_flat_atn
-                self.emulate_const_horizon = emulate_const_horizon
-                self.emulate_const_num_agents = emulate_const_num_agents
-                self.emulate_multiagent = not utils.is_multiagent(self.env)
-                self.suppress_env_prints = suppress_env_prints
-                self.record_episode_statistics = record_episode_statistics
-
-                # Standardize property vs method obs/atn space interface
-                if self.emulate_multiagent:
-                    self.possible_agents = [1]
-                else:
-                    self.possible_agents = self.env.possible_agents
-
-                # Manual LRU since functools.lru_cache is not pickleable
-                self.observation_space_cache = {}
-                self.action_space_cache = {}
-
-                # Cache observation and action spaces
-                if self.emulate_const_num_agents:
-                    for agent in self.possible_agents:
-                        self.observation_space(agent)
-                        self.action_space(agent)
-
-                # Set env metadata
-                if hasattr(self.env, 'metadata'):
-                    self.metadata = self.env.metadata
-                else:
-                    self.metadata = {}
-
-            @property
-            def max_agents(self):
-                return len(self.possible_agents)
-
-            @utils.profile
-            def action_space(self, agent):
-                '''Flattened (MultiDiscrete) and cached action space'''
-
-                if agent in self.action_space_cache:
-                    return self.action_space_cache[agent]
-
-                # Get single/multiagent action space
-                if self.emulate_multiagent:
-                    atn_space = self.env.action_space
-                else:
-                    atn_space = self.env.action_space(agent)
-
-                if self.emulate_flat_atn:
-                    assert type(atn_space) in (gym.spaces.Dict, gym.spaces.Discrete, gym.spaces.MultiDiscrete)
-                    if type(atn_space) == gym.spaces.Dict:
-                        atn_space = _pack_atn_space(atn_space)
-                    elif type(atn_space) == gym.spaces.Discrete:
-                        atn_space = gym.spaces.MultiDiscrete([atn_space.n])
-                    
-                self.action_space_cache[agent] = atn_space
-
-                return atn_space
-
-            @utils.profile
-            def observation_space(self, agent: int):
-                '''Flattened (Box) and cached observation space'''
-                if agent in self.observation_space_cache:
-                    return self.observation_space_cache[agent]
-
-                # Get single/multiagent observation space
-                if self.emulate_multiagent:
-                    obs_space = self.env.observation_space
-                else:
-                    obs_space = self.env.observation_space(agent)
+        if old_seed:
+            raw_obs = raw_local_env.reset()
+        else:
+            raw_obs = raw_local_env.reset(seed=42)
 
-                if agent not in self.dummy_obs:
-                    self.dummy_obs[agent] = _zero(obs_space.sample())
+        self._env_cls = make_puffer_env_cls(scope, raw_obs=raw_obs)
 
-                dummy = self.dummy_obs[agent]
+        local_env = self._env_cls(scope, env=raw_local_env)
 
-                if self.feature_parser:
-                    dummy = self.feature_parser({agent: dummy}, self._step)[agent]
+        self._default_agent = local_env.possible_agents[0]
+        self._max_agents = local_env.max_agents
 
-                if self.emulate_flat_obs:
-                    dummy = _flatten_ob(dummy, self.obs_dtype)
+        self._single_observation_space = local_env.observation_space(self._default_agent)
+        self._single_action_space = local_env.action_space(self._default_agent)
 
-                obs_space = gym.spaces.Box(
-                    low=-2**20, high=2**20,
-                    shape=dummy.shape, dtype=self.obs_dtype
-                )
+        self._featurized_single_observation_space = local_env.single_observation_space
+        self._raw_featurized_single_observation_space = local_env.raw_single_observation_space
 
-                self.observation_space_cache[agent] = obs_space
-                return obs_space
+        self._raw_single_observation_space = raw_local_env.observation_space(self._default_agent)
+        self._raw_single_action_space = raw_local_env.action_space(self._default_agent)
 
-            @utils.profile
-            def _process_obs(self, obs):
-                '''Process observation. Shared by reset and step.'''
-                if self.emulate_const_num_agents:
-                    for k in self.dummy_obs:
-                        if k not in obs:                                                  
-                            obs[k] = self.dummy_obs[k]
-
-                if self.feature_parser:
-                    obs = self.feature_parser(obs, self._step)
-
-                if self.emulate_flat_obs:
-                    obs = _pack_obs(obs, self.obs_dtype)
-
-                return obs
-
-            def seed(self, seed):
-                '''Seed the environment. Note that this is deprecated in new gym versions.'''
-                self.env.seed(seed)
-
-            @utils.profile
-            def reset(self):
-                '''Reset the environment and return observations'''
-                self._epoch_returns = defaultdict(float)
-                self._epoch_lengths = defaultdict(int)
-
-                self.reset_calls_step = False
-                obs = self._reset_env()
-
-                if self.emulate_multiagent:
-                    obs = {1: obs}
-                    self.agents = [1]
-                else:
-                    self.agents = self.env.agents
+    @property
+    def raw_env_cls(self):
+        '''Returns the original, unwrapped environment class used to create this binding, if available'''
+        if self._raw_env_cls is None:
+            raise ValueError('raw_env_cls not available when binding is not passed an env_cls')
+        return self._raw_env_cls
 
-                self.done = False
+    def raw_env_creator(self):
+        '''Returns the original, unwrapped env_creator function used to create this binding'''
+        with utils.Suppress() if self._suppress_env_prints else nullcontext():
+            if self._raw_env_cls is None:
+                return self._raw_env_creator(*self._default_args, **self._default_kwargs)
+            else:
+                return self._raw_env_cls(*self._default_args, **self._default_kwargs)
 
+    def pz_env_creator(self):
+        '''Returns the partially wrapped PettingZoo env_creator function created by this binding'''
+        raw_env = self.raw_env_creator()
 
-                # Some envs implement reset by calling step
-                if not self.reset_calls_step:
-                    obs = self._process_obs(obs)
-
-                self._step = 0
-                return obs
-
-            @utils.profile
-            def step(self, actions, **kwargs):
-                '''Step the environment and return (observations, rewards, dones, infos)'''
-                assert not self.done, 'step after done'
-                self.reset_calls_step = True
-
-                # Action shape test
-                if __debug__:
-                    for agent, atns in actions.items():
-                        assert self.action_space(agent).contains(atns)
-
-                # Unpack actions
-                with self.prestep_timer:
-                    if self.emulate_flat_atn:
-                        for k in list(actions):
-                            if k not in self.agents:
-                                del(actions[k])
-                                continue
-
-                            v = actions[k]
-                            if self.emulate_multiagent:
-                                orig_atn_space = self.env.action_space
-                            else:
-                                orig_atn_space = self.env.action_space(k)
-
-                            if type(orig_atn_space) == gym.spaces.Discrete:
-                                actions[k] = v[0]
-                            else:
-                                actions[k] = _unflatten(v, orig_atn_space)
-
-                if self.emulate_multiagent:
-                    action = actions[1]
-
-                    ob, reward, done, info = self._step_env(action)
-
-                    obs = {1: ob}
-                    rewards = {1: reward}
-                    dones = {1: done}
-                    infos = {1: info}
-
-                    if done:
-                        self.done = True
-                        self.agents = []
+        if utils.is_multiagent(raw_env):
+            return raw_env
 
-                else:
-                    obs, rewards, dones, infos = self._step_env(actions)
-                    self.agents = self.env.agents
-                    self.done = len(self.agents) == 0
-
-                # RLlib compat 
-                assert '__all__' not in dones, 'Base env should not return __all__'
-
-                self._step += 1
-            
-                obs = self._process_obs(obs)
-
-                with self.poststep_timer:
-                    if self.reward_shaper:
-                        rewards = self.reward_shaper(rewards, self._step)
-
-                    # Terminate episode at horizon or if all agents are done
-                    if self.emulate_const_horizon is not None:
-                        assert self._step <= self.emulate_const_horizon
-                        if self._step == self.emulate_const_horizon:
-                            self.done = True
-
-                    # Computed before padding dones. False if no agents
-                    # Pad rewards/dones/infos
-                    if self.emulate_const_num_agents:
-                        for k in self.dummy_obs:
-                            # TODO: Check that all keys are present
-                            if k not in rewards:
-                                rewards[k] = 0
-                            if k not in infos:
-                                infos[k] = {}
-                            if k not in dones:
-                                dones[k] = self.done
-
-                    # Sort by possible_agents ordering
-                    sorted_obs, sorted_rewards, sorted_dones, sorted_infos = {}, {}, {}, {}
-                    for agent in self.possible_agents:
-                        self._epoch_lengths[agent] += 1
-                        self._epoch_returns[agent] += rewards[agent]
-
-                        if self.record_episode_statistics and dones[agent]:
-                            if 'episode' not in infos[agent]:
-                                infos[agent]['episode'] = {}
-
-                            infos[agent]['episode']['r'] = self._epoch_returns[agent]
-                            infos[agent]['episode']['l'] = self._epoch_lengths[agent]
-
-                            self._epoch_lengths[agent] = 0
-                            self._epoch_returns[agent] = 0
- 
-                        sorted_obs[agent] = obs[agent]
-                        sorted_rewards[agent] = rewards[agent]
-                        sorted_dones[agent] = dones[agent]
-                        sorted_infos[agent] = infos[agent]
-
-                    obs, rewards, dones, infos = sorted_obs, sorted_rewards, sorted_dones, sorted_infos
-
-                    # Observation shape test
-                    if __debug__:
-                        for agent, ob in obs.items():
-                            assert self.observation_space(agent).contains(ob)
+        return GymToPettingZooParallelWrapper(raw_env)
 
-                return obs, rewards, dones, infos
+    @property
+    def env_cls(self):
+        '''Returns wrapped PufferEnv class created by this binding'''
+        return self._env_cls
 
-        self._env_cls = PufferEnv
-        local_env = PufferEnv(env=raw_local_env)
+    def env_creator(self):
+        '''Returns the wrapped PufferEnv env_creator function created by this binding'''
+        return self._env_cls(*self._default_args, **self._default_kwargs)
 
-        self._default_agent = local_env.possible_agents[0]
-        self._max_agents = local_env.max_agents
-        self._emulate_multiagent = local_env.emulate_multiagent
+    @property
+    def raw_single_observation_space(self):
+        '''Returns the unwrapped, structured observation space of a single agent.
 
-        self._single_observation_space = local_env.observation_space(self._default_agent)
-        self._single_action_space = local_env.action_space(self._default_agent)
+        PufferLib currently assumes that all agents share the same observation space'''
+        return self._raw_single_observation_space
 
-        if self._emulate_multiagent:
-            self._raw_single_observation_space = raw_local_env.observation_space
-            self._raw_single_action_space = raw_local_env.action_space
-        else:
-            self._raw_single_observation_space = raw_local_env.observation_space(self._default_agent)
-            self._raw_single_action_space = raw_local_env.action_space(self._default_agent)
+    @property
+    def featurized_single_observation_space(self):
+        '''Returns the wrapped, structured, featurized observation space of a single agent.
 
+        PufferLib currently assumes that all agents share the same observation space'''
+        return self._featurized_single_observation_space
 
-def unpack_batched_obs(obs_space, packed_obs):
-    '''Unpack a batch of observations into the original observation space
-    
-    Call this funtion in the forward pass of your network
-    '''
+    @property
+    def single_observation_space(self):
+        '''Returns the wrapped, flat observation space of a single agent.
 
-    assert(isinstance(obs_space, gym.Space)), 'First arg must be a gym space'
+        PufferLib currently assumes that all agents share the same observation space'''
+        return self._single_observation_space
 
-    batch = packed_obs.shape[0]
-    obs = {}
-    idx = 0
+    @property
+    def raw_single_action_space(self):
+        '''Returns the unwrapped, structured action space of a single agent.
 
-    flat_obs_space = _flatten(obs_space)
+        PufferLib currently assumes that all agents share the same action space'''
+        return self._raw_single_action_space
 
-    for key_list, val in flat_obs_space.items():
-        obs_ptr = obs
-        for key in key_list[:-1]:
-            if key not in obs_ptr:
-                obs_ptr[key] = {}
-            obs_ptr = obs_ptr[key]
-
-        key = key_list[-1]
-        inc = np.prod(val.shape)
-        obs_ptr[key] = packed_obs[:, idx:idx + inc].reshape(batch, *val.shape)
-        idx = idx + inc
+    @property
+    def single_action_space(self):
+        '''Returns the wrapped, flat action space of a single agent.
 
-    return obs
+        PufferLib currently assumes that all agents share the same action space'''
+        return self._single_action_space
 
-def _zero(ob):
-    if type(ob) == np.ndarray:
-        ob.fill(0)
-    elif type(ob) in (dict, OrderedDict):
-        for k, v in ob.items():
-            _zero(ob[k])
-    else:
-        for v in ob:
-            _zero(v)
-    return ob
-
-def _flatten(nested_dict, parent_key=None):
-    types = (gym.spaces.Dict, OrderedDict, list, dict, tuple)
-
-    if type(nested_dict) not in types:
-        return nested_dict
-
-    stack = [((), nested_dict)]
-    flat_dict = {}
-    while stack:
-        path, current = stack.pop()
-        for k, v in current.items():
-            new_key = path + (k,)
-            if type(v) in types:
-                stack.append((new_key, v))
-            else:
-                flat_dict[new_key] = v
+    @property
+    def max_agents(self):
+        '''Returns the maximum number of agents in the environment'''
+        return self._max_agents
 
-    return flat_dict
+    @property
+    def env_name(self):
+        '''Returns the environment name'''
+        return self._env_name
 
-def _unflatten(ary, space, nested_dict=None, idx=0):
-    outer_call = False
-    if nested_dict is None:
-        outer_call = True
-        nested_dict = {}
-
-    # TODO: Find a way to flip the check and the loop
-    # (Added for Gym microrts)
-    if type(space)  == gym.spaces.MultiDiscrete:
-        return ary
-
-    types = (gym.spaces.Dict, OrderedDict, list, dict, tuple)
-    for k, v in space.items():
-        if type(v) in types:
-            nested_dict[k] = {}
-            _, idx = _unflatten(ary, v, nested_dict[k], idx)
-        else:
-            nested_dict[k] = ary[idx]
-            idx += 1
+    def unpack_batched_obs(self, packed_obs):
+        '''Unpack a batch of observations into the original observation space
 
-    if outer_call:
-        return nested_dict
+        Call this funtion in the forward pass of your network
+        '''
+        return unpack_batched_obs(self._featurized_single_observation_space, packed_obs)
 
-    return nested_dict, idx
+    def pack_obs(self, obs):
+        return {k: _flatten_to_array(v, self._featurized_single_observation_space, self._obs_dtype) for k, v in obs.items()}
 
-def _pack_obs_space(obs_space, dtype=np.float32):
-    assert(isinstance(obs_space, gym.Space)), 'Arg must be a gym space'
+def unpack_batched_obs(flat_space, packed_obs):
+    if not isinstance(flat_space, dict):
+        return packed_obs.reshape(packed_obs.shape[0], *flat_space.shape)
 
-    if isinstance(obs_space, gym.spaces.Box):
-        return obs_space
+    batch = packed_obs.shape[0]
 
-    flat = _flatten(obs_space)
+    if () in flat_space:
+        return packed_obs.reshape(batch, *flat_space[()].shape)
 
-    n = 0
-    for e in flat.values():
-        n += np.prod(e.shape)
+    batched_obs = {}
+    idx = 0
 
-    return gym.spaces.Box(
-        low=-2**20, high=2**20,
-        shape=(int(n),), dtype=dtype
-    )
+    for key_list, space in flat_space.items():
+        current_dict = batched_obs
+        inc = np.prod(space.shape)
 
-def _pack_atn_space(atn_space):
-    assert(isinstance(atn_space, gym.Space)), 'Arg must be a gym space'
+        for key in key_list[:-1]:
+            if key not in current_dict:
+                current_dict[key] = {}
+            current_dict = current_dict[key]
 
-    if isinstance(atn_space, gym.spaces.Discrete):
-        return atn_space
+        last_key = key_list[-1]
+        current_dict[last_key] = packed_obs[:, idx:idx + inc].reshape(batch, *space.shape)
+        idx += inc
 
-    flat = _flatten(atn_space)
+    return batched_obs
 
-    lens = []
-    for e in flat.values():
-        lens.append(e.n)
+def _make_space_like(ob):
+    if type(ob) == np.ndarray:
+        mmin, mmax = utils._get_dtype_bounds(ob.dtype)
+        return gym.spaces.Box(
+            low=mmin, high=mmax,
+            shape=ob.shape, dtype=ob.dtype
+        )
+
+    # TODO: Handle Discrete (how to get max?)
+    if type(ob) in (tuple, list):
+        return gym.spaces.Tuple([_make_space_like(v) for v in ob])
+
+    if type(ob) in (dict, OrderedDict):
+        return gym.spaces.Dict({k: _make_space_like(v) for k, v in ob.items()})
+
+    raise ValueError(f'Invalid type for featurized obs: {type(ob)}')
+
+def _flatten_space(space):
+    flat_keys = {}
+
+    def _recursion_helper(current_space, key_list):
+        if isinstance(current_space, (list, tuple, gym.spaces.Tuple)):
+            for idx, elem in enumerate(current_space):
+                new_key_list = key_list + (idx,)
+                _recursion_helper(elem, new_key_list)
+        elif isinstance(current_space, (dict, OrderedDict, gym.spaces.Dict)):
+            for key, value in current_space.items():
+                new_key_list = key_list + (key,)
+                _recursion_helper(value, new_key_list)
+        else:
+            flat_keys[key_list] = current_space
 
-    return gym.spaces.MultiDiscrete(lens) 
+    _recursion_helper(space, ())
+    return flat_keys
 
-def _flatten_ob(ob, dtype=None):
+def _flatten_to_array(space_sample, flat_space, dtype=None):
     # TODO: Find a better way to handle Atari
-    if type(ob) == gym.wrappers.frame_stack.LazyFrames:
-       ob = np.array(ob)
+    if type(space_sample) == gym.wrappers.frame_stack.LazyFrames:
+       space_sample = np.array(space_sample)
 
-    #assert type(ob) == np.array
+    if () in flat_space:
+        if isinstance(space_sample, np.ndarray):
+            return space_sample.reshape(*flat_space[()].shape)
+        return np.array([space_sample])
+
+    tensors = []
+    for key_list in flat_space:
+        value = space_sample
+        for key in key_list:
+            value = value[key]
 
-    flat = _flatten(ob)
+        if not isinstance(value, np.ndarray):
+            value = np.array([value])
 
-    if type(ob) == np.ndarray:
-        flat = {'': flat}
+        tensors.append(value.ravel())
 
     # Preallocate the memory for the concatenated tensor
-    tensors = flat.values()
+    if type(tensors) == dict:
+        tensors = tensors.values()
 
     if dtype is None:
         tensors = list(tensors)
         dtype = tensors[0].dtype
 
-    tensor_sizes = [tensor.size for tensor in tensors] 
+    tensor_sizes = [tensor.size for tensor in tensors]
     prealloc = np.empty(sum(tensor_sizes), dtype=dtype)
 
     # Fill the concatenated tensor with the flattened tensors
     start = 0
     for tensor, size in zip(tensors, tensor_sizes):
         end = start + size
         prealloc[start:end] = tensor.ravel()
         start = end
 
     return prealloc
-
-def _pack_obs(obs, dtype=None):
-    return {k: _flatten_ob(v, dtype) for k, v in obs.items()}
-
-def _batch_obs(obs):
-    return np.stack(list(obs.values()), axis=0)
-
-def _pack_and_batch_obs(obs):
-    obs = _pack_obs(obs)
-    return _batch_obs(obs)
```

### Comparing `pufferlib-0.2.1/pufferlib/evaluation.py` & `pufferlib-0.3.0/pufferlib/evaluation.py`

 * *Files identical despite different names*

### Comparing `pufferlib-0.2.1/pufferlib/frameworks/cleanrl.py` & `pufferlib-0.3.0/pufferlib/frameworks/cleanrl.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,71 +4,83 @@
 from torch.distributions import Categorical
 
 import pufferlib
 import pufferlib.models
 import pufferlib.frameworks.base
 
 
-def make_policy(policy_cls, lstm_layers=0):
+def make_policy(policy_cls, recurrent_cls=torch.nn.LSTM,
+        recurrent_args=[512, 128], recurrent_kwargs={'num_layers': 1}):
     '''Wrap a PyTorch model for use with CleanRL
 
     Args:
         policy_cls: A pufferlib.models.Policy subclass that implements the PufferLib model API
-        lstm_layers: The number of LSTM layers to use. If 0, no LSTM is used
+        recurrent_cls: Recurrent cell class to use. Defaults to torch.nn.LSTM.
+        recurrent_args: Args to pass to recurrent_cls. Defaults to 512, 128 for LSTM.
+        recurrent_kwargs: Kwargs to pass to recurrent_cls. Defaults to num_layers: 1 for LSTM. Set num_layers to 0 to disable the recurrent cell.
 
     Returns:
         A new PyTorch class wrapping your model that implements the CleanRL API
     '''
     assert issubclass(policy_cls, pufferlib.models.Policy)
-    if lstm_layers > 0:
-        policy_cls = pufferlib.frameworks.base.make_recurrent_policy(
-            policy_cls, batch_first=False)
 
-    class CleanRLPolicy(policy_cls):
-        '''Temporary hack to get framework running with CleanRL
+    # Defaults for LSTM
+    if recurrent_cls == torch.nn.LSTM:
+        if len(recurrent_args) == 0:
+            recurrent_args = [512, 128]
+        if len(recurrent_kwargs) == 0:
+            recurrent_args = {'num_layers': 1}
 
-        Their LSTMs are kind of weird. Need to figure this out'''
-        def __init__(self, *args, **kwargs):
-            super().__init__(*args, **kwargs)
+    is_recurrent = recurrent_kwargs['num_layers'] != 0
+    if is_recurrent:
+        policy_cls = pufferlib.frameworks.base.make_recurrent_policy(
+            policy_cls, recurrent_cls, *recurrent_args, **recurrent_kwargs)
 
+    class CleanRLPolicy(policy_cls):
         def _compute_hidden(self, x, lstm_state=None):
-            if lstm_layers > 0:
+            if is_recurrent:
                 batch_size = lstm_state[0].shape[1]
                 x = x.reshape((-1, batch_size, x.shape[-1]))
                 hidden, state, lookup = self.encode_observations(x, lstm_state)
-                return hidden, state
+                return hidden, state, lookup
             else:
-                hidden, _ = self.encode_observations(x)
+                hidden, lookup = self.encode_observations(x)
 
-            return hidden
+            return hidden, lookup
+
+        @property
+        def lstm(self):
+            return self.recurrent_policy
 
         # TODO: Cache value
         def get_value(self, x, lstm_state=None, done=None):
-            if lstm_layers > 0:
-                hidden, lstm_state = self._compute_hidden(x, lstm_state)
+            if is_recurrent:
+                hidden, lstm_state, lookup = self._compute_hidden(x, lstm_state)
             else:
-                hidden = self._compute_hidden(x, lstm_state)
+                hidden, lookup = self._compute_hidden(x)
             return self.critic(hidden)
 
         # TODO: Compute seq_lens from done
         def get_action_and_value(self, x, lstm_state=None, done=None, action=None):
-            if lstm_layers > 0:
-                hidden, lstm_state = self._compute_hidden(x, lstm_state)
+            if is_recurrent:
+                hidden, lstm_state, lookup = self._compute_hidden(x, lstm_state)
             else:
-                hidden = self._compute_hidden(x, lstm_state)
+                hidden, lookup = self._compute_hidden(x)
 
             value = self.critic(hidden)
-            flat_logits = self.decode_actions(hidden, None, concat=False)
-
+            flat_logits = self.decode_actions(hidden, lookup, concat=False)
             multi_categorical = [Categorical(logits=l) for l in flat_logits]
 
             if action is None:
                 action = torch.stack([c.sample() for c in multi_categorical])
             else:
                 action = action.view(-1, action.shape[-1]).T
 
             logprob = torch.stack([c.log_prob(a) for c, a in zip(multi_categorical, action)]).T.sum(1)
             entropy = torch.stack([c.entropy() for c in multi_categorical]).T.sum(1)
 
-            return action.T, logprob, entropy, value, lstm_state
-   
+            if is_recurrent:
+                return action.T, logprob, entropy, value, lstm_state
+            else:
+                return action.T, logprob, entropy, value
+
     return CleanRLPolicy
```

### Comparing `pufferlib-0.2.1/pufferlib/frameworks/rllib.py` & `pufferlib-0.3.0/pufferlib/frameworks/rllib.py`

 * *Files identical despite different names*

### Comparing `pufferlib-0.2.1/pufferlib/models.py` & `pufferlib-0.3.0/pufferlib/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from abc import ABC, abstractmethod
 
 import torch
 import torch.nn as nn
 
 
 class Policy(torch.nn.Module, ABC):
-    def __init__(self, binding, input_size, hidden_size):
+    def __init__(self, binding):
         '''Pure PyTorch base policy
         
         This spec allows PufferLib to repackage your policy
         for compatibility with RL frameworks
 
         encode_observations -> decode_actions is PufferLib's equivalent of PyTorch forward
         This structure provides additional flexibility for us to include an LSTM
@@ -27,21 +27,17 @@
 
         Specify the value function in critic(). This is a single value for each batch element.
         It is called on the output of the recurrent cell (or, if no recurrent cell,
         the output of encode_observations)
 
         Args:
             binding: A pufferlib.emulation.Binding object
-            input_size: The size of the input to the recurrent cell 
-            hidden_size: The size of the output of the recurrent cell
         '''
         super().__init__()
         self.binding = binding
-        self.input_size = input_size
-        self.hidden_size = hidden_size
 
     @abstractmethod
     def critic(self, hidden):
         '''Computes the value function from the hidden state
         
         Returns a single value for each batch element'''
         raise NotImplementedError
@@ -84,15 +80,15 @@
     def __init__(self, binding, input_size=256, hidden_size=256):
         '''Default PyTorch policy, meant for debugging.
         This should run with any environment but is unlikely to learn anything.
         
         Uses a single linear layer to encode observations and a list of
         linear layers to decode actions. The value function is a single linear layer.
         '''
-        super().__init__(binding, input_size, hidden_size)
+        super().__init__(binding)
         self.encoder = nn.Linear(self.binding.single_observation_space.shape[0], hidden_size)
         self.decoders = nn.ModuleList([nn.Linear(hidden_size, n)
                 for n in self.binding.single_action_space.nvec])
         self.value_head = nn.Linear(hidden_size, 1)
 
     def critic(self, hidden):
         '''Linear value function'''
@@ -103,8 +99,8 @@
         return self.encoder(env_outputs), None
 
     def decode_actions(self, hidden, lookup, concat=True):
         '''Concatenated linear decoder function'''
         actions = [dec(hidden) for dec in self.decoders]
         if concat:
             return torch.cat(actions, dim=-1)
-        return actions
+        return actions
```

### Comparing `pufferlib-0.2.1/pufferlib/rating.py` & `pufferlib-0.3.0/pufferlib/rating.py`

 * *Files identical despite different names*

### Comparing `pufferlib-0.2.1/pufferlib/registry/atari.py` & `pufferlib-0.3.0/pufferlib/registry/atari.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,17 @@
         obs = np.zeros(0)
         for _ in range(noops):
             obs, _, done, _ = self.env.step(self.noop_action)
             if done:
                 obs = self.env.reset(**kwargs)
         return obs
 
+class AtariFeaturizer(pufferlib.emulation.Postprocessor):
+    def features(self, obs, step):
+        return np.array(obs[1], dtype=np.float32).ravel()
 
 def make_env(env_name, framestack):
     '''Atari creation function with default CleanRL preprocessing based on Stable Baselines3 wrappers'''
     try:
         with pufferlib.utils.Suppress():
             env = gym.make(env_name)
     except ImportError as e:
@@ -81,56 +84,57 @@
     except:
         raise pufferlib.utils.SetupError(f'{env_name} (ale)')
     else:
         return pufferlib.emulation.Binding(
             env_creator=make_env,
             default_args=[env_name, framestack],
             env_name=env_name,
+            postprocessor_cls=AtariFeaturizer,
             emulate_flat_atn=True,
             record_episode_statistics=False,
         )
 
 def layer_init(layer, std=np.sqrt(2), bias_const=0.0):
     '''CleanRL's default layer initialization'''
     torch.nn.init.orthogonal_(layer.weight, std)
     torch.nn.init.constant_(layer.bias, bias_const)
     return layer
 
 class Policy(pufferlib.models.Policy):
-    def __init__(self, binding, *args, framestack, input_size=512, hidden_size=512, **kwargs):
+    def __init__(self, binding, *args, framestack, input_size=512, hidden_size=128, **kwargs):
         '''The CleanRL default Atari policy: a stack of three convolutions followed by a linear layer
         
         Takes framestack as a mandatory keyword arguments. Suggested default is 1 frame
         with LSTM or 4 frames without.'''
-        super().__init__(binding, input_size, hidden_size, *args, **kwargs)
+        super().__init__(binding)
         self.observation_space = binding.raw_single_observation_space
         self.num_actions = binding.raw_single_action_space.n
 
         self.network = nn.Sequential(
             layer_init(nn.Conv2d(framestack, 32, 8, stride=4)),
             nn.ReLU(),
             layer_init(nn.Conv2d(32, 64, 4, stride=2)),
             nn.ReLU(),
             layer_init(nn.Conv2d(64, 64, 3, stride=1)),
             nn.ReLU(),
             nn.Flatten(),
-            layer_init(nn.Linear(64 * 7 * 7, self.hidden_size)),
+            layer_init(nn.Linear(64 * 7 * 7, input_size)),
             nn.ReLU(),
         )
 
-        self.actor = layer_init(nn.Linear(self.hidden_size, self.num_actions), std=0.01)
-        self.value_function = layer_init(nn.Linear(self.hidden_size, 1), std=1)
+        self.actor = layer_init(nn.Linear(hidden_size, self.num_actions), std=0.01)
+        self.value_function = layer_init(nn.Linear(hidden_size, 1), std=1)
 
     def critic(self, hidden):
         return self.value_function(hidden)
 
     def encode_observations(self, flat_observations):
         # TODO: Add flat obs support to emulation
         batch = flat_observations.shape[0]
         observations = flat_observations.reshape((batch,) + self.observation_space.shape)
         return self.network(observations / 255.0), None
 
     def decode_actions(self, flat_hidden, lookup, concat=None):
         action = self.actor(flat_hidden)
         if concat:
             return action
-        return [action]
+        return [action]
```

### Comparing `pufferlib-0.2.1/pufferlib/registry/butterfly.py` & `pufferlib-0.3.0/pufferlib/registry/butterfly.py`

 * *Files identical despite different names*

### Comparing `pufferlib-0.2.1/pufferlib/registry/classic_control.py` & `pufferlib-0.3.0/pufferlib/registry/classic_control.py`

 * *Files identical despite different names*

### Comparing `pufferlib-0.2.1/pufferlib/registry/griddly.py` & `pufferlib-0.3.0/pufferlib/registry/griddly.py`

 * *Files identical despite different names*

### Comparing `pufferlib-0.2.1/pufferlib/registry/magent.py` & `pufferlib-0.3.0/pufferlib/registry/magent.py`

 * *Files identical despite different names*

### Comparing `pufferlib-0.2.1/pufferlib/registry/microrts.py` & `pufferlib-0.3.0/pufferlib/registry/microrts.py`

 * *Files identical despite different names*

### Comparing `pufferlib-0.2.1/pufferlib/registry/nethack.py` & `pufferlib-0.3.0/pufferlib/registry/nethack.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,16 @@
         )
 
 
 class Policy(pufferlib.models.Policy):
     '''Default NetHack Learning Environment policy ported from the nle release'''
     def __init__(self, binding, *args,
             embedding_dim=32, crop_dim=9, num_layers=5,
-            input_size=512, hidden_size=512,
             **kwargs):
-        super().__init__(binding, input_size, hidden_size, *args, **kwargs)
+        super().__init__(binding, *args, **kwargs)
 
         self.observation_shape = binding.raw_single_observation_space
         self.glyph_shape = self.observation_shape["glyphs"].shape
         self.blstats_size = self.observation_shape["blstats"].shape[0]
 
         self.num_actions = binding.raw_single_action_space.n
 
@@ -215,8 +214,8 @@
             torch.round(F.grid_sample(inputs, grid, align_corners=True))
             .squeeze(1)
             .long()
         )
 
 def _step_to_range(delta, num_steps):
     """Range of `num_steps` integers with distance `delta` centered around zero."""
-    return delta * torch.arange(-num_steps // 2, num_steps // 2)
+    return delta * torch.arange(-num_steps // 2, num_steps // 2)
```

### Comparing `pufferlib-0.2.1/pufferlib/registry/nmmo.py` & `pufferlib-0.3.0/pufferlib/registry/nmmo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pdb import set_trace as T
 
 import torch
 
 import pufferlib
 import pufferlib.emulation
+import pufferlib.models
 
 
 def make_binding():
     '''Neural MMO binding creation function'''
     try:
         import nmmo
     except:
@@ -16,37 +17,37 @@
         return pufferlib.emulation.Binding(
             env_cls=nmmo.Env,
             env_name='Neural MMO',
         )
 
 
 class Policy(pufferlib.models.Policy):
-    def __init__(self, binding, input_size=512, hidden_size=512):
+    def __init__(self, binding, input_size=512, hidden_size=128):
         '''Default Neural MMO policy
         
         This is a dummy placeholder used to speed up tests because of the size of the
         Neural MMO observation space. It is not a good policy and will not learn anything.'''
-        super().__init__(binding, input_size, hidden_size)
-        self.raw_single_observation_space = binding.raw_single_observation_space
+        super().__init__(binding)
+        self.featurized_single_observation_space = binding.featurized_single_observation_space
 
         # A dumb example encoder that applies a linear layer to agent self features
         observation_size = binding.raw_single_observation_space['Entity'].shape[1]
-        self.encoder = torch.nn.Linear(observation_size, hidden_size)
+        self.encoder = torch.nn.Linear(observation_size, input_size)
 
         self.decoders = torch.nn.ModuleList([torch.nn.Linear(hidden_size, n)
                 for n in binding.single_action_space.nvec])
         self.value_head = torch.nn.Linear(hidden_size, 1)
 
     def critic(self, hidden):
         return self.value_head(hidden)
 
     def encode_observations(self, env_outputs):
         env_outputs = pufferlib.emulation.unpack_batched_obs(
-            self.raw_single_observation_space, env_outputs)
-        env_outputs = env_outputs['Entity'][:, 0, :]
+            self.featurized_single_observation_space, env_outputs)
+        env_outputs = env_outputs[0]['Entity'][:, 0, :]
         return self.encoder(env_outputs), None
 
     def decode_actions(self, hidden, lookup, concat=True):
         actions = [dec(hidden) for dec in self.decoders]
         if concat:
             return torch.cat(actions, dim=-1)
         return actions
```

### Comparing `pufferlib-0.2.1/pufferlib/registry/smac.py` & `pufferlib-0.3.0/pufferlib/registry/smac.py`

 * *Files identical despite different names*

### Comparing `pufferlib-0.2.1/pufferlib/torch.py` & `pufferlib-0.3.0/pufferlib/torch.py`

 * *Files identical despite different names*

### Comparing `pufferlib-0.2.1/pufferlib/vectorization.py` & `pufferlib-0.3.0/pufferlib/vectorization/ray.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,72 +1,19 @@
 from pdb import set_trace as T
 
-import ray
 import numpy as np
 import itertools
+import ray
 
 RESET = 0
 SEND = 1
 RECV = 2
 
-def make_remote_envs(env_creator, n):
-    '''Creates n serial environments on a single remote process
 
-    Called for you by RayVecEnvs
-    
-    Args:
-        env_creator: A function that creates a single environment
-        n: The number of environments to create
-
-    Returns:
-        A Ray-backed RemoteEnvs object. Used internally by RayVecEnvs
-    '''
-    @ray.remote
-    class RemoteEnvs:
-        def __init__(self):
-            self.envs = [env_creator() for _ in range(n)]
-
-        def seed(self, seed):
-            for env in self.envs:
-                env.seed(seed)
-                seed += 1
-
-        def profile_all(self):
-            return [e.timers for e in self.envs]
-
-        def put_all(self, *args, **kwargs):
-            for e in self.envs:
-                e.put(*args, **kwargs)
-            
-        def get_all(self, *args, **kwargs):
-            return [e.get(*args, **kwargs) for e in self.envs]
-        
-        def reset_all(self):
-            return [(e.reset(), {}, {}, {}) for e in self.envs]
-
-        def step(self, actions_lists):
-            returns = []
-            assert len(self.envs) == len(actions_lists)
-            for env, actions in zip(self.envs, actions_lists):
-                if env.done:
-                    obs = env.reset()
-                    rewards = {k: 0 for k in obs}
-                    dones = {k: False for k in obs}
-                    infos = {k: {} for k in obs}
-                else:
-                    obs, rewards, dones, infos = env.step(actions)
-
-                returns.append((obs, rewards, dones, infos))
-
-            return returns
-
-    return RemoteEnvs.remote()
-
-
-class RayVecEnv:
+class VecEnv:
     def __init__(self, binding, num_workers, envs_per_worker=1):
         '''Creates env_per_worker serial environments on each of num_workers remote processes
 
         Synchronous API: Use env.reset() and env.step(actions)
 
         Asynchronous API: Use env.async_reset(), env.send(actions), and env.recv(actions)
         This confers no advantage unless you are using multiple RayVecEnvs in a double-buffered
@@ -76,30 +23,30 @@
             binding: A pufferlib.emulation.Binding object
             num_workers: The number of remote processes to create
             envs_per_worker: The number of serial environments to create on each remote process
         '''
         assert envs_per_worker > 0, 'Each worker must have at least 1 env'
         assert type(envs_per_worker) == int
 
-        ray.init(
-            include_dashboard=False, # WSL Compatibility
-            ignore_reinit_error=True,
-        )
-
         self.binding = binding
         self.num_workers = num_workers
         self.envs_per_worker = envs_per_worker
 
         self.state = RESET
 
+        ray.init(
+            include_dashboard=False, # WSL Compatibility
+            ignore_reinit_error=True,
+        )
+
         self.remote_envs_lists = [
-            make_remote_envs(
-                binding.env_creator,
-                envs_per_worker,
-            ) for idx in range(num_workers)
+            make_remote_ray_envs(
+                self.binding.env_creator,
+                self.envs_per_worker,
+            ) for idx in range(self.num_workers)
         ]
 
     @property
     def single_observation_space(self):
         '''Convenience function; returns self.binding.single_observation_space'''
         return self.binding.single_observation_space
 
@@ -113,27 +60,25 @@
         #TODO: Implement close
         pass
 
     def profile(self):
         '''Returns profiling timers from all remote environments'''
         return list(itertools.chain.from_iterable(ray.get([e.profile_all.remote() for e in self.remote_envs_lists])))
 
-    def seed(self, seed):
-        '''Sets the seed for all remote environments'''
-        assert type(seed) == int
-        for env_list in self.remote_envs_lists:
-            env_list.seed.remote(seed)
-            seed += self.envs_per_worker * self.binding.max_agents
-
-    def async_reset(self):
+    def async_reset(self, seed=None):
         '''Asynchronously reset environments. Does not block.'''
         assert self.state == RESET, 'Call reset only once on initialization'
         self.state = RECV
 
-        self.async_handles = [e.reset_all.remote() for e in self.remote_envs_lists]
+        self.async_handles = []
+
+        for e in self.remote_envs_lists:
+            self.async_handles.append(e.reset_all.remote(seed=seed))
+            if seed is not None:
+                seed += self.envs_per_worker * self.binding.max_agents
 
     def recv(self):
         '''Receive observations from remote async environments. Blocks.'''
         assert self.state == RECV, 'Call reset before stepping'
         self.state = SEND
 
         self.agent_keys = []
@@ -141,15 +86,15 @@
         for envs in ray.get(self.async_handles):
             a_keys = []
             for o, r, d, i in envs:
                 a_keys.append(list(o.keys()))
                 obs += list(o.values())
                 rewards += list(r.values())
                 dones += list(d.values())
-                infos += list(i.values())
+                infos.append(i)
 
             self.agent_keys.append(a_keys)
 
         obs = np.stack(obs)
 
         return obs, rewards, dones, infos
 
@@ -166,16 +111,75 @@
 
         self.async_handles = []
         for envs_list, keys_list, atns_list in zip(self.remote_envs_lists, self.agent_keys, actions):
             atns_list = np.split(atns_list, self.envs_per_worker)
             atns_list = [dict(zip(keys, atns)) for keys, atns in zip(keys_list, atns_list)]
             self.async_handles.append(envs_list.step.remote(atns_list))
 
-    def reset(self):
+    def reset(self, seed=None):
         '''Syncronously resets remote environments. Blocks.'''
         self.async_reset()
         return self.recv()[0]
 
     def step(self, actions):
         '''Syncronously steps remote environments. Blocks.'''
         self.send(actions)
-        return self.recv()
+        return self.recv()
+
+
+def make_remote_ray_envs(env_creator, n):
+    '''Creates n serial environments on a single remote process
+
+    Called for you by RayVecEnvs
+    
+    Args:
+        env_creator: A function that creates a single environment
+        n: The number of environments to create
+
+    Returns:
+        A Ray-backed RemoteEnvs object. Used internally by RayVecEnvs
+    '''
+    @ray.remote
+    class RemoteEnvs:
+        def __init__(self):
+            self.envs = [env_creator() for _ in range(n)]
+
+        def seed(self, seed):
+            for env in self.envs:
+                env.seed(seed)
+                seed += 1
+
+        def profile_all(self):
+            return [e.timers for e in self.envs]
+
+        def put_all(self, *args, **kwargs):
+            for e in self.envs:
+                e.put(*args, **kwargs)
+            
+        def get_all(self, *args, **kwargs):
+            return [e.get(*args, **kwargs) for e in self.envs]
+        
+        def reset_all(self, seed=None):
+            async_handles = []
+            for e in self.envs:
+                async_handles.append((e.reset(seed=seed), {}, {}, {}))
+                if seed is not None:
+                    seed += 1
+            return async_handles
+
+        def step(self, actions_lists):
+            returns = []
+            assert len(self.envs) == len(actions_lists)
+            for env, actions in zip(self.envs, actions_lists):
+                if env.done:
+                    obs = env.reset()
+                    rewards = {k: 0 for k in obs}
+                    dones = {k: False for k in obs}
+                    infos = {}
+                else:
+                    obs, rewards, dones, infos = env.step(actions)
+
+                returns.append((obs, rewards, dones, infos))
+
+            return returns
+
+    return RemoteEnvs.remote()
```

### Comparing `pufferlib-0.2.1/pufferlib.egg-info/PKG-INFO` & `pufferlib-0.3.0/pufferlib.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pufferlib
-Version: 0.2.1
+Version: 0.3.0
 Summary: PufferAI LibraryPufferAI's library of RL tools and utilities
 Home-page: https://github.com/PufferAI/PufferLib
 Author: Joseph Suarez
 Author-email: jsuarez@mit.edu
 License: MIT
 Keywords: Puffer,AI,RL
 Platform: UNKNOWN
@@ -13,20 +13,24 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: rllib
+Provides-Extra: cleanrl
 Provides-Extra: tests
 Provides-Extra: all
 Provides-Extra: atari
 Provides-Extra: box2d
 Provides-Extra: butterfly
+Provides-Extra: crafter
+Provides-Extra: dm_control
+Provides-Extra: dm_lab
 Provides-Extra: magent
 Provides-Extra: microrts
+Provides-Extra: minerl
 Provides-Extra: nethack
-Provides-Extra: nmmo
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `pufferlib-0.2.1/setup.py` & `pufferlib-0.3.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,43 +21,59 @@
     'box2d': [
         'swig==4.1.1', #unspecified box2d dep
         'gym[box2d]',
     ],
     'butterfly': [
         'pettingzoo[butterfly]',
     ],
+    'crafter': [
+        'crafter==1.8.0',
+    ],
+    'dm_control': [
+        'dm_control==1.0.11',
+        'gym_dmc==0.2.5',
+        'gym==0.21.0',
+    ],
+    'dm_lab': [
+        'gym_deepmindlab==0.1.2',
+    ],
     #'griddly': [
     #    'imageio==2.23.0',
     #    'griddly==1.4.2',
     #],
     'magent': [
         'magent==0.2.4',
     ],
     'microrts': [
         'ffmpeg==1.4',
         'gym_microrts==0.3.2',
     ],
+    'minerl': [
+        'gym==0.19.0',
+        'minerl==0.4.4',
+    ],
     'nethack': [
         'nle==0.9.0',
     ],
-    'nmmo': [
-        'nmmo==1.7.0.1',
-    ],
     #'smac': [
     #    'git+https://github.com/oxwhirl/smac.git',
     #],
 }
 
 rllib = [
     'ray[all]==2.0.0',
+    'setproctitle==1.1.10',
+    'service-identity==21.1.0',
 ]
 
 cleanrl = [
-    'ray==2.0.0',
     'tensorboard==2.11.2',
+    'torch',
+    'wandb==0.13.7',
+    'psutil==5.9.5',
 ]
 
 flat_tests = list(set(chain.from_iterable(tests.values())))
 
 extra_all = docs + flat_tests + rllib
 
 setup(
@@ -68,20 +84,21 @@
     version=open('pufferlib/version.py').read().split()[-1].strip("'"),
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'gym==0.23',
         'numpy==1.23.3',
         'opencv-python==3.4.17.63',
-        'openskill==2.4.0',
+        'openskill==4.0.0',
         'pettingzoo==1.19.0',
     ],
     extras_require={
         'docs': docs,
         'rllib': rllib,
+        'cleanrl': cleanrl,
         'tests': flat_tests,
         'all': extra_all,
         **tests,
     },
     python_requires=">=3.8",
     license="MIT",
     author="Joseph Suarez",
```

