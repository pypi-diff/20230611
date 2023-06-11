# Comparing `tmp/cheerup-0.1.1.tar.gz` & `tmp/cheerup-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheerup-0.1.1.tar", last modified: Sun Jun 11 07:24:37 2023, max compression
+gzip compressed data, was "cheerup-0.1.2.tar", last modified: Sun Jun 11 12:15:11 2023, max compression
```

## Comparing `cheerup-0.1.1.tar` & `cheerup-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tyamamiya   (501) staff       (20)        0 2023-06-11 07:24:37.455913 cheerup-0.1.1/
--rw-r--r--   0 tyamamiya   (501) staff       (20)     1072 2023-06-11 06:23:09.000000 cheerup-0.1.1/LICENSE
--rw-r--r--   0 tyamamiya   (501) staff       (20)     2351 2023-06-11 07:24:37.455775 cheerup-0.1.1/PKG-INFO
--rw-r--r--   0 tyamamiya   (501) staff       (20)     1951 2023-06-11 07:19:24.000000 cheerup-0.1.1/README.md
--rw-r--r--   0 tyamamiya   (501) staff       (20)      552 2023-06-11 07:23:17.000000 cheerup-0.1.1/pyproject.toml
--rw-r--r--   0 tyamamiya   (501) staff       (20)       38 2023-06-11 07:24:37.455955 cheerup-0.1.1/setup.cfg
-drwxr-xr-x   0 tyamamiya   (501) staff       (20)        0 2023-06-11 07:24:37.454077 cheerup-0.1.1/src/
-drwxr-xr-x   0 tyamamiya   (501) staff       (20)        0 2023-06-11 07:24:37.454711 cheerup-0.1.1/src/cheerup/
--rw-r--r--   0 tyamamiya   (501) staff       (20)     3997 2023-06-11 07:18:58.000000 cheerup-0.1.1/src/cheerup/__init__.py
-drwxr-xr-x   0 tyamamiya   (501) staff       (20)        0 2023-06-11 07:24:37.455531 cheerup-0.1.1/src/cheerup.egg-info/
--rw-r--r--   0 tyamamiya   (501) staff       (20)     2351 2023-06-11 07:24:37.000000 cheerup-0.1.1/src/cheerup.egg-info/PKG-INFO
--rw-r--r--   0 tyamamiya   (501) staff       (20)      268 2023-06-11 07:24:37.000000 cheerup-0.1.1/src/cheerup.egg-info/SOURCES.txt
--rw-r--r--   0 tyamamiya   (501) staff       (20)        1 2023-06-11 07:24:37.000000 cheerup-0.1.1/src/cheerup.egg-info/dependency_links.txt
--rw-r--r--   0 tyamamiya   (501) staff       (20)       41 2023-06-11 07:24:37.000000 cheerup-0.1.1/src/cheerup.egg-info/entry_points.txt
--rw-r--r--   0 tyamamiya   (501) staff       (20)       44 2023-06-11 07:24:37.000000 cheerup-0.1.1/src/cheerup.egg-info/requires.txt
--rw-r--r--   0 tyamamiya   (501) staff       (20)        8 2023-06-11 07:24:37.000000 cheerup-0.1.1/src/cheerup.egg-info/top_level.txt
+drwxr-xr-x   0 tyamamiya   (501) staff       (20)        0 2023-06-11 12:15:11.887266 cheerup-0.1.2/
+-rw-r--r--   0 tyamamiya   (501) staff       (20)     1072 2023-06-11 06:23:09.000000 cheerup-0.1.2/LICENSE
+-rw-r--r--   0 tyamamiya   (501) staff       (20)     2700 2023-06-11 12:15:11.887049 cheerup-0.1.2/PKG-INFO
+-rw-r--r--   0 tyamamiya   (501) staff       (20)     2172 2023-06-11 09:51:06.000000 cheerup-0.1.2/README.md
+-rw-r--r--   0 tyamamiya   (501) staff       (20)      680 2023-06-11 12:09:45.000000 cheerup-0.1.2/pyproject.toml
+-rw-r--r--   0 tyamamiya   (501) staff       (20)       38 2023-06-11 12:15:11.887332 cheerup-0.1.2/setup.cfg
+drwxr-xr-x   0 tyamamiya   (501) staff       (20)        0 2023-06-11 12:15:11.884411 cheerup-0.1.2/src/
+drwxr-xr-x   0 tyamamiya   (501) staff       (20)        0 2023-06-11 12:15:11.885757 cheerup-0.1.2/src/cheerup/
+-rw-r--r--   0 tyamamiya   (501) staff       (20)     4021 2023-06-11 10:01:39.000000 cheerup-0.1.2/src/cheerup/__init__.py
+drwxr-xr-x   0 tyamamiya   (501) staff       (20)        0 2023-06-11 12:15:11.886747 cheerup-0.1.2/src/cheerup.egg-info/
+-rw-r--r--   0 tyamamiya   (501) staff       (20)     2700 2023-06-11 12:15:11.000000 cheerup-0.1.2/src/cheerup.egg-info/PKG-INFO
+-rw-r--r--   0 tyamamiya   (501) staff       (20)      268 2023-06-11 12:15:11.000000 cheerup-0.1.2/src/cheerup.egg-info/SOURCES.txt
+-rw-r--r--   0 tyamamiya   (501) staff       (20)        1 2023-06-11 12:15:11.000000 cheerup-0.1.2/src/cheerup.egg-info/dependency_links.txt
+-rw-r--r--   0 tyamamiya   (501) staff       (20)       41 2023-06-11 12:15:11.000000 cheerup-0.1.2/src/cheerup.egg-info/entry_points.txt
+-rw-r--r--   0 tyamamiya   (501) staff       (20)       44 2023-06-11 12:15:11.000000 cheerup-0.1.2/src/cheerup.egg-info/requires.txt
+-rw-r--r--   0 tyamamiya   (501) staff       (20)        8 2023-06-11 12:15:11.000000 cheerup-0.1.2/src/cheerup.egg-info/top_level.txt
```

### Comparing `cheerup-0.1.1/LICENSE` & `cheerup-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cheerup-0.1.1/PKG-INFO` & `cheerup-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: cheerup
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cheer on your command-line expertise!
 Author-email: Takashi Yamamiya <tak@metatoys.org>
