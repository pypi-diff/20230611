# Comparing `tmp/term-chatgpt-1.1.5.tar.gz` & `tmp/term-chatgpt-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "term-chatgpt-1.1.5.tar", last modified: Sun Jun 11 04:08:25 2023, max compression
+gzip compressed data, was "term-chatgpt-1.1.6.tar", last modified: Sun Jun 11 04:23:20 2023, max compression
```

## Comparing `term-chatgpt-1.1.5.tar` & `term-chatgpt-1.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 04:08:25.030387 term-chatgpt-1.1.5/
--rw-r--r--   0 runner    (1000) runner    (1000)     1070 2023-06-10 13:57:41.000000 term-chatgpt-1.1.5/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     2105 2023-06-11 04:08:25.026387 term-chatgpt-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1601 2023-06-10 14:28:51.000000 term-chatgpt-1.1.5/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-11 04:08:25.030387 term-chatgpt-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      802 2023-06-11 00:58:28.000000 term-chatgpt-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 04:08:25.026387 term-chatgpt-1.1.5/term_chatgpt.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2105 2023-06-11 04:08:24.000000 term-chatgpt-1.1.5/term_chatgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      330 2023-06-11 04:08:24.000000 term-chatgpt-1.1.5/term_chatgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-11 04:08:24.000000 term-chatgpt-1.1.5/term_chatgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       54 2023-06-11 04:08:24.000000 term-chatgpt-1.1.5/term_chatgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       22 2023-06-11 04:08:24.000000 term-chatgpt-1.1.5/term_chatgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-06-11 04:08:24.000000 term-chatgpt-1.1.5/term_chatgpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 04:08:25.026387 term-chatgpt-1.1.5/termgpt/
--rw-r--r--   0 runner    (1000) runner    (1000)      310 2023-06-10 14:02:02.000000 term-chatgpt-1.1.5/termgpt/__main__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2631 2023-06-10 13:40:59.000000 term-chatgpt-1.1.5/termgpt/cmd.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6093 2023-06-10 14:21:05.000000 term-chatgpt-1.1.5/termgpt/copilot.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2150 2023-06-11 00:57:49.000000 term-chatgpt-1.1.5/termgpt/main.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1246 2023-06-10 13:41:18.000000 term-chatgpt-1.1.5/termgpt/term.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 04:23:20.255318 term-chatgpt-1.1.6/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1070 2023-06-10 13:57:41.000000 term-chatgpt-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     2105 2023-06-11 04:23:20.255318 term-chatgpt-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1601 2023-06-10 14:28:51.000000 term-chatgpt-1.1.6/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-11 04:23:20.255318 term-chatgpt-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      793 2023-06-11 04:22:55.000000 term-chatgpt-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 04:23:20.251318 term-chatgpt-1.1.6/term_chatgpt.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2105 2023-06-11 04:23:19.000000 term-chatgpt-1.1.6/term_chatgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      330 2023-06-11 04:23:19.000000 term-chatgpt-1.1.6/term_chatgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-11 04:23:19.000000 term-chatgpt-1.1.6/term_chatgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       47 2023-06-11 04:23:19.000000 term-chatgpt-1.1.6/term_chatgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       22 2023-06-11 04:23:19.000000 term-chatgpt-1.1.6/term_chatgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-06-11 04:23:19.000000 term-chatgpt-1.1.6/term_chatgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-11 04:23:20.255318 term-chatgpt-1.1.6/termgpt/
+-rw-r--r--   0 runner    (1000) runner    (1000)      326 2023-06-11 04:22:05.000000 term-chatgpt-1.1.6/termgpt/__main__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2631 2023-06-10 13:40:59.000000 term-chatgpt-1.1.6/termgpt/cmd.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6093 2023-06-10 14:21:05.000000 term-chatgpt-1.1.6/termgpt/copilot.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2249 2023-06-11 04:21:34.000000 term-chatgpt-1.1.6/termgpt/main.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1246 2023-06-10 13:41:18.000000 term-chatgpt-1.1.6/termgpt/term.py
```

### Comparing `term-chatgpt-1.1.5/LICENSE` & `term-chatgpt-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1.5/PKG-INFO` & `term-chatgpt-1.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: term-chatgpt
-Version: 1.1.5
+Version: 1.1.6
 Summary: Ask ChatGPT directly on your terminal! Fast & Free.
 Author: AWeirdDev
 Author-email: aweirdscratcher@gmail.com
 License: MIT License
 Keywords: chatgpt,gpt,free,terminal,textual,rich,chat-gpt,ai
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `term-chatgpt-1.1.5/README.md` & `term-chatgpt-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1.5/setup.py` & `term-chatgpt-1.1.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
   name="term-chatgpt",
   author="AWeirdDev",
-  version="1.1.5",
+  version="1.1.6",
   license="MIT License",
   description="Ask ChatGPT directly on your terminal! Fast & Free.",
   long_description=open("README.md", "r", encoding="utf-8").read(),
   long_description_content_type="text/markdown",
   author_email="aweirdscratcher@gmail.com",
   packages=['termgpt'],
   classifiers=[
@@ -15,12 +15,12 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Environment :: Console",
   ],
   keywords=["chatgpt", "gpt", "free", "terminal", "textual", "rich", "chat-gpt", "ai"],
   entry_points={
     "console_scripts": [
-      "term-gpt = termgpt.main:placeholder"
+      "term-gpt=termgpt.main:main"
     ]
   },
   install_requires=["rich", "textual", "requests"]
 )
```

