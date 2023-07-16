# Comparing `tmp/plapperkasten-0.5.2.tar.gz` & `tmp/plapperkasten-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plapperkasten-0.5.2.tar", last modified: Wed Nov 30 20:34:39 2022, max compression
+gzip compressed data, was "plapperkasten-0.5.3.tar", last modified: Sun Jul 16 07:45:02 2023, max compression
```

## Comparing `plapperkasten-0.5.2.tar` & `plapperkasten-0.5.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2022-11-30 20:34:39.205026 plapperkasten-0.5.2/
--rw-r--r--   0 eike      (4202) wir       (4201)     1211 2022-08-28 08:46:06.000000 plapperkasten-0.5.2/LICENSE
--rw-r--r--   0 eike      (4202) wir       (4201)    10889 2022-11-30 20:34:39.204025 plapperkasten-0.5.2/PKG-INFO
--rw-r--r--   0 eike      (4202) wir       (4201)     9945 2022-11-17 15:09:40.000000 plapperkasten-0.5.2/README.md
--rw-r--r--   0 eike      (4202) wir       (4201)     2070 2022-11-30 20:04:27.000000 plapperkasten-0.5.2/pyproject.toml
--rw-r--r--   0 eike      (4202) wir       (4201)       38 2022-11-30 20:34:39.205026 plapperkasten-0.5.2/setup.cfg
-drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2022-11-30 20:34:39.169025 plapperkasten-0.5.2/src/
-drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2022-11-30 20:34:39.179025 plapperkasten-0.5.2/src/plapperkasten/
--rw-r--r--   0 eike      (4202) wir       (4201)        0 2022-08-28 08:46:06.000000 plapperkasten-0.5.2/src/plapperkasten/__init__.py
--rw-r--r--   0 eike      (4202) wir       (4201)    20455 2022-11-30 20:16:52.000000 plapperkasten-0.5.2/src/plapperkasten/config.py
--rw-r--r--   0 eike      (4202) wir       (4201)      978 2022-09-21 18:15:36.000000 plapperkasten-0.5.2/src/plapperkasten/event.py
--rw-r--r--   0 eike      (4202) wir       (4201)     3360 2022-09-21 18:19:25.000000 plapperkasten-0.5.2/src/plapperkasten/eventmap.py
--rw-r--r--   0 eike      (4202) wir       (4201)     7147 2022-09-21 18:19:27.000000 plapperkasten-0.5.2/src/plapperkasten/keymap.py
--rw-r--r--   0 eike      (4202) wir       (4201)    22064 2022-11-17 15:09:40.000000 plapperkasten-0.5.2/src/plapperkasten/plapperkasten.py
-drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2022-11-30 20:34:39.183025 plapperkasten-0.5.2/src/plapperkasten/plklogging/
--rw-r--r--   0 eike      (4202) wir       (4201)        0 2022-08-28 08:46:06.000000 plapperkasten-0.5.2/src/plapperkasten/plklogging/__init__.py
--rw-r--r--   0 eike      (4202) wir       (4201)     2706 2022-09-21 18:12:49.000000 plapperkasten-0.5.2/src/plapperkasten/plklogging/plklogging.py
--rw-r--r--   0 eike      (4202) wir       (4201)     6904 2022-09-21 18:19:53.000000 plapperkasten-0.5.2/src/plapperkasten/plugin.py
-drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2022-11-30 20:34:39.173025 plapperkasten-0.5.2/src/plapperkasten/plugins/
-drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2022-11-30 20:34:39.184025 plapperkasten-0.5.2/src/plapperkasten/plugins/autoshutdown/
--rw-r--r--   0 eike      (4202) wir       (4201)     2457 2022-09-21 18:19:55.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/autoshutdown/autoshutdown.py
--rw-r--r--   0 eike      (4202) wir       (4201)      164 2022-08-28 08:46:06.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/autoshutdown/config.yaml
-drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2022-11-30 20:34:39.185025 plapperkasten-0.5.2/src/plapperkasten/plugins/example/
--rw-r--r--   0 eike      (4202) wir       (4201)       88 2022-08-28 08:46:06.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/example/config.yaml
--rw-r--r--   0 eike      (4202) wir       (4201)     2634 2022-09-21 18:19:56.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/example/example.py
-drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2022-11-30 20:34:39.185025 plapperkasten-0.5.2/src/plapperkasten/plugins/inputdevinputevent/
--rw-r--r--   0 eike      (4202) wir       (4201)      136 2022-08-28 08:46:06.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/inputdevinputevent/config.yaml
--rw-r--r--   0 eike      (4202) wir       (4201)     3071 2022-09-21 18:19:58.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/inputdevinputevent/inputdevinputevent.py
-drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2022-11-30 20:34:39.186025 plapperkasten-0.5.2/src/plapperkasten/plugins/inputgpiod/
--rw-r--r--   0 eike      (4202) wir       (4201)      562 2022-11-30 20:24:08.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/inputgpiod/config.yaml
--rw-r--r--   0 eike      (4202) wir       (4201)     4498 2022-11-30 20:23:00.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/inputgpiod/inputgpiod.py
-drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2022-11-30 20:34:39.188025 plapperkasten-0.5.2/src/plapperkasten/plugins/mpdclient/
--rw-r--r--   0 eike      (4202) wir       (4201)        0 2022-08-28 08:53:06.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/mpdclient/__init__.py
--rw-r--r--   0 eike      (4202) wir       (4201)      478 2022-08-28 08:53:06.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/mpdclient/config.yaml
--rw-r--r--   0 eike      (4202) wir       (4201)    17633 2022-11-17 15:29:29.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/mpdclient/mpdclient.py
--rw-r--r--   0 eike      (4202) wir       (4201)     3771 2022-09-21 18:20:06.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/mpdclient/statusmap.py
-drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2022-11-30 20:34:39.189025 plapperkasten-0.5.2/src/plapperkasten/plugins/soundalsa/
--rw-r--r--   0 eike      (4202) wir       (4201)        0 2022-09-21 08:30:55.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundalsa/__init__.py
--rw-r--r--   0 eike      (4202) wir       (4201)      672 2022-09-29 09:00:57.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundalsa/config.yaml
--rw-r--r--   0 eike      (4202) wir       (4201)    11928 2022-09-29 11:19:08.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundalsa/soundalsa.py
--rw-r--r--   0 eike      (4202) wir       (4201)     3771 2022-09-21 18:20:09.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundalsa/statusmap.py
-drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2022-11-30 20:34:39.190025 plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/
--rw-r--r--   0 eike      (4202) wir       (4201)     1590 2022-09-28 06:29:59.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/config.yaml
--rw-r--r--   0 eike      (4202) wir       (4201)     4067 2022-09-28 06:30:32.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/soundeffects.py
-drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2022-11-30 20:34:39.203025 plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/
--rw-r--r--   0 eike      (4202) wir       (4201)   718926 2022-08-28 08:46:06.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/144319__fumiya112__decide.wav
--rw-r--r--   0 eike      (4202) wir       (4201)   171096 2022-08-28 08:46:06.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/273925__lemonjolly__hooray-yeah.wav
--rw-r--r--   0 eike      (4202) wir       (4201)    26902 2022-08-28 08:46:06.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/331381__qubodup__public-domain-jump-sound.wav
--rw-r--r--   0 eike      (4202) wir       (4201)  1324184 2022-08-28 08:46:06.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/411460__inspectorj__power-up-bright-a.wav
--rw-r--r--   0 eike      (4202) wir       (4201)   371014 2022-08-28 08:46:06.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/528867__eponn__beep-5.wav
--rw-r--r--   0 eike      (4202) wir       (4201)  1205512 2022-08-28 08:46:06.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/531510__eponn__correct-blips.wav
--rw-r--r--   0 eike      (4202) wir       (4201)   346926 2022-08-28 08:46:06.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/55001__stib__uh-oh.wav
--rw-r--r--   0 eike      (4202) wir       (4201)    20524 2022-09-28 06:26:13.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/560188__anthonychartier2020__beep-3.wav
--rw-r-----   0 eike      (4202) wir       (4201)      878 2022-09-28 06:29:02.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/attribution
-drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2022-11-30 20:34:39.204025 plapperkasten-0.5.2/src/plapperkasten/plugins/soundpwwp/
--rw-r--r--   0 eike      (4202) wir       (4201)        0 2022-10-06 22:45:53.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundpwwp/__init__.py
--rw-r--r--   0 eike      (4202) wir       (4201)      324 2022-10-06 22:45:53.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundpwwp/config.yaml
--rw-r--r--   0 eike      (4202) wir       (4201)    11129 2022-10-06 22:45:53.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundpwwp/soundpwwp.py
--rw-r--r--   0 eike      (4202) wir       (4201)     3771 2022-10-06 22:45:53.000000 plapperkasten-0.5.2/src/plapperkasten/plugins/soundpwwp/statusmap.py
-drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2022-11-30 20:34:39.204025 plapperkasten-0.5.2/src/plapperkasten/settings/
--rw-r--r--   0 eike      (4202) wir       (4201)      706 2022-11-17 15:09:40.000000 plapperkasten-0.5.2/src/plapperkasten/settings/config.yaml
--rw-r--r--   0 eike      (4202) wir       (4201)        0 2022-08-28 08:46:06.000000 plapperkasten-0.5.2/src/plapperkasten/settings/events.map
-drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2022-11-30 20:34:39.182025 plapperkasten-0.5.2/src/plapperkasten.egg-info/
--rw-r--r--   0 eike      (4202) wir       (4201)    10889 2022-11-30 20:34:38.000000 plapperkasten-0.5.2/src/plapperkasten.egg-info/PKG-INFO
--rw-r--r--   0 eike      (4202) wir       (4201)     2458 2022-11-30 20:34:39.000000 plapperkasten-0.5.2/src/plapperkasten.egg-info/SOURCES.txt
--rw-r--r--   0 eike      (4202) wir       (4201)        1 2022-11-30 20:34:38.000000 plapperkasten-0.5.2/src/plapperkasten.egg-info/dependency_links.txt
--rw-r--r--   0 eike      (4202) wir       (4201)       67 2022-11-30 20:34:38.000000 plapperkasten-0.5.2/src/plapperkasten.egg-info/entry_points.txt
--rw-r--r--   0 eike      (4202) wir       (4201)       78 2022-11-30 20:34:38.000000 plapperkasten-0.5.2/src/plapperkasten.egg-info/requires.txt
--rw-r--r--   0 eike      (4202) wir       (4201)       14 2022-11-30 20:34:38.000000 plapperkasten-0.5.2/src/plapperkasten.egg-info/top_level.txt
+drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2023-07-16 07:45:02.001808 plapperkasten-0.5.3/
+-rw-r--r--   0 eike      (4202) wir       (4201)     1211 2022-08-28 08:46:06.000000 plapperkasten-0.5.3/LICENSE
+-rw-r--r--   0 eike      (4202) wir       (4201)    10889 2023-07-16 07:45:02.001808 plapperkasten-0.5.3/PKG-INFO
+-rw-r--r--   0 eike      (4202) wir       (4201)     9945 2023-07-16 07:32:21.000000 plapperkasten-0.5.3/README.md
+-rw-r--r--   0 eike      (4202) wir       (4201)     2070 2023-07-16 07:32:21.000000 plapperkasten-0.5.3/pyproject.toml
+-rw-r--r--   0 eike      (4202) wir       (4201)       38 2023-07-16 07:45:02.002808 plapperkasten-0.5.3/setup.cfg
+drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2023-07-16 07:45:01.742801 plapperkasten-0.5.3/src/
+drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2023-07-16 07:45:01.772802 plapperkasten-0.5.3/src/plapperkasten/
+-rw-r--r--   0 eike      (4202) wir       (4201)        0 2022-08-28 08:46:06.000000 plapperkasten-0.5.3/src/plapperkasten/__init__.py
+-rw-r--r--   0 eike      (4202) wir       (4201)    20455 2023-07-16 07:32:21.000000 plapperkasten-0.5.3/src/plapperkasten/config.py
+-rw-r--r--   0 eike      (4202) wir       (4201)      978 2022-09-21 18:15:36.000000 plapperkasten-0.5.3/src/plapperkasten/event.py
+-rw-r--r--   0 eike      (4202) wir       (4201)     3360 2022-09-21 18:19:25.000000 plapperkasten-0.5.3/src/plapperkasten/eventmap.py
+-rw-r--r--   0 eike      (4202) wir       (4201)     7147 2022-09-21 18:19:27.000000 plapperkasten-0.5.3/src/plapperkasten/keymap.py
+-rw-r--r--   0 eike      (4202) wir       (4201)    22062 2023-07-16 07:32:21.000000 plapperkasten-0.5.3/src/plapperkasten/plapperkasten.py
+drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2023-07-16 07:45:01.773802 plapperkasten-0.5.3/src/plapperkasten/plklogging/
+-rw-r--r--   0 eike      (4202) wir       (4201)        0 2022-08-28 08:46:06.000000 plapperkasten-0.5.3/src/plapperkasten/plklogging/__init__.py
+-rw-r--r--   0 eike      (4202) wir       (4201)     2706 2022-09-21 18:12:49.000000 plapperkasten-0.5.3/src/plapperkasten/plklogging/plklogging.py
+-rw-r--r--   0 eike      (4202) wir       (4201)     6904 2022-09-21 18:19:53.000000 plapperkasten-0.5.3/src/plapperkasten/plugin.py
+drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2023-07-16 07:45:01.743801 plapperkasten-0.5.3/src/plapperkasten/plugins/
+drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2023-07-16 07:45:01.796803 plapperkasten-0.5.3/src/plapperkasten/plugins/autoshutdown/
+-rw-r--r--   0 eike      (4202) wir       (4201)     2457 2022-09-21 18:19:55.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/autoshutdown/autoshutdown.py
+-rw-r--r--   0 eike      (4202) wir       (4201)      164 2022-08-28 08:46:06.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/autoshutdown/config.yaml
+drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2023-07-16 07:45:01.809803 plapperkasten-0.5.3/src/plapperkasten/plugins/example/
+-rw-r--r--   0 eike      (4202) wir       (4201)       88 2022-08-28 08:46:06.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/example/config.yaml
+-rw-r--r--   0 eike      (4202) wir       (4201)     2634 2022-09-21 18:19:56.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/example/example.py
+drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2023-07-16 07:45:01.810803 plapperkasten-0.5.3/src/plapperkasten/plugins/inputdevinputevent/
+-rw-r--r--   0 eike      (4202) wir       (4201)      136 2022-08-28 08:46:06.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/inputdevinputevent/config.yaml
+-rw-r--r--   0 eike      (4202) wir       (4201)     3071 2022-09-21 18:19:58.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/inputdevinputevent/inputdevinputevent.py
+drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2023-07-16 07:45:01.819803 plapperkasten-0.5.3/src/plapperkasten/plugins/inputgpiod/
+-rw-r--r--   0 eike      (4202) wir       (4201)      562 2023-07-16 07:32:21.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/inputgpiod/config.yaml
+-rw-r--r--   0 eike      (4202) wir       (4201)     4498 2023-07-16 07:32:21.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/inputgpiod/inputgpiod.py
+drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2023-07-16 07:45:01.829804 plapperkasten-0.5.3/src/plapperkasten/plugins/mpdclient/
+-rw-r--r--   0 eike      (4202) wir       (4201)        0 2022-08-28 08:53:06.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/mpdclient/__init__.py
+-rw-r--r--   0 eike      (4202) wir       (4201)      478 2022-08-28 08:53:06.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/mpdclient/config.yaml
+-rw-r--r--   0 eike      (4202) wir       (4201)    19334 2023-07-16 07:32:21.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/mpdclient/mpdclient.py
+-rw-r--r--   0 eike      (4202) wir       (4201)     3771 2022-09-21 18:20:06.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/mpdclient/statusmap.py
+drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2023-07-16 07:45:01.860804 plapperkasten-0.5.3/src/plapperkasten/plugins/soundalsa/
+-rw-r--r--   0 eike      (4202) wir       (4201)        0 2022-09-21 08:30:55.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundalsa/__init__.py
+-rw-r--r--   0 eike      (4202) wir       (4201)      672 2022-09-29 09:00:57.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundalsa/config.yaml
+-rw-r--r--   0 eike      (4202) wir       (4201)    11928 2022-09-29 11:19:08.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundalsa/soundalsa.py
+-rw-r--r--   0 eike      (4202) wir       (4201)     3771 2022-09-21 18:20:09.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundalsa/statusmap.py
+drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2023-07-16 07:45:01.861804 plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/
+-rw-r--r--   0 eike      (4202) wir       (4201)     1590 2022-09-28 06:29:59.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/config.yaml
+-rw-r--r--   0 eike      (4202) wir       (4201)     4067 2022-09-28 06:30:32.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/soundeffects.py
+drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2023-07-16 07:45:01.978807 plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/
+-rw-r--r--   0 eike      (4202) wir       (4201)   718926 2022-08-28 08:46:06.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/144319__fumiya112__decide.wav
+-rw-r--r--   0 eike      (4202) wir       (4201)   171096 2022-08-28 08:46:06.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/273925__lemonjolly__hooray-yeah.wav
+-rw-r--r--   0 eike      (4202) wir       (4201)    26902 2022-08-28 08:46:06.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/331381__qubodup__public-domain-jump-sound.wav
+-rw-r--r--   0 eike      (4202) wir       (4201)  1324184 2022-08-28 08:46:06.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/411460__inspectorj__power-up-bright-a.wav
+-rw-r--r--   0 eike      (4202) wir       (4201)   371014 2022-08-28 08:46:06.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/528867__eponn__beep-5.wav
+-rw-r--r--   0 eike      (4202) wir       (4201)  1205512 2022-08-28 08:46:06.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/531510__eponn__correct-blips.wav
+-rw-r--r--   0 eike      (4202) wir       (4201)   346926 2022-08-28 08:46:06.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/55001__stib__uh-oh.wav
+-rw-r--r--   0 eike      (4202) wir       (4201)    20524 2022-09-28 06:26:13.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/560188__anthonychartier2020__beep-3.wav
+-rw-r-----   0 eike      (4202) wir       (4201)      878 2022-09-28 06:29:02.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/attribution
+drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2023-07-16 07:45:01.992808 plapperkasten-0.5.3/src/plapperkasten/plugins/soundpwwp/
+-rw-r--r--   0 eike      (4202) wir       (4201)        0 2022-10-06 22:45:53.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundpwwp/__init__.py
+-rw-r--r--   0 eike      (4202) wir       (4201)      324 2022-10-06 22:45:53.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundpwwp/config.yaml
+-rw-r--r--   0 eike      (4202) wir       (4201)    11129 2022-10-06 22:45:53.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundpwwp/soundpwwp.py
+-rw-r--r--   0 eike      (4202) wir       (4201)     3771 2022-10-06 22:45:53.000000 plapperkasten-0.5.3/src/plapperkasten/plugins/soundpwwp/statusmap.py
+drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2023-07-16 07:45:02.001808 plapperkasten-0.5.3/src/plapperkasten/settings/
+-rw-r--r--   0 eike      (4202) wir       (4201)      706 2023-07-16 07:32:21.000000 plapperkasten-0.5.3/src/plapperkasten/settings/config.yaml
+-rw-r--r--   0 eike      (4202) wir       (4201)        0 2022-08-28 08:46:06.000000 plapperkasten-0.5.3/src/plapperkasten/settings/events.map
+drwxr-xr-x   0 eike      (4202) wir       (4201)        0 2023-07-16 07:45:01.773802 plapperkasten-0.5.3/src/plapperkasten.egg-info/
+-rw-r--r--   0 eike      (4202) wir       (4201)    10889 2023-07-16 07:45:01.000000 plapperkasten-0.5.3/src/plapperkasten.egg-info/PKG-INFO
+-rw-r--r--   0 eike      (4202) wir       (4201)     2458 2023-07-16 07:45:01.000000 plapperkasten-0.5.3/src/plapperkasten.egg-info/SOURCES.txt
+-rw-r--r--   0 eike      (4202) wir       (4201)        1 2023-07-16 07:45:01.000000 plapperkasten-0.5.3/src/plapperkasten.egg-info/dependency_links.txt
+-rw-r--r--   0 eike      (4202) wir       (4201)       67 2023-07-16 07:45:01.000000 plapperkasten-0.5.3/src/plapperkasten.egg-info/entry_points.txt
+-rw-r--r--   0 eike      (4202) wir       (4201)       78 2023-07-16 07:45:01.000000 plapperkasten-0.5.3/src/plapperkasten.egg-info/requires.txt
+-rw-r--r--   0 eike      (4202) wir       (4201)       14 2023-07-16 07:45:01.000000 plapperkasten-0.5.3/src/plapperkasten.egg-info/top_level.txt
```

### Comparing `plapperkasten-0.5.2/LICENSE` & `plapperkasten-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/PKG-INFO` & `plapperkasten-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plapperkasten
-Version: 0.5.2
+Version: 0.5.3
 Author-email: Eike Kühn <eike.kuehn@pixelwoelkchen.de>
 Maintainer-email: Eike Kühn <eike.kuehn@pixelwoelkchen.de>
 Project-URL: homepage, https://github.com/randomchars42/plapperkasten
 Project-URL: documentation, https://github.com/randomchars42/plapperkasten
 Project-URL: source, https://github.com/randomchars42/plapperkasten
 Project-URL: tracker, https://github.com/randomchars42/plapperkasten/issues
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

