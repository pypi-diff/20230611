# Comparing `tmp/conlay-1.0.4.tar.gz` & `tmp/conlay-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conlay-1.0.4.tar", last modified: Fri Jun  9 14:34:46 2023, max compression
+gzip compressed data, was "conlay-1.0.5.tar", last modified: Sun Jun 11 18:08:53 2023, max compression
```

## Comparing `conlay-1.0.4.tar` & `conlay-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 14:34:46.928444 conlay-1.0.4/
--rw-rw-rw-   0        0        0     1085 2023-06-09 13:08:51.000000 conlay-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1543 2023-06-09 14:34:46.926823 conlay-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-06-09 14:30:21.000000 conlay-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 14:34:46.919322 conlay-1.0.4/conlay/
--rw-rw-rw-   0        0        0       19 2023-06-09 13:59:21.000000 conlay-1.0.4/conlay/__init__.py
--rw-rw-rw-   0        0        0    11535 2023-06-09 14:30:53.000000 conlay-1.0.4/conlay/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 14:34:46.925823 conlay-1.0.4/conlay.egg-info/
--rw-rw-rw-   0        0        0     1543 2023-06-09 14:34:46.000000 conlay-1.0.4/conlay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-06-09 14:34:46.000000 conlay-1.0.4/conlay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 14:34:46.000000 conlay-1.0.4/conlay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-09 14:34:46.000000 conlay-1.0.4/conlay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 14:34:46.928444 conlay-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-06-09 14:31:29.000000 conlay-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 18:08:53.559387 conlay-1.0.5/
+-rw-rw-rw-   0        0        0     1085 2023-06-09 13:08:51.000000 conlay-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0    22904 2023-06-11 18:08:53.557662 conlay-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    22599 2023-06-11 17:05:41.000000 conlay-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 18:08:53.549660 conlay-1.0.5/conlay/
+-rw-rw-rw-   0        0        0       19 2023-06-09 13:59:21.000000 conlay-1.0.5/conlay/__init__.py
+-rw-rw-rw-   0        0        0    11375 2023-06-11 16:52:38.000000 conlay-1.0.5/conlay/main.py
+drwxrwxrwx   0        0        0        0 2023-06-11 18:08:53.556161 conlay-1.0.5/conlay.egg-info/
+-rw-rw-rw-   0        0        0    22904 2023-06-11 18:08:53.000000 conlay-1.0.5/conlay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-06-11 18:08:53.000000 conlay-1.0.5/conlay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 18:08:53.000000 conlay-1.0.5/conlay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-11 18:08:53.000000 conlay-1.0.5/conlay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 18:08:53.559387 conlay-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      685 2023-06-11 18:08:20.000000 conlay-1.0.5/setup.py
```

### Comparing `conlay-1.0.4/LICENSE` & `conlay-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `conlay-1.0.4/conlay/main.py` & `conlay-1.0.5/conlay/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,18 +35,14 @@
         self.bottom_right = u"\u256F"
 
 
 
 
 class Color:
     """ color set """
-    
-    # clear color
-    clear = "\x1b[0m"
-
 
     class Bg:
         """ background color set """
 
         # clear background color
         clear = "\x1b[49m"
 
@@ -108,15 +104,15 @@
     def eraseLineToEnd() -> int:
         """ erase line from cursor to end """
 
         print("\x1b[0K", end="")
         return 1
     
 
-    def eraseLinefromStart() -> int:
+    def eraseLineFromStart() -> int:
         """ erase line from start to cursor """
 
         print("\x1b[1K", end="")
         return 1
     
 
     def eraseLine() -> int:
@@ -147,15 +143,15 @@
             return 1
         elif sh > 0:
             print("\x1b[{sh}C".format(sh=sh), end="")
             return 1
         return 0
 
 
-    def shiftVertikal(sh:int) -> int:
+    def shiftVertical(sh:int) -> int:
         """ shift cursor position on y axis
             value > 0: shift down
             value < 0: shift up """
 
         if sh < 0:
             print("\x1b[{sh}A".format(sh=sh*-1), end="")
             return 1
@@ -183,17 +179,16 @@
 
 class Conlay:
     """ main layout """
 
     # child list
     childs = []
 
-    # reset console and set cursor to (0, 0) after class call
+    # reset console
     Console.reset()
-    Cursor.setPosition(1, 1)
 
     def __init__(self) -> None:
         # class attributes
         self.relative_x = int()
         self.relative_y = int()
         self.absolute_x = int()
         self.absolute_y = int()
@@ -204,17 +199,17 @@
         self.min_height = int()
         self.max_height = int()
         self.zindex = int()
         self.padding_x = int()
         self.padding_y = int()
         self.text = str()
         self.background = bool()
-        self.background_color = Color.clear
-        self.border_color = Color.clear
-        self.text_color = Color.clear
+        self.background_color = Color.Bg.clear
+        self.border_color = Color.Fg.clear
+        self.text_color = Color.Fg.clear
 
 
     def __sort_childs_by_zindex__(self, reverse=False) -> list:
         """ sort child list by elements zindex attribute """
         
         return list(sorted(self.childs, key=lambda child: child.zindex, reverse=reverse))
     
@@ -234,55 +229,53 @@
     def __get_final_cursor_position__(self) -> int:
         """ calculate final cursor position """
 
         biggest_child = list(sorted(self.childs, key=lambda child: child.height + child.absolute_y, reverse=True))[0]
         return int(biggest_child.height + biggest_child.absolute_y) + 1
 
 
-    def add(self, element:None) -> int: 
+    def add(self, child:None) -> int: 
         """ add element to layout element """
 
         # set childs zindex to self zindex + 1
-        element.zindex = self.zindex + 1
+        child.zindex = self.zindex + 1
         
         # calculate childs absolute position based on self position, padding and childs relative position
-        element.absolute_x = self.absolute_x + self.padding_x + element.relative_x
-        element.absolute_y = self.absolute_y + self.padding_y + element.relative_y
+        child.absolute_x = self.absolute_x + self.padding_x + child.relative_x
+        child.absolute_y = self.absolute_y + self.padding_y + child.relative_y
 
         # calculate childs height, width based on min- and max- width/height
         if self.min_width != self.max_width and self.min_width < self.max_width and self.min_width >= 0:
-            element.width = min(max(element.min_width, element.width), element.max_width)
-            element.height = min(max(element.min_height, element.height), element.max_height)
+            child.width = min(max(child.min_width, child.width), child.max_width)
+            child.height = min(max(child.min_height, child.height), child.max_height)
+
+        try:
+            child.__preprint__()
+        except AttributeError:
+            pass
 
         # append child to layouts child list
-        self.childs.append(element)
+        self.childs.append(child)
         
         return 1
     
 
     def print(self) -> int:
         """ print layout """
 
+
         for element in self.__sort_childs_by_zindex__():
             # iterate through elements in child list sorted by zindex
 
-            # try elements pre-printing function
-            try:
-                element.__preprint__()
-            except AttributeError:
-                pass
-            
-
             # iterate through y axis
             for y in range(element.height):
 
                 # set cursors position
                 Cursor.setPosition(element.absolute_x, element.absolute_y + y)
 
-
                 # iterate through x axis
                 for x in range(element.width):
 
                     # print top left border
                     if x == 0 and y == 0:
                         print(element.background_color + element.border_color + element.border.top_left, end=Color.clear)
                     
@@ -309,20 +302,22 @@
                     # background behavior
                     else:
                         if element.background:
                             print(element.background_color + element.border_color + " ", end=Color.clear)
                         else:
                             Cursor.shiftHorizontal(1)
 
-
-            # try elements past-printing function
+            # try elements specific print function
             try:
-                element.__pastprint__()
+                element.__print__()
             except AttributeError:
                 pass
+            
+            # fixes pythons print bug
+            print()
         
         # set cursor position
         Cursor.setPosition(0, self.__get_final_cursor_position__())
 
 
 
 
@@ -377,15 +372,15 @@
     def __preprint__(self) -> int:
         self.width = self.width + self.padding_x * 2 + 2
         self.height = self.height + self.padding_y * 2 + 2
 
         return 1
 
 
-    def __pastprint__(self) -> int:
+    def __print__(self) -> int:
         Cursor.setPosition(self.absolute_x + 1 + self.padding_x, self.absolute_y + 1 + self.padding_y)
         print(self.text, end="")
 
         return 1
 
 
 class ThinLabel(Label):
```

### Comparing `conlay-1.0.4/setup.py` & `conlay-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = "1.0.4"
+VERSION = "1.0.5"
 
 with open("README.md", "r", encoding="utf-8") as readme:
     DESC_LONG = readme.read()
 
 
 setuptools.setup(
     name="conlay",
```

