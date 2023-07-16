# Comparing `tmp/dimples-0.2.2.tar.gz` & `tmp/dimples-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimples-0.2.2.tar", last modified: Sun Jul  9 10:01:21 2023, max compression
+gzip compressed data, was "dist/dimples-0.2.3.tar", last modified: Sun Jul 16 05:36:59 2023, max compression
```

## Comparing `dimples-0.2.2.tar` & `dimples-0.2.3.tar`

### file list

```diff
@@ -1,135 +1,136 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2023-07-09 10:01:21.000000 dimples-0.2.2/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.2.2/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/
--rw-r--r--   0 moky       (501) staff       (20)     7179 2023-07-05 16:12:35.000000 dimples-0.2.2/dimples/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/client/
--rw-r--r--   0 moky       (501) staff       (20)     1966 2023-07-05 17:00:59.000000 dimples-0.2.2/dimples/client/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/client/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2117 2023-07-05 16:57:49.000000 dimples-0.2.2/dimples/client/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4460 2023-07-09 09:34:27.000000 dimples-0.2.2/dimples/client/cpu/grp_expel.py
--rw-r--r--   0 moky       (501) staff       (20)     4324 2023-07-09 09:34:17.000000 dimples-0.2.2/dimples/client/cpu/grp_invite.py
--rw-r--r--   0 moky       (501) staff       (20)     3807 2023-07-09 09:34:07.000000 dimples-0.2.2/dimples/client/cpu/grp_query.py
--rw-r--r--   0 moky       (501) staff       (20)     3959 2023-07-09 09:34:01.000000 dimples-0.2.2/dimples/client/cpu/grp_quit.py
--rw-r--r--   0 moky       (501) staff       (20)     7077 2023-07-09 09:33:49.000000 dimples-0.2.2/dimples/client/cpu/grp_reset.py
--rw-r--r--   0 moky       (501) staff       (20)     5150 2023-02-23 14:17:47.000000 dimples-0.2.2/dimples/client/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     3065 2023-07-09 09:15:32.000000 dimples-0.2.2/dimples/client/cpu/history.py
--rw-r--r--   0 moky       (501) staff       (20)     1869 2023-01-31 05:28:07.000000 dimples-0.2.2/dimples/client/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     1895 2023-06-09 16:41:36.000000 dimples-0.2.2/dimples/client/cpu/text.py
--rw-r--r--   0 moky       (501) staff       (20)    16324 2023-06-02 17:03:56.000000 dimples-0.2.2/dimples/client/group.py
--rw-r--r--   0 moky       (501) staff       (20)     9952 2023-07-05 17:01:39.000000 dimples-0.2.2/dimples/client/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/client/network/
--rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.2.2/dimples/client/network/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6258 2023-02-23 14:14:03.000000 dimples-0.2.2/dimples/client/network/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8302 2023-06-03 11:39:42.000000 dimples-0.2.2/dimples/client/network/state.py
--rw-r--r--   0 moky       (501) staff       (20)     9531 2023-01-31 05:28:07.000000 dimples-0.2.2/dimples/client/network/transition.py
--rw-r--r--   0 moky       (501) staff       (20)     6619 2023-06-12 13:22:46.000000 dimples-0.2.2/dimples/client/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     7022 2023-07-05 17:01:13.000000 dimples-0.2.2/dimples/client/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5521 2023-02-23 14:13:41.000000 dimples-0.2.2/dimples/client/terminal.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/common/
--rw-r--r--   0 moky       (501) staff       (20)     2213 2023-07-05 16:06:45.000000 dimples-0.2.2/dimples/common/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     5644 2023-06-19 15:11:53.000000 dimples-0.2.2/dimples/common/ans.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/common/dbi/
--rw-r--r--   0 moky       (501) staff       (20)     2324 2023-06-09 14:20:27.000000 dimples-0.2.2/dimples/common/dbi/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6396 2023-06-02 10:33:41.000000 dimples-0.2.2/dimples/common/dbi/account.py
--rw-r--r--   0 moky       (501) staff       (20)     2465 2023-06-02 07:39:55.000000 dimples-0.2.2/dimples/common/dbi/message.py
--rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.2.2/dimples/common/dbi/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6739 2023-06-02 09:05:19.000000 dimples-0.2.2/dimples/common/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     7827 2023-06-12 14:51:01.000000 dimples-0.2.2/dimples/common/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     7710 2023-06-12 13:20:42.000000 dimples-0.2.2/dimples/common/packer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/common/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     2354 2023-07-05 16:06:45.000000 dimples-0.2.2/dimples/common/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3321 2023-06-09 16:01:10.000000 dimples-0.2.2/dimples/common/protocol/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     5004 2022-12-23 07:24:37.000000 dimples-0.2.2/dimples/common/protocol/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4523 2023-06-02 08:11:42.000000 dimples-0.2.2/dimples/common/protocol/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2521 2023-06-02 08:42:45.000000 dimples-0.2.2/dimples/common/protocol/report.py
--rw-r--r--   0 moky       (501) staff       (20)     4486 2023-06-04 16:41:38.000000 dimples-0.2.2/dimples/common/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6211 2023-06-03 12:24:47.000000 dimples-0.2.2/dimples/config.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/conn/
--rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.2.2/dimples/conn/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10335 2023-06-07 13:23:28.000000 dimples-0.2.2/dimples/conn/gate.py
--rw-r--r--   0 moky       (501) staff       (20)     9892 2023-01-31 05:28:07.000000 dimples-0.2.2/dimples/conn/gatekeeper.py
--rw-r--r--   0 moky       (501) staff       (20)    10305 2023-01-14 13:25:42.000000 dimples-0.2.2/dimples/conn/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     7851 2023-02-23 09:10:59.000000 dimples-0.2.2/dimples/conn/mtp.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/conn/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/conn/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/conn/protocol/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     8254 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/conn/protocol/ws.py
--rw-r--r--   0 moky       (501) staff       (20)     5411 2023-02-23 09:10:59.000000 dimples-0.2.2/dimples/conn/queue.py
--rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.2.2/dimples/conn/seeker.py
--rw-r--r--   0 moky       (501) staff       (20)     5726 2023-06-02 09:57:33.000000 dimples-0.2.2/dimples/conn/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6991 2023-01-14 12:47:37.000000 dimples-0.2.2/dimples/conn/ws.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/database/
--rw-r--r--   0 moky       (501) staff       (20)     2560 2023-06-04 16:46:57.000000 dimples-0.2.2/dimples/database/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7085 2023-06-19 07:42:03.000000 dimples-0.2.2/dimples/database/account.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/database/dos/
--rw-r--r--   0 moky       (501) staff       (20)     1808 2023-06-05 05:13:02.000000 dimples-0.2.2/dimples/database/dos/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4071 2022-12-22 17:59:17.000000 dimples-0.2.2/dimples/database/dos/base.py
--rw-r--r--   0 moky       (501) staff       (20)     3769 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/database/dos/document.py
--rw-r--r--   0 moky       (501) staff       (20)     4232 2023-06-02 10:30:44.000000 dimples-0.2.2/dimples/database/dos/group.py
--rw-r--r--   0 moky       (501) staff       (20)     3141 2023-06-02 11:02:33.000000 dimples-0.2.2/dimples/database/dos/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2680 2022-12-22 17:58:13.000000 dimples-0.2.2/dimples/database/dos/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5630 2023-06-02 11:04:20.000000 dimples-0.2.2/dimples/database/dos/private.py
--rw-r--r--   0 moky       (501) staff       (20)     8033 2023-06-09 14:40:24.000000 dimples-0.2.2/dimples/database/dos/station.py
--rw-r--r--   0 moky       (501) staff       (20)     5625 2023-06-02 11:01:02.000000 dimples-0.2.2/dimples/database/dos/user.py
--rw-r--r--   0 moky       (501) staff       (20)     3097 2022-12-13 10:56:52.000000 dimples-0.2.2/dimples/database/message.py
--rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.2.2/dimples/database/session.py
--rw-r--r--   0 moky       (501) staff       (20)     2972 2023-01-31 05:28:07.000000 dimples-0.2.2/dimples/database/t_cipherkey.py
--rw-r--r--   0 moky       (501) staff       (20)     3710 2023-06-09 14:19:20.000000 dimples-0.2.2/dimples/database/t_document.py
--rw-r--r--   0 moky       (501) staff       (20)     7715 2023-06-05 05:41:56.000000 dimples-0.2.2/dimples/database/t_group.py
--rw-r--r--   0 moky       (501) staff       (20)     3718 2023-06-09 14:19:56.000000 dimples-0.2.2/dimples/database/t_login.py
--rw-r--r--   0 moky       (501) staff       (20)     5144 2022-12-22 18:03:37.000000 dimples-0.2.2/dimples/database/t_message.py
--rw-r--r--   0 moky       (501) staff       (20)     3513 2023-06-05 05:36:10.000000 dimples-0.2.2/dimples/database/t_meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5589 2023-06-05 05:38:08.000000 dimples-0.2.2/dimples/database/t_private.py
--rw-r--r--   0 moky       (501) staff       (20)     6647 2023-06-05 05:31:39.000000 dimples-0.2.2/dimples/database/t_station.py
--rw-r--r--   0 moky       (501) staff       (20)     6455 2023-06-05 05:39:18.000000 dimples-0.2.2/dimples/database/t_user.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/edge/
--rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/edge/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    13567 2023-06-12 14:07:59.000000 dimples-0.2.2/dimples/edge/octopus.py
--rw-r--r--   0 moky       (501) staff       (20)     5929 2023-06-19 07:20:16.000000 dimples-0.2.2/dimples/edge/shared.py
--rw-r--r--   0 moky       (501) staff       (20)     2726 2023-06-04 10:23:09.000000 dimples-0.2.2/dimples/edge/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/register/
--rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/register/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     9516 2023-06-02 10:01:29.000000 dimples-0.2.2/dimples/register/generate.py
--rw-r--r--   0 moky       (501) staff       (20)     7045 2023-06-02 10:02:10.000000 dimples-0.2.2/dimples/register/modify.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3880 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/register/run.py
--rw-r--r--   0 moky       (501) staff       (20)     1971 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/register/shared.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/server/
--rw-r--r--   0 moky       (501) staff       (20)     2654 2023-07-05 16:58:00.000000 dimples-0.2.2/dimples/server/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8020 2023-06-18 10:50:18.000000 dimples-0.2.2/dimples/server/broadcast.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/server/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-0.2.2/dimples/server/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2640 2023-07-09 09:36:32.000000 dimples-0.2.2/dimples/server/cpu/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     4781 2023-06-19 07:56:29.000000 dimples-0.2.2/dimples/server/cpu/document.py
--rw-r--r--   0 moky       (501) staff       (20)     3622 2023-07-09 09:09:31.000000 dimples-0.2.2/dimples/server/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4021 2023-07-09 09:04:04.000000 dimples-0.2.2/dimples/server/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     3369 2023-07-09 09:09:31.000000 dimples-0.2.2/dimples/server/cpu/report.py
--rw-r--r--   0 moky       (501) staff       (20)    13524 2023-07-05 17:00:59.000000 dimples-0.2.2/dimples/server/dispatcher.py
--rw-r--r--   0 moky       (501) staff       (20)     9473 2023-06-18 09:35:15.000000 dimples-0.2.2/dimples/server/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     6638 2023-06-18 11:45:32.000000 dimples-0.2.2/dimples/server/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     5619 2023-07-09 09:40:25.000000 dimples-0.2.2/dimples/server/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5448 2023-06-18 14:36:35.000000 dimples-0.2.2/dimples/server/push.py
--rw-r--r--   0 moky       (501) staff       (20)     8005 2023-07-09 09:47:11.000000 dimples-0.2.2/dimples/server/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/server/session_center.py
--rw-r--r--   0 moky       (501) staff       (20)     9722 2023-06-26 11:02:55.000000 dimples-0.2.2/dimples/server/trace.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/station/
--rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.2.2/dimples/station/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4624 2023-06-07 12:21:10.000000 dimples-0.2.2/dimples/station/handler.py
--rw-r--r--   0 moky       (501) staff       (20)     6424 2023-06-19 07:20:09.000000 dimples-0.2.2/dimples/station/shared.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3708 2023-06-18 11:31:20.000000 dimples-0.2.2/dimples/station/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/utils/
--rw-r--r--   0 moky       (501) staff       (20)     2568 2023-02-23 13:38:40.000000 dimples-0.2.2/dimples/utils/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6446 2023-06-18 10:21:27.000000 dimples-0.2.2/dimples/utils/cache.py
--rw-r--r--   0 moky       (501) staff       (20)     4016 2023-06-02 18:00:31.000000 dimples-0.2.2/dimples/utils/checker.py
--rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/utils/dos.py
--rw-r--r--   0 moky       (501) staff       (20)     2805 2022-12-28 05:23:15.000000 dimples-0.2.2/dimples/utils/log.py
--rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/utils/singleton.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     3170 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)      118 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples.egg-info/entry_points.txt
--rw-r--r--   0 moky       (501) staff       (20)      108 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        8 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2023-07-09 10:01:21.000000 dimples-0.2.2/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1675 2023-07-09 09:00:39.000000 dimples-0.2.2/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2023-07-16 05:36:59.000000 dimples-0.2.3/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.2.3/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples/
+-rw-r--r--   0 moky       (501) staff       (20)     7179 2023-07-05 16:12:35.000000 dimples-0.2.3/dimples/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples/client/
+-rw-r--r--   0 moky       (501) staff       (20)     2019 2023-07-16 04:40:55.000000 dimples-0.2.3/dimples/client/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3447 2023-07-16 04:41:51.000000 dimples-0.2.3/dimples/client/checkpoint.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples/client/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2117 2023-07-05 16:57:49.000000 dimples-0.2.3/dimples/client/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4460 2023-07-09 09:34:27.000000 dimples-0.2.3/dimples/client/cpu/grp_expel.py
+-rw-r--r--   0 moky       (501) staff       (20)     4324 2023-07-09 09:34:17.000000 dimples-0.2.3/dimples/client/cpu/grp_invite.py
+-rw-r--r--   0 moky       (501) staff       (20)     3807 2023-07-09 09:34:07.000000 dimples-0.2.3/dimples/client/cpu/grp_query.py
+-rw-r--r--   0 moky       (501) staff       (20)     3959 2023-07-09 09:34:01.000000 dimples-0.2.3/dimples/client/cpu/grp_quit.py
+-rw-r--r--   0 moky       (501) staff       (20)     7077 2023-07-09 09:33:49.000000 dimples-0.2.3/dimples/client/cpu/grp_reset.py
+-rw-r--r--   0 moky       (501) staff       (20)     5150 2023-02-23 14:17:47.000000 dimples-0.2.3/dimples/client/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     3065 2023-07-09 09:15:32.000000 dimples-0.2.3/dimples/client/cpu/history.py
+-rw-r--r--   0 moky       (501) staff       (20)     1869 2023-01-31 05:28:07.000000 dimples-0.2.3/dimples/client/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     1895 2023-06-09 16:41:36.000000 dimples-0.2.3/dimples/client/cpu/text.py
+-rw-r--r--   0 moky       (501) staff       (20)    16324 2023-06-02 17:03:56.000000 dimples-0.2.3/dimples/client/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     9952 2023-07-05 17:01:39.000000 dimples-0.2.3/dimples/client/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples/client/network/
+-rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.2.3/dimples/client/network/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6258 2023-02-23 14:14:03.000000 dimples-0.2.3/dimples/client/network/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8302 2023-06-03 11:39:42.000000 dimples-0.2.3/dimples/client/network/state.py
+-rw-r--r--   0 moky       (501) staff       (20)     9531 2023-01-31 05:28:07.000000 dimples-0.2.3/dimples/client/network/transition.py
+-rw-r--r--   0 moky       (501) staff       (20)     7248 2023-07-16 05:13:19.000000 dimples-0.2.3/dimples/client/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     7022 2023-07-05 17:01:13.000000 dimples-0.2.3/dimples/client/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5521 2023-02-23 14:13:41.000000 dimples-0.2.3/dimples/client/terminal.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples/common/
+-rw-r--r--   0 moky       (501) staff       (20)     2213 2023-07-05 16:06:45.000000 dimples-0.2.3/dimples/common/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     5737 2023-07-12 08:17:31.000000 dimples-0.2.3/dimples/common/ans.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples/common/dbi/
+-rw-r--r--   0 moky       (501) staff       (20)     2324 2023-06-09 14:20:27.000000 dimples-0.2.3/dimples/common/dbi/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6396 2023-06-02 10:33:41.000000 dimples-0.2.3/dimples/common/dbi/account.py
+-rw-r--r--   0 moky       (501) staff       (20)     2465 2023-06-02 07:39:55.000000 dimples-0.2.3/dimples/common/dbi/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.2.3/dimples/common/dbi/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6739 2023-06-02 09:05:19.000000 dimples-0.2.3/dimples/common/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     7827 2023-06-12 14:51:01.000000 dimples-0.2.3/dimples/common/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     7710 2023-06-12 13:20:42.000000 dimples-0.2.3/dimples/common/packer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples/common/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     2354 2023-07-05 16:06:45.000000 dimples-0.2.3/dimples/common/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3321 2023-06-09 16:01:10.000000 dimples-0.2.3/dimples/common/protocol/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     5004 2022-12-23 07:24:37.000000 dimples-0.2.3/dimples/common/protocol/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4523 2023-06-02 08:11:42.000000 dimples-0.2.3/dimples/common/protocol/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2521 2023-06-02 08:42:45.000000 dimples-0.2.3/dimples/common/protocol/report.py
+-rw-r--r--   0 moky       (501) staff       (20)     4494 2023-07-13 17:06:03.000000 dimples-0.2.3/dimples/common/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6211 2023-06-03 12:24:47.000000 dimples-0.2.3/dimples/config.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples/conn/
+-rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.2.3/dimples/conn/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10335 2023-06-07 13:23:28.000000 dimples-0.2.3/dimples/conn/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)     9892 2023-01-31 05:28:07.000000 dimples-0.2.3/dimples/conn/gatekeeper.py
+-rw-r--r--   0 moky       (501) staff       (20)    10305 2023-01-14 13:25:42.000000 dimples-0.2.3/dimples/conn/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     7851 2023-02-23 09:10:59.000000 dimples-0.2.3/dimples/conn/mtp.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples/conn/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.2.3/dimples/conn/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.2.3/dimples/conn/protocol/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8254 2022-12-11 05:07:49.000000 dimples-0.2.3/dimples/conn/protocol/ws.py
+-rw-r--r--   0 moky       (501) staff       (20)     5411 2023-02-23 09:10:59.000000 dimples-0.2.3/dimples/conn/queue.py
+-rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.2.3/dimples/conn/seeker.py
+-rw-r--r--   0 moky       (501) staff       (20)     5726 2023-06-02 09:57:33.000000 dimples-0.2.3/dimples/conn/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6991 2023-01-14 12:47:37.000000 dimples-0.2.3/dimples/conn/ws.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples/database/
+-rw-r--r--   0 moky       (501) staff       (20)     2560 2023-06-04 16:46:57.000000 dimples-0.2.3/dimples/database/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7085 2023-06-19 07:42:03.000000 dimples-0.2.3/dimples/database/account.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples/database/dos/
+-rw-r--r--   0 moky       (501) staff       (20)     1808 2023-06-05 05:13:02.000000 dimples-0.2.3/dimples/database/dos/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4071 2022-12-22 17:59:17.000000 dimples-0.2.3/dimples/database/dos/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     3769 2022-12-11 05:07:49.000000 dimples-0.2.3/dimples/database/dos/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     4232 2023-06-02 10:30:44.000000 dimples-0.2.3/dimples/database/dos/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     3141 2023-06-02 11:02:33.000000 dimples-0.2.3/dimples/database/dos/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2680 2022-12-22 17:58:13.000000 dimples-0.2.3/dimples/database/dos/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5630 2023-06-02 11:04:20.000000 dimples-0.2.3/dimples/database/dos/private.py
+-rw-r--r--   0 moky       (501) staff       (20)     8033 2023-06-09 14:40:24.000000 dimples-0.2.3/dimples/database/dos/station.py
+-rw-r--r--   0 moky       (501) staff       (20)     5625 2023-06-02 11:01:02.000000 dimples-0.2.3/dimples/database/dos/user.py
+-rw-r--r--   0 moky       (501) staff       (20)     3097 2022-12-13 10:56:52.000000 dimples-0.2.3/dimples/database/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.2.3/dimples/database/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     2972 2023-01-31 05:28:07.000000 dimples-0.2.3/dimples/database/t_cipherkey.py
+-rw-r--r--   0 moky       (501) staff       (20)     3710 2023-06-09 14:19:20.000000 dimples-0.2.3/dimples/database/t_document.py
+-rw-r--r--   0 moky       (501) staff       (20)     7715 2023-06-05 05:41:56.000000 dimples-0.2.3/dimples/database/t_group.py
+-rw-r--r--   0 moky       (501) staff       (20)     3718 2023-06-09 14:19:56.000000 dimples-0.2.3/dimples/database/t_login.py
+-rw-r--r--   0 moky       (501) staff       (20)     5144 2022-12-22 18:03:37.000000 dimples-0.2.3/dimples/database/t_message.py
+-rw-r--r--   0 moky       (501) staff       (20)     3513 2023-06-05 05:36:10.000000 dimples-0.2.3/dimples/database/t_meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5589 2023-06-05 05:38:08.000000 dimples-0.2.3/dimples/database/t_private.py
+-rw-r--r--   0 moky       (501) staff       (20)     6647 2023-06-05 05:31:39.000000 dimples-0.2.3/dimples/database/t_station.py
+-rw-r--r--   0 moky       (501) staff       (20)     6455 2023-06-05 05:39:18.000000 dimples-0.2.3/dimples/database/t_user.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples/edge/
+-rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.2.3/dimples/edge/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    13567 2023-06-12 14:07:59.000000 dimples-0.2.3/dimples/edge/octopus.py
+-rw-r--r--   0 moky       (501) staff       (20)     5929 2023-06-19 07:20:16.000000 dimples-0.2.3/dimples/edge/shared.py
+-rw-r--r--   0 moky       (501) staff       (20)     2726 2023-06-04 10:23:09.000000 dimples-0.2.3/dimples/edge/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples/register/
+-rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.2.3/dimples/register/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     9516 2023-06-02 10:01:29.000000 dimples-0.2.3/dimples/register/generate.py
+-rw-r--r--   0 moky       (501) staff       (20)     7045 2023-06-02 10:02:10.000000 dimples-0.2.3/dimples/register/modify.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3880 2022-12-11 05:07:49.000000 dimples-0.2.3/dimples/register/run.py
+-rw-r--r--   0 moky       (501) staff       (20)     1971 2022-12-11 05:07:49.000000 dimples-0.2.3/dimples/register/shared.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples/server/
+-rw-r--r--   0 moky       (501) staff       (20)     2654 2023-07-05 16:58:00.000000 dimples-0.2.3/dimples/server/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8026 2023-07-12 08:49:16.000000 dimples-0.2.3/dimples/server/broadcast.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples/server/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-0.2.3/dimples/server/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2640 2023-07-09 09:36:32.000000 dimples-0.2.3/dimples/server/cpu/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     4781 2023-06-19 07:56:29.000000 dimples-0.2.3/dimples/server/cpu/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     3677 2023-07-09 12:26:02.000000 dimples-0.2.3/dimples/server/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4021 2023-07-09 09:04:04.000000 dimples-0.2.3/dimples/server/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     3369 2023-07-09 09:09:31.000000 dimples-0.2.3/dimples/server/cpu/report.py
+-rw-r--r--   0 moky       (501) staff       (20)    13524 2023-07-05 17:00:59.000000 dimples-0.2.3/dimples/server/dispatcher.py
+-rw-r--r--   0 moky       (501) staff       (20)     9479 2023-07-12 08:49:05.000000 dimples-0.2.3/dimples/server/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     6638 2023-06-18 11:45:32.000000 dimples-0.2.3/dimples/server/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     5619 2023-07-09 09:40:25.000000 dimples-0.2.3/dimples/server/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5448 2023-06-18 14:36:35.000000 dimples-0.2.3/dimples/server/push.py
+-rw-r--r--   0 moky       (501) staff       (20)     8013 2023-07-13 17:00:36.000000 dimples-0.2.3/dimples/server/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.2.3/dimples/server/session_center.py
+-rw-r--r--   0 moky       (501) staff       (20)     9722 2023-06-26 11:02:55.000000 dimples-0.2.3/dimples/server/trace.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples/station/
+-rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.2.3/dimples/station/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4624 2023-06-07 12:21:10.000000 dimples-0.2.3/dimples/station/handler.py
+-rw-r--r--   0 moky       (501) staff       (20)     6424 2023-06-19 07:20:09.000000 dimples-0.2.3/dimples/station/shared.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3708 2023-06-18 11:31:20.000000 dimples-0.2.3/dimples/station/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples/utils/
+-rw-r--r--   0 moky       (501) staff       (20)     2568 2023-02-23 13:38:40.000000 dimples-0.2.3/dimples/utils/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6446 2023-06-18 10:21:27.000000 dimples-0.2.3/dimples/utils/cache.py
+-rw-r--r--   0 moky       (501) staff       (20)     4016 2023-06-02 18:00:31.000000 dimples-0.2.3/dimples/utils/checker.py
+-rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.2.3/dimples/utils/dos.py
+-rw-r--r--   0 moky       (501) staff       (20)     2805 2022-12-28 05:23:15.000000 dimples-0.2.3/dimples/utils/log.py
+-rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.2.3/dimples/utils/singleton.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     3199 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)      118 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples.egg-info/entry_points.txt
+-rw-r--r--   0 moky       (501) staff       (20)      108 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        8 2023-07-16 05:36:59.000000 dimples-0.2.3/dimples.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2023-07-16 05:36:59.000000 dimples-0.2.3/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1675 2023-07-12 08:54:59.000000 dimples-0.2.3/setup.py
```

### Comparing `dimples-0.2.2/PKG-INFO` & `dimples-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.2.2
+Version: 0.2.3
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.2.2/README.md` & `dimples-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/__init__.py` & `dimples-0.2.3/dimples/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/__init__.py` & `dimples-0.2.3/dimples/client/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from .network import SessionState
 
 from .group import GroupManager
 from .messenger import ClientMessenger
 from .packer import ClientMessagePacker
 from .processor import ClientMessageProcessor, ClientContentProcessorCreator
 from .terminal import Terminal
