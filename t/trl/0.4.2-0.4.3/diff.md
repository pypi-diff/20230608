# Comparing `tmp/trl-0.4.2-py3-none-any.whl.zip` & `tmp/trl-0.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,31 +1,31 @@
-Zip file size: 68392 bytes, number of entries: 29
+Zip file size: 68425 bytes, number of entries: 29
 -rw-r--r--  2.0 unx        0 b- defN 23-May-03 09:18 tests/__init__.py
 -rw-r--r--  2.0 unx     1561 b- defN 23-May-03 09:18 tests/test_core.py
 -rw-r--r--  2.0 unx      152 b- defN 23-Jun-07 09:41 tests/test_e2e.py
 -rw-r--r--  2.0 unx    23191 b- defN 23-May-03 09:18 tests/test_modeling_value_head.py
 -rw-r--r--  2.0 unx     5439 b- defN 23-May-03 09:18 tests/test_no_peft.py
 -rw-r--r--  2.0 unx     9515 b- defN 23-May-18 06:29 tests/test_peft_models.py
 -rw-r--r--  2.0 unx    35334 b- defN 23-Jun-06 11:48 tests/test_ppo_trainer.py
--rw-r--r--  2.0 unx     9931 b- defN 23-Jun-07 09:41 tests/test_reward_trainer.py
+-rw-r--r--  2.0 unx     9990 b- defN 23-Jun-07 10:25 tests/test_reward_trainer.py
 -rw-r--r--  2.0 unx    15722 b- defN 23-May-03 09:18 tests/test_sft_trainer.py
 -rw-r--r--  2.0 unx      799 b- defN 23-May-03 09:18 tests/testing_constants.py
 -rw-r--r--  2.0 unx     1555 b- defN 23-May-03 09:18 tests/testing_utils.py
--rw-r--r--  2.0 unx      339 b- defN 23-Jun-07 09:42 trl/__init__.py
+-rw-r--r--  2.0 unx      339 b- defN 23-Jun-08 08:50 trl/__init__.py
 -rw-r--r--  2.0 unx     7920 b- defN 23-May-03 09:18 trl/core.py
 -rw-r--r--  2.0 unx     1120 b- defN 23-May-03 09:18 trl/import_utils.py
 -rw-r--r--  2.0 unx      910 b- defN 23-May-03 09:18 trl/models/__init__.py
 -rw-r--r--  2.0 unx    19369 b- defN 23-Jun-06 12:02 trl/models/modeling_base.py
 -rw-r--r--  2.0 unx    17967 b- defN 23-May-17 09:28 trl/models/modeling_value_head.py
 -rw-r--r--  2.0 unx     1002 b- defN 23-May-03 09:18 trl/trainer/__init__.py
 -rw-r--r--  2.0 unx     1772 b- defN 23-May-03 09:18 trl/trainer/base.py
 -rw-r--r--  2.0 unx     6037 b- defN 23-May-03 09:18 trl/trainer/ppo_config.py
 -rw-r--r--  2.0 unx    51977 b- defN 23-Jun-07 09:41 trl/trainer/ppo_trainer.py
 -rw-r--r--  2.0 unx     9949 b- defN 23-Jun-07 09:41 trl/trainer/reward_trainer.py
--rw-r--r--  2.0 unx    13562 b- defN 23-Jun-06 12:02 trl/trainer/sft_trainer.py
+-rw-r--r--  2.0 unx    13562 b- defN 23-Jun-07 10:30 trl/trainer/sft_trainer.py
 -rw-r--r--  2.0 unx     9263 b- defN 23-Jun-06 11:48 trl/trainer/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-07 09:44 trl-0.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     7180 b- defN 23-Jun-07 09:44 trl-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 09:44 trl-0.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-07 09:44 trl-0.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2287 b- defN 23-Jun-07 09:44 trl-0.4.2.dist-info/RECORD
