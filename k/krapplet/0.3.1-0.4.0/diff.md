# Comparing `tmp/krapplet-0.3.1.tar.gz` & `tmp/krapplet-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krapplet-0.3.1.tar", last modified: Sun Feb 21 17:30:00 2021, max compression
+gzip compressed data, was "krapplet-0.4.0.tar", last modified: Sun Jun 11 09:17:14 2023, max compression
```

## Comparing `krapplet-0.3.1.tar` & `krapplet-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,44 @@
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-02-21 17:30:00.124032 krapplet-0.3.1/
--rw-r--r--   0 hfern     (1000) users      (100)     1534 2021-01-16 13:17:35.000000 krapplet-0.3.1/LICENSE
--rw-r--r--   0 hfern     (1000) users      (100)       27 2021-02-21 16:57:53.000000 krapplet-0.3.1/MANIFEST.in
--rw-r--r--   0 hfern     (1000) users      (100)     2338 2021-02-21 17:30:00.124032 krapplet-0.3.1/PKG-INFO
--rw-r--r--   0 hfern     (1000) users      (100)     1093 2021-02-21 16:19:03.000000 krapplet-0.3.1/README.rst
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-02-21 17:30:00.120699 krapplet-0.3.1/krapplet/
--rw-r--r--   0 hfern     (1000) users      (100)      192 2021-02-07 17:27:25.000000 krapplet-0.3.1/krapplet/__init__.py
--rwxr-xr-x   0 hfern     (1000) users      (100)      309 2021-01-17 09:51:16.000000 krapplet-0.3.1/krapplet/__main__.py
--rw-r--r--   0 hfern     (1000) users      (100)    17592 2021-02-21 16:19:03.000000 krapplet-0.3.1/krapplet/kr_pass.py
--rw-r--r--   0 hfern     (1000) users      (100)     1566 2021-02-21 16:19:03.000000 krapplet-0.3.1/krapplet/kr_secretstorage.py
--rwxr-xr-x   0 hfern     (1000) users      (100)    40065 2021-02-21 17:16:50.000000 krapplet-0.3.1/krapplet/krapplet.py
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-02-21 17:30:00.120699 krapplet-0.3.1/krapplet.egg-info/
--rw-r--r--   0 hfern     (1000) users      (100)     2338 2021-02-21 17:29:59.000000 krapplet-0.3.1/krapplet.egg-info/PKG-INFO
--rw-r--r--   0 hfern     (1000) users      (100)      496 2021-02-21 17:29:59.000000 krapplet-0.3.1/krapplet.egg-info/SOURCES.txt
--rw-r--r--   0 hfern     (1000) users      (100)        1 2021-02-21 17:29:59.000000 krapplet-0.3.1/krapplet.egg-info/dependency_links.txt
--rw-r--r--   0 hfern     (1000) users      (100)       53 2021-02-21 17:29:59.000000 krapplet-0.3.1/krapplet.egg-info/entry_points.txt
--rw-r--r--   0 hfern     (1000) users      (100)       51 2021-02-21 17:29:59.000000 krapplet-0.3.1/krapplet.egg-info/requires.txt
--rw-r--r--   0 hfern     (1000) users      (100)        9 2021-02-21 17:29:59.000000 krapplet-0.3.1/krapplet.egg-info/top_level.txt
--rw-r--r--   0 hfern     (1000) users      (100)       14 2020-12-24 18:38:38.000000 krapplet-0.3.1/requirements.txt
--rw-r--r--   0 hfern     (1000) users      (100)     1274 2021-02-21 17:30:00.124032 krapplet-0.3.1/setup.cfg
--rw-r--r--   0 hfern     (1000) users      (100)      238 2021-02-21 16:19:03.000000 krapplet-0.3.1/setup.py
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-02-21 17:30:00.117366 krapplet-0.3.1/share/
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-02-21 17:30:00.120699 krapplet-0.3.1/share/applications/
--rw-r--r--   0 hfern     (1000) users      (100)      241 2020-12-27 09:45:59.000000 krapplet-0.3.1/share/applications/krapplet.desktop
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-02-21 17:30:00.117366 krapplet-0.3.1/share/icons/
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-02-21 17:30:00.117366 krapplet-0.3.1/share/icons/hicolor/
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-02-21 17:30:00.117366 krapplet-0.3.1/share/icons/hicolor/48x48/
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-02-21 17:30:00.124032 krapplet-0.3.1/share/icons/hicolor/48x48/apps/
--rw-r--r--   0 hfern     (1000) users      (100)     9171 2020-12-27 09:53:59.000000 krapplet-0.3.1/share/icons/hicolor/48x48/apps/krapplet.png
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-02-21 17:30:00.117366 krapplet-0.3.1/share/icons/hicolor/96x96/
-drwxr-xr-x   0 hfern     (1000) users      (100)        0 2021-02-21 17:30:00.124032 krapplet-0.3.1/share/icons/hicolor/96x96/apps/
--rw-r--r--   0 hfern     (1000) users      (100)    14596 2020-12-27 09:58:02.000000 krapplet-0.3.1/share/icons/hicolor/96x96/apps/krapplet.png
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 09:17:14.494523 krapplet-0.4.0/
+-rw-r--r--   0 hfern     (1000) users      (100)     1534 2023-06-11 08:47:40.000000 krapplet-0.4.0/LICENSE
+-rw-r--r--   0 hfern     (1000) users      (100)       27 2021-02-24 09:40:04.000000 krapplet-0.4.0/MANIFEST.in
+-rw-r--r--   0 hfern     (1000) users      (100)     1926 2023-06-11 09:17:14.494523 krapplet-0.4.0/PKG-INFO
+-rw-r--r--   0 hfern     (1000) users      (100)     1076 2023-06-11 08:47:40.000000 krapplet-0.4.0/README.md
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 09:17:14.494523 krapplet-0.4.0/krapplet/
+-rw-r--r--   0 hfern     (1000) users      (100)      192 2023-06-11 08:47:40.000000 krapplet-0.4.0/krapplet/__init__.py
+-rwxr-xr-x   0 hfern     (1000) users      (100)      200 2023-06-11 08:47:40.000000 krapplet-0.4.0/krapplet/__main__.py
+-rw-r--r--   0 hfern     (1000) users      (100)    13888 2023-06-11 08:47:40.000000 krapplet-0.4.0/krapplet/kr_backup.py
+-rw-r--r--   0 hfern     (1000) users      (100)     6755 2023-06-11 08:47:40.000000 krapplet-0.4.0/krapplet/kr_crypt.py
+-rw-r--r--   0 hfern     (1000) users      (100)     1817 2023-06-11 08:47:40.000000 krapplet-0.4.0/krapplet/kr_filepicker.py
+-rw-r--r--   0 hfern     (1000) users      (100)     2508 2023-06-11 08:47:40.000000 krapplet-0.4.0/krapplet/kr_json.py
+-rw-r--r--   0 hfern     (1000) users      (100)    15529 2023-06-11 08:47:40.000000 krapplet-0.4.0/krapplet/kr_memstorage.py
+-rw-r--r--   0 hfern     (1000) users      (100)    17393 2023-06-11 08:47:40.000000 krapplet-0.4.0/krapplet/kr_pass.py
+-rw-r--r--   0 hfern     (1000) users      (100)     1904 2023-06-11 08:47:40.000000 krapplet-0.4.0/krapplet/kr_password_entry.py
+-rw-r--r--   0 hfern     (1000) users      (100)     1753 2023-06-11 08:47:40.000000 krapplet-0.4.0/krapplet/kr_popup.py
+-rw-r--r--   0 hfern     (1000) users      (100)     1565 2023-06-11 08:47:40.000000 krapplet-0.4.0/krapplet/kr_secretstorage.py
+-rw-r--r--   0 hfern     (1000) users      (100)     1344 2023-06-11 08:47:40.000000 krapplet-0.4.0/krapplet/kr_storage.py
+-rw-r--r--   0 hfern     (1000) users      (100)     1178 2023-06-11 08:47:40.000000 krapplet-0.4.0/krapplet/kr_storage_select.py
+-rwxr-xr-x   0 hfern     (1000) users      (100)     8873 2023-06-11 08:47:40.000000 krapplet-0.4.0/krapplet/kr_test.py
+-rw-r--r--   0 hfern     (1000) users      (100)      678 2023-06-11 08:47:40.000000 krapplet-0.4.0/krapplet/kr_time.py
+-rwxr-xr-x   0 hfern     (1000) users      (100)    41978 2023-06-11 08:47:40.000000 krapplet-0.4.0/krapplet/krapplet.py
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 09:17:14.494523 krapplet-0.4.0/krapplet.egg-info/
+-rw-r--r--   0 hfern     (1000) users      (100)     1926 2023-06-11 09:17:14.000000 krapplet-0.4.0/krapplet.egg-info/PKG-INFO
+-rw-r--r--   0 hfern     (1000) users      (100)      769 2023-06-11 09:17:14.000000 krapplet-0.4.0/krapplet.egg-info/SOURCES.txt
+-rw-r--r--   0 hfern     (1000) users      (100)        1 2023-06-11 09:17:14.000000 krapplet-0.4.0/krapplet.egg-info/dependency_links.txt
+-rw-r--r--   0 hfern     (1000) users      (100)       52 2023-06-11 09:17:14.000000 krapplet-0.4.0/krapplet.egg-info/entry_points.txt
+-rw-r--r--   0 hfern     (1000) users      (100)       51 2023-06-11 09:17:14.000000 krapplet-0.4.0/krapplet.egg-info/requires.txt
+-rw-r--r--   0 hfern     (1000) users      (100)        9 2023-06-11 09:17:14.000000 krapplet-0.4.0/krapplet.egg-info/top_level.txt
+-rw-r--r--   0 hfern     (1000) users      (100)       82 2023-06-11 08:47:40.000000 krapplet-0.4.0/pyproject.toml
+-rw-r--r--   0 hfern     (1000) users      (100)       14 2020-12-24 18:38:38.000000 krapplet-0.4.0/requirements.txt
+-rw-r--r--   0 hfern     (1000) users      (100)     1240 2023-06-11 09:17:14.494523 krapplet-0.4.0/setup.cfg
+-rw-r--r--   0 hfern     (1000) users      (100)      270 2023-06-11 08:47:40.000000 krapplet-0.4.0/setup.py
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 09:17:14.491189 krapplet-0.4.0/share/
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 09:17:14.494523 krapplet-0.4.0/share/applications/
+-rw-r--r--   0 hfern     (1000) users      (100)      241 2020-12-27 09:45:59.000000 krapplet-0.4.0/share/applications/krapplet.desktop
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 09:17:14.491189 krapplet-0.4.0/share/icons/
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 09:17:14.491189 krapplet-0.4.0/share/icons/hicolor/
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 09:17:14.491189 krapplet-0.4.0/share/icons/hicolor/48x48/
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 09:17:14.494523 krapplet-0.4.0/share/icons/hicolor/48x48/apps/
+-rw-r--r--   0 hfern     (1000) users      (100)     9171 2020-12-27 09:53:59.000000 krapplet-0.4.0/share/icons/hicolor/48x48/apps/krapplet.png
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 09:17:14.491189 krapplet-0.4.0/share/icons/hicolor/96x96/
+drwxr-xr-x   0 hfern     (1000) users      (100)        0 2023-06-11 09:17:14.494523 krapplet-0.4.0/share/icons/hicolor/96x96/apps/
+-rw-r--r--   0 hfern     (1000) users      (100)    14596 2020-12-27 09:58:02.000000 krapplet-0.4.0/share/icons/hicolor/96x96/apps/krapplet.png
```

### Comparing `krapplet-0.3.1/LICENSE` & `krapplet-0.4.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2020-2021 Johannes Willem  Fernhout <hfern@fernhout.info> All rights reserved.
+Copyright 2020-2023 Johannes Willem  Fernhout <hfern@fernhout.info> All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `krapplet-0.3.1/krapplet/kr_pass.py` & `krapplet-0.4.0/krapplet/kr_pass.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 #!/usr/bin/env python3
 
 """
 kr_pass: the krapplet pass storage provider
-(c) 2020-2021 Johannes Willem Fernhout, BSD 3-Clause License applies.
+(c) 2020-2023 Johannes Willem Fernhout, BSD 3-Clause License applies.
 """
 
 import os
 import sys
-import time
-from typing import Dict, Iterator, Optional
-from subprocess import check_output, PIPE, STDOUT
+from typing import Dict, Iterator
+from subprocess import check_output, STDOUT
 
 
 # python-gnupg is a Python wrapper for gpg
 try:
     import gnupg
 except:
     sys.stderr.write("Please install python-gnupg")
     sys.exit(1)
 
-
+"""
 # Assume gtk availability check done in krapplet.py
 import gi
 gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk, GLib, Gdk
+from gi.repository import Gtk
+"""
 
+from .kr_password_entry import show_password_entry_window
 
 HOME_DIR = os.path.expanduser("~")
 DEFAULT_PASSWORD_STORE = HOME_DIR + "/.password-store"
 GPG_ID_FILE = DEFAULT_PASSWORD_STORE + "/.gpg-id"
 PASSWORD_STORE = DEFAULT_PASSWORD_STORE
 VERBOSE = False
 ARMOR = False                         # default no ASCII encoding of secrets
@@ -55,31 +56,30 @@
 class PromptDismissedException(PassException):
     pass
 
 
 def gpg_id():
     """ retrieves the gpg-id from file ${HOME}/.password-store/.gpg-id """
     rval = ""
-    try: 
-        with open(GPG_ID_FILE) as fh:
-            rval = fh.read()
+    try:
+        with open(GPG_ID_FILE) as file_handle:
+            rval = file_handle.read()
     except:
         print("Gpg_id not found")
     return rval
 
 
 def encrypt(unenc: str, recipients: str, passphrase: str) -> str:
     """ Encrypts a string using the passphrase """
     gpg = gnupg.GPG(verbose=VERBOSE, use_agent=False)
     enc = gpg.encrypt(unenc, passphrase=passphrase, sign=True,
                       recipients = recipients, armor = ARMOR)
     if enc.ok:
         return enc.data
-    else:
-        return ""
+    return ""
 
 
 def passwd_test( recipients: str, passphrase: str) -> bool:
     """ tests if we can encrypt a string """
     enc = encrypt("An unecrypted string", recipients, passphrase)
     return len( enc ) > 0
 
@@ -107,26 +107,25 @@
         in fact unlocking the connection """
         if passwd_test(Connection.recipients, Connection.passphrase):
             Connection.passphrase = passphrase
 
     def lock(self) -> None:
         """ Locks a connection by clearing the passphrase """
         Connection.passphrase = ""
-        msg = check_output(["gpgconf", "--reload", "gpg-agent"],
-                           stderr=STDOUT ).decode("utf-8")
+        check_output(["gpgconf", "--reload", "gpg-agent"],
+                      stderr=STDOUT ).decode("utf-8")
 
     def is_locked(self) -> bool:
         """ Returns the current lock state of a connection """
         self.check_validty()
         is_locked = Connection.passphrase == ""
         return is_locked
 
     def close(self) -> None:
-        # ignore, keep class vars for next instance
-        pass
+        """ closes the connection, no action needed actually """
 
 
 def connection_open() -> Connection:
     """ Opens the connection to the pass store, verifies it existence """
     conn = Connection()
     return conn
 
@@ -138,40 +137,41 @@
 
 
 def check_gpg( gpg_id ) -> None:
     """ rudimentary check for a gpg_id, exits when gpg
     command or gpg-id not found """
     return
 
-
+"""
 class PasswordEntryDialog(Gtk.Dialog):
-    """ PasswordEntryDialog: pops up a window to ask for a password """
+    "" PasswordEntryDialog: pops up a window to ask for a password ""
     def __init__(self, parent, title: str, unlock_item: str) -> None:
         Gtk.Dialog.__init__(self, title=title, flags=0)
         self.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL,
                          Gtk.STOCK_OK, Gtk.ResponseType.OK)
         self.set_default_size(150, 100)
         box = self.get_content_area()
         password_prompt = Gtk.Label(label=unlock_item, xalign=0)
         self.passord_entry = Gtk.Entry(xalign = 0, visibility=False)
         self.passord_entry.set_activates_default(True)
         self.set_default_response(Gtk.ResponseType.OK)
         grid = Gtk.Grid(row_spacing=2, column_spacing=5)
         box.add(grid)
         grid.attach_next_to(password_prompt, None,
                             Gtk.PositionType.BOTTOM, 1, 1)
-        grid.attach_next_to(self.passord_entry, password_prompt, 
+        grid.attach_next_to(self.passord_entry, password_prompt,
                             Gtk.PositionType.RIGHT, 1, 1)
         self.show_all()
 
     def get_pw( self ) -> str:
+        "" returns the entered passwd from screen ""
         return self.passord_entry.get_text()
+"""
 
-
-class Key(object):
+class Key():
     """Represents a secret item."""
     def __init__(self, connection, path: str, session = None) -> None:
         self.path = path
         self.session = session
         self.connection = connection
         self.attrs = {}
         self.secret = ""
@@ -185,43 +185,44 @@
     def save_encrypted(self) -> None:
         """ saves key data encrypted"""
         unenc_str = self.secret + "\n"
         for name in self.attrs.keys():
             unenc_str += name + ": " + self.attrs[name] + "\n"
         enc = encrypt(unenc_str, self.connection.recipients,
                       self.connection.get_passphrase())
-        if len(enc): 
+        if len(enc) > 0:
             with open(os.open(self.path,
                               os.O_CREAT | os.O_WRONLY, FILE_PERMISSIONS),
-                      "wb") as fh:
-                fh.write( enc )
+                      "wb") as file_handle:
+                file_handle.write( enc )
 
     def read_encrypted(self) -> bool:
-        gpg = gnupg.GPG(verbose=VERBOSE, use_agent=False)
+        """ reads the key from file """
+        gpg = gnupg.GPG(verbose=VERBOSE, use_agent=False,
+                        options="--ignore-mdc-error")
         passphrase=self.connection.get_passphrase()
-        with open(self.path, 'rb') as f:
-            dec = gpg.decrypt_file(f, passphrase=passphrase)
+        with open(self.path, 'rb') as file_handle:
+            dec = gpg.decrypt_file(file_handle, passphrase=passphrase)
         if dec.ok:
-            _, fname = os.path.split(self.path)
-            label, _ = os.path.splitext(fname)
+            #_, fname = os.path.split(self.path)   # don't think this needed
+            #label, _ = os.path.splitext(fname)
             self.created = self.modified = 0
             lines = str(dec).splitlines()
             secret = ""
             for line in lines:
-                if not len(secret):            # first line contains the secret
+                if len(secret) == 0:           # first line contains the secret
                     secret = line
                     self.secret = secret
                 else:                          # next lines contain the attribs
                     colon_idx = line.find(':')
                     name = line[:colon_idx]
                     val = line[colon_idx+2:]
                     self.attrs[name] = val
             return True
-        else:
-            print("Could not read decrypted file, status:", dec.status)
+        print("Could not read decrypted file, status:", dec.status)
         return False
 
     def is_locked(self) -> bool:
         """Returns :const:`True` if item is locked, otherwise :const:`False`."""
         return self.connection.is_locked()
 
     def ensure_not_locked(self) -> None:
@@ -234,53 +235,50 @@
         """ Lock the connection """
         self.connection.lock()
 
     def unlock(self) -> bool:
         """ to simulate unlocking, a password prompt is showm,
             the password is captured, and with the password we try to decrypt
             the key. Return True if successful, False otherwise """
+
         while self.is_locked():
-            dialog = PasswordEntryDialog(self, title = "Unlock",
-                                         unlock_item = "Passphrase")
-            response = dialog.run()
-            if response == Gtk.ResponseType.OK:
-                self.connection.set_passphrase(dialog.get_pw())
+            passwd = show_password_entry_window()
+            #if len( passwd ) > 0:
+            if passwd != None:
+                self.connection.set_passphrase(passwd)
                 if self.read_encrypted():
-                    dialog.destroy()
                     return True
-                else:
-                    self.lock()
-            elif response == Gtk.ResponseType.CANCEL:
-                dialog.destroy()
-                return False
-            dialog.destroy()
+                self.lock()
+            else:
+                return False           # no entry or escape pressed
 
     def get_attributes(self) -> Dict[str, str]:
         """Returns item attributes (dictionary)."""
         if self.attrs == {}:
             self.read_encrypted()
         return self.attrs
 
     def set_attributes(self, attributes: Dict[str, str]) -> None:
         """ Sets item attributes to attributes """
         self.ensure_not_locked()
         self.attrs = attributes
-        self.save_encrypted() 
+        self.save_encrypted()
 
     def get_label(self) -> str:
+        """ retrieves the label for a key """
         _, fname = os.path.split(self.path)
         label, _ = os.path.splitext(fname )
         return label
 
     def set_label(self, label: str) -> None:
-        """ the label is the last part of the itempath, 
+        """ the label is the last part of the itempath,
         changing the label means renamiing the file """
         self.ensure_not_locked()
         dname, fname = os.path.split(self.path)
-        base, ext = os.path.splitext(fname)
+        _, ext = os.path.splitext(fname)
         new_fname = label + ext
         newpath = os.path.join(dname, new_fname)
         if not self.path == newpath:
             os.rename(self.path, newpath)
             self.path = newpath
 
     def delete(self) -> None:
@@ -295,15 +293,15 @@
             self.read_encrypted()
         return str.encode(self.secret)
 
     def get_secret_content_type(self) -> str:
         """ Not supported as such, therefore always return text/plain """
         return "text/plain"
 
-    def set_secret(self, secret: bytes, 
+    def set_secret(self, secret: bytes,
                    content_type: str = 'text/plain') -> None:
         """Sets secret to `secret`,
            content_type is there for compat reasons, but is ignored """
         self.ensure_not_locked()
         self.secret = secret.decode("utf-8")
         self.save_encrypted()
 
@@ -325,64 +323,63 @@
                 _, fname = os.path.split(self.path)
                 newpath = os.path.join(keyring.path, fname)
                 os.replace(self.path, newpath)
                 self.path = newpath
                 return
 
 
-class Keyring(object):
+class Keyring():
     """Represents a kehyring."""
 
     def __init__(self,
-                 connection: Connection, 
+                 connection: Connection,
                  path: str = DEFAULT_COLLECTION,
                  session = None) -> None:
         self.connection = connection
         self.session = session
         self.path = path
 
     def is_locked(self) -> bool:
-        """Returns :const:`True` if item is locked, otherwise :const:`False`."""
+        """Returns :const:`True` if item is locked,
+           otherwise :const:`False`."""
         is_locked = self.connection.is_locked()
         return is_locked
 
     def ensure_not_locked(self) -> None:
         """If keyring is locked, raises LockedException"""
         if self.is_locked():
             raise LockedException('Keyring is locked!')
 
     def unlock(self) -> bool:
-        """ Attempts to unlock a Keyring, currently not using the gpg-agent """
+        """ Attempts to unlock a Keyring, 
+            currently not using the gpg-agent """
         is_locked = self.is_locked()
         while is_locked:
-            dialog = PasswordEntryDialog(self, title="Unlock",
-                                         unlock_item =  "Passphrase")
-            response = dialog.run()
-            if response == Gtk.ResponseType.OK:
-                passwd = dialog.get_pw()
+            passwd = show_password_entry_window()
+            #if len( passwd ) > 0:
+            if passwd != None:
                 if passwd_test(self.connection.recipients, passwd):
                     self.connection.set_passphrase(passwd)
                 is_locked = self.is_locked()
-            dialog.destroy()
-            if response == Gtk.ResponseType.CANCEL:
+            else:
                 break
         return self.is_locked()
 
     def lock(self) -> None:
         """Locks the keyring."""
         self.connection.lock()
 
     def delete(self) -> None:
         """Deletes the keyringi and all keys attached to it."""
         self.ensure_not_locked()
         for dirname, dirs, files in os.walk(self.path, topdown = False):
-            for d in dirs:
-                os.rmdir(os.path.join(dirname, d))
-            for f in files:
-                os.remove(os.path.join(dirname, f))
+            for directory in dirs:
+                os.rmdir(os.path.join(dirname, directory))
+            for fil in files:
+                os.remove(os.path.join(dirname, fil))
         os.rmdir(self.path)
         self.path = None
 
     def get_all_keys(self) -> Iterator[Key]:
         """Returns a generator of all keys on the keyring."""
         for fname in os.listdir(self.path):
             keypath = os.path.join(self.path, fname)
@@ -395,26 +392,26 @@
             for key in self.get_all_keys():
                 key_attributes = key.get_attributes()
                 for attrib in key_attributes:
                     if attrib == attributes:
                         return key
         else:
             return
-            yield 
+            yield
 
     def get_label(self) -> str:
         """Returns the keyring label."""
         _, label = os.path.split( self.path )
-        return label 
+        return label
 
     def set_label(self, label: str) -> None:
         """ the label is the last part of the keyring path,
             changing the label means renamiing the dir """
         self.ensure_not_locked()
-        path, oldlabel = os.path.split(self.path)
+        path, _ = os.path.split(self.path)
         newpath = os.path.join(path, label)
         if not self.path == newpath:
             os.rename(self.path, newpath)
             self.path = newpath
 
 
     def create_key(self, label: str, attributes: Dict[str, str],
@@ -429,27 +426,26 @@
             key.set_secret(secret)
             key.set_attributes(attributes)
             return key
         return None                     # FIXME: raise an exception ?
 
 
 
-def create_keyring(connection: Connection, label: str, 
+def create_keyring(connection: Connection, label: str,
                    alias: str = '', session = None) -> Keyring:
     """Creates a new keyring and returns it. Alias and session are ignored
     for this implementation it only requires a directory to be created """
 
     path =  os.path.join(DEFAULT_PASSWORD_STORE, label)
     if not os.path.exists(path):
         os.mkdir(path)
     if os.path.isdir(path):
         os.chmod(path, DIR_PERMISSIONS)
         return Keyring(connection, path)
-    else:
-        return None
+    return None
 
 
 def get_all_keyrings(connection) -> Iterator[Keyring]:
     """Returns a generator of all available keyrings."""
     for dname in os.listdir(DEFAULT_PASSWORD_STORE):
         path = os.path.join(DEFAULT_PASSWORD_STORE, dname)
         if os.path.isdir(path):
@@ -457,31 +453,29 @@
 
 
 def get_default_keyring(connection,session = None) -> Keyring:
     """Returns the default keyring. If it doesn't exist, creates it."""
     defaultpath = os.path.join(DEFAULT_PASSWORD_STORE, "default")
     if os.path.isdir(defaultpath):
         return Keyring(connection, defaultpath)
-    else:
-        return Keyring( connection, "default" )
+    return Keyring( connection, "default" )
 
 def get_any_keyring(connection) -> Keyring:
     """Returns any keyring, in the following order of preference:
     - The default keyring;
     - The "session" keyring (usually temporary);
     - The first keyring in the keyring list."""
 
     defaultpath = os.path.join(DEFAULT_PASSWORD_STORE, "default")
     if os.path.isdir(defaultpath):
         return Keyring(connection, defaultpath)
-    else:
-        for entry in os.listdir(DEFAULT_PASSWORD_STORE):
-            path = path.join(DEFAULT_PASSWORD_STORE, entry)
-            if os.path.isdir(path):
-                return Keyring(connection, path)
+    for entry in os.listdir(DEFAULT_PASSWORD_STORE):
+        path = path.join(DEFAULT_PASSWORD_STORE, entry)
+        if os.path.isdir(path):
+            return Keyring(connection, path)
     raise KeyNotFoundException('No keyring found.')
 
 
 def get_keyring_by_alias(connection, alias: str) -> Keyring:
     """Returns the keyring with the given `alias`. If there is no
     such keyring, raises KeyNotFoundException"""
 
@@ -495,8 +489,8 @@
     """Returns a generator of keys in all keyrings with the given
     attributes. `attributes` should be a dictionary."""
     for entry in os.listdir(DEFAULT_PASSWORD_STORE):
         path = os.path.join(DEFAULT_PASSWORD_STORE, entry)
         if os.path.isdir(path):
             keyring = Keyring(connection, path)
             return keyring.search_items(attributes)
-
+    return
```

