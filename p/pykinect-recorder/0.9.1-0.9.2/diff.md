# Comparing `tmp/pykinect_recorder-0.9.1.tar.gz` & `tmp/pykinect_recorder-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykinect_recorder-0.9.1.tar", max compression
+gzip compressed data, was "pykinect_recorder-0.9.2.tar", max compression
```

## Comparing `pykinect_recorder-0.9.1.tar` & `pykinect_recorder-0.9.2.tar`

### file list

```diff
@@ -1,76 +1,65 @@
--rw-r--r--   0        0        0        0 2023-03-18 05:42:01.519001 pykinect_recorder-0.9.1/LICENSE
--rw-r--r--   0        0        0       44 2023-03-21 13:06:28.655627 pykinect_recorder-0.9.1/pykinect_recorder/__init__.py
--rw-r--r--   0        0        0       87 2023-03-21 13:06:28.656629 pykinect_recorder-0.9.1/pykinect_recorder/main/__init__.py
--rw-r--r--   0        0        0       65 2023-03-21 13:06:28.657627 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/__init__.py
--rw-r--r--   0        0        0      264 2023-03-21 13:06:28.658628 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4a/__init__.py
--rw-r--r--   0        0        0    37544 2023-03-21 13:06:28.659628 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4a/_k4a.py
--rw-r--r--   0        0        0    11407 2023-04-27 05:17:40.159181 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4a/_k4atypes.py
--rw-r--r--   0        0        0     5639 2023-03-21 13:06:28.661630 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4a/calibration.py
--rw-r--r--   0        0        0     4160 2023-03-21 13:06:28.661630 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4a/capture.py
--rw-r--r--   0        0        0     4082 2023-04-27 05:17:40.160180 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4a/configuration.py
--rw-r--r--   0        0        0     6063 2023-03-21 13:06:28.663628 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4a/device.py
--rw-r--r--   0        0        0     5074 2023-03-21 13:06:28.664628 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4a/image.py
--rw-r--r--   0        0        0     1573 2023-03-21 13:06:28.664628 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4a/imu_sample.py
--rw-r--r--   0        0        0     4402 2023-03-21 13:06:28.665628 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4a/transformation.py
--rw-r--r--   0        0        0      164 2023-03-21 13:06:28.666628 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4abt/__init__.py
--rw-r--r--   0        0        0     8794 2023-03-21 13:06:28.667627 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4abt/_k4abt.py
--rw-r--r--   0        0        0     8268 2023-03-21 13:06:28.668628 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4abt/_k4abtTypes.py
--rw-r--r--   0        0        0     1146 2023-03-21 13:06:28.669628 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4abt/body.py
--rw-r--r--   0        0        0     3012 2023-03-21 13:06:28.670627 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4abt/body2d.py
--rw-r--r--   0        0        0     4620 2023-03-21 13:06:28.671628 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4abt/frame.py
--rw-r--r--   0        0        0     1617 2023-03-21 13:06:28.672629 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4abt/joint.py
--rw-r--r--   0        0        0     1228 2023-03-21 13:06:28.672629 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4abt/joint2d.py
--rw-r--r--   0        0        0     3223 2023-03-21 13:06:28.673629 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4abt/tracker.py
--rw-r--r--   0        0        0      149 2023-03-21 13:06:28.674627 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4arecord/__init__.py
--rw-r--r--   0        0        0    20479 2023-03-21 13:06:28.675628 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4arecord/_k4arecord.py
--rw-r--r--   0        0        0     2339 2023-03-21 13:06:28.676627 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4arecord/_k4arecordTypes.py
--rw-r--r--   0        0        0      952 2023-03-21 13:06:28.677628 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4arecord/datablock.py
--rw-r--r--   0        0        0     5495 2023-03-21 13:06:28.678628 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4arecord/playback.py
--rw-r--r--   0        0        0     1831 2023-03-21 13:06:28.679629 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4arecord/record.py
--rw-r--r--   0        0        0     2153 2023-03-21 13:06:28.679629 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4arecord/record_configuration.py
--rw-r--r--   0        0        0     2067 2023-03-21 13:06:28.680627 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/pykinect.py
--rw-r--r--   0        0        0       96 2023-03-21 13:06:28.681627 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/utils/__init__.py
--rw-r--r--   0        0        0     1175 2023-03-21 13:06:28.682628 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/utils/plot3dUtils.py
--rw-r--r--   0        0        0      917 2023-03-21 13:06:28.683628 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/utils/postProcessing.py
--rw-r--r--   0        0        0     2472 2023-03-21 13:06:28.683628 pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/utils/utils.py
--rw-r--r--   0        0        0        0 2023-03-21 13:06:28.684628 pykinect_recorder-0.9.1/pykinect_recorder/main/cli/__init__.py
--rw-r--r--   0        0        0      616 2023-03-21 13:06:28.685628 pykinect_recorder-0.9.1/pykinect_recorder/main/cli/command.py
--rw-r--r--   0        0        0     1814 2023-03-21 13:06:28.686628 pykinect_recorder-0.9.1/pykinect_recorder/main/logger.py
--rw-r--r--   0        0        0     9127 2023-04-27 03:18:54.866909 pykinect_recorder-0.9.1/pykinect_recorder/main/old_record_video.py
--rw-r--r--   0        0        0     3533 2023-04-27 03:18:54.867909 pykinect_recorder-0.9.1/pykinect_recorder/main/playback_sensors.py
--rw-r--r--   0        0        0     5527 2023-04-27 03:18:54.868912 pykinect_recorder-0.9.1/pykinect_recorder/main/pyk4a_thread.py
--rw-r--r--   0        0        0     6109 2023-03-21 13:06:28.688629 pykinect_recorder-0.9.1/pykinect_recorder/main/record_audio.py
--rw-r--r--   0        0        0     3021 2023-04-27 03:18:54.870422 pykinect_recorder-0.9.1/pykinect_recorder/main/record_video.py
--rw-r--r--   0        0        0     2539 2023-03-21 13:06:28.689628 pykinect_recorder-0.9.1/pykinect_recorder/main/synology_utils.py
--rw-r--r--   0        0        0     2436 2023-04-27 05:17:40.162181 pykinect_recorder-0.9.1/pykinect_recorder/main_window.py
--rw-r--r--   0        0        0     1267 2023-04-27 03:18:54.865909 pykinect_recorder-0.9.1/pykinect_recorder/README.md
--rw-r--r--   0        0        0       60 2023-04-27 03:18:54.872428 pykinect_recorder-0.9.1/pykinect_recorder/renderer/__init__.py
--rw-r--r--   0        0        0     4909 2023-04-27 05:17:40.163181 pykinect_recorder-0.9.1/pykinect_recorder/renderer/common_widgets.py
--rw-r--r--   0        0        0       15 2023-03-21 13:06:28.691630 pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/__init__.py
--rw-r--r--   0        0        0      312 2023-04-27 05:17:40.164181 pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/asidebar.py
--rw-r--r--   0        0        0     2936 2023-04-27 05:17:40.165180 pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/playback_sensors.py
--rw-r--r--   0        0        0     5365 2023-04-27 05:17:40.166687 pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/record_sensors.py
--rw-r--r--   0        0        0     1195 2023-04-27 03:18:54.876425 pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/sidebar_control.py
--rw-r--r--   0        0        0     3623 2023-04-27 05:24:39.738523 pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/sidebar_explorer.py
--rw-r--r--   0        0        0     3096 2023-04-27 05:17:40.170701 pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/sidebar_menu.py
--rw-r--r--   0        0        0    14390 2023-04-27 05:17:40.171703 pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/sidebar_record_control.py
--rw-r--r--   0        0        0      147 2023-04-27 03:18:54.880939 pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/sidebar_solutions.py
--rw-r--r--   0        0        0      303 2023-04-27 05:17:40.167694 pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/sidebarBtn.stylesheet
--rw-r--r--   0        0        0     1894 2023-04-27 05:17:40.172700 pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/toolbar.py
--rw-r--r--   0        0        0     1456 2023-04-27 05:17:40.173704 pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/viewer_audio.py
--rw-r--r--   0        0        0     1245 2023-04-27 05:17:40.175701 pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/viewer_control.py
--rw-r--r--   0        0        0     2053 2023-04-27 05:17:40.176702 pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/viewer_imu_sensors.py
--rw-r--r--   0        0        0     5793 2023-04-28 09:01:52.639672 pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/viewer_playback.py
--rw-r--r--   0        0        0    13649 2023-04-27 05:17:40.179224 pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/viewer_sensors.py
--rw-r--r--   0        0        0      243 2023-04-27 03:18:54.887939 pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/viewer_solution.py
--rw-r--r--   0        0        0     6528 2023-04-27 05:17:40.180226 pykinect_recorder-0.9.1/pykinect_recorder/renderer/public/ai.png
--rw-r--r--   0        0        0     3867 2023-04-27 05:17:40.181224 pykinect_recorder-0.9.1/pykinect_recorder/renderer/public/ai.svg
--rw-r--r--   0        0        0     1808 2023-04-27 05:17:40.182226 pykinect_recorder-0.9.1/pykinect_recorder/renderer/public/file.png
--rw-r--r--   0        0        0     1564 2023-04-27 05:17:40.184225 pykinect_recorder-0.9.1/pykinect_recorder/renderer/public/file.svg
--rw-r--r--   0        0        0    48895 2023-03-21 13:06:28.698628 pykinect_recorder-0.9.1/pykinect_recorder/renderer/public/kinect-sensor.ico
--rw-r--r--   0        0        0     2456 2023-04-27 05:17:40.185224 pykinect_recorder-0.9.1/pykinect_recorder/renderer/public/search.png
--rw-r--r--   0        0        0     1129 2023-04-27 05:17:40.185224 pykinect_recorder-0.9.1/pykinect_recorder/renderer/public/search.svg
--rw-r--r--   0        0        0      823 2023-04-27 05:17:40.186732 pykinect_recorder-0.9.1/pykinect_recorder/renderer/signals.py
--rw-r--r--   0        0        0     1356 2023-04-28 09:03:31.863374 pykinect_recorder-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      509 2023-04-12 12:39:20.808090 pykinect_recorder-0.9.1/README.md
--rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 pykinect_recorder-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-07-16 11:33:01.031615 pykinect_recorder-0.9.2/LICENSE
+-rw-r--r--   0        0        0       46 2023-07-16 11:32:31.458067 pykinect_recorder-0.9.2/pykinect_recorder/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:33:01.055130 pykinect_recorder-0.9.2/pykinect_recorder/cli/__init__.py
+-rw-r--r--   0        0        0      592 2023-07-16 11:33:01.056126 pykinect_recorder-0.9.2/pykinect_recorder/cli/command.py
+-rw-r--r--   0        0        0     3209 2023-07-16 11:33:01.057126 pykinect_recorder-0.9.2/pykinect_recorder/dev/record_sensors.py
+-rw-r--r--   0        0        0     3626 2023-07-16 11:33:01.058127 pykinect_recorder-0.9.2/pykinect_recorder/main_window.py
+-rw-r--r--   0        0        0      414 2023-07-16 11:33:01.058127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/__init__.py
+-rw-r--r--   0        0        0      266 2023-07-16 11:33:01.059128 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/__init__.py
+-rw-r--r--   0        0        0    90759 2023-07-16 11:33:01.060127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/_k4a.py
+-rw-r--r--   0        0        0    19864 2023-07-16 11:33:01.061127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/_k4atypes.py
+-rw-r--r--   0        0        0     8322 2023-07-16 11:33:01.062127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/calibration.py
+-rw-r--r--   0        0        0     4097 2023-07-16 11:33:01.062127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/capture.py
+-rw-r--r--   0        0        0     4004 2023-07-16 11:33:01.063127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/configuration.py
+-rw-r--r--   0        0        0     6625 2023-07-16 11:33:01.064127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/device.py
+-rw-r--r--   0        0        0     4774 2023-07-16 11:33:01.065128 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/image.py
+-rw-r--r--   0        0        0     1575 2023-07-16 11:33:01.065128 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/imu_sample.py
+-rw-r--r--   0        0        0     4386 2023-07-16 11:33:01.066128 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/transformation.py
+-rw-r--r--   0        0        0      164 2023-07-16 11:33:01.067127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/__init__.py
+-rw-r--r--   0        0        0    18158 2023-07-16 11:33:01.067127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/_k4abt.py
+-rw-r--r--   0        0        0    11712 2023-07-16 11:33:01.068127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/_k4abtTypes.py
+-rw-r--r--   0        0        0     1146 2023-07-16 11:33:01.069126 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/body.py
+-rw-r--r--   0        0        0     2948 2023-07-16 11:33:01.069126 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/body2d.py
+-rw-r--r--   0        0        0     4468 2023-07-16 11:33:01.070125 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/frame.py
+-rw-r--r--   0        0        0     1617 2023-07-16 11:33:01.071126 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/joint.py
+-rw-r--r--   0        0        0     1228 2023-07-16 11:33:01.071126 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/joint2d.py
+-rw-r--r--   0        0        0     3079 2023-07-16 11:33:01.072126 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/tracker.py
+-rw-r--r--   0        0        0      149 2023-07-16 11:33:01.072126 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/__init__.py
+-rw-r--r--   0        0        0    20837 2023-07-16 11:33:01.073161 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/_k4arecord.py
+-rw-r--r--   0        0        0     2344 2023-07-16 11:33:01.074127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/_k4arecordTypes.py
+-rw-r--r--   0        0        0      928 2023-07-16 11:33:01.074127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/datablock.py
+-rw-r--r--   0        0        0     5984 2023-07-16 11:33:01.075127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/playback.py
+-rw-r--r--   0        0        0     2182 2023-07-16 11:33:01.075127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/record.py
+-rw-r--r--   0        0        0     2153 2023-07-16 11:33:01.076127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/record_configuration.py
+-rw-r--r--   0        0        0     2049 2023-07-16 11:33:01.077125 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/pykinect.py
+-rw-r--r--   0        0        0     5587 2023-07-16 11:33:01.077125 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/utils.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:33:01.078126 pykinect_recorder-0.9.2/pykinect_recorder/pyrealsense/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:33:01.078126 pykinect_recorder-0.9.2/pykinect_recorder/pyzenmuse/__init__.py
+-rw-r--r--   0        0        0       56 2023-07-16 11:32:31.495067 pykinect_recorder-0.9.2/pykinect_recorder/renderer/__init__.py
+-rw-r--r--   0        0        0     9847 2023-07-16 11:33:01.079126 pykinect_recorder-0.9.2/pykinect_recorder/renderer/common_widgets.py
+-rw-r--r--   0        0        0       17 2023-07-16 11:32:31.496068 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/__init__.py
+-rw-r--r--   0        0        0     2824 2023-07-16 11:33:01.080178 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/playback_sensors.py
+-rw-r--r--   0        0        0     3348 2023-07-16 11:33:01.081127 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/record_sensors.py
+-rw-r--r--   0        0        0     1351 2023-07-16 11:33:01.082127 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/sidebar_control.py
+-rw-r--r--   0        0        0     6585 2023-07-16 11:33:01.083126 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/sidebar_explorer.py
+-rw-r--r--   0        0        0     3795 2023-07-16 11:33:01.083126 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/sidebar_menu.py
+-rw-r--r--   0        0        0    27968 2023-07-16 11:33:01.084128 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/sidebar_record_control.py
+-rw-r--r--   0        0        0      135 2023-07-16 11:32:31.503069 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/sidebar_solutions.py
+-rw-r--r--   0        0        0     2201 2023-07-16 11:33:01.085130 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/statusbar.py
+-rw-r--r--   0        0        0     4680 2023-07-16 11:33:01.085130 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/topbar.py
+-rw-r--r--   0        0        0      797 2023-07-16 11:33:01.086127 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_3dsensors.py
+-rw-r--r--   0        0        0     1964 2023-07-16 11:33:01.087127 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_audio.py
+-rw-r--r--   0        0        0     1511 2023-07-16 11:33:01.087127 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_control.py
+-rw-r--r--   0        0        0     2980 2023-07-16 11:33:01.088127 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_imu_sensors.py
+-rw-r--r--   0        0        0    12170 2023-07-16 11:33:01.089128 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_playback.py
+-rw-r--r--   0        0        0    11462 2023-07-16 11:33:01.090125 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_sensors.py
+-rw-r--r--   0        0        0      235 2023-07-16 11:32:31.508067 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_solution.py
+-rw-r--r--   0        0        0    12459 2023-07-16 11:33:01.090125 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_video_clipping.py
+-rw-r--r--   0        0        0     1802 2023-07-16 11:33:01.091125 pykinect_recorder-0.9.2/pykinect_recorder/renderer/logger.py
+-rw-r--r--   0        0        0    48895 2023-03-21 13:06:28.698628 pykinect_recorder-0.9.2/pykinect_recorder/renderer/public/kinect-sensor.ico
+-rw-r--r--   0        0        0     1646 2023-07-16 11:33:01.092126 pykinect_recorder-0.9.2/pykinect_recorder/renderer/signals.py
+-rw-r--r--   0        0        0     2943 2023-07-16 11:33:01.092126 pykinect_recorder-0.9.2/pykinect_recorder/renderer/split_data.py
+-rw-r--r--   0        0        0     2483 2023-07-16 11:33:01.093126 pykinect_recorder-0.9.2/pykinect_recorder/renderer/synology_utils.py
+-rw-r--r--   0        0        0     1561 2023-07-16 11:34:44.967052 pykinect_recorder-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2436 2023-07-16 11:33:01.033614 pykinect_recorder-0.9.2/README.md
+-rw-r--r--   0        0        0     4491 1970-01-01 00:00:00.000000 pykinect_recorder-0.9.2/PKG-INFO
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4a/calibration.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/calibration.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import ctypes
 
 from . import _k4a
 
 
 class Calibration:
+    """
+    Wrapper for `k4a_calibration_t`.
+
+    Provides member functions for `k4a_calibration_t`.
+    """
+
     def __init__(self, calibration_handle: _k4a.k4a_calibration_t):
         self._handle = calibration_handle
-        self.color_params = (
-            self._handle.color_camera_calibration.intrinsics.parameters.param
-        )
-        self.depth_params = (
-            self._handle.depth_camera_calibration.intrinsics.parameters.param
-        )
+        self.color_params = self._handle.color_camera_calibration.intrinsics.parameters.param
+        self.depth_params = self._handle.depth_camera_calibration.intrinsics.parameters.param
 
     def __del__(self):
         self.reset()
 
     def __str__(self):
         message = (
             "Rgb Intrinsic parameters: \n"
@@ -57,21 +59,38 @@
     def handle(self):
         return self._handle
 
     def reset(self):
         if self.is_valid():
             self._handle = None
 
-    # 3D point of source_camera to 3D point of target_camera  
+    # 3D point of source_camera to 3D point of target_camera
     def convert_3d_to_3d(
         self,
-        source_point3d: _k4a.k4a_float3_t(),
+        source_point3d: _k4a.k4a_float3_t,
         source_camera: _k4a.k4a_calibration_type_t,
         target_camera: _k4a.k4a_calibration_type_t,
-    ) -> _k4a.k4a_float3_t():
+    ) -> _k4a.k4a_float3_t:
+        """
+        Transform a 3d point of a source coordinate system into a 3d point of the target coordinate system.
+
+        Throws error on failure.
+
+        Note:
+            See also `k4a_calibration_3d_to_3d()`.
+
+        Args:
+            source_point3d (k4a_float3_t): The 3D coordinates in millimeters representing a point
+                in `source_camera`.
+            source_camera (k4a_calibration_type_t): The current camera.
+            target_camera (k4a_calibration_type_t): The target camera.
+
+        Returns:
+            k4a_float3_t: Three dimensional floating point vector.
+        """
         target_point3d = _k4a.k4a_float3_t()
 
         _k4a.VERIFY(
             _k4a.k4a_calibration_3d_to_3d(
                 self._handle,
                 source_point3d,
                 source_camera,
@@ -86,15 +105,33 @@
     # 2D depth of source_camera to 3D point of target_camera
     def convert_2d_to_3d(
         self,
         source_point2d: _k4a.k4a_float2_t,
         source_depth: float,
         source_camera: _k4a.k4a_calibration_type_t,
         target_camera: _k4a.k4a_calibration_type_t,
-    ) -> _k4a.k4a_float3_t():
+    ) -> _k4a.k4a_float3_t:
+        """
+        Transform a 2d pixel coordinate with an associated depth value of the source camera
+        into a 3d point of the target coordinate system.
+
+        Returns false if the point is invalid in the target coordinate system
+        (and therefore target_point3d should not be used) Throws error if calibration contains
+        invalid data.
+
+        Args:
+            source_point2d (_k4a.k4a_float2_t): The 2D pixel in `source_camera` coordinates.
+            source_depth (float): The depth of `source_point2d` in millimeters. One way to derive the
+                depth value in the color camera geometry is to use the function `k4a_transformation_depth_image_to_color_camera()`.
+            source_camera (_k4a.k4a_calibration_type_t): The current camera.
+            target_camera (_k4a.k4a_calibration_type_t): The target camera.
+
+        Returns:
+            _k4a.k4a_float3_t: Three dimensional floating point vector.
+        """
         target_point3d = _k4a.k4a_float3_t()
         valid = ctypes.c_int()
 
         _k4a.VERIFY(
             _k4a.k4a_calibration_2d_to_3d(
                 self._handle,
                 source_point2d,
@@ -111,15 +148,31 @@
 
     # 3D point of source_camera to 2D pixel of target_camera
     def convert_3d_to_2d(
         self,
         source_point3d: _k4a.k4a_float3_t,
         source_camera: _k4a.k4a_calibration_type_t,
         target_camera: _k4a.k4a_calibration_type_t,
-    ) -> _k4a.k4a_float2_t():
+    ) -> _k4a.k4a_float2_t:
+        """
+        Transform a 3d point of a source coordinate system into a 2d pixel coordinate of the target
+        camera.
+
+        Returns false if the point is invalid in the target coordinate system
+        (and therefore target_point2d should not be used) Throws error if calibration contains invalid data.
+
+        Args:
+            source_point3d (_k4a.k4a_float3_t): The 3D coordinates in millimeters representing
+                a point in source_camera.
+            source_camera (_k4a.k4a_calibration_type_t): _description_
+            target_camera (_k4a.k4a_calibration_type_t): _description_
+
+        Returns:
+            _k4a.k4a_float2_t: _description_
+        """
         target_point2d = _k4a.k4a_float2_t()
         valid = ctypes.c_int()
 
         _k4a.VERIFY(
             _k4a.k4a_calibration_3d_to_2d(
                 self._handle,
                 source_point3d,
@@ -136,15 +189,27 @@
     # 2D depth of source_camera to 2D pixel of target_camera
     def convert_2d_to_2d(
         self,
         source_point2d: _k4a.k4a_float2_t,
         source_depth: float,
         source_camera: _k4a.k4a_calibration_type_t,
         target_camera: _k4a.k4a_calibration_type_t,
-    ) -> _k4a.k4a_float2_t():
+    ) -> _k4a.k4a_float2_t:
+        """
+
+
+        Args:
+            source_point2d (_k4a.k4a_float2_t): _description_
+            source_depth (float): _description_
+            source_camera (_k4a.k4a_calibration_type_t): _description_
+            target_camera (_k4a.k4a_calibration_type_t): _description_
+
+        Returns:
+            _k4a.k4a_float2_t: _description_
+        """
         target_point2d = _k4a.k4a_float2_t()
         valid = ctypes.c_int()
 
         _k4a.VERIFY(
             _k4a.k4a_calibration_2d_to_2d(
                 self._handle,
                 source_point2d,
@@ -155,22 +220,20 @@
                 valid,
             ),
             "Failed to convert from 2D to 2D",
         )
 
         return target_point2d
 
-    # 2D pixel of color_camera to 2D pixel of depth camera 
+    # 2D pixel of color_camera to 2D pixel of depth camera
     def convert_color_2d_to_depth_2d(
         self, source_point2d: _k4a.k4a_float2_t, depth_image: _k4a.k4a_image_t
-    ) -> _k4a.k4a_float2_t():
+    ) -> _k4a.k4a_float2_t:
         target_point2d = _k4a.k4a_float2_t()
         valid = ctypes.c_int()
 
         _k4a.VERIFY(
-            _k4a.k4a_calibration_color_2d_to_depth_2d(
-                self._handle, source_point2d, depth_image, target_point2d, valid
-            ),
+            _k4a.k4a_calibration_color_2d_to_depth_2d(self._handle, source_point2d, depth_image, target_point2d, valid),
             "Failed to convert from Color 2D to Depth 2D",
         )
 
         return target_point2d
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4a/capture.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import cv2
 
 from . import _k4a
 from .image import Image
 from .transformation import Transformation
-from ..utils.postProcessing import smooth_depth_image
+from ..utils import smooth_depth_image
 
 
 class Capture:
     def __init__(self, capture_handle, calibration):
         self._handle = capture_handle
         self.calibration = calibration
         self.camera_transform = Transformation(calibration)
@@ -43,27 +43,23 @@
     def get_depth_image_object(self):
         return Image(_k4a.k4a_capture_get_depth_image(self._handle))
 
     def get_ir_image_object(self):
         return Image(_k4a.k4a_capture_get_ir_image(self._handle))
 
     def get_transformed_depth_object(self):
-        return self.camera_transform.depth_image_to_color_camera(
-            self.get_depth_image_object()
-        )
+        return self.camera_transform.depth_image_to_color_camera(self.get_depth_image_object())
 
     def get_transformed_color_object(self):
         return self.camera_transform.color_image_to_depth_camera(
             self.get_depth_image_object(), self.get_color_image_object()
         )
 
     def get_pointcloud_object(self, calibration_type=_k4a.K4A_CALIBRATION_TYPE_DEPTH):
-        return self.camera_transform.depth_image_to_point_cloud(
-            self.get_depth_image_object(), calibration_type
-        )
+        return self.camera_transform.depth_image_to_point_cloud(self.get_depth_image_object(), calibration_type)
 
     def get_transformed_pointcloud_object(self):
         return self.camera_transform.depth_image_to_point_cloud(
             self.get_transformed_depth_object(), _k4a.K4A_CALIBRATION_TYPE_COLOR
         )
 
     def get_color_image(self):
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4a/configuration.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,24 +54,18 @@
 
     def create_from_handle(self, configuration_handle):
         self.color_format = configuration_handle.color_format
         self.color_resolution = configuration_handle.color_resolution
         self.depth_mode = configuration_handle.depth_mode
         self.camera_fps = configuration_handle.camera_fps
         self.synchronized_images_only = configuration_handle.synchronized_images_only
-        self.depth_delay_off_color_usec = (
-            configuration_handle.depth_delay_off_color_usec
-        )
+        self.depth_delay_off_color_usec = configuration_handle.depth_delay_off_color_usec
         self.wired_sync_mode = configuration_handle.wired_sync_mode
-        self.subordinate_delay_off_master_usec = (
-            configuration_handle.subordinate_delay_off_master_usec
-        )
-        self.disable_streaming_indicator = (
-            configuration_handle.disable_streaming_indicator
-        )
+        self.subordinate_delay_off_master_usec = configuration_handle.subordinate_delay_off_master_usec
+        self.disable_streaming_indicator = configuration_handle.disable_streaming_indicator
 
         self._handle = configuration_handle
 
     def on_value_change(self):
         self._handle = _k4a.k4a_device_configuration_t(
             self.color_format,
             self.color_resolution,
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4a/device.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 from . import _k4a
 from .capture import Capture
 from .imu_sample import ImuSample
 from .calibration import Calibration
 from .configuration import Configuration
 from ..k4arecord.record import Record
 from ..k4a._k4atypes import K4A_WAIT_INFINITE
+from ..k4arecord._k4arecord import k4a_playback_get_next_capture, K4A_STREAM_RESULT_EOF
 
 
 class Device:
     calibration = None
     capture = None
     imu_sample = None
     filename_video = None
 
     def __init__(self, index: int = 0) -> None:
         self._handle = None
         self._handle = self.open(index)
         self.recording = False
         self.record = False
+        self.is_imu = True
 
     def __del__(self) -> None:
         self.close()
 
     def is_valid(self) -> None:
         return self._handle
 
@@ -36,117 +38,90 @@
 
     def is_imu_sample_initialized(self) -> None:
         return Device.imu_sample
 
     def handle(self) -> None:
         return self._handle
 
-    def start(
-        self, 
-        configuration: Configuration,
-        record=False,
-        record_filepath="output.mkv"
-    ) -> None:
-        
+    def start(self, configuration: Configuration, record=False, record_filepath="output.mkv") -> None:
         self.configuration = configuration
         self.start_cameras(configuration)
         self.start_imu()
-        
+
         if record:
-            self.record = Record(
-                self._handle, self.configuration.handle(), record_filepath
-            )
+            self.record = Record(self._handle, self.configuration.handle(), record_filepath)
+            self.record.add_imu_track()
             self.recording = True
 
     def close(self) -> None:
         if self.is_valid():
-            self.stop_imu()
             self.stop_cameras()
+            self.stop_imu()
             _k4a.k4a_device_close(self._handle)
 
             # Clear members
             self._handle = None
             self.record = None
             self.recording = False
 
-    def update(
-        self, 
-        timeout_in_ms: int = K4A_WAIT_INFINITE
-    ) -> Capture:
-        
+    def update(self, timeout_in_ms: int = K4A_WAIT_INFINITE) -> Capture:
         # Get cameras capture
         capture_handle = self.get_capture(timeout_in_ms)
 
         if self.is_capture_initialized():
             Device.capture._handle = capture_handle
         else:
             Device.capture = Capture(capture_handle, Device.calibration)
 
         # Write capture if recording
         if self.recording:
             self.record.write_capture(Device.capture.handle())
 
         return Device.capture
 
-    def update_imu(
-        self,
-        timeout_in_ms: int = K4A_WAIT_INFINITE
-    ) -> ImuSample:
-        
+    def update_imu(self, timeout_in_ms: int = K4A_WAIT_INFINITE) -> ImuSample:
         # Get imu sample
         imu_sample = self.get_imu_sample(timeout_in_ms)
 
         if self.is_imu_sample_initialized():
             Device.imu_sample._struct = imu_sample
             Device.imu_sample.parse_data()
         else:
             Device.imu_sample = ImuSample(imu_sample)
 
+        if self.recording:
+            self.record.write_imu(imu_sample)
+
         return Device.imu_sample
 
-    # TODO _k4a.K4A_WAIT_INFINITE는 없는데 ?
-    def get_capture(
-        self,
-        timeout_in_ms: int = K4A_WAIT_INFINITE
-    ) -> _k4a.ctypes.POINTER:
-        
+    def get_capture(self, timeout_in_ms: int = K4A_WAIT_INFINITE) -> _k4a.ctypes.POINTER:
         # Release current handle
         if self.is_capture_initialized():
             Device.capture.release_handle()
 
         capture_handle = _k4a.k4a_capture_t()
         _k4a.VERIFY(
             _k4a.k4a_device_get_capture(self._handle, capture_handle, timeout_in_ms),
             "Get capture failed!",
         )
 
         return capture_handle
 
-    def get_imu_sample(
-        self,
-        timeout_in_ms: int = K4A_WAIT_INFINITE
-    ) -> _k4a.k4a_imu_sample_t:
-        
+    def get_imu_sample(self, timeout_in_ms: int = K4A_WAIT_INFINITE) -> _k4a.k4a_imu_sample_t:
         imu_sample = _k4a.k4a_imu_sample_t()
 
         _k4a.VERIFY(
             _k4a.k4a_device_get_imu_sample(self._handle, imu_sample, timeout_in_ms),
             "Get IMU failed!",
         )
 
         return imu_sample
 
-    def start_cameras(
-        self,
-        device_config: Configuration
-    ) -> None:
-
-        Device.calibration = self.get_calibration(
-            device_config.depth_mode, device_config.color_resolution
-        )
+    def start_cameras(self, device_config: Configuration) -> None:
+        Device.calibration = self.get_calibration(device_config.depth_mode, device_config.color_resolution)
 
         _k4a.VERIFY(
             _k4a.k4a_device_start_cameras(self._handle, device_config.handle()),
             "Start K4A cameras failed!",
         )
 
     def stop_cameras(self) -> None:
@@ -156,62 +131,72 @@
         _k4a.VERIFY(_k4a.k4a_device_start_imu(self._handle), "Start K4A IMU failed!")
 
     def stop_imu(self) -> None:
         _k4a.k4a_device_stop_imu(self._handle)
 
     # get device serial number
     def get_serialnum(self) -> ctypes.c_int:
-        
         serial_number_size = ctypes.c_size_t()
         result = _k4a.k4a_device_get_serialnum(self._handle, None, serial_number_size)
 
         if result == _k4a.K4A_BUFFER_RESULT_TOO_SMALL:
             serial_number = ctypes.create_string_buffer(serial_number_size.value)
 
         _k4a.VERIFY(
-            _k4a.k4a_device_get_serialnum(
-                self._handle, serial_number, serial_number_size
-            ),
+            _k4a.k4a_device_get_serialnum(self._handle, serial_number, serial_number_size),
             "Read serial number failed!",
         )
 
         return serial_number.value.decode("utf-8")
 
     # ctypes.c_int => Configuration에 있는 Enum type
-    def get_calibration(
-        self,
-        depth_mode: ctypes.c_int,
-        color_resolution: ctypes.c_int
-    ) -> Calibration:
+    def get_calibration(self, depth_mode: ctypes.c_int, color_resolution: ctypes.c_int) -> Calibration:
         calibration_handle = _k4a.k4a_calibration_t()
 
         _k4a.VERIFY(
-            _k4a.k4a_device_get_calibration(
-                self._handle, depth_mode, color_resolution, calibration_handle
-            ),
+            _k4a.k4a_device_get_calibration(self._handle, depth_mode, color_resolution, calibration_handle),
             "Get calibration failed!",
         )
 
         return Calibration(calibration_handle)
 
     def get_version(self):
         version = _k4a.k4a_hardware_version_t()
 
-        _k4a.VERIFY(
-            _k4a.k4a_device_get_version(self._handle, version), "Get version failed!"
-        )
+        _k4a.VERIFY(_k4a.k4a_device_get_version(self._handle, version), "Get version failed!")
 
         return version
 
     @staticmethod
     def open(index=0):
         device_handle = _k4a.k4a_device_t()
 
-        _k4a.VERIFY(
-            _k4a.k4a_device_open(index, device_handle), "Open K4A Device failed!"
-        )
+        _k4a.VERIFY(_k4a.k4a_device_open(index, device_handle), "Open K4A Device failed!")
 
         return device_handle
 
     @staticmethod
     def device_get_installed_count():
         return int(_k4a.k4a_device_get_installed_count())
+
+    def get_playback_capture(self, playback_handle):
+        capture_handle = _k4a.k4a_capture_t()
+        ret = k4a_playback_get_next_capture(playback_handle, capture_handle) != K4A_STREAM_RESULT_EOF
+        if ret:
+            return capture_handle
+        else:
+            return None
+
+    def save_frame_for_clip(self, playback_handle, playback_calibration):
+        capture_handle = self.get_playback_capture(playback_handle)
+
+        if self.is_capture_initialized():
+            Device.capture.release_handle()
+            Device.capture._handle = capture_handle
+        else:
+            Device.capture = Capture(capture_handle, playback_calibration)
+
+        if self.recording:
+            self.record.write_capture(Device.capture.handle())
+            
+
+        return Device.capture
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4a/image.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,17 +27,15 @@
             _k4a.k4a_image_release(self._handle)
             self._handle = None
 
     @staticmethod
     def create(image_format, width_pixels, height_pixels, stride_bytes):
         handle = _k4a.k4a_image_t()
         _k4a.VERIFY(
-            _k4a.k4a_image_create(
-                image_format, width_pixels, height_pixels, stride_bytes, handle
-            ),
+            _k4a.k4a_image_create(image_format, width_pixels, height_pixels, stride_bytes, handle),
             "Create image failed!",
         )
 
         return Image(handle)
 
     @property
     def width(self):
@@ -105,46 +103,30 @@
         image_format = self.get_format()
 
         # Read the data in the buffer
         buffer_array = np.ctypeslib.as_array(self.buffer_pointer, shape=(image_size,))
 
         # Parse buffer based on image formats
         if image_format == _k4a.K4A_IMAGE_FORMAT_COLOR_MJPG:
-            return True, cv2.imdecode(
-                np.frombuffer(buffer_array, dtype=np.uint8).copy(), -1
-            )
+            return True, cv2.imdecode(np.frombuffer(buffer_array, dtype=np.uint8).copy(), -1)
         elif image_format == _k4a.K4A_IMAGE_FORMAT_COLOR_NV12:
-            yuv_image = (
-                np.frombuffer(buffer_array, dtype=np.uint8)
-                .copy()
-                .reshape(int(image_height * 1.5), image_width)
-            )
+            yuv_image = np.frombuffer(buffer_array, dtype=np.uint8).copy().reshape(int(image_height * 1.5), image_width)
             return True, cv2.cvtColor(yuv_image, cv2.COLOR_YUV2BGR_NV12)
         elif image_format == _k4a.K4A_IMAGE_FORMAT_COLOR_YUY2:
-            yuv_image = (
-                np.frombuffer(buffer_array, dtype=np.uint8)
-                .copy()
-                .reshape(image_height, image_width, 2)
-            )
+            yuv_image = np.frombuffer(buffer_array, dtype=np.uint8).copy().reshape(image_height, image_width, 2)
             return True, cv2.cvtColor(yuv_image, cv2.COLOR_YUV2BGR_YUY2)
         elif image_format == _k4a.K4A_IMAGE_FORMAT_COLOR_BGRA32:
-            return True, np.frombuffer(buffer_array, dtype=np.uint8).copy().reshape(
-                image_height, image_width, 4
-            )
+            return True, np.frombuffer(buffer_array, dtype=np.uint8).copy().reshape(image_height, image_width, 4)
         elif image_format == _k4a.K4A_IMAGE_FORMAT_DEPTH16:
             return True, np.frombuffer(buffer_array, dtype="<u2").copy().reshape(
                 image_height, image_width
             )  # little-endian 16 bits unsigned Depth data
         elif image_format == _k4a.K4A_IMAGE_FORMAT_IR16:
             return True, np.frombuffer(buffer_array, dtype="<u2").copy().reshape(
                 image_height, image_width
             )  # little-endian 16 bits unsigned IR data. For more details see: https://microsoft.github.io/Azure-Kinect-Sensor-SDK/release/1.2.x/namespace_microsoft_1_1_azure_1_1_kinect_1_1_sensor_a7a3cb7a0a3073650bf17c2fef2bfbd1b.html
         elif image_format == _k4a.K4A_IMAGE_FORMAT_CUSTOM8:
-            return True, np.frombuffer(buffer_array, dtype="<u1").copy().reshape(
-                image_height, image_width
-            )
+            return True, np.frombuffer(buffer_array, dtype="<u1").copy().reshape(image_height, image_width)
         elif image_format == _k4a.K4A_IMAGE_FORMAT_CUSTOM16:
-            return True, np.frombuffer(buffer_array, dtype="<u2").copy().reshape(
-                image_height, image_width
-            )
+            return True, np.frombuffer(buffer_array, dtype="<u2").copy().reshape(image_height, image_width)
         elif image_format == _k4a.K4A_IMAGE_FORMAT_CUSTOM:
             return True, np.frombuffer(buffer_array, dtype="<i2").copy()
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4a/imu_sample.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/imu_sample.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..utils import getdict
+from ..utils import get_dict
 
 
 class ImuSample:
     def __init__(self, imu_sample_struct):
         self._struct = imu_sample_struct
         self.parse_data()
 
@@ -16,15 +16,15 @@
         return self._struct
 
     def reset(self):
         if self.is_valid():
             self._struct = None
 
     def parse_data(self):
-        self.imu_sample_dict = getdict(self._struct)
+        self.imu_sample_dict = get_dict(self._struct)
 
         # Convert the acc and gyro dicts to numpy array
         self.imu_sample_dict["acc_sample"] = self.imu_sample_dict["acc_sample"]["v"]
         self.imu_sample_dict["gyro_sample"] = self.imu_sample_dict["gyro_sample"]["v"]
 
     @property
     def temp(self):
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4a/transformation.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/transformation.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,17 +101,15 @@
             depth_image.handle(),
             color_image.handle(),
             transformed_color_image.handle(),
         )
 
         return transformed_color_image
 
-    def depth_image_to_point_cloud(
-        self, depth_image, calibration_type=_k4a.K4A_CALIBRATION_TYPE_DEPTH
-    ):
+    def depth_image_to_point_cloud(self, depth_image, calibration_type=_k4a.K4A_CALIBRATION_TYPE_DEPTH):
         if not depth_image.is_valid():
             return Image()
 
         xyz_image = Image.create(
             _k4a.K4A_IMAGE_FORMAT_CUSTOM,
             depth_image.get_width_pixels(),
             depth_image.get_height_pixels(),
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4abt/body.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/body.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4abt/body2d.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/body2d.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,17 +53,15 @@
         )
 
         for segmentId in range(len(K4ABT_SEGMENT_PAIRS)):
             segment_pair = K4ABT_SEGMENT_PAIRS[segmentId]
             point1 = self.joints[segment_pair[0]].get_coordinates()
             point2 = self.joints[segment_pair[1]].get_coordinates()
 
-            if (point1[0] == 0 and point1[1] == 0) or (
-                point2[0] == 0 and point2[1] == 0
-            ):
+            if (point1[0] == 0 and point1[1] == 0) or (point2[0] == 0 and point2[1] == 0):
                 continue
             image = cv2.line(image, point1, point2, color, 2)
 
         if only_segments:
             return image
 
         for joint in self.joints:
@@ -76,17 +74,15 @@
         skeleton2d_handle = k4abt_skeleton2D_t()
         body2d_handle = k4abt_body2D_t()
 
         for jointID, joint in enumerate(body_handle.skeleton.joints):
             skeleton2d_handle.joints2D[jointID].position = calibration.convert_3d_to_2d(
                 joint.position, K4A_CALIBRATION_TYPE_DEPTH, dest_camera
             )
-            skeleton2d_handle.joints2D[
-                jointID
-            ].confidence_level = joint.confidence_level
+            skeleton2d_handle.joints2D[jointID].confidence_level = joint.confidence_level
 
         body2d_handle.skeleton = skeleton2d_handle
         body2d_handle.id = bodyIdx
 
         return Body2d(body2d_handle)
 
     def __str__(self):
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4abt/frame.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,59 +89,47 @@
         destination_image,
         dest_camera=K4A_CALIBRATION_TYPE_DEPTH,
         only_segments=False,
     ):
         num_bodies = self.get_num_bodies()
 
         for body_id in range(num_bodies):
-            destination_image = self.draw_body2d(
-                destination_image, body_id, dest_camera, only_segments
-            )
+            destination_image = self.draw_body2d(destination_image, body_id, dest_camera, only_segments)
 
         return destination_image
 
     def draw_body2d(
         self,
         destination_image,
         bodyIdx=0,
         dest_camera=K4A_CALIBRATION_TYPE_DEPTH,
         only_segments=False,
     ):
-        return self.get_body2d(bodyIdx, dest_camera).draw(
-            destination_image, only_segments
-        )
+        return self.get_body2d(bodyIdx, dest_camera).draw(destination_image, only_segments)
 
     def get_device_timestamp_usec(self):
         return _k4abt.k4abt_frame_get_device_timestamp_usec(self._handle)
 
     def get_body_index_map(self):
         return Image(_k4abt.k4abt_frame_get_body_index_map(self._handle))
 
     def get_body_index_map_image(self):
         return self.get_body_index_map().to_numpy()
 
     def get_transformed_body_index_map(self):
         depth_image = self.get_capture().get_depth_image_object()
-        return self.transformation.depth_image_to_color_camera_custom(
-            depth_image, self.get_body_index_map()
-        )
+        return self.transformation.depth_image_to_color_camera_custom(depth_image, self.get_body_index_map())
 
     def get_transformed_body_index_map_image(self):
         transformed_body_index_map = self.get_transformed_body_index_map()
         return transformed_body_index_map.to_numpy()
 
     def get_segmentation_image(self):
         ret, body_index_map = self.get_body_index_map_image()
-        return ret, np.dstack(
-            [cv2.LUT(body_index_map, body_colors[:, i]) for i in range(3)]
-        )
+        return ret, np.dstack([cv2.LUT(body_index_map, body_colors[:, i]) for i in range(3)])
 
     def get_transformed_segmentation_image(self):
         ret, transformed_body_index_map = self.get_transformed_body_index_map_image()
-        return ret, np.dstack(
-            [cv2.LUT(transformed_body_index_map, body_colors[:, i]) for i in range(3)]
-        )
+        return ret, np.dstack([cv2.LUT(transformed_body_index_map, body_colors[:, i]) for i in range(3)])
 
     def get_capture(self):
-        return Capture(
-            _k4abt.k4abt_frame_get_capture(self._handle), self.calibration._handle
-        )
+        return Capture(_k4abt.k4abt_frame_get_capture(self._handle), self.calibration._handle)
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4abt/joint.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/joint.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4abt/joint2d.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/joint2d.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4abt/tracker.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/tracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,35 +36,29 @@
         else:
             self.enqueue_capture(Device.capture.handle(), timeout_in_ms)
 
         return self.pop_result(timeout_in_ms)
 
     def enqueue_capture(self, capture_handle, timeout_in_ms=K4A_WAIT_INFINITE):
         _k4abt.VERIFY(
-            _k4abt.k4abt_tracker_enqueue_capture(
-                self._handle, capture_handle, timeout_in_ms
-            ),
+            _k4abt.k4abt_tracker_enqueue_capture(self._handle, capture_handle, timeout_in_ms),
             "Body tracker capture enqueue failed!",
         )
 
     def pop_result(self, timeout_in_ms=K4A_WAIT_INFINITE):
         if self.is_frame_initialized():
             self.frame.release()
             _k4abt.VERIFY(
-                _k4abt.k4abt_tracker_pop_result(
-                    self._handle, self.frame.handle(), timeout_in_ms
-                ),
+                _k4abt.k4abt_tracker_pop_result(self._handle, self.frame.handle(), timeout_in_ms),
                 "Body tracker get body frame failed!",
             )
         else:
             frame_handle = _k4abt.k4abt_frame_t()
             _k4abt.VERIFY(
-                _k4abt.k4abt_tracker_pop_result(
-                    self._handle, frame_handle, timeout_in_ms
-                ),
+                _k4abt.k4abt_tracker_pop_result(self._handle, frame_handle, timeout_in_ms),
                 "Body tracker get body frame failed!",
             )
             self.frame = Frame(frame_handle, self.calibration)
 
         return self.frame
 
     def set_temporal_smoothing(self, smoothing_factor):
@@ -74,17 +68,15 @@
         _k4abt.k4abt_tracker_shutdown(self._handle)
 
     def create(self, model_type):
         tracker_config = self.get_tracker_configuration(model_type)
 
         tracker_handle = _k4abt.k4abt_tracker_t()
         _k4abt.VERIFY(
-            _k4abt.k4abt_tracker_create(
-                self.calibration.handle(), tracker_config, tracker_handle
-            ),
+            _k4abt.k4abt_tracker_create(self.calibration.handle(), tracker_config, tracker_handle),
             "Body tracker initialization failed!",
         )
 
         return tracker_handle
 
     def get_tracker_configuration(self, model_type):
         tracker_config = k4abt_tracker_default_configuration
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4arecord/_k4arecord.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/_k4arecord.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import ctypes
 import sys
 import traceback
 
 from ._k4arecordTypes import *
 from ..k4a._k4atypes import *
+from ..k4a import _k4atypes
 
 record_dll = None
 
 
 def setup_library(module_k4arecord_path):
     global record_dll
 
@@ -44,14 +45,22 @@
     _k4a_record_write_header = record_dll.k4a_record_write_header
     _k4a_record_write_header.restype = k4a_result_t
     _k4a_record_write_header.argtypes = (k4a_record_t,)
 
     return _k4a_record_write_header(recording_handle)
 
 
+def k4a_record_write_imu_sample(recording_handle, imu_sample):
+    _k4a_record_write_imu_sample = record_dll.k4a_record_write_imu_sample
+    _k4a_record_write_imu_sample.restype = k4a_result_t
+    _k4a_record_write_imu_sample.argtypes = (k4a_record_t, k4a_imu_sample_t)
+
+    return _k4a_record_write_imu_sample(recording_handle, imu_sample)
+
+
 def k4a_record_write_capture(recording_handle, capture_handle):
     # K4ARECORD_EXPORT k4a_result_t k4a_record_write_capture(k4a_record_t recording_handle, k4a_capture_t capture_handle);
     _k4a_record_write_capture = record_dll.k4a_record_write_capture
     _k4a_record_write_capture.restype = k4a_result_t
     _k4a_record_write_capture.argtypes = (k4a_record_t, k4a_capture_t)
 
     return _k4a_record_write_capture(recording_handle, capture_handle)
@@ -71,14 +80,22 @@
     _k4a_record_close = record_dll.k4a_record_close
     _k4a_record_close.restype = None
     _k4a_record_close.argtypes = (k4a_record_t,)
 
     _k4a_record_close(recording_handle)
 
 
+def k4a_record_add_imu_track(recording_handle):
+    _k4a_record_add_imu_track = record_dll.k4a_record_add_imu_track
+    _k4a_record_add_imu_track.restype = k4a_result_t
+    _k4a_record_add_imu_track.argtypes = (k4a_record_t,)
+
+    return _k4a_record_add_imu_track(recording_handle)
+
+
 ###########################
 ###    Playback         ###
 ###########################
 
 
 def k4a_playback_open(file_path, playback_handle):
     # K4ARECORD_EXPORT k4a_result_t k4a_playback_open(const char *path, k4a_playback_t *playback_handle);
@@ -96,14 +113,15 @@
     # K4ARECORD_EXPORT void k4a_playback_close(k4a_playback_t playback_handle);
     _k4a_playback_close = record_dll.k4a_playback_close
     _k4a_playback_close.restype = None
     _k4a_playback_close.argtypes = (k4a_playback_t,)
 
     _k4a_playback_close(playback_handle)
 
+
 # get vs get raw?
 def k4a_playback_get_raw_calibration(playback_handle, data, data_size):
     """
     K4ARECORD_EXPORT k4a_buffer_result_t k4a_playback_get_raw_calibration(
         k4a_playback_t playback_handle,
         uint8_t *data,
         size_t *data_size
@@ -140,30 +158,29 @@
 def k4a_playback_get_record_configuration(playback_handle, config):
     """
     K4ARECORD_EXPORT k4a_result_t k4a_playback_get_record_configuration(
         k4a_playback_t playback_handle,
         k4a_record_configuration_t *config
     );
     """
-    _k4a_playback_get_record_configuration = (
-        record_dll.k4a_playback_get_record_configuration
-    )
+    _k4a_playback_get_record_configuration = record_dll.k4a_playback_get_record_configuration
     _k4a_playback_get_record_configuration.restype = k4a_result_t
     _k4a_playback_get_record_configuration.argtypes = (
         k4a_playback_t,
         ctypes.POINTER(k4a_record_configuration_t),
     )
 
     return _k4a_playback_get_record_configuration(playback_handle, config)
 
+
 # Check for files with the same name
 def k4a_playback_check_track_exists(playback_handle, track_name):
     """
     K4ARECORD_EXPORT bool k4a_playback_check_track_exists(
-        k4a_playback_t playback_handle, 
+        k4a_playback_t playback_handle,
         const char *track_name
     );
     """
     _k4a_playback_check_track_exists = record_dll.k4a_playback_check_track_exists
     _k4a_playback_check_track_exists.restype = ctypes.c_bool
     _k4a_playback_check_track_exists.argtypes = (
         k4a_playback_t,
@@ -180,18 +197,16 @@
     _k4a_playback_get_track_count = record_dll.k4a_playback_get_track_count
     _k4a_playback_get_track_count.restype = ctypes.c_size_t
     _k4a_playback_get_track_count.argtypes = (k4a_playback_t,)
 
     return _k4a_playback_get_track_count(playback_handle)
 
 
-#extract video with filename 
-def k4a_playback_get_track_name(
-    playback_handle, track_index, track_name, track_name_size
-):
+# extract video with filename
+def k4a_playback_get_track_name(playback_handle, track_index, track_name, track_name_size):
     """
     K4ARECORD_EXPORT k4a_buffer_result_t k4a_playback_get_track_name(
         k4a_playback_t playback_handle,
         size_t track_index,
         char *track_name,
         size_t *track_name_size
     );
@@ -201,25 +216,21 @@
     _k4a_playback_get_track_name.argtypes = (
         k4a_playback_t,
         ctypes.c_size_t,
         ctypes.POINTER(ctypes.c_char),
         ctypes.POINTER(ctypes.c_size_t),
     )
 
-    return _k4a_playback_get_track_name(
-        playback_handle, track_index, track_name, track_name_size
-    )
+    return _k4a_playback_get_track_name(playback_handle, track_index, track_name, track_name_size)
 
 
-def k4a_playbk4a_playback_track_is_builtinack_get_track_name(
-    playback_handle, track_name
-):
+def k4a_playbk4a_playback_track_is_builtinack_get_track_name(playback_handle, track_name):
     """
     K4ARECORD_EXPORT bool k4a_playback_track_is_builtin(
-        k4a_playback_t playback_handle, 
+        k4a_playback_t playback_handle,
         const char *track_name
     );
     """
     _k4a_playback_track_is_builtin = record_dll.k4a_playback_track_is_builtin
     _k4a_playback_track_is_builtin.restype = ctypes.c_bool
     _k4a_playback_track_is_builtin.argtypes = (
         k4a_playback_t,
@@ -233,32 +244,26 @@
     """
     K4ARECORD_EXPORT k4a_result_t k4a_playback_track_get_video_settings(
         k4a_playback_t playback_handle,
         const char *track_name,
         k4a_record_video_settings_t *video_settings
     );
     """
-    _k4a_playback_track_get_video_settings = (
-        record_dll.k4a_playback_track_get_video_settings
-    )
+    _k4a_playback_track_get_video_settings = record_dll.k4a_playback_track_get_video_settings
     _k4a_playback_track_get_video_settings.restype = k4a_result_t
     _k4a_playback_track_get_video_settings.argtypes = (
         k4a_playback_t,
         ctypes.POINTER(ctypes.c_char),
         ctypes.POINTER(k4a_record_video_settings_t),
     )
 
-    return _k4a_playback_track_get_video_settings(
-        playback_handle, track_name, video_settings
-    )
+    return _k4a_playback_track_get_video_settings(playback_handle, track_name, video_settings)
 
 
-def k4a_playback_track_get_codec_id(
-    playback_handle, track_name, codec_id, codec_id_size
-):
+def k4a_playback_track_get_codec_id(playback_handle, track_name, codec_id, codec_id_size):
     """
     K4ARECORD_EXPORT k4a_buffer_result_t k4a_playback_track_get_codec_id(
         k4a_playback_t playback_handle,
         const char *track_name,
         char *codec_id,
         size_t *codec_id_size
     );
@@ -268,44 +273,36 @@
     _k4a_playback_track_get_codec_id.argtypes = (
         k4a_playback_t,
         ctypes.POINTER(ctypes.c_char),
         ctypes.POINTER(ctypes.c_char),
         ctypes.POINTER(ctypes.c_size_t),
     )
 
-    return _k4a_playback_track_get_codec_id(
-        playback_handle, track_name, codec_id, codec_id_size
-    )
+    return _k4a_playback_track_get_codec_id(playback_handle, track_name, codec_id, codec_id_size)
 
 
-def k4a_playback_track_get_codec_context(
-    playback_handle, track_name, codec_context, codec_context_size
-):
+def k4a_playback_track_get_codec_context(playback_handle, track_name, codec_context, codec_context_size):
     """
     K4ARECORD_EXPORT k4a_buffer_result_t k4a_playback_track_get_codec_context(
         k4a_playback_t playback_handle,
         const char *track_name,
         uint8_t *codec_context,
         size_t *codec_context_size
     );
     """
-    _k4a_playback_track_get_codec_context = (
-        record_dll.k4a_playback_track_get_codec_context
-    )
+    _k4a_playback_track_get_codec_context = record_dll.k4a_playback_track_get_codec_context
     _k4a_playback_track_get_codec_context.restype = k4a_buffer_result_t
     _k4a_playback_track_get_codec_context.argtypes = (
         k4a_playback_t,
         ctypes.POINTER(ctypes.c_char),
         ctypes.POINTER(ctypes.c_uint8),
         ctypes.POINTER(ctypes.c_size_t),
     )
 
-    return _k4a_playback_track_get_codec_context(
-        playback_handle, track_name, codec_context, codec_context_size
-    )
+    return _k4a_playback_track_get_codec_context(playback_handle, track_name, codec_context, codec_context_size)
 
 
 def k4a_playback_get_tag(playback_handle, name, value, value_size):
     """
     K4ARECORD_EXPORT k4a_buffer_result_t k4a_playback_get_tag(
         k4a_playback_t playback_handle,
         const char *name,
@@ -321,15 +318,15 @@
         ctypes.POINTER(ctypes.c_char),
         ctypes.POINTER(ctypes.c_size_t),
     )
 
     return _k4a_playback_get_tag(playback_handle, name, value, value_size)
 
 
-# convert 
+# convert
 def k4a_playback_set_color_conversion(playback_handle, target_format):
     """
     K4ARECORD_EXPORT k4a_result_t k4a_playback_set_color_conversion(
         k4a_playback_t playback_handle,
         k4a_image_format_t target_format
     );
     """
@@ -415,17 +412,15 @@
 def k4a_playback_get_previous_imu_sample(playback_handle, imu_sample):
     """
     K4ARECORD_EXPORT k4a_stream_result_t k4a_playback_get_previous_imu_sample(
         k4a_playback_t playback_handle,
         k4a_imu_sample_t *imu_sample
     );
     """
-    _k4a_playback_get_previous_imu_sample = (
-        record_dll.k4a_playback_get_previous_imu_sample
-    )
+    _k4a_playback_get_previous_imu_sample = record_dll.k4a_playback_get_previous_imu_sample
     _k4a_playback_get_previous_imu_sample.restype = k4a_stream_result_t
     _k4a_playback_get_previous_imu_sample.argtypes = (
         k4a_playback_t,
         ctypes.POINTER(k4a_imu_sample_t),
     )
 
     return _k4a_playback_get_previous_imu_sample(playback_handle, imu_sample)
@@ -443,72 +438,58 @@
     _k4a_playback_get_next_data_block.restype = k4a_stream_result_t
     _k4a_playback_get_next_data_block.argtypes = (
         k4a_playback_t,
         ctypes.POINTER(ctypes.c_char),
         ctypes.POINTER(k4a_playback_data_block_t),
     )
 
-    return _k4a_playback_get_next_data_block(
-        playback_handle, track_name, data_block_handle
-    )
+    return _k4a_playback_get_next_data_block(playback_handle, track_name, data_block_handle)
 
 
-def k4a_playback_get_previous_data_block(
-    playback_handle, track_name, data_block_handle
-):
+def k4a_playback_get_previous_data_block(playback_handle, track_name, data_block_handle):
     """
     K4ARECORD_EXPORT k4a_stream_result_t k4a_playback_get_previous_data_block(
         k4a_playback_t playback_handle,
         const char *track_name,
         k4a_playback_data_block_t *data_block_handle
     );
     """
-    _k4a_playback_get_previous_data_block = (
-        record_dll.k4a_playback_get_previous_data_block
-    )
+    _k4a_playback_get_previous_data_block = record_dll.k4a_playback_get_previous_data_block
     _k4a_playback_get_previous_data_block.restype = k4a_stream_result_t
     _k4a_playback_get_previous_data_block.argtypes = (
         k4a_playback_t,
         ctypes.POINTER(ctypes.c_char),
         ctypes.POINTER(k4a_playback_data_block_t),
     )
 
-    return _k4a_playback_get_previous_data_block(
-        playback_handle, track_name, data_block_handle
-    )
+    return _k4a_playback_get_previous_data_block(playback_handle, track_name, data_block_handle)
 
 
 # Gets the last timestamp in a recording, relative to the start of the recording.
 def k4a_playback_data_block_get_device_timestamp_usec(data_block_handle):
     """
     K4ARECORD_EXPORT uint64_t k4a_playback_data_block_get_device_timestamp_usec(
         k4a_playback_data_block_t data_block_handle
     );
     """
-    _k4a_playback_data_block_get_device_timestamp_usec = (
-        record_dll.k4a_playback_data_block_get_device_timestamp_usec
-    )
+    _k4a_playback_data_block_get_device_timestamp_usec = record_dll.k4a_playback_data_block_get_device_timestamp_usec
     _k4a_playback_data_block_get_device_timestamp_usec.restype = ctypes.c_uint64
-    _k4a_playback_data_block_get_device_timestamp_usec.argtypes = (
-        k4a_playback_data_block_t,
-    )
+    _k4a_playback_data_block_get_device_timestamp_usec.argtypes = (k4a_playback_data_block_t,)
 
     return _k4a_playback_data_block_get_device_timestamp_usec(data_block_handle)
 
 
-# 
+#
 def k4a_playback_data_block_get_buffer_size(data_block_handle):
     """
     K4ARECORD_EXPORT size_t k4a_playback_data_block_get_buffer_size(
         k4a_playback_data_block_t data_block_handle
     );
     """
-    _k4a_playback_data_block_get_buffer_size = (
-        record_dll.k4a_playback_data_block_get_buffer_size
-    )
+    _k4a_playback_data_block_get_buffer_size = record_dll.k4a_playback_data_block_get_buffer_size
     _k4a_playback_data_block_get_buffer_size.restype = ctypes.c_size_t
     _k4a_playback_data_block_get_buffer_size.argtypes = (k4a_playback_data_block_t,)
 
     return _k4a_playback_data_block_get_buffer_size(data_block_handle)
 
 
 def k4a_playback_data_block_get_buffer(data_block_handle):
@@ -558,32 +539,28 @@
 
 def k4a_playback_get_recording_length_usec(playback_handle):
     """
     K4ARECORD_EXPORT uint64_t k4a_playback_get_recording_length_usec(
         k4a_playback_t playback_handle
     );
     """
-    _k4a_playback_get_recording_length_usec = (
-        record_dll.k4a_playback_get_recording_length_usec
-    )
+    _k4a_playback_get_recording_length_usec = record_dll.k4a_playback_get_recording_length_usec
     _k4a_playback_get_recording_length_usec.restype = ctypes.c_uint64
     _k4a_playback_get_recording_length_usec.argtypes = (k4a_playback_t,)
 
     return _k4a_playback_get_recording_length_usec(playback_handle)
 
 
 def k4a_playback_get_last_timestamp_usec(playback_handle):
     """
     K4ARECORD_DEPRECATED_EXPORT uint64_t k4a_playback_get_last_timestamp_usec(
         k4a_playback_t playback_handle
     );
     """
-    _k4a_playback_get_last_timestamp_usec = (
-        record_dll.k4a_playback_get_last_timestamp_usec
-    )
+    _k4a_playback_get_last_timestamp_usec = record_dll.k4a_playback_get_last_timestamp_usec
     _k4a_playback_get_last_timestamp_usec.restype = ctypes.c_uint64
     _k4a_playback_get_last_timestamp_usec.argtypes = (k4a_playback_t,)
 
     return _k4a_playback_get_last_timestamp_usec(playback_handle)
 
 
 def VERIFY(result, error):
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4arecord/_k4arecordTypes.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/_k4arecordTypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,34 +3,37 @@
 
 # K4A_DECLARE_HANDLE(k4a_record_t);
 class _handle_k4a_record_t(ctypes.Structure):
     _fields_ = [
         ("_rsvd", ctypes.c_size_t),
     ]
 
-# streaming frame record 
+
+# streaming frame record
 k4a_record_t = ctypes.POINTER(_handle_k4a_record_t)
 
 
 # K4A_DECLARE_HANDLE(k4a_playback_t);
 class _handle_k4a_playback_t(ctypes.Structure):
     _fields_ = [
         ("_rsvd", ctypes.c_size_t),
     ]
 
+
 # watching video which recorded by k4a_record
 k4a_playback_t = ctypes.POINTER(_handle_k4a_playback_t)
 
 
 # K4A_DECLARE_HANDLE(k4a_playback_data_block_t);
 class _handle_k4a_playback_data_block_t(ctypes.Structure):
     _fields_ = [
         ("_rsvd", ctypes.c_size_t),
     ]
 
+
 # Handle to a block of data read from k4a_playback
 k4a_playback_data_block_t = ctypes.POINTER(_handle_k4a_playback_data_block_t)
 
 
 # class k4a_stream_result_t(CtypeIntEnum):
 k4a_stream_result_t = ctypes.c_int
 K4A_STREAM_RESULT_SUCCEEDED = 0
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4arecord/datablock.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/datablock.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 
     def reset(self):
         if self.is_valid():
             _k4arecord.k4a_playback_data_block_release(self._handle)
             self._handle = None
 
     def get_device_timestamp_usec(self):
-        return int(
-            _k4arecord.k4a_playback_data_block_get_device_timestamp_usec(self._handle)
-        )
+        return int(_k4arecord.k4a_playback_data_block_get_device_timestamp_usec(self._handle))
 
     def get_buffer_size(self):
         return int(_k4arecord.k4a_playback_data_block_get_buffer_size(self._handle))
 
     def get_buffer(self):
         if not self.is_valid():
             return None
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4arecord/playback.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/playback.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from . import _k4arecord
 from .datablock import Datablock
 from .record_configuration import RecordConfiguration
 from ..k4a import _k4a
 from ..k4a.capture import Capture
 from ..k4a.calibration import Calibration
 from ..k4a.imu_sample import ImuSample
+from .record import Record
+from ..k4a.configuration import Configuration
 
 
 class Playback:
     def __init__(self, filepath):
         self._handle = _k4arecord.k4a_playback_t()
         self._capture = None
         self._datablock = None
+        self.clipping = None
 
         self.open(filepath)
         self.calibration = self.get_calibration()
 
     def __del__(self):
         self.close()
 
     def open(self, filepath):
         _k4arecord.VERIFY(
             _k4arecord.k4a_playback_open(filepath.encode("utf-8"), self._handle),
             "Failed to open recording!",
         )
 
     def update(self):
-        return self.get_next_capture()
+        return self.get_next_capture() if self.clipping is None else self.get_next_capture_with_record()
 
     def is_valid(self):
         return self._handle != None
 
     def is_capture_initialized(self):
         return self._capture
 
@@ -42,17 +45,15 @@
             _k4arecord.k4a_playback_close(self._handle)
             self._handle = None
 
     def get_calibration(self):
         calibration_handle = _k4arecord.k4a_calibration_t()
         if self.is_valid():
             _k4arecord.VERIFY(
-                _k4arecord.k4a_playback_get_calibration(
-                    self._handle, calibration_handle
-                ),
+                _k4arecord.k4a_playback_get_calibration(self._handle, calibration_handle),
                 "Failed to read device calibration from recording!",
             )
 
         return Calibration(calibration_handle)
 
     def get_record_configuration(self):
         config = _k4arecord.k4a_record_configuration_t()
@@ -70,18 +71,29 @@
 
         if self.is_capture_initialized():
             self._capture.release_handle()
             self._capture._handle = capture_handle
         else:
             self._capture = Capture(capture_handle, self.calibration)
 
-        ret = (
-            _k4arecord.k4a_playback_get_next_capture(self._handle, capture_handle)
-            != _k4arecord.K4A_STREAM_RESULT_EOF
-        )
+        ret = _k4arecord.k4a_playback_get_next_capture(self._handle, capture_handle) != _k4arecord.K4A_STREAM_RESULT_EOF
+
+        return ret, self._capture
+
+    def get_next_capture_with_record(self):
+        if self.is_capture_initialized():
+            self._capture.release_handle()
+
+        capture_handle = _k4a.k4a_capture_t()
+        ret = _k4arecord.k4a_playback_get_next_capture(self._handle, capture_handle) != _k4arecord.K4A_STREAM_RESULT_EOF
+
+        if self.is_capture_initialized():
+            self._capture._handle = capture_handle
+        else:
+            self._capture = Capture(capture_handle, self.calibration)
 
         return ret, self._capture
 
     def get_previous_capture(self):
         capture_handle = _k4a.k4a_capture_t()
 
         if self.is_capture_initialized():
@@ -96,31 +108,27 @@
         )
 
         return ret, self._capture
 
     def get_next_imu_sample(self):
         imu_sample_struct = _k4a.k4a_imu_sample_t()
         _k4a.VERIFY(
-            _k4arecord.k4a_playback_get_next_imu_sample(
-                self._handle, imu_sample_struct
-            ),
+            _k4arecord.k4a_playback_get_next_imu_sample(self._handle, imu_sample_struct),
             "Get next imu sample failed!",
         )
 
         # Convert the structure into a dictionary
         _imu_sample = ImuSample(imu_sample_struct)
 
         return _imu_sample
 
     def get_previous_imu_sample(self):
         imu_sample_struct = _k4a.k4a_imu_sample_t()
         _k4a.VERIFY(
-            _k4arecord.k4a_playback_get_previous_imu_sample(
-                self._handle, imu_sample_struct
-            ),
+            _k4arecord.k4a_playback_get_previous_imu_sample(self._handle, imu_sample_struct),
             "Get previous imu sample failed!",
         )
 
         # Convert the structure into a dictionary
         _imu_sample = ImuSample(imu_sample_struct)
 
         return _imu_sample
@@ -139,33 +147,29 @@
             _k4arecord.k4a_playback_set_color_conversion(self._handle, format),
             "Seek color conversio failed!",
         )
 
     def get_next_data_block(self, track):
         block_handle = _k4arecord.k4a_playback_data_block_t()
         _k4a.VERIFY(
-            _k4arecord.k4a_playback_get_next_data_block(
-                self._handle, track, block_handle
-            ),
+            _k4arecord.k4a_playback_get_next_data_block(self._handle, track, block_handle),
             "Get next data block failed!",
         )
 
         if self.is_datablock_initialized():
             self._datablock._handle = block_handle
         else:
             self._datablock = Datablock(block_handle)
 
         return self._datablock
 
     def get_previous_data_block(self, track):
         block_handle = _k4arecord.k4a_playback_data_block_t()
         _k4a.VERIFY(
-            _k4arecord.k4a_playback_get_previous_data_block(
-                self._handle, track, block_handle
-            ),
+            _k4arecord.k4a_playback_get_previous_data_block(self._handle, track, block_handle),
             "Get previous data block failed!",
         )
 
         if self.is_datablock_initialized():
             self._datablock._handle = block_handle
         else:
             self._datablock = Datablock(block_handle)
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4arecord/record.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/record.py`

 * *Files 27% similar despite different names*

```diff
@@ -26,34 +26,42 @@
     def is_valid(self):
         return self.record_handle != None
 
     def close(self):
         if self.is_valid():
             _k4arecord.k4a_record_close(self.record_handle)
             self.record_handle = None
