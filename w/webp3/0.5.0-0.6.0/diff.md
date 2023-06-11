# Comparing `tmp/webp3-0.5.0.tar.gz` & `tmp/webp3-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/webp3-0.5.0.tar", last modified: Fri Mar 13 22:23:14 2020, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `webp3-0.5.0.tar` & `webp3-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,22 @@
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2020-03-13 22:23:14.636323 webp3-0.5.0/
--rw-r--r--   0 ntome     (1000) ntome     (1000)      217 2020-03-13 22:22:53.000000 webp3-0.5.0/MANIFEST.in
--rw-r--r--   0 ntome     (1000) ntome     (1000)     1356 2020-03-13 22:23:14.636323 webp3-0.5.0/PKG-INFO
--rw-r--r--   0 ntome     (1000) ntome     (1000)     3792 2020-03-13 22:22:53.000000 webp3-0.5.0/README.rst
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2020-03-13 22:23:14.620322 webp3-0.5.0/apache/
--rw-r--r--   0 ntome     (1000) ntome     (1000)      313 2020-03-13 22:22:53.000000 webp3-0.5.0/apache/install-webp3.rst
--rw-r--r--   0 ntome     (1000) ntome     (1000)      550 2020-03-13 22:22:53.000000 webp3-0.5.0/apache/install-webp3.sh
--rw-r--r--   0 ntome     (1000) ntome     (1000)      352 2020-03-13 22:22:53.000000 webp3-0.5.0/apache/webp3.conf
--rw-r--r--   0 ntome     (1000) ntome     (1000)       38 2020-03-13 22:23:14.636323 webp3-0.5.0/setup.cfg
--rwxr-xr-x   0 ntome     (1000) ntome     (1000)     1710 2020-03-13 22:22:53.000000 webp3-0.5.0/setup.py
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2020-03-13 22:23:14.620322 webp3-0.5.0/webp3/
--rw-r--r--   0 ntome     (1000) ntome     (1000)        0 2020-03-13 22:22:53.000000 webp3-0.5.0/webp3/__init__.py
--rwxr-xr-x   0 ntome     (1000) ntome     (1000)      897 2020-03-13 22:22:53.000000 webp3-0.5.0/webp3/__main__.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)     3452 2020-03-13 22:22:53.000000 webp3-0.5.0/webp3/app.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)      399 2020-03-13 22:22:53.000000 webp3-0.5.0/webp3/conf.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)      181 2020-03-13 22:22:53.000000 webp3-0.5.0/webp3/exceptions.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)     2078 2020-03-13 22:22:53.000000 webp3-0.5.0/webp3/pathutils.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)     2649 2020-03-13 22:22:53.000000 webp3-0.5.0/webp3/requestutils.py
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2020-03-13 22:23:14.636323 webp3-0.5.0/webp3/static/
--rw-r--r--   0 ntome     (1000) ntome     (1000)      689 2020-03-13 22:22:53.000000 webp3-0.5.0/webp3/static/COPYING.WTFPL
--rw-r--r--   0 ntome     (1000) ntome     (1000)     1440 2020-03-13 22:22:53.000000 webp3-0.5.0/webp3/static/base.tpl
--rw-r--r--   0 ntome     (1000) ntome     (1000)     1166 2020-03-13 22:22:53.000000 webp3-0.5.0/webp3/static/favicon.png
--rw-r--r--   0 ntome     (1000) ntome     (1000)     6065 2020-03-13 22:22:53.000000 webp3-0.5.0/webp3/static/player.js
--rw-r--r--   0 ntome     (1000) ntome     (1000)      729 2020-03-13 22:22:53.000000 webp3-0.5.0/webp3/static/style.css
--rw-r--r--   0 ntome     (1000) ntome     (1000)      934 2020-03-13 22:22:53.000000 webp3-0.5.0/webp3/webp3.wsgi
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2020-03-13 22:23:14.636323 webp3-0.5.0/webp3.egg-info/
--rw-r--r--   0 ntome     (1000) ntome     (1000)     1356 2020-03-13 22:23:13.000000 webp3-0.5.0/webp3.egg-info/PKG-INFO
--rw-r--r--   0 ntome     (1000) ntome     (1000)      563 2020-03-13 22:23:13.000000 webp3-0.5.0/webp3.egg-info/SOURCES.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)        1 2020-03-13 22:23:13.000000 webp3-0.5.0/webp3.egg-info/dependency_links.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)       38 2020-03-13 22:23:13.000000 webp3-0.5.0/webp3.egg-info/entry_points.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)        1 2020-03-13 22:23:13.000000 webp3-0.5.0/webp3.egg-info/not-zip-safe
--rw-r--r--   0 ntome     (1000) ntome     (1000)       16 2020-03-13 22:23:13.000000 webp3-0.5.0/webp3.egg-info/requires.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)        6 2020-03-13 22:23:13.000000 webp3-0.5.0/webp3.egg-info/top_level.txt
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 webp3-0.6.0/apache/install-webp3.rst
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 webp3-0.6.0/apache/install-webp3.sh
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 webp3-0.6.0/apache/webp3.conf
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/__init__.py
+-rwxr-xr-x   0        0        0      820 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/__main__.py
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/app.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/conf.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/exceptions.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/main_wsgi.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/pathutils.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/requestutils.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/webp3.wsgi
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/static/COPYING.WTFPL
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/static/base.tpl
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/static/favicon.png
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/static/player.js
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/static/style.css
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 webp3-0.6.0/.gitignore
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 webp3-0.6.0/COPYING.WTFPL
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 webp3-0.6.0/README.rst
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 webp3-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 webp3-0.6.0/PKG-INFO
```

### Comparing `webp3-0.5.0/README.rst` & `webp3-0.6.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -58,44 +58,53 @@
 
 WebP3 will listen on port (default: 8000)
 
 WSGI
 ----
 
 WebP3 can be set up to run as a WSGI app, for example to be served by an existing Apache instance.
