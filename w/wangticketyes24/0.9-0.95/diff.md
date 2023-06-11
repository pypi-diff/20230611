# Comparing `tmp/wangticketyes24-0.9-py3-none-any.whl.zip` & `tmp/wangticketyes24-0.95-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 28236 bytes, number of entries: 12
--rw-r--r--  2.0 unx      114 b- defN 23-May-27 04:26 wangticketyes24/__init__.py
--rw-r--r--  2.0 unx    28119 b- defN 23-May-27 04:26 wangticketyes24/selenium_yes24.py
--rw-r--r--  2.0 unx    43060 b- defN 23-May-27 03:56 wangticketyes24/yes24.py
+Zip file size: 28285 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      115 b- defN 23-Jun-11 00:46 wangticketyes24/__init__.py
+-rw-r--r--  2.0 unx    28280 b- defN 23-Jun-11 00:43 wangticketyes24/selenium_yes24.py
+-rw-r--r--  2.0 unx    43062 b- defN 23-Jun-11 00:43 wangticketyes24/yes24.py
 -rw-r--r--  2.0 unx       94 b- defN 18-Dec-12 13:54 yes24ticket/__init__.py
 -rw-r--r--  2.0 unx     7490 b- defN 18-Dec-12 14:11 yes24ticket/selenium_yes24.py
 -rw-r--r--  2.0 unx    15460 b- defN 18-Dec-12 14:12 yes24ticket/yes24test.py
--rw-r--r--  2.0 unx       61 b- defN 23-May-27 04:28 wangticketyes24-0.9.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx      690 b- defN 23-May-27 04:28 wangticketyes24-0.9.dist-info/metadata.json
--rw-r--r--  2.0 unx       16 b- defN 23-May-27 04:28 wangticketyes24-0.9.dist-info/top_level.txt
--rw-r--r--  2.0 unx       92 b- defN 23-May-27 04:28 wangticketyes24-0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx      575 b- defN 23-May-27 04:28 wangticketyes24-0.9.dist-info/METADATA
--rw-r--r--  2.0 unx     1034 b- defN 23-May-27 04:28 wangticketyes24-0.9.dist-info/RECORD
-12 files, 96805 bytes uncompressed, 26502 bytes compressed:  72.6%
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-11 00:47 wangticketyes24-0.95.dist-info/DESCRIPTION.rst
+-rw-r--r--  2.0 unx      691 b- defN 23-Jun-11 00:47 wangticketyes24-0.95.dist-info/metadata.json
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-11 00:47 wangticketyes24-0.95.dist-info/top_level.txt
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 00:47 wangticketyes24-0.95.dist-info/WHEEL
+-rw-r--r--  2.0 unx      576 b- defN 23-Jun-11 00:47 wangticketyes24-0.95.dist-info/METADATA
+-rw-r--r--  2.0 unx     1040 b- defN 23-Jun-11 00:47 wangticketyes24-0.95.dist-info/RECORD
+12 files, 96977 bytes uncompressed, 26539 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: yes24ticket/selenium_yes24.py
 Comment: 
 
 Filename: yes24ticket/yes24test.py
 Comment: 
 
-Filename: wangticketyes24-0.9.dist-info/DESCRIPTION.rst
+Filename: wangticketyes24-0.95.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: wangticketyes24-0.9.dist-info/metadata.json
+Filename: wangticketyes24-0.95.dist-info/metadata.json
 Comment: 
 
-Filename: wangticketyes24-0.9.dist-info/top_level.txt
+Filename: wangticketyes24-0.95.dist-info/top_level.txt
 Comment: 
 
-Filename: wangticketyes24-0.9.dist-info/WHEEL
+Filename: wangticketyes24-0.95.dist-info/WHEEL
 Comment: 
 
-Filename: wangticketyes24-0.9.dist-info/METADATA
+Filename: wangticketyes24-0.95.dist-info/METADATA
 Comment: 
 
-Filename: wangticketyes24-0.9.dist-info/RECORD
+Filename: wangticketyes24-0.95.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wangticketyes24/__init__.py

```diff
@@ -1,5 +1,5 @@
 name = "wangticketyes24"
-__version__ = "0.9"
+__version__ = "0.95"
 
 from .yes24 import Yes24
 from .selenium_yes24 import Selenium_yes24
```

## wangticketyes24/selenium_yes24.py

```diff
@@ -697,18 +697,24 @@
 					print(traceback.format_exc())
 					# alert text check
 					# 주문이 완료되었습니다.
 					# 이용해 주셔서 감사합니다.
 
 					alert = self.driver.switch_to.alert
 					alertText = alert.text
-					msg = "[{}] alert:{} (seat:{})".format(self.userid, alertText, trying_seat)
-					print(msg)
-					self.notifyTelegram(message=msg)
-					time.sleep(10)
+
+					if '자동주문방지 문자를 잘못 입력하셨습니다' in alertText:
+						alert.accept()
+						print("alert accepted")
+						break
+					else:
+						msg = "[{}] alert:{} (seat:{})".format(self.userid, alertText, trying_seat)
+						print(msg)
+						self.notifyTelegram(message=msg)
+						time.sleep(10)
 
 				except WebDriverException as e:
 					print(traceback.format_exc())
 					print("This error temporarily happens in Windows..")
 				time.sleep(1)
 
 			self.driver.implicitly_wait(5)
```

