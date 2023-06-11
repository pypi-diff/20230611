# Comparing `tmp/tktermwidget-0.0.2.tar.gz` & `tmp/tktermwidget-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tktermwidget-0.0.2.tar", last modified: Fri Jun  2 23:38:56 2023, max compression
+gzip compressed data, was "tktermwidget-0.0.3.tar", last modified: Sun Jun 11 03:02:26 2023, max compression
```

## Comparing `tktermwidget-0.0.2.tar` & `tktermwidget-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:38:56.053158 tktermwidget-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-02 23:38:30.000000 tktermwidget-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-02 23:38:56.053158 tktermwidget-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-02 23:38:30.000000 tktermwidget-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-02 23:38:30.000000 tktermwidget-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 23:38:56.053158 tktermwidget-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-02 23:38:30.000000 tktermwidget-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:38:56.053158 tktermwidget-0.0.2/tktermwidget/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 23:38:30.000000 tktermwidget-0.0.2/tktermwidget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-06-02 23:38:30.000000 tktermwidget-0.0.2/tktermwidget/tkterm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:38:56.053158 tktermwidget-0.0.2/tktermwidget.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-02 23:38:56.000000 tktermwidget-0.0.2/tktermwidget.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-02 23:38:56.000000 tktermwidget-0.0.2/tktermwidget.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 23:38:56.000000 tktermwidget-0.0.2/tktermwidget.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 23:38:56.000000 tktermwidget-0.0.2/tktermwidget.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:02:26.074513 tktermwidget-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-11 03:02:07.000000 tktermwidget-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-11 03:02:26.074513 tktermwidget-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-11 03:02:07.000000 tktermwidget-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-11 03:02:07.000000 tktermwidget-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 03:02:26.074513 tktermwidget-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-11 03:02:07.000000 tktermwidget-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:02:26.074513 tktermwidget-0.0.3/tktermwidget/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 03:02:07.000000 tktermwidget-0.0.3/tktermwidget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-11 03:02:07.000000 tktermwidget-0.0.3/tktermwidget/tkterm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:02:26.074513 tktermwidget-0.0.3/tktermwidget.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-11 03:02:26.000000 tktermwidget-0.0.3/tktermwidget.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-11 03:02:26.000000 tktermwidget-0.0.3/tktermwidget.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 03:02:26.000000 tktermwidget-0.0.3/tktermwidget.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-11 03:02:26.000000 tktermwidget-0.0.3/tktermwidget.egg-info/top_level.txt
```

### Comparing `tktermwidget-0.0.2/LICENSE` & `tktermwidget-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tktermwidget-0.0.2/PKG-INFO` & `tktermwidget-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: tktermwidget
-Version: 0.0.2
+Version: 0.0.3
 Summary: A terminal emulator for Tkinter
 Home-page: https://github.com/littlewhitecloud/TkTerminal
 Author: littlewhitecloud
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# `tkterm`
-
-> A terminal emulator written in Python using tkinter
+# TkTerminal
+A terminal emulator written in Python using tkinter
 
 ## Views:
 ### Windows
 <img src="images/windows.png" width="85%" align="center">
 
 ### MacOS
 <img src="images/macos.png" width="85%" align="center">
@@ -57,9 +56,11 @@
 # Show root window
 root.deiconify()
 
 # Start mainloop
 root.mainloop()
 ```
 
-### Coming soon
-
+## Install:
+```batch
+pip install tktermwidget
+```
```

### Comparing `tktermwidget-0.0.2/README.md` & `tktermwidget-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# `tkterm`
-
-> A terminal emulator written in Python using tkinter
+# TkTerminal
+A terminal emulator written in Python using tkinter
 
 ## Views:
 ### Windows
 <img src="images/windows.png" width="85%" align="center">
 
 ### MacOS
 <img src="images/macos.png" width="85%" align="center">
@@ -48,9 +47,11 @@
 # Show root window
 root.deiconify()
 
 # Start mainloop
 root.mainloop()
 ```
 
-### Coming soon
-
+## Install:
+```batch
+pip install tktermwidget
+```
```

### Comparing `tktermwidget-0.0.2/tktermwidget/tkterm.py` & `tktermwidget-0.0.3/tktermwidget/tkterm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+"""Terminal widget for tkinter"""
 from __future__ import annotations
 
 from os import getcwd
 from pathlib import Path
 from platform import system
 from subprocess import PIPE, Popen
 from tkinter import Event, Misc, Text
 from tkinter.ttk import Frame, Scrollbar
 
 from platformdirs import user_cache_dir
 
 # Set constants
-
 HISTORY_PATH = Path(user_cache_dir("tkterm"))
 SYSTEM = system()
 CREATE_NEW_CONSOLE = 0
 DIR = "{command}$ "
 if SYSTEM == "Windows":
     from subprocess import CREATE_NEW_CONSOLE
 
