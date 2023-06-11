# Comparing `tmp/hoyo-daily-logins-helper-2.5.1.tar.gz` & `tmp/hoyo-daily-logins-helper-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoyo-daily-logins-helper-2.5.1.tar", last modified: Wed May 31 08:31:04 2023, max compression
+gzip compressed data, was "hoyo-daily-logins-helper-2.5.2.tar", last modified: Sun Jun 11 03:59:18 2023, max compression
```

## Comparing `hoyo-daily-logins-helper-2.5.1.tar` & `hoyo-daily-logins-helper-2.5.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:04.110168 hoyo-daily-logins-helper-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:04.106167 hoyo-daily-logins-helper-2.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:04.106167 hoyo-daily-logins-helper-2.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-31 08:31:04.110168 hoyo-daily-logins-helper-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/hoyo-daily-logins-helper.toml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:04.106167 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 08:31:04.000000 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper/games.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:04.106167 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-31 08:31:04.000000 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-31 08:31:04.000000 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:31:04.000000 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-31 08:31:04.000000 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 08:31:04.000000 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-31 08:31:04.000000 hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 08:31:04.110168 hoyo-daily-logins-helper-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 08:30:41.000000 hoyo-daily-logins-helper-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:18.914649 hoyo-daily-logins-helper-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:18.910649 hoyo-daily-logins-helper-2.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:18.914649 hoyo-daily-logins-helper-2.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-11 03:59:18.914649 hoyo-daily-logins-helper-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo-daily-logins-helper.toml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:18.914649 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 03:59:18.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/games.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:59:18.914649 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-11 03:59:18.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-11 03:59:18.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 03:59:18.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-11 03:59:18.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-11 03:59:18.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-11 03:59:18.000000 hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 03:59:18.914649 hoyo-daily-logins-helper-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 03:59:00.000000 hoyo-daily-logins-helper-2.5.2/setup.py
```

### Comparing `hoyo-daily-logins-helper-2.5.1/.github/workflows/deploy.yml` & `hoyo-daily-logins-helper-2.5.2/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.1/.github/workflows/tests.yml` & `hoyo-daily-logins-helper-2.5.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.1/.gitignore` & `hoyo-daily-logins-helper-2.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.1/LICENSE` & `hoyo-daily-logins-helper-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.1/PKG-INFO` & `hoyo-daily-logins-helper-2.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.5.1
+Version: 2.5.2
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -115,15 +115,19 @@
 
 Content:
 
 ```toml
 # you can configurate some things here like the language or the user agent
 # keep in mind that config and every key in there is optional and you can omit it
 [config]
+# i'd recommend against changing this value unless you know what you are doing
+# not setting this will make it look to the developer like we are using a normal
+# web browser while this is very suspicious
 user-agent = "My fancy user agent"
+# the language of the rewards and presumably return messages from the API
 language = "en-us"
 
 # every account starts with this index/key 
 [[accounts]]
 # accounts can have identifiers for you to differentiate them in the logs
 # you could for instance add your account name or UID here
 identifier = "My Genshin Account Name"
@@ -164,14 +168,17 @@
 
 ```toml
 [config]
 # ...
 notifications = [
     {type = "discord", webhook_url = "https://...."}
 ]
+
+[[accounts]]
+# ....
 ```
 
 ## License
 
 GNU General Public License v3
 
 ![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

### Comparing `hoyo-daily-logins-helper-2.5.1/README.md` & `hoyo-daily-logins-helper-2.5.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -104,15 +104,19 @@
 
 Content:
 
 ```toml
 # you can configurate some things here like the language or the user agent
 # keep in mind that config and every key in there is optional and you can omit it
 [config]
+# i'd recommend against changing this value unless you know what you are doing
+# not setting this will make it look to the developer like we are using a normal
+# web browser while this is very suspicious
 user-agent = "My fancy user agent"
+# the language of the rewards and presumably return messages from the API
 language = "en-us"
 
 # every account starts with this index/key 
 [[accounts]]
 # accounts can have identifiers for you to differentiate them in the logs
 # you could for instance add your account name or UID here
 identifier = "My Genshin Account Name"
@@ -153,14 +157,17 @@
 
 ```toml
 [config]
 # ...
 notifications = [
     {type = "discord", webhook_url = "https://...."}
 ]
