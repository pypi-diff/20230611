# Comparing `tmp/agixt-1.2.1b0.tar.gz` & `tmp/agixt-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.2.1b0.tar", max compression
+gzip compressed data, was "agixt-1.2.3.tar", last modified: Sun Jun 11 01:20:51 2023, max compression
```

## Comparing `agixt-1.2.1b0.tar` & `agixt-1.2.3.tar`

### file list

```diff
@@ -1,97 +1,198 @@
--rw-r--r--   0        0        0     1087 2023-06-09 02:39:17.188328 agixt-1.2.1b0/LICENSE
--rw-r--r--   0        0        0    19409 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/AGiXT.py
--rw-r--r--   0        0        0    23585 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/Agent.py
--rw-r--r--   0        0        0    10816 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/Chain.py
--rw-r--r--   0        0        0     1099 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/Config.py
--rw-r--r--   0        0        0     5900 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/Embedding.py
--rw-r--r--   0        0        0     6784 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/Extensions.py
--rw-r--r--   0        0        0     9489 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/Memories.py
--rw-r--r--   0        0        0     1986 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/Prompts.py
--rw-r--r--   0        0        0       38 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/WORKSPACE/example.txt
--rw-r--r--   0        0        0      230 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/__init__.py
--rw-r--r--   0        0        0      209 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/agents/gpt4free/config.json
--rw-r--r--   0        0        0    16006 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/app.py
--rw-r--r--   0        0        0     1839 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/chains/Poem Writing Chain/responses.json
--rw-r--r--   0        0        0     1126 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/chains/Smart Chat.json
--rw-r--r--   0        0        0     1142 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/chains/Smart Instruct.json
--rw-r--r--   0        0        0      744 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/chains/Task.json
--rw-r--r--   0        0        0     7108 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/chains/Test_Commands.json
--rw-r--r--   0        0        0     1030 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/chains/Write a Poem.json
--rw-r--r--   0        0        0    11935 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/example.ipynb
--rw-r--r--   0        0        0     8806 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/agixt_agent.py
--rw-r--r--   0        0        0      860 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/briantts.py
--rw-r--r--   0        0        0     1174 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/dalle.py
--rw-r--r--   0        0        0     2818 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/discord.py
--rw-r--r--   0        0        0     1170 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/elevenlabs.py
--rw-r--r--   0        0        0     6647 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/file_system.py
--rw-r--r--   0        0        0     1841 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/github.py
--rw-r--r--   0        0        0     2042 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/google.py
--rw-r--r--   0        0        0      539 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/gtts.py
--rw-r--r--   0        0        0     2475 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/huggingface.py
--rw-r--r--   0        0        0      622 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/macostts.py
--rw-r--r--   0        0        0     4236 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/microsoft_365.py
--rw-r--r--   0        0        0     1899 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/searxng.py
--rw-r--r--   0        0        0     1001 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/sendgrid_email.py
--rw-r--r--   0        0        0      315 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/times.py
--rw-r--r--   0        0        0     1169 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/twitter.py
--rw-r--r--   0        0        0     2287 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/web_playwright.py
--rw-r--r--   0        0        0      151 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Chat.txt
--rw-r--r--   0        0        0      181 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0        0        0      991 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Create New Command.txt
--rw-r--r--   0        0        0     1017 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Execution.txt
--rw-r--r--   0        0        0      396 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Get Task List.txt
--rw-r--r--   0        0        0     1178 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Instruction.txt
--rw-r--r--   0        0        0      378 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0        0        0      170 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Pick a Poem Subject.txt
--rw-r--r--   0        0        0      430 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0        0        0      326 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Prioritize.txt
--rw-r--r--   0        0        0      236 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0        0        0      270 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Score Response.txt
--rw-r--r--   0        0        0      349 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0        0        0      268 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0        0        0      298 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0        0        0      148 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0        0        0      474 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0        0        0      528 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0        0        0      452 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0        0        0      427 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0        0        0      160 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0        0        0      507 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0        0        0      560 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0        0        0      192 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0        0        0      836 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Task Execution.txt
--rw-r--r--   0        0        0      162 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Tell Me How.txt
--rw-r--r--   0        0        0      162 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Title a Poem.txt
--rw-r--r--   0        0        0      308 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Validation.txt
--rw-r--r--   0        0        0      856 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0        0        0      314 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/WebSearch.txt
--rw-r--r--   0        0        0       43 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Write a Haiku.txt
--rw-r--r--   0        0        0       43 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Write a Poem.txt
--rw-r--r--   0        0        0     1178 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
--rw-r--r--   0        0        0     1178 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0        0        0      777 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/instruct.txt
--rw-r--r--   0        0        0      824 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/starchat/instruct.txt
--rw-r--r--   0        0        0      616 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/vicuna/instruct.txt
--rw-r--r--   0        0        0     2329 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/__init__.py
--rw-r--r--   0        0        0     1729 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/azure.py
--rw-r--r--   0        0        0      493 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/bard.py
--rw-r--r--   0        0        0     1638 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/bing.py
--rw-r--r--   0        0        0      980 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/chatgpt.py
--rw-r--r--   0        0        0     1012 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/claude.py
--rw-r--r--   0        0        0      763 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/fastchat.py
--rw-r--r--   0        0        0      873 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/gpt4all.py
--rw-r--r--   0        0        0     5430 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/gpt4free.py
--rw-r--r--   0        0        0     1194 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0        0        0     1007 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/huggingchat.py
--rw-r--r--   0        0        0     1438 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/huggingface.py
--rw-r--r--   0        0        0     1091 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/kobold.py
--rw-r--r--   0        0        0     2048 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/llamacpp.py
--rw-r--r--   0        0        0     1071 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/llamacppapi.py
--rw-r--r--   0        0        0     1585 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/oobabooga.py
--rw-r--r--   0        0        0     1597 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/openai.py
--rw-r--r--   0        0        0      850 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/palm.py
--rw-r--r--   0        0        0     3730 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/runpod.py
--rw-r--r--   0        0        0     3106 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/transformer.py
--rw-r--r--   0        0        0    11862 2023-06-09 02:39:17.192328 agixt-1.2.1b0/docs/README.md
--rw-r--r--   0        0        0     2786 2023-06-09 02:39:17.204328 agixt-1.2.1b0/pyproject.toml
--rw-r--r--   0        0        0    14798 1970-01-01 00:00:00.000000 agixt-1.2.1b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.767129 agixt-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-11 01:20:40.000000 agixt-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-11 01:20:40.000000 agixt-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-06-11 01:20:51.767129 agixt-1.2.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.735129 agixt-1.2.3/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/Extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19416 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/Interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/Prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.735129 agixt-1.2.3/agixt/WORKSPACE/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/WORKSPACE/example.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.727129 agixt-1.2.3/agixt/agents/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.735129 agixt-1.2.3/agixt/agents/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/agents/gpt4free/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.735129 agixt-1.2.3/agixt/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/chains/Smart Chat.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/chains/Smart Instruct.json
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/chains/Task.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/chains/Test_Commands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/chains/Write a Poem.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.739129 agixt-1.2.3/agixt/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/agixt_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/briantts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/dalle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/gtts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/macostts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/microsoft_365.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/searxng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/web_playwright.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.747129 agixt-1.2.3/agixt/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Chat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Create New Command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Custom Input.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Get Task List.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Instruction.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Pick a Poem Subject.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Prioritize.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Score Response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Task Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Title a Poem.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Validation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/WebSearch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Write a Haiku.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Write a Poem.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.747129 agixt-1.2.3/agixt/prompts/gpt-3.5-turbo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/gpt-3.5-turbo/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.747129 agixt-1.2.3/agixt/prompts/gpt-4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.747129 agixt-1.2.3/agixt/prompts/starchat/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/starchat/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.747129 agixt-1.2.3/agixt/prompts/vicuna/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/vicuna/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.751129 agixt-1.2.3/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/llamacppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.735129 agixt-1.2.3/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-06-11 01:20:51.000000 agixt-1.2.3/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-11 01:20:51.000000 agixt-1.2.3/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 01:20:51.000000 agixt-1.2.3/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-11 01:20:51.000000 agixt-1.2.3/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 01:20:51.000000 agixt-1.2.3/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.751129 agixt-1.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.751129 agixt-1.2.3/docs/1-Getting started/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/1-Getting started/Quick Start.md
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/1-Getting started/Support.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.755129 agixt-1.2.3/docs/2-Concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/0-Core Concepts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Agents.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Chains.md
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Commands.md
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Instructions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Prompts.md
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Providers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Smart Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Smart Instruct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Smart Task.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Tasks.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.755129 agixt-1.2.3/docs/3-Providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/Anthropic Claude.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/Azure OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/ChatGPT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/FastChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/GPT4ALL-GPU.md
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/GPT4ALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/GPT4Free.md
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/Google Bard.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/Google Palm.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/Hugging Face Transformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/HuggingChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/Kobold.md
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/Microsoft Bing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/Oobabooga Text Generation Web UI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/llamacpp API.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/llamacpp.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.759129 agixt-1.2.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/AGiXT-gradient-flat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/AGiXT-gradient-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/AGiXT.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/AGiXT.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1707562 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/AGiXT_Original_PSD.psd
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/AGiXTwhiteborder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/Docker-desktop-win-setting-streamlit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/Smart Instruct.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/Smart Instruct.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/Smart Tasks.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/Smart Tasks.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/Untitled Diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-11 01:20:40.000000 agixt-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-11 01:20:40.000000 agixt-1.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 01:20:51.767129 agixt-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-11 01:20:40.000000 agixt-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.763129 agixt-1.2.3/streamlit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.763129 agixt-1.2.3/streamlit/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/ApiClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/Main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.763129 agixt-1.2.3/streamlit/auth_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/auth_libs/Cfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/auth_libs/Redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/auth_libs/Users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.763129 agixt-1.2.3/streamlit/auth_libs/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/auth_libs/pages/Login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/auth_libs/pages/Profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/auth_libs/pages/Register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.763129 agixt-1.2.3/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/components/agent_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/components/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/components/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/components/learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/components/verify_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.763129 agixt-1.2.3/streamlit/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/pages/0-Agent_Settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/pages/1-Prompt_Templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16638 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/pages/2-Chain_Management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/pages/3-Interact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.763129 agixt-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-06-11 01:20:40.000000 agixt-1.2.3/tests/ApiClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-11 01:20:40.000000 agixt-1.2.3/tests/test-commands.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    52056 2023-06-11 01:20:40.000000 agixt-1.2.3/tests/tests.ipynb
```

### Comparing `agixt-1.2.1b0/LICENSE` & `agixt-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/AGiXT.py` & `agixt-1.2.3/agixt/Interactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from Prompts import Prompts
 from extensions.searxng import searxng
 from urllib.parse import urlparse
 import logging
 from concurrent.futures import Future
 
 
