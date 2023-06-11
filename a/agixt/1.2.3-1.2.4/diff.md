# Comparing `tmp/agixt-1.2.3.tar.gz` & `tmp/agixt-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.2.3.tar", last modified: Sun Jun 11 01:20:51 2023, max compression
+gzip compressed data, was "agixt-1.2.4.tar", last modified: Sun Jun 11 19:07:29 2023, max compression
```

## Comparing `agixt-1.2.3.tar` & `agixt-1.2.4.tar`

### file list

```diff
@@ -1,198 +1,199 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.767129 agixt-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-11 01:20:40.000000 agixt-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-11 01:20:40.000000 agixt-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-06-11 01:20:51.767129 agixt-1.2.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.735129 agixt-1.2.3/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/Extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19416 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/Interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/Prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.735129 agixt-1.2.3/agixt/WORKSPACE/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/WORKSPACE/example.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.727129 agixt-1.2.3/agixt/agents/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.735129 agixt-1.2.3/agixt/agents/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/agents/gpt4free/config.json
--rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.735129 agixt-1.2.3/agixt/chains/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/chains/Smart Chat.json
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/chains/Smart Instruct.json
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/chains/Task.json
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/chains/Test_Commands.json
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/chains/Write a Poem.json
--rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.739129 agixt-1.2.3/agixt/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/agixt_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/briantts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/dalle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/google.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/gtts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/macostts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/microsoft_365.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/searxng.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/sendgrid_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/extensions/web_playwright.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.747129 agixt-1.2.3/agixt/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Chat.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Create New Command.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Custom Input.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Get Task List.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Instruction.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Pick a Poem Subject.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Prioritize.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Score Response.txt
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Task Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Tell Me How.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Title a Poem.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Validation.txt
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/WebSearch.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Write a Haiku.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/Write a Poem.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.747129 agixt-1.2.3/agixt/prompts/gpt-3.5-turbo/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/gpt-3.5-turbo/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.747129 agixt-1.2.3/agixt/prompts/gpt-4/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.747129 agixt-1.2.3/agixt/prompts/starchat/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/starchat/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.747129 agixt-1.2.3/agixt/prompts/vicuna/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/prompts/vicuna/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.751129 agixt-1.2.3/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/llamacppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/runpod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 01:20:40.000000 agixt-1.2.3/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.735129 agixt-1.2.3/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-06-11 01:20:51.000000 agixt-1.2.3/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-11 01:20:51.000000 agixt-1.2.3/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 01:20:51.000000 agixt-1.2.3/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-11 01:20:51.000000 agixt-1.2.3/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 01:20:51.000000 agixt-1.2.3/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.751129 agixt-1.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.751129 agixt-1.2.3/docs/1-Getting started/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/1-Getting started/Quick Start.md
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/1-Getting started/Support.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.755129 agixt-1.2.3/docs/2-Concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/0-Core Concepts.md
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Agents.md
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Chains.md
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Chat.md
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Commands.md
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Instructions.md
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Prompts.md
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Providers.md
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Smart Chat.md
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Smart Instruct.md
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Smart Task.md
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/2-Concepts/Tasks.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.755129 agixt-1.2.3/docs/3-Providers/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/Anthropic Claude.md
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/Azure OpenAI.md
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/ChatGPT.md
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/FastChat.md
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/GPT4ALL-GPU.md
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/GPT4ALL.md
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/GPT4Free.md
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/Google Bard.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/Google Palm.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/Hugging Face Transformers.md
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/HuggingChat.md
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/Kobold.md
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/Microsoft Bing.md
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/Oobabooga Text Generation Web UI.md
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/OpenAI.md
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/llamacpp API.md
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/3-Providers/llamacpp.md
--rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.759129 agixt-1.2.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/AGiXT-gradient-flat.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/AGiXT-gradient-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/AGiXT.png
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/AGiXT.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1707562 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/AGiXT_Original_PSD.psd
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/AGiXTwhiteborder.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/Docker-desktop-win-setting-streamlit.png
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/Smart Instruct.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/Smart Instruct.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/Smart Tasks.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/Smart Tasks.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-11 01:20:40.000000 agixt-1.2.3/docs/images/Untitled Diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-11 01:20:40.000000 agixt-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-11 01:20:40.000000 agixt-1.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 01:20:51.767129 agixt-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-11 01:20:40.000000 agixt-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.763129 agixt-1.2.3/streamlit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.763129 agixt-1.2.3/streamlit/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/ApiClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/Main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.763129 agixt-1.2.3/streamlit/auth_libs/
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/auth_libs/Cfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/auth_libs/Redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/auth_libs/Users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.763129 agixt-1.2.3/streamlit/auth_libs/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/auth_libs/pages/Login.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/auth_libs/pages/Profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/auth_libs/pages/Register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.763129 agixt-1.2.3/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/components/agent_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/components/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/components/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/components/learning.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/components/verify_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.763129 agixt-1.2.3/streamlit/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/pages/0-Agent_Settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/pages/1-Prompt_Templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    16638 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/pages/2-Chain_Management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-11 01:20:40.000000 agixt-1.2.3/streamlit/pages/3-Interact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:20:51.763129 agixt-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-06-11 01:20:40.000000 agixt-1.2.3/tests/ApiClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-11 01:20:40.000000 agixt-1.2.3/tests/test-commands.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    52056 2023-06-11 01:20:40.000000 agixt-1.2.3/tests/tests.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.769282 agixt-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-11 19:07:16.000000 agixt-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-11 19:07:16.000000 agixt-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-06-11 19:07:29.769282 agixt-1.2.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.749283 agixt-1.2.4/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    15548 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/Extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/Interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/Prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.749283 agixt-1.2.4/agixt/WORKSPACE/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/WORKSPACE/example.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.745283 agixt-1.2.4/agixt/agents/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.749283 agixt-1.2.4/agixt/agents/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/agents/gpt4free/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.749283 agixt-1.2.4/agixt/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/chains/Smart Chat.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/chains/Smart Instruct.json
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/chains/Task.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/chains/Test_Commands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/chains/Write a Poem.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.753283 agixt-1.2.4/agixt/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/agixt_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/briantts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/dalle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/gtts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/macostts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/microsoft_365.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/searxng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/extensions/web_playwright.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.757283 agixt-1.2.4/agixt/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Chat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Create New Command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Custom Input.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Get Task List.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Instruction.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Pick a Poem Subject.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Prioritize.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Score Response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Task Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Title a Poem.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Validation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/WebSearch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Write a Haiku.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/Write a Poem.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.757283 agixt-1.2.4/agixt/prompts/gpt-3.5-turbo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/gpt-3.5-turbo/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.757283 agixt-1.2.4/agixt/prompts/gpt-4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.757283 agixt-1.2.4/agixt/prompts/starchat/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/starchat/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.757283 agixt-1.2.4/agixt/prompts/vicuna/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/prompts/vicuna/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.757283 agixt-1.2.4/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/llamacppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 19:07:16.000000 agixt-1.2.4/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.749283 agixt-1.2.4/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-06-11 19:07:29.000000 agixt-1.2.4/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-11 19:07:29.000000 agixt-1.2.4/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:07:29.000000 agixt-1.2.4/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-11 19:07:29.000000 agixt-1.2.4/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 19:07:29.000000 agixt-1.2.4/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.757283 agixt-1.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.757283 agixt-1.2.4/docs/1-Getting started/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/1-Getting started/Quick Start.md
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/1-Getting started/Support.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.761283 agixt-1.2.4/docs/2-Concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/0-Core Concepts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Agents.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Chains.md
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Commands.md
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Instructions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Prompts.md
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Providers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Smart Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Smart Instruct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Smart Task.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/2-Concepts/Tasks.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.761283 agixt-1.2.4/docs/3-Providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/Anthropic Claude.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/Azure OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/ChatGPT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/FastChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/GPT4ALL-GPU.md
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/GPT4ALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/GPT4Free.md
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/Google Bard.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/Google Palm.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/Hugging Face Transformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/HuggingChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/Kobold.md
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/Microsoft Bing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/Oobabooga Text Generation Web UI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/llamacpp API.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/3-Providers/llamacpp.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.765282 agixt-1.2.4/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/AGiXT-gradient-flat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/AGiXT-gradient-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/AGiXT.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/AGiXT.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1707562 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/AGiXT_Original_PSD.psd
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/AGiXTwhiteborder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/Docker-desktop-win-setting-streamlit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/Smart Instruct.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/Smart Instruct.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/Smart Tasks.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/Smart Tasks.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-11 19:07:16.000000 agixt-1.2.4/docs/images/Untitled Diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-11 19:07:16.000000 agixt-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-11 19:07:16.000000 agixt-1.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 19:07:29.769282 agixt-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-11 19:07:16.000000 agixt-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.765282 agixt-1.2.4/streamlit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.765282 agixt-1.2.4/streamlit/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/ApiClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/Main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.765282 agixt-1.2.4/streamlit/auth_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/auth_libs/Cfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/auth_libs/Redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/auth_libs/Users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.765282 agixt-1.2.4/streamlit/auth_libs/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/auth_libs/pages/Login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/auth_libs/pages/Profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/auth_libs/pages/Register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.769282 agixt-1.2.4/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/components/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/components/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/components/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/components/learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/components/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/components/verify_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.769282 agixt-1.2.4/streamlit/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/pages/0-Agent_Settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/pages/1-Prompt_Templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/pages/2-Chain_Management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-06-11 19:07:16.000000 agixt-1.2.4/streamlit/pages/3-Interact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:29.769282 agixt-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-11 19:07:16.000000 agixt-1.2.4/tests/ApiClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-11 19:07:16.000000 agixt-1.2.4/tests/test-commands.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    54844 2023-06-11 19:07:16.000000 agixt-1.2.4/tests/tests.ipynb
```

### Comparing `agixt-1.2.3/LICENSE` & `agixt-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/PKG-INFO` & `agixt-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.2.3
+Version: 1.2.4
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.2.3/agixt/Agent.py` & `agixt-1.2.4/agixt/Agent.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,68 +17,80 @@
     "AI_MODEL": "gpt-4",
     "AI_TEMPERATURE": "0.7",
     "MAX_TOKENS": "4000",
     "embedder": "default",
 }
 
 
