# Comparing `tmp/panml-0.0.25.tar.gz` & `tmp/panml-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-0.0.25.tar", last modified: Mon Jun  5 12:57:49 2023, max compression
+gzip compressed data, was "panml-1.0.0.tar", last modified: Thu Jun  8 13:10:00 2023, max compression
```

## Comparing `panml-0.0.25.tar` & `panml-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-05 12:57:49.205567 panml-0.0.25/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.25/LICENSE
--rw-r--r--   0 williamzheng   (501) staff       (20)    14677 2023-06-05 12:57:49.205810 panml-0.0.25/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)    13498 2023-06-05 12:56:17.000000 panml-0.0.25/README.md
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-05 12:57:49.197886 panml-0.0.25/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-0.0.25/panml/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     4497 2023-06-05 12:56:17.000000 panml-0.0.25/panml/constants.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-05 12:57:49.200363 panml-0.0.25/panml/core/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.25/panml/core/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-05 12:57:49.201298 panml-0.0.25/panml/core/clustering/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.25/panml/core/clustering/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-05-24 12:19:14.000000 panml-0.0.25/panml/core/clustering/faiss.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-05 12:57:49.203129 panml-0.0.25/panml/core/llm/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.25/panml/core/llm/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    23368 2023-06-05 12:56:17.000000 panml-0.0.25/panml/core/llm/huggingface.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    13741 2023-06-01 22:37:04.000000 panml-0.0.25/panml/core/llm/openai.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     3090 2023-06-05 12:56:17.000000 panml-0.0.25/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     2608 2023-05-28 12:46:27.000000 panml-0.0.25/panml/search.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-05 12:57:49.199873 panml-0.0.25/panml.egg-info/
--rw-r--r--   0 williamzheng   (501) staff       (20)    14677 2023-06-05 12:57:49.000000 panml-0.0.25/panml.egg-info/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)      468 2023-06-05 12:57:49.000000 panml-0.0.25/panml.egg-info/SOURCES.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-05 12:57:49.000000 panml-0.0.25/panml.egg-info/dependency_links.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)      227 2023-06-05 12:57:49.000000 panml-0.0.25/panml.egg-info/requires.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-05 12:57:49.000000 panml-0.0.25/panml.egg-info/top_level.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-05 12:57:49.206751 panml-0.0.25/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2407 2023-06-05 12:56:17.000000 panml-0.0.25/setup.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-05 12:57:49.204679 panml-0.0.25/test/
--rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-05-25 13:23:02.000000 panml-0.0.25/test/test_ModelPack.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-0.0.25/test/test_VectorEngine.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:10:00.564454 panml-1.0.0/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-1.0.0/LICENSE
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-08 13:10:00.564832 panml-1.0.0/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)    13498 2023-06-05 12:56:17.000000 panml-1.0.0/README.md
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:10:00.557697 panml-1.0.0/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-1.0.0/panml/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:10:00.560836 panml-1.0.0/panml/clustering/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.0/panml/clustering/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-06-08 13:09:32.000000 panml-1.0.0/panml/clustering/faiss.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     5841 2023-06-08 13:09:32.000000 panml-1.0.0/panml/constants.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1749 2023-06-08 13:09:32.000000 panml-1.0.0/panml/environments.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:10:00.562576 panml-1.0.0/panml/llm/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.0/panml/llm/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    23699 2023-06-08 13:09:32.000000 panml-1.0.0/panml/llm/huggingface.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    15676 2023-06-08 13:09:32.000000 panml-1.0.0/panml/llm/openai.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2739 2023-06-08 13:09:32.000000 panml-1.0.0/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2451 2023-06-08 13:09:32.000000 panml-1.0.0/panml/search.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:10:00.559790 panml-1.0.0/panml.egg-info/
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-08 13:10:00.000000 panml-1.0.0/panml.egg-info/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)      442 2023-06-08 13:10:00.000000 panml-1.0.0/panml.egg-info/SOURCES.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-08 13:10:00.000000 panml-1.0.0/panml.egg-info/dependency_links.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)      227 2023-06-08 13:10:00.000000 panml-1.0.0/panml.egg-info/requires.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-08 13:10:00.000000 panml-1.0.0/panml.egg-info/top_level.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-08 13:10:00.566014 panml-1.0.0/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2406 2023-06-08 13:09:32.000000 panml-1.0.0/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:10:00.563851 panml-1.0.0/test/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-06-07 05:36:34.000000 panml-1.0.0/test/test_ModelPack.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-1.0.0/test/test_VectorEngine.py
```

### Comparing `panml-0.0.25/LICENSE` & `panml-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `panml-0.0.25/PKG-INFO` & `panml-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 0.0.25
+Version: 1.0.0
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-0.0.25/README.md` & `panml-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `panml-0.0.25/panml/core/clustering/faiss.py` & `panml-1.0.0/panml/clustering/faiss.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.25/panml/core/llm/huggingface.py` & `panml-1.0.0/panml/llm/huggingface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 from __future__ import annotations
 import pandas as pd
 import torch
