# Comparing `tmp/python-printr-2.9.tar.gz` & `tmp/python-printr-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-printr-2.9.tar", last modified: Tue Jun  6 13:18:28 2023, max compression
+gzip compressed data, was "python-printr-3.0.tar", last modified: Sun Jun 11 14:12:23 2023, max compression
```

## Comparing `python-printr-2.9.tar` & `python-printr-3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 13:18:28.671469 python-printr-2.9/
--rw-rw-rw-   0        0        0       66 2022-04-13 16:11:03.000000 python-printr-2.9/.gitignore
--rw-rw-rw-   0        0        0     3350 2023-06-06 13:18:28.671469 python-printr-2.9/PKG-INFO
--rw-rw-rw-   0        0        0     3092 2023-03-11 18:19:37.000000 python-printr-2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 13:18:28.666472 python-printr-2.9/printr/
--rw-rw-rw-   0        0        0     7817 2023-06-06 13:18:18.000000 python-printr-2.9/printr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:18:28.670469 python-printr-2.9/python_printr.egg-info/
--rw-rw-rw-   0        0        0     3350 2023-06-06 13:18:28.000000 python-printr-2.9/python_printr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-06-06 13:18:28.000000 python-printr-2.9/python_printr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 13:18:28.000000 python-printr-2.9/python_printr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-06 13:18:28.000000 python-printr-2.9/python_printr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 13:18:28.000000 python-printr-2.9/python_printr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-06 13:18:28.672469 python-printr-2.9/setup.cfg
--rw-rw-rw-   0        0        0      427 2023-06-06 13:18:24.000000 python-printr-2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:12:23.933689 python-printr-3.0/
+-rw-rw-rw-   0        0        0       66 2022-04-13 16:11:03.000000 python-printr-3.0/.gitignore
+-rw-rw-rw-   0        0        0     3347 2023-06-11 14:12:23.933689 python-printr-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3089 2023-06-11 14:12:17.000000 python-printr-3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 14:12:23.927694 python-printr-3.0/printr/
+-rw-rw-rw-   0        0        0     8183 2023-06-11 14:11:57.000000 python-printr-3.0/printr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:12:23.932690 python-printr-3.0/python_printr.egg-info/
+-rw-rw-rw-   0        0        0     3347 2023-06-11 14:12:23.000000 python-printr-3.0/python_printr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-06-11 14:12:23.000000 python-printr-3.0/python_printr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 14:12:23.000000 python-printr-3.0/python_printr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-11 14:12:23.000000 python-printr-3.0/python_printr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-11 14:12:23.000000 python-printr-3.0/python_printr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-11 14:12:23.934689 python-printr-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      427 2023-06-11 14:12:03.000000 python-printr-3.0/setup.py
```

### Comparing `python-printr-2.9/PKG-INFO` & `python-printr-3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-printr
-Version: 2.9
+Version: 3.0
 Summary: printr
 Home-page: https://github.com/xjxckk/python-printr/
 Download-URL: https://github.com/xjxckk/python-printr/archive/refs/tags/v0.1.tar.gz
 Description-Content-Type: text/markdown
 
 ### python-printr
 Python print functions to beautify output
@@ -19,20 +19,20 @@
 logger = logger(filename='test.log')
 log, current_time = logger.log, logger.current_time
 
 log('Here') # Prints to terminal and saves message to test.log
 ```
 
 ```
-from printr import printr, same_line, current_time
+from printr import print, same_line, current_time
 
 test_list = [{'id': 1, 'name': 'Leanne Graham', 'username': 'Bret', 'email': 'Sincere@april.biz', 'address': {'street': 'Kulas Light', 'suite': 'Apt. 556', 'city': 'Gwenborough', 'zipcode': '92998-3874', 'geo': {'lat': '-37.3159', 'lng': '81.1496'}}, 'phone': '1-770-736-8031 x56442', 'website': 'hildegard.org', 'company': {'name': 'Romaguera-Crona', 'catchPhrase': 'Multi-layered client-server neural-net', 'bs': 'harness real-time e-markets'}}, {'id': 2, 'name': 'Ervin Howell', 'username': 'Antonette', 'email': 'Shanna@melissa.tv', 'address': {'street': 'Victor Plains', 'suite': 'Suite 879', 'city': 'Wisokyburgh', 'zipcode': '90566-7771', 'geo': {'lat': '-43.9509', 'lng': '-34.4618'}}, 'phone': '010-692-6593 x09125', 'website': 'anastasia.net', 'company': {'name': 'Deckow-Crist', 'catchPhrase': 'Proactive didactic contingency', 'bs': 'synergize scalable supply-chains'}}]
 