+from .checkpoint import Checkpoint
 
 
 __all__ = [
 
     #
     #   CPU
     #
@@ -55,8 +56,9 @@
     'ClientSession', 'SessionState',
 
     'GroupManager',
     'ClientMessenger',
     'ClientMessagePacker',
     'ClientMessageProcessor', 'ClientContentProcessorCreator',
     'Terminal',
+    'Checkpoint',
 ]
```

### Comparing `dimples-0.2.2/dimples/client/cpu/__init__.py` & `dimples-0.2.3/dimples/client/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/cpu/grp_expel.py` & `dimples-0.2.3/dimples/client/cpu/grp_expel.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/cpu/grp_invite.py` & `dimples-0.2.3/dimples/client/cpu/grp_invite.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/cpu/grp_query.py` & `dimples-0.2.3/dimples/client/cpu/grp_query.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/cpu/grp_quit.py` & `dimples-0.2.3/dimples/client/cpu/grp_quit.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/cpu/grp_reset.py` & `dimples-0.2.3/dimples/client/cpu/grp_reset.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/cpu/handshake.py` & `dimples-0.2.3/dimples/client/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/cpu/history.py` & `dimples-0.2.3/dimples/client/cpu/history.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/cpu/login.py` & `dimples-0.2.3/dimples/client/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/cpu/text.py` & `dimples-0.2.3/dimples/client/cpu/text.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/group.py` & `dimples-0.2.3/dimples/client/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/messenger.py` & `dimples-0.2.3/dimples/client/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/network/__init__.py` & `dimples-0.2.3/dimples/client/network/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/network/session.py` & `dimples-0.2.3/dimples/client/network/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/network/state.py` & `dimples-0.2.3/dimples/client/network/state.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/network/transition.py` & `dimples-0.2.3/dimples/client/network/transition.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/packer.py` & `dimples-0.2.3/dimples/client/packer.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,17 @@
 from dimsdk import SymmetricKey
 from dimsdk import ID
 from dimsdk import InstantMessage, SecureMessage, ReliableMessage
 from dimsdk import DocumentCommand
 from dimsdk import Messenger
 
 from ..utils import base64_encode, sha256