+
+[[accounts]]
+# ....
 ```
 
 ## License
 
 GNU General Public License v3
 
 ![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

### Comparing `hoyo-daily-logins-helper-2.5.1/hoyo-daily-logins-helper.toml.template` & `hoyo-daily-logins-helper-2.5.2/hoyo-daily-logins-helper.toml.template`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper/games.py` & `hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/games.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,74 @@
 import json
 import logging
 import random
 import time
-from typing import Optional
 
 from hoyo_daily_logins_helper.http import http_get_json, http_post_json
-from hoyo_daily_logins_helper.notifications import NotificationManager, \
-    Notification
+from hoyo_daily_logins_helper.notifications import Notification, NotificationManager
 
 RET_CODE_ALREADY_SIGNED_IN = -5003
 
 GAMES = {
     "genshin": {
         "name": "Genshin Impact",
         "event_base_url": "https://hk4e-api-os.mihoyo.com/event/sol",
         "act_id": "e202102251931481",
+        "login_url": "https://act.hoyolab.com/ys/event/signin-sea-v3/index.html"
+                     "?act_id=e202102251931481",
     },
     "starrail": {
         "name": "Honkai: Star Rail",
         "event_base_url": "https://sg-public-api.hoyolab.com/event/luna/os",
         "act_id": "e202303301540311",
+        "login_url": "https://act.hoyolab.com/bbs/event/signin/hkrpg/index.html"
+                     "?act_id=e202303301540311",
     },
     "honkai": {
         "name": "Honkai Impact 3rd",
         "event_base_url": "https://sg-public-api.hoyolab.com/event/mani",
         "act_id": "e202110291205111",
+        "login_url": "https://act.hoyolab.com/bbs/event/signin-bh3/index.html"
+                     "?act_id=e202110291205111",
     },
     "themis": {
         "name": "Tears of Themis",
         "event_base_url": "https://sg-public-api.hoyolab.com/event/luna/os",
         "act_id": "e202202281857121",
-    }
+        "login_url": "https://act.hoyolab.com/bbs/event/signin/nxx/index.html"
+                     "?act_id=e202202281857121",
+    },
 }
+_CAPTCHA_MESSAGE = """Captcha is required, please sign into the website: %s"""
 
 
 def game_perform_checkin(
         account_ident: str,
         game: str,
         cookie_str: str,
         language: str,
-        notification_manager: Optional[NotificationManager],
+        notification_manager: NotificationManager | None,
         skip_checkin: bool = False,
 ):
     if game not in GAMES:
-        raise Exception(f"unknown game identifier found: {game}")
+        msg = f"unknown game identifier found: {game}"
+        raise Exception(msg)
 
     game_name = GAMES[game]["name"]
     event_base_url = GAMES[game]["event_base_url"]
     act_id = GAMES[game]["act_id"]
+    login_url = GAMES[game]["login_url"]
 
     referer_url = "https://act.hoyolab.com/"
-    reward_url = f"{event_base_url}/home?lang={language}" \
-                 f"&act_id={act_id}"
-    info_url = f"{event_base_url}/info?lang={language}" \
-               f"&act_id={act_id}"
+    reward_url = (
+        f"{event_base_url}/home?lang={language}&act_id={act_id}"
+    )
+    info_url = (
+        f"{event_base_url}/info?lang={language}&act_id={act_id}"
+    )
     sign_url = f"{event_base_url}/sign?lang={language}"
 
     headers = {
         "Referer": referer_url,
         "Accept-Encoding": "gzip, deflate, br",
         "Cookie": cookie_str,
     }
@@ -100,29 +111,42 @@
     }, ensure_ascii=False)
 
     if not skip_checkin:
         response = http_post_json(sign_url, headers=headers, data=request_data)
     else:
         response = {
             "retcode": 0,
-            "message": "Test Run, skipped actual checkin request"
+            "message": "Test Run, skipped actual checkin request",
         }
 
     # as we logged in for a day, the number of total sign ins has to increase
     total_sign_in_day += 1
 
     code = response.get("retcode", 99999)
 
     logging.debug(f"return code {code}")
 
     if code == RET_CODE_ALREADY_SIGNED_IN:
         logging.info("Already signed in for today...")
         return
-    elif code != 0:
-        logging.error(response['message'])
+
+    if is_captcha_required(response):
+        msg = _CAPTCHA_MESSAGE % login_url
+        logging.error(msg)
+        if notification_manager:
+            notification_manager.send(Notification(
+                success=False,
+                account_identifier=account_ident,
+                game_name=game_name,
+                message=msg,
+            ))
+        return
+
+    if code != 0:
+        logging.error(response["message"])
         if notification_manager:
             notification_manager.send(Notification(
                 success=False,
                 account_identifier=account_ident,
                 game_name=game_name,
                 message=response["message"],
             ))
@@ -140,15 +164,28 @@
             success=True,
             account_identifier=account_ident,
             game_name=game_name,
             message=response["message"],
             custom_fields=[
                 {
                     "key": "Total Sign-in days",
-                    "value": total_sign_in_day
+                    "value": total_sign_in_day,
                 },
                 {
                     "key": "Rewards",
                     "value": f"{reward['cnt']}x {reward['name']}",
                 },
             ],
         ))
+
+
+def is_captcha_required(response: dict) -> bool:
+    if "gt_result" not in response:
+        return False
+
+    gt = response["gt_result"]["gt"]
+    challenge = response["gt_result"]["challenge"]
+
+    if not gt and not challenge:
+        return False
+
+    return True
```

