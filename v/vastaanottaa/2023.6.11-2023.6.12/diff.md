# Comparing `tmp/vastaanottaa-2023.6.11.tar.gz` & `tmp/vastaanottaa-2023.6.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vastaanottaa-2023.6.11.tar", last modified: Sun Jun 11 15:26:18 2023, max compression
+gzip compressed data, was "vastaanottaa-2023.6.12.tar", last modified: Sun Jun 11 18:48:40 2023, max compression
```

## Comparing `vastaanottaa-2023.6.11.tar` & `vastaanottaa-2023.6.12.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-11 15:26:18.900881 vastaanottaa-2023.6.11/
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 vastaanottaa-2023.6.11/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 vastaanottaa-2023.6.11/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     3291 2023-06-11 15:26:18.900718 vastaanottaa-2023.6.11/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     2224 2023-06-11 10:48:35.000000 vastaanottaa-2023.6.11/README.md
--rw-r--r--   0 ruth       (501) staff       (20)     2657 2023-06-11 11:45:04.000000 vastaanottaa-2023.6.11/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-11 15:26:18.900923 vastaanottaa-2023.6.11/setup.cfg
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-11 15:26:18.889945 vastaanottaa-2023.6.11/test/
--rw-r--r--   0 ruth       (501) staff       (20)     2487 2023-06-11 15:03:30.000000 vastaanottaa-2023.6.11/test/test_cli.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-11 15:26:18.893523 vastaanottaa-2023.6.11/vastaanottaa/
--rw-r--r--   0 ruth       (501) staff       (20)      641 2023-06-11 15:24:19.000000 vastaanottaa-2023.6.11/vastaanottaa/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      125 2023-06-11 13:17:48.000000 vastaanottaa-2023.6.11/vastaanottaa/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)     2813 2023-06-11 14:59:05.000000 vastaanottaa-2023.6.11/vastaanottaa/cli.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-11 15:26:18.900526 vastaanottaa-2023.6.11/vastaanottaa.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     3291 2023-06-11 15:26:18.000000 vastaanottaa-2023.6.11/vastaanottaa.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)      349 2023-06-11 15:26:18.000000 vastaanottaa-2023.6.11/vastaanottaa.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-11 15:26:18.000000 vastaanottaa-2023.6.11/vastaanottaa.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       54 2023-06-11 15:26:18.000000 vastaanottaa-2023.6.11/vastaanottaa.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)       96 2023-06-11 15:26:18.000000 vastaanottaa-2023.6.11/vastaanottaa.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)       13 2023-06-11 15:26:18.000000 vastaanottaa-2023.6.11/vastaanottaa.egg-info/top_level.txt
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-11 18:48:40.580314 vastaanottaa-2023.6.12/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 vastaanottaa-2023.6.12/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 vastaanottaa-2023.6.12/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3291 2023-06-11 18:48:40.580175 vastaanottaa-2023.6.12/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2224 2023-06-11 10:48:35.000000 vastaanottaa-2023.6.12/README.md
+-rw-r--r--   0 ruth       (501) staff       (20)     2657 2023-06-11 16:15:51.000000 vastaanottaa-2023.6.12/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-11 18:48:40.580349 vastaanottaa-2023.6.12/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-11 18:48:40.576903 vastaanottaa-2023.6.12/test/
+-rw-r--r--   0 ruth       (501) staff       (20)     2458 2023-06-11 18:09:56.000000 vastaanottaa-2023.6.12/test/test_cli.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-11 18:48:40.578048 vastaanottaa-2023.6.12/vastaanottaa/
+-rw-r--r--   0 ruth       (501) staff       (20)      641 2023-06-11 18:47:21.000000 vastaanottaa-2023.6.12/vastaanottaa/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      125 2023-06-11 13:17:48.000000 vastaanottaa-2023.6.12/vastaanottaa/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3715 2023-06-11 18:09:09.000000 vastaanottaa-2023.6.12/vastaanottaa/cli.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-11 18:48:40.580004 vastaanottaa-2023.6.12/vastaanottaa.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3291 2023-06-11 18:48:40.000000 vastaanottaa-2023.6.12/vastaanottaa.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)      349 2023-06-11 18:48:40.000000 vastaanottaa-2023.6.12/vastaanottaa.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-11 18:48:40.000000 vastaanottaa-2023.6.12/vastaanottaa.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       54 2023-06-11 18:48:40.000000 vastaanottaa-2023.6.12/vastaanottaa.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       96 2023-06-11 18:48:40.000000 vastaanottaa-2023.6.12/vastaanottaa.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       13 2023-06-11 18:48:40.000000 vastaanottaa-2023.6.12/vastaanottaa.egg-info/top_level.txt
```

### Comparing `vastaanottaa-2023.6.11/LICENSE` & `vastaanottaa-2023.6.12/LICENSE`

 * *Files identical despite different names*

### Comparing `vastaanottaa-2023.6.11/PKG-INFO` & `vastaanottaa-2023.6.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastaanottaa
-Version: 2023.6.11
+Version: 2023.6.12
 Summary: Receive (Finnish: vastaanottaa) text traversing unknown territories.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/vastaanottaa
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/vastaanottaa
 Project-URL: Documentation, https://codes.dilettant.life/docs/vastaanottaa
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/vastaanottaa
```

### Comparing `vastaanottaa-2023.6.11/README.md` & `vastaanottaa-2023.6.12/README.md`

 * *Files identical despite different names*

### Comparing `vastaanottaa-2023.6.11/pyproject.toml` & `vastaanottaa-2023.6.12/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vastaanottaa"
-version = "2023.6.11"
+version = "2023.6.12"
 description = "Receive (Finnish: vastaanottaa) text traversing unknown territories."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `vastaanottaa-2023.6.11/test/test_cli.py` & `vastaanottaa-2023.6.12/test/test_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,100 +5,100 @@
 SEC = 'Wie schön.'
 SLT = 'n6ihE3dSantzwRwbs/prKw==\n'
 TRG = """\
 Z0FBQUFBQmtoZERaTHN6Yk8tcnhRVFZfYzhPRnJMLWR2Q2Fnb2lRRGk4b0FxdkUyYWh3T3lUcm80
 TFloYTEyTmdfbWJMQXhjblpkX3VSZmxDQ0xRcm5FSEJvZHlzWlNfYXc9PQ==
 """
 
+SLT_NULL = ''
+
 
 def test_cli_send_uc_1(capsys):
     rc = cli.app(['send', SEC, SRC, SLT])
     assert rc == 0
     out, err = capsys.readouterr()
-    assert 'test' in out
-    assert not err
+    assert 'salt provided as parameter' in err
+    assert 'MESSAGE' in out
 
 
 def test_cli_recv_uc_1(capsys):
     rc = cli.app(['recv', SEC, TRG, SLT])
     assert rc == 0
     out, err = capsys.readouterr()
-    assert SLT.split('==', 1)[0] + '==' in out
+    assert 'content' in err
     assert SRC in out
-    assert not err
 
 
 def test_cli_uc_version_1(capsys):
     for arg in ('-V', '--version', 'version'):
         rc = cli.app([arg])
         assert rc == 0
         out, err = capsys.readouterr()
-        assert APP_ALIAS in out
-        assert VERSION in out
-        assert not err
+        assert APP_ALIAS in err
+        assert VERSION in err
+        assert not out
 
 
 def test_cli_uc_help_1(capsys):
     for arg in ('-h', '--help', 'help'):
         rc = cli.app([arg])
         assert rc == 0
         out, err = capsys.readouterr()
-        assert out.startswith('usage: ')
-        assert not err
+        assert 'usage: ' in err
 
 
 def test_cli_uc_short_0(capsys):
     rc = cli.app([])
     assert rc == 0
     out, err = capsys.readouterr()
-    assert out.startswith('usage: ')
-    assert not err
+    assert 'usage: ' in err
+    assert not out
 
 
 def test_cli_ac_short_1(capsys):
     rc = cli.app(['send'])
     assert rc == 2
     out, err = capsys.readouterr()
-    assert 'count' in out
-    assert not err
+    assert 'count' in err
+    assert not out
 
 
 def test_cli_ac_short_2(capsys):
     rc = cli.app(['send', SEC])
     assert rc == 2
     out, err = capsys.readouterr()
-    assert 'count' in out
-    assert not err
+    assert 'count' in err
+    assert not out
 
 
 def test_cli_ac_short_5(capsys):
     rc = cli.app(['send', SEC, 'and', 'wun', 'off'])
     assert rc == 2
     out, err = capsys.readouterr()
-    assert 'count' in out
-    assert not err
+    assert 'count' in err
+    assert not out
 
 
 def test_cli_ab_action(capsys):
     rc = cli.app(['unknown', SEC, SRC, SLT])
     assert rc == 2
     out, err = capsys.readouterr()
-    assert 'goal' in out
-    assert not err
+    assert 'goal' in err
+    assert not out
 
 
 def test_cli_ab_recv_no_salt(capsys):
     rc = cli.app(['recv', SEC, TRG])
     assert rc == 2
     out, err = capsys.readouterr()
-    assert 'salt' in out
-    assert not err
+    assert 'salt' in err
+    assert not out
 
 
 def test_cli_ab_data_zero_bytes(capsys):
     empty_source = 'test/fixtures/basic/empty.src'
     rc = cli.app(['send', SEC, empty_source])
     assert rc == 1
     out, err = capsys.readouterr()
-    assert 'test' not in out
-    assert 'void' in out
-    assert not err
+    assert 'provided' not in err
+    assert 'void' in err
+    assert not out
```

