# Comparing `tmp/em_keyboard-3.9.0.tar.gz` & `tmp/em_keyboard-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Sun Jun 11 13:11:41 2023, max compression
```

## Comparing `em_keyboard-3.9.0.tar` & `em_keyboard-4.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/.coveragerc
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/.editorconfig
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/.flake8
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/RELEASING.md
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/tox.ini
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/.github/labels.yml
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/.github/release-drafter.yml
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/.github/renovate.json
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/.github/workflows/labels.yml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/.github/workflows/require-pr-label.yml
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/em/__init__.py
--rw-r--r--   0        0        0   175397 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/em/emoji-en-US.json
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/scripts/despacify.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/scripts/run_command.py
--rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/scripts/update-emojilib.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/tests/__init__.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/tests/test_em.py
--rw-r--r--   0        0        0   135718 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/em/emojis.json
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/.gitignore
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/LICENSE
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/NOTICE
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/README.md
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/pyproject.toml
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 em_keyboard-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/.coveragerc
+-rw-r--r--   0        0        0      313 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/.editorconfig
+-rw-r--r--   0        0        0       30 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/.flake8
+-rw-r--r--   0        0        0     1319 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      835 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/RELEASING.md
+-rw-r--r--   0        0        0      566 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/tox.ini
+-rw-r--r--   0        0        0     1785 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/.github/labels.yml
+-rw-r--r--   0        0        0      894 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      443 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/.github/renovate.json
+-rw-r--r--   0        0        0     1755 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      352 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      298 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1084 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      490 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1560 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      801 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/scripts/despacify.py
+-rw-r--r--   0        0        0      496 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/scripts/run_command.py
+-rwxr-xr-x   0        0        0      205 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/scripts/update-emojilib.sh
+-rw-r--r--   0        0        0     4507 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/src/em_keyboard/__init__.py
+-rw-r--r--   0        0        0   175264 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/src/em_keyboard/emoji-en-US.json
+-rw-r--r--   0        0        0   135636 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/src/em_keyboard/emojis.json
+-rw-r--r--   0        0        0        0 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     3934 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/tests/test_em.py
+-rw-r--r--   0        0        0      346 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/.gitignore
+-rw-r--r--   0        0        0      754 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/LICENSE
+-rw-r--r--   0        0        0     1086 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/NOTICE
+-rw-r--r--   0        0        0     2238 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/README.md
+-rw-r--r--   0        0        0     1682 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3706 2023-06-11 13:11:41.000000 em_keyboard-4.0.0/PKG-INFO
```

### Comparing `em_keyboard-3.9.0/.pre-commit-config.yaml` & `em_keyboard-4.0.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
-        args: [--py37-plus]
+        args: [--py38-plus]
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
-        args: [--target-version=py37]
 
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
-        additional_dependencies: [flake8-2020, flake8-implicit-str-concat]
+        additional_dependencies:
+          [flake8-2020, flake8-errmsg, flake8-implicit-str-concat]
 
   - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: python-check-blanket-noqa
+      - id: python-no-log-warn
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
-      - id: check-json
+      - id: check-case-conflict
       - id: check-merge-conflict
+      - id: check-json
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
         exclude: ^em/emojis.json$
       - id: trailing-whitespace
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.4.1
+    rev: 0.10.0
     hooks:
       - id: pyproject-fmt
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.10.1
+    rev: v0.13
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/tox-dev/tox-ini-fmt
-    rev: 0.5.2
+    rev: 1.3.0
     hooks:
       - id: tox-ini-fmt
 
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `em_keyboard-3.9.0/RELEASING.md` & `em_keyboard-4.0.0/RELEASING.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
       https://github.com/hugovk/em-keyboard/releases
 
 - [ ] Check next tag is correct, amend if needed
 
 - [ ] Publish release
 
 - [ ] Check the tagged
-      [GitHub Actions build](https://github.com/hugovk/em-keyboard/actions?query=workflow%3ADeploy)
+      [GitHub Actions build](https://github.com/hugovk/em-keyboard/actions/workflow/deploy.yml)
       has deployed to [PyPI](https://pypi.org/project/em-keyboard/#history)
 
 - [ ] Check installation:
 
 ```bash
 pip3 uninstall -y em-keyboard && pip3 install -U em-keyboard && em rocket
 ```
```

### Comparing `em_keyboard-3.9.0/tox.ini` & `em_keyboard-4.0.0/tox.ini`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [tox]
-envlist =
+requires =
+    tox>=4.2
+env_list =
     cli
     lint
-    py{py3, 312, 311, 310, 39, 38, 37}
-isolated_build = true
+    py{py3, 312, 311, 310, 39, 38}
 
 [testenv]
 extras =
     tests
 commands =
-    {envpython} -m pytest --cov em --cov tests --cov-report html --cov-report term --cov-report xml {posargs}
+    {envpython} -m pytest --cov em_keyboard --cov tests --cov-report html --cov-report term --cov-report xml {posargs}
 
 [testenv:cli]
 commands =
     em --help
     em --version
     em -s test
 
 [testenv:lint]
-passenv =
-    PRE_COMMIT_COLOR
 skip_install = true
 deps =
     pre-commit
+pass_env =
+    PRE_COMMIT_COLOR
 commands =
     pre-commit run --all-files --show-diff-on-failure
 
 [testenv:cog]
 skip_install = true
 deps =
     cogapp
