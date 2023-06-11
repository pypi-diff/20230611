# Comparing `tmp/VocalForge-0.0.4.tar.gz` & `tmp/VocalForge-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VocalForge-0.0.4.tar", last modified: Thu Jun  1 02:33:44 2023, max compression
+gzip compressed data, was "VocalForge-0.0.5.tar", last modified: Sun Jun 11 00:11:28 2023, max compression
```

## Comparing `VocalForge-0.0.4.tar` & `VocalForge-0.0.5.tar`

### file list

```diff
@@ -1,36 +1,34 @@
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:33:44.242594 VocalForge-0.0.4/
--rw-rw-r--   0 rio       (1000) rio       (1000)     1067 2023-05-21 03:39:13.000000 VocalForge-0.0.4/LICENSE.md
--rw-rw-r--   0 rio       (1000) rio       (1000)     6310 2023-06-01 02:33:44.242594 VocalForge-0.0.4/PKG-INFO
--rw-rw-r--   0 rio       (1000) rio       (1000)     5774 2023-05-21 03:39:13.000000 VocalForge-0.0.4/README.md
--rw-rw-r--   0 rio       (1000) rio       (1000)      706 2023-06-01 02:33:01.000000 VocalForge-0.0.4/pyproject.toml
--rw-rw-r--   0 rio       (1000) rio       (1000)      312 2023-06-01 02:32:29.000000 VocalForge-0.0.4/requirements.txt
--rw-rw-r--   0 rio       (1000) rio       (1000)       38 2023-06-01 02:33:44.242594 VocalForge-0.0.4/setup.cfg
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:33:44.242594 VocalForge-0.0.4/src/
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:33:44.242594 VocalForge-0.0.4/src/VocalForge/
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:33:44.242594 VocalForge-0.0.4/src/VocalForge/audio/
--rw-rw-r--   0 rio       (1000) rio       (1000)      204 2023-05-31 00:06:05.000000 VocalForge-0.0.4/src/VocalForge/audio/__init__.py
--rw-rw-r--   0 rio       (1000) rio       (1000)    10276 2023-05-30 05:30:07.000000 VocalForge-0.0.4/src/VocalForge/audio/audio_utils.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     4708 2023-05-31 03:13:49.000000 VocalForge-0.0.4/src/VocalForge/audio/export_audio.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     5777 2023-05-31 03:15:02.000000 VocalForge-0.0.4/src/VocalForge/audio/isolate.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2068 2023-05-30 05:32:42.000000 VocalForge-0.0.4/src/VocalForge/audio/overlap.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2386 2023-05-31 00:06:30.000000 VocalForge-0.0.4/src/VocalForge/audio/refine_audio.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     3002 2023-05-30 05:31:11.000000 VocalForge-0.0.4/src/VocalForge/audio/voice_detection.py
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:33:44.242594 VocalForge-0.0.4/src/VocalForge/text/
--rw-rw-r--   0 rio       (1000) rio       (1000)      250 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/__init__.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     3555 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/create_dataset.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2211 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/ctc.py
--rw-rw-r--   0 rio       (1000) rio       (1000)    26284 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/ctc_utils.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     1666 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/normalization_helpers.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     4247 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/normalize_text.py
--rw-rw-r--   0 rio       (1000) rio       (1000)    10460 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/process_text.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2442 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/refine_text.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2277 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/segment.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     1759 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/split_audio.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     5407 2023-05-31 04:31:49.000000 VocalForge-0.0.4/src/VocalForge/text/text_utils.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2330 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/transcribe.py
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:33:44.242594 VocalForge-0.0.4/src/VocalForge.egg-info/
--rw-rw-r--   0 rio       (1000) rio       (1000)     6310 2023-06-01 02:33:44.000000 VocalForge-0.0.4/src/VocalForge.egg-info/PKG-INFO
--rw-rw-r--   0 rio       (1000) rio       (1000)      906 2023-06-01 02:33:44.000000 VocalForge-0.0.4/src/VocalForge.egg-info/SOURCES.txt
--rw-rw-r--   0 rio       (1000) rio       (1000)        1 2023-06-01 02:33:44.000000 VocalForge-0.0.4/src/VocalForge.egg-info/dependency_links.txt
--rw-rw-r--   0 rio       (1000) rio       (1000)      312 2023-06-01 02:33:44.000000 VocalForge-0.0.4/src/VocalForge.egg-info/requires.txt
--rw-rw-r--   0 rio       (1000) rio       (1000)       11 2023-06-01 02:33:44.000000 VocalForge-0.0.4/src/VocalForge.egg-info/top_level.txt
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 00:11:28.977277 VocalForge-0.0.5/
+-rw-rw-r--   0 rio       (1000) rio       (1000)     1067 2023-05-21 03:39:13.000000 VocalForge-0.0.5/LICENSE.md
+-rw-rw-r--   0 rio       (1000) rio       (1000)     6156 2023-06-11 00:11:28.977277 VocalForge-0.0.5/PKG-INFO
+-rw-rw-r--   0 rio       (1000) rio       (1000)     5774 2023-05-21 03:39:13.000000 VocalForge-0.0.5/README.md
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 00:11:28.973277 VocalForge-0.0.5/VocalForge/
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 00:11:28.977277 VocalForge-0.0.5/VocalForge/VocalForge.egg-info/
+-rw-rw-r--   0 rio       (1000) rio       (1000)     6156 2023-06-11 00:11:28.000000 VocalForge-0.0.5/VocalForge/VocalForge.egg-info/PKG-INFO
+-rw-rw-r--   0 rio       (1000) rio       (1000)      848 2023-06-11 00:11:28.000000 VocalForge-0.0.5/VocalForge/VocalForge.egg-info/SOURCES.txt
+-rw-rw-r--   0 rio       (1000) rio       (1000)        1 2023-06-11 00:11:28.000000 VocalForge-0.0.5/VocalForge/VocalForge.egg-info/dependency_links.txt
+-rw-rw-r--   0 rio       (1000) rio       (1000)      279 2023-06-11 00:11:28.000000 VocalForge-0.0.5/VocalForge/VocalForge.egg-info/requires.txt
+-rw-rw-r--   0 rio       (1000) rio       (1000)       11 2023-06-11 00:11:28.000000 VocalForge-0.0.5/VocalForge/VocalForge.egg-info/top_level.txt
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 00:11:28.977277 VocalForge-0.0.5/VocalForge/audio/
+-rw-rw-r--   0 rio       (1000) rio       (1000)      204 2023-05-31 00:06:05.000000 VocalForge-0.0.5/VocalForge/audio/__init__.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)    11150 2023-06-06 03:10:36.000000 VocalForge-0.0.5/VocalForge/audio/audio_utils.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     4439 2023-06-04 02:30:09.000000 VocalForge-0.0.5/VocalForge/audio/export_audio.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     9966 2023-06-04 02:30:19.000000 VocalForge-0.0.5/VocalForge/audio/isolate.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2706 2023-06-10 23:55:14.000000 VocalForge-0.0.5/VocalForge/audio/overlap.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2386 2023-05-31 00:06:30.000000 VocalForge-0.0.5/VocalForge/audio/refine_audio.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     3825 2023-06-10 23:51:14.000000 VocalForge-0.0.5/VocalForge/audio/voice_detection.py
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 00:11:28.977277 VocalForge-0.0.5/VocalForge/text/
+-rw-rw-r--   0 rio       (1000) rio       (1000)      250 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/__init__.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     3555 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/create_dataset.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2211 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/ctc.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)    26284 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/ctc_utils.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     1666 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/normalization_helpers.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     4247 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/normalize_text.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)    10460 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/process_text.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2442 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/refine_text.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2277 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/segment.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     1759 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/split_audio.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     5407 2023-05-31 04:31:49.000000 VocalForge-0.0.5/VocalForge/text/text_utils.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2330 2023-05-21 03:39:13.000000 VocalForge-0.0.5/VocalForge/text/transcribe.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     1076 2023-06-11 00:11:24.000000 VocalForge-0.0.5/pyproject.toml
+-rw-rw-r--   0 rio       (1000) rio       (1000)       38 2023-06-11 00:11:28.977277 VocalForge-0.0.5/setup.cfg
```

### Comparing `VocalForge-0.0.4/LICENSE.md` & `VocalForge-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.4/PKG-INFO` & `VocalForge-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: VocalForge
-Version: 0.0.4
+Version: 0.0.5
 Summary: Your one-stop solution for voice dataset creation
