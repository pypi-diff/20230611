# Comparing `tmp/videoslides-0.0.5.tar.gz` & `tmp/videoslides-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\videoslides-0.0.5.tar", last modified: Fri May 19 16:30:38 2023, max compression
+gzip compressed data, was "dist\videoslides-0.0.6.tar", last modified: Sun Jun 11 01:14:22 2023, max compression
```

## Comparing `videoslides-0.0.5.tar` & `videoslides-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 16:30:38.000000 videoslides-0.0.5/
--rw-rw-rw-   0        0        0     6063 2022-07-20 03:36:12.000000 videoslides-0.0.5/esquema.drawio
--rw-rw-rw-   0        0        0     1103 2022-07-12 04:02:52.000000 videoslides-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0       46 2022-07-12 05:01:15.000000 videoslides-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1398 2023-05-19 16:30:38.000000 videoslides-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      767 2022-07-14 02:45:05.000000 videoslides-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-19 16:30:38.000000 videoslides-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2049 2023-05-19 16:26:07.000000 videoslides-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:30:38.000000 videoslides-0.0.5/src/
--rw-rw-rw-   0        0        0    45516 2023-05-11 02:57:14.000000 videoslides-0.0.5/src/functions.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:30:38.000000 videoslides-0.0.5/src/videoslides.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-19 16:30:38.000000 videoslides-0.0.5/src/videoslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1398 2023-05-19 16:30:38.000000 videoslides-0.0.5/src/videoslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-05-19 16:30:38.000000 videoslides-0.0.5/src/videoslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0      303 2023-05-19 16:30:38.000000 videoslides-0.0.5/src/videoslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       22 2023-05-19 16:30:38.000000 videoslides-0.0.5/src/videoslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13048 2023-05-11 03:10:08.000000 videoslides-0.0.5/src/videoslides.py
--rw-rw-rw-   0        0        0        0 2022-07-12 02:31:10.000000 videoslides-0.0.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 01:14:22.000000 videoslides-0.0.6/
+-rw-rw-rw-   0        0        0    42900 2023-06-09 22:00:49.000000 videoslides-0.0.6/esquema.drawio
+-rw-rw-rw-   0        0        0     1103 2022-07-12 04:02:52.000000 videoslides-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       46 2022-07-12 05:01:15.000000 videoslides-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1398 2023-06-11 01:14:22.000000 videoslides-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2022-07-14 02:45:05.000000 videoslides-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-11 01:14:22.000000 videoslides-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2120 2023-06-11 01:12:37.000000 videoslides-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 01:14:22.000000 videoslides-0.0.6/src/
+-rw-rw-rw-   0        0        0    45554 2023-06-10 22:06:28.000000 videoslides-0.0.6/src/functions.py
+drwxrwxrwx   0        0        0        0 2023-06-11 01:14:22.000000 videoslides-0.0.6/src/videoslides.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-11 01:14:21.000000 videoslides-0.0.6/src/videoslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1398 2023-06-11 01:14:21.000000 videoslides-0.0.6/src/videoslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-06-11 01:14:21.000000 videoslides-0.0.6/src/videoslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      303 2023-06-11 01:14:21.000000 videoslides-0.0.6/src/videoslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       22 2023-06-11 01:14:21.000000 videoslides-0.0.6/src/videoslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13496 2023-06-10 22:39:55.000000 videoslides-0.0.6/src/videoslides.py
+-rw-rw-rw-   0        0        0        0 2022-07-12 02:31:10.000000 videoslides-0.0.6/src/__init__.py
```

### Comparing `videoslides-0.0.5/LICENSE.txt` & `videoslides-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.5/PKG-INFO` & `videoslides-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videoslides
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file 
 Home-page: https://github.com/Zes7one/VideoSlides
 Author: Franco Palma
 Author-email: franco.pm10@gmail.com 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `videoslides-0.0.5/README.md` & `videoslides-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.5/setup.py` & `videoslides-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="videoslides",
-    version='0.0.5',
+    version='0.0.6',
     description='Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file ',
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=["videoslides", "functions"],
     package_dir={'':'src'},
     install_requires=[
         "easyocr >= 1.4.1",
@@ -17,15 +17,16 @@
         "numpy >= 1.19.5",
         "matplotlib >= 3.3.4",
         "pytube >= 12.0.0",
         "scikit-image >= 0.17.2",
         "validators >= 0.20.0",
         "nltk >= 3.6.7",
         "opencv-python-headless >= 4.1.2.30",
-        "sewar >= 0.4.5" 
+        "sewar >= 0.4.5",
+        "pytesseract >= 0.3.8"
     ],
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent", 
         "Intended Audience :: Developers"
     ],
@@ -62,8 +63,9 @@
 
 # py setup.py bdist_wheel sdist
 # cd dist
 # dir 
 
 # Subir a Pypi
 # pip install twine
-# twine upload dist/*
+# twine upload dist/*
+# twine upload --skip-existing dist/*
```

