# Comparing `tmp/joonmyung-1.4.5.tar.gz` & `tmp/joonmyung-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joonmyung-1.4.5.tar", last modified: Fri May 26 14:18:52 2023, max compression
+gzip compressed data, was "dist/joonmyung-1.4.6.tar", last modified: Sun Jun 11 04:46:05 2023, max compression
```

## Comparing `joonmyung-1.4.5.tar` & `joonmyung-1.4.6.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-26 14:18:52.750523 joonmyung-1.4.5/
--rw-r--r--   0 joonmyung   (501) staff       (20)        0 2023-02-22 17:22:56.000000 joonmyung-1.4.5/LICENSE.txt
--rw-r--r--   0 joonmyung   (501) staff       (20)      256 2023-05-26 14:18:52.750397 joonmyung-1.4.5/PKG-INFO
--rw-r--r--   0 joonmyung   (501) staff       (20)     1138 2023-04-06 18:15:10.000000 joonmyung-1.4.5/README.md
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-26 14:18:52.747009 joonmyung-1.4.5/joonmyung/
--rw-r--r--   0 joonmyung   (501) staff       (20)       15 2023-02-22 17:22:56.000000 joonmyung-1.4.5/joonmyung/__init__.py
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-26 14:18:52.748874 joonmyung-1.4.5/joonmyung/analysis/
--rw-r--r--   0 joonmyung   (501) staff       (20)      110 2023-03-01 06:50:39.000000 joonmyung-1.4.5/joonmyung/analysis/__init__.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     6956 2023-05-11 09:50:49.000000 joonmyung-1.4.5/joonmyung/analysis/analysis.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     4675 2023-05-21 08:24:43.000000 joonmyung-1.4.5/joonmyung/analysis/dataset.py
--rw-r--r--   0 joonmyung   (501) staff       (20)        0 2023-03-01 06:34:05.000000 joonmyung-1.4.5/joonmyung/analysis/hook.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     1192 2023-02-25 11:17:51.000000 joonmyung-1.4.5/joonmyung/analysis/metric.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     1784 2023-05-21 08:00:39.000000 joonmyung-1.4.5/joonmyung/analysis/model.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     6700 2023-04-03 12:26:27.000000 joonmyung-1.4.5/joonmyung/app.py
--rw-r--r--   0 joonmyung   (501) staff       (20)      695 2023-02-24 17:07:52.000000 joonmyung-1.4.5/joonmyung/data.py
--rw-r--r--   0 joonmyung   (501) staff       (20)    13698 2023-05-21 08:03:13.000000 joonmyung-1.4.5/joonmyung/draw.py
--rw-r--r--   0 joonmyung   (501) staff       (20)       29 2023-04-03 12:26:27.000000 joonmyung-1.4.5/joonmyung/dummy.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     2755 2023-02-22 17:22:56.000000 joonmyung-1.4.5/joonmyung/file.py
--rw-r--r--   0 joonmyung   (501) staff       (20)      920 2023-02-22 17:22:56.000000 joonmyung-1.4.5/joonmyung/gradcam.py
--rw-r--r--   0 joonmyung   (501) staff       (20)    10232 2023-05-21 08:10:17.000000 joonmyung-1.4.5/joonmyung/log.py
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-26 14:18:52.750093 joonmyung-1.4.5/joonmyung/meta_data/
--rw-r--r--   0 joonmyung   (501) staff       (20)       41 2023-03-01 06:51:46.000000 joonmyung-1.4.5/joonmyung/meta_data/__init__.py
--rw-r--r--   0 joonmyung   (501) staff       (20)    45491 2023-02-22 17:22:56.000000 joonmyung-1.4.5/joonmyung/meta_data/label.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     2182 2023-05-21 09:42:01.000000 joonmyung-1.4.5/joonmyung/meta_data/utils.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     4031 2023-05-26 13:55:28.000000 joonmyung-1.4.5/joonmyung/metric.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     3214 2023-05-11 09:51:38.000000 joonmyung-1.4.5/joonmyung/script.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     1487 2023-03-01 13:25:20.000000 joonmyung-1.4.5/joonmyung/status.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     3949 2023-04-06 17:51:01.000000 joonmyung-1.4.5/joonmyung/utils.py
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-26 14:18:52.747736 joonmyung-1.4.5/joonmyung.egg-info/
--rw-r--r--   0 joonmyung   (501) staff       (20)      256 2023-05-26 14:18:52.000000 joonmyung-1.4.5/joonmyung.egg-info/PKG-INFO
--rw-r--r--   0 joonmyung   (501) staff       (20)      689 2023-05-26 14:18:52.000000 joonmyung-1.4.5/joonmyung.egg-info/SOURCES.txt
--rw-r--r--   0 joonmyung   (501) staff       (20)        1 2023-05-26 14:18:52.000000 joonmyung-1.4.5/joonmyung.egg-info/dependency_links.txt
--rw-r--r--   0 joonmyung   (501) staff       (20)        1 2023-05-26 13:56:46.000000 joonmyung-1.4.5/joonmyung.egg-info/not-zip-safe
--rw-r--r--   0 joonmyung   (501) staff       (20)       10 2023-05-26 14:18:52.000000 joonmyung-1.4.5/joonmyung.egg-info/top_level.txt
--rw-r--r--   0 joonmyung   (501) staff       (20)       38 2023-05-26 14:18:52.750572 joonmyung-1.4.5/setup.cfg
--rw-r--r--   0 joonmyung   (501) staff       (20)      781 2023-05-26 13:56:19.000000 joonmyung-1.4.5/setup.py
+drwxrwxr-x   0 joonmyung  (1002) joonmyung  (1003)        0 2023-06-11 04:46:05.518205 joonmyung-1.4.6/
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)        0 2023-02-22 17:22:56.000000 joonmyung-1.4.6/LICENSE.txt
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)      256 2023-06-11 04:46:05.518205 joonmyung-1.4.6/PKG-INFO
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     1138 2023-04-06 18:15:10.000000 joonmyung-1.4.6/README.md
+drwxrwxr-x   0 joonmyung  (1002) joonmyung  (1003)        0 2023-06-11 04:46:05.518205 joonmyung-1.4.6/joonmyung/
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)       15 2023-02-22 17:22:56.000000 joonmyung-1.4.6/joonmyung/__init__.py
+drwxrwxr-x   0 joonmyung  (1002) joonmyung  (1003)        0 2023-06-11 04:46:05.518205 joonmyung-1.4.6/joonmyung/analysis/
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)      110 2023-03-01 06:50:39.000000 joonmyung-1.4.6/joonmyung/analysis/__init__.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     6956 2023-05-11 09:50:49.000000 joonmyung-1.4.6/joonmyung/analysis/analysis.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     4984 2023-05-21 08:17:20.000000 joonmyung-1.4.6/joonmyung/analysis/benchmark.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     4675 2023-05-21 08:24:43.000000 joonmyung-1.4.6/joonmyung/analysis/dataset.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)        0 2023-03-01 06:34:05.000000 joonmyung-1.4.6/joonmyung/analysis/hook.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     1217 2023-06-06 06:13:54.000000 joonmyung-1.4.6/joonmyung/analysis/metric.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     1999 2023-06-06 06:28:53.000000 joonmyung-1.4.6/joonmyung/analysis/model.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)      424 2023-06-06 06:36:54.000000 joonmyung-1.4.6/joonmyung/analysis/utils.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     6700 2023-04-03 12:26:27.000000 joonmyung-1.4.6/joonmyung/app.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)      695 2023-02-24 17:07:52.000000 joonmyung-1.4.6/joonmyung/data.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)    13698 2023-05-21 08:03:13.000000 joonmyung-1.4.6/joonmyung/draw.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)       29 2023-04-03 12:26:27.000000 joonmyung-1.4.6/joonmyung/dummy.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     2755 2023-02-22 17:22:56.000000 joonmyung-1.4.6/joonmyung/file.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)      920 2023-02-22 17:22:56.000000 joonmyung-1.4.6/joonmyung/gradcam.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)    10232 2023-05-21 08:10:17.000000 joonmyung-1.4.6/joonmyung/log.py
+drwxrwxr-x   0 joonmyung  (1002) joonmyung  (1003)        0 2023-06-11 04:46:05.518205 joonmyung-1.4.6/joonmyung/meta_data/
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)       41 2023-03-01 06:51:46.000000 joonmyung-1.4.6/joonmyung/meta_data/__init__.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)    45491 2023-02-22 17:22:56.000000 joonmyung-1.4.6/joonmyung/meta_data/label.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     2157 2023-06-11 04:39:41.000000 joonmyung-1.4.6/joonmyung/meta_data/utils.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     4031 2023-05-26 13:55:28.000000 joonmyung-1.4.6/joonmyung/metric.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     3214 2023-05-11 09:51:38.000000 joonmyung-1.4.6/joonmyung/script.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     1487 2023-03-01 13:25:20.000000 joonmyung-1.4.6/joonmyung/status.py
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)     3948 2023-06-06 06:13:54.000000 joonmyung-1.4.6/joonmyung/utils.py
+drwxrwxr-x   0 joonmyung  (1002) joonmyung  (1003)        0 2023-06-11 04:46:05.518205 joonmyung-1.4.6/joonmyung.egg-info/
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)      256 2023-06-11 04:46:05.000000 joonmyung-1.4.6/joonmyung.egg-info/PKG-INFO
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)      749 2023-06-11 04:46:05.000000 joonmyung-1.4.6/joonmyung.egg-info/SOURCES.txt
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)        1 2023-06-11 04:46:05.000000 joonmyung-1.4.6/joonmyung.egg-info/dependency_links.txt
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)        1 2023-05-26 13:56:46.000000 joonmyung-1.4.6/joonmyung.egg-info/not-zip-safe
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)       10 2023-06-11 04:46:05.000000 joonmyung-1.4.6/joonmyung.egg-info/top_level.txt
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)       38 2023-06-11 04:46:05.518205 joonmyung-1.4.6/setup.cfg
+-rw-rw-r--   0 joonmyung  (1002) joonmyung  (1003)      782 2023-06-11 04:43:38.000000 joonmyung-1.4.6/setup.py
```

### Comparing `joonmyung-1.4.5/README.md` & `joonmyung-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.5/joonmyung/analysis/analysis.py` & `joonmyung-1.4.6/joonmyung/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.5/joonmyung/analysis/dataset.py` & `joonmyung-1.4.6/joonmyung/analysis/dataset.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.5/joonmyung/analysis/metric.py` & `joonmyung-1.4.6/joonmyung/analysis/metric.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import torch
 
