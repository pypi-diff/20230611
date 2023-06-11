# Comparing `tmp/openai_forward-0.2.3.tar.gz` & `tmp/openai_forward-0.2.4.tar.gz`

## Comparing `openai_forward-0.2.3.tar` & `openai_forward-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/__init__.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/__main__.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/app.py
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/base.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/config.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/openai.py
--rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/content/__init__.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/content/chat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/content/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/routers/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/routers/openai_v1.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 openai_forward-0.2.3/openai_forward/routers/schemas.py
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 openai_forward-0.2.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.2.3/LICENSE
--rw-r--r--   0        0        0    10996 2020-02-02 00:00:00.000000 openai_forward-0.2.3/README.md
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 openai_forward-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    12391 2020-02-02 00:00:00.000000 openai_forward-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/__init__.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/__main__.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/app.py
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/base.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/config.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/openai.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/content/__init__.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/content/chat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/content/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/routers/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/routers/openai_v1.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 openai_forward-0.2.4/openai_forward/routers/schemas.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 openai_forward-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.2.4/LICENSE
+-rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 openai_forward-0.2.4/README.md
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 openai_forward-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0    12000 2020-02-02 00:00:00.000000 openai_forward-0.2.4/PKG-INFO
```

### Comparing `openai_forward-0.2.3/openai_forward/__main__.py` & `openai_forward-0.2.4/openai_forward/__main__.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.3/openai_forward/base.py` & `openai_forward-0.2.4/openai_forward/base.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.3/openai_forward/config.py` & `openai_forward-0.2.4/openai_forward/config.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.3/openai_forward/openai.py` & `openai_forward-0.2.4/openai_forward/openai.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.3/openai_forward/tool.py` & `openai_forward-0.2.4/openai_forward/tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ast
 import os
 from typing import Dict, List, Union
 
 import orjson
 from rich import print
-from sparrow import relp
+from sparrow import MeasureTime, relp
 
 
 def yaml_dump(data, filepath, rel_path=False, mode="w"):
     abs_path = relp(filepath, parents=1) if rel_path else filepath
     from yaml import dump
 
     try:
@@ -57,14 +57,16 @@
 
 
 def env2list(env_name: str, sep=" "):
     return str2list(os.environ.get(env_name, "").strip(), sep=sep)
 
 
 def get_matches(messages: List[Dict], assistant: List[Dict]):
+    mt = MeasureTime()
+    mt.start()
     msg_len, ass_len = len(messages), len(assistant)
     if msg_len != ass_len:
         print(f"message({msg_len}) 与 assistant({ass_len}) 长度不匹配")
     matches = []
     assis_idx_to_remove, msg_idx_to_remove = [], []
 
     def cvt(msg: dict, ass: dict):
@@ -72,15 +74,15 @@
             "forwarded-for": msg["forwarded-for"],
             "model": msg["model"],
             "messages": msg["messages"],
             "assistant": ass["assistant"],
         }
 
     for idx_msg in range(len(messages)):