### Comparing `videoslides-0.0.5/src/functions.py` & `videoslides-0.0.6/src/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,16 @@
     '''
     try:
         video = YouTube(url)
         title = video.title
         video = video.streams.get_highest_resolution()
         video.download()
         return True, title
-    except:
+    except Exception as e:
+        print(str(e))
         return False, ""
 
 def getqua(frame1, frame2, rgb = False, me = 4): 
     """ Funcion que compara dos frames con la metrica que indica el parametro "me"
     1:SSIM, 2:dif, 3:mse, 4:psnr, 5:uqi
     -------------------------------------------------------
     Input:
```

### Comparing `videoslides-0.0.5/src/videoslides.egg-info/PKG-INFO` & `videoslides-0.0.6/src/videoslides.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videoslides
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file 
 Home-page: https://github.com/Zes7one/VideoSlides
 Author: Franco Palma
 Author-email: franco.pm10@gmail.com 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `videoslides-0.0.5/src/videoslides.py` & `videoslides-0.0.6/src/videoslides.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import warnings
 
 import cv2
 import validators
-
+from pathlib import Path
 import functions as fc
 
 
 class Video:
     def __init__(self, path, scale = 100 , saltos = 1, rgb = False, runtime = True, lematiz = False, gpu_use = False, pix_lim = 0.001, ssimv_lim = 0.999): # scale:percent of original size
         """ Clase para manejar el video, frames y transcripcion 
         path (str): link del video o a la ruta local del archivo mp4
@@ -23,14 +23,15 @@
         self.pix_lim, self.ssimv_lim = pix_lim, ssimv_lim
         # ------------ Video de Youtube ------------
         extension = "mp4"
         if (validators.url(path)):
             status, real_VideoName = fc.download_video(path)
             real_VideoName = real_VideoName.replace("|", "")
             if(not status):
+                print(status)
                 raise Exception("El link entregado no es un video")
             # RutaFolder = os.path.dirname(os.path.abspath(__file__))+"\\"
             RutaFolder = os.path.abspath(os.getcwd())+"\\"
             self.path = RutaFolder+real_VideoName+f".{extension}"
             self.video_name = real_VideoName
         # ------------------------------------------
         # ------------ Video desde directorio ------------
@@ -43,16 +44,20 @@
             self.video_name = real_VideoName.replace(f".{extension}", "") #.replace("y2mate.com", "").replace(" ", "").replace(".", "").replace("-", "")
         # ------------------------------------------------
             
         # ------------ Se crea carpeta y se captura el video ------------
         self.frames_path = ""
         if(not runtime):
             self.frames_path = RutaFolder+"F_"+self.video_name+"\\"
+            # print('Path(self.frames_path)')
+            # print(self.frames_path)
+            # print(Path(self.frames_path))
             if (not os.path.isdir(self.frames_path)):
-                os.mkdir(self.frames_path)
+                os.mkdir(Path(self.frames_path) ) # data_folder = Path("source_data/text_files/")
+                # os.mkdir(self.frames_path) # data_folder = Path("source_data/text_files/")
         vidcap = cv2.VideoCapture(RutaFolder+self.video_name+f".{extension}")
         self.video_cap = vidcap
         # ---------------------------------------------------------------
         
         # ------------ Se elimina el video en caso de runtime y link ------------
         # if(runtime and link): 
         #     # TODO Se borra la carpeta con los frames -> solo se puede cuando se deje de usar el vidcap
@@ -65,18 +70,18 @@
         #     warnings.warn(string)
         # ---------------------------------------------------------------------
 
         self.num_frames = int(vidcap.get(cv2.CAP_PROP_FRAME_COUNT))
         self.fps    = int(vidcap.get(cv2.CAP_PROP_FPS))
         # ------------ Se lee un frame y se obtiene las dimensiones ------------
         success,image = vidcap.read()	
-        if(not rgb):
-            image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY) 
         if(not success):
             raise Exception("Problemas en la captura del video: video corrupto o formato incorrecto")
+        if(not rgb):
+            image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY) 
         width = int(image.shape[1] * scale / 100)
         height = int(image.shape[0] * scale / 100)
         dim = (width, height)
         self.dim = dim
         # ----------------------------------------------------------------------
 
         # ------------ Se guardan los frames o se crea lista de frames ------------
@@ -89,15 +94,16 @@
         while (count < self.num_frames-1):
             if(count%(self.fps*saltos) == 0):
                 # resize image
                 resized = cv2.resize(image, dim, interpolation = cv2.INTER_AREA)
                 if(runtime):
                     frames.append(resized)
                 else:
-                    cv2.imwrite(self.frames_path+"%d.jpg" % count, resized)     # save frame as JPEG file  
+                    # cv2.imwrite(Path(self.frames_path+f"{count}.jpg"), resized)     # save frame as JPEG file  
+                    cv2.imwrite(self.frames_path+f"{count}.jpg", resized)     # save frame as JPEG file  
             success,image = vidcap.read()
             if(not rgb):
                 image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY) 
             count += 1
 
         self.frames = frames
         # -------------------------------------------------------------------------
```