-from typing import Union, Callable
 from transformers import AutoModelForCausalLM, AutoModelForSeq2SeqLM, AutoModelForMaskedLM, AutoTokenizer
 from transformers import TrainingArguments, Trainer, Seq2SeqTrainingArguments, Seq2SeqTrainer, DataCollatorForLanguageModeling, DataCollatorForSeq2Seq
 from datasets import Dataset
 from peft import get_peft_model, PeftModel, PeftConfig, LoraConfig, TaskType
-from panml.constants import SUPPORTED_LLMS_PEFT_LORA
+from typing import Union, Callable
+from panml.constants import SUPPORTED_LLMS_PEFT_LORA, TOKENIZER_DEFAULT_ARGS, TRAINER_ARGS, PEFT_LORA_DEFAULT_ARGS
 
 # HuggingFace model class
 class HuggingFaceModelPack:
     '''
     HuggingFace Hub model pack class
     '''
     # Initialize class variables
-    def __init__(self, model: str, input_block_size: int, padding_length: int, tokenizer_batch: bool, source: str, model_args: dict) -> None:
-        self.model_name = model
-        self.padding_length = padding_length
-        self.input_block_size = input_block_size
-        self.tokenizer_batch = tokenizer_batch
-        self.prediction_history = []
-        self.evaluation_result = None
-        self.device = 'cpu'
-        self.supported_models_peft_lora = SUPPORTED_LLMS_PEFT_LORA
-        self.peft_config = None
-        self.train_default_args = ['title', 'num_train_epochs', 'optimizer', 'mlm', 
-                                   'per_device_train_batch_size', 'per_device_eval_batch_size',
-                                   'warmup_steps', 'weight_decay', 'logging_steps', 
-                                   'output_dir', 'logging_dir', 'save_model']
+    def __init__(self, model: str, source: str, model_args: dict) -> None:
+        self.model_name = model # model name
+        self.trainer_args = TRAINER_ARGS # model trainer arguments
+        self.supported_models_peft_lora = SUPPORTED_LLMS_PEFT_LORA # supported LLMs for LoRA implementation
+        self.peft_config = None # PEFT LoRA configuration
+        self.device = 'cpu' # model training and inference hardware setting
+        self.evaluation_result = None # model training evaluation result
+        self.prediction_history = [] # model inference history in prompt loop
+        
+        # Get tokenizer arguments
+        tokenzier_args = {k: model_args.pop(k) for k in list(TOKENIZER_DEFAULT_ARGS.keys()) if k in model_args}
+        for k in TOKENIZER_DEFAULT_ARGS:
+            tokenzier_args.setdefault(k, TOKENIZER_DEFAULT_ARGS[k])
+        self.padding_length = tokenzier_args['padding_length']
+        self.input_block_size = tokenzier_args['input_block_size']
+        self.tokenizer_batch = tokenzier_args['tokenizer_batch']
         
         # Get PEFT LoRA configuration from model args
-        peft_lora_args, load_peft_lora = {}, None
+        peft_lora_args, load_peft_lora = {}, False
         if 'peft_lora' in model_args:
             peft_lora_args = model_args.pop('peft_lora')
             if 'load' in peft_lora_args:
                 load_peft_lora = peft_lora_args.pop('load')
             else:
                 if not isinstance(load_peft_lora, bool):
                     raise TypeError('Input model args, peft_lora, load needs to be of type: boolean')
