# Comparing `tmp/pykinect_recorder-0.9.2.tar.gz` & `tmp/pykinect_recorder-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykinect_recorder-0.9.2.tar", max compression
+gzip compressed data, was "pykinect_recorder-0.9.3.tar", max compression
```

## Comparing `pykinect_recorder-0.9.2.tar` & `pykinect_recorder-0.9.3.tar`

### file list

```diff
@@ -1,65 +1,64 @@
--rw-r--r--   0        0        0     1086 2023-07-16 11:33:01.031615 pykinect_recorder-0.9.2/LICENSE
--rw-r--r--   0        0        0       46 2023-07-16 11:32:31.458067 pykinect_recorder-0.9.2/pykinect_recorder/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 11:33:01.055130 pykinect_recorder-0.9.2/pykinect_recorder/cli/__init__.py
--rw-r--r--   0        0        0      592 2023-07-16 11:33:01.056126 pykinect_recorder-0.9.2/pykinect_recorder/cli/command.py
--rw-r--r--   0        0        0     3209 2023-07-16 11:33:01.057126 pykinect_recorder-0.9.2/pykinect_recorder/dev/record_sensors.py
--rw-r--r--   0        0        0     3626 2023-07-16 11:33:01.058127 pykinect_recorder-0.9.2/pykinect_recorder/main_window.py
--rw-r--r--   0        0        0      414 2023-07-16 11:33:01.058127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/__init__.py
--rw-r--r--   0        0        0      266 2023-07-16 11:33:01.059128 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/__init__.py
--rw-r--r--   0        0        0    90759 2023-07-16 11:33:01.060127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/_k4a.py
--rw-r--r--   0        0        0    19864 2023-07-16 11:33:01.061127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/_k4atypes.py
--rw-r--r--   0        0        0     8322 2023-07-16 11:33:01.062127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/calibration.py
--rw-r--r--   0        0        0     4097 2023-07-16 11:33:01.062127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/capture.py
--rw-r--r--   0        0        0     4004 2023-07-16 11:33:01.063127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/configuration.py
--rw-r--r--   0        0        0     6625 2023-07-16 11:33:01.064127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/device.py
--rw-r--r--   0        0        0     4774 2023-07-16 11:33:01.065128 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/image.py
--rw-r--r--   0        0        0     1575 2023-07-16 11:33:01.065128 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/imu_sample.py
--rw-r--r--   0        0        0     4386 2023-07-16 11:33:01.066128 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/transformation.py
--rw-r--r--   0        0        0      164 2023-07-16 11:33:01.067127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/__init__.py
--rw-r--r--   0        0        0    18158 2023-07-16 11:33:01.067127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/_k4abt.py
--rw-r--r--   0        0        0    11712 2023-07-16 11:33:01.068127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/_k4abtTypes.py
--rw-r--r--   0        0        0     1146 2023-07-16 11:33:01.069126 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/body.py
--rw-r--r--   0        0        0     2948 2023-07-16 11:33:01.069126 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/body2d.py
--rw-r--r--   0        0        0     4468 2023-07-16 11:33:01.070125 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/frame.py
--rw-r--r--   0        0        0     1617 2023-07-16 11:33:01.071126 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/joint.py
--rw-r--r--   0        0        0     1228 2023-07-16 11:33:01.071126 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/joint2d.py
--rw-r--r--   0        0        0     3079 2023-07-16 11:33:01.072126 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/tracker.py
--rw-r--r--   0        0        0      149 2023-07-16 11:33:01.072126 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/__init__.py
--rw-r--r--   0        0        0    20837 2023-07-16 11:33:01.073161 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/_k4arecord.py
--rw-r--r--   0        0        0     2344 2023-07-16 11:33:01.074127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/_k4arecordTypes.py
--rw-r--r--   0        0        0      928 2023-07-16 11:33:01.074127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/datablock.py
--rw-r--r--   0        0        0     5984 2023-07-16 11:33:01.075127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/playback.py
--rw-r--r--   0        0        0     2182 2023-07-16 11:33:01.075127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/record.py
--rw-r--r--   0        0        0     2153 2023-07-16 11:33:01.076127 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/record_configuration.py
--rw-r--r--   0        0        0     2049 2023-07-16 11:33:01.077125 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/pykinect.py
--rw-r--r--   0        0        0     5587 2023-07-16 11:33:01.077125 pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/utils.py
--rw-r--r--   0        0        0        0 2023-07-16 11:33:01.078126 pykinect_recorder-0.9.2/pykinect_recorder/pyrealsense/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 11:33:01.078126 pykinect_recorder-0.9.2/pykinect_recorder/pyzenmuse/__init__.py
--rw-r--r--   0        0        0       56 2023-07-16 11:32:31.495067 pykinect_recorder-0.9.2/pykinect_recorder/renderer/__init__.py
--rw-r--r--   0        0        0     9847 2023-07-16 11:33:01.079126 pykinect_recorder-0.9.2/pykinect_recorder/renderer/common_widgets.py
--rw-r--r--   0        0        0       17 2023-07-16 11:32:31.496068 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/__init__.py
--rw-r--r--   0        0        0     2824 2023-07-16 11:33:01.080178 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/playback_sensors.py
--rw-r--r--   0        0        0     3348 2023-07-16 11:33:01.081127 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/record_sensors.py
--rw-r--r--   0        0        0     1351 2023-07-16 11:33:01.082127 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/sidebar_control.py
--rw-r--r--   0        0        0     6585 2023-07-16 11:33:01.083126 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/sidebar_explorer.py
--rw-r--r--   0        0        0     3795 2023-07-16 11:33:01.083126 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/sidebar_menu.py
--rw-r--r--   0        0        0    27968 2023-07-16 11:33:01.084128 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/sidebar_record_control.py
--rw-r--r--   0        0        0      135 2023-07-16 11:32:31.503069 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/sidebar_solutions.py
--rw-r--r--   0        0        0     2201 2023-07-16 11:33:01.085130 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/statusbar.py
--rw-r--r--   0        0        0     4680 2023-07-16 11:33:01.085130 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/topbar.py
--rw-r--r--   0        0        0      797 2023-07-16 11:33:01.086127 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_3dsensors.py
--rw-r--r--   0        0        0     1964 2023-07-16 11:33:01.087127 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_audio.py
--rw-r--r--   0        0        0     1511 2023-07-16 11:33:01.087127 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_control.py
--rw-r--r--   0        0        0     2980 2023-07-16 11:33:01.088127 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_imu_sensors.py
--rw-r--r--   0        0        0    12170 2023-07-16 11:33:01.089128 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_playback.py
--rw-r--r--   0        0        0    11462 2023-07-16 11:33:01.090125 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_sensors.py
--rw-r--r--   0        0        0      235 2023-07-16 11:32:31.508067 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_solution.py
--rw-r--r--   0        0        0    12459 2023-07-16 11:33:01.090125 pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_video_clipping.py
--rw-r--r--   0        0        0     1802 2023-07-16 11:33:01.091125 pykinect_recorder-0.9.2/pykinect_recorder/renderer/logger.py
--rw-r--r--   0        0        0    48895 2023-03-21 13:06:28.698628 pykinect_recorder-0.9.2/pykinect_recorder/renderer/public/kinect-sensor.ico
--rw-r--r--   0        0        0     1646 2023-07-16 11:33:01.092126 pykinect_recorder-0.9.2/pykinect_recorder/renderer/signals.py
--rw-r--r--   0        0        0     2943 2023-07-16 11:33:01.092126 pykinect_recorder-0.9.2/pykinect_recorder/renderer/split_data.py
--rw-r--r--   0        0        0     2483 2023-07-16 11:33:01.093126 pykinect_recorder-0.9.2/pykinect_recorder/renderer/synology_utils.py
--rw-r--r--   0        0        0     1561 2023-07-16 11:34:44.967052 pykinect_recorder-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2436 2023-07-16 11:33:01.033614 pykinect_recorder-0.9.2/README.md
--rw-r--r--   0        0        0     4491 1970-01-01 00:00:00.000000 pykinect_recorder-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-07-16 11:33:01.031615 pykinect_recorder-0.9.3/LICENSE
+-rw-r--r--   0        0        0       46 2023-07-16 11:32:31.458067 pykinect_recorder-0.9.3/pykinect_recorder/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:33:01.055130 pykinect_recorder-0.9.3/pykinect_recorder/cli/__init__.py
+-rw-r--r--   0        0        0      595 2023-07-16 12:22:34.306948 pykinect_recorder-0.9.3/pykinect_recorder/cli/command.py
+-rw-r--r--   0        0        0     3626 2023-07-16 11:33:01.058127 pykinect_recorder-0.9.3/pykinect_recorder/main_window.py
+-rw-r--r--   0        0        0      414 2023-07-16 11:33:01.058127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/__init__.py
+-rw-r--r--   0        0        0      266 2023-07-16 11:33:01.059128 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/__init__.py
+-rw-r--r--   0        0        0    90759 2023-07-16 11:33:01.060127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/_k4a.py
+-rw-r--r--   0        0        0    19864 2023-07-16 11:33:01.061127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/_k4atypes.py
+-rw-r--r--   0        0        0     8322 2023-07-16 11:33:01.062127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/calibration.py
+-rw-r--r--   0        0        0     4097 2023-07-16 11:33:01.062127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/capture.py
+-rw-r--r--   0        0        0     4004 2023-07-16 11:33:01.063127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/configuration.py
+-rw-r--r--   0        0        0     6625 2023-07-16 11:33:01.064127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/device.py
+-rw-r--r--   0        0        0     4774 2023-07-16 11:33:01.065128 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/image.py
+-rw-r--r--   0        0        0     1575 2023-07-16 11:33:01.065128 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/imu_sample.py
+-rw-r--r--   0        0        0     4386 2023-07-16 11:33:01.066128 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/transformation.py
+-rw-r--r--   0        0        0      164 2023-07-16 11:33:01.067127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/__init__.py
+-rw-r--r--   0        0        0    18158 2023-07-16 11:33:01.067127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/_k4abt.py
+-rw-r--r--   0        0        0    11712 2023-07-16 11:33:01.068127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/_k4abtTypes.py
+-rw-r--r--   0        0        0     1146 2023-07-16 11:33:01.069126 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/body.py
+-rw-r--r--   0        0        0     2948 2023-07-16 11:33:01.069126 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/body2d.py
+-rw-r--r--   0        0        0     4468 2023-07-16 11:33:01.070125 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/frame.py
+-rw-r--r--   0        0        0     1617 2023-07-16 11:33:01.071126 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/joint.py
+-rw-r--r--   0        0        0     1228 2023-07-16 11:33:01.071126 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/joint2d.py
+-rw-r--r--   0        0        0     3079 2023-07-16 11:33:01.072126 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/tracker.py
+-rw-r--r--   0        0        0      149 2023-07-16 11:33:01.072126 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/__init__.py
+-rw-r--r--   0        0        0    20837 2023-07-16 11:33:01.073161 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/_k4arecord.py
+-rw-r--r--   0        0        0     2344 2023-07-16 11:33:01.074127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/_k4arecordTypes.py
+-rw-r--r--   0        0        0      928 2023-07-16 11:33:01.074127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/datablock.py
+-rw-r--r--   0        0        0     5984 2023-07-16 11:33:01.075127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/playback.py
+-rw-r--r--   0        0        0     2182 2023-07-16 11:33:01.075127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/record.py
+-rw-r--r--   0        0        0     2153 2023-07-16 11:33:01.076127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/record_configuration.py
+-rw-r--r--   0        0        0     2049 2023-07-16 11:33:01.077125 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/pykinect.py
+-rw-r--r--   0        0        0     5587 2023-07-16 11:33:01.077125 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/utils.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:33:01.078126 pykinect_recorder-0.9.3/pykinect_recorder/pyrealsense/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:33:01.078126 pykinect_recorder-0.9.3/pykinect_recorder/pyzenmuse/__init__.py
+-rw-r--r--   0        0        0       56 2023-07-16 11:32:31.495067 pykinect_recorder-0.9.3/pykinect_recorder/renderer/__init__.py
+-rw-r--r--   0        0        0     9847 2023-07-16 11:33:01.079126 pykinect_recorder-0.9.3/pykinect_recorder/renderer/common_widgets.py
+-rw-r--r--   0        0        0       17 2023-07-16 11:32:31.496068 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/__init__.py
+-rw-r--r--   0        0        0     2824 2023-07-16 11:33:01.080178 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/playback_sensors.py
+-rw-r--r--   0        0        0     3348 2023-07-16 11:33:01.081127 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/record_sensors.py
+-rw-r--r--   0        0        0     1351 2023-07-16 11:33:01.082127 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_control.py
+-rw-r--r--   0        0        0     6585 2023-07-16 11:33:01.083126 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_explorer.py
+-rw-r--r--   0        0        0     3795 2023-07-16 11:33:01.083126 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_menu.py
+-rw-r--r--   0        0        0    27968 2023-07-16 11:33:01.084128 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_record_control.py
+-rw-r--r--   0        0        0      135 2023-07-16 11:32:31.503069 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_solutions.py
+-rw-r--r--   0        0        0     2201 2023-07-16 11:33:01.085130 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/statusbar.py
+-rw-r--r--   0        0        0     4680 2023-07-16 11:33:01.085130 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/topbar.py
+-rw-r--r--   0        0        0      797 2023-07-16 11:33:01.086127 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_3dsensors.py
+-rw-r--r--   0        0        0     1964 2023-07-16 11:33:01.087127 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_audio.py
+-rw-r--r--   0        0        0     1511 2023-07-16 11:33:01.087127 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_control.py
+-rw-r--r--   0        0        0     2980 2023-07-16 11:33:01.088127 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_imu_sensors.py
+-rw-r--r--   0        0        0    12170 2023-07-16 11:33:01.089128 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_playback.py
+-rw-r--r--   0        0        0    11462 2023-07-16 11:33:01.090125 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_sensors.py
+-rw-r--r--   0        0        0      235 2023-07-16 11:32:31.508067 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_solution.py
+-rw-r--r--   0        0        0    12459 2023-07-16 11:33:01.090125 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_video_clipping.py
+-rw-r--r--   0        0        0     1802 2023-07-16 11:33:01.091125 pykinect_recorder-0.9.3/pykinect_recorder/renderer/logger.py
+-rw-r--r--   0        0        0    48895 2023-03-21 13:06:28.698628 pykinect_recorder-0.9.3/pykinect_recorder/renderer/public/kinect-sensor.ico
+-rw-r--r--   0        0        0     1646 2023-07-16 11:33:01.092126 pykinect_recorder-0.9.3/pykinect_recorder/renderer/signals.py
+-rw-r--r--   0        0        0     2943 2023-07-16 11:33:01.092126 pykinect_recorder-0.9.3/pykinect_recorder/renderer/split_data.py
+-rw-r--r--   0        0        0     2483 2023-07-16 11:33:01.093126 pykinect_recorder-0.9.3/pykinect_recorder/renderer/synology_utils.py
+-rw-r--r--   0        0        0     1554 2023-07-16 12:22:34.307948 pykinect_recorder-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2493 2023-07-16 12:22:34.305946 pykinect_recorder-0.9.3/README.md
+-rw-r--r--   0        0        0     4544 1970-01-01 00:00:00.000000 pykinect_recorder-0.9.3/PKG-INFO
```

### Comparing `pykinect_recorder-0.9.2/LICENSE` & `pykinect_recorder-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/cli/command.py` & `pykinect_recorder-0.9.3/pykinect_recorder/cli/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import click
-from pykinect_recorder.renderer import MainWindow
+from pykinect_recorder.main_window import MainWindow
 import qdarktheme
 from PySide6.QtWidgets import QApplication
 
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
```

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/dev/record_sensors.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/record_sensors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import cv2
+import time
 
-from PySide6.QtCore import Qt, QTimer, QThread
+import cv2
+from PySide6.QtCore import Qt, QThread, QTimer
 from PySide6.QtGui import QImage
 from PySide6.QtMultimedia import (
     QAudioFormat,
     QAudioSource,
     QMediaDevices,
 )
 
@@ -16,71 +17,72 @@
 RESOLUTION = 4
 
 
 class RecordSensors(QThread):
     def __init__(self, device: Device) -> None:
         super().__init__()
         self.device = device
-        self.total_time = 0
         self.audio_input = None
         self.input_devices = QMediaDevices.audioInputs()
 
         dict_fps = {0: "5", 1: "15", 2: "30"}
         self.device_fps = int(dict_fps[self.device.configuration.camera_fps])
-        self.timer = QTimer()
-        self.timer.setInterval(1)
-        self.timer.timeout.connect(self.update_next_frame)
-
-    def start_audio(self):
-        self.ready_audio()
-        self.io_device = self.audio_input.start()
-    
-    def exit_audio(self):
-        self.audio_input.stop()
-        self.io_device = None
 
-    def ready_audio(self) -> None:
-        format_audio = QAudioFormat()
-        format_audio.setSampleRate(44200)
-        format_audio.setChannelCount(3)
-        format_audio.setSampleFormat(QAudioFormat.SampleFormat.UInt8)
-        self.audio_input = QAudioSource(self.input_devices[0], format_audio)
+        self.timer = QTimer()
+        self.timer.setInterval(1000 / self.device_fps)
+        self.timer.timeout.connect(self.update_next_frame)   
 
     def update_next_frame(self):
-        current_frame = self.device.update(1000//self.device_fps)
+        current_frame = self.device.update()
+        current_imu_data = self.device.update_imu()
         current_rgb_frame = current_frame.get_color_image()
-        current_depth_frame = current_frame.get_depth_image()
+        current_depth_frame = current_frame.get_colored_depth_image()
         current_ir_frame = current_frame.get_ir_image()
 
         if current_rgb_frame[0]:
             rgb_frame = cv2.cvtColor(current_rgb_frame[1], cv2.COLOR_BGR2RGB)
             h, w, ch = rgb_frame.shape
-            rgb_frame = QImage(rgb_frame, w, h, ch * w, QImage.Format_RGB888)
-            all_signals.captured_rgb.emit(rgb_frame)
+            rgb_frame = QImage(rgb_frame, w, h, ch * w, QImage.Format_RGB888)    
+            all_signals.record_signals.rgb_image.emit(rgb_frame)            
 
         if current_depth_frame[0]:
             depth_frame = colorize(current_depth_frame[1], (None, 5000), cv2.COLORMAP_HSV)
             h, w, ch = depth_frame.shape
             depth_frame = QImage(depth_frame, w, h, w * ch, QImage.Format_RGB888)
-            all_signals.captured_depth.emit(depth_frame)
+            all_signals.record_signals.depth_image.emit(depth_frame)
 
         if current_ir_frame[0]:
             ir_frame = colorize(current_ir_frame[1], (None, 5000), cv2.COLORMAP_BONE)
             h, w, ch = ir_frame.shape
             ir_frame = QImage(ir_frame, w, h, w * ch, QImage.Format_RGB888)
-            all_signals.captured_ir.emit(ir_frame)
+            all_signals.record_signals.ir_image.emit(ir_frame)
 
-        current_imu_data = self.device.update_imu()
-        self.total_time += current_imu_data.acc_time
+        end_time = time.time()
         acc_data = current_imu_data.acc
         gyro_data = current_imu_data.gyro
 
-        all_signals.captured_fps.emit(self.device_fps)
-        all_signals.captured_time.emit(self.total_time / 1e7)
-        all_signals.captured_acc_data.emit(acc_data)
-        all_signals.captured_gyro_data.emit(gyro_data)
-        # Test signal structure
-        all_signals.imu_signals.imu_gyro_data.emit(gyro_data)
-
+        # audio
         data = self.io_device.readAll()
         available_samples = data.size() // RESOLUTION
-        all_signals.captured_audio.emit([data, available_samples])
+
+        all_signals.record_signals.video_fps.emit(int(self.device_fps))
+        all_signals.record_signals.record_time.emit((end_time-self.start_time))
+        all_signals.record_signals.imu_acc_data.emit(acc_data)
+        all_signals.record_signals.imu_gyro_data.emit(gyro_data)
+        all_signals.record_signals.audio_data.emit([data, available_samples])
+
+    def start_audio(self):
+        self.ready_audio()
+        self.io_device = self.audio_input.start()
+        self.start_time = time.time()
+    
+    def stop_audio(self):
+        self.audio_input.stop()
+        self.io_device = None
+
+    def ready_audio(self) -> None:
+        # https://github.com/ShadarRim/opencvpythonvideoplayer/blob/master/player.py
+        format_audio = QAudioFormat()
+        format_audio.setSampleRate(44200)
+        format_audio.setChannelCount(3)
+        format_audio.setSampleFormat(QAudioFormat.SampleFormat.UInt8)
+        self.audio_input = QAudioSource(self.input_devices[0], format_audio)
```

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/main_window.py` & `pykinect_recorder-0.9.3/pykinect_recorder/main_window.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/_k4a.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/_k4a.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/_k4atypes.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/_k4atypes.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/calibration.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/calibration.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/capture.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/capture.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/configuration.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/configuration.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/device.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/device.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/image.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/image.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/imu_sample.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/imu_sample.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4a/transformation.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/transformation.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/_k4abt.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/_k4abt.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/_k4abtTypes.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/_k4abtTypes.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/body.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/body.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/body2d.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/body2d.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/frame.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/frame.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/joint.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/joint.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/joint2d.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/joint2d.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4abt/tracker.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/tracker.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/_k4arecord.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/_k4arecord.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/_k4arecordTypes.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/_k4arecordTypes.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/datablock.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/datablock.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/playback.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/playback.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/record.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/record.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/k4arecord/record_configuration.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/record_configuration.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/pykinect.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/pykinect.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/pyk4a/utils.py` & `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/utils.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/common_widgets.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/common_widgets.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/playback_sensors.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/playback_sensors.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/sidebar_control.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_control.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/sidebar_explorer.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_explorer.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/sidebar_menu.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_menu.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/sidebar_record_control.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_record_control.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/statusbar.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/statusbar.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/topbar.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/topbar.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_3dsensors.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_3dsensors.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_audio.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_audio.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_control.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_control.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_imu_sensors.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_imu_sensors.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_playback.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_playback.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_sensors.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_sensors.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/components/viewer_video_clipping.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_video_clipping.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/logger.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/logger.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/public/kinect-sensor.ico` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/public/kinect-sensor.ico`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/signals.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/signals.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/split_data.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/split_data.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pykinect_recorder/renderer/synology_utils.py` & `pykinect_recorder-0.9.3/pykinect_recorder/renderer/synology_utils.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.2/pyproject.toml` & `pykinect_recorder-0.9.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "pykinect-recorder"
-version = "0.9.2"
+version = "0.9.3"
 description = ""
 license = "MIT"
 authors = [
     "Kyung-Su Kang <unerue@me.com>",
     "Young-Il Kim <qhdrmfdl123@gmail.com>",
     "Yeo-Reum Lee <leeyeoreum01@gmail.com>",
 ]
 readme = ["README.md", "LICENSE"]
 packages = [{include = "pykinect_recorder"}]
 
 repository = "https://github.com/unerue/pykinect-recorder"
 keywords = ["azure", "kinect", "deep-learning", "computer-vision"]
 
 [tool.poetry.scripts]