-Author-email: Rio Harper <rio@rioharper.com>
-Project-URL: Homepage, https://github.com/rioharper/VocalForge/
-Project-URL: Bug Tracker, https://github.com/rioharper/VocalForge/issues
+Author-email: rio@rioharper.com
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: audio
+Provides-Extra: text
 License-File: LICENSE.md
 
 # An End-to-End Toolkit for Voice Datasets
 
 `VocalForge` is an open-source toolkit written in Python 🐍  that is meant to cut down the time to create datasets for, TTS models, hotword detection models, and more so you can spend more time training, and less time sifting through audio data.
 
 Using [Nvidia's NEMO](https://github.com/NVIDIA/NeMo), [PyAnnote](https://github.com/pyannote/pyannote-audio), [CTC segmentation](https://github.com/lumaku/ctc-segmentation) , [OpenAI's Whisper](https://github.com/openai/whisper), this repo will take you from raw audio to a fully formatted dataset, refining both the audio and text automatically.
```

### Comparing `VocalForge-0.0.4/README.md` & `VocalForge-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.4/src/VocalForge/audio/audio_utils.py` & `VocalForge-0.0.5/VocalForge/audio/audio_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,31 +23,40 @@
         }],
         'outtmpl': os.path.join(out_dir, '%(title)s.%(ext)s'),
     }
 
     with yt_dlp.YoutubeDL(ydl_opts) as ydl:
         error_code = ydl.download(url)
 
