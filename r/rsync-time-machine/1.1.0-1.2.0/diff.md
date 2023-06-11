# Comparing `tmp/rsync-time-machine-1.1.0.tar.gz` & `tmp/rsync-time-machine-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsync-time-machine-1.1.0.tar", last modified: Sun Jun  4 20:13:32 2023, max compression
+gzip compressed data, was "rsync-time-machine-1.2.0.tar", last modified: Sun Jun 11 20:49:04 2023, max compression
```

## Comparing `rsync-time-machine-1.1.0.tar` & `rsync-time-machine-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-06-04 20:13:32.189652 rsync-time-machine-1.1.0/
--rw-r--r--   0 basnijholt   (501) staff       (20)    11357 2023-05-10 17:54:27.000000 rsync-time-machine-1.1.0/LICENSE
--rw-r--r--   0 basnijholt   (501) staff       (20)    12892 2023-06-04 20:13:32.189329 rsync-time-machine-1.1.0/PKG-INFO
--rw-r--r--   0 basnijholt   (501) staff       (20)    12460 2023-06-04 20:11:35.000000 rsync-time-machine-1.1.0/README.md
--rw-r--r--   0 basnijholt   (501) staff       (20)     2251 2023-05-28 19:34:35.000000 rsync-time-machine-1.1.0/pyproject.toml
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-06-04 20:13:32.184585 rsync-time-machine-1.1.0/rsync_time_machine.egg-info/
--rw-r--r--   0 basnijholt   (501) staff       (20)    12892 2023-06-04 20:13:32.000000 rsync-time-machine-1.1.0/rsync_time_machine.egg-info/PKG-INFO
--rw-r--r--   0 basnijholt   (501) staff       (20)      326 2023-06-04 20:13:32.000000 rsync-time-machine-1.1.0/rsync_time_machine.egg-info/SOURCES.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)        1 2023-06-04 20:13:32.000000 rsync-time-machine-1.1.0/rsync_time_machine.egg-info/dependency_links.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)       63 2023-06-04 20:13:32.000000 rsync-time-machine-1.1.0/rsync_time_machine.egg-info/entry_points.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)       54 2023-06-04 20:13:32.000000 rsync-time-machine-1.1.0/rsync_time_machine.egg-info/requires.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)       19 2023-06-04 20:13:32.000000 rsync-time-machine-1.1.0/rsync_time_machine.egg-info/top_level.txt
--rwxr-xr-x   0 basnijholt   (501) staff       (20)    28867 2023-06-04 20:11:35.000000 rsync-time-machine-1.1.0/rsync_time_machine.py
--rw-r--r--   0 basnijholt   (501) staff       (20)       38 2023-06-04 20:13:32.189724 rsync-time-machine-1.1.0/setup.cfg
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-06-04 20:13:32.188016 rsync-time-machine-1.1.0/tests/
--rw-r--r--   0 basnijholt   (501) staff       (20)    14904 2023-05-28 20:38:17.000000 rsync-time-machine-1.1.0/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:49:04.408450 rsync-time-machine-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 20:48:46.000000 rsync-time-machine-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12892 2023-06-11 20:49:04.408450 rsync-time-machine-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-06-11 20:48:46.000000 rsync-time-machine-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-11 20:48:46.000000 rsync-time-machine-1.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:49:04.408450 rsync-time-machine-1.2.0/rsync_time_machine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12892 2023-06-11 20:49:04.000000 rsync-time-machine-1.2.0/rsync_time_machine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-11 20:49:04.000000 rsync-time-machine-1.2.0/rsync_time_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 20:49:04.000000 rsync-time-machine-1.2.0/rsync_time_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-11 20:49:04.000000 rsync-time-machine-1.2.0/rsync_time_machine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-11 20:49:04.000000 rsync-time-machine-1.2.0/rsync_time_machine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-11 20:49:04.000000 rsync-time-machine-1.2.0/rsync_time_machine.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29159 2023-06-11 20:48:46.000000 rsync-time-machine-1.2.0/rsync_time_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 20:49:04.408450 rsync-time-machine-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:49:04.408450 rsync-time-machine-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14904 2023-06-11 20:48:46.000000 rsync-time-machine-1.2.0/tests/test_app.py
```

### Comparing `rsync-time-machine-1.1.0/LICENSE` & `rsync-time-machine-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rsync-time-machine-1.1.0/PKG-INFO` & `rsync-time-machine-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsync-time-machine
-Version: 1.1.0
+Version: 1.2.0
 Summary: rsync-time-machine.py is a wrapper around rsync to make it easier to create and maintain Time Machine style backups.
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/rsync-time-machine.py
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
```

### Comparing `rsync-time-machine-1.1.0/README.md` & `rsync-time-machine-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rsync-time-machine-1.1.0/pyproject.toml` & `rsync-time-machine-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rsync-time-machine-1.1.0/rsync_time_machine.egg-info/PKG-INFO` & `rsync-time-machine-1.2.0/rsync_time_machine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsync-time-machine
-Version: 1.1.0
+Version: 1.2.0
 Summary: rsync-time-machine.py is a wrapper around rsync to make it easier to create and maintain Time Machine style backups.
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/rsync-time-machine.py
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
```

### Comparing `rsync-time-machine-1.1.0/rsync_time_machine.py` & `rsync-time-machine-1.2.0/rsync_time_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,17 +108,18 @@
         "--rsync-set-flags",
         help="Set the rsync flags that are going to be used for backup.",
     )
     parser.add_argument(
         "--rsync-append-flags",
         help="Append the rsync flags that are going to be used for backup.",
     )
