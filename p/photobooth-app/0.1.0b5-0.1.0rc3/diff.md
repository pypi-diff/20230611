# Comparing `tmp/photobooth_app-0.1.0b5.tar.gz` & `tmp/photobooth_app-0.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photobooth_app-0.1.0b5.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `photobooth_app-0.1.0b5.tar` & `photobooth_app-0.1.0rc3.tar`

### file list

```diff
@@ -1,135 +1,136 @@
--rw-r--r--   0        0        0     1084 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/LICENSE.md
--rw-r--r--   0        0        0     3305 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/README.md
--rw-r--r--   0        0        0       33 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/__init__.py
--rw-r--r--   0        0        0     3726 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/__main__.py
--rw-r--r--   0        0        0    17065 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/appconfig.py
--rw-r--r--   0        0        0     3322 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/application.py
--rw-r--r--   0        0        0     1427 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/containers.py
--rw-r--r--   0        0        0       36 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/__init__.py
--rw-r--r--   0        0        0     3379 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/aquisition.py
--rw-r--r--   0        0        0     2326 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/config.py
--rw-r--r--   0        0        0      593 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/home.py
--rw-r--r--   0        0        0      770 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/log.py
--rw-r--r--   0        0        0     2133 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/mediacollection.py
--rw-r--r--   0        0        0     3390 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/mediaprocessing.py
--rw-r--r--   0        0        0     1135 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/processing.py
--rw-r--r--   0        0        0     3908 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/sse.py
--rw-r--r--   0        0        0     1942 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/system.py
--rw-r--r--   0        0        0       36 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/services/__init__.py
--rw-r--r--   0        0        0     3121 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/services/aquisitionservice.py
--rw-r--r--   0        0        0      463 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/services/assets/systemservice/boothupload.service
--rw-r--r--   0        0        0      368 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/services/assets/systemservice/boothupload.sh
--rw-r--r--   0        0        0      699 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/services/assets/systemservice/photobooth-app.service
--rw-r--r--   0        0        0       36 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/services/backends/__init__.py
--rw-r--r--   0        0        0     7195 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/services/backends/abstractbackend.py
--rw-r--r--   0        0        0    11560 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
--rw-r--r--   0        0        0   167336 2023-06-10 11:33:48.008122 photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
--rw-r--r--   0        0        0   710982 2023-06-10 11:33:48.012122 photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
--rw-r--r--   0        0        0   585221 2023-06-10 11:33:48.016122 photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
--rw-r--r--   0        0        0   865667 2023-06-10 11:33:48.020122 photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
--rw-r--r--   0        0        0  2314332 2023-06-10 11:33:48.036122 photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
--rw-r--r--   0        0        0  2126411 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
--rw-r--r--   0        0        0    43739 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
--rw-r--r--   0        0        0     2618 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/containers.py
--rw-r--r--   0        0        0    10517 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/gphoto2.py
--rw-r--r--   0        0        0    16264 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/picamera2.py
--rw-r--r--   0        0        0     3001 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/picamera2_libcamafcontinuous.py
--rw-r--r--   0        0        0     4473 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/picamera2_libcamafinterval.py
--rw-r--r--   0        0        0     6965 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/simulated.py
--rw-r--r--   0        0        0    10084 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/webcamcv2.py
--rw-r--r--   0        0        0     7597 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/webcamv4l.py
--rw-r--r--   0        0        0      506 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/baseservice.py
--rw-r--r--   0        0        0     3207 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/containers.py
--rw-r--r--   0        0        0     4202 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/informationservice.py
--rw-r--r--   0        0        0     2022 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/keyboardservice.py
--rw-r--r--   0        0        0     6280 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/loggingservice.py
--rw-r--r--   0        0        0       36 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/mediacollection/__init__.py
--rw-r--r--   0        0        0     6853 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/mediacollection/mediaitem.py
--rw-r--r--   0        0        0     6010 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/mediacollectionservice.py
--rw-r--r--   0        0        0     1934 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/mediaprocessing/image_pipelinestages.py
--rw-r--r--   0        0        0    10102 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/mediaprocessingservice.py
--rw-r--r--   0        0        0     8753 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/processingservice.py
--rw-r--r--   0        0        0     4068 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/systemservice.py
--rw-r--r--   0        0        0     5647 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/wledservice.py
--rw-r--r--   0        0        0       93 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/utils/exceptions.py
--rw-r--r--   0        0        0      430 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/utils/fastapi_get_openapi.py
--rw-r--r--   0        0        0      454 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/utils/helper.py
--rw-r--r--   0        0        0      883 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/utils/repeatedtimer.py
--rw-r--r--   0        0        0      621 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/utils/stoppablethread.py
--rw-r--r--   0        0        0    11358 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   168060 2023-06-10 11:33:48.052122 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0        0        0   174108 2023-06-10 11:33:48.052122 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0        0        0   167336 2023-06-10 11:33:48.056122 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2023-06-10 11:33:48.056122 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2023-06-10 11:33:48.056122 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   167000 2023-06-10 11:33:48.060123 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0        0        0   173172 2023-06-10 11:33:48.060123 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0        0        0   168644 2023-06-10 11:33:48.060123 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0        0        0   173416 2023-06-10 11:33:48.064123 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0        0        0   168260 2023-06-10 11:33:48.064123 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0   168488 2023-06-10 11:33:48.064123 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0        0        0   172860 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0        0        0      483 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/.gitattributes
--rw-r--r--   0        0        0     2014 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/.gitignore
--rw-r--r--   0        0        0     6155 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/CHANGES.md
--rw-r--r--   0        0        0     1064 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/LICENSE.txt
--rw-r--r--   0        0        0       56 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/MANIFEST.in
--rw-r--r--   0        0        0      710 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/Makefile
--rw-r--r--   0        0        0    29447 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/README.md
--rw-r--r--   0        0        0      131 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/10_second_macro.py
--rw-r--r--   0        0        0      276 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/customizable_hotkey.py
--rw-r--r--   0        0        0      453 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/pressed_keys.py
--rw-r--r--   0        0        0      660 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py
--rw-r--r--   0        0        0     1601 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/segmented_macro.py
--rw-r--r--   0        0        0      210 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/simulate_held_down.py
--rw-r--r--   0        0        0      857 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py
--rw-r--r--   0        0        0      237 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/write.py
--rw-r--r--   0        0        0    46771 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/__init__.py
--rw-r--r--   0        0        0      364 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/__main__.py
--rw-r--r--   0        0        0    29387 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py
--rw-r--r--   0        0        0    19352 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py
--rw-r--r--   0        0        0     6457 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py
--rw-r--r--   0        0        0     2110 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_generic.py
--rw-r--r--   0        0        0     1551 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py
--rw-r--r--   0        0        0    36792 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py
--rw-r--r--   0        0        0      398 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_mouse_event.py
--rw-r--r--   0        0        0     9984 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py
--rw-r--r--   0        0        0     5947 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py
--rw-r--r--   0        0        0     6254 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py
--rw-r--r--   0        0        0     3384 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py
--rw-r--r--   0        0        0    20549 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py
--rw-r--r--   0        0        0     5804 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py
--rw-r--r--   0        0        0     7608 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/mouse.py
--rw-r--r--   0        0        0     3794 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/make_release.py
--rw-r--r--   0        0        0     1333 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/setup.py
--rw-r--r--   0        0        0      144 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/web_spa/css/31.363e41a9.css
--rw-r--r--   0        0        0       88 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/web_spa/css/706.42cb67d0.css
--rw-r--r--   0        0        0      163 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/web_spa/css/71.0be6c807.css
--rw-r--r--   0        0        0      359 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/web_spa/css/app.f5a22106.css
--rw-r--r--   0        0        0   208939 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/css/vendor.46e03c42.css
--rw-r--r--   0        0        0    64483 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/favicon.ico-todo
--rw-r--r--   0        0        0    20436 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0        0        0    20544 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0        0        0    20416 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0        0        0    20408 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0        0        0    20424 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0        0        0    20344 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0        0        0   164912 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0        0        0   128616 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-r--r--   0        0        0     5336 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/icons/favicon-128x128.png
--rw-r--r--   0        0        0      905 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/index.html
--rw-r--r--   0        0        0     9915 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/31.51d7e662.js
--rw-r--r--   0        0        0     2918 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/391.70a80bd8.js
--rw-r--r--   0        0        0     1217 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/546.92b02def.js
--rw-r--r--   0        0        0     3034 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/645.2ddc3ded.js
--rw-r--r--   0        0        0     5660 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/692.cf3b55d3.js
--rw-r--r--   0        0        0     3924 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/705.fc48b137.js
--rw-r--r--   0        0        0     9305 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/706.f32434a0.js
--rw-r--r--   0        0        0     5357 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/71.3aaf5d7d.js
--rw-r--r--   0        0        0     1581 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/770.b7df615e.js
--rw-r--r--   0        0        0      778 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/862.525f2f13.js
--rw-r--r--   0        0        0     1520 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/863.e0c5ac02.js
--rw-r--r--   0        0        0    12590 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/app.ed0492eb.js
--rw-r--r--   0        0        0  1417500 2023-06-10 11:33:48.084123 photobooth_app-0.1.0b5/photobooth/web_spa/js/vendor.c9e02ba9.js
--rw-r--r--   0        0        0     3970 2023-06-10 11:33:48.084123 photobooth_app-0.1.0b5/pyproject.toml
--rw-r--r--   0        0        0     4878 1970-01-01 00:00:00.000000 photobooth_app-0.1.0b5/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/__init__.py
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/__main__.py
+-rw-r--r--   0        0        0    17065 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/appconfig.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/application.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/containers.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/routers/__init__.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/routers/aquisition.py
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/routers/config.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/routers/home.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/routers/log.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/routers/mediacollection.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/routers/mediaprocessing.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/routers/processing.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/routers/sse.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/routers/system.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/__init__.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/aquisitionservice.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/baseservice.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/containers.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/informationservice.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/keyboardservice.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/loggingservice.py
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/mediacollectionservice.py
+-rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/mediaprocessingservice.py
+-rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/processingservice.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/systemservice.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/wledservice.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/assets/systemservice/boothupload.service
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/assets/systemservice/boothupload.sh
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/assets/systemservice/photobooth-app.service
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/__init__.py
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/abstractbackend.py
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/containers.py
+-rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/gphoto2.py
+-rw-r--r--   0        0        0    16283 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/picamera2.py
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/picamera2_libcamafcontinuous.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/picamera2_libcamafinterval.py
+-rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/simulated.py
+-rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/webcamcv2.py
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/webcamv4l.py
+-rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   710982 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
+-rw-r--r--   0        0        0   585221 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
+-rw-r--r--   0        0        0   865667 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
+-rw-r--r--   0        0        0  2314332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
+-rw-r--r--   0        0        0  2126411 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/mediacollection/__init__.py
+-rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/mediacollection/mediaitem.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/services/mediaprocessing/image_pipelinestages.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/utils/exceptions.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/utils/fastapi_get_openapi.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/utils/helper.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/utils/repeatedtimer.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/utils/stoppablethread.py
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   168060 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0        0        0   174108 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   167000 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0        0        0   173172 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0        0        0   168644 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0        0        0   173416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0   168488 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0        0        0   172860 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/.gitattributes
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/.gitignore
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/CHANGES.md
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/LICENSE.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/MANIFEST.in
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/Makefile
+-rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/README.md
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/make_release.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/setup.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/examples/10_second_macro.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/examples/customizable_hotkey.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/examples/pressed_keys.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/examples/segmented_macro.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/examples/simulate_held_down.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/examples/write.py
+-rw-r--r--   0        0        0    46771 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/__main__.py
+-rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py
+-rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_generic.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py
+-rw-r--r--   0        0        0    36792 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_mouse_event.py
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py
+-rw-r--r--   0        0        0    20549 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/mouse.py
+-rw-r--r--   0        0        0    64483 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/favicon.ico-todo
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/index.html
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/css/31.363e41a9.css
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/css/706.42cb67d0.css
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/css/71.0be6c807.css
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/css/app.f5a22106.css
+-rw-r--r--   0        0        0   208939 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/css/vendor.46e03c42.css
+-rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0        0        0    20544 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0        0        0    20424 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0        0        0    20344 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0        0        0   164912 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/icons/favicon-128x128.png
+-rw-r--r--   0        0        0     9915 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/js/31.51d7e662.js
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/js/391.70a80bd8.js
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/js/546.92b02def.js
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/js/645.2ddc3ded.js
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/js/692.cf3b55d3.js
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/js/705.fc48b137.js
+-rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/js/706.f32434a0.js
+-rw-r--r--   0        0        0     5357 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/js/71.3aaf5d7d.js
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/js/770.b7df615e.js
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/js/862.525f2f13.js
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/js/863.e0c5ac02.js
+-rw-r--r--   0        0        0    12590 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/js/app.ed0492eb.js
+-rw-r--r--   0        0        0  1417500 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/photobooth/web_spa/js/vendor.c9e02ba9.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/LICENSE.md
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/README.md
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     5139 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc3/PKG-INFO
```