-                
             if 'task_type' in peft_lora_args:
                 _ = peft_lora_args.pop('task_type') # remove task_type from input args to avoid duplication
 
+            for k in PEFT_LORA_DEFAULT_ARGS:
+                peft_lora_args.setdefault(k, PEFT_LORA_DEFAULT_ARGS[k]) # set default arguments for LoRA
+
         # Get CPU/GPU configuration from model args
         set_gpu = False
         if 'gpu' in model_args:
             if not isinstance(model_args['gpu'], bool):
                 raise TypeError('Input model args, gpu needs to be of type: boolean')
             set_gpu = model_args.pop('gpu')
             if set_gpu: # set model processing on GPU else defaults on CPU
@@ -97,27 +101,27 @@
             # Set non-LoRA trained model's tokenizer
             if self.model_hf.config.tokenizer_class:
                 self.tokenizer = AutoTokenizer.from_pretrained(self.model_hf.config.tokenizer_class.lower().replace('tokenizer', ''), mirror='https://huggingface.co')
             else:
                 self.tokenizer = AutoTokenizer.from_pretrained(self.model_name, mirror='https://huggingface.co')
 
         # Set LoRA for training
-        if peft_lora_args is not {} and load_peft_lora is False:
+        if len(peft_lora_args) > 0 and load_peft_lora is False:
             if self.model_name in self.supported_models_peft_lora:
                 if 'flan' in self.model_name:
                     self.peft_config = LoraConfig(task_type=TaskType['SEQ_2_SEQ_LM'], **peft_lora_args)
                 else:
                     self.peft_config = LoraConfig(task_type=TaskType['CAUSAL_LM'], **peft_lora_args)
                 
                 self.model_hf = get_peft_model(self.model_hf, self.peft_config)
                 
-                print('PEFT LoRA configuration applied:')
+                print('PEFT LoRA configuration is applied:')
                 self.model_hf.print_trainable_parameters()
             else:
-                print('PEFT LoRA configuration not set. Current supported models for LoRA are: ' + ' '.join([f"{m}" for m in self.supported_models_peft_lora]))
+                print('PEFT LoRA configuration is not set. Current supported models for LoRA are: ' + ' '.join([f"{m}" for m in self.supported_models_peft_lora]))
 
         # Set model on GPU if available and specified
         self.model_hf.to(torch.device(self.device))
         
     # Set initial prompt
     def _init_prompt(self) -> list[dict[str, Union[str, Callable]]]:
         return [{'prepend': '', 'append': '', 'transform': None}]