-printr(test_list) # Formats dictionary with indents
-printr() # Print a line break
+print(test_list) # Formats dictionary with indents
+print() # Print a line break
 same_line('test', current_time=True) # Print the current_time with the message test to the same line
 sleep(1)
 same_line('testing', current_time=True) # Print the current_time with the message testing to the same line
 ```
 
 Output:
 ```
```

### Comparing `python-printr-2.9/README.md` & `python-printr-3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 logger = logger(filename='test.log')
 log, current_time = logger.log, logger.current_time
 
 log('Here') # Prints to terminal and saves message to test.log
 ```
 
 ```
-from printr import printr, same_line, current_time
+from printr import print, same_line, current_time
 
 test_list = [{'id': 1, 'name': 'Leanne Graham', 'username': 'Bret', 'email': 'Sincere@april.biz', 'address': {'street': 'Kulas Light', 'suite': 'Apt. 556', 'city': 'Gwenborough', 'zipcode': '92998-3874', 'geo': {'lat': '-37.3159', 'lng': '81.1496'}}, 'phone': '1-770-736-8031 x56442', 'website': 'hildegard.org', 'company': {'name': 'Romaguera-Crona', 'catchPhrase': 'Multi-layered client-server neural-net', 'bs': 'harness real-time e-markets'}}, {'id': 2, 'name': 'Ervin Howell', 'username': 'Antonette', 'email': 'Shanna@melissa.tv', 'address': {'street': 'Victor Plains', 'suite': 'Suite 879', 'city': 'Wisokyburgh', 'zipcode': '90566-7771', 'geo': {'lat': '-43.9509', 'lng': '-34.4618'}}, 'phone': '010-692-6593 x09125', 'website': 'anastasia.net', 'company': {'name': 'Deckow-Crist', 'catchPhrase': 'Proactive didactic contingency', 'bs': 'synergize scalable supply-chains'}}]
 
-printr(test_list) # Formats dictionary with indents
-printr() # Print a line break
+print(test_list) # Formats dictionary with indents
+print() # Print a line break
 same_line('test', current_time=True) # Print the current_time with the message test to the same line
 sleep(1)
 same_line('testing', current_time=True) # Print the current_time with the message testing to the same line
 ```
 
 Output:
 ```