-        else:
-            print("sibal")
 
     def flush(self):
         if self.is_valid():
-            _k4arecord.VERIFY(
-                _k4arecord.k4a_record_flush(self.record_handle), "Failed to flush!"
-            )
+            _k4arecord.VERIFY(_k4arecord.k4a_record_flush(self.record_handle), "Failed to flush!")
 
     def write_header(self):
         if self.is_valid():
             _k4arecord.VERIFY(
                 _k4arecord.k4a_record_write_header(self.record_handle),
                 "Failed to write header!",
             )
 
+    def write_imu(self, imu_sample):
+        if self.is_valid():
+            _k4arecord.VERIFY(
+                _k4arecord.k4a_record_write_imu_sample(self.record_handle, imu_sample),
+                "Failed to write imu!",
+            )
+
     def write_capture(self, capture_handle):
         if not self.is_valid():
             raise NameError("Recording not found")
-
         if not self.header_written:
             self.write_header()
             self.header_written = True
         _k4arecord.VERIFY(
             _k4arecord.k4a_record_write_capture(self.record_handle, capture_handle),
             "Failed to write capture!",
         )
+
+    def add_imu_track(self):
+        _k4arecord.VERIFY(
+            _k4arecord.k4a_record_add_imu_track(self.record_handle),
+            "Failed to add imu track!",
+        )
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/k4arecord/record_configuration.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/record_configuration.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/_pyk4a/pykinect.py` & `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/pykinect.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 from .utils import (
     get_k4a_module_path,
     get_k4abt_module_path,
     get_k4arecord_module_path,
 )
 
 
