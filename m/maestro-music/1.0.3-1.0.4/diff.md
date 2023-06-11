# Comparing `tmp/maestro-music-1.0.3.tar.gz` & `tmp/maestro-music-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestro-music-1.0.3.tar", last modified: Thu Jun  8 06:15:43 2023, max compression
+gzip compressed data, was "maestro-music-1.0.4.tar", last modified: Sun Jun 11 17:24:11 2023, max compression
```

## Comparing `maestro-music-1.0.3.tar` & `maestro-music-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-06-08 06:15:43.855413 maestro-music-1.0.3/
--rw-r--r--   0 sysadmin   (501) staff       (20)     1067 2023-06-06 05:56:48.000000 maestro-music-1.0.3/LICENSE
--rw-r--r--   0 sysadmin   (501) staff       (20)    10863 2023-06-08 06:15:43.855203 maestro-music-1.0.3/PKG-INFO
--rw-r--r--   0 sysadmin   (501) staff       (20)    40364 2023-06-08 00:47:48.000000 maestro-music-1.0.3/helpers.py
--rw-r--r--   0 sysadmin   (501) staff       (20)   146639 2023-03-25 20:23:16.000000 maestro-music-1.0.3/icon.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     8837 2023-06-08 00:47:48.000000 maestro-music-1.0.3/mac_presence.py
--rw-r--r--   0 sysadmin   (501) staff       (20)   111717 2023-06-08 06:14:20.000000 maestro-music-1.0.3/maestro.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-06-08 06:15:43.854915 maestro-music-1.0.3/maestro_music.egg-info/
--rw-r--r--   0 sysadmin   (501) staff       (20)    10863 2023-06-08 06:15:43.000000 maestro-music-1.0.3/maestro_music.egg-info/PKG-INFO
--rw-r--r--   0 sysadmin   (501) staff       (20)      286 2023-06-08 06:15:43.000000 maestro-music-1.0.3/maestro_music.egg-info/SOURCES.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)        1 2023-06-08 06:15:43.000000 maestro-music-1.0.3/maestro_music.egg-info/dependency_links.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)       40 2023-06-08 06:15:43.000000 maestro-music-1.0.3/maestro_music.egg-info/entry_points.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)      367 2023-06-08 06:15:43.000000 maestro-music-1.0.3/maestro_music.egg-info/requires.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)       34 2023-06-08 06:15:43.000000 maestro-music-1.0.3/maestro_music.egg-info/top_level.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)       38 2023-06-08 06:15:43.855462 maestro-music-1.0.3/setup.cfg
--rw-r--r--   0 sysadmin   (501) staff       (20)     1646 2023-06-08 06:15:38.000000 maestro-music-1.0.3/setup.py
+drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-06-11 17:24:11.975870 maestro-music-1.0.4/
+-rw-r--r--   0 sysadmin   (501) staff       (20)     1067 2023-06-06 05:56:48.000000 maestro-music-1.0.4/LICENSE
+-rw-r--r--   0 sysadmin   (501) staff       (20)    10945 2023-06-11 17:24:11.975650 maestro-music-1.0.4/PKG-INFO
+-rw-r--r--   0 sysadmin   (501) staff       (20)    40729 2023-06-11 17:22:31.000000 maestro-music-1.0.4/helpers.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)   146639 2023-03-25 20:23:16.000000 maestro-music-1.0.4/icon.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)     8837 2023-06-08 00:47:48.000000 maestro-music-1.0.4/mac_presence.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)   111717 2023-06-08 06:29:07.000000 maestro-music-1.0.4/maestro.py
+drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-06-11 17:24:11.975391 maestro-music-1.0.4/maestro_music.egg-info/
+-rw-r--r--   0 sysadmin   (501) staff       (20)    10945 2023-06-11 17:24:11.000000 maestro-music-1.0.4/maestro_music.egg-info/PKG-INFO
+-rw-r--r--   0 sysadmin   (501) staff       (20)      286 2023-06-11 17:24:11.000000 maestro-music-1.0.4/maestro_music.egg-info/SOURCES.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)        1 2023-06-11 17:24:11.000000 maestro-music-1.0.4/maestro_music.egg-info/dependency_links.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)       40 2023-06-11 17:24:11.000000 maestro-music-1.0.4/maestro_music.egg-info/entry_points.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)      367 2023-06-11 17:24:11.000000 maestro-music-1.0.4/maestro_music.egg-info/requires.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)       34 2023-06-11 17:24:11.000000 maestro-music-1.0.4/maestro_music.egg-info/top_level.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)       38 2023-06-11 17:24:11.975937 maestro-music-1.0.4/setup.cfg
+-rw-r--r--   0 sysadmin   (501) staff       (20)     1646 2023-06-11 17:24:07.000000 maestro-music-1.0.4/setup.py
```

### Comparing `maestro-music-1.0.3/LICENSE` & `maestro-music-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `maestro-music-1.0.3/PKG-INFO` & `maestro-music-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestro-music
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple command line tool to play songs (or any audio files, really).
 Home-page: https://github.com/PrajwalVandana/maestro-cli
 Author: Prajwal Vandana
 License: MIT
 Keywords: music,sound,audio,music-player,cli,ogg,flac,mp3,wav,spotify,youtube,audio-visualization,audio-visualizer
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -147,14 +147,16 @@
 
 List details for a specific song.
 
 ### `maestro list`
 
 List songs (or tags) and details. Use `maestro list -h` to see full options (e.g. sort, list only songs with a certain tag, etc.).
 
+![maestro list example](data/list.png)
+
 ### `maestro play`
 
 Play songs. Use `maestro play -h` to see full options. Has lots of features:
 - pass tag(s) as arguments to play songs with any of those tag(s) (or songs with all of those tag(s) if you pass the `-M` or `--match-all` flag)
 - shuffle playlist with the `-s` or `--shuffle option (shuffle once, shuffle everytime the playlist repeats, or shuffle everytime the playlist repeats except the first)
 - play songs in reverse order with the `-R` or `--reverse` flag
 - loop playlist with the `-L` or `--loop` flag
