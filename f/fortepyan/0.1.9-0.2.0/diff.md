# Comparing `tmp/fortepyan-0.1.9.tar.gz` & `tmp/fortepyan-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortepyan-0.1.9.tar", last modified: Sun Apr  2 17:21:18 2023, max compression
+gzip compressed data, was "fortepyan-0.2.0.tar", last modified: Sun Jun 11 11:47:03 2023, max compression
```

## Comparing `fortepyan-0.1.9.tar` & `fortepyan-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,38 @@
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-04-02 17:21:18.612348 fortepyan-0.1.9/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1226 2023-04-02 17:21:18.612348 fortepyan-0.1.9/PKG-INFO
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      774 2023-02-26 14:45:22.000000 fortepyan-0.1.9/README.md
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-04-02 17:21:18.612348 fortepyan-0.1.9/fortepyan/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      468 2023-04-02 17:20:56.000000 fortepyan-0.1.9/fortepyan/__init__.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-04-02 17:21:18.612348 fortepyan-0.1.9/fortepyan/animation/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       96 2023-03-02 08:36:53.000000 fortepyan-0.1.9/fortepyan/animation/__init__.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)    15612 2023-03-08 21:12:29.000000 fortepyan-0.1.9/fortepyan/animation/evolution.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      756 2023-02-21 08:54:31.000000 fortepyan-0.1.9/fortepyan/animation/main.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     4985 2023-03-08 20:21:52.000000 fortepyan-0.1.9/fortepyan/animation/pianoroll.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-04-02 17:21:18.612348 fortepyan-0.1.9/fortepyan/audio/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1145 2023-02-11 18:30:36.000000 fortepyan-0.1.9/fortepyan/audio/render.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      514 2023-02-28 06:46:10.000000 fortepyan-0.1.9/fortepyan/audio/soundfont.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      249 2023-02-26 12:33:07.000000 fortepyan-0.1.9/fortepyan/config.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1962 2023-01-29 11:21:01.000000 fortepyan-0.1.9/fortepyan/main.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-04-02 17:21:18.612348 fortepyan-0.1.9/fortepyan/midi/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     8106 2023-04-02 17:19:30.000000 fortepyan-0.1.9/fortepyan/midi/structures.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2168 2023-03-04 16:57:37.000000 fortepyan-0.1.9/fortepyan/midi/tools.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-04-02 17:21:18.612348 fortepyan-0.1.9/fortepyan/viz/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-02-11 18:29:02.000000 fortepyan-0.1.9/fortepyan/viz/__init__.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5531 2023-03-08 21:09:31.000000 fortepyan-0.1.9/fortepyan/viz/pianoroll.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2925 2023-03-03 08:39:56.000000 fortepyan-0.1.9/fortepyan/viz/structures.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-04-02 17:21:18.612348 fortepyan-0.1.9/fortepyan.egg-info/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1226 2023-04-02 17:21:18.000000 fortepyan-0.1.9/fortepyan.egg-info/PKG-INFO
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      563 2023-04-02 17:21:18.000000 fortepyan-0.1.9/fortepyan.egg-info/SOURCES.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        1 2023-04-02 17:21:18.000000 fortepyan-0.1.9/fortepyan.egg-info/dependency_links.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      137 2023-04-02 17:21:18.000000 fortepyan-0.1.9/fortepyan.egg-info/requires.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       10 2023-04-02 17:21:18.000000 fortepyan-0.1.9/fortepyan.egg-info/top_level.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1326 2023-04-02 17:20:56.000000 fortepyan-0.1.9/pyproject.toml
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       38 2023-04-02 17:21:18.612348 fortepyan-0.1.9/setup.cfg
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.037683 fortepyan-0.2.0/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-06-11 11:47:03.037683 fortepyan-0.2.0/PKG-INFO
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      964 2023-06-11 10:38:07.000000 fortepyan-0.2.0/README.md
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.033683 fortepyan-0.2.0/fortepyan/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      361 2023-06-11 11:46:44.000000 fortepyan-0.2.0/fortepyan/__init__.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.033683 fortepyan-0.2.0/fortepyan/analytics/
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.033683 fortepyan-0.2.0/fortepyan/analytics/clustering/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:22:34.000000 fortepyan-0.2.0/fortepyan/analytics/clustering/__init__.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     7846 2023-06-11 11:36:25.000000 fortepyan-0.2.0/fortepyan/analytics/clustering/process.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1519 2023-06-11 11:36:25.000000 fortepyan-0.2.0/fortepyan/analytics/clustering/structures.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      768 2023-06-11 11:36:24.000000 fortepyan-0.2.0/fortepyan/analytics/clustering/views.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.037683 fortepyan-0.2.0/fortepyan/audio/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1145 2023-02-11 18:30:36.000000 fortepyan-0.2.0/fortepyan/audio/render.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      514 2023-02-28 06:46:10.000000 fortepyan-0.2.0/fortepyan/audio/soundfont.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      249 2023-02-26 12:33:07.000000 fortepyan-0.2.0/fortepyan/config.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1962 2023-01-29 11:21:01.000000 fortepyan-0.2.0/fortepyan/main.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.037683 fortepyan-0.2.0/fortepyan/midi/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     8284 2023-06-11 10:56:41.000000 fortepyan-0.2.0/fortepyan/midi/structures.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2189 2023-04-23 12:50:22.000000 fortepyan-0.2.0/fortepyan/midi/tools.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.037683 fortepyan-0.2.0/fortepyan/view/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      208 2023-06-11 08:17:56.000000 fortepyan-0.2.0/fortepyan/view/__init__.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.037683 fortepyan-0.2.0/fortepyan/view/animation/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 08:05:25.000000 fortepyan-0.2.0/fortepyan/view/animation/__init__.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)    15618 2023-06-11 08:41:59.000000 fortepyan-0.2.0/fortepyan/view/animation/evolution.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      761 2023-06-11 08:41:24.000000 fortepyan-0.2.0/fortepyan/view/animation/main.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5002 2023-06-11 08:41:45.000000 fortepyan-0.2.0/fortepyan/view/animation/pianoroll.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.037683 fortepyan-0.2.0/fortepyan/view/pianoroll/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       65 2023-06-11 11:36:25.000000 fortepyan-0.2.0/fortepyan/view/pianoroll/__init__.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5426 2023-06-11 08:19:09.000000 fortepyan-0.2.0/fortepyan/view/pianoroll/main.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2925 2023-06-11 08:18:40.000000 fortepyan-0.2.0/fortepyan/view/pianoroll/structures.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:47:03.033683 fortepyan-0.2.0/fortepyan.egg-info/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-06-11 11:47:03.000000 fortepyan-0.2.0/fortepyan.egg-info/PKG-INFO
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      808 2023-06-11 11:47:03.000000 fortepyan-0.2.0/fortepyan.egg-info/SOURCES.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        1 2023-06-11 11:47:03.000000 fortepyan-0.2.0/fortepyan.egg-info/dependency_links.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      157 2023-06-11 11:47:03.000000 fortepyan-0.2.0/fortepyan.egg-info/requires.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       10 2023-06-11 11:47:03.000000 fortepyan-0.2.0/fortepyan.egg-info/top_level.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1452 2023-06-11 11:46:44.000000 fortepyan-0.2.0/pyproject.toml
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       38 2023-06-11 11:47:03.037683 fortepyan-0.2.0/setup.cfg
```

### Comparing `fortepyan-0.1.9/PKG-INFO` & `fortepyan-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 Metadata-Version: 2.1
 Name: fortepyan
