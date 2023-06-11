# Comparing `tmp/libretrofuzz-3.0.9.tar.gz` & `tmp/libretrofuzz-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-3.0.9.tar", max compression
+gzip compressed data, was "libretrofuzz-3.1.0.tar", max compression
```

## Comparing `libretrofuzz-3.0.9.tar` & `libretrofuzz-3.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-11 01:54:38.443341 libretrofuzz-3.0.9/LICENSE
--rw-r--r--   0        0        0     7682 2023-06-11 01:54:38.443341 libretrofuzz-3.0.9/README.rst
--rw-r--r--   0        0        0       22 2023-06-11 01:54:38.443341 libretrofuzz-3.0.9/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    52994 2023-06-11 01:54:38.443341 libretrofuzz-3.0.9/libretrofuzz/__main__.py
--rw-r--r--   0        0        0     1275 2023-06-11 01:54:38.443341 libretrofuzz-3.0.9/pyproject.toml
--rw-r--r--   0        0        0     8859 2023-06-11 01:54:49.294640 libretrofuzz-3.0.9/setup.py
--rw-r--r--   0        0        0     8870 2023-06-11 01:54:49.295549 libretrofuzz-3.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-11 21:39:20.654725 libretrofuzz-3.1.0/LICENSE
+-rw-r--r--   0        0        0     7682 2023-06-11 21:39:20.654725 libretrofuzz-3.1.0/README.rst
+-rw-r--r--   0        0        0       22 2023-06-11 21:39:20.654725 libretrofuzz-3.1.0/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    53731 2023-06-11 21:39:20.658726 libretrofuzz-3.1.0/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0     1275 2023-06-11 21:39:20.658726 libretrofuzz-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8859 2023-06-11 21:39:34.919724 libretrofuzz-3.1.0/setup.py
+-rw-r--r--   0        0        0     8870 2023-06-11 21:39:34.920838 libretrofuzz-3.1.0/PKG-INFO
```

### Comparing `libretrofuzz-3.0.9/LICENSE` & `libretrofuzz-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.0.9/README.rst` & `libretrofuzz-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.0.9/libretrofuzz/__main__.py` & `libretrofuzz-3.1.0/libretrofuzz/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,14 +249,25 @@
         elif not paren_level:
             result += ch
     if paren_level != 0:
         error(f"'{input_str}' has a unclosed parenthesis")
     return result
 
 
+def extractbefore(name, before):
+    if before:
+        # Ignore metadata and get the string before it
+        name_without_meta = regex.search(r"(^[^\[({]*)", name)
+        if name_without_meta:
+            before_index = name_without_meta.group(1).find(before)
+            if before_index != -1:
+                return name[0:before_index]
+    return name
+
+
 def replacemany(our_str, to_be_replaced, replace_with):
     for nextchar in to_be_replaced:
         our_str = our_str.replace(nextchar, replace_with)
     return our_str
 
 
 def removefirst(name: str, suf: str):
@@ -280,51 +291,51 @@
 
 
 # -------------------------------------------------------------------
 # The heart of the program, what orders titles to be 'more similar'
 # or less to the local labels (after the normalization)
 # -------------------------------------------------------------------
 class TitleScorer(object):
-    def __init__(self, subtitles, other_subtitles):
+    def __init__(self, normcache, normcache2):
         # rapidfuzz says to use range 0-100, but this doesn't (it's much easier that way)
         # so it uses internal api to prevent a possible early exit at == 100
         self._RF_ScorerPy = {
             "get_scorer_flags": lambda **kwargs: {
                 "optimal_score": MAX_SCORE,
                 "worst_score": 0,
                 "flags": (1 << 6),
             }
         }
-        self.subtitles = subtitles
-        self.other_subtitles = other_subtitles
+        self.normcache = normcache
+        self.normcache2 = normcache2
 
-    def check_full_match(self, name, other_name):
-        if name == other_name:
+    def __call__(self, name, other, processor=None, score_cutoff=None):
+        if name == other:
             return 200
-        name_ns = "".join(name.split())
-        if name_ns == "".join(other_name.split()):
+        (_, name_ns, _, _) = self.normcache[name]
+        (_, other_ns, other_subs, other_ns_subs) = self.normcache2[other]
+        if name_ns == other_ns:
             return 200
-        candidates = []
-        other_subs = self.other_subtitles[other_name]
         # If a playlist has 'other name' that means 'other name' is
         # a perfect match to another game on the playlist.