### Comparing `hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper/http.py` & `hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/http.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 import json
 import logging
-from typing import Dict
 
 import requests
 from requests import HTTPError, Response
 
 from hoyo_daily_logins_helper.utils import dict_prettify
 
-USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) " \
-             "AppleWebKit/537.36 (KHTML, like Gecko) " \
-             "Chrome/74.0.3729.169 Safari/537.36"
+USER_AGENT = (
+    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) "
+    "AppleWebKit/537.36 (KHTML, like Gecko) "
+    "Chrome/74.0.3729.169 Safari/537.36"
+)
 _http_req_settings = {"user_agent": USER_AGENT}
 
 
 def http_set_user_agent(user_agent: str):
     _http_req_settings["user_agent"] = user_agent
 
 
 def http_get(url: str, max_retries: int = 2, **kwargs) -> Response:
     return http_request("get", url, max_retries, **kwargs)
 
 
-def http_get_json(url: str, max_retries: int = 2, **kwargs) -> Dict[str, any]:
+def http_get_json(url: str, max_retries: int = 2, **kwargs) -> dict[str, any]:
     resp = http_get(url, max_retries, **kwargs)
     data = resp.text
     return json.loads(data)
 
 
 def http_post(url: str, max_retries: int = 2, **kwargs) -> Response:
     return http_request("post", url, max_retries, **kwargs)
 
 
-def http_post_json(url: str, max_retries: int = 2, **kwargs) -> Dict[str, any]:
+def http_post_json(url: str, max_retries: int = 2, **kwargs) -> dict[str, any]:
     resp = http_post(url, max_retries, **kwargs)
     data = resp.text
     return json.loads(data)
 
 
 def http_request(
         method: str,
         url: str,
         max_retries: int = 2,
-        **kwargs
+        **kwargs,
 ) -> Response:
     for i in range(max_retries + 1):
         try:
             logging.debug(f"{method.upper()} {url}, REQ: {i + 1}/{max_retries}")
             session = requests.Session()
             session.headers["User-Agent"] = _http_req_settings["user_agent"]
             resp = session.request(method, url, **kwargs)
@@ -54,12 +55,11 @@
             if resp.headers.get("Content-Type", "") == "application/json":
                 text = dict_prettify(json.loads(text))
             logging.debug(f"Response: {resp.status_code}\n\n{text}\n")
         except HTTPError as e:
             logging.error(f"HTTP error: {e}, REQ: {i + 1}/{max_retries}")
         except KeyError as e:
             logging.error(f"Wrong response: {e}, REQ: {i + 1}/{max_retries}")
-        except Exception as e:
-            logging.error(f"Unknown error: {e}, REQ: {i + 1}/{max_retries}")
         else:
             return resp