-class AGiXT:
+class Interactions:
     def __init__(self, agent_name: str = "AGiXT"):
         self.agent_name = agent_name
         self.agent = Agent(self.agent_name)
         self.agent_commands = self.agent.get_commands_string()
         self.stop_running_event = None
         self.browsed_links = []
         self.failures = 0
```

### Comparing `agixt-1.2.1b0/agixt/Chain.py` & `agixt-1.2.3/agixt/Chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import json
-from AGiXT import AGiXT
+from Interactions import Interactions
 import argparse
 from Extensions import Extensions
 import logging
 from datetime import datetime
 
 
 class Chain:
@@ -112,18 +112,23 @@
     async def run_chain(self, chain_name, user_input=None):
         chain_data = self.get_chain(chain_name=chain_name)
         logging.info(f"Running chain '{chain_name}'")
         responses = {}  # Create a dictionary to hold responses.
         for step_data in chain_data["steps"]:
             if "prompt" in step_data and "step" in step_data:
                 logging.info(f"Running step {step_data['step']}")
+                step = {}
                 step_response = await self.run_chain_step(
                     step=step_data, chain_name=chain_name, user_input=user_input
                 )  # Get the response of the current step.
-                responses[step_data["step"]] = step_response  # Store the response.
+                step["response"] = step_response
+                step["agent_name"] = step_data["agent_name"]
+                step["prompt"] = step_data["prompt"]
+                step["prompt_type"] = step_data["prompt_type"]
+                responses[step_data["step"]] = step  # Store the response.
                 logging.info(f"Response: {step_response}")
                 # Write the responses to the json file.
                 dt = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
                 with open(
                     os.path.join("chains", chain_name, "responses.json"), "w"
                 ) as f:
                     json.dump(responses, f)