### Comparing `krapplet-0.3.1/krapplet/kr_secretstorage.py` & `krapplet-0.4.0/krapplet/kr_secretstorage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 """
 kr_secretservice: the krapplet secretservice backend
 This is just a wrapper around secretstorage, other backends should
 implement the same API as secretstorage provides
-(c) 2020-2021 Johannes Willem Fernhout, BSD 3-Clause License applie
+(c) 2020-2023 Johannes Willem Fernhout, BSD 3-Clause License applie
 """
 
 import sys
 
 try:
     import secretstorage
 except:
@@ -43,8 +43,7 @@
             attribs = key.get_attributes()
             secret  = key.get_secret()
             key.delete()
             key = keyring.create_key(label, attribs, secret)
             return key
 
 Key.move = movekey
-
```

### Comparing `krapplet-0.3.1/krapplet/krapplet.py` & `krapplet-0.4.0/krapplet/krapplet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,14 @@
 #!/usr/bin/env python3
 """
 krapplet: A password manager written as a gnome-keyring applet
 krapplet.py is the main program
-(c) 2020-2021 Johannes Willem Fernhout, BSD 3-Clause License applies
+(c) 2020-2023 Johannes Willem Fernhout, BSD 3-Clause License applies
 """
 
-BSD_LICENSE = """
-Copyright 2020-2021 Johannes Willem Fernhout <hfern@fernhout.info>.
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its contributors
-   may be used to endorse or promote products derived from this software
-   without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-ARE DISCLAIMED.  IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
-LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
-SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
-CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
-ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGE."""
-
 # standard Python modules
 import sys
 import os
 import signal
 import string
 import secrets
 import random
@@ -63,149 +33,169 @@
 
 
 # command line parsing to determine the storage provider
 parser = argparse.ArgumentParser( prog = "krapplet",
                                   description = "A password manager")
 
 # currently only gnome-keyring, and pass are supported,
-# ater on sqlite, and keepass will be added
+# later on sqlite, and keepass might be added
 parser.add_argument( "--storage", nargs='?',
-                     default="gnome-keyring", help="gnome-keyring, or pass")
+                     default="gnome-keyring",
+                     help="gnome-keyring, pass, or memory")
 parser.add_argument( "--gpg-id", nargs='?',
                      help="required for pass storage provider")
 parser.add_argument( "--armor", action='store_true',
                      help="ASCII encode secrets")
 cmd_line = parser.parse_args()
+from .kr_storage_select import StorageSelect
+st_sel=StorageSelect(cmd_line.storage, cmd_line.gpg_id, cmd_line.armor)
+from .kr_storage import \
+    connection_open, create_keyring, get_all_keyrings, search_keys, \
+    NotAvailableException, LockedException, KeyNotFoundException, \
+    PromptDismissedException
 
+from .kr_popup import show_error_message, show_info_message
+from . import kr_backup
 
-# import storage backends
-if cmd_line.storage == "gnome-keyring":
-    from krapplet.kr_secretstorage import \
-        connection_open, create_keyring, get_all_keyrings, search_keys, \
-        NotAvailableException, LockedException, KeyNotFoundException, \
-        PromptDismissedException
-elif cmd_line.storage == "pass":
-    from krapplet.kr_pass import \
-        check_gpg, set_armor, connection_open, create_keyring, \
-        get_all_keyrings, search_keys, NotAvailableException, \
-        LockedException, KeyNotFoundException, PromptDismissedException
-    check_gpg(cmd_line.gpg_id)
-    set_armor(cmd_line.armor)
+# application constants:
+BSD_LICENSE = """
+Copyright 2020-2021 Johannes Willem Fernhout <hfern@fernhout.info>.
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification are permitted provided that the following conditions are met:
 
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
 