-def initialize_libraries(
-    module_k4a_path=None, module_k4abt_path=None, track_body=False
-) -> bool:
+def initialize_libraries(module_k4a_path=None, module_k4abt_path=None, track_body=False) -> bool:
     # Search the module path for k4a if not available
     if module_k4a_path is None:
         module_k4a_path = get_k4a_module_path()
 
     module_k4arecord_path = get_k4arecord_module_path(module_k4a_path)
     _flag = True
     try:
@@ -32,15 +30,15 @@
         #         module_k4abt_path = get_k4abt_module_path()
 
         #     # Initialize k4abt related wrappers
         #     init_k4abt(module_k4abt_path)
     except:
         print("Can not setting .dll")
         _flag = False
-    
+
     finally:
         return _flag
 
 
 def init_k4a(module_k4a_path):
     _k4a.setup_library(module_k4a_path)
 
@@ -60,17 +58,16 @@
     record_filepath="output.mkv",
 ):
     # Create device object
     device = Device(device_index)
 
     # Start device
     device.start(config, record, record_filepath)
-    
-    return device
 
+    return device
 
 # def start_body_tracker(model_type=_k4abt.K4ABT_DEFAULT_MODEL, calibration=None):
 #     if calibration:
 #         return Tracker(calibration, model_type)
 #     else:
 #         return Tracker(Device.calibration, model_type)
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/cli/command.py` & `pykinect_recorder-0.9.2/pykinect_recorder/cli/command.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import click
 from pykinect_recorder.renderer import MainWindow
 import qdarktheme
 from PySide6.QtWidgets import QApplication