-29 files, 265312 bytes uncompressed, 64784 bytes compressed:  75.6%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-08 08:53 trl-0.4.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7190 b- defN 23-Jun-08 08:53 trl-0.4.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 08:53 trl-0.4.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-08 08:53 trl-0.4.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2287 b- defN 23-Jun-08 08:53 trl-0.4.3.dist-info/RECORD
+29 files, 265381 bytes uncompressed, 64817 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -66,23 +66,23 @@
 
 Filename: trl/trainer/sft_trainer.py
 Comment: 
 
 Filename: trl/trainer/utils.py
 Comment: 
 
-Filename: trl-0.4.2.dist-info/LICENSE
+Filename: trl-0.4.3.dist-info/LICENSE
 Comment: 
 
-Filename: trl-0.4.2.dist-info/METADATA
+Filename: trl-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: trl-0.4.2.dist-info/WHEEL
+Filename: trl-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: trl-0.4.2.dist-info/top_level.txt
+Filename: trl-0.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: trl-0.4.2.dist-info/RECORD
+Filename: trl-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tests/test_reward_trainer.py

```diff
@@ -20,14 +20,15 @@
 
 from trl import RewardTrainer
 from trl.trainer import compute_accuracy
 
 from .testing_utils import require_peft
 
 
+@unittest.skip("skip until the next transformers release")
 class RewardTrainerTester(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.model_id = "trl-internal-testing/dummy-GPT2-correct-vocab"
         cls.model = AutoModelForSequenceClassification.from_pretrained(cls.model_id)
         cls.tokenizer = AutoTokenizer.from_pretrained(cls.model_id)
         cls.tokenizer.pad_token = cls.tokenizer.eos_token
```

## trl/__init__.py

```diff
@@ -1,10 +1,10 @@
 # flake8: noqa
 
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 
 from .core import set_seed
 from .import_utils import is_peft_available
 from .models import (
     AutoModelForCausalLMWithValueHead,
     AutoModelForSeq2SeqLMWithValueHead,
     PreTrainedModelWrapper,
```

## Comparing `trl-0.4.2.dist-info/LICENSE` & `trl-0.4.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `trl-0.4.2.dist-info/METADATA` & `trl-0.4.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trl
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Pytorch implementation of Proximal Policy Optimization for transfomer language models.
 Home-page: https://github.com/lvwerra/trl
 Author: Leandro von Werra
 Author-email: leandro.vonwerra@gmail.com
 License: Apache 2.0
 Keywords: ppo,transformers,huggingface,gpt2,language modeling,rlhf
 Platform: UNKNOWN
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch (>=1.4.0)
 Requires-Dist: transformers (>=4.18.0)
 Requires-Dist: numpy (>=1.18.2)
-Requires-Dist: accelerate
+Requires-Dist: accelerate (<0.20.0)
 Requires-Dist: datasets
 Provides-Extra: dev
 Requires-Dist: parameterized ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: pytest-xdist ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
```

## Comparing `trl-0.4.2.dist-info/RECORD` & `trl-0.4.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_core.py,sha256=Jlr62saKWZBpdjGextXVhY1w7MFtTuL4P0pKa5rwyPI,1561
 tests/test_e2e.py,sha256=eUbrUuWkgM8KnMR1msSk-BNvovUk7JerdvjAsOh_KT0,152
 tests/test_modeling_value_head.py,sha256=5qFS28njLhV_fvg7InG22dcSi1IBC03p7T0tcH74Nv8,23191
 tests/test_no_peft.py,sha256=QYmX22qQHjdPUL-XgUfwJUJo_SQTp9poAKqoRolv6OM,5439
 tests/test_peft_models.py,sha256=AGeTQo00M5GEltJFrCSjHEfnWr4BIxgcTircSUwgjbo,9515
 tests/test_ppo_trainer.py,sha256=TKBgbpAhHuwz9CVg4fjxYO_PTvw0t2cHPz4zlj2IL68,35334
