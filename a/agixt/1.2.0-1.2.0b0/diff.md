# Comparing `tmp/agixt-1.2.0.tar.gz` & `tmp/agixt-1.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.2.0.tar", max compression
+gzip compressed data, was "agixt-1.2.0b0.tar", max compression
```

## Comparing `agixt-1.2.0.tar` & `agixt-1.2.0b0.tar`

### file list

```diff
@@ -1,92 +1,93 @@
--rw-r--r--   0        0        0     1087 2023-06-07 20:13:22.746698 agixt-1.2.0/LICENSE
--rw-r--r--   0        0        0    19409 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/AGiXT.py
--rw-r--r--   0        0        0    23585 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/Agent.py
--rw-r--r--   0        0        0    10083 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/Chain.py
--rw-r--r--   0        0        0     1099 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/Config.py
--rw-r--r--   0        0        0     5900 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/Embedding.py
--rw-r--r--   0        0        0     6805 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/Extensions.py
--rw-r--r--   0        0        0     9489 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/Memories.py
--rw-r--r--   0        0        0     1986 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/Prompts.py
--rw-r--r--   0        0        0     7093 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/Tasks.py
--rw-r--r--   0        0        0       38 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/WORKSPACE/example.txt
--rw-r--r--   0        0        0      230 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/__init__.py
--rw-r--r--   0        0        0      244 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/agents/gpt4free/config.json
--rw-r--r--   0        0        0    17835 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/app.py
--rw-r--r--   0        0        0     2012 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/chains/Smart Chat.json
--rw-r--r--   0        0        0     7108 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/chains/Test_Commands.json
--rw-r--r--   0        0        0     1030 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/chains/Write a Poem.json
--rw-r--r--   0        0        0    11935 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/example.ipynb
--rw-r--r--   0        0        0     6213 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/agixt_agent.py
--rw-r--r--   0        0        0      860 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/briantts.py
--rw-r--r--   0        0        0     1174 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/dalle.py
--rw-r--r--   0        0        0     2818 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/discord.py
--rw-r--r--   0        0        0     1170 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/elevenlabs.py
--rw-r--r--   0        0        0     6647 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/file_system.py
--rw-r--r--   0        0        0     1841 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/github.py
--rw-r--r--   0        0        0     2042 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/google.py
--rw-r--r--   0        0        0      539 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/gtts.py
--rw-r--r--   0        0        0     2475 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/huggingface.py
--rw-r--r--   0        0        0      622 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/macostts.py
--rw-r--r--   0        0        0     4236 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/microsoft_365.py
--rw-r--r--   0        0        0     1899 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/searxng.py
--rw-r--r--   0        0        0     1001 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/sendgrid_email.py
--rw-r--r--   0        0        0      315 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/times.py
--rw-r--r--   0        0        0     1169 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/twitter.py
--rw-r--r--   0        0        0     2287 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/extensions/web_playwright.py
--rw-r--r--   0        0        0      151 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Chat.txt
--rw-r--r--   0        0        0      181 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0        0        0      991 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Create New Command.txt
--rw-r--r--   0        0        0     1017 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Execution.txt
--rw-r--r--   0        0        0     1178 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Instruction.txt
--rw-r--r--   0        0        0      378 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0        0        0      170 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Pick a Poem Subject.txt
--rw-r--r--   0        0        0      430 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0        0        0      326 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Prioritize.txt
--rw-r--r--   0        0        0      236 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0        0        0      270 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Score Response.txt
--rw-r--r--   0        0        0      349 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0        0        0      274 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0        0        0      304 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0        0        0      148 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0        0        0      474 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0        0        0      528 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0        0        0      458 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0        0        0      433 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0        0        0      160 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0        0        0      507 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0        0        0      560 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0        0        0      192 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0        0        0      162 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Tell Me How.txt
--rw-r--r--   0        0        0      162 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Title a Poem.txt
--rw-r--r--   0        0        0      308 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Validation.txt
--rw-r--r--   0        0        0      856 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0        0        0      314 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/WebSearch.txt
--rw-r--r--   0        0        0       28 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/Write a Poem.txt
--rw-r--r--   0        0        0     1178 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/gpt-3.5-turbo/instruct.txt
--rw-r--r--   0        0        0     1178 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0        0        0      777 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/instruct.txt
--rw-r--r--   0        0        0      824 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/starchat/instruct.txt
--rw-r--r--   0        0        0      616 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/prompts/vicuna/instruct.txt
--rw-r--r--   0        0        0     2329 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/__init__.py
--rw-r--r--   0        0        0     1729 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/azure.py
--rw-r--r--   0        0        0      493 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/bard.py
--rw-r--r--   0        0        0     1638 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/bing.py
--rw-r--r--   0        0        0      980 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/chatgpt.py
--rw-r--r--   0        0        0     1012 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/claude.py
--rw-r--r--   0        0        0      763 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/fastchat.py
--rw-r--r--   0        0        0      873 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/gpt4all.py
--rw-r--r--   0        0        0     5430 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/gpt4free.py
--rw-r--r--   0        0        0     1194 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/gpugpt4all.py
--rw-r--r--   0        0        0     1007 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/huggingchat.py
--rw-r--r--   0        0        0     1438 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/huggingface.py
--rw-r--r--   0        0        0     1091 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/kobold.py
--rw-r--r--   0        0        0     2048 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/llamacpp.py
--rw-r--r--   0        0        0     1071 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/llamacppapi.py
--rw-r--r--   0        0        0     1585 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/oobabooga.py
--rw-r--r--   0        0        0     1597 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/openai.py
--rw-r--r--   0        0        0      850 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/palm.py
--rw-r--r--   0        0        0     3730 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/runpod.py
--rw-r--r--   0        0        0     3106 2023-06-07 20:13:22.746698 agixt-1.2.0/agixt/provider/transformer.py
--rw-r--r--   0        0        0    11848 2023-06-07 20:13:22.750698 agixt-1.2.0/docs/README.md
--rw-r--r--   0        0        0     2781 2023-06-07 20:13:22.758698 agixt-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    14782 1970-01-01 00:00:00.000000 agixt-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-06-08 01:05:47.963231 agixt-1.2.0b0/LICENSE
+-rw-r--r--   0        0        0    19409 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/AGiXT.py
+-rw-r--r--   0        0        0    23585 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/Agent.py
+-rw-r--r--   0        0        0    10083 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/Chain.py
+-rw-r--r--   0        0        0     1099 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/Config.py
+-rw-r--r--   0        0        0     5900 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/Embedding.py
+-rw-r--r--   0        0        0     6784 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/Extensions.py
+-rw-r--r--   0        0        0     9489 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/Memories.py
+-rw-r--r--   0        0        0     1986 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/Prompts.py
+-rw-r--r--   0        0        0     7093 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/Tasks.py
+-rw-r--r--   0        0        0       38 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/WORKSPACE/example.txt
+-rw-r--r--   0        0        0      230 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/__init__.py
+-rw-r--r--   0        0        0      244 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/agents/gpt4free/config.json
+-rw-r--r--   0        0        0    17684 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/app.py
+-rw-r--r--   0        0        0     2012 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/chains/Smart Chat.json
+-rw-r--r--   0        0        0     7108 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/chains/Test_Commands.json
+-rw-r--r--   0        0        0     1030 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/chains/Write a Poem.json
+-rw-r--r--   0        0        0    11935 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/example.ipynb
+-rw-r--r--   0        0        0     7807 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/agixt_agent.py
+-rw-r--r--   0        0        0      860 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/briantts.py
+-rw-r--r--   0        0        0     1174 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/dalle.py
+-rw-r--r--   0        0        0     2818 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/discord.py
+-rw-r--r--   0        0        0     1170 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/elevenlabs.py
+-rw-r--r--   0        0        0     6647 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/file_system.py
+-rw-r--r--   0        0        0     1841 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/github.py
+-rw-r--r--   0        0        0     2042 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/google.py
+-rw-r--r--   0        0        0      539 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/gtts.py
+-rw-r--r--   0        0        0     2475 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/huggingface.py
+-rw-r--r--   0        0        0      622 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/macostts.py
+-rw-r--r--   0        0        0     4236 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/microsoft_365.py
+-rw-r--r--   0        0        0     1899 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/searxng.py
+-rw-r--r--   0        0        0     1001 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0        0        0      315 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/times.py
+-rw-r--r--   0        0        0     1169 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/twitter.py
+-rw-r--r--   0        0        0     2287 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/web_playwright.py
+-rw-r--r--   0        0        0      151 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Chat.txt
+-rw-r--r--   0        0        0      181 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0        0        0      991 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Create New Command.txt
+-rw-r--r--   0        0        0     1017 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Execution.txt
+-rw-r--r--   0        0        0     1178 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Instruction.txt
+-rw-r--r--   0        0        0      378 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0        0        0      170 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Pick a Poem Subject.txt
+-rw-r--r--   0        0        0      430 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0        0        0      326 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Prioritize.txt
+-rw-r--r--   0        0        0      236 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0        0        0      270 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Score Response.txt
+-rw-r--r--   0        0        0      349 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0        0        0      274 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0        0        0      304 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0        0        0      148 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0        0        0      474 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0        0        0      528 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0        0        0      458 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0        0        0      433 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0        0        0      160 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0        0        0      507 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0        0        0      560 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0        0        0      192 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0        0        0      162 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0        0        0      162 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Title a Poem.txt
+-rw-r--r--   0        0        0      308 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Validation.txt
+-rw-r--r--   0        0        0      856 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0        0        0      314 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/WebSearch.txt
+-rw-r--r--   0        0        0       43 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Write a Haiku.txt
+-rw-r--r--   0        0        0       43 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Write a Poem.txt
+-rw-r--r--   0        0        0     1178 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
+-rw-r--r--   0        0        0     1178 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0        0        0      777 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/instruct.txt
+-rw-r--r--   0        0        0      824 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/starchat/instruct.txt
+-rw-r--r--   0        0        0      616 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/vicuna/instruct.txt
+-rw-r--r--   0        0        0     2329 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/__init__.py
+-rw-r--r--   0        0        0     1729 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/azure.py
+-rw-r--r--   0        0        0      493 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/bard.py
+-rw-r--r--   0        0        0     1638 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/bing.py
+-rw-r--r--   0        0        0      980 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/chatgpt.py
+-rw-r--r--   0        0        0     1012 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/claude.py
+-rw-r--r--   0        0        0      763 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/fastchat.py
+-rw-r--r--   0        0        0      873 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/gpt4all.py
+-rw-r--r--   0        0        0     5430 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/gpt4free.py
+-rw-r--r--   0        0        0     1194 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0        0        0     1007 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/huggingchat.py
+-rw-r--r--   0        0        0     1438 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/huggingface.py
+-rw-r--r--   0        0        0     1091 2023-06-08 01:05:47.971231 agixt-1.2.0b0/agixt/provider/kobold.py
+-rw-r--r--   0        0        0     2048 2023-06-08 01:05:47.971231 agixt-1.2.0b0/agixt/provider/llamacpp.py
+-rw-r--r--   0        0        0     1071 2023-06-08 01:05:47.971231 agixt-1.2.0b0/agixt/provider/llamacppapi.py
+-rw-r--r--   0        0        0     1585 2023-06-08 01:05:47.971231 agixt-1.2.0b0/agixt/provider/oobabooga.py
+-rw-r--r--   0        0        0     1597 2023-06-08 01:05:47.971231 agixt-1.2.0b0/agixt/provider/openai.py
+-rw-r--r--   0        0        0      850 2023-06-08 01:05:47.971231 agixt-1.2.0b0/agixt/provider/palm.py
+-rw-r--r--   0        0        0     3730 2023-06-08 01:05:47.971231 agixt-1.2.0b0/agixt/provider/runpod.py
+-rw-r--r--   0        0        0     3106 2023-06-08 01:05:47.971231 agixt-1.2.0b0/agixt/provider/transformer.py
+-rw-r--r--   0        0        0    11848 2023-06-08 01:05:47.971231 agixt-1.2.0b0/docs/README.md
+-rw-r--r--   0        0        0     2786 2023-06-08 01:05:47.983232 agixt-1.2.0b0/pyproject.toml
+-rw-r--r--   0        0        0    14784 1970-01-01 00:00:00.000000 agixt-1.2.0b0/PKG-INFO
```

### Comparing `agixt-1.2.0/LICENSE` & `agixt-1.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/AGiXT.py` & `agixt-1.2.0b0/agixt/AGiXT.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/Agent.py` & `agixt-1.2.0b0/agixt/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/Chain.py` & `agixt-1.2.0b0/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/Config.py` & `agixt-1.2.0b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/Embedding.py` & `agixt-1.2.0b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/Extensions.py` & `agixt-1.2.0b0/agixt/Extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,17 @@
         enabled_commands = []
         for command in self.available_commands:
             if command["enabled"]:
                 enabled_commands.append(command)
         return enabled_commands
 
     def get_command_args(self, command_name: str):