@@ -177,14 +179,16 @@
 - `i` to insert a song by ID after the currently playing song
 - `b` or `p` to go back to the previous song
 - `s` or `n` to go to the next song
 - space to pause/play
 - `e` to end after the current song
 - `q` to end immediately (don't just close the window or `CTRL-c`, this messes up the accuracy of the listen time statistics)
 
+![maestro play example](data/player.png)
+
 ### `maestro push`
 
 Push a song to the top (or bottom) of your song list. Useful, for example, if you usually play the most recently added songs first (`maestro play -R`)—you can use `maestro push` to push a song to the top of your list so it's the first song to play.
 
 ### `maestro recommend` (experimental)
 
 Recommend songs similar to a song title (specified directly or by ID) using YouTube Music. Equivalent to searching for the title of the song on YouTube Music, clicking on the first "Song" result, and then looking at the "Up Next" section.
```

### Comparing `maestro-music-1.0.3/helpers.py` & `maestro-music-1.0.4/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,24 +297,27 @@
         self.volume = volume
         self.clip_mode = clip_mode
         self.update_discord = update_discord
         self.visualize = visualize  # want to visualize
         self.can_visualize = LIBROSA is not None  # can generate visualization
         # space to show visualization
         self.can_show_visualization = (
-            self.can_visualize
+            self.visualize
+            and self.can_visualize
             and self.stdscr.getmaxyx()[0] > VISUALIZER_HEIGHT + 5
         )
         if self.visualize and self.can_visualize:
             t = threading.Thread(
                 target=self.load_visualizer_data,
                 daemon=True,
             )
             self.visualizer_data = {}
             t.start()
+        else:
+            self.visualizer_data = None
 
         self.looping_current_song = LOOP_MODES["none"]
         self.duration = 0
         self.paused = False
         self.ending = False
         self.prompting: None | tuple = None
         self.clip = (0, 0)
@@ -409,14 +412,22 @@
                     length_so_far,
                     curses.color_pair(14),
                 )
 
         visualize_message = ""
         visualize_color = 12
         if self.visualize:
+            if self.visualizer_data is None and self.can_visualize:
+                t = threading.Thread(
+                    target=self.load_visualizer_data,
+                    daemon=True,
+                )
+                self.visualizer_data = {}
+                t.start()
+
             if not self.can_visualize:
                 visualize_message = "Librosa is required for visualization."
                 visualize_color = 14
             elif not self.can_show_visualization:
                 visualize_message = "Window too small for visualization."
                 visualize_color = 14
             elif self.playlist[self.i][0] not in self.visualizer_data:
```

### Comparing `maestro-music-1.0.3/icon.py` & `maestro-music-1.0.4/icon.py`

 * *Files identical despite different names*

### Comparing `maestro-music-1.0.3/mac_presence.py` & `maestro-music-1.0.4/mac_presence.py`

 * *Files identical despite different names*

### Comparing `maestro-music-1.0.3/maestro.py` & `maestro-music-1.0.4/maestro.py`

 * *Files identical despite different names*

### Comparing `maestro-music-1.0.3/maestro_music.egg-info/PKG-INFO` & `maestro-music-1.0.4/maestro_music.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestro-music
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple command line tool to play songs (or any audio files, really).
 Home-page: https://github.com/PrajwalVandana/maestro-cli
 Author: Prajwal Vandana
 License: MIT
 Keywords: music,sound,audio,music-player,cli,ogg,flac,mp3,wav,spotify,youtube,audio-visualization,audio-visualizer
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -147,14 +147,16 @@
 
 List details for a specific song.
 
 ### `maestro list`
 
 List songs (or tags) and details. Use `maestro list -h` to see full options (e.g. sort, list only songs with a certain tag, etc.).
 
+![maestro list example](data/list.png)
+
 ### `maestro play`
 
 Play songs. Use `maestro play -h` to see full options. Has lots of features:
 - pass tag(s) as arguments to play songs with any of those tag(s) (or songs with all of those tag(s) if you pass the `-M` or `--match-all` flag)
 - shuffle playlist with the `-s` or `--shuffle option (shuffle once, shuffle everytime the playlist repeats, or shuffle everytime the playlist repeats except the first)
 - play songs in reverse order with the `-R` or `--reverse` flag
 - loop playlist with the `-L` or `--loop` flag
@@ -177,14 +179,16 @@
 - `i` to insert a song by ID after the currently playing song
 - `b` or `p` to go back to the previous song
 - `s` or `n` to go to the next song
 - space to pause/play
 - `e` to end after the current song
 - `q` to end immediately (don't just close the window or `CTRL-c`, this messes up the accuracy of the listen time statistics)
 
+![maestro play example](data/player.png)
+
 ### `maestro push`
 
 Push a song to the top (or bottom) of your song list. Useful, for example, if you usually play the most recently added songs first (`maestro play -R`)—you can use `maestro push` to push a song to the top of your list so it's the first song to play.
 
 ### `maestro recommend` (experimental)
 
 Recommend songs similar to a song title (specified directly or by ID) using YouTube Music. Equivalent to searching for the title of the song on YouTube Music, clicking on the first "Song" result, and then looking at the "Up Next" section.
```

### Comparing `maestro-music-1.0.3/setup.py` & `maestro-music-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "pyobjc-framework-CoreMedia; sys_platform == 'darwin'",
     "pyobjc-framework-MediaPlayer; sys_platform == 'darwin'",
     "pyobjc-framework-Quartz; sys_platform == 'darwin'",
 ]
 
 setup(
     name="maestro-music",
-    version="1.0.3",
+    version="1.0.4",
     author="Prajwal Vandana",
     url="https://github.com/PrajwalVandana/maestro-cli",
     description="A simple command line tool to play songs (or any audio files, really).",
     long_description=open("readme.md", encoding="utf-8").read(),
     license="MIT",
     license_files=["LICENSE"],
     long_description_content_type="text/markdown",
```