+from ..conn.session import get_sig
 from ..common import CommonFacebook, CommonMessagePacker
+from .checkpoint import Checkpoint
 
 
 class ClientMessagePacker(CommonMessagePacker):
 
     # Override
     def _check_instant_message_receiver(self, msg: InstantMessage) -> bool:
         receiver = msg.receiver
@@ -81,14 +83,27 @@
         return super()._check_instant_message_receiver(msg=msg)
 
     # Override
     def serialize_message(self, msg: ReliableMessage) -> bytes:
         attach_key_digest(msg=msg, messenger=self.messenger)
         return super().serialize_message(msg=msg)
 
+    # Override
+    def deserialize_message(self, data: bytes) -> Optional[ReliableMessage]:
+        msg = super().deserialize_message(data=data)
+        if msg is not None and self._message_duplicated(msg=msg):
+            msg = None
+        return msg
+
+    def _message_duplicated(self, msg: ReliableMessage) -> bool:
+        if g_checkpoint.duplicated(msg=msg):
+            sig = get_sig(msg=msg)
+            self.warning(msg='drop duplicated message (%s): %s -> %s' % (sig, msg.sender, msg.receiver))
+            return True
+
     # # Override
     # def encrypt_message(self, msg: InstantMessage) -> Optional[SecureMessage]:
     #     # make sure visa.key exists before encrypting message
     #     s_msg = super().encrypt_message(msg=msg)
     #     receiver = msg.receiver
     #     if receiver.is_group:
     #         # reuse group message keys
