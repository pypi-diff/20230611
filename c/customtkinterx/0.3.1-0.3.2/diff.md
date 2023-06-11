# Comparing `tmp/customtkinterx-0.3.1.tar.gz` & `tmp/customtkinterx-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customtkinterx-0.3.1.tar", max compression
+gzip compressed data, was "customtkinterx-0.3.2.tar", max compression
```

## Comparing `customtkinterx-0.3.1.tar` & `customtkinterx-0.3.2.tar`

### file list

```diff
@@ -1,42 +1,48 @@
--rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.3.1/customtkinterx/__base64.py
--rw-r--r--   0        0        0      982 2023-06-04 08:55:50.204860 customtkinterx-0.3.1/customtkinterx/__init__.py
--rw-r--r--   0        0        0      810 2023-06-04 08:43:25.091225 customtkinterx-0.3.1/customtkinterx/__main__.py
--rw-r--r--   0        0        0     8540 2023-06-03 22:47:50.802511 customtkinterx-0.3.1/customtkinterx/CTkCustom.py
--rw-r--r--   0        0        0     6312 2023-06-03 22:39:55.190954 customtkinterx-0.3.1/customtkinterx/CTkFluentTheme.py
--rw-r--r--   0        0        0     6286 2023-06-03 04:57:04.717519 customtkinterx-0.3.1/customtkinterx/CTkInfoBar.py
--rw-r--r--   0        0        0     1244 2023-06-02 11:00:54.754723 customtkinterx-0.3.1/customtkinterx/CTkListBox.py
--rw-r--r--   0        0        0     6321 2023-06-04 02:18:15.803265 customtkinterx-0.3.1/customtkinterx/CTkMaterialTheme.py
--rw-r--r--   0        0        0     2596 2023-06-04 02:13:08.630709 customtkinterx-0.3.1/customtkinterx/CTkMegaMenuBar.py
--rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.3.1/customtkinterx/CTkMenuBar/__init__.py
--rw-r--r--   0        0        0      522 2023-06-03 04:06:01.937274 customtkinterx-0.3.1/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16174 2023-06-03 04:13:46.399109 customtkinterx-0.3.1/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc
--rw-r--r--   0        0        0     5239 2023-06-03 04:13:46.393587 customtkinterx-0.3.1/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc
--rw-r--r--   0        0        0     9724 2023-06-03 04:13:46.396108 customtkinterx-0.3.1/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc
--rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.3.1/customtkinterx/CTkMenuBar/dropdown_menu.py
--rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.3.1/customtkinterx/CTkMenuBar/menu_bar.py
--rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.3.1/customtkinterx/CTkMenuBar/title_menu_win.py
--rw-r--r--   0        0        0     6285 2023-06-03 22:42:43.931473 customtkinterx-0.3.1/customtkinterx/CTkMinimalTheme.py
--rw-r--r--   0        0        0     6337 2023-06-04 02:14:05.106099 customtkinterx-0.3.1/customtkinterx/CTkOffice2019Theme.py
--rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.3.1/customtkinterx/CTkPDFViewer/__init__.py
--rw-r--r--   0        0        0      445 2023-06-03 04:13:46.400109 customtkinterx-0.3.1/customtkinterx/CTkPDFViewer/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6312 2023-06-03 05:49:55.800794 customtkinterx-0.3.1/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc
--rw-r--r--   0        0        0     3543 2023-06-03 05:14:11.938896 customtkinterx-0.3.1/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
--rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.3.1/customtkinterx/CTkTable/__init__.py
--rw-r--r--   0        0        0      427 2023-06-03 04:41:34.919572 customtkinterx-0.3.1/customtkinterx/CTkTable/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    11621 2023-06-03 04:41:34.922572 customtkinterx-0.3.1/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc
--rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.3.1/customtkinterx/CTkTable/ctktable.py
--rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.3.1/customtkinterx/CTkToolTip/__init__.py
--rw-r--r--   0        0        0      426 2023-06-03 04:22:17.427710 customtkinterx-0.3.1/customtkinterx/CTkToolTip/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    10684 2023-06-03 04:26:02.400121 customtkinterx-0.3.1/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc
--rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.3.1/customtkinterx/CTkToolTip/ctk_tooltip.py
--rw-r--r--   0        0        0     5690 2023-06-03 22:45:30.417651 customtkinterx-0.3.1/customtkinterx/Fluent.json
--rw-r--r--   0        0        0     9600 2023-06-04 10:39:24.007773 customtkinterx-0.3.1/customtkinterx/LaunchMusix.py
--rw-r--r--   0        0        0     5683 2023-06-04 02:21:16.783149 customtkinterx-0.3.1/customtkinterx/Material.json
--rw-r--r--   0        0        0     5655 2023-06-03 22:45:30.423651 customtkinterx-0.3.1/customtkinterx/Minimal.json
--rw-r--r--   0        0        0     1045 2023-06-04 10:35:45.029136 customtkinterx-0.3.1/customtkinterx/Musix-Dark.png
--rw-r--r--   0        0        0     1007 2023-06-04 10:34:21.619230 customtkinterx-0.3.1/customtkinterx/Musix.png
--rw-r--r--   0        0        0     5683 2023-06-03 23:01:51.610936 customtkinterx-0.3.1/customtkinterx/Office2019.json
--rw-r--r--   0        0        0     5435 2023-06-03 06:15:30.726312 customtkinterx-0.3.1/customtkinterx/tk_dragtool.py
--rw-r--r--   0        0        0      368 2023-06-04 10:41:51.563025 customtkinterx-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3686 2023-06-03 06:54:12.682589 customtkinterx-0.3.1/README.md
--rw-r--r--   0        0        0     4165 1970-01-01 00:00:00.000000 customtkinterx-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.3.2/customtkinterx/__base64.py
+-rw-r--r--   0        0        0     1036 2023-06-10 00:29:27.871591 customtkinterx-0.3.2/customtkinterx/__init__.py
+-rw-r--r--   0        0        0      812 2023-06-04 13:04:43.345604 customtkinterx-0.3.2/customtkinterx/__main__.py
+-rw-r--r--   0        0        0     8540 2023-06-03 22:47:50.802511 customtkinterx-0.3.2/customtkinterx/CTkCustom.py
+-rw-r--r--   0        0        0     6312 2023-06-03 22:39:55.190954 customtkinterx-0.3.2/customtkinterx/CTkFluentTheme.py
+-rw-r--r--   0        0        0     6344 2023-06-04 13:04:43.403550 customtkinterx-0.3.2/customtkinterx/CTkGhostSharkTheme.py
+-rw-r--r--   0        0        0     6286 2023-06-03 04:57:04.717519 customtkinterx-0.3.2/customtkinterx/CTkInfoBar.py
+-rw-r--r--   0        0        0     1244 2023-06-02 11:00:54.754723 customtkinterx-0.3.2/customtkinterx/CTkListBox.py
+-rw-r--r--   0        0        0     2596 2023-06-04 02:13:08.630709 customtkinterx-0.3.2/customtkinterx/CTkMegaMenuBar.py
+-rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__init__.py
+-rw-r--r--   0        0        0      522 2023-06-03 04:06:01.937274 customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16174 2023-06-03 04:13:46.399109 customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc
+-rw-r--r--   0        0        0     5239 2023-06-03 04:13:46.393587 customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc
+-rw-r--r--   0        0        0     9724 2023-06-03 04:13:46.396108 customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc
+-rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.3.2/customtkinterx/CTkMenuBar/dropdown_menu.py
+-rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.3.2/customtkinterx/CTkMenuBar/menu_bar.py
+-rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.3.2/customtkinterx/CTkMenuBar/title_menu_win.py
+-rw-r--r--   0        0        0     6285 2023-06-03 22:42:43.931473 customtkinterx-0.3.2/customtkinterx/CTkMinimalTheme.py
+-rw-r--r--   0        0        0     6337 2023-06-04 02:14:05.106099 customtkinterx-0.3.2/customtkinterx/CTkOffice2019Theme.py
+-rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.3.2/customtkinterx/CTkPDFViewer/__init__.py
+-rw-r--r--   0        0        0      445 2023-06-03 04:13:46.400109 customtkinterx-0.3.2/customtkinterx/CTkPDFViewer/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6312 2023-06-03 05:49:55.800794 customtkinterx-0.3.2/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc
+-rw-r--r--   0        0        0     3543 2023-06-03 05:14:11.938896 customtkinterx-0.3.2/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
+-rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.3.2/customtkinterx/CTkTable/__init__.py
+-rw-r--r--   0        0        0      427 2023-06-03 04:41:34.919572 customtkinterx-0.3.2/customtkinterx/CTkTable/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    11621 2023-06-03 04:41:34.922572 customtkinterx-0.3.2/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc
+-rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.3.2/customtkinterx/CTkTable/ctktable.py
+-rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.3.2/customtkinterx/CTkToolTip/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-03 04:22:17.427710 customtkinterx-0.3.2/customtkinterx/CTkToolTip/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    10684 2023-06-03 04:26:02.400121 customtkinterx-0.3.2/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc
+-rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.3.2/customtkinterx/CTkToolTip/ctk_tooltip.py
+-rw-r--r--   0        0        0     5690 2023-06-03 22:45:30.417651 customtkinterx-0.3.2/customtkinterx/Fluent.json
+-rw-r--r--   0        0        0      113 2023-06-09 23:34:51.644065 customtkinterx-0.3.2/customtkinterx/fluent_android/__init__.py
+-rw-r--r--   0        0        0      305 2023-06-09 23:34:52.417977 customtkinterx-0.3.2/customtkinterx/fluent_android/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7135 2023-06-09 23:42:37.438327 customtkinterx-0.3.2/customtkinterx/fluent_android/__pycache__/CTkFluentAndroidTheme.cpython-311.pyc
+-rw-r--r--   0        0        0     6375 2023-06-09 23:42:02.599385 customtkinterx-0.3.2/customtkinterx/fluent_android/CTkFluentAndroidTheme.py
+-rw-r--r--   0        0        0     1733 2023-06-10 00:34:11.681775 customtkinterx-0.3.2/customtkinterx/fluent_android/CTkFluentAppBar.py
+-rw-r--r--   0        0        0     5680 2023-06-10 00:28:44.744869 customtkinterx-0.3.2/customtkinterx/fluent_android/FluentAndroid.json
+-rw-r--r--   0        0        0     5437 2023-06-04 13:11:47.958728 customtkinterx-0.3.2/customtkinterx/GhostShark.json
+-rw-r--r--   0        0        0    10030 2023-06-10 00:29:27.916591 customtkinterx-0.3.2/customtkinterx/LaunchMusix.py
+-rw-r--r--   0        0        0     5655 2023-06-03 22:45:30.423651 customtkinterx-0.3.2/customtkinterx/Minimal.json
+-rw-r--r--   0        0        0     1377 2023-06-04 11:35:40.844283 customtkinterx-0.3.2/customtkinterx/Musix-Dark.png
+-rw-r--r--   0        0        0     1039 2023-06-04 11:33:35.093179 customtkinterx-0.3.2/customtkinterx/Musix.png
+-rw-r--r--   0        0        0     5683 2023-06-03 23:01:51.610936 customtkinterx-0.3.2/customtkinterx/Office2019.json
+-rw-r--r--   0        0        0     5435 2023-06-03 06:15:30.726312 customtkinterx-0.3.2/customtkinterx/tk_dragtool.py
+-rw-r--r--   0        0        0      368 2023-06-11 07:35:54.646052 customtkinterx-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3686 2023-06-03 06:54:12.682589 customtkinterx-0.3.2/README.md
+-rw-r--r--   0        0        0     4165 1970-01-01 00:00:00.000000 customtkinterx-0.3.2/PKG-INFO
```

### Comparing `customtkinterx-0.3.1/customtkinterx/__init__.py` & `customtkinterx-0.3.2/customtkinterx/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from customtkinterx.CTkCustom import CTkCustom
 from customtkinterx.CTkFluentTheme import use_fluent_theme as CTkFluentTheme
 from customtkinterx.CTkMinimalTheme import use_minimal_theme as CTkMinimalTheme
 from customtkinterx.CTkOffice2019Theme import use_office2019_theme as CTkOffice2019Theme