-        for command in self.available_commands:
-            if command["friendly_name"] == command_name:
-                return command["args"]
+        for command in self.get_extensions():
+            if command[0] == command_name:
+                return command[2]
         return None
 
     def load_commands(self):
         try:
             settings = self.agent_config["settings"]
         except:
             settings = {}
```

### Comparing `agixt-1.2.0/agixt/Memories.py` & `agixt-1.2.0b0/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/Prompts.py` & `agixt-1.2.0b0/agixt/Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/Tasks.py` & `agixt-1.2.0b0/agixt/Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/app.py` & `agixt-1.2.0b0/agixt/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
 
 class AgentNewName(BaseModel):
     new_name: str
 
 
 class AgentPrompt(BaseModel):
+    user_input: str
     prompt_name: str
     prompt_args: dict
     websearch: bool
     websearch_depth: int
     context_results: int
 
 
@@ -264,21 +265,15 @@
     )
     return {"response": str(response)}
 
 
 @app.post("/api/agent/{agent_name}/prompt", tags=["Agent"])
 async def prompt_agent(agent_name: str, agent_prompt: AgentPrompt):
     agent = AGiXT(agent_name=agent_name)
-    user_input = (
-        agent_prompt.prompt_args["user_input"]
-        if "user_input" in agent_prompt.prompt_args
-        else ""
-    )
     response = await agent.run(
-        user_input=user_input,
         prompt=agent_prompt.prompt_name,
         websearch=agent_prompt.websearch,
         websearch_depth=agent_prompt.websearch_depth,
         context_results=agent_prompt.context_results,
         **agent_prompt.prompt_args,
     )
     return {"response": str(response)}
