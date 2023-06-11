# Comparing `tmp/xgo-pythonlib-0.1.3.tar.gz` & `tmp/xgo-pythonlib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgo-pythonlib-0.1.3.tar", last modified: Thu Jun  8 09:12:47 2023, max compression
+gzip compressed data, was "xgo-pythonlib-0.1.4.tar", last modified: Sun Jun 11 07:50:18 2023, max compression
```

## Comparing `xgo-pythonlib-0.1.3.tar` & `xgo-pythonlib-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 09:12:47.886799 xgo-pythonlib-0.1.3/
--rw-rw-rw-   0        0        0     1671 2023-06-08 09:12:47.885799 xgo-pythonlib-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1044 2023-06-07 12:00:47.000000 xgo-pythonlib-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-08 09:12:47.886799 xgo-pythonlib-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     3684 2023-06-08 09:12:43.000000 xgo-pythonlib-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 09:12:47.874799 xgo-pythonlib-0.1.3/xgo_pythonlib.egg-info/
--rw-rw-rw-   0        0        0     1671 2023-06-08 09:12:47.000000 xgo-pythonlib-0.1.3/xgo_pythonlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-06-08 09:12:47.000000 xgo-pythonlib-0.1.3/xgo_pythonlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 09:12:47.000000 xgo-pythonlib-0.1.3/xgo_pythonlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-08 09:12:47.000000 xgo-pythonlib-0.1.3/xgo_pythonlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-08 09:12:47.876799 xgo-pythonlib-0.1.3/xgoedu/
--rw-rw-rw-   0        0        0    33489 2023-06-07 11:54:24.000000 xgo-pythonlib-0.1.3/xgoedu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 09:12:47.878799 xgo-pythonlib-0.1.3/xgolib/
--rw-rw-rw-   0        0        0    26384 2023-06-08 09:11:58.000000 xgo-pythonlib-0.1.3/xgolib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 09:12:47.883800 xgo-pythonlib-0.1.3/xgoscreen/
--rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.1.3/xgoscreen/LCD_2inch.py
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.1.3/xgoscreen/__init__.py
--rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.1.3/xgoscreen/lcdconfig.py
+drwxrwxrwx   0        0        0        0 2023-06-11 07:50:18.975680 xgo-pythonlib-0.1.4/
+-rw-rw-rw-   0        0        0     1733 2023-06-11 07:50:18.974681 xgo-pythonlib-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1106 2023-06-08 09:16:07.000000 xgo-pythonlib-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-11 07:50:18.976679 xgo-pythonlib-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     3684 2023-06-11 07:47:55.000000 xgo-pythonlib-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 07:50:18.957679 xgo-pythonlib-0.1.4/xgo_pythonlib.egg-info/
+-rw-rw-rw-   0        0        0     1733 2023-06-11 07:50:18.000000 xgo-pythonlib-0.1.4/xgo_pythonlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-06-11 07:50:18.000000 xgo-pythonlib-0.1.4/xgo_pythonlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 07:50:18.000000 xgo-pythonlib-0.1.4/xgo_pythonlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-11 07:50:18.000000 xgo-pythonlib-0.1.4/xgo_pythonlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 07:50:18.960678 xgo-pythonlib-0.1.4/xgoedu/
+-rw-rw-rw-   0        0        0    37176 2023-06-11 07:45:57.000000 xgo-pythonlib-0.1.4/xgoedu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 07:50:18.963680 xgo-pythonlib-0.1.4/xgolib/
+-rw-rw-rw-   0        0        0    26384 2023-06-08 09:11:58.000000 xgo-pythonlib-0.1.4/xgolib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 07:50:18.971680 xgo-pythonlib-0.1.4/xgoscreen/
+-rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.1.4/xgoscreen/LCD_2inch.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.1.4/xgoscreen/__init__.py
+-rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.1.4/xgoscreen/lcdconfig.py
```

### Comparing `xgo-pythonlib-0.1.3/PKG-INFO` & `xgo-pythonlib-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.1.3
+Version: 0.1.4
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -26,15 +26,15 @@
 
 [PythonLib-WIKI](https://www.yuque.com/luwudynamics/cn/mxkaodwpo2h5zmvw)
 
 
 
 ## Install instructions 
 
-1 Burn the official 0512 img image 
+1 Burn the official 0608 img image 
 
 2 Copy all files from the "model" directory to `\home\pi\model`
 
 3 Run this command:
 
 ```
 pip install --upgrade xgo-pythonlib
@@ -56,8 +56,15 @@
 ```
 xgolib library example
 ```python
 from xgolib import XGO
 dog = XGO('/dev/ttyAMA0')
 dog.action(1)
 ```
-### Lastest Verion:0.1.2
+### Lastest Verion:0.1.3
+
+### xgolib_version=1.3.0
+
+### xgoedu_version=1.2.1
+
+
+
```

### Comparing `xgo-pythonlib-0.1.3/README.md` & `xgo-pythonlib-0.1.4/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [PythonLib-WIKI](https://www.yuque.com/luwudynamics/cn/mxkaodwpo2h5zmvw)
 
 
 
 ## Install instructions 
 
-1 Burn the official 0512 img image 
+1 Burn the official 0608 img image 
 
 2 Copy all files from the "model" directory to `\home\pi\model`
 
 3 Run this command:
 
 ```
 pip install --upgrade xgo-pythonlib
@@ -38,8 +38,15 @@
 ```
 xgolib library example
 ```python
 from xgolib import XGO
 dog = XGO('/dev/ttyAMA0')
 dog.action(1)
 ```
-### Lastest Verion:0.1.2
+### Lastest Verion:0.1.3
+
+### xgolib_version=1.3.0
+
+### xgoedu_version=1.2.1
+
+
+
```

### Comparing `xgo-pythonlib-0.1.3/setup.py` & `xgo-pythonlib-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'xgo-pythonlib'
 DESCRIPTION = 'PythonLib for XGO2-DOG'
 URL = 'https://github.com/Xgorobot/XGO-PythonLib'
 EMAIL = 'hello@xgorobot.com'
 AUTHOR = 'luwudynamics'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `xgo-pythonlib-0.1.3/xgo_pythonlib.egg-info/PKG-INFO` & `xgo-pythonlib-0.1.4/xgo_pythonlib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.1.3
+Version: 0.1.4
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -26,15 +26,15 @@
 
 [PythonLib-WIKI](https://www.yuque.com/luwudynamics/cn/mxkaodwpo2h5zmvw)
 
 
 
 ## Install instructions 
 
-1 Burn the official 0512 img image 
+1 Burn the official 0608 img image 
 
 2 Copy all files from the "model" directory to `\home\pi\model`
 
 3 Run this command:
 
 ```
 pip install --upgrade xgo-pythonlib
@@ -56,8 +56,15 @@
 ```
 xgolib library example
 ```python
 from xgolib import XGO
 dog = XGO('/dev/ttyAMA0')
 dog.action(1)
 ```
-### Lastest Verion:0.1.2
+### Lastest Verion:0.1.3
+
+### xgolib_version=1.3.0
+
+### xgoedu_version=1.2.1
+
+
+
```

### Comparing `xgo-pythonlib-0.1.3/xgoedu/__init__.py` & `xgo-pythonlib-0.1.4/xgoedu/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,28 @@
 import math
 import os,sys,time
 import spidev as SPI
 import xgoscreen.LCD_2inch as LCD_2inch
 import RPi.GPIO as GPIO
 from PIL import Image,ImageDraw,ImageFont
 import json
-#from xgolib import XGO
+import threading
+# from xgolib import XGO
 # from keras.preprocessing import image
+# import _thread  使用_thread会报错，坑！
 
 
-__versinon__ = '1.2.1'
-__last_modified__ = '2023/6/7'
+__versinon__ = '1.2.2'
+__last_modified__ = '2023/6/11'
 
 GPIO.setwarnings(False)
 GPIO.setmode(GPIO.BCM)
 
+camera_still=False
+
 
 '''
 人脸检测
 '''
 def getFaceBox(net, frame, conf_threshold=0.7):
     frameOpencvDnn = frame.copy()
     frameHeight = frameOpencvDnn.shape[0]
@@ -90,14 +94,15 @@
   elif isinstance(value, str):
     a1 = digit.index(value[1]) * 16 + digit.index(value[2])
     a2 = digit.index(value[3]) * 16 + digit.index(value[4])
     a3 = digit.index(value[5]) * 16 + digit.index(value[6])
     return (a3, a2, a1)
 
 
+
 class XGOEDU():
     def __init__(self):
         self.display = LCD_2inch.LCD_2inch()
         self.display.Init()
         self.display.clear()
         self.splash = Image.new("RGB",(320,240),"black")
         self.display.ShowImage(self.splash)
@@ -110,14 +115,15 @@
         self.cap=None
         self.hand=None
         self.yolo=None
         self.face=None
         self.face_classifier=None
         self.classifier=None
         self.agesexmark=None
+        self.camera_still=False
         GPIO.setup(self.key1,GPIO.IN,GPIO.PUD_UP)
         GPIO.setup(self.key2,GPIO.IN,GPIO.PUD_UP)
         GPIO.setup(self.key3,GPIO.IN,GPIO.PUD_UP)
         GPIO.setup(self.key4,GPIO.IN,GPIO.PUD_UP)
 
     def open_camera(self):
         if self.cap==None:
@@ -195,29 +201,132 @@
             return(not last_state_d)
     #speaker
     '''
     filename 文件名 字符串
     '''
     def xgoSpeaker(self,filename):
         os.system("mplayer"+" "+filename)
+
+    def xgoVedioAudio(self,filename):
+        time.sleep(0.1)  #音画速度同步了 但是时间轴可能不同步 这里调试一下
+        cmd="sudo mplayer "+filename+" -novideo"
+        os.system(cmd)
+
+    def xgoVedio(self,filename):
+        x=threading.Thread(target=self.xgoVedioAudio,args=(filename,))
+        x.start()
+        global counter
+        video=cv2.VideoCapture(filename)
+        fps = video.get(cv2.CAP_PROP_FPS) 
+        print(fps)
+        init_time=time.time()
+        counter=0
+        while True:
+            grabbed, dst = video.read()
+            b,g,r = cv2.split(dst)
+            dst = cv2.merge((r,g,b))
+            imgok = Image.fromarray(dst)
+            self.display.ShowImage(imgok)
+            #强制卡帧数 实测帧数不要超过20贞 否则显示跟不上 但是20贞转换经常有问题 所以建议直接15贞
+            counter += 1
+            ctime=time.time()- init_time
+            if ctime != 0:
+                qtime=counter/fps-ctime
+                #print(qtime)
+                if qtime>0:
+                    time.sleep(qtime)
+            if not grabbed:
+                break
+        
     #audio_record
     '''
     filename 文件名 字符串
     seconds 录制时间S 字符串
     '''
-    def xgoAudioRecord(self,filename="record.wav",seconds=5):
+    def xgoAudioRecord(self,filename="record",seconds=5):
         command1 = "sudo arecord -d"
         command2 = "-f S32_LE -r 16000 -c 1 -t wav"
-        cmd=command1+" "+str(seconds)+" "+command2+" "+filename
+        cmd=command1+" "+str(seconds)+" "+command2+" "+filename+".wav"
         print(cmd)
         os.system(cmd)
+
+    def cameraOn(self,switch):
+        global camera_still
+        if switch:
+            self.open_camera()
+            self.camera_still=True
+            t = threading.Thread(target=self.camera_mode)  
+            t.start() 
+        else:
+            self.camera_still=False
+            time.sleep(0.5)
+            splash = Image.new("RGB",(320,240),"black")
+            self.display.ShowImage(splash)
+
+    def camera_mode(self):
+        self.camera_still=True
+        while 1:
+            success,image = self.cap.read()
+            b,g,r = cv2.split(image)
+            image = cv2.merge((r,g,b))
+            image = cv2.flip(image,1)
+            imgok = Image.fromarray(image)
+            self.display.ShowImage(imgok)
+            if not self.camera_still:
+                break
+
+    def xgoVedioRecord(self,filename="record",seconds=5):
+        self.camera_still=False
+        time.sleep(0.6)
+        self.open_camera()
+        FPS=15
+        fourcc = cv2.VideoWriter_fourcc(*'mp4v')
+        width = int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH))
+        height = int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
+        videoWrite = cv2.VideoWriter(filename+'.mp4', fourcc, FPS, (width,height))
+        starttime=time.time()
+        while 1:
+            print('recording...')
+            ret, image = self.cap.read()
+            if not ret:
+                break
+            videoWrite.write(image)
+            b,g,r = cv2.split(image)
+            image = cv2.merge((r,g,b))
+            image = cv2.flip(image,1)
+            imgok = Image.fromarray(image)
+            self.display.ShowImage(imgok)
+            if time.time()-starttime>seconds:
+                break
+        print('recording done')
+        self.cameraOn(True)
+        videoWrite.release()
+
+    def xgoTakePhoto(self,filename="photo.jpg"):
+        self.camera_still=False
+        time.sleep(0.6)
+        self.open_camera()
+        success,image = self.cap.read()
+        if not success:
+            print("Ignoring empty camera frame")
+        b,g,r = cv2.split(image)
+        image = cv2.merge((r,g,b))
+        image = cv2.flip(image,1)
+        imgok = Image.fromarray(image)
+        self.display.ShowImage(imgok)
+        cv2.imwrite(filename+'.jpg',image)
+        print('photo writed!')
+        time.sleep(0.7)
+        self.cameraOn(True)
+
+
     '''
     开启摄像头  A键拍照 B键录像 C键退出
     '''
-    def cameraOn(self,filename="camera"):
+    def camera(self,filename="camera"):
         font = ImageFont.truetype("/home/pi/model/msyh.ttc",20)
         self.open_camera()
         while True:
             success,image = self.cap.read()
             #cv2.imwrite('/home/pi/xgoEdu/camera/file.jpg',image)
             if not success:
                 print("Ignoring empty camera frame")
```

### Comparing `xgo-pythonlib-0.1.3/xgolib/__init__.py` & `xgo-pythonlib-0.1.4/xgolib/__init__.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.1.3/xgoscreen/LCD_2inch.py` & `xgo-pythonlib-0.1.4/xgoscreen/LCD_2inch.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.1.3/xgoscreen/lcdconfig.py` & `xgo-pythonlib-0.1.4/xgoscreen/lcdconfig.py`

 * *Files identical despite different names*

