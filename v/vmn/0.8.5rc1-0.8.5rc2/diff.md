# Comparing `tmp/vmn-0.8.5rc1-py3-none-any.whl.zip` & `tmp/vmn-0.8.5rc2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 45476 bytes, number of entries: 10
+Zip file size: 45615 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      152 b- defN 21-Jul-06 16:25 version_stamp/__init__.py
--rw-r--r--  2.0 unx    53161 b- defN 23-May-09 13:41 version_stamp/stamp_utils.py
--rw-r--r--  2.0 unx       58 b- defN 23-May-09 13:43 version_stamp/version.py
--rw-r--r--  2.0 unx   112443 b- defN 23-May-09 13:41 version_stamp/vmn.py
--rw-r--r--  2.0 unx    35127 b- defN 23-May-09 13:43 vmn-0.8.5rc1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      470 b- defN 23-May-09 13:43 vmn-0.8.5rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-09 13:43 vmn-0.8.5rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-May-09 13:43 vmn-0.8.5rc1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-May-09 13:43 vmn-0.8.5rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      804 b- defN 23-May-09 13:43 vmn-0.8.5rc1.dist-info/RECORD
-10 files, 202368 bytes uncompressed, 44106 bytes compressed:  78.2%
+-rw-r--r--  2.0 unx    53186 b- defN 23-Jun-11 21:33 version_stamp/stamp_utils.py
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-11 21:54 version_stamp/version.py
+-rw-r--r--  2.0 unx   113063 b- defN 23-Jun-11 21:40 version_stamp/vmn.py
+-rw-r--r--  2.0 unx    35127 b- defN 23-Jun-11 21:54 vmn-0.8.5rc2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      470 b- defN 23-Jun-11 21:54 vmn-0.8.5rc2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 21:54 vmn-0.8.5rc2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-11 21:54 vmn-0.8.5rc2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-11 21:54 vmn-0.8.5rc2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      804 b- defN 23-Jun-11 21:54 vmn-0.8.5rc2.dist-info/RECORD
+10 files, 203013 bytes uncompressed, 44245 bytes compressed:  78.2%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: version_stamp/version.py
 Comment: 
 
 Filename: version_stamp/vmn.py
 Comment: 
 
-Filename: vmn-0.8.5rc1.dist-info/LICENSE.txt
+Filename: vmn-0.8.5rc2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: vmn-0.8.5rc1.dist-info/METADATA
+Filename: vmn-0.8.5rc2.dist-info/METADATA
 Comment: 
 
-Filename: vmn-0.8.5rc1.dist-info/WHEEL
+Filename: vmn-0.8.5rc2.dist-info/WHEEL
 Comment: 
 
-Filename: vmn-0.8.5rc1.dist-info/entry_points.txt
+Filename: vmn-0.8.5rc2.dist-info/entry_points.txt
 Comment: 
 
-Filename: vmn-0.8.5rc1.dist-info/top_level.txt
+Filename: vmn-0.8.5rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: vmn-0.8.5rc1.dist-info/RECORD
+Filename: vmn-0.8.5rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## version_stamp/stamp_utils.py

```diff
@@ -13,14 +13,15 @@
 from functools import wraps
 
 import git
 import yaml
 
 INIT_COMMIT_MESSAGE = "Initialized vmn tracking"
 
+# Only used for printing
 VMN_VERSION_FORMAT = (
     "{major}.{minor}.{patch}[.{hotfix}][-{prerelease}][+{buildmetadata}]"
 )
 VMN_DEFAULT_TEMPLATE = (
     "[{major}][.{minor}][.{patch}][.{hotfix}]" "[-{prerelease}][+{buildmetadata}]"
 )
```

## version_stamp/version.py

```diff
@@ -1,3 +1,3 @@
 name = "vmn"
-version = "0.8.5-rc1"
-_version = "0.8.5-rc1"
+version = "0.8.5-rc2"
+_version = "0.8.5-rc2"
```

## version_stamp/vmn.py