-        # that probably means it's not the right game
-        perfect_for_another = 0.1 if other_name in self.subtitles else 0
-        if len(other_subs) > 1:
-            for sub in other_subs:
-                if name == sub or name_ns == "".join(sub.split()):
-                    candidates.append(200 - perfect_for_another)
-                else:
-                    candidates.append(fuzz.token_ratio(name, sub) - perfect_for_another)
-        candidates.append(fuzz.token_ratio(name, other_name) - perfect_for_another)
+        # That probably means it's not the right game.
+        if other in self.normcache or other_ns in self.normcache:
+            perfect_for_another = 0.1
+        else:
+            perfect_for_another = 0
+        candidates = []
+        for sub, sub2 in zip(other_subs, other_ns_subs):
+            if name == sub or name_ns == sub2:
+                candidates.append(200 - perfect_for_another)
+                break
+            else:
+                candidates.append(fuzz.token_ratio(name, sub) - perfect_for_another)
+        candidates.append(fuzz.token_ratio(name, other) - perfect_for_another)
         return max(candidates)
 
-    def __call__(self, s1, s2, processor=None, score_cutoff=None):
-        return self.check_full_match(s1, s2)
-
 
 # ---------------------------------------------------------------
 # Normalization functions, part of the functions that change both
 # local labels and remote names to be more similar to compare
 # ---------------------------------------------------------------
 # word splitter regex, wont even attempt to explain how and why
 camelcase_pattern = regex.compile(
@@ -350,14 +361,15 @@
     # but may occur in the local name. Do this before camelcase
     # split because its hard to do a regex that allows splitting
     # Word-Word or Word:Word without creating new subtitle
     # and removing articles from subtitles is helpful anyway
     subtitles = t.split(" - ")
     if len(subtitles) == 1:
         subtitles = t.split(": ")
+    subtitles2 = [None] * len(subtitles)
     for i, st in enumerate(subtitles):
         # remove all symbols, except, ',' and '''
         # this needs to be here for all the names
         # to be operating on the same base for definite articles
         st = regex.sub(almost_symbols_pattern, "", st)
         # CamelCaseNames for local labels are common when there are no spaces
         # do this to normalize for definite articles
@@ -425,15 +437,16 @@
         st = st.replace("ix", "9")
         st = st.replace("x", "10")
         st = st.replace("i", "1")
         # remove diacritics (not to asian languages diacritics, only for 2 to 1 character combinations)
         st = "".join([c for c in unicodedata.normalize("NFKD", st) if not unicodedata.combining(c)])
         st = st.strip().split()
         subtitles[i] = " ".join(st)
-    return " ".join(subtitles), subtitles
+        subtitles2[i] = "".join(st)
+    return " ".join(subtitles), "".join(subtitles2), subtitles, subtitles2
 
 
 # ---------------------------------------------------------------------------------
 # Initalization functions, since there are two main programs so the code is reused
 # ---------------------------------------------------------------------------------
 class RzipReader(object):
     """used to abstract the libretro compressed playlist format"""
@@ -958,57 +971,56 @@
     # since no mixed matches are allowed
     # (until you call again without --no-merge anyway)
     remote_names = set()
     remote_names.update(thumbs.Named_Boxarts.keys(), thumbs.Named_Titles.keys(), thumbs.Named_Snaps.keys())
 
     # preprocess data to build a heuristic later. Do not move
     # into the later loop because thats when the heuristic is used
-    subtitles1 = dict()
-    subtitles2 = dict()
-    mappings1 = dict()
-    mappings2 = dict()
-    for x in remote_names:
-        normstr, lst = norm(x)
-        subtitles2[normstr] = lst
-        mappings1[x] = normstr
-    remote_names = mappings1
-    # this loop is used to build a heuristic explained in titlescorer (dont merge it)
+    normcache = dict()
+    # nonetheless save the normalization to not be forced to redo it
     for name, _ in names:
-        name = regex.sub(forbidden, "_", name)
-        norm_name = name
-        if before:
-            # Ignore metadata and get the string before it
-            name_without_meta = regex.search(r"(^[^\[({]*)", norm_name)
-            if name_without_meta:
-                before_index = name_without_meta.group(1).find(before)
-                if before_index != -1:
-                    norm_name = norm_name[0:before_index]
-
-        (norm_name, namesubs) = norm(norm_name)
-        subtitles1[norm_name] = namesubs
-        mappings2[name] = norm_name
-
-    title_scorer = TitleScorer(subtitles1, subtitles2)
-
+        # done before the forbidden removal because the 'before' str might have '_'
+        norm_name = extractbefore(name, before)
+        # this is the character that libretro-thumbnails uses as placeholder
+        norm_name = regex.sub(forbidden, "_", norm_name)
+        normtuple = norm(norm_name)
+        # cache normalization with all the name variants checked
+        # reason is to be able to reuse the calculation (name)
+        normcache[name] = normtuple  # original
+        # check if server names are equal to playlist normalized variants
+        normcache[normtuple[0]] = normtuple  # normalized
+        normcache[normtuple[1]] = normtuple  # normalized nospace
+    tmpdict = dict()
+    normcache2 = dict()
+    for x in remote_names:
+        normtuple = norm(x)
+        normcache2[normtuple[0]] = normtuple  # normalized only
+        tmpdict[x] = normtuple[0]
+    remote_names = tmpdict
+    scorer = TitleScorer(normcache, normcache2)
     for name, destination in names:
         await asyncio.sleep(0)  # update key status
         checkEscape()  # check key status
         # if the user used filters, filter everything that doesn't match any of the globs
         if filters and not any(map(lambda x: fnmatch.fnmatch(name, x), filters)):
             continue
-        # only the local names should have forbidden characters
-        name = regex.sub(forbidden, "_", name)
-        nameaux = mappings2[name]
+        # cached normalized name
+        nameaux = normcache[name][0]
         # normalization can make it so that the winner has the same score as the runner up(s)
-        result = process.extract(nameaux, remote_names, scorer=title_scorer, limit=verbose or 2)
+        # so try in several versions (to prevent this use '--verbose 1')
+        # improves results because spaces or case errors happen in the server
+        result = process.extract(nameaux, remote_names, scorer=scorer, limit=verbose or 2)
         assert result and len(result) > 0
         _, max_score, _ = result[0]
         winners = [x for x in result if x[1] == max_score and x[1] >= score]
         show = result if verbose else winners
         name_format = style((nameaux if short_names else name) + ": ", bold=True)
+        # still remove the forbidden characters
+        # the name will be used in the filename
+        name = regex.sub(forbidden, "_", name)
         if winners:
             allow = True
             # these parent directories were created when reading the playlist
             # more efficient than doing it a playlist game loop
             real_thumb_dir = Path(thumbnails_dir, destination)
             down_thumb_dir = Path(tmpdir, destination)
             if not filters and nomerge:
@@ -1047,15 +1059,15 @@
                 )
                 try:
                     for dirname in Thumbs._fields:
                         real = Path(real_thumb_dir, dirname, name + ".png")
                         temp = Path(down_thumb_dir, dirname, name + ".png")
                         downloaded_dict[dirname] = (real, temp)
                         for winner in winners:
