# Comparing `tmp/turingpoint-0.1.1.tar.gz` & `tmp/turingpoint-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turingpoint-0.1.1.tar", last modified: Sat May 20 18:46:18 2023, max compression
+gzip compressed data, was "turingpoint-0.2.0.tar", last modified: Thu Jun  8 14:35:52 2023, max compression
```

## Comparing `turingpoint-0.1.1.tar` & `turingpoint-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-20 18:46:18.952157 turingpoint-0.1.1/
--rw-r--r--   0 oren      (1000) oren      (1000)     7023 2023-05-20 18:46:18.952157 turingpoint-0.1.1/PKG-INFO
--rw-r--r--   0 oren      (1000) oren      (1000)     6233 2023-02-25 19:46:15.000000 turingpoint-0.1.1/README.md
--rw-r--r--   0 oren      (1000) oren      (1000)      103 2023-01-21 13:37:50.000000 turingpoint-0.1.1/pyproject.toml
--rw-r--r--   0 oren      (1000) oren      (1000)     1185 2023-05-20 18:46:18.952157 turingpoint-0.1.1/setup.cfg
-drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-20 18:46:18.952157 turingpoint-0.1.1/turingpoint/
--rw-r--r--   0 oren      (1000) oren      (1000)      177 2023-05-20 16:03:17.000000 turingpoint-0.1.1/turingpoint/__init__.py
--rw-r--r--   0 oren      (1000) oren      (1000)     1458 2023-05-17 15:41:08.000000 turingpoint-0.1.1/turingpoint/assembly.py
--rw-r--r--   0 oren      (1000) oren      (1000)      476 2023-01-20 16:18:22.000000 turingpoint-0.1.1/turingpoint/definitions.py
--rw-r--r--   0 oren      (1000) oren      (1000)     1407 2023-05-17 15:41:47.000000 turingpoint-0.1.1/turingpoint/gymnasium_utils.py
--rw-r--r--   0 oren      (1000) oren      (1000)     2637 2023-05-20 18:01:34.000000 turingpoint-0.1.1/turingpoint/pz_utils.py
--rw-r--r--   0 oren      (1000) oren      (1000)      431 2023-05-20 16:04:30.000000 turingpoint-0.1.1/turingpoint/sb3_utils.py
--rw-r--r--   0 oren      (1000) oren      (1000)     1778 2023-02-10 15:09:28.000000 turingpoint-0.1.1/turingpoint/self_play.py
--rw-r--r--   0 oren      (1000) oren      (1000)     1058 2023-05-20 18:08:59.000000 turingpoint-0.1.1/turingpoint/utils.py
-drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-20 18:46:18.952157 turingpoint-0.1.1/turingpoint.egg-info/
--rw-r--r--   0 oren      (1000) oren      (1000)     7023 2023-05-20 18:46:18.000000 turingpoint-0.1.1/turingpoint.egg-info/PKG-INFO
--rw-r--r--   0 oren      (1000) oren      (1000)      439 2023-05-20 18:46:18.000000 turingpoint-0.1.1/turingpoint.egg-info/SOURCES.txt
--rw-r--r--   0 oren      (1000) oren      (1000)        1 2023-05-20 18:46:18.000000 turingpoint-0.1.1/turingpoint.egg-info/dependency_links.txt
--rw-r--r--   0 oren      (1000) oren      (1000)      146 2023-05-20 18:46:18.000000 turingpoint-0.1.1/turingpoint.egg-info/requires.txt
--rw-r--r--   0 oren      (1000) oren      (1000)       12 2023-05-20 18:46:18.000000 turingpoint-0.1.1/turingpoint.egg-info/top_level.txt
--rw-r--r--   0 oren      (1000) oren      (1000)        1 2023-01-21 13:51:35.000000 turingpoint-0.1.1/turingpoint.egg-info/zip-safe
+drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-06-08 14:35:52.174720 turingpoint-0.2.0/
+-rw-r--r--   0 oren      (1000) oren      (1000)     7393 2023-06-08 14:35:52.174720 turingpoint-0.2.0/PKG-INFO
+-rw-r--r--   0 oren      (1000) oren      (1000)     6603 2023-06-08 14:21:43.000000 turingpoint-0.2.0/README.md
+-rw-r--r--   0 oren      (1000) oren      (1000)      103 2023-01-21 13:37:50.000000 turingpoint-0.2.0/pyproject.toml
+-rw-r--r--   0 oren      (1000) oren      (1000)     1185 2023-06-08 14:35:52.174720 turingpoint-0.2.0/setup.cfg
+drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-06-08 14:35:52.174720 turingpoint-0.2.0/turingpoint/
+-rw-r--r--   0 oren      (1000) oren      (1000)      191 2023-06-08 07:12:57.000000 turingpoint-0.2.0/turingpoint/__init__.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1508 2023-06-08 12:02:25.000000 turingpoint-0.2.0/turingpoint/assembly.py
+-rw-r--r--   0 oren      (1000) oren      (1000)      571 2023-06-08 07:12:27.000000 turingpoint-0.2.0/turingpoint/definitions.py
+-rw-r--r--   0 oren      (1000) oren      (1000)      585 2023-06-08 14:04:10.000000 turingpoint-0.2.0/turingpoint/gymnasium_utils.py
+-rw-r--r--   0 oren      (1000) oren      (1000)      765 2023-06-08 14:03:24.000000 turingpoint-0.2.0/turingpoint/pz_utils.py
+-rw-r--r--   0 oren      (1000) oren      (1000)      262 2023-06-07 18:24:17.000000 turingpoint-0.2.0/turingpoint/sb3_utils.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1778 2023-02-10 15:09:28.000000 turingpoint-0.2.0/turingpoint/self_play.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1058 2023-05-20 18:08:59.000000 turingpoint-0.2.0/turingpoint/utils.py
+drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-06-08 14:35:52.174720 turingpoint-0.2.0/turingpoint.egg-info/
+-rw-r--r--   0 oren      (1000) oren      (1000)     7393 2023-06-08 14:35:52.000000 turingpoint-0.2.0/turingpoint.egg-info/PKG-INFO
+-rw-r--r--   0 oren      (1000) oren      (1000)      439 2023-06-08 14:35:52.000000 turingpoint-0.2.0/turingpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)        1 2023-06-08 14:35:52.000000 turingpoint-0.2.0/turingpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)      146 2023-06-08 14:35:52.000000 turingpoint-0.2.0/turingpoint.egg-info/requires.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)       12 2023-06-08 14:35:52.000000 turingpoint-0.2.0/turingpoint.egg-info/top_level.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)        1 2023-01-21 13:51:35.000000 turingpoint-0.2.0/turingpoint.egg-info/zip-safe
```

### Comparing `turingpoint-0.1.1/PKG-INFO` & `turingpoint-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,10 @@
-Metadata-Version: 2.1
-Name: turingpoint
-Version: 0.1.1
-Summary: Reinforcement Learning (RL) library
-Home-page: https://github.com/zbenmo/turingpoint
-Author: Oren Zeev-Ben-Mordehai
-Author-email: zbenmo@gmail.com
-Keywords: Reinforcement Learning,Framework,Integration
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-Provides-Extra: examples
-
 # turingpoint
 