@@ -165,15 +170,15 @@
                         new_step_number = int(value.split("{STEP")[1].split("}")[0])
                         # get the response from the step number
                         step_response = self.get_step_response(
                             chain_name=chain_name, step_number=new_step_number
                         )
                         # replace the {STEPx} with the response
                         value = value.replace(
-                            f"{{STEP{new_step_number}}}", step_response
+                            f"{{STEP{new_step_number}}}", f"{step_response['response']}"
                         )
                 new_prompt_content[arg] = value
         elif isinstance(prompt_content, str):
             new_prompt_content = prompt_content
             if "{user_input}" in prompt_content:
                 new_prompt_content = new_prompt_content.replace(
                     "{user_input}", user_input
@@ -191,26 +196,26 @@
                     )
                     # get the response from the step number
                     step_response = self.get_step_response(
                         chain_name=chain_name, step_number=new_step_number
                     )
                     # replace the {STEPx} with the response
                     new_prompt_content = prompt_content.replace(
-                        f"{{STEP{new_step_number}}}", step_response
+                        f"{{STEP{new_step_number}}}", f"{step_response['response']}"
                     )
             if new_prompt_content == {}:
                 new_prompt_content = prompt_content
         return new_prompt_content
 
     async def run_chain_step(self, step: dict = {}, chain_name="", user_input=""):
         logging.info(step)
         if step:
             if "prompt_type" in step:
                 agent_name = step["agent_name"]