- 
 
-CONTEXT_SETTINGS = dict(help_option_names=['-h','--help'])
+
+CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 @click.group(context_settings=CONTEXT_SETTINGS)
 def cli():
     pass
 
 
 # @click.command(help="pykinect")
 # @click.option("--open", is_flag=True)
 # def check(open):
 #     if open:
-#         print('sibal')
 #         # run()
 
 
 def main():
     app = QApplication()
     qdarktheme.setup_theme()
     main_window = MainWindow()
     main_window.show()
     app.exec()
 
 
-if __name__ == '__main__':
-    main()
+if __name__ == "__main__":
+    main()
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/logger.py` & `pykinect_recorder-0.9.2/pykinect_recorder/renderer/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import logging
 
 import termcolor
 
-from . import __appname__
+from ..pyk4a import __appname__
 
 COLORS = {
     "WARNING": "yellow",
     "INFO": "white",
     "DEBUG": "blue",
     "CRITICAL": "red",
     "ERROR": "red",
@@ -39,26 +39,23 @@
             record.module2 = termcolor.colored(record.module, color="cyan")
             record.funcName2 = termcolor.colored(record.funcName, color="cyan")
             record.lineno2 = termcolor.colored(record.lineno, color="cyan")
         return logging.Formatter.format(self, record)
 
 
 class ColoredLogger(logging.Logger):
-
-    FORMAT = (
-        "[%(levelname2)s] %(module2)s:%(funcName2)s:%(lineno2)s - %(message2)s"
-    )
+    FORMAT = "[%(levelname2)s] %(module2)s:%(funcName2)s:%(lineno2)s - %(message2)s"
 
     def __init__(self, name):
         logging.Logger.__init__(self, name, logging.INFO)
 
         color_formatter = ColoredFormatter(self.FORMAT)
 
         console = logging.StreamHandler()
         console.setFormatter(color_formatter)
 
         self.addHandler(console)
         return
 
 
 logger = logging.getLogger(__appname__)
-logger.__class__ = ColoredLogger
+logger.__class__ = ColoredLogger
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/record_audio.py` & `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/sidebar_explorer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,207 +1,165 @@
-import argparse
-import datetime
-import os
-import queue
-import sys
-import tempfile
-
-import numpy  # Make sure NumPy is loaded before it is used in the callback
-
-import sounddevice as sd
-import soundfile as sf
-
-assert numpy  # avoid "imported but unused" message (W0611)
-
 import os
-import sys
-import time
-from argparse import ArgumentParser
-
 import cv2
-import numpy as np
-import pyk4a
-from pydub import AudioSegment
-from pyk4a import Config, ImageFormat, PyK4A, PyK4ARecord
-from PySide6.QtCore import Qt, QThread, Signal, Slot
-from PySide6.QtGui import QAction, QImage, QKeySequence, QPixmap
+import datetime
+from pathlib import Path
+
+import qtawesome as qta
+from PySide6.QtGui import QImage, QPixmap
+from PySide6.QtCore import Qt, Signal, Slot, QSize
 from PySide6.QtWidgets import (
-    QApplication,
-    QComboBox,
-    QGroupBox,
-    QHBoxLayout,
-    QLabel,
-    QMainWindow,
-    QPushButton,
-    QSizePolicy,
-    QVBoxLayout,
-    QWidget,
+    QFrame, QWidget, QVBoxLayout, QScrollArea, 
+    QPushButton, QHBoxLayout, QFileDialog
 )
 
+from ..common_widgets import Label
+from ..signals import all_signals
+from ...pyk4a.pykinect import start_playback, initialize_libraries
 
-if not os.path.exists("./tools/pyk4a/example/outputs/"):
-    os.mkdir("./tools/pyk4a/example/outputs")
 
+class ExplorerSidebar(QFrame):
+    def __init__(self) -> None:
+        super().__init__()
+        initialize_libraries()
+        self.setStyleSheet(" background-color: #252526; border-radius: 0px; ")
 
-def callback(indata, frames, time, status):
-    global q
-    """This is called (from a separate thread) for each audio block."""
-    if status:
-        print(status, file=sys.stderr)
-    q.put(indata.copy())
-
-
-class Thread(QThread):
-    updateFrame = Signal(QImage)
-
-    def __init__(self, parent=None):
-        QThread.__init__(self, parent)
-        self.trained_file = None
-        self.status = True
-        self.cap = True
-        # self.args = args
-
-        self.set_filename()
-
-    def set_filename(self):
-        filename = datetime.datetime.now()
-        filename = filename.strftime("%Y_%m_%d_%H_%M_%S")
-        base_path = (
-            "C:\\Program Files\\Azure Kinect SDK v1.4.1\\tools\\pyk4a\\example\\outputs"
-        )
+        self.main_layout = QVBoxLayout()
+        self.title_layout = QHBoxLayout()
+        self.base_path = os.path.join(Path.home(), "Videos")
+
+        self.label_dirpath = Label(self.base_path)
+        self.label_dirpath.setFixedSize(180, 50)
+        
+        self.btn_reload = self.make_icons(qta.icon("mdi6.reload"), "Reload", scale=0.7)
+        self.btn_search = self.make_icons(qta.icon("ri.search-line"), "Search directory", scale=0.7)
+
+        self.title_layout.addWidget(self.label_dirpath)
+        self.title_layout.addWidget(self.btn_reload)
+        self.title_layout.addWidget(self.btn_search)
+
+        self.layout_scroll = QScrollArea()
+        self.layout_scroll.setWidgetResizable(True)
+        self.layout_scroll.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
+        self.layout_scroll.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
+
+        self.main_layout.addLayout(self.title_layout)
+        self.main_layout.addWidget(self.layout_scroll)
+        self.setMaximumHeight(1080)
+        self.setFixedWidth(300)
+        self.setLayout(self.main_layout)
+        self.set_scrollarea(self.base_path)
+
+        self.btn_reload.clicked.connect(self.reload_dir)
+        self.btn_search.clicked.connect(self.search_dir)
+
+    def reload_dir(self) -> None:
+        self.set_scrollarea(self.base_path)
+
+    def search_dir(self) -> None:
+        self.base_path = QFileDialog.getExistingDirectory(self, "Open Data Files", ".", QFileDialog.ShowDirsOnly)
+        self.label_dirpath.setText(self.base_path)  # /etc/ssh/ or /etc/ssh/config.txt
+        self.set_scrollarea(self.base_path)
+
+    def set_scrollarea(self, filedirs: str) -> None:
+        self._widget = QWidget()
+        layout_file = QVBoxLayout()
+        layout_file.setAlignment(Qt.AlignmentFlag.AlignTop)
+
+        for filedir in Path(filedirs).iterdir():
+            _filename = str(filedir).split("\\")[-1]
+            if _filename[-4:] == ".mkv":
+                try:
+                    fileinfo = _FileInfo()
+                    playback = start_playback(str(filedir))
+                    handle = playback.get_record_configuration()._handle
+                    start_time = handle.start_timestamp_offset_usec
+
+                    # Thumbnail
+                    # playback.seek_timestamp(start_time)
+                    # _, current_frame = playback.update()
+                    # rgb_frame = current_frame.get_color_image()
+                    # thumbnail = cv2.cvtColor(rgb_frame[1], cv2.COLOR_BGR2RGB)
+                    # thumbnail = QImage(thumbnail, 30, 30, 30*3, QImage.Format_RGB888)
+                    # fileinfo.label_thumbnail.setPixmap(QPixmap.fromImage(thumbnail))
+                    
+                    record_length = (playback.get_recording_length()-start_time) // 1e6
+                    fsize = os.path.getsize(filedir) / (2**30)
+                    record_time = str(datetime.timedelta(seconds=record_length))
+                    playback.close()
+                    
+                    font_metrics = fileinfo.label_file_name.fontMetrics()
+                    elided_text = font_metrics.elidedText(_filename, Qt.ElideRight, fileinfo.label_file_name.width())
+                    fileinfo.label_file_name.setText(elided_text)
+                    fileinfo.label_metadata.setText(f"{record_time} ({fsize:.2f}GB)")
+                    layout_file.addWidget(fileinfo)
+                    fileinfo.Filename.connect(self.emit_file_path)
+                except:
+                    pass
+
+        self._widget.setLayout(layout_file)
+        self.layout_scroll.setWidget(self._widget)
+    
+    def make_icons(self, icon: qta, tooltip: str, scale: float = 0.8) -> QPushButton:
+        w, h = int(35 * scale), int(35 * scale)
+        btn = QPushButton(icon, "")
+        btn.setObjectName(tooltip)
+        btn.setFixedSize(40, 40)
+        btn.setIconSize(QSize(w, h))
+        btn.setToolTip(f"<b>{tooltip}<b>")
+        btn.setStyleSheet("""
+            QPushButton {
+                border-radius: 0px;
+            }
+            QPushButton:hover {
+                border-color: white;
+            }
+            QToolTip {
+                font:"Arial"; font-size: 15px; color: #ffffff; border: 1px solid #ffffff; 
+            }
+        """)
+        return btn
+
+    @Slot(str)
+    def emit_file_path(self, filename) -> None:
+        tmp = os.path.join(self.base_path, filename)
+        all_signals.playback_signals.playback_filepath.emit(tmp)
 
-        self.filename_video = f"{base_path}\\{filename}.mkv"
-        self.filename_audio = f"{base_path}\\{filename}.wav"
-        print(filename)
-
-    def run(self):
-        global q
-        # pyk4a
-        config = Config(
-            color_format=ImageFormat.COLOR_BGRA32,
-            depth_mode=pyk4a.DepthMode.NFOV_UNBINNED,
-            color_resolution=pyk4a.ColorResolution.RES_720P,
-            synchronized_images_only=True,
-        )
-        azure_device = PyK4A(config=config, device_id=0)
-        azure_device.start()
-        record = PyK4ARecord(
-            device=azure_device, config=config, path=self.filename_video
-        )
-        record.create()
 
-        with sf.SoundFile(
-            self.filename_audio,
-            mode="x",
-            samplerate=44100,
-            channels=2,
-            subtype="PCM_24",
-        ) as file:
-            with sd.InputStream(
-                samplerate=44100,
-                device="Azure Kinect Microphone , MME",
-                channels=2,
-                callback=callback,
-            ):
-                while self.status:
-                    capture = azure_device.get_capture()
-                    record.write_capture(capture)
-                    file.write(q.get())
-
-                    # print(capture.color[:, :, :3])
-                    if np.any(capture.color):
-                        frame = capture.color[:, :, :3].copy()
-                        frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
-
-                        h, w, ch = capture.color[:, :, :3].shape
-                        img = QImage(frame, w, h, ch * w, QImage.Format_RGB888)
-                        scaled_img = img.scaled(640, 480, Qt.KeepAspectRatio)
-                        # Emit signal
-                        self.updateFrame.emit(scaled_img)
-
-        record.flush()
-        record.close()
-        print(f"{record.captures_count} frames written.")
-
-        src = self.filename_audio
-        dst = f"{self.filename_audio[:-4]}.mp3"
-
-        sound = AudioSegment.from_mp3(src)
-        sound.export(dst, format="wav")
+class _FileInfo(QPushButton):
+    Filename = Signal(str)
 
-        os.remove(self.filename_audio)
-        print("finish to save")
+    def __init__(self) -> None:
+        super().__init__()
+        self.setFixedSize(240, 60)
+        self.setObjectName("FileInfo")
+        self.setStyleSheet(
+            """
+            QPushButton#FileInfo {
+                border-color: white;
+                border-radius: 0px;
+            }
+            QPushButton#FileInfo:hover {
+                border-color: red;
+            }
+        """
+        )
 
+        main_layout = QVBoxLayout()
+        self.thumbnail_layout = QHBoxLayout()
+        # self.label_thumbnail = Label()
+        self.label_file_name = Label("File name: ", "Arial", 10, Qt.AlignLeft)
+        self.label_file_name.setWordWrap(True)
+        # self.label_file_name.setFixedWidth(240)
+        # self.thumbnail_layout.addWidget(self.label_thumbnail)
+        self.thumbnail_layout.addWidget(self.label_file_name)
+        main_layout.addLayout(self.thumbnail_layout)
+
+        self.metadata_layout = QHBoxLayout()
+        self.label_metadata = Label("", "Arial", 10, Qt.AlignLeft)
+        self.metadata_layout.addWidget(self.label_metadata)
+        main_layout.addLayout(self.metadata_layout)
+        self.setLayout(main_layout)
 
-class Window(QMainWindow):
-    def __init__(self):
-        super().__init__()
-        # Title and dimensions
-        self.setWindowTitle("Patterns detection")
-        self.setGeometry(0, 0, 800, 500)
-
-        # Create a label for the display camera
-        self.label = QLabel(self)
-        self.label.setFixedSize(640, 480)
-
-        # Thread in charge of updating the image
-        self.th = Thread(self)
-        # self.th.finished.connect(self.close)
-        self.th.updateFrame.connect(self.setImage)
-
-        # Buttons layout
-        buttons_layout = QHBoxLayout()
-        self.button1 = QPushButton("Start")
-        self.button2 = QPushButton("Stop/Close")
-        self.button1.setSizePolicy(QSizePolicy.Preferred, QSizePolicy.Expanding)
-        self.button2.setSizePolicy(QSizePolicy.Preferred, QSizePolicy.Expanding)
-        buttons_layout.addWidget(self.button2)
-        buttons_layout.addWidget(self.button1)
-
-        # Main layout
-        layout = QVBoxLayout()
-        layout.addWidget(self.label)
-        layout.addLayout(buttons_layout)
-        # layout.addLayout(right_layout)
-
-        # Central widget
-        widget = QWidget(self)
-        widget.setLayout(layout)
-        self.setCentralWidget(widget)
-
-        # Connections
-        self.button1.clicked.connect(self.start)
-        self.button2.clicked.connect(self.kill_thread)
-        self.button2.setEnabled(False)
-
-    @Slot()
-    def kill_thread(self):
-        print("Finishing...")
-        self.button2.setEnabled(False)
-        self.button1.setEnabled(True)
-        # cv2.destroyAllWindows()
-        self.th.status = False
-        # Give time for the thread to finish
-        time.sleep(1)
-
-    @Slot()
-    def start(self):
-        print("Starting...")
-        self.button2.setEnabled(True)
-        self.button1.setEnabled(False)
-        self.th.set_filename()
-        self.th.status = True
-        self.th.start()
-
-    @Slot(QImage)
-    def setImage(self, image):
-        self.label.setPixmap(QPixmap.fromImage(image))
-
-
-if __name__ == "__main__":
-    q = queue.Queue()
-    app = QApplication()
-    w = Window()
-    w.show()
-    sys.exit(app.exec())
+        self.clicked.connect(self.emitName)
 
-    # main(args)
+    def emitName(self) -> None:
+        self.Filename.emit(self.label_file_name.text())
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/main/synology_utils.py` & `pykinect_recorder-0.9.2/pykinect_recorder/renderer/synology_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,15 @@
             args.secure,
             args.cert_verify,
             args.dsm_version,
             args.debug,
             args.otp_code,
         )
 
