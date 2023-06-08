# Comparing `tmp/huggingface_sb3-2.2.4.tar.gz` & `tmp/huggingface_sb3-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huggingface_sb3-2.2.4.tar", last modified: Thu Oct 13 17:10:25 2022, max compression
+gzip compressed data, was "huggingface_sb3-2.2.5.tar", last modified: Thu Jun  8 14:52:36 2023, max compression
```

## Comparing `huggingface_sb3-2.2.4.tar` & `huggingface_sb3-2.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:10:25.846493 huggingface_sb3-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (121)     5859 2022-10-13 17:10:25.846493 huggingface_sb3-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5382 2022-10-13 17:10:16.000000 huggingface_sb3-2.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:10:25.846493 huggingface_sb3-2.2.4/huggingface_sb3/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-10-13 17:10:16.000000 huggingface_sb3-2.2.4/huggingface_sb3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-10-13 17:10:16.000000 huggingface_sb3-2.2.4/huggingface_sb3/load_from_hub.py
--rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-10-13 17:10:16.000000 huggingface_sb3-2.2.4/huggingface_sb3/naming_schemes.py
--rw-r--r--   0 runner    (1001) docker     (121)    14150 2022-10-13 17:10:16.000000 huggingface_sb3-2.2.4/huggingface_sb3/push_to_hub.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:10:25.846493 huggingface_sb3-2.2.4/huggingface_sb3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5859 2022-10-13 17:10:25.000000 huggingface_sb3-2.2.4/huggingface_sb3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-10-13 17:10:25.000000 huggingface_sb3-2.2.4/huggingface_sb3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 17:10:25.000000 huggingface_sb3-2.2.4/huggingface_sb3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-10-13 17:10:25.000000 huggingface_sb3-2.2.4/huggingface_sb3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-13 17:10:25.000000 huggingface_sb3-2.2.4/huggingface_sb3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-10-13 17:10:25.850493 huggingface_sb3-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-10-13 17:10:16.000000 huggingface_sb3-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:52:36.742938 huggingface_sb3-2.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-08 14:52:36.742938 huggingface_sb3-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-08 14:52:30.000000 huggingface_sb3-2.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:52:36.738938 huggingface_sb3-2.2.5/huggingface_sb3/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-08 14:52:30.000000 huggingface_sb3-2.2.5/huggingface_sb3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-08 14:52:30.000000 huggingface_sb3-2.2.5/huggingface_sb3/load_from_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-08 14:52:30.000000 huggingface_sb3-2.2.5/huggingface_sb3/naming_schemes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-06-08 14:52:30.000000 huggingface_sb3-2.2.5/huggingface_sb3/push_to_hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:52:36.742938 huggingface_sb3-2.2.5/huggingface_sb3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-08 14:52:36.000000 huggingface_sb3-2.2.5/huggingface_sb3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-08 14:52:36.000000 huggingface_sb3-2.2.5/huggingface_sb3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:52:36.000000 huggingface_sb3-2.2.5/huggingface_sb3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-08 14:52:36.000000 huggingface_sb3-2.2.5/huggingface_sb3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 14:52:36.000000 huggingface_sb3-2.2.5/huggingface_sb3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-08 14:52:36.742938 huggingface_sb3-2.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-08 14:52:30.000000 huggingface_sb3-2.2.5/setup.py
```

### Comparing `huggingface_sb3-2.2.4/PKG-INFO` & `huggingface_sb3-2.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huggingface_sb3
-Version: 2.2.4
+Version: 2.2.5
 Summary: Additional code for Stable-baselines3 to load and upload models from the Hub.
 Home-page: https://github.com/huggingface/huggingface_sb3
 Author: Thomas Simonini, Omar Sanseviero and Hugging Face Team
 Author-email: thomas.simonini@huggingface.co
 License: Apache
 Keywords: reinforcement learning deep reinforcement learning RL
 Platform: UNKNOWN
