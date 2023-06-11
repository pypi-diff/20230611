# Comparing `tmp/xmodem-0.4.6.tar.gz` & `tmp/xmodem-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xmodem-0.4.6.tar", last modified: Fri Mar 27 20:52:10 2020, max compression
+gzip compressed data, was "xmodem-0.4.7.tar", last modified: Sun Jun 11 18:00:37 2023, max compression
```

## Comparing `xmodem-0.4.6.tar` & `xmodem-0.4.7.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 wijnand    (501) staff       (20)        0 2020-03-27 20:52:10.000000 xmodem-0.4.6/
--rw-r--r--   0 wijnand    (501) staff       (20)     4193 2020-03-27 20:52:10.000000 xmodem-0.4.6/PKG-INFO
-drwxr-xr-x   0 wijnand    (501) staff       (20)        0 2020-03-27 20:52:10.000000 xmodem-0.4.6/xmodem/
--rw-r--r--   0 wijnand    (501) staff       (20)    29064 2020-03-27 20:42:36.000000 xmodem-0.4.6/xmodem/__init__.py
--rw-r--r--   0 wijnand    (501) staff       (20)       81 2020-03-27 20:03:30.000000 xmodem-0.4.6/xmodem/__main__.py
--rw-r--r--   0 wijnand    (501) staff       (20)       53 2016-11-03 15:28:19.000000 xmodem-0.4.6/MANIFEST.in
--rw-r--r--   0 wijnand    (501) staff       (20)      784 2020-03-27 20:48:42.000000 xmodem-0.4.6/setup.py
-drwxr-xr-x   0 wijnand    (501) staff       (20)        0 2020-03-27 20:52:10.000000 xmodem-0.4.6/doc/
--rw-r--r--   0 wijnand    (501) staff       (20)     5312 2016-11-03 15:28:19.000000 xmodem-0.4.6/doc/XMODMCRC.TXT
--rw-r--r--   0 wijnand    (501) staff       (20)     4692 2020-03-27 19:57:30.000000 xmodem-0.4.6/doc/XMODEM1K.TXT
--rw-r--r--   0 wijnand    (501) staff       (20)     4452 2020-03-27 19:57:30.000000 xmodem-0.4.6/doc/XMODEM.TXT
--rw-r--r--   0 wijnand    (501) staff       (20)    49446 2016-11-03 15:28:19.000000 xmodem-0.4.6/doc/ymodem.txt
--rw-r--r--   0 wijnand    (501) staff       (20)      159 2020-03-27 20:52:10.000000 xmodem-0.4.6/setup.cfg
--rw-r--r--   0 wijnand    (501) staff       (20)     3194 2020-03-27 20:50:32.000000 xmodem-0.4.6/README.rst
-drwxr-xr-x   0 wijnand    (501) staff       (20)        0 2020-03-27 20:52:10.000000 xmodem-0.4.6/xmodem.egg-info/
--rw-r--r--   0 wijnand    (501) staff       (20)     4193 2020-03-27 20:52:10.000000 xmodem-0.4.6/xmodem.egg-info/PKG-INFO
--rw-r--r--   0 wijnand    (501) staff       (20)      263 2020-03-27 20:52:10.000000 xmodem-0.4.6/xmodem.egg-info/SOURCES.txt
--rw-r--r--   0 wijnand    (501) staff       (20)        7 2020-03-27 20:52:10.000000 xmodem-0.4.6/xmodem.egg-info/top_level.txt
--rw-r--r--   0 wijnand    (501) staff       (20)        1 2020-03-27 20:52:10.000000 xmodem-0.4.6/xmodem.egg-info/dependency_links.txt
+drwxr-xr-x   0 jq         (501) staff       (20)        0 2023-06-11 18:00:37.510790 xmodem-0.4.7/
+-rw-r--r--   0 jq         (501) staff       (20)     1103 2023-05-01 17:27:48.000000 xmodem-0.4.7/LICENSE
+-rw-r--r--   0 jq         (501) staff       (20)       61 2023-05-01 17:27:48.000000 xmodem-0.4.7/MANIFEST.in
+-rw-r--r--   0 jq         (501) staff       (20)     4333 2023-06-11 18:00:37.510875 xmodem-0.4.7/PKG-INFO
+-rw-r--r--   0 jq         (501) staff       (20)     4055 2023-06-11 17:37:05.000000 xmodem-0.4.7/README.rst
+drwxr-xr-x   0 jq         (501) staff       (20)        0 2023-06-11 18:00:37.507957 xmodem-0.4.7/doc/
+-rw-r--r--   0 jq         (501) staff       (20)     4457 2023-05-01 17:27:48.000000 xmodem-0.4.7/doc/XMODEM.TXT
+-rw-r--r--   0 jq         (501) staff       (20)     4693 2023-05-01 17:27:48.000000 xmodem-0.4.7/doc/XMODEM1K.TXT
+-rw-r--r--   0 jq         (501) staff       (20)     5313 2023-05-01 17:27:48.000000 xmodem-0.4.7/doc/XMODMCRC.TXT
+drwxr-xr-x   0 jq         (501) staff       (20)        0 2023-06-11 18:00:37.506065 xmodem-0.4.7/doc/build/
+drwxr-xr-x   0 jq         (501) staff       (20)        0 2023-06-11 18:00:37.506122 xmodem-0.4.7/doc/build/html/
+drwxr-xr-x   0 jq         (501) staff       (20)        0 2023-06-11 18:00:37.509457 xmodem-0.4.7/doc/build/html/_sources/
+-rw-r--r--   0 jq         (501) staff       (20)      432 2014-11-29 22:15:27.000000 xmodem-0.4.7/doc/build/html/_sources/index.rst.txt
+-rw-r--r--   0 jq         (501) staff       (20)      254 2014-11-29 22:15:27.000000 xmodem-0.4.7/doc/build/html/_sources/xmodem.rst.txt
+-rw-r--r--   0 jq         (501) staff       (20)    49447 2023-05-01 17:27:48.000000 xmodem-0.4.7/doc/ymodem.txt
+-rw-r--r--   0 jq         (501) staff       (20)      159 2023-06-11 18:00:37.511107 xmodem-0.4.7/setup.cfg
+-rw-r--r--   0 jq         (501) staff       (20)      784 2023-05-01 17:27:48.000000 xmodem-0.4.7/setup.py
+drwxr-xr-x   0 jq         (501) staff       (20)        0 2023-06-11 18:00:37.510083 xmodem-0.4.7/xmodem/
+-rw-r--r--   0 jq         (501) staff       (20)    29627 2023-06-11 17:35:09.000000 xmodem-0.4.7/xmodem/__init__.py
+-rw-r--r--   0 jq         (501) staff       (20)       81 2023-05-01 17:27:48.000000 xmodem-0.4.7/xmodem/__main__.py
+drwxr-xr-x   0 jq         (501) staff       (20)        0 2023-06-11 18:00:37.510680 xmodem-0.4.7/xmodem.egg-info/
+-rw-r--r--   0 jq         (501) staff       (20)     4333 2023-06-11 18:00:37.000000 xmodem-0.4.7/xmodem.egg-info/PKG-INFO
+-rw-r--r--   0 jq         (501) staff       (20)      348 2023-06-11 18:00:37.000000 xmodem-0.4.7/xmodem.egg-info/SOURCES.txt
+-rw-r--r--   0 jq         (501) staff       (20)        1 2023-06-11 18:00:37.000000 xmodem-0.4.7/xmodem.egg-info/dependency_links.txt
+-rw-r--r--   0 jq         (501) staff       (20)        7 2023-06-11 18:00:37.000000 xmodem-0.4.7/xmodem.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `xmodem-0.4.6/PKG-INFO` & `xmodem-0.4.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,100 +1,116 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: xmodem
-Version: 0.4.6
+Version: 0.4.7
 Summary: XMODEM protocol implementation.
 Home-page: https://github.com/tehmaze/xmodem
 Author: Wijnand Modderman, Jeff Quast, Kris Hardy
 Author-email: maze@pyth0n.org
 License: MIT
-Description: .. image:: https://travis-ci.org/tehmaze/xmodem.png?branch=master
-           :target: https://travis-ci.org/tehmaze/xmodem
-        
-        .. image:: https://coveralls.io/repos/tehmaze/xmodem/badge.png
-           :target: https://coveralls.io/r/tehmaze/xmodem
-        
-        ================================
-         XMODEM protocol implementation
-        ================================
-        
-        Documentation available at http://packages.python.org/xmodem/
-        
-        Python Package Index (PyPI) page is available at https://pypi.python.org/pypi/xmodem
-        
-        Usage
-        =====
-        
-        Create a function to get and put character data (to a serial line for
-        example)::
-        
-            >>> import serial
-            >>> from xmodem import XMODEM
-            >>> ser = serial.Serial('/dev/ttyUSB0', timeout=0) # or whatever port you need
-            >>> def getc(size, timeout=1):
-            ...     return ser.read(size) or None
-            ...
-            >>> def putc(data, timeout=1):
-            ...     return ser.write(data)  # note that this ignores the timeout
-            ...
-            >>> modem = XMODEM(getc, putc)
-        
-        Now, to upload a file, use the ``send`` method::
-        
-            >>> stream = open('/etc/fstab', 'rb')
-            >>> modem.send(stream)
-        
-        To download a file, use the ``recv`` method::
-        
-            >>> stream = open('output', 'wb')
-            >>> modem.recv(stream)
-        
-        For more information, take a look at the documentation_.
-        
-        .. _documentation: http://packages.python.org/xmodem/xmodem.html
-        
-        Changes
-        =======
-        
-        0.4.6:
-          * bugfix: Abort send on EOT in startup-sequence `Issue #34 
-            <https://github.com/tehmaze/xmodem/issues/34>`_.
-          * enhancement: Include LICENSE file in the source distribution.
-        
-        0.4.5:
-          * bugfix: Remove bogus `assert False` code in ``recv()`` that resulted in
-            `AssertionError` introduced in version 0.4.0 commit-id `9b03fc20`, `PR #29
-            <https://github.com/tehmaze/xmodem/pull/29>`_.
-        
-        0.4.4:
-          * bugfix: Large file transfers in ``send()`` were more likely to fail for
-            small values of ``retry``: This value should be the maximum failures per
-            block transfer as documented, but was improperly implemented as the number
-            of failures allowed for the total duration of the transfer, `PR #21
-            <https://github.com/tehmaze/xmodem/pull/21>`_.
-          * bugfix: ``send(retry=n)`` and ``recv(retry=n)`` should retry ``n`` times
-            as documented, was retrying ``n - 1``.
-        
-        0.4.3:
-          * bugfix: ``putc()`` callback was called in series, 3 times for each part of
-            xmodem block header, data, and checksum during block transfer.  Now all
-            three data blocks are sent by single ``putc()`` call.  This resolves issues
-            when integrating with microcontrollers or equipment sensitive to timing
-            issues at stream boundaries, `PR #19
-            <https://github.com/tehmaze/xmodem/pull/19>`_.
-        
-        0.4.2:
-          * bugfix: documentation files missing from the release tarball
-            `Issue #16 <https://github.com/tehmaze/xmodem/issues/16>`_.
-        
-        0.4.1
-          * bugfix: re-transmit in ``send()`` on ``NAK`` or timeout, previously
-            re-transmissions (wrongly) occurred only on garbage bytes.
-            `PR #12 <https://github.com/tehmaze/xmodem/pull/12>`_.
-        
-        0.4.0
-          * enhancement: support for python 3
-            `PR #8 <https://github.com/tehmaze/xmodem/pull/8>`_.
-          * bugfix: CRC failures in XMODEM.recv() were not renegotiated correctly
-            `PR #11 <https://github.com/tehmaze/xmodem/issues/11>`_.
-        
 Keywords: xmodem protocol
