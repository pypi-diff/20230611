# Comparing `tmp/vader_umpt-0.1.0.tar.gz` & `tmp/vader_umpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vader_umpt-0.1.0.tar", max compression
+gzip compressed data, was "vader_umpt-0.1.1.tar", max compression
```

## Comparing `vader_umpt-0.1.0.tar` & `vader_umpt-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4115 2023-06-11 16:41:24.740181 vader_umpt-0.1.0/README.md
--rw-r--r--   0        0        0      489 2023-06-11 16:41:39.778480 vader_umpt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    20103 2023-06-11 13:47:59.932978 vader_umpt-0.1.0/vader_umpt/vader/__init__.py
--rw-r--r--   0        0        0      991 2023-06-07 19:48:20.087918 vader_umpt-0.1.0/vader_umpt/vader/lexicons/booster.txt
--rw-r--r--   0        0        0   132797 2023-06-07 19:48:20.088918 vader_umpt-0.1.0/vader_umpt/vader/lexicons/emoji_utf8_lexicon_ptbr.txt
--rw-r--r--   0        0        0      493 2023-06-07 19:48:20.088918 vader_umpt-0.1.0/vader_umpt/vader/lexicons/negate.txt
--rw-r--r--   0        0        0   427190 2023-06-07 19:48:20.090918 vader_umpt-0.1.0/vader_umpt/vader/lexicons/vader_lexicon_ptbr.txt
--rwxr-xr-x   0        0        0     2220 2023-06-11 11:54:26.050583 vader_umpt-0.1.0/vader_umpt/vader-umpt
--rw-r--r--   0        0        0      681 2023-06-07 20:22:40.921711 vader_umpt-0.1.0/vader_umpt/web.py
--rw-r--r--   0        0        0     4634 1970-01-01 00:00:00.000000 vader_umpt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7661 2023-06-11 17:13:00.398860 vader_umpt-0.1.1/README.md
+-rw-r--r--   0        0        0      541 2023-06-11 16:52:56.516928 vader_umpt-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0     2531 2023-06-11 16:53:30.850327 vader_umpt-0.1.1/vader_umpt/__init__.py
+-rw-r--r--   0        0        0    20103 2023-06-11 13:47:59.932978 vader_umpt-0.1.1/vader_umpt/vader/__init__.py
+-rw-r--r--   0        0        0      991 2023-06-07 19:48:20.087918 vader_umpt-0.1.1/vader_umpt/vader/lexicons/booster.txt
+-rw-r--r--   0        0        0   132797 2023-06-07 19:48:20.088918 vader_umpt-0.1.1/vader_umpt/vader/lexicons/emoji_utf8_lexicon_ptbr.txt
+-rw-r--r--   0        0        0      493 2023-06-07 19:48:20.088918 vader_umpt-0.1.1/vader_umpt/vader/lexicons/negate.txt
+-rw-r--r--   0        0        0   427190 2023-06-07 19:48:20.090918 vader_umpt-0.1.1/vader_umpt/vader/lexicons/vader_lexicon_ptbr.txt
+-rw-r--r--   0        0        0      681 2023-06-07 20:22:40.921711 vader_umpt-0.1.1/vader_umpt/web.py
+-rw-r--r--   0        0        0     8180 1970-01-01 00:00:00.000000 vader_umpt-0.1.1/PKG-INFO
```

### Comparing `vader_umpt-0.1.0/vader_umpt/vader/__init__.py` & `vader_umpt-0.1.1/vader_umpt/vader/__init__.py`

 * *Files identical despite different names*

### Comparing `vader_umpt-0.1.0/vader_umpt/vader/lexicons/booster.txt` & `vader_umpt-0.1.1/vader_umpt/vader/lexicons/booster.txt`

 * *Files identical despite different names*

### Comparing `vader_umpt-0.1.0/vader_umpt/vader/lexicons/emoji_utf8_lexicon_ptbr.txt` & `vader_umpt-0.1.1/vader_umpt/vader/lexicons/emoji_utf8_lexicon_ptbr.txt`

 * *Files identical despite different names*

### Comparing `vader_umpt-0.1.0/vader_umpt/vader/lexicons/vader_lexicon_ptbr.txt` & `vader_umpt-0.1.1/vader_umpt/vader/lexicons/vader_lexicon_ptbr.txt`

 * *Files identical despite different names*

### Comparing `vader_umpt-0.1.0/vader_umpt/vader-umpt` & `vader_umpt-0.1.1/vader_umpt/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,79 +3,83 @@
 from argparse import ArgumentParser
 import vader
 import os
 import json
 import sys
 from typing import cast, Dict, Any
 