### Comparing `plapperkasten-0.5.2/README.md` & `plapperkasten-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/pyproject.toml` & `plapperkasten-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'plapperkasten'
-version = '0.5.2'
+version = '0.5.3'
 description = ''
 readme = 'README.md'
 requires-python = '>=3.9'
 authors = [
 {name = 'Eike Kühn', email = 'eike.kuehn@pixelwoelkchen.de'},
 ]
 maintainers = [
```

### Comparing `plapperkasten-0.5.2/src/plapperkasten/config.py` & `plapperkasten-0.5.3/src/plapperkasten/config.py`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/event.py` & `plapperkasten-0.5.3/src/plapperkasten/event.py`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/eventmap.py` & `plapperkasten-0.5.3/src/plapperkasten/eventmap.py`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/keymap.py` & `plapperkasten-0.5.3/src/plapperkasten/keymap.py`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plapperkasten.py` & `plapperkasten-0.5.3/src/plapperkasten/plapperkasten.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,15 +501,15 @@
             thread_logger.handle(record)
 
     def process_event(self, event: plkevent.Event,
                       passthrough: list[str]) -> None:
         """Process incoming events.
 
         Events named 'raw' will be looked up in the event map. All other
-        events will be emitted if allowd by config.events.passthrough.
+        events will be emitted if allowed by config.events.passthrough.
 
         Args:
             event: The event to process.
             passthrough: List of events, that  wil be re-emitted if
                 they are recieved.
         """
         # events will be processed and reemitted
@@ -528,19 +528,19 @@
 
         if hasattr(self, 'on_' + event.name):
             # the way of the main process to respond to events
             # just check if an `on_EVENT` function is defined
             getattr(self, 'on_' + event.name)(*event.values, **event.params)
 
         if event.name in ('busy', 'idle'):
-            # those case are taken care of by `on_idle` and `on_busy` so
+            # those cases are taken care of by `on_idle` and `on_busy` so
             # return
             return
 
-        if new or not event.name in passthrough:
+        if new or event.name in passthrough:
             self.emit(event.name, *event.values, **event.params)
 
     def on_busy(self, *values: str, **params: str) -> None:
         # pylint: disable=unused-argument
         """Triggered if a plugin gets busy, increases the counter.
 
         Args:
```

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plklogging/plklogging.py` & `plapperkasten-0.5.3/src/plapperkasten/plklogging/plklogging.py`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugin.py` & `plapperkasten-0.5.3/src/plapperkasten/plugin.py`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/autoshutdown/autoshutdown.py` & `plapperkasten-0.5.3/src/plapperkasten/plugins/autoshutdown/autoshutdown.py`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/example/example.py` & `plapperkasten-0.5.3/src/plapperkasten/plugins/example/example.py`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/inputdevinputevent/inputdevinputevent.py` & `plapperkasten-0.5.3/src/plapperkasten/plugins/inputdevinputevent/inputdevinputevent.py`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/inputgpiod/config.yaml` & `plapperkasten-0.5.3/src/plapperkasten/plugins/inputgpiod/config.yaml`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/inputgpiod/inputgpiod.py` & `plapperkasten-0.5.3/src/plapperkasten/plugins/inputgpiod/inputgpiod.py`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/mpdclient/mpdclient.py` & `plapperkasten-0.5.3/src/plapperkasten/plugins/mpdclient/mpdclient.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,28 +57,58 @@
                                          default='localhost')
         self._port: int = config.get_int('plugins',
                                          'mpdclient',
                                          'port',
                                          default=6600)
 
         self._connected: bool = False
-        self._active: bool = False
         self._statusmap: statusmap.StatusMap = statusmap.StatusMap(config)
         self._status: statusmap.Status = statusmap.Status()
-        self._last_save: int = 0
-        self._last_check: int = 0
-        self._last_check_result: bool = False
+        self.reset_to_default()
 
         self.register_for('load_source')
         self.register_for('toggle')
         self.register_for('play')
         self.register_for('stop')
         self.register_for('next')
         self.register_for('previous')
 
+    def reset_to_default(self) -> None:
+        """Reset members to default, either on startup or on error."""
+        self._active: bool = False
+        self._last_save: int = 0
+        self._last_check: int = 0
+        self._last_check_result: bool = False
+
+    def on_error(self, message: str, stop: bool = True) -> None:
+        """Return to default state, log error and notify user.
+
+        Args:
+            message: message to log
+            stop: stop MPD? defaults to `True`
+        """
+        logger.error(message)
+        self.reset_to_default()
+        self.send_idle()
+        self.send_to_main("error")
+        if not stop:
+            return
+        try:
+            self._mpdclient.stop()
+            # do not diconnect as we might recover
+            #self._mpdclient.close()
+            #self._mpdclient.disconnect()
+        except:
+            logger.debug("could not stop")
+
+    def on_connection_error(self) -> None:
+        """Log event and mark as not connected."""
+
+        self.on_error('lost connection to MPD', False)
+
     def on_before_run(self) -> None:
         """Instantiate the MPD client.
 
         Do not do this in `on_init` as then the subprocess is not yet
         running and the object has to be copied into the process and
         havoc ensues in tidying up.
         """
@@ -87,20 +117,15 @@
         # the class is built using mixins and mypy cannot determine its member
         # functions
         self._mpdclient: Any = mpd.MPDClient()
         try:
             self._mpdclient.connect(self._host, self._port)
             self._connected = True
         except mpd.base.ConnectionError:
-            logger.error('could not connect to MPD')
-
-    def on_connection_error(self) -> None:
-        """Log event and mark as not connected."""
-        self._connected = False
-        logger.error('lost connection to MPD')
+            self.on_error('could not connect to MPD', False)
 
     def on_tick(self) -> None:
         """Called every `_tick_interval` [s] while the process runs.
 
         Use this function if you have to do anything at regular
         intervals.
 
@@ -132,35 +157,58 @@
 
         Args:
             values: Values attached to the event (ignored).
             params: Parameters attached to the event. Of those only
                 `use` and `key` are used.
         """
 
-        if not all(x in params for x in ('use', 'key')):
-            logger.error('malformed load_source event')
-            return
-        elif not params['use'] == self.get_name():
+        if not params['use'] == self.get_name():
             # event meant for another plugin
-            self._active = False
+            # we try to be nice and stop
+            # if we were already playing
+            if not self.check_mpd(save=False, force=False):
+                return
+
+            try:
+                self._mpdclient.stop()
+            except mpd.CommandError as error:
+                self.on_error('could not stop ("{error}")')
+                return
+            except mpd.base.ConnectionError:
+                self.on_connection_error()
+                return
+
+            # save position
+            self.check_mpd(save=True, force=True)
+            # and hand over
+            # we are not busy (anymore)
             self.send_idle()
+            # make `on_play()` etc. stop reacting to their events
+            # it's someone else's time to react (lod_source|for=someoneelse)
+            self._active = False
+            return
+
+        # we established that this event is meant for us so we check its
+        # integrity
+        if not all(x in params for x in ('use', 'key')):
+            self.on_error('malformed load_source event')
             return
 
         # create a playlist from the resource and play it
         status: statusmap.Status = self._statusmap.get_status(params['key'])
         if status.key == '':
             # empty status means that there's no entry with params['key'] as
             # key in the statusmap
             status.key = params['key']
         self.apply_status(status)
 
         try:
             self._mpdclient.play()
         except mpd.CommandError as error:
-            logger.error(f'could not start playing ("{error}")')
+            self.on_error(f'could not start playing ("{error}")')
             return
         except mpd.base.ConnectionError:
             self.on_connection_error()
             return
 
         # mark as active so that `on_play()`, `on_toggle()`, `on_stop()`,
         # `on_next()` and `on_prev()` react when called
@@ -202,15 +250,15 @@
             else:
                 # the key represents a path to a folder the files in which are
                 # to be coerced into a playlist
                 self._mpdclient.add(status.key)
 
             self._mpdclient.seek(status.position, status.elapsed)
         except mpd.CommandError as error:
-            logger.error(f'could not apply status ("{error}")')
+            self.on_error(f'could not apply status ("{error}")')
             return
         except mpd.base.ConnectionError:
             self.on_connection_error()
             return
         self._status = status
 
     def query_status(self) -> statusmap.Status:
@@ -248,15 +296,15 @@
 
     def is_current_playlist(self, key: str) -> bool:
         """Compares the playlist (or folder) with MPD playlist.
 
         There is no easy way to determine whether MPD's current
         playlist / queue is the same as has been loaded by
         `on_load_source()` as MPD. One needs to compare MPD's current
-        playlist with a hypthetical, expected playlist.
+        playlist with a hypothetical, expected playlist.
 
         In theory the queue should only be altered by another call to
         `on_load_source()` but as many clients could connect to MPD we
         make sure by checking if the current playlist matches what we
         expect.
 
         Args:
@@ -285,15 +333,15 @@
             else:
                 key_list = [
                     'file: ' + file['file']
                     for file in self._mpdclient.search('base', key)
                 ]
 
         except mpd.CommandError as error:
-            logger.error(f'could not compare playlists ("{error}")')
+            self.on_error(f'could not compare playlists ("{error}")')
             return False
         except mpd.base.ConnectionError:
             self.on_connection_error()
             return False
 
         return mpd_list == key_list
 
@@ -325,15 +373,15 @@
             logger.debug('no need for further checking')
             logger.debug('returning %s', self._last_check_result)
             return self._last_check_result
 
         self._last_check_result = False
 
         if not self._active:
-            # this function will might be called by a function triggered by a
+            # this function might be called by a function triggered by a
             # button (`on_next`, ...); this might hapen happen even if mpd is
             # not active in this case another plugin playing something might
             # be active
             logger.debug('not active')
             return False
 
         if not self._connected:
@@ -369,16 +417,18 @@
                      time.time() > self._last_save + self._save_min_interval):
             # save the status to file so the user may resume in the event of an
             # unexpected interruption, e.g., an empty battery
             logger.debug('saving status')
             self._statusmap.update_status(self._status)
 
         if self._status.state == 'play':