```diff
@@ -967,15 +967,15 @@
 
             if (
                 release_tag_formatted_app_name in ver_infos
                 and ver_infos[release_tag_formatted_app_name] is not None
             ):
                 stamp_utils.VMN_LOGGER.error(
                     f"The version {initial_version} was already released. "
-                    "Will refuse to stamp prerelease version "
+                    "Will refuse to stamp prerelease version"
                 )
                 raise RuntimeError()
 
         current_version, prerelease, prerelease_count = self.gen_advanced_version(
             initial_version, initialprerelease, initialprerelease_count
         )
 
@@ -1443,14 +1443,29 @@
 
     # For backward compatibility
     if vmn_ctx.vcs.release_mode == "micro":
         vmn_ctx.vcs.release_mode = "hotfix"
 
     assert vmn_ctx.vcs.release_mode is None or vmn_ctx.vcs.optional_release_mode is None
 
+    if vmn_ctx.vcs.override_version is not None:
+        match = re.search(stamp_utils.VMN_REGEX, vmn_ctx.vcs.override_version)
+
+        if match is None:
+            err = (
+                f"Provided override {vmn_ctx.vcs.override_version} doesn't comply with: "
+                f"{stamp_utils.VMN_VERSION_FORMAT} format")
+            stamp_utils.VMN_LOGGER.error(err)
+
+            raise RuntimeError(err)
+
+        gdict = match.groupdict()
+        assert gdict["prerelease"] is None
+        assert gdict["buildmetadata"] is None
+
     optional_status = {"modified", "detached"}
     expected_status = {
         "repos_exist_locally",
         "repo_tracked",
         "app_tracked",
         "deps_synced_with_conf",
     }
@@ -1497,19 +1512,23 @@
         initial_version,
         prerelease,
         prerelease_count,
     ) = VersionControlStamper.get_version_number_from_file(
         vmn_ctx.vcs.version_file_path
     )
 
+    is_release = vmn_ctx.vcs.ver_infos_from_repo[vmn_ctx.vcs.selected_tag]["ver_info"]["stamping"]["app"][
+                     "prerelease"] == "release"
+
     if vmn_ctx.vcs.override_version:
         initial_version = vmn_ctx.vcs.override_version
+        prerelease = 'release'
+        prerelease_count = {}
+        is_release = True
 
-    is_release = vmn_ctx.vcs.ver_infos_from_repo[vmn_ctx.vcs.selected_tag]["ver_info"]["stamping"]["app"][
-                     "prerelease"] == "release"
     if vmn_ctx.vcs.optional_release_mode and is_release:
         verstr = vmn_ctx.vcs.advance_version(initial_version, vmn_ctx.vcs.optional_release_mode, globally=False)
         tag_name_prefix = f'{vmn_ctx.vcs.name.replace("/", "-")}_{verstr}*'
         tag = vmn_ctx.vcs.backend.get_latest_available_tag(tag_name_prefix)
         if tag is not None and len(tag) < len(tag_name_prefix):
             tag = None
```

## Comparing `vmn-0.8.5rc1.dist-info/LICENSE.txt` & `vmn-0.8.5rc2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `vmn-0.8.5rc1.dist-info/RECORD` & `vmn-0.8.5rc2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 version_stamp/__init__.py,sha256=p_9bnBNpi1jHdKDsmBM7tN2Da3N-QOYEe8s09k9NIrk,152
-version_stamp/stamp_utils.py,sha256=uzHbTJwDRB8m0ECj88WmIz8-qynzMX8gd12OaL8sonM,53161
-version_stamp/version.py,sha256=jpCSZFCToz-MP_HvYsfZH3vLcarjZbM7bBPntCPAU4k,58
-version_stamp/vmn.py,sha256=_XeY1qPjTVW26Pf7EPolnpp9JVd3xQerbUxL4HI5gWg,112443
-vmn-0.8.5rc1.dist-info/LICENSE.txt,sha256=f6flbA23EQX0tZpqCsQCJesFmHb4XNOAOD99egZuaL4,35127
-vmn-0.8.5rc1.dist-info/METADATA,sha256=Pzs9P6hbkMK84MFL_4mKWqV0WYUy7eOOBnV7kaBZvs0,470
-vmn-0.8.5rc1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-vmn-0.8.5rc1.dist-info/entry_points.txt,sha256=8JQYxf_iGN3GSYg7ezJs-P8FM3Ss6Hspgg6QcV_s3uk,47
-vmn-0.8.5rc1.dist-info/top_level.txt,sha256=nVR6dU2EinKSe5A4ZJa7NR1aOPNV7QMXvB5Sm-rWbJs,14
-vmn-0.8.5rc1.dist-info/RECORD,,
+version_stamp/stamp_utils.py,sha256=-YavcLjR97hx7kXLQPxeZsz1Giv4YFV5bhZcBfrPD00,53186
+version_stamp/version.py,sha256=1f9Ei11VfuhHJctopm0T6YkYXvm6Oz6xdjpdBkYTEk0,58
+version_stamp/vmn.py,sha256=gZSfXOIz96ru49yc1a1m-k7iHYEaJXI67MunvBX_Fp4,113063
+vmn-0.8.5rc2.dist-info/LICENSE.txt,sha256=f6flbA23EQX0tZpqCsQCJesFmHb4XNOAOD99egZuaL4,35127
+vmn-0.8.5rc2.dist-info/METADATA,sha256=mfKE7aeFPFOxMJeCtWYt_A1F7WQNoVF7sGBvJcpj8bs,470
+vmn-0.8.5rc2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+vmn-0.8.5rc2.dist-info/entry_points.txt,sha256=8JQYxf_iGN3GSYg7ezJs-P8FM3Ss6Hspgg6QcV_s3uk,47
+vmn-0.8.5rc2.dist-info/top_level.txt,sha256=nVR6dU2EinKSe5A4ZJa7NR1aOPNV7QMXvB5Sm-rWbJs,14
+vmn-0.8.5rc2.dist-info/RECORD,,
```