-        win = min(5, len(messages) - 1)
+        win = min(max(abs(ass_len - msg_len), 16), len(messages) - 1)
         range_list = [idx_msg + (i + 1) // 2 * (-1) ** (i + 1) for i in range(win)]
         # range_list = [idx_msg + 0, idx_msg + 1, idx_msg - 1, idx_msg + 2, idx_msg - 2, ...]
         for idx_ass in range_list:
             if idx_ass >= len(assistant):
                 break
             if messages[idx_msg]["uid"] == assistant[idx_ass]["uid"]:
                 matches.append(cvt(messages[idx_msg], assistant[idx_ass]))
@@ -92,14 +94,15 @@
     remains = [
         cvt(x, y) for x in msg_remain for y in assis_remain if x["uid"] == y["uid"]
     ]
     matches.extend(remains)
     ref_len = max(msg_len, ass_len)
     if len(matches) != ref_len:
         print(f"存在{ref_len-len(matches)}条未匹配数据")
+    mt.show_interval("计算耗时：")
     return matches
 
 
 def parse_chat_log(filepath: str):
     with open(filepath, "r", encoding="utf-8") as f:
         messages, assistant = [], []
         for line in f.readlines():
```

### Comparing `openai_forward-0.2.3/openai_forward/content/chat.py` & `openai_forward-0.2.4/openai_forward/content/chat.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,25 +21,29 @@
 
 
 def parse_chat_completions(bytes_: bytes):
     txt_lines = decoder.decode(bytes_.decode("utf-8"))
     line0 = txt_lines[0]
     target_info = dict()
     if line0.startswith("data:"):
+        is_stream = True
         line0 = orjson.loads(line0[6:])
         msg = line0["choices"][0]["delta"]
     else:
-        line0 = orjson.loads(line0)
+        is_stream = False
+        line0 = orjson.loads("".join(txt_lines))
         msg = line0["choices"][0]["message"]
 
     target_info["created"] = line0["created"]
     target_info["id"] = line0["id"]
     target_info["model"] = line0["model"]
     target_info["role"] = msg["role"]
     target_info["content"] = msg.get("content", "")
+    if not is_stream:
+        return target_info
     # loop for stream
     for line in txt_lines[1:]:
         if line in ("", "\n", "\n\n"):
             continue
         elif line.startswith("data: "):
             target_info["content"] += _parse_iter_line_content(line)
         else:
```

### Comparing `openai_forward-0.2.3/openai_forward/routers/openai_v1.py` & `openai_forward-0.2.4/openai_forward/routers/openai_v1.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.3/openai_forward/routers/schemas.py` & `openai_forward-0.2.4/openai_forward/routers/schemas.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.3/.gitignore` & `openai_forward-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.3/LICENSE` & `openai_forward-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.2.3/README.md` & `openai_forward-0.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 <div align="center">
 
 [功能](#功能) |
 [部署指南](#部署指南) |
 [应用](#应用) |
 [配置选项](#配置选项) |
-[聊天日志](#聊天日志)
+[对话日志](#对话日志)
 
 [![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/tejCum?referralCode=U0-kXv)  
 [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/beidongjiedeguang/openai-forward)
 
 </div>
 
 本项目用于解决一些地区无法直接访问OpenAI的问题，将该服务部署在可以正常访问OpenAI API的(云)服务器上，
@@ -70,15 +70,15 @@
 - [x] Railway 一键部署
 - [x] Render 一键部署
 
 **高级功能**
 
 - [x] 允许输入多个openai api key 组成轮询池
 - [x] 自定义 转发api key (见[高级配置](#高级配置))
-- [x] 实时记录聊天记录(包括流式响应的聊天内容)
+- [x] 流式响应对话日志
 
 ## 部署指南
 
 [部署文档](deploy.md)
 
 提供以下几种部署方式  
 **有海外vps方案**
@@ -88,18 +88,18 @@
    > https://api.openai-forward.com
 
 **无vps免费部署方案**
 
 1. [一键Vercel部署](deploy.md#vercel-一键部署) (不推荐)
    > ~~https://vercel.openai-forward.com~~
 2. [cloudflare部署](deploy.md#cloudflare-部署) (推荐)
-   > https://cloudflare.openai-forward.com
+   > https://cloudflare.page.openai-forward.com
 3. [Railway部署](deploy.md#Railway-一键部署)
    > https://railway.openai-forward.com
-4. [Render一键部署](deploy.md#render-一键部署) (较推荐)
+4. [Render一键部署](deploy.md#render-一键部署) (推荐)
    > https://render.openai-forward.com
 
 ## 应用
 
 ### [聊天应用](https://chat.beidongjiedeguang.top)
 
 基于开源项目[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)搭建自己的chatgpt服务  
@@ -198,30 +198,26 @@
 
 
 </details>
 
 ### 环境变量配置项
 支持从运行目录下的`.env`文件中读取
 
-<details markdown="1">
-  <summary>Click for more details</summary>
-
 | 环境变量            | 说明                                                                                                                                |           默认值            |
 |-----------------|-----------------------------------------------------------------------------------------------------------------------------------|:------------------------:|
 | OPENAI_BASE_URL  | 默认 openai官方 api 地址                                                                                                                |        https://api.openai.com           |
 | OPENAI_API_KEY  | 默认openai api key，支持多个默认api key, 以 `sk-` 开头， 以空格分割                                                                                 |            无             |
 | FORWARD_KEY     | 允许调用方使用该key代替openai api key，支持多个forward key, 以空格分割; 如果设置了OPENAI_API_KEY，而没有设置FORWARD_KEY, 则客户端调用时无需提供密钥, 此时出于安全考虑不建议FORWARD_KEY置空 |            无             |
 | ROUTE_PREFIX    | 路由前缀                                                                                                                              |            无             |
 | LOG_CHAT        | 是否记录聊天内容                                                                                                                          |         `false`          |
 
-</details>
 
 ## 高级配置
 
-**设置api_key为自己设置的forward key**  
+**设置openai api_key为自定义的forward key**  
 需要配置 OPENAI_API_KEY 和 FORWARD_KEY, 例如
 <details markdown="1">
   <summary>Click for more details</summary>
 
 ```bash
 OPENAI_API_KEY=sk-*******
 FORWARD_KEY=fk-****** # 这里fk-token由我们自己定义
@@ -262,17 +258,17 @@
     -e BASE_URL="https://api.openai-forward.com" \
     -e CODE="<your password>" \
     yidadaa/chatgpt-next-web 
 ``` 
 
 </details>
 
-## 聊天日志
+## 对话日志
 
-默认不记录聊天日志，若要开启需设置环境变量`LOG_CHAT=true`
+默认不记录对话日志，若要开启需设置环境变量`LOG_CHAT=true`
 <details markdown="1">
   <summary>Click for more details</summary>
 
 保存路径在当前目录下的`Log/chat.log`路径中。  
 记录格式为
 
 ```text
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
                                 OpenAI Forward
                                      ******
                         OpenAI API æ¥å£è½¬åæå¡
                 The fastest way to deploy openai api forwarding
  [PyPI_version] [License] [Release_(latest_by_date)] [GitHub_repo_size] [docer
                 image_size] [tests] [pypi_downloads] [codecov]
    [åè½](#åè½) | [é¨ç½²æå](#é¨ç½²æå) | [åºç¨](#åºç¨) |
-  [éç½®éé¡¹](#éç½®éé¡¹) | [èå¤©æ¥å¿](#èå¤©æ¥å¿) [![Deploy on
+  [éç½®éé¡¹](#éç½®éé¡¹) | [å¯¹è¯æ¥å¿](#å¯¹è¯æ¥å¿) [![Deploy on
     Railway](https://railway.app/button.svg)](https://railway.app/template/
   tejCum?referralCode=U0-kXv) [![Deploy to Render](https://render.com/images/
      deploy-to-render-button.svg)](https://render.com/deploy?repo=https://
                  github.com/beidongjiedeguang/openai-forward)
 æ¬é¡¹ç®ç¨äºè§£å³ä¸äºå°åºæ æ³ç´æ¥è®¿é®OpenAIçé®é¢ï¼å°è¯¥æå¡é¨ç½²å¨å¯ä»¥æ­£å¸¸è®¿é®OpenAI
 APIç(äº)æå¡å¨ä¸ï¼
 éè¿è¯¥æå¡è½¬åOpenAIçè¯·æ±ãå³æ­å»ºååä»£çæå¡;
@@ -19,27 +19,27 @@
 key. --- ç±æ¬é¡¹ç®æ­å»ºçé¿æä»£çå°åï¼ > https://api.openai-
 forward.com ## åè½ **åºç¡åè½** - [x] æ¯æè½¬åOpenAIæææ¥å£ -
 [x] æ¯ææµå¼ååº - [x] æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½²
 - [x] pip å®è£é¨ç½² - [x] cloudflare é¨ç½² - [x] ~~Vercelä¸é®é¨ç½²
 (ä¸å»ºè®®)~~ - [x] Railway ä¸é®é¨ç½² - [x] Render ä¸é®é¨ç½²
 **é«çº§åè½** - [x] åè®¸è¾å¥å¤ä¸ªopenai api key ç»æè½®è¯¢æ±  - [x]
 èªå®ä¹ è½¬åapi key (è§[é«çº§éç½®](#é«çº§éç½®)) - [x]
-å®æ¶è®°å½èå¤©è®°å½(åæ¬æµå¼ååºçèå¤©åå®¹) ## é¨ç½²æå
-[é¨ç½²ææ¡£](deploy.md) æä¾ä»¥ä¸å ç§é¨ç½²æ¹å¼ **ææµ·å¤vpsæ¹æ¡**
-1. [pip å®è£é¨ç½²](deploy.md#pipé¨ç½²) (æ¨è) 2. [Dockeré¨ç½²]
-(deploy.md#dockeré¨ç½²) (æ¨è) > https://api.openai-forward.com
-**æ vpsåè´¹é¨ç½²æ¹æ¡** 1. [ä¸é®Vercelé¨ç½²](deploy.md#vercel-
-ä¸é®é¨ç½²) (ä¸æ¨è) > ~~https://vercel.openai-forward.com~~ 2.
-[cloudflareé¨ç½²](deploy.md#cloudflare-é¨ç½²) (æ¨è) > https://
-cloudflare.openai-forward.com 3. [Railwayé¨ç½²](deploy.md#Railway-
-ä¸é®é¨ç½²) > https://railway.openai-forward.com 4. [Renderä¸é®é¨ç½²]
-(deploy.md#render-ä¸é®é¨ç½²) (è¾æ¨è) > https://render.openai-forward.com
-## åºç¨ ### [èå¤©åºç¨](https://chat.beidongjiedeguang.top)
-åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-
-Web)æ­å»ºèªå·±çchatgptæå¡ æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
+æµå¼ååºå¯¹è¯æ¥å¿ ## é¨ç½²æå [é¨ç½²ææ¡£](deploy.md)
+æä¾ä»¥ä¸å ç§é¨ç½²æ¹å¼ **ææµ·å¤vpsæ¹æ¡** 1. [pip å®è£é¨ç½²]
+(deploy.md#pipé¨ç½²) (æ¨è) 2. [Dockeré¨ç½²](deploy.md#dockeré¨ç½²)
+(æ¨è) > https://api.openai-forward.com **æ vpsåè´¹é¨ç½²æ¹æ¡** 1.
+[ä¸é®Vercelé¨ç½²](deploy.md#vercel-ä¸é®é¨ç½²) (ä¸æ¨è) > ~~https://
+vercel.openai-forward.com~~ 2. [cloudflareé¨ç½²](deploy.md#cloudflare-é¨ç½²)
+(æ¨è) > https://cloudflare.page.openai-forward.com 3. [Railwayé¨ç½²]
+(deploy.md#Railway-ä¸é®é¨ç½²) > https://railway.openai-forward.com 4.
+[Renderä¸é®é¨ç½²](deploy.md#render-ä¸é®é¨ç½²) (æ¨è) > https://
+render.openai-forward.com ## åºç¨ ### [èå¤©åºç¨](https://
+chat.beidongjiedeguang.top) åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web](https://
+github.com/Yidadaa/ChatGPT-Next-Web)æ­å»ºèªå·±çchatgptæå¡
+æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
 `BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å  Click for more details
 ```bash docker run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -
 e BASE_URL="https://api.openai-forward.com" \ -e CODE="kunyuan" \ yidadaa/
 chatgpt-next-web ``` è¿éé¨ç½²äºä¸ä¸ªï¼ä¾å¤§å®¶è½»åº¦ä½¿ç¨: https://
 chat.beidongjiedeguang.top , è®¿é®å¯ç : `kunyuan`  ### å¨ä»£ç ä¸­ä½¿ç¨
 **Python** ```diff import openai + openai.api_base = "https://api.openai-
 forward.com/v1" openai.api_key = "sk-******" ```  More Examples **JS/TS**
@@ -59,27 +59,27 @@
 details **`openai-forward run`åæ°éç½®é¡¹** | éç½®é¡¹ | è¯´æ |
 é»è®¤å¼ | |-----------------|-------------------|:----------------------:| |
 --port | æå¡ç«¯å£å· | 8000 | | --workers | å·¥ä½è¿ç¨æ° | 1 | | --
 base_url | å OPENAI_BASE_URL | https://api.openai.com | | --api_key | å
 OPENAI_API_KEY | `None` | | --forward_key | å FORWARD_KEY | `None` | | --
 route_prefix | å ROUTE_PREFIX | `None` | | --log_chat | å LOG_CHAT |
 `False` |  ### ç¯å¢åééç½®é¡¹
-æ¯æä»è¿è¡ç®å½ä¸ç`.env`æä»¶ä¸­è¯»å  Click for more details |
-ç¯å¢åé | è¯´æ | é»è®¤å¼ | |-----------------|------------------------
+æ¯æä»è¿è¡ç®å½ä¸ç`.env`æä»¶ä¸­è¯»å | ç¯å¢åé | è¯´æ |
+é»è®¤å¼ | |-----------------|------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------------|:------------------------:| | OPENAI_BASE_URL |
-é»è®¤ openaiå®æ¹ api å°å | https://api.openai.com | | OPENAI_API_KEY |
-é»è®¤openai api keyï¼æ¯æå¤ä¸ªé»è®¤api key, ä»¥ `sk-` å¼å¤´ï¼
-ä»¥ç©ºæ ¼åå² | æ  | | FORWARD_KEY | åè®¸è°ç¨æ¹ä½¿ç¨è¯¥keyä»£æ¿openai
-api keyï¼æ¯æå¤ä¸ªforward key, ä»¥ç©ºæ ¼åå²;
+----|:------------------------:| | OPENAI_BASE_URL | é»è®¤ openaiå®æ¹ api
+å°å | https://api.openai.com | | OPENAI_API_KEY | é»è®¤openai api
+keyï¼æ¯æå¤ä¸ªé»è®¤api key, ä»¥ `sk-` å¼å¤´ï¼ ä»¥ç©ºæ ¼åå² | æ  | |
+FORWARD_KEY | åè®¸è°ç¨æ¹ä½¿ç¨è¯¥keyä»£æ¿openai api
+keyï¼æ¯æå¤ä¸ªforward key, ä»¥ç©ºæ ¼åå²;
 å¦æè®¾ç½®äºOPENAI_API_KEYï¼èæ²¡æè®¾ç½®FORWARD_KEY,
 åå®¢æ·ç«¯è°ç¨æ¶æ éæä¾å¯é¥,
 æ­¤æ¶åºäºå®å¨èèä¸å»ºè®®FORWARD_KEYç½®ç©º | æ  | | ROUTE_PREFIX |
-è·¯ç±åç¼ | æ  | | LOG_CHAT | æ¯å¦è®°å½èå¤©åå®¹ | `false` |  ##
-é«çº§éç½® **è®¾ç½®api_keyä¸ºèªå·±è®¾ç½®çforward key** éè¦éç½®
+è·¯ç±åç¼ | æ  | | LOG_CHAT | æ¯å¦è®°å½èå¤©åå®¹ | `false` | ##
+é«çº§éç½® **è®¾ç½®openai api_keyä¸ºèªå®ä¹çforward key** éè¦éç½®
 OPENAI_API_KEY å FORWARD_KEY, ä¾å¦  Click for more details ```bash
 OPENAI_API_KEY=sk-******* FORWARD_KEY=fk-****** # è¿éfk-
 tokenç±æä»¬èªå·±å®ä¹ ``` è¿éæä»¬éç½®äºFORWARD_KEYä¸º`fk-******`,
 é£ä¹åé¢å®¢æ·ç«¯å¨è°ç¨æ¶åªéè®¾ç½®OPENAI_API_KEYä¸ºæä»¬èªå®ä¹ç`fk-
 ******` å³å¯ã
 è¿æ ·çå¥½å¤æ¯å¨ä½¿ç¨ä¸äºéè¦è¾å¥OPENAI_API_KEYçç¬¬ä¸æ¹åºç¨æ¶ï¼æä»¬å¯ä»¥ä½¿ç¨`fk-
 ******`æ­éä»£çæå¡ä½¿ç¨ï¼å¦ä¸é¢çä¾å­ï¼
@@ -87,16 +87,16 @@
 **ç¨ä¾:** ```bash curl https://api.openai-forward.com/v1/chat/completions \ -
 H "Content-Type: application/json" \ -H "Authorization: Bearer fk-******" \ -
 d '{ "model": "gpt-3.5-turbo", "messages": [{"role": "user", "content":
 "Hello!"}] }' ``` **Python** ```diff import openai + openai.api_base = "https:/
 /api.openai-forward.com/v1" - openai.api_key = "sk-******" + openai.api_key =
 "fk-******" ``` **Web application** ```bash docker run -d \ -p 3000:3000 \ -
 e OPENAI_API_KEY="fk-******" \ -e BASE_URL="https://api.openai-forward.com" \ -
-e CODE="" \ yidadaa/chatgpt-next-web ```  ## èå¤©æ¥å¿
-é»è®¤ä¸è®°å½èå¤©æ¥å¿ï¼è¥è¦å¼å¯éè®¾ç½®ç¯å¢åé`LOG_CHAT=true`
+e CODE="" \ yidadaa/chatgpt-next-web ```  ## å¯¹è¯æ¥å¿
+é»è®¤ä¸è®°å½å¯¹è¯æ¥å¿ï¼è¥è¦å¼å¯éè®¾ç½®ç¯å¢åé`LOG_CHAT=true`
 Click for more details ä¿å­è·¯å¾å¨å½åç®å½ä¸ç`Log/
 chat.log`è·¯å¾ä¸­ã è®°å½æ ¼å¼ä¸º ```text {'messages': [{'user': 'hi'}],
 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-
 e722b3bdd5c3'} {'assistant': 'Hello! How can I assist you today?', 'uid':
 '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'} {'messages': [{'user': 'Hello!'}],
 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': 'f844d156-e747-4887-aef8-
 e40d977b5ee7'} {'assistant': 'Hi there! How can I assist you today?', 'uid':
```

### Comparing `openai_forward-0.2.3/pyproject.toml` & `openai_forward-0.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openai_forward"
-description = "🚀 Openai api forward · OpenAI 接口转发服务 · stream forwarding"
+description = "🚀 OpenAI API Reverse Proxy · ChatGPT API Proxy"
 authors = [
     { name = "kunyuan", email = "beidongjiedeguang@gmail.com" },
 ]
 license = "MIT"
 requires-python = ">=3.6"
 readme = "README.md"
-keywords = ["openai", "chatgpt", "openai-api", "openai-proxy", "OpenAI API Forwarding", "streaming-api", "fastapi", "python", "httpx"]
+keywords = ["openai", "chatgpt", "openai-api", "openai-proxy", "OpenAI API Forwarding", "streaming-api", "fastapi", "python"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3"
 ]
 
 dependencies = [
@@ -34,26 +34,14 @@
 [project.urls]
 Homepage = "https://github.com/beidongjiedeguang/openai-forward"
 Documentation = "https://github.com/beidongjiedeguang/openai-forward#openai-forward"
 Issues = "https://github.com/beidongjiedeguang/openai-forward/issues"
 Source = "https://github.com/beidongjiedeguang/openai-forward"
 
 [project.optional-dependencies]
-ssl = [
-    "certbot"
-]
-chatgpt = [
-    "revChatGPT",
-]
-bard = [
-    "GoogleBard",
-]
-edge = [
-    "EdgeGPT",
-]
 tool = [
     "orjsonl"
 ]
 
 [project.scripts]
 openai_forward = "openai_forward.__main__:main"
 openai-forward = "openai_forward.__main__:main"
```

### Comparing `openai_forward-0.2.3/PKG-INFO` & `openai_forward-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 Metadata-Version: 2.1
 Name: openai_forward
-Version: 0.2.3
-Summary: 🚀 Openai api forward · OpenAI 接口转发服务 · stream forwarding
+Version: 0.2.4
+Summary: 🚀 OpenAI API Reverse Proxy · ChatGPT API Proxy
 Project-URL: Homepage, https://github.com/beidongjiedeguang/openai-forward
 Project-URL: Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-forward
 Project-URL: Issues, https://github.com/beidongjiedeguang/openai-forward/issues
 Project-URL: Source, https://github.com/beidongjiedeguang/openai-forward
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
-Keywords: OpenAI API Forwarding,chatgpt,fastapi,httpx,openai,openai-api,openai-proxy,python,streaming-api
+Keywords: OpenAI API Forwarding,chatgpt,fastapi,openai,openai-api,openai-proxy,python,streaming-api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Requires-Dist: fastapi
 Requires-Dist: httpx
 Requires-Dist: loguru
 Requires-Dist: orjson
 Requires-Dist: python-dotenv
 Requires-Dist: pytz
 Requires-Dist: sparrow-python>=0.1.3
 Requires-Dist: uvicorn
-Provides-Extra: bard
-Requires-Dist: googlebard; extra == 'bard'
-Provides-Extra: chatgpt
-Requires-Dist: revchatgpt; extra == 'chatgpt'
-Provides-Extra: edge
-Requires-Dist: edgegpt; extra == 'edge'
-Provides-Extra: ssl
-Requires-Dist: certbot; extra == 'ssl'
 Provides-Extra: tool
 Requires-Dist: orjsonl; extra == 'tool'
 Description-Content-Type: text/markdown
 
 **中文** | [**English**](./README_EN.md)
 
 <h1 align="center">
@@ -73,15 +65,15 @@
 
 <div align="center">
 
 [功能](#功能) |
 [部署指南](#部署指南) |
 [应用](#应用) |
 [配置选项](#配置选项) |
-[聊天日志](#聊天日志)
+[对话日志](#对话日志)
 
 [![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/tejCum?referralCode=U0-kXv)  
 [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/beidongjiedeguang/openai-forward)
 
 </div>
 
 本项目用于解决一些地区无法直接访问OpenAI的问题，将该服务部署在可以正常访问OpenAI API的(云)服务器上，
@@ -106,15 +98,15 @@
 - [x] Railway 一键部署
 - [x] Render 一键部署
 
 **高级功能**
 
 - [x] 允许输入多个openai api key 组成轮询池
 - [x] 自定义 转发api key (见[高级配置](#高级配置))
-- [x] 实时记录聊天记录(包括流式响应的聊天内容)
+- [x] 流式响应对话日志
 
 ## 部署指南
 
 [部署文档](deploy.md)
 
 提供以下几种部署方式  
 **有海外vps方案**
@@ -124,18 +116,18 @@
    > https://api.openai-forward.com
 
 **无vps免费部署方案**
 
 1. [一键Vercel部署](deploy.md#vercel-一键部署) (不推荐)
    > ~~https://vercel.openai-forward.com~~
 2. [cloudflare部署](deploy.md#cloudflare-部署) (推荐)
-   > https://cloudflare.openai-forward.com
+   > https://cloudflare.page.openai-forward.com
 3. [Railway部署](deploy.md#Railway-一键部署)
    > https://railway.openai-forward.com
-4. [Render一键部署](deploy.md#render-一键部署) (较推荐)
+4. [Render一键部署](deploy.md#render-一键部署) (推荐)
    > https://render.openai-forward.com
 
 ## 应用
 
 ### [聊天应用](https://chat.beidongjiedeguang.top)
 
 基于开源项目[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)搭建自己的chatgpt服务  
@@ -234,30 +226,26 @@
 
 
 </details>
 
 ### 环境变量配置项
 支持从运行目录下的`.env`文件中读取
 
-<details markdown="1">
-  <summary>Click for more details</summary>
-
 | 环境变量            | 说明                                                                                                                                |           默认值            |
 |-----------------|-----------------------------------------------------------------------------------------------------------------------------------|:------------------------:|
 | OPENAI_BASE_URL  | 默认 openai官方 api 地址                                                                                                                |        https://api.openai.com           |
 | OPENAI_API_KEY  | 默认openai api key，支持多个默认api key, 以 `sk-` 开头， 以空格分割                                                                                 |            无             |
 | FORWARD_KEY     | 允许调用方使用该key代替openai api key，支持多个forward key, 以空格分割; 如果设置了OPENAI_API_KEY，而没有设置FORWARD_KEY, 则客户端调用时无需提供密钥, 此时出于安全考虑不建议FORWARD_KEY置空 |            无             |
 | ROUTE_PREFIX    | 路由前缀                                                                                                                              |            无             |
 | LOG_CHAT        | 是否记录聊天内容                                                                                                                          |         `false`          |
 
-</details>
 
 ## 高级配置
 
-**设置api_key为自己设置的forward key**  
+**设置openai api_key为自定义的forward key**  
 需要配置 OPENAI_API_KEY 和 FORWARD_KEY, 例如
 <details markdown="1">
   <summary>Click for more details</summary>
 
 ```bash
 OPENAI_API_KEY=sk-*******
 FORWARD_KEY=fk-****** # 这里fk-token由我们自己定义
@@ -298,17 +286,17 @@
     -e BASE_URL="https://api.openai-forward.com" \
     -e CODE="<your password>" \
     yidadaa/chatgpt-next-web 
 ``` 
 
 </details>
 
-## 聊天日志
+## 对话日志
 
-默认不记录聊天日志，若要开启需设置环境变量`LOG_CHAT=true`
+默认不记录对话日志，若要开启需设置环境变量`LOG_CHAT=true`
 <details markdown="1">
   <summary>Click for more details</summary>
 
 保存路径在当前目录下的`Log/chat.log`路径中。  
 记录格式为
 
 ```text
```

#### html2text {}

```diff
@@ -1,36 +1,32 @@
-Metadata-Version: 2.1 Name: openai_forward Version: 0.2.3 Summary: ð Openai
-api forward Â· OpenAI æ¥å£è½¬åæå¡ Â· stream forwarding Project-URL:
-Homepage, https://github.com/beidongjiedeguang/openai-forward Project-URL:
-Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-
-forward Project-URL: Issues, https://github.com/beidongjiedeguang/openai-
-forward/issues Project-URL: Source, https://github.com/beidongjiedeguang/
-openai-forward Author-email: kunyuan
+Metadata-Version: 2.1 Name: openai_forward Version: 0.2.4 Summary: ð OpenAI
+API Reverse Proxy Â· ChatGPT API Proxy Project-URL: Homepage, https://
+github.com/beidongjiedeguang/openai-forward Project-URL: Documentation, https:/
+/github.com/beidongjiedeguang/openai-forward#openai-forward Project-URL:
+Issues, https://github.com/beidongjiedeguang/openai-forward/issues Project-URL:
+Source, https://github.com/beidongjiedeguang/openai-forward Author-email:
+kunyuan
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords: OpenAI API
-Forwarding,chatgpt,fastapi,httpx,openai,openai-api,openai-
-proxy,python,streaming-api Classifier: Development Status :: 5 - Production/
-Stable Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python :: 3 Requires-Python: >=3.6 Requires-Dist: fastapi Requires-
-Dist: httpx Requires-Dist: loguru Requires-Dist: orjson Requires-Dist: python-
-dotenv Requires-Dist: pytz Requires-Dist: sparrow-python>=0.1.3 Requires-Dist:
-uvicorn Provides-Extra: bard Requires-Dist: googlebard; extra == 'bard'
-Provides-Extra: chatgpt Requires-Dist: revchatgpt; extra == 'chatgpt' Provides-
-Extra: edge Requires-Dist: edgegpt; extra == 'edge' Provides-Extra: ssl
-Requires-Dist: certbot; extra == 'ssl' Provides-Extra: tool Requires-Dist:
-orjsonl; extra == 'tool' Description-Content-Type: text/markdown **ä¸­æ** |
-[**English**](./README_EN.md)
+Forwarding,chatgpt,fastapi,openai,openai-api,openai-proxy,python,streaming-api
+Classifier: Development Status :: 5 - Production/Stable Classifier: Operating
+System :: OS Independent Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6 Requires-Dist: fastapi Requires-Dist: httpx Requires-
+Dist: loguru Requires-Dist: orjson Requires-Dist: python-dotenv Requires-Dist:
+pytz Requires-Dist: sparrow-python>=0.1.3 Requires-Dist: uvicorn Provides-
+Extra: tool Requires-Dist: orjsonl; extra == 'tool' Description-Content-Type:
+text/markdown **ä¸­æ** | [**English**](./README_EN.md)
                                     ******
                                 OpenAI Forward
                                      ******
                         OpenAI API æ¥å£è½¬åæå¡
                 The fastest way to deploy openai api forwarding
  [PyPI_version] [License] [Release_(latest_by_date)] [GitHub_repo_size] [docer
                 image_size] [tests] [pypi_downloads] [codecov]
    [åè½](#åè½) | [é¨ç½²æå](#é¨ç½²æå) | [åºç¨](#åºç¨) |
-  [éç½®éé¡¹](#éç½®éé¡¹) | [èå¤©æ¥å¿](#èå¤©æ¥å¿) [![Deploy on
+  [éç½®éé¡¹](#éç½®éé¡¹) | [å¯¹è¯æ¥å¿](#å¯¹è¯æ¥å¿) [![Deploy on
     Railway](https://railway.app/button.svg)](https://railway.app/template/
   tejCum?referralCode=U0-kXv) [![Deploy to Render](https://render.com/images/
      deploy-to-render-button.svg)](https://render.com/deploy?repo=https://
                  github.com/beidongjiedeguang/openai-forward)
 æ¬é¡¹ç®ç¨äºè§£å³ä¸äºå°åºæ æ³ç´æ¥è®¿é®OpenAIçé®é¢ï¼å°è¯¥æå¡é¨ç½²å¨å¯ä»¥æ­£å¸¸è®¿é®OpenAI
 APIç(äº)æå¡å¨ä¸ï¼
 éè¿è¯¥æå¡è½¬åOpenAIçè¯·æ±ãå³æ­å»ºååä»£çæå¡;
@@ -38,27 +34,27 @@
 key. --- ç±æ¬é¡¹ç®æ­å»ºçé¿æä»£çå°åï¼ > https://api.openai-
 forward.com ## åè½ **åºç¡åè½** - [x] æ¯æè½¬åOpenAIæææ¥å£ -
 [x] æ¯ææµå¼ååº - [x] æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½²
 - [x] pip å®è£é¨ç½² - [x] cloudflare é¨ç½² - [x] ~~Vercelä¸é®é¨ç½²
 (ä¸å»ºè®®)~~ - [x] Railway ä¸é®é¨ç½² - [x] Render ä¸é®é¨ç½²
 **é«çº§åè½** - [x] åè®¸è¾å¥å¤ä¸ªopenai api key ç»æè½®è¯¢æ±  - [x]
 èªå®ä¹ è½¬åapi key (è§[é«çº§éç½®](#é«çº§éç½®)) - [x]
-å®æ¶è®°å½èå¤©è®°å½(åæ¬æµå¼ååºçèå¤©åå®¹) ## é¨ç½²æå
-[é¨ç½²ææ¡£](deploy.md) æä¾ä»¥ä¸å ç§é¨ç½²æ¹å¼ **ææµ·å¤vpsæ¹æ¡**
-1. [pip å®è£é¨ç½²](deploy.md#pipé¨ç½²) (æ¨è) 2. [Dockeré¨ç½²]
-(deploy.md#dockeré¨ç½²) (æ¨è) > https://api.openai-forward.com
-**æ vpsåè´¹é¨ç½²æ¹æ¡** 1. [ä¸é®Vercelé¨ç½²](deploy.md#vercel-
-ä¸é®é¨ç½²) (ä¸æ¨è) > ~~https://vercel.openai-forward.com~~ 2.
-[cloudflareé¨ç½²](deploy.md#cloudflare-é¨ç½²) (æ¨è) > https://
-cloudflare.openai-forward.com 3. [Railwayé¨ç½²](deploy.md#Railway-
-ä¸é®é¨ç½²) > https://railway.openai-forward.com 4. [Renderä¸é®é¨ç½²]
-(deploy.md#render-ä¸é®é¨ç½²) (è¾æ¨è) > https://render.openai-forward.com
-## åºç¨ ### [èå¤©åºç¨](https://chat.beidongjiedeguang.top)
-åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-
-Web)æ­å»ºèªå·±çchatgptæå¡ æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
+æµå¼ååºå¯¹è¯æ¥å¿ ## é¨ç½²æå [é¨ç½²ææ¡£](deploy.md)
+æä¾ä»¥ä¸å ç§é¨ç½²æ¹å¼ **ææµ·å¤vpsæ¹æ¡** 1. [pip å®è£é¨ç½²]
+(deploy.md#pipé¨ç½²) (æ¨è) 2. [Dockeré¨ç½²](deploy.md#dockeré¨ç½²)
+(æ¨è) > https://api.openai-forward.com **æ vpsåè´¹é¨ç½²æ¹æ¡** 1.
+[ä¸é®Vercelé¨ç½²](deploy.md#vercel-ä¸é®é¨ç½²) (ä¸æ¨è) > ~~https://
+vercel.openai-forward.com~~ 2. [cloudflareé¨ç½²](deploy.md#cloudflare-é¨ç½²)
+(æ¨è) > https://cloudflare.page.openai-forward.com 3. [Railwayé¨ç½²]
+(deploy.md#Railway-ä¸é®é¨ç½²) > https://railway.openai-forward.com 4.
+[Renderä¸é®é¨ç½²](deploy.md#render-ä¸é®é¨ç½²) (æ¨è) > https://
+render.openai-forward.com ## åºç¨ ### [èå¤©åºç¨](https://
+chat.beidongjiedeguang.top) åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web](https://
+github.com/Yidadaa/ChatGPT-Next-Web)æ­å»ºèªå·±çchatgptæå¡
+æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
 `BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å  Click for more details
 ```bash docker run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -
 e BASE_URL="https://api.openai-forward.com" \ -e CODE="kunyuan" \ yidadaa/
 chatgpt-next-web ``` è¿éé¨ç½²äºä¸ä¸ªï¼ä¾å¤§å®¶è½»åº¦ä½¿ç¨: https://
 chat.beidongjiedeguang.top , è®¿é®å¯ç : `kunyuan`  ### å¨ä»£ç ä¸­ä½¿ç¨
 **Python** ```diff import openai + openai.api_base = "https://api.openai-
 forward.com/v1" openai.api_key = "sk-******" ```  More Examples **JS/TS**
@@ -78,27 +74,27 @@
 details **`openai-forward run`åæ°éç½®é¡¹** | éç½®é¡¹ | è¯´æ |
 é»è®¤å¼ | |-----------------|-------------------|:----------------------:| |
 --port | æå¡ç«¯å£å· | 8000 | | --workers | å·¥ä½è¿ç¨æ° | 1 | | --
 base_url | å OPENAI_BASE_URL | https://api.openai.com | | --api_key | å
 OPENAI_API_KEY | `None` | | --forward_key | å FORWARD_KEY | `None` | | --
 route_prefix | å ROUTE_PREFIX | `None` | | --log_chat | å LOG_CHAT |
 `False` |  ### ç¯å¢åééç½®é¡¹
-æ¯æä»è¿è¡ç®å½ä¸ç`.env`æä»¶ä¸­è¯»å  Click for more details |
-ç¯å¢åé | è¯´æ | é»è®¤å¼ | |-----------------|------------------------
+æ¯æä»è¿è¡ç®å½ä¸ç`.env`æä»¶ä¸­è¯»å | ç¯å¢åé | è¯´æ |
+é»è®¤å¼ | |-----------------|------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------------|:------------------------:| | OPENAI_BASE_URL |
-é»è®¤ openaiå®æ¹ api å°å | https://api.openai.com | | OPENAI_API_KEY |
-é»è®¤openai api keyï¼æ¯æå¤ä¸ªé»è®¤api key, ä»¥ `sk-` å¼å¤´ï¼
-ä»¥ç©ºæ ¼åå² | æ  | | FORWARD_KEY | åè®¸è°ç¨æ¹ä½¿ç¨è¯¥keyä»£æ¿openai
-api keyï¼æ¯æå¤ä¸ªforward key, ä»¥ç©ºæ ¼åå²;
+----|:------------------------:| | OPENAI_BASE_URL | é»è®¤ openaiå®æ¹ api
+å°å | https://api.openai.com | | OPENAI_API_KEY | é»è®¤openai api
+keyï¼æ¯æå¤ä¸ªé»è®¤api key, ä»¥ `sk-` å¼å¤´ï¼ ä»¥ç©ºæ ¼åå² | æ  | |
+FORWARD_KEY | åè®¸è°ç¨æ¹ä½¿ç¨è¯¥keyä»£æ¿openai api
+keyï¼æ¯æå¤ä¸ªforward key, ä»¥ç©ºæ ¼åå²;
 å¦æè®¾ç½®äºOPENAI_API_KEYï¼èæ²¡æè®¾ç½®FORWARD_KEY,
 åå®¢æ·ç«¯è°ç¨æ¶æ éæä¾å¯é¥,
 æ­¤æ¶åºäºå®å¨èèä¸å»ºè®®FORWARD_KEYç½®ç©º | æ  | | ROUTE_PREFIX |
-è·¯ç±åç¼ | æ  | | LOG_CHAT | æ¯å¦è®°å½èå¤©åå®¹ | `false` |  ##
-é«çº§éç½® **è®¾ç½®api_keyä¸ºèªå·±è®¾ç½®çforward key** éè¦éç½®
+è·¯ç±åç¼ | æ  | | LOG_CHAT | æ¯å¦è®°å½èå¤©åå®¹ | `false` | ##
+é«çº§éç½® **è®¾ç½®openai api_keyä¸ºèªå®ä¹çforward key** éè¦éç½®
 OPENAI_API_KEY å FORWARD_KEY, ä¾å¦  Click for more details ```bash
 OPENAI_API_KEY=sk-******* FORWARD_KEY=fk-****** # è¿éfk-
 tokenç±æä»¬èªå·±å®ä¹ ``` è¿éæä»¬éç½®äºFORWARD_KEYä¸º`fk-******`,
 é£ä¹åé¢å®¢æ·ç«¯å¨è°ç¨æ¶åªéè®¾ç½®OPENAI_API_KEYä¸ºæä»¬èªå®ä¹ç`fk-
 ******` å³å¯ã
 è¿æ ·çå¥½å¤æ¯å¨ä½¿ç¨ä¸äºéè¦è¾å¥OPENAI_API_KEYçç¬¬ä¸æ¹åºç¨æ¶ï¼æä»¬å¯ä»¥ä½¿ç¨`fk-
 ******`æ­éä»£çæå¡ä½¿ç¨ï¼å¦ä¸é¢çä¾å­ï¼
@@ -106,16 +102,16 @@
 **ç¨ä¾:** ```bash curl https://api.openai-forward.com/v1/chat/completions \ -
 H "Content-Type: application/json" \ -H "Authorization: Bearer fk-******" \ -
 d '{ "model": "gpt-3.5-turbo", "messages": [{"role": "user", "content":
 "Hello!"}] }' ``` **Python** ```diff import openai + openai.api_base = "https:/
 /api.openai-forward.com/v1" - openai.api_key = "sk-******" + openai.api_key =
 "fk-******" ``` **Web application** ```bash docker run -d \ -p 3000:3000 \ -
 e OPENAI_API_KEY="fk-******" \ -e BASE_URL="https://api.openai-forward.com" \ -
-e CODE="" \ yidadaa/chatgpt-next-web ```  ## èå¤©æ¥å¿
-é»è®¤ä¸è®°å½èå¤©æ¥å¿ï¼è¥è¦å¼å¯éè®¾ç½®ç¯å¢åé`LOG_CHAT=true`
+e CODE="" \ yidadaa/chatgpt-next-web ```  ## å¯¹è¯æ¥å¿
+é»è®¤ä¸è®°å½å¯¹è¯æ¥å¿ï¼è¥è¦å¼å¯éè®¾ç½®ç¯å¢åé`LOG_CHAT=true`
 Click for more details ä¿å­è·¯å¾å¨å½åç®å½ä¸ç`Log/
 chat.log`è·¯å¾ä¸­ã è®°å½æ ¼å¼ä¸º ```text {'messages': [{'user': 'hi'}],
 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': '467a17ec-bf39-4b65-9ebd-
 e722b3bdd5c3'} {'assistant': 'Hello! How can I assist you today?', 'uid':
 '467a17ec-bf39-4b65-9ebd-e722b3bdd5c3'} {'messages': [{'user': 'Hello!'}],
 'model': 'gpt-3.5-turbo', 'forwarded-for': '', 'uid': 'f844d156-e747-4887-aef8-
 e40d977b5ee7'} {'assistant': 'Hi there! How can I assist you today?', 'uid':
```