```

### Comparing `agixt-1.2.0/agixt/chains/Smart Chat.json` & `agixt-1.2.0b0/agixt/chains/Smart Chat.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/chains/Test_Commands.json` & `agixt-1.2.0b0/agixt/chains/Test_Commands.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/chains/Write a Poem.json` & `agixt-1.2.0b0/agixt/chains/Write a Poem.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/example.ipynb` & `agixt-1.2.0b0/agixt/example.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/extensions/agixt_agent.py` & `agixt-1.2.0b0/agixt/extensions/agixt_agent.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,108 +21,149 @@
             "Create a new command": self.create_command,
         }
         if agents != None:
             for agent in agents:
                 if "name" in agent:
                     name = f" AI Agent {agent['name']}"
                     self.commands.update(
-                        {f"Ask{name}": self.ask, f"Instruct{name}": self.instruct}
+                        {
+                            f"Ask{name}": self.ask,
+                            f"Instruct{name}": self.instruct,
+                            f"Prompt{name}": self.prompt_agent,
+                        }
                     )
         if self.chains != None:
             for chain in self.chains:
                 if "name" in chain:
                     self.commands.update(
                         {f"Run Chain: {chain['name']}": self.run_chain}
                     )
 
     def command_exists(self, file_name: str) -> bool:
         return os.path.exists(f"commands/{file_name}.py")
 
     async def create_command(
-        self, function_description: str, agent: str = "AGiXT"
+        self, function_description: str, agent_name: str = "AGiXT"
     ) -> List[str]:
         with open(f"prompts/Create New Command.txt", "r") as f:
             prompt = f.read()
         prompt = prompt.replace("{{NEW_FUNCTION_DESCRIPTION}}", function_description)
