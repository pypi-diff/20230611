# Comparing `tmp/yeref-0.1.80.tar.gz` & `tmp/yeref-0.1.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.80.tar", last modified: Sun Jun  4 09:24:15 2023, max compression
+gzip compressed data, was "yeref-0.1.81.tar", last modified: Sun Jun 11 13:21:30 2023, max compression
```

## Comparing `yeref-0.1.80.tar` & `yeref-0.1.81.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-04 09:24:15.859728 yeref-0.1.80/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-04 09:24:15.859881 yeref-0.1.80/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-04 09:24:15.860490 yeref-0.1.80/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-04 09:24:01.000000 yeref-0.1.80/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-04 09:24:15.847750 yeref-0.1.80/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.80/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   533408 2023-06-04 09:12:57.000000 yeref-0.1.80/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   208832 2023-06-04 07:17:18.000000 yeref-0.1.80/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-04 09:24:15.859277 yeref-0.1.80/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-04 09:24:15.000000 yeref-0.1.80/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-04 09:24:15.000000 yeref-0.1.80/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-04 09:24:15.000000 yeref-0.1.80/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-04 09:24:15.000000 yeref-0.1.80/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 13:21:30.844330 yeref-0.1.81/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 13:21:30.844572 yeref-0.1.81/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-11 13:21:30.845502 yeref-0.1.81/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-11 13:21:03.000000 yeref-0.1.81/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 13:21:30.836755 yeref-0.1.81/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.81/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   535217 2023-06-11 12:46:53.000000 yeref-0.1.81/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   212328 2023-06-11 13:20:55.000000 yeref-0.1.81/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 13:21:30.843347 yeref-0.1.81/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 13:21:30.000000 yeref-0.1.81/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-11 13:21:30.000000 yeref-0.1.81/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-11 13:21:30.000000 yeref-0.1.81/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-11 13:21:30.000000 yeref-0.1.81/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.80/setup.py` & `yeref-0.1.81/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.80',
+      version='0.1.81',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -43,12 +43,12 @@
 
 # twine upload dist/*
 # freey.sitner.ya
 # cejwez-nosgin-vaVfe7
 
 # python3 -m pip install --upgrade yeref
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.72-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.80-py3-none-any.whl
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
 # ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.1.80/yeref/l_.py` & `yeref-0.1.81/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,14 +109,22 @@
     'ru': "🚫 Удалить",
     'en': "🚫 Delete",
     'es': "🚫 Eliminar",
     'fr': "🚫 Supprimer",
     'zh': "🚫 删除",
     'ar': "🚫 حذف",
 }
+l_try_again = {
+    'ru': "👩🏽‍💻 <b>Попробуйте</b> позже",
+    'en': "👩🏽‍💻 Try again later",
+    'es': "🚫 Eliminar",
+    'fr': "🚫 Supprimer",
+    'zh': "🚫 删除",
+    'ar': "🚫 حذف",
+}
 
 l_choose_direction = {
     'ru': "👇🏽 <b>Выбери</b> направление",
     'en': "👇🏽 <b>Choose</b> a direction",
     'es': "👇🏽 <b>Elige</b> una dirección",
     'fr': "👇🏽 <b>Choisissez</b> une direction",
     'zh': "👇🏽<b>选择</b>方向",
@@ -126,30 +134,62 @@
     'ru': "<b>👩🏽‍💻 Ferey проекты</b>:\n\n▪️проекты: @FereyDemoBot\n▪️конструктор: @FereyBotBot\n▪️приватные посты: @FereyPostBot\n▪️публичные медиа: @FereyMediaBot\n▪️администрирование: @FereyChannelBot\n▪️модерация: @FereyGroupBot\n▪️поиск: @FereyFindBot\n▪️таргет: @FereyTargetBot\n▪️инструменты: @FereyToolsBot\n▪️vpn: @FereyVPNBot\n▪️ai: @FereyAIBot\n▪️автоматизация: @FereyUserBot\n▪️вакансии: @FereyWorkBot\n▪️реклама: @FereyAdsBot",
     'en': "<b>👩🏽‍💻 Ferey projects</b>:\n\n▪️projects: @FereyDemoBot\n▪️constructor: @FereyBotBot\n▪️private_posts: @FereyPostBot\n▪️public_media: @FereyMediaBot\n▪️administration: @FereyChannelBot\n▪️moderation: @FereyGroupBot\n▪️search: @FereyFindBot\n▪️target: @FereyTargetBot\n▪️tools: @FereyToolsBot\n▪️vpn: @FereyVPNBot\n▪️ai: @FereyAIBot\n▪️automation: @FereyUserBot\n▪️vacancies: @FereyWorkBot\n▪️advert: @FereyAdsBot",
     'es': "<b>👩🏽‍💻 Proyectos de Ferey</b> :\n\n▪️proyectos: @FereyDemoBot\n▪️constructor: @FereyBotBot\n▪️publicaciones_privadas: @FereyPostBot\n▪️medios_públicos: @FereyMediaBot\n▪️administración: @FereyChannelBot\n▪️moderación: @FereyGroupBot\nƒ️búsqueda: @FereyFindBot\nƒ️objetivo: @FereyTargetBot\nƒ️herramientas: @FereyToolsBot\nƒ️vpn: @FereyVPNBot\nƒ️ai: @FereyAIBot\nƒ️automatización: @FereyUserBot\nƒ️vacantes: @FereyWorkBot\n▪️anuncio: @FereyAdsBot",
     'fr': "<b>👩🏽‍💻 Projets Ferey</b> :\n\n▪️projets : @FereyDemoBot\n▪️constructeur : @FereyBotBot\n▪️public_medias : @FereyPostBot\n▪️public_media : @FereyMediaBot\n▪️administration : @FereyChannelBot\n▪️modération : @FereyGroupBot\n▪️recherche : @FereyFindBot\n▪️cible : @FereyTargetBot\n▪️outils : @FereyToolsBot\n▪️vpn : @FereyVPNBot\n▪️ai : @FereyAIBot\n▪️automatisation : @FereyUserBot\n▪️postes vacants : @FereyWorkBot\n▪️annonce : @FereyAdsBot",
     'zh': "<b>👩🏽‍💻 Ferey 项目</b>：\n\n▪️projects： @FereyDemoBot\n▪️constructor： @FereyBotBot\n▪️private_posts： @FereyPostBot\n▪️public_media： @FereyMediaBot\n▪️administration： @FereyChannelBot\n▪️moderation： @FereyGroupBot\n▪️搜索： @FereyFindBot\n▪️目标： @FereyTargetBot\n▪️工具： @FereyToolsBot\n▪️vpn： @FereyVPNBot\n▪️ai： @FereyAIBot\n▪️自动化： @FereyUserBot\n▪️空缺： @FereyWorkBot\n▪️广告： @FereyAdsBot",
     'ar': "<b>👩🏽‍💻 المشاريع السريعة</b> :\n\n▪️ المشاريع: @FereyDemoBot\n▪️ المُنشئ: @FereyBotBot\n▪️private_posts: @FereyPostBot\n▪️public_media: @FereyMediaBot\n▪️administration: @FereyChannelBot : @ @FereyGroupBot\n▪️search: @FereyFindBot\n▪️ الهدف: @FereyTargetBot\n▪️ الأدوات: @FereyToolsBot\n▪️vpn: @FereyVPNBot\n▪️ai: @FereyAIBot\n▪️automation: @FereyUserBot @FereyWorkBot\nإعلان: @FereyAdsBot",
 }