-    raise Exception(f"All {max_retries} HTTP requests have failed")
+    msg = f"All {max_retries} HTTP requests have failed"
+    raise Exception(msg)
```

### Comparing `hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper/main.py` & `hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 import os
 import sys
 import tomllib
 from pathlib import Path
-from typing import Optional
 
 import comboparse
 
 from hoyo_daily_logins_helper._version import __version__
 from hoyo_daily_logins_helper.consts import DEFAULT_LANGUAGE
 from hoyo_daily_logins_helper.games import GAMES, game_perform_checkin
 from hoyo_daily_logins_helper.http import http_set_user_agent
@@ -38,15 +37,15 @@
         has_config_file = True
 
     if default_file.exists():
         has_config_file = True
         cli_args.append("--config-file")
         cli_args.append(default_file.absolute().__str__())
 
-    for game in GAMES.keys():
+    for game in GAMES:
         if f"--{game}" in cli_args:
             has_single_game_flag = True
 
     # legacy GAME env var
     if "GAME" in os.environ:
         has_single_game_flag = True
     if "COOKIE" in os.environ:
@@ -66,15 +65,15 @@
         help="the game(s) for which this tool is supposed to run",
         action="append",
         choices=GAMES.keys(),
         required=not has_config_file and not has_single_game_flag,
         default=[],
     )
 
-    for game in GAMES.keys():
+    for game in GAMES:
         game_name = GAMES[game]["name"]
         parser.add_argument(
             f"--{game}",
             help=f"run for game {game_name}",
             action="store_const",
             dest="overwrite_game",
             const=game,
@@ -117,15 +116,15 @@
     )
 
     args = parser.parse_args(cli_args)
 
     logging.basicConfig(
         level=logging.DEBUG if args.debug else logging.INFO,
         format="[%(asctime)s][%(levelname)s]: %(message)s",
-        datefmt="%Y-%m-%dT%H:%M:%S"
+        datefmt="%Y-%m-%dT%H:%M:%S",
     )
 
     logging.info(f"Hoyo Daily Logins Helper - v{__version__}")
     logging.info("If this tool fails, try to update your cookie!")
     logging.debug(f"Arguments: {args}")
 
     if args.overwrite_game:
@@ -139,20 +138,20 @@
         if "COOKIE" in os.environ:
             args.cookie = [os.environ["COOKIE"]]
         if "GAME" in os.environ:
             args.game = [os.environ["GAME"]]
 
     enable_scheduler = False
     account_identifiers = [None for _ in args.game]
-    notification_manager: Optional[NotificationManager] = None
+    notification_manager: NotificationManager | None = None
 
     if args.config_file:
         logging.info(f"Found config file at: {args.config_file}")
 
-        with open(args.config_file, "rb") as file:
+        with Path.open(args.config_file, "rb") as file:
             config_data = tomllib.load(file)
             logging.debug(dict_prettify(config_data))
 
             # parse config from toml file
             language = config_data.get("config", {}).get("language", None)
 
             if language:
@@ -178,32 +177,32 @@
 
                 if not game:
                     logging.error(f"account #{index} has no game selected")
                     continue
 
                 if game not in GAMES:
                     logging.error(
-                        f"account #{index} has invalid game '{game}' set"
+                        f"account #{index} has invalid game '{game}' set",
                     )
                     continue
 
                 if not cookie:
                     logging.error(f"account #{index} has no cookie set")
                     continue
 
                 account_identifiers.append(account.get("identifier", None))
                 args.game.append(game)
                 args.cookie.append(cookie)
 
     if len(args.cookie) != len(args.game):
         logging.error(
             f"number of cookies ({len(args.cookie)}) and "
-            f"games ({len(args.game)}) does not match"
+            f"games ({len(args.game)}) does not match",
         )
-        exit(1)
+        sys.exit(1)
 
     if args.user_agent:
         http_set_user_agent(args.user_agent)
 
     if enable_scheduler:
         run_scheduler(config_data, args.language, notification_manager)
         return
@@ -217,16 +216,13 @@
 
         game_perform_checkin(
             identifier,
             game,
             cookie,
             args.language,
             notification_manager,
-            skip_checkin=args.skip_checkin
+            skip_checkin=args.skip_checkin,
         )
 
 
 def has_legacy_environment_variable() -> bool:
-    for env_var in ["LANGUAGE", "COOKIE", "GAME"]:
-        if env_var in os.environ:
-            return True
-    return False
+    return any(env_var in os.environ for env_var in ["LANGUAGE", "COOKIE", "GAME"])
```

### Comparing `hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper/notifications.py` & `hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/notifications.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 import json
 import logging
 from dataclasses import dataclass
-from datetime import datetime
-from typing import List
+from datetime import UTC, datetime
 
 from hoyo_daily_logins_helper.http import http_post
+from hoyo_daily_logins_helper.utils import dict_prettify
 
 
 @dataclass
 class Notification:
     success: bool
     game_name: str
     account_identifier: str
     message: str
-    custom_fields: List[dict] = ()
+    custom_fields: list[dict] = ()
 
 
 @dataclass
 class _NotificationHandler:
     pass
 
     @staticmethod
     def create(data: dict):
-        raise NotImplementedError()
+        raise NotImplementedError
 
     def send(self, notification: Notification):
-        raise NotImplementedError()
+        raise NotImplementedError
 
 
 @dataclass
 class _DiscordNotificationHandler(_NotificationHandler):
     webhook_url: str
 
     @staticmethod
     def create(data: dict):
         if "webhook_url" not in data:
-            raise Exception("No webhook_url defined in Discord notifications")
+            msg = "No webhook_url defined in Discord notifications"
+            raise Exception(msg)
         return _DiscordNotificationHandler(data["webhook_url"])
 
     def send(self, notification: Notification):
         color_success = 4431943
         color_failure = 15022389
 
         fields = [
@@ -56,14 +57,16 @@
         for custom_field in notification.custom_fields:
             fields.append({
                 "name": custom_field["key"],
                 "value": custom_field["value"],
                 "inline": False,
             })
 
+        tz = datetime.now(UTC).astimezone().tzinfo
+
         data = json.dumps({
             "content": "",
             "embeds": [
                 {
                     "author": {
                         "name": "atomicptr/hoyo-daily-logins-helper",
                         "url": "https://github.com/atomicptr/hoyo-daily-logins-helper",
@@ -71,39 +74,39 @@
                     "color": color_success if notification.success else color_failure,
                     "title": "Hoyo Daily Logins Helper",
                     "description": notification.message,
                     "fields": fields,
                     "thumbnail": {
                         "url": "https://i.imgur.com/LiWb3EG.png",
                     },
-                    "timestamp": datetime.now().isoformat(),
-                }
-            ]
+                    "timestamp": datetime.now(tz=tz).isoformat(),
+                },
+            ],
         }, ensure_ascii=False)
 
         http_post(self.webhook_url, data=data, headers={
             "Content-Type": "application/json",
         })
 
 
 class NotificationManager:
-    _handler: List[_NotificationHandler] = []
+    _handler: list[_NotificationHandler] = []
 
-    def __init__(self, notifications: List[dict]):
+    def __init__(self, notifications: list[dict]) -> None:
         for notification in notifications:
             if "type" not in notification:
                 logging.error(
-                    "Notification entry without type found",
-                    notification
+                    "Notification entry without type found:"
+                    f"\n{dict_prettify(notification)}",
                 )
                 continue
             match notification["type"]:
                 case "discord":
                     self._handler.append(
-                        _DiscordNotificationHandler.create(notification)
+                        _DiscordNotificationHandler.create(notification),
                     )
                 case other_type:
                     logging.error(f"Unknown notification type {other_type}")
                     continue
 
     def send(self, notification: Notification):
         logging.debug(notification)
```

### Comparing `hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper/scheduler.py` & `hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper/scheduler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import logging
-from datetime import datetime, timezone, time, timedelta
+import sys
+from datetime import UTC, datetime, time, timedelta
 from time import sleep
-from typing import Optional
 
 import pytz
 from scheduler import Scheduler
 