@@ -26,29 +26,26 @@
     # Also create the history file
     open(HISTORY_PATH / "history.txt", "w").close()
 
 # Check that the history file exists
 if not (HISTORY_PATH / "history.txt").exists():
     open(HISTORY_PATH / "history.txt", "w").close()
 
-
 class AutoHideScrollbar(Scrollbar):
     """Scrollbar that automatically hides when not needed"""
 
     def __init__(self, master=None, **kwargs):
         Scrollbar.__init__(self, master=master, **kwargs)
 
-    def set(self, length, height):
-        if float(length) <= 0.0 and float(height) >= 1.0:
+    def set(self, first: int, last: int):
+        if float(first) <= 0.0 and float(last) >= 1.0:
             self.grid_remove()
         else:
             self.grid()
-
-        Scrollbar.set(self, length, height)
-
+        Scrollbar.set(self, first, last)
 
 class Terminal(Frame):
     """A terminal widget for tkinter applications
 
     Args:
         master (Misc): The parent widget
         autohide (bool, optional): Whether to autohide the scrollbars. Defaults to True.
@@ -56,16 +53,18 @@
         **kwargs: Keyword arguments for the text widget
 
     Methods for outside use:
         None
 
     Methods for internal use:
         up (Event) -> str: Goes up in the history
-        down (Event) -> str: Goes down in the history (if the user is at the bottom of the history, it clears the command)
-        left (Event) -> str: Goes left in the command if the index is greater than the length of the directory (so the user can't delete the directory or go left of it)
+        down (Event) -> str: Goes down in the history 
+        (if the user is at the bottom of the history, it clears the command)
+        left (Event) -> str: Goes left in the command if the index is greater than the length of the directory
+        (so the user can't delete the directory or go left of it)
         kill (Event) -> str: Kills the current command
         loop (Event) -> str: Runs the command typed"""
 
     def __init__(self, master: Misc, autohide: bool = True, *args, **kwargs):
         Frame.__init__(self, master)
 
         # Set row and column weights
@@ -94,70 +93,68 @@
 
         # Grid widgets
         self.text.grid(row=0, column=0, sticky="nsew")
         self.xscroll.grid(row=1, column=0, sticky="ew")
         self.yscroll.grid(row=0, column=1, sticky="ns")
 
         # Create command prompt
-        self.text.insert(
-            "insert",
-            f"{DIR.format(command=getcwd())}",
-        )
+        self.directory()
 
         # Set variables
         self.index = 1
         self.current_process: Popen | None = None
 
-        # Bind events
+        # Bind events & tags
         self.text.bind("<Up>", self.up, add=True)
         self.text.bind("<Down>", self.down, add=True)
         self.text.bind("<Left>", self.left, add=True)
-        self.text.bind("<BackSpace>", self.left, add=True)
-        self.text.bind("<Control-KeyPress-c>", self.kill, add=True)  # Isn't working
         self.text.bind("<Return>", self.loop, add=True)
+        self.text.bind("<BackSpace>", self.left, add=True)
+
+        # TODO: Refactor the way we get output from subprocess
+        self.text.bind("<Control-KeyPress-c>", self.kill, add=True) # Isn't working
 
         # History recorder
         self.history = open(HISTORY_PATH / "history.txt", "r+")
         self.historys = [i.strip() for i in self.history.readlines() if i.strip()]
         self.hi = len(self.historys) - 1
 
+
+    def directory(self):
+        """Insert the directory"""
+        self.text.insert(
+            "insert",
+            f"{DIR.format(command=getcwd())}",
+        )
+
     def up(self, _: Event) -> str:
         """Go up in the history"""
         if self.hi >= 0:
             self.text.delete(f"{self.index}.0", "end-1c")
             # Insert the directory
-            self.text.insert(
-                "insert",
-                f"{DIR.format(command=getcwd())}",
-            )
+            self.directory()
             # Insert the command
             self.text.insert("insert", self.historys[self.hi].strip())
             self.hi -= 1
         return "break"
 
     def down(self, _: Event) -> str:
         """Go down in the history"""
         if self.hi < len(self.historys) - 1:
             self.text.delete(f"{self.index}.0", "end-1c")
             # Insert the directory
-            self.text.insert(
-                "insert",
-                f"{DIR.format(command=getcwd())}",
-            )
+            self.directory()
             # Insert the command
             self.text.insert("insert", self.historys[self.hi].strip())
             self.hi += 1
         else:
             # Clear the command
             self.text.delete(f"{self.index}.0", "end-1c")
             # Insert the directory