-from joonmyung.metric import MetricLogger, accuracy
+from joonmyung.log import MetricLogger
+from joonmyung.metric import accuracy
 
 
 @torch.no_grad()
 def evaluate(data_loader, model, device="cuda"):
     criterion = torch.nn.CrossEntropyLoss()
 
     metric_logger = MetricLogger(delimiter="  ")
```

### Comparing `joonmyung-1.4.5/joonmyung/analysis/model.py` & `joonmyung-1.4.6/joonmyung/analysis/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from collections import OrderedDict
+
 from joonmyung.utils import isDir
 from timm import create_model
 import torch
 import os
 
 class JModel():
     def __init__(self, num_classes = None, root_path= None,
@@ -12,20 +14,26 @@
         # Other
         if root_path:
             self.model_path = os.path.join(root_path, "checkpoint_{}.pth")
         if p and root_path:
             print("file list : ", sorted(os.listdir(root_path), reverse=True))
         self.device = device
 
-    def getModel(self, epoch=0, model_number=0, model_name = "deit_tiny", **kwargs):
+    def load_state_dict(self, model, state_dict):
+        state_dict = OrderedDict((k.replace("module.", ""), v) for k, v in state_dict.items())
+        model.load_state_dict(state_dict)
+
+
+    def getModel(self, model_number=0, model_name = "deit_tiny", **kwargs):
         model, args = None, None
         if model_number == 0:
             model = create_model(model_name, pretrained=True, num_classes=self.num_classes, in_chans=3, global_pool=None, scriptable=False).to(self.device)
         elif model_number == 1:
             model = torch.hub.load('facebookresearch/deit:main', model_name, pretrained=True).to(self.device)
+
         # elif model_number == 2:
         #     model_path = self.model_path.format(str(epoch))
         #     if not isDir(model_path): raise FileExistsError
         #
         #     checkpoint = torch.load(model_path, map_location='cpu')
         #     args = checkpoint['args']
         #     if "token_merging" in kwargs.keys():
@@ -37,10 +45,8 @@
         #         if "total_ops" not in n and "total_params" not in n:
         #             state_dict.append((n, p))
         #     state_dict = dict(state_dict)
         #     model.load_state_dict(state_dict)
 
         model.eval()
 
-        return model, args
-
-
+        return model, args
```

### Comparing `joonmyung-1.4.5/joonmyung/app.py` & `joonmyung-1.4.6/joonmyung/app.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.5/joonmyung/data.py` & `joonmyung-1.4.6/joonmyung/data.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.5/joonmyung/draw.py` & `joonmyung-1.4.6/joonmyung/draw.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.5/joonmyung/file.py` & `joonmyung-1.4.6/joonmyung/file.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.5/joonmyung/gradcam.py` & `joonmyung-1.4.6/joonmyung/gradcam.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.5/joonmyung/log.py` & `joonmyung-1.4.6/joonmyung/log.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.5/joonmyung/meta_data/label.py` & `joonmyung-1.4.6/joonmyung/meta_data/label.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.5/joonmyung/meta_data/utils.py` & `joonmyung-1.4.6/joonmyung/meta_data/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 
 
 
 def data2path(dataset, server = "",
               conference="", wandb_version="", wandb_name="",
               kisti_id=""):
 
-    # server = server if server else
     hostname = socket.gethostname()
     server = server if server is not "" \
-                else server if "mlv" in server \
+                else hostname if "mlv" in hostname \
                     else "kakao" if "dakao" in hostname \
                         else "kisti"
 
     if "kakao" in server:
         data_path = "/data/opensets"
         output_dir = "/data/project/rw/joonmyung/conference"
     elif "mlv" in server:
@@ -31,15 +30,15 @@
     else:
         raise ValueError
 
     if dataset in ["imagenet", "IMNET"]:
         data_path = os.path.join(data_path, "imagenet") if "kakao" not in server else os.path.join(data_path, "imagenet-pytorch")
     output_dir = os.path.join(output_dir, conference, wandb_version, wandb_name)
 
-    return data_path, output_dir
+    return data_path, output_dir, server
 
 def get_label(key, d_name ="imagenet"):
     d_name = d_name.lower()
     if d_name in ["imagenet", "IMNET"] :
         return imnet_label[key]
     elif d_name in ["cifar10", "cifar100"]:
         return cifar_label[key]
```

### Comparing `joonmyung-1.4.5/joonmyung/metric.py` & `joonmyung-1.4.6/joonmyung/metric.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.5/joonmyung/script.py` & `joonmyung-1.4.6/joonmyung/script.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.5/joonmyung/status.py` & `joonmyung-1.4.6/joonmyung/status.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.5/joonmyung/utils.py` & `joonmyung-1.4.6/joonmyung/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 def to_tensor(vs):
     if type(vs) == list:
         return [torch.Tensor(v) if type(v) is not torch.Tensor else v for v in vs]
     else:
         return torch.Tensor(vs) if type(vs) is not torch.Tensor else vs
 
-
 def str2list(s):
     v = ast.literal_eval(s.replace(" ", ""))
     if type(v) is not list:
         raise argparse.ArgumentTypeError("Argument \"%s\" is not a list" % (s))
     return v
 
 def str2bool(v):
```

### Comparing `joonmyung-1.4.5/joonmyung.egg-info/SOURCES.txt` & `joonmyung-1.4.6/joonmyung.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 joonmyung.egg-info/PKG-INFO
 joonmyung.egg-info/SOURCES.txt
 joonmyung.egg-info/dependency_links.txt
 joonmyung.egg-info/not-zip-safe
 joonmyung.egg-info/top_level.txt
 joonmyung/analysis/__init__.py
 joonmyung/analysis/analysis.py
+joonmyung/analysis/benchmark.py
 joonmyung/analysis/dataset.py
 joonmyung/analysis/hook.py
 joonmyung/analysis/metric.py
 joonmyung/analysis/model.py
+joonmyung/analysis/utils.py
 joonmyung/meta_data/__init__.py
 joonmyung/meta_data/label.py
 joonmyung/meta_data/utils.py
```

### Comparing `joonmyung-1.4.5/setup.py` & `joonmyung-1.4.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import setuptools
 from setuptools import find_packages
+
 setuptools.setup(
     name="joonmyung",
-    version="1.4.5",
+    version="1.4.6",
     author="JoonMyung Choi",
     author_email="pizard@korea.ac.kr",
     description="JoonMyung's Library",
     url="https://github.com/pizard/JoonMyung.git",
     license="MIT",
     packages=find_packages(exclude=["playground",
                                     "playground.*",
@@ -19,10 +20,10 @@
     ]
 )
 
 # git add .
 # git commit
 # git push
 # Remove *.egg-info
-#
+
 # python setup.py sdist; python -m twine upload dist/*
-# ID:JoonmyungChoi
+# ID:JoonmyungChoi
```

