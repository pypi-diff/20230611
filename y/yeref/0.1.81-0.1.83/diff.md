# Comparing `tmp/yeref-0.1.81.tar.gz` & `tmp/yeref-0.1.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.81.tar", last modified: Sun Jun 11 13:21:30 2023, max compression
+gzip compressed data, was "yeref-0.1.83.tar", last modified: Sun Jun 11 15:06:02 2023, max compression
```

## Comparing `yeref-0.1.81.tar` & `yeref-0.1.83.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 13:21:30.844330 yeref-0.1.81/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 13:21:30.844572 yeref-0.1.81/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-11 13:21:30.845502 yeref-0.1.81/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-11 13:21:03.000000 yeref-0.1.81/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 13:21:30.836755 yeref-0.1.81/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.81/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   535217 2023-06-11 12:46:53.000000 yeref-0.1.81/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   212328 2023-06-11 13:20:55.000000 yeref-0.1.81/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 13:21:30.843347 yeref-0.1.81/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 13:21:30.000000 yeref-0.1.81/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-11 13:21:30.000000 yeref-0.1.81/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-11 13:21:30.000000 yeref-0.1.81/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-11 13:21:30.000000 yeref-0.1.81/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:06:02.109545 yeref-0.1.83/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 15:06:02.109783 yeref-0.1.83/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-11 15:06:02.110845 yeref-0.1.83/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-11 15:03:29.000000 yeref-0.1.83/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:06:02.102001 yeref-0.1.83/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.83/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   552493 2023-06-11 15:03:29.000000 yeref-0.1.83/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   212331 2023-06-11 13:59:57.000000 yeref-0.1.83/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-11 15:06:02.108867 yeref-0.1.83/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-11 15:06:02.000000 yeref-0.1.83/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-11 15:06:02.000000 yeref-0.1.83/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-11 15:06:02.000000 yeref-0.1.83/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-11 15:06:02.000000 yeref-0.1.83/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.81/setup.py` & `yeref-0.1.83/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.81',
+      version='0.1.83',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.1.81/yeref/l_.py` & `yeref-0.1.83/yeref/l_.py`

 * *Files 2% similar despite different names*

```diff
@@ -940,21 +940,29 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_demo_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>проекта</code> <b>Ferey</b>:\n\n▪️<b>информация</b> обо всех проектах\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>проекта</code> <b>Ferey</b>:\n\n▪️<b>информация</b> обо всех проектах\n\n❗️Регулярно-обновляемый /content",
     'en': "🌱 {0}, welcome to <i>the landing bot</i> of the <b>Ferey</b> <code>проекта</code> :\n\n▪️ <b>information</b> about all projects\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del <code>проекта</code> <b>Ferey</b> :\n\n▪️ <b>información</b> sobre todos los proyectos\n\n❗️ también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du <code>проекта</code> <b>Ferey</b> :\n\n▪️ <b>informations</b> sur tous les projets\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
     'zh': "🌱 {0}，欢迎来到<b>Ferey</b> <code>проекта</code>的<i>落地机器人</i>：\n\n▪️ 所有项目的<b>信息</b>\n\n❗️ 您也可以在我们的Ferey工作室订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص <code>проекта</code> <b>Ferey</b> :\n\n▪️ <b>معلومات</b> حول جميع المشاريع\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
+l_subscribe_demo = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
 
 l_kind_1 = {
     'ru': "<b>👩🏽‍💻@FereyDemoBot</b>\n\n<b>Демо</b> бот всех проектов",
     'en': "<b>👩🏽‍💻</b> <b>@FereyDemoBot</b>\n\nDemo bot of all projects",
     'es': "<b>👩🏽‍💻</b> <b>@FereyDemoBot</b>\n\nBot de demostración de todos los proyectos",
     'fr': "<b>👩🏽‍💻</b> <b>@FereyDemoBot</b>\n\nDemo bot de tous les projets",
     'zh': "<b>👩🏽‍💻</b> <b>@FereyDemoBot</b>\n\n所有项目的演示机器人",
@@ -1081,21 +1089,30 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_work_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>проекта</code> <b>Ferey</b>:\n\n▪️<b>вакансии</b> нашего стартапа\n▪️конкурсы и <b>мероприятия</b>\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>проекта</code> <b>Ferey</b>:\n\n▪️<b>вакансии</b> нашего стартапа\n▪️конкурсы и <b>мероприятия</b>\n\n❗️Регулярно-обновляемый /content",
     'en': "🌱 {0}, welcome to <i>the landing bot</i> of the <b>Ferey</b> <code>проекта</code> :\n\n▪️ <b>vacancies</b> of our startup\n▪️ contests and <b>events</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del <code>проекта</code> <b>Ferey</b> :\n\n▪️ <b>vacantes</b> de nuestra startup\n▪️ concursos y <b>eventos</b>\n\n❗️ también puedes encargar el desarrollo de un chat bot en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du <code>проекта</code> <b>Ferey</b> :\n\n▪️ <b>offres d&#x27;emploi</b> de notre startup\n▪️ concours et <b>événements</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
     'zh': "🌱 {0}，欢迎来到<b>Ferey</b> <code>проекта</code>的<i>登陆机器人</i>：\n\n▪️ 我们初创公司的<b>职位空缺</b>\n▪️ 竞赛和<b>活动</b>\n\n❗️ 您也可以在我们的Ferey工作室订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> <code>проекта</code> <b>Ferey</b> :\n\n▪️ <b>الشواغر</b> في بدء التشغيل\n▪️ المسابقات <b>والأحداث</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey",
 }