-            self.text.insert(
-                "insert",
-                f"{DIR.format(command=getcwd())}",
-            )
+            self.directory()
         return "break"
 
     def left(self, _: Event) -> str:
         """Go left in the command if the command is greater than the path"""
         insert_index = self.text.index("insert")
         dir_index = f"{insert_index.split('.')[0]}.{len(DIR.format(command=getcwd()))}"
         if insert_index == dir_index:
@@ -170,67 +167,66 @@
             self.current_process = None
         return "break"
 
     def loop(self, _: Event) -> str:
         """Create an input loop"""
         cmd = self.text.get(f"{self.index}.0", "end-1c")
         # Determine command based on system
-        cmd = cmd.split("$")[-1]  # Unix
-        if SYSTEM == "Windows":
-            cmd = cmd.split(">")[-1].strip()
+        cmd = cmd.split("$")[-1].strip() if not SYSTEM == "Windows" else cmd.split(">")[-1].strip()
 
         # Record the command
         if cmd != "":
             self.history.write(cmd + "\n")
             self.historys.append(cmd)
             self.hi = len(self.historys) - 1
+        else:
+            self.text.insert("insert", "\n")
+            self.index += 1
+            self.directory()
+            return "break"
 
         # Check that the insert position is at the end
         if self.text.index("insert") != f"{self.index}.end":
             self.text.mark_set("insert", f"{self.index}.end")
             self.text.see("insert")
 
         # If the command is "clear" or "cls", clear the screen
         if cmd in ["clear", "cls"]:
             self.text.delete("1.0", "end")
-            self.text.insert(
-                "insert",
-                f"{DIR.format(command=getcwd())}",
-            )
+            self.directory()
             return "break"
 
         self.current_process = Popen(
             cmd,
             shell=True,
             stdout=PIPE,
             stderr=PIPE,
             stdin=PIPE,
             text=True,
-            cwd=getcwd(),  # Until a solution for changing the working directory is found, this will have to do
+            cwd=getcwd(), # Until a solution for changing the working directory is found, this will have to do
             creationflags=CREATE_NEW_CONSOLE,
-        )  # The following needs to be put in an after so the kill command works and the program doesn't freeze
+        )
+        # The following needs to be put in an after so the kill command works and the program doesn't freeze
+
         # Check if the command was successful
-        returncode = self.current_process.wait()
-        process = self.current_process
+        returnlines, errors, = self.current_process.communicate()
+        returncode = self.current_process.returncode
         self.current_process = None
-        returnlines = process.stdout.readlines()
         if returncode != 0:
-            returnlines += process.stderr.readlines()  # If the command was unsuccessful, it doesn't give stdout
+            returnlines += errors # If the command was unsuccessful, it doesn't give stdout
             # TODO: Get the success message from the command (see #16)
 
         self.text.insert("insert", "\n")
         self.index += 1
         for line in returnlines:
             self.text.insert("insert", line)
-            self.index += 1
+            if line == "\n":
+                self.index += 1
 
-        self.text.insert(
-            "insert",
-            f"{DIR.format(command=getcwd())}",
-        )
+        self.directory()
         return "break"  # Prevent the default newline character insertion
 
 
 if __name__ == "__main__":
     from tkinter import Tk
 
     # Create root window
@@ -247,15 +243,15 @@
     term.pack(expand=True, fill="both")
 
     # Set minimum size and center app
 
     # Update widgets so minimum size is accurate
     root.update_idletasks()
 
-    # Get minimum size
+    # Set the minimum size
     minimum_width: int = root.winfo_reqwidth()
     minimum_height: int = root.winfo_reqheight()
 
     # Get center of screen based on minimum size
     x_coords = int(root.winfo_screenwidth() / 2 - minimum_width / 2)
     y_coords = int(root.wm_maxsize()[1] / 2 - minimum_height / 2)
     # Place app and make the minimum size the actual minimum size (non-infringable)
```

### Comparing `tktermwidget-0.0.2/tktermwidget.egg-info/PKG-INFO` & `tktermwidget-0.0.3/tktermwidget.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: tktermwidget
-Version: 0.0.2
+Version: 0.0.3
 Summary: A terminal emulator for Tkinter
 Home-page: https://github.com/littlewhitecloud/TkTerminal
 Author: littlewhitecloud
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# `tkterm`
-
-> A terminal emulator written in Python using tkinter
+# TkTerminal
+A terminal emulator written in Python using tkinter
 
 ## Views:
 ### Windows
 <img src="images/windows.png" width="85%" align="center">
 
 ### MacOS
 <img src="images/macos.png" width="85%" align="center">
@@ -57,9 +56,11 @@
 # Show root window
 root.deiconify()
 
 # Start mainloop
 root.mainloop()
 ```
 
-### Coming soon
-
+## Install:
+```batch
+pip install tktermwidget
+```
```