### Comparing `vastaanottaa-2023.6.11/vastaanottaa/__init__.py` & `vastaanottaa-2023.6.12/vastaanottaa/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Receive (Finnish: vastaanottaa) text traversing unknown territories."""
 # [[[fill git_describe()]]]
-__version__ = '2023.6.11+parent.ge41c2001'
-# [[[end]]] (checksum: c75155d15a826e9b48b378a1069fbf16)
+__version__ = '2023.6.12+parent.gf1b5cf69'
+# [[[end]]] (checksum: c65b3f25c3013583a659479eccace65b)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 
 APP_NAME = 'Receive (Finnish: vastaanottaa) text traversing unknown territories.'
 APP_ALIAS = 'vastaanottaa'
 APP_ENV = APP_ALIAS.upper()
```

### Comparing `vastaanottaa-2023.6.11/vastaanottaa/cli.py` & `vastaanottaa-2023.6.12/vastaanottaa/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,102 +1,114 @@
 """Command line interface for vastaanottaa."""
 # import argparse
 import base64
+import datetime as dti
 import os
 import pathlib
 import sys
 import time
 from typing import no_type_check
 
 from cryptography.fernet import Fernet
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
-from vastaanottaa import APP_ALIAS, VERSION
+from vastaanottaa import APP_ALIAS, APP_ENV, VERSION
 
 SEND = 'send'
 RECV = 'recv'
 ACTIONS = (SEND, RECV)
 ENCODING = 'utf-8'
 HASH_ALG = hashes.BLAKE2b
 RES_KEY_LEN = 32
 SALT_LEN = 16
 SALT = os.urandom(SALT_LEN)
 N_ITER = 480000
 