-        success = f1.upload_file(
-            args.dest_path, args.file_path, verify=args.cert_verify
-        )
+        success = f1.upload_file(args.dest_path, args.file_path, verify=args.cert_verify)
         if type(success) == tuple:
             raise ConnectionAbortedError
         else:
             print(success)
 
     except ValueError:
         print("Connect Failed!! Please Check your ip, port, username, password, secure")
@@ -52,17 +50,15 @@
         type=str,
         default="hnvlab.synology.me",
         help="Set Ip address such as xxx.synology.me or 111.111.1.1",
     )
     parser.add_argument("--Synology_Port", type=str, default="", help="")
     parser.add_argument("--Username", type=str, default="", help="")
     parser.add_argument("--Password", type=str, default="", help="")
-    parser.add_argument(
-        "--secure", type=bool, default=True, help="Set True if https is required"
-    )
+    parser.add_argument("--secure", type=bool, default=True, help="Set True if https is required")
     parser.add_argument(
         "--cert_verify",
         type=bool,
         default=True,
         help="Set True if you want to verify your certificate",
     )
     parser.add_argument("--dsm_version", type=int, default=7)
@@ -71,14 +67,12 @@
 
     parser.add_argument(
         "--dest_path",
         type=str,
         default="/dataset/test",
         help="Destination path in synology nas",
     )
-    parser.add_argument(
-        "--file_path", type=str, default="ecord_with_mic.py", help="Upload file path"
-    )
+    parser.add_argument("--file_path", type=str, default="ecord_with_mic.py", help="Upload file path")
 
     args = parser.parse_args()
     # upload(args)
     download(args)
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/renderer/common_widgets.py` & `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/topbar.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,159 +1,123 @@
 import os
-from typing import Tuple, Union, List
-from PySide6.QtCore import Qt, QPoint
-from PySide6.QtGui import QFont, QPen, QPainter, QFontMetrics
 
+from PySide6.QtGui import QAction, QIcon
+from PySide6.QtCore import Qt, QSize
 from PySide6.QtWidgets import (
-    QLabel, QComboBox, QPushButton, QSlider, 
-    QFrame, QVBoxLayout, QHBoxLayout
+    QHBoxLayout, QFrame, QPushButton,
+    QMenuBar, QMenu, QApplication, QToolBar
 )
+import qtawesome as qta
 
+from ..signals import all_signals
+from ..common_widgets import Label
+from ...pyk4a.utils import get_root
 
-class ComboBox(QComboBox):
-    def __init__(
-        self, 
-        items: List[str], 
-        current_index: int,
-        stylesheet: Union[str, os.PathLike] = None
-    ) -> None:
-        super().__init__()
-        self.addItems(items)
-        self.setCurrentIndex(current_index)
 
-        # TODO: 외부 함수화 또는 PySide6에서 이런 함수 있는지 찾아보셈
-        if stylesheet is not None:
-            with open(os.path.join(os.path.split(__file__)[0], stylesheet), "r", encoding="utf-8") as f:
-                stylesheet = f.read()
-                print(stylesheet)
-            self.setStyleSheet(str(stylesheet))
-
-
-class PushButton(QPushButton):
-    def __init__(
-        self, 
-        text: str = "",
-        font: str = "Arial", 
-        fontsize: int = 10, 
-        stylesheet: Union[str, os.PathLike] = None
-    ) -> None:
+class Topbar(QFrame):
+    def __init__(self) -> None:
         super().__init__()
-        self.setText(text)
-        self.setFont(QFont(f"{font}", fontsize))
-        self.setStyleSheet(
-            "color: white;"
-        )
-
-        if stylesheet is not None:
-            with open(os.path.join(os.path.split(__file__)[0], stylesheet), "r", encoding="utf-8") as f:
-                stylesheet = f.read()
-                print(stylesheet)
-            self.setStyleSheet(str(stylesheet))
-
-
-class Slider(QSlider):
-    def __init__(
-        self, 
-        orientation, 
-        set_range_values: Tuple[int], 
-        set_value: int, 
-    ) -> None:
-        super().__init__(orientation)
-        self.setRange(*set_range_values)
-        self.setValue(set_value)
-
-        self.setStyleSheet(
-            """
-            QSlider { 
-                margin: 0px;
-                border-radius: 4px;
-            }
-            QSlider::sub-page:horizontal {
-                background-color: #3f4042;
-                height: 12px;
-                border-radius: 4px;
-            }
-            QSlider::groove:horizontal {
-                height: 12px;
-                margin: 1px;
-                border-radius: 4px;
-                background-color: "#3f4042"
-            }
-            QSlider::handle:horizontal {
-                border: 10px;
-                margin: 0px;
-                border-radius: 3px;
-                background-color: "#00bcf8";
+        self.setFixedHeight(40)
+        self.setMaximumWidth(4000)
+        self.setContentsMargins(0, 0, 0, 0)
+        self.setWindowFlags(self.windowFlags() | Qt.FramelessWindowHint)
+
+        self.setObjectName("Topbar")
+        self.setStyleSheet("""
+            QFrame#Topbar {
+                background-color: #323233; 
+                padding: 0px; margin: 0px; 
+                border-radius: 0px;
+            }
+        """)
+
+        main_layout = QHBoxLayout()
+        main_layout.setSpacing(0)
+        main_layout.setContentsMargins(0, 0, 0, 0)
+        main_layout.setAlignment(Qt.AlignLeft)
+
+        self.label_icon = Label()
+        self.label_icon.setStyleSheet("margin-left: 6px;")
+        self.label_icon.setFixedSize(40, 40)
+        self.icon = QIcon(os.path.join(get_root(), "renderer/public/kinect-sensor.ico"))
+        self.pixmap = self.icon.pixmap(25, 25)
+        self.label_icon.setPixmap(self.pixmap)
+        main_layout.addWidget(self.label_icon)    
+
+        self.menubar = QMenuBar()
+        self.menubar.setFixedWidth(100)
+        self.menubar.setContentsMargins(0, 0, 0, 0)
+        self.menubar.setStyleSheet("""
+            QMenuBar {
+                font-size: 15px; 
+                background-color: #323233; 
+                border: none;                              
             }
-            QSlider:handle:horizontal:hover {
-                background-color: "#4d96FF";
-            }
-            QSlider:handle:horizontal:pressed {
-                background-color: "#FFFFFF";
+            QMenuBar:item:selected {
+                border-color: white;
+                border-radius: 0px;                      
             }
-            """
-        )
-
-    def paintEvent(self, event):
-        QSlider.paintEvent(self, event)
+        """)
 
-        curr_value = str(self.value())
-        painter = QPainter(self)
-        painter.setPen(QPen(Qt.white))
-
-        font_metrics = QFontMetrics(self.font())
-        font_width = font_metrics.boundingRect(curr_value).width()
-
-        rect = self.geometry()
-        if self.orientation() == Qt.Horizontal:
-            horizontal_x_pos = rect.width()//2 - font_width//2 - 5
-            horizontal_y_pos = rect.height() * 0.7
-            painter.drawText(QPoint(horizontal_x_pos, horizontal_y_pos), curr_value)
-        else:
-            pass
-
-
-class Label(QLabel):
-    def __init__(
-        self, 
-        text: str = "",
-        font: str = "Arial", 
-        fontsize: int = 10, 
-        orientation = None,
-        stylesheet: Union[str, os.PathLike] = None
-    ) -> None:
-        super().__init__()
-        self.setText(text)
-        self.setFont(QFont(f"{font}", fontsize))
-        if orientation is not None:
-            self.setAlignment(orientation)
-
-        if stylesheet is not None:
-            with open(os.path.join(os.path.split(__file__)[0], stylesheet), "r", encoding="utf-8") as f:
-                stylesheet = f.read()
-                print(stylesheet)
-            self.setStyleSheet(str(stylesheet))
-
-
-class Frame(QFrame):
-    def __init__(
-        self,
-        text: str,
-        layout: Union[QVBoxLayout, QHBoxLayout] = None,
-    ) -> None:
-        super().__init__()
-        self.setMaximumHeight(480)
-        self.setFixedWidth(640)
-        self.setObjectName("Frame")
-        self.setStyleSheet(
-            """QFrame#Frame {
-                border-color: white;
-            }"""
-        )
+        self.file_menu = QMenu("File")
+        self.help_menu = QMenu("Help")
+        self.file_menu.setContentsMargins(0, 0, 0, 0)
+        self.help_menu.setContentsMargins(0, 0, 0, 0)
         
-        if layout is None:
-            self.layout_main = QVBoxLayout()
-            self.frame = Label(text, orientation=Qt.AlignmentFlag.AlignCenter)
-            self.layout_main.addWidget(self.frame)
-            self.setLayout(self.layout_main)
-        else:
-            self.setLayout(layout)
+        self.exit_action = QAction("Exit")
+        self.info_action = QAction("Info")
+
+        self.file_menu.addAction(self.exit_action)
+        self.help_menu.addAction(self.info_action)
+        self.menubar.addMenu(self.file_menu)
+        self.menubar.addMenu(self.help_menu)
+        main_layout.addWidget(self.menubar)
+
+        self.title_layout = QHBoxLayout()
+        self.title_layout.setAlignment(Qt.AlignCenter)
+        self.label_title = Label("pykinect-recorder", font="Arial", fontsize=12, orientation=Qt.AlignCenter)
+        self.title_layout.addWidget(self.label_title)
+        main_layout.addLayout(self.title_layout)
+
+        self.right_btn_layout = QHBoxLayout()
+        self.right_btn_layout.setSpacing(0)
+        self.right_btn_layout.setContentsMargins(0, 0, 0, 0)
+        self.btn_minimize = self.make_icons(qta.icon("msc.chrome-minimize"), "minimize")
+        self.btn_maximize = self.make_icons(qta.icon("msc.chrome-maximize"), "maximize")
+        self.btn_close = self.make_icons(qta.icon("msc.chrome-close"), "close")
+        self.right_btn_layout.addWidget(self.btn_minimize)
+        self.right_btn_layout.addWidget(self.btn_maximize)
+        self.right_btn_layout.addWidget(self.btn_close)
+        main_layout.addLayout(self.right_btn_layout)
+        self.setLayout(main_layout)
+
+        self.exit_action.triggered.connect(self.quit_window)
+        self.info_action.triggered.connect(self.get_window_info)
+        self.btn_minimize.clicked.connect(self.right_btn_clicked)
+        self.btn_maximize.clicked.connect(self.right_btn_clicked)
+        self.btn_close.clicked.connect(self.right_btn_clicked)
+    
+    def make_icons(self, icon: qta, tooltip: str, scale: float = 0.8) -> QPushButton:
+        w, h = int(35 * scale), int(35 * scale)
+        btn = QPushButton(icon, "")
+        btn.setObjectName(tooltip)
+        btn.setFixedSize(38, 38)
+        btn.setIconSize(QSize(w, h))
+        btn.setToolTip(f"<b>{tooltip}<b>")
+        btn.setStyleSheet("""
+            QPushButton {
+                border: none; border-radius: 0px;
+            }
+            QToolTip {
+                font:"Arial"; font-size: 15px; color: #ffffff; border: 1px solid #ffffff; 
+            }             
+        """)
+        return btn
+    
+    def right_btn_clicked(self):
+        all_signals.window_control.emit(self.sender().objectName())
+
+    def quit_window(self):
+        QApplication.instance().quit()
+
+    def get_window_info(self):
+        print("pass")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/playback_sensors.py` & `pykinect_recorder-0.9.2/pykinect_recorder/renderer/split_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,76 +1,77 @@
+import os
 import cv2
