# Comparing `tmp/micrOSDevToolKit-1.18.3.tar.gz` & `tmp/micrOSDevToolKit-1.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/micrOSDevToolKit-1.18.3.tar", last modified: Fri Jul 14 17:47:50 2023, max compression
+gzip compressed data, was "dist/micrOSDevToolKit-1.19.0.tar", last modified: Sat Jul 15 22:19:34 2023, max compression
```

## Comparing `micrOSDevToolKit-1.18.3.tar` & `micrOSDevToolKit-1.19.0.tar`

### file list

```diff
@@ -1,269 +1,248 @@
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.459323 micrOSDevToolKit-1.18.3/
--rw-r--r--   0 bnm        (501) staff       (20)      223 2023-07-06 08:46:44.000000 micrOSDevToolKit-1.18.3/MANIFEST.in
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-14 17:47:50.458766 micrOSDevToolKit-1.18.3/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.18.3/README.md
--rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.18.3/devToolKit.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.155562 micrOSDevToolKit-1.18.3/env/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.3/env/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.182551 micrOSDevToolKit-1.18.3/media/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.18.3/media/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/media/dnd.png
--rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.18.3/media/logo.png
--rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/media/logo_mini.png
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.185479 micrOSDevToolKit-1.18.3/micrOS/
--rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.18.3/micrOS/SchedulerUT.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.3/micrOS/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.244980 micrOSDevToolKit-1.18.3/micrOS/micropython/
--rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.3/micrOS/micropython/esp32-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.18.3/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.18.3/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
--rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.3/micrOS/micropython/tinypico-20220618-v1.19.1.bin
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.318768 micrOSDevToolKit-1.18.3/micrOS/source/
--rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.18.3/micrOS/source/.DS_Store
--rw-r--r--   0 bnm        (501) staff       (20)     6442 2023-07-06 10:43:08.000000 micrOSDevToolKit-1.18.3/micrOS/source/Common.py
--rw-r--r--   0 bnm        (501) staff       (20)     8431 2023-03-12 13:10:09.000000 micrOSDevToolKit-1.18.3/micrOS/source/ConfigHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     6345 2023-07-05 20:09:42.000000 micrOSDevToolKit-1.18.3/micrOS/source/Debug.py
--rw-r--r--   0 bnm        (501) staff       (20)     2047 2023-07-06 09:27:38.000000 micrOSDevToolKit-1.18.3/micrOS/source/Hooks.py
--rw-r--r--   0 bnm        (501) staff       (20)     7073 2023-07-14 17:40:17.000000 micrOSDevToolKit-1.18.3/micrOS/source/InterConnect.py
--rw-r--r--   0 bnm        (501) staff       (20)    11609 2023-07-14 17:20:00.000000 micrOSDevToolKit-1.18.3/micrOS/source/InterpreterShell.py
--rw-r--r--   0 bnm        (501) staff       (20)     7944 2023-07-04 16:56:58.000000 micrOSDevToolKit-1.18.3/micrOS/source/InterruptHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_L298N_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)    12706 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_bme280.py
--rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_buzzer.py
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_cct.py
--rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_co2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-03-19 11:46:39.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-03-02 19:54:55.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_dht11.py
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-03-02 19:54:55.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_dht22.py
--rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_ds18.py
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_genIO.py
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_intercon.py
--rw-r--r--   0 bnm        (501) staff       (20)     1618 2023-07-06 20:03:50.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_light_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_neoeffects.py
--rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_oled.py
--rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_oled_sh1106.py
--rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-04 18:36:10.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_oled_ui.py
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_presence.py
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_rgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_roboarm.py
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_servo.py
--rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_stepper.py
--rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_switch.py
--rw-r--r--   0 bnm        (501) staff       (20)     8246 2023-06-14 13:32:26.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_system.py
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_telegram.py
--rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LM_tinyrgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LP_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.18.3/micrOS/source/LP_esp32s2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.18.3/micrOS/source/LP_esp32s3.py
--rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.3/micrOS/source/LP_rp2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.3/micrOS/source/LP_tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.18.3/micrOS/source/LogicalPins.py
--rw-r--r--   0 bnm        (501) staff       (20)     9591 2023-03-12 13:32:36.000000 micrOSDevToolKit-1.18.3/micrOS/source/Network.py
--rw-r--r--   0 bnm        (501) staff       (20)     9190 2023-03-21 14:02:47.000000 micrOSDevToolKit-1.18.3/micrOS/source/Notify.py
--rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.18.3/micrOS/source/Scheduler.py
--rw-r--r--   0 bnm        (501) staff       (20)    11616 2023-07-12 17:38:11.000000 micrOSDevToolKit-1.18.3/micrOS/source/SocketServer.py
--rw-r--r--   0 bnm        (501) staff       (20)    19145 2023-07-14 17:39:42.000000 micrOSDevToolKit-1.18.3/micrOS/source/TaskManager.py
--rw-r--r--   0 bnm        (501) staff       (20)     6314 2023-03-19 12:22:25.000000 micrOSDevToolKit-1.18.3/micrOS/source/Time.py
--rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.3/micrOS/source/TinyPLed.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.335583 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/
--rw-r--r--   0 bnm        (501) staff       (20)     6020 2023-07-01 19:33:06.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/Common.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5582 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/ConfigHandler.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5406 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/Debug.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2010 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/Hooks.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5232 2023-07-01 19:36:00.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/InterConnect.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     8402 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/InterpreterShell.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4715 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/InterruptHandler.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1705 2023-07-01 19:36:00.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/LM_intercon.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1901 2023-07-01 19:35:59.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/LM_robustness.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     8842 2023-07-01 19:33:06.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/LM_system.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4265 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/LogicalPins.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     6294 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/Network.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4498 2023-07-13 18:33:20.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/Scheduler.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     8881 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/SocketServer.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)    15234 2023-07-13 18:33:20.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/TaskManager.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5912 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/Time.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      833 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/TinyPLed.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2139 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/micrOS.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     3684 2023-07-01 19:15:09.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/micrOSloader.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     3355 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.3/micrOS/source/__pycache__/urequests.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.3/micrOS/source/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     2765 2023-03-19 12:20:54.000000 micrOSDevToolKit-1.18.3/micrOS/source/micrOS.py
--rw-r--r--   0 bnm        (501) staff       (20)     4702 2023-07-06 11:13:33.000000 micrOSDevToolKit-1.18.3/micrOS/source/micrOSloader.py
--rw-r--r--   0 bnm        (501) staff       (20)   618293 2023-07-01 20:51:18.000000 micrOSDevToolKit-1.18.3/micrOS/source/pycallgraph.png
--rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.18.3/micrOS/source/reset.py
--rw-r--r--   0 bnm        (501) staff       (20)     4929 2023-03-17 16:35:50.000000 micrOSDevToolKit-1.18.3/micrOS/source/urequests.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.338931 micrOSDevToolKit-1.18.3/micrOSDevToolKit.egg-info/
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-14 17:47:49.000000 micrOSDevToolKit-1.18.3/micrOSDevToolKit.egg-info/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)     9782 2023-07-14 17:47:50.000000 micrOSDevToolKit-1.18.3/micrOSDevToolKit.egg-info/SOURCES.txt
--rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-14 17:47:49.000000 micrOSDevToolKit-1.18.3/micrOSDevToolKit.egg-info/dependency_links.txt
--rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-14 17:47:49.000000 micrOSDevToolKit-1.18.3/micrOSDevToolKit.egg-info/requires.txt
--rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-14 17:47:49.000000 micrOSDevToolKit-1.18.3/micrOSDevToolKit.egg-info/top_level.txt
--rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-14 17:47:50.459508 micrOSDevToolKit-1.18.3/setup.cfg
--rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-14 17:36:01.000000 micrOSDevToolKit-1.18.3/setup.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.348049 micrOSDevToolKit-1.18.3/toolkit/
--rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.18.3/toolkit/DevEnvCompile.py
--rw-r--r--   0 bnm        (501) staff       (20)    24176 2023-03-09 17:49:11.000000 micrOSDevToolKit-1.18.3/toolkit/DevEnvOTA.py
--rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.18.3/toolkit/DevEnvUSB.py
--rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/Gateway.py
--rw-r--r--   0 bnm        (501) staff       (20)    11568 2023-01-04 20:30:41.000000 micrOSDevToolKit-1.18.3/toolkit/MicrOSDevEnv.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.367305 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/
--rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/AirQualityBME280.py
--rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/CCTDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/CCTTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/CatGame.py
--rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/Dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/GetVersion.py
--rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/MicrophoneTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/NeoEffectsDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/NeopixelTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/RGBTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/RoboArm.py
--rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/SED_test.py
--rw-r--r--   0 bnm        (501) staff       (20)    16516 2023-07-04 19:11:19.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/SystemTest.py
--rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/Template_app.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/_micPlotting.py
--rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/uLightDemo.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.373632 micrOSDevToolKit-1.18.3/toolkit/lib/
--rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.18.3/toolkit/lib/LocalMachine.py
--rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.18.3/toolkit/lib/SearchDevices.py
--rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/lib/SerialDriverHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/lib/TerminalColors.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/lib/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.18.3/toolkit/lib/micrOSClient.py
--rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.18.3/toolkit/micrOSdashboard.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.387964 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/
--rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/LP_darwin.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.421403 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5397 2023-07-04 22:40:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/dotstar.py
--rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/ds18x20.py
--rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/framebuf.py
--rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/machine.py
--rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/micropython.py
--rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/network.py
--rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/ntptime.py
--rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/onewire.py
--rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/sim_console.py
--rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/simgc.py
--rw-r--r--   0 bnm        (501) staff       (20)     6512 2023-07-04 22:40:18.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/simulator.py
--rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/uasyncio.py
--rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/utime.py
--rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/simulator_lib/webrepl.py
--rwxr-xr-x   0 bnm        (501) staff       (20)    16943 2023-07-06 10:48:06.000000 micrOSDevToolKit-1.18.3/toolkit/socketClient.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.422417 micrOSDevToolKit-1.18.3/toolkit/workspace/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-14 17:47:50.457111 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/
--rw-r--r--   0 bnm        (501) staff       (20)     1835 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Common.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3072 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/ConfigHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1947 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Debug.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      780 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Hooks.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2225 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/InterConnect.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     4183 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/InterpreterShell.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2155 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/InterruptHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      869 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)     4282 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_bme280.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_buzzer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_cct.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_co2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)      795 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_dht11.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      795 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_dht22.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_dimmer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)      522 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_ds18.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_genIO.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)      616 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_intercon.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      512 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_light_sensor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_neoeffects.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_neopixel.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_oled.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     6082 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_oled_ui.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_presence.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_rgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_roboarm.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_servo.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_stepper.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_switch.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3632 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_system.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      872 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_telegram.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_tinyrgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      550 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LP_esp32.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      563 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LP_esp32s2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      553 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LP_esp32s3.mpy
--rw-r--r--   0 bnm        (501) staff       (20)       54 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LP_rp2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      491 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LP_tinypico.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LogicalPins.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3412 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Network.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Notify.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Scheduler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3807 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/SocketServer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     5485 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/TaskManager.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2742 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Time.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      434 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/TinyPLed.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      440 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     1250 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/micrOS.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1742 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/micrOSloader.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      198 2023-07-14 17:41:09.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/reset.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1450 2023-07-14 17:41:10.000000 micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/urequests.mpy
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.821118 micrOSDevToolKit-1.19.0/
+-rw-r--r--   0 bnm        (501) staff       (20)      223 2023-07-06 08:46:44.000000 micrOSDevToolKit-1.19.0/MANIFEST.in
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-15 22:19:34.818263 micrOSDevToolKit-1.19.0/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.19.0/README.md
+-rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.19.0/devToolKit.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.443977 micrOSDevToolKit-1.19.0/env/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.19.0/env/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.450500 micrOSDevToolKit-1.19.0/media/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.19.0/media/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/media/dnd.png
+-rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.19.0/media/logo.png
+-rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/media/logo_mini.png
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.452857 micrOSDevToolKit-1.19.0/micrOS/
+-rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.19.0/micrOS/SchedulerUT.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.19.0/micrOS/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.501919 micrOSDevToolKit-1.19.0/micrOS/micropython/
+-rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.19.0/micrOS/micropython/esp32-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.19.0/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.19.0/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
+-rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.19.0/micrOS/micropython/tinypico-20220618-v1.19.1.bin
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.567354 micrOSDevToolKit-1.19.0/micrOS/source/
+-rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.19.0/micrOS/source/.DS_Store
+-rw-r--r--   0 bnm        (501) staff       (20)     6432 2023-07-15 19:59:36.000000 micrOSDevToolKit-1.19.0/micrOS/source/Common.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8431 2023-03-12 13:10:09.000000 micrOSDevToolKit-1.19.0/micrOS/source/ConfigHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6346 2023-07-15 18:09:26.000000 micrOSDevToolKit-1.19.0/micrOS/source/Debug.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2072 2023-07-15 18:08:04.000000 micrOSDevToolKit-1.19.0/micrOS/source/Hooks.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6950 2023-07-15 20:29:58.000000 micrOSDevToolKit-1.19.0/micrOS/source/InterConnect.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11596 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.19.0/micrOS/source/InterpreterShell.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7944 2023-07-04 16:56:58.000000 micrOSDevToolKit-1.19.0/micrOS/source/InterruptHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_L298N_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_bme280.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_buzzer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_cct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_co2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-03-19 11:46:39.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_dht11.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_dht22.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_ds18.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_genIO.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_intercon.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1618 2023-07-06 20:03:50.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_light_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_neoeffects.py
+-rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_oled.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_oled_sh1106.py
+-rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-04 18:36:10.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_oled_ui.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_presence.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_rgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_roboarm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_servo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_stepper.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_switch.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8246 2023-06-14 13:32:26.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_system.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_telegram.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_tinyrgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LP_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.19.0/micrOS/source/LP_esp32s2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.19.0/micrOS/source/LP_esp32s3.py
+-rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.19.0/micrOS/source/LP_rp2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LP_tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.19.0/micrOS/source/LogicalPins.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9591 2023-03-12 13:32:36.000000 micrOSDevToolKit-1.19.0/micrOS/source/Network.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.19.0/micrOS/source/Notify.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.19.0/micrOS/source/Scheduler.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-15 19:57:59.000000 micrOSDevToolKit-1.19.0/micrOS/source/SocketServer.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19574 2023-07-15 21:22:42.000000 micrOSDevToolKit-1.19.0/micrOS/source/TaskManager.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.19.0/micrOS/source/Time.py
+-rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.19.0/micrOS/source/TinyPLed.py
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.19.0/micrOS/source/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2753 2023-07-15 18:06:40.000000 micrOSDevToolKit-1.19.0/micrOS/source/micrOS.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4702 2023-07-06 11:13:33.000000 micrOSDevToolKit-1.19.0/micrOS/source/micrOSloader.py
+-rw-r--r--   0 bnm        (501) staff       (20)   618293 2023-07-01 20:51:18.000000 micrOSDevToolKit-1.19.0/micrOS/source/pycallgraph.png
+-rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.19.0/micrOS/source/reset.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4929 2023-03-17 16:35:50.000000 micrOSDevToolKit-1.19.0/micrOS/source/urequests.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.570402 micrOSDevToolKit-1.19.0/micrOSDevToolKit.egg-info/
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-15 22:19:34.000000 micrOSDevToolKit-1.19.0/micrOSDevToolKit.egg-info/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)     8747 2023-07-15 22:19:34.000000 micrOSDevToolKit-1.19.0/micrOSDevToolKit.egg-info/SOURCES.txt
+-rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-15 22:19:34.000000 micrOSDevToolKit-1.19.0/micrOSDevToolKit.egg-info/dependency_links.txt
+-rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-15 22:19:34.000000 micrOSDevToolKit-1.19.0/micrOSDevToolKit.egg-info/requires.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-15 22:19:34.000000 micrOSDevToolKit-1.19.0/micrOSDevToolKit.egg-info/top_level.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-15 22:19:34.821301 micrOSDevToolKit-1.19.0/setup.cfg
+-rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-15 22:17:54.000000 micrOSDevToolKit-1.19.0/setup.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.578247 micrOSDevToolKit-1.19.0/toolkit/
+-rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.19.0/toolkit/DevEnvCompile.py
+-rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.19.0/toolkit/DevEnvOTA.py
+-rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.19.0/toolkit/DevEnvUSB.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/Gateway.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11568 2023-01-04 20:30:41.000000 micrOSDevToolKit-1.19.0/toolkit/MicrOSDevEnv.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.594991 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/
+-rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/AirQualityBME280.py
+-rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/CCTDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/CCTTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/CatGame.py
+-rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/Dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/GetVersion.py
+-rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/MicrophoneTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/NeoEffectsDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/NeopixelTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/RGBTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/RoboArm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/SED_test.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16516 2023-07-04 19:11:19.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/SystemTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/Template_app.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/_micPlotting.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/uLightDemo.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.598965 micrOSDevToolKit-1.19.0/toolkit/lib/
+-rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.19.0/toolkit/lib/LocalMachine.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.19.0/toolkit/lib/SearchDevices.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/lib/SerialDriverHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/lib/TerminalColors.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/lib/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.19.0/toolkit/lib/micrOSClient.py
+-rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.19.0/toolkit/micrOSdashboard.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.624214 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/
+-rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/LP_darwin.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.707354 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5397 2023-07-15 16:13:28.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/dotstar.py
+-rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/ds18x20.py
+-rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/framebuf.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/machine.py
+-rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/micropython.py
+-rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/network.py
+-rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/ntptime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/onewire.py
+-rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/sim_console.py
+-rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/simgc.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6545 2023-07-15 16:13:22.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/simulator.py
+-rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/uasyncio.py
+-rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/utime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/webrepl.py
+-rwxr-xr-x   0 bnm        (501) staff       (20)    16943 2023-07-06 10:48:06.000000 micrOSDevToolKit-1.19.0/toolkit/socketClient.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.711664 micrOSDevToolKit-1.19.0/toolkit/workspace/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.814433 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/
+-rw-r--r--   0 bnm        (501) staff       (20)     1825 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Common.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3072 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/ConfigHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1947 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Debug.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      780 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Hooks.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2117 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/InterConnect.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     4178 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/InterpreterShell.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2155 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/InterruptHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      869 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_bme280.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_buzzer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_cct.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_co2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_dht11.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_dht22.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_dimmer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)      522 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_ds18.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_genIO.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)      616 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_intercon.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      512 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_light_sensor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_neoeffects.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_neopixel.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_oled.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     6082 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_oled_ui.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_presence.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_rgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_roboarm.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_servo.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_stepper.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_switch.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3632 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_system.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      872 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_telegram.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_tinyrgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      550 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LP_esp32.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      563 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LP_esp32s2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      553 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LP_esp32s3.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)       54 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LP_rp2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      491 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LP_tinypico.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LogicalPins.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3412 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Network.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Notify.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Scheduler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/SocketServer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     5824 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/TaskManager.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Time.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      434 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/TinyPLed.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1250 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/micrOS.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1742 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/micrOSloader.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      198 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/reset.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1450 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/urequests.mpy
```

### Comparing `micrOSDevToolKit-1.18.3/PKG-INFO` & `micrOSDevToolKit-1.19.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.18.3
+Version: 1.19.0
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.18.3/README.md` & `micrOSDevToolKit-1.19.0/README.md`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/devToolKit.py` & `micrOSDevToolKit-1.19.0/devToolKit.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/media/dnd.png` & `micrOSDevToolKit-1.19.0/media/dnd.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/media/logo.png` & `micrOSDevToolKit-1.19.0/media/logo.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/media/logo_mini.png` & `micrOSDevToolKit-1.19.0/media/logo_mini.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/SchedulerUT.py` & `micrOSDevToolKit-1.19.0/micrOS/SchedulerUT.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/micropython/esp32-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.19.0/micrOS/micropython/esp32-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/micropython/esp32s2-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.19.0/micrOS/micropython/esp32s2-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin` & `micrOSDevToolKit-1.19.0/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2` & `micrOSDevToolKit-1.19.0/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/micropython/tinypico-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.19.0/micrOS/micropython/tinypico-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/.DS_Store` & `micrOSDevToolKit-1.19.0/micrOS/source/.DS_Store`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/Common.py` & `micrOSDevToolKit-1.19.0/micrOS/source/Common.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def socket_stream(func):
     """
     Provide socket message object as [msgobj]
     (SocketServer singleton class)
     """
     def wrapper(*args, **kwargs):
-        return func(*args, **kwargs, msgobj=SocketServer().reply_message)
+        return func(*args, **kwargs, msgobj=SocketServer.reply)
     return wrapper
 
 
 def transition(from_val, to_val, step_ms, interval_sec):
     """
     transition v1 (core)
     Generator for color transitions:
```

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/ConfigHandler.py` & `micrOSDevToolKit-1.19.0/micrOS/source/ConfigHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/Debug.py` & `micrOSDevToolKit-1.19.0/micrOS/source/Debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
         if analog:
             DebugCfg.step()
 
 #############################################
 #        LOGGING WITH DATA ROTATION         #
 #############################################
 
+
 def logger(data, f_name, limit):
     """
     Create generic logger function
     - implements log line rotation
     - automatic time stump
     :param data: input string data to log
     :param f_name: file name to use
@@ -186,15 +187,15 @@
 
 def errlog_add(data):
     """
     :param data: msg string / data
     :return: is ok
     """
     f_name = 'err.log'
-    return logger(data, f_name, limit=8)
+    return logger(data, f_name, limit=5)
 
 
 def errlog_get(msgobj=None):
     f_name = 'err.log'
     errcnt = log_get(f_name, msgobj)
     # Return error number
     return errcnt
```

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/Hooks.py` & `micrOSDevToolKit-1.19.0/micrOS/source/Hooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     if cfgget('boostmd') is True:
         console_write(f"[BOOT HOOKS] Set up CPU high Hz - boostmd: {cfgget('boostmd')}")
         if 'esp32' in detect_platform():
             freq(240_000_000)   # 240 Mhz
     else:
         console_write(f"[BOOT HOOKS] Set up CPU low Hz - boostmd: {cfgget('boostmd')}")
         if 'esp32' in detect_platform():
-            freq(160_000_000)   # 160 Mhz
+            freq(160_000_000)   # 160 Mhz / Half the max CPU clock
 
 
 def profiling_info(label=""):
     """
     Runtime memory measurements
     """
     if cfgget('dbg'):
```

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/InterConnect.py` & `micrOSDevToolKit-1.19.0/micrOS/source/InterConnect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 import uasyncio as asyncio
-from socket import getaddrinfo, AF_INET, SOCK_STREAM
+from socket import getaddrinfo, SOCK_STREAM
 from re import match
 from Debug import errlog_add
 from ConfigHandler import cfgget
 from SocketServer import SocketServer
 from TaskManager import Task
 
-try:
-    from gc import collect
-except:
-    console_write("[SIMULATOR MODE GC IMPORT]")
-    from simgc import collect
-
 
 class InterCon:
     CONN_MAP = {}
     PORT = cfgget('socport')
 
     def __init__(self):
         self.reader = None
@@ -43,29 +37,29 @@
             hostname = host
             # Retrieve IP address by hostname dynamically
             if InterCon.CONN_MAP.get(hostname, None) is None:
                 try:
                     addr_info = getaddrinfo(host, InterCon.PORT, 0, SOCK_STREAM)
                     host = addr_info[-1][4][0]
                 except OSError as e:
-                    SocketServer().reply_message("[intercon] NoHost: {}".format(e))
+                    SocketServer.reply("[intercon] NoHost: {}".format(e))
                     errlog_add("[intercon] send_cmd {} oserr: {}".format(host, e))
                     return ''
             else:
                 # Restore IP from cache by hostname
                 host = InterCon.CONN_MAP[hostname]
         # If IP address is available, send msg to the endpoint
         if InterCon.validate_ipv4(host):
             try:
                 # Create socket object
                 self.reader, self.writer = await asyncio.open_connection(host, InterCon.PORT)
                 # Send command over TCP/IP
                 output = await self.__run_command(cmd, hostname)
             except OSError as e:
-                SocketServer().reply_message("[intercon] NoHost: {}".format(e))
+                SocketServer.reply("[intercon] NoHost: {}".format(e))
                 errlog_add("[intercon] send_cmd {} oserr: {}".format(host, e))
                 output = None
             finally:
                 if self.writer:
                     self.writer.close()
                     await self.writer.wait_closed()
 
@@ -97,27 +91,27 @@
             await self.writer.drain()
             data, _ = await self.__receive_data(prompt=prompt)
             if data == '\0':
                 return None
             # Successful data receive, return data
             return data
         # Skip command run: prompt and host not the same!
-        SocketServer().reply_message("[intercon] prompt mismatch, hostname: {} prompt: {} ".format(hostname, prompt))
+        SocketServer.reply("[intercon] prompt mismatch, hostname: {} prompt: {} ".format(hostname, prompt))
         return None
 
     async def __receive_data(self, prompt=None):
         """
         Implements data receive loop until prompt / [configure] / Bye!
         :param prompt: socket shell prompt
         """
         data = ""
         # Collect answer data
         while True:
             try:
-                last_data = await self.reader.read(256)
+                last_data = await self.reader.read(128)
                 if not last_data:
                     break
                 last_data = last_data.decode('utf-8').strip()
                 # First data is prompt, get it
                 prompt = last_data.strip() if prompt is None else prompt
                 data += last_data
                 # Wait for prompt or special cases (conf, exit)
@@ -134,42 +128,41 @@
     Async send command wrapper for further async task integration and sync send_cmd usage (main)
     :param host: hostname / IP address
     :param cmd: command string to server socket shell
     :param com_obj: InterCon object to utilize send_cmd method and task status updates
     """
     # Send command
     with com_obj.task:
-        # Command send retry mechanism (retry: 3)
-        for _ in range(0, 3):
-            out = await com_obj.send_cmd(host, cmd)
-            if out is not None:
-                com_obj.task.out = out
-                break
+        out = await com_obj.send_cmd(host, cmd)
+        if out is None:
             await asyncio.sleep_ms(150)
-    collect()       # GC collect
+            out = await com_obj.send_cmd(host, cmd)
+            if out is None:
+                await asyncio.sleep_ms(150)
+                out = await com_obj.send_cmd(host, cmd)
+        com_obj.task.out = '' if out is None else out
     return com_obj.task.out
 
 
 def send_cmd(host, cmd):
     """
     Main wrapper of InterCon.send_cmd with
     - Intercon object creation
     - tag generation
     - task creation
     - task creation verdict generation
     :param host: hostname / IP address
     :param cmd: command string to server socket shell
     """
     def _tagify():
-        nonlocal host
-        nonlocal cmd
-        mod = cmd.split(' ')[0].strip()
+        nonlocal host, cmd
+        _mod = cmd.split(' ')[0].strip()
         if InterCon.validate_ipv4(host):
-            return f"{'.'.join(host.split('.')[-2:])}.{mod}"
-        return f"{host.replace('.local', '')}.{mod}"
+            return f"{'.'.join(host.split('.')[-2:])}.{_mod}"
+        return f"{host.replace('.local', '')}.{_mod}"
 
     com_obj = InterCon()
     tag = f"con.{_tagify()}"
     started = com_obj.task.create(callback=_send_cmd(host, cmd, com_obj), tag=tag)
     if started:
         result = {"verdict": f"Task started {host}:{cmd} -> task show {tag}", "tag": tag}
     else:
```

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/InterpreterShell.py` & `micrOSDevToolKit-1.19.0/micrOS/source/InterpreterShell.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,35 +20,35 @@
 
 
 #################################################################
 #                  SHELL Interpreter FUNCTIONS                  #
 #################################################################
 
 class Shell:
-    MICROS_VERSION = '1.18.2-0'
+    MICROS_VERSION = '1.19.0-0'
 
     def __init__(self, msg_obj=None):
         """
         comm_obj - communication object - send messages back
-                 - comm_obj.reply_message('msg')
+                 - comm_obj.reply('msg')
         """
         self.msg_obj = msg_obj
         # Used node_config parameters
         self.__devfid = cfgget('devfid')
         self.__auth_mode = cfgget('auth')
         self.__hwuid = cfgget("hwuid")
         # State machine
         self.__auth_ok = False          # session authentication state (auth mode)
         self.__conf_mode = False        # session conf mode: on / off
         # Set proper micrOS version
         try:
             cfgput('version', Shell.MICROS_VERSION)
         except Exception as e:
             console_write(f"Export system version to config failed: {e}")
-            errlog_add(f"[Shell.init][ERR] system version export error: {e}")
+            errlog_add(f"[Shell][ERR] system version export error: {e}")
 
     def msg(self, msg):
         """Message stream method"""
         try:
             self.msg_obj(msg)
         except:
             print(msg)
```

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/InterruptHandler.py` & `micrOSDevToolKit-1.19.0/micrOS/source/InterruptHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_L298N_DCmotor.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_L298N_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_VL53L0X.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_bme280.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_bme280.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Inspirated by :D
 https://randomnerdtutorials.com/micropython-bme280-esp32-esp8266/
 """
 
 
 import utime as time
 from machine import Pin, I2C
-from LM_co2 import measure_mq135
 from LogicalPins import physical_pin, pinmap_dump
 
 # BME280 default address.
 BME280_I2CADDR = 0x76
 
 # Operating Modes
 BME280_OSAMPLE_1 = 1
@@ -317,14 +316,15 @@
 
 
 def measure_w_co2():
     """
     Measure with bme280 and mq135 (CO2)
     :return dict: temp, hum, pressure, co2
     """
+    from LM_co2 import measure_mq135
     data = measure()
     data['co2 [ppm]'] = measure_mq135(data['temp [ºC]'], data['hum [%]'])
     return data
 
 
 #######################
 # LM helper functions #
```

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_buzzer.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_buzzer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_catgame.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_cct.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_cct.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_co2.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_co2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_demo.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_dht11.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_dht11.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from LM_co2 import measure_mq135
 from LogicalPins import physical_pin, pinmap_dump
 from Common import data_logger
 
 #########################################
 #  DHT22 temperature & humidity sensor  #
 #########################################
 __DHT_OBJ = None
@@ -40,14 +39,15 @@
 
 
 def measure_w_co2(log=False):
     """
     Measure with dht11 and mq135 (CO2)
     :return dict: temp, hum, co2
     """
+    from LM_co2 import measure_mq135
     _temp, _hum = __temp_hum()
     data = {'temp [ºC]': round(_temp, 2), 'hum [%]': round(_hum, 2), 'co2 [ppm]': measure_mq135(_temp, _hum)}
     if log:
         data_logger(_LOG_NAME, data=str(data))
     return data
```

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_dht22.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_dht22.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from LM_co2 import measure_mq135
 from LogicalPins import physical_pin, pinmap_dump
 from Common import data_logger
 
 #########################################
 #  DHT22 temperature & humidity sensor  #
 #########################################
 __DHT_OBJ = None
@@ -40,14 +39,15 @@
 
 
 def measure_w_co2(log=False):
     """
     Measure with dht22 and mq135 (CO2)
     :return dict: temp, hum, co2
     """
+    from LM_co2 import measure_mq135
     _temp, _hum = __temp_hum()
     data = {'temp [ºC]': round(_temp, 2), 'hum [%]': round(_hum, 2), 'co2 [ppm]': measure_mq135(_temp, _hum)}
     if log:
         data_logger(_LOG_NAME, data=str(data))
     return data
```

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_dimmer.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_distance.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_ds18.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_ds18.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_esp32.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_genIO.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_genIO.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_i2c.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_intercon.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_intercon.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_light_sensor.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_light_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_neoeffects.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_neoeffects.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_neopixel.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_oled.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_oled.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_oled_sh1106.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_oled_sh1106.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_oled_ui.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_oled_ui.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_pet_feeder.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_ph_sensor.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_presence.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_presence.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_rencoder.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_rgb.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_rgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_roboarm.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_roboarm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_robustness.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_servo.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_servo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_stepper.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_stepper.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_switch.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_switch.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_system.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_system.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_telegram.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_telegram.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LM_tinyrgb.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LM_tinyrgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LP_esp32.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LP_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LP_esp32s2.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LP_esp32s2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LP_esp32s3.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LP_esp32s3.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LP_tinypico.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LP_tinypico.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/LogicalPins.py` & `micrOSDevToolKit-1.19.0/micrOS/source/LogicalPins.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/Network.py` & `micrOSDevToolKit-1.19.0/micrOS/source/Network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/Notify.py` & `micrOSDevToolKit-1.19.0/micrOS/source/Notify.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from sys import modules
-
 import urequests
 from ConfigHandler import cfgget
 from TaskManager import exec_lm_core
 
 #########################################
 #          micrOS Notifications         #
 #          with Telegram Class          #
```

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/Scheduler.py` & `micrOSDevToolKit-1.19.0/micrOS/source/Scheduler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/SocketServer.py` & `micrOSDevToolKit-1.19.0/micrOS/source/SocketServer.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,53 +44,53 @@
         self.connected = True
         self.reader = reader
         self.writer = writer
         self.drain_event = asyncio.Event()
         self.drain_event.set()
 
         self.client_id = writer.get_extra_info('peername')
-        Debug().console(f"[Client] new conn: {self.client_id}")
+        Debug.console(f"[Client] new conn: {self.client_id}")
         client_tag = f"{'.'.join(self.client_id[0].split('.')[-2:])}:{str(self.client_id[1])}"
         self.client_id = client_tag
         self.shell = Shell(self.send)
         self.last_msg_t = ticks_ms()
 
     async def read(self):
         """
         Implements client read function, reader size: 2048
         - set timeout counter
         - read input from client (run: return False)
         - connection error handling (stop: return True)
         - exit command handling (stop: return True)
         """
-        Debug().console(f"[Client] read {self.client_id}")
+        Debug.console(f"[Client] read {self.client_id}")
         self.last_msg_t = ticks_ms()
         try:
             request = (await self.reader.read(2048))
             request = request.decode('utf8').strip()
         except Exception as e:
-            Debug().console(f"[Client] Stream read error ({self.client_id}): {e}")
+            Debug.console(f"[Client] Stream read error ({self.client_id}): {e}")
             collect()           # gc collection: "fix" for memory allocation failed, allocating 2049 bytes
             return True, ''
 
         # Input handling
-        Debug().console(f"[Client] raw request ({self.client_id}): |{request}|")
+        Debug.console(f"[Client] raw request ({self.client_id}): |{request}|")
         if request == 'exit' or request == '':
             return True, request
         return False, request
 
     def send(self, response):
         """
         Send response to client with non-async function
         """
         if self.connected:
             if self.shell.prompt() != response:
                 # Add new line if not prompt (?)
                 response = f"{response}\n"
-            # Debug().console("[Client] ----- SteamWrite: {}".format(response))
+            # Debug.console("[Client] ----- SteamWrite: {}".format(response))
             # Store data in stream buffer
             try:
                 self.writer.write(response.encode('utf8'))
             except Exception as e:
                 # Maintain ACTIVE_CLIS - remove closed connection by peer.
                 Client.drop_client(self.client_id)
                 errlog_add(f"[WARN] Client.send (auto-drop) {self.client_id}: {e}")
@@ -107,34 +107,34 @@
         # Wait for event set (True) - drain is free
         await self.drain_event.wait()
 
         # set drain busy
         self.drain_event.clear()
         try:
             # send write buffer
-            # Debug().console("  |----- start drain")
+            # Debug.console("  |----- start drain")
             await self.writer.drain()
-            # Debug().console("  |------ stop drain")
+            # Debug.console("  |------ stop drain")
         except Exception as e:
-            Debug().console(f"[Client] Drain error -> close conn: {e}")
+            Debug.console(f"[Client] Drain error -> close conn: {e}")
             await self.close()
         # set drain free
         self.drain_event.set()
 
     async def close(self):
-        Debug().console(f"[Client] Close connection {self.client_id}")
+        Debug.console(f"[Client] Close connection {self.client_id}")
         self.send("Bye!\n")
         # Reset shell state machine
         self.shell.reset()
         await asyncio.sleep_ms(50)
         try:
             self.writer.close()
             await self.writer.wait_closed()
         except Exception as e:
-            Debug().console(f"[Client] Close error {self.client_id}: {e}")
+            Debug.console(f"[Client] Close error {self.client_id}: {e}")
         self.connected = False
         Debug.INDENT = 0
         # Maintain ACTIVE_CLIS - remove closed connection by peer.
         Client.drop_client(self.client_id)
         # gc.collect()
         collect()
 
@@ -144,22 +144,22 @@
             Client.ACTIVE_CLIS.pop(client_id)
         # Update server task output (? test ?)
         Manager().server_task_msg(','.join(list(Client.ACTIVE_CLIS.keys())))
 
     async def __shell_cmd(self, request):
         # Run micrOS shell with request string
         try:
-            Debug().console("[CLIENT] --- #Run shell")
+            Debug.console("[CLIENT] --- #Run shell")
             state = self.shell.shell(request)
             if state:
                 return True
         except Exception as e:
             if "ECONNRESET" in e:
                 await self.close()
-            Debug().console(f"[Client] Shell exception: {e}")
+            Debug.console(f"[Client] Shell exception: {e}")
             return False
         collect()
         self.send(f"[HA] Shells cleanup: {mem_free()}")
         return True
 
     async def run_shell(self):
         # Update server task output (? test ?)
@@ -184,15 +184,15 @@
                 errlog_add(f"[ERR] handle_client: {e}")
                 break
         # Close connection
         await self.close()
 
     def __del__(self):
         collect()
-        Debug().console(f"Delete client connection: {self.client_id}")
+        Debug.console(f"Delete client connection: {self.client_id}")
 
 
 #########################################################
 #                    SOCKET SERVER CLASS                #
 #########################################################
 
 class SocketServer:
@@ -221,15 +221,15 @@
 
             # ---- Config ---
             SocketServer.__instance.__port = cfgget("socport")
             # ---- Set socket timeout (min 5 sec!!! hardcoded)
             soc_timeout = int(cfgget("soctout"))
             SocketServer.__instance.soc_timeout = 5 if soc_timeout < 5 else soc_timeout
             # ---         ----
-            Debug().console("[ socket server ] <<constructor>>")
+            Debug.console("[ socket server ] <<constructor>>")
         return SocketServer.__instance
 
     #####################################
     #       Socket Server Methods       #
     #####################################
 
     async def accept_client(cls, new_client):
@@ -245,31 +245,31 @@
         # Add new client immediately if queue not full
         if len(list(Client.ACTIVE_CLIS.keys())) < cls.__conn_queue:
             # Add new client to active clients dict
             Client.ACTIVE_CLIS[new_client_id] = new_client
             return True, new_client_id      # [!] Enable new connection
 
         # Get active clients timeout counters - handle new client depending on active client timeouts
-        Debug().console(f"NEW CLIENT CONN: {new_client_id}")
+        Debug.console(f"NEW CLIENT CONN: {new_client_id}")
         enable_new = False
         for cli_id, cli in Client.ACTIVE_CLIS.items():
             cli_inactive = int(ticks_diff(ticks_ms(), cli.last_msg_t) * 0.001)
-            Debug().console(f"[server] accept new {new_client_id} - active {cli_id} tout:{cls.soc_timeout - cli_inactive}s")
+            Debug.console(f"[server] accept new {new_client_id} - active {cli_id} tout:{cls.soc_timeout - cli_inactive}s")
             if not cli.connected or cli_inactive > cls.soc_timeout:
                 # OPEN CONNECTION IS INACTIVE > CLOSE
-                Debug().console("------- client timeout - accept new connection")
+                Debug.console("------- client timeout - accept new connection")
                 await cli.close()
                 enable_new = True
                 break
 
         # Interpret new connection is possible ...
         if enable_new:
             return True, new_client_id  # [!] Enable new connection
         # THERE IS ACTIVE OPEN CONNECTION, DROP NEW CLIENT!
-        Debug().console("------- connection busy")
+        Debug.console("------- connection busy")
         # Handle only single connection
         new_client.send("Connection is busy. Bye!")
         await new_client.close()  # Play nicely - close connection
         del new_client  # Clean up unused client
         return False, new_client_id     # [!] Deny new client
 
     async def handle_client(cls, reader, writer):
@@ -292,25 +292,25 @@
         await new_client.run_shell()
 
     async def run_server(cls):
         """
         Define async socket server (tcp by default)
         """
         addr = ifconfig()[1][0]
-        Debug().console(f"[ socket server ] Start socket server on {addr}:{cls.__port}")
+        Debug.console(f"[ socket server ] Start socket server on {addr}:{cls.__port}")
         cls.server = asyncio.start_server(cls.handle_client, cls.__host, cls.__port, backlog=cls.__conn_queue)
         await cls.server
-        Debug().console(f"- TCP server ready, connect: telnet {addr} {cls.__port}")
+        Debug.console(f"- TCP server ready, connect: telnet {addr} {cls.__port}")
 
     @staticmethod
-    def reply_message(msg):
+    def reply(msg):
         """
         Only used for LM msg stream over Common.socket_stream wrapper
         - stream data to all connection...
         """
         for cli_id, cli in Client.ACTIVE_CLIS.items():
             if cli.connected:
                 cli.send(msg)
 
     def __del__(cls):
-        Debug().console("[ socket server ] <<destructor>>")
+        Debug.console("[ socket server ] <<destructor>>")
         cls.server.close()
```

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/TaskManager.py` & `micrOSDevToolKit-1.19.0/micrOS/source/TaskManager.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,84 +16,93 @@
 from json import dumps
 from micropython import schedule
 import uasyncio as asyncio
 from Debug import console_write, errlog_add
 from ConfigHandler import cfgget
 from utime import ticks_ms, ticks_diff
 
+try:
+    from gc import collect
+except:
+    console_write("[SIMULATOR MODE GC IMPORT]")
+    from simgc import collect
 
 #################################################################
 #                Implement custom task class                    #
 #################################################################
 
 
 class Task:
     TASKS = {}                  # TASK OBJ list
 
     def __init__(self):
-        self.__callback = None  # [LM] Task callback: list of strings (LM call)
-        self.__inloop = False   # [LM] Task while loop for LM callback
-        self.__sleep = 20       # [LM] Task while loop - async wait (proc feed) [ms]
-        self.task = None        # [LM] Store created async task object
-        self.done = True        # [LM] Store task state
-        self.out = ""           # [LM] Store LM output
-        self.tag = None         # [LM] Task tag for identification
+        self.__callback = None       # [LM] Task callback: list of strings (LM call)
+        self.__inloop = False        # [LM] Task while loop for LM callback
+        self.__sleep = 20            # [LM] Task while loop - async wait (proc feed) [ms]
+        self.task = None             # [LM] Store created async task object
+        self.done = asyncio.Event()  # [LM] Store task state
+        self.out = ""                # [LM] Store LM output
+        self.tag = None              # [LM] Task tag for identification
 
     @staticmethod
     def is_busy(tag):
         """
         Check task is busy by tag in TASKS
         - exists + running = busy
         """
         task = Task.TASKS.get(tag, None)
-        if task is not None and not task.done:
+        if task is not None and not task.done.is_set():
             # is busy
             return True
         # is NOT busy
         return False
 
-    def __task_del(self):
+    def __task_del(self, keep_cache=False):
         """
         Delete task from TASKS
         """
-        self.done = True
+        print(f"++++++ __task_del keep_cache={keep_cache} ++++++")
+        self.done.set()
         if self.tag in Task.TASKS.keys():
-            del Task.TASKS[self.tag]
+            if keep_cache:
+                del Task.TASKS[self.tag]
+            del self.task
+        collect()           # GC collect
 
     def __enter__(self):
         """
         START CONDITION
         Helper function for Task creation in Load Modules
         [HINT] Use python with feature to utilize this feature
         """
-        self.done = False
+        self.done.clear()
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         """
         AUTOMATIC STOP CONDITION
         Helper function for Task creation in Load Modules
         [HINT] Use python with feature to utilize this feature
         """
-        self.done = True
+        self.done.set()
+        collect()           # GC collect
 
     def create(self, callback=None, tag=None):
         """
         Create async task with coroutine callback (no queue limit check!)
         - async socket server task start
         - other?
         """
         # Create task tag
         self.tag = f"aio{len(Task.TASKS)}" if tag is None else tag
         if Task.is_busy(self.tag):
             # Skip task if already running
             return False
 
         # Start task with coroutine callback
-        self.done = False
         self.task = asyncio.get_event_loop().create_task(callback)
         # Store Task object by key - for task control
         Task.TASKS[tag] = self
         return True
 
     def create_lm(self, callback=None, loop=None, sleep=None):
         """
@@ -111,16 +120,14 @@
 
         # Set parameters for async wrapper
         self.__callback = callback
         self.__inloop = self.__inloop if loop is None else loop
         # Set sleep value for async loop - optional parameter with min sleep limit check (20ms)
         self.__sleep = self.__sleep if sleep is None else sleep if sleep > 19 else self.__sleep
 
-        self.done = False
-
         self.task = asyncio.get_event_loop().create_task(self.task_wrapper())
         # Store Task object by key - for task control
         Task.TASKS[self.tag] = self
         return True
 
     def cancel(self):
         """
@@ -148,28 +155,24 @@
         - self.__callback: list - contains LM command strings
         - self.__sleep: main event loop feed
         - self.__inloop: lm call type - one-shot (False) / looped (True)
         - self.__msg_buf: lm msg object redirect to variable - store lm output
         """
         while True:
             await asyncio.sleep_ms(self.__sleep)
-            _exec_lm_core(self.__callback, msgobj=self.__msg_buff)
+            _exec_lm_core(self.__callback, msgobj=lambda msg: setattr(self, 'out', msg.strip()))
             if not self.__inloop:
                 break
-        self.done = True
-
-    def __msg_buff(self, msg):
-        """
-        Dummy msg object to store output value
-        """
-        self.out = msg
+        self.done.set()
 
     def __del__(self):
-        self.done = True
-        del self.task
+        try:
+            self.__task_del(keep_cache=True)
+        except Exception as e:
+            errlog_add(f"[ERR] Task.__del__: {e}")
 
 
 #################################################################
 #                 Implement Task manager class                  #
 #################################################################
 
 
@@ -183,93 +186,93 @@
         Singleton design pattern
         __new__ - Customize the instance creation
         cls     - class
         """
         if Manager.__instance is None:
             # TaskManager singleton properties
             Manager.__instance = super().__new__(cls)
-            # Set async event loop
-            Manager.__instance.loop = asyncio.get_event_loop()
-            Manager.__instance.loop.set_exception_handler(cls.axcept)
+            # Set async event loop exception handler
+            asyncio.get_event_loop().set_exception_handler(cls.axcept)
+            # Start system idle task (IRQ(hack) + monitoring)
             Manager.__instance.create_task(callback=Manager.idle_task(), tag="idle")
-            # [LM] Set limit for async task creation
             # ---         ----
         return Manager.__instance
 
     @staticmethod
     def axcept(loop=None, context=None):
         """
         Set as async exception handler
         """
         errlog_add(f"[aio] exception: {loop}:{context}")
 
     @staticmethod
-    def _queue_free():
+    def _queue_len():
         # Get active Load Module tasks (tag: module.function)
-        return sum([1 for tag, task in Task.TASKS.items() if not task.done and '.' in tag])
+        return sum([1 for tag, task in Task.TASKS.items() if not task.done.is_set() and '.' in tag])
 
     @staticmethod
     def _queue_limiter():
         """
         Check task queue limit
         - compare with active running tasks count
         - when queue full raise Exception!!!
         """
-        if Manager._queue_free() >= Manager.QUEUE_SIZE:
+        if Manager._queue_len() >= Manager.QUEUE_SIZE:
             msg = f"[aio] Task queue full: {Manager.QUEUE_SIZE}"
             errlog_add(msg)
             raise Exception(msg)
 
     @staticmethod
     async def idle_task():
         """
         Create IDLE task - fix IRQ task start
         - Try to measure system load - based on idle task latency
         """
         # FREQUENCY OF IDLE TASK - IMPACTS IRQ TASK SCHEDULING, SMALLER IS BEST
-        period_ms = 150
-        skip = 6        # skip idle task #SysLogic block X times, every X+1*period_ms will run this block
         my_task = Task.TASKS.get('idle')
-        my_task.out = f"i.d.l.e: {period_ms}ms"
+        my_task.out = f"i.d.l.e: 200ms"
         try:
             while True:
-                for _ in range(0, skip):
-                    # Idle task optimization
-                    await asyncio.sleep_ms(period_ms)
-                    continue
+                await asyncio.sleep_ms(200)     # 0.2s wake, irq
+                await asyncio.sleep_ms(200)     # 0.4s wake
+                await asyncio.sleep_ms(200)     # 0.6s wake
+                await asyncio.sleep_ms(200)     # 0.8s wake
+                # Probe system load
                 t = ticks_ms()
-                await asyncio.sleep_ms(period_ms)
-                # SysLogic block
-                delta_rate = int(((ticks_diff(ticks_ms(), t) / period_ms)-1) * 100)
-                Manager.OLOAD = int((Manager.OLOAD + delta_rate) / 2)
+                await asyncio.sleep_ms(200)     # 1.0s measure load
+                # SysLogic block - sys load
+                delta_rate = int(((ticks_diff(ticks_ms(), t) / 200)-1) * 100)
+                Manager.OLOAD = int((Manager.OLOAD + delta_rate) / 2)       # Average - smooth
         except Exception as e:
             errlog_add(f"[ERR] Idle task exists: {e}")
-        my_task.done = True
+        my_task.done.set()
 
-    def create_task(cls, callback, tag=None, loop=False, delay=None):
+    @staticmethod
+    def create_task(callback, tag=None, loop=False, delay=None):
         """
         Primary interface
         Generic task creator method
             Create async Task with coroutine/list(lm call) callback
         """
         if isinstance(callback, list):
+            # Check queue if task is load module
             Manager._queue_limiter()
             return Task().create_lm(callback=callback, loop=loop, sleep=delay)
         return Task().create(callback=callback, tag=tag)
 
     @staticmethod
     def list_tasks():
         """
         Primary interface
             List tasks - micrOS top :D
         """
-        q = Manager.QUEUE_SIZE - Manager._queue_free()
+        q = Manager.QUEUE_SIZE - Manager._queue_len()
         output = ["---- micrOS  top ----", f"#queue: {q} #load: {Manager.OLOAD}%\n", "#Active   #taskID"]
         for tag, task in Task.TASKS.items():
-            is_running = 'No' if task.done else 'Yes'
+            is_running = 'No' if task.done.is_set() else 'Yes'
             spcr = " " * (10 - len(is_running))
             task_view = f"{is_running}{spcr}{tag}"
             output.append(task_view)
         return tuple(output)
 
     @staticmethod
     def _parse_tag(tag):
@@ -330,23 +333,24 @@
         output = []
         for k in tasks:
             state &= terminate(k)
             output.append(f"{k}|{state}")
         msg = f"Kill: {', '.join(output)}"
         return state, msg
 
-    def run_forever(cls):
+    @staticmethod
+    def run_forever():
         """
         Run async event loop
         """
         try:
-            cls.loop.run_forever()
+            asyncio.get_event_loop().run_forever()
         except Exception as e:
             errlog_add(f"[aio] loop stopped: {e}")
-            cls.loop.close()
+            asyncio.get_event_loop().close()
 
     @staticmethod
     def server_task_msg(msg):
         server_task = Task.TASKS.get('server', None)
         if server_task is None:
             return
         server_task.out = msg
@@ -402,39 +406,39 @@
 
     def task_manager(msg_list):
         msg_len = len(msg_list)
         # [1] Handle task manipulation commands: list, kill, show - return True -> Command handled
         if 'task' == msg_list[0]:
             # task list
             if msg_len == 2 and 'list' == msg_list[1]:
-                tasks = '\n'.join(Manager().list_tasks())
+                tasks = '\n'.join(Manager.list_tasks())
                 tasks = f'{tasks}\n'
                 msgobj(tasks)
                 return True
             # task kill <taskID> / task show <taskID>
             if msg_len > 2:
                 if 'kill' == msg_list[1]:
-                    state, msg = Manager().kill(tag=msg_list[2])
+                    state, msg = Manager.kill(tag=msg_list[2])
                     msgobj(msg)
                     return True
                 if 'show' == msg_list[1]:
-                    msgobj(Manager().show(tag=msg_list[2]))
+                    msgobj(Manager.show(tag=msg_list[2]))
                     return True
             msgobj("Invalid task cmd! Help: task list / kill <taskID> / show <taskID>")
             return True
         # [2] Start async task, postfix: &, &&
         if msg_len > 2 and '&' in arg_list[-1]:
             # Evaluate task mode: loop + delay
             mode = arg_list.pop(-1)
             loop = True if mode.count('&') == 2 else False
             delay = mode.replace('&', '').strip()
             delay = int(delay) if delay.isdigit() else None
             # Create and start async lm task
             try:
-                state = Manager().create_task(arg_list, loop=loop, delay=delay)
+                state = Manager.create_task(arg_list, loop=loop, delay=delay)
             except Exception as e:
                 msgobj(e)
                 # Valid & handled task command
                 return True
             tag = '.'.join(arg_list[0:2])
             if state:
                 msgobj(f"Start {tag}")
```

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/Time.py` & `micrOSDevToolKit-1.19.0/micrOS/source/Time.py`

 * *Files 11% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             console_write(f"ntptime error.:{e}")
             err = e
         sleep_ms(100)
     errlog_add(f"[ERR] ntptime error: {err}")
     return False
 
 
-def __persistent_cache_manager(mode):
+def __sun_cache(mode):
     """
     pds - persistent data structure
     modes:
         r - recover, s - save
     """
     if mode == 's':
         # SAVE CACHE
@@ -158,22 +158,22 @@
         for key in sun.keys():
             sun[key] = [int(val) for val in sun[key]]
             sun[key][0] += int(Sun.UTC / 60)                # TODO: handle minute offset as well
             sun[key] = tuple(sun[key])
     except Exception as e:
         errlog_add(f'sunrise-api parse error: {e} sun: {sun}')
         # Retrieve cached data and return
-        __persistent_cache_manager('r')  # Using Sun.TIME
+        __sun_cache('r')  # Using Sun.TIME
         console_write('[suntime] loaded from cache')
         return Sun.TIME
 
     # Save to values class static variable for later access
     # Save and return with updated data
     Sun.TIME = sun
-    __persistent_cache_manager('s')              # Using Sun.TIME
+    __sun_cache('s')              # Using Sun.TIME
     console_write('[suntime] sync done and cached')
     return sun
 
 
 def uptime(update=False):
     """
     Get system uptime based on Sun.BOOTIME (time.time() stored at bootup)
@@ -185,8 +185,8 @@
         return "No time function was initialized..."
     delta = int(time() - Sun.BOOTIME)
     days, hours, minutes, sec = delta // 86400, (delta % 86400) // 3600, delta / 60 % 60, delta % 60
     return f"{int(days)} {int(hours)}:{int(minutes)}:{int(sec)}"
 
 
 # Initial suntime cache load (for AP mode)
-__persistent_cache_manager('r')
+__sun_cache('r')
```

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/TinyPLed.py` & `micrOSDevToolKit-1.19.0/micrOS/source/TinyPLed.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/micrOS.py` & `micrOSDevToolKit-1.19.0/micrOS/source/micrOS.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 #################################################################
 
 
 def micrOS():
     profiling_info(label='[memUsage] MAIN LOAD')
 
     # CREATE ASYNC TASK MANAGER
-    aio_man = Manager()
+    aio = Manager()
 
     # BOOT HOOK: Initial LM executions
     safe_boot_hook()
 
     # SET external interrupt with extirqcbf from nodeconfig
     external_interrupt_handler()
 
@@ -77,13 +77,13 @@
         uptime(update=True)
 
     # SET interrupt with timirqcbf from nodeconfig
     interrupt_handler()
     profiling_info(label='[memUsage] SYSTEM IS UP')
 
     # [SocketServer] as async task
-    aio_man.create_task(SocketServer().run_server(), tag='server')
+    aio.create_task(SocketServer().run_server(), tag='server')
     # [EVENT LOOP] Start async event loop
-    aio_man.run_forever()
+    aio.run_forever()
 
     # UNEXPECTED RESTART ???
     errlog_add("[ERR] !!! Unexpected micrOS restart")
```

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/micrOSloader.py` & `micrOSDevToolKit-1.19.0/micrOS/source/micrOSloader.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/pycallgraph.png` & `micrOSDevToolKit-1.19.0/micrOS/source/pycallgraph.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOS/source/urequests.py` & `micrOSDevToolKit-1.19.0/micrOS/source/urequests.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/micrOSDevToolKit.egg-info/PKG-INFO` & `micrOSDevToolKit-1.19.0/micrOSDevToolKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.18.3
+Version: 1.19.0
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.18.3/micrOSDevToolKit.egg-info/SOURCES.txt` & `micrOSDevToolKit-1.19.0/micrOSDevToolKit.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -74,34 +74,14 @@
 micrOS/source/TinyPLed.py
 micrOS/source/main.py
 micrOS/source/micrOS.py
 micrOS/source/micrOSloader.py
 micrOS/source/pycallgraph.png
 micrOS/source/reset.py
 micrOS/source/urequests.py
-micrOS/source/__pycache__/Common.cpython-39.pyc
-micrOS/source/__pycache__/ConfigHandler.cpython-39.pyc
-micrOS/source/__pycache__/Debug.cpython-39.pyc
-micrOS/source/__pycache__/Hooks.cpython-39.pyc
-micrOS/source/__pycache__/InterConnect.cpython-39.pyc
-micrOS/source/__pycache__/InterpreterShell.cpython-39.pyc
-micrOS/source/__pycache__/InterruptHandler.cpython-39.pyc
-micrOS/source/__pycache__/LM_intercon.cpython-39.pyc
-micrOS/source/__pycache__/LM_robustness.cpython-39.pyc
-micrOS/source/__pycache__/LM_system.cpython-39.pyc
-micrOS/source/__pycache__/LogicalPins.cpython-39.pyc
-micrOS/source/__pycache__/Network.cpython-39.pyc
-micrOS/source/__pycache__/Scheduler.cpython-39.pyc
-micrOS/source/__pycache__/SocketServer.cpython-39.pyc
-micrOS/source/__pycache__/TaskManager.cpython-39.pyc
-micrOS/source/__pycache__/Time.cpython-39.pyc
-micrOS/source/__pycache__/TinyPLed.cpython-39.pyc
-micrOS/source/__pycache__/micrOS.cpython-39.pyc
-micrOS/source/__pycache__/micrOSloader.cpython-39.pyc
-micrOS/source/__pycache__/urequests.cpython-39.pyc
 micrOSDevToolKit.egg-info/PKG-INFO
 micrOSDevToolKit.egg-info/SOURCES.txt
 micrOSDevToolKit.egg-info/dependency_links.txt
 micrOSDevToolKit.egg-info/requires.txt
 micrOSDevToolKit.egg-info/top_level.txt
 toolkit/DevEnvCompile.py
 toolkit/DevEnvOTA.py
```

### Comparing `micrOSDevToolKit-1.18.3/setup.py` & `micrOSDevToolKit-1.19.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # https://towardsdatascience.com/create-your-custom-python-package-that-you-can-pip-install-from-your-git-repository-f90465867893
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='micrOSDevToolKit',
-    version='1.18.3',
+    version='1.19.0',
     author='Marcell Ban',
     author_email='miros.framework@gmail.com',
     description='Development and deployment environment for micrOS, the diy micropython automation OS (IoT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/BxNxM/micrOS',
     project_urls={
```

### Comparing `micrOSDevToolKit-1.18.3/toolkit/DevEnvCompile.py` & `micrOSDevToolKit-1.19.0/toolkit/DevEnvCompile.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/DevEnvOTA.py` & `micrOSDevToolKit-1.19.0/toolkit/DevEnvOTA.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,14 +422,19 @@
             progress = round(((index + 1) / len(upload_path_list)) * 100)
 
             # Check no space in the file name
             if ' ' in os.path.basename(source):
                 self.console("\t[{}%][SKIP UPLOAD] space in resource name ... {}".format(progress, source),
                              state='WARN')
                 continue
+            # Check no "hidden" content.
+            if os.path.basename(source).startswith('__'):
+                self.console("\t[{}%][SKIP UPLOAD] resource name starts with __ {}".format(progress, source),
+                             state='WARN')
+                continue
 
             # Change workdir
             workdir_handler = LocalMachine.SimplePopPushd()
             workdir_handler.pushd(os.path.dirname(source))
 
             # Copy retry mechanism
             exitcode = -1
```

### Comparing `micrOSDevToolKit-1.18.3/toolkit/DevEnvUSB.py` & `micrOSDevToolKit-1.19.0/toolkit/DevEnvUSB.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/Gateway.py` & `micrOSDevToolKit-1.19.0/toolkit/Gateway.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/MicrOSDevEnv.py` & `micrOSDevToolKit-1.19.0/toolkit/MicrOSDevEnv.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/AirQualityBME280.py` & `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/AirQualityBME280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/AirQualityDHT22_CO2.py` & `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/AirQualityDHT22_CO2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/CCTDemo.py` & `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/CCTDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/CCTTest.py` & `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/CCTTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/CatGame.py` & `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/CatGame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/Dimmer.py` & `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/Dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/GetVersion.py` & `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/GetVersion.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/NeoEffectsDemo.py` & `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/NeoEffectsDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/NeopixelTest.py` & `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/NeopixelTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/RGBTest.py` & `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/RGBTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/RoboArm.py` & `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/RoboArm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/SED_test.py` & `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/SED_test.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/SystemTest.py` & `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/SystemTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/Template_app.py` & `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/Template_app.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/_micPlotting.py` & `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/_micPlotting.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/dashboard_apps/uLightDemo.py` & `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/uLightDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/lib/LocalMachine.py` & `micrOSDevToolKit-1.19.0/toolkit/lib/LocalMachine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/lib/SearchDevices.py` & `micrOSDevToolKit-1.19.0/toolkit/lib/SearchDevices.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/lib/SerialDriverHandler.py` & `micrOSDevToolKit-1.19.0/toolkit/lib/SerialDriverHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/lib/TerminalColors.py` & `micrOSDevToolKit-1.19.0/toolkit/lib/TerminalColors.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/lib/micrOSClient.py` & `micrOSDevToolKit-1.19.0/toolkit/lib/micrOSClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/micrOSdashboard.py` & `micrOSDevToolKit-1.19.0/toolkit/micrOSdashboard.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/LP_darwin.py` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/LP_darwin.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Jul  4 22:40:18 2023 UTC, .py size: 6512 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d29f a464 7019 0000  a..........dp...
+00000000: 610d 0d0a 0000 0000 a2c5 b264 9119 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 d600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6501 6a05 a006 6507 a101  d.l.Z.e.j...e...
 00000060: 5a08 6501 6a05 a009 6508 6402 a102 5a0a  Z.e.j...e.d...Z.
 00000070: 6500 6a05 a00b 6400 650a a102 0100 6500  e.j...d.e.....e.
@@ -83,15 +83,15 @@
 00000520: 5300 290e 4e7a 067b 3a2e 3265 7d7a 0a73  S.).Nz.{:.2e}z.s
 00000530: 696d 756c 6174 6f72 2f5a 0969 646c 655f  imulator/Z.idle_
 00000540: 7461 736b 7a32 2020 2020 2020 2020 2020  taskz2          
 00000550: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000560: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000570: 2020 2020 2020 2020 7a08 5b74 7261 6365          z.[trace
 00000580: 5d5b 7a03 735d 5b7a 025d 207a 023a 20fa  ][z.s][z.] z.: .
-00000590: 012f e9fe ffff ffda 012e fa01 20da 0029  ./.......... ..)
+00000590: 012f e9ff ffff ffda 012e fa01 20da 0029  ./.......... ..)
 000005a0: 0972 0700 0000 da04 7469 6d65 da06 665f  .r......time..f_
 000005b0: 636f 6465 da0b 636f 5f66 696c 656e 616d  code..co_filenam
 000005c0: 65da 0866 5f6c 696e 656e 6fda 0763 6f5f  e..f_lineno..co_
 000005d0: 6e61 6d65 da05 7072 696e 74da 046a 6f69  name..print..joi
 000005e0: 6eda 0573 706c 6974 2907 da05 6672 616d  n..split)...fram
 000005f0: 65da 0565 7665 6e74 da03 6172 67da 0c65  e..event..arg..e
 00000600: 6c61 7073 6564 5f74 696d 65da 0466 696c  lapsed_time..fil
@@ -110,27 +110,27 @@
 000006d0: 5448 7202 0000 0072 0700 0000 721a 0000  THr....r....r...
 000006e0: 00da 0373 7973 da08 7365 7474 7261 6365  ...sys..settrace
 000006f0: da0c 6d69 6372 4f53 6c6f 6164 6572 da04  ..micrOSloader..
 00000700: 6d61 696e da04 706f 7064 2903 7210 0000  main..popd).r...
 00000710: 005a 0873 696d 5f70 6174 6872 2a00 0000  .Z.sim_pathr*...
 00000720: 7212 0000 0072 2900 0000 7213 0000 0072  r....r)...r....r
 00000730: 0b00 0000 1f00 0000 7312 0000 0000 0108  ........s.......
-00000740: 010a 010e 0108 020c 0a0a 0108 020e 017a  ...............z
+00000740: 010a 010e 0108 020c 0b0a 0108 020e 017a  ...............z
 00000750: 1a6d 6963 724f 5349 4d2e 6d69 6372 4f53  .micrOSIM.micrOS
 00000760: 5f73 696d 5f77 6f72 6b65 7263 0100 0000  _sim_workerc....
 00000770: 0000 0000 0000 0000 0200 0000 0a00 0000  ................
 00000780: 4300 0000 7340 0000 007a 0e7c 006a 00a0  C...s@...z.|.j..
 00000790: 01a1 0001 0057 006e 2c04 0074 0279 3a01  .....W.n,..t.y:.
 000007a0: 007d 0101 007a 1474 037c 0183 0101 0057  .}...z.t.|.....W
 000007b0: 0059 0064 007d 017e 016e 0a64 007d 017e  .Y.d.}.~.n.d.}.~
 000007c0: 0130 0030 0064 0053 0029 014e 2904 720c  .0.0.d.S.).N).r.
 000007d0: 0000 0072 2000 0000 da09 4578 6365 7074  ...r .....Except
 000007e0: 696f 6e72 0200 0000 2902 7210 0000 00da  ionr....).r.....
 000007f0: 0165 7212 0000 0072 1200 0000 7213 0000  .er....r....r...
-00000800: 00da 0c77 6169 745f 7072 6f63 6573 7335  ...wait_process5
+00000800: 00da 0c77 6169 745f 7072 6f63 6573 7336  ...wait_process6
 00000810: 0000 0073 0800 0000 0001 0201 0e01 0e01  ...s............
 00000820: 7a15 6d69 6372 4f53 494d 2e77 6169 745f  z.micrOSIM.wait_
 00000830: 7072 6f63 6573 7363 0100 0000 0000 0000  processc........
 00000840: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
 00000850: 7330 0000 0074 0064 0183 0101 007c 006a  s0...t.d.....|.j
 00000860: 01a0 02a1 0001 007c 006a 016a 037c 005f  .......|.j.j.|._
 00000870: 0374 0064 02a0 047c 006a 03a1 0183 0101  .t.d...|.j......
@@ -139,15 +139,15 @@
 000008a0: 5320 7369 6d75 6c61 746f 7220 7072 6f63  S simulator proc
 000008b0: 6573 737a 295b 6d69 6372 4f53 494d 5d20  essz)[micrOSIM] 
 000008c0: 6d69 6372 4f53 2070 726f 6365 7373 2077  micrOS process w
 000008d0: 6173 2073 7461 7274 6564 3a20 7b7d 2905  as started: {}).
 000008e0: 7202 0000 0072 0c00 0000 da05 7374 6172  r....r......star
 000008f0: 7472 0d00 0000 7207 0000 00a9 0172 1000  tr....r......r..
 00000900: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00000910: 0072 3700 0000 3b00 0000 7308 0000 0000  .r7...;...s.....
+00000910: 0072 3700 0000 3c00 0000 7308 0000 0000  .r7...<...s.....
 00000920: 0108 010a 010a 017a 0e6d 6963 724f 5349  .......z.micrOSI
 00000930: 4d2e 7374 6172 7463 0100 0000 0000 0000  M.startc........
 00000940: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
 00000950: 7358 0000 007c 006a 00a0 01a1 0072 3a7c  sX...|.j.....r:|
 00000960: 006a 00a0 02a1 0001 007c 006a 00a0 01a1  .j.......|.j....
 00000970: 0072 3a74 0364 01a0 047c 006a 05a1 0183  .r:t.d...|.j....
 00000980: 0101 0074 06a0 0764 02a1 0101 0071 147c  ...t...d.....q.|
@@ -159,15 +159,15 @@
 000009e0: 205b 6d69 6372 4f53 494d 5d20 5072 6f63   [micrOSIM] Proc
 000009f0: 2077 6173 2066 696e 6973 6865 643a 207b   was finished: {
 00000a00: 7d29 0972 0c00 0000 da08 6973 5f61 6c69  }).r......is_ali
 00000a10: 7665 da09 7465 726d 696e 6174 6572 0200  ve..terminater..
 00000a20: 0000 7207 0000 0072 0d00 0000 721a 0000  ..r....r....r...
 00000a30: 00da 0573 6c65 6570 da05 636c 6f73 6572  ...sleep..closer
 00000a40: 3800 0000 7212 0000 0072 1200 0000 7213  8...r....r....r.
-00000a50: 0000 0072 3b00 0000 4100 0000 730e 0000  ...r;...A...s...
+00000a50: 0000 0072 3b00 0000 4200 0000 730e 0000  ...r;...B...s...
 00000a60: 0000 010a 010a 010a 0110 010c 010a 017a  ...............z
 00000a70: 126d 6963 724f 5349 4d2e 7465 726d 696e  .micrOSIM.termin
 00000a80: 6174 6563 0000 0000 0000 0000 0000 0000  atec............
 00000a90: 0500 0000 0b00 0000 4300 0000 73be 0000  ........C...s...
 00000aa0: 0074 006a 017d 0074 027c 0083 017d 0174  .t.j.}.t.|...}.t
 00000ab0: 037c 0083 0144 005d 9c5c 027d 027d 037a  .|...D.].\.}.}.z
 00000ac0: 447c 03a0 04a1 0072 587c 03a0 05a1 0001  D|.....rX|......
@@ -192,15 +192,15 @@
 00000bf0: 00da 036c 656e da09 656e 756d 6572 6174  ...len..enumerat
 00000c00: 6572 3a00 0000 723b 0000 0072 0200 0000  er:...r;...r....
 00000c10: 7207 0000 0072 1a00 0000 723c 0000 0072  r....r....r<...r
 00000c20: 3d00 0000 7234 0000 0029 055a 0970 726f  =...r4...).Z.pro
 00000c30: 635f 6c69 7374 5a08 7072 6f63 5f6c 656e  c_listZ.proc_len
 00000c40: da01 69da 0470 726f 6372 3500 0000 7212  ..i..procr5...r.
 00000c50: 0000 0072 1200 0000 7213 0000 00da 0873  ...r....r......s
-00000c60: 746f 705f 616c 6c4a 0000 0073 1c00 0000  top_allJ...s....
+00000c60: 746f 705f 616c 6c4b 0000 0073 1c00 0000  top_allK...s....
 00000c70: 0002 0601 0801 1001 0201 0801 0801 0801  ................
 00000c80: 1401 0c01 0c01 0e01 2c01 1601 7a11 6d69  ........,...z.mi
 00000c90: 6372 4f53 494d 2e73 746f 705f 616c 6c63  crOSIM.stop_allc
 00000ca0: 0200 0000 0000 0000 0000 0000 0c00 0000  ................
 00000cb0: 0c00 0000 4300 0000 73e6 0100 0074 00a0  ....C...s....t..
 00000cc0: 017c 01a1 017d 0274 02a0 03a1 007d 037c  .|...}.t.....}.|
 00000cd0: 03a0 0474 05a1 0101 007c 01a0 06a1 0044  ...t.....|.....D
@@ -274,15 +274,15 @@
 00001110: 6f5f 6874 6d6c 7233 0000 00da 036d 6f64  o_htmlr3.....mod
 00001120: 5a09 6675 6e63 5f64 6963 745a 0769 6d67  Z.func_dictZ.img
 00001130: 5f75 726c da04 6675 6e63 5a07 646f 635f  _url..funcZ.doc_
 00001140: 7374 725a 0a6d 6f64 5f70 696e 6d61 7072  strZ.mod_pinmapr
 00001150: 3500 0000 5a0a 7061 7261 6d5f 6365 6c6c  5...Z.param_cell
 00001160: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
 00001170: 0f5f 6c6d 5f64 6f63 5f73 7472 696e 6773  ._lm_doc_strings
-00001180: 5b00 0000 7348 0000 0000 070a 0308 010a  [...sH..........
+00001180: 5c00 0000 7348 0000 0000 070a 0308 010a  \...sH..........
 00001190: 0312 020c 011a 020a 0212 0102 0316 0102  ................
 000011a0: 020e 0116 020a 0210 0102 0110 0108 0112  ................
 000011b0: 010e 0106 010a 020c 0110 011e 0210 0116  ................
 000011c0: 0104 ff04 0104 ff10 0314 0118 0116 0308  ................
 000011d0: 017a 186d 6963 724f 5349 4d2e 5f6c 6d5f  .z.micrOSIM._lm_
 000011e0: 646f 635f 7374 7269 6e67 7363 0200 0000  doc_stringsc....
 000011f0: 0000 0000 0000 0000 0400 0000 0a00 0000  ................
@@ -301,27 +301,27 @@
 000012c0: 3a20 7b7d 290a 7208 0000 0072 0a00 0000  : {}).r....r....
 000012d0: 7257 0000 0072 3a00 0000 721a 0000 0072  rW...r:...r....r
 000012e0: 3c00 0000 7206 0000 0072 3400 0000 7202  <...r....r4...r.
 000012f0: 0000 0072 0700 0000 2904 7210 0000 0072  ...r....).r....r
 00001300: 5400 0000 7241 0000 0072 3500 0000 7212  T...rA...r5...r.
 00001310: 0000 0072 1200 0000 7213 0000 00da 1467  ...r....r......g
 00001320: 656e 5f6c 6d5f 646f 635f 6a73 6f6e 5f68  en_lm_doc_json_h
-00001330: 746d 6c95 0000 0073 1000 0000 0001 0201  tml....s........
+00001330: 746d 6c96 0000 0073 1000 0000 0001 0201  tml....s........
 00001340: 1201 0801 0c01 0801 0e01 2401 7a1d 6d69  ..........$.z.mi
 00001350: 6372 4f53 494d 2e67 656e 5f6c 6d5f 646f  crOSIM.gen_lm_do
 00001360: 635f 6a73 6f6e 5f68 746d 6c4e 2901 4629  c_json_htmlN).F)
 00001370: 0dda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
 00001380: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
 00001390: 616d 655f 5f72 0e00 0000 7214 0000 0072  ame__r....r....r
 000013a0: 0b00 0000 7236 0000 0072 3700 0000 723b  ....r6...r7...r;
 000013b0: 0000 00da 0c73 7461 7469 636d 6574 686f  .....staticmetho
 000013c0: 6472 4200 0000 7257 0000 0072 5800 0000  drB...rW...rX...
 000013d0: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
 000013e0: 1300 0000 7203 0000 0010 0000 0073 1400  ....r........s..
-000013f0: 0000 0801 0402 0a0c 0816 0806 0806 0809  ................
+000013f0: 0000 0801 0402 0a0c 0817 0806 0806 0809  ................
 00001400: 0201 0a10 083a 7203 0000 00da 085f 5f6d  .....:r......__m
 00001410: 6169 6e5f 5f7a 1c54 6573 7420 6d6f 6465  ain__z.Test mode
 00001420: 202d 2053 746f 7020 6166 7465 7220 3320   - Stop after 3 
 00001430: 7365 63e9 0300 0000 2917 722f 0000 00da  sec.....).r/....
 00001440: 026f 7372 0800 0000 721a 0000 0072 4700  .osr....r....rG.
 00001450: 0000 da04 7061 7468 da07 6469 726e 616d  ....path..dirnam
 00001460: 65da 085f 5f66 696c 655f 5fda 064d 5950  e..__file__..MYP
@@ -330,9 +330,9 @@
 00001490: 6c65 7202 0000 0072 3100 0000 722b 0000  ler....r1...r+..
 000014a0: 0072 0300 0000 7259 0000 00da 0373 696d  .r....rY.....sim
 000014b0: 7237 0000 0072 3c00 0000 723b 0000 0072  r7...r<...r;...r
 000014c0: 4200 0000 7212 0000 0072 1200 0000 7212  B...r....r....r.
 000014d0: 0000 0072 1300 0000 da08 3c6d 6f64 756c  ...r......<modul
 000014e0: 653e 0100 0000 732a 0000 0008 0108 0108  e>....s*........
 000014f0: 0108 0108 020c 010e 010e 0118 010c 0108  ................
-00001500: 0108 030e 7f00 1108 0106 0108 0108 0108  ................
+00001500: 0108 030e 7f00 1208 0106 0108 0108 0108  ................
 00001510: 010a 0108 01                             .....
```

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/machine.py` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/machine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/micropython.py` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/micropython.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/neopixel.py` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/network.py` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/sim_console.py` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/sim_console.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/simulator.py` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,17 @@
             nonlocal prev_t
             elapsed_time = "{:.2e}".format(time.time() - prev_t)
             prev_t = time.time()
             file = frame.f_code.co_filename
             line = frame.f_lineno
             code = frame.f_code.co_name
             if 'simulator/' in file and code != 'idle_task':
-                print(f"{' '*50}[trace][{elapsed_time}s][{event}] {line}: {'/'.join(file.split('/')[-2:])}.{code} {arg if arg else ''}")
+                print(f"{' '*50}[trace][{elapsed_time}s][{event}] {line}: {'/'.join(file.split('/')[-1:])}.{code} {arg if arg else ''}")
 
+        # Trace handling - DEBUG
         sys.settrace(trace_func)
         micrOSloader.main()
 
         console("[micrOSIM] Stop micrOS ({})".format(SIM_PATH))
         sim_path.popd()
 
     def wait_process(self):
```

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/uasyncio.py` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/uasyncio.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/simulator_lib/utime.py` & `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/utime.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/socketClient.py` & `micrOSDevToolKit-1.19.0/toolkit/socketClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Common.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Common.mpy`

 * *Files 7% similar despite different names*

```diff
@@ -16,100 +16,100 @@
 000000f0: 7573 7900 1663 7265 6174 655f 7461 736b  usy..create_task
 00000100: 0010 6361 6c6c 6261 636b 0006 7461 6700  ..callback..tag.
 00000110: 1664 6174 615f 6c6f 6767 6572 0008 2e64  .data_logger...d
 00000120: 6174 0081 1f08 7b7d 7b7d 000c 6d73 676f  at....{}{}..msgo
 00000130: 626a 000c 6e6f 7469 6679 0010 5465 6c65  bj..notify..Tele
 00000140: 6772 616d 000c 4e6f 7469 6679 0010 7365  gram..Notify..se
 00000150: 6e64 5f6d 7367 0008 5365 6e74 000e 7772  nd_msg..Sent..wr
-00000160: 6170 7065 7200 1a72 6570 6c79 5f6d 6573  apper..reply_mes
-00000170: 7361 6765 0014 3c6c 6973 7463 6f6d 703e  sage..<listcomp>
-00000180: 0023 0661 6463 0010 6164 705f 7072 6f70  .#.adc..adp_prop
-00000190: 000a 6174 7465 6e00 1241 5454 4e5f 3131  ..atten..ATTN_11
-000001a0: 4442 0010 7265 6164 5f75 3136 0006 7261  DB..read_u16..ra
-000001b0: 7700 0e70 6572 6365 6e74 0008 766f 6c74  w..percent..volt
-000001c0: 001a 6765 745f 7369 6e67 6c65 746f 6e00  ..get_singleton.
-000001d0: 084f 424a 5300 8155 4902 6500 8177 1054  .OBJS..UI.e..w.T
-000001e0: 454c 4547 5241 4d00 0866 756e 6300 1066  ELEGRAM..func..f
-000001f0: 726f 6d5f 7661 6c00 0c74 6f5f 7661 6c00  rom_val..to_val.
-00000200: 0e73 7465 705f 6d73 0082 0d73 066d 6178  .step_ms...s.max
-00000210: 0081 7981 5781 3d81 592f 2d35 8229 0874  ..y.W.=.Y/-5.).t
-00000220: 6173 6b00 0c66 5f6e 616d 6500 0864 6174  ask..f_name..dat
-00000230: 6100 0a6c 696d 6974 0008 7465 7874 0082  a..limit..text..
-00000240: 2f0b 8213 0670 696e 0081 4305 1d49 6d70  /....pin..C..Imp
-00000250: 6f72 7420 4552 524f 522c 2054 6173 6b4d  ort ERROR, TaskM
-00000260: 616e 6167 6572 3a20 7b7d 000a 0201 0108  anager: {}......
-00000270: 0331 2e30 0521 496d 706f 7274 2045 5252  .1.0.!Import ERR
-00000280: 4f52 2c20 4e6f 7469 6679 2e54 656c 6567  OR, Notify.Teleg
-00000290: 7261 6d3a 207b 7d00 0510 4e6f 7469 6679  ram: {}...Notify
-000002a0: 2045 5252 4f52 3a20 7b7d 000a 0207 0536   ERROR: {}.....6
-000002b0: 3535 3335 0704 3234 3530 8d7c b002 3201  5535..2450.|..2.
-000002c0: 800b 2c32 2c2c 3222 5e2d 3263 840a 8413  ..,2,,2"^-2c....
-000002d0: 8c14 8922 881d 8e17 8010 022a 011b 021c  ...".......*....
-000002e0: 0216 0259 8010 0310 042a 021b 051c 0316  ...Y.....*......
-000002f0: 031c 0416 0459 8010 062a 011b 071c 0616  .....Y...*......
-00000300: 0659 8010 082a 011b 091c 0816 0859 8010  .Y...*.......Y..
-00000310: 0a10 0b2a 021b 0c1c 0a16 0a1c 0b16 0b59  ...*...........Y
-00000320: 4814 8010 0d10 0e2a 021b 0f1c 0d16 0d1c  H......*........
-00000330: 0e16 0e59 4a29 5711 36df 4462 1637 4916  ...YJ)W.6.Db.7I.
-00000340: 1138 2300 1410 1137 3601 3401 5923 0130  .8#....76.4.Y#.0
-00000350: 0216 0d16 0e51 5116 3719 375d 4a01 5d51  .....QQ.7.7]J.]Q
-00000360: 1739 3200 1613 3201 1614 532c 0023 0210  .92...2...S,.#..
-00000370: 1162 3302 1615 5432 0310 1234 0216 1251  .b3...T2...4...Q
-00000380: 2a01 5333 0416 1611 1351 8c51 2a03 5333  *.S3.....Q.Q*.S3
-00000390: 0534 0116 1d32 0616 2251 6307 810c 110f  .4...2.."Qc.....
-000003a0: 133a 8019 6020 4500 b020 0001 c1b1 6301  .:..` E.. ....c.
-000003b0: 8158 c980 c040 0827 4f80 1e25 00b1 53b2  .X...@.'O..%..S.
-000003c0: 1021 1202 3400 1328 8135 8401 6386 08e8  .!..4..(.5..c...
-000003d0: 441e 143b 3c3d 1180 2380 0826 2c2a 2a28  D..;<=..#..&,**(
-000003e0: 58b3 80d8 44c0 8012 3eb3 2287 68f4 b2f7  X...D...>.".h...
-000003f0: 3401 c412 3fb0 b1f3 b4f7 3401 c5b0 b1d8  4...?.....4.....
-00000400: 4443 7f42 4181 c6b4 81f2 8042 5157 c712  DC.BA......BQW..
-00000410: 3eb0 b7b5 f4b6 f4f2 3401 6759 81e5 585a  >.......4.gY..XZ
-00000420: d743 2a59 5942 4712 3eb1 3401 6759 5163  .C*YYBG.>.4.gYQc
-00000430: 885c d888 80c0 409b 0115 1180 3680 0922  .\....@.....6.."
-00000440: 3936 2d3b 2928 0001 0585 c212 40b1 2000  96-;)(......@. .
-00000450: 0112 4180 1242 2501 3401 81f3 8234 0334  ..A..B%.4....4.4
-00000460: 0134 01c3 b380 d944 4380 424c 1243 2500  .4.....DC.BL.C%.
-00000470: 2287 68f4 b3f7 3401 2705 2505 b2d7 4443  ".h...4.'.%...DC
-00000480: b242 4225 0527 0512 44b0 b1b5 2001 0312  .BB%.'..D... ...
-00000490: 4180 1242 2501 3401 81f3 8234 0334 0134  A..B%.4....4.4.4
-000004a0: 01c4 1242 b434 0181 d944 48b4 8055 2505  ...B.4...DH..U%.
-000004b0: 2a02 6312 44b4 3401 2505 2a02 6302 8210  *.c.D.4.%.*.c...
-000004c0: 620a 294f 4f80 402b 00b1 5f4b 14c2 123f  b.)OO.@+.._K...?
-000004d0: 2500 b255 2500 b281 f255 f334 012f 1442  %..U%....U.4./.B
-000004e0: 2a63 8240 f004 0e29 4f4f 4f4f 8043 2b00  *c.@...)OOOO.C+.
-000004f0: b35f 4b17 c412 1425 01b4 5525 01b4 81f2  ._K....%..U%....
-00000500: 5525 0225 0034 042f 1442 2763 8254 0814  U%.%.4./.B'c.T..
-00000510: 1288 4a80 0844 8409 6460 1145 1646 1012  ..J..D..d`.E.F..
-00000520: 1647 2c00 1634 3200 162a 3201 1618 1148  .G,..42..*2....H
-00000530: 3202 3401 1633 5163 0384 2022 162a 5051  2.4..3Qc.. ".*PQ
-00000540: 8055 2425 2926 2c2c 51b0 182b 2a00 b018  .U$%)&,,Q..+*...
-00000550: 2c12 52b1 1243 3402 4346 1208 b134 01c1  ,.R..C4.CF...4..
-00000560: 1204 1203 b134 0134 01b0 182b b013 2b14  .....4.4...+..+.
-00000570: 2d12 0413 2e36 0159 2305 b018 2c51 6385  -....6.Y#...,Qc.
-00000580: 0039 0e18 5080 5e36 2831 1243 b013 2b14  .9..P.^6(1.C..+.
-00000590: 2f36 00b0 132b 142f 3600 f282 f734 01c1  /6...+./6....4..
-000005a0: b1b0 132c 8055 f7c2 123e b2b0 132c 8155  ...,.U...>...,.U
-000005b0: f422 8768 f782 3402 c32c 03b1 1030 6212  .".h..4..,...0b.
-000005c0: 3eb2 2280 64f4 8134 0210 3162 b310 3262  >.".d..4..1b..2b
-000005d0: 6382 7019 0e33 5180 652c 272b b012 1213  c.p..3Q.e,'+....
-000005e0: 3414 3536 00dd 4447 1212 1334 b055 6312  4.56..DG...4.Uc.
-000005f0: 12b0 3401 1212 1334 b056 1212 1334 b055  ..4....4.V...4.U
-00000600: 6385 10ca 0120 161c 4980 6c80 094c 2265  c.... ..I.l..L"e
-00000610: 2b22 6962 2030 120d 51de 4346 120e 51de  +"ib 0..Q.CF..Q.
-00000620: 4442 5163 b151 de44 4d12 0d13 1714 18b0  DBQc.Q.DM.......
-00000630: 5136 02c2 b263 120d 1419 b036 0144 4251  Q6...c.....6.DBQ
-00000640: 6312 0e34 0014 1a10 1bb1 101c b036 8400  c..4.........6..
-00000650: c3b3 6351 6384 10c0 8501 1c1d 4a4b 4c21  ..cQc.......JKL!
-00000660: 808a 800a 2354 452a 4210 1ec4 b014 1fb4  ....#TE*B.......
-00000670: 3601 4443 b042 4810 2014 10b0 b436 02c0  6.DC.BH. ....6..
-00000680: b151 de44 4c12 0bb0 1021 b334 8201 5952  .Q.DL....!.4..YR
-00000690: 6312 0ab1 b0b2 3403 6389 00d1 0226 224d  c.....4.c....&"M
-000006a0: 80a0 6040 2026 222b 4e2c 2b22 552c 2f2c  ..`@ &"+N,+"U,/,
-000006b0: 2212 3951 de44 7248 1080 1023 2a01 1b24  ".9Q.DrH...#*..$
-000006c0: 1c23 c159 b117 394a 2057 1236 df44 59c2  .#.Y..9J W.6.DY.
-000006d0: 490f 1238 2303 1410 b236 0134 0159 5063  I..8#....6.4.YPc
-000006e0: 5151 c228 025d 4a01 5d48 0c12 3934 0014  QQ.(.]J.]H..94..
-000006f0: 25b0 3601 c34a 2457 1236 df44 5dc2 4913  %.6..J$W.6.D].I.
-00000700: 1238 2304 1410 b236 0134 0159 124e b234  .8#....6.4.Y.N.4
-00000710: 01c3 5151 c228 025d 4a01 5db3 51de d344  ..QQ.(.]J.].Q..D
-00000720: 48b3 1026 d944 4252 6350 63              H..&.DBRcPc
+00000160: 6170 7065 7200 0a72 6570 6c79 0014 3c6c  apper..reply..<l
+00000170: 6973 7463 6f6d 703e 0023 0661 6463 0010  istcomp>.#.adc..
+00000180: 6164 705f 7072 6f70 000a 6174 7465 6e00  adp_prop..atten.
+00000190: 1241 5454 4e5f 3131 4442 0010 7265 6164  .ATTN_11DB..read
+000001a0: 5f75 3136 0006 7261 7700 0e70 6572 6365  _u16..raw..perce
+000001b0: 6e74 0008 766f 6c74 001a 6765 745f 7369  nt..volt..get_si
+000001c0: 6e67 6c65 746f 6e00 084f 424a 5300 8155  ngleton..OBJS..U
+000001d0: 4902 6500 8177 1054 454c 4547 5241 4d00  I.e..w.TELEGRAM.
+000001e0: 0866 756e 6300 1066 726f 6d5f 7661 6c00  .func..from_val.
+000001f0: 0c74 6f5f 7661 6c00 0e73 7465 705f 6d73  .to_val..step_ms
+00000200: 0082 0d73 066d 6178 0081 7981 5781 3d81  ...s.max..y.W.=.
+00000210: 592f 2d35 8229 0874 6173 6b00 0c66 5f6e  Y/-5.).task..f_n
+00000220: 616d 6500 0864 6174 6100 0a6c 696d 6974  ame..data..limit
+00000230: 0008 7465 7874 0082 2f0b 8213 0670 696e  ..text../....pin
+00000240: 0081 4305 1d49 6d70 6f72 7420 4552 524f  ..C..Import ERRO
+00000250: 522c 2054 6173 6b4d 616e 6167 6572 3a20  R, TaskManager: 
+00000260: 7b7d 000a 0201 0108 0331 2e30 0521 496d  {}.......1.0.!Im
+00000270: 706f 7274 2045 5252 4f52 2c20 4e6f 7469  port ERROR, Noti
+00000280: 6679 2e54 656c 6567 7261 6d3a 207b 7d00  fy.Telegram: {}.
+00000290: 0510 4e6f 7469 6679 2045 5252 4f52 3a20  ..Notify ERROR: 
+000002a0: 7b7d 000a 0207 0536 3535 3335 0704 3234  {}.....65535..24
+000002b0: 3530 8d7c b002 3201 800b 2c32 2c2c 3222  50.|..2...,2,,2"
+000002c0: 5e2d 3263 840a 8413 8c14 8922 881d 8e17  ^-2c......."....
+000002d0: 8010 022a 011b 021c 0216 0259 8010 0310  ...*.......Y....
+000002e0: 042a 021b 051c 0316 031c 0416 0459 8010  .*...........Y..
+000002f0: 062a 011b 071c 0616 0659 8010 082a 011b  .*.......Y...*..
+00000300: 091c 0816 0859 8010 0a10 0b2a 021b 0c1c  .....Y.....*....
+00000310: 0a16 0a1c 0b16 0b59 4814 8010 0d10 0e2a  .......YH......*
+00000320: 021b 0f1c 0d16 0d1c 0e16 0e59 4a29 5711  ...........YJ)W.
+00000330: 36df 4462 1637 4916 1138 2300 1410 1137  6.Db.7I..8#....7
+00000340: 3601 3401 5923 0130 0216 0d16 0e51 5116  6.4.Y#.0.....QQ.
+00000350: 3719 375d 4a01 5d51 1739 3200 1613 3201  7.7]J.]Q.92...2.
+00000360: 1614 532c 0023 0210 1162 3302 1615 5432  ..S,.#...b3...T2
+00000370: 0310 1234 0216 1251 2a01 5333 0416 1611  ...4...Q*.S3....
+00000380: 1351 8c51 2a03 5333 0534 0116 1d32 0616  .Q.Q*.S3.4...2..
+00000390: 2251 6307 810c 110f 133a 8019 6020 4500  "Qc......:..` E.
+000003a0: b020 0001 c1b1 6301 8148 c980 c040 0827  . ....c..H...@.'
+000003b0: 4f80 1e25 00b1 53b2 1021 1202 1328 8135  O..%..S..!...(.5
+000003c0: 8401 6386 08e8 441e 143b 3c3d 1180 2380  ..c...D..;<=..#.
+000003d0: 0826 2c2a 2a28 58b3 80d8 44c0 8012 3eb3  .&,**(X...D...>.
+000003e0: 2287 68f4 b2f7 3401 c412 3fb0 b1f3 b4f7  ".h...4...?.....
+000003f0: 3401 c5b0 b1d8 4443 7f42 4181 c6b4 81f2  4.....DC.BA.....
+00000400: 8042 5157 c712 3eb0 b7b5 f4b6 f4f2 3401  .BQW..>.......4.
+00000410: 6759 81e5 585a d743 2a59 5942 4712 3eb1  gY..XZ.C*YYBG.>.
+00000420: 3401 6759 5163 885c d888 80c0 409b 0115  4.gYQc.\....@...
+00000430: 1180 3680 0922 3936 2d3b 2928 0001 0585  ..6.."96-;)(....
+00000440: c212 40b1 2000 0112 4180 1242 2501 3401  ..@. ...A..B%.4.
+00000450: 81f3 8234 0334 0134 01c3 b380 d944 4380  ...4.4.4.....DC.
+00000460: 424c 1243 2500 2287 68f4 b3f7 3401 2705  BL.C%.".h...4.'.
+00000470: 2505 b2d7 4443 b242 4225 0527 0512 44b0  %...DC.BB%.'..D.
+00000480: b1b5 2001 0312 4180 1242 2501 3401 81f3  .. ...A..B%.4...
+00000490: 8234 0334 0134 01c4 1242 b434 0181 d944  .4.4.4...B.4...D
+000004a0: 48b4 8055 2505 2a02 6312 44b4 3401 2505  H..U%.*.c.D.4.%.
+000004b0: 2a02 6302 8210 620a 294f 4f80 402b 00b1  *.c...b.)OO.@+..
+000004c0: 5f4b 14c2 123f 2500 b255 2500 b281 f255  _K...?%..U%....U
+000004d0: f334 012f 1442 2a63 8240 f004 0e29 4f4f  .4./.B*c.@...)OO
+000004e0: 4f4f 8043 2b00 b35f 4b17 c412 1425 01b4  OO.C+.._K....%..
+000004f0: 5525 01b4 81f2 5525 0225 0034 042f 1442  U%....U%.%.4./.B
+00000500: 2763 8254 0814 1288 4a80 0844 8409 6460  'c.T....J..D..d`
+00000510: 1145 1646 1012 1647 2c00 1634 3200 162a  .E.F...G,..42..*
+00000520: 3201 1618 1148 3202 3401 1633 5163 0384  2....H2.4..3Qc..
+00000530: 2022 162a 5051 8055 2425 2926 2c2c 51b0   ".*PQ.U$%)&,,Q.
+00000540: 182b 2a00 b018 2c12 52b1 1243 3402 4346  .+*...,.R..C4.CF
+00000550: 1208 b134 01c1 1204 1203 b134 0134 01b0  ...4.......4.4..
+00000560: 182b b013 2b14 2d12 0413 2e36 0159 2305  .+..+.-....6.Y#.
+00000570: b018 2c51 6385 0039 0e18 5080 5e36 2831  ..,Qc..9..P.^6(1
+00000580: 1243 b013 2b14 2f36 00b0 132b 142f 3600  .C..+./6...+./6.
+00000590: f282 f734 01c1 b1b0 132c 8055 f7c2 123e  ...4.....,.U...>
+000005a0: b2b0 132c 8155 f422 8768 f782 3402 c32c  ...,.U.".h..4..,
+000005b0: 03b1 1030 6212 3eb2 2280 64f4 8134 0210  ...0b.>.".d..4..
+000005c0: 3162 b310 3262 6382 7019 0e33 5180 652c  1b..2bc.p..3Q.e,
+000005d0: 272b b012 1213 3414 3536 00dd 4447 1212  '+....4.56..DG..
+000005e0: 1334 b055 6312 12b0 3401 1212 1334 b056  .4.Uc...4....4.V
+000005f0: 1212 1334 b055 6385 10ca 0120 161c 4980  ...4.Uc.... ..I.
+00000600: 6c80 094c 2265 2b22 6962 2030 120d 51de  l..L"e+"ib 0..Q.
+00000610: 4346 120e 51de 4442 5163 b151 de44 4d12  CF..Q.DBQc.Q.DM.
+00000620: 0d13 1714 18b0 5136 02c2 b263 120d 1419  ......Q6...c....
+00000630: b036 0144 4251 6312 0e34 0014 1a10 1bb1  .6.DBQc..4......
+00000640: 101c b036 8400 c3b3 6351 6384 10c0 8501  ...6....cQc.....
+00000650: 1c1d 4a4b 4c21 808a 800a 2354 452a 4210  ..JKL!....#TE*B.
+00000660: 1ec4 b014 1fb4 3601 4443 b042 4810 2014  ......6.DC.BH. .
+00000670: 10b0 b436 02c0 b151 de44 4c12 0bb0 1021  ...6...Q.DL....!
+00000680: b334 8201 5952 6312 0ab1 b0b2 3403 6389  .4..YRc.....4.c.
+00000690: 00d1 0226 224d 80a0 6040 2026 222b 4e2c  ...&"M..`@ &"+N,
+000006a0: 2b22 552c 2f2c 2212 3951 de44 7248 1080  +"U,/,".9Q.DrH..
+000006b0: 1023 2a01 1b24 1c23 c159 b117 394a 2057  .#*..$.#.Y..9J W
+000006c0: 1236 df44 59c2 490f 1238 2303 1410 b236  .6.DY.I..8#....6
+000006d0: 0134 0159 5063 5151 c228 025d 4a01 5d48  .4.YPcQQ.(.]J.]H
+000006e0: 0c12 3934 0014 25b0 3601 c34a 2457 1236  ..94..%.6..J$W.6
+000006f0: df44 5dc2 4913 1238 2304 1410 b236 0134  .D].I..8#....6.4
+00000700: 0159 124e b234 01c3 5151 c228 025d 4a01  .Y.N.4..QQ.(.]J.
+00000710: 5db3 51de d344 48b3 1026 d944 4252 6350  ].Q..DH..&.DBRcP
+00000720: 63                                       c
```

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/ConfigHandler.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/ConfigHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Debug.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Debug.mpy`

 * *Files 12% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 00000250: 0005 1864 6562 7567 206c 6564 2073 7465  ...debug led ste
 00000260: 7020 6572 726f 723a 207b 7d00 0a03 0702  p error: {}.....
 00000270: 3130 0701 3007 0130 0a03 0701 3507 0135  10..0..0....5..5
 00000280: 0701 300a 0307 0130 0702 3130 0701 300a  ..0....0..10..0.
 00000290: 0307 0130 0701 3507 0135 0a03 0701 3007  ...0..5..5....0.
 000002a0: 0130 0702 3130 0a03 0701 3507 0130 0701  .0..10....5..0..
 000002b0: 358b 44a8 0230 0126 2c2c 4c22 5b46 4252  5.D..0.&,,L"[FBR
-000002c0: 8d08 894e 840b 842f 881c 8409 8807 8051  ...N.../.......Q
+000002c0: 8d08 894e 840c 842f 881c 8409 8807 8051  ...N.../.......Q
 000002d0: 1b02 1602 8010 032a 011b 041c 0316 0359  .......*.......Y
 000002e0: 8010 052a 011b 061c 0516 0559 8010 072a  ...*.......Y...*
 000002f0: 011b 081c 0716 0759 481a 8010 0910 0a10  .......YH.......
 00000300: 0b2a 031b 0c1c 0916 091c 0a16 0a1c 0b16  .*..............
 00000310: 0b59 4a07 5951 160b 4a01 5d48 0880 511b  .YJ.YQ..J.]H..Q.
 00000320: 0d16 0d4a 1757 113f df44 5016 4049 0451  ...J.W.?.DP.@I.Q
 00000330: 160d 5151 1640 1940 5d4a 015d 5432 0010  ..QQ.@.@]J.]T2..
@@ -82,41 +82,41 @@
 00000510: 120e 142c 3600 5950 6312 0d51 de43 5112  ...,6.YPc..Q.CQ.
 00000520: 0e13 2a51 de43 4912 0d14 1136 0059 5063  ..*Q.CI....6.YPc
 00000530: 4a20 5712 3fdf 4459 c049 0f12 1a23 0114  J W.?.DY.I...#..
 00000540: 20b0 3601 3401 5950 6351 51c0 2800 5d4a   .6.4.YPcQQ.(.]J
 00000550: 015d 5163 8248 1910 0f45 8065 2627 2623  .]Qc.H...E.e&'&#
 00000560: 120e 1310 4457 120e 1411 3600 c112 46b0  ....DW....6...F.
 00000570: 3401 59b1 4447 120e 1411 3600 5951 6383  4.Y.DG....6.YQc.
-00000580: 74db 021e 1247 481c 8070 800a 8818 424a  t....GH..p....BJ
+00000580: 74db 021e 1247 481c 8071 800a 8818 424a  t....GH..q....BJ
 00000590: 424c 2810 132a 0153 3300 c348 09b3 b0b1  BL(..*.S3..H....
 000005a0: b234 0359 4a17 5948 0bb3 b0b1 b210 1434  .4.YJ.YH.......4
 000005b0: 0459 4a06 5950 634a 015d 4a01 5d52 6301  .YJ.YPcJ.]J.]Rc.
-000005c0: 8a14 fc05 2831 4c4d 4e4f 807b 4a29 5d29  ....(1LMNO.{J)])
+000005c0: 8a14 fc05 2831 4c4d 4e4f 807c 4a29 5d29  ....(1LMNO.|J)])
 000005d0: 494a 2627 4725 284a 48b2 9ed8 4443 9e42  IJ&'G%(JH...DC.B
 000005e0: 41b2 c232 0012 0334 0034 01c4 1032 1433  A..2...4.4...2.3
 000005f0: b480 832e 0255 3601 1034 f210 3514 33b4  .....U6..4..5.3.
 00000600: 8386 2e02 5536 01f2 c512 4ab1 b334 0247  ....U6....J..4.G
 00000610: 4fc6 1036 1420 b5b0 3602 c032 01b6 1437  O..6. ..6..2...7
 00000620: 3600 3401 c712 50b7 3401 c8b7 1438 b036  6.4...P.4....8.6
 00000630: 0159 b614 3980 3601 59b8 b2db 4452 b7b2  .Y..9.6.Y...DR..
 00000640: d151 2e02 55c7 103a 1433 b736 01c9 4248  .Q..U..:.3.6..BH
 00000650: 103a 1433 b736 01c9 b614 2fb9 3601 5951  .:.3.6..../.6.YQ
-00000660: 5c5d 5163 0281 3841 083b 5180 7d2b 00b0  \]Qc..8A.;Q.}+..
+00000660: 5c5d 5163 0281 3841 083b 5180 7e2b 00b0  \]Qc..8A.;Q.~+..
 00000670: 5f4b 0ac1 1252 b134 012f 1442 3463 8178  _K...R.4./.B4c.x
-00000680: 4108 3b51 8083 2b00 b05f 4b12 c110 34b1  A.;Q..+.._K...4.
+00000680: 4108 3b51 8084 2b00 b05f 4b12 c110 34b1  A.;Q..+.._K...4.
 00000690: dd44 3710 32b1 dd44 31b1 2f14 422c 6386  .D7.2..D1./.B,c.
-000006a0: 30ca 0324 1548 4980 9f60 2022 222a 2a42  0..$.HI..` ""**B
+000006a0: 30ca 0324 1548 4980 a060 2022 222a 2a42  0..$.HI..` ""**B
 000006b0: 4d25 4825 5323 80c2 4847 124a b010 1634  M%H%S#..HG.J...4
 000006c0: 0247 3ac3 b314 1736 0014 1836 00c4 4269  .G:....6...6..Bi
 000006d0: b210 19b4 dd44 4381 4241 80e5 c2b1 51de  .....DC.BA....Q.
 000006e0: 4448 120f b434 0159 4245 b1b4 3401 59b3  DH...4.YBE..4.Y.
 000006f0: 1417 3600 1418 3600 c4b4 4314 515c 5d4a  ..6...6...C.Q\]J
-00000700: 0459 4a01 5db2 6381 3831 0e1a 4780 bb60  .YJ.].c.81..G..`
-00000710: 2023 101b c112 12b0 b110 1c88 3482 0263   #..........4..c
-00000720: 8128 a901 0c1d 4980 c423 4710 1bc1 1215  .(....I..#G.....
-00000730: b1b0 3402 c2b2 6384 1cd1 0114 1e49 80cb  ..4...c......I..
+00000700: 0459 4a01 5db2 6381 3831 0e1a 4780 bc60  .YJ.].c.81..G..`
+00000710: 2023 101b c112 12b0 b110 1c85 3482 0263   #..........4..c
+00000720: 8128 a901 0c1d 4980 c523 4710 1bc1 1215  .(....I..#G.....
+00000730: b1b0 3402 c2b2 6384 1cd1 0114 1e49 80cc  ..4...c......I..
 00000740: 2b25 2825 4825 3200 1202 141f 3600 3401  +%(%H%2.....6.4.
 00000750: c1b1 5f4b 25c2 2300 1420 b236 01c3 b051  .._K%.#.. .6...Q
 00000760: de44 4812 0fb3 3401 5942 45b0 b334 0159  .DH...4.YBE..4.Y
 00000770: 1202 1421 b236 0159 4219 5163 0181 6049  ...!.6.YB.Qc..`I
-00000780: 083b 5180 cb2b 00b0 5f4b 0fc1 b114 3c10  .;Q..+.._K....<.
+00000780: 083b 5180 cc2b 00b0 5f4b 0fc1 b114 3c10  .;Q..+.._K....<.
 00000790: 3d36 0144 34b1 2f14 422f 63              =6.D4./.B/c
```

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Hooks.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Hooks.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/InterConnect.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/InterConnect.mpy`

 * *Files 22% similar despite different names*

```diff
@@ -1,140 +1,133 @@
-00000000: 4d06 001f 530a 1e49 6e74 6572 436f 6e6e  M...S..InterConn
+00000000: 4d06 001f 4e09 1e49 6e74 6572 436f 6e6e  M...N..InterConn
 00000010: 6563 742e 7079 000f 1075 6173 796e 6369  ect.py...uasynci
-00000020: 6f00 1667 6574 6164 6472 696e 666f 000e  o..getaddrinfo..
-00000030: 4146 5f49 4e45 5400 1653 4f43 4b5f 5354  AF_INET..SOCK_ST
-00000040: 5245 414d 000c 736f 636b 6574 000a 6d61  REAM..socket..ma
-00000050: 7463 6800 0472 6500 1465 7272 6c6f 675f  tch..re..errlog_
-00000060: 6164 6400 0a44 6562 7567 000c 6366 6767  add..Debug..cfgg
-00000070: 6574 001a 436f 6e66 6967 4861 6e64 6c65  et..ConfigHandle
-00000080: 7200 1853 6f63 6b65 7453 6572 7665 7200  r..SocketServer.
-00000090: 0854 6173 6b00 1654 6173 6b4d 616e 6167  .Task..TaskManag
-000000a0: 6572 000e 636f 6c6c 6563 7400 0467 6300  er..collect..gc.
-000000b0: 0a73 696d 6763 0010 496e 7465 7243 6f6e  .simgc..InterCon
-000000c0: 000e 736f 6370 6f72 7400 125f 7365 6e64  ..socport.._send
-000000d0: 5f63 6d64 0008 7461 736b 0010 7365 6e64  _cmd..task..send
-000000e0: 5f63 6d64 0006 6f75 7400 1073 6c65 6570  _cmd..out..sleep
-000000f0: 5f6d 7300 0c63 6f6e 2e7b 7d00 8129 0c63  _ms..con.{}..).c
-00000100: 7265 6174 6500 1063 616c 6c62 6163 6b00  reate..callback.
-00000110: 0674 6167 000e 7665 7264 6963 7400 1464  .tag..verdict..d
-00000120: 756d 705f 6361 6368 6500 1043 4f4e 4e5f  ump_cache..CONN_
-00000130: 4d41 5000 230c 7265 6164 6572 000c 7772  MAP.#.reader..wr
-00000140: 6974 6572 001a 7661 6c69 6461 7465 5f69  iter..validate_i
-00000150: 7076 3400 812d 0850 4f52 5400 1a72 6570  pv4..-.PORT..rep
-00000160: 6c79 5f6d 6573 7361 6765 0003 1e6f 7065  ly_message...ope
-00000170: 6e5f 636f 6e6e 6563 7469 6f6e 001a 5f5f  n_connection..__
-00000180: 7275 6e5f 636f 6d6d 616e 6400 810f 1677  run_command....w
-00000190: 6169 745f 636c 6f73 6564 000c 656e 636f  ait_closed..enco
-000001a0: 6465 001c 5f5f 7265 6365 6976 655f 6461  de..__receive_da
-000001b0: 7461 0082 0302 2400 8231 8223 022e 0082  ta....$..1.#....
-000001c0: 490a 6472 6169 6e00 0c70 726f 6d70 7400  I.drain..prompt.
-000001d0: 0200 0081 7b0c 6465 636f 6465 0082 4308  ....{.decode..C.
-000001e0: 4279 6521 0007 090e 5f74 6167 6966 7900  Bye!...._tagify.
-000001f0: 0a7b 7d2e 7b7d 0081 510c 2e6c 6f63 616c  .{}.{}..Q..local
-00000200: 000e 6173 796e 6369 6f00 1a63 6f6e 736f  ..asyncio..conso
-00000210: 6c65 5f77 7269 7465 002f 2d35 8229 0868  le_write./-5.).h
-00000220: 6f73 7400 0663 6d64 000e 636f 6d5f 6f62  ost..cmd..com_ob
-00000230: 6a00 8213 0c73 7472 5f69 6e00 7d61 1068  j....str_in.}a.h
-00000240: 6f73 746e 616d 6500 822f 0b05 1a5b 5349  ostname../...[SI
-00000250: 4d55 4c41 544f 5220 4d4f 4445 2047 4320  MULATOR MODE GC 
-00000260: 494d 504f 5254 5d00 0522 5461 736b 2073  IMPORT].."Task s
-00000270: 7461 7274 6564 207b 7d3a 7b7d 202d 3e20  tarted {}:{} -> 
-00000280: 7461 736b 2073 686f 7720 7b7d 0005 0c54  task show {}...T
-00000290: 6173 6b20 6973 2042 7573 7900 0581 145e  ask is Busy....^
-000002a0: 285c 647c 5b31 2d39 5d5c 647c 315c 645c  (\d|[1-9]\d|1\d\
-000002b0: 647c 325b 302d 345d 5c64 7c32 355b 302d  d|2[0-4]\d|25[0-
-000002c0: 355d 295c 2e28 5c64 7c5b 312d 395d 5c64  5])\.(\d|[1-9]\d
-000002d0: 7c31 5c64 5c64 7c32 5b30 2d34 5d5c 647c  |1\d\d|2[0-4]\d|
-000002e0: 3235 5b30 2d35 5d29 5c2e 285c 647c 5b31  25[0-5])\.(\d|[1
-000002f0: 2d39 5d5c 647c 315c 645c 647c 325b 302d  -9]\d|1\d\d|2[0-
-00000300: 345d 5c64 7c32 355b 302d 355d 295c 2e28  4]\d|25[0-5])\.(
-00000310: 5c64 7c5b 312d 395d 5c64 7c31 5c64 5c64  \d|[1-9]\d|1\d\d
-00000320: 7c32 5b30 2d34 5d5c 647c 3235 5b30 2d35  |2[0-4]\d|25[0-5
-00000330: 5d29 2400 0515 5b69 6e74 6572 636f 6e5d  ])$...[intercon]
-00000340: 204e 6f48 6f73 743a 207b 7d00 0520 5b69   NoHost: {}.. [i
-00000350: 6e74 6572 636f 6e5d 2073 656e 645f 636d  ntercon] send_cm
-00000360: 6420 7b7d 206f 7365 7272 3a20 7b7d 0005  d {} oserr: {}..
-00000370: 205b 696e 7465 7263 6f6e 5d5b 4552 525d   [intercon][ERR]
-00000380: 2049 6e76 616c 6964 2068 6f73 743a 207b   Invalid host: {
-00000390: 7d00 0518 436f 6e6e 6563 7469 6f6e 2069  }...Connection i
-000003a0: 7320 6275 7379 2e20 4279 6521 0005 345b  s busy. Bye!..4[
-000003b0: 696e 7465 7263 6f6e 5d20 7072 6f6d 7074  intercon] prompt
-000003c0: 206d 6973 6d61 7463 682c 2068 6f73 746e   mismatch, hostn
-000003d0: 616d 653a 207b 7d20 7072 6f6d 7074 3a20  ame: {} prompt: 
-000003e0: 7b7d 2000 050b 5b63 6f6e 6669 6775 7265  {} ...[configure
-000003f0: 5d00 8a64 2424 0126 382c 2c2c 2c4c 224f  ]..d$$.&8,,,,L"O
-00000400: 276f 8974 8414 841c 8051 1b02 1643 8010  'o.t.....Q...C..
-00000410: 0310 0410 052a 031b 061c 0316 031c 0416  .....*..........
-00000420: 041c 0516 0559 8010 072a 011b 081c 0716  .....Y...*......
-00000430: 0759 8010 092a 011b 0a1c 0916 0959 8010  .Y...*.......Y..
-00000440: 0b2a 011b 0c1c 0b16 0b59 8010 0d2a 011b  .*.......Y...*..
-00000450: 0d1c 0d16 0d59 8010 0e2a 011b 0f1c 0e16  .....Y...*......
-00000460: 0e59 480e 8010 102a 011b 111c 1016 1059  .YH....*.......Y
-00000470: 4a17 5911 4423 0034 0159 8010 102a 011b  J.Y.D#.4.Y...*..
-00000480: 121c 1016 1059 4a01 5d54 3200 1013 3402  .....YJ.]T2...4.
-00000490: 1613 3201 1615 3202 1617 3203 1620 5163  ..2...2...2.. Qc
-000004a0: 0484 0c08 1a13 8810 2448 6440 8807 8432  ........$Hd@...2
-000004b0: 8419 1145 1646 1013 1647 2c00 1621 110b  ...E.F...G,..!..
-000004c0: 1014 3401 1627 3200 1622 1148 3201 3401  ..4..'2..".H2.4.
-000004d0: 1625 3202 1617 3203 162b 512a 0153 3304  .%2...2..+Q*.S3.
-000004e0: 162f 5163 0581 4811 0c22 4c80 1424 2451  ./Qc..H.."L..$$Q
-000004f0: b018 2351 b018 2412 0e34 00b0 1816 5163  ..#Q..$..4....Qc
-00000500: 8160 290e 254d 801a 232c 2223 03c1 124e  .`).%M..#,"#...N
-00000510: 1207 b1b0 3402 3401 4442 5263 5063 9338  ....4.4.DBRcPc.8
-00000520: f742 4217 4c49 4a80 2080 0742 2a42 2f22  .BB.LIJ. ..B*B/"
-00000530: 2d53 302d 6e47 2a44 5656 302d 4c25 286c  -S0-nG*DVV0-L%(l
-00000540: 464f 422c 51c3 1213 1425 b136 0143 e580  FOB,Q....%.6.C..
-00000550: b1c3 1213 1321 1426 b351 3602 51de 44cd  .....!.&.Q6.Q.D.
-00000560: 8048 1712 03b1 1213 1327 8012 0534 04c4  .H.......'...4..
-00000570: b47f 5584 5580 55c1 4a32 5712 4fdf 446b  ..U.U.U.J2W.O.Dk
-00000580: c549 2112 0d34 0014 2823 0414 1bb5 3601  .I!..4..(#....6.
-00000590: 3601 5912 0923 0514 1bb1 b536 0234 0159  6.Y..#.....6.4.Y
-000005a0: 1029 6351 51c5 2805 5d4a 015d 4247 1213  .)cQQ.(.]J.]BG..
-000005b0: 1321 b355 c112 1314 25b1 3601 4489 8149  .!.U....%.6.D..I
-000005c0: 5748 2312 4314 2ab1 1213 1327 3602 5e51  WH#.C.*....'6.^Q
-000005d0: 6830 02b0 1823 b018 24b0 142b b2b3 3602  h0...#..$..+..6.
-000005e0: 5e51 68c6 4a31 5712 4fdf 446a c549 2012  ^Qh.J1W.O.Dj.I .
-000005f0: 0d34 0014 2823 0414 1bb5 3601 3601 5912  .4..(#....6.6.Y.
-00000600: 0923 0514 1bb1 b536 0234 0159 51c6 5151  .#.....6.4.YQ.QQ
-00000610: c528 055d 4a01 5d51 b013 2444 53b0 1324  .(.]J.]Q..$DS..$
-00000620: 142c 3600 59b0 1324 142d 3600 5e51 6859  .,6.Y..$.-6.^QhY
-00000630: 5db3 51de d344 4fb6 51de 4443 5142 41b1  ].Q..DO.Q.DCQBA.
-00000640: 1213 1321 b356 b663 1209 2306 141b b136  ...!.V.c..#....6
-00000650: 0134 0159 1029 638a 00db 402a 2b4c 4a50  .4.Y.)c...@*+LJP
-00000660: 8052 6060 282c 2642 1f4c 292b 3026 4242  .R``(,&B.L)+0&BB
-00000670: 3112 5114 2eb1 3601 c1b0 142f 3600 5e51  1.Q...6..../6.^Q
-00000680: 6830 02c3 c423 07b4 dd44 4251 63b2 51de  h0...#...DBQc.Q.
-00000690: 4366 b451 de43 6112 51b4 3401 1430 1031  Cf.Q.Ca.Q.4..0.1
-000006a0: 1029 3602 1432 3600 1251 b234 0114 3310  .)6..26..Q.4..3.
-000006b0: 3436 0180 55d9 446e b013 2414 35b1 3601  46..U.Dn..$.5.6.
-000006c0: 59b0 1324 1436 3600 5e51 6859 b014 2f10  Y..$.66.^QhY../.
-000006d0: 37b4 3682 005e 5168 3002 c3c5 b310 38d9  7.6..^Qh0.....8.
-000006e0: 4442 5163 b363 120d 3400 1428 2308 141b  DBQc.c..4..(#...
-000006f0: b2b4 3602 3601 5951 6388 78ce 4128 2f4c  ..6.6.YQc.x.A(/L
-00000700: 3780 6b60 2043 2022 2e23 244c 2e44 354c  7.k` C ".#$L.D5L
-00000710: 2931 1029 c248 4db0 1323 1439 2282 0036  )1.).HM..#.9"..6
-00000720: 015e 5168 c3b3 4344 40c9 8001 b314 3a10  .^Qh..CD@.....:.
-00000730: 3b36 0114 3236 00c3 b151 de44 47b3 1432  ;6..26...Q.DG..2
-00000740: 3600 4241 b1c1 b2b3 e5c2 b1b2 1432 3600  6.BA.........26.
-00000750: dd43 4c23 09b2 dd43 4610 3cb3 dd44 4340  .CL#...CF.<..DC@
-00000760: 5301 4a0d 5712 4fdf 4446 5940 4701 4a01  S.J.W.O.DFY@G.J.
-00000770: 5d42 a17f b214 30b1 1029 3602 1430 103d  ]B....0..)6..0.=
-00000780: 103e 3602 c2b2 b12a 0263 8550 df40 2015  .>6....*.c.P.@ .
-00000790: 494a 4b80 8480 0746 252b 2626 2238 25b2  IJK....F%+&&"8%.
-000007a0: 1316 4735 5980 426a 57c3 b214 17b0 b136  ..G5Y.BjW......6
-000007b0: 025e 5168 c4b4 51de d344 48b4 b213 1618  .^Qh..Q..DH.....
-000007c0: 1842 5412 4314 1922 8116 3601 5e51 6859  .BT.C.."..6.^QhY
-000007d0: 81e5 5783 d743 1159 515c 5d12 1034 0059  ..W..C.YQ\]..4.Y
-000007e0: b213 1613 1863 8644 6a9e 0117 494a 8098  .....c.Dj...IJ..
-000007f0: 8009 8608 252a 3723 572c 0001 b0b1 2000  ....%*7#W,.... .
-00000800: 02c2 1213 3400 c310 1a14 1bb2 3400 3601  ....4.......4.6.
-00000810: c4b3 1316 141c 101d 1215 2500 2501 b334  ..........%.%..4
-00000820: 0310 1eb4 3684 00c5 b544 572c 0223 0114  ....6....DW,.#..
-00000830: 1b25 0025 01b4 3603 101f 62b4 101e 62c6  .%.%..6...b...b.
-00000840: 424c 2c02 2302 101f 62b4 101e 62c6 b663  BL,.#...b...b..c
-00000850: 0185 104a 143f 5252 80a2 2020 2f2a 3b25  ...J.?RR..  /*;%
-00000860: 0114 3310 3e36 0180 5514 3236 00c2 1213  ..3.>6..U.26....
-00000870: 1425 2500 3601 445b 1040 141b 1034 1441  .%%.6.D[.@...4.A
-00000880: 2500 1433 1034 3601 7e51 2e02 5536 01b2  %..3.46.~Q..U6..
-00000890: 3602 6310 4014 1b25 0014 3010 4210 2936  6.c.@..%..0.B.)6
-000008a0: 02b2 3602 6358 0008 2080 b460 1213 1321  ..6.cX.. ..`...!
-000008b0: 63                                       c
+00000020: 6f00 1667 6574 6164 6472 696e 666f 0016  o..getaddrinfo..
+00000030: 534f 434b 5f53 5452 4541 4d00 0c73 6f63  SOCK_STREAM..soc
+00000040: 6b65 7400 0a6d 6174 6368 0004 7265 0014  ket..match..re..
+00000050: 6572 726c 6f67 5f61 6464 000a 4465 6275  errlog_add..Debu
+00000060: 6700 0c63 6667 6765 7400 1a43 6f6e 6669  g..cfgget..Confi
+00000070: 6748 616e 646c 6572 0018 536f 636b 6574  gHandler..Socket
+00000080: 5365 7276 6572 0008 5461 736b 0016 5461  Server..Task..Ta
+00000090: 736b 4d61 6e61 6765 7200 1049 6e74 6572  skManager..Inter
+000000a0: 436f 6e00 0e73 6f63 706f 7274 0012 5f73  Con..socport.._s
+000000b0: 656e 645f 636d 6400 0874 6173 6b00 1073  end_cmd..task..s
+000000c0: 656e 645f 636d 6400 1073 6c65 6570 5f6d  end_cmd..sleep_m
+000000d0: 7300 0306 6f75 7400 0c63 6f6e 2e7b 7d00  s...out..con.{}.
+000000e0: 8129 0c63 7265 6174 6500 1063 616c 6c62  .).create..callb
+000000f0: 6163 6b00 0674 6167 000e 7665 7264 6963  ack..tag..verdic
+00000100: 7400 1464 756d 705f 6361 6368 6500 1043  t..dump_cache..C
+00000110: 4f4e 4e5f 4d41 5000 230c 7265 6164 6572  ONN_MAP.#.reader
+00000120: 000c 7772 6974 6572 001a 7661 6c69 6461  ..writer..valida
+00000130: 7465 5f69 7076 3400 812d 0850 4f52 5400  te_ipv4..-.PORT.
+00000140: 0a72 6570 6c79 001e 6f70 656e 5f63 6f6e  .reply..open_con
+00000150: 6e65 6374 696f 6e00 1a5f 5f72 756e 5f63  nection..__run_c
+00000160: 6f6d 6d61 6e64 0081 0f16 7761 6974 5f63  ommand....wait_c
+00000170: 6c6f 7365 6400 0c65 6e63 6f64 6500 1c5f  losed..encode.._
+00000180: 5f72 6563 6569 7665 5f64 6174 6100 8203  _receive_data...
+00000190: 0224 0082 3182 2302 2e00 8249 0a64 7261  .$..1.#....I.dra
+000001a0: 696e 000c 7072 6f6d 7074 0002 0000 817b  in..prompt.....{
+000001b0: 0c64 6563 6f64 6500 8243 0842 7965 2100  .decode..C.Bye!.
+000001c0: 0709 0e5f 7461 6769 6679 000a 7b7d 2e7b  ..._tagify..{}.{
+000001d0: 7d00 8151 0c2e 6c6f 6361 6c00 0e61 7379  }..Q..local..asy
+000001e0: 6e63 696f 002f 2d35 8229 0868 6f73 7400  ncio./-5.).host.
+000001f0: 0663 6d64 000e 636f 6d5f 6f62 6a00 8213  .cmd..com_obj...
+00000200: 0c73 7472 5f69 6e00 7d61 1068 6f73 746e  .str_in.}a.hostn
+00000210: 616d 6500 822f 0b05 2254 6173 6b20 7374  ame../.."Task st
+00000220: 6172 7465 6420 7b7d 3a7b 7d20 2d3e 2074  arted {}:{} -> t
+00000230: 6173 6b20 7368 6f77 207b 7d00 050c 5461  ask show {}...Ta
+00000240: 736b 2069 7320 4275 7379 0005 8114 5e28  sk is Busy....^(
+00000250: 5c64 7c5b 312d 395d 5c64 7c31 5c64 5c64  \d|[1-9]\d|1\d\d
+00000260: 7c32 5b30 2d34 5d5c 647c 3235 5b30 2d35  |2[0-4]\d|25[0-5
+00000270: 5d29 5c2e 285c 647c 5b31 2d39 5d5c 647c  ])\.(\d|[1-9]\d|
+00000280: 315c 645c 647c 325b 302d 345d 5c64 7c32  1\d\d|2[0-4]\d|2
+00000290: 355b 302d 355d 295c 2e28 5c64 7c5b 312d  5[0-5])\.(\d|[1-
+000002a0: 395d 5c64 7c31 5c64 5c64 7c32 5b30 2d34  9]\d|1\d\d|2[0-4
+000002b0: 5d5c 647c 3235 5b30 2d35 5d29 5c2e 285c  ]\d|25[0-5])\.(\
+000002c0: 647c 5b31 2d39 5d5c 647c 315c 645c 647c  d|[1-9]\d|1\d\d|
+000002d0: 325b 302d 345d 5c64 7c32 355b 302d 355d  2[0-4]\d|25[0-5]
+000002e0: 2924 0005 155b 696e 7465 7263 6f6e 5d20  )$...[intercon] 
+000002f0: 4e6f 486f 7374 3a20 7b7d 0005 205b 696e  NoHost: {}.. [in
+00000300: 7465 7263 6f6e 5d20 7365 6e64 5f63 6d64  tercon] send_cmd
+00000310: 207b 7d20 6f73 6572 723a 207b 7d00 0520   {} oserr: {}.. 
+00000320: 5b69 6e74 6572 636f 6e5d 5b45 5252 5d20  [intercon][ERR] 
+00000330: 496e 7661 6c69 6420 686f 7374 3a20 7b7d  Invalid host: {}
+00000340: 0005 1843 6f6e 6e65 6374 696f 6e20 6973  ...Connection is
+00000350: 2062 7573 792e 2042 7965 2100 0534 5b69   busy. Bye!..4[i
+00000360: 6e74 6572 636f 6e5d 2070 726f 6d70 7420  ntercon] prompt 
+00000370: 6d69 736d 6174 6368 2c20 686f 7374 6e61  mismatch, hostna
+00000380: 6d65 3a20 7b7d 2070 726f 6d70 743a 207b  me: {} prompt: {
+00000390: 7d20 0005 0b5b 636f 6e66 6967 7572 655d  } ...[configure]
+000003a0: 0087 5c10 1c01 2632 2c2c 2c2c 6c89 7484  ..\...&2,,,,l.t.
+000003b0: 1484 1b80 511b 0216 3f80 1003 1004 2a02  ....Q...?.....*.
+000003c0: 1b05 1c03 1603 1c04 1604 5980 1006 2a01  ..........Y...*.
+000003d0: 1b07 1c06 1606 5980 1008 2a01 1b09 1c08  ......Y...*.....
+000003e0: 1608 5980 100a 2a01 1b0b 1c0a 160a 5980  ..Y...*.......Y.
+000003f0: 100c 2a01 1b0c 1c0c 160c 5980 100d 2a01  ..*.......Y...*.
+00000400: 1b0e 1c0d 160d 5954 3200 100f 3402 160f  ......YT2...4...
+00000410: 3201 1611 3202 1613 3203 161d 5163 0484  2...2...2...Qc..
+00000420: 0c08 1a0f 880a 2448 6440 8807 8432 8419  ......$Hd@...2..
+00000430: 1140 1641 100f 1642 2c00 161e 110a 1010  .@.A...B,.......
+00000440: 3401 1624 3200 161f 1143 3201 3401 1622  4..$2....C2.4.."
+00000450: 3202 1613 3203 1627 512a 0153 3304 162b  2...2..'Q*.S3..+
+00000460: 5163 0581 4811 0c1f 4780 0e24 2451 b018  Qc..H...G..$$Q..
+00000470: 2051 b018 2112 0d34 00b0 1812 5163 8160   Q..!..4....Qc.`
+00000480: 290e 2248 8014 232c 2223 02c1 1249 1206  )."H..#,"#...I..
+00000490: b1b0 3402 3401 4442 5263 5063 9318 f742  ..4.4.DBRcPc...B
+000004a0: 4213 4744 4580 1a80 0742 2a42 2f22 2d53  B.GDE....B*B/"-S
+000004b0: 2e2d 6e47 2a44 5656 2e2d 4c25 286c 464f  .-nG*DVV.-L%(lFO
+000004c0: 422c 51c3 120f 1422 b136 0143 e380 b1c3  B,Q....".6.C....
+000004d0: 120f 131e 1423 b351 3602 51de 44cb 8048  .....#.Q6.Q.D..H
+000004e0: 1712 03b1 120f 1324 8012 0434 04c4 b47f  .......$...4....
+000004f0: 5584 5580 55c1 4a30 5712 4adf 4469 c549  U.U.U.J0W.J.Di.I
+00000500: 1f12 0c14 2523 0314 18b5 3601 3601 5912  ....%#....6.6.Y.
+00000510: 0823 0414 18b1 b536 0234 0159 1015 6351  .#.....6.4.Y..cQ
+00000520: 51c5 2805 5d4a 015d 4247 120f 131e b355  Q.(.]J.]BG.....U
+00000530: c112 0f14 22b1 3601 4487 8149 5548 2312  ....".6.D..IUH#.
+00000540: 3f14 26b1 120f 1324 3602 5e51 6830 02b0  ?.&....$6.^Qh0..
+00000550: 1820 b018 21b0 1427 b2b3 3602 5e51 68c6  . ..!..'..6.^Qh.
+00000560: 4a2f 5712 4adf 4468 c549 1e12 0c14 2523  J/W.J.Dh.I....%#
+00000570: 0314 18b5 3601 3601 5912 0823 0414 18b1  ....6.6.Y..#....
+00000580: b536 0234 0159 51c6 5151 c528 055d 4a01  .6.4.YQ.QQ.(.]J.
+00000590: 5d51 b013 2144 53b0 1321 1428 3600 59b0  ]Q..!DS..!.(6.Y.
+000005a0: 1321 1429 3600 5e51 6859 5db3 51de d344  .!.)6.^QhY].Q..D
+000005b0: 4fb6 51de 4443 5142 41b1 120f 131e b356  O.Q.DCQBA......V
+000005c0: b663 1208 2305 1418 b136 0134 0159 1015  .c..#....6.4.Y..
+000005d0: 6389 70db 402a 2747 454b 804c 6060 282c  c.p.@*'GEK.L``(,
+000005e0: 2642 1f4c 292b 3026 4242 2f12 4c14 2ab1  &B.L)+0&BB/.L.*.
+000005f0: 3601 c1b0 142b 3600 5e51 6830 02c3 c423  6....+6.^Qh0...#
+00000600: 06b4 dd44 4251 63b2 51de 4366 b451 de43  ...DBQc.Q.Cf.Q.C
+00000610: 6112 4cb4 3401 142c 102d 1015 3602 142e  a.L.4..,.-..6...
+00000620: 3600 124c b234 0114 2f10 3036 0180 55d9  6..L.4../.06..U.
+00000630: 446e b013 2114 31b1 3601 59b0 1321 1432  Dn..!.1.6.Y..!.2
+00000640: 3600 5e51 6859 b014 2b10 33b4 3682 005e  6.^QhY..+.3.6..^
+00000650: 5168 3002 c3c5 b310 34d9 4442 5163 b363  Qh0.....4.DBQc.c
+00000660: 120c 1425 2307 1418 b2b4 3602 3601 5951  ...%#.....6.6.YQ
+00000670: 6388 78ce 4128 2b47 3380 6560 2043 2022  c.x.A(+G3.e` C "
+00000680: 2e23 244c 2e44 354c 2931 1015 c248 4db0  .#$L.D5L)1...HM.
+00000690: 1320 1435 2281 0036 015e 5168 c3b3 4344  . .5"..6.^Qh..CD
+000006a0: 40c9 8001 b314 3610 3736 0114 2e36 00c3  @.....6.76...6..
+000006b0: b151 de44 47b3 142e 3600 4241 b1c1 b2b3  .Q.DG...6.BA....
+000006c0: e5c2 b1b2 142e 3600 dd43 4c23 08b2 dd43  ......6..CL#...C
+000006d0: 4610 38b3 dd44 4340 5301 4a0d 5712 4adf  F.8..DC@S.J.W.J.
+000006e0: 4446 5940 4701 4a01 5d42 a17f b214 2cb1  DFY@G.J.]B....,.
+000006f0: 1015 3602 142c 1039 103a 3602 c2b2 b12a  ..6..,.9.:6....*
+00000700: 0263 8738 cf40 2211 4445 4680 7e80 0726  .c.8.@".DEF.~..&
+00000710: 2b25 2d2b 252d 2b32 b213 1247 5659 b214  +%-+%-+2...GVY..
+00000720: 13b0 b136 025e 5168 c3b3 51de 4475 123f  ...6.^Qh..Q.Du.?
+00000730: 1414 2281 1636 015e 5168 59b2 1413 b0b1  .."..6.^QhY.....
+00000740: 3602 5e51 68c3 b351 de44 5812 3f14 1422  6.^Qh..Q.DX.?.."
+00000750: 8116 3601 5e51 6859 b214 13b0 b136 025e  ..6.^QhY.....6.^
+00000760: 5168 c3b3 51de 4444 1015 4241 b3b2 1312  Qh..Q.DD..BA....
+00000770: 1816 515c 5db2 1312 1316 6386 446a 9e01  ..Q\].....c.Dj..
+00000780: 1344 4580 9280 0986 0725 2a37 2357 2c00  .DE......%*7#W,.
+00000790: 01b0 b120 0002 c212 0f34 00c3 1017 1418  ... .....4......
+000007a0: b234 0036 01c4 b313 1214 1910 1a12 1125  .4.6...........%
+000007b0: 0025 01b3 3403 101b b436 8400 c5b5 4457  .%..4....6....DW
+000007c0: 2c02 2300 1418 2500 2501 b436 0310 1c62  ,.#...%.%..6...b
+000007d0: b410 1b62 c642 4c2c 0223 0110 1c62 b410  ...b.BL,.#...b..
+000007e0: 1b62 c6b6 6301 8508 4a12 3b4d 4d80 9c20  .b..c...J.;MM.. 
+000007f0: 2f2a 3b25 0114 2f10 3a36 0180 5514 2e36  /*;%../.:6..U..6
+00000800: 00c2 120f 1422 2500 3601 445b 103c 1418  ....."%.6.D[.<..
+00000810: 1030 143d 2500 142f 1030 3601 7e51 2e02  .0.=%../.06.~Q..
+00000820: 5536 01b2 3602 6310 3c14 1825 0014 2c10  U6..6.c.<..%..,.
+00000830: 3e10 1536 02b2 3602 6358 0008 1d80 ad60  >..6..6.cX.....`
+00000840: 120f 131e 63                             ....c
```

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/InterpreterShell.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/InterpreterShell.mpy`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 00000030: 7300 0673 7973 000c 6366 6767 6574 000c  s..sys..cfgget..
 00000040: 6366 6770 7574 001a 436f 6e66 6967 4861  cfgput..ConfigHa
 00000050: 6e64 6c65 7200 1865 7865 635f 6c6d 5f63  ndler..exec_lm_c
 00000060: 6f72 6500 1654 6173 6b4d 616e 6167 6572  ore..TaskManager
 00000070: 001a 636f 6e73 6f6c 655f 7772 6974 6500  ..console_write.
 00000080: 1465 7272 6c6f 675f 6164 6400 0a44 6562  .errlog_add..Deb
 00000090: 7567 000a 7265 7365 7400 0e6d 6163 6869  ug..reset..machi
-000000a0: 6e65 000a 5368 656c 6c00 1031 2e31 382e  ne..Shell..1.18.
-000000b0: 322d 3000 230e 6d73 675f 6f62 6a00 0c64  2-0.#.msg_obj..d
+000000a0: 6e65 000a 5368 656c 6c00 1031 2e31 392e  ne..Shell..1.19.
+000000b0: 302d 3000 230e 6d73 675f 6f62 6a00 0c64  0-0.#.msg_obj..d
 000000c0: 6576 6669 6400 105f 5f64 6576 6669 6400  evfid..__devfid.
 000000d0: 0861 7574 6800 165f 5f61 7574 685f 6d6f  .auth..__auth_mo
 000000e0: 6465 000a 6877 7569 6400 0e5f 5f68 7775  de..hwuid..__hwu
 000000f0: 6964 0012 5f5f 6175 7468 5f6f 6b00 165f  id..__auth_ok.._
 00000100: 5f63 6f6e 665f 6d6f 6465 000e 7665 7273  _conf_mode..vers
 00000110: 696f 6e00 1c4d 4943 524f 535f 5645 5253  ion..MICROS_VERS
 00000120: 494f 4e00 8129 066d 7367 000c 7265 626f  ION..).msg..rebo
@@ -44,219 +44,219 @@
 000002b0: 656e 6578 7072 3e00 0470 7900 1468 6172  enexpr>..py..har
 000002c0: 645f 7265 7365 7400 2f2d 3582 2949 8177  d_reset./-5.)I.w
 000002d0: 0868 6172 6400 106d 7367 5f6c 6973 7400  .hard..msg_list.
 000002e0: 8157 822f 1461 7474 7269 6275 7465 7300  .W./.attributes.
 000002f0: 816d 0b16 6d6f 6475 6c65 5f6c 6973 7400  .m..module_list.
 00000300: 052a 4578 706f 7274 2073 7973 7465 6d20  .*Export system 
 00000310: 7665 7273 696f 6e20 746f 2063 6f6e 6669  version to confi
-00000320: 6720 6661 696c 6564 3a20 7b7d 0005 315b  g failed: {}..1[
-00000330: 5368 656c 6c2e 696e 6974 5d5b 4552 525d  Shell.init][ERR]
-00000340: 2073 7973 7465 6d20 7665 7273 696f 6e20   system version 
-00000350: 6578 706f 7274 2065 7272 6f72 3a20 7b7d  export error: {}
-00000360: 0005 177b 7d52 6562 6f6f 7420 6d69 6372  ...{}Reboot micr
-00000370: 4f53 2073 7973 7465 6d2e 0005 0b5b 7061  OS system....[pa
-00000380: 7373 776f 7264 5d20 0005 0c5b 636f 6e66  ssword] ...[conf
-00000390: 6967 7572 655d 2000 050f 4175 7468 4661  igure] ...AuthFa
-000003a0: 696c 6564 0a42 7965 2100 050b 6865 6c6c  iled.Bye!...hell
-000003b0: 6f3a 7b7d 3a7b 7d00 0524 5b4d 4943 524f  o:{}:{}..$[MICRO
-000003c0: 535d 2020 202d 2062 7569 6c74 2d69 6e20  S]   - built-in 
-000003d0: 7368 656c 6c20 636f 6d6d 616e 6473 0005  shell commands..
-000003e0: 3220 2020 6865 6c6c 6f20 2020 2d20 6865  2   hello   - he
-000003f0: 6c6c 6f20 6d73 6720 2d20 666f 7220 6465  llo msg - for de
-00000400: 7669 6365 2069 6465 6e74 6966 6963 6174  vice identificat
-00000410: 696f 6e00 0523 2020 2076 6572 7369 6f6e  ion..#   version
-00000420: 202d 2072 6574 7572 6e73 206d 6963 724f   - returns micrO
-00000430: 5320 7665 7273 696f 6e00 052a 2020 2065  S version..*   e
-00000440: 7869 7420 2020 202d 2065 7869 7420 6672  xit    - exit fr
-00000450: 6f6d 2073 6865 6c6c 2073 6f63 6b65 7420  om shell socket 
-00000460: 7072 6f6d 7074 0005 4120 2020 7265 626f  prompt..A   rebo
-00000470: 6f74 2020 2d20 7379 7374 656d 2073 6f66  ot  - system sof
-00000480: 7420 7265 626f 6f74 2028 766d 292c 2068  t reboot (vm), h
-00000490: 6172 6420 7265 626f 6f74 2028 6877 293a  ard reboot (hw):
-000004a0: 2072 6562 6f6f 7420 2d68 0005 4020 2020   reboot -h..@   
-000004b0: 7765 6272 6570 6c20 2d20 7374 6172 7420  webrepl - start 
-000004c0: 7765 6272 6570 6c2c 2066 6f72 2066 696c  webrepl, for fil
-000004d0: 6520 7472 616e 7366 6572 7320 7573 6520  e transfers use 
-000004e0: 7769 7468 202d 2d75 7064 6174 6500 052f  with --update../
-000004f0: 5b43 4f4e 465d 2043 6f6e 6669 6775 7265  [CONF] Configure
-00000500: 206d 6f64 6520 2d20 6275 696c 742d 696e   mode - built-in
-00000510: 2073 6865 6c6c 2063 6f6d 6d61 6e64 7300   shell commands.
-00000520: 051e 2020 636f 6e66 2020 2020 2020 202d  ..  conf       -
-00000530: 2045 6e74 6572 2063 6f6e 6620 6d6f 6465   Enter conf mode
-00000540: 0005 1e20 2020 2064 756d 7020 2020 2020  ...    dump     
-00000550: 2020 2d20 4475 6d70 2061 6c6c 2064 6174    - Dump all dat
-00000560: 6100 051a 2020 2020 6b65 7920 2020 2020  a...    key     
-00000570: 2020 202d 2047 6574 2076 616c 7565 0005     - Get value..
-00000580: 1a20 2020 206b 6579 2076 616c 7565 2020  .    key value  
-00000590: 2d20 5365 7420 7661 6c75 6500 051d 2020  - Set value...  
-000005a0: 6e6f 636f 6e66 2020 2020 202d 2045 7869  noconf     - Exi
-000005b0: 7420 636f 6e66 206d 6f64 6500 0548 5b54  t conf mode..H[T
-000005c0: 4153 4b5d 2070 6f73 7466 6978 3a20 2678  ASK] postfix: &x
-000005d0: 202d 206f 6e65 2d74 696d 652c 2020 2626   - one-time,  &&
-000005e0: 7820 2d20 7065 7269 6f64 6963 2c20 783a  x - periodic, x:
-000005f0: 2077 6169 7420 6d73 205b 7820 6d69 6e3a   wait ms [x min:
-00000600: 2032 306d 735d 0005 2c20 2074 6173 6b20   20ms]..,  task 
-00000610: 6c69 7374 2020 2020 2020 2020 202d 206c  list         - l
-00000620: 6973 7420 7461 736b 7320 7769 7468 203c  ist tasks with <
-00000630: 7461 673e 7300 051f 2020 7461 736b 206b  tag>s...  task k
-00000640: 696c 6c20 3c74 6167 3e20 2020 2d20 7374  ill <tag>   - st
-00000650: 6f70 2074 6173 6b00 0526 2020 7461 736b  op task..&  task
-00000660: 2073 686f 7720 3c74 6167 3e20 2020 2d20   show <tag>   - 
-00000670: 7368 6f77 2074 6173 6b20 6f75 7470 7574  show task output
-00000680: 0005 1a5b 4558 4543 5d20 436f 6d6d 616e  ...[EXEC] Comman
-00000690: 6420 6d6f 6465 2028 4c4d 7329 3a00 0522  d mode (LMs):.."
-000006a0: 2020 2068 656c 7020 6c6d 2020 2d20 6c69     help lm  - li
-000006b0: 7374 2041 4c4c 204c 6f61 644d 6f64 756c  st ALL LoadModul
-000006c0: 6573 0005 285b 4552 524f 525d 2065 7865  es..([ERROR] exe
-000006d0: 635f 6c6d 5f73 6865 6c6c 2069 6e74 6572  c_lm_shell inter
-000006e0: 6e61 6c20 6572 726f 723a 207b 7d00 050c  nal error: {}...
-000006f0: 2020 7b7d 7b7d 3a7b 7d20 7b7d 0005 1b6e    {}{}:{} {}...n
-00000700: 6f64 655f 636f 6e66 6967 2077 7269 7465  ode_config write
-00000710: 2065 7272 6f72 3a20 7b7d 0005 0b49 6e76   error: {}...Inv
-00000720: 616c 6964 206b 6579 0005 0e46 6169 6c65  alid key...Faile
-00000730: 6420 746f 2073 6176 6500 0538 2053 7461  d to save..8 Sta
-00000740: 7274 206d 6963 726f 7079 7468 6f6e 2057  rt micropython W
-00000750: 4542 5245 504c 202d 2066 696c 6520 7472  EBREPL - file tr
-00000760: 616e 7366 6572 2061 6e64 2064 6562 7567  ansfer and debug
-00000770: 6769 6e67 0005 2c20 205b 695d 2072 6573  ging..,  [i] res
-00000780: 7461 7274 206d 6163 6869 6e65 2073 686f  tart machine sho
-00000790: 7274 6375 743a 2069 6d70 6f72 7420 7265  rtcut: import re
-000007a0: 7365 7400 0537 2020 436f 6e6e 6563 7420  set..7  Connect 
-000007b0: 6f76 6572 2068 7474 703a 2f2f 6d69 6372  over http://micr
-000007c0: 6f70 7974 686f 6e2e 6f72 672f 7765 6272  opython.org/webr
-000007d0: 6570 6c2f 237b 7d3a 3832 3636 2f00 051b  epl/#{}:8266/...
-000007e0: 2020 095b 215d 2077 6562 7265 706c 2070    .[!] webrepl p
-000007f0: 6173 7377 6f72 643a 207b 7d00 0524 2020  assword: {}..$  
-00000800: 5265 7374 6172 7420 6e6f 6465 2074 6865  Restart node the
-00000810: 6e20 7374 6172 7420 7765 6272 6570 6c2e  n start webrepl.
-00000820: 2e2e 0005 205b 4552 525d 2077 6869 6c65  .... [ERR] while
-00000830: 2073 7461 7274 696e 6720 7765 6272 6570   starting webrep
-00000840: 6c3a 207b 7d00 050f 6d69 6372 4f53 6973  l: {}...micrOSis
-00000850: 5468 6542 6573 7400 051f 5b7b 7d5d 2053  TheBest...[{}] S
-00000860: 484f 5720 4c4d 2050 4152 5345 5220 5741  HOW LM PARSER WA
-00000870: 524e 494e 473a 207b 7d00 865c 1014 0180  RNING: {}..\....
-00000880: 0d2c 2c32 2c32 8c07 8010 022a 011b 031c  .,,2,2.....*....
-00000890: 0216 0259 8010 042a 011b 051c 0416 0459  ...Y...*.......Y
-000008a0: 8010 0610 072a 021b 081c 0616 061c 0716  .....*..........
-000008b0: 0759 8010 092a 011b 0a1c 0916 0959 8010  .Y...*.......Y..
-000008c0: 0b10 0c2a 021b 0d1c 0b16 0b1c 0c16 0c59  ...*...........Y
-000008d0: 8010 0e2a 011b 0f1c 0e16 5e59 5432 0010  ...*......^YT2..
-000008e0: 1034 0216 1051 6301 8704 1030 1088 1a44  .4...Qc....0...D
-000008f0: 8814 8407 6440 8809 6460 840e 8409 846a  ....d@..d`.....j
-00000900: 8825 8c21 115f 1660 1010 1661 1011 161d  .%.!._.`...a....
-00000910: 512a 0153 3300 1612 3201 161f 3202 160e  Q*.S3...2...2...
-00000920: 502a 0153 3303 1620 3204 1625 3205 1627  P*.S3.. 2..%2..'
-00000930: 3206 162b 3207 162c 1162 3208 3401 163a  2..+2..,.b2.4..:
-00000940: 1162 502a 0153 3309 3401 1638 1162 502a  .bP*.S3.4..8.bP*
-00000950: 0153 330a 3401 1631 5163 0b87 28ca 0320  .S3.4..1Qc..(.. 
-00000960: 1258 1380 1d60 2044 2929 4924 4422 562c  .X...` D))I$D"V,
-00000970: b1b0 1813 1206 1014 3401 b018 1512 0610  ........4.......
-00000980: 1634 01b0 1817 1206 1018 3401 b018 1950  .4........4....P
-00000990: b018 1a50 b018 1b48 0d12 0710 1c12 1013  ...P...H........
-000009a0: 1d34 0259 4a2a 5712 63df 4463 c249 1912  .4.YJ*W.c.Dc.I..
-000009b0: 0b23 0014 1eb2 3601 3401 5912 0c23 0114  .#....6.4.Y..#..
-000009c0: 1eb2 3601 3401 5951 51c2 2802 5d4a 015d  ..6.4.YQQ.(.]J.]
-000009d0: 5163 8208 3610 1f58 1f80 3120 224a 4809  Qc..6..X..1 "JH.
-000009e0: b014 13b1 3601 594a 0a59 1264 b134 0159  ....6.YJ.Y.d.4.Y
-000009f0: 4a01 5d51 6381 1011 0c0e 5880 3820 2450  J.]Qc.....X.8 $P
-00000a00: b018 1a50 b018 1b51 6384 20ba 0116 2058  ...P...Qc. ... X
-00000a10: 6580 3d20 3528 2325 2bb0 141f 2302 141e  e.= 5(#%+...#...
-00000a20: b144 4410 2142 4210 2236 0136 0159 b014  .DD.!BB."6.6.Y..
-00000a30: 1f10 2336 0159 b144 4512 5e34 0059 8010  ..#6.Y.DE.^4.Y..
-00000a40: 242a 011b 0f1c 24c2 59b2 3400 5951 6383  $*....$.Y.4.YQc.
-00000a50: 1039 0e25 5880 4620 312c b013 1744 49b0  .9.%X.F 1,...DI.
-00000a60: 131a 4344 2303 4242 1022 c1b0 131b 4444  ..CD#.BB."....DD
-00000a70: 2304 4242 1022 c210 2614 1eb1 b2b0 1315  #.BB."..&.......
-00000a80: 3603 6385 082a 1c27 5866 804c 404a 272b  6.c..*.'Xf.L@J'+
-00000a90: 2428 2628 26b0 1317 4477 b013 1a43 7212  $(&(&...Dw...Cr.
-00000aa0: 0610 2834 01c2 b2b1 8055 1429 3600 d944  ..(4.....U.)6..D
-00000ab0: 5252 b018 1ab0 141f 102a 3601 5952 2b00  RR.......*6.YR+.
-00000ac0: 2a02 63b0 141f 2305 3601 5950 2b00 2a02  *.c...#.6.YP+.*.
-00000ad0: 6352 b12a 0263 8178 3212 2b58 1f80 5a60  cR.*.c.x2.+X..Z`
-00000ae0: 2027 2bb0 142c b136 01c2 b014 1fb0 1425   '+..,.6.......%
-00000af0: 3600 3601 59b2 63a4 00ea 0286 022c 581f  6.6.Y.c......,X.
-00000b00: 8063 800b 5222 8a08 4832 422a 2322 2962  .c..R"..H2B*#")b
-00000b10: 482e 6228 2251 2247 2b31 306d 2b24 222b  H.b("Q"G+10m+$"+
-00000b20: 2462 2928 2828 2828 2828 2828 2828 2828  $b)(((((((((((((
-00000b30: 2828 2828 282a 2d70 204e 4b60 4042 592d  (((((*-p NK`@BY-
-00000b40: b151 de43 4d12 67b1 1429 3600 3401 80d9  .Q.CM.g..)6.4...
-00000b50: 4442 5263 b114 2936 0014 2d36 00c2 b280  DBRc..)6..-6....
-00000b60: 5510 2ed9 4454 b014 1f23 0614 1eb0 1315  U...DT...#......
-00000b70: b013 1936 0236 0159 5263 b014 27b2 3601  ...6.6.YRc..'.6.
-00000b80: 3002 c3c2 b343 4250 6312 67b2 3401 80d9  0....CBPc.g.4...
-00000b90: 4442 5263 b280 5510 1cd9 4450 b014 1f12  DBRc..U...DP....
-00000ba0: 6812 1013 1d34 0136 0159 5263 b280 5510  h....4.6.YRc..U.
-00000bb0: 20d9 445c 50c4 1267 b234 0182 db44 4a10   .D\P..g.4...DJ.
-00000bc0: 2fb2 8155 dd44 4252 c4b0 1420 b436 0159  /..U.DBR... .6.Y
-00000bd0: b280 5514 3010 3136 0144 6e12 67b2 3401  ..U.0.16.Dn.g.4.
-00000be0: 82d9 4458 1032 b281 55dd 4450 1210 1431  ..DX.2..U.DP...1
-00000bf0: 1013 b013 1f10 3352 3684 0059 1210 1431  ......3R6..Y...1
-00000c00: 1013 b013 1f36 8200 59b2 8055 1430 1034  .....6..Y..U.0.4
-00000c10: 3601 4446 52b0 181b 5263 b280 5514 3010  6.DFR...Rc..U.0.
-00000c20: 3536 0144 4650 b018 1b52 63b2 8055 1036  56.DFP...Rc..U.6
-00000c30: d944 b781 b014 1f23 0736 0159 b014 1f23  .D.....#.6.Y...#
-00000c40: 0836 0159 b014 1f23 0936 0159 b014 1f23  .6.Y...#.6.Y...#
-00000c50: 0a36 0159 b014 1f23 0b36 0159 b014 1f23  .6.Y...#.6.Y...#
-00000c60: 0c36 0159 b014 1f23 0d36 0159 b014 1f23  .6.Y...#.6.Y...#
-00000c70: 0e36 0159 b014 1f23 0f36 0159 b014 1f23  .6.Y...#.6.Y...#
-00000c80: 1036 0159 b014 1f23 1136 0159 b014 1f23  .6.Y...#.6.Y...#
-00000c90: 1236 0159 b014 1f23 1336 0159 b014 1f23  .6.Y...#.6.Y...#
-00000ca0: 1436 0159 b014 1f23 1536 0159 b014 1f23  .6.Y...#.6.Y...#
-00000cb0: 1636 0159 b014 1f23 1736 0159 b014 1f23  .6.Y...#.6.Y...#
-00000cc0: 1836 0159 1037 1268 b234 01dd 444d 1210  .6.Y.7.h.4..DM..
-00000cd0: 1438 1013 b013 1f36 8200 6312 1014 3810  .8.....6..c...8.
-00000ce0: 13b0 131f 1039 5236 8400 63b0 131b 4454  .....9R6..c...DT
-00000cf0: 1267 b234 0180 d844 4b12 1014 3ab0 131f  .g.4...DK...:...
-00000d00: b236 0263 4810 1209 103b b210 3cb0 131f  .6.cH....;..<...
-00000d10: 3484 0063 4a21 5712 63df 445a c549 10b0  4..cJ!W.c.DZ.I..
-00000d20: 141f 2319 141e b536 0136 0159 5063 5151  ..#....6.6.YPcQQ
-00000d30: c528 055d 4a01 5d51 638d 0092 1230 3a13  .(.]J.]Qc....0:.
-00000d40: 6980 ce60 602a 482f 2836 422b 424a 244d  i..``*H/(6B+BJ$M
-00000d50: 2256 2b4b 302c 1267 b134 0181 d944 c480  "V+K0,.g.4...D..
-00000d60: b180 5510 3dd9 446f 1206 3400 143e 3600  ..U.=.Do..4..>6.
-00000d70: 5f4b 2230 02c2 c38a 1267 b234 01f3 c4b0  _K"0.....g.4....
-00000d80: 231a 141e b210 3fb4 f410 3f87 f4b3 3604  #.....?...?...6.
-00000d90: 3401 5942 1c52 63b0 1206 b180 5534 0134  4.YB.Rc.....U4.4
-00000da0: 0159 5263 1267 b134 0182 db44 db80 b180  .YRc.g.4...D....
-00000db0: 55c2 103f 1440 b181 512e 0255 3601 c348  U..?.@..Q..U6..H
-00000dc0: 0d12 07b2 b310 4152 3482 02c5 4a1f 5712  ......AR4...J.W.
-00000dd0: 63df 4458 c649 0eb0 231b 141e b636 0134  c.DX.I..#....6.4
-00000de0: 0159 50c5 5151 c628 065d 4a01 5d12 06b2  .YP.QQ.(.]J.]...
-00000df0: 3401 51de 4444 231c 4242 231d c7b0 b544  4.Q.DD#.BB#....D
-00000e00: 4410 4242 41b7 3401 5952 6383 64b2 019a  D.BBA.4.YRc.d...
-00000e10: 0138 1339 80f3 6020 8514 2328 2c45 0004  .8.9..` ..#(,E..
-00000e20: b020 0001 c2b1 4459 1204 1443 3600 2704  . ....DY...C6.'.
-00000e30: b420 0101 1202 3400 5e34 01c3 b2b3 3401  . ....4.^4....4.
-00000e40: 63b2 1202 3400 3401 6302 8f4c a212 2c4c  c...4.4.c..L..,L
-00000e50: 6b6c 80f8 2b32 232c 291f 2424 2a23 2326  kl..+2#,).$$*##&
-00000e60: 3b1f 572d 2e32 00b1 5e34 015f 4bd4 01c2  ;.W-.2..^4._K...
-00000e70: b214 4d10 4e10 2236 0214 2d10 4f36 0180  ..M.N."6..-.O6..
-00000e80: 55c3 489a 0125 0010 5014 1eb3 3601 3401  U.H..%..P...6.4.
-00000e90: 59b2 1451 1052 3601 4467 2500 1053 141e  Y..Q.R6.Dg%..S..
-00000ea0: 103f 1267 b214 4d10 4e10 2236 0214 2d10  .?.g..M.N."6..-.
-00000eb0: 4f36 0180 5534 01f4 3601 3401 5940 ac7f  O6..U4..6.4.Y@..
-00000ec0: 0112 6ab2 1054 3402 4751 c423 24c5 42c5  ..j..T4.GQ.#$.B.
-00000ed0: 80b4 1455 3600 c5b5 1429 3600 1430 1056  ...U6....)6..0.V
-00000ee0: 3601 4472 1057 b5dd d344 6b10 58b5 ddd3  6.Dr.W...Dk.X...
-00000ef0: 4464 2500 1059 141e 103f 1267 b334 01f4  Dd%..Y...?.g.4..
-00000f00: b514 4d10 5a10 2236 0214 2d10 5b36 0180  ..M.Z."6..-.[6..
-00000f10: 5536 0234 0159 b543 b77f 515c 5d4a 2157  U6.4.Y.C..Q\]J!W
-00000f20: 1263 df44 5ac6 4910 2500 2325 141e b2b6  .c.DZ.I.%.#%....
-00000f30: 3602 3401 5950 6351 51c6 2806 5d4a 015d  6.4.YPcQQ.(.]J.]
-00000f40: 42a9 7e52 6301 8238 c140 085c 6b80 f853  B.~Rc..8.@.\k..S
-00000f50: b053 534b 18c1 b114 3010 4e36 0144 34b1  .SSK....0.N6.D4.
-00000f60: 1451 105d 3601 442b b167 5942 2651 6382  .Q.]6.D+.gYB&Qc.
-00000f70: 20ca 400a 5c6b 6b90 0d53 b153 534b 14c2   .@.\kk..S.SSK..
-00000f80: b214 2d10 4f36 0180 5525 00dd 442f b267  ..-.O6..U%..D/.g
-00000f90: 5942 2a51 638c 00e2 032c 3113 3390 144b  YB*Qc....,1.3..K
-00000fa0: 2626 3130 2326 2643 2b2b 2522 255d 2825  &&10#&&C++%"%](%
-00000fb0: 8010 442a 011b 451c 44c2 59b0 231e 3401  ..D*..E.D.Y.#.4.
-00000fc0: 59b0 231f 3401 59b0 2320 141e b234 0081  Y.#.4.Y.# ...4..
-00000fd0: 5580 5536 0134 0159 b023 2114 1e12 0610  U.U6.4.Y.#!.....
-00000fe0: 2834 0136 0134 0159 b144 46b0 2322 3401  (4.6.4.Y.DF.#"4.
-00000ff0: 59b0 1046 3401 59b1 445b 126a 1047 1048  Y..F4.Y.D[.j.G.H
-00001000: 3402 470a c3b3 1449 1031 3601 5951 5c5d  4.G....I.16.YQ\]
-00001010: 125e 3400 5948 1980 511b 31c4 b0b4 144a  .^4.YH..Q.1....J
-00001020: 104b 1206 1028 3401 3682 0034 0159 4a25  .K...(4.6..4.YJ%
-00001030: 5712 63df 445e c549 1423 2314 1eb5 3601  W.c.D^.I.##...6.
-00001040: c6b0 b634 0159 120c b634 0159 5151 c528  ...4.Y...4.YQQ.(
-00001050: 055d 4a01 5d51 63                        .]J.]Qc
+00000320: 6720 6661 696c 6564 3a20 7b7d 0005 2c5b  g failed: {}..,[
+00000330: 5368 656c 6c5d 5b45 5252 5d20 7379 7374  Shell][ERR] syst
+00000340: 656d 2076 6572 7369 6f6e 2065 7870 6f72  em version expor
+00000350: 7420 6572 726f 723a 207b 7d00 0517 7b7d  t error: {}...{}
+00000360: 5265 626f 6f74 206d 6963 724f 5320 7379  Reboot micrOS sy
+00000370: 7374 656d 2e00 050b 5b70 6173 7377 6f72  stem....[passwor
+00000380: 645d 2000 050c 5b63 6f6e 6669 6775 7265  d] ...[configure
+00000390: 5d20 0005 0f41 7574 6846 6169 6c65 640a  ] ...AuthFailed.
+000003a0: 4279 6521 0005 0b68 656c 6c6f 3a7b 7d3a  Bye!...hello:{}:
+000003b0: 7b7d 0005 245b 4d49 4352 4f53 5d20 2020  {}..$[MICROS]   
+000003c0: 2d20 6275 696c 742d 696e 2073 6865 6c6c  - built-in shell
+000003d0: 2063 6f6d 6d61 6e64 7300 0532 2020 2068   commands..2   h
+000003e0: 656c 6c6f 2020 202d 2068 656c 6c6f 206d  ello   - hello m
+000003f0: 7367 202d 2066 6f72 2064 6576 6963 6520  sg - for device 
+00000400: 6964 656e 7469 6669 6361 7469 6f6e 0005  identification..
+00000410: 2320 2020 7665 7273 696f 6e20 2d20 7265  #   version - re
+00000420: 7475 726e 7320 6d69 6372 4f53 2076 6572  turns micrOS ver
+00000430: 7369 6f6e 0005 2a20 2020 6578 6974 2020  sion..*   exit  
+00000440: 2020 2d20 6578 6974 2066 726f 6d20 7368    - exit from sh
+00000450: 656c 6c20 736f 636b 6574 2070 726f 6d70  ell socket promp
+00000460: 7400 0541 2020 2072 6562 6f6f 7420 202d  t..A   reboot  -
+00000470: 2073 7973 7465 6d20 736f 6674 2072 6562   system soft reb
+00000480: 6f6f 7420 2876 6d29 2c20 6861 7264 2072  oot (vm), hard r
+00000490: 6562 6f6f 7420 2868 7729 3a20 7265 626f  eboot (hw): rebo
+000004a0: 6f74 202d 6800 0540 2020 2077 6562 7265  ot -h..@   webre
+000004b0: 706c 202d 2073 7461 7274 2077 6562 7265  pl - start webre
+000004c0: 706c 2c20 666f 7220 6669 6c65 2074 7261  pl, for file tra
+000004d0: 6e73 6665 7273 2075 7365 2077 6974 6820  nsfers use with 
+000004e0: 2d2d 7570 6461 7465 0005 2f5b 434f 4e46  --update../[CONF
+000004f0: 5d20 436f 6e66 6967 7572 6520 6d6f 6465  ] Configure mode
+00000500: 202d 2062 7569 6c74 2d69 6e20 7368 656c   - built-in shel
+00000510: 6c20 636f 6d6d 616e 6473 0005 1e20 2063  l commands...  c
+00000520: 6f6e 6620 2020 2020 2020 2d20 456e 7465  onf       - Ente
+00000530: 7220 636f 6e66 206d 6f64 6500 051e 2020  r conf mode...  
+00000540: 2020 6475 6d70 2020 2020 2020 202d 2044    dump       - D
+00000550: 756d 7020 616c 6c20 6461 7461 0005 1a20  ump all data... 
+00000560: 2020 206b 6579 2020 2020 2020 2020 2d20     key        - 
+00000570: 4765 7420 7661 6c75 6500 051a 2020 2020  Get value...    
+00000580: 6b65 7920 7661 6c75 6520 202d 2053 6574  key value  - Set
+00000590: 2076 616c 7565 0005 1d20 206e 6f63 6f6e   value...  nocon
+000005a0: 6620 2020 2020 2d20 4578 6974 2063 6f6e  f     - Exit con
+000005b0: 6620 6d6f 6465 0005 485b 5441 534b 5d20  f mode..H[TASK] 
+000005c0: 706f 7374 6669 783a 2026 7820 2d20 6f6e  postfix: &x - on
+000005d0: 652d 7469 6d65 2c20 2026 2678 202d 2070  e-time,  &&x - p
+000005e0: 6572 696f 6469 632c 2078 3a20 7761 6974  eriodic, x: wait
+000005f0: 206d 7320 5b78 206d 696e 3a20 3230 6d73   ms [x min: 20ms
+00000600: 5d00 052c 2020 7461 736b 206c 6973 7420  ]..,  task list 
+00000610: 2020 2020 2020 2020 2d20 6c69 7374 2074          - list t
+00000620: 6173 6b73 2077 6974 6820 3c74 6167 3e73  asks with <tag>s
+00000630: 0005 1f20 2074 6173 6b20 6b69 6c6c 203c  ...  task kill <
+00000640: 7461 673e 2020 202d 2073 746f 7020 7461  tag>   - stop ta
+00000650: 736b 0005 2620 2074 6173 6b20 7368 6f77  sk..&  task show
+00000660: 203c 7461 673e 2020 202d 2073 686f 7720   <tag>   - show 
+00000670: 7461 736b 206f 7574 7075 7400 051a 5b45  task output...[E
+00000680: 5845 435d 2043 6f6d 6d61 6e64 206d 6f64  XEC] Command mod
+00000690: 6520 284c 4d73 293a 0005 2220 2020 6865  e (LMs):.."   he
+000006a0: 6c70 206c 6d20 202d 206c 6973 7420 414c  lp lm  - list AL
+000006b0: 4c20 4c6f 6164 4d6f 6475 6c65 7300 0528  L LoadModules..(
+000006c0: 5b45 5252 4f52 5d20 6578 6563 5f6c 6d5f  [ERROR] exec_lm_
+000006d0: 7368 656c 6c20 696e 7465 726e 616c 2065  shell internal e
+000006e0: 7272 6f72 3a20 7b7d 0005 0c20 207b 7d7b  rror: {}...  {}{
+000006f0: 7d3a 7b7d 207b 7d00 051b 6e6f 6465 5f63  }:{} {}...node_c
+00000700: 6f6e 6669 6720 7772 6974 6520 6572 726f  onfig write erro
+00000710: 723a 207b 7d00 050b 496e 7661 6c69 6420  r: {}...Invalid 
+00000720: 6b65 7900 050e 4661 696c 6564 2074 6f20  key...Failed to 
+00000730: 7361 7665 0005 3820 5374 6172 7420 6d69  save..8 Start mi
+00000740: 6372 6f70 7974 686f 6e20 5745 4252 4550  cropython WEBREP
+00000750: 4c20 2d20 6669 6c65 2074 7261 6e73 6665  L - file transfe
+00000760: 7220 616e 6420 6465 6275 6767 696e 6700  r and debugging.
+00000770: 052c 2020 5b69 5d20 7265 7374 6172 7420  .,  [i] restart 
+00000780: 6d61 6368 696e 6520 7368 6f72 7463 7574  machine shortcut
+00000790: 3a20 696d 706f 7274 2072 6573 6574 0005  : import reset..
+000007a0: 3720 2043 6f6e 6e65 6374 206f 7665 7220  7  Connect over 
+000007b0: 6874 7470 3a2f 2f6d 6963 726f 7079 7468  http://micropyth
+000007c0: 6f6e 2e6f 7267 2f77 6562 7265 706c 2f23  on.org/webrepl/#
+000007d0: 7b7d 3a38 3236 362f 0005 1b20 2009 5b21  {}:8266/...  .[!
+000007e0: 5d20 7765 6272 6570 6c20 7061 7373 776f  ] webrepl passwo
+000007f0: 7264 3a20 7b7d 0005 2420 2052 6573 7461  rd: {}..$  Resta
+00000800: 7274 206e 6f64 6520 7468 656e 2073 7461  rt node then sta
+00000810: 7274 2077 6562 7265 706c 2e2e 2e00 0520  rt webrepl..... 
+00000820: 5b45 5252 5d20 7768 696c 6520 7374 6172  [ERR] while star
+00000830: 7469 6e67 2077 6562 7265 706c 3a20 7b7d  ting webrepl: {}
+00000840: 0005 0f6d 6963 724f 5369 7354 6865 4265  ...micrOSisTheBe
+00000850: 7374 0005 1f5b 7b7d 5d20 5348 4f57 204c  st...[{}] SHOW L
+00000860: 4d20 5041 5253 4552 2057 4152 4e49 4e47  M PARSER WARNING
+00000870: 3a20 7b7d 0086 5c10 1401 800d 2c2c 322c  : {}..\.....,,2,
+00000880: 328c 0780 1002 2a01 1b03 1c02 1602 5980  2.....*.......Y.
+00000890: 1004 2a01 1b05 1c04 1604 5980 1006 1007  ..*.......Y.....
+000008a0: 2a02 1b08 1c06 1606 1c07 1607 5980 1009  *...........Y...
+000008b0: 2a01 1b0a 1c09 1609 5980 100b 100c 2a02  *.......Y.....*.
+000008c0: 1b0d 1c0b 160b 1c0c 160c 5980 100e 2a01  ..........Y...*.
+000008d0: 1b0f 1c0e 165e 5954 3200 1010 3402 1610  .....^YT2...4...
+000008e0: 5163 0187 0410 3010 881a 4488 1484 0764  Qc....0...D....d
+000008f0: 4088 0964 6084 0e84 0984 6a88 258c 2111  @..d`.....j.%.!.
+00000900: 5f16 6010 1016 6110 1116 1d51 2a01 5333  _.`...a....Q*.S3
+00000910: 0016 1232 0116 1f32 0216 0e50 2a01 5333  ...2...2...P*.S3
+00000920: 0316 2032 0416 2532 0516 2732 0616 2b32  .. 2..%2..'2..+2
+00000930: 0716 2c11 6232 0834 0116 3a11 6250 2a01  ..,.b2.4..:.bP*.
+00000940: 5333 0934 0116 3811 6250 2a01 5333 0a34  S3.4..8.bP*.S3.4
+00000950: 0116 3151 630b 8728 ca03 2012 5813 801d  ..1Qc..(.. .X...
+00000960: 6020 4429 2949 2444 2256 2cb1 b018 1312  ` D))I$D"V,.....
+00000970: 0610 1434 01b0 1815 1206 1016 3401 b018  ...4........4...
+00000980: 1712 0610 1834 01b0 1819 50b0 181a 50b0  .....4....P...P.
+00000990: 181b 480d 1207 101c 1210 131d 3402 594a  ..H.........4.YJ
+000009a0: 2a57 1263 df44 63c2 4919 120b 2300 141e  *W.c.Dc.I...#...
+000009b0: b236 0134 0159 120c 2301 141e b236 0134  .6.4.Y..#....6.4
+000009c0: 0159 5151 c228 025d 4a01 5d51 6382 0836  .YQQ.(.]J.]Qc..6
+000009d0: 101f 581f 8031 2022 4a48 09b0 1413 b136  ..X..1 "JH.....6
+000009e0: 0159 4a0a 5912 64b1 3401 594a 015d 5163  .YJ.Y.d.4.YJ.]Qc
+000009f0: 8110 110c 0e58 8038 2024 50b0 181a 50b0  .....X.8 $P...P.
+00000a00: 181b 5163 8420 ba01 1620 5865 803d 2035  ..Qc. ... Xe.= 5
+00000a10: 2823 252b b014 1f23 0214 1eb1 4444 1021  (#%+...#....DD.!
+00000a20: 4242 1022 3601 3601 59b0 141f 1023 3601  BB."6.6.Y....#6.
+00000a30: 59b1 4445 125e 3400 5980 1024 2a01 1b0f  Y.DE.^4.Y..$*...
+00000a40: 1c24 c259 b234 0059 5163 8310 390e 2558  .$.Y.4.YQc..9.%X
+00000a50: 8046 2031 2cb0 1317 4449 b013 1a43 4423  .F 1,...DI...CD#
+00000a60: 0342 4210 22c1 b013 1b44 4423 0442 4210  .BB."....DD#.BB.
+00000a70: 22c2 1026 141e b1b2 b013 1536 0363 8508  "..&.......6.c..
+00000a80: 2a1c 2758 6680 4c40 4a27 2b24 2826 2826  *.'Xf.L@J'+$(&(&
+00000a90: b013 1744 77b0 131a 4372 1206 1028 3401  ...Dw...Cr...(4.
+00000aa0: c2b2 b180 5514 2936 00d9 4452 52b0 181a  ....U.)6..DRR...
+00000ab0: b014 1f10 2a36 0159 522b 002a 0263 b014  ....*6.YR+.*.c..
+00000ac0: 1f23 0536 0159 502b 002a 0263 52b1 2a02  .#.6.YP+.*.cR.*.
+00000ad0: 6381 7832 122b 581f 805a 6020 272b b014  c.x2.+X..Z` '+..
+00000ae0: 2cb1 3601 c2b0 141f b014 2536 0036 0159  ,.6.......%6.6.Y
+00000af0: b263 a400 ea02 8602 2c58 1f80 6380 0b52  .c......,X..c..R
+00000b00: 228a 0848 3242 2a23 2229 6248 2e62 2822  "..H2B*#")bH.b("
+00000b10: 5122 472b 3130 6d2b 2422 2b24 6229 2828  Q"G+10m+$"+$b)((
+00000b20: 2828 2828 2828 2828 2828 2828 2828 2828  ((((((((((((((((
+00000b30: 2a2d 7020 4e4b 6040 4259 2db1 51de 434d  *-p NK`@BY-.Q.CM
+00000b40: 1267 b114 2936 0034 0180 d944 4252 63b1  .g..)6.4...DBRc.
+00000b50: 1429 3600 142d 3600 c2b2 8055 102e d944  .)6..-6....U...D
+00000b60: 54b0 141f 2306 141e b013 15b0 1319 3602  T...#.........6.
+00000b70: 3601 5952 63b0 1427 b236 0130 02c3 c2b3  6.YRc..'.6.0....
+00000b80: 4342 5063 1267 b234 0180 d944 4252 63b2  CBPc.g.4...DBRc.
+00000b90: 8055 101c d944 50b0 141f 1268 1210 131d  .U...DP....h....
+00000ba0: 3401 3601 5952 63b2 8055 1020 d944 5c50  4.6.YRc..U. .D\P
+00000bb0: c412 67b2 3401 82db 444a 102f b281 55dd  ..g.4...DJ./..U.
+00000bc0: 4442 52c4 b014 20b4 3601 59b2 8055 1430  DBR... .6.Y..U.0
+00000bd0: 1031 3601 446e 1267 b234 0182 d944 5810  .16.Dn.g.4...DX.
+00000be0: 32b2 8155 dd44 5012 1014 3110 13b0 131f  2..U.DP...1.....
+00000bf0: 1033 5236 8400 5912 1014 3110 13b0 131f  .3R6..Y...1.....
+00000c00: 3682 0059 b280 5514 3010 3436 0144 4652  6..Y..U.0.46.DFR
+00000c10: b018 1b52 63b2 8055 1430 1035 3601 4446  ...Rc..U.0.56.DF
+00000c20: 50b0 181b 5263 b280 5510 36d9 44b7 81b0  P...Rc..U.6.D...
+00000c30: 141f 2307 3601 59b0 141f 2308 3601 59b0  ..#.6.Y...#.6.Y.
+00000c40: 141f 2309 3601 59b0 141f 230a 3601 59b0  ..#.6.Y...#.6.Y.
+00000c50: 141f 230b 3601 59b0 141f 230c 3601 59b0  ..#.6.Y...#.6.Y.
+00000c60: 141f 230d 3601 59b0 141f 230e 3601 59b0  ..#.6.Y...#.6.Y.
+00000c70: 141f 230f 3601 59b0 141f 2310 3601 59b0  ..#.6.Y...#.6.Y.
+00000c80: 141f 2311 3601 59b0 141f 2312 3601 59b0  ..#.6.Y...#.6.Y.
+00000c90: 141f 2313 3601 59b0 141f 2314 3601 59b0  ..#.6.Y...#.6.Y.
+00000ca0: 141f 2315 3601 59b0 141f 2316 3601 59b0  ..#.6.Y...#.6.Y.
+00000cb0: 141f 2317 3601 59b0 141f 2318 3601 5910  ..#.6.Y...#.6.Y.
+00000cc0: 3712 68b2 3401 dd44 4d12 1014 3810 13b0  7.h.4..DM...8...
+00000cd0: 131f 3682 0063 1210 1438 1013 b013 1f10  ..6..c...8......
+00000ce0: 3952 3684 0063 b013 1b44 5412 67b2 3401  9R6..c...DT.g.4.
+00000cf0: 80d8 444b 1210 143a b013 1fb2 3602 6348  ..DK...:....6.cH
+00000d00: 1012 0910 3bb2 103c b013 1f34 8400 634a  ....;..<...4..cJ
+00000d10: 2157 1263 df44 5ac5 4910 b014 1f23 1914  !W.c.DZ.I....#..
+00000d20: 1eb5 3601 3601 5950 6351 51c5 2805 5d4a  ..6.6.YPcQQ.(.]J
+00000d30: 015d 5163 8d00 9212 303a 1369 80ce 6060  .]Qc....0:.i..``
+00000d40: 2a48 2f28 3642 2b42 4a24 4d22 562b 4b30  *H/(6B+BJ$M"V+K0
+00000d50: 2c12 67b1 3401 81d9 44c4 80b1 8055 103d  ,.g.4...D....U.=
+00000d60: d944 6f12 0634 0014 3e36 005f 4b22 3002  .Do..4..>6._K"0.
+00000d70: c2c3 8a12 67b2 3401 f3c4 b023 1a14 1eb2  ....g.4....#....
+00000d80: 103f b4f4 103f 87f4 b336 0434 0159 421c  .?...?...6.4.YB.
+00000d90: 5263 b012 06b1 8055 3401 3401 5952 6312  Rc.....U4.4.YRc.
+00000da0: 67b1 3401 82db 44db 80b1 8055 c210 3f14  g.4...D....U..?.
+00000db0: 40b1 8151 2e02 5536 01c3 480d 1207 b2b3  @..Q..U6..H.....
+00000dc0: 1041 5234 8202 c54a 1f57 1263 df44 58c6  .AR4...J.W.c.DX.
+00000dd0: 490e b023 1b14 1eb6 3601 3401 5950 c551  I..#....6.4.YP.Q
+00000de0: 51c6 2806 5d4a 015d 1206 b234 0151 de44  Q.(.]J.]...4.Q.D
+00000df0: 4423 1c42 4223 1dc7 b0b5 4444 1042 4241  D#.BB#....DD.BBA
+00000e00: b734 0159 5263 8364 b201 9a01 3813 3980  .4.YRc.d....8.9.
+00000e10: f360 2085 1423 282c 4500 04b0 2000 01c2  .` ..#(,E... ...
+00000e20: b144 5912 0414 4336 0027 04b4 2001 0112  .DY...C6.'.. ...
+00000e30: 0234 005e 3401 c3b2 b334 0163 b212 0234  .4.^4....4.c...4
+00000e40: 0034 0163 028f 4ca2 122c 4c6b 6c80 f82b  .4.c..L..,Lkl..+
+00000e50: 3223 2c29 1f24 242a 2323 263b 1f57 2d2e  2#,).$$*##&;.W-.
+00000e60: 3200 b15e 3401 5f4b d401 c2b2 144d 104e  2..^4._K.....M.N
+00000e70: 1022 3602 142d 104f 3601 8055 c348 9a01  ."6..-.O6..U.H..
+00000e80: 2500 1050 141e b336 0134 0159 b214 5110  %..P...6.4.Y..Q.
+00000e90: 5236 0144 6725 0010 5314 1e10 3f12 67b2  R6.Dg%..S...?.g.
+00000ea0: 144d 104e 1022 3602 142d 104f 3601 8055  .M.N."6..-.O6..U
+00000eb0: 3401 f436 0134 0159 40ac 7f01 126a b210  4..6.4.Y@....j..
+00000ec0: 5434 0247 51c4 2324 c542 c580 b414 5536  T4.GQ.#$.B....U6
+00000ed0: 00c5 b514 2936 0014 3010 5636 0144 7210  ....)6..0.V6.Dr.
+00000ee0: 57b5 ddd3 446b 1058 b5dd d344 6425 0010  W...Dk.X...Dd%..
+00000ef0: 5914 1e10 3f12 67b3 3401 f4b5 144d 105a  Y...?.g.4....M.Z
+00000f00: 1022 3602 142d 105b 3601 8055 3602 3401  ."6..-.[6..U6.4.
+00000f10: 59b5 43b7 7f51 5c5d 4a21 5712 63df 445a  Y.C..Q\]J!W.c.DZ
+00000f20: c649 1025 0023 2514 1eb2 b636 0234 0159  .I.%.#%....6.4.Y
+00000f30: 5063 5151 c628 065d 4a01 5d42 a97e 5263  PcQQ.(.]J.]B.~Rc
+00000f40: 0182 38c1 4008 5c6b 80f8 53b0 5353 4b18  ..8.@.\k..S.SSK.
+00000f50: c1b1 1430 104e 3601 4434 b114 5110 5d36  ...0.N6.D4..Q.]6
+00000f60: 0144 2bb1 6759 4226 5163 8220 ca40 0a5c  .D+.gYB&Qc. .@.\
+00000f70: 6b6b 900d 53b1 5353 4b14 c2b2 142d 104f  kk..S.SSK....-.O
+00000f80: 3601 8055 2500 dd44 2fb2 6759 422a 5163  6..U%..D/.gYB*Qc
+00000f90: 8c00 e203 2c31 1333 9014 4b26 2631 3023  ....,1.3..K&&10#
+00000fa0: 2626 432b 2b25 2225 5d28 2580 1044 2a01  &&C++%"%](%..D*.
+00000fb0: 1b45 1c44 c259 b023 1e34 0159 b023 1f34  .E.D.Y.#.4.Y.#.4
+00000fc0: 0159 b023 2014 1eb2 3400 8155 8055 3601  .Y.# ...4..U.U6.
+00000fd0: 3401 59b0 2321 141e 1206 1028 3401 3601  4.Y.#!.....(4.6.
+00000fe0: 3401 59b1 4446 b023 2234 0159 b010 4634  4.Y.DF.#"4.Y..F4
+00000ff0: 0159 b144 5b12 6a10 4710 4834 0247 0ac3  .Y.D[.j.G.H4.G..
+00001000: b314 4910 3136 0159 515c 5d12 5e34 0059  ..I.16.YQ\].^4.Y
+00001010: 4819 8051 1b31 c4b0 b414 4a10 4b12 0610  H..Q.1....J.K...
+00001020: 2834 0136 8200 3401 594a 2557 1263 df44  (4.6..4.YJ%W.c.D
+00001030: 5ec5 4914 2323 141e b536 01c6 b0b6 3401  ^.I.##...6....4.
+00001040: 5912 0cb6 3401 5951 51c5 2805 5d4a 015d  Y...4.YQQ.(.]J.]
+00001050: 5163                                     Qc
```

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/InterruptHandler.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/InterruptHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_VL53L0X.py` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_bme280.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_bme280.mpy`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 00000000: 4d06 001f 8106 0518 4c4d 5f62 6d65 3238  M.......LM_bme28
 00000010: 302e 7079 000f 0a75 7469 6d65 0006 5069  0.py...utime..Pi
 00000020: 6e00 0649 3243 000e 6d61 6368 696e 6500  n..I2C..machine.
-00000030: 1a6d 6561 7375 7265 5f6d 7131 3335 000c  .measure_mq135..
-00000040: 4c4d 5f63 6f32 0018 7068 7973 6963 616c  LM_co2..physical
-00000050: 5f70 696e 0016 7069 6e6d 6170 5f64 756d  _pin..pinmap_dum
-00000060: 7000 164c 6f67 6963 616c 5069 6e73 000c  p..LogicalPins..
-00000070: 4465 7669 6365 000c 424d 4532 3830 0022  Device..BME280."
-00000080: 5f5f 696e 6974 5f62 6d65 3238 305f 6932  __init_bme280_i2
-00000090: 6300 0673 636c 000e 6932 635f 7363 6c00  c..scl..i2c_scl.
-000000a0: 0673 6461 000e 6932 635f 7364 6100 0866  .sda..i2c_sda..f
-000000b0: 7265 7100 0669 3263 000e 6d65 6173 7572  req..i2c..measur
-000000c0: 6500 1674 656d 7065 7261 7475 7265 0014  e..temperature..
-000000d0: 7465 6d70 205b c2ba 435d 0010 6875 6d69  temp [..C]..humi
-000000e0: 6469 7479 000e 6875 6d20 5b25 5d00 1070  dity..hum [%]..p
-000000f0: 7265 7373 7572 6500 1a6d 6561 7375 7265  ressure..measure
-00000100: 5f77 5f63 6f32 0012 636f 3220 5b70 706d  _w_co2..co2 [ppm
+00000030: 1870 6879 7369 6361 6c5f 7069 6e00 1670  .physical_pin..p
+00000040: 696e 6d61 705f 6475 6d70 0016 4c6f 6769  inmap_dump..Logi
+00000050: 6361 6c50 696e 7300 0c44 6576 6963 6500  calPins..Device.
+00000060: 0c42 4d45 3238 3000 225f 5f69 6e69 745f  .BME280."__init_
+00000070: 626d 6532 3830 5f69 3263 0006 7363 6c00  bme280_i2c..scl.
+00000080: 0e69 3263 5f73 636c 0006 7364 6100 0e69  .i2c_scl..sda..i
+00000090: 3263 5f73 6461 0008 6672 6571 0006 6932  2c_sda..freq..i2
+000000a0: 6300 0e6d 6561 7375 7265 0016 7465 6d70  c..measure..temp
+000000b0: 6572 6174 7572 6500 1474 656d 7020 5bc2  erature..temp [.
+000000c0: ba43 5d00 1068 756d 6964 6974 7900 0e68  .C]..humidity..h
+000000d0: 756d 205b 255d 0010 7072 6573 7375 7265  um [%]..pressure
+000000e0: 001a 6d65 6173 7572 655f 775f 636f 3200  ..measure_w_co2.
+000000f0: 1a6d 6561 7375 7265 5f6d 7131 3335 000c  .measure_mq135..
+00000100: 4c4d 5f63 6f32 0012 636f 3220 5b70 706d  LM_co2..co2 [ppm
 00000110: 5d00 0a6c 6d64 6570 0006 636f 3200 0c70  ]..lmdep..co2..p
 00000120: 696e 6d61 7000 0868 656c 7000 2310 5f61  inmap..help.#._a
 00000130: 6464 7265 7373 0008 5f69 3263 0012 7772  ddress.._i2c..wr
 00000140: 6974 6552 6177 3800 0e77 7269 7465 746f  iteRaw8..writeto
 00000150: 000c 7772 6974 6538 0016 7772 6974 6574  ..write8..writet
 00000160: 6f5f 6d65 6d00 0e77 7269 7465 3136 0010  o_mem..write16..
 00000170: 7265 6164 5261 7738 0081 2b10 7265 6164  readRaw8..+.read
@@ -114,155 +114,155 @@
 00000710: 414c 4f57 504f 5745 522c 2042 4d45 3238  ALOWPOWER, BME28
 00000720: 305f 5354 414e 4441 5244 2c20 424d 4532  0_STANDARD, BME2
 00000730: 3830 5f48 4947 4852 4553 2c20 6f72 2042  80_HIGHRES, or B
 00000740: 4d45 3238 305f 554c 5452 4148 4947 4852  ME280_ULTRAHIGHR
 00000750: 4553 0005 1a41 6e20 4932 4320 6f62 6a65  ES...An I2C obje
 00000760: 6374 2069 7320 7265 7175 6972 6564 2e00  ct is required..
 00000770: 070f 3134 3037 3337 3438 3833 3535 3332  ..14073748835532
-00000780: 3894 0410 7201 6060 2632 2c72 6523 2323  8...r.``&2,re###
-00000790: 2363 2025 2545 2525 2525 2525 2525 4525  #c %%E%%%%%%%%E%
-000007a0: 2525 2525 2545 2525 4525 2525 2525 4563  %%%%%E%%E%%%%%Ec
-000007b0: 8957 8997 840c 8409 840e 8409 840a 8051  .W.............Q
-000007c0: 1b02 1655 8010 0310 042a 021b 051c 0316  ...U.....*......
-000007d0: 031c 0416 0459 8010 062a 011b 071c 0616  .....Y...*......
-000007e0: 0659 8010 0810 092a 021b 0a1c 0816 081c  .Y.....*........
-000007f0: 0916 0959 2280 7616 5681 1657 8216 5883  ...Y".v.V..W..X.
-00000800: 1659 8416 5a85 165b 2281 0816 5c22 810a  .Y..Z..["...\"..
-00000810: 165d 2281 0c16 5e22 810e 165f 2281 1016  .]"...^"..._"...
-00000820: 6022 8112 1661 2281 1416 6222 8116 1663  `"...a"...b"...c
-00000830: 2281 1816 6422 811a 1665 2281 1c16 6622  "...d"...e"...f"
-00000840: 811e 1667 2281 2116 6822 8161 1669 2281  ...g".!.h".a.i".
-00000850: 6316 6a22 8164 166b 2281 6516 6c22 8166  c.j".d.k".e.l".f
-00000860: 166d 2281 6716 6e22 8150 166f 2281 5116  .m".g.n".P.o".Q.
-00000870: 7022 8160 1671 2281 7216 7222 8174 1673  p".`.q".r.r".t.s
-00000880: 2281 7516 7422 8177 1675 2281 7a16 7622  ".u.t".w.u".z.v"
-00000890: 817d 1677 5117 7854 3200 100b 3402 160b  .}.wQ.xT2...4...
-000008a0: 5432 0110 0c34 0216 0c32 0216 0d32 0316  T2...4...2...2..
-000008b0: 1432 0416 1a32 0516 1c32 0616 1e32 0716  .2...2...2...2..
-000008c0: 1f51 6308 862c 083a 0b88 3c60 4064 6064  .Qc..,.:..<`@d`d
-000008d0: 4064 6084 0864 2064 4084 0788 0a88 0964  @d`..d d@......d
-000008e0: 4064 4064 4011 7916 7a10 0b16 7b32 0016  @d@d@.y.z...{2..
-000008f0: 2032 0116 2332 0216 2532 0316 2732 0416   2..#2..%2..'2..
-00000900: 2832 0516 2c32 0616 2e52 2a01 5333 0716  (2..,2...R*.S3..
-00000910: 2f52 2a01 5333 0816 3032 0916 3132 0a16  /R*.S3..02..12..
-00000920: 3332 0b16 3432 0c16 3551 630d 8120 2310  32..42..5Qc.. #.
-00000930: 207d 7e13 8042 4024 b1b0 1821 b2b0 1822   }~..B@$...!..."
-00000940: 5163 8168 2a0e 237d 7f80 4820 26b1 2281  Qc.h*.#}..H &.".
-00000950: 7fef c1b0 1322 1424 b013 21b1 3602 5951  .....".$..!.6.YQ
-00000960: 6382 5043 1425 7d81 007f 804d 2027 2812  c.PC.%}....M '(.
-00000970: 8101 8134 01c3 b222 817f efb3 8056 b013  ...4...".....V..
-00000980: 2214 26b0 1321 b1b3 3603 5951 6383 6843  ".&..!..6.YQc.hC
-00000990: 1827 7d81 007f 8053 2027 2728 2ab2 2283  .'}....S ''(*.".
-000009a0: ff7f efc2 1281 0182 3401 c3b2 2281 7fef  ........4..."...
-000009b0: b380 56b2 88f1 2281 7fef b381 56b0 1313  ..V...".....V...
-000009c0: 1426 b013 21b1 b236 0359 5163 8200 310a  .&..!..6.YQc..1.
-000009d0: 287d 805b 2012 8102 1429 b013 2214 2ab0  (}.[ ....)..".*.
-000009e0: 1321 8136 0210 2b36 0222 817f ef63 8220  .!.6..+6."...c. 
-000009f0: 4210 2c7d 8100 805f 2025 1281 0214 29b0  B.,}..._ %....).
-00000a00: 1322 142d b013 21b1 8136 0310 2b36 0222  .".-..!..6..+6."
-00000a10: 817f ef63 8210 2a14 2e7d 8100 8064 2027  ...c..*..}...d '
-00000a20: 2726 b014 2cb1 3601 c2b2 2280 7fd8 4446  '&..,.6..."...DF
-00000a30: b222 8200 e6c2 b263 8360 d301 182f 7d81  .".....c.`.../}.
-00000a40: 0032 806b 6025 3623 2d12 8102 1429 b013  .2.k`%6#-....)..
-00000a50: 2214 2db0 1321 b182 3603 102b 3602 2283  ".-..!..6..+6.".
-00000a60: ff7f efc3 b243 4db3 88f0 2283 fe00 efb3  .....CM...".....
-00000a70: 88f1 f2c3 b363 8238 bb01 1630 7d81 0032  .....c.8...0}..2
-00000a80: 8075 6028 2827 b014 2fb1 b236 02c3 b322  .u`(('../..6..."
-00000a90: 81ff 7fd8 4447 b322 8480 00e6 c3b3 6381  ....DG."......c.
-00000aa0: 2032 0e31 7d81 0080 7e40 b014 2fb1 1032   2.1}...~@../..2
-00000ab0: 5236 8201 6381 2032 0e33 7d81 0080 8340  R6..c. 2.3}....@
-00000ac0: b014 2fb1 1032 5036 8201 6381 2032 0e34  ../..2P6..c. 2.4
-00000ad0: 7d81 0080 8840 b014 30b1 1032 5236 8201  }....@..0..2R6..
-00000ae0: 6381 2032 0e35 7d81 0080 8d40 b014 30b1  c. 2.5}....@..0.
-00000af0: 1032 5036 8201 6386 1c10 2e0c 8893 8c13  .2P6..c.........
-00000b00: 841e 8411 840a 8408 840a 8412 840d 8808  ................
-00000b10: 8808 1179 167a 100c 167b 1157 1156 512a  ...y.z...{.W.VQ*
-00000b20: 0353 3300 1620 3201 1639 3202 164d 3203  .S3.. 2..92..M2.
-00000b30: 164f 3204 1650 3205 1651 3206 1652 3207  .O2..P2..Q2..R2.
-00000b40: 1653 117c 3208 3401 1615 117c 3209 3401  .S.|2.4....|2.4.
-00000b50: 1619 117c 320a 3401 1617 5163 0b86 28d0  ...|2.4...Qc..(.
-00000b60: 8541 2220 7d81 037e 1380 9651 236a 4425  .A" }..~...Q#jD%
-00000b70: 2849 262c b112 5712 5812 5912 5a12 5b2b  (I&,..W.X.Y.Z.[+
-00000b80: 05dd d344 4d12 8104 2302 1436 b136 0134  ...DM...#..6.6.4
-00000b90: 0165 b1b0 1837 b351 de44 4812 8104 2303  .e...7.Q.DH...#.
-00000ba0: 3401 6512 0bb2 b334 02b0 1838 b014 3936  4.e....4...8..96
-00000bb0: 0059 b013 3814 2512 7322 3f36 0259 80b0  .Y..8.%.s"?6.Y..
-00000bc0: 183a 5163 9200 3134 397d 80a8 2c2c 4c2c  .:Qc..149}..,,L,
-00000bd0: 2c2c 2c2c 2c2c 2c4c 2c2c 2c4c 2a26 502a  ,,,,,,,L,,,L*&P*
-00000be0: 2621 b013 3814 3112 5c36 01b0 183b b013  &!..8.1.\6...;..
-00000bf0: 3814 3412 5d36 01b0 183c b013 3814 3412  8.4.]6...<..8.4.
-00000c00: 5e36 01b0 183d b013 3814 3112 5f36 01b0  ^6...=..8.1._6..
-00000c10: 183e b013 3814 3412 6036 01b0 183f b013  .>..8.4.`6...?..
-00000c20: 3814 3412 6136 01b0 1840 b013 3814 3412  8.4.a6...@..8.4.
-00000c30: 6236 01b0 1841 b013 3814 3412 6336 01b0  b6...A..8.4.c6..
-00000c40: 1842 b013 3814 3412 6436 01b0 1843 b013  .B..8.4.d6...C..
-00000c50: 3814 3412 6536 01b0 1844 b013 3814 3412  8.4.e6...D..8.4.
-00000c60: 6636 01b0 1845 b013 3814 3412 6736 01b0  f6...E..8.4.g6..
-00000c70: 1846 b013 3814 2c12 6836 01b0 1847 b013  .F..8.,.h6...G..
-00000c80: 3814 3412 6936 01b0 1848 b013 3814 2c12  8.4.i6...H..8.,.
-00000c90: 6a36 01b0 1849 b013 3814 2e12 6e36 01b0  j6...I..8...n6..
-00000ca0: 184a b013 3814 2e12 6b36 01c1 b198 f094  .J..8...k6......
-00000cb0: f1c1 b1b0 1338 142c 126c 3601 8fef edb0  .....8.,.l6.....
-00000cc0: 184b b013 3814 2e12 6d36 01c2 b298 f094  .K..8...m6......
-00000cd0: f1c2 b2b0 1338 142c 126c 3601 84f1 8fef  .....8.,.l6.....
-00000ce0: edb0 184c 5163 8a08 5122 4d7d 80c5 2024  ...LQc..Q"M}.. $
-00000cf0: 2b2e 2b4e 3030 282a 2c2c 2cb0 1337 c1b0  +.+N00(*,,,..7..
-00000d00: 1338 1425 1272 b136 0259 b013 3785 f0b0  .8.%.r.6.Y..7...
-00000d10: 1337 82f0 ed81 edc1 b013 3814 2512 73b1  .7........8.%.s.
-00000d20: 3602 5922 8962 2291 7c81 b013 37f0 f4f2  6.Y".b".|...7...
-00000d30: c2b2 2291 7c81 b013 37f0 f4f2 2284 3ff2  ..".|...7...".?.
-00000d40: c2b2 2291 7c81 b013 37f0 f4f2 2284 3ff2  ..".|...7...".?.
-00000d50: c212 5514 4eb2 3601 59b0 1338 142c 1276  ..U.N.6.Y..8.,.v
-00000d60: 3601 c3b0 1338 142c 1276 81f2 3601 c4b0  6....8.,.v..6...
-00000d70: 1338 142c 1276 82f2 3601 c5b3 90f0 b488  .8.,.v..6.......
-00000d80: f0ed b5ed 84f1 c6b6 6383 6841 164f 7d80  ........c.hA.O}.
-00000d90: d620 2020 2a2c 2c2c b013 3814 2c12 7536  .   *,,,..8.,.u6
-00000da0: 01c1 b013 3814 2c12 7581 f236 01c2 b013  ....8.,.u..6....
-00000db0: 3814 2c12 7582 f236 01c3 b190 f0b2 88f0  8.,.u..6........
-00000dc0: edb3 ed84 f1c4 b463 8248 3912 507d 80e0  .......c.H9.P}..
-00000dd0: 2020 2a2c 26b0 1338 142c 1277 3601 c1b0    *,&..8.,.w6...
-00000de0: 1338 142c 1277 81f2 3601 c2b1 88f0 b2ed  .8.,.w..6.......
-00000df0: c3b3 6384 6831 1651 7d80 e820 2630 2031  ..c.h1.Q}.. &0 1
-00000e00: 2726 b014 4d36 00c1 b183 f1b0 133b 81f0  '&..M6.......;..
-00000e10: f3b0 133c 8bf1 f4c2 b184 f1b0 133b f3b1  ...<.........;..
-00000e20: 84f1 b013 3bf3 f48c f1b0 133d f48e f1c3  ....;......=....
-00000e30: b2b3 f2b0 183a b013 3a85 f422 8100 f288  .....:..:.."....
-00000e40: f163 8950 3926 527d 80f2 2026 2928 2a28  .c.P9&R}.. &)(*(
-00000e50: 2929 2b25 2228 2c2e 28b0 144f 3600 c1b0  ))+%"(,.(..O6...
-00000e60: 133a 2287 e800 f3c2 b2b2 f4b0 1343 f4c3  .:"..........C..
-00000e70: b3b2 b013 42f4 91f0 f2c3 b3b0 1341 a3f0  ....B........A..
-00000e80: f2c3 b2b2 f4b0 1340 f488 f1b2 b013 3ff4  .......@......?.
-00000e90: 8cf1 f2c2 2304 b2f2 b013 3ef4 a1f1 c2b2  ....#.....>.....
-00000ea0: 80d9 4442 8063 2280 c080 00b1 f3c4 b49f  ..DB.c".........
-00000eb0: f0b3 f322 9835 f4b2 f6c4 b013 46b4 8df1  ...".5......F...
-00000ec0: f4b4 8df1 f499 f1c2 b013 45b4 f493 f1c3  ..........E.....
-00000ed0: b4b2 f2b3 f288 f1b0 1344 84f0 f263 8908  .........D...c..
-00000ee0: 311a 537d 9004 4629 3628 342d 322a 34b0  1.S}..F)6(4-2*4.
-00000ef0: 1450 3600 c1b0 133a 2284 d800 f3c2 b18e  .P6....:".......
-00000f00: f0b0 134b 94f0 f3b0 134c b2f4 f322 8180  ...K.....L..."..
-00000f10: 00f2 8ff1 b2b0 134a f48a f1b2 b013 49f4  .......J......I.
-00000f20: 8bf1 2282 8000 f2f4 8af1 2281 8080 00f2  ..".......".....
-00000f30: b013 48f4 2280 c000 f28e f1f4 c2b2 b28f  ..H."...........
-00000f40: f1b2 8ff1 f487 f1b0 1347 f484 f1f3 c2b2  .........G......
-00000f50: 80d7 4443 8042 41b2 c2b2 2281 c880 8000  ..DC.BA...".....
-00000f60: d844 4822 81c8 8080 0042 41b2 c2b2 8cf1  .DH".....BA.....
-00000f70: 6382 6041 1015 7d90 1220 2626 28b0 1451  c.`A..}.. &&(..Q
-00000f80: 3600 c1b1 2280 64f6 c2b1 b222 8064 f4f3  6...".d....".d..
-00000f90: c312 8105 1054 1436 b2b3 3602 3401 6383  .....T.6..6.4.c.
-00000fa0: 0041 1019 7d90 1a20 2a26 28b0 1452 3600  .A..}.. *&(..R6.
-00000fb0: 2282 00f6 c1b1 2280 64f6 c2b1 b222 8064  ".....".d....".d
-00000fc0: f4f3 c312 8105 1054 1436 b2b3 3602 3401  .......T.6..6.4.
-00000fd0: 6383 2041 1017 7d90 2220 2626 30b0 1453  c. A..}." &&0..S
-00000fe0: 3600 c1b1 2288 00f6 c2b1 2280 64f4 2288  6...".....".d.".
-00000ff0: 00f6 b222 8064 f4f3 c312 8105 1054 1436  ...".d.......T.6
-00001000: b2b3 3602 3401 6384 0838 100d 902a 2026  ..6.4.c..8...* &
-00001010: 1f25 2a12 7851 de44 6e12 0410 0e12 0312  .%*.xQ.Dn.......
-00001020: 0810 0f34 0134 0110 1012 0312 0810 1134  ...4.4.........4
-00001030: 0134 0110 1222 80ce 1034 8600 c012 0c10  .4..."...4......
-00001040: 13b0 3482 0017 7812 7863 8210 180c 1490  ..4...x.xc......
-00001050: 3660 2025 120d 3400 c02c 03b0 1315 1016  6` %..4..,......
-00001060: 62b0 1317 1018 62b0 1319 2300 6263 8200  b.....b...#.bc..
-00001070: 200e 1a90 3f60 2025 3012 1434 00c0 1206   ...?` %0..4....
-00001080: b010 1655 b010 1855 3402 b010 1b56 b063  ...U...U4....V.c
-00001090: 5000 0a1c 904d 6040 101d 6381 1010 0a1e  P....M`@..c.....
-000010a0: 9056 6060 1209 100f 1011 2b02 3401 6350  .V``......+.4.cP
-000010b0: 000a 1f90 6060 4023 0163                 ....``@#.c
+00000780: 3893 1c10 7001 6060 2632 7265 2323 2323  8...p.``&2re####
+00000790: 6320 2525 4525 2525 2525 2525 2545 2525  c %%E%%%%%%%%E%%
+000007a0: 2525 2525 4525 2545 2525 2525 2545 6389  %%%%E%%E%%%%%Ec.
+000007b0: 5789 9784 0c84 0984 0f84 0984 0a80 511b  W.............Q.
+000007c0: 0216 5580 1003 1004 2a02 1b05 1c03 1603  ..U.....*.......
+000007d0: 1c04 1604 5980 1006 1007 2a02 1b08 1c06  ....Y.....*.....
+000007e0: 1606 1c07 1607 5922 8076 1656 8116 5782  ......Y".v.V..W.
+000007f0: 1658 8316 5984 165a 8516 5b22 8108 165c  .X..Y..Z..["...\
+00000800: 2281 0a16 5d22 810c 165e 2281 0e16 5f22  "...]"...^"..._"
+00000810: 8110 1660 2281 1216 6122 8114 1662 2281  ...`"...a"...b".
+00000820: 1616 6322 8118 1664 2281 1a16 6522 811c  ..c"...d"...e"..
+00000830: 1666 2281 1e16 6722 8121 1668 2281 6116  .f"...g".!.h".a.
+00000840: 6922 8163 166a 2281 6416 6b22 8165 166c  i".c.j".d.k".e.l
+00000850: 2281 6616 6d22 8167 166e 2281 5016 6f22  ".f.m".g.n".P.o"
+00000860: 8151 1670 2281 6016 7122 8172 1672 2281  .Q.p".`.q".r.r".
+00000870: 7416 7322 8175 1674 2281 7716 7522 817a  t.s".u.t".w.u".z
+00000880: 1676 2281 7d16 7751 1778 5432 0010 0934  .v".}.wQ.xT2...4
+00000890: 0216 0954 3201 100a 3402 160a 3202 160b  ...T2...4...2...
+000008a0: 3203 1612 3204 1618 3205 161c 3206 161e  2...2...2...2...
+000008b0: 3207 161f 5163 0886 2c08 3a09 883b 6040  2...Qc..,.:..;`@
+000008c0: 6460 6440 6460 8408 6420 6440 8407 880a  d`d@d`..d d@....
+000008d0: 8809 6440 6440 6440 1179 167a 1009 167b  ..d@d@d@.y.z...{
+000008e0: 3200 1620 3201 1623 3202 1625 3203 1627  2.. 2..#2..%2..'
+000008f0: 3204 1628 3205 162c 3206 162e 522a 0153  2..(2..,2...R*.S
+00000900: 3307 162f 522a 0153 3308 1630 3209 1631  3../R*.S3..02..1
+00000910: 320a 1633 320b 1634 320c 1635 5163 0d81  2..32..42..5Qc..
+00000920: 2023 1020 7d7e 1180 4140 24b1 b018 21b2   #. }~..A@$...!.
+00000930: b018 2251 6381 682a 0e23 7d7f 8047 2026  .."Qc.h*.#}..G &
+00000940: b122 817f efc1 b013 2214 24b0 1321 b136  ."......".$..!.6
+00000950: 0259 5163 8250 4314 257d 8100 7f80 4c20  .YQc.PC.%}....L 
+00000960: 2728 1281 0181 3401 c3b2 2281 7fef b380  '(....4...".....
+00000970: 56b0 1322 1426 b013 21b1 b336 0359 5163  V..".&..!..6.YQc
+00000980: 8368 4318 277d 8100 7f80 5220 2727 282a  .hC.'}....R ''(*
+00000990: b222 83ff 7fef c212 8101 8234 01c3 b222  .".........4..."
+000009a0: 817f efb3 8056 b288 f122 817f efb3 8156  .....V...".....V
+000009b0: b013 1114 26b0 1321 b1b2 3603 5951 6382  ....&..!..6.YQc.
+000009c0: 0031 0a28 7d80 5a20 1281 0214 29b0 1322  .1.(}.Z ....).."
+000009d0: 142a b013 2181 3602 102b 3602 2281 7fef  .*..!.6..+6."...
+000009e0: 6382 2042 102c 7d81 0080 5e20 2512 8102  c. B.,}...^ %...
+000009f0: 1429 b013 2214 2db0 1321 b181 3603 102b  .)..".-..!..6..+
+00000a00: 3602 2281 7fef 6382 102a 142e 7d81 0080  6."...c..*..}...
+00000a10: 6320 2727 26b0 142c b136 01c2 b222 807f  c ''&..,.6..."..
+00000a20: d844 46b2 2282 00e6 c2b2 6383 60d3 0118  .DF.".....c.`...
+00000a30: 2f7d 8100 3280 6a60 2536 232d 1281 0214  /}..2.j`%6#-....
+00000a40: 29b0 1322 142d b013 21b1 8236 0310 2b36  )..".-..!..6..+6
+00000a50: 0222 83ff 7fef c3b2 434d b388 f022 83fe  ."......CM..."..
+00000a60: 00ef b388 f1f2 c3b3 6382 38bb 0116 307d  ........c.8...0}
+00000a70: 8100 3280 7460 2828 27b0 142f b1b2 3602  ..2.t`(('../..6.
+00000a80: c3b3 2281 ff7f d844 47b3 2284 8000 e6c3  .."....DG.".....
+00000a90: b363 8120 320e 317d 8100 807d 40b0 142f  .c. 2.1}...}@../
+00000aa0: b110 3252 3682 0163 8120 320e 337d 8100  ..2R6..c. 2.3}..
+00000ab0: 8082 40b0 142f b110 3250 3682 0163 8120  ..@../..2P6..c. 
+00000ac0: 320e 347d 8100 8087 40b0 1430 b110 3252  2.4}....@..0..2R
+00000ad0: 3682 0163 8120 320e 357d 8100 808c 40b0  6..c. 2.5}....@.
+00000ae0: 1430 b110 3250 3682 0163 861c 102e 0a88  .0..2P6..c......
+00000af0: 928c 1384 1e84 1184 0a84 0884 0a84 1284  ................
+00000b00: 0d88 0888 0811 7916 7a10 0a16 7b11 5711  ......y.z...{.W.
+00000b10: 5651 2a03 5333 0016 2032 0116 3932 0216  VQ*.S3.. 2..92..
+00000b20: 4d32 0316 4f32 0416 5032 0516 5132 0616  M2..O2..P2..Q2..
+00000b30: 5232 0716 5311 7c32 0834 0116 1311 7c32  R2..S.|2.4....|2
+00000b40: 0934 0116 1711 7c32 0a34 0116 1551 630b  .4....|2.4...Qc.
+00000b50: 8628 d085 4122 207d 8103 7e11 8095 5123  .(..A" }..~...Q#
+00000b60: 6a44 2528 4926 2cb1 1257 1258 1259 125a  jD%(I&,..W.X.Y.Z
+00000b70: 125b 2b05 ddd3 444d 1281 0423 0214 36b1  .[+...DM...#..6.
+00000b80: 3601 3401 65b1 b018 37b3 51de 4448 1281  6.4.e...7.Q.DH..
+00000b90: 0423 0334 0165 1209 b2b3 3402 b018 38b0  .#.4.e....4...8.
+00000ba0: 1439 3600 59b0 1338 1425 1273 223f 3602  .96.Y..8.%.s"?6.
+00000bb0: 5980 b018 3a51 6392 0031 3439 7d80 a72c  Y...:Qc..149}..,
+00000bc0: 2c4c 2c2c 2c2c 2c2c 2c2c 4c2c 2c2c 4c2a  ,L,,,,,,,,L,,,L*
+00000bd0: 2650 2a26 21b0 1338 1431 125c 3601 b018  &P*&!..8.1.\6...
+00000be0: 3bb0 1338 1434 125d 3601 b018 3cb0 1338  ;..8.4.]6...<..8
+00000bf0: 1434 125e 3601 b018 3db0 1338 1431 125f  .4.^6...=..8.1._
+00000c00: 3601 b018 3eb0 1338 1434 1260 3601 b018  6...>..8.4.`6...
+00000c10: 3fb0 1338 1434 1261 3601 b018 40b0 1338  ?..8.4.a6...@..8
+00000c20: 1434 1262 3601 b018 41b0 1338 1434 1263  .4.b6...A..8.4.c
+00000c30: 3601 b018 42b0 1338 1434 1264 3601 b018  6...B..8.4.d6...
+00000c40: 43b0 1338 1434 1265 3601 b018 44b0 1338  C..8.4.e6...D..8
+00000c50: 1434 1266 3601 b018 45b0 1338 1434 1267  .4.f6...E..8.4.g
+00000c60: 3601 b018 46b0 1338 142c 1268 3601 b018  6...F..8.,.h6...
+00000c70: 47b0 1338 1434 1269 3601 b018 48b0 1338  G..8.4.i6...H..8
+00000c80: 142c 126a 3601 b018 49b0 1338 142e 126e  .,.j6...I..8...n
+00000c90: 3601 b018 4ab0 1338 142e 126b 3601 c1b1  6...J..8...k6...
+00000ca0: 98f0 94f1 c1b1 b013 3814 2c12 6c36 018f  ........8.,.l6..
+00000cb0: efed b018 4bb0 1338 142e 126d 3601 c2b2  ....K..8...m6...
+00000cc0: 98f0 94f1 c2b2 b013 3814 2c12 6c36 0184  ........8.,.l6..
+00000cd0: f18f efed b018 4c51 638a 0851 224d 7d80  ......LQc..Q"M}.
+00000ce0: c420 242b 2e2b 4e30 3028 2a2c 2c2c b013  . $+.+N00(*,,,..
+00000cf0: 37c1 b013 3814 2512 72b1 3602 59b0 1337  7...8.%.r.6.Y..7
+00000d00: 85f0 b013 3782 f0ed 81ed c1b0 1338 1425  ....7........8.%
+00000d10: 1273 b136 0259 2289 6222 917c 81b0 1337  .s.6.Y".b".|...7
+00000d20: f0f4 f2c2 b222 917c 81b0 1337 f0f4 f222  .....".|...7..."
+00000d30: 843f f2c2 b222 917c 81b0 1337 f0f4 f222  .?...".|...7..."
+00000d40: 843f f2c2 1255 144e b236 0159 b013 3814  .?...U.N.6.Y..8.
+00000d50: 2c12 7636 01c3 b013 3814 2c12 7681 f236  ,.v6....8.,.v..6
+00000d60: 01c4 b013 3814 2c12 7682 f236 01c5 b390  ....8.,.v..6....
+00000d70: f0b4 88f0 edb5 ed84 f1c6 b663 8368 4116  ...........c.hA.
+00000d80: 4f7d 80d5 2020 202a 2c2c 2cb0 1338 142c  O}..   *,,,..8.,
+00000d90: 1275 3601 c1b0 1338 142c 1275 81f2 3601  .u6....8.,.u..6.
+00000da0: c2b0 1338 142c 1275 82f2 3601 c3b1 90f0  ...8.,.u..6.....
+00000db0: b288 f0ed b3ed 84f1 c4b4 6382 4839 1250  ..........c.H9.P
+00000dc0: 7d80 df20 202a 2c26 b013 3814 2c12 7736  }..  *,&..8.,.w6
+00000dd0: 01c1 b013 3814 2c12 7781 f236 01c2 b188  ....8.,.w..6....
+00000de0: f0b2 edc3 b363 8468 3116 517d 80e7 2026  .....c.h1.Q}.. &
+00000df0: 3020 3127 26b0 144d 3600 c1b1 83f1 b013  0 1'&..M6.......
+00000e00: 3b81 f0f3 b013 3c8b f1f4 c2b1 84f1 b013  ;.....<.........
+00000e10: 3bf3 b184 f1b0 133b f3f4 8cf1 b013 3df4  ;......;......=.
+00000e20: 8ef1 c3b2 b3f2 b018 3ab0 133a 85f4 2281  ........:..:..".
+00000e30: 00f2 88f1 6389 5039 2652 7d80 f120 2629  ....c.P9&R}.. &)
+00000e40: 282a 2829 292b 2522 282c 2e28 b014 4f36  (*())+%"(,.(..O6
+00000e50: 00c1 b013 3a22 87e8 00f3 c2b2 b2f4 b013  ....:"..........
+00000e60: 43f4 c3b3 b2b0 1342 f491 f0f2 c3b3 b013  C......B........
+00000e70: 41a3 f0f2 c3b2 b2f4 b013 40f4 88f1 b2b0  A.........@.....
+00000e80: 133f f48c f1f2 c223 04b2 f2b0 133e f4a1  .?.....#.....>..
+00000e90: f1c2 b280 d944 4280 6322 80c0 8000 b1f3  .....DB.c"......
+00000ea0: c4b4 9ff0 b3f3 2298 35f4 b2f6 c4b0 1346  ......".5......F
+00000eb0: b48d f1f4 b48d f1f4 99f1 c2b0 1345 b4f4  .............E..
+00000ec0: 93f1 c3b4 b2f2 b3f2 88f1 b013 4484 f0f2  ............D...
+00000ed0: 6389 0831 1a53 7d90 0346 2936 2834 2d32  c..1.S}..F)6(4-2
+00000ee0: 2a34 b014 5036 00c1 b013 3a22 84d8 00f3  *4..P6....:"....
+00000ef0: c2b1 8ef0 b013 4b94 f0f3 b013 4cb2 f4f3  ......K.....L...
+00000f00: 2281 8000 f28f f1b2 b013 4af4 8af1 b2b0  ".........J.....
+00000f10: 1349 f48b f122 8280 00f2 f48a f122 8180  .I..."......."..
+00000f20: 8000 f2b0 1348 f422 80c0 00f2 8ef1 f4c2  .....H."........
+00000f30: b2b2 8ff1 b28f f1f4 87f1 b013 47f4 84f1  ............G...
+00000f40: f3c2 b280 d744 4380 4241 b2c2 b222 81c8  .....DC.BA..."..
+00000f50: 8080 00d8 4448 2281 c880 8000 4241 b2c2  ....DH".....BA..
+00000f60: b28c f163 8260 4110 137d 9011 2026 2628  ...c.`A..}.. &&(
+00000f70: b014 5136 00c1 b122 8064 f6c2 b1b2 2280  ..Q6...".d....".
+00000f80: 64f4 f3c3 1281 0510 5414 36b2 b336 0234  d.......T.6..6.4
+00000f90: 0163 8300 4110 177d 9019 202a 2628 b014  .c..A..}.. *&(..
+00000fa0: 5236 0022 8200 f6c1 b122 8064 f6c2 b1b2  R6.".....".d....
+00000fb0: 2280 64f4 f3c3 1281 0510 5414 36b2 b336  ".d.......T.6..6
+00000fc0: 0234 0163 8320 4110 157d 9021 2026 2630  .4.c. A..}.! &&0
+00000fd0: b014 5336 00c1 b122 8800 f6c2 b122 8064  ..S6...".....".d
+00000fe0: f422 8800 f6b2 2280 64f4 f3c3 1281 0510  ."....".d.......
+00000ff0: 5414 36b2 b336 0234 0163 8408 3810 0b90  T.6..6.4.c..8...
+00001000: 2920 261f 252a 1278 51de 446e 1204 100c  ) &.%*.xQ.Dn....
+00001010: 1203 1206 100d 3401 3401 100e 1203 1206  ......4.4.......
+00001020: 100f 3401 3401 1010 2280 ce10 3486 00c0  ..4.4..."...4...
+00001030: 120a 1011 b034 8200 1778 1278 6382 1018  .....4...x.xc...
+00001040: 0c12 9035 6020 2512 0b34 00c0 2c03 b013  ...5` %..4..,...
+00001050: 1310 1462 b013 1510 1662 b013 1723 0062  ...b.....b...#.b
+00001060: 6382 5828 1018 903e 6020 2b25 2f80 1019  c.X(...>` +%/...
+00001070: 2a01 1b1a 1c19 c059 1212 3400 c1b0 b110  *......Y..4.....
+00001080: 1455 b110 1655 3402 b110 1b56 b163 5000  .U...U4....V.cP.
+00001090: 0a1c 904d 6040 101d 6381 1010 0a1e 9056  ...M`@..c......V
+000010a0: 6060 1207 100d 100f 2b02 3401 6350 000a  ``......+.4.cP..
+000010b0: 1f90 6060 4023 0163                      ..``@#.c
```

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_buzzer.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_buzzer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_catgame.py` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_cct.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_cct.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_co2.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_co2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_demo.py` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_dht11.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_dht22.mpy`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-00000000: 4d06 001f 2401 164c 4d5f 6468 7431 312e  M...$..LM_dht11.
-00000010: 7079 000f 1a6d 6561 7375 7265 5f6d 7131  py...measure_mq1
-00000020: 3335 000c 4c4d 5f63 6f32 0018 7068 7973  35..LM_co2..phys
-00000030: 6963 616c 5f70 696e 0016 7069 6e6d 6170  ical_pin..pinmap
-00000040: 5f64 756d 7000 164c 6f67 6963 616c 5069  _dump..LogicalPi
-00000050: 6e73 0016 6461 7461 5f6c 6f67 6765 7200  ns..data_logger.
-00000060: 0c43 6f6d 6d6f 6e00 0a64 6874 3131 0018  .Common..dht11..
-00000070: 5f5f 696e 6974 5f44 4854 3131 000a 4448  __init_DHT11..DH
-00000080: 5431 3100 0664 6874 0006 5069 6e00 0e6d  T11..dht..Pin..m
-00000090: 6163 6869 6e65 000c 6468 7470 696e 0014  achine..dhtpin..
-000000a0: 5f5f 7465 6d70 5f68 756d 000e 6d65 6173  __temp_hum..meas
-000000b0: 7572 6500 1674 656d 7065 7261 7475 7265  ure..temperature
-000000c0: 0010 6875 6d69 6469 7479 0014 7465 6d70  ..humidity..temp
-000000d0: 205b c2ba 435d 000e 6875 6d20 5b25 5d00   [..C]..hum [%].
-000000e0: 0864 6174 6100 1a6d 6561 7375 7265 5f77  .data..measure_w
+00000000: 4d06 001f 2401 164c 4d5f 6468 7432 322e  M...$..LM_dht22.
+00000010: 7079 000f 1870 6879 7369 6361 6c5f 7069  py...physical_pi
+00000020: 6e00 1670 696e 6d61 705f 6475 6d70 0016  n..pinmap_dump..
+00000030: 4c6f 6769 6361 6c50 696e 7300 1664 6174  LogicalPins..dat
+00000040: 615f 6c6f 6767 6572 000c 436f 6d6d 6f6e  a_logger..Common
+00000050: 000a 6468 7432 3200 185f 5f69 6e69 745f  ..dht22..__init_
+00000060: 4448 5432 3200 0a44 4854 3232 0006 6468  DHT22..DHT22..dh
+00000070: 7400 0650 696e 000e 6d61 6368 696e 6500  t..Pin..machine.
+00000080: 0c64 6874 7069 6e00 145f 5f74 656d 705f  .dhtpin..__temp_
+00000090: 6875 6d00 0e6d 6561 7375 7265 0016 7465  hum..measure..te
+000000a0: 6d70 6572 6174 7572 6500 1068 756d 6964  mperature..humid
+000000b0: 6974 7900 1474 656d 7020 5bc2 ba43 5d00  ity..temp [..C].
+000000c0: 0e68 756d 205b 255d 0008 6461 7461 001a  .hum [%]..data..
+000000d0: 6d65 6173 7572 655f 775f 636f 3200 1a6d  measure_w_co2..m
+000000e0: 6561 7375 7265 5f6d 7131 3335 000c 4c4d  easure_mq135..LM
 000000f0: 5f63 6f32 0012 636f 3220 5b70 706d 5d00  _co2..co2 [ppm].
 00000100: 0c6c 6f67 6765 7200 030a 6c6d 6465 7000  .logger...lmdep.
 00000110: 0663 6f32 000c 7069 6e6d 6170 0008 6865  .co2..pinmap..he
 00000120: 6c70 0012 5f5f 4448 545f 4f42 4a00 125f  lp..__DHT_OBJ.._
 00000130: 4c4f 475f 4e41 4d45 0006 6c6f 6700 820d  LOG_NAME..log...
 00000140: 822f 0a05 0511 6d65 6173 7572 6520 6c6f  ./....measure lo
 00000150: 673d 4661 6c73 6500 0517 6d65 6173 7572  g=False...measur
 00000160: 655f 775f 636f 3220 6c6f 673d 4661 6c73  e_w_co2 log=Fals
 00000170: 6500 0506 6c6f 6767 6572 0005 056c 6d64  e...logger...lmd
-00000180: 6570 0005 0670 696e 6d61 7000 8714 102a  ep...pinmap....*
-00000190: 012c 326c 4023 6484 0984 0988 0c88 0c84  .,2l@#d.........
-000001a0: 0c84 0984 0a80 1002 2a01 1b03 1c02 1602  ........*.......
-000001b0: 5980 1004 1005 2a02 1b06 1c04 1604 1c05  Y.....*.........
-000001c0: 1605 5980 1007 2a01 1b08 1c07 1607 5951  ..Y...*.......YQ
-000001d0: 171f 1009 1620 3200 160a 3201 1610 502a  ..... 2...2...P*
-000001e0: 0153 3302 1611 502a 0153 3303 1617 3204  .S3...P*.S3...2.
-000001f0: 1619 3205 161b 3206 161d 3207 161e 5163  ..2...2...2...Qc
-00000200: 0883 3828 100a 800c 2026 2b2b 2e12 1f51  ..8(.... &++...Q
-00000210: de44 6480 100b 2a01 1b0c 1c0b c059 8010  .Dd...*......Y..
-00000220: 0d2a 011b 0e1c 0dc1 59b0 b112 0410 0f34  .*......Y......4
-00000230: 0134 0134 0117 1f12 1f63 8170 1008 1080  .4.4.....c.p....
-00000240: 1529 120a 3400 1411 3600 5912 1f14 1236  .)..4...6.Y....6
-00000250: 0012 1f14 1336 002a 0263 8370 c101 1411  .....6.*.c.p....
-00000260: 2180 1e60 2028 3523 2f12 1034 0030 02c1  !..` (5#/..4.0..
-00000270: c22c 0212 22b1 8234 0210 1462 1222 b282  .,.."..4...b."..
-00000280: 3402 1015 62c3 b044 4f12 0712 2010 1612  4...b..DO... ...
-00000290: 23b3 3401 3482 0159 b363 8438 c101 1417  #.4.4..Y.c.8....
-000002a0: 2180 2a60 2028 3e23 2f12 1034 0030 02c1  !.*` (>#/..4.0..
-000002b0: c22c 0312 22b1 8234 0210 1462 1222 b282  .,.."..4...b."..
-000002c0: 3402 1015 6212 02b1 b234 0210 1862 c3b0  4...b....4...b..
-000002d0: 444f 1207 1220 1016 1223 b334 0134 8201  DO... ...#.4.4..
-000002e0: 59b3 6381 0808 0a19 8036 6027 1207 1220  Y.c......6`'... 
-000002f0: 3401 5910 1a63 5000 0a1b 8042 6040 101c  4.Y..cP....B`@..
-00000300: 6370 080a 1d80 4b60 6012 0510 0f34 0163  cp....K``....4.c
-00000310: 5000 0a1e 8055 6040 2300 63              P....U`@#.c
+00000180: 6570 0005 0670 696e 6d61 7000 862c 1028  ep...pinmap..,.(
+00000190: 0132 6c40 2364 8409 8409 880c 880d 840c  .2l@#d..........
+000001a0: 8409 840a 8010 0210 032a 021b 041c 0216  .........*......
+000001b0: 021c 0316 0359 8010 052a 011b 061c 0516  .....Y...*......
+000001c0: 0559 5117 1f10 0716 2032 0016 0832 0116  .YQ..... 2...2..
+000001d0: 0e50 2a01 5333 0216 0f50 2a01 5333 0316  .P*.S3...P*.S3..
+000001e0: 1532 0416 1932 0516 1b32 0616 1d32 0716  .2...2...2...2..
+000001f0: 1e51 6308 8338 2810 0880 0b20 262b 2b2e  .Qc..8(.... &++.
+00000200: 121f 51de 4464 8010 092a 011b 0a1c 09c0  ..Q.Dd...*......
+00000210: 5980 100b 2a01 1b0c 1c0b c159 b0b1 1202  Y...*......Y....
+00000220: 100d 3401 3401 3401 171f 121f 6381 7010  ..4.4.4.....c.p.
+00000230: 080e 8014 2912 0834 0014 0f36 0059 121f  ....)..4...6.Y..
+00000240: 1410 3600 121f 1411 3600 2a02 6383 70c1  ..6.....6.*.c.p.
+00000250: 0114 0f21 801d 6020 2835 232f 120e 3400  ...!..` (5#/..4.
+00000260: 3002 c1c2 2c02 1222 b182 3402 1012 6212  0...,.."..4...b.
+00000270: 22b2 8234 0210 1362 c3b0 444f 1205 1220  "..4...b..DO... 
+00000280: 1014 1223 b334 0134 8201 59b3 6385 10c9  ...#.4.4..Y.c...
+00000290: 0116 1521 8029 6020 2b28 3d23 2f80 1016  ...!.)` +(=#/...
+000002a0: 2a01 1b17 1c16 c159 120e 3400 3002 c2c3  *......Y..4.0...
+000002b0: 2c03 1222 b282 3402 1012 6212 22b3 8234  ,.."..4...b."..4
+000002c0: 0210 1362 b1b2 b334 0210 1862 c4b0 444f  ...b...4...b..DO
+000002d0: 1205 1220 1014 1223 b434 0134 8201 59b4  ... ...#.4.4..Y.
+000002e0: 6381 0808 0a19 8036 6027 1205 1220 3401  c......6`'... 4.
+000002f0: 5910 1a63 5000 0a1b 8042 6040 101c 6370  Y..cP....B`@..cp
+00000300: 080a 1d80 4b60 6012 0310 0d34 0163 5000  ....K``....4.cP.
+00000310: 0a1e 8055 6040 2300 63                   ...U`@#.c
```

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_dht22.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_dht11.mpy`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-00000000: 4d06 001f 2401 164c 4d5f 6468 7432 322e  M...$..LM_dht22.
-00000010: 7079 000f 1a6d 6561 7375 7265 5f6d 7131  py...measure_mq1
-00000020: 3335 000c 4c4d 5f63 6f32 0018 7068 7973  35..LM_co2..phys
-00000030: 6963 616c 5f70 696e 0016 7069 6e6d 6170  ical_pin..pinmap
-00000040: 5f64 756d 7000 164c 6f67 6963 616c 5069  _dump..LogicalPi
-00000050: 6e73 0016 6461 7461 5f6c 6f67 6765 7200  ns..data_logger.
-00000060: 0c43 6f6d 6d6f 6e00 0a64 6874 3232 0018  .Common..dht22..
-00000070: 5f5f 696e 6974 5f44 4854 3232 000a 4448  __init_DHT22..DH
-00000080: 5432 3200 0664 6874 0006 5069 6e00 0e6d  T22..dht..Pin..m
-00000090: 6163 6869 6e65 000c 6468 7470 696e 0014  achine..dhtpin..
-000000a0: 5f5f 7465 6d70 5f68 756d 000e 6d65 6173  __temp_hum..meas
-000000b0: 7572 6500 1674 656d 7065 7261 7475 7265  ure..temperature
-000000c0: 0010 6875 6d69 6469 7479 0014 7465 6d70  ..humidity..temp
-000000d0: 205b c2ba 435d 000e 6875 6d20 5b25 5d00   [..C]..hum [%].
-000000e0: 0864 6174 6100 1a6d 6561 7375 7265 5f77  .data..measure_w
+00000000: 4d06 001f 2401 164c 4d5f 6468 7431 312e  M...$..LM_dht11.
+00000010: 7079 000f 1870 6879 7369 6361 6c5f 7069  py...physical_pi
+00000020: 6e00 1670 696e 6d61 705f 6475 6d70 0016  n..pinmap_dump..
+00000030: 4c6f 6769 6361 6c50 696e 7300 1664 6174  LogicalPins..dat
+00000040: 615f 6c6f 6767 6572 000c 436f 6d6d 6f6e  a_logger..Common
+00000050: 000a 6468 7431 3100 185f 5f69 6e69 745f  ..dht11..__init_
+00000060: 4448 5431 3100 0a44 4854 3131 0006 6468  DHT11..DHT11..dh
+00000070: 7400 0650 696e 000e 6d61 6368 696e 6500  t..Pin..machine.
+00000080: 0c64 6874 7069 6e00 145f 5f74 656d 705f  .dhtpin..__temp_
+00000090: 6875 6d00 0e6d 6561 7375 7265 0016 7465  hum..measure..te
+000000a0: 6d70 6572 6174 7572 6500 1068 756d 6964  mperature..humid
+000000b0: 6974 7900 1474 656d 7020 5bc2 ba43 5d00  ity..temp [..C].
+000000c0: 0e68 756d 205b 255d 0008 6461 7461 001a  .hum [%]..data..
+000000d0: 6d65 6173 7572 655f 775f 636f 3200 1a6d  measure_w_co2..m
+000000e0: 6561 7375 7265 5f6d 7131 3335 000c 4c4d  easure_mq135..LM
 000000f0: 5f63 6f32 0012 636f 3220 5b70 706d 5d00  _co2..co2 [ppm].
 00000100: 0c6c 6f67 6765 7200 030a 6c6d 6465 7000  .logger...lmdep.
 00000110: 0663 6f32 000c 7069 6e6d 6170 0008 6865  .co2..pinmap..he
 00000120: 6c70 0012 5f5f 4448 545f 4f42 4a00 125f  lp..__DHT_OBJ.._
 00000130: 4c4f 475f 4e41 4d45 0006 6c6f 6700 820d  LOG_NAME..log...
 00000140: 822f 0a05 0511 6d65 6173 7572 6520 6c6f  ./....measure lo
 00000150: 673d 4661 6c73 6500 0517 6d65 6173 7572  g=False...measur
 00000160: 655f 775f 636f 3220 6c6f 673d 4661 6c73  e_w_co2 log=Fals
 00000170: 6500 0506 6c6f 6767 6572 0005 056c 6d64  e...logger...lmd
-00000180: 6570 0005 0670 696e 6d61 7000 8714 102a  ep...pinmap....*
-00000190: 012c 326c 4023 6484 0984 0988 0c88 0c84  .,2l@#d.........
-000001a0: 0c84 0984 0a80 1002 2a01 1b03 1c02 1602  ........*.......
-000001b0: 5980 1004 1005 2a02 1b06 1c04 1604 1c05  Y.....*.........
-000001c0: 1605 5980 1007 2a01 1b08 1c07 1607 5951  ..Y...*.......YQ
-000001d0: 171f 1009 1620 3200 160a 3201 1610 502a  ..... 2...2...P*
-000001e0: 0153 3302 1611 502a 0153 3303 1617 3204  .S3...P*.S3...2.
-000001f0: 1619 3205 161b 3206 161d 3207 161e 5163  ..2...2...2...Qc
-00000200: 0883 3828 100a 800c 2026 2b2b 2e12 1f51  ..8(.... &++...Q
-00000210: de44 6480 100b 2a01 1b0c 1c0b c059 8010  .Dd...*......Y..
-00000220: 0d2a 011b 0e1c 0dc1 59b0 b112 0410 0f34  .*......Y......4
-00000230: 0134 0134 0117 1f12 1f63 8170 1008 1080  .4.4.....c.p....
-00000240: 1529 120a 3400 1411 3600 5912 1f14 1236  .)..4...6.Y....6
-00000250: 0012 1f14 1336 002a 0263 8370 c101 1411  .....6.*.c.p....
-00000260: 2180 1e60 2028 3523 2f12 1034 0030 02c1  !..` (5#/..4.0..
-00000270: c22c 0212 22b1 8234 0210 1462 1222 b282  .,.."..4...b."..
-00000280: 3402 1015 62c3 b044 4f12 0712 2010 1612  4...b..DO... ...
-00000290: 23b3 3401 3482 0159 b363 8438 c101 1417  #.4.4..Y.c.8....
-000002a0: 2180 2a60 2028 3e23 2f12 1034 0030 02c1  !.*` (>#/..4.0..
-000002b0: c22c 0312 22b1 8234 0210 1462 1222 b282  .,.."..4...b."..
-000002c0: 3402 1015 6212 02b1 b234 0210 1862 c3b0  4...b....4...b..
-000002d0: 444f 1207 1220 1016 1223 b334 0134 8201  DO... ...#.4.4..
-000002e0: 59b3 6381 0808 0a19 8036 6027 1207 1220  Y.c......6`'... 
-000002f0: 3401 5910 1a63 5000 0a1b 8042 6040 101c  4.Y..cP....B`@..
-00000300: 6370 080a 1d80 4b60 6012 0510 0f34 0163  cp....K``....4.c
-00000310: 5000 0a1e 8055 6040 2300 63              P....U`@#.c
+00000180: 6570 0005 0670 696e 6d61 7000 862c 1028  ep...pinmap..,.(
+00000190: 0132 6c40 2364 8409 8409 880c 880d 840c  .2l@#d..........
+000001a0: 8409 840a 8010 0210 032a 021b 041c 0216  .........*......
+000001b0: 021c 0316 0359 8010 052a 011b 061c 0516  .....Y...*......
+000001c0: 0559 5117 1f10 0716 2032 0016 0832 0116  .YQ..... 2...2..
+000001d0: 0e50 2a01 5333 0216 0f50 2a01 5333 0316  .P*.S3...P*.S3..
+000001e0: 1532 0416 1932 0516 1b32 0616 1d32 0716  .2...2...2...2..
+000001f0: 1e51 6308 8338 2810 0880 0b20 262b 2b2e  .Qc..8(.... &++.
+00000200: 121f 51de 4464 8010 092a 011b 0a1c 09c0  ..Q.Dd...*......
+00000210: 5980 100b 2a01 1b0c 1c0b c159 b0b1 1202  Y...*......Y....
+00000220: 100d 3401 3401 3401 171f 121f 6381 7010  ..4.4.4.....c.p.
+00000230: 080e 8014 2912 0834 0014 0f36 0059 121f  ....)..4...6.Y..
+00000240: 1410 3600 121f 1411 3600 2a02 6383 70c1  ..6.....6.*.c.p.
+00000250: 0114 0f21 801d 6020 2835 232f 120e 3400  ...!..` (5#/..4.
+00000260: 3002 c1c2 2c02 1222 b182 3402 1012 6212  0...,.."..4...b.
+00000270: 22b2 8234 0210 1362 c3b0 444f 1205 1220  "..4...b..DO... 
+00000280: 1014 1223 b334 0134 8201 59b3 6385 10c9  ...#.4.4..Y.c...
+00000290: 0116 1521 8029 6020 2b28 3d23 2f80 1016  ...!.)` +(=#/...
+000002a0: 2a01 1b17 1c16 c159 120e 3400 3002 c2c3  *......Y..4.0...
+000002b0: 2c03 1222 b282 3402 1012 6212 22b3 8234  ,.."..4...b."..4
+000002c0: 0210 1362 b1b2 b334 0210 1862 c4b0 444f  ...b...4...b..DO
+000002d0: 1205 1220 1014 1223 b434 0134 8201 59b4  ... ...#.4.4..Y.
+000002e0: 6381 0808 0a19 8036 6027 1205 1220 3401  c......6`'... 4.
+000002f0: 5910 1a63 5000 0a1b 8042 6040 101c 6370  Y..cP....B`@..cp
+00000300: 080a 1d80 4b60 6012 0310 0d34 0163 5000  ....K``....4.cP.
+00000310: 0a1e 8055 6040 2300 63                   ...U`@#.c
```

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_dimmer.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_dimmer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_distance.py` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_ds18.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_ds18.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_esp32.py` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_genIO.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_genIO.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_i2c.py` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_intercon.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_intercon.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_light_sensor.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_light_sensor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_neoeffects.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_neoeffects.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_neopixel.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_neopixel.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_oled.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_oled.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_oled_sh1106.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_oled_sh1106.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_oled_ui.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_oled_ui.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_pet_feeder.py` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_ph_sensor.py` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_presence.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_presence.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_rencoder.py` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_rgb.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_rgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_roboarm.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_roboarm.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_robustness.py` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_servo.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_servo.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_stepper.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_stepper.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_switch.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_switch.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_system.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_system.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_telegram.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_telegram.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LM_tinyrgb.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_tinyrgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LP_esp32.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LP_esp32.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LP_esp32s2.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LP_esp32s2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LP_esp32s3.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LP_esp32s3.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/LogicalPins.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LogicalPins.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Network.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Network.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Notify.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Notify.mpy`

 * *Files 3% similar despite different names*

```diff
@@ -71,80 +71,80 @@
 00000460: 4375 7374 6f6d 2063 6f6d 6d61 6e64 7320  Custom commands 
 00000470: 7761 7320 7365 7400 050b 7b7d e29a 99ef  was set...{}....
 00000480: b88f 0a7b 7d00 0513 7265 706c 795f 746f  ...{}...reply_to
 00000490: 5f6d 6573 7361 6765 5f69 6400 050d 556e  _message_id...Un
 000004a0: 6b6e 6f77 6e20 6572 726f 7200 051c 4572  known error...Er
 000004b0: 726f 7220 7265 7472 6965 7669 6e67 2063  ror retrieving c
 000004c0: 6861 7420 4944 3a20 7b7d 0005 0c4e 6f41  hat ID: {}...NoA
-000004d0: 6363 6573 733a 207b 7d00 836c 100c 014c  ccess: {}..l...L
+000004d0: 6363 6573 733a 207b 7d00 836c 100c 012c  ccess: {}..l...,
 000004e0: 262c 8c08 8010 022a 011b 031c 0216 0259  &,.....*.......Y
 000004f0: 8051 1b04 1604 8010 052a 011b 061c 0516  .Q.......*......
 00000500: 0559 8010 072a 011b 081c 0716 0759 5432  .Y...*.......YT2
 00000510: 0010 0934 0216 0951 6301 865c 1024 0988  ...4...Qc..\.$..
-00000520: 0f23 2624 2843 8813 880a 8d2b 882a 8840  .#&$(C.....+.*.@
+00000520: 0e23 2624 2843 8813 880a 8d2b 882a 8840  .#&$(C.....+.*.@
 00000530: 115a 165b 1009 165c 5116 1711 5d34 0016  .Z.[...\Q...]4..
 00000540: 1123 0016 1c11 0510 0a34 0116 4251 1632  .#.......4..BQ.2
 00000550: 115e 3200 3401 160b 115e 3201 3401 1616  .^2.4....^2.4...
 00000560: 115e 5151 2a02 5333 0234 0116 1a11 5e32  .^QQ*.S3.4....^2
 00000570: 0334 0116 2211 5e32 0434 0116 3111 5e32  .4..".^2.4..1.^2
 00000580: 0534 0116 4551 6306 8674 c902 1c0b 5f80  .4..EQc..t...._.
-00000590: 1760 4046 2b37 2242 2b1f 42b0 100c d944  .`@F+7"B+.B....D
+00000590: 1660 4046 2b37 2242 2b1f 42b0 100c d944  .`@F+7"B+.B....D
 000005a0: 6412 6023 0110 0d34 0247 16c1 b114 0e10  d.`#...4.G......
 000005b0: 0f14 1032 0012 0913 1134 0136 0136 0159  ...2.....4.6.6.Y
 000005c0: 515c 5d51 6348 2b12 6023 0110 1234 0247  Q\]QcH+.`#...4.G
 000005d0: 1dc1 125d 3201 b114 1336 0014 1436 0014  ...]2....6...6..
 000005e0: 1510 0f36 0134 0134 0112 0918 1151 5c5d  ...6.4.4.....Q\]
 000005f0: 4a04 594a 015d 5163 0281 3841 084e 6380  J.YJ.]Qc..8A.Nc.
-00000600: 1f2b 00b0 5f4b 0ac1 1261 b134 012f 1442  .+.._K...a.4./.B
-00000610: 3463 8138 4108 4e63 8024 2b00 b05f 4b0a  4c.8A.Nc.$+.._K.
+00000600: 1e2b 00b0 5f4b 0ac1 1261 b134 012f 1442  .+.._K...a.4./.B
+00000610: 3463 8138 4108 4e63 8023 2b00 b05f 4b0a  4c.8A.Nc.#+.._K.
 00000620: c112 64b1 3401 2f14 4234 6383 0810 1216  ..d.4./.B4c.....
-00000630: 802a 2028 272b 2225 1209 1317 51de 4459  .* ('+"%....Q.DY
+00000630: 8029 2028 272b 2225 1209 1317 51de 4459  .) ('+"%....Q.DY
 00000640: 1205 1018 3401 c0b0 51de 4346 b010 19d9  ....4...Q.CF....
 00000650: 4442 5163 b012 0918 1712 0913 1763 8a14  DBQc.........c..
-00000660: 9390 01b0 8001 1a24 4041 8034 8007 8809  .......$@A.4....
+00000660: 9390 01b0 8001 1a24 4041 8033 8007 8809  .......$@A.3....
 00000670: 8307 2725 222d 4943 2527 287b 2835 0001  ..'%"-IC%'({(5..
 00000680: 090a b0b1 b9ba 2000 04c3 3201 c412 0914  ...... ...2.....
 00000690: 1636 00c5 b551 de44 4251 6323 0214 1bb5  .6...Q.DBQc#....
 000006a0: 1209 131c 3602 2709 2c01 2303 2304 6227  ....6.'.,.#.#.b'
 000006b0: 0a10 1dc6 b251 de44 6ab4 3400 5f4b 22c7  .....Q.Dj.4._K".
 000006c0: b310 1eb7 3482 00c8 b6b8 101f 5544 4910  ....4.......UDI.
 000006d0: 2014 1bb7 3601 4245 1261 b834 01e5 c642   ...6.BE.a.4...B
 000006e0: 1c42 5db3 101e b234 8200 c8b8 101f 5544  .B]....4......UD
 000006f0: 4910 2114 1bb2 3601 4245 1261 b834 01c6  I.!...6.BE.a.4..
-00000700: b663 0285 3081 141c 4f63 6363 631e 803c  .c..0...Occcc..<
+00000700: b663 0285 3081 141c 4f63 6363 631e 803b  .c..0...Occcc..;
 00000710: 2036 2a26 2637 2c02 b410 4162 230e 141b   6*&&7,...Ab#...
 00000720: 1209 1342 2500 3602 1024 62c5 1265 2501  ...B%.6..$b..e%.
 00000730: 1264 3402 444c 2501 b523 0f56 2501 1209  .d4.DL%..#.V%...
 00000740: 1832 1204 144b 2502 104c 2503 104d b510  .2...K%..L%..M..
 00000750: 2852 3686 0130 02c6 c7b7 6382 0008 0c50  (R6..0....c....P
-00000760: 8045 202c 2712 6212 0913 1134 0180 d944  .E ,'.b....4...D
+00000760: 8044 202c 2712 6212 0913 1134 0180 d944  .D ,'.b....4...D
 00000770: 4712 0914 2236 0059 1209 1311 638b 5c58  G..."6.Y....c.\X
-00000780: 2722 805f 6040 8516 2725 2233 2c30 2e27  '"._`@..'%"3,0.'
+00000780: 2722 805e 6040 8516 2725 2233 2c30 2e27  '".^`@..'%"3,0.'
 00000790: 2b1f 3131 06b6 2000 01c0 1209 1416 3600  +.11.. .......6.
 000007a0: c1b1 51de 4442 5163 2c04 5110 2362 5110  ..Q.DBQc,.Q.#bQ.
 000007b0: 2462 7f10 2562 5110 2662 c223 0514 1bb1  $b..%bQ.&b.#....
 000007c0: 1209 131c 3602 c312 0414 27b3 1028 5236  ....6.....'..(R6
 000007d0: 8201 3002 c427 0612 6225 0610 2955 3401  ..0..'..b%..)U4.
 000007e0: 80d8 44d3 80b0 3400 b210 2656 2506 1029  ..D...4...&V%..)
 000007f0: 557f 5510 2a55 c5b5 102b 5514 2710 2c51  U.U.*U...+U.'.,Q
 00000800: 3602 51de 4456 102d 141b b510 2b55 102e  6.Q.DV.-....+U..
 00000810: 55b5 102b 5510 2f55 3602 4247 b510 2b55  U..+U./U6.BG..+U
 00000820: 102c 55b2 1023 56b5 1024 55b5 1030 555a  .,U..#V..$U..0UZ
 00000830: b210 2456 b210 2556 b263 018a 3839 2451  ..$V..%V.c..89$Q
-00000840: 6380 6560 2022 3a51 2c29 2a2e 4b29 2c2b  c.e` ":Q,)*.K),+
+00000840: 6380 6460 2022 3a51 2c29 2a2e 4b29 2c2b  c.d` ":Q,)*.K),+
 00000850: 2c51 c125 0014 2710 1f51 3602 44d7 8012  ,Q.%..'..Q6.D...
 00000860: 6225 0010 2955 3401 80d8 44c9 8025 0010  b%..)U4...D..%..
 00000870: 2955 7f55 102a 5510 2b55 1052 55c1 1262  )U.U.*U.+U.RU..b
 00000880: 1209 1311 3401 84d7 446a 1262 1209 1311  ....4...Dj.b....
 00000890: 3401 c212 0913 1114 53b1 3601 5912 6212  4.......S.6.Y.b.
 000008a0: 0913 1134 01b2 f380 d844 4912 0914 0b10  ...4.....DI.....
 000008b0: 0c36 0159 426c 1209 140b 1012 3601 5912  .6.YBl......6.Y.
 000008c0: 6212 0913 1134 0180 d944 5725 0014 2723  b....4...DW%..'#
 000008d0: 0a23 1036 02c3 1266 2311 141b b336 0134  .#.6...f#....6.4
-000008e0: 0165 b163 931c 8010 bf80 0131 8089 6060  .e.c.......1..``
+000008e0: 0165 b163 931c 8010 bf80 0131 8088 6060  .e.c.......1..``
 000008f0: 2364 6620 890f 2725 4232 511f 432c 6929  #df ..'%B2Q.C,i)
 00000900: 7a29 522a 4c6d 2932 4924 0506 0708 0951  z)R*Lm)2I$.....Q
 00000910: 2705 101d 2706 b620 0001 2707 b5b6 b7b8  '...'.. ..'.....
 00000920: b920 0105 c012 0914 2236 00c1 b151 de44  . ......"6...Q.D
 00000930: 42b1 63b1 1024 55b1 1025 55b1 1026 555b  B.c..$U..%U..&U[
 00000940: 5ac2 2708 c3b2 51de d344 c681 2508 1209  Z.'...Q..D..%...
 00000950: 1332 dc44 bc81 b214 3310 3410 3536 0214  .2.D....3.4.56..
@@ -156,26 +156,26 @@
 000009b0: b214 3d23 0636 0144 75b2 1433 2306 101d  ..=#.6.Du..3#...
 000009c0: 3602 1414 3600 1415 3600 c4b4 8055 1209  6...6...6....U..
 000009d0: 1342 dd44 4cb0 b481 512e 0255 3401 5942  .B.DL...Q..U4.YB
 000009e0: 4b23 0714 1bb4 8055 3601 2705 4262 b214  K#.....U6.'.Bb..
 000009f0: 3d10 4336 0144 59b2 1433 1043 101d 3602  =.C6.DY..3.C..6.
 00000a00: 1414 3600 1415 3600 c4b0 b434 0159 4240  ..6...6....4.YB@
 00000a10: 4244 1044 2705 2505 6303 8100 1a0c 5463  BD.D'.%.c.....Tc
-00000a20: 6780 9420 2500 b1e5 2700 5163 8760 e206  g.. %...'.Qc.`..
-00000a30: 2255 6363 6363 6368 8098 2029 3122 5633  "Uccccch.. )1"V3
+00000a20: 6780 9320 2500 b1e5 2700 5163 8760 e206  g.. %...'.Qc.`..
+00000a30: 2255 6363 6363 6368 8097 2029 3122 5633  "Uccccch.. )1"V3
 00000a40: 502b b580 5525 04dd 44cc 8010 5614 1b10  P+..U%..D...V...
 00000a50: 5714 10b5 8055 3601 3601 2700 480d 1207  W....U6.6.'.H...
 00000a60: b510 5825 0234 8201 594a 1c57 1266 df44  ..X%.4..YJ.W.f.D
 00000a70: 55c6 490b 2502 1261 b634 0134 0159 5151  U.I.%..a.4.4.YQQ
 00000a80: c628 065d 4a01 5d12 0914 1a25 0110 4025  .(.]J.]....%..@%
 00000a90: 0336 8201 5942 5123 1214 1bb5 8055 3601  .6..YBQ#.....U6.
 00000aa0: 2700 2503 1209 1832 5163 8220 5108 4e63  '.%....2Qc. Q.Nc
-00000ab0: 80af 2b00 b05f 4b17 c1b1 143d 1059 3601  ..+.._K....=.Y6.
+00000ab0: 80ae 2b00 b05f 4b17 c1b1 143d 1059 3601  ..+.._K....=.Y6.
 00000ac0: 4434 b114 3310 5910 1d36 022f 1442 2763  D4..3.Y..6./.B'c
-00000ad0: 8810 701c 4580 c960 2027 2522 2c28 2e2c  ..p.E..` '%",(.,
+00000ad0: 8810 701c 4580 c860 2027 2522 2c28 2e2c  ..p.E..` '%",(.,
 00000ae0: 5235 1209 1416 3600 c0b0 51de 4442 5163  R5....6...Q.DBQc
 00000af0: 2308 141b b012 0913 1c36 02c1 2c01 2303  #........6..,.#.
 00000b00: 2304 62c2 2c01 2c02 1046 1047 6223 0923  #.b.,.,..F.Gb#.#
 00000b10: 0a62 2c02 1048 1047 6223 0b23 0a62 2c02  .b,..H.Gb#.#.b,.
 00000b20: 1049 1047 6223 0c23 0a62 2b03 104a 62c3  .I.Gb#.#.b+..Jb.
 00000b30: 1204 144b b110 4cb2 104d b310 2852 3686  ...K..L..M..(R6.
 00000b40: 0130 02c4 c5b5 101f 5544 4323 0d63 1261  .0......UDC#.c.a
```

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Scheduler.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Scheduler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/SocketServer.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/SocketServer.mpy`

 * *Files 7% similar despite different names*

```diff
@@ -43,196 +43,194 @@
 000002a0: 6f6e 6e5f 7175 6575 6500 0e73 6f63 706f  onn_queue..socpo
 000002b0: 7274 000c 5f5f 706f 7274 000e 736f 6374  rt..__port..soct
 000002c0: 6f75 7400 1673 6f63 5f74 696d 656f 7574  out..soc_timeout
 000002d0: 001a 6163 6365 7074 5f63 6c69 656e 7400  ..accept_client.
 000002e0: 814d 1a68 616e 646c 655f 636c 6965 6e74  .M.handle_client
 000002f0: 0014 7275 6e5f 7365 7276 6572 0018 7374  ..run_server..st
 00000300: 6172 745f 7365 7276 6572 000e 6261 636b  art_server..back
-00000310: 6c6f 6700 1a72 6570 6c79 5f6d 6573 7361  log..reply_messa
-00000320: 6765 000e 6173 796e 6369 6f00 2f2d 3582  ge..asyncio./-5.
-00000330: 2906 6d73 6700 8213 822f 4910 7265 7370  ).msg..../I.resp
-00000340: 6f6e 7365 0081 7781 590e 7265 7175 6573  onse..w.Y.reques
-00000350: 7400 0b06 636c 7300 8235 813d 146e 6577  t...cls..5.=.new
-00000360: 5f63 6c69 656e 7400 8157 051a 5b53 494d  _client..W..[SIM
-00000370: 554c 4154 4f52 204d 4f44 4520 4743 2049  ULATOR MODE GC I
-00000380: 4d50 4f52 545d 0005 155b 436c 6965 6e74  MPORT]...[Client
-00000390: 5d20 6e65 7720 636f 6e6e 3a20 7b7d 0005  ] new conn: {}..
-000003a0: 105b 436c 6965 6e74 5d20 7265 6164 207b  .[Client] read {
-000003b0: 7d00 0523 5b43 6c69 656e 745d 2053 7472  }..#[Client] Str
-000003c0: 6561 6d20 7265 6164 2065 7272 6f72 2028  eam read error (
-000003d0: 7b7d 293a 207b 7d00 0a02 0305 0000 051f  {}): {}.........
-000003e0: 5b43 6c69 656e 745d 2072 6177 2072 6571  [Client] raw req
-000003f0: 7565 7374 2028 7b7d 293a 207c 7b7d 7c00  uest ({}): |{}|.
-00000400: 0525 5b57 4152 4e5d 2043 6c69 656e 742e  .%[WARN] Client.
-00000410: 7365 6e64 2028 6175 746f 2d64 726f 7029  send (auto-drop)
-00000420: 207b 7d3a 207b 7d00 0526 5b43 6c69 656e   {}: {}..&[Clien
-00000430: 745d 2044 7261 696e 2065 7272 6f72 202d  t] Drain error -
-00000440: 3e20 636c 6f73 6520 636f 6e6e 3a20 7b7d  > close conn: {}
-00000450: 0005 1c5b 436c 6965 6e74 5d20 436c 6f73  ...[Client] Clos
-00000460: 6520 636f 6e6e 6563 7469 6f6e 207b 7d00  e connection {}.
-00000470: 051b 5b43 6c69 656e 745d 2043 6c6f 7365  ..[Client] Close
-00000480: 2065 7272 6f72 207b 7d3a 207b 7d00 0517   error {}: {}...
-00000490: 5b43 4c49 454e 545d 202d 2d2d 2023 5275  [CLIENT] --- #Ru
-000004a0: 6e20 7368 656c 6c00 051c 5b43 6c69 656e  n shell...[Clien
-000004b0: 745d 2053 6865 6c6c 2065 7863 6570 7469  t] Shell excepti
-000004c0: 6f6e 3a20 7b7d 0005 175b 4841 5d20 5368  on: {}...[HA] Sh
-000004d0: 656c 6c73 2063 6c65 616e 7570 3a20 7b7d  ells cleanup: {}
-000004e0: 0005 2d5b 4841 5d20 4372 6974 6963 616c  ..-[HA] Critical
-000004f0: 2065 7272 6f72 202d 2064 6973 636f 6e6e   error - disconn
-00000500: 6563 7420 2620 6861 7264 2072 6573 6574  ect & hard reset
-00000510: 0005 245b 4552 525d 2053 6f63 6b65 7420  ..$[ERR] Socket 
-00000520: 6372 6974 6963 616c 2065 7272 6f72 202d  critical error -
-00000530: 2072 6562 6f6f 7400 0517 5b45 5252 5d20   reboot...[ERR] 
-00000540: 6861 6e64 6c65 5f63 6c69 656e 743a 207b  handle_client: {
-00000550: 7d00 051c 4465 6c65 7465 2063 6c69 656e  }...Delete clien
-00000560: 7420 636f 6e6e 6563 7469 6f6e 3a20 7b7d  t connection: {}
-00000570: 0005 215b 2073 6f63 6b65 7420 7365 7276  ..![ socket serv
-00000580: 6572 205d 203c 3c63 6f6e 7374 7275 6374  er ] <<construct
-00000590: 6f72 3e3e 0005 134e 4557 2043 4c49 454e  or>>...NEW CLIEN
-000005a0: 5420 434f 4e4e 3a20 7b7d 0008 0530 2e30  T CONN: {}...0.0
-000005b0: 3031 052b 5b73 6572 7665 725d 2061 6363  01.+[server] acc
-000005c0: 6570 7420 6e65 7720 7b7d 202d 2061 6374  ept new {} - act
-000005d0: 6976 6520 7b7d 2074 6f75 743a 7b7d 7300  ive {} tout:{}s.
-000005e0: 052e 2d2d 2d2d 2d2d 2d20 636c 6965 6e74  ..------- client
-000005f0: 2074 696d 656f 7574 202d 2061 6363 6570   timeout - accep
-00000600: 7420 6e65 7720 636f 6e6e 6563 7469 6f6e  t new connection
-00000610: 0005 172d 2d2d 2d2d 2d2d 2063 6f6e 6e65  ...------- conne
-00000620: 6374 696f 6e20 6275 7379 0005 1843 6f6e  ction busy...Con
-00000630: 6e65 6374 696f 6e20 6973 2062 7573 792e  nection is busy.
-00000640: 2042 7965 2100 052e 5b20 736f 636b 6574   Bye!...[ socket
-00000650: 2073 6572 7665 7220 5d20 5374 6172 7420   server ] Start 
-00000660: 736f 636b 6574 2073 6572 7665 7220 6f6e  socket server on
-00000670: 207b 7d3a 7b7d 0005 292d 2054 4350 2073   {}:{}..)- TCP s
-00000680: 6572 7665 7220 7265 6164 792c 2063 6f6e  erver ready, con
-00000690: 6e65 6374 3a20 7465 6c6e 6574 207b 7d20  nect: telnet {} 
-000006a0: 7b7d 0005 205b 2073 6f63 6b65 7420 7365  {}.. [ socket se
-000006b0: 7276 6572 205d 203c 3c64 6573 7472 7563  rver ] <<destruc
-000006c0: 746f 723e 3e00 8b74 2c24 0180 0c2c 322c  tor>>..t,$...,2,
-000006d0: 2c26 2c32 2255 2775 890d 899e 8010 022a  ,&,2"U'u.......*
-000006e0: 011b 031c 0216 0259 8010 0410 052a 021b  .......Y.....*..
-000006f0: 061c 0416 041c 0516 0559 8010 072a 011b  .........Y...*..
-00000700: 081c 0716 0759 8010 092a 011b 0a1c 0916  .....Y...*......
-00000710: 0959 8051 1b0b 165e 8010 0c2a 011b 0d1c  .Y.Q...^...*....
-00000720: 0c16 0c59 8010 0e10 0f2a 021b 101c 0e16  ...Y.....*......
-00000730: 0e1c 0f16 0f59 4814 8010 1110 122a 021b  .....YH......*..
-00000740: 131c 1116 111c 1216 1259 4a1d 5911 0423  .........YJ.Y..#
-00000750: 0034 0159 8010 1110 122a 021b 141c 1116  .4.Y.....*......
-00000760: 111c 1216 1259 4a01 5d54 3200 1006 3402  .....YJ.]T2...4.
-00000770: 1606 5432 0110 1534 0216 1554 3202 1016  ..T2...4...T2...
-00000780: 3402 1616 5163 0381 5c08 0806 881b 4311  4...Qc..\.....C.
-00000790: 5f16 6010 0616 6180 161a 1162 3200 3401  _.`...a....b2.4.
-000007a0: 1617 5163 0183 0021 0a17 6380 1f31 1204  ..Qc...!..c..1..
-000007b0: 1018 1019 1206 131a f4f2 b0f2 3401 5912  ............4.Y.
-000007c0: 0657 131a 1206 131a 2232 d744 4381 4241  .W......"2.DC.BA
-000007d0: 80e5 5a18 1a51 6384 6408 2815 8828 4484  ..Z..Qc.d.(..(D.
-000007e0: 0e84 1884 1584 1584 1288 0784 1084 1911  ................
-000007f0: 5f16 6010 1516 612c 0016 4332 0016 1b32  _.`...a,..C2...2
-00000800: 0116 2d32 0216 2a32 0316 3a32 0416 3e11  ..-2..*2..:2..>.
-00000810: 6232 0534 0116 3732 0616 4932 0716 4b32  b2.4..72..I2..K2
-00000820: 0816 4d51 6309 8848 5322 1b64 1d1e 802b  ..MQc..HS".d...+
-00000830: 2424 2429 482a 321f 2724 2a52 b018 1cb1  $$$)H*2.'$*R....
-00000840: b018 1db2 b018 1e12 5e14 1f36 00b0 1820  ........^..6... 
-00000850: b013 2014 2136 0059 b214 2210 2336 01b0  .. .!6.Y..".#6..
-00000860: 1824 1206 3400 1417 2301 1425 b013 2436  .$..4...#..%..$6
-00000870: 0136 0159 1026 1425 1027 1428 b013 2480  .6.Y.&.%.'.(..$.
-00000880: 5514 2910 2736 017e 512e 0255 3601 1265  U.).'6.~Q..U6..e
-00000890: b013 2481 5534 0136 02c3 b3b0 1824 1207  ..$.U4.6.....$..
-000008a0: b013 2a34 01b0 182b 120e 3400 b018 2c51  ..*4...+..4...,Q
-000008b0: 638a 08d9 4222 2d64 8039 8007 3227 222e  c...B"-d.9..2'".
-000008c0: 5733 256c 332c 2512 0634 0014 1723 0214  W3%l3,%..4...#..
-000008d0: 25b0 1324 3601 3601 5912 0e34 00b0 182c  %..$6.6.Y..4...,
-000008e0: 481c b013 1d14 2d22 9000 3601 5e51 68c1  H.....-"..6.^Qh.
-000008f0: b114 2e10 2f36 0114 3036 00c1 4a2d 5712  ..../6..06..J-W.
-00000900: 66df 4466 c249 1c12 0634 0014 1723 0314  f.Df.I...4...#..
-00000910: 25b0 1324 b236 0236 0159 1211 3400 5923  %..$.6.6.Y..4.Y#
-00000920: 0463 5151 c228 025d 4a01 5d12 0634 0014  .cQQ.(.]J.]..4..
-00000930: 1723 0514 25b0 1324 b136 0236 0159 b110  .#..%..$.6.6.Y..
-00000940: 31d9 4346 b110 32d9 4445 52b1 2a02 6350  1.CF..2.DER.*.cP
-00000950: b12a 0263 8810 d202 1c2a 6467 8051 6026  .*.c.....*dg.Q`&
-00000960: 4b68 227a 2a58 52b0 131c 44e3 80b0 132b  Kh"z*XR...D....+
-00000970: 1433 3600 b1dc 4448 1034 1425 b136 01c1  .36...DH.4.%.6..
-00000980: 4811 b013 1e14 35b1 1436 102f 3601 3601  H.....5..6./6.6.
-00000990: 594a 2b57 1266 df44 64c2 491a 1215 1437  YJ+W.f.Dd.I....7
-000009a0: b013 2436 0159 1205 2306 1425 b013 24b2  ..$6.Y..#..%..$.
-000009b0: 3602 3401 5951 51c2 2802 5d4a 015d 125e  6.4.YQQ.(.]J.].^
-000009c0: 1438 3600 1439 b014 3a36 0036 0159 4246  .86..9..:6.6.YBF
-000009d0: 1268 b134 0159 5163 8630 c942 183a 6480  .h.4.YQc.0.B.:d.
-000009e0: 6660 406b 2862 7630 52b0 1320 143b 3600  f`@k(bv0R.. .;6.
-000009f0: 5e51 6859 b013 2014 3c36 0059 480d b013  ^QhY.. .<6.YH...
-00000a00: 1e14 3d36 005e 5168 594a 2b57 1266 df44  ..=6.^QhYJ+W.f.D
-00000a10: 64c1 491a 1206 3400 1417 2307 1425 b136  d.I...4...#..%.6
-00000a20: 0136 0159 b014 3e36 005e 5168 5951 51c1  .6.Y..>6.^QhYQQ.
-00000a30: 2801 5d4a 015d b013 2014 2136 0059 5163  (.]J.].. .!6.YQc
-00000a40: 8930 d142 1e3e 6480 7b32 4828 2c22 2856  .0.B.>d.{2H(,"(V
-00000a50: 3c24 454a 1206 3400 1417 2308 1425 b013  <$EJ..4...#..%..
-00000a60: 2436 0136 0159 b014 2a10 3f36 0159 b013  $6.6.Y..*.?6.Y..
-00000a70: 2b14 4036 0059 125e 1441 2232 3601 5e51  +.@6.Y.^.A"26.^Q
-00000a80: 6859 4815 b013 1e14 3e36 0059 b013 1e14  hYH.....>6.Y....
-00000a90: 4236 005e 5168 594a 2557 1266 df44 5ec1  B6.^QhYJ%W.f.D^.
-00000aa0: 4914 1206 3400 1417 2309 1425 b013 24b1  I...4...#..%..$.
-00000ab0: 3602 3601 5951 51c1 2801 5d4a 015d 50b0  6.6.YQQ.(.]J.]P.
-00000ac0: 181c 8012 0618 1a12 1514 37b0 1324 3601  ..........7..$6.
-00000ad0: 5912 1134 0059 5163 8370 390c 3724 808e  Y..4.YQc.p9.7$..
-00000ae0: 2f4a 1215 1343 1444 b051 3602 51de d344  /J...C.D.Q6.Q..D
-00000af0: 4a12 1513 4314 45b0 3601 5912 0c34 0014  J...C.E.6.Y..4..
-00000b00: 4610 4714 2812 6912 1513 4314 4836 0034  F.G.(.i...C.H6.4
-00000b10: 0136 0136 0159 5163 8750 da42 2049 646a  .6.6.YQc.P.B Idj
-00000b20: 8095 222b 2923 4d26 2930 2b25 3048 1b12  .."+)#M&)0+%0H..
-00000b30: 0634 0014 1723 0a36 0159 b013 2b14 2bb1  .4...#.6.Y..+.+.
-00000b40: 3601 c2b2 4442 5263 4a33 5712 66df 446c  6...DBRcJ3W.f.Dl
-00000b50: c349 2210 4ab3 dd44 49b0 143e 3600 5e51  .I".J..DI..>6.^Q
-00000b60: 6859 1206 3400 1417 230b 1425 b336 0136  hY..4...#..%.6.6
-00000b70: 0159 5063 5151 c328 035d 4a01 5d12 1134  .YPcQQ.(.]J.]..4
-00000b80: 0059 b014 2a23 0c14 2512 1234 0036 0136  .Y..*#..%..4.6.6
-00000b90: 0159 5263 8a68 d142 244b 6480 a57b 4d23  .YRc.h.B$Kd..{M#
-00000ba0: 422c 2344 2a23 2827 532c 5212 0c34 0014  B,#D*#('S,R..4..
-00000bb0: 4610 4714 2812 6912 1513 4314 4836 0034  F.G.(.i...C.H6.4
-00000bc0: 0136 0136 0159 b014 2ab0 132b 1433 3600  .6.6.Y..*..+.36.
-00000bd0: 3601 5942 dc80 4839 b014 2d36 005e 5168  6.YB..H9..-6.^Qh
-00000be0: 3002 c1c2 b144 4440 ce80 01b0 1449 b236  0....DD@.....I.6
-00000bf0: 015e 5168 c1b1 4357 b014 2a23 0d36 0159  .^Qh..CW..*#.6.Y
-00000c00: 1205 230e 3401 59b0 132b 144c 3600 594a  ..#.4.Y..+.L6.YJ
-00000c10: 2157 1266 df44 5ac3 4910 1205 230f 1425  !W.f.DZ.I...#..%
-00000c20: b336 0134 0159 4050 0251 51c3 2803 5d4a  .6.4.Y@P.QQ.(.]J
-00000c30: 015d b013 1c43 9e7f b014 3e36 005e 5168  .]...C....>6.^Qh
-00000c40: 5951 6382 0029 0a4d 6480 bd25 1211 3400  YQc..).Md..%..4.
-00000c50: 5912 0634 0014 1723 1014 25b0 1324 3601  Y..4...#..%..$6.
-00000c60: 3601 5951 6383 7410 2116 88c6 8007 4386  6.YQc.t.!.....C.
-00000c70: 1b84 2884 1384 0a88 0a00 115f 1660 1016  ..(........_.`..
-00000c80: 1661 5116 4fb0 2000 0116 4e32 0116 5732  .aQ.O. ...N2..W2
-00000c90: 0216 5932 0316 5a11 6232 0434 0116 5d32  ..Y2..Z.b2.4..]2
-00000ca0: 0516 4db0 6306 8728 2a20 4e6b 6c80 d060  ..M.c..(* Nkl..`
-00000cb0: 4049 4e28 2767 4c2b 4f2b 1216 134f 51de  @IN('gL+O+...OQ.
-00000cc0: 44d5 8012 6d25 00b1 154e b136 0112 1618  D...m%...N.6....
-00000cd0: 4f10 3212 1613 4f18 5051 1216 134f 1851  O.2...O.PQ...O.Q
-00000ce0: 8212 1613 4f18 5212 0210 5334 0112 1613  ....O.R...S4....
-00000cf0: 4f18 5412 6e12 0210 5534 0134 01c2 b285  O.T.n...U4.4....
-00000d00: d744 4385 4241 b212 1613 4f18 5612 0634  .DC.BA....O.V..4
-00000d10: 0014 1723 1136 0159 1216 134f 638e 2092  ...#.6.Y...Oc. .
-00000d20: 5036 576c 6f80 eb80 0764 5627 6530 222f  P6Wlo....dV'e0"/
-00000d30: 3336 4c2b 2922 6923 454b 2829 22b1 1324  36L+)"i#EK()"..$
-00000d40: c212 7012 6912 1513 4314 4836 0034 0134  ..p.i...C.H6.4.4
-00000d50: 01b0 1352 d744 4cb1 1215 1343 b256 52b2  ...R.DL....C.VR.
-00000d60: 2a02 6312 0634 0014 1723 1214 25b2 3601  *.c..4...#..%.6.
-00000d70: 3601 5950 c312 1513 4314 5836 005f 4b58  6.YP....C.X6._KX
-00000d80: 3002 c4c5 126e 120f 120e 3400 b513 2c34  0....n....4...,4
-00000d90: 0223 13f4 3401 c612 0634 0014 1723 1414  .#..4....4...#..
-00000da0: 25b2 b4b0 1356 b6f3 3603 3601 59b5 131c  %....V..6.6.Y...
-00000db0: 4447 b6b0 1356 d844 5c12 0634 0014 1723  DG...V.D\..4...#
-00000dc0: 1536 0159 b514 3e36 005e 5168 5952 c359  .6.Y..>6.^QhYR.Y
-00000dd0: 5959 5942 4342 a67f b344 4552 b22a 0263  YYYBCB...DER.*.c
-00000de0: 1206 3400 1417 2316 3601 59b1 142a 2317  ..4...#.6.Y..*#.
-00000df0: 3601 59b1 143e 3600 5e51 6859 2801 50b2  6.Y..>6.^QhY(.P.
-00000e00: 2a02 6383 18c3 4018 596c 1d1e 9013 6060  *.c...@.Yl....``
-00000e10: 672d 6362 1215 b1b2 3402 c3b0 1457 b336  g-cb....4....W.6
-00000e20: 015e 5168 3002 c4c5 b443 4251 63b3 144b  .^Qh0....CBQc..K
-00000e30: 3600 5e51 6859 5163 8560 c140 125a 6c90  6.^QhYQc.`.@.Zl.
-00000e40: 2660 2933 3827 1209 3400 8155 8055 c112  &`)38'..4..U.U..
-00000e50: 0634 0014 1723 1814 25b1 b013 5436 0236  .4...#..%...T6.6
-00000e60: 0159 125e 145b b013 59b0 1350 b013 5410  .Y.^.[..Y..P..T.
-00000e70: 5cb0 1352 3682 03b0 1851 b013 515e 5168  \..R6....Q..Q^Qh
-00000e80: 5912 0634 0014 1723 1914 25b1 b013 5436  Y..4...#..%...T6
-00000e90: 0236 0159 5163 8248 4910 5d63 9031 6020  .6.YQc.HI.]c.1` 
-00000ea0: 2f25 1215 1343 1458 3600 5f4b 1230 02c1  /%...C.X6._K.0..
-00000eb0: c2b2 131c 4447 b214 2ab0 3601 5942 2c51  ....DG..*.6.YB,Q
-00000ec0: 6381 6019 0a4d 6c90 3a2b 1206 3400 1417  c.`..Ml.:+..4...
-00000ed0: 231a 3601 59b0 1351 143e 3600 5951 63    #.6.Y..Q.>6.YQc
+00000310: 6c6f 6700 0a72 6570 6c79 000e 6173 796e  log..reply..asyn
+00000320: 6369 6f00 2f2d 3582 2906 6d73 6700 8213  cio./-5.).msg...
+00000330: 822f 4910 7265 7370 6f6e 7365 0081 7781  ./I.response..w.
+00000340: 590e 7265 7175 6573 7400 0b06 636c 7300  Y.request...cls.
+00000350: 8235 813d 146e 6577 5f63 6c69 656e 7400  .5.=.new_client.
+00000360: 8157 051a 5b53 494d 554c 4154 4f52 204d  .W..[SIMULATOR M
+00000370: 4f44 4520 4743 2049 4d50 4f52 545d 0005  ODE GC IMPORT]..
+00000380: 155b 436c 6965 6e74 5d20 6e65 7720 636f  .[Client] new co
+00000390: 6e6e 3a20 7b7d 0005 105b 436c 6965 6e74  nn: {}...[Client
+000003a0: 5d20 7265 6164 207b 7d00 0523 5b43 6c69  ] read {}..#[Cli
+000003b0: 656e 745d 2053 7472 6561 6d20 7265 6164  ent] Stream read
+000003c0: 2065 7272 6f72 2028 7b7d 293a 207b 7d00   error ({}): {}.
+000003d0: 0a02 0305 0000 051f 5b43 6c69 656e 745d  ........[Client]
+000003e0: 2072 6177 2072 6571 7565 7374 2028 7b7d   raw request ({}
+000003f0: 293a 207c 7b7d 7c00 0525 5b57 4152 4e5d  ): |{}|..%[WARN]
+00000400: 2043 6c69 656e 742e 7365 6e64 2028 6175   Client.send (au
+00000410: 746f 2d64 726f 7029 207b 7d3a 207b 7d00  to-drop) {}: {}.
+00000420: 0526 5b43 6c69 656e 745d 2044 7261 696e  .&[Client] Drain
+00000430: 2065 7272 6f72 202d 3e20 636c 6f73 6520   error -> close 
+00000440: 636f 6e6e 3a20 7b7d 0005 1c5b 436c 6965  conn: {}...[Clie
+00000450: 6e74 5d20 436c 6f73 6520 636f 6e6e 6563  nt] Close connec
+00000460: 7469 6f6e 207b 7d00 051b 5b43 6c69 656e  tion {}...[Clien
+00000470: 745d 2043 6c6f 7365 2065 7272 6f72 207b  t] Close error {
+00000480: 7d3a 207b 7d00 0517 5b43 4c49 454e 545d  }: {}...[CLIENT]
+00000490: 202d 2d2d 2023 5275 6e20 7368 656c 6c00   --- #Run shell.
+000004a0: 051c 5b43 6c69 656e 745d 2053 6865 6c6c  ..[Client] Shell
+000004b0: 2065 7863 6570 7469 6f6e 3a20 7b7d 0005   exception: {}..
+000004c0: 175b 4841 5d20 5368 656c 6c73 2063 6c65  .[HA] Shells cle
+000004d0: 616e 7570 3a20 7b7d 0005 2d5b 4841 5d20  anup: {}..-[HA] 
+000004e0: 4372 6974 6963 616c 2065 7272 6f72 202d  Critical error -
+000004f0: 2064 6973 636f 6e6e 6563 7420 2620 6861   disconnect & ha
+00000500: 7264 2072 6573 6574 0005 245b 4552 525d  rd reset..$[ERR]
+00000510: 2053 6f63 6b65 7420 6372 6974 6963 616c   Socket critical
+00000520: 2065 7272 6f72 202d 2072 6562 6f6f 7400   error - reboot.
+00000530: 0517 5b45 5252 5d20 6861 6e64 6c65 5f63  ..[ERR] handle_c
+00000540: 6c69 656e 743a 207b 7d00 051c 4465 6c65  lient: {}...Dele
+00000550: 7465 2063 6c69 656e 7420 636f 6e6e 6563  te client connec
+00000560: 7469 6f6e 3a20 7b7d 0005 215b 2073 6f63  tion: {}..![ soc
+00000570: 6b65 7420 7365 7276 6572 205d 203c 3c63  ket server ] <<c
+00000580: 6f6e 7374 7275 6374 6f72 3e3e 0005 134e  onstructor>>...N
+00000590: 4557 2043 4c49 454e 5420 434f 4e4e 3a20  EW CLIENT CONN: 
+000005a0: 7b7d 0008 0530 2e30 3031 052b 5b73 6572  {}...0.001.+[ser
+000005b0: 7665 725d 2061 6363 6570 7420 6e65 7720  ver] accept new 
+000005c0: 7b7d 202d 2061 6374 6976 6520 7b7d 2074  {} - active {} t
+000005d0: 6f75 743a 7b7d 7300 052e 2d2d 2d2d 2d2d  out:{}s...------
+000005e0: 2d20 636c 6965 6e74 2074 696d 656f 7574  - client timeout
+000005f0: 202d 2061 6363 6570 7420 6e65 7720 636f   - accept new co
+00000600: 6e6e 6563 7469 6f6e 0005 172d 2d2d 2d2d  nnection...-----
+00000610: 2d2d 2063 6f6e 6e65 6374 696f 6e20 6275  -- connection bu
+00000620: 7379 0005 1843 6f6e 6e65 6374 696f 6e20  sy...Connection 
+00000630: 6973 2062 7573 792e 2042 7965 2100 052e  is busy. Bye!...
+00000640: 5b20 736f 636b 6574 2073 6572 7665 7220  [ socket server 
+00000650: 5d20 5374 6172 7420 736f 636b 6574 2073  ] Start socket s
+00000660: 6572 7665 7220 6f6e 207b 7d3a 7b7d 0005  erver on {}:{}..
+00000670: 292d 2054 4350 2073 6572 7665 7220 7265  )- TCP server re
+00000680: 6164 792c 2063 6f6e 6e65 6374 3a20 7465  ady, connect: te
+00000690: 6c6e 6574 207b 7d20 7b7d 0005 205b 2073  lnet {} {}.. [ s
+000006a0: 6f63 6b65 7420 7365 7276 6572 205d 203c  ocket server ] <
+000006b0: 3c64 6573 7472 7563 746f 723e 3e00 8b74  <destructor>>..t
+000006c0: 2c24 0180 0c2c 322c 2c26 2c32 2255 2775  ,$...,2,,&,2"U'u
+000006d0: 890d 899e 8010 022a 011b 031c 0216 0259  .......*.......Y
+000006e0: 8010 0410 052a 021b 061c 0416 041c 0516  .....*..........
+000006f0: 0559 8010 072a 011b 081c 0716 0759 8010  .Y...*.......Y..
+00000700: 092a 011b 0a1c 0916 0959 8051 1b0b 165e  .*.......Y.Q...^
+00000710: 8010 0c2a 011b 0d1c 0c16 0c59 8010 0e10  ...*.......Y....
+00000720: 0f2a 021b 101c 0e16 0e1c 0f16 0f59 4814  .*...........YH.
+00000730: 8010 1110 122a 021b 131c 1116 111c 1216  .....*..........
+00000740: 1259 4a1d 5911 0423 0034 0159 8010 1110  .YJ.Y..#.4.Y....
+00000750: 122a 021b 141c 1116 111c 1216 1259 4a01  .*...........YJ.
+00000760: 5d54 3200 1006 3402 1606 5432 0110 1534  ]T2...4...T2...4
+00000770: 0216 1554 3202 1016 3402 1616 5163 0381  ...T2...4...Qc..
+00000780: 5c08 0806 881b 4311 5f16 6010 0616 6180  \.....C._.`...a.
+00000790: 161a 1162 3200 3401 1617 5163 0183 0021  ...b2.4...Qc...!
+000007a0: 0a17 6380 1f31 1204 1018 1019 1206 131a  ..c..1..........
+000007b0: f4f2 b0f2 3401 5912 0657 131a 1206 131a  ....4.Y..W......
+000007c0: 2232 d744 4381 4241 80e5 5a18 1a51 6384  "2.DC.BA..Z..Qc.
+000007d0: 6408 2815 8828 4484 0e84 1884 1584 1584  d.(..(D.........
+000007e0: 1288 0784 1084 1911 5f16 6010 1516 612c  ........_.`...a,
+000007f0: 0016 4332 0016 1b32 0116 2d32 0216 2a32  ..C2...2..-2..*2
+00000800: 0316 3a32 0416 3e11 6232 0534 0116 3732  ..:2..>.b2.4..72
+00000810: 0616 4932 0716 4b32 0816 4d51 6309 8838  ..I2..K2..MQc..8
+00000820: 5322 1b64 1d1e 802b 2424 2429 482a 301f  S".d...+$$$)H*0.
+00000830: 2724 2a52 b018 1cb1 b018 1db2 b018 1e12  '$*R............
+00000840: 5e14 1f36 00b0 1820 b013 2014 2136 0059  ^..6... .. .!6.Y
+00000850: b214 2210 2336 01b0 1824 1206 1417 2301  ..".#6...$....#.
+00000860: 1425 b013 2436 0136 0159 1026 1425 1027  .%..$6.6.Y.&.%.'
+00000870: 1428 b013 2480 5514 2910 2736 017e 512e  .(..$.U.).'6.~Q.
+00000880: 0255 3601 1265 b013 2481 5534 0136 02c3  .U6..e..$.U4.6..
+00000890: b3b0 1824 1207 b013 2a34 01b0 182b 120e  ...$....*4...+..
+000008a0: 3400 b018 2c51 6389 58d9 4222 2d64 8039  4...,Qc.X.B"-d.9
+000008b0: 8007 3027 222e 5731 256c 312c 2512 0614  ..0'".W1%l1,%...
+000008c0: 1723 0214 25b0 1324 3601 3601 5912 0e34  .#..%..$6.6.Y..4
+000008d0: 00b0 182c 481c b013 1d14 2d22 9000 3601  ...,H.....-"..6.
+000008e0: 5e51 68c1 b114 2e10 2f36 0114 3036 00c1  ^Qh...../6..06..
+000008f0: 4a2b 5712 66df 4464 c249 1a12 0614 1723  J+W.f.Dd.I.....#
+00000900: 0314 25b0 1324 b236 0236 0159 1211 3400  ..%..$.6.6.Y..4.
+00000910: 5923 0463 5151 c228 025d 4a01 5d12 0614  Y#.cQQ.(.]J.]...
+00000920: 1723 0514 25b0 1324 b136 0236 0159 b110  .#..%..$.6.6.Y..
+00000930: 31d9 4346 b110 32d9 4445 52b1 2a02 6350  1.CF..2.DER.*.cP
+00000940: b12a 0263 8810 d202 1c2a 6467 8051 6026  .*.c.....*dg.Q`&
+00000950: 4b68 227a 2a58 52b0 131c 44e3 80b0 132b  Kh"z*XR...D....+
+00000960: 1433 3600 b1dc 4448 1034 1425 b136 01c1  .36...DH.4.%.6..
+00000970: 4811 b013 1e14 35b1 1436 102f 3601 3601  H.....5..6./6.6.
+00000980: 594a 2b57 1266 df44 64c2 491a 1215 1437  YJ+W.f.Dd.I....7
+00000990: b013 2436 0159 1205 2306 1425 b013 24b2  ..$6.Y..#..%..$.
+000009a0: 3602 3401 5951 51c2 2802 5d4a 015d 125e  6.4.YQQ.(.]J.].^
+000009b0: 1438 3600 1439 b014 3a36 0036 0159 4246  .86..9..:6.6.YBF
+000009c0: 1268 b134 0159 5163 8620 c942 183a 6480  .h.4.YQc. .B.:d.
+000009d0: 6660 406b 2862 762e 52b0 1320 143b 3600  f`@k(bv.R.. .;6.
+000009e0: 5e51 6859 b013 2014 3c36 0059 480d b013  ^QhY.. .<6.YH...
+000009f0: 1e14 3d36 005e 5168 594a 2957 1266 df44  ..=6.^QhYJ)W.f.D
+00000a00: 62c1 4918 1206 1417 2307 1425 b136 0136  b.I.....#..%.6.6
+00000a10: 0159 b014 3e36 005e 5168 5951 51c1 2801  .Y..>6.^QhYQQ.(.
+00000a20: 5d4a 015d b013 2014 2136 0059 5163 8910  ]J.].. .!6.YQc..
+00000a30: d142 1e3e 6480 7b30 4828 2c22 2856 3a24  .B.>d.{0H(,"(V:$
+00000a40: 454a 1206 1417 2308 1425 b013 2436 0136  EJ....#..%..$6.6
+00000a50: 0159 b014 2a10 3f36 0159 b013 2b14 4036  .Y..*.?6.Y..+.@6
+00000a60: 0059 125e 1441 2232 3601 5e51 6859 4815  .Y.^.A"26.^QhYH.
+00000a70: b013 1e14 3e36 0059 b013 1e14 4236 005e  ....>6.Y....B6.^
+00000a80: 5168 594a 2357 1266 df44 5cc1 4912 1206  QhYJ#W.f.D\.I...
+00000a90: 1417 2309 1425 b013 24b1 3602 3601 5951  ..#..%..$.6.6.YQ
+00000aa0: 51c1 2801 5d4a 015d 50b0 181c 8012 0618  Q.(.]J.]P.......
+00000ab0: 1a12 1514 37b0 1324 3601 5912 1134 0059  ....7..$6.Y..4.Y
+00000ac0: 5163 8370 390c 3724 808e 2f4a 1215 1343  Qc.p9.7$../J...C
+00000ad0: 1444 b051 3602 51de d344 4a12 1513 4314  .D.Q6.Q..DJ...C.
+00000ae0: 45b0 3601 5912 0c34 0014 4610 4714 2812  E.6.Y..4..F.G.(.
+00000af0: 6912 1513 4314 4836 0034 0136 0136 0159  i...C.H6.4.6.6.Y
+00000b00: 5163 8730 da42 2049 646a 8095 2229 2923  Qc.0.B Idj.."))#
+00000b10: 4d26 292e 2b25 3048 1912 0614 1723 0a36  M&).+%0H.....#.6
+00000b20: 0159 b013 2b14 2bb1 3601 c2b2 4442 5263  .Y..+.+.6...DBRc
+00000b30: 4a31 5712 66df 446a c349 2010 4ab3 dd44  J1W.f.Dj.I .J..D
+00000b40: 49b0 143e 3600 5e51 6859 1206 1417 230b  I..>6.^QhY....#.
+00000b50: 1425 b336 0136 0159 5063 5151 c328 035d  .%.6.6.YPcQQ.(.]
+00000b60: 4a01 5d12 1134 0059 b014 2a23 0c14 2512  J.]..4.Y..*#..%.
+00000b70: 1234 0036 0136 0159 5263 8a68 d142 244b  .4.6.6.YRc.h.B$K
+00000b80: 6480 a57b 4d23 422c 2344 2a23 2827 532c  d..{M#B,#D*#('S,
+00000b90: 5212 0c34 0014 4610 4714 2812 6912 1513  R..4..F.G.(.i...
+00000ba0: 4314 4836 0034 0136 0136 0159 b014 2ab0  C.H6.4.6.6.Y..*.
+00000bb0: 132b 1433 3600 3601 5942 dc80 4839 b014  .+.36.6.YB..H9..
+00000bc0: 2d36 005e 5168 3002 c1c2 b144 4440 ce80  -6.^Qh0....DD@..
+00000bd0: 01b0 1449 b236 015e 5168 c1b1 4357 b014  ...I.6.^Qh..CW..
+00000be0: 2a23 0d36 0159 1205 230e 3401 59b0 132b  *#.6.Y..#.4.Y..+
+00000bf0: 144c 3600 594a 2157 1266 df44 5ac3 4910  .L6.YJ!W.f.DZ.I.
+00000c00: 1205 230f 1425 b336 0134 0159 4050 0251  ..#..%.6.4.Y@P.Q
+00000c10: 51c3 2803 5d4a 015d b013 1c43 9e7f b014  Q.(.]J.]...C....
+00000c20: 3e36 005e 5168 5951 6381 7029 0a4d 6480  >6.^QhYQc.p).Md.
+00000c30: bd25 1211 3400 5912 0614 1723 1014 25b0  .%..4.Y....#..%.
+00000c40: 1324 3601 3601 5951 6383 7410 2116 88c6  .$6.6.YQc.t.!...
+00000c50: 8007 4386 1b84 2884 1384 0a88 0a00 115f  ..C...(........_
+00000c60: 1660 1016 1661 5116 4fb0 2000 0116 4e32  .`...aQ.O. ...N2
+00000c70: 0116 5732 0216 5932 0316 5a11 6232 0434  ..W2..Y2..Z.b2.4
+00000c80: 0116 5d32 0516 4db0 6306 8718 2a20 4e6b  ..]2..M.c...* Nk
+00000c90: 6c80 d060 4049 4e28 2767 4c2b 4f29 1216  l..`@IN('gL+O)..
+00000ca0: 134f 51de 44d3 8012 6d25 00b1 154e b136  .OQ.D...m%...N.6
+00000cb0: 0112 1618 4f10 3212 1613 4f18 5051 1216  ....O.2...O.PQ..
+00000cc0: 134f 1851 8212 1613 4f18 5212 0210 5334  .O.Q....O.R...S4
+00000cd0: 0112 1613 4f18 5412 6e12 0210 5534 0134  ....O.T.n...U4.4
+00000ce0: 01c2 b285 d744 4385 4241 b212 1613 4f18  .....DC.BA....O.
+00000cf0: 5612 0614 1723 1136 0159 1216 134f 638d  V....#.6.Y...Oc.
+00000d00: 6092 5036 576c 6f80 eb80 0764 5627 652e  `.P6Wlo....dV'e.
+00000d10: 222f 3334 4c29 2922 6923 4549 2829 22b1  "/34L))"i#EI()".
+00000d20: 1324 c212 7012 6912 1513 4314 4836 0034  .$..p.i...C.H6.4
+00000d30: 0134 01b0 1352 d744 4cb1 1215 1343 b256  .4...R.DL....C.V
+00000d40: 52b2 2a02 6312 0614 1723 1214 25b2 3601  R.*.c....#..%.6.
+00000d50: 3601 5950 c312 1513 4314 5836 005f 4b54  6.YP....C.X6._KT
+00000d60: 3002 c4c5 126e 120f 120e 3400 b513 2c34  0....n....4...,4
+00000d70: 0223 13f4 3401 c612 0614 1723 1414 25b2  .#..4......#..%.
+00000d80: b4b0 1356 b6f3 3603 3601 59b5 131c 4447  ...V..6.6.Y...DG
+00000d90: b6b0 1356 d844 5a12 0614 1723 1536 0159  ...V.DZ....#.6.Y
+00000da0: b514 3e36 005e 5168 5952 c359 5959 5942  ..>6.^QhYR.YYYYB
+00000db0: 4342 aa7f b344 4552 b22a 0263 1206 1417  CB...DER.*.c....
+00000dc0: 2316 3601 59b1 142a 2317 3601 59b1 143e  #.6.Y..*#.6.Y..>
+00000dd0: 3600 5e51 6859 2801 50b2 2a02 6383 18c3  6.^QhY(.P.*.c...
+00000de0: 4018 596c 1d1e 9013 6060 672d 6362 1215  @.Yl....``g-cb..
+00000df0: b1b2 3402 c3b0 1457 b336 015e 5168 3002  ..4....W.6.^Qh0.
+00000e00: c4c5 b443 4251 63b3 144b 3600 5e51 6859  ...CBQc..K6.^QhY
+00000e10: 5163 8540 c140 125a 6c90 2660 2931 3827  Qc.@.@.Zl.&`)18'
+00000e20: 1209 3400 8155 8055 c112 0614 1723 1814  ..4..U.U.....#..
+00000e30: 25b1 b013 5436 0236 0159 125e 145b b013  %...T6.6.Y.^.[..
+00000e40: 59b0 1350 b013 5410 5cb0 1352 3682 03b0  Y..P..T.\..R6...
+00000e50: 1851 b013 515e 5168 5912 0614 1723 1914  .Q..Q^QhY....#..
+00000e60: 25b1 b013 5436 0236 0159 5163 8248 4910  %...T6.6.YQc.HI.
+00000e70: 5d63 9031 6020 2f25 1215 1343 1458 3600  ]c.1` /%...C.X6.
+00000e80: 5f4b 1230 02c1 c2b2 131c 4447 b214 2ab0  _K.0......DG..*.
+00000e90: 3601 5942 2c51 6381 5019 0a4d 6c90 3a29  6.YB,Qc.P..Ml.:)
+00000ea0: 1206 1417 231a 3601 59b0 1351 143e 3600  ....#.6.Y..Q.>6.
+00000eb0: 5951 63                                  YQc
```

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/TaskManager.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/TaskManager.mpy`

 * *Files 23% similar despite different names*

```diff
@@ -1,343 +1,364 @@
-00000000: 4d06 001f 8119 1a1c 5461 736b 4d61 6e61  M.......TaskMana
+00000000: 4d06 001f 8122 1d1c 5461 736b 4d61 6e61  M...."..TaskMana
 00000010: 6765 722e 7079 000f 0e6d 6f64 756c 6573  ger.py...modules
 00000020: 0006 7379 7300 0a64 756d 7073 0008 6a73  ..sys..dumps..js
 00000030: 6f6e 0010 7363 6865 6475 6c65 0081 6710  on..schedule..g.
 00000040: 7561 7379 6e63 696f 001a 636f 6e73 6f6c  uasyncio..consol
 00000050: 655f 7772 6974 6500 1465 7272 6c6f 675f  e_write..errlog_
 00000060: 6164 6400 0a44 6562 7567 000c 6366 6767  add..Debug..cfgg
 00000070: 6574 001a 436f 6e66 6967 4861 6e64 6c65  et..ConfigHandle
 00000080: 7200 1074 6963 6b73 5f6d 7300 1474 6963  r..ticks_ms..tic
-00000090: 6b73 5f64 6966 6600 0a75 7469 6d65 0008  ks_diff..utime..
-000000a0: 5461 736b 000e 4d61 6e61 6765 7200 1061  Task..Manager..a
-000000b0: 696f 7175 6575 6500 1865 7865 635f 6c6d  ioqueue..exec_lm
-000000c0: 5f70 6970 6500 8227 066e 2f61 0082 2302  _pipe..'.n/a..#.
-000000d0: 3b00 8129 2a65 7865 635f 6c6d 5f70 6970  ;..)*exec_lm_pip
-000000e0: 655f 7363 6865 6475 6c65 0018 6578 6563  e_schedule..exec
-000000f0: 5f6c 6d5f 636f 7265 001a 5f65 7865 635f  _lm_core.._exec_
-00000100: 6c6d 5f63 6f72 6500 0a3e 6a73 6f6e 000a  lm_core..>json..
-00000110: 4c4d 5f7b 7d00 0981 5112 696d 706f 7274  LM_{}...Q.import
-00000120: 207b 7d00 127b 7d2e 7b7d 287b 7d29 0081   {}..{}.{}({})..
-00000130: 552a 6578 6563 5f6c 6d5f 636f 7265 5f73  U*exec_lm_core_s
-00000140: 6368 6564 756c 6500 2314 5f5f 6361 6c6c  chedule.#.__call
-00000150: 6261 636b 0010 5f5f 696e 6c6f 6f70 000e  back..__inloop..
-00000160: 5f5f 736c 6565 7000 0874 6173 6b00 0864  __sleep..task..d
-00000170: 6f6e 6500 0306 6f75 7400 0674 6167 000e  one...out..tag..
-00000180: 6973 5f62 7573 7900 0a54 4153 4b53 0081  is_busy..TASKS..
-00000190: 2d14 5f5f 7461 736b 5f64 656c 0019 1b0c  -.__task_del....
-000001a0: 6372 6561 7465 000a 6169 6f7b 7d00 1c67  create..aio{}..g
-000001b0: 6574 5f65 7665 6e74 5f6c 6f6f 7000 1663  et_event_loop..c
-000001c0: 7265 6174 655f 7461 736b 0012 6372 6561  reate_task..crea
-000001d0: 7465 5f6c 6d00 022e 0018 7461 736b 5f77  te_lm.....task_w
-000001e0: 7261 7070 6572 000c 6361 6e63 656c 0010  rapper..cancel..
-000001f0: 736c 6565 705f 6d73 000c 6d73 676f 626a  sleep_ms..msgobj
-00000200: 0014 5f5f 6d73 675f 6275 6666 000e 5f5f  ..__msg_buff..__
-00000210: 6465 6c5f 5f00 3114 5f5f 696e 7374 616e  del__.1.__instan
-00000220: 6365 0008 6c6f 6f70 002a 7365 745f 6578  ce..loop.*set_ex
-00000230: 6365 7074 696f 6e5f 6861 6e64 6c65 7200  ception_handler.
-00000240: 0c61 7863 6570 7400 1063 616c 6c62 6163  .axcept..callbac
-00000250: 6b00 1269 646c 655f 7461 736b 0008 6964  k..idle_task..id
-00000260: 6c65 0016 5f71 7565 7565 5f66 7265 6500  le.._queue_free.
-00000270: 814d 1c5f 7175 6575 655f 6c69 6d69 7465  .M._queue_limite
-00000280: 7200 1451 5545 5545 5f53 495a 4500 0a4f  r..QUEUE_SIZE..O
-00000290: 4c4f 4144 000a 736c 6565 7000 146c 6973  LOAD..sleep..lis
-000002a0: 745f 7461 736b 7300 044e 6f00 0659 6573  t_tasks..No..Yes
-000002b0: 000c 7b7d 7b7d 7b7d 0079 145f 7061 7273  ..{}{}{}.y._pars
-000002c0: 655f 7461 6700 0b08 7368 6f77 000c 7b7d  e_tag...show..{}
-000002d0: 3a20 7b7d 0007 086b 696c 6c00 0a7b 7d7c  : {}...kill..{}|
-000002e0: 7b7d 0010 4b69 6c6c 3a20 7b7d 0004 2c20  {}..Kill: {}.., 
-000002f0: 0016 7275 6e5f 666f 7265 7665 7200 810f  ..run_forever...
-00000300: 1e73 6572 7665 725f 7461 736b 5f6d 7367  .server_task_msg
-00000310: 000c 7365 7276 6572 0012 3c67 656e 6578  ..server..<genex
-00000320: 7072 3e00 8231 103c 6c61 6d62 6461 3e00  pr>..1.<lambda>.
-00000330: 1874 6173 6b5f 6d61 6e61 6765 7200 8159  .task_manager..Y
-00000340: 067b 7d0a 0002 2600 8171 8115 8203 8141  .{}...&..q.....A
-00000350: 0a64 656c 6179 0010 5374 6172 7420 7b7d  .delay..Start {}
-00000360: 0014 7b7d 2069 7320 4275 7379 0024 5f5f  ..{} is Busy.$__
-00000370: 636f 6e76 5f66 756e 635f 7061 7261 6d73  conv_func_params
-00000380: 0002 2700 0222 0004 7b7d 0018 5f5f 666f  ..'.."..{}..__fo
-00000390: 726d 6174 5f6f 7574 0008 6865 6c70 0014  rmat_out..help..
-000003a0: 3c6c 6973 7463 6f6d 703e 0012 7465 726d  <listcomp>..term
-000003b0: 696e 6174 6500 0e20 7b7d 3a20 7b7d 0008  inate.. {}: {}..
-000003c0: 207b 7d2c 000e 6173 796e 6369 6f00 2f2d   {},..asyncio./-
-000003d0: 3582 290e 7461 736b 7374 7200 4910 6172  5.).taskstr.I.ar
-000003e0: 675f 6c69 7374 0081 5781 2381 2182 2f82  g_list..W.#.!./.
-000003f0: 1310 6578 635f 7479 7065 0012 6578 635f  ..exc_type..exc_
-00000400: 7661 6c75 6500 1274 7261 6365 6261 636b  value..traceback
-00000410: 0006 6d73 6700 0663 6c73 0082 350e 636f  ..msg..cls..5.co
-00000420: 6e74 6578 7400 8233 813d 8143 823b 106d  ntext..3.=.C.;.m
-00000430: 7367 5f6c 6973 7400 0a70 6172 616d 0012  sg_list..param..
-00000440: 656e 756d 6572 6174 6500 8179 126a 736f  enumerate..y.jso
-00000450: 6e5f 6d6f 6465 000e 6c6d 5f66 756e 6300  n_mode..lm_func.
-00000460: 0c6f 7574 7075 7400 8117 085f 7461 6700  .output...._tag.
-00000470: 051a 7c2d 5b4c 4d2d 5049 5045 5d20 7461  ..|-[LM-PIPE] ta
-00000480: 736b 2065 7272 6f72 3a20 7b7d 0005 175b  sk error: {}...[
-00000490: 4952 512d 5049 5045 5d20 6572 726f 723a  IRQ-PIPE] error:
-000004a0: 207b 7d0a 7b7d 0005 1c5b 4552 525d 2065   {}.{}...[ERR] e
-000004b0: 7865 635f 6c6d 5f70 6970 6520 6572 726f  xec_lm_pipe erro
-000004c0: 723a 207b 7d00 051f 6578 6563 5f6c 6d5f  r: {}...exec_lm_
-000004d0: 7069 7065 5f73 6368 6564 756c 6520 6572  pipe_schedule er
-000004e0: 726f 723a 207b 7d00 051b 5f65 7865 635f  ror: {}..._exec_
-000004f0: 6c6d 5f63 6f72 6520 7265 2d69 6d70 6f72  lm_core re-impor
-00000500: 7420 7b7d 2100 0517 6578 6563 5f6c 6d5f  t {}!...exec_lm_
-00000510: 636f 7265 207b 7d2d 3e7b 7d3a 207b 7d00  core {}->{}: {}.
-00000520: 0518 6d65 6d6f 7279 2061 6c6c 6f63 6174  ..memory allocat
-00000530: 696f 6e20 6661 696c 6564 0005 0e69 7320  ion failed...is 
-00000540: 6e6f 7420 6465 6669 6e65 6400 0534 5348  not defined..4SH
-00000550: 454c 4c3a 2074 7970 6520 6865 6c70 2066  ELL: type help f
-00000560: 6f72 2073 696e 676c 6520 776f 7264 2063  or single word c
-00000570: 6f6d 6d61 6e64 7320 2862 7569 6c74 2d69  ommands (built-i
-00000580: 6e29 0005 4353 4845 4c4c 3a20 666f 7220  n)..CSHELL: for 
-00000590: 4c4d 2065 7865 633a 205b 315d 284c 4d29  LM exec: [1](LM)
-000005a0: 6d6f 6475 6c65 205b 325d 6675 6e63 7469  module [2]functi
-000005b0: 6f6e 205b 332e 2e2e 5d6f 7074 696f 6e61  on [3...]optiona
-000005c0: 6c20 7061 7261 6d73 0005 1d73 6368 6564  l params...sched
-000005d0: 756c 655f 6c6d 5f65 7865 6320 7b7d 2065  ule_lm_exec {} e
-000005e0: 7272 6f72 3a20 7b7d 0005 1163 616e 2774  rror: {}...can't
-000005f0: 2063 616e 6365 6c20 7365 6c66 0005 265b   cancel self..&[
-00000600: 4952 5120 6c69 6d69 7461 7469 6f6e 5d20  IRQ limitation] 
-00000610: 5461 736b 2063 616e 6365 6c20 6572 726f  Task cancel erro
-00000620: 723a 207b 7d00 0519 5b45 5252 5d20 5461  r: {}...[ERR] Ta
-00000630: 736b 206b 696c 6c20 6572 726f 723a 207b  sk kill error: {
-00000640: 7d00 0516 5b61 696f 5d20 6578 6365 7074  }...[aio] except
-00000650: 696f 6e3a 207b 7d3a 7b7d 0005 195b 6169  ion: {}:{}...[ai
-00000660: 6f5d 2054 6173 6b20 7175 6575 6520 6675  o] Task queue fu
-00000670: 6c6c 3a20 7b7d 0005 0d69 2e64 2e6c 2e65  ll: {}...i.d.l.e
-00000680: 3a20 7b7d 6d73 0005 1a5b 4552 525d 2049  : {}ms...[ERR] I
-00000690: 646c 6520 7461 736b 2065 7869 7374 733a  dle task exists:
-000006a0: 207b 7d00 0515 2d2d 2d2d 206d 6963 724f   {}...---- micrO
-000006b0: 5320 2074 6f70 202d 2d2d 2d00 0516 2371  S  top ----...#q
-000006c0: 7565 7565 3a20 7b7d 2023 6c6f 6164 3a20  ueue: {} #load: 
-000006d0: 7b7d 250a 0005 1123 4163 7469 7665 2020  {}%....#Active  
-000006e0: 2023 7461 736b 4944 0005 114e 6f20 7461   #taskID...No ta
-000006f0: 736b 2066 6f75 6e64 3a20 7b7d 0005 0b4b  sk found: {}...K
-00000700: 696c 6c3a 207b 7d7c 7b7d 0005 165b 6169  ill: {}|{}...[ai
-00000710: 6f5d 206c 6f6f 7020 7374 6f70 7065 643a  o] loop stopped:
-00000720: 207b 7d00 0541 496e 7661 6c69 6420 7461   {}..AInvalid ta
-00000730: 736b 2063 6d64 2120 4865 6c70 3a20 7461  sk cmd! Help: ta
-00000740: 736b 206c 6973 7420 2f20 6b69 6c6c 203c  sk list / kill <
-00000750: 7461 736b 4944 3e20 2f20 7368 6f77 203c  taskID> / show <
-00000760: 7461 736b 4944 3e00 0513 5b45 5252 5d20  taskID>...[ERR] 
-00000770: 5461 736b 206b 696c 6c3a 207b 7d00 8a04  Task kill: {}...
-00000780: 1030 0180 0e2c 2c2c 2632 2c72 6040 8993  .0...,,,&2,r`@..
-00000790: 89b7 8414 840d 8840 8451 8010 022a 011b  .......@.Q...*..
-000007a0: 031c 0216 0259 8010 042a 011b 051c 0416  .....Y...*......
-000007b0: 0459 8010 062a 011b 071c 0616 0659 8051  .Y...*.......Y.Q
-000007c0: 1b08 1678 8010 0910 0a2a 021b 0b1c 0916  ...x.....*......
-000007d0: 091c 0a16 0a59 8010 0c2a 011b 0d1c 0c16  .....Y...*......
-000007e0: 0c59 8010 0e10 0f2a 021b 101c 0e16 0e1c  .Y.....*........
-000007f0: 0f16 0f59 5432 0010 1134 0216 1154 3201  ...YT2...4...T2.
-00000800: 1012 3402 1612 3202 1614 3203 161a 512a  ..4...2...2...Q*
-00000810: 0153 3304 161b 3205 161c 3206 1624 5163  .S3...2...2..$Qc
-00000820: 0786 1c10 3011 881d 4484 0988 0d84 0884  ....0...D.......
-00000830: 0984 0889 138a 1b84 1484 0f64 6011 7916  ...........d`.y.
-00000840: 7a10 1116 7b2c 0016 2f32 0016 2511 7c32  z...{,../2..%.|2
-00000850: 0134 0116 2e32 0216 3132 0316 3232 0416  .4...2..12..22..
-00000860: 3351 512a 0253 3305 1634 5151 512a 0353  3QQ*.S3..4QQQ*.S
-00000870: 3306 1638 3207 163b 3208 163a 3209 163e  3..82..;2..:2..>
-00000880: 320a 163f 5163 0b82 6011 1625 8104 8020  2..?Qc..`..%... 
-00000890: 2424 2424 2425 51b0 1826 50b0 1827 94b0  $$$$$%Q..&P..'..
-000008a0: 1828 51b0 1829 52b0 182a 102b b018 2c51  .(Q..)R..*.+..,Q
-000008b0: b018 2d51 6382 2829 122e 2d80 2a60 202b  ..-Qc.()..-.*` +
-000008c0: 4b42 1211 132f 1430 b051 3602 c1b1 51de  KB.../.0.Q6...Q.
-000008d0: d344 47b1 132a 4342 5263 5063 8240 1910  .DG..*CBRcPc.@..
-000008e0: 3181 0480 3660 242e 52b0 182a b013 2d12  1...6`$.R..*..-.
-000008f0: 1113 2f14 2336 00dd 444a 1211 132f b013  ../.#6..DJ.../..
-00000900: 2d53 5b56 5163 8100 1110 3281 0480 3e60  -S[VQc....2...>`
-00000910: 4024 50b0 182a b063 8130 a804 1a33 8104  @$P..*.c.0...3..
-00000920: 8105 8106 8107 8047 6040 52b0 182a 5163  .......G`@R..*Qc
-00000930: 8528 b380 011e 3481 0445 2d80 4f60 603a  .(....4..E-.O``:
-00000940: 4b62 244e 27b2 51de 4451 1035 1419 1281  Kb$N'.Q.DQ.5....
-00000950: 0012 1113 2f34 0136 0142 41b2 b018 2d12  ..../4.6.BA...-.
-00000960: 1114 2eb0 132d 3601 4442 5063 50b0 182a  .....-6.DBPcP..*
-00000970: 1278 1436 3600 1437 b136 01b0 1829 b012  .x.66..7.6...)..
-00000980: 1113 2fb2 5652 6387 70c0 8501 2638 8104  ../.VRc.p...&8..
-00000990: 4542 4d80 6280 082f 4b62 244e 5844 5229  EBM.b../Kb$NXDR)
-000009a0: 1039 1420 b180 822e 0255 3601 b018 2d12  .9. .....U6...-.
-000009b0: 1114 2eb0 132d 3601 4442 5063 b1b0 1826  .....-6.DBPc...&
-000009c0: b251 de44 45b0 1327 4241 b2b0 1827 b351  .Q.DE..'BA...'.Q
-000009d0: de44 45b0 1328 424b b393 d844 43b3 4243  .DE..(BK...DC.BC
-000009e0: b013 28b0 1828 50b0 182a 1278 1436 3600  ..(..(P..*.x.66.
-000009f0: 1437 b014 3a36 0036 01b0 1829 b012 1113  .7..:6.6...)....
-00000a00: 2fb0 132d 5652 6388 30c5 0222 3b81 0480  /..-VRc.0..";...
-00000a10: 7d60 2229 2422 532b 3548 4d2c 2b48 4eb0  }`")$"S+5HM,+HN.
-00000a20: 1329 51de d344 c180 50b0 1827 480a b013  .)Q..D..P..'H...
-00000a30: 2914 3b36 0059 4a29 5712 7edf 4462 c149  ).;6.YJ)W.~.Db.I
-00000a40: 1823 0b12 8103 b134 01dc 444c 120a 230c  .#.....4..DL..#.
-00000a50: 1419 b136 0134 0159 5151 c128 015d 4a01  ...6.4.YQQ.(.]J.
-00000a60: 5db0 1431 3600 5942 4250 634a 2057 127e  ]..16.YBBPcJ W.~
-00000a70: df44 59c1 490f 120a 230d 1419 b136 0134  .DY.I...#....6.4
-00000a80: 0159 5063 5151 c128 015d 4a01 5d52 6383  .YPcQQ.(.]J.]Rc.
-00000a90: 48a1 4018 3a81 0480 9180 0720 2d2e 2524  H.@.:...... -.%$
-00000aa0: 1278 143c b013 2836 015e 5168 5912 1cb0  .x.<..(6.^QhY...
-00000ab0: 1326 103d b013 3e34 8201 59b0 1327 4342  .&.=..>4..Y..'CB
-00000ac0: 4242 421c 52b0 182a 5163 8100 1a10 3e81  BBB.R..*Qc....>.
-00000ad0: 0481 0880 a060 b1b0 182c 5163 8118 110c  .....`...,Qc....
-00000ae0: 3f81 0480 a624 52b0 182a b053 5a18 2951  ?....$R..*.SZ.)Q
-00000af0: 6389 4418 3912 88b0 2328 4386 118d 0768  c.D.9...#(C....h
-00000b00: 4088 0c88 1a8a 0b88 0f88 0f88 1088 2084  @............. .
-00000b10: 0a00 1179 167a 1012 167b 5116 4111 0c10  ...y.z...{Q.A...
-00000b20: 1334 0116 4b80 164c b020 0001 1640 117c  .4..K..L. ...@.|
-00000b30: 5151 2a02 5333 0134 0116 4411 7c32 0234  QQ*.S3.4..D.|2.4
-00000b40: 0116 4811 7c32 0334 0116 4a11 7c32 0434  ..H.|2.4..J.|2.4
-00000b50: 0116 4651 5051 2a03 5333 0516 3711 7c32  ..FQPQ*.S3..7.|2
-00000b60: 0634 0116 4e11 7c32 0734 0116 5311 7c32  .4..N.|2.4..S.|2
-00000b70: 0834 0116 5511 7c32 0934 0116 5832 0a16  .4..U.|2.4..X2..
-00000b80: 5c11 7c32 0b34 0116 5eb0 630c 8560 3a1a  \.|2.4..^.c..`:.
-00000b90: 4054 8109 80b5 6040 494f 2c2e 7612 1213  @T....`@IO,.v...
-00000ba0: 4151 de44 bf80 1281 0a25 00b1 1540 b136  AQ.D.....%...@.6
-00000bb0: 0112 1218 4112 7814 3636 0012 1213 4118  ....A.x.66....A.
-00000bc0: 4212 1213 4113 4214 43b1 1344 3601 5912  B...A.B.C..D6.Y.
-00000bd0: 1213 4114 3710 4512 1214 4636 0010 2d10  ..A.7.E...F6..-.
-00000be0: 4736 8400 5912 1213 4163 8150 b280 010e  G6..Y...Ac.P....
-00000bf0: 4442 810b 80c7 6012 0a23 0e14 19b0 b136  DB....`..#.....6
-00000c00: 0234 0159 5163 813c 1806 4880 cf12 810c  .4.YQc.<..H.....
-00000c10: 3200 1211 132f 1449 3600 3401 3401 6301  2..../.I6.4.4.c.
-00000c20: 8208 4908 7454 80cf 2b00 b05f 4b14 3002  ..I.tT..+.._K.0.
-00000c30: c1c2 b213 2a43 3510 39b1 dd44 2f81 2f14  ....*C5.9..D/./.
-00000c40: 422a 6383 0018 104a 80d3 6040 2d2b 2612  B*c....J..`@-+&.
-00000c50: 1214 4836 0012 1213 4bdb 4457 230f 1419  ..H6....K.DW#...
-00000c60: 1212 134b 3601 c012 0ab0 3401 5912 7eb0  ...K6.....4.Y.~.
-00000c70: 3401 6551 638b 00e8 4226 4680 df60 4024  4.eQc...B&F..`@$
-00000c80: 222b 2a22 2046 2b2b 254b 375f 3522 8116  "+*" F++%K7_5"..
-00000c90: c086 c112 1113 2f14 3010 4736 01c2 2310  ....../.0.G6..#.
-00000ca0: 1419 b036 01b2 182c 4859 b180 4251 57c3  ...6...,HY..BQW.
-00000cb0: 1278 143c b036 015e 5168 5942 4081 e558  .x.<.6.^QhYB@..X
-00000cc0: 5ad7 432a 5959 120e 3400 c412 7814 3cb0  Z.C*YY..4...x.<.
-00000cd0: 3601 5e51 6859 1281 0d12 0f12 0e34 00b4  6.^QhY.......4..
-00000ce0: 3402 b0f7 81f3 2280 64f4 3401 c512 810d  4.....".d.4.....
-00000cf0: 1212 134c b5f2 82f7 3401 1212 184c 42a9  ...L....4....LB.
-00000d00: 7f4a 1e57 127e df44 57c6 490d 120a 2311  .J.W.~.DW.I...#.
-00000d10: 1419 b636 0134 0159 5151 c628 065d 4a01  ...6.4.YQQ.(.]J.
-00000d20: 5d52 b218 2a51 6384 30e1 8501 1c37 8109  ]R..*Qc.0....7..
-00000d30: 452d 426b 80f8 6040 2a27 3312 810e b112  E-Bk..`@*'3.....
-00000d40: 6434 0244 5a12 1214 4a36 0059 1211 3400  d4.DZ...J6.Y..4.
-00000d50: 1438 1045 b110 42b3 104d b436 8600 6312  .8.E..B..M.6..c.
-00000d60: 1134 0014 3410 45b1 102d b236 8400 6386  .4..4.E..-.6..c.
-00000d70: 6878 184e 9004 6020 2c32 2f2c 2c2a 2912  hx.N..` ,2/,,*).
-00000d80: 1213 4b12 1214 4836 00f3 c023 1223 1314  ..K...H6...#.#..
-00000d90: 19b0 1212 134c 3602 2314 2b03 c112 1113  .....L6.#.+.....
-00000da0: 2f14 4936 005f 4b2f 3002 c2c3 b313 2a44  /.I6._K/0.....*D
-00000db0: 4410 4f42 4210 50c4 101f 8a12 8100 b434  D.OBB.P........4
-00000dc0: 01f3 f4c5 1051 1419 b4b5 b236 03c6 b114  .....Q.....6....
-00000dd0: 52b6 3601 5942 0f12 810f b134 0163 8708  R.6.YB.....4.c..
-00000de0: 611e 532d 9013 202b 2623 282c 3c29 2a23  a.S-.. +&#(,<)*#
-00000df0: 2212 1113 2f14 30b0 5136 02c1 b151 de44  ".../.0.Q6...Q.D
-00000e00: cb80 2b00 c2b0 1417 1039 3601 c312 1113  ..+......96.....
-00000e10: 2f14 2336 005f 4b26 c4b4 1415 b380 5536  /.#6._K&......U6
-00000e20: 0144 5912 8100 b334 0181 d844 4fb3 8155  .DY....4...DO..U
-00000e30: 1054 d944 47b2 1452 b436 0159 4218 1281  .T.DG..R.6.YB...
-00000e40: 00b2 3401 80d9 4443 2b00 63b2 63b0 2b01  ..4...DC+.c.c.+.
-00000e50: 6386 3071 1c55 2d90 2260 2028 2a28 2a2b  c.0q.U-."` (*(*+
-00000e60: 2325 3712 1214 53b0 3601 c112 8100 b134  #%7...S.6......4
-00000e70: 0180 d944 4823 1514 19b0 3601 6312 8100  ...DH#....6.c...
-00000e80: b134 0181 d944 4b12 1113 2fb1 8055 5513  .4...DK.../..UU.
-00000e90: 2c63 2b00 c2b1 5f4b 18c3 b214 5210 5614  ,c+..._K....R.V.
-00000ea0: 19b3 1211 132f b355 132c 3602 3601 5942  ...../.U.,6.6.YB
-00000eb0: 2610 5714 20b2 3601 6388 5481 1028 582d  &.W. .6.c.T..(X-
-00000ec0: 9032 8007 8309 2822 2a2b 2a2b 2a23 2527  .2....("*+*+*#%'
-00000ed0: 302e 3200 c112 1214 53b0 3601 c252 c312  0.2.....S.6..R..
-00000ee0: 8100 b234 0180 d944 4bb3 2315 1419 b036  ...4...DK.#....6
-00000ef0: 012a 0263 1281 00b2 3401 81d9 4455 2316  .*.c....4...DU#.
-00000f00: 1419 b280 55b3 3602 c4b1 b280 5534 01b4  ....U.6.....U4..
-00000f10: 2a02 632b 00c5 b25f 4b18 c6b3 b1b6 3401  *.c+..._K.....4.
-00000f20: e2c3 b514 5210 5914 19b6 b336 0236 0159  ....R.Y....6.6.Y
-00000f30: 4226 105a 1419 105b 1420 b536 0136 01c4  B&.Z...[. .6.6..
-00000f40: b3b4 2a02 6301 8450 c902 1275 8118 903a  ..*.c..P...u...:
-00000f50: 2b22 582c 1211 132f 1430 b051 3602 c148  +"X,.../.0.Q6..H
-00000f60: 0fb1 51de 4442 5063 b114 3b36 0063 4a20  ..Q.DBPc..;6.cJ 
-00000f70: 5712 7edf 4459 c249 0f12 0a23 1914 19b2  W.~.DY.I...#....
-00000f80: 3601 3401 5950 6351 51c2 2802 5d4a 015d  6.4.YPcQQ.(.]J.]
-00000f90: 5163 8400 c102 125c 8109 9051 6022 532c  Qc.....\...Q`"S,
-00000fa0: 480a b013 4214 5c36 0059 4a26 5712 7edf  H...B.\6.YJ&W.~.
-00000fb0: 445f c149 1512 0a23 1714 19b1 3601 3401  D_.I...#....6.4.
-00000fc0: 59b0 1342 145d 3600 5951 51c1 2801 5d4a  Y..B.]6.YQQ.(.]J
-00000fd0: 015d 5163 8218 2910 5e81 0890 5c2c 2522  .]Qc..).^...\,%"
-00000fe0: 1211 132f 1430 105f 5136 02c1 b151 de44  .../.0._Q6...Q.D
-00000ff0: 4251 63b0 b118 2c51 6387 2cd1 021e 147d  BQc...,Qc.,....}
-00001000: 9067 6020 4229 4230 2759 2d2c 2b48 32b0  .g` B)B0'Y-,+H2.
-00001010: 1415 1016 3601 4442 5263 3200 b014 1710  ....6.DBRc2.....
-00001020: 1836 015e 3401 5f4b 16c1 121b b134 0143  .6.^4._K.....4.C
-00001030: 4c12 0923 0014 19b1 3601 3401 5942 284a  L..#....6.4.YB(J
-00001040: 2d57 127e df44 66c2 491c 1209 2301 1419  -W.~.Df.I...#...
-00001050: b0b2 3602 3401 5912 0a23 0214 19b2 3601  ..6.4.Y..#....6.
-00001060: 3401 5950 6351 51c2 2802 5d4a 015d 5263  4.YPcQQ.(.]J.]Rc
-00001070: 0182 38b9 4008 6054 9070 53b0 5353 4b18  ..8.@.`T.pS.SSK.
-00001080: c112 8100 b134 0180 d844 33b1 1461 3600  .....4...D3..a6.
-00001090: 1417 3600 6759 4226 5163 8368 c102 141a  ..6.gYB&Qc.h....
-000010a0: 7d90 7b60 2022 284d 2c48 0c12 0612 14b0  }.{` "(M,H......
-000010b0: 3402 5952 634a 2057 127e df44 59c1 490f  4.YRcJ W.~.DY.I.
-000010c0: 120a 2303 1419 b136 0134 0159 5063 5151  ..#....6.4.YPcQQ
-000010d0: c128 015d 4a01 5d51 6383 34aa 019c 011b  .(.]J.]Qc.4.....
-000010e0: 7f3d 9088 8007 2644 862c 6027 4200 0125  .=....&D.,`'B..%
-000010f0: 0151 de44 4432 0027 01b0 b120 0102 c2b2  .Q.DD2.'... ....
-00001100: 2500 3401 4442 5263 121c 2500 2501 3402  %.4.DBRc..%.%.4.
-00001110: 6302 4809 0a62 8108 9090 5163 9548 9312  c.H..b....Qc.H..
-00001120: 4c63 5454 8110 9093 4749 2d2f 2826 4226  LcTT....GI-/(&B&
-00001130: 2832 2622 2833 2227 4250 2830 2e51 225d  (2&"(3"'BP(0.Q"]
-00001140: 462b 2e23 4e4c 4212 8100 b234 01c3 1029  F+.#NLB....4...)
-00001150: b280 55d9 44fa 80b3 82d9 4467 1064 b281  ..U.D.....Dg.d..
-00001160: 55d9 445f 1057 1420 1212 3400 144e 3600  U.D_.W. ..4..N6.
-00001170: 3601 c410 6514 19b4 3601 c425 01b4 3401  6...e...6..%..4.
-00001180: 5952 63b3 82d8 44bf 8010 58b2 8155 d944  YRc...D...X..U.D
-00001190: 5a12 1234 0014 5810 2db2 8255 3682 0030  Z..4..X.-..U6..0
-000011a0: 02c5 c625 01b6 3401 5952 6310 55b2 8155  ...%..4.YRc.U..U
-000011b0: d944 5525 0112 1234 0014 5510 2db2 8255  .DU%...4..U.-..U
-000011c0: 3682 0034 0159 5263 2501 2318 3401 5952  6..4.YRc%.#.4.YR
-000011d0: 63b3 82d8 449e 8110 6625 007f 55dd 4494  c...D...f%..U.D.
-000011e0: 8125 0014 677f 3601 c7b7 1468 1066 3601  .%..g.6....h.f6.
-000011f0: 82d9 4443 5242 4150 c8b7 1469 1066 102b  ..DCRBAP...i.f.+
-00001200: 3602 1461 3600 c9b9 146a 3600 4448 1281  6..a6....j6.DH..
-00001210: 0db9 3401 4241 51c9 4814 1212 3400 1437  ..4.BAQ.H...4..7
-00001220: 2500 1042 b810 6bb9 3684 01c5 4a1a 5712  %..B..k.6...J.W.
-00001230: 7edf 4453 ca49 0925 01ba 3401 5952 6351  ~.DS.I.%..4.YRcQ
-00001240: 51ca 280a 5d4a 015d 1039 1420 2500 8082  Q.(.]J.].9. %...
-00001250: 2e02 5536 01cb b544 4e25 0110 6c14 19bb  ..U6...DN%..l...
-00001260: 3601 3401 5942 4c25 0110 6d14 19bb 3601  6.4.YBL%..m...6.
-00001270: 3401 5952 6350 6395 349e 1249 1c7f 3d90  4.YRcPc.4..I..=.
-00001280: c880 0883 0d85 0f27 4d2b 1f21 6327 2d42  .......'M+.!c'-B
-00001290: 7c2a 4c4d 526f 492b 6e2d 562a 462b 2646  |*LMRoI+n-V*F+&F
-000012a0: 0a32 00c2 ba20 0101 c3b0 7f55 101d d9c4  .2... .....U....
-000012b0: b444 48b0 807f 2e02 5542 41b0 c512 8100  .DH.....UBA.....
-000012c0: b534 0182 db44 f981 101e 1419 b580 5536  .4...D........U6
-000012d0: 01b5 8155 b210 1f14 20b5 8251 2e02 5536  ...U.... ..Q..U6
-000012e0: 0134 015b 5ac6 c7c8 488e 01b6 1202 ddd3  .4.[Z...H.......
-000012f0: 444d 1281 0110 2114 19b6 3601 3401 5948  DM....!...6.4.YH
-00001300: 1212 8102 1022 1419 b6b7 b836 0334 0127  .....".....6.4.'
-00001310: 0a4a 4e57 127e df44 c680 c949 3cb6 1281  .JNW.~.D...I<...
-00001320: 03b9 3401 dd44 6b12 0a23 0414 19b6 3601  ..4..Dk..#....6.
-00001330: 3401 5912 8101 1021 1419 b636 0134 0159  4.Y....!...6.4.Y
-00001340: 1281 0210 2214 19b6 b7b8 3603 3401 270a  ....".....6.4.'.
-00001350: 4246 127e b934 0165 5151 c928 095d 4a01  BF.~.4.eQQ.(.]J.
-00001360: 5db3 b4b7 250a 3403 270a b112 8103 250a  ]...%.4.'.....%.
-00001370: 3401 3401 5952 634a 4857 127e df44 c080  4.4.YRcJHW.~.D..
-00001380: c949 36b1 2305 1419 b6b7 b936 0334 0159  .I6.#......6.4.Y
-00001390: 2306 1281 03b9 3401 dd43 4b23 0712 8103  #.....4..CK#....
-000013a0: b934 01dd 4452 b612 0214 2336 00dd 4446  .4..DR....#6..DF
-000013b0: 1202 b653 5b56 5063 5151 c928 095d 4a01  ...S[VPcQQ.(.]J.
-000013c0: 5db1 2308 3401 59b1 2309 3401 5952 6302  ].#.4.Y.#.4.YRc.
-000013d0: 875c 599c 016e 8111 90d1 222e 2d36 252d  .\Y..n....".-6%-
-000013e0: 2c2a 2a00 0351 c110 6f25 00dd 4347 1070  ,**..Q..o%..CG.p
-000013f0: 2500 dd44 7532 0012 8112 2500 3401 3401  %..Du2....%.4.4.
-00001400: 2703 b0b3 2001 0212 8113 8012 8100 2503  '... .........%.
-00001410: 3401 8234 0334 01c1 b15f 4b0e c225 0014  4..4.4..._K..%..
-00001420: 69b2 1071 3602 2700 4230 2500 1469 101f  i..q6.'.B0%..i..
-00001430: 105b 3602 2700 1281 0eb1 1264 3402 444a  .[6.'......d4.DJ
-00001440: 2500 1419 b181 3701 2700 2500 6302 8210  %.....7.'.%.c...
-00001450: 4908 7454 90d3 2b00 b05f 4b15 3002 c1c2  I.tT..+.._K.0...
-00001460: b210 70d9 4346 b210 6fd9 442e b12f 1442  ..p.CF..o.D../.B
-00001470: 2963 8228 6b0c 7454 5454 90d4 2b00 b25f  )c.(k.tTTT..+.._
-00001480: 4b16 c325 0025 01b3 5525 01b3 81f2 5581  K..%.%..U%....U.
-00001490: f22e 0255 2f14 4228 6385 3cc0 0424 7254  ...U/.B(c.<..$rT
-000014a0: 8114 8115 8116 90de 2b23 4651 2623 462c  ........+#FQ&#F,
-000014b0: 1281 0eb3 1281 1734 0244 5ab1 4446 1204  .......4.DZ.DF..
-000014c0: b334 0163 1057 1420 3200 2500 1449 3600  .4.c.W. 2.%..I6.
-000014d0: 3401 3601 63b2 1073 d944 55b1 4446 1204  4.6.c..s.DU.DF..
-000014e0: b334 0163 1057 1420 3201 b334 0136 0163  .4.c.W. 2..4.6.c
-000014f0: b363 0281 6859 0874 5490 e22b 00b0 5f4b  .c..hY.tT..+.._K
-00001500: 1030 02c1 c210 7614 19b1 b236 022f 1442  .0....v....6./.B
-00001510: 2e63 8148 4908 7454 90e8 2b00 b05f 4b0c  .c.HI.tT..+.._K.
-00001520: c110 7714 19b1 3601 2f14 4232 6383 70c9  ..w...6./.B2c.p.
-00001530: 0214 247f a019 6040 2228 4d2d 480c 1206  ..$...`@"(M-H...
-00001540: 121b b034 0259 5263 4a21 5712 7edf 445a  ...4.YRcJ!W.~.DZ
-00001550: c149 1012 0a23 0a14 19b0 b136 0234 0159  .I...#.....6.4.Y
-00001560: 5063 5151 c128 015d 4a01 5d51 63         PcQQ.(.]J.]Qc
+00000090: 6b73 5f64 6966 6600 0a75 7469 6d65 000e  ks_diff..utime..
+000000a0: 636f 6c6c 6563 7400 0467 6300 0a73 696d  collect..gc..sim
+000000b0: 6763 0008 5461 736b 000e 4d61 6e61 6765  gc..Task..Manage
+000000c0: 7200 1061 696f 7175 6575 6500 1865 7865  r..aioqueue..exe
+000000d0: 635f 6c6d 5f70 6970 6500 8227 066e 2f61  c_lm_pipe..'.n/a
+000000e0: 0082 2302 3b00 8129 2a65 7865 635f 6c6d  ..#.;..)*exec_lm
+000000f0: 5f70 6970 655f 7363 6865 6475 6c65 0018  _pipe_schedule..
+00000100: 6578 6563 5f6c 6d5f 636f 7265 001a 5f65  exec_lm_core.._e
+00000110: 7865 635f 6c6d 5f63 6f72 6500 0a3e 6a73  xec_lm_core..>js
+00000120: 6f6e 000a 4c4d 5f7b 7d00 0981 5112 696d  on..LM_{}...Q.im
+00000130: 706f 7274 207b 7d00 127b 7d2e 7b7d 287b  port {}..{}.{}({
+00000140: 7d29 0081 552a 6578 6563 5f6c 6d5f 636f  })..U*exec_lm_co
+00000150: 7265 5f73 6368 6564 756c 6500 2314 5f5f  re_schedule.#.__
+00000160: 6361 6c6c 6261 636b 0010 5f5f 696e 6c6f  callback..__inlo
+00000170: 6f70 000e 5f5f 736c 6565 7000 0874 6173  op..__sleep..tas
+00000180: 6b00 0a45 7665 6e74 0008 646f 6e65 0003  k..Event..done..
+00000190: 066f 7574 0006 7461 6700 0e69 735f 6275  .out..tag..is_bu
+000001a0: 7379 000a 5441 534b 5300 812d 0c69 735f  sy..TASKS..-.is_
+000001b0: 7365 7400 145f 5f74 6173 6b5f 6465 6c00  set..__task_del.
+000001c0: 8219 1981 0d1b 0c63 7265 6174 6500 0a61  .......create..a
+000001d0: 696f 7b7d 001c 6765 745f 6576 656e 745f  io{}..get_event_
+000001e0: 6c6f 6f70 0016 6372 6561 7465 5f74 6173  loop..create_tas
+000001f0: 6b00 1263 7265 6174 655f 6c6d 0002 2e00  k..create_lm....
+00000200: 1874 6173 6b5f 7772 6170 7065 7200 0c63  .task_wrapper..c
+00000210: 616e 6365 6c00 1073 6c65 6570 5f6d 7300  ancel..sleep_ms.
+00000220: 0c6d 7367 6f62 6a00 0e5f 5f64 656c 5f5f  .msgobj..__del__
+00000230: 0014 6b65 6570 5f63 6163 6865 0031 145f  ..keep_cache.1._
+00000240: 5f69 6e73 7461 6e63 6500 2a73 6574 5f65  _instance.*set_e
+00000250: 7863 6570 7469 6f6e 5f68 616e 646c 6572  xception_handler
+00000260: 000c 6178 6365 7074 0010 6361 6c6c 6261  ..axcept..callba
+00000270: 636b 0012 6964 6c65 5f74 6173 6b00 0869  ck..idle_task..i
+00000280: 646c 6500 145f 7175 6575 655f 6c65 6e00  dle.._queue_len.
+00000290: 814d 1c5f 7175 6575 655f 6c69 6d69 7465  .M._queue_limite
+000002a0: 7200 1451 5545 5545 5f53 495a 4500 0a4f  r..QUEUE_SIZE..O
+000002b0: 4c4f 4144 0008 6c6f 6f70 000a 736c 6565  LOAD..loop..slee
+000002c0: 7000 146c 6973 745f 7461 736b 7300 044e  p..list_tasks..N
+000002d0: 6f00 0659 6573 000c 7b7d 7b7d 7b7d 0079  o..Yes..{}{}{}.y
+000002e0: 145f 7061 7273 655f 7461 6700 0b08 7368  ._parse_tag...sh
+000002f0: 6f77 000c 7b7d 3a20 7b7d 0007 086b 696c  ow..{}: {}...kil
+00000300: 6c00 0a7b 7d7c 7b7d 0010 4b69 6c6c 3a20  l..{}|{}..Kill: 
+00000310: 7b7d 0004 2c20 0016 7275 6e5f 666f 7265  {}.., ..run_fore
+00000320: 7665 7200 810f 1e73 6572 7665 725f 7461  ver....server_ta
+00000330: 736b 5f6d 7367 000c 7365 7276 6572 0012  sk_msg..server..
+00000340: 3c67 656e 6578 7072 3e00 8231 103c 6c61  <genexpr>..1.<la
+00000350: 6d62 6461 3e00 1874 6173 6b5f 6d61 6e61  mbda>..task_mana
+00000360: 6765 7200 8159 067b 7d0a 0002 2600 8171  ger..Y.{}...&..q
+00000370: 8115 8203 8141 0a64 656c 6179 0010 5374  .....A.delay..St
+00000380: 6172 7420 7b7d 0014 7b7d 2069 7320 4275  art {}..{} is Bu
+00000390: 7379 0024 5f5f 636f 6e76 5f66 756e 635f  sy.$__conv_func_
+000003a0: 7061 7261 6d73 0002 2700 0222 0004 7b7d  params..'.."..{}
+000003b0: 0018 5f5f 666f 726d 6174 5f6f 7574 0008  ..__format_out..
+000003c0: 6865 6c70 0014 3c6c 6973 7463 6f6d 703e  help..<listcomp>
+000003d0: 0012 7465 726d 696e 6174 6500 0e20 7b7d  ..terminate.. {}
+000003e0: 3a20 7b7d 0008 207b 7d2c 000e 6173 796e  : {}.. {},..asyn
+000003f0: 6369 6f00 2f2d 3582 290e 7461 736b 7374  cio./-5.).taskst
+00000400: 7200 4910 6172 675f 6c69 7374 0081 5781  r.I.arg_list..W.
+00000410: 2381 2182 2f82 1381 7710 6578 635f 7479  #.!./...w.exc_ty
+00000420: 7065 0012 6578 635f 7661 6c75 6500 1274  pe..exc_value..t
+00000430: 7261 6365 6261 636b 0006 636c 7300 8235  raceback..cls..5
+00000440: 0e63 6f6e 7465 7874 0082 3381 3d81 4382  .context..3.=.C.
+00000450: 3b06 6d73 6700 106d 7367 5f6c 6973 7400  ;.msg..msg_list.
+00000460: 0a70 6172 616d 0012 656e 756d 6572 6174  .param..enumerat
+00000470: 6500 8179 126a 736f 6e5f 6d6f 6465 000e  e..y.json_mode..
+00000480: 6c6d 5f66 756e 6300 0c6f 7574 7075 7400  lm_func..output.
+00000490: 8117 821b 085f 7461 6700 051a 5b53 494d  ....._tag...[SIM
+000004a0: 554c 4154 4f52 204d 4f44 4520 4743 2049  ULATOR MODE GC I
+000004b0: 4d50 4f52 545d 0005 1a7c 2d5b 4c4d 2d50  MPORT]...|-[LM-P
+000004c0: 4950 455d 2074 6173 6b20 6572 726f 723a  IPE] task error:
+000004d0: 207b 7d00 0517 5b49 5251 2d50 4950 455d   {}...[IRQ-PIPE]
+000004e0: 2065 7272 6f72 3a20 7b7d 0a7b 7d00 051c   error: {}.{}...
+000004f0: 5b45 5252 5d20 6578 6563 5f6c 6d5f 7069  [ERR] exec_lm_pi
+00000500: 7065 2065 7272 6f72 3a20 7b7d 0005 1f65  pe error: {}...e
+00000510: 7865 635f 6c6d 5f70 6970 655f 7363 6865  xec_lm_pipe_sche
+00000520: 6475 6c65 2065 7272 6f72 3a20 7b7d 0005  dule error: {}..
+00000530: 1b5f 6578 6563 5f6c 6d5f 636f 7265 2072  ._exec_lm_core r
+00000540: 652d 696d 706f 7274 207b 7d21 0005 1765  e-import {}!...e
+00000550: 7865 635f 6c6d 5f63 6f72 6520 7b7d 2d3e  xec_lm_core {}->
+00000560: 7b7d 3a20 7b7d 0005 186d 656d 6f72 7920  {}: {}...memory 
+00000570: 616c 6c6f 6361 7469 6f6e 2066 6169 6c65  allocation faile
+00000580: 6400 050e 6973 206e 6f74 2064 6566 696e  d...is not defin
+00000590: 6564 0005 3453 4845 4c4c 3a20 7479 7065  ed..4SHELL: type
+000005a0: 2068 656c 7020 666f 7220 7369 6e67 6c65   help for single
+000005b0: 2077 6f72 6420 636f 6d6d 616e 6473 2028   word commands (
+000005c0: 6275 696c 742d 696e 2900 0543 5348 454c  built-in)..CSHEL
+000005d0: 4c3a 2066 6f72 204c 4d20 6578 6563 3a20  L: for LM exec: 
+000005e0: 5b31 5d28 4c4d 296d 6f64 756c 6520 5b32  [1](LM)module [2
+000005f0: 5d66 756e 6374 696f 6e20 5b33 2e2e 2e5d  ]function [3...]
+00000600: 6f70 7469 6f6e 616c 2070 6172 616d 7300  optional params.
+00000610: 051d 7363 6865 6475 6c65 5f6c 6d5f 6578  ..schedule_lm_ex
+00000620: 6563 207b 7d20 6572 726f 723a 207b 7d00  ec {} error: {}.
+00000630: 0526 2b2b 2b2b 2b2b 205f 5f74 6173 6b5f  .&++++++ __task_
+00000640: 6465 6c20 6b65 6570 5f63 6163 6865 3d7b  del keep_cache={
+00000650: 7d20 2b2b 2b2b 2b2b 0005 1163 616e 2774  } ++++++...can't
+00000660: 2063 616e 6365 6c20 7365 6c66 0005 265b   cancel self..&[
+00000670: 4952 5120 6c69 6d69 7461 7469 6f6e 5d20  IRQ limitation] 
+00000680: 5461 736b 2063 616e 6365 6c20 6572 726f  Task cancel erro
+00000690: 723a 207b 7d00 0519 5b45 5252 5d20 5461  r: {}...[ERR] Ta
+000006a0: 736b 206b 696c 6c20 6572 726f 723a 207b  sk kill error: {
+000006b0: 7d00 0516 5b45 5252 5d20 5461 736b 2e5f  }...[ERR] Task._
+000006c0: 5f64 656c 5f5f 3a20 7b7d 0005 165b 6169  _del__: {}...[ai
+000006d0: 6f5d 2065 7863 6570 7469 6f6e 3a20 7b7d  o] exception: {}
+000006e0: 3a7b 7d00 0519 5b61 696f 5d20 5461 736b  :{}...[aio] Task
+000006f0: 2071 7565 7565 2066 756c 6c3a 207b 7d00   queue full: {}.
+00000700: 050e 692e 642e 6c2e 653a 2032 3030 6d73  ..i.d.l.e: 200ms
+00000710: 0005 1a5b 4552 525d 2049 646c 6520 7461  ...[ERR] Idle ta
+00000720: 736b 2065 7869 7374 733a 207b 7d00 0515  sk exists: {}...
+00000730: 2d2d 2d2d 206d 6963 724f 5320 2074 6f70  ---- micrOS  top
+00000740: 202d 2d2d 2d00 0516 2371 7565 7565 3a20   ----...#queue: 
+00000750: 7b7d 2023 6c6f 6164 3a20 7b7d 250a 0005  {} #load: {}%...
+00000760: 1123 4163 7469 7665 2020 2023 7461 736b  .#Active   #task
+00000770: 4944 0005 114e 6f20 7461 736b 2066 6f75  ID...No task fou
+00000780: 6e64 3a20 7b7d 0005 0b4b 696c 6c3a 207b  nd: {}...Kill: {
+00000790: 7d7c 7b7d 0005 165b 6169 6f5d 206c 6f6f  }|{}...[aio] loo
+000007a0: 7020 7374 6f70 7065 643a 207b 7d00 0541  p stopped: {}..A
+000007b0: 496e 7661 6c69 6420 7461 736b 2063 6d64  Invalid task cmd
+000007c0: 2120 4865 6c70 3a20 7461 736b 206c 6973  ! Help: task lis
+000007d0: 7420 2f20 6b69 6c6c 203c 7461 736b 4944  t / kill <taskID
+000007e0: 3e20 2f20 7368 6f77 203c 7461 736b 4944  > / show <taskID
+000007f0: 3e00 0513 5b45 5252 5d20 5461 736b 206b  >...[ERR] Task k
+00000800: 696c 6c3a 207b 7d00 8c54 2436 0180 0e2c  ill: {}..T$6...,
+00000810: 2c2c 2632 2c52 224f 278f 0789 9189 b884  ,,&2,R"O'.......
+00000820: 1484 0d88 4084 5180 1002 2a01 1b03 1c02  ....@.Q...*.....
+00000830: 1602 5980 1004 2a01 1b05 1c04 1604 5980  ..Y...*.......Y.
+00000840: 1006 2a01 1b07 1c06 1606 5980 511b 0816  ..*.......Y.Q...
+00000850: 7f80 1009 100a 2a02 1b0b 1c09 1609 1c0a  ......*.........
+00000860: 160a 5980 100c 2a01 1b0d 1c0c 160c 5980  ..Y...*.......Y.
+00000870: 100e 100f 2a02 1b10 1c0e 160e 1c0f 160f  ....*...........
+00000880: 5948 0e80 1011 2a01 1b12 1c11 1611 594a  YH....*.......YJ
+00000890: 1759 1109 2300 3401 5980 1011 2a01 1b13  .Y..#.4.Y...*...
+000008a0: 1c11 1611 594a 015d 5432 0010 1434 0216  ....YJ.]T2...4..
+000008b0: 1454 3201 1015 3402 1615 3202 1617 3203  .T2...4...2...2.
+000008c0: 161d 512a 0153 3304 161e 3205 161f 3206  ..Q*.S3...2...2.
+000008d0: 1627 5163 0786 2c10 2c14 8b22 4484 0989  .'Qc..,.,.."D...
+000008e0: 0d88 0c84 0984 0989 128a 1984 1484 0f11  ................
+000008f0: 8100 1681 0110 1416 8102 2c00 1633 3200  ..........,..32.
+00000900: 1628 1181 0332 0134 0116 3250 2a01 5333  .(...2.4..2P*.S3
+00000910: 0216 3632 0316 3832 0416 3a51 512a 0253  ..62..82..:QQ*.S
+00000920: 3305 163b 5151 512a 0353 3306 163f 3207  3..;QQQ*.S3..?2.
+00000930: 1642 3208 1641 3209 1645 5163 0a83 0811  .B2..A2..EQc....
+00000940: 1628 810b 8025 2424 2424 2925 51b0 1829  .(...%$$$$)%Q..)
+00000950: 50b0 182a 94b0 182b 51b0 182c 127f 142d  P..*...+Q..,...-
+00000960: 3600 b018 2e10 2fb0 1830 51b0 1831 5163  6...../..0Q..1Qc
+00000970: 8248 2912 3231 802f 6020 2b4f 4212 1413  .H).21./` +OB...
+00000980: 3314 34b0 5136 02c1 b151 ded3 444b b113  3.4.Q6...Q..DK..
+00000990: 2e14 3536 0043 4252 6350 6384 60aa 011a  ..56.CBRcPc.`...
+000009a0: 3681 0b46 803b 602d 282e 232a 2512 810c  6..F.;`-(.#*%...
+000009b0: 230c 141c b136 0134 0159 b013 2e14 3736  #....6.4.Y....76
+000009c0: 0059 b013 3112 1413 3314 2636 00dd 4452  .Y..1...3.&6..DR
+000009d0: b144 4a12 1413 33b0 1331 535b 56b0 535a  .DJ...3..1S[V.SZ
+000009e0: 182c 1211 3400 5951 6381 2011 1038 810b  .,..4.YQc. ..8..
+000009f0: 8047 6040 28b0 132e 1439 3600 59b0 6382  .G`@(....96.Y.c.
+00000a00: 00a8 041c 3a81 0b81 0d81 0e81 0f80 5060  ....:.........P`
+00000a10: 4028 b013 2e14 3736 0059 1211 3400 5951  @(....76.Y..4.YQ
+00000a20: 6385 00b3 8001 1c3b 810b 4b31 8059 6060  c......;..K1.Y``
+00000a30: 3a4b 624e 27b2 51de 4451 103c 141c 1281  :KbN'.Q.DQ.<....
+00000a40: 0712 1413 3334 0136 0142 41b2 b018 3112  ....34.6.BA...1.
+00000a50: 1414 32b0 1331 3601 4442 5063 127f 143d  ..2..16.DBPc...=
+00000a60: 3600 143e b136 01b0 182c b012 1413 33b2  6..>.6...,....3.
+00000a70: 5652 6387 48c0 8501 243f 810b 4b53 5480  VRc.H...$?..KST.
+00000a80: 6b80 082f 4b62 244e 5852 2910 4014 23b1  k../Kb$NXR).@.#.
+00000a90: 8082 2e02 5536 01b0 1831 1214 1432 b013  ....U6...1...2..
+00000aa0: 3136 0144 4250 63b1 b018 29b2 51de 4445  16.DBPc...).Q.DE
+00000ab0: b013 2a42 41b2 b018 2ab3 51de 4445 b013  ..*BA...*.Q.DE..
+00000ac0: 2b42 4bb3 93d8 4443 b342 43b0 132b b018  +BK...DC.BC..+..
+00000ad0: 2b12 7f14 3d36 0014 3eb0 1441 3600 3601  +...=6..>..A6.6.
+00000ae0: b018 2cb0 1214 1333 b013 3156 5263 8840  ..,....3..1VRc.@
+00000af0: c502 2242 810b 8084 6022 2924 2254 2b35  .."B....`")$"T+5
+00000b00: 484e 2c2b 484f b013 2c51 ded3 44c2 8050  HN,+HO..,Q..D..P
+00000b10: b018 2a48 0ab0 132c 1442 3600 594a 2a57  ..*H...,.B6.YJ*W
+00000b20: 1281 05df 4462 c149 1823 0d12 810a b134  ....Db.I.#.....4
+00000b30: 01dc 444c 120a 230e 141c b136 0134 0159  ..DL..#....6.4.Y
+00000b40: 5151 c128 015d 4a01 5db0 1436 3600 5942  QQ.(.]J.]..66.YB
+00000b50: 4250 634a 2157 1281 05df 4459 c149 0f12  BPcJ!W....DY.I..
+00000b60: 0a23 0f14 1cb1 3601 3401 5950 6351 51c1  .#....6.4.YPcQQ.
+00000b70: 2801 5d4a 015d 5263 841c a140 1941 810b  (.]J.]Rc...@.A..
+00000b80: 8098 8007 202e 3026 2400 127f 1443 2500  .... .0&$....C%.
+00000b90: 132b 3601 5e51 6859 121f 2500 1329 1044  .+6.^QhY..%..).D
+00000ba0: b020 0001 3482 0159 2500 132a 4342 4242  . ..4..Y%..*CBBB
+00000bb0: 4218 2500 132e 1437 3600 5951 6301 8138  B.%....76.YQc..8
+00000bc0: 320c 695b 8117 80a1 1281 2025 0010 30b1  2.i[...... %..0.
+00000bd0: 1468 3600 3403 6383 48c1 020e 4581 0b80  .h6.4.c.H...E...
+00000be0: a722 5648 0cb0 1436 1046 5236 8200 594a  ."VH...6.FR6..YJ
+00000bf0: 1f57 1281 05df 4457 c149 0d12 0a23 1014  .W....DW.I...#..
+00000c00: 1cb1 3601 3401 5951 51c1 2801 5d4a 015d  ..6.4.YQQ.(.]J.]
+00000c10: 5163 8a74 2039 158b b323 2843 8610 8e07  Qc.t 9...#(C....
+00000c20: 6940 890c 8919 8f0d 890f 890f 8910 8920  i@............. 
+00000c30: 890b 0011 8100 1681 0110 1516 8102 5116  ..............Q.
+00000c40: 4811 0c10 1634 0116 5180 1652 b020 0001  H....4..Q..R. ..
+00000c50: 1647 1181 0351 512a 0253 3301 3401 164a  .G...QQ*.S3.4..J
+00000c60: 1181 0332 0234 0116 4e11 8103 3203 3401  ...2.4..N...2.4.
+00000c70: 1650 1181 0332 0434 0116 4c11 8103 5150  .P...2.4..L...QP
+00000c80: 512a 0353 3305 3401 163e 1181 0332 0634  Q*.S3.4..>...2.4
+00000c90: 0116 5511 8103 3207 3401 165a 1181 0332  ..U...2.4..Z...2
+00000ca0: 0834 0116 5c11 8103 3209 3401 165f 1181  .4..\...2.4.._..
+00000cb0: 0332 0a34 0116 6311 8103 320b 3401 1665  .2.4..c...2.4..e
+00000cc0: b063 0c84 703a 1847 5b81 1080 b860 4048  .c..p:.G[....`@H
+00000cd0: 4f4e 5612 1513 4851 de44 7312 8111 2500  ONV...HQ.Ds...%.
+00000ce0: b115 47b1 3601 1215 1848 127f 143d 3600  ..G.6....H...=6.
+00000cf0: 1449 b113 4a36 0159 1215 1348 143e 104b  .I..J6.Y...H.>.K
+00000d00: 1215 144c 3600 1031 104d 3684 0059 1215  ...L6..1.M6..Y..
+00000d10: 1348 6381 50b2 8001 0e4a 5381 1280 c960  .Hc.P....JS....`
+00000d20: 120a 2311 141c b0b1 3602 3401 5951 6381  ..#.....6.4.YQc.
+00000d30: 3c18 064e 80d1 1281 1332 0012 1413 3314  <..N.....2....3.
+00000d40: 4f36 0034 0134 0163 0182 2849 087b 5b80  O6.4.4.c..(I.{[.
+00000d50: d12b 00b0 5f4b 1830 02c1 c2b2 132e 1435  .+.._K.0.......5
+00000d60: 3600 4331 1040 b1dd 442b 812f 1442 2663  6.C1.@..D+./.B&c
+00000d70: 8308 1810 5080 d560 402d 2b26 1215 144e  ....P..`@-+&...N
+00000d80: 3600 1215 1351 db44 5823 1214 1c12 1513  6....Q.DX#......
+00000d90: 5136 01c0 120a b034 0159 1281 05b0 3401  Q6.....4.Y....4.
+00000da0: 6551 638c 50d0 4226 4c80 e160 402b 2922  eQc.P.B&L..`@+)"
+00000db0: 202d 2d2d 4d25 4d39 1f41 3512 1413 3314   ---M%M9.A5...3.
+00000dc0: 3410 4d36 01c0 2313 141c 3600 b018 3048  4.M6..#...6...0H
+00000dd0: 7512 7f14 4322 8148 3601 5e51 6859 127f  u...C".H6.^QhY..
+00000de0: 1443 2281 4836 015e 5168 5912 7f14 4322  .C".H6.^QhY...C"
+00000df0: 8148 3601 5e51 6859 127f 1443 2281 4836  .H6.^QhY...C".H6
+00000e00: 015e 5168 5912 0e34 00c1 127f 1443 2281  .^QhY..4.....C".
+00000e10: 4836 015e 5168 5912 8114 120f 120e 3400  H6.^QhY.......4.
+00000e20: b134 0222 8148 f781 f322 8064 f434 01c2  .4.".H...".d.4..
+00000e30: 1281 1412 1513 52b2 f282 f734 0112 1518  ......R....4....
+00000e40: 5242 8d7f 4a1f 5712 8105 df44 57c3 490d  RB..J.W....DW.I.
+00000e50: 120a 2314 141c b336 0134 0159 5151 c328  ..#....6.4.YQQ.(
+00000e60: 035d 4a01 5db0 132e 1437 3600 5951 6384  .]J.]....76.YQc.
+00000e70: 20d8 8501 183e 4b31 5372 80fa 6040 4a27   ....>K1Sr..`@J'
+00000e80: 3312 8115 b012 6b34 0244 5a12 1514 5036  3.....k4.DZ...P6
+00000e90: 0059 1214 3400 143f 104b b010 53b2 1054  .Y..4..?.K..S..T
+00000ea0: b336 8600 6312 1434 0014 3b10 4bb0 1031  .6..c..4..;.K..1
+00000eb0: b136 8400 6387 0878 1855 9007 6020 2c32  .6..c..x.U..` ,2
+00000ec0: 2f30 2c2a 2912 1513 5112 1514 4e36 00f3  /0,*)...Q...N6..
+00000ed0: c023 1523 1614 1cb0 1215 1352 3602 2317  .#.#.......R6.#.
+00000ee0: 2b03 c112 1413 3314 4f36 005f 4b33 3002  +.....3.O6._K30.
+00000ef0: c2c3 b313 2e14 3536 0044 4410 5642 4210  ......56.DD.VBB.
+00000f00: 57c4 1022 8a12 8107 b434 01f3 f4c5 1058  W..".....4.....X
+00000f10: 141c b4b5 b236 03c6 b114 59b6 3601 5942  .....6....Y.6.YB
+00000f20: 0b12 8116 b134 0163 8708 611e 5a31 9016  .....4.c..a.Z1..
+00000f30: 202b 2623 282c 3c29 2a23 2212 1413 3314   +&#(,<)*#"...3.
+00000f40: 34b0 5136 02c1 b151 de44 cb80 2b00 c2b0  4.Q6...Q.D..+...
+00000f50: 141a 1040 3601 c312 1413 3314 2636 005f  ...@6.....3.&6._
+00000f60: 4b26 c4b4 1418 b380 5536 0144 5912 8107  K&......U6.DY...
+00000f70: b334 0181 d844 4fb3 8155 105b d944 47b2  .4...DO..U.[.DG.
+00000f80: 1459 b436 0159 4218 1281 07b2 3401 80d9  .Y.6.YB.....4...
+00000f90: 4443 2b00 63b2 63b0 2b01 6386 3071 1c5c  DC+.c.c.+.c.0q.\
+00000fa0: 3190 2560 2028 2a28 2a2b 2325 3712 1514  1.%` (*(*+#%7...
+00000fb0: 5ab0 3601 c112 8107 b134 0180 d944 4823  Z.6......4...DH#
+00000fc0: 1814 1cb0 3601 6312 8107 b134 0181 d944  ....6.c....4...D
+00000fd0: 4b12 1413 33b1 8055 5513 3063 2b00 c2b1  K...3..UU.0c+...
+00000fe0: 5f4b 18c3 b214 5910 5d14 1cb3 1214 1333  _K....Y.]......3
+00000ff0: b355 1330 3602 3601 5942 2610 5e14 23b2  .U.06.6.YB&.^.#.
+00001000: 3601 6388 5481 1028 5f31 9035 8007 8309  6.c.T..(_1.5....
+00001010: 2822 2a2b 2a2b 2a23 2527 302e 3200 c112  ("*+*+*#%'0.2...
+00001020: 1514 5ab0 3601 c252 c312 8107 b234 0180  ..Z.6..R.....4..
+00001030: d944 4bb3 2318 141c b036 012a 0263 1281  .DK.#....6.*.c..
+00001040: 07b2 3401 81d9 4455 2319 141c b280 55b3  ..4...DU#.....U.
+00001050: 3602 c4b1 b280 5534 01b4 2a02 632b 00c5  6.....U4..*.c+..
+00001060: b25f 4b18 c6b3 b1b6 3401 e2c3 b514 5910  ._K.....4.....Y.
+00001070: 6014 1cb6 b336 0236 0159 4226 1061 141c  `....6.6.YB&.a..
+00001080: 1062 1423 b536 0136 01c4 b3b4 2a02 6301  .b.#.6.6....*.c.
+00001090: 8458 c902 127c 8121 903d 2b22 592c 1214  .X...|.!.=+"Y,..
+000010a0: 1333 1434 b051 3602 c148 0fb1 51de 4442  .3.4.Q6..H..Q.DB
+000010b0: 5063 b114 4236 0063 4a21 5712 8105 df44  Pc..B6.cJ!W....D
+000010c0: 59c2 490f 120a 231c 141c b236 0134 0159  Y.I...#....6.4.Y
+000010d0: 5063 5151 c228 025d 4a01 5d51 6384 28b8  PcQQ.(.]J.]Qc.(.
+000010e0: 020e 6390 5560 2257 2c48 0d12 7f14 3d36  ..c.U`"W,H....=6
+000010f0: 0014 6336 0059 4a2a 5712 8105 df44 62c0  ..c6.YJ*W....Db.
+00001100: 4918 120a 231a 141c b036 0134 0159 127f  I...#....6.4.Y..
+00001110: 143d 3600 1464 3600 5951 51c0 2800 5d4a  .=6..d6.YQQ.(.]J
+00001120: 015d 5163 8218 2910 6581 1790 602c 2522  .]Qc..).e...`,%"
+00001130: 1214 1333 1434 1066 5136 02c1 b151 de44  ...3.4.fQ6...Q.D
+00001140: 4251 63b0 b118 3051 6387 3cd1 0220 1781  BQc...0Qc.<.. ..
+00001150: 0490 6b60 2042 2942 3027 5a2d 2c2b 4832  ..k` B)B0'Z-,+H2
+00001160: b014 1810 1936 0144 4252 6332 00b0 141a  .....6.DBRc2....
+00001170: 101b 3601 5e34 015f 4b16 c112 1eb1 3401  ..6.^4._K.....4.
+00001180: 434c 1209 2301 141c b136 0134 0159 4228  CL..#....6.4.YB(
+00001190: 4a2e 5712 8105 df44 66c2 491c 1209 2302  J.W....Df.I...#.
+000011a0: 141c b0b2 3602 3401 5912 0a23 0314 1cb2  ....6.4.Y..#....
+000011b0: 3601 3401 5950 6351 51c2 2802 5d4a 015d  6.4.YPcQQ.(.]J.]
+000011c0: 5263 0182 38b9 4008 675b 9074 53b0 5353  Rc..8.@.g[.tS.SS
+000011d0: 4b18 c112 8107 b134 0180 d844 33b1 1468  K......4...D3..h
+000011e0: 3600 141a 3600 6759 4226 5163 8378 c102  6...6.gYB&Qc.x..
+000011f0: 161d 8104 907f 6020 2228 4e2c 480c 1206  ......` "(N,H...
+00001200: 1217 b034 0259 5263 4a21 5712 8105 df44  ...4.YRcJ!W....D
+00001210: 59c1 490f 120a 2304 141c b136 0134 0159  Y.I...#....6.4.Y
+00001220: 5063 5151 c128 015d 4a01 5d51 6383 3caa  PcQQ.(.]J.]Qc.<.
+00001230: 019e 011e 8106 4490 8c80 0726 4486 2c60  ......D....&D.,`
+00001240: 2742 0001 2501 51de 4444 3200 2701 b0b1  'B..%.Q.DD2.'...
+00001250: 2001 02c2 b225 0034 0144 4252 6312 1f25   ....%.4.DBRc..%
+00001260: 0025 0134 0263 0248 090a 6981 1790 9451  .%.4.c.H..i....Q
+00001270: 6395 0893 124c 6a5b 5b81 1890 9747 492d  c....Lj[[....GI-
+00001280: 2d28 2642 2528 3026 2228 3122 2742 5028  -(&B%(0&"(1"'BP(
+00001290: 302e 5122 5c46 2b2e 234e 4c42 1281 07b2  0.Q"\F+.#NLB....
+000012a0: 3401 c310 2cb2 8055 d944 f380 b382 d944  4...,..U.D.....D
+000012b0: 6510 6bb2 8155 d944 5d10 5e14 2312 1514  e.k..U.D].^.#...
+000012c0: 5536 0036 01c4 106c 141c b436 01c4 2501  U6.6...l...6..%.
+000012d0: b434 0159 5263 b382 d844 7b10 5fb2 8155  .4.YRc...D{._..U
+000012e0: d944 5812 1514 5f10 31b2 8255 3682 0030  .DX..._.1..U6..0
+000012f0: 02c5 c625 01b6 3401 5952 6310 5cb2 8155  ...%..4.YRc.\..U
+00001300: d944 5325 0112 1514 5c10 31b2 8255 3682  .DS%....\.1..U6.
+00001310: 0034 0159 5263 2501 231b 3401 5952 63b3  .4.YRc%.#.4.YRc.
+00001320: 82d8 449d 8110 6d25 007f 55dd 4493 8125  ..D...m%..U.D..%
+00001330: 0014 6e7f 3601 c7b7 146f 106d 3601 82d9  ..n.6....o.m6...
+00001340: 4443 5242 4150 c8b7 1470 106d 102f 3602  DCRBAP...p.m./6.
+00001350: 1468 3600 c9b9 1471 3600 4448 1281 14b9  .h6....q6.DH....
+00001360: 3401 4241 51c9 4812 1215 143e 2500 1053  4.BAQ.H....>%..S
+00001370: b810 72b9 3684 01c5 4a1b 5712 8105 df44  ..r.6...J.W....D
+00001380: 53ca 4909 2501 ba34 0159 5263 5151 ca28  S.I.%..4.YRcQQ.(
+00001390: 0a5d 4a01 5d10 4014 2325 0080 822e 0255  .]J.].@.#%.....U
+000013a0: 3601 cbb5 444e 2501 1073 141c bb36 0134  6...DN%..s...6.4
+000013b0: 0159 424c 2501 1074 141c bb36 0134 0159  .YBL%..t...6.4.Y
+000013c0: 5263 5063 9554 9e12 4b1f 8106 4490 cc80  RcPc.T..K...D...
+000013d0: 0883 0d85 0f27 4d2b 1f21 6327 2d42 7d2a  .....'M+.!c'-B}*
+000013e0: 4c4d 5270 492b 6f2d 562a 462b 2646 0a32  LMRpI+o-V*F+&F.2
+000013f0: 00c2 ba20 0101 c3b0 7f55 1020 d9c4 b444  ... .....U. ...D
+00001400: 48b0 807f 2e02 5542 41b0 c512 8107 b534  H.....UBA......4
+00001410: 0182 db44 fc81 1021 141c b580 5536 01b5  ...D...!....U6..
+00001420: 8155 b210 2214 23b5 8251 2e02 5536 0134  .U..".#..Q..U6.4
+00001430: 015b 5ac6 c7c8 4890 01b6 1202 ddd3 444d  .[Z...H.......DM
+00001440: 1281 0810 2414 1cb6 3601 3401 5948 1212  ....$...6.4.YH..
+00001450: 8109 1025 141c b6b7 b836 0334 0127 0a4a  ...%.....6.4.'.J
+00001460: 5057 1281 05df 44c7 80c9 493d b612 810a  PW....D...I=....
+00001470: b934 01dd 446b 120a 2305 141c b636 0134  .4..Dk..#....6.4
+00001480: 0159 1281 0810 2414 1cb6 3601 3401 5912  .Y....$...6.4.Y.
+00001490: 8109 1025 141c b6b7 b836 0334 0127 0a42  ...%.....6.4.'.B
+000014a0: 4712 8105 b934 0165 5151 c928 095d 4a01  G....4.eQQ.(.]J.
+000014b0: 5db3 b4b7 250a 3403 270a b112 810a 250a  ]...%.4.'.....%.
+000014c0: 3401 3401 5952 634a 4957 1281 05df 44c0  4.4.YRcJIW....D.
+000014d0: 80c9 4936 b123 0614 1cb6 b7b9 3603 3401  ..I6.#......6.4.
+000014e0: 5923 0712 810a b934 01dd 434b 2308 1281  Y#.....4..CK#...
+000014f0: 0ab9 3401 dd44 52b6 1202 1426 3600 dd44  ..4..DR....&6..D
+00001500: 4612 02b6 535b 5650 6351 51c9 2809 5d4a  F...S[VPcQQ.(.]J
+00001510: 015d b123 0934 0159 b123 0a34 0159 5263  .].#.4.Y.#.4.YRc
+00001520: 0287 5c59 9c01 7581 1990 d522 2e2d 3625  ..\Y..u....".-6%
+00001530: 2d2c 2a2a 0003 51c1 1076 2500 dd43 4710  -,**..Q..v%..CG.
+00001540: 7725 00dd 4475 3200 1281 1a25 0034 0134  w%..Du2....%.4.4
+00001550: 0127 03b0 b320 0102 1281 1b80 1281 0725  .'... .........%
+00001560: 0334 0182 3403 3401 c1b1 5f4b 0ec2 2500  .4..4.4..._K..%.
+00001570: 1470 b210 7836 0227 0042 3025 0014 7010  .p..x6.'.B0%..p.
+00001580: 2210 6236 0227 0012 8115 b112 6b34 0244  ".b6.'......k4.D
+00001590: 4a25 0014 1cb1 8137 0127 0025 0063 0282  J%.....7.'.%.c..
+000015a0: 1049 087b 5b90 d72b 00b0 5f4b 1530 02c1  .I.{[..+.._K.0..
+000015b0: c2b2 1077 d943 46b2 1076 d944 2eb1 2f14  ...w.CF..v.D../.
+000015c0: 4229 6382 286b 0c7b 5b5b 5b90 d82b 00b2  B)c.(k.{[[[..+..
+000015d0: 5f4b 16c3 2500 2501 b355 2501 b381 f255  _K..%.%..U%....U
+000015e0: 81f2 2e02 552f 1442 2863 853c c004 2479  ....U/.B(c.<..$y
+000015f0: 5b81 1c81 1d81 1e90 e22b 2346 5126 2346  [........+#FQ&#F
+00001600: 2c12 8115 b312 811f 3402 445a b144 4612  ,.......4.DZ.DF.
+00001610: 04b3 3401 6310 5e14 2332 0025 0014 4f36  ..4.c.^.#2.%..O6
+00001620: 0034 0136 0163 b210 7ad9 4455 b144 4612  .4.6.c..z.DU.DF.
+00001630: 04b3 3401 6310 5e14 2332 01b3 3401 3601  ..4.c.^.#2..4.6.
+00001640: 63b3 6302 8168 5908 7b5b 90e6 2b00 b05f  c.c..hY.{[..+.._
+00001650: 4b10 3002 c1c2 107d 141c b1b2 3602 2f14  K.0....}....6./.
+00001660: 422e 6381 4849 087b 5b90 ec2b 00b0 5f4b  B.c.HI.{[..+.._K
+00001670: 0cc1 107e 141c b136 012f 1442 3263 8400  ...~...6./.B2c..
+00001680: c902 1627 8106 a01d 6040 2228 4e2d 480c  ...'....`@"(N-H.
+00001690: 1206 121e b034 0259 5263 4a22 5712 8105  .....4.YRcJ"W...
+000016a0: df44 5ac1 4910 120a 230b 141c b0b1 3602  .DZ.I...#.....6.
+000016b0: 3401 5950 6351 51c1 2801 5d4a 015d 5163  4.YPcQQ.(.]J.]Qc
```

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/Time.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Time.mpy`

 * *Files 3% similar despite different names*

```diff
@@ -13,160 +13,159 @@
 000000c0: 001a 636f 6e73 6f6c 655f 7772 6974 6500  ..console_write.
 000000d0: 0a44 6562 7567 0081 2d12 7572 6571 7565  .Debug..-.ureque
 000000e0: 7374 7300 0653 756e 0002 7200 0675 7463  sts..Sun..r..utc
 000000f0: 0010 7365 745f 7469 6d65 0010 6461 7465  ..set_time..date
 00000100: 7469 6d65 000e 424f 4f54 494d 4500 106e  time..BOOTIME..n
 00000110: 7470 5f74 696d 6500 1669 7363 6f6e 6e65  tp_time..isconne
 00000120: 6374 6564 000c 7374 7275 6374 0003 0863  cted..struct...c
-00000130: 726f 6e00 0655 5443 0081 2934 5f5f 7065  ron..UTC..)4__pe
-00000140: 7273 6973 7465 6e74 5f63 6163 6865 5f6d  rsistent_cache_m
-00000150: 616e 6167 6572 0002 7300 0e73 756e 2e70  anager..s..sun.p
-00000160: 6473 0002 7700 0854 494d 4500 814d 8249  ds..w..TIME..M.I
-00000170: 023b 0081 5181 7b82 3182 230e 7375 6e74  .;..Q.{.1.#.sunt
-00000180: 696d 6500 0e6a 736f 6e69 6679 0006 6c61  ime..jsonify..la
-00000190: 7400 066c 6f6e 000c 6f66 6673 6574 000e  t..lon..offset..
-000001a0: 7375 6e72 6973 6500 0c73 756e 7365 7400  sunrise..sunset.
-000001b0: 1273 6f63 6b5f 7369 7a65 000e 7265 7375  .sock_size..resu
-000001c0: 6c74 7300 1454 285b 302d 393a 5d2b 2900  lts..T([0-9:]+).
-000001d0: 0c73 6561 7263 6800 0a67 726f 7570 0002  .search..group..
-000001e0: 3a00 8155 0c75 7074 696d 6500 0e67 6574  :..U.uptime..get
-000001f0: 5f6e 7470 0014 7365 7474 696d 656f 7574  _ntp..settimeout
-00000200: 000c 7365 6e64 746f 0008 7265 6376 0081  ..sendto..recv..
-00000210: 0f0c 756e 7061 636b 0004 2149 0014 3c6c  ..unpack..!I..<l
-00000220: 6973 7463 6f6d 703e 000a 7b7d 3a7b 7d00  istcomp>..{}:{}.
-00000230: 022d 0014 3c64 6963 7463 6f6d 703e 0010  .-..<dictcomp>..
-00000240: 6874 7470 5f67 6574 002f 2d35 0879 6561  http_get./-5.yea
-00000250: 7200 0a6d 6f6e 7468 0008 6d64 6179 0008  r..month..mday..
-00000260: 686f 7572 0006 6d69 6e00 0673 6563 0049  hour..min..sec.I
-00000270: 086d 6f64 6500 816d 823b 813d 823f 0b81  .mode..m.;.=.?..
-00000280: 0182 2f05 1a53 5441 206e 6f74 2063 6f6e  ../..STA not con
-00000290: 6e65 6374 6564 3a20 6e74 7074 696d 6500  nected: ntptime.
-000002a0: 0511 6e74 7074 696d 6520 6572 726f 722e  ..ntptime error.
-000002b0: 3a7b 7d00 0517 5b45 5252 5d20 6e74 7074  :{}...[ERR] ntpt
-000002c0: 696d 6520 6572 726f 723a 207b 7d00 0514  ime error: {}...
-000002d0: 4372 6f6e 3a20 7b7d 202d 2053 4b49 5020  Cron: {} - SKIP 
-000002e0: 7379 6e63 0005 1e5b 7375 6e74 696d 655d  sync...[suntime]
-000002f0: 2061 7069 2073 796e 6320 7374 6172 7465   api sync starte
-00000300: 6420 2e2e 2e00 0536 6874 7470 3a2f 2f69  d .....6http://i
-00000310: 702d 6170 692e 636f 6d2f 6a73 6f6e 2f3f  p-api.com/json/?
-00000320: 6669 656c 6473 3d6c 6174 2c6c 6f6e 2c74  fields=lat,lon,t
-00000330: 696d 657a 6f6e 652c 6f66 6673 6574 0005  imezone,offset..
-00000340: 1969 702d 6170 6920 6572 726f 723a 207b  .ip-api error: {
-00000350: 7d20 6461 7461 3a20 7b7d 0005 4868 7474  } data: {}..Hhtt
-00000360: 7073 3a2f 2f61 7069 2e73 756e 7269 7365  ps://api.sunrise
-00000370: 2d73 756e 7365 742e 6f72 672f 6a73 6f6e  -sunset.org/json
-00000380: 3f6c 6174 3d7b 7d26 6c6e 673d 7b7d 2664  ?lat={}&lng={}&d
-00000390: 6174 653d 746f 6461 7926 666f 726d 6174  ate=today&format
-000003a0: 7465 643d 3000 051e 7375 6e72 6973 652d  ted=0...sunrise-
-000003b0: 6170 6920 6572 726f 723a 207b 7d20 6461  api error: {} da
-000003c0: 7461 3a20 7b7d 0005 2373 756e 7269 7365  ta: {}..#sunrise
-000003d0: 2d61 7069 2070 6172 7365 2065 7272 6f72  -api parse error
-000003e0: 3a20 7b7d 2073 756e 3a20 7b7d 0005 1b5b  : {} sun: {}...[
-000003f0: 7375 6e74 696d 655d 206c 6f61 6465 6420  suntime] loaded 
-00000400: 6672 6f6d 2063 6163 6865 0005 1e5b 7375  from cache...[su
-00000410: 6e74 696d 655d 2073 796e 6320 646f 6e65  ntime] sync done
-00000420: 2061 6e64 2063 6163 6865 6400 0523 4e6f   and cached..#No
-00000430: 2074 696d 6520 6675 6e63 7469 6f6e 2077   time function w
-00000440: 6173 2069 6e69 7469 616c 697a 6564 2e2e  as initialized..
-00000450: 2e00 050b 7b7d 207b 7d3a 7b7d 3a7b 7d00  ....{} {}:{}:{}.
-00000460: 050c 706f 6f6c 2e6e 7470 2e6f 7267 0007  ..pool.ntp.org..
-00000470: 0a33 3135 3536 3733 3630 308d 3c20 2a01  .3155673600.< *.
-00000480: 2c5e 2c32 5e32 326c 6960 8411 8432 841a  ,^,2^22li`...2..
-00000490: 8441 880f 8010 022a 011b 031c 0216 0259  .A.....*.......Y
-000004a0: 8010 0410 0510 0610 072a 041b 041c 0416  .........*......
-000004b0: 041c 0516 051c 0616 061c 0716 0759 8010  .............Y..
-000004c0: 082a 011b 091c 0816 0859 8010 0a10 0b2a  .*.......Y.....*
-000004d0: 021b 0c1c 0a16 0a1c 0b16 0b59 8010 0d10  ...........Y....
-000004e0: 0e10 0f10 102a 041b 111c 0d16 0d1c 0e16  .....*..........
-000004f0: 0e1c 0f16 0f1c 1016 1059 8010 1210 132a  .........Y.....*
-00000500: 021b 141c 1216 121c 1316 1359 8010 1510  ...........Y....
-00000510: 162a 021b 171c 1516 151c 1616 1659 8010  .*...........Y..
-00000520: 182a 011b 191c 1816 4d59 5432 0010 1a34  .*......MYT2...4
-00000530: 0216 1a32 0116 1d32 0216 2032 0316 2732  ...2...2.. 2..'2
-00000540: 0416 3350 2a01 5333 0516 4111 2710 1b34  ..3P*.S3..A.'..4
-00000550: 0159 5163 0682 0008 0a1a 880d 2428 114e  .YQc........$(.N
-00000560: 164f 101a 1650 2c00 162b 1113 101c 3401  .O...P,..+....4.
-00000570: 1625 5116 1f51 6384 6882 1420 1d51 5253  .%Q..Qc.h.. .QRS
-00000580: 5455 5680 1360 404f 4653 2828 120f b0b1  TUV..`@OFS((....
-00000590: b2b3 b4b5 8080 2a08 3401 c612 10b6 3401  ......*.4.....4.
-000005a0: 5912 0834 0014 1eb0 b1b2 80b3 b4b5 802a  Y..4...........*
-000005b0: 0836 0159 121a 131f 51de 4448 120e 3400  .6.Y....Q.DH..4.
-000005c0: 121a 181f 5263 8d6c 9012 3320 8024 6060  ....Rc.l..3 .$``
-000005d0: 2c27 4246 8511 2332 4224 4e1f 4428 284d  ,'BF..#2B$N.D((M
-000005e0: 2c2b 322c 0612 0a12 0b34 0114 2136 0043  ,+2,.....4..!6.C
-000005f0: 4912 1523 0034 0159 5063 8051 1b22 2706  I..#.4.YPc.Q."'.
-00000600: b620 0001 c010 23c1 1213 1024 3401 4443  . ....#....$4.DC
-00000610: 8442 4182 8042 f780 57c2 4849 b034 00c3  .BA..B..W.HI.4..
-00000620: 1210 b312 1a13 2522 3cf4 f234 01c4 1208  ......%"<..4....
-00000630: 3400 141e b480 55b4 8155 b482 55b4 8655  4.....U..U..U..U
-00000640: 81f2 b483 55b4 8455 b485 5580 2a08 3601  ....U..U..U.*.6.
-00000650: 5912 1a13 1f51 de44 4812 0e34 0012 1a18  Y....Q.DH..4....
-00000660: 1f52 634a 2057 1257 df44 59c5 490f 1216  .RcJ W.W.DY.I...
-00000670: 2301 1426 b536 0134 0159 b5c1 5151 c528  #..&.6.4.Y..QQ.(
-00000680: 055d 4a01 5d12 0d22 8064 3401 5981 e558  .]J.]..".d4.Y..X
-00000690: 5ad7 4383 7f59 5912 1523 0214 26b1 3601  Z.C..YY..#..&.6.
-000006a0: 3401 5950 6301 8678 7520 425d 8031 4323  4.YPc..xu B].1C#
-000006b0: 2724 2d29 2227 2849 2731 230e c123 0fc2  '$-)"'(I'1#..#..
-000006c0: 125e 2230 3401 c39b b380 5612 05b1 2280  .^"04.....V...".
-000006d0: 7b34 0280 557f 55c4 1204 1206 1207 3402  {4..U.U.......4.
-000006e0: c549 18b5 1443 8236 0159 b514 44b3 b436  .I...C.6.Y..D..6
-000006f0: 0259 b514 4522 3036 01c6 51b5 1446 3600  .Y..E"06..Q..F6.
-00000700: 595d 2500 1447 1048 b6a8 ac2e 0255 3602  Y]%..G.H.....U6.
-00000710: 8055 c7b7 b2f3 638a 7c89 1226 2758 8056  .U....c.|..&'X.V
-00000720: 6040 4723 222b 2f2e 5923 422b 342c 57b0  `@G#"+/.Y#B+4,W.
-00000730: 1028 d944 c980 2c00 c149 4112 5910 2910  .(.D..,..IA.Y.).
-00000740: 2a34 0247 34c2 121a 132b 142c 3600 5f4b  *4.G4....+.,6._K
-00000750: 1230 02c3 c412 5a32 00b4 3401 3401 b1b3  .0....Z2..4.4...
-00000760: 5642 2cb2 142d 102e 142f 3201 b114 2c36  VB,..-.../2...,6
-00000770: 0034 0136 0136 0159 515c 5d51 5163 5d48  .4.6.6.YQ\]QQc]H
-00000780: 4112 5910 2910 1b34 0247 33c2 3202 b214  A.Y.)..4.G3.2...
-00000790: 3036 0014 3136 0014 3210 2e36 0134 01c5  06..16..2..6.4..
-000007a0: b514 2c36 005f 4b15 3002 c3c4 125a 3203  ..,6._K.0....Z2.
-000007b0: b434 0134 0112 1a13 2bb3 5642 2951 5c5d  .4.4....+.VB)Q\]
-000007c0: 4a04 594a 015d 5163 0481 3841 0849 5d80  J.YJ.]Qc..8A.I].
-000007d0: 612b 00b0 5f4b 0ac1 125f b134 012f 1442  a+.._K..._.4./.B
-000007e0: 3463 8218 6908 495d 8062 2b00 b05f 4b16  4c..i.I].b+.._K.
-000007f0: 3002 c1c2 104a 1426 b110 4b14 2fb2 3601  0....J.&..K./.6.
-00000800: 3602 2f14 4228 6382 5051 084c 5d80 682c  6./.B(c.PQ.L].h,
-00000810: 00b0 5f4b 1dc1 b114 3210 3f36 0181 5514  .._K....2.?6..U.
-00000820: 3210 4b36 01b1 1432 103f 3601 8055 2f19  2.K6...2.?6..U/.
-00000830: 4221 6381 3841 0849 5d80 6a2b 00b0 5f4b  B!c.8A.I].j+.._K
-00000840: 0ac1 125b b134 012f 1442 3463 9d54 a012  ...[.4./.B4c.T..
-00000850: 5e33 8070 8007 282d 2642 6720 2323 222d  ^3.p..(-&Bg ##"-
-00000860: 2828 3257 2d6e 202d 2c29 2232 2827 223a  ((2W-n -,)"2('":
-00000870: 1f67 5622 292a 3457 4d27 276e 2025 2727  .gV")*4WM''n %''
-00000880: 1213 1024 3401 4355 2303 1426 1213 1024  ...$4.CU#..&...$
-00000890: 3401 3601 c012 16b0 3401 59b0 6312 1623  4.6.....4.Y.c..#
-000008a0: 0434 0159 2305 c12c 00c2 483d 124d b110  .4.Y#..,..H=.M..
-000008b0: 3452 3482 0130 02c3 c2b2 1418 1035 3601  4R4..0.......56.
-000008c0: c4b2 1418 1036 3601 c512 5bb2 1418 1037  .....66...[....7
-000008d0: 3601 223c f734 0112 1a18 2512 1210 1c12  6."<.4....%.....
-000008e0: 1a13 2552 3403 594a 2457 1257 df44 5dc6  ..%R4.YJ$W.W.D].
-000008f0: 4913 1215 2306 1426 b6b2 3602 3401 5912  I...#..&..6.4.Y.
-00000900: 1a13 2b63 5151 c628 065d 4a01 5d2c 022a  ..+cQQ.(.]J.],.*
-00000910: 0010 3862 2a00 1039 62c7 b451 de43 8a81  ..8b*..9b..Q.C..
-00000920: b551 de43 8481 2307 1426 b4b5 3602 c148  .Q.C..#..&..6..H
-00000930: 5a12 4db1 103a 2288 0010 3452 3484 0130  Z.M..:"...4R4..0
-00000940: 02c3 c2b2 1418 103b 3601 c812 0210 3c34  .......;6.....<4
-00000950: 01c9 2c02 b914 3db8 1418 1038 3601 3601  ..,...=....86.6.
-00000960: 143e 8136 0114 3210 3f36 0110 3862 b914  .>.6..2.?6..8b..
-00000970: 3db8 1418 1039 3601 3601 143e 8136 0114  =....96.6..>.6..
-00000980: 3210 3f36 0110 3962 c74a 1f57 1257 df44  2.?6..9b.J.W.W.D
-00000990: 58c6 490e 1215 2308 1426 b6b2 3602 3401  X.I...#..&..6.4.
-000009a0: 5951 51c6 2806 5d4a 015d 4835 b714 4036  YQQ.(.]J.]H5..@6
-000009b0: 005f 4b2b ca32 00b7 ba55 3401 b7ba 56b7  ._K+.2...U4...V.
-000009c0: ba55 8058 5512 5b12 1a13 2522 3cf7 3401  .U.XU.[...%"<.4.
-000009d0: e55b 5612 5ab7 ba55 3401 b7ba 5642 134a  .[V.Z..U4...VB.J
-000009e0: 3257 1257 df44 6bc6 4921 1215 2309 1426  2W.W.Dk.I!..#..&
-000009f0: b6b7 3602 3401 5912 2710 1b34 0159 1216  ..6.4.Y.'..4.Y..
-00000a00: 230a 3401 5912 1a13 2b63 5151 c628 065d  #.4.Y...+cQQ.(.]
-00000a10: 4a01 5db7 121a 182b 1227 1028 3401 5912  J.]....+.'.(4.Y.
-00000a20: 1623 0b34 0159 b763 0181 3841 0849 5d80  .#.4.Y.c..8A.I].
-00000a30: 9e2b 00b0 5f4b 0ac1 125b b134 012f 1442  .+.._K...[.4./.B
-00000a40: 3463 8710 e101 1a41 5c80 b160 2023 2828  4c.....A\..` #((
-00000a50: 232e 1f24 b044 4812 0e34 0012 1a18 1f12  #..$.DH..4......
-00000a60: 1a13 1f51 de44 4323 0c63 125b 120e 3400  ...Q.DC#.c.[..4.
-00000a70: 121a 131f f334 01c1 b122 85a3 00f6 b122  .....4..."....."
-00000a80: 85a3 00f8 229c 10f6 b122 3cf7 223c f8b1  ...."...."<."<..
-00000a90: 223c f82a 0430 04c2 c3c4 c523 0d14 2612  "<.*.0.....#..&.
-00000aa0: 5bb2 3401 125b b334 0112 5bb4 3401 125b  [.4..[.4..[.4..[
-00000ab0: b534 0136 0463                           .4.6.c
+00000130: 726f 6e00 0655 5443 0081 2916 5f5f 7375  ron..UTC..).__su
+00000140: 6e5f 6361 6368 6500 0273 000e 7375 6e2e  n_cache..s..sun.
+00000150: 7064 7300 0277 0008 5449 4d45 0081 4d82  pds..w..TIME..M.
+00000160: 4902 3b00 8151 817b 8231 8223 0e73 756e  I.;..Q.{.1.#.sun
+00000170: 7469 6d65 000e 6a73 6f6e 6966 7900 066c  time..jsonify..l
+00000180: 6174 0006 6c6f 6e00 0c6f 6666 7365 7400  at..lon..offset.
+00000190: 0e73 756e 7269 7365 000c 7375 6e73 6574  .sunrise..sunset
+000001a0: 0012 736f 636b 5f73 697a 6500 0e72 6573  ..sock_size..res
+000001b0: 756c 7473 0014 5428 5b30 2d39 3a5d 2b29  ults..T([0-9:]+)
+000001c0: 000c 7365 6172 6368 000a 6772 6f75 7000  ..search..group.
+000001d0: 023a 0081 550c 7570 7469 6d65 000e 6765  .:..U.uptime..ge
+000001e0: 745f 6e74 7000 1473 6574 7469 6d65 6f75  t_ntp..settimeou
+000001f0: 7400 0c73 656e 6474 6f00 0872 6563 7600  t..sendto..recv.
+00000200: 810f 0c75 6e70 6163 6b00 0421 4900 143c  ...unpack..!I..<
+00000210: 6c69 7374 636f 6d70 3e00 0a7b 7d3a 7b7d  listcomp>..{}:{}
+00000220: 0002 2d00 143c 6469 6374 636f 6d70 3e00  ..-..<dictcomp>.
+00000230: 1068 7474 705f 6765 7400 2f2d 3508 7965  .http_get./-5.ye
+00000240: 6172 000a 6d6f 6e74 6800 086d 6461 7900  ar..month..mday.
+00000250: 0868 6f75 7200 066d 696e 0006 7365 6300  .hour..min..sec.
+00000260: 4908 6d6f 6465 0081 6d82 3b81 3d82 3f0b  I.mode..m.;.=.?.
+00000270: 8101 822f 051a 5354 4120 6e6f 7420 636f  .../..STA not co
+00000280: 6e6e 6563 7465 643a 206e 7470 7469 6d65  nnected: ntptime
+00000290: 0005 116e 7470 7469 6d65 2065 7272 6f72  ...ntptime error
+000002a0: 2e3a 7b7d 0005 175b 4552 525d 206e 7470  .:{}...[ERR] ntp
+000002b0: 7469 6d65 2065 7272 6f72 3a20 7b7d 0005  time error: {}..
+000002c0: 1443 726f 6e3a 207b 7d20 2d20 534b 4950  .Cron: {} - SKIP
+000002d0: 2073 796e 6300 051e 5b73 756e 7469 6d65   sync...[suntime
+000002e0: 5d20 6170 6920 7379 6e63 2073 7461 7274  ] api sync start
+000002f0: 6564 202e 2e2e 0005 3668 7474 703a 2f2f  ed .....6http://
+00000300: 6970 2d61 7069 2e63 6f6d 2f6a 736f 6e2f  ip-api.com/json/
+00000310: 3f66 6965 6c64 733d 6c61 742c 6c6f 6e2c  ?fields=lat,lon,
+00000320: 7469 6d65 7a6f 6e65 2c6f 6666 7365 7400  timezone,offset.
+00000330: 0519 6970 2d61 7069 2065 7272 6f72 3a20  ..ip-api error: 
+00000340: 7b7d 2064 6174 613a 207b 7d00 0548 6874  {} data: {}..Hht
+00000350: 7470 733a 2f2f 6170 692e 7375 6e72 6973  tps://api.sunris
+00000360: 652d 7375 6e73 6574 2e6f 7267 2f6a 736f  e-sunset.org/jso
+00000370: 6e3f 6c61 743d 7b7d 266c 6e67 3d7b 7d26  n?lat={}&lng={}&
+00000380: 6461 7465 3d74 6f64 6179 2666 6f72 6d61  date=today&forma
+00000390: 7474 6564 3d30 0005 1e73 756e 7269 7365  tted=0...sunrise
+000003a0: 2d61 7069 2065 7272 6f72 3a20 7b7d 2064  -api error: {} d
+000003b0: 6174 613a 207b 7d00 0523 7375 6e72 6973  ata: {}..#sunris
+000003c0: 652d 6170 6920 7061 7273 6520 6572 726f  e-api parse erro
+000003d0: 723a 207b 7d20 7375 6e3a 207b 7d00 051b  r: {} sun: {}...
+000003e0: 5b73 756e 7469 6d65 5d20 6c6f 6164 6564  [suntime] loaded
+000003f0: 2066 726f 6d20 6361 6368 6500 051e 5b73   from cache...[s
+00000400: 756e 7469 6d65 5d20 7379 6e63 2064 6f6e  untime] sync don
+00000410: 6520 616e 6420 6361 6368 6564 0005 234e  e and cached..#N
+00000420: 6f20 7469 6d65 2066 756e 6374 696f 6e20  o time function 
+00000430: 7761 7320 696e 6974 6961 6c69 7a65 642e  was initialized.
+00000440: 2e2e 0005 0b7b 7d20 7b7d 3a7b 7d3a 7b7d  .....{} {}:{}:{}
+00000450: 0005 0c70 6f6f 6c2e 6e74 702e 6f72 6700  ...pool.ntp.org.
+00000460: 070a 3331 3535 3637 3336 3030 8d3c 202a  ..3155673600.< *
+00000470: 012c 5e2c 325e 3232 6c69 6084 1184 3284  .,^,2^22li`...2.
+00000480: 1a84 4188 0f80 1002 2a01 1b03 1c02 1602  ..A.....*.......
+00000490: 5980 1004 1005 1006 1007 2a04 1b04 1c04  Y.........*.....
+000004a0: 1604 1c05 1605 1c06 1606 1c07 1607 5980  ..............Y.
+000004b0: 1008 2a01 1b09 1c08 1608 5980 100a 100b  ..*.......Y.....
+000004c0: 2a02 1b0c 1c0a 160a 1c0b 160b 5980 100d  *...........Y...
+000004d0: 100e 100f 1010 2a04 1b11 1c0d 160d 1c0e  ......*.........
+000004e0: 160e 1c0f 160f 1c10 1610 5980 1012 1013  ..........Y.....
+000004f0: 2a02 1b14 1c12 1612 1c13 1613 5980 1015  *...........Y...
+00000500: 1016 2a02 1b17 1c15 1615 1c16 1616 5980  ..*...........Y.
+00000510: 1018 2a01 1b19 1c18 164d 5954 3200 101a  ..*......MYT2...
+00000520: 3402 161a 3201 161d 3202 1620 3203 1627  4...2...2.. 2..'
+00000530: 3204 1633 502a 0153 3305 1641 1127 101b  2..3P*.S3..A.'..
+00000540: 3401 5951 6306 8200 080a 1a88 0d24 2811  4.YQc........$(.
+00000550: 4e16 4f10 1a16 502c 0016 2b11 1310 1c34  N.O...P,..+....4
+00000560: 0116 2551 161f 5163 8468 8214 201d 5152  ..%Q..Qc.h.. .QR
+00000570: 5354 5556 8013 6040 4f46 5328 2812 0fb0  STUV..`@OFS((...
+00000580: b1b2 b3b4 b580 802a 0834 01c6 1210 b634  .......*.4.....4
+00000590: 0159 1208 3400 141e b0b1 b280 b3b4 b580  .Y..4...........
+000005a0: 2a08 3601 5912 1a13 1f51 de44 4812 0e34  *.6.Y....Q.DH..4
+000005b0: 0012 1a18 1f52 638d 6c90 1233 2080 2460  .....Rc.l..3 .$`
+000005c0: 602c 2742 4685 1123 3242 244e 1f44 2828  `,'BF..#2B$N.D((
+000005d0: 4d2c 2b32 2c06 120a 120b 3401 1421 3600  M,+2,.....4..!6.
+000005e0: 4349 1215 2300 3401 5950 6380 511b 2227  CI..#.4.YPc.Q."'
+000005f0: 06b6 2000 01c0 1023 c112 1310 2434 0144  .. ....#....$4.D
+00000600: 4384 4241 8280 42f7 8057 c248 49b0 3400  C.BA..B..W.HI.4.
+00000610: c312 10b3 121a 1325 223c f4f2 3401 c412  .......%"<..4...
+00000620: 0834 0014 1eb4 8055 b481 55b4 8255 b486  .4.....U..U..U..
+00000630: 5581 f2b4 8355 b484 55b4 8555 802a 0836  U....U..U..U.*.6
+00000640: 0159 121a 131f 51de 4448 120e 3400 121a  .Y....Q.DH..4...
+00000650: 181f 5263 4a20 5712 57df 4459 c549 0f12  ..RcJ W.W.DY.I..
+00000660: 1623 0114 26b5 3601 3401 59b5 c151 51c5  .#..&.6.4.Y..QQ.
+00000670: 2805 5d4a 015d 120d 2280 6434 0159 81e5  (.]J.]..".d4.Y..
+00000680: 585a d743 837f 5959 1215 2302 1426 b136  XZ.C..YY..#..&.6
+00000690: 0134 0159 5063 0186 7875 2042 5d80 3143  .4.YPc..xu B].1C
+000006a0: 2327 242d 2922 2728 4927 3123 0ec1 230f  #'$-)"'(I'1#..#.
+000006b0: c212 5e22 3034 01c3 9bb3 8056 1205 b122  ..^"04.....V..."
+000006c0: 807b 3402 8055 7f55 c412 0412 0612 0734  .{4..U.U.......4
+000006d0: 02c5 4918 b514 4382 3601 59b5 1444 b3b4  ..I...C.6.Y..D..
+000006e0: 3602 59b5 1445 2230 3601 c651 b514 4636  6.Y..E"06..Q..F6
+000006f0: 0059 5d25 0014 4710 48b6 a8ac 2e02 5536  .Y]%..G.H.....U6
+00000700: 0280 55c7 b7b2 f363 8a7c 8912 2627 5880  ..U....c.|..&'X.
+00000710: 5660 4047 2322 2b2f 2e59 2342 2b34 2c57  V`@G#"+/.Y#B+4,W
+00000720: b010 28d9 44c9 802c 00c1 4941 1259 1029  ..(.D..,..IA.Y.)
+00000730: 102a 3402 4734 c212 1a13 2b14 2c36 005f  .*4.G4....+.,6._
+00000740: 4b12 3002 c3c4 125a 3200 b434 0134 01b1  K.0....Z2..4.4..
+00000750: b356 422c b214 2d10 2e14 2f32 01b1 142c  .VB,..-.../2...,
+00000760: 3600 3401 3601 3601 5951 5c5d 5151 635d  6.4.6.6.YQ\]QQc]
+00000770: 4841 1259 1029 101b 3402 4733 c232 02b2  HA.Y.)..4.G3.2..
+00000780: 1430 3600 1431 3600 1432 102e 3601 3401  .06..16..2..6.4.
+00000790: c5b5 142c 3600 5f4b 1530 02c3 c412 5a32  ...,6._K.0....Z2
+000007a0: 03b4 3401 3401 121a 132b b356 4229 515c  ..4.4....+.VB)Q\
+000007b0: 5d4a 0459 4a01 5d51 6304 8138 4108 495d  ]J.YJ.]Qc..8A.I]
+000007c0: 8061 2b00 b05f 4b0a c112 5fb1 3401 2f14  .a+.._K..._.4./.
+000007d0: 4234 6382 1869 0849 5d80 622b 00b0 5f4b  B4c..i.I].b+.._K
+000007e0: 1630 02c1 c210 4a14 26b1 104b 142f b236  .0....J.&..K./.6
+000007f0: 0136 022f 1442 2863 8250 5108 4c5d 8068  .6./.B(c.PQ.L].h
+00000800: 2c00 b05f 4b1d c1b1 1432 103f 3601 8155  ,.._K....2.?6..U
+00000810: 1432 104b 3601 b114 3210 3f36 0180 552f  .2.K6...2.?6..U/
+00000820: 1942 2163 8138 4108 495d 806a 2b00 b05f  .B!c.8A.I].j+.._
+00000830: 4b0a c112 5bb1 3401 2f14 4234 639d 54a0  K...[.4./.B4c.T.
+00000840: 125e 3380 7080 0728 2d26 4267 2023 2322  .^3.p..(-&Bg ##"
+00000850: 2d28 2832 572d 6e20 2d2c 2922 3228 2722  -((2W-n -,)"2('"
+00000860: 3a1f 6756 2229 2a34 574d 2727 6e20 2527  :.gV")*4WM''n %'
+00000870: 2712 1310 2434 0143 5523 0314 2612 1310  '...$4.CU#..&...
+00000880: 2434 0136 01c0 1216 b034 0159 b063 1216  $4.6.....4.Y.c..
+00000890: 2304 3401 5923 05c1 2c00 c248 3d12 4db1  #.4.Y#..,..H=.M.
+000008a0: 1034 5234 8201 3002 c3c2 b214 1810 3536  .4R4..0.......56
+000008b0: 01c4 b214 1810 3636 01c5 125b b214 1810  ......66...[....
+000008c0: 3736 0122 3cf7 3401 121a 1825 1212 101c  76."<.4....%....
+000008d0: 121a 1325 5234 0359 4a24 5712 57df 445d  ...%R4.YJ$W.W.D]
+000008e0: c649 1312 1523 0614 26b6 b236 0234 0159  .I...#..&..6.4.Y
+000008f0: 121a 132b 6351 51c6 2806 5d4a 015d 2c02  ...+cQQ.(.]J.],.
+00000900: 2a00 1038 622a 0010 3962 c7b4 51de 438a  *..8b*..9b..Q.C.
+00000910: 81b5 51de 4384 8123 0714 26b4 b536 02c1  ..Q.C..#..&..6..
+00000920: 485a 124d b110 3a22 8800 1034 5234 8401  HZ.M..:"...4R4..
+00000930: 3002 c3c2 b214 1810 3b36 01c8 1202 103c  0.......;6.....<
+00000940: 3401 c92c 02b9 143d b814 1810 3836 0136  4..,...=....86.6
+00000950: 0114 3e81 3601 1432 103f 3601 1038 62b9  ..>.6..2.?6..8b.
+00000960: 143d b814 1810 3936 0136 0114 3e81 3601  .=....96.6..>.6.
+00000970: 1432 103f 3601 1039 62c7 4a1f 5712 57df  .2.?6..9b.J.W.W.
+00000980: 4458 c649 0e12 1523 0814 26b6 b236 0234  DX.I...#..&..6.4
+00000990: 0159 5151 c628 065d 4a01 5d48 35b7 1440  .YQQ.(.]J.]H5..@
+000009a0: 3600 5f4b 2bca 3200 b7ba 5534 01b7 ba56  6._K+.2...U4...V
+000009b0: b7ba 5580 5855 125b 121a 1325 223c f734  ..U.XU.[...%"<.4
+000009c0: 01e5 5b56 125a b7ba 5534 01b7 ba56 4213  ..[V.Z..U4...VB.
+000009d0: 4a32 5712 57df 446b c649 2112 1523 0914  J2W.W.Dk.I!..#..
+000009e0: 26b6 b736 0234 0159 1227 101b 3401 5912  &..6.4.Y.'..4.Y.
+000009f0: 1623 0a34 0159 121a 132b 6351 51c6 2806  .#.4.Y...+cQQ.(.
+00000a00: 5d4a 015d b712 1a18 2b12 2710 2834 0159  ]J.]....+.'.(4.Y
+00000a10: 1216 230b 3401 59b7 6301 8138 4108 495d  ..#.4.Y.c..8A.I]
+00000a20: 809e 2b00 b05f 4b0a c112 5bb1 3401 2f14  ..+.._K...[.4./.
+00000a30: 4234 6387 10e1 011a 415c 80b1 6020 2328  B4c.....A\..` #(
+00000a40: 2823 2e1f 24b0 4448 120e 3400 121a 181f  (#..$.DH..4.....
+00000a50: 121a 131f 51de 4443 230c 6312 5b12 0e34  ....Q.DC#.c.[..4
+00000a60: 0012 1a13 1ff3 3401 c1b1 2285 a300 f6b1  ......4...".....
+00000a70: 2285 a300 f822 9c10 f6b1 223c f722 3cf8  "...."...."<."<.
+00000a80: b122 3cf8 2a04 3004 c2c3 c4c5 230d 1426  ."<.*.0.....#..&
+00000a90: 125b b234 0112 5bb3 3401 125b b434 0112  .[.4..[.4..[.4..
+00000aa0: 5bb5 3401 3604 63                        [.4.6.c
```

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/micrOS.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/micrOS.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/micrOSloader.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/micrOSloader.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.18.3/toolkit/workspace/precompiled/urequests.mpy` & `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/urequests.mpy`

 * *Files identical despite different names*