-pykinect = "pykinect_recorder.main.cli.command:main"
+pykinect = "pykinect_recorder.cli.command:main"
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.9.1"
 pyside6 = "^6.4.2"
 open3d = "^0.17.0"
 pyqtdarktheme = "^2.1.0"
 opencv-python = "^4.7.0.72"
@@ -27,15 +27,14 @@
 sounddevice = "^0.4.6"
 soundfile = "^0.12.1"
 scikit-learn = "^1.2.2"
 qtawesome = "^1.2.3"
 pandas = "^2.0.2"
 superqt = "^0.4.1"
 
-
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 flake8 = "^6.0.0"
 black = "^23.1.0"
 isort = "^5.12.0"
 mypy = "^1.1.1"
 pyinstaller = "^5.10.1"
```

### Comparing `pykinect_recorder-0.9.2/README.md` & `pykinect_recorder-0.9.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,23 +50,27 @@
 - [ ] Intel RealSense 
 - [ ] Zenmuse SDK for Python
 
 
 ## Prerequisites
 
 ### Environment
-- Windows 10 (Recommended).
-- Windows 11.
+- Windows 10 (Recommended)
+- Windows 11
 
 ### Install Azure Kinect SDK 
 - Make sure you download Azure Kinect SDK before using this repo. 