@@ -218,15 +222,14 @@
         top_p: parameter from HuggingFace Hub, if set to float < 1, only the smallest set of most probable tokens with probabilities that add up to top_p or higher are kept for generation
         no_repeat_ngram_size: parameter from HuggingFace Hub, ff set to int > 0, all ngrams of that size can only occur once
 
         Returns: 
         prediction: list, or list of dict containing generated text with probabilities and perplexity if specified and available
         '''
         input_context = None
-        self.prediction_history = []
 
         # Catch input exceptions
         if not isinstance(text, str) and not isinstance(text, list) and not isinstance(text, pd.Series):
             raise TypeError('Input text needs to be of type: string, list or pandas.series')
         if isinstance(text, pd.Series): # convert to list from pandas series if available
             input_context = text.tolist()
             if len(input_context) == 0:
@@ -349,16 +352,16 @@
                 raise ValueError('Input num proc cannot be less than 1')
             
         # Convert to tokens format from pandas dataframes
         tokenized_data = self.tokenize_text(x, batched=self.tokenizer_batch, num_proc=num_proc)
         tokenized_target = self.tokenize_text(y, batched=self.tokenizer_batch, num_proc=num_proc)
         
         # Check for missing input arguments
-        if set(list(train_args.keys())) != set(self.train_default_args):
-            raise ValueError(f'Train args are not in the required format - missing: {", ".join(list(set(self.train_default_args) - set(list(train_args.keys()))))}')
+        if set(list(train_args.keys())) != set(self.trainer_args):
+            raise ValueError(f'Train args are not in the required format - missing: {", ".join(list(set(self.trainer_args) - set(list(train_args.keys()))))}')
         
         if instruct:
             print('Setting up training in sequence to sequence format...')
             tokenized_data = tokenized_data.add_column('labels', tokenized_target['input_ids']) # Create target sequence labels
             data_collator = DataCollatorForSeq2Seq(tokenizer=self.tokenizer) # Organise data for training
             
             # Setup training in sequence to sequence format
```

### Comparing `panml-0.0.25/panml/core/llm/openai.py` & `panml-1.0.0/panml/llm/openai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from __future__ import annotations
 import pandas as pd
+import openai
 import torch
 from typing import Union, Callable
-import openai
-from panml.constants import SUPPORTED_OAI_CODE_MODELS, SUPPORTED_OAI_COMPLETION_MODELS, SUPPORTED_OAI_CHAT_MODELS
+from panml.constants import SUPPORTED_OAI_CODE_MODELS, SUPPORTED_OAI_COMPLETION_MODELS, SUPPORTED_OAI_CHAT_MODELS, SUPPORTED_EMBEDDING_MODELS
 
 # OpenAI model class
 class OpenAIModelPack:
     '''
     OpenAI model pack class
     '''
     def __init__(self, model: str, api_key: str) -> None:
-        self.model_name = model
-        self.model_embedding = 'text-embedding-ada-002'
-        self.prediction_history = None
-        self.supported_code_models = SUPPORTED_OAI_CODE_MODELS
-        self.completion_models = SUPPORTED_OAI_COMPLETION_MODELS
-        self.chat_completion_models = SUPPORTED_OAI_CHAT_MODELS
-        openai.api_key = api_key
+        self.model_name = model # model name
+        self.model_embedding = SUPPORTED_EMBEDDING_MODELS['openai'] # model embedding name
+        self.supported_code_models = SUPPORTED_OAI_CODE_MODELS # supported code models
+        self.completion_models = SUPPORTED_OAI_COMPLETION_MODELS # supported completion models
+        self.chat_completion_models = SUPPORTED_OAI_CHAT_MODELS # supported chat models
+        openai.api_key = api_key # set api key
+        self.prediction_history = [] # model inference history in prompt loop
         
     def _init_prompt(self) -> list[dict[str, Union[str, Callable]]]:
         return [{'prepend': '', 'append': '', 'transform': None}]
     
     # Generate text of single model call
     def _predict(self, text: str, temperature: float, max_tokens: int, top_p: float, n: int, 
                  frequency_penalty: float, presence_penalty: float, display_probability: bool, logprobs: int, 
-                 chat_role: str) -> dict[str, str]:
+                 chat_role: str, stream: bool) -> dict[str, str]:
         '''
         Base function for text generation using OpenAI models
 
         Args:
         See predict function args
         
         Returns: 
@@ -49,31 +49,43 @@
                 prompt=text,
                 temperature=temperature,
                 max_tokens=max_tokens,
                 top_p=top_p,
                 n=n,
                 frequency_penalty=frequency_penalty,
                 presence_penalty=presence_penalty,
-                logprobs=logprobs
+                logprobs=logprobs,
+                stream=stream,
             )
+            
+            # Return response stream
+            if stream:
+                return response
+            
             output_context['text'] = response['choices'][0]['text']
             
         elif self.model_name in self.chat_completion_models:
             response = openai.ChatCompletion.create(
                 model=self.model_name,
                 messages = [
                     {'role': chat_role, 'content': text}
                 ],
                 temperature=temperature,
                 max_tokens=max_tokens,
                 top_p=top_p,
                 n=n,
                 frequency_penalty=frequency_penalty,
                 presence_penalty=presence_penalty,
+                stream=stream
             )
+
+            # Return response stream
+            if stream:
+                return response
+            
             output_context['text'] = response['choices'][0]['message']['content']
         else:
             raise ValueError(f'{self.model_name} is not currently supported in this package')
 
         # Get probability of output tokens
         if display_probability and self.model_name in self.completion_models:
             tokens = response["choices"][0]['logprobs']['tokens']
