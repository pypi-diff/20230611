# Comparing `tmp/survey-4.3.0a0.tar.gz` & `tmp/survey-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survey-4.3.0a0.tar", last modified: Sat May 27 18:34:08 2023, max compression
+gzip compressed data, was "survey-4.4.0.tar", last modified: Sun Jun 11 09:46:59 2023, max compression
```

## Comparing `survey-4.3.0a0.tar` & `survey-4.4.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:08.941357 survey-4.3.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-27 18:33:59.000000 survey-4.3.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-27 18:34:08.941357 survey-4.3.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-27 18:33:59.000000 survey-4.3.0a0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 18:34:08.941357 survey-4.3.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-27 18:33:59.000000 survey-4.3.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:08.937356 survey-4.3.0a0/survey/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_controls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:08.941357 survey-4.3.0a0/survey/_core/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_console.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_io_os.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_io_os_nt.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_io_os_posix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_core/_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_funnels.py
--rw-r--r--   0 runner    (1001) docker     (123)    13214 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_mutates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_printers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_searches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_visuals.py
--rw-r--r--   0 runner    (1001) docker     (123)    59354 2023-05-27 18:33:59.000000 survey-4.3.0a0/survey/_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:34:08.937356 survey-4.3.0a0/survey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-27 18:34:08.000000 survey-4.3.0a0/survey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-27 18:34:08.000000 survey-4.3.0a0/survey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 18:34:08.000000 survey-4.3.0a0/survey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-27 18:34:08.000000 survey-4.3.0a0/survey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 18:34:08.000000 survey-4.3.0a0/survey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:46:59.835433 survey-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-11 09:46:50.000000 survey-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-11 09:46:59.835433 survey-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-11 09:46:50.000000 survey-4.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 09:46:59.835433 survey-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-11 09:46:50.000000 survey-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:46:59.831433 survey-4.4.0/survey/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-11 09:46:50.000000 survey-4.4.0/survey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_controls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:46:59.835433 survey-4.4.0/survey/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_io_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_io_os_nt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_io_os_posix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_core/_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30590 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_funnels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13214 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_mutates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_printers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_visuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59339 2023-06-11 09:46:50.000000 survey-4.4.0/survey/_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:46:59.831433 survey-4.4.0/survey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-11 09:46:59.000000 survey-4.4.0/survey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-11 09:46:59.000000 survey-4.4.0/survey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 09:46:59.000000 survey-4.4.0/survey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-11 09:46:59.000000 survey-4.4.0/survey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 09:46:59.000000 survey-4.4.0/survey.egg-info/top_level.txt
```

### Comparing `survey-4.3.0a0/LICENSE` & `survey-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/PKG-INFO` & `survey-4.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 4.3.0a0
+Version: 4.4.0
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Provides-Extra: docs
 License-File: LICENSE
 
 ✨ A simple library for creating beautiful interactive prompts.
 
 .. image:: https://github.com/Exahilosys/survey/blob/main/docs/_static/images/showcase-1.gif?raw=true
 
@@ -22,15 +22,15 @@
 - **Complete**: Supports Windows 10 (Anniversary Update and up).
 
 Installing
 ----------
 
 .. code-block::
 
-    pip install survey==4.1.1a0
+    pip install survey
 
 Links
 -----
 
 - Check out the `Quickstart <https://survey.readthedocs.io/reference.html>`_ guide for more.
 - Greatly inspired by `AlecAivazis's GoLang <https://github.com/AlecAivazis/survey>`_ library.
```

### Comparing `survey-4.3.0a0/README.rst` & `survey-4.4.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 - **Complete**: Supports Windows 10 (Anniversary Update and up).
 
 Installing
 ----------
 
 .. code-block::
 
-    pip install survey==4.1.1a0
+    pip install survey
 
 Links
 -----
 
 - Check out the `Quickstart <https://survey.readthedocs.io/reference.html>`_ guide for more.
 - Greatly inspired by `AlecAivazis's GoLang <https://github.com/AlecAivazis/survey>`_ library.
```

### Comparing `survey-4.3.0a0/setup.py` & `survey-4.4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open('README.rst') as file:
     readme = file.read()
 
 author = 'Exahilosys'
 project = 'survey'