-Turing point is a Reinforcement Learning (RL) library. It adds the missing duck tape.
+Turing point is a Reinforcement Learning (RL) library. It adds the missing duct tape.
 It allows for multiple (hetrogenous) agents seamlessly. Per-agent partial observation is natural with Turing point.
 Different agents can act in differnet frequencies.
 You may opt to continue using also the environment and the agent libraries that you're currently using, for the such as Gym/Gymnasium, Stable-Baselines3, Tianshou, RLLib, etc.
 Turing point integrates easily with existing RL libraries and your own custom code.
 Integration of RL agents in the target applications should be significantly easier with Turing point.
 
 The main concept in Turing point is that there are multiple participants and each gets its turn.
@@ -59,15 +39,15 @@
 for i in range(1000):
     # The parameter for predict is the observation,
     #  which is good as our application (ex. an actual cartpole robot) can indeed provide such observations and use the return action.
     # Note: the action space as well as the observation space are defined in the environment.
     # Also note. The environment is aware of the agent. This is how the environment was designed.
     # The action space of the agent is coded in the environment.
     # The observation space is intended for the agent and reflects probably also what the agent should know about itself.
-    # The _state output is a bit suspicious. It is here probably as the model also predicts the state.
+    # The _state output is related to RNNs, AFAIK.
     action, _state = model.predict(obs, deterministic=True)
     # Here the reward, done, and info outputs are just for our evaluation.
     # Mainly what is happening here is that the environment moves to a new state.
     # The reward and done flag, are specific to the agent.
     # If there are other entities in the environments, those may continue to live also after done=True and may not care (directly) about this specific reward.
     obs, reward, done, info = vec_env.step(action)
     # We render here. We did not render during the training(learn) which probably makes sense performace wise.