@@ -85,15 +97,15 @@
 
         return output_context
     
     # Generate text in prompt loop
     def predict(self, text: Union[str, list[str], pd.Series], temperature: float=0, max_length: int=100, top_p: float=1, n: int=3, 
                 frequency_penalty: float=0, presence_penalty: float=0, display_probability: bool=False, logprobs: int=1, 
                 prompt_modifier: list[dict[str, str]]=None, keep_history: bool=False, 
-                chat_role: str='user') -> Union[dict[str, str], list[str]]:
+                chat_role: str='user', stream: bool=False) -> Union[dict[str, str], list[str]]:
         '''
         Generates output by prompting a language model from OpenAI
         
         Args:
         text: text of the prompt, can be a string, list, or pandas.series
         temperature: temperature of the generated text (for further details please refer to this topic covered in language model text generation)
         max_length: max number of tokens to be generated from OpenAI API
@@ -102,14 +114,15 @@
         frequency_penalty: parameter from OpenAI API (for further details please refer to this topic covered in language model text generation)
         presence_penalty: parameter from OpenAI API (for further details please refer to this topic covered in language model text generation)
         display_probability: show probability of the generated tokens
         logprobs: parameter from OpenAI API (for further details please refer to this topic covered in language model text generation)
         prompt_modifier: list of prompts to be added in the context of multi-stage prompt chaining
         keep_history: keep or discard the history of responses from the mulit-stage prompt chaining
         chat_role: parameter from OpenAI API, specifies the role of the LLM assistant. Currently this is available for models of gpt-3.5-turbo or above (for further details please refer to this topic covered in language model text generation)
+        stream: parameter from OpenAI API, specifies for streaming mode for text generation
 
         Returns: 
         prediction: list, or list of dict containing generated text with probabilities and perplexity if specified and available
         '''
         input_context = None
         self.prediction_history = []
 
@@ -131,14 +144,19 @@
         if prompt_modifier is None:
             prompt_modifier = self._init_prompt()
         else:
             if not isinstance(prompt_modifier, list):
                 raise TypeError('Input prompt modifier needs to be of type: list')
         if not isinstance(chat_role, str):
             raise TypeError('Input chat role needs to be of type: string')
+        if not isinstance(stream, bool):
+            raise TypeError('Input stream needs to be of type: boolean')
+        else:
+            if stream and not isinstance(text, str):
+                raise ValueError('Streaming is not available for inputs (e.g. list or pandas dataframe column) that are outside of the string input use-case')
             
         # Run prediction on text samples
         prediction = []
         for context in input_context:
             # Create loop for text prediction
             history = []
             for count, mod in enumerate(prompt_modifier):
@@ -154,37 +172,48 @@
                 if count > 0:
                     context = output_context['text']
                 if mod['transform'] is not None and callable(mod['transform']):
                     context = f"{mod['prepend']}\n{mod['transform'](context)}\n{mod['append']}"
                 else:
                     context = f"{mod['prepend']}\n{context}\n{mod['append']}"
 
-                # Call model for text generation
-                output_context = self._predict(context, temperature=temperature, max_tokens=max_length, top_p=top_p,
-                                               n=n, frequency_penalty=frequency_penalty, presence_penalty=presence_penalty,
-                                               display_probability=display_probability, logprobs=logprobs, chat_role=chat_role)
-
-                # Terminate loop for next prompt when context contains no meaningful words (less than 2)
-                output_context['text'] = output_context['text'].replace('\n', ' ').replace('\xa0', '').replace('  ', ' ')
-                output_context['text'] = output_context['text'].replace(',', ', ')
-                output_context['text'] = output_context['text'].replace('.', '. ')
-                output_context['text'] = output_context['text'].replace('  ', ' ')
-                if len(output_context['text'].replace(' ', '')) < 2:
-                    break
-
-                history.append(output_context)
-            
-            try:
-                if keep_history:
-                    prediction.append(history[-1]) # saves last prediction output
-                    self.prediction_history.append(history) # saves all historical prediction output
+                if stream and count == len(prompt_modifier) - 1 and isinstance(text, str):
+                    # Call model for text generation in streaming mode
+                    output_context = self._predict(context, temperature=temperature, max_tokens=max_length, top_p=top_p,
+                                                n=n, frequency_penalty=frequency_penalty, presence_penalty=presence_penalty,
+                                                display_probability=display_probability, logprobs=logprobs, chat_role=chat_role, 
+                                                stream=True)
+                    return output_context
                 else:
-                    prediction.append(history[-1])
-            except:
-                prediction.append({'text': None}) # if there is invalid response from the language model, return None
+                    if stream:
+                        print('Streaming is not applied. Streaming is only available for single prompt inputs.')
+                    # Call model for text generation
+                    output_context = self._predict(context, temperature=temperature, max_tokens=max_length, top_p=top_p,
+                                                n=n, frequency_penalty=frequency_penalty, presence_penalty=presence_penalty,
+                                                display_probability=display_probability, logprobs=logprobs, chat_role=chat_role, 
+                                                stream=False)
+
+                    # Terminate loop for next prompt when context contains no meaningful words (less than 2)
+                    output_context['text'] = output_context['text'].replace('\n', ' ').replace('\xa0', '').replace('  ', ' ')
+                    output_context['text'] = output_context['text'].replace(',', ', ')
+                    output_context['text'] = output_context['text'].replace('.', '. ')
+                    output_context['text'] = output_context['text'].replace('  ', ' ')
+                    if len(output_context['text'].replace(' ', '')) < 2:
+                        break
+
+                    history.append(output_context)
+            
+                    try:
+                        if keep_history:
+                            prediction.append(history[-1]) # saves last prediction output
+                            self.prediction_history.append(history) # saves all historical prediction output
+                        else:
+                            prediction.append(history[-1])
+                    except:
+                        prediction.append({'text': None}) # if there is invalid response from the language model, return None
 
         # Gather output
         if isinstance(text, str):
             return prediction[0] # return string text as result
         else:
             if display_probability:
                 return prediction # return list of output_context dict as result
```

### Comparing `panml-0.0.25/panml/models.py` & `panml-1.0.0/panml/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,50 @@
 from __future__ import annotations
 
-# Dependencies for data processing and general machine learning implementations
-import torch
-from typing import Union
-
 # Dependencies for specialised language model implementations
-from transformers import AutoTokenizer
-from panml.core.llm.huggingface import HuggingFaceModelPack
-from panml.core.llm.openai import OpenAIModelPack
+from panml.llm.huggingface import HuggingFaceModelPack
+from panml.llm.openai import OpenAIModelPack
 from panml.constants import SUPPORTED_LLMS, SUPPORTED_LLM_SOURCES
+from panml.environments import ImportEnvironment
 
 # Entry model pack class           
 class ModelPack:
     '''
     Main model pack class
     '''
-    def __init__(self, model: str, tokenizer: AutoTokenizer=None, input_block_size: int=20, padding_length: int=100, 
-                 tokenizer_batch: bool=False, source: str='huggingface', api_key: str=None, model_args: dict={}) -> None:
-        self.padding_length = padding_length
-        self.tokenizer = tokenizer
+    def __init__(self, model: str, source: str='huggingface', model_args: dict={}, api_key: str=None) -> None:
         self.model = model
-        self.input_block_size = input_block_size
-        self.tokenizer_batch = tokenizer_batch
         self.source = source
         self.api_key = api_key
         self.model_args = model_args
         self.supported_models = SUPPORTED_LLMS # supported models
         self.supported_sources = SUPPORTED_LLM_SOURCES # supported source descriptions
         
         # General exceptions handling on user input
         if self.source not in self.supported_sources:
             raise ValueError('The specified source is not recognized. Supported sources are: ' + ' '.join([f"{s}" for s in self.supported_sources]))
 
-        # HuggingFace Hub model call
+        # HuggingFace Hub model processing
         if self.source == 'huggingface':
+            ImportEnvironment(['transformers', 'datasets', 'peft', 'pandas', 'torch']).validate() # Validate required packages
             if self.model not in self.supported_models['huggingface']:
                 raise ValueError('The specified model is currently not supported in this package. Supported HuggingFace Hub models are: ' + ' '.join([f"{m}" for m in self.supported_models['huggingface']]))
-            self.instance = HuggingFaceModelPack(self.model, self.input_block_size, self.padding_length, self.tokenizer_batch, self.source, self.model_args)
+            self.instance = HuggingFaceModelPack(self.model, self.source, self.model_args)
 
-        # Locally trained model call of HuggingFace Hub model
+        # Locally trained HuggingFace Hub model processing
         elif self.source == 'local':