+    #5 second blank as pyannote doesnt seem to process first ~3 seconds of audio
+    blank = AudioSegment.silent(duration=5000)
+    
     #split if audio is above 1 hour
     for filename in os.listdir(out_dir):
         file = AudioSegment.from_file(os.path.join(out_dir, filename))
         if len(file) > 3500000:
             slices = file[::3500000]
             for index, slice in enumerate(slices):
                 slice.export(os.path.join(out_dir, f'{os.path.splitext(filename)[0]}_{index}.wav'), format='wav')
             os.remove(os.path.join(out_dir, filename))
+        #add 5 second blank at start
+
 
     for filename in os.listdir(out_dir):
         file_stat = os.stat(os.path.join(out_dir, filename))
+        file = AudioSegment.from_file(os.path.join(out_dir, filename))
         if file_stat.st_size > 500000000:
-            file = AudioSegment.from_file(os.path.join(out_dir, filename))
             slices = file[::int((file.duration_seconds*1000)/2)]
             for index, slice in enumerate(slices):
+                slice = blank + slice
                 slice.export(os.path.join(out_dir, f'{os.path.splitext(filename)[0]}_{index}.wav'), format='wav')
             os.remove(os.path.join(out_dir, filename))
+        else:
+            file = blank + file
+            file.export(os.path.join(out_dir, filename), format='wav')
 
     for count, filename in enumerate(os.listdir(out_dir)):
         dst = f"DATA{count}.wav"
         src = os.path.join(out_dir, filename)
         dst = os.path.join(out_dir, dst)
         os.rename(src, dst)
 
@@ -210,22 +219,33 @@
         else:
             concatenated_timestamps.append([current_start, current_stop])
             current_start = timestamps[i][0]
             current_stop = timestamps[i][1]
     concatenated_timestamps.append([current_start, current_stop])
     return concatenated_timestamps
 
-
 def calculate_duration(timestamps: List[Tuple[int, int]]) -> float:
     '''pretty self expainatory'''
     duration = 0
     for timestamp in timestamps:
         duration += timestamp[1] - timestamp[0]
     return duration
 