@@ -81,99 +61,106 @@
 
 In the comments above, we've tried to give the intuition why some additional thinking is needed about
 the software that is used to provision those environment / agent(s) realms.
 
 Let's see how above can be described with Turing point:
 
 ```python
-import gym
+...
+import turingpoint.gymnasium_utils as tp_gym_utils
+import turingpoint.sb3_utils as tp_sb3_utils
+import turingpoint.utils as tp_utils
+import turingpoint as tp
 
-from stable_baselines3 import A2C
 
-from turingpoint.gym_utils import (
-  AgentParticipant,
-  EnvironmentParticipant,
-  RenderParticipant,
-  GymAssembly
-)
+def evaluate(env, agent, num_episodes: int) -> float:
 
+  rewards_collector = tp_utils.Collector(['reward'])
 
-# Creating the specific Gym environment.
-env = gym.make("CartPole-v1")
+  def get_participants():
+    yield functools.partial(tp_gym_utils.call_reset, env=env)
+    yield from itertools.cycle([
+        functools.partial(tp_sb3_utils.call_predict, agent=agent, deterministic=True),
+        functools.partial(tp_gym_utils.call_step, env=env),
+        rewards_collector,
+        tp_gym_utils.check_done
+    ]) 
 
-# An agent is created, it is injected with the environment.
-# The agent probably makes a copy of the passed environment, wraps it etc.
-model = A2C("MlpPolicy", env, verbose=1)
+  evaluate_assembly = tp.Assembly(get_participants)
 
-# The agent is trained against its environment.
-# We can assume what is happening there (obs, action, reward, obs, ..), yet it is not explicit.
-model.learn(total_timesteps=10_000)
+  for _ in range(num_episodes):
+    _ = evaluate_assembly.launch()
+    # Note that we don't clear the rewards in 'rewards_collector', and so we continue to collect.
 
-# above starts the same
+  total_reward = sum(x['reward'] for x in rewards_collector.get_entries())
 
-# now ..
+  return total_reward / num_episodes
 
-vec_env = model.get_env()
-assembly = GymAssembly(vec_env, [
-    AgentParticipant(agent),
-    EnvironmentParticipant(vec_env),
-    RenderParticipant(vec_env)
-])
+..
 
-for i in range(1000):
-    assembly.launch()
-```
+def main():
 
-What did we gain and was it worth the extra coding? Let's add to the environment a second agent, wind, or maybe it is part of the augmented environment, does not really matter. Let's just add it.
+  random.seed(1)
+  np.random.seed(1)
+  torch.manual_seed(1)
 
-```python
-import gym
+  env = gym.make('CartPole-v1')
 
-from stable_baselines3 import A2C
+  env.reset(seed=1)
 
-from turingpoint.gym_utils import (
-  AgentParticipant,
-  EnvironmentParticipant,
-  RenderParticipant,
-  GymAssembly
-)
+  agent = PPO(MlpPolicy, env, verbose=0) # use verbose=1 for debugging
 
+  mean_reward_before_train = evaluate(env, agent, 100)
+  print("before training")
+  print(f'{mean_reward_before_train=}')
 
-# Creating the specific Gym environment.
-env = gym.make("CartPole-v1")
+..
+```
 
-# An agent is created, it is injected with the environment.
-# The agent probably makes a copy of the passed environment, wraps it etc.
-model = A2C("MlpPolicy", env, verbose=1)
+What did we gain and was it worth the extra coding? Let's add to the environment a second agent, wind, or maybe it is part of the augmented environment, does not really matter. Let's just add it.
 