-            self.instance = HuggingFaceModelPack(self.model, self.input_block_size, self.padding_length, self.tokenizer_batch, self.source, self.model_args)
+            ImportEnvironment(['transformers', 'datasets', 'peft', 'pandas', 'torch']).validate()
+            self.instance = HuggingFaceModelPack(self.model, self.source, self.model_args)
 
-        # OpenAI model call
+        # OpenAI model processing
         elif self.source == 'openai':
+            ImportEnvironment(['openai', 'pandas', 'torch']).validate()
             if self.model not in self.supported_models['openai']:
                 raise ValueError('The specified model currently is not supported in this package. Supported OpenAI models are: ' + ' '.join([f"{m}" for m in self.supported_models['openai']]))
             if self.api_key is None:
                 raise ValueError('api key has not been specified for OpenAI model call')
             self.instance = OpenAIModelPack(model=self.model, api_key=self.api_key)
 
     # Direct to the attribute ofthe sub model pack class (attribute not found in the main model pack class)
     def __getattr__(self, name):
         return self.instance.__getattribute__(name)
     
-# Set device type
-def set_device() -> str:
-    return 'cuda' if torch.cuda.is_available() else 'cpu'
```

### Comparing `panml-0.0.25/panml/search.py` & `panml-1.0.0/panml/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from __future__ import annotations
 
-# Dependencies for data processing and general machine learning implementations
-import torch
-import torch.nn.functional as F
-from typing import Union
-
 # Dependencies for vector search
-from panml.core.clustering.faiss import FAISSVectorEngine
+from panml.clustering.faiss import FAISSVectorEngine
 from panml.constants import SUPPORTED_VECTOR_SEARCH_SOURCES, SUPPORTED_EMBEDDING_MODELS
+from panml.environments import ImportEnvironment
 
 # Entry vector engine class           
 class VectorEngine:
     '''
     Main vector engine class
     '''
     def __init__(self, model: str='all-MiniLM-L6-v2', source: str='faiss', api_key: str=None) -> None:
@@ -29,22 +25,19 @@
             self.model not in self.supported_embedding_models['openai']:
             raise ValueError('The specified embedding model is currently not supported in this package. Supported embedding models for vector search are: ' + '\n' + str(self.supported_embedding_models))
         
         self.model_emb_source = [model_source for model_source, embedding_models in self.supported_embedding_models.items() if self.model in embedding_models][0]
         
         # FAISS vector search call
         if self.source == 'faiss':
+            ImportEnvironment(['faiss-cpu', 'sentence-transformers', 'openai', 'numpy', 'pandas']).validate() # Validate required packages
             self.instance = FAISSVectorEngine(self.model, self.model_emb_source, self.api_key)
             
         # Pinecone vector search call
         if self.source == 'pinecone':
             # TODO add Pinecone vecter search integration implementation
             print('Pinecone vector search integration not yet implemented')
             pass
             
     # Direct to the attribute of the sub vector engine class (attribute not found in the main vector engine class)
     def __getattr__(self, name):
         return self.instance.__getattribute__(name)
-
-# Calculate cosine similarity of two matrices    
-def cosine_similarity(t1: torch.Tensor, t2: torch.Tensor) -> torch.Tensor:
-    return F.cosine_similarity(t1.view(1, -1), t2.view(1, -1))
```

### Comparing `panml-0.0.25/panml.egg-info/PKG-INFO` & `panml-1.0.0/panml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 0.0.25
+Version: 1.0.0
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-0.0.25/setup.py` & `panml-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
   name = 'panml', # package name     
   packages = find_packages(exclude=['test']), # package name
-  version = '0.0.25', # version
+  version = '1.0.0', # version
   license = 'MIT', # license
   description = 'PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.', # short description about the package
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'PanML team', # team name
   author_email = 'teampanml@gmail.com', # contact email
   url = 'https://github.com/Pan-ML/panml', # url link
```

### Comparing `panml-0.0.25/test/test_ModelPack.py` & `panml-1.0.0/test/test_ModelPack.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.25/test/test_VectorEngine.py` & `panml-1.0.0/test/test_VectorEngine.py`

 * *Files identical despite different names*