-When using WSGI, the mappings that were passed on command-line should now be placed in a ``share.conf`` file, with one ``NAME=PATH`` entry per line.
+When using WSGI, the mappings that were passed on command-line should now be placed in a ``webp3.conf`` file, with one ``NAME=PATH`` entry per line.
 
 Using the documented script in the ``apache`` folder, the installation is as follows:
 
 * the WebP3 code and WSGI is typically in a path like /usr/lib/python3/dist-packages/webp3
 * the Apache configuration is in /etc/apache2/sites-available/webp3.conf
 * the WebP3 config indicating the locations of the music files is at /etc/webp3.conf
 
 Using an Apache instance to run the WebP3 WSGI allows:
 
 * HTTPS
 * serving the music tree under an URL prefix
 
+If not using the default location, the config file can be passed in env variable ``WEBP3_CONF``.
+
 Dependencies
 ++++++++++++
 
 WebP3 is written in Python 3 and uses:
 
-* `Bottle web framework <http://bottlepy.org/>`_
-* `Mako templates <http://www.makotemplates.org/>`_
+* `Bottle web framework <https://bottlepy.org/>`_
+* `Mako templates <https://www.makotemplates.org/>`_
 
 Security
 ++++++++
 
 WebP3 does not write files. However, it gives access to all files and folders contained in directories specified in its configuration.
 Therefore, directory containing sensitive data should not be put in its configuration.
 
 WebP3 does not have by itself any authentication mechanism to restrict access to its content.
 If this is desired a proxy should be used, or access can be configured in an existing WSGI server (like Apache).
 
 WebP3 reads files with the process' permissions. For example, if using WSGI, WebP3 will likely read files with the ``www-data`` user's permissions.
 WebP3 does not follow symlinks.
 
+Install
++++++++
+
+On `PyPI <https://pypi.org/project/webp3/>`_::
+
+	pip install webp3
+
 License
 +++++++
 
-WebP3 is licensed under the `do What The Fuck you want Public License v2 <http://wtfpl.net>`_.
+WebP3 is licensed under the `do What The Fuck you want Public License v2 <https://wtfpl.net>`_.
```

### Comparing `webp3-0.5.0/apache/install-webp3.sh` & `webp3-0.6.0/apache/install-webp3.sh`

 * *Files identical despite different names*

### Comparing `webp3-0.5.0/webp3/__main__.py` & `webp3-0.6.0/webp3/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# license: You can redistribute this file and/or modify it under the terms of the WTFPLv2 [see COPYING.WTFPL]
+# SPDX-License-Identifier: WTFPL
 
 import argparse
 from pathlib import Path
 
 from . import conf
```

### Comparing `webp3-0.5.0/webp3/app.py` & `webp3-0.6.0/webp3/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# license: You can redistribute this file and/or modify it under the terms of the WTFPLv2 [see COPYING.WTFPL]
+# SPDX-License-Identifier: WTFPL
 
 import json
 from urllib.parse import urljoin, quote as urlquote
 from pathlib import Path
 
 from bottle import request, response, redirect, mako_template, static_file, Bottle