```

### Comparing `em_keyboard-3.9.0/.github/labels.yml` & `em_keyboard-4.0.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `em_keyboard-3.9.0/.github/release-drafter.yml` & `em_keyboard-4.0.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `em_keyboard-3.9.0/.github/workflows/release-drafter.yml` & `em_keyboard-4.0.0/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `em_keyboard-3.9.0/.github/workflows/test.yml` & `em_keyboard-4.0.0/.github/workflows/test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["pypy-3.8", "3.7", "3.8", "3.9", "3.10", "3.11", "3.12-dev"]
+        python-version: ["pypy3.9", "3.8", "3.9", "3.10", "3.11", "3.12"]
         os: [windows-latest, macos-latest, ubuntu-latest]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
+          allow-prereleases: true
           cache: pip
           cache-dependency-path: pyproject.toml
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U wheel
```

### Comparing `em_keyboard-3.9.0/em/__init__.py` & `em_keyboard-4.0.0/src/em_keyboard/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,37 +11,31 @@
   - If all names provided map to emojis, the resulting emojis will be
     automatically added to your clipboard.
   - ✨ 🍰 ✨  (sparkles shortcake sparkles)
 """
 
 
 import argparse
+import importlib.metadata
 import itertools
 import json
 import os
 import random
 import re
 import sys
 
 try:
-    # Python 3.8+
-    import importlib.metadata as importlib_metadata
-except ImportError:
-    # Python 3.7 and lower
-    import importlib_metadata
-
-try:
     import pyperclip as copier
 except ImportError:
     try:
         import xerox as copier
     except ImportError:
         copier = None
 
-__version__: str = importlib_metadata.version("em_keyboard")
+__version__: str = importlib.metadata.version("em_keyboard")
 
 EMOJI_PATH = os.path.join(os.path.dirname(__file__), "emojis.json")
 CUSTOM_EMOJI_PATH = os.path.join(os.path.expanduser("~/.emojis.json"))
 
 
 def parse_emojis(filename=EMOJI_PATH):
     return json.load(open(filename, encoding="utf-8"))
@@ -121,20 +115,19 @@
     names = tuple(map(clean_name, args.name))
 
     # Marker for if the given emoji isn't found.
     missing = False
 
     # Search mode.
     if args.search:
-
         # Lookup the search term.
         found = do_find(lookup, names[0])
 
         # print them to the screen.
-        for (name, emoji) in found:
+        for name, emoji in found:
             # Some registered emoji have no value.
             try:
                 # Copy the results (and say so!) to the clipboard.
                 if copier and not no_copy and len(found) == 1:
                     copier.copy(emoji)
                     print(f"Copied! {emoji}  {name}")
                 else:
```

### Comparing `em_keyboard-3.9.0/em/emoji-en-US.json` & `em_keyboard-4.0.0/src/em_keyboard/emoji-en-US.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976065949795896%*

 * *Differences: {"'☎️'": '{delete: [4]}',*

 * * "'♏'": '{delete: [5]}',*

 * * "'🇨🇳'": '{delete: [8]}',*

 * * "'🇪🇸'": '{delete: [6]}',*

 * * "'🇫🇲'": '{delete: [8]}',*

 * * "'🇫🇷'": '{delete: [7]}',*

 * * "'🇮🇷'": '{delete: [8]}',*

 * * "'🇮🇹'": '{delete: [6]}',*

 * * "'🇲🇩'": '{delete: [7]}',*

 * * "'🇹🇷'": '{delete: [6]}',*

 * * "'🇹🇿'": '{delete: [8]}',*

 * * "'🎒'": '{delete: [4]}',*

 * * "'🐼'": '{delete: [3]}',*

 * * "'👄'": '{delete: [0]}',*

 * * "'👹'": "{insert: [(9, 'japanese_ogre')], delete: [10, 9]}",*

 * * "'👺'": "{insert: [(7, 'japanese_goblin')], delete: [8, 7]}",*

 * * "'💥'": '{delete: [4]}',*

 * * "'💻 […]*

```diff
@@ -358,16 +358,15 @@
         "comet",
         "space"
     ],
     "\u260e\ufe0f": [
         "telephone",
         "technology",
         "communication",
-        "dial",
-        "telephone"
+        "dial"
     ],
     "\u2611\ufe0f": [
         "check_box_with_check",
         "ok",
         "agree",
         "confirm",
         "black-square",
@@ -526,16 +525,15 @@
         "astrology"
     ],
     "\u264f": [
         "scorpio",
         "sign",
         "zodiac",
         "purple-square",
-        "astrology",
-        "scorpio"
+        "astrology"
     ],
     "\u2650": [
         "sagittarius",
         "sign",
         "zodiac",
         "purple-square",
         "astrology"
@@ -1746,16 +1744,15 @@
         "flag_china",
         "china",
         "chinese",
         "prc",
         "flag",
         "country",
         "nation",
-        "banner",
-        "china"
+        "banner"
     ],
     "\ud83c\udde8\ud83c\uddf4": [
         "flag_colombia",
         "co",
         "flag",
         "nation",
         "country",
@@ -1940,16 +1937,15 @@
     ],
     "\ud83c\uddea\ud83c\uddf8": [
         "flag_spain",
         "spain",
         "flag",
         "nation",
         "country",
-        "banner",
-        "spain"
+        "banner"
     ],
     "\ud83c\uddea\ud83c\uddf9": [
         "flag_ethiopia",
         "et",
         "flag",
         "nation",
         "country",
@@ -1996,16 +1992,15 @@
         "flag_micronesia",
         "micronesia",
         "federated",
         "states",
         "flag",
         "nation",
         "country",
-        "banner",
-        "micronesia"
+        "banner"
     ],
     "\ud83c\uddeb\ud83c\uddf4": [
         "flag_faroe_islands",
         "faroe",
         "islands",
         "flag",
         "nation",
@@ -2016,16 +2011,15 @@
     "\ud83c\uddeb\ud83c\uddf7": [
         "flag_france",
         "banner",
         "flag",
         "nation",
         "france",
         "french",
-        "country",
-        "france"
+        "country"
     ],
     "\ud83c\uddec\ud83c\udde6": [
         "flag_gabon",
         "ga",
         "flag",
         "nation",
         "country",
@@ -2339,16 +2333,15 @@
         "flag_iran",
         "iran",
         "islamic",
         "republic",
         "flag",
         "nation",
         "country",
-        "banner",
-        "iran"
+        "banner"
     ],
     "\ud83c\uddee\ud83c\uddf8": [
         "flag_iceland",
         "is",
         "flag",
         "nation",
         "country",
@@ -2357,16 +2350,15 @@
     ],
     "\ud83c\uddee\ud83c\uddf9": [
         "flag_italy",
         "italy",
         "flag",
         "nation",
         "country",
-        "banner",
-        "italy"
+        "banner"
     ],
     "\ud83c\uddef\ud83c\uddea": [
         "flag_jersey",
         "je",
         "flag",
         "nation",
         "country",
@@ -2630,16 +2622,15 @@
     "\ud83c\uddf2\ud83c\udde9": [
         "flag_moldova",
         "moldova",
         "republic",
         "flag",
         "nation",
         "country",
-        "banner",
-        "moldova"
+        "banner"
     ],
     "\ud83c\uddf2\ud83c\uddea": [
         "flag_montenegro",
         "me",
         "flag",
         "nation",
         "country",
@@ -3427,16 +3418,15 @@
     ],
     "\ud83c\uddf9\ud83c\uddf7": [
         "flag_turkey",
         "turkey",
         "flag",
         "nation",
         "country",
-        "banner",
-        "turkey"
+        "banner"
     ],
     "\ud83c\uddf9\ud83c\uddf9": [
         "flag_trinidad_tobago",
         "trinidad",
         "tobago",
         "flag",
         "nation",
@@ -3465,16 +3455,15 @@
         "flag_tanzania",
         "tanzania",
         "united",
         "republic",
         "flag",
         "nation",
         "country",
-        "banner",
-        "tanzania"
+        "banner"
     ],
     "\ud83c\uddfa\ud83c\udde6": [
         "flag_ukraine",
         "ua",
         "flag",
         "nation",
         "country",
@@ -4831,16 +4820,15 @@
         "asia",
         "tsukimi"
     ],
     "\ud83c\udf92": [
         "backpack",
         "student",
         "education",
-        "bag",
-        "backpack"
+        "bag"
     ],
     "\ud83c\udf93": [
         "graduation_cap",
         "school",
         "college",
         "degree",
         "university",
@@ -5995,16 +5983,15 @@
         "polar bear",
         "animal",
         "arctic"
     ],
     "\ud83d\udc3c": [
         "panda",
         "animal",
-        "nature",
-        "panda"
+        "nature"
     ],
     "\ud83d\udc3d": [
         "pig_nose",
         "animal",
         "oink"
     ],
     "\ud83d\udc3e": [
@@ -6054,15 +6041,14 @@
     "\ud83d\udc43": [
         "nose",
         "smell",
         "sniff"
     ],
     "\ud83d\udc44": [
         "mouth",
-        "mouth",
         "kiss"
     ],
     "\ud83d\udc45": [
         "tongue",
         "mouth",
         "playful"
     ],
@@ -7110,27 +7096,25 @@
         "red",
         "mask",
         "halloween",
         "scary",
         "creepy",
         "devil",
         "demon",
-        "japanese",
-        "ogre"
+        "japanese_ogre"
     ],
     "\ud83d\udc7a": [
         "goblin",
         "red",
         "evil",
         "mask",
         "monster",
         "scary",
         "creepy",
-        "japanese",
-        "goblin"
+        "japanese_goblin"
     ],
     "\ud83d\udc7b": [
         "ghost",
         "halloween",
         "spooky",
         "scary"
     ],
@@ -7488,15 +7472,14 @@
         "dream"
     ],
     "\ud83d\udca5": [
         "collision",
         "bomb",
         "explode",
         "explosion",
-        "collision",
         "blown"
     ],
     "\ud83d\udca6": [
         "sweat_droplets",
         "water",
         "drip",
         "oops"
@@ -7661,15 +7644,14 @@
         "bus",
         "flight",
         "fly"
     ],
     "\ud83d\udcbb": [
         "laptop",
         "technology",
-        "laptop",
         "screen",
         "display",
         "monitor"
     ],
     "\ud83d\udcbc": [
         "briefcase",
         "business",
@@ -7732,15 +7714,14 @@
         "documents",
         "office",
         "paper",
         "information"
     ],
     "\ud83d\udcc5": [
         "calendar",
-        "calendar",
         "schedule"
     ],
     "\ud83d\udcc6": [
         "tear_off_calendar",
         "schedule",
         "date",
         "planning"
@@ -8089,16 +8070,15 @@
         "record"
     ],
     "\ud83d\udcfa": [
         "television",
         "technology",
         "program",
         "oldschool",
-        "show",
-        "television"
+        "show"
     ],
     "\ud83d\udcfb": [
         "radio",
         "communication",
         "music",
         "podcast",
         "program"
@@ -8397,15 +8377,14 @@
         "kitchen",
         "weapon"
     ],
     "\ud83d\udd2b": [
         "pistol",
         "violence",
         "weapon",
-        "pistol",
         "revolver"
     ],
     "\ud83d\udd2c": [
         "microscope",
         "laboratory",
         "experiment",
         "zoomin",
@@ -8858,16 +8837,15 @@
         "levitate",
         "hover",
         "jump"
     ],
     "\ud83d\udd75\ufe0f": [
         "detective",
         "human",
-        "spy",
-        "detective"
+        "spy"
     ],
     "\ud83d\udd75\ufe0f\u200d\u2640\ufe0f": [
         "woman_detective",
         "human",
         "spy",
         "detective",
         "female",
@@ -9094,16 +9072,15 @@
         "country",
         "japanese",
         "asia"
     ],
     "\ud83d\uddff": [
         "moai",
         "rock",
-        "easter island",
-        "moai"
+        "easter island"
     ],
     "\ud83d\ude00": [
         "grinning_face",
         "face",
         "smile",
         "happy",
         "joy",
@@ -10134,15 +10111,14 @@
         "disallow",
         "circle"
     ],
     "\ud83d\udeac": [
         "cigarette",
         "kills",
         "tobacco",
-        "cigarette",
         "joint",
         "smoke"
     ],
     "\ud83d\udead": [
         "no_smoking",
         "cigarette",
         "blue-square",
@@ -10176,68 +10152,85 @@
         "drink",
         "faucet",
         "tap",
         "circle"
     ],
     "\ud83d\udeb2": [
         "bicycle",
+        "bike",
         "sports",
-        "bicycle",
         "exercise",
         "hipster"
     ],
     "\ud83d\udeb3": [
         "no_bicycles",
+        "no_bikes",
+        "bicycle",
+        "bike",
         "cyclist",
         "prohibited",
         "circle"
     ],
     "\ud83d\udeb4": [
         "person_biking",
+        "bicycle",
+        "bike",
+        "cyclist",
         "sport",
         "move"
     ],
     "\ud83d\udeb4\u200d\u2640\ufe0f": [
         "woman_biking",
-        "sports",
+        "bicycle",
         "bike",
+        "cyclist",
+        "sports",
         "exercise",
         "hipster",
         "woman",
         "female"
     ],
     "\ud83d\udeb4\u200d\u2642\ufe0f": [
         "man_biking",
-        "sports",
+        "bicycle",
         "bike",
+        "cyclist",
+        "sports",
         "exercise",
         "hipster"
     ],
     "\ud83d\udeb5": [
         "person_mountain_biking",
+        "bicycle",
+        "bike",
+        "cyclist",
         "sport",
         "move"
     ],
     "\ud83d\udeb5\u200d\u2640\ufe0f": [
         "woman_mountain_biking",
+        "bicycle",
+        "bike",
+        "cyclist",
         "transportation",
         "sports",
         "human",
         "race",
-        "bike",
         "woman",
         "female"
     ],
     "\ud83d\udeb5\u200d\u2642\ufe0f": [
         "man_mountain_biking",
+        "bicycle",
+        "bike",
+        "cyclist",
         "transportation",
         "sports",
         "human",
-        "race",
-        "bike"
+        "race"
     ],
     "\ud83d\udeb6": [
         "person_walking",
         "move"
     ],
     "\ud83d\udeb6\u200d\u2640\ufe0f": [
         "woman_walking",
@@ -11303,16 +11296,15 @@
     ],
     "\ud83e\udd6f": [
         "bagel",
         "food",
         "bread",
         "bakery",
         "schmear",
-        "jewish",
-        "bakery"
+        "jewish_bakery"
     ],
     "\ud83e\udd70": [
         "smiling_face_with_hearts",
         "face",
         "love",
         "like",
         "affection",
@@ -11575,15 +11567,14 @@
         "dinosaur",
         "tyrannosaurus",
         "extinct"
     ],
     "\ud83e\udd97": [
         "cricket",
         "animal",
-        "cricket",
         "chirp"
     ],
     "\ud83e\udd98": [
         "kangaroo",
         "animal",
         "nature",
         "australia",
@@ -11918,16 +11909,15 @@
         "face_with_monocle",
         "face",
         "stuffy",
         "wealthy"
     ],
     "\ud83e\uddd1": [
         "person",
-        "gender-neutral",
-        "person"
+        "gender-neutral"
     ],
     "\ud83e\uddd1\u200d\u2695\ufe0f": [
         "health_worker",
         "hospital"
     ],
     "\ud83e\uddd1\u200d\u2696\ufe0f": [
         "judge",
```

### Comparing `em_keyboard-3.9.0/scripts/despacify.py` & `em_keyboard-4.0.0/scripts/despacify.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Replace spaces in emoji keywords with underscores
 """
 from __future__ import annotations
 
 import json
 