### Comparing `photobooth_app-0.1.0b5/LICENSE.md` & `photobooth_app-0.1.0rc3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/README.md` & `photobooth_app-0.1.0rc3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# Photobooth App
+# ![photobooth-app logo](https://raw.githubusercontent.com/mgrl/photobooth-app/main/assets/logo/logo-text-black-transparent.png)
+
+Written in Python 🐍, coming along with a modern Vue frontend.
 
 ![python versions supported 3.9, 3.10, 3.11](https://img.shields.io/pypi/pyversions/photobooth-app)
 ![rpi, linux and windows platform supported](https://img.shields.io/badge/platform-rpi%20%7C%20linux%20%7C%20windows-lightgrey)
 [![ruff](https://github.com/mgrl/photobooth-app/actions/workflows/ruff.yml/badge.svg)](https://github.com/mgrl/photobooth-app/actions/workflows/ruff.yml)
 [![pytest](https://github.com/mgrl/photobooth-app/actions/workflows/pytests.yml/badge.svg)](https://github.com/mgrl/photobooth-app/actions/workflows/pytests.yml)
 [![codecov](https://codecov.io/gh/mgrl/photobooth-app/branch/dev/graph/badge.svg?token=SBB5DGX17V)](https://codecov.io/gh/mgrl/photobooth-app)
 
-The photobooth app is written in Python 🐍 and coming along with a modern Vue frontend.
-
 **[Installation](https://mgrl.github.io/photobooth-docs/installation/)** - **[Documentation](https://mgrl.github.io/photobooth-docs/)** - **[PyPI package](https://pypi.org/project/photobooth-app/)** - **[3d printed box](https://mgrl.github.io/photobooth-docs/photobox3dprint/)**
 
 ## 😍 Features
 
 - 📹 camera live preview with shortest delay as possible, permanent video live view in background
 - ⚡️ optimized for speed, live stream hardware accelerated on rpi, cpu load < 20%
 - 🫶 several camera backends supported for high quality stills and livestream
```

### Comparing `photobooth_app-0.1.0b5/photobooth/__main__.py` & `photobooth_app-0.1.0rc3/photobooth/__main__.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/appconfig.py` & `photobooth_app-0.1.0rc3/photobooth/appconfig.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/application.py` & `photobooth_app-0.1.0rc3/photobooth/application.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/containers.py` & `photobooth_app-0.1.0rc3/photobooth/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/routers/aquisition.py` & `photobooth_app-0.1.0rc3/photobooth/routers/aquisition.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/routers/config.py` & `photobooth_app-0.1.0rc3/photobooth/routers/config.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/routers/home.py` & `photobooth_app-0.1.0rc3/photobooth/routers/home.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/routers/log.py` & `photobooth_app-0.1.0rc3/photobooth/routers/log.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/routers/mediacollection.py` & `photobooth_app-0.1.0rc3/photobooth/routers/mediacollection.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/routers/mediaprocessing.py` & `photobooth_app-0.1.0rc3/photobooth/routers/mediaprocessing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/routers/processing.py` & `photobooth_app-0.1.0rc3/photobooth/routers/processing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/routers/sse.py` & `photobooth_app-0.1.0rc3/photobooth/routers/sse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/routers/system.py` & `photobooth_app-0.1.0rc3/photobooth/routers/system.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/aquisitionservice.py` & `photobooth_app-0.1.0rc3/photobooth/services/aquisitionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/assets/systemservice/photobooth-app.service` & `photobooth_app-0.1.0rc3/photobooth/services/assets/systemservice/photobooth-app.service`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/backends/abstractbackend.py` & `photobooth_app-0.1.0rc3/photobooth/services/backends/abstractbackend.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt` & `photobooth_app-0.1.0rc3/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf` & `photobooth_app-0.1.0rc3/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg` & `photobooth_app-0.1.0rc3/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg` & `photobooth_app-0.1.0rc3/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg` & `photobooth_app-0.1.0rc3/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg` & `photobooth_app-0.1.0rc3/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg` & `photobooth_app-0.1.0rc3/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg` & `photobooth_app-0.1.0rc3/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/backends/containers.py` & `photobooth_app-0.1.0rc3/photobooth/services/backends/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/backends/gphoto2.py` & `photobooth_app-0.1.0rc3/photobooth/services/backends/gphoto2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/backends/picamera2.py` & `photobooth_app-0.1.0rc3/photobooth/services/backends/picamera2.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 try:
     from libcamera import Transform  # type: ignore
     from picamera2 import Picamera2  # type: ignore
     from picamera2.encoders import MJPEGEncoder, Quality  # type: ignore
     from picamera2.outputs import FileOutput  # type: ignore
 except Exception as import_exc:
-    raise OSError("picamera2/libcamera not supported on windows platform") from import_exc
+    raise OSError("picamera2/libcamera import error; check picamera2/libcamera installation") from import_exc
 
 logger = logging.getLogger(__name__)
 
 
 class Picamera2Backend(AbstractBackend):
     """
     The backend implementation using picamera2
```

### Comparing `photobooth_app-0.1.0b5/photobooth/services/backends/picamera2_libcamafcontinuous.py` & `photobooth_app-0.1.0rc3/photobooth/services/backends/picamera2_libcamafcontinuous.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/backends/picamera2_libcamafinterval.py` & `photobooth_app-0.1.0rc3/photobooth/services/backends/picamera2_libcamafinterval.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/backends/simulated.py` & `photobooth_app-0.1.0rc3/photobooth/services/backends/simulated.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/backends/webcamcv2.py` & `photobooth_app-0.1.0rc3/photobooth/services/backends/webcamcv2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/backends/webcamv4l.py` & `photobooth_app-0.1.0rc3/photobooth/services/backends/webcamv4l.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     compile_buffer,
     decompile_buffer,
 )
 
 try:
     from v4l2py import Device
 except Exception as import_exc:
-    raise OSError("backend v4l2py not supported on windows platform") from import_exc
+    raise OSError("v4l2py import error; check v4l2py installation") from import_exc
 
 SHARED_MEMORY_BUFFER_BYTES = 15 * 1024**2
 
 logger = logging.getLogger(__name__)
 
 
 class WebcamV4lBackend(AbstractBackend):
```

### Comparing `photobooth_app-0.1.0b5/photobooth/services/containers.py` & `photobooth_app-0.1.0rc3/photobooth/services/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/informationservice.py` & `photobooth_app-0.1.0rc3/photobooth/services/informationservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/keyboardservice.py` & `photobooth_app-0.1.0rc3/photobooth/services/keyboardservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/loggingservice.py` & `photobooth_app-0.1.0rc3/photobooth/services/loggingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/mediacollection/mediaitem.py` & `photobooth_app-0.1.0rc3/photobooth/services/mediacollection/mediaitem.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/mediacollectionservice.py` & `photobooth_app-0.1.0rc3/photobooth/services/mediacollectionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/mediaprocessing/image_pipelinestages.py` & `photobooth_app-0.1.0rc3/photobooth/services/mediaprocessing/image_pipelinestages.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/mediaprocessingservice.py` & `photobooth_app-0.1.0rc3/photobooth/services/mediaprocessingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/processingservice.py` & `photobooth_app-0.1.0rc3/photobooth/services/processingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/systemservice.py` & `photobooth_app-0.1.0rc3/photobooth/services/systemservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/services/wledservice.py` & `photobooth_app-0.1.0rc3/photobooth/services/wledservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/utils/repeatedtimer.py` & `photobooth_app-0.1.0rc3/photobooth/utils/repeatedtimer.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/utils/stoppablethread.py` & `photobooth_app-0.1.0rc3/photobooth/utils/stoppablethread.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/LICENSE.txt` & `photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf` & `photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf` & `photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf` & `photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf` & `photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf` & `photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf` & `photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf` & `photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf` & `photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf` & `photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf` & `photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf` & `photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf` & `photobooth_app-0.1.0rc3/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/.gitignore` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/.gitignore`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/CHANGES.md` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/CHANGES.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/LICENSE.txt` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/Makefile` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/Makefile`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/README.md` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/README.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/segmented_macro.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/examples/segmented_macro.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/__init__.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_generic.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_generic.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/mouse.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/keyboard/mouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/make_release.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/make_release.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/setup.py` & `photobooth_app-0.1.0rc3/photobooth/vendor/packages/keyboard/setup.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/css/vendor.46e03c42.css` & `photobooth_app-0.1.0rc3/photobooth/web_spa/css/vendor.46e03c42.css`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/favicon.ico-todo` & `photobooth_app-0.1.0rc3/photobooth/web_spa/favicon.ico-todo`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `photobooth_app-0.1.0rc3/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `photobooth_app-0.1.0rc3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `photobooth_app-0.1.0rc3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `photobooth_app-0.1.0rc3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `photobooth_app-0.1.0rc3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `photobooth_app-0.1.0rc3/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `photobooth_app-0.1.0rc3/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `photobooth_app-0.1.0rc3/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/icons/favicon-128x128.png` & `photobooth_app-0.1.0rc3/photobooth/web_spa/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/index.html` & `photobooth_app-0.1.0rc3/photobooth/web_spa/index.html`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/js/31.51d7e662.js` & `photobooth_app-0.1.0rc3/photobooth/web_spa/js/31.51d7e662.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/js/391.70a80bd8.js` & `photobooth_app-0.1.0rc3/photobooth/web_spa/js/391.70a80bd8.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/js/546.92b02def.js` & `photobooth_app-0.1.0rc3/photobooth/web_spa/js/546.92b02def.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/js/645.2ddc3ded.js` & `photobooth_app-0.1.0rc3/photobooth/web_spa/js/645.2ddc3ded.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/js/692.cf3b55d3.js` & `photobooth_app-0.1.0rc3/photobooth/web_spa/js/692.cf3b55d3.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/js/705.fc48b137.js` & `photobooth_app-0.1.0rc3/photobooth/web_spa/js/705.fc48b137.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/js/706.f32434a0.js` & `photobooth_app-0.1.0rc3/photobooth/web_spa/js/706.f32434a0.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/js/71.3aaf5d7d.js` & `photobooth_app-0.1.0rc3/photobooth/web_spa/js/71.3aaf5d7d.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/js/770.b7df615e.js` & `photobooth_app-0.1.0rc3/photobooth/web_spa/js/770.b7df615e.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/js/862.525f2f13.js` & `photobooth_app-0.1.0rc3/photobooth/web_spa/js/862.525f2f13.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/js/863.e0c5ac02.js` & `photobooth_app-0.1.0rc3/photobooth/web_spa/js/863.e0c5ac02.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/js/app.ed0492eb.js` & `photobooth_app-0.1.0rc3/photobooth/web_spa/js/app.ed0492eb.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/photobooth/web_spa/js/vendor.c9e02ba9.js` & `photobooth_app-0.1.0rc3/photobooth/web_spa/js/vendor.c9e02ba9.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b5/PKG-INFO` & `photobooth_app-0.1.0rc3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 Metadata-Version: 2.1
 Name: photobooth-app
-Version: 0.1.0b5
+Version: 0.1.0rc3
 Summary: Photobooth app written in Python supporting DSLR, picamera2, webcameras
-Home-page: https://github.com/mgrl/photobooth-app
-License: MIT
-Author: Michael G
-Author-email: me@mgrl.de
-Requires-Python: >=3.9,<3.12
+Project-URL: homepage, https://github.com/mgrl/photobooth-app
+Project-URL: repository, https://github.com/mgrl/photobooth-app
+Project-URL: documentation, https://mgrl.github.io/photobooth-docs
+Author-email: Michael G <me@mgrl.de>
+Maintainer-email: Michael G <me@mgrl.de>
+License-File: LICENSE.md
+Keywords: camera,dslr,filter,gphoto2,photobooth,picamera2,python,raspberry-pi
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dependency-injector (>=4.41.0,<5.0.0)
-Requires-Dist: fastapi (>=0.95.2,<0.97.0)
-Requires-Dist: gphoto2 (>=2.3.4,<3.0.0) ; sys_platform == "linux"
-Requires-Dist: gpiozero (>=1.6.2,<2.0.0) ; sys_platform == "linux"
-Requires-Dist: jsonref (>=1.1.0,<2.0.0)
-Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
-Requires-Dist: piexif (>=1.1.3,<2.0.0)
-Requires-Dist: pilgram2 (>=2.0.2,<3.0.0)
-Requires-Dist: pillow (>=9.5.0,<10.0.0)
-Requires-Dist: psutil (>=5.9.5,<6.0.0)
-Requires-Dist: pydantic (>=1.10.8,<2.0.0)
-Requires-Dist: pymitter (>=0.4.0,<0.5.0)
-Requires-Dist: pyserial (>=3.5,<4.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: python-statemachine (>=2.0.0,<3.0.0)
-Requires-Dist: pyturbojpeg (>=1.7.1,<2.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: sse-starlette (>=1.6.1,<2.0.0)
-Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
-Requires-Dist: v4l2py (>=0.6.2,<0.7.0) ; sys_platform == "linux"
-Project-URL: Documentation, https://mgrl.github.io/photobooth-docs
-Project-URL: Repository, https://github.com/mgrl/photobooth-app
+Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Multimedia :: Graphics :: Capture :: Digital Camera
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: <3.12,>=3.9
+Requires-Dist: dependency-injector~=4.41.0
+Requires-Dist: fastapi~=0.95.2
+Requires-Dist: gphoto2~=2.3.4; platform_system == 'Linux'
+Requires-Dist: gpiozero~=1.6.2; platform_system == 'Linux'
+Requires-Dist: jsonref~=1.1.0
+Requires-Dist: opencv-python~=4.7.0
+Requires-Dist: piexif~=1.1.3
+Requires-Dist: pilgram2~=2.0.2
+Requires-Dist: pillow~=9.5.0
+Requires-Dist: psutil~=5.9.5
+Requires-Dist: pydantic~=1.10.8
+Requires-Dist: pymitter~=0.4.0
+Requires-Dist: pyserial~=3.5
+Requires-Dist: python-dotenv~=1.0.0
+Requires-Dist: python-statemachine~=2.0.0
+Requires-Dist: pyturbojpeg~=1.7.1
+Requires-Dist: requests~=2.31.0
+Requires-Dist: sse-starlette~=1.6.1
+Requires-Dist: uvicorn~=0.22.0
+Requires-Dist: v4l2py~=0.6.2; platform_system == 'Linux'
 Description-Content-Type: text/markdown
 
-# Photobooth App
+# ![photobooth-app logo](https://raw.githubusercontent.com/mgrl/photobooth-app/main/assets/logo/logo-text-black-transparent.png)
+
+Written in Python 🐍, coming along with a modern Vue frontend.
 
 ![python versions supported 3.9, 3.10, 3.11](https://img.shields.io/pypi/pyversions/photobooth-app)
 ![rpi, linux and windows platform supported](https://img.shields.io/badge/platform-rpi%20%7C%20linux%20%7C%20windows-lightgrey)
 [![ruff](https://github.com/mgrl/photobooth-app/actions/workflows/ruff.yml/badge.svg)](https://github.com/mgrl/photobooth-app/actions/workflows/ruff.yml)
 [![pytest](https://github.com/mgrl/photobooth-app/actions/workflows/pytests.yml/badge.svg)](https://github.com/mgrl/photobooth-app/actions/workflows/pytests.yml)
 [![codecov](https://codecov.io/gh/mgrl/photobooth-app/branch/dev/graph/badge.svg?token=SBB5DGX17V)](https://codecov.io/gh/mgrl/photobooth-app)
 
-The photobooth app is written in Python 🐍 and coming along with a modern Vue frontend.
-
 **[Installation](https://mgrl.github.io/photobooth-docs/installation/)** - **[Documentation](https://mgrl.github.io/photobooth-docs/)** - **[PyPI package](https://pypi.org/project/photobooth-app/)** - **[3d printed box](https://mgrl.github.io/photobooth-docs/photobox3dprint/)**
 
 ## 😍 Features
 
 - 📹 camera live preview with shortest delay as possible, permanent video live view in background
 - ⚡️ optimized for speed, live stream hardware accelerated on rpi, cpu load < 20%
 - 🫶 several camera backends supported for high quality stills and livestream
@@ -94,8 +99,7 @@
 The software is licensed under the MIT license.
 
 ### 🎉 Donation
 
 If you like my work and like to keep me motivated you can sponsor me:
 
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?hosted_button_id=8255Y566TBNEC)
-
```

