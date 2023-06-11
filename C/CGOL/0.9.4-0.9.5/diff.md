# Comparing `tmp/CGOL-0.9.4.tar.gz` & `tmp/CGOL-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CGOL-0.9.4.tar", last modified: Fri May 26 18:50:32 2023, max compression
+gzip compressed data, was "CGOL-0.9.5.tar", last modified: Sun Jun 11 13:48:55 2023, max compression
```

## Comparing `CGOL-0.9.4.tar` & `CGOL-0.9.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 neido     (1000) neido     (1000)        0 2023-05-26 18:50:32.717456 CGOL-0.9.4/
--rw-r--r--   0 neido     (1000) neido     (1000)    35149 2023-05-26 18:45:16.000000 CGOL-0.9.4/LICENSE
--rw-r--r--   0 neido     (1000) neido     (1000)     5626 2023-05-26 18:50:32.714123 CGOL-0.9.4/PKG-INFO
--rw-r--r--   0 neido     (1000) neido     (1000)     4819 2023-05-26 18:45:32.000000 CGOL-0.9.4/README.md
--rw-r--r--   0 neido     (1000) neido     (1000)     1025 2023-05-26 18:50:19.000000 CGOL-0.9.4/pyproject.toml
--rw-r--r--   0 neido     (1000) neido     (1000)       38 2023-05-26 18:50:32.717456 CGOL-0.9.4/setup.cfg
-drwxr-xr-x   0 neido     (1000) neido     (1000)        0 2023-05-26 18:50:32.714123 CGOL-0.9.4/src/
-drwxr-xr-x   0 neido     (1000) neido     (1000)        0 2023-05-26 18:50:32.714123 CGOL-0.9.4/src/CGOL.egg-info/
--rw-r--r--   0 neido     (1000) neido     (1000)     5626 2023-05-26 18:50:32.000000 CGOL-0.9.4/src/CGOL.egg-info/PKG-INFO
--rw-r--r--   0 neido     (1000) neido     (1000)      358 2023-05-26 18:50:32.000000 CGOL-0.9.4/src/CGOL.egg-info/SOURCES.txt
--rw-r--r--   0 neido     (1000) neido     (1000)        1 2023-05-26 18:50:32.000000 CGOL-0.9.4/src/CGOL.egg-info/dependency_links.txt
--rw-r--r--   0 neido     (1000) neido     (1000)       44 2023-05-26 18:50:32.000000 CGOL-0.9.4/src/CGOL.egg-info/entry_points.txt
--rw-r--r--   0 neido     (1000) neido     (1000)       13 2023-05-26 18:50:32.000000 CGOL-0.9.4/src/CGOL.egg-info/requires.txt
--rw-r--r--   0 neido     (1000) neido     (1000)        5 2023-05-26 18:50:32.000000 CGOL-0.9.4/src/CGOL.egg-info/top_level.txt
-drwxr-xr-x   0 neido     (1000) neido     (1000)        0 2023-05-26 18:50:32.714123 CGOL-0.9.4/src/cgol/
--rw-r--r--   0 neido     (1000) neido     (1000)      196 2023-05-26 18:45:16.000000 CGOL-0.9.4/src/cgol/__init__.py
--rw-r--r--   0 neido     (1000) neido     (1000)       81 2023-05-26 18:45:16.000000 CGOL-0.9.4/src/cgol/__main__.py
--rw-r--r--   0 neido     (1000) neido     (1000)    15834 2023-05-26 18:46:52.000000 CGOL-0.9.4/src/cgol/game.py
--rw-r--r--   0 neido     (1000) neido     (1000)     6162 2023-05-26 18:46:02.000000 CGOL-0.9.4/src/cgol/icon.png
--rw-r--r--   0 neido     (1000) neido     (1000)     7856 2023-05-26 18:45:16.000000 CGOL-0.9.4/src/cgol/parser.py
--rw-r--r--   0 neido     (1000) neido     (1000)     5888 2023-05-26 18:45:16.000000 CGOL-0.9.4/src/cgol/utils.py
--rw-r--r--   0 neido     (1000) neido     (1000)    10940 2023-05-26 18:45:16.000000 CGOL-0.9.4/src/cgol/world.py
+drwxr-xr-x   0 neido     (1000) neido     (1000)        0 2023-06-11 13:48:55.201281 CGOL-0.9.5/
+-rw-r--r--   0 neido     (1000) neido     (1000)    35149 2023-06-11 12:22:25.000000 CGOL-0.9.5/LICENSE
+-rw-r--r--   0 neido     (1000) neido     (1000)     5830 2023-06-11 13:48:55.201281 CGOL-0.9.5/PKG-INFO
+-rw-r--r--   0 neido     (1000) neido     (1000)     5023 2023-06-11 13:45:36.000000 CGOL-0.9.5/README.md
+-rw-r--r--   0 neido     (1000) neido     (1000)     1025 2023-06-11 13:46:45.000000 CGOL-0.9.5/pyproject.toml
+-rw-r--r--   0 neido     (1000) neido     (1000)       38 2023-06-11 13:48:55.201281 CGOL-0.9.5/setup.cfg
+drwxr-xr-x   0 neido     (1000) neido     (1000)        0 2023-06-11 13:48:55.197947 CGOL-0.9.5/src/
+drwxr-xr-x   0 neido     (1000) neido     (1000)        0 2023-06-11 13:48:55.197947 CGOL-0.9.5/src/CGOL.egg-info/
+-rw-r--r--   0 neido     (1000) neido     (1000)     5830 2023-06-11 13:48:55.000000 CGOL-0.9.5/src/CGOL.egg-info/PKG-INFO
+-rw-r--r--   0 neido     (1000) neido     (1000)      358 2023-06-11 13:48:55.000000 CGOL-0.9.5/src/CGOL.egg-info/SOURCES.txt
+-rw-r--r--   0 neido     (1000) neido     (1000)        1 2023-06-11 13:48:55.000000 CGOL-0.9.5/src/CGOL.egg-info/dependency_links.txt
+-rw-r--r--   0 neido     (1000) neido     (1000)       44 2023-06-11 13:48:55.000000 CGOL-0.9.5/src/CGOL.egg-info/entry_points.txt
+-rw-r--r--   0 neido     (1000) neido     (1000)       13 2023-06-11 13:48:55.000000 CGOL-0.9.5/src/CGOL.egg-info/requires.txt
+-rw-r--r--   0 neido     (1000) neido     (1000)        5 2023-06-11 13:48:55.000000 CGOL-0.9.5/src/CGOL.egg-info/top_level.txt
+drwxr-xr-x   0 neido     (1000) neido     (1000)        0 2023-06-11 13:48:55.201281 CGOL-0.9.5/src/cgol/
+-rw-r--r--   0 neido     (1000) neido     (1000)      196 2023-06-11 12:22:25.000000 CGOL-0.9.5/src/cgol/__init__.py
+-rw-r--r--   0 neido     (1000) neido     (1000)       81 2023-06-11 12:22:25.000000 CGOL-0.9.5/src/cgol/__main__.py
+-rw-r--r--   0 neido     (1000) neido     (1000)    17572 2023-06-11 13:48:38.000000 CGOL-0.9.5/src/cgol/game.py
+-rw-r--r--   0 neido     (1000) neido     (1000)     6162 2023-06-11 12:22:25.000000 CGOL-0.9.5/src/cgol/icon.png
+-rw-r--r--   0 neido     (1000) neido     (1000)     8333 2023-06-11 13:37:08.000000 CGOL-0.9.5/src/cgol/parser.py
+-rw-r--r--   0 neido     (1000) neido     (1000)     5888 2023-06-11 12:22:25.000000 CGOL-0.9.5/src/cgol/utils.py
+-rw-r--r--   0 neido     (1000) neido     (1000)    11293 2023-06-11 13:36:47.000000 CGOL-0.9.5/src/cgol/world.py
```

### Comparing `CGOL-0.9.4/LICENSE` & `CGOL-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CGOL-0.9.4/PKG-INFO` & `CGOL-0.9.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CGOL
-Version: 0.9.4
+Version: 0.9.5
 Summary: A whack Conway's Game of Life implementation.
 Author-email: Neido <reg@neido.de>
 Maintainer-email: Neido <reg@neido.de>
 License: GPL-3
 Project-URL: Homepage, https://github.com/INeido/CGOL/
 Project-URL: Repository, https://github.com/INeido/CGOL/
 Project-URL: Issues, https://github.com/INeido/CGOL/issues
