# Comparing `tmp/revolution-eda-0.5.1.tar.gz` & `tmp/revolution-eda-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revolution-eda-0.5.1.tar", last modified: Wed May 31 12:57:50 2023, max compression
+gzip compressed data, was "revolution-eda-0.5.2.tar", last modified: Sun Jun 11 09:39:49 2023, max compression
```

## Comparing `revolution-eda-0.5.1.tar` & `revolution-eda-0.5.2.tar`

### file list

```diff
@@ -1,158 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:50.537959 revolution-eda-0.5.1/
--rw-rw-rw-   0        0        0      114 2023-05-23 10:07:51.000000 revolution-eda-0.5.1/.env
--rw-rw-rw-   0        0        0     1087 2023-02-09 16:47:29.000000 revolution-eda-0.5.1/LICENSE.txt
--rw-rw-rw-   0        0        0      139 2023-05-31 12:16:47.000000 revolution-eda-0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2340 2023-05-31 12:57:50.536692 revolution-eda-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1900 2023-05-31 12:53:58.000000 revolution-eda-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.654364 revolution-eda-0.5.1/docs/
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.773021 revolution-eda-0.5.1/docs/assets/
--rw-rw-rw-   0        0        0     8942 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230209_082011.png
--rw-rw-rw-   0        0        0   475487 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230210_113658.png
--rw-rw-rw-   0        0        0    70438 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230210_142342.png
--rw-rw-rw-   0        0        0    63865 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230210_142507.png
--rw-rw-rw-   0        0        0    83180 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230214_204024.png
--rw-rw-rw-   0        0        0    82595 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230214_204324.png
--rw-rw-rw-   0        0        0    45362 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230214_210207.png
--rw-rw-rw-   0        0        0    33070 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230214_211158.png
--rw-rw-rw-   0        0        0    27216 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230214_212122.png
--rw-rw-rw-   0        0        0    26926 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230214_213352.png
--rw-rw-rw-   0        0        0    25662 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230214_213448.png
--rw-rw-rw-   0        0        0    23583 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230214_213534.png
--rw-rw-rw-   0        0        0    19764 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230214_214328.png
--rw-rw-rw-   0        0        0    52005 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230214_214720.png
--rw-rw-rw-   0        0        0    55425 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230214_215123.png
--rw-rw-rw-   0        0        0    33406 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230214_215437.png
--rw-rw-rw-   0        0        0    49907 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230214_215836.png
--rw-rw-rw-   0        0        0   105491 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230214_220729.png
--rw-rw-rw-   0        0        0   160790 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230214_221911.png
--rw-rw-rw-   0        0        0   139162 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230214_225857.png
--rw-rw-rw-   0        0        0    56372 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_104815.png
--rw-rw-rw-   0        0        0    52976 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_113354.png
--rw-rw-rw-   0        0        0    12448 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_113556.png
--rw-rw-rw-   0        0        0    27513 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_113949.png
--rw-rw-rw-   0        0        0    31774 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_114312.png
--rw-rw-rw-   0        0        0    62743 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_114438.png
--rw-rw-rw-   0        0        0    20453 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_152849.png
--rw-rw-rw-   0        0        0    43440 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_153445.png
--rw-rw-rw-   0        0        0    26210 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_153909.png
--rw-rw-rw-   0        0        0    68838 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_154320.png
--rw-rw-rw-   0        0        0    35198 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_154633.png
--rw-rw-rw-   0        0        0    35993 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_154905.png
--rw-rw-rw-   0        0        0    75895 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_155308.png
--rw-rw-rw-   0        0        0    68774 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_163913.png
--rw-rw-rw-   0        0        0    72575 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_164434.png
--rw-rw-rw-   0        0        0    41952 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_172217.png
--rw-rw-rw-   0        0        0    31943 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_172655.png
--rw-rw-rw-   0        0        0    38087 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230215_173829.png
--rw-rw-rw-   0        0        0   262766 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230216_100322.png
--rw-rw-rw-   0        0        0    49810 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230216_101413-1676540084030-7.png
--rw-rw-rw-   0        0        0    49810 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230216_101413.png
--rw-rw-rw-   0        0        0    45971 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230216_103427.png
--rw-rw-rw-   0        0        0    17810 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230216_120741.png
--rw-rw-rw-   0        0        0    22104 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230216_123430.png
--rw-rw-rw-   0        0        0    16465 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230216_123713.png
--rw-rw-rw-   0        0        0    66178 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/Screenshot_20230216_124059.png
--rw-rw-rw-   0        0        0     8675 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/image-20230209082042521.png
--rw-rw-rw-   0        0        0     8675 2023-05-11 16:50:24.000000 revolution-eda-0.5.1/docs/assets/image-20230209082047928.png
--rw-rw-rw-   0        0        0    32212 2023-05-26 11:27:21.000000 revolution-eda-0.5.1/docs/index.md
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.576822 revolution-eda-0.5.1/exampleLibraries/
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.776099 revolution-eda-0.5.1/exampleLibraries/analogLib/
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.786222 revolution-eda-0.5.1/exampleLibraries/analogLib/cap/
--rw-rw-rw-   0        0        0     3244 2023-05-23 19:09:34.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/cap/symbol.json
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.841848 revolution-eda-0.5.1/exampleLibraries/analogLib/capVa/
--rw-rw-rw-   0        0        0      825 2023-05-23 14:57:45.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/capVa/cap.va
--rw-rw-rw-   0        0        0     5055 2023-05-23 21:07:53.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/capVa/symbol.json
--rw-rw-rw-   0        0        0      247 2023-05-23 14:57:45.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/capVa/veriloga.json
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.855541 revolution-eda-0.5.1/exampleLibraries/analogLib/gnd/
--rw-rw-rw-   0        0        0     2017 2023-05-23 21:04:41.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/gnd/symbol.json
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.870341 revolution-eda-0.5.1/exampleLibraries/analogLib/ind/
--rw-rw-rw-   0        0        0     4485 2023-05-23 19:09:06.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/ind/symbol.json
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.881391 revolution-eda-0.5.1/exampleLibraries/analogLib/nmos/
--rw-rw-rw-   0        0        0     6697 2023-05-26 19:16:57.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/nmos/symbol.json
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.894836 revolution-eda-0.5.1/exampleLibraries/analogLib/res/
--rw-rw-rw-   0        0        0     3054 2023-05-25 12:55:41.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/res/symbol.json
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.927539 revolution-eda-0.5.1/exampleLibraries/analogLib/resVa/
--rw-rw-rw-   0        0        0      662 2023-04-01 17:10:48.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/resVa/res.va
--rw-rw-rw-   0        0        0      222 2023-02-19 22:52:34.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/resVa/veriloga.json
--rw-rw-rw-   0        0        0        0 2023-05-30 10:13:56.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/reveda.lib
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.957788 revolution-eda-0.5.1/exampleLibraries/analogLib/vaVco/
--rw-rw-rw-   0        0        0     6194 2023-05-25 11:37:58.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/vaVco/symbol.json
--rw-rw-rw-   0        0        0     1063 2023-05-22 11:34:55.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/vaVco/vaVco.va
--rw-rw-rw-   0        0        0      349 2023-05-22 11:34:55.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/vaVco/veriloga.json
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.966889 revolution-eda-0.5.1/exampleLibraries/analogLib/vdc/
--rw-rw-rw-   0        0        0     4044 2023-05-23 21:01:26.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/vdc/symbol.json
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.975522 revolution-eda-0.5.1/exampleLibraries/analogLib/vdd/
--rw-rw-rw-   0        0        0     1457 2023-05-23 21:08:20.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/vdd/symbol.json
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.982473 revolution-eda-0.5.1/exampleLibraries/analogLib/vpat/
--rw-rw-rw-   0        0        0     3132 2023-05-24 07:13:18.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/vpat/symbol.json
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.989932 revolution-eda-0.5.1/exampleLibraries/analogLib/vsin/
--rw-rw-rw-   0        0        0     5111 2023-05-23 20:43:36.000000 revolution-eda-0.5.1/exampleLibraries/analogLib/vsin/symbol.json
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.992198 revolution-eda-0.5.1/exampleLibraries/designs/
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:50.000488 revolution-eda-0.5.1/exampleLibraries/designs/LCFilter/
--rw-rw-rw-   0        0        0     1150 2023-05-23 21:17:16.000000 revolution-eda-0.5.1/exampleLibraries/designs/LCFilter/schematic.json
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:50.022676 revolution-eda-0.5.1/exampleLibraries/designs/anotherFilter/
--rw-rw-rw-   0        0        0     5252 2023-05-25 15:26:55.000000 revolution-eda-0.5.1/exampleLibraries/designs/anotherFilter/schematic.json
--rw-rw-rw-   0        0        0     3044 2023-05-23 21:11:05.000000 revolution-eda-0.5.1/exampleLibraries/designs/anotherFilter/symbol.json
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:50.042264 revolution-eda-0.5.1/exampleLibraries/designs/cascadedFilter/
--rw-rw-rw-   0        0        0       47 2023-05-30 20:37:11.000000 revolution-eda-0.5.1/exampleLibraries/designs/cascadedFilter/schematic.json
--rw-rw-rw-   0        0        0     2880 2022-12-13 11:37:24.000000 revolution-eda-0.5.1/exampleLibraries/designs/cascadedFilter/symbol.json
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:50.063172 revolution-eda-0.5.1/exampleLibraries/designs/complexFilter/
--rw-rw-rw-   0        0        0      727 2023-05-22 09:41:48.000000 revolution-eda-0.5.1/exampleLibraries/designs/complexFilter/config.json
--rw-rw-rw-   0        0        0     8530 2023-05-25 15:03:54.000000 revolution-eda-0.5.1/exampleLibraries/designs/complexFilter/schematic.json
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:50.083732 revolution-eda-0.5.1/exampleLibraries/designs/highPassFilter/
--rw-rw-rw-   0        0        0     4282 2023-05-25 18:22:47.000000 revolution-eda-0.5.1/exampleLibraries/designs/highPassFilter/schematic.json
--rw-rw-rw-   0        0        0     2874 2023-05-20 22:11:19.000000 revolution-eda-0.5.1/exampleLibraries/designs/highPassFilter/symbol.json
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:50.101880 revolution-eda-0.5.1/exampleLibraries/designs/higherOrderFilter/
--rw-rw-rw-   0        0        0     6567 2023-05-25 13:10:16.000000 revolution-eda-0.5.1/exampleLibraries/designs/higherOrderFilter/schematic.json
--rw-rw-rw-   0        0        0     2479 2023-05-23 15:10:23.000000 revolution-eda-0.5.1/exampleLibraries/designs/higherOrderFilter/symbol.json
--rw-rw-rw-   0        0        0        0 2023-05-09 20:31:10.000000 revolution-eda-0.5.1/exampleLibraries/designs/reveda.lib
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:50.123920 revolution-eda-0.5.1/exampleLibraries/designs/tb_anotherFilter/
--rw-rw-rw-   0        0        0      690 2023-05-24 17:45:31.000000 revolution-eda-0.5.1/exampleLibraries/designs/tb_anotherFilter/config.json
--rw-rw-rw-   0        0        0      662 2023-05-23 18:57:10.000000 revolution-eda-0.5.1/exampleLibraries/designs/tb_anotherFilter/res.va
--rw-rw-rw-   0        0        0     6277 2023-05-24 22:02:28.000000 revolution-eda-0.5.1/exampleLibraries/designs/tb_anotherFilter/schematic.json
--rw-rw-rw-   0        0        0    16727 2023-02-11 12:22:24.000000 revolution-eda-0.5.1/mozillaPublicLicense.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:50.147050 revolution-eda-0.5.1/pdk/
--rw-rw-rw-   0        0        0     1071 2022-12-15 13:57:32.000000 revolution-eda-0.5.1/pdk/__init__.py
--rw-rw-rw-   0        0        0     1972 2022-12-15 13:57:32.000000 revolution-eda-0.5.1/pdk/callbacks.py
--rw-rw-rw-   0        0        0      812 2023-05-31 12:57:10.000000 revolution-eda-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0     3842 2023-05-23 10:07:51.000000 revolution-eda-0.5.1/reveda.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:49.585737 revolution-eda-0.5.1/revedaEditor/
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:50.227324 revolution-eda-0.5.1/revedaEditor/backend/
--rw-rw-rw-   0        0        0     1071 2022-12-15 13:57:32.000000 revolution-eda-0.5.1/revedaEditor/backend/__init__.py
--rw-rw-rw-   0        0        0     1865 2023-05-28 21:01:30.000000 revolution-eda-0.5.1/revedaEditor/backend/dataDefinitions.py
--rw-rw-rw-   0        0        0     5918 2023-05-20 22:11:14.000000 revolution-eda-0.5.1/revedaEditor/backend/hdlBackEnd.py
--rw-rw-rw-   0        0        0    11682 2023-05-20 21:55:29.000000 revolution-eda-0.5.1/revedaEditor/backend/importViews.py
--rw-rw-rw-   0        0        0     2292 2023-03-31 22:24:42.000000 revolution-eda-0.5.1/revedaEditor/backend/libraryMethods.py
--rw-rw-rw-   0        0        0     9097 2023-05-23 12:11:02.000000 revolution-eda-0.5.1/revedaEditor/backend/schBackEnd.py
--rw-rw-rw-   0        0        0     3503 2023-05-11 17:00:40.000000 revolution-eda-0.5.1/revedaEditor/backend/undoStack.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:50.312833 revolution-eda-0.5.1/revedaEditor/common/
--rw-rw-rw-   0        0        0     1072 2023-05-13 22:43:30.000000 revolution-eda-0.5.1/revedaEditor/common/__init__.py
--rw-rw-rw-   0        0        0     2650 2022-12-16 17:29:48.000000 revolution-eda-0.5.1/revedaEditor/common/fonts.py
--rw-rw-rw-   0        0        0     2649 2022-12-15 13:57:32.000000 revolution-eda-0.5.1/revedaEditor/common/layers.py
--rw-rw-rw-   0        0        0    16666 2023-05-29 20:37:24.000000 revolution-eda-0.5.1/revedaEditor/common/net.py
--rw-rw-rw-   0        0        0     2848 2023-05-11 21:06:35.000000 revolution-eda-0.5.1/revedaEditor/common/pens.py
--rw-rw-rw-   0        0        0    61965 2023-05-28 21:54:20.000000 revolution-eda-0.5.1/revedaEditor/common/shape.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:50.352300 revolution-eda-0.5.1/revedaEditor/fileio/
--rw-rw-rw-   0        0        0     1072 2022-12-15 13:57:32.000000 revolution-eda-0.5.1/revedaEditor/fileio/__init__.py
--rw-rw-rw-   0        0        0     8844 2023-05-24 19:51:52.000000 revolution-eda-0.5.1/revedaEditor/fileio/loadJSON.py
--rw-rw-rw-   0        0        0     7358 2023-05-09 11:54:17.000000 revolution-eda-0.5.1/revedaEditor/fileio/symbolEncoder.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:50.485689 revolution-eda-0.5.1/revedaEditor/gui/
--rw-rw-rw-   0        0        0     1070 2023-05-22 14:30:52.000000 revolution-eda-0.5.1/revedaEditor/gui/__init__.py
--rw-rw-rw-   0        0        0     1617 2022-12-15 13:57:32.000000 revolution-eda-0.5.1/revedaEditor/gui/editFunctions.py
--rw-rw-rw-   0        0        0   173562 2023-05-30 11:14:11.000000 revolution-eda-0.5.1/revedaEditor/gui/editorWindows.py
--rw-rw-rw-   0        0        0    27142 2023-05-16 14:45:24.000000 revolution-eda-0.5.1/revedaEditor/gui/fileDialogues.py
--rw-rw-rw-   0        0        0    37119 2023-05-25 13:01:33.000000 revolution-eda-0.5.1/revedaEditor/gui/propertyDialogues.py
--rw-rw-rw-   0        0        0     6723 2023-03-31 22:24:42.000000 revolution-eda-0.5.1/revedaEditor/gui/pythonConsole.py
--rw-rw-rw-   0        0        0    10579 2023-05-23 18:44:24.000000 revolution-eda-0.5.1/revedaEditor/gui/revedaMain.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:50.499319 revolution-eda-0.5.1/revedaEditor/resources/
--rw-rw-rw-   0        0        0   158489 2023-02-13 11:31:30.000000 revolution-eda-0.5.1/revedaEditor/resources/resources.py
--rw-rw-rw-   0        0        0     1102 2023-05-31 12:56:51.000000 revolution-eda-0.5.1/revinit.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:57:50.536192 revolution-eda-0.5.1/revolution_eda.egg-info/
--rw-rw-rw-   0        0        0     2340 2023-05-31 12:57:49.000000 revolution-eda-0.5.1/revolution_eda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6565 2023-05-31 12:57:49.000000 revolution-eda-0.5.1/revolution_eda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 12:57:49.000000 revolution-eda-0.5.1/revolution_eda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-31 12:57:49.000000 revolution-eda-0.5.1/revolution_eda.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       31 2023-05-31 12:57:49.000000 revolution-eda-0.5.1/revolution_eda.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-05-31 12:57:49.000000 revolution-eda-0.5.1/revolution_eda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 12:57:50.538352 revolution-eda-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0       38 2023-02-11 13:22:24.000000 revolution-eda-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:39:49.615824 revolution-eda-0.5.2/
+-rw-rw-rw-   0        0        0     1087 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2340 2023-06-11 09:39:49.614805 revolution-eda-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1900 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 09:39:49.492986 revolution-eda-0.5.2/pdk/
+-rw-rw-rw-   0        0        0     1093 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/pdk/__init__.py
+-rw-rw-rw-   0        0        0     2022 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/pdk/callbacks.py
+-rw-rw-rw-   0        0        0      855 2023-06-11 09:38:14.000000 revolution-eda-0.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0     3842 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/reveda.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:39:49.466654 revolution-eda-0.5.2/revedaEditor/
+drwxrwxrwx   0        0        0        0 2023-06-11 09:39:49.532533 revolution-eda-0.5.2/revedaEditor/backend/
+-rw-rw-rw-   0        0        0     1093 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/backend/__init__.py
+-rw-rw-rw-   0        0        0     1865 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/backend/dataDefinitions.py
+-rw-rw-rw-   0        0        0     6066 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/backend/hdlBackEnd.py
+-rw-rw-rw-   0        0        0    11682 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/backend/importViews.py
+-rw-rw-rw-   0        0        0     2348 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/backend/libraryMethods.py
+-rw-rw-rw-   0        0        0     9097 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/backend/schBackEnd.py
+-rw-rw-rw-   0        0        0     3503 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/backend/undoStack.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:39:49.554051 revolution-eda-0.5.2/revedaEditor/common/
+-rw-rw-rw-   0        0        0     1095 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/common/__init__.py
+-rw-rw-rw-   0        0        0     2717 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/common/fonts.py
+-rw-rw-rw-   0        0        0     2728 2023-06-06 18:31:28.000000 revolution-eda-0.5.2/revedaEditor/common/layers.py
+-rw-rw-rw-   0        0        0    19461 2023-06-07 20:38:08.000000 revolution-eda-0.5.2/revedaEditor/common/net.py
+-rw-rw-rw-   0        0        0     2985 2023-06-06 18:36:31.000000 revolution-eda-0.5.2/revedaEditor/common/pens.py
+-rw-rw-rw-   0        0        0    63025 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/common/shape.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:39:49.565662 revolution-eda-0.5.2/revedaEditor/fileio/
+-rw-rw-rw-   0        0        0     1095 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/fileio/__init__.py
+-rw-rw-rw-   0        0        0     8915 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/fileio/loadJSON.py
+-rw-rw-rw-   0        0        0     7389 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/fileio/symbolEncoder.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:39:49.591181 revolution-eda-0.5.2/revedaEditor/gui/
+-rw-rw-rw-   0        0        0     1091 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/gui/__init__.py
+-rw-rw-rw-   0        0        0     1660 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/gui/editFunctions.py
+-rw-rw-rw-   0        0        0   172784 2023-06-10 16:46:03.000000 revolution-eda-0.5.2/revedaEditor/gui/editorWindows.py
+-rw-rw-rw-   0        0        0    27774 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/gui/fileDialogues.py
+-rw-rw-rw-   0        0        0    37477 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/gui/propertyDialogues.py
+-rw-rw-rw-   0        0        0     6916 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/gui/pythonConsole.py
+-rw-rw-rw-   0        0        0    10579 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revedaEditor/gui/revedaMain.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:39:49.593653 revolution-eda-0.5.2/revedaEditor/resources/
+-rw-rw-rw-   0        0        0   160849 2023-06-10 16:30:40.000000 revolution-eda-0.5.2/revedaEditor/resources/resources.py
+-rw-rw-rw-   0        0        0     1102 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/revinit.py
+drwxrwxrwx   0        0        0        0 2023-06-11 09:39:49.611637 revolution-eda-0.5.2/revolution_eda.egg-info/
+-rw-rw-rw-   0        0        0     2340 2023-06-11 09:39:49.000000 revolution-eda-0.5.2/revolution_eda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1127 2023-06-11 09:39:49.000000 revolution-eda-0.5.2/revolution_eda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 09:39:49.000000 revolution-eda-0.5.2/revolution_eda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-11 09:39:49.000000 revolution-eda-0.5.2/revolution_eda.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       31 2023-06-11 09:39:49.000000 revolution-eda-0.5.2/revolution_eda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-06-11 09:39:49.000000 revolution-eda-0.5.2/revolution_eda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 09:39:49.615824 revolution-eda-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-06-05 14:29:55.000000 revolution-eda-0.5.2/setup.py
```

### Comparing `revolution-eda-0.5.1/LICENSE.txt` & `revolution-eda-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revolution-eda-0.5.1/PKG-INFO` & `revolution-eda-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revolution-eda
-Version: 0.5.1
+Version: 0.5.2
 Summary: Revolution EDA is a new generation integrated circuit design environment.
 Project-URL: Homepage, https://github.com/eskiyerli/revedaRelease
 Keywords: electronic,design,schematic
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `revolution-eda-0.5.1/README.md` & `revolution-eda-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `revolution-eda-0.5.1/pdk/__init__.py` & `revolution-eda-0.5.2/revedaEditor/common/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
+
+#   “Commons Clause” License Condition v1.0
+#  #
+#   The Software is provided to you by the Licensor under the License, as defined
+#   below, subject to the following condition.
+#  #
+#   Without limiting other conditions in the License, the grant of rights under the
+#   License will not include, and the License does not grant to you, the right to
+#   Sell the Software.
+#  #
+#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#   granted to you under the License to provide to third parties, for a fee or other
+#   consideration (including without limitation fees for hosting or consulting/
+#   support services related to the Software), a product or service whose value
+#   derives, entirely or substantially, from the functionality of the Software. Any
+#   license notice or attribution required by the License must also include this
+#   Commons Clause License Condition notice.
+#  #
+#   Software: Revolution EDA
+#   License: Mozilla Public License 2.0
+#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
+
```

### Comparing `revolution-eda-0.5.1/pdk/callbacks.py` & `revolution-eda-0.5.2/pdk/callbacks.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
-from quantiphy import Quantity
-
-class baseInst():
-    def __init__(self, labels_dict: dict):
-        self._labelsDict = labels_dict
-
-class res(baseInst):
-    def __init__(self,labels_dict:dict):
-        super().__init__(labels_dict)
-
-    def doubleR(self):
-        Rvalue = self._labelsDict.get('R').labelValue
-        if Rvalue.isalnum():
-            return str(2*Quantity(Rvalue))
-        return '?'
-
-class nmos(baseInst):
-    def __init__(self,labels_dict:dict):
-        super().__init__(labels_dict)
-        self.w = Quantity(self._labelsDict['w'].labelValue)
-        self.l = Quantity(self._labelsDict['l'].labelValue)
-        self.nf= Quantity(self._labelsDict['nf'].labelValue)
-        self.sd1p8v = 0.28
-        self.sa1p8v = sb1p8v = 0.265
-        self.sourceDiffs = lambda nf: int(int(nf) / 2 + 1)
-
-    def asparm(self):
-        return self.sourceDiffs(self.nf)*(self.w/self.nf)*self.sd1p8v
+
+#   “Commons Clause” License Condition v1.0
+#  #
+#   The Software is provided to you by the Licensor under the License, as defined
+#   below, subject to the following condition.
+#  #
+#   Without limiting other conditions in the License, the grant of rights under the
+#   License will not include, and the License does not grant to you, the right to
+#   Sell the Software.
+#  #
+#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#   granted to you under the License to provide to third parties, for a fee or other
+#   consideration (including without limitation fees for hosting or consulting/
+#   support services related to the Software), a product or service whose value
+#   derives, entirely or substantially, from the functionality of the Software. Any
+#   license notice or attribution required by the License must also include this
+#   Commons Clause License Condition notice.
+#  #
+#   Software: Revolution EDA
+#   License: Mozilla Public License 2.0
+#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
+from quantiphy import Quantity
+
+class baseInst():
+    def __init__(self, labels_dict: dict):
+        self._labelsDict = labels_dict
+
+class res(baseInst):
+    def __init__(self,labels_dict:dict):
+        super().__init__(labels_dict)
+
+    def doubleR(self):
+        Rvalue = self._labelsDict.get('R').labelValue
+        if Rvalue.isalnum():
+            return str(2*Quantity(Rvalue))
+        return '?'
+
+class nmos(baseInst):
+    def __init__(self,labels_dict:dict):
+        super().__init__(labels_dict)
+        self.w = Quantity(self._labelsDict['w'].labelValue)
+        self.l = Quantity(self._labelsDict['l'].labelValue)
+        self.nf= Quantity(self._labelsDict['nf'].labelValue)
+        self.sd1p8v = 0.28
+        self.sa1p8v = sb1p8v = 0.265
+        self.sourceDiffs = lambda nf: int(int(nf) / 2 + 1)
+
+    def asparm(self):
+        return self.sourceDiffs(self.nf)*(self.w/self.nf)*self.sd1p8v
```

### Comparing `revolution-eda-0.5.1/pyproject.toml` & `revolution-eda-0.5.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #
 [build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
+requires = ["setuptools>=61.0.0", "wheel", "quantiphy>=2.19", "python-dotenv>=1.0.0"]
 build-backend = "setuptools.build_meta"
 [tool.setuptools]
 packages = ['revedaEditor.gui','revedaEditor.common','revedaEditor.fileio','revedaEditor.backend','revedaEditor.resources','pdk']
 py-modules = ['revinit', 'reveda']
 [project]
 name = "revolution-eda"
-version = "0.5.1"
+version = "0.5.2"
 description = 'Revolution EDA is a new generation integrated circuit design environment.'
 readme = "README.md"
 classifiers = ["Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["electronic", "design", "schematic"]
 dependencies = ["PySide6>=6.4.2",
```

### Comparing `revolution-eda-0.5.1/reveda.py` & `revolution-eda-0.5.2/reveda.py`

 * *Files identical despite different names*

### Comparing `revolution-eda-0.5.1/revedaEditor/backend/__init__.py` & `revolution-eda-0.5.2/revedaEditor/fileio/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
+
+#   “Commons Clause” License Condition v1.0
+#  #
+#   The Software is provided to you by the Licensor under the License, as defined
+#   below, subject to the following condition.
+#  #
+#   Without limiting other conditions in the License, the grant of rights under the
+#   License will not include, and the License does not grant to you, the right to
+#   Sell the Software.
+#  #
+#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#   granted to you under the License to provide to third parties, for a fee or other
+#   consideration (including without limitation fees for hosting or consulting/
+#   support services related to the Software), a product or service whose value
+#   derives, entirely or substantially, from the functionality of the Software. Any
+#   license notice or attribution required by the License must also include this
+#   Commons Clause License Condition notice.
+#  #
+#   Software: Revolution EDA
+#   License: Mozilla Public License 2.0
+#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
+
```

### Comparing `revolution-eda-0.5.1/revedaEditor/backend/dataDefinitions.py` & `revolution-eda-0.5.2/revedaEditor/backend/dataDefinitions.py`

 * *Files identical despite different names*

### Comparing `revolution-eda-0.5.1/revedaEditor/backend/hdlBackEnd.py` & `revolution-eda-0.5.2/revedaEditor/backend/hdlBackEnd.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
-import pathlib
-
-
-class verilogaC:
-    """
-    This class represents an imported verilog-A module.
-    """
-
-    def __init__(self, pathObj: pathlib.Path):
-        self._pathObj = pathObj
-        keyWords = ["analog", "electrical"]
-        self._vaModule = ''
-        self.instanceParams = dict()
-        self.modelParams = dict()
-        self.inPins = list()
-        self.inoutPins = list()
-        self.outPins = list()
-        self._netlistLine = ''
-        self.statementLines = list()
-        self._pinOrder = ''
-
-        with open(self._pathObj) as f:
-            self.fileLines = f.readlines()
-        self.stripComments()
-        self.oneLiners()
-        # splitLines=[fileline.split() for fileline in fileLines]
-
-    def stripComments(self):
-
-        comment = False
-        for line in self.fileLines:  # concatenate the lines until it reaches a ;
-            stripLine = line.strip()
-            if stripLine.startswith('/*'):
-                comment = True
-            if not comment:
-                doubleSlashLoc = stripLine.find('//')
-                if doubleSlashLoc > -1:
-                    stripLine = stripLine[:doubleSlashLoc]
-                if stripLine != '':
-                    self.statementLines.append(stripLine)
-            if comment and stripLine.endswith('*/'):
-                comment = False
-
-    def oneLiners(self):
-        tempLine = ''
-        oneLiners = list()
-        for line in self.statementLines:
-            stripLine = line.strip()
-            if not stripLine.startswith('`include'):
-                tempLine = f'{tempLine} {stripLine}'
-            if stripLine.endswith(';'):
-                oneLiners.append(tempLine.strip())
-                splitLine = tempLine.strip().split()
-                if splitLine:
-                    if splitLine[0] == 'module':
-                        self._vaModule = splitLine[1].split('(')[0]
-                        indexLow = line.index("(")
-                        indexHigh = line.index(")")
-                        self.pins = [pin.strip() for pin in
-                                     line[indexLow + 1: indexHigh].split(",")]
-                    elif splitLine[0] == 'in' or splitLine[0] == 'input':
-                        pinsList = splitLine[1].split(';')[0].split(',')
-                        self.inPins.extend([pin.strip() for pin in pinsList])
-                    elif splitLine[0] == 'out' or splitLine[0] == 'output':
-                        pinsList = splitLine[1].split(';')[0].split(',')
-                        self.outPins.extend([pin.strip() for pin in pinsList])
-                    elif splitLine[0] == 'inout':
-                        pinsList = splitLine[1].split(';')[0].split(',')
-                        self.inoutPins.extend([pin.strip() for pin in pinsList])
-
-                    elif splitLine[0] == "parameter":
-                        paramDefPart = tempLine.split('*(')[0]
-                        paramName = paramDefPart.split('=')[0].split()[-1].strip()
-                        paramValue = paramDefPart.split('=')[1].split()[0].strip()
-
-                        try:
-                            paramAttr = tempLine.strip().split("(*")[1]
-                        except IndexError:
-                            paramAttr = ""
-                        if "type" in paramAttr and '"instance"' in paramAttr:
-                            # parameter value is between = and (*
-                            self.instanceParams[paramName] = paramValue
-                            if "xyceAlsoModel" in paramAttr and '"yes"' in paramAttr:
-                                self.modelParams[paramName] = paramValue
-                        else:  # no parameter attribute statement
-                            self.modelParams[paramName] = paramValue
-                tempLine = ''
-
-    @property
-    def pathObj(self):
-        return self._pathObj
-
-    @pathObj.setter
-    def pathObj(self, value:pathlib.Path):
-        assert isinstance(value,pathlib.Path)
-        self._pathObj = value
-
-    @property
-    def pinOrder(self):
-        return self._pinOrder
-
-    @pinOrder.setter
-    def pinOrder(self, value:str):
-        assert isinstance(value,str)
-        self._pinOrder = value
-
-    @property
-    def netlistLine(self):
-        self._pinOrder = ','.join(self.pins)
-        print(f'pinOrder : {self.pinOrder}')
-        instParamString = ' '.join(
-            [f'[@{key}:{key}=%:{key}={item}]' for key, item in
-             self.instanceParams.items()])
-        self._netlistLine = f'Y{self._vaModule} [@instName] [@pinList]  ' \
-                            f'{self._vaModule}Model {instParamString}'
-        return self._netlistLine
-
-    @netlistLine.setter
-    def netListLine(self, value:str):
-        assert isinstance(value,str)
-        self._netlistLine = value
-
-    @property
-    def vaModule(self):
-        return self._vaModule
-
+
+#   “Commons Clause” License Condition v1.0
+#  #
+#   The Software is provided to you by the Licensor under the License, as defined
+#   below, subject to the following condition.
+#  #
+#   Without limiting other conditions in the License, the grant of rights under the
+#   License will not include, and the License does not grant to you, the right to
+#   Sell the Software.
+#  #
+#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#   granted to you under the License to provide to third parties, for a fee or other
+#   consideration (including without limitation fees for hosting or consulting/
+#   support services related to the Software), a product or service whose value
+#   derives, entirely or substantially, from the functionality of the Software. Any
+#   license notice or attribution required by the License must also include this
+#   Commons Clause License Condition notice.
+#  #
+#   Software: Revolution EDA
+#   License: Mozilla Public License 2.0
+#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
+import pathlib
+
+
+class verilogaC:
+    """
+    This class represents an imported verilog-A module.
+    """
+
+    def __init__(self, pathObj: pathlib.Path):
+        self._pathObj = pathObj
+        keyWords = ["analog", "electrical"]
+        self._vaModule = ''
+        self.instanceParams = dict()
+        self.modelParams = dict()
+        self.inPins = list()
+        self.inoutPins = list()
+        self.outPins = list()
+        self._netlistLine = ''
+        self.statementLines = list()
+        self._pinOrder = ''
+
+        with open(self._pathObj) as f:
+            self.fileLines = f.readlines()
+        self.stripComments()
+        self.oneLiners()
+        # splitLines=[fileline.split() for fileline in fileLines]
+
+    def stripComments(self):
+
+        comment = False
+        for line in self.fileLines:  # concatenate the lines until it reaches a ;
+            stripLine = line.strip()
+            if stripLine.startswith('/*'):
+                comment = True
+            if not comment:
+                doubleSlashLoc = stripLine.find('//')
+                if doubleSlashLoc > -1:
+                    stripLine = stripLine[:doubleSlashLoc]
+                if stripLine != '':
+                    self.statementLines.append(stripLine)
+            if comment and stripLine.endswith('*/'):
+                comment = False
+
+    def oneLiners(self):
+        tempLine = ''
+        oneLiners = list()
+        for line in self.statementLines:
+            stripLine = line.strip()
+            if not stripLine.startswith('`include'):
+                tempLine = f'{tempLine} {stripLine}'
+            if stripLine.endswith(';'):
+                oneLiners.append(tempLine.strip())
+                splitLine = tempLine.strip().split()
+                if splitLine:
+                    if splitLine[0] == 'module':
+                        self._vaModule = splitLine[1].split('(')[0]
+                        indexLow = line.index("(")
+                        indexHigh = line.index(")")
+                        self.pins = [pin.strip() for pin in
+                                     line[indexLow + 1: indexHigh].split(",")]
+                    elif splitLine[0] == 'in' or splitLine[0] == 'input':
+                        pinsList = splitLine[1].split(';')[0].split(',')
+                        self.inPins.extend([pin.strip() for pin in pinsList])
+                    elif splitLine[0] == 'out' or splitLine[0] == 'output':
+                        pinsList = splitLine[1].split(';')[0].split(',')
+                        self.outPins.extend([pin.strip() for pin in pinsList])
+                    elif splitLine[0] == 'inout':
+                        pinsList = splitLine[1].split(';')[0].split(',')
+                        self.inoutPins.extend([pin.strip() for pin in pinsList])
+
+                    elif splitLine[0] == "parameter":
+                        paramDefPart = tempLine.split('*(')[0]
+                        paramName = paramDefPart.split('=')[0].split()[-1].strip()
+                        paramValue = paramDefPart.split('=')[1].split()[0].strip()
+
+                        try:
+                            paramAttr = tempLine.strip().split("(*")[1]
+                        except IndexError:
+                            paramAttr = ""
+                        if "type" in paramAttr and '"instance"' in paramAttr:
+                            # parameter value is between = and (*
+                            self.instanceParams[paramName] = paramValue
+                            if "xyceAlsoModel" in paramAttr and '"yes"' in paramAttr:
+                                self.modelParams[paramName] = paramValue
+                        else:  # no parameter attribute statement
+                            self.modelParams[paramName] = paramValue
+                tempLine = ''
+
+    @property
+    def pathObj(self):
+        return self._pathObj
+
+    @pathObj.setter
+    def pathObj(self, value:pathlib.Path):
+        assert isinstance(value,pathlib.Path)
+        self._pathObj = value
+
+    @property
+    def pinOrder(self):
+        return self._pinOrder
+
+    @pinOrder.setter
+    def pinOrder(self, value:str):
+        assert isinstance(value,str)
+        self._pinOrder = value
+
+    @property
+    def netlistLine(self):
+        self._pinOrder = ','.join(self.pins)
+        print(f'pinOrder : {self.pinOrder}')
+        instParamString = ' '.join(
+            [f'[@{key}:{key}=%:{key}={item}]' for key, item in
+             self.instanceParams.items()])
+        self._netlistLine = f'Y{self._vaModule} [@instName] [@pinList]  ' \
+                            f'{self._vaModule}Model {instParamString}'
+        return self._netlistLine
+
+    @netlistLine.setter
+    def netListLine(self, value:str):
+        assert isinstance(value,str)
+        self._netlistLine = value
+
+    @property
+    def vaModule(self):
+        return self._vaModule
+
```

### Comparing `revolution-eda-0.5.1/revedaEditor/backend/importViews.py` & `revolution-eda-0.5.2/revedaEditor/backend/importViews.py`

 * *Files identical despite different names*

### Comparing `revolution-eda-0.5.1/revedaEditor/backend/libraryMethods.py` & `revolution-eda-0.5.2/revedaEditor/backend/libraryMethods.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-#    “Commons Clause” License Condition v1.0
-#   #
-#    The Software is provided to you by the Licensor under the License, as defined
-#    below, subject to the following condition.
-#   #
-#    Without limiting other conditions in the License, the grant of rights under the
-#    License will not include, and the License does not grant to you, the right to
-#    Sell the Software.
-#   #
-#    For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#    granted to you under the License to provide to third parties, for a fee or other
-#    consideration (including without limitation fees for hosting or consulting/
-#    support services related to the Software), a product or service whose value
-#    derives, entirely or substantially, from the functionality of the Software. Any
-#    license notice or attribution required by the License must also include this
-#    Commons Clause License Condition notice.
-#   #
-#    Software: Revolution EDA
-#    License: Mozilla Public License 2.0
-#    Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
-from PySide6.QtCore import (Qt, )
-from PySide6.QtGui import (QStandardItemModel)
-
-import revedaEditor.backend.schBackEnd as scb
-
-
-def getLibItem(libraryModel: QStandardItemModel, libName: str) -> scb.libraryItem:
-    libItem = [item for item in libraryModel.findItems(libName) if
-               item.data(Qt.UserRole + 1) == 'library'][0]
-    return libItem
-
-
-def getCellItem(libItem: scb.libraryItem, cellNameInp: str) -> scb.cellItem:
-    cellItems = [libItem.child(i) for i in range(libItem.rowCount()) if
-                 libItem.child(i).cellName == cellNameInp]
-    if cellItems:
-        return cellItems[0]
-    else:
-        return None
-
-
-def getViewItem(cellItem: scb.cellItem, viewNameInp: str) -> scb.viewItem:
-    if cellItem is not None:
-        viewItems = [cellItem.child(i) for i in range(cellItem.rowCount()) if
-                     cellItem.child(i).text() == viewNameInp]
-    else:
-        return None
-    if viewItems:
-        return viewItems[0]
-    else:
-        return None
-
-def findViewItem(libraryModel, libName:str,cellName:str,viewName:str):
-    libItem = getLibItem(libraryModel,libName)
-    cellItem = getCellItem(libItem, cellName)
+#    “Commons Clause” License Condition v1.0
+#   #
+#    The Software is provided to you by the Licensor under the License, as defined
+#    below, subject to the following condition.
+#   #
+#    Without limiting other conditions in the License, the grant of rights under the
+#    License will not include, and the License does not grant to you, the right to
+#    Sell the Software.
+#   #
+#    For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#    granted to you under the License to provide to third parties, for a fee or other
+#    consideration (including without limitation fees for hosting or consulting/
+#    support services related to the Software), a product or service whose value
+#    derives, entirely or substantially, from the functionality of the Software. Any
+#    license notice or attribution required by the License must also include this
+#    Commons Clause License Condition notice.
+#   #
+#    Software: Revolution EDA
+#    License: Mozilla Public License 2.0
+#    Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
+from PySide6.QtCore import (Qt, )
+from PySide6.QtGui import (QStandardItemModel)
+
+import revedaEditor.backend.schBackEnd as scb
+
+
+def getLibItem(libraryModel: QStandardItemModel, libName: str) -> scb.libraryItem:
+    libItem = [item for item in libraryModel.findItems(libName) if
+               item.data(Qt.UserRole + 1) == 'library'][0]
+    return libItem
+
+
+def getCellItem(libItem: scb.libraryItem, cellNameInp: str) -> scb.cellItem:
+    cellItems = [libItem.child(i) for i in range(libItem.rowCount()) if
+                 libItem.child(i).cellName == cellNameInp]
+    if cellItems:
+        return cellItems[0]
+    else:
+        return None
+
+
+def getViewItem(cellItem: scb.cellItem, viewNameInp: str) -> scb.viewItem:
+    if cellItem is not None:
+        viewItems = [cellItem.child(i) for i in range(cellItem.rowCount()) if
+                     cellItem.child(i).text() == viewNameInp]
+    else:
+        return None
+    if viewItems:
+        return viewItems[0]
+    else:
+        return None
+
+def findViewItem(libraryModel, libName:str,cellName:str,viewName:str):
+    libItem = getLibItem(libraryModel,libName)
+    cellItem = getCellItem(libItem, cellName)
     return getViewItem(cellItem,viewName)
```

### Comparing `revolution-eda-0.5.1/revedaEditor/backend/schBackEnd.py` & `revolution-eda-0.5.2/revedaEditor/backend/schBackEnd.py`

 * *Files identical despite different names*

### Comparing `revolution-eda-0.5.1/revedaEditor/backend/undoStack.py` & `revolution-eda-0.5.2/revedaEditor/backend/undoStack.py`

 * *Files identical despite different names*

### Comparing `revolution-eda-0.5.1/revedaEditor/common/__init__.py` & `revolution-eda-0.5.2/pdk/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
-
+
+#   “Commons Clause” License Condition v1.0
+#  #
+#   The Software is provided to you by the Licensor under the License, as defined
+#   below, subject to the following condition.
+#  #
+#   Without limiting other conditions in the License, the grant of rights under the
+#   License will not include, and the License does not grant to you, the right to
+#   Sell the Software.
+#  #
+#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#   granted to you under the License to provide to third parties, for a fee or other
+#   consideration (including without limitation fees for hosting or consulting/
+#   support services related to the Software), a product or service whose value
+#   derives, entirely or substantially, from the functionality of the Software. Any
+#   license notice or attribution required by the License must also include this
+#   Commons Clause License Condition notice.
+#  #
+#   Software: Revolution EDA
+#   License: Mozilla Public License 2.0
+#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
```

### Comparing `revolution-eda-0.5.1/revedaEditor/common/fonts.py` & `revolution-eda-0.5.2/revedaEditor/common/fonts.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
-from PySide6.QtGui import (QFont, QFontMetrics, QFontDatabase)
-
-class font(QFont):
-    def __init__(self,fontFamily:str, fontStyle:str, fontSize:int, kerning:bool,logger):
-        self._fontFamily = fontFamily
-        self._fontStyle = fontStyle
-        self._fontSize = fontSize
-        self._kerning = kerning
-        self._logger = logger
-        self.setFamily(self._fontFamily)
-        self.setStyle(self._fontStyle)
-        self.setPointSize(self._fontSize)
-        self.setKerning(self._kerning)
-        self.setStyleHint(QFont.TypeWriter)
-
-    @property
-    def fontFamily(self):
-        return self._fontFamily
-
-    @fontFamily.setter
-    def fontFamily(self, value:str):
-        fontFamilies = QFontDatabase.families(QFontDatabase.Latin)
-        fixedFamilies = [family for family in fontFamilies if
-                         QFontDatabase.isFixedPitch(family)]
-        if value not in fixedFamilies:
-            self._logger.warning('No such font family present in the system. Another '
-                                 'font '
-                           'will be substituted.')
-        self._fontFamily = value
-        self.setFamily(self._fontFamily)
-
-    @property
-    def fontStyle(self):
-        return self._fontStyle
-
-    @fontStyle.setter
-    def fontStyle(self,value:str):
-        fstyles = QFontDatabase.styles(self._fontFamily)
-        if value not in fstyles:
-            self._logger.warning(f'No matching style is available. Available styles '
-                                 f'are: {",".join(fstyles)}')
-        else:
-            self.setStyle(value)
-
-
+
+#   “Commons Clause” License Condition v1.0
+#  #
+#   The Software is provided to you by the Licensor under the License, as defined
+#   below, subject to the following condition.
+#  #
+#   Without limiting other conditions in the License, the grant of rights under the
+#   License will not include, and the License does not grant to you, the right to
+#   Sell the Software.
+#  #
+#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#   granted to you under the License to provide to third parties, for a fee or other
+#   consideration (including without limitation fees for hosting or consulting/
+#   support services related to the Software), a product or service whose value
+#   derives, entirely or substantially, from the functionality of the Software. Any
+#   license notice or attribution required by the License must also include this
+#   Commons Clause License Condition notice.
+#  #
+#   Software: Revolution EDA
+#   License: Mozilla Public License 2.0
+#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
+from PySide6.QtGui import (QFont, QFontMetrics, QFontDatabase)
+
+class font(QFont):
+    def __init__(self,fontFamily:str, fontStyle:str, fontSize:int, kerning:bool,logger):
+        self._fontFamily = fontFamily
+        self._fontStyle = fontStyle
+        self._fontSize = fontSize
+        self._kerning = kerning
+        self._logger = logger
+        self.setFamily(self._fontFamily)
+        self.setStyle(self._fontStyle)
+        self.setPointSize(self._fontSize)
+        self.setKerning(self._kerning)
+        self.setStyleHint(QFont.TypeWriter)
+
+    @property
+    def fontFamily(self):
+        return self._fontFamily
+
+    @fontFamily.setter
+    def fontFamily(self, value:str):
+        fontFamilies = QFontDatabase.families(QFontDatabase.Latin)
+        fixedFamilies = [family for family in fontFamilies if
+                         QFontDatabase.isFixedPitch(family)]
+        if value not in fixedFamilies:
+            self._logger.warning('No such font family present in the system. Another '
+                                 'font '
+                           'will be substituted.')
+        self._fontFamily = value
+        self.setFamily(self._fontFamily)
+
+    @property
+    def fontStyle(self):
+        return self._fontStyle
+
+    @fontStyle.setter
+    def fontStyle(self,value:str):
+        fstyles = QFontDatabase.styles(self._fontFamily)
+        if value not in fstyles:
+            self._logger.warning(f'No matching style is available. Available styles '
+                                 f'are: {",".join(fstyles)}')
+        else:
+            self.setStyle(value)
+
+
```

### Comparing `revolution-eda-0.5.1/revedaEditor/common/layers.py` & `revolution-eda-0.5.2/revedaEditor/common/layers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
-# Schematic and symbol editor classes
-# (C) Revolution Semiconductor, 2021
-from PySide6.QtGui import (QColor)
-
-
-class layer:
-    def __init__(self, name, color, z, visible):
-        self.name = name
-        self.color = color  # QColor type
-        self.z = z
-        self.visible = visible
-
-    def __str__(self):
-        return f'{self.name}  {str(self.color.toTuple())} {str(self.z)} {str(self.visible)}'
-
-    def __repr__(self):
-        return f'{self.name}  {str(self.color.toTuple())} {str(self.z)} {str(self.visible)}'
-
-    def __eq__(self, other):
-        return (self.name == other.cellName and self.color == other.color and self.z ==
-                other.z and self.visible == other.visible)
-
-    def __ne__(self, other):
-        return not self.__eq__(other)
-
-    def layerDelete(self):
-        del self
-
-
-wireLayer = layer(name="wireLayer", color=QColor("cyan"), z=1, visible=True)
-symbolLayer = layer(name="symbolLayer", color=QColor("green"), z=1, visible=True)
-guideLineLayer = layer(name="guideLineLayer", color=QColor("white"), z=1, visible=True)
-selectedWireLayer = layer(name="selectedWireLayer", color=QColor("red"), z=1,
-                          visible=True)
-pinLayer = layer(name="pinLayer", color=QColor("red"), z=2, visible=True)
-labelLayer = layer(name="labelLayer", color=QColor("yellow"), z=3, visible=True)
-textLayer = layer(name="textLayer", color=QColor("white"), z=4, visible=True)
-otherLayer = layer(name='otherLayer', color=QColor('white'), z=1, visible= True)
-draftLayer = layer(name='draftLayer', color = QColor('gray'), z=1, visible= True)
+
+#   “Commons Clause” License Condition v1.0
+#  #
+#   The Software is provided to you by the Licensor under the License, as defined
+#   below, subject to the following condition.
+#  #
+#   Without limiting other conditions in the License, the grant of rights under the
+#   License will not include, and the License does not grant to you, the right to
+#   Sell the Software.
+#  #
+#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#   granted to you under the License to provide to third parties, for a fee or other
+#   consideration (including without limitation fees for hosting or consulting/
+#   support services related to the Software), a product or service whose value
+#   derives, entirely or substantially, from the functionality of the Software. Any
+#   license notice or attribution required by the License must also include this
+#   Commons Clause License Condition notice.
+#  #
+#   Software: Revolution EDA
+#   License: Mozilla Public License 2.0
+#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
+# Schematic and symbol editor classes
+# (C) Revolution Semiconductor, 2021
+from PySide6.QtGui import (QColor, QColorConstants)
+
+
+class layer:
+    def __init__(self, name, color, z, visible):
+        self.name = name
+        self.color = color  # QColor type
+        self.z = z
+        self.visible = visible
+
+    def __str__(self):
+        return f'{self.name}  {str(self.color.toTuple())} {str(self.z)} {str(self.visible)}'
+
+    def __repr__(self):
+        return f'{self.name}  {str(self.color.toTuple())} {str(self.z)} {str(self.visible)}'
+
+    def __eq__(self, other):
+        return (self.name == other.cellName and self.color == other.color and self.z ==
+                other.z and self.visible == other.visible)
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
+    def layerDelete(self):
+        del self
+
+
+wireLayer = layer(name="wireLayer", color=QColor("cyan"), z=1, visible=True)
+symbolLayer = layer(name="symbolLayer", color=QColor("green"), z=1, visible=True)
+guideLineLayer = layer(name="guideLineLayer", color=QColor("white"), z=1, visible=True)
+selectedWireLayer = layer(name="selectedWireLayer", color=QColor("red"), z=1,
+                          visible=True)
+pinLayer = layer(name="pinLayer", color=QColor("red"), z=2, visible=True)
+labelLayer = layer(name="labelLayer", color=QColor("yellow"), z=3, visible=True)
+textLayer = layer(name="textLayer", color=QColor("white"), z=4, visible=True)
+otherLayer = layer(name='otherLayer', color=QColor('white'), z=1, visible= True)
+draftLayer = layer(name='draftLayer', color = QColor('gray'), z=1, visible= True)
```

### Comparing `revolution-eda-0.5.1/revedaEditor/common/net.py` & `revolution-eda-0.5.2/revedaEditor/common/net.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 #  #
 #   Software: Revolution EDA
 #   License: Mozilla Public License 2.0
 #   Licensor: Revolution Semiconductor (Registered in the Netherlands)
 
 # net class definition.
 from PySide6.QtCore import (QPoint, Qt, QLineF, QRectF, QPointF, QRect)
-from PySide6.QtGui import (QPen, QStaticText, QPainterPath, QColor, QFont,)
-from PySide6.QtWidgets import (QGraphicsLineItem, QGraphicsItem,
+from PySide6.QtGui import (QPen, QStaticText, QPainterPath, QColor, QFont,QColorConstants)
+from PySide6.QtWidgets import (QGraphicsLineItem, QGraphicsItem, QGraphicsPathItem,
                                QGraphicsEllipseItem, QGraphicsRectItem,
-                               QGraphicsSceneMouseEvent)
+                               QGraphicsSceneMouseEvent, QGraphicsSceneHoverEvent,)
 # import revedaEditor.common.pens as pens
 import revedaEditor.backend.dataDefinitions as ddef
 import revedaEditor.backend.undoStack as us
 
 
 class schematicNet(QGraphicsLineItem):
     '''
@@ -49,21 +49,25 @@
         self._nameConflict = False  # if a name conflict has been detected
         super().__init__(QLineF(self._start, self._end))
         self.setPen(self._pen)
         self.setFlag(QGraphicsItem.ItemIsMovable, True)
         self.setFlag(QGraphicsItem.ItemIsSelectable, True)
         self.setFlag(QGraphicsItem.ItemSendsGeometryChanges, True)
         self.setFlag(QGraphicsItem.ItemIsFocusable, True)
+        self.setAcceptHoverEvents(True)
         # self._createdNets = dict()
         self._endPoints = [self._start, self._end]
         self._dots = set()
         self._dotPoints = set()
         # self._touchingNets = set()
         self._dashedLines = dict()
         self._newWires = list()
+        self._connectedNetsSet = set()
+        self._flightLinesSet = set()
+        self._highlighted = False
 
     def __repr__(self):
         return f"schematicNet(start={self.mapToScene(self._start)}, " \
                f"end={self.mapToScene(self._end)}"
 
     def shape(self):
         '''
@@ -76,14 +80,16 @@
         return path
 
     def paint(self, painter, option, widget) -> None:
         line = self.line()
         painter.setPen(self._pen)
         if self.isSelected():
             painter.setPen(QPen(Qt.blue, 2, Qt.SolidLine))
+        elif self._highlighted:
+            painter.setPen(self.scene().hilightPen)
         if self.name is not None:
             if self._nameConflict:
                 painter.setPen(QPen(Qt.red, 2, Qt.SolidLine))
             # if there is name conflict, draw the line and name in red.
             textLoc = line.center()
             painter.drawStaticText(textLoc, QStaticText(self.name))
         painter.drawLine(line)
@@ -95,14 +101,54 @@
             if self.scene().drawWire:
                 return False
             super().sceneEvent(event)
             return True
         except AttributeError:
             return False
 
+    def hoverEnterEvent(self, event: QGraphicsSceneHoverEvent) -> None:
+        super().hoverEnterEvent(event)
+        if self.scene().highlightNets:
+            self._connectedNetsSet = {netItem for netItem in self.scene().items() if ((
+                    isinstance(netItem, schematicNet) and (self.nameSet or self.nameAdded) and
+                                                           netItem.name == self.name))}
+            [netItem.highlight() for netItem in self._connectedNetsSet]
+            for netItem in self._connectedNetsSet:
+                flightLine = netFlightLine(self.mapToScene(self.line().center()),
+                                           netItem.mapToScene(netItem.line().center()),
+                                           self.scene().hilightPen)
+                self._flightLinesSet.add(flightLine)
+                self.scene().addItem(flightLine)
+
+    def hoverLeaveEvent(self, event: QGraphicsSceneHoverEvent) -> None:
+        super().hoverLeaveEvent(event)
+        if self._highlighted:
+            for flightLine in self._flightLinesSet:
+                self.scene().removeItem(flightLine)
+            self._flightLinesSet = set()
+        [netItem.unhighlight() for netItem in self._connectedNetsSet]
+
+    def highlight(self):
+        self._highlighted = True
+        self.update()
+
+    def unhighlight(self):
+        self._highlighted = False
+        self.update()
+
+    @property
+    def highlighted(self):
+        return self._highlighted
+
+    @highlighted.setter
+    def highlighted(self, value: bool):
+        self._highlighted = value
+
+
+
     @property
     def start(self):
         return self._start
         # return self._start
 
     @start.setter
     def start(self, start: QPoint):
@@ -142,14 +188,23 @@
 
 
 
     @property
     def nameSet(self) -> bool:
         return self._nameSet
 
+    @property
+    def nameAdded(self) -> bool:
+        return self._nameAdded
+
+    @nameAdded.setter
+    def nameAdded(self, value: bool):
+        assert isinstance(value,bool)
+        self._nameAdded = value
+
     @nameSet.setter
     def nameSet(self, value: bool):
         assert isinstance(value,bool)
         self._nameSet = value
 
     @property
     def nameConflict(self) -> bool:
@@ -381,14 +436,34 @@
             self.start = QPoint(self.start.x(),startY)
             self.end = QPoint(self.end.x(),endY)
             self.update()
             for netItem in nets.difference({self}):
                 self.scene().removeItem(netItem)
                 del netItem
 
+class netFlightLine(QGraphicsPathItem):
+    def __init__(self, start: QPoint, end: QPoint, pen: QPen):
+        self._start = start
+        self._end = end
+        self._pen = pen
+        super().__init__()
+
+    def paint(self, painter, option, widget) -> None:
+
+        painter.setPen(self._pen)
+        line = QLineF(self._start, self._end)
+        perpendicularLine =  QLineF(line.center(), line.center()+QPointF(-line.dy(), line.dx()))
+        perpendicularLine.setLength(100)
+
+        path = QPainterPath()
+        path.moveTo(self._start)
+        path.quadTo(perpendicularLine.p2(), self._end)
+        painter.drawPath(path)
+
+
 
 class crossingDot(QGraphicsEllipseItem):
     def __init__(self, point: QPoint, radius: int, pen: QPen):
         self.radius = radius
         self._pen = pen
         self.point = point
         super().__init__(point.x() - radius, point.y() - radius, 2 * radius, 2 * radius)
```

### Comparing `revolution-eda-0.5.1/revedaEditor/common/pens.py` & `revolution-eda-0.5.2/revedaEditor/common/pens.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #   Commons Clause License Condition notice.
 #  #
 #   Software: Revolution EDA
 #   License: Mozilla Public License 2.0
 #   Licensor: Revolution Semiconductor (Registered in the Netherlands)
 
 from PySide6.QtCore import (Qt)
-from PySide6.QtGui import (QPen, QColor)
+from PySide6.QtGui import (QPen, QColor, QColorConstants)
 
 from revedaEditor.common.layers import (wireLayer, symbolLayer,
                                         selectedWireLayer, pinLayer,
                                         labelLayer,
                                         textLayer, draftLayer)
 
 
@@ -59,10 +59,12 @@
                 rpen = cls('pinPen', pinLayer.color, 2)
             case 'labelPen':
                 rpen = cls('labelPen', labelLayer.color, 1)
             case 'textPen':
                 rpen = cls('textPen', textLayer.color, 1)
             case 'draftPen':
                 rpen = cls('draftPen', draftLayer.color, 2, Qt.DashLine)
+            case 'hilightPen':
+                rpen = cls('hilightPen', QColorConstants.DarkMagenta, 5, Qt.SolidLine)
             case other:
                 rpen = cls('otherPen', QColor('darkGray'), 2, Qt.DotLine)
         return rpen
```

### Comparing `revolution-eda-0.5.1/revedaEditor/common/shape.py` & `revolution-eda-0.5.2/revedaEditor/common/shape.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,1727 +1,1699 @@
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
-import math
-
-# shape class definition for symbol editor.
-# base class for all shapes: rectangle, circle, line
-from PySide6.QtCore import QPoint, QRect, QRectF, Qt, QLine, QLineF
-from PySide6.QtGui import (QPen, QFont, QFontMetrics, QPainterPath, QTextOption,
-                           QFontDatabase, )
-from PySide6.QtWidgets import (QGraphicsItem, QGraphicsSceneMouseEvent, )
-from quantiphy import Quantity
-import revedaEditor.common.net as net
-import revedaEditor.backend.dataDefinitions as ddef
-import pdk.callbacks as cb
-
-
-class shape(QGraphicsItem):
-    def __init__(self, pen: QPen, gridTuple: tuple) -> None:
-        super().__init__()
-        self.setFlag(QGraphicsItem.ItemIsMovable, True)
-        self.setFlag(QGraphicsItem.ItemIsSelectable, True)
-        self.setFlag(QGraphicsItem.ItemSendsGeometryChanges, True)
-        self.setFlag(QGraphicsItem.ItemIsFocusable, True)
-        self.setAcceptHoverEvents(True)
-        # self.setZValue(self.layer.z)
-        self._pen = pen
-        self._gridTuple = gridTuple
-        self._angle = 0  # rotation angle
-        self._stretch: bool = False
-
-    def itemChange(self, change, value):
-        if change == QGraphicsItem.ItemPositionChange and self.scene():
-            newPos = value.toPoint()
-            sceneRect = self.scene().sceneRect()
-            viewRect = self.scene().views()[0].viewport().rect()
-            newPos.setX(
-                round(newPos.x() / self._gridTuple[0]) * self._gridTuple[0])
-            newPos.setY(
-                round(newPos.y() / self._gridTuple[1]) * self._gridTuple[1])
-
-            if not sceneRect.contains(newPos):
-                # Keep the item inside the scene rect.
-                if newPos.x() > sceneRect.right():
-                    sceneRect.setRight(newPos.x())
-                    viewRect.setRight(newPos.x())
-                elif newPos.x() < sceneRect.left():
-                    sceneRect.setLeft(newPos.x())
-                    viewRect.setLeft(newPos.x())
-                if newPos.y() > sceneRect.bottom():
-                    sceneRect.setBottom(newPos.y())
-                    viewRect.setBottom(newPos.y())
-                elif newPos.y() < sceneRect.top():
-                    sceneRect.setTop(newPos.y())
-                    viewRect.setTop(newPos.y())
-            return newPos
-        return super().itemChange(change, value)
-
-    @property
-    def angle(self):
-        return self._angle
-
-    @angle.setter
-    def angle(self, value):
-        self._angle = value
-        self.prepareGeometryChange()
-        self.setRotation(value)  # self.update(self.boundingRect())
-
-    @property
-    def pen(self):
-        return self._pen
-
-    @pen.setter
-    def pen(self, value):
-        self._pen = value  # self.update(self.boundingRect())
-
-    @property
-    def gridTuple(self):
-        return self._gridTuple
-
-    @gridTuple.setter
-    def gridTuple(self, value: int):
-        self._gridTuple = value
-
-    @property
-    def stretch(self):
-        return self._stretch
-
-    @stretch.setter
-    def stretch(self, value: bool):
-        self._stretch = value  # self.update(self.boundingRect())
-
-    def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        super().mousePressEvent(event)
-        if self.scene().changeOrigin:
-            self.setFlag(QGraphicsItem.ItemIsMovable, False)
-            self.setFlag(QGraphicsItem.ItemIsSelectable, False)
-        else:
-            self.setFlag(QGraphicsItem.ItemIsMovable, True)
-            self.setFlag(QGraphicsItem.ItemIsSelectable, True)
-
-    def sceneEvent(self, event):
-        """
-        Do not propagate event if shape needs to keep still.
-        """
-
-        if self.scene() and (self.scene().changeOrigin or self.scene().drawMode):
-            return False
-        else:
-            super().sceneEvent(event)
-            return True
-
-    def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        super().mouseMoveEvent(event)
-
-    def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        super().mouseReleaseEvent(event)  # self.setSelected(False)
-
-    def hoverEnterEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        self.setCursor(Qt.ArrowCursor)
-        self.setOpacity(0.75)
-        self.setFocus()
-        super().hoverEnterEvent(event)
-
-    def hoverLeaveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        super().hoverLeaveEvent(event)
-        self.setCursor(Qt.CrossCursor)
-        self.setOpacity(1)
-        self.clearFocus()
-
-    def contextMenuEvent(self, event):
-        self.scene().itemContextMenu.exec_(event.screenPos())
-
-    def snapToBase(self, number, base):
-        """
-        Restrict a number to the multiples of base
-        """
-        return base * int(round(number / base))
-
-    def snapToGrid(self, point: QPoint, gridTuple: tuple[int, int]):
-        """
-        snap point to grid. Divides and multiplies by grid size.
-        """
-        return QPoint(gridTuple[0] * int(round(point.x() / gridTuple[0])),
-                      gridTuple[1] * int(round(point.y() / gridTuple[1])), )
-
-
-class rectangle(shape):
-    """
-    rect: QRect defined by top left corner and bottom right corner. QRect(Point1,Point2)
-    """
-
-    sides = ["Left", "Right", "Top", "Bottom"]
-
-    def __init__(self, start: QPoint, end: QPoint, pen: QPen, grid: tuple, ):
-        super().__init__(pen, grid)
-        self._rect = QRectF(start, end).normalized()
-        self._start = self._rect.topLeft()
-        self._end = self._rect.bottomRight()
-        self._stretchSide = None
-
-    def boundingRect(self):
-        return self._rect.normalized().adjusted(-2, -2, 2, 2)
-
-    def paint(self, painter, option, widget):
-        if self.isSelected():
-            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
-            painter.drawRect(self._rect)
-            if self.stretch:
-                painter.setPen(QPen(Qt.red, 2, Qt.SolidLine))
-                if self._stretchSide == rectangle.sides[0]:
-                    painter.drawLine(self.rect.topLeft(), self.rect.bottomLeft())
-                elif self._stretchSide == rectangle.sides[1]:
-                    painter.drawLine(self.rect.topRight(),
-                                     self.rect.bottomRight())
-                elif self._stretchSide == rectangle.sides[2]:
-                    painter.drawLine(self.rect.topLeft(), self.rect.topRight())
-                elif self._stretchSide == rectangle.sides[3]:
-                    painter.drawLine(self.rect.bottomLeft(),
-                                     self.rect.bottomRight())
-        else:
-            painter.setPen(self._pen)
-            painter.drawRect(self._rect)
-
-    @property
-    def rect(self):
-        return self._rect
-
-    @rect.setter
-    def rect(self, rect: QRect):
-        self.prepareGeometryChange()
-        self._rect = rect
-
-    @property
-    def start(self):
-        return self._start
-
-    @start.setter
-    def start(self, start: QPoint):
-        self.prepareGeometryChange()
-        self._rect = QRectF(start, self.end).normalized()
-        self._start = start
-
-    @property
-    def end(self):
-        return self._end
-
-    @end.setter
-    def end(self, end: QPoint):
-        self.prepareGeometryChange()
-        self._rect = QRectF(self.start, end).normalized()
-        self._end = end
-
-    @property
-    def centre(self):
-        return QPoint(int(self._rect.x() + self._rect.width() / 2),
-                      int(self._rect.y() + self._rect.height() / 2), )
-
-    @property
-    def height(self):
-        return self.rect.height()
-
-    @height.setter
-    def height(self, height: int):
-        self.prepareGeometryChange()
-        self._rect.setHeight(height)
-
-    @property
-    def width(self):
-        return self.rect.width()
-
-    @width.setter
-    def width(self, width):
-        self.prepareGeometryChange()
-        self.rect.setWidth(width)
-
-    @property
-    def objName(self):
-        return "RECTANGLE"
-
-    @property
-    def left(self):
-        return self.rect.left()
-
-    @left.setter
-    def left(self, left: int):
-        self.rect.setLeft(left)
-
-    @property
-    def right(self):
-        return self.rect.right()
-
-    @right.setter
-    def right(self, right: int):
-        self.prepareGeometryChange()
-        self.rect.setRight(right)
-
-    @property
-    def top(self):
-        return self.rect.top()
-
-    @top.setter
-    def top(self, top: int):
-        self.prepareGeometryChange()
-        self.rect.setTop(top)
-
-    @property
-    def bottom(self):
-        return self.rect.bottom()
-
-    @bottom.setter
-    def bottom(self, bottom: int):
-        self.prepareGeometryChange()
-        self.rect.setBottom(bottom)
-
-    @property
-    def origin(self):
-        return self.rect.bottomLeft()
-
-    @property
-    def stretchSide(self):
-        return self._stretchSide
-
-    @stretchSide.setter
-    def stretchSide(self, value: str):
-        self.prepareGeometryChange()
-        self._stretchSide = value
-
-    def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        super().mousePressEvent(event)
-        eventPos = event.pos().toPoint()
-        if self._stretch:
-            self.setFlag(QGraphicsItem.ItemIsMovable, False)
-            if eventPos.x() == self.snapToBase(self._rect.left(),
-                                               self.gridTuple[0]):
-                if self._rect.top() <= eventPos.y() <= self._rect.bottom():
-                    self.setCursor(Qt.SizeHorCursor)
-                    self._stretchSide = rectangle.sides[0]
-            elif eventPos.x() == self.snapToBase(self._rect.right(),
-                                                 self.gridTuple[0]):
-                if self._rect.top() <= eventPos.y() <= self._rect.bottom():
-                    self.setCursor(Qt.SizeHorCursor)
-                    self._stretchSide = rectangle.sides[1]
-            elif eventPos.y() == self.snapToBase(self._rect.top(),
-                                                 self.gridTuple[1]):
-                if self._rect.left() <= eventPos.x() <= self._rect.right():
-                    self.setCursor(Qt.SizeVerCursor)
-                    self._stretchSide = rectangle.sides[2]
-            elif eventPos.y() == self.snapToBase(self._rect.bottom(),
-                                                 self.gridTuple[1]):
-                if self._rect.left() <= eventPos.x() <= self._rect.right():
-                    self.setCursor(Qt.SizeVerCursor)
-                    self._stretchSide = rectangle.sides[3]
-
-    def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        eventPos = event.pos().toPoint()
-        if self.stretch:
-            self.prepareGeometryChange()
-            if self.stretchSide == rectangle.sides[0]:
-                self.setCursor(Qt.SizeHorCursor)
-                self.rect.setLeft(eventPos.x())
-            elif self.stretchSide == rectangle.sides[1]:
-                self.setCursor(Qt.SizeHorCursor)
-                self.rect.setRight(eventPos.x() - int(self.pen.width() / 2))
-            elif self.stretchSide == rectangle.sides[2]:
-                self.setCursor(Qt.SizeVerCursor)
-                self.rect.setTop(eventPos.y())
-            elif self.stretchSide == rectangle.sides[3]:
-                self.setCursor(Qt.SizeVerCursor)
-                self.rect.setBottom(eventPos.y() - int(self.pen.width() / 2))
-            self.update()
-        else:
-            super().mouseMoveEvent(event)
-
-    def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        self.setFlag(QGraphicsItem.ItemIsMovable, True)
-        super().mouseReleaseEvent(event)
-        # self.start = self.rect.topLeft()
-        # self.end = self.rect.bottomRight()
-        if self.stretch:
-            self._stretch = False
-            self._stretchSide = None
-            self.setCursor(Qt.ArrowCursor)
-
-
-class circle(shape):
-    def __init__(self, centre: QPoint, end: QPoint, pen: QPen, gridTuple: tuple):
-        super().__init__(pen, gridTuple)
-        xlen = abs(end.x() - centre.x())
-        ylen = abs(end.y() - centre.y())
-        self._radius = self.snapToBase(int(math.sqrt(xlen ** 2 + ylen ** 2)),
-                                       self.gridTuple[0])
-        self._centre = centre
-        self._topLeft = self._centre - QPoint(self._radius, self._radius)
-        self._rightBottom = self._centre + QPoint(self._radius, self._radius)
-        self._end = self._centre + QPoint(self._radius, 0)  # along x-axis
-        self._stretch = False
-        self._startStretch = False
-
-    def paint(self, painter, option, widget) -> None:
-        if self.isSelected():
-            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
-            painter.drawEllipse(self._centre, 1, 1)
-            if self._stretch:
-                painter.setPen(QPen(Qt.red, 2, Qt.SolidLine))
-        else:
-            painter.setPen(self._pen)
-        painter.drawEllipse(self._centre, self._radius, self._radius)
-
-    @property
-    def centre(self):
-        return self._centre
-
-    @centre.setter
-    def centre(self, centre: QPoint):
-        self.prepareGeometryChange()
-        self._centre = self.snapToGrid(centre, self._gridTuple)
-        # self.topLeft = self._centre - QPoint(self._radius, self._radius)
-        # self.rightBottom = self._centre + QPoint(self._radius, self._radius)
-        self._end = self._centre + QPoint(self._radius, 0)
-
-    @property
-    def radius(self):
-        return self._radius
-
-    @radius.setter
-    def radius(self, radius: int):
-        self.prepareGeometryChange()
-        self._radius = self.snapToBase(radius, self._gridTuple[0])
-        self._end = self._centre + QPoint(self._radius, 0)
-        self._topLeft = self._centre - QPoint(self._radius, self._radius)
-        self._rightBottom = self._centre + QPoint(self._radius, self._radius)
-
-    @property
-    def centre(self):
-        return self._centre
-
-    @centre.setter
-    def centre(self, value: QPoint):
-        self.prepareGeometryChange()
-        if isinstance(value, QPoint):
-            self._centre = value
-
-    @property
-    def end(self):
-        return self._end
-
-    @end.setter
-    def end(self, value: QPoint):
-        if isinstance(value, QPoint):
-            self.prepareGeometryChange()
-            self._end = value
-
-    @property
-    def rightBottom(self):
-        return self._rightBottom
-
-    @rightBottom.setter
-    def rightBottom(self, value: QPoint):
-        if isinstance(value, QPoint):
-            self._rightBottom = value
-
-    @property
-    def topLeft(self):
-        return self._topLeft
-
-    @topLeft.setter
-    def topLeft(self, value: QPoint):
-        if isinstance(value, QPoint):
-            self._topLeft = value
-
-    @property
-    def objName(self):
-        return "CIRCLE"
-
-    def boundingRect(self):
-        return (
-            QRectF(self._topLeft, self._rightBottom).normalized().adjusted(-2, -2,
-                                                                           2, 2))
-
-    def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        super().mousePressEvent(event)
-        if self.isSelected() and self._stretch:
-            self.setFlag(QGraphicsItem.ItemIsMovable, False)
-            # eventPos = self.snap2grid(event.pos(), self._gridTuple)
-            eventPos = event.pos().toPoint()
-            distance = self.snapToBase(math.sqrt(
-                (eventPos.x() - self._centre.x()) ** 2 + (
-                        eventPos.y() - self._centre.y()) ** 2),
-                                       self._gridTuple[0], )
-            if distance == self._radius:
-                self._startStretch = True
-                self.setCursor(Qt.DragMoveCursor)
-
-    def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        super().mouseMoveEvent(event)
-        if self._startStretch:
-            eventPos = event.pos().toPoint()
-            distance = self.snapToBase(math.sqrt(
-                (eventPos.x() - self._centre.x()) ** 2 + (
-                        eventPos.y() - self._centre.y()) ** 2),
-                                       self._gridTuple[0], )
-            self.prepareGeometryChange()
-            self._radius = distance
-
-    def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        super().mouseReleaseEvent(event)
-        if self._startStretch:
-            self._startStretch = False
-            self.setFlag(QGraphicsItem.ItemIsMovable, True)
-            self.setFlag(QGraphicsItem.ItemIsSelectable, True)
-            self._topLeft = self._centre - QPoint(self._radius, self._radius)
-            self._rightBottom = self._centre + QPoint(self._radius, self._radius)
-            self._end = self._centre + QPoint(self._radius, 0)
-            self.setCursor(Qt.ArrowCursor)
-
-
-class arc(shape):
-    """
-    Class to draw arc shapes. Can have four directions.
-    """
-
-    arcTypes = ["Up", "Right", "Down", "Left"]
-    sides = ["Left", "Right", "Top", "Bottom"]
-
-    def __init__(self, start: QPoint, end: QPoint, pen: QPen, gridTuple: tuple):
-        super().__init__(pen, gridTuple)
-        self._start = start
-        self._end = end
-        self._rect = QRectF(self._start, self._end).normalized()
-        self._arcLine = QLineF(self._start, self._end)
-        self._arcAngle = 0
-        self._width = self._rect.width()
-        self._height = self._rect.height()
-        self._adjustment = int(self.pen.width() / 2)
-        self._stretchSide = None
-        self.findAngle()
-
-    def findAngle(self):
-        self._arcAngle = self._arcLine.angle()
-        if 90 >= self._arcAngle >= 0:
-            self._arcType = arc.arcTypes[0]
-        elif 180 >= self._arcAngle > 90:
-            self._arcType = arc.arcTypes[1]
-        elif 270 >= self._arcAngle > 180:
-            self._arcType = arc.arcTypes[2]
-        elif 360 > self._arcAngle > 270:
-            self._arcType = arc.arcTypes[3]
-
-    def paint(self, painter, option, widget) -> None:
-        if self.isSelected():
-            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
-            painter.drawRect(self.rect)
-            self.arcDraw(painter)
-            if self._stretch:
-                painter.setPen(QPen(Qt.red, 2, Qt.SolidLine))
-                self.arcDraw(painter)
-                if self._stretchSide == arc.sides[0]:
-                    painter.drawLine(self._rect.topLeft(),
-                                     self._rect.bottomLeft())
-                elif self._stretchSide == arc.sides[1]:
-                    painter.drawLine(self._rect.topRight(),
-                                     self._rect.bottomRight())
-                elif self._stretchSide == arc.sides[2]:
-                    painter.drawLine(self._rect.topLeft(), self._rect.topRight())
-                elif self._stretchSide == arc.sides[3]:
-                    painter.drawLine(self._rect.bottomLeft(),
-                                     self._rect.bottomRight())
-        else:
-            painter.setPen(self._pen)
-            self.arcDraw(painter)
-
-    def arcDraw(self, painter):
-        if self._arcType == arc.arcTypes[0]:
-            painter.drawArc(self._rect, 0, 180 * 16)
-        elif self._arcType == arc.arcTypes[1]:
-            painter.drawArc(self._rect, 90 * 16, 180 * 16)
-        elif self._arcType == arc.arcTypes[2]:
-            painter.drawArc(self._rect, 180 * 16, 180 * 16)
-        elif self._arcType == arc.arcTypes[3]:
-            painter.drawArc(self._rect, 270 * 16, 180 * 16)
-
-    def boundingRect(self):
-        return self._rect.adjusted(-2, -2, 2, 2)
-
-    @property
-    def objName(self):
-        return "ARC"
-
-    @property
-    def rect(self):
-        return self._rect
-
-    @rect.setter
-    def rect(self, arc_rect: QRect):
-        assert isinstance(arc_rect, QRect)
-        self._rect = arc_rect.normalized()
-
-    @property
-    def start(self):
-        return self._start
-
-    @start.setter
-    def start(self, point: QPoint):
-        assert isinstance(point, QPoint)
-        self.prepareGeometryChange()
-        self._start = self.snapToGrid(point, self.gridTuple)
-
-    @property
-    def end(self):
-        return self._end
-
-    @end.setter
-    def end(self, point: QPoint):
-        assert isinstance(point, QPoint)
-        self.prepareGeometryChange()
-        self._end = point
-        self._arcLine = QLineF(self._start, self._end)
-        self._arcAngle = self._arcLine.angle()
-        self.findAngle()
-        self._rect = QRectF(self._start, self._end).normalized()
-
-    @property
-    def width(self):
-        return self._width
-
-    @width.setter
-    def width(self, width):
-        self._width = width
-        self.prepareGeometryChange()
-        self.rect.setWidth(self._width)
-
-    @property
-    def height(self):
-        return self._height
-
-    @height.setter
-    def height(self, height):
-        self._height = height
-        self.prepareGeometryChange()
-        self.rect.setHeight(self._height)
-
-    def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        super().mousePressEvent(event)
-        eventPos = event.pos().toPoint()
-        if self._stretch:
-            self.setFlag(QGraphicsItem.ItemIsMovable, False)
-            if eventPos.x() == self.snapToBase(self._rect.left(),
-                                               self.gridTuple[0]):
-                if self._rect.top() <= eventPos.y() <= self._rect.bottom():
-                    self.setCursor(Qt.SizeHorCursor)
-                    self._stretchSide = arc.sides[0]
-            elif eventPos.x() == self.snapToBase(self._rect.right(),
-                                                 self.gridTuple[0]):
-                if self._rect.top() <= eventPos.y() <= self._rect.bottom():
-                    self.setCursor(Qt.SizeHorCursor)
-                    self._stretchSide = arc.sides[1]
-            elif eventPos.y() == self.snapToBase(self._rect.top(),
-                                                 self.gridTuple[1]):
-                if self._rect.left() <= eventPos.x() <= self._rect.right():
-                    self.setCursor(Qt.SizeVerCursor)
-                    self._stretchSide = arc.sides[2]
-            elif eventPos.y() == self.snapToBase(self._rect.bottom(),
-                                                 self.gridTuple[1]):
-                if self._rect.left() <= eventPos.x() <= self._rect.right():
-                    self.setCursor(Qt.SizeVerCursor)
-                    self._stretchSide = arc.sides[3]
-
-    def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        super().mouseMoveEvent(event)
-
-        eventPos = event.pos().toPoint()
-        if self._stretch:
-            self.prepareGeometryChange()
-            if self._stretchSide == arc.sides[0]:
-                self.setCursor(Qt.SizeHorCursor)
-                self._rect.setLeft(eventPos.x())
-            elif self._stretchSide == arc.sides[1]:
-                self.setCursor(Qt.SizeHorCursor)
-                self._rect.setRight(eventPos.x() - self._adjustment)
-            elif self._stretchSide == arc.sides[2]:
-                self.setCursor(Qt.SizeVerCursor)
-                self._rect.setTop(eventPos.y())
-            elif self._stretchSide == arc.sides[3]:
-                self.setCursor(Qt.SizeVerCursor)
-                self._rect.setBottom(eventPos.y() - self._adjustment)
-            self.update()
-
-    def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        self.setFlag(QGraphicsItem.ItemIsMovable, True)
-        super().mouseReleaseEvent(event)
-        if self.stretch:
-            self._stretch = False
-            self._stretchSide = None
-            self.setCursor(Qt.ArrowCursor)
-
-            if self._arcType == arc.arcTypes[0]:
-                self._start = self.snapToGrid(self._rect.bottomLeft(),
-                                              self.gridTuple)
-                self._end = self.snapToGrid(self._rect.topRight(), self.gridTuple)
-            elif self._arcType == arc.arcTypes[1]:
-                self._start = self.snapToGrid(self._rect.topLeft(),
-                                              self.gridTuple)
-                self._end = self.snapToGrid(self._rect.bottomRight(),
-                                            self.gridTuple)
-            elif self._arcType == arc.arcTypes[2]:
-                self._start = self.snapToGrid(self._rect.topRight(),
-                                              self.gridTuple)
-                self._end = self.snapToGrid(self._rect.bottomLeft(),
-                                            self.gridTuple)
-            elif self._arcType == arc.arcTypes[3]:
-                self._start = self.snapToGrid(self._rect.bottomRight(),
-                                              self.gridTuple)
-                self._end = self.snapToGrid(self._rect.topLeft(), self.gridTuple)
-            self._rect = QRectF(self._start, self._end).normalized()
-
-
-class line(shape):
-    """
-    line class definition for symbol drawing.
-    """
-
-    stretchSides = ["start", "end"]
-
-    def __init__(self, start: QPoint, end: QPoint, pen: QPen, grid: tuple, ):
-        super().__init__(pen, grid)
-        self._end = end
-        self._start = start
-        self._pen = pen
-        self._stretch = False
-        self._stretchSide = None
-        self._line = QLine(self._start, self._end)
-        self._rect = QRect(self._start, self._end).normalized()
-        self._horizontal = True  # True if line is horizontal, False if vertical
-
-    def boundingRect(self):
-        return self._rect.adjusted(-2, -2, 2, 2)
-
-    def shape(self):
-        path = QPainterPath()
-        path.addRect(self._rect.adjusted(-2, -2, 2, 2))
-        return path
-
-    def shape(self):
-        path = QPainterPath()
-        path.addRect(self._rect.adjusted(-2, -2, 2, 2))
-        return path
-
-    def paint(self, painter, option, widget):
-        if self.isSelected():
-            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
-            if self._stretch:
-                painter.setPen(QPen(Qt.red, 2, Qt.SolidLine))
-                if self._stretchSide == line.stretchSides[0]:
-                    painter.drawEllipse(self._start, self.gridTuple[0],
-                                        self.gridTuple[1])
-                elif self._stretchSide == line.stretchSides[1]:
-                    painter.drawEllipse(self._end, self.gridTuple[0],
-                                        self.gridTuple[1])
-        else:
-            painter.setPen(self._pen)
-        painter.drawLine(self._line)
-
-    def objName(self):
-        return "LINE"
-
-    @property
-    def rect(self):
-        return self._rect
-
-    @rect.setter
-    def rect(self, rect: QRect):
-        self._rect = rect
-
-    @property
-    def start(self):
-        return self._start
-
-    @start.setter
-    def start(self, start: QPoint):
-        self.prepareGeometryChange()
-        self._start = start
-        self._line = QLine(self._start, self._end)
-        self._rect = QRect(self._start, self._end).normalized()
-
-    @property
-    def end(self):
-        return self._end
-
-    @end.setter
-    def end(self, end: QPoint):
-        self.prepareGeometryChange()
-        self._end = end
-        self._line = QLine(self._start, self._end)
-        self._rect = QRect(self._start, self._end).normalized()
-
-    @property
-    def pen(self):
-        return self._pen
-
-    @pen.setter
-    def pen(self, pen: QPen):
-        self._pen = pen
-
-    @property
-    def width(self):
-        return self._pen.width()
-
-    @width.setter
-    def width(self, width: int):
-        self._pen.setWidth(width)
-
-    def bBox(self) -> QRect:
-        return self.boundingRect()
-
-    def Move(self, offset: QPoint):
-        self.start += offset
-        self._end += offset
-
-    @property
-    def length(self):
-        return math.sqrt((self.start.x() - self._end.x()) ** 2 + (
-                    self.start.y() - self._end.y()) ** 2)
-
-    def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        super().mousePressEvent(event)
-        if self.isSelected() and self._stretch:
-            self.setFlag(QGraphicsItem.ItemIsMovable, False)
-            eventPos = event.pos().toPoint()
-            if eventPos == self.start:
-                self._stretchSide = line.stretchSides[0]
-            elif eventPos == self._end:
-                self._stretchSide = line.stretchSides[1]
-
-    def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        eventPos = event.pos().toPoint()
-        if self._stretchSide == line.stretchSides[0]:
-            self.prepareGeometryChange()
-            self.start = eventPos
-            self._line = QLine(self.start, self._end)
-            self._rect = QRect(self.start, self._end).normalized()
-        elif self._stretchSide == line.stretchSides[1]:
-            self.prepareGeometryChange()
-            self._end = eventPos
-            self._line = QLine(self.start, self._end)
-            self._rect = QRect(self.start, self._end).normalized()
-
-        super().mouseMoveEvent(event)
-
-    def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        super().mouseReleaseEvent(event)
-        self._stretch = False
-        self.setFlag(QGraphicsItem.ItemIsMovable, True)
-        self.setFlag(QGraphicsItem.ItemIsSelectable, True)
-        self._stretchSide = ""
-
-
-class pin(shape):
-    """
-    symbol pin class definition for symbol drawing.
-    """
-
-    pinDirs = ["Input", "Output", "Inout"]
-    pinTypes = ["Signal", "Ground", "Power", "Clock", "Digital", "Analog"]
-
-    def __init__(self, start: QPoint, pen: QPen, pinName: str = "",
-                 pinDir: str = pinDirs[0], pinType: str = pinTypes[0],
-                 grid: tuple = (10, 10), ):
-        super().__init__(pen, grid)
-
-        self._start = start  # centre of pin
-        self._pinName = pinName
-        self._pinDir = pinDir
-        self._pinType = pinType
-        self._connected = False  # True if the pin is connected to a net.
-        self._rect = QRect(self._start.x() - 5, self._start.y() - 5, 10, 10)
-
-    def __repr__(self):
-        return f"pin: {self._pinName} {self.mapToScene(self._start)}"
-
-    def boundingRect(self):
-        return self._rect  #
-
-    def paint(self, painter, option, widget):
-        painter.setPen(self._pen)
-        painter.setBrush(self._pen.color())
-        painter.drawRect(self._rect)
-        painter.setFont(QFont("Arial", 12))
-        painter.drawText(QPoint(self._start.x() - 5, self._start.y() - 10),
-                         self._pinName)
-        if self.isSelected():
-            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
-            painter.setBrush(Qt.yellow)
-            painter.drawRect(self._rect)
-
-    def objName(self):
-        return "PIN"
-
-    @property
-    def start(self):
-        return self._start
-
-    @start.setter
-    def start(self, start):
-        self._start = start
-
-    @property
-    def pinName(self):
-        return self._pinName
-
-    @pinName.setter
-    def pinName(self, pinName):
-        if pinName != "":
-            self._pinName = pinName
-
-    @property
-    def pinDir(self):
-        return self._pinDir
-
-    @pinDir.setter
-    def pinDir(self, direction: str):
-        if direction in self.pinDirections:
-            self._pinDir = direction
-
-    @property
-    def pinType(self):
-        return self._pinType
-
-    @pinType.setter
-    def pinType(self, pintype: str):
-        if pintype in self.pinTypes:
-            self._pinType = pintype
-
-    @property
-    def connected(self):
-        return self._connected
-
-    @connected.setter
-    def connected(self, value: bool):
-        if isinstance(value, bool):
-            self._connected = value
-
-    def toSchematicPin(self, start: QPoint, pen: QPen, gridTuple):
-        return schematicPin(start, pen, self.pinName, self.pinDir, self.pinType,
-                            gridTuple)
-
-
-class text(shape):
-    """
-    This class is for text annotations on symbol or schematics.
-    """
-
-    textAlignments = ["Left", "Center", "Right"]
-    textOrients = ["R0", "R90", "R180", "R270"]
-
-    def __init__(self, start: QPoint, pen: QPen, textContent: str = "",
-                 grid: tuple = (10, 10), fontFamily="Helvetica",
-                 fontStyle="Regular", textHeight: str = "12",
-                 textAlign: str = "Left", textOrient: str = "R0", ):
-        super().__init__(pen, grid)
-
-        self._start = start
-        self._pen = pen
-        self._textContent = textContent
-        self._textHeight = textHeight
-        self._textAlign = textAlign
-        self._textOrient = textOrient
-        self._textFont = QFont(fontFamily)
-        self._textFont.setStyleName(fontStyle)
-        self._textFont.setPointSize(int(float(self._textHeight)))
-        self._textFont.setKerning(True)
-        self.setOpacity(1)
-        self._fm = QFontMetrics(self._textFont)
-        self._textOptions = QTextOption()
-        if self._textAlign == text.textAlignments[0]:
-            self._textOptions.setAlignment(Qt.AlignmentFlag.AlignLeft)
-        elif self._textAlign == text.textAlignments[1]:
-            self._textOptions.setAlignment(Qt.AlignmentFlag.AlignCenter)
-        elif self._textAlign == text.textAlignments[2]:
-            self._textOptions.setAlignment(Qt.AlignmentFlag.AlignRight)
-
-    def boundingRect(self):
-        if self._textAlign == text.textAlignments[0]:
-            self._rect = self._fm.boundingRect(QRect(0, 0, 400, 400),
-                                               Qt.AlignmentFlag.AlignLeft,
-                                               self._textContent)
-        elif self._textAlign == text.textAlignments[1]:
-            self._rect = self._fm.boundingRect(QRect(0, 0, 400, 400),
-                                               Qt.AlignmentFlag.AlignCenter,
-                                               self._textContent)
-        elif self._textAlign == text.textAlignments[2]:
-            self._rect = self._fm.boundingRect(QRect(0, 0, 400, 400),
-                                               Qt.AlignmentFlag.AlignRight,
-                                               self._textContent)
-        return QRect(self._start.x(), self._start.y() - self._rect.height(),
-                     self._rect.width(), self._rect.height(), )
-
-    def paint(self, painter, option, widget):
-        painter.setFont(self._textFont)
-        if self.isSelected():
-            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
-            painter.drawRect(self.boundingRect())
-        else:
-            painter.setPen(self._pen)
-        painter.drawText(self.boundingRect(), self._textContent,
-                         o=self._textOptions)
-
-    @property
-    def start(self):
-        return self._start
-
-    @start.setter
-    def start(self, value: QPoint):
-        self._start = value
-
-    @property
-    def textContent(self):
-        return self._textContent
-
-    @textContent.setter
-    def textContent(self, inputText: str):
-        if isinstance(inputText, str):
-            self._textContent = inputText
-        else:
-            self.scene().logger.error(f"Not a string: {inputText}")
-
-    @property
-    def fontFamily(self) -> str:
-        return self._textFont.family()
-
-    @fontFamily.setter
-    def fontFamily(self, familyName):
-        fontFamilies = QFontDatabase.families(QFontDatabase.Latin)
-        fixedFamilies = [family for family in fontFamilies if
-                         QFontDatabase.isFixedPitch(family)]
-        if familyName in fixedFamilies:
-            self._textFont.setFamily(familyName)
-        else:
-            self.scene().logger.error(f"Not a valid font name: {familyName}")
-
-    @property
-    def fontStyle(self) -> str:
-        return self._textFont.styleName()
-
-    @fontStyle.setter
-    def fontStyle(self, value: str):
-        if value in QFontDatabase.styles(self._textFont.family()):
-            self._textFont.setStyleName(value)
-        else:
-            self.scene().logger.error(f"Not a valid font style: {value}")
-
-    @property
-    def textHeight(self) -> int:
-        return self._textHeight
-
-    @textHeight.setter
-    def textHeight(self, value: int):
-        fontSizes = [str(size) for size in
-                     QFontDatabase.pointSizes(self._textFont.family(),
-                                              self._textFont.styleName())]
-        if value in fontSizes:
-            self._textHeight = value
-        else:
-            self.scene().logger.error(f"Not a valid font height: {value}")
-            self.scene().logger.warning(f"Valid font heights are: {fontSizes}")
-
-    @property
-    def textFont(self) -> QFont:
-        return self._textFont
-
-    @textFont.setter
-    def textFont(self, value: QFont):
-        assert isinstance(value, QFont)
-        self._textFont = value
-
-    @property
-    def textAlignment(self):
-        return self._textAlign
-
-    @textAlignment.setter
-    def textAlignment(self, value):
-        if value in text.textAlignments:
-            self._textAlign = value
-        else:
-            self.scene().logger.error(
-                f"Not a valid text alignment value: {value}")
-
-    @property
-    def textOrient(self):
-        return self._textOrient
-
-    @textOrient.setter
-    def textOrient(self, value):
-        if value in text.textOrients:
-            self._textOrient = value
-        else:
-            self.scene().logger.error(f"Not a valid text orientation: {value}")
-
-
-class label(shape):
-    """
-    label: text class definition for symbol drawing.
-    labelText is what is shown on the symbol in a schematic
-    """
-
-    labelAlignments = ["Left", "Center", "Right"]
-    labelOrients = ["R0", "R90", "R180", "R270", "MX", "MX90", "MY", "MY90"]
-    labelUses = ["Normal", "Instance", "Pin", "Device", "Annotation"]
-    labelTypes = ["Normal", "NLPLabel", "PyLabel"]
-    predefinedLabels = ["[@libName]", "[@cellName]", "[@viewName]", "[@instName]",
-                        "[@modelName]", "[@elementNum]"]
-
-    def __init__(self, start: QPoint, pen: QPen, labelDefinition: str = "",
-                 grid: tuple = (10, 10), labelType: str = "Normal",
-                 labelHeight: str = "12", labelAlign: str = "Left",
-                 labelOrient: str = "R0", labelUse: str = "Normal", ):
-        super().__init__(pen, grid)
-        self._start = start  # top left corner
-        self._pen = pen
-        self._labelDefinition = labelDefinition  # label definition is what is
-        # entered in the symbol editor
-        self._labelName = None  # label Name
-        self._labelValue = None  # label value
-        self._labelText = None  # Displayed label
-        self._labelHeight = labelHeight
-        self._labelAlign = labelAlign
-        self._labelOrient = labelOrient
-        self._labelUse = labelUse
-        self._labelType = labelType
-        self._labelFont = QFont("Arial")
-        self._labelFont.setPointSize(int(float(self._labelHeight)))
-        self._labelFont.setKerning(False)
-        self._labelVisible: bool = False
-        self._labelValueSet: bool = False
-        # labels are visible by default
-        self.setOpacity(1)
-        self._fm = QFontMetrics(self._labelFont)
-        self._rect = self._fm.boundingRect(self._labelDefinition)
-
-    def __repr__(self):
-        return f"label: {self._labelText} for {self._labelDefinition} at {self._start}, " \
-               f"value =  {self._labelValue}"
-
-    def boundingRect(self):
-        return QRect(self._start.x(), self._start.y(), self._rect.width(),
-                     self._rect.height()).normalized().adjusted(0, 0, 0,5)  #
-
-    def shape(self) -> QPainterPath:
-        path = QPainterPath()
-        path.addRect(self.boundingRect())
-        return path
-
-    def paint(self, painter, option, widget):
-        # self._rect = self.fm.boundingRect(self.labelName)
-        self._labelFont.setPointSize(int(self._labelHeight))
-        painter.setFont(self._labelFont)
-        if self.isSelected():
-            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
-            painter.drawRect(self.boundingRect())
-        else:
-            painter.setPen(self._pen)
-        if self._labelText:
-            painter.drawText(
-                QPoint(self._start.x(), self._start.y() + self._rect.height()),
-                self._labelText, )
-        else:
-            painter.drawText(
-                QPoint(self._start.x(), self._start.y() + self._rect.height()),
-                self._labelDefinition, )
-        self._fm = QFontMetrics(self._labelFont)
-        self._rect = self._fm.boundingRect(self._labelDefinition)
-
-    @property
-    def start(self):
-        return self._start
-
-    @start.setter
-    def start(self, value: QPoint):
-        self._start = value
-
-    @property
-    def left(self):
-        return self._start.x()
-
-    @property
-    def right(self):
-        return self._start.x() + self.boundingRect().width()
-
-    @property
-    def top(self):
-        return self._start.y()
-
-    @property
-    def bottom(self):
-        return self._start.y() + self.boundingRect().height()
-
-    @property
-    def width(self):
-        return self.boundingRect().width()
-
-    @property
-    def height(self):
-        return self.boundingRect().height()
-
-    @property
-    def labelName(self):
-        return self._labelName
-
-    @labelName.setter
-    def labelName(self, labelName: str):
-        self._labelName = labelName
-
-    @property
-    def labelDefinition(self):
-        return self._labelDefinition
-
-    @labelDefinition.setter
-    def labelDefinition(self, labelDefinition: str):
-        if isinstance(labelDefinition, str):
-            self._labelDefinition = labelDefinition.strip()
-
-    @property
-    def labelValue(self):
-        return self._labelValue
-
-    @labelValue.setter
-    def labelValue(self, labelValue):
-        self._labelValue = labelValue
-        self._labelValueSet = True
-        # self.labelDefs()
-
-    @property
-    def labelValueSet(self) -> bool:
-        return self._labelValueSet
-
-    @labelValueSet.setter
-    def labelValueSet(self, value: bool):
-        if isinstance(value, bool):
-            self._labelValueSet = value
-
-    @property
-    def labelHeight(self):
-        return self._labelHeight
-
-    @labelHeight.setter
-    def labelHeight(self, value: int):
-        self._labelHeight = value
-
-    @property
-    def labelText(self):
-        return self._labelText
-
-    @labelText.setter
-    def labelText(self, labelText):
-        self._labelText = labelText
-        self._rect = self._fm.boundingRect(self._labelText).normalized().adjusted(0, 0, 0, 5)
-
-    def objName(self):
-        return "LABEL"
-
-    @property
-    def labelType(self):
-        return self._labelType
-
-    @labelType.setter
-    def labelType(self, labelType):
-        if labelType in self.labelTypes:
-            self._labelType = labelType
-        elif self.scene():
-            self.scene().logger.error("Invalid label type")
-
-    @property
-    def labelAlign(self):
-        return self._labelAlign
-
-    @labelAlign.setter
-    def labelAlign(self, labelAlignment):
-        if labelAlignment in self.labelAlignments:
-            self._labelAlign = labelAlignment
-        elif self.scene():
-            self.scene().logger.error("Invalid label alignment")
-
-    @property
-    def labelOrient(self):
-        return self._labelOrient
-
-    @labelOrient.setter
-    def labelOrient(self, labelOrient):
-        if labelOrient in self.labelOrients:
-            self._labelOrient = labelOrient
-        else:
-            print("Invalid label orientation")
-
-    @property
-    def labelUse(self):
-        return self._labelUse
-
-    @labelUse.setter
-    def labelUse(self, labelUse):
-        if labelUse in self.labelUses:
-            self._labelUse = labelUse
-        elif self.scene():
-            self.scene().logger.error("Invalid label use")
-
-    @property
-    def labelFont(self):
-        return self._labelFont
-
-    @labelFont.setter
-    def labelFont(self, labelFont: QFont):
-        self._labelFont = labelFont
-
-    @property
-    def labelVisible(self) -> bool:
-        return self._labelVisible
-
-    @labelVisible.setter
-    def labelVisible(self, value: bool):
-        assert isinstance(value, bool)
-        if value:
-            self.setOpacity(1)
-            self._labelVisible = True
-        else:
-            self.setOpacity(0.001)
-            self._labelVisible = False
-
-    def moveBy(self, delta: QPoint):
-        self._start += delta
-
-    def labelDefs(self):
-        """
-        This method will create label name, value andtext from label
-        definition. It should be run label is defined or redefined.
-        """
-        self.prepareGeometryChange()
-        if self._labelType == label.labelTypes[0]:
-            self._labelName = self._labelDefinition
-            self._labelText = self._labelDefinition
-            self._labelValue = None
-            self._labelValueSet = True
-        elif self.labelType == label.labelTypes[1]:
-            try:
-                if self._labelDefinition in label.predefinedLabels:
-                    self._labelValueSet = True
-                    match self.labelDefinition:
-                        case "[@cellName]":
-                            self._labelName = "cellName"
-                            self._labelValue = self.parentItem().cellName
-                            self._labelText = self._labelValue
-                        case "[@instName]":
-                            self._labelName = "instName"
-                            self._labelValue = f"I{self.parentItem().counter}"
-                            self._labelText = self._labelValue
-                        case "[@libName]":
-                            self._labelName = "libName"
-                            self._labelValue = self.parentItem().libraryName
-                            self._labelText = self._labelValue
-                        case "[@viewName]":
-                            self._viewName = "viewName"
-                            self._labelValue = self.parentItem().viewName
-                            self._labelText = self._labelValue
-                        case "[@modelName]":
-                            self._labelName = "modelName"
-                            self._labelValue = self.parentItem().attr.get(
-                                "modelName", "")
-                            self._labelText = self._labelValue
-                        case "[@elementNum]":
-                            self._labelName = "elementNum"
-                            self._labelValue = f"{self.parentItem().counter}"
-                            self._labelText = self._labelValue
-                else:
-                    labelFields = (
-                        self._labelDefinition.lstrip("[@").rstrip("]").rstrip(
-                            ":").split(":"))
-                    self._labelName = labelFields[0].strip()
-                    match len(labelFields):
-                        case 1:
-                            if not self._labelValueSet:
-                                self._labelValue = "?"
-                            self._labelText = self._labelValue
-                        case 2:
-                            if self._labelValueSet:
-                                self._labelText = (
-                                    labelFields[1].strip().replace("%",
-                                                                   self._labelValue))
-                            else:
-                                self._labelValue = "?"
-                        case 3:
-                            tempLabelValue = (
-                                labelFields[2].strip().split("=")[-1].split()[-1])
-                            if self.labelValueSet:
-                                self._labelText = labelFields[2].replace(
-                                    tempLabelValue, self._labelValue)
-                            else:
-                                self._labelText = labelFields[2]
-                                self._labelValue = tempLabelValue
-
-            except Exception as e:
-                if self.scene():
-                    self.scene().logger.error(e)
-        elif self._labelType == label.labelTypes[2]:  # pyLabel
-            try:
-                labelFields = self._labelDefinition.strip().split("=")
-                self._labelName = labelFields[0].strip()
-                labelFunction = labelFields[1].strip()
-                # pass the PDK callback class named with "cellName" the labels
-                # dictionary of instance.w
-                expression = (
-                    f"cb.{self.parentItem().cellName}(self.parentItem().labels).{labelFunction}")
-                self._labelValue = Quantity(eval(expression)).render(prec=3)
-                self._labelText = f"{self._labelName}={self._labelValue}"
-            except Exception as e:
-                if self.scene():
-                    self.scene().logger.error(e)
-
-
-class symbolShape(shape):
-    def __init__(self, pen: QPen, gridTuple: tuple, shapes: list, attr: dict):
-        super().__init__(pen, gridTuple)
-        assert shapes is not None  # must not be an empty list
-        self.shapes = shapes  # list of shapes in the symbol
-        self.attr = attr  # parameters common to all instances of symbol
-        self._counter = 0  # item's number on schematic
-        self._libraryName = ""
-        self._cellName = ""
-        self._viewName = ""
-        self._instanceName = ""
-        self._netlistLine = ""
-        # self._simViewName = None
-        self._angle = 0.0
-        self._drawings = list()
-        self._labels = dict()  # dict of labels
-        self._pins = dict()  # dict of pins
-        self.pinLocations = dict()  # pinName: pinRect
-        self.pinNetMap = dict()  # pinName: netName
-        self.pinNetTupleList = list()  # list of pinNetTuple
-        for item in self.shapes:
-            item.setFlag(QGraphicsItem.ItemIsSelectable, False)
-            item.setFlag(QGraphicsItem.ItemStacksBehindParent, True)
-            item.setParentItem(self)
-            if type(item) is pin:
-                self._pins[item.pinName] = item
-            elif type(item) is label:
-                self._labels[item.labelName] = item
-            else:
-                self._drawings.append(item)
-        self.setFiltersChildEvents(True)
-        self.setHandlesChildEvents(True)
-        self.setFlag(QGraphicsItem.ItemContainsChildrenInShape, True)
-        self.borderRect = self._drawings[0].sceneBoundingRect()
-        if self._drawings[1:]:
-            for draw in self._drawings[1:]:
-                self.borderRect = self.borderRect.united(draw.sceneBoundingRect())
-        self.dashLines = dict()
-
-    def __repr__(self):
-        return (
-            f"symbolShape(name={self.cellName}, scene position= {self.scenePos()}, "
-            f"pins = {self.pins}, labels = {self.labels}, ")
-
-    def paint(self, painter, option, widget):
-        if self.isSelected():
-            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
-            painter.drawRect(self.borderRect)
-
-    def boundingRect(self):
-        return self.childrenBoundingRect()
-
-    def sceneEvent(self, event):
-        try:  # if net is being drawn, do not accept any event.
-            if self.scene().drawWire:
-                return False
-            else:
-                super().sceneEvent(event)
-                return True
-        except AttributeError:
-            return False
-
-    def itemChange(self, change, value):
-
-        if self.scene() and change == QGraphicsItem.ItemPositionHasChanged:
-            # item's position has changed
-            # do something here
-            for item in self.pinNetTupleList:
-                if item.start == 1:
-                    item.net.start = item.pin.mapToScene(item.pin.start)
-                elif item.start == 0:
-                    item.net.end = item.pin.mapToScene(item.pin.start)
-
-        return super().itemChange(change, value)
-
-    def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        self.pinNetTupleList = list()
-        # create a named tuple to record whether the pin is located at the start or at
-        # the end of the net.
-        pins = [item for item in self.pins.values()]
-        for pinItem in pins:
-            for pinNet in self.scene().items(pinItem.sceneBoundingRect().adjusted(
-                    -2, -2, 2, 2), Qt.IntersectsItemShape):
-                if isinstance(pinNet, net.schematicNet):
-                    if pinItem.sceneBoundingRect().adjusted(-2, -2, 2, 2).contains(
-                            pinNet.mapToScene(pinNet.start)):
-                        self.pinNetTupleList.append(ddef.pinNetTuple(pinItem, pinNet, 1))
-                    elif pinItem.sceneBoundingRect().adjusted(-2, -2, 2, 2).contains(
-                            pinNet.mapToScene(pinNet.end)):
-                        self.pinNetTupleList.append(ddef.pinNetTuple(pinItem, pinNet, 0))
-        for item in self.pinNetTupleList:
-            pinSceneLoc = item.pin.mapToScene(item.pin.start)
-            if item.start == 1:
-                item.net.start = pinSceneLoc
-            else:
-                item.net.end = pinSceneLoc
-            item.net.pen = self.scene().otherPen
-        super().mousePressEvent(event)
-
-    def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        super().mouseReleaseEvent(event)
-
-        for item in self.pinNetTupleList:
-            lines = self.scene().addWires(item.net.start, self.scene().wirePen)
-            self.scene().extendWires(lines,item.net.start,item.net.end)
-            self.scene().pruneWires(lines,self.scene().wirePen)
-            self.scene().removeItem(item.net)
-
-
-    @property
-    def libraryName(self):
-        return self._libraryName
-
-    @libraryName.setter
-    def libraryName(self, value):
-        self._libraryName = value
-
-    @property
-    def cellName(self):
-        return self._cellName
-
-    @cellName.setter
-    def cellName(self, value: str):
-        self._cellName = value
-
-    @property
-    def viewName(self):
-        return self._viewName
-
-    @viewName.setter
-    def viewName(self, value: str):
-        self._viewName = value
-
-    @property
-    def instanceName(self):
-        return self._instanceName
-
-    @instanceName.setter
-    def instanceName(self, value: str):
-        '''
-        If instance name is changed and [@instName] label exists, change it too.
-        '''
-        self._instanceName = value
-        if self.labels.get('instanceName', None):
-            self.labels['instanceName'].labelValue = value
-            self.labels['instanceName'].labelValueSet = True
-            self.labels['instanceName'].update()
-
-    @property
-    def counter(self) -> int:
-        return self._counter
-
-    @counter.setter
-    def counter(self, value: int):
-        assert isinstance(value, int)
-        self._counter = value
-
-    @property
-    def angle(self):
-        return self._angle
-
-    @angle.setter
-    def angle(self, value: float):
-        self.setRotation(value)
-        self._angle = value
-
-    @property
-    def labels(self):
-        return self._labels  # dictionary
-
-    @property
-    def pins(self):
-        return self._pins
-
-    @property
-    def drawings(self):
-        return self._drawings
-
-
-class schematicPin(shape):
-    """
-    schematic pin class.
-    """
-
-    pinDirs = ["Input", "Output", "Inout"]
-    pinTypes = ["Signal", "Ground", "Power", "Clock", "Digital", "Analog"]
-
-    def __init__(self, start: QPoint, pen: QPen, pinName, pinDir, pinType,
-                 gridTuple: tuple):
-        super().__init__(pen, gridTuple)
-        self._start = start
-        self._pinName = pinName
-        self._pinDir = pinDir
-        self._pinType = pinType
-        self._netTupleSet = set()
-
-    def __repr__(self):
-        return f"schematicPin({self._start}, {self._pen}, {self._pinName}, {self._pinDir}, {self._pinType})"
-
-    def paint(self, painter, option, widget):
-
-        painter.setPen(self._pen)
-        painter.setBrush(self._pen.color())
-        painter.setFont(QFont("Arial", 12))
-        match self.pinDir:
-            case "Input":
-                painter.drawPolygon(
-                    [QPoint(self._start.x() - 10, self._start.y() - 10),
-                     QPoint(self._start.x() + 10, self._start.y() - 10),
-                     QPoint(self._start.x() + 20, self._start.y()),
-                     QPoint(self._start.x() + 10, self._start.y() + 10),
-                     QPoint(self._start.x() - 10, self._start.y() + 10), ])
-            case "Output":
-                painter.drawPolygon(
-                    [QPoint(self._start.x() - 20, self._start.y()),
-                     QPoint(self._start.x() - 10, self._start.y() - 10),
-                     QPoint(self._start.x() + 10, self._start.y() - 10),
-                     QPoint(self._start.x() + 10, self._start.y() + 10),
-                     QPoint(self._start.x() - 10, self._start.y() + 10), ])
-            case "Inout":
-                painter.drawPolygon(
-                    [QPoint(self._start.x() - 20, self._start.y()),
-                     QPoint(self._start.x() - 10, self._start.y() - 10),
-                     QPoint(self._start.x() + 10, self._start.y() - 10),
-                     QPoint(self._start.x() + 20, self._start.y()),
-                     QPoint(self._start.x() + 10, self._start.y() + 10),
-                     QPoint(self._start.x() - 10, self._start.y() + 10), ])
-        painter.drawText(self._start.x(), self._start.y() - 20, self.pinName)
-        if self.isSelected():
-            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
-            # painter.setBrush(Qt.yellow)
-            painter.drawRect(
-                QRect.span(QPoint(self._start.x() - 10, self._start.y() - 10),
-                           QPoint(self._start.x() + 10, self._start.y() + 10), ))
-
-    def boundingRect(self):
-        return QRect(self._start.x() - 10, self._start.y() - 10, 30, 20).adjusted(
-            -5, -10, 5, 5)
-
-    def sceneEvent(self, event):
-        if self.scene().drawWire:
-            return False
-        else:
-            super().sceneEvent(event)
-            return True
-    #
-    def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        super().mousePressEvent(event)
-        # create a named tuple to record whether the pin is located at the start or at
-        # the end of the net.
-
-        for pinNet in self.scene().items(self.sceneBoundingRect().adjusted(
-                -2, -2, 2, 2), Qt.IntersectsItemShape):
-            if isinstance(pinNet, net.schematicNet):
-                if self.sceneBoundingRect().adjusted(-2, -2, 2, 2).contains(
-                        pinNet.mapToScene(pinNet.start)):
-                    self._netTupleSet.add(ddef.netTuple(pinNet, 1))
-                elif self.sceneBoundingRect().adjusted(-2, -2, 2, 2).contains(
-                        pinNet.mapToScene(pinNet.end)):
-                    self._netTupleSet.addd(ddef.netTuple(pinNet, 0))
-        for item in self._netTupleSet:
-            pinSceneLoc = self.mapToScene(self.start)
-            if item.start == 1:
-                item.net.start = pinSceneLoc
-            else:
-                item.net.end = pinSceneLoc
-            item.net.pen = self.scene().otherPen
-        super().mousePressEvent(event)
-    #
-    def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-        super().mouseReleaseEvent(event)
-
-        for item in self._netTupleSet:
-            lines = self.scene().addWires(item.net.start, self.scene().wirePen)
-            self.scene().extendWires(lines,item.net.start,item.net.end)
-            self.scene().pruneWires(lines,self.scene().wirePen)
-            self.scene().removeItem(item.net)
-        self._netTupleSet = set()
-
-    def itemChange(self, change, value):
-
-
-        if self.scene() and change == QGraphicsItem.ItemPositionHasChanged:
-            # item's position has changed
-            # do something here
-            for item in self._netTupleSet:
-                if item.start == 1:
-                    item.net.start = self.mapToScene(self.start)
-                elif item.start == 0:
-                    item.net.end = self.mapToScene(self.start)
-        return super().itemChange(change, value)
-
-    # def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
-    #     super().mouseMoveEvent(event)
-    #     self.setPos(event.scenePos() - event.buttonDownPos(Qt.LeftButton))
-
-    def toSymbolPin(self, start: QPoint, pen: QPen, gridTuple: tuple):
-        return pin(start, pen, self.pinName, self.pinDir, self.pinType, gridTuple)
-
-    @property
-    def start(self):
-        return self._start
-
-    @start.setter
-    def start(self, start):
-        self._start = start
-
-    @property
-    def pinName(self):
-        return self._pinName
-
-    @pinName.setter
-    def pinName(self, pinName):
-        if pinName != "":
-            self._pinName = pinName
-
-    @property
-    def pinDir(self):
-        return self._pinDir
-
-    @pinDir.setter
-    def pinDir(self, direction: str):
-        if direction in self.pinDirs:
-            self._pinDir = direction
-
-    @property
-    def pinType(self):
-        return self._pinType
-
-    @pinType.setter
-    def pinType(self, pintype: str):
-        if pintype in self.pinTypes:
-            self._pinType = pintype
+#   “Commons Clause” License Condition v1.0
+#  #
+#   The Software is provided to you by the Licensor under the License, as defined
+#   below, subject to the following condition.
+#  #
+#   Without limiting other conditions in the License, the grant of rights under the
+#   License will not include, and the License does not grant to you, the right to
+#   Sell the Software.
+#  #
+#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#   granted to you under the License to provide to third parties, for a fee or other
+#   consideration (including without limitation fees for hosting or consulting/
+#   support services related to the Software), a product or service whose value
+#   derives, entirely or substantially, from the functionality of the Software. Any
+#   license notice or attribution required by the License must also include this
+#   Commons Clause License Condition notice.
+#  #
+#   Software: Revolution EDA
+#   License: Mozilla Public License 2.0
+#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
+import math
+
+# shape class definition for symbol editor.
+# base class for all shapes: rectangle, circle, line
+from PySide6.QtCore import QPoint, QRect, QRectF, Qt, QLine, QLineF
+from PySide6.QtGui import (QPen, QFont, QFontMetrics, QPainterPath, QTextOption,
+                           QFontDatabase, )
+from PySide6.QtWidgets import (QGraphicsItem, QGraphicsSceneMouseEvent, )
+from quantiphy import Quantity
+import revedaEditor.common.net as net
+import revedaEditor.backend.dataDefinitions as ddef
+import pdk.callbacks as cb
+
+
+class shape(QGraphicsItem):
+    def __init__(self, pen: QPen, gridTuple: tuple) -> None:
+        super().__init__()
+        self.setFlag(QGraphicsItem.ItemIsMovable, True)
+        self.setFlag(QGraphicsItem.ItemIsSelectable, True)
+        self.setFlag(QGraphicsItem.ItemSendsGeometryChanges, True)
+        self.setFlag(QGraphicsItem.ItemIsFocusable, True)
+        self.setAcceptHoverEvents(True)
+        # self.setZValue(self.layer.z)
+        self._pen = pen
+        self._gridTuple = gridTuple
+        self._angle = 0  # rotation angle
+        self._stretch: bool = False
+
+    def itemChange(self, change, value):
+        if change == QGraphicsItem.ItemPositionChange and self.scene():
+            newPos = value.toPoint()
+            sceneRect = self.scene().sceneRect()
+            viewRect = self.scene().views()[0].viewport().rect()
+            newPos.setX(round(newPos.x() / self._gridTuple[0]) * self._gridTuple[0])
+            newPos.setY(round(newPos.y() / self._gridTuple[1]) * self._gridTuple[1])
+
+            if not sceneRect.contains(newPos):
+                # Keep the item inside the scene rect.
+                if newPos.x() > sceneRect.right():
+                    sceneRect.setRight(newPos.x())
+                    viewRect.setRight(newPos.x())
+                elif newPos.x() < sceneRect.left():
+                    sceneRect.setLeft(newPos.x())
+                    viewRect.setLeft(newPos.x())
+                if newPos.y() > sceneRect.bottom():
+                    sceneRect.setBottom(newPos.y())
+                    viewRect.setBottom(newPos.y())
+                elif newPos.y() < sceneRect.top():
+                    sceneRect.setTop(newPos.y())
+                    viewRect.setTop(newPos.y())
+            return newPos
+        return super().itemChange(change, value)
+
+    @property
+    def angle(self):
+        return self._angle
+
+    @angle.setter
+    def angle(self, value):
+        self._angle = value
+        self.prepareGeometryChange()
+        self.setRotation(value)  # self.update(self.boundingRect())
+
+    @property
+    def pen(self):
+        return self._pen
+
+    @pen.setter
+    def pen(self, value):
+        self._pen = value  # self.update(self.boundingRect())
+
+    @property
+    def gridTuple(self):
+        return self._gridTuple
+
+    @gridTuple.setter
+    def gridTuple(self, value: int):
+        self._gridTuple = value
+
+    @property
+    def stretch(self):
+        return self._stretch
+
+    @stretch.setter
+    def stretch(self, value: bool):
+        self._stretch = value  # self.update(self.boundingRect())
+
+    def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mousePressEvent(event)
+        if self.scene().changeOrigin:
+            self.setFlag(QGraphicsItem.ItemIsMovable, False)
+            self.setFlag(QGraphicsItem.ItemIsSelectable, False)
+        else:
+            self.setFlag(QGraphicsItem.ItemIsMovable, True)
+            self.setFlag(QGraphicsItem.ItemIsSelectable, True)
+
+    def sceneEvent(self, event):
+        """
+        Do not propagate event if shape needs to keep still.
+        """
+
+        if self.scene() and (self.scene().changeOrigin or self.scene().drawMode):
+            return False
+        else:
+            super().sceneEvent(event)
+            return True
+
+    def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mouseMoveEvent(event)
+
+    def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mouseReleaseEvent(event)  # self.setSelected(False)
+
+    def hoverEnterEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        self.setCursor(Qt.ArrowCursor)
+        self.setOpacity(0.75)
+        self.setFocus()
+        super().hoverEnterEvent(event)
+
+    def hoverLeaveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().hoverLeaveEvent(event)
+        self.setCursor(Qt.CrossCursor)
+        self.setOpacity(1)
+        self.clearFocus()
+
+    def contextMenuEvent(self, event):
+        self.scene().itemContextMenu.exec_(event.screenPos())
+
+    def snapToBase(self, number, base):
+        """
+        Restrict a number to the multiples of base
+        """
+        return base * int(round(number / base))
+
+    def snapToGrid(self, point: QPoint, gridTuple: tuple[int, int]):
+        """
+        snap point to grid. Divides and multiplies by grid size.
+        """
+        return QPoint(gridTuple[0] * int(round(point.x() / gridTuple[0])),
+                      gridTuple[1] * int(round(point.y() / gridTuple[1])), )
+
+
+class rectangle(shape):
+    """
+    rect: QRect defined by top left corner and bottom right corner. QRect(Point1,Point2)
+    """
+
+    sides = ["Left", "Right", "Top", "Bottom"]
+
+    def __init__(self, start: QPoint, end: QPoint, pen: QPen, grid: tuple, ):
+        super().__init__(pen, grid)
+        self._rect = QRectF(start, end).normalized()
+        self._start = self._rect.topLeft()
+        self._end = self._rect.bottomRight()
+        self._stretchSide = None
+
+    def boundingRect(self):
+        return self._rect.normalized().adjusted(-2, -2, 2, 2)
+
+    def paint(self, painter, option, widget):
+        if self.isSelected():
+            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
+            painter.drawRect(self._rect)
+            if self.stretch:
+                painter.setPen(QPen(Qt.red, 2, Qt.SolidLine))
+                if self._stretchSide == rectangle.sides[0]:
+                    painter.drawLine(self.rect.topLeft(), self.rect.bottomLeft())
+                elif self._stretchSide == rectangle.sides[1]:
+                    painter.drawLine(self.rect.topRight(), self.rect.bottomRight())
+                elif self._stretchSide == rectangle.sides[2]:
+                    painter.drawLine(self.rect.topLeft(), self.rect.topRight())
+                elif self._stretchSide == rectangle.sides[3]:
+                    painter.drawLine(self.rect.bottomLeft(), self.rect.bottomRight())
+        else:
+            painter.setPen(self._pen)
+            painter.drawRect(self._rect)
+
+    @property
+    def rect(self):
+        return self._rect
+
+    @rect.setter
+    def rect(self, rect: QRect):
+        self.prepareGeometryChange()
+        self._rect = rect
+
+    @property
+    def start(self):
+        return self._start
+
+    @start.setter
+    def start(self, start: QPoint):
+        self.prepareGeometryChange()
+        self._rect = QRectF(start, self.end).normalized()
+        self._start = start
+
+    @property
+    def end(self):
+        return self._end
+
+    @end.setter
+    def end(self, end: QPoint):
+        self.prepareGeometryChange()
+        self._rect = QRectF(self.start, end).normalized()
+        self._end = end
+
+    @property
+    def centre(self):
+        return QPoint(int(self._rect.x() + self._rect.width() / 2),
+                      int(self._rect.y() + self._rect.height() / 2), )
+
+    @property
+    def height(self):
+        return self.rect.height()
+
+    @height.setter
+    def height(self, height: int):
+        self.prepareGeometryChange()
+        self._rect.setHeight(height)
+
+    @property
+    def width(self):
+        return self.rect.width()
+
+    @width.setter
+    def width(self, width):
+        self.prepareGeometryChange()
+        self.rect.setWidth(width)
+
+    @property
+    def objName(self):
+        return "RECTANGLE"
+
+    @property
+    def left(self):
+        return self.rect.left()
+
+    @left.setter
+    def left(self, left: int):
+        self.rect.setLeft(left)
+
+    @property
+    def right(self):
+        return self.rect.right()
+
+    @right.setter
+    def right(self, right: int):
+        self.prepareGeometryChange()
+        self.rect.setRight(right)
+
+    @property
+    def top(self):
+        return self.rect.top()
+
+    @top.setter
+    def top(self, top: int):
+        self.prepareGeometryChange()
+        self.rect.setTop(top)
+
+    @property
+    def bottom(self):
+        return self.rect.bottom()
+
+    @bottom.setter
+    def bottom(self, bottom: int):
+        self.prepareGeometryChange()
+        self.rect.setBottom(bottom)
+
+    @property
+    def origin(self):
+        return self.rect.bottomLeft()
+
+    @property
+    def stretchSide(self):
+        return self._stretchSide
+
+    @stretchSide.setter
+    def stretchSide(self, value: str):
+        self.prepareGeometryChange()
+        self._stretchSide = value
+
+    def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mousePressEvent(event)
+        eventPos = event.pos().toPoint()
+        if self._stretch:
+            self.setFlag(QGraphicsItem.ItemIsMovable, False)
+            if eventPos.x() == self.snapToBase(self._rect.left(), self.gridTuple[0]):
+                if self._rect.top() <= eventPos.y() <= self._rect.bottom():
+                    self.setCursor(Qt.SizeHorCursor)
+                    self._stretchSide = rectangle.sides[0]
+            elif eventPos.x() == self.snapToBase(self._rect.right(), self.gridTuple[0]):
+                if self._rect.top() <= eventPos.y() <= self._rect.bottom():
+                    self.setCursor(Qt.SizeHorCursor)
+                    self._stretchSide = rectangle.sides[1]
+            elif eventPos.y() == self.snapToBase(self._rect.top(), self.gridTuple[1]):
+                if self._rect.left() <= eventPos.x() <= self._rect.right():
+                    self.setCursor(Qt.SizeVerCursor)
+                    self._stretchSide = rectangle.sides[2]
+            elif eventPos.y() == self.snapToBase(self._rect.bottom(), self.gridTuple[1]):
+                if self._rect.left() <= eventPos.x() <= self._rect.right():
+                    self.setCursor(Qt.SizeVerCursor)
+                    self._stretchSide = rectangle.sides[3]
+
+    def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        eventPos = event.pos().toPoint()
+        if self.stretch:
+            self.prepareGeometryChange()
+            if self.stretchSide == rectangle.sides[0]:
+                self.setCursor(Qt.SizeHorCursor)
+                self.rect.setLeft(eventPos.x())
+            elif self.stretchSide == rectangle.sides[1]:
+                self.setCursor(Qt.SizeHorCursor)
+                self.rect.setRight(eventPos.x() - int(self.pen.width() / 2))
+            elif self.stretchSide == rectangle.sides[2]:
+                self.setCursor(Qt.SizeVerCursor)
+                self.rect.setTop(eventPos.y())
+            elif self.stretchSide == rectangle.sides[3]:
+                self.setCursor(Qt.SizeVerCursor)
+                self.rect.setBottom(eventPos.y() - int(self.pen.width() / 2))
+            self.update()
+        else:
+            super().mouseMoveEvent(event)
+
+    def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        self.setFlag(QGraphicsItem.ItemIsMovable, True)
+        super().mouseReleaseEvent(event)
+        # self.start = self.rect.topLeft()
+        # self.end = self.rect.bottomRight()
+        if self.stretch:
+            self._stretch = False
+            self._stretchSide = None
+            self.setCursor(Qt.ArrowCursor)
+
+
+class circle(shape):
+    def __init__(self, centre: QPoint, end: QPoint, pen: QPen, gridTuple: tuple):
+        super().__init__(pen, gridTuple)
+        xlen = abs(end.x() - centre.x())
+        ylen = abs(end.y() - centre.y())
+        self._radius = self.snapToBase(int(math.sqrt(xlen ** 2 + ylen ** 2)),
+                                       self.gridTuple[0])
+        self._centre = centre
+        self._topLeft = self._centre - QPoint(self._radius, self._radius)
+        self._rightBottom = self._centre + QPoint(self._radius, self._radius)
+        self._end = self._centre + QPoint(self._radius, 0)  # along x-axis
+        self._stretch = False
+        self._startStretch = False
+
+    def paint(self, painter, option, widget) -> None:
+        if self.isSelected():
+            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
+            painter.drawEllipse(self._centre, 1, 1)
+            if self._stretch:
+                painter.setPen(QPen(Qt.red, 2, Qt.SolidLine))
+        else:
+            painter.setPen(self._pen)
+        painter.drawEllipse(self._centre, self._radius, self._radius)
+
+    @property
+    def centre(self):
+        return self._centre
+
+    @centre.setter
+    def centre(self, centre: QPoint):
+        self.prepareGeometryChange()
+        self._centre = self.snapToGrid(centre, self._gridTuple)
+        # self.topLeft = self._centre - QPoint(self._radius, self._radius)
+        # self.rightBottom = self._centre + QPoint(self._radius, self._radius)
+        self._end = self._centre + QPoint(self._radius, 0)
+
+    @property
+    def radius(self):
+        return self._radius
+
+    @radius.setter
+    def radius(self, radius: int):
+        self.prepareGeometryChange()
+        self._radius = self.snapToBase(radius, self._gridTuple[0])
+        self._end = self._centre + QPoint(self._radius, 0)
+        self._topLeft = self._centre - QPoint(self._radius, self._radius)
+        self._rightBottom = self._centre + QPoint(self._radius, self._radius)
+
+    @property
+    def centre(self):
+        return self._centre
+
+    @centre.setter
+    def centre(self, value: QPoint):
+        self.prepareGeometryChange()
+        if isinstance(value, QPoint):
+            self._centre = value
+
+    @property
+    def end(self):
+        return self._end
+
+    @end.setter
+    def end(self, value: QPoint):
+        if isinstance(value, QPoint):
+            self.prepareGeometryChange()
+            self._end = value
+
+    @property
+    def rightBottom(self):
+        return self._rightBottom
+
+    @rightBottom.setter
+    def rightBottom(self, value: QPoint):
+        if isinstance(value, QPoint):
+            self._rightBottom = value
+
+    @property
+    def topLeft(self):
+        return self._topLeft
+
+    @topLeft.setter
+    def topLeft(self, value: QPoint):
+        if isinstance(value, QPoint):
+            self._topLeft = value
+
+    @property
+    def objName(self):
+        return "CIRCLE"
+
+    def boundingRect(self):
+        return (
+            QRectF(self._topLeft, self._rightBottom).normalized().adjusted(-2, -2, 2, 2))
+
+    def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mousePressEvent(event)
+        if self.isSelected() and self._stretch:
+            self.setFlag(QGraphicsItem.ItemIsMovable, False)
+            # eventPos = self.snap2grid(event.pos(), self._gridTuple)
+            eventPos = event.pos().toPoint()
+            distance = self.snapToBase(math.sqrt((eventPos.x() - self._centre.x()) ** 2 + (
+                    eventPos.y() - self._centre.y()) ** 2), self._gridTuple[0], )
+            if distance == self._radius:
+                self._startStretch = True
+                self.setCursor(Qt.DragMoveCursor)
+
+    def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mouseMoveEvent(event)
+        if self._startStretch:
+            eventPos = event.pos().toPoint()
+            distance = self.snapToBase(math.sqrt((eventPos.x() - self._centre.x()) ** 2 + (
+                    eventPos.y() - self._centre.y()) ** 2), self._gridTuple[0], )
+            self.prepareGeometryChange()
+            self._radius = distance
+
+    def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mouseReleaseEvent(event)
+        if self._startStretch:
+            self._startStretch = False
+            self.setFlag(QGraphicsItem.ItemIsMovable, True)
+            self.setFlag(QGraphicsItem.ItemIsSelectable, True)
+            self._topLeft = self._centre - QPoint(self._radius, self._radius)
+            self._rightBottom = self._centre + QPoint(self._radius, self._radius)
+            self._end = self._centre + QPoint(self._radius, 0)
+            self.setCursor(Qt.ArrowCursor)
+
+
+class arc(shape):
+    """
+    Class to draw arc shapes. Can have four directions.
+    """
+
+    arcTypes = ["Up", "Right", "Down", "Left"]
+    sides = ["Left", "Right", "Top", "Bottom"]
+
+    def __init__(self, start: QPoint, end: QPoint, pen: QPen, gridTuple: tuple):
+        super().__init__(pen, gridTuple)
+        self._start = start
+        self._end = end
+        self._rect = QRectF(self._start, self._end).normalized()
+        self._arcLine = QLineF(self._start, self._end)
+        self._arcAngle = 0
+        self._width = self._rect.width()
+        self._height = self._rect.height()
+        self._adjustment = int(self.pen.width() / 2)
+        self._stretchSide = None
+        self.findAngle()
+
+    def findAngle(self):
+        self._arcAngle = self._arcLine.angle()
+        if 90 >= self._arcAngle >= 0:
+            self._arcType = arc.arcTypes[0]
+        elif 180 >= self._arcAngle > 90:
+            self._arcType = arc.arcTypes[1]
+        elif 270 >= self._arcAngle > 180:
+            self._arcType = arc.arcTypes[2]
+        elif 360 > self._arcAngle > 270:
+            self._arcType = arc.arcTypes[3]
+
+    def paint(self, painter, option, widget) -> None:
+        if self.isSelected():
+            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
+            painter.drawRect(self.rect)
+            self.arcDraw(painter)
+            if self._stretch:
+                painter.setPen(QPen(Qt.red, 2, Qt.SolidLine))
+                self.arcDraw(painter)
+                if self._stretchSide == arc.sides[0]:
+                    painter.drawLine(self._rect.topLeft(), self._rect.bottomLeft())
+                elif self._stretchSide == arc.sides[1]:
+                    painter.drawLine(self._rect.topRight(), self._rect.bottomRight())
+                elif self._stretchSide == arc.sides[2]:
+                    painter.drawLine(self._rect.topLeft(), self._rect.topRight())
+                elif self._stretchSide == arc.sides[3]:
+                    painter.drawLine(self._rect.bottomLeft(), self._rect.bottomRight())
+        else:
+            painter.setPen(self._pen)
+            self.arcDraw(painter)
+
+    def arcDraw(self, painter):
+        if self._arcType == arc.arcTypes[0]:
+            painter.drawArc(self._rect, 0, 180 * 16)
+        elif self._arcType == arc.arcTypes[1]:
+            painter.drawArc(self._rect, 90 * 16, 180 * 16)
+        elif self._arcType == arc.arcTypes[2]:
+            painter.drawArc(self._rect, 180 * 16, 180 * 16)
+        elif self._arcType == arc.arcTypes[3]:
+            painter.drawArc(self._rect, 270 * 16, 180 * 16)
+
+    def boundingRect(self):
+        return self._rect.adjusted(-2, -2, 2, 2)
+
+    @property
+    def objName(self):
+        return "ARC"
+
+    @property
+    def rect(self):
+        return self._rect
+
+    @rect.setter
+    def rect(self, arc_rect: QRect):
+        assert isinstance(arc_rect, QRect)
+        self._rect = arc_rect.normalized()
+
+    @property
+    def start(self):
+        return self._start
+
+    @start.setter
+    def start(self, point: QPoint):
+        assert isinstance(point, QPoint)
+        self.prepareGeometryChange()
+        self._start = self.snapToGrid(point, self.gridTuple)
+
+    @property
+    def end(self):
+        return self._end
+
+    @end.setter
+    def end(self, point: QPoint):
+        assert isinstance(point, QPoint)
+        self.prepareGeometryChange()
+        self._end = point
+        self._arcLine = QLineF(self._start, self._end)
+        self._arcAngle = self._arcLine.angle()
+        self.findAngle()
+        self._rect = QRectF(self._start, self._end).normalized()
+
+    @property
+    def width(self):
+        return self._width
+
+    @width.setter
+    def width(self, width):
+        self._width = width
+        self.prepareGeometryChange()
+        self.rect.setWidth(self._width)
+
+    @property
+    def height(self):
+        return self._height
+
+    @height.setter
+    def height(self, height):
+        self._height = height
+        self.prepareGeometryChange()
+        self.rect.setHeight(self._height)
+
+    def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mousePressEvent(event)
+        eventPos = event.pos().toPoint()
+        if self._stretch:
+            self.setFlag(QGraphicsItem.ItemIsMovable, False)
+            if eventPos.x() == self.snapToBase(self._rect.left(), self.gridTuple[0]):
+                if self._rect.top() <= eventPos.y() <= self._rect.bottom():
+                    self.setCursor(Qt.SizeHorCursor)
+                    self._stretchSide = arc.sides[0]
+            elif eventPos.x() == self.snapToBase(self._rect.right(), self.gridTuple[0]):
+                if self._rect.top() <= eventPos.y() <= self._rect.bottom():
+                    self.setCursor(Qt.SizeHorCursor)
+                    self._stretchSide = arc.sides[1]
+            elif eventPos.y() == self.snapToBase(self._rect.top(), self.gridTuple[1]):
+                if self._rect.left() <= eventPos.x() <= self._rect.right():
+                    self.setCursor(Qt.SizeVerCursor)
+                    self._stretchSide = arc.sides[2]
+            elif eventPos.y() == self.snapToBase(self._rect.bottom(), self.gridTuple[1]):
+                if self._rect.left() <= eventPos.x() <= self._rect.right():
+                    self.setCursor(Qt.SizeVerCursor)
+                    self._stretchSide = arc.sides[3]
+
+    def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mouseMoveEvent(event)
+
+        eventPos = event.pos().toPoint()
+        if self._stretch:
+            self.prepareGeometryChange()
+            if self._stretchSide == arc.sides[0]:
+                self.setCursor(Qt.SizeHorCursor)
+                self._rect.setLeft(eventPos.x())
+            elif self._stretchSide == arc.sides[1]:
+                self.setCursor(Qt.SizeHorCursor)
+                self._rect.setRight(eventPos.x() - self._adjustment)
+            elif self._stretchSide == arc.sides[2]:
+                self.setCursor(Qt.SizeVerCursor)
+                self._rect.setTop(eventPos.y())
+            elif self._stretchSide == arc.sides[3]:
+                self.setCursor(Qt.SizeVerCursor)
+                self._rect.setBottom(eventPos.y() - self._adjustment)
+            self.update()
+
+    def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        self.setFlag(QGraphicsItem.ItemIsMovable, True)
+        super().mouseReleaseEvent(event)
+        if self.stretch:
+            self._stretch = False
+            self._stretchSide = None
+            self.setCursor(Qt.ArrowCursor)
+
+            if self._arcType == arc.arcTypes[0]:
+                self._start = self.snapToGrid(self._rect.bottomLeft(), self.gridTuple)
+                self._end = self.snapToGrid(self._rect.topRight(), self.gridTuple)
+            elif self._arcType == arc.arcTypes[1]:
+                self._start = self.snapToGrid(self._rect.topLeft(), self.gridTuple)
+                self._end = self.snapToGrid(self._rect.bottomRight(), self.gridTuple)
+            elif self._arcType == arc.arcTypes[2]:
+                self._start = self.snapToGrid(self._rect.topRight(), self.gridTuple)
+                self._end = self.snapToGrid(self._rect.bottomLeft(), self.gridTuple)
+            elif self._arcType == arc.arcTypes[3]:
+                self._start = self.snapToGrid(self._rect.bottomRight(), self.gridTuple)
+                self._end = self.snapToGrid(self._rect.topLeft(), self.gridTuple)
+            self._rect = QRectF(self._start, self._end).normalized()
+
+
+class line(shape):
+    """
+    line class definition for symbol drawing.
+    """
+
+    stretchSides = ["start", "end"]
+
+    def __init__(self, start: QPoint, end: QPoint, pen: QPen, grid: tuple, ):
+        super().__init__(pen, grid)
+        self._end = end
+        self._start = start
+        self._pen = pen
+        self._stretch = False
+        self._stretchSide = None
+        self._line = QLine(self._start, self._end)
+        self._rect = QRect(self._start, self._end).normalized()
+        self._horizontal = True  # True if line is horizontal, False if vertical
+
+    def boundingRect(self):
+        return self._rect.adjusted(-2, -2, 2, 2)
+
+    def shape(self):
+        path = QPainterPath()
+        path.addRect(self._rect.adjusted(-2, -2, 2, 2))
+        return path
+
+    def shape(self):
+        path = QPainterPath()
+        path.addRect(self._rect.adjusted(-2, -2, 2, 2))
+        return path
+
+    def paint(self, painter, option, widget):
+        if self.isSelected():
+            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
+            if self._stretch:
+                painter.setPen(QPen(Qt.red, 2, Qt.SolidLine))
+                if self._stretchSide == line.stretchSides[0]:
+                    painter.drawEllipse(self._start, self.gridTuple[0], self.gridTuple[1])
+                elif self._stretchSide == line.stretchSides[1]:
+                    painter.drawEllipse(self._end, self.gridTuple[0], self.gridTuple[1])
+        else:
+            painter.setPen(self._pen)
+        painter.drawLine(self._line)
+
+    def objName(self):
+        return "LINE"
+
+    @property
+    def rect(self):
+        return self._rect
+
+    @rect.setter
+    def rect(self, rect: QRect):
+        self._rect = rect
+
+    @property
+    def start(self):
+        return self._start
+
+    @start.setter
+    def start(self, start: QPoint):
+        self.prepareGeometryChange()
+        self._start = start
+        self._line = QLine(self._start, self._end)
+        self._rect = QRect(self._start, self._end).normalized()
+
+    @property
+    def end(self):
+        return self._end
+
+    @end.setter
+    def end(self, end: QPoint):
+        self.prepareGeometryChange()
+        self._end = end
+        self._line = QLine(self._start, self._end)
+        self._rect = QRect(self._start, self._end).normalized()
+
+    @property
+    def pen(self):
+        return self._pen
+
+    @pen.setter
+    def pen(self, pen: QPen):
+        self._pen = pen
+
+    @property
+    def width(self):
+        return self._pen.width()
+
+    @width.setter
+    def width(self, width: int):
+        self._pen.setWidth(width)
+
+    def bBox(self) -> QRect:
+        return self.boundingRect()
+
+    def Move(self, offset: QPoint):
+        self.start += offset
+        self._end += offset
+
+    @property
+    def length(self):
+        return math.sqrt(
+            (self.start.x() - self._end.x()) ** 2 + (self.start.y() - self._end.y()) ** 2)
+
+    def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mousePressEvent(event)
+        if self.isSelected() and self._stretch:
+            self.setFlag(QGraphicsItem.ItemIsMovable, False)
+            eventPos = event.pos().toPoint()
+            if eventPos == self.start:
+                self._stretchSide = line.stretchSides[0]
+            elif eventPos == self._end:
+                self._stretchSide = line.stretchSides[1]
+
+    def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        eventPos = event.pos().toPoint()
+        if self._stretchSide == line.stretchSides[0]:
+            self.prepareGeometryChange()
+            self.start = eventPos
+            self._line = QLine(self.start, self._end)
+            self._rect = QRect(self.start, self._end).normalized()
+        elif self._stretchSide == line.stretchSides[1]:
+            self.prepareGeometryChange()
+            self._end = eventPos
+            self._line = QLine(self.start, self._end)
+            self._rect = QRect(self.start, self._end).normalized()
+
+        super().mouseMoveEvent(event)
+
+    def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mouseReleaseEvent(event)
+        self._stretch = False
+        self.setFlag(QGraphicsItem.ItemIsMovable, True)
+        self.setFlag(QGraphicsItem.ItemIsSelectable, True)
+        self._stretchSide = ""
+
+
+class pin(shape):
+    """
+    symbol pin class definition for symbol drawing.
+    """
+
+    pinDirs = ["Input", "Output", "Inout"]
+    pinTypes = ["Signal", "Ground", "Power", "Clock", "Digital", "Analog"]
+
+    def __init__(self, start: QPoint, pen: QPen, pinName: str = "",
+                 pinDir: str = pinDirs[0], pinType: str = pinTypes[0],
+                 grid: tuple = (10, 10), ):
+        super().__init__(pen, grid)
+
+        self._start = start  # centre of pin
+        self._pinName = pinName
+        self._pinDir = pinDir
+        self._pinType = pinType
+        self._connected = False  # True if the pin is connected to a net.
+        self._rect = QRect(self._start.x() - 5, self._start.y() - 5, 10, 10)
+
+    def __repr__(self):
+        return f"pin: {self._pinName} {self.mapToScene(self._start)}"
+
+    def boundingRect(self):
+        return self._rect  #
+
+    def paint(self, painter, option, widget):
+        painter.setPen(self._pen)
+        painter.setBrush(self._pen.color())
+        painter.drawRect(self._rect)
+        painter.setFont(QFont("Arial", 12))
+        painter.drawText(QPoint(self._start.x() - 5, self._start.y() - 10), self._pinName)
+        if self.isSelected():
+            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
+            painter.setBrush(Qt.yellow)
+            painter.drawRect(self._rect)
+
+    def objName(self):
+        return "PIN"
+
+    @property
+    def start(self):
+        return self._start
+
+    @start.setter
+    def start(self, start):
+        self._start = start
+
+    @property
+    def pinName(self):
+        return self._pinName
+
+    @pinName.setter
+    def pinName(self, pinName):
+        if pinName != "":
+            self._pinName = pinName
+
+    @property
+    def pinDir(self):
+        return self._pinDir
+
+    @pinDir.setter
+    def pinDir(self, direction: str):
+        if direction in self.pinDirections:
+            self._pinDir = direction
+
+    @property
+    def pinType(self):
+        return self._pinType
+
+    @pinType.setter
+    def pinType(self, pintype: str):
+        if pintype in self.pinTypes:
+            self._pinType = pintype
+
+    @property
+    def connected(self):
+        return self._connected
+
+    @connected.setter
+    def connected(self, value: bool):
+        if isinstance(value, bool):
+            self._connected = value
+
+    def toSchematicPin(self, start: QPoint, pen: QPen, gridTuple):
+        return schematicPin(start, pen, self.pinName, self.pinDir, self.pinType, gridTuple)
+
+
+class text(shape):
+    """
+    This class is for text annotations on symbol or schematics.
+    """
+
+    textAlignments = ["Left", "Center", "Right"]
+    textOrients = ["R0", "R90", "R180", "R270"]
+
+    def __init__(self, start: QPoint, pen: QPen, textContent: str = "",
+                 grid: tuple = (10, 10), fontFamily="Helvetica", fontStyle="Regular",
+                 textHeight: str = "12", textAlign: str = "Left", textOrient: str = "R0", ):
+        super().__init__(pen, grid)
+
+        self._start = start
+        self._pen = pen
+        self._textContent = textContent
+        self._textHeight = textHeight
+        self._textAlign = textAlign
+        self._textOrient = textOrient
+        self._textFont = QFont(fontFamily)
+        self._textFont.setStyleName(fontStyle)
+        self._textFont.setPointSize(int(float(self._textHeight)))
+        self._textFont.setKerning(True)
+        self.setOpacity(1)
+        self._fm = QFontMetrics(self._textFont)
+        self._textOptions = QTextOption()
+        if self._textAlign == text.textAlignments[0]:
+            self._textOptions.setAlignment(Qt.AlignmentFlag.AlignLeft)
+        elif self._textAlign == text.textAlignments[1]:
+            self._textOptions.setAlignment(Qt.AlignmentFlag.AlignCenter)
+        elif self._textAlign == text.textAlignments[2]:
+            self._textOptions.setAlignment(Qt.AlignmentFlag.AlignRight)
+
+    def boundingRect(self):
+        if self._textAlign == text.textAlignments[0]:
+            self._rect = self._fm.boundingRect(QRect(0, 0, 400, 400),
+                                               Qt.AlignmentFlag.AlignLeft,
+                                               self._textContent)
+        elif self._textAlign == text.textAlignments[1]:
+            self._rect = self._fm.boundingRect(QRect(0, 0, 400, 400),
+                                               Qt.AlignmentFlag.AlignCenter,
+                                               self._textContent)
+        elif self._textAlign == text.textAlignments[2]:
+            self._rect = self._fm.boundingRect(QRect(0, 0, 400, 400),
+                                               Qt.AlignmentFlag.AlignRight,
+                                               self._textContent)
+        return QRect(self._start.x(), self._start.y() - self._rect.height(),
+                     self._rect.width(), self._rect.height(), )
+
+    def paint(self, painter, option, widget):
+        painter.setFont(self._textFont)
+        if self.isSelected():
+            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
+            painter.drawRect(self.boundingRect())
+        else:
+            painter.setPen(self._pen)
+        painter.drawText(self.boundingRect(), self._textContent, o=self._textOptions)
+
+    @property
+    def start(self):
+        return self._start
+
+    @start.setter
+    def start(self, value: QPoint):
+        self._start = value
+
+    @property
+    def textContent(self):
+        return self._textContent
+
+    @textContent.setter
+    def textContent(self, inputText: str):
+        if isinstance(inputText, str):
+            self._textContent = inputText
+        else:
+            self.scene().logger.error(f"Not a string: {inputText}")
+
+    @property
+    def fontFamily(self) -> str:
+        return self._textFont.family()
+
+    @fontFamily.setter
+    def fontFamily(self, familyName):
+        fontFamilies = QFontDatabase.families(QFontDatabase.Latin)
+        fixedFamilies = [family for family in fontFamilies if
+                         QFontDatabase.isFixedPitch(family)]
+        if familyName in fixedFamilies:
+            self._textFont.setFamily(familyName)
+        else:
+            self.scene().logger.error(f"Not a valid font name: {familyName}")
+
+    @property
+    def fontStyle(self) -> str:
+        return self._textFont.styleName()
+
+    @fontStyle.setter
+    def fontStyle(self, value: str):
+        if value in QFontDatabase.styles(self._textFont.family()):
+            self._textFont.setStyleName(value)
+        else:
+            self.scene().logger.error(f"Not a valid font style: {value}")
+
+    @property
+    def textHeight(self) -> int:
+        return self._textHeight
+
+    @textHeight.setter
+    def textHeight(self, value: int):
+        fontSizes = [str(size) for size in QFontDatabase.pointSizes(self._textFont.family(),
+                                                                    self._textFont.styleName())]
+        if value in fontSizes:
+            self._textHeight = value
+        else:
+            self.scene().logger.error(f"Not a valid font height: {value}")
+            self.scene().logger.warning(f"Valid font heights are: {fontSizes}")
+
+    @property
+    def textFont(self) -> QFont:
+        return self._textFont
+
+    @textFont.setter
+    def textFont(self, value: QFont):
+        assert isinstance(value, QFont)
+        self._textFont = value
+
+    @property
+    def textAlignment(self):
+        return self._textAlign
+
+    @textAlignment.setter
+    def textAlignment(self, value):
+        if value in text.textAlignments:
+            self._textAlign = value
+        else:
+            self.scene().logger.error(f"Not a valid text alignment value: {value}")
+
+    @property
+    def textOrient(self):
+        return self._textOrient
+
+    @textOrient.setter
+    def textOrient(self, value):
+        if value in text.textOrients:
+            self._textOrient = value
+        else:
+            self.scene().logger.error(f"Not a valid text orientation: {value}")
+
+
+class label(shape):
+    """
+    label: text class definition for symbol drawing.
+    labelText is what is shown on the symbol in a schematic
+    """
+
+    labelAlignments = ["Left", "Center", "Right"]
+    labelOrients = ["R0", "R90", "R180", "R270", "MX", "MX90", "MY", "MY90"]
+    labelUses = ["Normal", "Instance", "Pin", "Device", "Annotation"]
+    labelTypes = ["Normal", "NLPLabel", "PyLabel"]
+    predefinedLabels = ["[@libName]", "[@cellName]", "[@viewName]", "[@instName]",
+                        "[@modelName]", "[@elementNum]"]
+
+    def __init__(self, start: QPoint, pen: QPen, labelDefinition: str = "",
+                 grid: tuple = (10, 10), labelType: str = "Normal", labelHeight: str = "12",
+                 labelAlign: str = "Left", labelOrient: str = "R0",
+                 labelUse: str = "Normal", ):
+        super().__init__(pen, grid)
+        self._start = start  # top left corner
+        self._pen = pen
+        self._labelDefinition = labelDefinition  # label definition is what is
+        # entered in the symbol editor
+        self._labelName = None  # label Name
+        self._labelValue = None  # label value
+        self._labelText = None  # Displayed label
+        self._labelHeight = labelHeight
+        self._labelAlign = labelAlign
+        self._labelOrient = labelOrient
+        self._labelUse = labelUse
+        self._labelType = labelType
+        self._labelFont = QFont("Arial")
+        self._labelFont.setPointSize(int(float(self._labelHeight)))
+        self._labelFont.setKerning(False)
+        self._labelVisible: bool = False
+        self._labelValueSet: bool = False
+        # labels are visible by default
+        self.setOpacity(1)
+        self._fm = QFontMetrics(self._labelFont)
+        self._rect = self._fm.boundingRect(self._labelDefinition)
+
+    def __repr__(self):
+        return f"label: {self._labelText} for {self._labelDefinition} at {self._start}, " \
+               f"value =  {self._labelValue}"
+
+    def boundingRect(self):
+        return QRect(self._start.x(), self._start.y(), self._rect.width(),
+                     self._rect.height()).normalized().adjusted(0, 0, 0, 5)  #
+
+    def shape(self) -> QPainterPath:
+        path = QPainterPath()
+        path.addRect(self.boundingRect())
+        return path
+
+    def paint(self, painter, option, widget):
+        # self._rect = self.fm.boundingRect(self.labelName)
+        self._labelFont.setPointSize(int(self._labelHeight))
+        painter.setFont(self._labelFont)
+        if self.isSelected():
+            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
+            painter.drawRect(self.boundingRect())
+        else:
+            painter.setPen(self._pen)
+        if self._labelText:
+            painter.drawText(QPoint(self._start.x(), self._start.y() + self._rect.height()),
+                self._labelText, )
+        else:
+            painter.drawText(QPoint(self._start.x(), self._start.y() + self._rect.height()),
+                self._labelDefinition, )
+        self._fm = QFontMetrics(self._labelFont)
+        self._rect = self._fm.boundingRect(self._labelDefinition)
+
+    @property
+    def start(self):
+        return self._start
+
+    @start.setter
+    def start(self, value: QPoint):
+        self._start = value
+
+    @property
+    def left(self):
+        return self._start.x()
+
+    @property
+    def right(self):
+        return self._start.x() + self.boundingRect().width()
+
+    @property
+    def top(self):
+        return self._start.y()
+
+    @property
+    def bottom(self):
+        return self._start.y() + self.boundingRect().height()
+
+    @property
+    def width(self):
+        return self.boundingRect().width()
+
+    @property
+    def height(self):
+        return self.boundingRect().height()
+
+    @property
+    def labelName(self):
+        return self._labelName
+
+    @labelName.setter
+    def labelName(self, labelName: str):
+        self._labelName = labelName
+
+    @property
+    def labelDefinition(self):
+        return self._labelDefinition
+
+    @labelDefinition.setter
+    def labelDefinition(self, labelDefinition: str):
+        if isinstance(labelDefinition, str):
+            self._labelDefinition = labelDefinition.strip()
+
+    @property
+    def labelValue(self):
+        return self._labelValue
+
+    @labelValue.setter
+    def labelValue(self, labelValue):
+        self._labelValue = labelValue
+        self._labelValueSet = True  # self.labelDefs()
+
+    @property
+    def labelValueSet(self) -> bool:
+        return self._labelValueSet
+
+    @labelValueSet.setter
+    def labelValueSet(self, value: bool):
+        if isinstance(value, bool):
+            self._labelValueSet = value
+
+    @property
+    def labelHeight(self):
+        return self._labelHeight
+
+    @labelHeight.setter
+    def labelHeight(self, value: int):
+        self._labelHeight = value
+
+    @property
+    def labelText(self):
+        return self._labelText
+
+    @labelText.setter
+    def labelText(self, labelText):
+        self._labelText = labelText
+        self._rect = self._fm.boundingRect(self._labelText).normalized().adjusted(0, 0, 0,
+                                                                                  5)
+
+    def objName(self):
+        return "LABEL"
+
+    @property
+    def labelType(self):
+        return self._labelType
+
+    @labelType.setter
+    def labelType(self, labelType):
+        if labelType in self.labelTypes:
+            self._labelType = labelType
+        elif self.scene():
+            self.scene().logger.error("Invalid label type")
+
+    @property
+    def labelAlign(self):
+        return self._labelAlign
+
+    @labelAlign.setter
+    def labelAlign(self, labelAlignment):
+        if labelAlignment in self.labelAlignments:
+            self._labelAlign = labelAlignment
+        elif self.scene():
+            self.scene().logger.error("Invalid label alignment")
+
+    @property
+    def labelOrient(self):
+        return self._labelOrient
+
+    @labelOrient.setter
+    def labelOrient(self, labelOrient):
+        if labelOrient in self.labelOrients:
+            self._labelOrient = labelOrient
+        else:
+            print("Invalid label orientation")
+
+    @property
+    def labelUse(self):
+        return self._labelUse
+
+    @labelUse.setter
+    def labelUse(self, labelUse):
+        if labelUse in self.labelUses:
+            self._labelUse = labelUse
+        elif self.scene():
+            self.scene().logger.error("Invalid label use")
+
+    @property
+    def labelFont(self):
+        return self._labelFont
+
+    @labelFont.setter
+    def labelFont(self, labelFont: QFont):
+        self._labelFont = labelFont
+
+    @property
+    def labelVisible(self) -> bool:
+        return self._labelVisible
+
+    @labelVisible.setter
+    def labelVisible(self, value: bool):
+        assert isinstance(value, bool)
+        if value:
+            self.setOpacity(1)
+            self._labelVisible = True
+        else:
+            self.setOpacity(0.001)
+            self._labelVisible = False
+
+    def moveBy(self, delta: QPoint):
+        self._start += delta
+
+    def labelDefs(self):
+        """
+        This method will create label name, value andtext from label
+        definition. It should be run label is defined or redefined.
+        """
+        self.prepareGeometryChange()
+        if self._labelType == label.labelTypes[0]:
+            self._labelName = self._labelDefinition
+            self._labelText = self._labelDefinition
+            self._labelValue = None
+            self._labelValueSet = True
+        elif self.labelType == label.labelTypes[1]:
+            try:
+                if self._labelDefinition in label.predefinedLabels:
+                    self._labelValueSet = True
+                    match self.labelDefinition:
+                        case "[@cellName]":
+                            self._labelName = "cellName"
+                            self._labelValue = self.parentItem().cellName
+                            self._labelText = self._labelValue
+                        case "[@instName]":
+                            self._labelName = "instName"
+                            self._labelValue = f"I{self.parentItem().counter}"
+                            self._labelText = self._labelValue
+                        case "[@libName]":
+                            self._labelName = "libName"
+                            self._labelValue = self.parentItem().libraryName
+                            self._labelText = self._labelValue
+                        case "[@viewName]":
+                            self._viewName = "viewName"
+                            self._labelValue = self.parentItem().viewName
+                            self._labelText = self._labelValue
+                        case "[@modelName]":
+                            self._labelName = "modelName"
+                            self._labelValue = self.parentItem().attr.get("modelName", "")
+                            self._labelText = self._labelValue
+                        case "[@elementNum]":
+                            self._labelName = "elementNum"
+                            self._labelValue = f"{self.parentItem().counter}"
+                            self._labelText = self._labelValue
+                else:
+                    labelFields = (
+                        self._labelDefinition.lstrip("[@").rstrip("]").rstrip(":").split(
+                            ":"))
+                    self._labelName = labelFields[0].strip()
+                    match len(labelFields):
+                        case 1:
+                            if not self._labelValueSet:
+                                self._labelValue = "?"
+                            self._labelText = self._labelValue
+                        case 2:
+                            if self._labelValueSet:
+                                self._labelText = (
+                                    labelFields[1].strip().replace("%", self._labelValue))
+                            else:
+                                self._labelValue = "?"
+                        case 3:
+                            tempLabelValue = (
+                                labelFields[2].strip().split("=")[-1].split()[-1])
+                            if self.labelValueSet:
+                                self._labelText = labelFields[2].replace(tempLabelValue,
+                                    self._labelValue)
+                            else:
+                                self._labelText = labelFields[2]
+                                self._labelValue = tempLabelValue
+
+            except Exception as e:
+                if self.scene():
+                    self.scene().logger.error(e)
+        elif self._labelType == label.labelTypes[2]:  # pyLabel
+            try:
+                labelFields = self._labelDefinition.strip().split("=")
+                self._labelName = labelFields[0].strip()
+                labelFunction = labelFields[1].strip()
+                # pass the PDK callback class named with "cellName" the labels
+                # dictionary of instance.w
+                expression = (
+                    f"cb.{self.parentItem().cellName}(self.parentItem().labels).{labelFunction}")
+                self._labelValue = Quantity(eval(expression)).render(prec=3)
+                self._labelText = f"{self._labelName}={self._labelValue}"
+            except Exception as e:
+                if self.scene():
+                    self.scene().logger.error(e)
+
+
+class symbolShape(shape):
+    def __init__(self, pen: QPen, gridTuple: tuple, shapes: list, attr: dict):
+        super().__init__(pen, gridTuple)
+        assert shapes is not None  # must not be an empty list
+        self.shapes = shapes  # list of shapes in the symbol
+        self.attr = attr  # parameters common to all instances of symbol
+        self._counter = 0  # item's number on schematic
+        self._libraryName = ""
+        self._cellName = ""
+        self._viewName = ""
+        self._instanceName = ""
+        self._netlistLine = ""
+        # self._simViewName = None
+        self._angle = 0.0
+        self._drawings = list()
+        self._labels = dict()  # dict of labels
+        self._pins = dict()  # dict of pins
+        self._netlistIgnore = False
+        self.pinLocations = dict()  # pinName: pinRect
+        self.pinNetMap = dict()  # pinName: netName
+        self.pinNetTupleList = list()  # list of pinNetTuple
+        for item in self.shapes:
+            item.setFlag(QGraphicsItem.ItemIsSelectable, False)
+            item.setFlag(QGraphicsItem.ItemStacksBehindParent, True)
+            item.setParentItem(self)
+            if type(item) is pin:
+                self._pins[item.pinName] = item
+            elif type(item) is label:
+                self._labels[item.labelName] = item
+            else:
+                self._drawings.append(item)
+        self.setFiltersChildEvents(True)
+        self.setHandlesChildEvents(True)
+        self.setFlag(QGraphicsItem.ItemContainsChildrenInShape, True)
+        self.borderRect = self._drawings[0].sceneBoundingRect()
+        if self._drawings[1:]:
+            for draw in self._drawings[1:]:
+                self.borderRect = self.borderRect.united(draw.sceneBoundingRect())
+        self.dashLines = dict()
+
+    def __repr__(self):
+        return (f"symbolShape(name={self.cellName}, scene position= {self.scenePos()}, "
+                f"pins = {self.pins}, labels = {self.labels}, ")
+
+    def paint(self, painter, option, widget):
+        if self.isSelected():
+            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
+            painter.drawRect(self.borderRect)
+        if self.netlistIgnore:
+            painter.setPen(QPen(Qt.red, 5, Qt.SolidLine))
+            painter.drawLine(self.borderRect.bottomLeft(), self.borderRect.topRight())
+            painter.drawLine(self.borderRect.topLeft(), self.borderRect.bottomRight())
+
+    def boundingRect(self):
+        return self.childrenBoundingRect()
+
+    def sceneEvent(self, event):
+        try:  # if net is being drawn, do not accept any event.
+            if self.scene().drawWire:
+                return False
+            else:
+                super().sceneEvent(event)
+                return True
+        except AttributeError:
+            return False
+
+    def itemChange(self, change, value):
+
+        if self.scene() and change == QGraphicsItem.ItemPositionHasChanged:
+            # item's position has changed
+            # do something here
+            for item in self.pinNetTupleList:
+                if item.start == 1:
+                    item.net.start = item.pin.mapToScene(item.pin.start)
+                elif item.start == 0:
+                    item.net.end = item.pin.mapToScene(item.pin.start)
+
+        return super().itemChange(change, value)
+
+    def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        self.pinNetTupleList = list()
+        # create a named tuple to record whether the pin is located at the start or at
+        # the end of the net.
+        pins = [item for item in self.pins.values()]
+        for pinItem in pins:
+            for pinNet in self.scene().items(
+                    pinItem.sceneBoundingRect().adjusted(-2, -2, 2, 2),
+                    Qt.IntersectsItemShape):
+                if isinstance(pinNet, net.schematicNet):
+                    if pinItem.sceneBoundingRect().adjusted(-2, -2, 2, 2).contains(
+                            pinNet.mapToScene(pinNet.start)):
+                        self.pinNetTupleList.append(ddef.pinNetTuple(pinItem, pinNet, 1))
+                    elif pinItem.sceneBoundingRect().adjusted(-2, -2, 2, 2).contains(
+                            pinNet.mapToScene(pinNet.end)):
+                        self.pinNetTupleList.append(ddef.pinNetTuple(pinItem, pinNet, 0))
+        for item in self.pinNetTupleList:
+            pinSceneLoc = item.pin.mapToScene(item.pin.start)
+            if item.start == 1:
+                item.net.start = pinSceneLoc
+            else:
+                item.net.end = pinSceneLoc
+            item.net.pen = self.scene().otherPen
+        super().mousePressEvent(event)
+
+    def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mouseReleaseEvent(event)
+
+        for item in self.pinNetTupleList:
+            lines = self.scene().addWires(item.net.start, self.scene().wirePen)
+            self.scene().extendWires(lines, item.net.start, item.net.end)
+            self.scene().pruneWires(lines, self.scene().wirePen)
+            self.scene().removeItem(item.net)
+
+    @property
+    def libraryName(self):
+        return self._libraryName
+
+    @libraryName.setter
+    def libraryName(self, value):
+        self._libraryName = value
+
+    @property
+    def cellName(self):
+        return self._cellName
+
+    @cellName.setter
+    def cellName(self, value: str):
+        self._cellName = value
+
+    @property
+    def viewName(self):
+        return self._viewName
+
+    @viewName.setter
+    def viewName(self, value: str):
+        self._viewName = value
+
+    @property
+    def instanceName(self):
+        return self._instanceName
+
+    @instanceName.setter
+    def instanceName(self, value: str):
+        '''
+        If instance name is changed and [@instName] label exists, change it too.
+        '''
+        self._instanceName = value
+        if self.labels.get('instanceName', None):
+            self.labels['instanceName'].labelValue = value
+            self.labels['instanceName'].labelValueSet = True
+            self.labels['instanceName'].update()
+
+    @property
+    def counter(self) -> int:
+        return self._counter
+
+    @counter.setter
+    def counter(self, value: int):
+        assert isinstance(value, int)
+        self._counter = value
+
+    @property
+    def angle(self):
+        return self._angle
+
+    @angle.setter
+    def angle(self, value: float):
+        self.setRotation(value)
+        self._angle = value
+
+    @property
+    def labels(self):
+        return self._labels  # dictionary
+
+    @property
+    def pins(self):
+        return self._pins
+
+    @property
+    def drawings(self):
+        return self._drawings
+
+    @property
+    def netlistIgnore(self) -> bool:
+        return self._netlistIgnore
+
+    @netlistIgnore.setter
+    def netlistIgnore(self, value: bool):
+        self._netlistIgnore = value
+
+
+class schematicPin(shape):
+    """
+    schematic pin class.
+    """
+
+    pinDirs = ["Input", "Output", "Inout"]
+    pinTypes = ["Signal", "Ground", "Power", "Clock", "Digital", "Analog"]
+
+    def __init__(self, start: QPoint, pen: QPen, pinName, pinDir, pinType,
+                 gridTuple: tuple):
+        super().__init__(pen, gridTuple)
+        self._start = start
+        self._pinName = pinName
+        self._pinDir = pinDir
+        self._pinType = pinType
+        self._netTupleSet = set()
+
+    def __repr__(self):
+        return f"schematicPin({self._start}, {self._pen}, {self._pinName}, {self._pinDir}, {self._pinType})"
+
+    def paint(self, painter, option, widget):
+
+        painter.setPen(self._pen)
+        painter.setBrush(self._pen.color())
+        painter.setFont(QFont("Arial", 12))
+        match self.pinDir:
+            case "Input":
+                painter.drawPolygon([QPoint(self._start.x() - 10, self._start.y() - 10),
+                                     QPoint(self._start.x() + 10, self._start.y() - 10),
+                                     QPoint(self._start.x() + 20, self._start.y()),
+                                     QPoint(self._start.x() + 10, self._start.y() + 10),
+                                     QPoint(self._start.x() - 10, self._start.y() + 10), ])
+            case "Output":
+                painter.drawPolygon([QPoint(self._start.x() - 20, self._start.y()),
+                                     QPoint(self._start.x() - 10, self._start.y() - 10),
+                                     QPoint(self._start.x() + 10, self._start.y() - 10),
+                                     QPoint(self._start.x() + 10, self._start.y() + 10),
+                                     QPoint(self._start.x() - 10, self._start.y() + 10), ])
+            case "Inout":
+                painter.drawPolygon([QPoint(self._start.x() - 20, self._start.y()),
+                                     QPoint(self._start.x() - 10, self._start.y() - 10),
+                                     QPoint(self._start.x() + 10, self._start.y() - 10),
+                                     QPoint(self._start.x() + 20, self._start.y()),
+                                     QPoint(self._start.x() + 10, self._start.y() + 10),
+                                     QPoint(self._start.x() - 10, self._start.y() + 10), ])
+        painter.drawText(self._start.x(), self._start.y() - 20, self.pinName)
+        if self.isSelected():
+            painter.setPen(QPen(Qt.yellow, 2, Qt.DashLine))
+            # painter.setBrush(Qt.yellow)
+            painter.drawRect(QRect.span(QPoint(self._start.x() - 10, self._start.y() - 10),
+                                        QPoint(self._start.x() + 10,
+                                               self._start.y() + 10), ))
+
+    def boundingRect(self):
+        return QRect(self._start.x() - 10, self._start.y() - 10, 30, 20).adjusted(-5, -10,
+            5, 5)
+
+    def sceneEvent(self, event):
+        if self.scene().drawWire:
+            return False
+        else:
+            super().sceneEvent(event)
+            return True
+
+    #
+    def mousePressEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mousePressEvent(event)
+        # create a named tuple to record whether the pin is located at the start or at
+        # the end of the net.
+
+        for pinNet in self.scene().items(self.sceneBoundingRect().adjusted(-2, -2, 2, 2),
+                Qt.IntersectsItemShape):
+            if isinstance(pinNet, net.schematicNet):
+                if self.sceneBoundingRect().adjusted(-2, -2, 2, 2).contains(
+                        pinNet.mapToScene(pinNet.start)):
+                    self._netTupleSet.add(ddef.netTuple(pinNet, 1))
+                elif self.sceneBoundingRect().adjusted(-2, -2, 2, 2).contains(
+                        pinNet.mapToScene(pinNet.end)):
+                    self._netTupleSet.add(ddef.netTuple(pinNet, 0))
+        for item in self._netTupleSet:
+            pinSceneLoc = self.mapToScene(self.start)
+            if item.start == 1:
+                item.net.start = pinSceneLoc
+            else:
+                item.net.end = pinSceneLoc
+            item.net.pen = self.scene().otherPen
+        super().mousePressEvent(event)
+
+    #
+    def mouseReleaseEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+        super().mouseReleaseEvent(event)
+
+        for item in self._netTupleSet:
+            lines = self.scene().addWires(item.net.start, self.scene().wirePen)
+            self.scene().extendWires(lines, item.net.start, item.net.end)
+            self.scene().pruneWires(lines, self.scene().wirePen)
+            self.scene().removeItem(item.net)
+        self._netTupleSet = set()
+
+    def itemChange(self, change, value):
+
+        if self.scene() and change == QGraphicsItem.ItemPositionHasChanged:
+            # item's position has changed
+            # do something here
+            for item in self._netTupleSet:
+                if item.start == 1:
+                    item.net.start = self.mapToScene(self.start)
+                elif item.start == 0:
+                    item.net.end = self.mapToScene(self.start)
+        return super().itemChange(change, value)
+
+    # def mouseMoveEvent(self, event: QGraphicsSceneMouseEvent) -> None:
+    #     super().mouseMoveEvent(event)
+    #     self.setPos(event.scenePos() - event.buttonDownPos(Qt.LeftButton))
+
+    def toSymbolPin(self, start: QPoint, pen: QPen, gridTuple: tuple):
+        return pin(start, pen, self.pinName, self.pinDir, self.pinType, gridTuple)
+
+    @property
+    def start(self):
+        return self._start
+
+    @start.setter
+    def start(self, start):
+        self._start = start
+
+    @property
+    def pinName(self):
+        return self._pinName
+
+    @pinName.setter
+    def pinName(self, pinName):
+        if pinName != "":
+            self._pinName = pinName
+
+    @property
+    def pinDir(self):
+        return self._pinDir
+
+    @pinDir.setter
+    def pinDir(self, direction: str):
+        if direction in self.pinDirs:
+            self._pinDir = direction
+
+    @property
+    def pinType(self):
+        return self._pinType
+
+    @pinType.setter
+    def pinType(self, pintype: str):
+        if pintype in self.pinTypes:
+            self._pinType = pintype
```

### Comparing `revolution-eda-0.5.1/revedaEditor/fileio/__init__.py` & `revolution-eda-0.5.2/revedaEditor/backend/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
-
+
+#   “Commons Clause” License Condition v1.0
+#  #
+#   The Software is provided to you by the Licensor under the License, as defined
+#   below, subject to the following condition.
+#  #
+#   Without limiting other conditions in the License, the grant of rights under the
+#   License will not include, and the License does not grant to you, the right to
+#   Sell the Software.
+#  #
+#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#   granted to you under the License to provide to third parties, for a fee or other
+#   consideration (including without limitation fees for hosting or consulting/
+#   support services related to the Software), a product or service whose value
+#   derives, entirely or substantially, from the functionality of the Software. Any
+#   license notice or attribution required by the License must also include this
+#   Commons Clause License Condition notice.
+#  #
+#   Software: Revolution EDA
+#   License: Mozilla Public License 2.0
+#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
```

### Comparing `revolution-eda-0.5.1/revedaEditor/fileio/loadJSON.py` & `revolution-eda-0.5.2/revedaEditor/fileio/loadJSON.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,16 @@
                 print("Error: Invalid Symbol file")
         symbolInstance = shp.symbolShape(draftPen, gridTuple, itemShapes,
                                          symbolAttributes)
         symbolInstance.libraryName = item["lib"]
         symbolInstance.cellName = item["cell"]
         symbolInstance.counter = instCounter
         symbolInstance.instanceName = item["nam"]
-        symbolInstance.angle = item["ang"]
+        symbolInstance.angle = item.get("ang", 0)
+        symbolInstance.netlistIgnore = bool(item.get("ign",0))
         symbolInstance.viewName = viewName
         symbolInstance.attributes = symbolAttributes
         for labelItem in symbolInstance.labels.values():
             if labelItem.labelName in labelDict.keys():
                 labelItem.labelValue = labelDict[labelItem.labelName][0]
                 labelItem.labelVisible = labelDict[labelItem.labelName][1]
         symbolInstance.setPos(item["loc"][0], item["loc"][1])
```

### Comparing `revolution-eda-0.5.1/revedaEditor/fileio/symbolEncoder.py` & `revolution-eda-0.5.2/revedaEditor/fileio/symbolEncoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
                 item.labelName: [item.labelValue, item.labelVisible] for item in
                 item.labels.values()}
             itemDict = {"type": "symbolShape", "lib": item.libraryName,
                         "cell": item.cellName, "view": item.viewName,
                         "nam": item.instanceName, "ic": item.counter,
                         "ld": itemLabelDict, "loc": (
                             item.scenePos() - item.scene().origin).toTuple(),
-                        "ang": item.angle, }
+                        "ang": item.angle, "ign": int(item.netlistIgnore) }
             return itemDict
         elif isinstance(item, net.schematicNet):
             itemDict = {"type": "schematicNet", "st": item.start.toTuple(),
                         "end": item.end.toTuple(), "pen": item.pen.pname,
                         "loc": (item.scenePos() - item.scene().origin).toTuple(),
                         "nam": item.name, "ns": item.nameSet, }
             return itemDict
```

### Comparing `revolution-eda-0.5.1/revedaEditor/gui/__init__.py` & `revolution-eda-0.5.2/revedaEditor/gui/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
+#   “Commons Clause” License Condition v1.0
+#  #
+#   The Software is provided to you by the Licensor under the License, as defined
+#   below, subject to the following condition.
+#  #
+#   Without limiting other conditions in the License, the grant of rights under the
+#   License will not include, and the License does not grant to you, the right to
+#   Sell the Software.
+#  #
+#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#   granted to you under the License to provide to third parties, for a fee or other
+#   consideration (including without limitation fees for hosting or consulting/
+#   support services related to the Software), a product or service whose value
+#   derives, entirely or substantially, from the functionality of the Software. Any
+#   license notice or attribution required by the License must also include this
+#   Commons Clause License Condition notice.
+#  #
+#   Software: Revolution EDA
+#   License: Mozilla Public License 2.0
+#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
```

### Comparing `revolution-eda-0.5.1/revedaEditor/gui/editFunctions.py` & `revolution-eda-0.5.2/revedaEditor/gui/editFunctions.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-
-
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
-from PySide6.QtCore import (Qt, )
-from PySide6.QtWidgets import (QLineEdit, QLabel, QWidget)
-
-class shortLineEdit(QLineEdit):
-    def __init__(self):
-        super().__init__(None)
-        self.setMaximumWidth(80)
-
-
-class boldLabel(QLabel):
-    def __init__(self, text: str, parent: QWidget = None):
-        super().__init__(text, parent)
-        self.setTextFormat(Qt.RichText)
-        self.setText("<b>" + text + "</b>")
-
-
-class longLineEdit(QLineEdit):
-    def __init__(self):
-        super().__init__(None)
-        self.setMaximumWidth(500)
+
+
+#   “Commons Clause” License Condition v1.0
+#  #
+#   The Software is provided to you by the Licensor under the License, as defined
+#   below, subject to the following condition.
+#  #
+#   Without limiting other conditions in the License, the grant of rights under the
+#   License will not include, and the License does not grant to you, the right to
+#   Sell the Software.
+#  #
+#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#   granted to you under the License to provide to third parties, for a fee or other
+#   consideration (including without limitation fees for hosting or consulting/
+#   support services related to the Software), a product or service whose value
+#   derives, entirely or substantially, from the functionality of the Software. Any
+#   license notice or attribution required by the License must also include this
+#   Commons Clause License Condition notice.
+#  #
+#   Software: Revolution EDA
+#   License: Mozilla Public License 2.0
+#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
+from PySide6.QtCore import (Qt, )
+from PySide6.QtWidgets import (QLineEdit, QLabel, QWidget)
+
+class shortLineEdit(QLineEdit):
+    def __init__(self):
+        super().__init__(None)
+        self.setMaximumWidth(80)
+
+
+class boldLabel(QLabel):
+    def __init__(self, text: str, parent: QWidget = None):
+        super().__init__(text, parent)
+        self.setTextFormat(Qt.RichText)
+        self.setText("<b>" + text + "</b>")
+
+
+class longLineEdit(QLineEdit):
+    def __init__(self):
+        super().__init__(None)
+        self.setMaximumWidth(500)
```

### Comparing `revolution-eda-0.5.1/revedaEditor/gui/editorWindows.py` & `revolution-eda-0.5.2/revedaEditor/gui/editorWindows.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,28 +27,28 @@
 import shutil
 from copy import deepcopy
 import os
 # if os.environ.get('REVEDASIM_PATH'):
 #     import revedasim.simMainWindow as smw
 
 # import numpy as np
-from PySide6.QtCore import (QEvent, QMargins, QPoint, QPointF, QProcess, QRect,
-                            QRectF, QRunnable, Qt, Slot)
-from PySide6.QtGui import (QAction, QCloseEvent, QColor, QCursor, QFont,
-                           QGuiApplication, QIcon, QImage, QKeySequence, QPainter,
-                           QPen, QStandardItem, QStandardItemModel, QTextDocument,
-                           QUndoStack)
+from PySide6.QtCore import (QEvent, QMargins, QPoint, QPointF, QProcess, QRect, QRectF,
+                            QRunnable, Qt, Slot)
+from PySide6.QtGui import (QAction, QCloseEvent, QColor, QCursor,
+                           QGuiApplication,
+                           QIcon, QImage, QKeySequence, QPainter, QPen, QStandardItem,
+                           QStandardItemModel, QTextDocument, QUndoStack)
 from PySide6.QtPrintSupport import (QPrintDialog, QPrinter, QPrintPreviewDialog)
-from PySide6.QtWidgets import (QAbstractItemView, QApplication, QComboBox,
-                               QDialog, QFileDialog, QFormLayout,
+from PySide6.QtWidgets import (QAbstractItemView, QApplication, QComboBox, QDialog,
+                                QGraphicsItem, QFileDialog, QFormLayout,
                                QGraphicsRectItem, QGraphicsScene,
-                               QGraphicsSceneMouseEvent, QGraphicsView,
-                               QGridLayout, QGroupBox, QLabel, QMainWindow, QMenu,
-                               QMessageBox, QTableView, QToolBar, QTreeView,
-                               QVBoxLayout, QWidget)
+                               QGraphicsSceneMouseEvent, QGraphicsView, QGridLayout,
+                               QGroupBox, QLabel, QMainWindow, QMenu, QMessageBox,
+                               QTableView, QToolBar, QTreeView, QVBoxLayout, QWidget,
+                               )
 
 import revedaEditor.backend.dataDefinitions as ddef
 import revedaEditor.backend.libraryMethods as libm
 import revedaEditor.backend.schBackEnd as scb
 import revedaEditor.backend.undoStack as us
 import revedaEditor.common.layers as cel
 import revedaEditor.common.net as net
@@ -57,14 +57,15 @@
 import revedaEditor.fileio.loadJSON as lj
 import revedaEditor.fileio.symbolEncoder as se
 import revedaEditor.gui.editFunctions as edf
 import revedaEditor.gui.fileDialogues as fd
 import revedaEditor.gui.propertyDialogues as pdlg
 import revedaEditor.resources.resources
 
+
 class editorWindow(QMainWindow):
     """
     Base class for editor windows.
     """
 
     def __init__(self, viewItem: scb.viewItem, libraryDict: dict,
                  libraryView):  # file is a pathlib.Path object
@@ -116,24 +117,27 @@
         self.menuWindow = self.editorMenuBar.addMenu("&Window")
         self.menuUtilities = self.editorMenuBar.addMenu("&Utilities")
 
     def _createActions(self):
         checkCellIcon = QIcon(":/icons/document-task.png")
         self.checkCellAction = QAction(checkCellIcon, "Check-Save", self)
 
+        saveCellIocn = QIcon(":/icons/document--plus.png")
+        self.saveCellAction = QAction(saveCellIocn, "Save", self)
+
         self.readOnlyCellIcon = QIcon(":/icons/lock.png")
-        self.readOnlyCellAction = QAction(self.readOnlyCellIcon, "Make Read Only",
-                                          self)
+        self.readOnlyCellAction = QAction("Read Only", self)
+        self.readOnlyCellAction.setCheckable(True)
+
 
         printIcon = QIcon(":/icons/printer--arrow.png")
         self.printAction = QAction(printIcon, "Print...", self)
 
         printPreviewIcon = QIcon(":/icons/printer--arrow.png")
-        self.printPreviewAction = QAction(printPreviewIcon, "Print Preview...",
-                                          self)
+        self.printPreviewAction = QAction(printPreviewIcon, "Print Preview...", self)
 
         exportImageIcon = QIcon(":/icons/image-export.png")
         self.exportImageAction = QAction(exportImageIcon, "Export...", self)
 
         exitIcon = QIcon(":/icons/external.png")
         self.exitAction = QAction(exitIcon, "Close Window", self)
         self.exitAction.setShortcut("Ctrl+Q")
@@ -161,20 +165,18 @@
         # self.menuView.addAction(self.delRulerAction)
 
         # display options
         dispConfigIcon = QIcon(":/icons/resource-monitor.png")
         self.dispConfigAction = QAction(dispConfigIcon, "Display Config...", self)
 
         selectConfigIcon = QIcon(":/icons/zone-select.png")
-        self.selectConfigAction = QAction(selectConfigIcon, "Selection Config...",
-                                          self)
+        self.selectConfigAction = QAction(selectConfigIcon, "Selection Config...", self)
 
         panZoomConfigIcon = QIcon(":/icons/selection-resize.png")
-        self.panZoomConfigAction = QAction(panZoomConfigIcon,
-                                           "Pan/Zoom Config...", self)
+        self.panZoomConfigAction = QAction(panZoomConfigIcon, "Pan/Zoom Config...", self)
 
         undoIcon = QIcon(":/icons/arrow-circle-315-left.png")
         self.undoAction = QAction(undoIcon, "Undo", self)
 
         redoIcon = QIcon(":/icons/arrow-circle-225.png")
         self.redoAction = QAction(redoIcon, "Redo", self)
 
@@ -230,73 +232,70 @@
         deselectAllIcon = QIcon(":/icons/node.png")
         self.deselectAllAction = QAction(deselectAllIcon, "Unselect All", self)
 
         objPropIcon = QIcon(":/icons/property-blue.png")
         self.objPropAction = QAction(objPropIcon, "Object Properties...", self)
 
         viewPropIcon = QIcon(":/icons/property.png")
-        self.viewPropAction = QAction(viewPropIcon, "Cellview Properties...",
-                                      self)
+        self.viewPropAction = QAction(viewPropIcon, "Cellview Properties...", self)
 
         viewCheckIcon = QIcon(":/icons/ui-check-box.png")
         self.viewCheckAction = QAction(viewCheckIcon, "Check CellView", self)
 
         viewErrorsIcon = QIcon(":/icons/report--exclamation.png")
         self.viewErrorsAction = QAction(viewErrorsIcon, "View Errors...", self)
 
         deleteErrorsIcon = QIcon(":/icons/report--minus.png")
-        self.deleteErrorsAction = QAction(deleteErrorsIcon, "Delete Errors...",
-                                          self)
+        self.deleteErrorsAction = QAction(deleteErrorsIcon, "Delete Errors...", self)
 
         netlistIcon = QIcon(":/icons/script-text.png")
         self.netlistAction = QAction(netlistIcon, "Create Netlist...", self)
 
         simulateIcon = QIcon(":/icons/application-wave.png")
         self.simulateAction = QAction(simulateIcon, "Run RevEDA Sim GUI", self)
 
         createLineIcon = QIcon(":/icons/layer-shape-line.png")
         self.createLineAction = QAction(createLineIcon, "Create Line...", self)
 
         createRectIcon = QIcon(":/icons/layer-shape.png")
-        self.createRectAction = QAction(createRectIcon, "Create Rectangle...",
-                                        self)
+        self.createRectAction = QAction(createRectIcon, "Create Rectangle...", self)
 
         createPolyIcon = QIcon(":/icons/layer-shape-polygon.png")
         self.createPolyAction = QAction(createPolyIcon, "Create Polygon...", self)
 
         createCircleIcon = QIcon(":/icons/layer-shape-ellipse.png")
-        self.createCircleAction = QAction(createCircleIcon, "Create Circle...",
-                                          self)
+        self.createCircleAction = QAction(createCircleIcon, "Create Circle...", self)
 
         createArcIcon = QIcon(":/icons/layer-shape-polyline.png")
         self.createArcAction = QAction(createArcIcon, "Create Arc...", self)
 
         createInstIcon = QIcon(":/icons/block--plus.png")
-        self.createInstAction = QAction(createInstIcon, "Create Instance...",
-                                        self)
+        self.createInstAction = QAction(createInstIcon, "Create Instance...", self)
 
         createWireIcon = QIcon(":/icons/node-insert.png")
         self.createWireAction = QAction(createWireIcon, "Create Wire...", self)
 
         createBusIcon = QIcon(":/icons/node-select-all.png")
         self.createBusAction = QAction(createBusIcon, "Create Bus...", self)
 
         createLabelIcon = QIcon(":/icons/tag-label-yellow.png")
         self.createLabelAction = QAction(createLabelIcon, "Create Label...", self)
 
         createPinIcon = QIcon(":/icons/pin--plus.png")
         self.createPinAction = QAction(createPinIcon, "Create Pin...", self)
 
         createSymbolIcon = QIcon(":/icons/application-block.png")
-        self.createSymbolAction = QAction(createSymbolIcon, "Create Symbol...",
-                                          self)
+        self.createSymbolAction = QAction(createSymbolIcon, "Create Symbol...", self)
 
         createTextIcon = QIcon(":icons/sticky-note-text.png")
         self.createTextAction = QAction(createTextIcon, "Create Text...", self)
 
+        ignoreIcon = QIcon(":/icons/minus-circle.png")
+        self.ignoreAction = QAction(ignoreIcon, "Ignore", self)
+
     def _createToolBars(self):
         # Create tools bar called "main toolbar"
         self.toolbar = QToolBar("Main Toolbar", self)
         # place toolbar at top
         self.addToolBar(self.toolbar)
         self.toolbar.addAction(self.printAction)
         self.toolbar.addAction(self.exportImageAction)
@@ -315,15 +314,15 @@
         self.toolbar.addAction(self.zoomOutAction)
         self.toolbar.addSeparator()
         self.toolbar.addAction(self.objPropAction)
 
     def _addActions(self):
         # file menu
         self.menuFile.addAction(self.checkCellAction)
-        self.menuFile.addAction(self.readOnlyCellAction)
+        self.menuFile.addAction(self.saveCellAction)
         self.menuFile.addAction(self.printAction)
         self.menuFile.addAction(self.printPreviewAction)
         self.menuFile.addAction(self.exportImageAction)
         self.menuFile.addAction(self.exitAction)
         # view menu
         self.menuView.addAction(self.fitAction)
         self.menuView.addAction(self.zoomInAction)
@@ -341,18 +340,19 @@
         self.menuEdit.addAction(self.deleteAction)
         self.menuEdit.addAction(self.copyAction)
         self.menuEdit.addAction(self.moveAction)
         self.menuEdit.addAction(self.moveByAction)
         self.menuEdit.addAction(self.moveOriginAction)
         self.menuEdit.addAction(self.stretchAction)
         self.menuEdit.addAction(self.rotateAction)
-
+        self.menuTools.addAction(self.readOnlyCellAction)
         self.menuCheck.addAction(self.viewCheckAction)
 
     def _createTriggers(self):
+        self.readOnlyCellAction.triggered.connect(self.readOnlyCellClick)
         self.printAction.triggered.connect(self.printClick)
         self.printPreviewAction.triggered.connect(self.printPreviewClick)
         self.exportImageAction.triggered.connect(self.imageExportClick)
         self.exitAction.triggered.connect(self.closeWindow)
         self.fitAction.triggered.connect(self.fitToWindow)
         self.zoomInAction.triggered.connect(self.zoomIn)
         self.zoomOutAction.triggered.connect(self.zoomOut)
@@ -396,37 +396,39 @@
     def selectConfigEdit(self):
         scd = pdlg.selectConfigDialogue(self)
         if self.centralW.scene.partialSelection:
             scd.partialSelection.setChecked(True)
         else:
             scd.fullSelection.setChecked(True)
         if scd.exec() == QDialog.Accepted:
-            if scd.partialSelection.isChecked():
-                self.centralW.scene.partialSelection = True
-            else:
-                self.centralW.scene.partialSelection = False
+            self.centralW.scene.partialSelection = scd.partialSelection.isChecked()
+            # if scd.partialSelection.isChecked():
+            #     self.centralW.scene.partialSelection = True
+            # else:
+            #     self.centralW.scene.partialSelection = False
+
+    def readOnlyCellClick(self):
+        self.centralW.scene.readOnly = self.readOnlyCellAction.isChecked()
+
 
     def printClick(self):
         dlg = QPrintDialog(self)
         if dlg.exec() == QDialog.Accepted:
             printer = dlg.printer()
             printRunner = startThread(self.centralW.view.printView(printer))
             self.appMainW.threadPool.start(printRunner)
-            self.logger.info('Printing started')
-            # self.centralW.view.printView(printer)
+            self.logger.info('Printing started')  # self.centralW.view.printView(printer)
 
     def printPreviewClick(self):
         printer = QPrinter(QPrinter.ScreenResolution)
         printer.setOutputFormat(QPrinter.PdfFormat)
         ppdlg = QPrintPreviewDialog(self)
         ppdlg.paintRequested.connect(self.centralW.view.printView)
         ppdlg.exec()
 
-
-
     def imageExportClick(self):
         image = QImage(self.centralW.view.viewport().size(),
                        QImage.Format_ARGB32_Premultiplied)
         self.centralW.view.printView(image)
         fdlg = QFileDialog(self, caption="Select or create an image file")
         fdlg.setDefaultSuffix("png")
         fdlg.setFileMode(QFileDialog.AnyFile)
@@ -463,19 +465,17 @@
         pass
 
     def moveOrigin(self):
         self.centralW.scene.changeOrigin = True
 
 
 class schematicEditor(editorWindow):
-    def __init__(self, viewItem: scb.viewItem, libraryDict: dict,
-                 libraryView) -> None:
+    def __init__(self, viewItem: scb.viewItem, libraryDict: dict, libraryView) -> None:
         super().__init__(viewItem, libraryDict, libraryView)
-        self.setWindowTitle(
-            f"Schematic Editor - {self.cellName} - {self.viewName}")
+        self.setWindowTitle(f"Schematic Editor - {self.cellName} - {self.viewName}")
         self.setWindowIcon(QIcon(":/icons/layer-shape.png"))
         self.configDict = dict()
         self.processedCells = set()  # cells included in config view
         self.symbolChooser = None
         self.cellViews = [
             "symbol"]  # only symbol can be instantiated in the schematic window.
         self._schematicActions()
@@ -484,32 +484,44 @@
         self.resize(1600, 800)
         self._createMenuBar()
         self._createToolBars()
         # create container to position all widgets
         self.centralW = schematicContainer(self)
         self.setCentralWidget(self.centralW)
 
+    def _createActions(self):
+
+        super()._createActions()
+        self.netNameAction = QAction("Net Name", self)
+        self.netNameAction.setShortcut("l")
+        self.hilightNetAction = QAction("Highlight Net", self)
+        self.hilightNetAction.setCheckable(True)
+
     def _createTriggers(self):
         super()._createTriggers()
-        self.checkCellAction.triggered.connect(self.checkSaveCell)
+        self.checkCellAction.triggered.connect(self.checkSaveCellClick)
+        self.saveCellAction.triggered.connect(self.saveCellClick)
         self.createWireAction.triggered.connect(self.createWireClick)
         self.createInstAction.triggered.connect(self.createInstClick)
         self.createPinAction.triggered.connect(self.createPinClick)
         self.createTextAction.triggered.connect(self.createNoteClick)
         self.createSymbolAction.triggered.connect(self.createSymbolClick)
         self.copyAction.triggered.connect(self.copyClick)
         self.deleteAction.triggered.connect(self.deleteClick)
         self.objPropAction.triggered.connect(self.objPropClick)
         self.undoAction.triggered.connect(self.undoClick)
         self.redoAction.triggered.connect(self.redoClick)
         self.netlistAction.triggered.connect(self.createNetlistClick)
         self.rotateAction.triggered.connect(self.rotateItemClick)
         self.simulateAction.triggered.connect(self.startSimClick)
+        self.ignoreAction.triggered.connect(self.ignoreClick)
         self.goDownAction.triggered.connect(self.goDownClick)
         self.goUpAction.triggered.connect(self.goUpClick)
+        self.hilightNetAction.triggered.connect(self.hilightNetClick)
+        self.netNameAction.triggered.connect(self.netNameClick)
 
     def _createMenuBar(self):
         super()._createMenuBar()
         self.menuSimulation = self.editorMenuBar.addMenu("&Simulation")
         self.menuHelp = self.editorMenuBar.addMenu("&Help")
         self._addActions()
 
@@ -540,14 +552,20 @@
         self.menuCreate.addAction(self.createTextAction)
         self.menuCreate.addAction(self.createSymbolAction)
 
         # check menu
         self.menuCheck.addAction(self.viewErrorsAction)
         self.menuCheck.addAction(self.deleteErrorsAction)
 
+        # tools menu
+        self.menuTools.addAction(self.hilightNetAction)
+        self.menuTools.addAction(self.netNameAction)
+
+        # help menu
+
         self.menuSimulation.addAction(self.netlistAction)
         if self._app.revedasim_path:
             self.menuSimulation.addAction(self.simulateAction)
 
     def _createToolBars(self):
         super()._createToolBars()
         # toolbar.addAction(self.rulerAction)
@@ -561,32 +579,35 @@
         self.schematicToolbar.addAction(self.createWireAction)
         self.schematicToolbar.addAction(self.createBusAction)
         self.schematicToolbar.addAction(self.createPinAction)
         # self.schematicToolbar.addAction(self.createLabelAction)
         self.schematicToolbar.addAction(self.createSymbolAction)
         self.schematicToolbar.addSeparator()
         self.schematicToolbar.addAction(self.viewCheckAction)
+        self.schematicToolbar.addSeparator()
+        self.schematicToolbar.addAction(self.goDownAction)
+
 
     def _schematicActions(self):
         self.centralW.scene.itemContextMenu.addAction(self.copyAction)
         self.centralW.scene.itemContextMenu.addAction(self.moveAction)
         self.centralW.scene.itemContextMenu.addAction(self.rotateAction)
         self.centralW.scene.itemContextMenu.addAction(self.deleteAction)
         self.centralW.scene.itemContextMenu.addAction(self.objPropAction)
+        self.centralW.scene.itemContextMenu.addAction(self.ignoreAction)
         self.centralW.scene.itemContextMenu.addAction(self.goDownAction)
-        if self.parentView is not None:
-            self.centralW.scene.itemContextMenu.addAction(self.goUpAction)
 
     def _createShortcuts(self):
         super()._createShortcuts()
         self.createInstAction.setShortcut(Qt.Key_I)
         self.createWireAction.setShortcut(Qt.Key_W)
         self.createPinAction.setShortcut(Qt.Key_P)
         self.goDownAction.setShortcut("Shift+E")
 
+
     def dispConfigEdit(self):
         super().dispConfigEdit()
         self.centralW.view.majorGrid = self.majorGrid
         self.centralW.scene.majorGrid = self.majorGrid
         self.centralW.scene.gridTuple = (self.majorGrid, self.majorGrid)
         self.centralW.view.gridTuple = (self.majorGrid, self.majorGrid)
 
@@ -605,20 +626,17 @@
             self.symbolChooser.show()
         else:
             self.symbolChooser.raise_()
         if self.symbolChooser.exec() == QDialog.Accepted:
             self.centralW.scene.addInstance = True
             libItem = libm.getLibItem(libraryModel,
                                       self.symbolChooser.libNamesCB.currentText())
-            cellItem = libm.getCellItem(libItem,
-                                        self.symbolChooser.cellCB.currentText())
-            viewItem = libm.getViewItem(cellItem,
-                                        self.symbolChooser.viewCB.currentText())
-            self.centralW.scene.instanceSymbolFile = viewItem.data(
-                Qt.UserRole + 2)
+            cellItem = libm.getCellItem(libItem, self.symbolChooser.cellCB.currentText())
+            viewItem = libm.getViewItem(cellItem, self.symbolChooser.viewCB.currentText())
+            self.centralW.scene.instanceSymbolFile = viewItem.data(Qt.UserRole + 2)
 
     def createPinClick(self, s):
         createPinDlg = pdlg.createSchematicPinDialog(self)
         if createPinDlg.exec() == QDialog.Accepted:
             self.centralW.scene.pinName = createPinDlg.pinName.text()
             self.centralW.scene.pinType = createPinDlg.pinType.currentText()
             self.centralW.scene.pinDir = createPinDlg.pinDir.currentText()
@@ -655,15 +673,19 @@
         self.centralW.scene.itemSelect = False
 
     def startSimClick(self, s):
         import revedasim.simMainWindow as smw
         simguiw = smw.simMainWindow(self)
         simguiw.show()
 
-    def checkSaveCell(self):
+    def checkSaveCellClick(self):
+        self.centralW.scene.groupAllNets()
+        self.centralW.scene.saveSchematicCell(self.file)
+
+    def saveCellClick(self):
         self.centralW.scene.saveSchematicCell(self.file)
 
     def loadSchematic(self):
         with open(self.file) as tempFile:
             items = json.load(tempFile)
         self.centralW.scene.loadSchematicCell(items)
         sceneNetsSet = self.centralW.scene.findSceneNetsSet()
@@ -672,22 +694,19 @@
             netItem.findDotPoints()
 
     def createConfigView(self, configItem: scb.viewItem, configDict: dict,
                          newConfigDict: dict, processedCells: set):
 
         sceneSymbolSet = self.centralW.scene.findSceneSymbolSet()
         for item in sceneSymbolSet:
-            libItem = libm.getLibItem(self.libraryView.libraryModel,
-                                      item.libraryName)
+            libItem = libm.getLibItem(self.libraryView.libraryModel, item.libraryName)
             cellItem = libm.getCellItem(libItem, item.cellName)
-            viewItems = [cellItem.child(row) for row in
-                         range(cellItem.rowCount())]
+            viewItems = [cellItem.child(row) for row in range(cellItem.rowCount())]
             viewNames = [viewItem.viewName for viewItem in viewItems]
-            netlistableViews = [viewItemName for viewItemName in
-                                self.switchViewList if
+            netlistableViews = [viewItemName for viewItemName in self.switchViewList if
                                 viewItemName in viewNames]
             itemSwitchViewList = deepcopy(netlistableViews)
             viewDict = dict(zip(viewNames, viewItems))
             itemCellTuple = ddef.cellTuple(libItem.libraryName, cellItem.cellName)
             if itemCellTuple not in processedCells:
                 cellLine = configDict.get(cellItem.cellName)
                 if cellLine:
@@ -699,16 +718,15 @@
                                 cellItem.cellName: [libItem.libraryName, viewName,
                                                     itemSwitchViewList, ]})
                             schematicObj = schematicEditor(viewDict[viewName],
                                                            self.libraryDict,
                                                            self.libraryView, )
                             schematicObj.loadSchematic()
                             schematicObj.createConfigView(configItem, configDict,
-                                                          newConfigDict,
-                                                          processedCells)
+                                                          newConfigDict, processedCells)
                             break
                         case other:
                             newConfigDict.update({
                                 cellItem.cellName: [libItem.libraryName, viewName,
                                                     itemSwitchViewList, ]})
                             break
                 processedCells.add(itemCellTuple)
@@ -734,22 +752,20 @@
                 if configItems[1]['reference'] == self.viewItem.viewName:
                     netlistableViews.append(item.viewName)
         dlg.viewNameCombo.addItems(netlistableViews)
         if hasattr(self.appMainW, "simulationPath"):
             dlg.netlistDirEdit.setText(str(self.appMainW.simulationPath))
         if dlg.exec() == QDialog.Accepted:
             try:
-                self.appMainW.simulationPath = pathlib.Path(
-                    dlg.netlistDirEdit.text())
+                self.appMainW.simulationPath = pathlib.Path(dlg.netlistDirEdit.text())
                 selectedViewName = dlg.viewNameCombo.currentText()
                 self.switchViewList = [item.strip() for item in
                                        dlg.switchViewEdit.text().split(",")]
                 self.stopViewList = [dlg.stopViewEdit.text().strip()]
-                subDirPathObj = self.appMainW.simulationPath.joinpath(
-                    self.cellName)
+                subDirPathObj = self.appMainW.simulationPath.joinpath(self.cellName)
                 subDirPathObj.mkdir(parents=True, exist_ok=True)
                 netlistFilePathObj = subDirPathObj.joinpath(f'{self.cellName}_'
                                                             f'{selectedViewName}').with_suffix(
                     '.cir')
                 simViewName = dlg.viewNameCombo.currentText()
                 if 'schematic' in simViewName:
                     netlistObj = xyceNetlist(self, netlistFilePathObj)
@@ -771,14 +787,23 @@
 
     def goDownClick(self, s):
         self.centralW.scene.goDownHier()
 
     def goUpClick(self, s):
         self.centralW.scene.goUpHier()
 
+    def ignoreClick(self, s):
+        self.centralW.scene.ignoreSymbol()
+
+    def netNameClick(self, s):
+        self.centralW.scene.netNameEdit()
+
+    def hilightNetClick(self, s):
+        self.centralW.scene.hilightNets()
+
 
 class symbolEditor(editorWindow):
     def __init__(self, viewItem: scb.viewItem, libraryDict: dict, libraryView):
         super().__init__(viewItem, libraryDict, libraryView)
         self.setWindowTitle(f"Symbol Editor - {self.cellName} - {self.viewName}")
         self._symbolActions()
 
@@ -884,20 +909,20 @@
         self.centralW.scene.drawRect = args[3]  # draw rect
         self.centralW.scene.drawLine = args[4]  # draw line
         self.centralW.scene.addLabel = args[5]
         self.centralW.scene.drawCircle = args[6]
         self.centralW.scene.rotateItem = args[7]
 
     def createRectClick(self, s):
-        modeList = [False for i in range(8)]
+        modeList = [False for _ in range(8)]
         modeList[3] = True
         self.setDrawMode(*modeList)
 
     def createLineClick(self, s):
-        modeList = [False for i in range(8)]
+        modeList = [False for _ in range(8)]
         modeList[4] = True
         self.setDrawMode(*modeList)
 
     def createPolyClick(self, s):
         pass
 
     def createArcClick(self, s):
@@ -956,30 +981,29 @@
                 self.logger.error("Cannot load symbol. JSON Decode Error")
         self.centralW.scene.loadSymbol(items)
 
     def createLabelClick(self):
         createLabelDlg = pdlg.createSymbolLabelDialog(self)
         self.messageLine.setText('Place a label')
         if createLabelDlg.exec() == QDialog.Accepted:
-            modeList = [False for i in range(8)]
+            modeList = [False for _ in range(8)]
             modeList[5] = True
             self.setDrawMode(*modeList)
             # directly setting scene class attributes here to pass the information.
             self.centralW.scene.labelDefinition = createLabelDlg.labelDefinition.text()
             self.centralW.scene.labelHeight = (
                 createLabelDlg.labelHeightEdit.text().strip())
             self.centralW.scene.labelAlignment = (
                 createLabelDlg.labelAlignCombo.currentText())
             self.centralW.scene.labelOrient = (
                 createLabelDlg.labelOrientCombo.currentText())
             self.centralW.scene.labelUse = createLabelDlg.labelUseCombo.currentText()
-            if createLabelDlg.labelVisiCombo.currentText() == "Yes":
-                self.centralW.scene.labelOpaque = True
-            else:
-                self.centralW.scene.labelOpaque = False
+            self.centralW.scene.labelOpaque = (
+                createLabelDlg.labelVisiCombo.currentText() == "Yes"
+            )
             self.centralW.scene.labelType = "Normal"  # default button
             if createLabelDlg.normalType.isChecked():
                 self.centralW.scene.labelType = "Normal"
             elif createLabelDlg.NLPType.isChecked():
                 self.centralW.scene.labelType = "NLPLabel"
             elif createLabelDlg.pyLType.isChecked():
                 self.centralW.scene.labelType = "PyLabel"
@@ -1066,14 +1090,15 @@
     def setPens(self):
         self.wirePen = pens.sPen.returnPen("wirePen")
         self.symbolPen = pens.sPen.returnPen("symbolPen")
         self.selectedWirePen = pens.sPen.returnPen("selectedWirePen")
         self.pinPen = pens.sPen.returnPen("pinPen")
         self.labelPen = pens.sPen.returnPen("labelPen")
         self.textPen = pens.sPen.returnPen("textPen")
+        self.hilightPen = pens.sPen.returnPen("hilightPen")
         self.otherPen = pens.sPen.returnPen("otherPen")
 
     def defineSceneLayers(self):
         self.wireLayer = cel.wireLayer
         self.symbolLayer = cel.symbolLayer
         self.guideLineLayer = cel.guideLineLayer
         self.selectedWireLayer = cel.selectedWireLayer
@@ -1113,56 +1138,53 @@
 
     def eventFilter(self, source, event):
         '''
         Mouse events should snap to background grid points.
         '''
         if self.readOnly:  # if read only do not propagate any mouse events
             return True
-        elif (event.type() == QEvent.GraphicsSceneMouseMove or
-              event.type() == QEvent.GraphicsSceneMousePress or
-              event.type() == QEvent.GraphicsSceneMouseRelease):
-            event.setScenePos(
-                self.snapToGrid(event.scenePos(), self.gridTuple).toPointF())
+        elif event.type() in [
+            QEvent.GraphicsSceneMouseMove,
+            QEvent.GraphicsSceneMousePress,
+            QEvent.GraphicsSceneMouseRelease,
+        ]:
+            event.setScenePos(self.snapToGrid(event.scenePos(), self.gridTuple).toPointF())
             return False
         else:
             return super().eventFilter(source, event)
 
     def selectSceneItems(self, modifiers):
         if modifiers == Qt.ShiftModifier:
 
-            self.editorWindow.messageLine.setText(
-                "Draw Selection Rectangle")
+            self.editorWindow.messageLine.setText("Draw Selection Rectangle")
             self.selectionRectItem = QGraphicsRectItem(
                 QRectF(self.mousePressLoc, self.mousePressLoc))
             self.selectionRectItem.setPen(self.draftPen)
             self.addItem(self.selectionRectItem)
         else:
             self.editorWindow.messageLine.setText("Select an item")
             itemsAtMousePress = self.items(self.mousePressLoc)
             if itemsAtMousePress:
-                self.selectedItems = [item for item in itemsAtMousePress
-                                      if
+                self.selectedItems = [item for item in itemsAtMousePress if
                                       item.isSelected()]
                 self.editorWindow.messageLine.setText("Item selected")
             else:
                 self.selectedItems = None
                 self.editorWindow.messageLine.setText("Nothing selected")
 
     def selectInRectItems(self, selectionRect: QRect, partialSelection=False):
         """
         Select items in the scene.
         """
 
         if partialSelection:  # partial selection
-            selectedItems = self.items(selectionRect,
-                                            mode=Qt.IntersectsItemShape)
+            selectedItems = self.items(selectionRect, mode=Qt.IntersectsItemShape)
         else:
             # full selection
-            selectedItems = self.items(selectionRect,
-                                            mode=Qt.ContainsItemShape)
+            selectedItems = self.items(selectionRect, mode=Qt.ContainsItemShape)
         [item.setSelected(True) for item in selectedItems]
         return selectedItems
 
     def selectAll(self):
         """
         Select all items in the scene.
         """
@@ -1193,16 +1215,15 @@
         self.drawPin = False
         self.itemSelect = True
         self.drawArc = False  # draw arc
         self.drawRect = False
         self.drawLine = False
         self.addLabel = False
         self.drawCircle = False
-        self.drawMode = (
-                    self.drawLine or self.drawArc or self.drawRect or self.drawCircle)
+        self.drawMode = (self.drawLine or self.drawArc or self.drawRect or self.drawCircle)
         self.symbolShapes = ["line", "arc", "rect", "circle", "pin", "label"]
         self.changeOrigin = False
         self.origin = QPoint(0, 0)
         # some default attributes
         self.newPin = None
         self.pinName = ""
         self.pinType = shp.pin.pinTypes[0]
@@ -1235,36 +1256,31 @@
                     self.selectSceneItems(modifiers)
                 if self.drawPin:
                     self.editorWindow.messageLine.setText("Add Symbol Pin")
                     self.newPin = self.pinDraw(self.mousePressLoc, self.gridTuple)
                     self.newPin.setSelected(True)
                 elif self.drawLine:
                     self.editorWindow.messageLine.setText('Drawing a Line')
-                    self.newLine = self.lineDraw(self.mousePressLoc,
-                                                 self.mousePressLoc,
+                    self.newLine = self.lineDraw(self.mousePressLoc, self.mousePressLoc,
                                                  self.symbolPen, self.gridTuple)
                     self.newLine.setSelected(True)
                 elif self.addLabel:
                     self.newLabel = self.labelDraw(self.mousePressLoc, self.labelPen,
-                                                   self.labelDefinition,
-                                                   self.labelType,
-                                                   self.labelHeight,
-                                                   self.labelAlignment,
+                                                   self.labelDefinition, self.labelType,
+                                                   self.labelHeight, self.labelAlignment,
                                                    self.labelOrient, self.labelUse,
                                                    self.gridTuple)
                     self.newLabel.setSelected(True)
                 elif self.drawRect:
-                    self.newRect = self.rectDraw(self.mousePressLoc,
-                                                 self.mousePressLoc,
+                    self.newRect = self.rectDraw(self.mousePressLoc, self.mousePressLoc,
                                                  self.symbolPen, self.gridTuple)
                 elif self.drawCircle:
                     self.editorWindow.messageLine.setText(
                         'Click on the center of the circle')
-                    self.newCircle = self.circleDraw(self.mousePressLoc,
-                                                     self.mousePressLoc,
+                    self.newCircle = self.circleDraw(self.mousePressLoc, self.mousePressLoc,
                                                      self.symbolPen, self.gridTuple)
                 elif self.drawArc:
                     self.editorWindow.messageLine.setText('Start drawing an arc')
                     self.newArc = self.arcDraw(self.mousePressLoc, self.mousePressLoc,
                                                self.symbolPen, self.gridTuple)
                 if self.rotateItem and self.selectedItems:
                     self.rotateSelectedItems(self.mousePressLoc)
@@ -1274,36 +1290,35 @@
     def mouseMoveEvent(self, mouse_event: QGraphicsSceneMouseEvent) -> None:
 
         super().mouseMoveEvent(mouse_event)
         self.mouseMoveLoc = mouse_event.scenePos().toPoint()
         modifiers = QGuiApplication.keyboardModifiers()
         if mouse_event.buttons() == Qt.LeftButton:
             if self.drawLine:
-                self.editorWindow.messageLine.setText(
-                    "Release mouse on the end point")
+                self.editorWindow.messageLine.setText("Release mouse on the end point")
                 self.newLine.end = self.mouseMoveLoc
             elif self.drawPin and self.newPin.isSelected():
                 self.newPin.setPos(self.mouseMoveLoc - self.mousePressLoc)
             elif self.drawRect:
                 self.editorWindow.messageLine.setText(
                     "Release mouse on the bottom left point")
                 self.newRect.end = self.mouseMoveLoc
             elif self.drawCircle:
                 self.editorWindow.messageLine.setText('Extend Circle')
                 radius = ((self.mouseMoveLoc.x() - self.mousePressLoc.x()) ** 2 + (
-                                self.mouseMoveLoc.y() - self.mousePressLoc.y()) ** 2) ** 0.5
+                        self.mouseMoveLoc.y() - self.mousePressLoc.y()) ** 2) ** 0.5
                 self.newCircle.radius = radius
             elif self.drawArc:
                 self.editorWindow.messageLine.setText('Extend Arc')
                 self.newArc.end = self.mouseMoveLoc
             elif self.itemSelect and modifiers == Qt.ShiftModifier:
-                self.selectionRectItem.setRect(QRectF(self.mousePressLoc,self.mouseMoveLoc))
+                self.selectionRectItem.setRect(
+                    QRectF(self.mousePressLoc, self.mouseMoveLoc))
         self.statusLine.showMessage(
-            "Cursor Position: " + str(
-                (self.mouseMoveLoc - self.origin).toTuple()))
+            f"Cursor Position: {(self.mouseMoveLoc - self.origin).toTuple()}")
 
     def mouseReleaseEvent(self, mouse_event: QGraphicsSceneMouseEvent) -> None:
         super().mouseReleaseEvent(mouse_event)
         try:
             self.mouseReleaseLoc = mouse_event.scenePos().toPoint()
             modifiers = QGuiApplication.keyboardModifiers()
             if mouse_event.button() == Qt.LeftButton:
@@ -1318,82 +1333,75 @@
                 elif self.drawRect:
                     self.newRect.setSelected(False)
                 elif self.drawArc:
                     self.newArc.setSelected(False)
                 elif self.addLabel:
                     self.newLabel.setSelected(False)
                 elif self.itemSelect and modifiers == Qt.ShiftModifier:
-                    self.selectedItems = self.selectInRectItems(self.selectionRectItem.rect(
-                    ), self.partialSelection)
+                    self.selectedItems = self.selectInRectItems(
+                        self.selectionRectItem.rect(), self.partialSelection)
                     self.removeItem(self.selectionRectItem)
                     self.selectionRectItem = None
         except Exception as e:
             print(e)
 
-
             self.selectMode()
 
     def lineDraw(self, start: QPoint, current: QPoint, pen: pens.sPen,
                  gridTuple: [int, int]):
         line = shp.line(start, current, pen, gridTuple)
         self.addItem(line)
         undoCommand = us.addShapeUndo(self, line)
         self.undoStack.push(undoCommand)
         return line
 
-    def rectDraw(self, start: QPoint, end: QPoint, pen: pens.sPen,
-                 gridTuple: [int, int]):
+    def rectDraw(self, start: QPoint, end: QPoint, pen: pens.sPen, gridTuple: [int, int]):
         """
         Draws a rectangle on the scene
         """
         # rect = shp.rectangle(start, end - QPoint(pen.width() / 2, pen.width() / 2), pen,
         #                      gridTuple)
         rect = shp.rectangle(start, end, pen, gridTuple)
         self.addItem(rect)
         undoCommand = us.addShapeUndo(self, rect)
         self.undoStack.push(undoCommand)
         return rect
 
-    def circleDraw(self, start: QPoint, end: QPoint, pen: pens.sPen,
-                   gridTuple: [int, int]):
+    def circleDraw(self, start: QPoint, end: QPoint, pen: pens.sPen, gridTuple: [int, int]):
         """
         Draws a circle on the scene
         """
         snappedEnd = self.snapToGrid(end, gridTuple)
         circle = shp.circle(start, snappedEnd, pen, gridTuple)
         self.addItem(circle)
         undoCommand = us.addShapeUndo(self, circle)
         self.undoStack.push(undoCommand)
         return circle
 
-    def arcDraw(self, start: QPoint, end: QPoint, pen: pens.sPen,
-                gridTuple: [int, int]):
+    def arcDraw(self, start: QPoint, end: QPoint, pen: pens.sPen, gridTuple: [int, int]):
         '''
         Draws an arc inside the rectangle defined by start and end points.
         '''
         arc = shp.arc(start, end, pen, self.gridTuple)
         self.addItem(arc)
         undoCommand = us.addShapeUndo(self, arc)
         self.undoStack.push(undoCommand)
         return arc
 
     def pinDraw(self, current, gridTuple: [int, int]):
-        pin = shp.pin(current, self.pinPen, self.pinName, self.pinDir,
-                      self.pinType,
+        pin = shp.pin(current, self.pinPen, self.pinName, self.pinDir, self.pinType,
                       gridTuple)
         self.addItem(pin)
         undoCommand = us.addShapeUndo(self, pin)
         self.undoStack.push(undoCommand)
         return pin
 
-    def labelDraw(self, current, pen: pens.sPen, labelDefinition, labelType,
-                  labelHeight,
+    def labelDraw(self, current, pen: pens.sPen, labelDefinition, labelType, labelHeight,
                   labelAlignment, labelOrient, labelUse, gridTuple: [int, int]):
-        label = shp.label(current, pen, labelDefinition, gridTuple, labelType,
-                          labelHeight,
+        label = shp.label(current, pen, labelDefinition, gridTuple, labelType, labelHeight,
                           labelAlignment, labelOrient, labelUse, )
         label.labelVisible = self.labelOpaque
         label.labelDefs()
         label.setOpacity(1)
         self.addItem(label)
         undoCommand = us.addShapeUndo(self, label)
         self.undoStack.push(undoCommand)
@@ -1472,18 +1480,16 @@
                         self.updatePinShape(item)
                 elif isinstance(item, shp.label):
                     self.queryDlg = pdlg.labelPropertyDialog(self.editorWindow, item)
                     if self.queryDlg.exec() == QDialog.Accepted:
                         self.updateLabelShape(item)
 
     def updateRectangleShape(self, item: shp.rectangle):
-        left = self.snapToBase(float(self.queryDlg.rectLeftLine.text()),
-                               self.gridTuple[0])
-        top = self.snapToBase(float(self.queryDlg.rectTopLine.text()),
-                              self.gridTuple[1])
+        left = self.snapToBase(float(self.queryDlg.rectLeftLine.text()), self.gridTuple[0])
+        top = self.snapToBase(float(self.queryDlg.rectTopLine.text()), self.gridTuple[1])
         width = self.snapToBase(float(self.queryDlg.rectWidthLine.text()),
                                 self.gridTuple[0])
         height = self.snapToBase(float(self.queryDlg.rectHeightLine.text()),
                                  self.gridTuple[1])
         topLeft = item.mapFromScene(QPoint(left, top))
         # undoUpdateRectangle = us.updateShapeUndo()
         # us.keepOriginalShape(self, item, self.gridTuple, parent=undoUpdateRectangle)
@@ -1493,26 +1499,23 @@
 
     def updateCircleShape(self, item: shp.circle):
 
         centerX = self.snapToBase(float(self.queryDlg.centerXEdit.text()),
                                   self.gridTuple[0])
         centerY = self.snapToBase(float(self.queryDlg.centerYEdit.text()),
                                   self.gridTuple[1])
-        radius = self.snapToBase(float(self.queryDlg.radiusEdit.text()),
-                                 self.gridTuple[0])
+        radius = self.snapToBase(float(self.queryDlg.radiusEdit.text()), self.gridTuple[0])
         centerPoint = self.snapToGrid(QPoint(centerX, centerY), self.gridTuple)
         item.centre(item.mapFromScene(centerPoint))
         item.radius(radius)
 
     def updateArcShape(self, item: shp.arc):
 
-        startX = self.snapToBase(float(self.queryDlg.startXEdit.text()),
-                                 self.gridTuple[0])
-        startY = self.snapToBase(float(self.queryDlg.startYEdit.text()),
-                                 self.gridTuple[1])
+        startX = self.snapToBase(float(self.queryDlg.startXEdit.text()), self.gridTuple[0])
+        startY = self.snapToBase(float(self.queryDlg.startYEdit.text()), self.gridTuple[1])
         item.start = item.mapFromScene(QPoint(startX, startY)).toPoint()
         item.width = self.snapToBase(float(self.queryDlg.widthEdit.text()),
                                      self.gridTuple[0])
         item.height = self.snapToBase(float(self.queryDlg.heightEdit.text()),
                                       self.gridTuple[1])
 
     def updateLineShape(self, item: shp.line):
@@ -1526,35 +1529,30 @@
                           int(float(self.queryDlg.endYLine.text())), )
         item.end = item.mapFromScene(endEntry).toPoint()
 
     def updatePinShape(self, item: shp.pin):
         location = item.scenePos().toTuple()
         item.start = self.snapToGrid(
             QPoint(int(float(self.queryDlg.pinXLine.text()) - float(location[0])),
-                   int(float(self.queryDlg.pinYLine.text()) - float(
-                       location[1])), ),
+                   int(float(self.queryDlg.pinYLine.text()) - float(location[1])), ),
             self.gridTuple, )
-        item.rect = QRect(self.item.start.x() - 5,
-                          self.item.start.y() - 5,
-                          10, 10)
+        item.rect = QRect(self.item.start.x() - 5, self.item.start.y() - 5, 10, 10)
         item.pinName = self.queryDlg.pinName.text()
         item.pinType = self.queryDlg.pinType.currentText()
         item.pinDir = self.queryDlg.pinDir.currentText()
         item.update()
 
     def updateLabelShape(self, item: shp.label):
         """
         update pin shape with new values.
         """
         location = item.scenePos().toTuple()
         item.start = self.snapToGrid(
-            QPoint(
-                int(float(self.queryDlg.labelXLine.text()) - float(location[0])),
-                int(float(self.queryDlg.labelYLine.text()) - float(
-                    location[1])), ),
+            QPoint(int(float(self.queryDlg.labelXLine.text()) - float(location[0])),
+                int(float(self.queryDlg.labelYLine.text()) - float(location[1])), ),
             self.gridTuple, )
         item.labelDefinition = self.queryDlg.labelDefinition.text()
         item.labelHeight = self.queryDlg.labelHeightEdit.text()
         item.labelAlign = self.queryDlg.labelAlignCombo.currentText()
         item.labelOrient = self.queryDlg.labelOrientCombo.currentText()
         item.labelUse = self.queryDlg.labelUseCombo.currentText()
         if self.queryDlg.labelVisiCombo.currentText() == "Yes":
@@ -1610,25 +1608,22 @@
 
     def viewSymbolProperties(self):
         """
         View symbol properties dialog.
         """
         # copy symbol attribute list to another list by deepcopy to be safe
         attributeListCopy = deepcopy(self.attributeList)
-        symbolPropDialogue = pdlg.symbolLabelsDialogue(self.parent.parent,
-                                                       self.items(),
+        symbolPropDialogue = pdlg.symbolLabelsDialogue(self.parent.parent, self.items(),
                                                        attributeListCopy)
         if symbolPropDialogue.exec() == QDialog.Accepted:
             for i, item in enumerate(symbolPropDialogue.labelItemList):
                 # label name is not changed.
                 item.labelHeight = symbolPropDialogue.labelHeightList[i].text()
-                item.labelAlign = symbolPropDialogue.labelAlignmentList[
-                    i].currentText()
-                item.labelOrient = symbolPropDialogue.labelOrientationList[
-                    i].currentText()
+                item.labelAlign = symbolPropDialogue.labelAlignmentList[i].currentText()
+                item.labelOrient = symbolPropDialogue.labelOrientationList[i].currentText()
                 item.labelUse = symbolPropDialogue.labelUseList[i].currentText()
                 item.labelType = symbolPropDialogue.labelTypeList[i].currentText()
                 item.update(item.boundingRect())
             # create an empty attribute list. If the dialog is OK, the local attribute list
             # will be copied to the symbol attribute list.
             localAttributeList = []
             for i, item in enumerate(symbolPropDialogue.attributeNameList):
@@ -1644,15 +1639,14 @@
         super().__init__(parent)
         self.parent = parent
         self.instCounter = 0
         self.start = QPoint(0, 0)
         self.current = QPoint(0, 0)
         self.selectedItems = None
         self.itemsAtMousePress = list()
-        self.itemContextMenu = QMenu()
         self.drawWire = False  # flag to add wire
         self.drawPin = False  # flag to add pin
         self.drawText = False  # flat to add text
         self.itemSelect = True  # flag to select item
         self.drawMode = self.drawWire or self.drawPin
         self.draftPen = QPen(self.guideLineLayer.color, 1)
         self.draftPen.setStyle(Qt.DashLine)
@@ -1673,14 +1667,15 @@
         self.pinDir = "Input"
         self.parentView = None
         self.wires = None
         self.newInstance = None
         self.newPin = None
         self.newText = None
         self.snapPointRect = None
+        self.highlightNets = False
 
     def mousePressEvent(self, mouse_event: QGraphicsSceneMouseEvent) -> None:
 
         super().mousePressEvent(mouse_event)
         try:
             modifiers = QGuiApplication.keyboardModifiers()
             self.viewRect = self.parent.view.mapToScene(
@@ -1738,55 +1733,54 @@
                     if self.snapPointRect is None:
                         rect = QRectF(QPointF(-5, -5), QPointF(5, 5))
                         self.snapPointRect = QGraphicsRectItem(rect)
                         self.snapPointRect.setPen(self.draftPen)
                         self.addItem(self.snapPointRect)
                     self.snapPointRect.setPos(self.mouseMoveLoc)
 
-                    self.extendWires(self.wires, self.mousePressLoc,
-                                     self.mouseMoveLoc)
+                    self.extendWires(self.wires, self.mousePressLoc, self.mouseMoveLoc)
                 elif self.drawPin and self.newPin.isSelected():
                     self.newPin.setPos(self.mouseMoveLoc - self.mousePressLoc)
 
                 elif self.drawText and self.newText.isSelected():
                     self.newText.setPos(self.mouseMoveLoc - self.mousePressLoc)
 
                 elif self.itemSelect and modifiers == Qt.ShiftModifier:
-                        self.selectionRectItem.setRect(
-                            QRectF(self.mousePressLoc, self.mouseMoveLoc))
+                    self.selectionRectItem.setRect(
+                        QRectF(self.mousePressLoc, self.mouseMoveLoc))
 
             self.editorWindow.statusLine.showMessage(
-                "Cursor Position: " + str(self.mouseMoveLoc.toTuple()))
+                f"Cursor Position: {str(self.mouseMoveLoc.toTuple())}"
+            )
         except Exception as e:
             self.logger.error(e)
 
     def mouseReleaseEvent(self, mouse_event: QGraphicsSceneMouseEvent) -> None:
         super().mouseReleaseEvent(mouse_event)
         try:
             self.mouseReleaseLoc = mouse_event.scenePos().toPoint()
             modifiers = QGuiApplication.keyboardModifiers()
             if mouse_event.button() == Qt.LeftButton:
                 if self.drawWire and self.wires:
                     self.mouseReleaseLoc = self.findSnapPoint(self.mouseReleaseLoc,
                                                               self.snapDistance,
                                                               set(self.wires))
-                    self.extendWires(self.wires, self.mousePressLoc,
-                                     self.mouseReleaseLoc)
+                    self.extendWires(self.wires, self.mousePressLoc, self.mouseReleaseLoc)
                     if self.snapPointRect:
                         self.removeItem(self.snapPointRect)
                         self.snapPointRect = None
 
                     lines = self.pruneWires(self.wires, self.wirePen)
                     if lines:
                         for line in lines:
                             line.mergeNets()
                     self.wires = None  # self.mergeNets()
                     viewNets = {netItem for netItem in
                                 self.editorWindow.centralW.view.items() if
-                                isinstance(netItem,net.schematicNet)}
+                                isinstance(netItem, net.schematicNet)}
                     [netItem.findDotPoints() for netItem in viewNets]
 
                 elif self.addInstance:
                     self.addInstance = False
                     self.newInstance = None
 
                 elif self.drawText:
@@ -1794,42 +1788,39 @@
                     self.drawText = False
                     self.newText = None
                 elif self.drawPin:
                     self.parent.parent.messageLine.setText("Pin added")
                     self.drawPin = False
                     self.newPin = None
                 elif self.itemSelect and modifiers == Qt.ShiftModifier:
-                    self.selectedItems = self.selectInRectItems(self.selectionRectItem.rect(
-                    ), self.partialSelection)
+                    self.selectedItems = self.selectInRectItems(
+                        self.selectionRectItem.rect(), self.partialSelection)
                     self.removeItem(self.selectionRectItem)
                     self.selectionRectItem = None
         except Exception as e:
             print(e)
 
-    def findSnapPoint(self, eventLoc: QPoint, snapDistance: int,
-                      ignoredNetSet: set):
+    def findSnapPoint(self, eventLoc: QPoint, snapDistance: int, ignoredNetSet: set):
         snapRect = QRect(eventLoc.x() - snapDistance, eventLoc.y() - snapDistance,
                          2 * snapDistance, 2 * snapDistance)
         snapItems = {item for item in self.items(snapRect) if
-                     isinstance(item, shp.pin) or isinstance(item,
-                                                             net.schematicNet)}
+                     isinstance(item, shp.pin) or isinstance(item, net.schematicNet)}
 
         try:
             snapItems -= ignoredNetSet
             lengths = list()
             points = list()
             items = list()
             if len(snapItems) > 0:
                 for item in snapItems:
                     if isinstance(item, shp.pin):
                         items.append(item)
                         points.append(item.mapToScene(item.start))
                         lengths.append(
-                            (item.mapToScene(
-                                item.start) - eventLoc).manhattanLength())
+                            (item.mapToScene(item.start) - eventLoc).manhattanLength())
                     elif isinstance(item, net.schematicNet):
                         if snapRect.contains(item.line().p1().toPoint()):
                             items.append(item)
                             # print(f'net start:{item.start}')
                             points.append(item.line().p1().toPoint())
                             lengths.append((item.mapToScene(
                                 item.line().p1()) - eventLoc).manhattanLength())
@@ -1872,16 +1863,15 @@
             sceneNetsSet = self.groupNamedNets(globalNetsSet, sceneNetsSet)
             # now find nets connected to schematic pins
             schemPinConNetsSet = self.findSchPinNets()
             sceneNetsSet -= schemPinConNetsSet
             # use these nets as starting nets to find other nets connected to them
             sceneNetsSet = self.groupNamedNets(schemPinConNetsSet, sceneNetsSet)
             # now find the set of nets whose name is set by the user
-            namedNetsSet = set(
-                [netItem for netItem in sceneNetsSet if netItem.nameSet])
+            namedNetsSet = set([netItem for netItem in sceneNetsSet if netItem.nameSet])
             sceneNetsSet -= namedNetsSet
             # now remove already named net set from firstNetSet
             unnamedNets = self.groupNamedNets(namedNetsSet, sceneNetsSet)
             # now start netlisting from the unnamed nets
             self.groupUnnamedNets(unnamedNets, self.netCounter)
         except Exception as e:
             self.logger.error(e)
@@ -1895,25 +1885,23 @@
             globalNetsSet = set()
             for symbolItem in self.findSceneSymbolSet():
                 for pinName, pinItem in symbolItem.pins.items():
                     if pinName[-1] == '!':
                         globalPinsSet.add(pinItem)
             # self.logger.warning(f'global pins:{globalPinsSet}')
             for pinItem in globalPinsSet:
-                pinNetSet = {netItem for netItem in
-                             self.items(pinItem.sceneBoundingRect())
+                pinNetSet = {netItem for netItem in self.items(pinItem.sceneBoundingRect())
                              if isinstance(netItem, net.schematicNet)}
                 for netItem in pinNetSet:
                     if netItem.nameSet or netItem.nameAdded:
                         # check if net is already named explicitly
                         if netItem.name != pinItem.pinName:
                             netItem.nameConflict = True
-                            self.logger.error(
-                                f"Net name conflict at {pinItem.pinName} of "
-                                f"{pinItem.parent.instanceName}.")
+                            self.logger.error(f"Net name conflict at {pinItem.pinName} of "
+                                              f"{pinItem.parent.instanceName}.")
                         else:
                             globalNetsSet.add(netItem)
                     else:
                         globalNetsSet.add(netItem)
                         netItem.name = pinItem.pinName
                         netItem.nameAdded = True
             return globalNetsSet
@@ -1950,39 +1938,35 @@
         """
         Groups nets with the same name using namedNetsSet members as seeds and going
         through connections. Returns the set of still unnamed nets.
         """
         for netItem in namedNetsSet:
             if self.schematicNets.get(netItem.name) is None:
                 self.schematicNets[netItem.name] = set()
-            connectedNets, unnamedNetsSet = self.traverseNets({netItem, },
-                                                              unnamedNetsSet, )
+            connectedNets, unnamedNetsSet = self.traverseNets({netItem, }, unnamedNetsSet, )
             self.schematicNets[netItem.name] |= connectedNets
         # These are the nets not connected to any named net
         return unnamedNetsSet
 
-    def groupUnnamedNets(self, unnamedNetsSet: set[net.schematicNet],
-                         nameCounter: int):
+    def groupUnnamedNets(self, unnamedNetsSet: set[net.schematicNet], nameCounter: int):
         """
         Groups nets together if they are connected and assign them default names
         if they don't have a name assigned.
         """
         # select a net from the set and remove it from the set
         try:
-            initialNet = (
-                unnamedNetsSet.pop())  # assign it a name, net0, net1, net2, etc.
+            initialNet = (unnamedNetsSet.pop())  # assign it a name, net0, net1, net2, etc.
         except KeyError:  # initialNet set is empty
             pass
         else:
             initialNet.name = "net" + str(nameCounter)
             # now go through the set and see if any of the
             # nets are connected to the initial net
             # remove them from the set and add them to the initial net's set
-            self.schematicNets[
-                initialNet.name], unnamedNetsSet = self.traverseNets(
+            self.schematicNets[initialNet.name], unnamedNetsSet = self.traverseNets(
                 {initialNet, }, unnamedNetsSet, )
             nameCounter += 1
             if len(unnamedNetsSet) > 1:
                 self.groupUnnamedNets(unnamedNetsSet, nameCounter)
             elif len(unnamedNetsSet) == 1:
                 lastNet = unnamedNetsSet.pop()
                 lastNet.name = "net" + str(nameCounter)
@@ -2013,23 +1997,21 @@
         # keep searching if you already found a net connected to the initial net
         if len(newFoundConnectedSet) > 0:
             connectedSet.update(newFoundConnectedSet)
             otherNetsSet -= newFoundConnectedSet
             self.traverseNets(connectedSet, otherNetsSet)
         return connectedSet, otherNetsSet
 
-    def checkPinNetConnect(self, pinItem: shp.schematicPin,
-                           netItem: net.schematicNet):
+    def checkPinNetConnect(self, pinItem: shp.schematicPin, netItem: net.schematicNet):
         """
         Determine if a pin is connected to a net.
         """
-        if pinItem.sceneBoundingRect().intersects(netItem.sceneBoundingRect()):
-            return True
-        else:
-            return False
+        return bool(
+            pinItem.sceneBoundingRect().intersects(netItem.sceneBoundingRect())
+        )
 
     def checkNetConnect(self, netItem, otherNetItem):
         """
         Determine if a net is connected to another one. One net should end on the other net.
         """
         netBRect = netItem.sceneBoundingRect().adjusted(-2, -2, 2, 2)
         if otherNetItem is not netItem:
@@ -2062,26 +2044,23 @@
                 if pinConnectedNets:
                     symbolItem.pinNetMap[pinName] = pinConnectedNets[0].name
                     pinItem.connected = True
 
                 if not pinItem.connected:
                     # assign a default net name prefixed with d(efault).
                     symbolItem.pinNetMap[pinName] = f"dnet{netCounter}"
-                    self.logger.warning(
-                        f"left unconnected:{symbolItem.pinNetMap[pinName]}")
+                    self.logger.warning(f"left unconnected:{symbolItem.pinNetMap[pinName]}")
                     netCounter += 1
             # now reorder pinNetMap according pinOrder attribute
             if symbolItem.attr.get('pinOrder'):
                 pinOrderList = list()
                 [pinOrderList.append(item.strip()) for item in
-                 symbolItem.attr.get(
-                     'pinOrder').split(',')]
-                symbolItem.pinNetMap = {
-                    pinName: symbolItem.pinNetMap[pinName] for pinName in
-                    pinOrderList}
+                 symbolItem.attr.get('pinOrder').split(',')]
+                symbolItem.pinNetMap = {pinName: symbolItem.pinNetMap[pinName] for pinName
+                    in pinOrderList}
 
     def findSceneCells(self, symbolSet):
         """
         This function just goes through set of symbol items in the scene and
         checks if that symbol's cell is encountered first time. If so, it adds
         it to a dictionary   cell_name:symbol
         """
@@ -2096,28 +2075,25 @@
         Find all the symbols on the scene as a set.
         """
         symbolSceneSet = {item for item in self.items() if
                           isinstance(item, shp.symbolShape)}
         return symbolSceneSet
 
     def findSceneNetsSet(self) -> set[net.schematicNet]:
-        return set(
-            item for item in self.items() if isinstance(item, net.schematicNet))
+        return set(item for item in self.items() if isinstance(item, net.schematicNet))
 
     def findSceneSchemPinsSet(self) -> set[shp.schematicPin]:
-        pinsSceneSet = {item for item in self.items() if
-                        isinstance(item, shp.schematicPin)}
+        pinsSceneSet = {item for item in self.items() if isinstance(item, shp.schematicPin)}
         if pinsSceneSet:  # check pinsSceneSet is empty
             return pinsSceneSet
         else:
             return set()
 
     def findSceneTextSet(self) -> set[shp.text]:
-        textSceneSet = {item for item in self.items() if
-                        isinstance(item, shp.text)}
+        textSceneSet = {item for item in self.items() if isinstance(item, shp.text)}
         if textSceneSet:  # check textSceneSet is empty
             return textSceneSet
         else:
             return set()
 
     def keyPressEvent(self, key_event):
         super().keyPressEvent(key_event)
@@ -2131,16 +2107,15 @@
         self.selectedItems = []
         self.parent.parent.messageLine.setText("Select Mode")
 
     def addWires(self, start: QPoint, pen: pens.sPen) -> net.schematicNet:
         """
         Add a net or nets to the scene.
         """
-        lines = [net.schematicNet(start, start, pen),
-                 net.schematicNet(start, start, pen),
+        lines = [net.schematicNet(start, start, pen), net.schematicNet(start, start, pen),
                  net.schematicNet(start, start, pen)]
         return lines
 
     def extendWires(self, lines: list, start: QPoint, end: QPoint):
         '''
         This method is to shape the wires drawn using addWires method.
         __|^^^
@@ -2158,24 +2133,22 @@
             lines[1].end = secondPoint
             lines[2].start = secondPoint
             lines[2].end = end
         except Exception as e:
             self.logger.error(e)
 
     def pruneWires(self, lines, pen):
-        if lines[0].start == lines[
-            2].end:  # if the first and last points are the same
+        if lines[0].start == lines[2].end:  # if the first and last points are the same
             for line in lines:
                 self.removeItem(line)
                 del line
             return None
         # if the line is vertical or horizontal
-        elif lines[0].start.x() == lines[2].end.x() or lines[0].start.y() == \
-                lines[
-                    2].end.y():
+        elif lines[0].start.x() == lines[2].end.x() or lines[0].start.y() == lines[
+            2].end.y():
             newLine = net.schematicNet(lines[0].start, lines[2].end, pen)
             self.addItem(newLine)
             undoCommand = us.addShapeUndo(self, newLine)
             self.undoStack.push(undoCommand)
             for line in lines:
                 self.removeItem(line)
                 del line
@@ -2190,30 +2163,28 @@
                     undoCommand = us.addShapeUndo(self, line)
                     self.undoStack.push(undoCommand)
             return lines
 
     def addPin(self, pos: QPoint):
         try:
             pin = shp.schematicPin(pos, self.pinPen, self.pinName, self.pinDir,
-                                   self.pinType,
-                                   self.gridTuple)
+                                   self.pinType, self.gridTuple)
             self.addItem(pin)
             undoCommand = us.addShapeUndo(self, pin)
             self.undoStack.push(undoCommand)
             return pin
         except Exception as e:
             self.logger.error(e)
 
     def addNote(self, pos: QPoint):
         """
         Changed the method name not to clash with qgraphicsscene addText method.
         """
         text = shp.text(pos, self.textPen, self.noteText, self.gridTuple,
-                        self.noteFontFamily, self.noteFontStyle,
-                        self.noteFontSize,
+                        self.noteFontFamily, self.noteFontStyle, self.noteFontSize,
                         self.noteAlign, self.noteOrient, )
         self.addItem(text)
         undoCommand = us.addShapeUndo(self, text)
         self.undoStack.push(undoCommand)
         return text
 
     def drawInstance(self, pos: QPoint):
@@ -2239,23 +2210,21 @@
             try:
                 items = json.load(temp)
                 if items[0]["cellView"] == "symbol":
                     for item in items[1:]:
                         if item["type"] == 'attr':
                             itemAttributes[item["nam"]] = item["def"]
                         else:
-                            itemShapes.append(
-                                lj.createSymbolItems(item, self.gridTuple))
+                            itemShapes.append(lj.createSymbolItems(item, self.gridTuple))
                 else:
                     self.logger.error("Not a symbol!")
 
                 # create a symbol instance passing item shapes and attributes as
                 # arguments
-                symbolInstance = shp.symbolShape(draftPen, self.gridTuple,
-                                                 itemShapes,
+                symbolInstance = shp.symbolShape(draftPen, self.gridTuple, itemShapes,
                                                  itemAttributes)
                 symbolInstance.setPos(pos)
                 # For each instance assign a counter number from the scene
                 symbolInstance.counter = self.itemCounter
 
                 symbolInstance.instanceName = f"I{symbolInstance.counter}"
                 symbolInstance.libraryName = file.parent.parent.stem
@@ -2284,16 +2253,15 @@
                 selectedItemJson = json.dumps(item, cls=se.schematicEncoder)
                 itemCopyDict = json.loads(selectedItemJson)
                 if isinstance(item, shp.symbolShape):
                     self.itemCounter += 1
                     itemCopyDict["name"] = f"I{self.itemCounter}"
                     itemCopyDict['ic'] = int(self.itemCounter)
                     itemCopyDict["ld"]["instName"][0] = f"I{self.itemCounter}"
-                    shape = lj.createSchematicItems(itemCopyDict,
-                                                    self.libraryDict,
+                    shape = lj.createSchematicItems(itemCopyDict, self.libraryDict,
                                                     item.viewName, self.gridTuple)
                     [label.labelDefs() for label in shape.labels.values()]
                 elif isinstance(item, net.schematicNet):
                     shape = lj.createSchematicNets(itemCopyDict)
                 elif isinstance(item, shp.schematicPin):
                     shape = lj.createSchematicPins(itemCopyDict, self.gridTuple)
                 elif isinstance(item, shp.text):
@@ -2327,16 +2295,15 @@
     def loadSchematicCell(self, itemsList):
         """
         load schematic from item list
         """
         for item in itemsList[1:]:
             if item is not None:
                 if item["type"] == "symbolShape":
-                    itemShape = lj.createSchematicItems(item, self.libraryDict,
-                                                        "symbol",
+                    itemShape = lj.createSchematicItems(item, self.libraryDict, "symbol",
                                                         self.gridTuple)
                     self.addItem(itemShape)
                     if itemShape.counter > self.itemCounter:
                         self.itemCounter = itemShape.counter
                     [labelItem.labelDefs() for labelItem in itemShape.labels.values()]
                 elif item["type"] == "schematicNet":
                     netShape = lj.createSchematicNets(item)
@@ -2353,72 +2320,117 @@
         # self.addItem(shp.text(QPoint(0, 200), self.textPen, 'Revolution EDA'))
         self.update()
 
     def viewObjProperties(self):
         """
         Display the properties of the selected object.
         """
-        if self.selectedItems is not None:
-            for item in self.selectedItems:
-                if isinstance(item, shp.symbolShape):
-                    dlg = pdlg.instanceProperties(self.editorWindow, item)
-                    if dlg.exec() == QDialog.Accepted:
-                        item.instanceName = dlg.instNameEdit.text().strip()
-                        item.angle = float(dlg.angleEdit.text().strip())
+        try:
+            if self.selectedItems is not None:
+                for item in self.selectedItems:
+                    if isinstance(item, shp.symbolShape):
+                        dlg = pdlg.instanceProperties(self.editorWindow, item)
+                        if dlg.exec() == QDialog.Accepted:
+                            item.instanceName = dlg.instNameEdit.text().strip()
+                            item.angle = float(dlg.angleEdit.text().strip())
+
+                            location = QPoint(float(dlg.xLocationEdit.text().strip()),
+                                    float(dlg.yLocationEdit.text().strip())) - self.origin
+                            item.setPos(self.snapToGrid(location, self.gridTuple))
+                            tempDoc = QTextDocument()
+                            for i in range(dlg.instanceLabelsLayout.rowCount()):
+                                # first create label name document with HTML annotations
+                                tempDoc.setHtml(dlg.instanceLabelsLayout.itemAtPosition(i,
+                                                                                        0).widget().text())
+                                # now strip html annotations
+                                tempLabelName = tempDoc.toPlainText().strip()
+                                # check if label name is in label dictionary of item.
+                                if item.labels.get(tempLabelName):
+                                    item.labels[tempLabelName].labelValue = (
+                                        dlg.instanceLabelsLayout.itemAtPosition(i,
+                                                                                1).widget().text())
+                                    visible = (dlg.instanceLabelsLayout.itemAtPosition(i,
+                                                                                       2).widget().currentText())
+                                    if visible == "True":
+                                        item.labels[tempLabelName].labelVisible = True
+                                    else:
+                                        item.labels[tempLabelName].labelVisible = False
+                            [labelItem.labelDefs() for labelItem in
+                             item.labels.values()]  # item.update()
+                    elif isinstance(item, net.schematicNet):
+                        dlg = pdlg.netProperties(self.editorWindow, item)
+                        if dlg.exec() == QDialog.Accepted:
+                            item.name = dlg.netNameEdit.text().strip()
+                            if item.name != "":
+                                item.nameSet = True
+                            item.update()
+                    elif isinstance(item, shp.text):
+                        dlg = pdlg.noteTextEditProperties(self.editorWindow, item)
+                        if dlg.exec() == QDialog.Accepted:
+                            # item.prepareGeometryChange()
+                            start = item.start
+                            self.removeItem(item)
+                            item = shp.text(start, self.textPen,
+                                            dlg.plainTextEdit.toPlainText(), self.gridTuple,
+                                            dlg.familyCB.currentText(),
+                                            dlg.fontStyleCB.currentText(),
+                                            dlg.fontsizeCB.currentText(),
+                                            dlg.textAlignmCB.currentText(),
+                                            dlg.textOrientCB.currentText(), )
+                            self.rotateAnItem(start, item, float(item.textOrient[1:]))
+                            self.addItem(item)
+                    elif isinstance(item, shp.schematicPin):
+                        dlg = pdlg.schematicPinPropertiesDialog(self.editorWindow, item)
+                        dlg.pinName.setText(item.pinName)
+                        dlg.pinDir.setCurrentText(item.pinDir)
+                        dlg.pinType.setCurrentText(item.pinType)
+                        dlg.angleEdit.setText(str(item.angle))
+                        dlg.xlocationEdit.setText(str(item.mapToScene(item.start).x()))
+                        dlg.ylocationEdit.setText(str(item.mapToScene(item.start).y()))
+                        if dlg.exec() == QDialog.Accepted:
+                            item.pinName = dlg.pinName.text().strip()
+                            item.pinDir = dlg.pinDir.currentText()
+                            item.pinType = dlg.pinType.currentText()
+                            itemStartPos = QPoint(float(dlg.xlocationEdit.text().strip(
+                            )), float(dlg.ylocationEdit.text().strip()))
+                            item.start=self.snapToGrid(itemStartPos-self.origin,
+                                                       self.gridTuple)
+                            item.angle = float(dlg.angleEdit.text().strip())
+        except Exception as e:
+            self.logger.error(e)
 
-                        location = self.snapToGrid(
-                            QPoint(float(dlg.xLocationEdit.text().strip()),
-                                   float(dlg.yLocationEdit.text().strip()), ),
-                            self.gridTuple, )
-                        item.setPos(location)
-                        tempDoc = QTextDocument()
-                        for i in range(dlg.instanceLabelsLayout.rowCount()):
-                            # first create label name document with HTML annotations
-                            tempDoc.setHtml(
-                                dlg.instanceLabelsLayout.itemAtPosition(i,
-                                                                        0).widget().text())
-                            # now strip html annotations
-                            tempLabelName = tempDoc.toPlainText().strip()
-                            # check if label name is in label dictionary of item.
-                            if item.labels.get(tempLabelName):
-                                item.labels[tempLabelName].labelValue = (
-                                    dlg.instanceLabelsLayout.itemAtPosition(i,
-                                                                            1).widget().text())
-                                visible = (
-                                    dlg.instanceLabelsLayout.itemAtPosition(i,
-                                                                            2).widget().currentText())
-                                if visible == "True":
-                                    item.labels[tempLabelName].labelVisible = True
-                                else:
-                                    item.labels[
-                                        tempLabelName].labelVisible = False
-                        [labelItem.labelDefs() for labelItem in
-                         item.labels.values()]  # item.update()
-                elif isinstance(item, net.schematicNet):
-                    dlg = pdlg.netProperties(self.parent.parent, item)
-                    if dlg.exec() == QDialog.Accepted:
-                        item.name = dlg.netNameEdit.text().strip()
-                        item.nameSet = True
-                        item.update()
-                elif isinstance(item, shp.text):
-                    dlg = pdlg.noteTextEditProperties(self.parent.parent, item)
-                    if dlg.exec() == QDialog.Accepted:
-                        # item.prepareGeometryChange()
-                        start = item.start
-                        self.removeItem(item)
-                        item = shp.text(start, self.textPen,
-                                        dlg.plainTextEdit.toPlainText(),
-                                        self.gridTuple,
-                                        dlg.familyCB.currentText(),
-                                        dlg.fontStyleCB.currentText(),
-                                        dlg.fontsizeCB.currentText(),
-                                        dlg.textAlignmCB.currentText(),
-                                        dlg.textOrientCB.currentText(), )
-                        self.rotateAnItem(start, item, float(item.textOrient[1:]))
-                        self.addItem(item)
+    def netNameEdit(self):
+        """
+        Edit the name of the selected net.
+        """
+        try:
+            if self.selectedItems is not None:
+                for item in self.selectedItems:
+                    if isinstance(item, net.schematicNet):
+                        dlg = pdlg.netProperties(self.editorWindow, item)
+                        if dlg.exec() == QDialog.Accepted:
+                            item.name = dlg.netNameEdit.text().strip()
+                            if item.name != "":
+                                item.nameSet = True
+                            item.update()
+        except Exception as e:
+            self.logger.error(e)
+
+    def hilightNets(self):
+        """
+        Show the connections the selected items.
+        """
+        try:
+            if self.editorWindow.hilightNetAction.isChecked():
+                self.highlightNets = True
+            else:
+                self.highlightNets = False
+
+        except Exception as e:
+            self.logger.error(e)
 
     def createSymbol(self):
         """
         Create a symbol view for a schematic.
         """
         oldSymbolItem = False
 
@@ -2426,34 +2438,30 @@
                                                self.parent.parent.cellName,
                                                self.parent.parent, )
         if askViewNameDlg.exec() == QDialog.Accepted:
             symbolViewName = askViewNameDlg.symbolViewsCB.currentText()
             if symbolViewName in askViewNameDlg.symbolViewNames:
                 oldSymbolItem = True
             if oldSymbolItem:
-                deleteSymViewDlg = fd.deleteSymbolDialog(
-                    self.parent.parent.cellName,
+                deleteSymViewDlg = fd.deleteSymbolDialog(self.parent.parent.cellName,
                     symbolViewName, self.parent.parent)
                 if deleteSymViewDlg.exec() == QDialog.Accepted:
                     symbolViewItem = self.generateSymbol(symbolViewName)
-                    self.editorWindow.appMainW.libraryBrowser.openCellView(
-                        symbolViewItem, self.editorWindow.cellItem,
-                        self.editorWindow.libItem)
+                    self.editorWindow.appMainW.libraryBrowser.openCellView(symbolViewItem,
+                        self.editorWindow.cellItem, self.editorWindow.libItem)
             else:
                 symbolViewItem = self.generateSymbol(symbolViewName)
-                self.editorWindow.appMainW.libraryBrowser.openCellView(
-                    symbolViewItem,
+                self.editorWindow.appMainW.libraryBrowser.openCellView(symbolViewItem,
                     self.editorWindow.cellItem, self.editorWindow.libItem)
 
     def generateSymbol(self, symbolViewName: str):
         # openPath = pathlib.Path(cellItem.data(Qt.UserRole + 2))
         libName = self.editorWindow.libName
         cellName = self.editorWindow.cellName
-        libItem = libm.getLibItem(self.editorWindow.libraryView.libraryModel,
-                                  libName)
+        libItem = libm.getLibItem(self.editorWindow.libraryView.libraryModel, libName)
         cellItem = libm.getCellItem(libItem, cellName)
         libraryView = self.editorWindow.libraryView
         schematicPins = list(self.findSceneSchemPinsSet())
 
         schematicPinNames = [pinItem.pinName for pinItem in schematicPins]
 
         inputPins = [pinItem.pinName for pinItem in schematicPins if
@@ -2461,148 +2469,132 @@
 
         outputPins = [pinItem.pinName for pinItem in schematicPins if
                       pinItem.pinDir == shp.schematicPin.pinDirs[1]]
 
         inoutPins = [pinItem.pinName for pinItem in schematicPins if
                      pinItem.pinDir == shp.schematicPin.pinDirs[2]]
 
-        dlg = pdlg.symbolCreateDialog(self.parent.parent, inputPins, outputPins,
-                                      inoutPins)
+        dlg = pdlg.symbolCreateDialog(self.parent.parent, inputPins, outputPins, inoutPins)
         if dlg.exec() == QDialog.Accepted:
-            symbolViewItem = scb.createCellView(self.parent.parent,
-                                                symbolViewName,
+            symbolViewItem = scb.createCellView(self.parent.parent, symbolViewName,
                                                 cellItem)
             libraryDict = self.parent.parent.libraryDict
             # create symbol editor window with an empty items list
             symbolWindow = symbolEditor(symbolViewItem, libraryDict, libraryView)
             try:
                 leftPinNames = list(filter(None, [pinName.strip() for pinName in
-                                                  dlg.leftPinsEdit.text().split(
-                                                      ",")], ))
+                                                  dlg.leftPinsEdit.text().split(",")], ))
                 rightPinNames = list(filter(None, [pinName.strip() for pinName in
-                                                   dlg.rightPinsEdit.text().split(
-                                                       ",")], ))
+                                                   dlg.rightPinsEdit.text().split(",")], ))
                 topPinNames = list(filter(None, [pinName.strip() for pinName in
-                                                 dlg.topPinsEdit.text().split(
-                                                     ",")], ))
+                                                 dlg.topPinsEdit.text().split(",")], ))
                 bottomPinNames = list(filter(None, [pinName.strip() for pinName in
                                                     dlg.bottomPinsEdit.text().split(
                                                         ",")], ))
                 stubLength = int(float(dlg.stubLengthEdit.text().strip()))
                 pinDistance = int(float(dlg.pinDistanceEdit.text().strip()))
-                rectXDim = (max(len(topPinNames),
-                                len(bottomPinNames)) + 1) * pinDistance
-                rectYDim = (max(len(leftPinNames),
-                                len(rightPinNames)) + 1) * pinDistance
+                rectXDim = (max(len(topPinNames), len(bottomPinNames)) + 1) * pinDistance
+                rectYDim = (max(len(leftPinNames), len(rightPinNames)) + 1) * pinDistance
             except ValueError:
                 self.logger.error("Enter valid value")
 
         # add window to open windows list
-        libraryView.openViews[
-            f"{libName}_{cellName}_{symbolViewName}"] = symbolWindow
+        libraryView.openViews[f"{libName}_{cellName}_{symbolViewName}"] = symbolWindow
         symbolScene = symbolWindow.centralW.scene
-        symbolScene.rectDraw(QPoint(0, 0), QPoint(rectXDim, rectYDim),
-                             self.symbolPen,
+        symbolScene.rectDraw(QPoint(0, 0), QPoint(rectXDim, rectYDim), self.symbolPen,
                              symbolScene.gridTuple)
         symbolScene.labelDraw(QPoint(int(0.25 * rectXDim), int(0.4 * rectYDim)),
-                              self.labelPen, "[@cellName]", "NLPLabel", "12",
-                              "Center",
+                              self.labelPen, "[@cellName]", "NLPLabel", "12", "Center",
                               "R0", "Instance", symbolScene.gridTuple)
-        symbolScene.labelDraw(QPoint(int(rectXDim), int(-0.2 * rectYDim)),
-                              self.labelPen,
-                              "[@instName]", "NLPLabel", "12", "Center", "R0",
-                              "Instance",
+        symbolScene.labelDraw(QPoint(int(rectXDim), int(-0.2 * rectYDim)), self.labelPen,
+                              "[@instName]", "NLPLabel", "12", "Center", "R0", "Instance",
                               symbolScene.gridTuple)
         leftPinLocs = [QPoint(-stubLength, (i + 1) * pinDistance) for i in
                        range(len(leftPinNames))]
-        rightPinLocs = [QPoint(rectXDim + stubLength, (i + 1) * pinDistance) for i
-                        in
+        rightPinLocs = [QPoint(rectXDim + stubLength, (i + 1) * pinDistance) for i in
                         range(len(rightPinNames))]
-        bottomPinLocs = [QPoint((i + 1) * pinDistance, rectYDim + stubLength) for
-                         i in
+        bottomPinLocs = [QPoint((i + 1) * pinDistance, rectYDim + stubLength) for i in
                          range(len(bottomPinNames))]
         topPinLocs = [QPoint((i + 1) * pinDistance, -stubLength) for i in
                       range(len(topPinNames))]
         for i in range(len(leftPinNames)):
-            symbolScene.lineDraw(leftPinLocs[i],
-                                 leftPinLocs[i] + QPoint(stubLength, 0),
+            symbolScene.lineDraw(leftPinLocs[i], leftPinLocs[i] + QPoint(stubLength, 0),
                                  symbolScene.symbolPen, symbolScene.gridTuple)
             symbolScene.addItem(
-                schematicPins[
-                    schematicPinNames.index(leftPinNames[i])].toSymbolPin(
+                schematicPins[schematicPinNames.index(leftPinNames[i])].toSymbolPin(
                     leftPinLocs[i], symbolScene.pinPen, symbolScene.gridTuple))
         for i in range(len(rightPinNames)):
-            symbolScene.lineDraw(rightPinLocs[i],
-                                 rightPinLocs[i] + QPoint(-stubLength, 0),
+            symbolScene.lineDraw(rightPinLocs[i], rightPinLocs[i] + QPoint(-stubLength, 0),
                                  symbolScene.symbolPen, symbolScene.gridTuple)
             symbolScene.addItem(
-                schematicPins[
-                    schematicPinNames.index(rightPinNames[i])].toSymbolPin(
+                schematicPins[schematicPinNames.index(rightPinNames[i])].toSymbolPin(
                     rightPinLocs[i], symbolScene.pinPen, symbolScene.gridTuple))
         for i in range(len(topPinNames)):
-            symbolScene.lineDraw(topPinLocs[i],
-                                 topPinLocs[i] + QPoint(0, stubLength),
+            symbolScene.lineDraw(topPinLocs[i], topPinLocs[i] + QPoint(0, stubLength),
                                  symbolScene.symbolPen, symbolScene.gridTuple)
             symbolScene.addItem(
-                schematicPins[
-                    schematicPinNames.index(topPinNames[i])].toSymbolPin(
+                schematicPins[schematicPinNames.index(topPinNames[i])].toSymbolPin(
                     topPinLocs[i], symbolScene.pinPen, symbolScene.gridTuple))
         for i in range(len(bottomPinNames)):
             symbolScene.lineDraw(bottomPinLocs[i],
                                  bottomPinLocs[i] + QPoint(0, -stubLength),
                                  symbolScene.symbolPen, symbolScene.gridTuple)
             symbolScene.addItem(
-                schematicPins[
-                    schematicPinNames.index(bottomPinNames[i])].toSymbolPin(
+                schematicPins[schematicPinNames.index(bottomPinNames[i])].toSymbolPin(
                     bottomPinLocs[i], symbolScene.pinPen,
                     symbolScene.gridTuple))  # symbol attribute generation for netlisting.
         symbolScene.attributeList = list()  # empty attribute list
 
-        symbolScene.attributeList.append(se.symbolAttribute("XyceNetlistLine",
-                                                            "X[@instName] [@cellName] [@pinList]"))
+        symbolScene.attributeList.append(
+            se.symbolAttribute("XyceNetlistLine", "X[@instName] [@cellName] [@pinList]"))
 
         symbolWindow.checkSaveCell()
         libraryView.reworkDesignLibrariesView(self.appMainW.libraryDict)
         # symbolWindow.show()
         return symbolViewItem
 
     def goDownHier(self):
         if self.selectedItems is not None:
             for item in self.selectedItems:
                 if isinstance(item, shp.symbolShape):
                     dlg = fd.goDownHierDialogue(self.editorWindow)
-                    libItem = libm.getLibItem(
-                        self.editorWindow.libraryView.libraryModel,
+                    libItem = libm.getLibItem(self.editorWindow.libraryView.libraryModel,
                         item.libraryName)
                     cellItem = libm.getCellItem(libItem, item.cellName)
-                    viewNames = [cellItem.child(i).text() for i in range(
-                        cellItem.rowCount()) if
+                    viewNames = [cellItem.child(i).text() for i in
+                                 range(cellItem.rowCount()) if
                                  cellItem.child(i).text() != item.viewName]
                     dlg.viewListCB.addItems(viewNames)
                     if dlg.exec() == QDialog.Accepted:
                         libItem = libm.getLibItem(
-                            self.editorWindow.libraryView.libraryModel,
-                            item.libraryName)
+                            self.editorWindow.libraryView.libraryModel, item.libraryName)
                         cellItem = libm.getCellItem(libItem, item.cellName)
-                        viewItem = libm.getViewItem(cellItem,
-                                                    dlg.viewListCB.currentText())
+                        viewItem = libm.getViewItem(cellItem, dlg.viewListCB.currentText())
                         openViewT = self.editorWindow.libraryView.libBrowsW.openCellView(
                             viewItem, cellItem, libItem)
                         if self.editorWindow.appMainW.openViews[openViewT]:
-                            childWindow = self.editorWindow.appMainW.openViews[
-                                openViewT]
+                            childWindow = self.editorWindow.appMainW.openViews[openViewT]
                             childWindow.parentView = self.editorWindow
+                            childWindow.schematicToolbar.addAction(childWindow.goUpAction)
                             if dlg.buttonId == 2:
                                 childWindow.centralW.scene.readOnly = True
 
     def goUpHier(self):
-        if self.editorWindow.parentView:
+        if self.editorWindow.parentView is not None:
             self.editorWindow.parentView.raise_()
             self.editorWindow.close()
 
+    def ignoreSymbol(self):
+        if self.selectedItems:
+            for item in self.selectedItems:
+                if isinstance(item, shp.symbolShape):
+                    item.netlistIgnore = not item.netlistIgnore
+        else:
+            self.logger.warning("No symbol selected")
+
 
 class editor_view(QGraphicsView):
     """
     The qgraphicsview for qgraphicsscene. It is used for both schematic and layout editors.
     """
 
     def __init__(self, scene, parent):
@@ -2632,16 +2624,15 @@
         if mouse_event.angleDelta().y() < 0:
             factor = 0.9
         view_pos = QPoint(int(mouse_event.globalPosition().x()),
                           int(mouse_event.globalPosition().y()))
         scene_pos = self.mapToScene(view_pos)
         self.centerOn(scene_pos)
         self.scale(factor, factor)
-        delta = self.mapToScene(view_pos) - self.mapToScene(
-            self.viewport().rect().center())
+        delta = self.mapToScene(view_pos) - self.mapToScene(self.viewport().rect().center())
         self.centerOn(scene_pos - delta)
         super().wheelEvent(mouse_event)
 
     def snapToBase(self, number, base):
         '''
         Restrict a number to the multiples of base
         '''
@@ -2656,18 +2647,16 @@
 
     def drawBackground(self, painter, rect):
 
         rectCoord = rect.getRect()
         if self.gridbackg:
             painter.fillRect(rect, QColor("black"))
             painter.setPen(QColor("gray"))
-            grid_x_start = math.ceil(rectCoord[0] / self.gridTuple[0]) * \
-                           self.gridTuple[0]
-            grid_y_start = math.ceil(rectCoord[1] / self.gridTuple[1]) * \
-                           self.gridTuple[1]
+            grid_x_start = math.ceil(rectCoord[0] / self.gridTuple[0]) * self.gridTuple[0]
+            grid_y_start = math.ceil(rectCoord[1] / self.gridTuple[1]) * self.gridTuple[1]
             num_x_points = math.floor(rectCoord[2] / self.gridTuple[0])
             num_y_points = math.floor(rectCoord[3] / self.gridTuple[1])
             for i in range(int(num_x_points)):  # rect width
                 for j in range(int(num_y_points)):  # rect length
                     painter.drawPoint(grid_x_start + i * self.gridTuple[0],
                                       grid_y_start + j * self.gridTuple[1], )
         elif self.linebackg:
@@ -2691,16 +2680,15 @@
 
     def keyPressEvent(self, key_event):
         if key_event.key() == Qt.Key_F:
             self.fitToView()
         super().keyPressEvent(key_event)
 
     def fitToView(self):
-        viewRect = self.scene.itemsBoundingRect().marginsAdded(
-            QMargins(40, 40, 40, 40))
+        viewRect = self.scene.itemsBoundingRect().marginsAdded(QMargins(40, 40, 40, 40))
         self.fitInView(viewRect, Qt.AspectRatioMode.KeepAspectRatio)
         self.show()
 
     def printView(self, printer):
         """
         Print view using selected Printer.
         """
@@ -2717,15 +2705,14 @@
     def revedaPrint(self, painter):
         self.drawBackground(painter, self.viewport().geometry())
         painter.drawText(self.viewport().geometry(), "Revolution EDA")
         self.render(painter)
         painter.end()
 
 
-
 class symbol_view(editor_view):
     def __init__(self, scene, parent):
         self.scene = scene
         self.parent = parent
         super().__init__(self.scene, self.parent)
         self.visibleRect = None
 
@@ -2737,15 +2724,15 @@
         super().__init__(self.scene, self.parent)
         self.visibleRect = None  # initialize to an empty rectangle
 
 
 class libraryBrowser(QMainWindow):
     def __init__(self, appMainW: QMainWindow) -> None:
         super().__init__()
-        self.resize(300,600)
+        self.resize(300, 600)
         self.appMainW = appMainW
         self.libraryDict = self.appMainW.libraryDict
         self.cellViews = self.appMainW.cellViews
         self.setWindowTitle("Library Browser")
         self._createMenuBar()
         self._createActions()
         self._createToolBars()
@@ -2766,16 +2753,15 @@
         openLibIcon = QIcon(":/icons/database--plus.png")
         self.openLibAction = QAction(openLibIcon, "Create/Open Lib...", self)
         self.openLibAction.setToolTip("Create/Open Lib...")
         self.libraryMenu.addAction(self.openLibAction)
         self.openLibAction.triggered.connect(self.openLibClick)
 
         libraryEditIcon = QIcon(":/icons/application-dialog.png")
-        self.libraryEditorAction = QAction(libraryEditIcon, "Library Editor",
-                                           self)
+        self.libraryEditorAction = QAction(libraryEditIcon, "Library Editor", self)
         self.libraryMenu.addAction(self.libraryEditorAction)
         self.libraryEditorAction.setToolTip("Open Library Editor...")
         self.libraryEditorAction.triggered.connect(self.libraryEditorClick)
 
         closeLibIcon = QIcon(":/icons/database-delete.png")
         self.closeLibAction = QAction(closeLibIcon, "Close Lib...", self)
         self.closeLibAction.setToolTip("Close Lib")
@@ -2795,30 +2781,27 @@
         self.deleteCellAction.setToolTip("Delete Cell")
         self.libraryMenu.addAction(self.deleteCellAction)
         self.deleteCellAction.triggered.connect(self.deleteCellClick)
 
         self.libraryMenu.addSeparator()
 
         newCellViewIcon = QIcon(":/icons/document--pencil.png")
-        self.newCellViewAction = QAction(newCellViewIcon,
-                                         "Create New CellView...", self)
+        self.newCellViewAction = QAction(newCellViewIcon, "Create New CellView...", self)
         self.newCellViewAction.setToolTip("Create New Cellview")
         self.libraryMenu.addAction(self.newCellViewAction)
         self.newCellViewAction.triggered.connect(self.newCellViewClick)
 
         openCellViewIcon = QIcon(":/icons/document--pencil.png")
-        self.openCellViewAction = QAction(openCellViewIcon, "Open CellView...",
-                                          self)
+        self.openCellViewAction = QAction(openCellViewIcon, "Open CellView...", self)
         self.openCellViewAction.setToolTip("Open CellView")
         self.libraryMenu.addAction(self.openCellViewAction)
         self.openCellViewAction.triggered.connect(self.openCellViewClick)
 
         deleteCellViewIcon = QIcon(":/icons/node-delete.png")
-        self.deleteCellViewAction = QAction(deleteCellViewIcon,
-                                            "Delete CellView...", self)
+        self.deleteCellViewAction = QAction(deleteCellViewIcon, "Delete CellView...", self)
         self.deleteCellViewAction.setToolTip("Delete Cellview")
         self.libraryMenu.addAction(self.deleteCellViewAction)
         self.deleteCellViewAction.triggered.connect(self.deleteCellViewClick)
 
     def _createToolBars(self):
         # Create tools bar called "main toolbar"
         toolbar = QToolBar("Main Toolbar", self)
@@ -2830,19 +2813,17 @@
         toolbar.addAction(self.newCellAction)
         toolbar.addAction(self.deleteCellAction)
         toolbar.addSeparator()
         toolbar.addAction(self.newCellViewAction)
         toolbar.addAction(self.openCellViewAction)
         toolbar.addAction(self.deleteCellViewAction)
 
-    def writeLibDefFile(self, libPathDict: dict,
-                        libFilePath: pathlib.Path) -> None:
+    def writeLibDefFile(self, libPathDict: dict, libFilePath: pathlib.Path) -> None:
 
-        libTempDict = dict(
-            zip(libPathDict.keys(), map(str, libPathDict.values())))
+        libTempDict = dict(zip(libPathDict.keys(), map(str, libPathDict.values())))
         try:
             with libFilePath.open(mode="w") as f:
                 json.dump({"libdefs": libTempDict}, f, indent=4)
             self.logger.info(f'Wrote library definition file in {libFilePath}')
         except IOError:
             self.logger.error(f"Cannot save library definitions in {libFilePath}")
 
@@ -2909,16 +2890,15 @@
             self.logger.error("Please enter a cell name.")
         else:
             scb.createCell(parent, libraryModel, libItem, cellName)
 
     def deleteCellClick(self, s):
         dlg = fd.deleteCellDialog(self, self.libraryModel)
         if dlg.exec() == QDialog.Accepted:
-            libItem = libm.getLibItem(self.libraryModel,
-                                      dlg.libNamesCB.currentText())
+            libItem = libm.getLibItem(self.libraryModel, dlg.libNamesCB.currentText())
             if dlg.cellCB.currentText().strip() == "":
                 self.logger.error("Please enter a cell name.")
             else:
                 # cellItemsLib = {libItem.child(i).cellName: libItem.child(i) for i in
                 #                 range(libItem.rowCount())}
                 # cellItem = cellItemsLib.get(dlg.cellCB.currentText())
                 cellItem = libm.getCellItem(libItem, dlg.cellCB.currentText())
@@ -2927,19 +2907,17 @@
                 cellItem.parent().removeRow(cellItem.row())
 
     def newCellViewClick(self, s):
         dlg = fd.newCellViewDialog(self, self.libraryModel)
         dlg.viewType.addItems(self.cellViews)
         if dlg.exec() == QDialog.Accepted:
             # cellPath = dlg.selectedLibPath.joinpath(dlg.cellCB.currentText())
-            libItem = libm.getLibItem(self.libraryModel,
-                                      dlg.libNamesCB.currentText())
+            libItem = libm.getLibItem(self.libraryModel, dlg.libNamesCB.currentText())
             cellItem = libm.getCellItem(libItem, dlg.cellCB.currentText())
-            viewItem = scb.createCellView(self.appMainW,
-                                          dlg.viewName.text().strip(),
+            viewItem = scb.createCellView(self.appMainW, dlg.viewName.text().strip(),
                                           cellItem)
             self.createNewCellView(libItem, cellItem, viewItem)
 
     def createNewCellView(self, libItem, cellItem, viewItem):
         viewTuple = ddef.viewTuple(libItem.libraryName, cellItem.cellName,
                                    viewItem.viewName)
         match viewItem.viewType:
@@ -2954,42 +2932,39 @@
                 dlg.viewNameCB.addItems(schViewsList)
                 dlg.switchViews.setText(", ".join(self.appMainW.switchViewList))
                 dlg.stopViews.setText(", ".join(self.appMainW.stopViewList))
                 # dlg.switchViews.setText(self.)
                 if dlg.exec() == QDialog.Accepted:
                     selectedSchName = dlg.viewNameCB.currentText()
                     selectedSchItem = libm.getViewItem(cellItem, selectedSchName)
-                    schematicWindow = schematicEditor(selectedSchItem,
-                                                      self.libraryDict,
+                    schematicWindow = schematicEditor(selectedSchItem, self.libraryDict,
                                                       self.libBrowserCont.designView, )
                     schematicWindow.loadSchematic()
                     switchViewList = [viewName.strip() for viewName in
                                       dlg.switchViews.text().split(",")]
                     stopViewList = [viewName.strip() for viewName in
                                     dlg.stopViews.text().split(",")]
                     schematicWindow.switchViewList = switchViewList
                     schematicWindow.stopViewList = stopViewList
                     schematicWindow.configDict = dict()  # clear config dictionary
 
                     # clear netlisted cells list
                     newConfigDict = dict()  # create an empty newconfig dict
-                    schematicWindow.createConfigView(viewItem,
-                                                     schematicWindow.configDict,
+                    schematicWindow.createConfigView(viewItem, schematicWindow.configDict,
                                                      newConfigDict,
                                                      schematicWindow.processedCells)
                     configFilePathObj = viewItem.data(Qt.UserRole + 2)
                     items = list()
                     items.insert(0, {"cellView": "config"})
                     items.insert(1, {"reference": selectedSchName})
                     items.insert(2, schematicWindow.configDict)
                     with configFilePathObj.open(mode="w+") as configFile:
                         json.dump(items, configFile, indent=4)
 
-                    configWindow = self.openConfigEditWindow(
-                        schematicWindow.configDict,
+                    configWindow = self.openConfigEditWindow(schematicWindow.configDict,
                         selectedSchItem, viewItem)
                     self.appMainW.openViews[viewTuple] = configWindow
             case "schematic":
                 # scb.createCellView(self.appMainW, viewItem.viewName, cellItem)
                 schematicWindow = schematicEditor(viewItem, self.libraryDict,
                                                   self.libBrowserCont.designView)
                 self.appMainW.openViews[viewTuple] = schematicWindow
@@ -3008,21 +2983,19 @@
                     self.editProcess = QProcess()
                     self.editProcess.finished.connect(self.editProcessFinished)
                     self.editProcess.start(str(self.appMainW.textEditorPath), [])
 
     def openConfigEditWindow(self, configDict, schViewItem, viewItem):
         schematicName = schViewItem.viewName
         libItem = schViewItem.parent().parent()
-        configWindow = configViewEdit(self.appMainW, schViewItem, configDict,
-                                      viewItem)
+        configWindow = configViewEdit(self.appMainW, schViewItem, configDict, viewItem)
         configWindow.centralWidget.libraryNameEdit.setText(libItem.libraryName)
         cellItem = viewItem.parent()
         configWindow.centralWidget.cellNameEdit.setText(cellItem.cellName)
-        schViewsList = [cellItem.child(row).viewName for row in
-                        range(cellItem.rowCount())
+        schViewsList = [cellItem.child(row).viewName for row in range(cellItem.rowCount())
                         if cellItem.child(row).viewType == "schematic"]
         configWindow.centralWidget.viewNameCB.addItems(schViewsList)
         configWindow.centralWidget.viewNameCB.setCurrentText(schematicName)
         configWindow.centralWidget.switchViewsEdit.setText(
             ", ".join(self.appMainW.switchViewList))
         configWindow.centralWidget.stopViewsEdit.setText(
             ", ".join(self.appMainW.stopViewList))
@@ -3074,29 +3047,27 @@
                 with open(viewItem.viewPath) as tempFile:
                     items = json.load(tempFile)
                 if items[1]["filePath"]:
                     if self.editProcess is None:
                         self.editProcess = QProcess()
                         VerilogafilePathObj = viewItem.parent().data(
                             Qt.UserRole + 2).joinpath(items[1]["filePath"])
-                        self.editProcess.finished.connect(
-                            self.editProcessFinished)
+                        self.editProcess.finished.connect(self.editProcessFinished)
                         self.editProcess.start(self.appMainW.textEditorPath,
                                                [str(VerilogafilePathObj)])
                 else:
                     self.logger.warning("File path not defined.")
             elif viewItem.viewType == "config":
                 with open(viewItem.viewPath) as tempFile:
                     items = json.load(tempFile)
                 viewName = items[0]["viewName"]
                 schematicName = items[1]["reference"]
                 schViewItem = libm.getViewItem(cellItem, schematicName)
                 configDict = items[2]
-                configWindow = self.openConfigEditWindow(configDict, schViewItem,
-                                                         viewItem)
+                configWindow = self.openConfigEditWindow(configDict, schViewItem, viewItem)
                 self.appMainW.openViews[openCellViewTuple] = configWindow
         return openCellViewTuple
 
     def editProcessFinished(self):
         self.appMainW.importVerilogaClick()
         self.editProcess = None
 
@@ -3126,15 +3097,15 @@
         self.layout.addWidget(self.designView)
         self.setLayout(self.layout)
 
 
 class designLibrariesView(QTreeView):
     def __init__(self, parent):
         super().__init__(parent=parent)  # QTreeView
-        self.parent = parent  # type: QWidget (libraryBrowserContainer)
+        self.parent = parent
         self.setSelectionMode(QAbstractItemView.SingleSelection)
         self.viewCounter = 0
         self.libBrowsW = self.parent.parent
         self.appMainW = self.libBrowsW.appMainW
         self.libraryDict = self.appMainW.libraryDict  # type: dict
         self.cellViews = self.appMainW.cellViews  # type: list
         self.openViews = self.appMainW.openViews  # type: dict
@@ -3168,16 +3139,15 @@
     def createCell(self):
         dlg = fd.createCellDialog(self, self.libraryModel)
         assert isinstance(self.selectedItem, scb.libraryItem)
         dlg.libNamesCB.setCurrentText(self.selectedItem.libraryName)
         if dlg.exec() == QDialog.Accepted:
             cellName = dlg.cellCB.currentText()
             if cellName.strip() != '':
-                scb.createCell(self, self.libraryModel, self.selectedItem,
-                               cellName)
+                scb.createCell(self, self.libraryModel, self.selectedItem, cellName)
             else:
                 self.logger.error("Please enter a cell name.")
 
     def copyCell(self):
         dlg = fd.copyCellDialog(self, self.libraryModel, self.selectedItem)
 
         if dlg.exec() == QDialog.Accepted:
@@ -3198,16 +3168,15 @@
             self.logger.warning(f"Error:{e}")
 
     def createCellView(self):
         dlg = fd.createCellViewDialog(self, self.libraryModel, self.selectedItem)
         if dlg.exec() == QDialog.Accepted:
             viewItem = scb.createCellView(self.appMainW, dlg.nameEdit.text(),
                                           self.selectedItem)
-            self.libBrowsW.createNewCellView(self.selectedItem.parent(),
-                                             self.selectedItem,
+            self.libBrowsW.createNewCellView(self.selectedItem.parent(), self.selectedItem,
                                              viewItem)
 
     def openView(self):
         viewItem = self.selectedItem
         cellItem = viewItem.parent()
         libItem = cellItem.parent()
         self.libBrowsW.openCellView(viewItem, cellItem, libItem)
@@ -3218,22 +3187,19 @@
             if self.selectedItem.data(Qt.UserRole + 1) == "view":
                 viewPath = self.selectedItem.data(Qt.UserRole + 2)
                 selectedLibItem = libm.getLibItem(self.libraryModel,
                                                   dlg.libNamesCB.currentText())
                 cellName = dlg.cellCB.currentText()
                 libCellNames = [selectedLibItem.child(row).cellName for row in
                                 range(selectedLibItem.rowCount())]
-                if (
-                        cellName in libCellNames):  # check if there is the cell in the library
-                    cellItem = libm.getCellItem(selectedLibItem,
-                                                dlg.cellCB.currentText())
+                if (cellName in libCellNames):  # check if there is the cell in the library
+                    cellItem = libm.getCellItem(selectedLibItem, dlg.cellCB.currentText())
                 else:
                     cellItem = scb.createCell(self.libBrowsW, self.libraryModel,
-                                              selectedLibItem,
-                                              dlg.cellCB.currentText(), )
+                                              selectedLibItem, dlg.cellCB.currentText(), )
                 cellViewNames = [cellItem.child(row).viewName for row in
                                  range(cellItem.rowCount())]
                 newViewName = dlg.viewName.text()
                 if newViewName in cellViewNames:
                     self.logger.warning(
                         "View already exists. Delete cellview and try again.")
                 else:
@@ -3262,15 +3228,15 @@
             itemRow = self.selectedItem.row()
             parent = self.selectedItem.parent()
             parent.removeRow(itemRow)
         except OSError as e:
             # print(f"Error:{e.strerror}")
             self.logger.warning(f"Error:{e.strerror}")
 
-    def reworkDesignLibrariesView(self,libraryDict:dict):
+    def reworkDesignLibrariesView(self, libraryDict: dict):
         """
         Recreate library model from libraryDict.
         """
         self.libraryModel = designLibrariesModel(libraryDict)
         self.setModel(self.libraryModel)
         self.libBrowsW.libraryModel = self.libraryModel
 
@@ -3285,31 +3251,23 @@
             self.selectedItem = self.libraryModel.itemFromIndex(index)
             if self.selectedItem.data(Qt.UserRole + 1) == "library":
                 menu.addAction("Rename Library", self.renameLib)
                 menu.addAction("Remove Library", self.removeLibrary)
                 menu.addAction("Create Cell", self.createCell)
             elif self.selectedItem.data(Qt.UserRole + 1) == "cell":
                 menu.addAction(
-                    QAction("Create CellView...", self,
-                            triggered=self.createCellView))
-                menu.addAction(
-                    QAction("Copy Cell...", self, triggered=self.copyCell))
-                menu.addAction(
-                    QAction("Rename Cell...", self, triggered=self.renameCell))
-                menu.addAction(
-                    QAction("Delete Cell...", self, triggered=self.deleteCell))
+                    QAction("Create CellView...", self, triggered=self.createCellView))
+                menu.addAction(QAction("Copy Cell...", self, triggered=self.copyCell))
+                menu.addAction(QAction("Rename Cell...", self, triggered=self.renameCell))
+                menu.addAction(QAction("Delete Cell...", self, triggered=self.deleteCell))
             elif self.selectedItem.data(Qt.UserRole + 1) == "view":
-                menu.addAction(
-                    QAction("Open View", self, triggered=self.openView))
-                menu.addAction(
-                    QAction("Copy View...", self, triggered=self.copyView))
-                menu.addAction(
-                    QAction("Rename View...", self, triggered=self.renameView))
-                menu.addAction(
-                    QAction("Delete View...", self, triggered=self.deleteView))
+                menu.addAction(QAction("Open View", self, triggered=self.openView))
+                menu.addAction(QAction("Copy View...", self, triggered=self.copyView))
+                menu.addAction(QAction("Rename View...", self, triggered=self.renameView))
+                menu.addAction(QAction("Delete View...", self, triggered=self.deleteView))
             menu.exec(event.globalPos())
         except UnboundLocalError:
             pass
 
 
 class designLibrariesModel(QStandardItemModel):
     def __init__(self, libraryDict):
@@ -3325,21 +3283,18 @@
 
     def populateLibrary(self, designPath):  # designPath: Path
         """
         Populate library view.
         """
         if designPath.joinpath("reveda.lib").exists():
             libraryItem = self.addLibraryToModel(designPath)
-            cellList = [cell.name for cell in designPath.iterdir() if
-                        cell.is_dir()]
+            cellList = [cell.name for cell in designPath.iterdir() if cell.is_dir()]
             for cell in cellList:  # type: str
-                cellItem = self.addCellToModel(designPath.joinpath(cell),
-                                               libraryItem)
-                viewList = [view.name for view in
-                            designPath.joinpath(cell).iterdir() if
+                cellItem = self.addCellToModel(designPath.joinpath(cell), libraryItem)
+                viewList = [view.name for view in designPath.joinpath(cell).iterdir() if
                             view.suffix == ".json"]
                 for view in viewList:
                     self.addViewToModel(designPath.joinpath(cell, view), cellItem)
 
     def addLibraryToModel(self, designPath):
         libraryEntry = scb.libraryItem(designPath)
         self.rootItem.appendRow(libraryEntry)
@@ -3391,21 +3346,18 @@
 
     def populateLibrary(self, designPath):  # designPath: Path
         """
         Populate library view.
         """
         if designPath.joinpath("reveda.lib").exists():
             libraryItem = self.addLibraryToModel(designPath)
-            cellList = [cell.name for cell in designPath.iterdir() if
-                        cell.is_dir()]
+            cellList = [cell.name for cell in designPath.iterdir() if cell.is_dir()]
             for cell in cellList:  # type: str
-                cellItem = self.addCellToModel(designPath.joinpath(cell),
-                                               libraryItem)
-                viewList = [view.name for view in
-                            designPath.joinpath(cell).iterdir() if
+                cellItem = self.addCellToModel(designPath.joinpath(cell), libraryItem)
+                viewList = [view.name for view in designPath.joinpath(cell).iterdir() if
                             view.suffix == ".json" and "symbol" in view.name]
                 for view in viewList:
                     self.addViewToModel(designPath.joinpath(cell, view), cellItem)
 
 
 class xyceNetlist:
     def __init__(self, schematic: schematicEditor, filePathObj: pathlib.Path,
@@ -3423,21 +3375,20 @@
 
         self.switchViewList = schematic.switchViewList
         self.stopViewList = schematic.stopViewList
         self.netlistedViewsSet = set()  # keeps track of netlisted views.
 
     def writeNetlist(self):
         with self.filePathObj.open(mode="w") as cirFile:
-            cirFile.write(
-                '*'.join(['\n', 80 * "*", "\n", "* Revolution EDA CDL Netlist\n",
-                          f"* Library: {self.schematic.libName}\n",
-                          f"* Top Cell Name: {self.schematic.cellName}\n",
-                          f"* View Name: {self.schematic.viewName}\n",
-                          f"* Date: {datetime.datetime.now()}\n", 80 * "*", "\n",
-                          ".GLOBAL gnd!\n\n"]))
+            cirFile.write('*'.join(['\n', 80 * "*", "\n", "* Revolution EDA CDL Netlist\n",
+                                    f"* Library: {self.schematic.libName}\n",
+                                    f"* Top Cell Name: {self.schematic.cellName}\n",
+                                    f"* View Name: {self.schematic.viewName}\n",
+                                    f"* Date: {datetime.datetime.now()}\n", 80 * "*", "\n",
+                                    ".GLOBAL gnd!\n\n"]))
 
             # now go down the rabbit hole to track all circuit elements.
             self.recursiveNetlisting(self.schematic, cirFile)
 
             cirFile.write(".END\n")
 
     @property
@@ -3457,88 +3408,81 @@
             schematicScene = schematic.centralW.scene
             schematicScene.groupAllNets()  # name all nets in the
             # schematic
             sceneSymbolSet = schematicScene.findSceneSymbolSet()
             schematicScene.generatePinNetMap(sceneSymbolSet)
             for item in sceneSymbolSet:
                 if item.attr.get("XyceNetlistLine") and item.attr.get(
-                        "XyceNetlistPass") != '1':
-                    self.netlistedViewsSet.add(ddef.viewTuple(item.libraryName,
-                                                              item.cellName,
-                                                              item.viewName))
+                        "XyceNetlistPass") != '1' and (not item.netlistIgnore):
+                    self.netlistedViewsSet.add(
+                        ddef.viewTuple(item.libraryName, item.cellName, item.viewName))
                     libItem = libm.getLibItem(schematic.libraryView.libraryModel,
                                               item.libraryName)
                     cellItem = libm.getCellItem(libItem, item.cellName)
-                    viewItems = [cellItem.child(row) for row in
-                                 range(cellItem.rowCount())]
+                    viewItems = [cellItem.child(row) for row in range(cellItem.rowCount())]
                     viewNames = [view.viewName for view in viewItems]
 
                     viewDict = dict(zip(viewNames, viewItems))
                     if self._use_config:
                         netlistableViews = [self.configDict.get(item.cellName)[1]]
                     else:
                         netlistableViews = [viewItemName for viewItemName in
                                             self.switchViewList if
                                             viewItemName in viewNames]
                     # now create the netlist line for that item.
 
                     self.createItemLine(cirFile, item, netlistableViews, viewDict)
+                elif item.netlistIgnore:
+                    cirFile.write(f'*{item.instanceName} is marked to be ignored\n')
                 elif not item.attr.get("XyceNetlistPass", False):
                     cirFile.write(f'*{item.instanceName} has no '
                                   f'XyceNetlistLine attribute\n')
-            # print(f'netlisted views: {self.netlistedViewsSet}')
+
         except Exception as e:
             self.schematic.logger.error(e)
 
-    def createItemLine(self, cirFile, item, netlistableViews: list,
-                       viewDict: dict):
+    def createItemLine(self, cirFile, item, netlistableViews: list, viewDict: dict):
         for viewName in netlistableViews:
-            if viewName in viewDict.keys():
-                viewTuple = ddef.viewTuple(item.libraryName, item.cellName,
-                                           viewName)
+            if viewName in viewDict:
+                viewTuple = ddef.viewTuple(item.libraryName, item.cellName, viewName)
                 # print(viewTuple)
                 if viewDict[viewName].viewType == "schematic":
                     cirFile.write(self.createXyceSymbolLine(item))
 
-                    schematicObj = schematicEditor(viewDict[viewName],
-                                                   self.libraryDict,
+                    schematicObj = schematicEditor(viewDict[viewName], self.libraryDict,
                                                    self.libraryView, )
 
                     schematicObj.loadSchematic()
                     if viewTuple not in self.netlistedViewsSet:
                         self.netlistedViewsSet.add(viewTuple)
                         # print(f'{schematicObj.cellName} {schematicObj.viewName}')
                         pinList = " ".join(item.pinNetMap.keys())
-                        cirFile.write(
-                            f".SUBCKT {schematicObj.cellName} {pinList}\n")
+                        cirFile.write(f".SUBCKT {schematicObj.cellName} {pinList}\n")
                         self.recursiveNetlisting(schematicObj, cirFile)
                         cirFile.write(".ENDS\n")
                 elif viewDict[viewName].viewType == "veriloga":
-                    with viewDict[viewName].data(Qt.UserRole + 2).open(
-                            mode="r") as vaview:
+                    with viewDict[viewName].data(Qt.UserRole + 2).open(mode="r") as vaview:
                         items = json.load(vaview)
                     netlistLine = items[3]['netlistLine']
-                    netlistLine = netlistLine.replace("[@instName]",
-                                                      f"{item.instanceName}")
+                    netlistLine = netlistLine.replace("[@instName]", f"{item.instanceName}")
                     # TODO: fix veriloga netlisting
                     # for pinName, netName in item.pinNetMap.items():
                     #     netlistLine = netlistLine.replace(f"[|{pinName}:%]", f"{netName}")
                     pinList = " ".join(item.pinNetMap.values())
                     netlistLine = netlistLine.replace("[@pinList]", pinList)
                     for labelItem in item.labels.values():
                         if labelItem.labelDefinition in netlistLine:
-                            netlistLine = netlistLine.replace(
-                                labelItem.labelDefinition,
+                            netlistLine = netlistLine.replace(labelItem.labelDefinition,
                                 labelItem.labelText)
                     cirFile.write(f"{netlistLine}\n")
                     self.netlistedViewsSet.add(viewTuple)
                 elif viewDict[viewName].viewType == "symbol":
                     cirFile.write(f"{self.createXyceSymbolLine(item)}")
-                    self.netlistedViewsSet.add(ddef.viewTuple(
-                        item.libraryName, item.cellName, item.viewName))
+                    self.netlistedViewsSet.add(
+                        ddef.viewTuple(item.libraryName, item.cellName, item.viewName))
                 break
 
     def createXyceSymbolLine(self, item):
         """
         Create a netlist line from a nlp device format line.
         """
         try:
@@ -3546,18 +3490,19 @@
             for labelItem in item.labels.values():
                 if labelItem.labelDefinition in xyceNetlistFormatLine:
                     xyceNetlistFormatLine = xyceNetlistFormatLine.replace(
                         labelItem.labelDefinition, labelItem.labelText)
 
             for attrb, value in item.attr.items():
                 if f'[%{attrb}]' in xyceNetlistFormatLine:
-                    xyceNetlistFormatLine = xyceNetlistFormatLine.replace(
-                        f'[%{attrb}]', value)
+                    xyceNetlistFormatLine = xyceNetlistFormatLine.replace(f'[%{attrb}]',
+                        value)
             pinList = " ".join(item.pinNetMap.values())
-            xyceNetlistFormatLine = xyceNetlistFormatLine.replace('[@pinList]', pinList)+'\n'
+            xyceNetlistFormatLine = xyceNetlistFormatLine.replace('[@pinList]',
+                                                                  pinList) + '\n'
             return xyceNetlistFormatLine
         except Exception as e:
             self._scene.logger.error(e)
             self._scene.logger.error(f"Netlist line is not defined for"
                                      f" {item.instanceName}")
             # if there is no NLPDeviceFormat line, create a warning line
             return f"*Netlist line is not defined for symbol of {item.instanceName}\n"
@@ -3605,33 +3550,28 @@
         self.configDict = dict()
         newConfigDict = dict()
         model = self.centralWidget.confModel
         for i in range(model.rowCount()):
             viewList = [item.strip() for item in
                         model.itemFromIndex(model.index(i, 3)).text().split(',')]
             self.configDict[model.item(i, 1).text()] = [model.item(i, 0).text(),
-                                                        model.item(i, 2).text(),
-                                                        viewList]
+                                                        model.item(i, 2).text(), viewList]
         if self.appmainW.libraryBrowser is None:
             self.appmainW.createLibraryBrowser()
-        topSchematicWindow = schematicEditor(self.schViewItem,
-                                             self.appmainW.libraryDict,
+        topSchematicWindow = schematicEditor(self.schViewItem, self.appmainW.libraryDict,
                                              self.appmainW.libraryBrowser.libBrowserCont.designView)
         topSchematicWindow.loadSchematic()
-        topSchematicWindow.createConfigView(self.viewItem, self.configDict,
-                                            newConfigDict,
+        topSchematicWindow.createConfigView(self.viewItem, self.configDict, newConfigDict,
                                             topSchematicWindow.processedCells)
         self.configDict = newConfigDict
 
         self.centralWidget.confModel = configModel(self.configDict)
         # self.centralWidget.configDictGroup.setVisible(False)
-        self.centralWidget.configDictLayout.removeWidget(
-            self.centralWidget.configViewTable)
-        self.centralWidget.configViewTable = configTable(
-            self.centralWidget.confModel)
+        self.centralWidget.configDictLayout.removeWidget(self.centralWidget.configViewTable)
+        self.centralWidget.configViewTable = configTable(self.centralWidget.confModel)
         self.centralWidget.configDictLayout.addWidget(
             self.centralWidget.configViewTable)  # self.centralWidget.configDictGroup.setVisible(True)
 
     def saveClick(self):
         configFilePathObj = self.viewItem.data(Qt.UserRole + 2)
         items = list()
         items.insert(0, {"viewName": "config"})
@@ -3675,17 +3615,16 @@
 
 
 class configModel(QStandardItemModel):
     def __init__(self, configDict: dict):
         row = len(configDict.keys())
         column = 4
         super().__init__(row, column)
-        self.setHorizontalHeaderLabels(
-            ['Library', 'Cell Name', 'View Found', 'View To '
-                                                   'Use'])
+        self.setHorizontalHeaderLabels(['Library', 'Cell Name', 'View Found', 'View To '
+                                                                              'Use'])
         for i, (k, v) in enumerate(configDict.items()):
             item = QStandardItem(v[0])
             self.setItem(i, 0, item)
             item = QStandardItem(k)
             self.setItem(i, 1, item)
             item = QStandardItem(v[1])
             self.setItem(i, 2, item)
@@ -3701,16 +3640,15 @@
         self.combos = list()
         self.horizontalHeader().setStretchLastSection(True)
         self.setSelectionMode(QTableView.SingleSelection)
         self.setEditTriggers(QTableView.NoEditTriggers)
         for row in range(self.model.rowCount()):
             self.combos.append(QComboBox())
             items = [item.strip() for item in
-                     self.model.itemFromIndex(
-                         self.model.index(row, 3)).text().split(',')]
+                     self.model.itemFromIndex(self.model.index(row, 3)).text().split(',')]
             self.combos[-1].addItems(items)
             self.combos[-1].setCurrentText(
                 self.model.itemFromIndex(self.model.index(row, 2)).text())
             self.setIndexWidget(self.model.index(row, 3), self.combos[-1])
 
     def updateModel(self):
         for row in range(self.model.rowCount()):
@@ -3727,8 +3665,7 @@
 
     @Slot()
     def run(self) -> None:
         try:
             self.fn
         except Exception as e:
             print(e)
-
```

### Comparing `revolution-eda-0.5.1/revedaEditor/gui/fileDialogues.py` & `revolution-eda-0.5.2/revedaEditor/gui/fileDialogues.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,633 +1,633 @@
-#   “Commons Clause” License Condition v1.0
-#  #
-#   The Software is provided to you by the Licensor under the License, as defined
-#   below, subject to the following condition.
-#  #
-#   Without limiting other conditions in the License, the grant of rights under the
-#   License will not include, and the License does not grant to you, the right to
-#   Sell the Software.
-#  #
-#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
-#   granted to you under the License to provide to third parties, for a fee or other
-#   consideration (including without limitation fees for hosting or consulting/
-#   support services related to the Software), a product or service whose value
-#   derives, entirely or substantially, from the functionality of the Software. Any
-#   license notice or attribution required by the License must also include this
-#   Commons Clause License Condition notice.
-#  #
-#   Software: Revolution EDA
-#   License: Mozilla Public License 2.0
-#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
-
-import pathlib
-
-import revedaEditor.backend.libraryMethods as libm
-import revedaEditor.common.shape as shp
-import revedaEditor.gui.editFunctions as edf
-from PySide6.QtCore import (Qt, QDir)
-from PySide6.QtGui import (QStandardItemModel, QStandardItem)
-from PySide6.QtWidgets import (QComboBox, QDialog, QDialogButtonBox, QFileDialog,
-                               QFormLayout, QHBoxLayout, QLabel, QLineEdit,
-                               QVBoxLayout, QRadioButton, QButtonGroup,
-                               QPushButton, QGroupBox, QTableView, QMenu,
-                               QCheckBox)
-
-
-class createCellDialog(QDialog):
-    def __init__(self, parent, model):
-        super().__init__(parent=parent)
-        self.parent = parent
-        self.model = model
-        self.init_UI()
-
-    def init_UI(self):
-        self.setWindowTitle("Create Cell")
-        self.layout = QFormLayout()
-        self.layout.setSpacing(10)
-        self.libNamesCB = QComboBox()
-        self.libNamesCB.setModel(self.model)
-        self.libNamesCB.setModelColumn(0)
-        self.libNamesCB.setCurrentIndex(0)
-        self.libNamesCB.currentTextChanged.connect(self.selectLibrary)
-        self.layout.addRow(edf.boldLabel("Library:"), self.libNamesCB)
-        self.cellCB = QComboBox()
-        libItem = libm.getLibItem(self.model, self.libNamesCB.currentText())
-        self.cellList = [libItem.child(i).cellName for i in range(libItem.rowCount())]
-        self.cellCB.addItems(self.cellList)
-        self.cellCB.setEditable(True)
-        self.layout.addRow(edf.boldLabel("Cell Name:"), self.cellCB)
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        self.layout.addWidget(self.buttonBox)
-        self.setLayout(self.layout)
-
-    def selectLibrary(self):
-        libItem = libm.getLibItem(self.model, self.libNamesCB.currentText())
-        cellList = [libItem.child(i).cellName for i in range(libItem.rowCount())]
-        self.cellCB.clear()
-        self.cellCB.addItems(cellList)
-
-
-
-class deleteCellDialog(createCellDialog):
-    def __init__(self, parent, model):
-        super().__init__(parent, model)
-        self.cellCB.setEditable(False)
-        self.setWindowTitle('Delete Cell')
-
-
-class newCellViewDialog(createCellDialog):
-    def __init__(self, parent, model):
-        super().__init__(parent, model)
-        self.cellCB.setEditable(False)
-        self.setWindowTitle('Create Cell View')
-        self.viewType = QComboBox()
-        self.layout.addRow(edf.boldLabel("View Type:"), self.viewType)
-        self.viewName = edf.longLineEdit()
-        self.layout.addRow(edf.boldLabel('View Name:'), self.viewName)
-        self.layout.setSpacing(10)
-        self.layout.addWidget(self.buttonBox)
-        self.setLayout(self.layout)
-
-
-class selectCellViewDialog(deleteCellDialog):
-    def __init__(self, parent, model):
-        super().__init__(parent=parent, model=model)
-        libItem = libm.getLibItem(self.model, self.libNamesCB.currentText())
-        self.setWindowTitle("Select CellView")
-        self.cellCB.currentTextChanged.connect(self.cellNameChanged)
-        self.viewCB = QComboBox()
-        cellItem = libm.getCellItem(libItem, self.cellCB.currentText())
-        self.viewCB.addItems(
-            [cellItem.child(i).text() for i in range(cellItem.rowCount())])
-
-        self.layout.addRow(edf.boldLabel('View Name:'), self.viewCB)
-        self.layout.setSpacing(10)
-        self.layout.addWidget(self.buttonBox)
-        self.setLayout(self.layout)
-
-    def cellNameChanged(self):
-        libItem = libm.getLibItem(self.model, self.libNamesCB.currentText())
-        cellItem = libm.getCellItem(libItem, self.cellCB.currentText())
-        if cellItem is not None:
-            viewList = [cellItem.child(i).text() for i in range(cellItem.rowCount())]
-        else:
-            viewList = []
-        self.viewCB.clear()
-        self.viewCB.addItems(viewList)
-
-
-class createCellViewDialog(QDialog):
-    def __init__(self, parent, model, cellItem):
-        super().__init__(parent=parent)
-        self.parent = parent
-        self.model = model
-        self.cellItem = cellItem
-        self.cellPath = self.cellItem.data(Qt.UserRole + 2)
-        self.init_UI()
-
-    def init_UI(self):
-        self.setWindowTitle("Create CellView")
-        layout = QFormLayout()
-        layout.setSpacing(10)
-        self.viewComboBox = QComboBox()
-        self.viewComboBox.addItems(self.parent.cellViews)
-        layout.addRow("Select View:", self.viewComboBox)
-        self.nameEdit = QLineEdit()
-        self.nameEdit.setPlaceholderText("CellView Name")
-        self.nameEdit.setFixedWidth(200)
-        layout.addRow(QLabel("View Name:"), self.nameEdit)
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        layout.addRow(self.buttonBox)
-        self.setLayout(layout)
-
-
-class renameCellDialog(QDialog):
-    def __init__(self, parent, cellItem):
-        super().__init__(parent=parent)
-        self.parent = parent
-        self.cellItem = cellItem
-
-        self.init_UI()
-
-    def init_UI(self):
-        self.setWindowTitle("Rename Cell")
-        layout = QFormLayout()
-        layout.setSpacing(10)
-        self.nameEdit = QLineEdit()
-        self.nameEdit.setPlaceholderText("Cell Name")
-        self.nameEdit.setFixedWidth(200)
-        layout.addRow(QLabel("Cell Name:"), self.nameEdit)
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        layout.addRow(self.buttonBox)
-        self.setLayout(layout)
-
-
-class copyCellDialog(QDialog):
-    def __init__(self, parent, model, cellItem):
-        super().__init__(parent=parent)
-        self.parent = parent
-        self.model = model
-        self.cellItem = cellItem
-
-        # self.index = 0
-        self.init_UI()
-
-    def init_UI(self):
-        self.setWindowTitle("Copy Cell")
-        layout = QFormLayout()
-        layout.setSpacing(10)
-        self.libraryComboBox = QComboBox()
-        self.libraryComboBox.setModel(self.model)
-        self.libraryComboBox.setModelColumn(0)
-        self.libraryComboBox.setCurrentIndex(0)
-        self.selectedLibPath = self.libraryComboBox.itemData(0, Qt.UserRole + 2)
-        self.libraryComboBox.currentTextChanged.connect(self.selectLibrary)
-        layout.addRow(QLabel("Library:"), self.libraryComboBox)
-        self.copyName = QLineEdit()
-        self.copyName.setPlaceholderText("Enter Cell Name")
-        self.copyName.setFixedWidth(130)
-        layout.addRow(QLabel("Cell Name:"), self.copyName)
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        layout.addRow(self.buttonBox)
-        self.setLayout(layout)
-
-    def selectLibrary(self):
-        self.selectedLibPath = self.libraryComboBox.itemData(
-            self.libraryComboBox.currentIndex(), Qt.UserRole + 2)
-
-
-class copyViewDialog(createCellDialog):
-    def __init__(self, parent, model):
-        super().__init__(parent=parent, model=model)
-        self.setWindowTitle('Copy View')
-        self.cellCB.setEditable(True)
-        self.cellCB.InsertPolicy = QComboBox.InsertAfterCurrent
-        self.viewName = edf.longLineEdit()
-        self.layout.addRow(edf.boldLabel('View Name:'), self.viewName)
-        self.layout.setSpacing(10)
-        self.layout.addWidget(self.buttonBox)
-        self.setLayout(self.layout)
-
-
-class closeLibDialog(QDialog):
-    def __init__(self, libraryDict, parent, *args):
-        super().__init__(parent, *args)
-        self.libraryDict = libraryDict
-        self.setWindowTitle('Select Library to close')
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-
-        layout = QVBoxLayout()
-        formLayout = QFormLayout()
-        self.libNamesCB = QComboBox()
-        self.libNamesCB.addItems(self.libraryDict.keys())
-        formLayout.addRow(edf.boldLabel('Select Library', self), self.libNamesCB)
-        layout.addLayout(formLayout)
-        layout.addSpacing(40)
-        layout.addWidget(self.buttonBox)
-        self.setLayout(layout)
-
-
-class renameLibDialog(QDialog):
-    def __init__(self, parent, oldLibraryName, *args):
-        super().__init__(parent, *args)
-        self.oldLibraryName = oldLibraryName
-        self.setWindowTitle(f'Change {oldLibraryName} to:')
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        formBox = QGroupBox('Rename Library')
-        layout = QVBoxLayout()
-        formLayout = QFormLayout()
-        self.newLibraryName = edf.longLineEdit()
-        formLayout.addRow(edf.boldLabel('New Library Name:', self), self.newLibraryName)
-        formBox.setLayout(formLayout)
-        layout.addWidget(formBox)
-        layout.addSpacing(40)
-        layout.addWidget(self.buttonBox)
-        self.setLayout(layout)
-
-
-class renameViewDialog(QDialog):
-    def __init__(self, parent, oldViewName):
-        super().__init__(parent)
-        self.oldViewName = oldViewName
-        self.setWindowTitle(f'Rename {oldViewName} ')
-        self.layout = QVBoxLayout()
-        formLayout = QFormLayout()
-        oldViewNameEdit = edf.longLineEdit()
-        oldViewNameEdit.setText(self.oldViewName)
-        oldViewNameEdit.setEnabled(False)
-        formLayout.addRow(edf.boldLabel('Old View Name:'), oldViewNameEdit)
-        self.newViewNameEdit = edf.longLineEdit()
-        formLayout.addRow(edf.boldLabel('New View Name:'), self.newViewNameEdit)
-        self.layout.addLayout(formLayout)
-        self.layout.setSpacing(10)
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-
-        self.layout.addWidget(self.buttonBox)
-        self.setLayout(self.layout)
-
-
-class deleteSymbolDialog(QDialog):
-    def __init__(self, cellName, viewName, *args):
-        super().__init__(*args)
-        self.setWindowTitle(f'Delete {cellName}-{viewName} CellView?')
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-
-        self.layout = QVBoxLayout()
-        message = QLabel(f"{cellName}-{viewName} will be recreated!")
-        self.layout.addWidget(message)
-        self.layout.addWidget(self.buttonBox)
-        self.setLayout(self.layout)
-
-
-class netlistExportDialogue(QDialog):
-    def __init__(self, parent):
-        super().__init__(parent)
-        self.parent = parent
-        self.setWindowTitle(f'Export Netlist?')
-        self.setMinimumSize(500, 100)
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-
-        self.mainLayout = QVBoxLayout()
-        self.mainLayout.addStretch(2)
-        viewBox = QGroupBox('Select a view to Netlist')
-        viewBoxLayout = QFormLayout()
-        self.libNameEdit = edf.longLineEdit()
-        self.libNameEdit.setDisabled(True)
-        viewBoxLayout.addRow(edf.boldLabel('Library:'),self.libNameEdit)
-        self.cellNameEdit = edf.longLineEdit()
-        self.cellNameEdit.setDisabled(True)
-        viewBoxLayout.addRow(edf.boldLabel('Cell:'), self.cellNameEdit)
-        self.viewNameCombo = QComboBox()
-        viewBoxLayout.addRow(edf.boldLabel('View:'),self.viewNameCombo)
-        viewBox.setLayout(viewBoxLayout)
-        self.mainLayout.addWidget(viewBox)
-        switchBox = QGroupBox('Switch and Stop View Lists')
-        self.formLayout = QFormLayout()
-        self.switchViewEdit = edf.longLineEdit()
-        self.switchViewEdit.setText((', ').join(self.parent.switchViewList))
-        self.formLayout.addRow(edf.boldLabel('Switch View List:'), self.switchViewEdit)
-        self.stopViewEdit = edf.longLineEdit()
-        self.stopViewEdit.setText((', ').join(self.parent.stopViewList))
-        self.formLayout.addRow((edf.boldLabel('Stop View: ')), self.stopViewEdit)
-        switchBox.setLayout(self.formLayout)
-        self.mainLayout.addWidget(switchBox)
-        fileBox = QGroupBox('Select Simulation Directory')
-        fileDialogLayout = QHBoxLayout()
-        fileDialogLayout.addWidget(edf.boldLabel('Export Directory:'))
-        self.netlistDirEdit = edf.longLineEdit()
-        fileDialogLayout.addWidget(self.netlistDirEdit)
-        self.netListDirButton = QPushButton('...')
-        self.netListDirButton.clicked.connect(self.onDirButtonClicked)
-        fileDialogLayout.addWidget(self.netListDirButton)
-        fileBox.setLayout(fileDialogLayout)
-        self.mainLayout.addWidget(fileBox)
-        self.mainLayout.addStretch(2)
-        self.mainLayout.addWidget(self.buttonBox)
-        self.setLayout(self.mainLayout)
-
-    def onDirButtonClicked(self):
-        self.dirName = QFileDialog.getExistingDirectory()
-        if self.dirName:
-            self.netlistDirEdit.setText(self.dirName)
-
-
-class goDownHierDialogue(QDialog):
-    def __init__(self, parent,):
-        super().__init__(parent=parent)
-        self._parent = parent
-        self.setWindowTitle('Go Down Hierarchy')
-        self.setMinimumWidth(250)
-        self.buttonId = 1
-        _mainLayout = QVBoxLayout()
-        viewGroup = QGroupBox('Select a cellview')
-        viewGroupLayout = QVBoxLayout()
-        viewGroup.setLayout(viewGroupLayout)
-        self.viewListCB = QComboBox()
-        viewGroupLayout.addWidget(self.viewListCB)
-        _mainLayout.addWidget(viewGroup)
-        buttonGroupBox = QGroupBox('Open')
-        buttonGroupLayout = QHBoxLayout()
-        buttonGroupBox.setLayout(buttonGroupLayout)
-        self.openButton = QRadioButton('Edit')
-        self.openButton.setChecked(True)
-        self.readOnlyButton = QRadioButton('Read Only')
-        buttonGroupLayout.addWidget(self.openButton)
-        buttonGroupLayout.addWidget(self.readOnlyButton)
-        _mainLayout.addWidget(buttonGroupBox)
-        self.buttonGroup = QButtonGroup()
-        self.buttonGroup.addButton(self.openButton, id = 1)
-        self.buttonGroup.addButton(self.readOnlyButton, id = 2)
-        self.buttonGroup.buttonClicked.connect(self.onButtonClicked)
-        _mainLayout.addWidget(buttonGroupBox)
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        buttonBox = QDialogButtonBox(QBtn)
-        buttonBox.accepted.connect(self.accept)
-        buttonBox.rejected.connect(self.reject)
-        _mainLayout.addWidget(buttonBox)
-        self.setLayout(_mainLayout)
-        self.show()
-
-    def onButtonClicked(self):
-        self.buttonId = self.buttonGroup.checkedId()
-
-class importVerilogaCellDialogue(QDialog):
-    def __init__(self, model, parent):
-        super().__init__(parent)
-        self._parent = parent
-        self.setWindowTitle('Import a Verilog-a File')
-        self._model = model
-        self.setMinimumSize(500, 200)
-        mainLayout = QVBoxLayout()
-        fileDialogLayout = QHBoxLayout()
-        fileDialogLayout.addWidget(edf.boldLabel('Select Verilog-A file:'), 1)
-        self.vaFileEdit = edf.longLineEdit()
-        fileDialogLayout.addWidget(self.vaFileEdit, 4)
-        self.vaFileButton = QPushButton('...')
-        self.vaFileButton.clicked.connect(self.onFileButtonClicked)
-        fileDialogLayout.addWidget(self.vaFileButton, 1)
-        mainLayout.addLayout(fileDialogLayout)
-        mainLayout.addSpacing(20)
-        layout = QFormLayout()
-        layout.setSpacing(10)
-        self.libNamesCB = QComboBox()
-        self.libNamesCB.setModel(self._model)
-        self.libNamesCB.currentTextChanged.connect(self.changeCells)
-        layout.addRow(edf.boldLabel('Library:'), self.libNamesCB)
-        self.cellNamesCB = QComboBox()
-        self.cellNamesCB.setEditable(True)
-        initialCellNames = [self._model.item(0).child(i).cellName for i in
-                            range(self._model.item(0).rowCount())]
-        self.cellNamesCB.addItems(initialCellNames)
-        layout.addRow(edf.boldLabel('Cell:'), self.cellNamesCB)
-        self.vaViewName = edf.longLineEdit()
-        layout.addRow(edf.boldLabel('Verilog-A view:'), self.vaViewName)
-        mainLayout.addLayout(layout)
-        symbolGroupBox = QGroupBox('Symbol Creation')
-        symbolGBLayout = QVBoxLayout()
-        self.symbolCheckBox = QCheckBox('Create a new symbol?')
-        symbolGBLayout.addWidget(self.symbolCheckBox)
-        symbolGroupBox.setLayout(symbolGBLayout)
-        mainLayout.addWidget(symbolGroupBox)
-        mainLayout.addSpacing(20)
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        mainLayout.addWidget(self.buttonBox)
-        self.setLayout(mainLayout)
-        self.show()
-
-    def changeCells(self):
-        selectedLibItemRow = self._model.findItems(self.libNamesCB.currentText())[0].row()
-        libCellNames = [self._model.item(selectedLibItemRow).child(i).cellName for i in
-                        range(self._model.item(selectedLibItemRow).rowCount())]
-        self.cellNamesCB.clear()
-        self.cellNamesCB.addItems(libCellNames)
-
-    def onFileButtonClicked(self):
-        self.vaFileName = QFileDialog.getOpenFileName(self, caption='Select Verilog-A '
-                                                                    'file.')[0]
-        if self.vaFileName:
-            self.vaFileEdit.setText(self.vaFileName)
-
-
-class createConfigViewDialogue(QDialog):
-    def __init__(self, parent):
-        super().__init__(parent=parent)
-        self.parent = parent
-        self.mainLayout = QVBoxLayout()
-        self.setWindowTitle("Create New Config View")
-        self.setMinimumSize(360, 400)
-        topCellGroup = QGroupBox('Top Cell')
-        topCellLayout = QFormLayout()
-        self.libraryNameEdit = edf.longLineEdit()
-        topCellLayout.addRow(edf.boldLabel('Library:'), self.libraryNameEdit)
-        self.cellNameEdit = edf.longLineEdit()
-        topCellLayout.addRow(edf.boldLabel('Cell:'), self.cellNameEdit)
-        self.viewNameCB = QComboBox()
-        topCellLayout.addRow(edf.boldLabel('View:'), self.viewNameCB)
-        topCellGroup.setLayout(topCellLayout)
-        self.mainLayout.addWidget(topCellGroup)
-        viewGroup = QGroupBox('Switch/Stop Views')
-        viewGroupLayout = QFormLayout()
-        viewGroup.setLayout(viewGroupLayout)
-        self.switchViews = edf.longLineEdit()
-        viewGroupLayout.addRow(edf.boldLabel('View List:'), self.switchViews)
-        self.stopViews = edf.longLineEdit()
-        viewGroupLayout.addRow(edf.boldLabel('Stop List:'), self.stopViews)
-        self.mainLayout.addWidget(viewGroup)
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        self.mainLayout.addWidget(self.buttonBox)
-        self.setLayout(self.mainLayout)
-
-
-class appProperties(QDialog):
-    def __init__(self, parent):
-        self.parent = parent
-        super().__init__(parent)
-        self.setMinimumSize(550, 200)
-        self.setWindowTitle('Revolution EDA Options')
-        mainLayout = QVBoxLayout()
-        filePathsGroup = QGroupBox('Paths')
-        filePathsLayout = QVBoxLayout()
-        fileDialogLayout = QHBoxLayout()
-        fileDialogLayout.addWidget(edf.boldLabel('Text Editor Path:'), 2)
-        self.editorPathEdit = edf.longLineEdit()
-        fileDialogLayout.addWidget(self.editorPathEdit, 5)
-        self.editFileButton = QPushButton('...')
-        self.editFileButton.clicked.connect(self.onFileButtonClicked)
-        fileDialogLayout.addWidget(self.editFileButton, 1)
-        filePathsLayout.addLayout(fileDialogLayout)
-        simPathDialogLayout = QHBoxLayout()
-        simPathDialogLayout.addWidget(edf.boldLabel('Simulation Path:'),2)
-        self.simPathEdit = edf.longLineEdit()
-        simPathDialogLayout.addWidget(self.simPathEdit,5)
-        self.simPathButton = QPushButton('...')
-        self.simPathButton.clicked.connect(self.onSimPathButtonClicked)
-        simPathDialogLayout.addWidget(self.simPathButton,1)
-        filePathsLayout.addLayout(simPathDialogLayout)
-        filePathsGroup.setLayout(filePathsLayout)
-        mainLayout.addWidget(filePathsGroup)
-        switchViewsGroup = QGroupBox('Switch and Stop Views')
-        switchViewsLayout = QFormLayout()
-        self.switchViewsEdit = edf.longLineEdit()
-        switchViewsLayout.addRow(edf.boldLabel('Switch Views:'), self.switchViewsEdit)
-        self.stopViewsEdit = edf.longLineEdit()
-        switchViewsLayout.addRow(edf.boldLabel('Stop Views:'), self.stopViewsEdit)
-        switchViewsGroup.setLayout(switchViewsLayout)
-        mainLayout.addWidget(switchViewsGroup)
-        saveGroupBox = QGroupBox('Save Options')
-        saveGBLayout = QVBoxLayout()
-        self.optionSaveBox = QCheckBox('Save options to configuration file?')
-        saveGBLayout.addWidget(self.optionSaveBox)
-        saveGroupBox.setLayout(saveGBLayout)
-        mainLayout.addWidget(saveGroupBox)
-        mainLayout.addSpacing(20)
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        mainLayout.addWidget(self.buttonBox)
-        self.setLayout(mainLayout)
-
-    def onFileButtonClicked(self):
-       self.editorPathEdit.setText(QFileDialog.getOpenFileName(self, caption='Select text '
-                                                                    'editor path.')[0])
-
-    def onSimPathButtonClicked(self):
-        self.simPathEdit.setText(QFileDialog.getExistingDirectory(self, caption =
-        'Simulation path:'))
-
-class libraryPathsModel(QStandardItemModel):
-    def __init__(self, libraryDict):
-        super().__init__()
-        self.libraryDict = libraryDict
-        self.setHorizontalHeaderLabels(['Library Name', 'Library Path'])
-        for key, value in self.libraryDict.items():
-            libName = QStandardItem(key)
-            libPath = QStandardItem(str(value))
-            self.appendRow([libName, libPath])
-        self.appendRow([QStandardItem('Right click here...'), QStandardItem('')])
-
-
-class libraryPathsTableView(QTableView):
-    def __init__(self, model,logger):
-        super().__init__()
-        self.model = model
-        self.logger = logger
-        self.setModel(self.model)
-        self.setShowGrid(True)
-        self.setColumnWidth(0,200)
-        self.setColumnWidth(1,400)
-        self.fileDialog = QFileDialog()
-        self.fileDialog.setFileMode(QFileDialog.Directory)
-        self.libNameEditList = list()
-        self.libPathEditList = list()
-        for row in range(self.model.rowCount()):
-            self.libPathEditList.append(edf.longLineEdit())
-            self.setIndexWidget(self.model.index(row,1),self.libPathEditList[-1])
-            self.libPathEditList[-1].setText(self.model.item(row,1).text())
-
-
-    def contextMenuEvent(self, event) -> None:
-        self.menu = QMenu(self)
-        try:
-            selectedIndex = self.selectedIndexes()[0]
-        except IndexError:
-            self.model.appendRow([QStandardItem('Click here...'), QStandardItem('')])
-            selectedIndex = self.model.index(0,0)
-        removePathAction = self.menu.addAction('Remove Path')
-        removePathAction.triggered.connect(lambda : self.removeLibraryPath(selectedIndex))
-        addPathAction = self.menu.addAction('Add Library Path')
-        addPathAction.triggered.connect(lambda : self.addLibraryPath(selectedIndex))
-        self.menu.exec(event.globalPos())
-
-    def removeLibraryPath(self,index):
-        self.model.takeRow(index.row())
-        self.logger.info('Removed Library Path.')
-
-    def addLibraryPath(self,index):
-        row = index.row()
-        self.selectRow(row)
-        self.fileDialog.exec()
-        if self.fileDialog.selectedFiles():
-            self.selectedDirectory = QDir(self.fileDialog.selectedFiles()[0])
-        self.model.insertRow(row,[QStandardItem(self.selectedDirectory.dirName()),
-                                  QStandardItem(self.selectedDirectory.absolutePath())])
-
-
-class libraryPathEditorDialog(QDialog):
-    def __init__(self, parent, libraryDict: dict):
-        super().__init__(parent)
-        self.parent = parent
-        self.logger = self.parent.logger
-        self.libraryDict = libraryDict
-        self.setWindowTitle('Library Paths Dialogue')
-        self.setMinimumSize(700,300)
-        self.mainLayout = QVBoxLayout()
-        self.pathsBox = QGroupBox()
-        self.boxLayout = QVBoxLayout()
-        self.pathsBox.setLayout(self.boxLayout)
-        self.pathsModel = libraryPathsModel(self.libraryDict)
-        self.tableView = libraryPathsTableView(self.pathsModel,self.logger)
-        self.boxLayout.addWidget(self.tableView)
-        self.mainLayout.addWidget(self.pathsBox)
-        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        self.mainLayout.addWidget(self.buttonBox)
+#   “Commons Clause” License Condition v1.0
+#  #
+#   The Software is provided to you by the Licensor under the License, as defined
+#   below, subject to the following condition.
+#  #
+#   Without limiting other conditions in the License, the grant of rights under the
+#   License will not include, and the License does not grant to you, the right to
+#   Sell the Software.
+#  #
+#   For purposes of the foregoing, “Sell” means practicing any or all of the rights
+#   granted to you under the License to provide to third parties, for a fee or other
+#   consideration (including without limitation fees for hosting or consulting/
+#   support services related to the Software), a product or service whose value
+#   derives, entirely or substantially, from the functionality of the Software. Any
+#   license notice or attribution required by the License must also include this
+#   Commons Clause License Condition notice.
+#  #
+#   Software: Revolution EDA
+#   License: Mozilla Public License 2.0
+#   Licensor: Revolution Semiconductor (Registered in the Netherlands)
+
+import pathlib
+
+import revedaEditor.backend.libraryMethods as libm
+import revedaEditor.common.shape as shp
+import revedaEditor.gui.editFunctions as edf
+from PySide6.QtCore import (Qt, QDir)
+from PySide6.QtGui import (QStandardItemModel, QStandardItem)
+from PySide6.QtWidgets import (QComboBox, QDialog, QDialogButtonBox, QFileDialog,
+                               QFormLayout, QHBoxLayout, QLabel, QLineEdit,
+                               QVBoxLayout, QRadioButton, QButtonGroup,
+                               QPushButton, QGroupBox, QTableView, QMenu,
+                               QCheckBox)
+
+
+class createCellDialog(QDialog):
+    def __init__(self, parent, model):
+        super().__init__(parent=parent)
+        self.parent = parent
+        self.model = model
+        self.init_UI()
+
+    def init_UI(self):
+        self.setWindowTitle("Create Cell")
+        self.layout = QFormLayout()
+        self.layout.setSpacing(10)
+        self.libNamesCB = QComboBox()
+        self.libNamesCB.setModel(self.model)
+        self.libNamesCB.setModelColumn(0)
+        self.libNamesCB.setCurrentIndex(0)
+        self.libNamesCB.currentTextChanged.connect(self.selectLibrary)
+        self.layout.addRow(edf.boldLabel("Library:"), self.libNamesCB)
+        self.cellCB = QComboBox()
+        libItem = libm.getLibItem(self.model, self.libNamesCB.currentText())
+        self.cellList = [libItem.child(i).cellName for i in range(libItem.rowCount())]
+        self.cellCB.addItems(self.cellList)
+        self.cellCB.setEditable(True)
+        self.layout.addRow(edf.boldLabel("Cell Name:"), self.cellCB)
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        self.layout.addWidget(self.buttonBox)
+        self.setLayout(self.layout)
+
+    def selectLibrary(self):
+        libItem = libm.getLibItem(self.model, self.libNamesCB.currentText())
+        cellList = [libItem.child(i).cellName for i in range(libItem.rowCount())]
+        self.cellCB.clear()
+        self.cellCB.addItems(cellList)
+
+
+
+class deleteCellDialog(createCellDialog):
+    def __init__(self, parent, model):
+        super().__init__(parent, model)
+        self.cellCB.setEditable(False)
+        self.setWindowTitle('Delete Cell')
+
+
+class newCellViewDialog(createCellDialog):
+    def __init__(self, parent, model):
+        super().__init__(parent, model)
+        self.cellCB.setEditable(False)
+        self.setWindowTitle('Create Cell View')
+        self.viewType = QComboBox()
+        self.layout.addRow(edf.boldLabel("View Type:"), self.viewType)
+        self.viewName = edf.longLineEdit()
+        self.layout.addRow(edf.boldLabel('View Name:'), self.viewName)
+        self.layout.setSpacing(10)
+        self.layout.addWidget(self.buttonBox)
+        self.setLayout(self.layout)
+
+
+class selectCellViewDialog(deleteCellDialog):
+    def __init__(self, parent, model):
+        super().__init__(parent=parent, model=model)
+        libItem = libm.getLibItem(self.model, self.libNamesCB.currentText())
+        self.setWindowTitle("Select CellView")
+        self.cellCB.currentTextChanged.connect(self.cellNameChanged)
+        self.viewCB = QComboBox()
+        cellItem = libm.getCellItem(libItem, self.cellCB.currentText())
+        self.viewCB.addItems(
+            [cellItem.child(i).text() for i in range(cellItem.rowCount())])
+
+        self.layout.addRow(edf.boldLabel('View Name:'), self.viewCB)
+        self.layout.setSpacing(10)
+        self.layout.addWidget(self.buttonBox)
+        self.setLayout(self.layout)
+
+    def cellNameChanged(self):
+        libItem = libm.getLibItem(self.model, self.libNamesCB.currentText())
+        cellItem = libm.getCellItem(libItem, self.cellCB.currentText())
+        if cellItem is not None:
+            viewList = [cellItem.child(i).text() for i in range(cellItem.rowCount())]
+        else:
+            viewList = []
+        self.viewCB.clear()
+        self.viewCB.addItems(viewList)
+
+
+class createCellViewDialog(QDialog):
+    def __init__(self, parent, model, cellItem):
+        super().__init__(parent=parent)
+        self.parent = parent
+        self.model = model
+        self.cellItem = cellItem
+        self.cellPath = self.cellItem.data(Qt.UserRole + 2)
+        self.init_UI()
+
+    def init_UI(self):
+        self.setWindowTitle("Create CellView")
+        layout = QFormLayout()
+        layout.setSpacing(10)
+        self.viewComboBox = QComboBox()
+        self.viewComboBox.addItems(self.parent.cellViews)
+        layout.addRow("Select View:", self.viewComboBox)
+        self.nameEdit = QLineEdit()
+        self.nameEdit.setPlaceholderText("CellView Name")
+        self.nameEdit.setFixedWidth(200)
+        layout.addRow(QLabel("View Name:"), self.nameEdit)
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        layout.addRow(self.buttonBox)
+        self.setLayout(layout)
+
+
+class renameCellDialog(QDialog):
+    def __init__(self, parent, cellItem):
+        super().__init__(parent=parent)
+        self.parent = parent
+        self.cellItem = cellItem
+
+        self.init_UI()
+
+    def init_UI(self):
+        self.setWindowTitle("Rename Cell")
+        layout = QFormLayout()
+        layout.setSpacing(10)
+        self.nameEdit = QLineEdit()
+        self.nameEdit.setPlaceholderText("Cell Name")
+        self.nameEdit.setFixedWidth(200)
+        layout.addRow(QLabel("Cell Name:"), self.nameEdit)
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        layout.addRow(self.buttonBox)
+        self.setLayout(layout)
+
+
+class copyCellDialog(QDialog):
+    def __init__(self, parent, model, cellItem):
+        super().__init__(parent=parent)
+        self.parent = parent
+        self.model = model
+        self.cellItem = cellItem
+
+        # self.index = 0
+        self.init_UI()
+
+    def init_UI(self):
+        self.setWindowTitle("Copy Cell")
+        layout = QFormLayout()
+        layout.setSpacing(10)
+        self.libraryComboBox = QComboBox()
+        self.libraryComboBox.setModel(self.model)
+        self.libraryComboBox.setModelColumn(0)
+        self.libraryComboBox.setCurrentIndex(0)
+        self.selectedLibPath = self.libraryComboBox.itemData(0, Qt.UserRole + 2)
+        self.libraryComboBox.currentTextChanged.connect(self.selectLibrary)
+        layout.addRow(QLabel("Library:"), self.libraryComboBox)
+        self.copyName = QLineEdit()
+        self.copyName.setPlaceholderText("Enter Cell Name")
+        self.copyName.setFixedWidth(130)
+        layout.addRow(QLabel("Cell Name:"), self.copyName)
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        layout.addRow(self.buttonBox)
+        self.setLayout(layout)
+
+    def selectLibrary(self):
+        self.selectedLibPath = self.libraryComboBox.itemData(
+            self.libraryComboBox.currentIndex(), Qt.UserRole + 2)
+
+
+class copyViewDialog(createCellDialog):
+    def __init__(self, parent, model):
+        super().__init__(parent=parent, model=model)
+        self.setWindowTitle('Copy View')
+        self.cellCB.setEditable(True)
+        self.cellCB.InsertPolicy = QComboBox.InsertAfterCurrent
+        self.viewName = edf.longLineEdit()
+        self.layout.addRow(edf.boldLabel('View Name:'), self.viewName)
+        self.layout.setSpacing(10)
+        self.layout.addWidget(self.buttonBox)
+        self.setLayout(self.layout)
+
+
+class closeLibDialog(QDialog):
+    def __init__(self, libraryDict, parent, *args):
+        super().__init__(parent, *args)
+        self.libraryDict = libraryDict
+        self.setWindowTitle('Select Library to close')
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+
+        layout = QVBoxLayout()
+        formLayout = QFormLayout()
+        self.libNamesCB = QComboBox()
+        self.libNamesCB.addItems(self.libraryDict.keys())
+        formLayout.addRow(edf.boldLabel('Select Library', self), self.libNamesCB)
+        layout.addLayout(formLayout)
+        layout.addSpacing(40)
+        layout.addWidget(self.buttonBox)
+        self.setLayout(layout)
+
+
+class renameLibDialog(QDialog):
+    def __init__(self, parent, oldLibraryName, *args):
+        super().__init__(parent, *args)
+        self.oldLibraryName = oldLibraryName
+        self.setWindowTitle(f'Change {oldLibraryName} to:')
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        formBox = QGroupBox('Rename Library')
+        layout = QVBoxLayout()
+        formLayout = QFormLayout()
+        self.newLibraryName = edf.longLineEdit()
+        formLayout.addRow(edf.boldLabel('New Library Name:', self), self.newLibraryName)
+        formBox.setLayout(formLayout)
+        layout.addWidget(formBox)
+        layout.addSpacing(40)
+        layout.addWidget(self.buttonBox)
+        self.setLayout(layout)
+
+
+class renameViewDialog(QDialog):
+    def __init__(self, parent, oldViewName):
+        super().__init__(parent)
+        self.oldViewName = oldViewName
+        self.setWindowTitle(f'Rename {oldViewName} ')
+        self.layout = QVBoxLayout()
+        formLayout = QFormLayout()
+        oldViewNameEdit = edf.longLineEdit()
+        oldViewNameEdit.setText(self.oldViewName)
+        oldViewNameEdit.setEnabled(False)
+        formLayout.addRow(edf.boldLabel('Old View Name:'), oldViewNameEdit)
+        self.newViewNameEdit = edf.longLineEdit()
+        formLayout.addRow(edf.boldLabel('New View Name:'), self.newViewNameEdit)
+        self.layout.addLayout(formLayout)
+        self.layout.setSpacing(10)
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+
+        self.layout.addWidget(self.buttonBox)
+        self.setLayout(self.layout)
+
+
+class deleteSymbolDialog(QDialog):
+    def __init__(self, cellName, viewName, *args):
+        super().__init__(*args)
+        self.setWindowTitle(f'Delete {cellName}-{viewName} CellView?')
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+
+        self.layout = QVBoxLayout()
+        message = QLabel(f"{cellName}-{viewName} will be recreated!")
+        self.layout.addWidget(message)
+        self.layout.addWidget(self.buttonBox)
+        self.setLayout(self.layout)
+
+
+class netlistExportDialogue(QDialog):
+    def __init__(self, parent):
+        super().__init__(parent)
+        self.parent = parent
+        self.setWindowTitle(f'Export Netlist?')
+        self.setMinimumSize(500, 100)
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+
+        self.mainLayout = QVBoxLayout()
+        self.mainLayout.addStretch(2)
+        viewBox = QGroupBox('Select a view to Netlist')
+        viewBoxLayout = QFormLayout()
+        self.libNameEdit = edf.longLineEdit()
+        self.libNameEdit.setDisabled(True)
+        viewBoxLayout.addRow(edf.boldLabel('Library:'),self.libNameEdit)
+        self.cellNameEdit = edf.longLineEdit()
+        self.cellNameEdit.setDisabled(True)
+        viewBoxLayout.addRow(edf.boldLabel('Cell:'), self.cellNameEdit)
+        self.viewNameCombo = QComboBox()
+        viewBoxLayout.addRow(edf.boldLabel('View:'),self.viewNameCombo)
+        viewBox.setLayout(viewBoxLayout)
+        self.mainLayout.addWidget(viewBox)
+        switchBox = QGroupBox('Switch and Stop View Lists')
+        self.formLayout = QFormLayout()
+        self.switchViewEdit = edf.longLineEdit()
+        self.switchViewEdit.setText((', ').join(self.parent.switchViewList))
+        self.formLayout.addRow(edf.boldLabel('Switch View List:'), self.switchViewEdit)
+        self.stopViewEdit = edf.longLineEdit()
+        self.stopViewEdit.setText((', ').join(self.parent.stopViewList))
+        self.formLayout.addRow((edf.boldLabel('Stop View: ')), self.stopViewEdit)
+        switchBox.setLayout(self.formLayout)
+        self.mainLayout.addWidget(switchBox)
+        fileBox = QGroupBox('Select Simulation Directory')
+        fileDialogLayout = QHBoxLayout()
+        fileDialogLayout.addWidget(edf.boldLabel('Export Directory:'))
+        self.netlistDirEdit = edf.longLineEdit()
+        fileDialogLayout.addWidget(self.netlistDirEdit)
+        self.netListDirButton = QPushButton('...')
+        self.netListDirButton.clicked.connect(self.onDirButtonClicked)
+        fileDialogLayout.addWidget(self.netListDirButton)
+        fileBox.setLayout(fileDialogLayout)
+        self.mainLayout.addWidget(fileBox)
+        self.mainLayout.addStretch(2)
+        self.mainLayout.addWidget(self.buttonBox)
+        self.setLayout(self.mainLayout)
+
+    def onDirButtonClicked(self):
+        self.dirName = QFileDialog.getExistingDirectory()
+        if self.dirName:
+            self.netlistDirEdit.setText(self.dirName)
+
+
+class goDownHierDialogue(QDialog):
+    def __init__(self, parent,):
+        super().__init__(parent=parent)
+        self._parent = parent
+        self.setWindowTitle('Go Down Hierarchy')
+        self.setMinimumWidth(250)
+        self.buttonId = 1
+        _mainLayout = QVBoxLayout()
+        viewGroup = QGroupBox('Select a cellview')
+        viewGroupLayout = QVBoxLayout()
+        viewGroup.setLayout(viewGroupLayout)
+        self.viewListCB = QComboBox()
+        viewGroupLayout.addWidget(self.viewListCB)
+        _mainLayout.addWidget(viewGroup)
+        buttonGroupBox = QGroupBox('Open')
+        buttonGroupLayout = QHBoxLayout()
+        buttonGroupBox.setLayout(buttonGroupLayout)
+        self.openButton = QRadioButton('Edit')
+        self.openButton.setChecked(True)
+        self.readOnlyButton = QRadioButton('Read Only')
+        buttonGroupLayout.addWidget(self.openButton)
+        buttonGroupLayout.addWidget(self.readOnlyButton)
+        _mainLayout.addWidget(buttonGroupBox)
+        self.buttonGroup = QButtonGroup()
+        self.buttonGroup.addButton(self.openButton, id = 1)
+        self.buttonGroup.addButton(self.readOnlyButton, id = 2)
+        self.buttonGroup.buttonClicked.connect(self.onButtonClicked)
+        _mainLayout.addWidget(buttonGroupBox)
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        buttonBox = QDialogButtonBox(QBtn)
+        buttonBox.accepted.connect(self.accept)
+        buttonBox.rejected.connect(self.reject)
+        _mainLayout.addWidget(buttonBox)
+        self.setLayout(_mainLayout)
+        self.show()
+
+    def onButtonClicked(self):
+        self.buttonId = self.buttonGroup.checkedId()
+
+class importVerilogaCellDialogue(QDialog):
+    def __init__(self, model, parent):
+        super().__init__(parent)
+        self._parent = parent
+        self.setWindowTitle('Import a Verilog-a File')
+        self._model = model
+        self.setMinimumSize(500, 200)
+        mainLayout = QVBoxLayout()
+        fileDialogLayout = QHBoxLayout()
+        fileDialogLayout.addWidget(edf.boldLabel('Select Verilog-A file:'), 1)
+        self.vaFileEdit = edf.longLineEdit()
+        fileDialogLayout.addWidget(self.vaFileEdit, 4)
+        self.vaFileButton = QPushButton('...')
+        self.vaFileButton.clicked.connect(self.onFileButtonClicked)
+        fileDialogLayout.addWidget(self.vaFileButton, 1)
+        mainLayout.addLayout(fileDialogLayout)
+        mainLayout.addSpacing(20)
+        layout = QFormLayout()
+        layout.setSpacing(10)
+        self.libNamesCB = QComboBox()
+        self.libNamesCB.setModel(self._model)
+        self.libNamesCB.currentTextChanged.connect(self.changeCells)
+        layout.addRow(edf.boldLabel('Library:'), self.libNamesCB)
+        self.cellNamesCB = QComboBox()
+        self.cellNamesCB.setEditable(True)
+        initialCellNames = [self._model.item(0).child(i).cellName for i in
+                            range(self._model.item(0).rowCount())]
+        self.cellNamesCB.addItems(initialCellNames)
+        layout.addRow(edf.boldLabel('Cell:'), self.cellNamesCB)
+        self.vaViewName = edf.longLineEdit()
+        layout.addRow(edf.boldLabel('Verilog-A view:'), self.vaViewName)
+        mainLayout.addLayout(layout)
+        symbolGroupBox = QGroupBox('Symbol Creation')
+        symbolGBLayout = QVBoxLayout()
+        self.symbolCheckBox = QCheckBox('Create a new symbol?')
+        symbolGBLayout.addWidget(self.symbolCheckBox)
+        symbolGroupBox.setLayout(symbolGBLayout)
+        mainLayout.addWidget(symbolGroupBox)
+        mainLayout.addSpacing(20)
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        mainLayout.addWidget(self.buttonBox)
+        self.setLayout(mainLayout)
+        self.show()
+
+    def changeCells(self):
+        selectedLibItemRow = self._model.findItems(self.libNamesCB.currentText())[0].row()
+        libCellNames = [self._model.item(selectedLibItemRow).child(i).cellName for i in
+                        range(self._model.item(selectedLibItemRow).rowCount())]
+        self.cellNamesCB.clear()
+        self.cellNamesCB.addItems(libCellNames)
+
+    def onFileButtonClicked(self):
+        self.vaFileName = QFileDialog.getOpenFileName(self, caption='Select Verilog-A '
+                                                                    'file.')[0]
+        if self.vaFileName:
+            self.vaFileEdit.setText(self.vaFileName)
+
+
+class createConfigViewDialogue(QDialog):
+    def __init__(self, parent):
+        super().__init__(parent=parent)
+        self.parent = parent
+        self.mainLayout = QVBoxLayout()
+        self.setWindowTitle("Create New Config View")
+        self.setMinimumSize(360, 400)
+        topCellGroup = QGroupBox('Top Cell')
+        topCellLayout = QFormLayout()
+        self.libraryNameEdit = edf.longLineEdit()
+        topCellLayout.addRow(edf.boldLabel('Library:'), self.libraryNameEdit)
+        self.cellNameEdit = edf.longLineEdit()
+        topCellLayout.addRow(edf.boldLabel('Cell:'), self.cellNameEdit)
+        self.viewNameCB = QComboBox()
+        topCellLayout.addRow(edf.boldLabel('View:'), self.viewNameCB)
+        topCellGroup.setLayout(topCellLayout)
+        self.mainLayout.addWidget(topCellGroup)
+        viewGroup = QGroupBox('Switch/Stop Views')
+        viewGroupLayout = QFormLayout()
+        viewGroup.setLayout(viewGroupLayout)
+        self.switchViews = edf.longLineEdit()
+        viewGroupLayout.addRow(edf.boldLabel('View List:'), self.switchViews)
+        self.stopViews = edf.longLineEdit()
+        viewGroupLayout.addRow(edf.boldLabel('Stop List:'), self.stopViews)
+        self.mainLayout.addWidget(viewGroup)
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        self.mainLayout.addWidget(self.buttonBox)
+        self.setLayout(self.mainLayout)
+
+
+class appProperties(QDialog):
+    def __init__(self, parent):
+        self.parent = parent
+        super().__init__(parent)
+        self.setMinimumSize(550, 200)
+        self.setWindowTitle('Revolution EDA Options')
+        mainLayout = QVBoxLayout()
+        filePathsGroup = QGroupBox('Paths')
+        filePathsLayout = QVBoxLayout()
+        fileDialogLayout = QHBoxLayout()
+        fileDialogLayout.addWidget(edf.boldLabel('Text Editor Path:'), 2)
+        self.editorPathEdit = edf.longLineEdit()
+        fileDialogLayout.addWidget(self.editorPathEdit, 5)
+        self.editFileButton = QPushButton('...')
+        self.editFileButton.clicked.connect(self.onFileButtonClicked)
+        fileDialogLayout.addWidget(self.editFileButton, 1)
+        filePathsLayout.addLayout(fileDialogLayout)
+        simPathDialogLayout = QHBoxLayout()
+        simPathDialogLayout.addWidget(edf.boldLabel('Simulation Path:'),2)
+        self.simPathEdit = edf.longLineEdit()
+        simPathDialogLayout.addWidget(self.simPathEdit,5)
+        self.simPathButton = QPushButton('...')
+        self.simPathButton.clicked.connect(self.onSimPathButtonClicked)
+        simPathDialogLayout.addWidget(self.simPathButton,1)
+        filePathsLayout.addLayout(simPathDialogLayout)
+        filePathsGroup.setLayout(filePathsLayout)
+        mainLayout.addWidget(filePathsGroup)
+        switchViewsGroup = QGroupBox('Switch and Stop Views')
+        switchViewsLayout = QFormLayout()
+        self.switchViewsEdit = edf.longLineEdit()
+        switchViewsLayout.addRow(edf.boldLabel('Switch Views:'), self.switchViewsEdit)
+        self.stopViewsEdit = edf.longLineEdit()
+        switchViewsLayout.addRow(edf.boldLabel('Stop Views:'), self.stopViewsEdit)
+        switchViewsGroup.setLayout(switchViewsLayout)
+        mainLayout.addWidget(switchViewsGroup)
+        saveGroupBox = QGroupBox('Save Options')
+        saveGBLayout = QVBoxLayout()
+        self.optionSaveBox = QCheckBox('Save options to configuration file?')
+        saveGBLayout.addWidget(self.optionSaveBox)
+        saveGroupBox.setLayout(saveGBLayout)
+        mainLayout.addWidget(saveGroupBox)
+        mainLayout.addSpacing(20)
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        mainLayout.addWidget(self.buttonBox)
+        self.setLayout(mainLayout)
+
+    def onFileButtonClicked(self):
+       self.editorPathEdit.setText(QFileDialog.getOpenFileName(self, caption='Select text '
+                                                                    'editor path.')[0])
+
+    def onSimPathButtonClicked(self):
+        self.simPathEdit.setText(QFileDialog.getExistingDirectory(self, caption =
+        'Simulation path:'))
+
+class libraryPathsModel(QStandardItemModel):
+    def __init__(self, libraryDict):
+        super().__init__()
+        self.libraryDict = libraryDict
+        self.setHorizontalHeaderLabels(['Library Name', 'Library Path'])
+        for key, value in self.libraryDict.items():
+            libName = QStandardItem(key)
+            libPath = QStandardItem(str(value))
+            self.appendRow([libName, libPath])
+        self.appendRow([QStandardItem('Right click here...'), QStandardItem('')])
+
+
+class libraryPathsTableView(QTableView):
+    def __init__(self, model,logger):
+        super().__init__()
+        self.model = model
+        self.logger = logger
+        self.setModel(self.model)
+        self.setShowGrid(True)
+        self.setColumnWidth(0,200)
+        self.setColumnWidth(1,400)
+        self.fileDialog = QFileDialog()
+        self.fileDialog.setFileMode(QFileDialog.Directory)
+        self.libNameEditList = list()
+        self.libPathEditList = list()
+        for row in range(self.model.rowCount()):
+            self.libPathEditList.append(edf.longLineEdit())
+            self.setIndexWidget(self.model.index(row,1),self.libPathEditList[-1])
+            self.libPathEditList[-1].setText(self.model.item(row,1).text())
+
+
+    def contextMenuEvent(self, event) -> None:
+        self.menu = QMenu(self)
+        try:
+            selectedIndex = self.selectedIndexes()[0]
+        except IndexError:
+            self.model.appendRow([QStandardItem('Click here...'), QStandardItem('')])
+            selectedIndex = self.model.index(0,0)
+        removePathAction = self.menu.addAction('Remove Path')
+        removePathAction.triggered.connect(lambda : self.removeLibraryPath(selectedIndex))
+        addPathAction = self.menu.addAction('Add Library Path')
+        addPathAction.triggered.connect(lambda : self.addLibraryPath(selectedIndex))
+        self.menu.exec(event.globalPos())
+
+    def removeLibraryPath(self,index):
+        self.model.takeRow(index.row())
+        self.logger.info('Removed Library Path.')
+
+    def addLibraryPath(self,index):
+        row = index.row()
+        self.selectRow(row)
+        self.fileDialog.exec()
+        if self.fileDialog.selectedFiles():
+            self.selectedDirectory = QDir(self.fileDialog.selectedFiles()[0])
+        self.model.insertRow(row,[QStandardItem(self.selectedDirectory.dirName()),
+                                  QStandardItem(self.selectedDirectory.absolutePath())])
+
+
+class libraryPathEditorDialog(QDialog):
+    def __init__(self, parent, libraryDict: dict):
+        super().__init__(parent)
+        self.parent = parent
+        self.logger = self.parent.logger
+        self.libraryDict = libraryDict
+        self.setWindowTitle('Library Paths Dialogue')
+        self.setMinimumSize(700,300)
+        self.mainLayout = QVBoxLayout()
+        self.pathsBox = QGroupBox()
+        self.boxLayout = QVBoxLayout()
+        self.pathsBox.setLayout(self.boxLayout)
+        self.pathsModel = libraryPathsModel(self.libraryDict)
+        self.tableView = libraryPathsTableView(self.pathsModel,self.logger)
+        self.boxLayout.addWidget(self.tableView)
+        self.mainLayout.addWidget(self.pathsBox)
+        QBtn = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        self.mainLayout.addWidget(self.buttonBox)
         self.setLayout(self.mainLayout)
```

### Comparing `revolution-eda-0.5.1/revedaEditor/gui/propertyDialogues.py` & `revolution-eda-0.5.2/revedaEditor/gui/propertyDialogues.py`

 * *Files 0% similar despite different names*

```diff
@@ -568,17 +568,24 @@
         self.setWindowTitle("Create Schematic Pin")
 
 
 class schematicPinPropertiesDialog(createPinDialog):
     def __init__(self, parent, item):
         super().__init__(parent)
         self.setWindowTitle(f"{item.pinName} - Pin Properties")
-        self.pinName.setText(item.pinName)
-        self.pinDir.setCurrentText(item.pinDir)
-        self.pinType.setCurrentText(item.pinType)
+        self.xlocationEdit = edf.shortLineEdit()
+        self.xlocationEdit.setToolTip("x location of pin")
+        self.fLayout.addRow("x location:", self.xlocationEdit)
+        self.ylocationEdit = edf.shortLineEdit()
+        self.ylocationEdit.setToolTip("y location of pin")
+        self.fLayout.addRow("y location:", self.ylocationEdit)
+        self.angleEdit = edf.shortLineEdit()
+        self.angleEdit.setToolTip("angle of pin")
+        self.fLayout.addRow("angle:", self.angleEdit)
+
 
 class symbolNameDialog(QDialog):
     def __init__(self, cellPath:pathlib.Path, cellName: str, parent):
         super().__init__(parent)
         self.cellPath = cellPath
         self.cellName = cellName
         self.symbolViewNames = [view.stem for view in cellPath.iterdir() if 'symbol' in
```

### Comparing `revolution-eda-0.5.1/revedaEditor/gui/pythonConsole.py` & `revolution-eda-0.5.2/revedaEditor/gui/pythonConsole.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-""" Console
-Interactive console widget.  Use to add an interactive python interpreter
-in a GUI application.
-"""
-
-import code
-import re
-from typing import Callable
-
-from PySide6.QtCore import (Qt, Signal, QEvent, QSize, )
-from PySide6.QtGui import (QTextCharFormat, QBrush, QColor, QFont)
-from PySide6.QtWidgets import (QLineEdit, QWidget, QGridLayout, QPlainTextEdit)
-
-
-class LineEdit(QLineEdit):
-    """QLIneEdit with a history buffer for recalling previous lines.
-    I also accept tab as input (4 spaces).
-    """
-    newline = Signal(str)  # Signal when return key pressed
-
-    def __init__(self, history: int = 100) -> 'LineEdit':
-        super().__init__()
-        self.historymax = history
-        self.clearhistory()
-        self.promptpattern = re.compile('^[>\.]')
-
-    def clearhistory(self) -> None:
-        """Clear history buffer"""
-        self.historyindex = 0
-        self.historylist = []
-
-    def event(self, ev: QEvent) -> bool:
-        """Intercept tab and arrow key presses.  Insert 4 spaces
-        when tab pressed instead of moving to next contorl.  WHen
-        arrow up or down are pressed select a line from the history
-        buffer.  Emit newline signal when return key is pressed.
-        """
-        if ev.type() == QEvent.KeyPress:
-            if ev.key() == int(Qt.Key_Tab):
-                self.insert('    ')
-                return True
-            elif ev.key() == int(Qt.Key_Up):
-                self.recall(self.historyindex - 1)
-                return True
-            elif ev.key() == int(Qt.Key_Down):
-                self.recall(self.historyindex + 1)
-                return True
-            elif ev.key() == int(Qt.Key_Home):
-                self.recall(0)
-                return True
-            elif ev.key() == int(Qt.Key_End):
-                self.recall(len(self.historylist) - 1)
-                return True
-            elif ev.key() == int(Qt.Key_Return):
-                self.returnkey()
-                return True
-        return super().event(ev)
-
-    def returnkey(self) -> None:
-        """Return key was pressed.  Add line to history and emit
-        the newline signal.
-        """
-        text = self.text().rstrip()
-        self.record(text)
-        self.newline.emit(text)
-        self.setText('')
-
-    def recall(self, index: int) -> None:
-        """Select a line from the history list"""
-        length = len(self.historylist)
-        if (length > 0):
-            index = max(0, min(index, length - 1))
-            self.setText(self.historylist[index])
-            self.historyindex = index
-
-    def record(self, line: str) -> None:
-        """Add line to history buffer"""
-        self.historyindex += 1
-        while len(self.historylist) >= self.historymax - 1:
-            self.historylist.pop()
-        self.historylist.append(line)
-        self.historyindex = min(self.historyindex, len(self.historylist))
-
-
-class Redirect():
-    """Map self.write to a function"""
-
-    def __init__(self, func: Callable) -> 'Redirect':
-        self.func = func
-
-    def write(self, line: str) -> None:
-        self.func(line)
-
-
-class pythonConsole(QWidget):
-    """A GUI version of code.InteractiveConsole."""
-
-    def __init__(self, context=locals(),  # context for interpreter
-            history: int = 200,  # max lines in history buffer
-            blockcount: int = 500  # max lines in output buffer
-    ) -> 'pythonConsole':
-        super().__init__()
-        self.setcontext(context)
-        self.buffer = []
-
-        self.content = QGridLayout(self)
-        self.content.setContentsMargins(0, 0, 0, 0)
-        self.content.setSpacing(0)
-
-        # Display for output and stderr
-        self.outdisplay = QPlainTextEdit(self)
-        self.outdisplay.setMaximumBlockCount(blockcount)
-        self.outdisplay.setReadOnly(True)
-        self.content.addWidget(self.outdisplay, 0, 0, 1, 2)
-
-        # Use color to differentiate input, output and stderr
-        self.inpfmt = self.outdisplay.currentCharFormat()
-        self.outfmt = QTextCharFormat(self.inpfmt)
-        self.outfmt.setForeground(QBrush(QColor(0, 0, 255)))
-        self.errfmt = QTextCharFormat(self.inpfmt)
-        self.errfmt.setForeground(QBrush(QColor(255, 0, 0)))
-
-        # Display input prompt left of input edit
-        self.promptdisp = QLineEdit(self)
-        self.promptdisp.setReadOnly(True)
-        self.promptdisp.setFixedWidth(15)
-        self.promptdisp.setFrame(False)
-        self.content.addWidget(self.promptdisp, 1, 0)
-        self.setprompt('> ')
-
-        # Enter commands here
-        self.inpedit = LineEdit(history=history)
-        self.inpedit.newline.connect(self.push)
-        self.inpedit.setFrame(False)
-        self.content.addWidget(self.inpedit, 1, 1)
-
-    def setcontext(self, context):
-        """Set context for interpreter"""
-        self.interp = code.InteractiveInterpreter(context)
-
-    def resetbuffer(self) -> None:
-        """Reset the input buffer."""
-        self.buffer = []
-
-    def setprompt(self, text: str):
-        self.prompt = text
-        self.promptdisp.setText(text)
-
-    def push(self, line: str) -> None:
-        """Execute entered command.  Command may span multiple lines"""
-        if line == 'clear':
-            self.inpedit.clearhistory()
-            self.outdisplay.clear()
-        else:
-            lines = line.split('\n')
-            for line in lines:
-                if re.match('^[\>\.] ', line):
-                    line = line[2:]
-                self.writeoutput(self.prompt + line, self.inpfmt)
-                self.setprompt('. ')
-                self.buffer.append(line)
-            # Built a command string from lines in the buffer
-            source = "\n".join(self.buffer)
-            more = self.interp.runsource(source, '<input>', 'exec')
-            if not more:
-                self.setprompt('> ')
-                self.resetbuffer()
-
-    def setfont(self, font: QFont) -> None:
-        """Set font for input and display widgets.  Should be monospaced"""
-        self.outdisplay.setFont(font)
-        self.inpedit.setFont(font)
-
-    def write(self, line: str) -> None:
-        """Capture stdout and display in outdisplay"""
-        if (len(line) != 1 or ord(line[0]) != 10):
-            self.writeoutput(line.rstrip(), self.outfmt)
-
-    def errorwrite(self, line: str) -> None:
-        """Capture stderr and display in outdisplay"""
-        self.writeoutput(line, self.errfmt)
-
-    def writeoutput(self, line: str, fmt: QTextCharFormat = None) -> None:
-        """Set text formatting and display line in outdisplay"""
-        if fmt is not None:
-            self.outdisplay.setCurrentCharFormat(fmt)
-        self.outdisplay.appendPlainText(line.rstrip())
-
-    def sizeHint(self):
-        return QSize(500, 200)
-
-
-
+""" Console
+Interactive console widget.  Use to add an interactive python interpreter
+in a GUI application.
+"""
+
+import code
+import re
+from typing import Callable
+
+from PySide6.QtCore import (Qt, Signal, QEvent, QSize, )
+from PySide6.QtGui import (QTextCharFormat, QBrush, QColor, QFont)
+from PySide6.QtWidgets import (QLineEdit, QWidget, QGridLayout, QPlainTextEdit)
+
+
+class LineEdit(QLineEdit):
+    """QLIneEdit with a history buffer for recalling previous lines.
+    I also accept tab as input (4 spaces).
+    """
+    newline = Signal(str)  # Signal when return key pressed
+
+    def __init__(self, history: int = 100) -> 'LineEdit':
+        super().__init__()
+        self.historymax = history
+        self.clearhistory()
+        self.promptpattern = re.compile('^[>\.]')
+
+    def clearhistory(self) -> None:
+        """Clear history buffer"""
+        self.historyindex = 0
+        self.historylist = []
+
+    def event(self, ev: QEvent) -> bool:
+        """Intercept tab and arrow key presses.  Insert 4 spaces
+        when tab pressed instead of moving to next contorl.  WHen
+        arrow up or down are pressed select a line from the history
+        buffer.  Emit newline signal when return key is pressed.
+        """
+        if ev.type() == QEvent.KeyPress:
+            if ev.key() == int(Qt.Key_Tab):
+                self.insert('    ')
+                return True
+            elif ev.key() == int(Qt.Key_Up):
+                self.recall(self.historyindex - 1)
+                return True
+            elif ev.key() == int(Qt.Key_Down):
+                self.recall(self.historyindex + 1)
+                return True
+            elif ev.key() == int(Qt.Key_Home):
+                self.recall(0)
+                return True
+            elif ev.key() == int(Qt.Key_End):
+                self.recall(len(self.historylist) - 1)
+                return True
+            elif ev.key() == int(Qt.Key_Return):
+                self.returnkey()
+                return True
+        return super().event(ev)
+
+    def returnkey(self) -> None:
+        """Return key was pressed.  Add line to history and emit
+        the newline signal.
+        """
+        text = self.text().rstrip()
+        self.record(text)
+        self.newline.emit(text)
+        self.setText('')
+
+    def recall(self, index: int) -> None:
+        """Select a line from the history list"""
+        length = len(self.historylist)
+        if (length > 0):
+            index = max(0, min(index, length - 1))
+            self.setText(self.historylist[index])
+            self.historyindex = index
+
+    def record(self, line: str) -> None:
+        """Add line to history buffer"""
+        self.historyindex += 1
+        while len(self.historylist) >= self.historymax - 1:
+            self.historylist.pop()
+        self.historylist.append(line)
+        self.historyindex = min(self.historyindex, len(self.historylist))
+
+
+class Redirect():
+    """Map self.write to a function"""
+
+    def __init__(self, func: Callable) -> 'Redirect':
+        self.func = func
+
+    def write(self, line: str) -> None:
+        self.func(line)
+
+
+class pythonConsole(QWidget):
+    """A GUI version of code.InteractiveConsole."""
+
+    def __init__(self, context=locals(),  # context for interpreter
+            history: int = 200,  # max lines in history buffer
+            blockcount: int = 500  # max lines in output buffer
+    ) -> 'pythonConsole':
+        super().__init__()
+        self.setcontext(context)
+        self.buffer = []
+
+        self.content = QGridLayout(self)
+        self.content.setContentsMargins(0, 0, 0, 0)
+        self.content.setSpacing(0)
+
+        # Display for output and stderr
+        self.outdisplay = QPlainTextEdit(self)
+        self.outdisplay.setMaximumBlockCount(blockcount)
+        self.outdisplay.setReadOnly(True)
+        self.content.addWidget(self.outdisplay, 0, 0, 1, 2)
+
+        # Use color to differentiate input, output and stderr
+        self.inpfmt = self.outdisplay.currentCharFormat()
+        self.outfmt = QTextCharFormat(self.inpfmt)
+        self.outfmt.setForeground(QBrush(QColor(0, 0, 255)))
+        self.errfmt = QTextCharFormat(self.inpfmt)
+        self.errfmt.setForeground(QBrush(QColor(255, 0, 0)))
+
+        # Display input prompt left of input edit
+        self.promptdisp = QLineEdit(self)
+        self.promptdisp.setReadOnly(True)
+        self.promptdisp.setFixedWidth(15)
+        self.promptdisp.setFrame(False)
+        self.content.addWidget(self.promptdisp, 1, 0)
+        self.setprompt('> ')
+
+        # Enter commands here
+        self.inpedit = LineEdit(history=history)
+        self.inpedit.newline.connect(self.push)
+        self.inpedit.setFrame(False)
+        self.content.addWidget(self.inpedit, 1, 1)
+
+    def setcontext(self, context):
+        """Set context for interpreter"""
+        self.interp = code.InteractiveInterpreter(context)
+
+    def resetbuffer(self) -> None:
+        """Reset the input buffer."""
+        self.buffer = []
+
+    def setprompt(self, text: str):
+        self.prompt = text
+        self.promptdisp.setText(text)
+
+    def push(self, line: str) -> None:
+        """Execute entered command.  Command may span multiple lines"""
+        if line == 'clear':
+            self.inpedit.clearhistory()
+            self.outdisplay.clear()
+        else:
+            lines = line.split('\n')
+            for line in lines:
+                if re.match('^[\>\.] ', line):
+                    line = line[2:]
+                self.writeoutput(self.prompt + line, self.inpfmt)
+                self.setprompt('. ')
+                self.buffer.append(line)
+            # Built a command string from lines in the buffer
+            source = "\n".join(self.buffer)
+            more = self.interp.runsource(source, '<input>', 'exec')
+            if not more:
+                self.setprompt('> ')
+                self.resetbuffer()
+
+    def setfont(self, font: QFont) -> None:
+        """Set font for input and display widgets.  Should be monospaced"""
+        self.outdisplay.setFont(font)
+        self.inpedit.setFont(font)
+
+    def write(self, line: str) -> None:
+        """Capture stdout and display in outdisplay"""
+        if (len(line) != 1 or ord(line[0]) != 10):
+            self.writeoutput(line.rstrip(), self.outfmt)
+
+    def errorwrite(self, line: str) -> None:
+        """Capture stderr and display in outdisplay"""
+        self.writeoutput(line, self.errfmt)
+
+    def writeoutput(self, line: str, fmt: QTextCharFormat = None) -> None:
+        """Set text formatting and display line in outdisplay"""
+        if fmt is not None:
+            self.outdisplay.setCurrentCharFormat(fmt)
+        self.outdisplay.appendPlainText(line.rstrip())
+
+    def sizeHint(self):
+        return QSize(500, 200)
+
+
+
```

### Comparing `revolution-eda-0.5.1/revedaEditor/gui/revedaMain.py` & `revolution-eda-0.5.2/revedaEditor/gui/revedaMain.py`

 * *Files identical despite different names*

### Comparing `revolution-eda-0.5.1/revedaEditor/resources/resources.py` & `revolution-eda-0.5.2/revedaEditor/resources/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1314,52 +1314,14 @@
 \x1f\xe1\xc8\xd1\xc6\xc6\x0e\xe5*I\x98\x1cz\xa2Tn\
 N\xf5\xbdjQ\x8bsc\xca\xb4,\xf5WJ\xc5\xbd\
 \xcca.\x1ft\x88\x10\xf4\x19\xc6\x0d\xe1\xf3\x1dv\xa7\
 \x9eO$\x1e\xdei\xdd?\xf7-\x1b\x98^\xda\xf0/\
 ;\xefe\xa1\xb0ZH&G\xe9\xf1\xe7?\x01\x06\x00\
 \xa6\xe8M\xd6m\xca\x89\x98\x00\x00\x00\x00IEND\
 \xaeB`\x82\
-\x00\x00\x023\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
-\x00\x00\x00\x19tEXtSoftware\
-\x00Adobe ImageRead\
-yq\xc9e<\x00\x00\x01\xd5IDATx\xda\x9c\
-\x93\xcbN\xdbP\x10\x86\x7f\x1b\x07\xc7\xa1E\xed\x12P\
-@N\x94\x8b\x12TQ\xaa\xaaR\xb7\xa1\xec\xba+\xef\
-@\xf7\xac\x13)O\xd1\x15O\xc0\x1b\xb0\xab*\x10 \
-\xee\x09\x8a\x88\x92\x88\xa6QV\xa8\x8bV!\x01\x1f\xbb\
-3\x93\xd8\xb9\xacJ\x8e4\xf2?\xb6\xff\x99o\x8e\x8f\
-\xb5\xadB\xe13\x80\x05L\xb7\xda\x86\xeb\xba\x8b{\xc5\
-\xe2\xb7i\xdc_\xf2\xf9m\xc3UJ\xf3(\xd9<\x05\
-<\xcf\x0b\x82\x0aKx|\x1d\xcd\x07\xcf\x8fs\xaf\xc0\
-^])\xa5\xf3\x0b\xbc>\xc55\xb9n\xc4\x86:G\
-:g{\xc1}_\xb3\x87\xbd\x86r\x1cMI\x01\x0d\
-\xfb5\x0f1\xa3K\x93u\xa4\xf3\x86E\x1d\xdb.4\
-z\xce\xda\x0d4\x99\xbdy\xb0\xd7p\x1cg\x8c\xc0\xfd\
-\xf5\x80\x9d\xcck\xc9Ono\xf1>\x99\x14}P.\
-\xe3c6+\xfa\xfb\xe5%\x11,\x83\xbd#\x04\x10\x82\
-\x9c\x09\x9c\xd7\xeb2\xef\x5c8\x8c\xa3JEf~a\
-Y\xf8q}-\x9a\x17{\x02\x02E/\x0f\x09\x80\xd5\
-\x95\x15\xc9/j5\xac'\x12}\x1a*\xf4!\x93\x11\
-}X*\x81=B \x05&\x08JwwB`\x99\
-&\xce\xaaU\xe9\x1aa\x9a\x9b\x9b1\x82~\x81\xa7\xa7\
-`\x04\x9f \x1d\x8dJ^j4\xf0&\x1e\x17}N\
-\xfb\xf1.\x9d\xee\xd3P!)@\xde\xb1M\xf4\x09*\
-\xcd\xa6\x10\x98\xb3\xb3\xb8\xa21\xb8k\x98hN\x07\xfb\
-\xe1\x7fF\xf6\xeaTEW\x13\xe7 \xb1\xb4\x84\x14Q\
-\xf4\x1e\x1f\x91\xb5m\xac\xc6b\xe8\xf6zX\xa3/\xf2\
-6\x95\x1a\x8e@^\xa3\xd7\xed\xceL\x12T[-!\
-\xe0U\xa61\xfc\xae\x174\xc6(\x01{\x8d\xdf\xf7\xf7\
-f(\x14\xc2n\xea\xef\xe0\x84\x9b\xff\xf5o\xb1\x87\xbd\
-\x9ae\xdb_\xf5Hdy\x9a\x9f\xc9\xedt~\xf2\xd0\
-\x16\xc5K\x0a\xe3\x99~\x87\xe2\xcf?\x01\x06\x00@(\
-K\xf8\xa2\x22\x9e\x10\x00\x00\x00\x00IEND\xaeB\
-`\x82\
 \x00\x00\x02\x86\
 \x89\
 PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
 \x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
 \x00\x00\x00\x19tEXtSoftware\
 \x00Adobe ImageRead\
 yq\xc9e<\x00\x00\x02(IDATx\xda|\
@@ -1395,14 +1357,52 @@
 \x17+\x0cJ#ci\xc2\xc4S\xfc\x7f_\x99\xfc\xb8\
 \xf1\xf2\xce!\xd1\xac\xad\x15?\xae\xeb\x83\xf8b;+\
 \xeb:a\xe4\x071N}\xf6\xec\xf7\x0fhRq\x5c\
 \x07[o\x17\x1em\xb7l\x06\xaf\xde\x1d\x07\xc7\xf8\xe6\
 ~\xb8\xff\x18y\x12\xa8\xd2\x1c\xe9\xcb\x04I\x7f\x04\x18\
 \x00*-\x12\x92\xf2.p\xe1\x00\x00\x00\x00IEN\
 D\xaeB`\x82\
+\x00\x00\x023\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x01\xd5IDATx\xda\x9c\
+\x93\xcbN\xdbP\x10\x86\x7f\x1b\x07\xc7\xa1E\xed\x12P\
+@N\x94\x8b\x12TQ\xaa\xaaR\xb7\xa1\xec\xba+\xef\
+@\xf7\xac\x13)O\xd1\x15O\xc0\x1b\xb0\xab*\x10 \
+\xee\x09\x8a\x88\x92\x88\xa6QV\xa8\x8bV!\x01\x1f\xbb\
+3\x93\xd8\xb9\xacJ\x8e4\xf2?\xb6\xff\x99o\x8e\x8f\
+\xb5\xadB\xe13\x80\x05L\xb7\xda\x86\xeb\xba\x8b{\xc5\
+\xe2\xb7i\xdc_\xf2\xf9m\xc3UJ\xf3(\xd9<\x05\
+<\xcf\x0b\x82\x0aKx|\x1d\xcd\x07\xcf\x8fs\xaf\xc0\
+^])\xa5\xf3\x0b\xbc>\xc55\xb9n\xc4\x86:G\
+:g{\xc1}_\xb3\x87\xbd\x86r\x1cMI\x01\x0d\
+\xfb5\x0f1\xa3K\x93u\xa4\xf3\x86E\x1d\xdb.4\
+z\xce\xda\x0d4\x99\xbdy\xb0\xd7p\x1cg\x8c\xc0\xfd\
+\xf5\x80\x9d\xcck\xc9Ono\xf1>\x99\x14}P.\
+\xe3c6+\xfa\xfb\xe5%\x11,\x83\xbd#\x04\x10\x82\
+\x9c\x09\x9c\xd7\xeb2\xef\x5c8\x8c\xa3JEf~a\
+Y\xf8q}-\x9a\x17{\x02\x02E/\x0f\x09\x80\xd5\
+\x95\x15\xc9/j5\xac'\x12}\x1a*\xf4!\x93\x11\
+}X*\x81=B \x05&\x08JwwB`\x99\
+&\xce\xaaU\xe9\x1aa\x9a\x9b\x9b1\x82~\x81\xa7\xa7\
+`\x04\x9f \x1d\x8dJ^j4\xf0&\x1e\x17}N\
+\xfb\xf1.\x9d\xee\xd3P!)@\xde\xb1M\xf4\x09*\
+\xcd\xa6\x10\x98\xb3\xb3\xb8\xa21\xb8k\x98hN\x07\xfb\
+\xe1\x7fF\xf6\xeaTEW\x13\xe7 \xb1\xb4\x84\x14Q\
+\xf4\x1e\x1f\x91\xb5m\xac\xc6b\xe8\xf6zX\xa3/\xf2\
+6\x95\x1a\x8e@^\xa3\xd7\xed\xceL\x12T[-!\
+\xe0U\xa61\xfc\xae\x174\xc6(\x01{\x8d\xdf\xf7\xf7\
+f(\x14\xc2n\xea\xef\xe0\x84\x9b\xff\xf5o\xb1\x87\xbd\
+\x9ae\xdb_\xf5Hdy\x9a\x9f\xc9\xedt~\xf2\xd0\
+\x16\xc5K\x0a\xe3\x99~\x87\xe2\xcf?\x01\x06\x00@(\
+K\xf8\xa2\x22\x9e\x10\x00\x00\x00\x00IEND\xaeB\
+`\x82\
 \x00\x00\x02$\
 \x89\
 PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
 \x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
 \x00\x00\x00\x19tEXtSoftware\
 \x00Adobe ImageRead\
 yq\xc9e<\x00\x00\x01\xc6IDATx\xda\xa4\
@@ -2913,14 +2913,55 @@
 \xa4\xa6I`\x10\xcc\xc9\x93\xad\xec\xe5\xedo{t\xeb\
 \x89M\xf2{\x18\xd6\xa1G\xb5|\x22I\x80cdh\
 \x10\xa5\xb2&\x11\xcfZ\xfc;\x84`W\xd6\xa5#e\
 \x04\xaalfq\xf7\xc9\x8d\xf1\xe5W`n\xb1\xafN\
 \xd0\xf2\xb8\xf6\xed\xe3\xa6\xf9\xe1\x8d\xa7a\xd3X}6\
 SJ\x11\xb3\xeb\xb6\xf3\x85\x00\x03\x00Kb\x16\x94\x80\
 n\x06\x02\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x02e\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
+\x00\x00\x00\x19tEXtSoftware\
+\x00Adobe ImageRead\
+yq\xc9e<\x00\x00\x02\x07IDATx\xda\x84\
+\x93AH\x14a\x14\xc7\xff\xf3\xedHM\xb8\x91\x82\xc5\
+\x8a\x1e<\xec\x12\x82\x10\xe8a\x0e\xab\xc2FBD\x07\
+!\xa8C\xd0\xb5SH\xe7RX:t\x8a\x10\xc1\xd5\
+\xe3\xe2\xde<u\x90b#\x10\x16\xc1C2\xd0\xc5H\
+\xf0\xa6\x08\xb5\x12;\xda\xba3\xf3}\xbd\xf7\xed\xec\xce\
+\xb4\xad\xfa\xe0\xcd\xfbf\xde\xbc\xdf\xfb\xbf\xf9\xe63\x1e\
+\xcd\xcf\x83\xcd0\x8c\x87\x14R\xb8\xd8\xbeH)\xf7d\
+\x10@)\x85\xddJ\x05&/\xd8(\x0e\x16\x17\x16\x0a\
+\x0dJz\xecR\x22\xa0\x5c+\xef8\x0e\x8a\xe5\xf2s\
+\xeeE\xfe\x83\x9f\xdd\xcef!\x98\x16\xba!\xb9\xc8\xf3\
+\xb47\xeau\xfc99\x81\xeb\xba\xa8\xd5j:\xae\xe7\
+\xf3\x05z\xef.\xd5\xa6[\x92\xcc\x80\x8aC3\x18-\
+\xe8\xda\x93HD\xa2}\x1f>\x81\xab\xd5*\x96J%\
+\xe4FG\x97\x17K\xa5\xd7\x94y\xa3\x012\x02\x08.\
+\x16\x1a\x83\xff \xb9\x5cN\x8f\x93L&\xf1\xc9q\x8e\
+\xdb\x0a\xfc\xb8\x82\x18\xa0\x1b\x84\x95\xe8%\x8d\x1b\x8d@\
+\x89\xce\x11\xe2\xd6\x09\xe1&T\xd3\x15\xd0\x1cA\x08 \
+\xec\xd4\x0d\x92h\x02D4B\x0c\xd0Vp\x01$A\
+\xd1?\x07\xa0\xbf\x81\xfe\x0eM=]!\x85\xedS\xa8\
+\xd4\xe4D\x10(x\x8d3\x1a\x81\xf6\xbcS\x01\x97\x9d\
+\x07\xf9~T\x87w\xe3\xce\x94\xea\xe9}z\xe6\xbak\
+\xff\x8e\xc0\x0ah\xab\xe2\x90\xb7\x9f\x8f\xb0KE*\x92\
+\x89g\x8f\xc7\x86\x96\x8b\xdf\xe6\x14\xc1\xc5\xef\xc3C\x9e\
+\x89\xbd\xbd\x0b\xedH\xee\xec\xffBv&\x83\x01;\x83\
+\xab\x13\x19\x5c\x19Oc\xeb'povl\xfc\xd4\xad\
+\xcd\x99{\x9b\x9b\x18\xb6mX}}f\xab\x03w\x96\
+\xa1\x92t\xbf\x89\x0fk\x15\x84\x07Fo\xb6;\x95E\
+ye\xe3\xab!\xc4{~l\x91\xdf\xbce\xdby\x15\
+3\x02\xa8@JE?\x8f\xa2\xc3\xa5\xe8\x90\xa9\xba\xef\
+\xab\xc9W\x1f\xd5\xf5'\xab\x07\xd7\xa6_\xbe\xe0ZV\
+\xdbO>h\x8d\x8c\xcc\x08\xcb\x1a\xb8\xe48\xc3O=\
+\xb8\xaf\x8e\xf7w\x1a;\xeb\xef\xe8\xf6\xe0\xaf\x00\x03\x00\
+#5\x19?I\x9f6P\x00\x00\x00\x00IEND\
+\xaeB`\x82\
 \x00\x00\x02\x98\
 \x89\
 PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
 \x00\x00\x10\x00\x00\x00\x10\x08\x06\x00\x00\x00\x1f\xf3\xffa\
 \x00\x00\x00\x19tEXtSoftware\
 \x00Adobe ImageRead\
 yq\xc9e<\x00\x00\x02:IDATx\xda\x94\
@@ -3338,23 +3379,23 @@
 \x00p\x00p\x00l\x00i\x00c\x00a\x00t\x00i\x00o\x00n\x00-\x00w\x00a\x00v\x00e\x00.\
 \x00p\x00n\x00g\
 \x00\x14\
 \x02Gc'\
 \x00d\
 \x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00-\x00p\x00e\x00n\x00c\x00i\x00l\x00.\
 \x00p\x00n\x00g\
-\x00\x09\
-\x09(\xa3\xa7\
-\x00t\
-\x00a\x00b\x00l\x00e\x00.\x00p\x00n\x00g\
 \x00\x12\
 \x05\xb4\x8ag\
 \x00a\
 \x00r\x00r\x00o\x00w\x00-\x00s\x00t\x00e\x00p\x00-\x00o\x00u\x00t\x00.\x00p\x00n\
 \x00g\
+\x00\x09\
+\x09(\xa3\xa7\
+\x00t\
+\x00a\x00b\x00l\x00e\x00.\x00p\x00n\x00g\
 \x00\x08\
 \x05\xa8Y\xe7\
 \x00n\
 \x00o\x00d\x00e\x00.\x00p\x00n\x00g\
 \x00\x16\
 \x02M\xd2'\
 \x00r\
@@ -3495,14 +3536,19 @@
 \x0d\xc8^g\
 \x00p\
 \x00i\x00n\x00-\x00-\x00p\x00l\x00u\x00s\x00.\x00p\x00n\x00g\
 \x00\x08\
 \x00/Z\xe7\
 \x00f\
 \x00i\x00l\x00l\x00.\x00p\x00n\x00g\
+\x00\x13\
+\x0e\xd5('\
+\x00d\
+\x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00-\x00a\x00r\x00r\x00o\x00w\x00.\x00p\
+\x00n\x00g\
 \x00\x12\
 \x08K\xc1\xa7\
 \x00d\
 \x00a\x00t\x00a\x00b\x00a\x00s\x00e\x00-\x00-\x00p\x00l\x00u\x00s\x00.\x00p\x00n\
 \x00g\
 \x00\x11\
 \x0ba\x09\xc7\
@@ -3528,164 +3574,166 @@
 \x00p\x00p\x00l\x00i\x00c\x00a\x00t\x00i\x00o\x00n\x00-\x00b\x00l\x00o\x00c\x00k\
 \x00.\x00p\x00n\x00g\
 "
 
 qt_resource_struct = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00J\x00\x00\x00\x02\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00K\x00\x00\x00\x02\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x0a\xc2\x00\x00\x00\x00\x00\x01\x00\x00\xaaB\
-\x00\x00\x01\x86Et\x06\x08\
+\x00\x00\x01\x86E\xaa\xf0`\
 \x00\x00\x01\x0e\x00\x00\x00\x00\x00\x01\x00\x00\x0cQ\
-\x00\x00\x01\x86Et\x87*\
+\x00\x00\x01\x86E\xabu0\
 \x00\x00\x05P\x00\x00\x00\x00\x00\x01\x00\x00HP\
-\x00\x00\x01\x86Es\xa6\x16\
+\x00\x00\x01\x86E\xaa\x92\xa0\
 \x00\x00\x07\xa8\x00\x00\x00\x00\x00\x01\x00\x00o\xd3\
-\x00\x00\x01\x86Es\xf4n\
+\x00\x00\x01\x86E\xaa\xe0\xc0\
 \x00\x00\x08\xe6\x00\x00\x00\x00\x00\x01\x00\x00\x88\xad\
-\x00\x00\x01\x86Es\xf3\x0e\
+\x00\x00\x01\x86E\xaa\xe0\xc0\
 \x00\x00\x07~\x00\x00\x00\x00\x00\x01\x00\x00mp\
-\x00\x00\x01\x86Es\xf0\xbe\
+\x00\x00\x01\x86E\xaa\xd8\xf0\
 \x00\x00\x04\x00\x00\x00\x00\x00\x00\x01\x00\x006\x19\
-\x00\x00\x01\x86Es\xcfV\
-\x00\x00\x0b\x90\x00\x00\x00\x00\x00\x01\x00\x00\xba&\
-\x00\x00\x01\x86Es\xa2\x98\
+\x00\x00\x01\x86E\xaa\xb9\xb0\
+\x00\x00\x0b\xbc\x00\x00\x00\x00\x00\x01\x00\x00\xbc\x8f\
+\x00\x00\x01\x86E\xaa\x8a\xd0\
 \x00\x00\x02\x82\x00\x00\x00\x00\x00\x01\x00\x00 \x96\
-\x00\x00\x01\x86Et\x1fA\
+\x00\x00\x01\x86E\xab\x07\xd0\
 \x00\x00\x08l\x00\x00\x00\x00\x00\x01\x00\x00\x80'\
-\x00\x00\x01\x86Es\xa8\x9e\
+\x00\x00\x01\x86E\xaa\x92\xa0\
 \x00\x00\x05~\x00\x00\x00\x00\x00\x01\x00\x00J\x9a\
-\x00\x00\x01\x86Es\xf0\xae\
+\x00\x00\x01\x86E\xaa\xd8\xf0\
 \x00\x00\x06\x04\x00\x00\x00\x00\x00\x01\x00\x00T<\
-\x00\x00\x01\x86EtL\x85\
+\x00\x00\x01\x86E\xab6\xb0\
 \x00\x00\x09\x5c\x00\x00\x00\x00\x00\x01\x00\x00\x8f\xa0\
-\x00\x00\x01\x86Es\xbc\x83\
+\x00\x00\x01\x86E\xaa\xaa\x10\
 \x00\x00\x0a\x0e\x00\x00\x00\x00\x00\x01\x00\x00\x9bN\
-\x00\x00\x01\x86Es\xf0\x9f\
+\x00\x00\x01\x86E\xaa\xd8\xf0\
 \x00\x00\x01\x84\x00\x00\x00\x00\x00\x01\x00\x00\x13B\
-\x00\x00\x01\x86Et\x87\xca\
+\x00\x00\x01\x86E\xabu0\
 \x00\x00\x06\xa2\x00\x00\x00\x00\x00\x01\x00\x00`p\
-\x00\x00\x01\x86Et\x1f\x00\
+\x00\x00\x01\x86E\xab\x07\xd0\
 \x00\x00\x00\xda\x00\x00\x00\x00\x00\x01\x00\x00\x0a\xb2\
-\x00\x00\x01\x86Es\xe4:\
+\x00\x00\x01\x86E\xaa\xd1 \
 \x00\x00\x02\xd4\x00\x00\x00\x00\x00\x01\x00\x00%\xc1\
-\x00\x00\x01\x86EtO)\
+\x00\x00\x01\x86E\xab6\xb0\
 \x00\x00\x07,\x00\x00\x00\x00\x00\x01\x00\x00g\x91\
-\x00\x00\x01\x86Es\xdc)\
+\x00\x00\x01\x86E\xaa\xc9P\
 \x00\x00\x08*\x00\x00\x00\x00\x00\x01\x00\x00z\xea\
-\x00\x00\x01\x86EtJ\x11\
+\x00\x00\x01\x86E\xab6\xb0\
 \x00\x00\x07X\x00\x00\x00\x00\x00\x01\x00\x00jB\
-\x00\x00\x01\x86Et\x0d\x91\
+\x00\x00\x01\x86E\xaa\xf80\
 \x00\x00\x01\xde\x00\x00\x00\x00\x00\x01\x00\x00\x16\x99\
-\x00\x00\x01\x86Ett\x96\
+\x00\x00\x01\x86E\xab]\xc0\
 \x00\x00\x00^\x00\x00\x00\x00\x00\x01\x00\x00\x03\xa6\
-\x00\x00\x01\x86Es\xec'\
+\x00\x00\x01\x86E\xaa\xd8\xf0\
 \x00\x00\x04\x5c\x00\x00\x00\x00\x00\x01\x00\x009\xaf\
-\x00\x00\x01\x86Et\x1f\x0f\
+\x00\x00\x01\x86E\xab\x07\xd0\
 \x00\x00\x00,\x00\x00\x00\x00\x00\x01\x00\x00\x01\xda\
-\x00\x00\x01\x86Es\xa2\xf3\
+\x00\x00\x01\x86E\xaa\x8a\xd0\
 \x00\x00\x012\x00\x00\x00\x00\x00\x01\x00\x00\x0e\x80\
-\x00\x00\x01\x86Et7\x22\
+\x00\x00\x01\x86E\xab\x1f@\
 \x00\x00\x06\xd0\x00\x00\x00\x00\x00\x01\x00\x00bW\
-\x00\x00\x01\x86Eto_\
+\x00\x00\x01\x86E\xab]\xc0\
 \x00\x00\x06Z\x00\x00\x00\x00\x00\x01\x00\x00[\xa5\
-\x00\x00\x01\x86Es\xacM\
-\x00\x00\x0b*\x00\x00\x00\x00\x00\x01\x00\x00\xb2\x16\
-\x00\x00\x01\x86Es\xecd\
+\x00\x00\x01\x86E\xaa\x9ap\
+\x00\x00\x0bV\x00\x00\x00\x00\x00\x01\x00\x00\xb4\x7f\
+\x00\x00\x01\x86E\xaa\xd8\xf0\
 \x00\x00\x0a:\x00\x00\x00\x00\x00\x01\x00\x00\x9d\x86\
-\x00\x00\x01\x86Et%#\
+\x00\x00\x01\x86E\xab\x0f\xa0\
 \x00\x00\x05\xee\x00\x00\x00\x00\x00\x01\x00\x00R\x14\
-\x00\x00\x01\x86Et7q\
-\x00\x00\x05\xc4\x00\x00\x00\x00\x00\x01\x00\x00O\x8a\
-\x00\x00\x01\x86Es\xac\x9d\
+\x00\x00\x01\x86E\xab\x1f@\
+\x00\x00\x05\xac\x00\x00\x00\x00\x00\x01\x00\x00MS\
+\x00\x00\x01\x86E\xaa\x9ap\
 \x00\x00\x09\xec\x00\x00\x00\x00\x00\x01\x00\x00\x98f\
-\x00\x00\x01\x86Es\xab\x07\
-\x00\x00\x0bz\x00\x00\x00\x00\x00\x01\x00\x00\xb72\
-\x00\x00\x01\x86Et\x16.\
+\x00\x00\x01\x86E\xaa\x92\xa0\
+\x00\x00\x0b\xa6\x00\x00\x00\x00\x00\x01\x00\x00\xb9\x9b\
+\x00\x00\x01\x86E\xab\x00\x00\
 \x00\x00\x09\x8e\x00\x00\x00\x00\x00\x01\x00\x00\x92s\
-\x00\x00\x01\x86Et\x87\xec\
+\x00\x00\x01\x86E\xabu0\
 \x00\x00\x020\x00\x00\x00\x00\x00\x01\x00\x00\x1b\x81\
-\x00\x00\x01\x86EtL\xc8\
+\x00\x00\x01\x86E\xab6\xb0\
 \x00\x00\x04\xc8\x00\x00\x00\x00\x00\x01\x00\x00?t\
-\x00\x00\x01\x86EtL\xb7\
+\x00\x00\x01\x86E\xab6\xb0\
 \x00\x00\x02\x12\x00\x00\x00\x00\x00\x01\x00\x00\x18|\
-\x00\x00\x01\x86EtI\x1b\
+\x00\x00\x01\x86E\xab6\xb0\
 \x00\x00\x05*\x00\x00\x00\x00\x00\x01\x00\x00E*\
-\x00\x00\x01\x86Es\xa8\xee\
+\x00\x00\x01\x86E\xaa\x92\xa0\
 \x00\x00\x048\x00\x00\x00\x00\x00\x01\x00\x007\xaa\
-\x00\x00\x01\x86Et\x1fQ\
+\x00\x00\x01\x86E\xab\x07\xd0\
 \x00\x00\x04\x90\x00\x00\x00\x00\x00\x01\x00\x00<6\
-\x00\x00\x01\x86Es\xa8\xad\
+\x00\x00\x01\x86E\xaa\x92\xa0\
 \x00\x00\x03P\x00\x00\x00\x00\x00\x01\x00\x00,\xc6\
-\x00\x00\x01\x86Et\x87\xbd\
+\x00\x00\x01\x86E\xabu0\
 \x00\x00\x07\xd4\x00\x00\x00\x00\x00\x01\x00\x00r\x87\
-\x00\x00\x01\x86EtM\x91\
-\x00\x00\x0a\xd8\x00\x00\x00\x00\x00\x01\x00\x00\xacv\
-\x00\x00\x01\x86Es\xec=\
+\x00\x00\x01\x86E\xab6\xb0\
+\x00\x00\x0b\x04\x00\x00\x00\x00\x00\x01\x00\x00\xae\xdf\
+\x00\x00\x01\x86E\xaa\xd8\xf0\
 \x00\x00\x09\x0e\x00\x00\x00\x00\x00\x01\x00\x00\x8b\x0f\
-\x00\x00\x01\x86Es\xe1\xfc\
+\x00\x00\x01\x86E\xaa\xc9P\
 \x00\x00\x02\xb0\x00\x00\x00\x00\x00\x01\x00\x00#\x02\
-\x00\x00\x01\x86Es\xb6\x88\
-\x00\x00\x05\xac\x00\x00\x00\x00\x00\x01\x00\x00MS\
-\x00\x00\x01\x86Eth}\
+\x00\x00\x01\x86E\xaa\xa2@\
+\x00\x00\x05\xd6\x00\x00\x00\x00\x00\x01\x00\x00O\xdd\
+\x00\x00\x01\x86E\xabU\xf0\
 \x00\x00\x06\xf8\x00\x00\x00\x00\x00\x01\x00\x00d\x94\
-\x00\x00\x01\x86Et\x1e\xef\
+\x00\x00\x01\x86E\xab\x07\xd0\
 \x00\x00\x00\x10\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x86Es\xe4_\
+\x00\x00\x01\x86E\xaa\xd1 \
 \x00\x00\x0aP\x00\x00\x00\x00\x00\x01\x00\x00\xa3\x89\
-\x00\x00\x01\x86Et7\x02\
+\x00\x00\x01\x86E\xab\x1f@\
 \x00\x00\x066\x00\x00\x00\x00\x00\x01\x00\x00Y\xe3\
-\x00\x00\x01\x86Et6\xb7\
+\x00\x00\x01\x86E\xab\x1f@\
 \x00\x00\x08\xc8\x00\x00\x00\x00\x00\x01\x00\x00\x85\xfc\
-\x00\x00\x01\x86Et\x04E\
+\x00\x00\x01\x86E\xaa\xf0`\
 \x00\x00\x09\xa4\x00\x00\x00\x00\x00\x01\x00\x00\x94)\
-\x00\x00\x01\x86Es\xac\xbe\
+\x00\x00\x01\x86E\xaa\x9ap\
 \x00\x00\x04\xfc\x00\x00\x00\x00\x00\x01\x00\x00B1\
-\x00\x00\x01\x86Eti\xaa\
+\x00\x00\x01\x86E\xabU\xf0\
 \x00\x00\x03\xce\x00\x00\x00\x00\x00\x01\x00\x003\xd9\
-\x00\x00\x01\x86Et\x87\xae\
+\x00\x00\x01\x86E\xabu0\
 \x00\x00\x09\xc6\x00\x00\x00\x00\x00\x01\x00\x00\x96\xaf\
-\x00\x00\x01\x86Ett\x87\
+\x00\x00\x01\x86E\xab]\xc0\
 \x00\x00\x08\x9a\x00\x00\x00\x00\x00\x01\x00\x00\x83h\
-\x00\x00\x01\x86Es\xad}\
+\x00\x00\x01\x86E\xaa\x9ap\
 \x00\x00\x098\x00\x00\x00\x00\x00\x01\x00\x00\x8dG\
-\x00\x00\x01\x86Et6\xc5\
-\x00\x00\x0b\x02\x00\x00\x00\x00\x00\x01\x00\x00\xaf\x12\
-\x00\x00\x01\x86EtH\xec\
+\x00\x00\x01\x86E\xab\x1f@\
+\x00\x00\x0b.\x00\x00\x00\x00\x00\x01\x00\x00\xb1{\
+\x00\x00\x01\x86E\xab6\xb0\
 \x00\x00\x00\xb6\x00\x00\x00\x00\x00\x01\x00\x00\x08\xb6\
-\x00\x00\x01\x86Es\xc7\x0d\
+\x00\x00\x01\x86E\xaa\xb1\xe0\
 \x00\x00\x02X\x00\x00\x00\x00\x00\x01\x00\x00\x1d\x88\
-\x00\x00\x01\x86EtF\xe0\
+\x00\x00\x01\x86E\xab.\xe0\
 \x00\x00\x01^\x00\x00\x00\x00\x00\x01\x00\x00\x10\xb7\
-\x00\x00\x01\x86EtS\xdc\
+\x00\x00\x01\x86E\xab>\x80\
 \x00\x00\x03\x10\x00\x00\x00\x00\x00\x01\x00\x00*P\
-\x00\x00\x01\x86Es\xb9@\
+\x00\x00\x01\x86E\xaa\xa2@\
 \x00\x00\x08H\x00\x00\x00\x00\x00\x01\x00\x00}\xec\
-\x00\x00\x01\x86EtP\xd0\
+\x00\x00\x01\x86E\xab>\x80\
 \x00\x00\x00\x8c\x00\x00\x00\x00\x00\x01\x00\x00\x06c\
-\x00\x00\x01\x86Es\xdc\x86\
+\x00\x00\x01\x86E\xaa\xc9P\
 \x00\x00\x0at\x00\x00\x00\x00\x00\x01\x00\x00\xa5O\
-\x00\x00\x01\x86EtT=\
+\x00\x00\x01\x86E\xab>\x80\
 \x00\x00\x06|\x00\x00\x00\x00\x00\x01\x00\x00^\x12\
-\x00\x00\x01\x86Et\x18\x1e\
+\x00\x00\x01\x86E\xab\x00\x00\
 \x00\x00\x0a\xa2\x00\x00\x00\x00\x00\x01\x00\x00\xa7\x7f\
-\x00\x00\x01\x86EtB\x03\
+\x00\x00\x01\x86E\xab.\xe0\
 \x00\x00\x03t\x00\x00\x00\x00\x00\x01\x00\x00.\xe1\
-\x00\x00\x01\x86Etch\
-\x00\x00\x0bV\x00\x00\x00\x00\x00\x01\x00\x00\xb4\xb8\
-\x00\x00\x01\x86Et7a\
+\x00\x00\x01\x86E\xabN \
+\x00\x00\x0b\x82\x00\x00\x00\x00\x00\x01\x00\x00\xb7!\
+\x00\x00\x01\x86E\xab\x1f@\
+\x00\x00\x0a\xd8\x00\x00\x00\x00\x00\x01\x00\x00\xacv\
+\x00\x00\x01\x86E\xaa\xd8\xf0\
 \x00\x00\x02\xec\x00\x00\x00\x00\x00\x01\x00\x00(4\
-\x00\x00\x01\x86EtS\x9a\
+\x00\x00\x01\x86E\xab>\x80\
 \x00\x00\x01\xa8\x00\x00\x00\x00\x00\x01\x00\x00\x14\xd3\
-\x00\x00\x01\x86Et\x1f \
+\x00\x00\x01\x86E\xab\x07\xd0\
 \x00\x00\x03\xa2\x00\x00\x00\x00\x00\x01\x00\x001\x03\
-\x00\x00\x01\x86Es\xec\x88\
+\x00\x00\x01\x86E\xaa\xd8\xf0\
 \x00\x00\x08\x02\x00\x00\x00\x00\x00\x01\x00\x00xQ\
-\x00\x00\x01\x86Es\xf7\x97\
+\x00\x00\x01\x86E\xaa\xe0\xc0\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
     QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
```

### Comparing `revolution-eda-0.5.1/revinit.py` & `revolution-eda-0.5.2/revinit.py`

 * *Files identical despite different names*

### Comparing `revolution-eda-0.5.1/revolution_eda.egg-info/PKG-INFO` & `revolution-eda-0.5.2/revolution_eda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revolution-eda
-Version: 0.5.1
+Version: 0.5.2
 Summary: Revolution EDA is a new generation integrated circuit design environment.
 Project-URL: Homepage, https://github.com/eskiyerli/revedaRelease
 Keywords: electronic,design,schematic
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

