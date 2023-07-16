# Comparing `tmp/photobooth_app-0.1.0rc6.tar.gz` & `tmp/photobooth_app-0.1.0rc7.tar.gz`

## Comparing `photobooth_app-0.1.0rc6.tar` & `photobooth_app-0.1.0rc7.tar`

### file list

```diff
@@ -1,139 +1,140 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/__init__.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/__main__.py
--rw-r--r--   0        0        0    17627 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/appconfig.py
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/application.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/containers.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/__init__.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/aquisition.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/config.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/home.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/log.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/mediacollection.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/mediaprocessing.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/processing.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/sse.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/routers/system.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/__init__.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/aquisitionservice.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/baseservice.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/containers.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/gpioservice.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/informationservice.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/keyboardservice.py
--rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/loggingservice.py
--rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/mediacollectionservice.py
--rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/mediaprocessingservice.py
--rw-r--r--   0        0        0     8999 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/processingservice.py
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/systemservice.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/wledservice.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/assets/systemservice/boothupload.service
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/assets/systemservice/boothupload.sh
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/assets/systemservice/photobooth-app.service
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/__init__.py
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/abstractbackend.py
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/containers.py
--rw-r--r--   0        0        0    11212 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/gphoto2.py
--rw-r--r--   0        0        0    16283 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/picamera2.py
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/picamera2_libcamafcontinuous.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/picamera2_libcamafinterval.py
--rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/simulated.py
--rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/webcamcv2.py
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/webcamv4l.py
--rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
--rw-r--r--   0        0        0   710982 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
--rw-r--r--   0        0        0   585221 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
--rw-r--r--   0        0        0   865667 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
--rw-r--r--   0        0        0  2314332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
--rw-r--r--   0        0        0  2126411 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/mediacollection/__init__.py
--rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/mediacollection/mediaitem.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/services/mediaprocessing/image_pipelinestages.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/utils/exceptions.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/utils/fastapi_get_openapi.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/utils/helper.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/utils/repeatedtimer.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/utils/stoppablethread.py
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   168060 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0        0        0   174108 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   167000 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0        0        0   173172 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0        0        0   168644 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0        0        0   173416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0   168488 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0        0        0   172860 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/.gitattributes
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/.gitignore
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/CHANGES.md
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/LICENSE.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/MANIFEST.in
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/Makefile
--rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/README.md
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/make_release.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/setup.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/10_second_macro.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/customizable_hotkey.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/pressed_keys.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/segmented_macro.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/simulate_held_down.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/write.py
--rw-r--r--   0        0        0    46771 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/__main__.py
--rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py
--rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_generic.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py
--rw-r--r--   0        0        0    36792 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_mouse_event.py
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py
--rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py
--rw-r--r--   0        0        0    20549 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py
--rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/mouse.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/index.html
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/css/272.0be6c807.css
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/css/706.28b224d0.css
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/css/835.eb55e979.css
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/css/app.f5a22106.css
--rw-r--r--   0        0        0   208939 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/css/vendor.46e03c42.css
--rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0        0        0    20544 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0        0        0    20424 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0        0        0    20344 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0        0        0   164912 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/icons/favicon-128x128.png
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/icons/logo-notext-black-transparent.png
--rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/icons/logo-text-black-transparent.png
--rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/icons/logo-text-white-transparent.png
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/247.74c0e45d.js
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/272.a73245eb.js
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/391.70a80bd8.js
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/429.76096bfa.js
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/546.92b02def.js
--rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/705.fc48b137.js
--rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/706.1c5cc1da.js
--rw-r--r--   0        0        0     9742 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/835.70f6a199.js
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/862.525f2f13.js
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/863.e0c5ac02.js
--rw-r--r--   0        0        0     7393 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/954.7419ae78.js
--rw-r--r--   0        0        0    12636 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/app.64608eed.js
--rw-r--r--   0        0        0  1417500 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/photobooth/web_spa/js/vendor.c9e02ba9.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/LICENSE.md
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/README.md
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/pyproject.toml
--rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc6/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/__init__.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/__main__.py
+-rw-r--r--   0        0        0    19560 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/appconfig.py
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/application.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/containers.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/__init__.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/aquisition.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/config.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/debug.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/home.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/mediacollection.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/mediaprocessing.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/processing.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/sse.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/routers/system.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/__init__.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/aquisitionservice.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/baseservice.py
+-rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/containers.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/gpioservice.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/informationservice.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/keyboardservice.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/loggingservice.py
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/mediacollectionservice.py
+-rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/mediaprocessingservice.py
+-rw-r--r--   0        0        0     8999 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/processingservice.py
+-rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/shareservice.py
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/systemservice.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/wledservice.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/assets/systemservice/boothupload.service
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/assets/systemservice/boothupload.sh
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/assets/systemservice/photobooth-app.service
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/__init__.py
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/abstractbackend.py
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/containers.py
+-rw-r--r--   0        0        0    11213 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/gphoto2.py
+-rw-r--r--   0        0        0    16283 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/picamera2.py
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/picamera2_libcamafcontinuous.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/picamera2_libcamafinterval.py
+-rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/simulated.py
+-rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/webcamcv2.py
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/webcamv4l.py
+-rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   710982 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
+-rw-r--r--   0        0        0   585221 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
+-rw-r--r--   0        0        0   865667 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
+-rw-r--r--   0        0        0  2314332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
+-rw-r--r--   0        0        0  2126411 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/mediacollection/__init__.py
+-rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/mediacollection/mediaitem.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/services/mediaprocessing/image_pipelinestages.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/utils/exceptions.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/utils/fastapi_get_openapi.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/utils/helper.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/utils/repeatedtimer.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/utils/stoppablethread.py
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   168060 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0        0        0   174108 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   167000 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0        0        0   173172 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0        0        0   168644 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0        0        0   173416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0   168488 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0        0        0   172860 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/.gitattributes
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/.gitignore
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/CHANGES.md
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/LICENSE.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/MANIFEST.in
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/Makefile
+-rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/README.md
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/make_release.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/setup.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/10_second_macro.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/customizable_hotkey.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/pressed_keys.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/segmented_macro.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/simulate_held_down.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/write.py
+-rw-r--r--   0        0        0    46771 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/__main__.py
+-rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py
+-rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_generic.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py
+-rw-r--r--   0        0        0    36792 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_mouse_event.py
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py
+-rw-r--r--   0        0        0    20549 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/mouse.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/index.html
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/css/272.0be6c807.css
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/css/706.5484da7d.css
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/css/835.ded66ce0.css
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/css/app.f5a22106.css
+-rw-r--r--   0        0        0   208939 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/css/vendor.46e03c42.css
+-rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0        0        0    20544 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0        0        0    20424 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0        0        0    20344 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0        0        0   164912 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/icons/favicon-128x128.png
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/icons/logo-notext-black-transparent.png
+-rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/icons/logo-text-black-transparent.png
+-rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/icons/logo-text-white-transparent.png
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/247.74c0e45d.js
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/272.a73245eb.js
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/429.76096bfa.js
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/546.92b02def.js
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/705.fc48b137.js
+-rw-r--r--   0        0        0     9058 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/706.98593961.js
+-rw-r--r--   0        0        0     9654 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/835.8e1bdcfb.js
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/862.525f2f13.js
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/863.e0c5ac02.js
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/931.55b1be58.js
+-rw-r--r--   0        0        0     7393 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/954.7419ae78.js
+-rw-r--r--   0        0        0    12636 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/app.979a8c9e.js
+-rw-r--r--   0        0        0  1417500 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/photobooth/web_spa/js/vendor.c9e02ba9.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/LICENSE.md
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/README.md
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/pyproject.toml
+-rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc7/PKG-INFO
```

### Comparing `photobooth_app-0.1.0rc6/photobooth/__main__.py` & `photobooth_app-0.1.0rc7/photobooth/__main__.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/application.py` & `photobooth_app-0.1.0rc7/photobooth/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from fastapi.exceptions import HTTPException, RequestValidationError
 from fastapi.staticfiles import StaticFiles
 
 # from .routers import home, config, mediacollection
 from .containers import ApplicationContainer
 from .routers.aquisition import aquisition_router
 from .routers.config import config_router
+from .routers.debug import debug_router
 from .routers.home import home_router