+def find_original_duration(input_file_dir: str) -> float:
+    '''pretty self expainatory'''
+    raw = AudioSegment.from_file(input_file_dir, format="wav")
+    return raw.duration_seconds
+
+def find_duration_diff(new_timestamps: List[Tuple[int, int]], original_duration: float) -> float:
+    '''pretty self expainatory'''
+    new_duration = calculate_duration(new_timestamps)
+    # if abs(original_duration - new_duration) > original_duration * 0.8:
+    #     return abs(new_duration - original_duration)
+    return abs(original_duration - new_duration)
+
 
 def export_from_timestamps(input_file_dir, export_file_dir, timestamps: List[Tuple[int, int]], combine_mode: str = 'timestamps') -> None:
     ''''Exports audio from timestamps to a new file.
     
         Inputs:
         - input_file_dir: a string representing the directory path of the input audio file.
         - export_file_dir: a string representing the directory path to save the exported audio file.
```

### Comparing `VocalForge-0.0.4/src/VocalForge/audio/export_audio.py` & `VocalForge-0.0.5/VocalForge/audio/export_audio.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,43 +46,43 @@
         normalized = normalize(audio)
         normalized.export(os.path.join(output_dir, os.path.basename(file_dir)), format="wav")
 
     def normalize_folder(self) -> None:
         """
         Normalize all audio files in the export directory and export them to the normalization directory.
         """
-        for file in get_files(self.Export_Dir, True):
-            audio = AudioSegment.from_file(file, format="wav")
+        for file in get_files(self.Export_Dir):
+            file_dir = os.path.join(self.Export_Dir, file)
+            audio = AudioSegment.from_file(file_dir, format="wav")
             normalized = normalize(audio)
             normalized.export(os.path.join(self.Normalization_Dir, os.path.basename(file)), format="wav")
 
-    def noise_remove_folder(self, input_folder_dir: Optional[str] = None) -> None:
+    def noise_remove(self) -> None:
         """
-        Remove noise from all audio files in the specified directory and export them to the noise-removed directory.
+        Removes noise from audio files in `file_or_folder` directory or file.
 
-        Args:
-            input_folder_dir (str, optional): The directory containing the audio files to remove noise from. Defaults to None.
-        """
-        if input_folder_dir is None:
-            input_folder_dir = self.Input_Dir
-        elif input_folder_dir is None and self.Input_Dir is None:
-            raise ValueError("Please provide either the folder_dir or the Noise_Removed_Dir")
+        Parameters:
+        file_or_folder (str or os.PathLike): The directory or file containing the audio files.
+        sample_rate (int): The sample rate of the audio files.
 
+        Returns:
+        None
+        """
         model, df_state, _ = init_df(config_allow_defaults=True)
 
-        for file in get_files(input_folder_dir, True, ".wav"):
+        for file in self.Input_Files:
+            print(f"Removing Noise from {file}...")
             try:
-                audio, _ = load_audio(file, sr=df_state.sr())
+                file_dir = os.path.join(self.Export_Dir, file)
+                audio, _ = load_audio(file_dir, sr=self.Sample_Rate)
                 enhanced = enhance(model, df_state, audio)
-                save_audio(os.path.join(self.Noise_Removed_Dir, os.path.basename(file)), enhanced, df_state.sr())
+                save_audio(file_dir, enhanced, sr=self.Sample_Rate)
                 cuda.empty_cache()
             except RuntimeError:
                 print(f"file is too large for GPU, skipping: {file}")
-                os.system(f"cp {file} {self.Noise_Removed_Dir}")
-        del model, df_state
 
     def format_audio_folder(self) -> None:
         """
         Format all audio files in the input directory and export them to the export directory.
         """
         for file in get_files(self.Input_Dir, full_dir=True, ext=".wav"):
             raw = AudioSegment.from_file(file, format="wav")
@@ -97,12 +97,12 @@
         if os.listdir(self.Export_Dir) != []:
             print("file(s) have already been formatted! Skipping...")
         else:
             self.format_audio_folder()
 
         if self.Noise_Removed_Dir is not None and os.listdir(self.Noise_Removed_Dir) == []:
             print("Removing Noise...")
-            self.noise_remove_folder(self.Export_Dir)
+            self.noise_remove()
 
         if self.Normalization_Dir is not None and os.listdir(self.Normalization_Dir) == []:
             print("Normalizing Audio...")
             self.normalize_folder()
```

### Comparing `VocalForge-0.0.4/src/VocalForge/audio/overlap.py` & `VocalForge-0.0.5/VocalForge/audio/overlap.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,66 @@
-from .audio_utils import get_files, concentrate_timestamps
+from .audio_utils import get_files
 from .audio_utils import get_timestamps, export_from_timestamps
 import os
-from pydub import AudioSegment
+from pyannote.audio import Pipeline
 
 class Overlap:
-    def __init__(self, input_dir=None, output_dir=None):
+    def __init__(self, input_dir=None, output_dir=None, hparams=None):
         self.Input_Dir = input_dir
         self.Output_Dir = output_dir
         self.Input_Files = get_files(self.Input_Dir, True, '.wav')
         self.Timelines = []
         self.Timestamps = []
-
+        self.Hparams = hparams
+        
+        
+        # Create a pipeline object using the pre-trained "pyannote/overlapped-speech-detection"
+        self.Pipeline = Pipeline.from_pretrained("pyannote/overlapped-speech-detection",
+                                            use_auth_token=True)
+        
+        self.isHparams = False
+        if self.Hparams is not None:
+            self.Pipeline.instantiate(self.Hparams)
+            self.isHparams = True
 
     def analyze(self) -> list:
         """
         Analyzes overlapping speech in a set of speech audio files.
 
         Parameters:
         input_dir: (str) dir of input wav files 
         """
-        from pyannote.audio import Pipeline
-        # Create a pipeline object using the pre-trained "pyannote/overlapped-speech-detection"
-        pipeline = Pipeline.from_pretrained("pyannote/overlapped-speech-detection",
-                                            use_auth_token=True)
+        
+        
+        if self.Hparams is not None and self.isHparams == False:
+            self.Pipeline.instantiate(self.Hparams)
+            self.isHparams = True
         
         for file in self.Input_Files:
-            overlap_timeline = pipeline(file)
+            overlap_timeline = self.Pipeline(file)
             self.Timelines.append(overlap_timeline)
 
 
     def find_timestamps(self):
         """
         This function processes speech metrics and returns timestamps
         of overlapping segments in the audio."""
         self.Timestamps = []
         for fileindex in range(len(self.Input_Files)):
             timestamps = get_timestamps(self.Timelines[fileindex])
             self.Timestamps.append(timestamps)
+
+    
+    def update_timeline(self, new_timeline, index: int):
+        """
+        This function updates the timeline for a given file with the new timestamps due to finetuning
+        """
+        self.Timelines[index] = new_timeline
+
+        self.Timestamps[index] = get_timestamps(new_timeline)
     
 
     def test_export(self):
         for index, file in enumerate(self.Input_Files):
             base_file_name = file.split('/')[-1]
             export_from_timestamps(file, os.path.join(self.Output_Dir, base_file_name), self.Timestamps[index], combine_mode='time_between')
```

### Comparing `VocalForge-0.0.4/src/VocalForge/audio/refine_audio.py` & `VocalForge-0.0.5/VocalForge/audio/refine_audio.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.4/src/VocalForge/text/create_dataset.py` & `VocalForge-0.0.5/VocalForge/text/create_dataset.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.4/src/VocalForge/text/ctc.py` & `VocalForge-0.0.5/VocalForge/text/ctc.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.4/src/VocalForge/text/ctc_utils.py` & `VocalForge-0.0.5/VocalForge/text/ctc_utils.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.4/src/VocalForge/text/normalization_helpers.py` & `VocalForge-0.0.5/VocalForge/text/normalization_helpers.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.4/src/VocalForge/text/normalize_text.py` & `VocalForge-0.0.5/VocalForge/text/normalize_text.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.4/src/VocalForge/text/process_text.py` & `VocalForge-0.0.5/VocalForge/text/process_text.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.4/src/VocalForge/text/refine_text.py` & `VocalForge-0.0.5/VocalForge/text/refine_text.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.4/src/VocalForge/text/segment.py` & `VocalForge-0.0.5/VocalForge/text/segment.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.4/src/VocalForge/text/split_audio.py` & `VocalForge-0.0.5/VocalForge/text/split_audio.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.4/src/VocalForge/text/text_utils.py` & `VocalForge-0.0.5/VocalForge/text/text_utils.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.4/src/VocalForge/text/transcribe.py` & `VocalForge-0.0.5/VocalForge/text/transcribe.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.4/src/VocalForge.egg-info/PKG-INFO` & `VocalForge-0.0.5/VocalForge/VocalForge.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: VocalForge
-Version: 0.0.4
+Version: 0.0.5
 Summary: Your one-stop solution for voice dataset creation
-Author-email: Rio Harper <rio@rioharper.com>
-Project-URL: Homepage, https://github.com/rioharper/VocalForge/
-Project-URL: Bug Tracker, https://github.com/rioharper/VocalForge/issues
+Author-email: rio@rioharper.com
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: audio
+Provides-Extra: text
 License-File: LICENSE.md
 
 # An End-to-End Toolkit for Voice Datasets
 
 `VocalForge` is an open-source toolkit written in Python 🐍  that is meant to cut down the time to create datasets for, TTS models, hotword detection models, and more so you can spend more time training, and less time sifting through audio data.
 
 Using [Nvidia's NEMO](https://github.com/NVIDIA/NeMo), [PyAnnote](https://github.com/pyannote/pyannote-audio), [CTC segmentation](https://github.com/lumaku/ctc-segmentation) , [OpenAI's Whisper](https://github.com/openai/whisper), this repo will take you from raw audio to a fully formatted dataset, refining both the audio and text automatically.
```