```

### Comparing `webp3-0.5.0/webp3/pathutils.py` & `webp3-0.6.0/webp3/pathutils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# license: You can redistribute this file and/or modify it under the terms of the WTFPLv2 [see COPYING.WTFPL]
+# SPDX-License-Identifier: WTFPL
 
 from collections import namedtuple
 import os
 import re
 import hashlib
 import mimetypes
 from pathlib import Path
```

### Comparing `webp3-0.5.0/webp3/requestutils.py` & `webp3-0.6.0/webp3/requestutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# license: You can redistribute this file and/or modify it under the terms of the WTFPLv2 [see COPYING.WTFPL]
+# SPDX-License-Identifier: WTFPL
 
 from functools import wraps
 import errno
 import hashlib
 
 from bottle import request, response, abort
```

### Comparing `webp3-0.5.0/webp3/static/COPYING.WTFPL` & `webp3-0.6.0/webp3/static/COPYING.WTFPL`

 * *Files identical despite different names*

### Comparing `webp3-0.5.0/webp3/static/base.tpl` & `webp3-0.6.0/webp3/static/base.tpl`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 
 <div id="toolbar"><a id="toolPrev" href="javascript:pl_prev()">&#x23EE;</a><a id="toolPP" href="javascript:playPause()">&#x23F5;</a><a id="toolNext" href="javascript:pl_next()">&#x23ED;</a><span id="song"></span><div id="time"><span id="timeText">--:--</span></div><div id="seekbar"> </div>
 </div>
 
 <h4 class="title">${relpath}</h4>
 
 <ul id="listing">
+	% if str(toroot) != ".":
 	<li class="parent"><a href="..">Parent</a></li>
+	% endif
 	% for item in items:
 		% if item['is_dir']:
 			<li class="dir"><a href="${item['basename'] | q}/">${item['basename']}</a>/</li>
 		% else:
 			<li class="file ${item['is_audio'] and 'audio' or ''}"><a href="${item['basename'] | q}">${item['basename']}</a></li>
 		% endif
 	% endfor
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
 <%! from urllib.parse import quote def q(u): return quote(u.encode('utf-8')) %>
 
 
 
 &#x23EE;&#x23F5;&#x23ED;
 --:--
 *** ${relpath} ***
+    * % if str(toroot) != ".":
     * Parent
-    * % for item in items: % if item['is_dir']:
+    * % endif % for item in items: % if item['is_dir']:
     * ${item['basename']}/
     * % else:
     * ${item['basename']}
     * % endif % endfor
 Play_directory
 Playlist
 [Image]
```

### Comparing `webp3-0.5.0/webp3/static/favicon.png` & `webp3-0.6.0/webp3/static/favicon.png`

 * *Files identical despite different names*

### Comparing `webp3-0.5.0/webp3/static/player.js` & `webp3-0.6.0/webp3/static/player.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/** You can redistribute this file and/or modify it under the terms of the WTFPLv2 [see /_/COPYING.WTFPL] */
+/** SPDX-License-Identifier: WTFPL */
 
 var useRemainingTime = false;
 var playlist = [];
 var playlist_index = 0;
 
 /* pad(7, 3) == "007" */
 function pad(n, width, z) {
```

### Comparing `webp3-0.5.0/webp3/static/style.css` & `webp3-0.6.0/webp3/static/style.css`

 * *Files identical despite different names*

### Comparing `webp3-0.5.0/webp3/webp3.wsgi` & `webp3-0.6.0/webp3/main_wsgi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-# license: You can redistribute this file and/or modify it under the terms of the WTFPLv2 [see COPYING.WTFPL]
+# SPDX-License-Identifier: WTFPL
 
-from __future__ import print_function
-import sys
 import os
 from pathlib import Path
 
-import bottle
 import webp3.conf
 import webp3.app
 
 
 def read_conf(environ):
-	path = environ.get('webp3.conf', '/etc/webp3.conf')
+	path = environ.get('webp3.conf', os.environ.get('WEBP3_CONF', '/etc/webp3.conf'))
 	if not os.path.exists(path):
 		raise RuntimeError('missing config file')
 
 	with open(path) as conf:
 		roots = {}
 		for line in conf:
 			line = line.rstrip()
```