-Platform: UNKNOWN
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/tehmaze/xmodem.png?branch=master
+   :target: https://travis-ci.org/tehmaze/xmodem
+
+.. image:: https://coveralls.io/repos/tehmaze/xmodem/badge.png
+   :target: https://coveralls.io/r/tehmaze/xmodem
+
+================================
+ XMODEM protocol implementation
+================================
+
+Documentation available at http://packages.python.org/xmodem/
+
+Python Package Index (PyPI) page is available at https://pypi.python.org/pypi/xmodem
+
+xmodem has been tested with python 2.7 through python 3.11
+
+Usage
+=====
+
+Create a function to get and put character data (to a serial line for
+example)::
+
+    >>> import serial
+    >>> from xmodem import XMODEM
+    >>> ser = serial.Serial('/dev/ttyUSB0', timeout=0) # or whatever port you need
+    >>> def getc(size, timeout=1):
+    ...     return ser.read(size) or None
+    ...
+    >>> def putc(data, timeout=1):
+    ...     return ser.write(data)  # note that this ignores the timeout
+    ...
+    >>> modem = XMODEM(getc, putc)
+
+Now, to upload a file, use the ``send`` method::
+
+    >>> stream = open('/etc/fstab', 'rb')
+    >>> modem.send(stream)
+
+To download a file, use the ``recv`` method::
+
+    >>> stream = open('output', 'wb')
+    >>> modem.recv(stream)
+
+For more information, take a look at the documentation_.
+
+.. _documentation: http://packages.python.org/xmodem/xmodem.html
+
+Changes
+=======
+0.4.7:
+   * bugfix: stall on some kinds of error in ``recv()``, `PR #56
+     <https://github.com/tehmaze/xmodem/pull/56>`_.
+   * bugfix: sequence number miscalculation in ``send()``, `PR #52
+     <https://github.com/tehmaze/xmodem/pull/52>`_.
+   * enhancement: callback function added for ``recv()``, `PR #53
+     <https://github.com/tehmaze/xmodem/pull/53>`_.
+   * bugfix: receiving empty file and stall condition in ``recv()``, `PR #50
+     <https://github.com/tehmaze/xmodem/pull/50>`_.
+   * bugfix: callback is now called for some kinds of errors
+     and some CLI fixes, `8a798e8b
+     <https://github.com/tehmaze/xmodem/commit/8a798e8b2af2a9cd6f9e789ef154a23a6467f98b>`_.
+   * bugfix: remove DepreactionWarning for ``logging.warn()``, `PR #49
+     <https://github.com/tehmaze/xmodem/pull/49>`_.
+
+0.4.6:
+  * bugfix: Abort send on EOT in startup-sequence `Issue #34 
+    <https://github.com/tehmaze/xmodem/issues/34>`_.
+  * enhancement: Include LICENSE file in the source distribution.
+
+0.4.5:
+  * bugfix: Remove bogus `assert False` code in ``recv()`` that resulted in
+    `AssertionError` introduced in version 0.4.0 commit-id `9b03fc20`, `PR #29
+    <https://github.com/tehmaze/xmodem/pull/29>`_.
+
+0.4.4:
+  * bugfix: Large file transfers in ``send()`` were more likely to fail for
+    small values of ``retry``: This value should be the maximum failures per
+    block transfer as documented, but was improperly implemented as the number
+    of failures allowed for the total duration of the transfer, `PR #21
+    <https://github.com/tehmaze/xmodem/pull/21>`_.
+  * bugfix: ``send(retry=n)`` and ``recv(retry=n)`` should retry ``n`` times
+    as documented, was retrying ``n - 1``.
+
+0.4.3:
+  * bugfix: ``putc()`` callback was called in series, 3 times for each part of
+    xmodem block header, data, and checksum during block transfer.  Now all
+    three data blocks are sent by single ``putc()`` call.  This resolves issues
+    when integrating with microcontrollers or equipment sensitive to timing
+    issues at stream boundaries, `PR #19
+    <https://github.com/tehmaze/xmodem/pull/19>`_.
+
+0.4.2:
+  * bugfix: documentation files missing from the release tarball
+    `Issue #16 <https://github.com/tehmaze/xmodem/issues/16>`_.
+
+0.4.1
+  * bugfix: re-transmit in ``send()`` on ``NAK`` or timeout, previously
+    re-transmissions (wrongly) occurred only on garbage bytes.
+    `PR #12 <https://github.com/tehmaze/xmodem/pull/12>`_.
+
+0.4.0
+  * enhancement: support for python 3
+    `PR #8 <https://github.com/tehmaze/xmodem/pull/8>`_.
+  * bugfix: CRC failures in XMODEM.recv() were not renegotiated correctly
+    `PR #11 <https://github.com/tehmaze/xmodem/issues/11>`_.
```

### Comparing `xmodem-0.4.6/xmodem/__init__.py` & `xmodem-0.4.7/xmodem/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 __copyright__ = ['Copyright (c) 2010 Wijnand Modderman',
                  'Copyright (c) 1981 Chuck Forsberg']
 __license__ = 'MIT'
 __version__ = '0.4.5'
 
 import platform
 import logging