-Version: 0.1.9
+Version: 0.2.0
 Summary: Process MIDI piano with (almost) no pain
 Author-email: Piano For AI <roszcz+fortepyan@gmail.com>
 Project-URL: Homepage, https://github.com/Nospoko/fortepyan
 Keywords: midi,music,piano
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # fortepyan :musical_keyboard:
 
+### Usage
+
+```python
+import fortepyan as ff
+
+piece = ff.MidiPiece.from_file("mymidi.mid")
+
+ff.view.draw_pianoroll_with_velocities(piece)
+ff.view.make_piano_roll_video(piece, "tmp.mp4")
+```
+
 ### Development
 
 Pre-commit hooks with forced python formatting ([black](https://github.com/psf/black), [flake8](https://flake8.pycqa.org/en/latest/), and [isort](https://pycqa.github.io/isort/)):
 
 ```sh
 pip install pre-commit
 pre-commit install
```

### Comparing `fortepyan-0.1.9/README.md` & `fortepyan-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # fortepyan :musical_keyboard:
 
+### Usage
+
+```python
+import fortepyan as ff
+
+piece = ff.MidiPiece.from_file("mymidi.mid")
+
+ff.view.draw_pianoroll_with_velocities(piece)
+ff.view.make_piano_roll_video(piece, "tmp.mp4")
+```
+
 ### Development
 
 Pre-commit hooks with forced python formatting ([black](https://github.com/psf/black), [flake8](https://flake8.pycqa.org/en/latest/), and [isort](https://pycqa.github.io/isort/)):
 
 ```sh
 pip install pre-commit
 pre-commit install
```

### Comparing `fortepyan-0.1.9/fortepyan/animation/evolution.py` & `fortepyan-0.2.0/fortepyan/view/animation/evolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from pathlib import Path
 import multiprocessing as mp
 
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 
-from fortepyan.viz import pianoroll as roll
 from fortepyan.viz.structures import PianoRoll
 from fortepyan.midi.structures import MidiPiece
+from fortepyan.view.pianoroll import main as roll
 
 
 class MutePianoRollEvolution:
     def __init__(
         self,
         pieces: list[MidiPiece],
         title_format: str = "{}",
```

### Comparing `fortepyan-0.1.9/fortepyan/animation/main.py` & `fortepyan-0.2.0/fortepyan/view/animation/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import subprocess
 
 from fortepyan.audio.render import midi_to_mp3
 from fortepyan.midi.structures import MidiPiece
-from fortepyan.animation import pianoroll as pianoroll_animation
+from fortepyan.view.animation import pianoroll as pianoroll_animation
 
 
 def make_piano_roll_video(
     piece: MidiPiece,
     movie_path: str,
     title: str = "animation",
     cmap: str = "PuBuGn",
```

### Comparing `fortepyan-0.1.9/fortepyan/animation/pianoroll.py` & `fortepyan-0.2.0/fortepyan/view/animation/pianoroll.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from pathlib import Path
 import multiprocessing as mp
 
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 
-from fortepyan.viz import pianoroll as roll
-from fortepyan.viz.structures import PianoRoll
 from fortepyan.midi.structures import MidiPiece
+from fortepyan.view.pianoroll import main as roll
+from fortepyan.view.pianoroll.structures import PianoRoll
 
 
 class PianoRollScene:
     def __init__(self, piece: MidiPiece, title: str, cmap: str = "GnBu"):
         self.axes = []
         self.content_dir = Path(tempfile.mkdtemp())
```

### Comparing `fortepyan-0.1.9/fortepyan/audio/render.py` & `fortepyan-0.2.0/fortepyan/audio/render.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.1.9/fortepyan/audio/soundfont.py` & `fortepyan-0.2.0/fortepyan/audio/soundfont.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.1.9/fortepyan/main.py` & `fortepyan-0.2.0/fortepyan/main.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.1.9/fortepyan/midi/structures.py` & `fortepyan-0.2.0/fortepyan/midi/structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,18 @@
         - start (float): start time in seconds
         - finish (float): end time in seconds
 
         Returns:
         - MidiPiece: the trimmed MidiPiece object
         """
         # Filter the rows in the data frame that are within the specified start and end time
-        ids = (self.df.start >= start) & (self.df.end <= finish)
+        ids = (self.df.start >= start) & (self.df.start <= finish)
         # Get the indices of the rows that meet the criteria
         idxs = np.where(ids)[0]
+
         # Get the start and end indices for the new MidiPiece object
         start = idxs[0]
         finish = idxs[-1] + 1
         # Slice the original MidiPiece object to create the trimmed MidiPiece object
         out = self[start:finish]
         # Return the trimmed MidiPiece object
         return out
@@ -124,22 +125,30 @@
 
         return track
 
     @classmethod
     def from_huggingface(cls, record: dict) -> "MidiPiece":
         df = pd.DataFrame(record["notes"])
         df["duration"] = df.end - df.start
+
         source = {
-            "composer": record["composer"],
-            "title": record["title"],
-            "midi_filename": record["midi_filename"],
+            "composer": record.get("composer"),
+            "title": record.get("title"),
+            "midi_filename": record.get("midi_filename"),
+            "record_id": record.get("record_id"),
+            "user": record.get("user"),
         }
         that = cls(df=df, source=source)
         return that
 
+    @classmethod
+    def from_file(cls, path: str) -> "MidiPiece":
+        piece = MidiFile(str(path)).piece
+        return piece
+
 
 @dataclass
 class MidiFile:
     path: str
     apply_sustain: bool = True
     sustain_threshold: int = 62
     df: pd.DataFrame = field(init=False)
@@ -205,16 +214,14 @@
                 df=self.raw_df,
                 sustain=self.sustain,
                 sustain_threshold=self.sustain_threshold,
             )
         else:
             self.df = self.raw_df
 
-        self.df["duration"] = self.df.end - self.df.start
-
     def __getitem__(self, index: slice) -> MidiPiece:
         return self.piece[index]
         if not isinstance(index, slice):
             raise TypeError("You can only get a part of MidiFile that has multiple notes: Index must be a slice")
 
         part = self.df[index].reset_index(drop=True)
         first_sound = part.start.min()
```

### Comparing `fortepyan-0.1.9/fortepyan/midi/tools.py` & `fortepyan-0.2.0/fortepyan/midi/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 
         # Modify end times of selected notes based on sustain pedal duration
         df = sustain_notes(
             df=df,
             pedal_down=pedal_down,
             pedal_up=pedal_up,
         )
-        # df.loc[ids, "end"] = modified_end_times
+
+    # Keep duration consistent
+    df["duration"] = df.end - df.start
 
     return df
 
 
 def sustain_notes(
     df: pd.DataFrame,
     pedal_down: float,
```

### Comparing `fortepyan-0.1.9/fortepyan/viz/pianoroll.py` & `fortepyan-0.2.0/fortepyan/view/pianoroll/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import matplotlib
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 
-from fortepyan.viz.structures import PianoRoll
 from fortepyan.midi.structures import MidiPiece
+from fortepyan.view.pianoroll.structures import PianoRoll
 
 
 def draw_pianoroll_with_velocities(
     midi_piece: MidiPiece,
     time_end: float = None,
     title: str = None,
     cmap: str = "GnBu",
@@ -87,17 +87,14 @@
         time (Optional[float]): Use for dynamic visualization - will highlight notes
             played at this *time* value
         cmap (str): colormap recognizable by Matplotlib
 
     Returns:
         ax: Matplotlib axis with pianoroll.
     """
-    # piece = sanitize_midi_piece(midi_piece)
-    # piano_roll = prepare_piano_roll(piece.df, time_indicator=time)
-
     ax.imshow(
         piano_roll.roll,
         aspect="auto",
         vmin=0,
         vmax=138,
         origin="lower",
         interpolation="none",
```

### Comparing `fortepyan-0.1.9/fortepyan/viz/structures.py` & `fortepyan-0.2.0/fortepyan/view/pianoroll/structures.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.1.9/fortepyan.egg-info/PKG-INFO` & `fortepyan-0.2.0/fortepyan.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 Metadata-Version: 2.1
 Name: fortepyan
-Version: 0.1.9
+Version: 0.2.0
 Summary: Process MIDI piano with (almost) no pain
 Author-email: Piano For AI <roszcz+fortepyan@gmail.com>
 Project-URL: Homepage, https://github.com/Nospoko/fortepyan
 Keywords: midi,music,piano
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # fortepyan :musical_keyboard:
 
+### Usage
+
+```python
+import fortepyan as ff
+
+piece = ff.MidiPiece.from_file("mymidi.mid")
+
+ff.view.draw_pianoroll_with_velocities(piece)
+ff.view.make_piano_roll_video(piece, "tmp.mp4")
+```
+
 ### Development
 
 Pre-commit hooks with forced python formatting ([black](https://github.com/psf/black), [flake8](https://flake8.pycqa.org/en/latest/), and [isort](https://pycqa.github.io/isort/)):
 
 ```sh
 pip install pre-commit
 pre-commit install
```

### Comparing `fortepyan-0.1.9/pyproject.toml` & `fortepyan-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fortepyan"
-version = "0.1.9"
+version = "0.2.0"
 description = "Process MIDI piano with (almost) no pain"
 readme = "README.md"
 authors = [{ name = "Piano For AI", email = "roszcz+fortepyan@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -23,25 +23,34 @@
     "midi2audio>=0.1.1",
     "numpy>=1.23.4",
     "pretty-midi>=0.2.9",
     "psycopg2>=2.9.5",
     "pydub>=0.25",
     "SQLAlchemy>=1.4.45",
     "matplotlib>=3.6.2",
+    "Levenshtein>=0.20.9",
 ]
 requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://github.com/Nospoko/fortepyan"
 
 [tool.setuptools]
-packages = ["fortepyan", "fortepyan.viz", "fortepyan.midi", "fortepyan.audio", "fortepyan.animation"]
+packages = [
+    "fortepyan",
+    "fortepyan.view",
+    "fortepyan.midi",
+    "fortepyan.audio",
+    "fortepyan.view.animation",
+    "fortepyan.view.pianoroll",
+    "fortepyan.analytics.clustering",
+]
 
 [tool.bumpver]
-current_version = "0.1.9"
+current_version = "0.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

