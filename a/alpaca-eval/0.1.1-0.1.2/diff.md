# Comparing `tmp/alpaca_eval-0.1.1.tar.gz` & `tmp/alpaca_eval-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_eval-0.1.1.tar", last modified: Thu Jun  8 19:00:22 2023, max compression
+gzip compressed data, was "alpaca_eval-0.1.2.tar", last modified: Thu Jun  8 19:04:08 2023, max compression
```

## Comparing `alpaca_eval-0.1.1.tar` & `alpaca_eval-0.1.2.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.783014 alpaca_eval-0.1.1/
--rw-r--r--   0 xuechenli   (501) staff       (20)    11409 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/LICENSE
--rw-r--r--   0 xuechenli   (501) staff       (20)      187 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/MANIFEST.in
--rw-r--r--   0 xuechenli   (501) staff       (20)      778 2023-06-08 19:00:22.782878 alpaca_eval-0.1.1/PKG-INFO
--rw-r--r--   0 xuechenli   (501) staff       (20)    63472 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/README.md
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.762484 alpaca_eval-0.1.1/example/
--rw-r--r--   0 xuechenli   (501) staff       (20)   517613 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/example/outputs.json
--rw-r--r--   0 xuechenli   (501) staff       (20)       38 2023-06-08 19:00:22.783053 alpaca_eval-0.1.1/setup.cfg
--rw-r--r--   0 xuechenli   (501) staff       (20)     2113 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/setup.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.757113 alpaca_eval-0.1.1/src/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.765778 alpaca_eval-0.1.1/src/alpaca_eval/
--rw-r--r--   0 xuechenli   (501) staff       (20)       22 2023-06-08 18:59:20.000000 alpaca_eval-0.1.1/src/alpaca_eval/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    20821 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/analyze.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.767034 alpaca_eval-0.1.1/src/alpaca_eval/annotators/
--rw-r--r--   0 xuechenli   (501) staff       (20)       33 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/annotators/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    31305 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/annotators/pairwise_evaluator.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3939 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/completion_parsers.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     5218 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/constants.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.769363 alpaca_eval-0.1.1/src/alpaca_eval/decoders/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1913 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/decoders/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     4730 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/decoders/anthropic.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2835 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/decoders/cohere.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3905 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/decoders/huggingface_api.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     4697 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/decoders/huggingface_local.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    11804 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/decoders/openai.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.769591 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/
--rw-r--r--   0 xuechenli   (501) staff       (20)     9670 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/README.md
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.769986 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1204 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      270 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.772440 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1650 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5869 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     2475 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3721 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3423 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6849 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6797 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6700 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6045 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)     1016 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3969 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5932 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5370 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.772846 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)     7373 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      362 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.773191 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/aviary_gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1048 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      324 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.773529 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/chatgpt/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1116 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      325 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.773851 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/claude/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1137 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      317 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/claude/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.774192 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/claude_ranking/
--rw-r--r--   0 xuechenli   (501) staff       (20)      259 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)     1087 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.774365 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/cohere/
--rw-r--r--   0 xuechenli   (501) staff       (20)      303 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.774531 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)      314 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.774874 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/guanaco_33b/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1298 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      452 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.775044 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)      322 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.775216 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)      317 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.775543 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)      319 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)     1051 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.775884 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1054 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      367 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.776217 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/text_davinci_003/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1017 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      341 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.759016 alpaca_eval-0.1.1/src/alpaca_eval/leaderboards/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.776699 alpaca_eval-0.1.1/src/alpaca_eval/leaderboards/data_AlpacaEval/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1739 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
--rw-r--r--   0 xuechenli   (501) staff       (20)     1744 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
--rw-r--r--   0 xuechenli   (501) staff       (20)      351 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.776860 alpaca_eval-0.1.1/src/alpaca_eval/leaderboards/evaluators/
--rw-r--r--   0 xuechenli   (501) staff       (20)     2577 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
--rw-r--r--   0 xuechenli   (501) staff       (20)    21692 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/main.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1313 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/metrics.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.761096 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.777192 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/alpaca-7b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      382 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)      152 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.777351 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
--rw-r--r--   0 xuechenli   (501) staff       (20)      433 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.777501 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
--rw-r--r--   0 xuechenli   (501) staff       (20)      456 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.777659 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/chatgpt/
--rw-r--r--   0 xuechenli   (501) staff       (20)      196 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.778005 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/claude/
--rw-r--r--   0 xuechenli   (501) staff       (20)      184 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/claude/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)       34 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/claude/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.778216 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/cohere/
--rw-r--r--   0 xuechenli   (501) staff       (20)      188 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/cohere/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.778392 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/falcon-40b-instruct/
--rw-r--r--   0 xuechenli   (501) staff       (20)      405 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.778649 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/falcon-7b-instruct/
--rw-r--r--   0 xuechenli   (501) staff       (20)      401 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.779000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)      100 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      178 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.779173 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/guanaco-13b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      430 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.779321 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/guanaco-33b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      430 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.779479 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/guanaco-65b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      430 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.779768 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/guanaco-7b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      425 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)      195 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.780056 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/nous-hermes-13b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      407 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)      185 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.780202 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      449 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.780537 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      436 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)       42 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.780877 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      458 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)       51 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.781102 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
--rw-r--r--   0 xuechenli   (501) staff       (20)      438 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.781270 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/text_davinci_001/
--rw-r--r--   0 xuechenli   (501) staff       (20)      211 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.781632 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/text_davinci_003/
--rw-r--r--   0 xuechenli   (501) staff       (20)      211 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)       34 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.781982 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/vicuna-13b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      387 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)      185 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/vicuna-13b/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.782335 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/vicuna-7b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      383 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)      185 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.782663 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/wizardlm-13b/
--rw-r--r--   0 xuechenli   (501) staff       (20)      394 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)      185 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)    22484 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/plotting.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      283 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/types.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    15488 2023-06-08 18:58:52.000000 alpaca_eval-0.1.1/src/alpaca_eval/utils.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:00:22.766653 alpaca_eval-0.1.1/src/alpaca_eval.egg-info/
--rw-r--r--   0 xuechenli   (501) staff       (20)      778 2023-06-08 19:00:22.000000 alpaca_eval-0.1.1/src/alpaca_eval.egg-info/PKG-INFO
--rw-r--r--   0 xuechenli   (501) staff       (20)     5723 2023-06-08 19:00:22.000000 alpaca_eval-0.1.1/src/alpaca_eval.egg-info/SOURCES.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)        1 2023-06-08 19:00:22.000000 alpaca_eval-0.1.1/src/alpaca_eval.egg-info/dependency_links.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)       54 2023-06-08 19:00:22.000000 alpaca_eval-0.1.1/src/alpaca_eval.egg-info/entry_points.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      418 2023-06-08 19:00:22.000000 alpaca_eval-0.1.1/src/alpaca_eval.egg-info/requires.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)       12 2023-06-08 19:00:22.000000 alpaca_eval-0.1.1/src/alpaca_eval.egg-info/top_level.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.548826 alpaca_eval-0.1.2/
+-rw-r--r--   0 xuechenli   (501) staff       (20)    11409 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/LICENSE
+-rw-r--r--   0 xuechenli   (501) staff       (20)      187 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/MANIFEST.in
+-rw-r--r--   0 xuechenli   (501) staff       (20)    64291 2023-06-08 19:04:08.548657 alpaca_eval-0.1.2/PKG-INFO
+-rw-r--r--   0 xuechenli   (501) staff       (20)    63472 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/README.md
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.527830 alpaca_eval-0.1.2/example/
+-rw-r--r--   0 xuechenli   (501) staff       (20)   517613 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/example/outputs.json
+-rw-r--r--   0 xuechenli   (501) staff       (20)       38 2023-06-08 19:04:08.548866 alpaca_eval-0.1.2/setup.cfg
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2121 2023-06-08 19:03:04.000000 alpaca_eval-0.1.2/setup.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.522109 alpaca_eval-0.1.2/src/
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.530988 alpaca_eval-0.1.2/src/alpaca_eval/
+-rw-r--r--   0 xuechenli   (501) staff       (20)       22 2023-06-08 19:03:26.000000 alpaca_eval-0.1.2/src/alpaca_eval/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    20821 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/analyze.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.532604 alpaca_eval-0.1.2/src/alpaca_eval/annotators/
+-rw-r--r--   0 xuechenli   (501) staff       (20)       33 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/annotators/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    31305 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/annotators/pairwise_evaluator.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3939 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/completion_parsers.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5218 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/constants.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.533859 alpaca_eval-0.1.2/src/alpaca_eval/decoders/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1913 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/decoders/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4730 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/decoders/anthropic.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2835 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/decoders/cohere.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3905 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/decoders/huggingface_api.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4697 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/decoders/huggingface_local.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    11804 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/decoders/openai.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.534034 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     9670 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/README.md
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.534401 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1204 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      270 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.536911 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1650 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5869 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2475 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3721 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3423 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6849 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6797 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6700 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6045 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1016 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3969 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5932 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5370 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.537309 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7373 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      362 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.537736 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1048 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      324 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.538138 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/chatgpt/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1116 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      325 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.538520 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/claude/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1137 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      317 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/claude/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.538839 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/claude_ranking/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      259 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1087 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.538996 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/cohere/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      303 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.539162 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/gpt4/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      314 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.539585 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/guanaco_33b/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1298 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      452 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.539803 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      322 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.539973 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      317 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.540304 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      319 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1051 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.540749 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1054 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      367 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.541230 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/text_davinci_003/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1017 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      341 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.523858 alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.541764 alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/data_AlpacaEval/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1739 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1744 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
+-rw-r--r--   0 xuechenli   (501) staff       (20)      351 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.541930 alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/evaluators/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2577 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
+-rw-r--r--   0 xuechenli   (501) staff       (20)    21692 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/main.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1313 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/metrics.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.526550 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.542286 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/alpaca-7b/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      382 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)      152 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.542490 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      433 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.542737 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      456 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.542921 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/chatgpt/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      196 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.543229 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/claude/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      184 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/claude/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)       34 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/claude/prompt.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.543391 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/cohere/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      188 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/cohere/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.543556 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/falcon-40b-instruct/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      405 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.543748 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/falcon-7b-instruct/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      401 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.544107 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/gpt4/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      100 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      178 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/gpt4/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.544315 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-13b/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      430 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.544510 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-33b/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      430 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.544677 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-65b/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      430 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.545038 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-7b/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      425 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)      195 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.545350 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/nous-hermes-13b/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      407 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)      185 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.545498 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      449 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.545831 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      436 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)       42 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.546158 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      458 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)       51 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.546319 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      438 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.546505 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/text_davinci_001/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      211 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.546820 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/text_davinci_003/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      211 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)       34 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.547230 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/vicuna-13b/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      387 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)      185 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/vicuna-13b/prompt.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.547673 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/vicuna-7b/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      383 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)      185 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.548101 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/wizardlm-13b/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      394 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)      185 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)    22484 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/plotting.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      283 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/types.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    15488 2023-06-08 18:58:52.000000 alpaca_eval-0.1.2/src/alpaca_eval/utils.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-08 19:04:08.532243 alpaca_eval-0.1.2/src/alpaca_eval.egg-info/
+-rw-r--r--   0 xuechenli   (501) staff       (20)    64291 2023-06-08 19:04:08.000000 alpaca_eval-0.1.2/src/alpaca_eval.egg-info/PKG-INFO
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5723 2023-06-08 19:04:08.000000 alpaca_eval-0.1.2/src/alpaca_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)        1 2023-06-08 19:04:08.000000 alpaca_eval-0.1.2/src/alpaca_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)       54 2023-06-08 19:04:08.000000 alpaca_eval-0.1.2/src/alpaca_eval.egg-info/entry_points.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      418 2023-06-08 19:04:08.000000 alpaca_eval-0.1.2/src/alpaca_eval.egg-info/requires.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)       12 2023-06-08 19:04:08.000000 alpaca_eval-0.1.2/src/alpaca_eval.egg-info/top_level.txt
```

### Comparing `alpaca_eval-0.1.1/LICENSE` & `alpaca_eval-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/README.md` & `alpaca_eval-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/example/outputs.json` & `alpaca_eval-0.1.2/example/outputs.json`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/setup.py` & `alpaca_eval-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -55,10 +55,11 @@
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     entry_points={
         "console_scripts": [
             "alpaca_eval=alpaca_eval.main:main",
         ],
     },
-    # package_data={'alpaca_eval': ['evaluators_configs/*/*.*', 'models_configs/*/*.*', 'leaderboards/*/*.csv']},
-    include_package_data=True
+    include_package_data=True,
+    long_description=open("README.md", "r", encoding="utf-8").read(),
+    long_description_content_type="text/markdown",
 )
```

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/analyze.py` & `alpaca_eval-0.1.2/src/alpaca_eval/analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/annotators/pairwise_evaluator.py` & `alpaca_eval-0.1.2/src/alpaca_eval/annotators/pairwise_evaluator.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/completion_parsers.py` & `alpaca_eval-0.1.2/src/alpaca_eval/completion_parsers.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/constants.py` & `alpaca_eval-0.1.2/src/alpaca_eval/constants.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/decoders/__init__.py` & `alpaca_eval-0.1.2/src/alpaca_eval/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/decoders/anthropic.py` & `alpaca_eval-0.1.2/src/alpaca_eval/decoders/anthropic.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/decoders/cohere.py` & `alpaca_eval-0.1.2/src/alpaca_eval/decoders/cohere.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/decoders/huggingface_api.py` & `alpaca_eval-0.1.2/src/alpaca_eval/decoders/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/decoders/huggingface_local.py` & `alpaca_eval-0.1.2/src/alpaca_eval/decoders/huggingface_local.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/decoders/openai.py` & `alpaca_eval-0.1.2/src/alpaca_eval/decoders/openai.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/README.md` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt` & `alpaca_eval-0.1.2/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv` & `alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv` & `alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv` & `alpaca_eval-0.1.2/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/main.py` & `alpaca_eval-0.1.2/src/alpaca_eval/main.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/metrics.py` & `alpaca_eval-0.1.2/src/alpaca_eval/metrics.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/plotting.py` & `alpaca_eval-0.1.2/src/alpaca_eval/plotting.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval/utils.py` & `alpaca_eval-0.1.2/src/alpaca_eval/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.1/src/alpaca_eval.egg-info/SOURCES.txt` & `alpaca_eval-0.1.2/src/alpaca_eval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