+import select
 import time
 import sys
 from functools import partial
 
 # Protocol bytes
 SOH = b'\x01'
 STX = b'\x02'
@@ -132,39 +133,40 @@
 
 
 class XMODEM(object):
     '''
     XMODEM Protocol handler, expects two callables which encapsulate the read
         and write operations on the underlying stream.
 
-    Example functions for reading and writing to a serial line:
+    Example functions for reading and writing to a serial line using `pyserial <http://pyserial.sourceforge.net/>`_,
 
-    >>> import serial
-    >>> from xmodem import XMODEM
-    >>> ser = serial.Serial('/dev/ttyUSB0', timeout=0) # or whatever you need
-    >>> def getc(size, timeout=1):
-    ...     return ser.read(size) or None
-    ...
-    >>> def putc(data, timeout=1):
-    ...     return ser.write(data) or None
-    ...
-    >>> modem = XMODEM(getc, putc)
+    .. code-block:: python
 
+        import serial
+        from xmodem import XMODEM
+        ser = serial.Serial('/dev/ttyUSB0', timeout=0) # or whatever you need
+        def getc(size, timeout=1):
+            return ser.read(size) or None
+
+        def putc(data, timeout=1):
+            return ser.write(data) or None
+
+        modem = XMODEM(getc, putc)
 
     :param getc: Function to retrieve bytes from a stream. The function takes
         the number of bytes to read from the stream and a timeout in seconds as
         parameters. It must return the bytes which were read, or ``None`` if a
-        timeout occured.
+        timeout occurred.
     :type getc: callable
     :param putc: Function to transmit bytes to a stream. The function takes the
         bytes to be written and a timeout in seconds as parameters. It must
         return the number of bytes written to the stream, or ``None`` in case of
         a timeout.
     :type putc: callable
-    :param mode: XMODEM protocol mode
+    :param mode: Either ``xmodem`` or ``xmodem1k``, defaults to ``xmodem``.
     :type mode: string
     :param pad: Padding character to make the packets match the packet size
     :type pad: char
 
     '''
 
     # crctab calculated by Mark G. Mendel, Network Systems Corporation
@@ -277,31 +279,31 @@
                     self.log.debug('16-bit CRC requested (CRC).')
                     crc_mode = 1
                     break
                 elif char == CAN:
                     if not quiet:
                         print('received CAN', file=sys.stderr)
                     if cancel:
-                        self.log.info('Transmission canceled: received 2xCAN '
+                        self.log.info('Transmission canceled: received CAN CAN '
                                       'at start-sequence')
                         return False
                     else:
-                        self.log.debug('cancellation at start sequence.')
+                        self.log.debug('received CAN at start of sequence.')
                         cancel = 1
                 elif char == EOT:
                     self.log.info('Transmission canceled: received EOT '
                                   'at start-sequence')
                     return False
                 else:
                     self.log.error('send error: expected NAK, CRC, EOT or CAN; '
                                    'got %r', char)
 
             error_count += 1
             if error_count > retry:
-                self.log.info('send error: error_count reached %d, '
+                self.log.error('send error: error_count reached %d, '
                               'aborting.', retry)
                 self.abort(timeout=timeout)
                 return False
 
         # send data
         error_count = 0
         success_count = 0
@@ -325,14 +327,16 @@
                 self.putc(header + data + checksum)
                 char = self.getc(1, timeout)
                 if char == ACK:
                     success_count += 1
                     if callable(callback):
                         callback(total_packets, success_count, error_count)
                     error_count = 0
+                    # keep track of sequence
+                    sequence = (sequence + 1) % 0x100
                     break
 
                 self.log.error('send error: expected ACK; got %r for block %d',
                                char, sequence)
                 error_count += 1
                 if callable(callback):
                     callback(total_packets, success_count, error_count)
@@ -340,31 +344,32 @@
                     # excessive amounts of retransmissions requested,
                     # abort transfer
                     self.log.error('send error: NAK received %d times, '
                                    'aborting.', error_count)
                     self.abort(timeout=timeout)
                     return False
 
-            # keep track of sequence
-            sequence = (sequence + 1) % 0x100
+
 
         while True:
             self.log.debug('sending EOT, awaiting ACK')
             # end of transmission
             self.putc(EOT)
 
             # An ACK should be returned
             char = self.getc(1, timeout)
             if char == ACK:
                 break
             else:
                 self.log.error('send error: expected ACK; got %r', char)
                 error_count += 1
+                if callback:
+                    callback(total_packets, success_count, error_count)
                 if error_count > retry:
-                    self.log.warn('EOT was not ACKd, aborting transfer')
+                    self.log.warning('EOT was not ACKd, aborting transfer')
                     self.abort(timeout=timeout)
                     return False
 
         self.log.info('Transmission successful (ACK received).')
         return True
 
     def _make_send_header(self, packet_size, sequence):
@@ -383,95 +388,122 @@
             crc = self.calc_crc(data)
             _bytes.extend([crc >> 8, crc & 0xff])
         else:
             crc = self.calc_checksum(data)
             _bytes.append(crc)
         return bytearray(_bytes)
 
-    def recv(self, stream, crc_mode=1, retry=16, timeout=60, delay=1, quiet=0):
+    def recv(self, stream, crc_mode=1, retry=16, timeout=60, delay=1, quiet=0, callback=None):
         '''
         Receive a stream via the XMODEM protocol.
 
             >>> stream = open('/etc/issue', 'wb')
             >>> print(modem.recv(stream))
             2342
 
         Returns the number of bytes received on success or ``None`` in case of
         failure.
 
         :param stream: The stream object to write data to.
         :type stream: stream (file, etc.)
-        :param crc_mode: XMODEM CRC mode
+        :param crc_mode: XMODEM CRC mode, 0 is standard checksum, 1 is 16-bit checksum.
         :type crc_mode: int
         :param retry: The maximum number of times to try to resend a failed
                       packet before failing.
         :type retry: int
         :param timeout: The number of seconds to wait for a response before
                         timing out.
         :type timeout: int
         :param delay: The number of seconds to wait between resend attempts
         :type delay: int
         :param quiet: If ``True``, write transfer information to stderr.
         :type quiet: bool
+        :param callback: Reference to a callback function that has the
+                         following signature::
+
+                           def callback(total_packets: int, success_count: int, error_count: int, packet_size: int)
 
+                         This is useful for tracking progress state while an xmodem transfer is
+                         underway. As packet size may be negotiated, it also included as the final
+                         argument of the callback. note that the value of error_count resets to 0
+                         after any successful block transfer.
+        :type callback: callable
         '''
 
         # initiate protocol
         error_count = 0
-        char = 0
         cancel = 0
+        empty = 0
         while True:
             # first try CRC mode, if this fails,
             # fall back to checksum mode
             if error_count >= retry:
-                self.log.info('error_count reached %d, aborting.', retry)
+                self.log.error('error_count reached %d, aborting.', retry)
                 self.abort(timeout=timeout)
                 return None
             elif crc_mode and error_count < (retry // 2):
                 if not self.putc(CRC):
-                    self.log.debug('recv error: putc failed, '
-                                   'sleeping for %d', delay)
+                    self.log.warning('recv error: putc failed, '
+                                     'sleeping for %d', delay)
                     time.sleep(delay)
                     error_count += 1
             else:
                 crc_mode = 0
                 if not self.putc(NAK):
-                    self.log.debug('recv error: putc failed, '
-                                   'sleeping for %d', delay)
+                    self.log.warning('recv error: putc failed, '
+                                     'sleeping for %d', delay)
                     time.sleep(delay)
                     error_count += 1
 
             char = self.getc(1, timeout)
             if char is None:
-                self.log.warn('recv error: getc timeout in start sequence')
+                self.log.warning('recv error: getc timeout in start sequence')
                 error_count += 1
                 continue
             elif char == SOH:
                 self.log.debug('recv: SOH')
                 break
             elif char == STX:
                 self.log.debug('recv: STX')
                 break
             elif char == CAN:
                 if cancel:
                     self.log.info('Transmission canceled: received 2xCAN '
                                   'at start-sequence')
                     return None
                 else:
-                    self.log.debug('cancellation at start sequence.')
+                    self.log.debug('recv: CAN, cancellation at start sequence')
                     cancel = 1
+            elif char == EOT:
+                if empty:
+                    self.log.info('transmission canceled: file empty')
+                    self.putc(CAN)
+                    self.putc(CAN)
+                    # 'purge' any remaining data on the line
+                    while True:
+                        if self.getc(1, timeout=1) is None:
+                            break
+                        time.sleep(.001) # better cpu usage
+                    return 0
+                else:
+                    self.log.debug('first eot received ')
+                    empty = 1
             else:
                 error_count += 1
+                if callable(callback):
+                    callback(0, 0, error_count, 128)
 
         # read data
         error_count = 0
         income_size = 0
         packet_size = 128
         sequence = 1
         cancel = 0
+        total_packets = 0
+        success_count = 0
         while True:
             while True:
                 if char == SOH:
                     if packet_size != 128:
                         self.log.debug('recv: SOH, using 128b packet_size')
                         packet_size = 128
                     break
@@ -482,14 +514,16 @@
                     break
                 elif char == EOT:
                     # We received an EOT, so send an ACK and return the
                     # received data length.
                     self.putc(ACK)
                     self.log.info("Transmission complete, %d bytes",
                                   income_size)
+                    if callable(callback):
+                        callback(total_packets, success_count, error_count, packet_size)
                     return income_size
                 elif char == CAN:
                     # cancel at two consecutive cancels
                     if cancel:
                         self.log.info('Transmission canceled: received 2xCAN '
                                       'at block %d', sequence)
                         return None
@@ -497,114 +531,132 @@
                         self.log.debug('cancellation at block %d', sequence)
                         cancel = 1
                 else:
                     err_msg = ('recv error: expected SOH, EOT; '
                                'got {0!r}'.format(char))
                     if not quiet:
                         print(err_msg, file=sys.stderr)
-                    self.log.warn(err_msg)
+                    self.log.warning(err_msg)
                     error_count += 1
+                    if callable(callback):
+                        callback(total_packets, success_count, error_count, packet_size)
                     if error_count > retry:
                         self.log.info('error_count reached %d, aborting.',
                                       retry)
                         self.abort()
                         return None
+                    time.sleep(timeout)
+
+                # Reads next char from stream
+                char = self.getc(1, timeout=1)
 
             # read sequence
             error_count = 0
             cancel = 0
             self.log.debug('recv: data block %d', sequence)
             seq1 = self.getc(1, timeout)
             if seq1 is None:
-                self.log.warn('getc failed to get first sequence byte')
+                self.log.warning('getc failed to get first sequence byte')
                 seq2 = None
             else:
                 seq1 = ord(seq1)
                 seq2 = self.getc(1, timeout)
                 if seq2 is None:
-                    self.log.warn('getc failed to get second sequence byte')
+                    self.log.warning('getc failed to get second sequence byte')
                 else:
                     # second byte is the same as first as 1's complement
                     seq2 = 0xff - ord(seq2)
 
             if not (seq1 == seq2 == sequence):
                 # consume data anyway ... even though we will discard it,
                 # it is not the sequence we expected!
                 self.log.error('expected sequence %d, '
-                               'got (seq1=%r, seq2=%r), '
-                               'receiving next block, will NAK.',
-                               sequence, seq1, seq2)
+                               'got (seq1=%r, seq2=%r), reading next '
+                               '%d bytes, anyway',
+                               sequence, seq1, seq2,
+                               packet_size + 1 + crc_mode)
                 self.getc(packet_size + 1 + crc_mode)
             else:
                 # sequence is ok, read packet
                 # packet_size + checksum
                 data = self.getc(packet_size + 1 + crc_mode, timeout)
                 valid, data = self._verify_recv_checksum(crc_mode, data)
 
                 # valid data, append chunk
                 if valid:
+                    total_packets += 1
+                    success_count += 1
+                    if callable(callback):
+                        callback(total_packets, success_count, error_count, packet_size)
                     income_size += len(data)
                     stream.write(data)
                     self.putc(ACK)
                     sequence = (sequence + 1) % 0x100
                     # get next start-of-header byte
                     char = self.getc(1, timeout)
                     continue
 
             # something went wrong, request retransmission
-            self.log.warn('recv error: purge, requesting retransmission (NAK)')
+            self.log.warning('recv error: purge, requesting retransmission (NAK)')
+            n_purged = 0
             while True:
                 # When the receiver wishes to <nak>, it should call a "PURGE"
                 # subroutine, to wait for the line to clear. Recall the sender
                 # tosses any characters in its UART buffer immediately upon
                 # completing sending a block, to ensure no glitches were mis-
                 # interpreted.  The most common technique is for "PURGE" to
                 # call the character receive subroutine, specifying a 1-second
                 # timeout, and looping back to PURGE until a timeout occurs.
                 # The <nak> is then sent, ensuring the other end will see it.
                 data = self.getc(1, timeout=1)
                 if data is None:
                     break
+                n_purged = len(data)
+            if n_purged:
+                self.log.warning('%d bytes purged from receiver', n_purged)
+            error_count += 1
+            if callable(callback):
+                callback(total_packets, success_count, error_count, packet_size)
             self.putc(NAK)
             # get next start-of-header byte
             char = self.getc(1, timeout)
             continue
 
     def _verify_recv_checksum(self, crc_mode, data):
         if crc_mode:
             _checksum = bytearray(data[-2:])
             their_sum = (_checksum[0] << 8) + _checksum[1]
             data = data[:-2]
 
             our_sum = self.calc_crc(data)
             valid = bool(their_sum == our_sum)
             if not valid:
-                self.log.warn('recv error: checksum fail '
+                self.log.warning('recv error: checksum fail '
                               '(theirs=%04x, ours=%04x), ',
                               their_sum, our_sum)
         else:
             _checksum = bytearray([data[-1]])
             their_sum = _checksum[0]
             data = data[:-1]
 
             our_sum = self.calc_checksum(data)
             valid = their_sum == our_sum
             if not valid:
-                self.log.warn('recv error: checksum fail '
+                self.log.warning('recv error: checksum fail '
                               '(theirs=%02x, ours=%02x)',
                               their_sum, our_sum)
         return valid, data
 
     def calc_checksum(self, data, checksum=0):
         '''
         Calculate the checksum for a given block of data, can also be used to
         update a checksum.
 
-            >>> csum = modem.calc_checksum('hello')
-            >>> csum = modem.calc_checksum('world', csum)
+            >>> csum = modem.calc_checksum(b'hello')
+            >>> csum = modem.calc_checksum(b'world', csum)
             >>> hex(csum)
             '0x3c'
 
         '''
         if platform.python_version_tuple() >= ('3', '0', '0'):
             return (sum(data) + checksum) % 256
         else:
@@ -628,27 +680,27 @@
 
 
 XMODEM1k = partial(XMODEM, mode='xmodem1k')
 
 
 def _send(mode='xmodem', filename=None, timeout=30):
     '''Send a file (or stdin) using the selected mode.'''
-    
+
     if filename is None:
         si = sys.stdin
     else:
         si = open(filename, 'rb')
 
     # TODO(maze): make this configurable, serial out, etc.
     so = sys.stdout
 
     def _getc(size, timeout=timeout):
         read_ready, _, _ = select.select([so], [], [], timeout)
         if read_ready:
-            data = stream.read(size)
+            data = si.read(size)
         else:
             data = None
         return data
 
     def _putc(data, timeout=timeout):
         _, write_ready, _ = select.select([], [si], [], timeout)
         if write_ready:
@@ -662,121 +714,49 @@
     xmodem = XMODEM(_getc, _putc, mode)
     return xmodem.send(si)
 
 
 def run():
     '''Run the main entry point for sending and receiving files.'''
     import argparse
-    import serial
     import sys
 
     platform = sys.platform.lower()
 
     if platform.startswith('win'):
         default_port = 'COM1'
     else:
         default_port = '/dev/ttyS0'
 
     parser = argparse.ArgumentParser()
-    parser.add_argument('-p', '--port', default=default_port,
-                        help='serial port')
-    parser.add_argument('-r', '--rate', default=9600, type=int,
-                        help='baud rate')
-    parser.add_argument('-b', '--bytesize', default=serial.EIGHTBITS,
-                        help='serial port transfer byte size')
-    parser.add_argument('-P', '--parity', default=serial.PARITY_NONE,
-                        help='serial port parity')
-    parser.add_argument('-S', '--stopbits', default=serial.STOPBITS_ONE,
-                        help='serial port stop bits')
+    # parser.add_argument('-p', '--port', default=default_port,
+    #                     help='serial port')
+    # parser.add_argument('-r', '--rate', default=9600, type=int,
+    #                     help='baud rate')
+    # parser.add_argument('-b', '--bytesize', default=serial.EIGHTBITS,
+    #                     help='serial port transfer byte size')
+    # parser.add_argument('-P', '--parity', default=serial.PARITY_NONE,
+    #                     help='serial port parity')
+    # parser.add_argument('-S', '--stopbits', default=serial.STOPBITS_ONE,
+    #                     help='serial port stop bits')
     parser.add_argument('-m', '--mode', default='xmodem',
                         help='XMODEM mode (xmodem, xmodem1k)')
     parser.add_argument('-t', '--timeout', default=30, type=int,
                         help='I/O timeout in seconds')
 
     subparsers = parser.add_subparsers(dest='subcommand')
     send_parser = subparsers.add_parser('send')
     send_parser.add_argument('filename', nargs='?',
                              help='filename to send, empty reads from stdin')
     recv_parser = subparsers.add_parser('recv')
     recv_parser.add_argument('filename', nargs='?',
                              help='filename to receive, empty sends to stdout')
 
     options = parser.parse_args()
-    
+
     if options.subcommand == 'send':
         return _send(options.mode, options.filename, options.timeout)
-    elif options.subcommand == 'recv':
-        return _recv(options.mode, options.filename, options.timeout)
-
-
-def runx():
-    import optparse
-    import subprocess
-
-    parser = optparse.OptionParser(
-        usage='%prog [<options>] <send|recv> filename filename')
-    parser.add_option('-m', '--mode', default='xmodem',
-                      help='XMODEM mode (xmodem, xmodem1k)')
-
-    options, args = parser.parse_args()
-    if len(args) != 3:
-        parser.error('invalid arguments')
-        return 1
-
-    elif args[0] not in ('send', 'recv'):
-        parser.error('invalid mode')
-        return 1
-
-    def _func(so, si):
-        import select
-
-        print(('si', si))
-        print(('so', so))
-
-        def getc(size, timeout=3):
-            read_ready, _, _ = select.select([so], [], [], timeout)
-            if read_ready:
-                data = so.read(size)
-            else:
-                data = None
-
-            print(('getc(', repr(data), ')'))
-            return data
-
-        def putc(data, timeout=3):
-            _, write_ready, _ = select.select([], [si], [], timeout)
-            if write_ready:
-                si.write(data)
-                si.flush()
-                size = len(data)
-            else:
-                size = None
-
-            print(('putc(', repr(data), repr(size), ')'))
-            return size
-
-        return getc, putc
-
-    def _pipe(*command):
-        pipe = subprocess.Popen(command,
-                                stdout=subprocess.PIPE,
-                                stdin=subprocess.PIPE)
-        return pipe.stdout, pipe.stdin
-
-    if args[0] == 'recv':
-        getc, putc = _func(*_pipe('sz', '--xmodem', args[2]))
-        stream = open(args[1], 'wb')
-        xmodem = XMODEM(getc, putc, mode=options.mode)
-        status = xmodem.recv(stream, retry=8)
-        assert status, ('Transfer failed, status is', False)
-        stream.close()
-
-    elif args[0] == 'send':
-        getc, putc = _func(*_pipe('rz', '--xmodem', args[2]))
-        stream = open(args[1], 'rb')
-        xmodem = XMODEM(getc, putc, mode=options.mode)
-        sent = xmodem.send(stream, retry=8)
-        assert sent is not None, ('Transfer failed, sent is', sent)
-        stream.close()
+    # elif options.subcommand == 'recv':
+    #     return _recv(options.mode, options.filename, options.timeout)
 
 if __name__ == '__main__':
     sys.exit(run())
```

### Comparing `xmodem-0.4.6/setup.py` & `xmodem-0.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 HERE = os.path.dirname(__file__)
 README_RST = os.path.join(HERE, 'README.rst')
 
 setup(
     name='xmodem',
-    version='0.4.6',
+    version='0.4.7',
     author='Wijnand Modderman, Jeff Quast, Kris Hardy',
     author_email='maze@pyth0n.org',
     description=('XMODEM protocol implementation.'),
     url='https://github.com/tehmaze/xmodem',
     long_description = codecs.open(README_RST, 'rb', 'utf8').read(),
     license='MIT',
     keywords='xmodem protocol',
```

### Comparing `xmodem-0.4.6/doc/XMODMCRC.TXT` & `xmodem-0.4.7/doc/XMODMCRC.TXT`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Perception presents:
 ---------- Understanding The X-Modem CRC File Transfer Protocol --------------
 
 			      by Em Decay
 
 This has to be one of the most internationally accepted protocols for upload-
  ing and downloading binary and text files.  It is fairly straight-forward as
- to how it is set up and there are some error checking capablities.
+ to how it is set up and there are some error checking capabilities.
 
 
 --- Before you begin ---
 
 Look at my XMODEM.TXT text file for a general understanding of the X-Modem
  file transfer protocol and the terms used in it.
```

### Comparing `xmodem-0.4.6/doc/XMODEM1K.TXT` & `xmodem-0.4.7/doc/XMODEM1K.TXT`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Perception presents:
 ---------- Understanding The X-Modem 1K File Transfer Protocol --------------
 
 			      by Em Decay
 
 This has to be one of the most internationally accepted protocols for upload-
  ing and downloading binary and text files.  It is fairly straight-forward as
- to how it is set up and there are fairly good error checking capablities.
+ to how it is set up and there are fairly good error checking capabilities.
 
 
 --- Before you begin ---
 
 Look at my XMODEM.TXT and XMODEMCRC.TXT text file for a general understanding 
  of the X-Modem file transfer protocol and the terms used in it.
```

### Comparing `xmodem-0.4.6/doc/XMODEM.TXT` & `xmodem-0.4.7/doc/XMODEM.TXT`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Perception presents:
 ------------ Understanding The X-Modem File Transfer Protocol ---------------
 
 			      by Em Decay
 
 This has to be one of the most internationally accepted protocols for upload-
  ing and downloading binary and text files.  It is fairly straight-forward as
- to how it is set up and there are some error checking capablities.
+ to how it is set up and there are some error checking capabilities.
 
 
 --- Before you begin ---
 
 Things you need to know beforehand...
 
 The following terms are simply ascii codes:
@@ -20,26 +20,26 @@
     CAN = chr(24) = CTRL-X = Cancel
 
 In order to send the file, you must first divide it into 128 byte sections
  (packets).  Bytes 0-127 of the file make up the first packet, bytes 128-255
  make up the second packet, etc.
 
 The packet number sent is simply the number of the packet.  If the packet
- number is greater than 255, then subtract 256 repeatly until the number is
+ number is greater than 255, then subtract 256 repeatedly until the number is
  between 0 and 255.  For example, if you were sending packet 731, then you
  would send 731 - 256 - 256 = 219.
 
 The 1's complement of a byte (to make life easy) is simply 255 minus the
  byte.  For example, if you had to take the 1's complement of 142, the answer
  would be 255 - 142 = 113.
 
 The checksum is the value of all the bytes in the packet added together.  For
  example, if the first five bytes were 45, 12, 64, 236, 173 and the other 123
  bytes were zeroes, the checksum would be 45+12+64+236+173+0+0+...+0 = 530.
- However, to make each block one byte smaller, they repeatly subtract 256
+ However, to make each block one byte smaller, they repeatedly subtract 256
  from the checksum until it is between 0 and 255.  In this case, the checksum
  would be 530 - 256 - 256 = 18.
 
 The first byte the downloader sends is referred to as the NCGbyte.
 
 Provided that you aren't lost already, here is what happens next.  The steps
  below describe who sends what when :)
```

### Comparing `xmodem-0.4.6/doc/ymodem.txt` & `xmodem-0.4.7/doc/ymodem.txt`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 Recent advances	in computing, modems and networking have revealed a number
 of weaknesses in the original protocol:
 
    + The short block length caused throughput to suffer	when used with
      timesharing systems, packet switched networks, satellite circuits,
      and buffered (error correcting) modems.
 
-   + The 8 bit arithemetic checksum and	other aspects allowed line
+   + The 8 bit arithmetic checksum and	other aspects allowed line
      impairments to interfere with dependable, accurate	transfers.
 
    + Only one file could be sent per command.  The file	name had to be
      given twice, first	to the sending program and then	again to the
      receiving program.
 
    + The transmitted file could	accumulate as many as 127 extraneous
@@ -299,15 +299,15 @@
 
 
 3.  XMODEM PROTOCOL ENHANCEMENTS
 
 This chapter discusses the protocol extensions to Ward Christensen's 1982
 XMODEM protocol	description document.
 
-The original document recommends the user be asked wether to continue
+The original document recommends the user be asked whether to continue
 trying or abort	after 10 retries.  Most	programs no longer ask the
 operator whether he wishes to keep retrying.  Virtually	all correctable
 errors are corrected within the	first few retransmissions.  If the line	is
 so bad that ten	attempts are insufficient, there is a significant danger
 of undetected errors.  If the connection is that bad, it's better to
 redial for a better connection,	or mail	a floppy disk.
 
@@ -841,15 +841,15 @@
 The g option to	YMODEM has proven effective under these	circumstances.
 The g option is	driven by the receiver,	which initiates	the batch transfer
 by transmitting	a G instead of C.  When	the sender recognizes the G, it
 bypasses the usual wait	for an ACK to each transmitted packet, sending
 succeeding packets at full speed, subject to XOFF/XON or other flow
 control	exerted	by the medium.
 
-The sender expects an inital G to initiate the transmission of a
+The sender expects an initial G to initiate the transmission of a
 particular file, and also expects an ACK on the	EOT sent at the	end of
 each file.  This synchronization allows	the receiver time to open and
 
 
 
 Chapter	5				      XMODEM Protocol Enhancements
```

### Comparing `xmodem-0.4.6/README.rst` & `xmodem-0.4.7/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,16 @@
  XMODEM protocol implementation
 ================================
 
 Documentation available at http://packages.python.org/xmodem/
 
 Python Package Index (PyPI) page is available at https://pypi.python.org/pypi/xmodem
 
+xmodem has been tested with python 2.7 through python 3.11
+
 Usage
 =====
 
 Create a function to get and put character data (to a serial line for
 example)::
 
     >>> import serial
@@ -41,14 +43,28 @@
 
 For more information, take a look at the documentation_.
 
 .. _documentation: http://packages.python.org/xmodem/xmodem.html
 
 Changes
 =======
+0.4.7:
+   * bugfix: stall on some kinds of error in ``recv()``, `PR #56
+     <https://github.com/tehmaze/xmodem/pull/56>`_.
+   * bugfix: sequence number miscalculation in ``send()``, `PR #52
+     <https://github.com/tehmaze/xmodem/pull/52>`_.
+   * enhancement: callback function added for ``recv()``, `PR #53
+     <https://github.com/tehmaze/xmodem/pull/53>`_.
+   * bugfix: receiving empty file and stall condition in ``recv()``, `PR #50
+     <https://github.com/tehmaze/xmodem/pull/50>`_.
+   * bugfix: callback is now called for some kinds of errors
+     and some CLI fixes, `8a798e8b
+     <https://github.com/tehmaze/xmodem/commit/8a798e8b2af2a9cd6f9e789ef154a23a6467f98b>`_.
+   * bugfix: remove DepreactionWarning for ``logging.warn()``, `PR #49
+     <https://github.com/tehmaze/xmodem/pull/49>`_.
 
 0.4.6:
   * bugfix: Abort send on EOT in startup-sequence `Issue #34 
     <https://github.com/tehmaze/xmodem/issues/34>`_.
   * enhancement: Include LICENSE file in the source distribution.
 
 0.4.5:
```

### Comparing `xmodem-0.4.6/xmodem.egg-info/PKG-INFO` & `xmodem-0.4.7/xmodem.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,100 +1,116 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: xmodem
-Version: 0.4.6
+Version: 0.4.7
 Summary: XMODEM protocol implementation.
 Home-page: https://github.com/tehmaze/xmodem
 Author: Wijnand Modderman, Jeff Quast, Kris Hardy
 Author-email: maze@pyth0n.org
 License: MIT
-Description: .. image:: https://travis-ci.org/tehmaze/xmodem.png?branch=master
-           :target: https://travis-ci.org/tehmaze/xmodem
-        
-        .. image:: https://coveralls.io/repos/tehmaze/xmodem/badge.png
-           :target: https://coveralls.io/r/tehmaze/xmodem
-        
-        ================================
-         XMODEM protocol implementation
-        ================================
-        
-        Documentation available at http://packages.python.org/xmodem/
-        
-        Python Package Index (PyPI) page is available at https://pypi.python.org/pypi/xmodem
-        
-        Usage
-        =====
-        
-        Create a function to get and put character data (to a serial line for
-        example)::
-        
-            >>> import serial
-            >>> from xmodem import XMODEM
-            >>> ser = serial.Serial('/dev/ttyUSB0', timeout=0) # or whatever port you need
-            >>> def getc(size, timeout=1):
-            ...     return ser.read(size) or None
-            ...
-            >>> def putc(data, timeout=1):
-            ...     return ser.write(data)  # note that this ignores the timeout
-            ...
-            >>> modem = XMODEM(getc, putc)
-        
-        Now, to upload a file, use the ``send`` method::
-        
-            >>> stream = open('/etc/fstab', 'rb')
-            >>> modem.send(stream)
-        
-        To download a file, use the ``recv`` method::
-        
-            >>> stream = open('output', 'wb')
-            >>> modem.recv(stream)
-        
-        For more information, take a look at the documentation_.
-        
-        .. _documentation: http://packages.python.org/xmodem/xmodem.html
-        
-        Changes
-        =======
-        
-        0.4.6:
-          * bugfix: Abort send on EOT in startup-sequence `Issue #34 
-            <https://github.com/tehmaze/xmodem/issues/34>`_.
-          * enhancement: Include LICENSE file in the source distribution.
-        
-        0.4.5:
-          * bugfix: Remove bogus `assert False` code in ``recv()`` that resulted in
-            `AssertionError` introduced in version 0.4.0 commit-id `9b03fc20`, `PR #29
-            <https://github.com/tehmaze/xmodem/pull/29>`_.
-        
-        0.4.4:
-          * bugfix: Large file transfers in ``send()`` were more likely to fail for
-            small values of ``retry``: This value should be the maximum failures per
-            block transfer as documented, but was improperly implemented as the number
-            of failures allowed for the total duration of the transfer, `PR #21
-            <https://github.com/tehmaze/xmodem/pull/21>`_.
-          * bugfix: ``send(retry=n)`` and ``recv(retry=n)`` should retry ``n`` times
-            as documented, was retrying ``n - 1``.
-        
-        0.4.3:
-          * bugfix: ``putc()`` callback was called in series, 3 times for each part of
-            xmodem block header, data, and checksum during block transfer.  Now all
-            three data blocks are sent by single ``putc()`` call.  This resolves issues
-            when integrating with microcontrollers or equipment sensitive to timing
-            issues at stream boundaries, `PR #19
-            <https://github.com/tehmaze/xmodem/pull/19>`_.
-        
-        0.4.2:
-          * bugfix: documentation files missing from the release tarball
-            `Issue #16 <https://github.com/tehmaze/xmodem/issues/16>`_.
-        
-        0.4.1
-          * bugfix: re-transmit in ``send()`` on ``NAK`` or timeout, previously
-            re-transmissions (wrongly) occurred only on garbage bytes.
-            `PR #12 <https://github.com/tehmaze/xmodem/pull/12>`_.
-        
-        0.4.0
-          * enhancement: support for python 3
-            `PR #8 <https://github.com/tehmaze/xmodem/pull/8>`_.
-          * bugfix: CRC failures in XMODEM.recv() were not renegotiated correctly
-            `PR #11 <https://github.com/tehmaze/xmodem/issues/11>`_.
-        
 Keywords: xmodem protocol
-Platform: UNKNOWN
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/tehmaze/xmodem.png?branch=master
+   :target: https://travis-ci.org/tehmaze/xmodem
+
+.. image:: https://coveralls.io/repos/tehmaze/xmodem/badge.png
+   :target: https://coveralls.io/r/tehmaze/xmodem
+
+================================
+ XMODEM protocol implementation
+================================
+
+Documentation available at http://packages.python.org/xmodem/
+
+Python Package Index (PyPI) page is available at https://pypi.python.org/pypi/xmodem
+
+xmodem has been tested with python 2.7 through python 3.11
+
+Usage
+=====
+
+Create a function to get and put character data (to a serial line for
+example)::
+
+    >>> import serial
+    >>> from xmodem import XMODEM
+    >>> ser = serial.Serial('/dev/ttyUSB0', timeout=0) # or whatever port you need
+    >>> def getc(size, timeout=1):
+    ...     return ser.read(size) or None
+    ...
+    >>> def putc(data, timeout=1):
+    ...     return ser.write(data)  # note that this ignores the timeout
+    ...
+    >>> modem = XMODEM(getc, putc)
+
+Now, to upload a file, use the ``send`` method::
+
+    >>> stream = open('/etc/fstab', 'rb')
+    >>> modem.send(stream)
+
+To download a file, use the ``recv`` method::
+
+    >>> stream = open('output', 'wb')
+    >>> modem.recv(stream)
+
+For more information, take a look at the documentation_.
+
+.. _documentation: http://packages.python.org/xmodem/xmodem.html
+
+Changes
+=======
+0.4.7:
+   * bugfix: stall on some kinds of error in ``recv()``, `PR #56
+     <https://github.com/tehmaze/xmodem/pull/56>`_.
+   * bugfix: sequence number miscalculation in ``send()``, `PR #52
+     <https://github.com/tehmaze/xmodem/pull/52>`_.
+   * enhancement: callback function added for ``recv()``, `PR #53
+     <https://github.com/tehmaze/xmodem/pull/53>`_.
+   * bugfix: receiving empty file and stall condition in ``recv()``, `PR #50
+     <https://github.com/tehmaze/xmodem/pull/50>`_.
+   * bugfix: callback is now called for some kinds of errors
+     and some CLI fixes, `8a798e8b
+     <https://github.com/tehmaze/xmodem/commit/8a798e8b2af2a9cd6f9e789ef154a23a6467f98b>`_.
+   * bugfix: remove DepreactionWarning for ``logging.warn()``, `PR #49
+     <https://github.com/tehmaze/xmodem/pull/49>`_.
+
+0.4.6:
+  * bugfix: Abort send on EOT in startup-sequence `Issue #34 
+    <https://github.com/tehmaze/xmodem/issues/34>`_.
+  * enhancement: Include LICENSE file in the source distribution.
+
+0.4.5:
+  * bugfix: Remove bogus `assert False` code in ``recv()`` that resulted in
+    `AssertionError` introduced in version 0.4.0 commit-id `9b03fc20`, `PR #29
+    <https://github.com/tehmaze/xmodem/pull/29>`_.
+
+0.4.4:
+  * bugfix: Large file transfers in ``send()`` were more likely to fail for
+    small values of ``retry``: This value should be the maximum failures per
+    block transfer as documented, but was improperly implemented as the number
+    of failures allowed for the total duration of the transfer, `PR #21
+    <https://github.com/tehmaze/xmodem/pull/21>`_.
+  * bugfix: ``send(retry=n)`` and ``recv(retry=n)`` should retry ``n`` times
+    as documented, was retrying ``n - 1``.
+
+0.4.3:
+  * bugfix: ``putc()`` callback was called in series, 3 times for each part of
+    xmodem block header, data, and checksum during block transfer.  Now all
+    three data blocks are sent by single ``putc()`` call.  This resolves issues
+    when integrating with microcontrollers or equipment sensitive to timing
+    issues at stream boundaries, `PR #19
+    <https://github.com/tehmaze/xmodem/pull/19>`_.
+
+0.4.2:
+  * bugfix: documentation files missing from the release tarball
+    `Issue #16 <https://github.com/tehmaze/xmodem/issues/16>`_.
+
+0.4.1
+  * bugfix: re-transmit in ``send()`` on ``NAK`` or timeout, previously
+    re-transmissions (wrongly) occurred only on garbage bytes.
+    `PR #12 <https://github.com/tehmaze/xmodem/pull/12>`_.
+
+0.4.0
+  * enhancement: support for python 3
+    `PR #8 <https://github.com/tehmaze/xmodem/pull/8>`_.
+  * bugfix: CRC failures in XMODEM.recv() were not renegotiated correctly
+    `PR #11 <https://github.com/tehmaze/xmodem/issues/11>`_.
```