-from em import parse_emojis
+from em_keyboard import parse_emojis
 
-INPUT_EMOJILIB_PATH = "em/emoji-en-US.json"
-OUTPUT_EMOJI_PATH = "em/emojis.json"
+INPUT_EMOJILIB_PATH = "src/em_keyboard/emoji-en-US.json"
+OUTPUT_EMOJI_PATH = "src/em_keyboard/emojis.json"
 
 
 def save_emojis(data: dict[str, list[str]], filename: str) -> None:
     with open(filename, "w") as outfile:
         json.dump(data, outfile, indent=None, separators=(",", ":"))
+        outfile.write("\n")
 
 
 def main() -> None:
     data = parse_emojis(INPUT_EMOJILIB_PATH)
     for emoji, keywords in data.items():
         keywords = [keyword.replace(" ", "_") for keyword in keywords]
         data[emoji] = keywords
```

### Comparing `em_keyboard-3.9.0/tests/test_em.py` & `em_keyboard-4.0.0/tests/test_em.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import argparse
 import random
 from unittest.mock import call, patch
 
 import pytest
 
-from em import cli, copier
+from em_keyboard import cli, copier
 
 
 @pytest.mark.parametrize(
     "test_name",
     [
         "star",
         ":star:",
         "STAR",
         ":Star:",
     ],
 )