+            logger.debug('status: playing')
             self.send_busy()
         else:
+            logger.debug('status: idle')
             self.send_idle()
 
         logger.debug('finished checking mpd')
         return self._last_check_result
 
     def on_play(self, *values: str, **params: str) -> None:
         # pylint: disable=unused-argument
@@ -391,15 +441,15 @@
 
         if not self.check_mpd(save=False, force=False):
             return
 
         try:
             self._mpdclient.play('0')
         except mpd.CommandError as error:
-            logger.error(f'could not play ("{error}")')
+            self.on_error(f'could not play ("{error}")')
             return
         except mpd.base.ConnectionError:
             self.on_connection_error()
             return
 
         self.check_mpd(save=True, force=True)
 
@@ -423,15 +473,15 @@
             elif self._status.state == 'stop':
                 # edge case
                 # playlist stopped at end of list
                 self._mpdclient.play('0')
             else:
                 self._mpdclient.pause('0')
         except mpd.CommandError as error:
-            logger.error(f'could not toggle ("{error}")')
+            self.on_error(f'could not toggle ("{error}")')
             return
         except mpd.base.ConnectionError:
             self.on_connection_error()
             return
 
         self.check_mpd(save=True, force=True)
 
@@ -447,15 +497,15 @@
         if not self.check_mpd(save=False, force=False):
             return
 
         try:
             self._mpdclient.stop()
             self._mpdclient.seek('0', '0')
         except mpd.CommandError as error:
-            logger.error('could not stop ("{error}")')
+            self.on_error('could not stop ("{error}")')
             return
         except mpd.base.ConnectionError:
             self.on_connection_error()
             return
 
         self.check_mpd(save=True, force=True)
 
@@ -470,15 +520,15 @@
 
         if not self.check_mpd(save=False, force=False):
             return
 
         try:
             self._mpdclient.next()
         except mpd.CommandError as error:
-            logger.error(f'could not jump to next title ("{error}")')
+            self.on_error(f'could not jump to next title ("{error}")')
             return
         except mpd.base.ConnectionError:
             self.on_connection_error()
             return
 
         self.check_mpd(save=True, force=True)
 
@@ -493,15 +543,15 @@
 
         if not self.check_mpd(save=False, force=False):
             return
 
         try:
             self._mpdclient.previous()
         except mpd.CommandError as error:
-            logger.error('could not jump to previous title ("{error}")')
+            self.on_error('could not jump to previous title ("{error}")')
             return
         except mpd.base.ConnectionError:
             self.on_connection_error()
             return
 
         self.check_mpd(save=True, force=True)
```

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/mpdclient/statusmap.py` & `plapperkasten-0.5.3/src/plapperkasten/plugins/mpdclient/statusmap.py`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/soundalsa/config.yaml` & `plapperkasten-0.5.3/src/plapperkasten/plugins/soundalsa/config.yaml`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/soundalsa/soundalsa.py` & `plapperkasten-0.5.3/src/plapperkasten/plugins/soundalsa/soundalsa.py`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/soundalsa/statusmap.py` & `plapperkasten-0.5.3/src/plapperkasten/plugins/soundalsa/statusmap.py`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/config.yaml` & `plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/config.yaml`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/soundeffects.py` & `plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/soundeffects.py`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/144319__fumiya112__decide.wav` & `plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/144319__fumiya112__decide.wav`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/273925__lemonjolly__hooray-yeah.wav` & `plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/273925__lemonjolly__hooray-yeah.wav`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/331381__qubodup__public-domain-jump-sound.wav` & `plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/331381__qubodup__public-domain-jump-sound.wav`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/411460__inspectorj__power-up-bright-a.wav` & `plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/411460__inspectorj__power-up-bright-a.wav`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/528867__eponn__beep-5.wav` & `plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/528867__eponn__beep-5.wav`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/531510__eponn__correct-blips.wav` & `plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/531510__eponn__correct-blips.wav`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/55001__stib__uh-oh.wav` & `plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/55001__stib__uh-oh.wav`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/560188__anthonychartier2020__beep-3.wav` & `plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/560188__anthonychartier2020__beep-3.wav`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/soundeffects/sounds/attribution` & `plapperkasten-0.5.3/src/plapperkasten/plugins/soundeffects/sounds/attribution`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/soundpwwp/soundpwwp.py` & `plapperkasten-0.5.3/src/plapperkasten/plugins/soundpwwp/soundpwwp.py`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/plugins/soundpwwp/statusmap.py` & `plapperkasten-0.5.3/src/plapperkasten/plugins/soundpwwp/statusmap.py`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten/settings/config.yaml` & `plapperkasten-0.5.3/src/plapperkasten/settings/config.yaml`

 * *Files identical despite different names*

### Comparing `plapperkasten-0.5.2/src/plapperkasten.egg-info/PKG-INFO` & `plapperkasten-0.5.3/src/plapperkasten.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plapperkasten
-Version: 0.5.2
+Version: 0.5.3
 Author-email: Eike Kühn <eike.kuehn@pixelwoelkchen.de>
 Maintainer-email: Eike Kühn <eike.kuehn@pixelwoelkchen.de>
 Project-URL: homepage, https://github.com/randomchars42/plapperkasten
 Project-URL: documentation, https://github.com/randomchars42/plapperkasten
 Project-URL: source, https://github.com/randomchars42/plapperkasten
 Project-URL: tracker, https://github.com/randomchars42/plapperkasten/issues
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

### Comparing `plapperkasten-0.5.2/src/plapperkasten.egg-info/SOURCES.txt` & `plapperkasten-0.5.3/src/plapperkasten.egg-info/SOURCES.txt`

 * *Files identical despite different names*