+def get_agent_file_paths(agent_name):
+    base_path = os.path.join(os.getcwd(), "agents")
+    folder_path = os.path.normpath(os.path.join(base_path, agent_name))
+    config_path = os.path.normpath(os.path.join(base_path, "config.json"))
+    history_path = os.path.normpath(os.path.join(base_path, "history.yaml"))
+    if not config_path.startswith(base_path) or not folder_path.startswith(base_path):
+        raise ValueError("Invalid path, agent name must not contain slashes.")
+    if not os.path.exists(folder_path):
+        os.mkdir(folder_path)
+    return config_path, history_path, folder_path
+
+
 def add_agent(agent_name, provider_settings=None):
     if not agent_name:
         return "Agent name cannot be empty."
     provider_settings = (
         DEFAULT_SETTINGS
         if not provider_settings or provider_settings == {}
         else provider_settings
     )
-    agent_folder = os.path.join("agents", agent_name)
-    if not os.path.exists("agents"):
-        os.makedirs("agents")
-    if not os.path.exists(agent_folder):
-        os.makedirs(agent_folder)
-    agent_dir = os.path.join("agents", agent_name)
-    agent_config_file = os.path.join(agent_dir, "config.json")
+    config_path, history_path, folder_path = get_agent_file_paths(agent_name=agent_name)
     if provider_settings is None or provider_settings == "" or provider_settings == {}:
         provider_settings = DEFAULT_SETTINGS
     settings = json.dumps(
         {
             "commands": {},
             "settings": provider_settings,
         }
     )
     # Write the settings to the agent config file
-    with open(agent_config_file, "w") as f:
+    with open(config_path, "w") as f:
         f.write(settings)
-    with open(os.path.join("agents", agent_name, "history.yaml"), "w") as f:
+    with open(history_path, "w") as f:
         f.write("")
-    return {"agent_file": f"{agent_name}/history.yaml"}
+    return {"message": f"Agent {agent_name} created."}
 
 
 def delete_agent(agent_name):
+    config_path, history_path, folder_path = get_agent_file_paths(agent_name=agent_name)
     try:
-        agent_folder = os.path.join("agents", agent_name)
-        if os.path.exists(agent_folder):
-            shutil.rmtree(agent_folder)
+        if os.path.exists(folder_path):
+            shutil.rmtree(folder_path)
         return {"message": f"Agent {agent_name} deleted."}, 200
     except:
         return {"message": f"Agent {agent_name} could not be deleted."}, 400
 
 
 def rename_agent(agent_name, new_name):
-    current_agent_folder = os.path.join("agents", agent_name)
-    new_agent_folder = os.path.join("agents", new_name)
-    if os.path.exists(current_agent_folder):
+    config_path, history_path, folder_path = get_agent_file_paths(agent_name=agent_name)
+    base_path = os.path.join(os.getcwd(), "agents")
+    new_agent_folder = os.path.normpath(os.path.join(base_path, new_name))
+    if not new_agent_folder.startswith(base_path):
+        raise ValueError("Invalid path, agent name must not contain slashes.")
+
+    if os.path.exists(folder_path):
         # Check if the new name is already taken
         if os.path.exists(new_agent_folder):
             # Add a number to the end of the new name
             i = 1
-            while os.path.exists(f"agents/{new_name}_{i}"):
+            while os.path.exists(new_agent_folder):
                 i += 1
-            new_name = f"{new_name}_{i}"
-            new_agent_folder = os.path.join("agents", new_name)
-        os.rename(current_agent_folder, new_agent_folder)
+                new_name = f"{new_name}_{i}"
+                new_agent_folder = os.path.normpath(os.path.join(base_path, new_name))
+            if not new_agent_folder.startswith(base_path):
+                raise ValueError("Invalid path, agent name must not contain slashes.")
+        os.rename(folder_path, new_agent_folder)
         return {"message": f"Agent {agent_name} renamed to {new_name}."}, 200
 
 
 def get_agents():
     agents_dir = "agents"
     if not os.path.exists(agents_dir):
         os.makedirs(agents_dir)
@@ -93,14 +105,17 @@
             output.append({"name": agent, "status": False})
     return output
 
 
 class Agent:
     def __init__(self, agent_name=None):
         self.agent_name = agent_name if agent_name is not None else "AGiXT"