-        response = await AGiXT(agent_name=agent).run(user_input=prompt)
+        response = await AGiXT(agent_name=agent_name).run(user_input=prompt)
         file_name = response.split("class ")[1].split("(")[0]
         code = code.replace("```", "")
 
         if not self.command_exists(file_name):
             with open(f"commands/{file_name}.py", "w") as f:
                 f.write(code)
             return f"Created new command: {file_name}."
         else:
             return f"Command {file_name} already exists. No changes were made."
 
-    async def evaluate_code(self, code: str, agent: str = "AGiXT") -> List[str]:
+    async def evaluate_code(self, code: str, agent_name: str = "AGiXT") -> List[str]:
         args = [code]
         function_string = "def analyze_code(code: str) -> List[str]:"
         description_string = "Analyzes the given code and returns a list of suggestions for improvements."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent).run(user_input=prompt)
+        return await AGiXT(agent_name=agent_name).run(user_input=prompt)
 
     async def analyze_pull_request(
-        self, pr_url: str, agent: str = "AGiXT"
+        self, pr_url: str, agent_name: str = "AGiXT"
     ) -> List[str]:
         args = [pr_url]
         function_string = "def analyze_pr(pr_url: str) -> List[str]:"
         description_string = "Analyzes the given pull request and returns a list of suggestions for improvements."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent).run(user_input=prompt)