-from customtkinterx.CTkMaterialTheme import use_material_theme as CTkMaterialTheme
+from customtkinterx.CTkGhostSharkTheme import use_ghost_shark_theme as CTkGhostSharkTheme
 
 from customtkinterx.CTkInfoBar import CTkInfoBar, NORMAL, SUCCESS, CAUTION, CRITICAL
 from customtkinterx.CTkMegaMenuBar import CTkMegaMenuBar
 
+from customtkinterx.fluent_android import *
+
 # From https://github.com/Akascape/CTkMenuBar
 from customtkinterx.CTkMenuBar import CTkMenuBar, CTkTitleMenu, CustomDropdownMenu as CTkCustomDropdownMenu
 
 # From https://github.com/Akascape/CTkPDFViewer
 from customtkinterx.CTkPDFViewer import CTkPDFViewer
 
 # From https://github.com/Akascape/CTkToolTip
```

### Comparing `customtkinterx-0.3.1/customtkinterx/__main__.py` & `customtkinterx-0.3.2/customtkinterx/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from customtkinter import *
 from customtkinterx import *
 
-CTkMaterialTheme()
+CTkGhostSharkTheme()
 
 set_appearance_mode("dark")
 
 root = CTkCustom()
 root.title("CustomTkinterX")
 root.titlebar_title.configure(text="CustomTkinterX")
 root.create_sizegrip(True)