@@ -16,17 +16,22 @@
 A library to load and upload Stable-baselines3 models from the Hub.
 
 ## Installation
 ### With pip
 ```
 pip install huggingface-sb3
 ```
+### IF YOU USE GYMNASIUM ENVIRONMENTS USE THIS INSTALL
+
+```
+pip install git+https://github.com/huggingface/huggingface_sb3@gymnasium
+```
 
 ## Examples
-We wrote a tutorial on how to use 🤗 Hub and Stable-Baselines3 [here](https://github.com/huggingface/huggingface_sb3/blob/main/notebooks/Stable_Baselines_3_and_Hugging_Face_%F0%9F%A4%97_tutorial.ipynb)
+We wrote a tutorial on how to use 🤗 Hub and Stable-Baselines3 [here](https://colab.research.google.com/github/huggingface/huggingface_sb3/blob/main/notebooks/sb3_huggingface.ipynb)
 
 If you use **Colab or a Virtual/Screenless Machine**, you can check Case 3 and Case 4.
 
 ### Case 1: I want to download a model from the Hub
 ```python
 import gym
 
@@ -179,7 +184,8 @@
 # This is where `model.save(model_name)` will place the model file
 print(model_name.filename)  
 
 # prints: `YourOrganization/ppo-seals-Walker2d-v0`
 print(repo_id)
 ```
 
+
```

### Comparing `huggingface_sb3-2.2.4/README.md` & `huggingface_sb3-2.2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 A library to load and upload Stable-baselines3 models from the Hub.
 
 ## Installation
 ### With pip
 ```
 pip install huggingface-sb3
 ```
+### IF YOU USE GYMNASIUM ENVIRONMENTS USE THIS INSTALL
+
+```
+pip install git+https://github.com/huggingface/huggingface_sb3@gymnasium
+```
 
 ## Examples
-We wrote a tutorial on how to use 🤗 Hub and Stable-Baselines3 [here](https://github.com/huggingface/huggingface_sb3/blob/main/notebooks/Stable_Baselines_3_and_Hugging_Face_%F0%9F%A4%97_tutorial.ipynb)
+We wrote a tutorial on how to use 🤗 Hub and Stable-Baselines3 [here](https://colab.research.google.com/github/huggingface/huggingface_sb3/blob/main/notebooks/sb3_huggingface.ipynb)
 
 If you use **Colab or a Virtual/Screenless Machine**, you can check Case 3 and Case 4.
 
 ### Case 1: I want to download a model from the Hub
 ```python
 import gym
 
@@ -164,8 +169,8 @@
 
 # prints: `ppo-seals-Walker2d-v0.zip`. 
 # This is where `model.save(model_name)` will place the model file
 print(model_name.filename)  
 
 # prints: `YourOrganization/ppo-seals-Walker2d-v0`
 print(repo_id)
-```
+```
```

### Comparing `huggingface_sb3-2.2.4/huggingface_sb3/load_from_hub.py` & `huggingface_sb3-2.2.5/huggingface_sb3/load_from_hub.py`

 * *Files identical despite different names*

### Comparing `huggingface_sb3-2.2.4/huggingface_sb3/naming_schemes.py` & `huggingface_sb3-2.2.5/huggingface_sb3/naming_schemes.py`

 * *Files identical despite different names*

### Comparing `huggingface_sb3-2.2.4/huggingface_sb3/push_to_hub.py` & `huggingface_sb3-2.2.5/huggingface_sb3/push_to_hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         )
 
         obs = env.reset()
         lstm_states = None
         episode_starts = np.ones((env.num_envs,), dtype=bool)
 
         try:
-            for _ in range(video_length + 1):
+            for _ in range(video_length):
                 action, lstm_states = model.predict(
                     obs,
                     state=lstm_states,
                     episode_start=episode_starts,
                     deterministic=is_deterministic,
                 )
                 obs, _, episode_starts, _ = env.step(action)
@@ -311,14 +311,16 @@
         (DQN, PPO, A2C, SAC...)
     :param env_id: name of the environment
     :param eval_env: environment used to evaluate the agent
     :param repo_id: id of the model repository from the Hugging Face Hub
     :param commit_message: commit message
     :param is_deterministic: use deterministic or stochastic actions (by default: True)
     :param n_eval_episodes: number of evaluation episodes (by default: 10)
+    :param token: authentication token (See https://huggingface.co/settings/token)
+        Caution: your token must remain secret. (See https://huggingface.co/docs/hub/security-tokens)
     :param video_length: length of the video (in timesteps)
     :param logs: directory on local machine of tensorboard logs you'd like to upload
     """
 
     # Autowrap, so we only have VecEnv afterward
     if not isinstance(eval_env, VecEnv):
         eval_env = DummyVecEnv([lambda: eval_env])
@@ -417,15 +419,16 @@
     token: Optional[str] = None,
 ):
     """
     Upload a model to Hugging Face Hub.
     :param repo_id: repo_id: id of the model repository from the Hugging Face Hub
     :param filename: name of the model zip or mp4 file from the repository
     :param commit_message: commit message
-    :param token
+    :param token: authentication token (See https://huggingface.co/settings/token)
+        Caution: your token must remain secret. (See https://huggingface.co/docs/hub/security-tokens)
     """
 
     repo_url = HfApi().create_repo(
         repo_id=repo_id,
         token=token,
         private=False,
         exist_ok=True,
```

### Comparing `huggingface_sb3-2.2.4/huggingface_sb3.egg-info/PKG-INFO` & `huggingface_sb3-2.2.5/huggingface_sb3.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huggingface-sb3
-Version: 2.2.4
+Version: 2.2.5
 Summary: Additional code for Stable-baselines3 to load and upload models from the Hub.
 Home-page: https://github.com/huggingface/huggingface_sb3
 Author: Thomas Simonini, Omar Sanseviero and Hugging Face Team
 Author-email: thomas.simonini@huggingface.co
 License: Apache
 Keywords: reinforcement learning deep reinforcement learning RL
 Platform: UNKNOWN
@@ -16,17 +16,22 @@
 A library to load and upload Stable-baselines3 models from the Hub.
 
 ## Installation
 ### With pip
 ```
 pip install huggingface-sb3
 ```
+### IF YOU USE GYMNASIUM ENVIRONMENTS USE THIS INSTALL
+
+```
+pip install git+https://github.com/huggingface/huggingface_sb3@gymnasium
+```
 
 ## Examples
-We wrote a tutorial on how to use 🤗 Hub and Stable-Baselines3 [here](https://github.com/huggingface/huggingface_sb3/blob/main/notebooks/Stable_Baselines_3_and_Hugging_Face_%F0%9F%A4%97_tutorial.ipynb)
+We wrote a tutorial on how to use 🤗 Hub and Stable-Baselines3 [here](https://colab.research.google.com/github/huggingface/huggingface_sb3/blob/main/notebooks/sb3_huggingface.ipynb)
 
 If you use **Colab or a Virtual/Screenless Machine**, you can check Case 3 and Case 4.
 
 ### Case 1: I want to download a model from the Hub
 ```python
 import gym
 
@@ -179,7 +184,8 @@
 # This is where `model.save(model_name)` will place the model file
 print(model_name.filename)  
 
 # prints: `YourOrganization/ppo-seals-Walker2d-v0`
 print(repo_id)
 ```
 
+
```

### Comparing `huggingface_sb3-2.2.4/setup.py` & `huggingface_sb3-2.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "black~=22.0",
     "isort>=5.5.4",
     "flake8>=3.8.3",
 ]
 
 setup(
     name='huggingface_sb3',
-    version='2.2.4',
+    version='2.2.5',
     packages=['huggingface_sb3'],
     url='https://github.com/huggingface/huggingface_sb3',
     license='Apache',
     author='Thomas Simonini, Omar Sanseviero and Hugging Face Team',
     author_email='thomas.simonini@huggingface.co',
     description='Additional code for Stable-baselines3 to load and upload models from the Hub.',
     install_requires=install_requires,
```