+ARMOR_MSG_BEGIN = f'---- BEGIN {APP_ENV} MESSAGE ----'
+ARMOR_MSG_END = f'---- END {APP_ENV} MESSAGE ----'
+
+ARMOR_SALT_BEGIN = f'---- BEGIN {APP_ENV} SALT ----'
+ARMOR_SALT_END = f'---- END {APP_ENV} SALT ----'
+
+USAGE_INFO = f'usage: {APP_ALIAS} send|recv given text-or-file salt-for-recv'
+
 
 @no_type_check
 def app(argv=None) -> int:
     """Do the thing."""
     argv = sys.argv[1:] if argv is None else argv
 
     if len(argv) == 1 and argv[0] in ('-V', '--version', 'version'):
-        print(f'{APP_ALIAS} v{VERSION}')
+        print(f'{APP_ALIAS} v{VERSION}', file=sys.stderr)
         return 0
 
     if not argv or len(argv) == 1 and argv[0] in ('-h', '--help', 'help'):
-        print(f'usage: {APP_ALIAS} send|recv given text-or-file salt-for-recv')
+        print(USAGE_INFO, file=sys.stderr)
         return 0
 
     if len(argv) not in (3, 4):
-        print('The count!')
+        print('ERROR: unexpected count of parameters', file=sys.stderr)
+        print(USAGE_INFO, file=sys.stderr)
         return 2
     action = argv[0].lower().strip()
     if action not in ACTIONS:
-        print('The goal?')
+        print('ERROR: unexpected goal/action - use either send or recv', file=sys.stderr)
+        print(USAGE_INFO, file=sys.stderr)
         return 2
     given = argv[1].encode(ENCODING)
     src = argv[2]
 
     salt = SALT
-    if len(argv) == 4:
-        print('A test, right?')
+    if action == SEND and len(argv) == 4:
+        print('WARNING: salt provided as parameter for send', file=sys.stderr)
         salt = base64.decodebytes(argv[3].encode(ENCODING))
     if action == RECV:
         if len(argv) != 4:
-            print('The salt!')
+            print('ERROR: salt missing for recv', file=sys.stderr)
+            print(USAGE_INFO, file=sys.stderr)
             return 2
         salt = base64.decodebytes(argv[3].encode(ENCODING))
 
     src_path = pathlib.Path(src)
     if src_path.is_file():
-        print('Reading file ...')
+        print('INFO: Reading content from file', file=sys.stderr)
         src_data = src_path.open('rb').read()
     else:
-        print('Name is content ...')
+        print('INFO: Loading content from parameter', file=sys.stderr)
         src_data = src.encode(ENCODING)
 
     if not src_data:
-        print('Afraid of the void!')
+        print('ERROR: afraid of the void - content for message has zero bytes', file=sys.stderr)
+        print(USAGE_INFO, file=sys.stderr)
         return 1
 
     kdf = PBKDF2HMAC(
         algorithm=HASH_ALG(64),
         length=RES_KEY_LEN,
         salt=salt,
         iterations=N_ITER,
     )
     key = base64.urlsafe_b64encode(kdf.derive(given))
     f = Fernet(key)
     ts = int(time.time())
+    ts_dt = dti.datetime.fromtimestamp(ts, dti.timezone.utc)
 
     if action == SEND:
         token = f.encrypt_at_time(src_data, ts)
         control_ts = f.extract_timestamp(token)
-        print(f'sender: {control_ts=} with {ts=}')
+        control_ts_dt = dti.datetime.fromtimestamp(control_ts, dti.timezone.utc)
+        print(f'DEBUG: timestamp embedded:  {control_ts} ({ts_dt})', file=sys.stderr)
+        print(f'DEBUG: timestamp extracted: {ts} ({control_ts_dt})', file=sys.stderr)
         trp = base64.encodebytes(token)
-        print('encoded:')
-        print(trp.decode(ENCODING))
-        rcv = base64.decodebytes(trp)
-        print(f'receiver: {f.extract_timestamp(rcv)=} with {ts=}')
-        print('data:')
-        print(f.decrypt(rcv).decode(ENCODING))
-        print('# --- 8< ---')
-        print(f'- no pepper but {base64.encodebytes(salt)=}')
+        print(ARMOR_MSG_BEGIN)
+        print(trp.decode(ENCODING), end='')
+        print(ARMOR_MSG_END)
+        print(file=sys.stderr)
+        print(ARMOR_SALT_BEGIN, file=sys.stderr)
+        print(base64.encodebytes(salt), file=sys.stderr)
+        print(ARMOR_SALT_END, file=sys.stderr)
         return 0
 
     rcv = base64.decodebytes(src_data)
-    print(f'receiver: {f.extract_timestamp(rcv)=} with {ts=}')
-    print(f'- using {base64.encodebytes(salt)=}')
-    print('data:')
     print(f.decrypt(rcv).decode(ENCODING))
 
     return 0
```

### Comparing `vastaanottaa-2023.6.11/vastaanottaa.egg-info/PKG-INFO` & `vastaanottaa-2023.6.12/vastaanottaa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastaanottaa
-Version: 2023.6.11
+Version: 2023.6.12
 Summary: Receive (Finnish: vastaanottaa) text traversing unknown territories.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/vastaanottaa
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/vastaanottaa
 Project-URL: Documentation, https://codes.dilettant.life/docs/vastaanottaa
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/vastaanottaa
```