-import time
-
-from numpy.typing import NDArray
-from typing import Optional, Tuple
-
-from PySide6.QtCore import Qt, Signal, QThread
-from PySide6.QtGui import QImage
-from pykinect_recorder.main._pyk4a.k4arecord.playback import Playback
-from ..signals import all_signals
-
-
-
-class PlaybackSensors(QThread):
-    def __init__(self, playback: Playback, parent=None) -> None:
-        QThread.__init__(self, parent)
-        self.playback = playback
-        self.is_run = None
-
-    def run(self):      
-        while self.is_run:
-            start_t = time.time()
-            _, current_frame = self.playback.update()
-            current_rgb_frame = current_frame.get_color_image()
-            current_depth_frame = current_frame.get_depth_image()
-            current_ir_frame = current_frame.get_ir_image()
-
-            if current_rgb_frame[0]:
-                rgb_frame = current_rgb_frame[1]
-                rgb_frame = cv2.cvtColor(rgb_frame, cv2.COLOR_BGR2RGB)
-                
-                h, w, ch = rgb_frame.shape
-                rgb_frame = QImage(rgb_frame, w, h, ch * w, QImage.Format_RGB888)
-                scaled_rgb_frame = rgb_frame.scaled(720, 440, Qt.KeepAspectRatio)
-                all_signals.captured_rgb.emit(scaled_rgb_frame)
-
-            if current_depth_frame[0]:
-                depth_frame = self._colorize(
-                    current_depth_frame[1], (None, 5000), cv2.COLORMAP_HSV
-                )
-                h, w, ch = depth_frame.shape
-
-                depth_frame = QImage(depth_frame, w, h, w * ch, QImage.Format_RGB888)
-                scaled_depth_frame = depth_frame.scaled(440, 440, Qt.KeepAspectRatio)
-                all_signals.captured_depth.emit(scaled_depth_frame)
-
-            if current_ir_frame[0]:
-                ir_frame = self._colorize(
-                    current_ir_frame[1], (None, 5000), cv2.COLORMAP_BONE
-                )
-                h, w, ch = ir_frame.shape
-
-                ir_frame = QImage(ir_frame, w, h, w * ch, QImage.Format_RGB888)
-                scaled_ir_frame = ir_frame.scaled(440, 440, Qt.KeepAspectRatio)
-                all_signals.captured_ir.emit(scaled_ir_frame)
-
-            end_time = time.time()
-            try:
-                fps = 1/(end_time-start_t)
-                all_signals.captured_fps.emit(fps)
-            except:
-                pass
-
-    def _colorize(
-        self,
-        image: NDArray,
-        clipping_range: Tuple[Optional[int], Optional[int]] = (None, None),
-        colormap: int = cv2.COLORMAP_HSV,
-    ) -> NDArray:
-        if clipping_range[0] or clipping_range[1]:
-            img = image.clip(clipping_range[0], clipping_range[1])  # type: ignore
-        else:
-            img = image.copy()
-        img = cv2.normalize(img, None, 0, 255, cv2.NORM_MINMAX, dtype=cv2.CV_8U)
-        img = cv2.applyColorMap(img, colormap)
-        return img
+import sys
+import pandas as pd
+from glob import glob
+from pathlib import Path
+from pykinect_recorder.pyk4a.pykinect import initialize_libraries
+from pykinect_recorder.pyk4a.k4arecord import Playback
+from pykinect_recorder.pyk4a.k4arecord._k4arecord import K4A_PLAYBACK_SEEK_BEGIN
+
+
+def colorize(
+    image,
+    clipping_range,
+    colormap,
+):
+    if clipping_range[0] or clipping_range[1]:
+        img = image.clip(clipping_range[0], clipping_range[1])  # type: ignore
+    else:
+        img = image.copy()
+    img = cv2.normalize(img, None, 0, 255, cv2.NORM_MINMAX, dtype=cv2.CV_8U)
+    img = cv2.applyColorMap(img, colormap)
+    return img
+
+
+if __name__ == "__main__":
+    initialize_libraries()
+    # with open("dataset_list.txt", "r", encoding="utf-8") as f:
+    #     file_paths = f.readlines()
+    file_paths = glob(os.path.join(Path.home(), "Desktop/baby", "*.mkv"))
+    root_path = "datas"
+    if not os.path.exists(root_path):
+        os.mkdir(root_path)
+    print(len(file_paths))
+
+    for i, file_path in enumerate(file_paths):
+        print(i, file_path)
+        file_name = file_path.split("\\")[-1][:-4]
+        os.makedirs(os.path.join(root_path, file_name, "rgb"), exist_ok=True)
+        os.makedirs(os.path.join(root_path, file_name, "ir"), exist_ok=True)
+        playback = Playback(file_path)
+        playback.seek_timestamp(offset=333555, origin=K4A_PLAYBACK_SEEK_BEGIN)
+        cnt = 0
+        # frame = 100
+        color_h, color_w = None, None
+        depth_h, depth_w = None, None
+
+        while True:
+            ret, current_frame = playback.update()
+            if ret:
+                current_rgb_frame = current_frame.get_color_image()
+                current_ir_frame = current_frame.get_ir_image()
+                if current_ir_frame[0]:
+                    ir_frame = colorize(current_ir_frame[1], (None, 5000), cv2.COLORMAP_BONE)
+                    depth_h, depth_w, _ = ir_frame.shape
+                    cv2.imwrite(
+                        os.path.join(root_path, file_name, "ir", f"{file_name}_ir_{str(cnt).zfill(6)}.png"),
+                        ir_frame,
+                    )
+
+                if current_rgb_frame[0]:
+                    rgb_frame = current_rgb_frame[1]
+                    color_h, color_w, _ = rgb_frame.shape
+                    cv2.imwrite(
+                        os.path.join(root_path, file_name, "rgb", f"{file_name}_rgb_{str(cnt).zfill(6)}.jpg"),
+                        rgb_frame,
+                        [cv2.IMWRITE_JPEG_QUALITY, 100],
+                    )
+                cnt += 1
+            else:
+                break
+
+        df = pd.read_csv("metadata.csv")
+        length = df.shape[0]
+        df.loc[length] = [file_name, 333555, cnt, f"'({color_h}, {color_w})'", f"'({depth_h}, {depth_w})'"]
+        df.to_csv("metadata.csv", index=False)
+        print(file_name)
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/sidebar_control.py` & `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/sidebar_control.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from PySide6.QtCore import Slot
-from PySide6.QtWidgets import (
-    QStackedLayout, QFrame
-)
+from PySide6.QtWidgets import QStackedLayout, QFrame
 
 from .sidebar_solutions import SolutionSidebar
 from .sidebar_record_control import ViewerSidebar
 from .sidebar_explorer import ExplorerSidebar
+from ..signals import all_signals
 
 
 class StackedSidebar(QFrame):
     def __init__(self) -> None:
         super().__init__()
-
+        self.setMaximumWidth(330)
+        self.setContentsMargins(0, 0, 0, 0)
         self.main_layout = QStackedLayout()
         self.sidebar_viewer = ViewerSidebar()
         self.sidebar_explorer = ExplorerSidebar()
         self.sidebar_solution = SolutionSidebar()
-        
-        self.main_layout.addWidget(self.sidebar_viewer) 
-        self.main_layout.addWidget(self.sidebar_explorer) 
-        self.main_layout.addWidget(self.sidebar_solution) 
-        
-        # 현재 index
+
+        self.main_layout.addWidget(self.sidebar_viewer)
+        self.main_layout.addWidget(self.sidebar_explorer)
+        self.main_layout.addWidget(self.sidebar_solution)
+
         self.main_layout.setCurrentIndex(0)
         self.setLayout(self.main_layout)
 
+        all_signals.option_signals.stacked_sidebar_status.connect(self.set_current_widget)
 
     @Slot(str)
-    def setCurrentWidget(self, value):
+    def set_current_widget(self, value):
         if value == "explorer":
             self.main_layout.setCurrentWidget(self.sidebar_explorer)
         elif value == "solution":
             self.main_layout.setCurrentWidget(self.sidebar_solution)
         else:
-            self.main_layout.setCurrentWidget(self.sidebar_viewer)
+            self.main_layout.setCurrentWidget(self.sidebar_viewer)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/viewer_control.py` & `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_control.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from PySide6.QtCore import Slot
-from PySide6.QtWidgets import (
-    QStackedLayout, QFrame
-)
+from PySide6.QtCore import Slot, Qt
+from PySide6.QtWidgets import QStackedLayout, QFrame, QHBoxLayout, QWidget
 
-from .viewer_sensors import SensorViewer 
+from .viewer_sensors import SensorViewer
 from .viewer_playback import PlaybackViewer
 from .viewer_solution import ViewerSolution
-from .asidebar import Asidebar
+from ..signals import all_signals
 
 
 class StackedViewer(QFrame):
     def __init__(self) -> None:
         super().__init__()
 
-        self.setMaximumHeight(1080)
-        self.setMaximumWidth(1300)
+        self.setMaximumHeight(2080)
+        self.setMaximumWidth(2300)
+        self.setContentsMargins(0, 0, 0, 0)
         self.main_layout = QStackedLayout()
+        # self.main_layout.setAlignment(Qt.AlignTop | Qt.AlignLeft)
         self.main_viewer = SensorViewer()
         self.main_explorer = PlaybackViewer()
         self.main_solution = ViewerSolution()
-        
+
         self.main_layout.addWidget(self.main_viewer)
         self.main_layout.addWidget(self.main_explorer)
         self.main_layout.addWidget(self.main_solution)
 
-        # 현재 index
         self.main_layout.setCurrentIndex(0)
-        self.setLayout(self.main_layout)
-
+        self.setLayout(self.main_layout)   
+        
+        all_signals.option_signals.stacked_sidebar_status.connect(self.set_current_widget)
 
     @Slot(str)
-    def setCurrentWidget(self, value):
+    def set_current_widget(self, value):
         if value == "explorer":
             self.main_layout.setCurrentWidget(self.main_explorer)
         elif value == "solution":
             self.main_layout.setCurrentWidget(self.main_solution)
         else:
-            self.main_layout.setCurrentWidget(self.main_viewer)
+            self.main_layout.setCurrentWidget(self.main_viewer)
+        all_signals.option_signals.clear_frame.emit(True)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/renderer/components/viewer_sensors.py` & `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_sensors.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,164 +1,197 @@
 import os
 import sys
 import time
 import ctypes
 import datetime
 from pathlib import Path
 
-from PySide6.QtCore import Qt, Slot, QEvent, QMimeData, QPointF
+from PySide6.QtCore import Qt, Slot, QEvent, QMimeData, QPointF, QSize
 from PySide6.QtGui import QImage, QPixmap, QDrag
-from PySide6.QtWidgets import (
-    QHBoxLayout, QPushButton, QVBoxLayout, 
-    QFrame, QDialog, QGridLayout
-)
+from PySide6.QtWidgets import QHBoxLayout, QVBoxLayout, QFrame, QGridLayout
 
-from ..common_widgets import Label, Frame
 from .record_sensors import RecordSensors
-from .playback_sensors import PlaybackSensors
 from .viewer_imu_sensors import ImuSensors
 from .viewer_audio import AudioSensor
-from pykinect_recorder.main._pyk4a.k4a._k4a import k4a_device_set_color_control
-from pykinect_recorder.main._pyk4a.k4a._k4atypes import color_command_dict, K4A_COLOR_CONTROL_MODE_MANUAL
-from pykinect_recorder.main._pyk4a.k4a.configuration import Configuration
-from pykinect_recorder.main._pyk4a.pykinect import start_device, initialize_libraries, start_playback
-from .sidebar_record_control import _config_sidebar
+from .sidebar_record_control import config_sidebar
 from ..signals import all_signals
+from ..common_widgets import Frame, VLine, CustomProgressBarDialog
+from ...pyk4a.k4a._k4a import k4a_device_set_color_control, k4a_image_set_exposure_time_usec
+from ...pyk4a.k4a._k4atypes import color_command_dict, K4A_COLOR_CONTROL_MODE_MANUAL
+from ...pyk4a.k4a.configuration import Configuration
+from ...pyk4a.pykinect import start_device
 
 
 SAMPLE_COUNT = 10000
 RESOLUTION = 4
 
 
 class SensorViewer(QFrame):
-    def __init__(self, size: tuple[int, int] = (1200, 1000)) -> None:
+    def __init__(self) -> None:
         super().__init__()
+        
+        self.setMinimumSize(QSize(920, 670))
+        self.setMaximumSize(QSize(1190, 1030))
+        self.setContentsMargins(0, 0, 0, 0)
+        self.setStyleSheet("background-color: #1e1e1e; border-radius: 0px;")
 
-        self.setStyleSheet("background-color: #1e1e1e;") 
         self.device = None
-        self.config = None
+        self.config = Configuration()
         self.color_control = None
         self.base_path = None
-        self.emit_configs = _config_sidebar
+        self.emit_configs = config_sidebar
 
-        self.grid_layout = QGridLayout()
-        self.frame_rgb = Frame("RGB Sensor")
-        self.frame_depth = Frame("Depth Sensor")
-        self.frame_ir = Frame("IR Sensor")
+        self.main_layout = QGridLayout()
+        self.main_layout.setSpacing(0)
+        self.main_layout.setContentsMargins(0, 0, 0, 0)
+        self.main_layout.setAlignment(Qt.AlignCenter)
+        self.frame_rgb = Frame("RGB Sensor", min_size=(460, 330), max_size=(595, 510))
+        self.frame_depth = Frame("Depth Sensor", min_size=(460, 330), max_size=(595, 510))
+        self.frame_ir = Frame("IR Sensor", min_size=(460, 330), max_size=(595, 510))
+
+        self.sensor_data_layout = QHBoxLayout()
+        self.sensor_data_layout.setSpacing(0)
+        self.sensor_data_layout.setContentsMargins(0, 0, 0, 0)
+        self.imu_senser = ImuSensors(min_size=(225, 300), max_size=(440, 480))
+        self.audio_sensor = AudioSensor(min_size=(225, 300), max_size=(440, 480))
+
+        self.v_line = QVBoxLayout()
+        self.v_line.setSpacing(0)
+        self.v_line.setContentsMargins(0, 0, 0, 0)
+        self.v_line.addWidget(VLine())
         
