# Comparing `tmp/TeenStudy-0.1.9.tar.gz` & `tmp/TeenStudy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TeenStudy-0.1.9.tar", max compression
+gzip compressed data, was "TeenStudy-0.2.0.tar", max compression
```

## Comparing `TeenStudy-0.1.9.tar` & `TeenStudy-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,41 @@
--rw-r--r--   0        0        0     1084 2023-05-20 16:35:19.074377 TeenStudy-0.1.9/LICENSE
--rw-r--r--   0        0        0     1002 2023-05-20 16:36:15.517840 TeenStudy-0.1.9/pyproject.toml
--rw-r--r--   0        0        0    10598 2023-05-20 17:11:32.317080 TeenStudy-0.1.9/README.md
--rw-r--r--   0        0        0      666 2023-05-20 16:35:19.076378 TeenStudy-0.1.9/TeenStudy/__init__.py
--rw-r--r--   0        0        0       28 2023-05-20 16:35:19.076378 TeenStudy-0.1.9/TeenStudy/models/__init__.py
--rw-r--r--   0        0        0     3547 2023-05-20 16:35:19.076378 TeenStudy-0.1.9/TeenStudy/models/accuont.py
--rw-r--r--   0        0        0     3621 2023-05-20 16:35:19.077425 TeenStudy-0.1.9/TeenStudy/models/dxx.py
--rw-r--r--   0        0        0   881164 2023-05-20 16:35:19.134720 TeenStudy-0.1.9/TeenStudy/resource/answer.png
--rw-r--r--   0        0        0    52240 2023-05-20 16:35:19.135720 TeenStudy-0.1.9/TeenStudy/resource/backgroud1.jpg
--rw-r--r--   0        0        0    52119 2023-05-20 16:35:19.136721 TeenStudy-0.1.9/TeenStudy/resource/backgroud2.jpg
--rw-r--r--   0        0        0    52136 2023-05-20 16:35:19.136721 TeenStudy-0.1.9/TeenStudy/resource/backgroud3.jpg
--rw-r--r--   0        0        0    51874 2023-05-20 16:35:19.137721 TeenStudy-0.1.9/TeenStudy/resource/backgroud4.jpg
--rw-r--r--   0        0        0    51634 2023-05-20 16:35:19.137721 TeenStudy-0.1.9/TeenStudy/resource/backgroud5.jpg
--rw-r--r--   0        0        0 10424793 2023-05-20 16:35:19.169356 TeenStudy-0.1.9/TeenStudy/resource/dxx_jx.json
--rw-r--r--   0        0        0  7977480 2023-05-20 16:35:19.131719 TeenStudy-0.1.9/TeenStudy/resource/MiSans-Light.ttf
--rw-r--r--   0        0        0      121 2023-05-20 16:35:19.170651 TeenStudy-0.1.9/TeenStudy/utils/__init__.py
--rw-r--r--   0        0        0    54138 2023-05-20 16:55:34.498100 TeenStudy-0.1.9/TeenStudy/utils/dxx.py
--rw-r--r--   0        0        0    18819 2023-05-20 16:35:19.171671 TeenStudy-0.1.9/TeenStudy/utils/handle.py
--rw-r--r--   0        0        0     4331 2023-05-20 16:35:19.171671 TeenStudy-0.1.9/TeenStudy/utils/path.py
--rw-r--r--   0        0        0     2026 2023-05-20 16:35:19.172718 TeenStudy-0.1.9/TeenStudy/utils/rule.py
--rw-r--r--   0        0        0    10411 2023-05-20 16:35:19.172718 TeenStudy-0.1.9/TeenStudy/utils/update.py
--rw-r--r--   0        0        0    24243 2023-05-20 16:57:33.116329 TeenStudy-0.1.9/TeenStudy/utils/utils.py
--rw-r--r--   0        0        0     2185 2023-05-20 16:35:19.174802 TeenStudy-0.1.9/TeenStudy/web/__init__.py
--rw-r--r--   0        0        0      396 2023-05-20 16:35:19.174802 TeenStudy-0.1.9/TeenStudy/web/api/__init__.py
--rw-r--r--   0        0        0    46020 2023-05-20 17:00:14.593604 TeenStudy-0.1.9/TeenStudy/web/api/add.py
--rw-r--r--   0        0        0    11925 2023-05-20 16:35:19.175806 TeenStudy-0.1.9/TeenStudy/web/api/admin.py
--rw-r--r--   0        0        0     4706 2023-05-20 16:35:19.175806 TeenStudy-0.1.9/TeenStudy/web/api/home.py
--rw-r--r--   0        0        0     6317 2023-05-20 16:35:19.176809 TeenStudy-0.1.9/TeenStudy/web/api/login.py
--rw-r--r--   0        0        0       78 2023-05-20 16:35:19.176809 TeenStudy-0.1.9/TeenStudy/web/pages/__init__.py
--rw-r--r--   0        0        0    38893 2023-05-20 16:59:29.116308 TeenStudy-0.1.9/TeenStudy/web/pages/add.py
--rw-r--r--   0        0        0    73709 2023-05-20 17:01:52.359960 TeenStudy-0.1.9/TeenStudy/web/pages/admin.py
--rw-r--r--   0        0        0    17385 2023-05-20 16:35:19.177813 TeenStudy-0.1.9/TeenStudy/web/pages/home.py
--rw-r--r--   0        0        0     1731 2023-05-20 16:35:19.177813 TeenStudy-0.1.9/TeenStudy/web/pages/login.py
--rw-r--r--   0        0        0       24 2023-05-20 16:35:19.179316 TeenStudy-0.1.9/TeenStudy/web/utils/__init__.py
--rw-r--r--   0        0        0     1902 2023-05-20 16:35:19.179316 TeenStudy-0.1.9/TeenStudy/web/utils/add.py
--rw-r--r--   0        0        0     2240 2023-05-20 16:35:19.180340 TeenStudy-0.1.9/TeenStudy/web/utils/status.py
--rw-r--r--   0        0        0    12060 1970-01-01 00:00:00.000000 TeenStudy-0.1.9/setup.py
--rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 TeenStudy-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-20 16:35:19.074377 TeenStudy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1022 2023-06-11 16:37:37.159481 TeenStudy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11618 2023-06-11 16:51:10.986157 TeenStudy-0.2.0/README.md
+-rw-r--r--   0        0        0      799 2023-06-09 14:41:48.014472 TeenStudy-0.2.0/TeenStudy/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-06 04:08:57.732319 TeenStudy-0.2.0/TeenStudy/models/__init__.py
+-rw-r--r--   0        0        0     3547 2023-05-06 04:08:57.733777 TeenStudy-0.2.0/TeenStudy/models/accuont.py
+-rw-r--r--   0        0        0     2864 2023-05-20 08:30:39.830063 TeenStudy-0.2.0/TeenStudy/models/dxx.py
+-rw-r--r--   0        0        0   881164 2023-05-06 04:08:57.790011 TeenStudy-0.2.0/TeenStudy/resource/answer.png
+-rw-r--r--   0        0        0    52240 2023-05-06 04:08:57.791011 TeenStudy-0.2.0/TeenStudy/resource/backgroud1.jpg
+-rw-r--r--   0        0        0    52119 2023-05-06 04:08:57.792437 TeenStudy-0.2.0/TeenStudy/resource/backgroud2.jpg
+-rw-r--r--   0        0        0    52136 2023-05-06 04:08:57.792437 TeenStudy-0.2.0/TeenStudy/resource/backgroud3.jpg
+-rw-r--r--   0        0        0    51874 2023-05-06 04:08:57.793437 TeenStudy-0.2.0/TeenStudy/resource/backgroud4.jpg
+-rw-r--r--   0        0        0    51634 2023-05-06 04:08:57.793437 TeenStudy-0.2.0/TeenStudy/resource/backgroud5.jpg
+-rw-r--r--   0        0        0 10424793 2023-05-20 16:35:19.169356 TeenStudy-0.2.0/TeenStudy/resource/dxx_jx.json
+-rw-r--r--   0        0        0  7977480 2023-05-06 04:08:57.787010 TeenStudy-0.2.0/TeenStudy/resource/MiSans-Light.ttf
+-rw-r--r--   0        0        0      121 2023-05-06 04:08:57.826444 TeenStudy-0.2.0/TeenStudy/utils/__init__.py
+-rw-r--r--   0        0        0    57274 2023-06-11 15:32:19.818471 TeenStudy-0.2.0/TeenStudy/utils/dxx.py
+-rw-r--r--   0        0        0    18836 2023-06-11 16:56:02.826779 TeenStudy-0.2.0/TeenStudy/utils/handle.py
+-rw-r--r--   0        0        0     4331 2023-05-06 08:28:06.723801 TeenStudy-0.2.0/TeenStudy/utils/path.py
+-rw-r--r--   0        0        0     2442 2023-06-11 09:56:43.495843 TeenStudy-0.2.0/TeenStudy/utils/rule.py
+-rw-r--r--   0        0        0    10411 2023-06-09 15:26:04.222499 TeenStudy-0.2.0/TeenStudy/utils/update.py
+-rw-r--r--   0        0        0    21537 2023-06-11 14:36:10.552923 TeenStudy-0.2.0/TeenStudy/utils/utils.py
+-rw-r--r--   0        0        0     2276 2023-06-11 15:56:06.759418 TeenStudy-0.2.0/TeenStudy/web/__init__.py
+-rw-r--r--   0        0        0      468 2023-06-09 16:00:15.975770 TeenStudy-0.2.0/TeenStudy/web/api/__init__.py
+-rw-r--r--   0        0        0    39320 2023-06-11 15:55:25.777627 TeenStudy-0.2.0/TeenStudy/web/api/add.py
+-rw-r--r--   0        0        0    11925 2023-05-06 04:08:57.831445 TeenStudy-0.2.0/TeenStudy/web/api/admin.py
+-rw-r--r--   0        0        0     4833 2023-06-10 08:09:47.464413 TeenStudy-0.2.0/TeenStudy/web/api/home.py
+-rw-r--r--   0        0        0     1450 2023-06-10 07:35:31.894315 TeenStudy-0.2.0/TeenStudy/web/api/log.py
+-rw-r--r--   0        0        0     5337 2023-06-10 08:09:47.467430 TeenStudy-0.2.0/TeenStudy/web/api/login.py
+-rw-r--r--   0        0        0      116 2023-06-10 10:38:18.685378 TeenStudy-0.2.0/TeenStudy/web/pages/__init__.py
+-rw-r--r--   0        0        0    30258 2023-06-11 15:46:44.026339 TeenStudy-0.2.0/TeenStudy/web/pages/add.py
+-rw-r--r--   0        0        0    46167 2023-06-11 15:58:49.021540 TeenStudy-0.2.0/TeenStudy/web/pages/addArea.py
+-rw-r--r--   0        0        0    23573 2023-06-11 15:58:08.477011 TeenStudy-0.2.0/TeenStudy/web/pages/admin.py
+-rw-r--r--   0        0        0    18318 2023-06-11 15:58:08.473417 TeenStudy-0.2.0/TeenStudy/web/pages/home.py
+-rw-r--r--   0        0        0     2112 2023-06-10 05:56:03.204971 TeenStudy-0.2.0/TeenStudy/web/pages/log.py
+-rw-r--r--   0        0        0     2029 2023-06-10 08:23:43.305225 TeenStudy-0.2.0/TeenStudy/web/pages/login.py
+-rw-r--r--   0        0        0       24 2023-05-06 04:08:57.834965 TeenStudy-0.2.0/TeenStudy/web/utils/__init__.py
+-rw-r--r--   0        0        0     2223 2023-06-10 10:55:00.537866 TeenStudy-0.2.0/TeenStudy/web/utils/add.py
+-rw-r--r--   0        0        0     2240 2023-05-06 04:08:57.835965 TeenStudy-0.2.0/TeenStudy/web/utils/status.py
+-rw-r--r--   0        0        0    13106 1970-01-01 00:00:00.000000 TeenStudy-0.2.0/setup.py
+-rw-r--r--   0        0        0    12849 1970-01-01 00:00:00.000000 TeenStudy-0.2.0/PKG-INFO
```

### Comparing `TeenStudy-0.1.9/LICENSE` & `TeenStudy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/pyproject.toml` & `TeenStudy-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "TeenStudy"
-version = "0.1.9"
+version = "0.2.0"
 description = "基于nonebot2异步框架的青年大学自动提交插件基于nonebot2的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图"
 authors = ["ZM25XC <xingling25@qq.com>"]
 license="MIT"
 readme="README.md"
 homepage="https://github.com/ZM25XC/TeenStudy"
 packages = [
   { include = "teenstudy" },
@@ -12,25 +12,26 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 amis-python="^1.0.7"
 anti-useragent="^1.0.10"
 beautifulsoup4="^4.11.2"
 bs4="^0.0.1"
 fastapi="^0.95.0,<1.0.0"
-httpx="^0.23.3,<1.0.0"
+httpx="^0.24.0,<1.0.0"
 Jinja2="^3.1.2"
 lxml="^4.9.2"
-nonebot-adapter-onebot="^2.2.1"
-nonebot-plugin-apscheduler="^0.2.0"
-nonebot2="^2.0.0rc2"
-Pillow="^9.4.0"
+nonebot-adapter-onebot="^2.2.3"
+nonebot-plugin-apscheduler="^0.3.0"
+nonebot2="^2.0.0"
+ddddocr="^1.4.7"
 python-jose="^3.3.0"
 tortoise-orm="^0.19.3"
 ujson="^5.7.0"
 uvicorn="^0.21.0,<1.0.0"
 qrcode="^7.4.2"
 psutil="^5.9.4"
+pycryptodome="^3.17"
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `TeenStudy-0.1.9/README.md` & `TeenStudy-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 <div align="center">
-    <img src="https://i.328888.xyz/2023/02/28/z23ho.png" alt="TeenStudy.png" border="0" width="500px" height="500px"/>
+    <img src="https://img1.imgtp.com/2023/06/11/sG4KdlpL.png" alt="TeenStudy.png" border="0" width="500px" height="500px"/>
     <h1>TeenStudy</h1>
     <b>基于nonebot2和go-cqhttp的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图</b>
     <br/>
     <a href="https://github.com/ZM25XC/TeenStudy/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/ZM25XC/TeenStudy?style=flat-square"></a>
     <a href="https://github.com/ZM25XC/TeenStudy/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/ZM25XC/TeenStudy?style=flat-square"></a>
     <a href="https://github.com/ZM25XC/TeenStudy/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/ZM25XC/TeenStudy?style=flat-square"></a>
     <a href="https://pypi.python.org/pypi/TeenStudy"><img src="https://img.shields.io/pypi/v/TeenStudy?color=yellow" alt="pypi"></a>
   	<a href="https://pypi.python.org/pypi/TeenStudy">
     <img src="https://img.shields.io/pypi/dm/TeenStudy" alt="pypi download"></a>
 	  <a href="https://github.com/ZM25XC/TeenStudy/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/ZM25XC/TeenStudy?style=flat-square"></a>
     <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS">
-    <img src="https://img.shields.io/badge/QQ%E7%BE%A4-511173803-orange?style=flat-square" alt="QQ Chat Group">
+    <img src="https://img.shields.io/badge/QQ反馈群-511173803-orange?style=flat-square" alt="QQ Chat Group">
+  </a>
+	<a href="http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm">
+    <img src="https://img.shields.io/badge/QQ体验群-821280615-orange?style=flat-square" alt="QQ Chat Group">
   </a>
   </div>
 
 ## 说明
 
 - 本项目为[青年大学习提交](https://github.com/ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`版
 - 本项目基于[nonebot2](https://github.com/nonebot/nonebot2)和[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)，使用本插件前请先阅读以上两个项目的使用文档
 -  **启动插件之后，一定要登录后台在推送列表中添加需要开启大学习功能的群聊**
 -  **本项目无法在国外IP环境下使用，如有开启代理，请关闭或添加代理规则**
 - 需要抓包的地区，绑定后尽量别进官方公众号，避免token或cookie刷新导致无法提交
 - 本项目需要部署在公网可访问的容器中，并开放端口（nonebot2配置的port），否则大部分功能将出现异常
-- 欢迎加入[QQ群](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)，交流讨论。
+- 欢迎加入[QQ反馈群](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)，交流讨论，如您不会搭建又想每周自动提交，可加入[QQ体验群](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm)。
 - 时间精力有限，目前只维护湖北和江西两个地区，其他地区出问题请提交Issues,我找个时间修，需要增加地区请进群帮忙测试，个别地区没账号无法测试
 
 - 觉得项目不错，不妨点个stars.
 
 ## 地区状态
 
 <details>
 
 | 共青团名称 | 开发状态 | 备注 |
 |:-----:|:----:|:----:|
 |青春湖北|支持|无需抓包|
 |江西共青团|支持|无需抓包|
 |安徽共青团|支持|无需抓包|
 |广东共青团|支持|无需抓包|
+|青春北京|支持|无需抓包|
 |青春上海|支持|微信扫码绑定|
 |青春浙江|支持|微信扫码绑定|
-|江苏共青团|支持|需要自行抓包|
+|津彩青春|支持|需要自行抓包|
 |青春山东|支持|需要自行抓包|
 |重庆共青团|支持|需要自行抓包|
 |吉青飞扬|支持|需要自行抓包|
-|黑龙江共青团|支持|需要自行抓包，该地区上线测试中|
 |天府新青年|支持|不进入公众号token时效大于1周|
 |河南共青团|不支持|cookie时效小于1周|
+|江苏共青团|不支持|cookie失效小于1周|
+|黑龙江共青团|不支持|cookie失效小于1周|
 |广西青年圈|待开发||
 |青春湖南|待开发||
 |甘肃青年|待开发||
 |山西青年|待开发||
 |河北共青团|待开发||
 |福建共青团|待开发||
 |内蒙古青年|待开发||
 |云南共青团|待开发||
 |三秦青年|待开发||
-|青春北京|待开发||
 |海南共青团|待开发||
-|津彩青春|待开发||
 |青春黔言|待开发||
 |青春柳州|待开发||
 |辽宁共青团|待开发||
 |宁夏共青团|待开发||
 |新疆共青团|待开发||
 |西藏共青团|待开发||
 </details>
@@ -156,18 +159,36 @@
 
 - [ ] 增加更多地区支持
 - [ ] 优化 Bot
 
 
 ## 更新日志
 
-### 2023/05/21
+### 2023/06/12
+
+- 适配北京地区，无需抓包
+- 增加天津地区，需要自行抓包
+- 因江苏和黑龙江地区Cookie时效小于1周，移除江苏和黑龙江地区
+- Web UI添加日志和主动退出功能
+- 更新江西地区拉取团支部数据方式，移除缓存团支部数据，包体积减小50%
+- 修复大学习公网检测失败问题
+- 更新Nonebot2强制meta字段
+- 同步UI依赖AMIS版本到最新版本
+- 开放体验群，不会搭建又想使用的可加[QQ体验群](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm)
+  
+
+<details>
+
+<summary>2023/05/21</summary>
 
 - 增加黑龙江地区，需要自行抓包，该地区上线测试中，请积极提issue反馈
 - 下版本为大版本更新，将添加新功能，优化功能，请积极提issue反馈或加交流群反馈
+- 
+</details>
+
 
 <details>
 <summary>2023/05/11</summary> 
 
 - 增加广东地区，无需抓包[#13](https://github.com/ZM25XC/TeenStudy/issues/13)，感谢[@neal240](https://github.com/neal240)提供账号测试
 
 </details>
```

#### html2text {}

```diff
@@ -1,46 +1,49 @@
                                 [TeenStudy.png]
                             ****** TeenStudy ******
                              åºäºnonebot2ågo-
 cqhttpçéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾
 
  [GitHub_issues] [GitHub_forks] [GitHub_stars] [pypi] [pypi_download] [GitHub
-                           license] [QQ_Chat_Group]
+                   license] [QQ_Chat_Group] [QQ_Chat_Group]
 ## è¯´æ - æ¬é¡¹ç®ä¸º[éå¹´å¤§å­¦ä¹ æäº¤](https://github.com/ZM25XC/
 nonebot_plugin_auto_teenstudy) `Web UI`ç - æ¬é¡¹ç®åºäº[nonebot2](https://
 github.com/nonebot/nonebot2)å[go-cqhttp](https://github.com/Mrs4s/go-
 cqhttp)ï¼ä½¿ç¨æ¬æä»¶åè¯·åéè¯»ä»¥ä¸ä¸¤ä¸ªé¡¹ç®çä½¿ç¨ææ¡£ -
 **å¯å¨æä»¶ä¹åï¼ä¸å®è¦ç»å½åå°å¨æ¨éåè¡¨ä¸­æ·»å éè¦å¼å¯å¤§å­¦ä¹ åè½çç¾¤è**
 -
 **æ¬é¡¹ç®æ æ³å¨å½å¤IPç¯å¢ä¸ä½¿ç¨ï¼å¦æå¼å¯ä»£çï¼è¯·å³é­ææ·»å ä»£çè§å**
 -
 éè¦æåçå°åºï¼ç»å®åå°½éå«è¿å®æ¹å¬ä¼å·ï¼é¿åtokenæcookieå·æ°å¯¼è´æ æ³æäº¤
 -
 æ¬é¡¹ç®éè¦é¨ç½²å¨å¬ç½å¯è®¿é®çå®¹å¨ä¸­ï¼å¹¶å¼æ¾ç«¯å£ï¼nonebot2éç½®çportï¼ï¼å¦åå¤§é¨ååè½å°åºç°å¼å¸¸
-- æ¬¢è¿å å¥[QQç¾¤](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)ï¼äº¤æµè®¨è®ºã
--
+- æ¬¢è¿å å¥[QQåé¦ç¾¤](https://jq.qq.com/
+?_wv=1027&k=NGFEwXyS)ï¼äº¤æµè®¨è®ºï¼å¦æ¨ä¸ä¼æ­å»ºåæ³æ¯å¨èªå¨æäº¤ï¼å¯å å¥
+[QQä½éªç¾¤](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-
+ai2aPGToBKm)ã -
 æ¶é´ç²¾åæéï¼ç®ååªç»´æ¤æ¹ååæ±è¥¿ä¸¤ä¸ªå°åºï¼å¶ä»å°åºåºé®é¢è¯·æäº¤Issues,ææ¾ä¸ªæ¶é´ä¿®ï¼éè¦å¢å å°åºè¯·è¿ç¾¤å¸®å¿æµè¯ï¼ä¸ªå«å°åºæ²¡è´¦å·æ æ³æµè¯
 - è§å¾é¡¹ç®ä¸éï¼ä¸å¦¨ç¹ä¸ªstars. ## å°åºç¶æ  | å±éå¢åç§° |
 å¼åç¶æ | å¤æ³¨ | |:-----:|:----:|:----:
 | |éæ¥æ¹å|æ¯æ|æ éæå| |æ±è¥¿å±éå¢|æ¯æ|æ éæå|
 |å®å¾½å±éå¢|æ¯æ|æ éæå| |å¹¿ä¸å±éå¢|æ¯æ|æ éæå|
-|éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
+|éæ¥åäº¬|æ¯æ|æ éæå| |éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
 |éæ¥æµæ±|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
-|æ±èå±éå¢|æ¯æ|éè¦èªè¡æå|
+|æ´¥å½©éæ¥|æ¯æ|éè¦èªè¡æå|
 |éæ¥å±±ä¸|æ¯æ|éè¦èªè¡æå|
 |éåºå±éå¢|æ¯æ|éè¦èªè¡æå|
 |åéé£æ¬|æ¯æ|éè¦èªè¡æå|
-|é»é¾æ±å±éå¢|æ¯æ|éè¦èªè¡æåï¼è¯¥å°åºä¸çº¿æµè¯ä¸­|
 |å¤©åºæ°éå¹´|æ¯æ|ä¸è¿å¥å¬ä¼å·tokenæ¶æå¤§äº1å¨|
-|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨| |å¹¿è¥¿éå¹´å|å¾å¼å||
-|éæ¥æ¹å|å¾å¼å|| |çèéå¹´|å¾å¼å|| |å±±è¥¿éå¹´|å¾å¼å||
+|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨|
+|æ±èå±éå¢|ä¸æ¯æ|cookieå¤±æå°äº1å¨|
+|é»é¾æ±å±éå¢|ä¸æ¯æ|cookieå¤±æå°äº1å¨|
+|å¹¿è¥¿éå¹´å|å¾å¼å|| |éæ¥æ¹å|å¾å¼å||
+|çèéå¹´|å¾å¼å|| |å±±è¥¿éå¹´|å¾å¼å||
 |æ²³åå±éå¢|å¾å¼å|| |ç¦å»ºå±éå¢|å¾å¼å||
 |åèå¤éå¹´|å¾å¼å|| |äºåå±éå¢|å¾å¼å||
-|ä¸ç§¦éå¹´|å¾å¼å|| |éæ¥åäº¬|å¾å¼å||
-|æµ·åå±éå¢|å¾å¼å|| |æ´¥å½©éæ¥|å¾å¼å||
+|ä¸ç§¦éå¹´|å¾å¼å|| |æµ·åå±éå¢|å¾å¼å||
 |éæ¥é»è¨|å¾å¼å|| |éæ¥æ³å·|å¾å¼å||
 |è¾½å®å±éå¢|å¾å¼å|| |å®å¤å±éå¢|å¾å¼å||
 |æ°çå±éå¢|å¾å¼å|| |è¥¿èå±éå¢|å¾å¼å||  ## å®è£åæ´æ°
 ç¬¬ä¸ç§æ¹å¼(ä¸æ¨è) - ä½¿ç¨`git clone https://github.com/ZM25XC/
 TeenStudy.git`æä»¤åéæ¬ä»åºæä¸è½½åç¼©åæä»¶   ç¬¬äºç§æ¹å¼
 (äºéä¸) - ä½¿ç¨`pip install TeenStudy`æ¥è¿è¡å®è£,ä½¿ç¨`pip install
 TeenStudy -U`è¿è¡æ´æ° - ä½¿ç¨`nb plugin install
@@ -76,20 +79,29 @@
 UIé»è®¤éç½® | | éç½®å¯ç  | éç½®å¯ç  | éç½®ç»å½Web
 UIçå¯ç ä¸ºç¨æ·ID |
 |å é¤å¤§å­¦ä¹ |å é¤å¤§å­¦ä¹ |ç¨æ·ç³è¯·æ¸é¤æ°æ®åºçä¿¡æ¯|
 |å¯¼åºç¨æ·æ°æ®|å¯¼åºç¨æ·æ°æ®ãå¯¼åºæ°æ®|å°æ°æ®å¯¼åºè³TeenStudyç®å½ä¸|
 |æ´æ°ç¨æ·æ°æ®|æ´æ°ç¨æ·æ°æ®ãå·æ°ç¨æ·æ°æ®|å°ç¨æ·æ°æ®å¯¼å¥å°æ°æ®åº|
 |æ´æ°èµæºæ°æ®|æ´æ°èµæºæ°æ®ãå·æ°èµæºæ°æ®|æ´æ°æ°æ®åºä¸­çèµæºæ°æ®ï¼æ±è¥¿å±éå¢å¢æ¯é¨æ°æ®ï¼|
 ## ToDo - [ ] å¢å æ´å¤å°åºæ¯æ - [ ] ä¼å Bot ## æ´æ°æ¥å¿ ###
-2023/05/21 -
+2023/06/12 - ééåäº¬å°åºï¼æ éæå -
+å¢å å¤©æ´¥å°åºï¼éè¦èªè¡æå -
+å æ±èåé»é¾æ±å°åºCookieæ¶æå°äº1å¨ï¼ç§»é¤æ±èåé»é¾æ±å°åº
+- Web UIæ·»å æ¥å¿åä¸»å¨éåºåè½ -
+æ´æ°æ±è¥¿å°åºæåå¢æ¯é¨æ°æ®æ¹å¼ï¼ç§»é¤ç¼å­å¢æ¯é¨æ°æ®ï¼åä½ç§¯åå°50%
+- ä¿®å¤å¤§å­¦ä¹ å¬ç½æ£æµå¤±è´¥é®é¢ - æ´æ°Nonebot2å¼ºå¶metaå­æ®µ -
+åæ­¥UIä¾èµAMISçæ¬å°ææ°çæ¬ -
+å¼æ¾ä½éªç¾¤ï¼ä¸ä¼æ­å»ºåæ³ä½¿ç¨çå¯å [QQä½éªç¾¤](http://
+qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm)  2023/05/
+21 -
 å¢å é»é¾æ±å°åºï¼éè¦èªè¡æåï¼è¯¥å°åºä¸çº¿æµè¯ä¸­ï¼è¯·ç§¯ææissueåé¦
 -
 ä¸çæ¬ä¸ºå¤§çæ¬æ´æ°ï¼å°æ·»å æ°åè½ï¼ä¼ååè½ï¼è¯·ç§¯ææissueåé¦æå äº¤æµç¾¤åé¦
-2023/05/11 - å¢å å¹¿ä¸å°åºï¼æ éæå[#13](https://github.com/ZM25XC/
-TeenStudy/issues/13)ï¼æè°¢[@neal240](https://github.com/
+-   2023/05/11 - å¢å å¹¿ä¸å°åºï¼æ éæå[#13](https://github.com/
+ZM25XC/TeenStudy/issues/13)ï¼æè°¢[@neal240](https://github.com/
 neal240)æä¾è´¦å·æµè¯   2023/05/06 -
 å¢å åæå°åºï¼éè¦èªè¡æå -
 ä¿®å¤è¶ç®¡æ´æ¹ç»å½å¯ç åç¨åå¯ç è½ç»§ç»­ç»å½é®é¢ -
 æ·»å äºç»´ç è½¬é¾æ¥å¼å³ï¼éè¦èªè¡å¨åå°éç½®é¡µé¢æå¼ -
 è°æ´é¨åä¾èµ    2023/04/12 -
 å æ²³åå°åºcookieæ¶æå°äº1å¨ï¼ç§»é¤æ²³åå°åº -
 æ·»å `å é¤å¤§å­¦ä¹ `åè½ï¼ç¨æ·å¯èªè¡å é¤æ°æ® -
```

### Comparing `TeenStudy-0.1.9/TeenStudy/models/accuont.py` & `TeenStudy-0.2.0/TeenStudy/models/accuont.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/models/dxx.py` & `TeenStudy-0.2.0/TeenStudy/models/dxx.py`

 * *Files 14% similar despite different names*

```diff
@@ -70,38 +70,14 @@
 
     class Meta:
         table = 'Resource'
         table_description = '大学习插件资源'
         indexes = ('time',)
 
 
-class JiangXi(Model):
-    id: int = fields.IntField(pk=True, generated=True, auto_increment=True)
-    """自增主键，数据库ID"""
-    time: int = fields.IntField()
-    """创建时间"""
-    university_id: str = fields.TextField(null=True)
-    """学校id"""
-    university: str = fields.TextField()
-    """学校名称"""
-    college_id: str = fields.TextField(null=True)
-    """学院id"""
-    college: str = fields.TextField()
-    """学院名称"""
-    organization = fields.TextField(null=True)
-    """团支部"""
-    organization_id: str = fields.TextField(null=True)
-    """团支部id"""
-
-    class Meta:
-        table = 'JiangXi'
-        table_description = '江西地区团支部数据'
-        indexes = ('time',)
-
-
 class PushList(Model):
     id: int = fields.IntField(pk=True, generated=True, auto_increment=True)
     """自增主键，数据库ID"""
     time: int = fields.IntField()
     """创建时间"""
     self_id: int = fields.IntField()
     """机器人Id"""
```

### Comparing `TeenStudy-0.1.9/TeenStudy/resource/answer.png` & `TeenStudy-0.2.0/TeenStudy/resource/answer.png`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/resource/backgroud1.jpg` & `TeenStudy-0.2.0/TeenStudy/resource/backgroud1.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/resource/backgroud2.jpg` & `TeenStudy-0.2.0/TeenStudy/resource/backgroud2.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/resource/backgroud3.jpg` & `TeenStudy-0.2.0/TeenStudy/resource/backgroud3.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/resource/backgroud4.jpg` & `TeenStudy-0.2.0/TeenStudy/resource/backgroud4.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/resource/backgroud5.jpg` & `TeenStudy-0.2.0/TeenStudy/resource/backgroud5.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/resource/dxx_jx.json` & `TeenStudy-0.2.0/TeenStudy/resource/dxx_jx.json`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/resource/MiSans-Light.ttf` & `TeenStudy-0.2.0/TeenStudy/resource/MiSans-Light.ttf`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/utils/dxx.py` & `TeenStudy-0.2.0/TeenStudy/utils/dxx.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 import random
 import re
 import secrets
 import time
 import urllib.parse
 
 from anti_useragent import UserAgent
+from bs4 import BeautifulSoup
+from ddddocr import DdddOcr
 from httpx import AsyncClient
 from nonebot import logger
 
+from .utils import encrypt
 from ..models.accuont import User, Commit
 from ..models.dxx import Answer
 
 headers = {
     'Accept': 'application/json, text/plain, */*',
     'Accept-Encoding': 'gzip, deflate',
     'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7',
@@ -139,47 +142,52 @@
                 'Cookie': 'JSESSIONID=' + secrets.token_urlsafe(40),
                 'Host': 'www.jxqingtuan.cn',
                 'Origin': 'http://www.jxqingtuan.cn',
                 'Referer': 'http://www.jxqingtuan.cn/html/h5_index.html?&accessToken=' + openid,
             })
             async with AsyncClient(headers=headers) as client:
                 course = await client.get(url=url)
-            course.encoding = course.charset_encoding
-            if json.loads(course.text).get('code') == 0:
-                title = json.loads(course.text).get("list")[0].get("title")
-                course = json.loads(course.text).get('list')[0].get('id')
-                resp_url = 'http://www.jxqingtuan.cn/pub/vol/volClass/join?accessToken='
-                data = {"course": course, "nid": nid, "cardNo": name, "subOrg": suborg}
-                async with AsyncClient(headers=headers) as client:
+                course.encoding = course.charset_encoding
+                if json.loads(course.text).get('code') == 0:
+                    title = json.loads(course.text).get("list")[0].get("title")
+                    course = json.loads(course.text).get('list')[0].get('id')
+                    resp_url = 'http://www.jxqingtuan.cn/pub/vol/volClass/join?accessToken='
+                    data = {"course": course, "nid": nid, "cardNo": name, "subOrg": suborg}
                     res = await client.post(url=resp_url, json=data)
                     res.encoding = res.charset_encoding
-                resp = json.loads(res.text)
-                if resp.get("status") == 200:
-                    await User.filter(user_id=user_id).update(
-                        commit_time=time.time(),
-                        catalogue=title
-                    )
-                    await commit(user_id=user_id, catalogue=title, status=True)
-                    return {
-                        "status": 0,
-                        "catalogue": title,
-                        "msg": "提交成功！"
-                    }
+                    resp = json.loads(res.text)
+                    if resp.get("status") == 200:
+                        await User.filter(user_id=user_id).update(
+                            commit_time=time.time(),
+                            catalogue=title
+                        )
+                        await commit(user_id=user_id, catalogue=title, status=True)
+                        return {
+                            "status": 0,
+                            "catalogue": title,
+                            "msg": "提交成功！"
+                        }
+                    else:
+                        await commit(user_id=user_id, catalogue=title, status=False)
+                        return {
+                            "status": 500,
+                            "msg": "提交失败,信息错误！"
+                        }
                 else:
-                    await commit(user_id=user_id, catalogue=title, status=False)
+                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
                     return {
                         "status": 500,
-                        "msg": "提交失败！"
+                        "msg": "提交失败,江西共青团访问错误！"
                     }
         except Exception as e:
             logger.error(e)
             await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
             return {
                 "status": 500,
-                "msg": "提交失败！"
+                "msg": f"提交失败,{e}"
             }
 
 
 async def zhejiang(user_id: int) -> dict:
     """
     青春浙江
     :param user_id:
@@ -215,56 +223,60 @@
                 "Sec-Fetch-Dest": "empty",
                 "Accept-Encoding": "gzip, deflate",
                 "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
             }
             url = f"https://qczj.h5yunban.com/qczj-youth-learning/cgi-bin/login/we-chat/callback?callback=https%3A%2F%2Fqczj.h5yunban.com%2Fqczj-youth-learning%2Findex.php&scope=snsapi_userinfo&appid=wx56b888a1409a2920&openid={openid}&nickname={nickname}&headimg={cookie}&time={int(time.time())}&source=common&sign=&t={int(time.time())}"
             async with AsyncClient(headers=headers) as client:
                 response = await client.get(url)
-            response.encoding = response.charset_encoding
-            accessToken = re.findall(r"\(\'accessToken\'\,\s+\'(.+?)\'\)", response.text)[0]
-            study_url = f"https://qczj.h5yunban.com/qczj-youth-learning/cgi-bin/common-api/course/current?accessToken={accessToken}"
-            async with AsyncClient(headers=headers, max_redirects=5, timeout=10) as client:
+                response.encoding = response.charset_encoding
+                accessToken = re.findall(r"\(\'accessToken\'\,\s+\'(.+?)\'\)", response.text)[0]
+                study_url = f"https://qczj.h5yunban.com/qczj-youth-learning/cgi-bin/common-api/course/current?accessToken={accessToken}"
                 response = await client.get(url=study_url)
-            response.encoding = response.charset_encoding
-            if response.json()['status'] == 200:
-                title = response.json()["result"]['title']
-                course = response.json()['result']['id']
-                commit_url = f"https://qczj.h5yunban.com/qczj-youth-learning/cgi-bin/user-api/course/join?accessToken={accessToken}"
-                params = {
-                    "course": course,
-                    "subOrg": suborg,
-                    "nid": nid,
-                    "cardNo": name
-                }
-                async with AsyncClient(headers=headers, timeout=10, max_redirects=5) as client:
-                    response = await client.post(url=commit_url, json=params)
                 response.encoding = response.charset_encoding
                 if response.json()['status'] == 200:
-                    await User.filter(user_id=user_id).update(
-                        commit_time=time.time(),
-                        catalogue=title
-                    )
-                    await commit(user_id=user_id, catalogue=title, status=True)
-                    return {
-                        "status": 0,
-                        "catalogue": title,
-                        "msg": "提交成功！"
+                    title = response.json()["result"]['title']
+                    course = response.json()['result']['id']
+                    commit_url = f"https://qczj.h5yunban.com/qczj-youth-learning/cgi-bin/user-api/course/join?accessToken={accessToken}"
+                    params = {
+                        "course": course,
+                        "subOrg": suborg,
+                        "nid": nid,
+                        "cardNo": name
                     }
+                    response = await client.post(url=commit_url, json=params)
+                    response.encoding = response.charset_encoding
+                    if response.json()['status'] == 200:
+                        await User.filter(user_id=user_id).update(
+                            commit_time=time.time(),
+                            catalogue=title
+                        )
+                        await commit(user_id=user_id, catalogue=title, status=True)
+                        return {
+                            "status": 0,
+                            "catalogue": title,
+                            "msg": "提交成功！"
+                        }
+                    else:
+                        await commit(user_id=user_id, catalogue=title, status=False)
+                        return {
+                            "status": 500,
+                            "msg": "提交失败，信息错误！"
+                        }
                 else:
-                    await commit(user_id=user_id, catalogue=title, status=False)
+                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
                     return {
                         "status": 500,
-                        "msg": "提交失败！"
+                        "msg": "提交失败，青春浙江访问失败！"
                     }
         except Exception as e:
             logger.error(e)
             await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
             return {
                 "status": 500,
-                "msg": "提交失败！"
+                "msg": f"提交失败,{e}"
             }
 
 
 async def shanghai(user_id: int) -> dict:
     """
     青春上海
     :param user_id:
@@ -301,129 +313,54 @@
                 "Referer": "https://qcsh.h5yunban.com/youth-learning/signUp.php?rv=2020",
                 "Accept-Encoding": "gzip, deflate",
                 "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
             }
             url = f"https://qcsh.h5yunban.com/youth-learning/cgi-bin/login/we-chat/callback?appid=wxa693f4127cc93fad&openid={openid}&nickname={nickname}&headimg={cookie}&callback=https://qcsh.h5yunban.com/youth-learning/&scope=snsapi_userinfo"
             async with AsyncClient(headers=headers) as client:
                 response = await client.get(url)
-            response.encoding = response.charset_encoding
-            accessToken = re.findall(r"\(\'accessToken\'\,\s+\'(.+?)\'\)", response.text)[0]
-            study_url = f"https://qcsh.h5yunban.com/youth-learning/cgi-bin/common-api/course/current?accessToken={accessToken}"
-            async with AsyncClient(headers=headers, max_redirects=5, timeout=10) as client:
+                response.encoding = response.charset_encoding
+                accessToken = re.findall(r"\(\'accessToken\'\,\s+\'(.+?)\'\)", response.text)[0]
+                study_url = f"https://qcsh.h5yunban.com/youth-learning/cgi-bin/common-api/course/current?accessToken={accessToken}"
                 response = await client.get(url=study_url)
-            response.encoding = response.charset_encoding
-            if response.json()['status'] == 200:
-                title = response.json()["result"]['title']
-                course = response.json()['result']['id']
-                commit_url = f"https://qcsh.h5yunban.com/youth-learning/cgi-bin/user-api/course/join?accessToken={accessToken}"
-                params = {
-                    "course": course,
-                    "subOrg": suborg,
-                    "nid": nid,
-                    "cardNo": name
-                }
-                async with AsyncClient(headers=headers, timeout=10, max_redirects=5) as client:
-                    response = await client.post(url=commit_url, json=params)
                 response.encoding = response.charset_encoding
                 if response.json()['status'] == 200:
-                    await User.filter(user_id=user_id).update(
-                        commit_time=time.time(),
-                        catalogue=title
-                    )
-                    await commit(user_id=user_id, catalogue=title, status=True)
-                    return {
-                        "status": 0,
-                        "catalogue": title,
-                        "msg": "提交成功！"
-                    }
-                else:
-                    await commit(user_id=user_id, catalogue=title, status=False)
-                    return {
-                        "status": 500,
-                        "msg": "提交失败！"
+                    title = response.json()["result"]['title']
+                    course = response.json()['result']['id']
+                    commit_url = f"https://qcsh.h5yunban.com/youth-learning/cgi-bin/user-api/course/join?accessToken={accessToken}"
+                    params = {
+                        "course": course,
+                        "subOrg": suborg,
+                        "nid": nid,
+                        "cardNo": name
                     }
-        except Exception as e:
-            logger.error(e)
-            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-            return {
-                "status": 500,
-                "msg": "提交失败！"
-            }
-
-
-async def jiangsu(user_id: int) -> dict:
-    """
-    江苏共青团
-    :param user_id:用户ID
-    :return:
-    """
-    result = await User.filter(user_id=user_id).values()
-    if not result:
-        return {
-            "status": 500,
-            "msg": "用户数据不存在！"
-        }
-    else:
-        cookie = result[0]["cookie"]
-        answer = await Answer.all().order_by("time").values()
-        headers = {
-            "Host": "service.jiangsugqt.org",
-            "Connection": "keep-alive",
-            "Upgrade-Insecure-Requests": '1',
-            "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220303.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3262 MMWEBSDK/20220204 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.20.2100(0x28001438) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/wxpic,image/tpg,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
-            "X-Requested-With": "com.tencent.mm",
-            "Sec-Fetch-Site": "none",
-            "Sec-Fetch-Mode": "navigate",
-            "Sec-Fetch-User": "?1",
-            "Sec-Fetch-Dest": "document",
-            "Accept-Encoding": "gzip, deflate",
-            "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
-            "Cookie": cookie
-        }
-        try:
-            url = "https://service.jiangsugqt.org/api/lessons"
-            params = {"pages": 1, "limit": 5}
-            async with AsyncClient(headers=headers) as client:
-                response = await client.post(url=url, json=params)
-            response.encoding = response.charset_encoding
-            result = response.json()
-            if result["status"] == 1:
-                params = {
-                    "lesson_id": result["data"][0]["id"]
-                }
-                title = result["data"][0]["title"]
-                commit_url = "https://service.jiangsugqt.org/api/doLesson"
-                async with AsyncClient(headers=headers) as client:
                     response = await client.post(url=commit_url, json=params)
-                response.encoding = response.charset_encoding
-                result = response.json()
-                if result["status"] == 1:
-                    await User.filter(user_id=user_id).update(
-                        commit_time=time.time(),
-                        catalogue=result["data"]["title"]
-                    )
-                    await commit(user_id=user_id, catalogue=result["data"]["title"], status=True)
-                    return {
-                        "status": 0,
-                        "catalogue": result["data"]["title"],
-                        "msg": "提交成功！"
-                    }
+                    response.encoding = response.charset_encoding
+                    if response.json()['status'] == 200:
+                        await User.filter(user_id=user_id).update(
+                            commit_time=time.time(),
+                            catalogue=title
+                        )
+                        await commit(user_id=user_id, catalogue=title, status=True)
+                        return {
+                            "status": 0,
+                            "catalogue": title,
+                            "msg": "提交成功！"
+                        }
+                    else:
+                        await commit(user_id=user_id, catalogue=title, status=False)
+                        return {
+                            "status": 500,
+                            "msg": "提交失败,信息错误！"
+                        }
                 else:
-                    await commit(user_id=user_id, catalogue=title, status=False)
+                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
                     return {
                         "status": 500,
-                        "msg": "提交失败！"
+                        "msg": "提交失败，青春上海访问失败！"
                     }
-            else:
-                await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-                return {
-                    "status": 500,
-                    "msg": "提交失败！"
-                }
         except Exception as e:
             logger.error(e)
             await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
             return {
                 "status": 500,
                 "msg": "提交失败！"
             }
@@ -449,108 +386,95 @@
         level2 = result[0]['university']
         level3 = result[0]['college']
         level4 = result[0]['organization']
         level5 = result[0]['organization_id']
         token = result[0]["token"]
         answer = await Answer.all().order_by("time").values()
         try:
-            headers.update({
+            headers = {
                 "Host": "dxx.ahyouth.org.cn",
                 "Accept": "application/json, text/plain, */*",
                 "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
                 "Referer": "http://dxx.ahyouth.org.cn/",
                 "Accept-Encoding": "gzip, deflate",
                 "Connection": "keep-alive",
                 'Content-Type': 'application/x-www-form-urlencoded',
                 "X-Requested-With": 'com.tencent.mm',
                 "Origin": 'http://dxx.ahyouth.org.cn',
                 "token": token
-            })
+            }
             data = {
                 'username': username,
                 'gender': gender,
                 'mobile': mobile,
                 'level1': level1,
                 'level2': level2,
                 'level3': level3,
                 'level4': level4,
                 'level5': level5
             }
             get_infor_url = 'http://dxx.ahyouth.org.cn/api/saveUserInfo'
             async with AsyncClient(headers=headers, timeout=30, max_redirects=5) as client:
                 infor_response = await client.post(url=get_infor_url, params=data)
-            infor_response.encoding = infor_response.charset_encoding
-            infor_response_json = infor_response.json()
-            if infor_response_json['code'] == 200:
-                username = infor_response_json['content']['username']
-                token = infor_response_json['content']['token']
-                gender = infor_response_json['content']['gender']
-                mobile = infor_response_json['content']['mobile']
-                level1 = infor_response_json['content']['level1']
-                level2 = infor_response_json['content']['level2']
-                level3 = infor_response_json['content']['level3']
-                level4 = infor_response_json['content']['level4']
-                level5 = infor_response_json['content']['level5']
-                headers.update({
-                    "Host": "dxx.ahyouth.org.cn",
-                    "Accept": "application/json, text/plain, */*",
-                    "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
-                    "Referer": "http://dxx.ahyouth.org.cn/",
-                    "Accept-Encoding": "gzip, deflate",
-                    "Connection": "keep-alive",
-                    'Content-Type': 'application/x-www-form-urlencoded',
-                    "X-Requested-With": 'com.tencent.mm',
-                    "Origin": 'http://dxx.ahyouth.org.cn',
-                    "token": token
-                })
-                data = {
-                    'username': username,
-                    'gender': gender,
-                    'mobile': mobile,
-                    'level1': level1,
-                    'level2': level2,
-                    'level3': level3,
-                    'level4': level4,
-                    'level5': level5
-                }
-                commit_url = 'http://dxx.ahyouth.org.cn/api/newLearn'
-                async with AsyncClient(headers=headers, timeout=30, max_redirects=5) as client:
-                    commit_response = await client.post(url=commit_url, params=data)
-                commit_response.encoding = commit_response.charset_encoding
-                commit_response_json = commit_response.json()
-                if commit_response_json['code'] == 200:
-                    await User.filter(user_id=user_id).update(
-                        token=token,
-                        commit_time=time.time(),
-                        catalogue=answer[-1]["catalogue"]
-                    )
-                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=True)
-                    return {
-                        "status": 0,
-                        "catalogue": answer[-1]["catalogue"],
-                        "msg": "提交成功！"
+                infor_response.encoding = infor_response.charset_encoding
+                infor_response_json = infor_response.json()
+                if infor_response_json['code'] == 200:
+                    username = infor_response_json['content']['username']
+                    token = infor_response_json['content']['token']
+                    gender = infor_response_json['content']['gender']
+                    mobile = infor_response_json['content']['mobile']
+                    level1 = infor_response_json['content']['level1']
+                    level2 = infor_response_json['content']['level2']
+                    level3 = infor_response_json['content']['level3']
+                    level4 = infor_response_json['content']['level4']
+                    level5 = infor_response_json['content']['level5']
+                    data = {
+                        'username': username,
+                        'gender': gender,
+                        'mobile': mobile,
+                        'level1': level1,
+                        'level2': level2,
+                        'level3': level3,
+                        'level4': level4,
+                        'level5': level5
                     }
+                    commit_url = 'http://dxx.ahyouth.org.cn/api/newLearn'
+                    commit_response = await client.post(url=commit_url, params=data)
+                    commit_response.encoding = commit_response.charset_encoding
+                    commit_response_json = commit_response.json()
+                    if commit_response_json['code'] == 200:
+                        await User.filter(user_id=user_id).update(
+                            token=token,
+                            commit_time=time.time(),
+                            catalogue=answer[-1]["catalogue"]
+                        )
+                        await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=True)
+                        return {
+                            "status": 0,
+                            "catalogue": answer[-1]["catalogue"],
+                            "msg": "提交成功！"
+                        }
+                    else:
+                        await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                        return {
+                            "status": 500,
+                            "msg": "提交失败，token失效！"
+                        }
                 else:
                     await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
                     return {
                         "status": 500,
-                        "msg": "提交失败！"
+                        "msg": "提交失败,token获取失败！"
                     }
-            else:
-                await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
-                return {
-                    "status": 500,
-                    "msg": "提交失败！"
-                }
         except Exception as e:
             logger.error(e)
             await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
             return {
                 "status": 500,
-                "msg": "提交失败！"
+                "msg": f"提交失败,{e}"
             }
 
 
 async def sichuan(user_id: int) -> dict:
     """
     天府新青年
     :param user_id:
@@ -601,49 +525,49 @@
         })
         answer = await Answer.all().order_by("time").values()
         title = answer[-1]["catalogue"]
         url = 'https://dxx.scyol.com/api/student/commit'
         try:
             async with AsyncClient(headers=headers) as client:
                 response = await client.post(url=url, json=data_json)
-            if response.status_code == 200:
-                response.encoding = response.charset_encoding
-                if response.json()["code"] == 2:
-                    await User.filter(user_id=user_id).update(
-                        commit_time=time.time(),
-                        catalogue=title
-                    )
-                    await commit(user_id=user_id, catalogue=title, status=True)
-                    return {
-                        "status": 0,
-                        "catalogue": title,
-                        "msg": "你已经提交了，请勿重复提交哦"
-                    }
-                elif response.json()["code"] == 200:
-                    await User.filter(user_id=user_id).update(
-                        commit_time=time.time(),
-                        catalogue=title
-                    )
-                    await commit(user_id=user_id, catalogue=title, status=True)
-                    return {
-                        "status": 0,
-                        "catalogue": title,
-                        "msg": "提交成功！"
-                    }
+                if response.status_code == 200:
+                    response.encoding = response.charset_encoding
+                    if response.json()["code"] == 2:
+                        await User.filter(user_id=user_id).update(
+                            commit_time=time.time(),
+                            catalogue=title
+                        )
+                        await commit(user_id=user_id, catalogue=title, status=True)
+                        return {
+                            "status": 0,
+                            "catalogue": title,
+                            "msg": "你已经提交了，请勿重复提交哦"
+                        }
+                    elif response.json()["code"] == 200:
+                        await User.filter(user_id=user_id).update(
+                            commit_time=time.time(),
+                            catalogue=title
+                        )
+                        await commit(user_id=user_id, catalogue=title, status=True)
+                        return {
+                            "status": 0,
+                            "catalogue": title,
+                            "msg": "提交成功！"
+                        }
+                    else:
+                        await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                        return {
+                            "status": 500,
+                            "msg": "提交失败！"
+                        }
                 else:
-                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
                     return {
                         "status": 500,
-                        "msg": "提交失败！"
+                        "msg": "提交失败,cookie失效！"
                     }
-            else:
-                return {
-                    "status": 500,
-                    "msg": "提交失败,cookie失效！"
-                }
         except Exception as e:
             return {
                 "status": 500,
                 "msg": f"提交失败,{e}"
             }
 
 
@@ -677,77 +601,76 @@
             "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
             "Cookie": cookie
         })
         try:
             version_url = f'http://qndxx.youth54.cn/SmartLA/dxxjfgl.w?method=getNewestVersionInfo&openid={openid}'
             async with AsyncClient(headers=headers) as client:
                 version_response = await client.post(url=version_url)
-            if version_response.status_code == 200:
-                version_response.encoding = version_response.charset_encoding
-                content = version_response.json()
-                if content["errcode"] == "0":
-                    versionname = content['versionname']
-                    version = content['version']
-                    headers.update({
-                        "Host": "qndxx.youth54.cn",
-                        "Connection": "keep-alive",
-                        "Accept": "*/*",
-                        "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220213.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3234 MMWEBSDK/20210902 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.15.2020(0x28000F30) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
-                        "X-Requested-With": "XMLHttpRequest",
-                        "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
-                        "Origin": "http://qndxx.youth54.cn",
-                        "Referer": "http://qndxx.youth54.cn/SmartLA/dxx.w?method=pageSdtwdt",
-                        "Accept-Encoding": "gzip, deflate",
-                        "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
-                        "Cookie": cookie
-                    })
-                    data = {
-                        'openid': openid,
-                        'version': version
-                    }
-                    commit_url = 'http://qndxx.youth54.cn/SmartLA/dxxjfgl.w?method=studyLatest'
-                    async with AsyncClient(headers=headers) as client:
-                        response = await client.post(url=commit_url, params=data)
-                    if response.status_code == 200:
-                        response.encoding = response.charset_encoding
-                        if response.json()["errcode"] == "0":
-                            await User.filter(user_id=user_id).update(
-                                commit_time=time.time(),
-                                catalogue=versionname
-                            )
-                            await commit(user_id=user_id, catalogue=versionname, status=True)
-                            return {
-                                "status": 0,
-                                "catalogue": versionname,
-                                "msg": "提交成功！"
-                            }
+                if version_response.status_code == 200:
+                    version_response.encoding = version_response.charset_encoding
+                    content = version_response.json()
+                    if content["errcode"] == "0":
+                        versionname = content['versionname']
+                        version = content['version']
+                        headers.update({
+                            "Host": "qndxx.youth54.cn",
+                            "Connection": "keep-alive",
+                            "Accept": "*/*",
+                            "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220213.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3234 MMWEBSDK/20210902 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.15.2020(0x28000F30) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
+                            "X-Requested-With": "XMLHttpRequest",
+                            "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
+                            "Origin": "http://qndxx.youth54.cn",
+                            "Referer": "http://qndxx.youth54.cn/SmartLA/dxx.w?method=pageSdtwdt",
+                            "Accept-Encoding": "gzip, deflate",
+                            "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
+                            "Cookie": cookie
+                        })
+                        data = {
+                            'openid': openid,
+                            'version': version
+                        }
+                        commit_url = 'http://qndxx.youth54.cn/SmartLA/dxxjfgl.w?method=studyLatest'
+                        response = await client.post(url=commit_url, params=data, headers=headers)
+                        if response.status_code == 200:
+                            response.encoding = response.charset_encoding
+                            if response.json()["errcode"] == "0":
+                                await User.filter(user_id=user_id).update(
+                                    commit_time=time.time(),
+                                    catalogue=versionname
+                                )
+                                await commit(user_id=user_id, catalogue=versionname, status=True)
+                                return {
+                                    "status": 0,
+                                    "catalogue": versionname,
+                                    "msg": "提交成功！"
+                                }
+                            else:
+                                await commit(user_id=user_id, catalogue=versionname, status=False)
+                                return {
+                                    "status": 500,
+                                    "msg": "提交失败,cookie失效！"
+                                }
                         else:
                             await commit(user_id=user_id, catalogue=versionname, status=False)
                             return {
                                 "status": 500,
-                                "msg": "提交失败！"
+                                "msg": "提交失败，cookie失效！"
                             }
                     else:
-                        await commit(user_id=user_id, catalogue=versionname, status=False)
+                        await commit(user_id=user_id, catalogue=title, status=False)
                         return {
                             "status": 500,
-                            "msg": "提交失败！"
+                            "msg": "提交失败，cookie失效！"
                         }
                 else:
                     await commit(user_id=user_id, catalogue=title, status=False)
                     return {
                         "status": 500,
-                        "msg": "提交失败！"
+                        "msg": "提交失败，青春山东访问失败！"
                     }
-            else:
-                await commit(user_id=user_id, catalogue=title, status=False)
-                return {
-                    "status": 500,
-                    "msg": "提交失败！"
-                }
         except Exception as e:
             await commit(user_id=user_id, catalogue=title, status=False)
             return {
                 "status": 500,
                 "msg": f"提交失败,{e}"
             }
 
@@ -779,62 +702,61 @@
                 "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7"
             }
         )
         try:
             new_url = f"http://qndxx.cqyouths.com/new_course.json?time={int(time.time())}"
             async with AsyncClient(headers=headers) as client:
                 new_response = await client.get(url=new_url)
-            if new_response.status_code == 200:
-                new_response.encoding = new_response.charset_encoding
-                course_id = new_response.json()['data'][0]['id']
-                commit_url = f"http://qndxx.cqyouths.com/api/course/studyCourse?openid={openid}&id={course_id}"
-                async with AsyncClient(headers=headers) as client:
+                if new_response.status_code == 200:
+                    new_response.encoding = new_response.charset_encoding
+                    course_id = new_response.json()['data'][0]['id']
+                    commit_url = f"http://qndxx.cqyouths.com/api/course/studyCourse?openid={openid}&id={course_id}"
                     response = await client.get(url=commit_url)
-                if response.status_code == 200:
-                    response.encoding = response.charset_encoding
-                    if response.json()["status"] == 200:
-                        await User.filter(user_id=user_id).update(
-                            commit_time=time.time(),
-                            catalogue=title
-                        )
-                        await commit(user_id=user_id, catalogue=title, status=True)
-                        return {
-                            "status": 0,
-                            "catalogue": title,
-                            "msg": "提交成功！"
-                        }
-                    elif response.json()["status"] == 201:
-                        await User.filter(user_id=user_id).update(
-                            commit_time=time.time(),
-                            catalogue=title
-                        )
-                        await commit(user_id=user_id, catalogue=title, status=True)
-                        return {
-                            "status": 0,
-                            "catalogue": title,
-                            "msg": "提交成功！"
-                        }
+                    if response.status_code == 200:
+                        response.encoding = response.charset_encoding
+                        if response.json()["status"] == 200:
+                            await User.filter(user_id=user_id).update(
+                                commit_time=time.time(),
+                                catalogue=title
+                            )
+                            await commit(user_id=user_id, catalogue=title, status=True)
+                            return {
+                                "status": 0,
+                                "catalogue": title,
+                                "msg": "提交成功！"
+                            }
+                        elif response.json()["status"] == 201:
+                            await User.filter(user_id=user_id).update(
+                                commit_time=time.time(),
+                                catalogue=title
+                            )
+                            await commit(user_id=user_id, catalogue=title, status=True)
+                            return {
+                                "status": 0,
+                                "catalogue": title,
+                                "msg": "提交成功！"
+                            }
+                        else:
+                            await commit(user_id=user_id, catalogue=title, status=False)
+                            return {
+                                "status": 500,
+                                "msg": "提交失败，openid错误！"
+                            }
                     else:
                         await commit(user_id=user_id, catalogue=title, status=False)
                         return {
                             "status": 500,
-                            "msg": "提交失败！"
+                            "msg": "提交失败，openid错误！"
                         }
                 else:
                     await commit(user_id=user_id, catalogue=title, status=False)
                     return {
                         "status": 500,
-                        "msg": "提交失败！"
+                        "msg": "提交失败，重庆共青团访问失败！"
                     }
-            else:
-                await commit(user_id=user_id, catalogue=title, status=False)
-                return {
-                    "status": 500,
-                    "msg": "提交失败！"
-                }
         except Exception as e:
             logger.error(e)
             return {
                 "status": 500,
                 "msg": f"提交失败,{e}"
             }
 
@@ -888,21 +810,21 @@
                         "catalogue": title,
                         "msg": "提交成功！"
                     }
                 else:
                     await commit(user_id=user_id, catalogue=title, status=False)
                     return {
                         "status": 500,
-                        "msg": f"提交失败!"
+                        "msg": f"提交失败，openid错误！"
                     }
             else:
                 await commit(user_id=user_id, catalogue=title, status=False)
                 return {
                     "status": 500,
-                    "msg": "提交失败！"
+                    "msg": "提交失败，吉青飞扬访问失败！"
                 }
         except Exception as e:
             logger.error(e)
             return {
                 "status": 500,
                 "msg": f"提交失败,{e}"
             }
@@ -939,15 +861,15 @@
                 'Sec-Fetch-Dest': 'empty',
                 'Referer': 'https://youthstudy.12355.net/h5/',
                 'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7',
             }
             new_study_url = "https://youthstudy.12355.net/saomah5/api/young/chapter/new"
             async with AsyncClient(headers=study_headers, timeout=30, max_redirects=5) as client:
                 study_response = await client.get(url=new_study_url)
-            study_response.encoding=study_response.charset_encoding
+            study_response.encoding = study_response.charset_encoding
             if study_response.json()["errno"] == 0:
                 chapterId = study_response.json().get('data').get('entity').get('id')
                 title = study_response.json().get('data').get('entity').get('name').replace('“青年大学习”', "").strip()
                 commit_url = "https://youthstudy.12355.net/saomah5/api/young/course/chapter/saveHistory"
                 async with AsyncClient(headers=study_headers, timeout=30, max_redirects=5) as client:
                     commit_response = await client.post(url=commit_url, data={
                         "chapterId": chapterId
@@ -1004,15 +926,16 @@
                             'Sec-Fetch-Site': 'same-origin',
                             'Sec-Fetch-Mode': 'cors',
                             'Referer': 'https://youthstudy.12355.net/h5/',
                             'Accept-Encoding': 'gzip, deflate',
                             'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7'
                         }
                         async with AsyncClient(headers=token_headers, timeout=30, max_redirects=5) as client:
-                            token_response = await client.post(url=token_url, data="sign="+urllib.parse.quote(content))
+                            token_response = await client.post(url=token_url,
+                                                               data="sign=" + urllib.parse.quote(content))
                         if token_response.json()["errno"] == 0:
                             token = token_response.json()['data']['entity']['token']
                             study_headers = {
                                 'Host': 'youthstudy.12355.net',
                                 'Connection': 'keep-alive',
                                 'X-Litemall-Token': token,
                                 'X-Litemall-IdentiFication': 'young',
@@ -1072,74 +995,184 @@
             logger.error(e)
             await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
             return {
                 "status": 500,
                 "msg": "提交失败！"
             }
 
-async def heilongjiang(user_id: int) -> dict:
+
+async def beijing(user_id: int) -> dict:
     """
-    黑龙江共青团
+    青春北京
+    :param user_id:用户ID
+    :return:
+    """
+    result = await User.filter(user_id=user_id).values()
+    if not result:
+        return {
+            "status": 500,
+            "msg": "用户数据不存在！"
+        }
+    else:
+        cookie = result[0]['cookie']
+        token = result[0]["token"]
+        answer = await Answer.all().order_by("time").values()
+        headers = {
+            "User-Agent": "Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Mobile/15E148 Safari/604.1 Edg/113.0.0.0", }
+        login_url = "https://m.bjyouth.net/site/login"
+        try:
+            async with AsyncClient(headers=headers) as client:
+                login_rsp = await client.get(login_url)
+                if login_rsp.status_code == 200:
+                    login_rsp.encoding = login_rsp.charset_encoding
+                    soup = BeautifulSoup(login_rsp.text, "lxml")
+                    code_url = "https://m.bjyouth.net" + soup.select("#verifyCode-image")[0].get("src")
+                    code_rsp = await client.get(code_url)
+                    code_text = DdddOcr(show_ad=False).classification(code_rsp.content)
+                    login_response = await client.post(
+                        url=login_url,
+                        data={
+                            '_csrf_mobile': client.cookies['_csrf_mobile'],
+                            'Login[password]': await encrypt(token),
+                            'Login[username]': await encrypt(cookie),
+                            'Login[verifyCode]': code_text
+                        }
+                    )
+                    if login_response.status_code == 200:
+                        login_response.encoding = login_response.charset_encoding
+                        if login_response.text == '8':
+                            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                            return {
+                                "status": 500,
+                                "msg": "提交失败，验证码识别失败！"
+                            }
+                        if 'fail' in login_response.text:
+                            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                            return {
+                                "status": 500,
+                                "msg": "提交失败，账号或密码错误！"
+                            }
+                        course_url = "https://m.bjyouth.net/dxx/index"
+                        course_rsp = await client.get(course_url)
+                        if course_rsp.json()["code"] == 200:
+                            title = course_rsp.json()['newCourse']['title']
+                            courseId = course_rsp.json()['newCourse']['id']
+                            organization_rsp = await client.get('https://m.bjyouth.net/dxx/is-league')
+                            organization_id = int(organization_rsp.text)
+                            study_url = "https://m.bjyouth.net/dxx/check"
+                            study_response = await client.post(url=study_url, json={
+                                "id": str(courseId),
+                                "org_id": organization_id
+                            })
+                            if study_response.status_code == 200:
+                                learnedInfo_url = 'https://m.bjyouth.net/dxx/my-study?page=1&limit=15&year=' + time.strftime(
+                                    "%Y",
+                                    time.localtime())
+                                haveLearned = await client.get(learnedInfo_url)
+                                if haveLearned.json()["code"] == 200:
+                                    if f"学习课程：《{title}》" in list(
+                                            map(lambda x: x['text'], haveLearned.json()['data'])):
+                                        await User.filter(user_id=user_id).update(
+                                            token=token,
+                                            commit_time=time.time(),
+                                            catalogue=answer[-1]["catalogue"]
+                                        )
+                                        await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=True)
+                                        return {
+                                            "status": 0,
+                                            "catalogue": answer[-1]["catalogue"],
+                                            "msg": "提交成功！"
+                                        }
+                                    else:
+                                        await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                                        return {
+                                            "status": 500,
+                                            "msg": "提交失败！"
+                                        }
+                                else:
+                                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                                    return {
+                                        "status": 500,
+                                        "msg": "提交失败,获取历史提交信息失败！"
+                                    }
+                            else:
+                                await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                                return {
+                                    "status": 500,
+                                    "msg": "提交失败！"
+                                }
+                    else:
+                        await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                        return {
+                            "status": 500,
+                            "msg": "提交失败，登录失败！"
+                        }
+                else:
+                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                    return {
+                        "status": 500,
+                        "msg": "提交失败，北京共青团官网异常"
+                    }
+        except Exception as e:
+            logger.error(e)
+            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+            return {
+                "status": 500,
+                "msg": f"提交失败,{e}"
+            }
+
+
+async def tianjin(user_id: int) -> dict:
+    """
+    津彩青春
     :param user_id:用户ID
     :return:
     """
     result = await User.filter(user_id=user_id).values()
     if not result:
         return {
             "status": 500,
             "msg": "用户数据不存在！"
         }
     else:
         cookie = result[0]["cookie"]
         answer = await Answer.all().order_by("time").values()
+        title = answer[-1]["catalogue"]
         headers = {
-            "Host": "tsw.ithyxy.com",
-            "Connection": "keep-alive",
-            "Accept": "application/json, text/plain, */*",
-            "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220303.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3262 MMWEBSDK/20220204 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.20.2100(0x28001438) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
-            "X-Requested-With": "com.tencent.mm",
-            "Referer": "http://tsw.ithyxy.com/login",
-            "Accept-Encoding": "gzip, deflate",
-            "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
-            "Cookie": cookie
+            "User-Agent": "Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Mobile/15E148 Safari/604.1 Edg/113.0.0.0",
+            "Cookie": cookie,
         }
         try:
-            learn_url = "http://tsw.ithyxy.com/h5/learn/home"
-            async with AsyncClient(headers=headers, timeout=5, max_redirects=5) as client:
-                response = await client.get(url=learn_url)
-            response.encoding = response.charset_encoding
-            if response.status_code == 200 and response.json()["code"] == 200:
-                learn_id = response.json()["data"]["id"]
-                commit_url = f"http://tsw.ithyxy.com/h5/learn/enter?id={learn_id}"
-                async with AsyncClient(headers=headers, timeout=5, max_redirects=5) as client:
-                    response = await client.get(url=commit_url)
+            commit_url = "http://admin.ddy.tjyun.com/zm/jump/1"
+            async with AsyncClient(headers=headers) as client:
+                response = await client.get(url=commit_url)
+            if response.status_code == 302:
                 response.encoding = response.charset_encoding
-                if response.status_code == 200 and response.json()["code"] == 200:
+                if "weui_text_area" not in response.text:
                     await User.filter(user_id=user_id).update(
                         commit_time=time.time(),
-                        catalogue=answer[-1]["catalogue"]
+                        catalogue=title
                     )
-                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=True)
+                    await commit(user_id=user_id, catalogue=title, status=True)
                     return {
                         "status": 0,
-                        "catalogue": answer[-1]["catalogue"],
+                        "catalogue": title,
                         "msg": "提交成功！"
                     }
                 else:
-                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                    await commit(user_id=user_id, catalogue=title, status=False)
                     return {
                         "status": 500,
-                        "msg": "提交失败，cookie失效！"
+                        "msg": f"提交失败，Cookie失效！"
                     }
             else:
-                await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                await commit(user_id=user_id, catalogue=title, status=False)
                 return {
                     "status": 500,
-                    "msg": "提交失败，cookie失效！"
+                    "msg": "提交失败，地址请求失败！"
                 }
         except Exception as e:
             logger.error(e)
-            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
             return {
                 "status": 500,
-                "msg": "提交失败！"
-            }
+                "msg": f"提交失败,{e}"
+            }
```

### Comparing `TeenStudy-0.1.9/TeenStudy/utils/handle.py` & `TeenStudy-0.2.0/TeenStudy/utils/handle.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                      priority=50)
 
 submit = on_command("submit", aliases={"提交大学习"}, permission=SUPERUSER | GROUP, rule=Rule(must_command, must_group),
                     priority=50)
 add = on_command("add_dxx", aliases={"添加大学习"}, permission=GROUP, rule=must_group, priority=50)
 my_info = on_command("my_info", aliases={"我的大学习"}, permission=SUPERUSER | GROUP,
                      rule=Rule(must_command, must_group), priority=50)
-poke_notify = on_notice(priority=60, rule=check_poke)
+poke_notify = on_notice(priority=60, rule=Rule(check_poke,must_group))
 answer_pic = on_command("answer_pic", aliases={"答案截图", "大学习"}, rule=Rule(must_command, must_group),
                         permission=SUPERUSER | GROUP,
                         priority=50)
 finish_dxx = on_command("finish_dxx", aliases={"完成大学习", "全员大学习"},
                         rule=Rule(must_command, must_group, must_leader), permission=GROUP | SUPERUSER, priority=50)
 reset_config = on_command("reset_config", aliases={"重置配置", "刷新配置"}, permission=SUPERUSER, rule=must_command,
                           priority=50)
```

### Comparing `TeenStudy-0.1.9/TeenStudy/utils/path.py` & `TeenStudy-0.2.0/TeenStudy/utils/path.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/utils/rule.py` & `TeenStudy-0.2.0/TeenStudy/utils/rule.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 import datetime
+from typing import Union
 
 from nonebot.adapters.onebot.v11 import Bot, Message, MessageEvent, NotifyEvent
 from nonebot.params import CommandArg
 
-from ..models.dxx import PushList
 from ..models.accuont import User
+from ..models.dxx import PushList
 
 
-async def must_group(bot: Bot, event: MessageEvent) -> bool:
+async def must_group(bot: Bot, event: Union[MessageEvent, NotifyEvent]) -> bool:
     """
     必须是群消息才响应
     :param bot: 机器人
     :param event: 事件
     :return: 返回True或False
     """
-    if event.message_type == "group":
+    if isinstance(event, MessageEvent):
+        if event.message_type == "group":
+            self_id = int(bot.self_id)
+            group_id = event.group_id
+            if await PushList.filter(group_id=group_id, status=True, self_id=self_id).count():
+                return True
+
+        else:
+            return False
+    else:
+        try:
+            group_id = event.group_id
+        except AttributeError:
+            return False
         self_id = int(bot.self_id)
-        group_id = event.group_id
         if await PushList.filter(group_id=group_id, status=True, self_id=self_id).count():
             return True
-    else:
         return False
 
 
 async def must_command(order: Message = CommandArg()) -> bool:
     """
     限制指令后面不能加内容才生效
     :param order: 指令后面的内容
@@ -63,14 +75,14 @@
     else:
         return False
 
 
 async def check_time():
     now_day = datetime.datetime.now().weekday()
     now_hour = datetime.datetime.now().hour
-    if now_day in [0,  6]:
+    if now_day in [0, 5, 6]:
         if now_day in [5, 6]:
             return False
         else:
             if now_hour in [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]:
                 return False
     return True
```

### Comparing `TeenStudy-0.1.9/TeenStudy/utils/update.py` & `TeenStudy-0.2.0/TeenStudy/utils/update.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
                 await bot.send_private_msg(user_id=admin["SUPERUSER"], message=MessageSegment.text(
                     f"检测到青年大学习有更新，下周一为{catalogue},详细信息请扫码登录后台查看d(´ω｀*)") + MessageSegment.image(
                     content["content"]))
             except Exception as e:
                 logger.error(e)
 
 
-@scheduler.scheduled_job('cron', second='*/15', misfire_grace_time=10)
+@scheduler.scheduled_job('cron', second='*/10', misfire_grace_time=10)
 async def check_apply():
     try:
         bot: Bot = get_bot()
     except ValueError as e:
         return
     apply_list = await AddUser.filter(status="未通过").values()
```

#### html2text {}

```diff
@@ -78,15 +78,15 @@
 ( f"æ£æµå°éå¹´å¤§å­¦ä¹ ææ´æ°ï¼ä¸å¨ä¸ä¸º
 {catalogue},è¯¦ç»ä¿¡æ¯è¯·ç¹å»é¾æ¥ç»å½åå°æ¥çï¼å¦æä¸å¼é¾æ¥ï¼è¯·å¤å¶é¾æ¥å°æµè§å¨d
 (Â´Ïï½*)\n") + MessageSegment.text( content["url"])) await
 bot.send_private_msg(user_id=admin["SUPERUSER"], message=MessageSegment.text
 ( f"æ£æµå°éå¹´å¤§å­¦ä¹ ææ´æ°ï¼ä¸å¨ä¸ä¸º
 {catalogue},è¯¦ç»ä¿¡æ¯è¯·æ«ç ç»å½åå°æ¥çd(Â´Ïï½*)") +
 MessageSegment.image( content["content"])) except Exception as e: logger.error
-(e) @scheduler.scheduled_job('cron', second='*/15', misfire_grace_time=10)
+(e) @scheduler.scheduled_job('cron', second='*/10', misfire_grace_time=10)
 async def check_apply(): try: bot: Bot = get_bot() except ValueError as e:
 return apply_list = await AddUser.filter(status="æªéè¿").values() for item
 in apply_list: result = await User.filter(user_id=item["user_id"],
 group_id=item["group_id"]).count() if result: await AddUser.filter(id=item
 ["id"]).update(status="å·²éè¿") await bot.send_group_msg(group_id=item
 ["group_id"], message=MessageSegment.at(user_id=item["user_id"]) +
 MessageSegment.text( "ä¿¡æ¯ç»å®æå( â¢ ÌÏâ¢Ì )â§")) await
```

### Comparing `TeenStudy-0.1.9/TeenStudy/utils/utils.py` & `TeenStudy-0.2.0/TeenStudy/utils/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 import random
 import socket
 import time
 from io import BytesIO
 from pathlib import Path
 
 import qrcode
+from Crypto.Cipher import PKCS1_v1_5
+from Crypto.PublicKey import RSA
 from PIL import Image, ImageDraw, ImageFont
 from httpx import AsyncClient
 from nonebot import logger, get_driver, on_command
 from nonebot.adapters.onebot.v11 import MessageEvent
 from nonebot.params import ArgStr
 from nonebot.permission import SUPERUSER
 from pydantic import BaseModel
 
 from . import dxx, path, rule
 from ..models.accuont import User
-from ..models.dxx import Area, Answer, Resource, JiangXi
+from ..models.dxx import Area, Answer, Resource
 
 USERDATA = path.DATABASE_PATH / "users.json"
 
 
 class UserModel(BaseModel):
     id: int = None
     """用户ID"""
@@ -113,23 +115,14 @@
         "referer": None,
         "origin": None,
         "url": "https://qcsh.h5yunban.com/youth-learning/cgi-bin/user-api/course/join?accessToken=",
         "status": True,
         "catalogue": None
     },
     {
-        "area": "江苏",
-        "host": "service.jiangsugqt.org",
-        "referer": None,
-        "origin": None,
-        "url": "https://service.jiangsugqt.org/youth/lesson/confirm",
-        "status": True,
-        "catalogue": None
-    },
-    {
         "area": "安徽",
         "host": "dxx.ahyouth.org.cn",
         "referer": "http://dxx.ahyouth.org.cn/",
         "origin": "http://dxx.ahyouth.org.cn",
         "url": "http://dxx.ahyouth.org.cn/api/hidtoryList",
         "status": True,
         "catalogue": None
@@ -176,19 +169,28 @@
         "referer": None,
         "origin": "https://tuan.12355.net",
         "url": "https://youthstudy.12355.net/saomah5/api/young/chapter/new",
         "status": True,
         "catalogue": None
     },
     {
-        "area": "黑龙江",
-        "host": "tsw.ithyxy.com",
+        "area": "北京",
+        "host": "m.bjyouth.net",
+        "referer": None,
+        "origin": "https://m.bjyouth.net",
+        "url": "https://m.bjyouth.net/dxx/index",
+        "status": True,
+        "catalogue": None
+    },
+    {
+        "area": "天津",
+        "host": "admin.ddy.tjyun.com",
         "referer": None,
-        "origin": "http://tsw.ithyxy.com/login",
-        "url": "http://tsw.ithyxy.com/h5/learn/home",
+        "origin": "https://admin.ddy.tjyun.com",
+        "url": "http://admin.ddy.tjyun.com/zm/jump/1",
         "status": True,
         "catalogue": None
     },
 ]
 RESOURCE = [
     {
         "name": "MiSans-Light.ttf",
@@ -239,15 +241,14 @@
 
 @update_resource.got(key="msg", prompt="是否刷新资源数据库信息？（是|否）")
 async def update_resource_(msg: str = ArgStr("msg")) -> None:
     if msg not in ["是", "yes", "Y", "y", "YES", "true"]:
         await update_resource.finish(message="操作取消(*^▽^*)", at_sender=True, reply_message=True)
     else:
         await update_resource.send("资源重新载入中（请等待1分钟左右）······", at_sender=True, reply_message=True)
-        await JiangXi.all().delete()
         await Resource.all().delete()
         await resource_init()
         await update_resource.finish(message="资源数据载入成功(^_−)☆", at_sender=True, reply_message=True)
 
 
 @export_data.got(key="msg", prompt="是否导出用户数据至TeenStudy目录？（是|否）")
 async def export_user(event: MessageEvent, msg: str = ArgStr("msg")) -> None:
@@ -326,60 +327,25 @@
         }
         try:
             logger.opt(colors=True).info(
                 f'<u><y>[大学习数据库]</y></u><g>加载配置公网IP</g>')
             ip = get_driver().config.dxx_ip
             logger.opt(colors=True).info(
                 f'<u><y>[大学习数据库]</y></u><g>加载配置公网IP成功，启动检测公网IP访问状态</g>ip:<m>{ip}</m>')
-            url = f"http://{ip}:{get_driver().config.port}/TeenStudy/login"
-            logger.info(url)
-            try:
-                async with AsyncClient(headers=headers) as client:
-                    response = await client.get(url=url)
-                logger.debug(f"公网请求状态：{response.status_code}")
-                if response.status_code != 200:
-                    ip = ""
-                    logger.opt(colors=True).info(
-                        f'<u><y>[大学习数据库]</y></u><g>检测到配置公网ip地址无法通过外网访问，将自动获取公网IP</g>')
-                logger.opt(colors=True).success(
-                    f'<u><y>[大学习提交 Web UI]</y></u><g>配置外网IP设置成功</g>，外网访问地址为:<m>http://{ip}:{get_driver().config.port}/TeenStudy/login</m>')
-            except Exception as e:
-                logger.error(e)
-                ip = ""
-                logger.opt(colors=True).info(
-                    f'<u><y>[大学习数据库]</y></u><g>检测到配置公网ip地址无法通过外网访问，将自动配置局域网IP</g>')
         except AttributeError:
             ip = ''
             logger.opt(colors=True).info(
                 f'<u><y>[大学习数据库]</y></u><g>加载配置IP失败，未检测到配置ip，启动自动获取公网IP</g>')
         if not ip:
             async with AsyncClient(headers=headers) as client:
                 response = await client.get("http://ip.42.pl/raw")
             if response.status_code == 200:
                 ip = response.text.strip()
                 logger.opt(colors=True).info(
-                    f'<u><y>[大学习数据库]</y></u><g>自动获取公网IP成功，启动检测公网IP访问状态</g>ip:<m>{ip}</m>')
-                url = f"http://{ip}:{get_driver().config.port}/TeenStudy/login"
-                logger.info(url)
-                try:
-                    async with AsyncClient(headers=headers, timeout=5) as client:
-                        response = await client.get(url=url)
-                    logger.debug(f"公网请求状态:{response.status_code}")
-                    if response.status_code != 200:
-                        ip = ""
-                        logger.opt(colors=True).warning(
-                            f'<u><y>[大学习数据库]</y></u><g>检测到ip地址无法通过外网访问，将自动配置局域网IP，请手动在.env.prod文件中配置公网IP，配置格式：DXX_IP="您的公网IP"</g>')
-                    else:
-                        logger.opt(colors=True).success(
-                            f'<u><y>[大学习提交 Web UI]</y></u><g>自动获取外网IP成功</g>，外网访问地址为:<m>http://{ip}:{get_driver().config.port}/TeenStudy/login</m>')
-                except Exception as e:
-                    ip = ""
-                    logger.debug(e)
-                    logger.opt(colors=True).warning(
-                        f'<u><y>[大学习数据库]</y></u><g>检测到ip地址无法通过外网访问，将自动配置局域网IP，请手动在.env.prod文件中配置公网IP，配置格式：DXX_IP="您的公网IP"</g>')
+                    f'<u><y>[大学习数据库]</y></u><g>自动获取公网IP成功</g>ip:<m>{ip}</m>')
             else:
                 ip = ""
                 logger.opt(colors=True).warning(
                     f'<u><y>[大学习数据库]</y></u><g>自动获取公网IP失败，将自动配置局域网IP，请手动在.env.prod文件中配置公网IP，配置格式：DXX_IP="您的公网IP"</g>')
         if not ip:
             s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             s.connect(('114.114.114.114', 12345))
@@ -415,32 +381,14 @@
                     file=content
                 )
                 logger.opt(colors=True).success(
                     f"<u><y>[大学习数据库]</y></u> <m>{item['type']}-{item['name']}</m> <g>更新成功!</g>")
             except Exception as e:
                 logger.success(e)
                 continue
-    try:
-        if not await JiangXi.all().count():
-            with open(base_file_path + "dxx_jx.json", 'r', encoding='utf-8') as r:
-                obj = json.load(r)
-            for item in obj:
-                await JiangXi.create(
-                    time=time.time(),
-                    university_id=item['university_id'],
-                    university=item['university'],
-                    college_id=item['college_id'],
-                    college=item['college'],
-                    organization=item['organization'],
-                    organization_id=item['organization_id']
-                )
-            logger.opt(colors=True).success(
-                f"<u><y>[大学习数据库]</y></u> <m>江西共青团团支部数据</m> <g>更新成功!</g>")
-    except Exception as e:
-        logger.error(e)
     logger.opt(colors=True).success("<u><y>[大学习数据库]</y></u><g>➤➤➤➤➤资源数据更新完成✔✔✔✔✔</g>")
 
 
 async def get_end_pic():
     font_data = await Resource.filter(type="字体").values()
     answer = await Answer.all().order_by('time').values()
     title = '"青年大学习"' + answer[-1]["catalogue"]
@@ -496,71 +444,89 @@
     img.save(buf, format="PNG")
     base64_str = base64.b64encode(buf.getbuffer()).decode()
     content = "base64://" + base64_str
     return content
 
 
 async def to_hash(text: str) -> str:
+    """
+    哈希散列加密
+    :param text:待加密文本
+    :return: 加密文本
+    """
     return hashlib.sha256(text.encode("utf-8")).hexdigest()
 
 
+async def encrypt(text: str):
+    """
+    RSA加密
+    :param text: 待加密文本
+    :return: 加密文本
+    """
+    public_key = "-----BEGIN PUBLIC KEY-----\nMIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQD5uIDebA2qU746e/NVPiQSBA0Q3J8/G23zfrwMz4qoip1vuKaVZykuMtsAkCJFZhEcmuaOVl8nAor7cz/KZe8ZCNInbXp2kUQNjJiOPwEhkGiVvxvU5V5vCK4mzGZhhawF5cI/pw2GJDSKbXK05YHXVtOAmg17zB1iJf+ie28TbwIDAQAB\n-----END PUBLIC KEY-----"
+    rsa_key = RSA.importKey(public_key)
+    cipher = PKCS1_v1_5.new(rsa_key)
+    cipher_text = base64.b64encode(cipher.encrypt(text.encode()))
+    return cipher_text.decode()
+
+
 async def distribute_area(user_id: int, area: str) -> dict:
     if area == "湖北":
         return await dxx.hubei(user_id=user_id)
     elif area == "江西":
         return await dxx.jiangxi(user_id=user_id)
     elif area == "浙江":
         return await dxx.zhejiang(user_id=user_id)
     elif area == "上海":
         return await dxx.shanghai(user_id=user_id)
-    elif area == "江苏":
-        return await dxx.jiangsu(user_id=user_id)
     elif area == "安徽":
         return await dxx.anhui(user_id=user_id)
     elif area == "四川":
         return await dxx.sichuan(user_id=user_id)
     elif area == "山东":
         return await dxx.shandong(user_id=user_id)
     elif area == "重庆":
         return await dxx.chongqing(user_id=user_id)
     elif area == "吉林":
         return await dxx.jilin(user_id=user_id)
     elif area == "广东":
         return await dxx.guangdong(user_id=user_id)
-    elif area == "黑龙江":
-        return await dxx.heilongjiang(user_id=user_id)
+    elif area == "北京":
+        return await dxx.beijing(user_id=user_id)
+    elif area == "天津":
+        return await dxx.tianjin(user_id=user_id)
     else:
         return {
             "status": 404,
             "msg": "该地区暂未支持！"
         }
 
 
 async def distribute_area_url(province: str, user_id: int, group_id: int) -> dict:
     config = path.getConfig()
     if province == "湖北":
         province = "hubei"
     elif province == "江西":
         province = "jiangxi"
-    elif province == "江苏":
-        province = "jiangsu"
     elif province == "安徽":
         province = "anhui"
     elif province == "四川":
         province = "sichuan"
     elif province == "山东":
         province = "shandong"
     elif province == "重庆":
         province = "chongqing"
     elif province == "吉林":
         province = "jilin"
     elif province == "广东":
-        province="guangdong"
-    elif province == "黑龙江":
-        province = "heilongjiang"
+        province = "guangdong"
+    elif province == "北京":
+        province = "beijing"
+    elif province == "天津":
+        province = "tianjin"
     data = f"http://{config['DXX_IP']}:{config['DXX_PORT']}/TeenStudy/api/{province}?user_id={user_id}&group_id={group_id}"
     img = qrcode.make(data=data)
     buf = BytesIO()
     img.save(buf, format="PNG")
     base64_str = base64.b64encode(buf.getbuffer()).decode()
     content = "base64://" + base64_str
     return {
```

### Comparing `TeenStudy-0.1.9/TeenStudy/web/__init__.py` & `TeenStudy-0.2.0/TeenStudy/web/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         window.sessionStorage.clear()
         window.alert('登录验证失败或已失效，请重新登录')
     }
     return payload
 },
 '''
 DRIVER = get_driver()
-icon_path = 'https://i.328888.xyz/2023/02/23/xIh5k.png'
+icon_path = 'https://img1.imgtp.com/2023/06/11/sG4KdlpL.png'
 
 
 @DRIVER.on_startup
 async def init_web():
     app: FastAPI = nonebot.get_app()
     logger.opt(colors=True).info(
         f'<u><y>[大学习提交 Web UI]</y></u><g>启用成功</g>，本机访问地址为:<m>http://127.0.0.1:{DRIVER.config.port}/TeenStudy/login</m>')
@@ -43,23 +43,25 @@
     async def login():
         return login_page.render(
             site_title='TeenStudy | 登录',
             site_icon=icon_path
         )
 
     @app.get('/TeenStudy/home', response_class=HTMLResponse)
-    async def home(user_id: int):
+    async def home():
         return home_app.render(
             site_title='TeenStudy 首页',
             site_icon=icon_path,
+            routerModel="createBrowserHistory",
             requestAdaptor=requestAdaptor,
             responseAdaptor=responseAdaptor
         )
 
     @app.get("/TeenStudy/admin", response_class=HTMLResponse)
     async def admin():
         return admin_app.render(
             site_title='TeenStudy | 管理后台',
             site_icon=icon_path,
+            routerModel="createBrowserHistory",
             requestAdaptor=requestAdaptor,
             responseAdaptor=responseAdaptor
         )
```

### Comparing `TeenStudy-0.1.9/TeenStudy/web/api/add.py` & `TeenStudy-0.2.0/TeenStudy/web/api/add.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import json
 import re
 import time
 import urllib.parse
-from typing import Optional
 
+from bs4 import BeautifulSoup
+from ddddocr import DdddOcr
 from fastapi import APIRouter
 from fastapi.responses import HTMLResponse, JSONResponse, RedirectResponse
 from httpx import AsyncClient
+from nonebot import logger
 
-from ..pages.add import hubei_page, jiangxi_page, jiangsu_page, anhui_page, sichuan_page, shandong_page, \
-    chongqing_page, jilin_page, guangdong_page,heilongjiang_page
+from ..pages.add import hubei_page, jiangxi_page, anhui_page, sichuan_page, shandong_page, \
+    chongqing_page, jilin_page, guangdong_page, beijing_page, tianjin_page
 from ..utils.add import write_to_database
 from ...models.accuont import User, AddUser
-from ...models.dxx import JiangXi
+from ...utils.utils import encrypt
 
 route = APIRouter()
 
 
 @route.post("/add", response_class=JSONResponse)
 async def add(data: dict) -> JSONResponse:
     user_id = data["user_id"]
@@ -43,82 +45,68 @@
 
 @route.get("/hubei", response_class=HTMLResponse)
 async def hubei(user_id: int, group_id: int):
     result = await AddUser.filter(user_id=user_id, group_id=group_id, status="未通过").count()
     if result:
         return hubei_page.render(
             site_title='青春湖北 | TeenStudy',
-            site_icon="https://i.328888.xyz/2023/02/23/xIh5k.png"
+            site_icon="https://img1.imgtp.com/2023/06/11/sG4KdlpL.png"
         )
     return RedirectResponse(
         url="/TeenStudy/login"
     )
 
 
 @route.get("/jiangxi", response_class=HTMLResponse)
 async def jiangxi(user_id: int, group_id: int):
     result = await AddUser.filter(user_id=user_id, group_id=group_id, status="未通过").count()
     if result:
         return jiangxi_page.render(
             site_title='江西共青团 | TeenStudy',
-            site_icon="https://i.328888.xyz/2023/02/23/xIh5k.png"
+            site_icon="https://img1.imgtp.com/2023/06/11/sG4KdlpL.png"
         )
     return RedirectResponse(
         url="/TeenStudy/login"
     )
 
 
 @route.get("/organization", response_class=JSONResponse)
-async def organization(type: str, university: Optional[str] = None, college: Optional[str] = None) -> JSONResponse:
-    if type == "jx":
-        if university and college == "":
-            result = await JiangXi.filter(university=university).values()
-            if result:
+async def organization(pid: str) -> JSONResponse:
+    base_url = f'http://www.jxqingtuan.cn/pub/vol/config/organization?pid={pid}'
+    headers = {
+        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 Edg/113.0.1774.35'
+    }
+    if pid:
+        async with AsyncClient(headers=headers) as client:
+            response = await client.get(base_url)
+        if response.status_code == 200:
+            if response.json()["status"] == 200:
                 options = []
-                for item in result:
+                for item in response.json()["result"]:
                     x = {
-                        "label": item["college"],
-                        "value": item["college"]
+                        "label": item["title"],
+                        "value": item["title"] + "-" + item["id"]
                     }
                     if x in options:
                         continue
                     options.append({
-                        "label": item["college"],
-                        "value": item["college"]
+                        "label": item["title"],
+                        "value": item["title"] + "-" + item["id"]
                     })
                 return JSONResponse({
                     "status": 0,
                     "msg": "数据加载成功！",
                     "data": {
-                        "university": university,
                         "options": options
                     }
                 })
-        else:
-            result = await JiangXi.filter(university=university, college=college).values()
-            if result:
-                options = []
-                for item in result:
-                    options.append({
-                        "label": item["organization"],
-                        "value": item["organization_id"]
-                    })
-                return JSONResponse({
-                    "status": 0,
-                    "msg": "数据加载成功！",
-                    "data": {
-                        "university": university,
-                        "options": options,
-                    }
-                })
     return JSONResponse({
         "status": 0,
         "msg": "数据加载成功！",
         "data": {
-            "university": university,
             "options": []
         }
     })
 
 
 @route.get("/shanghai/{user_id}/{group_id}", response_class=HTMLResponse)
 async def shanghai(user_id: int, group_id: int, appid: str, openid: str, nickname: str, headimg: str, t: str):
@@ -231,15 +219,14 @@
                         data["organization_id"] = item["id"]
                         data["organization"] = item["title"]
             except Exception as e:
                 return JSONResponse({
                     "status": 500,
                     "msg": f"请选择好个人信息再扫码,错误信息：{e}"
                 })
-
             status = await write_to_database(data=data)
             if status:
                 return JSONResponse(
                     {
                         "status": 0,
                         "msg": "添加成功！"
                     }
@@ -250,96 +237,14 @@
                     "msg": "添加失败！"
                 })
     return RedirectResponse(
         url="/TeenStudy/login"
     )
 
 
-@route.post("/jiangsu/add", response_class=JSONResponse)
-async def jiangsu_add(data: dict) -> JSONResponse:
-    user_id = data["user_id"]
-    if await User.filter(user_id=user_id).count():
-        return JSONResponse({
-            "status": 0,
-            "msg": "添加失败！，用户信息存在！"
-        })
-    else:
-        cookie = data["cookie"]
-        headers = {
-            "Host": "service.jiangsugqt.org",
-            "Connection": "keep-alive",
-            "Upgrade-Insecure-Requests": '1',
-            "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220303.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3262 MMWEBSDK/20220204 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.20.2100(0x28001438) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/wxpic,image/tpg,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
-            "X-Requested-With": "com.tencent.mm",
-            "Sec-Fetch-Site": "none",
-            "Sec-Fetch-Mode": "navigate",
-            "Sec-Fetch-User": "?1",
-            "Referer": "https://service.jiangsugqt.org/youth-h5/",
-            "Sec-Fetch-Dest": "document",
-            "Accept-Encoding": "gzip, deflate",
-            "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
-            "Cookie": cookie
-        }
-        try:
-            url = "https://service.jiangsugqt.org/api/my"
-            async with AsyncClient(headers=headers) as client:
-                response = await client.get(url)
-            response.encoding = response.charset_encoding
-            result = response.json()
-            if result["status"] == 1:
-                data["dxx_id"] = result["data"]["user_id"]
-                data["name"] = result["data"]["username"]
-                if result["data"]["orga"]:
-                    data["university"] = result["data"]["orga"].split("-")[0].strip()[:-2]
-                    if "学院" in result["data"]["orga"].split("-")[1].strip():
-                        data["college"] = result["data"]["orga"].split("-")[1].strip()
-                    else:
-                        data["college"] = result["data"]["orga"].split("-")[-1].strip()
-                else:
-                    data["university"] = ""
-                    data["college"] = ""
-                status = await write_to_database(data=data)
-                if status:
-                    return JSONResponse(
-                        {
-                            "status": 0,
-                            "msg": "添加成功！"
-                        }
-                    )
-                else:
-                    return JSONResponse({
-                        "status": 500,
-                        "msg": "添加失败！"
-                    })
-            else:
-                return JSONResponse({
-                    "status": 500,
-                    "msg": "添加失败！"
-                })
-        except Exception as e:
-            return JSONResponse({
-                "status": 500,
-                "msg": f"添加失败!{e}"
-            })
-
-
-@route.get("/jiangsu", response_class=HTMLResponse)
-async def jiangsu(user_id: int, group_id: int):
-    result = await AddUser.filter(user_id=user_id, group_id=group_id, status="未通过").count()
-    if result:
-        return jiangsu_page.render(
-            site_title='江苏共青团 | TeenStudy',
-            site_icon="https://i.328888.xyz/2023/02/23/xIh5k.png"
-        )
-    return RedirectResponse(
-        url="/TeenStudy/login"
-    )
-
-
 @route.post("/anhui/add", response_class=JSONResponse)
 async def anhui_add(data: dict) -> JSONResponse:
     user_id = data["user_id"]
     if await User.filter(user_id=user_id).count():
         return JSONResponse({
             "status": 0,
             "msg": "添加失败！，用户信息存在！"
@@ -434,15 +339,15 @@
 
 @route.get("/anhui", response_class=HTMLResponse)
 async def jiangsu(user_id: int, group_id: int):
     result = await AddUser.filter(user_id=user_id, group_id=group_id, status="未通过").count()
     if result:
         return anhui_page.render(
             site_title='安徽共青团 | TeenStudy',
-            site_icon="https://i.328888.xyz/2023/02/23/xIh5k.png"
+            site_icon="https://img1.imgtp.com/2023/06/11/sG4KdlpL.png"
         )
     return RedirectResponse(
         url="/TeenStudy/login"
     )
 
 
 @route.post("/sichuan/add", response_class=HTMLResponse)
@@ -483,15 +388,15 @@
 
 @route.get("/sichuan", response_class=HTMLResponse)
 async def sichuan(user_id: int, group_id: int):
     result = await AddUser.filter(user_id=user_id, group_id=group_id, status="未通过").count()
     if result:
         return sichuan_page.render(
             site_title='天府新青年 | TeenStudy',
-            site_icon="https://i.328888.xyz/2023/02/23/xIh5k.png"
+            site_icon="https://img1.imgtp.com/2023/06/11/sG4KdlpL.png"
         )
     return RedirectResponse(
         url="/TeenStudy/login"
     )
 
 
 @route.post("/shandong/add", response_class=HTMLResponse)
@@ -562,15 +467,15 @@
 
 @route.get("/shandong", response_class=HTMLResponse)
 async def shandong(user_id: int, group_id: int):
     result = await AddUser.filter(user_id=user_id, group_id=group_id, status="未通过").count()
     if result:
         return shandong_page.render(
             site_title='青春山东 | TeenStudy',
-            site_icon="https://i.328888.xyz/2023/02/23/xIh5k.png"
+            site_icon="https://img1.imgtp.com/2023/06/11/sG4KdlpL.png"
         )
     return RedirectResponse(
         url="/TeenStudy/login"
     )
 
 
 @route.post("/chongqing/add", response_class=HTMLResponse)
@@ -636,15 +541,15 @@
 
 @route.get("/chongqing", response_class=HTMLResponse)
 async def chongqing(user_id: int, group_id: int):
     result = await AddUser.filter(user_id=user_id, group_id=group_id, status="未通过").count()
     if result:
         return chongqing_page.render(
             site_title='重庆共青团 | TeenStudy',
-            site_icon="https://i.328888.xyz/2023/02/23/xIh5k.png"
+            site_icon="https://img1.imgtp.com/2023/06/11/sG4KdlpL.png"
         )
     return RedirectResponse(
         url="/TeenStudy/login"
     )
 
 
 @route.post("/jilin/add", response_class=HTMLResponse)
@@ -710,15 +615,15 @@
 
 @route.get("/jilin", response_class=HTMLResponse)
 async def jilin(user_id: int, group_id: int):
     result = await AddUser.filter(user_id=user_id, group_id=group_id, status="未通过").count()
     if result:
         return jilin_page.render(
             site_title='吉青飞扬 | TeenStudy',
-            site_icon="https://i.328888.xyz/2023/02/23/xIh5k.png"
+            site_icon="https://img1.imgtp.com/2023/06/11/sG4KdlpL.png"
         )
     return RedirectResponse(
         url="/TeenStudy/login"
     )
 
 
 @route.post("/guangdong/add", response_class=HTMLResponse)
@@ -765,23 +670,23 @@
                         'Sec-Fetch-Site': 'same-origin',
                         'Sec-Fetch-Mode': 'cors',
                         'Referer': 'https://youthstudy.12355.net/h5/',
                         'Accept-Encoding': 'gzip, deflate',
                         'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7'
                     }
                     async with AsyncClient(headers=token_headers, timeout=30, max_redirects=5) as client:
-                        token_response = await client.post(url=token_url, data="sign="+urllib.parse.quote(content))
+                        token_response = await client.post(url=token_url, data="sign=" + urllib.parse.quote(content))
                     if token_response.json()["errno"] == 0:
                         token = token_response.json()['data']['entity']['token']
                         name = token_response.json()['data']['entity']['nickName']
                         organization_id = token_response.json()['data']['entity']['organizeId']
                         data["name"] = name
                         data["organization_id"] = organization_id
                         data["dxx_id"] = dxx_id
-                        data["token"]=token
+                        data["token"] = token
                         data.pop("url")
                         status = await write_to_database(data=data)
                         if status:
                             return JSONResponse(
                                 {
                                     "status": 0,
                                     "msg": "添加成功！"
@@ -805,151 +710,125 @@
 
 @route.get("/guangdong", response_class=HTMLResponse)
 async def guangdong(user_id: int, group_id: int):
     result = await AddUser.filter(user_id=user_id, group_id=group_id, status="未通过").count()
     if result:
         return guangdong_page.render(
             site_title='广东共青团 | TeenStudy',
-            site_icon="https://i.328888.xyz/2023/02/23/xIh5k.png"
+            site_icon="https://img1.imgtp.com/2023/06/11/sG4KdlpL.png"
         )
     return RedirectResponse(
         url="/TeenStudy/login"
     )
 
 
-@route.post("/heilongjiang/add", response_class=HTMLResponse)
-async def heilongjiang_add(data: dict) -> JSONResponse:
+@route.post("/beijing/add", response_class=HTMLResponse)
+async def beijing_add(data: dict) -> JSONResponse:
     user_id = data["user_id"]
     if await User.filter(user_id=user_id).count():
         return JSONResponse({
             "status": 500,
             "msg": "添加失败！，用户信息存在！"
         })
     else:
+        token = data["token"]
+        cookie = data["cookie"]
+        login_url = "https://m.bjyouth.net/site/login"
+        headers = {
+            "User-Agent": "Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Mobile/15E148 Safari/604.1 Edg/113.0.0.0", }
         try:
-            cookie = data["cookie"]
-            url = "http://tsw.ithyxy.com/h5/auth/info"
-            headers = {
-                "Host": "tsw.ithyxy.com",
-                "Connection": "keep-alive",
-                "Accept": "application/json, text/plain, */*",
-                "User-Agent": "Mozilla/5.0 (Linux; Android 12; M2007J3SC Build/SKQ1.220303.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/86.0.4240.99 XWEB/3262 MMWEBSDK/20220204 Mobile Safari/537.36 MMWEBID/6170 MicroMessenger/8.0.20.2100(0x28001438) Process/toolsmp WeChat/arm32 Weixin NetType/WIFI Language/zh_CN ABI/arm64",
-                "X-Requested-With": "com.tencent.mm",
-                "Referer": "http://tsw.ithyxy.com/login",
-                "Accept-Encoding": "gzip, deflate",
-                "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
-                "Cookie": cookie
-            }
             async with AsyncClient(headers=headers) as client:
-                response = await client.get(url, headers=headers)
-            response.encoding = response.charset_encoding
-            if response.status_code == 200 and response.json()["code"] == 200:
-                result = response.json()
-                data["name"] = result["data"]["name"]
-                data["gender"] = result["data"]["sex"]
-                data["mobile"] = result["data"]["phone"]
-                class_url = "http://tsw.ithyxy.com/h5/auth/class?id=0"
-                async with AsyncClient(headers=headers) as client:
-                    response = await client.get(url=class_url)
-                response.encoding = response.charset_encoding
-                if response.status_code == 200 and response.json()["code"] == 200:
-                    university_list = response.json()["data"]
-                    for x, item in enumerate(result["data"]["path"]):
-                        if x == 0:
-                            for item2 in university_list:
-                                if item == item2["id"]:
-                                    data["university_type"] = item2["name"]
-                                    break
-                        elif x == 1:
-                            async with AsyncClient(headers=headers) as client:
-                                response = await client.get(
-                                    url=f"http://tsw.ithyxy.com/h5/auth/class?id={result['data']['path'][0]}")
-                            response.encoding = response.charset_encoding
-                            if response.status_code == 200 and response.json()["code"] == 200:
-                                university_list = response.json()["data"]
-                                for item2 in university_list:
-                                    if item == item2["id"]:
-                                        data["university"] = item2["name"]
-                                        data["university_id"] = item
-                                        break
-                            else:
-                                data["university"] = item
-                                continue
-                        elif x == 2:
-                            async with AsyncClient(headers=headers) as client:
-                                response = await client.get(
-                                    url=f"http://tsw.ithyxy.com/h5/auth/class?id={result['data']['path'][1]}")
-                            response.encoding = response.charset_encoding
-                            if response.status_code == 200 and response.json()["code"] == 200:
-                                university_list = response.json()["data"]
-                                for item2 in university_list:
-                                    if item == item2["id"]:
-                                        data["college"] = item2["name"]
-                                        data["college_id"] = item
-                                        break
-                            else:
-                                data["college"] = item
-                                continue
-                        elif x == 3:
-                            async with AsyncClient(headers=headers) as client:
-                                response = await client.get(
-                                    url=f"http://tsw.ithyxy.com/h5/auth/class?id={result['data']['path'][2]}")
-                            response.encoding = response.charset_encoding
-                            if response.status_code == 200 and response.json()["code"] == 200:
-                                university_list = response.json()["data"]
-                                for item2 in university_list:
-                                    if item == item2["id"]:
-                                        data["organization"] = item2["name"]
-                                        data["organization_id"] = item
-                                        break
-                            else:
-                                data["organization"] = item
-                                continue
-                    status = await write_to_database(data=data)
-                    if status:
-                        return JSONResponse(
-                            {
-                                "status": 0,
-                                "msg": "添加成功！"
-                            }
-                        )
+                login_rsp = await client.get(login_url)
+                if login_rsp.status_code == 200:
+                    login_rsp.encoding = login_rsp.charset_encoding
+                    soup = BeautifulSoup(login_rsp.text, "lxml")
+                    code_url = "https://m.bjyouth.net" + soup.select("#verifyCode-image")[0].get("src")
+                    code_rsp = await client.get(code_url)
+                    code_text = DdddOcr(show_ad=False).classification(code_rsp.content)
+                    login_response = await client.post(
+                        url=login_url,
+                        data={
+                            '_csrf_mobile': client.cookies['_csrf_mobile'],
+                            'Login[password]': await encrypt(token),
+                            'Login[username]': await encrypt(cookie),
+                            'Login[verifyCode]': code_text
+                        }
+                    )
+                    logger.debug(login_response.text)
+                    if login_response.status_code == 200:
+                        login_response.encoding = login_response.charset_encoding
+                        if login_response.text == '8':
+                            return JSONResponse({"status": 500, "msg": "添加失败,验证码错误！"})
+                        if 'fail' in login_response.text:
+                            return JSONResponse({"status": 500, "msg": "添加失败,账号或密码错误！"})
+                        status = await write_to_database(data=data)
+                        if status:
+                            return JSONResponse(
+                                {
+                                    "status": 0,
+                                    "msg": "添加成功！"
+                                }
+                            )
+                        else:
+                            return JSONResponse({
+                                "status": 500,
+                                "msg": "添加失败！"
+                            })
                     else:
-                        return JSONResponse({
-                            "status": 500,
-                            "msg": "添加失败！"
-                        })
+                        return JSONResponse({"status": 500, "msg": "添加失败！"})
                 else:
-                    data["university"] = result["data"]["path"][0]
-                    data["college"] = result["data"]["path"][1]
-                    status = await write_to_database(data=data)
-                    if status:
-                        return JSONResponse(
-                            {
-                                "status": 0,
-                                "msg": "添加成功！"
-                            }
-                        )
-                    else:
-                        return JSONResponse({
-                            "status": 500,
-                            "msg": "添加失败！"
-                        })
-            else:
-                return JSONResponse({"status": 500, "msg": "添加失败！"})
+                    return JSONResponse({"status": 500, "msg": "添加失败！"})
         except Exception as e:
             return JSONResponse({
                 "status": 500,
-                "msg": f"添加失败,{e}"
+                "msg": f"# 添加失败,{e}"
             })
 
 
-@route.get("/heilongjiang", response_class=HTMLResponse)
-async def heilongjiang(user_id: int, group_id: int):
+@route.get("/beijing", response_class=HTMLResponse)
+async def beijing(user_id: int, group_id: int):
     result = await AddUser.filter(user_id=user_id, group_id=group_id, status="未通过").count()
     if result:
-        return heilongjiang_page.render(
-            site_title='黑龙江共青团 | TeenStudy',
-            site_icon="https://i.328888.xyz/2023/02/23/xIh5k.png"
+        return beijing_page.render(
+            site_title='北京共青团 | TeenStudy',
+            site_icon="https://img1.imgtp.com/2023/06/11/sG4KdlpL.png"
         )
     return RedirectResponse(
         url="/TeenStudy/login"
-    )
+    )
+
+
+@route.post("/tianjin/add", response_class=JSONResponse)
+async def tianjin_add(data: dict) -> JSONResponse:
+    user_id = data["user_id"]
+    if await User.filter(user_id=user_id).count():
+        return JSONResponse({
+            "status": 0,
+            "msg": "添加失败！，用户信息存在！"
+        })
+    else:
+        status = await write_to_database(data=data)
+        if status:
+            return JSONResponse(
+                {
+                    "status": 0,
+                    "msg": "添加成功！"
+                }
+            )
+        else:
+            return JSONResponse({
+                "status": 500,
+                "msg": "添加失败！"
+            })
+
+
+@route.get("/tianjin", response_class=HTMLResponse)
+async def hubei(user_id: int, group_id: int):
+    result = await AddUser.filter(user_id=user_id, group_id=group_id, status="未通过").count()
+    if result:
+        return tianjin_page.render(
+            site_title='津彩青春 | TeenStudy',
+            site_icon="https://img1.imgtp.com/2023/06/11/sG4KdlpL.png"
+        )
+    return RedirectResponse(
+        url="/TeenStudy/login"
+    )
```

### Comparing `TeenStudy-0.1.9/TeenStudy/web/api/admin.py` & `TeenStudy-0.2.0/TeenStudy/web/api/admin.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/TeenStudy/web/api/home.py` & `TeenStudy-0.2.0/TeenStudy/web/api/home.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import datetime
 from typing import Optional
 
-from fastapi import APIRouter
+from fastapi import APIRouter, Header
 from fastapi.responses import JSONResponse
 
-from .login import authentication
+from .login import authentication, get_userInfo
 from ...models.accuont import User, Commit
 from ...models.dxx import Answer
 from ...utils.rule import check_time
 from ...utils.utils import distribute_area
 from ...utils.utils import to_hash
 
 route = APIRouter()
 
 
 @route.get("/get_user", response_class=JSONResponse, dependencies=[authentication()])
-async def get_user(user_id: int) -> JSONResponse:
+async def get_user(token: Optional[str] = Header(...)) -> JSONResponse:
+    userinfo = await get_userInfo(token=token)
+    user_id = userinfo["user_id"]
     result = await User.filter(user_id=user_id).values()
     if result:
         data = result[0]
         try:
             data["commit_time"] = datetime.datetime.fromtimestamp(data['commit_time']).strftime(
                 "%Y-%m-%d %H:%M:%S")
         except TypeError:
```

### Comparing `TeenStudy-0.1.9/TeenStudy/web/api/login.py` & `TeenStudy-0.2.0/TeenStudy/web/api/login.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from fastapi import APIRouter
 from fastapi import Header, HTTPException, Depends
 from fastapi.responses import JSONResponse
 from jose import jwt
 from pydantic import BaseModel
 
 from ...models.accuont import User
-from ...utils.utils import to_hash
 from ...utils.path import getConfig
+from ...utils.utils import to_hash
 
 
 class UserModel(BaseModel):
     user_id: int
     password: str
     role: bool
 
@@ -50,46 +50,36 @@
             }
         }
     else:
         return {
             'status': 0,
             'msg': '登录成功',
             'data': {
-                'url': f"home?user_id={user_id}",
+                'url': f"/home?user_id={user_id}",
                 'role': role,
                 'user_id': user_id,
                 'token': token
             }
         }
 
 
-def user_authentication():
-    async def inner(token: Optional[str] = Header(...)):
-        result = getConfig()
-        key = result["KEY"]
-        algorithm = result["ALGORITHM"]
-        try:
-            payload = jwt.decode(token, key, algorithms=algorithm)
-            if not (user_id := payload.get('user_id')):
-                raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-            else:
-                try:
-                    role = payload.get('role')
-                    if role:
-                        raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-                    else:
-                        result = await User.filter(user_id=user_id).count()
-                        if not result:
-                            raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-                except (jwt.JWTError, jwt.ExpiredSignatureError, AttributeError):
-                    raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-        except (jwt.JWTError, jwt.ExpiredSignatureError, AttributeError):
-            raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
-
-    return Depends(inner)
+async def get_userInfo(token: str) -> dict:
+    """
+    返回用户信息
+    :param token: token值
+    :return:
+    """
+    result = getConfig()
+    key = result["KEY"]
+    algorithm = result["ALGORITHM"]
+    payload = jwt.decode(token, key, algorithms=algorithm)
+    return {
+        "user_id": payload.get("user_id"),
+        "role": payload.get("role")
+    }
 
 
 def admin_authentication():
     async def inner(token: Optional[str] = Header(...)):
         result = getConfig()
         key = result["KEY"]
         algorithm = result["ALGORITHM"]
```

### Comparing `TeenStudy-0.1.9/TeenStudy/web/pages/admin.py` & `TeenStudy-0.2.0/TeenStudy/web/pages/addArea.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,4607 +1,2886 @@
 00000000: 6672 6f6d 2061 6d69 7320 696d 706f 7274  from amis import
-00000010: 2041 7070 2c20 5061 6765 5363 6865 6d61   App, PageSchema
-00000020: 2c20 5461 626c 6543 6f6c 756d 6e2c 205c  , TableColumn, \
-00000030: 0d0a 2020 2020 4352 5544 2c20 4163 7469  ..    CRUD, Acti
-00000040: 6f6e 5479 7065 2c20 4c65 7665 6c45 6e75  onType, LevelEnu
-00000050: 6d2c 2043 6172 642c 2054 706c 2c20 4361  m, Card, Tpl, Ca
-00000060: 7264 7343 5255 442c 2044 6961 6c6f 672c  rdsCRUD, Dialog,
-00000070: 2044 6973 706c 6179 4d6f 6465 456e 756d   DisplayModeEnum
-00000080: 2c20 5365 6c65 6374 2c20 466c 6578 2c20  , Select, Flex, 
-00000090: 5365 7276 6963 652c 2041 6c65 7274 2c20  Service, Alert, 
-000000a0: 5072 6f70 6572 7479 2c20 5c0d 0a20 2020  Property, \..   
-000000b0: 2053 7769 7463 682c 2049 6e70 7574 5469   Switch, InputTi
-000000c0: 6d65 2c20 496e 7075 744e 756d 6265 720d  me, InputNumber.
-000000d0: 0a66 726f 6d20 616d 6973 2069 6d70 6f72  .from amis impor
-000000e0: 7420 4874 6d6c 2c20 5061 6765 2c20 466f  t Html, Page, Fo
-000000f0: 726d 2c20 496e 7075 7454 6578 740d 0a0d  rm, InputText...
-00000100: 0a6c 6f67 6f20 3d20 4874 6d6c 2868 746d  .logo = Html(htm
-00000110: 6c3d 6627 2727 0d0a 3c70 2061 6c69 676e  l=f'''..<p align
-00000120: 3d22 6365 6e74 6572 223e 0d0a 2020 2020  ="center">..    
-00000130: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000140: 2f67 6974 6875 622e 636f 6d2f 5a4d 3235  /github.com/ZM25
-00000150: 5843 2f54 6565 6e53 7475 6479 2f22 3e0d  XC/TeenStudy/">.
-00000160: 0a20 2020 2020 2020 203c 696d 6720 7372  .        <img sr
-00000170: 633d 2268 7474 7073 3a2f 2f69 2e33 3238  c="https://i.328
-00000180: 3838 382e 7879 7a2f 3230 3233 2f30 322f  888.xyz/2023/02/
-00000190: 3233 2f78 4968 356b 2e70 6e67 220d 0a20  23/xIh5k.png".. 
-000001a0: 2020 2020 2020 2020 7769 6474 683d 2232          width="2
-000001b0: 3536 2220 6865 6967 6874 3d22 3235 3622  56" height="256"
-000001c0: 2061 6c74 3d22 5465 656e 5374 7564 7922   alt="TeenStudy"
-000001d0: 3e0d 0a20 2020 203c 2f61 3e0d 0a3c 2f70  >..    </a>..</p
-000001e0: 3e0d 0a3c 6832 2061 6c69 676e 3d22 6365  >..<h2 align="ce
-000001f0: 6e74 6572 223e e5a4 a7e5 ada6 e4b9 a0e8  nter">..........
-00000200: 87aa e58a a8e6 8f90 e4ba a43c 2f68 323e  ...........</h2>
-00000210: 0d0a 3c64 6976 2061 6c69 676e 3d22 6365  ..<div align="ce
-00000220: 6e74 6572 223e 0d0a 2020 2020 3c61 2068  nter">..    <a h
-00000230: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00000240: 6875 622e 636f 6d2f 5a4d 3235 5843 2f54  hub.com/ZM25XC/T
-00000250: 6565 6e53 7475 6479 2f22 2074 6172 6765  eenStudy/" targe
-00000260: 743d 225f 626c 616e 6b22 3e0d 0a20 2020  t="_blank">..   
-00000270: 2047 6974 6875 62e4 bb93 e5ba 933c 2f61   Github......</a
-00000280: 3e0d 0a20 2020 203c 6120 6872 6566 3d22  >..    <a href="
-00000290: 6874 7470 733a 2f2f 6a71 2e71 712e 636f  https://jq.qq.co
-000002a0: 6d2f 3f5f 7776 3d31 3032 3726 6b3d 4e47  m/?_wv=1027&k=NG
-000002b0: 4645 7758 7953 2220 7461 7267 6574 3d22  FEwXyS" target="
-000002c0: 5f62 6c61 6e6b 223e e4ba a4e6 b581 e7be  _blank">........
-000002d0: a43c 2f61 3e0d 0a3c 2f64 6976 3e0d 0a3c  .</a>..</div>..<
-000002e0: 6272 3e0d 0a27 2727 290d 0a67 6974 6875  br>..''')..githu
-000002f0: 625f 6c6f 676f 203d 2054 706c 2863 6c61  b_logo = Tpl(cla
-00000300: 7373 4e61 6d65 3d27 772d 6675 6c6c 272c  ssName='w-full',
-00000310: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000320: 2020 2020 7470 6c3d 273c 6469 7620 636c      tpl='<div cl
-00000330: 6173 733d 2266 6c65 7820 6a75 7374 6966  ass="flex justif
-00000340: 792d 6265 7477 6565 6e22 3e3c 6469 763e  y-between"><div>
-00000350: 3c2f 6469 763e 3c64 6976 3e3c 6120 6872  </div><div><a hr
-00000360: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00000370: 7562 2e63 6f6d 2f5a 4d32 3558 432f 5465  ub.com/ZM25XC/Te
-00000380: 656e 5374 7564 7922 2074 6172 6765 743d  enStudy" target=
-00000390: 225f 626c 616e 6b22 2074 6974 6c65 3d22  "_blank" title="
-000003a0: 4769 7468 7562 20e4 bb93 e5ba 9322 3e3c  Github ......"><
-000003b0: 6920 636c 6173 733d 2266 6120 6661 2d67  i class="fa fa-g
-000003c0: 6974 6875 6220 6661 2d32 7822 3e3c 2f69  ithub fa-2x"></i
-000003d0: 3e3c 2f61 3e3c 2f64 6976 3e3c 2f64 6976  ></a></div></div
-000003e0: 3e27 290d 0a68 6561 6465 7220 3d20 466c  >')..header = Fl
-000003f0: 6578 2863 6c61 7373 4e61 6d65 3d27 772d  ex(className='w-
-00000400: 6675 6c6c 272c 206a 7573 7469 6679 3d27  full', justify='
-00000410: 666c 6578 2d65 6e64 272c 2061 6c69 676e  flex-end', align
-00000420: 4974 656d 733d 2766 6c65 782d 656e 6427  Items='flex-end'
-00000430: 2c20 6974 656d 733d 5b67 6974 6875 625f  , items=[github_
-00000440: 6c6f 676f 5d29 0d0a 2222 22e6 9cba e599  logo])..""".....
-00000450: a8e4 baba e78a b6e6 8081 e99d a2e6 9dbf  ................
-00000460: 2222 220d 0a73 7461 7475 7320 3d20 5365  """..status = Se
-00000470: 7276 6963 6528 0d0a 2020 2020 6170 693d  rvice(..    api=
-00000480: 272f 5465 656e 5374 7564 792f 6170 692f  '/TeenStudy/api/
-00000490: 7374 6174 7573 272c 0d0a 2020 2020 696e  status',..    in
-000004a0: 7465 7276 616c 3d36 3030 3030 2c0d 0a20  terval=60000,.. 
-000004b0: 2020 2062 6f64 793d 5b50 726f 7065 7274     body=[Propert
-000004c0: 7928 0d0a 2020 2020 2020 2020 7469 746c  y(..        titl
-000004d0: 653d 27e6 9cba e599 a8e4 baba e4bf a1e6  e='.............
-000004e0: 81af 272c 0d0a 2020 2020 2020 2020 636f  ..',..        co
-000004f0: 6c75 6d6e 3d32 2c0d 0a20 2020 2020 2020  lumn=2,..       
-00000500: 2069 7465 6d73 3d5b 0d0a 2020 2020 2020   items=[..      
-00000510: 2020 2020 2020 5072 6f70 6572 7479 2e49        Property.I
-00000520: 7465 6d28 0d0a 2020 2020 2020 2020 2020  tem(..          
-00000530: 2020 2020 2020 6c61 6265 6c3d 2742 6f74        label='Bot
-00000540: e698 b5e7 a7b0 272c 0d0a 2020 2020 2020  ......',..      
-00000550: 2020 2020 2020 2020 2020 636f 6e74 656e            conten
-00000560: 743d 2724 7b6e 6963 6b6e 616d 657d 270d  t='${nickname}'.
-00000570: 0a20 2020 2020 2020 2020 2020 2029 2c0d  .            ),.
-00000580: 0a20 2020 2020 2020 2020 2020 2050 726f  .            Pro
-00000590: 7065 7274 792e 4974 656d 280d 0a20 2020  perty.Item(..   
-000005a0: 2020 2020 2020 2020 2020 2020 206c 6162               lab
-000005b0: 656c 3d27 426f 7420 7171 e58f b727 2c0d  el='Bot qq...',.
-000005c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000005d0: 2063 6f6e 7465 6e74 3d27 247b 626f 745f   content='${bot_
-000005e0: 6964 7d27 0d0a 2020 2020 2020 2020 2020  id}'..          
-000005f0: 2020 292c 0d0a 2020 2020 2020 2020 2020    ),..          
-00000600: 2020 5072 6f70 6572 7479 2e49 7465 6d28    Property.Item(
-00000610: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000620: 2020 6c61 6265 6c3d 2742 6f74 e5a5 bde5    label='Bot....
-00000630: 8f8b e695 b0e9 878f 272c 0d0a 2020 2020  ........',..    
-00000640: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00000650: 656e 743d 2724 7b66 7269 656e 645f 636f  ent='${friend_co
-00000660: 756e 747d 270d 0a20 2020 2020 2020 2020  unt}'..         
-00000670: 2020 2029 2c0d 0a20 2020 2020 2020 2020     ),..         
-00000680: 2020 2050 726f 7065 7274 792e 4974 656d     Property.Item
-00000690: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-000006a0: 2020 206c 6162 656c 3d27 426f 74e7 bea4     label='Bot...
-000006b0: e881 8ae6 95b0 e987 8f27 2c0d 0a20 2020  .........',..   
-000006c0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-000006d0: 7465 6e74 3d27 247b 6772 6f75 705f 636f  tent='${group_co
-000006e0: 756e 747d 270d 0a20 2020 2020 2020 2020  unt}'..         
-000006f0: 2020 2029 2c0d 0a20 2020 2020 2020 2020     ),..         
-00000700: 2020 2050 726f 7065 7274 792e 4974 656d     Property.Item
-00000710: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00000720: 2020 206c 6162 656c 3d27 426f 74e5 90af     label='Bot...
-00000730: e58a a8e6 97b6 e997 b427 2c0d 0a20 2020  .........',..   
-00000740: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00000750: 7465 6e74 3d27 247b 7374 6172 745f 7469  tent='${start_ti
-00000760: 6d65 7d27 0d0a 2020 2020 2020 2020 2020  me}'..          
-00000770: 2020 292c 0d0a 2020 2020 2020 2020 2020    ),..          
-00000780: 2020 5072 6f70 6572 7479 2e49 7465 6d28    Property.Item(
-00000790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000007a0: 2020 6c61 6265 6c3d 27e7 b3bb e7bb 9fe5    label='.......
-000007b0: 90af e58a a8e6 97b6 e997 b427 2c0d 0a20  ...........',.. 
-000007c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000007d0: 6f6e 7465 6e74 3d27 247b 7379 7374 656d  ontent='${system
-000007e0: 5f73 7461 7274 5f74 696d 657d 270d 0a20  _start_time}'.. 
-000007f0: 2020 2020 2020 2020 2020 2029 2c0d 0a20             ),.. 
-00000800: 2020 2020 2020 2020 2020 2050 726f 7065             Prope
-00000810: 7274 792e 4974 656d 280d 0a20 2020 2020  rty.Item(..     
-00000820: 2020 2020 2020 2020 2020 206c 6162 656c             label
-00000830: 3d27 e980 9ae7 9fa5 e7be a4e6 95b0 e987  ='..............
-00000840: 8f27 2c0d 0a20 2020 2020 2020 2020 2020  .',..           
-00000850: 2020 2020 2063 6f6e 7465 6e74 3d27 247b       content='${
-00000860: 6e6f 7469 6365 5f63 6f75 6e74 7d27 0d0a  notice_count}'..
-00000870: 2020 2020 2020 2020 2020 2020 292c 0d0a              ),..
-00000880: 2020 2020 2020 2020 2020 2020 5072 6f70              Prop
-00000890: 6572 7479 2e49 7465 6d28 0d0a 2020 2020  erty.Item(..    
-000008a0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-000008b0: 6c3d 27e7 94a8 e688 b7e6 95b0 e987 8f27  l='............'
-000008c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000008d0: 2020 2063 6f6e 7465 6e74 3d27 247b 7573     content='${us
-000008e0: 6572 5f63 6f75 6e74 7d27 0d0a 2020 2020  er_count}'..    
-000008f0: 2020 2020 2020 2020 292c 0d0a 2020 2020          ),..    
-00000900: 2020 2020 2020 2020 5072 6f70 6572 7479          Property
-00000910: 2e49 7465 6d28 0d0a 2020 2020 2020 2020  .Item(..        
-00000920: 2020 2020 2020 2020 6c61 6265 6c3d 27e6          label='.
-00000930: 94af e68c 81e5 9cb0 e58c bae6 95b0 e987  ................
-00000940: 8f27 2c0d 0a20 2020 2020 2020 2020 2020  .',..           
-00000950: 2020 2020 2063 6f6e 7465 6e74 3d27 247b       content='${
-00000960: 6172 6561 5f63 6f75 6e74 7d27 0d0a 2020  area_count}'..  
-00000970: 2020 2020 2020 2020 2020 292c 2050 726f            ), Pro
-00000980: 7065 7274 792e 4974 656d 280d 0a20 2020  perty.Item(..   
-00000990: 2020 2020 2020 2020 2020 2020 206c 6162               lab
-000009a0: 656c 3d27 e69c 80e6 96b0 e4b8 80e6 9c9f  el='............
-000009b0: e5a4 a7e5 ada6 e4b9 a027 2c0d 0a20 2020  .........',..   
-000009c0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-000009d0: 7465 6e74 3d27 247b 6361 7461 6c6f 6775  tent='${catalogu
-000009e0: 657d 270d 0a20 2020 2020 2020 2020 2020  e}'..           
-000009f0: 2029 2c20 5072 6f70 6572 7479 2e49 7465   ), Property.Ite
-00000a00: 6d28 0d0a 2020 2020 2020 2020 2020 2020  m(..            
-00000a10: 2020 2020 6c61 6265 6c3d 27e5 85ac e7bd      label='.....
-00000a20: 91e8 aebf e997 ae49 5027 2c0d 0a20 2020  .......IP',..   
-00000a30: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00000a40: 7465 6e74 3d27 247b 6970 7d27 0d0a 2020  tent='${ip}'..  
-00000a50: 2020 2020 2020 2020 2020 292c 0d0a 2020            ),..  
-00000a60: 2020 2020 2020 2020 2020 5072 6f70 6572            Proper
-00000a70: 7479 2e49 7465 6d28 0d0a 2020 2020 2020  ty.Item(..      
-00000a80: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
-00000a90: 2743 5055 e58d a0e7 94a8 e78e 8727 2c0d  'CPU.........',.
-00000aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000ab0: 2063 6f6e 7465 6e74 3d27 247b 6370 755f   content='${cpu_
-00000ac0: 7065 7263 656e 747d 270d 0a20 2020 2020  percent}'..     
-00000ad0: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
-00000ae0: 2020 2020 2020 2050 726f 7065 7274 792e         Property.
-00000af0: 4974 656d 280d 0a20 2020 2020 2020 2020  Item(..         
-00000b00: 2020 2020 2020 206c 6162 656c 3d27 5241         label='RA
-00000b10: 4de5 8da0 e794 a8e7 8e87 272c 0d0a 2020  M.........',..  
-00000b20: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00000b30: 6e74 656e 743d 2724 7b72 616d 5f70 6572  ntent='${ram_per
-00000b40: 6365 6e74 7d27 0d0a 2020 2020 2020 2020  cent}'..        
-00000b50: 2020 2020 292c 0d0a 2020 2020 2020 2020      ),..        
-00000b60: 2020 2020 5072 6f70 6572 7479 2e49 7465      Property.Ite
-00000b70: 6d28 0d0a 2020 2020 2020 2020 2020 2020  m(..            
-00000b80: 2020 2020 6c61 6265 6c3d 2753 5741 50e5      label='SWAP.
-00000b90: 8da0 e794 a8e7 8e87 272c 0d0a 2020 2020  ........',..    
-00000ba0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00000bb0: 656e 743d 2724 7b73 7761 705f 7065 7263  ent='${swap_perc
-00000bc0: 656e 747d 272c 0d0a 2020 2020 2020 2020  ent}',..        
-00000bd0: 2020 2020 292c 0d0a 2020 2020 2020 2020      ),..        
-00000be0: 5d0d 0a20 2020 2029 5d0d 0a29 0d0a 2222  ]..    )]..)..""
-00000bf0: 22e6 8f90 e4ba a4e8 aeb0 e5bd 95e6 a8a1  "...............
-00000c00: e69d bf22 2222 0d0a 7265 636f 7264 5f74  ..."""..record_t
-00000c10: 6162 6c65 203d 2043 5255 4428 6d6f 6465  able = CRUD(mode
-00000c20: 3d27 7461 626c 6527 2c0d 0a20 2020 2020  ='table',..     
-00000c30: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00000c40: 6974 6c65 3d27 272c 0d0a 2020 2020 2020  itle='',..      
-00000c50: 2020 2020 2020 2020 2020 2020 2020 7379                sy
-00000c60: 6e63 4c6f 6361 7469 6f6e 3d46 616c 7365  ncLocation=False
-00000c70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000c80: 2020 2020 2020 2061 7069 3d27 2f54 6565         api='/Tee
-00000c90: 6e53 7475 6479 2f61 7069 2f67 6574 5f72  nStudy/api/get_r
-00000ca0: 6563 6f72 6473 272c 0d0a 2020 2020 2020  ecords',..      
-00000cb0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00000cc0: 7465 7276 616c 3d36 3030 3030 2c0d 0a20  terval=60000,.. 
-00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ce0: 2020 2074 7970 653d 2763 7275 6427 2c0d     type='crud',.
-00000cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000d00: 2020 2020 2068 6561 6465 7254 6f6f 6c62       headerToolb
-00000d10: 6172 3d5b 4163 7469 6f6e 5479 7065 2e41  ar=[ActionType.A
-00000d20: 6a61 7828 6c61 6265 6c3d 27e5 88a0 e999  jax(label='.....
-00000d30: a4e6 8980 e69c 89e6 8f90 e4ba a4e8 aeb0  ................
-00000d40: e5bd 9527 2c0d 0a20 2020 2020 2020 2020  ...',..         
-00000d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d70: 2020 2020 2020 2020 2020 6c65 7665 6c3d            level=
-00000d80: 4c65 7665 6c45 6e75 6d2e 7761 726e 696e  LevelEnum.warnin
-00000d90: 672c 0d0a 2020 2020 2020 2020 2020 2020  g,..            
-00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000dc0: 2020 2020 2020 2063 6f6e 6669 726d 5465         confirmTe
-00000dd0: 7874 3d27 e7a1 aee5 ae9a e8a6 81e5 88a0  xt='............
-00000de0: e999 a4e6 8980 e69c 89e6 8f90 e4ba a4e8  ................
-00000df0: aeb0 e5bd 95e5 9097 efbc 9f27 2c0d 0a20  ...........',.. 
-00000e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e30: 2020 6170 693d 2764 656c 6574 653a 2f54    api='delete:/T
-00000e40: 6565 6e53 7475 6479 2f61 7069 2f64 656c  eenStudy/api/del
-00000e50: 6574 655f 616c 6c3f 7479 7065 3d72 6563  ete_all?type=rec
-00000e60: 6f72 6473 2729 2c0d 0a20 2020 2020 2020  ords'),..       
-00000e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e80: 2020 2020 2020 2020 2020 2020 2262 756c              "bul
-00000e90: 6b41 6374 696f 6e73 222c 2022 7265 6c6f  kActions", "relo
-00000ea0: 6164 225d 2c0d 0a20 2020 2020 2020 2020  ad"],..         
-00000eb0: 2020 2020 2020 2020 2020 2069 7465 6d41             itemA
-00000ec0: 6374 696f 6e73 3d5b 0d0a 2020 2020 2020  ctions=[..      
-00000ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ee0: 2020 4163 7469 6f6e 5479 7065 2e41 6a61    ActionType.Aja
-00000ef0: 7828 746f 6f6c 7469 703d 27e5 88a0 e999  x(tooltip='.....
-00000f00: a427 2c0d 0a20 2020 2020 2020 2020 2020  .',..           
-00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f20: 2020 2020 2020 2020 2020 2020 2069 636f               ico
-00000f30: 6e3d 2766 6120 6661 2d74 696d 6573 2074  n='fa fa-times t
-00000f40: 6578 742d 6461 6e67 6572 272c 0d0a 2020  ext-danger',..  
-00000f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f70: 2020 2020 2020 636f 6e66 6972 6d54 6578        confirmTex
-00000f80: 743d 27e5 88a0 e999 a4e8 afa5 e69d a1e6  t='.............
-00000f90: 8f90 e4ba a4e8 aeb0 e5bd 9527 2c0d 0a20  ...........',.. 
-00000fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 2020 2020 2020 2061 7069 3d27 6465 6c65         api='dele
-00000fd0: 7465 3a2f 5465 656e 5374 7564 792f 6170  te:/TeenStudy/ap
-00000fe0: 692f 6465 6c65 7465 5f72 6563 6f72 643f  i/delete_record?
-00000ff0: 6964 3d24 7b69 647d 2729 0d0a 2020 2020  id=${id}')..    
-00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001010: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00001020: 2020 2020 2020 2020 666f 6f74 6162 6c65          footable
-00001030: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
-00001040: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
-00001050: 6d6e 733d 5b0d 0a20 2020 2020 2020 2020  mns=[..         
-00001060: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-00001070: 6162 6c65 436f 6c75 6d6e 286c 6162 656c  ableColumn(label
-00001080: 3d27 e794 a8e6 88b7 4944 272c 206e 616d  ='......ID', nam
-00001090: 653d 2775 7365 725f 6964 272c 2073 6561  e='user_id', sea
-000010a0: 7263 6861 626c 653d 5472 7565 292c 0d0a  rchable=True),..
-000010b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010c0: 2020 2020 2020 2020 5461 626c 6543 6f6c          TableCol
-000010d0: 756d 6e28 6c61 6265 6c3d 27e5 a793 e590  umn(label='.....
-000010e0: 8d27 2c20 6e61 6d65 3d27 6e61 6d65 272c  .', name='name',
-000010f0: 2073 6561 7263 6861 626c 653d 5472 7565   searchable=True
-00001100: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-00001110: 2020 2020 2020 2020 2020 2020 5461 626c              Tabl
-00001120: 6543 6f6c 756d 6e28 6c61 6265 6c3d 27e6  eColumn(label='.
-00001130: 8f90 e4ba a4e5 9cb0 e58c ba27 2c20 6e61  ...........', na
-00001140: 6d65 3d27 6172 6561 272c 2073 6561 7263  me='area', searc
-00001150: 6861 626c 653d 5472 7565 292c 0d0a 2020  hable=True),..  
-00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001170: 2020 2020 2020 5461 626c 6543 6f6c 756d        TableColum
-00001180: 6e28 6c61 6265 6c3d 27e5 ada6 e6a0 a1e5  n(label='.......
-00001190: 908d e7a7 b027 2c20 6e61 6d65 3d27 756e  .....', name='un
-000011a0: 6976 6572 7369 7479 272c 2073 6561 7263  iversity', searc
-000011b0: 6861 626c 653d 5472 7565 292c 0d0a 2020  hable=True),..  
-000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011d0: 2020 2020 2020 5461 626c 6543 6f6c 756d        TableColum
-000011e0: 6e28 6c61 6265 6c3d 27e5 ada6 e999 a2e5  n(label='.......
-000011f0: 908d e7a7 b027 2c20 6e61 6d65 3d27 636f  .....', name='co
-00001200: 6c6c 6567 6527 2c20 7365 6172 6368 6162  llege', searchab
-00001210: 6c65 3d54 7275 6529 2c0d 0a20 2020 2020  le=True),..     
-00001220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001230: 2020 2054 6162 6c65 436f 6c75 6d6e 286c     TableColumn(l
-00001240: 6162 656c 3d27 e59b a2e6 94af e983 a827  abel='.........'
-00001250: 2c20 6e61 6d65 3d27 6f72 6761 6e69 7a61  , name='organiza
-00001260: 7469 6f6e 272c 2073 6561 7263 6861 626c  tion', searchabl
-00001270: 653d 5472 7565 292c 0d0a 2020 2020 2020  e=True),..      
-00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001290: 2020 5461 626c 6543 6f6c 756d 6e28 6c61    TableColumn(la
-000012a0: 6265 6c3d 27e6 8f90 e4ba a4e6 9c9f e695  bel='...........
-000012b0: b027 2c20 6e61 6d65 3d27 6361 7461 6c6f  .', name='catalo
-000012c0: 6775 6527 2c20 7365 6172 6368 6162 6c65  gue', searchable
-000012d0: 3d54 7275 6529 2c0d 0a20 2020 2020 2020  =True),..       
-000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012f0: 2054 6162 6c65 436f 6c75 6d6e 286c 6162   TableColumn(lab
-00001300: 656c 3d27 e68f 90e4 baa4 e78a b6e6 8081  el='............
-00001310: 272c 206e 616d 653d 2724 7b73 7461 7475  ', name='${statu
-00001320: 733d 3d74 7275 653f 22e6 8890 e58a 9f22  s==true?"......"
-00001330: 3a22 e5a4 b1e8 b4a5 227d 272c 2073 6561  :"......"}', sea
-00001340: 7263 6861 626c 653d 5472 7565 292c 0d0a  rchable=True),..
-00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001360: 2020 2020 2020 2020 5461 626c 6543 6f6c          TableCol
-00001370: 756d 6e28 7479 7065 3d27 7470 6c27 2c20  umn(type='tpl', 
-00001380: 7470 6c3d 2724 7b74 696d 657c 6461 7465  tpl='${time|date
-00001390: 3a59 5959 592d 4d4d 2d44 4420 4848 5c5c  :YYYY-MM-DD HH\\
-000013a0: 3a6d 6d5c 5c3a 7373 7d27 2c0d 0a20 2020  :mm\\:ss}',..   
-000013b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013d0: 206c 6162 656c 3d27 e68f 90e4 baa4 e697   label='........
-000013e0: b6e9 97b4 272c 0d0a 2020 2020 2020 2020  ....',..        
-000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001400: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00001410: 3d27 7469 6d65 272c 2073 6f72 7461 626c  ='time', sortabl
-00001420: 653d 5472 7565 290d 0a20 2020 2020 2020  e=True)..       
-00001430: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
-00001440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001450: 2020 2020 2062 756c 6b41 6374 696f 6e73       bulkActions
-00001460: 3d5b 0d0a 2020 2020 2020 2020 2020 2020  =[..            
-00001470: 2020 2020 2020 2020 2020 2020 4163 7469              Acti
-00001480: 6f6e 5479 7065 2e41 6a61 7828 6c61 6265  onType.Ajax(labe
-00001490: 6c3d 27e6 89b9 e987 8fe5 88a0 e999 a427  l='............'
-000014a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000014b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014c0: 2020 2020 2020 2020 2020 206c 6576 656c             level
-000014d0: 3d4c 6576 656c 456e 756d 2e77 6172 6e69  =LevelEnum.warni
-000014e0: 6e67 2c0d 0a20 2020 2020 2020 2020 2020  ng,..           
-000014f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001500: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00001510: 6669 726d 5465 7874 3d22 e7a1 aee5 ae9a  firmText="......
-00001520: e8a6 81e6 89b9 e987 8fe5 88a0 e999 a4ef  ................
-00001530: bc9f 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
-00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001550: 2020 2020 2020 2020 2020 2020 2020 6170                ap
-00001560: 693d 2264 656c 6574 653a 2f54 6565 6e53  i="delete:/TeenS
-00001570: 7475 6479 2f61 7069 2f64 656c 6574 655f  tudy/api/delete_
-00001580: 7265 636f 7264 733f 6964 733d 247b 6964  records?ids=${id
-00001590: 737c 7261 777d 2229 5d29 0d0a 616e 7377  s|raw}")])..answ
-000015a0: 6572 5f74 6162 6c65 203d 2043 5255 4428  er_table = CRUD(
-000015b0: 6d6f 6465 3d27 7461 626c 6527 2c0d 0a20  mode='table',.. 
-000015c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015d0: 2020 2074 6974 6c65 3d27 272c 0d0a 2020     title='',..  
-000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015f0: 2020 7379 6e63 4c6f 6361 7469 6f6e 3d46    syncLocation=F
-00001600: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
-00001610: 2020 2020 2020 2020 2020 2061 7069 3d27             api='
-00001620: 2f54 6565 6e53 7475 6479 2f61 7069 2f67  /TeenStudy/api/g
-00001630: 6574 5f61 6e73 7765 7273 272c 0d0a 2020  et_answers',..  
-00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001650: 2020 7479 7065 3d27 6372 7564 272c 0d0a    type='crud',..
-00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001670: 2020 2020 6865 6164 6572 546f 6f6c 6261      headerToolba
-00001680: 723d 5b41 6374 696f 6e54 7970 652e 416a  r=[ActionType.Aj
-00001690: 6178 286c 6162 656c 3d27 e588 a0e9 99a4  ax(label='......
-000016a0: e99d 92e5 b9b4 e5a4 a7e5 ada6 e4b9 a0e6  ................
-000016b0: 9c9f e695 b027 2c0d 0a20 2020 2020 2020  .....',..       
-000016c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000010: 2049 6e70 7574 5465 7874 2c20 466f 726d   InputText, Form
+00000020: 2c20 4469 7370 6c61 794d 6f64 6545 6e75  , DisplayModeEnu
+00000030: 6d2c 2041 6c65 7274 2c20 4c65 7665 6c45  m, Alert, LevelE
+00000040: 6e75 6d2c 2053 656c 6563 742c 2050 6167  num, Select, Pag
+00000050: 6553 6368 656d 610d 0a66 726f 6d20 616d  eSchema..from am
+00000060: 6973 2069 6d70 6f72 7420 5061 6765 2c20  is import Page, 
+00000070: 4163 7469 6f6e 5479 7065 2c20 4469 616c  ActionType, Dial
+00000080: 6f67 2c20 4361 7264 2c20 5470 6c2c 2053  og, Card, Tpl, S
+00000090: 7769 7463 682c 2043 6172 6473 4352 5544  witch, CardsCRUD
+000000a0: 0d0a 0d0a 6465 7461 696c 5f66 6f72 6d20  ....detail_form 
+000000b0: 3d20 466f 726d 280d 0a20 2020 2074 6974  = Form(..    tit
+000000c0: 6c65 3d27 272c 0d0a 2020 2020 6170 693d  le='',..    api=
+000000d0: 2770 7574 3a2f 5465 656e 5374 7564 792f  'put:/TeenStudy/
+000000e0: 6170 692f 6368 616e 6765 3f75 7365 725f  api/change?user_
+000000f0: 6964 3d24 7b75 7365 725f 6964 7d27 2c0d  id=${user_id}',.
+00000100: 0a20 2020 2073 7562 6d69 7454 6578 743d  .    submitText=
+00000110: 27e4 bf9d e5ad 98e4 bfae e694 b927 2c0d  '............',.
+00000120: 0a20 2020 206d 6f64 653d 4469 7370 6c61  .    mode=Displa
+00000130: 794d 6f64 6545 6e75 6d2e 686f 7269 7a6f  yModeEnum.horizo
+00000140: 6e74 616c 2c0d 0a20 2020 206c 6162 656c  ntal,..    label
+00000150: 416c 6967 6e3d 2772 6967 6874 272c 0d0a  Align='right',..
+00000160: 2020 2020 626f 6479 3d5b 0d0a 2020 2020      body=[..    
+00000170: 2020 2020 5365 6c65 6374 280d 0a20 2020      Select(..   
+00000180: 2020 2020 2020 2020 206c 6162 656c 3d22           label="
+00000190: e980 9ae7 9fa5 e7be a4e8 818a 222c 0d0a  ............",..
+000001a0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+000001b0: 3d22 6772 6f75 705f 6964 222c 0d0a 2020  ="group_id",..  
+000001c0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+000001d0: 7074 696f 6e3d 22e5 a4a7 e5ad a6e4 b9a0  ption=".........
+000001e0: e68f 90e9 8692 e7be a4e5 8fb7 222c 0d0a  ............",..
+000001f0: 2020 2020 2020 2020 2020 2020 6368 6563              chec
+00000200: 6b41 6c6c 3d46 616c 7365 2c0d 0a20 2020  kAll=False,..   
+00000210: 2020 2020 2020 2020 2073 6f75 7263 653d           source=
+00000220: 2267 6574 3a2f 5465 656e 5374 7564 792f  "get:/TeenStudy/
+00000230: 6170 692f 6765 745f 6772 6f75 705f 6c69  api/get_group_li
+00000240: 7374 222c 0d0a 2020 2020 2020 2020 2020  st",..          
+00000250: 2020 7661 6c75 653d 2724 7b67 726f 7570    value='${group
+00000260: 5f69 647d 272c 0d0a 2020 2020 2020 2020  _id}',..        
+00000270: 2020 2020 6d75 6c74 6970 6c65 3d46 616c      multiple=Fal
+00000280: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
+00000290: 2072 6571 7569 7265 643d 5472 7565 2c0d   required=True,.
+000002a0: 0a20 2020 2020 2020 2020 2020 2073 6561  .            sea
+000002b0: 7263 6861 626c 653d 5472 7565 2c0d 0a20  rchable=True,.. 
+000002c0: 2020 2020 2020 2020 2020 206a 6f69 6e56             joinV
+000002d0: 616c 7565 733d 4661 6c73 652c 0d0a 2020  alues=False,..  
+000002e0: 2020 2020 2020 2020 2020 6578 7472 6163            extrac
+000002f0: 7456 616c 7565 3d54 7275 652c 0d0a 2020  tValue=True,..  
+00000300: 2020 2020 2020 2020 2020 7374 6174 6973            statis
+00000310: 7469 6373 3d54 7275 652c 0d0a 2020 2020  tics=True,..    
+00000320: 2020 2020 292c 0d0a 2020 2020 2020 2020      ),..        
+00000330: 496e 7075 7454 6578 7428 6c61 6265 6c3d  InputText(label=
+00000340: 27e6 80a7 e588 ab27 2c20 6e61 6d65 3d27  '......', name='
+00000350: 6765 6e64 6572 272c 2076 616c 7565 3d27  gender', value='
+00000360: 247b 6765 6e64 6572 7d27 2c20 7265 7175  ${gender}', requ
+00000370: 6972 6564 3d54 7275 652c 0d0a 2020 2020  ired=True,..    
+00000380: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00000390: 696d 436f 6e74 656e 7473 3d54 7275 652c  imContents=True,
+000003a0: 2063 6c65 6172 6162 6c65 3d54 7275 652c   clearable=True,
+000003b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000003c0: 2020 2020 7368 6f77 436f 756e 7465 723d      showCounter=
+000003d0: 5472 7565 2c20 6d61 784c 656e 6774 683d  True, maxLength=
+000003e0: 332c 2076 6973 6962 6c65 4f6e 3d22 247b  3, visibleOn="${
+000003f0: 6765 6e64 6572 3d3d 6e75 6c6c 3f66 616c  gender==null?fal
+00000400: 7365 3a74 7275 657d 222c 0d0a 2020 2020  se:true}",..    
+00000410: 2020 2020 2020 2020 2020 2020 2020 6465                de
+00000420: 7363 7269 7074 696f 6e3d 27e6 80a7 e588  scription='.....
+00000430: ab27 292c 0d0a 2020 2020 2020 2020 496e  .'),..        In
+00000440: 7075 7454 6578 7428 6c61 6265 6c3d 2775  putText(label='u
+00000450: 6964 7c6e 6964 272c 206e 616d 653d 2764  id|nid', name='d
+00000460: 7878 5f69 6427 2c20 7661 6c75 653d 2724  xx_id', value='$
+00000470: 7b64 7878 5f69 647d 272c 2072 6571 7569  {dxx_id}', requi
+00000480: 7265 643d 5472 7565 2c0d 0a20 2020 2020  red=True,..     
+00000490: 2020 2020 2020 2020 2020 2020 2074 7269               tri
+000004a0: 6d43 6f6e 7465 6e74 733d 5472 7565 2c20  mContents=True, 
+000004b0: 636c 6561 7261 626c 653d 5472 7565 2c0d  clearable=True,.
+000004c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000004d0: 2020 2073 686f 7743 6f75 6e74 6572 3d54     showCounter=T
+000004e0: 7275 652c 206d 6178 4c65 6e67 7468 3d32  rue, maxLength=2
+000004f0: 342c 2076 6973 6962 6c65 4f6e 3d22 247b  4, visibleOn="${
+00000500: 6478 785f 6964 3d3d 6e75 6c6c 3f66 616c  dxx_id==null?fal
+00000510: 7365 3a74 7275 657d 222c 0d0a 2020 2020  se:true}",..    
+00000520: 2020 2020 2020 2020 2020 2020 2020 6465                de
+00000530: 7363 7269 7074 696f 6e3d 27e5 a4a7 e5ad  scription='.....
+00000540: a6e4 b9a0 e8ae a4e8 af81 4944 efbc 8ce4  ..........ID....
+00000550: b88d e6b8 85e6 a59a e8af b7e5 8bbf e694  ................
+00000560: b9e5 8aa8 2729 2c0d 0a20 2020 2020 2020  ....'),..       
+00000570: 2049 6e70 7574 5465 7874 286c 6162 656c   InputText(label
+00000580: 3d27 e689 8be6 9cba e58f b77c e5ad a6e5  ='.........|....
+00000590: 8fb7 272c 206e 616d 653d 276d 6f62 696c  ..', name='mobil
+000005a0: 6527 2c20 7661 6c75 653d 2724 7b6d 6f62  e', value='${mob
+000005b0: 696c 657d 272c 2072 6571 7569 7265 643d  ile}', required=
+000005c0: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+000005d0: 2020 2020 2020 2020 2020 7472 696d 436f            trimCo
+000005e0: 6e74 656e 7473 3d54 7275 652c 2063 6c65  ntents=True, cle
+000005f0: 6172 6162 6c65 3d54 7275 652c 0d0a 2020  arable=True,..  
+00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000610: 7368 6f77 436f 756e 7465 723d 5472 7565  showCounter=True
+00000620: 2c20 6d61 784c 656e 6774 683d 3234 2c20  , maxLength=24, 
+00000630: 7669 7369 626c 654f 6e3d 2224 7b6d 6f62  visibleOn="${mob
+00000640: 696c 653d 3d6e 756c 6c3f 6661 6c73 653a  ile==null?false:
+00000650: 7472 7565 7d22 2c0d 0a20 2020 2020 2020  true}",..       
+00000660: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+00000670: 6970 7469 6f6e 3d27 e689 8be6 9cba e58f  iption='........
+00000680: b727 292c 0d0a 2020 2020 2020 2020 496e  .'),..        In
+00000690: 7075 7454 6578 7428 6c61 6265 6c3d 27e5  putText(label='.
+000006a0: 9ba2 e694 afe4 b9a6 4944 272c 206e 616d  ........ID', nam
+000006b0: 653d 276c 6561 6465 7227 2c20 7661 6c75  e='leader', valu
+000006c0: 653d 2724 7b6c 6561 6465 727d 272c 0d0a  e='${leader}',..
+000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006e0: 2020 7368 6f77 436f 756e 7465 723d 5472    showCounter=Tr
+000006f0: 7565 2c20 6d61 784c 656e 6774 683d 3130  ue, maxLength=10
+00000700: 2c20 6869 6464 656e 4f6e 3d54 7275 652c  , hiddenOn=True,
+00000710: 2074 7269 6d43 6f6e 7465 6e74 733d 5472   trimContents=Tr
+00000720: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
+00000730: 2020 2020 2020 2063 6c65 6172 6162 6c65         clearable
+00000740: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+00000750: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+00000760: 7074 696f 6e3d 27e5 9ba2 e694 afe4 b9a6  ption='.........
+00000770: 4944 efbc 8ce5 a1ab e586 99e5 908e e59b  ID..............
+00000780: a2e6 94af e4b9 a6e5 8faf e693 8de4 bd9c  ................
+00000790: e68f 90e4 baa4 e58a 9fe8 83bd efbc 8ce4  ................
+000007a0: b88d e6b8 85e6 a59a e8af b7e5 8bbf e694  ................
+000007b0: b9e5 8aa8 2729 2c0d 0a20 2020 2020 2020  ....'),..       
+000007c0: 2049 6e70 7574 5465 7874 286c 6162 656c   InputText(label
+000007d0: 3d27 6f70 656e 6964 272c 206e 616d 653d  ='openid', name=
+000007e0: 276f 7065 6e69 6427 2c20 7661 6c75 653d  'openid', value=
+000007f0: 2724 7b6f 7065 6e69 647d 272c 2072 6571  '${openid}', req
+00000800: 7569 7265 643d 5472 7565 2c0d 0a20 2020  uired=True,..   
+00000810: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00000820: 7269 6d43 6f6e 7465 6e74 733d 5472 7565  rimContents=True
+00000830: 2c20 636c 6561 7261 626c 653d 5472 7565  , clearable=True
+00000840: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000850: 2020 2020 2073 686f 7743 6f75 6e74 6572       showCounter
+00000860: 3d54 7275 652c 206d 6178 4c65 6e67 7468  =True, maxLength
+00000870: 3d36 342c 2076 6973 6962 6c65 4f6e 3d22  =64, visibleOn="
+00000880: 247b 6f70 656e 6964 3d3d 6e75 6c6c 3f66  ${openid==null?f
+00000890: 616c 7365 3a74 7275 657d 222c 0d0a 2020  alse:true}",..  
+000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008b0: 6465 7363 7269 7074 696f 6e3d 27e5 beae  description='...
+000008c0: e4bf a1e8 aea4 e8af 8149 44ef bc8c e4b8  .........ID.....
+000008d0: 8de6 b885 e6a5 9ae8 afb7 e58b bfe6 94b9  ................
+000008e0: e58a a827 292c 0d0a 2020 2020 2020 2020  ...'),..        
+000008f0: 496e 7075 7454 6578 7428 6c61 6265 6c3d  InputText(label=
+00000900: 27e7 99bb e5bd 95e5 af86 e7a0 8127 2c20  '............', 
+00000910: 6e61 6d65 3d27 5061 7373 776f 7264 272c  name='Password',
+00000920: 2076 616c 7565 3d27 272c 2074 7970 653d   value='', type=
+00000930: 2269 6e70 7574 2d70 6173 7377 6f72 6422  "input-password"
+00000940: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000950: 2020 2020 2074 7269 6d43 6f6e 7465 6e74       trimContent
+00000960: 733d 5472 7565 2c20 636c 6561 7261 626c  s=True, clearabl
+00000970: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
+00000980: 2020 2020 2020 2020 2020 2073 686f 7743             showC
+00000990: 6f75 6e74 6572 3d54 7275 652c 206d 6178  ounter=True, max
+000009a0: 4c65 6e67 7468 3d31 362c 2076 6973 6962  Length=16, visib
+000009b0: 6c65 4f6e 3d22 247b 7061 7373 776f 7264  leOn="${password
+000009c0: 3d3d 6e75 6c6c 3f66 616c 7365 3a74 7275  ==null?false:tru
+000009d0: 657d 222c 0d0a 2020 2020 2020 2020 2020  e}",..          
+000009e0: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+000009f0: 696f 6e3d 27e7 99bb e5bd 9557 6562 2055  ion='......Web U
+00000a00: 49e7 9a84 e5af 86e7 a081 2729 2c0d 0a20  I.........'),.. 
+00000a10: 2020 2020 2020 2049 6e70 7574 5465 7874         InputText
+00000a20: 286c 6162 656c 3d27 e5ad a6e6 a0a1 e7b1  (label='........
+00000a30: bbe5 9e8b 272c 206e 616d 653d 2775 6e69  ....', name='uni
+00000a40: 7665 7273 6974 795f 7479 7065 272c 2076  versity_type', v
+00000a50: 616c 7565 3d27 247b 756e 6976 6572 7369  alue='${universi
+00000a60: 7479 5f74 7970 657d 272c 0d0a 2020 2020  ty_type}',..    
+00000a70: 2020 2020 2020 2020 2020 2020 2020 7368                sh
+00000a80: 6f77 436f 756e 7465 723d 5472 7565 2c20  owCounter=True, 
+00000a90: 6d61 784c 656e 6774 683d 3136 2c20 7265  maxLength=16, re
+00000aa0: 7175 6972 6564 3d54 7275 652c 2074 7269  quired=True, tri
+00000ab0: 6d43 6f6e 7465 6e74 733d 5472 7565 2c0d  mContents=True,.
+00000ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ad0: 2020 2063 6c65 6172 6162 6c65 3d54 7275     clearable=Tru
+00000ae0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00000af0: 2020 2020 2020 7669 7369 626c 654f 6e3d        visibleOn=
+00000b00: 2224 7b75 6e69 7665 7273 6974 795f 7479  "${university_ty
+00000b10: 7065 3d3d 6e75 6c6c 3f66 616c 7365 3a74  pe==null?false:t
+00000b20: 7275 657d 222c 0d0a 2020 2020 2020 2020  rue}",..        
+00000b30: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+00000b40: 7074 696f 6e3d 27e5 ada6 e6a0 a1e7 b1bb  ption='.........
+00000b50: e59e 8bef bc8c e4b8 8de6 b885 e6a5 9ae6  ................
+00000b60: b885 e697 a0e6 94b9 e58a a827 292c 0d0a  ...........'),..
+00000b70: 2020 2020 2020 2020 496e 7075 7454 6578          InputTex
+00000b80: 7428 6c61 6265 6c3d 27e5 ada6 e6a0 a149  t(label='......I
+00000b90: 4427 2c20 6e61 6d65 3d27 756e 6976 6572  D', name='univer
+00000ba0: 7369 7479 5f69 6427 2c20 7661 6c75 653d  sity_id', value=
+00000bb0: 2724 7b75 6e69 7665 7273 6974 795f 6964  '${university_id
+00000bc0: 7d27 2c0d 0a20 2020 2020 2020 2020 2020  }',..           
+00000bd0: 2020 2020 2020 2072 6571 7569 7265 643d         required=
+00000be0: 5472 7565 2c20 7472 696d 436f 6e74 656e  True, trimConten
+00000bf0: 7473 3d54 7275 652c 2063 6c65 6172 6162  ts=True, clearab
+00000c00: 6c65 3d54 7275 652c 0d0a 2020 2020 2020  le=True,..      
+00000c10: 2020 2020 2020 2020 2020 2020 7368 6f77              show
+00000c20: 436f 756e 7465 723d 5472 7565 2c20 6d61  Counter=True, ma
+00000c30: 784c 656e 6774 683d 3234 2c0d 0a20 2020  xLength=24,..   
+00000c40: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00000c50: 6973 6962 6c65 4f6e 3d22 247b 756e 6976  isibleOn="${univ
+00000c60: 6572 7369 7479 5f69 643d 3d6e 756c 6c3f  ersity_id==null?
+00000c70: 6661 6c73 653a 7472 7565 7d22 2c0d 0a20  false:true}",.. 
+00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c90: 2064 6573 6372 6970 7469 6f6e 3d27 e5ad   description='..
+00000ca0: a6e6 a0a1 4944 efbc 8ce4 b88d e6b8 85e6  ....ID..........
+00000cb0: a59a e8af b7e5 8bbf e694 b9e5 8aa8 2729  ..............')
+00000cc0: 2c0d 0a20 2020 2020 2020 2049 6e70 7574  ,..        Input
+00000cd0: 5465 7874 286c 6162 656c 3d27 e5ad a6e6  Text(label='....
+00000ce0: a0a1 e590 8de7 a7b0 272c 206e 616d 653d  ........', name=
+00000cf0: 2775 6e69 7665 7273 6974 7927 2c20 7661  'university', va
+00000d00: 6c75 653d 2724 7b75 6e69 7665 7273 6974  lue='${universit
+00000d10: 797d 272c 2072 6571 7569 7265 643d 5472  y}', required=Tr
+00000d20: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
+00000d30: 2020 2020 2020 2074 7269 6d43 6f6e 7465         trimConte
+00000d40: 6e74 733d 5472 7565 2c20 636c 6561 7261  nts=True, cleara
+00000d50: 626c 653d 5472 7565 2c0d 0a20 2020 2020  ble=True,..     
+00000d60: 2020 2020 2020 2020 2020 2020 2073 686f               sho
+00000d70: 7743 6f75 6e74 6572 3d54 7275 652c 206d  wCounter=True, m
+00000d80: 6178 4c65 6e67 7468 3d32 302c 2076 6973  axLength=20, vis
+00000d90: 6962 6c65 4f6e 3d22 247b 756e 6976 6572  ibleOn="${univer
+00000da0: 7369 7479 3d3d 6e75 6c6c 3f66 616c 7365  sity==null?false
+00000db0: 3a74 7275 657d 222c 0d0a 2020 2020 2020  :true}",..      
+00000dc0: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+00000dd0: 7269 7074 696f 6e3d 27e5 ada6 e6a0 a1e5  ription='.......
+00000de0: 908d e7a7 b027 292c 0d0a 2020 2020 2020  .....'),..      
+00000df0: 2020 496e 7075 7454 6578 7428 6c61 6265    InputText(labe
+00000e00: 6c3d 27e5 ada6 e999 a249 4427 2c20 6e61  l='......ID', na
+00000e10: 6d65 3d27 636f 6c6c 6567 655f 6964 272c  me='college_id',
+00000e20: 2076 616c 7565 3d27 247b 636f 6c6c 6567   value='${colleg
+00000e30: 655f 6964 7d27 2c20 7265 7175 6972 6564  e_id}', required
+00000e40: 3d46 616c 7365 2c0d 0a20 2020 2020 2020  =False,..       
+00000e50: 2020 2020 2020 2020 2020 2074 7269 6d43             trimC
+00000e60: 6f6e 7465 6e74 733d 5472 7565 2c20 636c  ontents=True, cl
+00000e70: 6561 7261 626c 653d 5472 7565 2c0d 0a20  earable=True,.. 
+00000e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e90: 2073 686f 7743 6f75 6e74 6572 3d54 7275   showCounter=Tru
+00000ea0: 652c 206d 6178 4c65 6e67 7468 3d32 342c  e, maxLength=24,
+00000eb0: 2076 6973 6962 6c65 4f6e 3d22 247b 636f   visibleOn="${co
+00000ec0: 6c6c 6567 655f 6964 3d3d 6e75 6c6c 3f66  llege_id==null?f
+00000ed0: 616c 7365 3a74 7275 657d 222c 0d0a 2020  alse:true}",..  
+00000ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ef0: 6465 7363 7269 7074 696f 6e3d 27e5 ada6  description='...
+00000f00: e999 a249 4427 292c 0d0a 2020 2020 2020  ...ID'),..      
+00000f10: 2020 496e 7075 7454 6578 7428 6c61 6265    InputText(labe
+00000f20: 6c3d 27e5 ada6 e999 a2e5 908d e7a7 b027  l='............'
+00000f30: 2c20 6e61 6d65 3d27 636f 6c6c 6567 6527  , name='college'
+00000f40: 2c20 7661 6c75 653d 2724 7b63 6f6c 6c65  , value='${colle
+00000f50: 6765 7d27 2c0d 0a20 2020 2020 2020 2020  ge}',..         
+00000f60: 2020 2020 2020 2020 2074 7269 6d43 6f6e           trimCon
+00000f70: 7465 6e74 733d 5472 7565 2c20 636c 6561  tents=True, clea
+00000f80: 7261 626c 653d 5472 7565 2c0d 0a20 2020  rable=True,..   
+00000f90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00000fa0: 686f 7743 6f75 6e74 6572 3d54 7275 652c  howCounter=True,
+00000fb0: 206d 6178 4c65 6e67 7468 3d32 342c 2076   maxLength=24, v
+00000fc0: 6973 6962 6c65 4f6e 3d22 247b 636f 6c6c  isibleOn="${coll
+00000fd0: 6567 653d 3d6e 756c 6c3f 6661 6c73 653a  ege==null?false:
+00000fe0: 7472 7565 7d22 2c0d 0a20 2020 2020 2020  true}",..       
+00000ff0: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+00001000: 6970 7469 6f6e 3d27 e5ad a6e9 99a2 e590  iption='........
+00001010: 8de7 a7b0 2729 2c0d 0a20 2020 2020 2020  ....'),..       
+00001020: 2049 6e70 7574 5465 7874 286c 6162 656c   InputText(label
+00001030: 3d27 e59b a2e6 94af e983 a849 4427 2c20  ='.........ID', 
+00001040: 6e61 6d65 3d27 6f72 6761 6e69 7a61 7469  name='organizati
+00001050: 6f6e 5f69 6427 2c20 7661 6c75 653d 2724  on_id', value='$
+00001060: 7b6f 7267 616e 697a 6174 696f 6e5f 6964  {organization_id
+00001070: 7d27 2c0d 0a20 2020 2020 2020 2020 2020  }',..           
+00001080: 2020 2020 2020 2072 6571 7569 7265 643d         required=
+00001090: 5472 7565 2c20 7472 696d 436f 6e74 656e  True, trimConten
+000010a0: 7473 3d54 7275 652c 2063 6c65 6172 6162  ts=True, clearab
+000010b0: 6c65 3d54 7275 652c 0d0a 2020 2020 2020  le=True,..      
+000010c0: 2020 2020 2020 2020 2020 2020 7368 6f77              show
+000010d0: 436f 756e 7465 723d 5472 7565 2c20 6d61  Counter=True, ma
+000010e0: 784c 656e 6774 683d 3234 2c0d 0a20 2020  xLength=24,..   
+000010f0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00001100: 6973 6962 6c65 4f6e 3d22 247b 6f72 6761  isibleOn="${orga
+00001110: 6e69 7a61 7469 6f6e 5f69 643d 3d6e 756c  nization_id==nul
+00001120: 6c3f 6661 6c73 653a 7472 7565 7d22 2c0d  l?false:true}",.
+00001130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001140: 2020 2064 6573 6372 6970 7469 6f6e 3d27     description='
+00001150: e59b a2e6 94af e983 a849 4427 292c 0d0a  .........ID'),..
+00001160: 2020 2020 2020 2020 496e 7075 7454 6578          InputTex
+00001170: 7428 6c61 6265 6c3d 27e5 9ba2 e694 afe9  t(label='.......
+00001180: 83a8 e590 8de7 a7b0 272c 206e 616d 653d  ........', name=
+00001190: 276f 7267 616e 697a 6174 696f 6e27 2c20  'organization', 
+000011a0: 7661 6c75 653d 2724 7b6f 7267 616e 697a  value='${organiz
+000011b0: 6174 696f 6e7d 272c 0d0a 2020 2020 2020  ation}',..      
+000011c0: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+000011d0: 6972 6564 3d46 616c 7365 2c20 7472 696d  ired=False, trim
+000011e0: 436f 6e74 656e 7473 3d54 7275 652c 2063  Contents=True, c
+000011f0: 6c65 6172 6162 6c65 3d54 7275 652c 0d0a  learable=True,..
+00001200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001210: 2020 7368 6f77 436f 756e 7465 723d 5472    showCounter=Tr
+00001220: 7565 2c20 6d61 784c 656e 6774 683d 3336  ue, maxLength=36
+00001230: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001240: 2020 2020 2076 6973 6962 6c65 4f6e 3d22       visibleOn="
+00001250: 247b 6f72 6761 6e69 7a61 7469 6f6e 3d3d  ${organization==
+00001260: 6e75 6c6c 3f66 616c 7365 3a74 7275 657d  null?false:true}
+00001270: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00001280: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00001290: 6e3d 27e5 9ba2 e694 afe9 83a8 e590 8de7  n='.............
+000012a0: a7b0 2729 2c0d 0a20 2020 2020 2020 2049  ..'),..        I
+000012b0: 6e70 7574 5465 7874 286c 6162 656c 3d27  nputText(label='
+000012c0: 746f 6b65 6e27 2c20 6e61 6d65 3d27 746f  token', name='to
+000012d0: 6b65 6e27 2c20 7661 6c75 653d 2724 7b74  ken', value='${t
+000012e0: 6f6b 656e 7d27 2c20 7265 7175 6972 6564  oken}', required
+000012f0: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+00001300: 2020 2020 2020 2020 2020 7472 696d 436f            trimCo
+00001310: 6e74 656e 7473 3d54 7275 652c 2063 6c65  ntents=True, cle
+00001320: 6172 6162 6c65 3d54 7275 652c 0d0a 2020  arable=True,..  
+00001330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001340: 7368 6f77 436f 756e 7465 723d 5472 7565  showCounter=True
+00001350: 2c20 7669 7369 626c 654f 6e3d 2224 7b74  , visibleOn="${t
+00001360: 6f6b 656e 3d3d 6e75 6c6c 3f66 616c 7365  oken==null?false
+00001370: 3a74 7275 657d 222c 0d0a 2020 2020 2020  :true}",..      
+00001380: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+00001390: 7269 7074 696f 6e3d 27e6 8f90 e4ba a4e5  ription='.......
+000013a0: a4a7 e5ad a6e4 b9a0 e99c 80e8 a681 e79a  ................
+000013b0: 8474 6f6b 656e 2729 2c0d 0a20 2020 2020  .token'),..     
+000013c0: 2020 2049 6e70 7574 5465 7874 286c 6162     InputText(lab
+000013d0: 656c 3d27 636f 6f6b 6965 272c 206e 616d  el='cookie', nam
+000013e0: 653d 2763 6f6f 6b69 6527 2c20 7661 6c75  e='cookie', valu
+000013f0: 653d 2724 7b63 6f6f 6b69 657d 272c 2072  e='${cookie}', r
+00001400: 6571 7569 7265 643d 5472 7565 2c0d 0a20  equired=True,.. 
+00001410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001420: 2074 7269 6d43 6f6e 7465 6e74 733d 5472   trimContents=Tr
+00001430: 7565 2c20 636c 6561 7261 626c 653d 5472  ue, clearable=Tr
+00001440: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
+00001450: 2020 2020 2020 2073 686f 7743 6f75 6e74         showCount
+00001460: 6572 3d54 7275 652c 2076 6973 6962 6c65  er=True, visible
+00001470: 4f6e 3d22 247b 636f 6f6b 6965 3d3d 6e75  On="${cookie==nu
+00001480: 6c6c 3f66 616c 7365 3a74 7275 657d 222c  ll?false:true}",
+00001490: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000014a0: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
+000014b0: 27e6 8f90 e4ba a4e5 a4a7 e5ad a6e4 b9a0  '...............
+000014c0: e99c 80e8 a681 e79a 8463 6f6f 6b69 6527  .........cookie'
+000014d0: 290d 0a20 2020 205d 290d 0a64 6574 6169  )..    ])..detai
+000014e0: 6c5f 6275 7474 6f6e 203d 2041 6374 696f  l_button = Actio
+000014f0: 6e54 7970 652e 4469 616c 6f67 286c 6162  nType.Dialog(lab
+00001500: 656c 3d27 e4bf a1e6 81af 272c 0d0a 2020  el='......',..  
+00001510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001530: 746f 6f6c 7469 703d 27e6 9fa5 e79c 8b7c  tooltip='......|
+00001540: e4bf aee6 94b9 e4bf a1e6 81af 272c 0d0a  ............',..
+00001550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001570: 2020 7369 7a65 3d27 6c67 272c 0d0a 2020    size='lg',..  
+00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015a0: 6963 6f6e 3d27 6661 2066 612d 7573 6572  icon='fa fa-user
+000015b0: 2d74 6167 2074 6578 742d 7072 696d 6172  -tag text-primar
+000015c0: 7927 2c0d 0a20 2020 2020 2020 2020 2020  y',..           
+000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015e0: 2020 2020 2020 2064 6961 6c6f 673d 4469         dialog=Di
+000015f0: 616c 6f67 2874 6974 6c65 3d27 247b 6e61  alog(title='${na
+00001600: 6d65 7de7 9a84 e8af a6e7 bb86 e4bf a1e6  me}.............
+00001610: 81af 272c 2073 697a 653d 276c 6727 2c20  ..', size='lg', 
+00001620: 626f 6479 3d5b 6465 7461 696c 5f66 6f72  body=[detail_for
+00001630: 6d5d 2929 0d0a 6361 7264 203d 2043 6172  m]))..card = Car
+00001640: 6428 0d0a 2020 2020 6865 6164 6572 3d43  d(..    header=C
+00001650: 6172 642e 4865 6164 6572 2874 6974 6c65  ard.Header(title
+00001660: 3d27 246e 616d 6527 2c0d 0a20 2020 2020  ='$name',..     
+00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001680: 2020 7375 6254 6974 6c65 3d27 2475 7365    subTitle='$use
+00001690: 725f 6964 272c 0d0a 2020 2020 2020 2020  r_id',..        
+000016a0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000016b0: 6573 6372 6970 7469 6f6e 3d27 2463 6174  escription='$cat
+000016c0: 616c 6f67 7565 272c 0d0a 2020 2020 2020  alogue',..      
 000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016e0: 2020 2020 2020 2020 2020 2020 6c65 7665              leve
-000016f0: 6c3d 4c65 7665 6c45 6e75 6d2e 7761 726e  l=LevelEnum.warn
-00001700: 696e 672c 0d0a 2020 2020 2020 2020 2020  ing,..          
-00001710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001730: 2020 2020 2020 2020 2063 6f6e 6669 726d           confirm
-00001740: 5465 7874 3d27 e7a1 aee5 ae9a e8a6 81e5  Text='..........
-00001750: 88a0 e999 a4e9 9d92 e5b9 b4e5 a4a7 e5ad  ................
-00001760: a6e4 b9a0 e69c 9fe6 95b0 e590 97ef bc9f  ................
-00001770: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00001780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017a0: 2020 2020 2020 2061 7069 3d27 6465 6c65         api='dele
-000017b0: 7465 3a2f 5465 656e 5374 7564 792f 6170  te:/TeenStudy/ap
-000017c0: 692f 6465 6c65 7465 5f61 6c6c 3f74 7970  i/delete_all?typ
-000017d0: 653d 616e 7377 6572 7327 292c 0d0a 2020  e=answers'),..  
-000017e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001800: 2022 6275 6c6b 4163 7469 6f6e 7322 2c20   "bulkActions", 
-00001810: 2272 656c 6f61 6422 5d2c 0d0a 2020 2020  "reload"],..    
-00001820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001830: 6974 656d 4163 7469 6f6e 733d 5b0d 0a20  itemActions=[.. 
-00001840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001850: 2020 2020 2020 2041 6374 696f 6e54 7970         ActionTyp
-00001860: 652e 416a 6178 2874 6f6f 6c74 6970 3d27  e.Ajax(tooltip='
-00001870: e588 a0e9 99a4 272c 0d0a 2020 2020 2020  ......',..      
-00001880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018a0: 2020 6963 6f6e 3d27 6661 2066 612d 7469    icon='fa fa-ti
-000018b0: 6d65 7320 7465 7874 2d64 616e 6765 7227  mes text-danger'
-000018c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000018d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018e0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-000018f0: 726d 5465 7874 3d27 e588 a0e9 99a4 e8af  rmText='........
-00001900: a5e6 9c9f e99d 92e5 b9b4 e5a4 a7e5 ada6  ................
-00001910: e4b9 a027 2c0d 0a20 2020 2020 2020 2020  ...',..         
-00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001930: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00001940: 7069 3d27 6465 6c65 7465 3a2f 5465 656e  pi='delete:/Teen
-00001950: 5374 7564 792f 6170 692f 6465 6c65 7465  Study/api/delete
-00001960: 5f61 6e73 7765 723f 6964 3d24 7b69 647d  _answer?id=${id}
-00001970: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-00001980: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
-00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019a0: 666f 6f74 6162 6c65 3d54 7275 652c 0d0a  footable=True,..
-000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019c0: 2020 2020 636f 6c75 6d6e 733d 5b0d 0a20      columns=[.. 
-000019d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019e0: 2020 2020 2020 2054 6162 6c65 436f 6c75         TableColu
-000019f0: 6d6e 286c 6162 656c 3d27 e695 b0e6 8dae  mn(label='......
-00001a00: e5ba 9349 4427 2c20 6e61 6d65 3d27 6964  ...ID', name='id
-00001a10: 2729 2c0d 0a20 2020 2020 2020 2020 2020  '),..           
-00001a20: 2020 2020 2020 2020 2020 2020 2054 6162               Tab
-00001a30: 6c65 436f 6c75 6d6e 286c 6162 656c 3d27  leColumn(label='
-00001a40: e5a4 a7e5 ada6 e4b9 a049 4427 2c20 6e61  .........ID', na
-00001a50: 6d65 3d27 636f 6465 2729 2c0d 0a20 2020  me='code'),..   
-00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a70: 2020 2020 2054 6162 6c65 436f 6c75 6d6e       TableColumn
-00001a80: 286c 6162 656c 3d27 e5a4 a7e5 ada6 e4b9  (label='........
-00001a90: a0e6 9c9f e695 b027 2c20 6e61 6d65 3d27  .......', name='
-00001aa0: 6361 7461 6c6f 6775 6527 2c20 7365 6172  catalogue', sear
-00001ab0: 6368 6162 6c65 3d54 7275 6529 2c0d 0a20  chable=True),.. 
-00001ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ad0: 2020 2020 2020 2054 6162 6c65 436f 6c75         TableColu
-00001ae0: 6d6e 2874 7970 653d 2774 706c 272c 2074  mn(type='tpl', t
-00001af0: 706c 3d27 247b 7572 6c7c 7472 756e 6361  pl='${url|trunca
-00001b00: 7465 3a32 307d 272c 206c 6162 656c 3d27  te:20}', label='
-00001b10: e5ae 98e6 96b9 e7bd 91e5 9d80 272c 0d0a  ............',..
-00001b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016e0: 2061 7661 7461 7254 6578 743d 2724 7b61   avatarText='${a
+000016f0: 7265 617d 272c 0d0a 2020 2020 2020 2020  rea}',..        
+00001700: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00001710: 7661 7461 7254 6578 7443 6c61 7373 4e61  vatarTextClassNa
+00001720: 6d65 3d27 6f76 6572 666c 6f77 2d68 6964  me='overflow-hid
+00001730: 6465 6e27 292c 0d0a 2020 2020 6163 7469  den'),..    acti
+00001740: 6f6e 733d 5b64 6574 6169 6c5f 6275 7474  ons=[detail_butt
+00001750: 6f6e 2c20 4163 7469 6f6e 5479 7065 2e41  on, ActionType.A
+00001760: 6a61 7828 0d0a 2020 2020 2020 2020 6c61  jax(..        la
+00001770: 6265 6c3d 22e6 8f90 e4ba a422 2c0d 0a20  bel="......",.. 
+00001780: 2020 2020 2020 2074 6f6f 6c74 6970 3d27         tooltip='
+00001790: e68f 90e4 baa4 e5a4 a7e5 ada6 e4b9 a027  ...............'
+000017a0: 2c0d 0a20 2020 2020 2020 2069 636f 6e3d  ,..        icon=
+000017b0: 2766 6120 6661 2d63 6865 636b 2074 6578  'fa fa-check tex
+000017c0: 742d 7375 6363 6573 7327 2c0d 0a20 2020  t-success',..   
+000017d0: 2020 2020 2063 6f6e 6669 726d 5465 7874       confirmText
+000017e0: 3d27 e698 afe5 90a6 e68f 90e4 baa4 e69c  ='..............
+000017f0: 80e6 96b0 e4b8 80e6 9c9f e99d 92e5 b9b4  ................
+00001800: e5a4 a7e5 ada6 e4b9 a0ef bc9f 272c 0d0a  ............',..
+00001810: 2020 2020 2020 2020 6170 693d 2767 6574          api='get
+00001820: 3a2f 5465 656e 5374 7564 792f 6170 692f  :/TeenStudy/api/
+00001830: 636f 6d6d 6974 3f75 7365 725f 6964 3d24  commit?user_id=$
+00001840: 7b75 7365 725f 6964 7d26 6172 6561 3d24  {user_id}&area=$
+00001850: 7b61 7265 617d 270d 0a20 2020 2029 2c20  {area}'..    ), 
+00001860: 4163 7469 6f6e 5479 7065 2e41 6a61 7828  ActionType.Ajax(
+00001870: 0d0a 2020 2020 2020 2020 746f 6f6c 7469  ..        toolti
+00001880: 703d 27e5 88a0 e999 a427 2c0d 0a20 2020  p='......',..   
+00001890: 2020 2020 206c 6162 656c 3d22 e588 a0e9       label="....
+000018a0: 99a4 222c 0d0a 2020 2020 2020 2020 6963  ..",..        ic
+000018b0: 6f6e 3d27 6661 2066 612d 7472 6173 682d  on='fa fa-trash-
+000018c0: 6361 6e20 7465 7874 2d64 616e 6765 7227  can text-danger'
+000018d0: 2c0d 0a20 2020 2020 2020 2063 6f6e 6669  ,..        confi
+000018e0: 726d 5465 7874 3d27 e588 a0e9 99a4 e8af  rmText='........
+000018f0: a5e7 94a8 e688 b727 2c0d 0a20 2020 2020  .......',..     
+00001900: 2020 2061 7069 3d27 6465 6c65 7465 3a2f     api='delete:/
+00001910: 5465 656e 5374 7564 792f 6170 692f 6465  TeenStudy/api/de
+00001920: 6c65 7465 5f6d 656d 6265 723f 7573 6572  lete_member?user
+00001930: 5f69 643d 247b 7573 6572 5f69 647d 270d  _id=${user_id}'.
+00001940: 0a20 2020 2029 2c20 5d2c 0d0a 2020 2020  .    ), ],..    
+00001950: 746f 6f6c 6261 723d 5b0d 0a20 2020 2020  toolbar=[..     
+00001960: 2020 2054 706c 2874 706c 3d27 2461 7265     Tpl(tpl='$are
+00001970: 6127 2c20 636c 6173 734e 616d 653d 276c  a', className='l
+00001980: 6162 656c 206c 6162 656c 2d77 6172 6e69  abel label-warni
+00001990: 6e67 272c 2068 6964 6465 6e4f 6e3d 5472  ng', hiddenOn=Tr
+000019a0: 7565 292c 0d0a 2020 2020 2020 2020 5377  ue),..        Sw
+000019b0: 6974 6368 286e 616d 653d 2761 7574 6f5f  itch(name='auto_
+000019c0: 7375 626d 6974 272c 0d0a 2020 2020 2020  submit',..      
+000019d0: 2020 2020 2020 2020 2076 616c 7565 3d27           value='
+000019e0: 247b 6175 746f 5f73 7562 6d69 747d 272c  ${auto_submit}',
+000019f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001a00: 2074 6f6f 6c74 6970 3d27 e887 aae5 8aa8   tooltip='......
+00001a10: e68f 90e4 baa4 e5a4 a7e5 ada6 e4b9 a0e5  ................
+00001a20: bc80 e585 b327 2c0d 0a20 2020 2020 2020  .....',..       
+00001a30: 2020 2020 2020 2020 6f6e 5465 7874 3d27          onText='
+00001a40: e5bc 80e5 90af 272c 0d0a 2020 2020 2020  ......',..      
+00001a50: 2020 2020 2020 2020 206f 6666 5465 7874           offText
+00001a60: 3d27 e585 b3e9 97ad 272c 0d0a 2020 2020  ='......',..    
+00001a70: 2020 2020 2020 2020 2020 206f 6e45 7665             onEve
+00001a80: 6e74 3d7b 0d0a 2020 2020 2020 2020 2020  nt={..          
+00001a90: 2020 2020 2020 2020 2027 6368 616e 6765           'change
+00001aa0: 273a 207b 0d0a 2020 2020 2020 2020 2020  ': {..          
+00001ab0: 2020 2020 2020 2020 2020 2020 2027 6163               'ac
+00001ac0: 7469 6f6e 7327 3a20 7b0d 0a20 2020 2020  tions': {..     
+00001ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ae0: 2020 2020 2020 2761 6374 696f 6e54 7970        'actionTyp
+00001af0: 6527 3a20 2761 6a61 7827 2c0d 0a20 2020  e': 'ajax',..   
+00001b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b10: 2020 2020 2020 2020 2761 7267 7327 3a20          'args': 
+00001b20: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
 00001b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b40: 2020 2020 6e61 6d65 3d27 7572 6c27 2c0d      name='url',.
-00001b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b70: 2020 2020 2070 6f70 4f76 6572 3d7b 276d       popOver={'m
-00001b80: 6f64 6527 3a20 2764 6961 6c6f 6727 2c20  ode': 'dialog', 
-00001b90: 2774 6974 6c65 273a 2027 e5ae 8ce6 95b4  'title': '......
-00001ba0: e7bd 91e5 9d80 272c 0d0a 2020 2020 2020  ......',..      
-00001bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bd0: 2020 2020 2020 2027 636c 6173 734e 616d         'classNam
-00001be0: 6527 3a20 2762 7265 616b 2d61 6c6c 272c  e': 'break-all',
-00001bf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c10: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001c20: 626f 6479 273a 207b 2774 7970 6527 3a20  body': {'type': 
-00001c30: 2774 706c 272c 0d0a 2020 2020 2020 2020  'tpl',..        
-00001c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c60: 2020 2020 2020 2020 2020 2020 2020 2774                't
-00001c70: 706c 273a 2027 247b 7572 6c7d 277d 7d2c  pl': '${url}'}},
-00001c80: 2063 6f70 7961 626c 653d 5472 7565 292c   copyable=True),
-00001c90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001ca0: 2020 2020 2020 2020 2020 5461 626c 6543            TableC
-00001cb0: 6f6c 756d 6e28 7479 7065 3d27 7470 6c27  olumn(type='tpl'
-00001cc0: 2c20 7470 6c3d 2724 7b65 6e64 5f75 726c  , tpl='${end_url
-00001cd0: 7c74 7275 6e63 6174 653a 3230 7d27 2c20  |truncate:20}', 
-00001ce0: 6c61 6265 6c3d 27e5 ae8c e688 90e6 88aa  label='.........
-00001cf0: e59b bee7 bd91 e59d 8027 2c0d 0a20 2020  .........',..   
+00001b40: 2020 2761 7069 273a 207b 0d0a 2020 2020    'api': {..    
+00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b60: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00001b70: 7572 6c27 3a20 272f 5465 656e 5374 7564  url': '/TeenStud
+00001b80: 792f 6170 692f 7365 745f 6175 746f 5f73  y/api/set_auto_s
+00001b90: 7562 6d69 7427 2c0d 0a20 2020 2020 2020  ubmit',..       
+00001ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bb0: 2020 2020 2020 2020 2020 2020 276d 6574              'met
+00001bc0: 686f 6427 3a20 2770 7574 270d 0a20 2020  hod': 'put'..   
+00001bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001be0: 2020 2020 2020 2020 2020 2020 7d2c 0d0a              },..
+00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00001c10: 6d65 7373 6167 6573 273a 207b 0d0a 2020  messages': {..  
+00001c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c40: 2027 7375 6363 6573 7327 3a20 27e8 87aa   'success': '...
+00001c50: e58a a8e6 8f90 e4ba a4e5 b7b2 e8ae bee7  ................
+00001c60: bdae e4b8 ba24 7b65 7665 6e74 2e64 6174  .....${event.dat
+00001c70: 612e 7661 6c75 653d 3d74 7275 653f 22e5  a.value==true?".
+00001c80: bc80 e590 af22 3a22 e585 b3e9 97ad 227d  .....":"......"}
+00001c90: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00001ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cb0: 2020 2020 2020 2027 6661 696c 6564 273a         'failed':
+00001cc0: 2027 e4bf aee6 94b9 e5a4 b1e8 b4a5 efbc   '..............
+00001cd0: 8127 0d0a 2020 2020 2020 2020 2020 2020  .'..            
+00001ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cf0: 2020 207d 2c0d 0a20 2020 2020 2020 2020     },..         
 00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d20: 206e 616d 653d 2765 6e64 5f75 726c 272c   name='end_url',
-00001d30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001d10: 2020 2020 2020 2773 7461 7475 7327 3a20        'status': 
+00001d20: 2724 7b65 7665 6e74 2e64 6174 612e 7661  '${event.data.va
+00001d30: 6c75 657d 272c 0d0a 2020 2020 2020 2020  lue}',..        
 00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d50: 2020 2020 2020 706f 704f 7665 723d 7b27        popOver={'
-00001d60: 6d6f 6465 273a 2027 6469 616c 6f67 272c  mode': 'dialog',
-00001d70: 2027 7469 746c 6527 3a20 27e5 ae8c e695   'title': '.....
-00001d80: b4e7 bd91 e59d 8027 2c0d 0a20 2020 2020  .......',..     
-00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d50: 2020 2020 2020 2027 6964 273a 2027 247b         'id': '${
+00001d60: 6964 7d27 0d0a 2020 2020 2020 2020 2020  id}'..          
+00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d80: 207d 0d0a 2020 2020 2020 2020 2020 2020   }..            
+00001d90: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
 00001da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001db0: 2020 2020 2020 2020 2763 6c61 7373 4e61          'classNa
-00001dc0: 6d65 273a 2027 6272 6561 6b2d 616c 6c27  me': 'break-all'
-00001dd0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e00: 2762 6f64 7927 3a20 7b27 7479 7065 273a  'body': {'type':
-00001e10: 2027 7470 6c27 2c0d 0a20 2020 2020 2020   'tpl',..       
-00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e40: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001e50: 7470 6c27 3a20 2724 7b65 6e64 5f75 726c  tpl': '${end_url
-00001e60: 7d27 7d7d 2c20 636f 7079 6162 6c65 3d54  }'}}, copyable=T
-00001e70: 7275 6529 2c0d 0a20 2020 2020 2020 2020  rue),..         
-00001e80: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-00001e90: 6162 6c65 436f 6c75 6d6e 2874 7970 653d  ableColumn(type=
-00001ea0: 2774 706c 272c 2074 706c 3d27 247b 616e  'tpl', tpl='${an
-00001eb0: 7377 6572 7c74 7275 6e63 6174 653a 3230  swer|truncate:20
-00001ec0: 7d27 2c20 6c61 6265 6c3d 27e7 ad94 e6a1  }', label='.....
-00001ed0: 8827 2c0d 0a20 2020 2020 2020 2020 2020  .',..           
-00001ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ef0: 2020 2020 2020 2020 206e 616d 653d 2761           name='a
-00001f00: 6e73 7765 7227 2c0d 0a20 2020 2020 2020  nswer',..       
-00001f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f20: 2020 2020 2020 2020 2020 2020 2070 6f70               pop
-00001f30: 4f76 6572 3d7b 276d 6f64 6527 3a20 2764  Over={'mode': 'd
-00001f40: 6961 6c6f 6727 2c20 2774 6974 6c65 273a  ialog', 'title':
-00001f50: 2027 e5ae 8ce6 95b4 e7ad 94e6 a188 272c   '............',
-00001f60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f80: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001f90: 636c 6173 734e 616d 6527 3a20 2762 7265  className': 'bre
-00001fa0: 616b 2d61 6c6c 272c 0d0a 2020 2020 2020  ak-all',..      
-00001fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fd0: 2020 2020 2020 2027 626f 6479 273a 207b         'body': {
-00001fe0: 2774 7970 6527 3a20 2774 706c 272c 0d0a  'type': 'tpl',..
-00001ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002020: 2020 2020 2020 2774 706c 273a 2027 247b        'tpl': '${
-00002030: 616e 7377 6572 7d27 7d7d 292c 0d0a 2020  answer}'}}),..  
-00002040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002050: 2020 2020 2020 5461 626c 6543 6f6c 756d        TableColum
-00002060: 6e28 7479 7065 3d27 7470 6c27 2c20 7470  n(type='tpl', tp
-00002070: 6c3d 2724 7b74 696d 657c 6461 7465 3a59  l='${time|date:Y
-00002080: 5959 592d 4d4d 2d44 4420 4848 5c5c 3a6d  YYY-MM-DD HH\\:m
-00002090: 6d5c 5c3a 7373 7d27 2c0d 0a20 2020 2020  m\\:ss}',..     
-000020a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020b0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000020c0: 6162 656c 3d27 e69b b4e6 96b0 e697 b6e9  abel='..........
-000020d0: 97b4 272c 0d0a 2020 2020 2020 2020 2020  ..',..          
+00001db0: 207d 0d0a 2020 2020 2020 2020 2020 2020   }..            
+00001dc0: 2020 207d 290d 0a20 2020 205d 290d 0a22     })..    ]).."
+00001dd0: 2222 e688 90e5 9198 e58d a1e7 8987 e99d  ""..............
+00001de0: a2e6 9dbf 2222 220d 0a63 6172 6473 5f63  ...."""..cards_c
+00001df0: 7572 6420 3d20 4361 7264 7343 5255 4428  urd = CardsCRUD(
+00001e00: 6d6f 6465 3d27 6361 7264 7327 2c0d 0a20  mode='cards',.. 
+00001e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e20: 2020 2020 2020 7469 746c 653d 2727 2c0d        title='',.
+00001e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001e40: 2020 2020 2020 2020 7379 6e63 4c6f 6361          syncLoca
+00001e50: 7469 6f6e 3d46 616c 7365 2c0d 0a20 2020  tion=False,..   
+00001e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e70: 2020 2020 6e61 6d65 3d22 6d65 6d62 6572      name="member
+00001e80: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00001e90: 2020 2020 2020 2020 2020 2066 6574 6368             fetch
+00001ea0: 4661 696c 6564 3d22 e695 b0e6 8dae e588  Failed="........
+00001eb0: 9de5 a78b e58c 96ef bc81 222c 0d0a 2020  ..........",..  
+00001ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ed0: 2020 2020 2061 7069 3d27 6765 743a 2f54       api='get:/T
+00001ee0: 6565 6e53 7475 6479 2f61 7069 2f67 6574  eenStudy/api/get
+00001ef0: 5f6d 656d 6265 7273 272c 0d0a 2020 2020  _members',..    
+00001f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f10: 2020 206c 6f61 6444 6174 614f 6e63 653d     loadDataOnce=
+00001f20: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+00001f30: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00001f40: 7465 7276 616c 3d31 3830 3030 302c 0d0a  terval=180000,..
+00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f60: 2020 2020 2020 2073 6f75 7263 653d 2724         source='$
+00001f70: 7b72 6f77 7320 7c20 6669 6c74 6572 3a75  {rows | filter:u
+00001f80: 7365 725f 6964 3a6b 6579 776f 7264 735f  ser_id:keywords_
+00001f90: 7573 6572 5f69 6420 7c20 6669 6c74 6572  user_id | filter
+00001fa0: 3a6e 616d 653a 6b65 7977 6f72 6473 5f6e  :name:keywords_n
+00001fb0: 616d 657c 6669 6c74 6572 3a61 7265 613a  ame|filter:area:
+00001fc0: 6b65 7977 6f72 6473 5f61 7265 617c 6669  keywords_area|fi
+00001fd0: 6c74 6572 3a75 6e69 7665 7273 6974 793a  lter:university:
+00001fe0: 6b65 7977 6f72 6473 5f75 6e69 7665 7273  keywords_univers
+00001ff0: 6974 797c 6669 6c74 6572 3a63 6f6c 6c65  ity|filter:colle
+00002000: 6765 3a6b 6579 776f 7264 735f 636f 6c6c  ge:keywords_coll
+00002010: 6567 657c 6669 6c74 6572 3a6f 7267 616e  ege|filter:organ
+00002020: 697a 6174 696f 6e3a 6b65 7977 6f72 6473  ization:keywords
+00002030: 5f6f 7267 616e 697a 6174 696f 6e7d 272c  _organization}',
+00002040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002050: 2020 2020 2020 2020 2066 696c 7465 723d           filter=
+00002060: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+00002070: 2020 2020 2020 2020 2020 2020 2020 2762                'b
+00002080: 6f64 7927 3a20 5b0d 0a20 2020 2020 2020  ody': [..       
+00002090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020a0: 2020 2020 2020 2020 496e 7075 7454 6578          InputTex
+000020b0: 7428 6e61 6d65 3d27 6b65 7977 6f72 6473  t(name='keywords
+000020c0: 5f75 7365 725f 6964 272c 206c 6162 656c  _user_id', label
+000020d0: 3d27 e794 a8e6 88b7 4944 272c 0d0a 2020  ='......ID',..  
 000020e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020f0: 2020 2020 2020 2020 2020 6e61 6d65 3d27            name='
-00002100: 7469 6d65 272c 2073 6f72 7461 626c 653d  time', sortable=
-00002110: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
-00002120: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
+000020f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002100: 2020 2020 2020 2074 7269 6d43 6f6e 7465         trimConte
+00002110: 6e74 733d 5472 7565 2c20 636c 6561 7261  nts=True, cleara
+00002120: 626c 653d 5472 7565 2c0d 0a20 2020 2020  ble=True,..     
 00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002140: 2020 2062 756c 6b41 6374 696f 6e73 3d5b     bulkActions=[
-00002150: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002160: 2020 2020 2020 2020 2020 4163 7469 6f6e            Action
-00002170: 5479 7065 2e41 6a61 7828 6c61 6265 6c3d  Type.Ajax(label=
-00002180: 27e6 89b9 e987 8fe5 88a0 e999 a427 2c0d  '............',.
-00002190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021b0: 2020 2020 2020 2020 206c 6576 656c 3d4c           level=L
-000021c0: 6576 656c 456e 756d 2e77 6172 6e69 6e67  evelEnum.warning
-000021d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000021e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021f0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00002200: 726d 5465 7874 3d22 e7a1 aee5 ae9a e8a6  rmText="........
-00002210: 81e6 89b9 e987 8fe5 88a0 e999 a4ef bc9f  ................
-00002220: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00002230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002240: 2020 2020 2020 2020 2020 2020 6170 693d              api=
-00002250: 2264 656c 6574 653a 2f54 6565 6e53 7475  "delete:/TeenStu
-00002260: 6479 2f61 7069 2f64 656c 6574 655f 616e  dy/api/delete_an
-00002270: 7377 6572 733f 6964 733d 247b 6964 737c  swers?ids=${ids|
-00002280: 7261 777d 2229 5d29 0d0a 0d0a 2222 2257  raw}")])...."""W
-00002290: 6562 e7ab afe9 858d e7bd aee8 a1a8 2222  eb............""
-000022a0: 220d 0a73 6574 7469 6e67 5f74 6162 6c65  "..setting_table
-000022b0: 203d 2046 6f72 6d28 0d0a 2020 2020 7469   = Form(..    ti
-000022c0: 746c 653d 2257 6562 e7ab afe9 858d e7bd  tle="Web........
-000022d0: ae22 2c0d 0a20 2020 2073 7562 6d69 7454  .",..    submitT
-000022e0: 6578 743d 22e4 bf9d e5ad 9822 2c0d 0a20  ext="......",.. 
-000022f0: 2020 2061 7069 3d22 7075 743a 2f54 6565     api="put:/Tee
-00002300: 6e53 7475 6479 2f61 7069 2f63 6861 6e67  nStudy/api/chang
-00002310: 655f 7365 7474 696e 6773 222c 0d0a 2020  e_settings",..  
-00002320: 2020 696e 6974 4170 693d 2267 6574 3a2f    initApi="get:/
-00002330: 5465 656e 5374 7564 792f 6170 692f 6765  TeenStudy/api/ge
-00002340: 745f 7365 7474 696e 6773 222c 0d0a 2020  t_settings",..  
-00002350: 2020 626f 6479 3d5b 0d0a 2020 2020 2020    body=[..      
-00002360: 2020 496e 7075 7454 6578 7428 0d0a 2020    InputText(..  
-00002370: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
-00002380: 5355 5045 5255 5345 5222 2c0d 0a20 2020  SUPERUSER",..   
-00002390: 2020 2020 2020 2020 206c 6162 656c 3d22           label="
-000023a0: e8b6 85e7 aea1 e799 bbe5 bd95 e8b4 a6e5  ................
-000023b0: 8fb7 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
-000023c0: 2020 6465 7363 7269 7074 696f 6e3d 22e8    description=".
-000023d0: b685 e7ae a1e7 99bb e5bd 95e8 b4a6 e58f  ................
-000023e0: b722 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
-000023f0: 2073 686f 7743 6f75 6e74 6572 3d54 7275   showCounter=Tru
-00002400: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00002410: 7661 6c75 653d 2224 7b53 5550 4552 5553  value="${SUPERUS
-00002420: 4552 7d22 2c0d 0a20 2020 2020 2020 2020  ER}",..         
-00002430: 2020 2074 7269 6d43 6f6e 7465 6e74 733d     trimContents=
-00002440: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
-00002450: 2020 206d 6178 4c65 6e67 7468 3d31 302c     maxLength=10,
-00002460: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00002470: 7175 6972 6564 3d54 7275 652c 0d0a 2020  quired=True,..  
-00002480: 2020 2020 2020 2020 2020 636c 6561 7261            cleara
-00002490: 626c 653d 5472 7565 0d0a 2020 2020 2020  ble=True..      
-000024a0: 2020 292c 0d0a 2020 2020 2020 2020 496e    ),..        In
-000024b0: 7075 7454 6578 7428 0d0a 2020 2020 2020  putText(..      
-000024c0: 2020 2020 2020 6e61 6d65 3d22 7061 7373        name="pass
-000024d0: 776f 7264 222c 0d0a 2020 2020 2020 2020  word",..        
-000024e0: 2020 2020 6c61 6265 6c3d 22e8 b685 e7ae      label=".....
-000024f0: a1e7 99bb e5bd 95e5 af86 e7a0 8122 2c0d  .............",.
-00002500: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-00002510: 6372 6970 7469 6f6e 3d22 e8b6 85e7 aea1  cription="......
-00002520: e799 bbe5 bd95 e5af 86e7 a081 efbc 8ce5  ................
-00002530: 8faf e4b8 8de5 a1ab efbc 8ce9 bb98 e8ae  ................
-00002540: a4e6 98af 6164 6d69 6e22 2c0d 0a20 2020  ....admin",..   
-00002550: 2020 2020 2020 2020 2073 686f 7743 6f75           showCou
-00002560: 6e74 6572 3d54 7275 652c 0d0a 2020 2020  nter=True,..    
-00002570: 2020 2020 2020 2020 6d61 784c 656e 6774          maxLengt
-00002580: 683d 3136 2c0d 0a20 2020 2020 2020 2020  h=16,..         
-00002590: 2020 2076 616c 7565 3d22 222c 0d0a 2020     value="",..  
-000025a0: 2020 2020 2020 2020 2020 7472 696d 436f            trimCo
-000025b0: 6e74 656e 7473 3d54 7275 652c 0d0a 2020  ntents=True,..  
-000025c0: 2020 2020 2020 2020 2020 7265 7175 6972            requir
-000025d0: 6564 3d46 616c 7365 2c20 636c 6561 7261  ed=False, cleara
-000025e0: 626c 653d 5472 7565 0d0a 0d0a 2020 2020  ble=True....    
-000025f0: 2020 2020 292c 0d0a 2020 2020 2020 2020      ),..        
-00002600: 496e 7075 7454 6578 7428 0d0a 2020 2020  InputText(..    
-00002610: 2020 2020 2020 2020 6e61 6d65 3d22 544f          name="TO
-00002620: 4b45 4e5f 5449 4d45 222c 0d0a 2020 2020  KEN_TIME",..    
-00002630: 2020 2020 2020 2020 6c61 6265 6c3d 2274          label="t
-00002640: 6f6b 656e e5a4 b1e6 9588 e697 b6e9 97b4  oken............
-00002650: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00002660: 6465 7363 7269 7074 696f 6e3d 2257 6562  description="Web
-00002670: e8ae bfe9 97ae 746f 6b65 6ee5 a4b1 e695  ......token.....
-00002680: 88e6 97b6 e997 b4ef bc8c e58d 95e4 bd8d  ................
-00002690: e4b8 bae5 8886 e992 9f22 2c0d 0a20 2020  .........",..   
-000026a0: 2020 2020 2020 2020 2073 686f 7743 6f75           showCou
-000026b0: 6e74 6572 3d54 7275 652c 0d0a 2020 2020  nter=True,..    
-000026c0: 2020 2020 2020 2020 6d61 784c 656e 6774          maxLengt
-000026d0: 683d 332c 0d0a 2020 2020 2020 2020 2020  h=3,..          
-000026e0: 2020 7661 6c75 653d 2224 7b54 4f4b 454e    value="${TOKEN
-000026f0: 5f54 494d 457d 222c 0d0a 2020 2020 2020  _TIME}",..      
-00002700: 2020 2020 2020 7472 696d 436f 6e74 656e        trimConten
-00002710: 7473 3d54 7275 652c 0d0a 2020 2020 2020  ts=True,..      
-00002720: 2020 2020 2020 7265 7365 7456 616c 7565        resetValue
-00002730: 3d33 302c 0d0a 2020 2020 2020 2020 2020  =30,..          
-00002740: 2020 7265 7175 6972 6564 3d54 7275 652c    required=True,
-00002750: 0d0a 2020 2020 2020 2020 2020 2020 636c  ..            cl
-00002760: 6561 7261 626c 653d 5472 7565 0d0a 2020  earable=True..  
-00002770: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
-00002780: 2020 496e 7075 7454 6578 7428 0d0a 2020    InputText(..  
-00002790: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
-000027a0: 4b45 5922 2c0d 0a20 2020 2020 2020 2020  KEY",..         
-000027b0: 2020 206c 6162 656c 3d22 e58a a0e5 af86     label="......
-000027c0: e7a7 98e9 92a5 222c 0d0a 2020 2020 2020  ......",..      
-000027d0: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-000027e0: 6e3d 22e5 8aa0 e5af 86e7 a798 e992 a5ef  n=".............
-000027f0: bc8c e4b8 ba36 34e4 bd8d e593 88e5 b88c  .....64.........
-00002800: e695 a3e5 8897 e580 bcef bc8c e794 a8e4  ................
-00002810: ba8e e794 9fe6 8890 746f 6b65 6e22 2c0d  ........token",.
-00002820: 0a20 2020 2020 2020 2020 2020 2073 686f  .            sho
-00002830: 7743 6f75 6e74 6572 3d54 7275 652c 0d0a  wCounter=True,..
-00002840: 2020 2020 2020 2020 2020 2020 6d61 784c              maxL
-00002850: 656e 6774 683d 3634 2c0d 0a20 2020 2020  ength=64,..     
-00002860: 2020 2020 2020 2076 616c 7565 3d22 247b         value="${
-00002870: 4b45 597d 222c 0d0a 2020 2020 2020 2020  KEY}",..        
-00002880: 2020 2020 7265 7365 7456 616c 7565 3d22      resetValue="
-00002890: 6438 3266 6661 6439 3131 3638 6662 3332  d82ffad91168fb32
-000028a0: 3461 6236 6562 6332 6265 6438 6461 6364  4ab6ebc2bed8dacd
-000028b0: 3433 6635 6166 3865 3334 6164 3064 3162  43f5af8e34ad0d1b
-000028c0: 3735 6438 3361 3061 6666 3936 3661 3036  75d83a0aff966a06
-000028d0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000028e0: 7472 696d 436f 6e74 656e 7473 3d54 7275  trimContents=Tru
-000028f0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00002900: 7265 7175 6972 6564 3d54 7275 652c 2063  required=True, c
-00002910: 6c65 6172 6162 6c65 3d54 7275 650d 0a20  learable=True.. 
-00002920: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
-00002930: 2020 2049 6e70 7574 5465 7874 280d 0a20     InputText(.. 
-00002940: 2020 2020 2020 2020 2020 206e 616d 653d             name=
-00002950: 2241 4c47 4f52 4954 484d 222c 0d0a 2020  "ALGORITHM",..  
-00002960: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
-00002970: 22e5 8aa0 e5af 86e7 ae97 e6b3 9522 2c0d  "............",.
-00002980: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-00002990: 6372 6970 7469 6f6e 3d22 e794 9fe6 8890  cription="......
-000029a0: 746f 6b65 6ee7 9a84 e7ae 97e6 b395 222c  token.........",
-000029b0: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-000029c0: 6c75 653d 2224 7b41 4c47 4f52 4954 484d  lue="${ALGORITHM
-000029d0: 7d22 2c0d 0a20 2020 2020 2020 2020 2020  }",..           
-000029e0: 2074 7269 6d43 6f6e 7465 6e74 733d 5472   trimContents=Tr
-000029f0: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-00002a00: 2073 686f 7743 6f75 6e74 6572 3d54 7275   showCounter=Tru
+00002140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002150: 2020 2020 7375 626d 6974 4f6e 4368 616e      submitOnChan
+00002160: 6765 3d54 7275 6529 2c0d 0a20 2020 2020  ge=True),..     
+00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002180: 2020 2020 2020 2020 2020 496e 7075 7454            InputT
+00002190: 6578 7428 6e61 6d65 3d27 6b65 7977 6f72  ext(name='keywor
+000021a0: 6473 5f6e 616d 6527 2c20 6c61 6265 6c3d  ds_name', label=
+000021b0: 27e7 94a8 e688 b7e5 a793 e590 8d27 2c0d  '............',.
+000021c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000021d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021e0: 2020 2020 2020 2020 2020 7472 696d 436f            trimCo
+000021f0: 6e74 656e 7473 3d54 7275 652c 2063 6c65  ntents=True, cle
+00002200: 6172 6162 6c65 3d54 7275 652c 0d0a 2020  arable=True,..  
+00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002230: 2020 2020 2020 2073 7562 6d69 744f 6e43         submitOnC
+00002240: 6861 6e67 653d 5472 7565 292c 0d0a 2020  hange=True),..  
+00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002260: 2020 2020 2020 2020 2020 2020 2049 6e70               Inp
+00002270: 7574 5465 7874 286e 616d 653d 276b 6579  utText(name='key
+00002280: 776f 7264 735f 6172 6561 272c 206c 6162  words_area', lab
+00002290: 656c 3d27 e59c b0e5 8cba 272c 0d0a 2020  el='......',..  
+000022a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022c0: 2020 2020 2020 2074 7269 6d43 6f6e 7465         trimConte
+000022d0: 6e74 733d 5472 7565 2c20 636c 6561 7261  nts=True, cleara
+000022e0: 626c 653d 5472 7565 2c0d 0a20 2020 2020  ble=True,..     
+000022f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002310: 2020 2020 7375 626d 6974 4f6e 4368 616e      submitOnChan
+00002320: 6765 3d54 7275 6529 2c0d 0a20 2020 2020  ge=True),..     
+00002330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002340: 2020 2020 2020 2020 2020 496e 7075 7454            InputT
+00002350: 6578 7428 6e61 6d65 3d27 6b65 7977 6f72  ext(name='keywor
+00002360: 6473 5f75 6e69 7665 7273 6974 7927 2c20  ds_university', 
+00002370: 6c61 6265 6c3d 27e5 ada6 e6a0 a127 2c0d  label='......',.
+00002380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023a0: 2020 2020 2020 2020 2020 7472 696d 436f            trimCo
+000023b0: 6e74 656e 7473 3d54 7275 652c 2063 6c65  ntents=True, cle
+000023c0: 6172 6162 6c65 3d54 7275 652c 0d0a 2020  arable=True,..  
+000023d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023f0: 2020 2020 2020 2073 7562 6d69 744f 6e43         submitOnC
+00002400: 6861 6e67 653d 5472 7565 292c 0d0a 2020  hange=True),..  
+00002410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002420: 2020 2020 2020 2020 2020 2020 2049 6e70               Inp
+00002430: 7574 5465 7874 286e 616d 653d 276b 6579  utText(name='key
+00002440: 776f 7264 735f 636f 6c6c 6567 6527 2c20  words_college', 
+00002450: 6c61 6265 6c3d 27e5 ada6 e999 a227 2c0d  label='......',.
+00002460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002480: 2020 2020 2020 2020 2020 7472 696d 436f            trimCo
+00002490: 6e74 656e 7473 3d54 7275 652c 2063 6c65  ntents=True, cle
+000024a0: 6172 6162 6c65 3d54 7275 652c 0d0a 2020  arable=True,..  
+000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024d0: 2020 2020 2020 2073 7562 6d69 744f 6e43         submitOnC
+000024e0: 6861 6e67 653d 5472 7565 292c 0d0a 2020  hange=True),..  
+000024f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002500: 2020 2020 2020 2020 2020 2020 2049 6e70               Inp
+00002510: 7574 5465 7874 286e 616d 653d 276b 6579  utText(name='key
+00002520: 776f 7264 735f 6f72 6761 6e69 7a61 7469  words_organizati
+00002530: 6f6e 272c 206c 6162 656c 3d27 e59b a2e6  on', label='....
+00002540: 94af e983 a827 2c0d 0a20 2020 2020 2020  .....',..       
+00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002570: 2020 7472 696d 436f 6e74 656e 7473 3d54    trimContents=T
+00002580: 7275 652c 2063 6c65 6172 6162 6c65 3d54  rue, clearable=T
+00002590: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000025c0: 7562 6d69 744f 6e43 6861 6e67 653d 5472  ubmitOnChange=Tr
+000025d0: 7565 292c 0d0a 2020 2020 2020 2020 2020  ue),..          
+000025e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025f0: 205d 0d0a 2020 2020 2020 2020 2020 2020   ]..            
+00002600: 2020 2020 2020 2020 2020 207d 2c0d 0a20             },.. 
+00002610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002620: 2020 2020 2020 7065 7250 6167 653d 3136        perPage=16
+00002630: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00002640: 2020 2020 2020 2020 2020 6175 746f 4a75            autoJu
+00002650: 6d70 546f 546f 704f 6e50 6167 6572 4368  mpToTopOnPagerCh
+00002660: 616e 6765 3d54 7275 652c 0d0a 2020 2020  ange=True,..    
+00002670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002680: 2020 2070 6c61 6365 686f 6c64 6572 3d27     placeholder='
+00002690: e69a 82e6 97a0 e5a4 a7e5 ada6 e4b9 a0e7  ................
+000026a0: 94a8 e688 b727 2c0d 0a20 2020 2020 2020  .....',..       
+000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026c0: 666f 6f74 6572 546f 6f6c 6261 723d 5b27  footerToolbar=['
+000026d0: 7377 6974 6368 2d70 6572 2d70 6167 6527  switch-per-page'
+000026e0: 2c20 2770 6167 696e 6174 696f 6e27 5d2c  , 'pagination'],
+000026f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002700: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
+00002710: 436f 756e 743d 342c 0d0a 2020 2020 2020  Count=4,..      
+00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002730: 2063 6172 643d 6361 7264 290d 0a0d 0a6c   card=card)....l
+00002740: 6973 745f 7061 6765 203d 2050 6167 6553  ist_page = PageS
+00002750: 6368 656d 6128 7572 6c3d 272f 5465 656e  chema(url='/Teen
+00002760: 5374 7564 792f 6c69 7374 272c 2069 636f  Study/list', ico
+00002770: 6e3d 2766 6120 6661 2d6c 6973 742d 756c  n='fa fa-list-ul
+00002780: 272c 206c 6162 656c 3d27 e688 90e5 9198  ', label='......
+00002790: e588 97e8 a1a8 272c 0d0a 2020 2020 2020  ......',..      
+000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027b0: 2073 6368 656d 613d 5061 6765 2874 6974   schema=Page(tit
+000027c0: 6c65 3d27 e688 90e5 9198 e588 97e8 a1a8  le='............
+000027d0: 272c 2062 6f64 793d 5b63 6172 6473 5f63  ', body=[cards_c
+000027e0: 7572 645d 2929 0d0a 0d0a 2222 22e6 b996  urd]))...."""...
+000027f0: e58c 97e6 b7bb e58a a0e6 8890 e591 98e9  ................
+00002800: 9da2 e69d bf22 2222 0d0a 6875 6265 695f  ....."""..hubei_
+00002810: 7461 626c 6520 3d20 466f 726d 280d 0a20  table = Form(.. 
+00002820: 2020 2074 6974 6c65 3d22 e6b7 bbe5 8aa0     title="......
+00002830: e99d 92e6 98a5 e6b9 96e5 8c97 e794 a8e6  ................
+00002840: 88b7 222c 0d0a 2020 2020 7375 626d 6974  ..",..    submit
+00002850: 5465 7874 3d22 e6b7 bbe5 8aa0 222c 0d0a  Text="......",..
+00002860: 2020 2020 6d6f 6465 3d44 6973 706c 6179      mode=Display
+00002870: 4d6f 6465 456e 756d 2e68 6f72 697a 6f6e  ModeEnum.horizon
+00002880: 7461 6c2c 0d0a 2020 2020 6170 693d 2270  tal,..    api="p
+00002890: 6f73 743a 2f54 6565 6e53 7475 6479 2f61  ost:/TeenStudy/a
+000028a0: 7069 2f61 6464 222c 0d0a 2020 2020 7265  pi/add",..    re
+000028b0: 7365 7441 6674 6572 5375 626d 6974 3d54  setAfterSubmit=T
+000028c0: 7275 652c 0d0a 2020 2020 626f 6479 3d5b  rue,..    body=[
+000028d0: 0d0a 2020 2020 2020 2020 5365 6c65 6374  ..        Select
+000028e0: 280d 0a20 2020 2020 2020 2020 2020 206c  (..            l
+000028f0: 6162 656c 3d22 e7be a4e8 818a 222c 0d0a  abel="......",..
+00002900: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+00002910: 3d22 6772 6f75 705f 6964 222c 0d0a 2020  ="group_id",..  
+00002920: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+00002930: 7074 696f 6e3d 22e9 9c80 e8a6 81e6 b7bb  ption=".........
+00002940: e58a a0e7 9a84 e7be a4e7 bb84 222c 0d0a  ............",..
+00002950: 2020 2020 2020 2020 2020 2020 6368 6563              chec
+00002960: 6b41 6c6c 3d46 616c 7365 2c0d 0a20 2020  kAll=False,..   
+00002970: 2020 2020 2020 2020 2073 6f75 7263 653d           source=
+00002980: 2267 6574 3a2f 5465 656e 5374 7564 792f  "get:/TeenStudy/
+00002990: 6170 692f 6765 745f 6772 6f75 705f 6c69  api/get_group_li
+000029a0: 7374 222c 0d0a 2020 2020 2020 2020 2020  st",..          
+000029b0: 2020 7661 6c75 653d 2727 2c0d 0a20 2020    value='',..   
+000029c0: 2020 2020 2020 2020 206d 756c 7469 706c           multipl
+000029d0: 653d 4661 6c73 652c 0d0a 2020 2020 2020  e=False,..      
+000029e0: 2020 2020 2020 7265 7175 6972 6564 3d54        required=T
+000029f0: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+00002a00: 2020 7365 6172 6368 6162 6c65 3d54 7275    searchable=Tru
 00002a10: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00002a20: 7265 7175 6972 6564 3d54 7275 652c 0d0a  required=True,..
-00002a30: 2020 2020 2020 2020 2020 2020 7265 7365              rese
-00002a40: 7456 616c 7565 3d22 4853 3235 3622 2c0d  tValue="HS256",.
-00002a50: 0a20 2020 2020 2020 2020 2020 2063 6c65  .            cle
-00002a60: 6172 6162 6c65 3d54 7275 650d 0a20 2020  arable=True..   
-00002a70: 2020 2020 2029 2c0d 0a20 2020 2020 2020       ),..       
-00002a80: 2049 6e70 7574 5465 7874 280d 0a20 2020   InputText(..   
-00002a90: 2020 2020 2020 2020 206e 616d 653d 2244           name="D
-00002aa0: 5858 5f49 5022 2c0d 0a20 2020 2020 2020  XX_IP",..       
-00002ab0: 2020 2020 206c 6162 656c 3d22 e585 ace7       label="....
-00002ac0: bd91 e8ae bfe9 97ae 4950 222c 0d0a 2020  ........IP",..  
-00002ad0: 2020 2020 2020 2020 2020 7661 6c75 653d            value=
-00002ae0: 2224 7b44 5858 5f49 507d 222c 0d0a 2020  "${DXX_IP}",..  
-00002af0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00002b00: 7074 696f 6e3d 22e5 85ac e7bd 91e8 aebf  ption=".........
-00002b10: e997 ae49 50ef bc8c e794 a8e4 ba8e e5a4  ...IP...........
-00002b20: 96e7 bd91 e8ae bfe9 97ae 222c 0d0a 2020  ..........",..  
-00002b30: 2020 2020 2020 2020 2020 7368 6f77 436f            showCo
-00002b40: 756e 7465 723d 5472 7565 2c0d 0a20 2020  unter=True,..   
-00002b50: 2020 2020 2020 2020 2074 7269 6d43 6f6e           trimCon
-00002b60: 7465 6e74 733d 5472 7565 2c0d 0a20 2020  tents=True,..   
-00002b70: 2020 2020 2020 2020 2072 6573 6574 5661           resetVa
-00002b80: 6c75 653d 2230 2e30 2e30 2e30 222c 0d0a  lue="0.0.0.0",..
-00002b90: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-00002ba0: 6972 6564 3d54 7275 652c 0d0a 2020 2020  ired=True,..    
-00002bb0: 2020 2020 2020 2020 636c 6561 7261 626c          clearabl
-00002bc0: 653d 5472 7565 0d0a 2020 2020 2020 2020  e=True..        
-00002bd0: 292c 0d0a 2020 2020 2020 2020 496e 7075  ),..        Inpu
-00002be0: 744e 756d 6265 7228 0d0a 2020 2020 2020  tNumber(..      
-00002bf0: 2020 2020 2020 6e61 6d65 3d22 4458 585f        name="DXX_
-00002c00: 504f 5254 222c 0d0a 2020 2020 2020 2020  PORT",..        
-00002c10: 2020 2020 6469 7370 6c61 794d 6f64 653d      displayMode=
-00002c20: 2265 6e68 616e 6365 222c 0d0a 2020 2020  "enhance",..    
-00002c30: 2020 2020 2020 2020 6c61 6265 6c3d 22e5          label=".
-00002c40: 85ac e7bd 91e8 aebf e997 aee7 abaf e58f  ................
-00002c50: a322 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
-00002c60: 2076 616c 7565 3d22 247b 4458 585f 504f   value="${DXX_PO
-00002c70: 5254 7d22 2c0d 0a20 2020 2020 2020 2020  RT}",..         
-00002c80: 2020 206d 696e 3d30 2c0d 0a20 2020 2020     min=0,..     
-00002c90: 2020 2020 2020 206d 6178 3d36 3535 3335         max=65535
-00002ca0: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
-00002cb0: 6573 6372 6970 7469 6f6e 3d22 e585 ace7  escription="....
-00002cc0: bd91 e8ae bfe9 97ae e7ab afe5 8fa3 efbc  ................
-00002cd0: 8ce7 94a8 e4ba 8ee5 a496 e7bd 91e8 aebf  ................
-00002ce0: e997 aeef bc8c e4b8 8de9 858d e7bd aee5  ................
-00002cf0: 9f9f e590 8de5 928c e58f 8de5 9091 e4bb  ................
-00002d00: a3e7 9086 e8af b7e5 8bbf e4bf aee6 94b9  ................
-00002d10: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00002d20: 7368 6f77 436f 756e 7465 723d 5472 7565  showCounter=True
-00002d30: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
-00002d40: 7269 6d43 6f6e 7465 6e74 733d 5472 7565  rimContents=True
-00002d50: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
-00002d60: 6573 6574 5661 6c75 653d 3830 3830 2c0d  esetValue=8080,.
-00002d70: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-00002d80: 7569 7265 643d 5472 7565 2c0d 0a20 2020  uired=True,..   
-00002d90: 2020 2020 2020 2020 2063 6c65 6172 6162           clearab
-00002da0: 6c65 3d54 7275 650d 0a20 2020 2020 2020  le=True..       
-00002db0: 2029 2c0d 0a20 2020 2020 2020 2053 7769   ),..        Swi
-00002dc0: 7463 6828 0d0a 2020 2020 2020 2020 2020  tch(..          
-00002dd0: 2020 6e61 6d65 3d22 5552 4c5f 5354 4154    name="URL_STAT
-00002de0: 5553 222c 0d0a 2020 2020 2020 2020 2020  US",..          
-00002df0: 2020 6c61 6265 6c3d 22e4 ba8c e7bb b4e7    label=".......
-00002e00: a081 e8bd ace9 93be e68e a5e5 bc80 e585  ................
-00002e10: b322 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
-00002e20: 2076 616c 7565 3d22 247b 5552 4c5f 5354   value="${URL_ST
-00002e30: 4154 5553 7d22 2c0d 0a20 2020 2020 2020  ATUS}",..       
-00002e40: 2020 2020 206f 6e54 6578 743d 27e5 bc80       onText='...
-00002e50: e590 af27 2c0d 0a20 2020 2020 2020 2020  ...',..         
-00002e60: 2020 206f 6666 5465 7874 3d27 e585 b3e9     offText='....
-00002e70: 97ad 272c 0d0a 2020 2020 2020 2020 2020  ..',..          
-00002e80: 2020 7265 7175 6972 6564 3d54 7275 652c    required=True,
-00002e90: 0d0a 2020 2020 2020 2020 292c 0d0a 2020  ..        ),..  
-00002ea0: 2020 2020 2020 5377 6974 6368 280d 0a20        Switch(.. 
-00002eb0: 2020 2020 2020 2020 2020 206e 616d 653d             name=
-00002ec0: 2250 4f4b 455f 5355 424d 4954 222c 0d0a  "POKE_SUBMIT",..
-00002ed0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-00002ee0: 6c3d 22e6 88b3 e4b8 80e6 88b3 e68f 90e4  l=".............
-00002ef0: baa4 e5a4 a7e5 ada6 e4b9 a0e5 bc80 e585  ................
-00002f00: b322 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
-00002f10: 2076 616c 7565 3d22 247b 504f 4b45 5f53   value="${POKE_S
-00002f20: 5542 4d49 547d 222c 0d0a 2020 2020 2020  UBMIT}",..      
-00002f30: 2020 2020 2020 6f6e 5465 7874 3d27 e5bc        onText='..
-00002f40: 80e5 90af 272c 0d0a 2020 2020 2020 2020  ....',..        
-00002f50: 2020 2020 6f66 6654 6578 743d 27e5 85b3      offText='...
-00002f60: e997 ad27 2c0d 0a20 2020 2020 2020 2020  ...',..         
-00002f70: 2020 2072 6571 7569 7265 643d 5472 7565     required=True
-00002f80: 2c0d 0a20 2020 2020 2020 2029 2c0d 0a20  ,..        ),.. 
-00002f90: 2020 2020 2020 2053 7769 7463 6828 0d0a         Switch(..
-00002fa0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00002fb0: 3d22 4458 585f 5245 4d49 4e44 222c 0d0a  ="DXX_REMIND",..
-00002fc0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-00002fd0: 6c3d 22e5 a4a7 e5ad a6e4 b9a0 e68f 90e9  l=".............
-00002fe0: 8692 e5bc 80e5 85b3 222c 0d0a 2020 2020  ........",..    
-00002ff0: 2020 2020 2020 2020 7661 6c75 653d 2224          value="$
-00003000: 7b44 5858 5f52 454d 494e 447d 222c 0d0a  {DXX_REMIND}",..
-00003010: 2020 2020 2020 2020 2020 2020 6f6e 5465              onTe
-00003020: 7874 3d27 e5bc 80e5 90af 272c 0d0a 2020  xt='......',..  
-00003030: 2020 2020 2020 2020 2020 6f66 6654 6578            offTex
-00003040: 743d 27e5 85b3 e997 ad27 2c0d 0a20 2020  t='......',..   
-00003050: 2020 2020 2020 2020 2072 6571 7569 7265           require
-00003060: 643d 5472 7565 2c0d 0a20 2020 2020 2020  d=True,..       
-00003070: 2029 2c0d 0a20 2020 2020 2020 2049 6e70   ),..        Inp
-00003080: 7574 5469 6d65 280d 0a20 2020 2020 2020  utTime(..       
-00003090: 2020 2020 206e 616d 653d 2272 656d 696e       name="remin
-000030a0: 6422 2c0d 0a20 2020 2020 2020 2020 2020  d",..           
-000030b0: 206c 6162 656c 3d22 e68f 90e9 8692 e697   label="........
-000030c0: b6e9 97b4 222c 0d0a 2020 2020 2020 2020  ....",..        
-000030d0: 2020 2020 7479 7065 3d22 696e 7075 742d      type="input-
-000030e0: 7469 6d65 222c 0d0a 2020 2020 2020 2020  time",..        
-000030f0: 2020 2020 7265 7175 6972 6564 3d54 7275      required=Tru
-00003100: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00003110: 7661 6c75 653d 2224 7b72 656d 696e 647d  value="${remind}
-00003120: 222c 0d0a 2020 2020 2020 2020 292c 0d0a  ",..        ),..
-00003130: 2020 2020 2020 2020 5377 6974 6368 280d          Switch(.
-00003140: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
-00003150: 653d 2241 5554 4f5f 5355 424d 4954 222c  e="AUTO_SUBMIT",
-00003160: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
-00003170: 6265 6c3d 22e5 a4a7 e5ad a6e4 b9a0 e887  bel="...........
-00003180: aae5 8aa8 e68f 90e4 baa4 e5bc 80e5 85b3  ................
-00003190: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000031a0: 7661 6c75 653d 2224 7b41 5554 4f5f 5355  value="${AUTO_SU
-000031b0: 424d 4954 7d22 2c0d 0a20 2020 2020 2020  BMIT}",..       
-000031c0: 2020 2020 206f 6e54 6578 743d 27e5 bc80       onText='...
-000031d0: e590 af27 2c0d 0a20 2020 2020 2020 2020  ...',..         
-000031e0: 2020 206f 6666 5465 7874 3d27 e585 b3e9     offText='....
-000031f0: 97ad 272c 0d0a 2020 2020 2020 2020 2020  ..',..          
-00003200: 2020 7265 7175 6972 6564 3d54 7275 652c    required=True,
-00003210: 0d0a 2020 2020 2020 2020 292c 0d0a 2020  ..        ),..  
-00003220: 2020 2020 2020 496e 7075 7454 696d 6528        InputTime(
-00003230: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
-00003240: 6d65 3d22 6175 746f 222c 0d0a 2020 2020  me="auto",..    
-00003250: 2020 2020 2020 2020 6c61 6265 6c3d 22e8          label=".
-00003260: 87aa e58a a8e6 8f90 e4ba a4e6 97b6 e997  ................
-00003270: b422 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
-00003280: 2074 7970 653d 2269 6e70 7574 2d74 696d   type="input-tim
-00003290: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
-000032a0: 2072 6571 7569 7265 643d 5472 7565 2c0d   required=True,.
-000032b0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-000032c0: 7565 3d22 247b 6175 746f 7d22 2c0d 0a20  ue="${auto}",.. 
-000032d0: 2020 2020 2020 2029 2c0d 0a20 2020 205d         ),..    ]
-000032e0: 0d0a 290d 0a22 2222 e794 b3e8 afb7 e8ae  ..).."""........
-000032f0: b0e5 bd95 e6a8 a1e6 9dbf 2222 220d 0a72  .........."""..r
-00003300: 6571 7565 7374 5f74 6162 6c65 203d 2043  equest_table = C
-00003310: 5255 4428 6d6f 6465 3d27 7461 626c 6527  RUD(mode='table'
-00003320: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003330: 2020 2020 2020 2020 7469 746c 653d 2727          title=''
-00003340: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003350: 2020 2020 2020 2020 7379 6e63 4c6f 6361          syncLoca
-00003360: 7469 6f6e 3d46 616c 7365 2c0d 0a20 2020  tion=False,..   
-00003370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003380: 2020 6170 693d 272f 5465 656e 5374 7564    api='/TeenStud
-00003390: 792f 6170 692f 6765 745f 7265 7175 6573  y/api/get_reques
-000033a0: 7473 272c 0d0a 2020 2020 2020 2020 2020  ts',..          
-000033b0: 2020 2020 2020 2020 2020 2069 6e74 6572             inter
-000033c0: 7661 6c3d 3630 3030 302c 0d0a 2020 2020  val=60000,..    
-000033d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033e0: 2074 7970 653d 2763 7275 6427 2c0d 0a20   type='crud',.. 
-000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003400: 2020 2020 6865 6164 6572 546f 6f6c 6261      headerToolba
-00003410: 723d 5b41 6374 696f 6e54 7970 652e 416a  r=[ActionType.Aj
-00003420: 6178 286c 6162 656c 3d27 e588 a0e9 99a4  ax(label='......
-00003430: e689 80e6 9c89 e794 b3e8 afb7 e8ae b0e5  ................
-00003440: bd95 272c 0d0a 2020 2020 2020 2020 2020  ..',..          
-00003450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003470: 2020 2020 2020 2020 2020 6c65 7665 6c3d            level=
-00003480: 4c65 7665 6c45 6e75 6d2e 7761 726e 696e  LevelEnum.warnin
-00003490: 672c 0d0a 2020 2020 2020 2020 2020 2020  g,..            
-000034a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034c0: 2020 2020 2020 2020 636f 6e66 6972 6d54          confirmT
-000034d0: 6578 743d 27e7 a1ae e5ae 9ae8 a681 e588  ext='...........
-000034e0: a0e9 99a4 e689 80e6 9c89 e794 b3e8 afb7  ................
-000034f0: e8ae b0e5 bd95 e590 97ef bc9f 272c 0d0a  ............',..
-00003500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003530: 2020 2020 6170 693d 2764 656c 6574 653a      api='delete:
-00003540: 2f54 6565 6e53 7475 6479 2f61 7069 2f64  /TeenStudy/api/d
-00003550: 656c 6574 655f 616c 6c3f 7479 7065 3d72  elete_all?type=r
-00003560: 6571 7565 7374 7327 292c 0d0a 2020 2020  equests'),..    
-00003570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003590: 2262 756c 6b41 6374 696f 6e73 222c 2022  "bulkActions", "
-000035a0: 7265 6c6f 6164 225d 2c0d 0a20 2020 2020  reload"],..     
-000035b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035c0: 6974 656d 4163 7469 6f6e 733d 5b0d 0a20  itemActions=[.. 
-000035d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035e0: 2020 2020 2020 2020 4163 7469 6f6e 5479          ActionTy
-000035f0: 7065 2e41 6a61 7828 746f 6f6c 7469 703d  pe.Ajax(tooltip=
-00003600: 27e5 88a0 e999 a427 2c0d 0a20 2020 2020  '......',..     
-00003610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003630: 2020 2020 6963 6f6e 3d27 6661 2066 612d      icon='fa fa-
-00003640: 7469 6d65 7320 7465 7874 2d64 616e 6765  times text-dange
-00003650: 7227 2c0d 0a20 2020 2020 2020 2020 2020  r',..           
-00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003670: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00003680: 6e66 6972 6d54 6578 743d 27e5 88a0 e999  nfirmText='.....
-00003690: a4e8 afa5 e69d a1e7 94b3 e8af b7e8 aeb0  ................
-000036a0: e5bd 9527 2c0d 0a20 2020 2020 2020 2020  ...',..         
-000036b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036d0: 6170 693d 2764 656c 6574 653a 2f54 6565  api='delete:/Tee
-000036e0: 6e53 7475 6479 2f61 7069 2f64 656c 6574  nStudy/api/delet
-000036f0: 655f 7265 7175 6573 743f 6964 3d24 7b69  e_request?id=${i
-00003700: 647d 2729 0d0a 2020 2020 2020 2020 2020  d}')..          
-00003710: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
-00003720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003730: 2020 2020 666f 6f74 6162 6c65 3d54 7275      footable=Tru
-00003740: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00003750: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
-00003760: 3d5b 0d0a 2020 2020 2020 2020 2020 2020  =[..            
-00003770: 2020 2020 2020 2020 2020 2020 2054 6162               Tab
-00003780: 6c65 436f 6c75 6d6e 286c 6162 656c 3d27  leColumn(label='
-00003790: e794 b3e8 afb7 4944 272c 206e 616d 653d  ......ID', name=
-000037a0: 2775 7365 725f 6964 272c 2073 6561 7263  'user_id', searc
-000037b0: 6861 626c 653d 5472 7565 292c 0d0a 2020  hable=True),..  
-000037c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037d0: 2020 2020 2020 2054 6162 6c65 436f 6c75         TableColu
-000037e0: 6d6e 286c 6162 656c 3d27 e794 b3e8 afb7  mn(label='......
-000037f0: e7be a4e5 8fb7 272c 206e 616d 653d 2767  ......', name='g
-00003800: 726f 7570 5f69 6427 2c20 7365 6172 6368  roup_id', search
-00003810: 6162 6c65 3d54 7275 6529 2c0d 0a20 2020  able=True),..   
-00003820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003830: 2020 2020 2020 5461 626c 6543 6f6c 756d        TableColum
-00003840: 6e28 6c61 6265 6c3d 27e7 94b3 e8af b7e5  n(label='.......
-00003850: 9cb0 e58c ba27 2c20 6e61 6d65 3d27 6172  .....', name='ar
-00003860: 6561 272c 2073 6561 7263 6861 626c 653d  ea', searchable=
-00003870: 5472 7565 292c 0d0a 2020 2020 2020 2020  True),..        
-00003880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003890: 2054 6162 6c65 436f 6c75 6d6e 286c 6162   TableColumn(lab
-000038a0: 656c 3d27 e794 b3e8 afb7 e78a b6e6 8081  el='............
-000038b0: 272c 206e 616d 653d 2773 7461 7475 7327  ', name='status'
-000038c0: 2c20 7365 6172 6368 6162 6c65 3d54 7275  , searchable=Tru
-000038d0: 6529 2c0d 0a20 2020 2020 2020 2020 2020  e),..           
-000038e0: 2020 2020 2020 2020 2020 2020 2020 5461                Ta
-000038f0: 626c 6543 6f6c 756d 6e28 7479 7065 3d27  bleColumn(type='
-00003900: 7470 6c27 2c20 7470 6c3d 2724 7b74 696d  tpl', tpl='${tim
-00003910: 657c 6461 7465 3a59 5959 592d 4d4d 2d44  e|date:YYYY-MM-D
-00003920: 4420 4848 5c5c 3a6d 6d5c 5c3a 7373 7d27  D HH\\:mm\\:ss}'
-00003930: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003950: 2020 2020 2020 2020 6c61 6265 6c3d 27e7          label='.
-00003960: 94b3 e8af b7e6 97b6 e997 b427 2c0d 0a20  ...........',.. 
-00003970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003990: 2020 2020 6e61 6d65 3d27 7469 6d65 272c      name='time',
-000039a0: 2073 6f72 7461 626c 653d 5472 7565 290d   sortable=True).
-000039b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000039c0: 2020 2020 2020 5d2c 0d0a 2020 2020 2020        ],..      
-000039d0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-000039e0: 756c 6b41 6374 696f 6e73 3d5b 0d0a 2020  ulkActions=[..  
-000039f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a00: 2020 2020 2020 2041 6374 696f 6e54 7970         ActionTyp
-00003a10: 652e 416a 6178 286c 6162 656c 3d27 e689  e.Ajax(label='..
-00003a20: b9e9 878f e588 a0e9 99a4 272c 0d0a 2020  ..........',..  
-00003a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a50: 2020 2020 2020 206c 6576 656c 3d4c 6576         level=Lev
-00003a60: 656c 456e 756d 2e77 6172 6e69 6e67 2c0d  elEnum.warning,.
-00003a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a90: 2020 2020 2020 2020 2020 636f 6e66 6972            confir
-00003aa0: 6d54 6578 743d 22e7 a1ae e5ae 9ae8 a681  mText=".........
-00003ab0: e689 b9e9 878f e588 a0e9 99a4 efbc 9f22  ..............."
-00003ac0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ae0: 2020 2020 2020 2020 2020 2020 6170 693d              api=
-00003af0: 2264 656c 6574 653a 2f54 6565 6e53 7475  "delete:/TeenStu
-00003b00: 6479 2f61 7069 2f64 656c 6574 655f 7265  dy/api/delete_re
-00003b10: 7175 6573 7473 3f69 6473 3d24 7b69 6473  quests?ids=${ids
-00003b20: 7c72 6177 7d22 295d 290d 0a64 6574 6169  |raw}")])..detai
-00003b30: 6c5f 666f 726d 203d 2046 6f72 6d28 0d0a  l_form = Form(..
-00003b40: 2020 2020 7469 746c 653d 2727 2c0d 0a20      title='',.. 
-00003b50: 2020 2061 7069 3d27 7075 743a 2f54 6565     api='put:/Tee
-00003b60: 6e53 7475 6479 2f61 7069 2f63 6861 6e67  nStudy/api/chang
-00003b70: 653f 7573 6572 5f69 643d 247b 7573 6572  e?user_id=${user
-00003b80: 5f69 647d 272c 0d0a 2020 2020 7375 626d  _id}',..    subm
-00003b90: 6974 5465 7874 3d27 e4bf 9de5 ad98 e4bf  itText='........
-00003ba0: aee6 94b9 272c 0d0a 2020 2020 6d6f 6465  ....',..    mode
-00003bb0: 3d44 6973 706c 6179 4d6f 6465 456e 756d  =DisplayModeEnum
-00003bc0: 2e68 6f72 697a 6f6e 7461 6c2c 0d0a 2020  .horizontal,..  
-00003bd0: 2020 6c61 6265 6c41 6c69 676e 3d27 7269    labelAlign='ri
-00003be0: 6768 7427 2c0d 0a20 2020 2062 6f64 793d  ght',..    body=
-00003bf0: 5b0d 0a20 2020 2020 2020 2053 656c 6563  [..        Selec
-00003c00: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
-00003c10: 6c61 6265 6c3d 22e9 809a e79f a5e7 bea4  label=".........
-00003c20: e881 8a22 2c0d 0a20 2020 2020 2020 2020  ...",..         
-00003c30: 2020 206e 616d 653d 2267 726f 7570 5f69     name="group_i
-00003c40: 6422 2c0d 0a20 2020 2020 2020 2020 2020  d",..           
-00003c50: 2064 6573 6372 6970 7469 6f6e 3d22 e5a4   description="..
-00003c60: a7e5 ada6 e4b9 a0e6 8f90 e986 92e7 bea4  ................
-00003c70: e58f b722 2c0d 0a20 2020 2020 2020 2020  ...",..         
-00003c80: 2020 2063 6865 636b 416c 6c3d 4661 6c73     checkAll=Fals
-00003c90: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00003ca0: 736f 7572 6365 3d22 6765 743a 2f54 6565  source="get:/Tee
-00003cb0: 6e53 7475 6479 2f61 7069 2f67 6574 5f67  nStudy/api/get_g
-00003cc0: 726f 7570 5f6c 6973 7422 2c0d 0a20 2020  roup_list",..   
-00003cd0: 2020 2020 2020 2020 2076 616c 7565 3d27           value='
-00003ce0: 247b 6772 6f75 705f 6964 7d27 2c0d 0a20  ${group_id}',.. 
-00003cf0: 2020 2020 2020 2020 2020 206d 756c 7469             multi
-00003d00: 706c 653d 4661 6c73 652c 0d0a 2020 2020  ple=False,..    
-00003d10: 2020 2020 2020 2020 7265 7175 6972 6564          required
-00003d20: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
-00003d30: 2020 2020 7365 6172 6368 6162 6c65 3d54      searchable=T
-00003d40: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-00003d50: 2020 6a6f 696e 5661 6c75 6573 3d46 616c    joinValues=Fal
-00003d60: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-00003d70: 2065 7874 7261 6374 5661 6c75 653d 5472   extractValue=Tr
-00003d80: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-00003d90: 2073 7461 7469 7374 6963 733d 5472 7565   statistics=True
-00003da0: 2c0d 0a20 2020 2020 2020 2029 2c0d 0a20  ,..        ),.. 
-00003db0: 2020 2020 2020 2049 6e70 7574 5465 7874         InputText
-00003dc0: 286c 6162 656c 3d27 e680 a7e5 88ab 272c  (label='......',
-00003dd0: 206e 616d 653d 2767 656e 6465 7227 2c20   name='gender', 
-00003de0: 7661 6c75 653d 2724 7b67 656e 6465 727d  value='${gender}
-00003df0: 272c 2072 6571 7569 7265 643d 5472 7565  ', required=True
-00003e00: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003e10: 2020 2020 2074 7269 6d43 6f6e 7465 6e74       trimContent
-00003e20: 733d 5472 7565 2c20 636c 6561 7261 626c  s=True, clearabl
-00003e30: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
-00003e40: 2020 2020 2020 2020 2020 2073 686f 7743             showC
-00003e50: 6f75 6e74 6572 3d54 7275 652c 206d 6178  ounter=True, max
-00003e60: 4c65 6e67 7468 3d33 2c20 7669 7369 626c  Length=3, visibl
-00003e70: 654f 6e3d 2224 7b67 656e 6465 723d 3d6e  eOn="${gender==n
-00003e80: 756c 6c3f 6661 6c73 653a 7472 7565 7d22  ull?false:true}"
-00003e90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003ea0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-00003eb0: 3d27 e680 a7e5 88ab 2729 2c0d 0a20 2020  ='......'),..   
-00003ec0: 2020 2020 2049 6e70 7574 5465 7874 286c       InputText(l
-00003ed0: 6162 656c 3d27 7569 647c 6e69 6427 2c20  abel='uid|nid', 
-00003ee0: 6e61 6d65 3d27 6478 785f 6964 272c 2076  name='dxx_id', v
-00003ef0: 616c 7565 3d27 247b 6478 785f 6964 7d27  alue='${dxx_id}'
-00003f00: 2c20 7265 7175 6972 6564 3d54 7275 652c  , required=True,
-00003f10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003f20: 2020 2020 7472 696d 436f 6e74 656e 7473      trimContents
-00003f30: 3d54 7275 652c 2063 6c65 6172 6162 6c65  =True, clearable
-00003f40: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
-00003f50: 2020 2020 2020 2020 2020 7368 6f77 436f            showCo
-00003f60: 756e 7465 723d 5472 7565 2c20 6d61 784c  unter=True, maxL
-00003f70: 656e 6774 683d 3234 2c20 7669 7369 626c  ength=24, visibl
-00003f80: 654f 6e3d 2224 7b64 7878 5f69 643d 3d6e  eOn="${dxx_id==n
-00003f90: 756c 6c3f 6661 6c73 653a 7472 7565 7d22  ull?false:true}"
-00003fa0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003fb0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-00003fc0: 3d27 e5a4 a7e5 ada6 e4b9 a0e8 aea4 e8af  ='..............
-00003fd0: 8149 44ef bc8c e4b8 8de6 b885 e6a5 9ae8  .ID.............
-00003fe0: afb7 e58b bfe6 94b9 e58a a827 292c 0d0a  ...........'),..
-00003ff0: 2020 2020 2020 2020 496e 7075 7454 6578          InputTex
-00004000: 7428 6c61 6265 6c3d 27e6 898b e69c bae5  t(label='.......
-00004010: 8fb7 7ce5 ada6 e58f b727 2c20 6e61 6d65  ..|......', name
-00004020: 3d27 6d6f 6269 6c65 272c 2076 616c 7565  ='mobile', value
-00004030: 3d27 247b 6d6f 6269 6c65 7d27 2c20 7265  ='${mobile}', re
-00004040: 7175 6972 6564 3d46 616c 7365 2c0d 0a20  quired=False,.. 
-00004050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004060: 2074 7269 6d43 6f6e 7465 6e74 733d 5472   trimContents=Tr
-00004070: 7565 2c20 636c 6561 7261 626c 653d 5472  ue, clearable=Tr
-00004080: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-00004090: 2020 2020 2020 2073 686f 7743 6f75 6e74         showCount
-000040a0: 6572 3d54 7275 652c 206d 6178 4c65 6e67  er=True, maxLeng
-000040b0: 7468 3d32 342c 2076 6973 6962 6c65 4f6e  th=24, visibleOn
-000040c0: 3d22 247b 6d6f 6269 6c65 3d3d 6e75 6c6c  ="${mobile==null
-000040d0: 3f66 616c 7365 3a74 7275 657d 222c 0d0a  ?false:true}",..
-000040e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040f0: 2020 6465 7363 7269 7074 696f 6e3d 27e6    description='.
-00004100: 898b e69c bae5 8fb7 2729 2c0d 0a20 2020  ........'),..   
-00004110: 2020 2020 2049 6e70 7574 5465 7874 286c       InputText(l
-00004120: 6162 656c 3d27 e59b a2e6 94af e4b9 a649  abel='.........I
-00004130: 4427 2c20 6e61 6d65 3d27 6c65 6164 6572  D', name='leader
-00004140: 272c 2076 616c 7565 3d27 247b 6c65 6164  ', value='${lead
-00004150: 6572 7d27 2c0d 0a20 2020 2020 2020 2020  er}',..         
-00004160: 2020 2020 2020 2020 2073 686f 7743 6f75           showCou
-00004170: 6e74 6572 3d54 7275 652c 206d 6178 4c65  nter=True, maxLe
-00004180: 6e67 7468 3d31 302c 2068 6964 6465 6e4f  ngth=10, hiddenO
-00004190: 6e3d 5472 7565 2c20 7472 696d 436f 6e74  n=True, trimCont
-000041a0: 656e 7473 3d54 7275 652c 0d0a 2020 2020  ents=True,..    
-000041b0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-000041c0: 6561 7261 626c 653d 5472 7565 2c0d 0a20  earable=True,.. 
-000041d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041e0: 2064 6573 6372 6970 7469 6f6e 3d27 e59b   description='..
-000041f0: a2e6 94af e4b9 a649 44ef bc8c e5a1 abe5  .......ID.......
-00004200: 8699 e590 8ee5 9ba2 e694 afe4 b9a6 e58f  ................
-00004210: afe6 938d e4bd 9ce6 8f90 e4ba a4e5 8a9f  ................
-00004220: e883 bdef bc8c e4b8 8de6 b885 e6a5 9ae8  ................
-00004230: afb7 e58b bfe6 94b9 e58a a827 292c 0d0a  ...........'),..
-00004240: 2020 2020 2020 2020 496e 7075 7454 6578          InputTex
-00004250: 7428 6c61 6265 6c3d 276f 7065 6e69 6427  t(label='openid'
-00004260: 2c20 6e61 6d65 3d27 6f70 656e 6964 272c  , name='openid',
-00004270: 2076 616c 7565 3d27 247b 6f70 656e 6964   value='${openid
-00004280: 7d27 2c20 7265 7175 6972 6564 3d54 7275  }', required=Tru
-00004290: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-000042a0: 2020 2020 2020 7472 696d 436f 6e74 656e        trimConten
-000042b0: 7473 3d54 7275 652c 2063 6c65 6172 6162  ts=True, clearab
-000042c0: 6c65 3d54 7275 652c 0d0a 2020 2020 2020  le=True,..      
-000042d0: 2020 2020 2020 2020 2020 2020 7368 6f77              show
-000042e0: 436f 756e 7465 723d 5472 7565 2c20 6d61  Counter=True, ma
-000042f0: 784c 656e 6774 683d 3634 2c20 7669 7369  xLength=64, visi
-00004300: 626c 654f 6e3d 2224 7b6f 7065 6e69 643d  bleOn="${openid=
-00004310: 3d6e 756c 6c3f 6661 6c73 653a 7472 7565  =null?false:true
-00004320: 7d22 2c0d 0a20 2020 2020 2020 2020 2020  }",..           
-00004330: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00004340: 6f6e 3d27 e5be aee4 bfa1 e8ae a4e8 af81  on='............
-00004350: 4944 efbc 8ce4 b88d e6b8 85e6 a59a e8af  ID..............
-00004360: b7e5 8bbf e694 b9e5 8aa8 2729 2c0d 0a20  ..........'),.. 
-00004370: 2020 2020 2020 2049 6e70 7574 5465 7874         InputText
-00004380: 286c 6162 656c 3d27 e799 bbe5 bd95 e5af  (label='........
-00004390: 86e7 a081 272c 206e 616d 653d 2750 6173  ....', name='Pas
-000043a0: 7377 6f72 6427 2c20 7661 6c75 653d 2727  sword', value=''
-000043b0: 2c20 7479 7065 3d22 696e 7075 742d 7061  , type="input-pa
-000043c0: 7373 776f 7264 222c 0d0a 2020 2020 2020  ssword",..      
-000043d0: 2020 2020 2020 2020 2020 2020 7472 696d              trim
-000043e0: 436f 6e74 656e 7473 3d54 7275 652c 2063  Contents=True, c
-000043f0: 6c65 6172 6162 6c65 3d54 7275 652c 0d0a  learable=True,..
-00004400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004410: 2020 7368 6f77 436f 756e 7465 723d 5472    showCounter=Tr
-00004420: 7565 2c20 6d61 784c 656e 6774 683d 3136  ue, maxLength=16
-00004430: 2c20 7669 7369 626c 654f 6e3d 2224 7b70  , visibleOn="${p
-00004440: 6173 7377 6f72 643d 3d6e 756c 6c3f 6661  assword==null?fa
-00004450: 6c73 653a 7472 7565 7d22 2c0d 0a20 2020  lse:true}",..   
-00004460: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004470: 6573 6372 6970 7469 6f6e 3d27 e799 bbe5  escription='....
-00004480: bd95 5765 6220 5549 e79a 84e5 af86 e7a0  ..Web UI........
-00004490: 8127 292c 0d0a 2020 2020 2020 2020 496e  .'),..        In
-000044a0: 7075 7454 6578 7428 6c61 6265 6c3d 27e5  putText(label='.
-000044b0: ada6 e6a0 a1e7 b1bb e59e 8b27 2c20 6e61  ...........', na
-000044c0: 6d65 3d27 756e 6976 6572 7369 7479 5f74  me='university_t
-000044d0: 7970 6527 2c20 7661 6c75 653d 2724 7b75  ype', value='${u
-000044e0: 6e69 7665 7273 6974 795f 7479 7065 7d27  niversity_type}'
-000044f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00004500: 2020 2020 2073 686f 7743 6f75 6e74 6572       showCounter
-00004510: 3d54 7275 652c 206d 6178 4c65 6e67 7468  =True, maxLength
-00004520: 3d31 362c 2072 6571 7569 7265 643d 5472  =16, required=Tr
-00004530: 7565 2c20 7472 696d 436f 6e74 656e 7473  ue, trimContents
-00004540: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
-00004550: 2020 2020 2020 2020 2020 636c 6561 7261            cleara
-00004560: 626c 653d 5472 7565 2c0d 0a20 2020 2020  ble=True,..     
-00004570: 2020 2020 2020 2020 2020 2020 2076 6973               vis
-00004580: 6962 6c65 4f6e 3d22 247b 756e 6976 6572  ibleOn="${univer
-00004590: 7369 7479 5f74 7970 653d 3d6e 756c 6c3f  sity_type==null?
-000045a0: 6661 6c73 653a 7472 7565 7d22 2c0d 0a20  false:true}",.. 
-000045b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045c0: 2064 6573 6372 6970 7469 6f6e 3d27 e5ad   description='..
-000045d0: a6e6 a0a1 e7b1 bbe5 9e8b efbc 8ce4 b88d  ................
-000045e0: e6b8 85e6 a59a e6b8 85e6 97a0 e694 b9e5  ................
-000045f0: 8aa8 2729 2c0d 0a20 2020 2020 2020 2049  ..'),..        I
-00004600: 6e70 7574 5465 7874 286c 6162 656c 3d27  nputText(label='
-00004610: e5ad a6e6 a0a1 4944 272c 206e 616d 653d  ......ID', name=
-00004620: 2775 6e69 7665 7273 6974 795f 6964 272c  'university_id',
-00004630: 2076 616c 7565 3d27 247b 756e 6976 6572   value='${univer
-00004640: 7369 7479 5f69 647d 272c 0d0a 2020 2020  sity_id}',..    
-00004650: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00004660: 7175 6972 6564 3d54 7275 652c 2074 7269  quired=True, tri
-00004670: 6d43 6f6e 7465 6e74 733d 5472 7565 2c20  mContents=True, 
-00004680: 636c 6561 7261 626c 653d 5472 7565 2c0d  clearable=True,.
-00004690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000046a0: 2020 2073 686f 7743 6f75 6e74 6572 3d54     showCounter=T
-000046b0: 7275 652c 206d 6178 4c65 6e67 7468 3d32  rue, maxLength=2
-000046c0: 342c 0d0a 2020 2020 2020 2020 2020 2020  4,..            
-000046d0: 2020 2020 2020 7669 7369 626c 654f 6e3d        visibleOn=
-000046e0: 2224 7b75 6e69 7665 7273 6974 795f 6964  "${university_id
-000046f0: 3d3d 6e75 6c6c 3f66 616c 7365 3a74 7275  ==null?false:tru
-00004700: 657d 222c 0d0a 2020 2020 2020 2020 2020  e}",..          
-00004710: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-00004720: 696f 6e3d 27e5 ada6 e6a0 a149 44ef bc8c  ion='......ID...
-00004730: e4b8 8de6 b885 e6a5 9ae8 afb7 e58b bfe6  ................
-00004740: 94b9 e58a a827 292c 0d0a 2020 2020 2020  .....'),..      
-00004750: 2020 496e 7075 7454 6578 7428 6c61 6265    InputText(labe
-00004760: 6c3d 27e5 ada6 e6a0 a1e5 908d e7a7 b027  l='............'
-00004770: 2c20 6e61 6d65 3d27 756e 6976 6572 7369  , name='universi
-00004780: 7479 272c 2076 616c 7565 3d27 247b 756e  ty', value='${un
-00004790: 6976 6572 7369 7479 7d27 2c20 7265 7175  iversity}', requ
-000047a0: 6972 6564 3d54 7275 652c 0d0a 2020 2020  ired=True,..    
-000047b0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-000047c0: 696d 436f 6e74 656e 7473 3d54 7275 652c  imContents=True,
-000047d0: 2063 6c65 6172 6162 6c65 3d54 7275 652c   clearable=True,
-000047e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000047f0: 2020 2020 7368 6f77 436f 756e 7465 723d      showCounter=
-00004800: 5472 7565 2c20 6d61 784c 656e 6774 683d  True, maxLength=
-00004810: 3230 2c20 7669 7369 626c 654f 6e3d 2224  20, visibleOn="$
-00004820: 7b75 6e69 7665 7273 6974 793d 3d6e 756c  {university==nul
-00004830: 6c3f 6661 6c73 653a 7472 7565 7d22 2c0d  l?false:true}",.
-00004840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004850: 2020 2064 6573 6372 6970 7469 6f6e 3d27     description='
-00004860: e5ad a6e6 a0a1 e590 8de7 a7b0 2729 2c0d  ............'),.
-00004870: 0a20 2020 2020 2020 2049 6e70 7574 5465  .        InputTe
-00004880: 7874 286c 6162 656c 3d27 e5ad a6e9 99a2  xt(label='......
-00004890: 4944 272c 206e 616d 653d 2763 6f6c 6c65  ID', name='colle
-000048a0: 6765 5f69 6427 2c20 7661 6c75 653d 2724  ge_id', value='$
-000048b0: 7b63 6f6c 6c65 6765 5f69 647d 272c 2072  {college_id}', r
-000048c0: 6571 7569 7265 643d 4661 6c73 652c 0d0a  equired=False,..
-000048d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048e0: 2020 7472 696d 436f 6e74 656e 7473 3d54    trimContents=T
-000048f0: 7275 652c 2063 6c65 6172 6162 6c65 3d54  rue, clearable=T
-00004900: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-00004910: 2020 2020 2020 2020 7368 6f77 436f 756e          showCoun
-00004920: 7465 723d 5472 7565 2c20 6d61 784c 656e  ter=True, maxLen
-00004930: 6774 683d 3234 2c20 7669 7369 626c 654f  gth=24, visibleO
-00004940: 6e3d 2224 7b63 6f6c 6c65 6765 5f69 643d  n="${college_id=
-00004950: 3d6e 756c 6c3f 6661 6c73 653a 7472 7565  =null?false:true
-00004960: 7d22 2c0d 0a20 2020 2020 2020 2020 2020  }",..           
-00004970: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00004980: 6f6e 3d27 e5ad a6e9 99a2 4944 2729 2c0d  on='......ID'),.
-00004990: 0a20 2020 2020 2020 2049 6e70 7574 5465  .        InputTe
-000049a0: 7874 286c 6162 656c 3d27 e5ad a6e9 99a2  xt(label='......
-000049b0: e590 8de7 a7b0 272c 206e 616d 653d 2763  ......', name='c
-000049c0: 6f6c 6c65 6765 272c 2076 616c 7565 3d27  ollege', value='
-000049d0: 247b 636f 6c6c 6567 657d 272c 0d0a 2020  ${college}',..  
-000049e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049f0: 7472 696d 436f 6e74 656e 7473 3d54 7275  trimContents=Tru
-00004a00: 652c 2063 6c65 6172 6162 6c65 3d54 7275  e, clearable=Tru
-00004a10: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00004a20: 2020 2020 2020 7368 6f77 436f 756e 7465        showCounte
-00004a30: 723d 5472 7565 2c20 6d61 784c 656e 6774  r=True, maxLengt
-00004a40: 683d 3234 2c20 7669 7369 626c 654f 6e3d  h=24, visibleOn=
-00004a50: 2224 7b63 6f6c 6c65 6765 3d3d 6e75 6c6c  "${college==null
-00004a60: 3f66 616c 7365 3a74 7275 657d 222c 0d0a  ?false:true}",..
-00004a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a80: 2020 6465 7363 7269 7074 696f 6e3d 27e5    description='.
-00004a90: ada6 e999 a2e5 908d e7a7 b027 292c 0d0a  ...........'),..
-00004aa0: 2020 2020 2020 2020 496e 7075 7454 6578          InputTex
-00004ab0: 7428 6c61 6265 6c3d 27e5 9ba2 e694 afe9  t(label='.......
-00004ac0: 83a8 4944 272c 206e 616d 653d 276f 7267  ..ID', name='org
-00004ad0: 616e 697a 6174 696f 6e5f 6964 272c 2076  anization_id', v
-00004ae0: 616c 7565 3d27 247b 6f72 6761 6e69 7a61  alue='${organiza
-00004af0: 7469 6f6e 5f69 647d 272c 0d0a 2020 2020  tion_id}',..    
-00004b00: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00004b10: 7175 6972 6564 3d54 7275 652c 2074 7269  quired=True, tri
-00004b20: 6d43 6f6e 7465 6e74 733d 5472 7565 2c20  mContents=True, 
-00004b30: 636c 6561 7261 626c 653d 5472 7565 2c0d  clearable=True,.
-00004b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004b50: 2020 2073 686f 7743 6f75 6e74 6572 3d54     showCounter=T
-00004b60: 7275 652c 206d 6178 4c65 6e67 7468 3d32  rue, maxLength=2
-00004b70: 342c 0d0a 2020 2020 2020 2020 2020 2020  4,..            
-00004b80: 2020 2020 2020 7669 7369 626c 654f 6e3d        visibleOn=
-00004b90: 2224 7b6f 7267 616e 697a 6174 696f 6e5f  "${organization_
-00004ba0: 6964 3d3d 6e75 6c6c 3f66 616c 7365 3a74  id==null?false:t
-00004bb0: 7275 657d 222c 0d0a 2020 2020 2020 2020  rue}",..        
-00004bc0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00004bd0: 7074 696f 6e3d 27e5 9ba2 e694 afe9 83a8  ption='.........
-00004be0: 4944 2729 2c0d 0a20 2020 2020 2020 2049  ID'),..        I
-00004bf0: 6e70 7574 5465 7874 286c 6162 656c 3d27  nputText(label='
-00004c00: e59b a2e6 94af e983 a8e5 908d e7a7 b027  ...............'
-00004c10: 2c20 6e61 6d65 3d27 6f72 6761 6e69 7a61  , name='organiza
-00004c20: 7469 6f6e 272c 2076 616c 7565 3d27 247b  tion', value='${
-00004c30: 6f72 6761 6e69 7a61 7469 6f6e 7d27 2c0d  organization}',.
-00004c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004c50: 2020 2072 6571 7569 7265 643d 4661 6c73     required=Fals
-00004c60: 652c 2074 7269 6d43 6f6e 7465 6e74 733d  e, trimContents=
-00004c70: 5472 7565 2c20 636c 6561 7261 626c 653d  True, clearable=
-00004c80: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
-00004c90: 2020 2020 2020 2020 2073 686f 7743 6f75           showCou
-00004ca0: 6e74 6572 3d54 7275 652c 206d 6178 4c65  nter=True, maxLe
-00004cb0: 6e67 7468 3d33 362c 0d0a 2020 2020 2020  ngth=36,..      
-00004cc0: 2020 2020 2020 2020 2020 2020 7669 7369              visi
-00004cd0: 626c 654f 6e3d 2224 7b6f 7267 616e 697a  bleOn="${organiz
-00004ce0: 6174 696f 6e3d 3d6e 756c 6c3f 6661 6c73  ation==null?fals
-00004cf0: 653a 7472 7565 7d22 2c0d 0a20 2020 2020  e:true}",..     
-00004d00: 2020 2020 2020 2020 2020 2020 2064 6573               des
-00004d10: 6372 6970 7469 6f6e 3d27 e59b a2e6 94af  cription='......
-00004d20: e983 a8e5 908d e7a7 b027 292c 0d0a 2020  .........'),..  
-00004d30: 2020 2020 2020 496e 7075 7454 6578 7428        InputText(
-00004d40: 6c61 6265 6c3d 2774 6f6b 656e 272c 206e  label='token', n
-00004d50: 616d 653d 2774 6f6b 656e 272c 2076 616c  ame='token', val
-00004d60: 7565 3d27 247b 746f 6b65 6e7d 272c 2072  ue='${token}', r
-00004d70: 6571 7569 7265 643d 5472 7565 2c0d 0a20  equired=True,.. 
-00004d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d90: 2074 7269 6d43 6f6e 7465 6e74 733d 5472   trimContents=Tr
-00004da0: 7565 2c20 636c 6561 7261 626c 653d 5472  ue, clearable=Tr
-00004db0: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-00004dc0: 2020 2020 2020 2073 686f 7743 6f75 6e74         showCount
-00004dd0: 6572 3d54 7275 652c 2076 6973 6962 6c65  er=True, visible
-00004de0: 4f6e 3d22 247b 746f 6b65 6e3d 3d6e 756c  On="${token==nul
-00004df0: 6c3f 6661 6c73 653a 7472 7565 7d22 2c0d  l?false:true}",.
-00004e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004e10: 2020 2064 6573 6372 6970 7469 6f6e 3d27     description='
-00004e20: e68f 90e4 baa4 e5a4 a7e5 ada6 e4b9 a0e9  ................
-00004e30: 9c80 e8a6 81e7 9a84 746f 6b65 6e27 292c  ........token'),
-00004e40: 0d0a 2020 2020 2020 2020 496e 7075 7454  ..        InputT
-00004e50: 6578 7428 6c61 6265 6c3d 2763 6f6f 6b69  ext(label='cooki
-00004e60: 6527 2c20 6e61 6d65 3d27 636f 6f6b 6965  e', name='cookie
-00004e70: 272c 2076 616c 7565 3d27 247b 636f 6f6b  ', value='${cook
-00004e80: 6965 7d27 2c20 7265 7175 6972 6564 3d54  ie}', required=T
-00004e90: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-00004ea0: 2020 2020 2020 2020 7472 696d 436f 6e74          trimCont
-00004eb0: 656e 7473 3d54 7275 652c 2063 6c65 6172  ents=True, clear
-00004ec0: 6162 6c65 3d54 7275 652c 0d0a 2020 2020  able=True,..    
-00004ed0: 2020 2020 2020 2020 2020 2020 2020 7368                sh
-00004ee0: 6f77 436f 756e 7465 723d 5472 7565 2c20  owCounter=True, 
-00004ef0: 7669 7369 626c 654f 6e3d 2224 7b63 6f6f  visibleOn="${coo
-00004f00: 6b69 653d 3d6e 756c 6c3f 6661 6c73 653a  kie==null?false:
-00004f10: 7472 7565 7d22 2c0d 0a20 2020 2020 2020  true}",..       
-00004f20: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-00004f30: 6970 7469 6f6e 3d27 e68f 90e4 baa4 e5a4  iption='........
-00004f40: a7e5 ada6 e4b9 a0e9 9c80 e8a6 81e7 9a84  ................
-00004f50: 636f 6f6b 6965 2729 0d0a 2020 2020 5d29  cookie')..    ])
-00004f60: 0d0a 6465 7461 696c 5f62 7574 746f 6e20  ..detail_button 
-00004f70: 3d20 4163 7469 6f6e 5479 7065 2e44 6961  = ActionType.Dia
-00004f80: 6c6f 6728 6c61 6265 6c3d 27e4 bfa1 e681  log(label='.....
-00004f90: af27 2c0d 0a20 2020 2020 2020 2020 2020  .',..           
-00004fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fb0: 2020 2020 2020 2074 6f6f 6c74 6970 3d27         tooltip='
-00004fc0: e69f a5e7 9c8b 7ce4 bfae e694 b9e4 bfa1  ......|.........
-00004fd0: e681 af27 2c0d 0a20 2020 2020 2020 2020  ...',..         
-00004fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ff0: 2020 2020 2020 2020 2073 697a 653d 276c           size='l
-00005000: 6727 2c0d 0a20 2020 2020 2020 2020 2020  g',..           
-00005010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005020: 2020 2020 2020 2069 636f 6e3d 2766 6120         icon='fa 
-00005030: 6661 2d75 7365 722d 7461 6720 7465 7874  fa-user-tag text
-00005040: 2d70 7269 6d61 7279 272c 0d0a 2020 2020  -primary',..    
-00005050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005060: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00005070: 616c 6f67 3d44 6961 6c6f 6728 7469 746c  alog=Dialog(titl
-00005080: 653d 2724 7b6e 616d 657d e79a 84e8 afa6  e='${name}......
-00005090: e7bb 86e4 bfa1 e681 af27 2c20 7369 7a65  .........', size
-000050a0: 3d27 6c67 272c 2062 6f64 793d 5b64 6574  ='lg', body=[det
-000050b0: 6169 6c5f 666f 726d 5d29 290d 0a63 6172  ail_form]))..car
-000050c0: 6420 3d20 4361 7264 280d 0a20 2020 2068  d = Card(..    h
-000050d0: 6561 6465 723d 4361 7264 2e48 6561 6465  eader=Card.Heade
-000050e0: 7228 7469 746c 653d 2724 6e61 6d65 272c  r(title='$name',
-000050f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005100: 2020 2020 2020 2020 2073 7562 5469 746c           subTitl
-00005110: 653d 2724 7573 6572 5f69 6427 2c0d 0a20  e='$user_id',.. 
-00005120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005130: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-00005140: 6e3d 2724 6361 7461 6c6f 6775 6527 2c0d  n='$catalogue',.
-00005150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005160: 2020 2020 2020 2020 6176 6174 6172 5465          avatarTe
-00005170: 7874 3d27 247b 6172 6561 7d27 2c0d 0a20  xt='${area}',.. 
-00005180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005190: 2020 2020 2020 6176 6174 6172 5465 7874        avatarText
-000051a0: 436c 6173 734e 616d 653d 276f 7665 7266  ClassName='overf
-000051b0: 6c6f 772d 6869 6464 656e 2729 2c0d 0a20  low-hidden'),.. 
-000051c0: 2020 2061 6374 696f 6e73 3d5b 6465 7461     actions=[deta
-000051d0: 696c 5f62 7574 746f 6e2c 2041 6374 696f  il_button, Actio
-000051e0: 6e54 7970 652e 416a 6178 280d 0a20 2020  nType.Ajax(..   
-000051f0: 2020 2020 206c 6162 656c 3d22 e68f 90e4       label="....
-00005200: baa4 222c 0d0a 2020 2020 2020 2020 746f  ..",..        to
-00005210: 6f6c 7469 703d 27e6 8f90 e4ba a4e5 a4a7  oltip='.........
-00005220: e5ad a6e4 b9a0 272c 0d0a 2020 2020 2020  ......',..      
-00005230: 2020 6963 6f6e 3d27 6661 2066 612d 6368    icon='fa fa-ch
-00005240: 6563 6b20 7465 7874 2d73 7563 6365 7373  eck text-success
-00005250: 272c 0d0a 2020 2020 2020 2020 636f 6e66  ',..        conf
-00005260: 6972 6d54 6578 743d 27e6 98af e590 a6e6  irmText='.......
-00005270: 8f90 e4ba a4e6 9c80 e696 b0e4 b880 e69c  ................
-00005280: 9fe9 9d92 e5b9 b4e5 a4a7 e5ad a6e4 b9a0  ................
-00005290: efbc 9f27 2c0d 0a20 2020 2020 2020 2061  ...',..        a
-000052a0: 7069 3d27 6765 743a 2f54 6565 6e53 7475  pi='get:/TeenStu
-000052b0: 6479 2f61 7069 2f63 6f6d 6d69 743f 7573  dy/api/commit?us
-000052c0: 6572 5f69 643d 247b 7573 6572 5f69 647d  er_id=${user_id}
-000052d0: 2661 7265 613d 247b 6172 6561 7d27 0d0a  &area=${area}'..
-000052e0: 2020 2020 292c 2041 6374 696f 6e54 7970      ), ActionTyp
-000052f0: 652e 416a 6178 280d 0a20 2020 2020 2020  e.Ajax(..       
-00005300: 2074 6f6f 6c74 6970 3d27 e588 a0e9 99a4   tooltip='......
-00005310: 272c 0d0a 2020 2020 2020 2020 6c61 6265  ',..        labe
-00005320: 6c3d 22e5 88a0 e999 a422 2c0d 0a20 2020  l="......",..   
-00005330: 2020 2020 2069 636f 6e3d 2766 6120 6661       icon='fa fa
-00005340: 2d74 7261 7368 2d63 616e 2074 6578 742d  -trash-can text-
-00005350: 6461 6e67 6572 272c 0d0a 2020 2020 2020  danger',..      
-00005360: 2020 636f 6e66 6972 6d54 6578 743d 27e5    confirmText='.
-00005370: 88a0 e999 a4e8 afa5 e794 a8e6 88b7 272c  ..............',
-00005380: 0d0a 2020 2020 2020 2020 6170 693d 2764  ..        api='d
-00005390: 656c 6574 653a 2f54 6565 6e53 7475 6479  elete:/TeenStudy
-000053a0: 2f61 7069 2f64 656c 6574 655f 6d65 6d62  /api/delete_memb
-000053b0: 6572 3f75 7365 725f 6964 3d24 7b75 7365  er?user_id=${use
-000053c0: 725f 6964 7d27 0d0a 2020 2020 292c 205d  r_id}'..    ), ]
-000053d0: 2c0d 0a20 2020 2074 6f6f 6c62 6172 3d5b  ,..    toolbar=[
-000053e0: 0d0a 2020 2020 2020 2020 5470 6c28 7470  ..        Tpl(tp
-000053f0: 6c3d 2724 6172 6561 272c 2063 6c61 7373  l='$area', class
-00005400: 4e61 6d65 3d27 6c61 6265 6c20 6c61 6265  Name='label labe
-00005410: 6c2d 7761 726e 696e 6727 2c20 6869 6464  l-warning', hidd
-00005420: 656e 4f6e 3d54 7275 6529 2c0d 0a20 2020  enOn=True),..   
-00005430: 2020 2020 2053 7769 7463 6828 6e61 6d65       Switch(name
-00005440: 3d27 6175 746f 5f73 7562 6d69 7427 2c0d  ='auto_submit',.
-00005450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005460: 7661 6c75 653d 2724 7b61 7574 6f5f 7375  value='${auto_su
-00005470: 626d 6974 7d27 2c0d 0a20 2020 2020 2020  bmit}',..       
-00005480: 2020 2020 2020 2020 746f 6f6c 7469 703d          tooltip=
-00005490: 27e8 87aa e58a a8e6 8f90 e4ba a4e5 a4a7  '...............
-000054a0: e5ad a6e4 b9a0 e5bc 80e5 85b3 272c 0d0a  ............',..
-000054b0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-000054c0: 6e54 6578 743d 27e5 bc80 e590 af27 2c0d  nText='......',.
-000054d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000054e0: 6f66 6654 6578 743d 27e5 85b3 e997 ad27  offText='......'
-000054f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005500: 2020 6f6e 4576 656e 743d 7b0d 0a20 2020    onEvent={..   
-00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005520: 2763 6861 6e67 6527 3a20 7b0d 0a20 2020  'change': {..   
-00005530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005540: 2020 2020 2761 6374 696f 6e73 273a 207b      'actions': {
-00005550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005560: 2020 2020 2020 2020 2020 2020 2027 6163               'ac
-00005570: 7469 6f6e 5479 7065 273a 2027 616a 6178  tionType': 'ajax
-00005580: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00005590: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000055a0: 6172 6773 273a 207b 0d0a 2020 2020 2020  args': {..      
-000055b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055c0: 2020 2020 2020 2020 2027 6170 6927 3a20           'api': 
-000055d0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055f0: 2020 2020 2020 2775 726c 273a 2027 2f54        'url': '/T
-00005600: 6565 6e53 7475 6479 2f61 7069 2f73 6574  eenStudy/api/set
-00005610: 5f61 7574 6f5f 7375 626d 6974 272c 0d0a  _auto_submit',..
-00005620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005640: 2020 2027 6d65 7468 6f64 273a 2027 7075     'method': 'pu
-00005650: 7427 0d0a 2020 2020 2020 2020 2020 2020  t'..            
-00005660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005670: 2020 207d 2c0d 0a20 2020 2020 2020 2020     },..         
-00005680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005690: 2020 2020 2020 276d 6573 7361 6765 7327        'messages'
-000056a0: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056c0: 2020 2020 2020 2020 2773 7563 6365 7373          'success
-000056d0: 273a 2027 e887 aae5 8aa8 e68f 90e4 baa4  ': '............
-000056e0: e5b7 b2e8 aebe e7bd aee4 b8ba 247b 6576  ............${ev
-000056f0: 656e 742e 6461 7461 2e76 616c 7565 3d3d  ent.data.value==
-00005700: 7472 7565 3f22 e5bc 80e5 90af 223a 22e5  true?"......":".
-00005710: 85b3 e997 ad22 7d27 2c0d 0a20 2020 2020  ....."}',..     
-00005720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005730: 2020 2020 2020 2020 2020 2020 2020 2766                'f
-00005740: 6169 6c65 6427 3a20 27e4 bfae e694 b9e5  ailed': '.......
-00005750: a4b1 e8b4 a5ef bc81 270d 0a20 2020 2020  ........'..     
-00005760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005770: 2020 2020 2020 2020 2020 7d2c 0d0a 2020            },..  
-00005780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005790: 2020 2020 2020 2020 2020 2020 2027 7374               'st
-000057a0: 6174 7573 273a 2027 247b 6576 656e 742e  atus': '${event.
-000057b0: 6461 7461 2e76 616c 7565 7d27 2c0d 0a20  data.value}',.. 
-000057c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057d0: 2020 2020 2020 2020 2020 2020 2020 2769                'i
-000057e0: 6427 3a20 2724 7b69 647d 270d 0a20 2020  d': '${id}'..   
-000057f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005800: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005820: 2020 7d0d 0a20 2020 2020 2020 2020 2020    }..           
-00005830: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-00005840: 2020 2020 2020 2020 2020 7d29 0d0a 2020            })..  
-00005850: 2020 5d29 0d0a 2222 22e6 8890 e591 98e5    ])..""".......
-00005860: 8da1 e789 87e9 9da2 e69d bf22 2222 0d0a  ..........."""..
-00005870: 6361 7264 735f 6375 7264 203d 2043 6172  cards_curd = Car
-00005880: 6473 4352 5544 286d 6f64 653d 2763 6172  dsCRUD(mode='car
-00005890: 6473 272c 0d0a 2020 2020 2020 2020 2020  ds',..          
-000058a0: 2020 2020 2020 2020 2020 2020 2074 6974               tit
-000058b0: 6c65 3d27 272c 0d0a 2020 2020 2020 2020  le='',..        
-000058c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000058d0: 796e 634c 6f63 6174 696f 6e3d 4661 6c73  yncLocation=Fals
-000058e0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-000058f0: 2020 2020 2020 2020 2020 206e 616d 653d             name=
-00005900: 226d 656d 6265 7222 2c0d 0a20 2020 2020  "member",..     
-00005910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005920: 2020 6665 7463 6846 6169 6c65 643d 22e6    fetchFailed=".
-00005930: 95b0 e68d aee5 889d e5a7 8be5 8c96 efbc  ................
-00005940: 8122 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
-00005950: 2020 2020 2020 2020 2020 2020 6170 693d              api=
-00005960: 2767 6574 3a2f 5465 656e 5374 7564 792f  'get:/TeenStudy/
-00005970: 6170 692f 6765 745f 6d65 6d62 6572 7327  api/get_members'
-00005980: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005990: 2020 2020 2020 2020 2020 6c6f 6164 4461            loadDa
-000059a0: 7461 4f6e 6365 3d54 7275 652c 0d0a 2020  taOnce=True,..  
-000059b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059c0: 2020 2020 2073 6f75 7263 653d 2724 7b72       source='${r
-000059d0: 6f77 7320 7c20 6669 6c74 6572 3a75 7365  ows | filter:use
-000059e0: 725f 6964 3a6b 6579 776f 7264 735f 7573  r_id:keywords_us
-000059f0: 6572 5f69 6420 7c20 6669 6c74 6572 3a6e  er_id | filter:n
-00005a00: 616d 653a 6b65 7977 6f72 6473 5f6e 616d  ame:keywords_nam
-00005a10: 657c 6669 6c74 6572 3a61 7265 613a 6b65  e|filter:area:ke
-00005a20: 7977 6f72 6473 5f61 7265 617c 6669 6c74  ywords_area|filt
-00005a30: 6572 3a75 6e69 7665 7273 6974 793a 6b65  er:university:ke
-00005a40: 7977 6f72 6473 5f75 6e69 7665 7273 6974  ywords_universit
-00005a50: 797c 6669 6c74 6572 3a63 6f6c 6c65 6765  y|filter:college
-00005a60: 3a6b 6579 776f 7264 735f 636f 6c6c 6567  :keywords_colleg
-00005a70: 657c 6669 6c74 6572 3a6f 7267 616e 697a  e|filter:organiz
-00005a80: 6174 696f 6e3a 6b65 7977 6f72 6473 5f6f  ation:keywords_o
-00005a90: 7267 616e 697a 6174 696f 6e7d 272c 0d0a  rganization}',..
-00005aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ab0: 2020 2020 2020 2066 696c 7465 723d 7b0d         filter={.
-00005ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005ad0: 2020 2020 2020 2020 2020 2020 2762 6f64              'bod
-00005ae0: 7927 3a20 5b0d 0a20 2020 2020 2020 2020  y': [..         
-00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b00: 2020 2020 2020 496e 7075 7454 6578 7428        InputText(
-00005b10: 6e61 6d65 3d27 6b65 7977 6f72 6473 5f75  name='keywords_u
-00005b20: 7365 725f 6964 272c 206c 6162 656c 3d27  ser_id', label='
-00005b30: e794 a8e6 88b7 4944 272c 0d0a 2020 2020  ......ID',..    
-00005b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b60: 2020 2020 2074 7269 6d43 6f6e 7465 6e74       trimContent
-00005b70: 733d 5472 7565 2c20 636c 6561 7261 626c  s=True, clearabl
-00005b80: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
-00005b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bb0: 2020 7375 626d 6974 4f6e 4368 616e 6765    submitOnChange
-00005bc0: 3d54 7275 6529 2c0d 0a20 2020 2020 2020  =True),..       
-00005bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005be0: 2020 2020 2020 2020 496e 7075 7454 6578          InputTex
-00005bf0: 7428 6e61 6d65 3d27 6b65 7977 6f72 6473  t(name='keywords
-00005c00: 5f6e 616d 6527 2c20 6c61 6265 6c3d 27e7  _name', label='.
-00005c10: 94a8 e688 b7e5 a793 e590 8d27 2c0d 0a20  ...........',.. 
-00005c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c40: 2020 2020 2020 2020 7472 696d 436f 6e74          trimCont
-00005c50: 656e 7473 3d54 7275 652c 2063 6c65 6172  ents=True, clear
-00005c60: 6162 6c65 3d54 7275 652c 0d0a 2020 2020  able=True,..    
-00005c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c90: 2020 2020 2073 7562 6d69 744f 6e43 6861       submitOnCha
-00005ca0: 6e67 653d 5472 7565 292c 0d0a 2020 2020  nge=True),..    
-00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cc0: 2020 2020 2020 2020 2020 2049 6e70 7574             Input
-00005cd0: 5465 7874 286e 616d 653d 276b 6579 776f  Text(name='keywo
-00005ce0: 7264 735f 6172 6561 272c 206c 6162 656c  rds_area', label
-00005cf0: 3d27 e59c b0e5 8cba 272c 0d0a 2020 2020  ='......',..    
-00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d20: 2020 2020 2074 7269 6d43 6f6e 7465 6e74       trimContent
-00005d30: 733d 5472 7565 2c20 636c 6561 7261 626c  s=True, clearabl
-00005d40: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
-00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d70: 2020 7375 626d 6974 4f6e 4368 616e 6765    submitOnChange
-00005d80: 3d54 7275 6529 2c0d 0a20 2020 2020 2020  =True),..       
-00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005da0: 2020 2020 2020 2020 496e 7075 7454 6578          InputTex
-00005db0: 7428 6e61 6d65 3d27 6b65 7977 6f72 6473  t(name='keywords
-00005dc0: 5f75 6e69 7665 7273 6974 7927 2c20 6c61  _university', la
-00005dd0: 6265 6c3d 27e5 ada6 e6a0 a127 2c0d 0a20  bel='......',.. 
-00005de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e00: 2020 2020 2020 2020 7472 696d 436f 6e74          trimCont
-00005e10: 656e 7473 3d54 7275 652c 2063 6c65 6172  ents=True, clear
-00005e20: 6162 6c65 3d54 7275 652c 0d0a 2020 2020  able=True,..    
-00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e50: 2020 2020 2073 7562 6d69 744f 6e43 6861       submitOnCha
-00005e60: 6e67 653d 5472 7565 292c 0d0a 2020 2020  nge=True),..    
-00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e80: 2020 2020 2020 2020 2020 2049 6e70 7574             Input
-00005e90: 5465 7874 286e 616d 653d 276b 6579 776f  Text(name='keywo
-00005ea0: 7264 735f 636f 6c6c 6567 6527 2c20 6c61  rds_college', la
-00005eb0: 6265 6c3d 27e5 ada6 e999 a227 2c0d 0a20  bel='......',.. 
-00005ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ee0: 2020 2020 2020 2020 7472 696d 436f 6e74          trimCont
-00005ef0: 656e 7473 3d54 7275 652c 2063 6c65 6172  ents=True, clear
-00005f00: 6162 6c65 3d54 7275 652c 0d0a 2020 2020  able=True,..    
-00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f30: 2020 2020 2073 7562 6d69 744f 6e43 6861       submitOnCha
-00005f40: 6e67 653d 5472 7565 292c 0d0a 2020 2020  nge=True),..    
-00005f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f60: 2020 2020 2020 2020 2020 2049 6e70 7574             Input
-00005f70: 5465 7874 286e 616d 653d 276b 6579 776f  Text(name='keywo
-00005f80: 7264 735f 6f72 6761 6e69 7a61 7469 6f6e  rds_organization
-00005f90: 272c 206c 6162 656c 3d27 e59b a2e6 94af  ', label='......
-00005fa0: e983 a827 2c0d 0a20 2020 2020 2020 2020  ...',..         
-00005fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fd0: 7472 696d 436f 6e74 656e 7473 3d54 7275  trimContents=Tru
-00005fe0: 652c 2063 6c65 6172 6162 6c65 3d54 7275  e, clearable=Tru
-00005ff0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00006000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006010: 2020 2020 2020 2020 2020 2020 2073 7562               sub
-00006020: 6d69 744f 6e43 6861 6e67 653d 5472 7565  mitOnChange=True
-00006030: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-00006040: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00006050: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006060: 2020 2020 2020 2020 207d 2c0d 0a20 2020           },..   
-00006070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006080: 2020 2020 7065 7250 6167 653d 3136 2c0d      perPage=16,.
-00006090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000060a0: 2020 2020 2020 2020 6175 746f 4a75 6d70          autoJump
-000060b0: 546f 546f 704f 6e50 6167 6572 4368 616e  ToTopOnPagerChan
-000060c0: 6765 3d54 7275 652c 0d0a 2020 2020 2020  ge=True,..      
-000060d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060e0: 2070 6c61 6365 686f 6c64 6572 3d27 e69a   placeholder='..
-000060f0: 82e6 97a0 e5a4 a7e5 ada6 e4b9 a0e7 94a8  ................
-00006100: e688 b727 2c0d 0a20 2020 2020 2020 2020  ...',..         
-00006110: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00006120: 6f74 6572 546f 6f6c 6261 723d 5b27 7377  oterToolbar=['sw
-00006130: 6974 6368 2d70 6572 2d70 6167 6527 2c20  itch-per-page', 
-00006140: 2770 6167 696e 6174 696f 6e27 5d2c 0d0a  'pagination'],..
-00006150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006160: 2020 2020 2020 2063 6f6c 756d 6e73 436f         columnsCo
-00006170: 756e 743d 342c 0d0a 2020 2020 2020 2020  unt=4,..        
-00006180: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00006190: 6172 643d 6361 7264 290d 0a0d 0a22 2222  ard=card)...."""
-000061a0: e6b9 96e5 8c97 e6b7 bbe5 8aa0 e688 90e5  ................
-000061b0: 9198 e99d a2e6 9dbf 2222 220d 0a68 7562  ........"""..hub
-000061c0: 6569 5f74 6162 6c65 203d 2046 6f72 6d28  ei_table = Form(
-000061d0: 0d0a 2020 2020 7469 746c 653d 22e6 b7bb  ..    title="...
-000061e0: e58a a0e9 9d92 e698 a5e6 b996 e58c 97e7  ................
-000061f0: 94a8 e688 b722 2c0d 0a20 2020 2073 7562  .....",..    sub
-00006200: 6d69 7454 6578 743d 22e6 b7bb e58a a022  mitText="......"
-00006210: 2c0d 0a20 2020 206d 6f64 653d 4469 7370  ,..    mode=Disp
-00006220: 6c61 794d 6f64 6545 6e75 6d2e 686f 7269  layModeEnum.hori
-00006230: 7a6f 6e74 616c 2c0d 0a20 2020 2061 7069  zontal,..    api
-00006240: 3d22 706f 7374 3a2f 5465 656e 5374 7564  ="post:/TeenStud
-00006250: 792f 6170 692f 6164 6422 2c0d 0a20 2020  y/api/add",..   
-00006260: 2072 6573 6574 4166 7465 7253 7562 6d69   resetAfterSubmi
-00006270: 743d 5472 7565 2c0d 0a20 2020 2062 6f64  t=True,..    bod
-00006280: 793d 5b0d 0a20 2020 2020 2020 2053 656c  y=[..        Sel
-00006290: 6563 7428 0d0a 2020 2020 2020 2020 2020  ect(..          
-000062a0: 2020 6c61 6265 6c3d 22e7 bea4 e881 8a22    label="......"
-000062b0: 2c0d 0a20 2020 2020 2020 2020 2020 206e  ,..            n
-000062c0: 616d 653d 2267 726f 7570 5f69 6422 2c0d  ame="group_id",.
-000062d0: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-000062e0: 6372 6970 7469 6f6e 3d22 e99c 80e8 a681  cription="......
-000062f0: e6b7 bbe5 8aa0 e79a 84e7 bea4 e7bb 8422  ..............."
-00006300: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
-00006310: 6865 636b 416c 6c3d 4661 6c73 652c 0d0a  heckAll=False,..
-00006320: 2020 2020 2020 2020 2020 2020 736f 7572              sour
-00006330: 6365 3d22 6765 743a 2f54 6565 6e53 7475  ce="get:/TeenStu
-00006340: 6479 2f61 7069 2f67 6574 5f67 726f 7570  dy/api/get_group
-00006350: 5f6c 6973 7422 2c0d 0a20 2020 2020 2020  _list",..       
-00006360: 2020 2020 2076 616c 7565 3d27 272c 0d0a       value='',..
-00006370: 2020 2020 2020 2020 2020 2020 6d75 6c74              mult
-00006380: 6970 6c65 3d46 616c 7365 2c0d 0a20 2020  iple=False,..   
-00006390: 2020 2020 2020 2020 2072 6571 7569 7265           require
-000063a0: 643d 5472 7565 2c0d 0a20 2020 2020 2020  d=True,..       
-000063b0: 2020 2020 2073 6561 7263 6861 626c 653d       searchable=
-000063c0: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
-000063d0: 2020 206a 6f69 6e56 616c 7565 733d 4661     joinValues=Fa
-000063e0: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
-000063f0: 2020 6578 7472 6163 7456 616c 7565 3d54    extractValue=T
-00006400: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-00006410: 2020 7374 6174 6973 7469 6373 3d54 7275    statistics=Tru
-00006420: 652c 0d0a 2020 2020 2020 2020 292c 0d0a  e,..        ),..
-00006430: 2020 2020 2020 2020 5365 6c65 6374 280d          Select(.
-00006440: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-00006450: 656c 3d22 e794 a8e6 88b7 4944 222c 0d0a  el="......ID",..
-00006460: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00006470: 3d22 7573 6572 5f69 6422 2c0d 0a20 2020  ="user_id",..   
-00006480: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-00006490: 7469 6f6e 3d22 e99c 80e8 a681 e6b7 bbe5  tion="..........
-000064a0: 8aa0 e79a 84e7 94a8 e688 b749 4422 2c0d  ...........ID",.
-000064b0: 0a20 2020 2020 2020 2020 2020 2063 6865  .            che
-000064c0: 636b 416c 6c3d 4661 6c73 652c 0d0a 2020  ckAll=False,..  
-000064d0: 2020 2020 2020 2020 2020 736f 7572 6365            source
-000064e0: 3d22 6765 743a 2f54 6565 6e53 7475 6479  ="get:/TeenStudy
-000064f0: 2f61 7069 2f67 6574 5f6d 656d 6265 725f  /api/get_member_
-00006500: 6c69 7374 3f67 726f 7570 5f69 643d 247b  list?group_id=${
-00006510: 6772 6f75 705f 6964 7d22 2c0d 0a20 2020  group_id}",..   
-00006520: 2020 2020 2020 2020 2076 616c 7565 3d27           value='
-00006530: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00006540: 6d75 6c74 6970 6c65 3d46 616c 7365 2c0d  multiple=False,.
-00006550: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-00006560: 7569 7265 643d 5472 7565 2c0d 0a20 2020  uired=True,..   
-00006570: 2020 2020 2020 2020 2073 6561 7263 6861           searcha
-00006580: 626c 653d 5472 7565 2c0d 0a20 2020 2020  ble=True,..     
-00006590: 2020 2020 2020 206a 6f69 6e56 616c 7565         joinValue
-000065a0: 733d 4661 6c73 652c 0d0a 2020 2020 2020  s=False,..      
-000065b0: 2020 2020 2020 6578 7472 6163 7456 616c        extractVal
-000065c0: 7565 3d54 7275 652c 0d0a 2020 2020 2020  ue=True,..      
-000065d0: 2020 2020 2020 7374 6174 6973 7469 6373        statistics
-000065e0: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
-000065f0: 2020 2020 6869 6464 656e 4f6e 3d22 247b      hiddenOn="${
-00006600: 6772 6f75 705f 6964 3d3d 2727 3f74 7275  group_id==''?tru
-00006610: 653a 6661 6c73 657d 220d 0a20 2020 2020  e:false}"..     
-00006620: 2020 2029 2c0d 0a20 2020 2020 2020 2049     ),..        I
-00006630: 6e70 7574 5465 7874 280d 0a20 2020 2020  nputText(..     
-00006640: 2020 2020 2020 206c 6162 656c 3d22 e59c         label="..
-00006650: b0e5 8cba 222c 0d0a 2020 2020 2020 2020  ....",..        
-00006660: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
-00006670: 22e6 8980 e5a4 84e7 9c81 e4bb bd22 2c0d  "............",.
-00006680: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
-00006690: 653d 2261 7265 6122 2c0d 0a20 2020 2020  e="area",..     
-000066a0: 2020 2020 2020 2076 616c 7565 3d22 e6b9         value="..
-000066b0: 96e5 8c97 222c 0d0a 2020 2020 2020 2020  ....",..        
-000066c0: 2020 2020 6469 7361 626c 6564 3d54 7275      disabled=Tru
-000066d0: 650d 0a20 2020 2020 2020 2029 2c0d 0a20  e..        ),.. 
-000066e0: 2020 2020 2020 2049 6e70 7574 5465 7874         InputText
-000066f0: 280d 0a20 2020 2020 2020 2020 2020 206c  (..            l
-00006700: 6162 656c 3d22 e799 bbe5 bd95 e5af 86e7  abel="..........
-00006710: a081 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
-00006720: 2020 7479 7065 3d27 696e 7075 742d 7061    type='input-pa
-00006730: 7373 776f 7264 272c 0d0a 2020 2020 2020  ssword',..      
-00006740: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-00006750: 6e3d 22e5 8faf e4b8 8de5 a1ab efbc 8ce9  n=".............
-00006760: bb98 e8ae a4e4 b8ba e794 a8e6 88b7 4944  ..............ID
-00006770: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00006780: 6e61 6d65 3d22 7061 7373 776f 7264 222c  name="password",
-00006790: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-000067a0: 6c69 6e65 3d46 616c 7365 2c0d 0a20 2020  line=False,..   
-000067b0: 2020 2020 2020 2020 2072 6571 7569 7265           require
-000067c0: 643d 4661 6c73 652c 0d0a 2020 2020 2020  d=False,..      
-000067d0: 2020 2020 2020 7661 6c75 653d 2222 2c0d        value="",.
-000067e0: 0a20 2020 2020 2020 2020 2020 2063 6c65  .            cle
-000067f0: 6172 6162 6c65 3d54 7275 652c 0d0a 2020  arable=True,..  
-00006800: 2020 2020 2020 2020 2020 6d61 784c 656e            maxLen
-00006810: 6774 683d 3136 0d0a 2020 2020 2020 2020  gth=16..        
-00006820: 292c 0d0a 2020 2020 2020 2020 496e 7075  ),..        Inpu
-00006830: 7454 6578 7428 0d0a 2020 2020 2020 2020  tText(..        
-00006840: 2020 2020 6c61 6265 6c3d 22e5 a793 e590      label=".....
-00006850: 8d22 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
-00006860: 2064 6573 6372 6970 7469 6f6e 3d22 e5af   description="..
-00006870: b9e5 ba94 e99d 92e6 98a5 e6b9 96e5 8c97  ................
-00006880: e4b8 aae4 baba e4bf a1e6 81af e9a1 b520  ............... 
-00006890: e682 a8e7 9a84 e5a7 93e5 908d 222c 0d0a  ............",..
-000068a0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-000068b0: 3d22 6e61 6d65 222c 0d0a 2020 2020 2020  ="name",..      
-000068c0: 2020 2020 2020 696e 6c69 6e65 3d46 616c        inline=Fal
-000068d0: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-000068e0: 2072 6571 7569 7265 643d 5472 7565 2c0d   required=True,.
-000068f0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-00006900: 7565 3d22 222c 0d0a 2020 2020 2020 2020  ue="",..        
-00006910: 2020 2020 636c 6561 7261 626c 653d 5472      clearable=Tr
-00006920: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-00006930: 206d 6178 4c65 6e67 7468 3d38 0d0a 2020   maxLength=8..  
-00006940: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
-00006950: 2020 496e 7075 7454 6578 7428 0d0a 2020    InputText(..  
-00006960: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
-00006970: 22e7 94a8 e688 b7e7 bc96 e58f b722 2c0d  "............",.
-00006980: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-00006990: 6372 6970 7469 6f6e 3d22 e5af b9e5 ba94  cription="......
-000069a0: e99d 92e6 98a5 e6b9 96e5 8c97 e4b8 aae4  ................
-000069b0: baba e4bf a1e6 81af e9a1 b520 e794 a8e6  ........... ....
-000069c0: 88b7 e7bc 96e5 8fb7 222c 0d0a 2020 2020  ........",..    
-000069d0: 2020 2020 2020 2020 6e61 6d65 3d22 6478          name="dx
-000069e0: 785f 6964 222c 0d0a 2020 2020 2020 2020  x_id",..        
-000069f0: 2020 2020 696e 6c69 6e65 3d46 616c 7365      inline=False
-00006a00: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
-00006a10: 6571 7569 7265 643d 5472 7565 2c0d 0a20  equired=True,.. 
-00006a20: 2020 2020 2020 2020 2020 2076 616c 7565             value
-00006a30: 3d22 222c 0d0a 2020 2020 2020 2020 2020  ="",..          
-00006a40: 2020 636c 6561 7261 626c 653d 5472 7565    clearable=True
-00006a50: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
-00006a60: 6178 4c65 6e67 7468 3d39 0d0a 2020 2020  axLength=9..    
-00006a70: 2020 2020 292c 0d0a 2020 2020 2020 2020      ),..        
-00006a80: 496e 7075 7454 6578 7428 0d0a 2020 2020  InputText(..    
-00006a90: 2020 2020 2020 2020 6c61 6265 6c3d 22e5          label=".
-00006aa0: ada6 e6a0 a122 2c0d 0a20 2020 2020 2020  .....",..       
-00006ab0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-00006ac0: 3d22 e5af b9e5 ba94 e99d 92e6 98a5 e6b9  ="..............
-00006ad0: 96e5 8c97 e5a1 abe5 8699 e4bf a1e6 81af  ................
-00006ae0: e9a1 b520 e9ab 98e6 a0a1 222c 0d0a 2020  ... ......",..  
-00006af0: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
-00006b00: 756e 6976 6572 7369 7479 222c 0d0a 2020  university",..  
-00006b10: 2020 2020 2020 2020 2020 696e 6c69 6e65            inline
-00006b20: 3d46 616c 7365 2c0d 0a20 2020 2020 2020  =False,..       
-00006b30: 2020 2020 2072 6571 7569 7265 643d 5472       required=Tr
-00006b40: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-00006b50: 2076 616c 7565 3d22 222c 0d0a 2020 2020   value="",..    
-00006b60: 2020 2020 2020 2020 636c 6561 7261 626c          clearabl
-00006b70: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
-00006b80: 2020 2020 206d 6178 4c65 6e67 7468 3d32       maxLength=2
-00006b90: 340d 0a20 2020 2020 2020 2029 2c0d 0a20  4..        ),.. 
-00006ba0: 2020 2020 2020 2049 6e70 7574 5465 7874         InputText
-00006bb0: 280d 0a20 2020 2020 2020 2020 2020 206c  (..            l
-00006bc0: 6162 656c 3d22 e5ad a6e9 99a2 222c 0d0a  abel="......",..
-00006bd0: 2020 2020 2020 2020 2020 2020 6465 7363              desc
-00006be0: 7269 7074 696f 6e3d 22e5 afb9 e5ba 94e9  ription=".......
-00006bf0: 9d92 e698 a5e6 b996 e58c 97e5 a1ab e586  ................
-00006c00: 99e4 bfa1 e681 afe9 a1b5 20e9 99a2 e7b3  .......... .....
-00006c10: bb22 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
-00006c20: 206e 616d 653d 2263 6f6c 6c65 6765 222c   name="college",
-00006c30: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-00006c40: 6c69 6e65 3d46 616c 7365 2c0d 0a20 2020  line=False,..   
-00006c50: 2020 2020 2020 2020 2072 6571 7569 7265           require
-00006c60: 643d 5472 7565 2c0d 0a20 2020 2020 2020  d=True,..       
-00006c70: 2020 2020 2076 616c 7565 3d22 222c 0d0a       value="",..
-00006c80: 2020 2020 2020 2020 2020 2020 636c 6561              clea
-00006c90: 7261 626c 653d 5472 7565 2c0d 0a20 2020  rable=True,..   
-00006ca0: 2020 2020 2020 2020 206d 6178 4c65 6e67           maxLeng
-00006cb0: 7468 3d33 320d 0a20 2020 2020 2020 2029  th=32..        )
-00006cc0: 2c0d 0a20 2020 2020 2020 2049 6e70 7574  ,..        Input
-00006cd0: 5465 7874 280d 0a20 2020 2020 2020 2020  Text(..         
-00006ce0: 2020 206c 6162 656c 3d22 e59b a2e6 94af     label="......
-00006cf0: e983 a822 2c0d 0a20 2020 2020 2020 2020  ...",..         
-00006d00: 2020 2064 6573 6372 6970 7469 6f6e 3d22     description="
-00006d10: e5af b9e5 ba94 e99d 92e6 98a5 e6b9 96e5  ................
-00006d20: 8c97 e5a1 abe5 8699 e4bf a1e6 81af e9a1  ................
-00006d30: b520 e980 89e6 8ba9 e7bb 84e7 bb87 222c  . ............",
-00006d40: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
-00006d50: 6d65 3d22 6f72 6761 6e69 7a61 7469 6f6e  me="organization
-00006d60: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00006d70: 696e 6c69 6e65 3d46 616c 7365 2c0d 0a20  inline=False,.. 
-00006d80: 2020 2020 2020 2020 2020 2072 6571 7569             requi
-00006d90: 7265 643d 4661 6c73 652c 0d0a 2020 2020  red=False,..    
-00006da0: 2020 2020 2020 2020 7661 6c75 653d 2222          value=""
-00006db0: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
-00006dc0: 6c65 6172 6162 6c65 3d54 7275 652c 0d0a  learable=True,..
-00006dd0: 2020 2020 2020 2020 2020 2020 6d61 784c              maxL
-00006de0: 656e 6774 683d 3332 0d0a 2020 2020 2020  ength=32..      
-00006df0: 2020 290d 0a0d 0a20 2020 205d 0d0a 290d    )....    ]..).
-00006e00: 0a22 2222 e6b1 9fe8 a5bf e6b7 bbe5 8aa0  ."""............
-00006e10: e688 90e5 9198 e99d a2e6 9dbf 2222 220d  ............""".
-00006e20: 0a6a 6961 6e67 7869 5f74 6162 6c65 203d  .jiangxi_table =
-00006e30: 2046 6f72 6d28 0d0a 2020 2020 7469 746c   Form(..    titl
-00006e40: 653d 22e6 b7bb e58a a0e6 b19f e8a5 bfe5  e=".............
-00006e50: 85b1 e99d 92e5 9ba2 e794 a8e6 88b7 222c  ..............",
-00006e60: 0d0a 2020 2020 7375 626d 6974 5465 7874  ..    submitText
-00006e70: 3d22 e6b7 bbe5 8aa0 222c 0d0a 2020 2020  ="......",..    
-00006e80: 6d6f 6465 3d44 6973 706c 6179 4d6f 6465  mode=DisplayMode
-00006e90: 456e 756d 2e68 6f72 697a 6f6e 7461 6c2c  Enum.horizontal,
-00006ea0: 0d0a 2020 2020 6170 693d 2270 6f73 743a  ..    api="post:
-00006eb0: 2f54 6565 6e53 7475 6479 2f61 7069 2f61  /TeenStudy/api/a
-00006ec0: 6464 222c 0d0a 2020 2020 7265 7365 7441  dd",..    resetA
-00006ed0: 6674 6572 5375 626d 6974 3d54 7275 652c  fterSubmit=True,
-00006ee0: 0d0a 2020 2020 626f 6479 3d5b 0d0a 2020  ..    body=[..  
-00006ef0: 2020 2020 2020 5365 6c65 6374 280d 0a20        Select(.. 
-00006f00: 2020 2020 2020 2020 2020 206c 6162 656c             label
-00006f10: 3d22 e7be a4e8 818a 222c 0d0a 2020 2020  ="......",..    
-00006f20: 2020 2020 2020 2020 6e61 6d65 3d22 6772          name="gr
-00006f30: 6f75 705f 6964 222c 0d0a 2020 2020 2020  oup_id",..      
-00006f40: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-00006f50: 6e3d 22e9 9c80 e8a6 81e6 b7bb e58a a0e7  n=".............
-00006f60: 9a84 e7be a4e7 bb84 222c 0d0a 2020 2020  ........",..    
-00006f70: 2020 2020 2020 2020 6368 6563 6b41 6c6c          checkAll
-00006f80: 3d46 616c 7365 2c0d 0a20 2020 2020 2020  =False,..       
-00006f90: 2020 2020 2073 6f75 7263 653d 2267 6574       source="get
-00006fa0: 3a2f 5465 656e 5374 7564 792f 6170 692f  :/TeenStudy/api/
-00006fb0: 6765 745f 6772 6f75 705f 6c69 7374 222c  get_group_list",
-00006fc0: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-00006fd0: 6c75 653d 2727 2c0d 0a20 2020 2020 2020  lue='',..       
-00006fe0: 2020 2020 206d 756c 7469 706c 653d 4661       multiple=Fa
-00006ff0: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
-00007000: 2020 7265 7175 6972 6564 3d54 7275 652c    required=True,
-00007010: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00007020: 6172 6368 6162 6c65 3d54 7275 652c 0d0a  archable=True,..
-00007030: 2020 2020 2020 2020 2020 2020 6a6f 696e              join
-00007040: 5661 6c75 6573 3d46 616c 7365 2c0d 0a20  Values=False,.. 
-00007050: 2020 2020 2020 2020 2020 2065 7874 7261             extra
-00007060: 6374 5661 6c75 653d 5472 7565 2c0d 0a20  ctValue=True,.. 
-00007070: 2020 2020 2020 2020 2020 2073 7461 7469             stati
-00007080: 7374 6963 733d 5472 7565 2c0d 0a20 2020  stics=True,..   
-00007090: 2020 2020 2029 2c0d 0a20 2020 2020 2020       ),..       
-000070a0: 2053 656c 6563 7428 0d0a 2020 2020 2020   Select(..      
-000070b0: 2020 2020 2020 6c61 6265 6c3d 22e7 94a8        label="...
-000070c0: e688 b749 4422 2c0d 0a20 2020 2020 2020  ...ID",..       
-000070d0: 2020 2020 206e 616d 653d 2275 7365 725f       name="user_
-000070e0: 6964 222c 0d0a 2020 2020 2020 2020 2020  id",..          
-000070f0: 2020 6465 7363 7269 7074 696f 6e3d 22e9    description=".
-00007100: 9c80 e8a6 81e6 b7bb e58a a0e7 9a84 e794  ................
-00007110: a8e6 88b7 4944 222c 0d0a 2020 2020 2020  ....ID",..      
-00007120: 2020 2020 2020 6368 6563 6b41 6c6c 3d46        checkAll=F
-00007130: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
-00007140: 2020 2073 6f75 7263 653d 2267 6574 3a2f     source="get:/
-00007150: 5465 656e 5374 7564 792f 6170 692f 6765  TeenStudy/api/ge
-00007160: 745f 6d65 6d62 6572 5f6c 6973 743f 6772  t_member_list?gr
-00007170: 6f75 705f 6964 3d24 7b67 726f 7570 5f69  oup_id=${group_i
-00007180: 647d 222c 0d0a 2020 2020 2020 2020 2020  d}",..          
-00007190: 2020 7661 6c75 653d 2727 2c0d 0a20 2020    value='',..   
-000071a0: 2020 2020 2020 2020 206d 756c 7469 706c           multipl
-000071b0: 653d 4661 6c73 652c 0d0a 2020 2020 2020  e=False,..      
-000071c0: 2020 2020 2020 7265 7175 6972 6564 3d54        required=T
-000071d0: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-000071e0: 2020 7365 6172 6368 6162 6c65 3d54 7275    searchable=Tru
-000071f0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00007200: 6a6f 696e 5661 6c75 6573 3d46 616c 7365  joinValues=False
-00007210: 2c0d 0a20 2020 2020 2020 2020 2020 2065  ,..            e
-00007220: 7874 7261 6374 5661 6c75 653d 5472 7565  xtractValue=True
-00007230: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
-00007240: 7461 7469 7374 6963 733d 5472 7565 2c0d  tatistics=True,.
-00007250: 0a20 2020 2020 2020 2020 2020 2068 6964  .            hid
-00007260: 6465 6e4f 6e3d 2224 7b67 726f 7570 5f69  denOn="${group_i
-00007270: 643d 3d27 273f 7472 7565 3a66 616c 7365  d==''?true:false
-00007280: 7d22 0d0a 2020 2020 2020 2020 292c 0d0a  }"..        ),..
-00007290: 2020 2020 2020 2020 496e 7075 7454 6578          InputTex
-000072a0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
-000072b0: 6c61 6265 6c3d 22e5 9cb0 e58c ba22 2c0d  label="......",.
-000072c0: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-000072d0: 6372 6970 7469 6f6e 3d22 e689 80e5 a484  cription="......
-000072e0: e79c 81e4 bbbd 222c 0d0a 2020 2020 2020  ......",..      
-000072f0: 2020 2020 2020 6e61 6d65 3d22 6172 6561        name="area
-00007300: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00007310: 7661 6c75 653d 22e6 b19f e8a5 bf22 2c0d  value="......",.
-00007320: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-00007330: 6162 6c65 643d 5472 7565 0d0a 2020 2020  abled=True..    
-00007340: 2020 2020 292c 0d0a 2020 2020 2020 2020      ),..        
-00007350: 496e 7075 7454 6578 7428 0d0a 2020 2020  InputText(..    
-00007360: 2020 2020 2020 2020 6c61 6265 6c3d 22e7          label=".
-00007370: 94a8 e688 b7e7 bc96 e58f b722 2c0d 0a20  ...........",.. 
-00007380: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-00007390: 6970 7469 6f6e 3d22 e59b a2e7 bb84 e7bb  iption="........
-000073a0: 8749 44ef bc8c e697 a0e9 9c80 e5a1 abe5  .ID.............
-000073b0: 8699 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
-000073c0: 2020 6e61 6d65 3d22 6478 785f 6964 222c    name="dxx_id",
-000073d0: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-000073e0: 6c69 6e65 3d46 616c 7365 2c0d 0a20 2020  line=False,..   
-000073f0: 2020 2020 2020 2020 2072 6571 7569 7265           require
-00007400: 643d 5472 7565 2c0d 0a20 2020 2020 2020  d=True,..       
-00007410: 2020 2020 2076 616c 7565 3d22 247b 6f72       value="${or
-00007420: 6761 6e69 7a61 7469 6f6e 7d22 2c0d 0a20  ganization}",.. 
-00007430: 2020 2020 2020 2020 2020 2064 6973 6162             disab
-00007440: 6c65 643d 5472 7565 0d0a 2020 2020 2020  led=True..      
-00007450: 2020 292c 0d0a 2020 2020 2020 2020 5365    ),..        Se
-00007460: 7276 6963 6528 0d0a 2020 2020 2020 2020  rvice(..        
-00007470: 2020 2020 696e 7465 7276 616c 3d33 3030      interval=300
-00007480: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-00007490: 7369 7a65 3d22 6c67 222c 0d0a 2020 2020  size="lg",..    
-000074a0: 2020 2020 2020 2020 626f 6479 3d5b 0d0a          body=[..
-000074b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074c0: 5365 6c65 6374 280d 0a20 2020 2020 2020  Select(..       
-000074d0: 2020 2020 2020 2020 2020 2020 2074 7970               typ
-000074e0: 653d 2273 656c 6563 7422 2c0d 0a20 2020  e="select",..   
-000074f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007500: 206c 6162 656c 3d22 e5ad a6e6 a0a1 e590   label="........
-00007510: 8de7 a7b0 222c 0d0a 2020 2020 2020 2020  ....",..        
-00007520: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00007530: 3d22 756e 6976 6572 7369 7479 222c 0d0a  ="university",..
-00007540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007550: 2020 2020 7365 6172 6368 6162 6c65 3d54      searchable=T
-00007560: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-00007570: 2020 2020 2020 2020 2020 7265 7175 6972            requir
-00007580: 6564 3d54 7275 652c 0d0a 2020 2020 2020  ed=True,..      
-00007590: 2020 2020 2020 2020 2020 2020 2020 6f70                op
-000075a0: 7469 6f6e 733d 5b7b 276c 6162 656c 273a  tions=[{'label':
-000075b0: 2027 e58d 97e6 988c e5a4 a7e5 ada6 272c   '............',
-000075c0: 2027 7661 6c75 6527 3a20 27e5 8d97 e698   'value': '.....
-000075d0: 8ce5 a4a7 e5ad a627 7d2c 0d0a 2020 2020  .......'},..    
-000075e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075f0: 2020 2020 2020 2020 207b 276c 6162 656c           {'label
-00007600: 273a 2027 e6b1 9fe8 a5bf e5b8 88e8 8c83  ': '............
-00007610: e5a4 a7e5 ada6 272c 2027 7661 6c75 6527  ......', 'value'
-00007620: 3a20 27e6 b19f e8a5 bfe5 b888 e88c 83e5  : '.............
-00007630: a4a7 e5ad a627 7d2c 0d0a 2020 2020 2020  .....'},..      
-00007640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007650: 2020 2020 2020 207b 276c 6162 656c 273a         {'label':
-00007660: 2027 e6b1 9fe8 a5bf e586 9ce4 b89a e5a4   '..............
-00007670: a7e5 ada6 272c 2027 7661 6c75 6527 3a20  ....', 'value': 
-00007680: 27e6 b19f e8a5 bfe5 869c e4b8 9ae5 a4a7  '...............
-00007690: e5ad a627 7d2c 0d0a 2020 2020 2020 2020  ...'},..        
-000076a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076b0: 2020 2020 207b 276c 6162 656c 273a 2027       {'label': '
-000076c0: e6b1 9fe8 a5bf e8b4 a2e7 bb8f e5a4 a7e5  ................
-000076d0: ada6 272c 2027 7661 6c75 6527 3a20 27e6  ..', 'value': '.
-000076e0: b19f e8a5 bfe8 b4a2 e7bb 8fe5 a4a7 e5ad  ................
-000076f0: a627 7d2c 0d0a 2020 2020 2020 2020 2020  .'},..          
-00007700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007710: 2020 207b 276c 6162 656c 273a 2027 e58d     {'label': '..
-00007720: 8ee4 b89c e4ba a4e9 809a e5a4 a7e5 ada6  ................
-00007730: 272c 2027 7661 6c75 6527 3a20 27e5 8d8e  ', 'value': '...
-00007740: e4b8 9ce4 baa4 e980 9ae5 a4a7 e5ad a627  ...............'
-00007750: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-00007760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007770: 207b 276c 6162 656c 273a 2027 e4b8 9ce5   {'label': '....
-00007780: 8d8e e790 86e5 b7a5 e5a4 a7e5 ada6 272c  ..............',
-00007790: 2027 7661 6c75 6527 3a20 27e4 b89c e58d   'value': '.....
-000077a0: 8ee7 9086 e5b7 a5e5 a4a7 e5ad a627 7d2c  .............'},
-000077b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000077c0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000077d0: 276c 6162 656c 273a 2027 e6b1 9fe8 a5bf  'label': '......
-000077e0: e790 86e5 b7a5 e5a4 a7e5 ada6 272c 2027  ............', '
-000077f0: 7661 6c75 6527 3a20 27e6 b19f e8a5 bfe7  value': '.......
-00007800: 9086 e5b7 a5e5 a4a7 e5ad a627 7d2c 0d0a  ...........'},..
-00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007820: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
-00007830: 6162 656c 273a 2027 e58d 97e6 988c e888  abel': '........
-00007840: aae7 a9ba e5a4 a7e5 ada6 272c 2027 7661  ..........', 'va
-00007850: 6c75 6527 3a20 27e5 8d97 e698 8ce8 88aa  lue': '.........
-00007860: e7a9 bae5 a4a7 e5ad a627 7d2c 0d0a 2020  .........'},..  
-00007870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007880: 2020 2020 2020 2020 2020 207b 276c 6162             {'lab
-00007890: 656c 273a 2027 e4ba 95e5 8688 e5b1 b1e5  el': '..........
-000078a0: a4a7 e5ad a627 2c20 2776 616c 7565 273a  .....', 'value':
-000078b0: 2027 e4ba 95e5 8688 e5b1 b1e5 a4a7 e5ad   '..............
-000078c0: a627 7d2c 0d0a 2020 2020 2020 2020 2020  .'},..          
-000078d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078e0: 2020 207b 276c 6162 656c 273a 2027 e6b1     {'label': '..
-000078f0: 9fe8 a5bf e7a7 91e6 8a80 e5b8 88e8 8c83  ................
-00007900: e5a4 a7e5 ada6 272c 2027 7661 6c75 6527  ......', 'value'
-00007910: 3a20 27e6 b19f e8a5 bfe7 a791 e68a 80e5  : '.............
-00007920: b888 e88c 83e5 a4a7 e5ad a627 7d2c 0d0a  ...........'},..
-00007930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007940: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
-00007950: 6162 656c 273a 2027 e6b1 9fe8 a5bf e4b8  abel': '........
-00007960: ade5 8cbb e88d afe5 a4a7 e5ad a627 2c20  .............', 
-00007970: 2776 616c 7565 273a 2027 e6b1 9fe8 a5bf  'value': '......
-00007980: e4b8 ade5 8cbb e88d afe5 a4a7 e5ad a627  ...............'
-00007990: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-000079a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079b0: 207b 276c 6162 656c 273a 2027 e699 afe5   {'label': '....
-000079c0: beb7 e995 87e9 99b6 e793 b7e5 a4a7 e5ad  ................
-000079d0: a627 2c20 2776 616c 7565 273a 2027 e699  .', 'value': '..
-000079e0: afe5 beb7 e995 87e9 99b6 e793 b7e5 a4a7  ................
-000079f0: e5ad a627 7d2c 0d0a 2020 2020 2020 2020  ...'},..        
-00007a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a10: 2020 2020 207b 276c 6162 656c 273a 2027       {'label': '
-00007a20: e8b5 a3e5 8d97 e5b8 88e8 8c83 e5a4 a7e5  ................
-00007a30: ada6 272c 2027 7661 6c75 6527 3a20 27e8  ..', 'value': '.
-00007a40: b5a3 e58d 97e5 b888 e88c 83e5 a4a7 e5ad  ................
-00007a50: a627 7d2c 0d0a 2020 2020 2020 2020 2020  .'},..          
-00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a70: 2020 207b 276c 6162 656c 273a 2027 e8b5     {'label': '..
-00007a80: a3e5 8d97 e58c bbe5 ada6 e999 a227 2c20  .............', 
-00007a90: 2776 616c 7565 273a 2027 e8b5 a3e5 8d97  'value': '......
-00007aa0: e58c bbe5 ada6 e999 a227 7d2c 0d0a 2020  .........'},..  
-00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ac0: 2020 2020 2020 2020 2020 207b 276c 6162             {'lab
-00007ad0: 656c 273a 2027 e58d 97e6 988c e5b7 a5e7  el': '..........
-00007ae0: a88b e5ad a6e9 99a2 272c 2027 7661 6c75  ........', 'valu
-00007af0: 6527 3a20 27e5 8d97 e698 8ce5 b7a5 e7a8  e': '...........
-00007b00: 8be5 ada6 e999 a227 7d2c 0d0a 2020 2020  .......'},..    
-00007b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b20: 2020 2020 2020 2020 207b 276c 6162 656c           {'label
-00007b30: 273a 2027 e6b1 9fe8 a5bf e7a7 91e6 8a80  ': '............
-00007b40: e5ad a6e9 99a2 272c 2027 7661 6c75 6527  ......', 'value'
-00007b50: 3a20 27e6 b19f e8a5 bfe7 a791 e68a 80e5  : '.............
-00007b60: ada6 e999 a227 7d2c 0d0a 2020 2020 2020  .....'},..      
-00007b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b80: 2020 2020 2020 207b 276c 6162 656c 273a         {'label':
-00007b90: 2027 e58d 97e6 988c e790 86e5 b7a5 e5ad   '..............
-00007ba0: a6e9 99a2 272c 2027 7661 6c75 6527 3a20  ....', 'value': 
-00007bb0: 27e5 8d97 e698 8ce7 9086 e5b7 a5e5 ada6  '...............
-00007bc0: e999 a227 7d2c 0d0a 2020 2020 2020 2020  ...'},..        
-00007bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007be0: 2020 2020 207b 276c 6162 656c 273a 2027       {'label': '
-00007bf0: e6b1 9fe8 a5bf e5ba 94e7 94a8 e7a7 91e6  ................
-00007c00: 8a80 e5ad a6e9 99a2 272c 2027 7661 6c75  ........', 'valu
-00007c10: 6527 3a20 27e6 b19f e8a5 bfe5 ba94 e794  e': '...........
-00007c20: a8e7 a791 e68a 80e5 ada6 e999 a227 7d2c  .............'},
-00007c30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007c40: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00007c50: 276c 6162 656c 273a 2027 e58d 97e6 988c  'label': '......
-00007c60: e5b8 88e8 8c83 e5ad a6e9 99a2 272c 2027  ............', '
-00007c70: 7661 6c75 6527 3a20 27e5 8d97 e698 8ce5  value': '.......
-00007c80: b888 e88c 83e5 ada6 e999 a227 7d2c 0d0a  ...........'},..
-00007c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ca0: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
-00007cb0: 6162 656c 273a 2027 e5ae 9ce6 98a5 e5ad  abel': '........
-00007cc0: a6e9 99a2 272c 2027 7661 6c75 6527 3a20  ....', 'value': 
-00007cd0: 27e5 ae9c e698 a5e5 ada6 e999 a227 7d2c  '............'},
-00007ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007cf0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00007d00: 276c 6162 656c 273a 2027 e4b8 8ae9 a5b6  'label': '......
-00007d10: e5b8 88e8 8c83 e5ad a6e9 99a2 272c 2027  ............', '
-00007d20: 7661 6c75 6527 3a20 27e4 b88a e9a5 b6e5  value': '.......
-00007d30: b888 e88c 83e5 ada6 e999 a227 7d2c 0d0a  ...........'},..
-00007d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d50: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
-00007d60: 6162 656c 273a 2027 e4b9 9de6 b19f e5ad  abel': '........
-00007d70: a6e9 99a2 272c 2027 7661 6c75 6527 3a20  ....', 'value': 
-00007d80: 27e4 b99d e6b1 9fe5 ada6 e999 a227 7d2c  '............'},
-00007d90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007da0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00007db0: 276c 6162 656c 273a 2027 e58d 97e6 988c  'label': '......
-00007dc0: e5a4 a7e5 ada6 e7a7 91e5 ada6 e68a 80e6  ................
-00007dd0: 9caf e5ad a6e9 99a2 272c 2027 7661 6c75  ........', 'valu
-00007de0: 6527 3a20 27e5 8d97 e698 8ce5 a4a7 e5ad  e': '...........
-00007df0: a6e7 a791 e5ad a6e6 8a80 e69c afe5 ada6  ................
-00007e00: e999 a227 7d2c 0d0a 2020 2020 2020 2020  ...'},..        
-00007e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e20: 2020 2020 207b 276c 6162 656c 273a 2027       {'label': '
-00007e30: e6b1 9fe8 a5bf e5bc 80e6 94be e5a4 a7e5  ................
-00007e40: ada6 e4ba bae6 b091 e6ad a6e8 a385 e5ad  ................
-00007e50: a6e9 99a2 272c 2027 7661 6c75 6527 3a20  ....', 'value': 
-00007e60: 27e6 b19f e8a5 bfe5 bc80 e694 bee5 a4a7  '...............
-00007e70: e5ad a6e4 baba e6b0 91e6 ada6 e8a3 85e5  ................
-00007e80: ada6 e999 a227 7d2c 0d0a 2020 2020 2020  .....'},..      
-00007e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ea0: 2020 2020 2020 207b 276c 6162 656c 273a         {'label':
-00007eb0: 2027 e58d 97e6 988c e5a4 a7e5 ada6 e585   '..............
-00007ec0: b1e9 9d92 e5ad a6e9 99a2 272c 2027 7661  ..........', 'va
-00007ed0: 6c75 6527 3a20 27e5 8d97 e698 8ce5 a4a7  lue': '.........
-00007ee0: e5ad a6e5 85b1 e99d 92e5 ada6 e999 a227  ...............'
-00007ef0: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f10: 207b 276c 6162 656c 273a 2027 e6b1 9fe8   {'label': '....
-00007f20: a5bf e5b8 88e8 8c83 e5a4 a7e5 ada6 e7a7  ................
-00007f30: 91e5 ada6 e68a 80e6 9caf e5ad a6e9 99a2  ................
-00007f40: 272c 2027 7661 6c75 6527 3a20 27e6 b19f  ', 'value': '...
-00007f50: e8a5 bfe5 b888 e88c 83e5 a4a7 e5ad a6e7  ................
-00007f60: a791 e5ad a6e6 8a80 e69c afe5 ada6 e999  ................
-00007f70: a227 7d2c 0d0a 2020 2020 2020 2020 2020  .'},..          
-00007f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f90: 2020 207b 276c 6162 656c 273a 2027 e6b1     {'label': '..
-00007fa0: 9fe8 a5bf e586 9ce4 b89a e5a4 a7e5 ada6  ................
-00007fb0: e58d 97e6 988c e595 86e5 ada6 e999 a227  ...............'
-00007fc0: 2c20 2776 616c 7565 273a 2027 e6b1 9fe8  , 'value': '....
-00007fd0: a5bf e586 9ce4 b89a e5a4 a7e5 ada6 e58d  ................
-00007fe0: 97e6 988c e595 86e5 ada6 e999 a227 7d2c  .............'},
-00007ff0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008000: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00008010: 276c 6162 656c 273a 2027 e6b1 9fe8 a5bf  'label': '......
-00008020: e8b4 a2e7 bb8f e5a4 a7e5 ada6 e78e b0e4  ................
-00008030: bba3 e7bb 8fe6 b58e e7ae a1e7 9086 e5ad  ................
-00008040: a6e9 99a2 272c 2027 7661 6c75 6527 3a20  ....', 'value': 
-00008050: 27e6 b19f e8a5 bfe8 b4a2 e7bb 8fe5 a4a7  '...............
-00008060: e5ad a6e7 8eb0 e4bb a3e7 bb8f e6b5 8ee7  ................
-00008070: aea1 e790 86e5 ada6 e999 a227 7d2c 0d0a  ...........'},..
-00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008090: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
-000080a0: 6162 656c 273a 2027 e58d 97e6 988c e4ba  abel': '........
-000080b0: a4e9 809a e5ad a6e9 99a2 272c 2027 7661  ..........', 'va
-000080c0: 6c75 6527 3a20 27e5 8d97 e698 8ce4 baa4  lue': '.........
-000080d0: e980 9ae5 ada6 e999 a227 7d2c 0d0a 2020  .........'},..  
-000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080f0: 2020 2020 2020 2020 2020 207b 276c 6162             {'lab
-00008100: 656c 273a 2027 e8b5 a3e5 8d97 e7a7 91e6  el': '..........
-00008110: 8a80 272c 2027 7661 6c75 6527 3a20 27e8  ..', 'value': '.
-00008120: b5a3 e58d 97e7 a791 e68a 8027 7d2c 0d0a  ...........'},..
-00008130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008140: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
-00008150: 6162 656c 273a 2027 e8b5 a3e4 b89c e5ad  abel': '........
-00008160: a6e9 99a2 272c 2027 7661 6c75 6527 3a20  ....', 'value': 
-00008170: 27e8 b5a3 e4b8 9ce5 ada6 e999 a227 7d2c  '............'},
-00008180: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008190: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000081a0: 276c 6162 656c 273a 2027 e58d 97e6 988c  'label': '......
-000081b0: e888 aae7 a9ba e5a4 a7e5 ada6 e7a7 91e6  ................
-000081c0: 8a80 e5ad a6e9 99a2 272c 2027 7661 6c75  ........', 'valu
-000081d0: 6527 3a20 27e5 8d97 e698 8ce8 88aa e7a9  e': '...........
-000081e0: bae5 a4a7 e5ad a6e7 a791 e68a 80e5 ada6  ................
-000081f0: e999 a227 7d2c 0d0a 2020 2020 2020 2020  ...'},..        
-00008200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008210: 2020 2020 207b 276c 6162 656c 273a 2027       {'label': '
-00008220: e699 afe5 beb7 e995 87e9 99b6 e793 b7e5  ................
-00008230: a4a7 e5ad a6e7 a791 e68a 80e8 89ba e69c  ................
-00008240: afe5 ada6 e999 a227 2c20 2776 616c 7565  .......', 'value
-00008250: 273a 2027 e699 afe5 beb7 e995 87e9 99b6  ': '............
-00008260: e793 b7e5 a4a7 e5ad a6e7 a791 e68a 80e8  ................
-00008270: 89ba e69c afe5 ada6 e999 a227 7d2c 0d0a  ...........'},..
-00008280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008290: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
-000082a0: 6162 656c 273a 2027 e6b1 9fe8 a5bf e4b8  abel': '........
-000082b0: ade5 8cbb e88d afe5 a4a7 e5ad a6e7 a791  ................
-000082c0: e68a 80e5 ada6 e999 a227 2c20 2776 616c  .........', 'val
-000082d0: 7565 273a 2027 e6b1 9fe8 a5bf e4b8 ade5  ue': '..........
-000082e0: 8cbb e88d afe5 a4a7 e5ad a6e7 a791 e68a  ................
-000082f0: 80e5 ada6 e999 a227 7d2c 0d0a 2020 2020  .......'},..    
-00008300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008310: 2020 2020 2020 2020 207b 276c 6162 656c           {'label
-00008320: 273a 2027 e8b5 a3e5 8d97 e5b8 88e8 8c83  ': '............
-00008330: e5a4 a7e5 ada6 e7a7 91e6 8a80 e5ad a6e9  ................
-00008340: 99a2 272c 2027 7661 6c75 6527 3a20 27e8  ..', 'value': '.
-00008350: b5a3 e58d 97e5 b888 e88c 83e5 a4a7 e5ad  ................
-00008360: a6e7 a791 e68a 80e5 ada6 e999 a227 7d2c  .............'},
-00008370: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008380: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00008390: 276c 6162 656c 273a 2027 e6b1 9fe8 a5bf  'label': '......
-000083a0: e8ad a6e5 af9f e5ad a6e9 99a2 272c 2027  ............', '
-000083b0: 7661 6c75 6527 3a20 27e6 b19f e8a5 bfe8  value': '.......
-000083c0: ada6 e5af 9fe5 ada6 e999 a227 7d2c 0d0a  ...........'},..
-000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083e0: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
-000083f0: 6162 656c 273a 2027 e696 b0e4 bd99 e5ad  abel': '........
-00008400: a6e9 99a2 272c 2027 7661 6c75 6527 3a20  ....', 'value': 
-00008410: 27e6 96b0 e4bd 99e5 ada6 e999 a227 7d2c  '............'},
-00008420: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008430: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00008440: 276c 6162 656c 273a 2027 e58d 97e6 988c  'label': '......
-00008450: e5b7 a5e5 ada6 e999 a227 2c20 2776 616c  .........', 'val
-00008460: 7565 273a 2027 e58d 97e6 988c e5b7 a5e5  ue': '..........
-00008470: ada6 e999 a227 7d2c 0d0a 2020 2020 2020  .....'},..      
-00008480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008490: 2020 2020 2020 207b 276c 6162 656c 273a         {'label':
-000084a0: 2027 e6b1 9fe8 a5bf e69c 8de8 a385 e5ad   '..............
-000084b0: a6e9 99a2 272c 2027 7661 6c75 6527 3a20  ....', 'value': 
-000084c0: 27e6 b19f e8a5 bfe6 9c8d e8a3 85e5 ada6  '...............
-000084d0: e999 a227 7d2c 0d0a 2020 2020 2020 2020  ...'},..        
-000084e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084f0: 2020 2020 207b 276c 6162 656c 273a 2027       {'label': '
-00008500: e699 afe5 beb7 e995 87e5 ada6 e999 a227  ...............'
-00008510: 2c20 2776 616c 7565 273a 2027 e699 afe5  , 'value': '....
-00008520: beb7 e995 87e5 ada6 e999 a227 7d2c 0d0a  ...........'},..
-00008530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008540: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
-00008550: 6162 656c 273a 2027 e890 8de4 b9a1 e5ad  abel': '........
-00008560: a6e9 99a2 272c 2027 7661 6c75 6527 3a20  ....', 'value': 
-00008570: 27e8 908d e4b9 a1e5 ada6 e999 a227 7d2c  '............'},
-00008580: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008590: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000085a0: 276c 6162 656c 273a 2027 e6b1 9fe8 a5bf  'label': '......
-000085b0: e5b7 a5e7 a88b e5ad a6e9 99a2 272c 2027  ............', '
-000085c0: 7661 6c75 6527 3a20 27e6 b19f e8a5 bfe5  value': '.......
-000085d0: b7a5 e7a8 8be5 ada6 e999 a227 7d2c 0d0a  ...........'},..
-000085e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085f0: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
-00008600: 6162 656c 273a 2027 e8b1 abe7 aba0 e5b8  abel': '........
-00008610: 88e8 8c83 e5ad a6e9 99a2 272c 2027 7661  ..........', 'va
-00008620: 6c75 6527 3a20 27e8 b1ab e7ab a0e5 b888  lue': '.........
-00008630: e88c 83e5 ada6 e999 a227 7d2c 0d0a 2020  .........'},..  
-00008640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008650: 2020 2020 2020 2020 2020 207b 276c 6162             {'lab
-00008660: 656c 273a 2027 e58d 97e6 988c e881 8ce4  el': '..........
-00008670: b89a e5a4 a7e5 ada6 272c 2027 7661 6c75  ........', 'valu
-00008680: 6527 3a20 27e5 8d97 e698 8ce8 818c e4b8  e': '...........
-00008690: 9ae5 a4a7 e5ad a627 7d2c 0d0a 2020 2020  .......'},..    
-000086a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086b0: 2020 2020 2020 2020 207b 276c 6162 656c           {'label
-000086c0: 273a 2027 e6b1 9fe8 a5bf e8bd afe4 bbb6  ': '............
-000086d0: e881 8ce4 b89a e68a 80e6 9caf e5a4 a7e5  ................
-000086e0: ada6 272c 2027 7661 6c75 6527 3a20 27e6  ..', 'value': '.
-000086f0: b19f e8a5 bfe8 bdaf e4bb b6e8 818c e4b8  ................
-00008700: 9ae6 8a80 e69c afe5 a4a7 e5ad a627 7d2c  .............'},
-00008710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008720: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00008730: 276c 6162 656c 273a 2027 e699 afe5 beb7  'label': '......
-00008740: e995 87e8 89ba e69c afe8 818c e4b8 9ae5  ................
-00008750: a4a7 e5ad a627 2c20 2776 616c 7565 273a  .....', 'value':
-00008760: 2027 e699 afe5 beb7 e995 87e8 89ba e69c   '..............
-00008770: afe8 818c e4b8 9ae5 a4a7 e5ad a627 7d2c  .............'},
-00008780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008790: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000087a0: 276c 6162 656c 273a 2027 e58d 97e6 988c  'label': '......
-000087b0: e58c bb27 2c20 2776 616c 7565 273a 2027  ...', 'value': '
-000087c0: e58d 97e6 988c e58c bb27 7d2c 0d0a 2020  .........'},..  
-000087d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087e0: 2020 2020 2020 2020 2020 207b 276c 6162             {'lab
-000087f0: 656c 273a 2027 e58d 97e6 988c e5ba 94e7  el': '..........
-00008800: 94a8 e68a 80e6 9caf e5b8 88e8 8c83 e5ad  ................
-00008810: a6e9 99a2 272c 2027 7661 6c75 6527 3a20  ....', 'value': 
-00008820: 27e5 8d97 e698 8ce5 ba94 e794 a8e6 8a80  '...............
-00008830: e69c afe5 b888 e88c 83e5 ada6 e999 a227  ...............'
-00008840: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-00008850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008860: 207b 276c 6162 656c 273a 2027 e6b1 9fe8   {'label': '....
-00008870: a5bf e4b8 ade5 8cbb e88d afe9 ab98 e7ad  ................
-00008880: 89e4 b893 e7a7 91e5 ada6 e6a0 a127 2c20  .............', 
-00008890: 2776 616c 7565 273a 2027 e6b1 9fe8 a5bf  'value': '......
-000088a0: e4b8 ade5 8cbb e88d afe9 ab98 e7ad 89e4  ................
-000088b0: b893 e7a7 91e5 ada6 e6a0 a127 7d2c 0d0a  ...........'},..
-000088c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088d0: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
-000088e0: 6162 656c 273a 2027 e4b9 9de6 b19f e881  abel': '........
-000088f0: 8ce4 b89a e5a4 a7e5 ada6 272c 2027 7661  ..........', 'va
-00008900: 6c75 6527 3a20 27e4 b99d e6b1 9fe8 818c  lue': '.........
-00008910: e4b8 9ae5 a4a7 e5ad a627 7d2c 0d0a 2020  .........'},..  
-00008920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008930: 2020 2020 2020 2020 2020 207b 276c 6162             {'lab
-00008940: 656c 273a 2027 e4b9 9de6 b19f e881 8ce4  el': '..........
-00008950: b89a e68a 80e6 9caf e5ad a6e9 99a2 272c  ..............',
-00008960: 2027 7661 6c75 6527 3a20 27e4 b99d e6b1   'value': '.....
-00008970: 9fe8 818c e4b8 9ae6 8a80 e69c afe5 ada6  ................
-00008980: e999 a227 7d2c 0d0a 2020 2020 2020 2020  ...'},..        
-00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089a0: 2020 2020 207b 276c 6162 656c 273a 2027       {'label': '
-000089b0: e6b1 9fe8 a5bf e5b7 a5e4 b89a e881 8ce4  ................
-000089c0: b89a e68a 80e6 9caf e5ad a6e9 99a2 272c  ..............',
-000089d0: 2027 7661 6c75 6527 3a20 27e6 b19f e8a5   'value': '.....
-000089e0: bfe5 b7a5 e4b8 9ae8 818c e4b8 9ae6 8a80  ................
-000089f0: e69c afe5 ada6 e999 a227 7d2c 0d0a 2020  .........'},..  
-00008a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a10: 2020 2020 2020 2020 2020 207b 276c 6162             {'lab
-00008a20: 656c 273a 2027 e6b1 9fe8 a5bf e794 b5e5  el': '..........
-00008a30: 8a9b e881 8ce4 b89a e68a 80e6 9caf e5ad  ................
-00008a40: a6e9 99a2 272c 2027 7661 6c75 6527 3a20  ....', 'value': 
-00008a50: 27e6 b19f e8a5 bfe7 94b5 e58a 9be8 818c  '...............
-00008a60: e4b8 9ae6 8a80 e69c afe5 ada6 e999 a227  ...............'
-00008a70: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-00008a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a90: 207b 276c 6162 656c 273a 2027 e6b1 9fe8   {'label': '....
-00008aa0: a5bf e697 85e6 b8b8 e595 86e8 b4b8 e881  ................
-00008ab0: 8ce4 b89a e5ad a6e9 99a2 272c 2027 7661  ..........', 'va
-00008ac0: 6c75 6527 3a20 27e6 b19f e8a5 bfe6 9785  lue': '.........
-00008ad0: e6b8 b8e5 9586 e8b4 b8e8 818c e4b8 9ae5  ................
-00008ae0: ada6 e999 a227 7d2c 0d0a 2020 2020 2020  .....'},..      
-00008af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b00: 2020 2020 2020 207b 276c 6162 656c 273a         {'label':
-00008b10: 2027 e6b1 9fe8 a5bf e69c bae7 94b5 e881   '..............
-00008b20: 8ce4 b89a e68a 80e6 9caf e5ad a6e9 99a2  ................
-00008b30: 272c 2027 7661 6c75 6527 3a20 27e6 b19f  ', 'value': '...
-00008b40: e8a5 bfe6 9cba e794 b5e8 818c e4b8 9ae6  ................
-00008b50: 8a80 e69c afe5 ada6 e999 a227 7d2c 0d0a  ...........'},..
-00008b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b70: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
-00008b80: 6162 656c 273a 2027 e6b1 9fe8 a5bf e999  abel': '........
-00008b90: b6e7 93b7 e5b7 a5e8 89ba e7be 8ee6 9caf  ................
-00008ba0: e881 8ce4 b89a e68a 80e6 9caf e5ad a6e9  ................
-00008bb0: 99a2 272c 2027 7661 6c75 6527 3a20 27e6  ..', 'value': '.
-00008bc0: b19f e8a5 bfe9 99b6 e793 b7e5 b7a5 e889  ................
-00008bd0: bae7 be8e e69c afe8 818c e4b8 9ae6 8a80  ................
-00008be0: e69c afe5 ada6 e999 a227 7d2c 0d0a 2020  .........'},..  
-00008bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c00: 2020 2020 2020 2020 2020 207b 276c 6162             {'lab
-00008c10: 656c 273a 2027 e6b1 9fe8 a5bf e78e afe5  el': '..........
-00008c20: a283 e5b7 a5e7 a88b e881 8ce4 b89a e5ad  ................
-00008c30: a6e9 99a2 272c 2027 7661 6c75 6527 3a20  ....', 'value': 
-00008c40: 27e6 b19f e8a5 bfe7 8eaf e5a2 83e5 b7a5  '...............
-00008c50: e7a8 8be8 818c e4b8 9ae5 ada6 e999 a227  ...............'
-00008c60: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-00008c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c80: 207b 276c 6162 656c 273a 2027 e6b1 9fe8   {'label': '....
-00008c90: a5bf e4bf a1e6 81af e5ba 94e7 94a8 e881  ................
-00008ca0: 8ce4 b89a e68a 80e6 9caf e5ad a6e9 99a2  ................
-00008cb0: 272c 2027 7661 6c75 6527 3a20 27e6 b19f  ', 'value': '...
-00008cc0: e8a5 bfe4 bfa1 e681 afe5 ba94 e794 a8e8  ................
-00008cd0: 818c e4b8 9ae6 8a80 e69c afe5 ada6 e999  ................
-00008ce0: a227 7d2c 0d0a 2020 2020 2020 2020 2020  .'},..          
-00008cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d00: 2020 207b 276c 6162 656c 273a 2027 e6b1     {'label': '..
-00008d10: 9fe8 a5bf e5b7 a5e4 b89a e5b7 a5e7 a88b  ................
-00008d20: e881 8ce4 b89a e68a 80e6 9caf e5ad a6e9  ................
-00008d30: 99a2 272c 2027 7661 6c75 6527 3a20 27e6  ..', 'value': '.
-00008d40: b19f e8a5 bfe5 b7a5 e4b8 9ae5 b7a5 e7a8  ................
-00008d50: 8be8 818c e4b8 9ae6 8a80 e69c afe5 ada6  ................
-00008d60: e999 a227 7d2c 0d0a 2020 2020 2020 2020  ...'},..        
-00008d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d80: 2020 2020 207b 276c 6162 656c 273a 2027       {'label': '
-00008d90: e6b1 9fe8 a5bf e4ba a4e9 809a e881 8ce4  ................
-00008da0: b89a e68a 80e6 9caf e5ad a6e9 99a2 272c  ..............',
-00008db0: 2027 7661 6c75 6527 3a20 27e6 b19f e8a5   'value': '.....
-00008dc0: bfe4 baa4 e980 9ae8 818c e4b8 9ae6 8a80  ................
-00008dd0: e69c afe5 ada6 e999 a227 7d2c 0d0a 2020  .........'},..  
-00008de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008df0: 2020 2020 2020 2020 2020 207b 276c 6162             {'lab
-00008e00: 656c 273a 2027 e6b1 9fe8 a5bf e889 bae6  el': '..........
-00008e10: 9caf e881 8ce4 b89a e5ad a6e9 99a2 272c  ..............',
-00008e20: 2027 7661 6c75 6527 3a20 27e6 b19f e8a5   'value': '.....
-00008e30: bfe8 89ba e69c afe8 818c e4b8 9ae5 ada6  ................
-00008e40: e999 a227 7d2c 0d0a 2020 2020 2020 2020  ...'},..        
-00008e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e60: 2020 2020 207b 276c 6162 656c 273a 2027       {'label': '
-00008e70: e6b1 9fe8 a5bf e8b4 a2e7 bb8f e881 8ce4  ................
-00008e80: b89a e5ad a6e9 99a2 272c 2027 7661 6c75  ........', 'valu
-00008e90: 6527 3a20 27e6 b19f e8a5 bfe8 b4a2 e7bb  e': '...........
-00008ea0: 8fe8 818c e4b8 9ae5 ada6 e999 a227 7d2c  .............'},
-00008eb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008ec0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00008ed0: 276c 6162 656c 273a 2027 e6b1 9fe8 a5bf  'label': '......
-00008ee0: e58f b8e6 b395 e8ad a6e5 ae98 e881 8ce4  ................
-00008ef0: b89a e5ad a6e9 99a2 272c 2027 7661 6c75  ........', 'valu
-00008f00: 6527 3a20 27e6 b19f e8a5 bfe5 8fb8 e6b3  e': '...........
-00008f10: 95e8 ada6 e5ae 98e8 818c e4b8 9ae5 ada6  ................
-00008f20: e999 a227 7d2c 0d0a 2020 2020 2020 2020  ...'},..        
-00008f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f40: 2020 2020 207b 276c 6162 656c 273a 2027       {'label': '
-00008f50: e6b1 9fe8 a5bf e5ba 94e7 94a8 e68a 80e6  ................
-00008f60: 9caf e881 8ce4 b89a e5ad a6e9 99a2 272c  ..............',
-00008f70: 2027 7661 6c75 6527 3a20 27e6 b19f e8a5   'value': '.....
-00008f80: bfe5 ba94 e794 a8e6 8a80 e69c afe8 818c  ................
-00008f90: e4b8 9ae5 ada6 e999 a227 7d2c 0d0a 2020  .........'},..  
-00008fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fb0: 2020 2020 2020 2020 2020 207b 276c 6162             {'lab
-00008fc0: 656c 273a 2027 e6b1 9fe8 a5bf e5b8 88e8  el': '..........
-00008fd0: 8c83 e9ab 98e7 ad89 e4b8 93e7 a791 e5ad  ................
-00008fe0: a6e6 a0a1 272c 2027 7661 6c75 6527 3a20  ....', 'value': 
-00008ff0: 27e6 b19f e8a5 bfe5 b888 e88c 83e9 ab98  '...............
-00009000: e7ad 89e4 b893 e7a7 91e5 ada6 e6a0 a127  ...............'
-00009010: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-00009020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009030: 207b 276c 6162 656c 273a 2027 e6b1 9fe8   {'label': '....
-00009040: a5bf e78e b0e4 bba3 e881 8ce4 b89a e68a  ................
-00009050: 80e6 9caf e5ad a6e9 99a2 272c 2027 7661  ..........', 'va
-00009060: 6c75 6527 3a20 27e6 b19f e8a5 bfe7 8eb0  lue': '.........
-00009070: e4bb a3e8 818c e4b8 9ae6 8a80 e69c afe5  ................
-00009080: ada6 e999 a227 7d2c 0d0a 2020 2020 2020  .....'},..      
-00009090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090a0: 2020 2020 2020 207b 276c 6162 656c 273a         {'label':
-000090b0: 2027 e6b1 9fe8 a5bf e5a4 96e8 afad e5a4   '..............
-000090c0: 96e8 b4b8 e881 8ce4 b89a e5ad a6e9 99a2  ................
-000090d0: 272c 2027 7661 6c75 6527 3a20 27e6 b19f  ', 'value': '...
-000090e0: e8a5 bfe5 a496 e8af ade5 a496 e8b4 b8e8  ................
-000090f0: 818c e4b8 9ae5 ada6 e999 a227 7d2c 0d0a  ...........'},..
-00009100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009110: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
-00009120: 6162 656c 273a 2027 e6b1 9fe8 a5bf e5b7  abel': '........
-00009130: a5e4 b89a e8b4 b8e6 9893 e881 8ce4 b89a  ................
-00009140: e68a 80e6 9caf e5ad a6e9 99a2 272c 2027  ............', '
-00009150: 7661 6c75 6527 3a20 27e6 b19f e8a5 bfe5  value': '.......
-00009160: b7a5 e4b8 9ae8 b4b8 e698 93e8 818c e4b8  ................
-00009170: 9ae6 8a80 e69c afe5 ada6 e999 a227 7d2c  .............'},
-00009180: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009190: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000091a0: 276c 6162 656c 273a 2027 e6b1 9fe8 a5bf  'label': '......
-000091b0: e5ba 94e7 94a8 e5b7 a5e7 a88b e881 8ce4  ................
-000091c0: b89a e5ad a6e9 99a2 272c 2027 7661 6c75  ........', 'valu
-000091d0: 6527 3a20 27e6 b19f e8a5 bfe5 ba94 e794  e': '...........
-000091e0: a8e5 b7a5 e7a8 8be8 818c e4b8 9ae5 ada6  ................
-000091f0: e999 a227 7d2c 0d0a 2020 2020 2020 2020  ...'},..        
-00009200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009210: 2020 2020 207b 276c 6162 656c 273a 2027       {'label': '
-00009220: e6b1 9fe8 a5bf e5bb bae8 aebe e881 8ce4  ................
-00009230: b89a e68a 80e6 9caf e5ad a6e9 99a2 272c  ..............',
-00009240: 2027 7661 6c75 6527 3a20 27e6 b19f e8a5   'value': '.....
-00009250: bfe5 bbba e8ae bee8 818c e4b8 9ae6 8a80  ................
-00009260: e69c afe5 ada6 e999 a227 7d2c 0d0a 2020  .........'},..  
-00009270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009280: 2020 2020 2020 2020 2020 207b 276c 6162             {'lab
-00009290: 656c 273a 2027 e5ae 9ce6 98a5 e881 8ce4  el': '..........
-000092a0: b89a e68a 80e6 9caf e5ad a6e9 99a2 272c  ..............',
-000092b0: 2027 7661 6c75 6527 3a20 27e5 ae9c e698   'value': '.....
-000092c0: a5e8 818c e4b8 9ae6 8a80 e69c afe5 ada6  ................
-000092d0: e999 a227 7d2c 0d0a 2020 2020 2020 2020  ...'},..        
-000092e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092f0: 2020 2020 207b 276c 6162 656c 273a 2027       {'label': '
-00009300: e68a 9ae5 b79e e881 8ce4 b89a e68a 80e6  ................
-00009310: 9caf e5ad a6e9 99a2 272c 2027 7661 6c75  ........', 'valu
-00009320: 6527 3a20 27e6 8a9a e5b7 9ee8 818c e4b8  e': '...........
-00009330: 9ae6 8a80 e69c afe5 ada6 e999 a227 7d2c  .............'},
-00009340: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009350: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00009360: 276c 6162 656c 273a 2027 e6b1 9fe8 a5bf  'label': '......
-00009370: e794 9fe7 89a9 e7a7 91e6 8a80 e881 8ce4  ................
-00009380: b89a e5ad a6e9 99a2 272c 2027 7661 6c75  ........', 'valu
-00009390: 6527 3a20 27e6 b19f e8a5 bfe7 949f e789  e': '...........
-000093a0: a9e7 a791 e68a 80e8 818c e4b8 9ae5 ada6  ................
-000093b0: e999 a227 7d2c 0d0a 2020 2020 2020 2020  ...'},..        
-000093c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093d0: 2020 2020 207b 276c 6162 656c 273a 2027       {'label': '
-000093e0: e6b1 9fe8 a5bf e58d abe7 949f e881 8ce4  ................
-000093f0: b89a e5ad a6e9 99a2 272c 2027 7661 6c75  ........', 'valu
-00009400: 6527 3a20 27e6 b19f e8a5 bfe5 8dab e794  e': '...........
-00009410: 9fe8 818c e4b8 9ae5 ada6 e999 a227 7d2c  .............'},
-00009420: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009430: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00009440: 276c 6162 656c 273a 2027 e6b1 9fe8 a5bf  'label': '......
-00009450: e99d 92e5 b9b4 e881 8ce4 b89a e5ad a6e9  ................
-00009460: 99a2 272c 2027 7661 6c75 6527 3a20 27e6  ..', 'value': '.
-00009470: b19f e8a5 bfe9 9d92 e5b9 b4e8 818c e4b8  ................
-00009480: 9ae5 ada6 e999 a227 7d2c 0d0a 2020 2020  .......'},..    
-00009490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094a0: 2020 2020 2020 2020 207b 276c 6162 656c           {'label
-000094b0: 273a 2027 e4b8 8ae9 a5b6 e881 8ce4 b89a  ': '............
-000094c0: e68a 80e6 9caf e5ad a6e9 99a2 272c 2027  ............', '
-000094d0: 7661 6c75 6527 3a20 27e4 b88a e9a5 b6e8  value': '.......
-000094e0: 818c e4b8 9ae6 8a80 e69c afe5 ada6 e999  ................
-000094f0: a227 7d2c 0d0a 2020 2020 2020 2020 2020  .'},..          
-00009500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009510: 2020 207b 276c 6162 656c 273a 2027 e6b1     {'label': '..
-00009520: 9fe8 a5bf e586 9ce4 b89a e5b7 a5e7 a88b  ................
-00009530: e881 8ce4 b89a e5ad a6e9 99a2 272c 2027  ............', '
-00009540: 7661 6c75 6527 3a20 27e6 b19f e8a5 bfe5  value': '.......
-00009550: 869c e4b8 9ae5 b7a5 e7a8 8be8 818c e4b8  ................
-00009560: 9ae5 ada6 e999 a227 7d2c 0d0a 2020 2020  .......'},..    
-00009570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009580: 2020 2020 2020 2020 207b 276c 6162 656c           {'label
-00009590: 273a 2027 e6b1 9fe8 a5bf e7a7 91e6 8a80  ': '............
-000095a0: e881 8ce4 b89a e5ad a6e9 99a2 272c 2027  ............', '
-000095b0: 7661 6c75 6527 3a20 27e6 b19f e8a5 bfe7  value': '.......
-000095c0: a791 e68a 80e8 818c e4b8 9ae5 ada6 e999  ................
-000095d0: a227 7d2c 0d0a 2020 2020 2020 2020 2020  .'},..          
-000095e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095f0: 2020 207b 276c 6162 656c 273a 2027 e6b1     {'label': '..
-00009600: 9fe8 a5bf e888 aae7 a9ba e881 8ce4 b89a  ................
-00009610: e68a 80e6 9caf e5ad a6e9 99a2 272c 2027  ............', '
-00009620: 7661 6c75 6527 3a20 27e6 b19f e8a5 bfe8  value': '.......
-00009630: 88aa e7a9 bae8 818c e4b8 9ae6 8a80 e69c  ................
-00009640: afe5 ada6 e999 a227 7d2c 0d0a 2020 2020  .......'},..    
-00009650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009660: 2020 2020 2020 2020 207b 276c 6162 656c           {'label
-00009670: 273a 2027 e8b5 a3e8 a5bf e7a7 91e6 8a80  ': '............
-00009680: e881 8ce4 b89a e5ad a6e9 99a2 272c 2027  ............', '
-00009690: 7661 6c75 6527 3a20 27e8 b5a3 e8a5 bfe7  value': '.......
-000096a0: a791 e68a 80e8 818c e4b8 9ae5 ada6 e999  ................
-000096b0: a227 7d2c 0d0a 2020 2020 2020 2020 2020  .'},..          
-000096c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096d0: 2020 207b 276c 6162 656c 273a 2027 e6b1     {'label': '..
-000096e0: 9fe8 a5bf e588 b6e9 80a0 e881 8ce4 b89a  ................
-000096f0: e68a 80e6 9caf e5ad a6e9 99a2 272c 2027  ............', '
-00009700: 7661 6c75 6527 3a20 27e6 b19f e8a5 bfe5  value': '.......
-00009710: 88b6 e980 a0e8 818c e4b8 9ae6 8a80 e69c  ................
-00009720: afe5 ada6 e999 a227 7d2c 0d0a 2020 2020  .......'},..    
-00009730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009740: 2020 2020 2020 2020 207b 276c 6162 656c           {'label
-00009750: 273a 2027 e6b1 9fe8 a5bf e5b7 a5e7 a88b  ': '............
-00009760: e881 8ce4 b89a e5ad a6e9 99a2 272c 2027  ............', '
-00009770: 7661 6c75 6527 3a20 27e6 b19f e8a5 bfe5  value': '.......
-00009780: b7a5 e7a8 8be8 818c e4b8 9ae5 ada6 e999  ................
-00009790: a227 7d2c 0d0a 2020 2020 2020 2020 2020  .'},..          
-000097a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097b0: 2020 207b 276c 6162 656c 273a 2027 e6b1     {'label': '..
-000097c0: 9fe8 a5bf e7bb 8fe6 b58e e7ae a1e7 9086  ................
-000097d0: e5b9 b2e9 83a8 e5ad a6e9 99a2 272c 2027  ............', '
-000097e0: 7661 6c75 6527 3a20 27e6 b19f e8a5 bfe7  value': '.......
-000097f0: bb8f e6b5 8ee7 aea1 e790 86e5 b9b2 e983  ................
-00009800: a8e5 ada6 e999 a227 7d2c 0d0a 2020 2020  .......'},..    
-00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009820: 2020 2020 2020 2020 207b 276c 6162 656c           {'label
-00009830: 273a 2027 e6b1 9fe8 a5bf e6b3 b0e8 b1aa  ': '............
-00009840: e58a a8e6 bcab e881 8ce4 b89a e5ad a6e9  ................
-00009850: 99a2 272c 2027 7661 6c75 6527 3a20 27e6  ..', 'value': '.
-00009860: b19f e8a5 bfe6 b3b0 e8b1 aae5 8aa8 e6bc  ................
-00009870: abe8 818c e4b8 9ae5 ada6 e999 a227 7d2c  .............'},
-00009880: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009890: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000098a0: 276c 6162 656c 273a 2027 e6b1 9fe8 a5bf  'label': '......
-000098b0: e69e abe6 9e97 e6b6 89e5 a496 e7bb 8fe8  ................
-000098c0: b4b8 e881 8ce4 b89a e5ad a6e9 99a2 272c  ..............',
-000098d0: 2027 7661 6c75 6527 3a20 27e6 b19f e8a5   'value': '.....
-000098e0: bfe6 9eab e69e 97e6 b689 e5a4 96e7 bb8f  ................
-000098f0: e8b4 b8e8 818c e4b8 9ae5 ada6 e999 a227  ...............'
-00009900: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-00009910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009920: 207b 276c 6162 656c 273a 2027 e6b1 9fe8   {'label': '....
-00009930: a5bf e696 b0e8 83bd e6ba 90e7 a791 e68a  ................
-00009940: 80e8 818c e4b8 9ae5 ada6 e999 a227 2c20  .............', 
-00009950: 2776 616c 7565 273a 2027 e6b1 9fe8 a5bf  'value': '......
-00009960: e696 b0e8 83bd e6ba 90e7 a791 e68a 80e8  ................
-00009970: 818c e4b8 9ae5 ada6 e999 a227 7d2c 0d0a  ...........'},..
-00009980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009990: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
-000099a0: 6162 656c 273a 2027 e6b1 9fe8 a5bf e4bc  abel': '........
-000099b0: a0e5 aa92 e881 8ce4 b89a e5ad a6e9 99a2  ................
-000099c0: 272c 2027 7661 6c75 6527 3a20 27e6 b19f  ', 'value': '...
-000099d0: e8a5 bfe4 bca0 e5aa 92e8 818c e4b8 9ae5  ................
-000099e0: ada6 e999 a227 7d2c 0d0a 2020 2020 2020  .....'},..      
-000099f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a00: 2020 2020 2020 207b 276c 6162 656c 273a         {'label':
-00009a10: 2027 e6b1 9fe8 a5bf e586 b6e9 8791 e881   '..............
-00009a20: 8ce4 b89a e68a 80e6 9caf e5ad a6e9 99a2  ................
-00009a30: 272c 2027 7661 6c75 6527 3a20 27e6 b19f  ', 'value': '...
-00009a40: e8a5 bfe5 86b6 e987 91e8 818c e4b8 9ae6  ................
-00009a50: 8a80 e69c afe5 ada6 e999 a227 7d2c 0d0a  ...........'},..
-00009a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a70: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
-00009a80: 6162 656c 273a 2027 e6b1 9fe8 a5bf e5b7  abel': '........
-00009a90: a5e5 9586 e881 8ce4 b89a e68a 80e6 9caf  ................
-00009aa0: e5ad a6e9 99a2 272c 2027 7661 6c75 6527  ......', 'value'
-00009ab0: 3a20 27e6 b19f e8a5 bfe5 b7a5 e595 86e8  : '.............
-00009ac0: 818c e4b8 9ae6 8a80 e69c afe5 ada6 e999  ................
-00009ad0: a227 7d2c 0d0a 2020 2020 2020 2020 2020  .'},..          
-00009ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009af0: 2020 207b 276c 6162 656c 273a 2027 e585     {'label': '..
-00009b00: b1e9 9d92 e7a7 91e6 8a80 e881 8ce4 b89a  ................
-00009b10: e5ad a6e9 99a2 272c 2027 7661 6c75 6527  ......', 'value'
-00009b20: 3a20 27e5 85b1 e99d 92e7 a791 e68a 80e8  : '.............
-00009b30: 818c e4b8 9ae5 ada6 e999 a227 7d2c 0d0a  ...........'},..
-00009b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b50: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
-00009b60: 6162 656c 273a 2027 e699 afe5 beb7 e995  abel': '........
-00009b70: 87e9 99b6 e793 b7e8 818c e4b8 9ae6 8a80  ................
-00009b80: e69c afe5 ada6 e999 a227 2c20 2776 616c  .........', 'val
-00009b90: 7565 273a 2027 e699 afe5 beb7 e995 87e9  ue': '..........
-00009ba0: 99b6 e793 b7e8 818c e4b8 9ae6 8a80 e69c  ................
-00009bb0: afe5 ada6 e999 a227 7d2c 0d0a 2020 2020  .......'},..    
-00009bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bd0: 2020 2020 2020 2020 207b 276c 6162 656c           {'label
-00009be0: 273a 2027 e6b1 9fe8 a5bf e58c bbe5 ada6  ': '............
-00009bf0: e9ab 98e7 ad89 e4b8 93e7 a791 e5ad a6e6  ................
-00009c00: a0a1 272c 2027 7661 6c75 6527 3a20 27e6  ..', 'value': '.
-00009c10: b19f e8a5 bfe5 8cbb e5ad a6e9 ab98 e7ad  ................
-00009c20: 89e4 b893 e7a7 91e5 ada6 e6a0 a127 7d2c  .............'},
-00009c30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009c40: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00009c50: 276c 6162 656c 273a 2027 e8b5 a3e5 b79e  'label': '......
-00009c60: e5b8 88e8 8c83 e9ab 98e7 ad89 e4b8 93e7  ................
-00009c70: a791 e5ad a6e6 a0a1 272c 2027 7661 6c75  ........', 'valu
-00009c80: 6527 3a20 27e8 b5a3 e5b7 9ee5 b888 e88c  e': '...........
-00009c90: 83e9 ab98 e7ad 89e4 b893 e7a7 91e5 ada6  ................
-00009ca0: e6a0 a127 7d2c 0d0a 2020 2020 2020 2020  ...'},..        
-00009cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cc0: 2020 2020 207b 276c 6162 656c 273a 2027       {'label': '
-00009cd0: e6b1 9fe8 a5bf e6b0 b4e5 88a9 e881 8ce4  ................
-00009ce0: b89a e5ad a6e9 99a2 272c 2027 7661 6c75  ........', 'valu
-00009cf0: 6527 3a20 27e6 b19f e8a5 bfe6 b0b4 e588  e': '...........
-00009d00: a9e8 818c e4b8 9ae5 ada6 e999 a227 7d2c  .............'},
-00009d10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009d20: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00009d30: 276c 6162 656c 273a 2027 e590 89e5 ae89  'label': '......
-00009d40: e881 8ce4 b89a e68a 80e6 9caf e5ad a6e9  ................
-00009d50: 99a2 272c 2027 7661 6c75 6527 3a20 27e5  ..', 'value': '.
-00009d60: 9089 e5ae 89e8 818c e4b8 9ae6 8a80 e69c  ................
-00009d70: afe5 ada6 e999 a227 7d2c 0d0a 2020 2020  .......'},..    
-00009d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d90: 2020 2020 2020 2020 207b 276c 6162 656c           {'label
-00009da0: 273a 2027 e6b1 9fe8 a5bf e6b4 aae5 b79e  ': '............
-00009db0: e881 8ce4 b89a e5ad a6e9 99a2 272c 2027  ............', '
-00009dc0: 7661 6c75 6527 3a20 27e6 b19f e8a5 bfe6  value': '.......
-00009dd0: b4aa e5b7 9ee8 818c e4b8 9ae5 ada6 e999  ................
-00009de0: a227 7d2c 0d0a 2020 2020 2020 2020 2020  .'},..          
-00009df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e00: 2020 207b 276c 6162 656c 273a 2027 e58d     {'label': '..
-00009e10: 97e6 988c e5bd b1e8 a786 e4bc a0e6 92ad  ................
-00009e20: e881 8ce4 b89a e5ad a6e9 99a2 272c 2027  ............', '
-00009e30: 7661 6c75 6527 3a20 27e5 8d97 e698 8ce5  value': '.......
-00009e40: bdb1 e8a7 86e4 bca0 e692 ade8 818c e4b8  ................
-00009e50: 9ae5 ada6 e999 a227 7d2c 0d0a 2020 2020  .......'},..    
-00009e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e70: 2020 2020 2020 2020 207b 276c 6162 656c           {'label
-00009e80: 273a 2027 e8b5 a3e5 8d97 e58d abe7 949f  ': '............
-00009e90: e581 a5e5 bab7 e881 8ce4 b89a e5ad a6e9  ................
-00009ea0: 99a2 272c 2027 7661 6c75 6527 3a20 27e8  ..', 'value': '.
-00009eb0: b5a3 e58d 97e5 8dab e794 9fe5 81a5 e5ba  ................
-00009ec0: b7e8 818c e4b8 9ae5 ada6 e999 a227 7d2c  .............'},
-00009ed0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009ee0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00009ef0: 276c 6162 656c 273a 2027 e68a 9ae5 b79e  'label': '......
-00009f00: e5b9 bce5 84bf e5b8 88e8 8c83 e9ab 98e7  ................
-00009f10: ad89 e4b8 93e7 a791 e5ad a6e6 a0a1 272c  ..............',
-00009f20: 2027 7661 6c75 6527 3a20 27e6 8a9a e5b7   'value': '.....
-00009f30: 9ee5 b9bc e584 bfe5 b888 e88c 83e9 ab98  ................
-00009f40: e7ad 89e4 b893 e7a7 91e5 ada6 e6a0 a127  ...............'
-00009f50: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-00009f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f70: 207b 276c 6162 656c 273a 2027 e4b8 8ae9   {'label': '....
-00009f80: a5b6 e5b9 bce5 84bf e5b8 88e8 8c83 e9ab  ................
-00009f90: 98e7 ad89 e4b8 93e7 a791 e5ad a6e6 a0a1  ................
-00009fa0: 272c 2027 7661 6c75 6527 3a20 27e4 b88a  ', 'value': '...
-00009fb0: e9a5 b6e5 b9bc e584 bfe5 b888 e88c 83e9  ................
-00009fc0: ab98 e7ad 89e4 b893 e7a7 91e5 ada6 e6a0  ................
-00009fd0: a127 7d2c 0d0a 2020 2020 2020 2020 2020  .'},..          
-00009fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ff0: 2020 207b 276c 6162 656c 273a 2027 e5ae     {'label': '..
-0000a000: 9ce6 98a5 e5b9 bce5 84bf e5b8 88e8 8c83  ................
-0000a010: e9ab 98e7 ad89 e4b8 93e7 a791 e5ad a6e6  ................
-0000a020: a0a1 272c 2027 7661 6c75 6527 3a20 27e5  ..', 'value': '.
-0000a030: ae9c e698 a5e5 b9bc e584 bfe5 b888 e88c  ................
-0000a040: 83e9 ab98 e7ad 89e4 b893 e7a7 91e5 ada6  ................
-0000a050: e6a0 a127 7d2c 0d0a 2020 2020 2020 2020  ...'},..        
-0000a060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a070: 2020 2020 207b 276c 6162 656c 273a 2027       {'label': '
-0000a080: e890 8de4 b9a1 e58d abe7 949f e881 8ce4  ................
-0000a090: b89a e5ad a6e9 99a2 272c 2027 7661 6c75  ........', 'valu
-0000a0a0: 6527 3a20 27e8 908d e4b9 a1e5 8dab e794  e': '...........
-0000a0b0: 9fe8 818c e4b8 9ae5 ada6 e999 a227 7d2c  .............'},
-0000a0c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a0d0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-0000a0e0: 276c 6162 656c 273a 2027 e6b1 9fe8 a5bf  'label': '......
-0000a0f0: e5a9 bae6 ba90 e88c b6e4 b89a e881 8ce4  ................
-0000a100: b89a e5ad a6e9 99a2 272c 2027 7661 6c75  ........', 'valu
-0000a110: 6527 3a20 27e6 b19f e8a5 bfe5 a9ba e6ba  e': '...........
-0000a120: 90e8 8cb6 e4b8 9ae8 818c e4b8 9ae5 ada6  ................
-0000a130: e999 a227 7d2c 0d0a 2020 2020 2020 2020  ...'},..        
-0000a140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a150: 2020 2020 207b 276c 6162 656c 273a 2027       {'label': '
-0000a160: e8b5 a3e5 b79e e881 8ce4 b89a e68a 80e6  ................
-0000a170: 9caf e5ad a6e9 99a2 272c 2027 7661 6c75  ........', 'valu
-0000a180: 6527 3a20 27e8 b5a3 e5b7 9ee8 818c e4b8  e': '...........
-0000a190: 9ae6 8a80 e69c afe5 ada6 e999 a227 7d2c  .............'},
-0000a1a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a1b0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-0000a1c0: 276c 6162 656c 273a 2027 e4b9 9de6 b19f  'label': '......
-0000a1d0: e790 86e5 b7a5 e881 8ce4 b89a e5ad a6e9  ................
-0000a1e0: 99a2 272c 2027 7661 6c75 6527 3a20 27e4  ..', 'value': '.
-0000a1f0: b99d e6b1 9fe7 9086 e5b7 a5e8 818c e4b8  ................
-0000a200: 9ae5 ada6 e999 a227 7d2c 0d0a 2020 2020  .......'},..    
-0000a210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a220: 2020 2020 2020 2020 207b 276c 6162 656c           {'label
-0000a230: 273a 2027 e592 8ce5 909b e881 8ce4 b89a  ': '............
-0000a240: e5ad a6e9 99a2 272c 2027 7661 6c75 6527  ......', 'value'
-0000a250: 3a20 27e5 928c e590 9be8 818c e4b8 9ae5  : '.............
-0000a260: ada6 e999 a227 7d5d 0d0a 0d0a 2020 2020  .....'}]....    
-0000a270: 2020 2020 2020 2020 2020 2020 292c 2053              ), S
-0000a280: 656c 6563 7428 0d0a 2020 2020 2020 2020  elect(..        
-0000a290: 2020 2020 2020 2020 2020 2020 7479 7065              type
-0000a2a0: 3d22 7365 6c65 6374 222c 0d0a 2020 2020  ="select",..    
-0000a2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2c0: 6c61 6265 6c3d 22e5 ada6 e999 a2e5 908d  label=".........
-0000a2d0: e7a7 b022 2c0d 0a20 2020 2020 2020 2020  ...",..         
-0000a2e0: 2020 2020 2020 2020 2020 206e 616d 653d             name=
-0000a2f0: 2263 6f6c 6c65 6765 222c 0d0a 2020 2020  "college",..    
-0000a300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a310: 7365 6172 6368 6162 6c65 3d54 7275 652c  searchable=True,
-0000a320: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a330: 2020 2020 2020 7265 7175 6972 6564 3d54        required=T
-0000a340: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-0000a350: 2020 2020 2020 2020 2020 736f 7572 6365            source
-0000a360: 3d22 6765 743a 2f54 6565 6e53 7475 6479  ="get:/TeenStudy
-0000a370: 2f61 7069 2f6f 7267 616e 697a 6174 696f  /api/organizatio
-0000a380: 6e3f 7479 7065 3d6a 7826 756e 6976 6572  n?type=jx&univer
-0000a390: 7369 7479 3d24 7b75 6e69 7665 7273 6974  sity=${universit
-0000a3a0: 797d 2663 6f6c 6c65 6765 3d22 0d0a 2020  y}&college="..  
-0000a3b0: 2020 2020 2020 2020 2020 2020 2020 292c                ),
-0000a3c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a3d0: 2020 5365 6c65 6374 280d 0a20 2020 2020    Select(..     
-0000a3e0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000a3f0: 7970 653d 2273 656c 6563 7422 2c0d 0a20  ype="select",.. 
-0000a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a410: 2020 206c 6162 656c 3d22 e59b a2e6 94af     label="......
-0000a420: e983 a822 2c0d 0a20 2020 2020 2020 2020  ...",..         
-0000a430: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-0000a440: 6970 7469 6f6e 3d22 e59b a2e6 94af e983  iption="........
-0000a450: a8e5 908d e7a7 b0ef bc8c e5af b9e5 ba94  ................
-0000a460: e6b1 9fe8 a5bf e585 b1e9 9d92 e59b a2e4  ................
-0000a470: b8aa e4ba bae4 bfae e694 b9e4 bfa1 e681  ................
-0000a480: afe9 a1b5 20e7 8fad e7ba a72f e59b a2e6  .... ....../....
-0000a490: 94af e983 a822 2c0d 0a20 2020 2020 2020  .....",..       
-0000a4a0: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-0000a4b0: 653d 226f 7267 616e 697a 6174 696f 6e22  e="organization"
-0000a4c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000a4d0: 2020 2020 2020 2073 6561 7263 6861 626c         searchabl
-0000a4e0: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
-0000a4f0: 2020 2020 2020 2020 2020 2020 2072 6571               req
-0000a500: 7569 7265 643d 5472 7565 2c0d 0a20 2020  uired=True,..   
-0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a520: 2073 6f75 7263 653d 2267 6574 3a2f 5465   source="get:/Te
-0000a530: 656e 5374 7564 792f 6170 692f 6f72 6761  enStudy/api/orga
-0000a540: 6e69 7a61 7469 6f6e 3f74 7970 653d 6a78  nization?type=jx
-0000a550: 2675 6e69 7665 7273 6974 793d 247b 756e  &university=${un
-0000a560: 6976 6572 7369 7479 7d26 636f 6c6c 6567  iversity}&colleg
-0000a570: 653d 247b 636f 6c6c 6567 657d 220d 0a20  e=${college}".. 
-0000a580: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000a590: 5d29 2c0d 0a20 2020 2020 2020 2049 6e70  ]),..        Inp
-0000a5a0: 7574 5465 7874 280d 0a20 2020 2020 2020  utText(..       
-0000a5b0: 2020 2020 206c 6162 656c 3d22 e799 bbe5       label="....
-0000a5c0: bd95 e5af 86e7 a081 222c 0d0a 2020 2020  ........",..    
-0000a5d0: 2020 2020 2020 2020 7479 7065 3d27 696e          type='in
-0000a5e0: 7075 742d 7061 7373 776f 7264 272c 0d0a  put-password',..
-0000a5f0: 2020 2020 2020 2020 2020 2020 6465 7363              desc
-0000a600: 7269 7074 696f 6e3d 22e5 8faf e4b8 8de5  ription=".......
-0000a610: a1ab efbc 8ce9 bb98 e8ae a4e4 b8ba e794  ................
-0000a620: a8e6 88b7 4944 222c 0d0a 2020 2020 2020  ....ID",..      
-0000a630: 2020 2020 2020 6e61 6d65 3d22 7061 7373        name="pass
-0000a640: 776f 7264 222c 0d0a 2020 2020 2020 2020  word",..        
-0000a650: 2020 2020 696e 6c69 6e65 3d46 616c 7365      inline=False
-0000a660: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
-0000a670: 6571 7569 7265 643d 4661 6c73 652c 0d0a  equired=False,..
-0000a680: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-0000a690: 653d 2222 2c0d 0a20 2020 2020 2020 2020  e="",..         
-0000a6a0: 2020 2063 6c65 6172 6162 6c65 3d54 7275     clearable=Tru
-0000a6b0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000a6c0: 6d61 784c 656e 6774 683d 3136 0d0a 2020  maxLength=16..  
-0000a6d0: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
-0000a6e0: 2020 496e 7075 7454 6578 7428 0d0a 2020    InputText(..  
-0000a6f0: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
-0000a700: 22e6 898b e69c bae5 8fb7 2fe5 ada6 e58f  "........./.....
-0000a710: b722 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
-0000a720: 2064 6573 6372 6970 7469 6f6e 3d22 e5af   description="..
-0000a730: b9e5 ba94 e6b1 9fe8 a5bf e585 b1e9 9d92  ................
-0000a740: e59b a2e4 b8aa e4ba bae4 bfae e694 b9e4  ................
-0000a750: bfa1 e681 afe9 a1b5 20e6 898b e69c bae5  ........ .......
-0000a760: 8fb7 2fe5 ada6 e58f b7ef bc8c e7a9 bae7  ../.............
-0000a770: 9d80 e4b8 8de7 94a8 e5a1 ab22 2c0d 0a20  ...........",.. 
-0000a780: 2020 2020 2020 2020 2020 206e 616d 653d             name=
-0000a790: 226d 6f62 696c 6522 2c0d 0a20 2020 2020  "mobile",..     
-0000a7a0: 2020 2020 2020 2069 6e6c 696e 653d 4661         inline=Fa
-0000a7b0: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
-0000a7c0: 2020 7265 7175 6972 6564 3d46 616c 7365    required=False
-0000a7d0: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
-0000a7e0: 616c 7565 3d22 222c 0d0a 2020 2020 2020  alue="",..      
-0000a7f0: 2020 2020 2020 636c 6561 7261 626c 653d        clearable=
-0000a800: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
-0000a810: 2020 206d 6178 4c65 6e67 7468 3d31 310d     maxLength=11.
-0000a820: 0a20 2020 2020 2020 2029 2c0d 0a20 2020  .        ),..   
-0000a830: 2020 2020 2049 6e70 7574 5465 7874 280d       InputText(.
-0000a840: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-0000a850: 656c 3d22 e5a7 93e5 908d 222c 0d0a 2020  el="......",..  
-0000a860: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-0000a870: 7074 696f 6e3d 22e5 afb9 e5ba 94e6 b19f  ption=".........
-0000a880: e8a5 bfe5 85b1 e99d 92e5 9ba2 e4b8 aae4  ................
-0000a890: baba e4bf aee6 94b9 e4bf a1e6 81af e9a1  ................
-0000a8a0: b520 e79c 9fe5 ae9e e5a7 93e5 908d 222c  . ............",
-0000a8b0: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
-0000a8c0: 6d65 3d22 6e61 6d65 222c 0d0a 2020 2020  me="name",..    
-0000a8d0: 2020 2020 2020 2020 696e 6c69 6e65 3d46          inline=F
-0000a8e0: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
-0000a8f0: 2020 2072 6571 7569 7265 643d 5472 7565     required=True
-0000a900: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
-0000a910: 616c 7565 3d22 222c 0d0a 2020 2020 2020  alue="",..      
-0000a920: 2020 2020 2020 636c 6561 7261 626c 653d        clearable=
-0000a930: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
-0000a940: 2020 206d 6178 4c65 6e67 7468 3d38 0d0a     maxLength=8..
-0000a950: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
-0000a960: 205d 0d0a 290d 0a22 2222 e6b1 9fe8 8b8f   ]..).."""......
-0000a970: e6b7 bbe5 8aa0 e688 90e5 9198 e99d a2e6  ................
-0000a980: 9dbf 2222 220d 0a6a 6961 6e67 7375 5f74  .."""..jiangsu_t
-0000a990: 6162 6c65 203d 2046 6f72 6d28 0d0a 2020  able = Form(..  
-0000a9a0: 2020 7469 746c 653d 22e6 b7bb e58a a0e6    title=".......
-0000a9b0: b19f e88b 8fe5 85b1 e99d 92e5 9ba2 e794  ................
-0000a9c0: a8e6 88b7 222c 0d0a 2020 2020 7375 626d  ....",..    subm
-0000a9d0: 6974 5465 7874 3d22 e6b7 bbe5 8aa0 222c  itText="......",
-0000a9e0: 0d0a 2020 2020 6d6f 6465 3d44 6973 706c  ..    mode=Displ
-0000a9f0: 6179 4d6f 6465 456e 756d 2e68 6f72 697a  ayModeEnum.horiz
-0000aa00: 6f6e 7461 6c2c 0d0a 2020 2020 6170 693d  ontal,..    api=
-0000aa10: 2270 6f73 743a 2f54 6565 6e53 7475 6479  "post:/TeenStudy
-0000aa20: 2f61 7069 2f6a 6961 6e67 7375 2f61 6464  /api/jiangsu/add
-0000aa30: 222c 0d0a 2020 2020 7265 7365 7441 6674  ",..    resetAft
-0000aa40: 6572 5375 626d 6974 3d54 7275 652c 0d0a  erSubmit=True,..
-0000aa50: 2020 2020 626f 6479 3d5b 0d0a 2020 2020      body=[..    
-0000aa60: 2020 2020 5365 6c65 6374 280d 0a20 2020      Select(..   
-0000aa70: 2020 2020 2020 2020 206c 6162 656c 3d22           label="
-0000aa80: e7be a4e8 818a 222c 0d0a 2020 2020 2020  ......",..      
-0000aa90: 2020 2020 2020 6e61 6d65 3d22 6772 6f75        name="grou
-0000aaa0: 705f 6964 222c 0d0a 2020 2020 2020 2020  p_id",..        
-0000aab0: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
-0000aac0: 22e9 9c80 e8a6 81e6 b7bb e58a a0e7 9a84  "...............
-0000aad0: e7be a4e7 bb84 222c 0d0a 2020 2020 2020  ......",..      
-0000aae0: 2020 2020 2020 6368 6563 6b41 6c6c 3d46        checkAll=F
-0000aaf0: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
-0000ab00: 2020 2073 6f75 7263 653d 2267 6574 3a2f     source="get:/
-0000ab10: 5465 656e 5374 7564 792f 6170 692f 6765  TeenStudy/api/ge
-0000ab20: 745f 6772 6f75 705f 6c69 7374 222c 0d0a  t_group_list",..
-0000ab30: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-0000ab40: 653d 2727 2c0d 0a20 2020 2020 2020 2020  e='',..         
-0000ab50: 2020 206d 756c 7469 706c 653d 4661 6c73     multiple=Fals
-0000ab60: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000ab70: 7265 7175 6972 6564 3d54 7275 652c 0d0a  required=True,..
-0000ab80: 2020 2020 2020 2020 2020 2020 7365 6172              sear
-0000ab90: 6368 6162 6c65 3d54 7275 652c 0d0a 2020  chable=True,..  
-0000aba0: 2020 2020 2020 2020 2020 6a6f 696e 5661            joinVa
-0000abb0: 6c75 6573 3d46 616c 7365 2c0d 0a20 2020  lues=False,..   
-0000abc0: 2020 2020 2020 2020 2065 7874 7261 6374           extract
-0000abd0: 5661 6c75 653d 5472 7565 2c0d 0a20 2020  Value=True,..   
-0000abe0: 2020 2020 2020 2020 2073 7461 7469 7374           statist
-0000abf0: 6963 733d 5472 7565 2c0d 0a20 2020 2020  ics=True,..     
-0000ac00: 2020 2029 2c0d 0a20 2020 2020 2020 2053     ),..        S
-0000ac10: 656c 6563 7428 0d0a 2020 2020 2020 2020  elect(..        
-0000ac20: 2020 2020 6c61 6265 6c3d 22e7 94a8 e688      label=".....
-0000ac30: b749 4422 2c0d 0a20 2020 2020 2020 2020  .ID",..         
-0000ac40: 2020 206e 616d 653d 2275 7365 725f 6964     name="user_id
-0000ac50: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000ac60: 6465 7363 7269 7074 696f 6e3d 22e9 9c80  description="...
-0000ac70: e8a6 81e6 b7bb e58a a0e7 9a84 e794 a8e6  ................
-0000ac80: 88b7 4944 222c 0d0a 2020 2020 2020 2020  ..ID",..        
-0000ac90: 2020 2020 6368 6563 6b41 6c6c 3d46 616c      checkAll=Fal
-0000aca0: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-0000acb0: 2073 6f75 7263 653d 2267 6574 3a2f 5465   source="get:/Te
-0000acc0: 656e 5374 7564 792f 6170 692f 6765 745f  enStudy/api/get_
-0000acd0: 6d65 6d62 6572 5f6c 6973 743f 6772 6f75  member_list?grou
-0000ace0: 705f 6964 3d24 7b67 726f 7570 5f69 647d  p_id=${group_id}
-0000acf0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000ad00: 7661 6c75 653d 2727 2c0d 0a20 2020 2020  value='',..     
-0000ad10: 2020 2020 2020 206d 756c 7469 706c 653d         multiple=
-0000ad20: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-0000ad30: 2020 2020 7265 7175 6972 6564 3d54 7275      required=Tru
-0000ad40: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000ad50: 7365 6172 6368 6162 6c65 3d54 7275 652c  searchable=True,
-0000ad60: 0d0a 2020 2020 2020 2020 2020 2020 6a6f  ..            jo
-0000ad70: 696e 5661 6c75 6573 3d46 616c 7365 2c0d  inValues=False,.
-0000ad80: 0a20 2020 2020 2020 2020 2020 2065 7874  .            ext
-0000ad90: 7261 6374 5661 6c75 653d 5472 7565 2c0d  ractValue=True,.
-0000ada0: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-0000adb0: 7469 7374 6963 733d 5472 7565 2c0d 0a20  tistics=True,.. 
-0000adc0: 2020 2020 2020 2020 2020 2068 6964 6465             hidde
-0000add0: 6e4f 6e3d 2224 7b67 726f 7570 5f69 643d  nOn="${group_id=
-0000ade0: 3d27 273f 7472 7565 3a66 616c 7365 7d22  =''?true:false}"
-0000adf0: 0d0a 2020 2020 2020 2020 292c 0d0a 2020  ..        ),..  
-0000ae00: 2020 2020 2020 496e 7075 7454 6578 7428        InputText(
-0000ae10: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
-0000ae20: 6265 6c3d 22e5 9cb0 e58c ba22 2c0d 0a20  bel="......",.. 
-0000ae30: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-0000ae40: 6970 7469 6f6e 3d22 e689 80e5 a484 e79c  iption="........
-0000ae50: 81e4 bbbd 222c 0d0a 2020 2020 2020 2020  ....",..        
-0000ae60: 2020 2020 6e61 6d65 3d22 6172 6561 222c      name="area",
-0000ae70: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-0000ae80: 6c75 653d 22e6 b19f e88b 8f22 2c0d 0a20  lue="......",.. 
-0000ae90: 2020 2020 2020 2020 2020 2064 6973 6162             disab
-0000aea0: 6c65 643d 5472 7565 0d0a 2020 2020 2020  led=True..      
-0000aeb0: 2020 292c 0d0a 2020 2020 2020 2020 496e    ),..        In
-0000aec0: 7075 7454 6578 7428 0d0a 2020 2020 2020  putText(..      
-0000aed0: 2020 2020 2020 6c61 6265 6c3d 22e7 99bb        label="...
-0000aee0: e5bd 95e5 af86 e7a0 8122 2c0d 0a20 2020  .........",..   
-0000aef0: 2020 2020 2020 2020 2074 7970 653d 2769           type='i
-0000af00: 6e70 7574 2d70 6173 7377 6f72 6427 2c0d  nput-password',.
-0000af10: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-0000af20: 6372 6970 7469 6f6e 3d22 e58f afe4 b88d  cription="......
-0000af30: e5a1 abef bc8c e9bb 98e8 aea4 e4b8 bae7  ................
-0000af40: 94a8 e688 b749 4422 2c0d 0a20 2020 2020  .....ID",..     
-0000af50: 2020 2020 2020 206e 616d 653d 2270 6173         name="pas
-0000af60: 7377 6f72 6422 2c0d 0a20 2020 2020 2020  sword",..       
-0000af70: 2020 2020 2069 6e6c 696e 653d 4661 6c73       inline=Fals
-0000af80: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000af90: 7265 7175 6972 6564 3d46 616c 7365 2c0d  required=False,.
-0000afa0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-0000afb0: 7565 3d22 222c 0d0a 2020 2020 2020 2020  ue="",..        
-0000afc0: 2020 2020 636c 6561 7261 626c 653d 5472      clearable=Tr
-0000afd0: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-0000afe0: 206d 6178 4c65 6e67 7468 3d31 360d 0a20   maxLength=16.. 
-0000aff0: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
-0000b000: 2020 2049 6e70 7574 5465 7874 280d 0a20     InputText(.. 
-0000b010: 2020 2020 2020 2020 2020 206c 6162 656c             label
-0000b020: 3d22 e5a7 93e5 908d 222c 0d0a 2020 2020  ="......",..    
-0000b030: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-0000b040: 696f 6e3d 22e5 afb9 e5ba 94e6 b19f e88b  ion="...........
-0000b050: 8fe5 85b1 e99d 92e5 9ba2 e4b8 aae4 baba  ................
-0000b060: e4bf a1e6 81af e9a1 b520 e682 a8e7 9a84  ......... ......
-0000b070: e5a7 93e5 908d 222c 0d0a 2020 2020 2020  ......",..      
-0000b080: 2020 2020 2020 6e61 6d65 3d22 6e61 6d65        name="name
-0000b090: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000b0a0: 696e 6c69 6e65 3d46 616c 7365 2c0d 0a20  inline=False,.. 
-0000b0b0: 2020 2020 2020 2020 2020 2072 6571 7569             requi
-0000b0c0: 7265 643d 5472 7565 2c0d 0a20 2020 2020  red=True,..     
-0000b0d0: 2020 2020 2020 2076 616c 7565 3d22 222c         value="",
-0000b0e0: 0d0a 2020 2020 2020 2020 2020 2020 636c  ..            cl
-0000b0f0: 6561 7261 626c 653d 5472 7565 2c0d 0a20  earable=True,.. 
-0000b100: 2020 2020 2020 2020 2020 206d 6178 4c65             maxLe
-0000b110: 6e67 7468 3d38 0d0a 2020 2020 2020 2020  ngth=8..        
-0000b120: 292c 0d0a 2020 2020 2020 2020 496e 7075  ),..        Inpu
-0000b130: 7454 6578 7428 0d0a 2020 2020 2020 2020  tText(..        
-0000b140: 2020 2020 6c61 6265 6c3d 22e7 94a8 e688      label=".....
-0000b150: b7e7 bc96 e58f b722 2c0d 0a20 2020 2020  .......",..     
-0000b160: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-0000b170: 6f6e 3d22 e5af b9e5 ba94 e6b1 9fe8 8b8f  on="............
-0000b180: e585 b1e9 9d92 e59b a2e4 b8aa e4ba bae4  ................
-0000b190: bfa1 e681 afe9 a1b5 20e7 94a8 e688 b7e7  ........ .......
-0000b1a0: bc96 e58f b722 2c0d 0a20 2020 2020 2020  .....",..       
-0000b1b0: 2020 2020 206e 616d 653d 2264 7878 5f69       name="dxx_i
-0000b1c0: 6422 2c0d 0a20 2020 2020 2020 2020 2020  d",..           
-0000b1d0: 2069 6e6c 696e 653d 4661 6c73 652c 0d0a   inline=False,..
-0000b1e0: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-0000b1f0: 6972 6564 3d54 7275 652c 0d0a 2020 2020  ired=True,..    
-0000b200: 2020 2020 2020 2020 7661 6c75 653d 2222          value=""
-0000b210: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
-0000b220: 6c65 6172 6162 6c65 3d54 7275 652c 0d0a  learable=True,..
-0000b230: 2020 2020 2020 2020 2020 2020 6d61 784c              maxL
-0000b240: 656e 6774 683d 390d 0a20 2020 2020 2020  ength=9..       
-0000b250: 2029 2c0d 0a20 2020 2020 2020 2049 6e70   ),..        Inp
-0000b260: 7574 5465 7874 280d 0a20 2020 2020 2020  utText(..       
-0000b270: 2020 2020 206c 6162 656c 3d22 636f 6f6b       label="cook
-0000b280: 6965 222c 0d0a 2020 2020 2020 2020 2020  ie",..          
-0000b290: 2020 6465 7363 7269 7074 696f 6e3d 22e8    description=".
-0000b2a0: 87aa e8a1 8ce6 8a93 e58c 85e8 8eb7 e58f  ................
-0000b2b0: 96ef bc8c e7bb 93e6 9e84 e4b8 baef bc9a  ................
-0000b2c0: 6c61 7261 7665 6c5f 7365 7373 696f 6e3d  laravel_session=
-0000b2d0: 4e73 6c64 4d6c 4950 6542 5856 352a 2a2a  NsldMlIPeBXV5***
-0000b2e0: 2a2a 2a2a 2a2a 366c 5944 434f 7065 4e41  ******6lYDCOpeNA
-0000b2f0: 4e6e 6c76 6622 2c0d 0a20 2020 2020 2020  Nnlvf",..       
-0000b300: 2020 2020 206e 616d 653d 2263 6f6f 6b69       name="cooki
-0000b310: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
-0000b320: 2069 6e6c 696e 653d 4661 6c73 652c 0d0a   inline=False,..
-0000b330: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-0000b340: 6972 6564 3d54 7275 652c 0d0a 2020 2020  ired=True,..    
-0000b350: 2020 2020 2020 2020 7661 6c75 653d 2222          value=""
-0000b360: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
-0000b370: 6c65 6172 6162 6c65 3d54 7275 652c 0d0a  learable=True,..
-0000b380: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
-0000b390: 205d 0d0a 290d 0a22 2222 e5ae 89e5 bebd   ]..).."""......
-0000b3a0: e6b7 bbe5 8aa0 e688 90e5 9198 e99d a2e6  ................
-0000b3b0: 9dbf 2222 220d 0a61 6e68 7569 5f74 6162  .."""..anhui_tab
-0000b3c0: 6c65 203d 2046 6f72 6d28 0d0a 2020 2020  le = Form(..    
-0000b3d0: 7469 746c 653d 22e6 b7bb e58a a0e5 ae89  title=".........
-0000b3e0: e5be bde5 85b1 e99d 92e5 9ba2 e794 a8e6  ................
-0000b3f0: 88b7 222c 0d0a 2020 2020 7375 626d 6974  ..",..    submit
-0000b400: 5465 7874 3d22 e6b7 bbe5 8aa0 222c 0d0a  Text="......",..
-0000b410: 2020 2020 6d6f 6465 3d44 6973 706c 6179      mode=Display
-0000b420: 4d6f 6465 456e 756d 2e68 6f72 697a 6f6e  ModeEnum.horizon
-0000b430: 7461 6c2c 0d0a 2020 2020 6170 693d 2270  tal,..    api="p
-0000b440: 6f73 743a 2f54 6565 6e53 7475 6479 2f61  ost:/TeenStudy/a
-0000b450: 7069 2f61 6e68 7569 2f61 6464 222c 0d0a  pi/anhui/add",..
-0000b460: 2020 2020 7265 7365 7441 6674 6572 5375      resetAfterSu
-0000b470: 626d 6974 3d54 7275 652c 0d0a 2020 2020  bmit=True,..    
-0000b480: 626f 6479 3d5b 0d0a 2020 2020 2020 2020  body=[..        
-0000b490: 5365 6c65 6374 280d 0a20 2020 2020 2020  Select(..       
-0000b4a0: 2020 2020 206c 6162 656c 3d22 e7be a4e8       label="....
-0000b4b0: 818a 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
-0000b4c0: 2020 6e61 6d65 3d22 6772 6f75 705f 6964    name="group_id
-0000b4d0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000b4e0: 6465 7363 7269 7074 696f 6e3d 22e9 9c80  description="...
-0000b4f0: e8a6 81e6 b7bb e58a a0e7 9a84 e7be a4e7  ................
-0000b500: bb84 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
-0000b510: 2020 6368 6563 6b41 6c6c 3d46 616c 7365    checkAll=False
-0000b520: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
-0000b530: 6f75 7263 653d 2267 6574 3a2f 5465 656e  ource="get:/Teen
-0000b540: 5374 7564 792f 6170 692f 6765 745f 6772  Study/api/get_gr
-0000b550: 6f75 705f 6c69 7374 222c 0d0a 2020 2020  oup_list",..    
-0000b560: 2020 2020 2020 2020 7661 6c75 653d 2727          value=''
-0000b570: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
-0000b580: 756c 7469 706c 653d 4661 6c73 652c 0d0a  ultiple=False,..
-0000b590: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-0000b5a0: 6972 6564 3d54 7275 652c 0d0a 2020 2020  ired=True,..    
-0000b5b0: 2020 2020 2020 2020 7365 6172 6368 6162          searchab
-0000b5c0: 6c65 3d54 7275 652c 0d0a 2020 2020 2020  le=True,..      
-0000b5d0: 2020 2020 2020 6a6f 696e 5661 6c75 6573        joinValues
-0000b5e0: 3d46 616c 7365 2c0d 0a20 2020 2020 2020  =False,..       
-0000b5f0: 2020 2020 2065 7874 7261 6374 5661 6c75       extractValu
-0000b600: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
-0000b610: 2020 2020 2073 7461 7469 7374 6963 733d       statistics=
-0000b620: 5472 7565 2c0d 0a20 2020 2020 2020 2029  True,..        )
-0000b630: 2c0d 0a20 2020 2020 2020 2053 656c 6563  ,..        Selec
-0000b640: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
-0000b650: 6c61 6265 6c3d 22e7 94a8 e688 b749 4422  label="......ID"
-0000b660: 2c0d 0a20 2020 2020 2020 2020 2020 206e  ,..            n
-0000b670: 616d 653d 2275 7365 725f 6964 222c 0d0a  ame="user_id",..
-0000b680: 2020 2020 2020 2020 2020 2020 6465 7363              desc
-0000b690: 7269 7074 696f 6e3d 22e9 9c80 e8a6 81e6  ription=".......
-0000b6a0: b7bb e58a a0e7 9a84 e794 a8e6 88b7 4944  ..............ID
-0000b6b0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000b6c0: 6368 6563 6b41 6c6c 3d46 616c 7365 2c0d  checkAll=False,.
-0000b6d0: 0a20 2020 2020 2020 2020 2020 2073 6f75  .            sou
-0000b6e0: 7263 653d 2267 6574 3a2f 5465 656e 5374  rce="get:/TeenSt
-0000b6f0: 7564 792f 6170 692f 6765 745f 6d65 6d62  udy/api/get_memb
-0000b700: 6572 5f6c 6973 743f 6772 6f75 705f 6964  er_list?group_id
-0000b710: 3d24 7b67 726f 7570 5f69 647d 222c 0d0a  =${group_id}",..
-0000b720: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-0000b730: 653d 2727 2c0d 0a20 2020 2020 2020 2020  e='',..         
-0000b740: 2020 206d 756c 7469 706c 653d 4661 6c73     multiple=Fals
-0000b750: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000b760: 7265 7175 6972 6564 3d54 7275 652c 0d0a  required=True,..
-0000b770: 2020 2020 2020 2020 2020 2020 7365 6172              sear
-0000b780: 6368 6162 6c65 3d54 7275 652c 0d0a 2020  chable=True,..  
-0000b790: 2020 2020 2020 2020 2020 6a6f 696e 5661            joinVa
-0000b7a0: 6c75 6573 3d46 616c 7365 2c0d 0a20 2020  lues=False,..   
-0000b7b0: 2020 2020 2020 2020 2065 7874 7261 6374           extract
-0000b7c0: 5661 6c75 653d 5472 7565 2c0d 0a20 2020  Value=True,..   
-0000b7d0: 2020 2020 2020 2020 2073 7461 7469 7374           statist
-0000b7e0: 6963 733d 5472 7565 2c0d 0a20 2020 2020  ics=True,..     
-0000b7f0: 2020 2020 2020 2068 6964 6465 6e4f 6e3d         hiddenOn=
-0000b800: 2224 7b67 726f 7570 5f69 643d 3d27 273f  "${group_id==''?
-0000b810: 7472 7565 3a66 616c 7365 7d22 0d0a 2020  true:false}"..  
-0000b820: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
-0000b830: 2020 496e 7075 7454 6578 7428 0d0a 2020    InputText(..  
-0000b840: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
-0000b850: 22e5 9cb0 e58c ba22 2c0d 0a20 2020 2020  "......",..     
-0000b860: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-0000b870: 6f6e 3d22 e689 80e5 a484 e79c 81e4 bbbd  on="............
-0000b880: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000b890: 6e61 6d65 3d22 6172 6561 222c 0d0a 2020  name="area",..  
-0000b8a0: 2020 2020 2020 2020 2020 7661 6c75 653d            value=
-0000b8b0: 22e5 ae89 e5be bd22 2c0d 0a20 2020 2020  "......",..     
-0000b8c0: 2020 2020 2020 2064 6973 6162 6c65 643d         disabled=
-0000b8d0: 5472 7565 0d0a 2020 2020 2020 2020 292c  True..        ),
-0000b8e0: 0d0a 2020 2020 2020 2020 496e 7075 7454  ..        InputT
-0000b8f0: 6578 7428 0d0a 2020 2020 2020 2020 2020  ext(..          
-0000b900: 2020 6c61 6265 6c3d 22e7 99bb e5bd 95e5    label=".......
-0000b910: af86 e7a0 8122 2c0d 0a20 2020 2020 2020  .....",..       
-0000b920: 2020 2020 2074 7970 653d 2769 6e70 7574       type='input
-0000b930: 2d70 6173 7377 6f72 6427 2c0d 0a20 2020  -password',..   
-0000b940: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-0000b950: 7469 6f6e 3d22 e58f afe4 b88d e5a1 abef  tion="..........
-0000b960: bc8c e9bb 98e8 aea4 e4b8 bae7 94a8 e688  ................
-0000b970: b749 4422 2c0d 0a20 2020 2020 2020 2020  .ID",..         
-0000b980: 2020 206e 616d 653d 2270 6173 7377 6f72     name="passwor
-0000b990: 6422 2c0d 0a20 2020 2020 2020 2020 2020  d",..           
-0000b9a0: 2069 6e6c 696e 653d 4661 6c73 652c 0d0a   inline=False,..
-0000b9b0: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-0000b9c0: 6972 6564 3d46 616c 7365 2c0d 0a20 2020  ired=False,..   
-0000b9d0: 2020 2020 2020 2020 2076 616c 7565 3d22           value="
-0000b9e0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000b9f0: 636c 6561 7261 626c 653d 5472 7565 2c0d  clearable=True,.
-0000ba00: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
-0000ba10: 4c65 6e67 7468 3d31 360d 0a20 2020 2020  Length=16..     
-0000ba20: 2020 2029 2c0d 0a20 2020 2020 2020 2049     ),..        I
-0000ba30: 6e70 7574 5465 7874 280d 0a20 2020 2020  nputText(..     
-0000ba40: 2020 2020 2020 206c 6162 656c 3d22 7572         label="ur
-0000ba50: 6c22 2c0d 0a20 2020 2020 2020 2020 2020  l",..           
-0000ba60: 2064 6573 6372 6970 7469 6f6e 3d22 e4b8   description="..
-0000ba70: aae4 baba e4bf a1e6 81af e4bf aee6 94b9  ................
-0000ba80: e9a1 b5ef bc8c e782 b9e5 8fb3 e4b8 8ae8  ................
-0000ba90: a792 e588 86e4 baab efbc 8ce5 a48d e588  ................
-0000baa0: b6e9 93be e68e a5e5 a1ab e585 a5e5 8db3  ................
-0000bab0: e58f af20 e993 bee6 8ea5 e6a0 bce5 bc8f  ... ............
-0000bac0: efbc 9a68 7474 703a 2f2f 6478 782e 6168  ...http://dxx.ah
-0000bad0: 796f 7574 682e 6f72 672e 636e 2f6d 6f64  youth.org.cn/mod
-0000bae0: 6966 792f 3f74 6b3d e682 a8e7 9a84 746f  ify/?tk=......to
-0000baf0: 6b65 6ee5 80bc 222c 0d0a 2020 2020 2020  ken...",..      
-0000bb00: 2020 2020 2020 6e61 6d65 3d22 7572 6c22        name="url"
-0000bb10: 2c0d 0a20 2020 2020 2020 2020 2020 2069  ,..            i
-0000bb20: 6e6c 696e 653d 4661 6c73 652c 0d0a 2020  nline=False,..  
-0000bb30: 2020 2020 2020 2020 2020 7265 7175 6972            requir
-0000bb40: 6564 3d54 7275 652c 0d0a 2020 2020 2020  ed=True,..      
-0000bb50: 2020 2020 2020 7661 6c75 653d 2222 2c0d        value="",.
-0000bb60: 0a20 2020 2020 2020 2020 2020 2063 6c65  .            cle
-0000bb70: 6172 6162 6c65 3d54 7275 652c 0d0a 2020  arable=True,..  
-0000bb80: 2020 2020 2020 2020 2020 6d61 784c 656e            maxLen
-0000bb90: 6774 683d 3132 380d 0a20 2020 2020 2020  gth=128..       
-0000bba0: 2029 0d0a 0d0a 2020 2020 5d0d 0a29 0d0a   )....    ]..)..
-0000bbb0: 2222 22e5 9b9b e5b7 9de6 b7bb e58a a0e6  """.............
-0000bbc0: 8890 e591 98e9 9da2 e69d bf22 2222 0d0a  ..........."""..
-0000bbd0: 7369 6368 7561 6e5f 7461 626c 6520 3d20  sichuan_table = 
-0000bbe0: 466f 726d 280d 0a20 2020 2074 6974 6c65  Form(..    title
-0000bbf0: 3d22 e6b7 bbe5 8aa0 e5a4 a9e5 ba9c e696  ="..............
-0000bc00: b0e9 9d92 e5b9 b4e7 94a8 e688 b722 2c0d  .............",.
-0000bc10: 0a20 2020 2073 7562 6d69 7454 6578 743d  .    submitText=
-0000bc20: 22e6 b7bb e58a a022 2c0d 0a20 2020 206d  "......",..    m
-0000bc30: 6f64 653d 4469 7370 6c61 794d 6f64 6545  ode=DisplayModeE
-0000bc40: 6e75 6d2e 686f 7269 7a6f 6e74 616c 2c0d  num.horizontal,.
-0000bc50: 0a20 2020 2061 7069 3d22 706f 7374 3a2f  .    api="post:/
-0000bc60: 5465 656e 5374 7564 792f 6170 692f 7369  TeenStudy/api/si
-0000bc70: 6368 7561 6e2f 6164 6422 2c0d 0a20 2020  chuan/add",..   
-0000bc80: 2072 6573 6574 4166 7465 7253 7562 6d69   resetAfterSubmi
-0000bc90: 743d 5472 7565 2c0d 0a20 2020 2062 6f64  t=True,..    bod
-0000bca0: 793d 5b0d 0a20 2020 2020 2020 2041 6c65  y=[..        Ale
-0000bcb0: 7274 286c 6576 656c 3d4c 6576 656c 456e  rt(level=LevelEn
-0000bcc0: 756d 2e69 6e66 6f2c 0d0a 2020 2020 2020  um.info,..      
-0000bcd0: 2020 2020 2020 2020 636c 6173 734e 616d          classNam
-0000bce0: 653d 2777 6869 7465 2d73 7061 6365 2d70  e='white-space-p
-0000bcf0: 7265 2d77 7261 7027 2c0d 0a20 2020 2020  re-wrap',..     
-0000bd00: 2020 2020 2020 2020 2062 6f64 793d 280d           body=(.
-0000bd10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bd20: 2020 2022 e8af a5e5 9cb0 e58c bae9 9c80     "............
-0000bd30: e8a6 81e8 87aa e8a1 8ce6 8a93 e58c 85e5  ................
-0000bd40: a1ab e585 a55c 6e74 6f6b 656e e580 bce5  .....\ntoken....
-0000bd50: 9ca8 6874 7470 733a 2f2f 6478 782e 7363  ..https://dxx.sc
-0000bd60: 796f 6c2e 636f 6d2f 6170 692f 7765 6368  yol.com/api/wech
-0000bd70: 6174 2f6c 6f67 696e 20e5 938d e5ba 94e9  at/login .......
-0000bd80: 878c 5c6e e585 b6e4 bd99 e4bf a1e6 81af  ..\n............
-0000bd90: e59c a820 6874 7470 733a 2f2f 6478 782e  ... https://dxx.
-0000bda0: 7363 796f 6c2e 636f 6d2f 6170 692f 7374  scyol.com/api/st
-0000bdb0: 7564 656e 742f 7368 6f77 5374 7564 7953  udent/showStudyS
-0000bdc0: 7461 6765 4f72 673f 6964 3d78 7878 7878  tageOrg?id=xxxxx
-0000bdd0: 7826 7374 6167 6549 643d 7878 20e5 938d  x&stageId=xx ...
-0000bde0: e5ba 94e9 878c 2229 292c 0d0a 2020 2020  ......")),..    
-0000bdf0: 2020 2020 5365 6c65 6374 280d 0a20 2020      Select(..   
-0000be00: 2020 2020 2020 2020 206c 6162 656c 3d22           label="
-0000be10: e7be a4e8 818a 222c 0d0a 2020 2020 2020  ......",..      
-0000be20: 2020 2020 2020 6e61 6d65 3d22 6772 6f75        name="grou
-0000be30: 705f 6964 222c 0d0a 2020 2020 2020 2020  p_id",..        
-0000be40: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
-0000be50: 22e9 9c80 e8a6 81e6 b7bb e58a a0e7 9a84  "...............
-0000be60: e7be a4e7 bb84 222c 0d0a 2020 2020 2020  ......",..      
-0000be70: 2020 2020 2020 6368 6563 6b41 6c6c 3d46        checkAll=F
-0000be80: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
-0000be90: 2020 2073 6f75 7263 653d 2267 6574 3a2f     source="get:/
-0000bea0: 5465 656e 5374 7564 792f 6170 692f 6765  TeenStudy/api/ge
-0000beb0: 745f 6772 6f75 705f 6c69 7374 222c 0d0a  t_group_list",..
-0000bec0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-0000bed0: 653d 2727 2c0d 0a20 2020 2020 2020 2020  e='',..         
-0000bee0: 2020 206d 756c 7469 706c 653d 4661 6c73     multiple=Fals
-0000bef0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000bf00: 7265 7175 6972 6564 3d54 7275 652c 0d0a  required=True,..
-0000bf10: 2020 2020 2020 2020 2020 2020 7365 6172              sear
-0000bf20: 6368 6162 6c65 3d54 7275 652c 0d0a 2020  chable=True,..  
-0000bf30: 2020 2020 2020 2020 2020 6a6f 696e 5661            joinVa
-0000bf40: 6c75 6573 3d46 616c 7365 2c0d 0a20 2020  lues=False,..   
-0000bf50: 2020 2020 2020 2020 2065 7874 7261 6374           extract
-0000bf60: 5661 6c75 653d 5472 7565 2c0d 0a20 2020  Value=True,..   
-0000bf70: 2020 2020 2020 2020 2073 7461 7469 7374           statist
-0000bf80: 6963 733d 5472 7565 2c0d 0a20 2020 2020  ics=True,..     
-0000bf90: 2020 2029 2c0d 0a20 2020 2020 2020 2053     ),..        S
-0000bfa0: 656c 6563 7428 0d0a 2020 2020 2020 2020  elect(..        
-0000bfb0: 2020 2020 6c61 6265 6c3d 22e7 94a8 e688      label=".....
-0000bfc0: b749 4422 2c0d 0a20 2020 2020 2020 2020  .ID",..         
-0000bfd0: 2020 206e 616d 653d 2275 7365 725f 6964     name="user_id
-0000bfe0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000bff0: 6465 7363 7269 7074 696f 6e3d 22e9 9c80  description="...
-0000c000: e8a6 81e6 b7bb e58a a0e7 9a84 e794 a8e6  ................
-0000c010: 88b7 4944 222c 0d0a 2020 2020 2020 2020  ..ID",..        
-0000c020: 2020 2020 6368 6563 6b41 6c6c 3d46 616c      checkAll=Fal
-0000c030: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-0000c040: 2073 6f75 7263 653d 2267 6574 3a2f 5465   source="get:/Te
-0000c050: 656e 5374 7564 792f 6170 692f 6765 745f  enStudy/api/get_
-0000c060: 6d65 6d62 6572 5f6c 6973 743f 6772 6f75  member_list?grou
-0000c070: 705f 6964 3d24 7b67 726f 7570 5f69 647d  p_id=${group_id}
-0000c080: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000c090: 7661 6c75 653d 2727 2c0d 0a20 2020 2020  value='',..     
-0000c0a0: 2020 2020 2020 206d 756c 7469 706c 653d         multiple=
-0000c0b0: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-0000c0c0: 2020 2020 7265 7175 6972 6564 3d54 7275      required=Tru
-0000c0d0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000c0e0: 7365 6172 6368 6162 6c65 3d54 7275 652c  searchable=True,
-0000c0f0: 0d0a 2020 2020 2020 2020 2020 2020 6a6f  ..            jo
-0000c100: 696e 5661 6c75 6573 3d46 616c 7365 2c0d  inValues=False,.
-0000c110: 0a20 2020 2020 2020 2020 2020 2065 7874  .            ext
-0000c120: 7261 6374 5661 6c75 653d 5472 7565 2c0d  ractValue=True,.
-0000c130: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-0000c140: 7469 7374 6963 733d 5472 7565 2c0d 0a20  tistics=True,.. 
-0000c150: 2020 2020 2020 2020 2020 2068 6964 6465             hidde
-0000c160: 6e4f 6e3d 2224 7b67 726f 7570 5f69 643d  nOn="${group_id=
-0000c170: 3d27 273f 7472 7565 3a66 616c 7365 7d22  =''?true:false}"
-0000c180: 0d0a 2020 2020 2020 2020 292c 0d0a 2020  ..        ),..  
-0000c190: 2020 2020 2020 496e 7075 7454 6578 7428        InputText(
-0000c1a0: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
-0000c1b0: 6265 6c3d 22e5 9cb0 e58c ba22 2c0d 0a20  bel="......",.. 
-0000c1c0: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-0000c1d0: 6970 7469 6f6e 3d22 e689 80e5 a484 e79c  iption="........
-0000c1e0: 81e4 bbbd 222c 0d0a 2020 2020 2020 2020  ....",..        
-0000c1f0: 2020 2020 6e61 6d65 3d22 6172 6561 222c      name="area",
-0000c200: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-0000c210: 6c75 653d 22e5 9b9b e5b7 9d22 2c0d 0a20  lue="......",.. 
-0000c220: 2020 2020 2020 2020 2020 2064 6973 6162             disab
-0000c230: 6c65 643d 5472 7565 0d0a 2020 2020 2020  led=True..      
-0000c240: 2020 292c 0d0a 2020 2020 2020 2020 496e    ),..        In
-0000c250: 7075 7454 6578 7428 0d0a 2020 2020 2020  putText(..      
-0000c260: 2020 2020 2020 6c61 6265 6c3d 22e7 99bb        label="...
-0000c270: e5bd 95e5 af86 e7a0 8122 2c0d 0a20 2020  .........",..   
-0000c280: 2020 2020 2020 2020 2074 7970 653d 2769           type='i
-0000c290: 6e70 7574 2d70 6173 7377 6f72 6427 2c0d  nput-password',.
-0000c2a0: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-0000c2b0: 6372 6970 7469 6f6e 3d22 e58f afe4 b88d  cription="......
-0000c2c0: e5a1 abef bc8c e9bb 98e8 aea4 e4b8 bae7  ................
-0000c2d0: 94a8 e688 b749 4422 2c0d 0a20 2020 2020  .....ID",..     
-0000c2e0: 2020 2020 2020 206e 616d 653d 2270 6173         name="pas
-0000c2f0: 7377 6f72 6422 2c0d 0a20 2020 2020 2020  sword",..       
-0000c300: 2020 2020 2069 6e6c 696e 653d 4661 6c73       inline=Fals
-0000c310: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000c320: 7265 7175 6972 6564 3d46 616c 7365 2c0d  required=False,.
-0000c330: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-0000c340: 7565 3d22 222c 0d0a 2020 2020 2020 2020  ue="",..        
-0000c350: 2020 2020 636c 6561 7261 626c 653d 5472      clearable=Tr
-0000c360: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-0000c370: 206d 6178 4c65 6e67 7468 3d31 360d 0a20   maxLength=16.. 
-0000c380: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
-0000c390: 2020 2049 6e70 7574 5465 7874 280d 0a20     InputText(.. 
-0000c3a0: 2020 2020 2020 2020 2020 206c 6162 656c             label
-0000c3b0: 3d22 e5a7 93e5 908d 222c 0d0a 2020 2020  ="......",..    
-0000c3c0: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-0000c3d0: 696f 6e3d 22e5 afb9 e5ba 94e6 8a93 e58c  ion="...........
-0000c3e0: 85e5 8685 e5ae b920 6e61 6d65 222c 0d0a  ....... name",..
-0000c3f0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-0000c400: 3d22 6e61 6d65 222c 0d0a 2020 2020 2020  ="name",..      
-0000c410: 2020 2020 2020 696e 6c69 6e65 3d46 616c        inline=Fal
-0000c420: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-0000c430: 2072 6571 7569 7265 643d 5472 7565 2c0d   required=True,.
-0000c440: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-0000c450: 7565 3d22 222c 0d0a 2020 2020 2020 2020  ue="",..        
-0000c460: 2020 2020 636c 6561 7261 626c 653d 5472      clearable=Tr
-0000c470: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-0000c480: 206d 6178 4c65 6e67 7468 3d38 0d0a 2020   maxLength=8..  
-0000c490: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
-0000c4a0: 2020 496e 7075 7454 6578 7428 0d0a 2020    InputText(..  
-0000c4b0: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
-0000c4c0: 2274 6f6b 656e 222c 0d0a 2020 2020 2020  "token",..      
-0000c4d0: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-0000c4e0: 6e3d 22e8 87aa e8a1 8ce6 8a93 e58c 85e8  n=".............
-0000c4f0: 8eb7 e58f 96ef bc8c e59c a8ef bc9a 6874  ..............ht
-0000c500: 7470 733a 2f2f 6478 782e 7363 796f 6c2e  tps://dxx.scyol.
-0000c510: 636f 6d2f 6170 692f 7765 6368 6174 2f6c  com/api/wechat/l
-0000c520: 6f67 696e 20e9 93be e68e a5e7 9a84 e593  ogin ...........
-0000c530: 8de5 ba94 e586 85e5 aeb9 e987 8c22 2c0d  .............",.
-0000c540: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
-0000c550: 653d 2274 6f6b 656e 222c 0d0a 2020 2020  e="token",..    
-0000c560: 2020 2020 2020 2020 696e 6c69 6e65 3d46          inline=F
-0000c570: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
-0000c580: 2020 2072 6571 7569 7265 643d 5472 7565     required=True
-0000c590: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
-0000c5a0: 616c 7565 3d22 222c 0d0a 2020 2020 2020  alue="",..      
-0000c5b0: 2020 2020 2020 636c 6561 7261 626c 653d        clearable=
-0000c5c0: 5472 7565 2c0d 0a20 2020 2020 2020 2029  True,..        )
-0000c5d0: 2c0d 0a20 2020 2020 2020 2049 6e70 7574  ,..        Input
-0000c5e0: 5465 7874 280d 0a20 2020 2020 2020 2020  Text(..         
-0000c5f0: 2020 206c 6162 656c 3d22 e689 8be6 9cba     label="......
-0000c600: e58f b722 2c0d 0a20 2020 2020 2020 2020  ...",..         
-0000c610: 2020 2064 6573 6372 6970 7469 6f6e 3d22     description="
-0000c620: e887 aae8 a18c e68a 93e5 8c85 e88e b7e5  ................
-0000c630: 8f96 efbc 8ce5 afb9 e5ba 9474 656c 222c  ...........tel",
-0000c640: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
-0000c650: 6d65 3d22 6d6f 6269 6c65 222c 0d0a 2020  me="mobile",..  
-0000c660: 2020 2020 2020 2020 2020 696e 6c69 6e65            inline
-0000c670: 3d46 616c 7365 2c0d 0a20 2020 2020 2020  =False,..       
-0000c680: 2020 2020 2072 6571 7569 7265 643d 5472       required=Tr
-0000c690: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-0000c6a0: 2076 616c 7565 3d22 222c 0d0a 2020 2020   value="",..    
-0000c6b0: 2020 2020 2020 2020 636c 6561 7261 626c          clearabl
-0000c6c0: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
-0000c6d0: 2029 2c0d 0a20 2020 2020 2020 2049 6e70   ),..        Inp
-0000c6e0: 7574 5465 7874 280d 0a20 2020 2020 2020  utText(..       
-0000c6f0: 2020 2020 206c 6162 656c 3d22 e695 b4e4       label="....
-0000c700: bd93 e7bb 84e7 bb87 4944 222c 0d0a 2020  ........ID",..  
-0000c710: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-0000c720: 7074 696f 6e3d 22e8 87aa e8a1 8ce6 8a93  ption=".........
-0000c730: e58c 85e8 8eb7 e58f 96ef bc8c e5af b9e5  ................
-0000c740: ba94 6f72 6722 2c0d 0a20 2020 2020 2020  ..org",..       
-0000c750: 2020 2020 206e 616d 653d 226f 7267 222c       name="org",
-0000c760: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-0000c770: 6c69 6e65 3d46 616c 7365 2c0d 0a20 2020  line=False,..   
-0000c780: 2020 2020 2020 2020 2072 6571 7569 7265           require
-0000c790: 643d 5472 7565 2c0d 0a20 2020 2020 2020  d=True,..       
-0000c7a0: 2020 2020 2076 616c 7565 3d22 222c 0d0a       value="",..
-0000c7b0: 2020 2020 2020 2020 2020 2020 636c 6561              clea
-0000c7c0: 7261 626c 653d 5472 7565 2c0d 0a20 2020  rable=True,..   
-0000c7d0: 2020 2020 2029 2c0d 0a20 2020 2020 2020       ),..       
-0000c7e0: 2049 6e70 7574 5465 7874 280d 0a20 2020   InputText(..   
-0000c7f0: 2020 2020 2020 2020 206c 6162 656c 3d22           label="
-0000c800: e7bb 84e7 bb87 4944 222c 0d0a 2020 2020  ......ID",..    
-0000c810: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-0000c820: 696f 6e3d 22e8 87aa e8a1 8ce6 8a93 e58c  ion="...........
-0000c830: 85e8 8eb7 e58f 96ef bc8c e5af b9e5 ba94  ................
-0000c840: 6c61 7374 4f72 6722 2c0d 0a20 2020 2020  lastOrg",..     
-0000c850: 2020 2020 2020 206e 616d 653d 226c 6173         name="las
-0000c860: 744f 7267 222c 0d0a 2020 2020 2020 2020  tOrg",..        
-0000c870: 2020 2020 696e 6c69 6e65 3d46 616c 7365      inline=False
-0000c880: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
-0000c890: 6571 7569 7265 643d 5472 7565 2c0d 0a20  equired=True,.. 
-0000c8a0: 2020 2020 2020 2020 2020 2076 616c 7565             value
-0000c8b0: 3d22 222c 0d0a 2020 2020 2020 2020 2020  ="",..          
-0000c8c0: 2020 636c 6561 7261 626c 653d 5472 7565    clearable=True
-0000c8d0: 2c0d 0a20 2020 2020 2020 2029 2c0d 0a20  ,..        ),.. 
-0000c8e0: 2020 2020 2020 2049 6e70 7574 5465 7874         InputText
-0000c8f0: 280d 0a20 2020 2020 2020 2020 2020 206c  (..            l
-0000c900: 6162 656c 3d22 e59b a2e6 94af e983 a8e5  abel="..........
-0000c910: 908d e7a7 b022 2c0d 0a20 2020 2020 2020  .....",..       
-0000c920: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-0000c930: 3d22 e887 aae8 a18c e68a 93e5 8c85 e88e  ="..............
-0000c940: b7e5 8f96 efbc 8ce5 afb9 e5ba 9420 6f72  ............. or
-0000c950: 674e 616d 6522 2c0d 0a20 2020 2020 2020  gName",..       
-0000c960: 2020 2020 206e 616d 653d 226f 7267 4e61       name="orgNa
-0000c970: 6d65 222c 0d0a 2020 2020 2020 2020 2020  me",..          
-0000c980: 2020 696e 6c69 6e65 3d46 616c 7365 2c0d    inline=False,.
-0000c990: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-0000c9a0: 7569 7265 643d 5472 7565 2c0d 0a20 2020  uired=True,..   
-0000c9b0: 2020 2020 2020 2020 2076 616c 7565 3d22           value="
-0000c9c0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000c9d0: 636c 6561 7261 626c 653d 5472 7565 2c0d  clearable=True,.
-0000c9e0: 0a20 2020 2020 2020 2029 2c20 496e 7075  .        ), Inpu
-0000c9f0: 7454 6578 7428 0d0a 2020 2020 2020 2020  tText(..        
-0000ca00: 2020 2020 6c61 6265 6c3d 22e7 bb84 e7bb      label=".....
-0000ca10: 87e5 85a8 e7a7 b022 2c0d 0a20 2020 2020  .......",..     
-0000ca20: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-0000ca30: 6f6e 3d22 e887 aae8 a18c e68a 93e5 8c85  on="............
-0000ca40: e88e b7e5 8f96 efbc 8ce5 afb9 e5ba 9461  ...............a
-0000ca50: 6c6c 4f72 674e 616d 6522 2c0d 0a20 2020  llOrgName",..   
-0000ca60: 2020 2020 2020 2020 206e 616d 653d 2261           name="a
-0000ca70: 6c6c 4f72 674e 616d 6522 2c0d 0a20 2020  llOrgName",..   
-0000ca80: 2020 2020 2020 2020 2069 6e6c 696e 653d           inline=
-0000ca90: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-0000caa0: 2020 2020 7265 7175 6972 6564 3d54 7275      required=Tru
-0000cab0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000cac0: 7661 6c75 653d 2222 2c0d 0a20 2020 2020  value="",..     
-0000cad0: 2020 2020 2020 2063 6c65 6172 6162 6c65         clearable
-0000cae0: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
-0000caf0: 290d 0a0d 0a20 2020 205d 0d0a 290d 0a22  )....    ]..).."
-0000cb00: 2222 e5b1 b1e4 b89c e6b7 bbe5 8aa0 e688  ""..............
-0000cb10: 90e5 9198 e99d a2e6 9dbf 2222 220d 0a73  .........."""..s
-0000cb20: 6861 6e64 6f6e 675f 7461 626c 6520 3d20  handong_table = 
-0000cb30: 466f 726d 280d 0a20 2020 2074 6974 6c65  Form(..    title
-0000cb40: 3d22 e6b7 bbe5 8aa0 e99d 92e6 98a5 e5b1  ="..............
-0000cb50: b1e4 b89c e794 a8e6 88b7 222c 0d0a 2020  ..........",..  
-0000cb60: 2020 7375 6e6d 6974 5465 7874 3d22 e6b7    sunmitText="..
-0000cb70: bbe5 8aa0 222c 0d0a 2020 2020 6d6f 6465  ....",..    mode
-0000cb80: 3d44 6973 706c 6179 4d6f 6465 456e 756d  =DisplayModeEnum
-0000cb90: 2e68 6f72 697a 6f6e 7461 6c2c 0d0a 2020  .horizontal,..  
-0000cba0: 2020 6170 693d 2270 6f73 743a 2f54 6565    api="post:/Tee
-0000cbb0: 6e53 7475 6479 2f61 7069 2f73 6861 6e64  nStudy/api/shand
-0000cbc0: 6f6e 672f 6164 6422 2c0d 0a20 2020 2072  ong/add",..    r
-0000cbd0: 6573 6574 4166 7465 7253 7562 6d69 743d  esetAfterSubmit=
-0000cbe0: 5472 7565 2c0d 0a20 2020 2062 6f64 793d  True,..    body=
-0000cbf0: 5b0d 0a20 2020 2020 2020 2053 656c 6563  [..        Selec
-0000cc00: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
-0000cc10: 6c61 6265 6c3d 22e7 bea4 e881 8a22 2c0d  label="......",.
-0000cc20: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
-0000cc30: 653d 2267 726f 7570 5f69 6422 2c0d 0a20  e="group_id",.. 
-0000cc40: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-0000cc50: 6970 7469 6f6e 3d22 e99c 80e8 a681 e6b7  iption="........
-0000cc60: bbe5 8aa0 e79a 84e7 bea4 e7bb 8422 2c0d  .............",.
-0000cc70: 0a20 2020 2020 2020 2020 2020 2063 6865  .            che
-0000cc80: 636b 416c 6c3d 4661 6c73 652c 0d0a 2020  ckAll=False,..  
-0000cc90: 2020 2020 2020 2020 2020 736f 7572 6365            source
-0000cca0: 3d22 6765 743a 2f54 6565 6e53 7475 6479  ="get:/TeenStudy
-0000ccb0: 2f61 7069 2f67 6574 5f67 726f 7570 5f6c  /api/get_group_l
-0000ccc0: 6973 7422 2c0d 0a20 2020 2020 2020 2020  ist",..         
-0000ccd0: 2020 2076 616c 7565 3d27 272c 0d0a 2020     value='',..  
-0000cce0: 2020 2020 2020 2020 2020 6d75 6c74 6970            multip
-0000ccf0: 6c65 3d46 616c 7365 2c0d 0a20 2020 2020  le=False,..     
-0000cd00: 2020 2020 2020 2072 6571 7569 7265 643d         required=
-0000cd10: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
-0000cd20: 2020 2073 6561 7263 6861 626c 653d 5472     searchable=Tr
-0000cd30: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-0000cd40: 206a 6f69 6e56 616c 7565 733d 4661 6c73   joinValues=Fals
-0000cd50: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000cd60: 6578 7472 6163 7456 616c 7565 3d54 7275  extractValue=Tru
-0000cd70: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000cd80: 7374 6174 6973 7469 6373 3d54 7275 652c  statistics=True,
-0000cd90: 0d0a 2020 2020 2020 2020 292c 0d0a 2020  ..        ),..  
-0000cda0: 2020 2020 2020 5365 6c65 6374 280d 0a20        Select(.. 
-0000cdb0: 2020 2020 2020 2020 2020 206c 6162 656c             label
-0000cdc0: 3d22 e794 a8e6 88b7 4944 222c 0d0a 2020  ="......ID",..  
-0000cdd0: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
-0000cde0: 7573 6572 5f69 6422 2c0d 0a20 2020 2020  user_id",..     
-0000cdf0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-0000ce00: 6f6e 3d22 e99c 80e8 a681 e6b7 bbe5 8aa0  on="............
-0000ce10: e79a 84e7 94a8 e688 b749 4422 2c0d 0a20  .........ID",.. 
-0000ce20: 2020 2020 2020 2020 2020 2063 6865 636b             check
-0000ce30: 416c 6c3d 4661 6c73 652c 0d0a 2020 2020  All=False,..    
-0000ce40: 2020 2020 2020 2020 736f 7572 6365 3d22          source="
-0000ce50: 6765 743a 2f54 6565 6e53 7475 6479 2f61  get:/TeenStudy/a
-0000ce60: 7069 2f67 6574 5f6d 656d 6265 725f 6c69  pi/get_member_li
-0000ce70: 7374 3f67 726f 7570 5f69 643d 247b 6772  st?group_id=${gr
-0000ce80: 6f75 705f 6964 7d22 2c0d 0a20 2020 2020  oup_id}",..     
-0000ce90: 2020 2020 2020 2076 616c 7565 3d27 272c         value='',
-0000cea0: 0d0a 2020 2020 2020 2020 2020 2020 6d75  ..            mu
-0000ceb0: 6c74 6970 6c65 3d46 616c 7365 2c0d 0a20  ltiple=False,.. 
-0000cec0: 2020 2020 2020 2020 2020 2072 6571 7569             requi
-0000ced0: 7265 643d 5472 7565 2c0d 0a20 2020 2020  red=True,..     
-0000cee0: 2020 2020 2020 2073 6561 7263 6861 626c         searchabl
-0000cef0: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
-0000cf00: 2020 2020 206a 6f69 6e56 616c 7565 733d       joinValues=
-0000cf10: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-0000cf20: 2020 2020 6578 7472 6163 7456 616c 7565      extractValue
-0000cf30: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
-0000cf40: 2020 2020 7374 6174 6973 7469 6373 3d54      statistics=T
-0000cf50: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-0000cf60: 2020 6869 6464 656e 4f6e 3d22 247b 6772    hiddenOn="${gr
-0000cf70: 6f75 705f 6964 3d3d 2727 3f74 7275 653a  oup_id==''?true:
-0000cf80: 6661 6c73 657d 220d 0a20 2020 2020 2020  false}"..       
-0000cf90: 2029 2c0d 0a20 2020 2020 2020 2049 6e70   ),..        Inp
-0000cfa0: 7574 5465 7874 280d 0a20 2020 2020 2020  utText(..       
-0000cfb0: 2020 2020 206c 6162 656c 3d22 e59c b0e5       label="....
-0000cfc0: 8cba 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
-0000cfd0: 2020 6465 7363 7269 7074 696f 6e3d 22e6    description=".
-0000cfe0: 8980 e5a4 84e7 9c81 e4bb bd22 2c0d 0a20  ...........",.. 
-0000cff0: 2020 2020 2020 2020 2020 206e 616d 653d             name=
-0000d000: 2261 7265 6122 2c0d 0a20 2020 2020 2020  "area",..       
-0000d010: 2020 2020 2076 616c 7565 3d22 e5b1 b1e4       value="....
-0000d020: b89c 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
-0000d030: 2020 6469 7361 626c 6564 3d54 7275 650d    disabled=True.
-0000d040: 0a20 2020 2020 2020 2029 2c0d 0a20 2020  .        ),..   
-0000d050: 2020 2020 2049 6e70 7574 5465 7874 280d       InputText(.
-0000d060: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-0000d070: 656c 3d22 e799 bbe5 bd95 e5af 86e7 a081  el="............
-0000d080: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000d090: 7479 7065 3d27 696e 7075 742d 7061 7373  type='input-pass
-0000d0a0: 776f 7264 272c 0d0a 2020 2020 2020 2020  word',..        
-0000d0b0: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
-0000d0c0: 22e5 8faf e4b8 8de5 a1ab efbc 8ce9 bb98  "...............
-0000d0d0: e8ae a4e4 b8ba e794 a8e6 88b7 4944 222c  ............ID",
-0000d0e0: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
-0000d0f0: 6d65 3d22 7061 7373 776f 7264 222c 0d0a  me="password",..
-0000d100: 2020 2020 2020 2020 2020 2020 696e 6c69              inli
-0000d110: 6e65 3d46 616c 7365 2c0d 0a20 2020 2020  ne=False,..     
-0000d120: 2020 2020 2020 2072 6571 7569 7265 643d         required=
-0000d130: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-0000d140: 2020 2020 7661 6c75 653d 2222 2c0d 0a20      value="",.. 
-0000d150: 2020 2020 2020 2020 2020 2063 6c65 6172             clear
-0000d160: 6162 6c65 3d54 7275 652c 0d0a 2020 2020  able=True,..    
-0000d170: 2020 2020 2020 2020 6d61 784c 656e 6774          maxLengt
-0000d180: 683d 3136 0d0a 2020 2020 2020 2020 292c  h=16..        ),
-0000d190: 0d0a 2020 2020 2020 2020 496e 7075 7454  ..        InputT
-0000d1a0: 6578 7428 0d0a 2020 2020 2020 2020 2020  ext(..          
-0000d1b0: 2020 6c61 6265 6c3d 22e5 a793 e590 8d22    label="......"
-0000d1c0: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
-0000d1d0: 6573 6372 6970 7469 6f6e 3d22 e5af b9e5  escription="....
-0000d1e0: ba94 e99d 92e6 98a5 e5b1 b1e4 b89c e4b8  ................
-0000d1f0: aae4 baba e4bf a1e6 81af e9a1 b520 e682  ............. ..
-0000d200: a8e7 9a84 e5a7 93e5 908d 222c 0d0a 2020  ..........",..  
-0000d210: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
-0000d220: 6e61 6d65 222c 0d0a 2020 2020 2020 2020  name",..        
-0000d230: 2020 2020 696e 6c69 6e65 3d46 616c 7365      inline=False
-0000d240: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
-0000d250: 6571 7569 7265 643d 5472 7565 2c0d 0a20  equired=True,.. 
-0000d260: 2020 2020 2020 2020 2020 2076 616c 7565             value
-0000d270: 3d22 222c 0d0a 2020 2020 2020 2020 2020  ="",..          
-0000d280: 2020 636c 6561 7261 626c 653d 5472 7565    clearable=True
-0000d290: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
-0000d2a0: 6178 4c65 6e67 7468 3d38 0d0a 2020 2020  axLength=8..    
-0000d2b0: 2020 2020 292c 0d0a 2020 2020 2020 2020      ),..        
-0000d2c0: 496e 7075 7454 6578 7428 0d0a 2020 2020  InputText(..    
-0000d2d0: 2020 2020 2020 2020 6c61 6265 6c3d 2263          label="c
-0000d2e0: 6f6f 6b69 6522 2c0d 0a20 2020 2020 2020  ookie",..       
-0000d2f0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-0000d300: 3d22 e887 aae8 a18c e68a 93e5 8c85 e88e  ="..............
-0000d310: b7e5 8f96 efbc 8ce7 bb93 e69e 84e4 b8ba  ................
-0000d320: efbc 9a4a 5345 5353 494f 4e49 443d 3138  ...JSESSIONID=18
-0000d330: 3733 4658 5858 5858 5858 5835 4446 4342  73FXXXXXXXX5DFCB
-0000d340: 4631 4343 3133 3730 3322 2c0d 0a20 2020  F1CC13703",..   
-0000d350: 2020 2020 2020 2020 206e 616d 653d 2263           name="c
-0000d360: 6f6f 6b69 6522 2c0d 0a20 2020 2020 2020  ookie",..       
-0000d370: 2020 2020 2069 6e6c 696e 653d 4661 6c73       inline=Fals
-0000d380: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000d390: 7265 7175 6972 6564 3d54 7275 652c 0d0a  required=True,..
-0000d3a0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-0000d3b0: 653d 2222 2c0d 0a20 2020 2020 2020 2020  e="",..         
-0000d3c0: 2020 2063 6c65 6172 6162 6c65 3d54 7275     clearable=Tru
-0000d3d0: 652c 0d0a 2020 2020 2020 2020 292c 0d0a  e,..        ),..
-0000d3e0: 2020 2020 2020 2020 496e 7075 7454 6578          InputTex
-0000d3f0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
-0000d400: 6c61 6265 6c3d 226f 7065 6e69 6422 2c0d  label="openid",.
-0000d410: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-0000d420: 6372 6970 7469 6f6e 3d22 e887 aae8 a18c  cription="......
-0000d430: e68a 93e5 8c85 e88e b7e5 8f96 efbc 8ce7  ................
-0000d440: bb93 e69e 84e4 b8ba efbc 9a6f 687a 3978  ...........ohz9x
-0000d450: 7878 7878 7878 7878 7878 786c 4630 496f  xxxxxxxxxxxlF0Io
-0000d460: 3075 436e 4d22 2c0d 0a20 2020 2020 2020  0uCnM",..       
-0000d470: 2020 2020 206e 616d 653d 226f 7065 6e69       name="openi
-0000d480: 6422 2c0d 0a20 2020 2020 2020 2020 2020  d",..           
-0000d490: 2069 6e6c 696e 653d 4661 6c73 652c 0d0a   inline=False,..
-0000d4a0: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-0000d4b0: 6972 6564 3d54 7275 652c 0d0a 2020 2020  ired=True,..    
-0000d4c0: 2020 2020 2020 2020 7661 6c75 653d 2222          value=""
-0000d4d0: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
-0000d4e0: 6c65 6172 6162 6c65 3d54 7275 652c 0d0a  learable=True,..
-0000d4f0: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
-0000d500: 205d 0d0a 290d 0a22 2222 e987 8de5 ba86   ]..).."""......
-0000d510: e6b7 bbe5 8aa0 e688 90e5 9198 e99d a2e6  ................
-0000d520: 9dbf 2222 220d 0a63 686f 6e67 7169 6e67  .."""..chongqing
-0000d530: 5f74 6162 6c65 203d 2046 6f72 6d28 0d0a  _table = Form(..
-0000d540: 2020 2020 7469 746c 653d 22e6 b7bb e58a      title=".....
-0000d550: a0e9 878d e5ba 86e5 85b1 e99d 92e5 9ba2  ................
-0000d560: e794 a8e6 88b7 222c 0d0a 2020 2020 7375  ......",..    su
-0000d570: 6e6d 6974 5465 7874 3d22 e6b7 bbe5 8aa0  nmitText="......
-0000d580: 222c 0d0a 2020 2020 6d6f 6465 3d44 6973  ",..    mode=Dis
-0000d590: 706c 6179 4d6f 6465 456e 756d 2e68 6f72  playModeEnum.hor
-0000d5a0: 697a 6f6e 7461 6c2c 0d0a 2020 2020 6170  izontal,..    ap
-0000d5b0: 693d 2270 6f73 743a 2f54 6565 6e53 7475  i="post:/TeenStu
-0000d5c0: 6479 2f61 7069 2f63 686f 6e67 7169 6e67  dy/api/chongqing
-0000d5d0: 2f61 6464 222c 0d0a 2020 2020 7265 7365  /add",..    rese
-0000d5e0: 7441 6674 6572 5375 626d 6974 3d54 7275  tAfterSubmit=Tru
-0000d5f0: 652c 0d0a 2020 2020 626f 6479 3d5b 0d0a  e,..    body=[..
-0000d600: 2020 2020 2020 2020 5365 6c65 6374 280d          Select(.
-0000d610: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-0000d620: 656c 3d22 e7be a4e8 818a 222c 0d0a 2020  el="......",..  
-0000d630: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
-0000d640: 6772 6f75 705f 6964 222c 0d0a 2020 2020  group_id",..    
-0000d650: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-0000d660: 696f 6e3d 22e9 9c80 e8a6 81e6 b7bb e58a  ion="...........
-0000d670: a0e7 9a84 e7be a4e7 bb84 222c 0d0a 2020  ..........",..  
-0000d680: 2020 2020 2020 2020 2020 6368 6563 6b41            checkA
-0000d690: 6c6c 3d46 616c 7365 2c0d 0a20 2020 2020  ll=False,..     
-0000d6a0: 2020 2020 2020 2073 6f75 7263 653d 2267         source="g
-0000d6b0: 6574 3a2f 5465 656e 5374 7564 792f 6170  et:/TeenStudy/ap
-0000d6c0: 692f 6765 745f 6772 6f75 705f 6c69 7374  i/get_group_list
-0000d6d0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000d6e0: 7661 6c75 653d 2727 2c0d 0a20 2020 2020  value='',..     
-0000d6f0: 2020 2020 2020 206d 756c 7469 706c 653d         multiple=
-0000d700: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-0000d710: 2020 2020 7265 7175 6972 6564 3d54 7275      required=Tru
-0000d720: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000d730: 7365 6172 6368 6162 6c65 3d54 7275 652c  searchable=True,
-0000d740: 0d0a 2020 2020 2020 2020 2020 2020 6a6f  ..            jo
-0000d750: 696e 5661 6c75 6573 3d46 616c 7365 2c0d  inValues=False,.
-0000d760: 0a20 2020 2020 2020 2020 2020 2065 7874  .            ext
-0000d770: 7261 6374 5661 6c75 653d 5472 7565 2c0d  ractValue=True,.
-0000d780: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-0000d790: 7469 7374 6963 733d 5472 7565 2c0d 0a20  tistics=True,.. 
-0000d7a0: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
-0000d7b0: 2020 2053 656c 6563 7428 0d0a 2020 2020     Select(..    
-0000d7c0: 2020 2020 2020 2020 6c61 6265 6c3d 22e7          label=".
-0000d7d0: 94a8 e688 b749 4422 2c0d 0a20 2020 2020  .....ID",..     
-0000d7e0: 2020 2020 2020 206e 616d 653d 2275 7365         name="use
-0000d7f0: 725f 6964 222c 0d0a 2020 2020 2020 2020  r_id",..        
-0000d800: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
-0000d810: 22e9 9c80 e8a6 81e6 b7bb e58a a0e7 9a84  "...............
-0000d820: e794 a8e6 88b7 4944 222c 0d0a 2020 2020  ......ID",..    
-0000d830: 2020 2020 2020 2020 6368 6563 6b41 6c6c          checkAll
-0000d840: 3d46 616c 7365 2c0d 0a20 2020 2020 2020  =False,..       
-0000d850: 2020 2020 2073 6f75 7263 653d 2267 6574       source="get
-0000d860: 3a2f 5465 656e 5374 7564 792f 6170 692f  :/TeenStudy/api/
-0000d870: 6765 745f 6d65 6d62 6572 5f6c 6973 743f  get_member_list?
-0000d880: 6772 6f75 705f 6964 3d24 7b67 726f 7570  group_id=${group
-0000d890: 5f69 647d 222c 0d0a 2020 2020 2020 2020  _id}",..        
-0000d8a0: 2020 2020 7661 6c75 653d 2727 2c0d 0a20      value='',.. 
-0000d8b0: 2020 2020 2020 2020 2020 206d 756c 7469             multi
-0000d8c0: 706c 653d 4661 6c73 652c 0d0a 2020 2020  ple=False,..    
-0000d8d0: 2020 2020 2020 2020 7265 7175 6972 6564          required
-0000d8e0: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
-0000d8f0: 2020 2020 7365 6172 6368 6162 6c65 3d54      searchable=T
-0000d900: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-0000d910: 2020 6a6f 696e 5661 6c75 6573 3d46 616c    joinValues=Fal
-0000d920: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-0000d930: 2065 7874 7261 6374 5661 6c75 653d 5472   extractValue=Tr
-0000d940: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-0000d950: 2073 7461 7469 7374 6963 733d 5472 7565   statistics=True
-0000d960: 2c0d 0a20 2020 2020 2020 2020 2020 2068  ,..            h
-0000d970: 6964 6465 6e4f 6e3d 2224 7b67 726f 7570  iddenOn="${group
-0000d980: 5f69 643d 3d27 273f 7472 7565 3a66 616c  _id==''?true:fal
-0000d990: 7365 7d22 0d0a 2020 2020 2020 2020 292c  se}"..        ),
-0000d9a0: 0d0a 2020 2020 2020 2020 496e 7075 7454  ..        InputT
-0000d9b0: 6578 7428 0d0a 2020 2020 2020 2020 2020  ext(..          
-0000d9c0: 2020 6c61 6265 6c3d 22e5 9cb0 e58c ba22    label="......"
-0000d9d0: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
-0000d9e0: 6573 6372 6970 7469 6f6e 3d22 e689 80e5  escription="....
-0000d9f0: a484 e79c 81e4 bbbd 222c 0d0a 2020 2020  ........",..    
-0000da00: 2020 2020 2020 2020 6e61 6d65 3d22 6172          name="ar
-0000da10: 6561 222c 0d0a 2020 2020 2020 2020 2020  ea",..          
-0000da20: 2020 7661 6c75 653d 22e9 878d e5ba 8622    value="......"
-0000da30: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
-0000da40: 6973 6162 6c65 643d 5472 7565 0d0a 2020  isabled=True..  
-0000da50: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
-0000da60: 2020 496e 7075 7454 6578 7428 0d0a 2020    InputText(..  
-0000da70: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
-0000da80: 22e7 99bb e5bd 95e5 af86 e7a0 8122 2c0d  "............",.
-0000da90: 0a20 2020 2020 2020 2020 2020 2074 7970  .            typ
-0000daa0: 653d 2769 6e70 7574 2d70 6173 7377 6f72  e='input-passwor
-0000dab0: 6427 2c0d 0a20 2020 2020 2020 2020 2020  d',..           
-0000dac0: 2064 6573 6372 6970 7469 6f6e 3d22 e58f   description="..
-0000dad0: afe4 b88d e5a1 abef bc8c e9bb 98e8 aea4  ................
-0000dae0: e4b8 bae7 94a8 e688 b749 4422 2c0d 0a20  .........ID",.. 
-0000daf0: 2020 2020 2020 2020 2020 206e 616d 653d             name=
-0000db00: 2270 6173 7377 6f72 6422 2c0d 0a20 2020  "password",..   
-0000db10: 2020 2020 2020 2020 2069 6e6c 696e 653d           inline=
-0000db20: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-0000db30: 2020 2020 7265 7175 6972 6564 3d46 616c      required=Fal
-0000db40: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-0000db50: 2076 616c 7565 3d22 222c 0d0a 2020 2020   value="",..    
-0000db60: 2020 2020 2020 2020 636c 6561 7261 626c          clearabl
-0000db70: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
-0000db80: 2020 2020 206d 6178 4c65 6e67 7468 3d31       maxLength=1
-0000db90: 360d 0a20 2020 2020 2020 2029 2c0d 0a20  6..        ),.. 
-0000dba0: 2020 2020 2020 2049 6e70 7574 5465 7874         InputText
-0000dbb0: 280d 0a20 2020 2020 2020 2020 2020 206c  (..            l
-0000dbc0: 6162 656c 3d22 e5a7 93e5 908d 222c 0d0a  abel="......",..
-0000dbd0: 2020 2020 2020 2020 2020 2020 6465 7363              desc
-0000dbe0: 7269 7074 696f 6e3d 22e5 afb9 e5ba 94e9  ription=".......
-0000dbf0: 878d e5ba 86e5 85b1 e99d 92e5 9ba2 e4b8  ................
-0000dc00: aae4 baba e4bf a1e6 81af e9a1 b520 e682  ............. ..
-0000dc10: a8e7 9a84 e5a7 93e5 908d 222c 0d0a 2020  ..........",..  
-0000dc20: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
-0000dc30: 6e61 6d65 222c 0d0a 2020 2020 2020 2020  name",..        
-0000dc40: 2020 2020 696e 6c69 6e65 3d46 616c 7365      inline=False
-0000dc50: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
-0000dc60: 6571 7569 7265 643d 5472 7565 2c0d 0a20  equired=True,.. 
-0000dc70: 2020 2020 2020 2020 2020 2076 616c 7565             value
-0000dc80: 3d22 222c 0d0a 2020 2020 2020 2020 2020  ="",..          
-0000dc90: 2020 636c 6561 7261 626c 653d 5472 7565    clearable=True
-0000dca0: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
-0000dcb0: 6178 4c65 6e67 7468 3d38 0d0a 2020 2020  axLength=8..    
-0000dcc0: 2020 2020 292c 0d0a 2020 2020 2020 2020      ),..        
-0000dcd0: 496e 7075 7454 6578 7428 0d0a 2020 2020  InputText(..    
-0000dce0: 2020 2020 2020 2020 6c61 6265 6c3d 226f          label="o
-0000dcf0: 7065 6e69 6422 2c0d 0a20 2020 2020 2020  penid",..       
-0000dd00: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-0000dd10: 3d22 e887 aae8 a18c e68a 93e5 8c85 e88e  ="..............
-0000dd20: b7e5 8f96 efbc 8ce7 bb93 e69e 84e4 b8ba  ................
-0000dd30: 3a20 6f68 7a39 7878 7878 7878 7878 7878  : ohz9xxxxxxxxxx
-0000dd40: 7878 6c46 3049 6f30 7543 6e4d 222c 0d0a  xxlF0Io0uCnM",..
-0000dd50: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-0000dd60: 3d22 6f70 656e 6964 222c 0d0a 2020 2020  ="openid",..    
-0000dd70: 2020 2020 2020 2020 696e 6c69 6e65 3d46          inline=F
-0000dd80: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
-0000dd90: 2020 2072 6571 7569 7265 643d 5472 7565     required=True
-0000dda0: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
-0000ddb0: 616c 7565 3d22 222c 0d0a 2020 2020 2020  alue="",..      
-0000ddc0: 2020 2020 2020 636c 6561 7261 626c 653d        clearable=
-0000ddd0: 5472 7565 2c0d 0a20 2020 2020 2020 2029  True,..        )
-0000dde0: 0d0a 0d0a 2020 2020 5d0d 0a29 0d0a 2222  ....    ]..)..""
-0000ddf0: 22e5 9089 e69e 97e6 b7bb e58a a0e6 8890  "...............
-0000de00: e591 98e9 9da2 e69d bf22 2222 0d0a 6a69  ........."""..ji
-0000de10: 6c69 6e5f 7461 626c 6520 3d20 466f 726d  lin_table = Form
-0000de20: 280d 0a20 2020 2074 6974 6c65 3d22 e590  (..    title="..
-0000de30: 89e9 9d92 e9a3 9ee6 89ac 222c 0d0a 2020  ..........",..  
-0000de40: 2020 6d6f 6465 3d44 6973 706c 6179 4d6f    mode=DisplayMo
-0000de50: 6465 456e 756d 2e68 6f72 697a 6f6e 7461  deEnum.horizonta
-0000de60: 6c2c 0d0a 2020 2020 6170 693d 2270 6f73  l,..    api="pos
-0000de70: 743a 2f54 6565 6e53 7475 6479 2f61 7069  t:/TeenStudy/api
-0000de80: 2f6a 696c 696e 2f61 6464 222c 0d0a 2020  /jilin/add",..  
-0000de90: 2020 7265 6469 7265 6374 3d22 2f54 6565    redirect="/Tee
-0000dea0: 6e53 7475 6479 2f6c 6f67 696e 222c 0d0a  nStudy/login",..
-0000deb0: 2020 2020 626f 6479 3d5b 0d0a 2020 2020      body=[..    
-0000dec0: 2020 2020 5365 6c65 6374 280d 0a20 2020      Select(..   
-0000ded0: 2020 2020 2020 2020 206c 6162 656c 3d22           label="
-0000dee0: e7be a4e8 818a 222c 0d0a 2020 2020 2020  ......",..      
-0000def0: 2020 2020 2020 6e61 6d65 3d22 6772 6f75        name="grou
-0000df00: 705f 6964 222c 0d0a 2020 2020 2020 2020  p_id",..        
-0000df10: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
-0000df20: 22e9 9c80 e8a6 81e6 b7bb e58a a0e7 9a84  "...............
-0000df30: e7be a4e7 bb84 222c 0d0a 2020 2020 2020  ......",..      
-0000df40: 2020 2020 2020 6368 6563 6b41 6c6c 3d46        checkAll=F
-0000df50: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
-0000df60: 2020 2073 6f75 7263 653d 2267 6574 3a2f     source="get:/
-0000df70: 5465 656e 5374 7564 792f 6170 692f 6765  TeenStudy/api/ge
-0000df80: 745f 6772 6f75 705f 6c69 7374 222c 0d0a  t_group_list",..
-0000df90: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-0000dfa0: 653d 2727 2c0d 0a20 2020 2020 2020 2020  e='',..         
-0000dfb0: 2020 206d 756c 7469 706c 653d 4661 6c73     multiple=Fals
-0000dfc0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000dfd0: 7265 7175 6972 6564 3d54 7275 652c 0d0a  required=True,..
-0000dfe0: 2020 2020 2020 2020 2020 2020 7365 6172              sear
-0000dff0: 6368 6162 6c65 3d54 7275 652c 0d0a 2020  chable=True,..  
-0000e000: 2020 2020 2020 2020 2020 6a6f 696e 5661            joinVa
-0000e010: 6c75 6573 3d46 616c 7365 2c0d 0a20 2020  lues=False,..   
-0000e020: 2020 2020 2020 2020 2065 7874 7261 6374           extract
-0000e030: 5661 6c75 653d 5472 7565 2c0d 0a20 2020  Value=True,..   
-0000e040: 2020 2020 2020 2020 2073 7461 7469 7374           statist
-0000e050: 6963 733d 5472 7565 2c0d 0a20 2020 2020  ics=True,..     
-0000e060: 2020 2029 2c0d 0a20 2020 2020 2020 2053     ),..        S
-0000e070: 656c 6563 7428 0d0a 2020 2020 2020 2020  elect(..        
-0000e080: 2020 2020 6c61 6265 6c3d 22e7 94a8 e688      label=".....
-0000e090: b749 4422 2c0d 0a20 2020 2020 2020 2020  .ID",..         
-0000e0a0: 2020 206e 616d 653d 2275 7365 725f 6964     name="user_id
-0000e0b0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000e0c0: 6465 7363 7269 7074 696f 6e3d 22e9 9c80  description="...
-0000e0d0: e8a6 81e6 b7bb e58a a0e7 9a84 e794 a8e6  ................
-0000e0e0: 88b7 4944 222c 0d0a 2020 2020 2020 2020  ..ID",..        
-0000e0f0: 2020 2020 6368 6563 6b41 6c6c 3d46 616c      checkAll=Fal
-0000e100: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-0000e110: 2073 6f75 7263 653d 2267 6574 3a2f 5465   source="get:/Te
-0000e120: 656e 5374 7564 792f 6170 692f 6765 745f  enStudy/api/get_
-0000e130: 6d65 6d62 6572 5f6c 6973 743f 6772 6f75  member_list?grou
-0000e140: 705f 6964 3d24 7b67 726f 7570 5f69 647d  p_id=${group_id}
-0000e150: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000e160: 7661 6c75 653d 2727 2c0d 0a20 2020 2020  value='',..     
-0000e170: 2020 2020 2020 206d 756c 7469 706c 653d         multiple=
-0000e180: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-0000e190: 2020 2020 7265 7175 6972 6564 3d54 7275      required=Tru
-0000e1a0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000e1b0: 7365 6172 6368 6162 6c65 3d54 7275 652c  searchable=True,
-0000e1c0: 0d0a 2020 2020 2020 2020 2020 2020 6a6f  ..            jo
-0000e1d0: 696e 5661 6c75 6573 3d46 616c 7365 2c0d  inValues=False,.
-0000e1e0: 0a20 2020 2020 2020 2020 2020 2065 7874  .            ext
-0000e1f0: 7261 6374 5661 6c75 653d 5472 7565 2c0d  ractValue=True,.
-0000e200: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-0000e210: 7469 7374 6963 733d 5472 7565 2c0d 0a20  tistics=True,.. 
-0000e220: 2020 2020 2020 2020 2020 2068 6964 6465             hidde
-0000e230: 6e4f 6e3d 2224 7b67 726f 7570 5f69 643d  nOn="${group_id=
-0000e240: 3d27 273f 7472 7565 3a66 616c 7365 7d22  =''?true:false}"
-0000e250: 0d0a 2020 2020 2020 2020 292c 0d0a 2020  ..        ),..  
-0000e260: 2020 2020 2020 496e 7075 7454 6578 7428        InputText(
-0000e270: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
-0000e280: 6265 6c3d 22e5 9cb0 e58c ba22 2c0d 0a20  bel="......",.. 
-0000e290: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-0000e2a0: 6970 7469 6f6e 3d22 e689 80e5 a484 e79c  iption="........
-0000e2b0: 81e4 bbbd 222c 0d0a 2020 2020 2020 2020  ....",..        
-0000e2c0: 2020 2020 6e61 6d65 3d22 6172 6561 222c      name="area",
-0000e2d0: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-0000e2e0: 6c75 653d 22e5 9089 e69e 9722 2c0d 0a20  lue="......",.. 
-0000e2f0: 2020 2020 2020 2020 2020 2064 6973 6162             disab
-0000e300: 6c65 643d 5472 7565 0d0a 2020 2020 2020  led=True..      
-0000e310: 2020 292c 0d0a 2020 2020 2020 2020 496e    ),..        In
-0000e320: 7075 7454 6578 7428 0d0a 2020 2020 2020  putText(..      
-0000e330: 2020 2020 2020 6c61 6265 6c3d 22e7 99bb        label="...
-0000e340: e5bd 95e5 af86 e7a0 8122 2c0d 0a20 2020  .........",..   
-0000e350: 2020 2020 2020 2020 2074 7970 653d 2769           type='i
-0000e360: 6e70 7574 2d70 6173 7377 6f72 6427 2c0d  nput-password',.
-0000e370: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-0000e380: 6372 6970 7469 6f6e 3d22 e58f afe4 b88d  cription="......
-0000e390: e5a1 abef bc8c e9bb 98e8 aea4 e4b8 bae7  ................
-0000e3a0: 94a8 e688 b749 4422 2c0d 0a20 2020 2020  .....ID",..     
-0000e3b0: 2020 2020 2020 206e 616d 653d 2270 6173         name="pas
-0000e3c0: 7377 6f72 6422 2c0d 0a20 2020 2020 2020  sword",..       
-0000e3d0: 2020 2020 2069 6e6c 696e 653d 4661 6c73       inline=Fals
-0000e3e0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000e3f0: 7265 7175 6972 6564 3d46 616c 7365 2c0d  required=False,.
-0000e400: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-0000e410: 7565 3d22 222c 0d0a 2020 2020 2020 2020  ue="",..        
-0000e420: 2020 2020 636c 6561 7261 626c 653d 5472      clearable=Tr
-0000e430: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-0000e440: 206d 6178 4c65 6e67 7468 3d31 360d 0a20   maxLength=16.. 
-0000e450: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
-0000e460: 2020 2049 6e70 7574 5465 7874 280d 0a20     InputText(.. 
-0000e470: 2020 2020 2020 2020 2020 206c 6162 656c             label
-0000e480: 3d22 e5a7 93e5 908d 222c 0d0a 2020 2020  ="......",..    
-0000e490: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-0000e4a0: 696f 6e3d 22e6 82a8 e79a 84e5 a793 e590  ion="...........
-0000e4b0: 8d22 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
-0000e4c0: 206e 616d 653d 226e 616d 6522 2c0d 0a20   name="name",.. 
-0000e4d0: 2020 2020 2020 2020 2020 2069 6e6c 696e             inlin
-0000e4e0: 653d 4661 6c73 652c 0d0a 2020 2020 2020  e=False,..      
-0000e4f0: 2020 2020 2020 7265 7175 6972 6564 3d54        required=T
-0000e500: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-0000e510: 2020 7661 6c75 653d 2222 2c0d 0a20 2020    value="",..   
-0000e520: 2020 2020 2020 2020 2063 6c65 6172 6162           clearab
-0000e530: 6c65 3d54 7275 652c 0d0a 2020 2020 2020  le=True,..      
-0000e540: 2020 2020 2020 6d61 784c 656e 6774 683d        maxLength=
-0000e550: 380d 0a20 2020 2020 2020 2029 2c0d 0a20  8..        ),.. 
-0000e560: 2020 2020 2020 2049 6e70 7574 5465 7874         InputText
-0000e570: 280d 0a20 2020 2020 2020 2020 2020 206c  (..            l
-0000e580: 6162 656c 3d22 6f70 656e 6964 222c 0d0a  abel="openid",..
-0000e590: 2020 2020 2020 2020 2020 2020 6465 7363              desc
-0000e5a0: 7269 7074 696f 6e3d 22e8 87aa e8a1 8ce6  ription=".......
-0000e5b0: 8a93 e58c 85e8 8eb7 e58f 96ef bc8c e7bb  ................
-0000e5c0: 93e6 9e84 e4b8 ba3a 206f 687a 3978 7878  .......: ohz9xxx
-0000e5d0: 7878 7878 7878 7878 786c 4630 496f 3075  xxxxxxxxxlF0Io0u
-0000e5e0: 436e 4d22 2c0d 0a20 2020 2020 2020 2020  CnM",..         
-0000e5f0: 2020 206e 616d 653d 226f 7065 6e69 6422     name="openid"
-0000e600: 2c0d 0a20 2020 2020 2020 2020 2020 2069  ,..            i
-0000e610: 6e6c 696e 653d 4661 6c73 652c 0d0a 2020  nline=False,..  
-0000e620: 2020 2020 2020 2020 2020 7265 7175 6972            requir
-0000e630: 6564 3d54 7275 652c 0d0a 2020 2020 2020  ed=True,..      
-0000e640: 2020 2020 2020 7661 6c75 653d 2222 2c0d        value="",.
-0000e650: 0a20 2020 2020 2020 2020 2020 2063 6c65  .            cle
-0000e660: 6172 6162 6c65 3d54 7275 652c 0d0a 2020  arable=True,..  
-0000e670: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
-0000e680: 2020 496e 7075 7454 6578 7428 0d0a 2020    InputText(..  
-0000e690: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
-0000e6a0: 22e5 ada6 e6a0 a122 2c0d 0a20 2020 2020  "......",..     
-0000e6b0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-0000e6c0: 6f6e 3d22 e4bd a0e5 b0b1 e8af bbe7 9a84  on="............
-0000e6d0: e9ab 98e6 a0a1 222c 0d0a 2020 2020 2020  ......",..      
-0000e6e0: 2020 2020 2020 6e61 6d65 3d22 756e 6976        name="univ
-0000e6f0: 6572 7369 7479 222c 0d0a 2020 2020 2020  ersity",..      
-0000e700: 2020 2020 2020 696e 6c69 6e65 3d46 616c        inline=Fal
-0000e710: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-0000e720: 2072 6571 7569 7265 643d 5472 7565 2c0d   required=True,.
-0000e730: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-0000e740: 7565 3d22 222c 0d0a 2020 2020 2020 2020  ue="",..        
-0000e750: 2020 2020 636c 6561 7261 626c 653d 5472      clearable=Tr
-0000e760: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-0000e770: 206d 6178 4c65 6e67 7468 3d32 340d 0a20   maxLength=24.. 
-0000e780: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
-0000e790: 2020 2049 6e70 7574 5465 7874 280d 0a20     InputText(.. 
-0000e7a0: 2020 2020 2020 2020 2020 206c 6162 656c             label
-0000e7b0: 3d22 e5ad a6e9 99a2 222c 0d0a 2020 2020  ="......",..    
-0000e7c0: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-0000e7d0: 696f 6e3d 22e5 ada6 e999 a2e5 908d e7a7  ion="...........
-0000e7e0: b022 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
-0000e7f0: 206e 616d 653d 2263 6f6c 6c65 6765 222c   name="college",
-0000e800: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-0000e810: 6c69 6e65 3d46 616c 7365 2c0d 0a20 2020  line=False,..   
-0000e820: 2020 2020 2020 2020 2072 6571 7569 7265           require
-0000e830: 643d 5472 7565 2c0d 0a20 2020 2020 2020  d=True,..       
-0000e840: 2020 2020 2076 616c 7565 3d22 222c 0d0a       value="",..
-0000e850: 2020 2020 2020 2020 2020 2020 636c 6561              clea
-0000e860: 7261 626c 653d 5472 7565 2c0d 0a20 2020  rable=True,..   
-0000e870: 2020 2020 2020 2020 206d 6178 4c65 6e67           maxLeng
-0000e880: 7468 3d33 320d 0a20 2020 2020 2020 2029  th=32..        )
-0000e890: 2c0d 0a20 2020 2020 2020 2049 6e70 7574  ,..        Input
-0000e8a0: 5465 7874 280d 0a20 2020 2020 2020 2020  Text(..         
-0000e8b0: 2020 206c 6162 656c 3d22 e59b a2e6 94af     label="......
-0000e8c0: e983 a822 2c0d 0a20 2020 2020 2020 2020  ...",..         
-0000e8d0: 2020 2064 6573 6372 6970 7469 6f6e 3d22     description="
-0000e8e0: e59b a2e6 94af e983 a87c e78f ade7 baa7  .........|......
-0000e8f0: efbc 8ce6 b2a1 e69c 89e5 8faf e4b8 8de5  ................
-0000e900: a1ab 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
-0000e910: 2020 6e61 6d65 3d22 6f72 6761 6e69 7a61    name="organiza
-0000e920: 7469 6f6e 222c 0d0a 2020 2020 2020 2020  tion",..        
-0000e930: 2020 2020 696e 6c69 6e65 3d46 616c 7365      inline=False
-0000e940: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
-0000e950: 6571 7569 7265 643d 4661 6c73 652c 0d0a  equired=False,..
-0000e960: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-0000e970: 653d 2222 2c0d 0a20 2020 2020 2020 2020  e="",..         
-0000e980: 2020 2063 6c65 6172 6162 6c65 3d54 7275     clearable=Tru
-0000e990: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000e9a0: 6d61 784c 656e 6774 683d 3332 0d0a 2020  maxLength=32..  
-0000e9b0: 2020 2020 2020 290d 0a0d 0a20 2020 205d        )....    ]
-0000e9c0: 0d0a 290d 0a22 2222 e5b9 bfe4 b89c e59c  ..).."""........
-0000e9d0: b0e5 8cba e6b7 bbe5 8aa0 e794 a8e6 88b7  ................
-0000e9e0: 2222 220d 0a67 7561 6e67 646f 6e67 5f74  """..guangdong_t
-0000e9f0: 6162 6c65 203d 2046 6f72 6d28 0d0a 2020  able = Form(..  
-0000ea00: 2020 7469 746c 653d 22e5 b9bf e4b8 9ce5    title=".......
-0000ea10: 85b1 e99d 92e5 9ba2 222c 0d0a 2020 2020  ........",..    
-0000ea20: 6d6f 6465 3d44 6973 706c 6179 4d6f 6465  mode=DisplayMode
-0000ea30: 456e 756d 2e68 6f72 697a 6f6e 7461 6c2c  Enum.horizontal,
-0000ea40: 0d0a 2020 2020 6170 693d 2270 6f73 743a  ..    api="post:
-0000ea50: 2f54 6565 6e53 7475 6479 2f61 7069 2f67  /TeenStudy/api/g
-0000ea60: 7561 6e67 646f 6e67 2f61 6464 222c 0d0a  uangdong/add",..
-0000ea70: 2020 2020 7265 6469 7265 6374 3d22 2f54      redirect="/T
-0000ea80: 6565 6e53 7475 6479 2f6c 6f67 696e 222c  eenStudy/login",
-0000ea90: 0d0a 2020 2020 626f 6479 3d5b 0d0a 2020  ..    body=[..  
-0000eaa0: 2020 2020 2020 416c 6572 7428 6c65 7665        Alert(leve
-0000eab0: 6c3d 4c65 7665 6c45 6e75 6d2e 696e 666f  l=LevelEnum.info
-0000eac0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000ead0: 2063 6c61 7373 4e61 6d65 3d27 7768 6974   className='whit
-0000eae0: 652d 7370 6163 652d 7072 652d 7772 6170  e-space-pre-wrap
-0000eaf0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-0000eb00: 2020 626f 6479 3d28 0d0a 2020 2020 2020    body=(..      
-0000eb10: 2020 2020 2020 2020 2020 2020 22e9 93be              "...
-0000eb20: e68e a5e8 8eb7 e58f 96e6 96b9 e5bc 8f3a  ...............:
-0000eb30: 5c6e 3132 3335 35e9 9d92 e698 a5e4 b98b  \n12355.........
-0000eb40: e5a3 b0e5 85ac e4bc 97e5 8fb7 5c6e e699  ............\n..
-0000eb50: bae6 85a7 e59b a2e5 bbba 2de8 aea4 e8af  ..........-.....
-0000eb60: 81e8 b584 e696 992d e794 9fe6 8890 e794  .......-........
-0000eb70: b5e5 ad90 e59b a2e5 9198 e8af 81ef bc8c  ................
-0000eb80: e782 b9e5 87bb e69c 80e4 b88b e696 b9e7  ................
-0000eb90: 949f e688 90e6 8c89 e992 aee3 8082 5c6e  ..............\n
-0000eba0: e59c a8e5 9ba2 e591 98e8 af81 e9a1 b5e9  ................
-0000ebb0: 9da2 e5a4 8de5 88b6 e993 bee6 8ea5 20e5  .............. .
-0000ebc0: ba94 e4b8 baef bc9a 6874 7470 733a 2f2f  ........https://
-0000ebd0: 7475 616e 2e31 3233 3535 2e6e 6574 2f77  tuan.12355.net/w
-0000ebe0: 6563 6861 742f 7669 6577 2f69 6e66 6f72  echat/view/infor
-0000ebf0: 6d61 7469 6f6e 2f6d 656d 6265 725f 6365  mation/member_ce
-0000ec00: 7274 6966 6963 6174 696f 6e5f 6765 6e65  rtification_gene
-0000ec10: 7261 7465 642e 6874 6d6c 3f6d 656d 6265  rated.html?membe
-0000ec20: 7249 643d 7878 7878 7878 2673 686f 774d  rId=xxxxxx&showM
-0000ec30: 656d 6265 7241 6464 6974 696f 6e4e 616d  emberAdditionNam
-0000ec40: 6573 3d26 7368 6f77 4d65 6d62 6572 5265  es=&showMemberRe
-0000ec50: 7761 7264 4964 733d 2669 7353 686f 7741  wardIds=&isShowA
-0000ec60: 6c6c 4665 653d 7472 7565 205c 6ee5 85b6  llFee=true \n...
-0000ec70: e4b8 ad78 7878 7878 78e5 8db3 e4b8 ba6d  ...xxxxxx......m
-0000ec80: 6964 2229 292c 0d0a 2020 2020 2020 2020  id")),..        
-0000ec90: 5365 6c65 6374 280d 0a20 2020 2020 2020  Select(..       
-0000eca0: 2020 2020 206c 6162 656c 3d22 e7be a4e8       label="....
-0000ecb0: 818a 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
-0000ecc0: 2020 6e61 6d65 3d22 6772 6f75 705f 6964    name="group_id
-0000ecd0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000ece0: 6465 7363 7269 7074 696f 6e3d 22e9 9c80  description="...
-0000ecf0: e8a6 81e6 b7bb e58a a0e7 9a84 e7be a4e7  ................
-0000ed00: bb84 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
-0000ed10: 2020 6368 6563 6b41 6c6c 3d46 616c 7365    checkAll=False
-0000ed20: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
-0000ed30: 6f75 7263 653d 2267 6574 3a2f 5465 656e  ource="get:/Teen
-0000ed40: 5374 7564 792f 6170 692f 6765 745f 6772  Study/api/get_gr
-0000ed50: 6f75 705f 6c69 7374 222c 0d0a 2020 2020  oup_list",..    
-0000ed60: 2020 2020 2020 2020 7661 6c75 653d 2727          value=''
-0000ed70: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
-0000ed80: 756c 7469 706c 653d 4661 6c73 652c 0d0a  ultiple=False,..
-0000ed90: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-0000eda0: 6972 6564 3d54 7275 652c 0d0a 2020 2020  ired=True,..    
-0000edb0: 2020 2020 2020 2020 7365 6172 6368 6162          searchab
-0000edc0: 6c65 3d54 7275 652c 0d0a 2020 2020 2020  le=True,..      
-0000edd0: 2020 2020 2020 6a6f 696e 5661 6c75 6573        joinValues
-0000ede0: 3d46 616c 7365 2c0d 0a20 2020 2020 2020  =False,..       
-0000edf0: 2020 2020 2065 7874 7261 6374 5661 6c75       extractValu
-0000ee00: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
-0000ee10: 2020 2020 2073 7461 7469 7374 6963 733d       statistics=
-0000ee20: 5472 7565 2c0d 0a20 2020 2020 2020 2029  True,..        )
-0000ee30: 2c0d 0a20 2020 2020 2020 2053 656c 6563  ,..        Selec
-0000ee40: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
-0000ee50: 6c61 6265 6c3d 22e7 94a8 e688 b749 4422  label="......ID"
-0000ee60: 2c0d 0a20 2020 2020 2020 2020 2020 206e  ,..            n
-0000ee70: 616d 653d 2275 7365 725f 6964 222c 0d0a  ame="user_id",..
-0000ee80: 2020 2020 2020 2020 2020 2020 6465 7363              desc
-0000ee90: 7269 7074 696f 6e3d 22e9 9c80 e8a6 81e6  ription=".......
-0000eea0: b7bb e58a a0e7 9a84 e794 a8e6 88b7 4944  ..............ID
-0000eeb0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000eec0: 6368 6563 6b41 6c6c 3d46 616c 7365 2c0d  checkAll=False,.
-0000eed0: 0a20 2020 2020 2020 2020 2020 2073 6f75  .            sou
-0000eee0: 7263 653d 2267 6574 3a2f 5465 656e 5374  rce="get:/TeenSt
-0000eef0: 7564 792f 6170 692f 6765 745f 6d65 6d62  udy/api/get_memb
-0000ef00: 6572 5f6c 6973 743f 6772 6f75 705f 6964  er_list?group_id
-0000ef10: 3d24 7b67 726f 7570 5f69 647d 222c 0d0a  =${group_id}",..
-0000ef20: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-0000ef30: 653d 2727 2c0d 0a20 2020 2020 2020 2020  e='',..         
-0000ef40: 2020 206d 756c 7469 706c 653d 4661 6c73     multiple=Fals
-0000ef50: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000ef60: 7265 7175 6972 6564 3d54 7275 652c 0d0a  required=True,..
-0000ef70: 2020 2020 2020 2020 2020 2020 7365 6172              sear
-0000ef80: 6368 6162 6c65 3d54 7275 652c 0d0a 2020  chable=True,..  
-0000ef90: 2020 2020 2020 2020 2020 6a6f 696e 5661            joinVa
-0000efa0: 6c75 6573 3d46 616c 7365 2c0d 0a20 2020  lues=False,..   
-0000efb0: 2020 2020 2020 2020 2065 7874 7261 6374           extract
-0000efc0: 5661 6c75 653d 5472 7565 2c0d 0a20 2020  Value=True,..   
-0000efd0: 2020 2020 2020 2020 2073 7461 7469 7374           statist
-0000efe0: 6963 733d 5472 7565 2c0d 0a20 2020 2020  ics=True,..     
-0000eff0: 2020 2020 2020 2068 6964 6465 6e4f 6e3d         hiddenOn=
-0000f000: 2224 7b67 726f 7570 5f69 643d 3d27 273f  "${group_id==''?
-0000f010: 7472 7565 3a66 616c 7365 7d22 0d0a 2020  true:false}"..  
-0000f020: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
-0000f030: 2020 496e 7075 7454 6578 7428 0d0a 2020    InputText(..  
-0000f040: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
-0000f050: 22e5 9cb0 e58c ba22 2c0d 0a20 2020 2020  "......",..     
-0000f060: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-0000f070: 6f6e 3d22 e689 80e5 a484 e79c 81e4 bbbd  on="............
-0000f080: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000f090: 6e61 6d65 3d22 6172 6561 222c 0d0a 2020  name="area",..  
-0000f0a0: 2020 2020 2020 2020 2020 7661 6c75 653d            value=
-0000f0b0: 22e5 b9bf e4b8 9c22 2c0d 0a20 2020 2020  "......",..     
-0000f0c0: 2020 2020 2020 2064 6973 6162 6c65 643d         disabled=
-0000f0d0: 5472 7565 0d0a 2020 2020 2020 2020 292c  True..        ),
-0000f0e0: 0d0a 2020 2020 2020 2020 496e 7075 7454  ..        InputT
-0000f0f0: 6578 7428 0d0a 2020 2020 2020 2020 2020  ext(..          
-0000f100: 2020 6c61 6265 6c3d 22e7 99bb e5bd 95e5    label=".......
-0000f110: af86 e7a0 8122 2c0d 0a20 2020 2020 2020  .....",..       
-0000f120: 2020 2020 2074 7970 653d 2769 6e70 7574       type='input
-0000f130: 2d70 6173 7377 6f72 6427 2c0d 0a20 2020  -password',..   
-0000f140: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-0000f150: 7469 6f6e 3d22 e58f afe4 b88d e5a1 abef  tion="..........
-0000f160: bc8c e9bb 98e8 aea4 e4b8 bae7 94a8 e688  ................
-0000f170: b749 4422 2c0d 0a20 2020 2020 2020 2020  .ID",..         
-0000f180: 2020 206e 616d 653d 2270 6173 7377 6f72     name="passwor
-0000f190: 6422 2c0d 0a20 2020 2020 2020 2020 2020  d",..           
-0000f1a0: 2069 6e6c 696e 653d 4661 6c73 652c 0d0a   inline=False,..
-0000f1b0: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-0000f1c0: 6972 6564 3d46 616c 7365 2c0d 0a20 2020  ired=False,..   
-0000f1d0: 2020 2020 2020 2020 2076 616c 7565 3d22           value="
-0000f1e0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000f1f0: 636c 6561 7261 626c 653d 5472 7565 2c0d  clearable=True,.
-0000f200: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
-0000f210: 4c65 6e67 7468 3d31 360d 0a20 2020 2020  Length=16..     
-0000f220: 2020 2029 2c0d 0a20 2020 2020 2020 2049     ),..        I
-0000f230: 6e70 7574 5465 7874 280d 0a20 2020 2020  nputText(..     
-0000f240: 2020 2020 2020 206c 6162 656c 3d22 e5a7         label="..
-0000f250: 93e5 908d 222c 0d0a 2020 2020 2020 2020  ....",..        
-0000f260: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
-0000f270: 22e6 82a8 e79a 84e5 a793 e590 8d22 2c0d  "............",.
-0000f280: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
-0000f290: 653d 226e 616d 6522 2c0d 0a20 2020 2020  e="name",..     
-0000f2a0: 2020 2020 2020 2069 6e6c 696e 653d 4661         inline=Fa
-0000f2b0: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
-0000f2c0: 2020 7265 7175 6972 6564 3d54 7275 652c    required=True,
-0000f2d0: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-0000f2e0: 6c75 653d 2222 2c0d 0a20 2020 2020 2020  lue="",..       
-0000f2f0: 2020 2020 2063 6c65 6172 6162 6c65 3d54       clearable=T
-0000f300: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-0000f310: 2020 6d61 784c 656e 6774 683d 380d 0a20    maxLength=8.. 
-0000f320: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
-0000f330: 2020 2049 6e70 7574 5465 7874 280d 0a20     InputText(.. 
-0000f340: 2020 2020 2020 2020 2020 206c 6162 656c             label
-0000f350: 3d22 7572 6c22 2c0d 0a20 2020 2020 2020  ="url",..       
-0000f360: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-0000f370: 3d22 e993 bee6 8ea5 e6a0 bce5 bc8f efbc  ="..............
-0000f380: 9a68 7474 7073 3a2f 2f74 7561 6e2e 3132  .https://tuan.12
-0000f390: 3335 352e 6e65 742f 7765 6368 6174 2f76  355.net/wechat/v
-0000f3a0: 6965 772f 696e 666f 726d 6174 696f 6e2f  iew/information/
-0000f3b0: 6d65 6d62 6572 5f63 6572 7469 6669 6361  member_certifica
-0000f3c0: 7469 6f6e 5f67 656e 6572 6174 6564 2e68  tion_generated.h
-0000f3d0: 746d 6c3f 6d65 6d62 6572 4964 3d78 7878  tml?memberId=xxx
-0000f3e0: 7878 7826 7368 6f77 4d65 6d62 6572 4164  xxx&showMemberAd
-0000f3f0: 6469 7469 6f6e 4e61 6d65 733d 2673 686f  ditionNames=&sho
-0000f400: 774d 656d 6265 7252 6577 6172 6449 6473  wMemberRewardIds
-0000f410: 3d26 6973 5368 6f77 416c 6c46 6565 3d74  =&isShowAllFee=t
-0000f420: 7275 6522 2c0d 0a20 2020 2020 2020 2020  rue",..         
-0000f430: 2020 206e 616d 653d 2275 726c 222c 0d0a     name="url",..
-0000f440: 2020 2020 2020 2020 2020 2020 696e 6c69              inli
-0000f450: 6e65 3d46 616c 7365 2c0d 0a20 2020 2020  ne=False,..     
-0000f460: 2020 2020 2020 2072 6571 7569 7265 643d         required=
-0000f470: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
-0000f480: 2020 2076 616c 7565 3d22 222c 0d0a 2020     value="",..  
-0000f490: 2020 2020 2020 2020 2020 636c 6561 7261            cleara
-0000f4a0: 626c 653d 5472 7565 2c0d 0a20 2020 2020  ble=True,..     
-0000f4b0: 2020 2020 2020 206d 6178 4c65 6e67 7468         maxLength
-0000f4c0: 3d35 3132 0d0a 2020 2020 2020 2020 292c  =512..        ),
-0000f4d0: 0d0a 2020 2020 2020 2020 496e 7075 7454  ..        InputT
-0000f4e0: 6578 7428 0d0a 2020 2020 2020 2020 2020  ext(..          
-0000f4f0: 2020 6c61 6265 6c3d 22e5 ada6 e6a0 a122    label="......"
-0000f500: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
-0000f510: 6573 6372 6970 7469 6f6e 3d22 e4bd a0e5  escription="....
-0000f520: b0b1 e8af bbe7 9a84 e9ab 98e6 a0a1 222c  ..............",
-0000f530: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
-0000f540: 6d65 3d22 756e 6976 6572 7369 7479 222c  me="university",
-0000f550: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-0000f560: 6c69 6e65 3d46 616c 7365 2c0d 0a20 2020  line=False,..   
-0000f570: 2020 2020 2020 2020 2072 6571 7569 7265           require
-0000f580: 643d 5472 7565 2c0d 0a20 2020 2020 2020  d=True,..       
-0000f590: 2020 2020 2076 616c 7565 3d22 222c 0d0a       value="",..
-0000f5a0: 2020 2020 2020 2020 2020 2020 636c 6561              clea
-0000f5b0: 7261 626c 653d 5472 7565 2c0d 0a20 2020  rable=True,..   
-0000f5c0: 2020 2020 2020 2020 206d 6178 4c65 6e67           maxLeng
-0000f5d0: 7468 3d32 340d 0a20 2020 2020 2020 2029  th=24..        )
-0000f5e0: 2c0d 0a20 2020 2020 2020 2049 6e70 7574  ,..        Input
-0000f5f0: 5465 7874 280d 0a20 2020 2020 2020 2020  Text(..         
-0000f600: 2020 206c 6162 656c 3d22 e5ad a6e9 99a2     label="......
-0000f610: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000f620: 6465 7363 7269 7074 696f 6e3d 22e5 ada6  description="...
-0000f630: e999 a2e5 908d e7a7 b022 2c0d 0a20 2020  .........",..   
-0000f640: 2020 2020 2020 2020 206e 616d 653d 2263           name="c
-0000f650: 6f6c 6c65 6765 222c 0d0a 2020 2020 2020  ollege",..      
-0000f660: 2020 2020 2020 696e 6c69 6e65 3d46 616c        inline=Fal
-0000f670: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-0000f680: 2072 6571 7569 7265 643d 5472 7565 2c0d   required=True,.
-0000f690: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-0000f6a0: 7565 3d22 222c 0d0a 2020 2020 2020 2020  ue="",..        
-0000f6b0: 2020 2020 636c 6561 7261 626c 653d 5472      clearable=Tr
-0000f6c0: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-0000f6d0: 206d 6178 4c65 6e67 7468 3d33 320d 0a20   maxLength=32.. 
-0000f6e0: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
-0000f6f0: 2020 2049 6e70 7574 5465 7874 280d 0a20     InputText(.. 
-0000f700: 2020 2020 2020 2020 2020 206c 6162 656c             label
-0000f710: 3d22 e59b a2e6 94af e983 a822 2c0d 0a20  =".........",.. 
-0000f720: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-0000f730: 6970 7469 6f6e 3d22 e59b a2e6 94af e983  iption="........
-0000f740: a87c e78f ade7 baa7 efbc 8ce6 b2a1 e69c  .|..............
-0000f750: 89e5 8faf e4b8 8de5 a1ab 222c 0d0a 2020  ..........",..  
-0000f760: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
-0000f770: 6f72 6761 6e69 7a61 7469 6f6e 222c 0d0a  organization",..
-0000f780: 2020 2020 2020 2020 2020 2020 696e 6c69              inli
-0000f790: 6e65 3d46 616c 7365 2c0d 0a20 2020 2020  ne=False,..     
-0000f7a0: 2020 2020 2020 2072 6571 7569 7265 643d         required=
-0000f7b0: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-0000f7c0: 2020 2020 7661 6c75 653d 2222 2c0d 0a20      value="",.. 
-0000f7d0: 2020 2020 2020 2020 2020 2063 6c65 6172             clear
-0000f7e0: 6162 6c65 3d54 7275 652c 0d0a 2020 2020  able=True,..    
-0000f7f0: 2020 2020 2020 2020 6d61 784c 656e 6774          maxLengt
-0000f800: 683d 3332 0d0a 2020 2020 2020 2020 295d  h=32..        )]
-0000f810: 0d0a 290d 0a22 2222 e9bb 91e9 be99 e6b1  ..).."""........
-0000f820: 9fe5 9cb0 e58c bae6 b7bb e58a a0e6 8890  ................
-0000f830: e591 98e9 9da2 e69d bf22 2222 0d0a 6865  ........."""..he
-0000f840: 696c 6f6e 676a 6961 6e67 5f74 6162 6c65  ilongjiang_table
-0000f850: 203d 2046 6f72 6d28 0d0a 2020 2020 7469   = Form(..    ti
-0000f860: 746c 653d 22e9 bb91 e9be 99e6 b19f e585  tle="...........
-0000f870: b1e9 9d92 e59b a222 2c0d 0a20 2020 206d  .......",..    m
-0000f880: 6f64 653d 4469 7370 6c61 794d 6f64 6545  ode=DisplayModeE
-0000f890: 6e75 6d2e 686f 7269 7a6f 6e74 616c 2c0d  num.horizontal,.
-0000f8a0: 0a20 2020 2061 7069 3d22 706f 7374 3a2f  .    api="post:/
-0000f8b0: 5465 656e 5374 7564 792f 6170 692f 6865  TeenStudy/api/he
-0000f8c0: 696c 6f6e 676a 6961 6e67 2f61 6464 222c  ilongjiang/add",
-0000f8d0: 0d0a 2020 2020 7265 6469 7265 6374 3d22  ..    redirect="
-0000f8e0: 2f54 6565 6e53 7475 6479 2f6c 6f67 696e  /TeenStudy/login
-0000f8f0: 222c 0d0a 2020 2020 626f 6479 3d5b 0d0a  ",..    body=[..
-0000f900: 2020 2020 2020 2020 5365 6c65 6374 280d          Select(.
-0000f910: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-0000f920: 656c 3d22 e7be a4e8 818a 222c 0d0a 2020  el="......",..  
-0000f930: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
-0000f940: 6772 6f75 705f 6964 222c 0d0a 2020 2020  group_id",..    
-0000f950: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-0000f960: 696f 6e3d 22e9 9c80 e8a6 81e6 b7bb e58a  ion="...........
-0000f970: a0e7 9a84 e7be a4e7 bb84 222c 0d0a 2020  ..........",..  
-0000f980: 2020 2020 2020 2020 2020 6368 6563 6b41            checkA
-0000f990: 6c6c 3d46 616c 7365 2c0d 0a20 2020 2020  ll=False,..     
-0000f9a0: 2020 2020 2020 2073 6f75 7263 653d 2267         source="g
-0000f9b0: 6574 3a2f 5465 656e 5374 7564 792f 6170  et:/TeenStudy/ap
-0000f9c0: 692f 6765 745f 6772 6f75 705f 6c69 7374  i/get_group_list
-0000f9d0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000f9e0: 7661 6c75 653d 2727 2c0d 0a20 2020 2020  value='',..     
-0000f9f0: 2020 2020 2020 206d 756c 7469 706c 653d         multiple=
-0000fa00: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-0000fa10: 2020 2020 7265 7175 6972 6564 3d54 7275      required=Tru
-0000fa20: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000fa30: 7365 6172 6368 6162 6c65 3d54 7275 652c  searchable=True,
-0000fa40: 0d0a 2020 2020 2020 2020 2020 2020 6a6f  ..            jo
-0000fa50: 696e 5661 6c75 6573 3d46 616c 7365 2c0d  inValues=False,.
-0000fa60: 0a20 2020 2020 2020 2020 2020 2065 7874  .            ext
-0000fa70: 7261 6374 5661 6c75 653d 5472 7565 2c0d  ractValue=True,.
-0000fa80: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-0000fa90: 7469 7374 6963 733d 5472 7565 2c0d 0a20  tistics=True,.. 
-0000faa0: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
-0000fab0: 2020 2053 656c 6563 7428 0d0a 2020 2020     Select(..    
-0000fac0: 2020 2020 2020 2020 6c61 6265 6c3d 22e7          label=".
-0000fad0: 94a8 e688 b749 4422 2c0d 0a20 2020 2020  .....ID",..     
-0000fae0: 2020 2020 2020 206e 616d 653d 2275 7365         name="use
-0000faf0: 725f 6964 222c 0d0a 2020 2020 2020 2020  r_id",..        
-0000fb00: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
-0000fb10: 22e9 9c80 e8a6 81e6 b7bb e58a a0e7 9a84  "...............
-0000fb20: e794 a8e6 88b7 4944 222c 0d0a 2020 2020  ......ID",..    
-0000fb30: 2020 2020 2020 2020 6368 6563 6b41 6c6c          checkAll
-0000fb40: 3d46 616c 7365 2c0d 0a20 2020 2020 2020  =False,..       
-0000fb50: 2020 2020 2073 6f75 7263 653d 2267 6574       source="get
-0000fb60: 3a2f 5465 656e 5374 7564 792f 6170 692f  :/TeenStudy/api/
-0000fb70: 6765 745f 6d65 6d62 6572 5f6c 6973 743f  get_member_list?
-0000fb80: 6772 6f75 705f 6964 3d24 7b67 726f 7570  group_id=${group
-0000fb90: 5f69 647d 222c 0d0a 2020 2020 2020 2020  _id}",..        
-0000fba0: 2020 2020 7661 6c75 653d 2727 2c0d 0a20      value='',.. 
-0000fbb0: 2020 2020 2020 2020 2020 206d 756c 7469             multi
-0000fbc0: 706c 653d 4661 6c73 652c 0d0a 2020 2020  ple=False,..    
-0000fbd0: 2020 2020 2020 2020 7265 7175 6972 6564          required
-0000fbe0: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
-0000fbf0: 2020 2020 7365 6172 6368 6162 6c65 3d54      searchable=T
-0000fc00: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-0000fc10: 2020 6a6f 696e 5661 6c75 6573 3d46 616c    joinValues=Fal
-0000fc20: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-0000fc30: 2065 7874 7261 6374 5661 6c75 653d 5472   extractValue=Tr
-0000fc40: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-0000fc50: 2073 7461 7469 7374 6963 733d 5472 7565   statistics=True
-0000fc60: 2c0d 0a20 2020 2020 2020 2020 2020 2068  ,..            h
-0000fc70: 6964 6465 6e4f 6e3d 2224 7b67 726f 7570  iddenOn="${group
-0000fc80: 5f69 643d 3d27 273f 7472 7565 3a66 616c  _id==''?true:fal
-0000fc90: 7365 7d22 0d0a 2020 2020 2020 2020 292c  se}"..        ),
-0000fca0: 0d0a 2020 2020 2020 2020 496e 7075 7454  ..        InputT
-0000fcb0: 6578 7428 0d0a 2020 2020 2020 2020 2020  ext(..          
-0000fcc0: 2020 6c61 6265 6c3d 22e5 9cb0 e58c ba22    label="......"
-0000fcd0: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
-0000fce0: 6573 6372 6970 7469 6f6e 3d22 e689 80e5  escription="....
-0000fcf0: a484 e79c 81e4 bbbd 222c 0d0a 2020 2020  ........",..    
-0000fd00: 2020 2020 2020 2020 6e61 6d65 3d22 6172          name="ar
-0000fd10: 6561 222c 0d0a 2020 2020 2020 2020 2020  ea",..          
-0000fd20: 2020 7661 6c75 653d 22e9 bb91 e9be 99e6    value=".......
-0000fd30: b19f 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
-0000fd40: 2020 6469 7361 626c 6564 3d54 7275 650d    disabled=True.
-0000fd50: 0a20 2020 2020 2020 2029 2c0d 0a20 2020  .        ),..   
-0000fd60: 2020 2020 2049 6e70 7574 5465 7874 280d       InputText(.
-0000fd70: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-0000fd80: 656c 3d22 e799 bbe5 bd95 e5af 86e7 a081  el="............
-0000fd90: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000fda0: 7479 7065 3d27 696e 7075 742d 7061 7373  type='input-pass
-0000fdb0: 776f 7264 272c 0d0a 2020 2020 2020 2020  word',..        
-0000fdc0: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
-0000fdd0: 22e5 8faf e4b8 8de5 a1ab efbc 8ce9 bb98  "...............
-0000fde0: e8ae a4e4 b8ba e794 a8e6 88b7 4944 222c  ............ID",
-0000fdf0: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
-0000fe00: 6d65 3d22 7061 7373 776f 7264 222c 0d0a  me="password",..
-0000fe10: 2020 2020 2020 2020 2020 2020 696e 6c69              inli
-0000fe20: 6e65 3d46 616c 7365 2c0d 0a20 2020 2020  ne=False,..     
-0000fe30: 2020 2020 2020 2072 6571 7569 7265 643d         required=
-0000fe40: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-0000fe50: 2020 2020 7661 6c75 653d 2222 2c0d 0a20      value="",.. 
-0000fe60: 2020 2020 2020 2020 2020 2063 6c65 6172             clear
-0000fe70: 6162 6c65 3d54 7275 652c 0d0a 2020 2020  able=True,..    
-0000fe80: 2020 2020 2020 2020 6d61 784c 656e 6774          maxLengt
-0000fe90: 683d 3136 0d0a 2020 2020 2020 2020 292c  h=16..        ),
-0000fea0: 0d0a 2020 2020 2020 2020 496e 7075 7454  ..        InputT
-0000feb0: 6578 7428 0d0a 2020 2020 2020 2020 2020  ext(..          
-0000fec0: 2020 6c61 6265 6c3d 22e5 a793 e590 8d22    label="......"
-0000fed0: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
-0000fee0: 6573 6372 6970 7469 6f6e 3d22 e5af b9e5  escription="....
-0000fef0: ba94 e9bb 91e9 be99 e6b1 9fe5 85b1 e99d  ................
-0000ff00: 92e5 9ba2 e4b8 aae4 baba e4bf a1e6 81af  ................
-0000ff10: e9a1 b520 e682 a8e7 9a84 e5a7 93e5 908d  ... ............
-0000ff20: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000ff30: 6e61 6d65 3d22 6e61 6d65 222c 0d0a 2020  name="name",..  
-0000ff40: 2020 2020 2020 2020 2020 696e 6c69 6e65            inline
-0000ff50: 3d46 616c 7365 2c0d 0a20 2020 2020 2020  =False,..       
-0000ff60: 2020 2020 2072 6571 7569 7265 643d 5472       required=Tr
-0000ff70: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-0000ff80: 2076 616c 7565 3d22 222c 0d0a 2020 2020   value="",..    
-0000ff90: 2020 2020 2020 2020 636c 6561 7261 626c          clearabl
-0000ffa0: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
-0000ffb0: 2020 2020 206d 6178 4c65 6e67 7468 3d38       maxLength=8
-0000ffc0: 0d0a 2020 2020 2020 2020 292c 0d0a 2020  ..        ),..  
-0000ffd0: 2020 2020 2020 496e 7075 7454 6578 7428        InputText(
-0000ffe0: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
-0000fff0: 6265 6c3d 2263 6f6f 6b69 6522 2c0d 0a20  bel="cookie",.. 
-00010000: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-00010010: 6970 7469 6f6e 3d22 e887 aae8 a18c e68a  iption="........
-00010020: 93e5 8c85 e88e b7e5 8f96 efbc 8ce7 bb93  ................
-00010030: e69e 84e4 b8ba efbc 9a53 4553 5349 4f4e  .........SESSION
-00010040: 3d59 3252 685a 5468 6d5a 5455 744d 3251  =Y2RhZThmZTUtM2Q
-00010050: 7a58 5858 5858 5858 5857 4978 4d44 6b74  zXXXXXXXXWIxMDkt
-00010060: 5a6a 4935 5a44 6b32 4e7a 4e6d 4f54 5935  ZjI5ZDk2NzNmOTY5
-00010070: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00010080: 6e61 6d65 3d22 636f 6f6b 6965 222c 0d0a  name="cookie",..
-00010090: 2020 2020 2020 2020 2020 2020 696e 6c69              inli
-000100a0: 6e65 3d46 616c 7365 2c0d 0a20 2020 2020  ne=False,..     
-000100b0: 2020 2020 2020 2072 6571 7569 7265 643d         required=
-000100c0: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
-000100d0: 2020 2076 616c 7565 3d22 222c 0d0a 2020     value="",..  
-000100e0: 2020 2020 2020 2020 2020 636c 6561 7261            cleara
-000100f0: 626c 653d 5472 7565 2c0d 0a20 2020 2020  ble=True,..     
-00010100: 2020 2029 0d0a 0d0a 2020 2020 5d0d 0a29     )....    ]..)
-00010110: 0d0a 2222 22e6 8ea8 e980 81e7 bea4 e881  .."""...........
-00010120: 8ae6 a8a1 e69d bf22 2222 0d0a 7075 7368  ......."""..push
-00010130: 5f74 6162 6c65 203d 2043 5255 4428 6d6f  _table = CRUD(mo
-00010140: 6465 3d27 7461 626c 6527 2c0d 0a20 2020  de='table',..   
-00010150: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00010160: 6974 6c65 3d27 272c 0d0a 2020 2020 2020  itle='',..      
-00010170: 2020 2020 2020 2020 2020 2020 7379 6e63              sync
-00010180: 4c6f 6361 7469 6f6e 3d46 616c 7365 2c0d  Location=False,.
-00010190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000101a0: 2020 2061 7069 3d27 2f54 6565 6e53 7475     api='/TeenStu
-000101b0: 6479 2f61 7069 2f67 6574 5f70 7573 685f  dy/api/get_push_
-000101c0: 6c69 7374 272c 0d0a 2020 2020 2020 2020  list',..        
-000101d0: 2020 2020 2020 2020 2020 7479 7065 3d27            type='
-000101e0: 6372 7564 272c 0d0a 2020 2020 2020 2020  crud',..        
-000101f0: 2020 2020 2020 2020 2020 6865 6164 6572            header
-00010200: 546f 6f6c 6261 723d 5b41 6374 696f 6e54  Toolbar=[ActionT
-00010210: 7970 652e 416a 6178 286c 6162 656c 3d27  ype.Ajax(label='
-00010220: e588 a0e9 99a4 e689 80e6 9c89 e68e a8e9  ................
-00010230: 8081 e7be a4e8 818a 272c 0d0a 2020 2020  ........',..    
-00010240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010260: 2020 2020 2020 2020 2020 2020 206c 6576               lev
-00010270: 656c 3d4c 6576 656c 456e 756d 2e77 6172  el=LevelEnum.war
-00010280: 6e69 6e67 2c0d 0a20 2020 2020 2020 2020  ning,..         
-00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102b0: 2020 2020 2020 2020 636f 6e66 6972 6d54          confirmT
-000102c0: 6578 743d 27e7 a1ae e5ae 9ae8 a681 e588  ext='...........
-000102d0: a0e9 99a4 e689 80e6 9c89 e68e a8e9 8081  ................
-000102e0: e7be a4e8 818a e590 97ef bc9f 272c 0d0a  ............',..
-000102f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010320: 2061 7069 3d27 6465 6c65 7465 3a2f 5465   api='delete:/Te
-00010330: 656e 5374 7564 792f 6170 692f 6465 6c65  enStudy/api/dele
-00010340: 7465 5f61 6c6c 3f74 7970 653d 7075 7368  te_all?type=push
-00010350: 5f6c 6973 7427 292c 0d0a 2020 2020 2020  _list'),..      
-00010360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010370: 2020 2020 2020 2020 2020 2022 6275 6c6b             "bulk
-00010380: 4163 7469 6f6e 7322 2c20 2272 656c 6f61  Actions", "reloa
-00010390: 6422 2c20 4163 7469 6f6e 5479 7065 2e44  d", ActionType.D
-000103a0: 6961 6c6f 6728 0d0a 2020 2020 2020 2020  ialog(..        
-000103b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103c0: 2020 6c61 6265 6c3d 27e6 b7bb e58a a0e6    label='.......
-000103d0: 8ea8 e980 81e7 bea4 e881 8a27 2c0d 0a20  ...........',.. 
-000103e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103f0: 2020 2020 2020 2020 206c 6576 656c 3d4c           level=L
-00010400: 6576 656c 456e 756d 2e69 6e66 6f2c 0d0a  evelEnum.info,..
-00010410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010420: 2020 2020 2020 2020 2020 6963 6f6e 3d27            icon='
-00010430: 6661 2066 612d 706c 7573 272c 0d0a 2020  fa fa-plus',..  
-00010440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010450: 2020 2020 2020 2020 6469 616c 6f67 3d44          dialog=D
-00010460: 6961 6c6f 6728 7469 746c 653d 27e6 b7bb  ialog(title='...
-00010470: e58a a0e6 8ea8 e980 81e7 bea4 e881 8a27  ...............'
-00010480: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00010490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104a0: 2020 2020 2020 2020 2020 2073 697a 653d             size=
-000104b0: 276c 6727 2c0d 0a20 2020 2020 2020 2020  'lg',..         
-000104c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104d0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-000104e0: 6f64 793d 5b0d 0a20 2020 2020 2020 2020  ody=[..         
-000104f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010510: 2020 2046 6f72 6d28 7469 746c 653d 2727     Form(title=''
-00010520: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00010530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010550: 2020 2020 6170 693d 2770 6f73 743a 2f54      api='post:/T
-00010560: 6565 6e53 7475 6479 2f61 7069 2f61 6464  eenStudy/api/add
-00010570: 5f70 7573 6827 2c0d 0a20 2020 2020 2020  _push',..       
-00010580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105a0: 2020 2020 2020 2020 2020 7375 626d 6974            submit
-000105b0: 5465 7874 3d27 e6b7 bbe5 8aa0 272c 0d0a  Text='......',..
-000105c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105f0: 206d 6f64 653d 4469 7370 6c61 794d 6f64   mode=DisplayMod
-00010600: 6545 6e75 6d2e 686f 7269 7a6f 6e74 616c  eEnum.horizontal
-00010610: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00010620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010640: 2020 2020 6c61 6265 6c41 6c69 676e 3d27      labelAlign='
-00010650: 7269 6768 7427 2c0d 0a20 2020 2020 2020  right',..       
-00010660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010680: 2020 2020 2020 2020 2020 626f 6479 3d5b            body=[
-00010690: 5365 6c65 6374 280d 0a20 2020 2020 2020  Select(..       
-000106a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106c0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-000106d0: 6265 6c3d 22e7 bea4 e881 8a22 2c0d 0a20  bel="......",.. 
-000106e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010710: 2020 2020 6e61 6d65 3d22 6772 6f75 7073      name="groups
-00010720: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00010730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010750: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-00010760: 7469 6f6e 3d22 e99c 80e8 a681 e68e a8e9  tion="..........
-00010770: 8081 e79a 84e7 bea4 e7bb 8422 2c0d 0a20  ...........",.. 
-00010780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107b0: 2020 2020 6368 6563 6b41 6c6c 3d54 7275      checkAll=Tru
-000107c0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-000107d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107f0: 2020 2020 2020 2020 2073 6f75 7263 653d           source=
-00010800: 2267 6574 3a2f 5465 656e 5374 7564 792f  "get:/TeenStudy/
-00010810: 6170 692f 6765 745f 6772 6f75 705f 6c69  api/get_group_li
-00010820: 7374 222c 0d0a 2020 2020 2020 2020 2020  st",..          
-00010830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010850: 2020 2020 2020 2020 2020 2076 616c 7565             value
-00010860: 3d27 272c 0d0a 2020 2020 2020 2020 2020  ='',..          
-00010870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010890: 2020 2020 2020 2020 2020 206d 756c 7469             multi
-000108a0: 706c 653d 5472 7565 2c0d 0a20 2020 2020  ple=True,..     
-000108b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108e0: 7265 7175 6972 6564 3d54 7275 652c 0d0a  required=True,..
-000108f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010920: 2020 2020 2073 6561 7263 6861 626c 653d       searchable=
-00010930: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
-00010940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010960: 2020 2020 2020 2020 2020 2020 6a6f 696e              join
-00010970: 5661 6c75 6573 3d46 616c 7365 2c0d 0a20  Values=False,.. 
-00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109b0: 2020 2020 6578 7472 6163 7456 616c 7565      extractValue
-000109c0: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
-000109d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109f0: 2020 2020 2020 2020 2020 2020 2073 7461               sta
-00010a00: 7469 7374 6963 733d 5472 7565 2c0d 0a20  tistics=True,.. 
-00010a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00010a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a70: 2020 2020 5d29 5d29 0d0a 2020 2020 2020      ])])..      
-00010a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a90: 295d 2c0d 0a20 2020 2020 2020 2020 2020  )],..           
-00010aa0: 2020 2020 2020 2069 7465 6d41 6374 696f         itemActio
-00010ab0: 6e73 3d5b 0d0a 2020 2020 2020 2020 2020  ns=[..          
-00010ac0: 2020 2020 2020 2020 2020 2020 4163 7469              Acti
-00010ad0: 6f6e 5479 7065 2e41 6a61 7828 746f 6f6c  onType.Ajax(tool
-00010ae0: 7469 703d 27e5 88a0 e999 a427 2c0d 0a20  tip='......',.. 
-00010af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b10: 2020 2020 2069 636f 6e3d 2766 6120 6661       icon='fa fa
-00010b20: 2d74 696d 6573 2074 6578 742d 6461 6e67  -times text-dang
-00010b30: 6572 272c 0d0a 2020 2020 2020 2020 2020  er',..          
-00010b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b50: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-00010b60: 6972 6d54 6578 743d 27e5 88a0 e999 a4e8  irmText='.......
-00010b70: afa5 e68e a8e9 8081 e7be a4e8 818a e590  ................
-00010b80: 9727 2c0d 0a20 2020 2020 2020 2020 2020  .',..           
-00010b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ba0: 2020 2020 2020 2020 2020 2061 7069 3d27             api='
-00010bb0: 6465 6c65 7465 3a2f 5465 656e 5374 7564  delete:/TeenStud
-00010bc0: 792f 6170 692f 6465 6c65 7465 5f70 7573  y/api/delete_pus
-00010bd0: 683f 6964 3d24 7b69 647d 2729 0d0a 2020  h?id=${id}')..  
-00010be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010bf0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00010c00: 2020 2020 2020 666f 6f74 6162 6c65 3d54        footable=T
-00010c10: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
-00010c20: 2020 2020 2020 2020 636f 6c75 6d6e 733d          columns=
-00010c30: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
-00010c40: 2020 2020 2020 2020 2054 6162 6c65 436f           TableCo
-00010c50: 6c75 6d6e 286c 6162 656c 3d27 e695 b0e6  lumn(label='....
-00010c60: 8dae e5ba 9349 4427 2c20 6e61 6d65 3d27  .....ID', name='
-00010c70: 6964 2729 2c0d 0a20 2020 2020 2020 2020  id'),..         
-00010c80: 2020 2020 2020 2020 2020 2020 2054 6162               Tab
-00010c90: 6c65 436f 6c75 6d6e 286c 6162 656c 3d27  leColumn(label='
-00010ca0: e69c bae5 99a8 e4ba ba49 4427 2c20 6e61  .........ID', na
-00010cb0: 6d65 3d27 7365 6c66 5f69 6427 2c20 7365  me='self_id', se
-00010cc0: 6172 6368 6162 6c65 3d54 7275 652c 2029  archable=True, )
-00010cd0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00010ce0: 2020 2020 2020 2020 2054 6162 6c65 436f           TableCo
-00010cf0: 6c75 6d6e 286c 6162 656c 3d27 e980 9ae7  lumn(label='....
-00010d00: 9fa5 e7be a4e5 8fb7 272c 206e 616d 653d  ........', name=
-00010d10: 2767 726f 7570 5f69 6427 292c 0d0a 2020  'group_id'),..  
-00010d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d30: 2020 2020 5461 626c 6543 6f6c 756d 6e28      TableColumn(
-00010d40: 6c61 6265 6c3d 27e6 b7bb e58a a0e4 baba  label='.........
-00010d50: e591 9827 2c20 6e61 6d65 3d27 7573 6572  ...', name='user
-00010d60: 5f69 6427 2c20 7365 6172 6368 6162 6c65  _id', searchable
-00010d70: 3d54 7275 652c 2029 2c0d 0a20 2020 2020  =True, ),..     
-00010d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d90: 2054 6162 6c65 436f 6c75 6d6e 286c 6162   TableColumn(lab
-00010da0: 656c 3d27 e68f 90e4 baa4 e78a b6e6 8081  el='............
-00010db0: 272c 206e 616d 653d 2724 7b73 7461 7475  ', name='${statu
-00010dc0: 733d 3d74 7275 653f 22e5 bc80 e590 af22  s==true?"......"
-00010dd0: 3a22 e585 b3e9 97ad 227d 272c 2073 6561  :"......"}', sea
-00010de0: 7263 6861 626c 653d 5472 7565 2c20 292c  rchable=True, ),
-00010df0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010e00: 2020 2020 2020 2020 5461 626c 6543 6f6c          TableCol
-00010e10: 756d 6e28 7479 7065 3d27 7470 6c27 2c20  umn(type='tpl', 
-00010e20: 7470 6c3d 2724 7b74 696d 657c 6461 7465  tpl='${time|date
-00010e30: 3a59 5959 592d 4d4d 2d44 4420 4848 5c5c  :YYYY-MM-DD HH\\
-00010e40: 3a6d 6d5c 5c3a 7373 7d27 2c0d 0a20 2020  :mm\\:ss}',..   
-00010e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e60: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00010e70: 6162 656c 3d27 e6b7 bbe5 8aa0 e697 b6e9  abel='..........
-00010e80: 97b4 272c 0d0a 2020 2020 2020 2020 2020  ..',..          
-00010e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ea0: 2020 2020 2020 2020 6e61 6d65 3d27 7469          name='ti
-00010eb0: 6d65 272c 2073 6f72 7461 626c 653d 5472  me', sortable=Tr
-00010ec0: 7565 290d 0a20 2020 2020 2020 2020 2020  ue)..           
-00010ed0: 2020 2020 2020 205d 2c0d 0a20 2020 2020         ],..     
-00010ee0: 2020 2020 2020 2020 2020 2020 2062 756c               bul
-00010ef0: 6b41 6374 696f 6e73 3d5b 0d0a 2020 2020  kActions=[..    
-00010f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f10: 2020 4163 7469 6f6e 5479 7065 2e41 6a61    ActionType.Aja
-00010f20: 7828 6c61 6265 6c3d 27e6 89b9 e987 8fe5  x(label='.......
-00010f30: 88a0 e999 a427 2c0d 0a20 2020 2020 2020  .....',..       
-00010f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f50: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00010f60: 6576 656c 3d4c 6576 656c 456e 756d 2e77  evel=LevelEnum.w
-00010f70: 6172 6e69 6e67 2c0d 0a20 2020 2020 2020  arning,..       
-00010f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00010fa0: 6f6e 6669 726d 5465 7874 3d22 e7a1 aee5  onfirmText="....
-00010fb0: ae9a e8a6 81e6 89b9 e987 8fe5 88a0 e999  ................
-00010fc0: a4ef bc9f 222c 0d0a 2020 2020 2020 2020  ....",..        
-00010fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fe0: 2020 2020 2020 2020 2020 2020 2020 6170                ap
-00010ff0: 693d 2264 656c 6574 653a 2f54 6565 6e53  i="delete:/TeenS
-00011000: 7475 6479 2f61 7069 2f64 656c 6574 655f  tudy/api/delete_
-00011010: 7075 7368 3f69 6473 3d24 7b69 6473 7c72  push?ids=${ids|r
-00011020: 6177 7d22 295d 290d 0a70 6167 655f 6465  aw}")])..page_de
-00011030: 7461 696c 203d 2050 6167 6528 7469 746c  tail = Page(titl
-00011040: 653d 2727 2c20 626f 6479 3d5b 6c6f 676f  e='', body=[logo
-00011050: 2c20 7374 6174 7573 5d29 0d0a 6164 6d69  , status])..admi
-00011060: 6e5f 7061 6765 203d 2050 6167 6553 6368  n_page = PageSch
-00011070: 656d 6128 7572 6c3d 272f 6164 6d69 6e27  ema(url='/admin'
-00011080: 2c20 6c61 6265 6c3d 27e9 a696 e9a1 b527  , label='......'
-00011090: 2c20 6963 6f6e 3d27 6661 2066 612d 686f  , icon='fa fa-ho
-000110a0: 6d65 272c 2069 7344 6566 6175 6c74 5061  me', isDefaultPa
-000110b0: 6765 3d54 7275 652c 2073 6368 656d 613d  ge=True, schema=
-000110c0: 7061 6765 5f64 6574 6169 6c29 0d0a 2222  page_detail)..""
-000110d0: 22e6 8890 e591 98e5 8897 e8a1 a8e9 a1b5  "...............
-000110e0: 2222 220d 0a6c 6973 745f 7061 6765 203d  """..list_page =
-000110f0: 2050 6167 6553 6368 656d 6128 7572 6c3d   PageSchema(url=
-00011100: 272f 6c69 7374 272c 2069 636f 6e3d 2766  '/list', icon='f
-00011110: 6120 6661 2d6c 6973 742d 756c 272c 206c  a fa-list-ul', l
-00011120: 6162 656c 3d27 e688 90e5 9198 e588 97e8  abel='..........
-00011130: a1a8 272c 0d0a 2020 2020 2020 2020 2020  ..',..          
-00011140: 2020 2020 2020 2020 2020 2020 2073 6368               sch
-00011150: 656d 613d 5061 6765 2874 6974 6c65 3d27  ema=Page(title='
-00011160: e688 90e5 9198 e588 97e8 a1a8 272c 2062  ............', b
-00011170: 6f64 793d 5b63 6172 6473 5f63 7572 645d  ody=[cards_curd]
-00011180: 2929 0d0a 6875 6265 695f 7061 6765 203d  ))..hubei_page =
-00011190: 2050 6167 6553 6368 656d 6128 7572 6c3d   PageSchema(url=
-000111a0: 272f 6164 642f 6875 6265 6927 2c20 6963  '/add/hubei', ic
-000111b0: 6f6e 3d27 6661 2066 612d 7065 6e2d 746f  on='fa fa-pen-to
-000111c0: 2d73 7175 6172 6527 2c20 6c61 6265 6c3d  -square', label=
-000111d0: 27e9 9d92 e698 a5e6 b996 e58c 9727 2c0d  '............',.
-000111e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000111f0: 2020 2020 2020 2020 2073 6368 656d 613d           schema=
-00011200: 5061 6765 2874 6974 6c65 3d27 e99d 92e6  Page(title='....
-00011210: 98a5 e6b9 96e5 8c97 272c 2062 6f64 793d  ........', body=
-00011220: 5b68 7562 6569 5f74 6162 6c65 5d29 290d  [hubei_table])).
-00011230: 0a6a 6961 6e67 7869 5f70 6167 6520 3d20  .jiangxi_page = 
-00011240: 5061 6765 5363 6865 6d61 2875 726c 3d27  PageSchema(url='
-00011250: 2f61 6464 2f6a 6961 6e67 7869 272c 2069  /add/jiangxi', i
-00011260: 636f 6e3d 2766 6120 6661 2d70 656e 2d74  con='fa fa-pen-t
-00011270: 6f2d 7371 7561 7265 272c 206c 6162 656c  o-square', label
-00011280: 3d27 e6b1 9fe8 a5bf e585 b1e9 9d92 e59b  ='..............
-00011290: a227 2c0d 0a20 2020 2020 2020 2020 2020  .',..           
-000112a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000112b0: 6368 656d 613d 5061 6765 2874 6974 6c65  chema=Page(title
-000112c0: 3d27 e6b1 9fe8 a5bf e585 b1e9 9d92 e59b  ='..............
-000112d0: a227 2c20 626f 6479 3d5b 6a69 616e 6778  .', body=[jiangx
-000112e0: 695f 7461 626c 655d 2929 0d0a 6a69 616e  i_table]))..jian
-000112f0: 6773 755f 7061 6765 203d 2050 6167 6553  gsu_page = PageS
-00011300: 6368 656d 6128 7572 6c3d 272f 6164 642f  chema(url='/add/
-00011310: 6a69 616e 6773 7527 2c20 6963 6f6e 3d27  jiangsu', icon='
-00011320: 6661 2066 612d 7065 6e2d 746f 2d73 7175  fa fa-pen-to-squ
-00011330: 6172 6527 2c20 6c61 6265 6c3d 27e6 b19f  are', label='...
-00011340: e88b 8fe5 85b1 e99d 92e5 9ba2 272c 0d0a  ............',..
-00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011360: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
-00011370: 3d50 6167 6528 7469 746c 653d 27e6 b19f  =Page(title='...
-00011380: e88b 8fe5 85b1 e99d 92e5 9ba2 272c 2062  ............', b
-00011390: 6f64 793d 5b6a 6961 6e67 7375 5f74 6162  ody=[jiangsu_tab
-000113a0: 6c65 5d29 290d 0a61 6e68 7569 5f70 6167  le]))..anhui_pag
-000113b0: 6520 3d20 5061 6765 5363 6865 6d61 2875  e = PageSchema(u
-000113c0: 726c 3d27 2f61 6464 2f61 6e68 7569 272c  rl='/add/anhui',
-000113d0: 2069 636f 6e3d 2766 6120 6661 2d70 656e   icon='fa fa-pen
-000113e0: 2d74 6f2d 7371 7561 7265 272c 206c 6162  -to-square', lab
-000113f0: 656c 3d27 e5ae 89e5 bebd e585 b1e9 9d92  el='............
-00011400: e59b a227 2c0d 0a20 2020 2020 2020 2020  ...',..         
-00011410: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011420: 6368 656d 613d 5061 6765 2874 6974 6c65  chema=Page(title
-00011430: 3d27 e5ae 89e5 bebd e585 b1e9 9d92 e59b  ='..............
-00011440: a227 2c20 626f 6479 3d5b 616e 6875 695f  .', body=[anhui_
-00011450: 7461 626c 655d 2929 0d0a 7369 6368 7561  table]))..sichua
-00011460: 6e5f 7061 6765 203d 2050 6167 6553 6368  n_page = PageSch
-00011470: 656d 6128 7572 6c3d 272f 6164 642f 7369  ema(url='/add/si
-00011480: 6368 7561 6e27 2c20 6963 6f6e 3d27 6661  chuan', icon='fa
-00011490: 2066 612d 7065 6e2d 746f 2d73 7175 6172   fa-pen-to-squar
-000114a0: 6527 2c20 6c61 6265 6c3d 27e5 a4a9 e5ba  e', label='.....
-000114b0: 9ce6 96b0 e99d 92e5 b9b4 272c 0d0a 2020  ..........',..  
-000114c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114d0: 2020 2020 2020 2020 7363 6865 6d61 3d50          schema=P
-000114e0: 6167 6528 7469 746c 653d 27e5 a4a9 e5ba  age(title='.....
-000114f0: 9ce6 96b0 e99d 92e5 b9b4 272c 2062 6f64  ..........', bod
-00011500: 793d 5b73 6963 6875 616e 5f74 6162 6c65  y=[sichuan_table
-00011510: 5d29 290d 0a73 6861 6e64 6f6e 675f 7061  ]))..shandong_pa
-00011520: 6765 203d 2050 6167 6553 6368 656d 6128  ge = PageSchema(
-00011530: 7572 6c3d 272f 6164 642f 7368 616e 646f  url='/add/shando
-00011540: 6e67 272c 2069 636f 6e3d 2766 6120 6661  ng', icon='fa fa
-00011550: 2d70 656e 2d74 6f2d 7371 7561 7265 272c  -pen-to-square',
-00011560: 206c 6162 656c 3d27 e99d 92e6 98a5 e5b1   label='........
-00011570: b1e4 b89c 272c 0d0a 2020 2020 2020 2020  ....',..        
-00011580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011590: 2020 2073 6368 656d 613d 5061 6765 2874     schema=Page(t
-000115a0: 6974 6c65 3d27 e99d 92e6 98a5 e5b1 b1e4  itle='..........
-000115b0: b89c 272c 2062 6f64 793d 5b73 6861 6e64  ..', body=[shand
-000115c0: 6f6e 675f 7461 626c 655d 2929 0d0a 6368  ong_table]))..ch
-000115d0: 6f6e 6771 696e 675f 7061 6765 203d 2050  ongqing_page = P
-000115e0: 6167 6553 6368 656d 6128 7572 6c3d 272f  ageSchema(url='/
-000115f0: 6164 642f 6368 6f6e 6771 696e 6727 2c20  add/chongqing', 
-00011600: 6963 6f6e 3d27 6661 2066 612d 7065 6e2d  icon='fa fa-pen-
-00011610: 746f 2d73 7175 6172 6527 2c20 6c61 6265  to-square', labe
-00011620: 6c3d 27e9 878d e5ba 86e5 85b1 e99d 92e5  l='.............
-00011630: 9ba2 272c 0d0a 2020 2020 2020 2020 2020  ..',..          
-00011640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011650: 2020 7363 6865 6d61 3d50 6167 6528 7469    schema=Page(ti
-00011660: 746c 653d 27e9 878d e5ba 86e5 85b1 e99d  tle='...........
-00011670: 92e5 9ba2 272c 2062 6f64 793d 5b63 686f  ....', body=[cho
-00011680: 6e67 7169 6e67 5f74 6162 6c65 5d29 290d  ngqing_table])).
-00011690: 0a6a 696c 696e 5f70 6167 6520 3d20 5061  .jilin_page = Pa
-000116a0: 6765 5363 6865 6d61 2875 726c 3d27 2f61  geSchema(url='/a
-000116b0: 6464 2f6a 696c 696e 272c 2069 636f 6e3d  dd/jilin', icon=
-000116c0: 2766 6120 6661 2d70 656e 2d74 6f2d 7371  'fa fa-pen-to-sq
-000116d0: 7561 7265 272c 206c 6162 656c 3d27 e590  uare', label='..
-000116e0: 89e9 9d92 e9a3 9ee6 89ac 272c 0d0a 2020  ..........',..  
-000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011700: 2020 2020 2020 7363 6865 6d61 3d50 6167        schema=Pag
-00011710: 6528 7469 746c 653d 27e5 9089 e99d 92e9  e(title='.......
-00011720: a39e e689 ac27 2c20 626f 6479 3d5b 6a69  .....', body=[ji
-00011730: 6c69 6e5f 7461 626c 655d 2929 0d0a 6775  lin_table]))..gu
-00011740: 616e 6764 6f6e 675f 7061 6765 203d 2050  angdong_page = P
-00011750: 6167 6553 6368 656d 6128 7572 6c3d 272f  ageSchema(url='/
-00011760: 6164 642f 6775 616e 6764 6f6e 6727 2c20  add/guangdong', 
-00011770: 6963 6f6e 3d27 6661 2066 612d 7065 6e2d  icon='fa fa-pen-
-00011780: 746f 2d73 7175 6172 6527 2c20 6c61 6265  to-square', labe
-00011790: 6c3d 27e5 b9bf e4b8 9ce5 85b1 e99d 92e5  l='.............
-000117a0: 9ba2 272c 0d0a 2020 2020 2020 2020 2020  ..',..          
-000117b0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-000117c0: 6865 6d61 3d50 6167 6528 7469 746c 653d  hema=Page(title=
-000117d0: 27e5 b9bf e4b8 9ce5 85b1 e99d 92e5 9ba2  '...............
-000117e0: 272c 2062 6f64 793d 5b67 7561 6e67 646f  ', body=[guangdo
-000117f0: 6e67 5f74 6162 6c65 5d29 290d 0a68 6569  ng_table]))..hei
-00011800: 6c6f 6e67 6a69 616e 675f 7061 6765 203d  longjiang_page =
-00011810: 2050 6167 6553 6368 656d 6128 7572 6c3d   PageSchema(url=
-00011820: 272f 6164 642f 6865 696c 6f6e 676a 6961  '/add/heilongjia
-00011830: 6e67 272c 2069 636f 6e3d 2766 6120 6661  ng', icon='fa fa
-00011840: 2d70 656e 2d74 6f2d 7371 7561 7265 272c  -pen-to-square',
-00011850: 206c 6162 656c 3d27 e9bb 91e9 be99 e6b1   label='........
-00011860: 9fe5 85b1 e99d 92e5 9ba2 272c 0d0a 2020  ..........',..  
-00011870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011880: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
-00011890: 3d50 6167 6528 7469 746c 653d 27e9 bb91  =Page(title='...
-000118a0: e9be 99e6 b19f e585 b1e9 9d92 e59b a227  ...............'
-000118b0: 2c20 626f 6479 3d5b 6865 696c 6f6e 676a  , body=[heilongj
-000118c0: 6961 6e67 5f74 6162 6c65 5d29 290d 0a61  iang_table]))..a
-000118d0: 646d 696e 5f61 7070 203d 2041 7070 2862  dmin_app = App(b
-000118e0: 7261 6e64 4e61 6d65 3d27 5465 656e 5374  randName='TeenSt
-000118f0: 7564 7927 2c0d 0a20 2020 2020 2020 2020  udy',..         
-00011900: 2020 2020 2020 206c 6f67 6f3d 2768 7474         logo='htt
-00011910: 7073 3a2f 2f69 2e33 3238 3838 382e 7879  ps://i.328888.xy
-00011920: 7a2f 3230 3233 2f30 322f 3233 2f78 4968  z/2023/02/23/xIh
-00011930: 356b 2e70 6e67 272c 0d0a 2020 2020 2020  5k.png',..      
-00011940: 2020 2020 2020 2020 2020 6865 6164 6572            header
-00011950: 3d68 6561 6465 722c 0d0a 2020 2020 2020  =header,..      
-00011960: 2020 2020 2020 2020 2020 7061 6765 733d            pages=
-00011970: 5b7b 0d0a 2020 2020 2020 2020 2020 2020  [{..            
-00011980: 2020 2020 2020 2020 2763 6869 6c64 7265          'childre
-00011990: 6e27 3a20 5b0d 0a20 2020 2020 2020 2020  n': [..         
-000119a0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000119b0: 646d 696e 5f70 6167 652c 0d0a 2020 2020  dmin_page,..    
-000119c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119d0: 2020 2020 5061 6765 5363 6865 6d61 2869      PageSchema(i
-000119e0: 636f 6e3d 2766 6120 6661 2d63 6972 636c  con='fa fa-circl
-000119f0: 652d 7573 6572 272c 206c 6162 656c 3d27  e-user', label='
-00011a00: e688 90e5 9198 e7ae a1e7 9086 272c 0d0a  ............',..
-00011a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a30: 2020 2063 6869 6c64 7265 6e3d 5b6c 6973     children=[lis
-00011a40: 745f 7061 6765 2c20 6875 6265 695f 7061  t_page, hubei_pa
-00011a50: 6765 2c20 6a69 616e 6778 695f 7061 6765  ge, jiangxi_page
-00011a60: 2c20 6a69 616e 6773 755f 7061 6765 2c20  , jiangsu_page, 
-00011a70: 616e 6875 695f 7061 6765 2c0d 0a20 2020  anhui_page,..   
-00011a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011aa0: 2020 2020 2020 2020 2020 7369 6368 7561            sichua
-00011ab0: 6e5f 7061 6765 2c20 7368 616e 646f 6e67  n_page, shandong
-00011ac0: 5f70 6167 652c 2063 686f 6e67 7169 6e67  _page, chongqing
-00011ad0: 5f70 6167 652c 206a 696c 696e 5f70 6167  _page, jilin_pag
-00011ae0: 652c 6775 616e 6764 6f6e 675f 7061 6765  e,guangdong_page
-00011af0: 2c68 6569 6c6f 6e67 6a69 616e 675f 7061  ,heilongjiang_pa
-00011b00: 6765 5d29 2c0d 0a20 2020 2020 2020 2020  ge]),..         
-00011b10: 2020 2020 2020 2020 2020 2020 2020 2050                 P
-00011b20: 6167 6553 6368 656d 6128 7572 6c3d 222f  ageSchema(url="/
-00011b30: 6e6f 7469 6365 222c 206c 6162 656c 3d27  notice", label='
-00011b40: e68e a8e9 8081 e588 97e8 a1a8 272c 2069  ............', i
-00011b50: 636f 6e3d 2766 6120 6661 2d62 656c 6c27  con='fa fa-bell'
-00011b60: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00011b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b80: 2020 2020 2020 7363 6865 6d61 3d50 6167        schema=Pag
-00011b90: 6528 7469 746c 653d 2727 2c20 626f 6479  e(title='', body
-00011ba0: 3d5b 7075 7368 5f74 6162 6c65 5d29 292c  =[push_table])),
-00011bb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011bc0: 2020 2020 2020 2020 2020 5061 6765 5363            PageSc
-00011bd0: 6865 6d61 2875 726c 3d22 2f72 6571 7565  hema(url="/reque
-00011be0: 7374 222c 206c 6162 656c 3d27 e794 b3e8  st", label='....
-00011bf0: afb7 e8ae b0e5 bd95 272c 2069 636f 6e3d  ........', icon=
-00011c00: 2766 6120 6661 2d63 6972 636c 652d 696e  'fa fa-circle-in
-00011c10: 666f 272c 0d0a 2020 2020 2020 2020 2020  fo',..          
-00011c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c30: 2020 2020 2020 2020 2073 6368 656d 613d           schema=
-00011c40: 5061 6765 2874 6974 6c65 3d27 272c 2062  Page(title='', b
-00011c50: 6f64 793d 5b72 6571 7565 7374 5f74 6162  ody=[request_tab
-00011c60: 6c65 5d29 292c 0d0a 2020 2020 2020 2020  le])),..        
-00011c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c80: 5061 6765 5363 6865 6d61 2875 726c 3d22  PageSchema(url="
-00011c90: 2f61 6e73 7765 7222 2c20 6c61 6265 6c3d  /answer", label=
-00011ca0: 27e5 a4a7 e5ad a6e4 b9a0 e588 97e8 a1a8  '...............
-00011cb0: 272c 2069 636f 6e3d 2766 6120 6661 2d62  ', icon='fa fa-b
-00011cc0: 6f6f 6b2d 6f70 656e 272c 0d0a 2020 2020  ook-open',..    
-00011cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ce0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011cf0: 6368 656d 613d 5061 6765 2874 6974 6c65  chema=Page(title
-00011d00: 3d27 272c 2062 6f64 793d 5b61 6e73 7765  ='', body=[answe
-00011d10: 725f 7461 626c 655d 2929 2c0d 0a20 2020  r_table])),..   
-00011d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d30: 2020 2020 2050 6167 6553 6368 656d 6128       PageSchema(
-00011d40: 7572 6c3d 222f 7265 636f 7264 7322 2c20  url="/records", 
-00011d50: 6c61 6265 6c3d 27e6 8f90 e4ba a4e8 aeb0  label='.........
-00011d60: e5bd 9527 2c20 6963 6f6e 3d27 6661 2066  ...', icon='fa f
-00011d70: 612d 636f 6465 2d63 6f6d 6d69 7427 2c0d  a-code-commit',.
-00011d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011da0: 2020 2020 7363 6865 6d61 3d50 6167 6528      schema=Page(
-00011db0: 7469 746c 653d 2727 2c20 626f 6479 3d5b  title='', body=[
-00011dc0: 7265 636f 7264 5f74 6162 6c65 5d29 292c  record_table])),
-00011dd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011de0: 2020 2020 2020 2020 2020 5061 6765 5363            PageSc
-00011df0: 6865 6d61 2875 726c 3d22 2f73 6574 7469  hema(url="/setti
-00011e00: 6e67 222c 206c 6162 656c 3d27 e985 8de7  ng", label='....
-00011e10: bdae 272c 2069 636f 6e3d 2766 6120 6661  ..', icon='fa fa
-00011e20: 2d67 6561 7227 2c0d 0a20 2020 2020 2020  -gear',..       
-00011e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e40: 2020 2020 2020 2020 2020 2020 7363 6865              sche
-00011e50: 6d61 3d50 6167 6528 7469 746c 653d 2727  ma=Page(title=''
-00011e60: 2c20 626f 6479 3d5b 7365 7474 696e 675f  , body=[setting_
-00011e70: 7461 626c 655d 2929 2c0d 0a20 2020 2020  table])),..     
-00011e80: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00011e90: 7d5d 2c0d 0a20 2020 2020 2020 2020 2020  }],..           
-00011ea0: 2020 2020 2066 6f6f 7465 723d 4874 6d6c       footer=Html
-00011eb0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00011ec0: 2020 2020 2020 2068 746d 6c3d 6627 3c64         html=f'<d
-00011ed0: 6976 2063 6c61 7373 3d22 702d 3220 7465  iv class="p-2 te
-00011ee0: 7874 2d63 656e 7465 7220 6267 2d62 6c75  xt-center bg-blu
-00011ef0: 652d 3130 3022 3e43 6f70 7972 6967 6874  e-100">Copyright
-00011f00: 20c2 a920 3230 3232 202d 2032 3032 3320   .. 2022 - 2023 
-00011f10: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00011f20: 2f67 6974 6875 622e 636f 6d2f 5a4d 3235  /github.com/ZM25
-00011f30: 5843 2f54 6565 6e53 7475 6479 2220 7461  XC/TeenStudy" ta
-00011f40: 7267 6574 3d22 5f62 6c61 6e6b 2220 636c  rget="_blank" cl
-00011f50: 6173 733d 226c 696e 6b2d 7365 636f 6e64  ass="link-second
-00011f60: 6172 7922 3e54 6565 6e53 7475 6479 3c2f  ary">TeenStudy</
-00011f70: 613e 2058 3c61 2074 6172 6765 743d 225f  a> X<a target="_
-00011f80: 626c 616e 6b22 2068 7265 663d 2268 7474  blank" href="htt
-00011f90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00011fa0: 6261 6964 752f 616d 6973 2220 636c 6173  baidu/amis" clas
-00011fb0: 733d 226c 696e 6b2d 7365 636f 6e64 6172  s="link-secondar
-00011fc0: 7922 2072 656c 3d22 6e6f 6f70 656e 6572  y" rel="noopener
-00011fd0: 223e 2061 6d69 7320 7632 2e32 2e30 3c2f  "> amis v2.2.0</
-00011fe0: 613e 3c2f 6469 763e 2729 290d 0a         a></div>'))..
+00002a20: 6a6f 696e 5661 6c75 6573 3d46 616c 7365  joinValues=False
+00002a30: 2c0d 0a20 2020 2020 2020 2020 2020 2065  ,..            e
+00002a40: 7874 7261 6374 5661 6c75 653d 5472 7565  xtractValue=True
+00002a50: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
+00002a60: 7461 7469 7374 6963 733d 5472 7565 2c0d  tatistics=True,.
+00002a70: 0a20 2020 2020 2020 2029 2c0d 0a20 2020  .        ),..   
+00002a80: 2020 2020 2053 656c 6563 7428 0d0a 2020       Select(..  
+00002a90: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
+00002aa0: 22e7 94a8 e688 b749 4422 2c0d 0a20 2020  "......ID",..   
+00002ab0: 2020 2020 2020 2020 206e 616d 653d 2275           name="u
+00002ac0: 7365 725f 6964 222c 0d0a 2020 2020 2020  ser_id",..      
+00002ad0: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00002ae0: 6e3d 22e9 9c80 e8a6 81e6 b7bb e58a a0e7  n=".............
+00002af0: 9a84 e794 a8e6 88b7 4944 222c 0d0a 2020  ........ID",..  
+00002b00: 2020 2020 2020 2020 2020 6368 6563 6b41            checkA
+00002b10: 6c6c 3d46 616c 7365 2c0d 0a20 2020 2020  ll=False,..     
+00002b20: 2020 2020 2020 2073 6f75 7263 653d 2267         source="g
+00002b30: 6574 3a2f 5465 656e 5374 7564 792f 6170  et:/TeenStudy/ap
+00002b40: 692f 6765 745f 6d65 6d62 6572 5f6c 6973  i/get_member_lis
+00002b50: 743f 6772 6f75 705f 6964 3d24 7b67 726f  t?group_id=${gro
+00002b60: 7570 5f69 647d 222c 0d0a 2020 2020 2020  up_id}",..      
+00002b70: 2020 2020 2020 7661 6c75 653d 2727 2c0d        value='',.
+00002b80: 0a20 2020 2020 2020 2020 2020 206d 756c  .            mul
+00002b90: 7469 706c 653d 4661 6c73 652c 0d0a 2020  tiple=False,..  
+00002ba0: 2020 2020 2020 2020 2020 7265 7175 6972            requir
+00002bb0: 6564 3d54 7275 652c 0d0a 2020 2020 2020  ed=True,..      
+00002bc0: 2020 2020 2020 7365 6172 6368 6162 6c65        searchable
+00002bd0: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+00002be0: 2020 2020 6a6f 696e 5661 6c75 6573 3d46      joinValues=F
+00002bf0: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
+00002c00: 2020 2065 7874 7261 6374 5661 6c75 653d     extractValue=
+00002c10: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+00002c20: 2020 2073 7461 7469 7374 6963 733d 5472     statistics=Tr
+00002c30: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
+00002c40: 2068 6964 6465 6e4f 6e3d 2224 7b67 726f   hiddenOn="${gro
+00002c50: 7570 5f69 643d 3d27 273f 7472 7565 3a66  up_id==''?true:f
+00002c60: 616c 7365 7d22 0d0a 2020 2020 2020 2020  alse}"..        
+00002c70: 292c 0d0a 2020 2020 2020 2020 496e 7075  ),..        Inpu
+00002c80: 7454 6578 7428 0d0a 2020 2020 2020 2020  tText(..        
+00002c90: 2020 2020 6c61 6265 6c3d 22e5 9cb0 e58c      label=".....
+00002ca0: ba22 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
+00002cb0: 2064 6573 6372 6970 7469 6f6e 3d22 e689   description="..
+00002cc0: 80e5 a484 e79c 81e4 bbbd 222c 0d0a 2020  ..........",..  
+00002cd0: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
+00002ce0: 6172 6561 222c 0d0a 2020 2020 2020 2020  area",..        
+00002cf0: 2020 2020 7661 6c75 653d 22e6 b996 e58c      value=".....
+00002d00: 9722 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
+00002d10: 2064 6973 6162 6c65 643d 5472 7565 0d0a   disabled=True..
+00002d20: 2020 2020 2020 2020 292c 0d0a 2020 2020          ),..    
+00002d30: 2020 2020 496e 7075 7454 6578 7428 0d0a      InputText(..
+00002d40: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+00002d50: 6c3d 22e7 99bb e5bd 95e5 af86 e7a0 8122  l="............"
+00002d60: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
+00002d70: 7970 653d 2769 6e70 7574 2d70 6173 7377  ype='input-passw
+00002d80: 6f72 6427 2c0d 0a20 2020 2020 2020 2020  ord',..         
+00002d90: 2020 2064 6573 6372 6970 7469 6f6e 3d22     description="
+00002da0: e58f afe4 b88d e5a1 abef bc8c e9bb 98e8  ................
+00002db0: aea4 e4b8 bae7 94a8 e688 b749 4422 2c0d  ...........ID",.
+00002dc0: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+00002dd0: 653d 2270 6173 7377 6f72 6422 2c0d 0a20  e="password",.. 
+00002de0: 2020 2020 2020 2020 2020 2069 6e6c 696e             inlin
+00002df0: 653d 4661 6c73 652c 0d0a 2020 2020 2020  e=False,..      
+00002e00: 2020 2020 2020 7265 7175 6972 6564 3d46        required=F
+00002e10: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
+00002e20: 2020 2076 616c 7565 3d22 222c 0d0a 2020     value="",..  
+00002e30: 2020 2020 2020 2020 2020 636c 6561 7261            cleara
+00002e40: 626c 653d 5472 7565 2c0d 0a20 2020 2020  ble=True,..     
+00002e50: 2020 2020 2020 206d 6178 4c65 6e67 7468         maxLength
+00002e60: 3d31 360d 0a20 2020 2020 2020 2029 2c0d  =16..        ),.
+00002e70: 0a20 2020 2020 2020 2049 6e70 7574 5465  .        InputTe
+00002e80: 7874 280d 0a20 2020 2020 2020 2020 2020  xt(..           
+00002e90: 206c 6162 656c 3d22 e5a7 93e5 908d 222c   label="......",
+00002ea0: 0d0a 2020 2020 2020 2020 2020 2020 6465  ..            de
+00002eb0: 7363 7269 7074 696f 6e3d 22e5 afb9 e5ba  scription=".....
+00002ec0: 94e9 9d92 e698 a5e6 b996 e58c 97e4 b8aa  ................
+00002ed0: e4ba bae4 bfa1 e681 afe9 a1b5 20e6 82a8  ............ ...
+00002ee0: e79a 84e5 a793 e590 8d22 2c0d 0a20 2020  .........",..   
+00002ef0: 2020 2020 2020 2020 206e 616d 653d 226e           name="n
+00002f00: 616d 6522 2c0d 0a20 2020 2020 2020 2020  ame",..         
+00002f10: 2020 2069 6e6c 696e 653d 4661 6c73 652c     inline=False,
+00002f20: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00002f30: 7175 6972 6564 3d54 7275 652c 0d0a 2020  quired=True,..  
+00002f40: 2020 2020 2020 2020 2020 7661 6c75 653d            value=
+00002f50: 2222 2c0d 0a20 2020 2020 2020 2020 2020  "",..           
+00002f60: 2063 6c65 6172 6162 6c65 3d54 7275 652c   clearable=True,
+00002f70: 0d0a 2020 2020 2020 2020 2020 2020 6d61  ..            ma
+00002f80: 784c 656e 6774 683d 380d 0a20 2020 2020  xLength=8..     
+00002f90: 2020 2029 2c0d 0a20 2020 2020 2020 2049     ),..        I
+00002fa0: 6e70 7574 5465 7874 280d 0a20 2020 2020  nputText(..     
+00002fb0: 2020 2020 2020 206c 6162 656c 3d22 e794         label="..
+00002fc0: a8e6 88b7 e7bc 96e5 8fb7 222c 0d0a 2020  ..........",..  
+00002fd0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+00002fe0: 7074 696f 6e3d 22e5 afb9 e5ba 94e9 9d92  ption=".........
+00002ff0: e698 a5e6 b996 e58c 97e4 b8aa e4ba bae4  ................
+00003000: bfa1 e681 afe9 a1b5 20e7 94a8 e688 b7e7  ........ .......
+00003010: bc96 e58f b722 2c0d 0a20 2020 2020 2020  .....",..       
+00003020: 2020 2020 206e 616d 653d 2264 7878 5f69       name="dxx_i
+00003030: 6422 2c0d 0a20 2020 2020 2020 2020 2020  d",..           
+00003040: 2069 6e6c 696e 653d 4661 6c73 652c 0d0a   inline=False,..
+00003050: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+00003060: 6972 6564 3d54 7275 652c 0d0a 2020 2020  ired=True,..    
+00003070: 2020 2020 2020 2020 7661 6c75 653d 2222          value=""
+00003080: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
+00003090: 6c65 6172 6162 6c65 3d54 7275 652c 0d0a  learable=True,..
+000030a0: 2020 2020 2020 2020 2020 2020 6d61 784c              maxL
+000030b0: 656e 6774 683d 390d 0a20 2020 2020 2020  ength=9..       
+000030c0: 2029 2c0d 0a20 2020 2020 2020 2049 6e70   ),..        Inp
+000030d0: 7574 5465 7874 280d 0a20 2020 2020 2020  utText(..       
+000030e0: 2020 2020 206c 6162 656c 3d22 e5ad a6e6       label="....
+000030f0: a0a1 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
+00003100: 2020 6465 7363 7269 7074 696f 6e3d 22e5    description=".
+00003110: afb9 e5ba 94e9 9d92 e698 a5e6 b996 e58c  ................
+00003120: 97e5 a1ab e586 99e4 bfa1 e681 afe9 a1b5  ................
+00003130: 20e9 ab98 e6a0 a122 2c0d 0a20 2020 2020   ......",..     
+00003140: 2020 2020 2020 206e 616d 653d 2275 6e69         name="uni
+00003150: 7665 7273 6974 7922 2c0d 0a20 2020 2020  versity",..     
+00003160: 2020 2020 2020 2069 6e6c 696e 653d 4661         inline=Fa
+00003170: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+00003180: 2020 7265 7175 6972 6564 3d54 7275 652c    required=True,
+00003190: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
+000031a0: 6c75 653d 2222 2c0d 0a20 2020 2020 2020  lue="",..       
+000031b0: 2020 2020 2063 6c65 6172 6162 6c65 3d54       clearable=T
+000031c0: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+000031d0: 2020 6d61 784c 656e 6774 683d 3234 0d0a    maxLength=24..
+000031e0: 2020 2020 2020 2020 292c 0d0a 2020 2020          ),..    
+000031f0: 2020 2020 496e 7075 7454 6578 7428 0d0a      InputText(..
+00003200: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+00003210: 6c3d 22e5 ada6 e999 a222 2c0d 0a20 2020  l="......",..   
+00003220: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+00003230: 7469 6f6e 3d22 e5af b9e5 ba94 e99d 92e6  tion="..........
+00003240: 98a5 e6b9 96e5 8c97 e5a1 abe5 8699 e4bf  ................
+00003250: a1e6 81af e9a1 b520 e999 a2e7 b3bb 222c  ....... ......",
+00003260: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
+00003270: 6d65 3d22 636f 6c6c 6567 6522 2c0d 0a20  me="college",.. 
+00003280: 2020 2020 2020 2020 2020 2069 6e6c 696e             inlin
+00003290: 653d 4661 6c73 652c 0d0a 2020 2020 2020  e=False,..      
+000032a0: 2020 2020 2020 7265 7175 6972 6564 3d54        required=T
+000032b0: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+000032c0: 2020 7661 6c75 653d 2222 2c0d 0a20 2020    value="",..   
+000032d0: 2020 2020 2020 2020 2063 6c65 6172 6162           clearab
+000032e0: 6c65 3d54 7275 652c 0d0a 2020 2020 2020  le=True,..      
+000032f0: 2020 2020 2020 6d61 784c 656e 6774 683d        maxLength=
+00003300: 3332 0d0a 2020 2020 2020 2020 292c 0d0a  32..        ),..
+00003310: 2020 2020 2020 2020 496e 7075 7454 6578          InputTex
+00003320: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+00003330: 6c61 6265 6c3d 22e5 9ba2 e694 afe9 83a8  label=".........
+00003340: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00003350: 6465 7363 7269 7074 696f 6e3d 22e5 afb9  description="...
+00003360: e5ba 94e9 9d92 e698 a5e6 b996 e58c 97e5  ................
+00003370: a1ab e586 99e4 bfa1 e681 afe9 a1b5 20e9  .............. .
+00003380: 8089 e68b a9e7 bb84 e7bb 8722 2c0d 0a20  ...........",.. 
+00003390: 2020 2020 2020 2020 2020 206e 616d 653d             name=
+000033a0: 226f 7267 616e 697a 6174 696f 6e22 2c0d  "organization",.
+000033b0: 0a20 2020 2020 2020 2020 2020 2069 6e6c  .            inl
+000033c0: 696e 653d 4661 6c73 652c 0d0a 2020 2020  ine=False,..    
+000033d0: 2020 2020 2020 2020 7265 7175 6972 6564          required
+000033e0: 3d46 616c 7365 2c0d 0a20 2020 2020 2020  =False,..       
+000033f0: 2020 2020 2076 616c 7565 3d22 222c 0d0a       value="",..
+00003400: 2020 2020 2020 2020 2020 2020 636c 6561              clea
+00003410: 7261 626c 653d 5472 7565 2c0d 0a20 2020  rable=True,..   
+00003420: 2020 2020 2020 2020 206d 6178 4c65 6e67           maxLeng
+00003430: 7468 3d33 320d 0a20 2020 2020 2020 2029  th=32..        )
+00003440: 0d0a 0d0a 2020 2020 5d0d 0a29 0d0a 2222  ....    ]..)..""
+00003450: 22e6 b19f e8a5 bfe6 b7bb e58a a0e6 8890  "...............
+00003460: e591 98e9 9da2 e69d bf22 2222 0d0a 6a69  ........."""..ji
+00003470: 616e 6778 695f 7461 626c 6520 3d20 466f  angxi_table = Fo
+00003480: 726d 280d 0a20 2020 2074 6974 6c65 3d22  rm(..    title="
+00003490: e6b7 bbe5 8aa0 e6b1 9fe8 a5bf e585 b1e9  ................
+000034a0: 9d92 e59b a2e7 94a8 e688 b722 2c0d 0a20  ...........",.. 
+000034b0: 2020 2073 7562 6d69 7454 6578 743d 22e6     submitText=".
+000034c0: b7bb e58a a022 2c0d 0a20 2020 206d 6f64  .....",..    mod
+000034d0: 653d 4469 7370 6c61 794d 6f64 6545 6e75  e=DisplayModeEnu
+000034e0: 6d2e 686f 7269 7a6f 6e74 616c 2c0d 0a20  m.horizontal,.. 
+000034f0: 2020 2061 7069 3d22 706f 7374 3a2f 5465     api="post:/Te
+00003500: 656e 5374 7564 792f 6170 692f 6164 6422  enStudy/api/add"
+00003510: 2c0d 0a20 2020 2072 6573 6574 4166 7465  ,..    resetAfte
+00003520: 7253 7562 6d69 743d 5472 7565 2c0d 0a20  rSubmit=True,.. 
+00003530: 2020 2062 6f64 793d 5b0d 0a20 2020 2020     body=[..     
+00003540: 2020 2053 656c 6563 7428 0d0a 2020 2020     Select(..    
+00003550: 2020 2020 2020 2020 6c61 6265 6c3d 22e7          label=".
+00003560: bea4 e881 8a22 2c0d 0a20 2020 2020 2020  .....",..       
+00003570: 2020 2020 206e 616d 653d 2267 726f 7570       name="group
+00003580: 5f69 6422 2c0d 0a20 2020 2020 2020 2020  _id",..         
+00003590: 2020 2064 6573 6372 6970 7469 6f6e 3d22     description="
+000035a0: e99c 80e8 a681 e6b7 bbe5 8aa0 e79a 84e7  ................
+000035b0: bea4 e7bb 8422 2c0d 0a20 2020 2020 2020  .....",..       
+000035c0: 2020 2020 2063 6865 636b 416c 6c3d 4661       checkAll=Fa
+000035d0: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+000035e0: 2020 736f 7572 6365 3d22 6765 743a 2f54    source="get:/T
+000035f0: 6565 6e53 7475 6479 2f61 7069 2f67 6574  eenStudy/api/get
+00003600: 5f67 726f 7570 5f6c 6973 7422 2c0d 0a20  _group_list",.. 
+00003610: 2020 2020 2020 2020 2020 2076 616c 7565             value
+00003620: 3d27 272c 0d0a 2020 2020 2020 2020 2020  ='',..          
+00003630: 2020 6d75 6c74 6970 6c65 3d46 616c 7365    multiple=False
+00003640: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+00003650: 6571 7569 7265 643d 5472 7565 2c0d 0a20  equired=True,.. 
+00003660: 2020 2020 2020 2020 2020 2073 6561 7263             searc
+00003670: 6861 626c 653d 5472 7565 2c0d 0a20 2020  hable=True,..   
+00003680: 2020 2020 2020 2020 206a 6f69 6e56 616c           joinVal
+00003690: 7565 733d 4661 6c73 652c 0d0a 2020 2020  ues=False,..    
+000036a0: 2020 2020 2020 2020 6578 7472 6163 7456          extractV
+000036b0: 616c 7565 3d54 7275 652c 0d0a 2020 2020  alue=True,..    
+000036c0: 2020 2020 2020 2020 7374 6174 6973 7469          statisti
+000036d0: 6373 3d54 7275 652c 0d0a 2020 2020 2020  cs=True,..      
+000036e0: 2020 292c 0d0a 2020 2020 2020 2020 5365    ),..        Se
+000036f0: 6c65 6374 280d 0a20 2020 2020 2020 2020  lect(..         
+00003700: 2020 206c 6162 656c 3d22 e794 a8e6 88b7     label="......
+00003710: 4944 222c 0d0a 2020 2020 2020 2020 2020  ID",..          
+00003720: 2020 6e61 6d65 3d22 7573 6572 5f69 6422    name="user_id"
+00003730: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
+00003740: 6573 6372 6970 7469 6f6e 3d22 e99c 80e8  escription="....
+00003750: a681 e6b7 bbe5 8aa0 e79a 84e7 94a8 e688  ................
+00003760: b749 4422 2c0d 0a20 2020 2020 2020 2020  .ID",..         
+00003770: 2020 2063 6865 636b 416c 6c3d 4661 6c73     checkAll=Fals
+00003780: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00003790: 736f 7572 6365 3d22 6765 743a 2f54 6565  source="get:/Tee
+000037a0: 6e53 7475 6479 2f61 7069 2f67 6574 5f6d  nStudy/api/get_m
+000037b0: 656d 6265 725f 6c69 7374 3f67 726f 7570  ember_list?group
+000037c0: 5f69 643d 247b 6772 6f75 705f 6964 7d22  _id=${group_id}"
+000037d0: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
+000037e0: 616c 7565 3d27 272c 0d0a 2020 2020 2020  alue='',..      
+000037f0: 2020 2020 2020 6d75 6c74 6970 6c65 3d46        multiple=F
+00003800: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
+00003810: 2020 2072 6571 7569 7265 643d 5472 7565     required=True
+00003820: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
+00003830: 6561 7263 6861 626c 653d 5472 7565 2c0d  earchable=True,.
+00003840: 0a20 2020 2020 2020 2020 2020 206a 6f69  .            joi
+00003850: 6e56 616c 7565 733d 4661 6c73 652c 0d0a  nValues=False,..
+00003860: 2020 2020 2020 2020 2020 2020 6578 7472              extr
+00003870: 6163 7456 616c 7565 3d54 7275 652c 0d0a  actValue=True,..
+00003880: 2020 2020 2020 2020 2020 2020 7374 6174              stat
+00003890: 6973 7469 6373 3d54 7275 652c 0d0a 2020  istics=True,..  
+000038a0: 2020 2020 2020 2020 2020 6869 6464 656e            hidden
+000038b0: 4f6e 3d22 7468 6973 2e67 726f 7570 5f69  On="this.group_i
+000038c0: 643d 3d27 273f 7472 7565 3a66 616c 7365  d==''?true:false
+000038d0: 220d 0a20 2020 2020 2020 2029 2c0d 0a20  "..        ),.. 
+000038e0: 2020 2020 2020 2049 6e70 7574 5465 7874         InputText
+000038f0: 280d 0a20 2020 2020 2020 2020 2020 206c  (..            l
+00003900: 6162 656c 3d22 e59c b0e5 8cba 222c 0d0a  abel="......",..
+00003910: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+00003920: 7269 7074 696f 6e3d 22e6 8980 e5a4 84e7  ription=".......
+00003930: 9c81 e4bb bd22 2c0d 0a20 2020 2020 2020  .....",..       
+00003940: 2020 2020 206e 616d 653d 2261 7265 6122       name="area"
+00003950: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
+00003960: 616c 7565 3d22 e6b1 9fe8 a5bf 222c 0d0a  alue="......",..
+00003970: 2020 2020 2020 2020 2020 2020 6469 7361              disa
+00003980: 626c 6564 3d54 7275 650d 0a20 2020 2020  bled=True..     
+00003990: 2020 2029 2c0d 0a20 2020 2020 2020 2049     ),..        I
+000039a0: 6e70 7574 5465 7874 280d 0a20 2020 2020  nputText(..     
+000039b0: 2020 2020 2020 206c 6162 656c 3d22 e794         label="..
+000039c0: a8e6 88b7 e7bc 96e5 8fb7 222c 0d0a 2020  ..........",..  
+000039d0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+000039e0: 7074 696f 6e3d 22e5 9ba2 e7bb 84e7 bb87  ption=".........
+000039f0: 4944 efbc 8ce6 97a0 e99c 80e5 a1ab e586  ID..............
+00003a00: 9922 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
+00003a10: 206e 616d 653d 2264 7878 5f69 6422 2c0d   name="dxx_id",.
+00003a20: 0a20 2020 2020 2020 2020 2020 2069 6e6c  .            inl
+00003a30: 696e 653d 4661 6c73 652c 0d0a 2020 2020  ine=False,..    
+00003a40: 2020 2020 2020 2020 7265 7175 6972 6564          required
+00003a50: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+00003a60: 2020 2020 7661 6c75 653d 2224 7b49 4628      value="${IF(
+00003a70: 4953 454d 5054 5928 6f72 6761 6e69 7a61  ISEMPTY(organiza
+00003a80: 7469 6f6e 292c 5350 4c49 5428 636f 6c6c  tion),SPLIT(coll
+00003a90: 6567 652c 272d 2729 5b31 5d2c 5350 4c49  ege,'-')[1],SPLI
+00003aa0: 5428 6f72 6761 6e69 7a61 7469 6f6e 2c27  T(organization,'
+00003ab0: 2d27 295b 315d 297d 222c 0d0a 2020 2020  -')[1])}",..    
+00003ac0: 2020 2020 2020 2020 6469 7361 626c 6564          disabled
+00003ad0: 3d54 7275 650d 0a20 2020 2020 2020 2029  =True..        )
+00003ae0: 2c0d 0a20 2020 2020 2020 2053 656c 6563  ,..        Selec
+00003af0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+00003b00: 7479 7065 3d22 7365 6c65 6374 222c 0d0a  type="select",..
+00003b10: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+00003b20: 6c3d 22e5 ada6 e6a0 a1e7 b1bb e59e 8b22  l="............"
+00003b30: 2c0d 0a20 2020 2020 2020 2020 2020 206e  ,..            n
+00003b40: 616d 653d 2275 6e69 7665 7273 6974 795f  ame="university_
+00003b50: 7479 7065 222c 0d0a 2020 2020 2020 2020  type",..        
+00003b60: 2020 2020 7365 6172 6368 6162 6c65 3d54      searchable=T
+00003b70: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+00003b80: 2020 7265 7175 6972 6564 3d54 7275 652c    required=True,
+00003b90: 0d0a 2020 2020 2020 2020 2020 2020 636c  ..            cl
+00003ba0: 6561 7261 626c 653d 5472 7565 2c0d 0a20  earable=True,.. 
+00003bb0: 2020 2020 2020 2020 2020 206f 7074 696f             optio
+00003bc0: 6e73 3d5b 0d0a 2020 2020 2020 2020 2020  ns=[..          
+00003bd0: 2020 2020 2020 7b27 6c61 6265 6c27 3a20        {'label': 
+00003be0: 22e5 9ba2 e79c 81e5 a794 e69c bae5 85b3  "...............
+00003bf0: 222c 2022 7661 6c75 6522 3a20 22e5 9ba2  ", "value": "...
+00003c00: e79c 81e5 a794 e69c bae5 85b3 2d4e 3030  ............-N00
+00003c10: 3137 227d 2c0d 0a20 2020 2020 2020 2020  17"},..         
+00003c20: 2020 2020 2020 207b 276c 6162 656c 273a         {'label':
+00003c30: 2022 e79c 81e7 9bb4 e5b1 9ee5 8d95 e4bd   "..............
+00003c40: 8de5 9ba2 e5a7 9422 2c20 2276 616c 7565  .......", "value
+00003c50: 223a 2022 e79c 81e7 9bb4 e5b1 9ee5 8d95  ": "............
+00003c60: e4bd 8de5 9ba2 e5a7 942d 4e30 3031 3622  .........-N0016"
+00003c70: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
+00003c80: 2020 2020 7b27 6c61 6265 6c27 3a20 22e7      {'label': ".
+00003c90: 9c81 e5b1 9ee6 9cac e7a7 91e9 99a2 e6a0  ................
+00003ca0: a1e5 9ba2 e5a7 9422 2c20 2276 616c 7565  .......", "value
+00003cb0: 223a 2022 e79c 81e5 b19e e69c ace7 a791  ": "............
+00003cc0: e999 a2e6 a0a1 e59b a2e5 a794 2d4e 3030  ............-N00
+00003cd0: 3133 227d 2c0d 0a20 2020 2020 2020 2020  13"},..         
+00003ce0: 2020 2020 2020 207b 276c 6162 656c 273a         {'label':
+00003cf0: 2022 e99d 9ee7 9c81 e5b1 9ee6 9cac e7a7   "..............
+00003d00: 91e9 99a2 e6a0 a1e5 9ba2 e5a7 9422 2c20  .............", 
+00003d10: 2276 616c 7565 223a 2022 e99d 9ee7 9c81  "value": "......
+00003d20: e5b1 9ee6 9cac e7a7 91e9 99a2 e6a0 a1e5  ................
+00003d30: 9ba2 e5a7 942d 4e30 3031 3422 7d2c 0d0a  .....-N0014"},..
+00003d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d50: 7b27 6c61 6265 6c27 3a20 22e9 ab98 e881  {'label': ".....
+00003d60: 8ce4 b893 e7a7 91e9 99a2 e6a0 a1e5 9ba2  ................
+00003d70: e5a7 9422 2c20 2276 616c 7565 223a 2022  ...", "value": "
+00003d80: e9ab 98e8 818c e4b8 93e7 a791 e999 a2e6  ................
+00003d90: a0a1 e59b a2e5 a794 2d4e 3030 3135 227d  ........-N0015"}
+00003da0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003db0: 2020 207b 276c 6162 656c 273a 2022 e58d     {'label': "..
+00003dc0: 97e6 988c e5b8 8222 2c20 2276 616c 7565  .......", "value
+00003dd0: 223a 2022 e58d 97e6 988c e5b8 822d 4e30  ": ".........-N0
+00003de0: 3030 3222 7d2c 0d0a 2020 2020 2020 2020  002"},..        
+00003df0: 2020 2020 2020 2020 7b27 6c61 6265 6c27          {'label'
+00003e00: 3a20 22e4 b99d e6b1 9fe5 b882 222c 2022  : ".........", "
+00003e10: 7661 6c75 6522 3a20 22e4 b99d e6b1 9fe5  value": ".......
+00003e20: b882 2d4e 3030 3033 227d 2c0d 0a20 2020  ..-N0003"},..   
+00003e30: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
+00003e40: 6162 656c 273a 2022 e699 afe5 beb7 e995  abel': "........
+00003e50: 87e5 b882 222c 2022 7661 6c75 6522 3a20  ....", "value": 
+00003e60: 22e6 99af e5be b7e9 9587 e5b8 822d 4e30  "............-N0
+00003e70: 3030 3422 7d2c 0d0a 2020 2020 2020 2020  004"},..        
+00003e80: 2020 2020 2020 2020 7b27 6c61 6265 6c27          {'label'
+00003e90: 3a20 22e8 908d e4b9 a1e5 b882 222c 2022  : ".........", "
+00003ea0: 7661 6c75 6522 3a20 22e8 908d e4b9 a1e5  value": ".......
+00003eb0: b882 2d4e 3030 3035 227d 2c0d 0a20 2020  ..-N0005"},..   
+00003ec0: 2020 2020 2020 2020 2020 2020 207b 276c               {'l
+00003ed0: 6162 656c 273a 2022 e696 b0e4 bd99 e5b8  abel': "........
+00003ee0: 8222 2c20 2276 616c 7565 223a 2022 e696  .", "value": "..
+00003ef0: b0e4 bd99 e5b8 822d 4e30 3030 3622 7d2c  .......-N0006"},
+00003f00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003f10: 2020 7b27 6c61 6265 6c27 3a20 22e9 b9b0    {'label': "...
+00003f20: e6bd ade5 b882 222c 2022 7661 6c75 6522  ......", "value"
+00003f30: 3a20 22e9 b9b0 e6bd ade5 b882 2d4e 3030  : ".........-N00
+00003f40: 3037 227d 2c0d 0a20 2020 2020 2020 2020  07"},..         
+00003f50: 2020 2020 2020 207b 276c 6162 656c 273a         {'label':
+00003f60: 2022 e8b5 a3e5 b79e e5b8 8222 2c20 2276   ".........", "v
+00003f70: 616c 7565 223a 2022 e8b5 a3e5 b79e e5b8  alue": "........
+00003f80: 822d 4e30 3030 3822 7d2c 0d0a 2020 2020  .-N0008"},..    
+00003f90: 2020 2020 2020 2020 2020 2020 7b27 6c61              {'la
+00003fa0: 6265 6c27 3a20 22e5 ae9c e698 a5e5 b882  bel': ".........
+00003fb0: 222c 2022 7661 6c75 6522 3a20 22e5 ae9c  ", "value": "...
+00003fc0: e698 a5e5 b882 2d4e 3030 3039 227d 2c0d  ......-N0009"},.
+00003fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003fe0: 207b 276c 6162 656c 273a 2022 e4b8 8ae9   {'label': "....
+00003ff0: a5b6 e5b8 8222 2c20 2276 616c 7565 223a  .....", "value":
+00004000: 2022 e4b8 8ae9 a5b6 e5b8 822d 4e30 3031   ".........-N001
+00004010: 3022 7d2c 0d0a 2020 2020 2020 2020 2020  0"},..          
+00004020: 2020 2020 2020 7b27 6c61 6265 6c27 3a20        {'label': 
+00004030: 22e5 9089 e5ae 89e5 b882 222c 2022 7661  ".........", "va
+00004040: 6c75 6522 3a20 22e5 9089 e5ae 89e5 b882  lue": ".........
+00004050: 2d4e 3030 3131 227d 2c0d 0a20 2020 2020  -N0011"},..     
+00004060: 2020 2020 2020 2020 2020 207b 276c 6162             {'lab
+00004070: 656c 273a 2022 e68a 9ae5 b79e e5b8 8222  el': "........."
+00004080: 2c20 2276 616c 7565 223a 2022 e68a 9ae5  , "value": "....
+00004090: b79e e5b8 822d 4e30 3031 3222 7d0d 0a20  .....-N0012"}.. 
+000040a0: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
+000040b0: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
+000040c0: 2020 5365 6c65 6374 280d 0a20 2020 2020    Select(..     
+000040d0: 2020 2020 2020 2074 7970 653d 2273 656c         type="sel
+000040e0: 6563 7422 2c0d 0a20 2020 2020 2020 2020  ect",..         
+000040f0: 2020 206c 6162 656c 3d22 e5ad a6e6 a0a1     label="......
+00004100: e590 8de7 a7b0 222c 0d0a 2020 2020 2020  ......",..      
+00004110: 2020 2020 2020 6e61 6d65 3d22 756e 6976        name="univ
+00004120: 6572 7369 7479 222c 0d0a 2020 2020 2020  ersity",..      
+00004130: 2020 2020 2020 7661 6c75 653d 2224 7b49        value="${I
+00004140: 4628 4953 454d 5054 5928 756e 6976 6572  F(ISEMPTY(univer
+00004150: 7369 7479 5f74 7970 6529 2c75 6e69 7665  sity_type),unive
+00004160: 7273 6974 792c 2727 297d 222c 0d0a 2020  rsity,'')}",..  
+00004170: 2020 2020 2020 2020 2020 7365 6172 6368            search
+00004180: 6162 6c65 3d54 7275 652c 0d0a 2020 2020  able=True,..    
+00004190: 2020 2020 2020 2020 7265 7175 6972 6564          required
+000041a0: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+000041b0: 2020 2020 636c 6561 7261 626c 653d 5472      clearable=Tr
+000041c0: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
+000041d0: 2073 6f75 7263 653d 7b0d 0a20 2020 2020   source={..     
+000041e0: 2020 2020 2020 2020 2020 2022 6d65 7468             "meth
+000041f0: 6f64 223a 2022 6765 7422 2c0d 0a20 2020  od": "get",..   
+00004200: 2020 2020 2020 2020 2020 2020 2022 7572               "ur
+00004210: 6c22 3a20 222f 5465 656e 5374 7564 792f  l": "/TeenStudy/
+00004220: 6170 692f 6f72 6761 6e69 7a61 7469 6f6e  api/organization
+00004230: 3f70 6964 3d24 7b53 504c 4954 2875 6e69  ?pid=${SPLIT(uni
+00004240: 7665 7273 6974 795f 7479 7065 2c27 2d27  versity_type,'-'
+00004250: 295b 315d 7d22 2c0d 0a20 2020 2020 2020  )[1]}",..       
+00004260: 2020 2020 2020 2020 2022 7365 6e64 4f6e           "sendOn
+00004270: 223a 2022 7468 6973 2e75 6e69 7665 7273  ": "this.univers
+00004280: 6974 795f 7479 7065 213d 3d27 2722 0d0a  ity_type!==''"..
+00004290: 2020 2020 2020 2020 2020 2020 7d2c 2068              }, h
+000042a0: 6964 6465 6e4f 6e3d 2274 6869 732e 756e  iddenOn="this.un
+000042b0: 6976 6572 7369 7479 5f74 7970 653d 3d3d  iversity_type===
+000042c0: 2727 7c7c 2074 6869 732e 756e 6976 6572  ''|| this.univer
+000042d0: 7369 7479 5f74 7970 653d 3d3d 756e 6465  sity_type===unde
+000042e0: 6669 6e65 6422 0d0a 2020 2020 2020 2020  fined"..        
+000042f0: 292c 0d0a 2020 2020 2020 2020 5365 6c65  ),..        Sele
+00004300: 6374 280d 0a20 2020 2020 2020 2020 2020  ct(..           
+00004310: 2074 7970 653d 2273 656c 6563 7422 2c0d   type="select",.
+00004320: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+00004330: 656c 3d22 e5ad a6e9 99a2 e590 8de7 a7b0  el="............
+00004340: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00004350: 6e61 6d65 3d22 636f 6c6c 6567 6522 2c0d  name="college",.
+00004360: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00004370: 7565 3d22 247b 4946 2849 5345 4d50 5459  ue="${IF(ISEMPTY
+00004380: 2875 6e69 7665 7273 6974 7929 2c63 6f6c  (university),col
+00004390: 6c65 6765 2c27 2729 7d22 2c0d 0a20 2020  lege,'')}",..   
+000043a0: 2020 2020 2020 2020 2073 6561 7263 6861           searcha
+000043b0: 626c 653d 5472 7565 2c0d 0a20 2020 2020  ble=True,..     
+000043c0: 2020 2020 2020 2072 6571 7569 7265 643d         required=
+000043d0: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+000043e0: 2020 2063 6c65 6172 6162 6c65 3d54 7275     clearable=Tru
+000043f0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00004400: 736f 7572 6365 3d7b 0d0a 2020 2020 2020  source={..      
+00004410: 2020 2020 2020 2020 2020 226d 6574 686f            "metho
+00004420: 6422 3a20 2267 6574 222c 0d0a 2020 2020  d": "get",..    
+00004430: 2020 2020 2020 2020 2020 2020 2275 726c              "url
+00004440: 223a 2022 2f54 6565 6e53 7475 6479 2f61  ": "/TeenStudy/a
+00004450: 7069 2f6f 7267 616e 697a 6174 696f 6e3f  pi/organization?
+00004460: 7069 643d 247b 5350 4c49 5428 756e 6976  pid=${SPLIT(univ
+00004470: 6572 7369 7479 2c27 2d27 295b 315d 7d22  ersity,'-')[1]}"
+00004480: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00004490: 2020 2022 7365 6e64 4f6e 223a 2022 7468     "sendOn": "th
+000044a0: 6973 2e75 6e69 7665 7273 6974 7921 3d3d  is.university!==
+000044b0: 2727 220d 0a20 2020 2020 2020 2020 2020  ''"..           
+000044c0: 207d 2c0d 0a20 2020 2020 2020 2020 2020   },..           
+000044d0: 2068 6964 6465 6e4f 6e3d 2274 6869 732e   hiddenOn="this.
+000044e0: 756e 6976 6572 7369 7479 5f74 7970 653d  university_type=
+000044f0: 3d3d 2727 207c 7c20 7468 6973 2e75 6e69  =='' || this.uni
+00004500: 7665 7273 6974 793d 3d3d 2727 7c7c 7468  versity===''||th
+00004510: 6973 2e75 6e69 7665 7273 6974 795f 7479  is.university_ty
+00004520: 7065 3d3d 3d75 6e64 6566 696e 6564 207c  pe===undefined |
+00004530: 7c20 7468 6973 2e75 6e69 7665 7273 6974  | this.universit
+00004540: 793d 3d3d 756e 6465 6669 6e65 6422 0d0a  y===undefined"..
+00004550: 2020 2020 2020 2020 292c 0d0a 2020 2020          ),..    
+00004560: 2020 2020 5365 6c65 6374 280d 0a20 2020      Select(..   
+00004570: 2020 2020 2020 2020 2074 7970 653d 2273           type="s
+00004580: 656c 6563 7422 2c0d 0a20 2020 2020 2020  elect",..       
+00004590: 2020 2020 206c 6162 656c 3d22 e59b a2e6       label="....
+000045a0: 94af e983 a822 2c0d 0a20 2020 2020 2020  .....",..       
+000045b0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+000045c0: 3d22 e59b a2e6 94af e983 a8e5 908d e7a7  ="..............
+000045d0: b0ef bc8c e5af b9e5 ba94 e6b1 9fe8 a5bf  ................
+000045e0: e585 b1e9 9d92 e59b a2e4 b8aa e4ba bae4  ................
+000045f0: bfae e694 b9e4 bfa1 e681 afe9 a1b5 20e7  .............. .
+00004600: 8fad e7ba a72f e59b a2e6 94af e983 a822  ...../........."
+00004610: 2c0d 0a20 2020 2020 2020 2020 2020 206e  ,..            n
+00004620: 616d 653d 226f 7267 616e 697a 6174 696f  ame="organizatio
+00004630: 6e22 2c0d 0a20 2020 2020 2020 2020 2020  n",..           
+00004640: 2076 616c 7565 3d22 247b 4946 2849 5345   value="${IF(ISE
+00004650: 4d50 5459 2863 6f6c 6c65 6765 292c 6f72  MPTY(college),or
+00004660: 6761 6e69 7a61 7469 6f6e 2c27 2729 7d22  ganization,'')}"
+00004670: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
+00004680: 6561 7263 6861 626c 653d 5472 7565 2c0d  earchable=True,.
+00004690: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
+000046a0: 7569 7265 643d 4661 6c73 652c 0d0a 2020  uired=False,..  
+000046b0: 2020 2020 2020 2020 2020 636c 6561 7261            cleara
+000046c0: 626c 653d 5472 7565 2c0d 0a20 2020 2020  ble=True,..     
+000046d0: 2020 2020 2020 2073 6f75 7263 653d 7b0d         source={.
+000046e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000046f0: 2022 6d65 7468 6f64 223a 2022 6765 7422   "method": "get"
+00004700: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00004710: 2020 2022 7572 6c22 3a20 222f 5465 656e     "url": "/Teen
+00004720: 5374 7564 792f 6170 692f 6f72 6761 6e69  Study/api/organi
+00004730: 7a61 7469 6f6e 3f70 6964 3d24 7b53 504c  zation?pid=${SPL
+00004740: 4954 2863 6f6c 6c65 6765 2c27 2d27 295b  IT(college,'-')[
+00004750: 315d 7d22 2c0d 0a20 2020 2020 2020 2020  1]}",..         
+00004760: 2020 2020 2020 2022 7365 6e64 4f6e 223a         "sendOn":
+00004770: 2022 7468 6973 2e63 6f6c 6c65 6765 213d   "this.college!=
+00004780: 3d27 2722 0d0a 2020 2020 2020 2020 2020  =''"..          
+00004790: 2020 7d2c 0d0a 2020 2020 2020 2020 2020    },..          
+000047a0: 2020 6869 6464 656e 4f6e 3d22 7468 6973    hiddenOn="this
+000047b0: 2e75 6e69 7665 7273 6974 795f 7479 7065  .university_type
+000047c0: 3d3d 3d27 277c 7c74 6869 732e 756e 6976  ===''||this.univ
+000047d0: 6572 7369 7479 3d3d 3d27 277c 7c74 6869  ersity===''||thi
+000047e0: 732e 636f 6c6c 6567 653d 3d3d 2727 7c7c  s.college===''||
+000047f0: 7468 6973 2e75 6e69 7665 7273 6974 795f  this.university_
+00004800: 7479 7065 3d3d 3d75 6e64 6566 696e 6564  type===undefined
+00004810: 7c7c 7468 6973 2e75 6e69 7665 7273 6974  ||this.universit
+00004820: 793d 3d3d 756e 6465 6669 6e65 647c 7c74  y===undefined||t
+00004830: 6869 732e 636f 6c6c 6567 653d 3d3d 756e  his.college===un
+00004840: 6465 6669 6e65 6422 0d0a 2020 2020 2020  defined"..      
+00004850: 2020 292c 0d0a 2020 2020 2020 2020 496e    ),..        In
+00004860: 7075 7454 6578 7428 0d0a 2020 2020 2020  putText(..      
+00004870: 2020 2020 2020 6c61 6265 6c3d 22e7 99bb        label="...
+00004880: e5bd 95e5 af86 e7a0 8122 2c0d 0a20 2020  .........",..   
+00004890: 2020 2020 2020 2020 2074 7970 653d 2769           type='i
+000048a0: 6e70 7574 2d70 6173 7377 6f72 6427 2c0d  nput-password',.
+000048b0: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
+000048c0: 6372 6970 7469 6f6e 3d22 e58f afe4 b88d  cription="......
+000048d0: e5a1 abef bc8c e9bb 98e8 aea4 e4b8 bae7  ................
+000048e0: 94a8 e688 b749 4422 2c0d 0a20 2020 2020  .....ID",..     
+000048f0: 2020 2020 2020 206e 616d 653d 2270 6173         name="pas
+00004900: 7377 6f72 6422 2c0d 0a20 2020 2020 2020  sword",..       
+00004910: 2020 2020 2069 6e6c 696e 653d 4661 6c73       inline=Fals
+00004920: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00004930: 7265 7175 6972 6564 3d46 616c 7365 2c0d  required=False,.
+00004940: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00004950: 7565 3d22 222c 0d0a 2020 2020 2020 2020  ue="",..        
+00004960: 2020 2020 636c 6561 7261 626c 653d 5472      clearable=Tr
+00004970: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
+00004980: 206d 6178 4c65 6e67 7468 3d31 360d 0a20   maxLength=16.. 
+00004990: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
+000049a0: 2020 2049 6e70 7574 5465 7874 280d 0a20     InputText(.. 
+000049b0: 2020 2020 2020 2020 2020 206c 6162 656c             label
+000049c0: 3d22 e689 8be6 9cba e58f b72f e5ad a6e5  ="........./....
+000049d0: 8fb7 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
+000049e0: 2020 6465 7363 7269 7074 696f 6e3d 22e5    description=".
+000049f0: afb9 e5ba 94e6 b19f e8a5 bfe5 85b1 e99d  ................
+00004a00: 92e5 9ba2 e4b8 aae4 baba e4bf aee6 94b9  ................
+00004a10: e4bf a1e6 81af e9a1 b520 e689 8be6 9cba  ......... ......
+00004a20: e58f b72f e5ad a6e5 8fb7 efbc 8ce7 a9ba  .../............
+00004a30: e79d 80e4 b88d e794 a8e5 a1ab 222c 0d0a  ............",..
+00004a40: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+00004a50: 3d22 6d6f 6269 6c65 222c 0d0a 2020 2020  ="mobile",..    
+00004a60: 2020 2020 2020 2020 696e 6c69 6e65 3d46          inline=F
+00004a70: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
+00004a80: 2020 2072 6571 7569 7265 643d 4661 6c73     required=Fals
+00004a90: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00004aa0: 7661 6c75 653d 2222 2c0d 0a20 2020 2020  value="",..     
+00004ab0: 2020 2020 2020 2063 6c65 6172 6162 6c65         clearable
+00004ac0: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+00004ad0: 2020 2020 6d61 784c 656e 6774 683d 3131      maxLength=11
+00004ae0: 0d0a 2020 2020 2020 2020 292c 0d0a 2020  ..        ),..  
+00004af0: 2020 2020 2020 496e 7075 7454 6578 7428        InputText(
+00004b00: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
+00004b10: 6265 6c3d 22e5 a793 e590 8d22 2c0d 0a20  bel="......",.. 
+00004b20: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+00004b30: 6970 7469 6f6e 3d22 e5af b9e5 ba94 e6b1  iption="........
+00004b40: 9fe8 a5bf e585 b1e9 9d92 e59b a2e4 b8aa  ................
+00004b50: e4ba bae4 bfae e694 b9e4 bfa1 e681 afe9  ................
+00004b60: a1b5 20e7 9c9f e5ae 9ee5 a793 e590 8d22  .. ............"
+00004b70: 2c0d 0a20 2020 2020 2020 2020 2020 206e  ,..            n
+00004b80: 616d 653d 226e 616d 6522 2c0d 0a20 2020  ame="name",..   
+00004b90: 2020 2020 2020 2020 2069 6e6c 696e 653d           inline=
+00004ba0: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+00004bb0: 2020 2020 7265 7175 6972 6564 3d54 7275      required=Tru
+00004bc0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00004bd0: 7661 6c75 653d 2222 2c0d 0a20 2020 2020  value="",..     
+00004be0: 2020 2020 2020 2063 6c65 6172 6162 6c65         clearable
+00004bf0: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+00004c00: 2020 2020 6d61 784c 656e 6774 683d 380d      maxLength=8.
+00004c10: 0a20 2020 2020 2020 2029 0d0a 0d0a 2020  .        )....  
+00004c20: 2020 5d0d 0a29 0d0a 0d0a 2222 22e5 ae89    ]..)...."""...
+00004c30: e5be bde6 b7bb e58a a0e6 8890 e591 98e9  ................
+00004c40: 9da2 e69d bf22 2222 0d0a 616e 6875 695f  ....."""..anhui_
+00004c50: 7461 626c 6520 3d20 466f 726d 280d 0a20  table = Form(.. 
+00004c60: 2020 2074 6974 6c65 3d22 e6b7 bbe5 8aa0     title="......
+00004c70: e5ae 89e5 bebd e585 b1e9 9d92 e59b a2e7  ................
+00004c80: 94a8 e688 b722 2c0d 0a20 2020 2073 7562  .....",..    sub
+00004c90: 6d69 7454 6578 743d 22e6 b7bb e58a a022  mitText="......"
+00004ca0: 2c0d 0a20 2020 206d 6f64 653d 4469 7370  ,..    mode=Disp
+00004cb0: 6c61 794d 6f64 6545 6e75 6d2e 686f 7269  layModeEnum.hori
+00004cc0: 7a6f 6e74 616c 2c0d 0a20 2020 2061 7069  zontal,..    api
+00004cd0: 3d22 706f 7374 3a2f 5465 656e 5374 7564  ="post:/TeenStud
+00004ce0: 792f 6170 692f 616e 6875 692f 6164 6422  y/api/anhui/add"
+00004cf0: 2c0d 0a20 2020 2072 6573 6574 4166 7465  ,..    resetAfte
+00004d00: 7253 7562 6d69 743d 5472 7565 2c0d 0a20  rSubmit=True,.. 
+00004d10: 2020 2062 6f64 793d 5b0d 0a20 2020 2020     body=[..     
+00004d20: 2020 2053 656c 6563 7428 0d0a 2020 2020     Select(..    
+00004d30: 2020 2020 2020 2020 6c61 6265 6c3d 22e7          label=".
+00004d40: bea4 e881 8a22 2c0d 0a20 2020 2020 2020  .....",..       
+00004d50: 2020 2020 206e 616d 653d 2267 726f 7570       name="group
+00004d60: 5f69 6422 2c0d 0a20 2020 2020 2020 2020  _id",..         
+00004d70: 2020 2064 6573 6372 6970 7469 6f6e 3d22     description="
+00004d80: e99c 80e8 a681 e6b7 bbe5 8aa0 e79a 84e7  ................
+00004d90: bea4 e7bb 8422 2c0d 0a20 2020 2020 2020  .....",..       
+00004da0: 2020 2020 2063 6865 636b 416c 6c3d 4661       checkAll=Fa
+00004db0: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+00004dc0: 2020 736f 7572 6365 3d22 6765 743a 2f54    source="get:/T
+00004dd0: 6565 6e53 7475 6479 2f61 7069 2f67 6574  eenStudy/api/get
+00004de0: 5f67 726f 7570 5f6c 6973 7422 2c0d 0a20  _group_list",.. 
+00004df0: 2020 2020 2020 2020 2020 2076 616c 7565             value
+00004e00: 3d27 272c 0d0a 2020 2020 2020 2020 2020  ='',..          
+00004e10: 2020 6d75 6c74 6970 6c65 3d46 616c 7365    multiple=False
+00004e20: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+00004e30: 6571 7569 7265 643d 5472 7565 2c0d 0a20  equired=True,.. 
+00004e40: 2020 2020 2020 2020 2020 2073 6561 7263             searc
+00004e50: 6861 626c 653d 5472 7565 2c0d 0a20 2020  hable=True,..   
+00004e60: 2020 2020 2020 2020 206a 6f69 6e56 616c           joinVal
+00004e70: 7565 733d 4661 6c73 652c 0d0a 2020 2020  ues=False,..    
+00004e80: 2020 2020 2020 2020 6578 7472 6163 7456          extractV
+00004e90: 616c 7565 3d54 7275 652c 0d0a 2020 2020  alue=True,..    
+00004ea0: 2020 2020 2020 2020 7374 6174 6973 7469          statisti
+00004eb0: 6373 3d54 7275 652c 0d0a 2020 2020 2020  cs=True,..      
+00004ec0: 2020 292c 0d0a 2020 2020 2020 2020 5365    ),..        Se
+00004ed0: 6c65 6374 280d 0a20 2020 2020 2020 2020  lect(..         
+00004ee0: 2020 206c 6162 656c 3d22 e794 a8e6 88b7     label="......
+00004ef0: 4944 222c 0d0a 2020 2020 2020 2020 2020  ID",..          
+00004f00: 2020 6e61 6d65 3d22 7573 6572 5f69 6422    name="user_id"
+00004f10: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
+00004f20: 6573 6372 6970 7469 6f6e 3d22 e99c 80e8  escription="....
+00004f30: a681 e6b7 bbe5 8aa0 e79a 84e7 94a8 e688  ................
+00004f40: b749 4422 2c0d 0a20 2020 2020 2020 2020  .ID",..         
+00004f50: 2020 2063 6865 636b 416c 6c3d 4661 6c73     checkAll=Fals
+00004f60: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00004f70: 736f 7572 6365 3d22 6765 743a 2f54 6565  source="get:/Tee
+00004f80: 6e53 7475 6479 2f61 7069 2f67 6574 5f6d  nStudy/api/get_m
+00004f90: 656d 6265 725f 6c69 7374 3f67 726f 7570  ember_list?group
+00004fa0: 5f69 643d 247b 6772 6f75 705f 6964 7d22  _id=${group_id}"
+00004fb0: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
+00004fc0: 616c 7565 3d27 272c 0d0a 2020 2020 2020  alue='',..      
+00004fd0: 2020 2020 2020 6d75 6c74 6970 6c65 3d46        multiple=F
+00004fe0: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
+00004ff0: 2020 2072 6571 7569 7265 643d 5472 7565     required=True
+00005000: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
+00005010: 6561 7263 6861 626c 653d 5472 7565 2c0d  earchable=True,.
+00005020: 0a20 2020 2020 2020 2020 2020 206a 6f69  .            joi
+00005030: 6e56 616c 7565 733d 4661 6c73 652c 0d0a  nValues=False,..
+00005040: 2020 2020 2020 2020 2020 2020 6578 7472              extr
+00005050: 6163 7456 616c 7565 3d54 7275 652c 0d0a  actValue=True,..
+00005060: 2020 2020 2020 2020 2020 2020 7374 6174              stat
+00005070: 6973 7469 6373 3d54 7275 652c 0d0a 2020  istics=True,..  
+00005080: 2020 2020 2020 2020 2020 6869 6464 656e            hidden
+00005090: 4f6e 3d22 247b 6772 6f75 705f 6964 3d3d  On="${group_id==
+000050a0: 2727 3f74 7275 653a 6661 6c73 657d 220d  ''?true:false}".
+000050b0: 0a20 2020 2020 2020 2029 2c0d 0a20 2020  .        ),..   
+000050c0: 2020 2020 2049 6e70 7574 5465 7874 280d       InputText(.
+000050d0: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+000050e0: 656c 3d22 e59c b0e5 8cba 222c 0d0a 2020  el="......",..  
+000050f0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+00005100: 7074 696f 6e3d 22e6 8980 e5a4 84e7 9c81  ption=".........
+00005110: e4bb bd22 2c0d 0a20 2020 2020 2020 2020  ...",..         
+00005120: 2020 206e 616d 653d 2261 7265 6122 2c0d     name="area",.
+00005130: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00005140: 7565 3d22 e5ae 89e5 bebd 222c 0d0a 2020  ue="......",..  
+00005150: 2020 2020 2020 2020 2020 6469 7361 626c            disabl
+00005160: 6564 3d54 7275 650d 0a20 2020 2020 2020  ed=True..       
+00005170: 2029 2c0d 0a20 2020 2020 2020 2049 6e70   ),..        Inp
+00005180: 7574 5465 7874 280d 0a20 2020 2020 2020  utText(..       
+00005190: 2020 2020 206c 6162 656c 3d22 e799 bbe5       label="....
+000051a0: bd95 e5af 86e7 a081 222c 0d0a 2020 2020  ........",..    
+000051b0: 2020 2020 2020 2020 7479 7065 3d27 696e          type='in
+000051c0: 7075 742d 7061 7373 776f 7264 272c 0d0a  put-password',..
+000051d0: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+000051e0: 7269 7074 696f 6e3d 22e5 8faf e4b8 8de5  ription=".......
+000051f0: a1ab efbc 8ce9 bb98 e8ae a4e4 b8ba e794  ................
+00005200: a8e6 88b7 4944 222c 0d0a 2020 2020 2020  ....ID",..      
+00005210: 2020 2020 2020 6e61 6d65 3d22 7061 7373        name="pass
+00005220: 776f 7264 222c 0d0a 2020 2020 2020 2020  word",..        
+00005230: 2020 2020 696e 6c69 6e65 3d46 616c 7365      inline=False
+00005240: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+00005250: 6571 7569 7265 643d 4661 6c73 652c 0d0a  equired=False,..
+00005260: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00005270: 653d 2222 2c0d 0a20 2020 2020 2020 2020  e="",..         
+00005280: 2020 2063 6c65 6172 6162 6c65 3d54 7275     clearable=Tru
+00005290: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+000052a0: 6d61 784c 656e 6774 683d 3136 0d0a 2020  maxLength=16..  
+000052b0: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
+000052c0: 2020 496e 7075 7454 6578 7428 0d0a 2020    InputText(..  
+000052d0: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
+000052e0: 2275 726c 222c 0d0a 2020 2020 2020 2020  "url",..        
+000052f0: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
+00005300: 22e4 b8aa e4ba bae4 bfa1 e681 afe4 bfae  "...............
+00005310: e694 b9e9 a1b5 efbc 8ce7 82b9 e58f b3e4  ................
+00005320: b88a e8a7 92e5 8886 e4ba abef bc8c e5a4  ................
+00005330: 8de5 88b6 e993 bee6 8ea5 e5a1 abe5 85a5  ................
+00005340: e58d b3e5 8faf 20e9 93be e68e a5e6 a0bc  ...... .........
+00005350: e5bc 8fef bc9a 6874 7470 3a2f 2f64 7878  ......http://dxx
+00005360: 2e61 6879 6f75 7468 2e6f 7267 2e63 6e2f  .ahyouth.org.cn/
+00005370: 6d6f 6469 6679 2f3f 746b 3de6 82a8 e79a  modify/?tk=.....
+00005380: 8474 6f6b 656e e580 bc22 2c0d 0a20 2020  .token...",..   
+00005390: 2020 2020 2020 2020 206e 616d 653d 2275           name="u
+000053a0: 726c 222c 0d0a 2020 2020 2020 2020 2020  rl",..          
+000053b0: 2020 696e 6c69 6e65 3d46 616c 7365 2c0d    inline=False,.
+000053c0: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
+000053d0: 7569 7265 643d 5472 7565 2c0d 0a20 2020  uired=True,..   
+000053e0: 2020 2020 2020 2020 2076 616c 7565 3d22           value="
+000053f0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00005400: 636c 6561 7261 626c 653d 5472 7565 2c0d  clearable=True,.
+00005410: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+00005420: 4c65 6e67 7468 3d31 3238 0d0a 2020 2020  Length=128..    
+00005430: 2020 2020 290d 0a0d 0a20 2020 205d 0d0a      )....    ]..
+00005440: 290d 0a22 2222 e59b 9be5 b79d e6b7 bbe5  ).."""..........
+00005450: 8aa0 e688 90e5 9198 e99d a2e6 9dbf 2222  ..............""
+00005460: 220d 0a73 6963 6875 616e 5f74 6162 6c65  "..sichuan_table
+00005470: 203d 2046 6f72 6d28 0d0a 2020 2020 7469   = Form(..    ti
+00005480: 746c 653d 22e6 b7bb e58a a0e5 a4a9 e5ba  tle="...........
+00005490: 9ce6 96b0 e99d 92e5 b9b4 e794 a8e6 88b7  ................
+000054a0: 222c 0d0a 2020 2020 7375 626d 6974 5465  ",..    submitTe
+000054b0: 7874 3d22 e6b7 bbe5 8aa0 222c 0d0a 2020  xt="......",..  
+000054c0: 2020 6d6f 6465 3d44 6973 706c 6179 4d6f    mode=DisplayMo
+000054d0: 6465 456e 756d 2e68 6f72 697a 6f6e 7461  deEnum.horizonta
+000054e0: 6c2c 0d0a 2020 2020 6170 693d 2270 6f73  l,..    api="pos
+000054f0: 743a 2f54 6565 6e53 7475 6479 2f61 7069  t:/TeenStudy/api
+00005500: 2f73 6963 6875 616e 2f61 6464 222c 0d0a  /sichuan/add",..
+00005510: 2020 2020 7265 7365 7441 6674 6572 5375      resetAfterSu
+00005520: 626d 6974 3d54 7275 652c 0d0a 2020 2020  bmit=True,..    
+00005530: 626f 6479 3d5b 0d0a 2020 2020 2020 2020  body=[..        
+00005540: 416c 6572 7428 6c65 7665 6c3d 4c65 7665  Alert(level=Leve
+00005550: 6c45 6e75 6d2e 696e 666f 2c0d 0a20 2020  lEnum.info,..   
+00005560: 2020 2020 2020 2020 2020 2063 6c61 7373             class
+00005570: 4e61 6d65 3d27 7768 6974 652d 7370 6163  Name='white-spac
+00005580: 652d 7072 652d 7772 6170 272c 0d0a 2020  e-pre-wrap',..  
+00005590: 2020 2020 2020 2020 2020 2020 626f 6479              body
+000055a0: 3d28 0d0a 2020 2020 2020 2020 2020 2020  =(..            
+000055b0: 2020 2020 2020 22e8 afa5 e59c b0e5 8cba        ".........
+000055c0: e99c 80e8 a681 e887 aae8 a18c e68a 93e5  ................
+000055d0: 8c85 e5a1 abe5 85a5 5c6e 746f 6b65 6ee5  ........\ntoken.
+000055e0: 80bc e59c a868 7474 7073 3a2f 2f64 7878  .....https://dxx
+000055f0: 2e73 6379 6f6c 2e63 6f6d 2f61 7069 2f77  .scyol.com/api/w
+00005600: 6563 6861 742f 6c6f 6769 6e20 e593 8de5  echat/login ....
+00005610: ba94 e987 8c5c 6ee5 85b6 e4bd 99e4 bfa1  .....\n.........
+00005620: e681 afe5 9ca8 2068 7474 7073 3a2f 2f64  ...... https://d
+00005630: 7878 2e73 6379 6f6c 2e63 6f6d 2f61 7069  xx.scyol.com/api
+00005640: 2f73 7475 6465 6e74 2f73 686f 7753 7475  /student/showStu
+00005650: 6479 5374 6167 654f 7267 3f69 643d 7878  dyStageOrg?id=xx
+00005660: 7878 7878 2673 7461 6765 4964 3d78 7820  xxxx&stageId=xx 
+00005670: e593 8de5 ba94 e987 8c22 2929 2c0d 0a20  .........")),.. 
+00005680: 2020 2020 2020 2053 656c 6563 7428 0d0a         Select(..
+00005690: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+000056a0: 6c3d 22e7 bea4 e881 8a22 2c0d 0a20 2020  l="......",..   
+000056b0: 2020 2020 2020 2020 206e 616d 653d 2267           name="g
+000056c0: 726f 7570 5f69 6422 2c0d 0a20 2020 2020  roup_id",..     
+000056d0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+000056e0: 6f6e 3d22 e99c 80e8 a681 e6b7 bbe5 8aa0  on="............
+000056f0: e79a 84e7 bea4 e7bb 8422 2c0d 0a20 2020  .........",..   
+00005700: 2020 2020 2020 2020 2063 6865 636b 416c           checkAl
+00005710: 6c3d 4661 6c73 652c 0d0a 2020 2020 2020  l=False,..      
+00005720: 2020 2020 2020 736f 7572 6365 3d22 6765        source="ge
+00005730: 743a 2f54 6565 6e53 7475 6479 2f61 7069  t:/TeenStudy/api
+00005740: 2f67 6574 5f67 726f 7570 5f6c 6973 7422  /get_group_list"
+00005750: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
+00005760: 616c 7565 3d27 272c 0d0a 2020 2020 2020  alue='',..      
+00005770: 2020 2020 2020 6d75 6c74 6970 6c65 3d46        multiple=F
+00005780: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
+00005790: 2020 2072 6571 7569 7265 643d 5472 7565     required=True
+000057a0: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
+000057b0: 6561 7263 6861 626c 653d 5472 7565 2c0d  earchable=True,.
+000057c0: 0a20 2020 2020 2020 2020 2020 206a 6f69  .            joi
+000057d0: 6e56 616c 7565 733d 4661 6c73 652c 0d0a  nValues=False,..
+000057e0: 2020 2020 2020 2020 2020 2020 6578 7472              extr
+000057f0: 6163 7456 616c 7565 3d54 7275 652c 0d0a  actValue=True,..
+00005800: 2020 2020 2020 2020 2020 2020 7374 6174              stat
+00005810: 6973 7469 6373 3d54 7275 652c 0d0a 2020  istics=True,..  
+00005820: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
+00005830: 2020 5365 6c65 6374 280d 0a20 2020 2020    Select(..     
+00005840: 2020 2020 2020 206c 6162 656c 3d22 e794         label="..
+00005850: a8e6 88b7 4944 222c 0d0a 2020 2020 2020  ....ID",..      
+00005860: 2020 2020 2020 6e61 6d65 3d22 7573 6572        name="user
+00005870: 5f69 6422 2c0d 0a20 2020 2020 2020 2020  _id",..         
+00005880: 2020 2064 6573 6372 6970 7469 6f6e 3d22     description="
+00005890: e99c 80e8 a681 e6b7 bbe5 8aa0 e79a 84e7  ................
+000058a0: 94a8 e688 b749 4422 2c0d 0a20 2020 2020  .....ID",..     
+000058b0: 2020 2020 2020 2063 6865 636b 416c 6c3d         checkAll=
+000058c0: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+000058d0: 2020 2020 736f 7572 6365 3d22 6765 743a      source="get:
+000058e0: 2f54 6565 6e53 7475 6479 2f61 7069 2f67  /TeenStudy/api/g
+000058f0: 6574 5f6d 656d 6265 725f 6c69 7374 3f67  et_member_list?g
+00005900: 726f 7570 5f69 643d 247b 6772 6f75 705f  roup_id=${group_
+00005910: 6964 7d22 2c0d 0a20 2020 2020 2020 2020  id}",..         
+00005920: 2020 2076 616c 7565 3d27 272c 0d0a 2020     value='',..  
+00005930: 2020 2020 2020 2020 2020 6d75 6c74 6970            multip
+00005940: 6c65 3d46 616c 7365 2c0d 0a20 2020 2020  le=False,..     
+00005950: 2020 2020 2020 2072 6571 7569 7265 643d         required=
+00005960: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+00005970: 2020 2073 6561 7263 6861 626c 653d 5472     searchable=Tr
+00005980: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
+00005990: 206a 6f69 6e56 616c 7565 733d 4661 6c73   joinValues=Fals
+000059a0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+000059b0: 6578 7472 6163 7456 616c 7565 3d54 7275  extractValue=Tru
+000059c0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+000059d0: 7374 6174 6973 7469 6373 3d54 7275 652c  statistics=True,
+000059e0: 0d0a 2020 2020 2020 2020 2020 2020 6869  ..            hi
+000059f0: 6464 656e 4f6e 3d22 247b 6772 6f75 705f  ddenOn="${group_
+00005a00: 6964 3d3d 2727 3f74 7275 653a 6661 6c73  id==''?true:fals
+00005a10: 657d 220d 0a20 2020 2020 2020 2029 2c0d  e}"..        ),.
+00005a20: 0a20 2020 2020 2020 2049 6e70 7574 5465  .        InputTe
+00005a30: 7874 280d 0a20 2020 2020 2020 2020 2020  xt(..           
+00005a40: 206c 6162 656c 3d22 e59c b0e5 8cba 222c   label="......",
+00005a50: 0d0a 2020 2020 2020 2020 2020 2020 6465  ..            de
+00005a60: 7363 7269 7074 696f 6e3d 22e6 8980 e5a4  scription=".....
+00005a70: 84e7 9c81 e4bb bd22 2c0d 0a20 2020 2020  .......",..     
+00005a80: 2020 2020 2020 206e 616d 653d 2261 7265         name="are
+00005a90: 6122 2c0d 0a20 2020 2020 2020 2020 2020  a",..           
+00005aa0: 2076 616c 7565 3d22 e59b 9be5 b79d 222c   value="......",
+00005ab0: 0d0a 2020 2020 2020 2020 2020 2020 6469  ..            di
+00005ac0: 7361 626c 6564 3d54 7275 650d 0a20 2020  sabled=True..   
+00005ad0: 2020 2020 2029 2c0d 0a20 2020 2020 2020       ),..       
+00005ae0: 2049 6e70 7574 5465 7874 280d 0a20 2020   InputText(..   
+00005af0: 2020 2020 2020 2020 206c 6162 656c 3d22           label="
+00005b00: e799 bbe5 bd95 e5af 86e7 a081 222c 0d0a  ............",..
+00005b10: 2020 2020 2020 2020 2020 2020 7479 7065              type
+00005b20: 3d27 696e 7075 742d 7061 7373 776f 7264  ='input-password
+00005b30: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00005b40: 6465 7363 7269 7074 696f 6e3d 22e5 8faf  description="...
+00005b50: e4b8 8de5 a1ab efbc 8ce9 bb98 e8ae a4e4  ................
+00005b60: b8ba e794 a8e6 88b7 4944 222c 0d0a 2020  ........ID",..  
+00005b70: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
+00005b80: 7061 7373 776f 7264 222c 0d0a 2020 2020  password",..    
+00005b90: 2020 2020 2020 2020 696e 6c69 6e65 3d46          inline=F
+00005ba0: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
+00005bb0: 2020 2072 6571 7569 7265 643d 4661 6c73     required=Fals
+00005bc0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00005bd0: 7661 6c75 653d 2222 2c0d 0a20 2020 2020  value="",..     
+00005be0: 2020 2020 2020 2063 6c65 6172 6162 6c65         clearable
+00005bf0: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+00005c00: 2020 2020 6d61 784c 656e 6774 683d 3136      maxLength=16
+00005c10: 0d0a 2020 2020 2020 2020 292c 0d0a 2020  ..        ),..  
+00005c20: 2020 2020 2020 496e 7075 7454 6578 7428        InputText(
+00005c30: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
+00005c40: 6265 6c3d 22e5 a793 e590 8d22 2c0d 0a20  bel="......",.. 
+00005c50: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+00005c60: 6970 7469 6f6e 3d22 e5af b9e5 ba94 e68a  iption="........
+00005c70: 93e5 8c85 e586 85e5 aeb9 206e 616d 6522  .......... name"
+00005c80: 2c0d 0a20 2020 2020 2020 2020 2020 206e  ,..            n
+00005c90: 616d 653d 226e 616d 6522 2c0d 0a20 2020  ame="name",..   
+00005ca0: 2020 2020 2020 2020 2069 6e6c 696e 653d           inline=
+00005cb0: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+00005cc0: 2020 2020 7265 7175 6972 6564 3d54 7275      required=Tru
+00005cd0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00005ce0: 7661 6c75 653d 2222 2c0d 0a20 2020 2020  value="",..     
+00005cf0: 2020 2020 2020 2063 6c65 6172 6162 6c65         clearable
+00005d00: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+00005d10: 2020 2020 6d61 784c 656e 6774 683d 380d      maxLength=8.
+00005d20: 0a20 2020 2020 2020 2029 2c0d 0a20 2020  .        ),..   
+00005d30: 2020 2020 2049 6e70 7574 5465 7874 280d       InputText(.
+00005d40: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+00005d50: 656c 3d22 746f 6b65 6e22 2c0d 0a20 2020  el="token",..   
+00005d60: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+00005d70: 7469 6f6e 3d22 e887 aae8 a18c e68a 93e5  tion="..........
+00005d80: 8c85 e88e b7e5 8f96 efbc 8ce5 9ca8 efbc  ................
+00005d90: 9a68 7474 7073 3a2f 2f64 7878 2e73 6379  .https://dxx.scy
+00005da0: 6f6c 2e63 6f6d 2f61 7069 2f77 6563 6861  ol.com/api/wecha
+00005db0: 742f 6c6f 6769 6e20 e993 bee6 8ea5 e79a  t/login ........
+00005dc0: 84e5 938d e5ba 94e5 8685 e5ae b9e9 878c  ................
+00005dd0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00005de0: 6e61 6d65 3d22 746f 6b65 6e22 2c0d 0a20  name="token",.. 
+00005df0: 2020 2020 2020 2020 2020 2069 6e6c 696e             inlin
+00005e00: 653d 4661 6c73 652c 0d0a 2020 2020 2020  e=False,..      
+00005e10: 2020 2020 2020 7265 7175 6972 6564 3d54        required=T
+00005e20: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+00005e30: 2020 7661 6c75 653d 2222 2c0d 0a20 2020    value="",..   
+00005e40: 2020 2020 2020 2020 2063 6c65 6172 6162           clearab
+00005e50: 6c65 3d54 7275 652c 0d0a 2020 2020 2020  le=True,..      
+00005e60: 2020 292c 0d0a 2020 2020 2020 2020 496e    ),..        In
+00005e70: 7075 7454 6578 7428 0d0a 2020 2020 2020  putText(..      
+00005e80: 2020 2020 2020 6c61 6265 6c3d 22e6 898b        label="...
+00005e90: e69c bae5 8fb7 222c 0d0a 2020 2020 2020  ......",..      
+00005ea0: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00005eb0: 6e3d 22e8 87aa e8a1 8ce6 8a93 e58c 85e8  n=".............
+00005ec0: 8eb7 e58f 96ef bc8c e5af b9e5 ba94 7465  ..............te
+00005ed0: 6c22 2c0d 0a20 2020 2020 2020 2020 2020  l",..           
+00005ee0: 206e 616d 653d 226d 6f62 696c 6522 2c0d   name="mobile",.
+00005ef0: 0a20 2020 2020 2020 2020 2020 2069 6e6c  .            inl
+00005f00: 696e 653d 4661 6c73 652c 0d0a 2020 2020  ine=False,..    
+00005f10: 2020 2020 2020 2020 7265 7175 6972 6564          required
+00005f20: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+00005f30: 2020 2020 7661 6c75 653d 2222 2c0d 0a20      value="",.. 
+00005f40: 2020 2020 2020 2020 2020 2063 6c65 6172             clear
+00005f50: 6162 6c65 3d54 7275 652c 0d0a 2020 2020  able=True,..    
+00005f60: 2020 2020 292c 0d0a 2020 2020 2020 2020      ),..        
+00005f70: 496e 7075 7454 6578 7428 0d0a 2020 2020  InputText(..    
+00005f80: 2020 2020 2020 2020 6c61 6265 6c3d 22e6          label=".
+00005f90: 95b4 e4bd 93e7 bb84 e7bb 8749 4422 2c0d  ...........ID",.
+00005fa0: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
+00005fb0: 6372 6970 7469 6f6e 3d22 e887 aae8 a18c  cription="......
+00005fc0: e68a 93e5 8c85 e88e b7e5 8f96 efbc 8ce5  ................
+00005fd0: afb9 e5ba 946f 7267 222c 0d0a 2020 2020  .....org",..    
+00005fe0: 2020 2020 2020 2020 6e61 6d65 3d22 6f72          name="or
+00005ff0: 6722 2c0d 0a20 2020 2020 2020 2020 2020  g",..           
+00006000: 2069 6e6c 696e 653d 4661 6c73 652c 0d0a   inline=False,..
+00006010: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+00006020: 6972 6564 3d54 7275 652c 0d0a 2020 2020  ired=True,..    
+00006030: 2020 2020 2020 2020 7661 6c75 653d 2222          value=""
+00006040: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
+00006050: 6c65 6172 6162 6c65 3d54 7275 652c 0d0a  learable=True,..
+00006060: 2020 2020 2020 2020 292c 0d0a 2020 2020          ),..    
+00006070: 2020 2020 496e 7075 7454 6578 7428 0d0a      InputText(..
+00006080: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+00006090: 6c3d 22e7 bb84 e7bb 8749 4422 2c0d 0a20  l="......ID",.. 
+000060a0: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+000060b0: 6970 7469 6f6e 3d22 e887 aae8 a18c e68a  iption="........
+000060c0: 93e5 8c85 e88e b7e5 8f96 efbc 8ce5 afb9  ................
+000060d0: e5ba 946c 6173 744f 7267 222c 0d0a 2020  ...lastOrg",..  
+000060e0: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
+000060f0: 6c61 7374 4f72 6722 2c0d 0a20 2020 2020  lastOrg",..     
+00006100: 2020 2020 2020 2069 6e6c 696e 653d 4661         inline=Fa
+00006110: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+00006120: 2020 7265 7175 6972 6564 3d54 7275 652c    required=True,
+00006130: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
+00006140: 6c75 653d 2222 2c0d 0a20 2020 2020 2020  lue="",..       
+00006150: 2020 2020 2063 6c65 6172 6162 6c65 3d54       clearable=T
+00006160: 7275 652c 0d0a 2020 2020 2020 2020 292c  rue,..        ),
+00006170: 0d0a 2020 2020 2020 2020 496e 7075 7454  ..        InputT
+00006180: 6578 7428 0d0a 2020 2020 2020 2020 2020  ext(..          
+00006190: 2020 6c61 6265 6c3d 22e5 9ba2 e694 afe9    label=".......
+000061a0: 83a8 e590 8de7 a7b0 222c 0d0a 2020 2020  ........",..    
+000061b0: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+000061c0: 696f 6e3d 22e8 87aa e8a1 8ce6 8a93 e58c  ion="...........
+000061d0: 85e8 8eb7 e58f 96ef bc8c e5af b9e5 ba94  ................
+000061e0: 206f 7267 4e61 6d65 222c 0d0a 2020 2020   orgName",..    
+000061f0: 2020 2020 2020 2020 6e61 6d65 3d22 6f72          name="or
+00006200: 674e 616d 6522 2c0d 0a20 2020 2020 2020  gName",..       
+00006210: 2020 2020 2069 6e6c 696e 653d 4661 6c73       inline=Fals
+00006220: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00006230: 7265 7175 6972 6564 3d54 7275 652c 0d0a  required=True,..
+00006240: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00006250: 653d 2222 2c0d 0a20 2020 2020 2020 2020  e="",..         
+00006260: 2020 2063 6c65 6172 6162 6c65 3d54 7275     clearable=Tru
+00006270: 652c 0d0a 2020 2020 2020 2020 292c 2049  e,..        ), I
+00006280: 6e70 7574 5465 7874 280d 0a20 2020 2020  nputText(..     
+00006290: 2020 2020 2020 206c 6162 656c 3d22 e7bb         label="..
+000062a0: 84e7 bb87 e585 a8e7 a7b0 222c 0d0a 2020  ..........",..  
+000062b0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+000062c0: 7074 696f 6e3d 22e8 87aa e8a1 8ce6 8a93  ption=".........
+000062d0: e58c 85e8 8eb7 e58f 96ef bc8c e5af b9e5  ................
+000062e0: ba94 616c 6c4f 7267 4e61 6d65 222c 0d0a  ..allOrgName",..
+000062f0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+00006300: 3d22 616c 6c4f 7267 4e61 6d65 222c 0d0a  ="allOrgName",..
+00006310: 2020 2020 2020 2020 2020 2020 696e 6c69              inli
+00006320: 6e65 3d46 616c 7365 2c0d 0a20 2020 2020  ne=False,..     
+00006330: 2020 2020 2020 2072 6571 7569 7265 643d         required=
+00006340: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+00006350: 2020 2076 616c 7565 3d22 222c 0d0a 2020     value="",..  
+00006360: 2020 2020 2020 2020 2020 636c 6561 7261            cleara
+00006370: 626c 653d 5472 7565 2c0d 0a20 2020 2020  ble=True,..     
+00006380: 2020 2029 0d0a 0d0a 2020 2020 5d0d 0a29     )....    ]..)
+00006390: 0d0a 2222 22e5 b1b1 e4b8 9ce6 b7bb e58a  .."""...........
+000063a0: a0e6 8890 e591 98e9 9da2 e69d bf22 2222  ............."""
+000063b0: 0d0a 7368 616e 646f 6e67 5f74 6162 6c65  ..shandong_table
+000063c0: 203d 2046 6f72 6d28 0d0a 2020 2020 7469   = Form(..    ti
+000063d0: 746c 653d 22e6 b7bb e58a a0e9 9d92 e698  tle="...........
+000063e0: a5e5 b1b1 e4b8 9ce7 94a8 e688 b722 2c0d  .............",.
+000063f0: 0a20 2020 2073 756e 6d69 7454 6578 743d  .    sunmitText=
+00006400: 22e6 b7bb e58a a022 2c0d 0a20 2020 206d  "......",..    m
+00006410: 6f64 653d 4469 7370 6c61 794d 6f64 6545  ode=DisplayModeE
+00006420: 6e75 6d2e 686f 7269 7a6f 6e74 616c 2c0d  num.horizontal,.
+00006430: 0a20 2020 2061 7069 3d22 706f 7374 3a2f  .    api="post:/
+00006440: 5465 656e 5374 7564 792f 6170 692f 7368  TeenStudy/api/sh
+00006450: 616e 646f 6e67 2f61 6464 222c 0d0a 2020  andong/add",..  
+00006460: 2020 7265 7365 7441 6674 6572 5375 626d    resetAfterSubm
+00006470: 6974 3d54 7275 652c 0d0a 2020 2020 626f  it=True,..    bo
+00006480: 6479 3d5b 0d0a 2020 2020 2020 2020 5365  dy=[..        Se
+00006490: 6c65 6374 280d 0a20 2020 2020 2020 2020  lect(..         
+000064a0: 2020 206c 6162 656c 3d22 e7be a4e8 818a     label="......
+000064b0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000064c0: 6e61 6d65 3d22 6772 6f75 705f 6964 222c  name="group_id",
+000064d0: 0d0a 2020 2020 2020 2020 2020 2020 6465  ..            de
+000064e0: 7363 7269 7074 696f 6e3d 22e9 9c80 e8a6  scription=".....
+000064f0: 81e6 b7bb e58a a0e7 9a84 e7be a4e7 bb84  ................
+00006500: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00006510: 6368 6563 6b41 6c6c 3d46 616c 7365 2c0d  checkAll=False,.
+00006520: 0a20 2020 2020 2020 2020 2020 2073 6f75  .            sou
+00006530: 7263 653d 2267 6574 3a2f 5465 656e 5374  rce="get:/TeenSt
+00006540: 7564 792f 6170 692f 6765 745f 6772 6f75  udy/api/get_grou
+00006550: 705f 6c69 7374 222c 0d0a 2020 2020 2020  p_list",..      
+00006560: 2020 2020 2020 7661 6c75 653d 2727 2c0d        value='',.
+00006570: 0a20 2020 2020 2020 2020 2020 206d 756c  .            mul
+00006580: 7469 706c 653d 4661 6c73 652c 0d0a 2020  tiple=False,..  
+00006590: 2020 2020 2020 2020 2020 7265 7175 6972            requir
+000065a0: 6564 3d54 7275 652c 0d0a 2020 2020 2020  ed=True,..      
+000065b0: 2020 2020 2020 7365 6172 6368 6162 6c65        searchable
+000065c0: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+000065d0: 2020 2020 6a6f 696e 5661 6c75 6573 3d46      joinValues=F
+000065e0: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
+000065f0: 2020 2065 7874 7261 6374 5661 6c75 653d     extractValue=
+00006600: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+00006610: 2020 2073 7461 7469 7374 6963 733d 5472     statistics=Tr
+00006620: 7565 2c0d 0a20 2020 2020 2020 2029 2c0d  ue,..        ),.
+00006630: 0a20 2020 2020 2020 2053 656c 6563 7428  .        Select(
+00006640: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
+00006650: 6265 6c3d 22e7 94a8 e688 b749 4422 2c0d  bel="......ID",.
+00006660: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+00006670: 653d 2275 7365 725f 6964 222c 0d0a 2020  e="user_id",..  
+00006680: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+00006690: 7074 696f 6e3d 22e9 9c80 e8a6 81e6 b7bb  ption=".........
+000066a0: e58a a0e7 9a84 e794 a8e6 88b7 4944 222c  ............ID",
+000066b0: 0d0a 2020 2020 2020 2020 2020 2020 6368  ..            ch
+000066c0: 6563 6b41 6c6c 3d46 616c 7365 2c0d 0a20  eckAll=False,.. 
+000066d0: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
+000066e0: 653d 2267 6574 3a2f 5465 656e 5374 7564  e="get:/TeenStud
+000066f0: 792f 6170 692f 6765 745f 6d65 6d62 6572  y/api/get_member
+00006700: 5f6c 6973 743f 6772 6f75 705f 6964 3d24  _list?group_id=$
+00006710: 7b67 726f 7570 5f69 647d 222c 0d0a 2020  {group_id}",..  
+00006720: 2020 2020 2020 2020 2020 7661 6c75 653d            value=
+00006730: 2727 2c0d 0a20 2020 2020 2020 2020 2020  '',..           
+00006740: 206d 756c 7469 706c 653d 4661 6c73 652c   multiple=False,
+00006750: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00006760: 7175 6972 6564 3d54 7275 652c 0d0a 2020  quired=True,..  
+00006770: 2020 2020 2020 2020 2020 7365 6172 6368            search
+00006780: 6162 6c65 3d54 7275 652c 0d0a 2020 2020  able=True,..    
+00006790: 2020 2020 2020 2020 6a6f 696e 5661 6c75          joinValu
+000067a0: 6573 3d46 616c 7365 2c0d 0a20 2020 2020  es=False,..     
+000067b0: 2020 2020 2020 2065 7874 7261 6374 5661         extractVa
+000067c0: 6c75 653d 5472 7565 2c0d 0a20 2020 2020  lue=True,..     
+000067d0: 2020 2020 2020 2073 7461 7469 7374 6963         statistic
+000067e0: 733d 5472 7565 2c0d 0a20 2020 2020 2020  s=True,..       
+000067f0: 2020 2020 2068 6964 6465 6e4f 6e3d 2224       hiddenOn="$
+00006800: 7b67 726f 7570 5f69 643d 3d27 273f 7472  {group_id==''?tr
+00006810: 7565 3a66 616c 7365 7d22 0d0a 2020 2020  ue:false}"..    
+00006820: 2020 2020 292c 0d0a 2020 2020 2020 2020      ),..        
+00006830: 496e 7075 7454 6578 7428 0d0a 2020 2020  InputText(..    
+00006840: 2020 2020 2020 2020 6c61 6265 6c3d 22e5          label=".
+00006850: 9cb0 e58c ba22 2c0d 0a20 2020 2020 2020  .....",..       
+00006860: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00006870: 3d22 e689 80e5 a484 e79c 81e4 bbbd 222c  ="............",
+00006880: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
+00006890: 6d65 3d22 6172 6561 222c 0d0a 2020 2020  me="area",..    
+000068a0: 2020 2020 2020 2020 7661 6c75 653d 22e5          value=".
+000068b0: b1b1 e4b8 9c22 2c0d 0a20 2020 2020 2020  .....",..       
+000068c0: 2020 2020 2064 6973 6162 6c65 643d 5472       disabled=Tr
+000068d0: 7565 0d0a 2020 2020 2020 2020 292c 0d0a  ue..        ),..
+000068e0: 2020 2020 2020 2020 496e 7075 7454 6578          InputTex
+000068f0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+00006900: 6c61 6265 6c3d 22e7 99bb e5bd 95e5 af86  label=".........
+00006910: e7a0 8122 2c0d 0a20 2020 2020 2020 2020  ...",..         
+00006920: 2020 2074 7970 653d 2769 6e70 7574 2d70     type='input-p
+00006930: 6173 7377 6f72 6427 2c0d 0a20 2020 2020  assword',..     
+00006940: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+00006950: 6f6e 3d22 e58f afe4 b88d e5a1 abef bc8c  on="............
+00006960: e9bb 98e8 aea4 e4b8 bae7 94a8 e688 b749  ...............I
+00006970: 4422 2c0d 0a20 2020 2020 2020 2020 2020  D",..           
+00006980: 206e 616d 653d 2270 6173 7377 6f72 6422   name="password"
+00006990: 2c0d 0a20 2020 2020 2020 2020 2020 2069  ,..            i
+000069a0: 6e6c 696e 653d 4661 6c73 652c 0d0a 2020  nline=False,..  
+000069b0: 2020 2020 2020 2020 2020 7265 7175 6972            requir
+000069c0: 6564 3d46 616c 7365 2c0d 0a20 2020 2020  ed=False,..     
+000069d0: 2020 2020 2020 2076 616c 7565 3d22 222c         value="",
+000069e0: 0d0a 2020 2020 2020 2020 2020 2020 636c  ..            cl
+000069f0: 6561 7261 626c 653d 5472 7565 2c0d 0a20  earable=True,.. 
+00006a00: 2020 2020 2020 2020 2020 206d 6178 4c65             maxLe
+00006a10: 6e67 7468 3d31 360d 0a20 2020 2020 2020  ngth=16..       
+00006a20: 2029 2c0d 0a20 2020 2020 2020 2049 6e70   ),..        Inp
+00006a30: 7574 5465 7874 280d 0a20 2020 2020 2020  utText(..       
+00006a40: 2020 2020 206c 6162 656c 3d22 e5a7 93e5       label="....
+00006a50: 908d 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
+00006a60: 2020 6465 7363 7269 7074 696f 6e3d 22e5    description=".
+00006a70: afb9 e5ba 94e9 9d92 e698 a5e5 b1b1 e4b8  ................
+00006a80: 9ce4 b8aa e4ba bae4 bfa1 e681 afe9 a1b5  ................
+00006a90: 20e6 82a8 e79a 84e5 a793 e590 8d22 2c0d   ............",.
+00006aa0: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+00006ab0: 653d 226e 616d 6522 2c0d 0a20 2020 2020  e="name",..     
+00006ac0: 2020 2020 2020 2069 6e6c 696e 653d 4661         inline=Fa
+00006ad0: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+00006ae0: 2020 7265 7175 6972 6564 3d54 7275 652c    required=True,
+00006af0: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
+00006b00: 6c75 653d 2222 2c0d 0a20 2020 2020 2020  lue="",..       
+00006b10: 2020 2020 2063 6c65 6172 6162 6c65 3d54       clearable=T
+00006b20: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+00006b30: 2020 6d61 784c 656e 6774 683d 380d 0a20    maxLength=8.. 
+00006b40: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
+00006b50: 2020 2049 6e70 7574 5465 7874 280d 0a20     InputText(.. 
+00006b60: 2020 2020 2020 2020 2020 206c 6162 656c             label
+00006b70: 3d22 636f 6f6b 6965 222c 0d0a 2020 2020  ="cookie",..    
+00006b80: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+00006b90: 696f 6e3d 22e8 87aa e8a1 8ce6 8a93 e58c  ion="...........
+00006ba0: 85e8 8eb7 e58f 96ef bc8c e7bb 93e6 9e84  ................
+00006bb0: e4b8 baef bc9a 4a53 4553 5349 4f4e 4944  ......JSESSIONID
+00006bc0: 3d31 3837 3346 5858 5858 5858 5858 3544  =1873FXXXXXXXX5D
+00006bd0: 4643 4246 3143 4331 3337 3033 222c 0d0a  FCBF1CC13703",..
+00006be0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+00006bf0: 3d22 636f 6f6b 6965 222c 0d0a 2020 2020  ="cookie",..    
+00006c00: 2020 2020 2020 2020 696e 6c69 6e65 3d46          inline=F
+00006c10: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
+00006c20: 2020 2072 6571 7569 7265 643d 5472 7565     required=True
+00006c30: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
+00006c40: 616c 7565 3d22 222c 0d0a 2020 2020 2020  alue="",..      
+00006c50: 2020 2020 2020 636c 6561 7261 626c 653d        clearable=
+00006c60: 5472 7565 2c0d 0a20 2020 2020 2020 2029  True,..        )
+00006c70: 2c0d 0a20 2020 2020 2020 2049 6e70 7574  ,..        Input
+00006c80: 5465 7874 280d 0a20 2020 2020 2020 2020  Text(..         
+00006c90: 2020 206c 6162 656c 3d22 6f70 656e 6964     label="openid
+00006ca0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00006cb0: 6465 7363 7269 7074 696f 6e3d 22e8 87aa  description="...
+00006cc0: e8a1 8ce6 8a93 e58c 85e8 8eb7 e58f 96ef  ................
+00006cd0: bc8c e7bb 93e6 9e84 e4b8 baef bc9a 6f68  ..............oh
+00006ce0: 7a39 7878 7878 7878 7878 7878 7878 6c46  z9xxxxxxxxxxxxlF
+00006cf0: 3049 6f30 7543 6e4d 222c 0d0a 2020 2020  0Io0uCnM",..    
+00006d00: 2020 2020 2020 2020 6e61 6d65 3d22 6f70          name="op
+00006d10: 656e 6964 222c 0d0a 2020 2020 2020 2020  enid",..        
+00006d20: 2020 2020 696e 6c69 6e65 3d46 616c 7365      inline=False
+00006d30: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+00006d40: 6571 7569 7265 643d 5472 7565 2c0d 0a20  equired=True,.. 
+00006d50: 2020 2020 2020 2020 2020 2076 616c 7565             value
+00006d60: 3d22 222c 0d0a 2020 2020 2020 2020 2020  ="",..          
+00006d70: 2020 636c 6561 7261 626c 653d 5472 7565    clearable=True
+00006d80: 2c0d 0a20 2020 2020 2020 2029 0d0a 0d0a  ,..        )....
+00006d90: 2020 2020 5d0d 0a29 0d0a 2222 22e9 878d      ]..).."""...
+00006da0: e5ba 86e6 b7bb e58a a0e6 8890 e591 98e9  ................
+00006db0: 9da2 e69d bf22 2222 0d0a 6368 6f6e 6771  ....."""..chongq
+00006dc0: 696e 675f 7461 626c 6520 3d20 466f 726d  ing_table = Form
+00006dd0: 280d 0a20 2020 2074 6974 6c65 3d22 e6b7  (..    title="..
+00006de0: bbe5 8aa0 e987 8de5 ba86 e585 b1e9 9d92  ................
+00006df0: e59b a2e7 94a8 e688 b722 2c0d 0a20 2020  .........",..   
+00006e00: 2073 756e 6d69 7454 6578 743d 22e6 b7bb   sunmitText="...
+00006e10: e58a a022 2c0d 0a20 2020 206d 6f64 653d  ...",..    mode=
+00006e20: 4469 7370 6c61 794d 6f64 6545 6e75 6d2e  DisplayModeEnum.
+00006e30: 686f 7269 7a6f 6e74 616c 2c0d 0a20 2020  horizontal,..   
+00006e40: 2061 7069 3d22 706f 7374 3a2f 5465 656e   api="post:/Teen
+00006e50: 5374 7564 792f 6170 692f 6368 6f6e 6771  Study/api/chongq
+00006e60: 696e 672f 6164 6422 2c0d 0a20 2020 2072  ing/add",..    r
+00006e70: 6573 6574 4166 7465 7253 7562 6d69 743d  esetAfterSubmit=
+00006e80: 5472 7565 2c0d 0a20 2020 2062 6f64 793d  True,..    body=
+00006e90: 5b0d 0a20 2020 2020 2020 2053 656c 6563  [..        Selec
+00006ea0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+00006eb0: 6c61 6265 6c3d 22e7 bea4 e881 8a22 2c0d  label="......",.
+00006ec0: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+00006ed0: 653d 2267 726f 7570 5f69 6422 2c0d 0a20  e="group_id",.. 
+00006ee0: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+00006ef0: 6970 7469 6f6e 3d22 e99c 80e8 a681 e6b7  iption="........
+00006f00: bbe5 8aa0 e79a 84e7 bea4 e7bb 8422 2c0d  .............",.
+00006f10: 0a20 2020 2020 2020 2020 2020 2063 6865  .            che
+00006f20: 636b 416c 6c3d 4661 6c73 652c 0d0a 2020  ckAll=False,..  
+00006f30: 2020 2020 2020 2020 2020 736f 7572 6365            source
+00006f40: 3d22 6765 743a 2f54 6565 6e53 7475 6479  ="get:/TeenStudy
+00006f50: 2f61 7069 2f67 6574 5f67 726f 7570 5f6c  /api/get_group_l
+00006f60: 6973 7422 2c0d 0a20 2020 2020 2020 2020  ist",..         
+00006f70: 2020 2076 616c 7565 3d27 272c 0d0a 2020     value='',..  
+00006f80: 2020 2020 2020 2020 2020 6d75 6c74 6970            multip
+00006f90: 6c65 3d46 616c 7365 2c0d 0a20 2020 2020  le=False,..     
+00006fa0: 2020 2020 2020 2072 6571 7569 7265 643d         required=
+00006fb0: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+00006fc0: 2020 2073 6561 7263 6861 626c 653d 5472     searchable=Tr
+00006fd0: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
+00006fe0: 206a 6f69 6e56 616c 7565 733d 4661 6c73   joinValues=Fals
+00006ff0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00007000: 6578 7472 6163 7456 616c 7565 3d54 7275  extractValue=Tru
+00007010: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00007020: 7374 6174 6973 7469 6373 3d54 7275 652c  statistics=True,
+00007030: 0d0a 2020 2020 2020 2020 292c 0d0a 2020  ..        ),..  
+00007040: 2020 2020 2020 5365 6c65 6374 280d 0a20        Select(.. 
+00007050: 2020 2020 2020 2020 2020 206c 6162 656c             label
+00007060: 3d22 e794 a8e6 88b7 4944 222c 0d0a 2020  ="......ID",..  
+00007070: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
+00007080: 7573 6572 5f69 6422 2c0d 0a20 2020 2020  user_id",..     
+00007090: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+000070a0: 6f6e 3d22 e99c 80e8 a681 e6b7 bbe5 8aa0  on="............
+000070b0: e79a 84e7 94a8 e688 b749 4422 2c0d 0a20  .........ID",.. 
+000070c0: 2020 2020 2020 2020 2020 2063 6865 636b             check
+000070d0: 416c 6c3d 4661 6c73 652c 0d0a 2020 2020  All=False,..    
+000070e0: 2020 2020 2020 2020 736f 7572 6365 3d22          source="
+000070f0: 6765 743a 2f54 6565 6e53 7475 6479 2f61  get:/TeenStudy/a
+00007100: 7069 2f67 6574 5f6d 656d 6265 725f 6c69  pi/get_member_li
+00007110: 7374 3f67 726f 7570 5f69 643d 247b 6772  st?group_id=${gr
+00007120: 6f75 705f 6964 7d22 2c0d 0a20 2020 2020  oup_id}",..     
+00007130: 2020 2020 2020 2076 616c 7565 3d27 272c         value='',
+00007140: 0d0a 2020 2020 2020 2020 2020 2020 6d75  ..            mu
+00007150: 6c74 6970 6c65 3d46 616c 7365 2c0d 0a20  ltiple=False,.. 
+00007160: 2020 2020 2020 2020 2020 2072 6571 7569             requi
+00007170: 7265 643d 5472 7565 2c0d 0a20 2020 2020  red=True,..     
+00007180: 2020 2020 2020 2073 6561 7263 6861 626c         searchabl
+00007190: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
+000071a0: 2020 2020 206a 6f69 6e56 616c 7565 733d       joinValues=
+000071b0: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+000071c0: 2020 2020 6578 7472 6163 7456 616c 7565      extractValue
+000071d0: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+000071e0: 2020 2020 7374 6174 6973 7469 6373 3d54      statistics=T
+000071f0: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+00007200: 2020 6869 6464 656e 4f6e 3d22 247b 6772    hiddenOn="${gr
+00007210: 6f75 705f 6964 3d3d 2727 3f74 7275 653a  oup_id==''?true:
+00007220: 6661 6c73 657d 220d 0a20 2020 2020 2020  false}"..       
+00007230: 2029 2c0d 0a20 2020 2020 2020 2049 6e70   ),..        Inp
+00007240: 7574 5465 7874 280d 0a20 2020 2020 2020  utText(..       
+00007250: 2020 2020 206c 6162 656c 3d22 e59c b0e5       label="....
+00007260: 8cba 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
+00007270: 2020 6465 7363 7269 7074 696f 6e3d 22e6    description=".
+00007280: 8980 e5a4 84e7 9c81 e4bb bd22 2c0d 0a20  ...........",.. 
+00007290: 2020 2020 2020 2020 2020 206e 616d 653d             name=
+000072a0: 2261 7265 6122 2c0d 0a20 2020 2020 2020  "area",..       
+000072b0: 2020 2020 2076 616c 7565 3d22 e987 8de5       value="....
+000072c0: ba86 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
+000072d0: 2020 6469 7361 626c 6564 3d54 7275 650d    disabled=True.
+000072e0: 0a20 2020 2020 2020 2029 2c0d 0a20 2020  .        ),..   
+000072f0: 2020 2020 2049 6e70 7574 5465 7874 280d       InputText(.
+00007300: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+00007310: 656c 3d22 e799 bbe5 bd95 e5af 86e7 a081  el="............
+00007320: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00007330: 7479 7065 3d27 696e 7075 742d 7061 7373  type='input-pass
+00007340: 776f 7264 272c 0d0a 2020 2020 2020 2020  word',..        
+00007350: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
+00007360: 22e5 8faf e4b8 8de5 a1ab efbc 8ce9 bb98  "...............
+00007370: e8ae a4e4 b8ba e794 a8e6 88b7 4944 222c  ............ID",
+00007380: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
+00007390: 6d65 3d22 7061 7373 776f 7264 222c 0d0a  me="password",..
+000073a0: 2020 2020 2020 2020 2020 2020 696e 6c69              inli
+000073b0: 6e65 3d46 616c 7365 2c0d 0a20 2020 2020  ne=False,..     
+000073c0: 2020 2020 2020 2072 6571 7569 7265 643d         required=
+000073d0: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+000073e0: 2020 2020 7661 6c75 653d 2222 2c0d 0a20      value="",.. 
+000073f0: 2020 2020 2020 2020 2020 2063 6c65 6172             clear
+00007400: 6162 6c65 3d54 7275 652c 0d0a 2020 2020  able=True,..    
+00007410: 2020 2020 2020 2020 6d61 784c 656e 6774          maxLengt
+00007420: 683d 3136 0d0a 2020 2020 2020 2020 292c  h=16..        ),
+00007430: 0d0a 2020 2020 2020 2020 496e 7075 7454  ..        InputT
+00007440: 6578 7428 0d0a 2020 2020 2020 2020 2020  ext(..          
+00007450: 2020 6c61 6265 6c3d 22e5 a793 e590 8d22    label="......"
+00007460: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
+00007470: 6573 6372 6970 7469 6f6e 3d22 e5af b9e5  escription="....
+00007480: ba94 e987 8de5 ba86 e585 b1e9 9d92 e59b  ................
+00007490: a2e4 b8aa e4ba bae4 bfa1 e681 afe9 a1b5  ................
+000074a0: 20e6 82a8 e79a 84e5 a793 e590 8d22 2c0d   ............",.
+000074b0: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+000074c0: 653d 226e 616d 6522 2c0d 0a20 2020 2020  e="name",..     
+000074d0: 2020 2020 2020 2069 6e6c 696e 653d 4661         inline=Fa
+000074e0: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+000074f0: 2020 7265 7175 6972 6564 3d54 7275 652c    required=True,
+00007500: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
+00007510: 6c75 653d 2222 2c0d 0a20 2020 2020 2020  lue="",..       
+00007520: 2020 2020 2063 6c65 6172 6162 6c65 3d54       clearable=T
+00007530: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+00007540: 2020 6d61 784c 656e 6774 683d 380d 0a20    maxLength=8.. 
+00007550: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
+00007560: 2020 2049 6e70 7574 5465 7874 280d 0a20     InputText(.. 
+00007570: 2020 2020 2020 2020 2020 206c 6162 656c             label
+00007580: 3d22 6f70 656e 6964 222c 0d0a 2020 2020  ="openid",..    
+00007590: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+000075a0: 696f 6e3d 22e8 87aa e8a1 8ce6 8a93 e58c  ion="...........
+000075b0: 85e8 8eb7 e58f 96ef bc8c e7bb 93e6 9e84  ................
+000075c0: e4b8 ba3a 206f 687a 3978 7878 7878 7878  ...: ohz9xxxxxxx
+000075d0: 7878 7878 786c 4630 496f 3075 436e 4d22  xxxxxlF0Io0uCnM"
+000075e0: 2c0d 0a20 2020 2020 2020 2020 2020 206e  ,..            n
+000075f0: 616d 653d 226f 7065 6e69 6422 2c0d 0a20  ame="openid",.. 
+00007600: 2020 2020 2020 2020 2020 2069 6e6c 696e             inlin
+00007610: 653d 4661 6c73 652c 0d0a 2020 2020 2020  e=False,..      
+00007620: 2020 2020 2020 7265 7175 6972 6564 3d54        required=T
+00007630: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+00007640: 2020 7661 6c75 653d 2222 2c0d 0a20 2020    value="",..   
+00007650: 2020 2020 2020 2020 2063 6c65 6172 6162           clearab
+00007660: 6c65 3d54 7275 652c 0d0a 2020 2020 2020  le=True,..      
+00007670: 2020 290d 0a0d 0a20 2020 205d 0d0a 290d    )....    ]..).
+00007680: 0a22 2222 e590 89e6 9e97 e6b7 bbe5 8aa0  ."""............
+00007690: e688 90e5 9198 e99d a2e6 9dbf 2222 220d  ............""".
+000076a0: 0a6a 696c 696e 5f74 6162 6c65 203d 2046  .jilin_table = F
+000076b0: 6f72 6d28 0d0a 2020 2020 7469 746c 653d  orm(..    title=
+000076c0: 22e6 b7bb e58a a0e5 9089 e99d 92e9 a39e  "...............
+000076d0: e689 ace7 94a8 e688 b722 2c0d 0a20 2020  .........",..   
+000076e0: 206d 6f64 653d 4469 7370 6c61 794d 6f64   mode=DisplayMod
+000076f0: 6545 6e75 6d2e 686f 7269 7a6f 6e74 616c  eEnum.horizontal
+00007700: 2c0d 0a20 2020 2061 7069 3d22 706f 7374  ,..    api="post
+00007710: 3a2f 5465 656e 5374 7564 792f 6170 692f  :/TeenStudy/api/
+00007720: 6a69 6c69 6e2f 6164 6422 2c0d 0a20 2020  jilin/add",..   
+00007730: 2072 6564 6972 6563 743d 222f 5465 656e   redirect="/Teen
+00007740: 5374 7564 792f 6c6f 6769 6e22 2c0d 0a20  Study/login",.. 
+00007750: 2020 2062 6f64 793d 5b0d 0a20 2020 2020     body=[..     
+00007760: 2020 2053 656c 6563 7428 0d0a 2020 2020     Select(..    
+00007770: 2020 2020 2020 2020 6c61 6265 6c3d 22e7          label=".
+00007780: bea4 e881 8a22 2c0d 0a20 2020 2020 2020  .....",..       
+00007790: 2020 2020 206e 616d 653d 2267 726f 7570       name="group
+000077a0: 5f69 6422 2c0d 0a20 2020 2020 2020 2020  _id",..         
+000077b0: 2020 2064 6573 6372 6970 7469 6f6e 3d22     description="
+000077c0: e99c 80e8 a681 e6b7 bbe5 8aa0 e79a 84e7  ................
+000077d0: bea4 e7bb 8422 2c0d 0a20 2020 2020 2020  .....",..       
+000077e0: 2020 2020 2063 6865 636b 416c 6c3d 4661       checkAll=Fa
+000077f0: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+00007800: 2020 736f 7572 6365 3d22 6765 743a 2f54    source="get:/T
+00007810: 6565 6e53 7475 6479 2f61 7069 2f67 6574  eenStudy/api/get
+00007820: 5f67 726f 7570 5f6c 6973 7422 2c0d 0a20  _group_list",.. 
+00007830: 2020 2020 2020 2020 2020 2076 616c 7565             value
+00007840: 3d27 272c 0d0a 2020 2020 2020 2020 2020  ='',..          
+00007850: 2020 6d75 6c74 6970 6c65 3d46 616c 7365    multiple=False
+00007860: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+00007870: 6571 7569 7265 643d 5472 7565 2c0d 0a20  equired=True,.. 
+00007880: 2020 2020 2020 2020 2020 2073 6561 7263             searc
+00007890: 6861 626c 653d 5472 7565 2c0d 0a20 2020  hable=True,..   
+000078a0: 2020 2020 2020 2020 206a 6f69 6e56 616c           joinVal
+000078b0: 7565 733d 4661 6c73 652c 0d0a 2020 2020  ues=False,..    
+000078c0: 2020 2020 2020 2020 6578 7472 6163 7456          extractV
+000078d0: 616c 7565 3d54 7275 652c 0d0a 2020 2020  alue=True,..    
+000078e0: 2020 2020 2020 2020 7374 6174 6973 7469          statisti
+000078f0: 6373 3d54 7275 652c 0d0a 2020 2020 2020  cs=True,..      
+00007900: 2020 292c 0d0a 2020 2020 2020 2020 5365    ),..        Se
+00007910: 6c65 6374 280d 0a20 2020 2020 2020 2020  lect(..         
+00007920: 2020 206c 6162 656c 3d22 e794 a8e6 88b7     label="......
+00007930: 4944 222c 0d0a 2020 2020 2020 2020 2020  ID",..          
+00007940: 2020 6e61 6d65 3d22 7573 6572 5f69 6422    name="user_id"
+00007950: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
+00007960: 6573 6372 6970 7469 6f6e 3d22 e99c 80e8  escription="....
+00007970: a681 e6b7 bbe5 8aa0 e79a 84e7 94a8 e688  ................
+00007980: b749 4422 2c0d 0a20 2020 2020 2020 2020  .ID",..         
+00007990: 2020 2063 6865 636b 416c 6c3d 4661 6c73     checkAll=Fals
+000079a0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+000079b0: 736f 7572 6365 3d22 6765 743a 2f54 6565  source="get:/Tee
+000079c0: 6e53 7475 6479 2f61 7069 2f67 6574 5f6d  nStudy/api/get_m
+000079d0: 656d 6265 725f 6c69 7374 3f67 726f 7570  ember_list?group
+000079e0: 5f69 643d 247b 6772 6f75 705f 6964 7d22  _id=${group_id}"
+000079f0: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
+00007a00: 616c 7565 3d27 272c 0d0a 2020 2020 2020  alue='',..      
+00007a10: 2020 2020 2020 6d75 6c74 6970 6c65 3d46        multiple=F
+00007a20: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
+00007a30: 2020 2072 6571 7569 7265 643d 5472 7565     required=True
+00007a40: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
+00007a50: 6561 7263 6861 626c 653d 5472 7565 2c0d  earchable=True,.
+00007a60: 0a20 2020 2020 2020 2020 2020 206a 6f69  .            joi
+00007a70: 6e56 616c 7565 733d 4661 6c73 652c 0d0a  nValues=False,..
+00007a80: 2020 2020 2020 2020 2020 2020 6578 7472              extr
+00007a90: 6163 7456 616c 7565 3d54 7275 652c 0d0a  actValue=True,..
+00007aa0: 2020 2020 2020 2020 2020 2020 7374 6174              stat
+00007ab0: 6973 7469 6373 3d54 7275 652c 0d0a 2020  istics=True,..  
+00007ac0: 2020 2020 2020 2020 2020 6869 6464 656e            hidden
+00007ad0: 4f6e 3d22 247b 6772 6f75 705f 6964 3d3d  On="${group_id==
+00007ae0: 2727 3f74 7275 653a 6661 6c73 657d 220d  ''?true:false}".
+00007af0: 0a20 2020 2020 2020 2029 2c0d 0a20 2020  .        ),..   
+00007b00: 2020 2020 2049 6e70 7574 5465 7874 280d       InputText(.
+00007b10: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+00007b20: 656c 3d22 e59c b0e5 8cba 222c 0d0a 2020  el="......",..  
+00007b30: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+00007b40: 7074 696f 6e3d 22e6 8980 e5a4 84e7 9c81  ption=".........
+00007b50: e4bb bd22 2c0d 0a20 2020 2020 2020 2020  ...",..         
+00007b60: 2020 206e 616d 653d 2261 7265 6122 2c0d     name="area",.
+00007b70: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00007b80: 7565 3d22 e590 89e6 9e97 222c 0d0a 2020  ue="......",..  
+00007b90: 2020 2020 2020 2020 2020 6469 7361 626c            disabl
+00007ba0: 6564 3d54 7275 650d 0a20 2020 2020 2020  ed=True..       
+00007bb0: 2029 2c0d 0a20 2020 2020 2020 2049 6e70   ),..        Inp
+00007bc0: 7574 5465 7874 280d 0a20 2020 2020 2020  utText(..       
+00007bd0: 2020 2020 206c 6162 656c 3d22 e799 bbe5       label="....
+00007be0: bd95 e5af 86e7 a081 222c 0d0a 2020 2020  ........",..    
+00007bf0: 2020 2020 2020 2020 7479 7065 3d27 696e          type='in
+00007c00: 7075 742d 7061 7373 776f 7264 272c 0d0a  put-password',..
+00007c10: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+00007c20: 7269 7074 696f 6e3d 22e5 8faf e4b8 8de5  ription=".......
+00007c30: a1ab efbc 8ce9 bb98 e8ae a4e4 b8ba e794  ................
+00007c40: a8e6 88b7 4944 222c 0d0a 2020 2020 2020  ....ID",..      
+00007c50: 2020 2020 2020 6e61 6d65 3d22 7061 7373        name="pass
+00007c60: 776f 7264 222c 0d0a 2020 2020 2020 2020  word",..        
+00007c70: 2020 2020 696e 6c69 6e65 3d46 616c 7365      inline=False
+00007c80: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+00007c90: 6571 7569 7265 643d 4661 6c73 652c 0d0a  equired=False,..
+00007ca0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00007cb0: 653d 2222 2c0d 0a20 2020 2020 2020 2020  e="",..         
+00007cc0: 2020 2063 6c65 6172 6162 6c65 3d54 7275     clearable=Tru
+00007cd0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00007ce0: 6d61 784c 656e 6774 683d 3136 0d0a 2020  maxLength=16..  
+00007cf0: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
+00007d00: 2020 496e 7075 7454 6578 7428 0d0a 2020    InputText(..  
+00007d10: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
+00007d20: 22e5 a793 e590 8d22 2c0d 0a20 2020 2020  "......",..     
+00007d30: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+00007d40: 6f6e 3d22 e682 a8e7 9a84 e5a7 93e5 908d  on="............
+00007d50: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00007d60: 6e61 6d65 3d22 6e61 6d65 222c 0d0a 2020  name="name",..  
+00007d70: 2020 2020 2020 2020 2020 696e 6c69 6e65            inline
+00007d80: 3d46 616c 7365 2c0d 0a20 2020 2020 2020  =False,..       
+00007d90: 2020 2020 2072 6571 7569 7265 643d 5472       required=Tr
+00007da0: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
+00007db0: 2076 616c 7565 3d22 222c 0d0a 2020 2020   value="",..    
+00007dc0: 2020 2020 2020 2020 636c 6561 7261 626c          clearabl
+00007dd0: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
+00007de0: 2020 2020 206d 6178 4c65 6e67 7468 3d38       maxLength=8
+00007df0: 0d0a 2020 2020 2020 2020 292c 0d0a 2020  ..        ),..  
+00007e00: 2020 2020 2020 496e 7075 7454 6578 7428        InputText(
+00007e10: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
+00007e20: 6265 6c3d 226f 7065 6e69 6422 2c0d 0a20  bel="openid",.. 
+00007e30: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+00007e40: 6970 7469 6f6e 3d22 e887 aae8 a18c e68a  iption="........
+00007e50: 93e5 8c85 e88e b7e5 8f96 efbc 8ce7 bb93  ................
+00007e60: e69e 84e4 b8ba 3a20 6f68 7a39 7878 7878  ......: ohz9xxxx
+00007e70: 7878 7878 7878 7878 6c46 3049 6f30 7543  xxxxxxxxlF0Io0uC
+00007e80: 6e4d 222c 0d0a 2020 2020 2020 2020 2020  nM",..          
+00007e90: 2020 6e61 6d65 3d22 6f70 656e 6964 222c    name="openid",
+00007ea0: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+00007eb0: 6c69 6e65 3d46 616c 7365 2c0d 0a20 2020  line=False,..   
+00007ec0: 2020 2020 2020 2020 2072 6571 7569 7265           require
+00007ed0: 643d 5472 7565 2c0d 0a20 2020 2020 2020  d=True,..       
+00007ee0: 2020 2020 2076 616c 7565 3d22 222c 0d0a       value="",..
+00007ef0: 2020 2020 2020 2020 2020 2020 636c 6561              clea
+00007f00: 7261 626c 653d 5472 7565 2c0d 0a20 2020  rable=True,..   
+00007f10: 2020 2020 2029 2c0d 0a20 2020 2020 2020       ),..       
+00007f20: 2049 6e70 7574 5465 7874 280d 0a20 2020   InputText(..   
+00007f30: 2020 2020 2020 2020 206c 6162 656c 3d22           label="
+00007f40: e5ad a6e6 a0a1 222c 0d0a 2020 2020 2020  ......",..      
+00007f50: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00007f60: 6e3d 22e4 bda0 e5b0 b1e8 afbb e79a 84e9  n=".............
+00007f70: ab98 e6a0 a122 2c0d 0a20 2020 2020 2020  .....",..       
+00007f80: 2020 2020 206e 616d 653d 2275 6e69 7665       name="unive
+00007f90: 7273 6974 7922 2c0d 0a20 2020 2020 2020  rsity",..       
+00007fa0: 2020 2020 2069 6e6c 696e 653d 4661 6c73       inline=Fals
+00007fb0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00007fc0: 7265 7175 6972 6564 3d54 7275 652c 0d0a  required=True,..
+00007fd0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00007fe0: 653d 2222 2c0d 0a20 2020 2020 2020 2020  e="",..         
+00007ff0: 2020 2063 6c65 6172 6162 6c65 3d54 7275     clearable=Tru
+00008000: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00008010: 6d61 784c 656e 6774 683d 3234 0d0a 2020  maxLength=24..  
+00008020: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
+00008030: 2020 496e 7075 7454 6578 7428 0d0a 2020    InputText(..  
+00008040: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
+00008050: 22e5 ada6 e999 a222 2c0d 0a20 2020 2020  "......",..     
+00008060: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+00008070: 6f6e 3d22 e5ad a6e9 99a2 e590 8de7 a7b0  on="............
+00008080: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00008090: 6e61 6d65 3d22 636f 6c6c 6567 6522 2c0d  name="college",.
+000080a0: 0a20 2020 2020 2020 2020 2020 2069 6e6c  .            inl
+000080b0: 696e 653d 4661 6c73 652c 0d0a 2020 2020  ine=False,..    
+000080c0: 2020 2020 2020 2020 7265 7175 6972 6564          required
+000080d0: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+000080e0: 2020 2020 7661 6c75 653d 2222 2c0d 0a20      value="",.. 
+000080f0: 2020 2020 2020 2020 2020 2063 6c65 6172             clear
+00008100: 6162 6c65 3d54 7275 652c 0d0a 2020 2020  able=True,..    
+00008110: 2020 2020 2020 2020 6d61 784c 656e 6774          maxLengt
+00008120: 683d 3332 0d0a 2020 2020 2020 2020 292c  h=32..        ),
+00008130: 0d0a 2020 2020 2020 2020 496e 7075 7454  ..        InputT
+00008140: 6578 7428 0d0a 2020 2020 2020 2020 2020  ext(..          
+00008150: 2020 6c61 6265 6c3d 22e5 9ba2 e694 afe9    label=".......
+00008160: 83a8 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
+00008170: 2020 6465 7363 7269 7074 696f 6e3d 22e5    description=".
+00008180: 9ba2 e694 afe9 83a8 7ce7 8fad e7ba a7ef  ........|.......
+00008190: bc8c e6b2 a1e6 9c89 e58f afe4 b88d e5a1  ................
+000081a0: ab22 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
+000081b0: 206e 616d 653d 226f 7267 616e 697a 6174   name="organizat
+000081c0: 696f 6e22 2c0d 0a20 2020 2020 2020 2020  ion",..         
+000081d0: 2020 2069 6e6c 696e 653d 4661 6c73 652c     inline=False,
+000081e0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000081f0: 7175 6972 6564 3d46 616c 7365 2c0d 0a20  quired=False,.. 
+00008200: 2020 2020 2020 2020 2020 2076 616c 7565             value
+00008210: 3d22 222c 0d0a 2020 2020 2020 2020 2020  ="",..          
+00008220: 2020 636c 6561 7261 626c 653d 5472 7565    clearable=True
+00008230: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
+00008240: 6178 4c65 6e67 7468 3d33 320d 0a20 2020  axLength=32..   
+00008250: 2020 2020 2029 0d0a 0d0a 2020 2020 5d0d       )....    ].
+00008260: 0a29 0d0a 2222 22e5 b9bf e4b8 9ce5 9cb0  .)..""".........
+00008270: e58c bae6 b7bb e58a a0e7 94a8 e688 b722  ..............."
+00008280: 2222 0d0a 6775 616e 6764 6f6e 675f 7461  ""..guangdong_ta
+00008290: 626c 6520 3d20 466f 726d 280d 0a20 2020  ble = Form(..   
+000082a0: 2074 6974 6c65 3d22 e6b7 bbe5 8aa0 e5b9   title="........
+000082b0: bfe4 b89c e585 b1e9 9d92 e59b a2e7 94a8  ................
+000082c0: e688 b722 2c0d 0a20 2020 206d 6f64 653d  ...",..    mode=
+000082d0: 4469 7370 6c61 794d 6f64 6545 6e75 6d2e  DisplayModeEnum.
+000082e0: 686f 7269 7a6f 6e74 616c 2c0d 0a20 2020  horizontal,..   
+000082f0: 2061 7069 3d22 706f 7374 3a2f 5465 656e   api="post:/Teen
+00008300: 5374 7564 792f 6170 692f 6775 616e 6764  Study/api/guangd
+00008310: 6f6e 672f 6164 6422 2c0d 0a20 2020 2072  ong/add",..    r
+00008320: 6564 6972 6563 743d 222f 5465 656e 5374  edirect="/TeenSt
+00008330: 7564 792f 6c6f 6769 6e22 2c0d 0a20 2020  udy/login",..   
+00008340: 2062 6f64 793d 5b0d 0a20 2020 2020 2020   body=[..       
+00008350: 2041 6c65 7274 286c 6576 656c 3d4c 6576   Alert(level=Lev
+00008360: 656c 456e 756d 2e69 6e66 6f2c 0d0a 2020  elEnum.info,..  
+00008370: 2020 2020 2020 2020 2020 2020 636c 6173              clas
+00008380: 734e 616d 653d 2777 6869 7465 2d73 7061  sName='white-spa
+00008390: 6365 2d70 7265 2d77 7261 7027 2c0d 0a20  ce-pre-wrap',.. 
+000083a0: 2020 2020 2020 2020 2020 2020 2062 6f64               bod
+000083b0: 793d 280d 0a20 2020 2020 2020 2020 2020  y=(..           
+000083c0: 2020 2020 2020 2022 e993 bee6 8ea5 e88e         "........
+000083d0: b7e5 8f96 e696 b9e5 bc8f 3a5c 6e31 3233  ..........:\n123
+000083e0: 3535 e99d 92e6 98a5 e4b9 8be5 a3b0 e585  55..............
+000083f0: ace4 bc97 e58f b75c 6ee6 99ba e685 a7e5  .......\n.......
+00008400: 9ba2 e5bb ba2d e8ae a4e8 af81 e8b5 84e6  .....-..........
+00008410: 9699 2de7 949f e688 90e7 94b5 e5ad 90e5  ..-.............
+00008420: 9ba2 e591 98e8 af81 efbc 8ce7 82b9 e587  ................
+00008430: bbe6 9c80 e4b8 8be6 96b9 e794 9fe6 8890  ................
+00008440: e68c 89e9 92ae e380 825c 6ee5 9ca8 e59b  .........\n.....
+00008450: a2e5 9198 e8af 81e9 a1b5 e99d a2e5 a48d  ................
+00008460: e588 b6e9 93be e68e a520 e5ba 94e4 b8ba  ......... ......
+00008470: efbc 9a68 7474 7073 3a2f 2f74 7561 6e2e  ...https://tuan.
+00008480: 3132 3335 352e 6e65 742f 7765 6368 6174  12355.net/wechat
+00008490: 2f76 6965 772f 696e 666f 726d 6174 696f  /view/informatio
+000084a0: 6e2f 6d65 6d62 6572 5f63 6572 7469 6669  n/member_certifi
+000084b0: 6361 7469 6f6e 5f67 656e 6572 6174 6564  cation_generated
+000084c0: 2e68 746d 6c3f 6d65 6d62 6572 4964 3d78  .html?memberId=x
+000084d0: 7878 7878 7826 7368 6f77 4d65 6d62 6572  xxxxx&showMember
+000084e0: 4164 6469 7469 6f6e 4e61 6d65 733d 2673  AdditionNames=&s
+000084f0: 686f 774d 656d 6265 7252 6577 6172 6449  howMemberRewardI
+00008500: 6473 3d26 6973 5368 6f77 416c 6c46 6565  ds=&isShowAllFee
+00008510: 3d74 7275 6520 5c6e e585 b6e4 b8ad 7878  =true \n......xx
+00008520: 7878 7878 e58d b3e4 b8ba 6d69 6422 2929  xxxx......mid"))
+00008530: 2c0d 0a20 2020 2020 2020 2053 656c 6563  ,..        Selec
+00008540: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+00008550: 6c61 6265 6c3d 22e7 bea4 e881 8a22 2c0d  label="......",.
+00008560: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+00008570: 653d 2267 726f 7570 5f69 6422 2c0d 0a20  e="group_id",.. 
+00008580: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+00008590: 6970 7469 6f6e 3d22 e99c 80e8 a681 e6b7  iption="........
+000085a0: bbe5 8aa0 e79a 84e7 bea4 e7bb 8422 2c0d  .............",.
+000085b0: 0a20 2020 2020 2020 2020 2020 2063 6865  .            che
+000085c0: 636b 416c 6c3d 4661 6c73 652c 0d0a 2020  ckAll=False,..  
+000085d0: 2020 2020 2020 2020 2020 736f 7572 6365            source
+000085e0: 3d22 6765 743a 2f54 6565 6e53 7475 6479  ="get:/TeenStudy
+000085f0: 2f61 7069 2f67 6574 5f67 726f 7570 5f6c  /api/get_group_l
+00008600: 6973 7422 2c0d 0a20 2020 2020 2020 2020  ist",..         
+00008610: 2020 2076 616c 7565 3d27 272c 0d0a 2020     value='',..  
+00008620: 2020 2020 2020 2020 2020 6d75 6c74 6970            multip
+00008630: 6c65 3d46 616c 7365 2c0d 0a20 2020 2020  le=False,..     
+00008640: 2020 2020 2020 2072 6571 7569 7265 643d         required=
+00008650: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+00008660: 2020 2073 6561 7263 6861 626c 653d 5472     searchable=Tr
+00008670: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
+00008680: 206a 6f69 6e56 616c 7565 733d 4661 6c73   joinValues=Fals
+00008690: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+000086a0: 6578 7472 6163 7456 616c 7565 3d54 7275  extractValue=Tru
+000086b0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+000086c0: 7374 6174 6973 7469 6373 3d54 7275 652c  statistics=True,
+000086d0: 0d0a 2020 2020 2020 2020 292c 0d0a 2020  ..        ),..  
+000086e0: 2020 2020 2020 5365 6c65 6374 280d 0a20        Select(.. 
+000086f0: 2020 2020 2020 2020 2020 206c 6162 656c             label
+00008700: 3d22 e794 a8e6 88b7 4944 222c 0d0a 2020  ="......ID",..  
+00008710: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
+00008720: 7573 6572 5f69 6422 2c0d 0a20 2020 2020  user_id",..     
+00008730: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+00008740: 6f6e 3d22 e99c 80e8 a681 e6b7 bbe5 8aa0  on="............
+00008750: e79a 84e7 94a8 e688 b749 4422 2c0d 0a20  .........ID",.. 
+00008760: 2020 2020 2020 2020 2020 2063 6865 636b             check
+00008770: 416c 6c3d 4661 6c73 652c 0d0a 2020 2020  All=False,..    
+00008780: 2020 2020 2020 2020 736f 7572 6365 3d22          source="
+00008790: 6765 743a 2f54 6565 6e53 7475 6479 2f61  get:/TeenStudy/a
+000087a0: 7069 2f67 6574 5f6d 656d 6265 725f 6c69  pi/get_member_li
+000087b0: 7374 3f67 726f 7570 5f69 643d 247b 6772  st?group_id=${gr
+000087c0: 6f75 705f 6964 7d22 2c0d 0a20 2020 2020  oup_id}",..     
+000087d0: 2020 2020 2020 2076 616c 7565 3d27 272c         value='',
+000087e0: 0d0a 2020 2020 2020 2020 2020 2020 6d75  ..            mu
+000087f0: 6c74 6970 6c65 3d46 616c 7365 2c0d 0a20  ltiple=False,.. 
+00008800: 2020 2020 2020 2020 2020 2072 6571 7569             requi
+00008810: 7265 643d 5472 7565 2c0d 0a20 2020 2020  red=True,..     
+00008820: 2020 2020 2020 2073 6561 7263 6861 626c         searchabl
+00008830: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
+00008840: 2020 2020 206a 6f69 6e56 616c 7565 733d       joinValues=
+00008850: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+00008860: 2020 2020 6578 7472 6163 7456 616c 7565      extractValue
+00008870: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+00008880: 2020 2020 7374 6174 6973 7469 6373 3d54      statistics=T
+00008890: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+000088a0: 2020 6869 6464 656e 4f6e 3d22 247b 6772    hiddenOn="${gr
+000088b0: 6f75 705f 6964 3d3d 2727 3f74 7275 653a  oup_id==''?true:
+000088c0: 6661 6c73 657d 220d 0a20 2020 2020 2020  false}"..       
+000088d0: 2029 2c0d 0a20 2020 2020 2020 2049 6e70   ),..        Inp
+000088e0: 7574 5465 7874 280d 0a20 2020 2020 2020  utText(..       
+000088f0: 2020 2020 206c 6162 656c 3d22 e59c b0e5       label="....
+00008900: 8cba 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
+00008910: 2020 6465 7363 7269 7074 696f 6e3d 22e6    description=".
+00008920: 8980 e5a4 84e7 9c81 e4bb bd22 2c0d 0a20  ...........",.. 
+00008930: 2020 2020 2020 2020 2020 206e 616d 653d             name=
+00008940: 2261 7265 6122 2c0d 0a20 2020 2020 2020  "area",..       
+00008950: 2020 2020 2076 616c 7565 3d22 e5b9 bfe4       value="....
+00008960: b89c 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
+00008970: 2020 6469 7361 626c 6564 3d54 7275 650d    disabled=True.
+00008980: 0a20 2020 2020 2020 2029 2c0d 0a20 2020  .        ),..   
+00008990: 2020 2020 2049 6e70 7574 5465 7874 280d       InputText(.
+000089a0: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+000089b0: 656c 3d22 e799 bbe5 bd95 e5af 86e7 a081  el="............
+000089c0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000089d0: 7479 7065 3d27 696e 7075 742d 7061 7373  type='input-pass
+000089e0: 776f 7264 272c 0d0a 2020 2020 2020 2020  word',..        
+000089f0: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
+00008a00: 22e5 8faf e4b8 8de5 a1ab efbc 8ce9 bb98  "...............
+00008a10: e8ae a4e4 b8ba e794 a8e6 88b7 4944 222c  ............ID",
+00008a20: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
+00008a30: 6d65 3d22 7061 7373 776f 7264 222c 0d0a  me="password",..
+00008a40: 2020 2020 2020 2020 2020 2020 696e 6c69              inli
+00008a50: 6e65 3d46 616c 7365 2c0d 0a20 2020 2020  ne=False,..     
+00008a60: 2020 2020 2020 2072 6571 7569 7265 643d         required=
+00008a70: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+00008a80: 2020 2020 7661 6c75 653d 2222 2c0d 0a20      value="",.. 
+00008a90: 2020 2020 2020 2020 2020 2063 6c65 6172             clear
+00008aa0: 6162 6c65 3d54 7275 652c 0d0a 2020 2020  able=True,..    
+00008ab0: 2020 2020 2020 2020 6d61 784c 656e 6774          maxLengt
+00008ac0: 683d 3136 0d0a 2020 2020 2020 2020 292c  h=16..        ),
+00008ad0: 0d0a 2020 2020 2020 2020 496e 7075 7454  ..        InputT
+00008ae0: 6578 7428 0d0a 2020 2020 2020 2020 2020  ext(..          
+00008af0: 2020 6c61 6265 6c3d 22e5 a793 e590 8d22    label="......"
+00008b00: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
+00008b10: 6573 6372 6970 7469 6f6e 3d22 e682 a8e7  escription="....
+00008b20: 9a84 e5a7 93e5 908d 222c 0d0a 2020 2020  ........",..    
+00008b30: 2020 2020 2020 2020 6e61 6d65 3d22 6e61          name="na
+00008b40: 6d65 222c 0d0a 2020 2020 2020 2020 2020  me",..          
+00008b50: 2020 696e 6c69 6e65 3d46 616c 7365 2c0d    inline=False,.
+00008b60: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
+00008b70: 7569 7265 643d 5472 7565 2c0d 0a20 2020  uired=True,..   
+00008b80: 2020 2020 2020 2020 2076 616c 7565 3d22           value="
+00008b90: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00008ba0: 636c 6561 7261 626c 653d 5472 7565 2c0d  clearable=True,.
+00008bb0: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+00008bc0: 4c65 6e67 7468 3d38 0d0a 2020 2020 2020  Length=8..      
+00008bd0: 2020 292c 0d0a 2020 2020 2020 2020 496e    ),..        In
+00008be0: 7075 7454 6578 7428 0d0a 2020 2020 2020  putText(..      
+00008bf0: 2020 2020 2020 6c61 6265 6c3d 2275 726c        label="url
+00008c00: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00008c10: 6465 7363 7269 7074 696f 6e3d 22e9 93be  description="...
+00008c20: e68e a5e6 a0bc e5bc 8fef bc9a 6874 7470  ............http
+00008c30: 733a 2f2f 7475 616e 2e31 3233 3535 2e6e  s://tuan.12355.n
+00008c40: 6574 2f77 6563 6861 742f 7669 6577 2f69  et/wechat/view/i
+00008c50: 6e66 6f72 6d61 7469 6f6e 2f6d 656d 6265  nformation/membe
+00008c60: 725f 6365 7274 6966 6963 6174 696f 6e5f  r_certification_
+00008c70: 6765 6e65 7261 7465 642e 6874 6d6c 3f6d  generated.html?m
+00008c80: 656d 6265 7249 643d 7878 7878 7878 2673  emberId=xxxxxx&s
+00008c90: 686f 774d 656d 6265 7241 6464 6974 696f  howMemberAdditio
+00008ca0: 6e4e 616d 6573 3d26 7368 6f77 4d65 6d62  nNames=&showMemb
+00008cb0: 6572 5265 7761 7264 4964 733d 2669 7353  erRewardIds=&isS
+00008cc0: 686f 7741 6c6c 4665 653d 7472 7565 222c  howAllFee=true",
+00008cd0: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
+00008ce0: 6d65 3d22 7572 6c22 2c0d 0a20 2020 2020  me="url",..     
+00008cf0: 2020 2020 2020 2069 6e6c 696e 653d 4661         inline=Fa
+00008d00: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+00008d10: 2020 7265 7175 6972 6564 3d54 7275 652c    required=True,
+00008d20: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
+00008d30: 6c75 653d 2222 2c0d 0a20 2020 2020 2020  lue="",..       
+00008d40: 2020 2020 2063 6c65 6172 6162 6c65 3d54       clearable=T
+00008d50: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+00008d60: 2020 6d61 784c 656e 6774 683d 3531 320d    maxLength=512.
+00008d70: 0a20 2020 2020 2020 2029 2c0d 0a20 2020  .        ),..   
+00008d80: 2020 2020 2049 6e70 7574 5465 7874 280d       InputText(.
+00008d90: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+00008da0: 656c 3d22 e5ad a6e6 a0a1 222c 0d0a 2020  el="......",..  
+00008db0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+00008dc0: 7074 696f 6e3d 22e4 bda0 e5b0 b1e8 afbb  ption=".........
+00008dd0: e79a 84e9 ab98 e6a0 a122 2c0d 0a20 2020  .........",..   
+00008de0: 2020 2020 2020 2020 206e 616d 653d 2275           name="u
+00008df0: 6e69 7665 7273 6974 7922 2c0d 0a20 2020  niversity",..   
+00008e00: 2020 2020 2020 2020 2069 6e6c 696e 653d           inline=
+00008e10: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+00008e20: 2020 2020 7265 7175 6972 6564 3d54 7275      required=Tru
+00008e30: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00008e40: 7661 6c75 653d 2222 2c0d 0a20 2020 2020  value="",..     
+00008e50: 2020 2020 2020 2063 6c65 6172 6162 6c65         clearable
+00008e60: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+00008e70: 2020 2020 6d61 784c 656e 6774 683d 3234      maxLength=24
+00008e80: 0d0a 2020 2020 2020 2020 292c 0d0a 2020  ..        ),..  
+00008e90: 2020 2020 2020 496e 7075 7454 6578 7428        InputText(
+00008ea0: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
+00008eb0: 6265 6c3d 22e5 ada6 e999 a222 2c0d 0a20  bel="......",.. 
+00008ec0: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+00008ed0: 6970 7469 6f6e 3d22 e5ad a6e9 99a2 e590  iption="........
+00008ee0: 8de7 a7b0 222c 0d0a 2020 2020 2020 2020  ....",..        
+00008ef0: 2020 2020 6e61 6d65 3d22 636f 6c6c 6567      name="colleg
+00008f00: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
+00008f10: 2069 6e6c 696e 653d 4661 6c73 652c 0d0a   inline=False,..
+00008f20: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+00008f30: 6972 6564 3d54 7275 652c 0d0a 2020 2020  ired=True,..    
+00008f40: 2020 2020 2020 2020 7661 6c75 653d 2222          value=""
+00008f50: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
+00008f60: 6c65 6172 6162 6c65 3d54 7275 652c 0d0a  learable=True,..
+00008f70: 2020 2020 2020 2020 2020 2020 6d61 784c              maxL
+00008f80: 656e 6774 683d 3332 0d0a 2020 2020 2020  ength=32..      
+00008f90: 2020 292c 0d0a 2020 2020 2020 2020 496e    ),..        In
+00008fa0: 7075 7454 6578 7428 0d0a 2020 2020 2020  putText(..      
+00008fb0: 2020 2020 2020 6c61 6265 6c3d 22e5 9ba2        label="...
+00008fc0: e694 afe9 83a8 222c 0d0a 2020 2020 2020  ......",..      
+00008fd0: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00008fe0: 6e3d 22e5 9ba2 e694 afe9 83a8 7ce7 8fad  n=".........|...
+00008ff0: e7ba a7ef bc8c e6b2 a1e6 9c89 e58f afe4  ................
+00009000: b88d e5a1 ab22 2c0d 0a20 2020 2020 2020  .....",..       
+00009010: 2020 2020 206e 616d 653d 226f 7267 616e       name="organ
+00009020: 697a 6174 696f 6e22 2c0d 0a20 2020 2020  ization",..     
+00009030: 2020 2020 2020 2069 6e6c 696e 653d 4661         inline=Fa
+00009040: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+00009050: 2020 7265 7175 6972 6564 3d46 616c 7365    required=False
+00009060: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
+00009070: 616c 7565 3d22 222c 0d0a 2020 2020 2020  alue="",..      
+00009080: 2020 2020 2020 636c 6561 7261 626c 653d        clearable=
+00009090: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+000090a0: 2020 206d 6178 4c65 6e67 7468 3d33 320d     maxLength=32.
+000090b0: 0a20 2020 2020 2020 2029 5d0d 0a29 0d0a  .        )]..)..
+000090c0: 2222 22e5 8c97 e4ba ace5 9cb0 e58c bae6  """.............
+000090d0: b7bb e58a a0e7 94a8 e688 b7e9 9da2 e69d  ................
+000090e0: bf22 2222 0d0a 6265 696a 696e 675f 7461  ."""..beijing_ta
+000090f0: 626c 6520 3d20 466f 726d 280d 0a20 2020  ble = Form(..   
+00009100: 2074 6974 6c65 3d22 e6b7 bbe5 8aa0 e58c   title="........
+00009110: 97e4 baac e585 b1e9 9d92 e59b a2e7 94a8  ................
+00009120: e688 b722 2c0d 0a20 2020 206d 6f64 653d  ...",..    mode=
+00009130: 4469 7370 6c61 794d 6f64 6545 6e75 6d2e  DisplayModeEnum.
+00009140: 686f 7269 7a6f 6e74 616c 2c0d 0a20 2020  horizontal,..   
+00009150: 2061 7069 3d22 706f 7374 3a2f 5465 656e   api="post:/Teen
+00009160: 5374 7564 792f 6170 692f 6265 696a 696e  Study/api/beijin
+00009170: 672f 6164 6422 2c0d 0a20 2020 2072 6564  g/add",..    red
+00009180: 6972 6563 743d 222f 5465 656e 5374 7564  irect="/TeenStud
+00009190: 792f 6c6f 6769 6e22 2c0d 0a20 2020 2062  y/login",..    b
+000091a0: 6f64 793d 5b0d 0a20 2020 2020 2020 2053  ody=[..        S
+000091b0: 656c 6563 7428 0d0a 2020 2020 2020 2020  elect(..        
+000091c0: 2020 2020 6c61 6265 6c3d 22e7 bea4 e881      label=".....
+000091d0: 8a22 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
+000091e0: 206e 616d 653d 2267 726f 7570 5f69 6422   name="group_id"
+000091f0: 2c0d 0a20 2020 2020 2020 2020 2020 2064  ,..            d
+00009200: 6573 6372 6970 7469 6f6e 3d22 e99c 80e8  escription="....
+00009210: a681 e6b7 bbe5 8aa0 e79a 84e7 bea4 e7bb  ................
+00009220: 8422 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
+00009230: 2063 6865 636b 416c 6c3d 4661 6c73 652c   checkAll=False,
+00009240: 0d0a 2020 2020 2020 2020 2020 2020 736f  ..            so
+00009250: 7572 6365 3d22 6765 743a 2f54 6565 6e53  urce="get:/TeenS
+00009260: 7475 6479 2f61 7069 2f67 6574 5f67 726f  tudy/api/get_gro
+00009270: 7570 5f6c 6973 7422 2c0d 0a20 2020 2020  up_list",..     
+00009280: 2020 2020 2020 2076 616c 7565 3d27 272c         value='',
+00009290: 0d0a 2020 2020 2020 2020 2020 2020 6d75  ..            mu
+000092a0: 6c74 6970 6c65 3d46 616c 7365 2c0d 0a20  ltiple=False,.. 
+000092b0: 2020 2020 2020 2020 2020 2072 6571 7569             requi
+000092c0: 7265 643d 5472 7565 2c0d 0a20 2020 2020  red=True,..     
+000092d0: 2020 2020 2020 2073 6561 7263 6861 626c         searchabl
+000092e0: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
+000092f0: 2020 2020 206a 6f69 6e56 616c 7565 733d       joinValues=
+00009300: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+00009310: 2020 2020 6578 7472 6163 7456 616c 7565      extractValue
+00009320: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+00009330: 2020 2020 7374 6174 6973 7469 6373 3d54      statistics=T
+00009340: 7275 652c 0d0a 2020 2020 2020 2020 292c  rue,..        ),
+00009350: 0d0a 2020 2020 2020 2020 5365 6c65 6374  ..        Select
+00009360: 280d 0a20 2020 2020 2020 2020 2020 206c  (..            l
+00009370: 6162 656c 3d22 e794 a8e6 88b7 4944 222c  abel="......ID",
+00009380: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
+00009390: 6d65 3d22 7573 6572 5f69 6422 2c0d 0a20  me="user_id",.. 
+000093a0: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+000093b0: 6970 7469 6f6e 3d22 e99c 80e8 a681 e6b7  iption="........
+000093c0: bbe5 8aa0 e79a 84e7 94a8 e688 b749 4422  .............ID"
+000093d0: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
+000093e0: 6865 636b 416c 6c3d 4661 6c73 652c 0d0a  heckAll=False,..
+000093f0: 2020 2020 2020 2020 2020 2020 736f 7572              sour
+00009400: 6365 3d22 6765 743a 2f54 6565 6e53 7475  ce="get:/TeenStu
+00009410: 6479 2f61 7069 2f67 6574 5f6d 656d 6265  dy/api/get_membe
+00009420: 725f 6c69 7374 3f67 726f 7570 5f69 643d  r_list?group_id=
+00009430: 247b 6772 6f75 705f 6964 7d22 2c0d 0a20  ${group_id}",.. 
+00009440: 2020 2020 2020 2020 2020 2076 616c 7565             value
+00009450: 3d27 272c 0d0a 2020 2020 2020 2020 2020  ='',..          
+00009460: 2020 6d75 6c74 6970 6c65 3d46 616c 7365    multiple=False
+00009470: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+00009480: 6571 7569 7265 643d 5472 7565 2c0d 0a20  equired=True,.. 
+00009490: 2020 2020 2020 2020 2020 2073 6561 7263             searc
+000094a0: 6861 626c 653d 5472 7565 2c0d 0a20 2020  hable=True,..   
+000094b0: 2020 2020 2020 2020 206a 6f69 6e56 616c           joinVal
+000094c0: 7565 733d 4661 6c73 652c 0d0a 2020 2020  ues=False,..    
+000094d0: 2020 2020 2020 2020 6578 7472 6163 7456          extractV
+000094e0: 616c 7565 3d54 7275 652c 0d0a 2020 2020  alue=True,..    
+000094f0: 2020 2020 2020 2020 7374 6174 6973 7469          statisti
+00009500: 6373 3d54 7275 652c 0d0a 2020 2020 2020  cs=True,..      
+00009510: 2020 2020 2020 6869 6464 656e 4f6e 3d22        hiddenOn="
+00009520: 247b 6772 6f75 705f 6964 3d3d 2727 3f74  ${group_id==''?t
+00009530: 7275 653a 6661 6c73 657d 220d 0a20 2020  rue:false}"..   
+00009540: 2020 2020 2029 2c0d 0a20 2020 2020 2020       ),..       
+00009550: 2049 6e70 7574 5465 7874 280d 0a20 2020   InputText(..   
+00009560: 2020 2020 2020 2020 206c 6162 656c 3d22           label="
+00009570: e59c b0e5 8cba 222c 0d0a 2020 2020 2020  ......",..      
+00009580: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00009590: 6e3d 22e6 8980 e5a4 84e7 9c81 e4bb bd22  n="............"
+000095a0: 2c0d 0a20 2020 2020 2020 2020 2020 206e  ,..            n
+000095b0: 616d 653d 2261 7265 6122 2c0d 0a20 2020  ame="area",..   
+000095c0: 2020 2020 2020 2020 2076 616c 7565 3d22           value="
+000095d0: e58c 97e4 baac 222c 0d0a 2020 2020 2020  ......",..      
+000095e0: 2020 2020 2020 6469 7361 626c 6564 3d54        disabled=T
+000095f0: 7275 650d 0a20 2020 2020 2020 2029 2c0d  rue..        ),.
+00009600: 0a20 2020 2020 2020 2049 6e70 7574 5465  .        InputTe
+00009610: 7874 280d 0a20 2020 2020 2020 2020 2020  xt(..           
+00009620: 206c 6162 656c 3d22 e799 bbe5 bd95 e5af   label="........
+00009630: 86e7 a081 222c 0d0a 2020 2020 2020 2020  ....",..        
+00009640: 2020 2020 7479 7065 3d27 696e 7075 742d      type='input-
+00009650: 7061 7373 776f 7264 272c 0d0a 2020 2020  password',..    
+00009660: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+00009670: 696f 6e3d 22e5 8faf e4b8 8de5 a1ab efbc  ion="...........
+00009680: 8ce9 bb98 e8ae a4e4 b8ba e794 a8e6 88b7  ................
+00009690: 4944 222c 0d0a 2020 2020 2020 2020 2020  ID",..          
+000096a0: 2020 6e61 6d65 3d22 7061 7373 776f 7264    name="password
+000096b0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000096c0: 696e 6c69 6e65 3d46 616c 7365 2c0d 0a20  inline=False,.. 
+000096d0: 2020 2020 2020 2020 2020 2072 6571 7569             requi
+000096e0: 7265 643d 4661 6c73 652c 0d0a 2020 2020  red=False,..    
+000096f0: 2020 2020 2020 2020 7661 6c75 653d 2222          value=""
+00009700: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
+00009710: 6c65 6172 6162 6c65 3d54 7275 652c 0d0a  learable=True,..
+00009720: 2020 2020 2020 2020 2020 2020 6d61 784c              maxL
+00009730: 656e 6774 683d 3136 0d0a 2020 2020 2020  ength=16..      
+00009740: 2020 292c 0d0a 2020 2020 2020 2020 496e    ),..        In
+00009750: 7075 7454 6578 7428 0d0a 2020 2020 2020  putText(..      
+00009760: 2020 2020 2020 6c61 6265 6c3d 22e5 a793        label="...
+00009770: e590 8d22 2c0d 0a20 2020 2020 2020 2020  ...",..         
+00009780: 2020 2064 6573 6372 6970 7469 6f6e 3d22     description="
+00009790: e682 a8e7 9a84 e5a7 93e5 908d 222c 0d0a  ............",..
+000097a0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+000097b0: 3d22 6e61 6d65 222c 0d0a 2020 2020 2020  ="name",..      
+000097c0: 2020 2020 2020 696e 6c69 6e65 3d46 616c        inline=Fal
+000097d0: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
+000097e0: 2072 6571 7569 7265 643d 5472 7565 2c0d   required=True,.
+000097f0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00009800: 7565 3d22 222c 0d0a 2020 2020 2020 2020  ue="",..        
+00009810: 2020 2020 636c 6561 7261 626c 653d 5472      clearable=Tr
+00009820: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
+00009830: 206d 6178 4c65 6e67 7468 3d38 0d0a 2020   maxLength=8..  
+00009840: 2020 2020 2020 292c 2049 6e70 7574 5465        ), InputTe
+00009850: 7874 280d 0a20 2020 2020 2020 2020 2020  xt(..           
+00009860: 206c 6162 656c 3d22 e5a4 a7e5 ada6 e4b9   label="........
+00009870: a049 4422 2c0d 0a20 2020 2020 2020 2020  .ID",..         
+00009880: 2020 2064 6573 6372 6970 7469 6f6e 3d22     description="
+00009890: e590 8de5 ad97 e590 8ee9 9da2 e68b ace5  ................
+000098a0: 8fb7 e586 85e7 9a84 e695 b0e5 ad97 222c  ..............",
+000098b0: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
+000098c0: 6d65 3d22 6478 785f 6964 222c 0d0a 2020  me="dxx_id",..  
+000098d0: 2020 2020 2020 2020 2020 696e 6c69 6e65            inline
+000098e0: 3d46 616c 7365 2c0d 0a20 2020 2020 2020  =False,..       
+000098f0: 2020 2020 2072 6571 7569 7265 643d 5472       required=Tr
+00009900: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
+00009910: 2076 616c 7565 3d22 222c 0d0a 2020 2020   value="",..    
+00009920: 2020 2020 2020 2020 636c 6561 7261 626c          clearabl
+00009930: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
+00009940: 2020 2020 206d 6178 4c65 6e67 7468 3d38       maxLength=8
+00009950: 0d0a 2020 2020 2020 2020 292c 0d0a 2020  ..        ),..  
+00009960: 2020 2020 2020 496e 7075 7454 6578 7428        InputText(
+00009970: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
+00009980: 6265 6c3d 22e5 ada6 e6a0 a122 2c0d 0a20  bel="......",.. 
+00009990: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+000099a0: 6970 7469 6f6e 3d22 e4bd a0e5 b0b1 e8af  iption="........
+000099b0: bbe7 9a84 e9ab 98e6 a0a1 222c 0d0a 2020  ..........",..  
+000099c0: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
+000099d0: 756e 6976 6572 7369 7479 222c 0d0a 2020  university",..  
+000099e0: 2020 2020 2020 2020 2020 696e 6c69 6e65            inline
+000099f0: 3d46 616c 7365 2c0d 0a20 2020 2020 2020  =False,..       
+00009a00: 2020 2020 2072 6571 7569 7265 643d 5472       required=Tr
+00009a10: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
+00009a20: 2076 616c 7565 3d22 222c 0d0a 2020 2020   value="",..    
+00009a30: 2020 2020 2020 2020 636c 6561 7261 626c          clearabl
+00009a40: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
+00009a50: 2020 2020 206d 6178 4c65 6e67 7468 3d32       maxLength=2
+00009a60: 340d 0a20 2020 2020 2020 2029 2c0d 0a20  4..        ),.. 
+00009a70: 2020 2020 2020 2049 6e70 7574 5465 7874         InputText
+00009a80: 280d 0a20 2020 2020 2020 2020 2020 206c  (..            l
+00009a90: 6162 656c 3d22 e5ad a6e9 99a2 222c 0d0a  abel="......",..
+00009aa0: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+00009ab0: 7269 7074 696f 6e3d 22e5 ada6 e999 a2e5  ription=".......
+00009ac0: 908d e7a7 b022 2c0d 0a20 2020 2020 2020  .....",..       
+00009ad0: 2020 2020 206e 616d 653d 2263 6f6c 6c65       name="colle
+00009ae0: 6765 222c 0d0a 2020 2020 2020 2020 2020  ge",..          
+00009af0: 2020 696e 6c69 6e65 3d46 616c 7365 2c0d    inline=False,.
+00009b00: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
+00009b10: 7569 7265 643d 5472 7565 2c0d 0a20 2020  uired=True,..   
+00009b20: 2020 2020 2020 2020 2076 616c 7565 3d22           value="
+00009b30: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00009b40: 636c 6561 7261 626c 653d 5472 7565 2c0d  clearable=True,.
+00009b50: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+00009b60: 4c65 6e67 7468 3d33 320d 0a20 2020 2020  Length=32..     
+00009b70: 2020 2029 2c0d 0a20 2020 2020 2020 2049     ),..        I
+00009b80: 6e70 7574 5465 7874 280d 0a20 2020 2020  nputText(..     
+00009b90: 2020 2020 2020 206c 6162 656c 3d22 e59b         label="..
+00009ba0: a2e6 94af e983 a822 2c0d 0a20 2020 2020  .......",..     
+00009bb0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+00009bc0: 6f6e 3d22 e59b a2e6 94af e983 a87c e78f  on=".........|..
+00009bd0: ade7 baa7 efbc 8ce6 b2a1 e69c 89e5 8faf  ................
+00009be0: e4b8 8de5 a1ab 222c 0d0a 2020 2020 2020  ......",..      
+00009bf0: 2020 2020 2020 6e61 6d65 3d22 6f72 6761        name="orga
+00009c00: 6e69 7a61 7469 6f6e 222c 0d0a 2020 2020  nization",..    
+00009c10: 2020 2020 2020 2020 696e 6c69 6e65 3d46          inline=F
+00009c20: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
+00009c30: 2020 2072 6571 7569 7265 643d 4661 6c73     required=Fals
+00009c40: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00009c50: 7661 6c75 653d 2222 2c0d 0a20 2020 2020  value="",..     
+00009c60: 2020 2020 2020 2063 6c65 6172 6162 6c65         clearable
+00009c70: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+00009c80: 2020 2020 6d61 784c 656e 6774 683d 3332      maxLength=32
+00009c90: 0d0a 2020 2020 2020 2020 292c 0d0a 2020  ..        ),..  
+00009ca0: 2020 2020 2020 496e 7075 7454 6578 7428        InputText(
+00009cb0: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
+00009cc0: 6265 6c3d 22e5 9ba2 e694 afe9 83a8 4944  bel=".........ID
+00009cd0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00009ce0: 6465 7363 7269 7074 696f 6e3d 22e6 94af  description="...
+00009cf0: e983 a8e5 908e e99d a2e6 8bac e58f b7e5  ................
+00009d00: 8685 e79a 84e6 95b0 e5ad 9722 2c0d 0a20  ...........",.. 
+00009d10: 2020 2020 2020 2020 2020 206e 616d 653d             name=
+00009d20: 226f 7267 616e 697a 6174 696f 6e5f 6964  "organization_id
+00009d30: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00009d40: 696e 6c69 6e65 3d46 616c 7365 2c0d 0a20  inline=False,.. 
+00009d50: 2020 2020 2020 2020 2020 2072 6571 7569             requi
+00009d60: 7265 643d 5472 7565 2c0d 0a20 2020 2020  red=True,..     
+00009d70: 2020 2020 2020 2076 616c 7565 3d22 222c         value="",
+00009d80: 0d0a 2020 2020 2020 2020 2020 2020 636c  ..            cl
+00009d90: 6561 7261 626c 653d 5472 7565 2c0d 0a20  earable=True,.. 
+00009da0: 2020 2020 2020 2020 2020 206d 6178 4c65             maxLe
+00009db0: 6e67 7468 3d33 320d 0a20 2020 2020 2020  ngth=32..       
+00009dc0: 2029 2c0d 0a20 2020 2020 2020 2049 6e70   ),..        Inp
+00009dd0: 7574 5465 7874 280d 0a20 2020 2020 2020  utText(..       
+00009de0: 2020 2020 206c 6162 656c 3d22 e8b4 a6e5       label="....
+00009df0: 8fb7 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
+00009e00: 2020 6465 7363 7269 7074 696f 6e3d 22e7    description=".
+00009e10: 99bb e5bd 95e5 8c97 e4ba ace5 85b1 e99d  ................
+00009e20: 92e5 9ba2 e79a 84e8 b4a6 e58f b722 2c0d  .............",.
+00009e30: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+00009e40: 653d 2263 6f6f 6b69 6522 2c0d 0a20 2020  e="cookie",..   
+00009e50: 2020 2020 2020 2020 2069 6e6c 696e 653d           inline=
+00009e60: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
+00009e70: 2020 2020 7265 7175 6972 6564 3d54 7275      required=Tru
+00009e80: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00009e90: 7661 6c75 653d 2222 2c0d 0a20 2020 2020  value="",..     
+00009ea0: 2020 2020 2020 2063 6c65 6172 6162 6c65         clearable
+00009eb0: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+00009ec0: 2020 2020 6d61 784c 656e 6774 683d 3332      maxLength=32
+00009ed0: 0d0a 2020 2020 2020 2020 292c 2049 6e70  ..        ), Inp
+00009ee0: 7574 5465 7874 280d 0a20 2020 2020 2020  utText(..       
+00009ef0: 2020 2020 206c 6162 656c 3d22 e5af 86e7       label="....
+00009f00: a081 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
+00009f10: 2020 6465 7363 7269 7074 696f 6e3d 22e7    description=".
+00009f20: 99bb e999 86e5 8c97 e4ba ace5 85b1 e99d  ................
+00009f30: 92e5 9ba2 e79a 84e5 af86 e7a0 8122 2c0d  .............",.
+00009f40: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+00009f50: 653d 2274 6f6b 656e 222c 0d0a 2020 2020  e="token",..    
+00009f60: 2020 2020 2020 2020 696e 6c69 6e65 3d46          inline=F
+00009f70: 616c 7365 2c0d 0a20 2020 2020 2020 2020  alse,..         
+00009f80: 2020 2072 6571 7569 7265 643d 5472 7565     required=True
+00009f90: 2c0d 0a20 2020 2020 2020 2020 2020 2076  ,..            v
+00009fa0: 616c 7565 3d22 222c 0d0a 2020 2020 2020  alue="",..      
+00009fb0: 2020 2020 2020 636c 6561 7261 626c 653d        clearable=
+00009fc0: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+00009fd0: 2020 206d 6178 4c65 6e67 7468 3d33 320d     maxLength=32.
+00009fe0: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
+00009ff0: 5d0d 0a29 0d0a 2222 22e5 a4a9 e6b4 a5e5  ]..)..""".......
+0000a000: 9cb0 e58c bae6 b7bb e58a a0e7 94a8 e688  ................
+0000a010: b722 2222 0d0a 7469 616e 6a69 6e5f 7461  ."""..tianjin_ta
+0000a020: 626c 6520 3d20 466f 726d 280d 0a20 2020  ble = Form(..   
+0000a030: 2074 6974 6c65 3d22 e6b7 bbe5 8aa0 e6b4   title="........
+0000a040: a5e5 bda9 e99d 92e6 98a5 e794 a8e6 88b7  ................
+0000a050: 222c 0d0a 2020 2020 6d6f 6465 3d44 6973  ",..    mode=Dis
+0000a060: 706c 6179 4d6f 6465 456e 756d 2e68 6f72  playModeEnum.hor
+0000a070: 697a 6f6e 7461 6c2c 0d0a 2020 2020 6170  izontal,..    ap
+0000a080: 693d 2270 6f73 743a 2f54 6565 6e53 7475  i="post:/TeenStu
+0000a090: 6479 2f61 7069 2f74 6961 6e6a 696e 2f61  dy/api/tianjin/a
+0000a0a0: 6464 222c 0d0a 2020 2020 7265 6469 7265  dd",..    redire
+0000a0b0: 6374 3d22 2f54 6565 6e53 7475 6479 2f6c  ct="/TeenStudy/l
+0000a0c0: 6f67 696e 222c 0d0a 2020 2020 626f 6479  ogin",..    body
+0000a0d0: 3d5b 0d0a 2020 2020 2020 2020 5365 6c65  =[..        Sele
+0000a0e0: 6374 280d 0a20 2020 2020 2020 2020 2020  ct(..           
+0000a0f0: 206c 6162 656c 3d22 e7be a4e8 818a 222c   label="......",
+0000a100: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
+0000a110: 6d65 3d22 6772 6f75 705f 6964 222c 0d0a  me="group_id",..
+0000a120: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+0000a130: 7269 7074 696f 6e3d 22e9 9c80 e8a6 81e6  ription=".......
+0000a140: b7bb e58a a0e7 9a84 e7be a4e7 bb84 222c  ..............",
+0000a150: 0d0a 2020 2020 2020 2020 2020 2020 6368  ..            ch
+0000a160: 6563 6b41 6c6c 3d46 616c 7365 2c0d 0a20  eckAll=False,.. 
+0000a170: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
+0000a180: 653d 2267 6574 3a2f 5465 656e 5374 7564  e="get:/TeenStud
+0000a190: 792f 6170 692f 6765 745f 6772 6f75 705f  y/api/get_group_
+0000a1a0: 6c69 7374 222c 0d0a 2020 2020 2020 2020  list",..        
+0000a1b0: 2020 2020 7661 6c75 653d 2727 2c0d 0a20      value='',.. 
+0000a1c0: 2020 2020 2020 2020 2020 206d 756c 7469             multi
+0000a1d0: 706c 653d 4661 6c73 652c 0d0a 2020 2020  ple=False,..    
+0000a1e0: 2020 2020 2020 2020 7265 7175 6972 6564          required
+0000a1f0: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
+0000a200: 2020 2020 7365 6172 6368 6162 6c65 3d54      searchable=T
+0000a210: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+0000a220: 2020 6a6f 696e 5661 6c75 6573 3d46 616c    joinValues=Fal
+0000a230: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
+0000a240: 2065 7874 7261 6374 5661 6c75 653d 5472   extractValue=Tr
+0000a250: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
+0000a260: 2073 7461 7469 7374 6963 733d 5472 7565   statistics=True
+0000a270: 2c0d 0a20 2020 2020 2020 2029 2c0d 0a20  ,..        ),.. 
+0000a280: 2020 2020 2020 2053 656c 6563 7428 0d0a         Select(..
+0000a290: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+0000a2a0: 6c3d 22e7 94a8 e688 b749 4422 2c0d 0a20  l="......ID",.. 
+0000a2b0: 2020 2020 2020 2020 2020 206e 616d 653d             name=
+0000a2c0: 2275 7365 725f 6964 222c 0d0a 2020 2020  "user_id",..    
+0000a2d0: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+0000a2e0: 696f 6e3d 22e9 9c80 e8a6 81e6 b7bb e58a  ion="...........
+0000a2f0: a0e7 9a84 e794 a8e6 88b7 4944 222c 0d0a  ..........ID",..
+0000a300: 2020 2020 2020 2020 2020 2020 6368 6563              chec
+0000a310: 6b41 6c6c 3d46 616c 7365 2c0d 0a20 2020  kAll=False,..   
+0000a320: 2020 2020 2020 2020 2073 6f75 7263 653d           source=
+0000a330: 2267 6574 3a2f 5465 656e 5374 7564 792f  "get:/TeenStudy/
+0000a340: 6170 692f 6765 745f 6d65 6d62 6572 5f6c  api/get_member_l
+0000a350: 6973 743f 6772 6f75 705f 6964 3d24 7b67  ist?group_id=${g
+0000a360: 726f 7570 5f69 647d 222c 0d0a 2020 2020  roup_id}",..    
+0000a370: 2020 2020 2020 2020 7661 6c75 653d 2727          value=''
+0000a380: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
+0000a390: 756c 7469 706c 653d 4661 6c73 652c 0d0a  ultiple=False,..
+0000a3a0: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+0000a3b0: 6972 6564 3d54 7275 652c 0d0a 2020 2020  ired=True,..    
+0000a3c0: 2020 2020 2020 2020 7365 6172 6368 6162          searchab
+0000a3d0: 6c65 3d54 7275 652c 0d0a 2020 2020 2020  le=True,..      
+0000a3e0: 2020 2020 2020 6a6f 696e 5661 6c75 6573        joinValues
+0000a3f0: 3d46 616c 7365 2c0d 0a20 2020 2020 2020  =False,..       
+0000a400: 2020 2020 2065 7874 7261 6374 5661 6c75       extractValu
+0000a410: 653d 5472 7565 2c0d 0a20 2020 2020 2020  e=True,..       
+0000a420: 2020 2020 2073 7461 7469 7374 6963 733d       statistics=
+0000a430: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+0000a440: 2020 2068 6964 6465 6e4f 6e3d 2224 7b67     hiddenOn="${g
+0000a450: 726f 7570 5f69 643d 3d27 273f 7472 7565  roup_id==''?true
+0000a460: 3a66 616c 7365 7d22 0d0a 2020 2020 2020  :false}"..      
+0000a470: 2020 292c 0d0a 2020 2020 2020 2020 496e    ),..        In
+0000a480: 7075 7454 6578 7428 0d0a 2020 2020 2020  putText(..      
+0000a490: 2020 2020 2020 6c61 6265 6c3d 22e5 9cb0        label="...
+0000a4a0: e58c ba22 2c0d 0a20 2020 2020 2020 2020  ...",..         
+0000a4b0: 2020 2064 6573 6372 6970 7469 6f6e 3d22     description="
+0000a4c0: e689 80e5 a484 e79c 81e4 bbbd 222c 0d0a  ............",..
+0000a4d0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+0000a4e0: 3d22 6172 6561 222c 0d0a 2020 2020 2020  ="area",..      
+0000a4f0: 2020 2020 2020 7661 6c75 653d 22e5 a4a9        value="...
+0000a500: e6b4 a522 2c0d 0a20 2020 2020 2020 2020  ...",..         
+0000a510: 2020 2064 6973 6162 6c65 643d 5472 7565     disabled=True
+0000a520: 0d0a 2020 2020 2020 2020 292c 0d0a 2020  ..        ),..  
+0000a530: 2020 2020 2020 496e 7075 7454 6578 7428        InputText(
+0000a540: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
+0000a550: 6265 6c3d 22e7 99bb e5bd 95e5 af86 e7a0  bel="...........
+0000a560: 8122 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
+0000a570: 2074 7970 653d 2769 6e70 7574 2d70 6173   type='input-pas
+0000a580: 7377 6f72 6427 2c0d 0a20 2020 2020 2020  sword',..       
+0000a590: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+0000a5a0: 3d22 e58f afe4 b88d e5a1 abef bc8c e9bb  ="..............
+0000a5b0: 98e8 aea4 e4b8 bae7 94a8 e688 b749 4422  .............ID"
+0000a5c0: 2c0d 0a20 2020 2020 2020 2020 2020 206e  ,..            n
+0000a5d0: 616d 653d 2270 6173 7377 6f72 6422 2c0d  ame="password",.
+0000a5e0: 0a20 2020 2020 2020 2020 2020 2069 6e6c  .            inl
+0000a5f0: 696e 653d 4661 6c73 652c 0d0a 2020 2020  ine=False,..    
+0000a600: 2020 2020 2020 2020 7265 7175 6972 6564          required
+0000a610: 3d46 616c 7365 2c0d 0a20 2020 2020 2020  =False,..       
+0000a620: 2020 2020 2076 616c 7565 3d22 222c 0d0a       value="",..
+0000a630: 2020 2020 2020 2020 2020 2020 636c 6561              clea
+0000a640: 7261 626c 653d 5472 7565 2c0d 0a20 2020  rable=True,..   
+0000a650: 2020 2020 2020 2020 206d 6178 4c65 6e67           maxLeng
+0000a660: 7468 3d31 360d 0a20 2020 2020 2020 2029  th=16..        )
+0000a670: 2c0d 0a20 2020 2020 2020 2049 6e70 7574  ,..        Input
+0000a680: 5465 7874 280d 0a20 2020 2020 2020 2020  Text(..         
+0000a690: 2020 206c 6162 656c 3d22 e5a7 93e5 908d     label="......
+0000a6a0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0000a6b0: 6465 7363 7269 7074 696f 6e3d 22e6 82a8  description="...
+0000a6c0: e79a 84e5 a793 e590 8d22 2c0d 0a20 2020  .........",..   
+0000a6d0: 2020 2020 2020 2020 206e 616d 653d 226e           name="n
+0000a6e0: 616d 6522 2c0d 0a20 2020 2020 2020 2020  ame",..         
+0000a6f0: 2020 2069 6e6c 696e 653d 4661 6c73 652c     inline=False,
+0000a700: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0000a710: 7175 6972 6564 3d54 7275 652c 0d0a 2020  quired=True,..  
+0000a720: 2020 2020 2020 2020 2020 7661 6c75 653d            value=
+0000a730: 2222 2c0d 0a20 2020 2020 2020 2020 2020  "",..           
+0000a740: 2063 6c65 6172 6162 6c65 3d54 7275 652c   clearable=True,
+0000a750: 0d0a 2020 2020 2020 2020 2020 2020 6d61  ..            ma
+0000a760: 784c 656e 6774 683d 380d 0a20 2020 2020  xLength=8..     
+0000a770: 2020 2029 2c0d 0a20 2020 2020 2020 2049     ),..        I
+0000a780: 6e70 7574 5465 7874 280d 0a20 2020 2020  nputText(..     
+0000a790: 2020 2020 2020 206c 6162 656c 3d22 e5ad         label="..
+0000a7a0: a6e6 a0a1 222c 0d0a 2020 2020 2020 2020  ....",..        
+0000a7b0: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
+0000a7c0: 22e4 bda0 e5b0 b1e8 afbb e79a 84e9 ab98  "...............
+0000a7d0: e6a0 a122 2c0d 0a20 2020 2020 2020 2020  ...",..         
+0000a7e0: 2020 206e 616d 653d 2275 6e69 7665 7273     name="univers
+0000a7f0: 6974 7922 2c0d 0a20 2020 2020 2020 2020  ity",..         
+0000a800: 2020 2069 6e6c 696e 653d 4661 6c73 652c     inline=False,
+0000a810: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0000a820: 7175 6972 6564 3d54 7275 652c 0d0a 2020  quired=True,..  
+0000a830: 2020 2020 2020 2020 2020 7661 6c75 653d            value=
+0000a840: 2222 2c0d 0a20 2020 2020 2020 2020 2020  "",..           
+0000a850: 2063 6c65 6172 6162 6c65 3d54 7275 652c   clearable=True,
+0000a860: 0d0a 2020 2020 2020 2020 2020 2020 6d61  ..            ma
+0000a870: 784c 656e 6774 683d 3234 0d0a 2020 2020  xLength=24..    
+0000a880: 2020 2020 292c 0d0a 2020 2020 2020 2020      ),..        
+0000a890: 496e 7075 7454 6578 7428 0d0a 2020 2020  InputText(..    
+0000a8a0: 2020 2020 2020 2020 6c61 6265 6c3d 22e5          label=".
+0000a8b0: ada6 e999 a222 2c0d 0a20 2020 2020 2020  .....",..       
+0000a8c0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+0000a8d0: 3d22 e5ad a6e9 99a2 e590 8de7 a7b0 222c  ="............",
+0000a8e0: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
+0000a8f0: 6d65 3d22 636f 6c6c 6567 6522 2c0d 0a20  me="college",.. 
+0000a900: 2020 2020 2020 2020 2020 2069 6e6c 696e             inlin
+0000a910: 653d 4661 6c73 652c 0d0a 2020 2020 2020  e=False,..      
+0000a920: 2020 2020 2020 7265 7175 6972 6564 3d54        required=T
+0000a930: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+0000a940: 2020 7661 6c75 653d 2222 2c0d 0a20 2020    value="",..   
+0000a950: 2020 2020 2020 2020 2063 6c65 6172 6162           clearab
+0000a960: 6c65 3d54 7275 652c 0d0a 2020 2020 2020  le=True,..      
+0000a970: 2020 2020 2020 6d61 784c 656e 6774 683d        maxLength=
+0000a980: 3332 0d0a 2020 2020 2020 2020 292c 0d0a  32..        ),..
+0000a990: 2020 2020 2020 2020 496e 7075 7454 6578          InputTex
+0000a9a0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+0000a9b0: 6c61 6265 6c3d 22e5 9ba2 e694 afe9 83a8  label=".........
+0000a9c0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0000a9d0: 6465 7363 7269 7074 696f 6e3d 22e5 9ba2  description="...
+0000a9e0: e694 afe9 83a8 7ce7 8fad e7ba a7ef bc8c  ......|.........
+0000a9f0: e6b2 a1e6 9c89 e58f afe4 b88d e5a1 ab22  ..............."
+0000aa00: 2c0d 0a20 2020 2020 2020 2020 2020 206e  ,..            n
+0000aa10: 616d 653d 226f 7267 616e 697a 6174 696f  ame="organizatio
+0000aa20: 6e22 2c0d 0a20 2020 2020 2020 2020 2020  n",..           
+0000aa30: 2069 6e6c 696e 653d 4661 6c73 652c 0d0a   inline=False,..
+0000aa40: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+0000aa50: 6972 6564 3d46 616c 7365 2c0d 0a20 2020  ired=False,..   
+0000aa60: 2020 2020 2020 2020 2076 616c 7565 3d22           value="
+0000aa70: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0000aa80: 636c 6561 7261 626c 653d 5472 7565 2c0d  clearable=True,.
+0000aa90: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+0000aaa0: 4c65 6e67 7468 3d33 320d 0a20 2020 2020  Length=32..     
+0000aab0: 2020 2029 2c0d 0a20 2020 2020 2020 2049     ),..        I
+0000aac0: 6e70 7574 5465 7874 280d 0a20 2020 2020  nputText(..     
+0000aad0: 2020 2020 2020 206c 6162 656c 3d22 636f         label="co
+0000aae0: 6f6b 6965 222c 0d0a 2020 2020 2020 2020  okie",..        
+0000aaf0: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
+0000ab00: 22e8 87aa e8a1 8ce6 8a93 e58c 85e8 8eb7  "...............
+0000ab10: e58f 96ef bc8c e7bb 93e6 9e84 e4b8 baef  ................
+0000ab20: bc9a 4a53 4553 5349 4f4e 4944 3d31 3837  ..JSESSIONID=187
+0000ab30: 3346 5858 5858 5858 5858 3544 4643 4246  3FXXXXXXXX5DFCBF
+0000ab40: 3143 4331 3337 3033 222c 0d0a 2020 2020  1CC13703",..    
+0000ab50: 2020 2020 2020 2020 6e61 6d65 3d22 636f          name="co
+0000ab60: 6f6b 6965 222c 0d0a 2020 2020 2020 2020  okie",..        
+0000ab70: 2020 2020 696e 6c69 6e65 3d46 616c 7365      inline=False
+0000ab80: 2c0d 0a20 2020 2020 2020 2020 2020 2072  ,..            r
+0000ab90: 6571 7569 7265 643d 5472 7565 2c0d 0a20  equired=True,.. 
+0000aba0: 2020 2020 2020 2020 2020 2076 616c 7565             value
+0000abb0: 3d22 222c 0d0a 2020 2020 2020 2020 2020  ="",..          
+0000abc0: 2020 636c 6561 7261 626c 653d 5472 7565    clearable=True
+0000abd0: 2c0d 0a20 2020 2020 2020 2029 2c0d 0a20  ,..        ),.. 
+0000abe0: 2020 205d 0d0a 290d 0a68 7562 6569 5f70     ]..)..hubei_p
+0000abf0: 6167 6520 3d20 5061 6765 5363 6865 6d61  age = PageSchema
+0000ac00: 2875 726c 3d27 2f54 6565 6e53 7475 6479  (url='/TeenStudy
+0000ac10: 2f61 6464 2f68 7562 6569 272c 2069 636f  /add/hubei', ico
+0000ac20: 6e3d 2766 6120 6661 2d70 656e 2d74 6f2d  n='fa fa-pen-to-
+0000ac30: 7371 7561 7265 272c 206c 6162 656c 3d27  square', label='
+0000ac40: e99d 92e6 98a5 e6b9 96e5 8c97 272c 0d0a  ............',..
+0000ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac60: 2020 2020 2020 2020 7363 6865 6d61 3d50          schema=P
+0000ac70: 6167 6528 7469 746c 653d 27e9 9d92 e698  age(title='.....
+0000ac80: a5e6 b996 e58c 9727 2c20 626f 6479 3d5b  .......', body=[
+0000ac90: 6875 6265 695f 7461 626c 655d 2929 0d0a  hubei_table]))..
+0000aca0: 6a69 616e 6778 695f 7061 6765 203d 2050  jiangxi_page = P
+0000acb0: 6167 6553 6368 656d 6128 7572 6c3d 272f  ageSchema(url='/
+0000acc0: 5465 656e 5374 7564 792f 6164 642f 6a69  TeenStudy/add/ji
+0000acd0: 616e 6778 6927 2c20 6963 6f6e 3d27 6661  angxi', icon='fa
+0000ace0: 2066 612d 7065 6e2d 746f 2d73 7175 6172   fa-pen-to-squar
+0000acf0: 6527 2c20 6c61 6265 6c3d 27e6 b19f e8a5  e', label='.....
+0000ad00: bfe5 85b1 e99d 92e5 9ba2 272c 0d0a 2020  ..........',..  
+0000ad10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad20: 2020 2020 2020 2020 7363 6865 6d61 3d50          schema=P
+0000ad30: 6167 6528 7469 746c 653d 27e6 b19f e8a5  age(title='.....
+0000ad40: bfe5 85b1 e99d 92e5 9ba2 272c 2062 6f64  ..........', bod
+0000ad50: 793d 5b6a 6961 6e67 7869 5f74 6162 6c65  y=[jiangxi_table
+0000ad60: 5d29 290d 0a61 6e68 7569 5f70 6167 6520  ]))..anhui_page 
+0000ad70: 3d20 5061 6765 5363 6865 6d61 2875 726c  = PageSchema(url
+0000ad80: 3d27 2f54 6565 6e53 7475 6479 2f61 6464  ='/TeenStudy/add
+0000ad90: 2f61 6e68 7569 272c 2069 636f 6e3d 2766  /anhui', icon='f
+0000ada0: 6120 6661 2d70 656e 2d74 6f2d 7371 7561  a fa-pen-to-squa
+0000adb0: 7265 272c 206c 6162 656c 3d27 e5ae 89e5  re', label='....
+0000adc0: bebd e585 b1e9 9d92 e59b a227 2c0d 0a20  ...........',.. 
+0000add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ade0: 2020 2020 2020 2073 6368 656d 613d 5061         schema=Pa
+0000adf0: 6765 2874 6974 6c65 3d27 e5ae 89e5 bebd  ge(title='......
+0000ae00: e585 b1e9 9d92 e59b a227 2c20 626f 6479  .........', body
+0000ae10: 3d5b 616e 6875 695f 7461 626c 655d 2929  =[anhui_table]))
+0000ae20: 0d0a 7369 6368 7561 6e5f 7061 6765 203d  ..sichuan_page =
+0000ae30: 2050 6167 6553 6368 656d 6128 7572 6c3d   PageSchema(url=
+0000ae40: 272f 5465 656e 5374 7564 792f 6164 642f  '/TeenStudy/add/
+0000ae50: 7369 6368 7561 6e27 2c20 6963 6f6e 3d27  sichuan', icon='
+0000ae60: 6661 2066 612d 7065 6e2d 746f 2d73 7175  fa fa-pen-to-squ
+0000ae70: 6172 6527 2c20 6c61 6265 6c3d 27e5 a4a9  are', label='...
+0000ae80: e5ba 9ce6 96b0 e99d 92e5 b9b4 272c 0d0a  ............',..
+0000ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aea0: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
+0000aeb0: 3d50 6167 6528 7469 746c 653d 27e5 a4a9  =Page(title='...
+0000aec0: e5ba 9ce6 96b0 e99d 92e5 b9b4 272c 2062  ............', b
+0000aed0: 6f64 793d 5b73 6963 6875 616e 5f74 6162  ody=[sichuan_tab
+0000aee0: 6c65 5d29 290d 0a73 6861 6e64 6f6e 675f  le]))..shandong_
+0000aef0: 7061 6765 203d 2050 6167 6553 6368 656d  page = PageSchem
+0000af00: 6128 7572 6c3d 272f 5465 656e 5374 7564  a(url='/TeenStud
+0000af10: 792f 6164 642f 7368 616e 646f 6e67 272c  y/add/shandong',
+0000af20: 2069 636f 6e3d 2766 6120 6661 2d70 656e   icon='fa fa-pen
+0000af30: 2d74 6f2d 7371 7561 7265 272c 206c 6162  -to-square', lab
+0000af40: 656c 3d27 e99d 92e6 98a5 e5b1 b1e4 b89c  el='............
+0000af50: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+0000af60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000af70: 6368 656d 613d 5061 6765 2874 6974 6c65  chema=Page(title
+0000af80: 3d27 e99d 92e6 98a5 e5b1 b1e4 b89c 272c  ='............',
+0000af90: 2062 6f64 793d 5b73 6861 6e64 6f6e 675f   body=[shandong_
+0000afa0: 7461 626c 655d 2929 0d0a 6368 6f6e 6771  table]))..chongq
+0000afb0: 696e 675f 7061 6765 203d 2050 6167 6553  ing_page = PageS
+0000afc0: 6368 656d 6128 7572 6c3d 272f 5465 656e  chema(url='/Teen
+0000afd0: 5374 7564 792f 6164 642f 6368 6f6e 6771  Study/add/chongq
+0000afe0: 696e 6727 2c20 6963 6f6e 3d27 6661 2066  ing', icon='fa f
+0000aff0: 612d 7065 6e2d 746f 2d73 7175 6172 6527  a-pen-to-square'
+0000b000: 2c20 6c61 6265 6c3d 27e9 878d e5ba 86e5  , label='.......
+0000b010: 85b1 e99d 92e5 9ba2 272c 0d0a 2020 2020  ........',..    
+0000b020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b030: 2020 2020 2020 2020 7363 6865 6d61 3d50          schema=P
+0000b040: 6167 6528 7469 746c 653d 27e9 878d e5ba  age(title='.....
+0000b050: 86e5 85b1 e99d 92e5 9ba2 272c 2062 6f64  ..........', bod
+0000b060: 793d 5b63 686f 6e67 7169 6e67 5f74 6162  y=[chongqing_tab
+0000b070: 6c65 5d29 290d 0a6a 696c 696e 5f70 6167  le]))..jilin_pag
+0000b080: 6520 3d20 5061 6765 5363 6865 6d61 2875  e = PageSchema(u
+0000b090: 726c 3d27 2f54 6565 6e53 7475 6479 2f61  rl='/TeenStudy/a
+0000b0a0: 6464 2f6a 696c 696e 272c 2069 636f 6e3d  dd/jilin', icon=
+0000b0b0: 2766 6120 6661 2d70 656e 2d74 6f2d 7371  'fa fa-pen-to-sq
+0000b0c0: 7561 7265 272c 206c 6162 656c 3d27 e590  uare', label='..
+0000b0d0: 89e9 9d92 e9a3 9ee6 89ac 272c 0d0a 2020  ..........',..  
+0000b0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0f0: 2020 2020 2020 7363 6865 6d61 3d50 6167        schema=Pag
+0000b100: 6528 7469 746c 653d 27e5 9089 e99d 92e9  e(title='.......
+0000b110: a39e e689 ac27 2c20 626f 6479 3d5b 6a69  .....', body=[ji
+0000b120: 6c69 6e5f 7461 626c 655d 2929 0d0a 6775  lin_table]))..gu
+0000b130: 616e 6764 6f6e 675f 7061 6765 203d 2050  angdong_page = P
+0000b140: 6167 6553 6368 656d 6128 7572 6c3d 272f  ageSchema(url='/
+0000b150: 5465 656e 5374 7564 792f 6164 642f 6775  TeenStudy/add/gu
+0000b160: 616e 6764 6f6e 6727 2c20 6963 6f6e 3d27  angdong', icon='
+0000b170: 6661 2066 612d 7065 6e2d 746f 2d73 7175  fa fa-pen-to-squ
+0000b180: 6172 6527 2c20 6c61 6265 6c3d 27e5 b9bf  are', label='...
+0000b190: e4b8 9ce5 85b1 e99d 92e5 9ba2 272c 0d0a  ............',..
+0000b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1b0: 2020 2020 2020 2020 2020 2020 7363 6865              sche
+0000b1c0: 6d61 3d50 6167 6528 7469 746c 653d 27e5  ma=Page(title='.
+0000b1d0: b9bf e4b8 9ce5 85b1 e99d 92e5 9ba2 272c  ..............',
+0000b1e0: 2062 6f64 793d 5b67 7561 6e67 646f 6e67   body=[guangdong
+0000b1f0: 5f74 6162 6c65 5d29 290d 0a62 6569 6a69  _table]))..beiji
+0000b200: 6e67 5f70 6167 6520 3d20 5061 6765 5363  ng_page = PageSc
+0000b210: 6865 6d61 2875 726c 3d27 2f54 6565 6e53  hema(url='/TeenS
+0000b220: 7475 6479 2f61 6464 2f62 6569 6a69 6e67  tudy/add/beijing
+0000b230: 272c 2069 636f 6e3d 2766 6120 6661 2d70  ', icon='fa fa-p
+0000b240: 656e 2d74 6f2d 7371 7561 7265 272c 206c  en-to-square', l
+0000b250: 6162 656c 3d27 e58c 97e4 baac e585 b1e9  abel='..........
+0000b260: 9d92 e59b a227 2c0d 0a20 2020 2020 2020  .....',..       
+0000b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b280: 2020 2073 6368 656d 613d 5061 6765 2874     schema=Page(t
+0000b290: 6974 6c65 3d27 e58c 97e4 baac e585 b1e9  itle='..........
+0000b2a0: 9d92 e59b a227 2c20 626f 6479 3d5b 6265  .....', body=[be
+0000b2b0: 696a 696e 675f 7461 626c 655d 2929 0d0a  ijing_table]))..
+0000b2c0: 7469 616e 6a69 6e5f 7061 6765 203d 2050  tianjin_page = P
+0000b2d0: 6167 6553 6368 656d 6128 7572 6c3d 272f  ageSchema(url='/
+0000b2e0: 5465 656e 5374 7564 792f 6164 642f 7469  TeenStudy/add/ti
+0000b2f0: 616e 6a69 6e27 2c20 6963 6f6e 3d27 6661  anjin', icon='fa
+0000b300: 2066 612d 7065 6e2d 746f 2d73 7175 6172   fa-pen-to-squar
+0000b310: 6527 2c20 6c61 6265 6c3d 27e6 b4a5 e5bd  e', label='.....
+0000b320: a9e9 9d92 e698 a527 2c0d 0a20 2020 2020  .......',..     
+0000b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b340: 2020 2020 2073 6368 656d 613d 5061 6765       schema=Page
+0000b350: 2874 6974 6c65 3d27 e6b4 a5e5 bda9 e99d  (title='........
+0000b360: 92e6 98a5 272c 2062 6f64 793d 5b74 6961  ....', body=[tia
+0000b370: 6e6a 696e 5f74 6162 6c65 5d29 290d 0a61  njin_table]))..a
+0000b380: 7265 6150 6167 6520 3d20 5b6c 6973 745f  reaPage = [list_
+0000b390: 7061 6765 2c0d 0a20 2020 2020 2020 2020  page,..         
+0000b3a0: 2020 2068 7562 6569 5f70 6167 652c 206a     hubei_page, j
+0000b3b0: 6961 6e67 7869 5f70 6167 652c 2061 6e68  iangxi_page, anh
+0000b3c0: 7569 5f70 6167 652c 0d0a 2020 2020 2020  ui_page,..      
+0000b3d0: 2020 2020 2020 7369 6368 7561 6e5f 7061        sichuan_pa
+0000b3e0: 6765 2c20 7368 616e 646f 6e67 5f70 6167  ge, shandong_pag
+0000b3f0: 652c 2063 686f 6e67 7169 6e67 5f70 6167  e, chongqing_pag
+0000b400: 652c 206a 696c 696e 5f70 6167 652c 2067  e, jilin_page, g
+0000b410: 7561 6e67 646f 6e67 5f70 6167 652c 2062  uangdong_page, b
+0000b420: 6569 6a69 6e67 5f70 6167 652c 0d0a 2020  eijing_page,..  
+0000b430: 2020 2020 2020 2020 2020 7469 616e 6a69            tianji
+0000b440: 6e5f 7061 6765 0d0a 2020 2020 2020 2020  n_page..        
+0000b450: 2020 2020 5d0d 0a                            ]..
```

### Comparing `TeenStudy-0.1.9/TeenStudy/web/pages/home.py` & `TeenStudy-0.2.0/TeenStudy/web/pages/home.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,50 @@
 from amis import App, PageSchema, Flex, ActionType, LevelEnum, Dialog, Form, DisplayModeEnum, InputText, TableColumn, \
     CRUD, Tpl, Switch
 from amis import Html, Page, Property, Service, Divider
 
 logo = Html(html=f'''
 <p align="center">
     <a href="https://github.com/ZM25XC/TeenStudy/">
-        <img src="https://i.328888.xyz/2023/02/23/xIh5k.png"
+        <img src="https://i.imgloc.com/2023/05/20/VyRjTV.png"
          width="256" height="256" alt="TeenStudy">
     </a>
 </p>
 <h2 align="center">大学习自动提交</h2>
 <div align="center">
     <a href="https://github.com/ZM25XC/TeenStudy/" target="_blank">
     Github仓库</a>
     <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS" target="_blank">交流群</a>
+    <a href="http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm" target="_blank">QQ体验群</a>
 </div>
 <br>
 ''')
 github_logo = Tpl(className='w-full',
                   tpl='<div class="flex justify-between"><div></div><div><a href="https://github.com/ZM25XC/TeenStudy" target="_blank" title="Github 仓库"><i class="fa fa-github fa-2x"></i></a></div></div>')
-header = Flex(className='w-full', justify='flex-end', alignItems='flex-end', items=[github_logo])
+header = Flex(className='w-full', justify='flex-end', alignItems='flex-end', items=[github_logo, {
+    "type": "button",
+    "label": "退出",
+    "onEvent": {
+        "click": {
+            "actions": [
+                {
+                    "actionType": "confirmDialog",
+                    "args": {
+                        "title": "操作确认",
+                        "msg": "是否退出系统？"
+                    }},
+
+                {
+                    "actionType": "custom",
+                    "script": "window.location.href = '/TeenStudy/login';window.localStorage.clear();window.sessionStorage.clear();\n //event.stopPropagation();"
+                }
+
+            ]
+        },
+    }}])
 operation_button = Flex(justify='center', items=[
     ActionType.Dialog(
         label='修改信息',
         className='m-l',
         level=LevelEnum.primary,
         dialog=Dialog(title='修改信息',
                       size='lg',
@@ -133,15 +154,21 @@
                    }
                }
            })
 ])
 
 from_table = Service(
     title="",
-    api="/TeenStudy/api/get_user?user_id=${user_id}",
+    api={
+        "method": "get",
+        "url": "/TeenStudy/api/get_user",
+        "headers": {
+            "token": """${window.localStorage.getItem("token")}""",
+        }
+    },
     interval=12000,
     body=[
         Property(
             title='用户详细信息',
             column=2,
             items=[
                 Property.Item(
@@ -287,21 +314,21 @@
                                              'body': {'type': 'tpl',
                                                       'tpl': '${answer}'}}),
                         TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}',
                                     label='更新时间',
                                     name='time', sortable=True)
                     ])
 page_detail = Page(title='', body=[logo, operation_button, Divider(), from_table])
-home_page = PageSchema(url='/home', label='首页', icon='fa fa-home', isDefaultPage=True, schema=page_detail)
+home_page = PageSchema(url='/TeenStudy/home', label='首页', icon='fa fa-home', isDefaultPage=True, schema=page_detail)
 home_app = App(brandName='TeenStudy',
-               logo='https://i.328888.xyz/2023/02/23/xIh5k.png',
+               logo='https://img1.imgtp.com/2023/06/11/sG4KdlpL.png',
                header=header,
                pages=[{
                    'children': [
                        home_page,
-                       PageSchema(url="answer", label='大学习列表', icon='fa fa-book-open',
+                       PageSchema(url="/TeenStudy/answer", label='大学习列表', icon='fa fa-book-open',
                                   schema=Page(title='', body=[answer_table])),
-                       PageSchema(url="/records", label='提交记录', icon='fa fa-code-commit',
+                       PageSchema(url="/TeenStudy/records", label='提交记录', icon='fa fa-code-commit',
                                   schema=Page(title='', body=[record_table]))
                    ]}],
                footer=Html(
-                   html=f'<div class="p-2 text-center bg-blue-100">Copyright © 2022 - 2023 <a href="https://github.com/ZM25XC/TeenStudy" target="_blank" class="link-secondary">TeenStudy</a> X<a target="_blank" href="https://github.com/baidu/amis" class="link-secondary" rel="noopener"> amis v2.2.0</a></div>'))
+                   html=f'<div class="p-2 text-center bg-blue-100">Copyright © 2022 - 2023 <a href="https://github.com/ZM25XC/TeenStudy" target="_blank" class="link-secondary">TeenStudy v0.2.0</a> X<a target="_blank" href="https://github.com/baidu/amis" class="link-secondary" rel="noopener"> amis v3.1.1</a></div>'))
```

#### html2text {}

```diff
@@ -1,26 +1,31 @@
 from amis import App, PageSchema, Flex, ActionType, LevelEnum, Dialog, Form,
 DisplayModeEnum, InputText, TableColumn, \ CRUD, Tpl, Switch from amis import
 Html, Page, Property, Service, Divider logo = Html(html=f'''
                                   [TeenStudy]
                        ***** å¤§å­¦ä¹ èªå¨æäº¤ *****
-                            Githubä»åº äº¤æµç¾¤
+                      Githubä»åº äº¤æµç¾¤ QQä½éªç¾¤
 
 ''') github_logo = Tpl(className='w-full', tpl='
 ') header = Flex(className='w-full', justify='flex-end', alignItems='flex-end',
-items=[github_logo]) operation_button = Flex(justify='center', items=
-[ ActionType.Dialog( label='ä¿®æ¹ä¿¡æ¯', className='m-l',
-level=LevelEnum.primary, dialog=Dialog(title='ä¿®æ¹ä¿¡æ¯', size='lg', body=
-[ Form( title='', api='put:/TeenStudy/api/change?user_id=${user_id}',
-submitText='ä¿å­ä¿®æ¹', mode=DisplayModeEnum.horizontal, labelAlign='right',
-body=[ InputText(label='æ§å«', name='gender', value='${gender}',
-required=True, trimContents=True, clearable=True, showCounter=True,
-maxLength=3, visibleOn="${gender==null?false:true}", description='æ§å«'),
-InputText(label='uid|nid', name='dxx_id', value='${dxx_id}', required=True,
-trimContents=True, clearable=True, showCounter=True, maxLength=24, visibleOn="$
+items=[github_logo, { "type": "button", "label": "éåº", "onEvent":
+{ "click": { "actions": [ { "actionType": "confirmDialog", "args": { "title":
+"æä½ç¡®è®¤", "msg": "æ¯å¦éåºç³»ç»ï¼" }}, { "actionType": "custom",
+"script": "window.location.href = '/TeenStudy/login';window.localStorage.clear
+();window.sessionStorage.clear();\n //event.stopPropagation();" } ] }, }}])
+operation_button = Flex(justify='center', items=[ ActionType.Dialog
+( label='ä¿®æ¹ä¿¡æ¯', className='m-l', level=LevelEnum.primary, dialog=Dialog
+(title='ä¿®æ¹ä¿¡æ¯', size='lg', body=[ Form( title='', api='put:/TeenStudy/
+api/change?user_id=${user_id}', submitText='ä¿å­ä¿®æ¹',
+mode=DisplayModeEnum.horizontal, labelAlign='right', body=[ InputText
+(label='æ§å«', name='gender', value='${gender}', required=True,
+trimContents=True, clearable=True, showCounter=True, maxLength=3, visibleOn="$
+{gender==null?false:true}", description='æ§å«'), InputText(label='uid|nid',
+name='dxx_id', value='${dxx_id}', required=True, trimContents=True,
+clearable=True, showCounter=True, maxLength=24, visibleOn="$
 {dxx_id==null?false:true}",
 description='å¤§å­¦ä¹ è®¤è¯IDï¼ä¸æ¸æ¥è¯·å¿æ¹å¨'), InputText
 (label='ææºå·', name='mobile', value='${mobile}', required=True,
 trimContents=True, clearable=True, showCounter=True, maxLength=24, visibleOn="$
 {mobile==null?false:true}", description='ææºå·'), InputText
 (label='å¢æ¯ä¹¦ID', name='leader', value='${leader}', showCounter=True,
 maxLength=10, hiddenOn=True, trimContents=True, clearable=True,
@@ -68,16 +73,17 @@
 api/commit?user_id=${user_id}&area=${area}' ), Switch(name='auto_submit',
 value='${auto_submit}', tooltip='èªå¨æäº¤å¤§å­¦ä¹ å¼å³',
 onText='èªå¨æäº¤å¤§å­¦ä¹ å¼', offText='èªå¨æäº¤å¤§å­¦ä¹ å³', onEvent=
 { 'change': { 'actions': { 'actionType': 'ajax', 'args': { 'api': { 'url': '/
 TeenStudy/api/set_auto_submit', 'method': 'put' }, 'messages': { 'success':
 'èªå¨æäº¤å·²è®¾ç½®ä¸º${event.data.value==true?"å¼å¯":"å³é­"}',
 'failed': 'ä¿®æ¹å¤±è´¥ï¼' }, 'status': '${event.data.value}', 'id': '${id}' }
-} } }) ]) from_table = Service( title="", api="/TeenStudy/api/
-get_user?user_id=${user_id}", interval=12000, body=[ Property
+} } }) ]) from_table = Service( title="", api={ "method": "get", "url": "/
+TeenStudy/api/get_user", "headers": { "token": """${window.localStorage.getItem
+("token")}""", } }, interval=12000, body=[ Property
 ( title='ç¨æ·è¯¦ç»ä¿¡æ¯', column=2, items=[ Property.Item
 ( label='ç¨æ·ID', content='${user_id}' ), Property.Item( label='å§å',
 content='${name}' ), Property.Item( label='å°åº', content='${area}' ),
 Property.Item( label='å­¦æ ¡', content='${university}' ), Property.Item
 ( label='å­¦é¢', content='${college}' ), Property.Item( label='å¢æ¯é¨',
 content='${organization}' ), Property.Item( label='ææ°æäº¤ææ°',
 content='${catalogue}' ), Property.Item( label='ææ°æäº¤æ¶é´', content='$
@@ -121,16 +127,17 @@
 'å®æ´ç½å', 'className': 'break-all', 'body': {'type': 'tpl', 'tpl': '$
 {end_url}'}}, copyable=True), TableColumn(type='tpl', tpl='${answer|truncate:
 20}', label='ç­æ¡', name='answer', popOver={'mode': 'dialog', 'title':
 'å®æ´ç­æ¡', 'className': 'break-all', 'body': {'type': 'tpl', 'tpl': '$
 {answer}'}}), TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:
 ss}', label='æ´æ°æ¶é´', name='time', sortable=True) ]) page_detail = Page
 (title='', body=[logo, operation_button, Divider(), from_table]) home_page =
-PageSchema(url='/home', label='é¦é¡µ', icon='fa fa-home', isDefaultPage=True,
-schema=page_detail) home_app = App(brandName='TeenStudy', logo='https://
-i.328888.xyz/2023/02/23/xIh5k.png', header=header, pages=[{ 'children':
-[ home_page, PageSchema(url="answer", label='å¤§å­¦ä¹ åè¡¨', icon='fa fa-
-book-open', schema=Page(title='', body=[answer_table])), PageSchema(url="/
-records", label='æäº¤è®°å½', icon='fa fa-code-commit', schema=Page(title='',
-body=[record_table])) ]}], footer=Html( html=f'
-Copyright Â© 2022 - 2023 TeenStudy Xamis_v2.2.0
+PageSchema(url='/TeenStudy/home', label='é¦é¡µ', icon='fa fa-home',
+isDefaultPage=True, schema=page_detail) home_app = App(brandName='TeenStudy',
+logo='https://img1.imgtp.com/2023/06/11/sG4KdlpL.png', header=header, pages=[
+{ 'children': [ home_page, PageSchema(url="/TeenStudy/answer",
+label='å¤§å­¦ä¹ åè¡¨', icon='fa fa-book-open', schema=Page(title='', body=
+[answer_table])), PageSchema(url="/TeenStudy/records", label='æäº¤è®°å½',
+icon='fa fa-code-commit', schema=Page(title='', body=[record_table])) ]}],
+footer=Html( html=f'
+Copyright Â© 2022 - 2023 TeenStudy_v0.2.0 Xamis_v3.1.1
 '))
```

### Comparing `TeenStudy-0.1.9/TeenStudy/web/pages/login.py` & `TeenStudy-0.2.0/TeenStudy/web/pages/login.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 from amis import Form, InputText, InputPassword, DisplayModeEnum, Horizontal, Remark, Html, Page, AmisAPI, Wrapper, \
     Switch
 
 logo = Html(html=f'''
 <p align="center">
     <a href="https://github.com/ZM25XC/TeenStudy/">
-        <img src="https://i.328888.xyz/2023/02/23/xIh5k.png"
+        <img src="https://i.imgloc.com/2023/05/20/VyRjTV.png"
          width="256" height="256" alt="TeenStudy">
     </a>
 </p>
 <h2 align="center">大学习自动提交</h2>
 <div align="center">
     <a href="https://github.com/ZM25XC/TeenStudy/" target="_blank">
     Github仓库</a>
-    <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS" target="_blank">交流群</a>
+    <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS" target="_blank">QQ反馈群</a>
+    <a href="http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm" target="_blank">QQ体验群</a>
 </div>
 <br>
 <br>
 ''')
 login_api = AmisAPI(
     url='/TeenStudy/api/login',
     method='post',
     adaptor='''
         if (payload.status == 0) {
             localStorage.setItem("token", payload.data.token);
             localStorage.setItem("user_id", payload.data.user_id);
             localStorage.setItem("role", payload.data.role);
+            if(payload.data.role){
+            window.location.href = '/TeenStudy/admin'
+            }
+            else{
+            window.location.href = '/TeenStudy/home?user_id='+payload.data.user_id;}
         }
         return payload;
     '''
 )
 
 login_form = Form(api=login_api, title='', body=[
     InputText(name='user_id', label='用户ID', description='默认为用户QQ号'),
     InputPassword(name='password', label='密码',
                   description='管理员默认为admin，普通用户默认为QQ号'),
     Switch(name='role', label='身份组', onText='管理员', offText='用户', value=False,
            labelRemark=Remark(shape='circle', content='是否以管理员身份登录'))
-], mode=DisplayModeEnum.horizontal, horizontal=Horizontal(left=3, right=9, offset=5),
-                  redirect='${url}', submitText="登录")
+], mode=DisplayModeEnum.horizontal, horizontal=Horizontal(left=3, right=9, offset=5), submitText="登录")
 body = Wrapper(className='w-2/5 mx-auto my-0 m:w-full', body=login_form)
 login_page = Page(title='', body=[logo, body])
```

#### html2text {}

```diff
@@ -1,21 +1,23 @@
 from amis import Form, InputText, InputPassword, DisplayModeEnum, Horizontal,
 Remark, Html, Page, AmisAPI, Wrapper, \ Switch logo = Html(html=f'''
                                   [TeenStudy]
                        ***** å¤§å­¦ä¹ èªå¨æäº¤ *****
-                            Githubä»åº äº¤æµç¾¤
+                     Githubä»åº QQåé¦ç¾¤ QQä½éªç¾¤
 
 
 ''') login_api = AmisAPI( url='/TeenStudy/api/login', method='post',
 adaptor=''' if (payload.status == 0) { localStorage.setItem("token",
 payload.data.token); localStorage.setItem("user_id", payload.data.user_id);
-localStorage.setItem("role", payload.data.role); } return payload; ''' )
+localStorage.setItem("role", payload.data.role); if(payload.data.role)
+{ window.location.href = '/TeenStudy/admin' } else{ window.location.href = '/
+TeenStudy/home?user_id='+payload.data.user_id;} } return payload; ''' )
 login_form = Form(api=login_api, title='', body=[ InputText(name='user_id',
 label='ç¨æ·ID', description='é»è®¤ä¸ºç¨æ·QQå·'), InputPassword
 (name='password', label='å¯ç ',
 description='ç®¡çåé»è®¤ä¸ºadminï¼æ®éç¨æ·é»è®¤ä¸ºQQå·'), Switch
 (name='role', label='èº«ä»½ç»', onText='ç®¡çå', offText='ç¨æ·',
 value=False, labelRemark=Remark(shape='circle',
 content='æ¯å¦ä»¥ç®¡çåèº«ä»½ç»å½')) ], mode=DisplayModeEnum.horizontal,
-horizontal=Horizontal(left=3, right=9, offset=5), redirect='${url}',
-submitText="ç»å½") body = Wrapper(className='w-2/5 mx-auto my-0 m:w-full',
-body=login_form) login_page = Page(title='', body=[logo, body])
+horizontal=Horizontal(left=3, right=9, offset=5), submitText="ç»å½") body =
+Wrapper(className='w-2/5 mx-auto my-0 m:w-full', body=login_form) login_page =
+Page(title='', body=[logo, body])
```

### Comparing `TeenStudy-0.1.9/TeenStudy/web/utils/add.py` & `TeenStudy-0.2.0/TeenStudy/web/utils/add.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 import random
 import string
 import time
 
 from nonebot import logger
 
 from ...models.accuont import User
-from ...models.dxx import JiangXi
 from ...utils.utils import to_hash
 
 
 async def get_openid() -> str:
     return ''.join(random.sample(string.ascii_letters + string.digits, 28))
 
 
 async def write_to_database(data: dict) -> bool:
     try:
         if data["password"]:
             data["password"] = await to_hash(str(data["password"]))
         else:
             data["password"] = await to_hash(str(data["user_id"]))
+        if await User.filter(user_id=int(data["user_id"])).count():
+            return False
         if data["area"] in ["湖北", "江西"]:
             data["openid"] = await get_openid()
             if data["area"] == "江西":
-                result = await JiangXi.filter(organization_id=data["dxx_id"]).values()
-                data["organization"] = result[0]["organization"]
-                data["university_id"] = result[0]["university_id"]
-                data["college_id"] = result[0]["college_id"]
-                data["organization_id"]=data["dxx_id"]
+                data["university_type"] = data["university_type"].split("-")[0]
+                data["university_id"] = data["university"].split("-")[-1]
+                data["university"] = data["university"].split("-")[0]
+                data["college_id"] = data["college"].split("-")[-1]
+                data["college"] = data["college"].split("-")[0]
+                if data["organization"]:
+                    data["organization"] = data["organization"].split("-")[0]
+                else:
+                    data["organization_id"] = data["dxx_id"]
         start = {
             "time": time.time(),
             "user_id": None,
             "area": None,
             "name": None,
             "password": None,
             "group_id": None,
@@ -45,14 +50,15 @@
             "college_id": None,
             "college": None,
             "organization_id": None,
             "organization": None,
             "token": None,
             "cookie": None,
             "catalogue": None,
+            "auto_submit": True,
             "commit_time": None
         }
         start.update(data)
         await User.create(**start)
         return True
     except Exception as e:
         logger.error(e)
```

### Comparing `TeenStudy-0.1.9/TeenStudy/web/utils/status.py` & `TeenStudy-0.2.0/TeenStudy/web/utils/status.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.9/setup.py` & `TeenStudy-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,37 +11,38 @@
  'teenstudy.web.utils']
 
 package_data = \
 {'': ['*'], 'teenstudy': ['resource/*']}
 
 install_requires = \
 ['Jinja2>=3.1.2,<4.0.0',
- 'Pillow>=9.4.0,<10.0.0',
  'amis-python>=1.0.7,<2.0.0',
  'anti-useragent>=1.0.10,<2.0.0',
  'beautifulsoup4>=4.11.2,<5.0.0',
  'bs4>=0.0.1,<0.0.2',
+ 'ddddocr>=1.4.7,<2.0.0',
  'fastapi>=0.95.0,<0.96.0',
- 'httpx>=0.23.3,<0.24.0',
+ 'httpx>=0.24.0,<0.25.0',
  'lxml>=4.9.2,<5.0.0',
- 'nonebot-adapter-onebot>=2.2.1,<3.0.0',
- 'nonebot-plugin-apscheduler>=0.2.0,<0.3.0',
- 'nonebot2>=2.0.0rc2,<3.0.0',
+ 'nonebot-adapter-onebot>=2.2.3,<3.0.0',
+ 'nonebot-plugin-apscheduler>=0.3.0,<0.4.0',
+ 'nonebot2>=2.0.0,<3.0.0',
  'psutil>=5.9.4,<6.0.0',
+ 'pycryptodome>=3.17,<4.0',
  'python-jose>=3.3.0,<4.0.0',
  'qrcode>=7.4.2,<8.0.0',
  'tortoise-orm>=0.19.3,<0.20.0',
  'ujson>=5.7.0,<6.0.0',
  'uvicorn>=0.21.0,<0.22.0']
 
 setup_kwargs = {
     'name': 'teenstudy',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'description': '基于nonebot2异步框架的青年大学自动提交插件基于nonebot2的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图',
-    'long_description': '<div align="center">\n    <img src="https://i.328888.xyz/2023/02/28/z23ho.png" alt="TeenStudy.png" border="0" width="500px" height="500px"/>\n    <h1>TeenStudy</h1>\n    <b>基于nonebot2和go-cqhttp的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图</b>\n    <br/>\n    <a href="https://github.com/ZM25XC/TeenStudy/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://github.com/ZM25XC/TeenStudy/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://github.com/ZM25XC/TeenStudy/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://pypi.python.org/pypi/TeenStudy"><img src="https://img.shields.io/pypi/v/TeenStudy?color=yellow" alt="pypi"></a>\n  \t<a href="https://pypi.python.org/pypi/TeenStudy">\n    <img src="https://img.shields.io/pypi/dm/TeenStudy" alt="pypi download"></a>\n\t  <a href="https://github.com/ZM25XC/TeenStudy/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS">\n    <img src="https://img.shields.io/badge/QQ%E7%BE%A4-511173803-orange?style=flat-square" alt="QQ Chat Group">\n  </a>\n  </div>\n\n## 说明\n\n- 本项目为[青年大学习提交](https://github.com/ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`版\n- 本项目基于[nonebot2](https://github.com/nonebot/nonebot2)和[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)，使用本插件前请先阅读以上两个项目的使用文档\n-  **启动插件之后，一定要登录后台在推送列表中添加需要开启大学习功能的群聊**\n-  **本项目无法在国外IP环境下使用，如有开启代理，请关闭或添加代理规则**\n- 需要抓包的地区，绑定后尽量别进官方公众号，避免token或cookie刷新导致无法提交\n- 本项目需要部署在公网可访问的容器中，并开放端口（nonebot2配置的port），否则大部分功能将出现异常\n- 欢迎加入[QQ群](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)，交流讨论。\n- 时间精力有限，目前只维护湖北和江西两个地区，其他地区出问题请提交Issues,我找个时间修，需要增加地区请进群帮忙测试，个别地区没账号无法测试\n\n- 觉得项目不错，不妨点个stars.\n\n## 地区状态\n\n<details>\n\n| 共青团名称 | 开发状态 | 备注 |\n|:-----:|:----:|:----:|\n|青春湖北|支持|无需抓包|\n|江西共青团|支持|无需抓包|\n|安徽共青团|支持|无需抓包|\n|广东共青团|支持|无需抓包|\n|青春上海|支持|微信扫码绑定|\n|青春浙江|支持|微信扫码绑定|\n|江苏共青团|支持|需要自行抓包|\n|青春山东|支持|需要自行抓包|\n|重庆共青团|支持|需要自行抓包|\n|吉青飞扬|支持|需要自行抓包|\n|黑龙江共青团|支持|需要自行抓包，该地区上线测试中|\n|天府新青年|支持|不进入公众号token时效大于1周|\n|河南共青团|不支持|cookie时效小于1周|\n|广西青年圈|待开发||\n|青春湖南|待开发||\n|甘肃青年|待开发||\n|山西青年|待开发||\n|河北共青团|待开发||\n|福建共青团|待开发||\n|内蒙古青年|待开发||\n|云南共青团|待开发||\n|三秦青年|待开发||\n|青春北京|待开发||\n|海南共青团|待开发||\n|津彩青春|待开发||\n|青春黔言|待开发||\n|青春柳州|待开发||\n|辽宁共青团|待开发||\n|宁夏共青团|待开发||\n|新疆共青团|待开发||\n|西藏共青团|待开发||\n</details>\n\n\n##  安装及更新\n\n<details>\n<summary>第一种方式(不推荐)</summary>\n\n- 使用`git clone https://github.com/ZM25XC/TeenStudy.git`指令克隆本仓库或下载压缩包文件\n\n</details>\n\n<details>\n<summary>第二种方式(二选一)</summary>\n\n- 使用`pip install TeenStudy`来进行安装,使用`pip install TeenStudy -U`进行更新\n- 使用`nb plugin install TeenStudy`来进行安装,使用`nb plugin install TeenStudy -U`进行更新\n\n</details>\n\n\n## 导入插件\n\n<details>\n<summary>使用第一种方式安装看此方法</summary>\n\n- 将`TeenStudy`放在nb的`plugins`目录下，运行nb机器人即可\n\n- 文件结构如下\n\n    ```py\n    📦 AweSome-Bot\n    ├── 📂 awesome_bot\n    │   └── 📂 plugins\n    |       └── 📂 TeenStudy\n    |           └── 📜 __init__.py\n    ├── 📜 .env.prod\n    ├── 📜 .gitignore\n    ├── 📜 pyproject.toml\n    └── 📜 README.md\n    ```\n\n    \n\n</details>\n\n<details>\n<summary>使用第二种方式安装看此方法</summary>\n\n- 在`pyproject.toml`里的`[tool.nonebot]`中添加`plugins = ["TeenStudy"]`\n\n</details>\n\n## 机器人配置\n\n- 在nonebot的`.env` 或 `.env.prod`配置文件中修改nonebot2的`HOST`为`0.0.0.0`、设置好超管账号和公网IP\n\n  ```py\n  HOST = "0.0.0.0"  #nonebot2监听的IP\n  SUPERUSERS = [""] # 超级用户\n  COMMAND_START=[""] # 命令前缀,根据需要自行修改\n  DXX_IP = ""\n  ```\n\n## 使用方式\n\n- 启动nb,等待插件加载数据，加载完毕后登录后台，账号默认为`nonebot配置文件中的超管账号`，密码默认为：`admin`,开放端口（默认为.env中配置的port）\n- 在管理后台的推送列表中添加需要开启大学习使用的群聊\n\n## 功能列表\n|    指令    |               指令格式               |                               说明                               |\n| :--------: | :----------------------------------: | :--------------------------------------------------------------: |\n| 添加大学习 |           添加大学习`地区`           |                    添加大学习湖北 添加大学习                     |\n| 我的大学习 |              我的大学习              |                           查询个人信息                           |\n| 提交大学习 |         提交大学习 戳一戳Bot         |                        提交最新一期大学习                        |\n|   大学习   |     大学习答案、大学习、答案截图     |                    获取最新一期青年大学习答案                    |\n|  完成截图  | 完成截图、大学习截图、大学习完成截图 |            获取最新一期青年大学习完成截图（带状态栏）            |\n| 完成大学习 |        完成大学习、全员大学习        | 团支书可用，需要成员填写团支书ID，填写后团支书可发指令提交大学习 |\n|  重置配置  |          重置配置、刷新配置          |                   超管可用，刷新Web UI默认配置                   |\n|  重置密码  |               重置密码               |                   重置登录Web UI的密码为用户ID                   |\n|删除大学习|删除大学习|用户申请清除数据库的信息|\n|导出用户数据|导出用户数据、导出数据|将数据导出至TeenStudy目录下|\n|更新用户数据|更新用户数据、刷新用户数据|将用户数据导入到数据库|\n|更新资源数据|更新资源数据、刷新资源数据|更新数据库中的资源数据（江西共青团团支部数据）|\n\n\n## ToDo\n\n\n- [ ] 增加更多地区支持\n- [ ] 优化 Bot\n\n\n## 更新日志\n\n### 2023/05/21\n\n- 增加黑龙江地区，需要自行抓包，该地区上线测试中，请积极提issue反馈\n- 下版本为大版本更新，将添加新功能，优化功能，请积极提issue反馈或加交流群反馈\n\n<details>\n<summary>2023/05/11</summary> \n\n- 增加广东地区，无需抓包[#13](https://github.com/ZM25XC/TeenStudy/issues/13)，感谢[@neal240](https://github.com/neal240)提供账号测试\n\n</details>\n\n<details>\n<summary>2023/05/06</summary> \n\n- 增加吉林地区，需要自行抓包\n- 修复超管更改登录密码后用原密码能继续登录问题\n- 添加二维码转链接开关，需要自行在后台配置页面打开\n- 调整部分依赖\n\n</details>\n\n<details>\n<summary> 2023/04/12</summary> \n\n- 因河南地区cookie时效小于1周，移除河南地区\n- 添加`删除大学习`功能，用户可自行删除数据\n- 添加`导出用户数据`功能\n- 添加`更新用户数据`功能\n- 添加`更新资源数据`功能，江西地区更新后请使用下此功能刷新团支部数据\n- 添加戳一戳提交大学习开关，默认开启，请在Web UI后台配置页面进行修改\n- 添加大学习提醒开关，默认开启，支持修改时间，请在Web UI后台配置页面进行修改\n- 添加自动提交大学习开关，默认开启，支持修改时间，请在Web UI后台进行修改\n- 调整安徽地区添加方式[#9](https://github.com/ZM25XC/TeenStudy/issues/9)，无需抓包，感谢[@yhzcake](https://github.com/yhzcake)测试提供方法\n- 修复Web UI 首页公网IP显示异常\n- 修复浙江地区用户重复显示\n- 更新江西共青团团支部数据\n  \n</details>\n\n\n<details>\n<summary>2023/03/18</summary>\n\n- 适配河南地区，需要自行抓包\n- 适配四川地区，需要自行抓包\n- 适配山东地区，需要自行抓包\n- 适配重庆地区，需要自行抓包\n- 添加自动获取公网IP功能，别再问如何配置公网IP啦\n- 添加重置密码功能，指令`重置密码`\n- 添加重置配置功能，指令`重置配置`，`刷新配置`\n- 添加完成大学习功能，团支书可一次性提交全班的大学习，指令`完成大学习`，`全员大学习`\n- 管理后台开放添加用户权限（浙江，上海地区无法添加）\n- 优化用户信息页\n- 优化登录界面提示\n- 将添加链接，登录链接转化成二维码，减少公网IP暴露，没啥用，样式好看一些\n- 修复Ubuntu系统导入资源失败BUG\n  \n</details>\n\n<details>\n\n<summary>2023/03/05</summary>\n\n- 适配浙江地区，使用微信扫码进行绑定\n- 适配上海地区，使用微信扫码进行绑定\n- 适配江苏地区，需要自行抓包\n- 适配安徽地区，需要自行抓包\n\n</details>\n\n<details>\n<summary>2023/03/01</summary>\n\n- 将代码上传至pypi，可使用`pip install TeenStudy`指令安装本插件\n- 上传基础代码\n- 适配湖北地区，无需抓包，安装即用\n- 适配江西地区，无需抓包，安装即用\n\n</details>\n',
+    'long_description': '<div align="center">\n    <img src="https://img1.imgtp.com/2023/06/11/sG4KdlpL.png" alt="TeenStudy.png" border="0" width="500px" height="500px"/>\n    <h1>TeenStudy</h1>\n    <b>基于nonebot2和go-cqhttp的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图</b>\n    <br/>\n    <a href="https://github.com/ZM25XC/TeenStudy/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://github.com/ZM25XC/TeenStudy/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://github.com/ZM25XC/TeenStudy/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://pypi.python.org/pypi/TeenStudy"><img src="https://img.shields.io/pypi/v/TeenStudy?color=yellow" alt="pypi"></a>\n  \t<a href="https://pypi.python.org/pypi/TeenStudy">\n    <img src="https://img.shields.io/pypi/dm/TeenStudy" alt="pypi download"></a>\n\t  <a href="https://github.com/ZM25XC/TeenStudy/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS">\n    <img src="https://img.shields.io/badge/QQ反馈群-511173803-orange?style=flat-square" alt="QQ Chat Group">\n  </a>\n\t<a href="http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm">\n    <img src="https://img.shields.io/badge/QQ体验群-821280615-orange?style=flat-square" alt="QQ Chat Group">\n  </a>\n  </div>\n\n## 说明\n\n- 本项目为[青年大学习提交](https://github.com/ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`版\n- 本项目基于[nonebot2](https://github.com/nonebot/nonebot2)和[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)，使用本插件前请先阅读以上两个项目的使用文档\n-  **启动插件之后，一定要登录后台在推送列表中添加需要开启大学习功能的群聊**\n-  **本项目无法在国外IP环境下使用，如有开启代理，请关闭或添加代理规则**\n- 需要抓包的地区，绑定后尽量别进官方公众号，避免token或cookie刷新导致无法提交\n- 本项目需要部署在公网可访问的容器中，并开放端口（nonebot2配置的port），否则大部分功能将出现异常\n- 欢迎加入[QQ反馈群](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)，交流讨论，如您不会搭建又想每周自动提交，可加入[QQ体验群](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm)。\n- 时间精力有限，目前只维护湖北和江西两个地区，其他地区出问题请提交Issues,我找个时间修，需要增加地区请进群帮忙测试，个别地区没账号无法测试\n\n- 觉得项目不错，不妨点个stars.\n\n## 地区状态\n\n<details>\n\n| 共青团名称 | 开发状态 | 备注 |\n|:-----:|:----:|:----:|\n|青春湖北|支持|无需抓包|\n|江西共青团|支持|无需抓包|\n|安徽共青团|支持|无需抓包|\n|广东共青团|支持|无需抓包|\n|青春北京|支持|无需抓包|\n|青春上海|支持|微信扫码绑定|\n|青春浙江|支持|微信扫码绑定|\n|津彩青春|支持|需要自行抓包|\n|青春山东|支持|需要自行抓包|\n|重庆共青团|支持|需要自行抓包|\n|吉青飞扬|支持|需要自行抓包|\n|天府新青年|支持|不进入公众号token时效大于1周|\n|河南共青团|不支持|cookie时效小于1周|\n|江苏共青团|不支持|cookie失效小于1周|\n|黑龙江共青团|不支持|cookie失效小于1周|\n|广西青年圈|待开发||\n|青春湖南|待开发||\n|甘肃青年|待开发||\n|山西青年|待开发||\n|河北共青团|待开发||\n|福建共青团|待开发||\n|内蒙古青年|待开发||\n|云南共青团|待开发||\n|三秦青年|待开发||\n|海南共青团|待开发||\n|青春黔言|待开发||\n|青春柳州|待开发||\n|辽宁共青团|待开发||\n|宁夏共青团|待开发||\n|新疆共青团|待开发||\n|西藏共青团|待开发||\n</details>\n\n\n##  安装及更新\n\n<details>\n<summary>第一种方式(不推荐)</summary>\n\n- 使用`git clone https://github.com/ZM25XC/TeenStudy.git`指令克隆本仓库或下载压缩包文件\n\n</details>\n\n<details>\n<summary>第二种方式(二选一)</summary>\n\n- 使用`pip install TeenStudy`来进行安装,使用`pip install TeenStudy -U`进行更新\n- 使用`nb plugin install TeenStudy`来进行安装,使用`nb plugin install TeenStudy -U`进行更新\n\n</details>\n\n\n## 导入插件\n\n<details>\n<summary>使用第一种方式安装看此方法</summary>\n\n- 将`TeenStudy`放在nb的`plugins`目录下，运行nb机器人即可\n\n- 文件结构如下\n\n    ```py\n    📦 AweSome-Bot\n    ├── 📂 awesome_bot\n    │   └── 📂 plugins\n    |       └── 📂 TeenStudy\n    |           └── 📜 __init__.py\n    ├── 📜 .env.prod\n    ├── 📜 .gitignore\n    ├── 📜 pyproject.toml\n    └── 📜 README.md\n    ```\n\n    \n\n</details>\n\n<details>\n<summary>使用第二种方式安装看此方法</summary>\n\n- 在`pyproject.toml`里的`[tool.nonebot]`中添加`plugins = ["TeenStudy"]`\n\n</details>\n\n## 机器人配置\n\n- 在nonebot的`.env` 或 `.env.prod`配置文件中修改nonebot2的`HOST`为`0.0.0.0`、设置好超管账号和公网IP\n\n  ```py\n  HOST = "0.0.0.0"  #nonebot2监听的IP\n  SUPERUSERS = [""] # 超级用户\n  COMMAND_START=[""] # 命令前缀,根据需要自行修改\n  DXX_IP = ""\n  ```\n\n## 使用方式\n\n- 启动nb,等待插件加载数据，加载完毕后登录后台，账号默认为`nonebot配置文件中的超管账号`，密码默认为：`admin`,开放端口（默认为.env中配置的port）\n- 在管理后台的推送列表中添加需要开启大学习使用的群聊\n\n## 功能列表\n|    指令    |               指令格式               |                               说明                               |\n| :--------: | :----------------------------------: | :--------------------------------------------------------------: |\n| 添加大学习 |           添加大学习`地区`           |                    添加大学习湖北 添加大学习                     |\n| 我的大学习 |              我的大学习              |                           查询个人信息                           |\n| 提交大学习 |         提交大学习 戳一戳Bot         |                        提交最新一期大学习                        |\n|   大学习   |     大学习答案、大学习、答案截图     |                    获取最新一期青年大学习答案                    |\n|  完成截图  | 完成截图、大学习截图、大学习完成截图 |            获取最新一期青年大学习完成截图（带状态栏）            |\n| 完成大学习 |        完成大学习、全员大学习        | 团支书可用，需要成员填写团支书ID，填写后团支书可发指令提交大学习 |\n|  重置配置  |          重置配置、刷新配置          |                   超管可用，刷新Web UI默认配置                   |\n|  重置密码  |               重置密码               |                   重置登录Web UI的密码为用户ID                   |\n|删除大学习|删除大学习|用户申请清除数据库的信息|\n|导出用户数据|导出用户数据、导出数据|将数据导出至TeenStudy目录下|\n|更新用户数据|更新用户数据、刷新用户数据|将用户数据导入到数据库|\n|更新资源数据|更新资源数据、刷新资源数据|更新数据库中的资源数据（江西共青团团支部数据）|\n\n\n## ToDo\n\n\n- [ ] 增加更多地区支持\n- [ ] 优化 Bot\n\n\n## 更新日志\n\n### 2023/06/12\n\n- 适配北京地区，无需抓包\n- 增加天津地区，需要自行抓包\n- 因江苏和黑龙江地区Cookie时效小于1周，移除江苏和黑龙江地区\n- Web UI添加日志和主动退出功能\n- 更新江西地区拉取团支部数据方式，移除缓存团支部数据，包体积减小50%\n- 修复大学习公网检测失败问题\n- 更新Nonebot2强制meta字段\n- 同步UI依赖AMIS版本到最新版本\n- 开放体验群，不会搭建又想使用的可加[QQ体验群](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm)\n  \n\n<details>\n\n<summary>2023/05/21</summary>\n\n- 增加黑龙江地区，需要自行抓包，该地区上线测试中，请积极提issue反馈\n- 下版本为大版本更新，将添加新功能，优化功能，请积极提issue反馈或加交流群反馈\n- \n</details>\n\n\n<details>\n<summary>2023/05/11</summary> \n\n- 增加广东地区，无需抓包[#13](https://github.com/ZM25XC/TeenStudy/issues/13)，感谢[@neal240](https://github.com/neal240)提供账号测试\n\n</details>\n\n<details>\n<summary>2023/05/06</summary> \n\n- 增加吉林地区，需要自行抓包\n- 修复超管更改登录密码后用原密码能继续登录问题\n- 添加二维码转链接开关，需要自行在后台配置页面打开\n- 调整部分依赖\n\n</details>\n\n<details>\n<summary> 2023/04/12</summary> \n\n- 因河南地区cookie时效小于1周，移除河南地区\n- 添加`删除大学习`功能，用户可自行删除数据\n- 添加`导出用户数据`功能\n- 添加`更新用户数据`功能\n- 添加`更新资源数据`功能，江西地区更新后请使用下此功能刷新团支部数据\n- 添加戳一戳提交大学习开关，默认开启，请在Web UI后台配置页面进行修改\n- 添加大学习提醒开关，默认开启，支持修改时间，请在Web UI后台配置页面进行修改\n- 添加自动提交大学习开关，默认开启，支持修改时间，请在Web UI后台进行修改\n- 调整安徽地区添加方式[#9](https://github.com/ZM25XC/TeenStudy/issues/9)，无需抓包，感谢[@yhzcake](https://github.com/yhzcake)测试提供方法\n- 修复Web UI 首页公网IP显示异常\n- 修复浙江地区用户重复显示\n- 更新江西共青团团支部数据\n  \n</details>\n\n\n<details>\n<summary>2023/03/18</summary>\n\n- 适配河南地区，需要自行抓包\n- 适配四川地区，需要自行抓包\n- 适配山东地区，需要自行抓包\n- 适配重庆地区，需要自行抓包\n- 添加自动获取公网IP功能，别再问如何配置公网IP啦\n- 添加重置密码功能，指令`重置密码`\n- 添加重置配置功能，指令`重置配置`，`刷新配置`\n- 添加完成大学习功能，团支书可一次性提交全班的大学习，指令`完成大学习`，`全员大学习`\n- 管理后台开放添加用户权限（浙江，上海地区无法添加）\n- 优化用户信息页\n- 优化登录界面提示\n- 将添加链接，登录链接转化成二维码，减少公网IP暴露，没啥用，样式好看一些\n- 修复Ubuntu系统导入资源失败BUG\n  \n</details>\n\n<details>\n\n<summary>2023/03/05</summary>\n\n- 适配浙江地区，使用微信扫码进行绑定\n- 适配上海地区，使用微信扫码进行绑定\n- 适配江苏地区，需要自行抓包\n- 适配安徽地区，需要自行抓包\n\n</details>\n\n<details>\n<summary>2023/03/01</summary>\n\n- 将代码上传至pypi，可使用`pip install TeenStudy`指令安装本插件\n- 上传基础代码\n- 适配湖北地区，无需抓包，安装即用\n- 适配江西地区，无需抓包，安装即用\n\n</details>\n',
     'author': 'ZM25XC',
     'author_email': 'xingling25@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ZM25XC/TeenStudy',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,43 +1,45 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['teenstudy',
 'teenstudy.models', 'teenstudy.utils', 'teenstudy.web', 'teenstudy.web.api',
 'teenstudy.web.pages', 'teenstudy.web.utils'] package_data = \ {'': ['*'],
 'teenstudy': ['resource/*']} install_requires = \ ['Jinja2>=3.1.2,<4.0.0',
-'Pillow>=9.4.0,<10.0.0', 'amis-python>=1.0.7,<2.0.0', 'anti-
-useragent>=1.0.10,<2.0.0', 'beautifulsoup4>=4.11.2,<5.0.0',
-'bs4>=0.0.1,<0.0.2', 'fastapi>=0.95.0,<0.96.0', 'httpx>=0.23.3,<0.24.0',
-'lxml>=4.9.2,<5.0.0', 'nonebot-adapter-onebot>=2.2.1,<3.0.0', 'nonebot-plugin-
-apscheduler>=0.2.0,<0.3.0', 'nonebot2>=2.0.0rc2,<3.0.0',
-'psutil>=5.9.4,<6.0.0', 'python-jose>=3.3.0,<4.0.0', 'qrcode>=7.4.2,<8.0.0',
+'amis-python>=1.0.7,<2.0.0', 'anti-useragent>=1.0.10,<2.0.0',
+'beautifulsoup4>=4.11.2,<5.0.0', 'bs4>=0.0.1,<0.0.2', 'ddddocr>=1.4.7,<2.0.0',
+'fastapi>=0.95.0,<0.96.0', 'httpx>=0.24.0,<0.25.0', 'lxml>=4.9.2,<5.0.0',
+'nonebot-adapter-onebot>=2.2.3,<3.0.0', 'nonebot-plugin-
+apscheduler>=0.3.0,<0.4.0', 'nonebot2>=2.0.0,<3.0.0', 'psutil>=5.9.4,<6.0.0',
+'pycryptodome>=3.17,<4.0', 'python-jose>=3.3.0,<4.0.0', 'qrcode>=7.4.2,<8.0.0',
 'tortoise-orm>=0.19.3,<0.20.0', 'ujson>=5.7.0,<6.0.0',
 'uvicorn>=0.21.0,<0.22.0'] setup_kwargs = { 'name': 'teenstudy', 'version':
-'0.1.9', 'description':
+'0.2.0', 'description':
 'åºäºnonebot2å¼æ­¥æ¡æ¶çéå¹´å¤§å­¦èªå¨æäº¤æä»¶åºäºnonebot2çéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾',
 'long_description': '
                              \n [TeenStudy.png]\n
                             ****** TeenStudy ******
                             \n åºäºnonebot2ågo-
 cqhttpçéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾\n
 
   \n [GitHub_issues]\n [GitHub_forks]\n [GitHub_stars]\n [pypi]\n \t\n_[pypi
-            download]\n\t [GitHub_license]\n \n_[QQ_Chat_Group]\n\n
+download]\n\t [GitHub_license]\n \n_[QQ_Chat_Group]\n\n\t\n_[QQ_Chat_Group]\n\n
 \n\n## è¯´æ\n\n- æ¬é¡¹ç®ä¸º[éå¹´å¤§å­¦ä¹ æäº¤](https://github.com/
 ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`ç\n- æ¬é¡¹ç®åºäº[nonebot2]
 (https://github.com/nonebot/nonebot2)å[go-cqhttp](https://github.com/Mrs4s/
 go-cqhttp)ï¼ä½¿ç¨æ¬æä»¶åè¯·åéè¯»ä»¥ä¸ä¸¤ä¸ªé¡¹ç®çä½¿ç¨ææ¡£\n-
 **å¯å¨æä»¶ä¹åï¼ä¸å®è¦ç»å½åå°å¨æ¨éåè¡¨ä¸­æ·»å éè¦å¼å¯å¤§å­¦ä¹ åè½çç¾¤è**\n-
 **æ¬é¡¹ç®æ æ³å¨å½å¤IPç¯å¢ä¸ä½¿ç¨ï¼å¦æå¼å¯ä»£çï¼è¯·å³é­ææ·»å ä»£çè§å**\n-
 éè¦æåçå°åºï¼ç»å®åå°½éå«è¿å®æ¹å¬ä¼å·ï¼é¿åtokenæcookieå·æ°å¯¼è´æ æ³æäº¤\n-
 æ¬é¡¹ç®éè¦é¨ç½²å¨å¬ç½å¯è®¿é®çå®¹å¨ä¸­ï¼å¹¶å¼æ¾ç«¯å£ï¼nonebot2éç½®çportï¼ï¼å¦åå¤§é¨ååè½å°åºç°å¼å¸¸\n-
-æ¬¢è¿å å¥[QQç¾¤](https://jq.qq.com/
-?_wv=1027&k=NGFEwXyS)ï¼äº¤æµè®¨è®ºã\n-
+æ¬¢è¿å å¥[QQåé¦ç¾¤](https://jq.qq.com/
+?_wv=1027&k=NGFEwXyS)ï¼äº¤æµè®¨è®ºï¼å¦æ¨ä¸ä¼æ­å»ºåæ³æ¯å¨èªå¨æäº¤ï¼å¯å å¥
+[QQä½éªç¾¤](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-
+ai2aPGToBKm)ã\n-
 æ¶é´ç²¾åæéï¼ç®ååªç»´æ¤æ¹ååæ±è¥¿ä¸¤ä¸ªå°åºï¼å¶ä»å°åºåºé®é¢è¯·æäº¤Issues,ææ¾ä¸ªæ¶é´ä¿®ï¼éè¦å¢å å°åºè¯·è¿ç¾¤å¸®å¿æµè¯ï¼ä¸ªå«å°åºæ²¡è´¦å·æ æ³æµè¯\n\n-
 è§å¾é¡¹ç®ä¸éï¼ä¸å¦¨ç¹ä¸ªstars.\n\n## å°åºç¶æ\n\n\n\n|
 å±éå¢åç§° | å¼åç¶æ | å¤æ³¨ |\n|:-----:|:----:|:----:
-|\n|éæ¥æ¹å|æ¯æ|æ éæå|\n|æ±è¥¿å±éå¢|æ¯æ|æ éæå|\n|å®å¾½å±éå¢|æ¯æ|æ éæå|\n|å¹¿ä¸å±éå¢|æ¯æ|æ éæå|\n|éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|\n|éæ¥æµæ±|æ¯æ|å¾®ä¿¡æ«ç ç»å®|\n|æ±èå±éå¢|æ¯æ|éè¦èªè¡æå|\n|éæ¥å±±ä¸|æ¯æ|éè¦èªè¡æå|\n|éåºå±éå¢|æ¯æ|éè¦èªè¡æå|\n|åéé£æ¬|æ¯æ|éè¦èªè¡æå|\n|é»é¾æ±å±éå¢|æ¯æ|éè¦èªè¡æåï¼è¯¥å°åºä¸çº¿æµè¯ä¸­|\n|å¤©åºæ°éå¹´|æ¯æ|ä¸è¿å¥å¬ä¼å·tokenæ¶æå¤§äº1å¨|\n|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨|\n|å¹¿è¥¿éå¹´å|å¾å¼å||\n|éæ¥æ¹å|å¾å¼å||\n|çèéå¹´|å¾å¼å||\n|å±±è¥¿éå¹´|å¾å¼å||\n|æ²³åå±éå¢|å¾å¼å||\n|ç¦å»ºå±éå¢|å¾å¼å||\n|åèå¤éå¹´|å¾å¼å||\n|äºåå±éå¢|å¾å¼å||\n|ä¸ç§¦éå¹´|å¾å¼å||\n|éæ¥åäº¬|å¾å¼å||\n|æµ·åå±éå¢|å¾å¼å||\n|æ´¥å½©éæ¥|å¾å¼å||\n|éæ¥é»è¨|å¾å¼å||\n|éæ¥æ³å·|å¾å¼å||\n|è¾½å®å±éå¢|å¾å¼å||\n|å®å¤å±éå¢|å¾å¼å||\n|æ°çå±éå¢|å¾å¼å||\n|è¥¿èå±éå¢|å¾å¼å||\n\n\n\n##
+|\n|éæ¥æ¹å|æ¯æ|æ éæå|\n|æ±è¥¿å±éå¢|æ¯æ|æ éæå|\n|å®å¾½å±éå¢|æ¯æ|æ éæå|\n|å¹¿ä¸å±éå¢|æ¯æ|æ éæå|\n|éæ¥åäº¬|æ¯æ|æ éæå|\n|éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|\n|éæ¥æµæ±|æ¯æ|å¾®ä¿¡æ«ç ç»å®|\n|æ´¥å½©éæ¥|æ¯æ|éè¦èªè¡æå|\n|éæ¥å±±ä¸|æ¯æ|éè¦èªè¡æå|\n|éåºå±éå¢|æ¯æ|éè¦èªè¡æå|\n|åéé£æ¬|æ¯æ|éè¦èªè¡æå|\n|å¤©åºæ°éå¹´|æ¯æ|ä¸è¿å¥å¬ä¼å·tokenæ¶æå¤§äº1å¨|\n|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨|\n|æ±èå±éå¢|ä¸æ¯æ|cookieå¤±æå°äº1å¨|\n|é»é¾æ±å±éå¢|ä¸æ¯æ|cookieå¤±æå°äº1å¨|\n|å¹¿è¥¿éå¹´å|å¾å¼å||\n|éæ¥æ¹å|å¾å¼å||\n|çèéå¹´|å¾å¼å||\n|å±±è¥¿éå¹´|å¾å¼å||\n|æ²³åå±éå¢|å¾å¼å||\n|ç¦å»ºå±éå¢|å¾å¼å||\n|åèå¤éå¹´|å¾å¼å||\n|äºåå±éå¢|å¾å¼å||\n|ä¸ç§¦éå¹´|å¾å¼å||\n|æµ·åå±éå¢|å¾å¼å||\n|éæ¥é»è¨|å¾å¼å||\n|éæ¥æ³å·|å¾å¼å||\n|è¾½å®å±éå¢|å¾å¼å||\n|å®å¤å±éå¢|å¾å¼å||\n|æ°çå±éå¢|å¾å¼å||\n|è¥¿èå±éå¢|å¾å¼å||\n\n\n\n##
 å®è£åæ´æ°\n\n\nç¬¬ä¸ç§æ¹å¼(ä¸æ¨è)\n\n- ä½¿ç¨`git clone https://
 github.com/ZM25XC/
 TeenStudy.git`æä»¤åéæ¬ä»åºæä¸è½½åç¼©åæä»¶\n\n\n\n\nç¬¬äºç§æ¹å¼
 (äºéä¸)\n\n- ä½¿ç¨`pip install TeenStudy`æ¥è¿è¡å®è£,ä½¿ç¨`pip
 install TeenStudy -U`è¿è¡æ´æ°\n- ä½¿ç¨`nb plugin install
 TeenStudy`æ¥è¿è¡å®è£,ä½¿ç¨`nb plugin install TeenStudy -
 U`è¿è¡æ´æ°\n\n\n\n\n##
@@ -69,19 +71,28 @@
 å®æå¤§å­¦ä¹  | å®æå¤§å­¦ä¹ ãå¨åå¤§å­¦ä¹  |
 å¢æ¯ä¹¦å¯ç¨ï¼éè¦æåå¡«åå¢æ¯ä¹¦IDï¼å¡«ååå¢æ¯ä¹¦å¯åæä»¤æäº¤å¤§å­¦ä¹ 
 |\n| éç½®éç½® | éç½®éç½®ãå·æ°éç½® | è¶ç®¡å¯ç¨ï¼å·æ°Web
 UIé»è®¤éç½® |\n| éç½®å¯ç  | éç½®å¯ç  | éç½®ç»å½Web
 UIçå¯ç ä¸ºç¨æ·ID
 |\n|å é¤å¤§å­¦ä¹ |å é¤å¤§å­¦ä¹ |ç¨æ·ç³è¯·æ¸é¤æ°æ®åºçä¿¡æ¯|\n|å¯¼åºç¨æ·æ°æ®|å¯¼åºç¨æ·æ°æ®ãå¯¼åºæ°æ®|å°æ°æ®å¯¼åºè³TeenStudyç®å½ä¸|\n|æ´æ°ç¨æ·æ°æ®|æ´æ°ç¨æ·æ°æ®ãå·æ°ç¨æ·æ°æ®|å°ç¨æ·æ°æ®å¯¼å¥å°æ°æ®åº|\n|æ´æ°èµæºæ°æ®|æ´æ°èµæºæ°æ®ãå·æ°èµæºæ°æ®|æ´æ°æ°æ®åºä¸­çèµæºæ°æ®ï¼æ±è¥¿å±éå¢å¢æ¯é¨æ°æ®ï¼|\n\n\n##
 ToDo\n\n\n- [ ] å¢å æ´å¤å°åºæ¯æ\n- [ ] ä¼å Bot\n\n\n##
-æ´æ°æ¥å¿\n\n### 2023/05/21\n\n-
+æ´æ°æ¥å¿\n\n### 2023/06/12\n\n- ééåäº¬å°åºï¼æ éæå\n-
+å¢å å¤©æ´¥å°åºï¼éè¦èªè¡æå\n-
+å æ±èåé»é¾æ±å°åºCookieæ¶æå°äº1å¨ï¼ç§»é¤æ±èåé»é¾æ±å°åº\n-
+Web UIæ·»å æ¥å¿åä¸»å¨éåºåè½\n-
+æ´æ°æ±è¥¿å°åºæåå¢æ¯é¨æ°æ®æ¹å¼ï¼ç§»é¤ç¼å­å¢æ¯é¨æ°æ®ï¼åä½ç§¯åå°50%\n-
+ä¿®å¤å¤§å­¦ä¹ å¬ç½æ£æµå¤±è´¥é®é¢\n- æ´æ°Nonebot2å¼ºå¶metaå­æ®µ\n-
+åæ­¥UIä¾èµAMISçæ¬å°ææ°çæ¬\n-
+å¼æ¾ä½éªç¾¤ï¼ä¸ä¼æ­å»ºåæ³ä½¿ç¨çå¯å [QQä½éªç¾¤](http://
+qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm)\n
+\n\n\n\n2023/05/21\n\n-
 å¢å é»é¾æ±å°åºï¼éè¦èªè¡æåï¼è¯¥å°åºä¸çº¿æµè¯ä¸­ï¼è¯·ç§¯ææissueåé¦\n-
-ä¸çæ¬ä¸ºå¤§çæ¬æ´æ°ï¼å°æ·»å æ°åè½ï¼ä¼ååè½ï¼è¯·ç§¯ææissueåé¦æå äº¤æµç¾¤åé¦\n\n\n2023/
-05/11 \n\n- å¢å å¹¿ä¸å°åºï¼æ éæå[#13](https://github.com/ZM25XC/
-TeenStudy/issues/13)ï¼æè°¢[@neal240](https://github.com/
+ä¸çæ¬ä¸ºå¤§çæ¬æ´æ°ï¼å°æ·»å æ°åè½ï¼ä¼ååè½ï¼è¯·ç§¯ææissueåé¦æå äº¤æµç¾¤åé¦\n-
+\n\n\n\n\n2023/05/11 \n\n- å¢å å¹¿ä¸å°åºï¼æ éæå[#13](https://
+github.com/ZM25XC/TeenStudy/issues/13)ï¼æè°¢[@neal240](https://github.com/
 neal240)æä¾è´¦å·æµè¯\n\n\n\n\n2023/05/06 \n\n-
 å¢å åæå°åºï¼éè¦èªè¡æå\n-
 ä¿®å¤è¶ç®¡æ´æ¹ç»å½å¯ç åç¨åå¯ç è½ç»§ç»­ç»å½é®é¢\n-
 æ·»å äºç»´ç è½¬é¾æ¥å¼å³ï¼éè¦èªè¡å¨åå°éç½®é¡µé¢æå¼\n-
 è°æ´é¨åä¾èµ\n\n\n\n\n 2023/04/12 \n\n-
 å æ²³åå°åºcookieæ¶æå°äº1å¨ï¼ç§»é¤æ²³åå°åº\n-
 æ·»å `å é¤å¤§å­¦ä¹ `åè½ï¼ç¨æ·å¯èªè¡å é¤æ°æ®\n-
```

### Comparing `TeenStudy-0.1.9/PKG-INFO` & `TeenStudy-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,102 +1,106 @@
 Metadata-Version: 2.1
 Name: teenstudy
-Version: 0.1.9
+Version: 0.2.0
 Summary: 基于nonebot2异步框架的青年大学自动提交插件基于nonebot2的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图
 Home-page: https://github.com/ZM25XC/TeenStudy
 License: MIT
 Author: ZM25XC
 Author-email: xingling25@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: Pillow (>=9.4.0,<10.0.0)
 Requires-Dist: amis-python (>=1.0.7,<2.0.0)
 Requires-Dist: anti-useragent (>=1.0.10,<2.0.0)
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
+Requires-Dist: ddddocr (>=1.4.7,<2.0.0)
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0)
-Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
+Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0,<0.4.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
+Requires-Dist: pycryptodome (>=3.17,<4.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: qrcode (>=7.4.2,<8.0.0)
 Requires-Dist: tortoise-orm (>=0.19.3,<0.20.0)
 Requires-Dist: ujson (>=5.7.0,<6.0.0)
 Requires-Dist: uvicorn (>=0.21.0,<0.22.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
-    <img src="https://i.328888.xyz/2023/02/28/z23ho.png" alt="TeenStudy.png" border="0" width="500px" height="500px"/>
+    <img src="https://img1.imgtp.com/2023/06/11/sG4KdlpL.png" alt="TeenStudy.png" border="0" width="500px" height="500px"/>
     <h1>TeenStudy</h1>
     <b>基于nonebot2和go-cqhttp的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图</b>
     <br/>
     <a href="https://github.com/ZM25XC/TeenStudy/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/ZM25XC/TeenStudy?style=flat-square"></a>
     <a href="https://github.com/ZM25XC/TeenStudy/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/ZM25XC/TeenStudy?style=flat-square"></a>
     <a href="https://github.com/ZM25XC/TeenStudy/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/ZM25XC/TeenStudy?style=flat-square"></a>
     <a href="https://pypi.python.org/pypi/TeenStudy"><img src="https://img.shields.io/pypi/v/TeenStudy?color=yellow" alt="pypi"></a>
   	<a href="https://pypi.python.org/pypi/TeenStudy">
     <img src="https://img.shields.io/pypi/dm/TeenStudy" alt="pypi download"></a>
 	  <a href="https://github.com/ZM25XC/TeenStudy/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/ZM25XC/TeenStudy?style=flat-square"></a>
     <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS">
-    <img src="https://img.shields.io/badge/QQ%E7%BE%A4-511173803-orange?style=flat-square" alt="QQ Chat Group">
+    <img src="https://img.shields.io/badge/QQ反馈群-511173803-orange?style=flat-square" alt="QQ Chat Group">
+  </a>
+	<a href="http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm">
+    <img src="https://img.shields.io/badge/QQ体验群-821280615-orange?style=flat-square" alt="QQ Chat Group">
   </a>
   </div>
 
 ## 说明
 
 - 本项目为[青年大学习提交](https://github.com/ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`版
 - 本项目基于[nonebot2](https://github.com/nonebot/nonebot2)和[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)，使用本插件前请先阅读以上两个项目的使用文档
 -  **启动插件之后，一定要登录后台在推送列表中添加需要开启大学习功能的群聊**
 -  **本项目无法在国外IP环境下使用，如有开启代理，请关闭或添加代理规则**
 - 需要抓包的地区，绑定后尽量别进官方公众号，避免token或cookie刷新导致无法提交
 - 本项目需要部署在公网可访问的容器中，并开放端口（nonebot2配置的port），否则大部分功能将出现异常
-- 欢迎加入[QQ群](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)，交流讨论。
+- 欢迎加入[QQ反馈群](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)，交流讨论，如您不会搭建又想每周自动提交，可加入[QQ体验群](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm)。
 - 时间精力有限，目前只维护湖北和江西两个地区，其他地区出问题请提交Issues,我找个时间修，需要增加地区请进群帮忙测试，个别地区没账号无法测试
 
 - 觉得项目不错，不妨点个stars.
 
 ## 地区状态
 
 <details>
 
 | 共青团名称 | 开发状态 | 备注 |
 |:-----:|:----:|:----:|
 |青春湖北|支持|无需抓包|
 |江西共青团|支持|无需抓包|
 |安徽共青团|支持|无需抓包|
 |广东共青团|支持|无需抓包|
+|青春北京|支持|无需抓包|
 |青春上海|支持|微信扫码绑定|
 |青春浙江|支持|微信扫码绑定|
-|江苏共青团|支持|需要自行抓包|
+|津彩青春|支持|需要自行抓包|
 |青春山东|支持|需要自行抓包|
 |重庆共青团|支持|需要自行抓包|
 |吉青飞扬|支持|需要自行抓包|
-|黑龙江共青团|支持|需要自行抓包，该地区上线测试中|
 |天府新青年|支持|不进入公众号token时效大于1周|
 |河南共青团|不支持|cookie时效小于1周|
+|江苏共青团|不支持|cookie失效小于1周|
+|黑龙江共青团|不支持|cookie失效小于1周|
 |广西青年圈|待开发||
 |青春湖南|待开发||
 |甘肃青年|待开发||
 |山西青年|待开发||
 |河北共青团|待开发||
 |福建共青团|待开发||
 |内蒙古青年|待开发||
 |云南共青团|待开发||
 |三秦青年|待开发||
-|青春北京|待开发||
 |海南共青团|待开发||
-|津彩青春|待开发||
 |青春黔言|待开发||
 |青春柳州|待开发||
 |辽宁共青团|待开发||
 |宁夏共青团|待开发||
 |新疆共青团|待开发||
 |西藏共青团|待开发||
 </details>
@@ -190,18 +194,36 @@
 
 - [ ] 增加更多地区支持
 - [ ] 优化 Bot
 
 
 ## 更新日志
 
-### 2023/05/21
+### 2023/06/12
+
+- 适配北京地区，无需抓包
+- 增加天津地区，需要自行抓包
+- 因江苏和黑龙江地区Cookie时效小于1周，移除江苏和黑龙江地区
+- Web UI添加日志和主动退出功能
+- 更新江西地区拉取团支部数据方式，移除缓存团支部数据，包体积减小50%
+- 修复大学习公网检测失败问题
+- 更新Nonebot2强制meta字段
+- 同步UI依赖AMIS版本到最新版本
+- 开放体验群，不会搭建又想使用的可加[QQ体验群](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm)
+  
+
+<details>
+
+<summary>2023/05/21</summary>
 
 - 增加黑龙江地区，需要自行抓包，该地区上线测试中，请积极提issue反馈
 - 下版本为大版本更新，将添加新功能，优化功能，请积极提issue反馈或加交流群反馈
+- 
+</details>
+
 
 <details>
 <summary>2023/05/11</summary> 
 
 - 增加广东地区，无需抓包[#13](https://github.com/ZM25XC/TeenStudy/issues/13)，感谢[@neal240](https://github.com/neal240)提供账号测试
 
 </details>
```

#### html2text {}

```diff
@@ -1,64 +1,68 @@
-Metadata-Version: 2.1 Name: teenstudy Version: 0.1.9 Summary:
+Metadata-Version: 2.1 Name: teenstudy Version: 0.2.0 Summary:
 åºäºnonebot2å¼æ­¥æ¡æ¶çéå¹´å¤§å­¦èªå¨æäº¤æä»¶åºäºnonebot2çéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾
 Home-page: https://github.com/ZM25XC/TeenStudy License: MIT Author: ZM25XC
 Author-email: xingling25@qq.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: Jinja2 (>=3.1.2,<4.0.0) Requires-Dist: Pillow (>=9.4.0,<10.0.0)
-Requires-Dist: amis-python (>=1.0.7,<2.0.0) Requires-Dist: anti-useragent
-(>=1.0.10,<2.0.0) Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0) Requires-
-Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist: fastapi (>=0.95.0,<0.96.0) Requires-
-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist: lxml (>=4.9.2,<5.0.0) Requires-
-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0) Requires-Dist: nonebot-plugin-
-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0)
-Requires-Dist: psutil (>=5.9.4,<6.0.0) Requires-Dist: python-jose
-(>=3.3.0,<4.0.0) Requires-Dist: qrcode (>=7.4.2,<8.0.0) Requires-Dist:
-tortoise-orm (>=0.19.3,<0.20.0) Requires-Dist: ujson (>=5.7.0,<6.0.0) Requires-
-Dist: uvicorn (>=0.21.0,<0.22.0) Description-Content-Type: text/markdown
+Requires-Dist: Jinja2 (>=3.1.2,<4.0.0) Requires-Dist: amis-python
+(>=1.0.7,<2.0.0) Requires-Dist: anti-useragent (>=1.0.10,<2.0.0) Requires-Dist:
+beautifulsoup4 (>=4.11.2,<5.0.0) Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-
+Dist: ddddocr (>=1.4.7,<2.0.0) Requires-Dist: fastapi (>=0.95.0,<0.96.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0) Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0) Requires-Dist: nonebot-
+plugin-apscheduler (>=0.3.0,<0.4.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
+Requires-Dist: psutil (>=5.9.4,<6.0.0) Requires-Dist: pycryptodome
+(>=3.17,<4.0) Requires-Dist: python-jose (>=3.3.0,<4.0.0) Requires-Dist: qrcode
+(>=7.4.2,<8.0.0) Requires-Dist: tortoise-orm (>=0.19.3,<0.20.0) Requires-Dist:
+ujson (>=5.7.0,<6.0.0) Requires-Dist: uvicorn (>=0.21.0,<0.22.0) Description-
+Content-Type: text/markdown
                                 [TeenStudy.png]
                             ****** TeenStudy ******
                              åºäºnonebot2ågo-
 cqhttpçéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾
 
  [GitHub_issues] [GitHub_forks] [GitHub_stars] [pypi] [pypi_download] [GitHub
-                           license] [QQ_Chat_Group]
+                   license] [QQ_Chat_Group] [QQ_Chat_Group]
 ## è¯´æ - æ¬é¡¹ç®ä¸º[éå¹´å¤§å­¦ä¹ æäº¤](https://github.com/ZM25XC/
 nonebot_plugin_auto_teenstudy) `Web UI`ç - æ¬é¡¹ç®åºäº[nonebot2](https://
 github.com/nonebot/nonebot2)å[go-cqhttp](https://github.com/Mrs4s/go-
 cqhttp)ï¼ä½¿ç¨æ¬æä»¶åè¯·åéè¯»ä»¥ä¸ä¸¤ä¸ªé¡¹ç®çä½¿ç¨ææ¡£ -
 **å¯å¨æä»¶ä¹åï¼ä¸å®è¦ç»å½åå°å¨æ¨éåè¡¨ä¸­æ·»å éè¦å¼å¯å¤§å­¦ä¹ åè½çç¾¤è**
 -
 **æ¬é¡¹ç®æ æ³å¨å½å¤IPç¯å¢ä¸ä½¿ç¨ï¼å¦æå¼å¯ä»£çï¼è¯·å³é­ææ·»å ä»£çè§å**
 -
 éè¦æåçå°åºï¼ç»å®åå°½éå«è¿å®æ¹å¬ä¼å·ï¼é¿åtokenæcookieå·æ°å¯¼è´æ æ³æäº¤
 -
 æ¬é¡¹ç®éè¦é¨ç½²å¨å¬ç½å¯è®¿é®çå®¹å¨ä¸­ï¼å¹¶å¼æ¾ç«¯å£ï¼nonebot2éç½®çportï¼ï¼å¦åå¤§é¨ååè½å°åºç°å¼å¸¸
-- æ¬¢è¿å å¥[QQç¾¤](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)ï¼äº¤æµè®¨è®ºã
--
+- æ¬¢è¿å å¥[QQåé¦ç¾¤](https://jq.qq.com/
+?_wv=1027&k=NGFEwXyS)ï¼äº¤æµè®¨è®ºï¼å¦æ¨ä¸ä¼æ­å»ºåæ³æ¯å¨èªå¨æäº¤ï¼å¯å å¥
+[QQä½éªç¾¤](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-
+ai2aPGToBKm)ã -
 æ¶é´ç²¾åæéï¼ç®ååªç»´æ¤æ¹ååæ±è¥¿ä¸¤ä¸ªå°åºï¼å¶ä»å°åºåºé®é¢è¯·æäº¤Issues,ææ¾ä¸ªæ¶é´ä¿®ï¼éè¦å¢å å°åºè¯·è¿ç¾¤å¸®å¿æµè¯ï¼ä¸ªå«å°åºæ²¡è´¦å·æ æ³æµè¯
 - è§å¾é¡¹ç®ä¸éï¼ä¸å¦¨ç¹ä¸ªstars. ## å°åºç¶æ  | å±éå¢åç§° |
 å¼åç¶æ | å¤æ³¨ | |:-----:|:----:|:----:
 | |éæ¥æ¹å|æ¯æ|æ éæå| |æ±è¥¿å±éå¢|æ¯æ|æ éæå|
 |å®å¾½å±éå¢|æ¯æ|æ éæå| |å¹¿ä¸å±éå¢|æ¯æ|æ éæå|
-|éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
+|éæ¥åäº¬|æ¯æ|æ éæå| |éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
 |éæ¥æµæ±|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
-|æ±èå±éå¢|æ¯æ|éè¦èªè¡æå|
+|æ´¥å½©éæ¥|æ¯æ|éè¦èªè¡æå|
 |éæ¥å±±ä¸|æ¯æ|éè¦èªè¡æå|
 |éåºå±éå¢|æ¯æ|éè¦èªè¡æå|
 |åéé£æ¬|æ¯æ|éè¦èªè¡æå|
-|é»é¾æ±å±éå¢|æ¯æ|éè¦èªè¡æåï¼è¯¥å°åºä¸çº¿æµè¯ä¸­|
 |å¤©åºæ°éå¹´|æ¯æ|ä¸è¿å¥å¬ä¼å·tokenæ¶æå¤§äº1å¨|
-|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨| |å¹¿è¥¿éå¹´å|å¾å¼å||
-|éæ¥æ¹å|å¾å¼å|| |çèéå¹´|å¾å¼å|| |å±±è¥¿éå¹´|å¾å¼å||
+|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨|
+|æ±èå±éå¢|ä¸æ¯æ|cookieå¤±æå°äº1å¨|
+|é»é¾æ±å±éå¢|ä¸æ¯æ|cookieå¤±æå°äº1å¨|
+|å¹¿è¥¿éå¹´å|å¾å¼å|| |éæ¥æ¹å|å¾å¼å||
+|çèéå¹´|å¾å¼å|| |å±±è¥¿éå¹´|å¾å¼å||
 |æ²³åå±éå¢|å¾å¼å|| |ç¦å»ºå±éå¢|å¾å¼å||
 |åèå¤éå¹´|å¾å¼å|| |äºåå±éå¢|å¾å¼å||
-|ä¸ç§¦éå¹´|å¾å¼å|| |éæ¥åäº¬|å¾å¼å||
-|æµ·åå±éå¢|å¾å¼å|| |æ´¥å½©éæ¥|å¾å¼å||
+|ä¸ç§¦éå¹´|å¾å¼å|| |æµ·åå±éå¢|å¾å¼å||
 |éæ¥é»è¨|å¾å¼å|| |éæ¥æ³å·|å¾å¼å||
 |è¾½å®å±éå¢|å¾å¼å|| |å®å¤å±éå¢|å¾å¼å||
 |æ°çå±éå¢|å¾å¼å|| |è¥¿èå±éå¢|å¾å¼å||  ## å®è£åæ´æ°
 ç¬¬ä¸ç§æ¹å¼(ä¸æ¨è) - ä½¿ç¨`git clone https://github.com/ZM25XC/
 TeenStudy.git`æä»¤åéæ¬ä»åºæä¸è½½åç¼©åæä»¶   ç¬¬äºç§æ¹å¼
 (äºéä¸) - ä½¿ç¨`pip install TeenStudy`æ¥è¿è¡å®è£,ä½¿ç¨`pip install
 TeenStudy -U`è¿è¡æ´æ° - ä½¿ç¨`nb plugin install
@@ -94,20 +98,29 @@
 UIé»è®¤éç½® | | éç½®å¯ç  | éç½®å¯ç  | éç½®ç»å½Web
 UIçå¯ç ä¸ºç¨æ·ID |
 |å é¤å¤§å­¦ä¹ |å é¤å¤§å­¦ä¹ |ç¨æ·ç³è¯·æ¸é¤æ°æ®åºçä¿¡æ¯|
 |å¯¼åºç¨æ·æ°æ®|å¯¼åºç¨æ·æ°æ®ãå¯¼åºæ°æ®|å°æ°æ®å¯¼åºè³TeenStudyç®å½ä¸|
 |æ´æ°ç¨æ·æ°æ®|æ´æ°ç¨æ·æ°æ®ãå·æ°ç¨æ·æ°æ®|å°ç¨æ·æ°æ®å¯¼å¥å°æ°æ®åº|
 |æ´æ°èµæºæ°æ®|æ´æ°èµæºæ°æ®ãå·æ°èµæºæ°æ®|æ´æ°æ°æ®åºä¸­çèµæºæ°æ®ï¼æ±è¥¿å±éå¢å¢æ¯é¨æ°æ®ï¼|
 ## ToDo - [ ] å¢å æ´å¤å°åºæ¯æ - [ ] ä¼å Bot ## æ´æ°æ¥å¿ ###
-2023/05/21 -
+2023/06/12 - ééåäº¬å°åºï¼æ éæå -
+å¢å å¤©æ´¥å°åºï¼éè¦èªè¡æå -
+å æ±èåé»é¾æ±å°åºCookieæ¶æå°äº1å¨ï¼ç§»é¤æ±èåé»é¾æ±å°åº
+- Web UIæ·»å æ¥å¿åä¸»å¨éåºåè½ -
+æ´æ°æ±è¥¿å°åºæåå¢æ¯é¨æ°æ®æ¹å¼ï¼ç§»é¤ç¼å­å¢æ¯é¨æ°æ®ï¼åä½ç§¯åå°50%
+- ä¿®å¤å¤§å­¦ä¹ å¬ç½æ£æµå¤±è´¥é®é¢ - æ´æ°Nonebot2å¼ºå¶metaå­æ®µ -
+åæ­¥UIä¾èµAMISçæ¬å°ææ°çæ¬ -
+å¼æ¾ä½éªç¾¤ï¼ä¸ä¼æ­å»ºåæ³ä½¿ç¨çå¯å [QQä½éªç¾¤](http://
+qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=2PQucjirnkHyPjoS1Pkr-ai2aPGToBKm)  2023/05/
+21 -
 å¢å é»é¾æ±å°åºï¼éè¦èªè¡æåï¼è¯¥å°åºä¸çº¿æµè¯ä¸­ï¼è¯·ç§¯ææissueåé¦
 -
 ä¸çæ¬ä¸ºå¤§çæ¬æ´æ°ï¼å°æ·»å æ°åè½ï¼ä¼ååè½ï¼è¯·ç§¯ææissueåé¦æå äº¤æµç¾¤åé¦
-2023/05/11 - å¢å å¹¿ä¸å°åºï¼æ éæå[#13](https://github.com/ZM25XC/
-TeenStudy/issues/13)ï¼æè°¢[@neal240](https://github.com/
+-   2023/05/11 - å¢å å¹¿ä¸å°åºï¼æ éæå[#13](https://github.com/
+ZM25XC/TeenStudy/issues/13)ï¼æè°¢[@neal240](https://github.com/
 neal240)æä¾è´¦å·æµè¯   2023/05/06 -
 å¢å åæå°åºï¼éè¦èªè¡æå -
 ä¿®å¤è¶ç®¡æ´æ¹ç»å½å¯ç åç¨åå¯ç è½ç»§ç»­ç»å½é®é¢ -
 æ·»å äºç»´ç è½¬é¾æ¥å¼å³ï¼éè¦èªè¡å¨åå°éç½®é¡µé¢æå¼ -
 è°æ´é¨åä¾èµ    2023/04/12 -
 å æ²³åå°åºcookieæ¶æå°äº1å¨ï¼ç§»é¤æ²³åå°åº -
 æ·»å `å é¤å¤§å­¦ä¹ `åè½ï¼ç¨æ·å¯èªè¡å é¤æ°æ® -
```