+l_subscribe_work = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
+
 l_vacancy_1 = {
     'ru': "👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company",
     'en': "👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company",
     'es': "👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTareas: crear máscaras ferey (video realista) para cualquier humano\nGénero: niña\nEdad: menos de 30\nPago: parte de la empresa",
     'fr': "👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTâches : créer des masques de ferey (vidéo réaliste) pour tout humain\nSexe : fille\nÂge : moins de 30 ans\nPaiement : part de l'entreprise",
     'zh': "👩🏽‍💻<b>文本到视频 ai-designer</b>\n\n任务：为任何人创建 ferey-mask（逼真的视频）\n性别：女孩\n年龄：30 岁以下\n薪酬：公司股份",
     'ar': "👩🏽‍💻 <b>نص إلى فيديو مصمم ai</b>\n\nالمهام: إنشاء أقنعة ضيقة (فيديو واقعي) لأي إنسان\nالجنس: فتاة\nالعمر: أقل من 30\nالدفع: حصة الشركة",
@@ -1133,21 +1150,30 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_ai_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>генерации</code> контента:\n\n▪️<b>текст</b>\n▪️<b>изображение</b>\n▪️<b>анализ Telegram-канала</b>\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для <code>генерации</code> контента:\n\n▪️<b>текст</b>\n▪️<b>изображение</b>\n▪️<b>анализ Telegram-канала</b>\n▪️<b>распознавание</b> речи\n▪️<b>очистка истории</b> /start\n\n❗️Регулярно-обновляемый /content",
     'en': "🌱 {0}, welcome to the content <code>генерации</code> <i>landing bot</i> :\n\n▪️ <b>text</b>\n▪️ <b>image</b>\n▪️ <b>analysis of the Telegram channel</b>\n\n❗️ you can also order the development of a chat bot in our studio Ferey",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> <code>генерации</code> de contenido :\n\n▪️ <b>texto</b>\n▪️ <b>imagen</b>\n▪️ <b>análisis del canal de Telegram</b>\n\n❗️ también puedes encargar el desarrollo de un chat bot en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue dans le <i>landing bot</i> <code>генерации</code> de contenu :\n\n▪️ <b>texte</b>\n▪️ <b>image</b>\n▪️ <b>analyse de la chaîne Telegram</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
     'zh': "🌱 {0}，欢迎使用内容<code>генерации</code><i>登陆机器人</i>：\n\n▪️<b>文字</b>\n▪️<b>图片</b>\n▪️ <b>Telegram 频道分析</b>\n\n❗️ 您也可以在我们的工作室Ferey订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت إنشاء</i> <code>генерации</code> :\n\n▪️ <b>نص</b>\n▪️ <b>صورة</b>\n▪️ <b>تحليل قناة Telegram</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
+l_subscribe_ai = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️отсутствие <b>режима ожидания</b>\n▪️аналитика постов канала\n(<i>+финансовый потенциал</i>)\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
+
 l_gen_txt = {
     'ru': "📘 Текст{0}",
     'en': "📘 Text{0}",
     'es': "📘 Texto{0}",
     'fr': "📘 Texte{0}",
     'zh': "📘 文字{0}",
     'ar': "📘 نص {0}",
@@ -1241,21 +1267,30 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_ads_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для создания креативных <code>постов</code> <b>Ferey</b>\n\n▪️️реклама во всех Ferey-ботах\n▪️️заказ рекламы на канале\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для создания креативных <code>постов</code> <b>Ferey</b>\n\n▪️️реклама во всех Ferey-ботах\n▪️️заказ рекламы на канале\n\n❗️Регулярно-обновляемый /content",
     'en': "🌱 {0}, welcome to <i>the landing bot</i> for creating creative <code>постов</code> <b>Ferey</b>\n\n▪️️advertising in all Ferey bots\n▪️️ ordering advertising on the channel\n\n❗️you can also order the development of a chat bot in our Ferey studio",
     'es': "🌱 {0}, bienvenido <i>al bot de aterrizaje</i> para crear <code>постов</code> creativas <b>Ferey</b>\n\n▪️️publicidad en todos los bots de Ferey\n▪️️solicitando publicidad en el canal\n\n❗️también puedes ordenar el desarrollo de un chatbot en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue dans <i>le bot de débarquement</i> pour la création <code>постов</code> créatives <b>Ferey</b>\n\n▪️️publicité dans tous les bots Ferey\n▪️️commande de publicité sur la chaîne\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
     'zh': "🌱 {0}，欢迎来到<b>Ferey</b>创建创意<code>постов</code>的<i>登陆机器人</i>\n\n▪️️在所有 Ferey 机器人中投放广告\n▪️️ 在频道订购广告\n\n❗️您也可以在以下订购聊天机器人的开发我们的Ferey工作室",
     'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> لإنشاء <code>постов</code> إبداعية <b>Ferey</b>\n\nالإعلان في جميع برامج Ferey\n▪️️ طلب الإعلانات على القناة\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
+l_subscribe_ads = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [Донат на баланс]:\n▪️возможность сделать рассылку в боте\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
+
 l_post_media_ads = {
     'ru': "✏️ 2. Прикрепи <b>медиа</b> контент: фото/гиф/видео до 5Mb\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
     'en': "✏️ 2. Attach <b>media</b> content: photo/gif/video up to 5Mb\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
     'es': "✏️ 2. Adjunte contenido <b>multimedia</b> : foto/gif/video de hasta 5 Mb\n\n( <i>o presione &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
     'fr': "✏️ 2. Joignez du contenu <b>multimédia</b> : photo/gif/vidéo jusqu&#x27;à 5 Mb\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
     'zh': "✏️ 2.附加<b>媒体</b>内容：照片/gif/视频最大5Mb\n\n（<i>或按“➡️️/Next”跳过此步骤</i>）",
     'ar': "✏️ 2. إرفاق محتوى <b>وسائط</b> : صورة / صورة / فيديو بحجم يصل إلى 5 ميغا بايت\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
@@ -1277,21 +1312,29 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_post_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для создания креативных <code>постов</code> <b>Ferey</b>\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для создания креативных <code>постов</code> <b>Ferey</b>\n▪️инлайн-<b>телескопы</b>\n▪️<b>уведомления</b> о нажатиях\n\n❗️Регулярно-обновляемый /content",
     'en': "🌱 {0}, welcome to <i>the landing bot</i> for creating creative <code>постов</code> <b>Ferey</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> para crear <code>постов</code> creativas <b>Ferey</b>\n\n❗️también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> pour créer <code>постов</code> créatifs <b>Ferey</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
     'zh': "🌱 {0}，欢迎使用<b>Ferey</b>创建创意<code>постов</code>的<i>登陆机器人</i>\n\n❗️ 您也可以在我们的Ferey工作室订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> لإنشاء <code>постов</code> إبداعية <b>Ferey</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
+l_subscribe_post = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>уведомления</b> о нажатиях\n(<i>ссылка на пользователя</i>)\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
 
 # endregion
 
 
 # region FereyVPNBot
 l_vpn_btn1 = {
     'ru': "⛰️ VPN",
@@ -1306,21 +1349,30 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_vpn_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> проекта Ferey:\n\n▪️<b>openvpn</b>\n▪️<b>wireguard</b>\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> проекта Ferey:\n\n▪️<b>openvpn</b>\n▪️<b>wireguard</b>\n\n❗️Регулярно-обновляемый /content",
     'en': "🌱 {0}, welcome to <i>the landing bot</i> of the Ferey project:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del proyecto Ferey:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ también puedes encargar el desarrollo de un chat bot en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du projet Ferey :\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
     'zh': "🌱 {0}，欢迎来到 Ferey 项目的<i>落地机器人</i>：\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص بمشروع Ferey:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey",
 }
+l_subscribe_vpn = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
+
 l_vpn_1 = {
     'ru': "👩🏽‍💻 <b>Open VPN</b>\n\n{0}",
     'en': "👩🏽‍💻 <b>Open VPN</b>\n\n{0}",
     'es': "👩🏽‍💻 <b>Abrir VPN</b>\n\n{0}",
     'fr': "👩🏽‍💻 <b>Ouvrez le VPN</b>\n\n{0}",
     'zh': "👩🏽‍💻<b>打开 VPN</b>\n\n{0}",
     'ar': "👩🏽‍💻 <b>افتح VPN</b>\n\n{0}",
@@ -1350,21 +1402,30 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_tools_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> Telegram-<code>инструментов</code>:\n\n▪️<b>преобразование</b> контента\n▪️<b>получение</b> информации о сообщении\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> Telegram-<code>инструментов</code>:\n\n▪️<b>преобразование</b> контента\n▪️<b>получение</b> информации о сообщ\n▪️<b>удаление</b> фона\n▪️<b>конвертация</b> в телескопы\n▪️<b>сообщение</b> 0-длины\n\n❗️Регулярно-обновляемый /content",
     'en': "🌱 {0}, welcome to <i>the landing bot</i> of Telegram <code>инструментов</code> :\n\n▪️ content <b>conversion</b>\n▪️ <b>getting</b> information about the message\n\n❗️you can also order the development of a chat bot in our studio Ferey",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> de <code>инструментов</code> de Telegram:\n\n▪️ <b>conversión</b> de contenido\n▪️ <b>obtener</b> información sobre el mensaje\n\n❗️también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue dans <i>le landing bot</i> des <code>инструментов</code> Telegram :\n\n▪️ <b>conversion</b> de contenu\n▪️ <b>obtenir</b> des informations sur le message\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
     'zh': "🌱 {0}，欢迎使用 Telegram <code>инструментов</code>的<i>登陆机器人</i>：\n\n▪️ 内容<b>转换</b>\n▪️<b>获取</b>有关消息的信息\n\n❗️您也可以在我们的工作室Ferey订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص <code>инструментов</code> Telegram:\n\n▪️ <b>تحويل</b> المحتوى\n▪️ <b>الحصول على</b> معلومات حول الرسالة\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
+l_subscribe_tools = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
+
 l_image_text = {
     'ru': "👩🏽‍💻 <b>Выбери</b> инструменты для преобразования <i>изображения</i> в",
     'en': "👩🏽‍💻 <b>Choose</b> tools to convert <i>your image</i> to",
     'es': "👩🏽‍💻 <b>Elija</b> herramientas para convertir <i>su imagen</i> a",
     'fr': "👩🏽‍💻 <b>Choisissez</b> des outils pour convertir <i>votre image</i> en",
     'zh': "👩🏽‍💻<b>选择</b>将<i>图像</i>转换为的工具",
     'ar': "👩🏽‍💻 <b>اختر</b> أدوات لتحويل <i>صورتك</i> إلى",
@@ -1887,21 +1948,29 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_media_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>медиа</code>-заметок:\n\n▪️<b>стикеры</b> из текста и фото\n▪️<b>аудио-звуки</b>\n▪️<b>видео-заметки</b>\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>медиа</code>-заметок:\n\n▪️<b>стикеры</b> из текста и фото\n▪️<b>аудио-тренды</b>\n▪️<b>видео-заметки</b>\n▪️инлайн-<b>телескопы</b>\n▪️<b>кнопочные</b> премиум-заметки\n\n❗️Регулярно-обновляемый /content",
     'en': "🌱 {0}, welcome to <i>the landing bot of</i> <code>медиа</code> notes:\n\n▪️ <b>stickers</b> from text and photos\n▪️ <b>audio sounds</b>\n▪️ <b>video notes</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
     'es': "🌱 {0}, bienvenido <i>al bot de aterrizaje de</i> notas <code>медиа</code> :\n\n▪️ <b>pegatinas</b> de texto y fotos\n▪️ <b>sonidos de audio</b>\n▪️ <b>notas de video</b>\n\n❗️ también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue dans <i>le bot de débarquement des</i> notes <code>медиа</code> :\n\n▪️ <b>autocollants</b> à partir de textes et de photos\n▪️ <b>sons audio</b>\n▪️ <b>notes vidéo</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
     'zh': "🌱 {0}，欢迎来到<code>медиа</code>笔记<i>的登陆机器人</i>：\n\n▪️文字和照片的<b>贴纸</b>\n▪️<b>音频声音</b>\n▪️<b>视频笔记</b>\n\n❗️您也可以在我们的Ferey工作室",
     'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الأساسي</i> لملاحظات <code>медиа</code> :\n\n▪️ <b>ملصقات</b> من النصوص والصور\n▪️ <b>الأصوات الصوتية</b>\n▪️ <b>ملاحظات الفيديو</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت الدردشة في استوديو Ferey الخاص بنا",
 }
+l_subscribe_media = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>кнопочные</b> премиум-заметки\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
 
 l_media_text = {
     'ru': "👩🏽‍💻 <b>Здесь</b> можно выбрать тип выпадающих media-заметок (/add | /del)",
     'en': "👩🏽‍💻 <b>Here</b> you can select the type of drop-down media notes (/add | /del)",
     'es': "👩🏽‍💻 <b>Aquí</b> puede seleccionar el tipo de notas multimedia desplegables (/add | /del)",
     'fr': "👩🏽‍💻 <b>Ici,</b> vous pouvez sélectionner le type de notes multimédia déroulantes (/add | /del)",
     'zh': "👩🏽‍💻<b>在这里</b>可以选择下拉媒体备注的类型（/add | /del）",
@@ -2059,14 +2128,23 @@
     'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>поиска</code> в <b>Telegram</b>:\n\n▪️<b>top</b> каналы/группы\n▪️<b>vip</b> пользователи/боты\n▪️<b>гео</b> парсинг\n▪️<b>пассивный</b> маркетинг\n\n❗️также можно заказать разработку Telegram-продвижения в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
     'en': "🌱 {0}, welcome to <b>Telegram</b> <code>поиска</code> <i>landing bot</i> :\n\n▪️ <b>top</b> channels/groups\n▪️ <b>vip</b> users/bots\n▪️ <b>geo</b> parsing\n▪️ <b>passive</b> marketing\n\n❗️ you can also order development Telegram promotions in our Ferey studio",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> <code>поиска</code> <b>de Telegram</b> :\n\n▪️ canales/grupos <b>principales</b>\n▪️ usuarios <b>vip</b> /bots\n▪️ análisis <b>geográfico</b>\n▪️ marketing <b>pasivo</b>\n\n❗️ también puedes solicitar promociones de desarrollo de Telegram en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue sur <b>Telegram</b> <code>поиска</code> <i>landing bot</i> :\n\n▪️ <b>meilleurs</b> canaux/groupes\n▪️ utilisateurs/bots <b>vip</b>\n▪️ analyse <b>géographique</b>\n▪️ marketing <b>passif</b>\n\n❗️ vous pouvez également commander des promotions de développement Telegram dans notre atelier de Ferey",
     'zh': "🌱 {0}，欢迎使用<b>Telegram</b> <code>поиска</code><i>登陆机器人</i>：\n\n▪️<b>热门</b>频道/群组\n▪️ <b>vip</b>用户/机器人\n▪️<b>地理</b>解析\n▪️<b>被动</b>营销\n\n❗️ 您也可以订购开发 Telegram 促销在我们的Ferey工作室",
     'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوطي</i> <code>поиска</code> <b>Telegram</b> :\n\n▪️ <b>أفضل</b> القنوات / المجموعات\n▪️ مستخدمين / برامج تتبع <b>لكبار</b> الشخصيات\n▪️ تحليل <b>جغرافي</b>\n▪️ تسويق <b>سلبي</b>\n\n❗️ يمكنك أيضًا طلب ترويجات Telegram للتطوير في استوديو Ferey الخاص بنا",
 }
+l_subscribe_find = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>уведомления</b> об услуге\n(<i>ссылка на сообщение</i>)\n▪️<b>приоритетная</b> выдача при поиске\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
+
 l_geo_minus = {
     'ru': "-",
     'en': "-",
     'es': "-",
     'fr': "-",
     'zh': "-",
     'ar': "-",
@@ -2841,21 +2919,30 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_chn_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>администрирования</code> <b>Telegram</b>-каналов:\n\n▪️<b>защита</b> канала от вступления шпионов\n▪️вывод <b>статистики</b> и вовлеченности (%)\n▪️ограничение прав до <b>подписки</b> на канал\n▪️<b>организация</b> бана и антифлуда\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>администрирования</code> <b>Telegram</b>-каналов:\n\n▪️<b>защита</b> канала от вступления шпионов\n▪️<b>организация</b> бана и антифлуда\n▪️<b>сбор</b> подписчиков\n▪️<b>счетчик</b> нажатий\n▪️<b>реакции</b> и просмотры\n\n❗️Регулярно-обновляемый /content",
     'en': "🌱 {0}, welcome to the <b>Telegram</b> channel <code>администрирования</code> <i>landing bot</i> :\n\n▪️ <b>protection</b> of the channel from spyware entry\n▪️display <b>of statistics</b> and engagement (%)\n▪️restriction of rights before <b>subscribing</b> to the channel\n▪️ <b>organization</b> of a ban and anti-flood\n\n❗️you can also order the development of a chat bot in our Ferey studio",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> <code>администрирования</code> de canales <b>de Telegram</b> :\n\ <b>n▪️protección</b> del canal contra la entrada de software espía\n▪️visualización <b>de estadísticas</b> e interacción (%)\n▪️restricción de derechos antes de <b>suscribirse</b> al canal\n▪️ <b>organización</b> de una prohibición y anti-inundación\n\n❗️también puedes encargar el desarrollo de un chatbot en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue dans le <i>landing bot</i> <code>администрирования</code> de la chaîne <b>Telegram</b> :\n\n▪️ <b>protection</b> de la chaîne contre l&#x27;entrée de logiciels espions\n▪️affichage <b>des statistiques</b> et de l&#x27;engagement (%)\n▪️restriction des droits avant de <b>s&#x27;abonner</b> à la chaîne\n<b>▪️organisation</b> d'une interdiction et anti-flood\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio de Ferey",
     'zh': "🌱 {0}，欢迎使用<b>Telegram</b>频道<code>администрирования</code><i>登陆机器人</i>：\n\n▪️<b>保护</b>频道免受间谍软件入侵\n▪️ 显示<b>统计信息</b>和参与度 (%)\n▪️<b>订阅</b>频道前的权利限制\n▪️<b>组织</b>禁令和反洪水\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت</i> <code>администрирования</code> قناة <b>Telegram</b> :\n\n▪️ <b>حماية</b> القناة من إدخال برامج التجسس\n▪️ <b>عرض الإحصائيات</b> والمشاركة (٪)\n▪️ تقييد الحقوق قبل <b>الاشتراك</b> في القناة\n▪️ <b>تنظيم</b> حظر ومكافحة الفيضانات\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
+l_subscribe_channel= {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>реакции</b> и просмотры\n▪️<b>выгрузка</b> базы пользователей\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
+
 l_add_chn_text = {
     'ru': "👮🏽‍♀️ <b>Добавь</b> @{0}-бота как  <b>Administrator</b> через настройки своего канала: ‹👤Add Admin›\n\n👮🏽‍♀️ <b>Опция</b> [✅ Назначение администраторов] позволит сделать парсинг старых пользователей, даже если в канале более 200 пользователей",
     'en': "👮🏽‍♀️ <b>Add</b> @{0}-bot as <b>an Administrator</b> via your channel settings: ‹👤Add Admin›\n\n👮🏽‍♀️ The [✅ Assign Admins] <b>option</b> will allow you to parse old users, even if there are more than 200 users in the channel",
     'es': "👮🏽‍♀️ <b>Agregue</b> @{0}-bot como <b>administrador</b> a través de la configuración de su canal: ‹👤Agregar administrador›\n\n👮🏽‍♀️ La <b>opción</b> [✅ Asignar administradores] le permitirá analizar usuarios antiguos, incluso si hay hay mas de 200 usuarios en el canal",
     'fr': "👮🏽‍♀️ <b>Ajoutez</b> @{0}-bot en tant <b>qu&#x27;administrateur</b> via les paramètres de votre chaîne : ‹👤Add Admin›\n\n👮🏽‍♀️ L&#x27; <b>option</b> [✅ Assign Admins] vous permettra d'analyser les anciens utilisateurs, même s'il y a sont plus de 200 utilisateurs dans le canal",
     'zh': "👮🏽‍♀️ 通过您的频道设置将@{0}-bot<b>添加</b>为<b>管理员</b>：‹👤添加管理员›\n\n👮🏽‍♀️ [✅ 分配管理员]<b>选项</b>将允许您解析旧用户，即使有频道中有超过 200 个用户",
     'ar': "👮🏽‍♀️ <b>إضافة</b> @ {0} -bot <b>كمسؤول</b> عبر إعدادات القناة: ‹👤 إضافة مسؤول›\n\n👮🏽‍♀️ سيسمح لك <b>خيار</b> [✅ تعيين المسؤولين] بتحليل المستخدمين القدامى ، حتى لو كان هناك أكثر من 200 مستخدم في القناة",
@@ -3880,21 +3967,30 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_group_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>администрирования</code> <b>Telegram</b>-групп:\n\n▪️<b>защита</b> группы от вступления шпионов\n▪️вывод <b>статистики</b> и вовлеченности (%)\n▪️ограничение прав до <b>подписки</b> на канал\n▪️<b>организация</b> бана и антифлуда\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>администрирования</code> <b>Telegram</b>-групп:\n\n▪️<b>защита</b> группы от вступления шпионов\n▪️вывод <b>статистики</b> и вовлеченности (%)\n▪️ограничение прав до <b>подписки</b>\n▪️<b>организация</b> бана и антифлуда\n▪️<b>авто-ответы</b> и стоп-слова\n\n❗️Регулярно-обновляемый /content",
     'en': "🌱 {0}, welcome to <i>the landing bot</i> <code>администрирования</code> <b>Telegram</b> groups:\n\n▪️ <b>protecting</b> the group from spyware\n▪️displaying <b>statistics</b> and engagement (%)\n▪️restricting rights before <b>subscribing</b> to the channel\n▪️ <b>organizing</b> a ban and anti-flood\n\n❗️you can also order the development of a chat bot in our Ferey studio",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> <code>администрирования</code> grupos <b>de Telegram</b> :\n\ <b>n▪️proteger</b> al grupo de spyware\n▪️mostrar <b>estadísticas</b> e interacción (%)\n▪️restringir los derechos antes de <b>suscribirse</b> al canal\ <b>n▪️organizar</b> un prohibición y anti-inundación\n\n❗️también puede solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue dans <i>le landing bot</i> <code>администрирования</code> des groupes <b>Telegram</b> :\n\n▪️ <b>protéger</b> le groupe des spywares\n▪️afficher <b>les statistiques</b> et l&#x27;engagement (%)\n▪️restreindre les droits avant de <b>s&#x27;abonner</b> à la chaîne\n▪️ <b>organiser</b> un interdiction et anti-flood\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio de Ferey",
     'zh': "🌱 {0}，欢迎使用<code>администрирования</code> <b>Telegram</b>群组的<i>登陆机器人</i>：\n\n▪️<b>保护</b>群组免受间谍软件的侵害\n▪️ 显示<b>统计数据</b>和参与度 (%)\n▪️ 在<b>订阅</b>频道之前限制权利\n▪️<b>组织</b>一个ban 和 anti-flood\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوط</i> <code>администрирования</code> مجموعات <b>Telegram</b> :\n\n▪️ <b>حماية</b> المجموعة من برامج التجسس\n▪️ عرض <b>الإحصائيات</b> والمشاركة (٪)\n▪️ تقييد الحقوق قبل <b>الاشتراك</b> في القناة\n▪️ <b>تنظيم</b> الحظر ومكافحة الفيضانات\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
+l_subscribe_group = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>стоп-слова</b> без ограничений\n▪️<b>старт-слова</b> без ограничений\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
+
 l_add_group_text = {
     'ru': "👇🏽 <b>Жми</b> на ‹➕ Добавить группу›, чтобы добавить в свою группу (с настройками по ум) бота: @{0}\n\n👮🏽‍♀️ Или добавь бота как <b>Administrator</b> через настройки своей группы: ‹👤Add Admin›\n\n👮🏽‍♀️ Если не добавляется группа, то измени <b>Должность</b> (см. скрин)",
     'en': "👇🏽 <b>Click</b> on ‹➕ Add group› to add a bot to your group (with custom settings): @{0}\n\n👮🏽‍♀️ Or add a bot as <b>Administrator</b> through your group settings: ‹👤Add Admin›\n\n👮🏽‍♀️ If the group is not added, then change <b>the Position</b> (see screenshot)",
     'es': "👇🏽 <b>Haz clic</b> en ‹➕ Agregar grupo› para agregar un bot a tu grupo (con configuraciones personalizadas): @{0}\n\n👮🏽‍♀️ O agrega un bot como <b>administrador</b> a través de la configuración de tu grupo: ‹👤Agregar administrador›\n\n👮🏽‍♀️ Si el grupo no se agrega, cambie <b>la Posición</b> (ver captura de pantalla)",
     'fr': "👇🏽 <b>Cliquez</b> sur ‹➕ Ajouter un groupe› pour ajouter un bot à votre groupe (avec des paramètres personnalisés) : @{0}\n\n👮🏽‍♀️ Ou ajoutez un bot en tant <b>qu&#x27;administrateur</b> via les paramètres de votre groupe : ‹👤Ajouter un administrateur›\n\n👮🏽‍♀️ Si le groupe n&#x27;est pas ajouté, alors changez <b>la position</b> (voir capture d'écran)",
     'zh': "👇🏽<b>点击</b>‹➕添加组›将机器人添加到您的组（使用自定义设置）：@{0}\n\n👮🏽‍♀️或通过您的组设置将机器人添加为<b>管理员</b>：‹👤添加管理员›\n\n👮🏽‍♀️ 如果没有添加组，则更改<b>位置</b>（见截图）",
     'ar': "👇🏽 <b>انقر</b> فوق ‹➕ إضافة مجموعة› لإضافة روبوت إلى مجموعتك (بإعدادات مخصصة): @ {0}\n\n👮🏽‍♀️ أو أضف روبوتًا <b>كمسؤول</b> من خلال إعدادات مجموعتك: ‹👤 إضافة مسؤول›\n\n👮🏽‍♀️ إذا لم تتم إضافة المجموعة ، فقم بتغيير <b>الموضع</b> (انظر لقطة الشاشة)",
@@ -6222,15 +6318,15 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_bot_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>автоматизации</code> <b>Telegram</b>-ботов:\n\n▪️авто-постинг и <b>авто-перевод</b>\n▪️<b>авто-ответы</b> и оповещения\n▪️интеграции и платежи\n▪️пользователи и администраторы\n\n❗️также можно заказать разработку чат-бота в нашей <a href='https://t.me/{1}'>ferey</a>-студии",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>автоматизации</code> <b>Telegram</b>-ботов:\n\n▪️авто-постинг и <b>авто-перевод</b>\n▪️<b>авто-ответы</b> и оповещения\n▪️нейросети: графика и текст бота\n▪️интеграции и платежи\n\n❗️также можно заказать разработку чат-бота в нашей <a href='https://t.me/{1}'>ferey</a>-студии",
     'en': "🌱 {0}, welcome to the <b>Telegram</b> bot <code>автоматизации</code> <i>landing bot</i> :\n\n▪️auto-posting and <b>auto-translation</b>\n▪️ <b>auto-replies</b> and notifications\n▪️integrations and payments\n▪️users and administrators\n\n❗️You can also order the development of a chatbot in our ferey studio",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> <code>автоматизации</code> de bots <b>de Telegram</b> :\n\n▪️auto-publicación y <b>auto-traducción</b>\n▪️auto <b>-respuestas</b> y notificaciones\n▪️integraciones y pagos\n▪️usuarios y administradores\n\n❗️también puedes encargar el desarrollo de un chatbot en nuestro ferey studio",
     'fr': "🌱 {0}, bienvenue dans le <i>bot d&#x27;atterrissage</i> <code>автоматизации</code> du bot <b>Telegram</b> :\n\n▪️publication et <b>traduction automatiques</b>\n▪️ <b>réponses et notifications automatiques</b>\n▪️intégrations et paiements\n▪️utilisateurs et administrateurs\n\n❗️Vous pouvez également commander le développement d'un chatbot dans notre studio ferey",
     'zh': "🌱 {0}，欢迎使用<b>Telegram</b>机器人<code>автоматизации</code><i>登陆机器人</i>：\n\n▪️自动发布和<b>自动翻译</b>\n▪️<b>自动回复</b>和通知\n▪️集成和支付\n▪️用户和管理员\n\n❗️您也可以在我们的ferey工作室订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوط</i> <code>автоматизации</code> لروبوت <b>Telegram</b> :\n\n▪️ النشر التلقائي <b>والترجمة التلقائية</b>\n▪️ <b>الردود التلقائية</b> والإشعارات\n▪️ عمليات الدمج والمدفوعات\nالمستخدمون والمسؤولون\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو ferey الخاص بنا",
 }
 l_subscribe_bot = {
@@ -7519,7 +7615,31 @@
     'es': "Mensaje tranquilo",
     'fr': "Message silencieux",
     'zh': "悄悄话",
     'ar': "رسالة هادئة",
 }
 # endregion
 # endregion
+
+
+# region FereyUserBot
+l_subscribe_user = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>рассылка</b> пользователям\n▪️<b>экстра</b> бот\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
+# endregion
+
+
+# region FereyTargetBot
+l_subscribe_target = {
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [Донат на баланс]:\n▪️возможность сделать рассылку в боте\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
+# endregion
```

### Comparing `yeref-0.1.81/yeref/yeref.py` & `yeref-0.1.83/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 import yeref
 
 
 elly_a = 5900268983
 my_tid = 5491025132
 my_tids = [
     '5900268983',
-    '6283902226',
-    '6090677494',
+    '6179455648',
+    '6236215930',
 
     '5754810063',
     '5491025132',
     '5360564451',
     '6281795468',
 ]
 channel_library_ru = -1001484489131
@@ -4767,15 +4767,15 @@
 # certbot certificates
 # endregion
 
 
 # region payment
 async def update_subscribe(bot, BASE_D):
     try:
-        dt_ = datetime.datetime.now()
+        dt_ = datetime.datetime.utcnow()
         if not (dt_.hour % 2 == 0 and dt_.minute % 2 == 0 and dt_.second % 2 == 0): return
         sql = "SELECT USER_TID, USER_LZ, USER_PAYDT FROM USER WHERE USER_ISPAID=1"
         data = await db_select(sql, (), BASE_D)
 
         for item in data:
             try:
                 await asyncio.sleep(round(random.uniform(0, 1), 2))
```

