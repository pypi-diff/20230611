# Comparing `tmp/extract_msg-0.41.3.tar.gz` & `tmp/extract_msg-0.41.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extract_msg-0.41.3.tar", last modified: Sun Jun 11 02:28:03 2023, max compression
+gzip compressed data, was "extract_msg-0.41.4.tar", last modified: Sun Jun 11 16:43:27 2023, max compression
```

## Comparing `extract_msg-0.41.3.tar` & `extract_msg-0.41.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 02:28:03.610829 extract_msg-0.41.3/
--rw-rw-rw-   0        0        0    75763 2023-06-11 02:28:00.000000 extract_msg-0.41.3/CHANGELOG.md
--rw-rw-rw-   0        0        0    35147 2023-05-09 19:47:37.000000 extract_msg-0.41.3/LICENSE.txt
--rw-rw-rw-   0        0        0      165 2023-05-09 19:47:37.000000 extract_msg-0.41.3/MANIFEST.in
--rw-rw-rw-   0        0        0    12267 2023-06-11 02:28:03.610829 extract_msg-0.41.3/PKG-INFO
--rw-rw-rw-   0        0        0    11460 2023-06-11 02:28:00.000000 extract_msg-0.41.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-11 02:28:03.524058 extract_msg-0.41.3/extract_msg/
--rw-rw-rw-   0        0        0     2254 2023-06-11 02:28:00.000000 extract_msg-0.41.3/extract_msg/__init__.py
--rw-rw-rw-   0        0        0     3542 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 02:28:03.563952 extract_msg-0.41.3/extract_msg/_rtf/
--rw-rw-rw-   0        0        0      425 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/_rtf/__init__.py
--rw-rw-rw-   0        0        0      845 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/_rtf/create_doc.py
--rw-rw-rw-   0        0        0     6250 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/_rtf/inject_rtf.py
--rw-rw-rw-   0        0        0      856 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/_rtf/token.py
--rw-rw-rw-   0        0        0     8932 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/_rtf/tokenize_rtf.py
--rw-rw-rw-   0        0        0     6954 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/appointment.py
--rw-rw-rw-   0        0        0    13262 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/attachment.py
--rw-rw-rw-   0        0        0    16369 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/attachment_base.py
--rw-rw-rw-   0        0        0     3169 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/calendar.py
--rw-rw-rw-   0        0        0    21050 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/calendar_base.py
--rw-rw-rw-   0        0        0    27572 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/constants.py
--rw-rw-rw-   0        0        0    50103 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/contact.py
--rw-rw-rw-   0        0        0    58866 2023-05-25 02:02:13.000000 extract_msg-0.41.3/extract_msg/enums.py
--rw-rw-rw-   0        0        0     3377 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-11 02:28:03.568939 extract_msg-0.41.3/extract_msg/logging-config/
--rw-rw-rw-   0        0        0     2082 2023-05-09 19:47:37.000000 extract_msg-0.41.3/extract_msg/logging-config/logging-nt.json
--rw-rw-rw-   0        0        0     2058 2023-05-09 19:47:37.000000 extract_msg-0.41.3/extract_msg/logging-config/logging-posix.json
--rw-rw-rw-   0        0        0     3588 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/meeting_cancellation.py
--rw-rw-rw-   0        0        0     1628 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/meeting_exception.py
--rw-rw-rw-   0        0        0     3771 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/meeting_forward.py
--rw-rw-rw-   0        0        0     2043 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/meeting_related.py
--rw-rw-rw-   0        0        0     6784 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/meeting_request.py
--rw-rw-rw-   0        0        0     2415 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/meeting_response.py
--rw-rw-rw-   0        0        0      375 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/message.py
--rw-rw-rw-   0        0        0    59297 2023-06-11 02:28:00.000000 extract_msg-0.41.3/extract_msg/message_base.py
--rw-rw-rw-   0        0        0      201 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/message_signed.py
--rw-rw-rw-   0        0        0     7201 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/message_signed_base.py
--rw-rw-rw-   0        0        0    39208 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/msg.py
--rw-rw-rw-   0        0        0    12647 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/named.py
--rw-rw-rw-   0        0        0    41608 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/ole_writer.py
--rw-rw-rw-   0        0        0     2578 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/post.py
--rw-rw-rw-   0        0        0     6723 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/prop.py
--rw-rw-rw-   0        0        0     7602 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/properties.py
--rw-rw-rw-   0        0        0        0 2023-05-09 19:47:37.000000 extract_msg-0.41.3/extract_msg/py.typed
--rw-rw-rw-   0        0        0    12677 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/recipient.py
--rw-rw-rw-   0        0        0     8976 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/signed_attachment.py
-drwxrwxrwx   0        0        0        0 2023-06-11 02:28:03.609841 extract_msg-0.41.3/extract_msg/structures/
--rw-rw-rw-   0        0        0      336 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/structures/__init__.py
--rw-rw-rw-   0        0        0    11677 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/structures/_helpers.py
--rw-rw-rw-   0        0        0     6676 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/structures/business_card.py
--rw-rw-rw-   0        0        0    19038 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/structures/entry_id.py
--rw-rw-rw-   0        0        0     6161 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/structures/misc_id.py
--rw-rw-rw-   0        0        0     7370 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/structures/recurrence_pattern.py
--rw-rw-rw-   0        0        0     3263 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/structures/report_tag.py
--rw-rw-rw-   0        0        0     1391 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/structures/system_time.py
--rw-rw-rw-   0        0        0     1616 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/structures/time_zone_definition.py
--rw-rw-rw-   0        0        0     2440 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/structures/time_zone_struct.py
--rw-rw-rw-   0        0        0     3263 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/structures/tz_rule.py
--rw-rw-rw-   0        0        0    13190 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/task.py
--rw-rw-rw-   0        0        0     4162 2023-05-09 19:54:43.000000 extract_msg-0.41.3/extract_msg/task_request.py
--rw-rw-rw-   0        0        0    56482 2023-06-11 02:28:00.000000 extract_msg-0.41.3/extract_msg/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-11 02:28:03.545003 extract_msg-0.41.3/extract_msg.egg-info/
--rw-rw-rw-   0        0        0    12267 2023-06-11 02:28:03.000000 extract_msg-0.41.3/extract_msg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1827 2023-06-11 02:28:03.000000 extract_msg-0.41.3/extract_msg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 02:28:03.000000 extract_msg-0.41.3/extract_msg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-11 02:28:03.000000 extract_msg-0.41.3/extract_msg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      228 2023-06-11 02:28:03.000000 extract_msg-0.41.3/extract_msg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-11 02:28:03.000000 extract_msg-0.41.3/extract_msg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      197 2023-05-09 19:54:43.000000 extract_msg-0.41.3/requirements.txt
--rw-rw-rw-   0        0        0      167 2023-06-11 02:28:03.612822 extract_msg-0.41.3/setup.cfg
--rw-rw-rw-   0        0        0     1657 2023-05-09 19:47:37.000000 extract_msg-0.41.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:43:27.662832 extract_msg-0.41.4/
+-rw-rw-rw-   0        0        0    75966 2023-06-11 16:43:24.000000 extract_msg-0.41.4/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35147 2023-05-09 19:47:37.000000 extract_msg-0.41.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      165 2023-05-09 19:47:37.000000 extract_msg-0.41.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    12267 2023-06-11 16:43:27.663830 extract_msg-0.41.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11460 2023-06-11 16:43:24.000000 extract_msg-0.41.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-11 16:43:27.489278 extract_msg-0.41.4/extract_msg/
+-rw-rw-rw-   0        0        0     2254 2023-06-11 16:43:24.000000 extract_msg-0.41.4/extract_msg/__init__.py
+-rw-rw-rw-   0        0        0     3542 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:43:27.575067 extract_msg-0.41.4/extract_msg/_rtf/
+-rw-rw-rw-   0        0        0      425 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/_rtf/__init__.py
+-rw-rw-rw-   0        0        0      845 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/_rtf/create_doc.py
+-rw-rw-rw-   0        0        0     6250 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/_rtf/inject_rtf.py
+-rw-rw-rw-   0        0        0      856 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/_rtf/token.py
+-rw-rw-rw-   0        0        0     8932 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/_rtf/tokenize_rtf.py
+-rw-rw-rw-   0        0        0     6954 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/appointment.py
+-rw-rw-rw-   0        0        0    13262 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/attachment.py
+-rw-rw-rw-   0        0        0    16369 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/attachment_base.py
+-rw-rw-rw-   0        0        0     3169 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/calendar.py
+-rw-rw-rw-   0        0        0    21050 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/calendar_base.py
+-rw-rw-rw-   0        0        0    27572 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/constants.py
+-rw-rw-rw-   0        0        0    50103 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/contact.py
+-rw-rw-rw-   0        0        0    58866 2023-05-25 02:02:13.000000 extract_msg-0.41.4/extract_msg/enums.py
+-rw-rw-rw-   0        0        0     3377 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:43:27.584044 extract_msg-0.41.4/extract_msg/logging-config/
+-rw-rw-rw-   0        0        0     2082 2023-05-09 19:47:37.000000 extract_msg-0.41.4/extract_msg/logging-config/logging-nt.json
+-rw-rw-rw-   0        0        0     2058 2023-05-09 19:47:37.000000 extract_msg-0.41.4/extract_msg/logging-config/logging-posix.json
+-rw-rw-rw-   0        0        0     3588 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/meeting_cancellation.py
+-rw-rw-rw-   0        0        0     1628 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/meeting_exception.py
+-rw-rw-rw-   0        0        0     3771 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/meeting_forward.py
+-rw-rw-rw-   0        0        0     2043 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/meeting_related.py
+-rw-rw-rw-   0        0        0     6784 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/meeting_request.py
+-rw-rw-rw-   0        0        0     2415 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/meeting_response.py
+-rw-rw-rw-   0        0        0      375 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/message.py
+-rw-rw-rw-   0        0        0    59297 2023-06-11 02:28:00.000000 extract_msg-0.41.4/extract_msg/message_base.py
+-rw-rw-rw-   0        0        0      201 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/message_signed.py
+-rw-rw-rw-   0        0        0     7201 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/message_signed_base.py
+-rw-rw-rw-   0        0        0    39208 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/msg.py
+-rw-rw-rw-   0        0        0    12647 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/named.py
+-rw-rw-rw-   0        0        0    41608 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/ole_writer.py
+-rw-rw-rw-   0        0        0     2578 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/post.py
+-rw-rw-rw-   0        0        0     6723 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/prop.py
+-rw-rw-rw-   0        0        0     7602 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/properties.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:47:37.000000 extract_msg-0.41.4/extract_msg/py.typed
+-rw-rw-rw-   0        0        0    12677 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/recipient.py
+-rw-rw-rw-   0        0        0     8976 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/signed_attachment.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:43:27.661835 extract_msg-0.41.4/extract_msg/structures/
+-rw-rw-rw-   0        0        0      336 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/structures/__init__.py
+-rw-rw-rw-   0        0        0    11677 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/structures/_helpers.py
+-rw-rw-rw-   0        0        0     6676 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/structures/business_card.py
+-rw-rw-rw-   0        0        0    19038 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/structures/entry_id.py
+-rw-rw-rw-   0        0        0     6161 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/structures/misc_id.py
+-rw-rw-rw-   0        0        0     7370 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/structures/recurrence_pattern.py
+-rw-rw-rw-   0        0        0     3263 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/structures/report_tag.py
+-rw-rw-rw-   0        0        0     1391 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/structures/system_time.py
+-rw-rw-rw-   0        0        0     1616 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/structures/time_zone_definition.py
+-rw-rw-rw-   0        0        0     2440 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/structures/time_zone_struct.py
+-rw-rw-rw-   0        0        0     3263 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/structures/tz_rule.py
+-rw-rw-rw-   0        0        0    13190 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/task.py
+-rw-rw-rw-   0        0        0     4162 2023-05-09 19:54:43.000000 extract_msg-0.41.4/extract_msg/task_request.py
+-rw-rw-rw-   0        0        0    56485 2023-06-11 16:43:24.000000 extract_msg-0.41.4/extract_msg/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-11 16:43:27.535176 extract_msg-0.41.4/extract_msg.egg-info/
+-rw-rw-rw-   0        0        0    12267 2023-06-11 16:43:27.000000 extract_msg-0.41.4/extract_msg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1827 2023-06-11 16:43:27.000000 extract_msg-0.41.4/extract_msg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 16:43:27.000000 extract_msg-0.41.4/extract_msg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-11 16:43:27.000000 extract_msg-0.41.4/extract_msg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      237 2023-06-11 16:43:27.000000 extract_msg-0.41.4/extract_msg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-11 16:43:27.000000 extract_msg-0.41.4/extract_msg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      206 2023-06-11 16:43:24.000000 extract_msg-0.41.4/requirements.txt
+-rw-rw-rw-   0        0        0      167 2023-06-11 16:43:27.669816 extract_msg-0.41.4/setup.cfg
+-rw-rw-rw-   0        0        0     1657 2023-05-09 19:47:37.000000 extract_msg-0.41.4/setup.py
```

### Comparing `extract_msg-0.41.3/CHANGELOG.md` & `extract_msg-0.41.4/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+**v0.41.4**
+* Fixed an issue in the last version that would break the decoding function if the contents were not encoded.
+* Updated `tzlocal` and allow future updates for `compressed_rtf` and `ebcdic`.
+
 **v0.41.3**
 * [[TeamMsgExtractor #365](https://github.com/TeamMsgExtractor/msg-extractor/issues/365)] Fixed an issue that would cause certain values retrieved from the header to not be decoded properly. It does this when retrieving the values, so nothing about the header has been changed.
 * Added new property `MessageBase.headerText` which is the text content of the header stream. Adjusted other things to use this instead of trying to retrieve the stream directly in multiple places.
 * Added typing to `MessageBase.header`.
 
 **v0.41.2**
 * Updated annotations on `MessageBase.save`.
```

### Comparing `extract_msg-0.41.3/LICENSE.txt` & `extract_msg-0.41.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/PKG-INFO` & `extract_msg-0.41.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extract_msg
-Version: 0.41.3
+Version: 0.41.4
 Summary: Extracts emails and attachments saved in Microsoft Outlook's .msg files
 Home-page: https://github.com/TeamMsgExtractor/msg-extractor
 Download-URL: https://github.com/TeamMsgExtractor/msg-extractor/archives/master
 Author: Destiny Peterson & Matthew Walker
 Author-email: arceusthe@gmail.com, mattgwwalker@gmail.com
 License: GPL
 Requires-Python: >=3.8
@@ -261,16 +261,16 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.41.3-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.41.3/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.41.4-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.41.4/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3816/
 .. _Matthew Walker: https://github.com/mattgwwalker
 .. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
 .. _JP Bourget: https://github.com/punkrokk
 .. _Philippe Lagadec: https://github.com/decalage2
```

### Comparing `extract_msg-0.41.3/README.rst` & `extract_msg-0.41.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -246,16 +246,16 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.41.3-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.41.3/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.41.4-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.41.4/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3816/
 .. _Matthew Walker: https://github.com/mattgwwalker
 .. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
 .. _JP Bourget: https://github.com/punkrokk
 .. _Philippe Lagadec: https://github.com/decalage2
```

### Comparing `extract_msg-0.41.3/extract_msg/__init__.py` & `extract_msg-0.41.4/extract_msg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __author__ = 'Destiny Peterson & Matthew Walker'
-__date__ = '2023-06-10'
-__version__ = '0.41.3'
+__date__ = '2023-06-11'
+__version__ = '0.41.4'
 
 __all__ = [
     # Modules:
     'constants',
     'enums',
     'exceptions',
```

### Comparing `extract_msg-0.41.3/extract_msg/__main__.py` & `extract_msg-0.41.4/extract_msg/__main__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/_rtf/create_doc.py` & `extract_msg-0.41.4/extract_msg/_rtf/create_doc.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/_rtf/inject_rtf.py` & `extract_msg-0.41.4/extract_msg/_rtf/inject_rtf.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/_rtf/token.py` & `extract_msg-0.41.4/extract_msg/_rtf/token.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/_rtf/tokenize_rtf.py` & `extract_msg-0.41.4/extract_msg/_rtf/tokenize_rtf.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/appointment.py` & `extract_msg-0.41.4/extract_msg/appointment.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/attachment.py` & `extract_msg-0.41.4/extract_msg/attachment.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/attachment_base.py` & `extract_msg-0.41.4/extract_msg/attachment_base.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/calendar.py` & `extract_msg-0.41.4/extract_msg/calendar.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/calendar_base.py` & `extract_msg-0.41.4/extract_msg/calendar_base.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/constants.py` & `extract_msg-0.41.4/extract_msg/constants.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/contact.py` & `extract_msg-0.41.4/extract_msg/contact.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/enums.py` & `extract_msg-0.41.4/extract_msg/enums.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/exceptions.py` & `extract_msg-0.41.4/extract_msg/exceptions.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/logging-config/logging-nt.json` & `extract_msg-0.41.4/extract_msg/logging-config/logging-nt.json`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/logging-config/logging-posix.json` & `extract_msg-0.41.4/extract_msg/logging-config/logging-posix.json`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/meeting_cancellation.py` & `extract_msg-0.41.4/extract_msg/meeting_cancellation.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/meeting_exception.py` & `extract_msg-0.41.4/extract_msg/meeting_exception.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/meeting_forward.py` & `extract_msg-0.41.4/extract_msg/meeting_forward.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/meeting_related.py` & `extract_msg-0.41.4/extract_msg/meeting_related.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/meeting_request.py` & `extract_msg-0.41.4/extract_msg/meeting_request.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/meeting_response.py` & `extract_msg-0.41.4/extract_msg/meeting_response.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/message_base.py` & `extract_msg-0.41.4/extract_msg/message_base.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/message_signed_base.py` & `extract_msg-0.41.4/extract_msg/message_signed_base.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/msg.py` & `extract_msg-0.41.4/extract_msg/msg.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/named.py` & `extract_msg-0.41.4/extract_msg/named.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/ole_writer.py` & `extract_msg-0.41.4/extract_msg/ole_writer.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/post.py` & `extract_msg-0.41.4/extract_msg/post.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/prop.py` & `extract_msg-0.41.4/extract_msg/prop.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/properties.py` & `extract_msg-0.41.4/extract_msg/properties.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/recipient.py` & `extract_msg-0.41.4/extract_msg/recipient.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/signed_attachment.py` & `extract_msg-0.41.4/extract_msg/signed_attachment.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/structures/_helpers.py` & `extract_msg-0.41.4/extract_msg/structures/_helpers.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/structures/business_card.py` & `extract_msg-0.41.4/extract_msg/structures/business_card.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/structures/entry_id.py` & `extract_msg-0.41.4/extract_msg/structures/entry_id.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/structures/misc_id.py` & `extract_msg-0.41.4/extract_msg/structures/misc_id.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/structures/recurrence_pattern.py` & `extract_msg-0.41.4/extract_msg/structures/recurrence_pattern.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/structures/report_tag.py` & `extract_msg-0.41.4/extract_msg/structures/report_tag.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/structures/system_time.py` & `extract_msg-0.41.4/extract_msg/structures/system_time.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/structures/time_zone_definition.py` & `extract_msg-0.41.4/extract_msg/structures/time_zone_definition.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/structures/time_zone_struct.py` & `extract_msg-0.41.4/extract_msg/structures/time_zone_struct.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/structures/tz_rule.py` & `extract_msg-0.41.4/extract_msg/structures/tz_rule.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/task.py` & `extract_msg-0.41.4/extract_msg/task.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/task_request.py` & `extract_msg-0.41.4/extract_msg/task_request.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/extract_msg/utils.py` & `extract_msg-0.41.4/extract_msg/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     """
     # This returns a list of tuples containing the bytes and the encoding they
     # are using, so we decode each one and join them together.
     #
     # decode_header header will return a string instead of bytes for the first
     # object if the input is not encoded, something that is frustrating.
     return ''.join(
-        x[0].decode(x[1] or 'ascii') if isinstance(x[0], bytes) else x
+        x[0].decode(x[1] or 'ascii') if isinstance(x[0], bytes) else x[0]
         for x in email.header.decode_header(encoded)
     )
 
 
 def dictGetCasedKey(_dict : Dict, key : Any) -> Any:
     """
     Retrieves the key from the dictionary with the proper casing using a
```

### Comparing `extract_msg-0.41.3/extract_msg.egg-info/PKG-INFO` & `extract_msg-0.41.4/extract_msg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extract-msg
-Version: 0.41.3
+Version: 0.41.4
 Summary: Extracts emails and attachments saved in Microsoft Outlook's .msg files
 Home-page: https://github.com/TeamMsgExtractor/msg-extractor
 Download-URL: https://github.com/TeamMsgExtractor/msg-extractor/archives/master
 Author: Destiny Peterson & Matthew Walker
 Author-email: arceusthe@gmail.com, mattgwwalker@gmail.com
 License: GPL
 Requires-Python: >=3.8
@@ -261,16 +261,16 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.41.3-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.41.3/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.41.4-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.41.4/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3816/
 .. _Matthew Walker: https://github.com/mattgwwalker
 .. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
 .. _JP Bourget: https://github.com/punkrokk
 .. _Philippe Lagadec: https://github.com/decalage2
```

### Comparing `extract_msg-0.41.3/extract_msg.egg-info/SOURCES.txt` & `extract_msg-0.41.4/extract_msg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.3/setup.py` & `extract_msg-0.41.4/setup.py`

 * *Files identical despite different names*