@@ -145,10 +145,16 @@
 | D | Fill with dead cells. |
 | K | Kill alive cells. |
 | R | Reset game. |
 | L | Load last saved game. |
 | S | Save current game. |
 | C | Center view. |
 | P | Save screenshot. |
+| I | Toggle Insert Mode. |
+| Left Click | (Insert Mode) Place loaded pattern. |
+| Middle Scroll | (Insert Mode) Rotate loaded pattern. |
+| 1 | Load `1.rle`. |
+| 2 | Load `2.rle`. |
+| 3 | Load `3.rle`. |
 | Right Arrow | Forward one generation. |
 | + | Extend grid by one cell in every direction. |
 | - | Reduce grid by one cell in every direction. |
```

### Comparing `CGOL-0.9.4/README.md` & `CGOL-0.9.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -124,10 +124,16 @@
 | D | Fill with dead cells. |
 | K | Kill alive cells. |
 | R | Reset game. |
 | L | Load last saved game. |
 | S | Save current game. |
 | C | Center view. |
 | P | Save screenshot. |
+| I | Toggle Insert Mode. |
+| Left Click | (Insert Mode) Place loaded pattern. |
+| Middle Scroll | (Insert Mode) Rotate loaded pattern. |
+| 1 | Load `1.rle`. |
+| 2 | Load `2.rle`. |
+| 3 | Load `3.rle`. |
 | Right Arrow | Forward one generation. |
 | + | Extend grid by one cell in every direction. |
 | - | Reduce grid by one cell in every direction. |