-from .routers.log import log_router
 from .routers.mediacollection import mediacollection_router
 from .routers.mediaprocessing import mediaprocessing_router
 from .routers.processing import processing_router
 from .routers.sse import sse_router
 from .routers.system import system_router
 
 FASTAPI_DECRIPTION = """
@@ -65,15 +65,15 @@
         redoc_url=None,
         openapi_url="/api/openapi.json",
     )
 
     _app.include_router(config_router)
     _app.include_router(home_router)
     _app.include_router(aquisition_router)
-    _app.include_router(log_router)
+    _app.include_router(debug_router)
     _app.include_router(mediacollection_router)
     _app.include_router(mediaprocessing_router)
     _app.include_router(sse_router)
     _app.include_router(system_router)
     _app.include_router(processing_router)
     # serve data directory holding images, thumbnails, ...
     _app.mount("/data", StaticFiles(directory="data"), name="data")
```

### Comparing `photobooth_app-0.1.0rc6/photobooth/containers.py` & `photobooth_app-0.1.0rc7/photobooth/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/routers/aquisition.py` & `photobooth_app-0.1.0rc7/photobooth/routers/aquisition.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/routers/config.py` & `photobooth_app-0.1.0rc7/photobooth/routers/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     """returns currently cached and active settings"""
     return config
 
 
 @config_router.get("/current")
 def api_get_config_current():
     """read settings from drive and return"""
-    return AppConfig().dict()
+    return AppConfig().model_dump()
 
 
 @config_router.post("/current")
 @inject
 def api_post_config_current(
     updated_config: AppConfig,
     # appcontainer: ApplicationContainer = Depends(Provide[ApplicationContainer]),
```

### Comparing `photobooth_app-0.1.0rc6/photobooth/routers/home.py` & `photobooth_app-0.1.0rc7/photobooth/routers/home.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/routers/mediacollection.py` & `photobooth_app-0.1.0rc7/photobooth/routers/mediacollection.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/routers/mediaprocessing.py` & `photobooth_app-0.1.0rc7/photobooth/routers/mediaprocessing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,27 @@
 import io
 import logging
 
 from dependency_injector.wiring import Provide, inject
 from fastapi import APIRouter, Depends, HTTPException, Response, status
 from PIL import Image
 
-from ..appconfig import EnumPilgramFilter
 from ..containers import ApplicationContainer
 from ..services.mediacollectionservice import MediacollectionService
 from ..services.mediaprocessing.image_pipelinestages import pilgram_stage
 from ..services.mediaprocessingservice import MediaprocessingService
 from ..utils.exceptions import PipelineError
 
 logger = logging.getLogger(__name__)
 mediaprocessing_router = APIRouter(
     prefix="/mediaprocessing",
     tags=["mediaprocessing"],
 )
 
 
-@mediaprocessing_router.get("/list/filter")
-@inject
-def api_get_list_filteravail(
-    mediacollection_service: MediacollectionService = Depends(
-        Provide[ApplicationContainer.services.mediacollection_service]
-    ),
-):
-    return [e.value for e in EnumPilgramFilter]
-
-
 @mediaprocessing_router.get("/preview/{mediaitem_id}/{filter}", response_class=Response)
 @inject
 def api_get_preview_image_filtered(
     mediaitem_id,
     filter=None,
     mediacollection_service: MediacollectionService = Depends(
         Provide[ApplicationContainer.services.mediacollection_service]
```

### Comparing `photobooth_app-0.1.0rc6/photobooth/routers/processing.py` & `photobooth_app-0.1.0rc7/photobooth/routers/processing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/routers/sse.py` & `photobooth_app-0.1.0rc7/photobooth/routers/sse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/routers/system.py` & `photobooth_app-0.1.0rc7/photobooth/routers/system.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/aquisitionservice.py` & `photobooth_app-0.1.0rc7/photobooth/services/aquisitionservice.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,22 +74,26 @@
         """start backends"""
         if self.primary_backend:
             self.primary_backend.start()
 
         if self.secondary_backend:
             self.secondary_backend.start()
 
+        super().set_status_started()
+
     def stop(self):
         """stop backends"""
         if self.primary_backend:
             self.primary_backend.stop()
 
         if self.secondary_backend:
             self.secondary_backend.stop()
 
+        super().set_status_stopped()
+
     def stats(self):
         """
         Gather stats from active backends.
         Backend stats are converted to dict to be processable by JSON lib
 
         Returns:
             _type_: _description_
```

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/containers.py` & `photobooth_app-0.1.0rc7/photobooth/services/containers.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .aquisitionservice import AquisitionService
 from .gpioservice import GpioService
 from .informationservice import InformationService
 from .keyboardservice import KeyboardService
 from .mediacollectionservice import MediacollectionService
 from .mediaprocessingservice import MediaprocessingService
 from .processingservice import ProcessingService
+from .shareservice import ShareService
 from .systemservice import SystemService
 from .wledservice import WledService
 
 logger = logging.getLogger(__name__)
 
 
 def init_aquisition_resource(evtbus, config, primary, secondary):
@@ -64,14 +65,21 @@
 def init_gpio_resource(evtbus, config, processing_service):
     resource = GpioService(evtbus=evtbus, config=config, processing_service=processing_service)
     resource.start()
     yield resource
     resource.stop()
 
 
+def init_share_resource(evtbus, config, mediacollection_service):
+    resource = ShareService(evtbus=evtbus, config=config, mediacollection_service=mediacollection_service)
+    resource.start()
+    yield resource
+    resource.stop()
+
+
 class ServicesContainer(containers.DeclarativeContainer):
     evtbus = providers.Dependency(instance_of=EventEmitter)
     config = providers.Dependency(instance_of=AppConfig)
     backends = providers.DependenciesContainer()
 
     # Services: Core
 
@@ -122,7 +130,14 @@
 
     gpio_service = providers.Resource(
         init_gpio_resource,
         evtbus=evtbus,
         config=config,
         processing_service=processing_service,
     )
+
+    share_service = providers.Resource(
+        init_share_resource,
+        evtbus=evtbus,
+        config=config,
+        mediacollection_service=mediacollection_service,
+    )
```

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/gpioservice.py` & `photobooth_app-0.1.0rc7/photobooth/services/gpioservice.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,18 +61,18 @@
         self.take1pic_btn: Button = Button(
             self._config.hardwareinputoutput.gpio_pin_take1pic, bounce_time=DEBOUNCE_TIME
         )
 
         self._register_listener()
 
     def start(self):
-        pass
+        super().set_status_started()
 
     def stop(self):
-        pass
+        super().set_status_stopped()
 
     def _shutdown(self):
         self._logger.info("trigger _shutdown")
         subprocess.check_call(["poweroff"])
 
     def _reboot(self):
         self._logger.info("trigger _reboot")
@@ -91,16 +91,14 @@
             self._logger.critical(exc)
 
     def _register_listener(self):
         self._register_listener_inputs()
         self._register_listener_outputs()
 
     def _register_listener_inputs(self):
-        self._logger.warning(f"{self.shutdown_btn=}")
-
         # shutdown
         self.shutdown_btn.when_held = self._shutdown
         # reboot
         self.reboot_btn.when_held = self._reboot
         # takepic
         self.take1pic_btn.when_pressed = self._take1pic
```

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/informationservice.py` & `photobooth_app-0.1.0rc7/photobooth/services/informationservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/keyboardservice.py` & `photobooth_app-0.1.0rc7/photobooth/services/keyboardservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/loggingservice.py` & `photobooth_app-0.1.0rc7/photobooth/services/loggingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/mediacollectionservice.py` & `photobooth_app-0.1.0rc7/photobooth/services/mediacollectionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/mediaprocessingservice.py` & `photobooth_app-0.1.0rc7/photobooth/services/mediaprocessingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/processingservice.py` & `photobooth_app-0.1.0rc7/photobooth/services/processingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/systemservice.py` & `photobooth_app-0.1.0rc7/photobooth/services/systemservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/wledservice.py` & `photobooth_app-0.1.0rc7/photobooth/services/wledservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/assets/systemservice/photobooth-app.service` & `photobooth_app-0.1.0rc7/photobooth/services/assets/systemservice/photobooth-app.service`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/backends/abstractbackend.py` & `photobooth_app-0.1.0rc7/photobooth/services/backends/abstractbackend.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/backends/containers.py` & `photobooth_app-0.1.0rc7/photobooth/services/backends/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/backends/gphoto2.py` & `photobooth_app-0.1.0rc7/photobooth/services/backends/gphoto2.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,14 +306,15 @@
         logger.warning("_generate_images_fun exits")
 
 
 def available_camera_indexes():
     """
     find available cameras, return valid indexes.
     """
+
     camera_list = gp.Camera.autodetect()
     if len(camera_list) == 0:
         logger.info("no camera detected")
         return []
 
     available_indexes = []
     for index, (name, addr) in enumerate(camera_list):
```

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/backends/picamera2.py` & `photobooth_app-0.1.0rc7/photobooth/services/backends/picamera2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/backends/picamera2_libcamafcontinuous.py` & `photobooth_app-0.1.0rc7/photobooth/services/backends/picamera2_libcamafcontinuous.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/backends/picamera2_libcamafinterval.py` & `photobooth_app-0.1.0rc7/photobooth/services/backends/picamera2_libcamafinterval.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/backends/simulated.py` & `photobooth_app-0.1.0rc7/photobooth/services/backends/simulated.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/backends/webcamcv2.py` & `photobooth_app-0.1.0rc7/photobooth/services/backends/webcamcv2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/backends/webcamv4l.py` & `photobooth_app-0.1.0rc7/photobooth/services/backends/webcamv4l.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg` & `photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt` & `photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf` & `photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg` & `photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg` & `photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg` & `photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg` & `photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg` & `photobooth_app-0.1.0rc7/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/mediacollection/mediaitem.py` & `photobooth_app-0.1.0rc7/photobooth/services/mediacollection/mediaitem.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import logging
 import os
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
 
+from ...appconfig import AppConfig
+
 logger = logging.getLogger(__name__)
 
 DATA_PATH = "./data/"
 # as from image source
 PATH_ORIGINAL = "".join([DATA_PATH, "original/"])
 # represents unaltered data from image source in S/M/L
 PATH_UNPROCESSED = "".join([DATA_PATH, "unprocessed/"])
@@ -149,14 +151,22 @@
 
     @property
     def thumbnail(self) -> str:
         """filepath of media item thumbnail resolution scaled represents full
         external use as urls"""
         return Path(PATH_THUMBNAIL, self.filename).as_posix()
 
+    @property
+    def share_url(self) -> str:
+        """share url for example to use in qr code"""
+
+        # exception here for now to use appconfig like this not via container - maybe find better solution in future.
+        # config changes are not reflected like this, always needs restart
+        return f"{AppConfig().common.shareservice_url}?action=download&id={self.id}"
+
     def __post_init__(self):
         if not self.filename:
             raise ValueError("Filename must be given")
 
         # if filename has no information about type and visibility: raise Exception
         if not (len(split_filename(self.filename)) == 3):
             raise ValueError(f"the original_file {self.filename} is not a valid filename - ignored")
```

