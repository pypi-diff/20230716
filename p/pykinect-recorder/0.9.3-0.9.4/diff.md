# Comparing `tmp/pykinect_recorder-0.9.3.tar.gz` & `tmp/pykinect_recorder-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykinect_recorder-0.9.3.tar", max compression
+gzip compressed data, was "pykinect_recorder-0.9.4.tar", max compression
```

## Comparing `pykinect_recorder-0.9.3.tar` & `pykinect_recorder-0.9.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1086 2023-07-16 11:33:01.031615 pykinect_recorder-0.9.3/LICENSE
--rw-r--r--   0        0        0       46 2023-07-16 11:32:31.458067 pykinect_recorder-0.9.3/pykinect_recorder/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 11:33:01.055130 pykinect_recorder-0.9.3/pykinect_recorder/cli/__init__.py
--rw-r--r--   0        0        0      595 2023-07-16 12:22:34.306948 pykinect_recorder-0.9.3/pykinect_recorder/cli/command.py
--rw-r--r--   0        0        0     3626 2023-07-16 11:33:01.058127 pykinect_recorder-0.9.3/pykinect_recorder/main_window.py
--rw-r--r--   0        0        0      414 2023-07-16 11:33:01.058127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/__init__.py
--rw-r--r--   0        0        0      266 2023-07-16 11:33:01.059128 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/__init__.py
--rw-r--r--   0        0        0    90759 2023-07-16 11:33:01.060127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/_k4a.py
--rw-r--r--   0        0        0    19864 2023-07-16 11:33:01.061127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/_k4atypes.py
--rw-r--r--   0        0        0     8322 2023-07-16 11:33:01.062127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/calibration.py
--rw-r--r--   0        0        0     4097 2023-07-16 11:33:01.062127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/capture.py
--rw-r--r--   0        0        0     4004 2023-07-16 11:33:01.063127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/configuration.py
--rw-r--r--   0        0        0     6625 2023-07-16 11:33:01.064127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/device.py
--rw-r--r--   0        0        0     4774 2023-07-16 11:33:01.065128 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/image.py
--rw-r--r--   0        0        0     1575 2023-07-16 11:33:01.065128 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/imu_sample.py
--rw-r--r--   0        0        0     4386 2023-07-16 11:33:01.066128 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/transformation.py
--rw-r--r--   0        0        0      164 2023-07-16 11:33:01.067127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/__init__.py
--rw-r--r--   0        0        0    18158 2023-07-16 11:33:01.067127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/_k4abt.py
--rw-r--r--   0        0        0    11712 2023-07-16 11:33:01.068127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/_k4abtTypes.py
--rw-r--r--   0        0        0     1146 2023-07-16 11:33:01.069126 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/body.py
--rw-r--r--   0        0        0     2948 2023-07-16 11:33:01.069126 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/body2d.py
--rw-r--r--   0        0        0     4468 2023-07-16 11:33:01.070125 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/frame.py
--rw-r--r--   0        0        0     1617 2023-07-16 11:33:01.071126 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/joint.py
--rw-r--r--   0        0        0     1228 2023-07-16 11:33:01.071126 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/joint2d.py
--rw-r--r--   0        0        0     3079 2023-07-16 11:33:01.072126 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/tracker.py
--rw-r--r--   0        0        0      149 2023-07-16 11:33:01.072126 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/__init__.py
--rw-r--r--   0        0        0    20837 2023-07-16 11:33:01.073161 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/_k4arecord.py
--rw-r--r--   0        0        0     2344 2023-07-16 11:33:01.074127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/_k4arecordTypes.py
--rw-r--r--   0        0        0      928 2023-07-16 11:33:01.074127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/datablock.py
--rw-r--r--   0        0        0     5984 2023-07-16 11:33:01.075127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/playback.py
--rw-r--r--   0        0        0     2182 2023-07-16 11:33:01.075127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/record.py
--rw-r--r--   0        0        0     2153 2023-07-16 11:33:01.076127 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/record_configuration.py
--rw-r--r--   0        0        0     2049 2023-07-16 11:33:01.077125 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/pykinect.py
--rw-r--r--   0        0        0     5587 2023-07-16 11:33:01.077125 pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/utils.py
--rw-r--r--   0        0        0        0 2023-07-16 11:33:01.078126 pykinect_recorder-0.9.3/pykinect_recorder/pyrealsense/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 11:33:01.078126 pykinect_recorder-0.9.3/pykinect_recorder/pyzenmuse/__init__.py
--rw-r--r--   0        0        0       56 2023-07-16 11:32:31.495067 pykinect_recorder-0.9.3/pykinect_recorder/renderer/__init__.py
--rw-r--r--   0        0        0     9847 2023-07-16 11:33:01.079126 pykinect_recorder-0.9.3/pykinect_recorder/renderer/common_widgets.py
--rw-r--r--   0        0        0       17 2023-07-16 11:32:31.496068 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/__init__.py
--rw-r--r--   0        0        0     2824 2023-07-16 11:33:01.080178 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/playback_sensors.py
--rw-r--r--   0        0        0     3348 2023-07-16 11:33:01.081127 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/record_sensors.py
--rw-r--r--   0        0        0     1351 2023-07-16 11:33:01.082127 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_control.py
--rw-r--r--   0        0        0     6585 2023-07-16 11:33:01.083126 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_explorer.py
--rw-r--r--   0        0        0     3795 2023-07-16 11:33:01.083126 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_menu.py
--rw-r--r--   0        0        0    27968 2023-07-16 11:33:01.084128 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_record_control.py
--rw-r--r--   0        0        0      135 2023-07-16 11:32:31.503069 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_solutions.py
--rw-r--r--   0        0        0     2201 2023-07-16 11:33:01.085130 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/statusbar.py
--rw-r--r--   0        0        0     4680 2023-07-16 11:33:01.085130 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/topbar.py
--rw-r--r--   0        0        0      797 2023-07-16 11:33:01.086127 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_3dsensors.py
--rw-r--r--   0        0        0     1964 2023-07-16 11:33:01.087127 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_audio.py
--rw-r--r--   0        0        0     1511 2023-07-16 11:33:01.087127 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_control.py
--rw-r--r--   0        0        0     2980 2023-07-16 11:33:01.088127 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_imu_sensors.py
--rw-r--r--   0        0        0    12170 2023-07-16 11:33:01.089128 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_playback.py
--rw-r--r--   0        0        0    11462 2023-07-16 11:33:01.090125 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_sensors.py
--rw-r--r--   0        0        0      235 2023-07-16 11:32:31.508067 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_solution.py
--rw-r--r--   0        0        0    12459 2023-07-16 11:33:01.090125 pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_video_clipping.py
--rw-r--r--   0        0        0     1802 2023-07-16 11:33:01.091125 pykinect_recorder-0.9.3/pykinect_recorder/renderer/logger.py
--rw-r--r--   0        0        0    48895 2023-03-21 13:06:28.698628 pykinect_recorder-0.9.3/pykinect_recorder/renderer/public/kinect-sensor.ico
--rw-r--r--   0        0        0     1646 2023-07-16 11:33:01.092126 pykinect_recorder-0.9.3/pykinect_recorder/renderer/signals.py
--rw-r--r--   0        0        0     2943 2023-07-16 11:33:01.092126 pykinect_recorder-0.9.3/pykinect_recorder/renderer/split_data.py
--rw-r--r--   0        0        0     2483 2023-07-16 11:33:01.093126 pykinect_recorder-0.9.3/pykinect_recorder/renderer/synology_utils.py
--rw-r--r--   0        0        0     1554 2023-07-16 12:22:34.307948 pykinect_recorder-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     2493 2023-07-16 12:22:34.305946 pykinect_recorder-0.9.3/README.md
--rw-r--r--   0        0        0     4544 1970-01-01 00:00:00.000000 pykinect_recorder-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-07-16 11:33:01.031615 pykinect_recorder-0.9.4/LICENSE
+-rw-r--r--   0        0        0       46 2023-07-16 11:32:31.458067 pykinect_recorder-0.9.4/pykinect_recorder/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:33:01.055130 pykinect_recorder-0.9.4/pykinect_recorder/cli/__init__.py
+-rw-r--r--   0        0        0      717 2023-07-16 12:36:05.399548 pykinect_recorder-0.9.4/pykinect_recorder/cli/command.py
+-rw-r--r--   0        0        0     3626 2023-07-16 11:33:01.058127 pykinect_recorder-0.9.4/pykinect_recorder/main_window.py
+-rw-r--r--   0        0        0      414 2023-07-16 11:33:01.058127 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/__init__.py
+-rw-r--r--   0        0        0      266 2023-07-16 11:33:01.059128 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/__init__.py
+-rw-r--r--   0        0        0    90759 2023-07-16 11:33:01.060127 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/_k4a.py
+-rw-r--r--   0        0        0    19864 2023-07-16 11:33:01.061127 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/_k4atypes.py
+-rw-r--r--   0        0        0     8322 2023-07-16 11:33:01.062127 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/calibration.py
+-rw-r--r--   0        0        0     4097 2023-07-16 11:33:01.062127 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/capture.py
+-rw-r--r--   0        0        0     4004 2023-07-16 11:33:01.063127 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/configuration.py
+-rw-r--r--   0        0        0     6625 2023-07-16 11:33:01.064127 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/device.py
+-rw-r--r--   0        0        0     4774 2023-07-16 11:33:01.065128 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/image.py
+-rw-r--r--   0        0        0     1575 2023-07-16 11:33:01.065128 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/imu_sample.py
+-rw-r--r--   0        0        0     4386 2023-07-16 11:33:01.066128 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/transformation.py
+-rw-r--r--   0        0        0      164 2023-07-16 11:33:01.067127 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4abt/__init__.py
+-rw-r--r--   0        0        0    18158 2023-07-16 11:33:01.067127 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4abt/_k4abt.py
+-rw-r--r--   0        0        0    11712 2023-07-16 11:33:01.068127 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4abt/_k4abtTypes.py
+-rw-r--r--   0        0        0     1146 2023-07-16 11:33:01.069126 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4abt/body.py
+-rw-r--r--   0        0        0     2948 2023-07-16 11:33:01.069126 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4abt/body2d.py
+-rw-r--r--   0        0        0     4468 2023-07-16 11:33:01.070125 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4abt/frame.py
+-rw-r--r--   0        0        0     1617 2023-07-16 11:33:01.071126 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4abt/joint.py
+-rw-r--r--   0        0        0     1228 2023-07-16 11:33:01.071126 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4abt/joint2d.py
+-rw-r--r--   0        0        0     3079 2023-07-16 11:33:01.072126 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4abt/tracker.py
+-rw-r--r--   0        0        0      149 2023-07-16 11:33:01.072126 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4arecord/__init__.py
+-rw-r--r--   0        0        0    20837 2023-07-16 11:33:01.073161 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4arecord/_k4arecord.py
+-rw-r--r--   0        0        0     2344 2023-07-16 11:33:01.074127 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4arecord/_k4arecordTypes.py
+-rw-r--r--   0        0        0      928 2023-07-16 11:33:01.074127 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4arecord/datablock.py
+-rw-r--r--   0        0        0     5984 2023-07-16 11:33:01.075127 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4arecord/playback.py
+-rw-r--r--   0        0        0     2182 2023-07-16 11:33:01.075127 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4arecord/record.py
+-rw-r--r--   0        0        0     2153 2023-07-16 11:33:01.076127 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4arecord/record_configuration.py
+-rw-r--r--   0        0        0     2049 2023-07-16 11:33:01.077125 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/pykinect.py
+-rw-r--r--   0        0        0     5587 2023-07-16 11:33:01.077125 pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/utils.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:33:01.078126 pykinect_recorder-0.9.4/pykinect_recorder/pyrealsense/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 11:33:01.078126 pykinect_recorder-0.9.4/pykinect_recorder/pyzenmuse/__init__.py
+-rw-r--r--   0        0        0       56 2023-07-16 11:32:31.495067 pykinect_recorder-0.9.4/pykinect_recorder/renderer/__init__.py
+-rw-r--r--   0        0        0     9847 2023-07-16 11:33:01.079126 pykinect_recorder-0.9.4/pykinect_recorder/renderer/common_widgets.py
+-rw-r--r--   0        0        0       17 2023-07-16 11:32:31.496068 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/__init__.py
+-rw-r--r--   0        0        0     2824 2023-07-16 11:33:01.080178 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/playback_sensors.py
+-rw-r--r--   0        0        0     3348 2023-07-16 11:33:01.081127 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/record_sensors.py
+-rw-r--r--   0        0        0     1351 2023-07-16 11:33:01.082127 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/sidebar_control.py
+-rw-r--r--   0        0        0     6585 2023-07-16 11:33:01.083126 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/sidebar_explorer.py
+-rw-r--r--   0        0        0     3795 2023-07-16 11:33:01.083126 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/sidebar_menu.py
+-rw-r--r--   0        0        0    27968 2023-07-16 11:33:01.084128 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/sidebar_record_control.py
+-rw-r--r--   0        0        0      135 2023-07-16 11:32:31.503069 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/sidebar_solutions.py
+-rw-r--r--   0        0        0     2201 2023-07-16 11:33:01.085130 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/statusbar.py
+-rw-r--r--   0        0        0     4680 2023-07-16 11:33:01.085130 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/topbar.py
+-rw-r--r--   0        0        0      797 2023-07-16 11:33:01.086127 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/viewer_3dsensors.py
+-rw-r--r--   0        0        0     1964 2023-07-16 11:33:01.087127 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/viewer_audio.py
+-rw-r--r--   0        0        0     1511 2023-07-16 11:33:01.087127 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/viewer_control.py
+-rw-r--r--   0        0        0     2980 2023-07-16 11:33:01.088127 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/viewer_imu_sensors.py
+-rw-r--r--   0        0        0    12170 2023-07-16 11:33:01.089128 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/viewer_playback.py
+-rw-r--r--   0        0        0    11462 2023-07-16 11:33:01.090125 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/viewer_sensors.py
+-rw-r--r--   0        0        0      235 2023-07-16 11:32:31.508067 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/viewer_solution.py
+-rw-r--r--   0        0        0    12459 2023-07-16 11:33:01.090125 pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/viewer_video_clipping.py
+-rw-r--r--   0        0        0     1802 2023-07-16 11:33:01.091125 pykinect_recorder-0.9.4/pykinect_recorder/renderer/logger.py
+-rw-r--r--   0        0        0    48895 2023-03-21 13:06:28.698628 pykinect_recorder-0.9.4/pykinect_recorder/renderer/public/kinect-sensor.ico
+-rw-r--r--   0        0        0     1646 2023-07-16 11:33:01.092126 pykinect_recorder-0.9.4/pykinect_recorder/renderer/signals.py
+-rw-r--r--   0        0        0     2943 2023-07-16 11:33:01.092126 pykinect_recorder-0.9.4/pykinect_recorder/renderer/split_data.py
+-rw-r--r--   0        0        0     2483 2023-07-16 11:33:01.093126 pykinect_recorder-0.9.4/pykinect_recorder/renderer/synology_utils.py
+-rw-r--r--   0        0        0     1554 2023-07-16 12:36:22.434733 pykinect_recorder-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     2493 2023-07-16 12:22:34.305946 pykinect_recorder-0.9.4/README.md
+-rw-r--r--   0        0        0     4544 1970-01-01 00:00:00.000000 pykinect_recorder-0.9.4/PKG-INFO
```

### Comparing `pykinect_recorder-0.9.3/LICENSE` & `pykinect_recorder-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/cli/command.py` & `pykinect_recorder-0.9.4/pykinect_recorder/cli/command.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 #     if open:
 #         # run()
 
 
 def main():
     app = QApplication()
     qdarktheme.setup_theme()