## wangticketyes24/yes24.py

```diff
@@ -537,16 +537,16 @@
 	def _lockSeat(self, block, date, idtime, seats):
 		if len(seats) == 0:
 			return False
 
 		self.triedSeats.extend(seats)
 
 		#### TEST CODE [S]
-		print("Lock fake done")
-		return True
+		#print("Lock fake done")
+		#return True
 		#### TEST CODE [E]
 
 		mytoken = ",".join([seat.seatid for seat in seats])
 		print(date, idtime, mytoken)
 		[print(seat) for seat in seats]
 		#myptags = "".join([seat.getPTag() for seat in seats])
 		#print(myptags)
```

## Comparing `wangticketyes24-0.9.dist-info/metadata.json` & `wangticketyes24-0.95.dist-info/metadata.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.95'"}*

```diff
@@ -33,9 +33,9 @@
                 "beautifulsoup4",
                 "requests",
                 "selenium"
             ]
         }
     ],
     "summary": "wangticket for y",
-    "version": "0.9"
+    "version": "0.95"
 }
```

## Comparing `wangticketyes24-0.9.dist-info/METADATA` & `wangticketyes24-0.95.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: wangticketyes24
-Version: 0.9
+Version: 0.95
 Summary: wangticket for y
 Home-page: https://gitlab.com/wangticket/yes24-ticket
 Author: Wangticket
 Author-email: wangticket77@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `wangticketyes24-0.9.dist-info/RECORD` & `wangticketyes24-0.95.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-wangticketyes24/__init__.py,sha256=-OyKPe-HRsDsrSGNIrn0hDrS78nLI4zS7c05Ehwwrx8,114
-wangticketyes24/selenium_yes24.py,sha256=ehj760D8oJsqTJOGCvyPtF_veEibWULjyZRzA_BPg1U,28119
-wangticketyes24/yes24.py,sha256=vXsSawgcRQ8Vbj8nYPC_g0JKKcz-fMeLfY6Ekg8EKBE,43060
-wangticketyes24-0.9.dist-info/DESCRIPTION.rst,sha256=iA1-u5zGsM2eQRcqv1-vqBiJevH0U-KhtkZxpjzmfx4,61
-wangticketyes24-0.9.dist-info/METADATA,sha256=QKnByf54JZHim-I3OAvFGNCEFObSMfYOx1beQeJMTwM,575
-wangticketyes24-0.9.dist-info/RECORD,,
-wangticketyes24-0.9.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
-wangticketyes24-0.9.dist-info/metadata.json,sha256=HWJfyAi3SJbVjgpc_Bsv84LPZUqwm05bFgjWbbQAm7Y,690
-wangticketyes24-0.9.dist-info/top_level.txt,sha256=gHGxU_Wfy3Ly7zkKLxm67DoXktNcwN0ImDzlhzNaiW4,16
+wangticketyes24/__init__.py,sha256=mg8SLW1u3fUWHX7YUUeEdxApvI5Ny1ohXzIHeYhNG58,115
+wangticketyes24/selenium_yes24.py,sha256=maWgh1gXUw8-LqKkXcAZHuhyluyvwymUBK-8PUC2uek,28280
+wangticketyes24/yes24.py,sha256=943Mh-foz9fwlJ_931tgJpvDzmHqWSp2EwXquVHW5UM,43062
+wangticketyes24-0.95.dist-info/DESCRIPTION.rst,sha256=iA1-u5zGsM2eQRcqv1-vqBiJevH0U-KhtkZxpjzmfx4,61
+wangticketyes24-0.95.dist-info/METADATA,sha256=C76O0kpMd06iKBJUVBxLQtSaHZ3C1N-8hhyiEPFidTI,576
+wangticketyes24-0.95.dist-info/RECORD,,
+wangticketyes24-0.95.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
+wangticketyes24-0.95.dist-info/metadata.json,sha256=6FFk8-Djfbt-vA6xN5jSjL6sEMd6oiA-T7j9rtZGpP4,691
+wangticketyes24-0.95.dist-info/top_level.txt,sha256=gHGxU_Wfy3Ly7zkKLxm67DoXktNcwN0ImDzlhzNaiW4,16
 yes24ticket/__init__.py,sha256=amffzfln3WNiLWWyUul39xXObS4TmQRza8OBgfN24M8,94
 yes24ticket/selenium_yes24.py,sha256=z6ataHl-e3AVhQTZFSYPdn1OfSOklBTizd2mLA57DAM,7490
 yes24ticket/yes24test.py,sha256=6my-oQh4NITv3IkaT_W_v61Z5iPDqNmDU6b3Qx9N5l8,15460
```