-# The agent is trained against its environment.
-# We can assume what is happening there (obs, action, reward, obs, ..), yet it is not explicit.
-model.learn(total_timesteps=10_000)
+```python
+..
 
 def wind(parcel: dict) -> None:
     action_wind = "blow left" if random() < 0.5 else "blow right"
     parcel['action_wind'] = action_wind
 
+
 def wind_impact(parcel: dict) -> None:
     action_wind = parcel['action_wind']
     # We'll modify the action of the agent, given the wind,
     # as we don't have here access to the state of the environment.
     parcel['action'] = ...
 
-vec_env = model.get_env()
-assembly = GymAssembly(vec_env, [
-    AgentParticipant(agent),
-    wind,
-    wind_impact,
-    EnvironmentParticipant(vec_env),
-    RenderParticipant(vec_env)
-])
 
-for i in range(1000):
-    assembly.launch()
+def evaluate(env, agent, num_episodes: int) -> float:
+
+  rewards_collector = tp_utils.Collector(['reward'])
+
+  def get_participants():
+    yield functools.partial(tp_gym_utils.call_reset, env=env)
+    yield from itertools.cycle([
+        functools.partial(tp_sb3_utils.call_predict, agent=agent, deterministic=True),
+        wind,
+        wind_impact,
+        functools.partial(tp_gym_utils.call_step, env=env),
+        rewards_collector,
+        tp_gym_utils.check_done
+    ]) 
+
+  evaluate_assembly = tp.Assembly(get_participants)
+
+  for _ in range(num_episodes):
+    _ = evaluate_assembly.launch()
+    # Note that we don't clear the rewards in 'rewards_collector', and so we continue to collect.
+
+  total_reward = sum(x['reward'] for x in rewards_collector.get_entries())
+
+  return total_reward / num_episodes
 ```
 
 To install use for example:
 
 ```
 pip install turingpoint
 ```
```

### Comparing `turingpoint-0.1.1/README.md` & `turingpoint-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,30 @@
+Metadata-Version: 2.1
+Name: turingpoint
+Version: 0.2.0
+Summary: Reinforcement Learning (RL) library
+Home-page: https://github.com/zbenmo/turingpoint
+Author: Oren Zeev-Ben-Mordehai
+Author-email: zbenmo@gmail.com
+Keywords: Reinforcement Learning,Framework,Integration
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+Provides-Extra: examples
+
 # turingpoint
 
-Turing point is a Reinforcement Learning (RL) library. It adds the missing duck tape.
+Turing point is a Reinforcement Learning (RL) library. It adds the missing duct tape.
 It allows for multiple (hetrogenous) agents seamlessly. Per-agent partial observation is natural with Turing point.
 Different agents can act in differnet frequencies.
 You may opt to continue using also the environment and the agent libraries that you're currently using, for the such as Gym/Gymnasium, Stable-Baselines3, Tianshou, RLLib, etc.
 Turing point integrates easily with existing RL libraries and your own custom code.
 Integration of RL agents in the target applications should be significantly easier with Turing point.
 
 The main concept in Turing point is that there are multiple participants and each gets its turn.
@@ -39,15 +59,15 @@
 for i in range(1000):
     # The parameter for predict is the observation,
     #  which is good as our application (ex. an actual cartpole robot) can indeed provide such observations and use the return action.
     # Note: the action space as well as the observation space are defined in the environment.
     # Also note. The environment is aware of the agent. This is how the environment was designed.
     # The action space of the agent is coded in the environment.
     # The observation space is intended for the agent and reflects probably also what the agent should know about itself.
-    # The _state output is a bit suspicious. It is here probably as the model also predicts the state.
+    # The _state output is related to RNNs, AFAIK.
     action, _state = model.predict(obs, deterministic=True)
     # Here the reward, done, and info outputs are just for our evaluation.
     # Mainly what is happening here is that the environment moves to a new state.
     # The reward and done flag, are specific to the agent.
     # If there are other entities in the environments, those may continue to live also after done=True and may not care (directly) about this specific reward.
     obs, reward, done, info = vec_env.step(action)
     # We render here. We did not render during the training(learn) which probably makes sense performace wise.
