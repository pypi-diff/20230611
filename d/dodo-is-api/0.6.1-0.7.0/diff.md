# Comparing `tmp/dodo_is_api-0.6.1.tar.gz` & `tmp/dodo_is_api-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dodo_is_api-0.6.1.tar", max compression
+gzip compressed data, was "dodo_is_api-0.7.0.tar", max compression
```

## Comparing `dodo_is_api-0.6.1.tar` & `dodo_is_api-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,25 @@
--rw-r--r--   0        0        0     1075 2023-03-22 13:32:15.868970 dodo_is_api-0.6.1/LICENSE
--rw-r--r--   0        0        0     3628 2023-03-24 05:03:49.211961 dodo_is_api-0.6.1/README.md
--rw-r--r--   0        0        0        0 2023-03-18 06:06:54.111388 dodo_is_api-0.6.1/dodo_is_api/__init__.py
--rw-r--r--   0        0        0       55 2023-05-10 05:26:32.091241 dodo_is_api-0.6.1/dodo_is_api/connection/__init__.py
--rw-r--r--   0        0        0     3607 2023-06-10 06:32:02.342004 dodo_is_api-0.6.1/dodo_is_api/connection/asynchronous.py
--rw-r--r--   0        0        0     1291 2023-05-10 05:26:32.091787 dodo_is_api-0.6.1/dodo_is_api/connection/base.py
--rw-r--r--   0        0        0     2131 2023-03-18 06:06:54.112897 dodo_is_api-0.6.1/dodo_is_api/connection/http_clients.py
--rw-r--r--   0        0        0     8913 2023-06-10 06:30:13.600381 dodo_is_api-0.6.1/dodo_is_api/connection/synchronous.py
--rw-r--r--   0        0        0      248 2023-03-18 06:06:54.113625 dodo_is_api-0.6.1/dodo_is_api/exceptions.py
--rw-r--r--   0        0        0      583 2023-06-10 06:25:28.732549 dodo_is_api-0.6.1/dodo_is_api/logger.py
--rw-r--r--   0        0        0     8145 2023-06-10 06:09:51.664171 dodo_is_api-0.6.1/dodo_is_api/mappers.py
--rw-r--r--   0        0        0       45 2023-03-18 11:36:04.461463 dodo_is_api-0.6.1/dodo_is_api/models/__init__.py
--rw-r--r--   0        0        0     3110 2023-06-10 06:07:19.624806 dodo_is_api-0.6.1/dodo_is_api/models/dodo_is_api.py
--rw-r--r--   0        0        0     1938 2023-06-10 05:51:51.801439 dodo_is_api-0.6.1/dodo_is_api/models/raw.py
--rw-r--r--   0        0        0      561 2023-06-10 06:44:45.178633 dodo_is_api-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4440 1970-01-01 00:00:00.000000 dodo_is_api-0.6.1/setup.py
--rw-r--r--   0        0        0     4002 1970-01-01 00:00:00.000000 dodo_is_api-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-03-22 13:32:15.868970 dodo_is_api-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2689 2023-06-11 19:00:32.393182 dodo_is_api-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-18 06:06:54.111388 dodo_is_api-0.7.0/dodo_is_api/__init__.py
+-rw-r--r--   0        0        0       55 2023-05-10 05:26:32.091241 dodo_is_api-0.7.0/dodo_is_api/connection/__init__.py
+-rw-r--r--   0        0        0    16088 2023-06-11 18:35:09.363455 dodo_is_api-0.7.0/dodo_is_api/connection/asynchronous.py
+-rw-r--r--   0        0        0     3055 2023-06-11 18:22:28.674699 dodo_is_api-0.7.0/dodo_is_api/connection/base.py
+-rw-r--r--   0        0        0    15937 2023-06-11 18:35:09.368594 dodo_is_api-0.7.0/dodo_is_api/connection/synchronous.py
+-rw-r--r--   0        0        0      248 2023-03-18 06:06:54.113625 dodo_is_api-0.7.0/dodo_is_api/exceptions.py
+-rw-r--r--   0        0        0      583 2023-06-11 08:10:22.290413 dodo_is_api-0.7.0/dodo_is_api/logger.py
+-rw-r--r--   0        0        0      419 2023-06-11 13:11:06.903175 dodo_is_api-0.7.0/dodo_is_api/models/__init__.py
+-rw-r--r--   0        0        0      149 2023-06-11 08:39:51.057307 dodo_is_api-0.7.0/dodo_is_api/models/channel_stop_types.py
+-rw-r--r--   0        0        0      349 2023-06-11 08:21:43.504521 dodo_is_api-0.7.0/dodo_is_api/models/country_codes.py
+-rw-r--r--   0        0        0     1486 2023-06-11 18:45:38.105232 dodo_is_api-0.7.0/dodo_is_api/models/courier_orders.py
+-rw-r--r--   0        0        0     1003 2023-06-11 18:41:47.749513 dodo_is_api-0.7.0/dodo_is_api/models/delivery_statistics.py
+-rw-r--r--   0        0        0      174 2023-06-11 08:41:14.500495 dodo_is_api-0.7.0/dodo_is_api/models/delivery_transport_names.py
+-rw-r--r--   0        0        0      795 2023-06-11 18:37:40.416183 dodo_is_api-0.7.0/dodo_is_api/models/late_delivery_vouchers.py
+-rw-r--r--   0        0        0      308 2023-06-11 13:11:06.905522 dodo_is_api-0.7.0/dodo_is_api/models/order_sources.py
+-rw-r--r--   0        0        0      582 2023-06-11 18:27:52.552568 dodo_is_api-0.7.0/dodo_is_api/models/orders_handover_statistics.py
+-rw-r--r--   0        0        0      804 2023-06-11 18:27:52.555279 dodo_is_api-0.7.0/dodo_is_api/models/orders_handover_time.py
+-rw-r--r--   0        0        0      716 2023-06-11 18:27:52.548339 dodo_is_api-0.7.0/dodo_is_api/models/production_productivity_statistics.py
+-rw-r--r--   0        0        0      161 2023-06-11 08:37:28.682394 dodo_is_api-0.7.0/dodo_is_api/models/sales_channels.py
+-rw-r--r--   0        0        0     1050 2023-06-11 18:32:37.831792 dodo_is_api-0.7.0/dodo_is_api/models/stop_sales.py
+-rw-r--r--   0        0        0      582 2023-06-11 19:01:00.460213 dodo_is_api-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3521 1970-01-01 00:00:00.000000 dodo_is_api-0.7.0/setup.py
+-rw-r--r--   0        0        0     3105 1970-01-01 00:00:00.000000 dodo_is_api-0.7.0/PKG-INFO
```

### Comparing `dodo_is_api-0.6.1/LICENSE` & `dodo_is_api-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.6.1/README.md` & `dodo_is_api-0.7.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,227 +1,169 @@
-00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
-00000010: 6572 223e 0a3c 6120 6872 6566 3d22 6874  er">.<a href="ht
-00000020: 7470 733a 2f2f 646f 646f 2d62 7261 6e64  tps://dodo-brand
-00000030: 732e 7374 6f70 6c69 6768 742e 696f 223e  s.stoplight.io">
-00000040: 0a3c 696d 6720 7769 6474 683d 2233 3530  .<img width="350
-00000050: 7078 2220 7372 633d 2268 7474 7073 3a2f  px" src="https:/
-00000060: 2f61 7069 2e68 756e 7466 6c6f 772e 696f  /api.huntflow.io
-00000070: 2f6c 6f67 6f2f 3836 3664 6633 6335 3865  /logo/866df3c58e
-00000080: 6134 3463 3135 3863 3665 3336 3031 3036  a44c158c6e360106
-00000090: 3331 6664 3966 2e6a 7067 223e 0a3c 2f61  31fd9f.jpg">.</a
-000000a0: 3e0a 3c2f 6469 763e 0a20 2020 200a 3c68  >.</div>.    .<h
-000000b0: 3120 616c 6967 6e3d 2263 656e 7465 7222  1 align="center"
-000000c0: 3e0a f09f 8d95 2044 6f64 6f20 4953 2041  >..... Dodo IS A
-000000d0: 5049 2057 7261 7070 6572 0a3c 2f68 313e  PI Wrapper.</h1>
-000000e0: 0a0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
-000000f0: 6572 223e 0a3c 6120 6872 6566 3d22 6874  er">.<a href="ht
-00000100: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000110: 2f67 6f72 6574 736b 792d 696e 7465 6772  /goretsky-integr
-00000120: 6174 696f 6e2f 646f 646f 2d69 732d 6170  ation/dodo-is-ap
-00000130: 692d 7079 7468 6f6e 2d77 7261 7070 6572  i-python-wrapper
-00000140: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000150: 7773 2f75 6e69 7474 6573 742e 7961 6d6c  ws/unittest.yaml
-00000160: 223e 0a3c 696d 6720 7372 633d 2268 7474  ">.<img src="htt
-00000170: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000180: 676f 7265 7473 6b79 2d69 6e74 6567 7261  goretsky-integra
-00000190: 7469 6f6e 2f64 6f64 6f2d 6973 2d61 7069  tion/dodo-is-api
-000001a0: 2d70 7974 686f 6e2d 7772 6170 7065 722f  -python-wrapper/
-000001b0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-000001c0: 732f 756e 6974 7465 7374 2e79 616d 6c2f  s/unittest.yaml/
-000001d0: 6261 6467 652e 7376 6722 2061 6c74 3d22  badge.svg" alt="
-000001e0: 5465 7374 2062 6164 6765 223e 0a3c 2f61  Test badge">.</a
-000001f0: 3e0a 3c61 2068 7265 663d 2268 7474 7073  >.<a href="https
-00000200: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
-00000210: 2f67 6f72 6574 736b 792d 696e 7465 6772  /goretsky-integr
-00000220: 6174 696f 6e2f 646f 646f 2d69 732d 6170  ation/dodo-is-ap
-00000230: 692d 7079 7468 6f6e 2d77 7261 7070 6572  i-python-wrapper
-00000240: 223e 0a3c 696d 6720 7372 633d 2268 7474  ">.<img src="htt
-00000250: 7073 3a2f 2f63 6f64 6563 6f76 2e69 6f2f  ps://codecov.io/
-00000260: 6768 2f67 6f72 6574 736b 792d 696e 7465  gh/goretsky-inte
-00000270: 6772 6174 696f 6e2f 646f 646f 2d69 732d  gration/dodo-is-
-00000280: 6170 692d 7079 7468 6f6e 2d77 7261 7070  api-python-wrapp
-00000290: 6572 2f62 7261 6e63 682f 6d61 696e 2f67  er/branch/main/g
-000002a0: 7261 7068 2f62 6164 6765 2e73 7667 3f74  raph/badge.svg?t
-000002b0: 6f6b 656e 3d75 6e7a 6c4d 6d41 6a73 4422  oken=unzlMmAjsD"
-000002c0: 2f3e 0a3c 2f61 3e0a 3c69 6d67 2073 7263  />.</a>.<img src
-000002d0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-000002e0: 6965 6c64 732e 696f 2f62 6164 6765 2f70  ields.io/badge/p
-000002f0: 7974 686f 6e2d 332e 3131 2d62 7269 6768  ython-3.11-brigh
-00000300: 7467 7265 656e 2220 616c 743d 2270 7974  tgreen" alt="pyt
-00000310: 686f 6e22 3e0a 3c2f 703e 0a0a 2d2d 2d0a  hon">.</p>..---.
-00000320: 0a23 2323 2049 6e73 7461 6c6c 6174 696f  .### Installatio
-00000330: 6e0a 0a56 6961 2070 6970 3a0a 6060 6073  n..Via pip:.```s
-00000340: 6865 6c6c 0a70 6970 2069 6e73 7461 6c6c  hell.pip install
-00000350: 2064 6f64 6f2d 6973 2d61 7069 0a60 6060   dodo-is-api.```
-00000360: 0a0a 5669 6120 706f 6574 7279 3a0a 6060  ..Via poetry:.``
-00000370: 6073 6865 6c6c 0a70 6f65 7472 7920 6164  `shell.poetry ad
-00000380: 6420 646f 646f 2d69 732d 6170 690a 6060  d dodo-is-api.``
-00000390: 600a 0a2d 2d2d 0a0a 2323 2323 20f0 9f93  `..---..#### ...
-000003a0: 9d20 5b43 6861 6e67 656c 6f67 5d28 6874  . [Changelog](ht
-000003b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000003c0: 2f67 6f72 6574 736b 792d 696e 7465 6772  /goretsky-integr
-000003d0: 6174 696f 6e2f 646f 646f 2d69 732d 6170  ation/dodo-is-ap
-000003e0: 692d 7079 7468 6f6e 2d77 7261 7070 6572  i-python-wrapper
-000003f0: 2f62 6c6f 622f 6d61 696e 2f43 4841 4e47  /blob/main/CHANG
-00000400: 454c 4f47 2e6d 6429 2069 7320 6865 7265  ELOG.md) is here
-00000410: 2e0a 0a2d 2d2d 0a0a 2323 2320 f09f a7aa  ...---..### ....
-00000420: 2055 7361 6765 3a0a 0a2d 2044 656c 6976   Usage:..- Deliv
-00000430: 6572 793a 0a20 2020 202d 205b 4c61 7465  ery:.    - [Late
-00000440: 2064 656c 6976 6572 7920 766f 7563 6865   delivery vouche
-00000450: 7273 5d28 2367 6574 2d6c 6174 652d 6465  rs](#get-late-de
-00000460: 6c69 7665 7279 2d76 6f75 6368 6572 732d  livery-vouchers-
-00000470: 290a 2d20 5072 6f64 7563 7469 6f6e 3a0a  ).- Production:.
-00000480: 2020 2020 2d20 5b53 746f 7020 7361 6c65      - [Stop sale
-00000490: 735d 2823 6765 742d 7374 6f70 2d73 616c  s](#get-stop-sal
-000004a0: 6573 2d29 0a0a 2d2d 2d0a 0a23 2323 2320  es-)..---..#### 
-000004b0: f09f 9bb5 2047 6574 206c 6174 6520 6465  .... Get late de
-000004c0: 6c69 7665 7279 2076 6f75 6368 6572 733a  livery vouchers:
-000004d0: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
-000004e0: 7274 2064 6174 6574 696d 650a 6672 6f6d  rt datetime.from
-000004f0: 2075 7569 6420 696d 706f 7274 2055 5549   uuid import UUI
-00000500: 440a 0a66 726f 6d20 646f 646f 5f69 735f  D..from dodo_is_
-00000510: 6170 692e 636f 6e6e 6563 7469 6f6e 2069  api.connection i
-00000520: 6d70 6f72 7420 446f 646f 4953 4150 4943  mport DodoISAPIC
-00000530: 6f6e 6e65 6374 696f 6e0a 6672 6f6d 2064  onnection.from d
-00000540: 6f64 6f5f 6973 5f61 7069 2e63 6f6e 6e65  odo_is_api.conne
-00000550: 6374 696f 6e2e 6874 7470 5f63 6c69 656e  ction.http_clien
-00000560: 7473 2069 6d70 6f72 7420 636c 6f73 696e  ts import closin
-00000570: 675f 6874 7470 5f63 6c69 656e 740a 6672  g_http_client.fr
-00000580: 6f6d 2064 6f64 6f5f 6973 5f61 7069 2e6d  om dodo_is_api.m
-00000590: 6170 7065 7273 2069 6d70 6f72 7420 6d61  appers import ma
-000005a0: 705f 6c61 7465 5f64 656c 6976 6572 795f  p_late_delivery_
-000005b0: 766f 7563 6865 725f 6474 6f0a 0a61 6363  voucher_dto..acc
-000005c0: 6573 735f 746f 6b65 6e20 3d20 276d 792d  ess_token = 'my-
-000005d0: 746f 6b65 6e27 0a63 6f75 6e74 7279 5f63  token'.country_c
-000005e0: 6f64 6520 3d20 276b 6727 0a0a 756e 6974  ode = 'kg'..unit
-000005f0: 7320 3d20 5b55 5549 4428 2765 3063 6530  s = [UUID('e0ce0
-00000600: 3432 332d 3330 3634 2d34 6530 342d 6164  423-3064-4e04-ad
-00000610: 3365 2d33 3939 3036 3634 3365 6631 3427  3e-39906643ef14'
-00000620: 292c 2055 5549 4428 2762 6430 3962 3061  ), UUID('bd09b0a
-00000630: 382d 3134 3764 2d34 3666 372d 3839 3038  8-147d-46f7-8908
-00000640: 2d38 3734 6635 6635 3963 3961 3227 295d  -874f5f59c9a2')]
-00000650: 0a66 726f 6d5f 6461 7465 203d 2064 6174  .from_date = dat
-00000660: 6574 696d 652e 6461 7465 7469 6d65 2879  etime.datetime(y
-00000670: 6561 723d 3230 3233 2c20 6d6f 6e74 683d  ear=2023, month=
-00000680: 332c 2064 6179 3d31 3629 0a74 6f5f 6461  3, day=16).to_da
-00000690: 7465 203d 2064 6174 6574 696d 652e 6461  te = datetime.da
-000006a0: 7465 7469 6d65 2879 6561 723d 3230 3233  tetime(year=2023
-000006b0: 2c20 6d6f 6e74 683d 332c 2064 6179 3d31  , month=3, day=1
-000006c0: 3729 0a0a 7769 7468 2063 6c6f 7369 6e67  7)..with closing
-000006d0: 5f68 7474 705f 636c 6965 6e74 2861 6363  _http_client(acc
-000006e0: 6573 735f 746f 6b65 6e3d 6163 6365 7373  ess_token=access
-000006f0: 5f74 6f6b 656e 2c20 636f 756e 7472 795f  _token, country_
-00000700: 636f 6465 3d63 6f75 6e74 7279 5f63 6f64  code=country_cod
-00000710: 6529 2061 7320 6874 7470 5f63 6c69 656e  e) as http_clien
-00000720: 743a 0a20 2020 2064 6f64 6f5f 6973 5f61  t:.    dodo_is_a
-00000730: 7069 5f63 6f6e 6e65 6374 696f 6e20 3d20  pi_connection = 
-00000740: 446f 646f 4953 4150 4943 6f6e 6e65 6374  DodoISAPIConnect
-00000750: 696f 6e28 6874 7470 5f63 6c69 656e 743d  ion(http_client=
-00000760: 6874 7470 5f63 6c69 656e 7429 0a0a 2020  http_client)..  
-00000770: 2020 2320 6974 2077 696c 6c20 6861 6e64    # it will hand
-00000780: 6c65 2070 6167 696e 6174 696f 6e20 666f  le pagination fo
-00000790: 7220 796f 750a 2020 2020 666f 7220 6c61  r you.    for la
-000007a0: 7465 5f64 656c 6976 6572 795f 766f 7563  te_delivery_vouc
-000007b0: 6865 7273 2069 6e20 646f 646f 5f69 735f  hers in dodo_is_
-000007c0: 6170 695f 636f 6e6e 6563 7469 6f6e 2e69  api_connection.i
-000007d0: 7465 725f 6c61 7465 5f64 656c 6976 6572  ter_late_deliver
-000007e0: 795f 766f 7563 6865 7273 280a 2020 2020  y_vouchers(.    
-000007f0: 2020 2020 2020 2020 6672 6f6d 5f64 6174          from_dat
-00000800: 653d 6672 6f6d 5f64 6174 652c 0a20 2020  e=from_date,.   
-00000810: 2020 2020 2020 2020 2074 6f5f 6461 7465           to_date
-00000820: 3d74 6f5f 6461 7465 2c0a 2020 2020 2020  =to_date,.      
-00000830: 2020 2020 2020 756e 6974 733d 756e 6974        units=unit
-00000840: 730a 2020 2020 293a 0a20 2020 2020 2020  s.    ):.       
-00000850: 2023 206d 6170 2074 6f20 6461 7461 636c   # map to datacl
-00000860: 6173 7320 4454 4f20 6966 2079 6f75 206e  ass DTO if you n
-00000870: 6565 640a 2020 2020 2020 2020 6c61 7465  eed.        late
-00000880: 5f64 656c 6976 6572 795f 766f 7563 6865  _delivery_vouche
-00000890: 725f 6474 6f73 203d 205b 0a20 2020 2020  r_dtos = [.     
-000008a0: 2020 2020 2020 206d 6170 5f6c 6174 655f         map_late_
-000008b0: 6465 6c69 7665 7279 5f76 6f75 6368 6572  delivery_voucher
-000008c0: 5f64 746f 286c 6174 655f 6465 6c69 7665  _dto(late_delive
-000008d0: 7279 5f76 6f75 6368 6572 290a 2020 2020  ry_voucher).    
-000008e0: 2020 2020 2020 2020 666f 7220 6c61 7465          for late
-000008f0: 5f64 656c 6976 6572 795f 766f 7563 6865  _delivery_vouche
-00000900: 7220 696e 206c 6174 655f 6465 6c69 7665  r in late_delive
-00000910: 7279 5f76 6f75 6368 6572 730a 2020 2020  ry_vouchers.    
-00000920: 2020 2020 5d0a 2020 2020 2020 2020 2e2e      ].        ..
-00000930: 2e0a 6060 600a 0a2d 2d2d 0a0a 2323 2323  ..```..---..####
-00000940: 20f0 9f93 a620 4765 7420 7374 6f70 2073   .... Get stop s
-00000950: 616c 6573 3a0a 0a60 6060 7079 7468 6f6e  ales:..```python
-00000960: 0a69 6d70 6f72 7420 6461 7465 7469 6d65  .import datetime
-00000970: 0a66 726f 6d20 7575 6964 2069 6d70 6f72  .from uuid impor
-00000980: 7420 5555 4944 0a0a 6672 6f6d 2064 6f64  t UUID..from dod
-00000990: 6f5f 6973 5f61 7069 2e63 6f6e 6e65 6374  o_is_api.connect
-000009a0: 696f 6e20 696d 706f 7274 2044 6f64 6f49  ion import DodoI
-000009b0: 5341 5049 436f 6e6e 6563 7469 6f6e 0a66  SAPIConnection.f
-000009c0: 726f 6d20 646f 646f 5f69 735f 6170 692e  rom dodo_is_api.
-000009d0: 636f 6e6e 6563 7469 6f6e 2e68 7474 705f  connection.http_
-000009e0: 636c 6965 6e74 7320 696d 706f 7274 2063  clients import c
-000009f0: 6c6f 7369 6e67 5f68 7474 705f 636c 6965  losing_http_clie
-00000a00: 6e74 0a66 726f 6d20 646f 646f 5f69 735f  nt.from dodo_is_
-00000a10: 6170 692e 6d61 7070 6572 7320 696d 706f  api.mappers impo
-00000a20: 7274 206d 6170 5f73 746f 705f 7361 6c65  rt map_stop_sale
-00000a30: 5f62 795f 696e 6772 6564 6965 6e74 5f64  _by_ingredient_d
-00000a40: 746f 0a0a 6163 6365 7373 5f74 6f6b 656e  to..access_token
-00000a50: 203d 2027 6d79 2d74 6f6b 656e 270a 636f   = 'my-token'.co
-00000a60: 756e 7472 795f 636f 6465 203d 2027 6b67  untry_code = 'kg
-00000a70: 270a 0a75 6e69 7473 203d 205b 5555 4944  '..units = [UUID
-00000a80: 2827 6530 6365 3034 3233 2d33 3036 342d  ('e0ce0423-3064-
-00000a90: 3465 3034 2d61 6433 652d 3339 3930 3636  4e04-ad3e-399066
-00000aa0: 3433 6566 3134 2729 2c20 5555 4944 2827  43ef14'), UUID('
-00000ab0: 6264 3039 6230 6138 2d31 3437 642d 3436  bd09b0a8-147d-46
-00000ac0: 6637 2d38 3930 382d 3837 3466 3566 3539  f7-8908-874f5f59
-00000ad0: 6339 6132 2729 5d0a 6672 6f6d 5f64 6174  c9a2')].from_dat
-00000ae0: 6520 3d20 6461 7465 7469 6d65 2e64 6174  e = datetime.dat
-00000af0: 6574 696d 6528 7965 6172 3d32 3032 332c  etime(year=2023,
-00000b00: 206d 6f6e 7468 3d33 2c20 6461 793d 3136   month=3, day=16
-00000b10: 290a 746f 5f64 6174 6520 3d20 6461 7465  ).to_date = date
-00000b20: 7469 6d65 2e64 6174 6574 696d 6528 7965  time.datetime(ye
-00000b30: 6172 3d32 3032 332c 206d 6f6e 7468 3d33  ar=2023, month=3
-00000b40: 2c20 6461 793d 3137 290a 0a77 6974 6820  , day=17)..with 
-00000b50: 636c 6f73 696e 675f 6874 7470 5f63 6c69  closing_http_cli
-00000b60: 656e 7428 6163 6365 7373 5f74 6f6b 656e  ent(access_token
-00000b70: 3d61 6363 6573 735f 746f 6b65 6e2c 2063  =access_token, c
-00000b80: 6f75 6e74 7279 5f63 6f64 653d 636f 756e  ountry_code=coun
-00000b90: 7472 795f 636f 6465 2920 6173 2068 7474  try_code) as htt
-00000ba0: 705f 636c 6965 6e74 3a0a 2020 2020 646f  p_client:.    do
-00000bb0: 646f 5f69 735f 6170 695f 636f 6e6e 6563  do_is_api_connec
-00000bc0: 7469 6f6e 203d 2044 6f64 6f49 5341 5049  tion = DodoISAPI
-00000bd0: 436f 6e6e 6563 7469 6f6e 2868 7474 705f  Connection(http_
-00000be0: 636c 6965 6e74 3d68 7474 705f 636c 6965  client=http_clie
-00000bf0: 6e74 290a 0a20 2020 2023 2066 6f72 2070  nt)..    # for p
-00000c00: 726f 6475 6374 7320 2d20 646f 646f 5f69  roducts - dodo_i
-00000c10: 735f 6170 695f 636f 6e6e 6563 7469 6f6e  s_api_connection
-00000c20: 2e67 6574 5f73 746f 705f 7361 6c65 735f  .get_stop_sales_
-00000c30: 6279 5f70 726f 6475 6374 730a 2020 2020  by_products.    
-00000c40: 2320 666f 7220 7361 6c65 7320 6368 616e  # for sales chan
-00000c50: 6e65 6c73 202d 2064 6f64 6f5f 6973 5f61  nels - dodo_is_a
-00000c60: 7069 5f63 6f6e 6e65 6374 696f 6e2e 6765  pi_connection.ge
-00000c70: 745f 7374 6f70 5f73 616c 6573 5f62 795f  t_stop_sales_by_
-00000c80: 7361 6c65 735f 6368 616e 6e65 6c73 0a20  sales_channels. 
-00000c90: 2020 2073 746f 705f 7361 6c65 7320 3d20     stop_sales = 
-00000ca0: 646f 646f 5f69 735f 6170 695f 636f 6e6e  dodo_is_api_conn
-00000cb0: 6563 7469 6f6e 2e67 6574 5f73 746f 705f  ection.get_stop_
-00000cc0: 7361 6c65 735f 6279 5f69 6e67 7265 6469  sales_by_ingredi
-00000cd0: 656e 7473 280a 2020 2020 2020 2020 6672  ents(.        fr
-00000ce0: 6f6d 5f64 6174 653d 6672 6f6d 5f64 6174  om_date=from_dat
-00000cf0: 652c 0a20 2020 2020 2020 2074 6f5f 6461  e,.        to_da
-00000d00: 7465 3d74 6f5f 6461 7465 2c0a 2020 2020  te=to_date,.    
-00000d10: 2020 2020 756e 6974 733d 756e 6974 730a      units=units.
-00000d20: 2020 2020 290a 0a20 2020 2023 206d 6170      )..    # map
-00000d30: 2074 6f20 6461 7461 636c 6173 7320 4454   to dataclass DT
-00000d40: 4f20 6966 2079 6f75 206e 6565 640a 2020  O if you need.  
-00000d50: 2020 2320 7573 6520 7375 6974 6162 6c65    # use suitable
-00000d60: 206d 6170 7065 720a 2020 2020 2320 696e   mapper.    # in
-00000d70: 2074 6869 7320 6361 7365 2c20 696e 6772   this case, ingr
-00000d80: 6564 6965 6e74 2073 746f 7020 7361 6c65  edient stop sale
-00000d90: 206d 6170 7065 7220 6973 2075 7365 640a   mapper is used.
-00000da0: 2020 2020 6c61 7465 5f64 656c 6976 6572      late_deliver
-00000db0: 795f 766f 7563 6865 725f 6474 6f73 203d  y_voucher_dtos =
-00000dc0: 205b 0a20 2020 2020 2020 206d 6170 5f73   [.        map_s
-00000dd0: 746f 705f 7361 6c65 5f62 795f 696e 6772  top_sale_by_ingr
-00000de0: 6564 6965 6e74 5f64 746f 2873 746f 705f  edient_dto(stop_
-00000df0: 7361 6c65 290a 2020 2020 2020 2020 666f  sale).        fo
-00000e00: 7220 7374 6f70 5f73 616c 6520 696e 2073  r stop_sale in s
-00000e10: 746f 705f 7361 6c65 730a 2020 2020 5d0a  top_sales.    ].
-00000e20: 2020 2020 2e2e 2e0a 6060 600a                ....```.
+00000000: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
+00000010: 7222 3e0a f09f 8d95 2044 6f64 6f20 4953  r">..... Dodo IS
+00000020: 2041 5049 2057 7261 7070 6572 0a3c 2f68   API Wrapper.</h
+00000030: 313e 0a0a 3c70 2061 6c69 676e 3d22 6365  1>..<p align="ce
+00000040: 6e74 6572 223e 0a3c 6120 6872 6566 3d22  nter">.<a href="
+00000050: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000060: 6f6d 2f67 6f72 6574 736b 792d 696e 7465  om/goretsky-inte
+00000070: 6772 6174 696f 6e2f 646f 646f 2d69 732d  gration/dodo-is-
+00000080: 6170 692d 7079 7468 6f6e 2d77 7261 7070  api-python-wrapp
+00000090: 6572 2f61 6374 696f 6e73 2f77 6f72 6b66  er/actions/workf
+000000a0: 6c6f 7773 2f75 6e69 7474 6573 742e 7961  lows/unittest.ya
+000000b0: 6d6c 223e 0a3c 696d 6720 7372 633d 2268  ml">.<img src="h
+000000c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000000d0: 6d2f 676f 7265 7473 6b79 2d69 6e74 6567  m/goretsky-integ
+000000e0: 7261 7469 6f6e 2f64 6f64 6f2d 6973 2d61  ration/dodo-is-a
+000000f0: 7069 2d70 7974 686f 6e2d 7772 6170 7065  pi-python-wrappe
+00000100: 722f 6163 7469 6f6e 732f 776f 726b 666c  r/actions/workfl
+00000110: 6f77 732f 756e 6974 7465 7374 2e79 616d  ows/unittest.yam
+00000120: 6c2f 6261 6467 652e 7376 6722 2061 6c74  l/badge.svg" alt
+00000130: 3d22 5465 7374 2062 6164 6765 223e 0a3c  ="Test badge">.<
+00000140: 2f61 3e0a 3c61 2068 7265 663d 2268 7474  /a>.<a href="htt
+00000150: 7073 3a2f 2f63 6f64 6563 6f76 2e69 6f2f  ps://codecov.io/
+00000160: 6768 2f67 6f72 6574 736b 792d 696e 7465  gh/goretsky-inte
+00000170: 6772 6174 696f 6e2f 646f 646f 2d69 732d  gration/dodo-is-
+00000180: 6170 692d 7079 7468 6f6e 2d77 7261 7070  api-python-wrapp
+00000190: 6572 223e 0a3c 696d 6720 7372 633d 2268  er">.<img src="h
+000001a0: 7474 7073 3a2f 2f63 6f64 6563 6f76 2e69  ttps://codecov.i
+000001b0: 6f2f 6768 2f67 6f72 6574 736b 792d 696e  o/gh/goretsky-in
+000001c0: 7465 6772 6174 696f 6e2f 646f 646f 2d69  tegration/dodo-i
+000001d0: 732d 6170 692d 7079 7468 6f6e 2d77 7261  s-api-python-wra
+000001e0: 7070 6572 2f62 7261 6e63 682f 6d61 696e  pper/branch/main
+000001f0: 2f67 7261 7068 2f62 6164 6765 2e73 7667  /graph/badge.svg
+00000200: 3f74 6f6b 656e 3d75 6e7a 6c4d 6d41 6a73  ?token=unzlMmAjs
+00000210: 4422 2f3e 0a3c 2f61 3e0a 3c69 6d67 2073  D"/>.</a>.<img s
+00000220: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000230: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00000240: 2f70 7974 686f 6e2d 332e 3131 2d62 7269  /python-3.11-bri
+00000250: 6768 7467 7265 656e 2220 616c 743d 2270  ghtgreen" alt="p
+00000260: 7974 686f 6e22 3e0a 3c2f 703e 0a0a 2d2d  ython">.</p>..--
+00000270: 2d0a 0a23 2323 2049 6e73 7461 6c6c 6174  -..### Installat
+00000280: 696f 6e0a 0a56 6961 2070 6970 3a0a 0a60  ion..Via pip:..`
+00000290: 6060 7368 656c 6c0a 7069 7020 696e 7374  ``shell.pip inst
+000002a0: 616c 6c20 646f 646f 2d69 732d 6170 690a  all dodo-is-api.
+000002b0: 6060 600a 0a56 6961 2070 6f65 7472 793a  ```..Via poetry:
+000002c0: 0a0a 6060 6073 6865 6c6c 0a70 6f65 7472  ..```shell.poetr
+000002d0: 7920 6164 6420 646f 646f 2d69 732d 6170  y add dodo-is-ap
+000002e0: 690a 6060 600a 0a2d 2d2d 0a0a 2323 2323  i.```..---..####
+000002f0: 20f0 9f93 9d20 5b43 6861 6e67 656c 6f67   .... [Changelog
+00000300: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000310: 2e63 6f6d 2f67 6f72 6574 736b 792d 696e  .com/goretsky-in
+00000320: 7465 6772 6174 696f 6e2f 646f 646f 2d69  tegration/dodo-i
+00000330: 732d 6170 692d 7079 7468 6f6e 2d77 7261  s-api-python-wra
+00000340: 7070 6572 2f62 6c6f 622f 6d61 696e 2f43  pper/blob/main/C
+00000350: 4841 4e47 454c 4f47 2e6d 6429 2069 7320  HANGELOG.md) is 
+00000360: 6865 7265 2e0a 0a2d 2d2d 0a0a 2323 2320  here...---..### 
+00000370: f09f a7aa 2055 7361 6765 3a0a 0af0 9f8c  .... Usage:.....
+00000380: a9ef b88f 2053 796e 6368 726f 6e6f 7573  .... Synchronous
+00000390: 2076 6572 7369 6f6e 3a0a 0a60 6060 7079   version:..```py
+000003a0: 7468 6f6e 0a66 726f 6d20 6461 7465 7469  thon.from dateti
+000003b0: 6d65 2069 6d70 6f72 7420 6461 7465 7469  me import dateti
+000003c0: 6d65 0a66 726f 6d20 7575 6964 2069 6d70  me.from uuid imp
+000003d0: 6f72 7420 5555 4944 0a0a 696d 706f 7274  ort UUID..import
+000003e0: 2068 7474 7078 0a0a 6672 6f6d 2064 6f64   httpx..from dod
+000003f0: 6f5f 6973 5f61 7069 2069 6d70 6f72 7420  o_is_api import 
+00000400: 6d6f 6465 6c73 0a66 726f 6d20 646f 646f  models.from dodo
+00000410: 5f69 735f 6170 692e 636f 6e6e 6563 7469  _is_api.connecti
+00000420: 6f6e 2e73 796e 6368 726f 6e6f 7573 2069  on.synchronous i
+00000430: 6d70 6f72 7420 446f 646f 4953 4150 4943  mport DodoISAPIC
+00000440: 6f6e 6e65 6374 696f 6e0a 0a0a 6465 6620  onnection...def 
+00000450: 6d61 696e 2829 3a0a 2020 2020 6163 6365  main():.    acce
+00000460: 7373 5f74 6f6b 656e 203d 2027 796f 7572  ss_token = 'your
+00000470: 2061 6363 6573 7320 746f 6b65 6e27 0a20   access token'. 
+00000480: 2020 2063 6f75 6e74 7279 5f63 6f64 6520     country_code 
+00000490: 3d20 6d6f 6465 6c73 2e43 6f75 6e74 7279  = models.Country
+000004a0: 436f 6465 2e52 550a 0a20 2020 2066 726f  Code.RU..    fro
+000004b0: 6d5f 6461 7465 203d 2064 6174 6574 696d  m_date = datetim
+000004c0: 6528 3230 3034 2c20 3130 2c20 3729 0a20  e(2004, 10, 7). 
+000004d0: 2020 2074 6f5f 6461 7465 203d 2064 6174     to_date = dat
+000004e0: 6574 696d 6528 3230 3034 2c20 3130 2c20  etime(2004, 10, 
+000004f0: 372c 2032 3329 0a20 2020 2075 6e69 7473  7, 23).    units
+00000500: 203d 205b 5555 4944 2827 6563 3831 3833   = [UUID('ec8183
+00000510: 3163 2d62 3861 372d 3462 6138 2d61 3661  1c-b8a7-4ba8-a6a
+00000520: 612d 3761 6537 6430 6334 6530 6262 2729  a-7ae7d0c4e0bb')
+00000530: 5d0a 0a20 2020 2077 6974 6820 6874 7470  ]..    with http
+00000540: 782e 436c 6965 6e74 2829 2061 7320 6874  x.Client() as ht
+00000550: 7470 5f63 6c69 656e 743a 0a20 2020 2020  tp_client:.     
+00000560: 2020 2063 6f6e 6e65 6374 696f 6e20 3d20     connection = 
+00000570: 446f 646f 4953 4150 4943 6f6e 6e65 6374  DodoISAPIConnect
+00000580: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+00000590: 2068 7474 705f 636c 6965 6e74 3d68 7474   http_client=htt
+000005a0: 705f 636c 6965 6e74 2c0a 2020 2020 2020  p_client,.      
+000005b0: 2020 2020 2020 6163 6365 7373 5f74 6f6b        access_tok
+000005c0: 656e 3d61 6363 6573 735f 746f 6b65 6e2c  en=access_token,
+000005d0: 0a20 2020 2020 2020 2020 2020 2063 6f75  .            cou
+000005e0: 6e74 7279 5f63 6f64 653d 636f 756e 7472  ntry_code=countr
+000005f0: 795f 636f 6465 2c0a 2020 2020 2020 2020  y_code,.        
+00000600: 290a 0a20 2020 2020 2020 2073 746f 705f  )..        stop_
+00000610: 7361 6c65 7320 3d20 636f 6e6e 6563 7469  sales = connecti
+00000620: 6f6e 2e67 6574 5f73 746f 705f 7361 6c65  on.get_stop_sale
+00000630: 735f 6279 5f70 726f 6475 6374 7328 0a20  s_by_products(. 
+00000640: 2020 2020 2020 2020 2020 2066 726f 6d5f             from_
+00000650: 6461 7465 3d66 726f 6d5f 6461 7465 2c0a  date=from_date,.
+00000660: 2020 2020 2020 2020 2020 2020 746f 5f64              to_d
+00000670: 6174 653d 746f 5f64 6174 652c 0a20 2020  ate=to_date,.   
+00000680: 2020 2020 2020 2020 2075 6e69 7473 3d75           units=u
+00000690: 6e69 7473 2c0a 2020 2020 2020 2020 290a  nits,.        ).
+000006a0: 0a20 2020 2070 7269 6e74 2873 746f 705f  .    print(stop_
+000006b0: 7361 6c65 7329 0a0a 0a69 6620 5f5f 6e61  sales)...if __na
+000006c0: 6d65 5f5f 203d 3d20 275f 5f6d 6169 6e5f  me__ == '__main_
+000006d0: 5f27 3a0a 2020 2020 6d61 696e 2829 0a60  _':.    main().`
+000006e0: 6060 0a0a e29a a1ef b88f 2041 7379 6e63  ``........ Async
+000006f0: 6872 6f6e 6f75 7320 7665 7273 696f 6e3a  hronous version:
+00000700: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+00000710: 7274 2061 7379 6e63 696f 0a66 726f 6d20  rt asyncio.from 
+00000720: 6461 7465 7469 6d65 2069 6d70 6f72 7420  datetime import 
+00000730: 6461 7465 7469 6d65 0a66 726f 6d20 7575  datetime.from uu
+00000740: 6964 2069 6d70 6f72 7420 5555 4944 0a0a  id import UUID..
+00000750: 696d 706f 7274 2068 7474 7078 0a0a 6672  import httpx..fr
+00000760: 6f6d 2064 6f64 6f5f 6973 5f61 7069 2069  om dodo_is_api i
+00000770: 6d70 6f72 7420 6d6f 6465 6c73 0a66 726f  mport models.fro
+00000780: 6d20 646f 646f 5f69 735f 6170 692e 636f  m dodo_is_api.co
+00000790: 6e6e 6563 7469 6f6e 2e61 7379 6e63 6872  nnection.asynchr
+000007a0: 6f6e 6f75 7320 696d 706f 7274 2041 7379  onous import Asy
+000007b0: 6e63 446f 646f 4953 4150 4943 6f6e 6e65  ncDodoISAPIConne
+000007c0: 6374 696f 6e0a 0a0a 6173 796e 6320 6465  ction...async de
+000007d0: 6620 6d61 696e 2829 3a0a 2020 2020 6163  f main():.    ac
+000007e0: 6365 7373 5f74 6f6b 656e 203d 2027 796f  cess_token = 'yo
+000007f0: 7572 2061 6363 6573 7320 746f 6b65 6e27  ur access token'
+00000800: 0a20 2020 2063 6f75 6e74 7279 5f63 6f64  .    country_cod
+00000810: 6520 3d20 6d6f 6465 6c73 2e43 6f75 6e74  e = models.Count
+00000820: 7279 436f 6465 2e52 550a 0a20 2020 2066  ryCode.RU..    f
+00000830: 726f 6d5f 6461 7465 203d 2064 6174 6574  rom_date = datet
+00000840: 696d 6528 3230 3034 2c20 3130 2c20 3729  ime(2004, 10, 7)
+00000850: 0a20 2020 2074 6f5f 6461 7465 203d 2064  .    to_date = d
+00000860: 6174 6574 696d 6528 3230 3034 2c20 3130  atetime(2004, 10
+00000870: 2c20 372c 2032 3329 0a20 2020 2075 6e69  , 7, 23).    uni
+00000880: 7473 203d 205b 5555 4944 2827 6563 3831  ts = [UUID('ec81
+00000890: 3833 3163 2d62 3861 372d 3462 6138 2d61  831c-b8a7-4ba8-a
+000008a0: 3661 612d 3761 6537 6430 6334 6530 6262  6aa-7ae7d0c4e0bb
+000008b0: 2729 5d0a 0a20 2020 2077 6974 6820 6874  ')]..    with ht
+000008c0: 7470 782e 4173 796e 6343 6c69 656e 7428  tpx.AsyncClient(
+000008d0: 2920 6173 2068 7474 705f 636c 6965 6e74  ) as http_client
+000008e0: 3a0a 2020 2020 2020 2020 636f 6e6e 6563  :.        connec
+000008f0: 7469 6f6e 203d 2041 7379 6e63 446f 646f  tion = AsyncDodo
+00000900: 4953 4150 4943 6f6e 6e65 6374 696f 6e28  ISAPIConnection(
+00000910: 0a20 2020 2020 2020 2020 2020 2068 7474  .            htt
+00000920: 705f 636c 6965 6e74 3d68 7474 705f 636c  p_client=http_cl
+00000930: 6965 6e74 2c0a 2020 2020 2020 2020 2020  ient,.          
+00000940: 2020 6163 6365 7373 5f74 6f6b 656e 3d61    access_token=a
+00000950: 6363 6573 735f 746f 6b65 6e2c 0a20 2020  ccess_token,.   
+00000960: 2020 2020 2020 2020 2063 6f75 6e74 7279           country
+00000970: 5f63 6f64 653d 636f 756e 7472 795f 636f  _code=country_co
+00000980: 6465 2c0a 2020 2020 2020 2020 290a 0a20  de,.        ).. 
+00000990: 2020 2020 2020 2073 746f 705f 7361 6c65         stop_sale
+000009a0: 7320 3d20 6177 6169 7420 636f 6e6e 6563  s = await connec
+000009b0: 7469 6f6e 2e67 6574 5f73 746f 705f 7361  tion.get_stop_sa
+000009c0: 6c65 735f 6279 5f70 726f 6475 6374 7328  les_by_products(
+000009d0: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
+000009e0: 6d5f 6461 7465 3d66 726f 6d5f 6461 7465  m_date=from_date
+000009f0: 2c0a 2020 2020 2020 2020 2020 2020 746f  ,.            to
+00000a00: 5f64 6174 653d 746f 5f64 6174 652c 0a20  _date=to_date,. 
+00000a10: 2020 2020 2020 2020 2020 2075 6e69 7473             units
+00000a20: 3d75 6e69 7473 2c0a 2020 2020 2020 2020  =units,.        
+00000a30: 290a 0a20 2020 2070 7269 6e74 2873 746f  )..    print(sto
+00000a40: 705f 7361 6c65 7329 0a0a 0a69 6620 5f5f  p_sales)...if __
+00000a50: 6e61 6d65 5f5f 203d 3d20 275f 5f6d 6169  name__ == '__mai
+00000a60: 6e5f 5f27 3a0a 2020 2020 6173 796e 6369  n__':.    asynci
+00000a70: 6f2e 7275 6e28 6d61 696e 2829 290a 6060  o.run(main()).``
+00000a80: 60                                       `
```

### Comparing `dodo_is_api-0.6.1/dodo_is_api/logger.py` & `dodo_is_api-0.7.0/dodo_is_api/logger.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.6.1/pyproject.toml` & `dodo_is_api-0.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "dodo-is-api"
-version = "0.6.1"
+version = "0.7.0"
 description = ""
 authors = ["Eldos <eldos.baktybekov@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dodo_is_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 httpx = "^0.23.3"
 structlog = "^23.1.0"
+pydantic = "^1.10.9"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-asyncio = "^0.20.3"
 pytest-httpx = "^0.21.3"
```

### Comparing `dodo_is_api-0.6.1/setup.py` & `dodo_is_api-0.7.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 packages = \
 ['dodo_is_api', 'dodo_is_api.connection', 'dodo_is_api.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['httpx>=0.23.3,<0.24.0', 'structlog>=23.1.0,<24.0.0']
+['httpx>=0.23.3,<0.24.0',
+ 'pydantic>=1.10.9,<2.0.0',
+ 'structlog>=23.1.0,<24.0.0']
 
 setup_kwargs = {
     'name': 'dodo-is-api',
-    'version': '0.6.1',
+    'version': '0.7.0',
     'description': '',
-    'long_description': '<div align="center">\n<a href="https://dodo-brands.stoplight.io">\n<img width="350px" src="https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg">\n</a>\n</div>\n    \n<h1 align="center">\n🍕 Dodo IS API Wrapper\n</h1>\n\n<p align="center">\n<a href="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml">\n<img src="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml/badge.svg" alt="Test badge">\n</a>\n<a href="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper">\n<img src="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD"/>\n</a>\n<img src="https://img.shields.io/badge/python-3.11-brightgreen" alt="python">\n</p>\n\n---\n\n### Installation\n\nVia pip:\n```shell\npip install dodo-is-api\n```\n\nVia poetry:\n```shell\npoetry add dodo-is-api\n```\n\n---\n\n#### 📝 [Changelog](https://github.com/goretsky-integration/dodo-is-api-python-wrapper/blob/main/CHANGELOG.md) is here.\n\n---\n\n### 🧪 Usage:\n\n- Delivery:\n    - [Late delivery vouchers](#get-late-delivery-vouchers-)\n- Production:\n    - [Stop sales](#get-stop-sales-)\n\n---\n\n#### 🛵 Get late delivery vouchers:\n\n```python\nimport datetime\nfrom uuid import UUID\n\nfrom dodo_is_api.connection import DodoISAPIConnection\nfrom dodo_is_api.connection.http_clients import closing_http_client\nfrom dodo_is_api.mappers import map_late_delivery_voucher_dto\n\naccess_token = \'my-token\'\ncountry_code = \'kg\'\n\nunits = [UUID(\'e0ce0423-3064-4e04-ad3e-39906643ef14\'), UUID(\'bd09b0a8-147d-46f7-8908-874f5f59c9a2\')]\nfrom_date = datetime.datetime(year=2023, month=3, day=16)\nto_date = datetime.datetime(year=2023, month=3, day=17)\n\nwith closing_http_client(access_token=access_token, country_code=country_code) as http_client:\n    dodo_is_api_connection = DodoISAPIConnection(http_client=http_client)\n\n    # it will handle pagination for you\n    for late_delivery_vouchers in dodo_is_api_connection.iter_late_delivery_vouchers(\n            from_date=from_date,\n            to_date=to_date,\n            units=units\n    ):\n        # map to dataclass DTO if you need\n        late_delivery_voucher_dtos = [\n            map_late_delivery_voucher_dto(late_delivery_voucher)\n            for late_delivery_voucher in late_delivery_vouchers\n        ]\n        ...\n```\n\n---\n\n#### 📦 Get stop sales:\n\n```python\nimport datetime\nfrom uuid import UUID\n\nfrom dodo_is_api.connection import DodoISAPIConnection\nfrom dodo_is_api.connection.http_clients import closing_http_client\nfrom dodo_is_api.mappers import map_stop_sale_by_ingredient_dto\n\naccess_token = \'my-token\'\ncountry_code = \'kg\'\n\nunits = [UUID(\'e0ce0423-3064-4e04-ad3e-39906643ef14\'), UUID(\'bd09b0a8-147d-46f7-8908-874f5f59c9a2\')]\nfrom_date = datetime.datetime(year=2023, month=3, day=16)\nto_date = datetime.datetime(year=2023, month=3, day=17)\n\nwith closing_http_client(access_token=access_token, country_code=country_code) as http_client:\n    dodo_is_api_connection = DodoISAPIConnection(http_client=http_client)\n\n    # for products - dodo_is_api_connection.get_stop_sales_by_products\n    # for sales channels - dodo_is_api_connection.get_stop_sales_by_sales_channels\n    stop_sales = dodo_is_api_connection.get_stop_sales_by_ingredients(\n        from_date=from_date,\n        to_date=to_date,\n        units=units\n    )\n\n    # map to dataclass DTO if you need\n    # use suitable mapper\n    # in this case, ingredient stop sale mapper is used\n    late_delivery_voucher_dtos = [\n        map_stop_sale_by_ingredient_dto(stop_sale)\n        for stop_sale in stop_sales\n    ]\n    ...\n```\n',
+    'long_description': '<h1 align="center">\n🍕 Dodo IS API Wrapper\n</h1>\n\n<p align="center">\n<a href="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml">\n<img src="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml/badge.svg" alt="Test badge">\n</a>\n<a href="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper">\n<img src="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD"/>\n</a>\n<img src="https://img.shields.io/badge/python-3.11-brightgreen" alt="python">\n</p>\n\n---\n\n### Installation\n\nVia pip:\n\n```shell\npip install dodo-is-api\n```\n\nVia poetry:\n\n```shell\npoetry add dodo-is-api\n```\n\n---\n\n#### 📝 [Changelog](https://github.com/goretsky-integration/dodo-is-api-python-wrapper/blob/main/CHANGELOG.md) is here.\n\n---\n\n### 🧪 Usage:\n\n🌩️ Synchronous version:\n\n```python\nfrom datetime import datetime\nfrom uuid import UUID\n\nimport httpx\n\nfrom dodo_is_api import models\nfrom dodo_is_api.connection.synchronous import DodoISAPIConnection\n\n\ndef main():\n    access_token = \'your access token\'\n    country_code = models.CountryCode.RU\n\n    from_date = datetime(2004, 10, 7)\n    to_date = datetime(2004, 10, 7, 23)\n    units = [UUID(\'ec81831c-b8a7-4ba8-a6aa-7ae7d0c4e0bb\')]\n\n    with httpx.Client() as http_client:\n        connection = DodoISAPIConnection(\n            http_client=http_client,\n            access_token=access_token,\n            country_code=country_code,\n        )\n\n        stop_sales = connection.get_stop_sales_by_products(\n            from_date=from_date,\n            to_date=to_date,\n            units=units,\n        )\n\n    print(stop_sales)\n\n\nif __name__ == \'__main__\':\n    main()\n```\n\n⚡️ Asynchronous version:\n\n```python\nimport asyncio\nfrom datetime import datetime\nfrom uuid import UUID\n\nimport httpx\n\nfrom dodo_is_api import models\nfrom dodo_is_api.connection.asynchronous import AsyncDodoISAPIConnection\n\n\nasync def main():\n    access_token = \'your access token\'\n    country_code = models.CountryCode.RU\n\n    from_date = datetime(2004, 10, 7)\n    to_date = datetime(2004, 10, 7, 23)\n    units = [UUID(\'ec81831c-b8a7-4ba8-a6aa-7ae7d0c4e0bb\')]\n\n    with httpx.AsyncClient() as http_client:\n        connection = AsyncDodoISAPIConnection(\n            http_client=http_client,\n            access_token=access_token,\n            country_code=country_code,\n        )\n\n        stop_sales = await connection.get_stop_sales_by_products(\n            from_date=from_date,\n            to_date=to_date,\n            units=units,\n        )\n\n    print(stop_sales)\n\n\nif __name__ == \'__main__\':\n    asyncio.run(main())\n```',
     'author': 'Eldos',
     'author_email': 'eldos.baktybekov@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,54 +1,42 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['dodo_is_api', 'dodo_is_api.connection', 'dodo_is_api.models'] package_data =
 \ {'': ['*']} install_requires = \ ['httpx>=0.23.3,<0.24.0',
-'structlog>=23.1.0,<24.0.0'] setup_kwargs = { 'name': 'dodo-is-api', 'version':
-'0.6.1', 'description': '', 'long_description': '
-  \n\n[https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg]\n\n
-\n \n
+'pydantic>=1.10.9,<2.0.0', 'structlog>=23.1.0,<24.0.0'] setup_kwargs =
+{ 'name': 'dodo-is-api', 'version': '0.7.0', 'description': '',
+'long_description': '
                   ****** \nð Dodo IS API Wrapper\n ******
 \n\n
 \n\n[Test_badge]\n\n\n[https://codecov.io/gh/goretsky-integration/dodo-is-api-
   python-wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD]\n\n[python]\n
-\n\n---\n\n### Installation\n\nVia pip:\n```shell\npip install dodo-is-
-api\n```\n\nVia poetry:\n```shell\npoetry add dodo-is-api\n```\n\n---\n\n####
+\n\n---\n\n### Installation\n\nVia pip:\n\n```shell\npip install dodo-is-
+api\n```\n\nVia poetry:\n\n```shell\npoetry add dodo-is-api\n```\n\n---\n\n####
 ð [Changelog](https://github.com/goretsky-integration/dodo-is-api-python-
-wrapper/blob/main/CHANGELOG.md) is here.\n\n---\n\n### ð§ª Usage:\n\n-
-Delivery:\n - [Late delivery vouchers](#get-late-delivery-vouchers-)\n-
-Production:\n - [Stop sales](#get-stop-sales-)\n\n---\n\n#### ðµ Get late
-delivery vouchers:\n\n```python\nimport datetime\nfrom uuid import UUID\n\nfrom
-dodo_is_api.connection import DodoISAPIConnection\nfrom
-dodo_is_api.connection.http_clients import closing_http_client\nfrom
-dodo_is_api.mappers import map_late_delivery_voucher_dto\n\naccess_token =
-\'my-token\'\ncountry_code = \'kg\'\n\nunits = [UUID(\'e0ce0423-3064-4e04-ad3e-
-39906643ef14\'), UUID(\'bd09b0a8-147d-46f7-8908-874f5f59c9a2\')]\nfrom_date =
-datetime.datetime(year=2023, month=3, day=16)\nto_date = datetime.datetime
-(year=2023, month=3, day=17)\n\nwith closing_http_client
-(access_token=access_token, country_code=country_code) as http_client:\n
-dodo_is_api_connection = DodoISAPIConnection(http_client=http_client)\n\n # it
-will handle pagination for you\n for late_delivery_vouchers in
-dodo_is_api_connection.iter_late_delivery_vouchers(\n from_date=from_date,\n
-to_date=to_date,\n units=units\n ):\n # map to dataclass DTO if you need\n
-late_delivery_voucher_dtos = [\n map_late_delivery_voucher_dto
-(late_delivery_voucher)\n for late_delivery_voucher in late_delivery_vouchers\n
-]\n ...\n```\n\n---\n\n#### ð¦ Get stop sales:\n\n```python\nimport
-datetime\nfrom uuid import UUID\n\nfrom dodo_is_api.connection import
-DodoISAPIConnection\nfrom dodo_is_api.connection.http_clients import
-closing_http_client\nfrom dodo_is_api.mappers import
-map_stop_sale_by_ingredient_dto\n\naccess_token = \'my-token\'\ncountry_code =
-\'kg\'\n\nunits = [UUID(\'e0ce0423-3064-4e04-ad3e-39906643ef14\'), UUID
-(\'bd09b0a8-147d-46f7-8908-874f5f59c9a2\')]\nfrom_date = datetime.datetime
-(year=2023, month=3, day=16)\nto_date = datetime.datetime(year=2023, month=3,
-day=17)\n\nwith closing_http_client(access_token=access_token,
-country_code=country_code) as http_client:\n dodo_is_api_connection =
-DodoISAPIConnection(http_client=http_client)\n\n # for products -
-dodo_is_api_connection.get_stop_sales_by_products\n # for sales channels -
-dodo_is_api_connection.get_stop_sales_by_sales_channels\n stop_sales =
-dodo_is_api_connection.get_stop_sales_by_ingredients(\n from_date=from_date,\n
-to_date=to_date,\n units=units\n )\n\n # map to dataclass DTO if you need\n #
-use suitable mapper\n # in this case, ingredient stop sale mapper is used\n
-late_delivery_voucher_dtos = [\n map_stop_sale_by_ingredient_dto(stop_sale)\n
-for stop_sale in stop_sales\n ]\n ...\n```\n', 'author': 'Eldos',
-'author_email': 'eldos.baktybekov@gmail.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'None', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.11,<4.0', } setup(**setup_kwargs)
+wrapper/blob/main/CHANGELOG.md) is here.\n\n---\n\n### ð§ª Usage:\n\nð©ï¸
+Synchronous version:\n\n```python\nfrom datetime import datetime\nfrom uuid
+import UUID\n\nimport httpx\n\nfrom dodo_is_api import models\nfrom
+dodo_is_api.connection.synchronous import DodoISAPIConnection\n\n\ndef main():
+\n access_token = \'your access token\'\n country_code =
+models.CountryCode.RU\n\n from_date = datetime(2004, 10, 7)\n to_date =
+datetime(2004, 10, 7, 23)\n units = [UUID(\'ec81831c-b8a7-4ba8-a6aa-
+7ae7d0c4e0bb\')]\n\n with httpx.Client() as http_client:\n connection =
+DodoISAPIConnection(\n http_client=http_client,\n access_token=access_token,\n
+country_code=country_code,\n )\n\n stop_sales =
+connection.get_stop_sales_by_products(\n from_date=from_date,\n
+to_date=to_date,\n units=units,\n )\n\n print(stop_sales)\n\n\nif __name__ ==
+\'__main__\':\n main()\n```\n\nâ¡ï¸ Asynchronous version:
+\n\n```python\nimport asyncio\nfrom datetime import datetime\nfrom uuid import
+UUID\n\nimport httpx\n\nfrom dodo_is_api import models\nfrom
+dodo_is_api.connection.asynchronous import AsyncDodoISAPIConnection\n\n\nasync
+def main():\n access_token = \'your access token\'\n country_code =
+models.CountryCode.RU\n\n from_date = datetime(2004, 10, 7)\n to_date =
+datetime(2004, 10, 7, 23)\n units = [UUID(\'ec81831c-b8a7-4ba8-a6aa-
+7ae7d0c4e0bb\')]\n\n with httpx.AsyncClient() as http_client:\n connection =
+AsyncDodoISAPIConnection(\n http_client=http_client,\n
+access_token=access_token,\n country_code=country_code,\n )\n\n stop_sales =
+await connection.get_stop_sales_by_products(\n from_date=from_date,\n
+to_date=to_date,\n units=units,\n )\n\n print(stop_sales)\n\n\nif __name__ ==
+\'__main__\':\n asyncio.run(main())\n```', 'author': 'Eldos', 'author_email':
+'eldos.baktybekov@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None',
+'url': 'None', 'packages': packages, 'package_data': package_data,
+'install_requires': install_requires, 'python_requires': '>=3.11,<4.0', } setup
+(**setup_kwargs)
```

