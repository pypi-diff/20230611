# Comparing `tmp/les_louisdelatech-0.3.1.tar.gz` & `tmp/les_louisdelatech-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "les_louisdelatech-0.3.1.tar", max compression
+gzip compressed data, was "les_louisdelatech-0.3.2.tar", max compression
```

## Comparing `les_louisdelatech-0.3.1.tar` & `les_louisdelatech-0.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    22294 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/LICENSE
--rw-r--r--   0        0        0    23504 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/LICENSE.fr
--rw-r--r--   0        0        0     2307 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/__init__.py
--rw-r--r--   0        0        0     3330 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/bot.py
--rw-r--r--   0        0        0      824 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/extensions/cats.py
--rw-r--r--   0        0        0      492 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/extensions/config.py
--rw-r--r--   0        0        0     2913 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/extensions/management.py
--rw-r--r--   0        0        0     4632 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/extensions/otp.py
--rw-r--r--   0        0        0      683 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/extensions/task.py
--rw-r--r--   0        0        0    15315 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/extensions/user.py
--rw-r--r--   0        0        0     1366 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/main.py
--rw-r--r--   0        0        0       45 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/models/__init__.py
--rw-r--r--   0        0        0      481 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/models/otp.py
--rw-r--r--   0        0        0     1094 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/base.j2
--rw-r--r--   0        0        0        0 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/ca.j2
--rw-r--r--   0        0        0        0 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/logistique.j2
--rw-r--r--   0        0        0        0 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/marketing.j2
--rw-r--r--   0        0        0      459 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/reset_password.j2
--rw-r--r--   0        0        0        0 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/scene.j2
--rw-r--r--   0        0        0        0 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/technique.j2
--rw-r--r--   0        0        0        0 2023-05-18 18:55:38.704489 les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/tournoi.j2
--rw-r--r--   0        0        0     2705 2023-05-18 18:55:38.708489 les_louisdelatech-0.3.1/les_louisdelatech/templates/google/gmail_signature.j2
--rw-r--r--   0        0        0       48 2023-05-18 18:55:38.708489 les_louisdelatech-0.3.1/les_louisdelatech/utils/LouisDeLaTechError.py
--rw-r--r--   0        0        0     2958 2023-05-18 18:55:38.708489 les_louisdelatech-0.3.1/les_louisdelatech/utils/User.py
--rw-r--r--   0        0        0      753 2023-05-18 18:55:38.708489 les_louisdelatech-0.3.1/les_louisdelatech/utils/discord.py
--rw-r--r--   0        0        0     6169 2023-05-18 18:55:38.708489 les_louisdelatech-0.3.1/les_louisdelatech/utils/gsuite.py
--rw-r--r--   0        0        0      380 2023-05-18 18:55:38.708489 les_louisdelatech-0.3.1/les_louisdelatech/utils/password.py
--rw-r--r--   0        0        0     1474 2023-05-18 18:56:14.196703 les_louisdelatech-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3861 1970-01-01 00:00:00.000000 les_louisdelatech-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    22294 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/LICENSE
+-rw-r--r--   0        0        0    23504 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/LICENSE.fr
+-rw-r--r--   0        0        0     2307 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/__init__.py
+-rw-r--r--   0        0        0     3330 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/bot.py
+-rw-r--r--   0        0        0      850 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/extensions/cats.py
+-rw-r--r--   0        0        0      519 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/extensions/config.py
+-rw-r--r--   0        0        0     2940 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/extensions/management.py
+-rw-r--r--   0        0        0     4740 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/extensions/otp.py
+-rw-r--r--   0        0        0      683 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/extensions/task.py
+-rw-r--r--   0        0        0    15504 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/extensions/user.py
+-rw-r--r--   0        0        0     1366 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/main.py
+-rw-r--r--   0        0        0       45 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/models/__init__.py
+-rw-r--r--   0        0        0      481 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/models/otp.py
+-rw-r--r--   0        0        0     1094 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/templates/discord/base.j2
+-rw-r--r--   0        0        0        0 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/templates/discord/ca.j2
+-rw-r--r--   0        0        0        0 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/templates/discord/logistique.j2
+-rw-r--r--   0        0        0        0 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/templates/discord/marketing.j2
+-rw-r--r--   0        0        0      459 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/templates/discord/reset_password.j2
+-rw-r--r--   0        0        0        0 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/templates/discord/scene.j2
+-rw-r--r--   0        0        0        0 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/templates/discord/technique.j2
+-rw-r--r--   0        0        0        0 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/templates/discord/tournoi.j2
+-rw-r--r--   0        0        0     2705 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/templates/google/gmail_signature.j2
+-rw-r--r--   0        0        0       48 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/utils/LouisDeLaTechError.py
+-rw-r--r--   0        0        0     2958 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/utils/User.py
+-rw-r--r--   0        0        0      753 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/utils/discord.py
+-rw-r--r--   0        0        0     6169 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/utils/gsuite.py
+-rw-r--r--   0        0        0      380 2023-06-10 21:59:18.630087 les_louisdelatech-0.3.2/les_louisdelatech/utils/password.py
+-rw-r--r--   0        0        0     1474 2023-06-10 21:59:45.806328 les_louisdelatech-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3659 1970-01-01 00:00:00.000000 les_louisdelatech-0.3.2/PKG-INFO
```

### Comparing `les_louisdelatech-0.3.1/LICENSE` & `les_louisdelatech-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.1/LICENSE.fr` & `les_louisdelatech-0.3.2/LICENSE.fr`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.1/README.md` & `les_louisdelatech-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.1/les_louisdelatech/bot.py` & `les_louisdelatech-0.3.2/les_louisdelatech/bot.py`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.1/les_louisdelatech/extensions/cats.py` & `les_louisdelatech-0.3.2/les_louisdelatech/extensions/cats.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 class CatCog(commands.Cog):
     def __init__(self, bot):
         self.bot = bot
 
     @commands.hybrid_command(name="cat", help="Get cat")
     async def get_cat(self, ctx: Context):
