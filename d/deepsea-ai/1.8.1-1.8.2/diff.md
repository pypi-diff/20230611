# Comparing `tmp/deepsea_ai-1.8.1.tar.gz` & `tmp/deepsea_ai-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsea_ai-1.8.1.tar", max compression
+gzip compressed data, was "deepsea_ai-1.8.2.tar", max compression
```

## Comparing `deepsea_ai-1.8.1.tar` & `deepsea_ai-1.8.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3173 2022-11-08 03:50:20.735992 deepsea_ai-1.8.1/README.md
--rw-r--r--   0        0        0       44 2022-11-08 03:50:20.735992 deepsea_ai-1.8.1/deepsea_ai/__init__.py
--rw-r--r--   0        0        0    16017 2022-11-08 03:50:20.735992 deepsea_ai-1.8.1/deepsea_ai/__main__.py
--rw-r--r--   0        0        0        0 2022-11-08 03:50:20.735992 deepsea_ai-1.8.1/deepsea_ai/commands/__init__.py
--rw-r--r--   0        0        0     2731 2022-11-08 03:50:20.735992 deepsea_ai-1.8.1/deepsea_ai/commands/bucket.py
--rw-r--r--   0        0        0      815 2022-11-08 03:50:20.735992 deepsea_ai-1.8.1/deepsea_ai/commands/monitor.py
--rw-r--r--   0        0        0     4806 2022-11-08 03:50:20.739992 deepsea_ai-1.8.1/deepsea_ai/commands/process.py
--rw-r--r--   0        0        0    10674 2022-11-08 03:50:20.739992 deepsea_ai-1.8.1/deepsea_ai/commands/train.py
--rw-r--r--   0        0        0     4555 2022-11-08 03:50:20.739992 deepsea_ai-1.8.1/deepsea_ai/commands/upload_tag.py
--rw-r--r--   0        0        0       27 2022-11-08 03:50:20.739992 deepsea_ai-1.8.1/deepsea_ai/config/__init__.py
--rw-r--r--   0        0        0      536 2022-11-08 03:50:20.739992 deepsea_ai-1.8.1/deepsea_ai/config/config.ini
--rw-r--r--   0        0        0     7068 2022-11-08 03:50:20.739992 deepsea_ai-1.8.1/deepsea_ai/config/config.py
--rw-r--r--   0        0        0     6803 2022-11-08 03:50:20.739992 deepsea_ai-1.8.1/deepsea_ai/config/setup.py
--rw-r--r--   0        0        0       26 2022-11-08 03:50:20.739992 deepsea_ai-1.8.1/deepsea_ai/database/__init__.py
--rw-r--r--   0        0        0     1747 2022-11-08 03:50:20.739992 deepsea_ai-1.8.1/deepsea_ai/database/api.py
--rw-r--r--   0        0        0      505 2022-11-08 03:50:20.739992 deepsea_ai-1.8.1/deepsea_ai/database/queries.py
--rw-r--r--   0        0        0       44 2022-11-08 03:50:20.739992 deepsea_ai-1.8.1/deepsea_ai/pipeline/__init__.py
--rw-r--r--   0        0        0    14025 2022-11-08 03:50:20.739992 deepsea_ai-1.8.1/deepsea_ai/pipeline/run_deepsort.py
--rw-r--r--   0        0        0    14488 2022-11-08 03:50:20.739992 deepsea_ai-1.8.1/deepsea_ai/pipeline/run_strongsort.py
--rw-r--r--   0        0        0        0 2022-11-08 03:50:20.739992 deepsea_ai-1.8.1/deepsea_ai/tests/__init__.py
--rw-r--r--   0        0        0      119 2022-11-08 03:50:20.739992 deepsea_ai-1.8.1/deepsea_ai/tests/test_deepsea_ai.py
--rw-r--r--   0        0        0     1284 2022-11-08 03:50:20.739992 deepsea_ai-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     4335 1970-01-01 00:00:00.000000 deepsea_ai-1.8.1/setup.py
--rw-r--r--   0        0        0     4800 1970-01-01 00:00:00.000000 deepsea_ai-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     3173 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/README.md
+-rw-r--r--   0        0        0       44 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/__init__.py
+-rw-r--r--   0        0        0    16007 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/__main__.py
+-rw-r--r--   0        0        0        0 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/commands/__init__.py
+-rw-r--r--   0        0        0     2731 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/commands/bucket.py
+-rw-r--r--   0        0        0      815 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/commands/monitor.py
+-rw-r--r--   0        0        0     4806 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/commands/process.py
+-rw-r--r--   0        0        0    10674 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/commands/train.py
+-rw-r--r--   0        0        0     4555 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/commands/upload_tag.py
+-rw-r--r--   0        0        0       27 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/config/__init__.py
+-rw-r--r--   0        0        0      536 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/config/config.ini
+-rw-r--r--   0        0        0     7109 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/config/config.py
+-rw-r--r--   0        0        0     6803 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/config/setup.py
+-rw-r--r--   0        0        0       26 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/database/__init__.py
+-rw-r--r--   0        0        0     1747 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/database/api.py
+-rw-r--r--   0        0        0      505 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/database/queries.py
+-rw-r--r--   0        0        0       44 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/pipeline/__init__.py
+-rw-r--r--   0        0        0    14025 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/pipeline/run_deepsort.py
+-rw-r--r--   0        0        0    14488 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/pipeline/run_strongsort.py
+-rw-r--r--   0        0        0        0 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/tests/__init__.py
+-rw-r--r--   0        0        0      119 2022-11-09 18:36:03.744985 deepsea_ai-1.8.2/deepsea_ai/tests/test_deepsea_ai.py
+-rw-r--r--   0        0        0     1284 2022-11-09 18:36:03.748985 deepsea_ai-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0     4335 1970-01-01 00:00:00.000000 deepsea_ai-1.8.2/setup.py
+-rw-r--r--   0        0        0     4800 1970-01-01 00:00:00.000000 deepsea_ai-1.8.2/PKG-INFO
```

### Comparing `deepsea_ai-1.8.1/README.md` & `deepsea_ai-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `deepsea_ai-1.8.1/deepsea_ai/__main__.py` & `deepsea_ai-1.8.2/deepsea_ai/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,18 +88,18 @@
               help='Set option to upload local video files to S3 bucket')
 @click.option('--clean', is_flag=True, default=True,
               help='Clean up unused artifact (e.g. video) from s3 after processing')
 @click.option('-i', '--input', type=str, default="/Volumes/M3/mezzanine/DocRicketts/2022/02/1423/",
               help='Path to the folder with video files to upload. These can be either mp4 or mov files that '
                    'ffmpeg '
                    'understands.')
-@click.option('--cluster', type=str, default='lonny33k',
+@click.option('--cluster', type=str, required=True,
               help='Name of the cluster to use to batch process.  This must correspond to an available Elastic '
                    'Container Service cluster.')
-@click.option('--job', type=str, default='lonny33k',
+@click.option('--job', type=str, required=True,
               help='Name of the job, e.g. DiveV4361 benthic outline')
 def batchprocess_command(config, check, upload, clean, cluster, job, input):
     """
      (optional) upload, then batch process in an ECS cluster
     """
     custom_config = cfg.Config(config)
     database = None
```