```

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkCustom.py` & `customtkinterx-0.3.2/customtkinterx/CTkCustom.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkFluentTheme.py` & `customtkinterx-0.3.2/customtkinterx/CTkFluentTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkInfoBar.py` & `customtkinterx-0.3.2/customtkinterx/CTkInfoBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkListBox.py` & `customtkinterx-0.3.2/customtkinterx/CTkListBox.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkMaterialTheme.py` & `customtkinterx-0.3.2/customtkinterx/CTkGhostSharkTheme.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-material_json = """
+ghost_shark_json = """
 {
   "CTkCustom": {
     "titlebar_color": ["#106ebe", "#106ebe"],
     "title_color": ["#ffffff", "#ffffff"],
 
     "transparent_color": "#101010",
 
@@ -187,25 +187,25 @@
 }
 """
 
 
 import os.path
 
 
-material_path = os.path.abspath(os.path.dirname(__file__)).replace("\\", "/") + "/Material.json"
+ghost_shark_path = os.path.abspath(os.path.dirname(__file__)).replace("\\", "/") + "/GhostShark.json"
 
 
-def material_theme():
+def ghost_shark_theme():
     from tempfile import mkstemp
     from customtkinter import set_default_color_theme
     _, __temp = mkstemp(suffix=".json")
     with open(__temp, "w") as __temp_file:
-        __temp_file.write(material_json)
+        __temp_file.write(ghost_shark_json)
     return __temp
 
 
-def use_material_theme():
+def use_ghost_shark_theme():
     from customtkinter import set_default_color_theme
     try:
-        set_default_color_theme(material_path)
+        set_default_color_theme(ghost_shark_path)
     except FileNotFoundError:
-        set_default_color_theme(material_theme())
+        set_default_color_theme(ghost_shark_theme())
```

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkMegaMenuBar.py` & `customtkinterx-0.3.2/customtkinterx/CTkMegaMenuBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc` & `customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc` & `customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc` & `customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc` & `customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkMenuBar/dropdown_menu.py` & `customtkinterx-0.3.2/customtkinterx/CTkMenuBar/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkMenuBar/menu_bar.py` & `customtkinterx-0.3.2/customtkinterx/CTkMenuBar/menu_bar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkMenuBar/title_menu_win.py` & `customtkinterx-0.3.2/customtkinterx/CTkMenuBar/title_menu_win.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkMinimalTheme.py` & `customtkinterx-0.3.2/customtkinterx/CTkMinimalTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkOffice2019Theme.py` & `customtkinterx-0.3.2/customtkinterx/CTkOffice2019Theme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc` & `customtkinterx-0.3.2/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py` & `customtkinterx-0.3.2/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc` & `customtkinterx-0.3.2/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkTable/ctktable.py` & `customtkinterx-0.3.2/customtkinterx/CTkTable/ctktable.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc` & `customtkinterx-0.3.2/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/CTkToolTip/ctk_tooltip.py` & `customtkinterx-0.3.2/customtkinterx/CTkToolTip/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/Fluent.json` & `customtkinterx-0.3.2/customtkinterx/Fluent.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/LaunchMusix.py` & `customtkinterx-0.3.2/customtkinterx/LaunchMusix.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,34 +164,45 @@
             self.download = CTkButton(self, width=100, text="下载", command=download)
             self.download.pack(side="right", padx=5, pady=5)
 
             self.args = CTkComboBox(self, values=["standard", "higher", "exhigh", "lossless"])
             self.args.set("higher")
             self.args.pack(side="right", padx=5, pady=5)
 