-from hoyo_daily_logins_helper.games import game_perform_checkin, GAMES
+from hoyo_daily_logins_helper.games import GAMES, game_perform_checkin
 from hoyo_daily_logins_helper.notifications import NotificationManager
 
 _RESET_TIME = time(tzinfo=pytz.timezone("Asia/Shanghai"), hour=0, minute=5)
 
 
 def run_scheduler(
         config_data: dict,
         language: str,
-        notifications_manager: Optional[NotificationManager]
+        notifications_manager: NotificationManager | None,
 ):
     logging.info("Run in scheduler mode")
 
-    tz = datetime.now(timezone.utc).astimezone().tzinfo
+    tz = datetime.now(UTC).astimezone().tzinfo
 
     schedule = Scheduler(tzinfo=tz)
 
     accounts = config_data.get("accounts", [])
 
     for index, account in enumerate(accounts):
         identifier = account.get("identifier", None)
@@ -38,29 +38,29 @@
             _RESET_TIME,
             create_checkin_job(
                 identifier,
                 game,
                 account.get("cookie"),
                 language,
                 notifications_manager,
-            )
+            ),
         )
 
         logging.info(
-            f"Added {game_name} account '{identifier}' to scheduler"
+            f"Added {game_name} account '{identifier}' to scheduler",
         )
 
     if len(schedule.jobs) == 0:
         logging.error("No jobs scheduled")
-        exit(1)
+        sys.exit(1)
 
     print_time_till_next_reset()
     schedule.hourly(
         time(minute=0, second=0, tzinfo=tz),
-        print_time_till_next_reset
+        print_time_till_next_reset,
     )
 
     logging.debug("Job schedule:")
     logging.debug(schedule)
 
     while True:
         schedule.exec_jobs()
@@ -68,31 +68,31 @@
 
 
 def create_checkin_job(
         account_ident: str,
         game: str,
         cookie_str: str,
         language: str,
-        notification_manager: Optional[NotificationManager]
+        notification_manager: NotificationManager | None,
 ):
     def _checkin_job():
         logging.info(f"Running scheduler for '{account_ident}'...")
         game_perform_checkin(
             account_ident,
             game,
             cookie_str,
             language,
-            notification_manager
+            notification_manager,
         )
 
     return _checkin_job
 
 
 def print_time_till_next_reset():
-    tz = datetime.now(timezone.utc).astimezone().tzinfo
+    tz = datetime.now(UTC).astimezone().tzinfo
     now = datetime.now(tz=tz)
     next_reset = datetime.now(tz=_RESET_TIME.tzinfo)
     next_reset = next_reset.replace(
         hour=_RESET_TIME.hour,
         minute=_RESET_TIME.minute,
         second=0,
     )
@@ -100,8 +100,8 @@
     if next_reset < now:
         next_reset = next_reset + timedelta(days=1)
 
     diff = next_reset - now
 
     hours = round(diff.total_seconds() / 60 / 60, 1)
 
-    logging.info(f"Next reset time is in {hours} hours.")
+    logging.info(f"Next reset time is in {hours} hours.")
```

### Comparing `hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper.egg-info/PKG-INFO` & `hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.5.1
+Version: 2.5.2
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -115,15 +115,19 @@
 
 Content:
 
 ```toml
 # you can configurate some things here like the language or the user agent
 # keep in mind that config and every key in there is optional and you can omit it
 [config]
+# i'd recommend against changing this value unless you know what you are doing
+# not setting this will make it look to the developer like we are using a normal
+# web browser while this is very suspicious
 user-agent = "My fancy user agent"
+# the language of the rewards and presumably return messages from the API
 language = "en-us"
 
 # every account starts with this index/key 
 [[accounts]]
 # accounts can have identifiers for you to differentiate them in the logs
 # you could for instance add your account name or UID here
 identifier = "My Genshin Account Name"
@@ -164,14 +168,17 @@
 
 ```toml
 [config]
 # ...
 notifications = [
     {type = "discord", webhook_url = "https://...."}
 ]
+
+[[accounts]]
+# ....
 ```
 
 ## License
 
 GNU General Public License v3
 
 ![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

### Comparing `hoyo-daily-logins-helper-2.5.1/hoyo_daily_logins_helper.egg-info/SOURCES.txt` & `hoyo-daily-logins-helper-2.5.2/hoyo_daily_logins_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.5.1/requirements.txt` & `hoyo-daily-logins-helper-2.5.2/requirements.txt`

 * *Files identical despite different names*

