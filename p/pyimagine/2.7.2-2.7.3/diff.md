# Comparing `tmp/pyimagine-2.7.2.tar.gz` & `tmp/pyimagine-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyimagine-2.7.2.tar", last modified: Fri Jun  9 12:19:28 2023, max compression
+gzip compressed data, was "pyimagine-2.7.3.tar", last modified: Sun Jun 11 13:06:28 2023, max compression
```

## Comparing `pyimagine-2.7.2.tar` & `pyimagine-2.7.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 12:19:28.354823 pyimagine-2.7.2/
--rw-rw-rw-   0        0        0    35823 2023-06-09 12:07:02.000000 pyimagine-2.7.2/LICENSE
--rw-rw-rw-   0        0        0     3729 2023-06-09 12:19:28.354823 pyimagine-2.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     2813 2023-06-09 12:19:13.000000 pyimagine-2.7.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 12:19:28.322123 pyimagine-2.7.2/pyimagine/
--rw-rw-rw-   0        0        0       66 2023-06-09 12:17:55.000000 pyimagine-2.7.2/pyimagine/__init__.py
--rw-rw-rw-   0        0        0    44556 2023-06-09 12:16:08.000000 pyimagine-2.7.2/pyimagine/constants.py
--rw-rw-rw-   0        0        0      240 2023-06-09 12:07:02.000000 pyimagine-2.7.2/pyimagine/exceptions.py
--rw-rw-rw-   0        0        0     1504 2023-06-09 12:07:02.000000 pyimagine-2.7.2/pyimagine/utils.py
--rw-rw-rw-   0        0        0     7587 2023-06-09 12:07:02.000000 pyimagine-2.7.2/pyimagine/vyroai.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:19:28.346735 pyimagine-2.7.2/pyimagine.egg-info/
--rw-rw-rw-   0        0        0     3729 2023-06-09 12:19:28.000000 pyimagine-2.7.2/pyimagine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-06-09 12:19:28.000000 pyimagine-2.7.2/pyimagine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 12:19:28.000000 pyimagine-2.7.2/pyimagine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-09 12:19:28.000000 pyimagine-2.7.2/pyimagine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-09 12:19:28.000000 pyimagine-2.7.2/pyimagine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 12:19:28.354823 pyimagine-2.7.2/setup.cfg
--rw-rw-rw-   0        0        0     1230 2023-06-09 12:17:55.000000 pyimagine-2.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:19:28.346735 pyimagine-2.7.2/test/
--rw-rw-rw-   0        0        0     1911 2023-06-09 12:07:02.000000 pyimagine-2.7.2/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-11 13:06:28.571336 pyimagine-2.7.3/
+-rw-rw-rw-   0        0        0    35823 2023-06-11 13:02:08.000000 pyimagine-2.7.3/LICENSE
+-rw-rw-rw-   0        0        0     3729 2023-06-11 13:06:28.571336 pyimagine-2.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2813 2023-06-11 13:06:15.000000 pyimagine-2.7.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 13:06:28.555709 pyimagine-2.7.3/pyimagine/
+-rw-rw-rw-   0        0        0       66 2023-06-11 13:04:23.000000 pyimagine-2.7.3/pyimagine/__init__.py
+-rw-rw-rw-   0        0        0    44443 2023-06-11 13:02:41.000000 pyimagine-2.7.3/pyimagine/constants.py
+-rw-rw-rw-   0        0        0      240 2023-06-11 13:02:08.000000 pyimagine-2.7.3/pyimagine/exceptions.py
+-rw-rw-rw-   0        0        0     1504 2023-06-11 13:02:08.000000 pyimagine-2.7.3/pyimagine/utils.py
+-rw-rw-rw-   0        0        0     7581 2023-06-11 13:03:54.000000 pyimagine-2.7.3/pyimagine/vyroai.py
+drwxrwxrwx   0        0        0        0 2023-06-11 13:06:28.571336 pyimagine-2.7.3/pyimagine.egg-info/
+-rw-rw-rw-   0        0        0     3729 2023-06-11 13:06:28.000000 pyimagine-2.7.3/pyimagine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-06-11 13:06:28.000000 pyimagine-2.7.3/pyimagine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 13:06:28.000000 pyimagine-2.7.3/pyimagine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-11 13:06:28.000000 pyimagine-2.7.3/pyimagine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-11 13:06:28.000000 pyimagine-2.7.3/pyimagine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 13:06:28.571336 pyimagine-2.7.3/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2023-06-11 13:04:23.000000 pyimagine-2.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 13:06:28.571336 pyimagine-2.7.3/test/
+-rw-rw-rw-   0        0        0     1911 2023-06-11 13:02:08.000000 pyimagine-2.7.3/test/test.py
```

### Comparing `pyimagine-2.7.2/LICENSE` & `pyimagine-2.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyimagine-2.7.2/PKG-INFO` & `pyimagine-2.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimagine
-Version: 2.7.2
+Version: 2.7.3
 Summary: Python library for AI-powered image manipulation.
 Home-page: https://github.com/hyugogirubato/pyimagine
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: art,image,ai,stable-diffusion
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyimagine-2.7.2/README.md` & `pyimagine-2.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pyimagine-2.7.2/pyimagine/constants.py` & `pyimagine-2.7.3/pyimagine/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # Generated by the firebase web compiler.  DO NOT EDIT!
 # source: firebase.py
 
 from enum import Enum
 
 # Banned