@@ -61,99 +81,106 @@
 
 In the comments above, we've tried to give the intuition why some additional thinking is needed about
 the software that is used to provision those environment / agent(s) realms.
 
 Let's see how above can be described with Turing point:
 
 ```python
-import gym
+...
+import turingpoint.gymnasium_utils as tp_gym_utils
+import turingpoint.sb3_utils as tp_sb3_utils
+import turingpoint.utils as tp_utils
+import turingpoint as tp
 
-from stable_baselines3 import A2C
 
-from turingpoint.gym_utils import (
-  AgentParticipant,
-  EnvironmentParticipant,
-  RenderParticipant,
-  GymAssembly
-)
+def evaluate(env, agent, num_episodes: int) -> float:
 
+  rewards_collector = tp_utils.Collector(['reward'])
 
-# Creating the specific Gym environment.
-env = gym.make("CartPole-v1")
+  def get_participants():
+    yield functools.partial(tp_gym_utils.call_reset, env=env)
+    yield from itertools.cycle([
+        functools.partial(tp_sb3_utils.call_predict, agent=agent, deterministic=True),
+        functools.partial(tp_gym_utils.call_step, env=env),
+        rewards_collector,
+        tp_gym_utils.check_done
+    ]) 
 
-# An agent is created, it is injected with the environment.
-# The agent probably makes a copy of the passed environment, wraps it etc.
-model = A2C("MlpPolicy", env, verbose=1)
+  evaluate_assembly = tp.Assembly(get_participants)
 
-# The agent is trained against its environment.
-# We can assume what is happening there (obs, action, reward, obs, ..), yet it is not explicit.
-model.learn(total_timesteps=10_000)
+  for _ in range(num_episodes):
+    _ = evaluate_assembly.launch()
+    # Note that we don't clear the rewards in 'rewards_collector', and so we continue to collect.
 
-# above starts the same
+  total_reward = sum(x['reward'] for x in rewards_collector.get_entries())
 
-# now ..
+  return total_reward / num_episodes
 
-vec_env = model.get_env()
-assembly = GymAssembly(vec_env, [
-    AgentParticipant(agent),
-    EnvironmentParticipant(vec_env),
-    RenderParticipant(vec_env)
-])
+..
 
-for i in range(1000):
-    assembly.launch()
-```
+def main():
 
-What did we gain and was it worth the extra coding? Let's add to the environment a second agent, wind, or maybe it is part of the augmented environment, does not really matter. Let's just add it.
+  random.seed(1)
+  np.random.seed(1)
+  torch.manual_seed(1)
 
-```python
-import gym
+  env = gym.make('CartPole-v1')
 
-from stable_baselines3 import A2C
+  env.reset(seed=1)
 
-from turingpoint.gym_utils import (
-  AgentParticipant,
-  EnvironmentParticipant,
-  RenderParticipant,
-  GymAssembly
-)
+  agent = PPO(MlpPolicy, env, verbose=0) # use verbose=1 for debugging
 
+  mean_reward_before_train = evaluate(env, agent, 100)
+  print("before training")
+  print(f'{mean_reward_before_train=}')
 
-# Creating the specific Gym environment.
-env = gym.make("CartPole-v1")
+..
+```
 
-# An agent is created, it is injected with the environment.
-# The agent probably makes a copy of the passed environment, wraps it etc.
-model = A2C("MlpPolicy", env, verbose=1)
+What did we gain and was it worth the extra coding? Let's add to the environment a second agent, wind, or maybe it is part of the augmented environment, does not really matter. Let's just add it.
 
-# The agent is trained against its environment.
-# We can assume what is happening there (obs, action, reward, obs, ..), yet it is not explicit.
-model.learn(total_timesteps=10_000)
+```python
+..
 
 def wind(parcel: dict) -> None:
     action_wind = "blow left" if random() < 0.5 else "blow right"
     parcel['action_wind'] = action_wind
 
+
 def wind_impact(parcel: dict) -> None:
     action_wind = parcel['action_wind']
     # We'll modify the action of the agent, given the wind,
     # as we don't have here access to the state of the environment.
     parcel['action'] = ...
 
-vec_env = model.get_env()
-assembly = GymAssembly(vec_env, [
-    AgentParticipant(agent),
-    wind,
-    wind_impact,
-    EnvironmentParticipant(vec_env),
-    RenderParticipant(vec_env)
-])
 
-for i in range(1000):
-    assembly.launch()
+def evaluate(env, agent, num_episodes: int) -> float:
+
+  rewards_collector = tp_utils.Collector(['reward'])
+
+  def get_participants():
+    yield functools.partial(tp_gym_utils.call_reset, env=env)
+    yield from itertools.cycle([
+        functools.partial(tp_sb3_utils.call_predict, agent=agent, deterministic=True),
+        wind,
+        wind_impact,
+        functools.partial(tp_gym_utils.call_step, env=env),
+        rewards_collector,
+        tp_gym_utils.check_done
+    ]) 
+
+  evaluate_assembly = tp.Assembly(get_participants)
+
+  for _ in range(num_episodes):
+    _ = evaluate_assembly.launch()
+    # Note that we don't clear the rewards in 'rewards_collector', and so we continue to collect.
+
+  total_reward = sum(x['reward'] for x in rewards_collector.get_entries())
+
+  return total_reward / num_episodes
 ```
 
 To install use for example:
 
 ```
 pip install turingpoint
 ```