### Comparing `deepsea_ai-1.8.1/deepsea_ai/commands/bucket.py` & `deepsea_ai-1.8.2/deepsea_ai/commands/bucket.py`

 * *Files identical despite different names*

### Comparing `deepsea_ai-1.8.1/deepsea_ai/commands/monitor.py` & `deepsea_ai-1.8.2/deepsea_ai/commands/monitor.py`

 * *Files identical despite different names*

### Comparing `deepsea_ai-1.8.1/deepsea_ai/commands/process.py` & `deepsea_ai-1.8.2/deepsea_ai/commands/process.py`

 * *Files identical despite different names*

### Comparing `deepsea_ai-1.8.1/deepsea_ai/commands/train.py` & `deepsea_ai-1.8.2/deepsea_ai/commands/train.py`

 * *Files identical despite different names*

### Comparing `deepsea_ai-1.8.1/deepsea_ai/commands/upload_tag.py` & `deepsea_ai-1.8.2/deepsea_ai/commands/upload_tag.py`

 * *Files identical despite different names*

### Comparing `deepsea_ai-1.8.1/deepsea_ai/config/config.ini` & `deepsea_ai-1.8.2/deepsea_ai/config/config.ini`

 * *Files identical despite different names*

### Comparing `deepsea_ai-1.8.1/deepsea_ai/config/config.py` & `deepsea_ai-1.8.2/deepsea_ai/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.parser = ConfigParser()
         if path:
             self.path = path
         else:
             self.path = default_config_ini
 
         if not os.path.isfile(self.path):
-            raise Exception(f'Bad path to {self.path}')
+            raise Exception(f'Bad path to {self.path}. Is your {self.path} missing?')
 
         self.parser.read(self.path)
         lines = open(self.path).readlines()
         if not quiet:
             print(f"===============>Config file {self.path}<=================")
             for l in lines:
                 print(l.strip())