@@ -169,7 +184,10 @@
     # get digest for the last 6 bytes of key.data
     pos = len(data) - 6
     digest = sha256(data[pos:])
     base64 = base64_encode(digest)
     # get last 8 chars as key digest
     pos = len(base64) - 8
     return base64[pos:]
+
+
+g_checkpoint = Checkpoint()
```

### Comparing `dimples-0.2.2/dimples/client/processor.py` & `dimples-0.2.3/dimples/client/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/client/terminal.py` & `dimples-0.2.3/dimples/client/terminal.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/common/__init__.py` & `dimples-0.2.3/dimples/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/common/ans.py` & `dimples-0.2.3/dimples/common/ans.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,34 +105,36 @@
         if self.cache(name=name, identifier=identifier):
             # TODO: save new record into database
             return True
 
     def fix(self, records: Dict[str, str]) -> int:
         """ remove the keywords temporary before save new records """
         count = 0
-        self.__reserved['apns'] = False
+        # self.__reserved['apns'] = False
         self.__reserved['master'] = False
         self.__reserved['monitor'] = False
         self.__reserved['archivist'] = False
+        self.__reserved['announcer'] = False
         self.__reserved['assistant'] = False
         # self.__reserved['station'] = False
         for alias in records:
             value = records[alias]
             if value is None or len(value) == 0:
                 continue
             identifier = ID.parse(identifier=value)
             assert identifier is not None, 'record error: %s => %s' % (alias, value)
             if self.save(name=alias, identifier=identifier):
                 count += 1
         # self.__reserved['station'] = True
         self.__reserved['assistant'] = True