```

### Comparing `turingpoint-0.1.1/setup.cfg` & `turingpoint-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `turingpoint-0.1.1/turingpoint/self_play.py` & `turingpoint-0.2.0/turingpoint/self_play.py`

 * *Files identical despite different names*

### Comparing `turingpoint-0.1.1/turingpoint/utils.py` & `turingpoint-0.2.0/turingpoint/utils.py`

 * *Files identical despite different names*

### Comparing `turingpoint-0.1.1/turingpoint.egg-info/PKG-INFO` & `turingpoint-0.2.0/turingpoint.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turingpoint
-Version: 0.1.1
+Version: 0.2.0
 Summary: Reinforcement Learning (RL) library
 Home-page: https://github.com/zbenmo/turingpoint
 Author: Oren Zeev-Ben-Mordehai
 Author-email: zbenmo@gmail.com
 Keywords: Reinforcement Learning,Framework,Integration
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -16,15 +16,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: examples
 
 # turingpoint
 
-Turing point is a Reinforcement Learning (RL) library. It adds the missing duck tape.
+Turing point is a Reinforcement Learning (RL) library. It adds the missing duct tape.
 It allows for multiple (hetrogenous) agents seamlessly. Per-agent partial observation is natural with Turing point.
 Different agents can act in differnet frequencies.
 You may opt to continue using also the environment and the agent libraries that you're currently using, for the such as Gym/Gymnasium, Stable-Baselines3, Tianshou, RLLib, etc.
 Turing point integrates easily with existing RL libraries and your own custom code.
 Integration of RL agents in the target applications should be significantly easier with Turing point.
 
 The main concept in Turing point is that there are multiple participants and each gets its turn.
@@ -59,15 +59,15 @@
 for i in range(1000):
     # The parameter for predict is the observation,
     #  which is good as our application (ex. an actual cartpole robot) can indeed provide such observations and use the return action.
     # Note: the action space as well as the observation space are defined in the environment.
     # Also note. The environment is aware of the agent. This is how the environment was designed.
     # The action space of the agent is coded in the environment.
     # The observation space is intended for the agent and reflects probably also what the agent should know about itself.
-    # The _state output is a bit suspicious. It is here probably as the model also predicts the state.
+    # The _state output is related to RNNs, AFAIK.
     action, _state = model.predict(obs, deterministic=True)
     # Here the reward, done, and info outputs are just for our evaluation.
     # Mainly what is happening here is that the environment moves to a new state.
     # The reward and done flag, are specific to the agent.
     # If there are other entities in the environments, those may continue to live also after done=True and may not care (directly) about this specific reward.
     obs, reward, done, info = vec_env.step(action)
     # We render here. We did not render during the training(learn) which probably makes sense performace wise.