-# application constants:
-APP_response_delete = 1
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its contributors
+   may be used to endorse or promote products derived from this software
+   without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ARE DISCLAIMED.  IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+POSSIBILITY OF SUCH DAMAGE."""
+APP_RESPONSE_DELETE = 1
 FRAME_LABEL_XALIGN = 0.025
 APP_EMBED_TIMEOUT = 5000                       # 5 seconds
-pw_special_chars = "!#$%&()*+,-./:;<=>?@[\\]^_`{|}~"
-iconname = "krapplet"
-default_pw_len = 16
-__VERSION__ = "0.3.1"
+PW_SPECIAL_CHARS = "!#$%&()*+,-./:;<=>?@[\\]^_`{|}~"
+ICONNAME = "krapplet"
+DEFAULT_PW_LEN = 16
+__VERSION__ = "0.4.0"
 
 
 # utility functions:
 def add_item2menu(mnu=None, label=None, action=None, data=None):
     """ adds a menuitem to a menu (mnu), optionally with an activate action
         and data to be passed to the action """
-    if  mnu == None or label == None:
+    if  mnu is None or label is None:
         print("add_item2menu: mnu nor label can be None", file=sys.stderr)
         raise AssertionError
     mni =  Gtk.MenuItem(label=label)
     if action:
         if data:
             mni.connect("activate", action, data)
         else:
             mni.connect("activate", action)
     mnu.append( mni )
 
 
 def add_separator2menu(mnu):
-     """ add_separator2menu: adds a separator to a menu """
-     mni =  Gtk.SeparatorMenuItem()
-     mnu.append( mni )
-
+    """ add_separator2menu: adds a separator to a menu """
+    mni =  Gtk.SeparatorMenuItem()
+    mnu.append( mni )
 
-def show_info_or_error_message(active_widget, primary_msg, 
+"""
+def show_info_or_error_message(active_widget, primary_msg,
                                secondary_msg, msg_type, title, buttons ):