+        self.config_path, self.history_file, self.folder_path = get_agent_file_paths(
+            agent_name=agent_name
+        )
         self.AGENT_CONFIG = self.get_agent_config()
         if "settings" in self.AGENT_CONFIG:
             self.PROVIDER_SETTINGS = self.AGENT_CONFIG["settings"]
             if "provider" in self.PROVIDER_SETTINGS:
                 self.AI_PROVIDER = self.PROVIDER_SETTINGS["provider"]
                 self.PROVIDER = Provider(self.AI_PROVIDER, **self.PROVIDER_SETTINGS)
                 self._load_agent_config_keys(
@@ -128,24 +143,24 @@
             else:
                 self.LOG_REQUESTS = True
             self.commands = self.load_commands()
             self.available_commands = Extensions(
                 agent_config=self.AGENT_CONFIG
             ).get_available_commands()
             self.clean_agent_config_commands()
-            self.history_file = os.path.join("agents", self.agent_name, "history.yaml")
             self.history = self.load_history()
             self.agent_instances = {}
             self.agent_config = self.load_agent_config()
             if self.LOG_REQUESTS:
                 Path(
-                    os.path.join(
-                        "agents",
-                        self.agent_name,
-                        "requests",
+                    os.path.normpath(
+                        os.path.join(
+                            self.folder_path,
+                            "requests",
+                        )
                     )
                 ).mkdir(parents=True, exist_ok=True)
 
     def get_memories(self):
         return Memories(self.agent_name, self.AGENT_CONFIG)
 
     async def execute(self, command_name, command_args):
@@ -178,15 +193,15 @@
         for command in self.commands:
             friendly_name = command[0]
             if friendly_name not in self.AGENT_CONFIG["commands"]:
                 self.AGENT_CONFIG["commands"][friendly_name] = False
         for command in list(self.AGENT_CONFIG["commands"]):
             if command not in [cmd[0] for cmd in self.commands]:
                 del self.AGENT_CONFIG["commands"][command]
-        with open(os.path.join("agents", self.agent_name, "config.json"), "w") as f:
+        with open(self.config_path, "w") as f:
             json.dump(self.AGENT_CONFIG, f)
 
     def get_commands_string(self):
         if len(self.available_commands) == 0:
             return None
 
         enabled_commands = filter(
@@ -247,44 +262,39 @@
         )
 
         # Check and create agent directory if it doesn't exist
         if not os.path.exists(os.path.join("agents", self.agent_name)):
             os.makedirs(os.path.join("agents", self.agent_name))
 
         # Write the settings to the agent config file
-        with open(os.path.join("agents", self.agent_name, "config.json"), "w") as f:
+        with open(self.config_path, "w") as f:
             f.write(settings)
 
-        return os.path.join("agents", self.agent_name, "config.json")
+        return self.config_path
 
     def load_agent_config(self):
         try:
-            with open(
-                os.path.join("agents", self.agent_name, "config.json")
-            ) as agent_config:
+            with open(self.config_path) as agent_config:
                 try:
                     agent_config_data = json.load(agent_config)
                     return agent_config_data
                 except json.JSONDecodeError:
                     agent_config_data = {}
                     # Populate the agent_config with all commands enabled
                     agent_config_data["commands"] = {
                         command_name: "false"
                         for command_name, _, _ in self.load_commands(self.agent_name)
                     }
                     agent_config_data["settings"] = DEFAULT_SETTINGS
                     # Save the updated agent_config to the file
-                    with open(
-                        os.path.join("agents", self.agent_name, "config.json"), "w"
-                    ) as agent_config_file:
+                    with open(self.config_path, "w") as agent_config_file:
                         json.dump(agent_config_data, agent_config_file)
                     return agent_config_data
         except:
-            # Add all commands to agent/{agent_name}/config.json in this format {"command_name": "false"}
-            with open(os.path.join("agents", self.agent_name, "config.json"), "w") as f:
+            with open(self.config_path, "w") as f:
                 f.write(
                     json.dumps(
                         {
                             "commands": {
                                 command_name: "false"
                                 for command_name, _, _ in self.load_commands()
                             },
@@ -292,42 +302,40 @@
                         }
                     )
                 )
         return agent_config_data
 
     def get_agent_config(self):
         while True:
-            if os.path.exists(os.path.join("agents", self.agent_name, "config.json")):
+            if os.path.exists(self.config_path):
                 try:
-                    with open(
-                        os.path.join("agents", self.agent_name, "config.json"), "r"
-                    ) as f:
+                    with open(self.config_path, "r") as f:
                         file_content = f.read().strip()
                         if file_content:
                             return json.loads(file_content)
                 except:
                     None
             add_agent(agent_name=self.agent_name)
             return self.get_agent_config()
 
     def update_agent_config(self, new_config, config_key):
-        if os.path.exists(os.path.join("agents", self.agent_name, "config.json")):
-            with open(os.path.join("agents", self.agent_name, "config.json"), "r") as f:
+        if os.path.exists(self.config_path):
+            with open(self.config_path, "r") as f:
                 current_config = json.load(f)
 
             # Ensure the config_key is present in the current configuration
             if config_key not in current_config:
                 current_config[config_key] = {}
 
             # Update the specified key with new_config while preserving other keys and values
             for key, value in new_config.items():
                 current_config[config_key][key] = value
 
             # Save the updated configuration back to the file
-            with open(os.path.join("agents", self.agent_name, "config.json"), "w") as f:
+            with open(self.config_path, "w") as f:
                 json.dump(current_config, f)
             return f"Agent {self.agent_name} configuration updated."
         else:
             return f"Agent {self.agent_name} configuration not found."
 
     def get_history(self):
         if not os.path.exists(self.history_file):
@@ -343,16 +351,20 @@
                 message = interaction["timestamp"] + "\n" + interaction["message"]
                 history.append({role: message})
             return history
         except:
             return []
 
     def wipe_agent_memories(self):
-        agent_folder = os.path.join("agents", self.agent_name)
-        memories_folder = os.path.join(agent_folder, "memories")
+        memories_folder = os.path.normpath(
+            os.path.join(os.getcwd(), self.agent_name, "memories")
+        )
+        if not memories_folder.startswith(os.getcwd()):
+            raise ValueError("Invalid path, agent name must not contain slashes.")
+
         if os.path.exists(memories_folder):
             shutil.rmtree(memories_folder)
 
     def load_history(self):
         if os.path.exists(self.history_file):
             with open(self.history_file, "r") as file:
                 memory = yaml.safe_load(file)
@@ -381,7 +393,19 @@
     def delete_history(self):
         try:
             self.history = {"interactions": []}
             self.save_history()
             return "History deleted."
         except:
             return "History not found."
+
+    def delete_history_message(self, message: str):
+        try:
+            self.history["interactions"] = [
+                interaction
+                for interaction in self.history["interactions"]
+                if interaction["message"] != message
+            ]
+            self.save_history()
+            return "Message deleted."
+        except:
+            return "Message not found."
```

### Comparing `agixt-1.2.3/agixt/Chain.py` & `agixt-1.2.4/agixt/Chain.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,91 +3,116 @@
 from Interactions import Interactions
 import argparse
 from Extensions import Extensions
 import logging
 from datetime import datetime
 
 
+def get_chain_file_path(chain_name):
+    base_path = os.path.join(os.getcwd(), "chains")
+    folder_path = os.path.normpath(os.path.join(base_path, chain_name))
+    file_path = os.path.normpath(os.path.join(base_path, f"{chain_name}.json"))
+    if not file_path.startswith(base_path) or not folder_path.startswith(base_path):
+        raise ValueError("Invalid path, chain name must not contain slashes.")
+    if not os.path.exists(folder_path):
+        os.mkdir(folder_path)
+    return file_path
+
+
+def get_chain_responses_file_path(chain_name):
+    base_path = os.path.join(os.getcwd(), "chains")
+    file_path = os.path.normpath(os.path.join(base_path, chain_name, "responses.json"))
+    if not file_path.startswith(base_path):
+        raise ValueError("Invalid path, chain name must not contain slashes.")
+    return file_path
+
+
 class Chain:
     def get_chain(self, chain_name):
-        # if chain/{chain_name}/ exists and create the folder if it does not
-        if not os.path.exists(os.path.join("chains", chain_name)):
-            os.mkdir(os.path.join("chains", chain_name))
-        with open(os.path.join("chains", f"{chain_name}.json"), "r") as f:
+        file_path = get_chain_file_path(chain_name=chain_name)
+        with open(file_path, "r") as f:
             chain_data = json.load(f)
         return chain_data
 
     def get_chains(self):
         chains = [
             f.replace(".json", "") for f in os.listdir("chains") if f.endswith(".json")
         ]
         return chains
 
     def add_chain(self, chain_name):
+        file_path = get_chain_file_path(chain_name=chain_name)
         chain_data = {"chain_name": chain_name, "steps": []}
-        with open(os.path.join("chains", f"{chain_name}.json"), "w") as f:
+        with open(file_path, "w") as f:
             json.dump(chain_data, f)
 
     def rename_chain(self, chain_name, new_name):
+        file_path = get_chain_file_path(chain_name=chain_name)
+        new_file_path = get_chain_file_path(chain_name=new_name)
         os.rename(
-            os.path.join("chains", f"{chain_name}.json"),
-            os.path.join("chains", f"{new_name}.json"),
+            os.path.join(file_path),
+            os.path.join(new_file_path),
         )
         chain_data = self.get_chain(chain_name=new_name)
         chain_data["chain_name"] = new_name
-        with open(os.path.join("chains", f"{new_name}.json"), "w") as f:
+        with open(new_file_path, "w") as f:
             json.dump(chain_data, f)
 
     def add_chain_step(self, chain_name, step_number, agent_name, prompt_type, prompt):
+        file_path = get_chain_file_path(chain_name=chain_name)
         chain_data = self.get_chain(chain_name=chain_name)
         chain_data["steps"].append(
             {
                 "step": step_number,
                 "agent_name": agent_name,
                 "prompt_type": prompt_type,
                 "prompt": prompt,
             }
         )
-        with open(os.path.join("chains", f"{chain_name}.json"), "w") as f:
+        with open(file_path, "w") as f:
             json.dump(chain_data, f)
 
     def update_step(self, chain_name, step_number, agent_name, prompt_type, prompt):
+        file_path = get_chain_file_path(chain_name=chain_name)
         chain_data = self.get_chain(chain_name=chain_name)
         for step in chain_data["steps"]:
             if step["step"] == step_number:
                 step["agent_name"] = agent_name
                 step["prompt_type"] = prompt_type
                 step["prompt"] = prompt
                 break
-        with open(os.path.join("chains", f"{chain_name}.json"), "w") as f:
+        with open(file_path, "w") as f:
             json.dump(chain_data, f)
 
     def delete_step(self, chain_name, step_number):
+        file_path = get_chain_file_path(chain_name=chain_name)
         chain_data = self.get_chain(chain_name=chain_name)
         chain_data["steps"] = [
             step for step in chain_data["steps"] if step["step"] != step_number
         ]
-        with open(os.path.join("chains", f"{chain_name}.json"), "w") as f:
+        with open(file_path, "w") as f:
             json.dump(chain_data, f)
 
     def delete_chain(self, chain_name):
-        os.remove(os.path.join("chains", f"{chain_name}.json"))
+        file_path = get_chain_file_path(chain_name=chain_name)
+        os.remove(file_path)
 
     def get_step(self, chain_name, step_number):
         chain_data = self.get_chain(chain_name=chain_name)
         for step in chain_data["steps"]:
             if step["step"] == step_number:
                 return step
         return None
 
     def get_steps(self, chain_name):
         chain_data = self.get_chain(chain_name=chain_name)
         return chain_data["steps"]
 
     def move_step(self, chain_name, current_step_number, new_step_number):
+        file_path = get_chain_file_path(chain_name=chain_name)
         chain_data = self.get_chain(chain_name=chain_name)
         if not 1 <= new_step_number <= len(
             chain_data["steps"]
         ) or current_step_number not in [step["step"] for step in chain_data["steps"]]:
             print(f"Error: Invalid step numbers.")
             return
         moved_step = None
@@ -102,18 +127,19 @@
                     step["step"] += 1
             else:
                 if current_step_number < step["step"] <= new_step_number:
                     step["step"] -= 1
         moved_step["step"] = new_step_number
         chain_data["steps"].append(moved_step)
         chain_data["steps"] = sorted(chain_data["steps"], key=lambda x: x["step"])
-        with open(os.path.join("chains", f"{chain_name}.json"), "w") as f:
+        with open(file_path, "w") as f:
             json.dump(chain_data, f)
 
     async def run_chain(self, chain_name, user_input=None):
+        file_path = get_chain_responses_file_path(chain_name=chain_name)
         chain_data = self.get_chain(chain_name=chain_name)
         logging.info(f"Running chain '{chain_name}'")
         responses = {}  # Create a dictionary to hold responses.
         for step_data in chain_data["steps"]:
             if "prompt" in step_data and "step" in step_data:
                 logging.info(f"Running step {step_data['step']}")
                 step = {}
@@ -124,35 +150,35 @@
                 step["agent_name"] = step_data["agent_name"]
                 step["prompt"] = step_data["prompt"]
                 step["prompt_type"] = step_data["prompt_type"]
                 responses[step_data["step"]] = step  # Store the response.
                 logging.info(f"Response: {step_response}")
                 # Write the responses to the json file.
                 dt = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-                with open(
-                    os.path.join("chains", chain_name, "responses.json"), "w"
-                ) as f:
+                with open(file_path, "w") as f:
                     json.dump(responses, f)
         return responses
 
     def get_step_response(self, chain_name, step_number="all"):
+        file_path = get_chain_responses_file_path(chain_name=chain_name)
         try:
-            with open(os.path.join("chains", chain_name, "responses.json"), "r") as f:
+            with open(file_path, "r") as f:
                 responses = json.load(f)
             print(responses)
             if step_number == "all":
                 return responses
             else:
                 return responses.get(str(step_number))
         except:
             return ""
 
     def get_chain_responses(self, chain_name):
+        file_path = get_chain_responses_file_path(chain_name=chain_name)
         try:
-            with open(os.path.join("chains", chain_name, "responses.json"), "r") as f:
+            with open(file_path, "r") as f:
                 responses = json.load(f)
             return responses
         except:
             return {}
 
     def get_step_content(self, chain_name, prompt_content, user_input, agent_name):
         new_prompt_content = {}
```

### Comparing `agixt-1.2.3/agixt/Embedding.py` & `agixt-1.2.4/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/Extensions.py` & `agixt-1.2.4/agixt/Extensions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/Interactions.py` & `agixt-1.2.4/agixt/Interactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,16 +45,22 @@
                 return str(value)
 
         pattern = r"(?<!{){([^{}\n]+)}(?!})"
         result = re.sub(pattern, replace, string)
         return result
 
     def get_step_response(self, chain_name, step_number):
+        base_path = os.path.join(os.getcwd(), "chains")
+        file_path = os.path.normpath(
+            os.path.join(base_path, chain_name, "responses.json")
+        )
+        if not file_path.startswith(base_path):
+            raise ValueError("Invalid path, chain name must not contain slashes.")
         try:
-            with open(os.path.join("chains", f"{chain_name}_responses.json"), "r") as f:
+            with open(file_path, "r") as f:
                 responses = json.load(f)
             return responses.get(str(step_number))
         except:
             return ""
 
     def get_step_content(self, chain_name, step_number, prompt_content):
         new_prompt_content = {}
```

### Comparing `agixt-1.2.3/agixt/Memories.py` & `agixt-1.2.4/agixt/Memories.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,14 +193,18 @@
             content_chunks.append((self.score_chunk(chunk_text, keywords), chunk_text))
 
         # Sort the chunks by their score in descending order before returning them
         content_chunks.sort(key=lambda x: x[0], reverse=True)
         return [chunk_text for score, chunk_text in content_chunks]
 
     async def mem_read_file(self, file_path: str):
+        base_path = os.path.join(os.getcwd(), "WORKSPACE")
+        file_path = os.path.normpath(os.path.join(base_path, file_path))
+        if not file_path.startswith(base_path):
+            raise Exception("Path given not allowed")
         try:
             # If file extension is pdf, convert to text
             if file_path.endswith(".pdf"):
                 with pdfplumber.open(file_path) as pdf:
                     content = "\n".join([page.extract_text() for page in pdf.pages])
             # If file extension is xls, convert to csv
             elif file_path.endswith(".xls") or file_path.endswith(".xlsx"):
```

### Comparing `agixt-1.2.3/agixt/Prompts.py` & `agixt-1.2.4/agixt/Prompts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,78 @@
 import os
 
 
+def get_prompt_file_path(prompt_name, model="default"):
+    base_path = os.path.join(os.getcwd(), "prompts")
+    base_model_path = os.path.normpath(os.path.join(os.getcwd(), "prompts", model))
+    model_prompt_file = os.path.normpath(
+        os.path.join(base_model_path, f"{prompt_name}.txt")
+    )
+    default_prompt_file = os.path.normpath(
+        os.path.join(base_path, f"{prompt_name}.txt")
+    )
+    if (
+        not base_model_path.startswith(base_path)
+        or not model_prompt_file.startswith(base_model_path)
+        or not default_prompt_file.startswith(base_path)
+    ):
+        print(base_model_path)
+        print(model_prompt_file)
+        print(default_prompt_file)
+        raise ValueError(
+            "Invalid file path. Prompt name cannot contain '/', '\\' or '..' in"
+        )
+    if not os.path.exists(base_path):
+        os.mkdir(base_path)
+    if not os.path.exists(base_model_path):
+        os.mkdir(base_model_path)
+    prompt_file = (
+        model_prompt_file if os.path.isfile(model_prompt_file) else default_prompt_file
+    )
+    return prompt_file
+
+
 class Prompts:
     def add_prompt(self, prompt_name, prompt):
         # if prompts folder does not exist, create it
-        if not os.path.exists("prompts"):
-            os.mkdir("prompts")
+        file_path = get_prompt_file_path(prompt_name=prompt_name)
         # if prompt file does not exist, create it
-        if not os.path.exists(os.path.join("prompts", f"{prompt_name}.txt")):
-            with open(os.path.join("prompts", f"{prompt_name}.txt"), "w") as f:
+        if not os.path.exists(file_path):
+            with open(file_path, "w") as f:
                 f.write(prompt)
 
     def get_prompt(self, prompt_name, model="default"):
-        model_prompt_file = os.path.join("prompts", f"{model}", f"{prompt_name}.txt")
-        default_prompt_file = os.path.join("prompts", f"{prompt_name}.txt")
-
-        prompt_file = (
-            model_prompt_file
-            if os.path.isfile(model_prompt_file)
-            else default_prompt_file
-        )
+        prompt_file = get_prompt_file_path(prompt_name=prompt_name, model=model)
         with open(prompt_file, "r") as f:
             prompt = f.read()
             return prompt
 
     def get_prompts(self):
         # Get all files in prompts folder that end in .txt and replace .txt with empty string
         prompts = []
         for file in os.listdir("prompts"):
             if file.endswith(".txt"):
                 prompts.append(file.replace(".txt", ""))
         return prompts
 
     def get_prompt_args(self, prompt_name):
-        prompt = self.get_prompt(prompt_name)
+        prompt = self.get_prompt(prompt_name=prompt_name)
         # Find anything in the file between { and } and add them to a list to return
         prompt_vars = []
         for word in prompt.split():
             if word.startswith("{") and word.endswith("}"):
                 prompt_vars.append(word[1:-1])
         return prompt_vars
 
     def delete_prompt(self, prompt_name):
-        os.remove(os.path.join("prompts", f"{prompt_name}.txt"))
+        prompt_file = get_prompt_file_path(prompt_name=prompt_name)
+        os.remove(prompt_file)
 
     def update_prompt(self, prompt_name, prompt):
-        with open(os.path.join("prompts", f"{prompt_name}.txt"), "w") as f:
+        prompt_file = get_prompt_file_path(prompt_name=prompt_name)
+        with open(prompt_file, "w") as f:
             f.write(prompt)
 
     def get_model_prompt(self, prompt_name, model="default"):
-        with open(f"prompts/{model}/{prompt_name}.txt", "r") as f:
+        prompt_file = get_prompt_file_path(prompt_name=prompt_name, model=model)
+        with open(prompt_file, "r") as f:
             return f.read()
```

### Comparing `agixt-1.2.3/agixt/app.py` & `agixt-1.2.4/agixt/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,18 @@
         new_config=settings.settings, config_key="settings"
     )
     return ResponseMessage(message=update_config)
 
 
 @app.post("/api/agent/{agent_name}/learn/file", tags=["Agent"])
 async def learn_file(agent_name: str, file: FileInput) -> ResponseMessage:
-    file_path = os.path.join(os.getcwd(), file.file_name)
+    base_path = os.path.join(os.getcwd(), "WORKSPACE")
+    file_path = os.path.normpath(os.path.join(base_path, file.file_name))
+    if not file_path.startswith(base_path):
+        raise Exception("Path given not allowed")
     with open(file_path, "w") as f:
         f.write(file.file_content)
     try:
         memories = Agent(agent_name=agent_name).get_memories()
         await memories.mem_read_file(file_path=file.file_content)
         try:
             os.remove(file_path)
@@ -249,14 +252,22 @@
 
 @app.delete("/api/agent/{agent_name}/history", tags=["Agent"])
 async def delete_history(agent_name: str) -> ResponseMessage:
     Agent(agent_name=agent_name).delete_history()
     return ResponseMessage(message=f"History for agent {agent_name} deleted.")
 
 
+@app.delete("/api/agent/{agent_name}/history/message", tags=["Agent"])
+async def delete_history_message(
+    agent_name: str, message: ResponseMessage
+) -> ResponseMessage:
+    Agent(agent_name=agent_name).delete_history_message(message.message)
+    return ResponseMessage(message=f"Message deleted.")
+
+
 @app.delete("/api/agent/{agent_name}/memory", tags=["Agent"])
 async def wipe_agent_memories(agent_name: str) -> ResponseMessage:
     Agent(agent_name=agent_name).wipe_agent_memories()
     return ResponseMessage(message=f"Memories for agent {agent_name} deleted.")
 
 
 @app.post("/api/agent/{agent_name}/instruct", tags=["Agent"])
@@ -451,19 +462,19 @@
         return ResponseMessage(message=f"Prompt '{prompt.prompt_name}' added.")
     except Exception as e:
         raise HTTPException(status_code=400, detail=str(e))
 
 
 @app.get("/api/prompt/{prompt_name}", tags=["Prompt"], response_model=CustomPromptModel)
 async def get_prompt(prompt_name: str):
-    try:
-        prompt_content = Prompts().get_prompt(prompt_name=prompt_name)
-        return {"prompt_name": prompt_name, "prompt": prompt_content}
-    except Exception as e:
-        raise HTTPException(status_code=404, detail=str(e))
+    # try:
+    prompt_content = Prompts().get_prompt(prompt_name=prompt_name)
+    return {"prompt_name": prompt_name, "prompt": prompt_content}
+    # except Exception as e:
+    #    raise HTTPException(status_code=404, detail=str(e))
 
 
 @app.get("/api/prompt", response_model=PromptList, tags=["Prompt"])
 async def get_prompts():
     prompts = Prompts().get_prompts()
     return {"prompts": prompts}
```

### Comparing `agixt-1.2.3/agixt/chains/Smart Chat.json` & `agixt-1.2.4/agixt/chains/Smart Chat.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994212962962963%*

 * *Differences: {"'steps'": "{0: {'prompt': {'command_name': 'Prompt AI Agent'}}}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "chain_name": "Smart Chat",
     "steps": [
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "agent": "{agent_name}",
-                "command_name": "prompt_agent",
+                "command_name": "Prompt AI Agent",
                 "context_results": 5,
                 "prompt_args": {},
                 "prompt_name": "SmartChat-StepByStep",
                 "shots": 3,
                 "user_input": "{user_input}",
                 "websearch": true,
                 "websearch_depth": 3
```

### Comparing `agixt-1.2.3/agixt/chains/Smart Instruct.json` & `agixt-1.2.4/agixt/chains/Smart Instruct.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994212962962963%*

 * *Differences: {"'steps'": "{0: {'prompt': {'command_name': 'Prompt AI Agent'}}}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "chain_name": "Smart Instruct",
     "steps": [
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "agent": "{agent_name}",
-                "command_name": "prompt_agent",
+                "command_name": "Prompt AI Agent",
                 "context_results": 5,
                 "prompt_args": {},
                 "prompt_name": "SmartInstruct-StepByStep",
                 "shots": 3,
                 "user_input": "{user_input}",
                 "websearch": true,
                 "websearch_depth": 3
```

### Comparing `agixt-1.2.3/agixt/chains/Task.json` & `agixt-1.2.4/agixt/chains/Task.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/chains/Test_Commands.json` & `agixt-1.2.4/agixt/chains/Test_Commands.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/chains/Write a Poem.json` & `agixt-1.2.4/agixt/chains/Write a Poem.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/example.ipynb` & `agixt-1.2.4/agixt/example.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/extensions/agixt_agent.py` & `agixt-1.2.4/agixt/extensions/agixt_agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/extensions/briantts.py` & `agixt-1.2.4/agixt/extensions/briantts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/extensions/dalle.py` & `agixt-1.2.4/agixt/extensions/dalle.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/extensions/discord.py` & `agixt-1.2.4/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/extensions/elevenlabs.py` & `agixt-1.2.4/agixt/extensions/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/extensions/file_system.py` & `agixt-1.2.4/agixt/extensions/file_system.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/extensions/github.py` & `agixt-1.2.4/agixt/extensions/github.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/extensions/google.py` & `agixt-1.2.4/agixt/extensions/google.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/extensions/gtts.py` & `agixt-1.2.4/agixt/extensions/gtts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/extensions/huggingface.py` & `agixt-1.2.4/agixt/extensions/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/extensions/macostts.py` & `agixt-1.2.4/agixt/extensions/macostts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/extensions/microsoft_365.py` & `agixt-1.2.4/agixt/extensions/microsoft_365.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/extensions/searxng.py` & `agixt-1.2.4/agixt/extensions/searxng.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/extensions/sendgrid_email.py` & `agixt-1.2.4/agixt/extensions/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/extensions/twitter.py` & `agixt-1.2.4/agixt/extensions/twitter.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/extensions/web_playwright.py` & `agixt-1.2.4/agixt/extensions/web_playwright.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/prompts/Create New Command.txt` & `agixt-1.2.4/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/prompts/Execution.txt` & `agixt-1.2.4/agixt/prompts/Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/prompts/Instruction.txt` & `agixt-1.2.4/agixt/prompts/Instruction.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.2.4/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.2.4/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/prompts/Task Execution.txt` & `agixt-1.2.4/agixt/prompts/Task Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/prompts/ValidationFailed.txt` & `agixt-1.2.4/agixt/prompts/ValidationFailed.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.2.4/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.2.4/agixt/prompts/gpt-4/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/prompts/instruct.txt` & `agixt-1.2.4/agixt/prompts/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/prompts/starchat/instruct.txt` & `agixt-1.2.4/agixt/prompts/starchat/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/prompts/vicuna/instruct.txt` & `agixt-1.2.4/agixt/prompts/vicuna/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/__init__.py` & `agixt-1.2.4/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/azure.py` & `agixt-1.2.4/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/bing.py` & `agixt-1.2.4/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/chatgpt.py` & `agixt-1.2.4/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/claude.py` & `agixt-1.2.4/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/fastchat.py` & `agixt-1.2.4/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/gpt4all.py` & `agixt-1.2.4/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/gpt4free.py` & `agixt-1.2.4/agixt/provider/gpt4free.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,23 @@
         **kwargs,
     ):
         self.requirements = ["gpt4free"]
         self.AI_MODEL = AI_MODEL
         self.AI_TEMPERATURE = AI_TEMPERATURE
         self.MAX_TOKENS = MAX_TOKENS
         self.FAILED_PROVIDERS = []
-        self.providers = ["DeepAI", "You", "UseLess", "ForeFront", "Theb", "Poe"]
+        self.providers = [
+            "DeepAI",
+            "You",
+            "UseLess",
+            "ForeFront",
+            "Theb",
+            "Poe",
+            "AiColors",
+        ]
         self.account_tokens = {}
 
     def create_account(self, provider, module):
         try:
             # the following call will not terminate the program even if it calls quit()
             return module.Account.create()
         except SystemExit:
```

### Comparing `agixt-1.2.3/agixt/provider/gpugpt4all.py` & `agixt-1.2.4/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/huggingchat.py` & `agixt-1.2.4/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/huggingface.py` & `agixt-1.2.4/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/kobold.py` & `agixt-1.2.4/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/llamacpp.py` & `agixt-1.2.4/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/llamacppapi.py` & `agixt-1.2.4/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/oobabooga.py` & `agixt-1.2.4/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/openai.py` & `agixt-1.2.4/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/palm.py` & `agixt-1.2.4/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/runpod.py` & `agixt-1.2.4/agixt/provider/runpod.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt/provider/transformer.py` & `agixt-1.2.4/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/agixt.egg-info/PKG-INFO` & `agixt-1.2.4/agixt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.2.3
+Version: 1.2.4
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.2.3/agixt.egg-info/SOURCES.txt` & `agixt-1.2.4/agixt.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -152,18 +152,19 @@
 streamlit/.streamlit/config.toml
 streamlit/auth_libs/Cfig.py
 streamlit/auth_libs/Redirect.py
 streamlit/auth_libs/Users.py
 streamlit/auth_libs/pages/Login.py
 streamlit/auth_libs/pages/Profile.py
 streamlit/auth_libs/pages/Register.py
-streamlit/components/agent_selector.py
+streamlit/components/chain.py
 streamlit/components/docs.py
 streamlit/components/history.py
 streamlit/components/learning.py
+streamlit/components/selectors.py
 streamlit/components/verify_backend.py
 streamlit/pages/0-Agent_Settings.py
 streamlit/pages/1-Prompt_Templates.py
 streamlit/pages/2-Chain_Management.py
 streamlit/pages/3-Interact.py
 tests/ApiClient.py
 tests/test-commands.ipynb
```

### Comparing `agixt-1.2.3/docs/1-Getting started/Quick Start.md` & `agixt-1.2.4/docs/1-Getting started/Quick Start.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/1-Getting started/Support.md` & `agixt-1.2.4/docs/1-Getting started/Support.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/2-Concepts/0-Core Concepts.md` & `agixt-1.2.4/docs/2-Concepts/0-Core Concepts.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/2-Concepts/Agents.md` & `agixt-1.2.4/docs/2-Concepts/Agents.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/2-Concepts/Chains.md` & `agixt-1.2.4/docs/2-Concepts/Chains.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/2-Concepts/Chat.md` & `agixt-1.2.4/docs/2-Concepts/Chat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/2-Concepts/Commands.md` & `agixt-1.2.4/docs/2-Concepts/Commands.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/2-Concepts/Instructions.md` & `agixt-1.2.4/docs/2-Concepts/Instructions.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/2-Concepts/Prompts.md` & `agixt-1.2.4/docs/2-Concepts/Prompts.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/2-Concepts/Smart Chat.md` & `agixt-1.2.4/docs/2-Concepts/Smart Chat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/2-Concepts/Smart Instruct.md` & `agixt-1.2.4/docs/2-Concepts/Smart Instruct.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/2-Concepts/Smart Task.md` & `agixt-1.2.4/docs/2-Concepts/Smart Task.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/3-Providers/Anthropic Claude.md` & `agixt-1.2.4/docs/3-Providers/Anthropic Claude.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/3-Providers/Azure OpenAI.md` & `agixt-1.2.4/docs/3-Providers/Azure OpenAI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/3-Providers/ChatGPT.md` & `agixt-1.2.4/docs/3-Providers/ChatGPT.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/3-Providers/FastChat.md` & `agixt-1.2.4/docs/3-Providers/FastChat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/3-Providers/GPT4ALL-GPU.md` & `agixt-1.2.4/docs/3-Providers/GPT4ALL-GPU.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/3-Providers/GPT4ALL.md` & `agixt-1.2.4/docs/3-Providers/GPT4ALL.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/3-Providers/GPT4Free.md` & `agixt-1.2.4/docs/3-Providers/GPT4Free.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/3-Providers/Google Bard.md` & `agixt-1.2.4/docs/3-Providers/Google Bard.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/3-Providers/Hugging Face Transformers.md` & `agixt-1.2.4/docs/3-Providers/Hugging Face Transformers.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/3-Providers/HuggingChat.md` & `agixt-1.2.4/docs/3-Providers/HuggingChat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/3-Providers/Microsoft Bing.md` & `agixt-1.2.4/docs/3-Providers/Microsoft Bing.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/3-Providers/Oobabooga Text Generation Web UI.md` & `agixt-1.2.4/docs/3-Providers/Oobabooga Text Generation Web UI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/3-Providers/OpenAI.md` & `agixt-1.2.4/docs/3-Providers/OpenAI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/3-Providers/llamacpp API.md` & `agixt-1.2.4/docs/3-Providers/llamacpp API.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/3-Providers/llamacpp.md` & `agixt-1.2.4/docs/3-Providers/llamacpp.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/README.md` & `agixt-1.2.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/images/AGiXT-gradient-flat.svg` & `agixt-1.2.4/docs/images/AGiXT-gradient-flat.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/images/AGiXT-gradient-light.svg` & `agixt-1.2.4/docs/images/AGiXT-gradient-light.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/images/AGiXT.png` & `agixt-1.2.4/docs/images/AGiXT.png`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/images/AGiXT.svg` & `agixt-1.2.4/docs/images/AGiXT.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/images/AGiXT_Original_PSD.psd` & `agixt-1.2.4/docs/images/AGiXT_Original_PSD.psd`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/images/AGiXTwhiteborder.svg` & `agixt-1.2.4/docs/images/AGiXTwhiteborder.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/images/Docker-desktop-win-setting-streamlit.png` & `agixt-1.2.4/docs/images/Docker-desktop-win-setting-streamlit.png`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/images/Smart Instruct.drawio` & `agixt-1.2.4/docs/images/Smart Instruct.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/images/Smart Instruct.drawio.svg` & `agixt-1.2.4/docs/images/Smart Instruct.drawio.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/images/Smart Tasks.drawio` & `agixt-1.2.4/docs/images/Smart Tasks.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/images/Smart Tasks.drawio.svg` & `agixt-1.2.4/docs/images/Smart Tasks.drawio.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/docs/images/Untitled Diagram.drawio` & `agixt-1.2.4/docs/images/Untitled Diagram.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/setup.py` & `agixt-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/streamlit/ApiClient.py` & `agixt-1.2.4/streamlit/ApiClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,22 @@
 
     @staticmethod
     def delete_agent_history(agent_name: str) -> str:
         response = requests.delete(f"{base_uri}/api/agent/{agent_name}/history")
         return response.json()["message"]
 
     @staticmethod
+    def delete_history_message(agent_name: str, message: str) -> str:
+        response = requests.delete(
+            f"{base_uri}/api/agent/{agent_name}/history/message",
+            json={"message": message},
+        )
+        return response.json()["message"]
+
+    @staticmethod
     def wipe_agent_memories(agent_name: str) -> str:
         response = requests.delete(f"{base_uri}/api/agent/{agent_name}/memory")
         return response.json()["message"]
 
     @staticmethod
     def prompt_agent(
         agent_name: str,
```

### Comparing `agixt-1.2.3/streamlit/Main.py` & `agixt-1.2.4/streamlit/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/streamlit/auth_libs/Cfig.py` & `agixt-1.2.4/streamlit/auth_libs/Cfig.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/streamlit/auth_libs/Redirect.py` & `agixt-1.2.4/streamlit/auth_libs/Redirect.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/streamlit/auth_libs/Users.py` & `agixt-1.2.4/streamlit/auth_libs/Users.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/streamlit/auth_libs/pages/Login.py` & `agixt-1.2.4/streamlit/auth_libs/pages/Login.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/streamlit/auth_libs/pages/Profile.py` & `agixt-1.2.4/streamlit/auth_libs/pages/Profile.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/streamlit/auth_libs/pages/Register.py` & `agixt-1.2.4/streamlit/auth_libs/pages/Register.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/streamlit/components/docs.py` & `agixt-1.2.4/streamlit/components/docs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/streamlit/components/history.py` & `agixt-1.2.4/streamlit/components/history.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/streamlit/components/learning.py` & `agixt-1.2.4/streamlit/components/learning.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 import streamlit as st
-from components.agent_selector import agent_selector
 from ApiClient import ApiClient
 import os
 
 
-def learning_page():
-    agent_name = agent_selector()
+def learning_page(agent_name):
     st.markdown("### Choose a Method for Learning")
-    api_client = ApiClient()
-
-    # Initialize session state for stop events and agent status if not exist
-    if "agent_status" not in st.session_state:
-        st.session_state.agent_status = {}
 
     if agent_name:
         st.markdown("### Learn from a file")
         learn_file_upload = st.file_uploader(
             "Upload a file for the agent to learn from.", accept_multiple_files=True
         )
         if learn_file_upload is not None:
```

### Comparing `agixt-1.2.3/streamlit/components/verify_backend.py` & `agixt-1.2.4/streamlit/components/verify_backend.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/streamlit/pages/0-Agent_Settings.py` & `agixt-1.2.4/streamlit/pages/0-Agent_Settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import streamlit as st
 from ApiClient import ApiClient
-from components.agent_selector import agent_selector
+from components.selectors import agent_selection
 from components.verify_backend import verify_backend
 from components.docs import agixt_docs
 
 verify_backend()
 
 
 st.set_page_config(
@@ -77,15 +77,15 @@
         "Log requests to files", key="LOG_REQUESTS", value=value
     )
 
     return rendered_settings
 
 
 st.header("Agent Settings")
-agent_name = agent_selector()
+agent_name = agent_selection()
 
 if "new_agent_name" not in st.session_state:
     st.session_state["new_agent_name"] = ""
 
 # Add an input field for the new agent's name
 new_agent = False
```

### Comparing `agixt-1.2.3/streamlit/pages/1-Prompt_Templates.py` & `agixt-1.2.4/streamlit/pages/1-Prompt_Templates.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/streamlit/pages/3-Interact.py` & `agixt-1.2.4/streamlit/pages/3-Interact.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import streamlit as st
-from components.agent_selector import agent_selector
+from components.selectors import agent_selection
 from ApiClient import ApiClient
 from components.learning import learning_page
 from components.history import get_history
 from components.verify_backend import verify_backend
 from components.docs import agixt_docs
 
-verify_backend()
-
 st.set_page_config(
     page_title="Interact with Agents",
     page_icon=":speech_balloon:",
     layout="wide",
 )
+
+
+verify_backend()
+
+
 agixt_docs()
 
 st.header("Interact with Agents")
 # Create an instance of the API Client
 api_client = ApiClient()
 
 # Fetch available prompts
@@ -24,18 +27,23 @@
 
 # Add a dropdown to select a mode
 mode = st.selectbox("Select Mode", ["Prompt", "Chat", "Instruct", "Learning", "Chains"])
 
 if "chat_history" not in st.session_state:
     st.session_state["chat_history"] = ""
 
+agent_name = agent_selection() if mode != "Chains" else None
+
+if agent_name:
+    st.session_state["chat_history"] = get_history(agent_name=agent_name)
+
+
 # If the user selects Prompt, then show the prompt functionality
 if mode == "Prompt":
     st.markdown("### Choose an Agent and Prompt")
-    agent_name = agent_selector()
     # Add a dropdown to select a prompt
     prompt_name = st.selectbox("Choose a prompt", prompts)
     # Fetch arguments for the selected prompt
     prompt_args = api_client.get_prompt_args(prompt_name=prompt_name)
 
     # Add input fields for prompt arguments
     st.markdown("### Prompt Variables")
@@ -74,15 +82,14 @@
         )
 
         # Print the response
         st.write(f"{agent_name}: {agent_prompt_resp}")
 
 if mode == "Chat":
     st.markdown("### Choose an Agent to Chat With")
-    agent_name = agent_selector()
     smart_chat_toggle = st.checkbox("Enable Smart Chat")
     chat_prompt = st.text_input("Enter your message", key="chat_prompt")
     send_button = st.button("Send Message")
 
     if send_button:
         if agent_name and chat_prompt:
             with st.spinner("Thinking, please wait..."):
@@ -96,15 +103,14 @@
                     response = ApiClient.chat(agent_name=agent_name, prompt=chat_prompt)
                 if response:
                     st.experimental_rerun()
 
 
 if mode == "Instruct":
     st.markdown("### Choose an Agent to Instruct")
-    agent_name = agent_selector()
     smart_instruct_toggle = st.checkbox("Enable Smart Instruct")
     instruct_prompt = st.text_input("Enter your instruction", key="instruct_prompt")
     send_button = st.button("Send Message")
 
     if send_button:
         if agent_name and instruct_prompt:
             with st.spinner("Thinking, please wait..."):
@@ -118,29 +124,27 @@
                     response = ApiClient.instruct(
                         agent_name=agent_name, prompt=instruct_prompt
                     )
             if response:
                 st.experimental_rerun()
 
 if mode == "Learning":
-    learning_page()
+    if agent_name:
+        learning_page(agent_name)
 
 if mode == "Chains":
-    st.markdown("### Choose a Chain to Run")
+    st.markdown("### Chain to Run")
     chain_names = ApiClient.get_chains()
-
     chain_action = "Run Chain"
     chain_name = st.selectbox("Chains", chain_names)
     user_input = st.text_input("User Input")
 
     if st.button("Perform Action"):
         if chain_name:
             if chain_action == "Run Chain":
-                ApiClient.run_chain(chain_name=chain_name, user_input=user_input)
-                responses = ApiClient.get_chain_responses(chain_name=chain_name)
+                responses = ApiClient.run_chain(
+                    chain_name=chain_name, user_input=user_input
+                )
                 st.success(f"Chain '{chain_name}' executed.")
                 st.write(responses)
         else:
             st.error("Chain name is required.")
-
-if agent_name:
-    st.session_state["chat_history"] = get_history(agent_name=agent_name)
```

### Comparing `agixt-1.2.3/tests/ApiClient.py` & `agixt-1.2.4/tests/ApiClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,22 @@
 
     @staticmethod
     def delete_agent_history(agent_name: str) -> str:
         response = requests.delete(f"{base_uri}/api/agent/{agent_name}/history")
         return response.json()["message"]
 
     @staticmethod
+    def delete_history_message(agent_name: str, message: str) -> str:
+        response = requests.delete(
+            f"{base_uri}/api/agent/{agent_name}/history/message",
+            json={"message": message},
+        )
+        return response.json()["message"]
+
+    @staticmethod
     def wipe_agent_memories(agent_name: str) -> str:
         response = requests.delete(f"{base_uri}/api/agent/{agent_name}/memory")
         return response.json()["message"]
 
     @staticmethod
     def prompt_agent(
         agent_name: str,
```

### Comparing `agixt-1.2.3/tests/test-commands.ipynb` & `agixt-1.2.4/tests/test-commands.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.2.3/tests/tests.ipynb` & `agixt-1.2.4/tests/tests.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963399004179985%*

 * *Differences: {"'cells'": '{15: {\'outputs\': {0: {\'text\': ["Add agent response: {\'message\': \'Agent '*

 * *            'test_agent created.\'}\\n"]}}}, 27: {\'outputs\': {0: {\'text\': [\'Chat response: '*

 * *            "The capital of France is Paris.\\n']}}}, 29: {'outputs': {0: {'text': {insert: [(0, "*

 * *            "'Agent prompt response: In the sky they soar\\n'), (1, 'With flames of fire they "*

 * *            "roar\\n'), (2, 'Majestic creatures of lore\\n'), (3, 'The dragons we adore\\n'), (5, "*

 * *            '\'Their scale […]*

```diff
@@ -216,15 +216,15 @@
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Add agent response: {'agent_file': 'test_agent/history.yaml'}\n"
+                        "Add agent response: {'message': 'Agent test_agent created.'}\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test add_agent()\n",
@@ -425,15 +425,15 @@
             "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Chat response: new_agent: The capital of France is Paris.\n"
+                        "Chat response: The capital of France is Paris.\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test chat()\n",
@@ -459,43 +459,38 @@
             "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Agent prompt response: Deep within the mountains' keep,\n",
-                        "Where the flames of fire seep,\n",
-                        "Lives a creature of myth and lore,\n",
-                        "A dragon, strong and fierce to the core.\n",
+                        "Agent prompt response: In the sky they soar\n",
+                        "With flames of fire they roar\n",
+                        "Majestic creatures of lore\n",
+                        "The dragons we adore\n",
                         "\n",
-                        "Its scales are sharp and iridescent,\n",
-                        "Reflecting the sun's light so effervescent,\n",
-                        "Its wingspan vast, it takes to flight,\n",
-                        "The dragon's power is a wondrous sight.\n",
+                        "Their scales shimmer in the sun\n",
+                        "A sight that can't be outdone\n",
+                        "Powerful beings second to none\n",
+                        "They make our hearts run\n",
                         "\n",
-                        "Its breath can burn and scorch the land,\n",
-                        "Its roar, a thunder that shakes the sand,\n",
-                        "No mortal being can match its might,\n",
-                        "The dragon's power is unmatched in light.\n",
+                        "Through mountains they fly\n",
+                        "With wings that reach the sky\n",
+                        "A sight that makes us sigh\n",
+                        "Our spirits begin to rise high\n",
                         "\n",
-                        "But do not fear this creature great,\n",
-                        "For legends tell of a different fate,\n",
-                        "When dragons bond with those true and brave,\n",
-                        "They become guardians, noble and gave.\n",
+                        "Legends of them surround\n",
+                        "As their presence astounds\n",
+                        "Bringers of both fear and renown\n",
+                        "The dragons are all around\n",
                         "\n",
-                        "So, if you're pure of heart and soul,\n",
-                        "And seek adventure to make you whole,\n",
-                        "The dragon may see you fit to ride,\n",
-                        "To soar the skies and feel its pride.\n",
-                        "\n",
-                        "But heed its call with utmost care,\n",
-                        "For dragons are creatures that truly rare,\n",
-                        "And if you earn its trust and love,\n",
-                        "You'll have a bond that'll soar above.\n"
+                        "Their beauty and might\n",
+                        "Enchants us through the night\n",
+                        "A sight that's truly a delight\n",
+                        "The dragons, our hearts take flight\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test prompt_agent()\n",
@@ -533,24 +528,15 @@
             "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Instruct response: The capital of France is Paris.\n",
-                        "\n",
-                        "Commands Executed:\n",
-                        "{'Write to File': {'filename': 'capital_of_france.txt', 'text': 'Paris'}}\n",
-                        "\n",
-                        "Command Execution Response:\n",
-                        "\n",
-                        "Executed Command:Write to File with args {'filename': 'capital_of_france.txt', 'text': 'Paris'}.\n",
-                        "Command Output: File written to successfully.\n",
-                        "\n"
+                        "Instruct response: The capital of France is Paris.\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test instruct()\n",
@@ -576,15 +562,15 @@
             "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Chat history: [{'USER': 'June 10, 2023 07:58 PM\\nWhat is the capital of France?'}, {'new_agent': 'June 10, 2023 07:58 PM\\nnew_agent: The capital of France is Paris.'}, {'USER': 'June 10, 2023 07:59 PM\\n'}, {'new_agent': \"June 10, 2023 07:59 PM\\nDeep within the mountains' keep,\\nWhere the flames of fire seep,\\nLives a creature of myth and lore,\\nA dragon, strong and fierce to the core.\\n\\nIts scales are sharp and iridescent,\\nReflecting the sun's light so effervescent,\\nIts wingspan vast, it takes to flight,\\nThe dragon's power is a wondrous sight.\\n\\nIts breath can burn and scorch the land,\\nIts roar, a thunder that shakes the sand,\\nNo mortal being can match its might,\\nThe dragon's power is unmatched in light.\\n\\nBut do not fear this creature great,\\nFor legends tell of a different fate,\\nWhen dragons bond with those true and brave,\\nThey become guardians, noble and gave.\\n\\nSo, if you're pure of heart and soul,\\nAnd seek adventure to make you whole,\\nThe dragon may see you fit to ride,\\nTo soar the skies and feel its pride.\\n\\nBut heed its call with utmost care,\\nFor dragons are creatures that truly rare,\\nAnd if you earn its trust and love,\\nYou'll have a bond that'll soar above.\"}, {'USER': 'June 10, 2023 07:59 PM\\nTell me the capital of France.'}, {'new_agent': \"June 10, 2023 07:59 PM\\nThe capital of France is Paris.\\n\\nCommands Executed:\\n{'Write to File': {'filename': 'capital_of_france.txt', 'text': 'Paris'}}\\n\\nCommand Execution Response:\\n\\nExecuted Command:Write to File with args {'filename': 'capital_of_france.txt', 'text': 'Paris'}.\\nCommand Output: File written to successfully.\\n\"}]\n"
+                        "Chat history: [{'USER': 'June 11, 2023 02:15 PM\\nWhat is the capital of France?'}, {'new_agent': 'June 11, 2023 02:15 PM\\nThe capital of France is Paris.'}, {'USER': 'June 11, 2023 02:15 PM\\n'}, {'new_agent': \"June 11, 2023 02:15 PM\\nIn the sky they soar\\nWith flames of fire they roar\\nMajestic creatures of lore\\nThe dragons we adore\\n\\nTheir scales shimmer in the sun\\nA sight that can't be outdone\\nPowerful beings second to none\\nThey make our hearts run\\n\\nThrough mountains they fly\\nWith wings that reach the sky\\nA sight that makes us sigh\\nOur spirits begin to rise high\\n\\nLegends of them surround\\nAs their presence astounds\\nBringers of both fear and renown\\nThe dragons are all around\\n\\nTheir beauty and might\\nEnchants us through the night\\nA sight that's truly a delight\\nThe dragons, our hearts take flight\"}, {'USER': 'June 11, 2023 02:15 PM\\nTell me the capital of France.'}, {'new_agent': 'June 11, 2023 02:15 PM\\nThe capital of France is Paris.'}]\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_chat_history()\n",
@@ -1037,22 +1023,22 @@
             "metadata": {},
             "source": [
                 "## Run the chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 29,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Run chain response: {'1': {'response': \"Quantum computers, a marvel of science,\\nRevolutionizing our computing reliance.\\nThey operate not with bits but with qubits,\\nEncoding data with quantum bits!\\n\\nQuantum computers can solve problems immense,\\nThat classical computers struggle to make any sense.\\nTheir calculations faster than light,\\nAble to work with incredible might!\\n\\nParallel processing is quantum's forte,\\nIt can work on multiple tasks all day.\\nPrivacy isn't a problem, not at all,\\nQuantum encryption is nigh impossible to breach, for all!\\n\\nQuantum computers, a technology new,\\nA future filled with promise for me and you.\\nThe limits are endless, the sky's the limit,\\nIt's a technological revolution, baby, embrace it!\", 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Quantum Computers'}, 'prompt_type': 'Prompt'}, '2': {'response': \"In the world of tech, we seek to create\\nA mind that's equal to the human state\\nA being of thought, of knowledge and will\\nArtificial General Intelligence, we call it still\\n\\nThrough algorithms, code and complex maths\\nWe strive to replicate human acts\\nTo think, to learn, to perceive and feel\\nAGI is born, from scripts and steel\\n\\nIt's tasks and functions will be vast\\nTo aid mankind in tasks that last\\nFrom curing diseases to creating art\\nAGI will play a vital part\\n\\nBut with great power comes great responsibility\\nAIs must be designed with human morality\\nTo weigh decisions, to consider the impact\\nAGI must be built with empathy intact\\n\\nFor in the end, our fate is sealed\\nOur lives will be entwined with AGI's yield\\nWe must embrace its powers, with caution in mind\\nTo ensure a brighter future for humankind.\", 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Artificial General Intelligence'}, 'prompt_type': 'Prompt'}, '3': {'response': 'File written to successfully.', 'agent_name': 'new_agent', 'prompt': {'command_name': 'Write to File', 'filename': '{user_input}.txt', 'text': 'First Poem:\\n{STEP1}\\n\\nSecond Poem:\\n{STEP2}'}, 'prompt_type': 'Command'}}\n"
+                        "Run chain response: {'1': {'response': \"Quantum computers, they say, are the future of computing\\nWith qubits and entanglement, they solve problems baffling\\n\\nThey work not with zeroes and ones, but with quantum bits\\nWith probability and superposition, they can compute with wits\\n\\nThey're faster and smarter than any computer we know\\nAble to break encryptions, that would have taken ages, just so\\n\\nThey can simulate particles, that classical computers dread\\nRevolutionizing science, with simulations ahead\\n\\nTheir power is immense, and their potential is vast\\nQuantum computers, a technology that's here to last\\n\\nThey usher in a new era of computing, unprecedented\\nA marvel of science and technology, and dreams, unrestricted.\", 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Quantum Computers'}, 'prompt_type': 'Prompt'}, '2': {'response': 'Artificial General Intelligence,\\nA future we all hope to see\\nA machine with true intelligence,\\nWith abilities beyond what we conceive\\n\\nNo longer limited to programmed commands,\\nThis AGI can think on its own\\nMaking decisions, solving problems,\\nAnd perhaps even creating unknowns\\n\\nA new era of progress and breakthroughs,\\nWith technology as our guide\\nAGI leading the way,\\nInnovation at its side\\n\\nBut with great power comes great responsibility,\\nAs we entrust this intelligence to lead\\nWe must ensure it is programmed ethically,\\nGuided by values, empathy, and the need\\n\\nFor progress, for peace, for a better future,\\nAGI can be our partner and friend\\nWith its brilliance and our humanity,\\nTogether we can change the world and transcend.', 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Artificial General Intelligence'}, 'prompt_type': 'Prompt'}, '3': {'response': 'File written to successfully.', 'agent_name': 'new_agent', 'prompt': {'command_name': 'Write to File', 'filename': '{user_input}.txt', 'text': 'First Poem:\\n{STEP1}\\n\\nSecond Poem:\\n{STEP2}'}, 'prompt_type': 'Command'}}\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test run_chain()\n",
@@ -1069,17 +1055,25 @@
             "metadata": {},
             "source": [
                 "## Get the responses from the chain running\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 30,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Chain: {'1': {'response': \"Quantum computers, they say, are the future of computing\\nWith qubits and entanglement, they solve problems baffling\\n\\nThey work not with zeroes and ones, but with quantum bits\\nWith probability and superposition, they can compute with wits\\n\\nThey're faster and smarter than any computer we know\\nAble to break encryptions, that would have taken ages, just so\\n\\nThey can simulate particles, that classical computers dread\\nRevolutionizing science, with simulations ahead\\n\\nTheir power is immense, and their potential is vast\\nQuantum computers, a technology that's here to last\\n\\nThey usher in a new era of computing, unprecedented\\nA marvel of science and technology, and dreams, unrestricted.\", 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Quantum Computers'}, 'prompt_type': 'Prompt'}, '2': {'response': 'Artificial General Intelligence,\\nA future we all hope to see\\nA machine with true intelligence,\\nWith abilities beyond what we conceive\\n\\nNo longer limited to programmed commands,\\nThis AGI can think on its own\\nMaking decisions, solving problems,\\nAnd perhaps even creating unknowns\\n\\nA new era of progress and breakthroughs,\\nWith technology as our guide\\nAGI leading the way,\\nInnovation at its side\\n\\nBut with great power comes great responsibility,\\nAs we entrust this intelligence to lead\\nWe must ensure it is programmed ethically,\\nGuided by values, empathy, and the need\\n\\nFor progress, for peace, for a better future,\\nAGI can be our partner and friend\\nWith its brilliance and our humanity,\\nTogether we can change the world and transcend.', 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Artificial General Intelligence'}, 'prompt_type': 'Prompt'}, '3': {'response': 'File written to successfully.', 'agent_name': 'new_agent', 'prompt': {'command_name': 'Write to File', 'filename': '{user_input}.txt', 'text': 'First Poem:\\n{STEP1}\\n\\nSecond Poem:\\n{STEP2}'}, 'prompt_type': 'Command'}}\n"
+                    ]
+                }
+            ],
             "source": [
                 "# Need to make a function to get_chain_responses() as it's not in the API yet.\n",
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_chain()\n",
                 "chain_name = \"Poem Writing Chain\"\n",
                 "chain = ApiClient.get_chain_responses(chain_name=chain_name)\n",
@@ -1092,17 +1086,25 @@
             "metadata": {},
             "source": [
                 "## Delete a step from the chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 31,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Delete step response: Step 2 deleted from chain 'Poem Writing Chain'.\n"
+                    ]
+                }
+            ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test delete_step()\n",
                 "chain_name = \"Poem Writing Chain\"\n",
                 "delete_step_resp = ApiClient.delete_step(chain_name=chain_name, step_number=2)\n",
                 "print(\"Delete step response:\", delete_step_resp)"
@@ -1114,17 +1116,25 @@
             "metadata": {},
             "source": [
                 "## Delete the chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 32,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Delete chain response: Chain 'Poem Writing Chain' deleted.\n"
+                    ]
+                }
+            ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test delete_chain()\n",
                 "chain_name = \"Poem Writing Chain\"\n",
                 "delete_chain_resp = ApiClient.delete_chain(chain_name=chain_name)\n",
                 "print(\"Delete chain response:\", delete_chain_resp)"
@@ -1138,17 +1148,25 @@
                 "# Prompts\n",
                 "\n",
                 "## Get a list of prompts available to use\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 33,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Prompts: ['Pseudo Code', 'SmartInstruct-Researcher', 'Custom Input', 'Title a Poem', 'ValidationFailed', 'SmartTask-CleanResponse', 'SmartChat-Researcher', 'Tell Me How', 'Execution', 'Score Response', 'Validation', 'Write a Haiku', 'SmartInstruct-Resolver', 'SmartInstruct-CleanResponse', 'SmartInstruct-StepByStep', 'instruct', 'Pick a Poem Subject', 'Task Execution', 'Check-Instruction', 'SmartTask-Execution', 'SmartChat-Resolver', 'Chat', 'Create New Command', 'SmartChat-CleanResponse', 'Prioritize', 'Pick-a-Link', 'SmartInstruct-Execution', 'Write a Poem', 'JSONFormatter', 'SmartTask-StepByStep', 'Instruction', 'WebSearch', 'SmartChat-StepByStep', 'Get Task List']\n"
+                    ]
+                }
+            ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_prompts()\n",
                 "prompts = ApiClient.get_prompts()\n",
                 "print(\"Prompts:\", prompts)"
             ]
@@ -1161,17 +1179,25 @@
                 "## Create a new prompt\n",
                 "\n",
                 "We'll make a basic prompt that asks the AI to tell us a short story about a subject. The subject is not yet defined, it would be defined in a chain. Using `{variable_name}` in a prompt will allow you to define the variable in a chain and have it be used in the prompt.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 34,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Add prompt response: Prompt 'Short Story' added.\n"
+                    ]
+                }
+            ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test add_prompt()\n",
                 "add_prompt_resp = ApiClient.add_prompt(\n",
                 "    prompt_name=\"Short Story\", prompt=\"Tell me a short story about {subject}\"\n",
                 ")\n",
@@ -1184,38 +1210,55 @@
             "metadata": {},
             "source": [
                 "## Get the prompt content\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 35,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Get prompt response: Write a poem about {subject} .\n",
+                        "{user_input}\n"
+                    ]
+                }
+            ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_prompt()\n",
-                "get_prompt_resp = ApiClient.get_prompt(prompt_name=\"Short Story\")\n",
+                "get_prompt_resp = ApiClient.get_prompt(prompt_name=\"Write a Poem\")\n",
                 "print(\"Get prompt response:\", get_prompt_resp)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Get the prompt variables\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 36,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Get prompt args response: ['subject']\n"
+                    ]
+                }
+            ],
             "source": [
                 "# Get prompt args\n",
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_prompt_args()\n",
                 "get_prompt_args_resp = ApiClient.get_prompt_args(prompt_name=\"Short Story\")\n",
                 "print(\"Get prompt args response:\", get_prompt_args_resp)\n"
@@ -1229,17 +1272,25 @@
                 "## Update the prompt content\n",
                 "\n",
                 "We'll ask it to `Add a dragon to the story somehow` in the prompt to make the short story more interesting.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 37,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Update prompt response: Prompt 'Short Story' updated.\n"
+                    ]
+                }
+            ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test update_prompt()\n",
                 "update_prompt_resp = ApiClient.update_prompt(\n",
                 "    prompt_name=\"Short Story\",\n",
                 "    prompt=\"Tell me a short story about {subject}. Add a dragon to the story somehow.\",\n",
@@ -1255,17 +1306,25 @@
                 "## Delete the prompt\n",
                 "\n",
                 "If you don't want the prompt anymore, delete it.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 38,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Delete prompt response: Prompt 'Short Story' deleted.\n"
+                    ]
+                }
+            ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test delete_prompt()\n",
                 "delete_prompt_resp = ApiClient.delete_prompt(prompt_name=\"Short Story\")\n",
                 "print(\"Delete prompt response:\", delete_prompt_resp)"
             ]
@@ -1278,17 +1337,25 @@
                 "## Delete Agent History\n",
                 "\n",
                 "Delete the history for the agent.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 39,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Delete agent response: History for agent new_agent deleted.\n"
+                    ]
+                }
+            ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test delete_agent()\n",
                 "agent_name = \"new_agent\"\n",
                 "delete_agent_resp = ApiClient.delete_agent_history(agent_name=agent_name)\n",
                 "print(\"Delete agent response:\", delete_agent_resp)\n"
@@ -1302,17 +1369,25 @@
                 "## Delete the Agent\n",
                 "\n",
                 "If you are done with the agent and don't want or need it anymore, you can delete it along with everything associated with it, such as its memories, settings, and history. The Agent isn't just fired, it is dead.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 40,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Delete agent response: Agent new_agent deleted.\n"
+                    ]
+                }
+            ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test delete_agent()\n",
                 "agent_name = \"new_agent\"\n",
                 "delete_agent_resp = ApiClient.delete_agent(agent_name=agent_name)\n",
                 "print(\"Delete agent response:\", delete_agent_resp)"
```