@@ -81,99 +81,106 @@
 
 In the comments above, we've tried to give the intuition why some additional thinking is needed about
 the software that is used to provision those environment / agent(s) realms.
 
 Let's see how above can be described with Turing point:
 
 ```python
-import gym
+...
+import turingpoint.gymnasium_utils as tp_gym_utils
+import turingpoint.sb3_utils as tp_sb3_utils
+import turingpoint.utils as tp_utils
+import turingpoint as tp
 
-from stable_baselines3 import A2C
 
-from turingpoint.gym_utils import (
-  AgentParticipant,
-  EnvironmentParticipant,
-  RenderParticipant,
-  GymAssembly
-)
+def evaluate(env, agent, num_episodes: int) -> float:
 
+  rewards_collector = tp_utils.Collector(['reward'])
 
-# Creating the specific Gym environment.
-env = gym.make("CartPole-v1")
+  def get_participants():
+    yield functools.partial(tp_gym_utils.call_reset, env=env)
+    yield from itertools.cycle([
+        functools.partial(tp_sb3_utils.call_predict, agent=agent, deterministic=True),
+        functools.partial(tp_gym_utils.call_step, env=env),
+        rewards_collector,
+        tp_gym_utils.check_done
+    ]) 
 
-# An agent is created, it is injected with the environment.
-# The agent probably makes a copy of the passed environment, wraps it etc.
-model = A2C("MlpPolicy", env, verbose=1)
+  evaluate_assembly = tp.Assembly(get_participants)
 
-# The agent is trained against its environment.
-# We can assume what is happening there (obs, action, reward, obs, ..), yet it is not explicit.
-model.learn(total_timesteps=10_000)
+  for _ in range(num_episodes):
+    _ = evaluate_assembly.launch()
+    # Note that we don't clear the rewards in 'rewards_collector', and so we continue to collect.
 
-# above starts the same
+  total_reward = sum(x['reward'] for x in rewards_collector.get_entries())
 
-# now ..
+  return total_reward / num_episodes
 
-vec_env = model.get_env()
-assembly = GymAssembly(vec_env, [
-    AgentParticipant(agent),
-    EnvironmentParticipant(vec_env),
-    RenderParticipant(vec_env)
-])
+..
 
-for i in range(1000):
-    assembly.launch()
-```
+def main():
 
-What did we gain and was it worth the extra coding? Let's add to the environment a second agent, wind, or maybe it is part of the augmented environment, does not really matter. Let's just add it.
+  random.seed(1)
+  np.random.seed(1)
+  torch.manual_seed(1)
 
-```python
-import gym
+  env = gym.make('CartPole-v1')
 
-from stable_baselines3 import A2C
+  env.reset(seed=1)
 
-from turingpoint.gym_utils import (
-  AgentParticipant,
-  EnvironmentParticipant,
-  RenderParticipant,
-  GymAssembly
-)
+  agent = PPO(MlpPolicy, env, verbose=0) # use verbose=1 for debugging
 
+  mean_reward_before_train = evaluate(env, agent, 100)
+  print("before training")
+  print(f'{mean_reward_before_train=}')
 
-# Creating the specific Gym environment.
-env = gym.make("CartPole-v1")
+..
+```
 
-# An agent is created, it is injected with the environment.
-# The agent probably makes a copy of the passed environment, wraps it etc.
-model = A2C("MlpPolicy", env, verbose=1)
+What did we gain and was it worth the extra coding? Let's add to the environment a second agent, wind, or maybe it is part of the augmented environment, does not really matter. Let's just add it.
 
-# The agent is trained against its environment.
-# We can assume what is happening there (obs, action, reward, obs, ..), yet it is not explicit.
-model.learn(total_timesteps=10_000)
+```python
+..
 
 def wind(parcel: dict) -> None:
     action_wind = "blow left" if random() < 0.5 else "blow right"
     parcel['action_wind'] = action_wind
 
+
 def wind_impact(parcel: dict) -> None:
     action_wind = parcel['action_wind']
     # We'll modify the action of the agent, given the wind,
     # as we don't have here access to the state of the environment.
     parcel['action'] = ...
 
-vec_env = model.get_env()
-assembly = GymAssembly(vec_env, [
-    AgentParticipant(agent),
-    wind,
-    wind_impact,
-    EnvironmentParticipant(vec_env),
-    RenderParticipant(vec_env)
-])
 
-for i in range(1000):
-    assembly.launch()
+def evaluate(env, agent, num_episodes: int) -> float:
+
+  rewards_collector = tp_utils.Collector(['reward'])
+
+  def get_participants():
+    yield functools.partial(tp_gym_utils.call_reset, env=env)
+    yield from itertools.cycle([
+        functools.partial(tp_sb3_utils.call_predict, agent=agent, deterministic=True),
+        wind,
+        wind_impact,
+        functools.partial(tp_gym_utils.call_step, env=env),
+        rewards_collector,
+        tp_gym_utils.check_done
+    ]) 
+
+  evaluate_assembly = tp.Assembly(get_participants)
+
+  for _ in range(num_episodes):
+    _ = evaluate_assembly.launch()
+    # Note that we don't clear the rewards in 'rewards_collector', and so we continue to collect.
+
+  total_reward = sum(x['reward'] for x in rewards_collector.get_entries())
+
+  return total_reward / num_episodes
 ```
 
 To install use for example:
 
 ```
 pip install turingpoint
 ```
```