-                agent = AGiXT(agent_name)
+                agent = Interactions(agent_name)
                 prompt_type = step["prompt_type"]
                 step_number = step["step"]
                 if "prompt_name" in step["prompt"]:
                     prompt_name = step["prompt"]["prompt_name"]
                 else:
                     prompt_name = ""
                 args = self.get_step_content(
```

### Comparing `agixt-1.2.1b0/agixt/Embedding.py` & `agixt-1.2.3/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/Extensions.py` & `agixt-1.2.3/agixt/Extensions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/Memories.py` & `agixt-1.2.3/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/Prompts.py` & `agixt-1.2.3/agixt/Prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
             os.mkdir("prompts")
         # if prompt file does not exist, create it
         if not os.path.exists(os.path.join("prompts", f"{prompt_name}.txt")):
             with open(os.path.join("prompts", f"{prompt_name}.txt"), "w") as f:
                 f.write(prompt)
 
     def get_prompt(self, prompt_name, model="default"):
-        model_prompt_file = f"prompts/{model}/{prompt_name}.txt"
+        model_prompt_file = os.path.join("prompts", f"{model}", f"{prompt_name}.txt")
         default_prompt_file = os.path.join("prompts", f"{prompt_name}.txt")
 
         prompt_file = (
             model_prompt_file
             if os.path.isfile(model_prompt_file)
             else default_prompt_file
         )
```

### Comparing `agixt-1.2.1b0/agixt/app.py` & `agixt-1.2.3/agixt/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import uvicorn
 from fastapi import FastAPI, HTTPException
 from fastapi.middleware.cors import CORSMiddleware
 from pydantic import BaseModel
-from Config import Config
-from AGiXT import AGiXT
-from Agent import Agent
+from Interactions import Interactions
+from Agent import Agent, add_agent, delete_agent, rename_agent, get_agents
 from Chain import Chain
 from Prompts import Prompts
 from typing import Optional, Dict, List, Any
-from provider import get_provider_options
+from provider import get_provider_options, get_providers
 from Embedding import get_embedding_providers
 from Extensions import Extensions
 import os
 import logging
-import argparse
-import asyncio
 
-CFG = Config()
+this_directory = os.path.abspath(os.path.dirname(__file__))
+with open(os.path.join(this_directory, "version"), encoding="utf-8") as f:
+    version = f.read().strip()
+
+logging.basicConfig(
+    level=os.environ.get("LOGLEVEL", "INFO"),
+    format="%(asctime)s | %(levelname)s | %(message)s",
+)
+
 app = FastAPI(
     title="AGiXT",
     description="AGiXT is an Artificial Intelligence Automation platform for creating and managing AI agents. Visit the GitHub repo for more information or to report issues. https://github.com/Josh-XT/AGiXT/",
-    version="1.0.0",  # API version according to https://restfulapi.net/versioning/
+    version=version,
     docs_url="/",
 )
-agent_threads = {}
-agent_stop_events = {}
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"],
@@ -79,14 +82,21 @@
 class StepInfo(BaseModel):
     step_number: int
     agent_name: str
     prompt_type: str
     prompt: dict
 
 
+class RunChainResponse(BaseModel):
+    response: str
+    agent_name: str
+    prompt: dict
+    prompt_type: str
+
+
 class ChainStep(BaseModel):
     step_number: int
     agent_name: str
     prompt_type: str
     prompt: dict
 
 
@@ -130,16 +140,16 @@
 
 class AgentCommands(BaseModel):
     agent_name: str
     commands: Dict[str, Any]
 
 
 @app.get("/api/provider", tags=["Provider"])
-async def get_providers():
-    providers = CFG.get_providers()
+async def getproviders():
+    providers = get_providers()
     return {"providers": providers}
 
 
 @app.get("/api/provider/{provider_name}", tags=["Provider"])
 async def get_provider_settings(provider_name: str):
     settings = get_provider_options(provider_name=provider_name)
     return {"settings": settings}
@@ -148,29 +158,22 @@
 @app.get("/api/embedding_providers", tags=["Provider"])
 async def get_embed_providers():
     providers = get_embedding_providers()
     return {"providers": providers}
 
 
 @app.post("/api/agent", tags=["Agent"])
-async def add_agent(agent: AgentSettings) -> Dict[str, str]:
-    agent_info = Agent(agent.agent_name).add_agent(
-        agent_name=agent.agent_name, provider_settings=agent.settings
-    )
-    return {"message": "Agent added", "agent_file": agent_info["agent_file"]}
+async def addagent(agent: AgentSettings) -> Dict[str, str]:
+    return add_agent(agent_name=agent.agent_name, provider_settings=agent.settings)
 
 
 @app.patch("/api/agent/{agent_name}", tags=["Agent"])
-async def rename_agent(agent_name: str, new_name: AgentNewName) -> ResponseMessage:
-    Agent(agent_name=agent_name).rename_agent(
-        agent_name=agent_name, new_name=new_name.new_name
-    )
-    return ResponseMessage(
-        message=f"Agent {agent_name} renamed to {new_name.new_name}."
-    )
+async def renameagent(agent_name: str, new_name: AgentNewName) -> ResponseMessage:
+    rename_agent(agent_name=agent_name, new_name=new_name.new_name)
+    return ResponseMessage(message="Agent renamed.")
 
 
 @app.put("/api/agent/{agent_name}", tags=["Agent"])
 async def update_agent_settings(
     agent_name: str, settings: AgentSettings
 ) -> ResponseMessage:
     update_config = Agent(agent_name=agent_name).update_agent_config(
@@ -217,90 +220,91 @@
     update_config = Agent(agent_name=agent_name).update_agent_config(
         new_config=commands.commands, config_key="commands"
     )
     return ResponseMessage(message=update_config)
 
 
 @app.delete("/api/agent/{agent_name}", tags=["Agent"])
-async def delete_agent(agent_name: str) -> ResponseMessage:
-    result, status_code = Agent(agent_name=agent_name).delete_agent(
-        agent_name=agent_name
-    )
-    if status_code == 200:
-        return ResponseMessage(message=result["message"])
-    else:
-        raise HTTPException(status_code=status_code, detail=result["message"])
+async def deleteagent(agent_name: str) -> ResponseMessage:
+    delete_agent(agent_name=agent_name)
+    return ResponseMessage(message=f"Agent {agent_name} deleted.")
 
 
 @app.get("/api/agent", tags=["Agent"])
-async def get_agents():
-    agents = CFG.get_agents()
+async def getagents():
+    agents = get_agents()
     return {"agents": agents}
 
 
 @app.get("/api/agent/{agent_name}", tags=["Agent"])
 async def get_agentconfig(agent_name: str):
     agent_config = Agent(agent_name=agent_name).get_agent_config()
     return {"agent": agent_config}
 
 
 @app.get("/api/{agent_name}/chat", tags=["Agent"])
 async def get_chat_history(agent_name: str):
-    chat_history = Agent(agent_name=agent_name).get_chat_history(agent_name=agent_name)
+    chat_history = Agent(agent_name=agent_name).get_history()
     return {"chat_history": chat_history}
 
 
+@app.delete("/api/agent/{agent_name}/history", tags=["Agent"])
+async def delete_history(agent_name: str) -> ResponseMessage:
+    Agent(agent_name=agent_name).delete_history()
+    return ResponseMessage(message=f"History for agent {agent_name} deleted.")
+
+
 @app.delete("/api/agent/{agent_name}/memory", tags=["Agent"])
 async def wipe_agent_memories(agent_name: str) -> ResponseMessage:
-    Agent(agent_name=agent_name).wipe_agent_memories(agent_name=agent_name)
+    Agent(agent_name=agent_name).wipe_agent_memories()
     return ResponseMessage(message=f"Memories for agent {agent_name} deleted.")
 
 
 @app.post("/api/agent/{agent_name}/instruct", tags=["Agent"])
 async def instruct(agent_name: str, prompt: Prompt):
-    agent = AGiXT(agent_name=agent_name)
+    agent = Interactions(agent_name=agent_name)
     response = await agent.run(
         user_input=prompt.prompt,
         prompt="instruct",
     )
     return {"response": str(response)}
 
 
 @app.post("/api/agent/{agent_name}/prompt", tags=["Agent"])
 async def prompt_agent(agent_name: str, agent_prompt: AgentPrompt):
-    agent = AGiXT(agent_name=agent_name)
+    agent = Interactions(agent_name=agent_name)
     response = await agent.run(
         prompt=agent_prompt.prompt_name,
         websearch=agent_prompt.websearch,
         websearch_depth=agent_prompt.websearch_depth,
         context_results=agent_prompt.context_results,
         **agent_prompt.prompt_args,
     )
     return {"response": str(response)}
 
 
 @app.post("/api/agent/{agent_name}/smartinstruct/{shots}", tags=["Agent"])
 async def smartinstruct(agent_name: str, shots: int, prompt: Prompt):
-    agent = AGiXT(agent_name=agent_name)
+    agent = Interactions(agent_name=agent_name)
     response = await agent.smart_instruct(user_input=prompt.prompt, shots=int(shots))
     return {"response": str(response)}
 
 
 @app.post("/api/agent/{agent_name}/chat", tags=["Agent"])
 async def chat(agent_name: str, prompt: Prompt):
-    agent = AGiXT(agent_name=agent_name)
+    agent = Interactions(agent_name=agent_name)
     response = await agent.run(
         user_input=prompt.prompt, prompt="Chat", context_results=6
     )
     return {"response": str(response)}
 
 
 @app.post("/api/agent/{agent_name}/smartchat/{shots}", tags=["Agent"])
 async def smartchat(agent_name: str, shots: int, prompt: Prompt):
-    agent = AGiXT(agent_name=agent_name)
+    agent = Interactions(agent_name=agent_name)
     response = await agent.smart_chat(user_input=prompt.prompt, shots=shots)
     return {"response": str(response)}
 
 
 @app.get("/api/agent/{agent_name}/command", tags=["Agent"])
 async def get_commands(agent_name: str):
     agent = Agent(agent_name=agent_name)
@@ -352,26 +356,28 @@
         chain_data = Chain().get_chain(chain_name=chain_name)
         return {"chain": chain_data}
     except:
         raise HTTPException(status_code=404, detail="Chain not found")
 
 
 @app.get("/api/chain/{chain_name}/responses", tags=["Chain"])
-async def get_chain(chain_name: str):
+async def get_chain_responses(chain_name: str):
     try:
         chain_data = Chain().get_step_response(chain_name=chain_name, step_number="all")
         return {"chain": chain_data}
     except:
         raise HTTPException(status_code=404, detail="Chain not found")
 
 
 @app.post("/api/chain/{chain_name}/run", tags=["Chain"])
-async def run_chain(chain_name: str, user_input: Prompt) -> ResponseMessage:
-    await Chain().run_chain(chain_name=chain_name, user_input=user_input.prompt)
-    return {"message": f"Chain '{chain_name}' completed."}
+async def run_chain(chain_name: str, user_input: Prompt):
+    chain_response = await Chain().run_chain(
+        chain_name=chain_name, user_input=user_input.prompt
+    )
+    return chain_response
 
 
 @app.post("/api/chain", tags=["Chain"])
 async def add_chain(chain_name: ChainName) -> ResponseMessage:
     Chain().add_chain(chain_name=chain_name.chain_name)
     return ResponseMessage(message=f"Chain '{chain_name.chain_name}' created.")
```

### Comparing `agixt-1.2.1b0/agixt/chains/Smart Chat.json` & `agixt-1.2.3/agixt/chains/Smart Chat.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/chains/Smart Instruct.json` & `agixt-1.2.3/agixt/chains/Smart Instruct.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/chains/Task.json` & `agixt-1.2.3/agixt/chains/Task.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/chains/Test_Commands.json` & `agixt-1.2.3/agixt/chains/Test_Commands.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/chains/Write a Poem.json` & `agixt-1.2.3/agixt/chains/Write a Poem.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/example.ipynb` & `agixt-1.2.3/agixt/example.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996562850729518%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'from Interactions import Interactions, Prompts\\n'), "*

 * *            "(3, 'ai = Interactions(agent_name)\\n')], delete: [3, 0]}}, 3: {'source': {insert: "*

 * *            "[(0, 'from Interactions import Interactions, Prompts\\n'), (21, 'ai = "*

 * *            "Interactions(agent_name)\\n')], delete: [21, 0]}}}"}*

