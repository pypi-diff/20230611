# Comparing `tmp/chatgpt-tool-hub-0.4.4.tar.gz` & `tmp/chatgpt-tool-hub-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-tool-hub-0.4.4.tar", last modified: Mon May 15 15:53:25 2023, max compression
+gzip compressed data, was "chatgpt-tool-hub-0.4.5.tar", last modified: Sun Jun 11 16:29:23 2023, max compression
```

## Comparing `chatgpt-tool-hub-0.4.4.tar` & `chatgpt-tool-hub-0.4.5.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.545026 chatgpt-tool-hub-0.4.4/
--rw-r--r--   0 goldfish   (502) staff       (20)     1068 2023-03-27 01:02:03.000000 chatgpt-tool-hub-0.4.4/LICENSE
--rw-r--r--   0 goldfish   (502) staff       (20)    14697 2023-05-15 15:53:25.544794 chatgpt-tool-hub-0.4.4/PKG-INFO
--rw-r--r--   0 goldfish   (502) staff       (20)    13902 2023-05-04 15:37:21.000000 chatgpt-tool-hub-0.4.4/README.md
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.516544 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/
--rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.518368 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/
--rw-r--r--   0 goldfish   (502) staff       (20)       99 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2516 2023-05-04 17:20:51.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/app.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2874 2023-05-12 01:12:49.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/app_factory.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1921 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/lite_app.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5190 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/victorinox.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.519129 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/
--rw-r--r--   0 goldfish   (502) staff       (20)      150 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      210 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/all_bot_list.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.519780 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/chat_bot/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/chat_bot/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)    11410 2023-05-15 14:37:49.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/chat_bot/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2310 2023-05-15 15:34:09.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/chat_bot/prompt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.520303 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/qa_bot/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/qa_bot/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4988 2023-05-15 14:37:53.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/qa_bot/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)      883 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/qa_bot/prompt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.521413 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/
--rw-r--r--   0 goldfish   (502) staff       (20)      155 2023-04-08 18:26:04.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.521952 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/api/
--rw-r--r--   0 goldfish   (502) staff       (20)      138 2023-04-08 18:27:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/api/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4749 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/api/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1273 2023-05-15 15:34:57.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/api/prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)    10572 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     7498 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/llm.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.525100 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5081 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/cache.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2079 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/calculate_token.py
--rw-r--r--   0 goldfish   (502) staff       (20)    24793 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/callbacks.py
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/config.py
--rw-r--r--   0 goldfish   (502) staff       (20)      359 2023-05-12 01:00:31.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/constants.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1256 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/document.py
--rw-r--r--   0 goldfish   (502) staff       (20)      968 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/formatting.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1020 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/input.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5776 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/json_utils.py
--rw-r--r--   0 goldfish   (502) staff       (20)      859 2023-05-13 16:15:44.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/log.py
--rw-r--r--   0 goldfish   (502) staff       (20)     8577 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/schema.py
--rw-r--r--   0 goldfish   (502) staff       (20)      630 2023-03-27 14:21:20.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/singleton.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6621 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/text_splitter.py
--rw-r--r--   0 goldfish   (502) staff       (20)      882 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/utils.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.526044 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/database/
--rw-r--r--   0 goldfish   (502) staff       (20)      133 2023-03-27 18:19:31.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/database/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1696 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/database/chat_memory.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2388 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/database/token_buffer.py
--rw-r--r--   0 goldfish   (502) staff       (20)      526 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/database/utils.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.526973 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/engine/
--rw-r--r--   0 goldfish   (502) staff       (20)      103 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/engine/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)    12786 2023-05-12 00:47:46.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/engine/bot.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2071 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/engine/initialize.py
--rw-r--r--   0 goldfish   (502) staff       (20)    13050 2023-04-27 15:08:27.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/engine/tool_engine.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.528001 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/
--rw-r--r--   0 goldfish   (502) staff       (20)     2456 2023-05-13 15:52:05.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)    12913 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/base.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.528927 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/chatgpt/
--rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-03-27 18:19:49.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/chatgpt/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4872 2023-05-04 10:03:38.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/chatgpt/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)    15985 2023-05-04 12:49:56.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/chatgpt/chatgpt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.529220 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/dashscope/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-05-04 10:59:11.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/dashscope/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      903 2023-05-04 10:14:15.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/model_factory.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.529326 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/moss/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-05-04 10:58:43.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/moss/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.530159 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/
--rw-r--r--   0 goldfish   (502) staff       (20)      751 2023-03-27 18:21:02.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6359 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6316 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/chat.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4323 2023-03-30 16:33:18.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/prompt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.531510 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/
--rw-r--r--   0 goldfish   (502) staff       (20)     1395 2023-05-12 01:15:02.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      321 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/all_tool_list.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.532469 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/arxiv_search/
--rw-r--r--   0 goldfish   (502) staff       (20)       63 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/arxiv_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1700 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/arxiv_search/api_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2937 2023-05-05 15:15:58.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/arxiv_search/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3219 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/arxiv_search/wrapper.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4140 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/base_tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.533105 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/bing_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      140 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/bing_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1476 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/bing_search/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3427 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/bing_search/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.533676 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/google_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      165 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/google_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2290 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/google_search/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3552 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/google_search/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.534052 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/hello_tool/
--rw-r--r--   0 goldfish   (502) staff       (20)       60 2023-05-04 14:00:20.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/hello_tool/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1070 2023-05-04 13:53:09.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/hello_tool/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2608 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/load_tools.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.534792 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/meteo/
--rw-r--r--   0 goldfish   (502) staff       (20)       62 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/meteo/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5263 2023-04-26 16:51:21.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/meteo/docs_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1965 2023-05-06 18:07:09.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/meteo/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.535241 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/
--rw-r--r--   0 goldfish   (502) staff       (20)      884 2023-05-12 00:47:46.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.535660 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/finance_news/
--rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/finance_news/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1349 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/finance_news/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.536800 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/morning_news/
--rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/morning_news/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      639 2023-04-11 16:17:29.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/morning_news/prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3142 2023-05-12 01:24:50.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/morning_news/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.537356 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/news_api/
--rw-r--r--   0 goldfish   (502) staff       (20)       66 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/news_api/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2709 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/news_api/docs_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1826 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/news_api/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2257 2023-05-12 01:22:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.537750 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/python/
--rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/python/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2375 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/python/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.538310 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/searxng_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      169 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/searxng_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2323 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/searxng_search/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)    15639 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/searxng_search/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.538903 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/summary/
--rw-r--r--   0 goldfish   (502) staff       (20)      196 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/summary/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      665 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/summary/map_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)      464 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/summary/reduce_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     7304 2023-05-15 14:53:02.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/summary/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.539570 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/system/
--rw-r--r--   0 goldfish   (502) staff       (20)      127 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/system/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1046 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/system/answer_user.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1329 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/system/debug.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.540198 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/terminal/
--rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/terminal/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4412 2023-04-28 11:33:01.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/terminal/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3667 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)      916 2023-05-12 01:15:02.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/tool_register.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.540716 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/visual_dl/
--rw-r--r--   0 goldfish   (502) staff       (20)       73 2023-04-09 04:05:39.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/visual_dl/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2377 2023-04-28 11:33:15.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/visual_dl/text2image.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.542687 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/
--rw-r--r--   0 goldfish   (502) staff       (20)     2397 2023-04-26 15:57:51.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5173 2023-05-05 16:21:45.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/browser.py
--rw-r--r--   0 goldfish   (502) staff       (20)      753 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/delete.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2117 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/get.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1231 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/patch.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2054 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/post.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1215 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/put.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4629 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.543869 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wikipedia/
--rw-r--r--   0 goldfish   (502) staff       (20)      142 2023-04-04 16:47:52.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wikipedia/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1372 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wikipedia/wikipedia.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2494 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wikipedia/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.544430 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wolfram_alpha/
--rw-r--r--   0 goldfish   (502) staff       (20)      166 2023-04-08 17:59:17.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wolfram_alpha/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1511 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1896 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py
--rw-r--r--   0 goldfish   (502) staff       (20)       22 2023-05-15 15:02:02.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/version.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-05-15 15:53:25.517210 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub.egg-info/
--rw-r--r--   0 goldfish   (502) staff       (20)    14697 2023-05-15 15:53:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub.egg-info/PKG-INFO
--rw-r--r--   0 goldfish   (502) staff       (20)     5003 2023-05-15 15:53:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub.egg-info/SOURCES.txt
--rw-r--r--   0 goldfish   (502) staff       (20)        1 2023-05-15 15:53:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub.egg-info/dependency_links.txt
--rw-r--r--   0 goldfish   (502) staff       (20)      250 2023-05-15 15:53:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub.egg-info/requires.txt
--rw-r--r--   0 goldfish   (502) staff       (20)       17 2023-05-15 15:53:25.000000 chatgpt-tool-hub-0.4.4/chatgpt_tool_hub.egg-info/top_level.txt
--rw-r--r--   0 goldfish   (502) staff       (20)       38 2023-05-15 15:53:25.545071 chatgpt-tool-hub-0.4.4/setup.cfg
--rw-r--r--   0 goldfish   (502) staff       (20)     1977 2023-04-25 17:38:17.000000 chatgpt-tool-hub-0.4.4/setup.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.016620 chatgpt-tool-hub-0.4.5/
+-rw-r--r--   0 goldfish   (502) staff       (20)     1068 2023-03-27 01:02:03.000000 chatgpt-tool-hub-0.4.5/LICENSE
+-rw-r--r--   0 goldfish   (502) staff       (20)    14697 2023-06-11 16:29:23.016401 chatgpt-tool-hub-0.4.5/PKG-INFO
+-rw-r--r--   0 goldfish   (502) staff       (20)    13902 2023-05-04 15:37:21.000000 chatgpt-tool-hub-0.4.5/README.md
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.989922 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/
+-rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.991733 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/
+-rw-r--r--   0 goldfish   (502) staff       (20)       99 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2516 2023-05-04 17:20:51.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/app.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2874 2023-05-12 01:12:49.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/app_factory.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1921 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/lite_app.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5190 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/victorinox.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.992380 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/
+-rw-r--r--   0 goldfish   (502) staff       (20)      150 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      210 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/all_bot_list.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.992991 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/chat_bot/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/chat_bot/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    11410 2023-05-15 14:37:49.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/chat_bot/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2310 2023-05-15 15:34:09.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/chat_bot/prompt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.993622 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/qa_bot/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/qa_bot/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4988 2023-05-15 14:37:53.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/qa_bot/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      883 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/qa_bot/prompt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.994250 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/
+-rw-r--r--   0 goldfish   (502) staff       (20)      155 2023-04-08 18:26:04.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.994783 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/api/
+-rw-r--r--   0 goldfish   (502) staff       (20)      138 2023-04-08 18:27:25.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/api/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4749 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/api/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1273 2023-05-15 15:34:57.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/api/prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    10572 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     7498 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/llm.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.997401 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5081 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/cache.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2079 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/calculate_token.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    24793 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/callbacks.py
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/config.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      359 2023-05-12 01:00:31.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/constants.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1256 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/document.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      968 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/formatting.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1020 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/input.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5776 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/json_utils.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      859 2023-05-13 16:15:44.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/log.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     8577 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/schema.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      630 2023-03-27 14:21:20.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/singleton.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6621 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/text_splitter.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      882 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/utils.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.998260 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/database/
+-rw-r--r--   0 goldfish   (502) staff       (20)      133 2023-03-27 18:19:31.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/database/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1696 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/database/chat_memory.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2388 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/database/token_buffer.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      526 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/database/utils.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.999187 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/engine/
+-rw-r--r--   0 goldfish   (502) staff       (20)      103 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/engine/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    12786 2023-05-12 00:47:46.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/engine/bot.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2071 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/engine/initialize.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    13050 2023-04-27 15:08:27.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/engine/tool_engine.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.999925 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/
+-rw-r--r--   0 goldfish   (502) staff       (20)     2766 2023-05-20 10:34:57.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    12913 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/base.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.000818 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/chatgpt/
+-rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-03-27 18:19:49.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/chatgpt/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4872 2023-05-04 10:03:38.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/chatgpt/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    16231 2023-05-20 10:32:17.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/chatgpt/chatgpt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.001214 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/dashscope/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-05-04 10:59:11.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/dashscope/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      903 2023-05-04 10:14:15.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/model_factory.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.001340 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/moss/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-05-04 10:58:43.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/moss/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.002313 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/
+-rw-r--r--   0 goldfish   (502) staff       (20)      751 2023-03-27 18:21:02.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6359 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6316 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/chat.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4323 2023-03-30 16:33:18.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/prompt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.003453 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/
+-rw-r--r--   0 goldfish   (502) staff       (20)     1395 2023-05-12 01:15:02.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      321 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/all_tool_list.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.004246 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/arxiv_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)       63 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/arxiv_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1700 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/arxiv_search/api_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2937 2023-05-05 15:15:58.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/arxiv_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3219 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/arxiv_search/wrapper.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4140 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/base_tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.004878 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/bing_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      140 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/bing_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1476 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/bing_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3427 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/bing_search/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.005445 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/google_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      165 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/google_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2290 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/google_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3552 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/google_search/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.005916 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/hello_tool/
+-rw-r--r--   0 goldfish   (502) staff       (20)       60 2023-05-04 14:00:20.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/hello_tool/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1070 2023-05-04 13:53:09.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/hello_tool/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2608 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/load_tools.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.006646 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/meteo/
+-rw-r--r--   0 goldfish   (502) staff       (20)       62 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/meteo/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5263 2023-04-26 16:51:21.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/meteo/docs_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1965 2023-05-06 18:07:09.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/meteo/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.007100 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/
+-rw-r--r--   0 goldfish   (502) staff       (20)      884 2023-05-12 00:47:46.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.007583 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/finance_news/
+-rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/finance_news/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1349 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/finance_news/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.008421 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/morning_news/
+-rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/morning_news/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      639 2023-04-11 16:17:29.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/morning_news/prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3142 2023-05-12 01:24:50.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/morning_news/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.008892 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/news_api/
+-rw-r--r--   0 goldfish   (502) staff       (20)       66 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/news_api/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2709 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/news_api/docs_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1826 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/news_api/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2257 2023-05-12 01:22:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.009183 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/python/
+-rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/python/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2375 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/python/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.009721 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/searxng_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      169 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/searxng_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2323 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/searxng_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    15639 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/searxng_search/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.010450 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/summary/
+-rw-r--r--   0 goldfish   (502) staff       (20)      196 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/summary/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      665 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/summary/map_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      464 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/summary/reduce_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     7304 2023-05-15 14:53:02.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/summary/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.011122 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/system/
+-rw-r--r--   0 goldfish   (502) staff       (20)      127 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/system/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1046 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/system/answer_user.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1329 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/system/debug.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.011809 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/terminal/
+-rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/terminal/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4412 2023-04-28 11:33:01.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/terminal/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3667 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      916 2023-05-12 01:15:02.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/tool_register.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.012363 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/visual_dl/
+-rw-r--r--   0 goldfish   (502) staff       (20)       73 2023-04-09 04:05:39.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/visual_dl/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2377 2023-04-28 11:33:15.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/visual_dl/text2image.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.014043 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/
+-rw-r--r--   0 goldfish   (502) staff       (20)     2397 2023-04-26 15:57:51.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5173 2023-05-05 16:21:45.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/browser.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      753 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/delete.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2117 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/get.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1231 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/patch.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2054 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/post.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1215 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/put.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4629 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.015319 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wikipedia/
+-rw-r--r--   0 goldfish   (502) staff       (20)      142 2023-04-04 16:47:52.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wikipedia/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1372 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wikipedia/wikipedia.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2494 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wikipedia/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:23.016124 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wolfram_alpha/
+-rw-r--r--   0 goldfish   (502) staff       (20)      166 2023-04-08 17:59:17.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wolfram_alpha/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1511 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1896 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py
+-rw-r--r--   0 goldfish   (502) staff       (20)       22 2023-06-11 16:27:47.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/version.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-06-11 16:29:22.990621 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub.egg-info/
+-rw-r--r--   0 goldfish   (502) staff       (20)    14697 2023-06-11 16:29:22.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub.egg-info/PKG-INFO
+-rw-r--r--   0 goldfish   (502) staff       (20)     5003 2023-06-11 16:29:22.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)        1 2023-06-11 16:29:22.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)      250 2023-06-11 16:29:22.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub.egg-info/requires.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)       17 2023-06-11 16:29:22.000000 chatgpt-tool-hub-0.4.5/chatgpt_tool_hub.egg-info/top_level.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)       38 2023-06-11 16:29:23.016664 chatgpt-tool-hub-0.4.5/setup.cfg
+-rw-r--r--   0 goldfish   (502) staff       (20)     1977 2023-04-25 17:38:17.000000 chatgpt-tool-hub-0.4.5/setup.py
```

### Comparing `chatgpt-tool-hub-0.4.4/LICENSE` & `chatgpt-tool-hub-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/PKG-INFO` & `chatgpt-tool-hub-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-tool-hub
-Version: 0.4.4
+Version: 0.4.5
 Summary: An open-source chatgpt tool ecosystem where you can combine tools with chatgpt and use natural language to do anything.
 Home-page: https://github.com/goldfishh/chatgpt-tool-hub
 Author: goldfishh
 Author-email: goldfish.buaa@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `chatgpt-tool-hub-0.4.4/README.md` & `chatgpt-tool-hub-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/app.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/app.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/app_factory.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/app_factory.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/lite_app.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/lite_app.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/apps/victorinox.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/apps/victorinox.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/chat_bot/base.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/chat_bot/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/chat_bot/prompt.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/chat_bot/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/qa_bot/base.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/qa_bot/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/bots/qa_bot/prompt.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/bots/qa_bot/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/api/base.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/api/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/api/prompt.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/api/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/base.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/chains/llm.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/chains/llm.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/cache.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/cache.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/calculate_token.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/calculate_token.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/callbacks.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/callbacks.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/document.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/document.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/formatting.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/formatting.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/input.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/input.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/json_utils.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/json_utils.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/log.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/log.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/schema.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/schema.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/singleton.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/singleton.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/text_splitter.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/text_splitter.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/common/utils.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/common/utils.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/database/chat_memory.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/database/chat_memory.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/database/token_buffer.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/database/token_buffer.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/database/utils.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/database/utils.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/engine/bot.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/engine/bot.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/engine/initialize.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/engine/initialize.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/engine/tool_engine.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/engine/tool_engine.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/base.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/chatgpt/base.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/chatgpt/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/chatgpt/chatgpt.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/chatgpt/chatgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,17 @@
         )
         _llm_api_base_url = get_from_dict_or_env(
             values, "llm_api_base_url", "LLM_API_BASE_URL",
             openai_default_api_base)
         _proxy = get_from_dict_or_env(
             values, "proxy", "PROXY", ""
         )
+        _deployment_id = get_from_dict_or_env(
+            values, "deployment_id", "DEPLOYMENT_ID", ""
+        )
         try:
             import openai
 
             if openai.proxy != _proxy:
                 if _proxy:
                     openai.proxy = _proxy
                     values["proxy"] = _proxy
@@ -188,14 +191,18 @@
                 LOG.info(f"success use customized api base url: {_llm_api_base_url}")
 
             if openai.api_key != _llm_api_key:
                 openai.api_key = _llm_api_key
                 values["llm_api_key"] = _llm_api_key
                 LOG.debug(f"success use llm api key: {_llm_api_key}")
 
+            if _deployment_id:
+                openai.api_type = "azure"
+                openai.api_version = "2023-03-15-preview"
+
         except ImportError:
             raise ValueError(
                 "Could not import openai python package. "
                 "Please it install it with `pip install openai`."
             )
 
         try:
```

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/models/model_factory.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/models/model_factory.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/__init__.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/base.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/chat.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/prompts/prompt.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/__init__.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/arxiv_search/api_prompt.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/arxiv_search/api_prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/arxiv_search/tool.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/arxiv_search/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/arxiv_search/wrapper.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/arxiv_search/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/base_tool.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/bing_search/tool.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/bing_search/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/bing_search/wrapper.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/bing_search/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/google_search/tool.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/google_search/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/google_search/wrapper.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/google_search/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/hello_tool/tool.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/hello_tool/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/load_tools.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/load_tools.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/meteo/docs_prompt.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/meteo/docs_prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/meteo/tool.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/meteo/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/__init__.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/__init__.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/finance_news/tool.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/finance_news/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/morning_news/prompt.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/morning_news/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/morning_news/tool.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/morning_news/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/news_api/docs_prompt.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/news_api/docs_prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/news_api/tool.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/news_api/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/news/tool.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/news/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/python/tool.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/python/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/searxng_search/tool.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/searxng_search/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/searxng_search/wrapper.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/searxng_search/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/summary/map_prompt.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/summary/map_prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/summary/tool.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/summary/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/system/answer_user.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/system/answer_user.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/system/debug.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/system/debug.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/terminal/base.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/terminal/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/tool.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/tool_register.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/tool_register.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/visual_dl/text2image.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/visual_dl/text2image.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/__init__.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/browser.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/browser.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/delete.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/delete.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/get.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/get.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/patch.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/patch.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/post.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/post.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/put.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/put.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/web_requests/wrapper.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/web_requests/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wikipedia/wikipedia.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wikipedia/wrapper.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wikipedia/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub.egg-info/PKG-INFO` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-tool-hub
-Version: 0.4.4
+Version: 0.4.5
 Summary: An open-source chatgpt tool ecosystem where you can combine tools with chatgpt and use natural language to do anything.
 Home-page: https://github.com/goldfishh/chatgpt-tool-hub
 Author: goldfishh
 Author-email: goldfish.buaa@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `chatgpt-tool-hub-0.4.4/chatgpt_tool_hub.egg-info/SOURCES.txt` & `chatgpt-tool-hub-0.4.5/chatgpt_tool_hub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.4/setup.py` & `chatgpt-tool-hub-0.4.5/setup.py`

 * *Files identical despite different names*