-@patch("em.argparse.ArgumentParser.parse_args")
+@patch("em_keyboard.argparse.ArgumentParser.parse_args")
 @patch("builtins.print")
 def test_star(mock_print, mock_argparse, test_name):
     # Arrange
     mock_argparse.return_value = argparse.Namespace(
         name=[test_name], no_copy=None, search=False, random=False
     )
 
@@ -33,15 +33,15 @@
         mock_print.assert_called_once_with("Copied! ⭐")
     else:
         mock_print.assert_called_once_with("⭐")
     assert e.type == SystemExit
     assert e.value.code == 0
 
 
-@patch("em.argparse.ArgumentParser.parse_args")
+@patch("em_keyboard.argparse.ArgumentParser.parse_args")
 @patch("builtins.print")
 def test_not_found(mock_print, mock_argparse):
     # Arrange
     mock_argparse.return_value = argparse.Namespace(
         name=["xxx"], no_copy=None, search=False, random=False
     )
 
@@ -50,15 +50,15 @@
 
     # Assert
     mock_print.assert_called_once_with("")
     assert e.type == SystemExit
     assert e.value.code == 1
 
 
-@patch("em.argparse.ArgumentParser.parse_args")
+@patch("em_keyboard.argparse.ArgumentParser.parse_args")
 @patch("builtins.print")
 def test_no_copy(mock_print, mock_argparse):
     # Arrange
     mock_argparse.return_value = argparse.Namespace(
         name=["star"], no_copy=True, search=False, random=False
     )
 