+        self.__reserved['announcer'] = True
         self.__reserved['archivist'] = True
         self.__reserved['monitor'] = True
         self.__reserved['master'] = True
-        self.__reserved['apns'] = True
+        # self.__reserved['apns'] = True
         return count
 
 
 class ANSFactory(IDFactory):
 
     def __init__(self, factory: IDFactory, ans: AddressNameServer):
         super().__init__()
```

### Comparing `dimples-0.2.2/dimples/common/dbi/__init__.py` & `dimples-0.2.3/dimples/common/dbi/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/common/dbi/account.py` & `dimples-0.2.3/dimples/common/dbi/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/common/dbi/message.py` & `dimples-0.2.3/dimples/common/dbi/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/common/dbi/session.py` & `dimples-0.2.3/dimples/common/dbi/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/common/facebook.py` & `dimples-0.2.3/dimples/common/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/common/messenger.py` & `dimples-0.2.3/dimples/common/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/common/packer.py` & `dimples-0.2.3/dimples/common/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/common/protocol/__init__.py` & `dimples-0.2.3/dimples/common/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/common/protocol/ans.py` & `dimples-0.2.3/dimples/common/protocol/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/common/protocol/handshake.py` & `dimples-0.2.3/dimples/common/protocol/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/common/protocol/login.py` & `dimples-0.2.3/dimples/common/protocol/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/common/protocol/report.py` & `dimples-0.2.3/dimples/common/protocol/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/common/session.py` & `dimples-0.2.3/dimples/common/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
     @property
     def active(self) -> bool:
         """ Session active """
         raise NotImplemented
 
     @abstractmethod