+        return await AGiXT(agent_name=agent_name).run(user_input=prompt)
 
     async def perform_automated_testing(
-        self, test_url: str, agent: str = "AGiXT"
+        self, test_url: str, agent_name: str = "AGiXT"
     ) -> List[str]:
         args = [test_url]
         function_string = "def perform_testing(test_url: str) -> List[str]:"
         description_string = "Performs automated testing using AI-driven tools and returns a list of test results."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent).run(user_input=prompt)
+        return await AGiXT(agent_name=agent_name).run(user_input=prompt)
 
     async def improve_code(
-        self, suggestions: List[str], code: str, agent: str = "AGiXT"
+        self, suggestions: List[str], code: str, agent_name: str = "AGiXT"
     ) -> str:
         args = [json.dumps(suggestions), code]
         function_string = (
             "def generate_improved_code(suggestions: List[str], code: str) -> str:"
         )
         description_string = "Improves the provided code based on the suggestions provided, making no other changes."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent).run(user_input=prompt)
+        return await AGiXT(agent_name=agent_name).run(user_input=prompt)
 
     async def write_tests(
         self,
         code: str,
         focus: Optional[List[str]] = None,
-        agent: str = "AGiXT",
+        agent_name: str = "AGiXT",
     ) -> str:
         args = [code, json.dumps(focus) if focus else "None"]
         function_string = "def create_test_cases(code: str, focus: Optional[List[str]] = None) -> str:"
         description_string = "Generates test cases for the existing code, focusing on specific areas if required."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent).run(user_input=prompt)
+        return await AGiXT(agent_name=agent_name).run(user_input=prompt)
 
-    async def run_ci_cd_pipeline(self, repo_url: str, agent: str = "AGiXT") -> str:
+    async def run_ci_cd_pipeline(self, repo_url: str, agent_name: str = "AGiXT") -> str:
         args = [repo_url]
         function_string = "def run_pipeline(repo_url: str) -> str:"
         description_string = (
             "Runs the entire CI/CD pipeline for the given repository URL."
         )
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent).run(user_input=prompt)
+        return await AGiXT(agent_name=agent_name).run(user_input=prompt)
 
     async def run_chain(self, chain_name: str = "", user_input: str = ""):
         await Chain().run_chain(chain_name=chain_name, user_input=user_input)
         return "Chain started successfully."
 