-        self.layout_subdata = QHBoxLayout() # TODO => 네이밍 다시 하기
-        self.imu_senser = ImuSensors()
-        self.audio_sensor = AudioSensor()
-        self.layout_subdata.addWidget(self.imu_senser)
-        self.layout_subdata.addWidget(self.audio_sensor)
-        self.frame_subdata = Frame("subdata", layout=self.layout_subdata)
-
-        layout_btn = QHBoxLayout()
-        layout_btn.setAlignment(Qt.AlignmentFlag.AlignCenter)
-        self.btn_open = QPushButton("Device open")
-        self.btn_open.setFixedSize(200, 40)
-        self.btn_viewer = QPushButton("▶")
-        self.btn_viewer.setFixedSize(200, 40)
-        self.btn_record = QPushButton("●")
-        self.btn_record.setFixedSize(200, 40)
-
-        self.btn_open.setStyleSheet("""
-            QPushButton:hover {
-                border-color: "white";
-            }
-        """)
-        self.btn_viewer.setStyleSheet("""
-            QToolTip {
-                font:"Arial"; font-size: 15px; color: #ffffff; border: 1px solid #ffffff; 
-            }
-            QPushButton:hover {
-                border-color: "white";
-            }
-            """
-        )
-        self.btn_record.setStyleSheet("""
-            QToolTip {
-                font:"Arial"; font-size: 15px; color: #ffffff; border: 1px solid #ffffff; 
-            }
-            QPushButton {
-                background-color: red;
-            }
-            QPushButton:hover {
-                border-color: "white";
-            }
-            """
+        self.sensor_data_layout.addWidget(self.imu_senser)
+        self.sensor_data_layout.addLayout(self.v_line)
+        self.sensor_data_layout.addWidget(self.audio_sensor)
+        self.frame_subdata = Frame(
+            "IMU & Audio Sensor", 
+            layout=self.sensor_data_layout, 
+            min_size=(460, 330), 
+            max_size=(595, 510)
         )
-        
-
-        self.btn_viewer.setToolTip("<b>Streaming Button</b>")
-        self.btn_record.setToolTip("<b>Recording Button</b>")
 
-        layout_btn.addStretch()
-        layout_btn.addStretch()
-        layout_btn.addWidget(self.btn_open)
-        layout_btn.addStretch()
-        layout_btn.addWidget(self.btn_viewer)
-        layout_btn.addStretch()
-        layout_btn.addWidget(self.btn_record)      
-        layout_btn.addStretch()
-        layout_btn.addStretch()
-        
         self.buffer = [QPointF(x, 0) for x in range(SAMPLE_COUNT)]
-        self.th = RecordSensors(device=self.device)
-        all_signals.captured_rgb.connect(self.setRGBImage)
-        all_signals.captured_depth.connect(self.setDepthImage)
-        all_signals.captured_ir.connect(self.setIRImage)
-        all_signals.captured_time.connect(self.setTime)
-        all_signals.captured_acc_data.connect(self.setAccData)
-        all_signals.captured_gyro_data.connect(self.setGyroData)
-        all_signals.captured_fps.connect(self.setFps)
-        all_signals.captured_audio.connect(self.setAudioData)
-            
-        self.is_device = True
-        self.is_viewer = True
+        self.main_layout.addWidget(self.frame_ir, 0, 0)
+        self.main_layout.addWidget(self.frame_depth, 0, 1)
+        self.main_layout.addWidget(self.frame_rgb, 1, 0)
+        self.main_layout.addWidget(self.frame_subdata, 1, 1)
+
+        self.setAcceptDrops(True)
+        self.setLayout(self.main_layout)
+
+        self.is_play = True
         self.is_record = True
-        self.btn_open.clicked.connect(self.open_device)
-        self.btn_viewer.clicked.connect(self.streaming)
-        self.btn_record.clicked.connect(self.recording)
-        self.btn_viewer.setEnabled(False)
+        self.setLayout(self.main_layout)
+
+        # UI option signals 
+        all_signals.option_signals.save_filepath.connect(self.set_base_path)
+        all_signals.option_signals.sidebar_toggle.connect(self.set_config)
+        all_signals.option_signals.device_option.connect(self.select_option)
+        all_signals.option_signals.camera_option.connect(self.set_config)
+        all_signals.option_signals.clear_frame.connect(self.clear_frame)
         
-        self.target = None
-        self.grid_layout.addWidget(self.frame_rgb, 0, 0)
-        self.grid_layout.addWidget(self.frame_depth, 0, 1)
-        self.grid_layout.addWidget(self.frame_ir, 1, 0)
-        self.grid_layout.addWidget(self.frame_subdata, 1, 1)
-        self.grid_layout.addLayout(layout_btn, 2, 0, 1, 2)
+        # Recording signals
+        all_signals.record_signals.rgb_image.connect(self.set_rgb_image)
+        all_signals.record_signals.depth_image.connect(self.set_depth_image)
+        all_signals.record_signals.ir_image.connect(self.set_ir_image)
+        all_signals.record_signals.record_time.connect(self.set_time)
+        all_signals.record_signals.video_fps.connect(self.set_fps)
+        all_signals.record_signals.imu_acc_data.connect(self.set_acc_data)
+        all_signals.record_signals.imu_gyro_data.connect(self.set_gyro_data)
+        all_signals.record_signals.audio_data.connect(self.set_audio_data)
+
+    def select_option(self, value):
+        if value == "viewer":
+            self.streaming()
+        else:
+            self.recording()
 
-        self.setAcceptDrops(True)
-        self.setLayout(self.grid_layout)
+    def streaming(self) -> None:
+        self.is_record = False
+        self.play()
+
+    def recording(self) -> None:
+        self.is_record = True
+        self.play()
+
+    def play(self) -> None:
+        if self.is_play:
+            self.set_filename()
+            for k, v in self.emit_configs["color"].items():
+                setattr(self.config, k, v)
+                
+            self.device = start_device(
+                config=self.config, 
+                record=self.is_record, 
+                record_filepath=self.filename_video
+            )
+            setattr(self.config, "depth_mode", self.emit_configs["depth_mode"])
+            for k, v in self.emit_configs["color_option"].items():
+                k4a_device_set_color_control(
+                    self.device._handle, color_command_dict[k], K4A_COLOR_CONTROL_MODE_MANUAL, ctypes.c_int32(int(v))
+                )
+
+            self.viewer = RecordSensors(device=self.device)
+            self.viewer.start_audio()
+            self.viewer.timer.start()
+            self.is_play = False
+        else:
+            self.viewer.timer.stop()
+            self.viewer.stop_audio()
+            self.viewer.quit()
+            self.device.close()
+            self.is_play = True
+
+            if self.is_record:
+                wait_dialog = CustomProgressBarDialog(msec=500)
+                wait_dialog.show()
+
+    def set_filename(self) -> None:
+        if self.base_path is None:
+            self.base_path = os.path.join(Path.home(), "Videos")
+
+        filename = datetime.datetime.now()
+        filename = filename.strftime("%Y_%m_%d_%H_%M_%S")
+
+        self.filename_video = os.path.join(self.base_path, f"{filename}.mkv")
+        if sys.flags.debug:
+            print(self.base_path, self.filename_video)
+
+    @Slot(dict)
+    def set_config(self, value: dict) -> None:
+        self.emit_configs = value
+
+    @Slot(str)
+    def set_base_path(self, value: str) -> None:
+        self.base_path = value
 
     def eventFilter(self, watched, event):
         if event.type() == QEvent.MouseButtonPress:
             self.mousePressEvent(event)
         elif event.type() == QEvent.MouseMove:
             self.mouseMoveEvent(event)
         elif event.type() == QEvent.MouseButtonRelease:
             self.mouseReleaseEvent(event)
         return super().eventFilter(watched, event)
-    
+
     def get_index(self, pos):
-        for i in range(self.grid_layout.count()):
-            if self.grid_layout.itemAt(i).geometry().contains(pos) and i != self.target:
+        for i in range(self.main_layout.count()):
+            if self.main_layout.itemAt(i).geometry().contains(pos) and i != self.target:
                 return i
 
     def mousePressEvent(self, event):
         if event.button() == Qt.LeftButton:
             self.target = self.get_index(event.windowPos().toPoint())
         else:
             self.target = None
 
     def mouseMoveEvent(self, event):
         if event.buttons() & Qt.LeftButton and self.target is not None:
-            drag = QDrag(self.grid_layout.itemAt(self.target).widget())
-            pix = self.grid_layout.itemAt(self.target).widget().grab()
+            drag = QDrag(self.main_layout.itemAt(self.target).widget())
+            pix = self.main_layout.itemAt(self.target).widget().grab()
             mimedata = QMimeData()
             mimedata.setImageData(pix)
             drag.setMimeData(mimedata)
             drag.setPixmap(pix)
             drag.exec(Qt.DropAction.CopyAction | Qt.DropAction.MoveAction)
 
     def mouseReleaseEvent(self, event):
@@ -176,191 +209,81 @@
     def dropEvent(self, event):
         if not event.source().geometry().contains(event.pos()):
             source = self.get_index(event.pos())
             if source is None:
                 return
 
             i, j = max(self.target, source), min(self.target, source)
-            p1, p2 = self.grid_layout.getItemPosition(i), self.grid_layout.getItemPosition(j)
-
-            self.grid_layout.addItem(self.grid_layout.takeAt(i), *p2)
-            self.grid_layout.addItem(self.grid_layout.takeAt(j), *p1)
+            p1, p2 = self.main_layout.getItemPosition(i), self.main_layout.getItemPosition(j)
 
+            self.main_layout.addItem(self.main_layout.takeAt(i), *p2)
+            self.main_layout.addItem(self.main_layout.takeAt(j), *p1)
             event.accept()
-        
-    def check_device(self) -> bool:
-        try:
-            self.config = Configuration()     
-            initialize_libraries()
-            _device = start_device(config=self.config)
-            _device.close()
-        except:
-            modal = QDialog()
-            layout_modal = QVBoxLayout()
-            e_message = Label(
-                "<b>카메라 연결에 문제가 있습니다. <br> 연결을 재시도해주세요.</b>", 
-                "Arial", 20, Qt.AlignmentFlag.AlignCenter
-            )
-            layout_modal.addWidget(e_message)
-            modal.setLayout(layout_modal)
-            modal.setWindowTitle("Error Message")
-            modal.resize(400, 200)
-            modal.exec()
-
-    def open_device(self) -> None:
-        if self.is_device is True:
-            self.check_device()
-            self.is_device = False
-            self.btn_open.setText("Device close")
-        else:
-            self.frame_rgb.frame.setText("RGB Frame")
-            self.frame_depth.frame.setText("Depth Frame")
-            self.frame_ir.frame.setText("IR Frame")
-            self.is_device = True
-            self.btn_open.setText("Device open")
-            self.device = None
-    
-    # TODO Streaming 이랑 Recording 겹치는 코드가 많음.
-    def streaming(self) -> None:
-        if self.is_viewer:
-            self.set_filename()
-
-            for k, v in self.emit_configs["color"].items():
-                setattr(self.config, k, v)
-            setattr(self.config, "depth_mode", self.emit_configs["depth_mode"])
-            self.device = start_device(config=self.config, record=False)   
-
-            for k, v in self.emit_configs["color_option"].items():
-                k4a_device_set_color_control(
-                    self.device._handle,
-                    color_command_dict[k],
-                    K4A_COLOR_CONTROL_MODE_MANUAL,
-                    ctypes.c_int32(int(v))
-                )
-
-            self.th.device = self.device
-            self.th.audio_file = self.filename_audio
 
-            self.btn_record.setEnabled(False)
-            self.btn_open.setEnabled(False)
-            self.btn_viewer.setText("■")
-            self.th.is_run = True
-            self.is_viewer = False
-            self.th.start()
-        else:
-            self.btn_record.setEnabled(True)
-            self.btn_open.setEnabled(True)
-            self.btn_viewer.setText("▶")
-            self.th.is_run = False
-            self.is_viewer = True
-            self.device.close()
-            self.th.quit()
-            time.sleep(1)   
-        
-    def recording(self) -> None:
-        if self.is_record:
-            self.set_filename()
-
-            for k, v in self.emit_configs["color"].items():
-                setattr(self.config, k, v)
-            setattr(self.config, "depth_mode", self.emit_configs["depth_mode"])
-            self.device = start_device(
-                config=self.config, 
-                record_filepath=self.filename_video,
-                record=True
-            )   
-
-            for k, v in self.emit_configs["color_option"].items():
-                k4a_device_set_color_control(
-                    self.device._handle,
-                    color_command_dict[k],
-                    K4A_COLOR_CONTROL_MODE_MANUAL,
-                    ctypes.c_int32(int(v))
-                )
-            
-            self.th.device = self.device
-            self.th.audio_record = True
-            self.th.audio_file = self.filename_audio
-
-            # self.btn_viewer.setEnabled(False)
-            self.btn_open.setEnabled(False)
-            self.btn_record.setText("■")
-            self.th.is_run = True
-            self.is_record = False
-            self.th.start()
-        else:
-            # self.btn_viewer.setEnabled(True)
-            self.btn_open.setEnabled(True)
-            self.btn_record.setText("▶")
-            self.th.is_run = False
-            self.is_record = True
-            self.device.close()
-            self.th.quit()
-            time.sleep(1)
-
-    def set_filename(self) -> None:
-        if self.base_path is None:
-            self.base_path = os.path.join(Path.home(), "Videos")
-
-        filename = datetime.datetime.now()
-        filename = filename.strftime("%Y_%m_%d_%H_%M_%S")
-
-        self.filename_video = os.path.join(self.base_path, f"{filename}.mkv")
-        self.filename_audio = os.path.join(self.base_path, f"{filename}.mp3")
-        if sys.flags.debug:
-            print(self.base_path, self.filename_video)
-
-    @Slot(dict)
-    def setConfig(self, value: dict) -> None:
-        self.emit_configs = value
-
-    @Slot(str)
-    def setBasePath(self, value: str) -> None:
-        self.base_path = value
-        
     @Slot(QImage)
-    def setRGBImage(self, image: QImage) -> None:
-        self.frame_rgb.frame.setPixmap(QPixmap.fromImage(image))
-    
+    def set_rgb_image(self, image: QImage) -> None:
+        w, h = self.frame_rgb.label_image.width(), self.frame_rgb.label_image.height()
+        image = image.scaled(w-5, h-5, Qt.KeepAspectRatio)
+        self.frame_rgb.label_image.setPixmap(QPixmap.fromImage(image))
+
     @Slot(QImage)
-    def setDepthImage(self, image: QImage) -> None:
-        self.frame_depth.frame.setPixmap(QPixmap.fromImage(image))
-        
+    def set_depth_image(self, image: QImage) -> None:
+        w, h = self.frame_depth.label_image.width(), self.frame_depth.label_image.height()
+        image = image.scaled(w-5, h-5, Qt.KeepAspectRatio)
+        self.frame_depth.label_image.setPixmap(QPixmap.fromImage(image))
+
     @Slot(QImage)
-    def setIRImage(self, image: QImage) -> None:
-        self.frame_ir.frame.setPixmap(QPixmap.fromImage(image))
+    def set_ir_image(self, image: QImage) -> None:
+        w, h = self.frame_ir.label_image.width(), self.frame_ir.label_image.height()
+        image = image.scaled(w-5, h-5, Qt.KeepAspectRatio)
+        self.frame_ir.label_image.setPixmap(QPixmap.fromImage(image))
 
     @Slot(float)
-    def setTime(self, time) -> None:
-        self.imu_senser.label_time.setText("Time(s) : %.3f" %time)
+    def set_time(self, time) -> None:
+        self.imu_senser.label_time.setText("Time(s) : %.3f" % time)
 
-    @Slot(float)
-    def setFps(self, value) -> None:
-        self.imu_senser.label_fps.setText("FPS : %.2f" %value)
+    @Slot(int)
+    def set_fps(self, value) -> None:
+        self.imu_senser.label_fps.setText("FPS : %d" % value)
 
     @Slot(list)
-    def setAccData(self, values) -> None:
-        self.imu_senser.acc_x.setText("X : %.5f" %values[0])
-        self.imu_senser.acc_y.setText("Y : %.5f" %values[1])
-        self.imu_senser.acc_z.setText("Z : %.5f" %values[2])
+    def set_acc_data(self, values) -> None:
+        self.imu_senser.label_acc_x.setText("X : %.5f" % values[0])
+        self.imu_senser.label_acc_y.setText("Y : %.5f" % values[1])
+        self.imu_senser.label_acc_z.setText("Z : %.5f" % values[2])
 
     @Slot(float)
-    def setGyroData(self, values) -> None:
-        self.imu_senser.gyro_x.setText("X : %.5f" %values[0])
-        self.imu_senser.gyro_y.setText("Y : %.5f" %values[1])
-        self.imu_senser.gyro_z.setText("Z : %.5f" %values[2])
+    def set_gyro_data(self, values) -> None:
+        # self.imu_senser.label_gyro_x.setText("X : %.5f" % values[0])
+        self.imu_senser.label_gyro_x.setText(f"X : {values[0]:.5f}")
+        self.imu_senser.label_gyro_y.setText("Y : %.5f" % values[1])
+        self.imu_senser.label_gyro_z.setText("Z : %.5f" % values[2])
 
     @Slot(list)
-    def setAudioData(self, values) -> None:
+    def set_audio_data(self, values) -> None:
         start = 0
-        if (values[1] < SAMPLE_COUNT):
+        if values[1] < SAMPLE_COUNT:
             start = SAMPLE_COUNT - values[1]
             for s in range(start):
                 self.buffer[s].setY(self.buffer[s + values[1]].y())
 
         data_index = 0
         for s in range(start, SAMPLE_COUNT):
             value = (ord(values[0][data_index]) - 128) / 128
             self.buffer[s].setY(value)
             data_index = data_index + RESOLUTION
-        
-        self.audio_sensor.series.replace(self.buffer)
+
+        self.audio_sensor.series.replace(self.buffer)
+
+    def clear_frame(self):
+        self.frame_rgb.label_image.clear()
+        self.frame_depth.label_image.clear()
+        self.frame_ir.label_image.clear()
+        self.imu_senser.label_time.setText("Time(s) : ")
+        self.imu_senser.label_fps.setText("FPS : ")
+        self.imu_senser.label_acc_x.setText("X : ")
+        self.imu_senser.label_acc_y.setText("Y : ")
+        self.imu_senser.label_acc_z.setText("Z : ")
+        self.imu_senser.label_gyro_x.setText("X : ")
+        self.imu_senser.label_gyro_y.setText("Y : ")
+        self.imu_senser.label_gyro_z.setText("Z : ")
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pykinect_recorder-0.9.1/pykinect_recorder/renderer/public/kinect-sensor.ico` & `pykinect_recorder-0.9.2/pykinect_recorder/renderer/public/kinect-sensor.ico`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.1/pyproject.toml` & `pykinect_recorder-0.9.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "pykinect-recorder"
-version = "v0.9.1"
+version = "0.9.2"
 description = ""
 license = "MIT"
 authors = [
     "Kyung-Su Kang <unerue@me.com>",
-    "Young-Il Kim <qhdrmfdl123@gmail.com>"
+    "Young-Il Kim <qhdrmfdl123@gmail.com>",
+    "Yeo-Reum Lee <leeyeoreum01@gmail.com>",
 ]
 readme = ["README.md", "LICENSE"]
 packages = [{include = "pykinect_recorder"}]
 
 repository = "https://github.com/unerue/pykinect-recorder"
 keywords = ["azure", "kinect", "deep-learning", "computer-vision"]
 
@@ -18,31 +19,39 @@
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.9.1"
 pyside6 = "^6.4.2"
 open3d = "^0.17.0"
 pyqtdarktheme = "^2.1.0"
 opencv-python = "^4.7.0.72"
-termcolor = "^2.2.0"
-click = "^8.1.3"
-pyqtgraph = "^0.13.2"
 matplotlib = "^3.7.1"
 sounddevice = "^0.4.6"
 soundfile = "^0.12.1"
 scikit-learn = "^1.2.2"
 qtawesome = "^1.2.3"
+pandas = "^2.0.2"
+superqt = "^0.4.1"
+
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 flake8 = "^6.0.0"
 black = "^23.1.0"
 isort = "^5.12.0"
 mypy = "^1.1.1"
 pyinstaller = "^5.10.1"
 
+[tool.poetry.group.docs.dependencies]
+sphinx = "^4.5.0"
+sphinx-rtd-theme = "^1.0.0"
+readthedocs-sphinx-search = "^0.3.1"
+pyyaml = "^6.0"
+addict = "^2.4.0"
+tqdm = "^4.65.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
```