```diff
@@ -40,18 +40,18 @@
                         "Collaboration also involves encouraging feedback and input from all stakeholders. This includes not only team members but also clients and end-users. By soliciting feedback from these groups, software projects can be tailored to meet their specific needs and requirements. This also ensures that the final product is user-friendly and meets the needs of the intended audience.\n",
                         "\n",
                         "In conclusion, collaboration is critical for the success of software products and the growth of the industry. It starts with communication, teamwork, and feedback, and requires a culture of inclusiveness and mutual respect. At our software company, we strive to foster collaboration at every level of our organization to deliver the best possible software solutions to our clients and end-users. We believe that by working together, we can achieve success and innovation in the software industry.\n"
                     ]
                 }
             ],
             "source": [
-                "from AGiXT import AGiXT, Prompts\n",
+                "from Interactions import Interactions, Prompts\n",
                 "\n",
                 "agent_name = \"gpt4free\"\n",
-                "ai = AGiXT(agent_name)\n",
+                "ai = Interactions(agent_name)\n",
                 "\n",
                 "Prompts().add_prompt(\n",
                 "    prompt_name=\"Write a blog post\",\n",
                 "    prompt=\"Write a blog post for the {industry} instustry. For context, here is a description of my business: {business_description}\",\n",
                 ")\n",
                 "\n",
                 "response = ai.run(\n",
@@ -87,15 +87,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from AGiXT import AGiXT, Prompts\n",
+                "from Interactions import Interactions, Prompts\n",
                 "from Chain import Chain\n",
                 "\n",
                 "chain = Chain()\n",
                 "cp = Prompts()\n",
                 "\n",
                 "# Set your agent, we'll use gpt4free as the default for now unless you have an agent set up.\n",
                 "agent_name = \"gpt4free\"\n",
@@ -108,15 +108,15 @@
                 "# This chain is now flexible and powerful for any business.\n",
                 "\n",
                 "industry = \"software\"\n",
                 "business_description = \"We're a artificial intelligence software development company.\"\n",
                 "website = \"https://devxt.com\"\n",
                 "\n",
                 "# Set up your ai agent\n",
-                "ai = AGiXT(agent_name)\n",
+                "ai = Interactions(agent_name)\n",
                 "\n",
                 "# Create the new chain to start adding steps to.\n",
                 "chain.add_chain(chain_name)\n"
             ]
         },
         {
             "attachments": {},
```