-    def set_active(self, active: bool, when: float = None):
+    def set_active(self, active: bool, when: float = None) -> bool:
         """ Update active flag and return True on changed """
         raise NotImplemented
 
     def __str__(self) -> str:
         clazz = self.__class__.__name__
         return '<%s:%s %s|%s active=%s />' % (clazz, self.key, self.remote_address, self.identifier, self.active)
```

### Comparing `dimples-0.2.2/dimples/config.py` & `dimples-0.2.3/dimples/config.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/conn/__init__.py` & `dimples-0.2.3/dimples/conn/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/conn/gate.py` & `dimples-0.2.3/dimples/conn/gate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/conn/gatekeeper.py` & `dimples-0.2.3/dimples/conn/gatekeeper.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/conn/mars.py` & `dimples-0.2.3/dimples/conn/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/conn/mtp.py` & `dimples-0.2.3/dimples/conn/mtp.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/conn/protocol/__init__.py` & `dimples-0.2.3/dimples/conn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/conn/protocol/mars.py` & `dimples-0.2.3/dimples/conn/protocol/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/conn/protocol/ws.py` & `dimples-0.2.3/dimples/conn/protocol/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/conn/queue.py` & `dimples-0.2.3/dimples/conn/queue.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/conn/seeker.py` & `dimples-0.2.3/dimples/conn/seeker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/conn/session.py` & `dimples-0.2.3/dimples/conn/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/conn/ws.py` & `dimples-0.2.3/dimples/conn/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/__init__.py` & `dimples-0.2.3/dimples/database/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/account.py` & `dimples-0.2.3/dimples/database/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/dos/__init__.py` & `dimples-0.2.3/dimples/database/dos/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/dos/base.py` & `dimples-0.2.3/dimples/database/dos/base.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/dos/document.py` & `dimples-0.2.3/dimples/database/dos/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/dos/group.py` & `dimples-0.2.3/dimples/database/dos/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/dos/login.py` & `dimples-0.2.3/dimples/database/dos/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/dos/meta.py` & `dimples-0.2.3/dimples/database/dos/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/dos/private.py` & `dimples-0.2.3/dimples/database/dos/private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/dos/station.py` & `dimples-0.2.3/dimples/database/dos/station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/dos/user.py` & `dimples-0.2.3/dimples/database/dos/user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/message.py` & `dimples-0.2.3/dimples/database/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/session.py` & `dimples-0.2.3/dimples/database/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/t_cipherkey.py` & `dimples-0.2.3/dimples/database/t_cipherkey.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/t_document.py` & `dimples-0.2.3/dimples/database/t_document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/t_group.py` & `dimples-0.2.3/dimples/database/t_group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/t_login.py` & `dimples-0.2.3/dimples/database/t_login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/t_message.py` & `dimples-0.2.3/dimples/database/t_message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/t_meta.py` & `dimples-0.2.3/dimples/database/t_meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/t_private.py` & `dimples-0.2.3/dimples/database/t_private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/t_station.py` & `dimples-0.2.3/dimples/database/t_station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/database/t_user.py` & `dimples-0.2.3/dimples/database/t_user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/edge/__init__.py` & `dimples-0.2.3/dimples/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/edge/octopus.py` & `dimples-0.2.3/dimples/edge/octopus.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/edge/shared.py` & `dimples-0.2.3/dimples/edge/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/edge/start.py` & `dimples-0.2.3/dimples/edge/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/register/__init__.py` & `dimples-0.2.3/dimples/register/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/register/generate.py` & `dimples-0.2.3/dimples/register/generate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/register/modify.py` & `dimples-0.2.3/dimples/register/modify.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/register/run.py` & `dimples-0.2.3/dimples/register/run.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/register/shared.py` & `dimples-0.2.3/dimples/register/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/server/__init__.py` & `dimples-0.2.3/dimples/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/server/broadcast.py` & `dimples-0.2.3/dimples/server/broadcast.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
                 bots = self.station_bots
                 for bid in bots:
                     if traces.search(node=bid) >= 0:
                         self.warning(msg='skip duplicated bot: %s' % bid)
                         continue
                     recipients.add(bid)
         elif receiver.is_user:
-            # 'archivist@anywhere', 'apns@anywhere', 'master@anywhere'
+            # 'archivist@anywhere', 'announcer@anywhere', 'monitor@anywhere'
             name = receiver.name
             if name is not None:
                 assert name != 'station' and name != 'anyone', 'receiver error: %s' % receiver
                 bot = AnsCommandProcessor.ans_id(name=name)
                 self.info(msg='forward to bot: %s -> %s' % (name, bot))
                 if bot is not None and traces.search(node=bot) < 0:
                     recipients.add(bot)
```

### Comparing `dimples-0.2.2/dimples/server/cpu/__init__.py` & `dimples-0.2.3/dimples/server/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/server/cpu/ans.py` & `dimples-0.2.3/dimples/server/cpu/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/server/cpu/document.py` & `dimples-0.2.3/dimples/server/cpu/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/server/cpu/handshake.py` & `dimples-0.2.3/dimples/server/cpu/handshake.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,14 +71,15 @@
             # verified success
             handshake_accepted(identifier=msg.sender, session=session, messenger=messenger)
             res = HandshakeCommand.success(session=session.key)
         else:
             # session key not match
             # ask client to sign it with the new session key
             res = HandshakeCommand.again(session=session.key)
+        res['remote_address'] = session.remote_address
         return [res]
 
 
 def handshake_accepted(identifier: ID, session: Session, messenger: CommonMessenger):
     from ..session_center import SessionCenter
     center = SessionCenter()
     # 1. update session ID