### Comparing `photobooth_app-0.1.0rc6/photobooth/services/mediaprocessing/image_pipelinestages.py` & `photobooth_app-0.1.0rc7/photobooth/services/mediaprocessing/image_pipelinestages.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/utils/repeatedtimer.py` & `photobooth_app-0.1.0rc7/photobooth/utils/repeatedtimer.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/utils/stoppablethread.py` & `photobooth_app-0.1.0rc7/photobooth/utils/stoppablethread.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/LICENSE.txt` & `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf` & `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf` & `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf` & `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf` & `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf` & `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf` & `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf` & `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf` & `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf` & `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf` & `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf` & `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf` & `photobooth_app-0.1.0rc7/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/.gitignore` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/.gitignore`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/CHANGES.md` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/CHANGES.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/LICENSE.txt` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/Makefile` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/Makefile`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/README.md` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/README.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/make_release.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/make_release.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/setup.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/setup.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/segmented_macro.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/segmented_macro.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/__init__.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_generic.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_generic.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/vendor/packages/keyboard/keyboard/mouse.py` & `photobooth_app-0.1.0rc7/photobooth/vendor/packages/keyboard/keyboard/mouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/index.html` & `photobooth_app-0.1.0rc7/photobooth/web_spa/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>qPhotobooth</title><meta charset=utf-8><meta name=description content=qPhotobooth><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><script defer src=js/vendor.c9e02ba9.js></script><script defer src=js/app.64608eed.js></script><link href=css/vendor.46e03c42.css rel=stylesheet><link href=css/app.f5a22106.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>qPhotobooth</title><meta charset=utf-8><meta name=description content=qPhotobooth><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><script defer src=js/vendor.c9e02ba9.js></script><script defer src=js/app.979a8c9e.js></script><link href=css/vendor.46e03c42.css rel=stylesheet><link href=css/app.f5a22106.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/css/vendor.46e03c42.css` & `photobooth_app-0.1.0rc7/photobooth/web_spa/css/vendor.46e03c42.css`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `photobooth_app-0.1.0rc7/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/icons/favicon-128x128.png` & `photobooth_app-0.1.0rc7/photobooth/web_spa/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/icons/logo-notext-black-transparent.png` & `photobooth_app-0.1.0rc7/photobooth/web_spa/icons/logo-notext-black-transparent.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/icons/logo-text-black-transparent.png` & `photobooth_app-0.1.0rc7/photobooth/web_spa/icons/logo-text-black-transparent.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/icons/logo-text-white-transparent.png` & `photobooth_app-0.1.0rc7/photobooth/web_spa/icons/logo-text-white-transparent.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/js/247.74c0e45d.js` & `photobooth_app-0.1.0rc7/photobooth/web_spa/js/247.74c0e45d.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/js/272.a73245eb.js` & `photobooth_app-0.1.0rc7/photobooth/web_spa/js/272.a73245eb.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/js/391.70a80bd8.js` & `photobooth_app-0.1.0rc7/photobooth/web_spa/js/931.55b1be58.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (globalThis["webpackChunkqPhotobooth"] = globalThis["webpackChunkqPhotobooth"] || []).push([
-    [391], {
-        6391: (t, e, l) => {
+    [931], {
+        2931: (t, e, l) => {
             l.r(e), l.d(e, {
                 default: () => C
             });
             var o = l(9835),
                 a = l(6970);
             const n = {
                     class: "row col-xs-12 col-sm-4 col-md-3 col-lg-3"
@@ -31,16 +31,16 @@
                 }, "Message")])], -1);
 
             function m(t, e, l, m, c, _) {
                 const w = (0, o.up)("q-card-section"),
                     f = (0, o.up)("q-card"),
                     h = (0, o.up)("QBtn"),
                     p = (0, o.up)("q-markup-table"),
-                    v = (0, o.up)("q-page");
-                return (0, o.wg)(), (0, o.j4)(v, {
+                    g = (0, o.up)("q-page");
+                return (0, o.wg)(), (0, o.j4)(g, {
                     padding: ""
                 }, {
                     default: (0, o.w5)((() => [(0, o._)("div", n, [(0, o.Wm)(f, {
                         style: {},
                         class: "q-pa-md q-ma-md"
                     }, {
                         default: (0, o.w5)((() => [(0, o.Wm)(w, null, {
@@ -48,15 +48,15 @@
                             _: 1
                         })])),
                         _: 1
                     })]), (0, o.Wm)(f, {
                         class: "q-pa-md q-mt-md"
                     }, {
                         default: (0, o.w5)((() => [(0, o._)("div", s, [d, (0, o.Wm)(h, {
-                            href: "/log/latest",
+                            href: "/debug/log/latest",
                             target: "_blank"
                         }, {
                             default: (0, o.w5)((() => [(0, o.Uk)("download log")])),
                             _: 1
                         })]), (0, o.Wm)(p, null, {
                             default: (0, o.w5)((() => [u, (0, o._)("tbody", null, [((0, o.wg)(!0), (0, o.iD)(o.HY, null, (0, o.Ko)(this.store.logrecords, ((t, e) => ((0, o.wg)(), (0, o.iD)("tr", {
                                 key: e
@@ -82,27 +82,27 @@
                         store: t,
                         remoteProcedureCall: _.remoteProcedureCall
                     }
                 }
             });
             var h = l(1639),
                 p = l(9885),
-                v = l(4458),
-                g = l(3190),
+                g = l(4458),
+                v = l(3190),
                 z = l(990),
                 b = l(6933),
                 q = l(9984),
                 k = l.n(q);
             const x = (0, h.Z)(f, [
                     ["render", m]
                 ]),
                 C = x;
             k()(f, "components", {
                 QPage: p.Z,
-                QCard: v.Z,
-                QCardSection: g.Z,
+                QCard: g.Z,
+                QCardSection: v.Z,
                 QBadge: z.Z,
                 QMarkupTable: b.Z
             })
         }
     }
 ]);
```

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/js/429.76096bfa.js` & `photobooth_app-0.1.0rc7/photobooth/web_spa/js/429.76096bfa.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/js/546.92b02def.js` & `photobooth_app-0.1.0rc7/photobooth/web_spa/js/546.92b02def.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/js/705.fc48b137.js` & `photobooth_app-0.1.0rc7/photobooth/web_spa/js/705.fc48b137.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/js/706.1c5cc1da.js` & `photobooth_app-0.1.0rc7/photobooth/web_spa/js/706.98593961.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (globalThis["webpackChunkqPhotobooth"] = globalThis["webpackChunkqPhotobooth"] || []).push([
     [706], {
-        9815: (e, t, i) => {
+        9683: (e, t, i) => {
             i.d(t, {
                 Z: () => W
             });
             var r = i(9835),
                 a = i(6970);
             const l = {
                     class: "q-mr-sm"
@@ -28,16 +28,16 @@
                     S = (0, r.up)("q-linear-progress"),
                     w = (0, r.up)("q-header"),
                     y = (0, r.up)("q-img"),
                     I = (0, r.up)("q-drawer"),
                     v = (0, r.up)("q-carousel-slide"),
                     f = (0, r.up)("q-carousel"),
                     b = (0, r.up)("vue-qrcode"),
-                    _ = (0, r.up)("q-page-sticky"),
-                    q = (0, r.up)("q-page-container"),
+                    q = (0, r.up)("q-page-sticky"),
+                    _ = (0, r.up)("q-page-container"),
                     k = (0, r.up)("q-layout"),
                     T = (0, r.Q2)("close-popup"),
                     R = (0, r.Q2)("touch-swipe");
                 return (0, r.wg)(), (0, r.j4)(k, {
                     view: "hhh Lpr ffr",
                     onClick: u.abortTimer
                 }, {
@@ -109,15 +109,15 @@
                             key: e,
                             onClick: t => u.applyFilter(d.currentSlideId, e)
                         }, {
                             default: (0, r.w5)((() => [(0, r._)("div", o, (0, a.zw)(e), 1)])),
                             _: 2
                         }, 1032, ["src", "onClick"])))), 128))])),
                         _: 1
-                    }, 8, ["modelValue"])) : (0, r.kq)("", !0), (0, r.Wm)(q, {
+                    }, 8, ["modelValue"])) : (0, r.kq)("", !0), (0, r.Wm)(_, {
                         class: "q-pa-none galleryimagedetail full-height"
                     }, {
                         default: (0, r.w5)((() => [(0, r.wy)(((0, r.wg)(), (0, r.j4)(f, {
                             class: "bg-image",
                             style: {
                                 width: "100%",
                                 height: "100%"
@@ -145,15 +145,15 @@
                             }, null, 8, ["img-src", "name"])))), 128))])),
                             _: 1
                         }, 8, ["modelValue", "autoplay"])), [
                             [R, d.handleSwipeDown, void 0, {
                                 mouse: !0,
                                 down: !0
                             }]
-                        ]), (0, r.Wm)(_, {
+                        ]), (0, r.Wm)(q, {
                             position: "top-right",
                             offset: [30, 30]
                         }, {
                             default: (0, r.w5)((() => [(0, r._)("div", s, [(0, r.Wm)(b, {
                                 type: "image/png",
                                 tag: "svg",
                                 margin: 2,
@@ -264,16 +264,15 @@
                             console.log(e), this.itemRepository.splice(this.currentSlideIndex, 1)
                         })).catch((e => console.log(e)))
                     },
                     getImageDetail(e, t = "thumbnail") {
                         return this.itemRepository[e][t]
                     },
                     getImageQrData() {
-                        const e = String(this.uiSettingsStore.uiSettings.EXT_DOWNLOAD_URL).replace("{filename}", this.itemRepository[this.currentSlideIndex]["filename"]);
-                        return e
+                        return this.itemRepository[this.currentSlideIndex]["share_url"]
                     },
                     abortTimer() {
                         clearInterval(this.intervalTimerId), this.remainingSeconds = 0, this.remainingSecondsNormalized = 0
                     },
                     startTimer() {
                         var e = this.uiSettingsStore.uiSettings["AUTOCLOSE_NEW_ITEM_ARRIVED"];
                         console.log(`starting newitemarrived timer, duration=${e}`), this.remainingSeconds = e, this.intervalTimerId = setInterval((() => {
@@ -288,39 +287,39 @@
                 S = i(7605),
                 w = i(6602),
                 y = i(1663),
                 I = i(8879),
                 v = i(136),
                 f = i(2857),
                 b = i(8289),
-                _ = i(906),
-                q = i(335),
+                q = i(906),
+                _ = i(335),
                 k = i(2133),
                 T = i(7052),
                 R = i(1694),
                 D = i(627),
                 Z = i(2146),
                 x = i(4871),
                 Q = i(9984),
                 C = i.n(Q);
             const E = (0, p.Z)(h, [
                     ["render", d],
-                    ["__scopeId", "data-v-3e1a07b8"]
+                    ["__scopeId", "data-v-2ceef1d0"]
                 ]),
                 W = E;
             C()(h, "components", {
                 QLayout: S.Z,
                 QHeader: w.Z,
                 QToolbar: y.Z,
                 QBtn: I.Z,
                 QSpace: v.Z,
                 QIcon: f.Z,
                 QLinearProgress: b.Z,
-                QDrawer: _.Z,
-                QImg: q.Z,
+                QDrawer: q.Z,
+                QImg: _.Z,
                 QPageContainer: k.Z,
                 QCarousel: T.Z,
                 QCarouselSlide: R.Z,
                 QPageSticky: D.Z
             }), C()(h, "directives", {
                 ClosePopup: Z.Z,
                 TouchSwipe: x.Z
@@ -361,15 +360,15 @@
                     }, 8, ["modelValue"])])),
                     _: 1
                 }, 8, ["onClick"])
             }
             i(9665);
             var l = i(7575),
                 n = i(6694),
-                o = i(9815);
+                o = i(9683);
             const s = {
                 components: {
                     GalleryImageDetail: o.Z
                 },
                 data() {
                     return {
                         intervalTimerId: null,
```

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/js/835.70f6a199.js` & `photobooth_app-0.1.0rc7/photobooth/web_spa/js/835.8e1bdcfb.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (globalThis["webpackChunkqPhotobooth"] = globalThis["webpackChunkqPhotobooth"] || []).push([
     [835], {
-        9815: (e, t, i) => {
+        9683: (e, t, i) => {
             i.d(t, {
-                Z: () => W
+                Z: () => $
             });
             var l = i(9835),
                 r = i(6970);
             const a = {
                     class: "q-mr-sm"
                 },
                 o = {
@@ -31,40 +31,40 @@
                     I = (0, l.up)("q-drawer"),
                     f = (0, l.up)("q-carousel-slide"),
                     v = (0, l.up)("q-carousel"),
                     b = (0, l.up)("vue-qrcode"),
                     _ = (0, l.up)("q-page-sticky"),
                     q = (0, l.up)("q-page-container"),
                     k = (0, l.up)("q-layout"),
-                    D = (0, l.Q2)("close-popup"),
-                    x = (0, l.Q2)("touch-swipe");
+                    x = (0, l.Q2)("close-popup"),
+                    D = (0, l.Q2)("touch-swipe");
                 return (0, l.wg)(), (0, l.j4)(k, {
                     view: "hhh Lpr ffr",
                     onClick: c.abortTimer
                 }, {
                     default: (0, l.w5)((() => [(0, l.Wm)(w, {
                         elevated: "",
                         class: "bg-primary text-white"
                     }, {
                         default: (0, l.w5)((() => [(0, l.Wm)(p, null, {
                             default: (0, l.w5)((() => [(0, l.wy)((0, l.Wm)(m, {
                                 dense: "",
                                 flat: "",
                                 icon: "close"
                             }, null, 512), [
-                                [D]
+                                [x]
                             ]), (0, l.Wm)(u), d.uiSettingsStore.uiSettings.gallery_show_delete ? (0, l.wy)(((0, l.wg)(), (0, l.j4)(m, {
                                 key: 0,
                                 flat: "",
                                 class: "q-mr-sm",
                                 icon: "delete",
                                 label: "Delete",
                                 onClick: t[0] || (t[0] = e => c.deleteImage(d.currentSlideId))
                             }, null, 512)), [
-                                [D]
+                                [x]
                             ]) : (0, l.kq)("", !0), d.uiSettingsStore.uiSettings.gallery_show_download ? ((0, l.wg)(), (0, l.j4)(m, {
                                 key: 1,
                                 flat: "",
                                 class: "q-mr-sm",
                                 icon: "download",
                                 label: "Download",
                                 onClick: t[1] || (t[1] = e => {
@@ -141,15 +141,15 @@
                             default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(c.slicedImages, (e => ((0, l.wg)(), (0, l.j4)(f, {
                                 "img-src": e.preview,
                                 key: e.id,
                                 name: e.id
                             }, null, 8, ["img-src", "name"])))), 128))])),
                             _: 1
                         }, 8, ["modelValue", "autoplay"])), [
-                            [x, d.handleSwipeDown, void 0, {
+                            [D, d.handleSwipeDown, void 0, {
                                 mouse: !0,
                                 down: !0
                             }]
                         ]), (0, l.Wm)(_, {
                             position: "top-right",
                             offset: [30, 30]
                         }, {
@@ -264,16 +264,15 @@
                             console.log(e), this.itemRepository.splice(this.currentSlideIndex, 1)
                         })).catch((e => console.log(e)))
                     },
                     getImageDetail(e, t = "thumbnail") {
                         return this.itemRepository[e][t]
                     },
                     getImageQrData() {
-                        const e = String(this.uiSettingsStore.uiSettings.EXT_DOWNLOAD_URL).replace("{filename}", this.itemRepository[this.currentSlideIndex]["filename"]);
-                        return e
+                        return this.itemRepository[this.currentSlideIndex]["share_url"]
                     },
                     abortTimer() {
                         clearInterval(this.intervalTimerId), this.remainingSeconds = 0, this.remainingSecondsNormalized = 0
                     },
                     startTimer() {
                         var e = this.uiSettingsStore.uiSettings["AUTOCLOSE_NEW_ITEM_ARRIVED"];
                         console.log(`starting newitemarrived timer, duration=${e}`), this.remainingSeconds = e, this.intervalTimerId = setInterval((() => {
@@ -291,41 +290,41 @@
                 I = i(8879),
                 f = i(136),
                 v = i(2857),
                 b = i(8289),
                 _ = i(906),
                 q = i(335),
                 k = i(2133),
-                D = i(7052),
-                x = i(1694),
+                x = i(7052),
+                D = i(1694),
                 Z = i(627),
                 R = i(2146),
                 Q = i(4871),
-                T = i(9984),
-                C = i.n(T);
+                C = i(9984),
+                T = i.n(C);
             const j = (0, p.Z)(h, [
                     ["render", d],
-                    ["__scopeId", "data-v-3e1a07b8"]
+                    ["__scopeId", "data-v-2ceef1d0"]
                 ]),
-                W = j;
-            C()(h, "components", {
+                $ = j;
+            T()(h, "components", {
                 QLayout: y.Z,
                 QHeader: w.Z,
                 QToolbar: S.Z,
                 QBtn: I.Z,
                 QSpace: f.Z,
                 QIcon: v.Z,
                 QLinearProgress: b.Z,
                 QDrawer: _.Z,
                 QImg: q.Z,
                 QPageContainer: k.Z,
-                QCarousel: D.Z,
-                QCarouselSlide: x.Z,
+                QCarousel: x.Z,
+                QCarouselSlide: D.Z,
                 QPageSticky: Z.Z
-            }), C()(h, "directives", {
+            }), T()(h, "directives", {
                 ClosePopup: R.Z,
                 TouchSwipe: Q.Z
             })
         },
         3835: (e, t, i) => {
             i.r(t), i.d(t, {
                 default: () => v
@@ -386,15 +385,15 @@
                         _: 1
                     }, 8, ["modelValue"])])),
                     _: 1
                 })
             }
             var s = i(7575),
                 d = i(499),
-                g = i(9815);
+                g = i(9683);
             const c = {
                 components: {
                     GalleryImageDetail: g.Z
                 },
                 setup() {
                     const e = (0, s.h)();
                     return {
```

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/js/862.525f2f13.js` & `photobooth_app-0.1.0rc7/photobooth/web_spa/js/862.525f2f13.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/js/863.e0c5ac02.js` & `photobooth_app-0.1.0rc7/photobooth/web_spa/js/863.e0c5ac02.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/js/954.7419ae78.js` & `photobooth_app-0.1.0rc7/photobooth/web_spa/js/954.7419ae78.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/js/app.64608eed.js` & `photobooth_app-0.1.0rc7/photobooth/web_spa/js/app.979a8c9e.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -201,15 +201,15 @@
                             path: "",
                             component: () => Promise.all([o.e(736), o.e(954)]).then(o.bind(o, 5954))
                         }, {
                             path: "gallery",
                             component: () => Promise.all([o.e(736), o.e(835)]).then(o.bind(o, 3835))
                         }, {
                             path: "status",
-                            component: () => Promise.all([o.e(736), o.e(391)]).then(o.bind(o, 6391))
+                            component: () => Promise.all([o.e(736), o.e(931)]).then(o.bind(o, 2931))
                         }, {
                             path: "help",
                             component: () => Promise.all([o.e(736), o.e(429)]).then(o.bind(o, 6429))
                         }, {
                             path: "playground",
                             component: () => Promise.all([o.e(736), o.e(863)]).then(o.bind(o, 2863))
                         }, {
@@ -523,29 +523,29 @@
         }
     })(), (() => {
         o.f = {}, o.e = e => Promise.all(Object.keys(o.f).reduce(((t, n) => (o.f[n](e, t), t)), []))
     })(), (() => {
         o.u = e => "js/" + e + "." + {
             247: "74c0e45d",
             272: "a73245eb",
-            391: "70a80bd8",
             429: "76096bfa",
             546: "92b02def",
             705: "fc48b137",
-            706: "1c5cc1da",
-            835: "70f6a199",
+            706: "98593961",
+            835: "8e1bdcfb",
             862: "525f2f13",
             863: "e0c5ac02",
+            931: "55b1be58",
             954: "7419ae78"
         } [e] + ".js"
     })(), (() => {
         o.miniCssF = e => "css/" + e + "." + {
             272: "0be6c807",
-            706: "28b224d0",
-            835: "eb55e979"
+            706: "5484da7d",
+            835: "ded66ce0"
         } [e] + ".css"
     })(), (() => {
         o.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
             } catch (e) {
```

### Comparing `photobooth_app-0.1.0rc6/photobooth/web_spa/js/vendor.c9e02ba9.js` & `photobooth_app-0.1.0rc7/photobooth/web_spa/js/vendor.c9e02ba9.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/LICENSE.md` & `photobooth_app-0.1.0rc7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/README.md` & `photobooth_app-0.1.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc6/pyproject.toml` & `photobooth_app-0.1.0rc7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2270 686f 746f 626f 6f74 682d 6170  = "photobooth-ap
 00000020: 7022 0d0a 7265 7175 6972 6573 2d70 7974  p"..requires-pyt
 00000030: 686f 6e20 3d20 223e 3d33 2e39 2c3c 332e  hon = ">=3.9,<3.
 00000040: 3132 220d 0a76 6572 7369 6f6e 203d 2022  12"..version = "
-00000050: 302e 312e 3072 6336 220d 0a64 6573 6372  0.1.0rc6"..descr
+00000050: 302e 312e 3072 6337 220d 0a64 6573 6372  0.1.0rc7"..descr
 00000060: 6970 7469 6f6e 203d 2022 5068 6f74 6f62  iption = "Photob
 00000070: 6f6f 7468 2061 7070 2077 7269 7474 656e  ooth app written
 00000080: 2069 6e20 5079 7468 6f6e 2073 7570 706f   in Python suppo
 00000090: 7274 696e 6720 4453 4c52 2c20 7069 6361  rting DSLR, pica
 000000a0: 6d65 7261 322c 2077 6562 6361 6d65 7261  mera2, webcamera
 000000b0: 7322 0d0a 6175 7468 6f72 7320 3d20 5b7b  s"..authors = [{
 000000c0: 206e 616d 6520 3d20 224d 6963 6861 656c   name = "Michael
@@ -55,153 +55,158 @@
 00000360: 6922 2c0d 0a20 2022 6361 6d65 7261 222c  i",..  "camera",
 00000370: 0d0a 2020 2270 7974 686f 6e22 2c0d 0a20  ..  "python",.. 
 00000380: 2022 6669 6c74 6572 222c 0d0a 2020 2267   "filter",..  "g
 00000390: 7068 6f74 6f32 222c 0d0a 2020 2264 736c  photo2",..  "dsl
 000003a0: 7222 2c0d 0a20 2022 7069 6361 6d65 7261  r",..  "picamera
 000003b0: 3222 0d0a 5d0d 0a0d 0a64 6570 656e 6465  2"..]....depende
 000003c0: 6e63 6965 733d 205b 0d0a 2022 6661 7374  ncies= [.. "fast
-000003d0: 6170 693e 3d30 2e39 352e 322c 3c30 2e39  api>=0.95.2,<0.9
-000003e0: 372e 3022 2c0d 0a20 226f 7065 6e63 762d  7.0",.. "opencv-
-000003f0: 7079 7468 6f6e 7e3d 342e 372e 3022 2c0d  python~=4.7.0",.
-00000400: 0a20 2270 6965 7869 667e 3d31 2e31 2e33  . "piexif~=1.1.3
-00000410: 222c 0d0a 2022 7069 6c6c 6f77 7e3d 392e  ",.. "pillow~=9.
-00000420: 352e 3022 2c0d 0a20 2270 7375 7469 6c7e  5.0",.. "psutil~
-00000430: 3d35 2e39 2e35 222c 0d0a 2022 7079 6461  =5.9.5",.. "pyda
-00000440: 6e74 6963 7e3d 312e 3130 2e38 222c 0d0a  ntic~=1.10.8",..
-00000450: 2022 7079 6d69 7474 6572 7e3d 302e 342e   "pymitter~=0.4.
-00000460: 3022 2c0d 0a20 2270 7974 7572 626f 6a70  0",.. "pyturbojp
-00000470: 6567 7e3d 312e 372e 3122 2c0d 0a20 2272  eg~=1.7.1",.. "r
-00000480: 6571 7565 7374 737e 3d32 2e33 312e 3022  equests~=2.31.0"
-00000490: 2c0d 0a20 2273 7365 2d73 7461 726c 6574  ,.. "sse-starlet
-000004a0: 7465 7e3d 312e 362e 3122 2c0d 0a20 2275  te~=1.6.1",.. "u
-000004b0: 7669 636f 726e 7e3d 302e 3232 2e30 222c  vicorn~=0.22.0",
-000004c0: 0d0a 2022 7079 7468 6f6e 2d64 6f74 656e  .. "python-doten
-000004d0: 767e 3d31 2e30 2e30 222c 0d0a 2022 7079  v~=1.0.0",.. "py
-000004e0: 7365 7269 616c 7e3d 332e 3522 2c0d 0a20  serial~=3.5",.. 
-000004f0: 226a 736f 6e72 6566 7e3d 312e 312e 3022  "jsonref~=1.1.0"
-00000500: 2c0d 0a20 2264 6570 656e 6465 6e63 792d  ,.. "dependency-
-00000510: 696e 6a65 6374 6f72 7e3d 342e 3431 2e30  injector~=4.41.0
-00000520: 222c 0d0a 2022 7069 6c67 7261 6d32 7e3d  ",.. "pilgram2~=
-00000530: 322e 302e 3222 2c0d 0a20 2276 346c 3270  2.0.2",.. "v4l2p
-00000540: 797e 3d30 2e36 2e32 3b20 706c 6174 666f  y~=0.6.2; platfo
-00000550: 726d 5f73 7973 7465 6d20 3d3d 2027 4c69  rm_system == 'Li
-00000560: 6e75 7827 222c 0d0a 2022 6770 696f 7a65  nux'",.. "gpioze
-00000570: 726f 7e3d 312e 362e 3222 2c0d 0a20 2267  ro~=1.6.2",.. "g
-00000580: 7068 6f74 6f32 7e3d 322e 332e 343b 2070  photo2~=2.3.4; p
-00000590: 6c61 7466 6f72 6d5f 7379 7374 656d 203d  latform_system =
-000005a0: 3d20 274c 696e 7578 2722 2c0d 0a20 2270  = 'Linux'",.. "p
-000005b0: 7974 686f 6e2d 7374 6174 656d 6163 6869  ython-statemachi
-000005c0: 6e65 7e3d 322e 302e 3022 0d0a 5d0d 0a0d  ne~=2.0.0"..]...
-000005d0: 0a5b 746f 6f6c 2e68 6174 6368 2e65 6e76  .[tool.hatch.env
-000005e0: 732e 7465 7374 5d0d 0a64 6570 656e 6465  s.test]..depende
-000005f0: 6e63 6965 7320 3d20 5b0d 0a20 2022 7079  ncies = [..  "py
-00000600: 7465 7374 7e3d 372e 322e 3022 2c0d 0a20  test~=7.2.0",.. 
-00000610: 2022 7079 7465 7374 2d62 656e 6368 6d61   "pytest-benchma
-00000620: 726b 7e3d 342e 302e 3022 2c0d 0a20 2022  rk~=4.0.0",..  "
-00000630: 7079 7465 7374 2d63 6f76 7e3d 342e 302e  pytest-cov~=4.0.
-00000640: 3022 2c0d 0a20 2022 7275 6666 7e3d 302e  0",..  "ruff~=0.
-00000650: 302e 3237 3022 2c0d 0a20 2022 6874 7470  0.270",..  "http
-00000660: 782d 7373 657e 3d30 2e33 2e31 222c 0d0a  x-sse~=0.3.1",..
-00000670: 2020 2268 7474 7078 7e3d 302e 3234 2e31    "httpx~=0.24.1
-00000680: 222c 0d0a 2020 2273 696d 706c 656a 7065  ",..  "simplejpe
-00000690: 677e 3d31 2e36 2e36 222c 0d0a 2020 2263  g~=1.6.6",..  "c
-000006a0: 6f76 6572 6167 655b 746f 6d6c 5d7e 3d37  overage[toml]~=7
-000006b0: 2e32 2e37 222c 0d0a 2020 2262 6c61 636b  .2.7",..  "black
-000006c0: 220d 0a5d 0d0a 2320 6c69 6263 616d 6572  "..]..# libcamer
-000006d0: 612f 7069 6361 6d65 7261 3220 6172 6520  a/picamera2 are 
-000006e0: 6176 6169 6c20 666f 7220 6e6f 7720 6f6e  avail for now on
-000006f0: 6c79 2061 7320 7379 7374 656d 2070 7974  ly as system pyt
-00000700: 686f 6e20 7061 636b 6167 6520 2d20 6973  hon package - is
-00000710: 6f6c 6174 6564 2065 6e76 2063 616e 6e6f  olated env canno
-00000720: 7420 7573 6520 7468 656d 2077 6974 686f  t use them witho
-00000730: 7574 2067 6c6f 6261 6c20 6163 6365 7373  ut global access
-00000740: 0d0a 7379 7374 656d 2d70 6163 6b61 6765  ..system-package
-00000750: 7320 3d20 7472 7565 0d0a 0d0a 5b74 6f6f  s = true....[too
-00000760: 6c2e 6861 7463 682e 656e 7673 2e74 6573  l.hatch.envs.tes
-00000770: 742e 7363 7269 7074 735d 0d0a 7465 7374  t.scripts]..test
-00000780: 203d 2022 7079 7465 7374 202d 7620 2d2d   = "pytest -v --
-00000790: 636f 762d 7265 706f 7274 3d74 6572 6d20  cov-report=term 
-000007a0: 2d2d 636f 762d 7265 706f 7274 3d78 6d6c  --cov-report=xml
-000007b0: 3a63 6f76 6572 6167 652e 786d 6c20 2d2d  :coverage.xml --
-000007c0: 636f 7620 2e2f 220d 0a0d 0a0d 0a0d 0a5b  cov ./"........[
-000007d0: 7072 6f6a 6563 742e 7572 6c73 5d0d 0a68  project.urls]..h
-000007e0: 6f6d 6570 6167 6520 3d20 2268 7474 7073  omepage = "https
-000007f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d67  ://github.com/mg
-00000800: 726c 2f70 686f 746f 626f 6f74 682d 6170  rl/photobooth-ap
-00000810: 7022 0d0a 7265 706f 7369 746f 7279 203d  p"..repository =
-00000820: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
-00000830: 2e63 6f6d 2f6d 6772 6c2f 7068 6f74 6f62  .com/mgrl/photob
-00000840: 6f6f 7468 2d61 7070 220d 0a64 6f63 756d  ooth-app"..docum
-00000850: 656e 7461 7469 6f6e 203d 2022 6874 7470  entation = "http
-00000860: 733a 2f2f 6d67 726c 2e67 6974 6875 622e  s://mgrl.github.
-00000870: 696f 2f70 686f 746f 626f 6f74 682d 646f  io/photobooth-do
-00000880: 6373 220d 0a0d 0a5b 7072 6f6a 6563 742e  cs"....[project.
-00000890: 7363 7269 7074 735d 0d0a 7068 6f74 6f62  scripts]..photob
-000008a0: 6f6f 7468 203d 2022 7068 6f74 6f62 6f6f  ooth = "photoboo
-000008b0: 7468 2e5f 5f6d 6169 6e5f 5f3a 6d61 696e  th.__main__:main
-000008c0: 220d 0a0d 0a5b 746f 6f6c 2e68 6174 6368  "....[tool.hatch
-000008d0: 2e62 7569 6c64 5d0d 0a69 6e63 6c75 6465  .build]..include
-000008e0: 203d 205b 0d0a 2020 222f 7068 6f74 6f62   = [..  "/photob
-000008f0: 6f6f 7468 222c 0d0a 5d0d 0a0d 0a5b 6275  ooth",..]....[bu
-00000900: 696c 642d 7379 7374 656d 5d0d 0a72 6571  ild-system]..req
-00000910: 7569 7265 7320 3d20 5b22 6861 7463 686c  uires = ["hatchl
-00000920: 696e 6722 5d0d 0a62 7569 6c64 2d62 6163  ing"]..build-bac
-00000930: 6b65 6e64 203d 2022 6861 7463 686c 696e  kend = "hatchlin
-00000940: 672e 6275 696c 6422 0d0a 0d0a 5b74 6f6f  g.build"....[too
-00000950: 6c2e 7079 7465 7374 2e69 6e69 5f6f 7074  l.pytest.ini_opt
-00000960: 696f 6e73 5d0d 0a6c 6f67 5f63 6c69 203d  ions]..log_cli =
-00000970: 2074 7275 650d 0a6c 6f67 5f63 6c69 5f6c   true..log_cli_l
-00000980: 6576 656c 203d 2022 4445 4255 4722 0d0a  evel = "DEBUG"..
-00000990: 6c6f 675f 636c 695f 666f 726d 6174 203d  log_cli_format =
-000009a0: 2022 2528 6173 6374 696d 6529 7320 5b25   "%(asctime)s [%
-000009b0: 286c 6576 656c 6e61 6d65 2938 735d 2025  (levelname)8s] %
-000009c0: 286d 6573 7361 6765 2973 2028 2528 6669  (message)s (%(fi
-000009d0: 6c65 6e61 6d65 2973 3a25 286c 696e 656e  lename)s:%(linen
-000009e0: 6f29 7329 220d 0a6c 6f67 5f63 6c69 5f64  o)s)"..log_cli_d
-000009f0: 6174 655f 666f 726d 6174 203d 2022 2559  ate_format = "%Y
-00000a00: 2d25 6d2d 2564 2025 483a 254d 3a25 5322  -%m-%d %H:%M:%S"
-00000a10: 0d0a 0d0a 5b74 6f6f 6c2e 636f 7665 7261  ....[tool.covera
-00000a20: 6765 2e72 756e 5d0d 0a23 2064 6973 6162  ge.run]..# disab
-00000a30: 6c65 2063 6f75 6c64 6e74 2d70 6172 7365  le couldnt-parse
-00000a40: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-00000a50: 2e63 6f6d 2f6e 6564 6261 742f 636f 7665  .com/nedbat/cove
-00000a60: 7261 6765 7079 2f69 7373 7565 732f 3133  ragepy/issues/13
-00000a70: 3932 0d0a 6469 7361 626c 655f 7761 726e  92..disable_warn
-00000a80: 696e 6773 203d 205b 2263 6f75 6c64 6e74  ings = ["couldnt
-00000a90: 2d70 6172 7365 225d 0d0a 6f6d 6974 203d  -parse"]..omit =
-00000aa0: 205b 0d0a 2020 2020 2274 6573 745f 2a2e   [..    "test_*.
-00000ab0: 7079 222c 0d0a 2020 2020 222e 2f74 6573  py",..    "./tes
-00000ac0: 7473 2f2a 222c 0d0a 2020 2020 222e 2f70  ts/*",..    "./p
-00000ad0: 686f 746f 626f 6f74 682f 7665 6e64 6f72  hotobooth/vendor
-00000ae0: 2f2a 220d 0a20 2020 205d 0d0a 7061 7261  /*"..    ]..para
-00000af0: 6c6c 656c 203d 2074 7275 650d 0a63 6f6e  llel = true..con
-00000b00: 6375 7272 656e 6379 203d 205b 2274 6872  currency = ["thr
-00000b10: 6561 6422 2c22 6d75 6c74 6970 726f 6365  ead","multiproce
-00000b20: 7373 696e 6722 5d0d 0a0d 0a5b 746f 6f6c  ssing"]....[tool
-00000b30: 2e62 6c61 636b 5d0d 0a6c 696e 652d 6c65  .black]..line-le
-00000b40: 6e67 7468 203d 2031 3230 0d0a 0d0a 5b74  ngth = 120....[t
-00000b50: 6f6f 6c2e 7275 6666 5d0d 0a6c 696e 652d  ool.ruff]..line-
-00000b60: 6c65 6e67 7468 203d 2031 3230 0d0a 7365  length = 120..se
-00000b70: 6c65 6374 203d 205b 0d0a 2020 2245 222c  lect = [..  "E",
-00000b80: 2020 2023 2070 7963 6f64 6573 7479 6c65     # pycodestyle
-00000b90: 0d0a 2020 2257 222c 2020 2023 2070 7963  ..  "W",   # pyc
-00000ba0: 6f64 6573 7479 6c65 0d0a 2020 2246 222c  odestyle..  "F",
-00000bb0: 2020 2023 2070 7966 6c61 6b65 730d 0a20     # pyflakes.. 
-00000bc0: 2022 4222 2c20 2020 2320 6275 6762 6561   "B",   # bugbea
-00000bd0: 720d 0a20 2022 5550 222c 2020 2320 7079  r..  "UP",  # py
-00000be0: 7570 6772 6164 650d 0a20 2022 4922 2c20  upgrade..  "I", 
-00000bf0: 2020 2320 6973 6f72 740d 0a20 2023 2244    # isort..  #"D
-00000c00: 222c 2020 2023 2070 7964 6f63 7374 796c  ",   # pydocstyl
-00000c10: 6520 2020 2320 6164 6420 6c61 7465 720d  e   # add later.
-00000c20: 0a5d 0d0a 6967 6e6f 7265 203d 205b 0d0a  .]..ignore = [..
-00000c30: 2020 2242 3030 3822 2023 7573 6564 2066    "B008" #used f
-00000c40: 6f72 2044 4920 696e 6a65 6374 696f 6e0d  or DI injection.
-00000c50: 0a20 205d 0d0a 6578 7465 6e64 2d65 7863  .  ]..extend-exc
-00000c60: 6c75 6465 203d 205b 2276 656e 646f 7222  lude = ["vendor"
-00000c70: 5d0d 0a0d 0a5b 746f 6f6c 2e72 7566 662e  ]....[tool.ruff.
-00000c80: 7065 722d 6669 6c65 2d69 676e 6f72 6573  per-file-ignores
-00000c90: 5d0d 0a22 7068 6f74 6f62 6f6f 7468 2f61  ].."photobooth/a
-00000ca0: 7070 636f 6e66 6967 2e70 7922 203d 205b  ppconfig.py" = [
-00000cb0: 2245 3530 3122 5d0d 0a0d 0a5b 746f 6f6c  "E501"]....[tool
-00000cc0: 2e72 7566 662e 7079 646f 6373 7479 6c65  .ruff.pydocstyle
-00000cd0: 5d0d 0a63 6f6e 7665 6e74 696f 6e20 3d20  ]..convention = 
-00000ce0: 2267 6f6f 676c 6522                      "google"
+000003d0: 6170 693e 3d30 2e31 3030 2e30 2c3c 302e  api>=0.100.0,<0.
+000003e0: 3130 312e 3022 2c0d 0a20 226f 7065 6e63  101.0",.. "openc
+000003f0: 762d 7079 7468 6f6e 3e3d 342e 372c 3c34  v-python>=4.7,<4
+00000400: 2e39 222c 0d0a 2022 7069 6578 6966 7e3d  .9",.. "piexif~=
+00000410: 312e 312e 3322 2c0d 0a20 2270 696c 6c6f  1.1.3",.. "pillo
+00000420: 773e 3d39 2e35 2c3c 3130 2e31 222c 0d0a  w>=9.5,<10.1",..
+00000430: 2022 7073 7574 696c 7e3d 352e 392e 3522   "psutil~=5.9.5"
+00000440: 2c0d 0a20 2270 7964 616e 7469 633e 3d32  ,.. "pydantic>=2
+00000450: 2e30 2e33 222c 0d0a 2022 7079 6461 6e74  .0.3",.. "pydant
+00000460: 6963 2d65 7874 7261 2d74 7970 6573 3e3d  ic-extra-types>=
+00000470: 322e 302e 3022 2c0d 0a20 2270 7964 616e  2.0.0",.. "pydan
+00000480: 7469 632d 7365 7474 696e 6773 3e3d 322e  tic-settings>=2.
+00000490: 302e 3222 2c0d 0a20 2270 796d 6974 7465  0.2",.. "pymitte
+000004a0: 727e 3d30 2e34 2e30 222c 0d0a 2022 7079  r~=0.4.0",.. "py
+000004b0: 7475 7262 6f6a 7065 677e 3d31 2e37 2e31  turbojpeg~=1.7.1
+000004c0: 222c 0d0a 2022 7265 7175 6573 7473 7e3d  ",.. "requests~=
+000004d0: 322e 3331 2e30 222c 0d0a 2022 7373 652d  2.31.0",.. "sse-
+000004e0: 7374 6172 6c65 7474 657e 3d31 2e36 2e31  starlette~=1.6.1
+000004f0: 222c 0d0a 2022 7576 6963 6f72 6e7e 3d30  ",.. "uvicorn~=0
+00000500: 2e32 322e 3022 2c0d 0a20 2270 7974 686f  .22.0",.. "pytho
+00000510: 6e2d 646f 7465 6e76 7e3d 312e 302e 3022  n-dotenv~=1.0.0"
+00000520: 2c0d 0a20 2270 7973 6572 6961 6c7e 3d33  ,.. "pyserial~=3
+00000530: 2e35 222c 0d0a 2022 6a73 6f6e 7265 667e  .5",.. "jsonref~
+00000540: 3d31 2e31 2e30 222c 0d0a 2022 6465 7065  =1.1.0",.. "depe
+00000550: 6e64 656e 6379 2d69 6e6a 6563 746f 727e  ndency-injector~
+00000560: 3d34 2e34 312e 3022 2c0d 0a20 2270 696c  =4.41.0",.. "pil
+00000570: 6772 616d 327e 3d32 2e30 2e32 222c 0d0a  gram2~=2.0.2",..
+00000580: 2022 7634 6c32 7079 7e3d 302e 362e 323b   "v4l2py~=0.6.2;
+00000590: 2070 6c61 7466 6f72 6d5f 7379 7374 656d   platform_system
+000005a0: 203d 3d20 274c 696e 7578 2722 2c0d 0a20   == 'Linux'",.. 
+000005b0: 2267 7069 6f7a 6572 6f7e 3d31 2e36 2e32  "gpiozero~=1.6.2
+000005c0: 222c 0d0a 2022 6770 686f 746f 323c 3d32  ",.. "gphoto2<=2
+000005d0: 2e33 2e34 3b20 706c 6174 666f 726d 5f73  .3.4; platform_s
+000005e0: 7973 7465 6d20 3d3d 2027 4c69 6e75 7827  ystem == 'Linux'
+000005f0: 222c 0d0a 2022 7079 7468 6f6e 2d73 7461  ",.. "python-sta
+00000600: 7465 6d61 6368 696e 653e 3d32 2e30 2c3c  temachine>=2.0,<
+00000610: 322e 3222 0d0a 5d0d 0a0d 0a5b 746f 6f6c  2.2"..]....[tool
+00000620: 2e68 6174 6368 2e65 6e76 732e 7465 7374  .hatch.envs.test
+00000630: 5d0d 0a64 6570 656e 6465 6e63 6965 7320  ]..dependencies 
+00000640: 3d20 5b0d 0a20 2022 7079 7465 7374 7e3d  = [..  "pytest~=
+00000650: 372e 342e 3022 2c0d 0a20 2022 7079 7465  7.4.0",..  "pyte
+00000660: 7374 2d62 656e 6368 6d61 726b 7e3d 342e  st-benchmark~=4.
+00000670: 302e 3022 2c0d 0a20 2022 7079 7465 7374  0.0",..  "pytest
+00000680: 2d63 6f76 7e3d 342e 312e 3022 2c0d 0a20  -cov~=4.1.0",.. 
+00000690: 2022 7275 6666 7e3d 302e 302e 3237 3822   "ruff~=0.0.278"
+000006a0: 2c0d 0a20 2022 6874 7470 782d 7373 657e  ,..  "httpx-sse~
+000006b0: 3d30 2e33 2e31 222c 0d0a 2020 2268 7474  =0.3.1",..  "htt
+000006c0: 7078 7e3d 302e 3234 2e31 222c 0d0a 2020  px~=0.24.1",..  
+000006d0: 2273 696d 706c 656a 7065 677e 3d31 2e36  "simplejpeg~=1.6
+000006e0: 2e36 222c 0d0a 2020 2263 6f76 6572 6167  .6",..  "coverag
+000006f0: 655b 746f 6d6c 5d7e 3d37 2e32 2e37 222c  e[toml]~=7.2.7",
+00000700: 0d0a 2020 2262 6c61 636b 220d 0a5d 0d0a  ..  "black"..]..
+00000710: 2320 6c69 6263 616d 6572 612f 7069 6361  # libcamera/pica
+00000720: 6d65 7261 3220 6172 6520 6176 6169 6c20  mera2 are avail 
+00000730: 666f 7220 6e6f 7720 6f6e 6c79 2061 7320  for now only as 
+00000740: 7379 7374 656d 2070 7974 686f 6e20 7061  system python pa
+00000750: 636b 6167 6520 2d20 6973 6f6c 6174 6564  ckage - isolated
+00000760: 2065 6e76 2063 616e 6e6f 7420 7573 6520   env cannot use 
+00000770: 7468 656d 2077 6974 686f 7574 2067 6c6f  them without glo
+00000780: 6261 6c20 6163 6365 7373 0d0a 7379 7374  bal access..syst
+00000790: 656d 2d70 6163 6b61 6765 7320 3d20 7472  em-packages = tr
+000007a0: 7565 0d0a 0d0a 5b74 6f6f 6c2e 6861 7463  ue....[tool.hatc
+000007b0: 682e 656e 7673 2e74 6573 742e 7363 7269  h.envs.test.scri
+000007c0: 7074 735d 0d0a 7465 7374 203d 2022 7079  pts]..test = "py
+000007d0: 7465 7374 202d 7620 2d2d 636f 762d 7265  test -v --cov-re
+000007e0: 706f 7274 3d74 6572 6d20 2d2d 636f 762d  port=term --cov-
+000007f0: 7265 706f 7274 3d78 6d6c 3a63 6f76 6572  report=xml:cover
+00000800: 6167 652e 786d 6c20 2d2d 636f 7620 2e2f  age.xml --cov ./
+00000810: 220d 0a0d 0a0d 0a0d 0a5b 7072 6f6a 6563  "........[projec
+00000820: 742e 7572 6c73 5d0d 0a68 6f6d 6570 6167  t.urls]..homepag
+00000830: 6520 3d20 2268 7474 7073 3a2f 2f67 6974  e = "https://git
+00000840: 6875 622e 636f 6d2f 6d67 726c 2f70 686f  hub.com/mgrl/pho
+00000850: 746f 626f 6f74 682d 6170 7022 0d0a 7265  tobooth-app"..re
+00000860: 706f 7369 746f 7279 203d 2022 6874 7470  pository = "http
+00000870: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+00000880: 6772 6c2f 7068 6f74 6f62 6f6f 7468 2d61  grl/photobooth-a
+00000890: 7070 220d 0a64 6f63 756d 656e 7461 7469  pp"..documentati
+000008a0: 6f6e 203d 2022 6874 7470 733a 2f2f 6d67  on = "https://mg
+000008b0: 726c 2e67 6974 6875 622e 696f 2f70 686f  rl.github.io/pho
+000008c0: 746f 626f 6f74 682d 646f 6373 220d 0a0d  tobooth-docs"...
+000008d0: 0a5b 7072 6f6a 6563 742e 7363 7269 7074  .[project.script
+000008e0: 735d 0d0a 7068 6f74 6f62 6f6f 7468 203d  s]..photobooth =
+000008f0: 2022 7068 6f74 6f62 6f6f 7468 2e5f 5f6d   "photobooth.__m
+00000900: 6169 6e5f 5f3a 6d61 696e 220d 0a0d 0a5b  ain__:main"....[
+00000910: 746f 6f6c 2e68 6174 6368 2e62 7569 6c64  tool.hatch.build
+00000920: 5d0d 0a69 6e63 6c75 6465 203d 205b 0d0a  ]..include = [..
+00000930: 2020 222f 7068 6f74 6f62 6f6f 7468 222c    "/photobooth",
+00000940: 0d0a 5d0d 0a0d 0a5b 6275 696c 642d 7379  ..]....[build-sy
+00000950: 7374 656d 5d0d 0a72 6571 7569 7265 7320  stem]..requires 
+00000960: 3d20 5b22 6861 7463 686c 696e 6722 5d0d  = ["hatchling"].
+00000970: 0a62 7569 6c64 2d62 6163 6b65 6e64 203d  .build-backend =
+00000980: 2022 6861 7463 686c 696e 672e 6275 696c   "hatchling.buil
+00000990: 6422 0d0a 0d0a 5b74 6f6f 6c2e 7079 7465  d"....[tool.pyte
+000009a0: 7374 2e69 6e69 5f6f 7074 696f 6e73 5d0d  st.ini_options].
+000009b0: 0a6c 6f67 5f63 6c69 203d 2074 7275 650d  .log_cli = true.
+000009c0: 0a6c 6f67 5f63 6c69 5f6c 6576 656c 203d  .log_cli_level =
+000009d0: 2022 4445 4255 4722 0d0a 6c6f 675f 636c   "DEBUG"..log_cl
+000009e0: 695f 666f 726d 6174 203d 2022 2528 6173  i_format = "%(as
+000009f0: 6374 696d 6529 7320 5b25 286c 6576 656c  ctime)s [%(level
+00000a00: 6e61 6d65 2938 735d 2025 286d 6573 7361  name)8s] %(messa
+00000a10: 6765 2973 2028 2528 6669 6c65 6e61 6d65  ge)s (%(filename
+00000a20: 2973 3a25 286c 696e 656e 6f29 7329 220d  )s:%(lineno)s)".
+00000a30: 0a6c 6f67 5f63 6c69 5f64 6174 655f 666f  .log_cli_date_fo
+00000a40: 726d 6174 203d 2022 2559 2d25 6d2d 2564  rmat = "%Y-%m-%d
+00000a50: 2025 483a 254d 3a25 5322 0d0a 0d0a 5b74   %H:%M:%S"....[t
+00000a60: 6f6f 6c2e 636f 7665 7261 6765 2e72 756e  ool.coverage.run
+00000a70: 5d0d 0a23 2064 6973 6162 6c65 2063 6f75  ]..# disable cou
+00000a80: 6c64 6e74 2d70 6172 7365 3a20 6874 7470  ldnt-parse: http
+00000a90: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6e  s://github.com/n
+00000aa0: 6564 6261 742f 636f 7665 7261 6765 7079  edbat/coveragepy
+00000ab0: 2f69 7373 7565 732f 3133 3932 0d0a 6469  /issues/1392..di
+00000ac0: 7361 626c 655f 7761 726e 696e 6773 203d  sable_warnings =
+00000ad0: 205b 2263 6f75 6c64 6e74 2d70 6172 7365   ["couldnt-parse
+00000ae0: 225d 0d0a 6f6d 6974 203d 205b 0d0a 2020  "]..omit = [..  
+00000af0: 2020 2274 6573 745f 2a2e 7079 222c 0d0a    "test_*.py",..
+00000b00: 2020 2020 222e 2f74 6573 7473 2f2a 222c      "./tests/*",
+00000b10: 0d0a 2020 2020 222e 2f70 686f 746f 626f  ..    "./photobo
+00000b20: 6f74 682f 7665 6e64 6f72 2f2a 220d 0a20  oth/vendor/*".. 
+00000b30: 2020 205d 0d0a 7061 7261 6c6c 656c 203d     ]..parallel =
+00000b40: 2074 7275 650d 0a63 6f6e 6375 7272 656e   true..concurren
+00000b50: 6379 203d 205b 2274 6872 6561 6422 2c22  cy = ["thread","
+00000b60: 6d75 6c74 6970 726f 6365 7373 696e 6722  multiprocessing"
+00000b70: 5d0d 0a0d 0a5b 746f 6f6c 2e62 6c61 636b  ]....[tool.black
+00000b80: 5d0d 0a6c 696e 652d 6c65 6e67 7468 203d  ]..line-length =
+00000b90: 2031 3230 0d0a 0d0a 5b74 6f6f 6c2e 7275   120....[tool.ru
+00000ba0: 6666 5d0d 0a6c 696e 652d 6c65 6e67 7468  ff]..line-length
+00000bb0: 203d 2031 3230 0d0a 7365 6c65 6374 203d   = 120..select =
+00000bc0: 205b 0d0a 2020 2245 222c 2020 2023 2070   [..  "E",   # p
+00000bd0: 7963 6f64 6573 7479 6c65 0d0a 2020 2257  ycodestyle..  "W
+00000be0: 222c 2020 2023 2070 7963 6f64 6573 7479  ",   # pycodesty
+00000bf0: 6c65 0d0a 2020 2246 222c 2020 2023 2070  le..  "F",   # p
+00000c00: 7966 6c61 6b65 730d 0a20 2022 4222 2c20  yflakes..  "B", 
+00000c10: 2020 2320 6275 6762 6561 720d 0a20 2022    # bugbear..  "
+00000c20: 5550 222c 2020 2320 7079 7570 6772 6164  UP",  # pyupgrad
+00000c30: 650d 0a20 2022 4922 2c20 2020 2320 6973  e..  "I",   # is
+00000c40: 6f72 740d 0a20 2023 2244 222c 2020 2023  ort..  #"D",   #
+00000c50: 2070 7964 6f63 7374 796c 6520 2020 2320   pydocstyle   # 
+00000c60: 6164 6420 6c61 7465 720d 0a5d 0d0a 6967  add later..]..ig
+00000c70: 6e6f 7265 203d 205b 0d0a 2020 2242 3030  nore = [..  "B00
+00000c80: 3822 2023 7573 6564 2066 6f72 2044 4920  8" #used for DI 
+00000c90: 696e 6a65 6374 696f 6e0d 0a20 205d 0d0a  injection..  ]..
+00000ca0: 6578 7465 6e64 2d65 7863 6c75 6465 203d  extend-exclude =
+00000cb0: 205b 2276 656e 646f 7222 5d0d 0a0d 0a5b   ["vendor"]....[
+00000cc0: 746f 6f6c 2e72 7566 662e 7065 722d 6669  tool.ruff.per-fi
+00000cd0: 6c65 2d69 676e 6f72 6573 5d0d 0a22 7068  le-ignores].."ph
+00000ce0: 6f74 6f62 6f6f 7468 2f61 7070 636f 6e66  otobooth/appconf
+00000cf0: 6967 2e70 7922 203d 205b 2245 3530 3122  ig.py" = ["E501"
+00000d00: 5d0d 0a0d 0a5b 746f 6f6c 2e72 7566 662e  ]....[tool.ruff.
+00000d10: 7079 646f 6373 7479 6c65 5d0d 0a63 6f6e  pydocstyle]..con
+00000d20: 7665 6e74 696f 6e20 3d20 2267 6f6f 676c  vention = "googl
+00000d30: 6522                                     e"
```

### Comparing `photobooth_app-0.1.0rc6/PKG-INFO` & `photobooth_app-0.1.0rc7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photobooth-app
-Version: 0.1.0rc6
+Version: 0.1.0rc7
 Summary: Photobooth app written in Python supporting DSLR, picamera2, webcameras
 Project-URL: homepage, https://github.com/mgrl/photobooth-app
 Project-URL: repository, https://github.com/mgrl/photobooth-app
 Project-URL: documentation, https://mgrl.github.io/photobooth-docs
 Author-email: Michael G <me@mgrl.de>
 Maintainer-email: Michael G <me@mgrl.de>
 License-File: LICENSE.md
@@ -16,28 +16,30 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Capture :: Digital Camera
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: <3.12,>=3.9
 Requires-Dist: dependency-injector~=4.41.0
-Requires-Dist: fastapi<0.97.0,>=0.95.2
-Requires-Dist: gphoto2~=2.3.4; platform_system == 'Linux'
+Requires-Dist: fastapi<0.101.0,>=0.100.0
+Requires-Dist: gphoto2<=2.3.4; platform_system == 'Linux'
 Requires-Dist: gpiozero~=1.6.2
 Requires-Dist: jsonref~=1.1.0
-Requires-Dist: opencv-python~=4.7.0
+Requires-Dist: opencv-python<4.9,>=4.7
 Requires-Dist: piexif~=1.1.3
 Requires-Dist: pilgram2~=2.0.2
-Requires-Dist: pillow~=9.5.0
+Requires-Dist: pillow<10.1,>=9.5
 Requires-Dist: psutil~=5.9.5
-Requires-Dist: pydantic~=1.10.8
+Requires-Dist: pydantic-extra-types>=2.0.0
+Requires-Dist: pydantic-settings>=2.0.2
+Requires-Dist: pydantic>=2.0.3
 Requires-Dist: pymitter~=0.4.0
 Requires-Dist: pyserial~=3.5
 Requires-Dist: python-dotenv~=1.0.0
-Requires-Dist: python-statemachine~=2.0.0
+Requires-Dist: python-statemachine<2.2,>=2.0
 Requires-Dist: pyturbojpeg~=1.7.1
 Requires-Dist: requests~=2.31.0
 Requires-Dist: sse-starlette~=1.6.1
 Requires-Dist: uvicorn~=0.22.0
 Requires-Dist: v4l2py~=0.6.2; platform_system == 'Linux'
 Description-Content-Type: text/markdown
```