### Comparing `term-chatgpt-1.1.5/term_chatgpt.egg-info/PKG-INFO` & `term-chatgpt-1.1.6/term_chatgpt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: term-chatgpt
-Version: 1.1.5
+Version: 1.1.6
 Summary: Ask ChatGPT directly on your terminal! Fast & Free.
 Author: AWeirdDev
 Author-email: aweirdscratcher@gmail.com
 License: MIT License
 Keywords: chatgpt,gpt,free,terminal,textual,rich,chat-gpt,ai
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `term-chatgpt-1.1.5/termgpt/cmd.py` & `term-chatgpt-1.1.6/termgpt/cmd.py`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1.5/termgpt/copilot.py` & `term-chatgpt-1.1.6/termgpt/copilot.py`

 * *Files identical despite different names*

### Comparing `term-chatgpt-1.1.5/termgpt/main.py` & `term-chatgpt-1.1.6/termgpt/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,77 +4,76 @@
 from rich.markdown import Markdown
 from argparse import ArgumentParser
 
 from .copilot import Copilot
 from .cmd import run_commands
 from .term import terminal_chat
 
-parser = ArgumentParser()
-parser.add_argument("-m", "--mode", help="Set the mode. (terminal / full / quick / run)", dest="mode", default=None)
-parser.add_argument("-a", "--ask", help="Quickly ask Copilot.", dest="content", default=None)
-args = parser.parse_args()
-
-if not args.mode:
-  ans = questionary.select(
-    "Select mode",
-    choices=[
-      "terminal chat",
-      "full screen",
-      "quick ask",
-      "run commands"
-    ],
-    instruction="(Use arrow keys or k-up and j-down keys.)"
-  ).ask()
-else:
-  table = {
-    "terminal": "terminal chat",
-    "full": "full screen",
-    "quick": "quick ask",
-    "run": "run commands"
-  }
-  try:
-    ans = table[args.mode]
-  except KeyError:
-    available = "\n".join([
-      f"- {k}: {v}" for k, v in table.items()
-    ])
-    print(f"Invalid mode.\n\nAvailable ones:\n{available}")
-    exit(2)
-
-
-# match syntax (python 3.10+)
-match ans:
-  case 'full screen':
-    Copilot().run()
-
-  case 'terminal chat':
-    terminal_chat(args.content)
-
-  case "quick ask":
-    if args.content:
-      print("Ask: " + args.content)
-      prompt = args.content
-    else:
-      prompt = input("Ask: ")
-    print("✨ Response:")
-    res = requests.post("https://chatgpt.awdev.repl.co/copilot", json={
-      "prompt": "You will now act like Copilot, a large language model trained by OpenAI.\nI will ask you some questions, and you'll answer as concisely as possible.\nMy first request is: " + prompt
-    }, stream=True)
-
-    fetched = ""
-    def generate(cursor: bool = True):
-      return Markdown(fetched + ("█" if cursor else ""), code_theme="one-dark")
-
-    with Live(generate(), refresh_per_second=4) as live:
-      for chunk in res.iter_content():
-        fetched += chunk.decode('utf-8')
-        live.update(generate())
+def main():
+  parser = ArgumentParser()
+  parser.add_argument("-m", "--mode", help="Set the mode. (terminal / full / quick / run)", dest="mode", default=None)
+  parser.add_argument("-a", "--ask", help="Quickly ask Copilot.", dest="content", default=None)
+  args = parser.parse_args()
+
+  if not args.mode:
+    ans = questionary.select(
+      "Select mode",
+      choices=[
+        "terminal chat",
+        "full screen",
+        "quick ask",
+        "run commands"
+      ],
+      instruction="(Use arrow keys or k-up and j-down keys.)"
+    ).ask()
+  else:
+    table = {
+      "terminal": "terminal chat",
+      "full": "full screen",
+      "quick": "quick ask",
+      "run": "run commands"
+    }
+    try:
+      ans = table[args.mode]
+    except KeyError:
+      available = "\n".join([
+        f"- {k}: {v}" for k, v in table.items()
+      ])
+      print(f"Invalid mode.\n\nAvailable ones:\n{available}")
+      exit(2)
+
+
+  # match syntax (python 3.10+)
+  match ans:
+    case 'full screen':
+      Copilot().run()
+
+    case 'terminal chat':
+      terminal_chat(args.content)
+
+    case "quick ask":
+      if args.content:
+        print("Ask: " + args.content)
+        prompt = args.content
+      else:
+        prompt = input("Ask: ")
+      print("✨ Response:")
+      res = requests.post("https://chatgpt.awdev.repl.co/copilot", json={
+        "prompt": "You will now act like Copilot, a large language model trained by OpenAI.\nI will ask you some questions, and you'll answer as concisely as possible.\nMy first request is: " + prompt
+      }, stream=True)
+
+      fetched = ""
+      def generate(cursor: bool = True):
+        return Markdown(fetched + ("█" if cursor else ""), code_theme="one-dark")
+
+      with Live(generate(), refresh_per_second=4) as live:
+        for chunk in res.iter_content():
+          fetched += chunk.decode('utf-8')
+          live.update(generate())
 
-      live.update(generate(False))
+        live.update(generate(False))
       
-  case 'run commands':
-    run_commands(args.content)
+    case 'run commands':
+      run_commands(args.content)
 
 PLACEHOLDER = "I love placeholders! :)"
 
-def placeholder():
-  pass
```

### Comparing `term-chatgpt-1.1.5/termgpt/term.py` & `term-chatgpt-1.1.6/termgpt/term.py`

 * *Files identical despite different names*