```

### Comparing `dimples-0.2.2/dimples/server/cpu/login.py` & `dimples-0.2.3/dimples/server/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/server/cpu/report.py` & `dimples-0.2.3/dimples/server/cpu/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/server/dispatcher.py` & `dimples-0.2.3/dimples/server/dispatcher.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/server/messenger.py` & `dimples-0.2.3/dimples/server/messenger.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,15 @@
             broadcast_reliable_message(msg=msg, station=sid)
             # if receiver.is_group:
             #     broadcast message to multiple destinations,
             #     current station is it's receiver too.
             if receiver.is_group:
                 return s_msg
             # otherwise, this message should have been redirected
-            # e.g.: 'archivist@anywhere', 'apns@anywhere', 'master@anywhere'
+            # e.g.: 'archivist@anywhere', 'announcer@anywhere', 'monitor@anywhere'
             return None
         elif receiver.is_group:
             self.error(msg='group message should not send to station: %s -> %s' % (sender, receiver))
             return None
         # 3. this message is not for current station,
         # deliver to the real receiver and respond to sender
         dispatcher = Dispatcher()
```

### Comparing `dimples-0.2.2/dimples/server/packer.py` & `dimples-0.2.3/dimples/server/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/server/processor.py` & `dimples-0.2.3/dimples/server/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/server/push.py` & `dimples-0.2.3/dimples/server/push.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/server/session.py` & `dimples-0.2.3/dimples/server/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         old = self.identifier
         if super().set_identifier(identifier=identifier):
             session_change_id(session=self, new_id=identifier, old_id=old)
             load_cached_messages(session=self)
             return True
 
     # Override
-    def set_active(self, active: bool, when: float = None):
+    def set_active(self, active: bool, when: float = None) -> bool:
         if super().set_active(active=active, when=when):
             session_change_active(session=self, active=active)
             if active:
                 load_cached_messages(session=self)
             return True
 
     @property  # Override
```

### Comparing `dimples-0.2.2/dimples/server/session_center.py` & `dimples-0.2.3/dimples/server/session_center.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/server/trace.py` & `dimples-0.2.3/dimples/server/trace.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/station/__init__.py` & `dimples-0.2.3/dimples/station/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/station/handler.py` & `dimples-0.2.3/dimples/station/handler.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/station/shared.py` & `dimples-0.2.3/dimples/station/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/station/start.py` & `dimples-0.2.3/dimples/station/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/utils/__init__.py` & `dimples-0.2.3/dimples/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/utils/cache.py` & `dimples-0.2.3/dimples/utils/cache.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/utils/checker.py` & `dimples-0.2.3/dimples/utils/checker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/utils/dos.py` & `dimples-0.2.3/dimples/utils/dos.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/utils/log.py` & `dimples-0.2.3/dimples/utils/log.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples/utils/singleton.py` & `dimples-0.2.3/dimples/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.2/dimples.egg-info/PKG-INFO` & `dimples-0.2.3/dimples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.2.2
+Version: 0.2.3
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.2.2/dimples.egg-info/SOURCES.txt` & `dimples-0.2.3/dimples.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 dimples.egg-info/PKG-INFO
 dimples.egg-info/SOURCES.txt
 dimples.egg-info/dependency_links.txt
 dimples.egg-info/entry_points.txt
 dimples.egg-info/requires.txt
 dimples.egg-info/top_level.txt
 dimples/client/__init__.py
+dimples/client/checkpoint.py
 dimples/client/group.py
 dimples/client/messenger.py
 dimples/client/packer.py
 dimples/client/processor.py
 dimples/client/terminal.py
 dimples/client/cpu/__init__.py
 dimples/client/cpu/grp_expel.py
```

### Comparing `dimples-0.2.2/setup.py` & `dimples-0.2.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
```