+Project-URL: Homepage, https://github.com/propella/cheerup
+Project-URL: Bug Tracker, https://github.com/propella/cheerup/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # cheerup - Cheer on your command-line expertise!
 
-`cheerup` is a tool designed to elevate your programming experience by complimenting your Unix command-line inputs. Created with the goal to foster learning, motivation, and a sense of achievement among programmers, it's like your own personal assistant that helps you see the magic in every command you run.
+`cheerup` is a tool powered by GPT-3 designed to elevate your programming experience by complimenting your Unix command-line inputs. Created with the goal to foster learning, motivation, and a sense of achievement among programmers, it's like your own personal assistant that helps you see the magic in every command you run.
 
 Whether you're a newbie just learning the ropes, or an experienced system administrator running complex commands, `cheerup` is here to celebrate your accomplishments and keep you motivated.
 
 https://github.com/propella/cheerup/assets/79028/bfb30b42-2eaa-46e0-aa91-bbf4dcad24ee
 
 ## Instructions for ZSH
 
+This tool requires your OpenAI API key. You can generate one at https://platform.openai.com/account/api-keys. Once you have obtained an API key, please set it as the OPENAI_API_KEY environment variable.
+
 ```shell
 $ export OPENAI_API_KEY=<Your OpenAI API key>
 $ pip3 install cheerup
 $ source <(cheerup --zsh)
 
 $ ls
 Makefile	README.md	cheerup.zsh	pyproject.toml	random.md	src
```

### Comparing `cheerup-0.1.1/README.md` & `cheerup-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # cheerup - Cheer on your command-line expertise!
 