```

### Comparing `python-printr-2.9/printr/__init__.py` & `python-printr-3.0/printr/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,20 +120,21 @@
     def remove_indent(self):
         if self.log_to_file:
             log_format = logging.Formatter(fmt='%(levelname)s - %(asctime)s.%(msecs)03d - Line %(lineno)s: %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
             self.log_file.setFormatter(log_format)
         coloredlogs.install(level=self.level, logger=self.logger, fmt='%(message)s') # Reset to default log format
         self.indent = ''
 
-class printr:
+say = print
+class print:
     '''printr'''
-    def __init__(self, *items, same_line=False, current_time=False, check_for_log=True, level='info'):
+    def __init__(self, *items, same_line=False, current_time=False, check_for_log=True, level='info', beautify=True):
         if len(items) == 1:
             message = items[0]
-            if isinstance(message, dict) or isinstance(message, list):
+            if beautify and (isinstance(message, dict) or isinstance(message, list)):
                 try: message = json.dumps(message, indent=4) # Beautify JSON objects
                 except TypeError: pass
         else:
             message = ''
             for item in items:
                 if message:
                     message += ' ' # Add space in between variables
@@ -144,33 +145,38 @@
         if current_time:
             current_time = datetime.now()
             current_time = current_time.strftime('%H:%M:%S:%f')
             message = f'{current_time}: {message}'
         if same_line:
             terminal_size = shutil.get_terminal_size() # Uses shutil rather than os to support piping output to file
             max_characters = terminal_size.columns - 1
-            print(' ' * max_characters, end='') # Clear previous output
-            print('\r', end='')
-            print(message, end='')
-            print('\r', end='')
+            say(' ' * max_characters, end='') # Clear previous output
+            say('\r', end='')
+            say(message, end='')
+            say('\r', end='')
         else:
             if not check_for_log:
-                print(message)
+                say(message)
             else:
                 logger = logging.getLogger()
                 if logger.level != 30:
                     if level == 'debug':
                         logger.debug(message)
                     elif level == 'error':
                         logger.error(message)
                     else:
                         logger.info(message)
                 elif level != 'debug':
-                    print(message)
+                    say(message)
+
+
+class printr:
+    def __init__(self, *items, same_line=False, current_time=False, check_for_log=True, level='info', beautify=True):
+        print(*items, same_line=same_line, current_time=current_time, check_for_log=check_for_log, level=level, beautify=beautify)
 
 class current_time:
-    def __init__(self, *items, same_line=False, check_for_log=True):
-        printr(*items, same_line=same_line, current_time=True, check_for_log=check_for_log)
+    def __init__(self, *items, same_line=False, check_for_log=True, beautify=True):
+        print(*items, same_line=same_line, current_time=True, check_for_log=check_for_log, beautify=beautify)
 
 class same_line:
-    def __init__(self, *items, current_time=False, check_for_log=True):
-        printr(*items, same_line=same_line, current_time=current_time, check_for_log=check_for_log)
+    def __init__(self, *items, current_time=False, check_for_log=True, beautify=True):
+        print(*items, same_line=same_line, current_time=current_time, check_for_log=check_for_log, beautify=beautify)
```

### Comparing `python-printr-2.9/python_printr.egg-info/PKG-INFO` & `python-printr-3.0/python_printr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-printr
-Version: 2.9
+Version: 3.0
 Summary: printr
 Home-page: https://github.com/xjxckk/python-printr/
 Download-URL: https://github.com/xjxckk/python-printr/archive/refs/tags/v0.1.tar.gz
 Description-Content-Type: text/markdown
 
 ### python-printr
 Python print functions to beautify output
@@ -19,20 +19,20 @@
 logger = logger(filename='test.log')
 log, current_time = logger.log, logger.current_time
 
 log('Here') # Prints to terminal and saves message to test.log
 ```
 
 ```
-from printr import printr, same_line, current_time
+from printr import print, same_line, current_time
 
 test_list = [{'id': 1, 'name': 'Leanne Graham', 'username': 'Bret', 'email': 'Sincere@april.biz', 'address': {'street': 'Kulas Light', 'suite': 'Apt. 556', 'city': 'Gwenborough', 'zipcode': '92998-3874', 'geo': {'lat': '-37.3159', 'lng': '81.1496'}}, 'phone': '1-770-736-8031 x56442', 'website': 'hildegard.org', 'company': {'name': 'Romaguera-Crona', 'catchPhrase': 'Multi-layered client-server neural-net', 'bs': 'harness real-time e-markets'}}, {'id': 2, 'name': 'Ervin Howell', 'username': 'Antonette', 'email': 'Shanna@melissa.tv', 'address': {'street': 'Victor Plains', 'suite': 'Suite 879', 'city': 'Wisokyburgh', 'zipcode': '90566-7771', 'geo': {'lat': '-43.9509', 'lng': '-34.4618'}}, 'phone': '010-692-6593 x09125', 'website': 'anastasia.net', 'company': {'name': 'Deckow-Crist', 'catchPhrase': 'Proactive didactic contingency', 'bs': 'synergize scalable supply-chains'}}]
 
-printr(test_list) # Formats dictionary with indents
-printr() # Print a line break
+print(test_list) # Formats dictionary with indents
+print() # Print a line break
 same_line('test', current_time=True) # Print the current_time with the message test to the same line
 sleep(1)
 same_line('testing', current_time=True) # Print the current_time with the message testing to the same line
 ```
 
 Output:
 ```
```

