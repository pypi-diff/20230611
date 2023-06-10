# Comparing `tmp/nextguild-1.2.2.tar.gz` & `tmp/nextguild-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextguild-1.2.2.tar", last modified: Sat Jun 10 22:31:43 2023, max compression
+gzip compressed data, was "nextguild-1.2.3.tar", last modified: Sat Jun 10 22:58:01 2023, max compression
```

## Comparing `nextguild-1.2.2.tar` & `nextguild-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:31:43.986807 nextguild-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 22:31:28.000000 nextguild-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-10 22:31:43.986807 nextguild-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-10 22:31:28.000000 nextguild-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:31:43.982807 nextguild-1.2.2/nextguild/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-10 22:31:28.000000 nextguild-1.2.2/nextguild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26735 2023-06-10 22:31:28.000000 nextguild-1.2.2/nextguild/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    41054 2023-06-10 22:31:28.000000 nextguild-1.2.2/nextguild/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-10 22:31:28.000000 nextguild-1.2.2/nextguild/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    48069 2023-06-10 22:31:28.000000 nextguild-1.2.2/nextguild/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:31:43.986807 nextguild-1.2.2/nextguild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-10 22:31:43.000000 nextguild-1.2.2/nextguild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-10 22:31:43.000000 nextguild-1.2.2/nextguild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 22:31:43.000000 nextguild-1.2.2/nextguild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-10 22:31:43.000000 nextguild-1.2.2/nextguild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-10 22:31:28.000000 nextguild-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 22:31:43.986807 nextguild-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:58:01.720759 nextguild-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 22:57:51.000000 nextguild-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-10 22:58:01.720759 nextguild-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-10 22:57:51.000000 nextguild-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:58:01.720759 nextguild-1.2.3/nextguild/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-10 22:57:51.000000 nextguild-1.2.3/nextguild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26747 2023-06-10 22:57:51.000000 nextguild-1.2.3/nextguild/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41054 2023-06-10 22:57:51.000000 nextguild-1.2.3/nextguild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-10 22:57:51.000000 nextguild-1.2.3/nextguild/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48059 2023-06-10 22:57:51.000000 nextguild-1.2.3/nextguild/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:58:01.720759 nextguild-1.2.3/nextguild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-10 22:58:01.000000 nextguild-1.2.3/nextguild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-10 22:58:01.000000 nextguild-1.2.3/nextguild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 22:58:01.000000 nextguild-1.2.3/nextguild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-10 22:58:01.000000 nextguild-1.2.3/nextguild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-10 22:57:51.000000 nextguild-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 22:58:01.720759 nextguild-1.2.3/setup.cfg
```

### Comparing `nextguild-1.2.2/LICENSE` & `nextguild-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.2/PKG-INFO` & `nextguild-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.2.2
+Version: 1.2.3
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.2.2/README.md` & `nextguild-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.2/nextguild/classes.py` & `nextguild-1.2.3/nextguild/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                     data = self._get_webhook_id(event_data)
                 return data
         return 'None'
     
     def _get_id(self, event_data: dict):
         scenarios = [
             ('serverMemberBan', 'user', 'id'),
-            ('id'),
+            ('id',),
             ('message', 'id'),
             ('member', 'user', 'id'),
             ('userId'),
             ('userInfo', 'id'),
             ('channel', 'id'),
             ('webhook', 'id'),
             ('docs', 'id'),
@@ -144,21 +144,21 @@
             ('socialLink', 'userId'),
             ('calendarEventRsvp', 'userId'),
         ]
         return self._scenario(event_data, scenarios)
 
     def _get_server_id(self, event_data: dict):
         scenarios = [
-            ('serverId'),
+            ('reaction', 'serverId'),
+            ('serverId',),
             ('server', 'id'),
             ('message', 'serverId'),
             ('webhook', 'serverId'),
             ('doc', 'serverId'),
             ('calendarEvent', 'serverId'),
-            ('reaction', 'serverId')
         ]
         return self._scenario(event_data, scenarios)
             
     def _get_group_id(self, event_data: dict):
         scenarios = [
             ('group', 'id'),
             ('message', 'groupId'),
@@ -183,15 +183,15 @@
             ('announcement', 'channelId'),
             ('announcementComment', 'channelId'),
         ]
         return self._scenario(event_data, scenarios)
 
     def _get_created_by(self, event_data: dict):
         scenarios = [
-            ('createdBy'),
+            ('createdBy',),
             ('message', 'createdBy'),
             ('serverMemberBan', 'createdBy'),
             ('channel', 'createdBy'),
             ('webhook', 'createdBy'),
             ('doc', 'createdBy'),
             ('docComment', 'createdBy'),
             ('calendarEvent', 'createdBy'),
@@ -206,15 +206,15 @@
             ('announcement', 'createdBy'),
             ('announcementComment', 'createdBy'),
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_deleted_by(self, event_data: dict):
         scenarios = [
-            ('deletedBy'),
+            ('deletedBy',),
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_owner_id(self, event_data: dict):
         scenarios = [
             ('server', 'ownerId'),
         ]
@@ -531,21 +531,21 @@
         scenarios = [
             ('calendarEvent', 'cancellation'),
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_is_kick(self, event_data: dict):
         scenarios = [
-            ('isKick'),
+            ('isKick',),
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_is_ban(self, event_data: dict):
         scenarios = [
-            ('isBan'),
+            ('isBan',),
         ]
         return self._scenario(event_data, scenarios)
 
     def _get_bumped_at(self, event_data: dict):
         scenarios = [
             ('forumTopic', 'bumpedAt'),
         ]
@@ -555,15 +555,15 @@
         scenarios = [
             ('userInfo', 'nickname'),
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_role_ids(self, event_data: dict):
         scenarios = [
-            ('memberRoleIds'),
+            ('memberRoleIds',),
             ('calendarEvent', 'roleIds'),
         ]
         return self._scenario(event_data, scenarios)
 
     def _get_reason(self, event_data: dict):
         scenarios = [
             ('serverMemberBan', 'reason'),
@@ -645,35 +645,35 @@
         scenarios = [
             ('reaction', 'emote', 'serverId'),
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_forum_topic_id(self, event_data: dict):
         scenarios = [
-            ('forumTopicId'),
+            ('forumTopicId',),
             ('forumTopicComment', 'forumTopicId'),
             ('reaction', 'forumTopicId'),
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_calendar_event_rsvps(self, event_data: dict):
         scenarios = [
-            ('calendarEventRsvps'),
+            ('calendarEventRsvps',),
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_webhook_id(self, event_data: dict):
         scenarios = [
             ('listItem', 'createdByWebhookId'),
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_count(self, event_data: dict):
         scenarios = [
-            ('count'),
+            ('count',),
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_comment_id(self, event_data: dict):
         scenarios = [
             ('reaction', 'forumTopicCommentId'),
             ('reaction', 'calendarEventCommentId'),
@@ -681,15 +681,15 @@
             ('reaction', 'announcementCommentId'),
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_event_id(self, event_data: dict):
         scenarios = [
             ('calendarEventComment', 'calendarEventId'),
-            ('calendarEventId'),
+            ('calendarEventId',),
         ]
         return self._scenario(event_data, scenarios)
     
     def _get_doc_id(self, event_data: dict):
         scenarios = [
             ('reaction', 'docId'),
         ]
```

### Comparing `nextguild-1.2.2/nextguild/client.py` & `nextguild-1.2.3/nextguild/client.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.2/nextguild/embed.py` & `nextguild-1.2.3/nextguild/embed.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.2/nextguild/events.py` & `nextguild-1.2.3/nextguild/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,19 +91,19 @@
         self._announcement_comment_update_handlers = []
         self._announcement_comment_delete_handlers = []
         self._announcement_comment_reaction_create_handlers = []
         self._announcement_comment_reaction_delete_handlers = []
         self._group_create_handlers = []
         self._group_update_handlers = []
         self._group_delete_handlers = []
-        self.on_user_status_create_handlers = []
-        self.on_user_status_delete_handlers = []
-        self.on_role_create_handlers = []
-        self.on_role_update_handlers = []
-        self.on_role_delete_handlers = []
+        self._user_status_create_handlers = []
+        self._user_status_delete_handlers = []
+        self._role_create_handlers = []
+        self._role_update_handlers = []
+        self._role_delete_handlers = []
         self.client = client
     
     def on_bot_membership_created(self, func):
         @wraps(func)
         def wrapper(server):
             return func(server)
```

### Comparing `nextguild-1.2.2/nextguild.egg-info/PKG-INFO` & `nextguild-1.2.3/nextguild.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.2.2
+Version: 1.2.3
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.2.2/pyproject.toml` & `nextguild-1.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "requests", "asyncio", "websockets"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nextguild"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
     { name="Arjun Sharda", email="sharda.aj17@gmail.com" },
     { name="Erik Thorsell", email="contact@erikthorsell.com" },
 ]
 description = "Interactions with the Guilded API made simpler"
 readme = "README.md"
 license = { file="LICENSE" }
```