### Comparing `agixt-1.2.1b0/agixt/extensions/agixt_agent.py` & `agixt-1.2.3/agixt/extensions/agixt_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from Extensions import Extensions
-from Config import Config
+from Agent import get_agents
 from Chain import Chain
-from AGiXT import AGiXT
+from Interactions import Interactions
 import json
 import os
 from typing import List, Optional
 
 
 class agixt_agent(Extensions):
     def __init__(self, **kwargs):
-        agents = Config().get_agents()
+        agents = get_agents()
         self.chains = Chain().get_chains()
         self.commands = {
             "Evaluate Code": self.evaluate_code,
             "Analyze Pull Request": self.analyze_pull_request,
             "Perform Automated Testing": self.perform_automated_testing,
             "Run CI-CD Pipeline": self.run_ci_cd_pipeline,
             "Improve Code": self.improve_code,
@@ -45,15 +45,15 @@
 
     async def create_command(
         self, function_description: str, agent: str = "AGiXT"
     ) -> List[str]:
         with open(f"prompts/Create New Command.txt", "r") as f:
             prompt = f.read()
         prompt = prompt.replace("{{NEW_FUNCTION_DESCRIPTION}}", function_description)
-        response = await AGiXT(agent_name=agent).run(user_input=prompt)
+        response = await Interactions(agent_name=agent).run(user_input=prompt)
         file_name = response.split("class ")[1].split("(")[0]
         code = code.replace("```", "")
 
         if not self.command_exists(file_name):
             with open(f"commands/{file_name}.py", "w") as f:
                 f.write(code)
             return f"Created new command: {file_name}."
@@ -61,104 +61,104 @@
             return f"Command {file_name} already exists. No changes were made."
 
     async def evaluate_code(self, code: str, agent: str = "AGiXT") -> List[str]:
         args = [code]
         function_string = "def analyze_code(code: str) -> List[str]:"
         description_string = "Analyzes the given code and returns a list of suggestions for improvements."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent_name=agent).run(user_input=prompt)
+        return await Interactions(agent_name=agent).run(user_input=prompt)
 
     async def analyze_pull_request(
         self, pr_url: str, agent: str = "AGiXT"
     ) -> List[str]:
         args = [pr_url]
         function_string = "def analyze_pr(pr_url: str) -> List[str]:"
         description_string = "Analyzes the given pull request and returns a list of suggestions for improvements."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent_name=agent).run(user_input=prompt)
+        return await Interactions(agent_name=agent).run(user_input=prompt)
 
     async def perform_automated_testing(
         self, test_url: str, agent: str = "AGiXT"
     ) -> List[str]:
         args = [test_url]
         function_string = "def perform_testing(test_url: str) -> List[str]:"
         description_string = "Performs automated testing using AI-driven tools and returns a list of test results."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent_name=agent).run(user_input=prompt)
+        return await Interactions(agent_name=agent).run(user_input=prompt)
 
     async def improve_code(
         self, suggestions: List[str], code: str, agent: str = "AGiXT"
     ) -> str:
         args = [json.dumps(suggestions), code]
         function_string = (
             "def generate_improved_code(suggestions: List[str], code: str) -> str:"
         )
         description_string = "Improves the provided code based on the suggestions provided, making no other changes."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent_name=agent).run(user_input=prompt)
+        return await Interactions(agent_name=agent).run(user_input=prompt)
 
     async def write_tests(
         self,
         code: str,
         focus: Optional[List[str]] = None,
         agent: str = "AGiXT",
     ) -> str:
         args = [code, json.dumps(focus) if focus else "None"]
         function_string = "def create_test_cases(code: str, focus: Optional[List[str]] = None) -> str:"
         description_string = "Generates test cases for the existing code, focusing on specific areas if required."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent_name=agent).run(user_input=prompt)
+        return await Interactions(agent_name=agent).run(user_input=prompt)
 
     async def run_ci_cd_pipeline(self, repo_url: str, agent: str = "AGiXT") -> str:
         args = [repo_url]
         function_string = "def run_pipeline(repo_url: str) -> str:"
         description_string = (
             "Runs the entire CI/CD pipeline for the given repository URL."
         )
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent_name=agent).run(user_input=prompt)
+        return await Interactions(agent_name=agent).run(user_input=prompt)
 
     async def run_chain(self, chain_name: str = "", user_input: str = ""):
         await Chain().run_chain(chain_name=chain_name, user_input=user_input)
         return "Chain started successfully."
 
     async def ask(self, user_input: str, agent: str = "AGiXT") -> str:
-        response = await AGiXT(agent_name=agent).run(
+        response = await Interactions(agent_name=agent).run(
             user_input=user_input, prompt="chat", websearch=True, websearch_depth=4
         )
         return response
 
     async def instruct(self, user_input: str, agent: str = "AGiXT") -> str:
-        response = await AGiXT(agent_name=agent).run(
+        response = await Interactions(agent_name=agent).run(
             user_input=user_input, prompt="instruct", websearch=True, websearch_depth=8
         )
         return response
 
     async def prompt_agent(
         agent: str,
         user_input: str,
         prompt_name: int,
         prompt_args: dict,
         websearch: bool = False,
         websearch_depth: int = 3,
         context_results: int = 5,
         shots: int = 1,
     ) -> str:
-        response = await AGiXT(agent_name=agent).run(
+        response = await Interactions(agent_name=agent).run(
             user_input=user_input,
             prompt=prompt_name,
             prompt_args=prompt_args,
             websearch=websearch,
             websearch_depth=websearch_depth,
             context_results=context_results,
         )
         if shots > 1:
             responses = [response]
             for shot in range(shots - 1):
-                response = await AGiXT(agent_name=agent).run(
+                response = await Interactions(agent_name=agent).run(
                     user_input=user_input,
                     prompt=prompt_name,
                     prompt_args=prompt_args,
                     context_results=context_results,
                 )
                 responses.append(response)
             # Join responses by "Response # <shot number>:" and return
@@ -184,15 +184,15 @@
             task
             for task in task_list
             if task and task[0] in [str(i) for i in range(10)]
         ]
         responses = []
         for task in task_list:
             if "task_name" in task:
-                response = await AGiXT(agent_name=agent).run(
+                response = await Interactions(agent_name=agent).run(
                     user_input=user_input,
                     prompt="Task Execution",
                     prompt_args={
                         "task": task["task_name"],
                     },
                     websearch=websearch,
                     websearch_depth=websearch_depth,
```

### Comparing `agixt-1.2.1b0/agixt/extensions/briantts.py` & `agixt-1.2.3/agixt/extensions/briantts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/extensions/dalle.py` & `agixt-1.2.3/agixt/extensions/dalle.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/extensions/discord.py` & `agixt-1.2.3/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/extensions/elevenlabs.py` & `agixt-1.2.3/agixt/extensions/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/extensions/file_system.py` & `agixt-1.2.3/agixt/extensions/file_system.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/extensions/github.py` & `agixt-1.2.3/agixt/extensions/github.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 import git
 from github import Github
 from Extensions import Extensions
 
 
 class github(Extensions):
     def __init__(
@@ -23,16 +25,18 @@
         if self.GITHUB_USERNAME is not None and self.GITHUB_API_KEY is not None:
             auth_repo_url = f"//{self.GITHUB_USERNAME}:{self.GITHUB_API_KEY}@".join(
                 split_url
             )
         else:
             auth_repo_url = "//".join(split_url)
         try:
-            git.Repo.clone_from(auth_repo_url, self.WORKING_DIRECTORY + clone_path)
-            return f"""Cloned {repo_url} to {self.WORKING_DIRECTORY + clone_path}"""
+            git.Repo.clone_from(
+                auth_repo_url, os.path.join(self.WORKING_DIRECTORY, clone_path)
+            )
+            return f"""Cloned {repo_url} to {os.path.join(self.WORKING_DIRECTORY, clone_path)}"""
         except Exception as e:
             return f"Error: {str(e)}"
 
     async def create_repo(self, repo_name: str, readme: str) -> str:
         g = Github(self.GITHUB_API_KEY)
         user = g.get_user(self.GITHUB_USERNAME)
         repo = user.create_repo(repo_name, private=True)
```

### Comparing `agixt-1.2.1b0/agixt/extensions/google.py` & `agixt-1.2.3/agixt/extensions/google.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/extensions/gtts.py` & `agixt-1.2.3/agixt/extensions/gtts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/extensions/huggingface.py` & `agixt-1.2.3/agixt/extensions/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/extensions/macostts.py` & `agixt-1.2.3/agixt/extensions/macostts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/extensions/microsoft_365.py` & `agixt-1.2.3/agixt/extensions/microsoft_365.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/extensions/searxng.py` & `agixt-1.2.3/agixt/extensions/searxng.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/extensions/sendgrid_email.py` & `agixt-1.2.3/agixt/extensions/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/extensions/twitter.py` & `agixt-1.2.3/agixt/extensions/twitter.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/extensions/web_playwright.py` & `agixt-1.2.3/agixt/extensions/web_playwright.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/prompts/Create New Command.txt` & `agixt-1.2.3/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/prompts/Execution.txt` & `agixt-1.2.3/agixt/prompts/Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/prompts/Instruction.txt` & `agixt-1.2.3/agixt/prompts/Instruction.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.2.3/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.2.3/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/prompts/Task Execution.txt` & `agixt-1.2.3/agixt/prompts/Task Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/prompts/ValidationFailed.txt` & `agixt-1.2.3/agixt/prompts/ValidationFailed.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.2.3/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.2.3/agixt/prompts/gpt-4/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/prompts/instruct.txt` & `agixt-1.2.3/agixt/prompts/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/prompts/starchat/instruct.txt` & `agixt-1.2.3/agixt/prompts/starchat/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/prompts/vicuna/instruct.txt` & `agixt-1.2.3/agixt/prompts/vicuna/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/provider/__init__.py` & `agixt-1.2.3/agixt/provider/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 import subprocess
 import pkg_resources
 import glob
 import os
 import inspect
 
 
+def get_providers():
+    providers = []
+    for provider in glob.glob("provider/*.py"):
+        if "__init__.py" not in provider:
+            providers.append(os.path.splitext(os.path.basename(provider))[0])
+    return providers
+
+
 def get_provider_options(provider_name):
     provider_name = provider_name.lower()
     module = importlib.import_module(f"provider.{provider_name}")
     provider_class = getattr(module, f"{provider_name.capitalize()}Provider")
     signature = inspect.signature(provider_class.__init__)
     options = {
         name: param.default if param.default is not inspect.Parameter.empty else None
```

### Comparing `agixt-1.2.1b0/agixt/provider/azure.py` & `agixt-1.2.3/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/provider/bing.py` & `agixt-1.2.3/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/provider/chatgpt.py` & `agixt-1.2.3/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/provider/claude.py` & `agixt-1.2.3/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/provider/fastchat.py` & `agixt-1.2.3/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/provider/gpt4all.py` & `agixt-1.2.3/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/provider/gpt4free.py` & `agixt-1.2.3/agixt/provider/gpt4free.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,16 +41,15 @@
                 self.FAILED_PROVIDERS = []
                 logging.info(
                     "All providers failed, sleeping for 10 seconds before trying again..."
                 )
                 time.sleep(10)
 
     async def instruct(self, prompt, tokens: int = 0):
-        final_response = None
-        while final_response is None:
+        while True:
             for provider in self.providers:
                 try:
                     if provider not in self.FAILED_PROVIDERS:
                         logging.info(f"[GPT4Free] Using: {provider}")
                         if provider not in self.account_tokens:
                             try:
                                 if provider == "Poe":
@@ -92,28 +91,14 @@
                                 ):
                                     response = None
                             if (
                                 response
                                 == "Unable to fetch the response, Please try again."
                             ):
                                 response = None
-                        if response:
-                            final_response = response
+                        if response and len(response) > 1:
+                            return response
                         else:
                             await self.provider_failure(provider)
-                    if final_response:
-                        if len(final_response) > 1:
-                            return final_response
-                    else:
-                        logging.info(f"Failed to use {provider}")
-                        self.FAILED_PROVIDERS.append(provider)
-                        if len(self.FAILED_PROVIDERS) == len(self.providers):
-                            self.FAILED_PROVIDERS = []
-                            logging.info(
-                                "All providers failed, sleeping for 10 seconds before trying again..."
-                            )
-                            time.sleep(10)
                 except Exception as e:
-                    await self.provider_failure(provider=provider)
-                    final_response = None
-
-            await self.provider_failure(provider=provider)
+                    logging.info(f"[GPT4Free] Exception: {e}")
+                    await self.provider_failure(provider)
```

### Comparing `agixt-1.2.1b0/agixt/provider/gpugpt4all.py` & `agixt-1.2.3/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/provider/huggingchat.py` & `agixt-1.2.3/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/provider/huggingface.py` & `agixt-1.2.3/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/provider/kobold.py` & `agixt-1.2.3/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/provider/llamacpp.py` & `agixt-1.2.3/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/provider/llamacppapi.py` & `agixt-1.2.3/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/provider/oobabooga.py` & `agixt-1.2.3/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/provider/openai.py` & `agixt-1.2.3/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/provider/palm.py` & `agixt-1.2.3/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/provider/runpod.py` & `agixt-1.2.3/agixt/provider/runpod.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/agixt/provider/transformer.py` & `agixt-1.2.3/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.1b0/docs/README.md` & `agixt-1.2.3/docs/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,14 @@
 - [AGiXT](#agixt)
   - [Table of Contents 📖](#table-of-contents-)
   - [⚠️ Disclaimers!](#️-disclaimers)
     - [Monitor Your Usage!](#monitor-your-usage)
     - [Under Development!](#under-development)
   - [Key Features 🗝️](#key-features-️)
   - [Quick Start Guide](#quick-start-guide)
-    - [Local Quick Start Guide](#local-quick-start-guide)
-    - [Docker Quick Start Guide](#docker-quick-start-guide)
-      - [Update Docker Containers](#update-docker-containers)
   - [Configuration](#configuration)
   - [Documentation](#documentation)
   - [Contributing](#contributing)
   - [Donations and Sponsorships](#donations-and-sponsorships)
   - [Our Team 🧑‍💻](#our-team-)
   - [History](#history)
 
@@ -56,51 +53,29 @@
 - **Audio-to-Text & Text-to-Speech Options**: Integration with Hugging Face for seamless audio-to-text transcription, and multiple TTS choices, featuring Brian TTS, Mac OS TTS, and ElevenLabs.
 - **Platform Interoperability & AI Agent Management**: Streamlined creation, renaming, deletion, and updating of AI agent settings along with easy interaction with popular platforms like Twitter, GitHub, Google, DALL-E, and more.
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
 ## Quick Start Guide
-You have two options for running AGiXT currently, you can either run it with Python locally or you can run it with Docker.
 
-### Local Quick Start Guide
 To get started quickly locally, you will need at least Python 3.10.6 installed.  If using Windows, we recommend installing [Windows Subsystem For Linux](https://learn.microsoft.com/en-us/windows/wsl/install) first.
 
 Open a terminal and run the following commands:
 
 ```
 git clone https://github.com/Josh-XT/AGiXT
 cd AGiXT
 ./AGiXT.sh
 ```
 
-Any time you want to run AGiXT after that, you can just run `./AGiXT.sh` from the AGiXT directory.  This will pull the latest changes from the main branch then launch AGiXT.
-
-You may have to press `Ctrl+C` multiple times to stop AGiXT running in the terminal due to it running multiple processes.
-
-- Access the web interface at http://localhost:8501
-- Access the AGiXT API documentation at http://localhost:7437
-
-### Docker Quick Start Guide
-To get started quickly with Docker, you will need at least Docker 24.0.2 installed. You can check your version by running `docker --version` in a terminal. You can install Docker by following the instructions [here](https://docs.docker.com/get-docker/).
-
-Open a terminal and run the following commands:
-```
-git clone https://github.com/Josh-XT/AGiXT
-cd AGiXT
-docker-compose up
-```
+Follow the prompts to install the required dependencies.  Any time you want to run AGiXT in the future, just run `./AGiXT.sh` again.
 
 - Access the web interface at http://localhost:8501
 - Access the AGiXT API documentation at http://localhost:7437
-#### Update Docker Containers
-
-```
-docker compose pull
-```
 
 ## Configuration
 
 Each AGiXT Agent has its own settings for interfacing with AI providers, and other configuration options. These settings can be set and modified through the web interface.
 ## Documentation
 
 Need more information? Check out the [documentation](https://josh-xt.github.io/AGiXT) for more details to get a better understanding of the concepts and features of AGiXT.
```

