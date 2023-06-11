# Comparing `tmp/pytubemusic-0.1.2.tar.gz` & `tmp/pytubemusic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytubemusic-0.1.2.tar", last modified: Thu May 25 09:06:57 2023, max compression
+gzip compressed data, was "pytubemusic-0.2.0.tar", last modified: Sun Jun 11 09:33:57 2023, max compression
```

## Comparing `pytubemusic-0.1.2.tar` & `pytubemusic-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-25 09:06:57.128493 pytubemusic-0.1.2/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1075 2023-01-01 00:59:16.000000 pytubemusic-0.1.2/LICENSE
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     5274 2023-05-25 09:06:57.128340 pytubemusic-0.1.2/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3567 2023-05-25 09:05:25.000000 pytubemusic-0.1.2/README.md
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      858 2023-05-25 09:06:40.000000 pytubemusic-0.1.2/pyproject.toml
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      132 2023-05-25 08:59:56.000000 pytubemusic-0.1.2/requirements.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-05-25 09:06:57.128535 pytubemusic-0.1.2/setup.cfg
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-25 09:06:57.123354 pytubemusic-0.1.2/src/
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-25 09:06:57.125565 pytubemusic-0.1.2/src/pytubemusic/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-01-01 00:52:45.000000 pytubemusic-0.1.2/src/pytubemusic/__init__.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3428 2023-04-17 20:41:20.000000 pytubemusic-0.1.2/src/pytubemusic/__main__.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2005 2023-04-17 20:36:11.000000 pytubemusic-0.1.2/src/pytubemusic/audio.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3185 2023-04-16 01:35:20.000000 pytubemusic-0.1.2/src/pytubemusic/logutils.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     5710 2023-05-09 07:34:40.000000 pytubemusic-0.1.2/src/pytubemusic/track.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3625 2023-04-16 01:34:45.000000 pytubemusic-0.1.2/src/pytubemusic/utils.py
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-25 09:06:57.126680 pytubemusic-0.1.2/src/pytubemusic/validation/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1143 2023-04-16 03:47:20.000000 pytubemusic-0.1.2/src/pytubemusic/validation/__init__.py
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-25 09:06:57.127756 pytubemusic-0.1.2/src/pytubemusic/validation/schemata/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1879 2023-04-16 01:15:44.000000 pytubemusic-0.1.2/src/pytubemusic/validation/schemata/album.schema.json
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1830 2023-04-16 01:20:40.000000 pytubemusic-0.1.2/src/pytubemusic/validation/schemata/playlist.schema.json
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1189 2023-04-16 01:15:44.000000 pytubemusic-0.1.2/src/pytubemusic/validation/schemata/track.schema.json
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-25 09:06:57.126567 pytubemusic-0.1.2/src/pytubemusic.egg-info/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     5274 2023-05-25 09:06:57.000000 pytubemusic-0.1.2/src/pytubemusic.egg-info/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      668 2023-05-25 09:06:57.000000 pytubemusic-0.1.2/src/pytubemusic.egg-info/SOURCES.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-05-25 09:06:57.000000 pytubemusic-0.1.2/src/pytubemusic.egg-info/dependency_links.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       53 2023-05-25 09:06:57.000000 pytubemusic-0.1.2/src/pytubemusic.egg-info/entry_points.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      132 2023-05-25 09:06:57.000000 pytubemusic-0.1.2/src/pytubemusic.egg-info/requires.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       12 2023-05-25 09:06:57.000000 pytubemusic-0.1.2/src/pytubemusic.egg-info/top_level.txt
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-25 09:06:57.127964 pytubemusic-0.1.2/tests/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1641 2023-02-14 00:54:23.000000 pytubemusic-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-11 09:33:57.387145 pytubemusic-0.2.0/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1075 2023-01-01 00:59:16.000000 pytubemusic-0.2.0/LICENSE
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     5958 2023-06-11 09:33:57.387015 pytubemusic-0.2.0/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     4251 2023-06-11 06:38:30.000000 pytubemusic-0.2.0/README.md
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      858 2023-06-11 09:33:23.000000 pytubemusic-0.2.0/pyproject.toml
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      132 2023-05-25 08:59:56.000000 pytubemusic-0.2.0/requirements.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-06-11 09:33:57.387187 pytubemusic-0.2.0/setup.cfg
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-11 09:33:57.382594 pytubemusic-0.2.0/src/
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-11 09:33:57.384063 pytubemusic-0.2.0/src/pytubemusic/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-01-01 00:52:45.000000 pytubemusic-0.2.0/src/pytubemusic/__init__.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     4344 2023-06-11 08:56:55.000000 pytubemusic-0.2.0/src/pytubemusic/__main__.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2385 2023-06-11 07:30:56.000000 pytubemusic-0.2.0/src/pytubemusic/audio.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3700 2023-06-11 05:49:47.000000 pytubemusic-0.2.0/src/pytubemusic/logutils.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     6752 2023-06-11 07:30:56.000000 pytubemusic-0.2.0/src/pytubemusic/track.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2821 2023-06-11 07:21:31.000000 pytubemusic-0.2.0/src/pytubemusic/utils.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-11 09:33:57.385113 pytubemusic-0.2.0/src/pytubemusic/validation/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1143 2023-04-16 03:47:20.000000 pytubemusic-0.2.0/src/pytubemusic/validation/__init__.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-11 09:33:57.386448 pytubemusic-0.2.0/src/pytubemusic/validation/schemata/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1879 2023-04-16 01:15:44.000000 pytubemusic-0.2.0/src/pytubemusic/validation/schemata/album.schema.json
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1542 2023-06-11 05:29:02.000000 pytubemusic-0.2.0/src/pytubemusic/validation/schemata/multitrack.schema.json
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1830 2023-04-16 01:20:40.000000 pytubemusic-0.2.0/src/pytubemusic/validation/schemata/playlist.schema.json
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1189 2023-04-16 01:15:44.000000 pytubemusic-0.2.0/src/pytubemusic/validation/schemata/track.schema.json
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-11 09:33:57.384985 pytubemusic-0.2.0/src/pytubemusic.egg-info/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     5958 2023-06-11 09:33:57.000000 pytubemusic-0.2.0/src/pytubemusic.egg-info/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      727 2023-06-11 09:33:57.000000 pytubemusic-0.2.0/src/pytubemusic.egg-info/SOURCES.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-06-11 09:33:57.000000 pytubemusic-0.2.0/src/pytubemusic.egg-info/dependency_links.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       53 2023-06-11 09:33:57.000000 pytubemusic-0.2.0/src/pytubemusic.egg-info/entry_points.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      132 2023-06-11 09:33:57.000000 pytubemusic-0.2.0/src/pytubemusic.egg-info/requires.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       12 2023-06-11 09:33:57.000000 pytubemusic-0.2.0/src/pytubemusic.egg-info/top_level.txt
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-11 09:33:57.386695 pytubemusic-0.2.0/tests/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1641 2023-02-14 00:54:23.000000 pytubemusic-0.2.0/tests/test_utils.py
```

### Comparing `pytubemusic-0.1.2/LICENSE` & `pytubemusic-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.1.2/PKG-INFO` & `pytubemusic-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubemusic
-Version: 0.1.2
+Version: 0.2.0
 Summary: A cli that may or may not download albums from a certain website
 License: MIT License
         
         Copyright (c) 2023 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -40,34 +40,38 @@
 
 ```
 pip install pytubemusic
 ```
 
 **Requires [ffmpeg](https://ffmpeg.org/) to be installed on your machine.**
 
-### Installation Note
+<details>
+<summary>Installation Note</summary>
 
 PyTubeMusic uses the [PyTube](https://github.com/pytube/pytube) library. This
 can occasionally break. However, patches are usually quickly released as new
 versions or as pull requests. Try upgrading to the latest version of PyTube if
 downloading fails.
 
 > Note, to pip install from a pull request do:
 > ```text
 >  pip install git+https://github.com/pytube/pytube.git@refs/pull/<PR_NUM>/head
 > ```
 > Where `<PR_NUM>` is the number of the pull request.
 
+</details>
+
 ## Usage
 
 PyTubeMusic can download tracks in three formats:
 
 - Tracks (Single files)
 - Albums (A single video that is split up into individual tracks on an album)
 - Playlists (Videos in a playlist that are downloaded as tracks on an album)
+- Multi Tracks (Several videos that get combined into a single track)
 
 Each type of track needs a different configuration file that includes metadata.
 These are described below.
 
 Note: the term "timestamp" refers to a string of the form: "H?:M:S.f?" – for
 example: "23:55.75", "1:12:00", "5:03", "17:00.5"
 
@@ -137,19 +141,41 @@
 track_data = []
 
 [metadata]
 album = "..."  # Album name (required)
 # Any other FFMPEG MP3 metadata tags
 ```
 
+### Multi Tracks
+
+> Several videos combined into a single track
+
+Effectively a list of URLs with metadata and an optional cover image. Note
+that `track_data` here has a different format to other cli commands:
+
+```toml
+cover_url = "..."  # Track cover jpg URL (optional – uses thumbnail of first video by default)
+
+# Required track data
+track_data = [
+    # Url to video and optional start and end timestamps
+    { url = "...", start = "...", end = "..." },
+    # ...
+]
+
+[metadata]
+title = "..."  # Track name (required)
+# Any other FFMPEG MP3 metadata tags
+```
+
 ### CLI
 
 A `pytubemusic` command will be exposed.
 
-This has three commands: `album`, `track`, `playlist`.
+This has four commands: `album`, `track`, `playlist`, `multitrack`.
 Each command corresponds to one of the file types mentioned above.
 
 The commands all take the path to a config TOML file and an optional `-o`
 or `--out` option pointing to a directory to write the resulting tracks too.
 (Note: albums and playlists are put into their own subdirectory with the album
 name under the out directory).
```

### Comparing `pytubemusic-0.1.2/README.md` & `pytubemusic-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,34 +6,38 @@
 
 ```
 pip install pytubemusic
 ```
 
 **Requires [ffmpeg](https://ffmpeg.org/) to be installed on your machine.**
 
-### Installation Note
+<details>
+<summary>Installation Note</summary>
 
 PyTubeMusic uses the [PyTube](https://github.com/pytube/pytube) library. This
 can occasionally break. However, patches are usually quickly released as new
 versions or as pull requests. Try upgrading to the latest version of PyTube if
 downloading fails.
 
 > Note, to pip install from a pull request do:
 > ```text
 >  pip install git+https://github.com/pytube/pytube.git@refs/pull/<PR_NUM>/head
 > ```
 > Where `<PR_NUM>` is the number of the pull request.
 
+</details>
+
 ## Usage
 
 PyTubeMusic can download tracks in three formats:
 
 - Tracks (Single files)
 - Albums (A single video that is split up into individual tracks on an album)
 - Playlists (Videos in a playlist that are downloaded as tracks on an album)
+- Multi Tracks (Several videos that get combined into a single track)
 
 Each type of track needs a different configuration file that includes metadata.
 These are described below.
 
 Note: the term "timestamp" refers to a string of the form: "H?:M:S.f?" – for
 example: "23:55.75", "1:12:00", "5:03", "17:00.5"
 
@@ -103,19 +107,41 @@
 track_data = []
 
 [metadata]
 album = "..."  # Album name (required)
 # Any other FFMPEG MP3 metadata tags
 ```
 
+### Multi Tracks
+
+> Several videos combined into a single track
+
+Effectively a list of URLs with metadata and an optional cover image. Note
+that `track_data` here has a different format to other cli commands:
+
+```toml
+cover_url = "..."  # Track cover jpg URL (optional – uses thumbnail of first video by default)
+
+# Required track data
+track_data = [
+    # Url to video and optional start and end timestamps
+    { url = "...", start = "...", end = "..." },
+    # ...
+]
+
+[metadata]
+title = "..."  # Track name (required)
+# Any other FFMPEG MP3 metadata tags
+```
+
 ### CLI
 
 A `pytubemusic` command will be exposed.
 
-This has three commands: `album`, `track`, `playlist`.
+This has four commands: `album`, `track`, `playlist`, `multitrack`.
 Each command corresponds to one of the file types mentioned above.
 
 The commands all take the path to a config TOML file and an optional `-o`
 or `--out` option pointing to a directory to write the resulting tracks too.
 (Note: albums and playlists are put into their own subdirectory with the album
 name under the out directory).
```

### Comparing `pytubemusic-0.1.2/pyproject.toml` & `pytubemusic-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytubemusic"
-version = "0.1.2"
+version = "0.2.0"
 description = 'A cli that may or may not download albums from a certain website'
 
 readme = "README.md"
 requires-python = ">=3.11"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `pytubemusic-0.1.2/src/pytubemusic/__main__.py` & `pytubemusic-0.2.0/src/pytubemusic/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -97,13 +97,40 @@
         playlist_data = loadf_or_panic(f, "playlist", err_msg)
     tracks = list(Track.from_playlist(**playlist_data))
     with log_block(on_enter="Exporting tracks"):
         for track in tracks:
             track.export(out / track.album)
 
 
+@app.command(
+    "multitrack",
+    help="Combines several tracks into one",
+)
+@log_call(
+    on_enter="Building track from '{multi_track_data}'",
+    on_exit="\x1b[32mDONE!\x1b[0m",
+    on_error="\x1b[31mProcessing track Failed.\x1b[0m",
+)
+def make_multi_track(
+        multi_track_data: Path = Argument(..., help="The track data"),
+        out: Path = Option(
+            Path("."),
+            "--out", "-o",
+            help="The directory album tracks will be written to. "
+                 "Defaults to the cwd",
+        )
+):
+    prefix = "Processing Multi Track Failed.\n"
+    err_msg = f"{prefix}Cannot open `{multi_track_data}`"
+    with open_or_panic(multi_track_data, "rb", err_msg) as f:
+        err_msg = f"{prefix}Invalid Track TOML format for `{multi_track_data}`."
+        track_data = loadf_or_panic(f, "multitrack", err_msg)
+    track = Track.from_multi_track(**track_data)
+    track.export(out)
+
+
 @app.callback(invoke_without_command=True)
 def main():
     cowexcept.activate()
 
 
 app()
```

### Comparing `pytubemusic-0.1.2/src/pytubemusic/audio.py` & `pytubemusic-0.2.0/src/pytubemusic/audio.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import io
-from collections.abc import Mapping
+from collections.abc import Iterable, Mapping
 from datetime import timedelta
 from typing import BinaryIO, Self
 
 import backoff
 from pydub import AudioSegment
 from pytube import YouTube
+from pytube.exceptions import PytubeError
 
 from pytubemusic.utils import to_microseconds
 
 __all__ = ["Audio"]
 
 
 class Audio:
@@ -43,21 +44,31 @@
             format="mp3",
             tags=metadata,
             parameters=["-b:a", f"{self.bitrate}"],
             cover=cover,
         )
 
     @classmethod
-    @backoff.on_exception(backoff.expo, KeyError, max_tries=5)
+    @backoff.on_exception(backoff.expo, (PytubeError, KeyError), max_tries=5)
     def from_url(cls, url: str) -> Self:
         """
         Downloads audio from the video associated with the URL
 
         :param url: The video URL
         :return: An Audio object
         """
         buffer = io.BytesIO()
         raw_audio = YouTube(url).streams.get_audio_only()
         raw_audio.stream_to_buffer(buffer)
         buffer.seek(0)
         audio_data = AudioSegment.from_file(buffer)
         return cls(audio_data, raw_audio.bitrate)
+
+    @classmethod
+    def join(cls, tracks: Iterable["Audio"]) -> Self:
+        tracks = iter(tracks)
+        first = next(tracks)
+        bitrate = first.bitrate
+        audio = first._audio_data
+        for track in tracks:
+            audio = audio.append(track._audio_data)
+        return cls(audio, bitrate)
```

### Comparing `pytubemusic-0.1.2/src/pytubemusic/logutils.py` & `pytubemusic-0.2.0/src/pytubemusic/logutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,7 +113,27 @@
         logger.log(level, msg)
 
 
 @contextlib.contextmanager
 def open_or_panic(file_name, mode, msg):
     with (PanicOn(OSError, msg), open(file_name, mode) as f):
         yield f
+
+
+def log_iter(
+        level=logging.INFO,
+        on_each: str = None,
+        on_enter: str = None,
+        on_exit: str = None,
+        start: int = 0,
+):
+    def iterator(data: Iterable):
+        global _INDENT
+        _INDENT += INDENT_WIDTH
+        log_message(on_enter, [], {}, level)
+        for i, e in enumerate(data, start=start):
+            log_message(on_each, [e], {"i": i}, level)
+            yield e
+        log_message(on_exit, [], {}, level)
+        _INDENT -= INDENT_WIDTH
+
+    return iterator
```

### Comparing `pytubemusic-0.1.2/src/pytubemusic/track.py` & `pytubemusic-0.2.0/src/pytubemusic/track.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 from tempfile import NamedTemporaryFile
 from typing import Any, Self
 
 from pipe_utils import Pipe
 from pytube import Playlist
 
 from pytubemusic.audio import Audio
-from pytubemusic.logutils import log_call
+from pytubemusic.logutils import log_call, log_iter
 from pytubemusic.utils import *
 
 __all__ = ["Track"]
 
 STR_MAP = Mapping[str, Any]
 TRACK_DATA = Iterable[STR_MAP]
 
 
-@dataclass
+@dataclass(frozen=True)
 class Track:
     raw_audio: Audio
     cover: NamedTemporaryFile
-    start: timedelta
-    end: timedelta
     metadata: STR_MAP
+    start: timedelta = None
+    end: timedelta = None
 
     @property
     def audio(self) -> Audio:
         """The raw audio snipped to the track start and end times"""
         return self.raw_audio.snip(self.start, self.end)
 
     @property
@@ -90,18 +90,18 @@
                 Pipe(track_data)
                 | (set_ends, audio.duration)
                 | (merge_metadata, metadata)
         ).get()
         for track in track_data:
             yield cls(
                 audio,
-                thumbnail(url) if cover_url is None else get_cover(cover_url),
+                get_cover(url, cover_url),
+                track["metadata"],
                 to_delta(track["start"]),
                 to_delta(track["end"]),
-                track["metadata"],
             )
 
     @classmethod
     @log_call(on_enter="Downloading '{metadata[title]}' from {url}")
     def from_video(
             cls,
             url: str,
@@ -122,18 +122,18 @@
             Defaults to the length of the audio
         :param cover_url: The url to a JPG cover image
         :return: A new Track
         """
         audio = Audio.from_url(url)
         return cls(
             audio,
-            thumbnail(url) if cover_url is None else get_cover(cover_url),
+            get_cover(url, cover_url),
+            metadata,
             to_delta(start),
             to_delta(end) if end is not None else audio.duration,
-            metadata,
         )
 
     @classmethod
     @log_call(on_enter="Downloading '{metadata[album]}' from playlist {url}")
     def from_playlist(
             cls,
             url: str,
@@ -163,7 +163,37 @@
                     **metadata,
                     "track": i,
                     "title": video.title,
                     **data.get("metadata", {}),
                 },
                 **{k: v for k, v in data.items() if k != "metadata"},
             )
+
+    @classmethod
+    @log_call(on_enter="Downloading multitrack '{metadata[title]}'")
+    def from_multi_track(
+            cls,
+            *,
+            track_data: Iterable[STR_MAP],
+            metadata: Mapping[str, str],
+            cover_url: str = None,
+    ) -> Self:
+        """
+        Factory that constructs a Track from a list of videos.
+
+        :param track_data: An iterable of mappings of the form:
+                ``{"url": ..., "start": ..., "end": ...}``
+        :param metadata: A String map of FFMPEG MP3 metadata tags
+        :param cover_url: The url to a JPG cover image
+        :return: A new Track
+        """
+        track_data = [
+            (t["url"], t.get("start"), t.get("end")) for t in track_data
+        ]
+        logged_iter = log_iter(
+            on_each="Downloading track part {i}: {0[0]}", start=1,
+        )
+        audio = Audio.join(
+            Audio.from_url(url).snip(start, end)
+            for url, start, end in logged_iter(track_data)
+        )
+        return cls(audio, get_cover(track_data[0][0], cover_url), metadata)
```

### Comparing `pytubemusic-0.1.2/src/pytubemusic/utils.py` & `pytubemusic-0.2.0/src/pytubemusic/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import urllib.request
-from collections.abc import Iterable, Iterator, Mapping
+from collections.abc import Iterable, Mapping
 from datetime import datetime, timedelta
 from itertools import chain, pairwise
 from pathlib import PurePath
 from tempfile import NamedTemporaryFile
 from typing import Any
 
 from pytube import YouTube
 
 __all__ = [
-    "to_delta", "to_timestamp", "to_microseconds", "pathify", "make_track_data",
-    "set_ends", "merge_metadata", "get_cover", "thumbnail",
+    "to_delta", "to_timestamp", "to_microseconds", "pathify",
+    "set_ends", "merge_metadata", "get_cover",
 ]
 
 STR_MAP = Mapping[str, Any]
 TRACK_DATA = Iterable[STR_MAP]
 
 
 def to_delta(timestamp: str) -> timedelta:
@@ -50,35 +50,14 @@
     """
     Replaces invalid characters in filenames and joins the params to a path
     with the given extension
     """
     return root / (title.replace("/", "\u2044") + ext)
 
 
-def make_track_data(
-        track_data: list[Mapping],
-        end: timedelta,
-) -> Iterator[Mapping]:
-    """
-    Adds track number metadata to a list of track data and ensures tracks have
-    start and end timestamps
-
-    :param track_data: A list of string maps of incomplete track data
-    :param end: The length of the Album in seconds
-    :return: Yields string maps of track data
-    """
-    track_data = track_data + [{"start": to_timestamp(end)}]
-    for i, (t1, t2) in enumerate(pairwise(track_data), start=1):
-        yield t1 | {
-            "start": t1["start"],
-            "end": t1.get("end", t2["start"]),
-            "metadata": {"track": i} | t1.get("metadata", {}),
-        }
-
-
 def set_ends(track_data: TRACK_DATA, end: timedelta) -> TRACK_DATA:
     """
     Fills in missing "end" timestamps setting them to the start of the next
     track. Returns a new mapping of track data.
     """
     track_data = chain(track_data, [{"start": to_timestamp(end)}])
     for i, (t1, t2) in enumerate(pairwise(track_data), start=1):
@@ -94,19 +73,17 @@
     Merges any album metadata with track-specific metadata.
     Track metadata overrides album metadata.
     """
     for data in track_data:
         yield {**data, "metadata": {**metadata, **data["metadata"]}}
 
 
-def thumbnail(url) -> NamedTemporaryFile:
-    """Returns a default cover – the video's thumbnail"""
-    thumbnail_url = YouTube(url).thumbnail_url
-    return get_cover(thumbnail_url)
-
-
-def get_cover(url) -> NamedTemporaryFile:
+def get_cover(video_url, cover_url) -> NamedTemporaryFile:
     """Downloads an image into a named temporary file to be used as cover art"""
+    if cover_url is None:
+        url = YouTube(video_url).thumbnail_url
+    else:
+        url = cover_url
     f = NamedTemporaryFile(suffix='.jpg')
     img = urllib.request.urlopen(url).read()
     f.write(img)
     return f
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pytubemusic-0.1.2/src/pytubemusic/validation/__init__.py` & `pytubemusic-0.2.0/src/pytubemusic/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.1.2/src/pytubemusic/validation/schemata/album.schema.json` & `pytubemusic-0.2.0/src/pytubemusic/validation/schemata/album.schema.json`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.1.2/src/pytubemusic/validation/schemata/playlist.schema.json` & `pytubemusic-0.2.0/src/pytubemusic/validation/schemata/playlist.schema.json`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.1.2/src/pytubemusic/validation/schemata/track.schema.json` & `pytubemusic-0.2.0/src/pytubemusic/validation/schemata/track.schema.json`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.1.2/src/pytubemusic.egg-info/PKG-INFO` & `pytubemusic-0.2.0/src/pytubemusic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubemusic
-Version: 0.1.2
+Version: 0.2.0
 Summary: A cli that may or may not download albums from a certain website
 License: MIT License
         
         Copyright (c) 2023 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -40,34 +40,38 @@
 
 ```
 pip install pytubemusic
 ```
 
 **Requires [ffmpeg](https://ffmpeg.org/) to be installed on your machine.**
 
-### Installation Note
+<details>
+<summary>Installation Note</summary>
 
 PyTubeMusic uses the [PyTube](https://github.com/pytube/pytube) library. This
 can occasionally break. However, patches are usually quickly released as new
 versions or as pull requests. Try upgrading to the latest version of PyTube if
 downloading fails.
 
 > Note, to pip install from a pull request do:
 > ```text
 >  pip install git+https://github.com/pytube/pytube.git@refs/pull/<PR_NUM>/head
 > ```
 > Where `<PR_NUM>` is the number of the pull request.
 
+</details>
+
 ## Usage
 
 PyTubeMusic can download tracks in three formats:
 
 - Tracks (Single files)
 - Albums (A single video that is split up into individual tracks on an album)
 - Playlists (Videos in a playlist that are downloaded as tracks on an album)
+- Multi Tracks (Several videos that get combined into a single track)
 
 Each type of track needs a different configuration file that includes metadata.
 These are described below.
 
 Note: the term "timestamp" refers to a string of the form: "H?:M:S.f?" – for
 example: "23:55.75", "1:12:00", "5:03", "17:00.5"
 
@@ -137,19 +141,41 @@
 track_data = []
 
 [metadata]
 album = "..."  # Album name (required)
 # Any other FFMPEG MP3 metadata tags
 ```
 
+### Multi Tracks
+
+> Several videos combined into a single track
+
+Effectively a list of URLs with metadata and an optional cover image. Note
+that `track_data` here has a different format to other cli commands:
+
+```toml
+cover_url = "..."  # Track cover jpg URL (optional – uses thumbnail of first video by default)
+
+# Required track data
+track_data = [
+    # Url to video and optional start and end timestamps
+    { url = "...", start = "...", end = "..." },
+    # ...
+]
+
+[metadata]
+title = "..."  # Track name (required)
+# Any other FFMPEG MP3 metadata tags
+```
+
 ### CLI
 
 A `pytubemusic` command will be exposed.
 
-This has three commands: `album`, `track`, `playlist`.
+This has four commands: `album`, `track`, `playlist`, `multitrack`.
 Each command corresponds to one of the file types mentioned above.
 
 The commands all take the path to a config TOML file and an optional `-o`
 or `--out` option pointing to a directory to write the resulting tracks too.
 (Note: albums and playlists are put into their own subdirectory with the album
 name under the out directory).
```

### Comparing `pytubemusic-0.1.2/src/pytubemusic.egg-info/SOURCES.txt` & `pytubemusic-0.2.0/src/pytubemusic.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -12,10 +12,11 @@
 src/pytubemusic.egg-info/SOURCES.txt
 src/pytubemusic.egg-info/dependency_links.txt
 src/pytubemusic.egg-info/entry_points.txt
 src/pytubemusic.egg-info/requires.txt
 src/pytubemusic.egg-info/top_level.txt
 src/pytubemusic/validation/__init__.py
 src/pytubemusic/validation/schemata/album.schema.json
+src/pytubemusic/validation/schemata/multitrack.schema.json
 src/pytubemusic/validation/schemata/playlist.schema.json
 src/pytubemusic/validation/schemata/track.schema.json
 tests/test_utils.py
```

### Comparing `pytubemusic-0.1.2/tests/test_utils.py` & `pytubemusic-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

