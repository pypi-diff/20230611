# Comparing `tmp/yle-dl-20221231.tar.gz` & `tmp/yle_dl-20230611.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yle-dl-20221231.tar", last modified: Sat Dec 31 09:37:45 2022, max compression
+gzip compressed data, was "yle_dl-20230611.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `yle-dl-20221231.tar` & `yle_dl-20230611.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     6669 2022-12-06 07:51:33.323869 yle-dl-20221231/README.md
--rw-r--r--   0        0        0     1401 2022-11-11 18:00:12.915686 yle-dl-20221231/pyproject.toml
--rw-r--r--   0        0        0     1222 2022-11-11 18:00:12.915686 yle-dl-20221231/yledl/__init__.py
--rw-r--r--   0        0        0      782 2022-11-11 18:00:12.915686 yle-dl-20221231/yledl/__main__.py
--rw-r--r--   0        0        0    20666 2022-11-11 18:00:12.915686 yle-dl-20221231/yledl/backends.py
--rw-r--r--   0        0        0    16727 2022-12-17 18:32:23.934161 yle-dl-20221231/yledl/downloader.py
--rw-r--r--   0        0        0     1161 2022-11-11 18:00:12.915686 yle-dl-20221231/yledl/errors.py
--rw-r--r--   0        0        0      744 2022-11-11 18:00:12.915686 yle-dl-20221231/yledl/exitcodes.py
--rw-r--r--   0        0        0    39694 2022-12-31 09:14:12.855357 yle-dl-20221231/yledl/extractors.py
--rw-r--r--   0        0        0     4013 2022-11-11 18:00:12.915686 yle-dl-20221231/yledl/ffprobe.py
--rw-r--r--   0        0        0     1684 2022-11-11 18:00:12.915686 yle-dl-20221231/yledl/geolocation.py
--rw-r--r--   0        0        0     5417 2022-11-11 18:00:12.915686 yle-dl-20221231/yledl/http.py
--rw-r--r--   0        0        0     6884 2022-11-11 18:00:12.919686 yle-dl-20221231/yledl/io.py
--rw-r--r--   0        0        0     9871 2022-11-11 18:00:12.919686 yle-dl-20221231/yledl/kaltura.py
--rw-r--r--   0        0        0     2070 2022-11-11 18:00:12.919686 yle-dl-20221231/yledl/localization.py
--rw-r--r--   0        0        0     1123 2022-11-11 18:00:12.919686 yle-dl-20221231/yledl/streamfilters.py
--rw-r--r--   0        0        0     1450 2022-11-11 18:00:12.919686 yle-dl-20221231/yledl/streamflavor.py
--rw-r--r--   0        0        0     2734 2022-11-11 18:00:12.919686 yle-dl-20221231/yledl/streamprobe.py
--rw-r--r--   0        0        0      860 2022-11-11 18:00:12.919686 yle-dl-20221231/yledl/subtitles.py
--rw-r--r--   0        0        0     2055 2022-11-11 18:00:12.919686 yle-dl-20221231/yledl/timestamp.py
--rw-r--r--   0        0        0     6488 2022-11-11 18:00:12.919686 yle-dl-20221231/yledl/titleformatter.py
--rw-r--r--   0        0        0     1704 2022-11-11 18:00:12.919686 yle-dl-20221231/yledl/utils.py
--rw-r--r--   0        0        0      722 2022-12-31 09:35:15.843629 yle-dl-20221231/yledl/version.py
--rw-r--r--   0        0        0    20428 2022-11-11 18:00:12.919686 yle-dl-20221231/yledl/yledl.py
--rw-r--r--   0        0        0     7948 1970-01-01 00:00:00.000000 yle-dl-20221231/PKG-INFO
+-rw-r--r--   0        0        0     6669 2023-06-11 14:32:15.808487 yle_dl-20230611/README.md
+-rw-r--r--   0        0        0     1401 2023-01-07 19:04:39.632454 yle_dl-20230611/pyproject.toml
+-rw-r--r--   0        0        0     1222 2023-06-11 14:30:54.763328 yle_dl-20230611/yledl/__init__.py
+-rw-r--r--   0        0        0      782 2023-06-11 14:30:54.763328 yle_dl-20230611/yledl/__main__.py
+-rw-r--r--   0        0        0    20666 2022-12-31 09:54:58.828317 yle_dl-20230611/yledl/backends.py
+-rw-r--r--   0        0        0    16727 2022-12-31 09:54:58.828317 yle_dl-20230611/yledl/downloader.py
+-rw-r--r--   0        0        0     1161 2023-06-11 14:30:54.763328 yle_dl-20230611/yledl/errors.py
+-rw-r--r--   0        0        0      744 2022-12-31 09:54:58.828317 yle_dl-20230611/yledl/exitcodes.py
+-rw-r--r--   0        0        0    39895 2023-06-11 14:34:19.886327 yle_dl-20230611/yledl/extractors.py
+-rw-r--r--   0        0        0     4013 2023-06-11 14:30:54.763328 yle_dl-20230611/yledl/ffprobe.py
+-rw-r--r--   0        0        0     1684 2023-06-11 14:30:54.763328 yle_dl-20230611/yledl/geolocation.py
+-rw-r--r--   0        0        0     5417 2023-06-11 14:30:54.767328 yle_dl-20230611/yledl/http.py
+-rw-r--r--   0        0        0     6884 2022-12-31 09:54:58.828317 yle_dl-20230611/yledl/io.py
+-rw-r--r--   0        0        0     9871 2023-06-11 14:30:54.767328 yle_dl-20230611/yledl/kaltura.py
+-rw-r--r--   0        0        0     2070 2022-12-31 09:54:58.828317 yle_dl-20230611/yledl/localization.py
+-rw-r--r--   0        0        0     1123 2022-12-31 09:54:58.828317 yle_dl-20230611/yledl/streamfilters.py
+-rw-r--r--   0        0        0     1450 2022-12-31 09:54:58.828317 yle_dl-20230611/yledl/streamflavor.py
+-rw-r--r--   0        0        0     2734 2022-12-31 09:54:58.828317 yle_dl-20230611/yledl/streamprobe.py
+-rw-r--r--   0        0        0      860 2023-06-11 14:30:54.767328 yle_dl-20230611/yledl/subtitles.py
+-rw-r--r--   0        0        0     2055 2023-06-11 14:30:54.767328 yle_dl-20230611/yledl/timestamp.py
+-rw-r--r--   0        0        0     6488 2023-06-11 14:30:54.767328 yle_dl-20230611/yledl/titleformatter.py
+-rw-r--r--   0        0        0     1704 2023-06-11 14:30:54.767328 yle_dl-20230611/yledl/utils.py
+-rw-r--r--   0        0        0      722 2023-06-11 14:35:47.023659 yle_dl-20230611/yledl/version.py
+-rw-r--r--   0        0        0    20428 2023-06-11 14:31:14.911613 yle_dl-20230611/yledl/yledl.py
+-rw-r--r--   0        0        0     7948 1970-01-01 00:00:00.000000 yle_dl-20230611/PKG-INFO
```

### Comparing `yle-dl-20221231/README.md` & `yle_dl-20230611/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Download videos from Yle servers
 
 [![Build status](https://circleci.com/gh/aajanki/yle-dl.svg?style=shield)](https://app.circleci.com/pipelines/github/aajanki/yle-dl)
 [![PyPI version](https://badge.fury.io/py/yle-dl.svg)](https://badge.fury.io/py/yle-dl)
 
-Copyright (C) 2010-2022 Antti Ajanki, antti.ajanki@iki.fi
+Copyright (C) 2010-2023 Antti Ajanki, antti.ajanki@iki.fi
 
 License: GPL v3 or later
 
 Homepage: https://aajanki.github.io/yle-dl/index-en.html
 
 Source code: https://github.com/aajanki/yle-dl
```

### Comparing `yle-dl-20221231/pyproject.toml` & `yle_dl-20230611/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/__init__.py` & `yle_dl-20230611/yledl/__init__.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/__main__.py` & `yle_dl-20230611/yledl/__main__.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/backends.py` & `yle_dl-20230611/yledl/backends.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/downloader.py` & `yle_dl-20230611/yledl/downloader.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/errors.py` & `yle_dl-20230611/yledl/errors.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/exitcodes.py` & `yle_dl-20230611/yledl/exitcodes.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/extractors.py` & `yle_dl-20230611/yledl/extractors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of yle-dl.
 #
-# Copyright 2010-2022 Antti Ajanki and others
+# Copyright 2010-2023 Antti Ajanki and others
 #
 # Yle-dl is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # Yle-dl is distributed in the hope that it will be useful, but
@@ -774,29 +774,33 @@
             flavors = self.hls_probe_flavors(hls_manifest_url, is_live, ffprobe)
             error = [FailedFlavor('Manifest URL is missing')]
             return flavors or error
         elif self.is_html5_media(media_id):
             logger.debug('Detected an HTML5 media')
             return (kaltura_flavors or
                     self.hls_probe_flavors(hls_manifest_url, False, ffprobe))
-        elif self.is_media_67(media_id):
+        elif self.is_media_67(media_id) or self.is_media_78(media_id):
             return []
         else:
             return [FailedFlavor('Unknown stream flavor')]
 
     def is_html5_media(self, media_id):
         return media_id and media_id.startswith('29-')
 
     def is_full_hd_media(self, media_id):
         return media_id and media_id.startswith('55-')
 
     def is_media_67(self, media_id):
         # A new hosting alternative (June 2021)? Hosted on yleawsmpodamdipv4.akamaized.net
         return media_id and media_id.startswith('67-')
 
+    def is_media_78(self, media_id):
+        # Podcast streams (Spring 2023). Prefer download_url, no extra flavors here.
+        return media_id and media_id.startswith('78-')
+
     def is_live_media(self, media_id):
         return media_id and media_id.startswith('10-')
 
     def kaltura_entry_id(self, mediaid):
         return mediaid.split('-', 1)[-1]
 
     def hls_flavors(self, hls_manifest_url, media_type):
@@ -1034,17 +1038,17 @@
             if len(state_div_nodes) > 0:
                 state = json.loads(state_div_nodes[0].attrib.get('data-state'))
 
         if state is None:
             return []
 
         data_ids = []
-        article = state.get('article', {}).get('article', {})
+        article = state.get('pageData', {}).get('article', {})
         if article.get('mainMedia') is not None:
-            medias = article.get('mainMedia', [])
+            medias = article['mainMedia']
             data_ids = [m.get('id') for m in medias if m.get('type') == 'VideoBlock']
         else:
             headline_video_id = article.get('headline', {}).get('video', {}).get('id')
             if headline_video_id:
                 data_ids = [headline_video_id]
 
         content = article.get('content', [])
```

### Comparing `yle-dl-20221231/yledl/ffprobe.py` & `yle_dl-20230611/yledl/ffprobe.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/geolocation.py` & `yle_dl-20230611/yledl/geolocation.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/http.py` & `yle_dl-20230611/yledl/http.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/io.py` & `yle_dl-20230611/yledl/io.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/kaltura.py` & `yle_dl-20230611/yledl/kaltura.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/localization.py` & `yle_dl-20230611/yledl/localization.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/streamfilters.py` & `yle_dl-20230611/yledl/streamfilters.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/streamflavor.py` & `yle_dl-20230611/yledl/streamflavor.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/streamprobe.py` & `yle_dl-20230611/yledl/streamprobe.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/subtitles.py` & `yle_dl-20230611/yledl/subtitles.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/timestamp.py` & `yle_dl-20230611/yledl/timestamp.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/titleformatter.py` & `yle_dl-20230611/yledl/titleformatter.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/utils.py` & `yle_dl-20230611/yledl/utils.py`

 * *Files identical despite different names*

### Comparing `yle-dl-20221231/yledl/version.py` & `yle_dl-20230611/yledl/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # This file is part of yle-dl.
 #
-# Copyright 2010-2022 Antti Ajanki and others
+# Copyright 2010-2023 Antti Ajanki and others
 #
 # Yle-dl is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # Yle-dl is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with yle-dl. If not, see <https://www.gnu.org/licenses/>.
 
-__version__ = '20221231'
+__version__ = '20230611'
```

### Comparing `yle-dl-20221231/yledl/yledl.py` & `yle_dl-20230611/yledl/yledl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 """
 yle-dl - download videos from Yle servers
 
-Copyright (C) 2010-2022 Antti Ajanki <antti.ajanki@iki.fi>
+Copyright (C) 2010-2023 Antti Ajanki <antti.ajanki@iki.fi>
 
 This script downloads video and audio streams from Yle Areena
 (https://areena.yle.fi) and Elävä Arkisto
 (http://yle.fi/aihe/elava-arkisto).
 """
 
 # This program is free software: you can redistribute it and/or modify
@@ -80,15 +80,15 @@
             if message:
                 if file is None:
                     file = sys.stderr
                 print_enc(message, file, False)
 
     description = (
         f'yle-dl {__version__}: Download media files from Yle Areena and Elävä Arkisto\n'
-        'Copyright (C) 2009-2022 Antti Ajanki <antti.ajanki@iki.fi>, license: GPLv3\n'
+        'Copyright (C) 2009-2023 Antti Ajanki <antti.ajanki@iki.fi>, license: GPLv3\n'
     )
 
     parser = ArgumentParserEncoded(
         default_config_files=['~/.yledl.conf'],
         description=description,
         formatter_class=configargparse.RawDescriptionHelpFormatter)
     parser.add_argument('-V', '--verbose',
```

### Comparing `yle-dl-20221231/PKG-INFO` & `yle_dl-20230611/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yle-dl
-Version: 20221231
+Version: 20230611
 Summary: Download videos from Yle servers
 Author-email: Antti Ajanki <antti.ajanki@iki.fi>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -31,15 +31,15 @@
 Provides-Extra: test
 
 Download videos from Yle servers
 
 [![Build status](https://circleci.com/gh/aajanki/yle-dl.svg?style=shield)](https://app.circleci.com/pipelines/github/aajanki/yle-dl)
 [![PyPI version](https://badge.fury.io/py/yle-dl.svg)](https://badge.fury.io/py/yle-dl)
 
-Copyright (C) 2010-2022 Antti Ajanki, antti.ajanki@iki.fi
+Copyright (C) 2010-2023 Antti Ajanki, antti.ajanki@iki.fi
 
 License: GPL v3 or later
 
 Homepage: https://aajanki.github.io/yle-dl/index-en.html
 
 Source code: https://github.com/aajanki/yle-dl
```