```

### Comparing `CGOL-0.9.4/pyproject.toml` & `CGOL-0.9.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CGOL"
-version = "0.9.4"
+version = "0.9.5"
 description = "A whack Conway's Game of Life implementation."
 readme = "README.md"
 requires-python = ">=3"
 license = {text = "GPL-3"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
```

### Comparing `CGOL-0.9.4/src/CGOL.egg-info/PKG-INFO` & `CGOL-0.9.5/src/CGOL.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CGOL
-Version: 0.9.4
+Version: 0.9.5
 Summary: A whack Conway's Game of Life implementation.
 Author-email: Neido <reg@neido.de>
 Maintainer-email: Neido <reg@neido.de>
 License: GPL-3
 Project-URL: Homepage, https://github.com/INeido/CGOL/
 Project-URL: Repository, https://github.com/INeido/CGOL/
 Project-URL: Issues, https://github.com/INeido/CGOL/issues
@@ -145,10 +145,16 @@
 | D | Fill with dead cells. |
 | K | Kill alive cells. |
 | R | Reset game. |
 | L | Load last saved game. |
 | S | Save current game. |
 | C | Center view. |
 | P | Save screenshot. |
+| I | Toggle Insert Mode. |
+| Left Click | (Insert Mode) Place loaded pattern. |
+| Middle Scroll | (Insert Mode) Rotate loaded pattern. |
+| 1 | Load `1.rle`. |
+| 2 | Load `2.rle`. |
+| 3 | Load `3.rle`. |
 | Right Arrow | Forward one generation. |
 | + | Extend grid by one cell in every direction. |
 | - | Reduce grid by one cell in every direction. |
```

### Comparing `CGOL-0.9.4/src/cgol/game.py` & `CGOL-0.9.5/src/cgol/game.py`

 * *Files 17% similar despite different names*

```diff
@@ -229,25 +229,27 @@
 
             return int(x), int(y)
 
     def run(self, pause=False) -> None:
         """The main loop that runs the game.
         """
         # Flags
-        is_looping = True
         running = not pause
         draw = False
         drag = False
         prev_pos = None
+        insert_mode = False
+        rotation = 0
 
         while True:
             self.clock.tick(self.tickrate)
 
             # Save mouse position
             curr_pos = pygame.mouse.get_pos()
+            curr_pos_cell = int((curr_pos[0]-self.offset_x)//self.cell_size), int((curr_pos[1]-self.offset_y)//self.cell_size)
 
             # Screen drag
             if drag and prev_pos != None:
                 self.offset_x, self.offset_y = numpy.add(numpy.subtract(curr_pos, prev_pos), (oldoffset_x, oldoffset_y))
                 self.get_borders()
 
             # Event loop
@@ -265,14 +267,17 @@
                         running = not running
                     # ESCAPE pressed: Close game
                     if event.key == pygame.K_ESCAPE:
                         shutdown(pygame)
                     # Right Arrow pressed: Forward one generation
                     if event.key == pygame.K_RIGHT:
                         self.calc_generation()
+                    # I pressed: Insert Mode
+                    if event.key == pygame.K_i:
+                        insert_mode = not insert_mode
                     # R pressed: Reset game
                     if event.key == pygame.K_r:
                         self.world.populate("seed")
                     # F pressed: Fill with random cells
                     if event.key == pygame.K_f:
                         self.world.populate("random")
                     # A pressed: Fill with alive cells
@@ -282,89 +287,110 @@
                     if event.key == pygame.K_d:
                         self.world.populate("dead")
                     # K pressed: Kill alive cells
                     if event.key == pygame.K_k:
                         self.world.populate("kill")
                     # L pressed: Load last saved game
                     if event.key == pygame.K_l:
-                        self.world.load_list(CSV.decode(load_import(get_save_path("/cgol/exports/") + "save.csv")))
-                        self.get_borders()
+                        grid = CSV.decode(load_import(get_save_path("/cgol/exports/") + "save.csv"))
+                        if grid is not None:
+                            self.world.load_list(grid)
+                            self.get_borders()
                     # S pressed: Save current game
                     if event.key == pygame.K_s:
-                        save_export(CSV.encode((numpy.where(self.world.grid < 1, 0, 1))), get_save_path("/cgol/exports/") + "save.csv")
+                        grid = CSV.encode((numpy.where(self.world.grid < 1, 0, 1)))
+                        if grid is not None:
+                            save_export(grid, get_save_path("/cgol/exports/") + "save.csv")
                     # C pressed: Center view
                     if event.key == pygame.K_c:
                         self.center()
                         self.get_borders()
                     # P pressed: Save screenshot
                     if event.key == pygame.K_p:
-                        pygame.image.save(self.sur, f"{get_save_path() + str(self.world.generations)}.png")
+                        pygame.image.save(self.sur, f"{get_save_path('/cgol/images/') + str(self.world.seed) + str(self.world.generations)}.png")
                     # + pressed: Extend grid
                     if event.key == pygame.K_PLUS:
                         self.world.extend()
                         self.get_borders()
                     # - pressed: Reduce grid
                     if event.key == pygame.K_MINUS:
                         self.world.reduce()
                         self.get_borders()
+                    if event.key == pygame.K_1 and insert_mode:
+                        self.pattern = RLE.decode(load_import(get_save_path("/cgol/patterns/") + "1.rle"))
+                    if event.key == pygame.K_2 and insert_mode:
+                        self.pattern = RLE.decode(load_import(get_save_path("/cgol/patterns/") + "2.rle"))
+                    if event.key == pygame.K_3 and insert_mode:
+                        self.pattern = RLE.decode(load_import(get_save_path("/cgol/patterns/") + "3.rle"))
 
                 # Mouse events
                 elif event.type == pygame.MOUSEBUTTONDOWN:
-                    # Left/Right Click: Draw
-                    if event.button == 1 or event.button == 3:
-                        oldoffset_x, oldoffset_y = self.offset_x, self.offset_y
-                        prev_pos = curr_pos
-                        draw = True
-                    if event.button == 1:
-                        draw_color = 1
-                    if event.button == 3:
-                        draw_color = 0
-                    # Middle Mouse: Drag screen
-                    if event.button == 2:
-                        oldoffset_x, oldoffset_y = self.offset_x, self.offset_y
-                        prev_pos = curr_pos
-                        drag = True
+                    if insert_mode:
+                        if event.button == 1:
+                            try:
+                                if self.pattern is not None:
+                                    self.world.insert_pattern(numpy.array(self.pattern.decoded), curr_pos_cell, rotation)
+                            except AttributeError:
+                                print("Couldn't insert pattern.")
+                  
+                    else:
+                        # Left/Right Click: Draw
+                        if event.button == 1 or event.button == 3:
+                            oldoffset_x, oldoffset_y = self.offset_x, self.offset_y
+                            prev_pos = curr_pos
+                            draw = True
+                        if event.button == 1:
+                            draw_color = 1
+                        if event.button == 3:
+                            draw_color = 0
+                        # Middle Mouse: Drag screen
+                        if event.button == 2:
+                            oldoffset_x, oldoffset_y = self.offset_x, self.offset_y
+                            prev_pos = curr_pos
+                            drag = True
                 elif event.type == pygame.MOUSEBUTTONUP:
                     # Left/Right Click: Draw
                     if event.button == 1 or event.button == 3:
                         prev_pos = None
                         draw = False
                     # Middle Mouse: Drag screen
                     if event.button == 2:
                         prev_pos = None
                         drag = False
 
                 # Zoom
                 elif event.type == pygame.MOUSEWHEEL:
-                    if event.y == 1:
-                        self.cell_size *= 2
-                        self.offset_x = curr_pos[0] + (self.offset_x - curr_pos[0]) * 2
-                        self.offset_y = curr_pos[1] + (self.offset_y - curr_pos[1]) * 2
-                        self.get_borders()
-                    elif event.y == -1 and self.cell_size > 1:
-                        self.cell_size /= 2
-                        self.offset_x = curr_pos[0] + (self.offset_x - curr_pos[0]) / 2
-                        self.offset_y = curr_pos[1] + (self.offset_y - curr_pos[1]) / 2
-                        self.get_borders()
+                    if insert_mode:
+                        if event.y == 1:
+                            rotation += 1
+                        elif event.y == -1:
+                            rotation -= 1
+                    else:
+                        if event.y == 1:
+                            self.cell_size *= 2
+                            self.offset_x = curr_pos[0] + (self.offset_x - curr_pos[0]) * 2
+                            self.offset_y = curr_pos[1] + (self.offset_y - curr_pos[1]) * 2
+                            self.get_borders()
+                        elif event.y == -1 and self.cell_size > 1:
+                            self.cell_size /= 2
+                            self.offset_x = curr_pos[0] + (self.offset_x - curr_pos[0]) / 2
+                            self.offset_y = curr_pos[1] + (self.offset_y - curr_pos[1]) / 2
+                            self.get_borders()
 
             # Interpolate to prevent dotted line
-            if draw and prev_pos != None:
+            if draw and prev_pos != None and not insert_mode:
                 x, y = self.interpolate(prev_pos, curr_pos)
                 if isinstance(x, int) and isinstance(y, int):
                     if 0 <= x < self.world.grid_width and 0 <= y < self.world.grid_height:
                         self.world.grid[x, y] = draw_color or (0.5 if self.world.grid[x, y] == 1.0 and not draw_color else self.world.grid[x, y])
                 elif min(x) >= 0 and max(x) < self.world.grid_width and min(y) >= 0 and max(y) < self.world.grid_height:
                     for xc, yc in zip(x, y):
                         self.world.grid[xc, yc] = draw_color or (0.5 if self.world.grid[xc, yc] == 1.0 and not draw_color else self.world.grid[xc, yc])
                 prev_pos = curr_pos
 
-            # Break out of main loop
-            if not is_looping:
-                break
-
             # Draw before we start updating the cells
             self.draw()
 
             # Skip over generation to pause game
             if not running or draw:
                 continue
```

### Comparing `CGOL-0.9.4/src/cgol/icon.png` & `CGOL-0.9.5/src/cgol/icon.png`

 * *Files identical despite different names*

### Comparing `CGOL-0.9.4/src/cgol/parser.py` & `CGOL-0.9.5/src/cgol/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""COGL File Parser
+"""
+COGL File Parser
 """
 import csv as csv_
 
 
 class CSV:
     """A pretty basic CSV parser.
 
@@ -31,19 +32,19 @@
     def decode(string: str) -> list:
         """Loads the Grid from a CSV string.
 
         :param str string: The string to be decoded.
         :return: The decoded array.
         :rtype: array
         """
-        reader = csv_.reader(string.split('\n'), delimiter=',')
-        result = []
-        row = []
-
         try:
+            reader = csv_.reader(string.split('\n'), delimiter=',')
+            result = []
+            row = []
+
             for row_ in reader:
                 for x in row_:
                     if x == "1" or x == "0":
                         row.append(int(x))
                 if len(row) != 0:
                     result.append(row)
                     row = []
@@ -56,15 +57,14 @@
 class RLE:
     """A Run Length Encoded file parser.
 
     https://conwaylife.com/wiki/Run_Length_Encoded
     """
 
     def encode(array, name: str, author: str = "", comments: str = "", rule="B3/S23"):
-        print(array)
         parser = RLE(len(array), len(array[0]), rule, name, author, comments)
 
         # Add the header rows
         parser.encode_header()
 
         # Add the rules
         parser.encode_rules()
@@ -73,14 +73,18 @@
         parser.encode_pattern(array)
 
         return parser
 
     def decode(text: str):
         parser = RLE()
 
+        if text is None:
+            print("Got a NoneType string.")
+            return None
+
         # Parse the file line by line
         for line in text.split("\n"):
             parser.decode_line(line)
 
         # Decode the extracted pattern string
         parser.decode_pattern()
 
@@ -184,15 +188,15 @@
         if line[1:].startswith("C"):
             self.comments += line[2:] + "\n"
         elif line[1:].startswith("O"):
             self.author = line[2:]
         elif line[1:].startswith("N"):
             self.name = line[2:]
         else:
-            raise Exception("Unknown header,")
+            raise Exception("Unknown header.")
 
     def decode_rule(self, line: str) -> None:
         """Extracts rules by splitting after the ',' and '='.
 
         Rules commonly look like this:
         x = 12, y = 10
         But they can also have a 'rule' variable determining the game rules:
@@ -209,44 +213,51 @@
         # Third rule is not mandatory
         try:
             r_parts = parts[2].split("=")
             self.rule = r_parts[1].strip()
         except:
             pass
 
+        if self.rule != "B3/S23" and self.rule != "":
+            raise Exception("Sorry, cant decode a pattern using rule " + self.rule)
+
     def decode_pattern(self) -> None:
         """Decodes the pattern string and write the array into self.decoded.
 
         The rules are as follows:
         b = Dead cell
         o = Alive cell
         $ = New row
         ! = End of string
         Any number in front of b or o is a multiplier. (So 2b is [0, 0].)
         Dead cells at the end of a row can be omitted.
         """
         result = []
         row = []
-        multiplier = 1
+        multiplier = None
 
         for char in self.encoded:
             if char == 'b':
-                row.extend([0] * multiplier)
-                multiplier = 1
+                row.extend([0] * (1 if multiplier is None else multiplier))
+                multiplier = None
             elif char == 'o':
-                row.extend([1] * multiplier)
-                multiplier = 1
+                row.extend([1] * (1 if multiplier is None else multiplier))
+                multiplier = None
             elif char == '$':
                 row.extend([0] * (self.width - len(row)))
                 if len(row) > self.width:
                     raise Exception("Line too long for pattern width.")
                 result.append(row)
                 row = []
             elif char.isdigit():
-                if multiplier > 1:
+                if multiplier is not None:
                     multiplier = int(str(multiplier) + char)
                 else:
                     multiplier = int(char)
             elif char == '!':
+                row.extend([0] * (self.width - len(row)))
+                if len(row) > self.width:
+                    raise Exception("Line too long for pattern width.")
                 result.append(row)
                 break
+
         self.decoded = result
```

### Comparing `CGOL-0.9.4/src/cgol/utils.py` & `CGOL-0.9.5/src/cgol/utils.py`

 * *Files identical despite different names*

### Comparing `CGOL-0.9.4/src/cgol/world.py` & `CGOL-0.9.5/src/cgol/world.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,24 @@
     def backup(self) -> None:
         """Creates a shallow copy of the grid.
         """
         temp = numpy.copy(self.grid_backup_0)
         self.grid_backup_0 = numpy.copy(self.grid)
         self.grid_backup_1 = numpy.copy(temp)
 
+    def insert_pattern(self, pattern, pos, rotation=0) -> None:
+        if not isinstance(pattern, numpy.ndarray) or pattern.ndim < 2:
+            print("Error: Invalid pattern array")
+            return
+
+        pattern = numpy.rot90(pattern, k=rotation)
+        x, y = pos
+
+        self.grid[x:x + pattern.shape[0], y:y + pattern.shape[1]] = pattern
+
     def check_stalemate(self) -> bool:
         """Compares the last backup with the current grid to see of it changed.
 
         :return: Is the backup the same as the current grid?
         :rtype: bool
         """
         return numpy.array_equal(self.grid, self.grid_backup_0)
```

