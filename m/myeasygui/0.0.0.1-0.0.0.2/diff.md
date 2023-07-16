# Comparing `tmp/myeasygui-0.0.0.1.tar.gz` & `tmp/myeasygui-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\myeasygui-0.0.0.1.tar", last modified: Sat Jul 15 06:11:42 2023, max compression
+gzip compressed data, was "dist\myeasygui-0.0.0.2.tar", last modified: Sun Jul 16 06:49:58 2023, max compression
```

## Comparing `myeasygui-0.0.0.1.tar` & `myeasygui-0.0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 06:11:42.000000 myeasygui-0.0.0.1/
--rw-rw-rw-   0        0        0      122 2023-07-15 06:11:42.000000 myeasygui-0.0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-15 06:11:42.000000 myeasygui-0.0.0.1/myeasygui.egg-info/
--rw-rw-rw-   0        0        0      122 2023-07-15 06:11:42.000000 myeasygui-0.0.0.1/myeasygui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      580 2023-07-15 06:11:42.000000 myeasygui-0.0.0.1/myeasygui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 06:11:42.000000 myeasygui-0.0.0.1/myeasygui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-15 06:11:42.000000 myeasygui-0.0.0.1/myeasygui.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 06:11:42.000000 myeasygui-0.0.0.1/mygui/
--rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.1/mygui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 06:11:42.000000 myeasygui-0.0.0.1/mygui/boxes/
--rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.1/mygui/boxes/Errorbox.py
--rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.1/mygui/boxes/Warningbox.py
--rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.1/mygui/boxes/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.1/mygui/boxes/directorybox.py
--rw-rw-rw-   0        0        0      369 2023-07-15 06:09:19.000000 myeasygui-0.0.0.1/mygui/boxes/enterbox.py
--rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.1/mygui/boxes/fileopenbox.py
--rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.1/mygui/boxes/filesavesbox.py
--rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.1/mygui/boxes/msgbox.py
--rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.1/mygui/boxes/okcancelbox.py
--rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.1/mygui/boxes/passwordbox.py
--rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.1/mygui/boxes/questionbox.py
--rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.1/mygui/boxes/retrycancelbox.py
--rw-rw-rw-   0        0        0      265 2023-07-15 06:09:19.000000 myeasygui-0.0.0.1/mygui/boxes/textbox.py
--rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.1/mygui/boxes/userpasswordbox.py
--rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.1/mygui/boxes/yesnobox.py
--rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.1/mygui/boxes/yesnocancelbox.py
--rw-rw-rw-   0        0        0       42 2023-07-15 06:11:42.000000 myeasygui-0.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      243 2023-07-15 06:08:10.000000 myeasygui-0.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:49:58.000000 myeasygui-0.0.0.2/
+-rw-rw-rw-   0        0        0      169 2023-07-16 06:49:58.000000 myeasygui-0.0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-16 06:49:57.000000 myeasygui-0.0.0.2/myeasygui/
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.2/myeasygui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:49:58.000000 myeasygui-0.0.0.2/myeasygui/boxes/
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.2/myeasygui/boxes/Errorbox.py
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.2/myeasygui/boxes/Warningbox.py
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.2/myeasygui/boxes/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.2/myeasygui/boxes/directorybox.py
+-rw-rw-rw-   0        0        0      369 2023-07-15 06:09:19.000000 myeasygui-0.0.0.2/myeasygui/boxes/enterbox.py
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.2/myeasygui/boxes/fileopenbox.py
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.2/myeasygui/boxes/filesavesbox.py
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.2/myeasygui/boxes/msgbox.py
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.2/myeasygui/boxes/okcancelbox.py
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.2/myeasygui/boxes/passwordbox.py
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.2/myeasygui/boxes/questionbox.py
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.2/myeasygui/boxes/retrycancelbox.py
+-rw-rw-rw-   0        0        0      265 2023-07-15 06:09:19.000000 myeasygui-0.0.0.2/myeasygui/boxes/textbox.py
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.2/myeasygui/boxes/userpasswordbox.py
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.2/myeasygui/boxes/yesnobox.py
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:09:19.000000 myeasygui-0.0.0.2/myeasygui/boxes/yesnocancelbox.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:49:57.000000 myeasygui-0.0.0.2/myeasygui.egg-info/
+-rw-rw-rw-   0        0        0      169 2023-07-16 06:49:57.000000 myeasygui-0.0.0.2/myeasygui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      648 2023-07-16 06:49:57.000000 myeasygui-0.0.0.2/myeasygui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 06:49:57.000000 myeasygui-0.0.0.2/myeasygui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-16 06:49:57.000000 myeasygui-0.0.0.2/myeasygui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 06:49:58.000000 myeasygui-0.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      522 2023-07-15 07:40:33.000000 myeasygui-0.0.0.2/setup.py
```

