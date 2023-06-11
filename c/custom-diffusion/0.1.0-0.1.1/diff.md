# Comparing `tmp/custom_diffusion-0.1.0.tar.gz` & `tmp/custom_diffusion-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_diffusion-0.1.0.tar", last modified: Sat Jun 10 13:20:54 2023, max compression
+gzip compressed data, was "custom_diffusion-0.1.1.tar", last modified: Sun Jun 11 10:56:52 2023, max compression
```

## Comparing `custom_diffusion-0.1.0.tar` & `custom_diffusion-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 13:20:54.259650 custom_diffusion-0.1.0/
--rw-rw-rw-   0        0        0    11558 2023-06-07 17:52:13.000000 custom_diffusion-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       24 2023-06-09 11:29:48.000000 custom_diffusion-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2598 2023-06-10 13:20:54.259650 custom_diffusion-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1431 2023-06-10 13:17:02.000000 custom_diffusion-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 13:20:54.230750 custom_diffusion-0.1.0/custom_diffusion/
--rw-rw-rw-   0        0        0       23 2023-06-10 13:19:54.000000 custom_diffusion-0.1.0/custom_diffusion/__init__.py
--rw-rw-rw-   0        0        0     1618 2023-06-10 13:11:21.000000 custom_diffusion-0.1.0/custom_diffusion/demo.py
--rw-rw-rw-   0        0        0     9310 2023-06-10 12:22:15.000000 custom_diffusion-0.1.0/custom_diffusion/preprocces.py
-drwxrwxrwx   0        0        0        0 2023-06-10 13:20:54.257654 custom_diffusion-0.1.0/custom_diffusion/utils/
--rw-rw-rw-   0        0        0        0 2023-06-09 11:02:04.000000 custom_diffusion-0.1.0/custom_diffusion/utils/__init__.py
--rw-rw-rw-   0        0        0     2242 2023-06-09 11:02:04.000000 custom_diffusion-0.1.0/custom_diffusion/utils/data_utils.py
--rw-rw-rw-   0        0        0     1375 2023-06-09 11:02:04.000000 custom_diffusion-0.1.0/custom_diffusion/utils/downloads.py
--rw-rw-rw-   0        0        0     1307 2023-06-10 12:22:15.000000 custom_diffusion-0.1.0/custom_diffusion/utils/scheduler_utils.py
--rw-rw-rw-   0        0        0     3637 2023-06-09 11:02:04.000000 custom_diffusion-0.1.0/custom_diffusion/utils/video_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-10 13:20:54.246686 custom_diffusion-0.1.0/custom_diffusion.egg-info/
--rw-rw-rw-   0        0        0     2598 2023-06-10 13:20:54.000000 custom_diffusion-0.1.0/custom_diffusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2023-06-10 13:20:54.000000 custom_diffusion-0.1.0/custom_diffusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 13:20:54.000000 custom_diffusion-0.1.0/custom_diffusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      175 2023-06-10 13:20:54.000000 custom_diffusion-0.1.0/custom_diffusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-10 13:20:54.000000 custom_diffusion-0.1.0/custom_diffusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-06-09 11:02:04.000000 custom_diffusion-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      123 2023-06-10 12:22:15.000000 custom_diffusion-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0      375 2023-06-10 13:20:54.262643 custom_diffusion-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2218 2023-06-09 11:29:48.000000 custom_diffusion-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 10:56:52.429332 custom_diffusion-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2023-06-07 17:52:13.000000 custom_diffusion-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-06-09 11:29:48.000000 custom_diffusion-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2595 2023-06-11 10:56:52.430313 custom_diffusion-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1451 2023-06-11 10:55:21.000000 custom_diffusion-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 10:56:52.384073 custom_diffusion-0.1.1/custom_diffusion/
+-rw-rw-rw-   0        0        0       23 2023-06-11 10:56:31.000000 custom_diffusion-0.1.1/custom_diffusion/__init__.py
+-rw-rw-rw-   0        0        0     1636 2023-06-11 10:55:21.000000 custom_diffusion-0.1.1/custom_diffusion/demo.py
+drwxrwxrwx   0        0        0        0 2023-06-11 10:56:52.416266 custom_diffusion-0.1.1/custom_diffusion/pipelines/
+-rw-rw-rw-   0        0        0        0 2023-06-11 10:55:21.000000 custom_diffusion-0.1.1/custom_diffusion/pipelines/__init__.py
+-rw-rw-rw-   0        0        0     6872 2023-06-10 12:22:15.000000 custom_diffusion-0.1.1/custom_diffusion/pipelines/controlnet_inpaint_pipeline.py
+-rw-rw-rw-   0        0        0     7175 2023-06-11 10:55:21.000000 custom_diffusion-0.1.1/custom_diffusion/pipelines/controlnet_pipeline.py
+-rw-rw-rw-   0        0        0     9308 2023-06-11 10:55:21.000000 custom_diffusion-0.1.1/custom_diffusion/preprocces.py
+drwxrwxrwx   0        0        0        0 2023-06-11 10:56:52.427323 custom_diffusion-0.1.1/custom_diffusion/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-09 11:02:04.000000 custom_diffusion-0.1.1/custom_diffusion/utils/__init__.py
+-rw-rw-rw-   0        0        0     2242 2023-06-11 10:45:10.000000 custom_diffusion-0.1.1/custom_diffusion/utils/data_utils.py
+-rw-rw-rw-   0        0        0     1791 2023-06-11 10:55:21.000000 custom_diffusion-0.1.1/custom_diffusion/utils/downloads.py
+-rw-rw-rw-   0        0        0     1307 2023-06-10 12:22:15.000000 custom_diffusion-0.1.1/custom_diffusion/utils/scheduler_utils.py
+-rw-rw-rw-   0        0        0     3637 2023-06-11 10:55:21.000000 custom_diffusion-0.1.1/custom_diffusion/utils/video_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-11 10:56:52.411177 custom_diffusion-0.1.1/custom_diffusion.egg-info/
+-rw-rw-rw-   0        0        0     2595 2023-06-11 10:56:52.000000 custom_diffusion-0.1.1/custom_diffusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      699 2023-06-11 10:56:52.000000 custom_diffusion-0.1.1/custom_diffusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 10:56:52.000000 custom_diffusion-0.1.1/custom_diffusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      175 2023-06-11 10:56:52.000000 custom_diffusion-0.1.1/custom_diffusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-11 10:56:52.000000 custom_diffusion-0.1.1/custom_diffusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-06-09 11:02:04.000000 custom_diffusion-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      123 2023-06-10 12:22:15.000000 custom_diffusion-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0      375 2023-06-11 10:56:52.436282 custom_diffusion-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2218 2023-06-09 11:29:48.000000 custom_diffusion-0.1.1/setup.py
```

### Comparing `custom_diffusion-0.1.0/LICENSE` & `custom_diffusion-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.0/PKG-INFO` & `custom_diffusion-0.1.1/custom_diffusion.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
-Name: custom_diffusion
-Version: 0.1.0
+Name: custom-diffusion
+Version: 0.1.1
 Summary: Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
 Home-page: https://github.com/kadirnar/Custom-Diffusion
 Author: kadirnar
 License: Apache License 2.0
 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion models,controlnet,stable diffusion
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -40,15 +39,15 @@
 ### Installation
 ```bash
 pip install custom_diffusion
 ```
 
 ### Usage
 ```python
-from custom_diffusion.pipelines import StableDiffusionControlNetGenerator
+from custom_diffusion.pipelines.controlnet_pipeline import StableDiffusionControlNetGenerator
 
 
 generator = StableDiffusionControlNetGenerator()
 
 generated_image = generator.generate_image(
      stable_model_path="runwayml/stable-diffusion-v1-5"
      controlnet_model_path="lllyasviel/control_v11p_sd15_canny",
@@ -65,9 +64,7 @@
      controlnet_conditioning_scale=1.0,
      generator_seed=0,
      preprocess_type="Canny",
      resize_type="center_crop_and_resize",
      crop_size=512,
 )
 ```