-- SDK version '1.4.1' supported in release 1.0.0.
+- SDK version '1.4.1' supported in release 0.9.3.
 - You can download Azure Kinect SDK [here](https://github.com/microsoft/Azure-Kinect-Sensor-SDK/blob/develop/docs/usage.md).
     
 
 ## Installation
  
 ### Using pip
 ```bash
+python -m venv .venv
+.venv/Scripts/activate.ps1
 pip install pykinect-recorder
-pykinect-recorder
+pykinect
 ```
+
+### Using .exe
```

#### html2text {}

```diff
@@ -18,13 +18,14 @@
 github.com/microsoft/Azure-Kinect-Sensor-SDK. ## Features - [x] See RGB, IR,
 Depth, IMU and Audio data when recoding. - [x] Control recording option (FPS,
 brightness, ...). - [x] Change layout with drag and drop. - [x] Playback
 recorded video. - [ ] 3D reconstruction viewer with streaming/recorded video. -
 [ ] Sync devices - [ ] screen zoom in-out - [ ] imu, microphone panel redesign
 - [ ] Recording audio. - [ ] Deep learning inference (mediapipe and native)
 with streaming/recorded video. - [ ] Intel RealSense - [ ] Zenmuse SDK for
-Python ## Prerequisites ### Environment - Windows 10 (Recommended). - Windows
-11. ### Install Azure Kinect SDK - Make sure you download Azure Kinect SDK
-before using this repo. - SDK version '1.4.1' supported in release 1.0.0. - You
-can download Azure Kinect SDK [here](https://github.com/microsoft/Azure-Kinect-
+Python ## Prerequisites ### Environment - Windows 10 (Recommended) - Windows 11
+### Install Azure Kinect SDK - Make sure you download Azure Kinect SDK before
+using this repo. - SDK version '1.4.1' supported in release 0.9.3. - You can
+download Azure Kinect SDK [here](https://github.com/microsoft/Azure-Kinect-
 Sensor-SDK/blob/develop/docs/usage.md). ## Installation ### Using pip ```bash
-pip install pykinect-recorder pykinect-recorder ```
+python -m venv .venv .venv/Scripts/activate.ps1 pip install pykinect-recorder
+pykinect ``` ### Using .exe
```

### Comparing `pykinect_recorder-0.9.2/PKG-INFO` & `pykinect_recorder-0.9.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykinect-recorder
-Version: 0.9.2
+Version: 0.9.3
 Summary: 
 Home-page: https://github.com/unerue/pykinect-recorder
 License: MIT
 Keywords: azure,kinect,deep-learning,computer-vision
 Author: Kyung-Su Kang
 Author-email: unerue@me.com
 Requires-Python: >=3.9.1,<3.12
@@ -78,31 +78,35 @@
 - [ ] Intel RealSense 
 - [ ] Zenmuse SDK for Python
 
 
 ## Prerequisites
 
 ### Environment
-- Windows 10 (Recommended).
-- Windows 11.
+- Windows 10 (Recommended)
+- Windows 11
 
 ### Install Azure Kinect SDK 
 - Make sure you download Azure Kinect SDK before using this repo. 
-- SDK version '1.4.1' supported in release 1.0.0.
+- SDK version '1.4.1' supported in release 0.9.3.
 - You can download Azure Kinect SDK [here](https://github.com/microsoft/Azure-Kinect-Sensor-SDK/blob/develop/docs/usage.md).
     
 
 ## Installation
  
 ### Using pip
 ```bash
+python -m venv .venv
+.venv/Scripts/activate.ps1
 pip install pykinect-recorder
-pykinect-recorder
+pykinect
 ```
 
+### Using .exe
+
 MIT License
 
 Copyright (c) 2023 teamvisual
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pykinect-recorder Version: 0.9.2 Summary: Home-
+Metadata-Version: 2.1 Name: pykinect-recorder Version: 0.9.3 Summary: Home-
 page: https://github.com/unerue/pykinect-recorder License: MIT Keywords:
 azure,kinect,deep-learning,computer-vision Author: Kyung-Su Kang Author-email:
 unerue@me.com Requires-Python: >=3.9.1,<3.12 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-
 Dist: open3d (>=0.17.0,<0.18.0) Requires-Dist: opencv-python
@@ -33,27 +33,28 @@
 github.com/microsoft/Azure-Kinect-Sensor-SDK. ## Features - [x] See RGB, IR,
 Depth, IMU and Audio data when recoding. - [x] Control recording option (FPS,
 brightness, ...). - [x] Change layout with drag and drop. - [x] Playback
 recorded video. - [ ] 3D reconstruction viewer with streaming/recorded video. -
 [ ] Sync devices - [ ] screen zoom in-out - [ ] imu, microphone panel redesign
 - [ ] Recording audio. - [ ] Deep learning inference (mediapipe and native)
 with streaming/recorded video. - [ ] Intel RealSense - [ ] Zenmuse SDK for
-Python ## Prerequisites ### Environment - Windows 10 (Recommended). - Windows
-11. ### Install Azure Kinect SDK - Make sure you download Azure Kinect SDK
-before using this repo. - SDK version '1.4.1' supported in release 1.0.0. - You
-can download Azure Kinect SDK [here](https://github.com/microsoft/Azure-Kinect-
+Python ## Prerequisites ### Environment - Windows 10 (Recommended) - Windows 11
+### Install Azure Kinect SDK - Make sure you download Azure Kinect SDK before
+using this repo. - SDK version '1.4.1' supported in release 0.9.3. - You can
+download Azure Kinect SDK [here](https://github.com/microsoft/Azure-Kinect-
 Sensor-SDK/blob/develop/docs/usage.md). ## Installation ### Using pip ```bash
-pip install pykinect-recorder pykinect-recorder ``` MIT License Copyright (c)
-2023 teamvisual Permission is hereby granted, free of charge, to any person
-obtaining a copy of this software and associated documentation files (the
-"Software"), to deal in the Software without restriction, including without
-limitation the rights to use, copy, modify, merge, publish, distribute,
-sublicense, and/or sell copies of the Software, and to permit persons to whom
-the Software is furnished to do so, subject to the following conditions: The
-above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS
-IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
-LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
-AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
-LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
-CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
-SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+python -m venv .venv .venv/Scripts/activate.ps1 pip install pykinect-recorder
+pykinect ``` ### Using .exe MIT License Copyright (c) 2023 teamvisual
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions: The above copyright notice and this
+permission notice shall be included in all copies or substantial portions of
+the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
+EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
+OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
```