-tests/test_reward_trainer.py,sha256=WK9bglvoKHc6oDSoLToQ4HDaFwcjaBHE0l1H-aViX1s,9931
+tests/test_reward_trainer.py,sha256=9gfEbes7OC9d-ez2GX5ifT-FPzG3WVk8oYrfmh9mWAs,9990
 tests/test_sft_trainer.py,sha256=n_KIE9CYE5Gr8YIpmeFdpu7oRhEflxmDyYqVz6Lkrq8,15722
 tests/testing_constants.py,sha256=NjVJ5Q7LaQcEhbU2OIgK81fgR3H97Nuq3eW6aLPIisg,799
 tests/testing_utils.py,sha256=YyrL_F30bspcnSP2WdxkGGvA4O2laDs7oXmSc-Bo56Y,1555
-trl/__init__.py,sha256=0x3iYtaINsQ4hH54634ajAysUEB59hi9T3AcP0ocglg,339
+trl/__init__.py,sha256=veeJcbv6Iz87dVYH1ZNPGRhcZ9IIsKQjebwxkWfw_WQ,339
 trl/core.py,sha256=ImIMWwFmcht58G69kocy13O5ezevgbxcDe6g8mW9fzs,7920
 trl/import_utils.py,sha256=0dx0aONJfNEv0Le30Qw4qUXKT-dSkKXnnJTO6Wp6JGM,1120
 trl/models/__init__.py,sha256=9hseGjYJt9lhUib5e1k8vDWnQmJOIYa5zg0EUb3zUvI,910
 trl/models/modeling_base.py,sha256=FTzIup__dPjA5b2MjEfDLWkeG4dEbVd6ib6-tNMGES0,19369
 trl/models/modeling_value_head.py,sha256=Cn1U4L7Yh5Ljxs9-hqHOcSIVPqFjgwCXf-k7xlHfgmY,17967
 trl/trainer/__init__.py,sha256=aVC3ZpV_3cEq0Xx6QRNfU-2w8YEFfBuDt3uqafTQ_6o,1002
 trl/trainer/base.py,sha256=51YAcpsjJ8ghVbfhBXcP7BT0_yXnmhj0G_zfZhl3guE,1772
 trl/trainer/ppo_config.py,sha256=gUF8X563zBK53idvE0l1b0T1SMsYnKIxljKZ8lQ-Q3g,6037
 trl/trainer/ppo_trainer.py,sha256=6qCfquj6riT5P67R7uTSac7kmoPuX2nYLgYkoDFGQCM,51977
 trl/trainer/reward_trainer.py,sha256=ZE0tCoFbQpNR7jE4JTafzzpcRY_3zoyojFjDPVRgy60,9949
 trl/trainer/sft_trainer.py,sha256=_uhSY2RsTROgWa255VG9_fpF_1V6OXSroccfwwMXHVM,13562
 trl/trainer/utils.py,sha256=aHyTs4sq-wcB8xZgntqckQpPnCuzjYpaw6KOBkj-2A4,9263
-trl-0.4.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-trl-0.4.2.dist-info/METADATA,sha256=hNkFJAozaeXzXm-_jGEuiS0jW3weQ8pyCdwZWoyUjRM,7180
-trl-0.4.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-trl-0.4.2.dist-info/top_level.txt,sha256=TUKDSfcN6PgBU9dnJ6_YJ7qhDzZ0CKzHvHehR6GKpWg,10
-trl-0.4.2.dist-info/RECORD,,
+trl-0.4.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+trl-0.4.3.dist-info/METADATA,sha256=L8i4AhKRh5EZAs8eVpKUowiIkJUL8FpMMnW75MUECqY,7190
+trl-0.4.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+trl-0.4.3.dist-info/top_level.txt,sha256=TUKDSfcN6PgBU9dnJ6_YJ7qhDzZ0CKzHvHehR6GKpWg,10
+trl-0.4.3.dist-info/RECORD,,
```