+        await ctx.defer()
         async with httpx.AsyncClient() as client:
             cat_data = await client.get("https://api.thecatapi.com/v1/images/search")
 
         payload = cat_data.json()
         if not payload:
             return
         cat_url = payload[0]["url"]
```

### Comparing `les_louisdelatech-0.3.1/les_louisdelatech/extensions/management.py` & `les_louisdelatech-0.3.2/les_louisdelatech/extensions/management.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     @commands.hybrid_command(help="Change channel topic")
     @is_team_allowed
     async def topic(
         self,
         ctx,
         description: str = commands.parameter(description="Topic description"),
     ):
+        await ctx.defer()
         await ctx.channel.edit(topic=description)
         await ctx.send("Channel topic updated")
 
     # Meeting voice channel creation & deletion listener
     @commands.Cog.listener()
     async def on_voice_state_update(self, member, before, after):
         # Create voice channel block
```

### Comparing `les_louisdelatech-0.3.1/les_louisdelatech/extensions/otp.py` & `les_louisdelatech-0.3.2/les_louisdelatech/extensions/otp.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     def __init__(self, bot):
         self.bot = bot
 
     @commands.hybrid_command(name="lotp", help="List otp code")
     @commands.guild_only()
     @is_team_allowed
     async def list_otp(self, ctx):
+        await ctx.defer()
         try:
             user = User(
                 search_user(self.bot.admin_sdk(), ctx.author.name, ctx.author.id)
             )
         except LouisDeLaTechError as e:
             await ctx.send(f"{ctx.author} => {e.args[0]}")
             return
@@ -46,14 +47,15 @@
 
     @commands.hybrid_command(name="gotp", help="Get otp code")
     @commands.guild_only()
     @is_team_allowed
     async def get_otp(
         self, ctx, name: str = commands.parameter(description="Otp name")
     ):
+        await ctx.defer()
         try:
             user = User(
                 search_user(self.bot.admin_sdk(), ctx.author.name, ctx.author.id)
             )
         except LouisDeLaTechError as e:
             await ctx.send(f"{ctx.author} => {e.args[0]}")
             return