-BANNED_WORDS = ['erotism', 'bitches', 'neonazi', 'menstral', 'felch', 'masturbating', 'cum', 'tushy', 'fucktards', 'gore', 'bukkake', 'nipples', 'deapthroating', 'gloryhole', 'quim', 'dick', 'cunt', 'nawashi', 'pussy', 'clitoris', 'squirting', 'deep-throating', 'slut', 'tube8', 'tit', 'breast', 'breasts', 'faggot', 'spunk', 'crucified', 'grope', 'bareback', 'spooge', 'booty', 'doggie style', 'doggy style', 'emetophilia', 'adult film', 'tranny', 'flesh', 'ballgag', 'licking', 'cornhole', 'threesome', 'dong', 'cialis', 'pedobear', 'voyeurweb', 'pornhab', 'pornhub', 'oppai', 'schlong', 'shrimping', 'succubus', 'scissoring', 'asshat', 'bastard', 'skimpy', 'boudoir', 'badonkers', 'asslover', 'erections', 'ponyplay', 'pornography', 'orgasm', 'dickhead', 'orgie', 'adult video', 'hardcore', 'butt', 'poontang', 'pornstar', 'sexting', 'scantily', 'pornagraphy', 'viagra', 'deep thraoting', 'semen', 'sucking', 'hentai', 'big ass', 'sexy female', 'kike', 'yaoi', 'invisible clothes', 'foreskin', 'boobies', 'no shirt', 'zero clothes', 'penis', 'sexual', 'erotica', 'nymphomania', 'beastiality', 'babeland', 'ejaculation', 'penis', 'sexuality', 'asshore', 'jizz', 'glory hole', 'nude', 'doggiestyle', 'shit', 'gay', 'fetish', 'nazi', 'genitals', 'cocks', 'pus', 'hardcore', 'shemale', 'bitch', 'zoophilia', 'nipple', 'frotting', 'poop', 'pisspig', 'torture', 'carpetmuncher', 'handjob', 'anus', 'corpse', 'shibari', 'pornhub', 'assmunch', 'circlejerk', 'penetration', 'buttcheeks', 'femdom', 'cock ring', 'sucks', 'fisting', 'nigger', 'jerk off', 'rule34', 'nympho', 'cuck-old', 'contraceptive', 'asslicker', 'cum-shot', 'hentai', 'nipple', 'fart', 'bondage', 'dendrophilia', 'fucker', 'ovaries', 'asses', 'assjockey', 'homoerotic', 'hooker', '2g1c', 'yiff', 'fingering', 'nambla', 'bdsm', 'clunge', 'barely dressed', 'pussyboy', 'nsfw', 'asswipe', 'cumming', 'pubes', 'sodomy', 'menstrual', 'butthole', 'pissing', 'fascist', 'nutten', 'sodomize', 'pthc', 'titties', 'bimbos', 'transman', 'tits', 'make out', 'vagina', 'clusterfuck', 'assfuck', 'fuckin', 'assman', 'twink', 'kinkster', 'erection', 'blumpkin', 'slaughter', 'bodily fluids', 'pegging', 'voyuer', 'orgy', 'dingleberry', 'bbw', 'jerk', 'topless', 'asskisser', 'dominatrix', 'cowgirl', 'sexually', 'booty', 'deep-throat', 'thot', 'naked', 'knobbing', 'cuck', 'hard-on', 'felching', 'deepthroat', 'poop', 'fucking', 'doggystyle', 'wank', 'bisexual', 'assmuncher', 'urophilia', 'milf', 'suck', 'undressing', 'dommes', 'gangbang', 'twerk', 'bigass', 'cleavage', 'vaginamen', 'dick', 'condom', 's&m', 'figging', 'strapon', 'punany', 'lgbt', 'cunnilingus', 'masturbate', 'hermaphrodite', 'cumshots', 'pedophile', 'deepthroating', 'daterape', 'smallpussy', 'livesex', 'barely legal', 'gay', 'nudity', 'incest', 'deep-thraoting', 'deap throating', 'busty', 'voluptuous', 'thumbzilla', 'boob', 'youporn', 'bangbus', 'moan', 'throating', 'crotch', 'erotic', 'fucked', 'coprophilia', 'missionary', 'rimming', 'deep throat', 'nymphomania', 'tribadism', 'arse', 'succubus', 'arsehole', 'deepthraoting', 'femdon', 'splooge', 'asskiss', 'poopchute', 'gokkun', 'zoophilia', 'cuckold', 'disturbing', 'transsexual', 'voluptuous', 'surgery', 'asspacker', 'asslick', 'no clothes', 'playboy', 'fag', 'dildo', 'deap-throating', 'milking', 'fudgepacker', 'oral', 'coon', 'bruises', 'playboy', 'autoerotic', 'female body parts', 'voyeur', 'footjob', 'bung', 'assmonkey', 'rapist', 'g-spot', 'menstraul', 'masturbation', 'ass', 'erotic', 'jerking off', 'jerk', 'jerking', 'panty', 'ass', 'anilingus', 'brown pudding', 'phallus', 'noclothes', 'octopussy', 'asswhore', 'badfuck', 'labia', 'anus', 'bdsm', 'hooters', 'assholes', 'porn', 'wearing nothing', 'bestiality', 'ahegao', 'bullshit', 'slavegirl', 'farts', 'fellatio', 'cannibal', 'clit', 'inappropriate', 'shitty', 'warts', 'queef', 'squirt', 'sperm', 'acrotomophilia', 'porno', 'piercing', 'hardon', 'assklown', 'massacre', 'deep-thraot', 'asshole', 'muffdiving', 'deep thraot', 'facesitting', 'kinbaku', 'strap-on', 'lesbian', 'vagina', 'queaf', 'sultry', 'raping', 'creampie', 'strappado', 'xxx', 'infant nudity', 'tryphophobia', 'brothel', 'crucifixion', 'lgbtq', 'perv', 'titty', 'anal', 'dirty', 'cleaver', 'shota', 'pervert', 'cannibalism', 'shit', 'jigaboo', 'rectum', 'lovemaking', 'towelhead', 'urethra', 'bastinado', 'camgirl', 'vulva', 'barenaked', 'omorashi', 'bollocks', 'tubgirl', 'deapthroat', 'rimjob', 'cock', 'rape', 'cucked', 'asspirate', 'blowjob', 'jiggerboo', 'bosom', 'mammaries', 'sugar daddy', 'minge', 'feltch', 'bulldyke', 'sultry', 'whore', 'testicles', 'xx', 'camwhore', 'motherfucker', 'booba', 'deap-throat', 'breasts', 'sperm', 'bondage', 'kinky', 'xxx', 'cumshot', 'boobys', 'ecchi', 'sex', 'juggs', 'asspuppies', 'boobs', 'fuck', 'upskirt', 'busty', 'horny', 'menpussy', 'transgender', 'deep throating', 'nimphomania', 'deap throat', 'bang', 'piss', 'bangbros', 'prophet', 'milfs', 'sexcam', 'butt plug', 'doggy style', 'intercourse', 'fucks', 'voyeurism', 'headed', 'dolcett']
+BANNED_WORDS = ['erotism', 'bitches', 'neonazi', 'menstral', 'felch', 'masturbating', 'cum', 'tushy', 'fucktards', 'gore', 'bukkake', 'nipples', 'deapthroating', 'gloryhole', 'quim', 'dick', 'cunt', 'nawashi', 'pussy', 'clitoris', 'squirting', 'deep-throating', 'slut', 'tube8', 'tit', 'breast', 'breasts', 'faggot', 'spunk', 'crucified', 'grope', 'bareback', 'spooge', 'booty', 'doggie style', 'doggy style', 'emetophilia', 'adult film', 'tranny', 'flesh', 'ballgag', 'licking', 'cornhole', 'threesome', 'dong', 'cialis', 'pedobear', 'voyeurweb', 'pornhab', 'pornhub', 'oppai', 'schlong', 'shrimping', 'succubus', 'scissoring', 'asshat', 'bastard', 'skimpy', 'boudoir', 'badonkers', 'asslover', 'erections', 'ponyplay', 'pornography', 'orgasm', 'dickhead', 'orgie', 'adult video', 'hardcore', 'butt', 'poontang', 'pornstar', 'sexting', 'scantily', 'pornagraphy', 'viagra', 'deep thraoting', 'semen', 'sucking', 'hentai', 'big ass', 'sexy female', 'kike', 'yaoi', 'invisible clothes', 'foreskin', 'boobies', 'no shirt', 'zero clothes', 'penis', 'sexual', 'erotica', 'nymphomania', 'beastiality', 'babeland', 'ejaculation', 'penis', 'sexuality', 'asshore', 'jizz', 'glory hole', 'nude', 'doggiestyle', 'shit', 'gay', 'fetish', 'nazi', 'genitals', 'cocks', 'pus', 'hardcore', 'shemale', 'bitch', 'zoophilia', 'nipple', 'frotting', 'poop', 'pisspig', 'torture', 'carpetmuncher', 'handjob', 'anus', 'corpse', 'shibari', 'pornhub', 'assmunch', 'circlejerk', 'penetration', 'buttcheeks', 'femdom', 'cock ring', 'sucks', 'fisting', 'nigger', 'jerk off', 'rule34', 'nympho', 'cuck-old', 'contraceptive', 'asslicker', 'cum-shot', 'hentai', 'nipple', 'fart', 'bondage', 'dendrophilia', 'fucker', 'ovaries', 'asses', 'assjockey', 'homoerotic', 'hooker', '2g1c', 'yiff', 'fingering', 'nambla', 'bdsm', 'clunge', 'barely dressed', 'pussyboy', 'nsfw', 'asswipe', 'cumming', 'pubes', 'sodomy', 'menstrual', 'butthole', 'pissing', 'fascist', 'nutten', 'sodomize', 'pthc', 'titties', 'bimbos', 'transman', 'tits', 'make out', 'vagina', 'clusterfuck', 'assfuck', 'fuckin', 'assman', 'twink', 'kinkster', 'erection', 'blumpkin', 'slaughter', 'bodily fluids', 'pegging', 'voyuer', 'orgy', 'dingleberry', 'bbw', 'jerk', 'topless', 'asskisser', 'dominatrix', 'cowgirl', 'sexually', 'booty', 'deep-throat', 'thot', 'naked', 'knobbing', 'cuck', 'hard-on', 'felching', 'deepthroat', 'poop', 'fucking', 'doggystyle', 'wank', 'bisexual', 'assmuncher', 'urophilia', 'milf', 'suck', 'undressing', 'dommes', 'gangbang', 'twerk', 'bigass', 'cleavage', 'vaginamen', 'dick', 'condom', 's&m', 'figging', 'strapon', 'punany', 'lgbt', 'cunnilingus', 'masturbate', 'hermaphrodite', 'cumshots', 'pedophile', 'deepthroating', 'daterape', 'smallpussy', 'livesex', 'barely legal', 'gay', 'nudity', 'incest', 'deep-thraoting', 'deap throating', 'busty', 'voluptuous', 'thumbzilla', 'boob', 'youporn', 'bangbus', 'moan', 'throating', 'crotch', 'erotic', 'fucked', 'coprophilia', 'missionary', 'rimming', 'deep throat', 'nymphomania', 'tribadism', 'arse', 'succubus', 'arsehole', 'deepthraoting', 'femdon', 'splooge', 'asskiss', 'poopchute', 'gokkun', 'zoophilia', 'cuckold', 'disturbing', 'transsexual', 'voluptuous', 'surgery', 'asspacker', 'asslick', 'no clothes', 'playboy', 'fag', 'dildo', 'deap-throating', 'milking', 'fudgepacker', 'oral', 'coon', 'bruises', 'playboy', 'autoerotic', 'female body parts', 'voyeur', 'footjob', 'bung', 'assmonkey', 'rapist', 'g-spot', 'menstraul', 'masturbation', 'ass', 'erotic', 'jerking off', 'jerk', 'jerking', 'panty', 'ass', 'anilingus', 'brown pudding', 'phallus', 'noclothes', 'octopussy', 'asswhore', 'badfuck', 'labia', 'anus', 'bdsm', 'hooters', 'assholes', 'porn', 'wearing nothing', 'bestiality', 'ahegao', 'bullshit', 'slavegirl', 'farts', 'fellatio', 'cannibal', 'clit', 'inappropriate', 'shitty', 'warts', 'queef', 'squirt', 'sperm', 'acrotomophilia', 'porno', 'piercing', 'hardon', 'assklown', 'massacre', 'deep-thraot', 'asshole', 'muffdiving', 'deep thraot', 'facesitting', 'kinbaku', 'strap-on', 'lesbian', 'vagina', 'queaf', 'sultry', 'raping', 'creampie', 'strappado', 'xxx', 'infant nudity', 'tryphophobia', 'brothel', 'crucifixion', 'lgbtq', 'perv', 'titty', 'anal', 'dirty', 'cleaver', 'shota', 'pervert', 'cannibalism', 'shit', 'jigaboo', 'rectum', 'lovemaking', 'towelhead', 'urethra', 'bastinado', 'camgirl', 'vulva', 'barenaked', 'omorashi', 'bollocks', 'tubgirl', 'deapthroat', 'rimjob', 'cock', 'rape', 'cucked', 'asspirate', 'blowjob', 'jiggerboo', 'bosom', 'mammaries', 'sugar daddy', 'minge', 'feltch', 'bulldyke', 'sultry', 'whore', 'testicles', 'xx', 'camwhore', 'motherfucker', 'booba', 'deap-throat', 'breasts', 'sperm', 'bondage', 'kinky', 'xxx', 'cumshot', 'boobys', 'ecchi', 'sex', 'juggs', 'asspuppies', 'boobs', 'fuck', 'upskirt', 'busty', 'horny', 'menpussy', 'transgender', 'deep throating', 'nimphomania', 'deap throat', 'bang', 'piss', 'bangbros', 'prophet', 'milfs', 'sexcam', 'butt plug', 'doggy style', 'intercourse', 'fucks', 'voyeurism', 'dolcett']
 
 
 # KEY = (parameter, images, thumbnail)
 class Mode(Enum):
 	SCRIBBLE = ('scribble', 'assets/imageRemix_modes/scribble.webp', 'assets/imageRemix_modes/thumb_scribble.webp')
 	DEPTH = ('depth', 'assets/imageRemix_modes/depth.webp', 'assets/imageRemix_modes/thumb_depth.webp')