-parser = ArgumentParser(
-    prog="VADER-UMPT",
-    description="Ferramenta para análise de sentimento em português",
-)
-
-parser.add_argument(
-    "--export-dicts", help="Exporta os dicionários", action="store_true"
-)
-
-parser.add_argument(
-    "-l",
-    "--lexicon",
-    help="Ficheiro com o dicionário a ser utilizado",
-    type=str,
-    default=os.path.join(vader.PACKAGE_DIRECTORY, "lexicons", "vader_lexicon_ptbr.txt"),
-)
-parser.add_argument(
-    "--emoji-lexicon",
-    help="Ficheiro com o dicionário de emojis a ser utilizado",
-    type=str,
-    default=os.path.join(
-        vader.PACKAGE_DIRECTORY, "lexicons", "emoji_utf8_lexicon_ptbr.txt"
-    ),
-)
-parser.add_argument(
-    "-e",
-    "--explain",
-    help="Imprimir explicação detalhada sobre como a pontuação foi calculada",
-    action="store_true",
-)
-parser.add_argument(
-    "-w",
-    "--web",
-    help="Executar um playground web para testar o analisador",
-    action="store_true",
-)
-
-args = parser.parse_args()
-
-analyser = vader.SentimentIntensityAnalyzer(
-    lexicon_file=args.lexicon, emoji_lexicon=args.emoji_lexicon
-)
-
-if args.web:
-    import streamlit.web.bootstrap
-    from streamlit import config as _config
-
-    _config.set_option("server.headless", True)
-    args = []
-    streamlit.web.bootstrap.run(
-        os.path.join((os.path.dirname(__file__)), "web.py"), "", args, flag_options={}
-    )
-else:
-    if args.export_dicts:
-        e = {
-            "lexicon": analyser.lexicon,
-            "emojis": analyser.emojis,
-            "punctuation": vader.PUNC_LIST,
-            "negation": vader.NEGATE,
-            "booster": vader.BOOSTER_DICT,
-        }
+def main():
+    parser = ArgumentParser(
+        prog="VADER-UMPT",
+        description="Ferramenta para análise de sentimento em português",
+    )
+
+    parser.add_argument(
+        "--export-dicts", help="Exporta os dicionários", action="store_true"
+    )
+
+    parser.add_argument(
+        "-l",
+        "--lexicon",
+        help="Ficheiro com o dicionário a ser utilizado",
+        type=str,
+        default=os.path.join(vader.PACKAGE_DIRECTORY, "lexicons", "vader_lexicon_ptbr.txt"),
+    )
+    parser.add_argument(
+        "--emoji-lexicon",
+        help="Ficheiro com o dicionário de emojis a ser utilizado",
+        type=str,
+        default=os.path.join(
+            vader.PACKAGE_DIRECTORY, "lexicons", "emoji_utf8_lexicon_ptbr.txt"
+        ),
+    )
+    parser.add_argument(
+        "-e",
+        "--explain",
+        help="Imprimir explicação detalhada sobre como a pontuação foi calculada",
+        action="store_true",
+    )
+    parser.add_argument(
+        "-w",
+        "--web",
+        help="Executar um playground web para testar o analisador",
+        action="store_true",
+    )
+
+    args = parser.parse_args()
 
-        print(json.dumps(e, ensure_ascii=False))
+    analyser = vader.SentimentIntensityAnalyzer(
+        lexicon_file=args.lexicon, emoji_lexicon=args.emoji_lexicon
+    )
+
+    if args.web:
+        import streamlit.web.bootstrap
+        from streamlit import config as _config
+
+        _config.set_option("server.headless", True)
+        args = []
+        streamlit.web.bootstrap.run(
+            os.path.join((os.path.dirname(__file__)), "web.py"), "", args, flag_options={}
+        )
     else:
-        for line in sys.stdin:
-            scores = analyser.polarity_scores(line)
-            if not args.explain:
-                print(json.dumps(scores[0], ensure_ascii=False))
-            else:
-                new_scores = cast(Dict[str, Any], scores[0])
-                new_scores["explanation"] = scores[1]
-                print(json.dumps(new_scores, ensure_ascii=False))
+        if args.export_dicts:
+            e = {
+                "lexicon": analyser.lexicon,
+                "emojis": analyser.emojis,
+                "punctuation": vader.PUNC_LIST,
+                "negation": vader.NEGATE,
+                "booster": vader.BOOSTER_DICT,
+            }
+
+            print(json.dumps(e, ensure_ascii=False))
+        else:
+            for line in sys.stdin:
+                scores = analyser.polarity_scores(line)
+                if not args.explain:
+                    print(json.dumps(scores[0], ensure_ascii=False))
+                else:
+                    new_scores = cast(Dict[str, Any], scores[0])
+                    new_scores["explanation"] = scores[1]
+                    print(json.dumps(new_scores, ensure_ascii=False))
+
+if __name__ == '__main__':
+    main()
```

### Comparing `vader_umpt-0.1.0/vader_umpt/web.py` & `vader_umpt-0.1.1/vader_umpt/web.py`

 * *Files identical despite different names*