@@ -83,14 +85,15 @@
         self,
         ctx,
         name: str = commands.parameter(description="Otp name"),
         digest: str = commands.parameter(description="Otp digest"),
         digits: str = commands.parameter(description="Otp digits"),
         secret: str = commands.parameter(description="Otp secret"),
     ):
+        await ctx.defer()
         await ctx.message.delete()
 
         try:
             user = User(
                 search_user(self.bot.admin_sdk(), ctx.author.name, ctx.author.id)
             )
         except LouisDeLaTechError as e:
@@ -113,14 +116,15 @@
 
     @commands.hybrid_command(name="dotp", help="Delete otp code")
     @commands.guild_only()
     @is_team_allowed
     async def delete_otp(
         self, ctx, name: str = commands.parameter(description="Otp name")
     ):
+        await ctx.defer()
         try:
             user = User(
                 search_user(self.bot.admin_sdk(), ctx.author.name, ctx.author.id)
             )
         except LouisDeLaTechError as e:
             await ctx.send(f"{ctx.author} => {e.args[0]}")
             return
```

### Comparing `les_louisdelatech-0.3.1/les_louisdelatech/extensions/task.py` & `les_louisdelatech-0.3.2/les_louisdelatech/extensions/task.py`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.1/les_louisdelatech/extensions/user.py` & `les_louisdelatech-0.3.2/les_louisdelatech/extensions/user.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         Provision an user
         [Discord]
             => User will be added to default group
             => User will be added to team group
         [Google]
             => User will be created and added to team group
         """
+        await ctx.defer()
         user_email = User.email_from_name(firstname, lastname)
         user_team = self.bot.config["teams"].get(role_name, None)
         password = generate_password()
         admin_sdk = self.bot.admin_sdk()
         signature_template = Template(
             open(
                 os.path.join(
@@ -161,14 +162,15 @@
     ):
         """
         [Discord]
             => User will be removed from all groups
         [Google]
             => User will be suspended
         """
+        await ctx.defer()
         try:
             user = User(search_user(self.bot.admin_sdk(), member.name, member.id))
             is_user_managed(
                 self.bot.admin_sdk(), user.email, self.bot.config["teams_to_skip"]
             )
         except LouisDeLaTechError as e:
             await ctx.send(f"{member} => {e.args[0]}")
@@ -201,14 +203,15 @@
             => User will be removed from all team groups
             => User will be added to this new team
         [Google]
             => User will be removed from all team groups
             => User will be added to this new team
             => User signature will be updated
         """
+        await ctx.defer()
         try:
             user = User(search_user(self.bot.admin_sdk(), member.name, member.id))
             is_user_managed(
                 self.bot.admin_sdk(), user.email, self.bot.config["teams_to_skip"]
             )
             user.team = new_team_name
         except LouisDeLaTechError as e:
@@ -288,14 +291,15 @@
     ):
         """
         [Discord]
             => User will be renamed
         [Google]
             => User pseudo will be renamed
         """
+        await ctx.defer()
         try:
             user = User(search_user(self.bot.admin_sdk(), member.name, member.id))
             is_user_managed(
                 self.bot.admin_sdk(), user.email, self.bot.config["teams_to_skip"]
             )
             user.pseudo = new_pseudo
         except LouisDeLaTechError as e:
@@ -325,14 +329,15 @@
 
     @commands.hybrid_command(
         name="usignatures", help="Update the signature of all users on gmail"
     )
     @commands.guild_only()
     @is_gsuite_admin
     async def update_signatures(self, ctx):
+        await ctx.defer()
         user_updated = 0
         try:
             users = get_users(self.bot.admin_sdk())
         except HttpError as e:
             await ctx.send(format_google_api_error(e))
             raise
 
@@ -378,14 +383,15 @@
     @is_gsuite_admin
     async def urecovery(
         self,
         ctx,
         member: discord.Member = commands.parameter(description="Discord user"),
         backup_email: str = commands.parameter(description="User backup email"),
     ):
+        await ctx.defer()
         try:
             user = User(search_user(self.bot.admin_sdk(), member.name, member.id))
             is_user_managed(
                 self.bot.admin_sdk(), user.email, self.bot.config["teams_to_skip"]
             )
         except LouisDeLaTechError as e:
             await ctx.send(f"{member} => {e.args[0]}")
@@ -405,14 +411,15 @@
     @commands.guild_only()
     @is_gsuite_admin
     async def rpassword(
         self,
         ctx,
         member: discord.Member = commands.parameter(description="Discord user"),
     ):
+        await ctx.defer()
         try:
             user = User(search_user(self.bot.admin_sdk(), member.name, member.id))
             is_user_managed(
                 self.bot.admin_sdk(), user.email, self.bot.config["teams_to_skip"]
             )
         except LouisDeLaTechError as e:
             await ctx.send(f"{member} => {e.args[0]}")
```