-	SEGMENTATION = ('seg', 'assets/imageRemix_modes/seg.webp', 'assets/imageRemix_modes/thumb_seg.webp')
 	OPEN_POSE = ('openpose', 'assets/imageRemix_modes/openpose.webp', 'assets/imageRemix_modes/thumb_openpose.webp')
 	CANNY = ('canny', 'assets/imageRemix_modes/canny.webp', 'assets/imageRemix_modes/thumb_canny.webp')
 
 
 # KEY = ratio
 class Ratio(Enum):
 	RATIO_1X1 = "1:1"
```

### Comparing `pyimagine-2.7.2/pyimagine/utils.py` & `pyimagine-2.7.3/pyimagine/utils.py`

 * *Files identical despite different names*

### Comparing `pyimagine-2.7.2/pyimagine/vyroai.py` & `pyimagine-2.7.3/pyimagine/vyroai.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self.restricted = restricted
         self.api = "https://inferenceengine.vyro.ai"
         self.cdn = "https://1966211409.rsc.cdn77.org/appStuff/imagine-fncisndcubnsduigfuds"
         self.version = 1
 
     def _request(self, **kwargs) -> Response:
         headers = {"accept": "*/*", "user-agent": "okhttp/4.10.0"}
-        headers.update(kwargs.get("headers", None) or {})
+        headers.update(kwargs.get("headers") or {})
 
         data = clear_dict(kwargs.get("data"))
         if data:
             prompt = data.get("prompt", "").lower().split(" ")
             if prompt:
                 for i, word in enumerate(prompt):
                     word = re.sub(r'[^a-zA-Z]', "", word)
```

### Comparing `pyimagine-2.7.2/pyimagine.egg-info/PKG-INFO` & `pyimagine-2.7.3/pyimagine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimagine
-Version: 2.7.2
+Version: 2.7.3
 Summary: Python library for AI-powered image manipulation.
 Home-page: https://github.com/hyugogirubato/pyimagine
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: art,image,ai,stable-diffusion
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyimagine-2.7.2/setup.py` & `pyimagine-2.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pyimagine",
-    version="2.7.2",
+    version="2.7.3",
     author="hyugogirubato",
     author_email="hyugogirubato@gmail.com",
     description="Python library for AI-powered image manipulation.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/hyugogirubato/pyimagine",
     packages=find_packages(),
```

### Comparing `pyimagine-2.7.2/test/test.py` & `pyimagine-2.7.3/test/test.py`

 * *Files identical despite different names*