-
-
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1 Name: custom_diffusion Version: 0.1.0 Summary: Custom
+Metadata-Version: 2.1 Name: custom-diffusion Version: 0.1.1 Summary: Custom
 Diffusion: Creating Video from Frame Using Multiple Diffusion Home-page: https:
 //github.com/kadirnar/Custom-Diffusion Author: kadirnar License: Apache License
 2.0 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion
-models,controlnet,stable diffusion Platform: UNKNOWN Classifier: Development
-Status :: 5 - Production/Stable Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Science/Research Classifier: Programming Language :: Python :: 3 Classifier:
+models,controlnet,stable diffusion Classifier: Development Status :: 5 -
+Production/Stable Classifier: Operating System :: OS Independent Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Science/
+Research Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Requires-Python: >=3.6 Description-
 Content-Type: text/markdown Provides-Extra: dev License-File: LICENSE
   ***** Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
                                      *****
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 ### Installation ```bash pip install custom_diffusion ``` ### Usage ```python
-from custom_diffusion.pipelines import StableDiffusionControlNetGenerator
-generator = StableDiffusionControlNetGenerator() generated_image =
-generator.generate_image( stable_model_path="runwayml/stable-diffusion-v1-5"
+from custom_diffusion.pipelines.controlnet_pipeline import
+StableDiffusionControlNetGenerator generator =
+StableDiffusionControlNetGenerator() generated_image = generator.generate_image
+( stable_model_path="runwayml/stable-diffusion-v1-5"
 controlnet_model_path="lllyasviel/control_v11p_sd15_canny",
 scheduler_name="DDIM", image_path="test.png", prompt="Anime boy",
 negative_prompt="bad", height=512, width=512, guess_mode=False,
 num_images_per_prompt=1, num_inference_steps=20, guidance_scale=7.0,
 controlnet_conditioning_scale=1.0, generator_seed=0, preprocess_type="Canny",
 resize_type="center_crop_and_resize", crop_size=512, ) ```
```

### Comparing `custom_diffusion-0.1.0/README.md` & `custom_diffusion-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ### Installation
 ```bash
 pip install custom_diffusion
 ```
 
 ### Usage
 ```python
-from custom_diffusion.pipelines import StableDiffusionControlNetGenerator
+from custom_diffusion.pipelines.controlnet_pipeline import StableDiffusionControlNetGenerator
 
 
 generator = StableDiffusionControlNetGenerator()
 
 generated_image = generator.generate_image(
      stable_model_path="runwayml/stable-diffusion-v1-5"
      controlnet_model_path="lllyasviel/control_v11p_sd15_canny",
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
   ***** Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
                                      *****
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 ### Installation ```bash pip install custom_diffusion ``` ### Usage ```python
-from custom_diffusion.pipelines import StableDiffusionControlNetGenerator
-generator = StableDiffusionControlNetGenerator() generated_image =
-generator.generate_image( stable_model_path="runwayml/stable-diffusion-v1-5"
+from custom_diffusion.pipelines.controlnet_pipeline import
+StableDiffusionControlNetGenerator generator =
+StableDiffusionControlNetGenerator() generated_image = generator.generate_image
+( stable_model_path="runwayml/stable-diffusion-v1-5"
 controlnet_model_path="lllyasviel/control_v11p_sd15_canny",
 scheduler_name="DDIM", image_path="test.png", prompt="Anime boy",
 negative_prompt="bad", height=512, width=512, guess_mode=False,
 num_images_per_prompt=1, num_inference_steps=20, guidance_scale=7.0,
 controlnet_conditioning_scale=1.0, generator_seed=0, preprocess_type="Canny",
 resize_type="center_crop_and_resize", crop_size=512, ) ```
```

### Comparing `custom_diffusion-0.1.0/custom_diffusion/demo.py` & `custom_diffusion-0.1.1/custom_diffusion/demo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from custom_diffusion.pipelines import StableDiffusionControlNetGenerator
+from custom_diffusion.pipelines.controlnet_pipeline import StableDiffusionControlNetGenerator
+
 
 def main(
     stable_model_path: str = "runwayml/stable-diffusion-v1-5",
     controlnet_model_path: str = "lllyasviel/control_v11p_sd15_canny",
     scheduler_name: str = "DDIM",
     image_path: str = "test.png",
     prompt: str = "Anime boy",
@@ -14,15 +15,15 @@
     num_inference_steps: int = 20,
     guidance_scale: float = 7.0,
     controlnet_conditioning_scale: float = 1.0,
     generator_seed: int = 0,
     preprocess_type: str = "Canny",
     resize_type: str = "center_crop_and_resize",
     crop_size: int = 512,
-    ):
+):
     generator = StableDiffusionControlNetGenerator()
 
     generated_image = generator.generate_image(
         stable_model_path=stable_model_path,
         controlnet_model_path=controlnet_model_path,
         scheduler_name=scheduler_name,
         image_path=image_path,
```

### Comparing `custom_diffusion-0.1.0/custom_diffusion/preprocces.py` & `custom_diffusion-0.1.1/custom_diffusion/preprocces.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     bg_threhold = 0.4
     x = cv2.Sobel(image, cv2.CV_32F, 1, 0, ksize=3)
     x[image_depth < bg_threhold] = 0
     y = cv2.Sobel(image, cv2.CV_32F, 0, 1, ksize=3)
     y[image_depth < bg_threhold] = 0
     z = np.ones_like(x) * np.pi * 2.0
     image = np.stack([x, y, z], axis=2)
-    image /= np.sum(image ** 2.0, axis=2, keepdims=True) ** 0.5
+    image /= np.sum(image**2.0, axis=2, keepdims=True) ** 0.5
     image = (image * 127.5 + 127.5).clip(0, 255).astype(np.uint8)
     image = Image.fromarray(image)
 
     return image
 
 
 def pose_image(image):
```

### Comparing `custom_diffusion-0.1.0/custom_diffusion/utils/data_utils.py` & `custom_diffusion-0.1.1/custom_diffusion/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.0/custom_diffusion/utils/downloads.py` & `custom_diffusion-0.1.1/custom_diffusion/utils/downloads.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-def download_video(
-    video_url: str = "https://www.youtube.com/watch?v=8QRG4vzbdE0",
+def download_from_youtube_url(
+    youtube_video_url: str = "https://www.youtube.com/watch?v=8QRG4vzbdE0",
     output_path: str = "output_videos",
     quality: str = "720p",
     filename: str = "downloaded_video.mp4",
 ):
     """
     This function downloads a video and corresponding audio from YouTube and saves it in the designated output folder.
 
@@ -17,21 +17,36 @@
     None
     """
     import os
 
     from pytube import YouTube
 
     # Create a YouTube object
-    yt = YouTube(video_url)
+    yt = YouTube(youtube_video_url)
 
     # Find the stream with the desired quality that also contains audio
     video_stream = yt.streams.filter(progressive=True, file_extension="mp4", res=quality).first()
 
     if video_stream is not None:
         # Download the stream
         video_stream.download(output_path, filename=filename)
         print("Video downloaded successfully!")
     else:
         print(f"No video stream found for {quality} quality.")
 
     save_path = os.path.join(output_path, filename)
     return save_path
+
+
+def download_from_url(from_url: str, to_path: str):
+    # https://github.com/obss/sahi/blob/main/sahi/utils/file.py
+    import os
+    import urllib.request
+    from pathlib import Path
+
+    Path(to_path).parent.mkdir(parents=True, exist_ok=True)
+
+    if not os.path.exists(to_path):
+        urllib.request.urlretrieve(
+            from_url,
+            to_path,
+        )
```

### Comparing `custom_diffusion-0.1.0/custom_diffusion/utils/scheduler_utils.py` & `custom_diffusion-0.1.1/custom_diffusion/utils/scheduler_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.0/custom_diffusion/utils/video_utils.py` & `custom_diffusion-0.1.1/custom_diffusion/utils/video_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,31 +30,31 @@
         # Read frame
         success, image = vidcap.read()
 
         if success:
             # Only save frame if it is the right id (based on frame_rate)
             if frame_id % frame_rate == 0:
                 # Save frame to specified output path with zero-padded file name
-                cv2.imwrite(os.path.join(output_path, f"{str(count).zfill(5)}.jpg"), image)
+                cv2.imwrite(os.path.join(output_path, f"{str(count).zfill(5)}.png"), image)
                 count += 1
 
             frame_id += 1
 
     print("Video frames saved successfully!")
 
     return output_path
 
 
-def trim_video(video_path: str, output_path: str, start_time: int, end_time: int):
+def trim_video(video_path: str, output_name: str, start_time: int, end_time: int):
     """
     This function trims a video clip from the given start time to the end time.
 
     Args:
     video_path (str): Path to the input video file.
-    output_path (str): Path to save the output trimmed video file.
+    output_name (str): Path to save the output trimmed video file.
     start_time (int): The start time of the clip in seconds.
     end_time (int): The end time of the clip in seconds.
 
     Returns:
     None
     """
     from moviepy.editor import VideoFileClip
@@ -62,19 +62,19 @@
     # Load the video
     clip = VideoFileClip(video_path)
 
     # Trim the video
     trimmed_clip = clip.subclip(start_time, end_time)
 
     # Write the result to a file (without processing audio)
-    trimmed_clip.write_videofile(output_path, audio=True)
+    trimmed_clip.write_videofile(output_name, audio=True)
 
     print("Video trimmed successfully!")
 
-    return output_path
+    return output_name
 
 
 def frames_to_video(folder_path, output_folder, output_video_name="output.avi", duration=10):
     """
     This function takes a folder with image files, orders them, and creates a video file from them.
     The video is then saved in the designated output folder.
 
@@ -90,15 +90,15 @@
     import glob
     import os
 
     import cv2
 
     # Get the list of images
     img_array = []
-    for filename in sorted(glob.glob(os.path.join(folder_path, "*.jpg"))):
+    for filename in sorted(glob.glob(os.path.join(folder_path, "*.png"))):
         img = cv2.imread(filename)
         height, width, layers = img.shape
         size = (width, height)
         img_array.append(img)
 
     # Calculate fps based on the desired duration
     fps = len(img_array) / duration
```

### Comparing `custom_diffusion-0.1.0/custom_diffusion.egg-info/PKG-INFO` & `custom_diffusion-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
-Name: custom-diffusion
-Version: 0.1.0
+Name: custom_diffusion
+Version: 0.1.1
 Summary: Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
 Home-page: https://github.com/kadirnar/Custom-Diffusion
 Author: kadirnar
 License: Apache License 2.0
 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion models,controlnet,stable diffusion
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -40,15 +39,15 @@
 ### Installation
 ```bash
 pip install custom_diffusion
 ```
 
 ### Usage
 ```python
-from custom_diffusion.pipelines import StableDiffusionControlNetGenerator
+from custom_diffusion.pipelines.controlnet_pipeline import StableDiffusionControlNetGenerator
 
 
 generator = StableDiffusionControlNetGenerator()
 
 generated_image = generator.generate_image(
      stable_model_path="runwayml/stable-diffusion-v1-5"
      controlnet_model_path="lllyasviel/control_v11p_sd15_canny",
@@ -65,9 +64,7 @@
      controlnet_conditioning_scale=1.0,
      generator_seed=0,
      preprocess_type="Canny",
      resize_type="center_crop_and_resize",
      crop_size=512,
 )
 ```
-
-
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1 Name: custom-diffusion Version: 0.1.0 Summary: Custom
+Metadata-Version: 2.1 Name: custom_diffusion Version: 0.1.1 Summary: Custom
 Diffusion: Creating Video from Frame Using Multiple Diffusion Home-page: https:
 //github.com/kadirnar/Custom-Diffusion Author: kadirnar License: Apache License
 2.0 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion
-models,controlnet,stable diffusion Platform: UNKNOWN Classifier: Development
-Status :: 5 - Production/Stable Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Science/Research Classifier: Programming Language :: Python :: 3 Classifier:
+models,controlnet,stable diffusion Classifier: Development Status :: 5 -
+Production/Stable Classifier: Operating System :: OS Independent Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Science/
+Research Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Requires-Python: >=3.6 Description-
 Content-Type: text/markdown Provides-Extra: dev License-File: LICENSE
   ***** Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
                                      *****
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 ### Installation ```bash pip install custom_diffusion ``` ### Usage ```python
-from custom_diffusion.pipelines import StableDiffusionControlNetGenerator
-generator = StableDiffusionControlNetGenerator() generated_image =
-generator.generate_image( stable_model_path="runwayml/stable-diffusion-v1-5"
+from custom_diffusion.pipelines.controlnet_pipeline import
+StableDiffusionControlNetGenerator generator =
+StableDiffusionControlNetGenerator() generated_image = generator.generate_image
+( stable_model_path="runwayml/stable-diffusion-v1-5"
 controlnet_model_path="lllyasviel/control_v11p_sd15_canny",
 scheduler_name="DDIM", image_path="test.png", prompt="Anime boy",
 negative_prompt="bad", height=512, width=512, guess_mode=False,
 num_images_per_prompt=1, num_inference_steps=20, guidance_scale=7.0,
 controlnet_conditioning_scale=1.0, generator_seed=0, preprocess_type="Canny",
 resize_type="center_crop_and_resize", crop_size=512, ) ```
```

### Comparing `custom_diffusion-0.1.0/custom_diffusion.egg-info/SOURCES.txt` & `custom_diffusion-0.1.1/custom_diffusion.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -9,12 +9,15 @@
 custom_diffusion/demo.py
 custom_diffusion/preprocces.py
 custom_diffusion.egg-info/PKG-INFO
 custom_diffusion.egg-info/SOURCES.txt
 custom_diffusion.egg-info/dependency_links.txt
 custom_diffusion.egg-info/requires.txt
 custom_diffusion.egg-info/top_level.txt
+custom_diffusion/pipelines/__init__.py
+custom_diffusion/pipelines/controlnet_inpaint_pipeline.py
+custom_diffusion/pipelines/controlnet_pipeline.py
 custom_diffusion/utils/__init__.py
 custom_diffusion/utils/data_utils.py
 custom_diffusion/utils/downloads.py
 custom_diffusion/utils/scheduler_utils.py
 custom_diffusion/utils/video_utils.py
```

### Comparing `custom_diffusion-0.1.0/setup.py` & `custom_diffusion-0.1.1/setup.py`

 * *Files identical despite different names*

