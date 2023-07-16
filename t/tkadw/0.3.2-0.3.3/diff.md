# Comparing `tmp/tkadw-0.3.2.tar.gz` & `tmp/tkadw-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkadw-0.3.2.tar", max compression
+gzip compressed data, was "tkadw-0.3.3.tar", max compression
```

## Comparing `tkadw-0.3.2.tar` & `tkadw-0.3.3.tar`

### file list

```diff
@@ -1,80 +1,82 @@
--rw-r--r--   0        0        0      421 2023-07-15 05:12:31.168424 tkadw-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2623 2023-07-15 05:13:40.274575 tkadw-0.3.2/README.md
--rw-r--r--   0        0        0      591 2023-07-14 05:18:03.595214 tkadw-0.3.2/tkadw/__init__.py
--rw-r--r--   0        0        0      729 2023-07-15 04:57:05.864349 tkadw-0.3.2/tkadw/__main__.py
--rw-r--r--   0        0        0       82 2023-07-09 09:06:40.819424 tkadw-0.3.2/tkadw/game/__init__.py
--rw-r--r--   0        0        0      274 2023-07-09 10:06:51.337745 tkadw-0.3.2/tkadw/game/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1081 2023-07-09 09:05:04.428075 tkadw-0.3.2/tkadw/game/__pycache__/surface.cpython-311.pyc
--rw-r--r--   0        0        0     1486 2023-07-09 10:06:51.339744 tkadw-0.3.2/tkadw/game/__pycache__/window.cpython-311.pyc
--rw-r--r--   0        0        0        0 2023-07-09 09:06:15.869430 tkadw-0.3.2/tkadw/game/action.py
--rw-r--r--   0        0        0      302 2023-07-09 09:05:03.855776 tkadw-0.3.2/tkadw/game/surface.py
--rw-r--r--   0        0        0      503 2023-07-09 09:03:53.662343 tkadw-0.3.2/tkadw/game/window.py
--rw-r--r--   0        0        0        0 2023-07-05 02:47:22.168814 tkadw-0.3.2/tkadw/utility/__init__.py
--rw-r--r--   0        0        0      127 2023-07-05 03:10:22.091006 tkadw-0.3.2/tkadw/utility/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      143 2023-07-05 02:48:08.371100 tkadw-0.3.2/tkadw/utility/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      851 2023-07-05 03:10:22.094005 tkadw-0.3.2/tkadw/utility/__pycache__/appconfig.cpython-310.pyc
--rw-r--r--   0        0        0     1779 2023-07-05 02:48:08.372100 tkadw-0.3.2/tkadw/utility/__pycache__/appconfig.cpython-311.pyc
--rw-r--r--   0        0        0    10003 2023-07-15 00:06:35.798144 tkadw-0.3.2/tkadw/utility/__pycache__/dragtool.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.3.2/tkadw/utility/app.config
--rw-r--r--   0        0        0      944 2023-07-05 02:48:08.189796 tkadw-0.3.2/tkadw/utility/appconfig.py
--rw-r--r--   0        0        0     5435 2023-07-15 00:06:32.738325 tkadw-0.3.2/tkadw/utility/dragtool.py
--rw-r--r--   0        0        0      107 2023-07-05 01:34:36.098785 tkadw-0.3.2/tkadw/windows/__init__.py
--rw-r--r--   0        0        0      229 2023-07-05 03:10:20.021585 tkadw-0.3.2/tkadw/windows/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      273 2023-07-05 01:35:29.380630 tkadw-0.3.2/tkadw/windows/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6883 2023-07-05 03:12:28.822756 tkadw-0.3.2/tkadw/windows/__pycache__/theme.cpython-310.pyc
--rw-r--r--   0        0        0    14199 2023-07-09 15:40:13.496015 tkadw-0.3.2/tkadw/windows/__pycache__/theme.cpython-311.pyc
--rw-r--r--   0        0        0     1138 2023-07-14 23:55:33.173781 tkadw-0.3.2/tkadw/windows/canvas/__init__.py
--rw-r--r--   0        0        0     1263 2023-07-05 03:10:20.085734 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1945 2023-07-14 23:57:15.913264 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    12827 2023-07-05 03:10:21.840626 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/button.cpython-310.pyc
--rw-r--r--   0        0        0    23268 2023-07-14 05:54:14.950226 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0    38279 2023-07-05 03:10:20.174751 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/drawengine.cpython-310.pyc
--rw-r--r--   0        0        0    44914 2023-07-05 01:35:29.406154 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/drawengine.cpython-311.pyc
--rw-r--r--   0        0        0    11053 2023-07-05 03:10:21.911520 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/entry.cpython-310.pyc
--rw-r--r--   0        0        0    21085 2023-07-05 01:35:43.431699 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0     6171 2023-07-05 03:10:22.086485 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/frame.cpython-310.pyc
--rw-r--r--   0        0        0    11531 2023-07-05 01:36:48.740493 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/frame.cpython-311.pyc
--rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2694 2023-07-05 03:12:28.867163 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/separator.cpython-310.pyc
--rw-r--r--   0        0        0     4558 2023-07-05 01:36:52.241618 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/separator.cpython-311.pyc
--rw-r--r--   0        0        0    13219 2023-07-05 03:10:21.930952 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/textbox.cpython-310.pyc
--rw-r--r--   0        0        0    25106 2023-07-09 15:08:09.223638 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/textbox.cpython-311.pyc
--rw-r--r--   0        0        0      943 2023-07-05 03:10:21.883207 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/widget.cpython-310.pyc
--rw-r--r--   0        0        0     1538 2023-07-14 05:57:28.861208 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/widget.cpython-311.pyc
--rw-r--r--   0        0        0    18129 2023-07-14 05:53:34.112161 tkadw-0.3.2/tkadw/windows/canvas/button.py
--rw-r--r--   0        0        0     6156 2023-07-05 01:39:19.281978 tkadw-0.3.2/tkadw/windows/canvas/checkbox.py
--rw-r--r--   0        0        0    39862 2023-07-04 09:19:04.412974 tkadw-0.3.2/tkadw/windows/canvas/drawengine.py
--rw-r--r--   0        0        0    15971 2023-07-05 01:35:43.285417 tkadw-0.3.2/tkadw/windows/canvas/entry.py
--rw-r--r--   0        0        0     6460 2023-07-05 01:36:48.456711 tkadw-0.3.2/tkadw/windows/canvas/frame.py
--rw-r--r--   0        0        0     2442 2023-07-05 01:36:52.052770 tkadw-0.3.2/tkadw/windows/canvas/separator.py
--rw-r--r--   0        0        0    17817 2023-07-09 15:08:09.086448 tkadw-0.3.2/tkadw/windows/canvas/textbox.py
--rw-r--r--   0        0        0     4597 2023-05-27 23:04:22.860566 tkadw-0.3.2/tkadw/windows/canvas/titlebar.py
--rw-r--r--   0        0        0      520 2023-07-14 05:57:26.216938 tkadw-0.3.2/tkadw/windows/canvas/widget.py
--rw-r--r--   0        0        0      223 2023-07-05 01:38:08.509601 tkadw-0.3.2/tkadw/windows/fluent/__init__.py
--rw-r--r--   0        0        0      401 2023-07-05 03:10:21.986646 tkadw-0.3.2/tkadw/windows/fluent/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      481 2023-07-05 01:38:08.644612 tkadw-0.3.2/tkadw/windows/fluent/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2899 2023-07-05 03:10:22.025283 tkadw-0.3.2/tkadw/windows/fluent/__pycache__/button.cpython-310.pyc
--rw-r--r--   0        0        0     5148 2023-07-05 01:38:39.662205 tkadw-0.3.2/tkadw/windows/fluent/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0     2955 2023-07-05 03:10:22.017187 tkadw-0.3.2/tkadw/windows/fluent/__pycache__/entry.cpython-310.pyc
--rw-r--r--   0        0        0     5190 2023-07-05 01:36:27.311777 tkadw-0.3.2/tkadw/windows/fluent/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0     1315 2023-07-05 03:10:22.047317 tkadw-0.3.2/tkadw/windows/fluent/__pycache__/frame.cpython-310.pyc
--rw-r--r--   0        0        0     1968 2023-07-05 01:38:48.418651 tkadw-0.3.2/tkadw/windows/fluent/__pycache__/frame.cpython-311.pyc
--rw-r--r--   0        0        0     4604 2023-07-05 01:38:39.519641 tkadw-0.3.2/tkadw/windows/fluent/button.py
--rw-r--r--   0        0        0     4545 2023-07-05 01:36:27.195727 tkadw-0.3.2/tkadw/windows/fluent/entry.py
--rw-r--r--   0        0        0      952 2023-07-05 01:38:48.118337 tkadw-0.3.2/tkadw/windows/fluent/frame.py
--rw-r--r--   0        0        0    66280 2022-07-26 17:24:46.000000 tkadw-0.3.2/tkadw/windows/fluent/GeneralSans-Regular.ttf
--rw-r--r--   0        0        0      639 2023-07-05 01:37:20.730737 tkadw-0.3.2/tkadw/windows/fluent/test.py
--rw-r--r--   0        0        0    20620 2023-07-09 15:40:13.355715 tkadw-0.3.2/tkadw/windows/theme.py
--rw-r--r--   0        0        0      151 2023-07-15 04:00:51.951970 tkadw-0.3.2/tkadw/windows/widgets/__init__.py
--rw-r--r--   0        0        0      271 2023-07-05 03:10:21.933019 tkadw-0.3.2/tkadw/windows/widgets/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      395 2023-07-15 04:02:14.716290 tkadw-0.3.2/tkadw/windows/widgets/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    19005 2023-07-05 03:10:21.948576 tkadw-0.3.2/tkadw/windows/widgets/__pycache__/adw.cpython-310.pyc
--rw-r--r--   0        0        0    21509 2023-07-05 02:08:39.052688 tkadw-0.3.2/tkadw/windows/widgets/__pycache__/adw.cpython-311.pyc
--rw-r--r--   0        0        0     2545 2023-07-05 03:10:21.971123 tkadw-0.3.2/tkadw/windows/widgets/__pycache__/label.cpython-310.pyc
--rw-r--r--   0        0        0     4377 2023-07-05 01:35:47.771212 tkadw-0.3.2/tkadw/windows/widgets/__pycache__/label.cpython-311.pyc
--rw-r--r--   0        0        0     3435 2023-07-15 04:48:08.638319 tkadw-0.3.2/tkadw/windows/widgets/__pycache__/mdi.cpython-311.pyc
--rw-r--r--   0        0        0    19150 2023-07-04 14:22:25.521559 tkadw-0.3.2/tkadw/windows/widgets/adw.py
--rw-r--r--   0        0        0     1992 2023-07-04 10:38:07.052633 tkadw-0.3.2/tkadw/windows/widgets/label.py
--rw-r--r--   0        0        0        0 2023-07-04 10:38:58.527667 tkadw-0.3.2/tkadw/windows/widgets/listbox.py
--rw-r--r--   0        0        0     1469 2023-07-15 04:48:08.519396 tkadw-0.3.2/tkadw/windows/widgets/mdi.py
--rw-r--r--   0        0        0     3215 1970-01-01 00:00:00.000000 tkadw-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      421 2023-07-16 05:19:58.382178 tkadw-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2745 2023-07-16 05:19:27.945475 tkadw-0.3.3/README.md
+-rw-r--r--   0        0        0      591 2023-07-14 05:18:03.595214 tkadw-0.3.3/tkadw/__init__.py
+-rw-r--r--   0        0        0      729 2023-07-15 04:57:05.864349 tkadw-0.3.3/tkadw/__main__.py
+-rw-r--r--   0        0        0    14254 2023-07-16 00:41:12.056850 tkadw-0.3.3/tkadw/doc.py
+-rw-r--r--   0        0        0       82 2023-07-09 09:06:40.819424 tkadw-0.3.3/tkadw/game/__init__.py
+-rw-r--r--   0        0        0      274 2023-07-09 10:06:51.337745 tkadw-0.3.3/tkadw/game/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1081 2023-07-09 09:05:04.428075 tkadw-0.3.3/tkadw/game/__pycache__/surface.cpython-311.pyc
+-rw-r--r--   0        0        0     1486 2023-07-09 10:06:51.339744 tkadw-0.3.3/tkadw/game/__pycache__/window.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2023-07-09 09:06:15.869430 tkadw-0.3.3/tkadw/game/action.py
+-rw-r--r--   0        0        0      302 2023-07-09 09:05:03.855776 tkadw-0.3.3/tkadw/game/surface.py
+-rw-r--r--   0        0        0      503 2023-07-09 09:03:53.662343 tkadw-0.3.3/tkadw/game/window.py
+-rw-r--r--   0        0        0        0 2023-07-05 02:47:22.168814 tkadw-0.3.3/tkadw/utility/__init__.py
+-rw-r--r--   0        0        0      127 2023-07-05 03:10:22.091006 tkadw-0.3.3/tkadw/utility/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      143 2023-07-05 02:48:08.371100 tkadw-0.3.3/tkadw/utility/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      851 2023-07-05 03:10:22.094005 tkadw-0.3.3/tkadw/utility/__pycache__/appconfig.cpython-310.pyc
+-rw-r--r--   0        0        0     1779 2023-07-05 02:48:08.372100 tkadw-0.3.3/tkadw/utility/__pycache__/appconfig.cpython-311.pyc
+-rw-r--r--   0        0        0    10003 2023-07-15 00:06:35.798144 tkadw-0.3.3/tkadw/utility/__pycache__/dragtool.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.3.3/tkadw/utility/app.config
+-rw-r--r--   0        0        0      944 2023-07-05 02:48:08.189796 tkadw-0.3.3/tkadw/utility/appconfig.py
+-rw-r--r--   0        0        0     5435 2023-07-15 00:06:32.738325 tkadw-0.3.3/tkadw/utility/dragtool.py
+-rw-r--r--   0        0        0      107 2023-07-05 01:34:36.098785 tkadw-0.3.3/tkadw/windows/__init__.py
+-rw-r--r--   0        0        0      229 2023-07-05 03:10:20.021585 tkadw-0.3.3/tkadw/windows/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      273 2023-07-05 01:35:29.380630 tkadw-0.3.3/tkadw/windows/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6883 2023-07-05 03:12:28.822756 tkadw-0.3.3/tkadw/windows/__pycache__/theme.cpython-310.pyc
+-rw-r--r--   0        0        0    15793 2023-07-16 02:32:48.335683 tkadw-0.3.3/tkadw/windows/__pycache__/theme.cpython-311.pyc
+-rw-r--r--   0        0        0     1138 2023-07-14 23:55:33.173781 tkadw-0.3.3/tkadw/windows/canvas/__init__.py
+-rw-r--r--   0        0        0     1263 2023-07-05 03:10:20.085734 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1945 2023-07-14 23:57:15.913264 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    12827 2023-07-05 03:10:21.840626 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/button.cpython-310.pyc
+-rw-r--r--   0        0        0    23197 2023-07-15 12:30:24.901956 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0    38279 2023-07-05 03:10:20.174751 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/drawengine.cpython-310.pyc
+-rw-r--r--   0        0        0    46492 2023-07-15 05:42:36.854511 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/drawengine.cpython-311.pyc
+-rw-r--r--   0        0        0    11053 2023-07-05 03:10:21.911520 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/entry.cpython-310.pyc
+-rw-r--r--   0        0        0    21085 2023-07-05 01:35:43.431699 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0     6171 2023-07-05 03:10:22.086485 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/frame.cpython-310.pyc
+-rw-r--r--   0        0        0    11993 2023-07-16 02:33:29.600856 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2694 2023-07-05 03:12:28.867163 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/separator.cpython-310.pyc
+-rw-r--r--   0        0        0     4558 2023-07-05 01:36:52.241618 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/separator.cpython-311.pyc
+-rw-r--r--   0        0        0    13219 2023-07-05 03:10:21.930952 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/textbox.cpython-310.pyc
+-rw-r--r--   0        0        0    25157 2023-07-16 00:24:41.799054 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/textbox.cpython-311.pyc
+-rw-r--r--   0        0        0      943 2023-07-05 03:10:21.883207 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2148 2023-07-16 00:33:11.740565 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/widget.cpython-311.pyc
+-rw-r--r--   0        0        0    18105 2023-07-15 12:30:12.087468 tkadw-0.3.3/tkadw/windows/canvas/button.py
+-rw-r--r--   0        0        0     6156 2023-07-05 01:39:19.281978 tkadw-0.3.3/tkadw/windows/canvas/checkbox.py
+-rw-r--r--   0        0        0    41631 2023-07-15 05:42:31.545384 tkadw-0.3.3/tkadw/windows/canvas/drawengine.py
+-rw-r--r--   0        0        0    15971 2023-07-05 01:35:43.285417 tkadw-0.3.3/tkadw/windows/canvas/entry.py
+-rw-r--r--   0        0        0     7018 2023-07-16 02:33:29.496750 tkadw-0.3.3/tkadw/windows/canvas/frame.py
+-rw-r--r--   0        0        0     2442 2023-07-05 01:36:52.052770 tkadw-0.3.3/tkadw/windows/canvas/separator.py
+-rw-r--r--   0        0        0    17828 2023-07-16 00:24:41.660268 tkadw-0.3.3/tkadw/windows/canvas/textbox.py
+-rw-r--r--   0        0        0     4625 2023-07-16 02:11:24.455259 tkadw-0.3.3/tkadw/windows/canvas/titlebar.py
+-rw-r--r--   0        0        0      782 2023-07-16 00:33:11.573705 tkadw-0.3.3/tkadw/windows/canvas/widget.py
+-rw-r--r--   0        0        0      223 2023-07-05 01:38:08.509601 tkadw-0.3.3/tkadw/windows/fluent/__init__.py
+-rw-r--r--   0        0        0      401 2023-07-05 03:10:21.986646 tkadw-0.3.3/tkadw/windows/fluent/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      481 2023-07-05 01:38:08.644612 tkadw-0.3.3/tkadw/windows/fluent/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2899 2023-07-05 03:10:22.025283 tkadw-0.3.3/tkadw/windows/fluent/__pycache__/button.cpython-310.pyc
+-rw-r--r--   0        0        0     5148 2023-07-05 01:38:39.662205 tkadw-0.3.3/tkadw/windows/fluent/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0     2955 2023-07-05 03:10:22.017187 tkadw-0.3.3/tkadw/windows/fluent/__pycache__/entry.cpython-310.pyc
+-rw-r--r--   0        0        0     5190 2023-07-05 01:36:27.311777 tkadw-0.3.3/tkadw/windows/fluent/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0     1315 2023-07-05 03:10:22.047317 tkadw-0.3.3/tkadw/windows/fluent/__pycache__/frame.cpython-310.pyc
+-rw-r--r--   0        0        0     1968 2023-07-05 01:38:48.418651 tkadw-0.3.3/tkadw/windows/fluent/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0     4604 2023-07-05 01:38:39.519641 tkadw-0.3.3/tkadw/windows/fluent/button.py
+-rw-r--r--   0        0        0     4545 2023-07-05 01:36:27.195727 tkadw-0.3.3/tkadw/windows/fluent/entry.py
+-rw-r--r--   0        0        0      952 2023-07-05 01:38:48.118337 tkadw-0.3.3/tkadw/windows/fluent/frame.py
+-rw-r--r--   0        0        0    66280 2022-07-26 17:24:46.000000 tkadw-0.3.3/tkadw/windows/fluent/GeneralSans-Regular.ttf
+-rw-r--r--   0        0        0      639 2023-07-05 01:37:20.730737 tkadw-0.3.3/tkadw/windows/fluent/test.py
+-rw-r--r--   0        0        0    25229 2023-07-16 02:32:48.172721 tkadw-0.3.3/tkadw/windows/theme.py
+-rw-r--r--   0        0        0      151 2023-07-15 04:00:51.951970 tkadw-0.3.3/tkadw/windows/widgets/__init__.py
+-rw-r--r--   0        0        0      271 2023-07-05 03:10:21.933019 tkadw-0.3.3/tkadw/windows/widgets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      395 2023-07-15 04:02:14.716290 tkadw-0.3.3/tkadw/windows/widgets/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    19005 2023-07-05 03:10:21.948576 tkadw-0.3.3/tkadw/windows/widgets/__pycache__/adw.cpython-310.pyc
+-rw-r--r--   0        0        0    23348 2023-07-15 09:49:04.159720 tkadw-0.3.3/tkadw/windows/widgets/__pycache__/adw.cpython-311.pyc
+-rw-r--r--   0        0        0     2545 2023-07-05 03:10:21.971123 tkadw-0.3.3/tkadw/windows/widgets/__pycache__/label.cpython-310.pyc
+-rw-r--r--   0        0        0     4377 2023-07-05 01:35:47.771212 tkadw-0.3.3/tkadw/windows/widgets/__pycache__/label.cpython-311.pyc
+-rw-r--r--   0        0        0     3435 2023-07-15 04:48:08.638319 tkadw-0.3.3/tkadw/windows/widgets/__pycache__/mdi.cpython-311.pyc
+-rw-r--r--   0        0        0    20035 2023-07-15 09:49:03.946070 tkadw-0.3.3/tkadw/windows/widgets/adw.py
+-rw-r--r--   0        0        0     1992 2023-07-04 10:38:07.052633 tkadw-0.3.3/tkadw/windows/widgets/label.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:38:58.527667 tkadw-0.3.3/tkadw/windows/widgets/listbox.py
+-rw-r--r--   0        0        0     1469 2023-07-15 04:48:08.519396 tkadw-0.3.3/tkadw/windows/widgets/mdi.py
+-rw-r--r--   0        0        0        0 2023-07-15 06:50:07.630293 tkadw-0.3.3/tkadw/windows/widgets/toolbox.py
+-rw-r--r--   0        0        0     3332 1970-01-01 00:00:00.000000 tkadw-0.3.3/PKG-INFO
```

### Comparing `tkadw-0.3.2/README.md` & `tkadw-0.3.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -71,8 +71,13 @@
 >> `303`调改`AdwDrawEntry`和`AdwDrawText`的焦点事件绑定
 > 
 >> `304`新增主题类组件，只需使用`set_default_theme`设置主题。对于经过特殊设计和特殊样式的组件，比如`Fluent`主题组件、`Win11`主题控件`AccentButton`，将不加入主题变量内
 
 > `0.3.2`
 >> `321` 新增`AdwMDI`组件
 > 
->> `322` 添加`metro`主题
+>> `322` 添加`metro`主题
+
+> `0.3.3`
+>> `331` 修复`AdwDrawFrame`的边框宽度问题
+> 
+>> `332` 增加主题属性`AdwDrawFrame` `padding`
```

### Comparing `tkadw-0.3.2/tkadw/__init__.py` & `tkadw-0.3.3/tkadw/__init__.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/__main__.py` & `tkadw-0.3.3/tkadw/__main__.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/game/__pycache__/surface.cpython-311.pyc` & `tkadw-0.3.3/tkadw/game/__pycache__/surface.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/game/__pycache__/window.cpython-311.pyc` & `tkadw-0.3.3/tkadw/game/__pycache__/window.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/utility/__pycache__/appconfig.cpython-310.pyc` & `tkadw-0.3.3/tkadw/utility/__pycache__/appconfig.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/utility/__pycache__/appconfig.cpython-311.pyc` & `tkadw-0.3.3/tkadw/utility/__pycache__/appconfig.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/utility/__pycache__/dragtool.cpython-311-pytest-7.3.1.pyc` & `tkadw-0.3.3/tkadw/utility/__pycache__/dragtool.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/utility/appconfig.py` & `tkadw-0.3.3/tkadw/utility/appconfig.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/utility/dragtool.py` & `tkadw-0.3.3/tkadw/utility/dragtool.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/__pycache__/theme.cpython-310.pyc` & `tkadw-0.3.3/tkadw/windows/__pycache__/theme.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/__pycache__/theme.cpython-311.pyc` & `tkadw-0.3.3/tkadw/windows/__pycache__/theme.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,1463 +1,1768 @@
 magic:    0xa70d0d0a
-moddate:  0xddd4aa64 (Sun Jul  9 15:40:13 2023 UTC)
-files sz: 20620
+moddate:  0xd056b364 (Sun Jul 16 02:32:48 2023 UTC)
+files sz: 25229
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 20
    flags     : 0
    code
       0x97006400640169016402640364049c0264056406640764086409640a64
       0b64086409640c9c04640d640e64086409640c9c04640f9c076410640d64
-      11641264139c04640564146406640e64156409641664096417640e641564
-      096418641264199c06641a9c09640564146406640e641564096416640964
-      17640e641564096418641264199c06641a9c09641b6409641c641d9c0364
-      1e9c075a006400640869016402641764049c026405641f6420640e640964
-      216420640e6409640c9c0464226423640e6409640c9c04640f9c07641064
-      246421641264139c04640564146425642564266409642764096424642364
-      2664096428641264199c06641a9c09640564146425642564266409642764
-      0964246423642664096428641264199c06641a9c0964296409641c641d9c
-      03641e9c075a016400641769016402640364049c02642a642b642c642d64
-      2e642f6430642d642e640c9c0464306430642d642e640c9c04640f9c0764
-      31642b6432641264139c04642a6433641764346403640964356431641764
-      36640364096437643164199c06641a9c0964336431641764346403640964
-      35643164176436640364096437643164199c0664389c0964396409641c64
-      1d9c03641e9c075a026400643a69016402641764049c02642a643a643b64
-      3c642e643d643b643c642e640c9c04643e643f643c642e640c9c04640f9c
-      0764316420643b641264139c04642a643364406441644264096435643164
-      406436641764096436643164199c06641a9c096433643164406441644264
-      096435643164406436641764096436643164199c0664389c09643f640964
-      1c641d9c03641e9c075a036400641769016402640364049c026443641764
-      44641564096444644464156409640c9c046445644464466409640c9c0464
-      0f9c07644764486449641264139c04644364146417644464156409643564
-      316417644a641564096437643164199c06641a9c09644364146417644464
-      156409643564316417644a641564096437643164199c06641a9c09644964
-      09641c641d9c03641e9c075a046400644b69016402641764049c02644364
-      4c644d644e6409644d644d644e6409640c9c04644f644d64506409640c9c
-      04640f9c07644764516452641264139c0464436414644b644d6426640964
-      356431644b6453642664096453643164199c06641a9c0964436414644b64
-      4d6426640964356431644b6453642664096453643164199c06641a9c0964
-      526409641c641d9c03641e9c075a056400641769016402640364049c0264
-      3164546442640364096455645564176409640c9c04645664566417640964
-      0c9c04640f9c07643164176457641264139c046431645864176459640364
-      09641764316417645a640364096417643164199c06641a9c096431645864
-      17645964036409641764316417645a640364096417643164199c06641a9c
-      0964596409641c641d9c03641e9c075a066400645b69016402640364049c
-      026431645c645d64176409645e645e64036409640c9c0464546454640364
-      09640c9c04640f9c076431645b643d641264139c0464316458645b645964
-      17640964036431645b645a641764096403643164199c06641a9c09643164
-      58645b64596417640964036431645b645a641764096403643164199c0664
-      1a9c0964596409645f641d9c03641e9c075a07646084005a08646184005a
-      096484646384015a0a0200650a6464a6010000ab01000000000000000001
-      00643164656c0b6d0c5a0c010002004700646684006467650ca6030000ab
-      0300000000000000005a0d643164686c0e6d0f5a0f010002004700646984
-      00646a650fa6030000ab0300000000000000005a106431646b6c116d125a
-      12010002004700646c8400646d6512a6030000ab0300000000000000005a
-      136431646e6c146d155a15010002004700646f840064706515a6030000ab
-      0300000000000000005a16643164716c176d185a18010002004700647284
-      0064736518a6030000ab0300000000000000005a19643164746c1a6d1b5a
-      1b010002004700647584006476651ba6030000ab0300000000000000005a
-      1c643164776c1d6d1e5a1e010002004700647884006479651ea6030000ab
-      0300000000000000005a1f6520647a6b020000000072ef6431647b6c216d
-      225a2201000200650da6000000ab0000000000000000005a236523a00a00
-      00000000000000000000000000000000000000647ca6010000ab01000000
-      00000000000100647d84005a2402006513646d6524ac7ea6020000ab0200
-      000000000000005a256525a0260000000000000000000000000000000000
-      000000647f64806480ac81a6030000ab0300000000000000000100020065
-      1fa6000000ab0000000000000000005a276527a026000000000000000000
-      0000000000000000000000647f64806480ac81a6030000ab030000000000
-      0000000100020065166470ac82a6010000ab0100000000000000005a2865
-      28a0260000000000000000000000000000000000000000647f64806480ac
-      81a6030000ab0300000000000000000100020065196473ac82a6010000ab
-      0100000000000000005a296529a026000000000000000000000000000000
-      0000000000647f64806480ac81a6030000ab030000000000000000010002
-      00651ca6000000ab0000000000000000005a2a652aa02600000000000000
-      00000000000000000000000000647f64806480ac81a6030000ab03000000
-      000000000001006523a02b00000000000000000000000000000000000000
-      00a6000000ab00000000000000000001006483530064835300
-     0           0 RESUME                   0
+      116409641264139c05640564146415641664176409641864096415640e64
+      1764096419641a641b9c06641c9c09640564146415641664176409641864
+      096415640e641764096419641a641b9c06641c9c09641d6409641e641f9c
+      0364209c075a006400640869016402641564049c02640564216422640e64
+      0964236422640e6409640c9c0464246425640e6409640c9c04640f9c0764
+      10642664236409641264139c056405641464256427642864096429640964
+      26642564286409642a641a641b9c06641c9c096405641464256427642864
+      09642964096426642564286409642a641a641b9c06641c9c09642b640964
+      1e641f9c0364209c075a016400641569016402640364049c02642c642d64
+      2e642f643064316432642f6430640c9c0464326432642f6430640c9c0464
+      0f9c076412642d64336409641264139c05642c6434641564356403640964
+      366412641564376403640964386412641b9c06641c9c0964346412641564
+      356403640964366412641564376403640964386412641b9c0664399c0964
+      3a6409641e641f9c0364209c075a026400643b69016402641564049c0264
+      2c643b643c643d6430643e643c643d6430640c9c04643f6440643d643064
+      0c9c04640f9c0764126422643c6409641264139c05642c64346441644264
+      43640964366412644164376415640964376412641b9c06641c9c09643464
+      12644164426443640964366412644164376415640964376412641b9c0664
+      399c0964406409641e641f9c0364209c075a036400641569016402640364
+      049c02644464156445641764096445644564176409640c9c046446644564
+      476409640c9c04640f9c0764486449644a6409641264139c056444641464
+      15644564176409643664126415644b6417640964386412641b9c06641c9c
+      09644464146415644564176409643664126415644b641764096438641264
+      1b9c06641c9c09644a6409641e641f9c0364209c075a046400644c690164
+      02641564049c026444644d644e644f6409644e644e644f6409640c9c0464
+      50644e64516409640c9c04640f9c076448645264536409641264139c0564
+      446414644c644e6428640964366412644c64546428640964546412641b9c
+      06641c9c0964446414644c644e6428640964366412644c64546428640964
+      546412641b9c06641c9c0964536409641e641f9c0364209c075a05640064
+      1569016402640364049c0264126455644364036409645664566415640964
+      0c9c046457645764156409640c9c04640f9c076412641564586409641264
+      139c05641264596415645a64036409641564126415645b64036409641564
+      12641b9c06641c9c09641264596415645a64036409641564126415645b64
+      03640964156412641b9c06641c9c09645a6409641e641f9c0364209c075a
+      066400645c69016402640364049c026412645d645e64156409645f645f64
+      036409640c9c046455645564036409640c9c04640f9c076412645c643e64
+      09641264139c0564126459645c645a6415640964036412645c645b641564
+      0964036412641b9c06641c9c0964126459645c645a641564096403641264
+      5c645b6415640964036412641b9c06641c9c09645a64096460641f9c0364
+      209c075a076400646169016402640364049c026412641564626403640964
+      63646264036409640c9c04646364646403641a640c9c04640f9c07641264
+      6164656409641264139c0564126459641564626403640964156412641564
+      626403640964156412641b9c06641c9c0964126459641564626403640964
+      156412641564626403640964156412641b9c06641c9c09645a6409641e64
+      1f9c0364209c075a086400646669016402641564049c0264126424646764
+      156409643e646764156409640c9c04643e64646415641a640c9c04640f9c
+      076412646664686409641264139c05641264596424646764156409641564
+      12642464676415640964156412641b9c06641c9c09641264596424646764
+      15640964156412642464676415640964156412641b9c06641c9c09646864
+      096460641f9c0364209c075a09646984005a0a646a84005a0b648b646c84
+      015a0c0200650c646da6010000ab01000000000000000001006412646e6c
+      0d6d0e5a0e010002004700646f84006470650ea6030000ab030000000000
+      0000005a0f641264716c106d115a110100020047006472840064736511a6
+      030000ab0300000000000000005a12641264746c136d145a140100020047
+      006475840064766514a6030000ab0300000000000000005a15641264776c
+      166d175a170100020047006478840064796517a6030000ab030000000000
+      0000005a186412647a6c196d1a5a1a010002004700647b8400647c651aa6
+      030000ab0300000000000000005a1b6412647d6c1c6d1d5a1d0100020047
+      00647e8400647f651da6030000ab0300000000000000005a1e641264806c
+      1f6d205a200100020047006481840064826520a6030000ab030000000000
+      0000005a21652264836b020000000072ec641264846c236d245a24010002
+      00650fa6000000ab0000000000000000005a256525a00c00000000000000
+      00000000000000000000000000646d6485a6020000ab0200000000000000
+      000100020065156476ac86a6010000ab0100000000000000005a266526a0
+      270000000000000000000000000000000000000000648764886488ac89a6
+      030000ab030000000000000000010002006521a6000000ab000000000000
+      0000005a286528a027000000000000000000000000000000000000000064
+      8764886488ac89a6030000ab0300000000000000000100020065186479ac
+      86a6010000ab0100000000000000005a296529a027000000000000000000
+      0000000000000000000000648764886488ac89a6030000ab030000000000
+      00000001000200651b647cac86a6010000ab0100000000000000005a2a65
+      2aa0270000000000000000000000000000000000000000648764886488ac
+      89a6030000ab03000000000000000001000200651ea6000000ab00000000
+      00000000005a2b652ba02700000000000000000000000000000000000000
+      00648764886488ac89a6030000ab03000000000000000001006525a02c00
+      00000000000000000000000000000000000000a6000000ab000000000000
+      0000000100648a5300648a5300
+      0           0 RESUME                   0
    
-     3           2 LOAD_CONST               0 ('back')
-                 4 LOAD_CONST               1 ('#f4f4f4')
+      3           2 LOAD_CONST               0 ('back')
+                  4 LOAD_CONST               1 ('#f4f4f4')
    
-     2           6 BUILD_MAP                1
+      2           6 BUILD_MAP                1
    
-     7           8 LOAD_CONST               2 ('transparent')
+      7           8 LOAD_CONST               2 ('transparent')
    
-     8          10 LOAD_CONST               3 ('#000000')
+      8          10 LOAD_CONST               3 ('#000000')
    
-     6          12 LOAD_CONST               4 (('back', 'text_back'))
-                14 BUILD_CONST_KEY_MAP      2
+      6          12 LOAD_CONST               4 (('back', 'text_back'))
+                 14 BUILD_CONST_KEY_MAP      2
    
-    12          16 LOAD_CONST               5 (13)
+     12          16 LOAD_CONST               5 (13)
    
-    13          18 LOAD_CONST               6 ('#fdfdfd')
+     13          18 LOAD_CONST               6 ('#fdfdfd')
    
-    14          20 LOAD_CONST               7 ('#ededed')
+     14          20 LOAD_CONST               7 ('#ededed')
    
-    15          22 LOAD_CONST               8 ('#202020')
+     15          22 LOAD_CONST               8 ('#202020')
    
-    16          24 LOAD_CONST               9 (1)
+     16          24 LOAD_CONST               9 (1)
    
-    19          26 LOAD_CONST              10 ('#f9f9f9')
+     19          26 LOAD_CONST              10 ('#f9f9f9')
    
-    20          28 LOAD_CONST              11 ('#d5d5d5')
+     20          28 LOAD_CONST              11 ('#d5d5d5')
    
-    21          30 LOAD_CONST               8 ('#202020')
+     21          30 LOAD_CONST               8 ('#202020')
    
-    22          32 LOAD_CONST               9 (1)
+     22          32 LOAD_CONST               9 (1)
    
-    18          34 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
-                36 BUILD_CONST_KEY_MAP      4
+     18          34 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+                 36 BUILD_CONST_KEY_MAP      4
    
-    26          38 LOAD_CONST              13 ('#fafafa')
+     26          38 LOAD_CONST              13 ('#fafafa')
    
-    27          40 LOAD_CONST              14 ('#ebebeb')
+     27          40 LOAD_CONST              14 ('#ebebeb')
    
-    28          42 LOAD_CONST               8 ('#202020')
+     28          42 LOAD_CONST               8 ('#202020')
    
-    29          44 LOAD_CONST               9 (1)
+     29          44 LOAD_CONST               9 (1)
    
-    25          46 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
-                48 BUILD_CONST_KEY_MAP      4
+     25          46 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+                 48 BUILD_CONST_KEY_MAP      4
    
-    11          50 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
-                52 BUILD_CONST_KEY_MAP      7
+     11          50 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                 52 BUILD_CONST_KEY_MAP      7
    
-    34          54 LOAD_CONST              16 (15)
+     34          54 LOAD_CONST              16 (15)
    
-    35          56 LOAD_CONST              13 ('#fafafa')
+     35          56 LOAD_CONST              13 ('#fafafa')
    
-    36          58 LOAD_CONST              17 ('#e7e7e7')
+     36          58 LOAD_CONST              17 ('#e7e7e7')
    
-    37          60 LOAD_CONST              18 (2)
+     37          60 LOAD_CONST               9 (1)
    
-    33          62 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width'))
-                64 BUILD_CONST_KEY_MAP      4
+     38          62 LOAD_CONST              18 (0)
    
-    41          66 LOAD_CONST               5 (13)
+     33          64 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width', 'padding'))
+                 66 BUILD_CONST_KEY_MAP      5
    
-    42          68 LOAD_CONST              20 ((8, 8))
+     42          68 LOAD_CONST               5 (13)
    
-    44          70 LOAD_CONST               6 ('#fdfdfd')
+     43          70 LOAD_CONST              20 ((8, 8))
    
-    45          72 LOAD_CONST              14 ('#ebebeb')
+     45          72 LOAD_CONST              21 ('#ffffff')
    
-    46          74 LOAD_CONST              21 ('#18191c')
+     46          74 LOAD_CONST              22 ('#e6e6e6')
    
-    47          76 LOAD_CONST               9 (1)
+     47          76 LOAD_CONST              23 ('#18191c')
    
-    49          78 LOAD_CONST              22 ('#8a8a8a')
+     48          78 LOAD_CONST               9 (1)
    
-    50          80 LOAD_CONST               9 (1)
+     50          80 LOAD_CONST              24 ('#9c9c9c')
    
-    53          82 LOAD_CONST              23 ('#ffffff')
+     51          82 LOAD_CONST               9 (1)
    
-    54          84 LOAD_CONST              14 ('#ebebeb')
+     54          84 LOAD_CONST              21 ('#ffffff')
    
-    55          86 LOAD_CONST              21 ('#18191c')
+     55          86 LOAD_CONST              14 ('#ebebeb')
    
-    56          88 LOAD_CONST               9 (1)
+     56          88 LOAD_CONST              23 ('#18191c')
    
-    58          90 LOAD_CONST              24 ('#005fb8')
+     57          90 LOAD_CONST               9 (1)
    
-    59          92 LOAD_CONST              18 (2)
+     59          92 LOAD_CONST              25 ('#005fb8')
    
-    52          94 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
-                96 BUILD_CONST_KEY_MAP      6
+     60          94 LOAD_CONST              26 (2)
    
-    40          98 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
-               100 BUILD_CONST_KEY_MAP      9
+     53          96 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                 98 BUILD_CONST_KEY_MAP      6
    
-    64         102 LOAD_CONST               5 (13)
+     41         100 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                102 BUILD_CONST_KEY_MAP      9
    
-    65         104 LOAD_CONST              20 ((8, 8))
+     65         104 LOAD_CONST               5 (13)
    
-    67         106 LOAD_CONST               6 ('#fdfdfd')
+     66         106 LOAD_CONST              20 ((8, 8))
    
-    68         108 LOAD_CONST              14 ('#ebebeb')
+     68         108 LOAD_CONST              21 ('#ffffff')
    
-    69         110 LOAD_CONST              21 ('#18191c')
+     69         110 LOAD_CONST              22 ('#e6e6e6')
    
-    70         112 LOAD_CONST               9 (1)
+     70         112 LOAD_CONST              23 ('#18191c')
    
-    72         114 LOAD_CONST              22 ('#8a8a8a')
+     71         114 LOAD_CONST               9 (1)
    
-    73         116 LOAD_CONST               9 (1)
+     73         116 LOAD_CONST              24 ('#9c9c9c')
    
-    76         118 LOAD_CONST              23 ('#ffffff')
+     74         118 LOAD_CONST               9 (1)
    
-    77         120 LOAD_CONST              14 ('#ebebeb')
+     77         120 LOAD_CONST              21 ('#ffffff')
    
-    78         122 LOAD_CONST              21 ('#18191c')
+     78         122 LOAD_CONST              14 ('#ebebeb')
    
-    79         124 LOAD_CONST               9 (1)
+     79         124 LOAD_CONST              23 ('#18191c')
    
-    81         126 LOAD_CONST              24 ('#005fb8')
+     80         126 LOAD_CONST               9 (1)
    
-    82         128 LOAD_CONST              18 (2)
+     82         128 LOAD_CONST              25 ('#005fb8')
    
-    75         130 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
-               132 BUILD_CONST_KEY_MAP      6
+     83         130 LOAD_CONST              26 (2)
    
-    63         134 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
-               136 BUILD_CONST_KEY_MAP      9
+     76         132 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                134 BUILD_CONST_KEY_MAP      6
    
-    87         138 LOAD_CONST              27 ('#d0d0d0')
+     64         136 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                138 BUILD_CONST_KEY_MAP      9
    
-    88         140 LOAD_CONST               9 (1)
+     88         140 LOAD_CONST              29 ('#d0d0d0')
    
-    90         142 LOAD_CONST              28 (True)
+     89         142 LOAD_CONST               9 (1)
    
-    86         144 LOAD_CONST              29 (('back', 'border_width', 'rounded'))
-               146 BUILD_CONST_KEY_MAP      3
+     91         144 LOAD_CONST              30 (True)
    
-     1         148 LOAD_CONST              30 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
-               150 BUILD_CONST_KEY_MAP      7
-               152 STORE_NAME               0 (win11_theme)
+     87         146 LOAD_CONST              31 (('back', 'border_width', 'rounded'))
+                148 BUILD_CONST_KEY_MAP      3
    
-    96         154 LOAD_CONST               0 ('back')
-               156 LOAD_CONST               8 ('#202020')
+      1         150 LOAD_CONST              32 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
+                152 BUILD_CONST_KEY_MAP      7
+                154 STORE_NAME               0 (win11_theme)
    
-    95         158 BUILD_MAP                1
+     97         156 LOAD_CONST               0 ('back')
+                158 LOAD_CONST               8 ('#202020')
    
-   100         160 LOAD_CONST               2 ('transparent')
+     96         160 BUILD_MAP                1
    
-   101         162 LOAD_CONST              23 ('#ffffff')
+    101         162 LOAD_CONST               2 ('transparent')
    
-    99         164 LOAD_CONST               4 (('back', 'text_back'))
-               166 BUILD_CONST_KEY_MAP      2
+    102         164 LOAD_CONST              21 ('#ffffff')
    
-   105         168 LOAD_CONST               5 (13)
+    100         166 LOAD_CONST               4 (('back', 'text_back'))
+                168 BUILD_CONST_KEY_MAP      2
    
-   106         170 LOAD_CONST              31 ('#2a2a2a')
+    106         170 LOAD_CONST               5 (13)
    
-   107         172 LOAD_CONST              32 ('#313131')
+    107         172 LOAD_CONST              33 ('#2a2a2a')
    
-   108         174 LOAD_CONST              14 ('#ebebeb')
+    108         174 LOAD_CONST              34 ('#313131')
    
-   109         176 LOAD_CONST               9 (1)
+    109         176 LOAD_CONST              14 ('#ebebeb')
    
-   112         178 LOAD_CONST              33 ('#2f2f2f')
+    110         178 LOAD_CONST               9 (1)
    
-   113         180 LOAD_CONST              32 ('#313131')
+    113         180 LOAD_CONST              35 ('#2f2f2f')
    
-   114         182 LOAD_CONST              14 ('#ebebeb')
+    114         182 LOAD_CONST              34 ('#313131')
    
-   115         184 LOAD_CONST               9 (1)
+    115         184 LOAD_CONST              14 ('#ebebeb')
    
-   111         186 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
-               188 BUILD_CONST_KEY_MAP      4
+    116         186 LOAD_CONST               9 (1)
    
-   119         190 LOAD_CONST              34 ('#232323')
+    112         188 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+                190 BUILD_CONST_KEY_MAP      4
    
-   120         192 LOAD_CONST              35 ('#2c2c2c')
+    120         192 LOAD_CONST              36 ('#232323')
    
-   121         194 LOAD_CONST              14 ('#ebebeb')
+    121         194 LOAD_CONST              37 ('#2c2c2c')
    
-   122         196 LOAD_CONST               9 (1)
+    122         196 LOAD_CONST              14 ('#ebebeb')
    
-   118         198 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
-               200 BUILD_CONST_KEY_MAP      4
+    123         198 LOAD_CONST               9 (1)
    
-   104         202 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
-               204 BUILD_CONST_KEY_MAP      7
+    119         200 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+                202 BUILD_CONST_KEY_MAP      4
    
-   127         206 LOAD_CONST              16 (15)
+    105         204 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                206 BUILD_CONST_KEY_MAP      7
    
-   128         208 LOAD_CONST              36 ('#1c1c1c')
+    128         208 LOAD_CONST              16 (15)
    
-   129         210 LOAD_CONST              33 ('#2f2f2f')
+    129         210 LOAD_CONST              38 ('#1c1c1c')
    
-   130         212 LOAD_CONST              18 (2)
+    130         212 LOAD_CONST              35 ('#2f2f2f')
    
-   126         214 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width'))
-               216 BUILD_CONST_KEY_MAP      4
+    131         214 LOAD_CONST               9 (1)
    
-   134         218 LOAD_CONST               5 (13)
+    132         216 LOAD_CONST              18 (0)
    
-   135         220 LOAD_CONST              20 ((8, 8))
+    127         218 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width', 'padding'))
+                220 BUILD_CONST_KEY_MAP      5
    
-   137         222 LOAD_CONST              37 ('#292929')
+    136         222 LOAD_CONST               5 (13)
    
-   138         224 LOAD_CONST              37 ('#292929')
+    137         224 LOAD_CONST              20 ((8, 8))
    
-   139         226 LOAD_CONST              38 ('#e7e9eb')
+    139         226 LOAD_CONST              37 ('#2c2c2c')
    
-   140         228 LOAD_CONST               9 (1)
+    140         228 LOAD_CONST              39 ('#383838')
    
-   142         230 LOAD_CONST              39 ('#989898')
+    141         230 LOAD_CONST              40 ('#e7e9eb')
    
-   143         232 LOAD_CONST               9 (1)
+    142         232 LOAD_CONST               9 (1)
    
-   146         234 LOAD_CONST              36 ('#1c1c1c')
+    144         234 LOAD_CONST              41 ('#686868')
    
-   147         236 LOAD_CONST              35 ('#2c2c2c')
+    145         236 LOAD_CONST               9 (1)
    
-   148         238 LOAD_CONST              38 ('#e7e9eb')
+    148         238 LOAD_CONST              38 ('#1c1c1c')
    
-   149         240 LOAD_CONST               9 (1)
+    149         240 LOAD_CONST              37 ('#2c2c2c')
    
-   151         242 LOAD_CONST              40 ('#57c8ff')
+    150         242 LOAD_CONST              40 ('#e7e9eb')
    
-   152         244 LOAD_CONST              18 (2)
+    151         244 LOAD_CONST               9 (1)
    
-   145         246 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
-               248 BUILD_CONST_KEY_MAP      6
+    153         246 LOAD_CONST              42 ('#57c8ff')
    
-   133         250 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
-               252 BUILD_CONST_KEY_MAP      9
+    154         248 LOAD_CONST              26 (2)
    
-   157         254 LOAD_CONST               5 (13)
+    147         250 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                252 BUILD_CONST_KEY_MAP      6
    
-   158         256 LOAD_CONST              20 ((8, 8))
+    135         254 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                256 BUILD_CONST_KEY_MAP      9
    
-   160         258 LOAD_CONST              37 ('#292929')
+    159         258 LOAD_CONST               5 (13)
    
-   161         260 LOAD_CONST              37 ('#292929')
+    160         260 LOAD_CONST              20 ((8, 8))
    
-   162         262 LOAD_CONST              38 ('#e7e9eb')
+    162         262 LOAD_CONST              37 ('#2c2c2c')
    
-   163         264 LOAD_CONST               9 (1)
+    163         264 LOAD_CONST              39 ('#383838')
    
-   165         266 LOAD_CONST              39 ('#989898')
+    164         266 LOAD_CONST              40 ('#e7e9eb')
    
-   166         268 LOAD_CONST               9 (1)
+    165         268 LOAD_CONST               9 (1)
    
-   169         270 LOAD_CONST              36 ('#1c1c1c')
+    167         270 LOAD_CONST              41 ('#686868')
    
-   170         272 LOAD_CONST              35 ('#2c2c2c')
+    168         272 LOAD_CONST               9 (1)
    
-   171         274 LOAD_CONST              38 ('#e7e9eb')
+    171         274 LOAD_CONST              38 ('#1c1c1c')
    
-   172         276 LOAD_CONST               9 (1)
+    172         276 LOAD_CONST              37 ('#2c2c2c')
    
-   174         278 LOAD_CONST              40 ('#57c8ff')
+    173         278 LOAD_CONST              40 ('#e7e9eb')
    
-   175         280 LOAD_CONST              18 (2)
+    174         280 LOAD_CONST               9 (1)
    
-   168         282 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
-               284 BUILD_CONST_KEY_MAP      6
+    176         282 LOAD_CONST              42 ('#57c8ff')
    
-   156         286 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
-               288 BUILD_CONST_KEY_MAP      9
+    177         284 LOAD_CONST              26 (2)
    
-   180         290 LOAD_CONST              41 ('#404040')
+    170         286 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                288 BUILD_CONST_KEY_MAP      6
    
-   181         292 LOAD_CONST               9 (1)
+    158         290 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                292 BUILD_CONST_KEY_MAP      9
    
-   183         294 LOAD_CONST              28 (True)
+    182         294 LOAD_CONST              43 ('#404040')
    
-   179         296 LOAD_CONST              29 (('back', 'border_width', 'rounded'))
-               298 BUILD_CONST_KEY_MAP      3
+    183         296 LOAD_CONST               9 (1)
    
-    94         300 LOAD_CONST              30 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
-               302 BUILD_CONST_KEY_MAP      7
-               304 STORE_NAME               1 (win11_dark_theme)
+    185         298 LOAD_CONST              30 (True)
    
-   189         306 LOAD_CONST               0 ('back')
-               308 LOAD_CONST              23 ('#ffffff')
+    181         300 LOAD_CONST              31 (('back', 'border_width', 'rounded'))
+                302 BUILD_CONST_KEY_MAP      3
    
-   188         310 BUILD_MAP                1
+     95         304 LOAD_CONST              32 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
+                306 BUILD_CONST_KEY_MAP      7
+                308 STORE_NAME               1 (win11_dark_theme)
    
-   193         312 LOAD_CONST               2 ('transparent')
+    191         310 LOAD_CONST               0 ('back')
+                312 LOAD_CONST              21 ('#ffffff')
    
-   194         314 LOAD_CONST               3 ('#000000')
+    190         314 BUILD_MAP                1
    
-   192         316 LOAD_CONST               4 (('back', 'text_back'))
-               318 BUILD_CONST_KEY_MAP      2
+    195         316 LOAD_CONST               2 ('transparent')
    
-   198         320 LOAD_CONST              42 (11)
+    196         318 LOAD_CONST               3 ('#000000')
    
-   199         322 LOAD_CONST              43 ('#f6f5f4')
+    194         320 LOAD_CONST               4 (('back', 'text_back'))
+                322 BUILD_CONST_KEY_MAP      2
    
-   200         324 LOAD_CONST              44 ('#ccc6c1')
+    200         324 LOAD_CONST              44 (11)
    
-   201         326 LOAD_CONST              45 ('#2e3436')
+    201         326 LOAD_CONST              45 ('#f6f5f4')
    
-   202         328 LOAD_CONST              46 (1.3)
+    202         328 LOAD_CONST              46 ('#ccc6c1')
    
-   205         330 LOAD_CONST              47 ('#f8f8f7')
+    203         330 LOAD_CONST              47 ('#2e3436')
    
-   206         332 LOAD_CONST              48 ('#dad6d2')
+    204         332 LOAD_CONST              48 (1.3)
    
-   207         334 LOAD_CONST              45 ('#2e3436')
+    207         334 LOAD_CONST              49 ('#f8f8f7')
    
-   208         336 LOAD_CONST              46 (1.3)
+    208         336 LOAD_CONST              50 ('#dad6d2')
    
-   204         338 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
-               340 BUILD_CONST_KEY_MAP      4
+    209         338 LOAD_CONST              47 ('#2e3436')
    
-   212         342 LOAD_CONST              48 ('#dad6d2')
+    210         340 LOAD_CONST              48 (1.3)
    
-   213         344 LOAD_CONST              48 ('#dad6d2')
+    206         342 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+                344 BUILD_CONST_KEY_MAP      4
    
-   214         346 LOAD_CONST              45 ('#2e3436')
+    214         346 LOAD_CONST              50 ('#dad6d2')
    
-   215         348 LOAD_CONST              46 (1.3)
+    215         348 LOAD_CONST              50 ('#dad6d2')
    
-   211         350 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
-               352 BUILD_CONST_KEY_MAP      4
+    216         350 LOAD_CONST              47 ('#2e3436')
    
-   197         354 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
-               356 BUILD_CONST_KEY_MAP      7
+    217         352 LOAD_CONST              48 (1.3)
    
-   220         358 LOAD_CONST              49 (0)
+    213         354 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+                356 BUILD_CONST_KEY_MAP      4
    
-   221         360 LOAD_CONST              43 ('#f6f5f4')
+    199         358 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                360 BUILD_CONST_KEY_MAP      7
    
-   222         362 LOAD_CONST              50 ('#d5d0cc')
+    222         362 LOAD_CONST              18 (0)
    
-   223         364 LOAD_CONST              18 (2)
+    223         364 LOAD_CONST              45 ('#f6f5f4')
    
-   219         366 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width'))
-               368 BUILD_CONST_KEY_MAP      4
+    224         366 LOAD_CONST              51 ('#d5d0cc')
    
-   227         370 LOAD_CONST              42 (11)
+    225         368 LOAD_CONST               9 (1)
    
-   228         372 LOAD_CONST              51 ((5, 5))
+    226         370 LOAD_CONST              18 (0)
    
-   230         374 LOAD_CONST              23 ('#ffffff')
+    221         372 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width', 'padding'))
+                374 BUILD_CONST_KEY_MAP      5
    
-   231         376 LOAD_CONST              52 ('#cdc7c2')
+    230         376 LOAD_CONST              44 (11)
    
-   232         378 LOAD_CONST               3 ('#000000')
+    231         378 LOAD_CONST              52 ((5, 5))
    
-   233         380 LOAD_CONST               9 (1)
+    233         380 LOAD_CONST              21 ('#ffffff')
    
-   235         382 LOAD_CONST              53 ('#eaeaea')
+    234         382 LOAD_CONST              53 ('#cdc7c2')
    
-   236         384 LOAD_CONST              49 (0)
+    235         384 LOAD_CONST               3 ('#000000')
    
-   239         386 LOAD_CONST              23 ('#ffffff')
+    236         386 LOAD_CONST               9 (1)
    
-   240         388 LOAD_CONST              54 ('#3584e4')
+    238         388 LOAD_CONST              54 ('#eaeaea')
    
-   241         390 LOAD_CONST               3 ('#000000')
+    239         390 LOAD_CONST              18 (0)
    
-   242         392 LOAD_CONST               9 (1)
+    242         392 LOAD_CONST              21 ('#ffffff')
    
-   244         394 LOAD_CONST              55 ('#185fb4')
+    243         394 LOAD_CONST              55 ('#3584e4')
    
-   245         396 LOAD_CONST              49 (0)
+    244         396 LOAD_CONST               3 ('#000000')
    
-   238         398 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
-               400 BUILD_CONST_KEY_MAP      6
+    245         398 LOAD_CONST               9 (1)
    
-   226         402 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
-               404 BUILD_CONST_KEY_MAP      9
+    247         400 LOAD_CONST              56 ('#185fb4')
    
-   250         406 LOAD_CONST              51 ((5, 5))
+    248         402 LOAD_CONST              18 (0)
    
-   252         408 LOAD_CONST              49 (0)
+    241         404 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                406 BUILD_CONST_KEY_MAP      6
    
-   253         410 LOAD_CONST              23 ('#ffffff')
+    229         408 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                410 BUILD_CONST_KEY_MAP      9
    
-   254         412 LOAD_CONST              52 ('#cdc7c2')
+    253         412 LOAD_CONST              52 ((5, 5))
    
-   255         414 LOAD_CONST               3 ('#000000')
+    255         414 LOAD_CONST              18 (0)
    
-   256         416 LOAD_CONST               9 (1)
+    256         416 LOAD_CONST              21 ('#ffffff')
    
-   258         418 LOAD_CONST              53 ('#eaeaea')
+    257         418 LOAD_CONST              53 ('#cdc7c2')
    
-   259         420 LOAD_CONST              49 (0)
+    258         420 LOAD_CONST               3 ('#000000')
    
-   262         422 LOAD_CONST              23 ('#ffffff')
+    259         422 LOAD_CONST               9 (1)
    
-   263         424 LOAD_CONST              54 ('#3584e4')
+    261         424 LOAD_CONST              54 ('#eaeaea')
    
-   264         426 LOAD_CONST               3 ('#000000')
+    262         426 LOAD_CONST              18 (0)
    
-   265         428 LOAD_CONST               9 (1)
+    265         428 LOAD_CONST              21 ('#ffffff')
    
-   267         430 LOAD_CONST              55 ('#185fb4')
+    266         430 LOAD_CONST              55 ('#3584e4')
    
-   268         432 LOAD_CONST              49 (0)
+    267         432 LOAD_CONST               3 ('#000000')
    
-   261         434 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
-               436 BUILD_CONST_KEY_MAP      6
+    268         434 LOAD_CONST               9 (1)
    
-   249         438 LOAD_CONST              56 (('padding', 'radius', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
-               440 BUILD_CONST_KEY_MAP      9
+    270         436 LOAD_CONST              56 ('#185fb4')
    
-   273         442 LOAD_CONST              57 ('#d8d4d0')
+    271         438 LOAD_CONST              18 (0)
    
-   274         444 LOAD_CONST               9 (1)
+    264         440 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                442 BUILD_CONST_KEY_MAP      6
    
-   276         446 LOAD_CONST              28 (True)
+    252         444 LOAD_CONST              57 (('padding', 'radius', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                446 BUILD_CONST_KEY_MAP      9
    
-   272         448 LOAD_CONST              29 (('back', 'border_width', 'rounded'))
-               450 BUILD_CONST_KEY_MAP      3
+    276         448 LOAD_CONST              58 ('#d8d4d0')
    
-   187         452 LOAD_CONST              30 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
-               454 BUILD_CONST_KEY_MAP      7
-               456 STORE_NAME               2 (gtk_theme)
+    277         450 LOAD_CONST               9 (1)
    
-   282         458 LOAD_CONST               0 ('back')
-               460 LOAD_CONST              58 ('#353535')
+    279         452 LOAD_CONST              30 (True)
    
-   281         462 BUILD_MAP                1
+    275         454 LOAD_CONST              31 (('back', 'border_width', 'rounded'))
+                456 BUILD_CONST_KEY_MAP      3
    
-   286         464 LOAD_CONST               2 ('transparent')
+    189         458 LOAD_CONST              32 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
+                460 BUILD_CONST_KEY_MAP      7
+                462 STORE_NAME               2 (gtk_theme)
    
-   287         466 LOAD_CONST              23 ('#ffffff')
+    285         464 LOAD_CONST               0 ('back')
+                466 LOAD_CONST              59 ('#353535')
    
-   285         468 LOAD_CONST               4 (('back', 'text_back'))
-               470 BUILD_CONST_KEY_MAP      2
+    284         468 BUILD_MAP                1
    
-   291         472 LOAD_CONST              42 (11)
+    289         470 LOAD_CONST               2 ('transparent')
    
-   292         474 LOAD_CONST              58 ('#353535')
+    290         472 LOAD_CONST              21 ('#ffffff')
    
-   293         476 LOAD_CONST              59 ('#1b1b1b')
+    288         474 LOAD_CONST               4 (('back', 'text_back'))
+                476 BUILD_CONST_KEY_MAP      2
    
-   294         478 LOAD_CONST              60 ('#eeeeec')
+    294         478 LOAD_CONST              44 (11)
    
-   295         480 LOAD_CONST              46 (1.3)
+    295         480 LOAD_CONST              59 ('#353535')
    
-   298         482 LOAD_CONST              61 ('#373737')
+    296         482 LOAD_CONST              60 ('#1b1b1b')
    
-   299         484 LOAD_CONST              59 ('#1b1b1b')
+    297         484 LOAD_CONST              61 ('#eeeeec')
    
-   300         486 LOAD_CONST              60 ('#eeeeec')
+    298         486 LOAD_CONST              48 (1.3)
    
-   301         488 LOAD_CONST              46 (1.3)
+    301         488 LOAD_CONST              62 ('#373737')
    
-   297         490 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
-               492 BUILD_CONST_KEY_MAP      4
+    302         490 LOAD_CONST              60 ('#1b1b1b')
    
-   305         494 LOAD_CONST              62 ('#1e1e1e')
+    303         492 LOAD_CONST              61 ('#eeeeec')
    
-   306         496 LOAD_CONST              63 ('#282828')
+    304         494 LOAD_CONST              48 (1.3)
    
-   307         498 LOAD_CONST              60 ('#eeeeec')
+    300         496 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+                498 BUILD_CONST_KEY_MAP      4
    
-   308         500 LOAD_CONST              46 (1.3)
+    308         500 LOAD_CONST              63 ('#1e1e1e')
    
-   304         502 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
-               504 BUILD_CONST_KEY_MAP      4
+    309         502 LOAD_CONST              64 ('#282828')
    
-   290         506 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
-               508 BUILD_CONST_KEY_MAP      7
+    310         504 LOAD_CONST              61 ('#eeeeec')
    
-   313         510 LOAD_CONST              49 (0)
+    311         506 LOAD_CONST              48 (1.3)
    
-   314         512 LOAD_CONST              32 ('#313131')
+    307         508 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+                510 BUILD_CONST_KEY_MAP      4
    
-   315         514 LOAD_CONST              59 ('#1b1b1b')
+    293         512 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                514 BUILD_CONST_KEY_MAP      7
    
-   316         516 LOAD_CONST              18 (2)
+    316         516 LOAD_CONST              18 (0)
    
-   312         518 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width'))
-               520 BUILD_CONST_KEY_MAP      4
+    317         518 LOAD_CONST              34 ('#313131')
    
-   320         522 LOAD_CONST              42 (11)
+    318         520 LOAD_CONST              60 ('#1b1b1b')
    
-   321         524 LOAD_CONST              51 ((5, 5))
+    319         522 LOAD_CONST               9 (1)
    
-   323         526 LOAD_CONST              64 ('#2d2d2d')
+    320         524 LOAD_CONST              18 (0)
    
-   324         528 LOAD_CONST              65 ('#1f1f1f')
+    315         526 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width', 'padding'))
+                528 BUILD_CONST_KEY_MAP      5
    
-   325         530 LOAD_CONST              66 ('#cccccc')
+    324         530 LOAD_CONST              44 (11)
    
-   326         532 LOAD_CONST               9 (1)
+    325         532 LOAD_CONST              52 ((5, 5))
    
-   328         534 LOAD_CONST              53 ('#eaeaea')
+    327         534 LOAD_CONST              65 ('#2d2d2d')
    
-   329         536 LOAD_CONST              49 (0)
+    328         536 LOAD_CONST              66 ('#1f1f1f')
    
-   332         538 LOAD_CONST              64 ('#2d2d2d')
+    329         538 LOAD_CONST              67 ('#cccccc')
    
-   333         540 LOAD_CONST              54 ('#3584e4')
+    330         540 LOAD_CONST               9 (1)
    
-   334         542 LOAD_CONST              23 ('#ffffff')
+    332         542 LOAD_CONST              54 ('#eaeaea')
    
-   335         544 LOAD_CONST               9 (1)
+    333         544 LOAD_CONST              18 (0)
    
-   337         546 LOAD_CONST              54 ('#3584e4')
+    336         546 LOAD_CONST              65 ('#2d2d2d')
    
-   338         548 LOAD_CONST              49 (0)
+    337         548 LOAD_CONST              55 ('#3584e4')
    
-   331         550 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
-               552 BUILD_CONST_KEY_MAP      6
+    338         550 LOAD_CONST              21 ('#ffffff')
    
-   319         554 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
-               556 BUILD_CONST_KEY_MAP      9
+    339         552 LOAD_CONST               9 (1)
    
-   343         558 LOAD_CONST              51 ((5, 5))
+    341         554 LOAD_CONST              55 ('#3584e4')
    
-   345         560 LOAD_CONST              49 (0)
+    342         556 LOAD_CONST              18 (0)
    
-   346         562 LOAD_CONST              64 ('#2d2d2d')
+    335         558 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                560 BUILD_CONST_KEY_MAP      6
    
-   347         564 LOAD_CONST              65 ('#1f1f1f')
+    323         562 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                564 BUILD_CONST_KEY_MAP      9
    
-   348         566 LOAD_CONST              66 ('#cccccc')
+    347         566 LOAD_CONST              52 ((5, 5))
    
-   349         568 LOAD_CONST               9 (1)
+    349         568 LOAD_CONST              18 (0)
    
-   351         570 LOAD_CONST              53 ('#eaeaea')
+    350         570 LOAD_CONST              65 ('#2d2d2d')
    
-   352         572 LOAD_CONST              49 (0)
+    351         572 LOAD_CONST              66 ('#1f1f1f')
    
-   355         574 LOAD_CONST              64 ('#2d2d2d')
+    352         574 LOAD_CONST              67 ('#cccccc')
    
-   356         576 LOAD_CONST              54 ('#3584e4')
+    353         576 LOAD_CONST               9 (1)
    
-   357         578 LOAD_CONST              23 ('#ffffff')
+    355         578 LOAD_CONST              54 ('#eaeaea')
    
-   358         580 LOAD_CONST               9 (1)
+    356         580 LOAD_CONST              18 (0)
    
-   360         582 LOAD_CONST              54 ('#3584e4')
+    359         582 LOAD_CONST              65 ('#2d2d2d')
    
-   361         584 LOAD_CONST              49 (0)
+    360         584 LOAD_CONST              55 ('#3584e4')
    
-   354         586 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
-               588 BUILD_CONST_KEY_MAP      6
+    361         586 LOAD_CONST              21 ('#ffffff')
    
-   342         590 LOAD_CONST              56 (('padding', 'radius', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
-               592 BUILD_CONST_KEY_MAP      9
+    362         588 LOAD_CONST               9 (1)
    
-   366         594 LOAD_CONST              63 ('#282828')
+    364         590 LOAD_CONST              55 ('#3584e4')
    
-   367         596 LOAD_CONST               9 (1)
+    365         592 LOAD_CONST              18 (0)
    
-   369         598 LOAD_CONST              28 (True)
+    358         594 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                596 BUILD_CONST_KEY_MAP      6
    
-   365         600 LOAD_CONST              29 (('back', 'border_width', 'rounded'))
-               602 BUILD_CONST_KEY_MAP      3
+    346         598 LOAD_CONST              57 (('padding', 'radius', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                600 BUILD_CONST_KEY_MAP      9
    
-   280         604 LOAD_CONST              30 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
-               606 BUILD_CONST_KEY_MAP      7
-               608 STORE_NAME               3 (gtk_dark_theme)
+    370         602 LOAD_CONST              64 ('#282828')
    
-   375         610 LOAD_CONST               0 ('back')
-               612 LOAD_CONST              23 ('#ffffff')
+    371         604 LOAD_CONST               9 (1)
    
-   374         614 BUILD_MAP                1
+    373         606 LOAD_CONST              30 (True)
    
-   379         616 LOAD_CONST               2 ('transparent')
+    369         608 LOAD_CONST              31 (('back', 'border_width', 'rounded'))
+                610 BUILD_CONST_KEY_MAP      3
    
-   380         618 LOAD_CONST               3 ('#000000')
+    283         612 LOAD_CONST              32 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
+                614 BUILD_CONST_KEY_MAP      7
+                616 STORE_NAME               3 (gtk_dark_theme)
    
-   378         620 LOAD_CONST               4 (('back', 'text_back'))
-               622 BUILD_CONST_KEY_MAP      2
+    379         618 LOAD_CONST               0 ('back')
+                620 LOAD_CONST              21 ('#ffffff')
    
-   384         624 LOAD_CONST              67 (16)
+    378         622 BUILD_MAP                1
    
-   385         626 LOAD_CONST              23 ('#ffffff')
+    383         624 LOAD_CONST               2 ('transparent')
    
-   386         628 LOAD_CONST              68 ('#e3e5e7')
+    384         626 LOAD_CONST               3 ('#000000')
    
-   387         630 LOAD_CONST              21 ('#18191c')
+    382         628 LOAD_CONST               4 (('back', 'text_back'))
+                630 BUILD_CONST_KEY_MAP      2
    
-   388         632 LOAD_CONST               9 (1)
+    388         632 LOAD_CONST              68 (16)
    
-   391         634 LOAD_CONST              68 ('#e3e5e7')
+    389         634 LOAD_CONST              21 ('#ffffff')
    
-   392         636 LOAD_CONST              68 ('#e3e5e7')
+    390         636 LOAD_CONST              69 ('#e3e5e7')
    
-   393         638 LOAD_CONST              21 ('#18191c')
+    391         638 LOAD_CONST              23 ('#18191c')
    
-   394         640 LOAD_CONST               9 (1)
+    392         640 LOAD_CONST               9 (1)
    
-   390         642 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
-               644 BUILD_CONST_KEY_MAP      4
+    395         642 LOAD_CONST              69 ('#e3e5e7')
    
-   398         646 LOAD_CONST              69 ('#eceff0')
+    396         644 LOAD_CONST              69 ('#e3e5e7')
    
-   399         648 LOAD_CONST              68 ('#e3e5e7')
+    397         646 LOAD_CONST              23 ('#18191c')
    
-   400         650 LOAD_CONST              70 ('#6d7479')
+    398         648 LOAD_CONST               9 (1)
    
-   401         652 LOAD_CONST               9 (1)
+    394         650 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+                652 BUILD_CONST_KEY_MAP      4
    
-   397         654 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
-               656 BUILD_CONST_KEY_MAP      4
+    402         654 LOAD_CONST              70 ('#eceff0')
    
-   383         658 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
-               660 BUILD_CONST_KEY_MAP      7
+    403         656 LOAD_CONST              69 ('#e3e5e7')
    
-   406         662 LOAD_CONST              71 (18)
+    404         658 LOAD_CONST              71 ('#6d7479')
    
-   407         664 LOAD_CONST              72 ('#f6f7f8')
+    405         660 LOAD_CONST               9 (1)
    
-   408         666 LOAD_CONST              73 ('#f1f2f3')
+    401         662 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+                664 BUILD_CONST_KEY_MAP      4
    
-   409         668 LOAD_CONST              18 (2)
+    387         666 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                668 BUILD_CONST_KEY_MAP      7
    
-   405         670 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width'))
-               672 BUILD_CONST_KEY_MAP      4
+    410         670 LOAD_CONST              72 (18)
    
-   413         674 LOAD_CONST              67 (16)
+    411         672 LOAD_CONST              73 ('#f6f7f8')
    
-   414         676 LOAD_CONST              20 ((8, 8))
+    412         674 LOAD_CONST              74 ('#f1f2f3')
    
-   416         678 LOAD_CONST              23 ('#ffffff')
+    413         676 LOAD_CONST               9 (1)
    
-   417         680 LOAD_CONST              68 ('#e3e5e7')
+    414         678 LOAD_CONST              18 (0)
    
-   418         682 LOAD_CONST              21 ('#18191c')
+    409         680 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width', 'padding'))
+                682 BUILD_CONST_KEY_MAP      5
    
-   419         684 LOAD_CONST               9 (1)
+    418         684 LOAD_CONST              68 (16)
    
-   421         686 LOAD_CONST              53 ('#eaeaea')
+    419         686 LOAD_CONST              20 ((8, 8))
    
-   422         688 LOAD_CONST              49 (0)
+    421         688 LOAD_CONST              21 ('#ffffff')
    
-   425         690 LOAD_CONST              23 ('#ffffff')
+    422         690 LOAD_CONST              69 ('#e3e5e7')
    
-   426         692 LOAD_CONST              74 ('#ff6699')
+    423         692 LOAD_CONST              23 ('#18191c')
    
-   427         694 LOAD_CONST              21 ('#18191c')
+    424         694 LOAD_CONST               9 (1)
    
-   428         696 LOAD_CONST               9 (1)
+    426         696 LOAD_CONST              54 ('#eaeaea')
    
-   430         698 LOAD_CONST              55 ('#185fb4')
+    427         698 LOAD_CONST              18 (0)
    
-   431         700 LOAD_CONST              49 (0)
+    430         700 LOAD_CONST              21 ('#ffffff')
    
-   424         702 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
-               704 BUILD_CONST_KEY_MAP      6
+    431         702 LOAD_CONST              75 ('#ff6699')
    
-   412         706 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
-               708 BUILD_CONST_KEY_MAP      9
+    432         704 LOAD_CONST              23 ('#18191c')
    
-   436         710 LOAD_CONST              67 (16)
+    433         706 LOAD_CONST               9 (1)
    
-   437         712 LOAD_CONST              20 ((8, 8))
+    435         708 LOAD_CONST              56 ('#185fb4')
    
-   439         714 LOAD_CONST              23 ('#ffffff')
+    436         710 LOAD_CONST              18 (0)
    
-   440         716 LOAD_CONST              68 ('#e3e5e7')
+    429         712 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                714 BUILD_CONST_KEY_MAP      6
    
-   441         718 LOAD_CONST              21 ('#18191c')
+    417         716 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                718 BUILD_CONST_KEY_MAP      9
    
-   442         720 LOAD_CONST               9 (1)
+    441         720 LOAD_CONST              68 (16)
    
-   444         722 LOAD_CONST              53 ('#eaeaea')
+    442         722 LOAD_CONST              20 ((8, 8))
    
-   445         724 LOAD_CONST              49 (0)
+    444         724 LOAD_CONST              21 ('#ffffff')
    
-   448         726 LOAD_CONST              23 ('#ffffff')
+    445         726 LOAD_CONST              69 ('#e3e5e7')
    
-   449         728 LOAD_CONST              74 ('#ff6699')
+    446         728 LOAD_CONST              23 ('#18191c')
    
-   450         730 LOAD_CONST              21 ('#18191c')
+    447         730 LOAD_CONST               9 (1)
    
-   451         732 LOAD_CONST               9 (1)
+    449         732 LOAD_CONST              54 ('#eaeaea')
    
-   453         734 LOAD_CONST              55 ('#185fb4')
+    450         734 LOAD_CONST              18 (0)
    
-   454         736 LOAD_CONST              49 (0)
+    453         736 LOAD_CONST              21 ('#ffffff')
    
-   447         738 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
-               740 BUILD_CONST_KEY_MAP      6
+    454         738 LOAD_CONST              75 ('#ff6699')
    
-   435         742 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
-               744 BUILD_CONST_KEY_MAP      9
+    455         740 LOAD_CONST              23 ('#18191c')
    
-   459         746 LOAD_CONST              73 ('#f1f2f3')
+    456         742 LOAD_CONST               9 (1)
    
-   460         748 LOAD_CONST               9 (1)
+    458         744 LOAD_CONST              56 ('#185fb4')
    
-   462         750 LOAD_CONST              28 (True)
+    459         746 LOAD_CONST              18 (0)
    
-   458         752 LOAD_CONST              29 (('back', 'border_width', 'rounded'))
-               754 BUILD_CONST_KEY_MAP      3
+    452         748 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                750 BUILD_CONST_KEY_MAP      6
    
-   373         756 LOAD_CONST              30 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
-               758 BUILD_CONST_KEY_MAP      7
-               760 STORE_NAME               4 (bilibili_theme)
+    440         752 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                754 BUILD_CONST_KEY_MAP      9
    
-   468         762 LOAD_CONST               0 ('back')
-               764 LOAD_CONST              75 ('#17181a')
+    464         756 LOAD_CONST              74 ('#f1f2f3')
    
-   467         766 BUILD_MAP                1
+    465         758 LOAD_CONST               9 (1)
    
-   472         768 LOAD_CONST               2 ('transparent')
+    467         760 LOAD_CONST              30 (True)
    
-   473         770 LOAD_CONST              23 ('#ffffff')
+    463         762 LOAD_CONST              31 (('back', 'border_width', 'rounded'))
+                764 BUILD_CONST_KEY_MAP      3
    
-   471         772 LOAD_CONST               4 (('back', 'text_back'))
-               774 BUILD_CONST_KEY_MAP      2
+    377         766 LOAD_CONST              32 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
+                768 BUILD_CONST_KEY_MAP      7
+                770 STORE_NAME               4 (bilibili_theme)
    
-   477         776 LOAD_CONST              67 (16)
+    473         772 LOAD_CONST               0 ('back')
+                774 LOAD_CONST              76 ('#17181a')
    
-   478         778 LOAD_CONST              76 ('#242628')
+    472         776 BUILD_MAP                1
    
-   479         780 LOAD_CONST              77 ('#2f3134')
+    477         778 LOAD_CONST               2 ('transparent')
    
-   480         782 LOAD_CONST              78 ('#dcdee0')
+    478         780 LOAD_CONST              21 ('#ffffff')
    
-   481         784 LOAD_CONST               9 (1)
+    476         782 LOAD_CONST               4 (('back', 'text_back'))
+                784 BUILD_CONST_KEY_MAP      2
    
-   484         786 LOAD_CONST              77 ('#2f3134')
+    482         786 LOAD_CONST              68 (16)
    
-   485         788 LOAD_CONST              77 ('#2f3134')
+    483         788 LOAD_CONST              77 ('#242628')
    
-   486         790 LOAD_CONST              78 ('#dcdee0')
+    484         790 LOAD_CONST              78 ('#2f3134')
    
-   487         792 LOAD_CONST               9 (1)
+    485         792 LOAD_CONST              79 ('#dcdee0')
    
-   483         794 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
-               796 BUILD_CONST_KEY_MAP      4
+    486         794 LOAD_CONST               9 (1)
    
-   491         798 LOAD_CONST              79 ('#26282a')
+    489         796 LOAD_CONST              78 ('#2f3134')
    
-   492         800 LOAD_CONST              77 ('#2f3134')
+    490         798 LOAD_CONST              78 ('#2f3134')
    
-   493         802 LOAD_CONST              80 ('#a9abad')
+    491         800 LOAD_CONST              79 ('#dcdee0')
    
-   494         804 LOAD_CONST               9 (1)
+    492         802 LOAD_CONST               9 (1)
    
-   490         806 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
-               808 BUILD_CONST_KEY_MAP      4
+    488         804 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+                806 BUILD_CONST_KEY_MAP      4
    
-   476         810 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
-               812 BUILD_CONST_KEY_MAP      7
+    496         808 LOAD_CONST              80 ('#26282a')
    
-   499         814 LOAD_CONST              71 (18)
+    497         810 LOAD_CONST              78 ('#2f3134')
    
-   500         816 LOAD_CONST              81 ('#1e2022')
+    498         812 LOAD_CONST              81 ('#a9abad')
    
-   501         818 LOAD_CONST              82 ('#232527')
+    499         814 LOAD_CONST               9 (1)
    
-   502         820 LOAD_CONST              18 (2)
+    495         816 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+                818 BUILD_CONST_KEY_MAP      4
    
-   498         822 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width'))
-               824 BUILD_CONST_KEY_MAP      4
+    481         820 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                822 BUILD_CONST_KEY_MAP      7
    
-   506         826 LOAD_CONST              67 (16)
+    504         824 LOAD_CONST              72 (18)
    
-   507         828 LOAD_CONST              20 ((8, 8))
+    505         826 LOAD_CONST              82 ('#1e2022')
    
-   509         830 LOAD_CONST              75 ('#17181a')
+    506         828 LOAD_CONST              83 ('#232527')
    
-   510         832 LOAD_CONST              77 ('#2f3134')
+    507         830 LOAD_CONST               9 (1)
    
-   511         834 LOAD_CONST              38 ('#e7e9eb')
+    508         832 LOAD_CONST              18 (0)
    
-   512         836 LOAD_CONST               9 (1)
+    503         834 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width', 'padding'))
+                836 BUILD_CONST_KEY_MAP      5
    
-   514         838 LOAD_CONST              53 ('#eaeaea')
+    512         838 LOAD_CONST              68 (16)
    
-   515         840 LOAD_CONST              49 (0)
+    513         840 LOAD_CONST              20 ((8, 8))
    
-   518         842 LOAD_CONST              75 ('#17181a')
+    515         842 LOAD_CONST              76 ('#17181a')
    
-   519         844 LOAD_CONST              83 ('#d44e7d')
+    516         844 LOAD_CONST              78 ('#2f3134')
    
-   520         846 LOAD_CONST              38 ('#e7e9eb')
+    517         846 LOAD_CONST              40 ('#e7e9eb')
    
-   521         848 LOAD_CONST               9 (1)
+    518         848 LOAD_CONST               9 (1)
    
-   523         850 LOAD_CONST              83 ('#d44e7d')
+    520         850 LOAD_CONST              54 ('#eaeaea')
    
-   524         852 LOAD_CONST              49 (0)
+    521         852 LOAD_CONST              18 (0)
    
-   517         854 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
-               856 BUILD_CONST_KEY_MAP      6
+    524         854 LOAD_CONST              76 ('#17181a')
    
-   505         858 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
-               860 BUILD_CONST_KEY_MAP      9
+    525         856 LOAD_CONST              84 ('#d44e7d')
    
-   529         862 LOAD_CONST              67 (16)
+    526         858 LOAD_CONST              40 ('#e7e9eb')
    
-   530         864 LOAD_CONST              20 ((8, 8))
+    527         860 LOAD_CONST               9 (1)
    
-   532         866 LOAD_CONST              75 ('#17181a')
+    529         862 LOAD_CONST              84 ('#d44e7d')
    
-   533         868 LOAD_CONST              77 ('#2f3134')
+    530         864 LOAD_CONST              18 (0)
    
-   534         870 LOAD_CONST              38 ('#e7e9eb')
+    523         866 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                868 BUILD_CONST_KEY_MAP      6
    
-   535         872 LOAD_CONST               9 (1)
+    511         870 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                872 BUILD_CONST_KEY_MAP      9
    
-   537         874 LOAD_CONST              53 ('#eaeaea')
+    535         874 LOAD_CONST              68 (16)
    
-   538         876 LOAD_CONST              49 (0)
+    536         876 LOAD_CONST              20 ((8, 8))
    
-   541         878 LOAD_CONST              75 ('#17181a')
+    538         878 LOAD_CONST              76 ('#17181a')
    
-   542         880 LOAD_CONST              83 ('#d44e7d')
+    539         880 LOAD_CONST              78 ('#2f3134')
    
-   543         882 LOAD_CONST              38 ('#e7e9eb')
+    540         882 LOAD_CONST              40 ('#e7e9eb')
    
-   544         884 LOAD_CONST               9 (1)
+    541         884 LOAD_CONST               9 (1)
    
-   546         886 LOAD_CONST              83 ('#d44e7d')
+    543         886 LOAD_CONST              54 ('#eaeaea')
    
-   547         888 LOAD_CONST              49 (0)
+    544         888 LOAD_CONST              18 (0)
    
-   540         890 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
-               892 BUILD_CONST_KEY_MAP      6
+    547         890 LOAD_CONST              76 ('#17181a')
    
-   528         894 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
-               896 BUILD_CONST_KEY_MAP      9
+    548         892 LOAD_CONST              84 ('#d44e7d')
    
-   552         898 LOAD_CONST              82 ('#232527')
+    549         894 LOAD_CONST              40 ('#e7e9eb')
    
-   553         900 LOAD_CONST               9 (1)
+    550         896 LOAD_CONST               9 (1)
    
-   555         902 LOAD_CONST              28 (True)
+    552         898 LOAD_CONST              84 ('#d44e7d')
    
-   551         904 LOAD_CONST              29 (('back', 'border_width', 'rounded'))
-               906 BUILD_CONST_KEY_MAP      3
+    553         900 LOAD_CONST              18 (0)
    
-   466         908 LOAD_CONST              30 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
-               910 BUILD_CONST_KEY_MAP      7
-               912 STORE_NAME               5 (bilibili_dark_theme)
+    546         902 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+                904 BUILD_CONST_KEY_MAP      6
    
-   561         914 LOAD_CONST               0 ('back')
-               916 LOAD_CONST              23 ('#ffffff')
+    534         906 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+                908 BUILD_CONST_KEY_MAP      9
    
-   560         918 BUILD_MAP                1
+    558         910 LOAD_CONST              83 ('#232527')
    
-   565         920 LOAD_CONST               2 ('transparent')
+    559         912 LOAD_CONST               9 (1)
    
-   566         922 LOAD_CONST               3 ('#000000')
+    561         914 LOAD_CONST              30 (True)
    
-   564         924 LOAD_CONST               4 (('back', 'text_back'))
-               926 BUILD_CONST_KEY_MAP      2
+    557         916 LOAD_CONST              31 (('back', 'border_width', 'rounded'))
+                918 BUILD_CONST_KEY_MAP      3
    
-   570         928 LOAD_CONST              49 (0)
+    471         920 LOAD_CONST              32 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
+                922 BUILD_CONST_KEY_MAP      7
+                924 STORE_NAME               5 (bilibili_dark_theme)
    
-   571         930 LOAD_CONST              84 ('#eeeeee')
+    567         926 LOAD_CONST               0 ('back')
+                928 LOAD_CONST              21 ('#ffffff')
    
-   572         932 LOAD_CONST              66 ('#cccccc')
+    566         930 BUILD_MAP                1
    
-   573         934 LOAD_CONST               3 ('#000000')
+    571         932 LOAD_CONST               2 ('transparent')
    
-   574         936 LOAD_CONST               9 (1)
+    572         934 LOAD_CONST               3 ('#000000')
    
-   577         938 LOAD_CONST              85 ('#666666')
+    570         936 LOAD_CONST               4 (('back', 'text_back'))
+                938 BUILD_CONST_KEY_MAP      2
    
-   578         940 LOAD_CONST              85 ('#666666')
+    576         940 LOAD_CONST              18 (0)
    
-   579         942 LOAD_CONST              23 ('#ffffff')
+    577         942 LOAD_CONST              85 ('#eeeeee')
    
-   580         944 LOAD_CONST               9 (1)
+    578         944 LOAD_CONST              67 ('#cccccc')
    
-   576         946 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
-               948 BUILD_CONST_KEY_MAP      4
+    579         946 LOAD_CONST               3 ('#000000')
    
-   584         950 LOAD_CONST              86 ('#333333')
+    580         948 LOAD_CONST               9 (1)
    
-   585         952 LOAD_CONST              86 ('#333333')
+    583         950 LOAD_CONST              86 ('#666666')
    
-   586         954 LOAD_CONST              23 ('#ffffff')
+    584         952 LOAD_CONST              86 ('#666666')
    
-   587         956 LOAD_CONST               9 (1)
+    585         954 LOAD_CONST              21 ('#ffffff')
    
-   583         958 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
-               960 BUILD_CONST_KEY_MAP      4
+    586         956 LOAD_CONST               9 (1)
    
-   569         962 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
-               964 BUILD_CONST_KEY_MAP      7
+    582         958 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+                960 BUILD_CONST_KEY_MAP      4
    
-   592         966 LOAD_CONST              49 (0)
+    590         962 LOAD_CONST              87 ('#333333')
    
-   593         968 LOAD_CONST              23 ('#ffffff')
+    591         964 LOAD_CONST              87 ('#333333')
    
-   594         970 LOAD_CONST              87 ('#bfbfbf')
+    592         966 LOAD_CONST              21 ('#ffffff')
    
-   595         972 LOAD_CONST              18 (2)
+    593         968 LOAD_CONST               9 (1)
    
-   591         974 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width'))
-               976 BUILD_CONST_KEY_MAP      4
+    589         970 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+                972 BUILD_CONST_KEY_MAP      4
    
-   599         978 LOAD_CONST              49 (0)
+    575         974 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+                976 BUILD_CONST_KEY_MAP      7
    
-   600         980 LOAD_CONST              88 ((3, 3))
+    598         978 LOAD_CONST              18 (0)
    
-   602         982 LOAD_CONST              23 ('#ffffff')
+    599         980 LOAD_CONST              21 ('#ffffff')
    
-   603         984 LOAD_CONST              89 ('#999999')
+    600         982 LOAD_CONST              88 ('#bfbfbf')
    
-   604         986 LOAD_CONST               3 ('#000000')
+    601         984 LOAD_CONST               9 (1)
    
-   605         988 LOAD_CONST               9 (1)
+    602         986 LOAD_CONST              18 (0)
    
-   607         990 LOAD_CONST              23 ('#ffffff')
+    597         988 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width', 'padding'))
+                990 BUILD_CONST_KEY_MAP      5
    
-   608         992 LOAD_CONST              49 (0)
+    606         992 LOAD_CONST              18 (0)
    
-   611         994 LOAD_CONST              23 ('#ffffff')
+    607         994 LOAD_CONST              89 ((3, 3))
    
-   612         996 LOAD_CONST              90 ('#00aedb')
+    609         996 LOAD_CONST              21 ('#ffffff')
    
-   613         998 LOAD_CONST               3 ('#000000')
+    610         998 LOAD_CONST              90 ('#999999')
    
-   614        1000 LOAD_CONST               9 (1)
+    611        1000 LOAD_CONST               3 ('#000000')
    
-   616        1002 LOAD_CONST              23 ('#ffffff')
+    612        1002 LOAD_CONST               9 (1)
    
-   617        1004 LOAD_CONST              49 (0)
+    614        1004 LOAD_CONST              21 ('#ffffff')
    
-   610        1006 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
-              1008 BUILD_CONST_KEY_MAP      6
+    615        1006 LOAD_CONST              18 (0)
    
-   598        1010 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
-              1012 BUILD_CONST_KEY_MAP      9
+    618        1008 LOAD_CONST              21 ('#ffffff')
    
-   622        1014 LOAD_CONST              49 (0)
+    619        1010 LOAD_CONST              91 ('#00aedb')
    
-   623        1016 LOAD_CONST              88 ((3, 3))
+    620        1012 LOAD_CONST               3 ('#000000')
    
-   625        1018 LOAD_CONST              23 ('#ffffff')
+    621        1014 LOAD_CONST               9 (1)
    
-   626        1020 LOAD_CONST              89 ('#999999')
+    623        1016 LOAD_CONST              21 ('#ffffff')
    
-   627        1022 LOAD_CONST               3 ('#000000')
+    624        1018 LOAD_CONST              18 (0)
    
-   628        1024 LOAD_CONST               9 (1)
+    617        1020 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               1022 BUILD_CONST_KEY_MAP      6
    
-   630        1026 LOAD_CONST              23 ('#ffffff')
+    605        1024 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               1026 BUILD_CONST_KEY_MAP      9
    
-   631        1028 LOAD_CONST              49 (0)
+    629        1028 LOAD_CONST              18 (0)
    
-   634        1030 LOAD_CONST              23 ('#ffffff')
+    630        1030 LOAD_CONST              89 ((3, 3))
    
-   635        1032 LOAD_CONST              90 ('#00aedb')
+    632        1032 LOAD_CONST              21 ('#ffffff')
    
-   636        1034 LOAD_CONST               3 ('#000000')
+    633        1034 LOAD_CONST              90 ('#999999')
    
-   637        1036 LOAD_CONST               9 (1)
+    634        1036 LOAD_CONST               3 ('#000000')
    
-   639        1038 LOAD_CONST              23 ('#ffffff')
+    635        1038 LOAD_CONST               9 (1)
    
-   640        1040 LOAD_CONST              49 (0)
+    637        1040 LOAD_CONST              21 ('#ffffff')
    
-   633        1042 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
-              1044 BUILD_CONST_KEY_MAP      6
+    638        1042 LOAD_CONST              18 (0)
    
-   621        1046 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
-              1048 BUILD_CONST_KEY_MAP      9
+    641        1044 LOAD_CONST              21 ('#ffffff')
    
-   645        1050 LOAD_CONST              89 ('#999999')
+    642        1046 LOAD_CONST              91 ('#00aedb')
    
-   646        1052 LOAD_CONST               9 (1)
+    643        1048 LOAD_CONST               3 ('#000000')
    
-   648        1054 LOAD_CONST              28 (True)
+    644        1050 LOAD_CONST               9 (1)
    
-   644        1056 LOAD_CONST              29 (('back', 'border_width', 'rounded'))
-              1058 BUILD_CONST_KEY_MAP      3
+    646        1052 LOAD_CONST              21 ('#ffffff')
    
-   559        1060 LOAD_CONST              30 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
-              1062 BUILD_CONST_KEY_MAP      7
-              1064 STORE_NAME               6 (metro_theme)
+    647        1054 LOAD_CONST              18 (0)
    
-   654        1066 LOAD_CONST               0 ('back')
-              1068 LOAD_CONST              91 ('#111111')
+    640        1056 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               1058 BUILD_CONST_KEY_MAP      6
    
-   653        1070 BUILD_MAP                1
+    628        1060 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               1062 BUILD_CONST_KEY_MAP      9
    
-   658        1072 LOAD_CONST               2 ('transparent')
+    652        1064 LOAD_CONST              90 ('#999999')
    
-   659        1074 LOAD_CONST               3 ('#000000')
+    653        1066 LOAD_CONST               9 (1)
    
-   657        1076 LOAD_CONST               4 (('back', 'text_back'))
-              1078 BUILD_CONST_KEY_MAP      2
+    655        1068 LOAD_CONST              30 (True)
    
-   663        1080 LOAD_CONST              49 (0)
+    651        1070 LOAD_CONST              31 (('back', 'border_width', 'rounded'))
+               1072 BUILD_CONST_KEY_MAP      3
    
-   664        1082 LOAD_CONST              92 ('#222222')
+    565        1074 LOAD_CONST              32 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
+               1076 BUILD_CONST_KEY_MAP      7
+               1078 STORE_NAME               6 (metro_theme)
    
-   665        1084 LOAD_CONST              93 ('#444444')
+    661        1080 LOAD_CONST               0 ('back')
+               1082 LOAD_CONST              92 ('#111111')
    
-   666        1086 LOAD_CONST              23 ('#ffffff')
+    660        1084 BUILD_MAP                1
    
-   667        1088 LOAD_CONST               9 (1)
+    665        1086 LOAD_CONST               2 ('transparent')
    
-   670        1090 LOAD_CONST              94 ('#aaaaaa')
+    666        1088 LOAD_CONST               3 ('#000000')
    
-   671        1092 LOAD_CONST              94 ('#aaaaaa')
+    664        1090 LOAD_CONST               4 (('back', 'text_back'))
+               1092 BUILD_CONST_KEY_MAP      2
    
-   672        1094 LOAD_CONST               3 ('#000000')
+    670        1094 LOAD_CONST              18 (0)
    
-   673        1096 LOAD_CONST               9 (1)
+    671        1096 LOAD_CONST              93 ('#222222')
    
-   669        1098 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
-              1100 BUILD_CONST_KEY_MAP      4
+    672        1098 LOAD_CONST              94 ('#444444')
    
-   677        1102 LOAD_CONST              84 ('#eeeeee')
+    673        1100 LOAD_CONST              21 ('#ffffff')
    
-   678        1104 LOAD_CONST              84 ('#eeeeee')
+    674        1102 LOAD_CONST               9 (1)
    
-   679        1106 LOAD_CONST               3 ('#000000')
+    677        1104 LOAD_CONST              95 ('#aaaaaa')
    
-   680        1108 LOAD_CONST               9 (1)
+    678        1106 LOAD_CONST              95 ('#aaaaaa')
    
-   676        1110 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
-              1112 BUILD_CONST_KEY_MAP      4
+    679        1108 LOAD_CONST               3 ('#000000')
    
-   662        1114 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
-              1116 BUILD_CONST_KEY_MAP      7
+    680        1110 LOAD_CONST               9 (1)
    
-   685        1118 LOAD_CONST              49 (0)
+    676        1112 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+               1114 BUILD_CONST_KEY_MAP      4
    
-   686        1120 LOAD_CONST              91 ('#111111')
+    684        1116 LOAD_CONST              85 ('#eeeeee')
    
-   687        1122 LOAD_CONST              61 ('#373737')
+    685        1118 LOAD_CONST              85 ('#eeeeee')
    
-   688        1124 LOAD_CONST              18 (2)
+    686        1120 LOAD_CONST               3 ('#000000')
    
-   684        1126 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width'))
-              1128 BUILD_CONST_KEY_MAP      4
+    687        1122 LOAD_CONST               9 (1)
    
-   692        1130 LOAD_CONST              49 (0)
+    683        1124 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+               1126 BUILD_CONST_KEY_MAP      4
    
-   693        1132 LOAD_CONST              88 ((3, 3))
+    669        1128 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+               1130 BUILD_CONST_KEY_MAP      7
    
-   695        1134 LOAD_CONST              91 ('#111111')
+    692        1132 LOAD_CONST              18 (0)
    
-   696        1136 LOAD_CONST              89 ('#999999')
+    693        1134 LOAD_CONST              92 ('#111111')
    
-   697        1138 LOAD_CONST              23 ('#ffffff')
+    694        1136 LOAD_CONST              62 ('#373737')
    
-   698        1140 LOAD_CONST               9 (1)
+    695        1138 LOAD_CONST               9 (1)
    
-   700        1142 LOAD_CONST               3 ('#000000')
+    696        1140 LOAD_CONST              18 (0)
    
-   701        1144 LOAD_CONST              49 (0)
+    691        1142 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width', 'padding'))
+               1144 BUILD_CONST_KEY_MAP      5
    
-   704        1146 LOAD_CONST              91 ('#111111')
+    700        1146 LOAD_CONST              18 (0)
    
-   705        1148 LOAD_CONST              90 ('#00aedb')
+    701        1148 LOAD_CONST              89 ((3, 3))
    
-   706        1150 LOAD_CONST              23 ('#ffffff')
+    703        1150 LOAD_CONST              92 ('#111111')
    
-   707        1152 LOAD_CONST               9 (1)
+    704        1152 LOAD_CONST              90 ('#999999')
    
-   709        1154 LOAD_CONST               3 ('#000000')
+    705        1154 LOAD_CONST              21 ('#ffffff')
    
-   710        1156 LOAD_CONST              49 (0)
+    706        1156 LOAD_CONST               9 (1)
    
-   703        1158 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
-              1160 BUILD_CONST_KEY_MAP      6
+    708        1158 LOAD_CONST               3 ('#000000')
    
-   691        1162 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
-              1164 BUILD_CONST_KEY_MAP      9
+    709        1160 LOAD_CONST              18 (0)
    
-   715        1166 LOAD_CONST              49 (0)
+    712        1162 LOAD_CONST              92 ('#111111')
    
-   716        1168 LOAD_CONST              88 ((3, 3))
+    713        1164 LOAD_CONST              91 ('#00aedb')
    
-   718        1170 LOAD_CONST              91 ('#111111')
+    714        1166 LOAD_CONST              21 ('#ffffff')
    
-   719        1172 LOAD_CONST              89 ('#999999')
+    715        1168 LOAD_CONST               9 (1)
    
-   720        1174 LOAD_CONST              23 ('#ffffff')
+    717        1170 LOAD_CONST               3 ('#000000')
    
-   721        1176 LOAD_CONST               9 (1)
+    718        1172 LOAD_CONST              18 (0)
    
-   723        1178 LOAD_CONST               3 ('#000000')
+    711        1174 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               1176 BUILD_CONST_KEY_MAP      6
    
-   724        1180 LOAD_CONST              49 (0)
+    699        1178 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               1180 BUILD_CONST_KEY_MAP      9
    
-   727        1182 LOAD_CONST              91 ('#111111')
+    723        1182 LOAD_CONST              18 (0)
    
-   728        1184 LOAD_CONST              90 ('#00aedb')
+    724        1184 LOAD_CONST              89 ((3, 3))
    
-   729        1186 LOAD_CONST              23 ('#ffffff')
+    726        1186 LOAD_CONST              92 ('#111111')
    
-   730        1188 LOAD_CONST               9 (1)
+    727        1188 LOAD_CONST              90 ('#999999')
    
-   732        1190 LOAD_CONST               3 ('#000000')
+    728        1190 LOAD_CONST              21 ('#ffffff')
    
-   733        1192 LOAD_CONST              49 (0)
+    729        1192 LOAD_CONST               9 (1)
    
-   726        1194 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
-              1196 BUILD_CONST_KEY_MAP      6
+    731        1194 LOAD_CONST               3 ('#000000')
    
-   714        1198 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
-              1200 BUILD_CONST_KEY_MAP      9
+    732        1196 LOAD_CONST              18 (0)
    
-   738        1202 LOAD_CONST              89 ('#999999')
+    735        1198 LOAD_CONST              92 ('#111111')
    
-   739        1204 LOAD_CONST               9 (1)
+    736        1200 LOAD_CONST              91 ('#00aedb')
    
-   741        1206 LOAD_CONST              95 (False)
+    737        1202 LOAD_CONST              21 ('#ffffff')
    
-   737        1208 LOAD_CONST              29 (('back', 'border_width', 'rounded'))
-              1210 BUILD_CONST_KEY_MAP      3
+    738        1204 LOAD_CONST               9 (1)
    
-   652        1212 LOAD_CONST              30 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
-              1214 BUILD_CONST_KEY_MAP      7
-              1216 STORE_NAME               7 (metro_dark_theme)
+    740        1206 LOAD_CONST               3 ('#000000')
    
-   746        1218 LOAD_CONST              96 (<code object get_default_theme, file "D:\tkadw\tkadw\windows\theme.py", line 746>)
-              1220 MAKE_FUNCTION            0
-              1222 STORE_NAME               8 (get_default_theme)
+    741        1208 LOAD_CONST              18 (0)
    
-   755        1224 LOAD_CONST              97 (<code object _set_default_theme, file "D:\tkadw\tkadw\windows\theme.py", line 755>)
-              1226 MAKE_FUNCTION            0
-              1228 STORE_NAME               9 (_set_default_theme)
+    734        1210 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               1212 BUILD_CONST_KEY_MAP      6
    
-   761        1230 LOAD_CONST             132 (('system',))
-              1232 LOAD_CONST              99 (<code object set_default_theme, file "D:\tkadw\tkadw\windows\theme.py", line 761>)
-              1234 MAKE_FUNCTION            1 (defaults)
-              1236 STORE_NAME              10 (set_default_theme)
+    722        1214 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               1216 BUILD_CONST_KEY_MAP      9
    
-   827        1238 PUSH_NULL
-              1240 LOAD_NAME               10 (set_default_theme)
-              1242 LOAD_CONST             100 ('win11')
-              1244 PRECALL                  1
-              1248 CALL                     1
-              1258 POP_TOP
+    746        1218 LOAD_CONST              90 ('#999999')
    
-   830        1260 LOAD_CONST              49 (0)
-              1262 LOAD_CONST             101 (('Adw',))
-              1264 IMPORT_NAME             11 (tkadw.windows.widgets.adw)
-              1266 IMPORT_FROM             12 (Adw)
-              1268 STORE_NAME              12 (Adw)
-              1270 POP_TOP
+    747        1220 LOAD_CONST               9 (1)
    
-   833        1272 PUSH_NULL
-              1274 LOAD_BUILD_CLASS
-              1276 LOAD_CONST             102 (<code object Adwite, file "D:\tkadw\tkadw\windows\theme.py", line 833>)
-              1278 MAKE_FUNCTION            0
-              1280 LOAD_CONST             103 ('Adwite')
-              1282 LOAD_NAME               12 (Adw)
-              1284 PRECALL                  3
-              1288 CALL                     3
-              1298 STORE_NAME              13 (Adwite)
+    749        1222 LOAD_CONST              96 (False)
    
-   847        1300 LOAD_CONST              49 (0)
-              1302 LOAD_CONST             104 (('AdwLabel',))
-              1304 IMPORT_NAME             14 (tkadw.windows.widgets)
-              1306 IMPORT_FROM             15 (AdwLabel)
-              1308 STORE_NAME              15 (AdwLabel)
-              1310 POP_TOP
+    745        1224 LOAD_CONST              31 (('back', 'border_width', 'rounded'))
+               1226 BUILD_CONST_KEY_MAP      3
    
-   850        1312 PUSH_NULL
-              1314 LOAD_BUILD_CLASS
-              1316 LOAD_CONST             105 (<code object AdwTLabel, file "D:\tkadw\tkadw\windows\theme.py", line 850>)
-              1318 MAKE_FUNCTION            0
-              1320 LOAD_CONST             106 ('AdwTLabel')
-              1322 LOAD_NAME               15 (AdwLabel)
-              1324 PRECALL                  3
-              1328 CALL                     3
-              1338 STORE_NAME              16 (AdwTLabel)
+    659        1228 LOAD_CONST              32 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
+               1230 BUILD_CONST_KEY_MAP      7
+               1232 STORE_NAME               7 (metro_dark_theme)
    
-   855        1340 LOAD_CONST              49 (0)
-              1342 LOAD_CONST             107 (('AdwDrawRoundButton3',))
-              1344 IMPORT_NAME             17 (tkadw.windows.canvas.button)
-              1346 IMPORT_FROM             18 (AdwDrawRoundButton3)
-              1348 STORE_NAME              18 (AdwDrawRoundButton3)
-              1350 POP_TOP
+    755        1234 LOAD_CONST               0 ('back')
+               1236 LOAD_CONST              97 ('#f0f0f0')
    
-   858        1352 PUSH_NULL
-              1354 LOAD_BUILD_CLASS
-              1356 LOAD_CONST             108 (<code object AdwTButton, file "D:\tkadw\tkadw\windows\theme.py", line 858>)
-              1358 MAKE_FUNCTION            0
-              1360 LOAD_CONST             109 ('AdwTButton')
-              1362 LOAD_NAME               18 (AdwDrawRoundButton3)
-              1364 PRECALL                  3
-              1368 CALL                     3
-              1378 STORE_NAME              19 (AdwTButton)
+    754        1238 BUILD_MAP                1
    
-   863        1380 LOAD_CONST              49 (0)
-              1382 LOAD_CONST             110 (('AdwDrawRoundEntry3',))
-              1384 IMPORT_NAME             20 (tkadw.windows.canvas.entry)
-              1386 IMPORT_FROM             21 (AdwDrawRoundEntry3)
-              1388 STORE_NAME              21 (AdwDrawRoundEntry3)
-              1390 POP_TOP
+    759        1240 LOAD_CONST               2 ('transparent')
    
-   866        1392 PUSH_NULL
-              1394 LOAD_BUILD_CLASS
-              1396 LOAD_CONST             111 (<code object AdwTEntry, file "D:\tkadw\tkadw\windows\theme.py", line 866>)
-              1398 MAKE_FUNCTION            0
-              1400 LOAD_CONST             112 ('AdwTEntry')
-              1402 LOAD_NAME               21 (AdwDrawRoundEntry3)
-              1404 PRECALL                  3
-              1408 CALL                     3
-              1418 STORE_NAME              22 (AdwTEntry)
+    760        1242 LOAD_CONST               3 ('#000000')
    
-   871        1420 LOAD_CONST              49 (0)
-              1422 LOAD_CONST             113 (('AdwDrawRoundText3',))
-              1424 IMPORT_NAME             23 (tkadw.windows.canvas.textbox)
-              1426 IMPORT_FROM             24 (AdwDrawRoundText3)
-              1428 STORE_NAME              24 (AdwDrawRoundText3)
-              1430 POP_TOP
+    758        1244 LOAD_CONST               4 (('back', 'text_back'))
+               1246 BUILD_CONST_KEY_MAP      2
    
-   874        1432 PUSH_NULL
-              1434 LOAD_BUILD_CLASS
-              1436 LOAD_CONST             114 (<code object AdwTText, file "D:\tkadw\tkadw\windows\theme.py", line 874>)
-              1438 MAKE_FUNCTION            0
-              1440 LOAD_CONST             115 ('AdwTText')
-              1442 LOAD_NAME               24 (AdwDrawRoundText3)
-              1444 PRECALL                  3
-              1448 CALL                     3
-              1458 STORE_NAME              25 (AdwTText)
+    764        1248 LOAD_CONST              18 (0)
    
-   879        1460 LOAD_CONST              49 (0)
-              1462 LOAD_CONST             116 (('AdwDrawRoundFrame3',))
-              1464 IMPORT_NAME             26 (tkadw.windows.canvas.frame)
-              1466 IMPORT_FROM             27 (AdwDrawRoundFrame3)
-              1468 STORE_NAME              27 (AdwDrawRoundFrame3)
-              1470 POP_TOP
+    765        1250 LOAD_CONST              21 ('#ffffff')
    
-   882        1472 PUSH_NULL
-              1474 LOAD_BUILD_CLASS
-              1476 LOAD_CONST             117 (<code object AdwTFrame, file "D:\tkadw\tkadw\windows\theme.py", line 882>)
-              1478 MAKE_FUNCTION            0
-              1480 LOAD_CONST             118 ('AdwTFrame')
-              1482 LOAD_NAME               27 (AdwDrawRoundFrame3)
-              1484 PRECALL                  3
-              1488 CALL                     3
-              1498 STORE_NAME              28 (AdwTFrame)
+    766        1252 LOAD_CONST              98 ('#a0a0a0')
    
-   887        1500 LOAD_CONST              49 (0)
-              1502 LOAD_CONST             119 (('AdwDrawSeparator',))
-              1504 IMPORT_NAME             29 (tkadw.windows.canvas.separator)
-              1506 IMPORT_FROM             30 (AdwDrawSeparator)
-              1508 STORE_NAME              30 (AdwDrawSeparator)
-              1510 POP_TOP
+    767        1254 LOAD_CONST               3 ('#000000')
    
-   890        1512 PUSH_NULL
-              1514 LOAD_BUILD_CLASS
-              1516 LOAD_CONST             120 (<code object AdwTSeparator, file "D:\tkadw\tkadw\windows\theme.py", line 890>)
-              1518 MAKE_FUNCTION            0
-              1520 LOAD_CONST             121 ('AdwTSeparator')
-              1522 LOAD_NAME               30 (AdwDrawSeparator)
-              1524 PRECALL                  3
-              1528 CALL                     3
-              1538 STORE_NAME              31 (AdwTSeparator)
+    768        1256 LOAD_CONST               9 (1)
    
-   895        1540 LOAD_NAME               32 (__name__)
-              1542 LOAD_CONST             122 ('__main__')
-              1544 COMPARE_OP               2 (==)
-              1550 POP_JUMP_FORWARD_IF_FALSE   239 (to 2030)
+    771        1258 LOAD_CONST              99 ('#dce9fc')
    
-   896        1552 LOAD_CONST              49 (0)
-              1554 LOAD_CONST             123 (('isDark',))
-              1556 IMPORT_NAME             33 (darkdetect)
-              1558 IMPORT_FROM             34 (isDark)
-              1560 STORE_NAME              34 (isDark)
-              1562 POP_TOP
+    772        1260 LOAD_CONST              98 ('#a0a0a0')
    
-   898        1564 PUSH_NULL
-              1566 LOAD_NAME               13 (Adwite)
-              1568 PRECALL                  0
-              1572 CALL                     0
-              1582 STORE_NAME              35 (root)
+    773        1262 LOAD_CONST               3 ('#000000')
    
-   899        1584 LOAD_NAME               35 (root)
-              1586 LOAD_METHOD             10 (set_default_theme)
-              1608 LOAD_CONST             124 ('metro')
-              1610 PRECALL                  1
-              1614 CALL                     1
-              1624 POP_TOP
+    774        1264 LOAD_CONST               9 (1)
    
-   901        1626 LOAD_CONST             125 (<code object toggle, file "D:\tkadw\tkadw\windows\theme.py", line 901>)
-              1628 MAKE_FUNCTION            0
-              1630 STORE_NAME              36 (toggle)
+    770        1266 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+               1268 BUILD_CONST_KEY_MAP      4
    
-   904        1632 PUSH_NULL
-              1634 LOAD_NAME               19 (AdwTButton)
-              1636 LOAD_CONST             109 ('AdwTButton')
-              1638 LOAD_NAME               36 (toggle)
-              1640 KW_NAMES               126
-              1642 PRECALL                  2
-              1646 CALL                     2
-              1656 STORE_NAME              37 (button)
+    778        1270 LOAD_CONST              99 ('#dce9fc')
    
-   905        1658 LOAD_NAME               37 (button)
-              1660 LOAD_METHOD             38 (pack)
-              1682 LOAD_CONST             127 ('x')
-              1684 LOAD_CONST             128 (5)
-              1686 LOAD_CONST             128 (5)
-              1688 KW_NAMES               129
-              1690 PRECALL                  3
-              1694 CALL                     3
-              1704 POP_TOP
+    779        1272 LOAD_CONST             100 ('#4e6d9c')
    
-   906        1706 PUSH_NULL
-              1708 LOAD_NAME               31 (AdwTSeparator)
-              1710 PRECALL                  0
-              1714 CALL                     0
-              1724 STORE_NAME              39 (separator)
+    780        1274 LOAD_CONST               3 ('#000000')
    
-   907        1726 LOAD_NAME               39 (separator)
-              1728 LOAD_METHOD             38 (pack)
-              1750 LOAD_CONST             127 ('x')
-              1752 LOAD_CONST             128 (5)
-              1754 LOAD_CONST             128 (5)
-              1756 KW_NAMES               129
-              1758 PRECALL                  3
-              1762 CALL                     3
-              1772 POP_TOP
+    781        1276 LOAD_CONST              26 (2)
    
-   908        1774 PUSH_NULL
-              1776 LOAD_NAME               22 (AdwTEntry)
-              1778 LOAD_CONST             112 ('AdwTEntry')
-              1780 KW_NAMES               130
-              1782 PRECALL                  1
-              1786 CALL                     1
-              1796 STORE_NAME              40 (entry)
+    777        1278 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+               1280 BUILD_CONST_KEY_MAP      4
    
-   909        1798 LOAD_NAME               40 (entry)
-              1800 LOAD_METHOD             38 (pack)
-              1822 LOAD_CONST             127 ('x')
-              1824 LOAD_CONST             128 (5)
-              1826 LOAD_CONST             128 (5)
-              1828 KW_NAMES               129
-              1830 PRECALL                  3
-              1834 CALL                     3
-              1844 POP_TOP
+    763        1282 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+               1284 BUILD_CONST_KEY_MAP      7
    
-   910        1846 PUSH_NULL
-              1848 LOAD_NAME               25 (AdwTText)
-              1850 LOAD_CONST             115 ('AdwTText')
-              1852 KW_NAMES               130
-              1854 PRECALL                  1
-              1858 CALL                     1
-              1868 STORE_NAME              41 (text)
+    786        1286 LOAD_CONST              18 (0)
    
-   911        1870 LOAD_NAME               41 (text)
-              1872 LOAD_METHOD             38 (pack)
-              1894 LOAD_CONST             127 ('x')
-              1896 LOAD_CONST             128 (5)
-              1898 LOAD_CONST             128 (5)
-              1900 KW_NAMES               129
-              1902 PRECALL                  3
-              1906 CALL                     3
-              1916 POP_TOP
+    787        1288 LOAD_CONST              97 ('#f0f0f0')
    
-   912        1918 PUSH_NULL
-              1920 LOAD_NAME               28 (AdwTFrame)
-              1922 PRECALL                  0
-              1926 CALL                     0
-              1936 STORE_NAME              42 (frame)
+    788        1290 LOAD_CONST             101 ('#c8c8c8')
    
-   913        1938 LOAD_NAME               42 (frame)
-              1940 LOAD_METHOD             38 (pack)
-              1962 LOAD_CONST             127 ('x')
-              1964 LOAD_CONST             128 (5)
-              1966 LOAD_CONST             128 (5)
-              1968 KW_NAMES               129
-              1970 PRECALL                  3
-              1974 CALL                     3
-              1984 POP_TOP
+    789        1292 LOAD_CONST               9 (1)
    
-   914        1986 LOAD_NAME               35 (root)
-              1988 LOAD_METHOD             43 (mainloop)
-              2010 PRECALL                  0
-              2014 CALL                     0
-              2024 POP_TOP
-              2026 LOAD_CONST             131 (None)
-              2028 RETURN_VALUE
+    790        1294 LOAD_CONST              18 (0)
    
-   895     >> 2030 LOAD_CONST             131 (None)
-              2032 RETURN_VALUE
+    785        1296 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width', 'padding'))
+               1298 BUILD_CONST_KEY_MAP      5
+   
+    794        1300 LOAD_CONST              18 (0)
+   
+    795        1302 LOAD_CONST              89 ((3, 3))
+   
+    797        1304 LOAD_CONST              21 ('#ffffff')
+   
+    798        1306 LOAD_CONST              98 ('#a0a0a0')
+   
+    799        1308 LOAD_CONST               3 ('#000000')
+   
+    800        1310 LOAD_CONST               9 (1)
+   
+    802        1312 LOAD_CONST              21 ('#ffffff')
+   
+    803        1314 LOAD_CONST              18 (0)
+   
+    806        1316 LOAD_CONST              21 ('#ffffff')
+   
+    807        1318 LOAD_CONST              98 ('#a0a0a0')
+   
+    808        1320 LOAD_CONST               3 ('#000000')
+   
+    809        1322 LOAD_CONST               9 (1)
+   
+    811        1324 LOAD_CONST              21 ('#ffffff')
+   
+    812        1326 LOAD_CONST              18 (0)
+   
+    805        1328 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               1330 BUILD_CONST_KEY_MAP      6
+   
+    793        1332 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               1334 BUILD_CONST_KEY_MAP      9
+   
+    817        1336 LOAD_CONST              18 (0)
+   
+    818        1338 LOAD_CONST              89 ((3, 3))
+   
+    820        1340 LOAD_CONST              21 ('#ffffff')
+   
+    821        1342 LOAD_CONST              98 ('#a0a0a0')
+   
+    822        1344 LOAD_CONST               3 ('#000000')
+   
+    823        1346 LOAD_CONST               9 (1)
+   
+    825        1348 LOAD_CONST              21 ('#ffffff')
+   
+    826        1350 LOAD_CONST              18 (0)
+   
+    829        1352 LOAD_CONST              21 ('#ffffff')
+   
+    830        1354 LOAD_CONST              98 ('#a0a0a0')
+   
+    831        1356 LOAD_CONST               3 ('#000000')
+   
+    832        1358 LOAD_CONST               9 (1)
+   
+    834        1360 LOAD_CONST              21 ('#ffffff')
+   
+    835        1362 LOAD_CONST              18 (0)
+   
+    828        1364 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               1366 BUILD_CONST_KEY_MAP      6
+   
+    816        1368 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               1370 BUILD_CONST_KEY_MAP      9
+   
+    840        1372 LOAD_CONST              90 ('#999999')
+   
+    841        1374 LOAD_CONST               9 (1)
+   
+    843        1376 LOAD_CONST              30 (True)
+   
+    839        1378 LOAD_CONST              31 (('back', 'border_width', 'rounded'))
+               1380 BUILD_CONST_KEY_MAP      3
+   
+    753        1382 LOAD_CONST              32 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
+               1384 BUILD_CONST_KEY_MAP      7
+               1386 STORE_NAME               8 (basic_theme)
+   
+    849        1388 LOAD_CONST               0 ('back')
+               1390 LOAD_CONST             102 ('#323232')
+   
+    848        1392 BUILD_MAP                1
+   
+    853        1394 LOAD_CONST               2 ('transparent')
+   
+    854        1396 LOAD_CONST              21 ('#ffffff')
+   
+    852        1398 LOAD_CONST               4 (('back', 'text_back'))
+               1400 BUILD_CONST_KEY_MAP      2
+   
+    858        1402 LOAD_CONST              18 (0)
+   
+    859        1404 LOAD_CONST              36 ('#232323')
+   
+    860        1406 LOAD_CONST             103 ('#4b4b4b')
+   
+    861        1408 LOAD_CONST              21 ('#ffffff')
+   
+    862        1410 LOAD_CONST               9 (1)
+   
+    865        1412 LOAD_CONST              62 ('#373737')
+   
+    866        1414 LOAD_CONST             103 ('#4b4b4b')
+   
+    867        1416 LOAD_CONST              21 ('#ffffff')
+   
+    868        1418 LOAD_CONST               9 (1)
+   
+    864        1420 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+               1422 BUILD_CONST_KEY_MAP      4
+   
+    872        1424 LOAD_CONST              62 ('#373737')
+   
+    873        1426 LOAD_CONST             100 ('#4e6d9c')
+   
+    874        1428 LOAD_CONST              21 ('#ffffff')
+   
+    875        1430 LOAD_CONST              26 (2)
+   
+    871        1432 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+               1434 BUILD_CONST_KEY_MAP      4
+   
+    857        1436 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+               1438 BUILD_CONST_KEY_MAP      7
+   
+    880        1440 LOAD_CONST              18 (0)
+   
+    881        1442 LOAD_CONST             102 ('#323232')
+   
+    882        1444 LOAD_CONST             104 ('#464646')
+   
+    883        1446 LOAD_CONST               9 (1)
+   
+    884        1448 LOAD_CONST              18 (0)
+   
+    879        1450 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width', 'padding'))
+               1452 BUILD_CONST_KEY_MAP      5
+   
+    888        1454 LOAD_CONST              18 (0)
+   
+    889        1456 LOAD_CONST              89 ((3, 3))
+   
+    891        1458 LOAD_CONST              36 ('#232323')
+   
+    892        1460 LOAD_CONST             103 ('#4b4b4b')
+   
+    893        1462 LOAD_CONST              21 ('#ffffff')
+   
+    894        1464 LOAD_CONST               9 (1)
+   
+    896        1466 LOAD_CONST              21 ('#ffffff')
+   
+    897        1468 LOAD_CONST              18 (0)
+   
+    900        1470 LOAD_CONST              36 ('#232323')
+   
+    901        1472 LOAD_CONST             103 ('#4b4b4b')
+   
+    902        1474 LOAD_CONST              21 ('#ffffff')
+   
+    903        1476 LOAD_CONST               9 (1)
+   
+    905        1478 LOAD_CONST              21 ('#ffffff')
+   
+    906        1480 LOAD_CONST              18 (0)
+   
+    899        1482 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               1484 BUILD_CONST_KEY_MAP      6
+   
+    887        1486 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               1488 BUILD_CONST_KEY_MAP      9
+   
+    911        1490 LOAD_CONST              18 (0)
+   
+    912        1492 LOAD_CONST              89 ((3, 3))
+   
+    914        1494 LOAD_CONST              36 ('#232323')
+   
+    915        1496 LOAD_CONST             103 ('#4b4b4b')
+   
+    916        1498 LOAD_CONST              21 ('#ffffff')
+   
+    917        1500 LOAD_CONST               9 (1)
+   
+    919        1502 LOAD_CONST              21 ('#ffffff')
+   
+    920        1504 LOAD_CONST              18 (0)
+   
+    923        1506 LOAD_CONST              36 ('#232323')
+   
+    924        1508 LOAD_CONST             103 ('#4b4b4b')
+   
+    925        1510 LOAD_CONST              21 ('#ffffff')
+   
+    926        1512 LOAD_CONST               9 (1)
+   
+    928        1514 LOAD_CONST              21 ('#ffffff')
+   
+    929        1516 LOAD_CONST              18 (0)
+   
+    922        1518 LOAD_CONST              27 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               1520 BUILD_CONST_KEY_MAP      6
+   
+    910        1522 LOAD_CONST              28 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               1524 BUILD_CONST_KEY_MAP      9
+   
+    934        1526 LOAD_CONST             104 ('#464646')
+   
+    935        1528 LOAD_CONST               9 (1)
+   
+    937        1530 LOAD_CONST              96 (False)
+   
+    933        1532 LOAD_CONST              31 (('back', 'border_width', 'rounded'))
+               1534 BUILD_CONST_KEY_MAP      3
+   
+    847        1536 LOAD_CONST              32 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
+               1538 BUILD_CONST_KEY_MAP      7
+               1540 STORE_NAME               9 (basic_dark_theme)
+   
+    942        1542 LOAD_CONST             105 (<code object get_default_theme, file "D:\tkadw\tkadw\windows\theme.py", line 942>)
+               1544 MAKE_FUNCTION            0
+               1546 STORE_NAME              10 (get_default_theme)
+   
+    951        1548 LOAD_CONST             106 (<code object _set_default_theme, file "D:\tkadw\tkadw\windows\theme.py", line 951>)
+               1550 MAKE_FUNCTION            0
+               1552 STORE_NAME              11 (_set_default_theme)
+   
+    957        1554 LOAD_CONST             139 (('system',))
+               1556 LOAD_CONST             108 (<code object set_default_theme, file "D:\tkadw\tkadw\windows\theme.py", line 957>)
+               1558 MAKE_FUNCTION            1 (defaults)
+               1560 STORE_NAME              12 (set_default_theme)
+   
+   1038        1562 PUSH_NULL
+               1564 LOAD_NAME               12 (set_default_theme)
+               1566 LOAD_CONST             109 ('win11')
+               1568 PRECALL                  1
+               1572 CALL                     1
+               1582 POP_TOP
+   
+   1041        1584 LOAD_CONST              18 (0)
+               1586 LOAD_CONST             110 (('Adw',))
+               1588 IMPORT_NAME             13 (tkadw.windows.widgets.adw)
+               1590 IMPORT_FROM             14 (Adw)
+               1592 STORE_NAME              14 (Adw)
+               1594 POP_TOP
+   
+   1044        1596 PUSH_NULL
+               1598 LOAD_BUILD_CLASS
+               1600 LOAD_CONST             111 (<code object Adwite, file "D:\tkadw\tkadw\windows\theme.py", line 1044>)
+               1602 MAKE_FUNCTION            0
+               1604 LOAD_CONST             112 ('Adwite')
+               1606 LOAD_NAME               14 (Adw)
+               1608 PRECALL                  3
+               1612 CALL                     3
+               1622 STORE_NAME              15 (Adwite)
+   
+   1058        1624 LOAD_CONST              18 (0)
+               1626 LOAD_CONST             113 (('AdwLabel',))
+               1628 IMPORT_NAME             16 (tkadw.windows.widgets)
+               1630 IMPORT_FROM             17 (AdwLabel)
+               1632 STORE_NAME              17 (AdwLabel)
+               1634 POP_TOP
+   
+   1061        1636 PUSH_NULL
+               1638 LOAD_BUILD_CLASS
+               1640 LOAD_CONST             114 (<code object AdwTLabel, file "D:\tkadw\tkadw\windows\theme.py", line 1061>)
+               1642 MAKE_FUNCTION            0
+               1644 LOAD_CONST             115 ('AdwTLabel')
+               1646 LOAD_NAME               17 (AdwLabel)
+               1648 PRECALL                  3
+               1652 CALL                     3
+               1662 STORE_NAME              18 (AdwTLabel)
+   
+   1066        1664 LOAD_CONST              18 (0)
+               1666 LOAD_CONST             116 (('AdwDrawRoundButton3',))
+               1668 IMPORT_NAME             19 (tkadw.windows.canvas.button)
+               1670 IMPORT_FROM             20 (AdwDrawRoundButton3)
+               1672 STORE_NAME              20 (AdwDrawRoundButton3)
+               1674 POP_TOP
+   
+   1069        1676 PUSH_NULL
+               1678 LOAD_BUILD_CLASS
+               1680 LOAD_CONST             117 (<code object AdwTButton, file "D:\tkadw\tkadw\windows\theme.py", line 1069>)
+               1682 MAKE_FUNCTION            0
+               1684 LOAD_CONST             118 ('AdwTButton')
+               1686 LOAD_NAME               20 (AdwDrawRoundButton3)
+               1688 PRECALL                  3
+               1692 CALL                     3
+               1702 STORE_NAME              21 (AdwTButton)
+   
+   1074        1704 LOAD_CONST              18 (0)
+               1706 LOAD_CONST             119 (('AdwDrawRoundEntry3',))
+               1708 IMPORT_NAME             22 (tkadw.windows.canvas.entry)
+               1710 IMPORT_FROM             23 (AdwDrawRoundEntry3)
+               1712 STORE_NAME              23 (AdwDrawRoundEntry3)
+               1714 POP_TOP
+   
+   1077        1716 PUSH_NULL
+               1718 LOAD_BUILD_CLASS
+               1720 LOAD_CONST             120 (<code object AdwTEntry, file "D:\tkadw\tkadw\windows\theme.py", line 1077>)
+               1722 MAKE_FUNCTION            0
+               1724 LOAD_CONST             121 ('AdwTEntry')
+               1726 LOAD_NAME               23 (AdwDrawRoundEntry3)
+               1728 PRECALL                  3
+               1732 CALL                     3
+               1742 STORE_NAME              24 (AdwTEntry)
+   
+   1082        1744 LOAD_CONST              18 (0)
+               1746 LOAD_CONST             122 (('AdwDrawRoundText3',))
+               1748 IMPORT_NAME             25 (tkadw.windows.canvas.textbox)
+               1750 IMPORT_FROM             26 (AdwDrawRoundText3)
+               1752 STORE_NAME              26 (AdwDrawRoundText3)
+               1754 POP_TOP
+   
+   1085        1756 PUSH_NULL
+               1758 LOAD_BUILD_CLASS
+               1760 LOAD_CONST             123 (<code object AdwTText, file "D:\tkadw\tkadw\windows\theme.py", line 1085>)
+               1762 MAKE_FUNCTION            0
+               1764 LOAD_CONST             124 ('AdwTText')
+               1766 LOAD_NAME               26 (AdwDrawRoundText3)
+               1768 PRECALL                  3
+               1772 CALL                     3
+               1782 STORE_NAME              27 (AdwTText)
+   
+   1090        1784 LOAD_CONST              18 (0)
+               1786 LOAD_CONST             125 (('AdwDrawRoundFrame3',))
+               1788 IMPORT_NAME             28 (tkadw.windows.canvas.frame)
+               1790 IMPORT_FROM             29 (AdwDrawRoundFrame3)
+               1792 STORE_NAME              29 (AdwDrawRoundFrame3)
+               1794 POP_TOP
+   
+   1093        1796 PUSH_NULL
+               1798 LOAD_BUILD_CLASS
+               1800 LOAD_CONST             126 (<code object AdwTFrame, file "D:\tkadw\tkadw\windows\theme.py", line 1093>)
+               1802 MAKE_FUNCTION            0
+               1804 LOAD_CONST             127 ('AdwTFrame')
+               1806 LOAD_NAME               29 (AdwDrawRoundFrame3)
+               1808 PRECALL                  3
+               1812 CALL                     3
+               1822 STORE_NAME              30 (AdwTFrame)
+   
+   1098        1824 LOAD_CONST              18 (0)
+               1826 LOAD_CONST             128 (('AdwDrawSeparator',))
+               1828 IMPORT_NAME             31 (tkadw.windows.canvas.separator)
+               1830 IMPORT_FROM             32 (AdwDrawSeparator)
+               1832 STORE_NAME              32 (AdwDrawSeparator)
+               1834 POP_TOP
+   
+   1101        1836 PUSH_NULL
+               1838 LOAD_BUILD_CLASS
+               1840 LOAD_CONST             129 (<code object AdwTSeparator, file "D:\tkadw\tkadw\windows\theme.py", line 1101>)
+               1842 MAKE_FUNCTION            0
+               1844 LOAD_CONST             130 ('AdwTSeparator')
+               1846 LOAD_NAME               32 (AdwDrawSeparator)
+               1848 PRECALL                  3
+               1852 CALL                     3
+               1862 STORE_NAME              33 (AdwTSeparator)
+   
+   1106        1864 LOAD_NAME               34 (__name__)
+               1866 LOAD_CONST             131 ('__main__')
+               1868 COMPARE_OP               2 (==)
+               1874 POP_JUMP_FORWARD_IF_FALSE   236 (to 2348)
+   
+   1107        1876 LOAD_CONST              18 (0)
+               1878 LOAD_CONST             132 (('isDark',))
+               1880 IMPORT_NAME             35 (darkdetect)
+               1882 IMPORT_FROM             36 (isDark)
+               1884 STORE_NAME              36 (isDark)
+               1886 POP_TOP
+   
+   1109        1888 PUSH_NULL
+               1890 LOAD_NAME               15 (Adwite)
+               1892 PRECALL                  0
+               1896 CALL                     0
+               1906 STORE_NAME              37 (root)
+   
+   1110        1908 LOAD_NAME               37 (root)
+               1910 LOAD_METHOD             12 (set_default_theme)
+               1932 LOAD_CONST             109 ('win11')
+               1934 LOAD_CONST             133 ('dark')
+               1936 PRECALL                  2
+               1940 CALL                     2
+               1950 POP_TOP
+   
+   1112        1952 PUSH_NULL
+               1954 LOAD_NAME               21 (AdwTButton)
+               1956 LOAD_CONST             118 ('AdwTButton')
+               1958 KW_NAMES               134
+               1960 PRECALL                  1
+               1964 CALL                     1
+               1974 STORE_NAME              38 (button)
+   
+   1113        1976 LOAD_NAME               38 (button)
+               1978 LOAD_METHOD             39 (pack)
+               2000 LOAD_CONST             135 ('x')
+               2002 LOAD_CONST             136 (5)
+               2004 LOAD_CONST             136 (5)
+               2006 KW_NAMES               137
+               2008 PRECALL                  3
+               2012 CALL                     3
+               2022 POP_TOP
+   
+   1114        2024 PUSH_NULL
+               2026 LOAD_NAME               33 (AdwTSeparator)
+               2028 PRECALL                  0
+               2032 CALL                     0
+               2042 STORE_NAME              40 (separator)
+   
+   1115        2044 LOAD_NAME               40 (separator)
+               2046 LOAD_METHOD             39 (pack)
+               2068 LOAD_CONST             135 ('x')
+               2070 LOAD_CONST             136 (5)
+               2072 LOAD_CONST             136 (5)
+               2074 KW_NAMES               137
+               2076 PRECALL                  3
+               2080 CALL                     3
+               2090 POP_TOP
+   
+   1116        2092 PUSH_NULL
+               2094 LOAD_NAME               24 (AdwTEntry)
+               2096 LOAD_CONST             121 ('AdwTEntry')
+               2098 KW_NAMES               134
+               2100 PRECALL                  1
+               2104 CALL                     1
+               2114 STORE_NAME              41 (entry)
+   
+   1117        2116 LOAD_NAME               41 (entry)
+               2118 LOAD_METHOD             39 (pack)
+               2140 LOAD_CONST             135 ('x')
+               2142 LOAD_CONST             136 (5)
+               2144 LOAD_CONST             136 (5)
+               2146 KW_NAMES               137
+               2148 PRECALL                  3
+               2152 CALL                     3
+               2162 POP_TOP
+   
+   1118        2164 PUSH_NULL
+               2166 LOAD_NAME               27 (AdwTText)
+               2168 LOAD_CONST             124 ('AdwTText')
+               2170 KW_NAMES               134
+               2172 PRECALL                  1
+               2176 CALL                     1
+               2186 STORE_NAME              42 (text)
+   
+   1119        2188 LOAD_NAME               42 (text)
+               2190 LOAD_METHOD             39 (pack)
+               2212 LOAD_CONST             135 ('x')
+               2214 LOAD_CONST             136 (5)
+               2216 LOAD_CONST             136 (5)
+               2218 KW_NAMES               137
+               2220 PRECALL                  3
+               2224 CALL                     3
+               2234 POP_TOP
+   
+   1120        2236 PUSH_NULL
+               2238 LOAD_NAME               30 (AdwTFrame)
+               2240 PRECALL                  0
+               2244 CALL                     0
+               2254 STORE_NAME              43 (frame)
+   
+   1121        2256 LOAD_NAME               43 (frame)
+               2258 LOAD_METHOD             39 (pack)
+               2280 LOAD_CONST             135 ('x')
+               2282 LOAD_CONST             136 (5)
+               2284 LOAD_CONST             136 (5)
+               2286 KW_NAMES               137
+               2288 PRECALL                  3
+               2292 CALL                     3
+               2302 POP_TOP
+   
+   1122        2304 LOAD_NAME               37 (root)
+               2306 LOAD_METHOD             44 (mainloop)
+               2328 PRECALL                  0
+               2332 CALL                     0
+               2342 POP_TOP
+               2344 LOAD_CONST             138 (None)
+               2346 RETURN_VALUE
+   
+   1106     >> 2348 LOAD_CONST             138 (None)
+               2350 RETURN_VALUE
    consts
       'back'
       '#f4f4f4'
       'transparent'
       '#000000'
       ('back', 'text_back')
       13
@@ -1469,46 +1774,47 @@
       '#d5d5d5'
       ('back', 'border', 'text_back', 'border_width')
       '#fafafa'
       '#ebebeb'
       ('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed')
       15
       '#e7e7e7'
-      2
-      ('radius', 'back', 'border', 'border_width')
+      0
+      ('radius', 'back', 'border', 'border_width', 'padding')
       (8, 8)
-      '#18191c'
-      '#8a8a8a'
       '#ffffff'
+      '#e6e6e6'
+      '#18191c'
+      '#9c9c9c'
       '#005fb8'
+      2
       ('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width')
       ('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
       '#d0d0d0'
       True
       ('back', 'border_width', 'rounded')
       ('window', 'label', 'button', 'frame', 'entry', 'text', 'separator')
       '#2a2a2a'
       '#313131'
       '#2f2f2f'
       '#232323'
       '#2c2c2c'
       '#1c1c1c'
-      '#292929'
+      '#383838'
       '#e7e9eb'
-      '#989898'
+      '#686868'
       '#57c8ff'
       '#404040'
       11
       '#f6f5f4'
       '#ccc6c1'
       '#2e3436'
       1.3
       '#f8f8f7'
       '#dad6d2'
-      0
       '#d5d0cc'
       (5, 5)
       '#cdc7c2'
       '#eaeaea'
       '#3584e4'
       '#185fb4'
       ('padding', 'radius', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
@@ -1547,62 +1853,70 @@
       '#999999'
       '#00aedb'
       '#111111'
       '#222222'
       '#444444'
       '#aaaaaa'
       False
+      '#f0f0f0'
+      '#a0a0a0'
+      '#dce9fc'
+      '#4e6d9c'
+      '#c8c8c8'
+      '#323232'
+      '#4b4b4b'
+      '#464646'
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x9700640164026c006d017d000100640164036c026d037d010100090002
             007c017c00640419000000000000000000a6010000ab0100000000000000
             005300230074080000000000000000000024007204010059006400530077
             00780359007701
-         746           0 RESUME                   0
+         942           0 RESUME                   0
          
-         747           2 LOAD_CONST               1 (0)
+         943           2 LOAD_CONST               1 (0)
                        4 LOAD_CONST               2 (('environ',))
                        6 IMPORT_NAME              0 (os)
                        8 IMPORT_FROM              1 (environ)
                       10 STORE_FAST               0 (environ)
                       12 POP_TOP
          
-         748          14 LOAD_CONST               1 (0)
+         944          14 LOAD_CONST               1 (0)
                       16 LOAD_CONST               3 (('loads',))
                       18 IMPORT_NAME              2 (json)
                       20 IMPORT_FROM              3 (loads)
                       22 STORE_FAST               1 (loads)
                       24 POP_TOP
          
-         749          26 NOP
+         945          26 NOP
          
-         750          28 PUSH_NULL
+         946          28 PUSH_NULL
                       30 LOAD_FAST                1 (loads)
                       32 LOAD_FAST                0 (environ)
                       34 LOAD_CONST               4 ('tkAdwite.DefaultTheme')
                       36 BINARY_SUBSCR
                       46 PRECALL                  1
                       50 CALL                     1
                       60 RETURN_VALUE
                  >>   62 PUSH_EXC_INFO
          
-         751          64 LOAD_GLOBAL              8 (KeyError)
+         947          64 LOAD_GLOBAL              8 (KeyError)
                       76 CHECK_EXC_MATCH
                       78 POP_JUMP_FORWARD_IF_FALSE     4 (to 88)
                       80 POP_TOP
          
-         752          82 POP_EXCEPT
+         948          82 POP_EXCEPT
                       84 LOAD_CONST               0 (None)
                       86 RETURN_VALUE
          
-         751     >>   88 RERAISE                  0
+         947     >>   88 RERAISE                  0
                  >>   90 COPY                     3
                       92 POP_EXCEPT
                       94 RERAISE                  1
          ExceptionTable:
            28 to 58 -> 62 [0]
            62 to 80 -> 90 [1] lasti
            88 to 88 -> 90 [1] lasti
@@ -1614,41 +1928,41 @@
             'tkAdwite.DefaultTheme'
          names      ('os', 'environ', 'json', 'loads', 'KeyError')
          varnames   ('environ', 'loads')
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'get_default_theme'
-         firstlineno 746
+         firstlineno 942
          lnotab 0x02010c010c0102012401120106ff
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 3
          flags     : 3
          code
             0x9700640164026c006d017d010100640164036c026d037d02010002007c
             027c00a6010000ab0100000000000000007c0164043c00000064005300
-         755           0 RESUME                   0
+         951           0 RESUME                   0
          
-         756           2 LOAD_CONST               1 (0)
+         952           2 LOAD_CONST               1 (0)
                        4 LOAD_CONST               2 (('environ',))
                        6 IMPORT_NAME              0 (os)
                        8 IMPORT_FROM              1 (environ)
                       10 STORE_FAST               1 (environ)
                       12 POP_TOP
          
-         757          14 LOAD_CONST               1 (0)
+         953          14 LOAD_CONST               1 (0)
                       16 LOAD_CONST               3 (('dumps',))
                       18 IMPORT_NAME              2 (json)
                       20 IMPORT_FROM              3 (dumps)
                       22 STORE_FAST               2 (dumps)
                       24 POP_TOP
          
-         758          26 PUSH_NULL
+         954          26 PUSH_NULL
                       28 LOAD_FAST                2 (dumps)
                       30 LOAD_FAST                0 (theme)
                       32 PRECALL                  1
                       36 CALL                     1
                       46 LOAD_FAST                1 (environ)
                       48 LOAD_CONST               4 ('tkAdwite.DefaultTheme')
                       50 STORE_SUBSCR
@@ -1662,15 +1976,15 @@
             'tkAdwite.DefaultTheme'
          names      ('os', 'environ', 'json', 'dumps')
          varnames   ('theme', 'environ', 'dumps')
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       '_set_default_theme'
-         firstlineno 755
+         firstlineno 951
          lnotab 0x02010c010c01
       'system'
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 4
          flags     : 3
@@ -1732,442 +2046,559 @@
             00640053002300740c000000000000000000002400721801007407000000
             00000000000000741800000000000000000000a6010000ab010000000000
             000000010059006400530077007803590077017c01a00000000000000000
             00000000000000000000000000a6000000ab00000000000000000064096b
             020000000072167407000000000000000000007416000000000000000000
             00a6010000ab010000000000000000010064005300740700000000000000
             000000741800000000000000000000a6010000ab01000000000000000001
-            00640053007407000000000000000000007c00a6010000ab010000000000
-            000000010064005300
-         761           0 RESUME                   0
-         
-         762           2 LOAD_FAST                0 (theme)
-                       4 LOAD_CONST               1 ('win11')
-                       6 COMPARE_OP               2 (==)
-                      12 POP_JUMP_FORWARD_IF_TRUE    18 (to 50)
-                      14 LOAD_FAST                0 (theme)
-                      16 LOAD_CONST               2 ('windows11')
-                      18 COMPARE_OP               2 (==)
-                      24 POP_JUMP_FORWARD_IF_TRUE    12 (to 50)
-                      26 LOAD_FAST                0 (theme)
-                      28 LOAD_CONST               3 ('Windows11')
-                      30 COMPARE_OP               2 (==)
-                      36 POP_JUMP_FORWARD_IF_TRUE     6 (to 50)
-                      38 LOAD_FAST                0 (theme)
-                      40 LOAD_CONST               4 ('Win11')
-                      42 COMPARE_OP               2 (==)
-                      48 POP_JUMP_FORWARD_IF_FALSE   214 (to 478)
-         
-         763     >>   50 LOAD_FAST                1 (mode)
-                      52 LOAD_METHOD              0 (lower)
-                      74 PRECALL                  0
-                      78 CALL                     0
-                      88 LOAD_CONST               5 ('system')
-                      90 COMPARE_OP               2 (==)
-                      96 POP_JUMP_FORWARD_IF_TRUE    24 (to 146)
-                      98 LOAD_FAST                1 (mode)
-                     100 LOAD_METHOD              0 (lower)
-                     122 PRECALL                  0
-                     126 CALL                     0
-                     136 LOAD_CONST               6 ('auto')
-                     138 COMPARE_OP               2 (==)
-                     144 POP_JUMP_FORWARD_IF_FALSE    98 (to 342)
-         
-         764     >>  146 NOP
-         
-         765         148 LOAD_CONST               7 (0)
-                     150 LOAD_CONST               8 (('isDark',))
-                     152 IMPORT_NAME              1 (darkdetect)
-                     154 IMPORT_FROM              2 (isDark)
-                     156 STORE_FAST               2 (isDark)
-                     158 POP_TOP
-         
-         769         160 PUSH_NULL
-                     162 LOAD_FAST                2 (isDark)
-                     164 PRECALL                  0
-                     168 CALL                     0
-                     178 POP_JUMP_FORWARD_IF_FALSE    22 (to 224)
-         
-         770         180 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     192 LOAD_GLOBAL              8 (win11_dark_theme)
-                     204 PRECALL                  1
-                     208 CALL                     1
-                     218 POP_TOP
-                     220 LOAD_CONST               0 (None)
-                     222 RETURN_VALUE
-         
-         772     >>  224 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     236 LOAD_GLOBAL             10 (win11_theme)
-                     248 PRECALL                  1
-                     252 CALL                     1
-                     262 POP_TOP
-                     264 LOAD_CONST               0 (None)
-                     266 RETURN_VALUE
-                 >>  268 PUSH_EXC_INFO
-         
-         766         270 LOAD_GLOBAL             12 (ModuleNotFoundError)
-                     282 CHECK_EXC_MATCH
-                     284 POP_JUMP_FORWARD_IF_FALSE    24 (to 334)
-                     286 POP_TOP
-         
-         767         288 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     300 LOAD_GLOBAL             10 (win11_theme)
-                     312 PRECALL                  1
-                     316 CALL                     1
-                     326 POP_TOP
-                     328 POP_EXCEPT
-                     330 LOAD_CONST               0 (None)
-                     332 RETURN_VALUE
-         
-         766     >>  334 RERAISE                  0
-                 >>  336 COPY                     3
-                     338 POP_EXCEPT
-                     340 RERAISE                  1
-         
-         773     >>  342 LOAD_FAST                1 (mode)
-                     344 LOAD_METHOD              0 (lower)
-                     366 PRECALL                  0
-                     370 CALL                     0
-                     380 LOAD_CONST               9 ('dark')
-                     382 COMPARE_OP               2 (==)
-                     388 POP_JUMP_FORWARD_IF_FALSE    22 (to 434)
-         
-         774         390 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     402 LOAD_GLOBAL              8 (win11_dark_theme)
-                     414 PRECALL                  1
-                     418 CALL                     1
-                     428 POP_TOP
-                     430 LOAD_CONST               0 (None)
-                     432 RETURN_VALUE
-         
-         776     >>  434 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     446 LOAD_GLOBAL             10 (win11_theme)
-                     458 PRECALL                  1
-                     462 CALL                     1
-                     472 POP_TOP
-                     474 LOAD_CONST               0 (None)
-                     476 RETURN_VALUE
-         
-         777     >>  478 LOAD_FAST                0 (theme)
-                     480 LOAD_CONST              10 ('gtk')
-                     482 COMPARE_OP               2 (==)
-                     488 POP_JUMP_FORWARD_IF_TRUE     6 (to 502)
-                     490 LOAD_FAST                0 (theme)
-                     492 LOAD_CONST              11 ('Gtk')
-                     494 COMPARE_OP               2 (==)
-                     500 POP_JUMP_FORWARD_IF_FALSE   214 (to 930)
-         
-         778     >>  502 LOAD_FAST                1 (mode)
-                     504 LOAD_METHOD              0 (lower)
-                     526 PRECALL                  0
-                     530 CALL                     0
-                     540 LOAD_CONST               5 ('system')
-                     542 COMPARE_OP               2 (==)
-                     548 POP_JUMP_FORWARD_IF_TRUE    24 (to 598)
-                     550 LOAD_FAST                1 (mode)
-                     552 LOAD_METHOD              0 (lower)
-                     574 PRECALL                  0
-                     578 CALL                     0
-                     588 LOAD_CONST               6 ('auto')
-                     590 COMPARE_OP               2 (==)
-                     596 POP_JUMP_FORWARD_IF_FALSE    98 (to 794)
-         
-         779     >>  598 NOP
-         
-         780         600 LOAD_CONST               7 (0)
-                     602 LOAD_CONST               8 (('isDark',))
-                     604 IMPORT_NAME              1 (darkdetect)
-                     606 IMPORT_FROM              2 (isDark)
-                     608 STORE_FAST               2 (isDark)
-                     610 POP_TOP
-         
-         784         612 PUSH_NULL
-                     614 LOAD_FAST                2 (isDark)
-                     616 PRECALL                  0
-                     620 CALL                     0
-                     630 POP_JUMP_FORWARD_IF_FALSE    22 (to 676)
-         
-         785         632 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     644 LOAD_GLOBAL             14 (gtk_dark_theme)
-                     656 PRECALL                  1
-                     660 CALL                     1
-                     670 POP_TOP
-                     672 LOAD_CONST               0 (None)
-                     674 RETURN_VALUE
-         
-         787     >>  676 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     688 LOAD_GLOBAL             16 (gtk_theme)
-                     700 PRECALL                  1
-                     704 CALL                     1
-                     714 POP_TOP
-                     716 LOAD_CONST               0 (None)
-                     718 RETURN_VALUE
-                 >>  720 PUSH_EXC_INFO
-         
-         781         722 LOAD_GLOBAL             12 (ModuleNotFoundError)
-                     734 CHECK_EXC_MATCH
-                     736 POP_JUMP_FORWARD_IF_FALSE    24 (to 786)
-                     738 POP_TOP
-         
-         782         740 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     752 LOAD_GLOBAL             16 (gtk_theme)
-                     764 PRECALL                  1
-                     768 CALL                     1
-                     778 POP_TOP
-                     780 POP_EXCEPT
-                     782 LOAD_CONST               0 (None)
-                     784 RETURN_VALUE
-         
-         781     >>  786 RERAISE                  0
-                 >>  788 COPY                     3
-                     790 POP_EXCEPT
-                     792 RERAISE                  1
-         
-         789     >>  794 LOAD_FAST                1 (mode)
-                     796 LOAD_METHOD              0 (lower)
-                     818 PRECALL                  0
-                     822 CALL                     0
-                     832 LOAD_CONST               9 ('dark')
-                     834 COMPARE_OP               2 (==)
-                     840 POP_JUMP_FORWARD_IF_FALSE    22 (to 886)
-         
-         790         842 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     854 LOAD_GLOBAL             14 (gtk_dark_theme)
-                     866 PRECALL                  1
-                     870 CALL                     1
-                     880 POP_TOP
-                     882 LOAD_CONST               0 (None)
-                     884 RETURN_VALUE
-         
-         792     >>  886 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     898 LOAD_GLOBAL             16 (gtk_theme)
-                     910 PRECALL                  1
-                     914 CALL                     1
-                     924 POP_TOP
-                     926 LOAD_CONST               0 (None)
-                     928 RETURN_VALUE
-         
-         793     >>  930 LOAD_FAST                0 (theme)
-                     932 LOAD_CONST              12 ('bilibili')
-                     934 COMPARE_OP               2 (==)
-                     940 POP_JUMP_FORWARD_IF_TRUE     6 (to 954)
-                     942 LOAD_FAST                0 (theme)
-                     944 LOAD_CONST              13 ('BiliBili')
-                     946 COMPARE_OP               2 (==)
-                     952 POP_JUMP_FORWARD_IF_FALSE   214 (to 1382)
-         
-         794     >>  954 LOAD_FAST                1 (mode)
-                     956 LOAD_METHOD              0 (lower)
-                     978 PRECALL                  0
-                     982 CALL                     0
-                     992 LOAD_CONST               5 ('system')
-                     994 COMPARE_OP               2 (==)
-                    1000 POP_JUMP_FORWARD_IF_TRUE    24 (to 1050)
-                    1002 LOAD_FAST                1 (mode)
-                    1004 LOAD_METHOD              0 (lower)
-                    1026 PRECALL                  0
-                    1030 CALL                     0
-                    1040 LOAD_CONST               6 ('auto')
-                    1042 COMPARE_OP               2 (==)
-                    1048 POP_JUMP_FORWARD_IF_FALSE    98 (to 1246)
-         
-         795     >> 1050 NOP
-         
-         796        1052 LOAD_CONST               7 (0)
-                    1054 LOAD_CONST               8 (('isDark',))
-                    1056 IMPORT_NAME              1 (darkdetect)
-                    1058 IMPORT_FROM              2 (isDark)
-                    1060 STORE_FAST               2 (isDark)
-                    1062 POP_TOP
-         
-         800        1064 PUSH_NULL
-                    1066 LOAD_FAST                2 (isDark)
-                    1068 PRECALL                  0
-                    1072 CALL                     0
-                    1082 POP_JUMP_FORWARD_IF_FALSE    22 (to 1128)
-         
-         801        1084 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                    1096 LOAD_GLOBAL             18 (bilibili_dark_theme)
-                    1108 PRECALL                  1
-                    1112 CALL                     1
-                    1122 POP_TOP
-                    1124 LOAD_CONST               0 (None)
-                    1126 RETURN_VALUE
-         
-         803     >> 1128 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                    1140 LOAD_GLOBAL             20 (bilibili_theme)
-                    1152 PRECALL                  1
-                    1156 CALL                     1
-                    1166 POP_TOP
-                    1168 LOAD_CONST               0 (None)
-                    1170 RETURN_VALUE
-                 >> 1172 PUSH_EXC_INFO
-         
-         797        1174 LOAD_GLOBAL             12 (ModuleNotFoundError)
-                    1186 CHECK_EXC_MATCH
-                    1188 POP_JUMP_FORWARD_IF_FALSE    24 (to 1238)
-                    1190 POP_TOP
-         
-         798        1192 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                    1204 LOAD_GLOBAL             20 (bilibili_theme)
-                    1216 PRECALL                  1
-                    1220 CALL                     1
-                    1230 POP_TOP
-                    1232 POP_EXCEPT
-                    1234 LOAD_CONST               0 (None)
-                    1236 RETURN_VALUE
-         
-         797     >> 1238 RERAISE                  0
-                 >> 1240 COPY                     3
-                    1242 POP_EXCEPT
-                    1244 RERAISE                  1
-         
-         804     >> 1246 LOAD_FAST                1 (mode)
-                    1248 LOAD_METHOD              0 (lower)
-                    1270 PRECALL                  0
-                    1274 CALL                     0
-                    1284 LOAD_CONST               9 ('dark')
-                    1286 COMPARE_OP               2 (==)
-                    1292 POP_JUMP_FORWARD_IF_FALSE    22 (to 1338)
-         
-         805        1294 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                    1306 LOAD_GLOBAL             18 (bilibili_dark_theme)
-                    1318 PRECALL                  1
-                    1322 CALL                     1
-                    1332 POP_TOP
-                    1334 LOAD_CONST               0 (None)
-                    1336 RETURN_VALUE
-         
-         807     >> 1338 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                    1350 LOAD_GLOBAL             20 (bilibili_theme)
-                    1362 PRECALL                  1
-                    1366 CALL                     1
-                    1376 POP_TOP
-                    1378 LOAD_CONST               0 (None)
-                    1380 RETURN_VALUE
-         
-         808     >> 1382 LOAD_FAST                0 (theme)
-                    1384 LOAD_CONST              14 ('metro')
-                    1386 COMPARE_OP               2 (==)
-                    1392 POP_JUMP_FORWARD_IF_TRUE     6 (to 1406)
-                    1394 LOAD_FAST                0 (theme)
-                    1396 LOAD_CONST              15 ('Metro')
-                    1398 COMPARE_OP               2 (==)
-                    1404 POP_JUMP_FORWARD_IF_FALSE   214 (to 1834)
-         
-         809     >> 1406 LOAD_FAST                1 (mode)
-                    1408 LOAD_METHOD              0 (lower)
-                    1430 PRECALL                  0
-                    1434 CALL                     0
-                    1444 LOAD_CONST               5 ('system')
-                    1446 COMPARE_OP               2 (==)
-                    1452 POP_JUMP_FORWARD_IF_TRUE    24 (to 1502)
-                    1454 LOAD_FAST                1 (mode)
-                    1456 LOAD_METHOD              0 (lower)
-                    1478 PRECALL                  0
-                    1482 CALL                     0
-                    1492 LOAD_CONST               6 ('auto')
-                    1494 COMPARE_OP               2 (==)
-                    1500 POP_JUMP_FORWARD_IF_FALSE    98 (to 1698)
-         
-         810     >> 1502 NOP
-         
-         811        1504 LOAD_CONST               7 (0)
-                    1506 LOAD_CONST               8 (('isDark',))
-                    1508 IMPORT_NAME              1 (darkdetect)
-                    1510 IMPORT_FROM              2 (isDark)
-                    1512 STORE_FAST               2 (isDark)
-                    1514 POP_TOP
-         
-         815        1516 PUSH_NULL
-                    1518 LOAD_FAST                2 (isDark)
-                    1520 PRECALL                  0
-                    1524 CALL                     0
-                    1534 POP_JUMP_FORWARD_IF_FALSE    22 (to 1580)
-         
-         816        1536 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                    1548 LOAD_GLOBAL             22 (metro_dark_theme)
-                    1560 PRECALL                  1
-                    1564 CALL                     1
-                    1574 POP_TOP
-                    1576 LOAD_CONST               0 (None)
-                    1578 RETURN_VALUE
-         
-         818     >> 1580 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                    1592 LOAD_GLOBAL             24 (metro_theme)
-                    1604 PRECALL                  1
-                    1608 CALL                     1
-                    1618 POP_TOP
-                    1620 LOAD_CONST               0 (None)
-                    1622 RETURN_VALUE
-                 >> 1624 PUSH_EXC_INFO
-         
-         812        1626 LOAD_GLOBAL             12 (ModuleNotFoundError)
-                    1638 CHECK_EXC_MATCH
-                    1640 POP_JUMP_FORWARD_IF_FALSE    24 (to 1690)
-                    1642 POP_TOP
-         
-         813        1644 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                    1656 LOAD_GLOBAL             24 (metro_theme)
-                    1668 PRECALL                  1
-                    1672 CALL                     1
-                    1682 POP_TOP
-                    1684 POP_EXCEPT
-                    1686 LOAD_CONST               0 (None)
-                    1688 RETURN_VALUE
-         
-         812     >> 1690 RERAISE                  0
-                 >> 1692 COPY                     3
-                    1694 POP_EXCEPT
-                    1696 RERAISE                  1
-         
-         819     >> 1698 LOAD_FAST                1 (mode)
-                    1700 LOAD_METHOD              0 (lower)
-                    1722 PRECALL                  0
-                    1726 CALL                     0
-                    1736 LOAD_CONST               9 ('dark')
-                    1738 COMPARE_OP               2 (==)
-                    1744 POP_JUMP_FORWARD_IF_FALSE    22 (to 1790)
-         
-         820        1746 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                    1758 LOAD_GLOBAL             22 (metro_dark_theme)
-                    1770 PRECALL                  1
-                    1774 CALL                     1
-                    1784 POP_TOP
-                    1786 LOAD_CONST               0 (None)
-                    1788 RETURN_VALUE
-         
-         822     >> 1790 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                    1802 LOAD_GLOBAL             24 (metro_theme)
-                    1814 PRECALL                  1
-                    1818 CALL                     1
-                    1828 POP_TOP
-                    1830 LOAD_CONST               0 (None)
-                    1832 RETURN_VALUE
-         
-         824     >> 1834 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                    1846 LOAD_FAST                0 (theme)
-                    1848 PRECALL                  1
-                    1852 CALL                     1
-                    1862 POP_TOP
-                    1864 LOAD_CONST               0 (None)
-                    1866 RETURN_VALUE
+            00640053007c0064106b020000000073067c0064116b020000000072d67c
+            01a0000000000000000000000000000000000000000000a6000000ab0000
+            0000000000000064056b020000000073187c01a000000000000000000000
+            0000000000000000000000a6000000ab00000000000000000064066b0200
+            00000072620900640764086c016d027d02010002007c02a6000000ab0000
+            000000000000007216740700000000000000000000741a00000000000000
+            000000a6010000ab01000000000000000001006400530074070000000000
+            0000000000741c00000000000000000000a6010000ab0100000000000000
+            000100640053002300740c00000000000000000000240072180100740700
+            000000000000000000741c00000000000000000000a6010000ab01000000
+            0000000000010059006400530077007803590077017c01a0000000000000
+            000000000000000000000000000000a6000000ab00000000000000000064
+            096b02000000007216740700000000000000000000741a00000000000000
+            000000a6010000ab01000000000000000001006400530074070000000000
+            0000000000741c00000000000000000000a6010000ab0100000000000000
+            000100640053007407000000000000000000007c00a6010000ab01000000
+            0000000000010064005300
+          957           0 RESUME                   0
+         
+          958           2 LOAD_FAST                0 (theme)
+                        4 LOAD_CONST               1 ('win11')
+                        6 COMPARE_OP               2 (==)
+                       12 POP_JUMP_FORWARD_IF_TRUE    18 (to 50)
+                       14 LOAD_FAST                0 (theme)
+                       16 LOAD_CONST               2 ('windows11')
+                       18 COMPARE_OP               2 (==)
+                       24 POP_JUMP_FORWARD_IF_TRUE    12 (to 50)
+                       26 LOAD_FAST                0 (theme)
+                       28 LOAD_CONST               3 ('Windows11')
+                       30 COMPARE_OP               2 (==)
+                       36 POP_JUMP_FORWARD_IF_TRUE     6 (to 50)
+                       38 LOAD_FAST                0 (theme)
+                       40 LOAD_CONST               4 ('Win11')
+                       42 COMPARE_OP               2 (==)
+                       48 POP_JUMP_FORWARD_IF_FALSE   214 (to 478)
+         
+          959     >>   50 LOAD_FAST                1 (mode)
+                       52 LOAD_METHOD              0 (lower)
+                       74 PRECALL                  0
+                       78 CALL                     0
+                       88 LOAD_CONST               5 ('system')
+                       90 COMPARE_OP               2 (==)
+                       96 POP_JUMP_FORWARD_IF_TRUE    24 (to 146)
+                       98 LOAD_FAST                1 (mode)
+                      100 LOAD_METHOD              0 (lower)
+                      122 PRECALL                  0
+                      126 CALL                     0
+                      136 LOAD_CONST               6 ('auto')
+                      138 COMPARE_OP               2 (==)
+                      144 POP_JUMP_FORWARD_IF_FALSE    98 (to 342)
+         
+          960     >>  146 NOP
+         
+          961         148 LOAD_CONST               7 (0)
+                      150 LOAD_CONST               8 (('isDark',))
+                      152 IMPORT_NAME              1 (darkdetect)
+                      154 IMPORT_FROM              2 (isDark)
+                      156 STORE_FAST               2 (isDark)
+                      158 POP_TOP
+         
+          965         160 PUSH_NULL
+                      162 LOAD_FAST                2 (isDark)
+                      164 PRECALL                  0
+                      168 CALL                     0
+                      178 POP_JUMP_FORWARD_IF_FALSE    22 (to 224)
+         
+          966         180 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                      192 LOAD_GLOBAL              8 (win11_dark_theme)
+                      204 PRECALL                  1
+                      208 CALL                     1
+                      218 POP_TOP
+                      220 LOAD_CONST               0 (None)
+                      222 RETURN_VALUE
+         
+          968     >>  224 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                      236 LOAD_GLOBAL             10 (win11_theme)
+                      248 PRECALL                  1
+                      252 CALL                     1
+                      262 POP_TOP
+                      264 LOAD_CONST               0 (None)
+                      266 RETURN_VALUE
+                  >>  268 PUSH_EXC_INFO
+         
+          962         270 LOAD_GLOBAL             12 (ModuleNotFoundError)
+                      282 CHECK_EXC_MATCH
+                      284 POP_JUMP_FORWARD_IF_FALSE    24 (to 334)
+                      286 POP_TOP
+         
+          963         288 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                      300 LOAD_GLOBAL             10 (win11_theme)
+                      312 PRECALL                  1
+                      316 CALL                     1
+                      326 POP_TOP
+                      328 POP_EXCEPT
+                      330 LOAD_CONST               0 (None)
+                      332 RETURN_VALUE
+         
+          962     >>  334 RERAISE                  0
+                  >>  336 COPY                     3
+                      338 POP_EXCEPT
+                      340 RERAISE                  1
+         
+          969     >>  342 LOAD_FAST                1 (mode)
+                      344 LOAD_METHOD              0 (lower)
+                      366 PRECALL                  0
+                      370 CALL                     0
+                      380 LOAD_CONST               9 ('dark')
+                      382 COMPARE_OP               2 (==)
+                      388 POP_JUMP_FORWARD_IF_FALSE    22 (to 434)
+         
+          970         390 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                      402 LOAD_GLOBAL              8 (win11_dark_theme)
+                      414 PRECALL                  1
+                      418 CALL                     1
+                      428 POP_TOP
+                      430 LOAD_CONST               0 (None)
+                      432 RETURN_VALUE
+         
+          972     >>  434 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                      446 LOAD_GLOBAL             10 (win11_theme)
+                      458 PRECALL                  1
+                      462 CALL                     1
+                      472 POP_TOP
+                      474 LOAD_CONST               0 (None)
+                      476 RETURN_VALUE
+         
+          973     >>  478 LOAD_FAST                0 (theme)
+                      480 LOAD_CONST              10 ('gtk')
+                      482 COMPARE_OP               2 (==)
+                      488 POP_JUMP_FORWARD_IF_TRUE     6 (to 502)
+                      490 LOAD_FAST                0 (theme)
+                      492 LOAD_CONST              11 ('Gtk')
+                      494 COMPARE_OP               2 (==)
+                      500 POP_JUMP_FORWARD_IF_FALSE   214 (to 930)
+         
+          974     >>  502 LOAD_FAST                1 (mode)
+                      504 LOAD_METHOD              0 (lower)
+                      526 PRECALL                  0
+                      530 CALL                     0
+                      540 LOAD_CONST               5 ('system')
+                      542 COMPARE_OP               2 (==)
+                      548 POP_JUMP_FORWARD_IF_TRUE    24 (to 598)
+                      550 LOAD_FAST                1 (mode)
+                      552 LOAD_METHOD              0 (lower)
+                      574 PRECALL                  0
+                      578 CALL                     0
+                      588 LOAD_CONST               6 ('auto')
+                      590 COMPARE_OP               2 (==)
+                      596 POP_JUMP_FORWARD_IF_FALSE    98 (to 794)
+         
+          975     >>  598 NOP
+         
+          976         600 LOAD_CONST               7 (0)
+                      602 LOAD_CONST               8 (('isDark',))
+                      604 IMPORT_NAME              1 (darkdetect)
+                      606 IMPORT_FROM              2 (isDark)
+                      608 STORE_FAST               2 (isDark)
+                      610 POP_TOP
+         
+          980         612 PUSH_NULL
+                      614 LOAD_FAST                2 (isDark)
+                      616 PRECALL                  0
+                      620 CALL                     0
+                      630 POP_JUMP_FORWARD_IF_FALSE    22 (to 676)
+         
+          981         632 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                      644 LOAD_GLOBAL             14 (gtk_dark_theme)
+                      656 PRECALL                  1
+                      660 CALL                     1
+                      670 POP_TOP
+                      672 LOAD_CONST               0 (None)
+                      674 RETURN_VALUE
+         
+          983     >>  676 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                      688 LOAD_GLOBAL             16 (gtk_theme)
+                      700 PRECALL                  1
+                      704 CALL                     1
+                      714 POP_TOP
+                      716 LOAD_CONST               0 (None)
+                      718 RETURN_VALUE
+                  >>  720 PUSH_EXC_INFO
+         
+          977         722 LOAD_GLOBAL             12 (ModuleNotFoundError)
+                      734 CHECK_EXC_MATCH
+                      736 POP_JUMP_FORWARD_IF_FALSE    24 (to 786)
+                      738 POP_TOP
+         
+          978         740 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                      752 LOAD_GLOBAL             16 (gtk_theme)
+                      764 PRECALL                  1
+                      768 CALL                     1
+                      778 POP_TOP
+                      780 POP_EXCEPT
+                      782 LOAD_CONST               0 (None)
+                      784 RETURN_VALUE
+         
+          977     >>  786 RERAISE                  0
+                  >>  788 COPY                     3
+                      790 POP_EXCEPT
+                      792 RERAISE                  1
+         
+          985     >>  794 LOAD_FAST                1 (mode)
+                      796 LOAD_METHOD              0 (lower)
+                      818 PRECALL                  0
+                      822 CALL                     0
+                      832 LOAD_CONST               9 ('dark')
+                      834 COMPARE_OP               2 (==)
+                      840 POP_JUMP_FORWARD_IF_FALSE    22 (to 886)
+         
+          986         842 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                      854 LOAD_GLOBAL             14 (gtk_dark_theme)
+                      866 PRECALL                  1
+                      870 CALL                     1
+                      880 POP_TOP
+                      882 LOAD_CONST               0 (None)
+                      884 RETURN_VALUE
+         
+          988     >>  886 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                      898 LOAD_GLOBAL             16 (gtk_theme)
+                      910 PRECALL                  1
+                      914 CALL                     1
+                      924 POP_TOP
+                      926 LOAD_CONST               0 (None)
+                      928 RETURN_VALUE
+         
+          989     >>  930 LOAD_FAST                0 (theme)
+                      932 LOAD_CONST              12 ('bilibili')
+                      934 COMPARE_OP               2 (==)
+                      940 POP_JUMP_FORWARD_IF_TRUE     6 (to 954)
+                      942 LOAD_FAST                0 (theme)
+                      944 LOAD_CONST              13 ('BiliBili')
+                      946 COMPARE_OP               2 (==)
+                      952 POP_JUMP_FORWARD_IF_FALSE   214 (to 1382)
+         
+          990     >>  954 LOAD_FAST                1 (mode)
+                      956 LOAD_METHOD              0 (lower)
+                      978 PRECALL                  0
+                      982 CALL                     0
+                      992 LOAD_CONST               5 ('system')
+                      994 COMPARE_OP               2 (==)
+                     1000 POP_JUMP_FORWARD_IF_TRUE    24 (to 1050)
+                     1002 LOAD_FAST                1 (mode)
+                     1004 LOAD_METHOD              0 (lower)
+                     1026 PRECALL                  0
+                     1030 CALL                     0
+                     1040 LOAD_CONST               6 ('auto')
+                     1042 COMPARE_OP               2 (==)
+                     1048 POP_JUMP_FORWARD_IF_FALSE    98 (to 1246)
+         
+          991     >> 1050 NOP
+         
+          992        1052 LOAD_CONST               7 (0)
+                     1054 LOAD_CONST               8 (('isDark',))
+                     1056 IMPORT_NAME              1 (darkdetect)
+                     1058 IMPORT_FROM              2 (isDark)
+                     1060 STORE_FAST               2 (isDark)
+                     1062 POP_TOP
+         
+          996        1064 PUSH_NULL
+                     1066 LOAD_FAST                2 (isDark)
+                     1068 PRECALL                  0
+                     1072 CALL                     0
+                     1082 POP_JUMP_FORWARD_IF_FALSE    22 (to 1128)
+         
+          997        1084 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     1096 LOAD_GLOBAL             18 (bilibili_dark_theme)
+                     1108 PRECALL                  1
+                     1112 CALL                     1
+                     1122 POP_TOP
+                     1124 LOAD_CONST               0 (None)
+                     1126 RETURN_VALUE
+         
+          999     >> 1128 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     1140 LOAD_GLOBAL             20 (bilibili_theme)
+                     1152 PRECALL                  1
+                     1156 CALL                     1
+                     1166 POP_TOP
+                     1168 LOAD_CONST               0 (None)
+                     1170 RETURN_VALUE
+                  >> 1172 PUSH_EXC_INFO
+         
+          993        1174 LOAD_GLOBAL             12 (ModuleNotFoundError)
+                     1186 CHECK_EXC_MATCH
+                     1188 POP_JUMP_FORWARD_IF_FALSE    24 (to 1238)
+                     1190 POP_TOP
+         
+          994        1192 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     1204 LOAD_GLOBAL             20 (bilibili_theme)
+                     1216 PRECALL                  1
+                     1220 CALL                     1
+                     1230 POP_TOP
+                     1232 POP_EXCEPT
+                     1234 LOAD_CONST               0 (None)
+                     1236 RETURN_VALUE
+         
+          993     >> 1238 RERAISE                  0
+                  >> 1240 COPY                     3
+                     1242 POP_EXCEPT
+                     1244 RERAISE                  1
+         
+         1000     >> 1246 LOAD_FAST                1 (mode)
+                     1248 LOAD_METHOD              0 (lower)
+                     1270 PRECALL                  0
+                     1274 CALL                     0
+                     1284 LOAD_CONST               9 ('dark')
+                     1286 COMPARE_OP               2 (==)
+                     1292 POP_JUMP_FORWARD_IF_FALSE    22 (to 1338)
+         
+         1001        1294 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     1306 LOAD_GLOBAL             18 (bilibili_dark_theme)
+                     1318 PRECALL                  1
+                     1322 CALL                     1
+                     1332 POP_TOP
+                     1334 LOAD_CONST               0 (None)
+                     1336 RETURN_VALUE
+         
+         1003     >> 1338 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     1350 LOAD_GLOBAL             20 (bilibili_theme)
+                     1362 PRECALL                  1
+                     1366 CALL                     1
+                     1376 POP_TOP
+                     1378 LOAD_CONST               0 (None)
+                     1380 RETURN_VALUE
+         
+         1004     >> 1382 LOAD_FAST                0 (theme)
+                     1384 LOAD_CONST              14 ('metro')
+                     1386 COMPARE_OP               2 (==)
+                     1392 POP_JUMP_FORWARD_IF_TRUE     6 (to 1406)
+                     1394 LOAD_FAST                0 (theme)
+                     1396 LOAD_CONST              15 ('Metro')
+                     1398 COMPARE_OP               2 (==)
+                     1404 POP_JUMP_FORWARD_IF_FALSE   214 (to 1834)
+         
+         1005     >> 1406 LOAD_FAST                1 (mode)
+                     1408 LOAD_METHOD              0 (lower)
+                     1430 PRECALL                  0
+                     1434 CALL                     0
+                     1444 LOAD_CONST               5 ('system')
+                     1446 COMPARE_OP               2 (==)
+                     1452 POP_JUMP_FORWARD_IF_TRUE    24 (to 1502)
+                     1454 LOAD_FAST                1 (mode)
+                     1456 LOAD_METHOD              0 (lower)
+                     1478 PRECALL                  0
+                     1482 CALL                     0
+                     1492 LOAD_CONST               6 ('auto')
+                     1494 COMPARE_OP               2 (==)
+                     1500 POP_JUMP_FORWARD_IF_FALSE    98 (to 1698)
+         
+         1006     >> 1502 NOP
+         
+         1007        1504 LOAD_CONST               7 (0)
+                     1506 LOAD_CONST               8 (('isDark',))
+                     1508 IMPORT_NAME              1 (darkdetect)
+                     1510 IMPORT_FROM              2 (isDark)
+                     1512 STORE_FAST               2 (isDark)
+                     1514 POP_TOP
+         
+         1011        1516 PUSH_NULL
+                     1518 LOAD_FAST                2 (isDark)
+                     1520 PRECALL                  0
+                     1524 CALL                     0
+                     1534 POP_JUMP_FORWARD_IF_FALSE    22 (to 1580)
+         
+         1012        1536 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     1548 LOAD_GLOBAL             22 (metro_dark_theme)
+                     1560 PRECALL                  1
+                     1564 CALL                     1
+                     1574 POP_TOP
+                     1576 LOAD_CONST               0 (None)
+                     1578 RETURN_VALUE
+         
+         1014     >> 1580 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     1592 LOAD_GLOBAL             24 (metro_theme)
+                     1604 PRECALL                  1
+                     1608 CALL                     1
+                     1618 POP_TOP
+                     1620 LOAD_CONST               0 (None)
+                     1622 RETURN_VALUE
+                  >> 1624 PUSH_EXC_INFO
+         
+         1008        1626 LOAD_GLOBAL             12 (ModuleNotFoundError)
+                     1638 CHECK_EXC_MATCH
+                     1640 POP_JUMP_FORWARD_IF_FALSE    24 (to 1690)
+                     1642 POP_TOP
+         
+         1009        1644 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     1656 LOAD_GLOBAL             24 (metro_theme)
+                     1668 PRECALL                  1
+                     1672 CALL                     1
+                     1682 POP_TOP
+                     1684 POP_EXCEPT
+                     1686 LOAD_CONST               0 (None)
+                     1688 RETURN_VALUE
+         
+         1008     >> 1690 RERAISE                  0
+                  >> 1692 COPY                     3
+                     1694 POP_EXCEPT
+                     1696 RERAISE                  1
+         
+         1015     >> 1698 LOAD_FAST                1 (mode)
+                     1700 LOAD_METHOD              0 (lower)
+                     1722 PRECALL                  0
+                     1726 CALL                     0
+                     1736 LOAD_CONST               9 ('dark')
+                     1738 COMPARE_OP               2 (==)
+                     1744 POP_JUMP_FORWARD_IF_FALSE    22 (to 1790)
+         
+         1016        1746 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     1758 LOAD_GLOBAL             22 (metro_dark_theme)
+                     1770 PRECALL                  1
+                     1774 CALL                     1
+                     1784 POP_TOP
+                     1786 LOAD_CONST               0 (None)
+                     1788 RETURN_VALUE
+         
+         1018     >> 1790 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     1802 LOAD_GLOBAL             24 (metro_theme)
+                     1814 PRECALL                  1
+                     1818 CALL                     1
+                     1828 POP_TOP
+                     1830 LOAD_CONST               0 (None)
+                     1832 RETURN_VALUE
+         
+         1019     >> 1834 LOAD_FAST                0 (theme)
+                     1836 LOAD_CONST              16 ('basic')
+                     1838 COMPARE_OP               2 (==)
+                     1844 POP_JUMP_FORWARD_IF_TRUE     6 (to 1858)
+                     1846 LOAD_FAST                0 (theme)
+                     1848 LOAD_CONST              17 ('Basic')
+                     1850 COMPARE_OP               2 (==)
+                     1856 POP_JUMP_FORWARD_IF_FALSE   214 (to 2286)
+         
+         1020     >> 1858 LOAD_FAST                1 (mode)
+                     1860 LOAD_METHOD              0 (lower)
+                     1882 PRECALL                  0
+                     1886 CALL                     0
+                     1896 LOAD_CONST               5 ('system')
+                     1898 COMPARE_OP               2 (==)
+                     1904 POP_JUMP_FORWARD_IF_TRUE    24 (to 1954)
+                     1906 LOAD_FAST                1 (mode)
+                     1908 LOAD_METHOD              0 (lower)
+                     1930 PRECALL                  0
+                     1934 CALL                     0
+                     1944 LOAD_CONST               6 ('auto')
+                     1946 COMPARE_OP               2 (==)
+                     1952 POP_JUMP_FORWARD_IF_FALSE    98 (to 2150)
+         
+         1021     >> 1954 NOP
+         
+         1022        1956 LOAD_CONST               7 (0)
+                     1958 LOAD_CONST               8 (('isDark',))
+                     1960 IMPORT_NAME              1 (darkdetect)
+                     1962 IMPORT_FROM              2 (isDark)
+                     1964 STORE_FAST               2 (isDark)
+                     1966 POP_TOP
+         
+         1026        1968 PUSH_NULL
+                     1970 LOAD_FAST                2 (isDark)
+                     1972 PRECALL                  0
+                     1976 CALL                     0
+                     1986 POP_JUMP_FORWARD_IF_FALSE    22 (to 2032)
+         
+         1027        1988 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     2000 LOAD_GLOBAL             26 (basic_dark_theme)
+                     2012 PRECALL                  1
+                     2016 CALL                     1
+                     2026 POP_TOP
+                     2028 LOAD_CONST               0 (None)
+                     2030 RETURN_VALUE
+         
+         1029     >> 2032 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     2044 LOAD_GLOBAL             28 (basic_theme)
+                     2056 PRECALL                  1
+                     2060 CALL                     1
+                     2070 POP_TOP
+                     2072 LOAD_CONST               0 (None)
+                     2074 RETURN_VALUE
+                  >> 2076 PUSH_EXC_INFO
+         
+         1023        2078 LOAD_GLOBAL             12 (ModuleNotFoundError)
+                     2090 CHECK_EXC_MATCH
+                     2092 POP_JUMP_FORWARD_IF_FALSE    24 (to 2142)
+                     2094 POP_TOP
+         
+         1024        2096 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     2108 LOAD_GLOBAL             28 (basic_theme)
+                     2120 PRECALL                  1
+                     2124 CALL                     1
+                     2134 POP_TOP
+                     2136 POP_EXCEPT
+                     2138 LOAD_CONST               0 (None)
+                     2140 RETURN_VALUE
+         
+         1023     >> 2142 RERAISE                  0
+                  >> 2144 COPY                     3
+                     2146 POP_EXCEPT
+                     2148 RERAISE                  1
+         
+         1030     >> 2150 LOAD_FAST                1 (mode)
+                     2152 LOAD_METHOD              0 (lower)
+                     2174 PRECALL                  0
+                     2178 CALL                     0
+                     2188 LOAD_CONST               9 ('dark')
+                     2190 COMPARE_OP               2 (==)
+                     2196 POP_JUMP_FORWARD_IF_FALSE    22 (to 2242)
+         
+         1031        2198 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     2210 LOAD_GLOBAL             26 (basic_dark_theme)
+                     2222 PRECALL                  1
+                     2226 CALL                     1
+                     2236 POP_TOP
+                     2238 LOAD_CONST               0 (None)
+                     2240 RETURN_VALUE
+         
+         1033     >> 2242 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     2254 LOAD_GLOBAL             28 (basic_theme)
+                     2266 PRECALL                  1
+                     2270 CALL                     1
+                     2280 POP_TOP
+                     2282 LOAD_CONST               0 (None)
+                     2284 RETURN_VALUE
+         
+         1035     >> 2286 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     2298 LOAD_FAST                0 (theme)
+                     2300 PRECALL                  1
+                     2304 CALL                     1
+                     2314 POP_TOP
+                     2316 LOAD_CONST               0 (None)
+                     2318 RETURN_VALUE
          ExceptionTable:
            148 to 158 -> 268 [0]
            268 to 326 -> 336 [1] lasti
            334 to 334 -> 336 [1] lasti
            600 to 610 -> 720 [0]
            720 to 778 -> 788 [1] lasti
            786 to 786 -> 788 [1] lasti
            1052 to 1062 -> 1172 [0]
            1172 to 1230 -> 1240 [1] lasti
            1238 to 1238 -> 1240 [1] lasti
            1504 to 1514 -> 1624 [0]
            1624 to 1682 -> 1692 [1] lasti
            1690 to 1690 -> 1692 [1] lasti
+           1956 to 1966 -> 2076 [0]
+           2076 to 2134 -> 2144 [1] lasti
+           2142 to 2142 -> 2144 [1] lasti
          consts
             None
             'win11'
             'windows11'
             'Windows11'
             'Win11'
             'system'
@@ -2177,634 +2608,615 @@
             'dark'
             'gtk'
             'Gtk'
             'bilibili'
             'BiliBili'
             'metro'
             'Metro'
-         names      ('lower', 'darkdetect', 'isDark', '_set_default_theme', 'win11_dark_theme', 'win11_theme', 'ModuleNotFoundError', 'gtk_dark_theme', 'gtk_theme', 'bilibili_dark_theme', 'bilibili_theme', 'metro_dark_theme', 'metro_theme')
+            'basic'
+            'Basic'
+         names      ('lower', 'darkdetect', 'isDark', '_set_default_theme', 'win11_dark_theme', 'win11_theme', 'ModuleNotFoundError', 'gtk_dark_theme', 'gtk_theme', 'bilibili_dark_theme', 'bilibili_theme', 'metro_dark_theme', 'metro_theme', 'basic_dark_theme', 'basic_theme')
          varnames   ('theme', 'mode', 'isDark')
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'set_default_theme'
-         firstlineno 761
+         firstlineno 957
          lnotab
             0x02013001600102010c0414012c022efa12012eff080730012c022c0118
             01600102010c0414012c022efa12012eff080830012c022c011801600102
             010c0414012c022efa12012eff080730012c022c011801600102010c0414
-            012c022efa12012eff080730012c022c02
+            012c022efa12012eff080730012c022c011801600102010c0414012c022e
+            fa12012eff080730012c022c02
       'win11'
       ('Adw',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code 0x970065005a0164005a026405640284015a03640384005a0464045300
-         833           0 RESUME                   0
-                       2 LOAD_NAME                0 (__name__)
-                       4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('Adwite')
-                       8 STORE_NAME               2 (__qualname__)
-         
-         834          10 LOAD_CONST               5 (('auto',))
-                      12 LOAD_CONST               2 (<code object set_default_theme, file "D:\tkadw\tkadw\windows\theme.py", line 834>)
-                      14 MAKE_FUNCTION            1 (defaults)
-                      16 STORE_NAME               3 (set_default_theme)
-         
-         843          18 LOAD_CONST               3 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 843>)
-                      20 MAKE_FUNCTION            0
-                      22 STORE_NAME               4 (default_palette)
-                      24 LOAD_CONST               4 (None)
-                      26 RETURN_VALUE
+         1044           0 RESUME                   0
+                        2 LOAD_NAME                0 (__name__)
+                        4 STORE_NAME               1 (__module__)
+                        6 LOAD_CONST               0 ('Adwite')
+                        8 STORE_NAME               2 (__qualname__)
+         
+         1045          10 LOAD_CONST               5 (('auto',))
+                       12 LOAD_CONST               2 (<code object set_default_theme, file "D:\tkadw\tkadw\windows\theme.py", line 1045>)
+                       14 MAKE_FUNCTION            1 (defaults)
+                       16 STORE_NAME               3 (set_default_theme)
+         
+         1054          18 LOAD_CONST               3 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 1054>)
+                       20 MAKE_FUNCTION            0
+                       22 STORE_NAME               4 (default_palette)
+                       24 LOAD_CONST               4 (None)
+                       26 RETURN_VALUE
          consts
             'Adwite'
             'auto'
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 6
                flags     : 3
                code
                   0x97007401000000000000000000007c017c02a6020000ab020000000000
                   00000001007c00a0010000000000000000000000000000000000000000a6
-                  000000ab00000000000000000044005d767d037405000000000000000000
-                  007c036401a6020000ab02000000000000000072647c03a0030000000000
+                  000000ab00000000000000000044005d757d037405000000000000000000
+                  007c036401a6020000ab02000000000000000072637c03a0030000000000
                   000000000000000000000000000000740900000000000000000000a60000
                   00ab000000000000000000a6010000ab01000000000000000001007c03a0
                   0500000000000000000000000000000000000000007c036a060000000000
                   000000a00700000000000000000000000000000000000000006402a60100
                   00ab010000000000000000ac03a6010000ab01000000000000000001007c
-                  03a00800000000000000000000000000000000000000006400a6010000ab
-                  01000000000000000001008c777c00a00300000000000000000000000000
-                  00000000000000740900000000000000000000a6000000ab000000000000
-                  000000a6010000ab010000000000000000010064005300
-               834           0 RESUME                   0
+                  03a0080000000000000000000000000000000000000000a6000000ab0000
+                  0000000000000001008c767c00a003000000000000000000000000000000
+                  0000000000740900000000000000000000a6000000ab0000000000000000
+                  00a6010000ab010000000000000000010064005300
+               1045           0 RESUME                   0
                
-               835           2 LOAD_GLOBAL              1 (NULL + set_default_theme)
-                            14 LOAD_FAST                1 (theme)
-                            16 LOAD_FAST                2 (_mode)
-                            18 PRECALL                  2
-                            22 CALL                     2
-                            32 POP_TOP
+               1046           2 LOAD_GLOBAL              1 (NULL + set_default_theme)
+                             14 LOAD_FAST                1 (theme)
+                             16 LOAD_FAST                2 (_mode)
+                             18 PRECALL                  2
+                             22 CALL                     2
+                             32 POP_TOP
                
-               836          34 LOAD_FAST                0 (self)
-                            36 LOAD_METHOD              1 (winfo_children)
-                            58 PRECALL                  0
-                            62 CALL                     0
-                            72 GET_ITER
-                       >>   74 FOR_ITER               118 (to 312)
-                            76 STORE_FAST               3 (widget)
+               1047          34 LOAD_FAST                0 (self)
+                             36 LOAD_METHOD              1 (winfo_children)
+                             58 PRECALL                  0
+                             62 CALL                     0
+                             72 GET_ITER
+                        >>   74 FOR_ITER               117 (to 310)
+                             76 STORE_FAST               3 (widget)
                
-               837          78 LOAD_GLOBAL              5 (NULL + hasattr)
-                            90 LOAD_FAST                3 (widget)
-                            92 LOAD_CONST               1 ('palette')
-                            94 PRECALL                  2
-                            98 CALL                     2
-                           108 POP_JUMP_FORWARD_IF_FALSE   100 (to 310)
+               1048          78 LOAD_GLOBAL              5 (NULL + hasattr)
+                             90 LOAD_FAST                3 (widget)
+                             92 LOAD_CONST               1 ('palette')
+                             94 PRECALL                  2
+                             98 CALL                     2
+                            108 POP_JUMP_FORWARD_IF_FALSE    99 (to 308)
                
-               838         110 LOAD_FAST                3 (widget)
-                           112 LOAD_METHOD              3 (palette)
-                           134 LOAD_GLOBAL              9 (NULL + get_default_theme)
-                           146 PRECALL                  0
-                           150 CALL                     0
-                           160 PRECALL                  1
-                           164 CALL                     1
-                           174 POP_TOP
+               1049         110 LOAD_FAST                3 (widget)
+                            112 LOAD_METHOD              3 (palette)
+                            134 LOAD_GLOBAL              9 (NULL + get_default_theme)
+                            146 PRECALL                  0
+                            150 CALL                     0
+                            160 PRECALL                  1
+                            164 CALL                     1
+                            174 POP_TOP
                
-               839         176 LOAD_FAST                3 (widget)
-                           178 LOAD_METHOD              5 (configure)
-                           200 LOAD_FAST                3 (widget)
-                           202 LOAD_ATTR                6 (master)
-                           212 LOAD_METHOD              7 (cget)
-                           234 LOAD_CONST               2 ('bg')
-                           236 PRECALL                  1
-                           240 CALL                     1
-                           250 KW_NAMES                 3
-                           252 PRECALL                  1
-                           256 CALL                     1
-                           266 POP_TOP
+               1050         176 LOAD_FAST                3 (widget)
+                            178 LOAD_METHOD              5 (configure)
+                            200 LOAD_FAST                3 (widget)
+                            202 LOAD_ATTR                6 (master)
+                            212 LOAD_METHOD              7 (cget)
+                            234 LOAD_CONST               2 ('bg')
+                            236 PRECALL                  1
+                            240 CALL                     1
+                            250 KW_NAMES                 3
+                            252 PRECALL                  1
+                            256 CALL                     1
+                            266 POP_TOP
                
-               840         268 LOAD_FAST                3 (widget)
-                           270 LOAD_METHOD              8 (_draw)
-                           292 LOAD_CONST               0 (None)
-                           294 PRECALL                  1
-                           298 CALL                     1
-                           308 POP_TOP
-                       >>  310 JUMP_BACKWARD          119 (to 74)
+               1051         268 LOAD_FAST                3 (widget)
+                            270 LOAD_METHOD              8 (update)
+                            292 PRECALL                  0
+                            296 CALL                     0
+                            306 POP_TOP
+                        >>  308 JUMP_BACKWARD          118 (to 74)
                
-               841     >>  312 LOAD_FAST                0 (self)
-                           314 LOAD_METHOD              3 (palette)
-                           336 LOAD_GLOBAL              9 (NULL + get_default_theme)
-                           348 PRECALL                  0
-                           352 CALL                     0
-                           362 PRECALL                  1
-                           366 CALL                     1
-                           376 POP_TOP
-                           378 LOAD_CONST               0 (None)
-                           380 RETURN_VALUE
+               1052     >>  310 LOAD_FAST                0 (self)
+                            312 LOAD_METHOD              3 (palette)
+                            334 LOAD_GLOBAL              9 (NULL + get_default_theme)
+                            346 PRECALL                  0
+                            350 CALL                     0
+                            360 PRECALL                  1
+                            364 CALL                     1
+                            374 POP_TOP
+                            376 LOAD_CONST               0 (None)
+                            378 RETURN_VALUE
                consts
                   None
                   'palette'
                   'bg'
                   ('background',)
-               names      ('set_default_theme', 'winfo_children', 'hasattr', 'palette', 'get_default_theme', 'configure', 'master', 'cget', '_draw')
+               names      ('set_default_theme', 'winfo_children', 'hasattr', 'palette', 'get_default_theme', 'configure', 'master', 'cget', 'update')
                varnames   ('self', 'theme', '_mode', 'widget')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
                name       'set_default_theme'
-               firstlineno 834
-               lnotab 0x020120012c01200142015c012c01
+               firstlineno 1045
+               lnotab 0x020120012c01200142015c012a01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000740300
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   00000000000000010064005300
-               843           0 RESUME                   0
+               1054           0 RESUME                   0
                
-               844           2 LOAD_FAST                0 (self)
-                             4 LOAD_METHOD              0 (palette)
-                            26 LOAD_GLOBAL              3 (NULL + get_default_theme)
-                            38 PRECALL                  0
-                            42 CALL                     0
-                            52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+               1055           2 LOAD_FAST                0 (self)
+                              4 LOAD_METHOD              0 (palette)
+                             26 LOAD_GLOBAL              3 (NULL + get_default_theme)
+                             38 PRECALL                  0
+                             42 CALL                     0
+                             52 PRECALL                  1
+                             56 CALL                     1
+                             66 POP_TOP
+                             68 LOAD_CONST               0 (None)
+                             70 RETURN_VALUE
                consts
                   None
                names      ('palette', 'get_default_theme')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
                name       'default_palette'
-               firstlineno 843
+               firstlineno 1054
                lnotab 0x0201
             None
             ('auto',)
          names      ('__name__', '__module__', '__qualname__', 'set_default_theme', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'Adwite'
-         firstlineno 833
+         firstlineno 1044
          lnotab 0x0a010809
       'Adwite'
       ('AdwLabel',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         850           0 RESUME                   0
-                       2 LOAD_NAME                0 (__name__)
-                       4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('AdwTLabel')
-                       8 STORE_NAME               2 (__qualname__)
-         
-         851          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 851>)
-                      12 MAKE_FUNCTION            0
-                      14 STORE_NAME               3 (default_palette)
-                      16 LOAD_CONST               2 (None)
-                      18 RETURN_VALUE
+         1061           0 RESUME                   0
+                        2 LOAD_NAME                0 (__name__)
+                        4 STORE_NAME               1 (__module__)
+                        6 LOAD_CONST               0 ('AdwTLabel')
+                        8 STORE_NAME               2 (__qualname__)
+         
+         1062          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 1062>)
+                       12 MAKE_FUNCTION            0
+                       14 STORE_NAME               3 (default_palette)
+                       16 LOAD_CONST               2 (None)
+                       18 RETURN_VALUE
          consts
             'AdwTLabel'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000740300
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   00000000000000010064005300
-               851           0 RESUME                   0
+               1062           0 RESUME                   0
                
-               852           2 LOAD_FAST                0 (self)
-                             4 LOAD_METHOD              0 (palette)
-                            26 LOAD_GLOBAL              3 (NULL + get_default_theme)
-                            38 PRECALL                  0
-                            42 CALL                     0
-                            52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+               1063           2 LOAD_FAST                0 (self)
+                              4 LOAD_METHOD              0 (palette)
+                             26 LOAD_GLOBAL              3 (NULL + get_default_theme)
+                             38 PRECALL                  0
+                             42 CALL                     0
+                             52 PRECALL                  1
+                             56 CALL                     1
+                             66 POP_TOP
+                             68 LOAD_CONST               0 (None)
+                             70 RETURN_VALUE
                consts
                   None
                names      ('palette', 'get_default_theme')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
                name       'default_palette'
-               firstlineno 851
+               firstlineno 1062
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'AdwTLabel'
-         firstlineno 850
+         firstlineno 1061
          lnotab 0x0a01
       'AdwTLabel'
       ('AdwDrawRoundButton3',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         858           0 RESUME                   0
-                       2 LOAD_NAME                0 (__name__)
-                       4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('AdwTButton')
-                       8 STORE_NAME               2 (__qualname__)
-         
-         859          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 859>)
-                      12 MAKE_FUNCTION            0
-                      14 STORE_NAME               3 (default_palette)
-                      16 LOAD_CONST               2 (None)
-                      18 RETURN_VALUE
+         1069           0 RESUME                   0
+                        2 LOAD_NAME                0 (__name__)
+                        4 STORE_NAME               1 (__module__)
+                        6 LOAD_CONST               0 ('AdwTButton')
+                        8 STORE_NAME               2 (__qualname__)
+         
+         1070          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 1070>)
+                       12 MAKE_FUNCTION            0
+                       14 STORE_NAME               3 (default_palette)
+                       16 LOAD_CONST               2 (None)
+                       18 RETURN_VALUE
          consts
             'AdwTButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000740300
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   00000000000000010064005300
-               859           0 RESUME                   0
+               1070           0 RESUME                   0
                
-               860           2 LOAD_FAST                0 (self)
-                             4 LOAD_METHOD              0 (palette)
-                            26 LOAD_GLOBAL              3 (NULL + get_default_theme)
-                            38 PRECALL                  0
-                            42 CALL                     0
-                            52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+               1071           2 LOAD_FAST                0 (self)
+                              4 LOAD_METHOD              0 (palette)
+                             26 LOAD_GLOBAL              3 (NULL + get_default_theme)
+                             38 PRECALL                  0
+                             42 CALL                     0
+                             52 PRECALL                  1
+                             56 CALL                     1
+                             66 POP_TOP
+                             68 LOAD_CONST               0 (None)
+                             70 RETURN_VALUE
                consts
                   None
                names      ('palette', 'get_default_theme')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
                name       'default_palette'
-               firstlineno 859
+               firstlineno 1070
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'AdwTButton'
-         firstlineno 858
+         firstlineno 1069
          lnotab 0x0a01
       'AdwTButton'
       ('AdwDrawRoundEntry3',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         866           0 RESUME                   0
-                       2 LOAD_NAME                0 (__name__)
-                       4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('AdwTEntry')
-                       8 STORE_NAME               2 (__qualname__)
-         
-         867          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 867>)
-                      12 MAKE_FUNCTION            0
-                      14 STORE_NAME               3 (default_palette)
-                      16 LOAD_CONST               2 (None)
-                      18 RETURN_VALUE
+         1077           0 RESUME                   0
+                        2 LOAD_NAME                0 (__name__)
+                        4 STORE_NAME               1 (__module__)
+                        6 LOAD_CONST               0 ('AdwTEntry')
+                        8 STORE_NAME               2 (__qualname__)
+         
+         1078          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 1078>)
+                       12 MAKE_FUNCTION            0
+                       14 STORE_NAME               3 (default_palette)
+                       16 LOAD_CONST               2 (None)
+                       18 RETURN_VALUE
          consts
             'AdwTEntry'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000740300
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   00000000000000010064005300
-               867           0 RESUME                   0
+               1078           0 RESUME                   0
                
-               868           2 LOAD_FAST                0 (self)
-                             4 LOAD_METHOD              0 (palette)
-                            26 LOAD_GLOBAL              3 (NULL + get_default_theme)
-                            38 PRECALL                  0
-                            42 CALL                     0
-                            52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+               1079           2 LOAD_FAST                0 (self)
+                              4 LOAD_METHOD              0 (palette)
+                             26 LOAD_GLOBAL              3 (NULL + get_default_theme)
+                             38 PRECALL                  0
+                             42 CALL                     0
+                             52 PRECALL                  1
+                             56 CALL                     1
+                             66 POP_TOP
+                             68 LOAD_CONST               0 (None)
+                             70 RETURN_VALUE
                consts
                   None
                names      ('palette', 'get_default_theme')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
                name       'default_palette'
-               firstlineno 867
+               firstlineno 1078
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'AdwTEntry'
-         firstlineno 866
+         firstlineno 1077
          lnotab 0x0a01
       'AdwTEntry'
       ('AdwDrawRoundText3',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         874           0 RESUME                   0
-                       2 LOAD_NAME                0 (__name__)
-                       4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('AdwTText')
-                       8 STORE_NAME               2 (__qualname__)
-         
-         875          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 875>)
-                      12 MAKE_FUNCTION            0
-                      14 STORE_NAME               3 (default_palette)
-                      16 LOAD_CONST               2 (None)
-                      18 RETURN_VALUE
+         1085           0 RESUME                   0
+                        2 LOAD_NAME                0 (__name__)
+                        4 STORE_NAME               1 (__module__)
+                        6 LOAD_CONST               0 ('AdwTText')
+                        8 STORE_NAME               2 (__qualname__)
+         
+         1086          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 1086>)
+                       12 MAKE_FUNCTION            0
+                       14 STORE_NAME               3 (default_palette)
+                       16 LOAD_CONST               2 (None)
+                       18 RETURN_VALUE
          consts
             'AdwTText'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000740300
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   00000000000000010064005300
-               875           0 RESUME                   0
+               1086           0 RESUME                   0
                
-               876           2 LOAD_FAST                0 (self)
-                             4 LOAD_METHOD              0 (palette)
-                            26 LOAD_GLOBAL              3 (NULL + get_default_theme)
-                            38 PRECALL                  0
-                            42 CALL                     0
-                            52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+               1087           2 LOAD_FAST                0 (self)
+                              4 LOAD_METHOD              0 (palette)
+                             26 LOAD_GLOBAL              3 (NULL + get_default_theme)
+                             38 PRECALL                  0
+                             42 CALL                     0
+                             52 PRECALL                  1
+                             56 CALL                     1
+                             66 POP_TOP
+                             68 LOAD_CONST               0 (None)
+                             70 RETURN_VALUE
                consts
                   None
                names      ('palette', 'get_default_theme')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
                name       'default_palette'
-               firstlineno 875
+               firstlineno 1086
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'AdwTText'
-         firstlineno 874
+         firstlineno 1085
          lnotab 0x0a01
       'AdwTText'
       ('AdwDrawRoundFrame3',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         882           0 RESUME                   0
-                       2 LOAD_NAME                0 (__name__)
-                       4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('AdwTFrame')
-                       8 STORE_NAME               2 (__qualname__)
-         
-         883          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 883>)
-                      12 MAKE_FUNCTION            0
-                      14 STORE_NAME               3 (default_palette)
-                      16 LOAD_CONST               2 (None)
-                      18 RETURN_VALUE
+         1093           0 RESUME                   0
+                        2 LOAD_NAME                0 (__name__)
+                        4 STORE_NAME               1 (__module__)
+                        6 LOAD_CONST               0 ('AdwTFrame')
+                        8 STORE_NAME               2 (__qualname__)
+         
+         1094          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 1094>)
+                       12 MAKE_FUNCTION            0
+                       14 STORE_NAME               3 (default_palette)
+                       16 LOAD_CONST               2 (None)
+                       18 RETURN_VALUE
          consts
             'AdwTFrame'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000740300
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   00000000000000010064005300
-               883           0 RESUME                   0
+               1094           0 RESUME                   0
                
-               884           2 LOAD_FAST                0 (self)
-                             4 LOAD_METHOD              0 (palette)
-                            26 LOAD_GLOBAL              3 (NULL + get_default_theme)
-                            38 PRECALL                  0
-                            42 CALL                     0
-                            52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+               1095           2 LOAD_FAST                0 (self)
+                              4 LOAD_METHOD              0 (palette)
+                             26 LOAD_GLOBAL              3 (NULL + get_default_theme)
+                             38 PRECALL                  0
+                             42 CALL                     0
+                             52 PRECALL                  1
+                             56 CALL                     1
+                             66 POP_TOP
+                             68 LOAD_CONST               0 (None)
+                             70 RETURN_VALUE
                consts
                   None
                names      ('palette', 'get_default_theme')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
                name       'default_palette'
-               firstlineno 883
+               firstlineno 1094
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'AdwTFrame'
-         firstlineno 882
+         firstlineno 1093
          lnotab 0x0a01
       'AdwTFrame'
       ('AdwDrawSeparator',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         890           0 RESUME                   0
-                       2 LOAD_NAME                0 (__name__)
-                       4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('AdwTSeparator')
-                       8 STORE_NAME               2 (__qualname__)
-         
-         891          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 891>)
-                      12 MAKE_FUNCTION            0
-                      14 STORE_NAME               3 (default_palette)
-                      16 LOAD_CONST               2 (None)
-                      18 RETURN_VALUE
+         1101           0 RESUME                   0
+                        2 LOAD_NAME                0 (__name__)
+                        4 STORE_NAME               1 (__module__)
+                        6 LOAD_CONST               0 ('AdwTSeparator')
+                        8 STORE_NAME               2 (__qualname__)
+         
+         1102          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 1102>)
+                       12 MAKE_FUNCTION            0
+                       14 STORE_NAME               3 (default_palette)
+                       16 LOAD_CONST               2 (None)
+                       18 RETURN_VALUE
          consts
             'AdwTSeparator'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000740300
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   00000000000000010064005300
-               891           0 RESUME                   0
+               1102           0 RESUME                   0
                
-               892           2 LOAD_FAST                0 (self)
-                             4 LOAD_METHOD              0 (palette)
-                            26 LOAD_GLOBAL              3 (NULL + get_default_theme)
-                            38 PRECALL                  0
-                            42 CALL                     0
-                            52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-                            68 LOAD_CONST               0 (None)
-                            70 RETURN_VALUE
+               1103           2 LOAD_FAST                0 (self)
+                              4 LOAD_METHOD              0 (palette)
+                             26 LOAD_GLOBAL              3 (NULL + get_default_theme)
+                             38 PRECALL                  0
+                             42 CALL                     0
+                             52 PRECALL                  1
+                             56 CALL                     1
+                             66 POP_TOP
+                             68 LOAD_CONST               0 (None)
+                             70 RETURN_VALUE
                consts
                   None
                names      ('palette', 'get_default_theme')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
                name       'default_palette'
-               firstlineno 891
+               firstlineno 1102
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'AdwTSeparator'
-         firstlineno 890
+         firstlineno 1101
          lnotab 0x0a01
       'AdwTSeparator'
       '__main__'
       ('isDark',)
-      'metro'
-      code
-         argcount  : 0
-         nlocals   : 0
-         stacksize : 3
-         flags     : 3
-         code
-            0x9700740000000000000000000000a00100000000000000000000000000
-            000000000000006401a6010000ab010000000000000000010064005300
-         901           0 RESUME                   0
-         
-         902           2 LOAD_GLOBAL              0 (root)
-                      14 LOAD_METHOD              1 (set_default_theme)
-                      36 LOAD_CONST               1 ('win11')
-                      38 PRECALL                  1
-                      42 CALL                     1
-                      52 POP_TOP
-                      54 LOAD_CONST               0 (None)
-                      56 RETURN_VALUE
-         consts
-            None
-            'win11'
-         names      ('root', 'set_default_theme')
-         varnames   ()
-         freevars   ()
-         cellvars   ()
-         filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
-         name       'toggle'
-         firstlineno 901
-         lnotab 0x0201
-      ('text', 'command')
+      'dark'
+      ('text',)
       'x'
       5
       ('fill', 'padx', 'pady')
-      ('text',)
       None
       ('system',)
-   names      ('win11_theme', 'win11_dark_theme', 'gtk_theme', 'gtk_dark_theme', 'bilibili_theme', 'bilibili_dark_theme', 'metro_theme', 'metro_dark_theme', 'get_default_theme', '_set_default_theme', 'set_default_theme', 'tkadw.windows.widgets.adw', 'Adw', 'Adwite', 'tkadw.windows.widgets', 'AdwLabel', 'AdwTLabel', 'tkadw.windows.canvas.button', 'AdwDrawRoundButton3', 'AdwTButton', 'tkadw.windows.canvas.entry', 'AdwDrawRoundEntry3', 'AdwTEntry', 'tkadw.windows.canvas.textbox', 'AdwDrawRoundText3', 'AdwTText', 'tkadw.windows.canvas.frame', 'AdwDrawRoundFrame3', 'AdwTFrame', 'tkadw.windows.canvas.separator', 'AdwDrawSeparator', 'AdwTSeparator', '__name__', 'darkdetect', 'isDark', 'root', 'toggle', 'button', 'pack', 'separator', 'entry', 'text', 'frame', 'mainloop')
+   names      ('win11_theme', 'win11_dark_theme', 'gtk_theme', 'gtk_dark_theme', 'bilibili_theme', 'bilibili_dark_theme', 'metro_theme', 'metro_dark_theme', 'basic_theme', 'basic_dark_theme', 'get_default_theme', '_set_default_theme', 'set_default_theme', 'tkadw.windows.widgets.adw', 'Adw', 'Adwite', 'tkadw.windows.widgets', 'AdwLabel', 'AdwTLabel', 'tkadw.windows.canvas.button', 'AdwDrawRoundButton3', 'AdwTButton', 'tkadw.windows.canvas.entry', 'AdwDrawRoundEntry3', 'AdwTEntry', 'tkadw.windows.canvas.textbox', 'AdwDrawRoundText3', 'AdwTText', 'tkadw.windows.canvas.frame', 'AdwDrawRoundFrame3', 'AdwTFrame', 'tkadw.windows.canvas.separator', 'AdwDrawSeparator', 'AdwTSeparator', '__name__', 'darkdetect', 'isDark', 'root', 'button', 'pack', 'separator', 'entry', 'text', 'frame', 'mainloop')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020304ff0205020102fe0406020102010201020102030201020102
-      0102fc040802010201020102fc04f2041702010201020102fc0408020102
-      020201020102010202020102030201020102010202020102f904f4041802
+      0102fc040802010201020102fc04f20417020102010201020102fb040902
       0102020201020102010202020102030201020102010202020102f904f404
-      180201020202fc04ab065f04ff0205020102fe0406020102010201020102
-      0302010201020102fc040802010201020102fc04f2041702010201020102
-      fc0408020102020201020102010202020102030201020102010202020102
-      f904f4041802010202020102010201020202010203020102010201020202
-      0102f904f404180201020202fc04ab065f04ff0205020102fe0406020102
-      0102010201020302010201020102fc040802010201020102fc04f2041702
-      010201020102fc0408020102020201020102010202020102030201020102
-      010202020102f904f4041802020201020102010201020202010203020102
-      0102010202020102f904f404180201020202fc04ab065f04ff0205020102
-      fe04060201020102010201020302010201020102fc040802010201020102
-      fc04f2041702010201020102fc0408020102020201020102010202020102
+      18020102020201020102010202020102030201020102010202020102f904
+      f404180201020202fc04aa066004ff0205020102fe040602010201020102
+      01020302010201020102fc040802010201020102fc04f204170201020102
+      01020102fb04090201020202010201020102020201020302010201020102
+      02020102f904f40418020102020201020102010202020102030201020102
+      010202020102f904f404180201020202fc04aa066004ff0205020102fe04
+      060201020102010201020302010201020102fc040802010201020102fc04
+      f20417020102010201020102fb0409020102020201020102010202020102
       030201020102010202020102f904f4041802020201020102010201020202
-      0102030201020102010202020102f904f404180201020202fc04ab065f04
+      0102030201020102010202020102f904f404180201020202fc04aa066004
       ff0205020102fe04060201020102010201020302010201020102fc040802
-      010201020102fc04f2041702010201020102fc0408020102020201020102
-      010202020102030201020102010202020102f904f4041802010202020102
-      0102010202020102030201020102010202020102f904f404180201020202
-      fc04ab065f04ff0205020102fe0406020102010201020102030201020102
-      0102fc040802010201020102fc04f2041702010201020102fc0408020102
+      010201020102fc04f20417020102010201020102fb040902010202020102
+      0102010202020102030201020102010202020102f904f404180202020102
+      01020102010202020102030201020102010202020102f904f40418020102
+      0202fc04aa066004ff0205020102fe040602010201020102010203020102
+      01020102fc040802010201020102fc04f20417020102010201020102fb04
+      09020102020201020102010202020102030201020102010202020102f904
+      f40418020102020201020102010202020102030201020102010202020102
+      f904f404180201020202fc04aa066004ff0205020102fe04060201020102
+      010201020302010201020102fc040802010201020102fc04f20417020102
+      010201020102fb0409020102020201020102010202020102030201020102
+      010202020102f904f4041802010202020102010201020202010203020102
+      0102010202020102f904f404180201020202fc04aa066004ff0205020102
+      fe04060201020102010201020302010201020102fc040802010201020102
+      fc04f20417020102010201020102fb040902010202020102010201020202
+      0102030201020102010202020102f904f404180201020202010201020102
+      02020102030201020102010202020102f904f404180201020202fc04aa06
+      6004ff0205020102fe04060201020102010201020302010201020102fc04
+      0802010201020102fc04f20417020102010201020102fb04090201020202
+      01020102010202020102030201020102010202020102f904f40418020102
       020201020102010202020102030201020102010202020102f904f4041802
-      0102020201020102010202020102030201020102010202020102f904f404
-      180201020202fc04ab065f04ff0205020102fe0406020102010201020102
-      0302010201020102fc040802010201020102fc04f2041702010201020102
-      fc0408020102020201020102010202020102030201020102010202020102
+      01020202fc04aa066004ff0205020102fe04060201020102010201020302
+      010201020102fc040802010201020102fc04f20417020102010201020102
+      fb0409020102020201020102010202020102030201020102010202020102
       f904f4041802010202020102010201020202010203020102010201020202
-      0102f904f404180201020202fc04ab065f04ff0205020102fe0406020102
+      0102f904f404180201020202fc04aa066004ff0205020102fe0406020102
       0102010201020302010201020102fc040802010201020102fc04f2041702
-      010201020102fc0408020102020201020102010202020102030201020102
-      010202020102f904f4041802010202020102010201020202010203020102
-      0102010202020102f904f404180201020202fc04ab065e06090606084216
-      030c031c0e0c031c050c031c050c031c050c031c050c031c050c031c050c
-      010c0214012a0206031a013001140130011801300118013001140130012c
-      ed
+      0102010201020102fb040902010202020102010201020202010203020102
+      0102010202020102f904f404180201020202010201020102020201020302
+      01020102010202020102f904f404180201020202fc04aa065f0609060608
+      5116030c031c0e0c031c050c031c050c031c050c031c050c031c050c031c
+      050c010c0214012c0218013001140130011801300118013001140130012c
+      f0
```

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__init__.py` & `tkadw-0.3.3/tkadw/windows/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/__init__.cpython-310.pyc` & `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/__init__.cpython-311.pyc` & `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/button.cpython-310.pyc` & `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/button.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/button.cpython-311.pyc` & `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/button.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xdee2b064 (Fri Jul 14 05:53:34 2023 UTC)
-files sz: 18129
+moddate:  0x5491b264 (Sat Jul 15 12:30:12 2023 UTC)
+files sz: 18105
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
@@ -3067,142 +3067,128 @@
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000006401a6
                   010000ab01000000000000000001007c00a0010000000000000000000000
-                  0000000000000000007c006a02000000000000000064027a0a00007c006a
-                  02000000000000000064027a0a00007c00a0030000000000000000000000
-                  000000000000000000a6000000ab0000000000000000007c006a02000000
-                  000000000064037a0500007a0a000064027a0000007c00a0040000000000
-                  000000000000000000000000000000a6000000ab0000000000000000007c
-                  006a02000000000000000064037a0500007a0a000064027a0000007c006a
-                  0500000000000000007c006a0200000000000000007c006a060000000000
-                  0000007c006a070000000000000000ac04a6080000ab0800000000000000
-                  00010064057c005f0800000000000000007c00a009000000000000000000
-                  00000000000000000000007c00a003000000000000000000000000000000
-                  0000000000a6000000ab00000000000000000064037a0b00007c00a00400
-                  00000000000000000000000000000000000000a6000000ab000000000000
-                  00000064037a0b00007c006a0a00000000000000007c006a0b0000000000
-                  0000007c006a0c0000000000000000ac06a6050000ab0500000000000000
-                  007c005f0d000000000000000064005300
+                  0000000000000000007c006a0200000000000000007c006a020000000000
+                  0000007c00a0030000000000000000000000000000000000000000a60000
+                  00ab0000000000000000007c006a0200000000000000007a0a00007c00a0
+                  040000000000000000000000000000000000000000a6000000ab00000000
+                  00000000007c006a0200000000000000007a0a00007c006a050000000000
+                  0000007c006a0200000000000000007c006a0600000000000000007c006a
+                  070000000000000000ac02a6080000ab080000000000000000010064037c
+                  005f0800000000000000007c00a009000000000000000000000000000000
+                  00000000007c00a0030000000000000000000000000000000000000000a6
+                  000000ab00000000000000000064047a0b00007c00a00400000000000000
+                  00000000000000000000000000a6000000ab00000000000000000064047a
+                  0b00007c006a0a00000000000000007c006a0b00000000000000007c006a
+                  0c0000000000000000ac05a6050000ab0500000000000000007c005f0d00
+                  0000000000000064005300
                442           0 RESUME                   0
                
                443           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
                446          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect4)
                
                447          68 LOAD_FAST                0 (self)
                             70 LOAD_ATTR                2 (_button_border_width)
-                            80 LOAD_CONST               2 (1)
-                            82 BINARY_OP               10 (-)
-                            86 LOAD_FAST                0 (self)
-                            88 LOAD_ATTR                2 (_button_border_width)
-                            98 LOAD_CONST               2 (1)
-                           100 BINARY_OP               10 (-)
+                            80 LOAD_FAST                0 (self)
+                            82 LOAD_ATTR                2 (_button_border_width)
                
-               448         104 LOAD_FAST                0 (self)
-                           106 LOAD_METHOD              3 (winfo_width)
-                           128 PRECALL                  0
-                           132 CALL                     0
-                           142 LOAD_FAST                0 (self)
-                           144 LOAD_ATTR                2 (_button_border_width)
-                           154 LOAD_CONST               3 (2)
-                           156 BINARY_OP                5 (*)
-                           160 BINARY_OP               10 (-)
-                           164 LOAD_CONST               2 (1)
-                           166 BINARY_OP                0 (+)
-               
-               449         170 LOAD_FAST                0 (self)
-                           172 LOAD_METHOD              4 (winfo_height)
-                           194 PRECALL                  0
-                           198 CALL                     0
-                           208 LOAD_FAST                0 (self)
-                           210 LOAD_ATTR                2 (_button_border_width)
-                           220 LOAD_CONST               3 (2)
-                           222 BINARY_OP                5 (*)
-                           226 BINARY_OP               10 (-)
-                           230 LOAD_CONST               2 (1)
-                           232 BINARY_OP                0 (+)
+               448          92 LOAD_FAST                0 (self)
+                            94 LOAD_METHOD              3 (winfo_width)
+                           116 PRECALL                  0
+                           120 CALL                     0
+                           130 LOAD_FAST                0 (self)
+                           132 LOAD_ATTR                2 (_button_border_width)
+                           142 BINARY_OP               10 (-)
+               
+               449         146 LOAD_FAST                0 (self)
+                           148 LOAD_METHOD              4 (winfo_height)
+                           170 PRECALL                  0
+                           174 CALL                     0
+                           184 LOAD_FAST                0 (self)
+                           186 LOAD_ATTR                2 (_button_border_width)
+                           196 BINARY_OP               10 (-)
                
-               450         236 LOAD_FAST                0 (self)
-                           238 LOAD_ATTR                5 (button_radius)
-               
-               451         248 LOAD_FAST                0 (self)
-                           250 LOAD_ATTR                2 (_button_border_width)
+               450         200 LOAD_FAST                0 (self)
+                           202 LOAD_ATTR                5 (button_radius)
                
-               452         260 LOAD_FAST                0 (self)
-                           262 LOAD_ATTR                6 (_button_border)
-                           272 LOAD_FAST                0 (self)
-                           274 LOAD_ATTR                7 (_button_back)
+               451         212 LOAD_FAST                0 (self)
+                           214 LOAD_ATTR                2 (_button_border_width)
                
-               446         284 KW_NAMES                 4
-                           286 PRECALL                  8
-                           290 CALL                     8
-                           300 POP_TOP
+               452         224 LOAD_FAST                0 (self)
+                           226 LOAD_ATTR                6 (_button_border)
+                           236 LOAD_FAST                0 (self)
+                           238 LOAD_ATTR                7 (_button_back)
                
-               455         302 LOAD_CONST               5 ('button_frame')
-                           304 LOAD_FAST                0 (self)
-                           306 STORE_ATTR               8 (button_frame)
-               
-               458         316 LOAD_FAST                0 (self)
-                           318 LOAD_METHOD              9 (create_text)
-               
-               459         340 LOAD_FAST                0 (self)
-                           342 LOAD_METHOD              3 (winfo_width)
-                           364 PRECALL                  0
-                           368 CALL                     0
-                           378 LOAD_CONST               3 (2)
-                           380 BINARY_OP               11 (/)
-                           384 LOAD_FAST                0 (self)
-                           386 LOAD_METHOD              4 (winfo_height)
-                           408 PRECALL                  0
-                           412 CALL                     0
-                           422 LOAD_CONST               3 (2)
-                           424 BINARY_OP               11 (/)
-               
-               460         428 LOAD_FAST                0 (self)
-                           430 LOAD_ATTR               10 (text)
-                           440 LOAD_FAST                0 (self)
-                           442 LOAD_ATTR               11 (_button_text_back)
-               
-               461         452 LOAD_FAST                0 (self)
-                           454 LOAD_ATTR               12 (button_text_font)
-               
-               458         464 KW_NAMES                 6
-                           466 PRECALL                  5
-                           470 CALL                     5
-                           480 LOAD_FAST                0 (self)
-                           482 STORE_ATTR              13 (button_text)
-                           492 LOAD_CONST               0 (None)
-                           494 RETURN_VALUE
+               446         248 KW_NAMES                 2
+                           250 PRECALL                  8
+                           254 CALL                     8
+                           264 POP_TOP
+               
+               455         266 LOAD_CONST               3 ('button_frame')
+                           268 LOAD_FAST                0 (self)
+                           270 STORE_ATTR               8 (button_frame)
+               
+               458         280 LOAD_FAST                0 (self)
+                           282 LOAD_METHOD              9 (create_text)
+               
+               459         304 LOAD_FAST                0 (self)
+                           306 LOAD_METHOD              3 (winfo_width)
+                           328 PRECALL                  0
+                           332 CALL                     0
+                           342 LOAD_CONST               4 (2)
+                           344 BINARY_OP               11 (/)
+                           348 LOAD_FAST                0 (self)
+                           350 LOAD_METHOD              4 (winfo_height)
+                           372 PRECALL                  0
+                           376 CALL                     0
+                           386 LOAD_CONST               4 (2)
+                           388 BINARY_OP               11 (/)
+               
+               460         392 LOAD_FAST                0 (self)
+                           394 LOAD_ATTR               10 (text)
+                           404 LOAD_FAST                0 (self)
+                           406 LOAD_ATTR               11 (_button_text_back)
+               
+               461         416 LOAD_FAST                0 (self)
+                           418 LOAD_ATTR               12 (button_text_font)
+               
+               458         428 KW_NAMES                 5
+                           430 PRECALL                  5
+                           434 CALL                     5
+                           444 LOAD_FAST                0 (self)
+                           446 STORE_ATTR              13 (button_text)
+                           456 LOAD_CONST               0 (None)
+                           458 RETURN_VALUE
                consts
                   None
                   'all'
-                  1
-                  2
                   ('width', 'outline', 'fill')
                   'button_frame'
+                  2
                   ('text', 'fill', 'font')
                names      ('delete', 'create_round_rect4', '_button_border_width', 'winfo_width', 'winfo_height', 'button_radius', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       '_draw'
                firstlineno 442
                lnotab
-                  0x02012a0318012401420142010c010c0118fa12090e031801580118010c
+                  0x02012a0318011801360136010c010c0118fa12090e031801580118010c
                   fd
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
```

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/drawengine.cpython-310.pyc` & `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/drawengine.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/drawengine.cpython-311.pyc` & `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/drawengine.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x08e4a364 (Tue Jul  4 09:19:04 2023 UTC)
-files sz: 39862
+moddate:  0xc731b264 (Sat Jul 15 05:42:31 2023 UTC)
+files sz: 41631
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 12
    flags     : 0
    code
       0x9700640064016c006d015a010100640284005a0264035a0364045a0464
@@ -57,39 +57,39 @@
                  54 MAKE_FUNCTION            0
                  56 LOAD_CONST              11 ('AdwDrawEngine')
                  58 LOAD_NAME                1 (Canvas)
                  60 PRECALL                  3
                  64 CALL                     3
                  74 STORE_NAME              10 (AdwDrawEngine)
    
-   1014          76 LOAD_NAME               11 (__name__)
+   1083          76 LOAD_NAME               11 (__name__)
                  78 LOAD_CONST              12 ('__main__')
                  80 COMPARE_OP               2 (==)
                  86 POP_JUMP_FORWARD_IF_FALSE   102 (to 292)
    
-   1015          88 LOAD_CONST               0 (0)
+   1084          88 LOAD_CONST               0 (0)
                  90 LOAD_CONST              13 (('Tk',))
                  92 IMPORT_NAME              0 (tkinter)
                  94 IMPORT_FROM             12 (Tk)
                  96 STORE_NAME              12 (Tk)
                  98 POP_TOP
    
-   1017         100 PUSH_NULL
+   1086         100 PUSH_NULL
                 102 LOAD_NAME               12 (Tk)
                 104 PRECALL                  0
                 108 CALL                     0
                 118 STORE_NAME              13 (root)
    
-   1019         120 PUSH_NULL
+   1088         120 PUSH_NULL
                 122 LOAD_NAME               10 (AdwDrawEngine)
                 124 PRECALL                  0
                 128 CALL                     0
                 138 STORE_NAME              14 (canvas)
    
-   1025         140 LOAD_NAME               14 (canvas)
+   1094         140 LOAD_NAME               14 (canvas)
                 142 LOAD_METHOD             15 (gradient_draw)
                 164 LOAD_CONST              14 (123)
                 166 LOAD_CONST              15 (5)
                 168 LOAD_CONST              15 (5)
                 170 LOAD_CONST              16 (100)
                 172 LOAD_CONST              16 (100)
                 174 LOAD_NAME                5 (ARC)
@@ -98,32 +98,32 @@
                 180 LOAD_CONST              19 (90)
                 182 LOAD_CONST              20 (150)
                 184 KW_NAMES                21
                 186 PRECALL                 10
                 190 CALL                    10
                 200 POP_TOP
    
-   1027         202 LOAD_NAME               14 (canvas)
+   1096         202 LOAD_NAME               14 (canvas)
                 204 LOAD_METHOD             16 (pack)
                 226 LOAD_CONST              22 ('both')
                 228 LOAD_CONST              23 ('yes')
                 230 KW_NAMES                24
                 232 PRECALL                  2
                 236 CALL                     2
                 246 POP_TOP
    
-   1029         248 LOAD_NAME               13 (root)
+   1098         248 LOAD_NAME               13 (root)
                 250 LOAD_METHOD             17 (mainloop)
                 272 PRECALL                  0
                 276 CALL                     0
                 286 POP_TOP
                 288 LOAD_CONST              25 (None)
                 290 RETURN_VALUE
    
-   1014     >>  292 LOAD_CONST              25 (None)
+   1083     >>  292 LOAD_CONST              25 (None)
                 294 RETURN_VALUE
    consts
       0
       ('Canvas',)
       code
          argcount  : 3
          nlocals   : 7
@@ -235,164 +235,164 @@
                        18 MAKE_FUNCTION            8 (closure)
                        20 STORE_NAME               3 (__init__)
          
           245          22 LOAD_CONST               2 (<code object win32_high_dpi, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 245>)
                        24 MAKE_FUNCTION            0
                        26 STORE_NAME               4 (win32_high_dpi)
          
-          249          28 LOAD_CONST               3 (<code object rgb_to_num, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 249>)
+          252          28 LOAD_CONST               3 (<code object rgb_to_num, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 252>)
                        30 MAKE_FUNCTION            0
                        32 STORE_NAME               5 (rgb_to_num)
          
-          252          34 LOAD_CONST               4 ('hexs')
+          255          34 LOAD_CONST               4 ('hexs')
                        36 LOAD_NAME                6 (tuple)
                        38 BUILD_TUPLE              2
-                       40 LOAD_CONST               5 (<code object num_to_rgb, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 252>)
+                       40 LOAD_CONST               5 (<code object num_to_rgb, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 255>)
                        42 MAKE_FUNCTION            4 (annotations)
                        44 STORE_NAME               7 (num_to_rgb)
          
-          258          46 LOAD_CONST              43 ((26,))
-                       48 LOAD_CONST               7 (<code object get_color_change, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 258>)
+          261          46 LOAD_CONST              43 ((26,))
+                       48 LOAD_CONST               7 (<code object get_color_change, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 261>)
                        50 MAKE_FUNCTION            1 (defaults)
                        52 STORE_NAME               8 (get_color_change)
          
-          269          54 LOAD_CONST               8 (<code object gradient_init, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 269>)
+          272          54 LOAD_CONST               8 (<code object gradient_init, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 272>)
                        56 MAKE_FUNCTION            0
                        58 STORE_NAME               9 (gradient_init)
          
-          611          60 LOAD_CONST               9 (<code object gradient_demo, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 611>)
+          617          60 LOAD_CONST               9 (<code object gradient_demo, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 617>)
                        62 MAKE_FUNCTION            0
                        64 STORE_NAME              10 (gradient_demo)
          
-          615          66 LOAD_CONST              10 ('tags')
+          624          66 LOAD_CONST              10 ('tags')
                        68 LOAD_NAME               11 (str)
                        70 LOAD_CONST              11 ('x')
                        72 LOAD_NAME               12 (int)
                        74 LOAD_CONST              12 ('y')
                        76 LOAD_NAME               12 (int)
                        78 LOAD_CONST              13 ('width')
                        80 LOAD_NAME               12 (int)
                        82 LOAD_CONST              14 ('height')
                        84 LOAD_NAME               12 (int)
                        86 BUILD_TUPLE             10
-                       88 LOAD_CONST              15 (<code object gradient_resize, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 615>)
+                       88 LOAD_CONST              15 (<code object gradient_resize, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 624>)
                        90 MAKE_FUNCTION            4 (annotations)
                        92 STORE_NAME              13 (gradient_resize)
          
-          619          94 LOAD_CONST              10 ('tags')
+          631          94 LOAD_CONST              10 ('tags')
                        96 LOAD_NAME               11 (str)
                        98 LOAD_CONST              11 ('x')
                       100 LOAD_NAME               12 (int)
                       102 LOAD_CONST              12 ('y')
                       104 LOAD_NAME               12 (int)
                       106 BUILD_TUPLE              6
-                      108 LOAD_CONST              16 (<code object gradient_recolor, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 619>)
+                      108 LOAD_CONST              16 (<code object gradient_recolor, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 631>)
                       110 MAKE_FUNCTION            4 (annotations)
                       112 STORE_NAME              14 (gradient_recolor)
          
-          623         114 LOAD_CONST              10 ('tags')
+          638         114 LOAD_CONST              10 ('tags')
                       116 LOAD_NAME               11 (str)
                       118 LOAD_CONST              11 ('x')
                       120 LOAD_NAME               12 (int)
                       122 LOAD_CONST              12 ('y')
                       124 LOAD_NAME               12 (int)
                       126 LOAD_CONST              13 ('width')
                       128 LOAD_NAME               12 (int)
                       130 LOAD_CONST              14 ('height')
                       132 LOAD_NAME               12 (int)
                       134 BUILD_TUPLE             10
-                      136 LOAD_CONST              17 (<code object gradient_draw, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 623>)
+                      136 LOAD_CONST              17 (<code object gradient_draw, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 638>)
                       138 MAKE_FUNCTION            4 (annotations)
                       140 STORE_NAME              15 (gradient_draw)
          
-          630         142 LOAD_CONST              18 (<code object gradient_redraw, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 630>)
+          648         142 LOAD_CONST              18 (<code object gradient_redraw, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 648>)
                       144 MAKE_FUNCTION            0
                       146 STORE_NAME              16 (gradient_redraw)
          
-          633         148 LOAD_CONST              19 (<code object create_gradient_v_rectangle, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 633>)
+          654         148 LOAD_CONST              19 (<code object create_gradient_v_rectangle, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 654>)
                       150 MAKE_FUNCTION            0
                       152 STORE_NAME              17 (create_gradient_v_rectangle)
          
-          637         154 LOAD_CONST              20 (<code object create_gradient_h_rectangle, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 637>)
+          670         154 LOAD_CONST              20 (<code object create_gradient_h_rectangle, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 670>)
                       156 MAKE_FUNCTION            0
                       158 STORE_NAME              18 (create_gradient_h_rectangle)
          
-          641         160 LOAD_CONST              21 (<code object create_gradient_circular, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 641>)
+          686         160 LOAD_CONST              21 (<code object create_gradient_circular, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 686>)
                       162 MAKE_FUNCTION            0
                       164 STORE_NAME              19 (create_gradient_circular)
          
-          645         166 LOAD_CONST              44 (('x',))
-                      168 LOAD_CONST              22 (<code object draw_gradient, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 645>)
+          702         166 LOAD_CONST              44 (('x',))
+                      168 LOAD_CONST              22 (<code object draw_gradient, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 702>)
                       170 MAKE_FUNCTION            1 (defaults)
                       172 STORE_NAME              20 (draw_gradient)
          
-          712         174 LOAD_CONST              45 ((5, 2, 'white', 'black'))
+          769         174 LOAD_CONST              45 ((5, 2, 'white', 'black'))
                       176 LOAD_CONST              27 ('radius')
                       178 LOAD_NAME               21 (float)
                       180 BUILD_TUPLE              2
-                      182 LOAD_CONST              28 (<code object create_round_rectangle, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 712>)
+                      182 LOAD_CONST              28 (<code object create_round_rectangle, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 769>)
                       184 MAKE_FUNCTION            5 (defaults, annotations)
                       186 STORE_NAME              22 (create_round_rectangle)
          
-          746         188 LOAD_NAME               22 (create_round_rectangle)
+          806         188 LOAD_NAME               22 (create_round_rectangle)
                       190 STORE_NAME              23 (create_round_rect)
          
-          748         192 LOAD_CONST              29 (<code object create_round_rectangle2, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 748>)
+          808         192 LOAD_CONST              29 (<code object create_round_rectangle2, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 808>)
                       194 MAKE_FUNCTION            0
                       196 STORE_NAME              24 (create_round_rectangle2)
          
-          816         198 LOAD_NAME               24 (create_round_rectangle2)
+          879         198 LOAD_NAME               24 (create_round_rectangle2)
                       200 STORE_NAME              25 (create_round_rect2)
          
-          818         202 LOAD_CONST              46 (('black', 'black'))
+          881         202 LOAD_CONST              46 (('black', 'black'))
                       204 LOAD_CONST              30 ('fill')
                       206 LOAD_NAME               11 (str)
                       208 LOAD_CONST              31 ('outline')
                       210 LOAD_NAME               11 (str)
                       212 BUILD_TUPLE              4
-                      214 LOAD_CONST              32 (<code object create_round_rectangle3, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 818>)
+                      214 LOAD_CONST              32 (<code object create_round_rectangle3, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 881>)
                       216 MAKE_FUNCTION            5 (defaults, annotations)
                       218 STORE_NAME              26 (create_round_rectangle3)
          
-          836         220 LOAD_NAME               26 (create_round_rectangle3)
+          902         220 LOAD_NAME               26 (create_round_rectangle3)
                       222 STORE_NAME              27 (create_round_rect3)
          
-          838         224 LOAD_CONST              33 (<code object create_round_rectangle4, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 838>)
+          904         224 LOAD_CONST              33 (<code object create_round_rectangle4, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 904>)
                       226 MAKE_FUNCTION            0
                       228 STORE_NAME              28 (create_round_rectangle4)
          
-          864         230 LOAD_NAME               28 (create_round_rectangle4)
+          933         230 LOAD_NAME               28 (create_round_rectangle4)
                       232 STORE_NAME              29 (create_round_rect4)
          
-          866         234 LOAD_CONST              46 (('black', 'black'))
-                      236 LOAD_CONST              34 (<code object polygon_round, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 866>)
+          935         234 LOAD_CONST              46 (('black', 'black'))
+                      236 LOAD_CONST              34 (<code object polygon_round, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 935>)
                       238 MAKE_FUNCTION            1 (defaults)
                       240 STORE_NAME              30 (polygon_round)
          
-          872         242 LOAD_NAME               30 (polygon_round)
+          941         242 LOAD_NAME               30 (polygon_round)
                       244 STORE_NAME              31 (poly_round)
          
-          874         246 LOAD_CONST              35 (<code object demo_polygon_round, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 874>)
+          943         246 LOAD_CONST              35 (<code object demo_polygon_round, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 943>)
                       248 MAKE_FUNCTION            0
                       250 STORE_NAME              32 (demo_polygon_round)
          
-          982         252 LOAD_CONST              36 ('content')
+         1051         252 LOAD_CONST              36 ('content')
                       254 LOAD_NAME               11 (str)
                       256 BUILD_TUPLE              2
-                      258 LOAD_CONST              37 (<code object create_svg_image, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 982>)
+                      258 LOAD_CONST              37 (<code object create_svg_image, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 1051>)
                       260 MAKE_FUNCTION            4 (annotations)
                       262 STORE_NAME              33 (create_svg_image)
          
-          997         264 LOAD_CONST              47 ((10, 10, 18))
-                      266 LOAD_CONST              40 (<code object draw_copy_icon, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 997>)
+         1066         264 LOAD_CONST              47 ((10, 10, 18))
+                      266 LOAD_CONST              40 (<code object draw_copy_icon, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 1066>)
                       268 MAKE_FUNCTION            1 (defaults)
                       270 STORE_NAME              34 (draw_copy_icon)
          
-         1006         272 LOAD_CONST              48 (('black', 16))
-                      274 LOAD_CONST              42 (<code object create_round_rectangle5, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 1006>)
+         1075         272 LOAD_CONST              48 (('black', 16))
+                      274 LOAD_CONST              42 (<code object create_round_rectangle5, file "D:\tkadw\tkadw\windows\canvas\drawengine.py", line 1075>)
                       276 MAKE_FUNCTION            1 (defaults)
                       278 STORE_NAME              35 (create_round_rectangle5)
                       280 LOAD_CLOSURE             0 (__class__)
                       282 COPY                     1
                       284 STORE_NAME              36 (__classcell__)
                       286 RETURN_VALUE
          consts
@@ -436,60 +436,61 @@
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x9700640164026c006d017d0101007c016a020000000000000000a00300
                   000000000000000000000000000000000000006403a6010000ab01000000
-                  0000000000010064005300
+                  0000000000010064045300
                245           0 RESUME                   0
                
-               246           2 LOAD_CONST               1 (0)
+               249           2 LOAD_CONST               1 (0)
                              4 LOAD_CONST               2 (('windll',))
                              6 IMPORT_NAME              0 (ctypes)
                              8 IMPORT_FROM              1 (windll)
                             10 STORE_FAST               1 (windll)
                             12 POP_TOP
                
-               247          14 LOAD_FAST                1 (windll)
+               250          14 LOAD_FAST                1 (windll)
                             16 LOAD_ATTR                2 (shcore)
                             26 LOAD_METHOD              3 (SetProcessDpiAwareness)
                             48 LOAD_CONST               3 (2)
                             50 PRECALL                  1
                             54 CALL                     1
                             64 POP_TOP
-                            66 LOAD_CONST               0 (None)
+                            66 LOAD_CONST               4 (None)
                             68 RETURN_VALUE
                consts
-                  None
+                  '\n        windows平台高DPI启用\n        '
                   0
                   ('windll',)
                   2
+                  None
                names      ('ctypes', 'windll', 'shcore', 'SetProcessDpiAwareness')
                varnames   ('self', 'windll')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'win32_high_dpi'
                firstlineno 245
-               lnotab 0x02010c01
+               lnotab 0x02040c01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 7
                flags     : 3
                code
                   0x97007401000000000000000000007c0164016402850219000000000000
                   0000006403a6020000ab0200000000000000007401000000000000000000
                   007c01640264048502190000000000000000006403a6020000ab02000000
                   00000000007401000000000000000000007c016404640085021900000000
                   00000000006403a6020000ab02000000000000000066035300
-               249           0 RESUME                   0
+               252           0 RESUME                   0
                
-               250           2 LOAD_GLOBAL              1 (NULL + int)
+               253           2 LOAD_GLOBAL              1 (NULL + int)
                             14 LOAD_FAST                1 (rgb)
                             16 LOAD_CONST               1 (1)
                             18 LOAD_CONST               2 (3)
                             20 BUILD_SLICE              2
                             22 BINARY_SUBSCR
                             32 LOAD_CONST               3 (16)
                             34 PRECALL                  2
@@ -522,38 +523,38 @@
                   5
                names      ('int',)
                varnames   ('self', 'rgb')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'rgb_to_num'
-               firstlineno 249
+               firstlineno 252
                lnotab 0x0201
             'hexs'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 7
                flags     : 3
                code
                   0x970064017d027c0144005d297d037c0274010000000000000000000074
                   03000000000000000000007c03a6010000ab010000000000000000a60100
                   00ab010000000000000000640264008502190000000000000000007a0d00
                   007d028c2a7c025300
-               252           0 RESUME                   0
+               255           0 RESUME                   0
                
-               253           2 LOAD_CONST               1 ('#')
+               256           2 LOAD_CONST               1 ('#')
                              4 STORE_FAST               2 (co)
                
-               254           6 LOAD_FAST                1 (hexs)
+               257           6 LOAD_FAST                1 (hexs)
                              8 GET_ITER
                        >>   10 FOR_ITER                41 (to 94)
                             12 STORE_FAST               3 (i)
                
-               255          14 LOAD_FAST                2 (co)
+               258          14 LOAD_FAST                2 (co)
                             16 LOAD_GLOBAL              1 (NULL + str)
                             28 LOAD_GLOBAL              3 (NULL + hex)
                             40 LOAD_FAST                3 (i)
                             42 PRECALL                  1
                             46 CALL                     1
                             56 PRECALL                  1
                             60 CALL                     1
@@ -561,27 +562,27 @@
                             72 LOAD_CONST               0 (None)
                             74 BUILD_SLICE              2
                             76 BINARY_SUBSCR
                             86 BINARY_OP               13 (+=)
                             90 STORE_FAST               2 (co)
                             92 JUMP_BACKWARD           42 (to 10)
                
-               256     >>   94 LOAD_FAST                2 (co)
+               259     >>   94 LOAD_FAST                2 (co)
                             96 RETURN_VALUE
                consts
                   None
                   '#'
                   2
                names      ('str', 'hex')
                varnames   ('self', 'hexs', 'co', 'i')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'num_to_rgb'
-               firstlineno 252
+               firstlineno 255
                lnotab 0x0201040108015001
             26
             code
                argcount  : 4
                nlocals   : 17
                stacksize : 8
                flags     : 3
@@ -596,68 +597,68 @@
                   000000a6010000ab0100000000000000007405000000000000000000007c
                   067c0c7c0f7a0500007a000000a6010000ab010000000000000000740500
                   0000000000000000007c077c0d7c0f7a0500007a000000a6010000ab0100
                   0000000000000066037d107c04a003000000000000000000000000000000
                   00000000007c00a00400000000000000000000000000000000000000007c
                   10a6010000ab010000000000000000a6010000ab01000000000000000001
                   008c717c045300
-               258           0 RESUME                   0
+               261           0 RESUME                   0
                
-               259           2 BUILD_LIST               0
+               262           2 BUILD_LIST               0
                              4 STORE_FAST               4 (colors)
                
-               260           6 LOAD_FAST                0 (self)
+               263           6 LOAD_FAST                0 (self)
                              8 LOAD_METHOD              0 (rgb_to_num)
                             30 LOAD_FAST                1 (color1)
                             32 PRECALL                  1
                             36 CALL                     1
                             46 UNPACK_SEQUENCE          3
                             50 STORE_FAST               5 (a1)
                             52 STORE_FAST               6 (a2)
                             54 STORE_FAST               7 (a3)
                
-               261          56 LOAD_FAST                0 (self)
+               264          56 LOAD_FAST                0 (self)
                             58 LOAD_METHOD              0 (rgb_to_num)
                             80 LOAD_FAST                2 (color2)
                             82 PRECALL                  1
                             86 CALL                     1
                             96 UNPACK_SEQUENCE          3
                            100 STORE_FAST               8 (b1)
                            102 STORE_FAST               9 (b2)
                            104 STORE_FAST              10 (b3)
                
-               262         106 LOAD_FAST                8 (b1)
+               265         106 LOAD_FAST                8 (b1)
                            108 LOAD_FAST                5 (a1)
                            110 BINARY_OP               10 (-)
                            114 LOAD_FAST                9 (b2)
                            116 LOAD_FAST                6 (a2)
                            118 BINARY_OP               10 (-)
                            122 LOAD_FAST               10 (b3)
                            124 LOAD_FAST                7 (a3)
                            126 BINARY_OP               10 (-)
                            130 STORE_FAST              13 (b)
                            132 STORE_FAST              12 (g)
                            134 STORE_FAST              11 (r)
                
-               263         136 LOAD_GLOBAL              3 (NULL + range)
+               266         136 LOAD_GLOBAL              3 (NULL + range)
                            148 LOAD_FAST                3 (num)
                            150 PRECALL                  1
                            154 CALL                     1
                            164 GET_ITER
                        >>  166 FOR_ITER               112 (to 392)
                            168 STORE_FAST              14 (i)
                
-               264         170 LOAD_FAST               14 (i)
+               267         170 LOAD_FAST               14 (i)
                            172 LOAD_FAST                3 (num)
                            174 BINARY_OP               11 (/)
                            178 LOAD_CONST               1 (1)
                            180 BINARY_OP               10 (-)
                            184 STORE_FAST              15 (t)
                
-               265         186 LOAD_GLOBAL              5 (NULL + int)
+               268         186 LOAD_GLOBAL              5 (NULL + int)
                            198 LOAD_FAST                5 (a1)
                            200 LOAD_FAST               11 (r)
                            202 LOAD_FAST               15 (t)
                            204 BINARY_OP                5 (*)
                            208 BINARY_OP                0 (+)
                            212 PRECALL                  1
                            216 CALL                     1
@@ -676,109 +677,111 @@
                            284 BINARY_OP                5 (*)
                            288 BINARY_OP                0 (+)
                            292 PRECALL                  1
                            296 CALL                     1
                            306 BUILD_TUPLE              3
                            308 STORE_FAST              16 (rgb)
                
-               266         310 LOAD_FAST                4 (colors)
+               269         310 LOAD_FAST                4 (colors)
                            312 LOAD_METHOD              3 (append)
                            334 LOAD_FAST                0 (self)
                            336 LOAD_METHOD              4 (num_to_rgb)
                            358 LOAD_FAST               16 (rgb)
                            360 PRECALL                  1
                            364 CALL                     1
                            374 PRECALL                  1
                            378 CALL                     1
                            388 POP_TOP
                            390 JUMP_BACKWARD          113 (to 166)
                
-               267     >>  392 LOAD_FAST                4 (colors)
+               270     >>  392 LOAD_FAST                4 (colors)
                            394 RETURN_VALUE
                consts
                   None
                   1
                names      ('rgb_to_num', 'range', 'int', 'append', 'num_to_rgb')
                varnames   ('self', 'color1', 'color2', 'num', 'colors', 'a1', 'a2', 'a3', 'b1', 'b2', 'b3', 'r', 'g', 'b', 'i', 't', 'rgb')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'get_color_change'
-               firstlineno 258
+               firstlineno 261
                lnotab 0x02010401320132011e01220110017c015201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
-                  000000000000006401a6010000ab010000000000000000010064005300
-               269           0 RESUME                   0
+                  000000000000006401a6010000ab010000000000000000010064025300
+               272           0 RESUME                   0
                
-               270           2 LOAD_FAST                0 (self)
+               276           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (tk)
                             14 LOAD_METHOD              1 (eval)
                             36 LOAD_CONST               1 ('\n        # Create color gradients of various shapes and sizes on a canvas.\n#   Usage:\n#       gradient draw    <canvas> <tags> <x> <y> <width> <height> <vertical|horizontal|circular|central|arc> <color1> <color2>  ?-animate? ?option? ...\n#       gradient redraw  <canvas> <tags> <x> <y> <width> <height> <vertical|horizontal|circular|central|arc> <color1> <color2>  ?-animate? ?option? ...\n#       gradient resize  <canvas> <tags> <x> <y> <width> <height>\n#       gradient recolor <canvas> <tags> <color1> <color2>\n\nnamespace eval gradient {\n    namespace ensemble create -subcommands {\n        draw\n        redraw\n        recolor\n        resize\n        demo\n    }\n\n    # Create a gradient on a canvas. The gradient will be placed at the top of the display list.\n    proc draw {canvas tags x y width height orient color1 color2 args} {\n        # Ensure valid colors are provided while also converting to lists of 16-bit RGB values.\n        if { [catch {winfo rgb . $color1} rgb1] } {\n            error "invalid color: $color1"\n        }\n        if { [catch {winfo rgb . $color2} rgb2] } {\n            error "invalid color: $color2"\n        }\n        \n        # Delete the gradient if it already exists.\n        $canvas delete [join $tags &&]\n        \n        # Create a hidden canvas item to store meta data about this gradient.\n        set meta_data [list x $x  y $y  width $width  height $height  orient $orient  color1 $color1  color2 $color2  args $args]\n        $canvas create line $x $y $x $y  -state hidden  -tags [list {*}$tags meta [list gradient: {*}$meta_data]]\n        \n        # Intercept the -animate option.\n        if { "-animate" in $args} {\n            set index [lsearch $args "-animate"]\n            set args  [lreplace $args $index $index]\n            set animate 1\n        } else {\n            set animate 0\n        }\n        \n        # Draw the gradient.\n        if { $orient eq "central" } {\n            # Create the canvas rectangle items.\n            foreach {x1 y1 x2 y2 color} [get_rects $x $y $width $height $rgb1 $rgb2] {\n                $canvas create rectangle $x1 $y1 $x2 $y2  -outline $color  -width 2  -tags $tags  {*}$args\n                if {$animate} {update}\n            }\n        } elseif { $orient eq "circular" } {\n            # Create the canvas oval items.\n            foreach {x1 y1 x2 y2 color} [get_rects $x $y $width $height $rgb1 $rgb2] {\n                $canvas create oval $x1 $y1 $x2 $y2  -outline $color  -width 2  -tags $tags  {*}$args\n                if {$animate} {update}\n            }\n        } elseif { $orient eq "arc" } {\n            # Create the canvas arc items.\n            foreach {x1 y1 x2 y2 color} [get_rects $x $y $width $height $rgb1 $rgb2] {\n                $canvas create arc $x1 $y1 $x2 $y2  -outline $color  -width 2  -tags $tags  -style arc  {*}$args\n                if {$animate} {update}\n            }\n        } elseif { $orient in [list "vertical" "horizontal"] } {        \n            # Create the canvas line items.\n            foreach {x1 y1 x2 y2 color} [get_lines $x $y $width $height $orient $rgb1 $rgb2] {\n                $canvas create line $x1 $y1 $x2 $y2  -fill $color  -tags $tags  -capstyle projecting  {*}$args\n                if {$animate} {update}\n            }\n        } else {\n            # Delete the meta data and throw an error.\n            $canvas delete [join $tags &&]\n            error "invalid orientation: $orient; must be: vertical, horizontal, circular, central, or arc"\n        }\n        \n        return\n    }\n    \n    # Same as draw, but if the gradient already exists then it will retain its position in the canvas\'s display list after being redrawn.\n    proc redraw {canvas tags x y width height orient color1 color2 args} {\n        # If the gradient already exists, remember its location in the display list.\n        set item_above [$canvas find above [join $tags &&]]\n        \n        # Draw the gradient.\n        draw $canvas $tags $x $y $width $height $orient $color1 $color2 {*}$args\n        \n        # Move the gradient to its previous location in the display list, if any.\n        if { $item_above ne "" } {\n            $canvas lower [join $tags &&] $item_above\n        }\n        \n        return\n    }\n    \n    # Shortcut procedure to change the colors of the gradient. Same as redraw but introspectively determines some meta data. \n    # This will use the gradient\'s x/y location when it was last drawn.\n    proc recolor {canvas tags color1 color2} {\n        # Retrieve the gradient\'s meta data.\n        set meta [get_meta_data $canvas $tags]\n        set meta [dict remove $meta color1 color2]\n        dict with meta {}\n        \n        # Redraw the gradient with the new colors.\n        redraw $canvas $tags $x $y $width $height $orient $color1 $color2 {*}$args\n        return     \n    }\n    \n    # Shortcut procedure to resize and reposition a gradient. Same as redraw but introspectively determines some meta data. \n    proc resize {canvas tags x y width height} {\n        # Retrieve the gradient\'s meta data.\n        set meta [get_meta_data $canvas $tags]\n        set meta [dict remove $meta x y width height]\n        dict with meta {}\n        \n        # Recreate the canvas lines with the new dimensions.\n        redraw $canvas $tags $x $y $width $height $orient $color1 $color2 {*}$args\n        return\n    }\n    \n    # Retrieve meta information on a gradient.\n    proc get_meta_data {canvas tags} {\n        if { [string is integer -strict $tags] } {\n            # This is supposedly a canvas item ID instead of a list of tags describing a gradient. Avoid introducing subtle logic errors.\n            error "cannot provide canvas item ID in lieu of gradient tags: $tags"\n        }\n        # This is a list of tags for a gradient. Find the hidden meta item for this gradient.\n        set all_tags [$canvas gettags "meta&&[join $tags &&]"]\n        set meta_data [lrange [lsearch -inline -index 0 $all_tags "gradient:"] 1 end]\n        if { [llength $meta_data] == 0 } {\n            error "cannot find meta data for gradient with tags: $tags"\n        }\n        return $meta_data\n    }\n    \n    # For a canvas item ID, return all tags that are not gradient meta tags.\n    proc get_non_meta_tags {canvas id} {\n        set tags [$canvas gettags $id]\n        set index [lsearch $tags "meta"]\n        set tags [lreplace $tags $index $index]\n        set index [lsearch -index 0 $tags "gradient:"]\n        set tags [lreplace $tags $index $index]\n        return $tags\n    }\n\n    # Calculate a list of center-to-outward colored rectangles suitable for [canvas create rectangle] or [canvas create oval].\n    proc get_rects {x y width height rgb1 rgb2} {\n        set rects [list]\n        set x1 [expr {int($x)+1}]\n        set y1 [expr {int($y)+1}]\n        set x2 [expr {$x1+$width-1}]\n        set y2 [expr {$y1+$height-1}]\n        \n        # Calculate each rectangle.\n        if { $width > $height } {\n            # Decrement X by one pixel in both directions. Decrement Y by a fraction in both directions.\n            # The Y axis will be more heavily concentrated.\n            set ratio  [expr { 1.0*$height/$width }]\n            set length [expr { $width/2 }]\n            while { $x2 > $x1 } {\n                lappend rects $x1 $y1 $x2 $y2 [get_color $rgb1 $rgb2 $length [expr { ($x2-$x1)/2 }]]\n                set x1 [expr { $x1+1 }]\n                set x2 [expr { $x2-1 }]\n                set y1 [expr { $y1+$ratio }]\n                set y2 [expr { $y2-$ratio }]\n            }\n        } else {\n            # Decrement Y by one pixel in both directions. Decrement X by a fraction in both directions.\n            # The X axis will be more heavily concentrated (unless width==height).\n            set ratio  [expr { 1.0*$width/$height }]\n            set length [expr { $height/2 }]\n            while { $y2 > $y1 } {\n                lappend rects $x1 $y1 $x2 $y2 [get_color $rgb1 $rgb2 $length [expr { ($y2-$y1)/2 }]]\n                set x1 [expr { $x1+$ratio }]\n                set x2 [expr { $x2-$ratio }]\n                set y1 [expr { $y1+1 }]\n                set y2 [expr { $y2-1 }]\n            }\n        }\n        return $rects\n    }\n\n    # Calculate a list of left-to-right or top-to-bottom colored lines suitable for [canvas create line].\n    proc get_lines {x1 y1 width height orient rgb1 rgb2} {\n        set lines [list]\n        set x1 [expr {int($x1)}]\n        set y1 [expr {int($y1)}]\n        set x2 [expr {$x1+$width}]\n        set y2 [expr {$y1+$height}]\n        if { $orient eq "vertical" } {\n            # Calculate the color for each horizontal line.\n            for {set y $y1} {$y < $y2} {incr y} {\n                lappend lines $x1 $y $x2 $y [get_color $rgb1 $rgb2 $height [expr {$y-$y1}]]\n            }\n        } elseif { $orient eq "horizontal" } {\n            # Calculate the color for each vertical column.\n            for {set x $x1} {$x < $x2} {incr x} {\n                lappend lines $x $y1 $x $y2 [get_color $rgb1 $rgb2 $width [expr {$x-$x1}]]\n            }\n        } else {\n            error "invalid orientation: $orient; must be: vertical or horizontal"\n        }\n        \n        return $lines\n    }\n\n    # Calculates the color at the specified index between rgb1 and rgb2 where rgb1 and rgb2 are the specified length apart.\n    proc get_color {rgb1 rgb2 length index} {\n        # Throw an error if the index is out of bounds.\n        if { $index < 0  ||  $index >= $length } {\n            error "index $index is out of bounds for length $length"\n        }\n        \n        lassign $rgb1 r1 g1 b1\n        lassign $rgb2 r2 g2 b2\n        \n        # Determine the ratio between each starting component color and ending component color.\n        set r_ratio [expr { 1.00*($r2-$r1+1)/$length }]\n        set g_ratio [expr { 1.00*($g2-$g1+1)/$length }]\n        set b_ratio [expr { 1.00*($b2-$b1+1)/$length }]\n\n        # Calculate the new component colors at the given index. \n        set r [expr { int($r_ratio*$index+$r1) }]\n        set g [expr { int($g_ratio*$index+$g1) }]\n        set b [expr { int($b_ratio*$index+$b1) }]\n\n        # A hacky workaround to make up for a lack of precision (or faulty math?).\n        # The final pixel of the gradient should exactly match the color of rgb2\n        if { $index == [expr {$length-1}] } {\n            lassign $rgb2 r g b\n        }\n\n        # Convert the integer RGB values to a hex color.\n        return [rgb_to_hex [list $r $g $b]]\n    }\n    \n    # Convert a list of 16-bit RGB values to an 8-bit hex color. Using 8-bit hex colors instead of 16-bit\n    # speeds up drawing of images two-fold (I haven\'t benchmarked this for canvases).\n    proc rgb_to_hex {rgb} {\n        lassign $rgb r g b\n        set r [format %02x [expr {$r/256}]]\n        set g [format %02x [expr {$g/256}]]\n        set b [format %02x [expr {$b/256}]]\n        return #$r$g$b\n    }\n    \n    # Converts 8-bit RGB values to 16-bit RGB values.\n    proc rgb_8_to_16_bit {rgb} {\n        lassign $rgb r g b\n        return [list [expr {$r*256}] [expr {$g*256}] [expr {$b*256}]]\n    }\n    \n    # Returns a random 8-bit hex color.\n    proc random_color {} {\n        return [rgb_to_hex "[expr {int(rand()*65536)}] [expr {int(rand()*65536)}] [expr {int(rand()*65536)}]"]\n    }\n\n    # Redraw all gradients with random colors\n    proc randomize_all_gradient_colors {canvas} {\n        foreach id [$canvas find withtag meta] {\n            set tags [get_non_meta_tags $canvas $id]\n            recolor $canvas $tags [random_color] [random_color]\n        }\n      return\n    }\n    \n    # Randomize colors for all canvas items.\n    proc randomize_all_canvas_item_colors {canvas} {\n        foreach id [$canvas find withtag all] {\n            if { [$canvas type $id] in {window} } {\n                continue\n            }\n            $canvas itemconfigure $id -fill [random_color]\n            if { [$canvas type $id] in {rectangle arc oval} } {\n                 $canvas itemconfigure $id -outline [random_color]\n            }\n        }\n        return\n    }\n    \n    # Run a demonstration.\n    proc demo {} {\n        # Create a toplevel window with a canvas filling the contents.\n        set win .gradients\n        if { [winfo exists $win] } {\n            destroy $win\n        }\n        toplevel $win\n        set cvs [canvas $win.cvs -highlightthickness 0]\n        pack $cvs -fill both -expand yes\n        wm geometry $win 800x600\n        raise $win\n\n        # Fill the bottom of the screen with a striped green fade.\n        gradient draw $cvs footer 0 0 10 10 vertical white darkgreen -dash {3 1}\n        bind $cvs <Configure> {\n            gradient resize %W footer 0 [expr {%h-300}] %w 300\n        }\n        \n        # Draw a strip of rainbow.\n        set width  100\n        set colors {white red orange yellow green blue purple violet white}\n        for {set i 1} {$i < [llength $colors]} {incr i} {\n            set c1 [lindex $colors $i-1]\n            set c2 [lindex $colors $i]\n            gradient draw $cvs "wave $i" [expr {$width*($i-1)}] 0 $width 50 horizontal $c1 $c2\n        }\n        \n        # Draw some balls with diameters of 100.\n        set colors {green red yellow blue orange white}\n        for {set i 0} {$i < 6} {incr i} {\n            gradient draw $cvs "beachball $i" 0 55 100 100 arc [lindex $colors $i] #333 -start [expr {$i*60}] -extent 60\n        }\n        set colors {cyan pink orange firebrick}\n        for {set i 0} {$i < [llength $colors]} {incr i} {\n            gradient draw $cvs "quadball $i" 110 55 100 100 arc [lindex $colors $i] #eee -start [expr {$i*90}] -extent 90\n        }\n        gradient draw $cvs ball1    220 55 100 100 circular #bbbbbb white\n        gradient draw $cvs ball2    330 55 100 100 circular #888 #eee\n        gradient draw $cvs ball3    440 55 100 100 circular black grey\n        gradient draw $cvs ball4    550 55 100 100 circular black #555\n        gradient draw $cvs ball5    660 55 100 100 circular cyan black\n        \n        # Draw some boxes.\n        gradient draw $cvs box1   0 160 150 100 horizontal white firebrick\n        gradient draw $cvs box2 150 160 200 100 central    black firebrick\n        gradient draw $cvs box3 350 160 100 100 horizontal firebrick black\n        gradient draw $cvs box4 450 160 200 100 central    firebrick black\n        gradient draw $cvs box5 650 160 150 100 horizontal black white\n        \n        # Display some control buttons.\n        frame $cvs.f\n        button $cvs.f.b1 -text "Redraw with random gradient colors" -command [list [namespace current]::randomize_all_gradient_colors $cvs]\n        button $cvs.f.b2 -text "Relaunch demo with default colors" -command [list [namespace current]::demo]\n        button $cvs.f.b3 -text "Chaos" -command [list [namespace current]::randomize_all_canvas_item_colors $cvs]\n        pack $cvs.f.b1 $cvs.f.b2 $cvs.f.b3 -fill x\n        $cvs create window 400 400 -window $cvs.f\n\n        return\n    }\n}\n        ')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
-                            54 LOAD_CONST               0 (None)
+                            54 LOAD_CONST               2 (None)
                             56 RETURN_VALUE
                consts
-                  None
+                  '\n        初始化渐变引擎\n        '
                   '\n        # Create color gradients of various shapes and sizes on a canvas.\n#   Usage:\n#       gradient draw    <canvas> <tags> <x> <y> <width> <height> <vertical|horizontal|circular|central|arc> <color1> <color2>  ?-animate? ?option? ...\n#       gradient redraw  <canvas> <tags> <x> <y> <width> <height> <vertical|horizontal|circular|central|arc> <color1> <color2>  ?-animate? ?option? ...\n#       gradient resize  <canvas> <tags> <x> <y> <width> <height>\n#       gradient recolor <canvas> <tags> <color1> <color2>\n\nnamespace eval gradient {\n    namespace ensemble create -subcommands {\n        draw\n        redraw\n        recolor\n        resize\n        demo\n    }\n\n    # Create a gradient on a canvas. The gradient will be placed at the top of the display list.\n    proc draw {canvas tags x y width height orient color1 color2 args} {\n        # Ensure valid colors are provided while also converting to lists of 16-bit RGB values.\n        if { [catch {winfo rgb . $color1} rgb1] } {\n            error "invalid color: $color1"\n        }\n        if { [catch {winfo rgb . $color2} rgb2] } {\n            error "invalid color: $color2"\n        }\n        \n        # Delete the gradient if it already exists.\n        $canvas delete [join $tags &&]\n        \n        # Create a hidden canvas item to store meta data about this gradient.\n        set meta_data [list x $x  y $y  width $width  height $height  orient $orient  color1 $color1  color2 $color2  args $args]\n        $canvas create line $x $y $x $y  -state hidden  -tags [list {*}$tags meta [list gradient: {*}$meta_data]]\n        \n        # Intercept the -animate option.\n        if { "-animate" in $args} {\n            set index [lsearch $args "-animate"]\n            set args  [lreplace $args $index $index]\n            set animate 1\n        } else {\n            set animate 0\n        }\n        \n        # Draw the gradient.\n        if { $orient eq "central" } {\n            # Create the canvas rectangle items.\n            foreach {x1 y1 x2 y2 color} [get_rects $x $y $width $height $rgb1 $rgb2] {\n                $canvas create rectangle $x1 $y1 $x2 $y2  -outline $color  -width 2  -tags $tags  {*}$args\n                if {$animate} {update}\n            }\n        } elseif { $orient eq "circular" } {\n            # Create the canvas oval items.\n            foreach {x1 y1 x2 y2 color} [get_rects $x $y $width $height $rgb1 $rgb2] {\n                $canvas create oval $x1 $y1 $x2 $y2  -outline $color  -width 2  -tags $tags  {*}$args\n                if {$animate} {update}\n            }\n        } elseif { $orient eq "arc" } {\n            # Create the canvas arc items.\n            foreach {x1 y1 x2 y2 color} [get_rects $x $y $width $height $rgb1 $rgb2] {\n                $canvas create arc $x1 $y1 $x2 $y2  -outline $color  -width 2  -tags $tags  -style arc  {*}$args\n                if {$animate} {update}\n            }\n        } elseif { $orient in [list "vertical" "horizontal"] } {        \n            # Create the canvas line items.\n            foreach {x1 y1 x2 y2 color} [get_lines $x $y $width $height $orient $rgb1 $rgb2] {\n                $canvas create line $x1 $y1 $x2 $y2  -fill $color  -tags $tags  -capstyle projecting  {*}$args\n                if {$animate} {update}\n            }\n        } else {\n            # Delete the meta data and throw an error.\n            $canvas delete [join $tags &&]\n            error "invalid orientation: $orient; must be: vertical, horizontal, circular, central, or arc"\n        }\n        \n        return\n    }\n    \n    # Same as draw, but if the gradient already exists then it will retain its position in the canvas\'s display list after being redrawn.\n    proc redraw {canvas tags x y width height orient color1 color2 args} {\n        # If the gradient already exists, remember its location in the display list.\n        set item_above [$canvas find above [join $tags &&]]\n        \n        # Draw the gradient.\n        draw $canvas $tags $x $y $width $height $orient $color1 $color2 {*}$args\n        \n        # Move the gradient to its previous location in the display list, if any.\n        if { $item_above ne "" } {\n            $canvas lower [join $tags &&] $item_above\n        }\n        \n        return\n    }\n    \n    # Shortcut procedure to change the colors of the gradient. Same as redraw but introspectively determines some meta data. \n    # This will use the gradient\'s x/y location when it was last drawn.\n    proc recolor {canvas tags color1 color2} {\n        # Retrieve the gradient\'s meta data.\n        set meta [get_meta_data $canvas $tags]\n        set meta [dict remove $meta color1 color2]\n        dict with meta {}\n        \n        # Redraw the gradient with the new colors.\n        redraw $canvas $tags $x $y $width $height $orient $color1 $color2 {*}$args\n        return     \n    }\n    \n    # Shortcut procedure to resize and reposition a gradient. Same as redraw but introspectively determines some meta data. \n    proc resize {canvas tags x y width height} {\n        # Retrieve the gradient\'s meta data.\n        set meta [get_meta_data $canvas $tags]\n        set meta [dict remove $meta x y width height]\n        dict with meta {}\n        \n        # Recreate the canvas lines with the new dimensions.\n        redraw $canvas $tags $x $y $width $height $orient $color1 $color2 {*}$args\n        return\n    }\n    \n    # Retrieve meta information on a gradient.\n    proc get_meta_data {canvas tags} {\n        if { [string is integer -strict $tags] } {\n            # This is supposedly a canvas item ID instead of a list of tags describing a gradient. Avoid introducing subtle logic errors.\n            error "cannot provide canvas item ID in lieu of gradient tags: $tags"\n        }\n        # This is a list of tags for a gradient. Find the hidden meta item for this gradient.\n        set all_tags [$canvas gettags "meta&&[join $tags &&]"]\n        set meta_data [lrange [lsearch -inline -index 0 $all_tags "gradient:"] 1 end]\n        if { [llength $meta_data] == 0 } {\n            error "cannot find meta data for gradient with tags: $tags"\n        }\n        return $meta_data\n    }\n    \n    # For a canvas item ID, return all tags that are not gradient meta tags.\n    proc get_non_meta_tags {canvas id} {\n        set tags [$canvas gettags $id]\n        set index [lsearch $tags "meta"]\n        set tags [lreplace $tags $index $index]\n        set index [lsearch -index 0 $tags "gradient:"]\n        set tags [lreplace $tags $index $index]\n        return $tags\n    }\n\n    # Calculate a list of center-to-outward colored rectangles suitable for [canvas create rectangle] or [canvas create oval].\n    proc get_rects {x y width height rgb1 rgb2} {\n        set rects [list]\n        set x1 [expr {int($x)+1}]\n        set y1 [expr {int($y)+1}]\n        set x2 [expr {$x1+$width-1}]\n        set y2 [expr {$y1+$height-1}]\n        \n        # Calculate each rectangle.\n        if { $width > $height } {\n            # Decrement X by one pixel in both directions. Decrement Y by a fraction in both directions.\n            # The Y axis will be more heavily concentrated.\n            set ratio  [expr { 1.0*$height/$width }]\n            set length [expr { $width/2 }]\n            while { $x2 > $x1 } {\n                lappend rects $x1 $y1 $x2 $y2 [get_color $rgb1 $rgb2 $length [expr { ($x2-$x1)/2 }]]\n                set x1 [expr { $x1+1 }]\n                set x2 [expr { $x2-1 }]\n                set y1 [expr { $y1+$ratio }]\n                set y2 [expr { $y2-$ratio }]\n            }\n        } else {\n            # Decrement Y by one pixel in both directions. Decrement X by a fraction in both directions.\n            # The X axis will be more heavily concentrated (unless width==height).\n            set ratio  [expr { 1.0*$width/$height }]\n            set length [expr { $height/2 }]\n            while { $y2 > $y1 } {\n                lappend rects $x1 $y1 $x2 $y2 [get_color $rgb1 $rgb2 $length [expr { ($y2-$y1)/2 }]]\n                set x1 [expr { $x1+$ratio }]\n                set x2 [expr { $x2-$ratio }]\n                set y1 [expr { $y1+1 }]\n                set y2 [expr { $y2-1 }]\n            }\n        }\n        return $rects\n    }\n\n    # Calculate a list of left-to-right or top-to-bottom colored lines suitable for [canvas create line].\n    proc get_lines {x1 y1 width height orient rgb1 rgb2} {\n        set lines [list]\n        set x1 [expr {int($x1)}]\n        set y1 [expr {int($y1)}]\n        set x2 [expr {$x1+$width}]\n        set y2 [expr {$y1+$height}]\n        if { $orient eq "vertical" } {\n            # Calculate the color for each horizontal line.\n            for {set y $y1} {$y < $y2} {incr y} {\n                lappend lines $x1 $y $x2 $y [get_color $rgb1 $rgb2 $height [expr {$y-$y1}]]\n            }\n        } elseif { $orient eq "horizontal" } {\n            # Calculate the color for each vertical column.\n            for {set x $x1} {$x < $x2} {incr x} {\n                lappend lines $x $y1 $x $y2 [get_color $rgb1 $rgb2 $width [expr {$x-$x1}]]\n            }\n        } else {\n            error "invalid orientation: $orient; must be: vertical or horizontal"\n        }\n        \n        return $lines\n    }\n\n    # Calculates the color at the specified index between rgb1 and rgb2 where rgb1 and rgb2 are the specified length apart.\n    proc get_color {rgb1 rgb2 length index} {\n        # Throw an error if the index is out of bounds.\n        if { $index < 0  ||  $index >= $length } {\n            error "index $index is out of bounds for length $length"\n        }\n        \n        lassign $rgb1 r1 g1 b1\n        lassign $rgb2 r2 g2 b2\n        \n        # Determine the ratio between each starting component color and ending component color.\n        set r_ratio [expr { 1.00*($r2-$r1+1)/$length }]\n        set g_ratio [expr { 1.00*($g2-$g1+1)/$length }]\n        set b_ratio [expr { 1.00*($b2-$b1+1)/$length }]\n\n        # Calculate the new component colors at the given index. \n        set r [expr { int($r_ratio*$index+$r1) }]\n        set g [expr { int($g_ratio*$index+$g1) }]\n        set b [expr { int($b_ratio*$index+$b1) }]\n\n        # A hacky workaround to make up for a lack of precision (or faulty math?).\n        # The final pixel of the gradient should exactly match the color of rgb2\n        if { $index == [expr {$length-1}] } {\n            lassign $rgb2 r g b\n        }\n\n        # Convert the integer RGB values to a hex color.\n        return [rgb_to_hex [list $r $g $b]]\n    }\n    \n    # Convert a list of 16-bit RGB values to an 8-bit hex color. Using 8-bit hex colors instead of 16-bit\n    # speeds up drawing of images two-fold (I haven\'t benchmarked this for canvases).\n    proc rgb_to_hex {rgb} {\n        lassign $rgb r g b\n        set r [format %02x [expr {$r/256}]]\n        set g [format %02x [expr {$g/256}]]\n        set b [format %02x [expr {$b/256}]]\n        return #$r$g$b\n    }\n    \n    # Converts 8-bit RGB values to 16-bit RGB values.\n    proc rgb_8_to_16_bit {rgb} {\n        lassign $rgb r g b\n        return [list [expr {$r*256}] [expr {$g*256}] [expr {$b*256}]]\n    }\n    \n    # Returns a random 8-bit hex color.\n    proc random_color {} {\n        return [rgb_to_hex "[expr {int(rand()*65536)}] [expr {int(rand()*65536)}] [expr {int(rand()*65536)}]"]\n    }\n\n    # Redraw all gradients with random colors\n    proc randomize_all_gradient_colors {canvas} {\n        foreach id [$canvas find withtag meta] {\n            set tags [get_non_meta_tags $canvas $id]\n            recolor $canvas $tags [random_color] [random_color]\n        }\n      return\n    }\n    \n    # Randomize colors for all canvas items.\n    proc randomize_all_canvas_item_colors {canvas} {\n        foreach id [$canvas find withtag all] {\n            if { [$canvas type $id] in {window} } {\n                continue\n            }\n            $canvas itemconfigure $id -fill [random_color]\n            if { [$canvas type $id] in {rectangle arc oval} } {\n                 $canvas itemconfigure $id -outline [random_color]\n            }\n        }\n        return\n    }\n    \n    # Run a demonstration.\n    proc demo {} {\n        # Create a toplevel window with a canvas filling the contents.\n        set win .gradients\n        if { [winfo exists $win] } {\n            destroy $win\n        }\n        toplevel $win\n        set cvs [canvas $win.cvs -highlightthickness 0]\n        pack $cvs -fill both -expand yes\n        wm geometry $win 800x600\n        raise $win\n\n        # Fill the bottom of the screen with a striped green fade.\n        gradient draw $cvs footer 0 0 10 10 vertical white darkgreen -dash {3 1}\n        bind $cvs <Configure> {\n            gradient resize %W footer 0 [expr {%h-300}] %w 300\n        }\n        \n        # Draw a strip of rainbow.\n        set width  100\n        set colors {white red orange yellow green blue purple violet white}\n        for {set i 1} {$i < [llength $colors]} {incr i} {\n            set c1 [lindex $colors $i-1]\n            set c2 [lindex $colors $i]\n            gradient draw $cvs "wave $i" [expr {$width*($i-1)}] 0 $width 50 horizontal $c1 $c2\n        }\n        \n        # Draw some balls with diameters of 100.\n        set colors {green red yellow blue orange white}\n        for {set i 0} {$i < 6} {incr i} {\n            gradient draw $cvs "beachball $i" 0 55 100 100 arc [lindex $colors $i] #333 -start [expr {$i*60}] -extent 60\n        }\n        set colors {cyan pink orange firebrick}\n        for {set i 0} {$i < [llength $colors]} {incr i} {\n            gradient draw $cvs "quadball $i" 110 55 100 100 arc [lindex $colors $i] #eee -start [expr {$i*90}] -extent 90\n        }\n        gradient draw $cvs ball1    220 55 100 100 circular #bbbbbb white\n        gradient draw $cvs ball2    330 55 100 100 circular #888 #eee\n        gradient draw $cvs ball3    440 55 100 100 circular black grey\n        gradient draw $cvs ball4    550 55 100 100 circular black #555\n        gradient draw $cvs ball5    660 55 100 100 circular cyan black\n        \n        # Draw some boxes.\n        gradient draw $cvs box1   0 160 150 100 horizontal white firebrick\n        gradient draw $cvs box2 150 160 200 100 central    black firebrick\n        gradient draw $cvs box3 350 160 100 100 horizontal firebrick black\n        gradient draw $cvs box4 450 160 200 100 central    firebrick black\n        gradient draw $cvs box5 650 160 150 100 horizontal black white\n        \n        # Display some control buttons.\n        frame $cvs.f\n        button $cvs.f.b1 -text "Redraw with random gradient colors" -command [list [namespace current]::randomize_all_gradient_colors $cvs]\n        button $cvs.f.b2 -text "Relaunch demo with default colors" -command [list [namespace current]::demo]\n        button $cvs.f.b3 -text "Chaos" -command [list [namespace current]::randomize_all_canvas_item_colors $cvs]\n        pack $cvs.f.b1 $cvs.f.b2 $cvs.f.b3 -fill x\n        $cvs create window 400 400 -window $cvs.f\n\n        return\n    }\n}\n        '
+                  None
                names      ('tk', 'eval')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'gradient_init'
-               firstlineno 269
-               lnotab 0x0201
+               firstlineno 272
+               lnotab 0x0204
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab00000000000000000001007c006a010000000000000000a002000000
                   000000000000000000000000000000000064016402a6020000ab02000000
-                  0000000000010064005300
-               611           0 RESUME                   0
+                  0000000000010064035300
+               617           0 RESUME                   0
                
-               612           2 LOAD_FAST                0 (self)
+               621           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (gradient_init)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                
-               613          42 LOAD_FAST                0 (self)
+               622          42 LOAD_FAST                0 (self)
                             44 LOAD_ATTR                1 (tk)
                             54 LOAD_METHOD              2 (call)
                             76 LOAD_CONST               1 ('gradient')
                             78 LOAD_CONST               2 ('demo')
                             80 PRECALL                  2
                             84 CALL                     2
                             94 POP_TOP
-                            96 LOAD_CONST               0 (None)
+                            96 LOAD_CONST               3 (None)
                             98 RETURN_VALUE
                consts
-                  None
+                  '\n        启动渐变引擎示例\n        '
                   'gradient'
                   'demo'
+                  None
                names      ('gradient_init', 'tk', 'call')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'gradient_demo'
-               firstlineno 611
-               lnotab 0x02012801
+               firstlineno 617
+               lnotab 0x02042801
             'tags'
             'x'
             'y'
             'width'
             'height'
             code
                argcount  : 6
@@ -786,118 +789,120 @@
                stacksize : 10
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab00000000000000000001007c006a010000000000000000a002000000
                   0000000000000000000000000000000000640164027c006a030000000000
                   0000007c017c027c037c047c05a6080000ab080000000000000000010064
-                  005300
-               615           0 RESUME                   0
+                  035300
+               624           0 RESUME                   0
                
-               616           2 LOAD_FAST                0 (self)
+               628           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (gradient_init)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                
-               617          42 LOAD_FAST                0 (self)
+               629          42 LOAD_FAST                0 (self)
                             44 LOAD_ATTR                1 (tk)
                             54 LOAD_METHOD              2 (call)
                             76 LOAD_CONST               1 ('gradient')
                             78 LOAD_CONST               2 ('resize')
                             80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                3 (_w)
                             92 LOAD_FAST                1 (tags)
                             94 LOAD_FAST                2 (x)
                             96 LOAD_FAST                3 (y)
                             98 LOAD_FAST                4 (width)
                            100 LOAD_FAST                5 (height)
                            102 PRECALL                  8
                            106 CALL                     8
                            116 POP_TOP
-                           118 LOAD_CONST               0 (None)
+                           118 LOAD_CONST               3 (None)
                            120 RETURN_VALUE
                consts
-                  None
+                  '\n        修改渐变图形的大小位置\n        '
                   'gradient'
                   'resize'
+                  None
                names      ('gradient_init', 'tk', 'call', '_w')
                varnames   ('self', 'tags', 'x', 'y', 'width', 'height')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'gradient_resize'
-               firstlineno 615
-               lnotab 0x02012801
+               firstlineno 624
+               lnotab 0x02042801
             code
                argcount  : 6
                nlocals   : 6
                stacksize : 8
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab00000000000000000001007c006a010000000000000000a002000000
                   0000000000000000000000000000000000640164027c006a030000000000
-                  0000007c017c047c05a6060000ab060000000000000000010064005300
-               619           0 RESUME                   0
+                  0000007c017c047c05a6060000ab060000000000000000010064035300
+               631           0 RESUME                   0
                
-               620           2 LOAD_FAST                0 (self)
+               635           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (gradient_init)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                
-               621          42 LOAD_FAST                0 (self)
+               636          42 LOAD_FAST                0 (self)
                             44 LOAD_ATTR                1 (tk)
                             54 LOAD_METHOD              2 (call)
                             76 LOAD_CONST               1 ('gradient')
                             78 LOAD_CONST               2 ('color')
                             80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                3 (_w)
                             92 LOAD_FAST                1 (tags)
                             94 LOAD_FAST                4 (color1)
                             96 LOAD_FAST                5 (color2)
                             98 PRECALL                  6
                            102 CALL                     6
                            112 POP_TOP
-                           114 LOAD_CONST               0 (None)
+                           114 LOAD_CONST               3 (None)
                            116 RETURN_VALUE
                consts
-                  None
+                  '\n        修改渐变组件的颜色\n        '
                   'gradient'
                   'color'
+                  None
                names      ('gradient_init', 'tk', 'call', '_w')
                varnames   ('self', 'tags', 'x', 'y', 'color1', 'color2')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'gradient_recolor'
-               firstlineno 619
-               lnotab 0x02012801
+               firstlineno 631
+               lnotab 0x02042801
             code
                argcount  : 9
                nlocals   : 12
                stacksize : 13
                flags     : 15
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab00000000000000000001007c006a010000000000000000a002000000
                   0000000000000000000000000000000000640164027c006a030000000000
                   0000007c017c027c037c047c057c067c077c08a60b0000ab0b0000000000
                   0000007d0b02007c006a0400000000000000007c0167017c09a201520069
                   007c0aa4018e0101007c0b5300
-               623           0 RESUME                   0
+               638           0 RESUME                   0
                
-               625           2 LOAD_FAST                0 (self)
+               643           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (gradient_init)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                
-               626          42 LOAD_FAST                0 (self)
+               644          42 LOAD_FAST                0 (self)
                             44 LOAD_ATTR                1 (tk)
                             54 LOAD_METHOD              2 (call)
                             76 LOAD_CONST               1 ('gradient')
                             78 LOAD_CONST               2 ('draw')
                             80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                3 (_w)
                             92 LOAD_FAST                1 (tags)
@@ -908,230 +913,231 @@
                            102 LOAD_FAST                6 (orient)
                            104 LOAD_FAST                7 (color1)
                            106 LOAD_FAST                8 (color2)
                            108 PRECALL                 11
                            112 CALL                    11
                            122 STORE_FAST              11 (id)
                
-               627         124 PUSH_NULL
+               645         124 PUSH_NULL
                            126 LOAD_FAST                0 (self)
                            128 LOAD_ATTR                4 (itemconfigure)
                            138 LOAD_FAST                1 (tags)
                            140 BUILD_LIST               1
                            142 LOAD_FAST                9 (args)
                            144 LIST_EXTEND              1
                            146 LIST_TO_TUPLE
                            148 BUILD_MAP                0
                            150 LOAD_FAST               10 (kwargs)
                            152 DICT_MERGE               1
                            154 CALL_FUNCTION_EX         1
                            156 POP_TOP
                
-               628         158 LOAD_FAST               11 (id)
+               646         158 LOAD_FAST               11 (id)
                            160 RETURN_VALUE
                consts
-                  None
+                  '\n        绘制渐变图形\n        '
                   'gradient'
                   'draw'
                names      ('gradient_init', 'tk', 'call', '_w', 'itemconfigure')
                varnames   ('self', 'tags', 'x', 'y', 'width', 'height', 'orient', 'color1', 'color2', 'args', 'kwargs', 'id')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'gradient_draw'
-               firstlineno 623
-               lnotab 0x0202280152012201
+               firstlineno 638
+               lnotab 0x0205280152012201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x970002007c006a0000000000000000007c0169007c02a4018e01010064
-                  005300
-               630           0 RESUME                   0
+                  015300
+               648           0 RESUME                   0
                
-               631           2 PUSH_NULL
+               652           2 PUSH_NULL
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (gradient_draw)
                             16 LOAD_FAST                1 (args)
                             18 BUILD_MAP                0
                             20 LOAD_FAST                2 (kwargs)
                             22 DICT_MERGE               1
                             24 CALL_FUNCTION_EX         1
                             26 POP_TOP
-                            28 LOAD_CONST               0 (None)
+                            28 LOAD_CONST               1 (None)
                             30 RETURN_VALUE
                consts
+                  '\n        同gradient_draw\n        '
                   None
                names      ('gradient_draw',)
                varnames   ('self', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'gradient_redraw'
-               firstlineno 630
-               lnotab 0x0201
+               firstlineno 648
+               lnotab 0x0204
             code
                argcount  : 8
                nlocals   : 10
                stacksize : 12
                flags     : 15
                code
                   0x970002007c006a0000000000000000007c087c057c017c027c037c047c
                   067c0774020000000000000000000064019c087c09a4018e015300
-               633           0 RESUME                   0
+               654           0 RESUME                   0
                
-               634           2 PUSH_NULL
+               667           2 PUSH_NULL
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (gradient_draw)
                
-               635          16 LOAD_FAST                8 (args)
+               668          16 LOAD_FAST                8 (args)
                
-               634          18 LOAD_FAST                5 (tags)
+               667          18 LOAD_FAST                5 (tags)
                             20 LOAD_FAST                1 (x)
                             22 LOAD_FAST                2 (y)
                             24 LOAD_FAST                3 (width)
                             26 LOAD_FAST                4 (height)
                             28 LOAD_FAST                6 (color1)
                             30 LOAD_FAST                7 (color2)
                
-               635          32 LOAD_GLOBAL              2 (VERTICAL)
+               668          32 LOAD_GLOBAL              2 (VERTICAL)
                
-               634          44 LOAD_CONST               1 (('tags', 'x', 'y', 'width', 'height', 'color1', 'color2', 'orient'))
+               667          44 LOAD_CONST               1 (('tags', 'x', 'y', 'width', 'height', 'color1', 'color2', 'orient'))
                             46 BUILD_CONST_KEY_MAP      8
                
-               635          48 LOAD_FAST                9 (kwargs)
+               668          48 LOAD_FAST                9 (kwargs)
                
-               634          50 DICT_MERGE               1
+               667          50 DICT_MERGE               1
                             52 CALL_FUNCTION_EX         1
                             54 RETURN_VALUE
                consts
-                  None
+                  '\n        创建水平渐变矩形\n\n        :param x: 图形x位置\n        :param y: 图形y位置\n        :param width: 图形宽度\n        :param height: 图形高度\n        :param tags: 标签名\n        :param color1: 渐变颜色1\n        :param color2: 渐变颜色2\n        :return:\n        '
                   ('tags', 'x', 'y', 'width', 'height', 'color1', 'color2', 'orient')
                names      ('gradient_draw', 'VERTICAL')
                varnames   ('self', 'x', 'y', 'width', 'height', 'tags', 'color1', 'color2', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'create_gradient_v_rectangle'
-               firstlineno 633
-               lnotab 0x02010e0102ff0e010cff040102ff
+               firstlineno 654
+               lnotab 0x020d0e0102ff0e010cff040102ff
             code
                argcount  : 8
                nlocals   : 10
                stacksize : 12
                flags     : 15
                code
                   0x970002007c006a0000000000000000007c087c057c017c027c037c047c
                   067c0774020000000000000000000064019c087c09a4018e015300
-               637           0 RESUME                   0
+               670           0 RESUME                   0
                
-               638           2 PUSH_NULL
+               683           2 PUSH_NULL
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (gradient_draw)
                
-               639          16 LOAD_FAST                8 (args)
+               684          16 LOAD_FAST                8 (args)
                
-               638          18 LOAD_FAST                5 (tags)
+               683          18 LOAD_FAST                5 (tags)
                             20 LOAD_FAST                1 (x)
                             22 LOAD_FAST                2 (y)
                             24 LOAD_FAST                3 (width)
                             26 LOAD_FAST                4 (height)
                             28 LOAD_FAST                6 (color1)
                             30 LOAD_FAST                7 (color2)
                
-               639          32 LOAD_GLOBAL              2 (HORIZONTAL)
+               684          32 LOAD_GLOBAL              2 (HORIZONTAL)
                
-               638          44 LOAD_CONST               1 (('tags', 'x', 'y', 'width', 'height', 'color1', 'color2', 'orient'))
+               683          44 LOAD_CONST               1 (('tags', 'x', 'y', 'width', 'height', 'color1', 'color2', 'orient'))
                             46 BUILD_CONST_KEY_MAP      8
                
-               639          48 LOAD_FAST                9 (kwargs)
+               684          48 LOAD_FAST                9 (kwargs)
                
-               638          50 DICT_MERGE               1
+               683          50 DICT_MERGE               1
                             52 CALL_FUNCTION_EX         1
                             54 RETURN_VALUE
                consts
-                  None
+                  '\n        创建垂直渐变矩形\n\n        :param x: 图形x位置\n        :param y: 图形y位置\n        :param width: 图形宽度\n        :param height: 图形高度\n        :param tags: 标签名\n        :param color1: 渐变颜色1\n        :param color2: 渐变颜色2\n        :return:\n        '
                   ('tags', 'x', 'y', 'width', 'height', 'color1', 'color2', 'orient')
                names      ('gradient_draw', 'HORIZONTAL')
                varnames   ('self', 'x', 'y', 'width', 'height', 'tags', 'color1', 'color2', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'create_gradient_h_rectangle'
-               firstlineno 637
-               lnotab 0x02010e0102ff0e010cff040102ff
+               firstlineno 670
+               lnotab 0x020d0e0102ff0e010cff040102ff
             code
                argcount  : 8
                nlocals   : 10
                stacksize : 12
                flags     : 15
                code
                   0x970002007c006a0000000000000000007c087c057c017c027c037c047c
                   067c0774020000000000000000000064019c087c09a4018e015300
-               641           0 RESUME                   0
+               686           0 RESUME                   0
                
-               642           2 PUSH_NULL
+               699           2 PUSH_NULL
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (gradient_draw)
                
-               643          16 LOAD_FAST                8 (args)
+               700          16 LOAD_FAST                8 (args)
                
-               642          18 LOAD_FAST                5 (tags)
+               699          18 LOAD_FAST                5 (tags)
                             20 LOAD_FAST                1 (x)
                             22 LOAD_FAST                2 (y)
                             24 LOAD_FAST                3 (width)
                             26 LOAD_FAST                4 (height)
                             28 LOAD_FAST                6 (color1)
                             30 LOAD_FAST                7 (color2)
                
-               643          32 LOAD_GLOBAL              2 (CIRCULAR)
+               700          32 LOAD_GLOBAL              2 (CIRCULAR)
                
-               642          44 LOAD_CONST               1 (('tags', 'x', 'y', 'width', 'height', 'color1', 'color2', 'orient'))
+               699          44 LOAD_CONST               1 (('tags', 'x', 'y', 'width', 'height', 'color1', 'color2', 'orient'))
                             46 BUILD_CONST_KEY_MAP      8
                
-               643          48 LOAD_FAST                9 (kwargs)
+               700          48 LOAD_FAST                9 (kwargs)
                
-               642          50 DICT_MERGE               1
+               699          50 DICT_MERGE               1
                             52 CALL_FUNCTION_EX         1
                             54 RETURN_VALUE
                consts
-                  None
+                  '\n        创建垂直渐变圆形\n\n        :param x: 图形x位置\n        :param y: 图形y位置\n        :param width: 图形宽度\n        :param height: 图形高度\n        :param tags: 标签名\n        :param color1: 渐变颜色1\n        :param color2: 渐变颜色2\n        :return:\n        '
                   ('tags', 'x', 'y', 'width', 'height', 'color1', 'color2', 'orient')
                names      ('gradient_draw', 'CIRCULAR')
                varnames   ('self', 'x', 'y', 'width', 'height', 'tags', 'color1', 'color2', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'create_gradient_circular'
-               firstlineno 641
-               lnotab 0x02010e0102ff0e010cff040102ff
+               firstlineno 686
+               lnotab 0x020d0e0102ff0e010cff040102ff
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 7
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab01000000000000000001007c006a0000
                   00000000000000a002000000000000000000000000000000000000000064
                   027c006a0300000000000000007c037c017c02a6050000ab050000000000
                   000000010064005300
-               645           0 RESUME                   0
+               702           0 RESUME                   0
                
-               646           2 LOAD_FAST                0 (self)
+               703           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (tk)
                             14 LOAD_METHOD              1 (eval)
                             36 LOAD_CONST               1 ('\n  proc + {n1 n2} {\n    expr {$n1 + $n2}\n  }\n  proc - {n1 n2} {\n    expr {$n1 - $n2}\n  }\n  proc * {n1 n2} {\n    expr {$n1 * $n2}\n  }\n  proc / {n1 n2} {\n    expr {$n1 / $n2}\n  }\n  proc toInt {n} {\n    expr int($n)\n  }\n  \n  proc drawGradient {win type col1Str col2Str} {\n    $win delete gradient\n    \n    set width [winfo width $win]\n    set height [winfo height $win]\n    \n    lassign [winfo rgb $win $col1Str] r1 g1 b1\n    lassign  [winfo rgb $win $col2Str] r2 g2 b2\n    set rRange [- $r2.0 $r1]\n    set gRange [- $g2.0 $g1]\n    set bRange [- $b2.0 $b1]\n  \n    if {$type == "x"} {\n      set rRatio [/ $rRange $width]\n      set gRatio [/ $gRange $width]\n      set bRatio [/ $bRange $width]\n    \n      for {set x 0} {$x < $width} {incr x} {\n        set nR [toInt [+ $r1 [* $rRatio $x]]]\n        set nG [toInt [+ $g1 [* $gRatio $x]]]\n        set nB [toInt [+ $b1 [* $bRatio $x]]]\n  \n        set col [format {%4.4x} $nR]\n        append col [format {%4.4x} $nG]\n        append col [format {%4.4x} $nB]\n        $win create line $x 0 $x $height -tags gradient -fill #${col}\n      }\n    } else {\n      set rRatio [/ $rRange $height]\n      set gRatio [/ $gRange $height]\n      set bRatio [/ $bRange $height]\n  \n      for {set y 0} {$y < $height} {incr y} {\n        set nR [toInt [+ $r1 [* $rRatio $y]]]\n        set nG [toInt [+ $g1 [* $gRatio $y]]]\n        set nB [toInt [+ $b1 [* $bRatio $y]]]\n  \n        set col [format {%4.4x} $nR]\n        append col [format {%4.4x} $nG]\n        append col [format {%4.4x} $nB]\n        $win create line 0 $y $width $y -tags gradient -fill #${col}\n      }\n    }\n    return $win\n  }\n        ')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               710          54 LOAD_FAST                0 (self)
+               767          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                0 (tk)
                             66 LOAD_METHOD              2 (call)
                             88 LOAD_CONST               2 ('drawGradient')
                             90 LOAD_FAST                0 (self)
                             92 LOAD_ATTR                3 (_w)
                            102 LOAD_FAST                3 (type)
                            104 LOAD_FAST                1 (color1)
@@ -1147,15 +1153,15 @@
                   'drawGradient'
                names      ('tk', 'eval', 'call', '_w')
                varnames   ('self', 'color1', 'color2', 'type')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'draw_gradient'
-               firstlineno 645
+               firstlineno 702
                lnotab 0x02013440
             5
             2
             'white'
             'black'
             'radius'
             code
@@ -1193,110 +1199,110 @@
                   067a0a00007c037c0664017a0b00007a0a00007c047c0964017a0b00007a
                   0a00007c067a0000007c076405ac08a6060000ab0600000000000000007d
                   137c00a00200000000000000000000000000000000000000007c017c0964
                   017a0b00007a0000007c067a0a00007c047c0964017a0b00007a0a00007c
                   037c0964017a0b00007a0a00007c067a0000007c047c0664017a0b00007a
                   0a00007c076405ac08a6060000ab0600000000000000007d147c0a7c0b7c
                   0c7c0d7c0e7c0f7c107c117c127c137c1464099c0b5300
-               712           0 RESUME                   0
+               769           0 RESUME                   0
                
-               714           2 LOAD_FAST                5 (radius)
+               774           2 LOAD_FAST                5 (radius)
                              4 LOAD_CONST               1 (2)
                              6 BINARY_OP                5 (*)
                             10 STORE_FAST               9 (_radius)
                
-               715          12 LOAD_FAST                0 (self)
+               775          12 LOAD_FAST                0 (self)
                             14 LOAD_METHOD              0 (create_arc)
                             36 LOAD_FAST                1 (x1)
                             38 LOAD_FAST                2 (y1)
                             40 LOAD_FAST                1 (x1)
                             42 LOAD_FAST                9 (_radius)
                             44 BINARY_OP                0 (+)
                             48 LOAD_FAST                2 (y1)
                             50 LOAD_FAST                9 (_radius)
                             52 BINARY_OP                0 (+)
                             56 LOAD_CONST               2 (90)
                             58 LOAD_CONST               2 (90)
                             60 LOAD_FAST                6 (width)
                             62 LOAD_FAST                7 (fill)
                
-               716          64 LOAD_FAST                8 (outline)
+               776          64 LOAD_FAST                8 (outline)
                
-               715          66 KW_NAMES                 3
+               775          66 KW_NAMES                 3
                             68 PRECALL                  9
                             72 CALL                     9
                             82 STORE_FAST              10 (nw)
                
-               717          84 LOAD_FAST                0 (self)
+               777          84 LOAD_FAST                0 (self)
                             86 LOAD_METHOD              0 (create_arc)
                            108 LOAD_FAST                1 (x1)
                            110 LOAD_FAST                4 (y2)
                            112 LOAD_FAST                1 (x1)
                            114 LOAD_FAST                9 (_radius)
                            116 BINARY_OP                0 (+)
                            120 LOAD_FAST                4 (y2)
                            122 LOAD_FAST                9 (_radius)
                            124 BINARY_OP               10 (-)
                            128 LOAD_CONST               4 (180)
                            130 LOAD_CONST               2 (90)
                            132 LOAD_FAST                6 (width)
                            134 LOAD_FAST                7 (fill)
                
-               718         136 LOAD_FAST                8 (outline)
+               778         136 LOAD_FAST                8 (outline)
                
-               717         138 KW_NAMES                 3
+               777         138 KW_NAMES                 3
                            140 PRECALL                  9
                            144 CALL                     9
                            154 STORE_FAST              11 (sw)
                
-               719         156 LOAD_FAST                0 (self)
+               779         156 LOAD_FAST                0 (self)
                            158 LOAD_METHOD              0 (create_arc)
                            180 LOAD_FAST                3 (x2)
                            182 LOAD_FAST                9 (_radius)
                            184 BINARY_OP               10 (-)
                            188 LOAD_FAST                2 (y1)
                            190 LOAD_FAST                3 (x2)
                            192 LOAD_FAST                2 (y1)
                            194 LOAD_FAST                9 (_radius)
                            196 BINARY_OP                0 (+)
                            200 LOAD_CONST               5 (0)
                            202 LOAD_CONST               2 (90)
                            204 LOAD_FAST                6 (width)
                            206 LOAD_FAST                7 (fill)
                
-               720         208 LOAD_FAST                8 (outline)
+               780         208 LOAD_FAST                8 (outline)
                
-               719         210 KW_NAMES                 3
+               779         210 KW_NAMES                 3
                            212 PRECALL                  9
                            216 CALL                     9
                            226 STORE_FAST              12 (ne)
                
-               721         228 LOAD_FAST                0 (self)
+               781         228 LOAD_FAST                0 (self)
                            230 LOAD_METHOD              0 (create_arc)
                            252 LOAD_FAST                3 (x2)
                            254 LOAD_FAST                9 (_radius)
                            256 BINARY_OP               10 (-)
                            260 LOAD_FAST                4 (y2)
                            262 LOAD_FAST                3 (x2)
                            264 LOAD_FAST                4 (y2)
                            266 LOAD_FAST                9 (_radius)
                            268 BINARY_OP               10 (-)
                            272 LOAD_CONST               6 (270)
                            274 LOAD_CONST               2 (90)
                            276 LOAD_FAST                6 (width)
                            278 LOAD_FAST                7 (fill)
                
-               722         280 LOAD_FAST                8 (outline)
+               782         280 LOAD_FAST                8 (outline)
                
-               721         282 KW_NAMES                 3
+               781         282 KW_NAMES                 3
                            284 PRECALL                  9
                            288 CALL                     9
                            298 STORE_FAST              13 (se)
                
-               724         300 LOAD_FAST                0 (self)
+               784         300 LOAD_FAST                0 (self)
                            302 LOAD_METHOD              1 (create_line)
                            324 LOAD_FAST                1 (x1)
                            326 LOAD_FAST                2 (y1)
                            328 LOAD_FAST                9 (_radius)
                            330 LOAD_CONST               1 (2)
                            332 BINARY_OP               11 (/)
                            336 BINARY_OP                0 (+)
@@ -1309,15 +1315,15 @@
                            356 LOAD_FAST                6 (width)
                            358 LOAD_FAST                8 (outline)
                            360 KW_NAMES                 7
                            362 PRECALL                  6
                            366 CALL                     6
                            376 STORE_FAST              14 (w)
                
-               725         378 LOAD_FAST                0 (self)
+               785         378 LOAD_FAST                0 (self)
                            380 LOAD_METHOD              1 (create_line)
                            402 LOAD_FAST                1 (x1)
                            404 LOAD_FAST                9 (_radius)
                            406 LOAD_CONST               1 (2)
                            408 BINARY_OP               11 (/)
                            412 BINARY_OP                0 (+)
                            416 LOAD_FAST                2 (y1)
@@ -1330,15 +1336,15 @@
                            434 LOAD_FAST                6 (width)
                            436 LOAD_FAST                8 (outline)
                            438 KW_NAMES                 7
                            440 PRECALL                  6
                            444 CALL                     6
                            454 STORE_FAST              15 (n)
                
-               726         456 LOAD_FAST                0 (self)
+               786         456 LOAD_FAST                0 (self)
                            458 LOAD_METHOD              1 (create_line)
                            480 LOAD_FAST                3 (x2)
                            482 LOAD_FAST                2 (y1)
                            484 LOAD_FAST                9 (_radius)
                            486 LOAD_CONST               1 (2)
                            488 BINARY_OP               11 (/)
                            492 BINARY_OP                0 (+)
@@ -1351,15 +1357,15 @@
                            512 LOAD_FAST                6 (width)
                            514 LOAD_FAST                8 (outline)
                            516 KW_NAMES                 7
                            518 PRECALL                  6
                            522 CALL                     6
                            532 STORE_FAST              16 (e)
                
-               727         534 LOAD_FAST                0 (self)
+               787         534 LOAD_FAST                0 (self)
                            536 LOAD_METHOD              1 (create_line)
                            558 LOAD_FAST                1 (x1)
                            560 LOAD_FAST                9 (_radius)
                            562 LOAD_CONST               1 (2)
                            564 BINARY_OP               11 (/)
                            568 BINARY_OP                0 (+)
                            572 LOAD_FAST                4 (y2)
@@ -1372,15 +1378,15 @@
                            590 LOAD_FAST                6 (width)
                            592 LOAD_FAST                8 (outline)
                            594 KW_NAMES                 7
                            596 PRECALL                  6
                            600 CALL                     6
                            610 STORE_FAST              17 (s)
                
-               729         612 LOAD_FAST                0 (self)
+               789         612 LOAD_FAST                0 (self)
                            614 LOAD_METHOD              2 (create_rectangle)
                            636 LOAD_FAST                1 (x1)
                            638 LOAD_FAST                9 (_radius)
                            640 LOAD_CONST               1 (2)
                            642 BINARY_OP               11 (/)
                            646 BINARY_OP                0 (+)
                            650 LOAD_FAST                6 (width)
@@ -1394,29 +1400,29 @@
                            672 LOAD_FAST                9 (_radius)
                            674 LOAD_CONST               1 (2)
                            676 BINARY_OP               11 (/)
                            680 BINARY_OP               10 (-)
                            684 LOAD_FAST                6 (width)
                            686 BINARY_OP                0 (+)
                
-               730         690 LOAD_FAST                2 (y1)
+               790         690 LOAD_FAST                2 (y1)
                            692 LOAD_FAST                9 (_radius)
                            694 LOAD_CONST               1 (2)
                            696 BINARY_OP               11 (/)
                            700 BINARY_OP                0 (+)
                            704 LOAD_FAST                7 (fill)
                
-               731         706 LOAD_CONST               5 (0)
+               791         706 LOAD_CONST               5 (0)
                
-               729         708 KW_NAMES                 8
+               789         708 KW_NAMES                 8
                            710 PRECALL                  6
                            714 CALL                     6
                            724 STORE_FAST              18 (top)
                
-               733         726 LOAD_FAST                0 (self)
+               793         726 LOAD_FAST                0 (self)
                            728 LOAD_METHOD              2 (create_rectangle)
                            750 LOAD_FAST                1 (x1)
                            752 LOAD_FAST                6 (width)
                            754 LOAD_CONST               1 (2)
                            756 BINARY_OP               11 (/)
                            760 BINARY_OP                0 (+)
                            764 LOAD_FAST                2 (y1)
@@ -1428,31 +1434,31 @@
                            780 BINARY_OP               10 (-)
                            784 LOAD_FAST                3 (x2)
                            786 LOAD_FAST                6 (width)
                            788 LOAD_CONST               1 (2)
                            790 BINARY_OP               11 (/)
                            794 BINARY_OP               10 (-)
                
-               734         798 LOAD_FAST                4 (y2)
+               794         798 LOAD_FAST                4 (y2)
                            800 LOAD_FAST                9 (_radius)
                            802 LOAD_CONST               1 (2)
                            804 BINARY_OP               11 (/)
                            808 BINARY_OP               10 (-)
                            812 LOAD_FAST                6 (width)
                            814 BINARY_OP                0 (+)
                            818 LOAD_FAST                7 (fill)
                
-               735         820 LOAD_CONST               5 (0)
+               795         820 LOAD_CONST               5 (0)
                
-               733         822 KW_NAMES                 8
+               793         822 KW_NAMES                 8
                            824 PRECALL                  6
                            828 CALL                     6
                            838 STORE_FAST              19 (center)
                
-               737         840 LOAD_FAST                0 (self)
+               797         840 LOAD_FAST                0 (self)
                            842 LOAD_METHOD              2 (create_rectangle)
                            864 LOAD_FAST                1 (x1)
                            866 LOAD_FAST                9 (_radius)
                            868 LOAD_CONST               1 (2)
                            870 BINARY_OP               11 (/)
                            874 BINARY_OP                0 (+)
                            878 LOAD_FAST                6 (width)
@@ -1466,46 +1472,46 @@
                            900 LOAD_FAST                9 (_radius)
                            902 LOAD_CONST               1 (2)
                            904 BINARY_OP               11 (/)
                            908 BINARY_OP               10 (-)
                            912 LOAD_FAST                6 (width)
                            914 BINARY_OP                0 (+)
                
-               738         918 LOAD_FAST                4 (y2)
+               798         918 LOAD_FAST                4 (y2)
                            920 LOAD_FAST                6 (width)
                            922 LOAD_CONST               1 (2)
                            924 BINARY_OP               11 (/)
                            928 BINARY_OP               10 (-)
                            932 LOAD_FAST                7 (fill)
                
-               739         934 LOAD_CONST               5 (0)
+               799         934 LOAD_CONST               5 (0)
                
-               737         936 KW_NAMES                 8
+               797         936 KW_NAMES                 8
                            938 PRECALL                  6
                            942 CALL                     6
                            952 STORE_FAST              20 (bottom)
                
-               742         954 LOAD_FAST               10 (nw)
+               802         954 LOAD_FAST               10 (nw)
                            956 LOAD_FAST               11 (sw)
                            958 LOAD_FAST               12 (ne)
                            960 LOAD_FAST               13 (se)
                            962 LOAD_FAST               14 (w)
                            964 LOAD_FAST               15 (n)
                            966 LOAD_FAST               16 (e)
                            968 LOAD_FAST               17 (s)
                
-               743         970 LOAD_FAST               18 (top)
+               803         970 LOAD_FAST               18 (top)
                            972 LOAD_FAST               19 (center)
                            974 LOAD_FAST               20 (bottom)
                
-               741         976 LOAD_CONST               9 (('nw', 'sw', 'ne', 'se', 'w', 'n', 'e', 's', 'top', 'center', 'bottom'))
+               801         976 LOAD_CONST               9 (('nw', 'sw', 'ne', 'se', 'w', 'n', 'e', 's', 'top', 'center', 'bottom'))
                            978 BUILD_CONST_KEY_MAP     11
                            980 RETURN_VALUE
                consts
-                  None
+                  '\n        创建圆角矩形 ： 自绘版\n        '
                   2
                   90
                   ('start', 'extent', 'width', 'fill', 'outline')
                   180
                   0
                   270
                   ('width', 'fill')
@@ -1513,109 +1519,109 @@
                   ('nw', 'sw', 'ne', 'se', 'w', 'n', 'e', 's', 'top', 'center', 'bottom')
                names      ('create_arc', 'create_line', 'create_rectangle')
                varnames   ('self', 'x1', 'y1', 'x2', 'y2', 'radius', 'width', 'fill', 'outline', '_radius', 'nw', 'sw', 'ne', 'se', 'w', 'n', 'e', 's', 'top', 'center', 'bottom')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'create_round_rectangle'
-               firstlineno 712
+               firstlineno 769
                lnotab
-                  0x02020a01340102ff1202340102ff1202340102ff1202340102ff12034e
+                  0x02050a01340102ff1202340102ff1202340102ff1202340102ff12034e
                   014e014e014e024e01100102fe12044801160102fe12044e01100102fe12
                   05100106fe
             code
                argcount  : 6
                nlocals   : 9
                stacksize : 9
                flags     : 15
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab01000000000000000001007c006a0000
                   00000000000000a002000000000000000000000000000000000000000064
                   027c006a0300000000000000007c017c027c037c047c05a6070000ab0700
                   000000000000007d0802007c006a0400000000000000007c0867017c06a2
                   01520069007c07a4018e0101007c085300
-               748           0 RESUME                   0
+               808           0 RESUME                   0
                
-               750           2 LOAD_FAST                0 (self)
+               813           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (tk)
                             14 LOAD_METHOD              1 (eval)
                             36 LOAD_CONST               1 ("\n#----------------------------------------------------------------------\n#\n# roundRect --\n#\n#       Draw a rounded rectangle in the canvas.\n#\n# Parameters:\n#       w - Path name of the canvas\n#       x0, y0 - Co-ordinates of the upper left corner, in pixels\n#       x3, y3 - Co-ordinates of the lower right corner, in pixels\n#       radius - Radius of the bend at the corners, in any form\n#                acceptable to Tk_GetPixels\n#       args - Other args suitable to a 'polygon' item on the canvas\n#\n# Results:\n#       Returns the canvas item number of the rounded rectangle.\n#\n# Side effects:\n#       Creates a rounded rectangle as a smooth polygon in the canvas.\n#\n#----------------------------------------------------------------------\n\nproc roundRect { w x0 y0 x3 y3 radius args } {\n\nset r [winfo pixels $w $radius]\nset d [expr { 2 * $r }]\n\n# Make sure that the radius of the curve is less than 3/8\n# size of the box!\n\nset maxr 0.75\n\nif { $d > $maxr * ( $x3 - $x0 ) } {\n    set d [expr { $maxr * ( $x3 - $x0 ) }]\n}\nif { $d > $maxr * ( $y3 - $y0 ) } {\n    set d [expr { $maxr * ( $y3 - $y0 ) }]\n}\n\nset x1 [expr { $x0 + $d }]\nset x2 [expr { $x3 - $d }]\nset y1 [expr { $y0 + $d }]\nset y2 [expr { $y3 - $d }]\n\nset cmd [list $w create polygon]\nlappend cmd $x0 $y0\nlappend cmd $x1 $y0\nlappend cmd $x2 $y0\nlappend cmd $x3 $y0\nlappend cmd $x3 $y1\nlappend cmd $x3 $y2\nlappend cmd $x3 $y3\nlappend cmd $x2 $y3\nlappend cmd $x1 $y3\nlappend cmd $x0 $y3\nlappend cmd $x0 $y2\nlappend cmd $x0 $y1\nlappend cmd -smooth 1\nreturn [eval $cmd $args]\n}\n        ")
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               812          54 LOAD_FAST                0 (self)
+               875          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                0 (tk)
                             66 LOAD_METHOD              2 (call)
                             88 LOAD_CONST               2 ('roundRect')
                             90 LOAD_FAST                0 (self)
                             92 LOAD_ATTR                3 (_w)
                            102 LOAD_FAST                1 (x0)
                            104 LOAD_FAST                2 (y0)
                            106 LOAD_FAST                3 (x3)
                            108 LOAD_FAST                4 (y3)
                            110 LOAD_FAST                5 (radius)
                            112 PRECALL                  7
                            116 CALL                     7
                            126 STORE_FAST               8 (rect)
                
-               813         128 PUSH_NULL
+               876         128 PUSH_NULL
                            130 LOAD_FAST                0 (self)
                            132 LOAD_ATTR                4 (itemconfig)
                            142 LOAD_FAST                8 (rect)
                            144 BUILD_LIST               1
                            146 LOAD_FAST                6 (args)
                            148 LIST_EXTEND              1
                            150 LIST_TO_TUPLE
                            152 BUILD_MAP                0
                            154 LOAD_FAST                7 (kwargs)
                            156 DICT_MERGE               1
                            158 CALL_FUNCTION_EX         1
                            160 POP_TOP
                
-               814         162 LOAD_FAST                8 (rect)
+               877         162 LOAD_FAST                8 (rect)
                            164 RETURN_VALUE
                consts
-                  None
+                  '\n        创建圆角矩形 ： 其他开发者制作 ： 边框有问题（不推荐）\n        '
                   "\n#----------------------------------------------------------------------\n#\n# roundRect --\n#\n#       Draw a rounded rectangle in the canvas.\n#\n# Parameters:\n#       w - Path name of the canvas\n#       x0, y0 - Co-ordinates of the upper left corner, in pixels\n#       x3, y3 - Co-ordinates of the lower right corner, in pixels\n#       radius - Radius of the bend at the corners, in any form\n#                acceptable to Tk_GetPixels\n#       args - Other args suitable to a 'polygon' item on the canvas\n#\n# Results:\n#       Returns the canvas item number of the rounded rectangle.\n#\n# Side effects:\n#       Creates a rounded rectangle as a smooth polygon in the canvas.\n#\n#----------------------------------------------------------------------\n\nproc roundRect { w x0 y0 x3 y3 radius args } {\n\nset r [winfo pixels $w $radius]\nset d [expr { 2 * $r }]\n\n# Make sure that the radius of the curve is less than 3/8\n# size of the box!\n\nset maxr 0.75\n\nif { $d > $maxr * ( $x3 - $x0 ) } {\n    set d [expr { $maxr * ( $x3 - $x0 ) }]\n}\nif { $d > $maxr * ( $y3 - $y0 ) } {\n    set d [expr { $maxr * ( $y3 - $y0 ) }]\n}\n\nset x1 [expr { $x0 + $d }]\nset x2 [expr { $x3 - $d }]\nset y1 [expr { $y0 + $d }]\nset y2 [expr { $y3 - $d }]\n\nset cmd [list $w create polygon]\nlappend cmd $x0 $y0\nlappend cmd $x1 $y0\nlappend cmd $x2 $y0\nlappend cmd $x3 $y0\nlappend cmd $x3 $y1\nlappend cmd $x3 $y2\nlappend cmd $x3 $y3\nlappend cmd $x2 $y3\nlappend cmd $x1 $y3\nlappend cmd $x0 $y3\nlappend cmd $x0 $y2\nlappend cmd $x0 $y1\nlappend cmd -smooth 1\nreturn [eval $cmd $args]\n}\n        "
                   'roundRect'
                names      ('tk', 'eval', 'call', '_w', 'itemconfig')
                varnames   ('self', 'x0', 'y0', 'x3', 'y3', 'radius', 'args', 'kwargs', 'rect')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'create_round_rectangle2'
-               firstlineno 748
-               lnotab 0x0202343e4a012201
+               firstlineno 808
+               lnotab 0x0205343e4a012201
             'fill'
             'outline'
             code
                argcount  : 9
                nlocals   : 12
                stacksize : 12
                flags     : 15
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab01000000000000000001007c006a0000
                   00000000000000a002000000000000000000000000000000000000000064
                   027c006a0300000000000000007c027c037c067c047c057c077c087c01a6
                   0a0000ab0a00000000000000007d0b02007c006a0400000000000000007c
                   0b67017c09a201520069007c0aa4018e0101007c0b5300
-               818           0 RESUME                   0
+               881           0 RESUME                   0
                
-               821           2 LOAD_FAST                0 (self)
+               887           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (tk)
                             14 LOAD_METHOD              1 (eval)
                             36 LOAD_CONST               1 ('\nproc roundRect2 {w L T Rad width height fill outline tag} {\n\n  $w create oval $L $T [expr $L + $Rad] [expr $T + $Rad] -fill $fill -outline $outline -tag $tag\n  $w create oval [expr $width-$Rad] $T $width [expr $T + $Rad] -fill $fill -outline $outline -tag $tag\n  $w create oval $L [expr $height-$Rad] [expr $L+$Rad] $height -fill $fill -outline $outline -tag $tag\n  $w create oval [expr $width-$Rad] [expr $height-$Rad] [expr $width] $height -fill $fill -outline $outline -tag $tag\n  $w create rectangle [expr $L + ($Rad/2.0)] $T [expr $width-($Rad/2.0)] $height -fill $fill -outline $outline -tag $tag\n  $w create rectangle $L [expr $T + ($Rad/2.0)] $width [expr $height-($Rad/2.0)] -fill $fill -outline $outline -tag $tag\n}\n            ')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               832          54 LOAD_FAST                0 (self)
+               898          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                0 (tk)
                             66 LOAD_METHOD              2 (call)
                             88 LOAD_CONST               2 ('roundRect2')
                             90 LOAD_FAST                0 (self)
                             92 LOAD_ATTR                3 (_w)
                            102 LOAD_FAST                2 (x)
                            104 LOAD_FAST                3 (y)
@@ -1625,42 +1631,42 @@
                            112 LOAD_FAST                7 (fill)
                            114 LOAD_FAST                8 (outline)
                            116 LOAD_FAST                1 (tag)
                            118 PRECALL                 10
                            122 CALL                    10
                            132 STORE_FAST              11 (_rect)
                
-               833         134 PUSH_NULL
+               899         134 PUSH_NULL
                            136 LOAD_FAST                0 (self)
                            138 LOAD_ATTR                4 (itemconfig)
                            148 LOAD_FAST               11 (_rect)
                            150 BUILD_LIST               1
                            152 LOAD_FAST                9 (args)
                            154 LIST_EXTEND              1
                            156 LIST_TO_TUPLE
                            158 BUILD_MAP                0
                            160 LOAD_FAST               10 (kwargs)
                            162 DICT_MERGE               1
                            164 CALL_FUNCTION_EX         1
                            166 POP_TOP
                
-               834         168 LOAD_FAST               11 (_rect)
+               900         168 LOAD_FAST               11 (_rect)
                            170 RETURN_VALUE
                consts
-                  None
+                  '\n        创建圆角矩形 ： 其他开发者制作 ： 圆角看起来更舒服\n        '
                   '\nproc roundRect2 {w L T Rad width height fill outline tag} {\n\n  $w create oval $L $T [expr $L + $Rad] [expr $T + $Rad] -fill $fill -outline $outline -tag $tag\n  $w create oval [expr $width-$Rad] $T $width [expr $T + $Rad] -fill $fill -outline $outline -tag $tag\n  $w create oval $L [expr $height-$Rad] [expr $L+$Rad] $height -fill $fill -outline $outline -tag $tag\n  $w create oval [expr $width-$Rad] [expr $height-$Rad] [expr $width] $height -fill $fill -outline $outline -tag $tag\n  $w create rectangle [expr $L + ($Rad/2.0)] $T [expr $width-($Rad/2.0)] $height -fill $fill -outline $outline -tag $tag\n  $w create rectangle $L [expr $T + ($Rad/2.0)] $width [expr $height-($Rad/2.0)] -fill $fill -outline $outline -tag $tag\n}\n            '
                   'roundRect2'
                names      ('tk', 'eval', 'call', '_w', 'itemconfig')
                varnames   ('self', 'tag', 'x', 'y', 'width', 'height', 'radius', 'fill', 'outline', 'args', 'kwargs', '_rect')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'create_round_rectangle3'
-               firstlineno 818
-               lnotab 0x0203340b50012201
+               firstlineno 881
+               lnotab 0x0206340b50012201
             code
                argcount  : 6
                nlocals   : 9
                stacksize : 6
                flags     : 11
                code
                   0x970067007c017c057a00000091017c0291017c017c057a00000091017c
@@ -1670,237 +1676,237 @@
                   0a000091017c0391017c0491017c037c057a0a000091017c0491017c037c
                   057a0a000091017c0491017c017c057a00000091017c0491017c017c057a
                   00000091017c0491017c0191017c0491017c0191017c047c057a0a000091
                   017c0191017c047c057a0a000091017c0191017c027c057a00000091017c
                   0191017c027c057a00000091017c0191017c0291017d0702007c006a0000
                   000000000000007c07660169007c06a401640164026901a4018e017d087c
                   085300
-               838           0 RESUME                   0
+               904           0 RESUME                   0
                
-               839           2 BUILD_LIST               0
+               908           2 BUILD_LIST               0
                              4 LOAD_FAST                1 (x1)
                              6 LOAD_FAST                5 (radius)
                              8 BINARY_OP                0 (+)
                             12 LIST_APPEND              1
                             14 LOAD_FAST                2 (y1)
                             16 LIST_APPEND              1
                
-               840          18 LOAD_FAST                1 (x1)
+               909          18 LOAD_FAST                1 (x1)
                             20 LOAD_FAST                5 (radius)
                             22 BINARY_OP                0 (+)
                
-               839          26 LIST_APPEND              1
+               908          26 LIST_APPEND              1
                
-               840          28 LOAD_FAST                2 (y1)
+               909          28 LOAD_FAST                2 (y1)
                
-               839          30 LIST_APPEND              1
+               908          30 LIST_APPEND              1
                
-               841          32 LOAD_FAST                3 (x2)
+               910          32 LOAD_FAST                3 (x2)
                             34 LOAD_FAST                5 (radius)
                             36 BINARY_OP               10 (-)
                
-               839          40 LIST_APPEND              1
+               908          40 LIST_APPEND              1
                
-               841          42 LOAD_FAST                2 (y1)
+               910          42 LOAD_FAST                2 (y1)
                
-               839          44 LIST_APPEND              1
+               908          44 LIST_APPEND              1
                
-               842          46 LOAD_FAST                3 (x2)
+               911          46 LOAD_FAST                3 (x2)
                             48 LOAD_FAST                5 (radius)
                             50 BINARY_OP               10 (-)
                
-               839          54 LIST_APPEND              1
+               908          54 LIST_APPEND              1
                
-               842          56 LOAD_FAST                2 (y1)
+               911          56 LOAD_FAST                2 (y1)
                
-               839          58 LIST_APPEND              1
+               908          58 LIST_APPEND              1
                
-               843          60 LOAD_FAST                3 (x2)
+               912          60 LOAD_FAST                3 (x2)
                
-               839          62 LIST_APPEND              1
+               908          62 LIST_APPEND              1
                
-               843          64 LOAD_FAST                2 (y1)
+               912          64 LOAD_FAST                2 (y1)
                
-               839          66 LIST_APPEND              1
+               908          66 LIST_APPEND              1
                
-               844          68 LOAD_FAST                3 (x2)
+               913          68 LOAD_FAST                3 (x2)
                
-               839          70 LIST_APPEND              1
+               908          70 LIST_APPEND              1
                
-               844          72 LOAD_FAST                2 (y1)
+               913          72 LOAD_FAST                2 (y1)
                             74 LOAD_FAST                5 (radius)
                             76 BINARY_OP                0 (+)
                
-               839          80 LIST_APPEND              1
+               908          80 LIST_APPEND              1
                
-               845          82 LOAD_FAST                3 (x2)
+               914          82 LOAD_FAST                3 (x2)
                
-               839          84 LIST_APPEND              1
+               908          84 LIST_APPEND              1
                
-               845          86 LOAD_FAST                2 (y1)
+               914          86 LOAD_FAST                2 (y1)
                             88 LOAD_FAST                5 (radius)
                             90 BINARY_OP                0 (+)
                
-               839          94 LIST_APPEND              1
+               908          94 LIST_APPEND              1
                
-               846          96 LOAD_FAST                3 (x2)
+               915          96 LOAD_FAST                3 (x2)
                
-               839          98 LIST_APPEND              1
+               908          98 LIST_APPEND              1
                
-               846         100 LOAD_FAST                4 (y2)
+               915         100 LOAD_FAST                4 (y2)
                            102 LOAD_FAST                5 (radius)
                            104 BINARY_OP               10 (-)
                
-               839         108 LIST_APPEND              1
+               908         108 LIST_APPEND              1
                
-               847         110 LOAD_FAST                3 (x2)
+               916         110 LOAD_FAST                3 (x2)
                
-               839         112 LIST_APPEND              1
+               908         112 LIST_APPEND              1
                
-               847         114 LOAD_FAST                4 (y2)
+               916         114 LOAD_FAST                4 (y2)
                            116 LOAD_FAST                5 (radius)
                            118 BINARY_OP               10 (-)
                
-               839         122 LIST_APPEND              1
+               908         122 LIST_APPEND              1
                
-               848         124 LOAD_FAST                3 (x2)
+               917         124 LOAD_FAST                3 (x2)
                
-               839         126 LIST_APPEND              1
+               908         126 LIST_APPEND              1
                
-               848         128 LOAD_FAST                4 (y2)
+               917         128 LOAD_FAST                4 (y2)
                
-               839         130 LIST_APPEND              1
+               908         130 LIST_APPEND              1
                
-               849         132 LOAD_FAST                3 (x2)
+               918         132 LOAD_FAST                3 (x2)
                            134 LOAD_FAST                5 (radius)
                            136 BINARY_OP               10 (-)
                
-               839         140 LIST_APPEND              1
+               908         140 LIST_APPEND              1
                
-               849         142 LOAD_FAST                4 (y2)
+               918         142 LOAD_FAST                4 (y2)
                
-               839         144 LIST_APPEND              1
+               908         144 LIST_APPEND              1
                
-               850         146 LOAD_FAST                3 (x2)
+               919         146 LOAD_FAST                3 (x2)
                            148 LOAD_FAST                5 (radius)
                            150 BINARY_OP               10 (-)
                
-               839         154 LIST_APPEND              1
+               908         154 LIST_APPEND              1
                
-               850         156 LOAD_FAST                4 (y2)
+               919         156 LOAD_FAST                4 (y2)
                
-               839         158 LIST_APPEND              1
+               908         158 LIST_APPEND              1
                
-               851         160 LOAD_FAST                1 (x1)
+               920         160 LOAD_FAST                1 (x1)
                            162 LOAD_FAST                5 (radius)
                            164 BINARY_OP                0 (+)
                
-               839         168 LIST_APPEND              1
+               908         168 LIST_APPEND              1
                
-               851         170 LOAD_FAST                4 (y2)
+               920         170 LOAD_FAST                4 (y2)
                
-               839         172 LIST_APPEND              1
+               908         172 LIST_APPEND              1
                
-               852         174 LOAD_FAST                1 (x1)
+               921         174 LOAD_FAST                1 (x1)
                            176 LOAD_FAST                5 (radius)
                            178 BINARY_OP                0 (+)
                
-               839         182 LIST_APPEND              1
+               908         182 LIST_APPEND              1
                
-               852         184 LOAD_FAST                4 (y2)
+               921         184 LOAD_FAST                4 (y2)
                
-               839         186 LIST_APPEND              1
+               908         186 LIST_APPEND              1
                
-               853         188 LOAD_FAST                1 (x1)
+               922         188 LOAD_FAST                1 (x1)
                
-               839         190 LIST_APPEND              1
+               908         190 LIST_APPEND              1
                
-               853         192 LOAD_FAST                4 (y2)
+               922         192 LOAD_FAST                4 (y2)
                
-               839         194 LIST_APPEND              1
+               908         194 LIST_APPEND              1
                
-               854         196 LOAD_FAST                1 (x1)
+               923         196 LOAD_FAST                1 (x1)
                
-               839         198 LIST_APPEND              1
+               908         198 LIST_APPEND              1
                
-               854         200 LOAD_FAST                4 (y2)
+               923         200 LOAD_FAST                4 (y2)
                            202 LOAD_FAST                5 (radius)
                            204 BINARY_OP               10 (-)
                
-               839         208 LIST_APPEND              1
+               908         208 LIST_APPEND              1
                
-               855         210 LOAD_FAST                1 (x1)
+               924         210 LOAD_FAST                1 (x1)
                
-               839         212 LIST_APPEND              1
+               908         212 LIST_APPEND              1
                
-               855         214 LOAD_FAST                4 (y2)
+               924         214 LOAD_FAST                4 (y2)
                            216 LOAD_FAST                5 (radius)
                            218 BINARY_OP               10 (-)
                
-               839         222 LIST_APPEND              1
+               908         222 LIST_APPEND              1
                
-               856         224 LOAD_FAST                1 (x1)
+               925         224 LOAD_FAST                1 (x1)
                
-               839         226 LIST_APPEND              1
+               908         226 LIST_APPEND              1
                
-               856         228 LOAD_FAST                2 (y1)
+               925         228 LOAD_FAST                2 (y1)
                            230 LOAD_FAST                5 (radius)
                            232 BINARY_OP                0 (+)
                
-               839         236 LIST_APPEND              1
+               908         236 LIST_APPEND              1
                
-               857         238 LOAD_FAST                1 (x1)
+               926         238 LOAD_FAST                1 (x1)
                
-               839         240 LIST_APPEND              1
+               908         240 LIST_APPEND              1
                
-               857         242 LOAD_FAST                2 (y1)
+               926         242 LOAD_FAST                2 (y1)
                            244 LOAD_FAST                5 (radius)
                            246 BINARY_OP                0 (+)
                
-               839         250 LIST_APPEND              1
+               908         250 LIST_APPEND              1
                
-               858         252 LOAD_FAST                1 (x1)
+               927         252 LOAD_FAST                1 (x1)
                
-               839         254 LIST_APPEND              1
+               908         254 LIST_APPEND              1
                
-               858         256 LOAD_FAST                2 (y1)
+               927         256 LOAD_FAST                2 (y1)
                
-               839         258 LIST_APPEND              1
+               908         258 LIST_APPEND              1
                            260 STORE_FAST               7 (points)
                
-               860         262 PUSH_NULL
+               929         262 PUSH_NULL
                            264 LOAD_FAST                0 (self)
                            266 LOAD_ATTR                0 (create_polygon)
                            276 LOAD_FAST                7 (points)
                            278 BUILD_TUPLE              1
                            280 BUILD_MAP                0
                            282 LOAD_FAST                6 (kwargs)
                            284 DICT_MERGE               1
                            286 LOAD_CONST               1 ('smooth')
                            288 LOAD_CONST               2 (True)
                            290 BUILD_MAP                1
                            292 DICT_MERGE               1
                            294 CALL_FUNCTION_EX         1
                            296 STORE_FAST               8 (_poly)
                
-               862         298 LOAD_FAST                8 (_poly)
+               931         298 LOAD_FAST                8 (_poly)
                            300 RETURN_VALUE
                consts
-                  None
+                  '\n        创建圆角矩形 ： 其他开发者制作\n        '
                   'smooth'
                   True
                names      ('create_polygon',)
                varnames   ('self', 'x1', 'y1', 'x2', 'y2', 'radius', 'kwargs', 'points', '_poly')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'create_round_rectangle4'
-               firstlineno 838
+               firstlineno 904
                lnotab
-                  0x0201100108ff020102ff020208fe020202fe020308fd020302fd020402
+                  0x0204100108ff020102ff020208fe020202fe020308fd020302fd020402
                   fc020402fc020502fb020508fb020602fa020608fa020702f9020708f902
                   0802f8020808f8020902f7020902f7020a08f6020a02f6020b08f5020b02
                   f5020c08f4020c02f4020d08f3020d02f3020e02f2020e02f2020f02f102
                   0f08f1021002f0021008f0021102ef021108ef021202ee021208ee021302
                   ed021302ed04152402
             code
                argcount  : 4
@@ -1910,25 +1916,25 @@
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000740400000000000000000000a6010000ab010000000000
                   00000001007c006a000000000000000000a0010000000000000000000000
                   00000000000000000064017c019b0064027c029b0064027c039b009d06a6
                   010000ab0100000000000000007d0602007c006a0300000000000000007c
                   0667017c04a201520069007c05a4018e0101007c065300
-               866           0 RESUME                   0
+               935           0 RESUME                   0
                
-               867           2 LOAD_FAST                0 (self)
+               936           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (tk)
                             14 LOAD_METHOD              1 (eval)
                             36 LOAD_GLOBAL              4 (poly)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               868          64 LOAD_FAST                0 (self)
+               937          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (tk)
                             76 LOAD_METHOD              1 (eval)
                             98 LOAD_CONST               1 ('poly_round ')
                            100 LOAD_FAST                1 (win)
                            102 FORMAT_VALUE             0
                            104 LOAD_CONST               2 (' ')
                            106 LOAD_FAST                2 (outline)
@@ -1937,85 +1943,85 @@
                            112 LOAD_FAST                3 (fill)
                            114 FORMAT_VALUE             0
                            116 BUILD_STRING             6
                            118 PRECALL                  1
                            122 CALL                     1
                            132 STORE_FAST               6 (_poly)
                
-               869         134 PUSH_NULL
+               938         134 PUSH_NULL
                            136 LOAD_FAST                0 (self)
                            138 LOAD_ATTR                3 (itemconfig)
                            148 LOAD_FAST                6 (_poly)
                            150 BUILD_LIST               1
                            152 LOAD_FAST                4 (args)
                            154 LIST_EXTEND              1
                            156 LIST_TO_TUPLE
                            158 BUILD_MAP                0
                            160 LOAD_FAST                5 (kwargs)
                            162 DICT_MERGE               1
                            164 CALL_FUNCTION_EX         1
                            166 POP_TOP
                
-               870         168 LOAD_FAST                6 (_poly)
+               939         168 LOAD_FAST                6 (_poly)
                            170 RETURN_VALUE
                consts
                   None
                   'poly_round '
                   ' '
                names      ('tk', 'eval', 'poly', 'itemconfig')
                varnames   ('self', 'win', 'outline', 'fill', 'args', 'kwargs', '_poly')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'polygon_round'
-               firstlineno 866
+               firstlineno 935
                lnotab 0x02013e0146012201
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x970064017d017c006a000000000000000000a001000000000000000000
                   0000000000000000000000740400000000000000000000a6010000ab0100
                   0000000000000001007c006a000000000000000000a00100000000000000
                   000000000000000000000000007c01a6010000ab01000000000000000001
                   0064005300
-               874           0 RESUME                   0
+                943           0 RESUME                   0
                
-               875           2 LOAD_CONST               1 ('\n package require Tcl 8.5\n package require Tk\n\n proc draw {win} {\n     global demo\n\n     set sharp_pts [list]\n     set round_pts [list]\n     for {set id 0} {$id < $demo(num_pts)} {incr id} {\n         set x [expr {([lindex [$win coords vtx#$id] 0] +\n                       [lindex [$win coords vtx#$id] 2]) / 2}]\n         set y [expr {([lindex [$win coords vtx#$id] 1] +\n                       [lindex [$win coords vtx#$id] 3]) / 2}]\n         lappend sharp_pts $x $y\n         lappend round_pts $x $y $demo(radius)\n     }\n\n     .c delete sharp_poly\n     .c create polygon {*}$sharp_pts -outline gray50 -fill ""             -dash {6 5} -tags {sharp_poly}\n\n     if {[info exists demo(tag)]} {\n         .c delete $demo(tag)\n     }\n     set demo(tag) [poly_round .c $demo(outline) $demo(fill) {*}$round_pts]\n     .c itemconfigure $demo(tag) -width $demo(thickness)\n\n     .c raise vtx\n }\n\n proc down {win x y} {\n     global demo\n\n     $win dtag selected\n     $win addtag selected withtag current\n     $win raise current\n     set demo(last_x) $x\n     set demo(last_y) $y\n }\n \n proc move {win x y} {\n     global demo\n\n     if {[info exists demo(last_x)]} {\n         $win move selected                 [expr {$x - $demo(last_x)}]                 [expr {$y - $demo(last_y)}]\n         set demo(last_x) $x\n         set demo(last_y) $y\n\n         draw $win\n     }\n }\n\n proc main {args} {\n     global demo\n\n     array set demo {\n         num_pts 3       radius 20      thickness 1\n         outline black   fill   white   background gray\n         width   400     height 400\n     }\n     foreach {option value} $args {\n         set option [regsub {^-} $option ""]\n         if {![info exists demo($option)]} {\n             puts "Options: -[join [array names demo] " -"]"\n             exit\n         } else {\n             set demo([regsub {^-} $option ""]) $value\n         }\n     }\n\n     canvas .c -width $demo(width) -height $demo(height) -highlightthickness 0             -background $demo(background)\n     pack .c\n     wm title . "Round Polygon Demo"\n     wm resizable . 0 0\n\n     set 2pi [expr {2 * acos(-1)}]\n     set cx [expr {$demo(width)  / 2}]; set sx [expr {$demo(width)  * 3 / 8}]\n     set cy [expr {$demo(height) / 2}]; set sy [expr {$demo(height) * 3 / 8}]\n     for {set id 0} {$id < $demo(num_pts)} {incr id} {\n         set x [expr {$cx + $sx * cos(($id + 0.5) * $2pi / $demo(num_pts))}]\n         set y [expr {$cy - $sy * sin(($id + 0.5) * $2pi / $demo(num_pts))}]\n         .c create oval [expr {$x - 3}] [expr {$y - 3}]                        [expr {$x + 3}] [expr {$y + 3}]                        -tags [list vtx vtx#$id] -fill brown\n     }\n\n     .c bind vtx <Any-Enter> {.c itemconfigure current -fill red}\n     .c bind vtx <Any-Leave> {.c itemconfigure current -fill brown}\n     .c bind vtx <ButtonPress-1> {down .c %x %y}\n     .c bind vtx <ButtonRelease-1> {.c dtag selected}\n     bind .c <B1-Motion> {move .c %x %y}\n\n     focus .c\n     draw .c\n }\n\n main\n\n        ')
-                             4 STORE_FAST               1 (demo)
+                944           2 LOAD_CONST               1 ('\n package require Tcl 8.5\n package require Tk\n\n proc draw {win} {\n     global demo\n\n     set sharp_pts [list]\n     set round_pts [list]\n     for {set id 0} {$id < $demo(num_pts)} {incr id} {\n         set x [expr {([lindex [$win coords vtx#$id] 0] +\n                       [lindex [$win coords vtx#$id] 2]) / 2}]\n         set y [expr {([lindex [$win coords vtx#$id] 1] +\n                       [lindex [$win coords vtx#$id] 3]) / 2}]\n         lappend sharp_pts $x $y\n         lappend round_pts $x $y $demo(radius)\n     }\n\n     .c delete sharp_poly\n     .c create polygon {*}$sharp_pts -outline gray50 -fill ""             -dash {6 5} -tags {sharp_poly}\n\n     if {[info exists demo(tag)]} {\n         .c delete $demo(tag)\n     }\n     set demo(tag) [poly_round .c $demo(outline) $demo(fill) {*}$round_pts]\n     .c itemconfigure $demo(tag) -width $demo(thickness)\n\n     .c raise vtx\n }\n\n proc down {win x y} {\n     global demo\n\n     $win dtag selected\n     $win addtag selected withtag current\n     $win raise current\n     set demo(last_x) $x\n     set demo(last_y) $y\n }\n \n proc move {win x y} {\n     global demo\n\n     if {[info exists demo(last_x)]} {\n         $win move selected                 [expr {$x - $demo(last_x)}]                 [expr {$y - $demo(last_y)}]\n         set demo(last_x) $x\n         set demo(last_y) $y\n\n         draw $win\n     }\n }\n\n proc main {args} {\n     global demo\n\n     array set demo {\n         num_pts 3       radius 20      thickness 1\n         outline black   fill   white   background gray\n         width   400     height 400\n     }\n     foreach {option value} $args {\n         set option [regsub {^-} $option ""]\n         if {![info exists demo($option)]} {\n             puts "Options: -[join [array names demo] " -"]"\n             exit\n         } else {\n             set demo([regsub {^-} $option ""]) $value\n         }\n     }\n\n     canvas .c -width $demo(width) -height $demo(height) -highlightthickness 0             -background $demo(background)\n     pack .c\n     wm title . "Round Polygon Demo"\n     wm resizable . 0 0\n\n     set 2pi [expr {2 * acos(-1)}]\n     set cx [expr {$demo(width)  / 2}]; set sx [expr {$demo(width)  * 3 / 8}]\n     set cy [expr {$demo(height) / 2}]; set sy [expr {$demo(height) * 3 / 8}]\n     for {set id 0} {$id < $demo(num_pts)} {incr id} {\n         set x [expr {$cx + $sx * cos(($id + 0.5) * $2pi / $demo(num_pts))}]\n         set y [expr {$cy - $sy * sin(($id + 0.5) * $2pi / $demo(num_pts))}]\n         .c create oval [expr {$x - 3}] [expr {$y - 3}]                        [expr {$x + 3}] [expr {$y + 3}]                        -tags [list vtx vtx#$id] -fill brown\n     }\n\n     .c bind vtx <Any-Enter> {.c itemconfigure current -fill red}\n     .c bind vtx <Any-Leave> {.c itemconfigure current -fill brown}\n     .c bind vtx <ButtonPress-1> {down .c %x %y}\n     .c bind vtx <ButtonRelease-1> {.c dtag selected}\n     bind .c <B1-Motion> {move .c %x %y}\n\n     focus .c\n     draw .c\n }\n\n main\n\n        ')
+                              4 STORE_FAST               1 (demo)
                
-               979           6 LOAD_FAST                0 (self)
-                             8 LOAD_ATTR                0 (tk)
-                            18 LOAD_METHOD              1 (eval)
-                            40 LOAD_GLOBAL              4 (poly)
-                            52 PRECALL                  1
-                            56 CALL                     1
-                            66 POP_TOP
-               
-               980          68 LOAD_FAST                0 (self)
-                            70 LOAD_ATTR                0 (tk)
-                            80 LOAD_METHOD              1 (eval)
-                           102 LOAD_FAST                1 (demo)
-                           104 PRECALL                  1
-                           108 CALL                     1
-                           118 POP_TOP
-                           120 LOAD_CONST               0 (None)
-                           122 RETURN_VALUE
+               1048           6 LOAD_FAST                0 (self)
+                              8 LOAD_ATTR                0 (tk)
+                             18 LOAD_METHOD              1 (eval)
+                             40 LOAD_GLOBAL              4 (poly)
+                             52 PRECALL                  1
+                             56 CALL                     1
+                             66 POP_TOP
+               
+               1049          68 LOAD_FAST                0 (self)
+                             70 LOAD_ATTR                0 (tk)
+                             80 LOAD_METHOD              1 (eval)
+                            102 LOAD_FAST                1 (demo)
+                            104 PRECALL                  1
+                            108 CALL                     1
+                            118 POP_TOP
+                            120 LOAD_CONST               0 (None)
+                            122 RETURN_VALUE
                consts
                   None
                   '\n package require Tcl 8.5\n package require Tk\n\n proc draw {win} {\n     global demo\n\n     set sharp_pts [list]\n     set round_pts [list]\n     for {set id 0} {$id < $demo(num_pts)} {incr id} {\n         set x [expr {([lindex [$win coords vtx#$id] 0] +\n                       [lindex [$win coords vtx#$id] 2]) / 2}]\n         set y [expr {([lindex [$win coords vtx#$id] 1] +\n                       [lindex [$win coords vtx#$id] 3]) / 2}]\n         lappend sharp_pts $x $y\n         lappend round_pts $x $y $demo(radius)\n     }\n\n     .c delete sharp_poly\n     .c create polygon {*}$sharp_pts -outline gray50 -fill ""             -dash {6 5} -tags {sharp_poly}\n\n     if {[info exists demo(tag)]} {\n         .c delete $demo(tag)\n     }\n     set demo(tag) [poly_round .c $demo(outline) $demo(fill) {*}$round_pts]\n     .c itemconfigure $demo(tag) -width $demo(thickness)\n\n     .c raise vtx\n }\n\n proc down {win x y} {\n     global demo\n\n     $win dtag selected\n     $win addtag selected withtag current\n     $win raise current\n     set demo(last_x) $x\n     set demo(last_y) $y\n }\n \n proc move {win x y} {\n     global demo\n\n     if {[info exists demo(last_x)]} {\n         $win move selected                 [expr {$x - $demo(last_x)}]                 [expr {$y - $demo(last_y)}]\n         set demo(last_x) $x\n         set demo(last_y) $y\n\n         draw $win\n     }\n }\n\n proc main {args} {\n     global demo\n\n     array set demo {\n         num_pts 3       radius 20      thickness 1\n         outline black   fill   white   background gray\n         width   400     height 400\n     }\n     foreach {option value} $args {\n         set option [regsub {^-} $option ""]\n         if {![info exists demo($option)]} {\n             puts "Options: -[join [array names demo] " -"]"\n             exit\n         } else {\n             set demo([regsub {^-} $option ""]) $value\n         }\n     }\n\n     canvas .c -width $demo(width) -height $demo(height) -highlightthickness 0             -background $demo(background)\n     pack .c\n     wm title . "Round Polygon Demo"\n     wm resizable . 0 0\n\n     set 2pi [expr {2 * acos(-1)}]\n     set cx [expr {$demo(width)  / 2}]; set sx [expr {$demo(width)  * 3 / 8}]\n     set cy [expr {$demo(height) / 2}]; set sy [expr {$demo(height) * 3 / 8}]\n     for {set id 0} {$id < $demo(num_pts)} {incr id} {\n         set x [expr {$cx + $sx * cos(($id + 0.5) * $2pi / $demo(num_pts))}]\n         set y [expr {$cy - $sy * sin(($id + 0.5) * $2pi / $demo(num_pts))}]\n         .c create oval [expr {$x - 3}] [expr {$y - 3}]                        [expr {$x + 3}] [expr {$y + 3}]                        -tags [list vtx vtx#$id] -fill brown\n     }\n\n     .c bind vtx <Any-Enter> {.c itemconfigure current -fill red}\n     .c bind vtx <Any-Leave> {.c itemconfigure current -fill brown}\n     .c bind vtx <ButtonPress-1> {down .c %x %y}\n     .c bind vtx <ButtonRelease-1> {.c dtag selected}\n     bind .c <B1-Motion> {move .c %x %y}\n\n     focus .c\n     draw .c\n }\n\n main\n\n        '
                names      ('tk', 'eval', 'poly')
                varnames   ('self', 'demo')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'demo_polygon_round'
-               firstlineno 874
+               firstlineno 943
                lnotab 0x020104683e01
             'content'
             code
                argcount  : 4
                nlocals   : 12
                stacksize : 6
                flags     : 11
@@ -2027,110 +2033,110 @@
                   097c09a00600000000000000000000000000000000000000007c03a60100
                   00ab01000000000000000001007c09a00700000000000000000000000000
                   00000000000000a6000000ab0000000000000000000100640064006400a6
                   020000ab02000000000000000001006e0b23003100730477027803590077
                   01010059000100010002007c067c08ac07a6010000ab0100000000000000
                   007d0a02007c006a0800000000000000007c017c02660264087c0a69017c
                   04a4018e017d0b7c0b5300
-               982           0 RESUME                   0
+               1051           0 RESUME                   0
                
-               983           2 LOAD_CONST               1 (0)
-                             4 LOAD_CONST               2 (('mkstemp',))
-                             6 IMPORT_NAME              0 (tempfile)
-                             8 IMPORT_FROM              1 (mkstemp)
-                            10 STORE_FAST               5 (mkstemp)
-                            12 POP_TOP
-               
-               984          14 LOAD_CONST               1 (0)
-                            16 LOAD_CONST               3 (('SvgImage',))
-                            18 IMPORT_NAME              2 (tksvg)
-                            20 IMPORT_FROM              3 (SvgImage)
-                            22 STORE_FAST               6 (SvgImage)
-                            24 POP_TOP
-               
-               986          26 PUSH_NULL
-                            28 LOAD_FAST                5 (mkstemp)
-                            30 LOAD_CONST               4 ('.svg')
-                            32 KW_NAMES                 5
-                            34 PRECALL                  1
-                            38 CALL                     1
-                            48 UNPACK_SEQUENCE          2
-                            52 STORE_FAST               7 (_)
-                            54 STORE_FAST               8 (file)
-               
-               987          56 LOAD_GLOBAL              9 (NULL + print)
-                            68 LOAD_FAST                8 (file)
-                            70 PRECALL                  1
-                            74 CALL                     1
-                            84 POP_TOP
-               
-               988          86 LOAD_GLOBAL             11 (NULL + open)
-                            98 LOAD_FAST                8 (file)
-                           100 LOAD_CONST               6 ('w')
-                           102 PRECALL                  2
-                           106 CALL                     2
-                           116 BEFORE_WITH
-                           118 STORE_FAST               9 (f)
-               
-               989         120 LOAD_FAST                9 (f)
-                           122 LOAD_METHOD              6 (write)
-                           144 LOAD_FAST                3 (content)
-                           146 PRECALL                  1
-                           150 CALL                     1
-                           160 POP_TOP
+               1052           2 LOAD_CONST               1 (0)
+                              4 LOAD_CONST               2 (('mkstemp',))
+                              6 IMPORT_NAME              0 (tempfile)
+                              8 IMPORT_FROM              1 (mkstemp)
+                             10 STORE_FAST               5 (mkstemp)
+                             12 POP_TOP
                
-               990         162 LOAD_FAST                9 (f)
-                           164 LOAD_METHOD              7 (close)
-                           186 PRECALL                  0
-                           190 CALL                     0
-                           200 POP_TOP
-               
-               988         202 LOAD_CONST               0 (None)
-                           204 LOAD_CONST               0 (None)
-                           206 LOAD_CONST               0 (None)
-                           208 PRECALL                  2
-                           212 CALL                     2
-                           222 POP_TOP
-                           224 JUMP_FORWARD            11 (to 248)
-                       >>  226 PUSH_EXC_INFO
-                           228 WITH_EXCEPT_START
-                           230 POP_JUMP_FORWARD_IF_TRUE     4 (to 240)
-                           232 RERAISE                  2
-                       >>  234 COPY                     3
-                           236 POP_EXCEPT
-                           238 RERAISE                  1
-                       >>  240 POP_TOP
-                           242 POP_EXCEPT
-                           244 POP_TOP
-                           246 POP_TOP
-               
-               991     >>  248 PUSH_NULL
-                           250 LOAD_FAST                6 (SvgImage)
-                           252 LOAD_FAST                8 (file)
-                           254 KW_NAMES                 7
-                           256 PRECALL                  1
-                           260 CALL                     1
-                           270 STORE_FAST              10 (image)
-               
-               993         272 PUSH_NULL
-                           274 LOAD_FAST                0 (self)
-                           276 LOAD_ATTR                8 (create_image)
-                           286 LOAD_FAST                1 (x)
-                           288 LOAD_FAST                2 (y)
-                           290 BUILD_TUPLE              2
-                           292 LOAD_CONST               8 ('image')
-                           294 LOAD_FAST               10 (image)
-                           296 BUILD_MAP                1
-                           298 LOAD_FAST                4 (kwargs)
-                           300 DICT_MERGE               1
-                           302 CALL_FUNCTION_EX         1
-                           304 STORE_FAST              11 (i)
+               1053          14 LOAD_CONST               1 (0)
+                             16 LOAD_CONST               3 (('SvgImage',))
+                             18 IMPORT_NAME              2 (tksvg)
+                             20 IMPORT_FROM              3 (SvgImage)
+                             22 STORE_FAST               6 (SvgImage)
+                             24 POP_TOP
+               
+               1055          26 PUSH_NULL
+                             28 LOAD_FAST                5 (mkstemp)
+                             30 LOAD_CONST               4 ('.svg')
+                             32 KW_NAMES                 5
+                             34 PRECALL                  1
+                             38 CALL                     1
+                             48 UNPACK_SEQUENCE          2
+                             52 STORE_FAST               7 (_)
+                             54 STORE_FAST               8 (file)
+               
+               1056          56 LOAD_GLOBAL              9 (NULL + print)
+                             68 LOAD_FAST                8 (file)
+                             70 PRECALL                  1
+                             74 CALL                     1
+                             84 POP_TOP
+               
+               1057          86 LOAD_GLOBAL             11 (NULL + open)
+                             98 LOAD_FAST                8 (file)
+                            100 LOAD_CONST               6 ('w')
+                            102 PRECALL                  2
+                            106 CALL                     2
+                            116 BEFORE_WITH
+                            118 STORE_FAST               9 (f)
+               
+               1058         120 LOAD_FAST                9 (f)
+                            122 LOAD_METHOD              6 (write)
+                            144 LOAD_FAST                3 (content)
+                            146 PRECALL                  1
+                            150 CALL                     1
+                            160 POP_TOP
+               
+               1059         162 LOAD_FAST                9 (f)
+                            164 LOAD_METHOD              7 (close)
+                            186 PRECALL                  0
+                            190 CALL                     0
+                            200 POP_TOP
+               
+               1057         202 LOAD_CONST               0 (None)
+                            204 LOAD_CONST               0 (None)
+                            206 LOAD_CONST               0 (None)
+                            208 PRECALL                  2
+                            212 CALL                     2
+                            222 POP_TOP
+                            224 JUMP_FORWARD            11 (to 248)
+                        >>  226 PUSH_EXC_INFO
+                            228 WITH_EXCEPT_START
+                            230 POP_JUMP_FORWARD_IF_TRUE     4 (to 240)
+                            232 RERAISE                  2
+                        >>  234 COPY                     3
+                            236 POP_EXCEPT
+                            238 RERAISE                  1
+                        >>  240 POP_TOP
+                            242 POP_EXCEPT
+                            244 POP_TOP
+                            246 POP_TOP
+               
+               1060     >>  248 PUSH_NULL
+                            250 LOAD_FAST                6 (SvgImage)
+                            252 LOAD_FAST                8 (file)
+                            254 KW_NAMES                 7
+                            256 PRECALL                  1
+                            260 CALL                     1
+                            270 STORE_FAST              10 (image)
+               
+               1062         272 PUSH_NULL
+                            274 LOAD_FAST                0 (self)
+                            276 LOAD_ATTR                8 (create_image)
+                            286 LOAD_FAST                1 (x)
+                            288 LOAD_FAST                2 (y)
+                            290 BUILD_TUPLE              2
+                            292 LOAD_CONST               8 ('image')
+                            294 LOAD_FAST               10 (image)
+                            296 BUILD_MAP                1
+                            298 LOAD_FAST                4 (kwargs)
+                            300 DICT_MERGE               1
+                            302 CALL_FUNCTION_EX         1
+                            304 STORE_FAST              11 (i)
                
-               995         306 LOAD_FAST               11 (i)
-                           308 RETURN_VALUE
+               1064         306 LOAD_FAST               11 (i)
+                            308 RETURN_VALUE
                ExceptionTable:
                  118 to 200 -> 226 [1] lasti
                  226 to 232 -> 234 [3] lasti
                  240 to 240 -> 234 [3] lasti
                consts
                   None
                   0
@@ -2143,15 +2149,15 @@
                   'image'
                names      ('tempfile', 'mkstemp', 'tksvg', 'SvgImage', 'print', 'open', 'write', 'close', 'create_image')
                varnames   ('self', 'x', 'y', 'content', 'kwargs', 'mkstemp', 'SvgImage', '_', 'file', 'f', 'image', 'i')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'create_svg_image'
-               firstlineno 982
+               firstlineno 1051
                lnotab 0x02010c010c021e011e0122012a0128fe2e0318022202
             10
             18
             code
                argcount  : 6
                nlocals   : 10
                stacksize : 8
@@ -2168,17 +2174,17 @@
                   0364057a0500007a0000007c027c0364057a0500007a0000007c05a60500
                   00ab0500000000000000007d087c00a00000000000000000000000000000
                   000000000000007c017c0364027a0500007a0000007c047a0000007c027c
                   0364027a0500007a0000007c047a0000007c017c0364057a0500007a0000
                   007c047a0a00007c027c0364057a0500007a0000007c047a0a00007c0564
                   027a0b00006403ac04a6060000ab0600000000000000007d097c067c077c
                   087c0966045300
-                997           0 RESUME                   0
+               1066           0 RESUME                   0
                
-                998           2 LOAD_FAST                0 (self)
+               1067           2 LOAD_FAST                0 (self)
                               4 LOAD_METHOD              0 (create_round_rect4)
                              26 LOAD_FAST                1 (_AdwDrawEngine__x)
                              28 LOAD_FAST                2 (_AdwDrawEngine__y)
                              30 LOAD_FAST                1 (_AdwDrawEngine__x)
                              32 LOAD_FAST                3 (size)
                              34 LOAD_CONST               1 (5)
                              36 BINARY_OP                5 (*)
@@ -2189,15 +2195,15 @@
                              50 BINARY_OP                5 (*)
                              54 BINARY_OP                0 (+)
                              58 LOAD_FAST                5 (radius)
                              60 PRECALL                  5
                              64 CALL                     5
                              74 STORE_FAST               6 (_1)
                
-                999          76 LOAD_FAST                0 (self)
+               1068          76 LOAD_FAST                0 (self)
                              78 LOAD_METHOD              0 (create_round_rect4)
                             100 LOAD_FAST                1 (_AdwDrawEngine__x)
                             102 LOAD_FAST                4 (padding)
                             104 BINARY_OP                0 (+)
                             108 LOAD_FAST                2 (_AdwDrawEngine__y)
                             110 LOAD_FAST                4 (padding)
                             112 BINARY_OP                0 (+)
@@ -2212,25 +2218,25 @@
                             138 LOAD_FAST                3 (size)
                             140 LOAD_CONST               1 (5)
                             142 BINARY_OP                5 (*)
                             146 BINARY_OP                0 (+)
                             150 LOAD_FAST                4 (padding)
                             152 BINARY_OP               10 (-)
                
-               1000         156 LOAD_FAST                5 (radius)
+               1069         156 LOAD_FAST                5 (radius)
                             158 LOAD_CONST               2 (2)
                             160 BINARY_OP               11 (/)
                             164 LOAD_CONST               3 ('white')
                
-                999         166 KW_NAMES                 4
+               1068         166 KW_NAMES                 4
                             168 PRECALL                  6
                             172 CALL                     6
                             182 STORE_FAST               7 (_2)
                
-               1001         184 LOAD_FAST                0 (self)
+               1070         184 LOAD_FAST                0 (self)
                             186 LOAD_METHOD              0 (create_round_rect4)
                             208 LOAD_FAST                1 (_AdwDrawEngine__x)
                             210 LOAD_FAST                3 (size)
                             212 LOAD_CONST               2 (2)
                             214 BINARY_OP                5 (*)
                             218 BINARY_OP                0 (+)
                             222 LOAD_FAST                2 (_AdwDrawEngine__y)
@@ -2249,15 +2255,15 @@
                             256 BINARY_OP                5 (*)
                             260 BINARY_OP                0 (+)
                             264 LOAD_FAST                5 (radius)
                             266 PRECALL                  5
                             270 CALL                     5
                             280 STORE_FAST               8 (_3)
                
-               1002         282 LOAD_FAST                0 (self)
+               1071         282 LOAD_FAST                0 (self)
                             284 LOAD_METHOD              0 (create_round_rect4)
                             306 LOAD_FAST                1 (_AdwDrawEngine__x)
                             308 LOAD_FAST                3 (size)
                             310 LOAD_CONST               2 (2)
                             312 BINARY_OP                5 (*)
                             316 BINARY_OP                0 (+)
                             320 LOAD_FAST                4 (padding)
@@ -2273,32 +2279,32 @@
                             348 LOAD_FAST                3 (size)
                             350 LOAD_CONST               5 (7)
                             352 BINARY_OP                5 (*)
                             356 BINARY_OP                0 (+)
                             360 LOAD_FAST                4 (padding)
                             362 BINARY_OP               10 (-)
                
-               1003         366 LOAD_FAST                2 (_AdwDrawEngine__y)
+               1072         366 LOAD_FAST                2 (_AdwDrawEngine__y)
                             368 LOAD_FAST                3 (size)
                             370 LOAD_CONST               5 (7)
                             372 BINARY_OP                5 (*)
                             376 BINARY_OP                0 (+)
                             380 LOAD_FAST                4 (padding)
                             382 BINARY_OP               10 (-)
                             386 LOAD_FAST                5 (radius)
                             388 LOAD_CONST               2 (2)
                             390 BINARY_OP               11 (/)
                             394 LOAD_CONST               3 ('white')
                
-               1002         396 KW_NAMES                 4
+               1071         396 KW_NAMES                 4
                             398 PRECALL                  6
                             402 CALL                     6
                             412 STORE_FAST               9 (_4)
                
-               1004         414 LOAD_FAST                6 (_1)
+               1073         414 LOAD_FAST                6 (_1)
                             416 LOAD_FAST                7 (_2)
                             418 LOAD_FAST                8 (_3)
                             420 LOAD_FAST                9 (_4)
                             422 BUILD_TUPLE              4
                             424 RETURN_VALUE
                consts
                   None
@@ -2309,38 +2315,38 @@
                   7
                names      ('create_round_rect4',)
                varnames   ('self', '_AdwDrawEngine__x', '_AdwDrawEngine__y', 'size', 'padding', 'radius', '_1', '_2', '_3', '_4')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'draw_copy_icon'
-               firstlineno 997
+               firstlineno 1066
                lnotab 0x02014a0150010aff1202620154011eff1202
             16
             code
                argcount  : 7
                nlocals   : 12
                stacksize : 6
                flags     : 15
                code
                   0x9700640164026c006d017d0901007405000000000000000000007c037c
                   0466027c067c0567037c07a201520069007c08a4018e017d0a7c09a00300
                   000000000000000000000000000000000000007c0aa6010000ab01000000
                   00000000007d0b7c00a00400000000000000000000000000000000000000
                   007c017c027c0b6403ac04a6040000ab0400000000000000005300
-               1006           0 RESUME                   0
+               1075           0 RESUME                   0
                
-               1007           2 LOAD_CONST               1 (0)
+               1076           2 LOAD_CONST               1 (0)
                               4 LOAD_CONST               2 (('ImageTk',))
                               6 IMPORT_NAME              0 (PIL)
                               8 IMPORT_FROM              1 (ImageTk)
                              10 STORE_FAST               9 (ImageTk)
                              12 POP_TOP
                
-               1008          14 LOAD_GLOBAL              5 (NULL + rounded_rectangle)
+               1077          14 LOAD_GLOBAL              5 (NULL + rounded_rectangle)
                              26 LOAD_FAST                3 (_AdwDrawEngine__width)
                              28 LOAD_FAST                4 (_AdwDrawEngine__height)
                              30 BUILD_TUPLE              2
                              32 LOAD_FAST                6 (radius)
                              34 LOAD_FAST                5 (fill)
                              36 BUILD_LIST               3
                              38 LOAD_FAST                7 (args)
@@ -2348,22 +2354,22 @@
                              42 LIST_TO_TUPLE
                              44 BUILD_MAP                0
                              46 LOAD_FAST                8 (kwargs)
                              48 DICT_MERGE               1
                              50 CALL_FUNCTION_EX         1
                              52 STORE_FAST              10 (img)
                
-               1009          54 LOAD_FAST                9 (ImageTk)
+               1078          54 LOAD_FAST                9 (ImageTk)
                              56 LOAD_METHOD              3 (PhotoImage)
                              78 LOAD_FAST               10 (img)
                              80 PRECALL                  1
                              84 CALL                     1
                              94 STORE_FAST              11 (photo)
                
-               1011          96 LOAD_FAST                0 (self)
+               1080          96 LOAD_FAST                0 (self)
                              98 LOAD_METHOD              4 (create_image)
                             120 LOAD_FAST                1 (_AdwDrawEngine__x)
                             122 LOAD_FAST                2 (_AdwDrawEngine__y)
                             124 LOAD_FAST               11 (photo)
                             126 LOAD_CONST               3 ('nw')
                             128 KW_NAMES                 4
                             130 PRECALL                  4
@@ -2377,15 +2383,15 @@
                   ('image', 'anchor')
                names      ('PIL', 'ImageTk', 'rounded_rectangle', 'PhotoImage', 'create_image')
                varnames   ('self', '_AdwDrawEngine__x', '_AdwDrawEngine__y', '_AdwDrawEngine__width', '_AdwDrawEngine__height', 'fill', 'radius', 'args', 'kwargs', 'ImageTk', 'img', 'photo')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
                name       'create_round_rectangle5'
-               firstlineno 1006
+               firstlineno 1075
                lnotab 0x02010c0128012a02
             (26,)
             ('x',)
             (5, 2, 'white', 'black')
             ('black', 'black')
             (10, 10, 18)
             ('black', 16)
@@ -2393,16 +2399,16 @@
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
          name       'AdwDrawEngine'
          firstlineno 241
          lnotab
-            0x0c010a03060406030c06080b067f007f005806041c0414041c07060306
-            040604060408430e2204020644040212120402061a040208060402066c0c
+            0x0c010a03060706030c06080b067f007f005b06071c0714071c0a060606
+            100610061008430e2504020647040212150402061d040208060402066c0c
             0f0809
       'AdwDrawEngine'
       '__main__'
       ('Tk',)
       123
       5
       100
@@ -2420,8 +2426,8 @@
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\windows\\canvas\\drawengine.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c030608047f0015044a040104010401040104031c7f007f00
-      7f007f007f007f000b0c010c02140214063e022e022cf1
+      7f007f007f007f00500c010c02140214063e022e022cf1
```

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/entry.cpython-310.pyc` & `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/entry.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/entry.cpython-311.pyc` & `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/frame.cpython-310.pyc` & `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/frame.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/frame.cpython-311.pyc` & `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/frame.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x30c9a464 (Wed Jul  5 01:36:48 2023 UTC)
-files sz: 6460
+moddate:  0xf956b364 (Sun Jul 16 02:33:29 2023 UTC)
+files sz: 7018
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100020047
@@ -57,224 +57,224 @@
                 32 MAKE_FUNCTION            0
                 34 LOAD_CONST               4 ('AdwDrawBasicFrame')
                 36 LOAD_NAME                1 (AdwWidget)
                 38 PRECALL                  3
                 42 CALL                     3
                 52 STORE_NAME               4 (AdwDrawBasicFrame)
    
-    78          54 PUSH_NULL
+    81          54 PUSH_NULL
                 56 LOAD_BUILD_CLASS
-                58 LOAD_CONST               5 (<code object AdwDrawFrame, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 78>)
+                58 LOAD_CONST               5 (<code object AdwDrawFrame, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 81>)
                 60 MAKE_FUNCTION            0
                 62 LOAD_CONST               6 ('AdwDrawFrame')
                 64 LOAD_NAME                4 (AdwDrawBasicFrame)
                 66 PRECALL                  3
                 70 CALL                     3
                 80 STORE_NAME               5 (AdwDrawFrame)
    
-    83          82 PUSH_NULL
+    86          82 PUSH_NULL
                 84 LOAD_BUILD_CLASS
-                86 LOAD_CONST               7 (<code object AdwDrawDarkFrame, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 83>)
+                86 LOAD_CONST               7 (<code object AdwDrawDarkFrame, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 86>)
                 88 MAKE_FUNCTION            0
                 90 LOAD_CONST               8 ('AdwDrawDarkFrame')
                 92 LOAD_NAME                4 (AdwDrawBasicFrame)
                 94 PRECALL                  3
                 98 CALL                     3
                108 STORE_NAME               6 (AdwDrawDarkFrame)
    
-    88         110 PUSH_NULL
+    91         110 PUSH_NULL
                112 LOAD_BUILD_CLASS
-               114 LOAD_CONST               9 (<code object AdwDrawBasicRoundFrame, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 88>)
+               114 LOAD_CONST               9 (<code object AdwDrawBasicRoundFrame, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 91>)
                116 MAKE_FUNCTION            0
                118 LOAD_CONST              10 ('AdwDrawBasicRoundFrame')
                120 LOAD_NAME                4 (AdwDrawBasicFrame)
                122 PRECALL                  3
                126 CALL                     3
                136 STORE_NAME               7 (AdwDrawBasicRoundFrame)
    
-   149         138 PUSH_NULL
+   156         138 PUSH_NULL
                140 LOAD_BUILD_CLASS
-               142 LOAD_CONST              11 (<code object AdwDrawRoundFrame, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 149>)
+               142 LOAD_CONST              11 (<code object AdwDrawRoundFrame, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 156>)
                144 MAKE_FUNCTION            0
                146 LOAD_CONST              12 ('AdwDrawRoundFrame')
                148 LOAD_NAME                7 (AdwDrawBasicRoundFrame)
                150 PRECALL                  3
                154 CALL                     3
                164 STORE_NAME               8 (AdwDrawRoundFrame)
    
-   154         166 PUSH_NULL
+   161         166 PUSH_NULL
                168 LOAD_BUILD_CLASS
-               170 LOAD_CONST              13 (<code object AdwDrawDarkRoundFrame, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 154>)
+               170 LOAD_CONST              13 (<code object AdwDrawDarkRoundFrame, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 161>)
                172 MAKE_FUNCTION            0
                174 LOAD_CONST              14 ('AdwDrawDarkRoundFrame')
                176 LOAD_NAME                7 (AdwDrawBasicRoundFrame)
                178 PRECALL                  3
                182 CALL                     3
                192 STORE_NAME               9 (AdwDrawDarkRoundFrame)
    
-   159         194 PUSH_NULL
+   166         194 PUSH_NULL
                196 LOAD_BUILD_CLASS
-               198 LOAD_CONST              15 (<code object AdwDrawBasicRoundFrame3, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 159>)
+               198 LOAD_CONST              15 (<code object AdwDrawBasicRoundFrame3, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 166>)
                200 MAKE_FUNCTION            0
                202 LOAD_CONST              16 ('AdwDrawBasicRoundFrame3')
                204 LOAD_NAME                7 (AdwDrawBasicRoundFrame)
                206 PRECALL                  3
                210 CALL                     3
                220 STORE_NAME              10 (AdwDrawBasicRoundFrame3)
    
-   195         222 PUSH_NULL
+   204         222 PUSH_NULL
                224 LOAD_BUILD_CLASS
-               226 LOAD_CONST              17 (<code object AdwDrawRoundFrame3, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 195>)
+               226 LOAD_CONST              17 (<code object AdwDrawRoundFrame3, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 204>)
                228 MAKE_FUNCTION            0
                230 LOAD_CONST              18 ('AdwDrawRoundFrame3')
                232 LOAD_NAME               10 (AdwDrawBasicRoundFrame3)
                234 PRECALL                  3
                238 CALL                     3
                248 STORE_NAME              11 (AdwDrawRoundFrame3)
    
-   200         250 PUSH_NULL
+   209         250 PUSH_NULL
                252 LOAD_BUILD_CLASS
-               254 LOAD_CONST              19 (<code object AdwDrawDarkRoundFrame3, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 200>)
+               254 LOAD_CONST              19 (<code object AdwDrawDarkRoundFrame3, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 209>)
                256 MAKE_FUNCTION            0
                258 LOAD_CONST              20 ('AdwDrawDarkRoundFrame3')
                260 LOAD_NAME               10 (AdwDrawBasicRoundFrame3)
                262 PRECALL                  3
                266 CALL                     3
                276 STORE_NAME              12 (AdwDrawDarkRoundFrame3)
    
-   205         278 LOAD_NAME               13 (__name__)
+   214         278 LOAD_NAME               13 (__name__)
                280 LOAD_CONST              21 ('__main__')
                282 COMPARE_OP               2 (==)
                288 EXTENDED_ARG             1
                290 POP_JUMP_FORWARD_IF_FALSE   260 (to 812)
    
-   206         292 LOAD_CONST               0 (0)
+   215         292 LOAD_CONST               0 (0)
                294 LOAD_CONST              22 (('Tk',))
                296 IMPORT_NAME              2 (tkinter)
                298 IMPORT_FROM             14 (Tk)
                300 STORE_NAME              14 (Tk)
                302 POP_TOP
    
-   208         304 PUSH_NULL
+   217         304 PUSH_NULL
                306 LOAD_NAME               14 (Tk)
                308 PRECALL                  0
                312 CALL                     0
                322 STORE_NAME              15 (root)
    
-   210         324 PUSH_NULL
+   219         324 PUSH_NULL
                326 LOAD_NAME                6 (AdwDrawDarkFrame)
                328 PRECALL                  0
                332 CALL                     0
                342 STORE_NAME              16 (frame)
    
-   211         344 LOAD_NAME               16 (frame)
+   220         344 LOAD_NAME               16 (frame)
                346 LOAD_METHOD             17 (pack)
                368 LOAD_CONST              23 ('both')
                370 LOAD_CONST              24 ('yes')
                372 KW_NAMES                25
                374 PRECALL                  2
                378 CALL                     2
                388 POP_TOP
    
-   213         390 PUSH_NULL
+   222         390 PUSH_NULL
                392 LOAD_NAME                6 (AdwDrawDarkFrame)
                394 LOAD_NAME               16 (frame)
                396 LOAD_ATTR               16 (frame)
                406 PRECALL                  1
                410 CALL                     1
                420 STORE_NAME              18 (frame2)
    
-   214         422 LOAD_NAME               18 (frame2)
+   223         422 LOAD_NAME               18 (frame2)
                424 LOAD_METHOD             17 (pack)
                446 LOAD_CONST              23 ('both')
                448 LOAD_CONST              24 ('yes')
                450 LOAD_CONST              26 (8)
                452 LOAD_CONST              26 (8)
                454 KW_NAMES                27
                456 PRECALL                  4
                460 CALL                     4
                470 POP_TOP
    
-   216         472 PUSH_NULL
+   225         472 PUSH_NULL
                474 LOAD_NAME                9 (AdwDrawDarkRoundFrame)
                476 PRECALL                  0
                480 CALL                     0
                490 STORE_NAME              19 (frame3)
    
-   217         492 LOAD_NAME               19 (frame3)
+   226         492 LOAD_NAME               19 (frame3)
                494 LOAD_METHOD             17 (pack)
                516 LOAD_CONST              23 ('both')
                518 LOAD_CONST              24 ('yes')
                520 KW_NAMES                25
                522 PRECALL                  2
                526 CALL                     2
                536 POP_TOP
    
-   219         538 PUSH_NULL
+   228         538 PUSH_NULL
                540 LOAD_NAME                9 (AdwDrawDarkRoundFrame)
                542 LOAD_NAME               19 (frame3)
                544 LOAD_ATTR               16 (frame)
                554 PRECALL                  1
                558 CALL                     1
                568 STORE_NAME              20 (frame4)
    
-   220         570 LOAD_NAME               20 (frame4)
+   229         570 LOAD_NAME               20 (frame4)
                572 LOAD_METHOD             17 (pack)
                594 LOAD_CONST              23 ('both')
                596 LOAD_CONST              24 ('yes')
                598 LOAD_CONST              26 (8)
                600 LOAD_CONST              26 (8)
                602 KW_NAMES                27
                604 PRECALL                  4
                608 CALL                     4
                618 POP_TOP
    
-   222         620 PUSH_NULL
+   231         620 PUSH_NULL
                622 LOAD_NAME               12 (AdwDrawDarkRoundFrame3)
                624 PRECALL                  0
                628 CALL                     0
                638 STORE_NAME              21 (frame5)
    
-   223         640 LOAD_NAME               21 (frame5)
+   232         640 LOAD_NAME               21 (frame5)
                642 LOAD_METHOD             17 (pack)
                664 LOAD_CONST              23 ('both')
                666 LOAD_CONST              24 ('yes')
                668 KW_NAMES                25
                670 PRECALL                  2
                674 CALL                     2
                684 POP_TOP
    
-   225         686 PUSH_NULL
+   234         686 PUSH_NULL
                688 LOAD_NAME               12 (AdwDrawDarkRoundFrame3)
                690 LOAD_NAME               21 (frame5)
                692 LOAD_ATTR               16 (frame)
                702 PRECALL                  1
                706 CALL                     1
                716 STORE_NAME              22 (frame6)
    
-   226         718 LOAD_NAME               22 (frame6)
+   235         718 LOAD_NAME               22 (frame6)
                720 LOAD_METHOD             17 (pack)
                742 LOAD_CONST              23 ('both')
                744 LOAD_CONST              24 ('yes')
                746 LOAD_CONST              26 (8)
                748 LOAD_CONST              26 (8)
                750 KW_NAMES                27
                752 PRECALL                  4
                756 CALL                     4
                766 POP_TOP
    
-   228         768 LOAD_NAME               15 (root)
+   237         768 LOAD_NAME               15 (root)
                770 LOAD_METHOD             23 (mainloop)
                792 PRECALL                  0
                796 CALL                     0
                806 POP_TOP
                808 LOAD_CONST              28 (None)
                810 RETURN_VALUE
    
-   205     >>  812 LOAD_CONST              28 (None)
+   214     >>  812 LOAD_CONST              28 (None)
                814 RETURN_VALUE
    consts
       0
       ('AdwWidget',)
       ('Frame',)
       code
          argcount  : 0
@@ -311,20 +311,20 @@
                       38 MAKE_FUNCTION            0
                       40 STORE_NAME               5 (default_palette)
          
           39          42 LOAD_CONST               6 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 39>)
                       44 MAKE_FUNCTION            0
                       46 STORE_NAME               6 (palette_light)
          
-          50          48 LOAD_CONST               7 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 50>)
+          51          48 LOAD_CONST               7 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 51>)
                       50 MAKE_FUNCTION            0
                       52 STORE_NAME               7 (palette_dark)
          
-          61          54 LOAD_CONST              10 ((None,))
-                      56 LOAD_CONST               9 (<code object palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 61>)
+          63          54 LOAD_CONST              10 ((None,))
+                      56 LOAD_CONST               9 (<code object palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 63>)
                       58 MAKE_FUNCTION            1 (defaults)
                       60 STORE_NAME               8 (palette)
                       62 LOAD_CLOSURE             0 (__class__)
                       64 COPY                     1
                       66 STORE_NAME               9 (__classcell__)
                       68 RETURN_VALUE
          consts
@@ -415,18 +415,19 @@
                   000000000000007c006a0600000000000000006402ac04a6020000ab0200
                   0000000000000001007c00a00a0000000000000000000000000000000000
                   0000007c00a0020000000000000000000000000000000000000000a60000
                   00ab00000000000000000064057a0b00007c00a003000000000000000000
                   0000000000000000000000a6000000ab00000000000000000064057a0b00
                   007c006a0800000000000000007c00a00200000000000000000000000000
                   00000000000000a6000000ab00000000000000000064067a0a00007c006a
-                  0400000000000000007a0a00007c00a00300000000000000000000000000
-                  00000000000000a6000000ab00000000000000000064067a0a00007c006a
-                  0400000000000000007a0a0000ac07a6050000ab0500000000000000007c
-                  005f0b000000000000000064005300
+                  0400000000000000007a0a00007c006a0b00000000000000007a0a00007c
+                  00a0030000000000000000000000000000000000000000a6000000ab0000
+                  0000000000000064067a0a00007c006a0400000000000000007a0a00007c
+                  006a0b00000000000000007a0a0000ac07a6050000ab0500000000000000
+                  007c005f0c000000000000000064005300
                 16           0 RESUME                   0
                
                 17           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
@@ -495,49 +496,55 @@
                            426 PRECALL                  0
                            430 CALL                     0
                            440 LOAD_CONST               6 (6)
                            442 BINARY_OP               10 (-)
                            446 LOAD_FAST                0 (self)
                            448 LOAD_ATTR                4 (frame_border_width)
                            458 BINARY_OP               10 (-)
+                           462 LOAD_FAST                0 (self)
+                           464 LOAD_ATTR               11 (frame_padding)
+                           474 BINARY_OP               10 (-)
                
-                33         462 LOAD_FAST                0 (self)
-                           464 LOAD_METHOD              3 (winfo_height)
-                           486 PRECALL                  0
-                           490 CALL                     0
-                           500 LOAD_CONST               6 (6)
-                           502 BINARY_OP               10 (-)
-                           506 LOAD_FAST                0 (self)
-                           508 LOAD_ATTR                4 (frame_border_width)
+                33         478 LOAD_FAST                0 (self)
+                           480 LOAD_METHOD              3 (winfo_height)
+                           502 PRECALL                  0
+                           506 CALL                     0
+                           516 LOAD_CONST               6 (6)
                            518 BINARY_OP               10 (-)
-               
-                29         522 KW_NAMES                 7
-                           524 PRECALL                  5
-                           528 CALL                     5
+                           522 LOAD_FAST                0 (self)
+                           524 LOAD_ATTR                4 (frame_border_width)
+                           534 BINARY_OP               10 (-)
                            538 LOAD_FAST                0 (self)
-                           540 STORE_ATTR              11 (frame_f)
-                           550 LOAD_CONST               0 (None)
-                           552 RETURN_VALUE
+                           540 LOAD_ATTR               11 (frame_padding)
+                           550 BINARY_OP               10 (-)
+               
+                29         554 KW_NAMES                 7
+                           556 PRECALL                  5
+                           560 CALL                     5
+                           570 LOAD_FAST                0 (self)
+                           572 STORE_ATTR              12 (frame_f)
+                           582 LOAD_CONST               0 (None)
+                           584 RETURN_VALUE
                consts
                   None
                   'all'
                   0
                   ('width', 'outline', 'fill')
                   ('background', 'bd')
                   2
                   6
                   ('window', 'width', 'height')
-               names      ('delete', 'create_rectangle', 'winfo_width', 'winfo_height', 'frame_border_width', 'frame_border', 'frame_back', 'frame_frame', 'frame', 'configure', 'create_window', 'frame_f')
+               names      ('delete', 'create_rectangle', 'winfo_width', 'winfo_height', 'frame_border_width', 'frame_border', 'frame_back', 'frame_frame', 'frame', 'configure', 'create_window', 'frame_padding', 'frame_f')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       '_draw'
                firstlineno 16
-               lnotab 0x02012a03180150010c0118fd1c064203180158010c013c013cfc
+               lnotab 0x02012a03180150010c0118fd1c064203180158010c014c014cfc
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
@@ -560,370 +567,387 @@
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       'default_palette'
                firstlineno 36
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 7
+               stacksize : 8
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  026403640464059c036901a6010000ab0100000000000000000100640053
-                  00
+                  0264036404640564069c046901a6010000ab010000000000000000010064
+                  005300
                 39           0 RESUME                   0
                
                 40           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
                 42          26 LOAD_CONST               1 ('frame')
                
                 43          28 LOAD_CONST               2 ('#ffffff')
                
                 44          30 LOAD_CONST               3 ('#eaeaea')
                
                 45          32 LOAD_CONST               4 (2)
                
-                42          34 LOAD_CONST               5 (('back', 'border', 'border_width'))
-                            36 BUILD_CONST_KEY_MAP      3
+                46          34 LOAD_CONST               5 (0)
+               
+                42          36 LOAD_CONST               6 (('back', 'border', 'border_width', 'padding'))
+                            38 BUILD_CONST_KEY_MAP      4
                
-                41          38 BUILD_MAP                1
+                41          40 BUILD_MAP                1
                
-                40          40 PRECALL                  1
-                            44 CALL                     1
-                            54 POP_TOP
-                            56 LOAD_CONST               0 (None)
-                            58 RETURN_VALUE
+                40          42 PRECALL                  1
+                            46 CALL                     1
+                            56 POP_TOP
+                            58 LOAD_CONST               0 (None)
+                            60 RETURN_VALUE
                consts
                   None
                   'frame'
                   '#ffffff'
                   '#eaeaea'
                   2
-                  ('back', 'border', 'border_width')
+                  0
+                  ('back', 'border', 'border_width', 'padding')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       'palette_light'
                firstlineno 39
-               lnotab 0x0201180202010201020102fd04ff02ff
+               lnotab 0x02011802020102010201020102fc04ff02ff
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 7
+               stacksize : 8
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  026403640464059c036901a6010000ab0100000000000000000100640053
-                  00
-                50           0 RESUME                   0
+                  0264036404640564069c046901a6010000ab010000000000000000010064
+                  005300
+                51           0 RESUME                   0
                
-                51           2 LOAD_FAST                0 (self)
+                52           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-                53          26 LOAD_CONST               1 ('frame')
+                54          26 LOAD_CONST               1 ('frame')
+               
+                55          28 LOAD_CONST               2 ('#0f0f0f')
                
-                54          28 LOAD_CONST               2 ('#0f0f0f')
+                56          30 LOAD_CONST               3 ('#333333')
                
-                55          30 LOAD_CONST               3 ('#333333')
+                57          32 LOAD_CONST               4 (2)
                
-                56          32 LOAD_CONST               4 (2)
+                58          34 LOAD_CONST               5 (0)
                
-                53          34 LOAD_CONST               5 (('back', 'border', 'border_width'))
-                            36 BUILD_CONST_KEY_MAP      3
+                54          36 LOAD_CONST               6 (('back', 'border', 'border_width', 'padding'))
+                            38 BUILD_CONST_KEY_MAP      4
                
-                52          38 BUILD_MAP                1
+                53          40 BUILD_MAP                1
                
-                51          40 PRECALL                  1
-                            44 CALL                     1
-                            54 POP_TOP
-                            56 LOAD_CONST               0 (None)
-                            58 RETURN_VALUE
+                52          42 PRECALL                  1
+                            46 CALL                     1
+                            56 POP_TOP
+                            58 LOAD_CONST               0 (None)
+                            60 RETURN_VALUE
                consts
                   None
                   'frame'
                   '#0f0f0f'
                   '#333333'
                   2
-                  ('back', 'border', 'border_width')
+                  0
+                  ('back', 'border', 'border_width', 'padding')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       'palette_dark'
-               firstlineno 50
-               lnotab 0x0201180202010201020102fd04ff02ff
+               firstlineno 51
+               lnotab 0x02011802020102010201020102fc04ff02ff
             None
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
-                  0x97007c01816d64017c01760072397c0164011900000000000000000064
+                  0x97007c01818064017c017600724c7c0164011900000000000000000064
                   02190000000000000000007c005f0000000000000000007c016401190000
                   000000000000006403190000000000000000007c005f0100000000000000
                   007c016401190000000000000000006404190000000000000000007c005f
-                  0200000000000000007c017c005f03000000000000000009007c00a00400
-                  000000000000000000000000000000000000006400a6010000ab01000000
-                  00000000000100640053002300740a000000000000000000002400720401
-                  0059006400530077007803590077017c006a0300000000000000005300
-                61           0 RESUME                   0
+                  0200000000000000007c0164011900000000000000000064051900000000
+                  00000000007c005f0300000000000000007c017c005f0400000000000000
+                  0009007c00a00500000000000000000000000000000000000000006400a6
+                  010000ab0100000000000000000100640053002300740c00000000000000
+                  00000024007204010059006400530077007803590077017c006a04000000
+                  00000000005300
+                63           0 RESUME                   0
                
-                62           2 LOAD_FAST                1 (dict)
-                             4 POP_JUMP_FORWARD_IF_NONE   109 (to 224)
+                64           2 LOAD_FAST                1 (dict)
+                             4 POP_JUMP_FORWARD_IF_NONE   128 (to 262)
                
-                63           6 LOAD_CONST               1 ('frame')
+                65           6 LOAD_CONST               1 ('frame')
                              8 LOAD_FAST                1 (dict)
                             10 CONTAINS_OP              0
-                            12 POP_JUMP_FORWARD_IF_FALSE    57 (to 128)
+                            12 POP_JUMP_FORWARD_IF_FALSE    76 (to 166)
                
-                64          14 LOAD_FAST                1 (dict)
+                66          14 LOAD_FAST                1 (dict)
                             16 LOAD_CONST               1 ('frame')
                             18 BINARY_SUBSCR
                             28 LOAD_CONST               2 ('back')
                             30 BINARY_SUBSCR
                             40 LOAD_FAST                0 (self)
                             42 STORE_ATTR               0 (frame_back)
                
-                65          52 LOAD_FAST                1 (dict)
+                67          52 LOAD_FAST                1 (dict)
                             54 LOAD_CONST               1 ('frame')
                             56 BINARY_SUBSCR
                             66 LOAD_CONST               3 ('border')
                             68 BINARY_SUBSCR
                             78 LOAD_FAST                0 (self)
                             80 STORE_ATTR               1 (frame_border)
                
-                66          90 LOAD_FAST                1 (dict)
+                68          90 LOAD_FAST                1 (dict)
                             92 LOAD_CONST               1 ('frame')
                             94 BINARY_SUBSCR
                            104 LOAD_CONST               4 ('border_width')
                            106 BINARY_SUBSCR
                            116 LOAD_FAST                0 (self)
                            118 STORE_ATTR               2 (frame_border_width)
                
-                68     >>  128 LOAD_FAST                1 (dict)
-                           130 LOAD_FAST                0 (self)
-                           132 STORE_ATTR               3 (_palette)
-               
-                70         142 NOP
-               
-                71         144 LOAD_FAST                0 (self)
-                           146 LOAD_METHOD              4 (_draw)
-                           168 LOAD_CONST               0 (None)
-                           170 PRECALL                  1
-                           174 CALL                     1
-                           184 POP_TOP
-                           186 LOAD_CONST               0 (None)
-                           188 RETURN_VALUE
-                       >>  190 PUSH_EXC_INFO
-               
-                72         192 LOAD_GLOBAL             10 (AttributeError)
-                           204 CHECK_EXC_MATCH
-                           206 POP_JUMP_FORWARD_IF_FALSE     4 (to 216)
-                           208 POP_TOP
-               
-                73         210 POP_EXCEPT
-                           212 LOAD_CONST               0 (None)
-                           214 RETURN_VALUE
-               
-                72     >>  216 RERAISE                  0
-                       >>  218 COPY                     3
-                           220 POP_EXCEPT
-                           222 RERAISE                  1
-               
-                75     >>  224 LOAD_FAST                0 (self)
-                           226 LOAD_ATTR                3 (_palette)
-                           236 RETURN_VALUE
+                69         128 LOAD_FAST                1 (dict)
+                           130 LOAD_CONST               1 ('frame')
+                           132 BINARY_SUBSCR
+                           142 LOAD_CONST               5 ('padding')
+                           144 BINARY_SUBSCR
+                           154 LOAD_FAST                0 (self)
+                           156 STORE_ATTR               3 (frame_padding)
+               
+                71     >>  166 LOAD_FAST                1 (dict)
+                           168 LOAD_FAST                0 (self)
+                           170 STORE_ATTR               4 (_palette)
+               
+                73         180 NOP
+               
+                74         182 LOAD_FAST                0 (self)
+                           184 LOAD_METHOD              5 (_draw)
+                           206 LOAD_CONST               0 (None)
+                           208 PRECALL                  1
+                           212 CALL                     1
+                           222 POP_TOP
+                           224 LOAD_CONST               0 (None)
+                           226 RETURN_VALUE
+                       >>  228 PUSH_EXC_INFO
+               
+                75         230 LOAD_GLOBAL             12 (AttributeError)
+                           242 CHECK_EXC_MATCH
+                           244 POP_JUMP_FORWARD_IF_FALSE     4 (to 254)
+                           246 POP_TOP
+               
+                76         248 POP_EXCEPT
+                           250 LOAD_CONST               0 (None)
+                           252 RETURN_VALUE
+               
+                75     >>  254 RERAISE                  0
+                       >>  256 COPY                     3
+                           258 POP_EXCEPT
+                           260 RERAISE                  1
+               
+                78     >>  262 LOAD_FAST                0 (self)
+                           264 LOAD_ATTR                4 (_palette)
+                           274 RETURN_VALUE
                ExceptionTable:
-                 144 to 184 -> 190 [0]
-                 190 to 208 -> 218 [1] lasti
-                 216 to 216 -> 218 [1] lasti
+                 182 to 222 -> 228 [0]
+                 228 to 246 -> 256 [1] lasti
+                 254 to 254 -> 256 [1] lasti
                consts
                   None
                   'frame'
                   'back'
                   'border'
                   'border_width'
-               names      ('frame_back', 'frame_border', 'frame_border_width', '_palette', '_draw', 'AttributeError')
+                  'padding'
+               names      ('frame_back', 'frame_border', 'frame_border_width', 'frame_padding', '_palette', '_draw', 'AttributeError')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       'palette'
-               firstlineno 61
-               lnotab 0x0201040108012601260126020e0202013001120106ff0803
+               firstlineno 63
+               lnotab 0x02010401080126012601260126020e0202013001120106ff0803
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', '_draw', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
          name       'AdwDrawBasicFrame'
          firstlineno 6
-         lnotab 0x0c01120906140603060b060b
+         lnotab 0x0c01120906140603060c060c
       'AdwDrawBasicFrame'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          78           0 RESUME                   0
+          81           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawFrame')
                        8 STORE_NAME               2 (__qualname__)
          
-          79          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 79>)
+          82          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 82>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawFrame'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-                79           0 RESUME                   0
+                82           0 RESUME                   0
                
-                80           2 LOAD_FAST                0 (self)
+                83           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       'default_palette'
-               firstlineno 79
+               firstlineno 82
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
          name       'AdwDrawFrame'
-         firstlineno 78
+         firstlineno 81
          lnotab 0x0a01
       'AdwDrawFrame'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          83           0 RESUME                   0
+          86           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawDarkFrame')
                        8 STORE_NAME               2 (__qualname__)
          
-          84          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 84>)
+          87          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 87>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawDarkFrame'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-                84           0 RESUME                   0
+                87           0 RESUME                   0
                
-                85           2 LOAD_FAST                0 (self)
+                88           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       'default_palette'
-               firstlineno 84
+               firstlineno 87
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
          name       'AdwDrawDarkFrame'
-         firstlineno 83
+         firstlineno 86
          lnotab 0x0a01
       'AdwDrawDarkFrame'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
             0384005a05640484005a06640584005a07640888006601640784095a0888
             0078015a095300
                        0 MAKE_CELL                0 (__class__)
          
-          88           2 RESUME                   0
+          91           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundFrame')
                       10 STORE_NAME               2 (__qualname__)
          
-          89          12 LOAD_CLOSURE             0 (__class__)
+          92          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 89>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 92>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-          96          22 LOAD_CONST               2 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 96>)
+          99          22 LOAD_CONST               2 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 99>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_draw)
          
-         116          28 LOAD_CONST               3 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 116>)
+         121          28 LOAD_CONST               3 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 121>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               5 (default_palette)
          
-         119          34 LOAD_CONST               4 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 119>)
+         124          34 LOAD_CONST               4 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 124>)
                       36 MAKE_FUNCTION            0
                       38 STORE_NAME               6 (palette_light)
          
-         131          40 LOAD_CONST               5 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 131>)
+         137          40 LOAD_CONST               5 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 137>)
                       42 MAKE_FUNCTION            0
                       44 STORE_NAME               7 (palette_dark)
          
-         143          46 LOAD_CONST               8 ((None,))
+         150          46 LOAD_CONST               8 ((None,))
                       48 LOAD_CLOSURE             0 (__class__)
                       50 BUILD_TUPLE              1
-                      52 LOAD_CONST               7 (<code object palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 143>)
+                      52 LOAD_CONST               7 (<code object palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 150>)
                       54 MAKE_FUNCTION            9 (defaults, closure)
                       56 STORE_NAME               8 (palette)
                       58 LOAD_CLOSURE             0 (__class__)
                       60 COPY                     1
                       62 STORE_NAME               9 (__classcell__)
                       64 RETURN_VALUE
          consts
@@ -938,31 +962,31 @@
                   0000006a0100000000000000007c0169007c02a4018e01010009007c00a0
                   0200000000000000000000000000000000000000007c006a030000000000
                   000000a00400000000000000000000000000000000000000006401a60100
                   00ab010000000000000000ac02a6010000ab010000000000000000010064
                   00530023000100590064005300780359007701
                              0 COPY_FREE_VARS           1
                
-                89           2 RESUME                   0
+                92           2 RESUME                   0
                
-                90           4 PUSH_NULL
+                93           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
                             48 DICT_MERGE               1
                             50 CALL_FUNCTION_EX         1
                             52 POP_TOP
                
-                91          54 NOP
+                94          54 NOP
                
-                92          56 LOAD_FAST                0 (self)
+                95          56 LOAD_FAST                0 (self)
                             58 LOAD_METHOD              2 (configure)
                             80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                3 (master)
                             92 LOAD_METHOD              4 (cget)
                            114 LOAD_CONST               1 ('background')
                            116 PRECALL                  1
                            120 CALL                     1
@@ -970,17 +994,17 @@
                            132 PRECALL                  1
                            136 CALL                     1
                            146 POP_TOP
                            148 LOAD_CONST               0 (None)
                            150 RETURN_VALUE
                        >>  152 PUSH_EXC_INFO
                
-                93         154 POP_TOP
+                96         154 POP_TOP
                
-                94         156 POP_EXCEPT
+                97         156 POP_EXCEPT
                            158 LOAD_CONST               0 (None)
                            160 RETURN_VALUE
                        >>  162 COPY                     3
                            164 POP_EXCEPT
                            166 RERAISE                  1
                ExceptionTable:
                  56 to 146 -> 152 [0]
@@ -991,484 +1015,511 @@
                   ('background',)
                names      ('super', '__init__', 'configure', 'master', 'cget')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       '__init__'
-               firstlineno 89
+               firstlineno 92
                lnotab 0x04013201020162010201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000006401a6
                   010000ab01000000000000000001007c00a0010000000000000000000000
-                  000000000000000000640264027c00a00200000000000000000000000000
-                  00000000000000a6000000ab0000000000000000007c00a0030000000000
-                  000000000000000000000000000000a6000000ab0000000000000000007c
-                  006a0400000000000000007c006a0500000000000000007c006a06000000
-                  00000000007c006a070000000000000000ac03a6080000ab080000000000
-                  0000007c005f0800000000000000007c006a090000000000000000a00a00
-                  000000000000000000000000000000000000007c006a0700000000000000
-                  006402ac04a6020000ab02000000000000000001007c00a00b0000000000
-                  0000000000000000000000000000007c00a0020000000000000000000000
-                  000000000000000000a6000000ab00000000000000000064057a0b00007c
-                  00a0030000000000000000000000000000000000000000a6000000ab0000
-                  0000000000000064057a0b00007c006a0900000000000000007c00a00200
-                  00000000000000000000000000000000000000a6000000ab000000000000
-                  00000064067a0a00007c006a0500000000000000007a0a00007c00a00300
-                  00000000000000000000000000000000000000a6000000ab000000000000
-                  00000064067a0a00007c006a0500000000000000007a0a0000ac07a60500
-                  00ab0500000000000000007c005f0c000000000000000064005300
-                96           0 RESUME                   0
+                  0000000000000000007c006a0200000000000000007c006a020000000000
+                  0000007c00a0030000000000000000000000000000000000000000a60000
+                  00ab0000000000000000007c006a0200000000000000007a0a00007c00a0
+                  040000000000000000000000000000000000000000a6000000ab00000000
+                  00000000007c006a0200000000000000007a0a00007c006a050000000000
+                  0000007c006a0200000000000000007c006a0600000000000000007c006a
+                  070000000000000000ac02a6080000ab0800000000000000007c005f0800
+                  000000000000007c006a090000000000000000a00a000000000000000000
+                  00000000000000000000007c006a0700000000000000006403ac04a60200
+                  00ab02000000000000000001007c00a00b00000000000000000000000000
+                  000000000000007c00a00300000000000000000000000000000000000000
+                  00a6000000ab00000000000000000064057a0b00007c00a0040000000000
+                  000000000000000000000000000000a6000000ab00000000000000000064
+                  057a0b00007c006a0900000000000000007c00a003000000000000000000
+                  0000000000000000000000a6000000ab00000000000000000064067a0a00
+                  007c006a0200000000000000007a0a00007c006a0c00000000000000007a
+                  0a00007c00a0040000000000000000000000000000000000000000a60000
+                  00ab00000000000000000064067a0a00007c006a0200000000000000007a
+                  0a00007c006a0c00000000000000007a0a0000ac07a6050000ab05000000
+                  00000000007c005f0d000000000000000064005300
+                99           0 RESUME                   0
                
-                97           2 LOAD_FAST                0 (self)
+               100           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               100          44 LOAD_FAST                0 (self)
+               103          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect2)
                
-               101          68 LOAD_CONST               2 (0)
-                            70 LOAD_CONST               2 (0)
-                            72 LOAD_FAST                0 (self)
-                            74 LOAD_METHOD              2 (winfo_width)
-                            96 PRECALL                  0
-                           100 CALL                     0
-                           110 LOAD_FAST                0 (self)
-                           112 LOAD_METHOD              3 (winfo_height)
-                           134 PRECALL                  0
-                           138 CALL                     0
-                           148 LOAD_FAST                0 (self)
-                           150 LOAD_ATTR                4 (frame_radius)
-               
-               102         160 LOAD_FAST                0 (self)
-                           162 LOAD_ATTR                5 (frame_border_width)
+               104          68 LOAD_FAST                0 (self)
+                            70 LOAD_ATTR                2 (frame_border_width)
+                            80 LOAD_FAST                0 (self)
+                            82 LOAD_ATTR                2 (frame_border_width)
                
-               103         172 LOAD_FAST                0 (self)
-                           174 LOAD_ATTR                6 (frame_border)
+               105          92 LOAD_FAST                0 (self)
+                            94 LOAD_METHOD              3 (winfo_width)
+                           116 PRECALL                  0
+                           120 CALL                     0
+                           130 LOAD_FAST                0 (self)
+                           132 LOAD_ATTR                2 (frame_border_width)
+                           142 BINARY_OP               10 (-)
+                           146 LOAD_FAST                0 (self)
+                           148 LOAD_METHOD              4 (winfo_height)
+                           170 PRECALL                  0
+                           174 CALL                     0
                            184 LOAD_FAST                0 (self)
-                           186 LOAD_ATTR                7 (frame_back)
+                           186 LOAD_ATTR                2 (frame_border_width)
+                           196 BINARY_OP               10 (-)
                
-               100         196 KW_NAMES                 3
-                           198 PRECALL                  8
-                           202 CALL                     8
-                           212 LOAD_FAST                0 (self)
-                           214 STORE_ATTR               8 (frame_frame)
-               
-               106         224 LOAD_FAST                0 (self)
-                           226 LOAD_ATTR                9 (frame)
-                           236 LOAD_METHOD             10 (configure)
-                           258 LOAD_FAST                0 (self)
-                           260 LOAD_ATTR                7 (frame_back)
-                           270 LOAD_CONST               2 (0)
-                           272 KW_NAMES                 4
-                           274 PRECALL                  2
-                           278 CALL                     2
-                           288 POP_TOP
-               
-               109         290 LOAD_FAST                0 (self)
-                           292 LOAD_METHOD             11 (create_window)
-               
-               110         314 LOAD_FAST                0 (self)
-                           316 LOAD_METHOD              2 (winfo_width)
-                           338 PRECALL                  0
-                           342 CALL                     0
-                           352 LOAD_CONST               5 (2)
-                           354 BINARY_OP               11 (/)
-                           358 LOAD_FAST                0 (self)
-                           360 LOAD_METHOD              3 (winfo_height)
-                           382 PRECALL                  0
-                           386 CALL                     0
-                           396 LOAD_CONST               5 (2)
-                           398 BINARY_OP               11 (/)
+               106         200 LOAD_FAST                0 (self)
+                           202 LOAD_ATTR                5 (frame_radius)
                
-               111         402 LOAD_FAST                0 (self)
-                           404 LOAD_ATTR                9 (frame)
+               107         212 LOAD_FAST                0 (self)
+                           214 LOAD_ATTR                2 (frame_border_width)
                
-               112         414 LOAD_FAST                0 (self)
-                           416 LOAD_METHOD              2 (winfo_width)
-                           438 PRECALL                  0
-                           442 CALL                     0
-                           452 LOAD_CONST               6 (6)
-                           454 BINARY_OP               10 (-)
-                           458 LOAD_FAST                0 (self)
-                           460 LOAD_ATTR                5 (frame_border_width)
-                           470 BINARY_OP               10 (-)
-               
-               113         474 LOAD_FAST                0 (self)
-                           476 LOAD_METHOD              3 (winfo_height)
-                           498 PRECALL                  0
-                           502 CALL                     0
-                           512 LOAD_CONST               6 (6)
-                           514 BINARY_OP               10 (-)
-                           518 LOAD_FAST                0 (self)
-                           520 LOAD_ATTR                5 (frame_border_width)
-                           530 BINARY_OP               10 (-)
-               
-               109         534 KW_NAMES                 7
-                           536 PRECALL                  5
-                           540 CALL                     5
-                           550 LOAD_FAST                0 (self)
-                           552 STORE_ATTR              12 (frame_f)
-                           562 LOAD_CONST               0 (None)
-                           564 RETURN_VALUE
+               108         224 LOAD_FAST                0 (self)
+                           226 LOAD_ATTR                6 (frame_border)
+                           236 LOAD_FAST                0 (self)
+                           238 LOAD_ATTR                7 (frame_back)
+               
+               103         248 KW_NAMES                 2
+                           250 PRECALL                  8
+                           254 CALL                     8
+                           264 LOAD_FAST                0 (self)
+                           266 STORE_ATTR               8 (frame_frame)
+               
+               111         276 LOAD_FAST                0 (self)
+                           278 LOAD_ATTR                9 (frame)
+                           288 LOAD_METHOD             10 (configure)
+                           310 LOAD_FAST                0 (self)
+                           312 LOAD_ATTR                7 (frame_back)
+                           322 LOAD_CONST               3 (0)
+                           324 KW_NAMES                 4
+                           326 PRECALL                  2
+                           330 CALL                     2
+                           340 POP_TOP
+               
+               114         342 LOAD_FAST                0 (self)
+                           344 LOAD_METHOD             11 (create_window)
+               
+               115         366 LOAD_FAST                0 (self)
+                           368 LOAD_METHOD              3 (winfo_width)
+                           390 PRECALL                  0
+                           394 CALL                     0
+                           404 LOAD_CONST               5 (2)
+                           406 BINARY_OP               11 (/)
+                           410 LOAD_FAST                0 (self)
+                           412 LOAD_METHOD              4 (winfo_height)
+                           434 PRECALL                  0
+                           438 CALL                     0
+                           448 LOAD_CONST               5 (2)
+                           450 BINARY_OP               11 (/)
+               
+               116         454 LOAD_FAST                0 (self)
+                           456 LOAD_ATTR                9 (frame)
+               
+               117         466 LOAD_FAST                0 (self)
+                           468 LOAD_METHOD              3 (winfo_width)
+                           490 PRECALL                  0
+                           494 CALL                     0
+                           504 LOAD_CONST               6 (6)
+                           506 BINARY_OP               10 (-)
+                           510 LOAD_FAST                0 (self)
+                           512 LOAD_ATTR                2 (frame_border_width)
+                           522 BINARY_OP               10 (-)
+                           526 LOAD_FAST                0 (self)
+                           528 LOAD_ATTR               12 (frame_padding)
+                           538 BINARY_OP               10 (-)
+               
+               118         542 LOAD_FAST                0 (self)
+                           544 LOAD_METHOD              4 (winfo_height)
+                           566 PRECALL                  0
+                           570 CALL                     0
+                           580 LOAD_CONST               6 (6)
+                           582 BINARY_OP               10 (-)
+                           586 LOAD_FAST                0 (self)
+                           588 LOAD_ATTR                2 (frame_border_width)
+                           598 BINARY_OP               10 (-)
+                           602 LOAD_FAST                0 (self)
+                           604 LOAD_ATTR               12 (frame_padding)
+                           614 BINARY_OP               10 (-)
+               
+               114         618 KW_NAMES                 7
+                           620 PRECALL                  5
+                           624 CALL                     5
+                           634 LOAD_FAST                0 (self)
+                           636 STORE_ATTR              13 (frame_f)
+                           646 LOAD_CONST               0 (None)
+                           648 RETURN_VALUE
                consts
                   None
                   'all'
-                  0
                   ('width', 'outline', 'fill')
+                  0
                   ('background', 'bd')
                   2
                   6
                   ('window', 'width', 'height')
-               names      ('delete', 'create_round_rect2', 'winfo_width', 'winfo_height', 'frame_radius', 'frame_border_width', 'frame_border', 'frame_back', 'frame_frame', 'frame', 'configure', 'create_window', 'frame_f')
+               names      ('delete', 'create_round_rect2', 'frame_border_width', 'winfo_width', 'winfo_height', 'frame_radius', 'frame_border', 'frame_back', 'frame_frame', 'frame', 'configure', 'create_window', 'frame_padding', 'frame_f')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       '_draw'
-               firstlineno 96
-               lnotab 0x02012a0318015c010c0118fd1c064203180158010c013c013cfc
+               firstlineno 99
+               lnotab
+                  0x02012a03180118016c010c010c0118fb1c084203180158010c014c014c
+                  fc
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               116           0 RESUME                   0
+               121           0 RESUME                   0
                
-               117           2 LOAD_FAST                0 (self)
+               122           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       'default_palette'
-               firstlineno 116
+               firstlineno 121
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 8
+               stacksize : 9
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564069c046901a6010000ab010000000000000000010064
-                  005300
-               119           0 RESUME                   0
+                  02640364046405640664079c056901a6010000ab01000000000000000001
+                  0064005300
+               124           0 RESUME                   0
                
-               120           2 LOAD_FAST                0 (self)
+               125           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               122          26 LOAD_CONST               1 ('frame')
+               127          26 LOAD_CONST               1 ('frame')
                
-               123          28 LOAD_CONST               2 (6)
+               128          28 LOAD_CONST               2 (6)
                
-               124          30 LOAD_CONST               3 ('#0f0f0f')
+               129          30 LOAD_CONST               3 ('#0f0f0f')
                
-               125          32 LOAD_CONST               4 ('#333333')
+               130          32 LOAD_CONST               4 ('#333333')
                
-               126          34 LOAD_CONST               5 (2)
+               131          34 LOAD_CONST               5 (2)
                
-               122          36 LOAD_CONST               6 (('radius', 'back', 'border', 'border_width'))
-                            38 BUILD_CONST_KEY_MAP      4
+               132          36 LOAD_CONST               6 (0)
                
-               121          40 BUILD_MAP                1
+               127          38 LOAD_CONST               7 (('radius', 'back', 'border', 'border_width', 'padding'))
+                            40 BUILD_CONST_KEY_MAP      5
                
-               120          42 PRECALL                  1
-                            46 CALL                     1
-                            56 POP_TOP
-                            58 LOAD_CONST               0 (None)
-                            60 RETURN_VALUE
+               126          42 BUILD_MAP                1
+               
+               125          44 PRECALL                  1
+                            48 CALL                     1
+                            58 POP_TOP
+                            60 LOAD_CONST               0 (None)
+                            62 RETURN_VALUE
                consts
                   None
                   'frame'
                   6
                   '#0f0f0f'
                   '#333333'
                   2
-                  ('radius', 'back', 'border', 'border_width')
+                  0
+                  ('radius', 'back', 'border', 'border_width', 'padding')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       'palette_light'
-               firstlineno 119
-               lnotab 0x02011802020102010201020102fc04ff02ff
+               firstlineno 124
+               lnotab 0x020118020201020102010201020102fb04ff02ff
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 8
+               stacksize : 9
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
-                  0264036404640564069c046901a6010000ab010000000000000000010064
-                  005300
-               131           0 RESUME                   0
+                  02640364046405640664079c056901a6010000ab01000000000000000001
+                  0064005300
+               137           0 RESUME                   0
                
-               132           2 LOAD_FAST                0 (self)
+               138           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               134          26 LOAD_CONST               1 ('frame')
+               140          26 LOAD_CONST               1 ('frame')
                
-               135          28 LOAD_CONST               2 (6)
+               141          28 LOAD_CONST               2 (6)
                
-               136          30 LOAD_CONST               3 ('#0f0f0f')
+               142          30 LOAD_CONST               3 ('#0f0f0f')
                
-               137          32 LOAD_CONST               4 ('#333333')
+               143          32 LOAD_CONST               4 ('#333333')
                
-               138          34 LOAD_CONST               5 (2)
+               144          34 LOAD_CONST               5 (2)
                
-               134          36 LOAD_CONST               6 (('radius', 'back', 'border', 'border_width'))
-                            38 BUILD_CONST_KEY_MAP      4
+               145          36 LOAD_CONST               6 (0)
                
-               133          40 BUILD_MAP                1
+               140          38 LOAD_CONST               7 (('radius', 'back', 'border', 'border_width', 'padding'))
+                            40 BUILD_CONST_KEY_MAP      5
                
-               132          42 PRECALL                  1
-                            46 CALL                     1
-                            56 POP_TOP
-                            58 LOAD_CONST               0 (None)
-                            60 RETURN_VALUE
+               139          42 BUILD_MAP                1
+               
+               138          44 PRECALL                  1
+                            48 CALL                     1
+                            58 POP_TOP
+                            60 LOAD_CONST               0 (None)
+                            62 RETURN_VALUE
                consts
                   None
                   'frame'
                   6
                   '#0f0f0f'
                   '#333333'
                   2
-                  ('radius', 'back', 'border', 'border_width')
+                  0
+                  ('radius', 'back', 'border', 'border_width', 'padding')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       'palette_dark'
-               firstlineno 131
-               lnotab 0x02011802020102010201020102fc04ff02ff
+               firstlineno 137
+               lnotab 0x020118020201020102010201020102fb04ff02ff
             None
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
                   00a00100000000000000000000000000000000000000007c01a6010000ab
                   010000000000000000010064017c01760072157c01640119000000000000
                   0000006402190000000000000000007c005f020000000000000000640053
                   0064005300
                              0 COPY_FREE_VARS           1
                
-               143           2 RESUME                   0
+               150           2 RESUME                   0
                
-               144           4 LOAD_GLOBAL              1 (NULL + super)
+               151           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (palette)
                             52 LOAD_FAST                1 (dict)
                             54 PRECALL                  1
                             58 CALL                     1
                             68 POP_TOP
                
-               145          70 LOAD_CONST               1 ('frame')
+               152          70 LOAD_CONST               1 ('frame')
                             72 LOAD_FAST                1 (dict)
                             74 CONTAINS_OP              0
                             76 POP_JUMP_FORWARD_IF_FALSE    21 (to 120)
                
-               146          78 LOAD_FAST                1 (dict)
+               153          78 LOAD_FAST                1 (dict)
                             80 LOAD_CONST               1 ('frame')
                             82 BINARY_SUBSCR
                             92 LOAD_CONST               2 ('radius')
                             94 BINARY_SUBSCR
                            104 LOAD_FAST                0 (self)
                            106 STORE_ATTR               2 (frame_radius)
                            116 LOAD_CONST               0 (None)
                            118 RETURN_VALUE
                
-               145     >>  120 LOAD_CONST               0 (None)
+               152     >>  120 LOAD_CONST               0 (None)
                            122 RETURN_VALUE
                consts
                   None
                   'frame'
                   'radius'
                names      ('super', 'palette', 'frame_radius')
                varnames   ('self', 'dict')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       'palette'
-               firstlineno 143
+               firstlineno 150
                lnotab 0x0401420108012aff
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', '_draw', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
          name       'AdwDrawBasicRoundFrame'
-         firstlineno 88
-         lnotab 0x0c010a0706140603060c060c
+         firstlineno 91
+         lnotab 0x0c010a0706160603060d060d
       'AdwDrawBasicRoundFrame'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         149           0 RESUME                   0
+         156           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundFrame')
                        8 STORE_NAME               2 (__qualname__)
          
-         150          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 150>)
+         157          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 157>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundFrame'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               150           0 RESUME                   0
+               157           0 RESUME                   0
                
-               151           2 LOAD_FAST                0 (self)
+               158           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       'default_palette'
-               firstlineno 150
+               firstlineno 157
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
          name       'AdwDrawRoundFrame'
-         firstlineno 149
+         firstlineno 156
          lnotab 0x0a01
       'AdwDrawRoundFrame'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         154           0 RESUME                   0
+         161           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawDarkRoundFrame')
                        8 STORE_NAME               2 (__qualname__)
          
-         155          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 155>)
+         162          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 162>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawDarkRoundFrame'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               155           0 RESUME                   0
+               162           0 RESUME                   0
                
-               156           2 LOAD_FAST                0 (self)
+               163           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       'default_palette'
-               firstlineno 155
+               firstlineno 162
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
          name       'AdwDrawDarkRoundFrame'
-         firstlineno 154
+         firstlineno 161
          lnotab 0x0a01
       'AdwDrawDarkRoundFrame'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
             0384005a05880078015a065300
                        0 MAKE_CELL                0 (__class__)
          
-         159           2 RESUME                   0
+         166           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundFrame3')
                       10 STORE_NAME               2 (__qualname__)
          
-         160          12 LOAD_CLOSURE             0 (__class__)
+         167          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 160>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 167>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         167          22 LOAD_CONST               2 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 167>)
+         174          22 LOAD_CONST               2 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 174>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_draw)
          
-         191          28 LOAD_CONST               3 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 191>)
+         200          28 LOAD_CONST               3 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 200>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               5 (default_palette)
                       34 LOAD_CLOSURE             0 (__class__)
                       36 COPY                     1
                       38 STORE_NAME               6 (__classcell__)
                       40 RETURN_VALUE
          consts
@@ -1483,31 +1534,31 @@
                   0000006a0100000000000000007c0169007c02a4018e01010009007c00a0
                   0200000000000000000000000000000000000000007c006a030000000000
                   000000a00400000000000000000000000000000000000000006401a60100
                   00ab010000000000000000ac02a6010000ab010000000000000000010064
                   00530023000100590064005300780359007701
                              0 COPY_FREE_VARS           1
                
-               160           2 RESUME                   0
+               167           2 RESUME                   0
                
-               161           4 PUSH_NULL
+               168           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
                             48 DICT_MERGE               1
                             50 CALL_FUNCTION_EX         1
                             52 POP_TOP
                
-               162          54 NOP
+               169          54 NOP
                
-               163          56 LOAD_FAST                0 (self)
+               170          56 LOAD_FAST                0 (self)
                             58 LOAD_METHOD              2 (configure)
                             80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                3 (master)
                             92 LOAD_METHOD              4 (cget)
                            114 LOAD_CONST               1 ('background')
                            116 PRECALL                  1
                            120 CALL                     1
@@ -1515,17 +1566,17 @@
                            132 PRECALL                  1
                            136 CALL                     1
                            146 POP_TOP
                            148 LOAD_CONST               0 (None)
                            150 RETURN_VALUE
                        >>  152 PUSH_EXC_INFO
                
-               164         154 POP_TOP
+               171         154 POP_TOP
                
-               165         156 POP_EXCEPT
+               172         156 POP_EXCEPT
                            158 LOAD_CONST               0 (None)
                            160 RETURN_VALUE
                        >>  162 COPY                     3
                            164 POP_EXCEPT
                            166 RERAISE                  1
                ExceptionTable:
                  56 to 146 -> 152 [0]
@@ -1536,309 +1587,326 @@
                   ('background',)
                names      ('super', '__init__', 'configure', 'master', 'cget')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       '__init__'
-               firstlineno 160
+               firstlineno 167
                lnotab 0x04013201020162010201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000006401a6
                   010000ab01000000000000000001007c00a0010000000000000000000000
-                  000000000000000000640264027c00a00200000000000000000000000000
-                  00000000000000a6000000ab0000000000000000007c00a0030000000000
-                  000000000000000000000000000000a6000000ab0000000000000000007c
-                  006a0400000000000000007c006a0500000000000000007c006a06000000
-                  00000000007c006a070000000000000000ac03a6080000ab080000000000
-                  000000010064047c005f0800000000000000007c006a0900000000000000
-                  00a00a00000000000000000000000000000000000000007c006a07000000
-                  00000000006402ac05a6020000ab02000000000000000001007c00a00b00
-                  000000000000000000000000000000000000007c00a00200000000000000
-                  00000000000000000000000000a6000000ab00000000000000000064067a
-                  0b00007c00a0030000000000000000000000000000000000000000a60000
-                  00ab00000000000000000064067a0b00007c006a0900000000000000007c
-                  00a0020000000000000000000000000000000000000000a6000000ab0000
-                  0000000000000064077a0a00007c006a0500000000000000007a0a00007c
-                  00a0030000000000000000000000000000000000000000a6000000ab0000
-                  0000000000000064077a0a00007c006a0500000000000000007a0a0000ac
-                  08a6050000ab0500000000000000007c005f0c0000000000000000640053
-                  00
-               167           0 RESUME                   0
+                  0000000000000000007c006a0200000000000000007c006a020000000000
+                  0000007c00a0030000000000000000000000000000000000000000a60000
+                  00ab0000000000000000007c006a0200000000000000007a0a00007c00a0
+                  040000000000000000000000000000000000000000a6000000ab00000000
+                  00000000007c006a0200000000000000007a0a00007c006a050000000000
+                  0000007c006a0200000000000000007c006a0600000000000000007c006a
+                  070000000000000000ac02a6080000ab080000000000000000010064037c
+                  005f0800000000000000007c006a090000000000000000a00a0000000000
+                  0000000000000000000000000000007c006a0700000000000000006404ac
+                  05a6020000ab02000000000000000001007c00a00b000000000000000000
+                  00000000000000000000007c00a003000000000000000000000000000000
+                  0000000000a6000000ab00000000000000000064067a0b00007c00a00400
+                  00000000000000000000000000000000000000a6000000ab000000000000
+                  00000064067a0b00007c006a0900000000000000007c00a0030000000000
+                  000000000000000000000000000000a6000000ab00000000000000000064
+                  077a0a00007c006a0200000000000000007a0a00007c006a0c0000000000
+                  0000007a0a00007c00a00400000000000000000000000000000000000000
+                  00a6000000ab00000000000000000064077a0a00007c006a020000000000
+                  0000007a0a00007c006a0c00000000000000007a0a0000ac08a6050000ab
+                  0500000000000000007c005f0d000000000000000064005300
+               174           0 RESUME                   0
                
-               168           2 LOAD_FAST                0 (self)
+               175           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               171          44 LOAD_FAST                0 (self)
+               178          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect4)
                
-               172          68 LOAD_CONST               2 (0)
-                            70 LOAD_CONST               2 (0)
+               179          68 LOAD_FAST                0 (self)
+                            70 LOAD_ATTR                2 (frame_border_width)
+                            80 LOAD_FAST                0 (self)
+                            82 LOAD_ATTR                2 (frame_border_width)
                
-               173          72 LOAD_FAST                0 (self)
-                            74 LOAD_METHOD              2 (winfo_width)
-                            96 PRECALL                  0
-                           100 CALL                     0
+               180          92 LOAD_FAST                0 (self)
+                            94 LOAD_METHOD              3 (winfo_width)
+                           116 PRECALL                  0
+                           120 CALL                     0
+                           130 LOAD_FAST                0 (self)
+                           132 LOAD_ATTR                2 (frame_border_width)
+                           142 BINARY_OP               10 (-)
                
-               174         110 LOAD_FAST                0 (self)
-                           112 LOAD_METHOD              3 (winfo_height)
-                           134 PRECALL                  0
-                           138 CALL                     0
-                           148 LOAD_FAST                0 (self)
-                           150 LOAD_ATTR                4 (frame_radius)
+               181         146 LOAD_FAST                0 (self)
+                           148 LOAD_METHOD              4 (winfo_height)
+                           170 PRECALL                  0
+                           174 CALL                     0
+                           184 LOAD_FAST                0 (self)
+                           186 LOAD_ATTR                2 (frame_border_width)
+                           196 BINARY_OP               10 (-)
                
-               175         160 LOAD_FAST                0 (self)
-                           162 LOAD_ATTR                5 (frame_border_width)
+               182         200 LOAD_FAST                0 (self)
+                           202 LOAD_ATTR                5 (frame_radius)
                
-               176         172 LOAD_FAST                0 (self)
-                           174 LOAD_ATTR                6 (frame_border)
-                           184 LOAD_FAST                0 (self)
-                           186 LOAD_ATTR                7 (frame_back)
+               183         212 LOAD_FAST                0 (self)
+                           214 LOAD_ATTR                2 (frame_border_width)
                
-               171         196 KW_NAMES                 3
-                           198 PRECALL                  8
-                           202 CALL                     8
-                           212 POP_TOP
-               
-               179         214 LOAD_CONST               4 ('button_frame')
-                           216 LOAD_FAST                0 (self)
-                           218 STORE_ATTR               8 (entry_frame)
-               
-               181         228 LOAD_FAST                0 (self)
-                           230 LOAD_ATTR                9 (frame)
-                           240 LOAD_METHOD             10 (configure)
-                           262 LOAD_FAST                0 (self)
-                           264 LOAD_ATTR                7 (frame_back)
-                           274 LOAD_CONST               2 (0)
-                           276 KW_NAMES                 5
-                           278 PRECALL                  2
-                           282 CALL                     2
-                           292 POP_TOP
-               
-               184         294 LOAD_FAST                0 (self)
-                           296 LOAD_METHOD             11 (create_window)
-               
-               185         318 LOAD_FAST                0 (self)
-                           320 LOAD_METHOD              2 (winfo_width)
-                           342 PRECALL                  0
-                           346 CALL                     0
-                           356 LOAD_CONST               6 (2)
-                           358 BINARY_OP               11 (/)
-                           362 LOAD_FAST                0 (self)
-                           364 LOAD_METHOD              3 (winfo_height)
-                           386 PRECALL                  0
-                           390 CALL                     0
-                           400 LOAD_CONST               6 (2)
-                           402 BINARY_OP               11 (/)
-               
-               186         406 LOAD_FAST                0 (self)
-                           408 LOAD_ATTR                9 (frame)
-               
-               187         418 LOAD_FAST                0 (self)
-                           420 LOAD_METHOD              2 (winfo_width)
-                           442 PRECALL                  0
-                           446 CALL                     0
-                           456 LOAD_CONST               7 (6)
-                           458 BINARY_OP               10 (-)
-                           462 LOAD_FAST                0 (self)
-                           464 LOAD_ATTR                5 (frame_border_width)
-                           474 BINARY_OP               10 (-)
+               184         224 LOAD_FAST                0 (self)
+                           226 LOAD_ATTR                6 (frame_border)
+                           236 LOAD_FAST                0 (self)
+                           238 LOAD_ATTR                7 (frame_back)
+               
+               178         248 KW_NAMES                 2
+                           250 PRECALL                  8
+                           254 CALL                     8
+                           264 POP_TOP
+               
+               188         266 LOAD_CONST               3 ('button_frame')
+                           268 LOAD_FAST                0 (self)
+                           270 STORE_ATTR               8 (entry_frame)
+               
+               190         280 LOAD_FAST                0 (self)
+                           282 LOAD_ATTR                9 (frame)
+                           292 LOAD_METHOD             10 (configure)
+                           314 LOAD_FAST                0 (self)
+                           316 LOAD_ATTR                7 (frame_back)
+                           326 LOAD_CONST               4 (0)
+                           328 KW_NAMES                 5
+                           330 PRECALL                  2
+                           334 CALL                     2
+                           344 POP_TOP
+               
+               193         346 LOAD_FAST                0 (self)
+                           348 LOAD_METHOD             11 (create_window)
+               
+               194         370 LOAD_FAST                0 (self)
+                           372 LOAD_METHOD              3 (winfo_width)
+                           394 PRECALL                  0
+                           398 CALL                     0
+                           408 LOAD_CONST               6 (2)
+                           410 BINARY_OP               11 (/)
+                           414 LOAD_FAST                0 (self)
+                           416 LOAD_METHOD              4 (winfo_height)
+                           438 PRECALL                  0
+                           442 CALL                     0
+                           452 LOAD_CONST               6 (2)
+                           454 BINARY_OP               11 (/)
                
-               188         478 LOAD_FAST                0 (self)
-                           480 LOAD_METHOD              3 (winfo_height)
-                           502 PRECALL                  0
-                           506 CALL                     0
-                           516 LOAD_CONST               7 (6)
-                           518 BINARY_OP               10 (-)
-                           522 LOAD_FAST                0 (self)
-                           524 LOAD_ATTR                5 (frame_border_width)
-                           534 BINARY_OP               10 (-)
+               195         458 LOAD_FAST                0 (self)
+                           460 LOAD_ATTR                9 (frame)
                
-               184         538 KW_NAMES                 8
-                           540 PRECALL                  5
-                           544 CALL                     5
-                           554 LOAD_FAST                0 (self)
-                           556 STORE_ATTR              12 (frame_f)
-                           566 LOAD_CONST               0 (None)
-                           568 RETURN_VALUE
+               196         470 LOAD_FAST                0 (self)
+                           472 LOAD_METHOD              3 (winfo_width)
+                           494 PRECALL                  0
+                           498 CALL                     0
+                           508 LOAD_CONST               7 (6)
+                           510 BINARY_OP               10 (-)
+                           514 LOAD_FAST                0 (self)
+                           516 LOAD_ATTR                2 (frame_border_width)
+                           526 BINARY_OP               10 (-)
+                           530 LOAD_FAST                0 (self)
+                           532 LOAD_ATTR               12 (frame_padding)
+                           542 BINARY_OP               10 (-)
+               
+               197         546 LOAD_FAST                0 (self)
+                           548 LOAD_METHOD              4 (winfo_height)
+                           570 PRECALL                  0
+                           574 CALL                     0
+                           584 LOAD_CONST               7 (6)
+                           586 BINARY_OP               10 (-)
+                           590 LOAD_FAST                0 (self)
+                           592 LOAD_ATTR                2 (frame_border_width)
+                           602 BINARY_OP               10 (-)
+                           606 LOAD_FAST                0 (self)
+                           608 LOAD_ATTR               12 (frame_padding)
+                           618 BINARY_OP               10 (-)
+               
+               193         622 KW_NAMES                 8
+                           624 PRECALL                  5
+                           628 CALL                     5
+                           638 LOAD_FAST                0 (self)
+                           640 STORE_ATTR              13 (frame_f)
+                           650 LOAD_CONST               0 (None)
+                           652 RETURN_VALUE
                consts
                   None
                   'all'
-                  0
                   ('width', 'outline', 'fill')
                   'button_frame'
+                  0
                   ('background', 'bd')
                   2
                   6
                   ('window', 'width', 'height')
-               names      ('delete', 'create_round_rect4', 'winfo_width', 'winfo_height', 'frame_radius', 'frame_border_width', 'frame_border', 'frame_back', 'entry_frame', 'frame', 'configure', 'create_window', 'frame_f')
+               names      ('delete', 'create_round_rect4', 'frame_border_width', 'winfo_width', 'winfo_height', 'frame_radius', 'frame_border', 'frame_back', 'entry_frame', 'frame', 'configure', 'create_window', 'frame_padding', 'frame_f')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       '_draw'
-               firstlineno 167
+               firstlineno 174
                lnotab
-                  0x02012a0318010401260132010c0118fb12080e024203180158010c013c
-                  013cfc
+                  0x02012a0318011801360136010c010c0118fa120a0e024203180158010c
+                  014c014cfc
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               191           0 RESUME                   0
+               200           0 RESUME                   0
                
-               192           2 LOAD_FAST                0 (self)
+               201           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       'default_palette'
-               firstlineno 191
+               firstlineno 200
                lnotab 0x0201
          names      ('__name__', '__module__', '__qualname__', '__init__', '_draw', 'default_palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
          name       'AdwDrawBasicRoundFrame3'
-         firstlineno 159
-         lnotab 0x0c010a070618
+         firstlineno 166
+         lnotab 0x0c010a07061a
       'AdwDrawBasicRoundFrame3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         195           0 RESUME                   0
+         204           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundFrame3')
                        8 STORE_NAME               2 (__qualname__)
          
-         196          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 196>)
+         205          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 205>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundFrame3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               196           0 RESUME                   0
+               205           0 RESUME                   0
                
-               197           2 LOAD_FAST                0 (self)
+               206           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       'default_palette'
-               firstlineno 196
+               firstlineno 205
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
          name       'AdwDrawRoundFrame3'
-         firstlineno 195
+         firstlineno 204
          lnotab 0x0a01
       'AdwDrawRoundFrame3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         200           0 RESUME                   0
+         209           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawDarkRoundFrame3')
                        8 STORE_NAME               2 (__qualname__)
          
-         201          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 201>)
+         210          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\frame.py", line 210>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawDarkRoundFrame3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               201           0 RESUME                   0
+               210           0 RESUME                   0
                
-               202           2 LOAD_FAST                0 (self)
+               211           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
                name       'default_palette'
-               firstlineno 201
+               firstlineno 210
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
          name       'AdwDrawDarkRoundFrame3'
-         firstlineno 200
+         firstlineno 209
          lnotab 0x0a01
       'AdwDrawDarkRoundFrame3'
       '__main__'
       ('Tk',)
       'both'
       'yes'
       ('fill', 'expand')
@@ -1849,9 +1917,9 @@
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\windows\\canvas\\frame.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c010c041c481c051c051c3d1c051c051c241c051c050e010c
+      0x00ff02010c010c041c4b1c051c051c411c051c051c261c051c050e010c
       02140214012e022001320214012e022001320214012e02200132022ce9
```

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc` & `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/separator.cpython-310.pyc` & `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/separator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/separator.cpython-311.pyc` & `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/separator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/textbox.cpython-310.pyc` & `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/textbox.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/textbox.cpython-311.pyc` & `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/textbox.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x59cdaa64 (Sun Jul  9 15:08:09 2023 UTC)
-files sz: 17817
+moddate:  0xc938b364 (Sun Jul 16 00:24:41 2023 UTC)
+files sz: 17828
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
@@ -42,238 +42,238 @@
                  8 IMPORT_FROM              1 (Font)
                 10 STORE_NAME               1 (Font)
                 12 IMPORT_FROM              2 (nametofont)
                 14 STORE_NAME               2 (nametofont)
                 16 POP_TOP
    
      2          18 LOAD_CONST               0 (0)
-                20 LOAD_CONST               2 (('AdwDrawEngine',))
-                22 IMPORT_NAME              3 (tkadw.windows.canvas.drawengine)
-                24 IMPORT_FROM              4 (AdwDrawEngine)
-                26 STORE_NAME               4 (AdwDrawEngine)
+                20 LOAD_CONST               2 (('AdwWidget',))
+                22 IMPORT_NAME              3 (tkadw.windows.canvas.widget)
+                24 IMPORT_FROM              4 (AdwWidget)
+                26 STORE_NAME               4 (AdwWidget)
                 28 POP_TOP
    
      6          30 PUSH_NULL
                 32 LOAD_BUILD_CLASS
                 34 LOAD_CONST               3 (<code object AdwDrawBasicText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 6>)
                 36 MAKE_FUNCTION            0
                 38 LOAD_CONST               4 ('AdwDrawBasicText')
-                40 LOAD_NAME                4 (AdwDrawEngine)
+                40 LOAD_NAME                4 (AdwWidget)
                 42 PRECALL                  3
                 46 CALL                     3
                 56 STORE_NAME               5 (AdwDrawBasicText)
    
-   263          58 PUSH_NULL
+   264          58 PUSH_NULL
                 60 LOAD_BUILD_CLASS
-                62 LOAD_CONST               5 (<code object AdwDrawText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 263>)
+                62 LOAD_CONST               5 (<code object AdwDrawText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 264>)
                 64 MAKE_FUNCTION            0
                 66 LOAD_CONST               6 ('AdwDrawText')
                 68 LOAD_NAME                5 (AdwDrawBasicText)
                 70 PRECALL                  3
                 74 CALL                     3
                 84 STORE_NAME               6 (AdwDrawText)
    
-   268          86 PUSH_NULL
+   269          86 PUSH_NULL
                 88 LOAD_BUILD_CLASS
-                90 LOAD_CONST               7 (<code object AdwDrawDarkText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 268>)
+                90 LOAD_CONST               7 (<code object AdwDrawDarkText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 269>)
                 92 MAKE_FUNCTION            0
                 94 LOAD_CONST               8 ('AdwDrawDarkText')
                 96 LOAD_NAME                5 (AdwDrawBasicText)
                 98 PRECALL                  3
                102 CALL                     3
                112 STORE_NAME               7 (AdwDrawDarkText)
    
-   274         114 PUSH_NULL
+   275         114 PUSH_NULL
                116 LOAD_BUILD_CLASS
-               118 LOAD_CONST               9 (<code object AdwDrawBasicRoundText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 274>)
+               118 LOAD_CONST               9 (<code object AdwDrawBasicRoundText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 275>)
                120 MAKE_FUNCTION            0
                122 LOAD_CONST              10 ('AdwDrawBasicRoundText')
                124 LOAD_NAME                5 (AdwDrawBasicText)
                126 PRECALL                  3
                130 CALL                     3
                140 STORE_NAME               8 (AdwDrawBasicRoundText)
    
-   382         142 PUSH_NULL
+   383         142 PUSH_NULL
                144 LOAD_BUILD_CLASS
-               146 LOAD_CONST              11 (<code object AdwDrawRoundText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 382>)
+               146 LOAD_CONST              11 (<code object AdwDrawRoundText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 383>)
                148 MAKE_FUNCTION            0
                150 LOAD_CONST              12 ('AdwDrawRoundText')
                152 LOAD_NAME                8 (AdwDrawBasicRoundText)
                154 PRECALL                  3
                158 CALL                     3
                168 STORE_NAME               9 (AdwDrawRoundText)
    
-   387         170 PUSH_NULL
+   388         170 PUSH_NULL
                172 LOAD_BUILD_CLASS
-               174 LOAD_CONST              13 (<code object AdwDrawRoundDarkText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 387>)
+               174 LOAD_CONST              13 (<code object AdwDrawRoundDarkText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 388>)
                176 MAKE_FUNCTION            0
                178 LOAD_CONST              14 ('AdwDrawRoundDarkText')
                180 LOAD_NAME                8 (AdwDrawBasicRoundText)
                182 PRECALL                  3
                186 CALL                     3
                196 STORE_NAME              10 (AdwDrawRoundDarkText)
    
-   392         198 PUSH_NULL
+   393         198 PUSH_NULL
                200 LOAD_BUILD_CLASS
-               202 LOAD_CONST              15 (<code object AdwDrawBasicRoundText3, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 392>)
+               202 LOAD_CONST              15 (<code object AdwDrawBasicRoundText3, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 393>)
                204 MAKE_FUNCTION            0
                206 LOAD_CONST              16 ('AdwDrawBasicRoundText3')
                208 LOAD_NAME                8 (AdwDrawBasicRoundText)
                210 PRECALL                  3
                214 CALL                     3
                224 STORE_NAME              11 (AdwDrawBasicRoundText3)
    
-   501         226 PUSH_NULL
+   502         226 PUSH_NULL
                228 LOAD_BUILD_CLASS
-               230 LOAD_CONST              17 (<code object AdwDrawRoundText3, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 501>)
+               230 LOAD_CONST              17 (<code object AdwDrawRoundText3, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 502>)
                232 MAKE_FUNCTION            0
                234 LOAD_CONST              18 ('AdwDrawRoundText3')
                236 LOAD_NAME               11 (AdwDrawBasicRoundText3)
                238 PRECALL                  3
                242 CALL                     3
                252 STORE_NAME              12 (AdwDrawRoundText3)
    
-   506         254 PUSH_NULL
+   507         254 PUSH_NULL
                256 LOAD_BUILD_CLASS
-               258 LOAD_CONST              19 (<code object AdwDrawRoundDarkText3, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 506>)
+               258 LOAD_CONST              19 (<code object AdwDrawRoundDarkText3, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 507>)
                260 MAKE_FUNCTION            0
                262 LOAD_CONST              20 ('AdwDrawRoundDarkText3')
                264 LOAD_NAME               11 (AdwDrawBasicRoundText3)
                266 PRECALL                  3
                270 CALL                     3
                280 STORE_NAME              13 (AdwDrawRoundDarkText3)
    
-   511         282 LOAD_NAME               14 (__name__)
+   512         282 LOAD_NAME               14 (__name__)
                284 LOAD_CONST              21 ('__main__')
                286 COMPARE_OP               2 (==)
                292 POP_JUMP_FORWARD_IF_FALSE   242 (to 778)
    
-   512         294 LOAD_CONST               0 (0)
+   513         294 LOAD_CONST               0 (0)
                296 LOAD_CONST              22 (('Tk',))
                298 IMPORT_NAME             15 (tkinter)
                300 IMPORT_FROM             16 (Tk)
                302 STORE_NAME              16 (Tk)
                304 POP_TOP
    
-   514         306 PUSH_NULL
+   515         306 PUSH_NULL
                308 LOAD_NAME               16 (Tk)
                310 PRECALL                  0
                314 CALL                     0
                324 STORE_NAME              17 (root)
    
-   516         326 PUSH_NULL
+   517         326 PUSH_NULL
                328 LOAD_NAME                6 (AdwDrawText)
                330 PRECALL                  0
                334 CALL                     0
                344 STORE_NAME              18 (text1)
    
-   517         346 LOAD_NAME               18 (text1)
+   518         346 LOAD_NAME               18 (text1)
                348 LOAD_METHOD             19 (pack)
                370 LOAD_CONST              23 ('x')
                372 LOAD_CONST              24 (5)
                374 LOAD_CONST              24 (5)
                376 KW_NAMES                25
                378 PRECALL                  3
                382 CALL                     3
                392 POP_TOP
    
-   519         394 PUSH_NULL
+   520         394 PUSH_NULL
                396 LOAD_NAME                7 (AdwDrawDarkText)
                398 PRECALL                  0
                402 CALL                     0
                412 STORE_NAME              20 (text2)
    
-   520         414 LOAD_NAME               20 (text2)
+   521         414 LOAD_NAME               20 (text2)
                416 LOAD_METHOD             19 (pack)
                438 LOAD_CONST              23 ('x')
                440 LOAD_CONST              24 (5)
                442 LOAD_CONST              24 (5)
                444 KW_NAMES                25
                446 PRECALL                  3
                450 CALL                     3
                460 POP_TOP
    
-   522         462 PUSH_NULL
+   523         462 PUSH_NULL
                464 LOAD_NAME                9 (AdwDrawRoundText)
                466 PRECALL                  0
                470 CALL                     0
                480 STORE_NAME              21 (text3)
    
-   523         482 LOAD_NAME               21 (text3)
+   524         482 LOAD_NAME               21 (text3)
                484 LOAD_METHOD             19 (pack)
                506 LOAD_CONST              23 ('x')
                508 LOAD_CONST              24 (5)
                510 LOAD_CONST              24 (5)
                512 KW_NAMES                25
                514 PRECALL                  3
                518 CALL                     3
                528 POP_TOP
    
-   525         530 PUSH_NULL
+   526         530 PUSH_NULL
                532 LOAD_NAME               10 (AdwDrawRoundDarkText)
                534 PRECALL                  0
                538 CALL                     0
                548 STORE_NAME              22 (text4)
    
-   526         550 LOAD_NAME               22 (text4)
+   527         550 LOAD_NAME               22 (text4)
                552 LOAD_METHOD             19 (pack)
                574 LOAD_CONST              23 ('x')
                576 LOAD_CONST              24 (5)
                578 LOAD_CONST              24 (5)
                580 KW_NAMES                25
                582 PRECALL                  3
                586 CALL                     3
                596 POP_TOP
    
-   528         598 PUSH_NULL
+   529         598 PUSH_NULL
                600 LOAD_NAME               12 (AdwDrawRoundText3)
                602 PRECALL                  0
                606 CALL                     0
                616 STORE_NAME              23 (text5)
    
-   529         618 LOAD_NAME               23 (text5)
+   530         618 LOAD_NAME               23 (text5)
                620 LOAD_METHOD             19 (pack)
                642 LOAD_CONST              23 ('x')
                644 LOAD_CONST              24 (5)
                646 LOAD_CONST              24 (5)
                648 KW_NAMES                25
                650 PRECALL                  3
                654 CALL                     3
                664 POP_TOP
    
-   531         666 PUSH_NULL
+   532         666 PUSH_NULL
                668 LOAD_NAME               13 (AdwDrawRoundDarkText3)
                670 PRECALL                  0
                674 CALL                     0
                684 STORE_NAME              24 (text6)
    
-   532         686 LOAD_NAME               24 (text6)
+   533         686 LOAD_NAME               24 (text6)
                688 LOAD_METHOD             19 (pack)
                710 LOAD_CONST              23 ('x')
                712 LOAD_CONST              24 (5)
                714 LOAD_CONST              24 (5)
                716 KW_NAMES                25
                718 PRECALL                  3
                722 CALL                     3
                732 POP_TOP
    
-   534         734 LOAD_NAME               17 (root)
+   535         734 LOAD_NAME               17 (root)
                736 LOAD_METHOD             25 (mainloop)
                758 PRECALL                  0
                762 CALL                     0
                772 POP_TOP
                774 LOAD_CONST              26 (None)
                776 RETURN_VALUE
    
-   511     >>  778 LOAD_CONST              26 (None)
+   512     >>  778 LOAD_CONST              26 (None)
                780 RETURN_VALUE
    consts
       0
       ('Font', 'nametofont')
-      ('AdwDrawEngine',)
+      ('AdwWidget',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x8700970065005a0164005a0264016402640364049c0364056503660288
@@ -395,28 +395,28 @@
                      170 LOAD_CONST              28 ('font')
                      172 LOAD_NAME               25 (Font)
                      174 BUILD_TUPLE              2
                      176 LOAD_CONST              29 (<code object font, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 162>)
                      178 MAKE_FUNCTION            5 (defaults, annotations)
                      180 STORE_NAME              26 (font)
          
-         168         182 LOAD_CONST              30 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 168>)
+         169         182 LOAD_CONST              30 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 169>)
                      184 MAKE_FUNCTION            0
                      186 STORE_NAME              27 (default_palette)
          
-         171         188 LOAD_CONST              31 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 171>)
+         172         188 LOAD_CONST              31 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 172>)
                      190 MAKE_FUNCTION            0
                      192 STORE_NAME              28 (palette_light)
          
-         198         194 LOAD_CONST              32 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 198>)
+         199         194 LOAD_CONST              32 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 199>)
                      196 MAKE_FUNCTION            0
                      198 STORE_NAME              29 (palette_dark)
          
-         225         200 LOAD_CONST              34 ((None,))
-                     202 LOAD_CONST              33 (<code object palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 225>)
+         226         200 LOAD_CONST              34 ((None,))
+                     202 LOAD_CONST              33 (<code object palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 226>)
                      204 MAKE_FUNCTION            1 (defaults)
                      206 STORE_NAME              30 (palette)
                      208 LOAD_CLOSURE             0 (__class__)
                      210 COPY                     1
                      212 STORE_NAME              31 (__classcell__)
                      214 RETURN_VALUE
          consts
@@ -1938,117 +1938,124 @@
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
-                  000000000064005300
+                  00000000007c00a0010000000000000000000000000000000000000000a6
+                  000000ab000000000000000000010064005300
                162           0 RESUME                   0
                
                163           2 LOAD_FAST                1 (font)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
                164           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (text_text_font)
                             18 RETURN_VALUE
                
                166     >>   20 LOAD_FAST                1 (font)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (text_text_font)
-                            34 LOAD_CONST               0 (None)
-                            36 RETURN_VALUE
+               
+               167          34 LOAD_FAST                0 (self)
+                            36 LOAD_METHOD              1 (update)
+                            58 PRECALL                  0
+                            62 CALL                     0
+                            72 POP_TOP
+                            74 LOAD_CONST               0 (None)
+                            76 RETURN_VALUE
                consts
                   None
-               names      ('text_text_font',)
+               names      ('text_text_font', 'update')
                varnames   ('self', 'font')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'font'
                firstlineno 162
-               lnotab 0x020104010e02
+               lnotab 0x020104010e020e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               168           0 RESUME                   0
+               169           0 RESUME                   0
                
-               169           2 LOAD_FAST                0 (self)
+               170           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 168
+               firstlineno 169
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066404640764086409640a6406640b640c640d9c0664
                   0e9c086901a6010000ab010000000000000000010064005300
-               171           0 RESUME                   0
+               172           0 RESUME                   0
                
-               172           2 LOAD_FAST                0 (self)
+               173           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               174          26 LOAD_CONST               1 ('text')
+               175          26 LOAD_CONST               1 ('text')
                
-               175          28 LOAD_CONST               2 ((3, 4))
+               176          28 LOAD_CONST               2 ((3, 4))
                
-               177          30 LOAD_CONST               3 ('#fdfdfd')
+               178          30 LOAD_CONST               3 ('#fdfdfd')
                
-               178          32 LOAD_CONST               4 ('#eaeaea')
+               179          32 LOAD_CONST               4 ('#eaeaea')
                
-               179          34 LOAD_CONST               5 ('#5f5f5f')
+               180          34 LOAD_CONST               5 ('#5f5f5f')
                
-               180          36 LOAD_CONST               6 (1)
+               181          36 LOAD_CONST               6 (1)
                
-               182          38 LOAD_CONST               4 ('#eaeaea')
+               183          38 LOAD_CONST               4 ('#eaeaea')
                
-               183          40 LOAD_CONST               7 (0)
+               184          40 LOAD_CONST               7 (0)
                
-               186          42 LOAD_CONST               8 ('#f9f9f9')
+               187          42 LOAD_CONST               8 ('#f9f9f9')
                
-               187          44 LOAD_CONST               9 ('#e2e2e2')
+               188          44 LOAD_CONST               9 ('#e2e2e2')
                
-               188          46 LOAD_CONST              10 ('#1a1a1a')
+               189          46 LOAD_CONST              10 ('#1a1a1a')
                
-               189          48 LOAD_CONST               6 (1)
+               190          48 LOAD_CONST               6 (1)
                
-               191          50 LOAD_CONST              11 ('#185fb4')
+               192          50 LOAD_CONST              11 ('#185fb4')
                
-               192          52 LOAD_CONST              12 (2)
+               193          52 LOAD_CONST              12 (2)
                
-               185          54 LOAD_CONST              13 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               186          54 LOAD_CONST              13 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
                             56 BUILD_CONST_KEY_MAP      6
                
-               174          58 LOAD_CONST              14 (('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               175          58 LOAD_CONST              14 (('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
                             60 BUILD_CONST_KEY_MAP      8
                
-               173          62 BUILD_MAP                1
+               174          62 BUILD_MAP                1
                
-               172          64 PRECALL                  1
+               173          64 PRECALL                  1
                             68 CALL                     1
                             78 POP_TOP
                             80 LOAD_CONST               0 (None)
                             82 RETURN_VALUE
                consts
                   None
                   'text'
@@ -2067,69 +2074,69 @@
                   ('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'palette_light'
-               firstlineno 171
+               firstlineno 172
                lnotab
                   0x0201180202010202020102010201020202010203020102010201020202
                   0102f904f504ff02ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   026403640464056406640764086409640464076406640a640b640c9c0664
                   0d9c086901a6010000ab010000000000000000010064005300
-               198           0 RESUME                   0
+               199           0 RESUME                   0
                
-               199           2 LOAD_FAST                0 (self)
+               200           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               201          26 LOAD_CONST               1 ('text')
+               202          26 LOAD_CONST               1 ('text')
                
-               202          28 LOAD_CONST               2 ((3, 4))
+               203          28 LOAD_CONST               2 ((3, 4))
                
-               204          30 LOAD_CONST               3 ('#353535')
+               205          30 LOAD_CONST               3 ('#353535')
                
-               205          32 LOAD_CONST               4 ('#454545')
+               206          32 LOAD_CONST               4 ('#454545')
                
-               206          34 LOAD_CONST               5 ('#cecece')
+               207          34 LOAD_CONST               5 ('#cecece')
                
-               207          36 LOAD_CONST               6 (1)
+               208          36 LOAD_CONST               6 (1)
                
-               209          38 LOAD_CONST               7 ('#ffffff')
+               210          38 LOAD_CONST               7 ('#ffffff')
                
-               210          40 LOAD_CONST               8 (0)
+               211          40 LOAD_CONST               8 (0)
                
-               213          42 LOAD_CONST               9 ('#2f2f2f')
+               214          42 LOAD_CONST               9 ('#2f2f2f')
                
-               214          44 LOAD_CONST               4 ('#454545')
+               215          44 LOAD_CONST               4 ('#454545')
                
-               215          46 LOAD_CONST               7 ('#ffffff')
+               216          46 LOAD_CONST               7 ('#ffffff')
                
-               216          48 LOAD_CONST               6 (1)
+               217          48 LOAD_CONST               6 (1)
                
-               218          50 LOAD_CONST              10 ('#4cc2ff')
+               219          50 LOAD_CONST              10 ('#4cc2ff')
                
-               219          52 LOAD_CONST              11 (2)
+               220          52 LOAD_CONST              11 (2)
                
-               212          54 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               213          54 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
                             56 BUILD_CONST_KEY_MAP      6
                
-               201          58 LOAD_CONST              13 (('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               202          58 LOAD_CONST              13 (('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
                             60 BUILD_CONST_KEY_MAP      8
                
-               200          62 BUILD_MAP                1
+               201          62 BUILD_MAP                1
                
-               199          64 PRECALL                  1
+               200          64 PRECALL                  1
                             68 CALL                     1
                             78 POP_TOP
                             80 LOAD_CONST               0 (None)
                             82 RETURN_VALUE
                consts
                   None
                   'text'
@@ -2147,15 +2154,15 @@
                   ('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'palette_dark'
-               firstlineno 198
+               firstlineno 199
                lnotab
                   0x0201180202010202020102010201020202010203020102010201020202
                   0102f904f504ff02ff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
@@ -2185,205 +2192,205 @@
                   006a0200000000000000007c005f0e00000000000000007c006a03000000
                   00000000007c005f0f00000000000000007c006a0500000000000000007c
                   005f1000000000000000007c006a0600000000000000007c005f11000000
                   00000000007c017c005f12000000000000000009007c00a0130000000000
                   0000000000000000000000000000006400a6010000ab0100000000000000
                   000100640053002300742800000000000000000000240072040100590064
                   00530077007803590077017c006a1200000000000000005300
-               225           0 RESUME                   0
+               226           0 RESUME                   0
                
-               226           2 LOAD_FAST                1 (dict)
+               227           2 LOAD_FAST                1 (dict)
                              4 EXTENDED_ARG             1
                              6 POP_JUMP_FORWARD_IF_NONE   406 (to 820)
                
-               227           8 LOAD_CONST               1 ('text')
+               228           8 LOAD_CONST               1 ('text')
                             10 LOAD_FAST                1 (dict)
                             12 CONTAINS_OP              0
                             14 EXTENDED_ARG             1
                             16 POP_JUMP_FORWARD_IF_FALSE   293 (to 604)
                
-               228          18 LOAD_FAST                1 (dict)
+               229          18 LOAD_FAST                1 (dict)
                             20 LOAD_CONST               1 ('text')
                             22 BINARY_SUBSCR
                             32 LOAD_CONST               2 ('padding')
                             34 BINARY_SUBSCR
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               0 (text_padding)
                
-               230          56 LOAD_FAST                1 (dict)
+               231          56 LOAD_FAST                1 (dict)
                             58 LOAD_CONST               1 ('text')
                             60 BINARY_SUBSCR
                             70 LOAD_CONST               3 ('back')
                             72 BINARY_SUBSCR
                             82 LOAD_FAST                0 (self)
                             84 STORE_ATTR               1 (text_back)
                
-               231          94 LOAD_FAST                1 (dict)
+               232          94 LOAD_FAST                1 (dict)
                             96 LOAD_CONST               1 ('text')
                             98 BINARY_SUBSCR
                            108 LOAD_CONST               4 ('border')
                            110 BINARY_SUBSCR
                            120 LOAD_FAST                0 (self)
                            122 STORE_ATTR               2 (text_border)
                
-               232         132 LOAD_FAST                1 (dict)
+               233         132 LOAD_FAST                1 (dict)
                            134 LOAD_CONST               1 ('text')
                            136 BINARY_SUBSCR
                            146 LOAD_CONST               5 ('text_back')
                            148 BINARY_SUBSCR
                            158 LOAD_FAST                0 (self)
                            160 STORE_ATTR               3 (text_text_back)
                
-               233         170 LOAD_FAST                1 (dict)
+               234         170 LOAD_FAST                1 (dict)
                            172 LOAD_CONST               1 ('text')
                            174 BINARY_SUBSCR
                            184 LOAD_CONST               6 ('border_width')
                            186 BINARY_SUBSCR
                            196 LOAD_FAST                0 (self)
                            198 STORE_ATTR               4 (text_border_width)
                
-               235         208 LOAD_FAST                1 (dict)
+               236         208 LOAD_FAST                1 (dict)
                            210 LOAD_CONST               1 ('text')
                            212 BINARY_SUBSCR
                            222 LOAD_CONST               7 ('bottom_line')
                            224 BINARY_SUBSCR
                            234 LOAD_FAST                0 (self)
                            236 STORE_ATTR               5 (text_bottom_line)
                
-               236         246 LOAD_FAST                1 (dict)
+               237         246 LOAD_FAST                1 (dict)
                            248 LOAD_CONST               1 ('text')
                            250 BINARY_SUBSCR
                            260 LOAD_CONST               8 ('bottom_width')
                            262 BINARY_SUBSCR
                            272 LOAD_FAST                0 (self)
                            274 STORE_ATTR               6 (text_bottom_width)
                
-               238         284 LOAD_CONST               9 ('focusin')
+               239         284 LOAD_CONST               9 ('focusin')
                            286 LOAD_FAST                1 (dict)
                            288 LOAD_CONST               1 ('text')
                            290 BINARY_SUBSCR
                            300 CONTAINS_OP              0
                            302 POP_JUMP_FORWARD_IF_FALSE   150 (to 604)
                
-               239         304 LOAD_FAST                1 (dict)
+               240         304 LOAD_FAST                1 (dict)
                            306 LOAD_CONST               1 ('text')
                            308 BINARY_SUBSCR
                            318 LOAD_CONST               9 ('focusin')
                            320 BINARY_SUBSCR
                            330 LOAD_CONST               3 ('back')
                            332 BINARY_SUBSCR
                            342 LOAD_FAST                0 (self)
                            344 STORE_ATTR               7 (text_focusin_back)
                
-               240         354 LOAD_FAST                1 (dict)
+               241         354 LOAD_FAST                1 (dict)
                            356 LOAD_CONST               1 ('text')
                            358 BINARY_SUBSCR
                            368 LOAD_CONST               9 ('focusin')
                            370 BINARY_SUBSCR
                            380 LOAD_CONST               4 ('border')
                            382 BINARY_SUBSCR
                            392 LOAD_FAST                0 (self)
                            394 STORE_ATTR               8 (text_focusin_border)
                
-               241         404 LOAD_FAST                1 (dict)
+               242         404 LOAD_FAST                1 (dict)
                            406 LOAD_CONST               1 ('text')
                            408 BINARY_SUBSCR
                            418 LOAD_CONST               9 ('focusin')
                            420 BINARY_SUBSCR
                            430 LOAD_CONST               5 ('text_back')
                            432 BINARY_SUBSCR
                            442 LOAD_FAST                0 (self)
                            444 STORE_ATTR               9 (text_focusin_text_back)
                
-               242         454 LOAD_FAST                1 (dict)
+               243         454 LOAD_FAST                1 (dict)
                            456 LOAD_CONST               1 ('text')
                            458 BINARY_SUBSCR
                            468 LOAD_CONST               9 ('focusin')
                            470 BINARY_SUBSCR
                            480 LOAD_CONST               6 ('border_width')
                            482 BINARY_SUBSCR
                            492 LOAD_FAST                0 (self)
                            494 STORE_ATTR              10 (text_focusin_border_width)
                
-               244         504 LOAD_FAST                1 (dict)
+               245         504 LOAD_FAST                1 (dict)
                            506 LOAD_CONST               1 ('text')
                            508 BINARY_SUBSCR
                            518 LOAD_CONST               9 ('focusin')
                            520 BINARY_SUBSCR
                            530 LOAD_CONST               7 ('bottom_line')
                            532 BINARY_SUBSCR
                            542 LOAD_FAST                0 (self)
                            544 STORE_ATTR              11 (text_focusin_bottom_line)
                
-               245         554 LOAD_FAST                1 (dict)
+               246         554 LOAD_FAST                1 (dict)
                            556 LOAD_CONST               1 ('text')
                            558 BINARY_SUBSCR
                            568 LOAD_CONST               9 ('focusin')
                            570 BINARY_SUBSCR
                            580 LOAD_CONST               8 ('bottom_width')
                            582 BINARY_SUBSCR
                            592 LOAD_FAST                0 (self)
                            594 STORE_ATTR              12 (text_focusin_bottom_width)
                
-               247     >>  604 LOAD_FAST                0 (self)
+               248     >>  604 LOAD_FAST                0 (self)
                            606 LOAD_ATTR                1 (text_back)
                            616 LOAD_FAST                0 (self)
                            618 STORE_ATTR              13 (_text_back)
                
-               248         628 LOAD_FAST                0 (self)
+               249         628 LOAD_FAST                0 (self)
                            630 LOAD_ATTR                2 (text_border)
                            640 LOAD_FAST                0 (self)
                            642 STORE_ATTR              14 (_text_border)
                
-               249         652 LOAD_FAST                0 (self)
+               250         652 LOAD_FAST                0 (self)
                            654 LOAD_ATTR                3 (text_text_back)
                            664 LOAD_FAST                0 (self)
                            666 STORE_ATTR              15 (_text_text_back)
                
-               250         676 LOAD_FAST                0 (self)
+               251         676 LOAD_FAST                0 (self)
                            678 LOAD_ATTR                5 (text_bottom_line)
                            688 LOAD_FAST                0 (self)
                            690 STORE_ATTR              16 (_text_bottom_line)
                
-               251         700 LOAD_FAST                0 (self)
+               252         700 LOAD_FAST                0 (self)
                            702 LOAD_ATTR                6 (text_bottom_width)
                            712 LOAD_FAST                0 (self)
                            714 STORE_ATTR              17 (_text_bottom_width)
                
-               253         724 LOAD_FAST                1 (dict)
+               254         724 LOAD_FAST                1 (dict)
                            726 LOAD_FAST                0 (self)
                            728 STORE_ATTR              18 (_palette)
                
-               255         738 NOP
+               256         738 NOP
                
-               256         740 LOAD_FAST                0 (self)
+               257         740 LOAD_FAST                0 (self)
                            742 LOAD_METHOD             19 (_draw)
                            764 LOAD_CONST               0 (None)
                            766 PRECALL                  1
                            770 CALL                     1
                            780 POP_TOP
                            782 LOAD_CONST               0 (None)
                            784 RETURN_VALUE
                        >>  786 PUSH_EXC_INFO
                
-               257         788 LOAD_GLOBAL             40 (AttributeError)
+               258         788 LOAD_GLOBAL             40 (AttributeError)
                            800 CHECK_EXC_MATCH
                            802 POP_JUMP_FORWARD_IF_FALSE     4 (to 812)
                            804 POP_TOP
                
-               258         806 POP_EXCEPT
+               259         806 POP_EXCEPT
                            808 LOAD_CONST               0 (None)
                            810 RETURN_VALUE
                
-               257     >>  812 RERAISE                  0
+               258     >>  812 RERAISE                  0
                        >>  814 COPY                     3
                            816 POP_EXCEPT
                            818 RERAISE                  1
                
-               260     >>  820 LOAD_FAST                0 (self)
+               261     >>  820 LOAD_FAST                0 (self)
                            822 LOAD_ATTR               18 (_palette)
                            832 RETURN_VALUE
                ExceptionTable:
                  740 to 780 -> 786 [0]
                  786 to 804 -> 814 [1] lasti
                  812 to 812 -> 814 [1] lasti
                consts
@@ -2399,194 +2406,194 @@
                   'focusin'
                names      ('text_padding', 'text_back', 'text_border', 'text_text_back', 'text_border_width', 'text_bottom_line', 'text_bottom_width', 'text_focusin_back', 'text_focusin_border', 'text_focusin_text_back', 'text_focusin_border_width', 'text_focusin_bottom_line', 'text_focusin_bottom_width', '_text_back', '_text_border', '_text_text_back', '_text_bottom_line', '_text_bottom_width', '_palette', '_draw', 'AttributeError')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'palette'
-               firstlineno 225
+               firstlineno 226
                lnotab
                   0x020106010a012602260126012601260226012602140132013201320132
                   0232013202180118011801180118020e0202013001120106ff0803
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'str', '__init__', 'tbbox', 'compare', 'count', 'debug', 'tdelete', 'dump', 'get', 'tindex', 'tinsert', 'search', 'see', 'undo', 'redo', '_other', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawBasicText'
          firstlineno 6
          lnotab
             0x0c011a2b06030603060306030603060306030603060306030603060606
-            060604061c0809080908030803080b0e060603061b061b
+            060604061c0809080908030803080b0e070603061b061b
       'AdwDrawBasicText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         263           0 RESUME                   0
+         264           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawText')
                        8 STORE_NAME               2 (__qualname__)
          
-         264          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 264>)
+         265          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 265>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawText'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               264           0 RESUME                   0
+               265           0 RESUME                   0
                
-               265           2 LOAD_FAST                0 (self)
+               266           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 264
+               firstlineno 265
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawText'
-         firstlineno 263
+         firstlineno 264
          lnotab 0x0a01
       'AdwDrawText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         268           0 RESUME                   0
+         269           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawDarkText')
                        8 STORE_NAME               2 (__qualname__)
          
-         269          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 269>)
+         270          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 270>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawDarkText'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               269           0 RESUME                   0
+               270           0 RESUME                   0
                
-               270           2 LOAD_FAST                0 (self)
+               271           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 269
+               firstlineno 270
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawDarkText'
-         firstlineno 268
+         firstlineno 269
          lnotab 0x0a01
       'AdwDrawDarkText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
             0a640484015a05640584005a06640684005a07640784005a08640884005a
             09640a88006601640984095a0a880078015a0b5300
                        0 MAKE_CELL                0 (__class__)
          
-         274           2 RESUME                   0
+         275           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundText')
                       10 STORE_NAME               2 (__qualname__)
          
-         275          12 LOAD_CLOSURE             0 (__class__)
+         276          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 275>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 276>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         278          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 278>)
+         279          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 279>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_other)
          
-         281          28 LOAD_CONST              10 ((None,))
-                      30 LOAD_CONST               4 (<code object border_radius, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 281>)
+         282          28 LOAD_CONST              10 ((None,))
+                      30 LOAD_CONST               4 (<code object border_radius, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 282>)
                       32 MAKE_FUNCTION            1 (defaults)
                       34 STORE_NAME               5 (border_radius)
          
-         287          36 LOAD_CONST               5 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 287>)
+         288          36 LOAD_CONST               5 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 288>)
                       38 MAKE_FUNCTION            0
                       40 STORE_NAME               6 (_draw)
          
-         317          42 LOAD_CONST               6 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 317>)
+         318          42 LOAD_CONST               6 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 318>)
                       44 MAKE_FUNCTION            0
                       46 STORE_NAME               7 (default_palette)
          
-         320          48 LOAD_CONST               7 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 320>)
+         321          48 LOAD_CONST               7 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 321>)
                       50 MAKE_FUNCTION            0
                       52 STORE_NAME               8 (palette_light)
          
-         348          54 LOAD_CONST               8 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 348>)
+         349          54 LOAD_CONST               8 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 349>)
                       56 MAKE_FUNCTION            0
                       58 STORE_NAME               9 (palette_dark)
          
-         376          60 LOAD_CONST              10 ((None,))
+         377          60 LOAD_CONST              10 ((None,))
                       62 LOAD_CLOSURE             0 (__class__)
                       64 BUILD_TUPLE              1
-                      66 LOAD_CONST               9 (<code object palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 376>)
+                      66 LOAD_CONST               9 (<code object palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 377>)
                       68 MAKE_FUNCTION            9 (defaults, closure)
                       70 STORE_NAME              10 (palette)
                       72 LOAD_CLOSURE             0 (__class__)
                       74 COPY                     1
                       76 STORE_NAME              11 (__classcell__)
                       78 RETURN_VALUE
          consts
@@ -2597,17 +2604,17 @@
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-               275           2 RESUME                   0
+               276           2 RESUME                   0
                
-               276           4 PUSH_NULL
+               277           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
@@ -2620,29 +2627,29 @@
                   None
                names      ('super', '__init__')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '__init__'
-               firstlineno 275
+               firstlineno 276
                lnotab 0x0401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c006a
                   010000000000000000a00200000000000000000000000000000000000000
                   006401a6010000ab0100000000000000006402ac03a6020000ab02000000
                   0000000000010064005300
-               278           0 RESUME                   0
+               279           0 RESUME                   0
                
-               279           2 LOAD_FAST                0 (self)
+               280           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (configure)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                1 (master)
                             38 LOAD_METHOD              2 (cget)
                             60 LOAD_CONST               1 ('bg')
                             62 PRECALL                  1
                             66 CALL                     1
@@ -2660,48 +2667,48 @@
                   ('background', 'borderwidth')
                names      ('configure', 'master', 'cget')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '_other'
-               firstlineno 278
+               firstlineno 279
                lnotab 0x0201
             None
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               281           0 RESUME                   0
+               282           0 RESUME                   0
                
-               282           2 LOAD_FAST                1 (radius)
+               283           2 LOAD_FAST                1 (radius)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               283           6 LOAD_FAST                0 (self)
+               284           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (button_radius)
                             18 RETURN_VALUE
                
-               285     >>   20 LOAD_FAST                1 (radius)
+               286     >>   20 LOAD_FAST                1 (radius)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (button_radius)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('button_radius',)
                varnames   ('self', 'radius')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'border_radius'
-               firstlineno 281
+               firstlineno 282
                lnotab 0x020104010e02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
@@ -2737,27 +2744,27 @@
                   000000000000000000000000007c006a100000000000000000a6010000ab
                   01000000000000000001007c00a011000000000000000000000000000000
                   00000000007c006a1000000000000000007c006a0c0000000000000000a6
                   020000ab02000000000000000001007c006a0b0000000000000000a01200
                   000000000000000000000000000000000000007c006a0700000000000000
                   007c006a1300000000000000007c006a130000000000000000ac0ba60300
                   00ab030000000000000000010064005300
-               287           0 RESUME                   0
+               288           0 RESUME                   0
                
-               288           2 LOAD_FAST                0 (self)
+               289           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               290          44 LOAD_FAST                0 (self)
+               291          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect2)
                
-               291          68 LOAD_CONST               2 (2)
+               292          68 LOAD_CONST               2 (2)
                             70 LOAD_CONST               2 (2)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (3)
                            112 BINARY_OP               10 (-)
@@ -2766,159 +2773,159 @@
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (3)
                            156 BINARY_OP               10 (-)
                            160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (text_radius)
                
-               292         172 LOAD_FAST                0 (self)
+               293         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (text_border_width)
                
-               293         184 LOAD_FAST                0 (self)
+               294         184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_text_border)
                            196 LOAD_FAST                0 (self)
                            198 LOAD_ATTR                7 (_text_back)
                
-               290         208 KW_NAMES                 4
+               291         208 KW_NAMES                 4
                            210 PRECALL                  8
                            214 CALL                     8
                            224 LOAD_FAST                0 (self)
                            226 STORE_ATTR               8 (text_frame)
                
-               296         236 LOAD_FAST                0 (self)
+               297         236 LOAD_FAST                0 (self)
                            238 LOAD_METHOD              9 (create_window)
                
-               297         260 LOAD_FAST                0 (self)
+               298         260 LOAD_FAST                0 (self)
                            262 LOAD_METHOD              2 (winfo_width)
                            284 PRECALL                  0
                            288 CALL                     0
                            298 LOAD_CONST               2 (2)
                            300 BINARY_OP               11 (/)
                            304 LOAD_FAST                0 (self)
                            306 LOAD_METHOD              3 (winfo_height)
                            328 PRECALL                  0
                            332 CALL                     0
                            342 LOAD_CONST               2 (2)
                            344 BINARY_OP               11 (/)
                
-               298         348 LOAD_FAST                0 (self)
+               299         348 LOAD_FAST                0 (self)
                            350 LOAD_METHOD              2 (winfo_width)
                            372 PRECALL                  0
                            376 CALL                     0
                            386 LOAD_FAST                0 (self)
                            388 LOAD_ATTR                5 (text_border_width)
                            398 BINARY_OP               10 (-)
                            402 LOAD_CONST               5 (5)
                            404 BINARY_OP               10 (-)
                            408 LOAD_FAST                0 (self)
                            410 LOAD_ATTR               10 (text_padding)
                            420 LOAD_CONST               6 (0)
                            422 BINARY_SUBSCR
                            432 BINARY_OP               10 (-)
                
-               299         436 LOAD_FAST                0 (self)
+               300         436 LOAD_FAST                0 (self)
                            438 LOAD_METHOD              3 (winfo_height)
                            460 PRECALL                  0
                            464 CALL                     0
                            474 LOAD_FAST                0 (self)
                            476 LOAD_ATTR                5 (text_border_width)
                            486 BINARY_OP               10 (-)
                            490 LOAD_CONST               5 (5)
                            492 BINARY_OP               10 (-)
                            496 LOAD_FAST                0 (self)
                            498 LOAD_ATTR               10 (text_padding)
                            508 LOAD_CONST               7 (1)
                            510 BINARY_SUBSCR
                            520 BINARY_OP               10 (-)
                
-               300         524 LOAD_FAST                0 (self)
+               301         524 LOAD_FAST                0 (self)
                            526 LOAD_ATTR               11 (text)
                
-               296         536 KW_NAMES                 8
+               297         536 KW_NAMES                 8
                            538 PRECALL                  5
                            542 CALL                     5
                            552 LOAD_FAST                0 (self)
                            554 STORE_ATTR              12 (text_text)
                
-               303         564 LOAD_FAST                0 (self)
+               304         564 LOAD_FAST                0 (self)
                            566 LOAD_METHOD             13 (create_rectangle)
                            588 LOAD_CONST               3 (3)
                            590 LOAD_FAST                0 (self)
                            592 LOAD_ATTR                4 (text_radius)
                            602 LOAD_CONST               2 (2)
                            604 BINARY_OP               11 (/)
                            608 BINARY_OP                0 (+)
                
-               304         612 LOAD_FAST                0 (self)
+               305         612 LOAD_FAST                0 (self)
                            614 LOAD_METHOD              3 (winfo_height)
                            636 PRECALL                  0
                            640 CALL                     0
                            650 LOAD_FAST                0 (self)
                            652 LOAD_ATTR               14 (_text_bottom_width)
                            662 BINARY_OP               10 (-)
                            666 LOAD_CONST               3 (3)
                            668 BINARY_OP               10 (-)
                
-               305         672 LOAD_FAST                0 (self)
+               306         672 LOAD_FAST                0 (self)
                            674 LOAD_METHOD              2 (winfo_width)
                            696 PRECALL                  0
                            700 CALL                     0
                            710 LOAD_CONST               3 (3)
                            712 BINARY_OP               10 (-)
                            716 LOAD_FAST                0 (self)
                            718 LOAD_ATTR                4 (text_radius)
                            728 LOAD_CONST               2 (2)
                            730 BINARY_OP               11 (/)
                            734 BINARY_OP               10 (-)
                
-               306         738 LOAD_FAST                0 (self)
+               307         738 LOAD_FAST                0 (self)
                            740 LOAD_METHOD              3 (winfo_height)
                            762 PRECALL                  0
                            766 CALL                     0
                            776 LOAD_CONST               9 (3.5)
                            778 BINARY_OP               10 (-)
                
-               307         782 LOAD_FAST                0 (self)
+               308         782 LOAD_FAST                0 (self)
                            784 LOAD_ATTR               15 (_text_bottom_line)
                            794 LOAD_FAST                0 (self)
                            796 LOAD_ATTR               15 (_text_bottom_line)
                
-               308         806 LOAD_CONST               6 (0)
+               309         806 LOAD_CONST               6 (0)
                
-               303         808 KW_NAMES                10
+               304         808 KW_NAMES                10
                            810 PRECALL                  7
                            814 CALL                     7
                            824 LOAD_FAST                0 (self)
                            826 STORE_ATTR              16 (text_bottom)
                
-               310         836 LOAD_FAST                0 (self)
+               311         836 LOAD_FAST                0 (self)
                            838 LOAD_ATTR               14 (_text_bottom_width)
                            848 LOAD_CONST               6 (0)
                            850 COMPARE_OP               2 (==)
                            856 POP_JUMP_FORWARD_IF_FALSE    26 (to 910)
                
-               311         858 LOAD_FAST                0 (self)
+               312         858 LOAD_FAST                0 (self)
                            860 LOAD_METHOD              0 (delete)
                            882 LOAD_FAST                0 (self)
                            884 LOAD_ATTR               16 (text_bottom)
                            894 PRECALL                  1
                            898 CALL                     1
                            908 POP_TOP
                
-               313     >>  910 LOAD_FAST                0 (self)
+               314     >>  910 LOAD_FAST                0 (self)
                            912 LOAD_METHOD             17 (tag_raise)
                            934 LOAD_FAST                0 (self)
                            936 LOAD_ATTR               16 (text_bottom)
                            946 LOAD_FAST                0 (self)
                            948 LOAD_ATTR               12 (text_text)
                            958 PRECALL                  2
                            962 CALL                     2
                            972 POP_TOP
                
-               315         974 LOAD_FAST                0 (self)
+               316         974 LOAD_FAST                0 (self)
                            976 LOAD_ATTR               11 (text)
                            986 LOAD_METHOD             18 (configure)
                           1008 LOAD_FAST                0 (self)
                           1010 LOAD_ATTR                7 (_text_back)
                           1020 LOAD_FAST                0 (self)
                           1022 LOAD_ATTR               19 (_text_text_back)
                           1032 LOAD_FAST                0 (self)
@@ -2944,98 +2951,98 @@
                   ('background', 'foreground', 'insertbackground')
                names      ('delete', 'create_round_rect2', 'winfo_width', 'winfo_height', 'text_radius', 'text_border_width', '_text_border', '_text_back', 'text_frame', 'create_window', 'text_padding', 'text', 'text_text', 'create_rectangle', '_text_bottom_width', '_text_bottom_line', 'text_bottom', 'tag_raise', 'configure', '_text_text_back')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '_draw'
-               firstlineno 287
+               firstlineno 288
                lnotab
                   0x02012a02180168010c0118fd1c0618015801580158010cfc1c0730013c
                   0142012c01180102fb1c07160134024002
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               317           0 RESUME                   0
+               318           0 RESUME                   0
                
-               318           2 LOAD_FAST                0 (self)
+               319           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 317
+               firstlineno 318
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 18
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066407640564086409640a640b6407640c640d640e9c
                   06640f9c096901a6010000ab010000000000000000010064005300
-               320           0 RESUME                   0
+               321           0 RESUME                   0
                
-               321           2 LOAD_FAST                0 (self)
+               322           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               323          26 LOAD_CONST               1 ('text')
+               324          26 LOAD_CONST               1 ('text')
                
-               324          28 LOAD_CONST               2 (6)
+               325          28 LOAD_CONST               2 (6)
                
-               325          30 LOAD_CONST               3 ((3, 4))
+               326          30 LOAD_CONST               3 ((3, 4))
                
-               327          32 LOAD_CONST               4 ('#fdfdfd')
+               328          32 LOAD_CONST               4 ('#fdfdfd')
                
-               328          34 LOAD_CONST               5 ('#eaeaea')
+               329          34 LOAD_CONST               5 ('#eaeaea')
                
-               329          36 LOAD_CONST               6 ('#5f5f5f')
+               330          36 LOAD_CONST               6 ('#5f5f5f')
                
-               330          38 LOAD_CONST               7 (1)
+               331          38 LOAD_CONST               7 (1)
                
-               332          40 LOAD_CONST               5 ('#eaeaea')
+               333          40 LOAD_CONST               5 ('#eaeaea')
                
-               333          42 LOAD_CONST               8 (0)
+               334          42 LOAD_CONST               8 (0)
                
-               336          44 LOAD_CONST               9 ('#f9f9f9')
+               337          44 LOAD_CONST               9 ('#f9f9f9')
                
-               337          46 LOAD_CONST              10 ('#e2e2e2')
+               338          46 LOAD_CONST              10 ('#e2e2e2')
                
-               338          48 LOAD_CONST              11 ('#1a1a1a')
+               339          48 LOAD_CONST              11 ('#1a1a1a')
                
-               339          50 LOAD_CONST               7 (1)
+               340          50 LOAD_CONST               7 (1)
                
-               341          52 LOAD_CONST              12 ('#185fb4')
+               342          52 LOAD_CONST              12 ('#185fb4')
                
-               342          54 LOAD_CONST              13 (2)
+               343          54 LOAD_CONST              13 (2)
                
-               335          56 LOAD_CONST              14 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               336          56 LOAD_CONST              14 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
                             58 BUILD_CONST_KEY_MAP      6
                
-               323          60 LOAD_CONST              15 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               324          60 LOAD_CONST              15 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
                             62 BUILD_CONST_KEY_MAP      9
                
-               322          64 BUILD_MAP                1
+               323          64 BUILD_MAP                1
                
-               321          66 PRECALL                  1
+               322          66 PRECALL                  1
                             70 CALL                     1
                             80 POP_TOP
                             82 LOAD_CONST               0 (None)
                             84 RETURN_VALUE
                consts
                   None
                   'text'
@@ -3055,71 +3062,71 @@
                   ('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'palette_light'
-               firstlineno 320
+               firstlineno 321
                lnotab
                   0x0201180202010201020202010201020102020201020302010201020102
                   02020102f904f404ff02ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 18
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   026403640464056406640764086409640a640564086407640b640c640d9c
                   06640e9c096901a6010000ab010000000000000000010064005300
-               348           0 RESUME                   0
+               349           0 RESUME                   0
                
-               349           2 LOAD_FAST                0 (self)
+               350           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               351          26 LOAD_CONST               1 ('text')
+               352          26 LOAD_CONST               1 ('text')
                
-               352          28 LOAD_CONST               2 (6)
+               353          28 LOAD_CONST               2 (6)
                
-               353          30 LOAD_CONST               3 ((3, 4))
+               354          30 LOAD_CONST               3 ((3, 4))
                
-               355          32 LOAD_CONST               4 ('#353535')
+               356          32 LOAD_CONST               4 ('#353535')
                
-               356          34 LOAD_CONST               5 ('#454545')
+               357          34 LOAD_CONST               5 ('#454545')
                
-               357          36 LOAD_CONST               6 ('#cecece')
+               358          36 LOAD_CONST               6 ('#cecece')
                
-               358          38 LOAD_CONST               7 (1)
+               359          38 LOAD_CONST               7 (1)
                
-               360          40 LOAD_CONST               8 ('#ffffff')
+               361          40 LOAD_CONST               8 ('#ffffff')
                
-               361          42 LOAD_CONST               9 (0)
+               362          42 LOAD_CONST               9 (0)
                
-               364          44 LOAD_CONST              10 ('#2f2f2f')
+               365          44 LOAD_CONST              10 ('#2f2f2f')
                
-               365          46 LOAD_CONST               5 ('#454545')
+               366          46 LOAD_CONST               5 ('#454545')
                
-               366          48 LOAD_CONST               8 ('#ffffff')
+               367          48 LOAD_CONST               8 ('#ffffff')
                
-               367          50 LOAD_CONST               7 (1)
+               368          50 LOAD_CONST               7 (1)
                
-               369          52 LOAD_CONST              11 ('#4cc2ff')
+               370          52 LOAD_CONST              11 ('#4cc2ff')
                
-               370          54 LOAD_CONST              12 (2)
+               371          54 LOAD_CONST              12 (2)
                
-               363          56 LOAD_CONST              13 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               364          56 LOAD_CONST              13 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
                             58 BUILD_CONST_KEY_MAP      6
                
-               351          60 LOAD_CONST              14 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               352          60 LOAD_CONST              14 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
                             62 BUILD_CONST_KEY_MAP      9
                
-               350          64 BUILD_MAP                1
+               351          64 BUILD_MAP                1
                
-               349          66 PRECALL                  1
+               350          66 PRECALL                  1
                             70 CALL                     1
                             80 POP_TOP
                             82 LOAD_CONST               0 (None)
                             84 RETURN_VALUE
                consts
                   None
                   'text'
@@ -3138,15 +3145,15 @@
                   ('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'palette_dark'
-               firstlineno 348
+               firstlineno 349
                lnotab
                   0x0201180202010201020202010201020102020201020302010201020102
                   02020102f904f404ff02ff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
@@ -3155,221 +3162,221 @@
                   0x95019700740100000000000000000000a6000000ab0000000000000000
                   00a00100000000000000000000000000000000000000007c01a6010000ab
                   010000000000000000010064017c01760072157c01640119000000000000
                   0000006402190000000000000000007c005f020000000000000000640053
                   0064005300
                              0 COPY_FREE_VARS           1
                
-               376           2 RESUME                   0
+               377           2 RESUME                   0
                
-               377           4 LOAD_GLOBAL              1 (NULL + super)
+               378           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (palette)
                             52 LOAD_FAST                1 (dict)
                             54 PRECALL                  1
                             58 CALL                     1
                             68 POP_TOP
                
-               378          70 LOAD_CONST               1 ('text')
+               379          70 LOAD_CONST               1 ('text')
                             72 LOAD_FAST                1 (dict)
                             74 CONTAINS_OP              0
                             76 POP_JUMP_FORWARD_IF_FALSE    21 (to 120)
                
-               379          78 LOAD_FAST                1 (dict)
+               380          78 LOAD_FAST                1 (dict)
                             80 LOAD_CONST               1 ('text')
                             82 BINARY_SUBSCR
                             92 LOAD_CONST               2 ('radius')
                             94 BINARY_SUBSCR
                            104 LOAD_FAST                0 (self)
                            106 STORE_ATTR               2 (text_radius)
                            116 LOAD_CONST               0 (None)
                            118 RETURN_VALUE
                
-               378     >>  120 LOAD_CONST               0 (None)
+               379     >>  120 LOAD_CONST               0 (None)
                            122 RETURN_VALUE
                consts
                   None
                   'text'
                   'radius'
                names      ('super', 'palette', 'text_radius')
                varnames   ('self', 'dict')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'palette'
-               firstlineno 376
+               firstlineno 377
                lnotab 0x0401420108012aff
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'border_radius', '_draw', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawBasicRoundText'
-         firstlineno 274
+         firstlineno 275
          lnotab 0x0c010a0306030806061e0603061c061c
       'AdwDrawBasicRoundText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         382           0 RESUME                   0
+         383           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundText')
                        8 STORE_NAME               2 (__qualname__)
          
-         383          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 383>)
+         384          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 384>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundText'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               383           0 RESUME                   0
+               384           0 RESUME                   0
                
-               384           2 LOAD_FAST                0 (self)
+               385           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 383
+               firstlineno 384
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawRoundText'
-         firstlineno 382
+         firstlineno 383
          lnotab 0x0a01
       'AdwDrawRoundText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         387           0 RESUME                   0
+         388           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkText')
                        8 STORE_NAME               2 (__qualname__)
          
-         388          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 388>)
+         389          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 389>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkText'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               388           0 RESUME                   0
+               389           0 RESUME                   0
                
-               389           2 LOAD_FAST                0 (self)
+               390           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 388
+               firstlineno 389
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawRoundDarkText'
-         firstlineno 387
+         firstlineno 388
          lnotab 0x0a01
       'AdwDrawRoundDarkText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
             09640484015a05640584005a06640684005a07640784005a08640884005a
             09880078015a0a5300
                        0 MAKE_CELL                0 (__class__)
          
-         392           2 RESUME                   0
+         393           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundText3')
                       10 STORE_NAME               2 (__qualname__)
          
-         393          12 LOAD_CLOSURE             0 (__class__)
+         394          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 393>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 394>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         396          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 396>)
+         397          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 397>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_other)
          
-         399          28 LOAD_CONST               9 ((None,))
-                      30 LOAD_CONST               4 (<code object border_radius, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 399>)
+         400          28 LOAD_CONST               9 ((None,))
+                      30 LOAD_CONST               4 (<code object border_radius, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 400>)
                       32 MAKE_FUNCTION            1 (defaults)
                       34 STORE_NAME               5 (border_radius)
          
-         405          36 LOAD_CONST               5 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 405>)
+         406          36 LOAD_CONST               5 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 406>)
                       38 MAKE_FUNCTION            0
                       40 STORE_NAME               6 (_draw)
          
-         441          42 LOAD_CONST               6 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 441>)
+         442          42 LOAD_CONST               6 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 442>)
                       44 MAKE_FUNCTION            0
                       46 STORE_NAME               7 (default_palette)
          
-         444          48 LOAD_CONST               7 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 444>)
+         445          48 LOAD_CONST               7 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 445>)
                       50 MAKE_FUNCTION            0
                       52 STORE_NAME               8 (palette_light)
          
-         472          54 LOAD_CONST               8 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 472>)
+         473          54 LOAD_CONST               8 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 473>)
                       56 MAKE_FUNCTION            0
                       58 STORE_NAME               9 (palette_dark)
                       60 LOAD_CLOSURE             0 (__class__)
                       62 COPY                     1
                       64 STORE_NAME              10 (__classcell__)
                       66 RETURN_VALUE
          consts
@@ -3380,17 +3387,17 @@
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-               393           2 RESUME                   0
+               394           2 RESUME                   0
                
-               394           4 PUSH_NULL
+               395           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
@@ -3403,29 +3410,29 @@
                   None
                names      ('super', '__init__')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '__init__'
-               firstlineno 393
+               firstlineno 394
                lnotab 0x0401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c006a
                   010000000000000000a00200000000000000000000000000000000000000
                   006401a6010000ab0100000000000000006402ac03a6020000ab02000000
                   0000000000010064005300
-               396           0 RESUME                   0
+               397           0 RESUME                   0
                
-               397           2 LOAD_FAST                0 (self)
+               398           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (configure)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                1 (master)
                             38 LOAD_METHOD              2 (cget)
                             60 LOAD_CONST               1 ('bg')
                             62 PRECALL                  1
                             66 CALL                     1
@@ -3443,48 +3450,48 @@
                   ('background', 'borderwidth')
                names      ('configure', 'master', 'cget')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '_other'
-               firstlineno 396
+               firstlineno 397
                lnotab 0x0201
             None
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               399           0 RESUME                   0
+               400           0 RESUME                   0
                
-               400           2 LOAD_FAST                1 (radius)
+               401           2 LOAD_FAST                1 (radius)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               401           6 LOAD_FAST                0 (self)
+               402           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (button_radius)
                             18 RETURN_VALUE
                
-               403     >>   20 LOAD_FAST                1 (radius)
+               404     >>   20 LOAD_FAST                1 (radius)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (button_radius)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('button_radius',)
                varnames   ('self', 'radius')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'border_radius'
-               firstlineno 399
+               firstlineno 400
                lnotab 0x020104010e02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
@@ -3520,195 +3527,195 @@
                   00000000000000000000000000000000007c006a100000000000000000a6
                   010000ab01000000000000000001007c00a0110000000000000000000000
                   0000000000000000007c006a1000000000000000007c006a0c0000000000
                   000000a6020000ab02000000000000000001007c006a0b00000000000000
                   00a01200000000000000000000000000000000000000007c006a07000000
                   00000000007c006a1300000000000000007c006a130000000000000000ac
                   0aa6030000ab030000000000000000010064005300
-               405           0 RESUME                   0
+               406           0 RESUME                   0
                
-               406           2 LOAD_FAST                0 (self)
+               407           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               408          44 LOAD_FAST                0 (self)
+               409          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect4)
                
-               409          68 LOAD_CONST               2 (0)
+               410          68 LOAD_CONST               2 (0)
                
-               410          70 LOAD_CONST               2 (0)
+               411          70 LOAD_CONST               2 (0)
                
-               411          72 LOAD_FAST                0 (self)
+               412          72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (1)
                            112 BINARY_OP               10 (-)
                
-               412         116 LOAD_FAST                0 (self)
+               413         116 LOAD_FAST                0 (self)
                            118 LOAD_METHOD              3 (winfo_height)
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (1)
                            156 BINARY_OP               10 (-)
                
-               413         160 LOAD_FAST                0 (self)
+               414         160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (text_radius)
                
-               414         172 LOAD_FAST                0 (self)
+               415         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (text_border_width)
                
-               415         184 LOAD_FAST                0 (self)
+               416         184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_text_border)
                            196 LOAD_FAST                0 (self)
                            198 LOAD_ATTR                7 (_text_back)
                
-               408         208 KW_NAMES                 4
+               409         208 KW_NAMES                 4
                            210 PRECALL                  8
                            214 CALL                     8
                            224 POP_TOP
                
-               418         226 LOAD_CONST               5 ('button_frame')
+               419         226 LOAD_CONST               5 ('button_frame')
                            228 LOAD_FAST                0 (self)
                            230 STORE_ATTR               8 (text_frame)
                
-               420         240 LOAD_FAST                0 (self)
+               421         240 LOAD_FAST                0 (self)
                            242 LOAD_METHOD              9 (create_window)
                
-               421         264 LOAD_FAST                0 (self)
+               422         264 LOAD_FAST                0 (self)
                            266 LOAD_METHOD              2 (winfo_width)
                            288 PRECALL                  0
                            292 CALL                     0
                            302 LOAD_CONST               6 (2)
                            304 BINARY_OP               11 (/)
                            308 LOAD_FAST                0 (self)
                            310 LOAD_METHOD              3 (winfo_height)
                            332 PRECALL                  0
                            336 CALL                     0
                            346 LOAD_CONST               6 (2)
                            348 BINARY_OP               11 (/)
                
-               422         352 LOAD_FAST                0 (self)
+               423         352 LOAD_FAST                0 (self)
                            354 LOAD_METHOD              2 (winfo_width)
                            376 PRECALL                  0
                            380 CALL                     0
                            390 LOAD_FAST                0 (self)
                            392 LOAD_ATTR                5 (text_border_width)
                            402 BINARY_OP               10 (-)
                            406 LOAD_FAST                0 (self)
                            408 LOAD_ATTR               10 (text_padding)
                            418 LOAD_CONST               2 (0)
                            420 BINARY_SUBSCR
                            430 BINARY_OP               10 (-)
                            434 LOAD_CONST               6 (2)
                            436 BINARY_OP               10 (-)
                
-               423         440 LOAD_FAST                0 (self)
+               424         440 LOAD_FAST                0 (self)
                            442 LOAD_METHOD              3 (winfo_height)
                            464 PRECALL                  0
                            468 CALL                     0
                            478 LOAD_FAST                0 (self)
                            480 LOAD_ATTR                5 (text_border_width)
                            490 BINARY_OP               10 (-)
                            494 LOAD_FAST                0 (self)
                            496 LOAD_ATTR               10 (text_padding)
                            506 LOAD_CONST               3 (1)
                            508 BINARY_SUBSCR
                            518 BINARY_OP               10 (-)
                            522 LOAD_CONST               6 (2)
                            524 BINARY_OP               10 (-)
                
-               424         528 LOAD_FAST                0 (self)
+               425         528 LOAD_FAST                0 (self)
                            530 LOAD_ATTR               11 (text)
                
-               420         540 KW_NAMES                 7
+               421         540 KW_NAMES                 7
                            542 PRECALL                  5
                            546 CALL                     5
                            556 LOAD_FAST                0 (self)
                            558 STORE_ATTR              12 (text_text)
                
-               427         568 LOAD_FAST                0 (self)
+               428         568 LOAD_FAST                0 (self)
                            570 LOAD_METHOD             13 (create_rectangle)
                            592 LOAD_CONST               3 (1)
                            594 LOAD_FAST                0 (self)
                            596 LOAD_ATTR                4 (text_radius)
                            606 LOAD_CONST               8 (5)
                            608 BINARY_OP               11 (/)
                            612 BINARY_OP                0 (+)
                
-               428         616 LOAD_FAST                0 (self)
+               429         616 LOAD_FAST                0 (self)
                            618 LOAD_METHOD              3 (winfo_height)
                            640 PRECALL                  0
                            644 CALL                     0
                            654 LOAD_FAST                0 (self)
                            656 LOAD_ATTR               14 (_text_bottom_width)
                            666 BINARY_OP               10 (-)
                            670 LOAD_CONST               3 (1)
                            672 BINARY_OP               10 (-)
                
-               429         676 LOAD_FAST                0 (self)
+               430         676 LOAD_FAST                0 (self)
                            678 LOAD_METHOD              2 (winfo_width)
                            700 PRECALL                  0
                            704 CALL                     0
                            714 LOAD_CONST               3 (1)
                            716 BINARY_OP               10 (-)
                            720 LOAD_FAST                0 (self)
                            722 LOAD_ATTR                4 (text_radius)
                            732 LOAD_CONST               8 (5)
                            734 BINARY_OP               11 (/)
                            738 BINARY_OP               10 (-)
                
-               430         742 LOAD_FAST                0 (self)
+               431         742 LOAD_FAST                0 (self)
                            744 LOAD_METHOD              3 (winfo_height)
                            766 PRECALL                  0
                            770 CALL                     0
                            780 LOAD_CONST               3 (1)
                            782 BINARY_OP               10 (-)
                
-               431         786 LOAD_FAST                0 (self)
+               432         786 LOAD_FAST                0 (self)
                            788 LOAD_ATTR               15 (_text_bottom_line)
                            798 LOAD_FAST                0 (self)
                            800 LOAD_ATTR               15 (_text_bottom_line)
                
-               432         810 LOAD_CONST               2 (0)
+               433         810 LOAD_CONST               2 (0)
                
-               427         812 KW_NAMES                 9
+               428         812 KW_NAMES                 9
                            814 PRECALL                  7
                            818 CALL                     7
                            828 LOAD_FAST                0 (self)
                            830 STORE_ATTR              16 (text_bottom)
                
-               434         840 LOAD_FAST                0 (self)
+               435         840 LOAD_FAST                0 (self)
                            842 LOAD_ATTR               14 (_text_bottom_width)
                            852 LOAD_CONST               2 (0)
                            854 COMPARE_OP               2 (==)
                            860 POP_JUMP_FORWARD_IF_FALSE    26 (to 914)
                
-               435         862 LOAD_FAST                0 (self)
+               436         862 LOAD_FAST                0 (self)
                            864 LOAD_METHOD              0 (delete)
                            886 LOAD_FAST                0 (self)
                            888 LOAD_ATTR               16 (text_bottom)
                            898 PRECALL                  1
                            902 CALL                     1
                            912 POP_TOP
                
-               437     >>  914 LOAD_FAST                0 (self)
+               438     >>  914 LOAD_FAST                0 (self)
                            916 LOAD_METHOD             17 (tag_raise)
                            938 LOAD_FAST                0 (self)
                            940 LOAD_ATTR               16 (text_bottom)
                            950 LOAD_FAST                0 (self)
                            952 LOAD_ATTR               12 (text_text)
                            962 PRECALL                  2
                            966 CALL                     2
                            976 POP_TOP
                
-               439         978 LOAD_FAST                0 (self)
+               440         978 LOAD_FAST                0 (self)
                            980 LOAD_ATTR               11 (text)
                            990 LOAD_METHOD             18 (configure)
                           1012 LOAD_FAST                0 (self)
                           1014 LOAD_ATTR                7 (_text_back)
                           1024 LOAD_FAST                0 (self)
                           1026 LOAD_ATTR               19 (_text_text_back)
                           1036 LOAD_FAST                0 (self)
@@ -3733,98 +3740,98 @@
                   ('background', 'foreground', 'insertbackground')
                names      ('delete', 'create_round_rect4', 'winfo_width', 'winfo_height', 'text_radius', 'text_border_width', '_text_border', '_text_back', 'text_frame', 'create_window', 'text_padding', 'text', 'text_text', 'create_rectangle', '_text_bottom_width', '_text_bottom_line', 'text_bottom', 'tag_raise', 'configure', '_text_text_back')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '_draw'
-               firstlineno 405
+               firstlineno 406
                lnotab
                   0x02012a021801020102012c012c010c010c0118f9120a0e021801580158
                   0158010cfc1c0730013c0142012c01180102fb1c07160134024002
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               441           0 RESUME                   0
+               442           0 RESUME                   0
                
-               442           2 LOAD_FAST                0 (self)
+               443           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 441
+               firstlineno 442
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 18
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066407640564086409640a640b6407640c640d640e9c
                   06640f9c096901a6010000ab010000000000000000010064005300
-               444           0 RESUME                   0
+               445           0 RESUME                   0
                
-               445           2 LOAD_FAST                0 (self)
+               446           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               447          26 LOAD_CONST               1 ('text')
+               448          26 LOAD_CONST               1 ('text')
                
-               448          28 LOAD_CONST               2 (6)
+               449          28 LOAD_CONST               2 (6)
                
-               449          30 LOAD_CONST               3 ((3, 4))
+               450          30 LOAD_CONST               3 ((3, 4))
                
-               451          32 LOAD_CONST               4 ('#fdfdfd')
+               452          32 LOAD_CONST               4 ('#fdfdfd')
                
-               452          34 LOAD_CONST               5 ('#eaeaea')
+               453          34 LOAD_CONST               5 ('#eaeaea')
                
-               453          36 LOAD_CONST               6 ('#5f5f5f')
+               454          36 LOAD_CONST               6 ('#5f5f5f')
                
-               454          38 LOAD_CONST               7 (1)
+               455          38 LOAD_CONST               7 (1)
                
-               456          40 LOAD_CONST               5 ('#eaeaea')
+               457          40 LOAD_CONST               5 ('#eaeaea')
                
-               457          42 LOAD_CONST               8 (0)
+               458          42 LOAD_CONST               8 (0)
                
-               460          44 LOAD_CONST               9 ('#f9f9f9')
+               461          44 LOAD_CONST               9 ('#f9f9f9')
                
-               461          46 LOAD_CONST              10 ('#e2e2e2')
+               462          46 LOAD_CONST              10 ('#e2e2e2')
                
-               462          48 LOAD_CONST              11 ('#1a1a1a')
+               463          48 LOAD_CONST              11 ('#1a1a1a')
                
-               463          50 LOAD_CONST               7 (1)
+               464          50 LOAD_CONST               7 (1)
                
-               465          52 LOAD_CONST              12 ('#185fb4')
+               466          52 LOAD_CONST              12 ('#185fb4')
                
-               466          54 LOAD_CONST              13 (2)
+               467          54 LOAD_CONST              13 (2)
                
-               459          56 LOAD_CONST              14 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               460          56 LOAD_CONST              14 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
                             58 BUILD_CONST_KEY_MAP      6
                
-               447          60 LOAD_CONST              15 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               448          60 LOAD_CONST              15 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
                             62 BUILD_CONST_KEY_MAP      9
                
-               446          64 BUILD_MAP                1
+               447          64 BUILD_MAP                1
                
-               445          66 PRECALL                  1
+               446          66 PRECALL                  1
                             70 CALL                     1
                             80 POP_TOP
                             82 LOAD_CONST               0 (None)
                             84 RETURN_VALUE
                consts
                   None
                   'text'
@@ -3844,71 +3851,71 @@
                   ('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'palette_light'
-               firstlineno 444
+               firstlineno 445
                lnotab
                   0x0201180202010201020202010201020102020201020302010201020102
                   02020102f904f404ff02ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 18
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   026403640464056406640764086409640a640564086407640b640c640d9c
                   06640e9c096901a6010000ab010000000000000000010064005300
-               472           0 RESUME                   0
+               473           0 RESUME                   0
                
-               473           2 LOAD_FAST                0 (self)
+               474           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               475          26 LOAD_CONST               1 ('text')
+               476          26 LOAD_CONST               1 ('text')
                
-               476          28 LOAD_CONST               2 (6)
+               477          28 LOAD_CONST               2 (6)
                
-               477          30 LOAD_CONST               3 ((3, 4))
+               478          30 LOAD_CONST               3 ((3, 4))
                
-               479          32 LOAD_CONST               4 ('#353535')
+               480          32 LOAD_CONST               4 ('#353535')
                
-               480          34 LOAD_CONST               5 ('#454545')
+               481          34 LOAD_CONST               5 ('#454545')
                
-               481          36 LOAD_CONST               6 ('#cecece')
+               482          36 LOAD_CONST               6 ('#cecece')
                
-               482          38 LOAD_CONST               7 (1)
+               483          38 LOAD_CONST               7 (1)
                
-               484          40 LOAD_CONST               8 ('#ffffff')
+               485          40 LOAD_CONST               8 ('#ffffff')
                
-               485          42 LOAD_CONST               9 (0)
+               486          42 LOAD_CONST               9 (0)
                
-               488          44 LOAD_CONST              10 ('#2f2f2f')
+               489          44 LOAD_CONST              10 ('#2f2f2f')
                
-               489          46 LOAD_CONST               5 ('#454545')
+               490          46 LOAD_CONST               5 ('#454545')
                
-               490          48 LOAD_CONST               8 ('#ffffff')
+               491          48 LOAD_CONST               8 ('#ffffff')
                
-               491          50 LOAD_CONST               7 (1)
+               492          50 LOAD_CONST               7 (1)
                
-               493          52 LOAD_CONST              11 ('#4cc2ff')
+               494          52 LOAD_CONST              11 ('#4cc2ff')
                
-               494          54 LOAD_CONST              12 (2)
+               495          54 LOAD_CONST              12 (2)
                
-               487          56 LOAD_CONST              13 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               488          56 LOAD_CONST              13 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
                             58 BUILD_CONST_KEY_MAP      6
                
-               475          60 LOAD_CONST              14 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               476          60 LOAD_CONST              14 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
                             62 BUILD_CONST_KEY_MAP      9
                
-               474          64 BUILD_MAP                1
+               475          64 BUILD_MAP                1
                
-               473          66 PRECALL                  1
+               474          66 PRECALL                  1
                             70 CALL                     1
                             80 POP_TOP
                             82 LOAD_CONST               0 (None)
                             84 RETURN_VALUE
                consts
                   None
                   'text'
@@ -3927,150 +3934,150 @@
                   ('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'palette_dark'
-               firstlineno 472
+               firstlineno 473
                lnotab
                   0x0201180202010201020202010201020102020201020302010201020102
                   02020102f904f404ff02ff
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'border_radius', '_draw', 'default_palette', 'palette_light', 'palette_dark', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawBasicRoundText3'
-         firstlineno 392
+         firstlineno 393
          lnotab 0x0c010a030603080606240603061c
       'AdwDrawBasicRoundText3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         501           0 RESUME                   0
+         502           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundText3')
                        8 STORE_NAME               2 (__qualname__)
          
-         502          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 502>)
+         503          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 503>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundText3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               502           0 RESUME                   0
+               503           0 RESUME                   0
                
-               503           2 LOAD_FAST                0 (self)
+               504           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 502
+               firstlineno 503
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawRoundText3'
-         firstlineno 501
+         firstlineno 502
          lnotab 0x0a01
       'AdwDrawRoundText3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         506           0 RESUME                   0
+         507           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkText3')
                        8 STORE_NAME               2 (__qualname__)
          
-         507          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 507>)
+         508          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 508>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkText3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               507           0 RESUME                   0
+               508           0 RESUME                   0
                
-               508           2 LOAD_FAST                0 (self)
+               509           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 507
+               firstlineno 508
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawRoundDarkText3'
-         firstlineno 506
+         firstlineno 507
          lnotab 0x0a01
       'AdwDrawRoundDarkText3'
       '__main__'
       ('Tk',)
       'x'
       5
       ('fill', 'padx', 'pady')
       None
-   names      ('tkinter.font', 'Font', 'nametofont', 'tkadw.windows.canvas.drawengine', 'AdwDrawEngine', 'AdwDrawBasicText', 'AdwDrawText', 'AdwDrawDarkText', 'AdwDrawBasicRoundText', 'AdwDrawRoundText', 'AdwDrawRoundDarkText', 'AdwDrawBasicRoundText3', 'AdwDrawRoundText3', 'AdwDrawRoundDarkText3', '__name__', 'tkinter', 'Tk', 'root', 'text1', 'pack', 'text2', 'text3', 'text4', 'text5', 'text6', 'mainloop')
+   names      ('tkinter.font', 'Font', 'nametofont', 'tkadw.windows.canvas.widget', 'AdwWidget', 'AdwDrawBasicText', 'AdwDrawText', 'AdwDrawDarkText', 'AdwDrawBasicRoundText', 'AdwDrawRoundText', 'AdwDrawRoundDarkText', 'AdwDrawBasicRoundText3', 'AdwDrawRoundText3', 'AdwDrawRoundDarkText3', '__name__', 'tkinter', 'Tk', 'root', 'text1', 'pack', 'text2', 'text3', 'text4', 'text5', 'text6', 'mainloop')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020110010c041c7f007f00031c051c061c6c1c051c051c6d1c051c
+      0x00ff020110010c041c7f007f00041c051c061c6c1c051c051c6d1c051c
       050c010c0214021401300214013002140130021401300214013002140130
       022ce9
```

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/widget.cpython-310.pyc` & `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/widget.cpython-311.pyc` & `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/widget.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xc6e3b064 (Fri Jul 14 05:57:26 2023 UTC)
-files sz: 520
+moddate:  0xc73ab364 (Sun Jul 16 00:33:11 2023 UTC)
+files sz: 782
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100020047006402840064036501a60300
@@ -31,19 +31,20 @@
                 44 RETURN_VALUE
    consts
       0
       ('AdwDrawEngine',)
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 2
+         stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0388006601640284085a04640384
-            005a056406640584015a06880078015a075300
+            005a056408880066016406840c5a066409640784015a07880078015a0853
+            00
                        0 MAKE_CELL                0 (__class__)
          
            4           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwWidget')
                       10 STORE_NAME               2 (__qualname__)
@@ -57,22 +58,29 @@
                       22 MAKE_FUNCTION            8 (closure)
                       24 STORE_NAME               4 (__init__)
          
           18          26 LOAD_CONST               3 (<code object _other, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 18>)
                       28 MAKE_FUNCTION            0
                       30 STORE_NAME               5 (_other)
          
-          21          32 LOAD_CONST               6 ((None,))
-                      34 LOAD_CONST               5 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 21>)
-                      36 MAKE_FUNCTION            1 (defaults)
-                      38 STORE_NAME               6 (_draw)
-                      40 LOAD_CLOSURE             0 (__class__)
-                      42 COPY                     1
-                      44 STORE_NAME               7 (__classcell__)
-                      46 RETURN_VALUE
+          24          32 LOAD_CONST               8 (('return', None))
+                      34 LOAD_CLOSURE             0 (__class__)
+                      36 BUILD_TUPLE              1
+                      38 LOAD_CONST               6 (<code object update, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 24>)
+                      40 MAKE_FUNCTION           12 (annotations, closure)
+                      42 STORE_NAME               6 (update)
+         
+          28          44 LOAD_CONST               9 ((None,))
+                      46 LOAD_CONST               7 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 28>)
+                      48 MAKE_FUNCTION            1 (defaults)
+                      50 STORE_NAME               7 (_draw)
+                      52 LOAD_CLOSURE             0 (__class__)
+                      54 COPY                     1
+                      56 STORE_NAME               8 (__classcell__)
+                      58 RETURN_VALUE
          consts
             'AdwWidget'
             '\n    基础绘制组件类\n\n    特性：自动将背景颜色设为父组件背景颜色\n    '
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
@@ -129,82 +137,156 @@
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\widget.py'
                name       '__init__'
                firstlineno 12
                lnotab 0x040132023a01
             code
                argcount  : 1
-               nlocals   : 1
+               nlocals   : 2
                stacksize : 5
                flags     : 3
                code
-                  0x97007c00a00000000000000000000000000000000000000000007c006a
-                  010000000000000000a00200000000000000000000000000000000000000
-                  006401a6010000ab0100000000000000006402ac03a6020000ab02000000
-                  0000000000010064005300
+                  0x9700640164026c006d017d0101007405000000000000000000007c006a
+                  0300000000000000006403a6020000ab02000000000000000072207c00a0
+                  0400000000000000000000000000000000000000007c006a030000000000
+                  0000006a050000000000000000ac04a6010000ab01000000000000000001
+                  007c00a00400000000000000000000000000000000000000007c006a0300
+                  00000000000000a006000000000000000000000000000000000000000064
+                  05a6010000ab0100000000000000006401ac06a6020000ab020000000000
+                  000000010064005300
                 18           0 RESUME                   0
                
-                19           2 LOAD_FAST                0 (self)
-                             4 LOAD_METHOD              0 (configure)
+                19           2 LOAD_CONST               1 (0)
+                             4 LOAD_CONST               2 (('AdwDrawBasicFrame',))
+                             6 IMPORT_NAME              0 (tkadw.windows.canvas.frame)
+                             8 IMPORT_FROM              1 (AdwDrawBasicFrame)
+                            10 STORE_FAST               1 (AdwDrawBasicFrame)
+                            12 POP_TOP
+               
+                20          14 LOAD_GLOBAL              5 (NULL + hasattr)
                             26 LOAD_FAST                0 (self)
-                            28 LOAD_ATTR                1 (master)
-                            38 LOAD_METHOD              2 (cget)
-                            60 LOAD_CONST               1 ('bg')
-                            62 PRECALL                  1
-                            66 CALL                     1
-                            76 LOAD_CONST               2 (0)
-                            78 KW_NAMES                 3
-                            80 PRECALL                  2
-                            84 CALL                     2
-                            94 POP_TOP
-                            96 LOAD_CONST               0 (None)
-                            98 RETURN_VALUE
+                            28 LOAD_ATTR                3 (master)
+                            38 LOAD_CONST               3 ('frame_back')
+                            40 PRECALL                  2
+                            44 CALL                     2
+                            54 POP_JUMP_FORWARD_IF_FALSE    32 (to 120)
+               
+                21          56 LOAD_FAST                0 (self)
+                            58 LOAD_METHOD              4 (configure)
+                            80 LOAD_FAST                0 (self)
+                            82 LOAD_ATTR                3 (master)
+                            92 LOAD_ATTR                5 (frame_back)
+                           102 KW_NAMES                 4
+                           104 PRECALL                  1
+                           108 CALL                     1
+                           118 POP_TOP
+               
+                22     >>  120 LOAD_FAST                0 (self)
+                           122 LOAD_METHOD              4 (configure)
+                           144 LOAD_FAST                0 (self)
+                           146 LOAD_ATTR                3 (master)
+                           156 LOAD_METHOD              6 (cget)
+                           178 LOAD_CONST               5 ('bg')
+                           180 PRECALL                  1
+                           184 CALL                     1
+                           194 LOAD_CONST               1 (0)
+                           196 KW_NAMES                 6
+                           198 PRECALL                  2
+                           202 CALL                     2
+                           212 POP_TOP
+                           214 LOAD_CONST               0 (None)
+                           216 RETURN_VALUE
                consts
                   None
-                  'bg'
                   0
+                  ('AdwDrawBasicFrame',)
+                  'frame_back'
+                  ('background',)
+                  'bg'
                   ('background', 'borderwidth')
-               names      ('configure', 'master', 'cget')
-               varnames   ('self',)
+               names      ('tkadw.windows.canvas.frame', 'AdwDrawBasicFrame', 'hasattr', 'master', 'configure', 'frame_back', 'cget')
+               varnames   ('self', 'AdwDrawBasicFrame')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\widget.py'
                name       '_other'
                firstlineno 18
-               lnotab 0x0201
+               lnotab 0x02010c012a014001
+            'return'
             None
             code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 3
+               flags     : 3
+               code
+                  0x95019700740100000000000000000000a6000000ab0000000000000000
+                  00a0010000000000000000000000000000000000000000a6000000ab0000
+                  0000000000000001007c00a0020000000000000000000000000000000000
+                  0000006400a6010000ab010000000000000000010064005300
+                             0 COPY_FREE_VARS           1
+               
+                24           2 RESUME                   0
+               
+                25           4 LOAD_GLOBAL              1 (NULL + super)
+                            16 PRECALL                  0
+                            20 CALL                     0
+                            30 LOAD_METHOD              1 (update)
+                            52 PRECALL                  0
+                            56 CALL                     0
+                            66 POP_TOP
+               
+                26          68 LOAD_FAST                0 (self)
+                            70 LOAD_METHOD              2 (_draw)
+                            92 LOAD_CONST               0 (None)
+                            94 PRECALL                  1
+                            98 CALL                     1
+                           108 POP_TOP
+                           110 LOAD_CONST               0 (None)
+                           112 RETURN_VALUE
+               consts
+                  None
+               names      ('super', 'update', '_draw')
+               varnames   ('self',)
+               freevars   ('__class__',)
+               cellvars   ()
+               filename   'D:\\tkadw\\tkadw\\windows\\canvas\\widget.py'
+               name       'update'
+               firstlineno 24
+               lnotab 0x04014001
+            code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x970064005300
-                21           0 RESUME                   0
+                28           0 RESUME                   0
                
-                22           2 LOAD_CONST               0 (None)
+                29           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\widget.py'
                name       '_draw'
-               firstlineno 21
+               firstlineno 28
                lnotab 0x0201
+            ('return', None)
             (None,)
-         names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', '_other', '_draw', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', '_other', 'update', '_draw', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\widget.py'
          name       'AdwWidget'
          firstlineno 4
-         lnotab 0x0c0204060a060603
+         lnotab 0x0c0204060a0606060c04
       'AdwWidget'
       None
    names      ('tkadw.windows.canvas.drawengine', 'AdwDrawEngine', 'AdwWidget')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\windows\\canvas\\widget.py'
```

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/button.py` & `tkadw-0.3.3/tkadw/windows/canvas/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,17 +440,17 @@
 
 class AdwDrawRoundButton3(AdwDrawBasicRoundButton):
     def _draw(self, evt):
         self.delete("all")
 
         # 绘制按钮边框
         self.create_round_rect4(
-            self._button_border_width - 1, self._button_border_width - 1,
-            self.winfo_width() - self._button_border_width * 2 + 1,
-            self.winfo_height() - self._button_border_width * 2 + 1,
+            self._button_border_width, self._button_border_width,
+            self.winfo_width() - self._button_border_width,
+            self.winfo_height() - self._button_border_width,
             self.button_radius,
             width=self._button_border_width,
             outline=self._button_border, fill=self._button_back,
         )
 
         self.button_frame = "button_frame"
```

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/checkbox.py` & `tkadw-0.3.3/tkadw/windows/canvas/checkbox.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/drawengine.py` & `tkadw-0.3.3/tkadw/windows/canvas/drawengine.py`

 * *Files 3% similar despite different names*

```diff
@@ -239,14 +239,17 @@
 
 
 class AdwDrawEngine(Canvas):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def win32_high_dpi(self):
+        """
+        windows平台高DPI启用
+        """
         from ctypes import windll
         windll.shcore.SetProcessDpiAwareness(2)
 
     def rgb_to_num(self, rgb):
         return int(rgb[1:3], 16), int(rgb[3:5], 16), int(rgb[5:], 16)
 
     def num_to_rgb(self, hexs: tuple):
@@ -263,14 +266,17 @@
         for i in range(num):
             t = i / num-1
             rgb = (int(a1 + r * t), int(a2 + g * t), int(a3 + b * t))
             colors.append(self.num_to_rgb(rgb))
         return colors
 
     def gradient_init(self):
+        """
+        初始化渐变引擎
+        """
         self.tk.eval("""
         # Create color gradients of various shapes and sizes on a canvas.
 #   Usage:
 #       gradient draw    <canvas> <tags> <x> <y> <width> <height> <vertical|horizontal|circular|central|arc> <color1> <color2>  ?-animate? ?option? ...
 #       gradient redraw  <canvas> <tags> <x> <y> <width> <height> <vertical|horizontal|circular|central|arc> <color1> <color2>  ?-animate? ?option? ...
 #       gradient resize  <canvas> <tags> <x> <y> <width> <height>
 #       gradient recolor <canvas> <tags> <color1> <color2>
@@ -605,44 +611,95 @@
 
         return
     }
 }
         """)
 
     def gradient_demo(self):
+        """
+        启动渐变引擎示例
+        """
         self.gradient_init()
         self.tk.call("gradient", "demo")
 
     def gradient_resize(self, tags: str, x: int, y: int, width: int, height: int):
+        """
+        修改渐变图形的大小位置
+        """
         self.gradient_init()
         self.tk.call("gradient", "resize", self._w, tags, x, y, width, height)
 
     def gradient_recolor(self, tags: str, x: int, y: int, color1, color2):
+        """
+        修改渐变组件的颜色
+        """
         self.gradient_init()
         self.tk.call("gradient", "color", self._w, tags, color1, color2)
 
     def gradient_draw(self, tags: str, x: int, y: int, width: int, height: int, orient, color1, color2, *args,
                       **kwargs):
+        """
+        绘制渐变图形
+        """
         self.gradient_init()
         id = self.tk.call("gradient", "draw", self._w, tags, x, y, width, height, orient, color1, color2)
         self.itemconfigure(tags, *args, **kwargs)
         return id
 
     def gradient_redraw(self, *args, **kwargs):
+        """
+        同gradient_draw
+        """
         self.gradient_draw(*args, **kwargs)
 
     def create_gradient_v_rectangle(self, x, y, width, height, tags, color1, color2, *args, **kwargs):
+        """
+        创建水平渐变矩形
+
+        :param x: 图形x位置
+        :param y: 图形y位置
+        :param width: 图形宽度
+        :param height: 图形高度
+        :param tags: 标签名
+        :param color1: 渐变颜色1
+        :param color2: 渐变颜色2
+        :return:
+        """
         return self.gradient_draw(tags=tags, x=x, y=y, width=width, height=height, color1=color1, color2=color2,
                                   orient=VERTICAL, *args, **kwargs)
 
     def create_gradient_h_rectangle(self, x, y, width, height, tags, color1, color2, *args, **kwargs):
+        """
+        创建垂直渐变矩形
+
+        :param x: 图形x位置
+        :param y: 图形y位置
+        :param width: 图形宽度
+        :param height: 图形高度
+        :param tags: 标签名
+        :param color1: 渐变颜色1
+        :param color2: 渐变颜色2
+        :return:
+        """
         return self.gradient_draw(tags=tags, x=x, y=y, width=width, height=height, color1=color1, color2=color2,
                                   orient=HORIZONTAL, *args, **kwargs)
 
     def create_gradient_circular(self, x, y, width, height, tags, color1, color2, *args, **kwargs):
+        """
+        创建垂直渐变圆形
+
+        :param x: 图形x位置
+        :param y: 图形y位置
+        :param width: 图形宽度
+        :param height: 图形高度
+        :param tags: 标签名
+        :param color1: 渐变颜色1
+        :param color2: 渐变颜色2
+        :return:
+        """
         return self.gradient_draw(tags=tags, x=x, y=y, width=width, height=height, color1=color1, color2=color2,
                                   orient=CIRCULAR, *args, **kwargs)
 
     def draw_gradient(self, color1, color2, type="x"):
         self.tk.eval("""
   proc + {n1 n2} {
     expr {$n1 + $n2}
@@ -706,14 +763,17 @@
     return $win
   }
         """)
 
         self.tk.call("drawGradient", self._w, type, color1, color2)
 
     def create_round_rectangle(self, x1, y1, x2, y2, radius: float = 5, width=2, fill="white", outline="black"):
+        """
+        创建圆角矩形 ： 自绘版
+        """
         # 自研
         _radius = radius * 2
         nw = self.create_arc(x1, y1, x1 + _radius, y1 + _radius, start=90, extent=90, width=width, fill=fill,
                              outline=outline)  # ⌜ north | west
         sw = self.create_arc(x1, y2, x1 + _radius, y2 - _radius, start=180, extent=90, width=width, fill=fill,
                              outline=outline)  # ⌞ south | wast
         ne = self.create_arc(x2 - _radius, y1, x2, y1 + _radius, start=0, extent=90, width=width, fill=fill,
@@ -742,14 +802,17 @@
             "nw": nw, "sw": sw, "ne": ne, "se": se, "w": w, "n": n, "e": e, "s": s,
             "top": top, "center": center, "bottom": bottom
         }
 
     create_round_rect = create_round_rectangle
 
     def create_round_rectangle2(self, x0, y0, x3, y3, radius, *args, **kwargs):
+        """
+        创建圆角矩形 ： 其他开发者制作 ： 边框有问题（不推荐）
+        """
         # wiki上
         self.tk.eval("""
 #----------------------------------------------------------------------
 #
 # roundRect --
 #
 #       Draw a rounded rectangle in the canvas.
@@ -813,14 +876,17 @@
         self.itemconfig(rect, *args, **kwargs)
         return rect
 
     create_round_rect2 = create_round_rectangle2
 
     def create_round_rectangle3(self, tag, x, y, width, height, radius, fill: str = "black", outline: str = "black",
                                 *args, **kwargs):
+        """
+        创建圆角矩形 ： 其他开发者制作 ： 圆角看起来更舒服
+        """
         # wiki上 圆角看起来更舒服
         self.tk.eval("""
 proc roundRect2 {w L T Rad width height fill outline tag} {
 
   $w create oval $L $T [expr $L + $Rad] [expr $T + $Rad] -fill $fill -outline $outline -tag $tag
   $w create oval [expr $width-$Rad] $T $width [expr $T + $Rad] -fill $fill -outline $outline -tag $tag
   $w create oval $L [expr $height-$Rad] [expr $L+$Rad] $height -fill $fill -outline $outline -tag $tag
@@ -832,14 +898,17 @@
         _rect = self.tk.call("roundRect2", self._w, x, y, radius, width, height, fill, outline, tag)
         self.itemconfig(_rect, *args, **kwargs)
         return _rect
 
     create_round_rect3 = create_round_rectangle3
 
     def create_round_rectangle4(self, x1, y1, x2, y2, radius, **kwargs):
+        """
+        创建圆角矩形 ： 其他开发者制作
+        """
         points = [x1 + radius, y1,
                   x1 + radius, y1,
                   x2 - radius, y1,
                   x2 - radius, y1,
                   x2, y1,
                   x2, y1 + radius,
                   x2, y1 + radius,
```

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/entry.py` & `tkadw-0.3.3/tkadw/windows/canvas/entry.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/frame.py` & `tkadw-0.3.3/tkadw/windows/canvas/frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,49 +25,52 @@
 
         self.frame.configure(background=self.frame_back, bd=0, )
 
         # 绘制框架区域
         self.frame_f = self.create_window(
             self.winfo_width() / 2, self.winfo_height() / 2,
             window=self.frame,
-            width=self.winfo_width() - 6 - self.frame_border_width,
-            height=self.winfo_height() - 6 - self.frame_border_width,
+            width=self.winfo_width() - 6 - self.frame_border_width - self.frame_padding,
+            height=self.winfo_height() - 6 - self.frame_border_width - self.frame_padding,
         )
 
     def default_palette(self):
         self.palette_light()
 
     def palette_light(self):
         self.palette(
             {
                 "frame": {
                     "back": "#ffffff",
                     "border": "#eaeaea",
                     "border_width": 2,
+                    "padding": 0
                 }
             }
         )
 
     def palette_dark(self):
         self.palette(
             {
                 "frame": {
                     "back": "#0f0f0f",
                     "border": "#333333",
                     "border_width": 2,
+                    "padding": 0
                 }
             }
         )
 
     def palette(self, dict=None):
         if dict is not None:
             if "frame" in dict:
                 self.frame_back = dict["frame"]["back"]
                 self.frame_border = dict["frame"]["border"]
                 self.frame_border_width = dict["frame"]["border_width"]
+                self.frame_padding = dict["frame"]["padding"]
 
             self._palette = dict
 
             try:
                 self._draw(None)
             except AttributeError:
                 pass
@@ -94,52 +97,56 @@
             pass
 
     def _draw(self, evt):
         self.delete("all")
 
         # 绘制框架边框
         self.frame_frame = self.create_round_rect2(
-            0, 0, self.winfo_width(), self.winfo_height(), self.frame_radius,
+            self.frame_border_width, self.frame_border_width,
+            self.winfo_width() - self.frame_border_width, self.winfo_height() - self.frame_border_width,
+            self.frame_radius,
             width=self.frame_border_width,
             outline=self.frame_border, fill=self.frame_back,
         )
 
         self.frame.configure(background=self.frame_back, bd=0, )
 
         # 绘制框架区域
         self.frame_f = self.create_window(
             self.winfo_width() / 2, self.winfo_height() / 2,
             window=self.frame,
-            width=self.winfo_width() - 6 - self.frame_border_width,
-            height=self.winfo_height() - 6 - self.frame_border_width,
+            width=self.winfo_width() - 6 - self.frame_border_width - self.frame_padding,
+            height=self.winfo_height() - 6 - self.frame_border_width - self.frame_padding,
         )
 
     def default_palette(self):
         self.palette_light()
 
     def palette_light(self):
         self.palette(
             {
                 "frame": {
                     "radius": 6,
                     "back": "#0f0f0f",
                     "border": "#333333",
                     "border_width": 2,
+                    "padding": 0
                 }
             }
         )
 
     def palette_dark(self):
         self.palette(
             {
                 "frame": {
                     "radius": 6,
                     "back": "#0f0f0f",
                     "border": "#333333",
                     "border_width": 2,
+                    "padding": 0
                 }
             }
         )
 
     def palette(self, dict=None):
         super().palette(dict)
         if "frame" in dict:
@@ -165,31 +172,33 @@
             pass
 
     def _draw(self, evt):
         self.delete("all")
 
         # 绘制框架边框
         self.create_round_rect4(
-            0, 0,
-            self.winfo_width(),
-            self.winfo_height(), self.frame_radius,
+            self.frame_border_width, self.frame_border_width,
+            self.winfo_width() - self.frame_border_width,
+            self.winfo_height() - self.frame_border_width,
+            self.frame_radius,
             width=self.frame_border_width,
             outline=self.frame_border, fill=self.frame_back,
         )
 
+
         self.entry_frame = "button_frame"
 
         self.frame.configure(background=self.frame_back, bd=0, )
 
         # 绘制框架区域
         self.frame_f = self.create_window(
             self.winfo_width() / 2, self.winfo_height() / 2,
             window=self.frame,
-            width=self.winfo_width() - 6 - self.frame_border_width,
-            height=self.winfo_height() - 6 - self.frame_border_width,
+            width=self.winfo_width() - 6 - self.frame_border_width - self.frame_padding,
+            height=self.winfo_height() - 6 - self.frame_border_width - self.frame_padding,
         )
 
     def default_palette(self):
         self.palette_light()
 
 
 class AdwDrawRoundFrame3(AdwDrawBasicRoundFrame3):
```

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/separator.py` & `tkadw-0.3.3/tkadw/windows/canvas/separator.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/textbox.py` & `tkadw-0.3.3/tkadw/windows/canvas/textbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from tkinter.font import Font, nametofont
-from tkadw.windows.canvas.drawengine import AdwDrawEngine
+from tkadw.windows.canvas.widget import AdwWidget
 
 
 # Text
-class AdwDrawBasicText(AdwDrawEngine):
+class AdwDrawBasicText(AdwWidget):
     def __init__(self, *args, text: str = "", width=120, height=80, **kwargs):
 
         super().__init__(*args, width=width, height=height, highlightthickness=0, **kwargs)
 
         from tkinter import Text
 
         self.text_text_font = nametofont("TkDefaultFont")
@@ -160,14 +160,15 @@
             self._draw(None)
 
     def font(self, font: Font = None):
         if font is None:
             return self.text_text_font
         else:
             self.text_text_font = font
+        self.update()
 
     def default_palette(self):
         self.palette_light()
 
     def palette_light(self):
         self.palette(
             {
```

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/titlebar.py` & `tkadw-0.3.3/tkadw/windows/canvas/titlebar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from tkinter import Tk, Frame, Label, ttk
-from tkadw.canvas.button import AdwDrawButton
+from tkadw.windows.theme import AdwTButton, AdwTFrame, AdwTLabel, Adwite
 from sys import platform
 
 
-class AdwCustomTk(Tk):
+class AdwCustomTk(Adwite):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.frameless()
         self.build()
         
         self.x, self.y = 0, 0
 
@@ -26,31 +25,32 @@
             res = windll.user32.SetWindowLongW(hwnd, GWL_EXSTYLE, style)
         except:
             self.wm_attributes("-topmost", True)
 
         self.minsize(150, 180)
 
     def build(self):
-        self.frame_border = Frame(self, borderwidth=1, relief="ridge")
+        self.frame_border = AdwTFrame(self)
         self.frame_border.pack(fill="both", expand=True, padx=3, pady=3)
 
-        self.frame_title = Frame(self.frame_border, borderwidth=0)
+        self.frame_title = AdwTFrame(self.frame_border.frame, borderwidth=0)
+
         self.frame_title.pack(fill="x", side="top", padx=2, pady=2)
-        self.bind_move(self.frame_title)
+        self.bind_move(self.frame_title.frame)
 
-        self.label_title = Label(self.frame_title, text=self.wm_title())
+        self.label_title = AdwTLabel(self.frame_title.frame, text=self.wm_title())
         self.label_title.pack(side="left", anchor="w", padx=10, pady=5)
         self.bind_move(self.label_title)
 
         self.maximized = False
 
-        self.button_close = AdwDrawButton(self.frame_title, text="✕", width=30, height=30, command=lambda: self.destroy())
+        self.button_close = AdwTButton(self.frame_title.frame, text="✕", width=30, height=30, command=lambda: self.destroy())
         self.button_close.pack(side="right", anchor="e", padx=5, pady=5)
 
-        self.button_minimize = AdwDrawButton(self.frame_title, text="–", width=30, height=30, command=lambda: self.minimize())
+        self.button_minimize = AdwTButton(self.frame_title.frame, text="–", width=30, height=30, command=lambda: self.minimize())
         self.button_minimize.pack(side="right", anchor="e", padx=5, pady=5)
 
     def minimize(self):
         try:
             from ctypes import windll
             hwnd = windll.user32.GetParent(self.winfo_id())
             windll.user32.ShowWindow(hwnd, 2)
@@ -58,14 +58,15 @@
             pass
 
     def bind_move(self, widget):
         widget.bind("<Button-1>", self._click)
         widget.bind("<B1-Motion>", self._move)
 
     def create_sizegrip(self):
+        from tkinter import ttk
         ttk.Style().configure("CTkCustom.TSizegrip", background="#ffffff")
         self.sizegrip = ttk.Sizegrip(self.frame_border, style="CTkCustom.TSizegrip")
         self.sizegrip.pack(side="bottom", anchor="se", padx=5, pady=5, ipady=2)
         return self.sizegrip
 
     @property
     def titlebar(self):
```

### Comparing `tkadw-0.3.2/tkadw/windows/canvas/widget.py` & `tkadw-0.3.3/tkadw/windows/canvas/widget.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,11 +12,18 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.bind("<Configure>", self._draw, add="+")
         self._other()
 
     def _other(self):
+        from tkadw.windows.canvas.frame import AdwDrawBasicFrame
+        if hasattr(self.master, "frame_back"):
+            self.configure(background=self.master.frame_back)
         self.configure(background=self.master.cget("bg"), borderwidth=0)
 
+    def update(self) -> None:
+        super().update()
+        self._draw(None)
+
     def _draw(self, evt=None):
         pass
```

### Comparing `tkadw-0.3.2/tkadw/windows/fluent/__pycache__/button.cpython-310.pyc` & `tkadw-0.3.3/tkadw/windows/fluent/__pycache__/button.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/fluent/__pycache__/button.cpython-311.pyc` & `tkadw-0.3.3/tkadw/windows/fluent/__pycache__/button.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/fluent/__pycache__/entry.cpython-310.pyc` & `tkadw-0.3.3/tkadw/windows/fluent/__pycache__/entry.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/fluent/__pycache__/entry.cpython-311.pyc` & `tkadw-0.3.3/tkadw/windows/fluent/__pycache__/entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/fluent/__pycache__/frame.cpython-310.pyc` & `tkadw-0.3.3/tkadw/windows/fluent/__pycache__/frame.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/fluent/__pycache__/frame.cpython-311.pyc` & `tkadw-0.3.3/tkadw/windows/fluent/__pycache__/frame.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/fluent/button.py` & `tkadw-0.3.3/tkadw/windows/fluent/button.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/fluent/entry.py` & `tkadw-0.3.3/tkadw/windows/fluent/entry.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/fluent/frame.py` & `tkadw-0.3.3/tkadw/windows/fluent/frame.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/fluent/GeneralSans-Regular.ttf` & `tkadw-0.3.3/tkadw/windows/fluent/GeneralSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/fluent/test.py` & `tkadw-0.3.3/tkadw/windows/fluent/test.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/theme.py` & `tkadw-0.3.3/tkadw/windows/theme.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,27 +30,28 @@
         },
     },
 
     "frame": {
         "radius": 15,
         "back": "#fafafa",
         "border": "#e7e7e7",
-        "border_width": 2,
+        "border_width": 1,
+        "padding": 0
     },
 
     "entry": {
         "radius": 13,
         "padding": (8, 8),
 
-        "back": "#fdfdfd",
-        "border": "#ebebeb",
+        "back": "#ffffff",
+        "border": "#e6e6e6",
         "text_back": "#18191c",
         "border_width": 1,
 
-        "bottom_line": "#8a8a8a",
+        "bottom_line": "#9c9c9c",
         "bottom_width": 1,
 
         "focusin": {
             "back": "#ffffff",
             "border": "#ebebeb",
             "text_back": "#18191c",
             "border_width": 1,
@@ -60,20 +61,20 @@
         }
     },
 
     "text": {
         "radius": 13,
         "padding": (8, 8),
 
-        "back": "#fdfdfd",
-        "border": "#ebebeb",
+        "back": "#ffffff",
+        "border": "#e6e6e6",
         "text_back": "#18191c",
         "border_width": 1,
 
-        "bottom_line": "#8a8a8a",
+        "bottom_line": "#9c9c9c",
         "bottom_width": 1,
 
         "focusin": {
             "back": "#ffffff",
             "border": "#ebebeb",
             "text_back": "#18191c",
             "border_width": 1,
@@ -123,27 +124,28 @@
         },
     },
 
     "frame": {
         "radius": 15,
         "back": "#1c1c1c",
         "border": "#2f2f2f",
-        "border_width": 2,
+        "border_width": 1,
+        "padding": 0
     },
 
     "entry": {
         "radius": 13,
         "padding": (8, 8),
 
-        "back": "#292929",
-        "border": "#292929",
+        "back": "#2c2c2c",
+        "border": "#383838",
         "text_back": "#e7e9eb",
         "border_width": 1,
 
-        "bottom_line": "#989898",
+        "bottom_line": "#686868",
         "bottom_width": 1,
 
         "focusin": {
             "back": "#1c1c1c",
             "border": "#2c2c2c",
             "text_back": "#e7e9eb",
             "border_width": 1,
@@ -153,20 +155,20 @@
         }
     },
 
     "text": {
         "radius": 13,
         "padding": (8, 8),
 
-        "back": "#292929",
-        "border": "#292929",
+        "back": "#2c2c2c",
+        "border": "#383838",
         "text_back": "#e7e9eb",
         "border_width": 1,
 
-        "bottom_line": "#989898",
+        "bottom_line": "#686868",
         "bottom_width": 1,
 
         "focusin": {
             "back": "#1c1c1c",
             "border": "#2c2c2c",
             "text_back": "#e7e9eb",
             "border_width": 1,
@@ -216,15 +218,16 @@
         },
     },
 
     "frame": {
         "radius": 0,
         "back": "#f6f5f4",
         "border": "#d5d0cc",
-        "border_width": 2,
+        "border_width": 1,
+        "padding": 0
     },
 
     "entry": {
         "radius": 11,
         "padding": (5, 5),
 
         "back": "#ffffff",
@@ -309,15 +312,16 @@
         },
     },
 
     "frame": {
         "radius": 0,
         "back": "#313131",
         "border": "#1b1b1b",
-        "border_width": 2,
+        "border_width": 1,
+        "padding": 0
     },
 
     "entry": {
         "radius": 11,
         "padding": (5, 5),
 
         "back": "#2d2d2d",
@@ -402,15 +406,16 @@
         },
     },
 
     "frame": {
         "radius": 18,
         "back": "#f6f7f8",
         "border": "#f1f2f3",
-        "border_width": 2,
+        "border_width": 1,
+        "padding": 0
     },
 
     "entry": {
         "radius": 16,
         "padding": (8, 8),
 
         "back": "#ffffff",
@@ -495,15 +500,16 @@
         },
     },
 
     "frame": {
         "radius": 18,
         "back": "#1e2022",
         "border": "#232527",
-        "border_width": 2,
+        "border_width": 1,
+        "padding": 0
     },
 
     "entry": {
         "radius": 16,
         "padding": (8, 8),
 
         "back": "#17181a",
@@ -588,15 +594,16 @@
         },
     },
 
     "frame": {
         "radius": 0,
         "back": "#ffffff",
         "border": "#bfbfbf",
-        "border_width": 2,
+        "border_width": 1,
+        "padding": 0
     },
 
     "entry": {
         "radius": 0,
         "padding": (3, 3),
 
         "back": "#ffffff",
@@ -681,15 +688,16 @@
         },
     },
 
     "frame": {
         "radius": 0,
         "back": "#111111",
         "border": "#373737",
-        "border_width": 2,
+        "border_width": 1,
+        "padding": 0
     },
 
     "entry": {
         "radius": 0,
         "padding": (3, 3),
 
         "back": "#111111",
@@ -738,14 +746,202 @@
         "back": "#999999",
         "border_width": 1,
 
         "rounded": False
     }
 }
 
+basic_theme = {
+    "window": {
+        "back": "#f0f0f0"
+    },
+
+    "label": {
+        "back": "transparent",
+        "text_back": "#000000",
+    },
+
+    "button": {
+        "radius": 0,
+        "back": "#ffffff",
+        "border": "#a0a0a0",
+        "text_back": "#000000",
+        "border_width": 1,
+
+        "active": {
+            "back": "#dce9fc",
+            "border": "#a0a0a0",
+            "text_back": "#000000",
+            "border_width": 1,
+        },
+
+        "pressed": {
+            "back": "#dce9fc",
+            "border": "#4e6d9c",
+            "text_back": "#000000",
+            "border_width": 2,
+        },
+    },
+
+    "frame": {
+        "radius": 0,
+        "back": "#f0f0f0",
+        "border": "#c8c8c8",
+        "border_width": 1,
+        "padding": 0
+    },
+
+    "entry": {
+        "radius": 0,
+        "padding": (3, 3),
+
+        "back": "#ffffff",
+        "border": "#a0a0a0",
+        "text_back": "#000000",
+        "border_width": 1,
+
+        "bottom_line": "#ffffff",
+        "bottom_width": 0,
+
+        "focusin": {
+            "back": "#ffffff",
+            "border": "#a0a0a0",
+            "text_back": "#000000",
+            "border_width": 1,
+
+            "bottom_line": "#ffffff",
+            "bottom_width": 0,
+        }
+    },
+
+    "text": {
+        "radius": 0,
+        "padding": (3, 3),
+
+        "back": "#ffffff",
+        "border": "#a0a0a0",
+        "text_back": "#000000",
+        "border_width": 1,
+
+        "bottom_line": "#ffffff",
+        "bottom_width": 0,
+
+        "focusin": {
+            "back": "#ffffff",
+            "border": "#a0a0a0",
+            "text_back": "#000000",
+            "border_width": 1,
+
+            "bottom_line": "#ffffff",
+            "bottom_width": 0,
+        }
+    },
+
+    "separator": {
+        "back": "#999999",
+        "border_width": 1,
+
+        "rounded": True
+    }
+}
+
+basic_dark_theme = {
+    "window": {
+        "back": "#323232"
+    },
+
+    "label": {
+        "back": "transparent",
+        "text_back": "#ffffff",
+    },
+
+    "button": {
+        "radius": 0,
+        "back": "#232323",
+        "border": "#4b4b4b",
+        "text_back": "#ffffff",
+        "border_width": 1,
+
+        "active": {
+            "back": "#373737",
+            "border": "#4b4b4b",
+            "text_back": "#ffffff",
+            "border_width": 1,
+        },
+
+        "pressed": {
+            "back": "#373737",
+            "border": "#4e6d9c",
+            "text_back": "#ffffff",
+            "border_width": 2,
+        },
+    },
+
+    "frame": {
+        "radius": 0,
+        "back": "#323232",
+        "border": "#464646",
+        "border_width": 1,
+        "padding": 0
+    },
+
+    "entry": {
+        "radius": 0,
+        "padding": (3, 3),
+
+        "back": "#232323",
+        "border": "#4b4b4b",
+        "text_back": "#ffffff",
+        "border_width": 1,
+
+        "bottom_line": "#ffffff",
+        "bottom_width": 0,
+
+        "focusin": {
+            "back": "#232323",
+            "border": "#4b4b4b",
+            "text_back": "#ffffff",
+            "border_width": 1,
+
+            "bottom_line": "#ffffff",
+            "bottom_width": 0,
+        }
+    },
+
+    "text": {
+        "radius": 0,
+        "padding": (3, 3),
+
+        "back": "#232323",
+        "border": "#4b4b4b",
+        "text_back": "#ffffff",
+        "border_width": 1,
+
+        "bottom_line": "#ffffff",
+        "bottom_width": 0,
+
+        "focusin": {
+            "back": "#232323",
+            "border": "#4b4b4b",
+            "text_back": "#ffffff",
+            "border_width": 1,
+
+            "bottom_line": "#ffffff",
+            "bottom_width": 0,
+        }
+    },
+
+    "separator": {
+        "back": "#464646",
+        "border_width": 1,
+
+        "rounded": False
+    }
+}
+
 
 def get_default_theme():
     from os import environ
     from json import loads
     try:
         return loads(environ["tkAdwite.DefaultTheme"])
     except KeyError:
@@ -816,14 +1012,29 @@
                     _set_default_theme(metro_dark_theme)
                 else:
                     _set_default_theme(metro_theme)
         elif mode.lower() == "dark":
             _set_default_theme(metro_dark_theme)
         else:
             _set_default_theme(metro_theme)
+    elif theme == "basic" or theme == "Basic":
+        if mode.lower() == "system" or mode.lower() == "auto":
+            try:
+                from darkdetect import isDark
+            except ModuleNotFoundError:
+                _set_default_theme(basic_theme)
+            else:
+                if isDark():
+                    _set_default_theme(basic_dark_theme)
+                else:
+                    _set_default_theme(basic_theme)
+        elif mode.lower() == "dark":
+            _set_default_theme(basic_dark_theme)
+        else:
+            _set_default_theme(basic_theme)
     else:
         _set_default_theme(theme)
 
 
 set_default_theme("win11")
 
 
@@ -833,15 +1044,15 @@
 class Adwite(Adw):
     def set_default_theme(self, theme, _mode="auto"):
         set_default_theme(theme, _mode)
         for widget in self.winfo_children():
             if hasattr(widget, "palette"):
                 widget.palette(get_default_theme())
                 widget.configure(background=widget.master.cget("bg"))
-                widget._draw(None)
+                widget.update()
         self.palette(get_default_theme())
 
     def default_palette(self):
         self.palette(get_default_theme())
 
 
 from tkadw.windows.widgets import AdwLabel
@@ -892,20 +1103,17 @@
         self.palette(get_default_theme())
 
 
 if __name__ == '__main__':
     from darkdetect import isDark
 
     root = Adwite()
-    root.set_default_theme("metro")
-
-    def toggle():
-        root.set_default_theme("win11")
+    root.set_default_theme("win11", "dark")
 
-    button = AdwTButton(text="AdwTButton", command=toggle)
+    button = AdwTButton(text="AdwTButton")
     button.pack(fill="x", padx=5, pady=5)
     separator = AdwTSeparator()
     separator.pack(fill="x", padx=5, pady=5)
     entry = AdwTEntry(text="AdwTEntry")
     entry.pack(fill="x", padx=5, pady=5)
     text = AdwTText(text="AdwTText")
     text.pack(fill="x", padx=5, pady=5)
```

### Comparing `tkadw-0.3.2/tkadw/windows/widgets/__pycache__/adw.cpython-310.pyc` & `tkadw-0.3.3/tkadw/windows/widgets/__pycache__/adw.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/widgets/__pycache__/adw.cpython-311.pyc` & `tkadw-0.3.3/tkadw/windows/widgets/__pycache__/adw.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,21 +1,18 @@
 magic:    0xa70d0d0a
-moddate:  0x212ba464 (Tue Jul  4 14:22:25 2023 UTC)
-files sz: 19150
+moddate:  0x8f6bb264 (Sat Jul 15 09:49:03 2023 UTC)
+files sz: 20035
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100020047006402840064036501a60300
-      00ab0300000000000000005a02650364046b020000000072220200650264
-      05ac06a6010000ab0100000000000000005a046504a00500000000000000
-      00000000000000000000000000a6000000ab000000000000000000010064
-      07530064075300
+      00ab0300000000000000005a0264045300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Tk',))
                  6 IMPORT_NAME              0 (tkinter)
                  8 IMPORT_FROM              1 (Tk)
                 10 STORE_NAME               1 (Tk)
@@ -26,50 +23,28 @@
                 18 LOAD_CONST               2 (<code object Adw, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 4>)
                 20 MAKE_FUNCTION            0
                 22 LOAD_CONST               3 ('Adw')
                 24 LOAD_NAME                1 (Tk)
                 26 PRECALL                  3
                 30 CALL                     3
                 40 STORE_NAME               2 (Adw)
-   
-    73          42 LOAD_NAME                3 (__name__)
-                44 LOAD_CONST               4 ('__main__')
-                46 COMPARE_OP               2 (==)
-                52 POP_JUMP_FORWARD_IF_FALSE    34 (to 122)
-   
-    74          54 PUSH_NULL
-                56 LOAD_NAME                2 (Adw)
-                58 LOAD_CONST               5 ('light')
-                60 KW_NAMES                 6
-                62 PRECALL                  1
-                66 CALL                     1
-                76 STORE_NAME               4 (root)
-   
-    75          78 LOAD_NAME                4 (root)
-                80 LOAD_METHOD              5 (mainloop)
-               102 PRECALL                  0
-               106 CALL                     0
-               116 POP_TOP
-               118 LOAD_CONST               7 (None)
-               120 RETURN_VALUE
-   
-    73     >>  122 LOAD_CONST               7 (None)
-               124 RETURN_VALUE
+                42 LOAD_CONST               4 (None)
+                44 RETURN_VALUE
    consts
       0
       ('Tk',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x8700970065005a0164005a02640164026403640464059c046406650364
-            0765046604880066016408840e5a05640984005a06640a84005a07880078
-            015a085300
+            0765046604880066016408840e5a05640e640a84015a06640b84005a0764
+            0c84005a08640d84005a09880078015a0a5300
                        0 MAKE_CELL                0 (__class__)
          
            4           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Adw')
                       10 STORE_NAME               2 (__qualname__)
@@ -87,25 +62,34 @@
                       32 BUILD_TUPLE              4
                       34 LOAD_CLOSURE             0 (__class__)
                       36 BUILD_TUPLE              1
                       38 LOAD_CONST               8 (<code object __init__, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 5>)
                       40 MAKE_FUNCTION           14 (kwdefaults, annotations, closure)
                       42 STORE_NAME               5 (__init__)
          
-          64          44 LOAD_CONST               9 (<code object default_palette, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 64>)
-                      46 MAKE_FUNCTION            0
-                      48 STORE_NAME               6 (default_palette)
+          64          44 LOAD_CONST              14 (('#0a080a',))
+                      46 LOAD_CONST              10 (<code object custom, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 64>)
+                      48 MAKE_FUNCTION            1 (defaults)
+                      50 STORE_NAME               6 (custom)
          
-          67          50 LOAD_CONST              10 (<code object palette, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 67>)
-                      52 MAKE_FUNCTION            0
-                      54 STORE_NAME               7 (palette)
-                      56 LOAD_CLOSURE             0 (__class__)
-                      58 COPY                     1
-                      60 STORE_NAME               8 (__classcell__)
-                      62 RETURN_VALUE
+          82          52 LOAD_CONST              11 (<code object bind_move, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 82>)
+                      54 MAKE_FUNCTION            0
+                      56 STORE_NAME               7 (bind_move)
+         
+          96          58 LOAD_CONST              12 (<code object default_palette, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 96>)
+                      60 MAKE_FUNCTION            0
+                      62 STORE_NAME               8 (default_palette)
+         
+          99          64 LOAD_CONST              13 (<code object palette, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 99>)
+                      66 MAKE_FUNCTION            0
+                      68 STORE_NAME               9 (palette)
+                      70 LOAD_CLOSURE             0 (__class__)
+                      72 COPY                     1
+                      74 STORE_NAME              10 (__classcell__)
+                      76 RETURN_VALUE
          consts
             'Adw'
             'adw'
             'light'
             True
             None
             ('title', 'icon', 'windark', 'wincaption')
@@ -662,100 +646,380 @@
                name       '__init__'
                firstlineno 5
                lnotab
                   0x080132012a020c02040104021a011a0222010c013cfe2e0422010c013c
                   fe2e042c012c020a040a0430011601300114012c0228020c01100102011c
                   011601220156010201140114fc140602010a0110010c0118010c01da0114
                   ff14fc
+            '#0a080a'
+            code
+               argcount  : 2
+               nlocals   : 4
+               stacksize : 4
+               flags     : 3
+               code
+                  0x9700640164026c006d017d0201007c00a0020000000000000000000000
+                  0000000000000000006403a6010000ab0100000000000000000100640164
+                  046c036d047d03010002007c02a6000000ab0000000000000000007c005f
+                  0500000000000000007c006a050000000000000000a00600000000000000
+                  0000000000000000000000000064056406ac07a6020000ab020000000000
+                  00000001007c006a050000000000000000a0070000000000000000000000
+                  0000000000000000007c01ac08a6010000ab01000000000000000001007c
+                  0364096b020000000072177c00a008000000000000000000000000000000
+                  0000000000640a7c01a6020000ab02000000000000000001006e2564017c
+                  006a0500000000000000005f0900000000000000007c006a050000000000
+                  000000a00a0000000000000000000000000000000000000000a6000000ab
+                  00000000000000000001007c00a00b000000000000000000000000000000
+                  0000000000640b6403a6020000ab020000000000000000010064005300
+                64           0 RESUME                   0
+               
+                65           2 LOAD_CONST               1 (0)
+                             4 LOAD_CONST               2 (('AdwTFrame',))
+                             6 IMPORT_NAME              0 (tkadw.windows.theme)
+                             8 IMPORT_FROM              1 (AdwTFrame)
+                            10 STORE_FAST               2 (AdwTFrame)
+                            12 POP_TOP
+               
+                66          14 LOAD_FAST                0 (self)
+                            16 LOAD_METHOD              2 (overrideredirect)
+                            38 LOAD_CONST               3 (True)
+                            40 PRECALL                  1
+                            44 CALL                     1
+                            54 POP_TOP
+               
+                68          56 LOAD_CONST               1 (0)
+                            58 LOAD_CONST               4 (('platform',))
+                            60 IMPORT_NAME              3 (sys)
+                            62 IMPORT_FROM              4 (platform)
+                            64 STORE_FAST               3 (platform)
+                            66 POP_TOP
+               
+                70          68 PUSH_NULL
+                            70 LOAD_FAST                2 (AdwTFrame)
+                            72 PRECALL                  0
+                            76 CALL                     0
+                            86 LOAD_FAST                0 (self)
+                            88 STORE_ATTR               5 (frame)
+               
+                71          98 LOAD_FAST                0 (self)
+                           100 LOAD_ATTR                5 (frame)
+                           110 LOAD_METHOD              6 (pack)
+                           132 LOAD_CONST               5 ('both')
+                           134 LOAD_CONST               6 ('yes')
+                           136 KW_NAMES                 7
+                           138 PRECALL                  2
+                           142 CALL                     2
+                           152 POP_TOP
+               
+                72         154 LOAD_FAST                0 (self)
+                           156 LOAD_ATTR                5 (frame)
+                           166 LOAD_METHOD              7 (configure)
+                           188 LOAD_FAST                1 (tcolor)
+                           190 KW_NAMES                 8
+                           192 PRECALL                  1
+                           196 CALL                     1
+                           206 POP_TOP
+               
+                74         208 LOAD_FAST                3 (platform)
+                           210 LOAD_CONST               9 ('win32')
+                           212 COMPARE_OP               2 (==)
+                           218 POP_JUMP_FORWARD_IF_FALSE    23 (to 266)
+               
+                75         220 LOAD_FAST                0 (self)
+                           222 LOAD_METHOD              8 (attributes)
+                           244 LOAD_CONST              10 ('-transparentcolor')
+                           246 LOAD_FAST                1 (tcolor)
+                           248 PRECALL                  2
+                           252 CALL                     2
+                           262 POP_TOP
+                           264 JUMP_FORWARD            37 (to 340)
+               
+                77     >>  266 LOAD_CONST               1 (0)
+                           268 LOAD_FAST                0 (self)
+                           270 LOAD_ATTR                5 (frame)
+                           280 STORE_ATTR               9 (frame_radius)
+               
+                78         290 LOAD_FAST                0 (self)
+                           292 LOAD_ATTR                5 (frame)
+                           302 LOAD_METHOD             10 (update)
+                           324 PRECALL                  0
+                           328 CALL                     0
+                           338 POP_TOP
+               
+                80     >>  340 LOAD_FAST                0 (self)
+                           342 LOAD_METHOD             11 (wm_attributes)
+                           364 LOAD_CONST              11 ('-topmost')
+                           366 LOAD_CONST               3 (True)
+                           368 PRECALL                  2
+                           372 CALL                     2
+                           382 POP_TOP
+                           384 LOAD_CONST               0 (None)
+                           386 RETURN_VALUE
+               consts
+                  None
+                  0
+                  ('AdwTFrame',)
+                  True
+                  ('platform',)
+                  'both'
+                  'yes'
+                  ('fill', 'expand')
+                  ('background',)
+                  'win32'
+                  '-transparentcolor'
+                  '-topmost'
+               names      ('tkadw.windows.theme', 'AdwTFrame', 'overrideredirect', 'sys', 'platform', 'frame', 'pack', 'configure', 'attributes', 'frame_radius', 'update', 'wm_attributes')
+               varnames   ('self', 'tcolor', 'AdwTFrame', 'platform')
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\tkadw\\tkadw\\windows\\widgets\\adw.py'
+               name       'custom'
+               firstlineno 64
+               lnotab 0x02010c012a020c021e01380136020c012e0218013202
+            code
+               argcount  : 2
+               nlocals   : 4
+               stacksize : 5
+               flags     : 3
+               code
+                  0x87009700640184007d0288006601640284087d037c01a0000000000000
+                  00000000000000000000000000000064037c026404ac05a6030000ab0300
+                  0000000000000001007c01a0000000000000000000000000000000000000
+                  00000064067c036404ac05a6030000ab0300000000000000000100640053
+                  00
+                             0 MAKE_CELL                0 (self)
+               
+                82           2 RESUME                   0
+               
+                83           4 LOAD_CONST               1 (<code object _click, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 83>)
+                             6 MAKE_FUNCTION            0
+                             8 STORE_FAST               2 (_click)
+               
+                87          10 LOAD_CLOSURE             0 (self)
+                            12 BUILD_TUPLE              1
+                            14 LOAD_CONST               2 (<code object _move, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 87>)
+                            16 MAKE_FUNCTION            8 (closure)
+                            18 STORE_FAST               3 (_move)
+               
+                93          20 LOAD_FAST                1 (widget)
+                            22 LOAD_METHOD              0 (bind)
+                            44 LOAD_CONST               3 ('<Button-1>')
+                            46 LOAD_FAST                2 (_click)
+                            48 LOAD_CONST               4 ('+')
+                            50 KW_NAMES                 5
+                            52 PRECALL                  3
+                            56 CALL                     3
+                            66 POP_TOP
+               
+                94          68 LOAD_FAST                1 (widget)
+                            70 LOAD_METHOD              0 (bind)
+                            92 LOAD_CONST               6 ('<B1-Motion>')
+                            94 LOAD_FAST                3 (_move)
+                            96 LOAD_CONST               4 ('+')
+                            98 KW_NAMES                 5
+                           100 PRECALL                  3
+                           104 CALL                     3
+                           114 POP_TOP
+                           116 LOAD_CONST               0 (None)
+                           118 RETURN_VALUE
+               consts
+                  None
+                  code
+                     argcount  : 1
+                     nlocals   : 1
+                     stacksize : 2
+                     flags     : 19
+                     code
+                        0x97007c006a0000000000000000007c006a010000000000000000630261
+                        00610164005300
+                      83           0 RESUME                   0
+                     
+                      85           2 LOAD_FAST                0 (event)
+                                   4 LOAD_ATTR                0 (x)
+                                  14 LOAD_FAST                0 (event)
+                                  16 LOAD_ATTR                1 (y)
+                                  26 SWAP                     2
+                                  28 STORE_GLOBAL             0 (x)
+                                  30 STORE_GLOBAL             1 (y)
+                                  32 LOAD_CONST               0 (None)
+                                  34 RETURN_VALUE
+                     consts
+                        None
+                     names      ('x', 'y')
+                     varnames   ('event',)
+                     freevars   ()
+                     cellvars   ()
+                     filename   'D:\\tkadw\\tkadw\\windows\\widgets\\adw.py'
+                     name       '_click'
+                     firstlineno 83
+                     lnotab 0x0202
+                  code
+                     argcount  : 1
+                     nlocals   : 4
+                     stacksize : 4
+                     flags     : 19
+                     code
+                        0x950197007c006a0000000000000000007400000000000000000000007a
+                        0a00008904a0010000000000000000000000000000000000000000a60000
+                        00ab0000000000000000007a0000007d017c006a02000000000000000074
+                        04000000000000000000007a0a00008904a0030000000000000000000000
+                        000000000000000000a6000000ab0000000000000000007a0000007d0264
+                        017c019b0064017c029b009d047d038904a0040000000000000000000000
+                        0000000000000000007c03a6010000ab0100000000000000000100640053
+                        00
+                                   0 COPY_FREE_VARS           1
+                     
+                      87           2 RESUME                   0
+                     
+                      88           4 LOAD_FAST                0 (event)
+                                   6 LOAD_ATTR                0 (x)
+                                  16 LOAD_GLOBAL              0 (x)
+                                  28 BINARY_OP               10 (-)
+                                  32 LOAD_DEREF               4 (self)
+                                  34 LOAD_METHOD              1 (winfo_x)
+                                  56 PRECALL                  0
+                                  60 CALL                     0
+                                  70 BINARY_OP                0 (+)
+                                  74 STORE_FAST               1 (new_x)
+                     
+                      89          76 LOAD_FAST                0 (event)
+                                  78 LOAD_ATTR                2 (y)
+                                  88 LOAD_GLOBAL              4 (y)
+                                 100 BINARY_OP               10 (-)
+                                 104 LOAD_DEREF               4 (self)
+                                 106 LOAD_METHOD              3 (winfo_y)
+                                 128 PRECALL                  0
+                                 132 CALL                     0
+                                 142 BINARY_OP                0 (+)
+                                 146 STORE_FAST               2 (new_y)
+                     
+                      90         148 LOAD_CONST               1 ('+')
+                                 150 LOAD_FAST                1 (new_x)
+                                 152 FORMAT_VALUE             0
+                                 154 LOAD_CONST               1 ('+')
+                                 156 LOAD_FAST                2 (new_y)
+                                 158 FORMAT_VALUE             0
+                                 160 BUILD_STRING             4
+                                 162 STORE_FAST               3 (s)
+                     
+                      91         164 LOAD_DEREF               4 (self)
+                                 166 LOAD_METHOD              4 (geometry)
+                                 188 LOAD_FAST                3 (s)
+                                 190 PRECALL                  1
+                                 194 CALL                     1
+                                 204 POP_TOP
+                                 206 LOAD_CONST               0 (None)
+                                 208 RETURN_VALUE
+                     consts
+                        None
+                        '+'
+                     names      ('x', 'winfo_x', 'y', 'winfo_y', 'geometry')
+                     varnames   ('event', 'new_x', 'new_y', 's')
+                     freevars   ('self',)
+                     cellvars   ()
+                     filename   'D:\\tkadw\\tkadw\\windows\\widgets\\adw.py'
+                     name       '_move'
+                     firstlineno 87
+                     lnotab 0x0401480148011001
+                  '<Button-1>'
+                  '+'
+                  ('add',)
+                  '<B1-Motion>'
+               names      ('bind',)
+               varnames   ('self', 'widget', '_click', '_move')
+               freevars   ()
+               cellvars   ('self',)
+               filename   'D:\\tkadw\\tkadw\\windows\\widgets\\adw.py'
+               name       'bind_move'
+               firstlineno 82
+               lnotab 0x040106040a063001
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-                64           0 RESUME                   0
+                96           0 RESUME                   0
                
-                65           2 LOAD_CONST               0 (None)
+                97           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\widgets\\adw.py'
                name       'default_palette'
-               firstlineno 64
+               firstlineno 96
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007c01812864017c01760072267c00a0000000000000000000000000
                   0000000000000000007c0164011900000000000000000064021900000000
                   0000000000ac03a6010000ab010000000000000000010064005300640053
                   0064005300
-                67           0 RESUME                   0
+                99           0 RESUME                   0
                
-                68           2 LOAD_FAST                1 (dict)
+               100           2 LOAD_FAST                1 (dict)
                              4 POP_JUMP_FORWARD_IF_NONE    40 (to 86)
                
-                69           6 LOAD_CONST               1 ('window')
+               101           6 LOAD_CONST               1 ('window')
                              8 LOAD_FAST                1 (dict)
                             10 CONTAINS_OP              0
                             12 POP_JUMP_FORWARD_IF_FALSE    38 (to 90)
                
-                70          14 LOAD_FAST                0 (self)
+               102          14 LOAD_FAST                0 (self)
                             16 LOAD_METHOD              0 (configure)
                             38 LOAD_FAST                1 (dict)
                             40 LOAD_CONST               1 ('window')
                             42 BINARY_SUBSCR
                             52 LOAD_CONST               2 ('back')
                             54 BINARY_SUBSCR
                             64 KW_NAMES                 3
                             66 PRECALL                  1
                             70 CALL                     1
                             80 POP_TOP
                             82 LOAD_CONST               0 (None)
                             84 RETURN_VALUE
                
-                68     >>   86 LOAD_CONST               0 (None)
+               100     >>   86 LOAD_CONST               0 (None)
                             88 RETURN_VALUE
                
-                69     >>   90 LOAD_CONST               0 (None)
+               101     >>   90 LOAD_CONST               0 (None)
                             92 RETURN_VALUE
                consts
                   None
                   'window'
                   'back'
                   ('background',)
                names      ('configure',)
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\widgets\\adw.py'
                name       'palette'
-               firstlineno 67
+               firstlineno 99
                lnotab 0x02010401080148fe0401
-         names      ('__name__', '__module__', '__qualname__', 'str', 'bool', '__init__', 'default_palette', 'palette', '__classcell__')
+            ('#0a080a',)
+         names      ('__name__', '__module__', '__qualname__', 'str', 'bool', '__init__', 'custom', 'bind_move', 'default_palette', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\widgets\\adw.py'
          name       'Adw'
          firstlineno 4
-         lnotab 0x0c01203b0603
+         lnotab 0x0c01203b0812060e0603
       'Adw'
-      '__main__'
-      'light'
-      ('icon',)
       None
-   names      ('tkinter', 'Tk', 'Adw', '__name__', 'root', 'mainloop')
+   names      ('tkinter', 'Tk', 'Adw')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\windows\\widgets\\adw.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c031c450c0118012cfe
+   lnotab 0x00ff02010c03
```

### Comparing `tkadw-0.3.2/tkadw/windows/widgets/__pycache__/label.cpython-310.pyc` & `tkadw-0.3.3/tkadw/windows/widgets/__pycache__/label.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/widgets/__pycache__/label.cpython-311.pyc` & `tkadw-0.3.3/tkadw/windows/widgets/__pycache__/label.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/widgets/__pycache__/mdi.cpython-311.pyc` & `tkadw-0.3.3/tkadw/windows/widgets/__pycache__/mdi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/widgets/adw.py` & `tkadw-0.3.3/tkadw/windows/widgets/adw.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,19 +57,47 @@
         if platform == "win32" and wincaption is not None:
             from sys import platform
             from ctypes import windll, byref, sizeof, c_int
             from ctypes.wintypes import RGB
             windll.dwmapi.DwmSetWindowAttribute(windll.user32.GetParent(self.winfo_id()), 35, byref(c_int(RGB(wincaption[0], wincaption[1], wincaption[2]))),
                                                 sizeof(c_int))
 
+    def custom(self, tcolor="#0a080a"):
+        from tkadw.windows.theme import AdwTFrame
+        self.overrideredirect(True)
+
+        from sys import platform
+
+        self.frame = AdwTFrame()
+        self.frame.pack(fill="both", expand="yes")
+        self.frame.configure(background=tcolor)
+
+        if platform == "win32":
+            self.attributes("-transparentcolor", tcolor)
+        else:
+            self.frame.frame_radius = 0
+            self.frame.update()
+
+        self.wm_attributes("-topmost", True)
+
+    def bind_move(self, widget):
+        def _click(event):
+            global x, y
+            x, y = event.x, event.y
+
+        def _move(event):
+            new_x = (event.x - x) + self.winfo_x()
+            new_y = (event.y - y) + self.winfo_y()
+            s = f"+{new_x}+{new_y}"
+            self.geometry(s)
+
+        widget.bind("<Button-1>", _click, add="+")
+        widget.bind("<B1-Motion>", _move, add="+")
+
     def default_palette(self):
         pass
 
     def palette(self, dict):
         if dict is not None:
             if "window" in dict:
                 self.configure(background=dict["window"]["back"])
 
-
-if __name__ == '__main__':
-    root = Adw(icon="light")
-    root.mainloop()
```

### Comparing `tkadw-0.3.2/tkadw/windows/widgets/label.py` & `tkadw-0.3.3/tkadw/windows/widgets/label.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/tkadw/windows/widgets/mdi.py` & `tkadw-0.3.3/tkadw/windows/widgets/mdi.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.2/PKG-INFO` & `tkadw-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkadw
-Version: 0.3.2
+Version: 0.3.3
 Summary: extra for tkinter
 License: MIT
 Author: XiangQinxi
 Author-email: 1379773753@qq.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -91,7 +91,12 @@
 > 
 >> `304`新增主题类组件，只需使用`set_default_theme`设置主题。对于经过特殊设计和特殊样式的组件，比如`Fluent`主题组件、`Win11`主题控件`AccentButton`，将不加入主题变量内
 
 > `0.3.2`
 >> `321` 新增`AdwMDI`组件
 > 
 >> `322` 添加`metro`主题
+
+> `0.3.3`
+>> `331` 修复`AdwDrawFrame`的边框宽度问题
+> 
+>> `332` 增加主题属性`AdwDrawFrame` `padding`
```