-l_subscribe = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>\n\n¹ на @{0}-бота [{1} ₽]\n▪️ отсутствие рекламы\n▪️ творческие задания\n² Подписка на <u>всех</u> ботов [{2} ₽]",
-    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
-    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
-    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
-    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
-    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
-}
 l_subscribe_btn = {
     'ru': "👩🏽‍💻 Я подписался",
     'en': "👩🏽‍💻 I subscribed",
     'es': "👩🏽‍💻 Me suscribí",
     'fr': "👩🏽‍💻 je me suis abonné",
     'zh': "👩🏽‍💻 我订阅了",
     'ar': "👩🏽‍💻 لقد اشتركت",
 }
+l_subscribe_all = {
+    'ru': "¹ Все боты и проекты",
+    'en': "¹ All bots & projects",
+    'es': "¹ All bots & projects",
+    'fr': "¹ All bots & projects",
+    'zh': "¹ All bots & projects",
+    'ar': "¹ All bots & projects",
+}
+l_subscribe_already = {
+    'ru': "👩🏽‍💻 У вас уже есть активная подписка",
+    'en': "¹ All bots & projects",
+    'es': "¹ All bots & projects",
+    'fr': "¹ All bots & projects",
+    'zh': "¹ All bots & projects",
+    'ar': "¹ All bots & projects",
+}
+l_subscribe_wait = {
+    'ru': "👩🏽‍💻 Обработка @donate..\n\n#длительность 1мин",
+    'en': "¹ All bots & projects",
+    'es': "¹ All bots & projects",
+    'fr': "¹ All bots & projects",
+    'zh': "¹ All bots & projects",
+    'ar': "¹ All bots & projects",
+}
+l_subscribe_success = {
+    'ru': "👩🏽‍💻 <b>Успешный</b> донат!",
+    'en': "👩🏽‍💻 Успешный донат!",
+    'es': "¹ All bots & projects",
+    'fr': "¹ All bots & projects",
+    'zh': "¹ All bots & projects",
+    'ar': "¹ All bots & projects",
+}
+l_subscribe_balance = {
+    'ru': "👩🏽‍💻 Текущий /balance {0}{1}",
+    'en': "👩🏽‍💻 Current /balance {0}{1}",
+    'es': "¹ All bots & projects",
+    'fr': "¹ All bots & projects",
+    'zh': "¹ All bots & projects",
+    'ar': "¹ All bots & projects",
+}
 l_language_get = {
     'ru': "🌏 <b>Выбери</b> один из доступных языков",
     'en': "🌏 <b>Choose</b> one of the available languages",
     'es': "🌏 <b>Elige</b> uno de los idiomas disponibles",
     'fr': "🌏 <b>Choisissez</b> l'une des langues disponibles",
     'zh': "🌏<b>选择</b>一种可用的语言",
     'ar': "🌏 <b>اختر</b> إحدى اللغات المتاحة",
@@ -6189,14 +6229,22 @@
     'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>автоматизации</code> <b>Telegram</b>-ботов:\n\n▪️авто-постинг и <b>авто-перевод</b>\n▪️<b>авто-ответы</b> и оповещения\n▪️интеграции и платежи\n▪️пользователи и администраторы\n\n❗️также можно заказать разработку чат-бота в нашей <a href='https://t.me/{1}'>ferey</a>-студии",
     'en': "🌱 {0}, welcome to the <b>Telegram</b> bot <code>автоматизации</code> <i>landing bot</i> :\n\n▪️auto-posting and <b>auto-translation</b>\n▪️ <b>auto-replies</b> and notifications\n▪️integrations and payments\n▪️users and administrators\n\n❗️You can also order the development of a chatbot in our ferey studio",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> <code>автоматизации</code> de bots <b>de Telegram</b> :\n\n▪️auto-publicación y <b>auto-traducción</b>\n▪️auto <b>-respuestas</b> y notificaciones\n▪️integraciones y pagos\n▪️usuarios y administradores\n\n❗️también puedes encargar el desarrollo de un chatbot en nuestro ferey studio",
     'fr': "🌱 {0}, bienvenue dans le <i>bot d&#x27;atterrissage</i> <code>автоматизации</code> du bot <b>Telegram</b> :\n\n▪️publication et <b>traduction automatiques</b>\n▪️ <b>réponses et notifications automatiques</b>\n▪️intégrations et paiements\n▪️utilisateurs et administrateurs\n\n❗️Vous pouvez également commander le développement d'un chatbot dans notre studio ferey",
     'zh': "🌱 {0}，欢迎使用<b>Telegram</b>机器人<code>автоматизации</code><i>登陆机器人</i>：\n\n▪️自动发布和<b>自动翻译</b>\n▪️<b>自动回复</b>和通知\n▪️集成和支付\n▪️用户和管理员\n\n❗️您也可以在我们的ferey工作室订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوط</i> <code>автоматизации</code> لروبوت <b>Telegram</b> :\n\n▪️ النشر التلقائي <b>والترجمة التلقائية</b>\n▪️ <b>الردود التلقائية</b> والإشعارات\n▪️ عمليات الدمج والمدفوعات\nالمستخدمون والمسؤولون\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو ferey الخاص بنا",
 }