-    main_window = MainWindow()
+    screen_rect = app.primaryScreen().size()
+    width, height = screen_rect.width(), screen_rect.height()
+    main_window = MainWindow(width, height)
     main_window.show()
     app.exec()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/main_window.py` & `pykinect_recorder-0.9.4/pykinect_recorder/main_window.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/_k4a.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/_k4a.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/_k4atypes.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/_k4atypes.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/calibration.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/calibration.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/capture.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/capture.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/configuration.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/configuration.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/device.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/device.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/image.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/image.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/imu_sample.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/imu_sample.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4a/transformation.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4a/transformation.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/_k4abt.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4abt/_k4abt.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/_k4abtTypes.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4abt/_k4abtTypes.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/body.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4abt/body.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/body2d.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4abt/body2d.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/frame.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4abt/frame.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/joint.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4abt/joint.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/joint2d.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4abt/joint2d.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4abt/tracker.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4abt/tracker.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/_k4arecord.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4arecord/_k4arecord.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/_k4arecordTypes.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4arecord/_k4arecordTypes.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/datablock.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4arecord/datablock.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/playback.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4arecord/playback.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/record.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4arecord/record.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/k4arecord/record_configuration.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/k4arecord/record_configuration.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/pykinect.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/pykinect.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/pyk4a/utils.py` & `pykinect_recorder-0.9.4/pykinect_recorder/pyk4a/utils.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/common_widgets.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/common_widgets.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/playback_sensors.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/playback_sensors.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/record_sensors.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/record_sensors.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_control.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/sidebar_control.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_explorer.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/sidebar_explorer.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_menu.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/sidebar_menu.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/sidebar_record_control.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/sidebar_record_control.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/statusbar.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/statusbar.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/topbar.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/topbar.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_3dsensors.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/viewer_3dsensors.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_audio.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/viewer_audio.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_control.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/viewer_control.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_imu_sensors.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/viewer_imu_sensors.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_playback.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/viewer_playback.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_sensors.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/viewer_sensors.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/components/viewer_video_clipping.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/components/viewer_video_clipping.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/logger.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/logger.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/public/kinect-sensor.ico` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/public/kinect-sensor.ico`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/signals.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/signals.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/split_data.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/split_data.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pykinect_recorder/renderer/synology_utils.py` & `pykinect_recorder-0.9.4/pykinect_recorder/renderer/synology_utils.py`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/pyproject.toml` & `pykinect_recorder-0.9.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykinect-recorder"
-version = "0.9.3"
+version = "0.9.4"
 description = ""
 license = "MIT"
 authors = [
     "Kyung-Su Kang <unerue@me.com>",
     "Young-Il Kim <qhdrmfdl123@gmail.com>",
     "Yeo-Reum Lee <leeyeoreum01@gmail.com>",
 ]
```

### Comparing `pykinect_recorder-0.9.3/README.md` & `pykinect_recorder-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pykinect_recorder-0.9.3/PKG-INFO` & `pykinect_recorder-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykinect-recorder
-Version: 0.9.3
+Version: 0.9.4
 Summary: 
 Home-page: https://github.com/unerue/pykinect-recorder
 License: MIT
 Keywords: azure,kinect,deep-learning,computer-vision
 Author: Kyung-Su Kang
 Author-email: unerue@me.com
 Requires-Python: >=3.9.1,<3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pykinect-recorder Version: 0.9.3 Summary: Home-
+Metadata-Version: 2.1 Name: pykinect-recorder Version: 0.9.4 Summary: Home-
 page: https://github.com/unerue/pykinect-recorder License: MIT Keywords:
 azure,kinect,deep-learning,computer-vision Author: Kyung-Su Kang Author-email:
 unerue@me.com Requires-Python: >=3.9.1,<3.12 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-
 Dist: open3d (>=0.17.0,<0.18.0) Requires-Dist: opencv-python
```