-    async def ask(self, user_input: str, agent: str = "AGiXT") -> str:
-        response = await AGiXT(agent).run(
+    async def ask(self, user_input: str, agent_name: str = "AGiXT") -> str:
+        response = await AGiXT(agent_name=agent_name).run(
             user_input=user_input, prompt="chat", websearch=True, websearch_depth=4
         )
         return response
 
-    async def instruct(self, user_input: str, agent: str = "AGiXT") -> str:
-        response = await AGiXT(agent).run(
+    async def instruct(self, user_input: str, agent_name: str = "AGiXT") -> str:
+        response = await AGiXT(agent_name=agent_name).run(
             user_input=user_input, prompt="instruct", websearch=True, websearch_depth=8
         )
         return response
+
+    async def prompt_agent(
+        agent_name: str,
+        user_input: str,
+        prompt_name: int,
+        prompt_args: dict,
+        websearch: bool = False,
+        websearch_depth: int = 3,
+        context_results: int = 5,
+        shots: int = 1,
+    ) -> str:
+        response = await AGiXT(agent_name=agent_name).run(
+            user_input=user_input,
+            prompt=prompt_name,
+            prompt_args=prompt_args,
+            websearch=websearch,
+            websearch_depth=websearch_depth,
+            context_results=context_results,
+        )
+        if shots > 1:
+            responses = [response]
+            for shot in range(shots - 1):
+                response = await AGiXT(agent_name=agent_name).run(
+                    user_input=user_input,
+                    prompt=prompt_name,
+                    prompt_args=prompt_args,
+                    context_results=context_results,
+                )
+                responses.append(response)
+            # Join responses by "Response # <shot number>:" and return
+            return "\n".join(
+                [
+                    f"Response {shot + 1}:\n{response}"
+                    for shot, response in enumerate(responses)
+                ]
+            )
+        return response
```

### Comparing `agixt-1.2.0/agixt/extensions/briantts.py` & `agixt-1.2.0b0/agixt/extensions/briantts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/extensions/dalle.py` & `agixt-1.2.0b0/agixt/extensions/dalle.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/extensions/discord.py` & `agixt-1.2.0b0/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/extensions/elevenlabs.py` & `agixt-1.2.0b0/agixt/extensions/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/extensions/file_system.py` & `agixt-1.2.0b0/agixt/extensions/file_system.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/extensions/github.py` & `agixt-1.2.0b0/agixt/extensions/github.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/extensions/google.py` & `agixt-1.2.0b0/agixt/extensions/google.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/extensions/gtts.py` & `agixt-1.2.0b0/agixt/extensions/gtts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/extensions/huggingface.py` & `agixt-1.2.0b0/agixt/extensions/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/extensions/macostts.py` & `agixt-1.2.0b0/agixt/extensions/macostts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/extensions/microsoft_365.py` & `agixt-1.2.0b0/agixt/extensions/microsoft_365.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/extensions/searxng.py` & `agixt-1.2.0b0/agixt/extensions/searxng.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/extensions/sendgrid_email.py` & `agixt-1.2.0b0/agixt/extensions/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/extensions/twitter.py` & `agixt-1.2.0b0/agixt/extensions/twitter.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/extensions/web_playwright.py` & `agixt-1.2.0b0/agixt/extensions/web_playwright.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/prompts/Create New Command.txt` & `agixt-1.2.0b0/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/prompts/Execution.txt` & `agixt-1.2.0b0/agixt/prompts/Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/prompts/Instruction.txt` & `agixt-1.2.0b0/agixt/prompts/Instruction.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.2.0b0/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.2.0b0/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/prompts/ValidationFailed.txt` & `agixt-1.2.0b0/agixt/prompts/ValidationFailed.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.2.0b0/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.2.0b0/agixt/prompts/gpt-4/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/prompts/instruct.txt` & `agixt-1.2.0b0/agixt/prompts/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/prompts/starchat/instruct.txt` & `agixt-1.2.0b0/agixt/prompts/starchat/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/prompts/vicuna/instruct.txt` & `agixt-1.2.0b0/agixt/prompts/vicuna/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/__init__.py` & `agixt-1.2.0b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/azure.py` & `agixt-1.2.0b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/bing.py` & `agixt-1.2.0b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/chatgpt.py` & `agixt-1.2.0b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/claude.py` & `agixt-1.2.0b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/fastchat.py` & `agixt-1.2.0b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/gpt4all.py` & `agixt-1.2.0b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/gpt4free.py` & `agixt-1.2.0b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/gpugpt4all.py` & `agixt-1.2.0b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/huggingchat.py` & `agixt-1.2.0b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/huggingface.py` & `agixt-1.2.0b0/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/kobold.py` & `agixt-1.2.0b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/llamacpp.py` & `agixt-1.2.0b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/llamacppapi.py` & `agixt-1.2.0b0/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/oobabooga.py` & `agixt-1.2.0b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/openai.py` & `agixt-1.2.0b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/palm.py` & `agixt-1.2.0b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/runpod.py` & `agixt-1.2.0b0/agixt/provider/runpod.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/agixt/provider/transformer.py` & `agixt-1.2.0b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/docs/README.md` & `agixt-1.2.0b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0/pyproject.toml` & `agixt-1.2.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AGiXT"
-version = "v1.2.0"
+version = "v1.2.0-beta"
 description = "An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day."
 homepage = "https://AGiXT.com"
 documentation = "https://AGiXT.com"
 keywords = ["AI", "AGI", "Agent", "skynet"]
 license = "MIT"
 authors = ["Josh XT <josh@devxt.com>"]
 maintainers = [
```

### Comparing `agixt-1.2.0/PKG-INFO` & `agixt-1.2.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.2.0
+Version: 1.2.0b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Home-page: https://AGiXT.com
 License: MIT
 Keywords: AI,AGI,Agent,skynet
 Author: Josh XT
 Author-email: josh@devxt.com
 Maintainer: Josh XT
```