-    CTkMinimalTheme()
+    CTkFluentAndroidTheme()
     set_appearance_mode("Light")
 
     root = CTkCustom(title="Musix")
+    root.titlebar.configure(corner_radius=13)
     root.geometry("720x360")
-    root.create_sizegrip(True)
-    root.sizegrip.configure(text="", width=20, height=20, border_width=1)
+
+    from sys import platform
+
+    if platform == "win32":
+        root.create_sizegrip(True)
+        root.sizegrip.configure(text="", width=20, height=20, border_width=1)
+    else:
+        root.create_sizegrip(False)
 
     from PIL import Image
 
     root.titlebar_title.destroy()
 
     icon = CTkImage(light_image=Image.open("Musix.png"), dark_image=Image.open("Musix-Dark.png"), size=(30, 30))
     iconlabel = CTkLabel(root.titlebar, image=icon, text="", width=30, height=30)
     iconlabel.pack(side="left", padx=5, pady=5)
 
     title = CTkLabel(root.titlebar, text=root.title())
     title.pack(side="left", anchor="w", padx=10, pady=5)
     root.bind_move(title)
 
+    version = CTkLabel(root.titlebar, text="v2.2.0", font=CTkFont(size=10))
+    version.pack(side="left", anchor="sw", padx=10, pady=5)
+    root.bind_move(version)
+
     info = CTkInfoBar(root.mainframe, title="公告", text="当前版本为重制版2.0，已是最新版本", severity=SUCCESS, can_close=False)
     info.show()
 
     def dark():
         if darkbox.get():
             set_appearance_mode("Dark")
         else:
@@ -249,16 +260,17 @@
     searchbutton.pack(side="right", padx=5, pady=5)
 
     searchbox = CTkEntry(root.titlebar, width=200, height=30)
     searchbox.configure(placeholder_text="请输入歌曲名称 （按Enter键搜索）")
     searchbox.bind("<Return>", lambda event: search())
     searchbox.pack(side="right", fill="x", expand="yes", padx=(15, 5), pady=5)
 
+    #set_widget_scaling(1.15)
+    root.wm_iconphoto(False, PhotoImage(file="Musix.png"))
     root.mainloop()
 
-
 def run():
     run_v2()
 
 
 if __name__ == '__main__':
     run()
```

### Comparing `customtkinterx-0.3.1/customtkinterx/Material.json` & `customtkinterx-0.3.2/customtkinterx/Office2019.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.995275888133031%*

 * *Differences: {"'CTkButton'": "{'fg_color': ['#e5e5e5', '#3d3d3d'], 'border_color': ['#f3f3f3', '#949A9F']}",*

 * * "'CTkCustom'": "{'titlebar_color': ['#106ebe', '#106ebe']}"}*

```diff
@@ -3,22 +3,22 @@
         "fg_color": [
             "#ffffff",
             "#101010"
         ]
     },
     "CTkButton": {
         "border_color": [
-            "#d7d7d7",
-            "#282828"
+            "#f3f3f3",
+            "#949A9F"
         ],
         "border_width": 1,
         "corner_radius": 0,
         "fg_color": [
-            "#ffffff",
-            "#0a0a0a"
+            "#e5e5e5",
+            "#3d3d3d"
         ],
         "hover_color": [
             "#b2b2b2",
             "#151515"
         ],
         "text_color": [
             "#000000",
@@ -111,16 +111,16 @@
             "#ffffff"
         ],
         "title_color": [
             "#ffffff",
             "#ffffff"
         ],
         "titlebar_color": [
-            "#3f51b5",
-            "#3f51b5"
+            "#106ebe",
+            "#106ebe"
         ],
         "transparent_color": "#101010"
     },
     "CTkEntry": {
         "border_color": [
             "#f3f3f3",
             "#949A9F"
```