+l_subscribe_bot = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️авто-перевод\n(<i>в том числе, текста кнопок</i>)\n▪️авто-ответ\n(<i>chatgpt видит блоки бота</i>)\n▪️приоритетная поддержка\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
 
 l_add_bot_button = {
     'ru': "➕ Добавить бота",
     'en': "➕ Add a bot",
     'es': "➕ Agregar un bot",
     'fr': "➕ Ajouter un robot",
     'zh': "➕ 添加机器人",
@@ -6883,15 +6931,15 @@
     'en': "👮🏽 <b>Done!</b> /admin-list @{0}-bot:\n\n{1}\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/admin - add/remove administrator\n/parse - display all users\n\n👩🏽‍💻 <b>Current</b> number of admins: <u>{2}/10</u>",
     'es': "👮🏽 <b>Listo!</b> /admin-list @{0}-bot:\n\n{1}\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/admin - agregar/eliminar administrador\n/parse - mostrar todos los usuarios\n\n👩🏽‍💻 Número <b>actual</b> de administradores: <u>{2}/10</u>",
     'fr': "👮🏽 <b>C&#x27;est fait !</b> /admin-list @{0}-bot :\n\n{1}\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/admin - ajouter/supprimer un administrateur\n/parse - afficher tous les utilisateurs\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;administrateurs : <u>{2}/10</u>",
     'zh': "👮🏽<b>完成！</b> /admin-list @{0}-bot:\n\n{1}\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/admin - 添加/删除管理员\n/parse - 显示所有用户\n\n👩🏽‍💻<b>当前</b>管理员人数： <u>{2}/10</u>",
     'ar': "👮🏽 <b>انتهى!</b> / admin-list @ {0} -bot:\n\n{1}\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - جميع الأوامر\n/ admin - إضافة / إزالة المسؤول\n/ parse - عرض جميع المستخدمين\n\n👩🏽‍💻 العدد <b>الحالي</b> للمسؤولين: <u>{2} / 10</u>",
 }
 l_cadmin_add = {
-    'ru': "👮🏽 <b>Введи</b> <code>id</code> пользователей через пробельные символы или разделители, чтобы добавить их в /admin-список\n\n👩🏽‍💻 <b>Текущее</b> число администраторов: <u>{0}</u>",
+    'ru': "👮🏽 <b>Введи</b> до 10 <code>id</code>-пользователей через пробельные символы или разделители, чтобы добавить их в /admin-список\n\n👩🏽‍💻 <b>Текущее</b> число администраторов: <u>{0}</u>",
     'en': "👮🏽 <b>Enter</b> user <code>id</code> separated by spaces or separators to add them to /admin-list\n\n👩🏽‍💻 <b>Current</b> number of admins: <u>{0}</u>",
     'es': "👮🏽 <b>Ingrese</b> <code>id</code> de usuario separados por espacios o separadores para agregarlos a /admin-list\n\n👩🏽‍💻 Número <b>actual</b> de administradores: <u>{0}</u>",
     'fr': "👮🏽 <b>Entrez</b> <code>id</code> des utilisateurs séparés par des espaces ou des séparateurs pour les ajouter à /admin-list\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;administrateurs : <u>{0}</u>",
     'zh': "👮🏽<b>输入</b>以空格或分隔符分隔的用户<code>id</code> ，以将其添加到 /admin-list\n\n👩🏽‍💻<b>当前</b>管理员人数： <u>{0}</u>",
     'ar': "👮🏽 <b>أدخل</b> <code>id</code> المستخدمين مفصولة بمسافات أو فواصل لإضافتها إلى / قائمة المشرف\n\n👩🏽‍💻 العدد <b>الحالي</b> للمسؤولين: <u>{0}</u>",
 }
 l_cadmin_remove = {
```

### Comparing `yeref-0.1.80/yeref/yeref.py` & `yeref-0.1.81/yeref/yeref.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from contextlib import closing
 from math import radians, cos, sin, asin, sqrt
 from random import randrange
 from uuid import uuid4
 import httplib2
 import moviepy.editor as mp
 from PIL import Image
-from aiogram import types
+from aiogram import types, Bot
 from aiogram.enums import ParseMode
 from aiogram.exceptions import TelegramRetryAfter
 from aiogram.utils.keyboard import InlineKeyboardBuilder
 from aiogram.utils.text_decorations import markdown_decoration
 from exiftool import ExifToolHelper
 from googleapiclient.discovery import build
 from googleapiclient.http import MediaFileUpload, MediaIoBaseDownload
@@ -38,41 +38,32 @@
     InviteHashExpired, InviteHashInvalid, ChatAdminRequired, UserDeactivated, UsernameNotOccupied, ChannelBanned
 from pyrogram.raw import functions
 from stegano import lsb, exifHeader
 from telegraph.aio import Telegraph
 
 import yeref
 
-one_minute = 60
-one_hour = 3600
-seconds_in_day = 86400
+
+elly_a = 5900268983
 my_tid = 5491025132
 my_tids = [
     '5900268983',
     '6283902226',
     '6090677494',
 
     '5754810063',
     '5491025132',
     '5360564451',
     '6281795468',
 ]
-old_tid = 5_000_000_000
-lat_company = 59.395881
-long_company = 24.658980
-lkjhgfdsa_channel_id = -1001657854832
-lkjhgfdsa_channel_un = "lkjhgfdsa_channel"
-tg_ch_ads_un = 'kiejakn3_djdjn4m_ads'
-tg_ch_ads_id = -1001921910898
-price_one = 200
-price_all = 500
-passwd = 'lost9'
-bin_empty = b'\xe2\x81\xa0\xe2\x81\xa0'  # .encode("utf-8")
-hex_empty = 'e281a0e281a0'  # .encode("utf-8").hex()  || bytes.fromhex()
-str_empty = bin_empty.decode('utf-8')
+channel_library_ru = -1001484489131
+channel_library_en = -1001481302043
+BOT_TOKEN_E18B = '5663692429:AAHolleuTfJmSimvSr9i3BsxCvbeOAU7Kbk'
+e18b_bot = '@e18be3f08cf66117744a889900dc_bot'
+e18b_channel = -1001956430283
 
 TGPH_TOKEN_MAIN = 'a9335172886eae62ec0743bf8a4e195286ec30cff067da5fd1db2899d008'
 TGPH_TOKENS = {
     "https://telegra.ph/pst-FereyDemoBot-05-08": "f8c69d50846e8d55e08f8e3de514f41266e0150434219059f2c91fb4d75f",
     "https://telegra.ph/pst-FereyBotBot-05-08": "e7f943fcc98bac07ad6aaf6e570d0f51abadf02567938c997dbc1ad1923b",
     "https://telegra.ph/pst-FereyPostBot-05-08": "14085be3058c0a25616d094f4bb65c73dc61f783468f01da41d99fb6ace1",
     "https://telegra.ph/pst-FereyMediaBot-05-08": "cf71a596b7ecdc96d30ddffdbf1e26863dd39755f47b4fc343fc3867f373",
@@ -83,14 +74,29 @@
     "https://telegra.ph/pst-FereyToolsBot-05-08": "ea83403eb6ac7d2ad24d7e7a86163be20cd2d7f4734267808e154a8fd0a6",
     "https://telegra.ph/pst-FereyVPNBot-05-08": "38086caf43905ef827715da999aae0be2427ebd7a05d9ff7420543b50613",
     "https://telegra.ph/pst-FereyAIBot-05-08": "bcda631d991c16b4fdfd15e7af6512bcf8fd679fee6bd4c717f6266671a0",
     "https://telegra.ph/pst-FereyUserBot-05-08": "3698a3432c233bef48c238b35cfe94db844858b2ba98594007c7757dcf03",
     "https://telegra.ph/pst-FereyWorkBot-05-08": "d4930b2a9311ad63f7f0ae3d61ca7224ecf76a2434a50161e239a45199c5",
     "https://telegra.ph/pst-FereyAdsBot-05-08": "c1024508f1a5de4f9544dd10793b1401da95de5719bdcf0b4c9f6c26a672",
 }
+
+one_minute = 60
+one_hour = 3600
+seconds_in_day = 86400
+old_tid = 5_000_000_000
+lat_company = 59.395881
+long_company = 24.658980
+price_one = 200
+price_all = 500
+passwd = 'lost9'
+bin_empty = b'\xe2\x81\xa0\xe2\x81\xa0'  # .encode("utf-8")
+hex_empty = 'e281a0e281a0'  # .encode("utf-8").hex()  || bytes.fromhex()
+str_empty = bin_empty.decode('utf-8')
+
+
 SECTION = 'CONFIG'
 LINES_ON_PAGE = 5
 short_name = 'me'
 const_url = 'https://t.me/'
 phone_number = '79999999999'
 vk_group = 'https://vk.com'
 vk_account = 'https://vk.com'
@@ -142,18 +148,21 @@
 🇬🇧🇨🇳🇦🇪🇪🇸🇷🇸🇫🇷
 """
 
 markupAdmin = types.ReplyKeyboardMarkup(keyboard=[
     [types.KeyboardButton(text='⬅️ Prev'), types.KeyboardButton(text='↩️ Menu'),
      types.KeyboardButton(text='➡️️ Next')]], resize_keyboard=True, selective=True, row_width=3)
 
-BOT_VARS_ = '{"DATE_TIME": 0, "BOT_PROMO": "#911", "BOT_CHANNEL": 0, "BOT_CHANNELTID": 0, "BOT_GROUP": 0, "BOT_GROUPTID": 0, "BOT_TZ": 0}'
-BOT_LSTS_ = '{"ADMIN_USERS": [], "PREMIUM_USERS": [], "CHANNEL_USERS": [], "GROUP_USERS": [], "PROMO_USERS": [], "UTM_USERS": []}'
-USER_VARS_ = '{"USER_TEXT": "", "USER_PHONE": "", "USER_EMAIL": "", "USER_GEO": "", "USER_PROMO": "", "USER_QUIZ": 0, "USER_DICE": 0, "USER_PAY": 0, "USER_UTM": "", "USER_ID": 0, "USER_TZ": 0, "USER_LC": "", "USER_DT": "", "USER_ISADMIN": 0, "USER_ISPREMIUM": 0, "USER_BALL": 0, "USER_RAND": 0, "DATE_TIME": 0}'
+BOT_VARS_ = '{"BOT_PROMO": "#911", "BOT_CHANNEL": 0, "BOT_CHANNELTID": 0, "BOT_GROUP": 0, "BOT_GROUPTID": 0, "BOT_TZ": 0, "BOT_TZ": 0, "BOT_LZ": "en", "BOT_LC": "en"}'
+BOT_LSTS_ = '{"BOT_ADMINS": []}'
+USER_VARS_ = '{"USER_TEXT": "", "USER_EMAIL": "", "USER_PROMO": "", "USER_PHONE": "", "USER_GEO": "", "USER_UTM": "", "USER_ID": 0, "USER_DT": "", "USER_TZ": 0, "USER_LC": "en", "USER_ISADMIN": 0, "USER_ISPREMIUM": 0, "USER_BALL": 0, "USER_RAND": 0, "USER_QUIZ": 0, "USER_DICE": 0, "USER_PAY": 0, "DATE_TIME": 0}'
 USER_LSTS_ = '{"USER_UTMREF": []}'
+
+logger.add('debug.log', format="{time:DD-MM-YYYY HH:mm:ss} | {name}({line}): {message}", level="INFO",
+           colorize=True, enqueue=True, backtrace=True, diagnose=True, rotation="1 week")
 # endregion
 
 
 # region db
 def sqlite_lower(value_):
     return value_.lower() if value_ else None
 
@@ -314,15 +323,15 @@
             POST_ISSILENCE     BOOLEAN     DEFAULT 0,
             POST_ISGALLERY     BOOLEAN     DEFAULT 0,
 
             POST_STATUS        BOOLEAN     DEFAULT 0,
             POST_TZ            VARCHAR,
             POST_DT            VARCHAR
         )''')
-        
+
         # USER
         cur.execute(f'''CREATE TABLE IF NOT EXISTS USER ( 
             USER_ID         INTEGER     PRIMARY KEY AUTOINCREMENT
                                         UNIQUE
                                         NOT NULL,
             USER_TID        BIGINT      UNIQUE
                                         NOT NULL,
@@ -348,14 +357,16 @@
         con.commit()
         cur.close()
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
         con.close()
+
+
 # endregion
 
 
 # region menu
 async def post_offer(bot, data, BASE_D):
     try:
         for item in data:
@@ -491,20 +502,21 @@
                 post_dumps = json.dumps(content_json, ensure_ascii=False)
                 await telegraph_.edit_page(path=page_['path'], title=page_['title'], html_content=post_dumps)
                 return 1
         except Exception as e:
             if 'Flood control exceeded' in str(e):
                 try:
                     secs = int(str(e).split(' seconds')[0].split()[-1])
-                    if secs < 10: await asyncio.sleep(secs+1)
+                    if secs < 10: await asyncio.sleep(secs + 1)
                 except Exception as e:
                     logger.info(log_ % str(e))
                     await asyncio.sleep(round(random.uniform(1, 2), 2))
-            logger.info(log_ % str(e))
-            await asyncio.sleep(round(random.uniform(1, 2), 2))
+            else:
+                logger.info(log_ % str(e))
+                await asyncio.sleep(round(random.uniform(1, 2), 2))
         finally:
             retry -= 1
     return 0
 
 
 async def tgph_clear(access_token, url):
     retry = 2
@@ -692,43 +704,45 @@
                 page = await telegraph_.get_page(path=item['path'], return_content=True, return_html=False)
                 try:
                     content_json = json.loads(str(page['content'][0]))
                 except:
                     content_json = {}
 
                 for OFFER_USERTID, v in content_json.items():
-                        OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_BUTTON, OFFER_ISBUTTON, OFFER_TGPHLINK, \
-                            OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, \
-                            OFFER_DT, OFFER_TZ = v
-
-                        sql = "INSERT OR IGNORE INTO OFFER (OFFER_USERTID, OFFER_TEXT, OFFER_MEDIATYPE, " \
-                              "OFFER_FILEID, OFFER_BUTTON, OFFER_ISBUTTON, OFFER_TGPHLINK, OFFER_ISTGPH, " \
-                              "OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, OFFER_DT, " \
-                              "OFFER_TZ) VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)"
-                        await db_change(sql, (int(OFFER_USERTID), v[OFFER_TEXT], v[OFFER_MEDIATYPE],
-                                              v[OFFER_FILEID], v[OFFER_BUTTON], v[OFFER_ISBUTTON],
-                                              v[OFFER_TGPHLINK], v[OFFER_ISTGPH], v[OFFER_ISSPOILER],
-                                              v[OFFER_ISPIN], v[OFFER_ISSILENCE], v[OFFER_ISGALLERY],
-                                              v[OFFER_DT], v[OFFER_TZ],), BASE_D)
-
-                        del content_json[str(OFFER_USERTID)]
-                        post_dumps = json.dumps(content_json, ensure_ascii=False)
-                        await telegraph_.edit_page(path=item['path'], title=access_key, html_content=post_dumps)
-                        return
+                    OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_BUTTON, OFFER_ISBUTTON, OFFER_TGPHLINK, \
+                        OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, \
+                        OFFER_DT, OFFER_TZ = v
+
+                    sql = "INSERT OR IGNORE INTO OFFER (OFFER_USERTID, OFFER_TEXT, OFFER_MEDIATYPE, " \
+                          "OFFER_FILEID, OFFER_BUTTON, OFFER_ISBUTTON, OFFER_TGPHLINK, OFFER_ISTGPH, " \
+                          "OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, OFFER_DT, " \
+                          "OFFER_TZ) VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)"
+                    await db_change(sql, (int(OFFER_USERTID), v[OFFER_TEXT], v[OFFER_MEDIATYPE],
+                                          v[OFFER_FILEID], v[OFFER_BUTTON], v[OFFER_ISBUTTON],
+                                          v[OFFER_TGPHLINK], v[OFFER_ISTGPH], v[OFFER_ISSPOILER],
+                                          v[OFFER_ISPIN], v[OFFER_ISSILENCE], v[OFFER_ISGALLERY],
+                                          v[OFFER_DT], v[OFFER_TZ],), BASE_D)
+
+                    del content_json[str(OFFER_USERTID)]
+                    post_dumps = json.dumps(content_json, ensure_ascii=False)
+                    await telegraph_.edit_page(path=item['path'], title=access_key, html_content=post_dumps)
+                    return
             except Exception as e:
                 if 'Flood control exceeded' in str(e):
                     await run_shell(f'/usr/bin/pm2 restart {bot_username}')
                 logger.info(log_ % str(e))
                 await asyncio.sleep(round(random.uniform(0, 1), 2))
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
+
+
 # endregion
 
 
 # region admin
 async def pre_upload(bot, chat_id, media_name, media_type, EXTRA_D, BASE_D):
     result = None
     try:
@@ -1039,20 +1053,26 @@
             text = yeref.l_broadcast_start[lz].format(duration)
             await bot.send_message(chat_id, text, parse_mode=ParseMode.HTML)
         all_len = len(user_ids)
         max_size = 20  # 1
         # max_size = 1  # 1
         fact_len = 0
 
+        sql = "SELECT OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_FILEIDNOTE, OFFER_BUTTON, OFFER_ISBUTTON, " \
+              "OFFER_TGPHLINK, OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, " \
+              "OFFER_DT FROM OFFER WHERE OFFER_ID=?"
+        data = await db_select(sql, (offer_id,), BASE_D)
+        if not len(data): return
+
         while True:
             try:
                 random.shuffle(user_ids)
                 await asyncio.sleep(0.05)
                 tmp_user_ids = [user_ids.pop() for _ in range(0, max_size) if len(user_ids)]
-                coroutines = [send_user(bot, tmp_user_id, offer_id, BASE_D) for tmp_user_id in tmp_user_ids]
+                coroutines = [send_user(bot, tmp_user_id, offer_id, data[0]) for tmp_user_id in tmp_user_ids]
                 results = await asyncio.gather(*coroutines)
 
                 for result in results:
                     if result:
                         fact_len += 1
 
                 if not len(user_ids): break
@@ -1072,24 +1092,19 @@
         text = yeref.l_broadcast_finish[lz].format(fact_len)
         await bot.send_message(chat_id, text, parse_mode=ParseMode.HTML)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
-async def send_user(bot, chat_id, offer_id, BASE_D, message_id=None, current=1):
+async def send_user(bot, chat_id, offer_id, item, message_id=None, current=1):
     result = None
     try:
-        sql = "SELECT OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_FILEIDNOTE, OFFER_BUTTON, OFFER_ISBUTTON, " \
-              "OFFER_TGPHLINK, OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, " \
-              "OFFER_DT FROM OFFER WHERE OFFER_ID=?"
-        data = await db_select(sql, (offer_id,), BASE_D)
-        if not len(data): return
         OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_FILEIDNOTE, OFFER_BUTTON, OFFER_ISBUTTON, OFFER_TGPHLINK, \
-            OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, OFFER_DT = data[0]
+            OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, OFFER_DT = item
 
         len_ = 1
         if OFFER_ISBUTTON:
             reply_markup = await create_replymarkup2(bot, offer_id, OFFER_BUTTON, 'ofr')
         else:
             reply_markup = InlineKeyboardBuilder()
 
@@ -1592,15 +1607,15 @@
                 await state.set_state(FsmOffer.text)
             else:
                 text = yeref.l_post_button[lz].replace('XXXXX', message.chat.username) if message.chat.username else \
                     yeref.l_post_button[lz].replace('XXXXX', '')
                 await bot.send_message(chat_id, text)
                 await state.set_state(FsmOffer.button)
         else:
-            file_name = file_name_part = file_id = file_id_note = file_type = offer_tgph_link = None
+            file_name = file_name_part = file_id = file_id_note = file_type = None
             if message.text:
                 await bot.send_message(chat_id=chat_id, text=yeref.l_post_media[lz])
                 return
             elif message.photo:
                 file_id = message.photo[-1].file_id
                 file_name_part = f"{datetime.datetime.utcnow().strftime('%d-%m-%Y_%H-%M-%S-%f.jpg')}"
                 file_name = os.path.join(MEDIA_D, file_name_part)
@@ -2006,19 +2021,31 @@
         message_id = call.message.message_id
         data, option, offer_id, current, len_ = call.data.split("_")
         offer_id = int(offer_id)
         current = int(current)
         len_ = int(len_)
 
         if option == 'prev':
+            sql = "SELECT OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_FILEIDNOTE, OFFER_BUTTON, OFFER_ISBUTTON, " \
+                  "OFFER_TGPHLINK, OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, " \
+                  "OFFER_DT FROM OFFER WHERE OFFER_ID=?"
+            data = await db_select(sql, (offer_id,), BASE_D)
+            if not len(data): return
+
             current = len_ if current == 1 and option == 'prev' else current - 1
-            await send_user(bot, chat_id, offer_id, BASE_D, message_id, current)
+            await send_user(bot, chat_id, offer_id, data[0], message_id, current)
         elif option == 'next':
+            sql = "SELECT OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_FILEIDNOTE, OFFER_BUTTON, OFFER_ISBUTTON, " \
+                  "OFFER_TGPHLINK, OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, " \
+                  "OFFER_DT FROM OFFER WHERE OFFER_ID=?"
+            data = await db_select(sql, (offer_id,), BASE_D)
+            if not len(data): return
+
             current = 1 if current == len_ and option == 'next' else current + 1
-            await send_user(bot, chat_id, offer_id, BASE_D, message_id, current)
+            await send_user(bot, chat_id, offer_id, data[0], message_id, current)
         elif data[1] == 'current':
             pass
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
@@ -2177,15 +2204,16 @@
                                          reply_markup=reply_markup.as_markup())
         elif POST_MEDIATYPE == 'document':
             media = types.InputMediaDocument(media=POST_FILEID, caption=POST_TEXT)
             await bot.edit_message_media(media=media, chat_id=chat_id, message_id=message_id,
                                          reply_markup=reply_markup.as_markup())
         else:
             OFFER_FILEID = ast.literal_eval(POST_FILEID) if POST_FILEID and '[' in POST_FILEID else POST_FILEID
-            OFFER_MEDIATYPE = ast.literal_eval(POST_MEDIATYPE) if POST_MEDIATYPE and '[' in POST_MEDIATYPE else POST_MEDIATYPE
+            OFFER_MEDIATYPE = ast.literal_eval(
+                POST_MEDIATYPE) if POST_MEDIATYPE and '[' in POST_MEDIATYPE else POST_MEDIATYPE
 
             media = []
             for i in range(0, len(OFFER_FILEID)):
                 caption = POST_TEXT if i == 0 else None
 
                 if OFFER_MEDIATYPE[i] == 'photo':
                     media.append(
@@ -2202,14 +2230,15 @@
             await bot.send_media_group(chat_id, media)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
 
+
 # endregion
 
 
 # region functions
 async def run_shell(cmd):
     result = None
     try:
@@ -2234,15 +2263,15 @@
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
         return result
 
 
 def escape_md(*content, sep=" ") -> str:
     """
-    Escape markdown text
+    Escape Markdown text
 
     E.g. for usernames
 
     :param content:
     :param sep:
     :return:
     """
@@ -3106,15 +3135,16 @@
             try:
                 if v[0]:
                     if len(tmp) > 0 and tmp[-1] is None:
                         result.add(*buttons)
                         if 'ᴵ' in v[0]:
                             buttons = [types.InlineKeyboardButton(text=str(v[0]), switch_inline_query_current_chat='')]
                         elif str(v[1]).startswith("btn_"):
-                            buttons = [types.InlineKeyboardButton(text=str(v[0]), callback_data=f"btn_{type_}_{offer_id}_{k}")]
+                            buttons = [
+                                types.InlineKeyboardButton(text=str(v[0]), callback_data=f"btn_{type_}_{offer_id}_{k}")]
                         else:
                             buttons = [types.InlineKeyboardButton(text=str(v[0]), url=v[1])]
                     else:
                         if 'ᴵ' in v[0]:
                             buttons.append(
                                 types.InlineKeyboardButton(text=str(v[0]), switch_inline_query_current_chat=''))
                         elif str(v[1]).startswith("btn_"):
@@ -3331,15 +3361,15 @@
             for el in link:
                 if el not in string.ascii_letters + string.digits + "@_https://t.me/+ ":
                     link = link.replace(el, '')
         except Exception:
             pass
 
         result = link
-    except Exception:
+    except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
 
 
 def is_names(phrase):
@@ -4734,13 +4764,59 @@
 # apt install python3-certbot-nginx -y
 # certbot --nginx -d tg6001.YOURDOMAIN.com -d www.tg6001.YOURDOMAIN.com
 # carwellhobbot4@mail.ee, Agree, No, Redirect, True
 # certbot certificates
 # endregion
 
 
+# region payment
+async def update_subscribe(bot, BASE_D):
+    try:
+        dt_ = datetime.datetime.now()
+        if not (dt_.hour % 2 == 0 and dt_.minute % 2 == 0 and dt_.second % 2 == 0): return
+        sql = "SELECT USER_TID, USER_LZ, USER_PAYDT FROM USER WHERE USER_ISPAID=1"
+        data = await db_select(sql, (), BASE_D)
+
+        for item in data:
+            try:
+                await asyncio.sleep(round(random.uniform(0, 1), 2))
+                USER_TID, USER_LZ, USER_PAYDT = item
+                get_ = await bot.get_chat(chat_id=USER_TID)
+
+                if (dt_ - datetime.datetime.strptime(USER_PAYDT, '%d-%m-%Y_%H-%M-%S')).days > 32:
+                    chan_private_donate = channel_library_ru if USER_LZ == 'ru' else channel_library_en
+                    extra_bot = Bot(token=BOT_TOKEN_E18B)
+                    get_chat_member_ = await extra_bot.get_chat_member(chat_id=chan_private_donate, user_id=USER_TID)
+                    await extra_bot.session.close()
+
+                    if get_chat_member_.status in ['member', 'administrator', 'creator']:
+                        USER_PAYDT = datetime.datetime.utcnow().strftime('%d-%m-%Y_%H-%M-%S')
+                        sql = "UPDATE USER SET USER_ISPAID=1, USER_USERNAME=?, USER_FULLNAME=?, USER_PAYDT=? " \
+                              "WHERE USER_TID=?"
+                        await db_change(sql, (get_.username, get_.full_name, USER_PAYDT, USER_TID,), BASE_D)
+                    else:
+                        sql = "UPDATE USER SET USER_ISPAID=0, USER_USERNAME=?, USER_FULLNAME=? WHERE USER_TID=?"
+                        await db_change(sql, (get_.username, get_.full_name, USER_TID, ), BASE_D)
+                else:
+                    sql = "UPDATE USER SET USER_USERNAME=?, USER_FULLNAME=? WHERE USER_TID=?"
+                    await db_change(sql, (get_.username, get_.full_name, USER_TID,), BASE_D)
+            except TelegramRetryAfter as e:
+                logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
+                await asyncio.sleep(e.retry_after + 1)
+            except Exception as e:
+                logger.info(log_ % str(e))
+                await asyncio.sleep(round(random.uniform(0, 1), 2))
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
+        await asyncio.sleep(e.retry_after + 1)
+    except Exception as e:
+        logger.info(log_ % str(e))
+        await asyncio.sleep(round(random.uniform(0, 1), 2))
+# endregion
+
+
 def main():
     pass
 
 
 if __name__ == "__main__":
     main()
```