-version = '4.3.0-alpha'
+version = '4.4.0'
 
 url = 'https://github.com/{0}/{1}'.format(author, project)
 
 setuptools.setup(
     name = project,
-    python_requires = '>=3.11',
+    python_requires = '>=3.10',
     version = version,
     url = url,
     packages = setuptools.find_packages(),
     license = 'MIT',
     description = 'A simple library for creating beautiful interactive prompts.',
     long_description = readme,
     extras_require = {
```

### Comparing `survey-4.3.0a0/survey/__init__.py` & `survey-4.4.0/survey/__init__.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_colors.py` & `survey-4.4.0/survey/_colors.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_controls.py` & `survey-4.4.0/survey/_controls.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_core/__init__.py` & `survey-4.4.0/survey/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_core/_ansi.py` & `survey-4.4.0/survey/_core/_ansi.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_core/_console.py` & `survey-4.4.0/survey/_core/_console.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_core/_cursor.py` & `survey-4.4.0/survey/_core/_cursor.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_core/_handle.py` & `survey-4.4.0/survey/_core/_handle.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_core/_helpers.py` & `survey-4.4.0/survey/_core/_helpers.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_core/_io.py` & `survey-4.4.0/survey/_core/_io.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_core/_io_os.py` & `survey-4.4.0/survey/_core/_io_os.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_core/_io_os_nt.py` & `survey-4.4.0/survey/_core/_io_os_nt.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_core/_io_os_posix.py` & `survey-4.4.0/survey/_core/_io_os_posix.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_core/_render.py` & `survey-4.4.0/survey/_core/_render.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,20 +75,23 @@
 
     # turn to index via count
     usr_y -= 1
 
     return (usr_y, usr_x)
 
 
-@dataclasses.dataclass(slots = True, weakref_slot = True, eq = False)
 class Memory:
 
-    y: int
-    x: int
+    __slots__ = ('y', 'x', '__weakref__')
 
+    def __init__(self, y, x):
+
+        self.y = y
+        self.x = x
+    
 
 _type_Render_draw_lines: typing.TypeAlias = list[list[str]]
 _type_Render_draw_point: typing.TypeAlias = list[int, int] | None
 
 
 class Render:
```

### Comparing `survey-4.3.0a0/survey/_core/_screen.py` & `survey-4.4.0/survey/_core/_screen.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_core/_source.py` & `survey-4.4.0/survey/_core/_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     none     = None
     text     = _ansi.Text
     control  = _ansi.Control
     escape   = _ansi.Escape
     sequence = _ansi.Sequence
 
 
-class Event(enum.StrEnum):
+class Event(str, enum.Enum):
 
     """
     Event()
 
     Names for received events.
     """
```

### Comparing `survey-4.3.0a0/survey/_funnels.py` & `survey-4.4.0/survey/_funnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         '********|***************'
         '******** *************'
     """
 
     return functools.partial(_text_replace, rune)
 
 
-class JustType(enum.StrEnum):
+class JustType(str, enum.Enum):
 
     """
     JustType()
 
     Denotes the type of alignment.
     """
```

### Comparing `survey-4.3.0a0/survey/_graphics.py` & `survey-4.4.0/survey/_graphics.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_handle.py` & `survey-4.4.0/survey/_handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from . import _core
 from . import _controls
 
 
 __all__ = ('EventType', 'Abort', 'Handle')
 
 
-class EventType(enum.StrEnum):
+class EventType(str, enum.Enum):
 
     """
     Flags whether the event is called back before or after invokation.
     """
 
     enter = 'enter'
     leave = 'leave'
```

### Comparing `survey-4.3.0a0/survey/_helpers.py` & `survey-4.4.0/survey/_helpers.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_mutates.py` & `survey-4.4.0/survey/_mutates.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_printers.py` & `survey-4.4.0/survey/_printers.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_routines.py` & `survey-4.4.0/survey/_routines.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_searches.py` & `survey-4.4.0/survey/_searches.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_stage.py` & `survey-4.4.0/survey/_stage.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_theme.py` & `survey-4.4.0/survey/_theme.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_utils.py` & `survey-4.4.0/survey/_utils.py`

 * *Files identical despite different names*

### Comparing `survey-4.3.0a0/survey/_visuals.py` & `survey-4.4.0/survey/_visuals.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from . import _core
 
 
 __all__ = ('Visual', 'Text', 'Mesh', 'Line')
 
 
 _type_Visual_init_get         : typing.TypeAlias = typing.Callable[[bool, bool], tuple[typing.Any]]
-_type_Visual_init_funnel_enter: typing.TypeAlias = typing.Callable[[typing.Unpack[typing.Any]], None] | None
+_type_Visual_init_funnel_enter: typing.TypeAlias = typing.Callable[[typing.Any], None] | None
 _type_Visual_init_funnel_leave: typing.TypeAlias = typing.Callable[[_core._type_Render_draw_lines, _core._type_Render_draw_point], None] | None
 
 _type_Visual_get_enter        : typing.TypeAlias = bool
 _type_Visual_get_leave        : typing.TypeAlias = bool
 _type_Visual_get_return       : typing.TypeAlias = tuple[_core._type_Render_draw_lines, _core._type_Render_draw_point] | None
```

### Comparing `survey-4.3.0a0/survey/_widgets.py` & `survey-4.4.0/survey/_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
 
     wrapper = _start_get_actor_contextual(parse, context)
 
     return wrapper
 
 
 _type_start_start_get_actor_dynamic_parse: typing.TypeAlias = _type_start_get_actor_contextual_parse
-_type_start_start_get_actor_dynamic_fetch: typing.TypeAlias = typing.Callable[[typing.Unpack[typing.Any]], tuple[_visuals._type_Text_link_lines, _visuals._type_Text_link_point]]
+_type_start_start_get_actor_dynamic_fetch: typing.TypeAlias = typing.Callable[[typing.Any], tuple[_visuals._type_Text_link_lines, _visuals._type_Text_link_point]]
 
 
 def _start_get_actor_dynamic(parse: _type_start_start_get_actor_dynamic_parse, 
                              fetch: _type_start_start_get_actor_dynamic_fetch):
 
     context = contextvars.ContextVar('state')
```

### Comparing `survey-4.3.0a0/survey.egg-info/PKG-INFO` & `survey-4.4.0/survey.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 4.3.0a0
+Version: 4.4.0
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Provides-Extra: docs
 License-File: LICENSE
 
 ✨ A simple library for creating beautiful interactive prompts.
 
 .. image:: https://github.com/Exahilosys/survey/blob/main/docs/_static/images/showcase-1.gif?raw=true
 
@@ -22,15 +22,15 @@
 - **Complete**: Supports Windows 10 (Anniversary Update and up).
 
 Installing
 ----------
 
 .. code-block::
 
-    pip install survey==4.1.1a0
+    pip install survey
 
 Links
 -----
 
 - Check out the `Quickstart <https://survey.readthedocs.io/reference.html>`_ guide for more.
 - Greatly inspired by `AlecAivazis's GoLang <https://github.com/AlecAivazis/survey>`_ library.
```

### Comparing `survey-4.3.0a0/survey.egg-info/SOURCES.txt` & `survey-4.4.0/survey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