-                            t_norm, t_score, t_name = winner
+                            _, t_score, t_name = winner
                             # something to download
                             url = getattr(thumbs, dirname).get(t_name, None)
                             if not url:
                                 continue
 
                             # with filters/reset you always download, and
                             # without only if it doesn't exist already.
@@ -1126,15 +1138,15 @@
             checkDownload()
             await asyncio.sleep(0.1)
 
 
 def strfy(required_score, short_names, nub_verbose, r, urlsdict=None):
     thumb_norm, thumb_score, thumb_name = r
     score_color = RED if thumb_score < required_score else GREEN
-    thumb_magnt = f"{thumb_score:.6f}" if short_names else f"{thumb_score:.2f}"
+    thumb_magnt = f"{thumb_score:.4f}" if short_names else f"{thumb_score:.1f}"
     score_text = style(thumb_magnt, fg=score_color, bold=True)
     if nub_verbose:
         return f"{score_text} {thumb_norm}"
     elif urlsdict:
         url1 = urlsdict.get((Thumbs._fields[0], r), None)
         url2 = urlsdict.get((Thumbs._fields[1], r), None)
         url3 = urlsdict.get((Thumbs._fields[2], r), None)
```

### Comparing `libretrofuzz-3.0.9/pyproject.toml` & `libretrofuzz-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "3.0.9"
+version = "3.1.0"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-3.0.9/setup.py` & `libretrofuzz-3.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '3.0.9',
+    'version': '3.1.0',
     'description': 'Fuzzy Retroarch thumbnail downloader',
     'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (require exact matches after the standard heuristics). If you still want more thumbnails, using ``libretro-fuzz --min 100 --delay 5 --delay 5`` works (lowering ``--min`` increases fuzz), with some delays introduced before and after downloading to check if you want to keep the game selected for the thumbnails.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-merge --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before`` and ``--no-meta``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=30]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=30]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100=fuzzy match, 200=equal,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose N           | Show length N list: score, name, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
```

### Comparing `libretrofuzz-3.0.9/PKG-INFO` & `libretrofuzz-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 3.0.9
+Version: 3.1.0
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