### Comparing `customtkinterx-0.3.1/customtkinterx/Minimal.json` & `customtkinterx-0.3.2/customtkinterx/Minimal.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/customtkinterx/Office2019.json` & `customtkinterx-0.3.2/customtkinterx/fluent_android/FluentAndroid.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9561933106575964%*

 * *Differences: {"'CTkButton'": "{'corner_radius': 2, 'border_width': 0, 'fg_color': ['#0078d4', '#0078d4'], "*

 * *                "'hover_color': ['#106ebe', '#0086f0'], 'text_color': {insert: [(1, '#000000')], "*

 * *                "delete: [0]}, 'text_color_disabled': ['#acacac', '#004a83']}",*

 * * "'CTkComboBox'": "{'corner_radius': 6, 'fg_color': ['#F9F9FA', '#343638'], 'border_color': "*

 * *                  "['#f2f2f2', '#303030']}",*

 * * "'CTkCustom'": "{'titlebar_color': ['#ffffff', '#2c2c2c'], 'title_color': ['gray10', '#DCE4EE']}", […]*

```diff
@@ -6,31 +6,31 @@
         ]
     },
     "CTkButton": {
         "border_color": [
             "#f3f3f3",
             "#949A9F"
         ],
-        "border_width": 1,
-        "corner_radius": 0,
+        "border_width": 0,
+        "corner_radius": 2,
         "fg_color": [
-            "#e5e5e5",
-            "#3d3d3d"
+            "#0078d4",
+            "#0078d4"
         ],
         "hover_color": [
-            "#b2b2b2",
-            "#151515"
+            "#106ebe",
+            "#0086f0"
         ],
         "text_color": [
-            "#000000",
-            "#ffffff"
+            "#ffffff",
+            "#000000"
         ],
         "text_color_disabled": [
-            "gray74",
-            "gray60"
+            "#acacac",
+            "#004a83"
         ]
     },
     "CTkCheckbox": {
         "border_color": [
             "#3E454A",
             "#949A9F"
         ],
@@ -55,30 +55,30 @@
         "text_color_disabled": [
             "gray60",
             "gray45"
         ]
     },
     "CTkComboBox": {
         "border_color": [
-            "#f3f3f3",
-            "#949A9F"
+            "#f2f2f2",
+            "#303030"
         ],
         "border_width": 1,
         "button_color": [
             "#f2f2f2",
             "#565B5E"
         ],
         "button_hover_color": [
             "#f2f2f2",
             "#565B5E"
         ],
-        "corner_radius": 0,
+        "corner_radius": 6,
         "fg_color": [
-            "#ffffff",
-            "#2f2f2f"
+            "#F9F9FA",
+            "#343638"
         ],
         "text_color": [
             "gray10",
             "#ffffff"
         ],
         "text_color_disabled": [
             "gray50",
@@ -107,70 +107,70 @@
             "#282828"
         ],
         "minimizebutton_text_color": [
             "#000000",
             "#ffffff"
         ],
         "title_color": [
-            "#ffffff",
-            "#ffffff"
+            "gray10",
+            "#DCE4EE"
         ],
         "titlebar_color": [
-            "#106ebe",
-            "#106ebe"
+            "#ffffff",
+            "#2c2c2c"
         ],
         "transparent_color": "#101010"
     },
     "CTkEntry": {
         "border_color": [
-            "#f3f3f3",
-            "#949A9F"
+            "#f2f2f2",
+            "#303030"
         ],
         "border_width": 1,
-        "corner_radius": 0,
+        "corner_radius": 6,
         "fg_color": [
-            "#ffffff",
-            "#2f2f2f"
+            "#F9F9FA",
+            "#343638"
         ],
         "placeholder_text_color": [
             "gray52",
             "gray62"
         ],
         "text_color": [
             "#000000",
             "#ffffff"
         ]
     },
     "CTkFont": {
         "Linux": {
             "family": "Roboto",
             "size": 13,
-            "weight": "normal"
+            "weight": "bold"
         },
         "Windows": {
-            "family": "Segoe UI",
+            "family": "Roboto",
             "size": 13,
-            "weight": "normal"
+            "weight": "bold"
         },
         "macOS": {
-            "family": "SF Display",
+            "family": "Roboto",
             "size": 13,
-            "weight": "normal"
+            "weight": "bold"
         }
     },
     "CTkFrame": {
         "border_color": [
             "#b0b2b2",
             "#424556"
         ],
-        "border_width": 1,
+        "border_width": 0,
         "corner_radius": 0,
         "fg_color": [
             "#ffffff",
-            "#1c1c1c"
+            "#212121"
         ],
         "top_fg_color": [
             "#ffffff",
             "#2c2c2c"
         ]
     },
     "CTkInfoBar": {
@@ -288,24 +288,24 @@
     "CTkScrollableFrame": {
         "label_fg_color": [
             "gray78",
             "gray23"
         ]
     },
     "CTkScrollbar": {
-        "border_spacing": 9,
+        "border_spacing": 4,
         "button_color": [
             "gray55",
             "gray41"
         ],
         "button_hover_color": [
             "gray40",
             "gray53"
         ],
-        "corner_radius": 0,
+        "corner_radius": 1000,
         "fg_color": "transparent"
     },
     "CTkSegmentedButton": {
         "border_width": 2,
         "corner_radius": 6,
         "fg_color": [
             "#979DA2",
@@ -355,25 +355,25 @@
         ],
         "progress_color": [
             "gray40",
             "#AAB0B5"
         ]
     },
     "CTkSwitch": {
-        "border_width": 1,
+        "border_width": 0.1,
         "button_color": [
             "#f3f3f3",
             "#000000"
         ],
         "button_hover_color": [
             "#bfbfbf",
             "#050505"
         ],
-        "button_length": 2,
-        "corner_radius": 8,
+        "button_length": 0,
+        "corner_radius": 1000,
         "fg_color": [
             "#ededed",
             "#1d1d1d"
         ],
         "progress_color": [
             "#0067c0",
             "#4cc2ff"
@@ -385,19 +385,19 @@
         "text_color_disabled": [
             "gray60",
             "gray45"
         ]
     },
     "CTkTextbox": {
         "border_color": [
-            "#f3f3f3",
-            "#949A9F"
+            "#979DA2",
+            "#565B5E"
         ],
-        "border_width": 1,
-        "corner_radius": 0,
+        "border_width": 0,
+        "corner_radius": 6,
         "fg_color": [
             "#F9F9FA",
             "#1D1E1E"
         ],
         "scrollbar_button_color": [
             "gray55",
             "gray41"
```

### Comparing `customtkinterx-0.3.1/customtkinterx/tk_dragtool.py` & `customtkinterx-0.3.2/customtkinterx/tk_dragtool.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/README.md` & `customtkinterx-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.1/PKG-INFO` & `customtkinterx-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customtkinterx
-Version: 0.3.1
+Version: 0.3.2
 Summary: extra widgets for customtkinter
 Author: XiangQinxi
 Author-email: XiangQinxi@outlook.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