+    log_dir_default = "$HOME/.rsync-time-backup"
     parser.add_argument(
         "--log-dir",
-        default="$HOME/.rsync-time-backup",
+        default=log_dir_default,
         help="Set the log file directory. If this flag is set, generated files will not be managed by the script - in particular they will not be automatically deleted. Default: $HOME/.rsync-time-backup",  # noqa: E501
     )
     parser.add_argument(
         "--strategy",
         default="1:1 30:7 365:30",
         help='Set the expiration strategy. Default: "1:1 30:7 365:30" means after one day, keep one backup per day. After 30 days, keep one backup every 7 days. After 365 days keep one backup every 30 days.',  # noqa: E501
     )
@@ -171,14 +172,16 @@
             " provided. Please use only one of them.",
         )
 
     # If --exclude-from is provided, set exclusion_file to its value
     if args.exclude_from:
         args.exclusion_file = args.exclude_from
 
+    args._auto_delete_log = args.log_dir == log_dir_default
+
     return args
 
 
 def parse_ssh_pattern(
     folder: str,
     *,
     allow_host_only: bool = False,
@@ -277,15 +280,15 @@
 ) -> None:
     """Expire backups according to the expiration strategy."""
     current_timestamp = int(datetime.now().timestamp())
     last_kept_timestamp = 9999999999
     backups = find_backups(dest_folder, ssh)
 
     # We will also keep the oldest backup
-    oldest_backup_to_keep = sorted(backups)[0]
+    oldest_backup_to_keep = sorted(backups)[0] if backups else None
 
     # Process each backup dir from the oldest to the most recent
     for backup_dir in sorted(backups):
         backup_date = os.path.basename(backup_dir)
         backup_timestamp = parse_date_to_epoch(backup_date)
 
         # Skip if failed to parse date...
@@ -393,14 +396,18 @@
     stdout, stderr = await asyncio.gather(
         read_stream(process.stdout, log_info, "magenta"),
         read_stream(process.stderr, log_info, "red"),
     )
 
     await process.wait()
     assert process.returncode is not None, "Process has not returned"
+
+    if VERBOSE and process.returncode != 0:
+        msg = style(str(process.returncode), "red", bold=True)
+        log_error(f"Command exit code: {msg}")
     return CmdResult(stdout, stderr, process.returncode)
 
 
 async def read_stream(
     stream: asyncio.StreamReader,
     callback: Callable[[str], None],
     color: str,
@@ -898,15 +905,15 @@
     VERBOSE = args.verbose
     signal.signal(signal.SIGINT, lambda n, f: terminate_script(n, f))
     backup(
         src_folder=args.src_folder,
         dest_folder=args.dest_folder,
         exclusion_file=args.exclusion_file,
         log_dir=os.path.expandvars(os.path.expanduser(args.log_dir)),
-        auto_delete_log=True,
+        auto_delete_log=args._auto_delete_log,
         expiration_strategy=args.strategy,
         auto_expire=not args.no_auto_expire,
         port=args.port,
         id_rsa=args.id_rsa,
         rsync_set_flags=args.rsync_set_flags,
         rsync_append_flags=args.rsync_append_flags,
         rsync_get_flags=args.rsync_get_flags,
```

### Comparing `rsync-time-machine-1.1.0/tests/test_app.py` & `rsync-time-machine-1.2.0/tests/test_app.py`

 * *Files identical despite different names*