@@ -68,15 +68,15 @@
 
     # Assert
     mock_print.assert_called_once_with("⭐")
     assert e.type == SystemExit
     assert e.value.code == 0
 
 
-@patch("em.argparse.ArgumentParser.parse_args")
+@patch("em_keyboard.argparse.ArgumentParser.parse_args")
 @patch("builtins.print")
 def test_search_star(mock_print, mock_argparse):
     # Arrange
     mock_argparse.return_value = argparse.Namespace(
         name=["star"], no_copy=None, search=True, random=False
     )
     expected = (
@@ -92,15 +92,15 @@
     # Assert
     for arg in expected:
         assert call(arg) in mock_print.call_args_list
     assert e.type == SystemExit
     assert e.value.code == 0
 
 
-@patch("em.argparse.ArgumentParser.parse_args")
+@patch("em_keyboard.argparse.ArgumentParser.parse_args")
 @patch("builtins.print")
 def test_search_single_result_is_copied(mock_print, mock_argparse):
     # Arrange
     mock_argparse.return_value = argparse.Namespace(
         name=["ukraine"], no_copy=None, search=True, random=False
     )
 
@@ -113,15 +113,15 @@
         mock_print.assert_called_once_with("Copied! 🇺🇦  flag_ukraine")
     else:
         mock_print.assert_called_once_with("🇺🇦  flag_ukraine")
     assert e.type == SystemExit
     assert e.value.code == 0
 
 
-@patch("em.argparse.ArgumentParser.parse_args")
+@patch("em_keyboard.argparse.ArgumentParser.parse_args")
 @patch("builtins.print")
 def test_search_not_found(mock_print, mock_argparse):
     # Arrange
     mock_argparse.return_value = argparse.Namespace(
         name=["twenty_o_clock"], no_copy=None, search=True, random=False
     )
 
@@ -131,15 +131,15 @@
 
     # Assert
     mock_print.assert_not_called()
     assert e.type == SystemExit
     assert e.value.code == 1
 
 
-@patch("em.argparse.ArgumentParser.parse_args")
+@patch("em_keyboard.argparse.ArgumentParser.parse_args")
 @patch("builtins.print")
 def test_random(mock_print, mock_argparse):
     # Arrange
     mock_argparse.return_value = argparse.Namespace(
         name=None, no_copy=None, search=False, random=True
     )
     random.seed(123)
```

### Comparing `em_keyboard-3.9.0/em/emojis.json` & `em_keyboard-4.0.0/src/em_keyboard/emojis.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976065949795896%*

 * *Differences: {"'☎️'": '{delete: [4]}',*

 * * "'♏'": '{delete: [5]}',*

 * * "'🇨🇳'": '{delete: [8]}',*

 * * "'🇪🇸'": '{delete: [6]}',*

 * * "'🇫🇲'": '{delete: [8]}',*

 * * "'🇫🇷'": '{delete: [7]}',*

 * * "'🇮🇷'": '{delete: [8]}',*

 * * "'🇮🇹'": '{delete: [6]}',*

 * * "'🇲🇩'": '{delete: [7]}',*

 * * "'🇹🇷'": '{delete: [6]}',*

 * * "'🇹🇿'": '{delete: [8]}',*

 * * "'🎒'": '{delete: [4]}',*

 * * "'🐼'": '{delete: [3]}',*

 * * "'👄'": '{delete: [0]}',*

 * * "'👹'": "{insert: [(9, 'japanese_ogre')], delete: [10, 9]}",*

 * * "'👺'": "{insert: [(7, 'japanese_goblin')], delete: [8, 7]}",*

 * * "'💥'": '{delete: [4]}',*

 * * "'💻 […]*

```diff
@@ -358,16 +358,15 @@
         "comet",
         "space"
     ],
     "\u260e\ufe0f": [
         "telephone",
         "technology",
         "communication",
-        "dial",
-        "telephone"
+        "dial"
     ],
     "\u2611\ufe0f": [
         "check_box_with_check",
         "ok",
         "agree",
         "confirm",
         "black-square",
@@ -526,16 +525,15 @@
         "astrology"
     ],
     "\u264f": [
         "scorpio",
         "sign",
         "zodiac",
         "purple-square",
-        "astrology",
-        "scorpio"
+        "astrology"
     ],
     "\u2650": [
         "sagittarius",
         "sign",
         "zodiac",
         "purple-square",
         "astrology"
@@ -1746,16 +1744,15 @@
         "flag_china",
         "china",
         "chinese",
         "prc",
         "flag",
         "country",
         "nation",
-        "banner",
-        "china"
+        "banner"
     ],
     "\ud83c\udde8\ud83c\uddf4": [
         "flag_colombia",
         "co",
         "flag",
         "nation",
         "country",
@@ -1940,16 +1937,15 @@
     ],
     "\ud83c\uddea\ud83c\uddf8": [
         "flag_spain",
         "spain",
         "flag",
         "nation",
         "country",
-        "banner",
-        "spain"
+        "banner"
     ],
     "\ud83c\uddea\ud83c\uddf9": [
         "flag_ethiopia",
         "et",
         "flag",
         "nation",
         "country",
@@ -1996,16 +1992,15 @@
         "flag_micronesia",
         "micronesia",
         "federated",
         "states",
         "flag",
         "nation",
         "country",
-        "banner",
-        "micronesia"
+        "banner"
     ],
     "\ud83c\uddeb\ud83c\uddf4": [
         "flag_faroe_islands",
         "faroe",
         "islands",
         "flag",
         "nation",
@@ -2016,16 +2011,15 @@
     "\ud83c\uddeb\ud83c\uddf7": [
         "flag_france",
         "banner",
         "flag",
         "nation",
         "france",
         "french",
-        "country",
-        "france"
+        "country"
     ],
     "\ud83c\uddec\ud83c\udde6": [
         "flag_gabon",
         "ga",
         "flag",
         "nation",
         "country",
@@ -2339,16 +2333,15 @@
         "flag_iran",
         "iran",
         "islamic",
         "republic",
         "flag",
         "nation",
         "country",
-        "banner",
-        "iran"
+        "banner"
     ],
     "\ud83c\uddee\ud83c\uddf8": [
         "flag_iceland",
         "is",
         "flag",
         "nation",
         "country",
@@ -2357,16 +2350,15 @@
     ],
     "\ud83c\uddee\ud83c\uddf9": [
         "flag_italy",
         "italy",
         "flag",
         "nation",
         "country",
-        "banner",
-        "italy"
+        "banner"
     ],
     "\ud83c\uddef\ud83c\uddea": [
         "flag_jersey",
         "je",
         "flag",
         "nation",
         "country",
@@ -2630,16 +2622,15 @@
     "\ud83c\uddf2\ud83c\udde9": [
         "flag_moldova",
         "moldova",
         "republic",
         "flag",
         "nation",
         "country",
-        "banner",
-        "moldova"
+        "banner"
     ],
     "\ud83c\uddf2\ud83c\uddea": [
         "flag_montenegro",
         "me",
         "flag",
         "nation",
         "country",
@@ -3427,16 +3418,15 @@
     ],
     "\ud83c\uddf9\ud83c\uddf7": [
         "flag_turkey",
         "turkey",
         "flag",
         "nation",
         "country",
-        "banner",
-        "turkey"
+        "banner"
     ],
     "\ud83c\uddf9\ud83c\uddf9": [
         "flag_trinidad_tobago",
         "trinidad",
         "tobago",
         "flag",
         "nation",
@@ -3465,16 +3455,15 @@
         "flag_tanzania",
         "tanzania",
         "united",
         "republic",
         "flag",
         "nation",
         "country",
-        "banner",
-        "tanzania"
+        "banner"
     ],
     "\ud83c\uddfa\ud83c\udde6": [
         "flag_ukraine",
         "ua",
         "flag",
         "nation",
         "country",
@@ -4831,16 +4820,15 @@
         "asia",
         "tsukimi"
     ],
     "\ud83c\udf92": [
         "backpack",
         "student",
         "education",
-        "bag",
-        "backpack"
+        "bag"
     ],
     "\ud83c\udf93": [
         "graduation_cap",
         "school",
         "college",
         "degree",
         "university",
@@ -5995,16 +5983,15 @@
         "polar_bear",
         "animal",
         "arctic"
     ],
     "\ud83d\udc3c": [
         "panda",
         "animal",
-        "nature",
-        "panda"
+        "nature"
     ],
     "\ud83d\udc3d": [
         "pig_nose",
         "animal",
         "oink"
     ],
     "\ud83d\udc3e": [
@@ -6054,15 +6041,14 @@
     "\ud83d\udc43": [
         "nose",
         "smell",
         "sniff"
     ],
     "\ud83d\udc44": [
         "mouth",
-        "mouth",
         "kiss"
     ],
     "\ud83d\udc45": [
         "tongue",
         "mouth",
         "playful"
     ],
@@ -7110,27 +7096,25 @@
         "red",
         "mask",
         "halloween",
         "scary",
         "creepy",
         "devil",
         "demon",
-        "japanese",
-        "ogre"
+        "japanese_ogre"
     ],
     "\ud83d\udc7a": [
         "goblin",
         "red",
         "evil",
         "mask",
         "monster",
         "scary",
         "creepy",
-        "japanese",
-        "goblin"
+        "japanese_goblin"
     ],
     "\ud83d\udc7b": [
         "ghost",
         "halloween",
         "spooky",
         "scary"
     ],
@@ -7488,15 +7472,14 @@
         "dream"
     ],
     "\ud83d\udca5": [
         "collision",
         "bomb",
         "explode",
         "explosion",
-        "collision",
         "blown"
     ],
     "\ud83d\udca6": [
         "sweat_droplets",
         "water",
         "drip",
         "oops"
@@ -7661,15 +7644,14 @@
         "bus",
         "flight",
         "fly"
     ],
     "\ud83d\udcbb": [
         "laptop",
         "technology",
-        "laptop",
         "screen",
         "display",
         "monitor"
     ],
     "\ud83d\udcbc": [
         "briefcase",
         "business",
@@ -7732,15 +7714,14 @@
         "documents",
         "office",
         "paper",
         "information"
     ],
     "\ud83d\udcc5": [
         "calendar",
-        "calendar",
         "schedule"
     ],
     "\ud83d\udcc6": [
         "tear_off_calendar",
         "schedule",
         "date",
         "planning"
@@ -8089,16 +8070,15 @@
         "record"
     ],
     "\ud83d\udcfa": [
         "television",
         "technology",
         "program",
         "oldschool",
-        "show",
-        "television"
+        "show"
     ],
     "\ud83d\udcfb": [
         "radio",
         "communication",
         "music",
         "podcast",
         "program"
@@ -8397,15 +8377,14 @@
         "kitchen",
         "weapon"
     ],
     "\ud83d\udd2b": [
         "pistol",
         "violence",
         "weapon",
-        "pistol",
         "revolver"
     ],
     "\ud83d\udd2c": [
         "microscope",
         "laboratory",
         "experiment",
         "zoomin",
@@ -8858,16 +8837,15 @@
         "levitate",
         "hover",
         "jump"
     ],
     "\ud83d\udd75\ufe0f": [
         "detective",
         "human",
-        "spy",
-        "detective"
+        "spy"
     ],
     "\ud83d\udd75\ufe0f\u200d\u2640\ufe0f": [
         "woman_detective",
         "human",
         "spy",
         "detective",
         "female",
@@ -9094,16 +9072,15 @@
         "country",
         "japanese",
         "asia"
     ],
     "\ud83d\uddff": [
         "moai",
         "rock",
-        "easter_island",
-        "moai"
+        "easter_island"
     ],
     "\ud83d\ude00": [
         "grinning_face",
         "face",
         "smile",
         "happy",
         "joy",
@@ -10134,15 +10111,14 @@
         "disallow",
         "circle"
     ],
     "\ud83d\udeac": [
         "cigarette",
         "kills",
         "tobacco",
-        "cigarette",
         "joint",
         "smoke"
     ],
     "\ud83d\udead": [
         "no_smoking",
         "cigarette",
         "blue-square",
@@ -10176,68 +10152,85 @@
         "drink",
         "faucet",
         "tap",
         "circle"
     ],
     "\ud83d\udeb2": [
         "bicycle",
+        "bike",
         "sports",
-        "bicycle",
         "exercise",
         "hipster"
     ],
     "\ud83d\udeb3": [
         "no_bicycles",
+        "no_bikes",
+        "bicycle",
+        "bike",
         "cyclist",
         "prohibited",
         "circle"
     ],
     "\ud83d\udeb4": [
         "person_biking",
+        "bicycle",
+        "bike",
+        "cyclist",
         "sport",
         "move"
     ],
     "\ud83d\udeb4\u200d\u2640\ufe0f": [
         "woman_biking",
-        "sports",
+        "bicycle",
         "bike",
+        "cyclist",
+        "sports",
         "exercise",
         "hipster",
         "woman",
         "female"
     ],
     "\ud83d\udeb4\u200d\u2642\ufe0f": [
         "man_biking",
-        "sports",
+        "bicycle",
         "bike",
+        "cyclist",
+        "sports",
         "exercise",
         "hipster"
     ],
     "\ud83d\udeb5": [
         "person_mountain_biking",
+        "bicycle",
+        "bike",
+        "cyclist",
         "sport",
         "move"
     ],
     "\ud83d\udeb5\u200d\u2640\ufe0f": [
         "woman_mountain_biking",
+        "bicycle",
+        "bike",
+        "cyclist",
         "transportation",
         "sports",
         "human",
         "race",
-        "bike",
         "woman",
         "female"
     ],
     "\ud83d\udeb5\u200d\u2642\ufe0f": [
         "man_mountain_biking",
+        "bicycle",
+        "bike",
+        "cyclist",
         "transportation",
         "sports",
         "human",
-        "race",
-        "bike"
+        "race"
     ],
     "\ud83d\udeb6": [
         "person_walking",
         "move"
     ],
     "\ud83d\udeb6\u200d\u2640\ufe0f": [
         "woman_walking",
@@ -11303,16 +11296,15 @@
     ],
     "\ud83e\udd6f": [
         "bagel",
         "food",
         "bread",
         "bakery",
         "schmear",
-        "jewish",
-        "bakery"
+        "jewish_bakery"
     ],
     "\ud83e\udd70": [
         "smiling_face_with_hearts",
         "face",
         "love",
         "like",
         "affection",
@@ -11575,15 +11567,14 @@
         "dinosaur",
         "tyrannosaurus",
         "extinct"
     ],
     "\ud83e\udd97": [
         "cricket",
         "animal",
-        "cricket",
         "chirp"
     ],
     "\ud83e\udd98": [
         "kangaroo",
         "animal",
         "nature",
         "australia",
@@ -11918,16 +11909,15 @@
         "face_with_monocle",
         "face",
         "stuffy",
         "wealthy"
     ],
     "\ud83e\uddd1": [
         "person",
-        "gender-neutral",
-        "person"
+        "gender-neutral"
     ],
     "\ud83e\uddd1\u200d\u2695\ufe0f": [
         "health_worker",
         "hospital"
     ],
     "\ud83e\uddd1\u200d\u2696\ufe0f": [
         "judge",
```

### Comparing `em_keyboard-3.9.0/LICENSE` & `em_keyboard-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `em_keyboard-3.9.0/NOTICE` & `em_keyboard-4.0.0/NOTICE`

 * *Files identical despite different names*

### Comparing `em_keyboard-3.9.0/README.md` & `em_keyboard-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `em_keyboard-3.9.0/pyproject.toml` & `em_keyboard-4.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,76 +2,65 @@
 build-backend = "hatchling.build"
 requires = [
   "hatch-vcs",
   "hatchling",
 ]
 
 [project]
-name = "em_keyboard"
+name = "em-keyboard"
 description = "The CLI Emoji Keyboard"
 readme = "README.md"
 keywords = [
   "CLI",
   "emoji",
   "keyboard",
   "search",
 ]
 license = {text = "ISC"}
 maintainers = [{name = "Hugo van Kemenade"}]
 authors = [{name = "Kenneth Reitz", email = "me@kennethreitz.org"}]
-requires-python = ">=3.7"
-dependencies = [
-  'importlib-metadata; python_version < "3.8"',
-  'pyperclip; platform_system == "Darwin"',
-  'pyperclip; platform_system == "Windows"',
+requires-python = ">=3.8"
+classifiers = [
+  "Development Status :: 5 - Production/Stable",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: ISC License (ISCL)",
+  "Natural Language :: English",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dynamic = [
   "version",
 ]
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: ISC License (ISCL)",
-    "Natural Language :: English",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
+dependencies = [
+  'pyperclip; platform_system == "Darwin"',
+  'pyperclip; platform_system == "Windows"',
 ]
 [project.optional-dependencies]
 tests = [
   "pytest",
   "pytest-cov",
 ]
-
 [project.urls]
 Changelog = "https://github.com/hugovk/em-keyboard/releases"
 Homepage = "https://github.com/hugovk/em-keyboard"
 Source = "https://github.com/hugovk/em-keyboard"
-
 [project.scripts]
-em = "em:cli"
-
-
-[tool.black]
-target_version = ["py37"]
+em = "em_keyboard:cli"
 
 [tool.hatch]
 version.source = "vcs"
 
-[tool.hatch.build.force-include]
-"em/emojis.json" = "em/emojis.json"
-
 [tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
 
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
```

### Comparing `em_keyboard-3.9.0/PKG-INFO` & `em_keyboard-4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: em_keyboard
-Version: 3.9.0
+Name: em-keyboard
+Version: 4.0.0
 Summary: The CLI Emoji Keyboard
 Project-URL: Changelog, https://github.com/hugovk/em-keyboard/releases
 Project-URL: Homepage, https://github.com/hugovk/em-keyboard
 Project-URL: Source, https://github.com/hugovk/em-keyboard
 Author-email: Kenneth Reitz <me@kennethreitz.org>
 Maintainer: Hugo van Kemenade
 License: ISC
@@ -14,24 +14,22 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Requires-Dist: importlib-metadata; python_version < '3.8'
+Requires-Python: >=3.8
 Requires-Dist: pyperclip; platform_system == 'Darwin'
 Requires-Dist: pyperclip; platform_system == 'Windows'
 Provides-Extra: tests
 Requires-Dist: pytest; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
 Description-Content-Type: text/markdown
```