### Comparing `les_louisdelatech-0.3.1/les_louisdelatech/main.py` & `les_louisdelatech-0.3.2/les_louisdelatech/main.py`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.1/les_louisdelatech/templates/discord/base.j2` & `les_louisdelatech-0.3.2/les_louisdelatech/templates/discord/base.j2`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.1/les_louisdelatech/templates/google/gmail_signature.j2` & `les_louisdelatech-0.3.2/les_louisdelatech/templates/google/gmail_signature.j2`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.1/les_louisdelatech/utils/User.py` & `les_louisdelatech-0.3.2/les_louisdelatech/utils/User.py`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.1/les_louisdelatech/utils/discord.py` & `les_louisdelatech-0.3.2/les_louisdelatech/utils/discord.py`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.1/les_louisdelatech/utils/gsuite.py` & `les_louisdelatech-0.3.2/les_louisdelatech/utils/gsuite.py`

 * *Files identical despite different names*

### Comparing `les_louisdelatech-0.3.1/pyproject.toml` & `les_louisdelatech-0.3.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "les-louisdelatech"
-version = "0.3.1"
+version = "0.3.2"
 description = "LouisDeLaTech is a discord bot manager for Lyon e-Sport"
 authors = [
     "Ludovic Ortega <ludovic.ortega@lyon-esport.fr>",
     "Etienne 'PoPs' G. <etienne.guilluy@lyon-esport.fr>",
     "Pierre 'DrumSlayer' Sarret <pierre.sarret@lyon-esport.fr>",
 
 ]
@@ -33,15 +33,15 @@
 discord-py = "^2.2.3"
 Jinja2 = "^3.1.2"
 google-api-python-client = "^2.52.0"
 google-auth-httplib2 = "^0.1.0"
 pyotp = "^2.6.0"
 tortoise-orm = "^0.19.1"
 aiosqlite = "^0.17.0"
-cryptography = ">=37.0.4,<41.0.0"
+cryptography = ">=37.0.4,<42.0.0"
 sentry-sdk = "^1.6.0"
 httpx = ">=0.23,<0.25"
 tomli = "^2.0.1"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^3.3.2"
```

### Comparing `les_louisdelatech-0.3.1/PKG-INFO` & `les_louisdelatech-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: les-louisdelatech
-Version: 0.3.1
+Version: 0.3.2
 Summary: LouisDeLaTech is a discord bot manager for Lyon e-Sport
 Home-page: https://github.com/lyon-esport/LouisDeLaTech
 License: CeCILL
 Keywords: google,discord
 Author: Ludovic Ortega
 Author-email: ludovic.ortega@lyon-esport.fr
 Requires-Python: >=3.8,<4.0
@@ -13,22 +13,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: aiosqlite (>=0.17.0,<0.18.0)
-Requires-Dist: cryptography (>=37.0.4,<41.0.0)
+Requires-Dist: cryptography (>=37.0.4,<42.0.0)
 Requires-Dist: discord-py (>=2.2.3,<3.0.0)
 Requires-Dist: google-api-python-client (>=2.52.0,<3.0.0)
 Requires-Dist: google-auth-httplib2 (>=0.1.0,<0.2.0)
 Requires-Dist: httpx (>=0.23,<0.25)
 Requires-Dist: pyotp (>=2.6.0,<3.0.0)
 Requires-Dist: sentry-sdk (>=1.6.0,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
```