@@ -100,15 +100,15 @@
         Get the user name using IAM; if IAM is not configured, this will default to the root user which may be the case
         for a new AWS account
         :return:
         """
         try:
             sts = boto3.client('sts')
             response = sts.get_caller_identity()
-            user_name = response['UserId'].split(":")[-1]
+            user_name = response['Arn'].split("/")[-1].split("@")[0]
         except ClientError as e:
             # The user_name may be specified in the Access Denied message...
             user_name = "Unknown"
 
         return user_name
```

### Comparing `deepsea_ai-1.8.1/deepsea_ai/config/setup.py` & `deepsea_ai-1.8.2/deepsea_ai/config/setup.py`

 * *Files identical despite different names*

### Comparing `deepsea_ai-1.8.1/deepsea_ai/database/api.py` & `deepsea_ai-1.8.2/deepsea_ai/database/api.py`

 * *Files identical despite different names*

### Comparing `deepsea_ai-1.8.1/deepsea_ai/pipeline/run_deepsort.py` & `deepsea_ai-1.8.2/deepsea_ai/pipeline/run_deepsort.py`

 * *Files identical despite different names*

### Comparing `deepsea_ai-1.8.1/deepsea_ai/pipeline/run_strongsort.py` & `deepsea_ai-1.8.2/deepsea_ai/pipeline/run_strongsort.py`

 * *Files identical despite different names*

### Comparing `deepsea_ai-1.8.1/pyproject.toml` & `deepsea_ai-1.8.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepsea-ai"
-version = "1.8.1"
+version = "1.8.2"
 description = "DeepSeaAI is a Python package to simplify processing deep sea video in AWS from a command line."
 authors = ["Danelle Cline <dcline@mbari.org>", "Duane Edgington <duane@mbari.org>"]
 repository = "https://github.com/mbari-org/deepsea-ai"
 readme = "README.md"
 license = "GPL3"
 classifiers = [
     'Development Status :: 1 - Planning',
```

### Comparing `deepsea_ai-1.8.1/setup.py` & `deepsea_ai-1.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'tqdm>=4.41.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['deepsea-ai = deepsea_ai.__main__:cli']}
 
 setup_kwargs = {
     'name': 'deepsea-ai',
-    'version': '1.8.1',
+    'version': '1.8.2',
     'description': 'DeepSeaAI is a Python package to simplify processing deep sea video in AWS from a command line.',
     'long_description': '[![MBARI](https://www.mbari.org/wp-content/uploads/2014/11/logo-mbari-3b.png)](http://www.mbari.org)\n[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)\n![license-GPL](https://img.shields.io/badge/license-GPL-blue)\n[![Python](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org/downloads/)\n\n**DeepSeaAI** is a Python package to simplify processing deep sea video in [AWS](https://aws.amazon.com) from a command line. \n \nIt includes reasonable defaults that have been optimized for deep sea video. The goal is to simplify running these algorithms in AWS.\n\nDeepSea-AI currently supports:\n\n - *Training [YOLOv5](http://github.com/ultralytics/yolov5) object detection* models\n - *Processing video with [YOLOv5](http://github.com/ultralytics/yolov5) detection and tracking pipelines* using either:\n     * [DeepSort](https://github.com/mikel-brostrom/Yolov5_DeepSort_Pytorch) tracking\n     * [StrongSort](https://github.com/mikel-brostrom/Yolov5_StrongSORT_OSNet) tracking\n\n## Install\n\nSetup [an AWS account](https://aws.amazon.com).\n\nAfter you have setup your AWS account, configure it using the awscli tool, and confirm your AWS Account by listing your s3 buckets\n\n```\npip install awscli\naws configure\naws --version\naws s3 ls \n```\n\nInstall and update using [pip](https://pip.pypa.io/en/stable/getting-started/) in a Python>=3.8.0 environment:\n\n```shell\npip install -U deepsea-ai\n```\n\nSetup your AWS account for use with this module with\n\n```shell\ndeepsea-ai setup\n```\n\n\n\n## Tutorials\n\n* [FathomNet](docs/notebooks/fathomnet_train.ipynb) ✨ Recommended first step to learn more about how to train a YOLOv5 object detection model using freely available FathomNet data\n\nThe best way to use the tutorials is with [Anaconda](https://www.anaconda.com/products/distribution).\n\n### Create the Anaconda environment\n\nThis will create an environment called *deepsea-ai-notebooks* and make that available in your local jupyter notebook as the kernel named *deepsea-ai-notebooks*\n```\nconda env create \nconda activate deepsea-ai-notebooks\npip install ipykernel\npython -m ipykernel install --user --name=deepsea-ai-notebooks\n```\n\n### Launch jupyter\n\n```\ncd docs/notebooks\njupyter notebook\n```\n---\n\n## Commands\n\n* `deepsea-ai setup --help` - Setup the AWS environment. Must run this once before any other commands.\n* [`deepsea-ai train --help` - Train a YOLOv5 model and save the model to a bucket](commands/train.md)\n* [`deepsea-ai process --help` - Process one or more videos and save the results to  a bucket](commands/process.md)\n* [`deepsea-ai ecsprocess --help` - Process one or more videos using the Elastic Container Service and save the results to a bucket](commands/process.md)\n* [`deepsea-ai split --help` - Split your training data. This is required before the train command.](data.md) \n* `deepsea-ai -h` - Print help message and exit.\n \nSource code is available at [github.com/mbari-org/deepsea-ai](https://github.com/mbari-org/deepsea-ai/).\n  \nFor more details, see the [official documentation](http://docs.mbari.org/deepsea-ai/install).',
     'author': 'Danelle Cline',
     'author_email': 'dcline@mbari.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mbari-org/deepsea-ai',
```

### Comparing `deepsea_ai-1.8.1/PKG-INFO` & `deepsea_ai-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsea-ai
-Version: 1.8.1
+Version: 1.8.2
 Summary: DeepSeaAI is a Python package to simplify processing deep sea video in AWS from a command line.
 Home-page: https://github.com/mbari-org/deepsea-ai
 License: GPL3
 Author: Danelle Cline
 Author-email: dcline@mbari.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 1 - Planning
```