-`cheerup` is a tool designed to elevate your programming experience by complimenting your Unix command-line inputs. Created with the goal to foster learning, motivation, and a sense of achievement among programmers, it's like your own personal assistant that helps you see the magic in every command you run.
+`cheerup` is a tool powered by GPT-3 designed to elevate your programming experience by complimenting your Unix command-line inputs. Created with the goal to foster learning, motivation, and a sense of achievement among programmers, it's like your own personal assistant that helps you see the magic in every command you run.
 
 Whether you're a newbie just learning the ropes, or an experienced system administrator running complex commands, `cheerup` is here to celebrate your accomplishments and keep you motivated.
 
 https://github.com/propella/cheerup/assets/79028/bfb30b42-2eaa-46e0-aa91-bbf4dcad24ee
 
 ## Instructions for ZSH
 
+This tool requires your OpenAI API key. You can generate one at https://platform.openai.com/account/api-keys. Once you have obtained an API key, please set it as the OPENAI_API_KEY environment variable.
+
 ```shell
 $ export OPENAI_API_KEY=<Your OpenAI API key>
 $ pip3 install cheerup
 $ source <(cheerup --zsh)
 
 $ ls
 Makefile	README.md	cheerup.zsh	pyproject.toml	random.md	src
```

### Comparing `cheerup-0.1.1/src/cheerup/__init__.py` & `cheerup-0.1.2/src/cheerup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,34 +84,39 @@
     while True:
         try:
             cmd = input("$ ")
             chat(cmd, lang)
         except (KeyboardInterrupt, EOFError):
             return
 
+
 # pylint: disable=consider-using-f-string)
 def show_zsh_script() -> None:
     """Show inititialize script for zsh."""
     command = sys.argv[0]
-    print("""
+    print(
+        """
 # Save the last command.
 CHEERUP_LAST_COMMAND=""
 CHEEUP_EXE="%s"
 
 preexec() {
     CHEERUP_LAST_COMMAND=$1
 }
 
 precmd() {
     # Prevent cheerup command from running on itself.
     if [[ "$CHEERUP_LAST_COMMAND" != "$CHEEUP_EXE -c"* ]]; then
         $CHEEUP_EXE -c "$CHEERUP_LAST_COMMAND"
     fi
 }
-""" % (command))
+"""
+        % (command)
+    )
+
 
 def show_history() -> None:
     """Show history."""
     print(f"History file: {historyfile}")
     pprint(get_history())
```

### Comparing `cheerup-0.1.1/src/cheerup.egg-info/PKG-INFO` & `cheerup-0.1.2/src/cheerup.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: cheerup
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cheer on your command-line expertise!
 Author-email: Takashi Yamamiya <tak@metatoys.org>
+Project-URL: Homepage, https://github.com/propella/cheerup
+Project-URL: Bug Tracker, https://github.com/propella/cheerup/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # cheerup - Cheer on your command-line expertise!
 
-`cheerup` is a tool designed to elevate your programming experience by complimenting your Unix command-line inputs. Created with the goal to foster learning, motivation, and a sense of achievement among programmers, it's like your own personal assistant that helps you see the magic in every command you run.
+`cheerup` is a tool powered by GPT-3 designed to elevate your programming experience by complimenting your Unix command-line inputs. Created with the goal to foster learning, motivation, and a sense of achievement among programmers, it's like your own personal assistant that helps you see the magic in every command you run.
 
 Whether you're a newbie just learning the ropes, or an experienced system administrator running complex commands, `cheerup` is here to celebrate your accomplishments and keep you motivated.
 
 https://github.com/propella/cheerup/assets/79028/bfb30b42-2eaa-46e0-aa91-bbf4dcad24ee
 
 ## Instructions for ZSH
 
+This tool requires your OpenAI API key. You can generate one at https://platform.openai.com/account/api-keys. Once you have obtained an API key, please set it as the OPENAI_API_KEY environment variable.
+
 ```shell
 $ export OPENAI_API_KEY=<Your OpenAI API key>
 $ pip3 install cheerup
 $ source <(cheerup --zsh)
 
 $ ls
 Makefile	README.md	cheerup.zsh	pyproject.toml	random.md	src
```