-    """Shows an error or info  message dialog"""
     dialog = Gtk.MessageDialog(title=title, transient_for=active_widget,
-                               flags=0, message_type=msg_type, 
+                               flags=0, message_type=msg_type,
                                buttons=buttons, text=primary_msg)
     if secondary_msg:
         dialog.format_secondary_text(secondary_msg)
     dialog.run()
     dialog.destroy()
 
 
 def show_error_message(active_widget, primary_msg, secondary_msg):
-    """Shows an error message dialog"""
     show_info_or_error_message(active_widget, primary_msg, secondary_msg,
                                Gtk.MessageType.ERROR, "ERROR",
                                Gtk.ButtonsType.CLOSE)
 
 
 def show_info_message(active_widget, primary_msg, secondary_msg):
-    """ Shows an informational message dialog """
     show_info_or_error_message(active_widget, primary_msg, secondary_msg,
                                Gtk.MessageType.INFO, "Informational",
                                Gtk.ButtonsType.CLOSE)
-
+"""
 
 def abs_path(rel_path):
     """ returns the absolute path for a file,
     given the relative path to this ,py file """
     packagedir = os.path.dirname(__file__)
     joinedpath = os.path.join(packagedir, rel_path)
     path = os.path.abspath(joinedpath)
     return path
 
 
 def icon_path(iconname, res):
     """ finds the path to an icon, based on std Gtk functions,
-    so looking in standard locations like $HOME/.icons, 
+    so looking in standard locations like $HOME/.icons,
     $XDG_DATA_DIRS/icons, and /usr/share/pixmaps """
     icon_theme = Gtk.IconTheme.get_default()
     icon = icon_theme.lookup_icon(iconname, res, 0)
     if icon:
         path = icon.get_filename()
         return path
-    else:
-        print("Krapplet icon "
-              + iconname 
-              + " with resolution "
-              + str(res)
-              + " not found", file=sys.stderr)
-        return ""
+    print("Krapplet icon "
+          + iconname
+          + " with resolution "
+          + str(res)
+          + " not found", file=sys.stderr)
+    return ""
 
 
 def copy_text2clipboard(txt):
     """ copy_text2clipboard copies the txt parameter to the cliboard """
     clipboard = Gtk.Clipboard.get(Gdk.SELECTION_CLIPBOARD)
     clipboard.set_text(txt, -1)
 
 
 def timestamp(since_epoch):
     """returns a string according to local locale
     based on seconds since epoch 1-JAN-1970"""
     if since_epoch:
-        dt = datetime.fromtimestamp(since_epoch)
-        dstr = dt.strftime(locale.nl_langinfo(locale.D_T_FMT))
-        return dstr
-    else:
-        return ""
+        from_timestamp = datetime.fromtimestamp(since_epoch)
+        date_string = from_timestamp.strftime(
+            locale.nl_langinfo(locale.D_T_FMT))
+        return date_string
+    return ""
 
 
-def int2(str):
+def int2(a_string):
+    """ converts string to in, return 0 on failure """
     try:
-        return int(str)
-    except:
+        return int(a_string)
+    except ValueError:
         return 0
 
 
-def sigint_handler(sig, frame):
+def sigint_handler(sig, frame):      # frame is stack frame, and is ignored
     """ Signal handler for SIGINT, or Ctrl-C,
     to avoid standard Python stack dump """
     print("Signal", sig, "received, terminating", file=sys.stderr)
     toplevels = Gtk.Window.list_toplevels()
     for toplevel in toplevels:
         toplevel.destroy()
     Gtk.main_quit()
@@ -214,14 +204,15 @@
 def setup_ccs():
     """ Sets up neccessary cascading style sheets"""
     # FIXME: should come from file, not from memory
     css = """
         levelbar block.weak   { background-color: #FF0000; border: #FF0000; }
         levelbar block.ok     { background-color: #FFA500; border: #FF0000; }
         levelbar block.strong { background-color: #00FF00; border: #FF0000; }
+        button:active         { background-color: #0274d9; }
     """
     css_provider = Gtk.CssProvider()
     css_provider.load_from_data(bytes(css.encode()))
     Gtk.StyleContext.add_provider_for_screen(
         Gdk.Screen.get_default(),
         css_provider,
         Gtk.STYLE_PROVIDER_PRIORITY_APPLICATION
@@ -230,201 +221,216 @@
 
 def password_complexity( passwd):
     """ Calculates password complexity based on the logic found at this
     website: http://passwordstrengthcalculator.com/interpret.php.
     Complexity is the base 2 log of the cardinalty times the password length"""
     if len(passwd) == 0:
         return 0
-    AZ_present = az_present = nm_present = sp_present = False
+    upperc_present = lowerc_present = num_present = special_present = False
     cardinality = 0
-    for ch in passwd:
-        if not AZ_present and ch in string.ascii_uppercase:
+    for char in passwd:
+        if not upperc_present and char in string.ascii_uppercase:
             cardinality += len(string.ascii_uppercase)
-            AZ_present = True
-        elif not az_present and ch in string.ascii_lowercase:
+            upperc_present = True
+        elif not lowerc_present and char in string.ascii_lowercase:
             cardinality += len(string.ascii_lowercase)
-            az_present = True
-        elif not nm_present and ch in string.digits:
+            lowerc_present = True
+        elif not num_present and char in string.digits:
             cardinality += len(string.digits)
-            nm_present = True
-        elif not sp_present and ch in pw_special_chars:
-            cardinality += len(pw_special_chars)
-            sp_present = True
+            num_present = True
+        elif not special_present and char in PW_SPECIAL_CHARS:
+            cardinality += len(PW_SPECIAL_CHARS)
+            special_present = True
     complexity = math.log2(cardinality) * len(passwd)
     return int(complexity)
 
 
-def gen_pw( tot_len, AZ_len, az_len, nm_len, sp_len):
+def gen_pw( tot_len, upperc_len, lowerc_len, numeric_len, special_len):
     """ Returns a generated password based on total lenght, and
     the number of capital, lowercase, numeric and special characters"""
 
     def part_passwd(length, chars):
         """passwd create string of random chars from a set of chars"""
-        pw = ""
-        for i in range(length):
-            pw += secrets.choice(chars)
-        return pw
+        passw = ""
+        #for i in range(length):
+        for _ in range(length):
+            passw += secrets.choice(chars)
+        return passw
 
     def shuffle_word(word):
         """shuffle_word shuffles the letters of a word"""
         word = list(word)
         random.shuffle(word)
         return ''.join(word)
 
-    ex_len = tot_len - AZ_len - az_len - nm_len - sp_len
-    AZ_str = part_passwd(AZ_len, string.ascii_uppercase)
-    az_str = part_passwd(az_len, string.ascii_lowercase)
-    nm_str = part_passwd(nm_len, string.digits)
-    sp_str = part_passwd(sp_len, pw_special_chars)
-    ex_str = ""
-    if ex_len > 0:
-        if AZ_len: ex_str += string.ascii_uppercase
-        if az_len: ex_str += string.ascii_lowercase
-        if nm_len: ex_str += string.digits
-        if sp_len: ex_str += pw_special_chars
-        ex_str = part_passwd(ex_len, ex_str)
-    pw = shuffle_word(AZ_str + az_str + nm_str + sp_str + ex_str)
-    return pw
+    extra_len = tot_len - upperc_len - lowerc_len - numeric_len - special_len
+    upperc_str = part_passwd(upperc_len, string.ascii_uppercase)
+    lowerc_str = part_passwd(lowerc_len, string.ascii_lowercase)
+    numeric_str = part_passwd(numeric_len, string.digits)
+    special_str = part_passwd(special_len, PW_SPECIAL_CHARS)
+    extra_str = ""
+    if extra_len > 0:
+        if upperc_len:
+            extra_str += string.ascii_uppercase
+        if lowerc_len:
+            extra_str += string.ascii_lowercase
+        if numeric_len:
+            extra_str += string.digits
+        if special_len:
+            extra_str += PW_SPECIAL_CHARS
+        extra_str = part_passwd(extra_len, extra_str)
+    passw = shuffle_word(upperc_str
+                      + lowerc_str
+                      + numeric_str
+                      + special_str
+                      + extra_str)
+    return passw
 
 
 class PasswordGeneratorDialog(Gtk.Dialog):
     """ NewPasswordDialog: dialog window to generate a new password """
     def __init__(self, parent ):
         Gtk.Dialog.__init__(self, title="Generate password", flags=0)
-        self.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL, 
+        self.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL,
                          Gtk.STOCK_OK, Gtk.ResponseType.OK)
-        self.tot_len = default_pw_len
-        self.AZ_len = self.az_len = self.nm_len = self.sp_len = 2
+        self.tot_len = DEFAULT_PW_LEN
+        self.upperc_len = 2
+        self.lowerc_len = 2
+        self.numeric_len = 2
+        self.special_len = 2
         self.show_window()
         self.set_transient_for(parent)
 
     def show_window( self ):
         """ show_window builds up a window based on the values i
             of self.new_keyname/new_attribs/new_secret """
 
         self.set_default_size(100, 100)
         box = self.get_content_area()
         frame = Gtk.Frame(label="Parameters", label_xalign=FRAME_LABEL_XALIGN)
         box.add(frame)
-        self.grid = Gtk.Grid(row_spacing=2, column_spacing=5) 
+        self.grid = Gtk.Grid(row_spacing=2, column_spacing=5)
         frame.add(self.grid)
 
         prompt_length = Gtk.Label(label="Total length", xalign=0)
         self.entry_lenght = Gtk.Entry( text=str(self.tot_len), \
                                        input_purpose=Gtk.InputPurpose.DIGITS,
                                        xalign=0, width_request=3 )
         self.entry_lenght.connect("insert_text", self.validate, 2)
-        prompt_AZ = Gtk.Label(label="Uppercase", xalign=0)
-        self.entry_AZ = Gtk.Entry(text=str(self.AZ_len),
+        prompt_upperc = Gtk.Label(label="Uppercase", xalign=0)
+        self.entry_upperc = Gtk.Entry(text=str(self.upperc_len),
                                   input_purpose=Gtk.InputPurpose.DIGITS,
                                   xalign=0)
-        self.entry_AZ.connect("insert_text", self.validate, 2)
-        prompt_az = Gtk.Label(label="Lowercase", xalign=0)
-        self.entry_az = Gtk.Entry(text=str(self.az_len),
+        self.entry_upperc.connect("insert_text", self.validate, 2)
+        prompt_lowerc = Gtk.Label(label="Lowercase", xalign=0)
+        self.entry_lowerc = Gtk.Entry(text=str(self.lowerc_len),
                                   input_purpose=Gtk.InputPurpose.DIGITS,
                                   xalign=0 )
-        self.entry_az.connect("insert_text", self.validate, 2)
-        prompt_nm = Gtk.Label(label="Numeric", xalign=0)
-        self.entry_nm = Gtk.Entry(text=str(self.nm_len),
+        self.entry_lowerc.connect("insert_text", self.validate, 2)
+        prompt_numeric = Gtk.Label(label="Numeric", xalign=0)
+        self.entry_numeric = Gtk.Entry(text=str(self.numeric_len),
                                   input_purpose=Gtk.InputPurpose.DIGITS,
                                   xalign=0 )
-        self.entry_nm.connect("insert_text", self.validate, 2)
-        prompt_sp = Gtk.Label(label="special", xalign=0)
-        self.entry_sp = Gtk.Entry(text=str(self.sp_len), \
+        self.entry_numeric.connect("insert_text", self.validate, 2)
+        prompt_special = Gtk.Label(label="special", xalign=0)
+        self.entry_special = Gtk.Entry(text=str(self.special_len),
                                   input_purpose=Gtk.InputPurpose.DIGITS,
                                   xalign=0 )
-        self.entry_sp.connect("insert_text", self.validate, 2)
+        self.entry_special.connect("insert_text", self.validate, 2)
         empty_line = Gtk.Label()
 
         self.grid.attach_next_to(prompt_length, None,
                                  Gtk.PositionType.BOTTOM, 1, 1)
         self.grid.attach_next_to(self.entry_lenght, prompt_length,
                                  Gtk.PositionType.RIGHT, 1, 1)
-        self.grid.attach_next_to(prompt_AZ, prompt_length,
+        self.grid.attach_next_to(prompt_upperc, prompt_length,
                                  Gtk.PositionType.BOTTOM, 1, 1)
-        self.grid.attach_next_to(self.entry_AZ, prompt_AZ,
+        self.grid.attach_next_to(self.entry_upperc, prompt_upperc,
                                  Gtk.PositionType.RIGHT, 1, 1)
-        self.grid.attach_next_to(prompt_az, prompt_AZ,
+        self.grid.attach_next_to(prompt_lowerc, prompt_upperc,
                                  Gtk.PositionType.BOTTOM, 1, 1)
-        self.grid.attach_next_to(self.entry_az, prompt_az,
+        self.grid.attach_next_to(self.entry_lowerc, prompt_lowerc,
                                  Gtk.PositionType.RIGHT, 1, 1)
-        self.grid.attach_next_to(prompt_nm, prompt_az,
+        self.grid.attach_next_to(prompt_numeric, prompt_lowerc,
                                  Gtk.PositionType.BOTTOM, 1, 1)
-        self.grid.attach_next_to(self.entry_nm, prompt_nm,
+        self.grid.attach_next_to(self.entry_numeric, prompt_numeric,
                                  Gtk.PositionType.RIGHT, 1, 1)
-        self.grid.attach_next_to(prompt_sp, prompt_nm,
+        self.grid.attach_next_to(prompt_special, prompt_numeric,
                                  Gtk.PositionType.BOTTOM, 1, 1)
-        self.grid.attach_next_to(self.entry_sp, prompt_sp,
+        self.grid.attach_next_to(self.entry_special, prompt_special,
                                  Gtk.PositionType.RIGHT, 1, 1)
         box.add( empty_line )
         self.show_all()
 
     def update_from_window( self ):
+        """ updates instance vars from window """
         self.tot_len = int2(self.entry_lenght.get_text())
-        self.AZ_len = int2(self.entry_AZ.get_text())
-        self.az_len = int2(self.entry_az.get_text())
-        self.nm_len = int2(self.entry_nm.get_text())
-        self.sp_len = int2(self.entry_sp.get_text())
+        self.upperc_len = int2(self.entry_upperc.get_text())
+        self.lowerc_len = int2(self.entry_lowerc.get_text())
+        self.numeric_len = int2(self.entry_numeric.get_text())
+        self.special_len = int2(self.entry_special.get_text())
 
     def validate(self, widget, new_text, new_text_length, position, maxlen ):
         """ validates keyboard input for numberic, and nrof digits, and
             enables/disables the OK button based on the input given"""
         field_contents = widget.get_text()
-        newpos = widget.get_position() 
-        if (new_text.isnumeric() 
+        newpos = widget.get_position()
+        if (new_text.isnumeric()
             and (new_text_length + len(field_contents)) <= maxlen):
             field_contents = (field_contents[:newpos]
                               + new_text
                               + field_contents[newpos:])
         widget.handler_block_by_func(self.validate)
         widget.set_text(field_contents)
         widget.handler_unblock_by_func(self.validate)
         GLib.idle_add(widget.set_position, newpos+1)
         widget.stop_emission_by_name("insert_text")
         self.update_from_window()
-        enabled = ((self.tot_len >= (self.AZ_len + self.az_len
-                                     + self.nm_len + self.sp_len))
-                   and (self.AZ_len or self.az_len
-                        or self.nm_len or self.sp_len ))
+        enabled = ((self.tot_len >= (self.upperc_len + self.lowerc_len
+                                     + self.numeric_len + self.special_len))
+                   and (self.upperc_len or self.lowerc_len
+                        or self.numeric_len or self.special_len ))
         self.set_response_sensitive( Gtk.ResponseType.OK, enabled )
 
     def generate_new_password(self):
+        """ Returns a newly generated passwd """
         self.update_from_window()
-        pw = gen_pw(self.tot_len, self.AZ_len,
-                    self.az_len, self.nm_len, self.sp_len)
-        return pw
+        passwd = gen_pw(self.tot_len, self.upperc_len,
+                        self.lowerc_len, self.numeric_len, self.special_len)
+        return passwd
 
 
 class KeyDialog(Gtk.Dialog):
     """ KeyDialog: shows a dialog window for keys """
     def __init__(self, parent, key=None, keyring=None):
         Gtk.Dialog.__init__(self, title="Edit key", flags=0 )
-        self.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL, 
-                         Gtk.STOCK_DELETE, APP_response_delete,
+        self.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL,
+                         Gtk.STOCK_DELETE, APP_RESPONSE_DELETE,
                          Gtk.STOCK_OK, Gtk.ResponseType.OK)
         self.key = key
         self.keyring = keyring
         self.extra_attribs = 0
         self.out_of_focus_handler = None
         if self.key:
             self.old_keyring_label = self.new_keyring_label = key.keyring_label
             self.old_keyname = self.new_keyname = key.get_label()
             self.old_attribs = self.new_attribs = key.get_attributes()
-            self.old_secret = self.new_secret = key.get_secret().decode("utf-8") 
+            self.old_secret = self.new_secret = key.get_secret().decode("utf-8")
             self.old_created = key.get_created()
             self.old_modified= key.get_modified()
             self.connection = self.key.connection
         else:
             self.old_keyring_label = self.new_keyring_label = keyring.get_label()
             self.old_keyname = self.new_keyname = "New key"
             self.old_attribs = self.new_attribs = {}
             self.new_attribs["URL"] = "https://"
             self.new_attribs["username"] = ""
             self.new_attribs["validity"] = "90"
-            self.old_secret = self.new_secret = gen_pw(default_pw_len, 2, 2, 2, 2)
+            self.old_secret = self.new_secret = gen_pw(DEFAULT_PW_LEN,
+                                                       2, 2, 2, 2)
             self.old_created = self.old_modified = 0
             self.connection = keyring.connection
         self.secret_visibilty = False
         self.box = None
         self.show_window()
 
     def show_window( self ):
@@ -436,47 +442,47 @@
             self.box.destroy()
         self.box = Gtk.Box(orientation = Gtk.Orientation.VERTICAL)
         content_area.add(self.box)
 
         keyring_frame = Gtk.Frame(label="Keyring",
                                   label_xalign=FRAME_LABEL_XALIGN)
         keyring_box = Gtk.Box(orientation = Gtk.Orientation.VERTICAL)
-        self.box.add(keyring_frame) 
+        self.box.add(keyring_frame)
         keyring_frame.add(keyring_box)
         self.newkeyring_combo = Gtk.ComboBoxText()
         idx = active_idx = 0
         keyrings = get_all_keyrings(self.connection)
         for keyring in keyrings:
             keyring_label = keyring.get_label()
-            if len(keyring_label):
+            if len(keyring_label) > 0:
                 self.newkeyring_combo.append_text(keyring_label)
                 if keyring_label == self.new_keyring_label:
                     self.keyring = keyring
                     active_idx = idx
                 idx += 1
         self.newkeyring_combo.set_active(active_idx)
         keyring_box.pack_start(self.newkeyring_combo, True, True, 0)
 
         key_frame = Gtk.Frame(label="Key", label_xalign=FRAME_LABEL_XALIGN)
-        key_grid = Gtk.Grid(row_spacing=2, column_spacing=5) 
-        self.box.add(key_frame) 
+        key_grid = Gtk.Grid(row_spacing=2, column_spacing=5)
+        self.box.add(key_frame)
         key_frame.add(key_grid)
 
         self.newkey_entry = Gtk.Entry(text=self.new_keyname,xalign=0)
         self.newkey_entry.set_max_width_chars(64)
-        key_grid.attach_next_to(self.newkey_entry, None, 
+        key_grid.attach_next_to(self.newkey_entry, None,
                                 Gtk.PositionType.RIGHT, 2, 1)
         last_prompt = self.newkey_entry
 
         if self.old_created:
             if self.old_created != self.old_modified:
                 created_prompt = Gtk.Label(label="Created", xalign=0)
                 created_value  = Gtk.Label(label=timestamp( self.old_created),
                                                             xalign=0)
-                key_grid.attach_next_to(created_prompt, last_prompt, 
+                key_grid.attach_next_to(created_prompt, last_prompt,
                                         Gtk.PositionType.BOTTOM, 1, 1)
                 key_grid.attach_next_to(created_value, created_prompt,
                                         Gtk.PositionType.RIGHT, 1, 1)
                 last_prompt = created_prompt
             modified_prompt = Gtk.Label(label=" Modified", xalign=0)
             modified_value  = Gtk.Label(label=timestamp( self.old_modified ),
                                                          xalign=0)
@@ -485,28 +491,28 @@
             key_grid.attach_next_to(modified_value, modified_prompt,
                                     Gtk.PositionType.RIGHT, 1, 1)
             last_prompt = modified_prompt
 
         self.box.add( Gtk.Label())
         attr_frame = Gtk.Frame(label="Attributes",
                                label_xalign=FRAME_LABEL_XALIGN)
-        attr_grid = Gtk.Grid(row_spacing=2, column_spacing=5) 
+        attr_grid = Gtk.Grid(row_spacing=2, column_spacing=5)
         self.box.add(attr_frame)
         attr_frame.add(attr_grid)
         self.attr_prompt = {}
         self.attr_value  = {}
         last_prompt = None
         launch_button_active = False
         expiry_check = False
         for attr in self.new_attribs:
             if  attr != "xdg:schema":
                 self.attr_prompt[attr] = Gtk.Entry(text=attr, xalign=0,
                                                    max_width_chars=20)
                 self.attr_prompt[attr].set_max_width_chars(20)
-                self.attr_value[attr]  = Gtk.Entry(text=self.new_attribs[attr], 
+                self.attr_value[attr]  = Gtk.Entry(text=self.new_attribs[attr],
                                                    xalign = 0)
                 self.attr_value[attr].set_max_width_chars( 42 )
                 attr_grid.attach_next_to(self.attr_prompt[attr], last_prompt,
                                          Gtk.PositionType.BOTTOM, 1, 1 )
                 attr_grid.attach_next_to(self.attr_value[attr],
                                          self.attr_prompt[attr],
                                          Gtk.PositionType.RIGHT, 1, 1)
@@ -555,15 +561,15 @@
                 expiring = True
                 label = '<span foreground="orange" weight="bold">Expiring secret</span>'
                 secr_frame_label = label
         secr_frame = Gtk.Frame(label=secr_frame_label,
                                label_xalign=FRAME_LABEL_XALIGN)
         if expiring or expired:
             secr_frame.get_label_widget().set_use_markup(True)
-        secr_grid = Gtk.Grid(row_spacing=2, column_spacing=5) 
+        secr_grid = Gtk.Grid(row_spacing=2, column_spacing=5)
         self.box.add(secr_frame)
         secr_frame.add(secr_grid)
         self.secret_value = Gtk.Entry(text=self.new_secret, xalign=0,
                                       visibility=self.secret_visibilty)
         self.secret_value.connect("changed", self.update_complexity_levelbar)
         self.secret_value.set_max_width_chars(64)
         self.complexity_levelbar = Gtk.LevelBar()
@@ -614,15 +620,15 @@
         self.secret_visibilty = False
         self.show_window()
 
     def launch(self, button):
         """ tries to find an attrib["URL"] and lauches it in a webbrowser """
         self.update_key_from_window()
         url = self.new_attribs["URL"]
-        webbrowser.open(url, new=0, autoraise=True) 
+        webbrowser.open(url, new=0, autoraise=True)
         self.out_of_focus_handler = self.connect("focus-out-event",
                                                  self.refocus)
 
     def refocus(self, widget, event):
         """ Tries to grab focus back after we lost it due to lauching an URL """
         self.present()
         if self.out_of_focus_handler:
@@ -644,83 +650,102 @@
             prompt = self.extra_attr_prompt.get_text()
             if prompt != "":
                 value  = self.extra_attr_entry.get_text()
                 screen_attribs[prompt] = value
             self.extra_attribs = False
         self.new_secret = self.secret_value.get_text()
         self.new_attribs = screen_attribs
-            
+
     def toggle_secret_visibility(self, button):
         """ toggles the visibiity of the password """
         self.update_key_from_window()
         self.secret_visibilty = not self.secret_visibilty
         self.show_window()
 
     def add_attr(self, button):
         """ adds an attribute line to the window """
         self.update_key_from_window()
         self.extra_attribs = True
         self.show_window()
 
     def copy_secret2clipboard(self, widget):
+        " copies the secret from screen to the clipboard """
         self.update_key_from_window()
         copy_text2clipboard(self.new_secret)
 
     def deletekey(self):
-        self.key.delete()
+        """ Deletes a key """
+        dialog = Gtk.Dialog(title="Delete key", flags=0)
+        dialog.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL,
+                         Gtk.STOCK_OK, Gtk.ResponseType.OK)
+        dialog.set_default_size(150, 100)
+        content_area = dialog.get_content_area()
+        box = Gtk.Box(orientation = Gtk.Orientation.VERTICAL)
+        box.pack_start(Gtk.Label(), True, True, 0)
+        box.pack_start(Gtk.Label(label="  Are you sure to delete key '"
+                                + self.old_keyname
+                                + "' ?  "), True, True, 0)
+        content_area.add(box)
+        dialog.show_all()
+        response = dialog.run()
+        if response == Gtk.ResponseType.OK:
+            self.key.delete()
+        dialog.destroy()
 
     def savekey(self):
+        """ Saves a key """
         self.update_key_from_window()
         if self.old_keyname != self.new_keyname:
             self.key.set_label(self.new_keyname)
         if self.old_attribs != self.new_attribs:
             self.key.set_attributes(self.new_attribs)
         if self.old_secret != self.new_secret:
             self.key.set_secret(self.new_secret.encode("utf-8"))
         if self.keyring and self.old_keyring_label != self.new_keyring_label:
             self.key.move(self.new_keyring_label)
 
     def create_newkey( self, keyring):
+        """ Creates a new key """
         self.update_key_from_window()
         self.key = keyring.create_key( label=self.new_keyname,
-                                       attributes=self.new_attribs, 
+                                       attributes=self.new_attribs,
                                        secret=self.new_secret.encode("utf-8"))
 
 
 class AddKeyRingDialog(Gtk.Dialog):
     """ AddKeyRingDialog: window class to add a keyring,
         prompts for keyring name """
     def __init__(self, parent):
         Gtk.Dialog.__init__(self, title="New keyring", flags=0)
-        self.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL, 
+        self.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL,
                          Gtk.STOCK_OK, Gtk.ResponseType.OK)
         self.set_default_size(150, 100)
         box = self.get_content_area()
         keyringname_prompt = Gtk.Label(label="Keyring name", xalign=0)
         self.keyringname_input = Gtk.Entry(text="New keyring", xalign = 0)
-        grid = Gtk.Grid(row_spacing=2, column_spacing=5) 
+        grid = Gtk.Grid(row_spacing=2, column_spacing=5)
         box.add(grid)
         grid.attach_next_to(keyringname_prompt, None,
                             Gtk.PositionType.BOTTOM, 1, 1)
         grid.attach_next_to(self.keyringname_input, keyringname_prompt,
                             Gtk.PositionType.RIGHT, 1, 1)
         self.set_position(Gtk.WindowPosition.MOUSE)
         self.show_all()
 
     def get_newkeyringname(self):
         """ get_newkeyringname: returns the entered name for a new keyring"""
-        return self.keyringname_input.get_text() 
+        return self.keyringname_input.get_text()
 
 
 class StatusIcon:
     """Main entry point, creates a tray icon, and handles rightclicks"""
     def __init__(self):
         self.dbus_open = False
         self.statusicon = Gtk.StatusIcon()
-        self.statusicon.set_from_file( icon_path(iconname, 48))
+        self.statusicon.set_from_file( icon_path(ICONNAME, 48))
         self.statusicon.connect("popup-menu", self.right_click_event)
         self.statusicon.set_title("Password manager")
         self.statusicon.set_tooltip_text("krapplet: a password manager")
         self.statusicon.set_visible(True)
         self.embedded = False
         GLib.idle_add(self.embed_check)
         GLib.timeout_add(APP_EMBED_TIMEOUT, self.embed_timeout)
@@ -733,29 +758,28 @@
             return False                    # don't call again
         return True
 
     def embed_timeout(self):
         """ if still not emebedded then exit program """
         if self.embedded:
             return False                    # don't call again
-        else:
-            print("Error: could not embed in systray", file=sys.stderr)
-            Gtk.main_quit()
-            return True
+        print("Error: could not embed in systray", file=sys.stderr)
+        Gtk.main_quit()
+        return True
 
     def right_click_event(self, icon, button, time):
         """ shows the popop menu """
         if self.active_widget:
             self.active_widget.present()
             return
         if self.dbus_open:
             self.connection.close()
         self.connection = connection_open()
         self.dbus_open = True
-        self.menu = Gtk.Menu() 
+        self.menu = Gtk.Menu()
         self.keyrings = get_all_keyrings(self.connection)
         self.keyring_labels = []
         for keyring in self.keyrings:
             keyring_label = keyring.get_label()
             if len(keyring_label):
                 item = Gtk.MenuItem(label=keyring_label)
                 submenu = Gtk.Menu()
@@ -782,42 +806,47 @@
                             key.keyring_labels = self.keyring_labels
                             add_item2menu(mnu=submenu, label=key.get_label(),
                                           action=self.key_dialog, data=key)
                             nrof_keys += 1
                     except KeyNotFoundException:
                         show_error_message(
                             self.active_widget,
-                            "Key not found exception", 
+                            "Key not found exception",
                             "Restarting gnome-keyring; this will lock all keyrings" )
                         msg = subprocess.check_output(
                             ["gnome-keyring-daemon", "-r", "-d"],
                             stderr=subprocess.STDOUT )
                         show_info_message(
                              self.active_widget,
                              "Output of gnome-restart command",
                              msg.decode("utf-8"))
                     except:
-                        show_error_message(
-                             self.active_widget, 
+                        print( "class sys.exc_info()[0]:" , sys.exc_info()[0].__class__)
+                        """show_error_message(
+                             self.active_widget,
                              "Unexpected error occured, please report this error",
-                             sys.exc_info()[0])
-                    if nrof_keys: 
+                             sys.exc_info()[0]) """
+                    if nrof_keys:
                         add_separator2menu(submenu)
                     add_item2menu(mnu=submenu, label="Add key",
                                   action=self.add_key, data=keyring)
                     if  not nrof_keys:
                         add_item2menu(mnu=submenu, label="Remove keyring",
                                       action=self.remove_keyring, data=keyring)
                     add_item2menu(mnu=submenu, label="Lock keyring",
                                   action=self.lock_keyring, data=keyring )
                 item.set_submenu(submenu)
                 self.menu.append(item)
         add_separator2menu( self.menu )
         add_item2menu(mnu=self.menu, label="Add keyring",
                       action=self.add_keyring, data=None)
+        add_item2menu(mnu=self.menu, label="Backup",
+                      action=self.backup, data=None)
+        add_item2menu(mnu=self.menu, label="Restore",
+                      action=self.restore, data=None)
         add_item2menu(mnu=self.menu, label="About",
                       action=self.show_about_dialog, data=None)
         add_item2menu(mnu=self.menu, label="Quit",
                       action=Gtk.main_quit, data=None)
         self.menu.show_all()
         self.menu.popup(None, None, None, self.statusicon, button, time)
 
@@ -832,43 +861,43 @@
     def remove_keyring(self, widget, keyring):
         """Removes a keyring, when it is empty.
         If not it shows an error message"""
         keycount = 0
         for key in keyring.get_all_keys():
             keycount += 1
         if keycount:
-            show_error_message(self.active_widget, 
-                               "Error deleting  keyring", 
+            show_error_message(self.active_widget,
+                               "Error deleting  keyring",
                                "Keys are still attached to keyring" )
         else:
             keyring.delete()
 
     def key_dialog(self, widget, key):
         """Pops up a window showing a key, with all the attribs"""
         if not key.is_locked():               # check check double check
             self.active_widget = dialog = KeyDialog(self, key=key)
             response = dialog.run()
             if response == Gtk.ResponseType.OK:
                 dialog.savekey()
-            elif response == APP_response_delete:
+            elif response == APP_RESPONSE_DELETE:
                 dialog.deletekey()
             copy_text2clipboard("")
             dialog.destroy()
             self.active_widget = None
         else:
             show_error_message(self.active_widget,
                                "Key locked", key.get_label() )
 
     def add_key(self, widget, keyring):
         """Add_key adds a key to a keyrng"""
         self.active_widget = dialog = KeyDialog(self, keyring=keyring)
         response = dialog.run()
         if response == Gtk.ResponseType.OK:
             dialog.create_newkey(keyring)
-        dialog.destroy() 
+        dialog.destroy()
         self.active_widget = None
 
     def add_keyring(self, widget):
         """Pops up a window asking for a new keyring name"""
         self.active_widget = dialog = AddKeyRingDialog(self)
         response = dialog.run()
         if response == Gtk.ResponseType.OK:
@@ -877,39 +906,45 @@
                 create_keyring(self.connection, keyringname)
             except Exception as e:
                 show_error_message(self.active_widget,
                                    "Error saving new keyring", str( e ))
         dialog.destroy()
         self.active_widget = None
 
+    def backup(self, widget):
+        kr_backup.backup()
+
+    def restore(self, widget):
+        kr_backup.restore()
+
     def show_about_dialog(self, widget):
         """Shows the about dialog"""
         image = Gtk.Image()
-        image.set_from_file(icon_path( iconname, 96))
+        image.set_from_file(icon_path( ICONNAME, 96))
         icon_pixbuf = image.get_pixbuf()
         self.active_widget = about_dialog = Gtk.AboutDialog()
         about_dialog.set_destroy_with_parent(True)
         about_dialog.set_logo(icon_pixbuf)
         about_dialog.set_program_name("krapplet")
         about_dialog.set_version("Version " + __VERSION__)
-        about_dialog.set_comments("A password manager written as a gnome-keyring applet")
+        about_dialog.set_comments("A password manager using gnome-keyring or pass")
         about_dialog.set_authors(["Johannes Willem Fernhout"])
-        about_dialog.set_copyright( "(c) 2020-2021 Johannes Willem Fernhout")
+        about_dialog.set_copyright( "(c) 2020-2022 Johannes Willem Fernhout")
         about_dialog.set_license(BSD_LICENSE)
         about_dialog.set_website("https://gitlab.com/hfernh/krapplet")
         about_dialog.set_website_label("krapplet on GitLab")
         about_dialog.show_all()
         about_dialog.run()
         about_dialog.destroy()
         self.active_widget = None
 
     def __del__(self):
         """ exit code, just some housekeeping """
         if self.dbus_open:
-            self.connection.close() 
+            self.connection.close()
 
 
 def main():
     """ krapplet main """
     # ignore GTK deprecation warnings gwhen not in development mode
     # for development mode, run program as python3 -X dev krapplet
     if not sys.warnoptions:
```

### Comparing `krapplet-0.3.1/setup.cfg` & `krapplet-0.4.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [metadata]
 name = krapplet
 version = attr: krapplet.krapplet.__VERSION__
 description = A password manager written as a gnome-keyring applet
-long_description = file: README.rst
-long_description_content_type = text/x-rst
+long_description = file: README.md
+long_description_content_type = text/markdown
 author = Johannes Willem Fernhout
 author_email = hfern@fernhout.info
 url = https://gitlab.com/hfernh/krapplet
 license = BSD 3-Clause License
 license_file = LICENSE
 keywords = password manager, gnome-keyring, pass
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: BSD License
 	Operating System :: POSIX
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Security
 	Topic :: Utilities
 platforms = Linux
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.10
 packages = find:
 
 [options.data_files]
 share/applications = share/applications/krapplet.desktop
 share/icons/hicolor/48x48/apps = share/icons/hicolor/48x48/apps/krapplet.png
 share/icons/hicolor/96x96/apps = share/icons/hicolor/96x96/apps/krapplet.png
```

### Comparing `krapplet-0.3.1/share/icons/hicolor/48x48/apps/krapplet.png` & `krapplet-0.4.0/share/icons/hicolor/48x48/apps/krapplet.png`

 * *Files identical despite different names*

### Comparing `krapplet-0.3.1/share/icons/hicolor/96x96/apps/krapplet.png` & `krapplet-0.4.0/share/icons/hicolor/96x96/apps/krapplet.png`

 * *Files identical despite different names*

