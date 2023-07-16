# Comparing `tmp/robingame-0.1.0.tar.gz` & `tmp/robingame-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robingame-0.1.0.tar", last modified: Wed Jul  5 14:04:27 2023, max compression
+gzip compressed data, was "robingame-1.0.1.tar", last modified: Sun Jul 16 16:53:02 2023, max compression
```

## Comparing `robingame-0.1.0.tar` & `robingame-1.0.1.tar`

### file list

```diff
@@ -1,115 +1,112 @@
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/
--rw-rw-r--   0 robin     (1000) robin     (1000)     1070 2023-05-14 09:02:00.000000 robingame-0.1.0/LICENSE
--rw-rw-r--   0 robin     (1000) robin     (1000)       30 2023-05-14 09:02:00.000000 robingame-0.1.0/MANIFEST.in
--rw-rw-r--   0 robin     (1000) robin     (1000)     1005 2023-07-05 14:04:27.769086 robingame-0.1.0/PKG-INFO
--rw-rw-r--   0 robin     (1000) robin     (1000)      491 2023-07-05 13:47:52.000000 robingame-0.1.0/README.md
--rw-rw-r--   0 robin     (1000) robin     (1000)       85 2023-05-14 09:02:00.000000 robingame-0.1.0/pyproject.toml
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/
--rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/__pycache__/
--rw-rw-r--   0 robin     (1000) robin     (1000)      141 2023-06-29 14:46:13.000000 robingame-0.1.0/robingame/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     1696 2023-06-29 14:46:13.000000 robingame-0.1.0/robingame/__pycache__/animation.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     7698 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/__pycache__/utils.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     1076 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/animation.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/examples/
--rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/examples/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/examples/__pycache__/
--rw-rw-r--   0 robin     (1000) robin     (1000)      150 2023-06-29 14:59:39.000000 robingame-0.1.0/robingame/examples/__pycache__/__init__.cpython-310.pyc
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/examples/gui_examples/
--rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/examples/gui_examples/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/examples/gui_examples/__pycache__/
--rw-rw-r--   0 robin     (1000) robin     (1000)      163 2023-06-29 14:59:39.000000 robingame-0.1.0/robingame/examples/gui_examples/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     6899 2023-07-05 11:38:56.000000 robingame-0.1.0/robingame/examples/gui_examples/__pycache__/coloured_button_effects.cpython-310.pyc
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/examples/gui_examples/assets/
--rw-rw-r--   0 robin     (1000) robin     (1000)      235 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/examples/gui_examples/assets/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/examples/gui_examples/assets/__pycache__/
--rw-rw-r--   0 robin     (1000) robin     (1000)      411 2023-06-29 14:59:39.000000 robingame-0.1.0/robingame/examples/gui_examples/assets/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)      663 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/examples/gui_examples/assets/button-up.aseprite
--rw-rw-r--   0 robin     (1000) robin     (1000)      239 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/examples/gui_examples/assets/button-up.png
--rw-rw-r--   0 robin     (1000) robin     (1000)     1228 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/examples/gui_examples/assets/flashybutton.aseprite
--rw-rw-r--   0 robin     (1000) robin     (1000)      638 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/examples/gui_examples/assets/flashybutton.png
--rw-rw-r--   0 robin     (1000) robin     (1000)     4884 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/examples/gui_examples/coloured_button_effects.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1836 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/examples/gui_examples/complicated_on_press_hook.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1601 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/examples/gui_examples/on_press_event.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1711 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/examples/particle_example.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/gui/
--rw-rw-r--   0 robin     (1000) robin     (1000)       50 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/gui/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/gui/__pycache__/
--rw-rw-r--   0 robin     (1000) robin     (1000)      215 2023-06-29 14:46:14.000000 robingame-0.1.0/robingame/gui/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     4682 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/gui/__pycache__/button.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     1563 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/gui/__pycache__/menu.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     4973 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/gui/button.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1060 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/gui/menu.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/image/
--rw-rw-r--   0 robin     (1000) robin     (1000)       58 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/image/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/image/__pycache__/
--rw-rw-r--   0 robin     (1000) robin     (1000)      216 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/image/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     4184 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/image/__pycache__/classes.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     6057 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/image/__pycache__/utils.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     3928 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/image/classes.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     6228 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/image/utils.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame/input/
--rw-rw-r--   0 robin     (1000) robin     (1000)      142 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/input/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/robingame/input/__pycache__/
--rw-rw-r--   0 robin     (1000) robin     (1000)      329 2023-06-29 14:46:13.000000 robingame-0.1.0/robingame/input/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     2244 2023-06-29 14:46:13.000000 robingame-0.1.0/robingame/input/__pycache__/event.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)    14615 2023-06-29 14:46:13.000000 robingame-0.1.0/robingame/input/__pycache__/gamecube.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)      815 2023-06-29 14:46:14.000000 robingame-0.1.0/robingame/input/__pycache__/keyboard.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     4266 2023-06-29 14:46:13.000000 robingame-0.1.0/robingame/input/__pycache__/queue.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     1623 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/input/event.py
--rw-rw-r--   0 robin     (1000) robin     (1000)    13533 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/input/gamecube.py
--rw-rw-r--   0 robin     (1000) robin     (1000)      278 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/input/keyboard.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     3194 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/input/queue.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     5928 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/input/visualization.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/robingame/objects/
--rw-rw-r--   0 robin     (1000) robin     (1000)      139 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/objects/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/robingame/objects/__pycache__/
--rw-rw-r--   0 robin     (1000) robin     (1000)      338 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/objects/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     3021 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/objects/__pycache__/entity.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     2985 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/objects/__pycache__/game.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     1668 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/objects/__pycache__/group.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     1707 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/objects/__pycache__/helpers.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     2105 2023-07-05 13:48:00.000000 robingame-0.1.0/robingame/objects/__pycache__/particles.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     2755 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/objects/entity.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     2526 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/objects/game.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1098 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/objects/group.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1188 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/objects/helpers.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     2045 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/objects/particles.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     4452 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/recording.py
--rw-rw-r--   0 robin     (1000) robin     (1000)      566 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/sound.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/robingame/text/
--rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/robingame/text/__pycache__/
--rw-rw-r--   0 robin     (1000) robin     (1000)      146 2023-06-29 14:46:14.000000 robingame-0.1.0/robingame/text/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)      314 2023-06-29 14:46:14.000000 robingame-0.1.0/robingame/text/__pycache__/exceptions.cpython-310.pyc
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/robingame/text/assets/
--rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/assets/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1138 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/assets/cellphone-black.png
--rw-rw-r--   0 robin     (1000) robin     (1000)     1103 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/assets/cellphone-white.png
--rw-rw-r--   0 robin     (1000) robin     (1000)     8303 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/assets/test_font.aseprite
--rw-rw-r--   0 robin     (1000) robin     (1000)     2612 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/assets/test_font.png
--rw-rw-r--   0 robin     (1000) robin     (1000)       37 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/exceptions.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/robingame/text/font/
--rw-rw-r--   0 robin     (1000) robin     (1000)       26 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/font/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/robingame/text/font/__pycache__/
--rw-rw-r--   0 robin     (1000) robin     (1000)      187 2023-06-29 14:46:14.000000 robingame-0.1.0/robingame/text/font/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     4035 2023-06-29 14:46:14.000000 robingame-0.1.0/robingame/text/font/__pycache__/classes.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     1073 2023-06-29 14:47:29.000000 robingame-0.1.0/robingame/text/font/__pycache__/fonts.cpython-310.pyc
--rw-rw-r--   0 robin     (1000) robin     (1000)     4112 2023-05-14 09:02:00.000000 robingame-0.1.0/robingame/text/font/classes.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1142 2023-06-29 14:58:35.000000 robingame-0.1.0/robingame/text/font/font_sandbox.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1415 2023-06-29 14:47:25.000000 robingame-0.1.0/robingame/text/font/fonts.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     7727 2023-07-05 13:47:52.000000 robingame-0.1.0/robingame/utils.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.765086 robingame-0.1.0/robingame.egg-info/
--rw-rw-r--   0 robin     (1000) robin     (1000)     1005 2023-07-05 14:04:27.000000 robingame-0.1.0/robingame.egg-info/PKG-INFO
--rw-rw-r--   0 robin     (1000) robin     (1000)     3459 2023-07-05 14:04:27.000000 robingame-0.1.0/robingame.egg-info/SOURCES.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)        1 2023-07-05 14:04:27.000000 robingame-0.1.0/robingame.egg-info/dependency_links.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       45 2023-07-05 14:04:27.000000 robingame-0.1.0/robingame.egg-info/requires.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       10 2023-07-05 14:04:27.000000 robingame-0.1.0/robingame.egg-info/top_level.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)      728 2023-07-05 14:04:27.769086 robingame-0.1.0/setup.cfg
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-05 14:04:27.769086 robingame-0.1.0/tests/
--rw-rw-r--   0 robin     (1000) robin     (1000)      469 2023-05-14 09:02:00.000000 robingame-0.1.0/tests/test_animation.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     2028 2023-07-05 10:07:02.000000 robingame-0.1.0/tests/test_event.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     7148 2023-05-14 09:02:00.000000 robingame-0.1.0/tests/test_image.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     4392 2023-05-14 09:02:00.000000 robingame-0.1.0/tests/test_inputs.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1036 2023-05-14 09:02:00.000000 robingame-0.1.0/tests/test_text.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     2289 2023-05-14 09:02:00.000000 robingame-0.1.0/tests/test_utils.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.684015 robingame-1.0.1/
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1070 2023-05-14 09:02:00.000000 robingame-1.0.1/LICENSE
+-rw-rw-r--   0 robin     (1000) robin     (1000)       30 2023-05-14 09:02:00.000000 robingame-1.0.1/MANIFEST.in
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1918 2023-07-16 16:53:02.684015 robingame-1.0.1/PKG-INFO
+-rw-rw-r--   0 robin     (1000) robin     (1000)      127 2023-07-16 11:05:26.000000 robingame-1.0.1/README.md
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1203 2023-07-16 16:52:48.000000 robingame-1.0.1/pyproject.toml
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.676015 robingame-1.0.1/robingame/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       51 2023-07-16 16:52:48.000000 robingame-1.0.1/robingame/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.676015 robingame-1.0.1/robingame/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      195 2023-07-16 16:52:46.000000 robingame-1.0.1/robingame/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1696 2023-06-29 14:46:13.000000 robingame-1.0.1/robingame/__pycache__/animation.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     7712 2023-07-16 16:38:45.000000 robingame-1.0.1/robingame/__pycache__/utils.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1076 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/animation.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.676015 robingame-1.0.1/robingame/examples/
+-rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/examples/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.676015 robingame-1.0.1/robingame/examples/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      150 2023-06-29 14:59:39.000000 robingame-1.0.1/robingame/examples/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1137 2023-07-16 16:38:37.000000 robingame-1.0.1/robingame/examples/font_sandbox.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.680015 robingame-1.0.1/robingame/examples/gui_examples/
+-rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/examples/gui_examples/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.680015 robingame-1.0.1/robingame/examples/gui_examples/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      163 2023-06-29 14:59:39.000000 robingame-1.0.1/robingame/examples/gui_examples/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     6899 2023-07-05 11:38:56.000000 robingame-1.0.1/robingame/examples/gui_examples/__pycache__/coloured_button_effects.cpython-310.pyc
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.680015 robingame-1.0.1/robingame/examples/gui_examples/assets/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      235 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/examples/gui_examples/assets/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.680015 robingame-1.0.1/robingame/examples/gui_examples/assets/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      411 2023-06-29 14:59:39.000000 robingame-1.0.1/robingame/examples/gui_examples/assets/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)      663 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/examples/gui_examples/assets/button-up.aseprite
+-rw-rw-r--   0 robin     (1000) robin     (1000)      239 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/examples/gui_examples/assets/button-up.png
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1228 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/examples/gui_examples/assets/flashybutton.aseprite
+-rw-rw-r--   0 robin     (1000) robin     (1000)      638 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/examples/gui_examples/assets/flashybutton.png
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4884 2023-07-05 13:47:52.000000 robingame-1.0.1/robingame/examples/gui_examples/coloured_button_effects.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1836 2023-07-05 13:47:52.000000 robingame-1.0.1/robingame/examples/gui_examples/complicated_on_press_hook.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1601 2023-07-05 13:47:52.000000 robingame-1.0.1/robingame/examples/gui_examples/on_press_event.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2142 2023-07-16 16:38:38.000000 robingame-1.0.1/robingame/examples/hello_world.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1711 2023-07-05 13:47:52.000000 robingame-1.0.1/robingame/examples/particle_example.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.680015 robingame-1.0.1/robingame/gui/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       50 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/gui/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.680015 robingame-1.0.1/robingame/gui/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      215 2023-06-29 14:46:14.000000 robingame-1.0.1/robingame/gui/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4682 2023-07-05 13:48:00.000000 robingame-1.0.1/robingame/gui/__pycache__/button.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1563 2023-07-05 13:48:00.000000 robingame-1.0.1/robingame/gui/__pycache__/menu.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4973 2023-07-05 13:47:52.000000 robingame-1.0.1/robingame/gui/button.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1060 2023-07-05 13:47:52.000000 robingame-1.0.1/robingame/gui/menu.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.680015 robingame-1.0.1/robingame/image/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       67 2023-07-16 16:38:38.000000 robingame-1.0.1/robingame/image/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.680015 robingame-1.0.1/robingame/image/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      225 2023-07-16 16:38:45.000000 robingame-1.0.1/robingame/image/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     6032 2023-07-16 16:38:45.000000 robingame-1.0.1/robingame/image/__pycache__/sprite_animation.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     9037 2023-07-16 16:38:45.000000 robingame-1.0.1/robingame/image/__pycache__/utils.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     5935 2023-07-16 16:38:38.000000 robingame-1.0.1/robingame/image/sprite_animation.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     9289 2023-07-16 16:38:38.000000 robingame-1.0.1/robingame/image/utils.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.680015 robingame-1.0.1/robingame/input/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      142 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/input/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.680015 robingame-1.0.1/robingame/input/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      329 2023-06-29 14:46:13.000000 robingame-1.0.1/robingame/input/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2558 2023-07-16 16:38:45.000000 robingame-1.0.1/robingame/input/__pycache__/event.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)    14615 2023-06-29 14:46:13.000000 robingame-1.0.1/robingame/input/__pycache__/gamecube.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1058 2023-07-16 16:38:46.000000 robingame-1.0.1/robingame/input/__pycache__/keyboard.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     5487 2023-07-16 16:38:45.000000 robingame-1.0.1/robingame/input/__pycache__/queue.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1950 2023-07-16 16:38:38.000000 robingame-1.0.1/robingame/input/event.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    13533 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/input/gamecube.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      516 2023-07-16 16:38:38.000000 robingame-1.0.1/robingame/input/keyboard.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4778 2023-07-16 16:38:38.000000 robingame-1.0.1/robingame/input/queue.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     5928 2023-07-05 13:47:52.000000 robingame-1.0.1/robingame/input/visualization.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.684015 robingame-1.0.1/robingame/objects/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      139 2023-07-16 10:16:37.000000 robingame-1.0.1/robingame/objects/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.684015 robingame-1.0.1/robingame/objects/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      338 2023-07-16 11:11:57.000000 robingame-1.0.1/robingame/objects/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     3902 2023-07-16 11:11:57.000000 robingame-1.0.1/robingame/objects/__pycache__/entity.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     3327 2023-07-16 11:11:57.000000 robingame-1.0.1/robingame/objects/__pycache__/game.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1844 2023-07-16 11:11:57.000000 robingame-1.0.1/robingame/objects/__pycache__/group.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1712 2023-07-16 16:38:46.000000 robingame-1.0.1/robingame/objects/__pycache__/helpers.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2105 2023-07-05 13:48:00.000000 robingame-1.0.1/robingame/objects/__pycache__/particles.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     3379 2023-07-16 10:30:09.000000 robingame-1.0.1/robingame/objects/entity.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     3188 2023-07-16 10:59:07.000000 robingame-1.0.1/robingame/objects/game.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1300 2023-07-16 10:38:43.000000 robingame-1.0.1/robingame/objects/group.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1193 2023-07-16 16:38:37.000000 robingame-1.0.1/robingame/objects/helpers.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2045 2023-07-05 13:47:52.000000 robingame-1.0.1/robingame/objects/particles.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4452 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/recording.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      566 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/sound.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.684015 robingame-1.0.1/robingame/text/
+-rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-07-16 12:12:31.000000 robingame-1.0.1/robingame/text/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.684015 robingame-1.0.1/robingame/text/__pycache__/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      146 2023-07-16 12:42:29.000000 robingame-1.0.1/robingame/text/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)      314 2023-06-29 14:46:14.000000 robingame-1.0.1/robingame/text/__pycache__/exceptions.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     6619 2023-07-16 16:38:46.000000 robingame-1.0.1/robingame/text/__pycache__/font.cpython-310.pyc
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1066 2023-07-16 16:38:46.000000 robingame-1.0.1/robingame/text/__pycache__/fonts.cpython-310.pyc
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.684015 robingame-1.0.1/robingame/text/assets/
+-rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/text/assets/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1138 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/text/assets/cellphone-black.png
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1103 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/text/assets/cellphone-white.png
+-rw-rw-r--   0 robin     (1000) robin     (1000)     8303 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/text/assets/test_font.aseprite
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2612 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/text/assets/test_font.png
+-rw-rw-r--   0 robin     (1000) robin     (1000)       37 2023-05-14 09:02:00.000000 robingame-1.0.1/robingame/text/exceptions.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     6698 2023-07-16 16:38:37.000000 robingame-1.0.1/robingame/text/font.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1408 2023-07-16 16:38:37.000000 robingame-1.0.1/robingame/text/fonts.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     7746 2023-07-16 16:38:38.000000 robingame-1.0.1/robingame/utils.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.676015 robingame-1.0.1/robingame.egg-info/
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1918 2023-07-16 16:53:02.000000 robingame-1.0.1/robingame.egg-info/PKG-INFO
+-rw-rw-r--   0 robin     (1000) robin     (1000)     3385 2023-07-16 16:53:02.000000 robingame-1.0.1/robingame.egg-info/SOURCES.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)        1 2023-07-16 16:53:02.000000 robingame-1.0.1/robingame.egg-info/dependency_links.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       27 2023-07-16 16:53:02.000000 robingame-1.0.1/robingame.egg-info/requires.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       10 2023-07-16 16:53:02.000000 robingame-1.0.1/robingame.egg-info/top_level.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       38 2023-07-16 16:53:02.684015 robingame-1.0.1/setup.cfg
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-07-16 16:53:02.684015 robingame-1.0.1/tests/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      469 2023-05-14 09:02:00.000000 robingame-1.0.1/tests/test_animation.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2028 2023-07-05 10:07:02.000000 robingame-1.0.1/tests/test_event.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     8106 2023-07-16 16:38:38.000000 robingame-1.0.1/tests/test_image.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4392 2023-05-14 09:02:00.000000 robingame-1.0.1/tests/test_inputs.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1036 2023-05-14 09:02:00.000000 robingame-1.0.1/tests/test_text.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2289 2023-05-14 09:02:00.000000 robingame-1.0.1/tests/test_utils.py
```

### Comparing `robingame-0.1.0/LICENSE` & `robingame-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/__pycache__/animation.cpython-310.pyc` & `robingame-1.0.1/robingame/__pycache__/animation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/__pycache__/utils.cpython-310.pyc` & `robingame-1.0.1/robingame/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jul  5 13:47:52 2023 UTC, .py size: 7727 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,482 +1,482 @@
-00000000: 6f0d 0d0a 0000 0000 8874 a564 2f1e 0000  o........t.d/...
+00000000: 6f0d 0d0a 0000 0000 0e1d b464 421e 0000  o..........dB...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 6601 0000 6400  .....@...sf...d.
+00000020: 0006 0000 0040 0000 0073 7401 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 0100 6400 6401 6c0a  m.Z.m.Z...d.d.l.
 00000070: 5a0a 6400 6401 6c0b 5a0b 6400 6405 6c0c  Z.d.d.l.Z.d.d.l.
 00000080: 6d0d 5a0d 0100 6507 7234 6400 6406 6c0e  m.Z...e.r4d.d.l.
 00000090: 6d0f 5a0f 0100 6503 6407 6408 6409 6702  m.Z...e.d.d.d.g.
 000000a0: 8302 5a10 640a 640b 640c 640b 640d 6511  ..Z.d.d.d.d.d.e.
 000000b0: 6606 640e 640f 8404 5a12 6410 6411 8400  f.d.d...Z.d.d...
 000000c0: 5a13 6412 6413 8400 5a14 643c 6415 6416  Z.d.d...Z.d<d.d.
 000000d0: 8401 5a15 643d 6417 6418 8401 5a16 6419  ..Z.d=d.d...Z.d.
 000000e0: 650d 6602 641a 641b 8404 5a17 643e 641d  e.f.d.d...Z.d>d.
 000000f0: 641e 8401 5a18 643f 641f 6420 8401 5a19  d...Z.d?d.d ..Z.
 00000100: 6421 6422 8400 5a1a 6423 6424 8400 5a1b  d!d"..Z.d#d$..Z.
-00000110: 6425 6426 8400 5a1c 643d 6427 6428 8401  d%d&..Z.d=d'd(..
-00000120: 5a1d 6429 642a 8400 5a1e 642b 642c 8400  Z.d)d*..Z.d+d,..
-00000130: 5a1f 642d 642e 8400 5a20 642f 6430 8400  Z.d-d...Z d/d0..
-00000140: 5a21 6431 6508 6509 6509 6602 1900 6602  Z!d1e.e.e.f...f.
-00000150: 6432 6433 8404 5a22 6434 6435 8400 5a23  d2d3..Z"d4d5..Z#
-00000160: 6524 6525 6525 6602 1900 5a26 4700 6436  e$e%e%f...Z&G.d6
-00000170: 6437 8400 6437 6527 8303 5a28 6440 6439  d7..d7e'..Z(d@d9
-00000180: 6529 6419 650d 6604 643a 643b 8405 5a2a  e)d.e.f.d:d;..Z*
-00000190: 6401 5300 2941 e900 0000 004e 2901 da0a  d.S.)A.....N)...
-000001a0: 6e61 6d65 6474 7570 6c65 a901 da03 7369  namedtuple....si
-000001b0: 6e29 03da 0d54 5950 455f 4348 4543 4b49  n)...TYPE_CHECKI
-000001c0: 4e47 da05 5475 706c 65da 0341 6e79 2901  NG..Tuple..Any).
-000001d0: da07 5375 7266 6163 6529 01da 0645 6e74  ..Surface)...Ent
-000001e0: 6974 79da 0550 6f69 6e74 da01 78da 0179  ity..Point..x..y
-000001f0: da07 656e 7469 7479 3172 0900 0000 da07  ..entity1r......
-00000200: 656e 7469 7479 32da 0672 6574 7572 6e63  entity2..returnc
-00000210: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000220: 0300 0000 4300 0000 730e 0000 007c 006a  ....C...s....|.j
-00000230: 00a0 017c 016a 02a1 0153 0029 0161 c702  ...|.j...S.).a..
-00000240: 0000 4465 7465 726d 696e 6520 7768 6574  ..Determine whet
-00000250: 6865 7220 656e 7469 7479 3120 6973 2074  her entity1 is t
-00000260: 6f75 6368 696e 6720 656e 7469 7479 322e  ouching entity2.
-00000270: 2054 6869 7320 6675 6e63 7469 6f6e 2069   This function i
-00000280: 7320 6469 7265 6374 696f 6e61 6c20 6279  s directional by
-00000290: 0a20 2020 2064 6573 6967 6e2d 2d2d 692e  .    design---i.
-000002a0: 652e 2069 7420 6368 6563 6b73 2077 6865  e. it checks whe
-000002b0: 7468 6572 0a20 2020 2020 2020 2028 6129  ther.        (a)
-000002c0: 2065 6e74 6974 7931 2e74 6f75 6368 626f   entity1.touchbo
-000002d0: 7820 636f 6c6c 6964 6573 2077 6974 6820  x collides with 
-000002e0: 656e 7469 7479 322e 7265 6374 0a20 2020  entity2.rect.   
-000002f0: 2020 2020 2069 7420 646f 6573 202a 6e6f       it does *no
-00000300: 742a 2063 6865 636b 2077 6865 7468 6572  t* check whether
-00000310: 0a20 2020 2020 2020 2028 6229 2065 6e74  .        (b) ent
-00000320: 6974 7932 2e74 6f75 6368 626f 7820 636f  ity2.touchbox co
-00000330: 6c6c 6964 6573 2077 6974 6820 656e 7469  llides with enti
-00000340: 7479 312e 7265 6374 2e0a 0a20 2020 2054  ty1.rect...    T
-00000350: 6869 7320 6973 2062 6563 6175 7365 2069  his is because i
-00000360: 6e20 6d6f 7374 2063 6173 6573 2074 6865  n most cases the
-00000370: 2065 6e74 6974 6965 7320 7769 6c6c 2068   entities will h
-00000380: 6176 6520 746f 7563 6862 6f78 6573 2077  ave touchboxes w
-00000390: 6974 6820 7468 6520 7361 6d65 2077 6964  ith the same wid
-000003a0: 7468 0a20 2020 2062 7566 6665 722e 2049  th.    buffer. I
-000003b0: 6620 7468 6973 2069 7320 7468 6520 6361  f this is the ca
-000003c0: 7365 2074 6865 6e20 2861 2920 6361 6e6e  se then (a) cann
-000003d0: 6f74 2062 6520 7472 7565 2077 6974 686f  ot be true witho
-000003e0: 7574 2028 6229 2061 6c73 6f20 6265 696e  ut (b) also bein
-000003f0: 6720 7472 7565 2c0a 2020 2020 616e 6420  g true,.    and 
-00000400: 7765 206e 6565 646e 2774 2062 6f74 6865  we needn't bothe
-00000410: 7220 646f 696e 6720 626f 7468 2063 616c  r doing both cal
-00000420: 6375 6c61 7469 6f6e 732e 0a0a 2020 2020  culations...    
-00000430: 416c 736f 2c20 4920 7761 6e74 2074 6f20  Also, I want to 
-00000440: 616c 6c6f 7720 666f 7220 7468 6520 706f  allow for the po
-00000450: 7373 6962 696c 6974 7920 6f66 2075 6e65  ssibility of une
-00000460: 7175 616c 2074 6f75 6368 626f 7820 6275  qual touchbox bu
-00000470: 6666 6572 2077 6964 7468 733b 2069 6e0a  ffer widths; in.
-00000480: 2020 2020 7468 6973 2063 6173 652c 2074      this case, t
-00000490: 6865 206f 7264 6572 202a 7769 6c6c 2a20  he order *will* 
-000004a0: 6d61 7474 6572 2e20 5468 6520 656e 7469  matter. The enti
-000004b0: 7479 2077 6974 6820 7468 6520 6c61 7267  ty with the larg
-000004c0: 6572 2074 6f75 6368 626f 7820 6275 6666  er touchbox buff
-000004d0: 6572 2077 696c 6c0a 2020 2020 2274 6f75  er will.    "tou
-000004e0: 6368 2220 7468 6520 6f74 6865 7220 656e  ch" the other en
-000004f0: 7469 7479 2c20 6275 7420 6e6f 7420 7669  tity, but not vi
-00000500: 6365 2076 6572 7361 2e29 03da 0874 6f75  ce versa.)...tou
-00000510: 6368 626f 78da 0b63 6f6c 6c69 6465 7265  chbox..collidere
-00000520: 6374 da04 7265 6374 2902 720d 0000 0072  ct..rect).r....r
-00000530: 0e00 0000 a900 7213 0000 00fa 2d2f 686f  ......r.....-/ho
-00000540: 6d65 2f72 6f62 696e 2f63 6f64 652f 726f  me/robin/code/ro
-00000550: 6269 6e67 616d 652f 726f 6269 6e67 616d  bingame/robingam
-00000560: 652f 7574 696c 732e 7079 da08 746f 7563  e/utils.py..touc
-00000570: 6869 6e67 1200 0000 7302 0000 000e 0e72  hing....s......r
-00000580: 1500 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00000590: 0004 0000 0004 0000 0043 0000 0073 5000  .........C...sP.
-000005a0: 0000 7400 7c00 6a01 6a02 7c01 6a01 6a02  ..t.|.j.j.|.j.j.
-000005b0: 8302 7403 7c00 6a01 6a04 7c01 6a01 6a04  ..t.|.j.j.|.j.j.
-000005c0: 8302 1800 7d02 7400 7c00 6a01 6a05 7c01  ....}.t.|.j.j.|.
-000005d0: 6a01 6a05 8302 7403 7c00 6a01 6a06 7c01  j.j...t.|.j.j.|.
-000005e0: 6a01 6a06 8302 1800 7d03 7c02 7c03 6602  j.j.....}.|.|.f.
-000005f0: 5300 2901 7a32 4765 7420 7468 6520 7820  S.).z2Get the x 
-00000600: 616e 6420 7920 6f76 6572 6c61 7020 6265  and y overlap be
-00000610: 7477 6565 6e20 6f62 6a31 2061 6e64 206f  tween obj1 and o
-00000620: 626a 322e 7265 6374 2907 da03 6d69 6e72  bj2.rect)...minr
-00000630: 1200 0000 da05 7269 6768 74da 036d 6178  ......right..max
-00000640: da04 6c65 6674 da06 626f 7474 6f6d da03  ..left..bottom..
-00000650: 746f 7029 04da 046f 626a 31da 046f 626a  top)...obj1..obj
-00000660: 32da 0978 5f6f 7665 726c 6170 da09 795f  2..x_overlap..y_
-00000670: 6f76 6572 6c61 7072 1300 0000 7213 0000  overlapr....r...
-00000680: 0072 1400 0000 da1b 6765 745f 6f76 6572  .r......get_over
-00000690: 6c61 705f 6265 7477 6565 6e5f 6f62 6a65  lap_between_obje
-000006a0: 6374 7323 0000 0073 0600 0000 2402 2401  cts#...s....$.$.
-000006b0: 0801 7220 0000 0063 0200 0000 0000 0000  ..r ...c........
-000006c0: 0000 0000 0400 0000 0300 0000 4300 0000  ............C...
-000006d0: 7376 0000 0074 007c 007c 0183 025c 027d  sv...t.|.|...\.}
-000006e0: 027d 037c 027c 036b 0472 237c 006a 016a  .}.|.|.k.r#|.j.j
-000006f0: 027c 016a 016a 026b 0572 1b7c 016a 036a  .|.j.j.k.r.|.j.j
-00000700: 047c 006a 035f 0564 0153 007c 016a 036a  .|.j._.d.S.|.j.j
-00000710: 057c 006a 035f 0464 0153 007c 006a 016a  .|.j._.d.S.|.j.j
-00000720: 067c 016a 016a 066b 0572 337c 016a 036a  .|.j.j.k.r3|.j.j
-00000730: 077c 006a 035f 0864 0153 007c 016a 036a  .|.j._.d.S.|.j.j
-00000740: 087c 006a 035f 0764 0153 0029 027a 3b4d  .|.j._.d.S.).z;M
-00000750: 6f76 6520 6d6f 7661 626c 655f 6f62 6a65  ove movable_obje
-00000760: 6374 206f 7574 7369 6465 2062 6f75 6e64  ct outside bound
-00000770: 6172 6965 7320 6f66 2069 6d6d 6f76 6162  aries of immovab
-00000780: 6c65 5f6f 626a 6563 742e 4e29 0972 2000  le_object.N).r .
-00000790: 0000 da08 6365 6e74 726f 6964 720c 0000  ....centroidr...
-000007a0: 0072 1200 0000 721a 0000 0072 1b00 0000  .r....r....r....
-000007b0: 720b 0000 0072 1700 0000 7219 0000 0029  r....r....r....)
-000007c0: 04da 0e6d 6f76 6162 6c65 5f6f 626a 6563  ...movable_objec
-000007d0: 74da 1069 6d6d 6f76 6162 6c65 5f6f 626a  t..immovable_obj
-000007e0: 6563 7472 1e00 0000 721f 0000 0072 1300  ectr....r....r..
-000007f0: 0000 7213 0000 0072 1400 0000 da0a 756e  ..r....r......un
-00000800: 5f6f 7665 726c 6170 2a00 0000 7310 0000  _overlap*...s...
-00000810: 000e 0208 0110 0110 0110 0210 0210 0110  ................
-00000820: 0272 2400 0000 e97f 0000 0063 0200 0000  .r$........c....
-00000830: 0000 0000 0000 0000 0600 0000 0600 0000  ................
-00000840: 4300 0000 73b4 0000 0074 006a 01a0 027c  C...s....t.j...|
-00000850: 00a0 03a1 00a1 017d 027c 00a0 04a1 007d  .......}.|.....}
-00000860: 037c 0372 3374 057c 00a0 06a1 0083 0144  .|.r3t.|.......D
-00000870: 005d 1c7d 0474 057c 00a0 07a1 0083 0144  .].}.t.|.......D
-00000880: 005d 137d 057c 00a0 087c 057c 0466 02a1  .].}.|...|.|.f..
-00000890: 017c 036b 0372 2f7c 02a0 097c 057c 0466  .|.k.r/|...|.|.f
-000008a0: 0264 01a1 0201 0071 1c71 147c 0253 0074  .d.....q.q.|.S.t
-000008b0: 057c 00a0 06a1 0083 0144 005d 1e7d 0474  .|.......D.].}.t
-000008c0: 057c 00a0 07a1 0083 0144 005d 157d 057c  .|.......D.].}.|
-000008d0: 00a0 087c 057c 0466 02a1 0164 0219 007c  ...|.|.f...d...|
-000008e0: 016b 0472 567c 02a0 097c 057c 0466 0264  .k.rV|...|.|.f.d
-000008f0: 01a1 0201 0071 4171 397c 0253 0029 034e  .....qAq9|.S.).N
-00000900: e901 0000 00e9 0300 0000 290a da06 7079  ..........)...py
-00000910: 6761 6d65 da04 6d61 736b da04 4d61 736b  game..mask..Mask
-00000920: da08 6765 745f 7369 7a65 da0c 6765 745f  ..get_size..get_
-00000930: 636f 6c6f 726b 6579 da05 7261 6e67 65da  colorkey..range.
-00000940: 0a67 6574 5f68 6569 6768 74da 0967 6574  .get_height..get
-00000950: 5f77 6964 7468 da06 6765 745f 6174 da06  _width..get_at..
-00000960: 7365 745f 6174 2906 da07 7375 7266 6163  set_at)...surfac
-00000970: 65da 0974 6872 6573 686f 6c64 7229 0000  e..thresholdr)..
-00000980: 00da 036b 6579 720c 0000 0072 0b00 0000  ...keyr....r....
-00000990: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-000009a0: 0f6d 6173 6b46 726f 6d53 7572 6661 6365  .maskFromSurface
-000009b0: 3b00 0000 7322 0000 0010 0308 0104 0110  ;...s"..........
-000009c0: 0110 0112 0110 0102 8002 fe04 0810 fc10  ................
-000009d0: 0116 0110 0102 8002 fe04 0372 3500 0000  ...........r5...
-000009e0: 6302 0000 0000 0000 0000 0000 0007 0000  c...............
-000009f0: 0006 0000 0043 0000 0073 7a00 0000 7c01  .....C...sz...|.
-00000a00: 7204 7c01 6e05 7400 6a01 6a02 6401 1900  r.|.n.t.j.j.d...
-00000a10: 7d01 7c00 a003 a100 5c02 7d02 7d03 7400  }.|.....\.}.}.t.
-00000a20: a004 7c02 7c03 6602 a101 a005 a100 7d04  ..|.|.f.......}.
-00000a30: 7c04 a006 6402 a101 0100 7407 7c03 8301  |...d.....t.|...
-00000a40: 4400 5d18 7d05 7407 7c02 8301 4400 5d11  D.].}.t.|...D.].
-00000a50: 7d06 7c00 a008 7c06 7c05 6602 a101 7239  }.|...|.|.f...r9
-00000a60: 7c04 a009 7c06 7c05 6602 7c01 a102 0100  |...|.|.f.|.....
-00000a70: 7128 7122 7c04 5300 2903 4eda 076d 6167  q(q"|.S.).N..mag
-00000a80: 656e 7461 a904 7201 0000 0072 0100 0000  enta..r....r....
-00000a90: 7201 0000 0072 0100 0000 290a 7228 0000  r....r....).r(..
-00000aa0: 00da 0563 6f6c 6f72 da09 5448 4543 4f4c  ...color..THECOL
-00000ab0: 4f52 5372 2b00 0000 7208 0000 00da 0d63  ORSr+...r......c
-00000ac0: 6f6e 7665 7274 5f61 6c70 6861 da04 6669  onvert_alpha..fi
-00000ad0: 6c6c 722d 0000 0072 3000 0000 7231 0000  llr-...r0...r1..
-00000ae0: 0029 0772 2900 0000 da09 7365 745f 636f  .).r).....set_co
-00000af0: 6c6f 72da 0577 6964 7468 da06 6865 6967  lor..width..heig
-00000b00: 6874 7232 0000 0072 0c00 0000 720b 0000  htr2...r....r...
-00000b10: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
-00000b20: da0f 6d61 736b 5f74 6f5f 7375 7266 6163  ..mask_to_surfac
-00000b30: 654d 0000 0073 1600 0000 1401 0c01 1201  eM...s..........
-00000b40: 0a01 0c01 0c01 0e01 1001 0280 02fe 0403  ................
-00000b50: 723f 0000 0072 3200 0000 6301 0000 0000  r?...r2...c.....
-00000b60: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
-00000b70: 0000 0073 1000 0000 7400 7c00 8301 7d01  ...s....t.|...}.
-00000b80: 7c01 a001 a100 5300 a901 4e29 0272 3500  |.....S...N).r5.
-00000b90: 0000 da07 6f75 746c 696e 6529 0272 3200  ....outline).r2.
-00000ba0: 0000 7229 0000 0072 1300 0000 7213 0000  ..r)...r....r...
-00000bb0: 0072 1400 0000 da0d 6f75 746c 696e 655f  .r......outline_
-00000bc0: 696d 6167 6559 0000 0073 0400 0000 0801  imageY...s......
-00000bd0: 0801 7242 0000 00e9 3200 0000 6305 0000  ..rB....2...c...
-00000be0: 0000 0000 0000 0000 0007 0000 0006 0000  ................
-00000bf0: 0043 0000 0073 4a00 0000 7400 7c04 7c04  .C...sJ...t.|.|.
-00000c00: 6401 1a00 7c04 6402 1a00 8303 7d05 7401  d...|.d.....}.t.
-00000c10: 7c02 8301 7d06 7c05 a002 7c06 a101 7d05  |...}.|...|...}.
-00000c20: 7c05 7403 a004 7c01 a101 3700 7d05 7405  |.t...|...7.}.t.
-00000c30: 6a06 a007 7c00 7c03 7c05 6403 a104 0100  j...|.|.|.d.....
-00000c40: 6404 5300 2905 7a1c 616e 676c 6520 6e65  d.S.).z.angle ne
-00000c50: 6564 7320 746f 2062 6520 696e 2064 6567  eds to be in deg
-00000c60: 7265 6573 e90a 0000 00e9 0400 0000 e902  rees............
-00000c70: 0000 004e 2908 da0c 6172 726f 775f 636f  ...N)...arrow_co
-00000c80: 6f72 6473 da0f 726f 7461 7469 6f6e 5f6d  ords..rotation_m
-00000c90: 6174 7269 78da 0364 6f74 da05 6e75 6d70  atrix..dot..nump
-00000ca0: 79da 0561 7272 6179 7228 0000 00da 0464  y..arrayr(.....d
-00000cb0: 7261 77da 0770 6f6c 7967 6f6e 2907 7232  raw..polygon).r2
-00000cc0: 0000 00da 066f 7269 6769 6eda 0961 6e67  .....origin..ang
-00000cd0: 6c65 5f64 6567 7238 0000 00da 066c 656e  le_degr8.....len
-00000ce0: 6774 68da 0861 7272 6f77 5f78 79da 0172  gth..arrow_xy..r
-00000cf0: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-00000d00: 0a64 7261 775f 6172 726f 775e 0000 0073  .draw_arrow^...s
-00000d10: 0a00 0000 1402 0801 0a01 0e01 1601 7253  ..............rS
-00000d20: 0000 0063 0400 0000 0000 0000 0000 0000  ...c............
-00000d30: 0500 0000 0600 0000 4300 0000 7346 0000  ........C...sF..
-00000d40: 0074 00a0 017c 00a0 02a1 007c 00a0 03a1  .t...|.....|....
-00000d50: 0066 02a1 01a0 04a1 007d 047c 04a0 0564  .f.......}.|...d
-00000d60: 01a1 0101 0074 006a 06a0 077c 047c 017c  .....t.j...|.|.|
-00000d70: 027c 03a1 0401 007c 00a0 087c 0464 02a1  .|.....|...|.d..
-00000d80: 0201 0064 0053 0029 034e 7237 0000 00a9  ...d.S.).Nr7....
-00000d90: 0272 0100 0000 7201 0000 0029 0972 2800  .r....r....).r(.
-00000da0: 0000 7208 0000 0072 2f00 0000 722e 0000  ..r....r/...r...
-00000db0: 0072 3a00 0000 723b 0000 0072 4c00 0000  .r:...r;...rL...
-00000dc0: 7212 0000 00da 0462 6c69 7429 0572 3200  r......blit).r2.
-00000dd0: 0000 7238 0000 0072 1200 0000 723d 0000  ..r8...r....r=..
-00000de0: 00da 1273 7572 6661 6365 5f77 6974 685f  ...surface_with_
-00000df0: 616c 7068 6172 1300 0000 7213 0000 0072  alphar....r....r
-00000e00: 1400 0000 da09 6472 6177 5f72 6563 7467  ......draw_rectg
-00000e10: 0000 0073 0800 0000 1a02 0a01 1202 1002  ...s............
-00000e20: 7257 0000 0063 0100 0000 0000 0000 0000  rW...c..........
-00000e30: 0000 0300 0000 0700 0000 4300 0000 733e  ..........C...s>
-00000e40: 0000 0074 00a0 017c 00a1 017d 0174 00a0  ...t...|...}.t..
-00000e50: 0274 00a0 037c 01a1 0174 00a0 047c 01a1  .t...|...t...|..
-00000e60: 010b 0066 0274 00a0 047c 01a1 0174 00a0  ...f.t...|...t..
-00000e70: 037c 01a1 0166 0267 02a1 017d 027c 0253  .|...f.g...}.|.S
-00000e80: 0072 4000 0000 2905 724a 0000 00da 0764  .r@...).rJ.....d
-00000e90: 6567 3272 6164 724b 0000 00da 0363 6f73  eg2radrK.....cos
-00000ea0: 7204 0000 0029 0372 4f00 0000 da09 616e  r....).rO.....an
-00000eb0: 676c 655f 7261 6472 4800 0000 7213 0000  gle_radrH...r...
-00000ec0: 0072 1300 0000 7214 0000 0072 4800 0000  .r....r....rH...
-00000ed0: 7400 0000 730e 0000 000a 0104 0114 0212  t...s...........
-00000ee0: 0102 fe04 ff04 0672 4800 0000 6303 0000  .......rH...c...
-00000ef0: 0000 0000 0000 0000 0003 0000 0008 0000  ................
-00000f00: 0043 0000 0073 2e00 0000 7400 a001 6401  .C...s....t...d.
-00000f10: 7c00 6402 6602 7c00 7c02 1800 7c01 6602  |.d.f.|.|...|.f.
-00000f20: 7c00 7c02 1800 7c01 0b00 6602 7c00 6402  |.|...|...f.|.d.
-00000f30: 6602 6705 a101 5300 2903 4e72 5400 0000  f.g...S.).NrT...
-00000f40: 7201 0000 0029 0272 4a00 0000 724b 0000  r....).rJ...rK..
-00000f50: 0029 0372 5000 0000 723d 0000 00da 0b68  .).rP...r=.....h
-00000f60: 6561 645f 6c65 6e67 7468 7213 0000 0072  ead_lengthr....r
-00000f70: 1300 0000 7214 0000 0072 4700 0000 7f00  ....r....rG.....
-00000f80: 0000 7310 0000 0004 0102 0206 010a 010c  ..s.............
-00000f90: 0106 0102 fb04 ff72 4700 0000 6301 0000  .......rG...c...
-00000fa0: 0000 0000 0000 0000 0006 0000 0003 0000  ................
-00000fb0: 0043 0000 0073 5200 0000 6401 7d01 6401  .C...sR...d.}.d.
-00000fc0: 7d02 7400 7c00 8301 4400 5d1c 5c02 7d03  }.t.|...D.].\.}.
-00000fd0: 7d04 7c03 6401 6b02 7212 7c04 7d05 7c04  }.|.d.k.r.|.}.|.
-00000fe0: 721a 7c05 731a 7c01 6402 3700 7d01 7c04  r.|.s.|.d.7.}.|.
-00000ff0: 7322 7c05 7222 7c02 6402 3700 7d02 7c04  s"|.r"|.d.7.}.|.
-00001000: 7d05 7108 7c01 7c02 6602 5300 2903 4e72  }.q.|.|.f.S.).Nr
-00001010: 0100 0000 7226 0000 0029 01da 0965 6e75  ....r&...)...enu
-00001020: 6d65 7261 7465 2906 da06 7661 6c75 6573  merate)...values
-00001030: da0c 7269 7369 6e67 5f65 6467 6573 da0d  ..rising_edges..
-00001040: 6661 6c6c 696e 675f 6564 6765 73da 0269  falling_edges..i
-00001050: 69da 0576 616c 7565 da0e 7072 6576 696f  i..value..previo
-00001060: 7573 5f76 616c 7565 7213 0000 0072 1300  us_valuer....r..
-00001070: 0000 7214 0000 00da 0b63 6f75 6e74 5f65  ..r......count_e
-00001080: 6467 6573 8b00 0000 7316 0000 0004 0104  dges....s.......
-00001090: 0110 0108 0104 0108 0108 0108 0108 0106  ................
-000010a0: 0108 0172 6300 0000 6305 0000 0000 0000  ...rc...c.......
-000010b0: 0000 0000 0007 0000 0004 0000 0043 0000  .............C..
-000010c0: 0073 3800 0000 7c04 7204 7c04 6e01 7400  .s8...|.r.|.n.t.
-000010d0: 7d04 7c02 7c01 1800 6401 1b00 7d05 7c02  }.|.|...d...}.|.
-000010e0: 7c01 1700 6401 1b00 7d06 7c05 7c04 7c00  |...d...}.|.|.|.
-000010f0: 7c03 1400 8301 1400 7c06 1700 5300 2902  |.......|...S.).
-00001100: 4e72 4600 0000 7203 0000 0029 07da 0474  NrF...r....)...t
-00001110: 6963 6b72 1600 0000 7218 0000 00da 0466  ickr....r......f
-00001120: 7265 71da 0466 756e 63da 0141 da01 4272  req..func..A..Br
-00001130: 1300 0000 7213 0000 0072 1400 0000 da0d  ....r....r......
-00001140: 7075 6c73 696e 675f 7661 6c75 6599 0000  pulsing_value...
-00001150: 0073 0800 0000 0c01 0c01 0c01 1401 7269  .s............ri
-00001160: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001170: 0300 0000 0400 0000 4300 0000 731c 0000  ........C...s...
-00001180: 0074 006a 01a0 02a1 005c 027d 017d 027c  .t.j.....\.}.}.|
-00001190: 006a 03a0 047c 017c 02a1 0253 0072 4000  .j...|.|...S.r@.
-000011a0: 0000 2905 7228 0000 00da 056d 6f75 7365  ..).r(.....mouse
-000011b0: da07 6765 745f 706f 7372 1200 0000 da0c  ..get_posr......
-000011c0: 636f 6c6c 6964 6570 6f69 6e74 2903 da07  collidepoint)...
-000011d0: 656c 656d 656e 74da 076d 6f75 7365 5f78  element..mouse_x
-000011e0: da07 6d6f 7573 655f 7972 1300 0000 7213  ..mouse_yr....r.
-000011f0: 0000 0072 1400 0000 da13 6d6f 7573 655f  ...r......mouse_
-00001200: 686f 7665 7269 6e67 5f6f 7665 72a0 0000  hovering_over...
-00001210: 0073 0400 0000 0e01 0e01 7270 0000 0063  .s........rp...c
-00001220: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00001230: 0600 0000 4300 0000 7340 0000 0074 007c  ....C...s@...t.|
-00001240: 0083 017d 0074 017c 0064 0114 007c 0064  ...}.t.|.d...|.d
-00001250: 0114 0066 0283 017d 0274 026a 03a0 047c  ...f...}.t.j...|
-00001260: 027c 017c 007c 0066 027c 00a1 0401 007c  .|.|.|.f.|.....|
-00001270: 02a0 0564 02a1 0101 007c 0253 0029 034e  ...d.....|.S.).N
-00001280: 7246 0000 0029 0372 0100 0000 7201 0000  rF...).r....r...
-00001290: 0072 0100 0000 2906 da03 696e 7472 0800  .r....)...intr..
-000012a0: 0000 7228 0000 0072 4c00 0000 da06 6369  ..r(...rL.....ci
-000012b0: 7263 6c65 da0c 7365 745f 636f 6c6f 726b  rcle..set_colork
-000012c0: 6579 2903 da06 7261 6469 7573 7238 0000  ey)...radiusr8..
-000012d0: 00da 0473 7572 6672 1300 0000 7213 0000  ...surfr....r...
-000012e0: 0072 1400 0000 da0b 6369 7263 6c65 5f73  .r......circle_s
-000012f0: 7572 66a5 0000 0073 0a00 0000 0801 1401  urf....s........
-00001300: 1601 0a01 0401 7276 0000 0063 0200 0000  ......rv...c....
-00001310: 0000 0000 0000 0000 0400 0000 0300 0000  ................
-00001320: 4300 0000 7328 0000 007c 007c 016b 0073  C...s(...|.|.k.s
-00001330: 064a 0082 017c 017c 0018 007d 027c 0074  .J...|.|...}.|.t
-00001340: 00a0 00a1 007c 0214 0017 007d 037c 0353  .....|.....}.|.S
-00001350: 0072 4000 0000 2901 da06 7261 6e64 6f6d  .r@...)...random
-00001360: 2904 7216 0000 0072 1800 0000 da06 7370  ).r....r......sp
-00001370: 7265 6164 7261 0000 0072 1300 0000 7213  readra...r....r.
-00001380: 0000 0072 1400 0000 da0c 7261 6e64 6f6d  ...r......random
-00001390: 5f66 6c6f 6174 ad00 0000 7308 0000 000c  _float....s.....
-000013a0: 0108 0110 0104 0172 7900 0000 6302 0000  .......ry...c...
-000013b0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-000013c0: 0043 0000 0073 0c00 0000 7400 a001 7c00  .C...s....t...|.
-000013d0: 7c01 a102 5300 7240 0000 0029 0272 7700  |...S.r@...).rw.
-000013e0: 0000 da07 7261 6e64 696e 7429 0272 1600  ....randint).r..
-000013f0: 0000 7218 0000 0072 1300 0000 7213 0000  ..r....r....r...
-00001400: 0072 1400 0000 da0a 7261 6e64 6f6d 5f69  .r......random_i
-00001410: 6e74 b400 0000 f302 0000 000c 0172 7b00  nt...........r{.
-00001420: 0000 da07 6265 7477 6565 6e63 0200 0000  ....betweenc....
-00001430: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-00001440: 4300 0000 7318 0000 007c 015c 027d 027d  C...s....|.\.}.}
-00001450: 0374 007c 0274 017c 007c 0383 0283 0253  .t.|.t.|.|.....S
-00001460: 0072 4000 0000 2902 7218 0000 0072 1600  .r@...).r....r..
-00001470: 0000 2904 7261 0000 0072 7d00 0000 da04  ..).ra...r}.....
-00001480: 5f6d 696e da04 5f6d 6178 7213 0000 0072  _min.._maxr....r
-00001490: 1300 0000 7214 0000 00da 0b6c 696d 6974  ....r......limit
-000014a0: 5f76 616c 7565 b800 0000 7304 0000 0008  _value....s.....
-000014b0: 0110 0172 8000 0000 6301 0000 0000 0000  ...r....c.......
-000014c0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-000014d0: 0073 0c00 0000 7400 7401 7c00 8e00 8301  .s....t.t.|.....
-000014e0: 5300 7240 0000 0029 02da 0574 7570 6c65  S.r@...)...tuple
-000014f0: da03 7a69 7029 01da 067a 6970 7065 6472  ..zip)...zippedr
-00001500: 1300 0000 7213 0000 0072 1400 0000 da05  ....r....r......
-00001510: 756e 7a69 70bd 0000 0072 7c00 0000 7284  unzip....r|...r.
-00001520: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00001530: 0000 0000 0500 0000 0000 0000 73ae 0000  ............s...
-00001540: 0065 005a 0164 005a 0264 015a 0365 0465  .e.Z.d.Z.d.Z.e.e
-00001550: 0565 0566 0219 0065 0464 0219 0042 005a  .e.f...e.d...B.Z
-00001560: 0665 0764 0365 0465 0665 0666 0219 0066  .e.d.e.e.e.f...f
-00001570: 0264 0464 0584 0483 015a 0865 0764 0365  .d.d.....Z.e.d.e
-00001580: 0565 0566 0266 0264 0664 0784 0483 015a  .e.f.f.d.d.....Z
-00001590: 0965 0764 0365 0666 0264 0864 0984 0483  .e.d.e.f.d.d....
-000015a0: 015a 0a65 0764 0365 0666 0264 0a64 0b84  .Z.e.d.e.f.d.d..
-000015b0: 0483 015a 0b65 0764 0365 0566 0264 0c64  ...Z.e.d.e.f.d.d
-000015c0: 0d84 0483 015a 0c65 0764 0365 0566 0264  .....Z.e.d.e.f.d
-000015d0: 0e64 0f84 0483 015a 0d64 1287 0066 0164  .d.....Z.d...f.d
-000015e0: 1064 1184 0c5a 0e87 0004 005a 0f53 0029  .d...Z.....Z.S.)
-000015f0: 13da 0c53 7061 7273 654d 6174 7269 787a  ...SparseMatrixz
-00001600: b80a 2020 2020 4469 6374 696f 6e61 7279  ..    Dictionary
-00001610: 206f 6620 7468 6520 666f 726d 207b 2878   of the form {(x
-00001620: 2c20 7929 3a20 7661 6c75 657d 2e20 4361  , y): value}. Ca
-00001630: 6e20 6265 2075 7365 6420 746f 2073 696d  n be used to sim
-00001640: 756c 6174 6520 616e 2069 6e66 696e 6974  ulate an infinit
-00001650: 6520 6772 6964 2e0a 2020 2020 4561 6368  e grid..    Each
-00001660: 2065 6e74 7279 2072 6570 7265 7365 6e74   entry represent
-00001670: 7320 6120 6365 6c6c 2077 6974 6820 7769  s a cell with wi
-00001680: 6474 6820 616e 6420 6865 6967 6874 206f  dth and height o
-00001690: 6620 3120 2869 2e65 2e20 4e4f 5420 6120  f 1 (i.e. NOT a 
-000016a0: 6469 6d65 6e73 696f 6e6c 6573 7320 706f  dimensionless po
-000016b0: 696e 7429 0a20 2020 20a9 024e 4e72 0f00  int).    ..NNr..
-000016c0: 0000 6301 0000 0000 0000 0000 0000 0005  ..c.............
-000016d0: 0000 0003 0000 0043 0000 0073 4c00 0000  .......C...sL...
-000016e0: 7c00 721e 7400 7c00 a001 a100 8301 5c02  |.r.t.|.......\.
-000016f0: 7d01 7d02 7402 7c01 8301 7403 7c01 8301  }.}.t.|...t.|...
-00001700: 6602 7d03 7402 7c02 8301 7403 7c02 8301  f.}.t.|...t.|...
-00001710: 6602 7d04 7c03 7c04 6602 5300 6401 0400  f.}.|.|.f.S.d...
-00001720: 7d03 7d04 7c03 7c04 6602 5300 2902 7a29  }.}.|.|.f.S.).z)
-00001730: 5468 6520 6d69 6e20 616e 6420 6d61 7820  The min and max 
-00001740: 782f 7920 636f 6f72 6473 206f 6620 616c  x/y coords of al
-00001750: 6c20 656e 7472 6965 7372 8600 0000 2904  l entriesr....).
-00001760: 7284 0000 00da 046b 6579 7372 1600 0000  r......keysr....
-00001770: 7218 0000 0029 05da 0473 656c 66da 0278  r....)...self..x
-00001780: 73da 0279 73da 0478 6c69 6dda 0479 6c69  s..ys..xlim..yli
-00001790: 6d72 1300 0000 7213 0000 0072 1400 0000  mr....r....r....
-000017a0: da06 6c69 6d69 7473 cc00 0000 730e 0000  ..limits....s...
-000017b0: 0004 0310 0110 0110 0108 0308 ff08 017a  ...............z
-000017c0: 1353 7061 7273 654d 6174 7269 782e 6c69  .SparseMatrix.li
-000017d0: 6d69 7473 6301 0000 0000 0000 0000 0000  mitsc...........
-000017e0: 0005 0000 0003 0000 0043 0000 0073 4e00  .........C...sN.
-000017f0: 0000 7c00 721f 7c00 6a00 5c02 7d01 7d02  ..|.r.|.j.\.}.}.
-00001800: 7c01 6401 1900 7c01 6402 1900 1800 6401  |.d...|.d.....d.
-00001810: 1700 7d03 7c02 6401 1900 7c02 6402 1900  ..}.|.d...|.d...
-00001820: 1800 6401 1700 7d04 7c03 7c04 6602 5300  ..d...}.|.|.f.S.
-00001830: 6402 0400 7d03 7d04 7c03 7c04 6602 5300  d...}.}.|.|.f.S.
-00001840: 2903 4e72 2600 0000 7201 0000 00a9 0172  ).Nr&...r......r
-00001850: 8d00 0000 2905 7288 0000 0072 8b00 0000  ....).r....r....
-00001860: 728c 0000 0072 3d00 0000 723e 0000 0072  r....r=...r>...r
-00001870: 1300 0000 7213 0000 0072 1400 0000 da04  ....r....r......
-00001880: 7369 7a65 d700 0000 730e 0000 0004 020a  size....s.......
-00001890: 0114 0114 0108 0308 ff08 017a 1153 7061  ...........z.Spa
-000018a0: 7273 654d 6174 7269 782e 7369 7a65 6301  rseMatrix.sizec.
-000018b0: 0000 0000 0000 0000 0000 0003 0000 0002  ................
-000018c0: 0000 0043 0000 00f3 0e00 0000 7c00 6a00  ...C........|.j.
-000018d0: 5c02 7d01 7d02 7c01 5300 7240 0000 0072  \.}.}.|.S.r@...r
-000018e0: 8e00 0000 2903 7288 0000 0072 8b00 0000  ....).r....r....
-000018f0: da01 5f72 1300 0000 7213 0000 0072 1400  .._r....r....r..
-00001900: 0000 728b 0000 00e1 0000 00f3 0400 0000  ..r.............
-00001910: 0a02 0401 7a11 5370 6172 7365 4d61 7472  ....z.SparseMatr
-00001920: 6978 2e78 6c69 6d63 0100 0000 0000 0000  ix.xlimc........
-00001930: 0000 0000 0300 0000 0200 0000 4300 0000  ............C...
-00001940: f30e 0000 007c 006a 005c 027d 017d 027c  .....|.j.\.}.}.|
-00001950: 0253 0072 4000 0000 728e 0000 0029 0372  .S.r@...r....).r
-00001960: 8800 0000 7291 0000 0072 8c00 0000 7213  ....r....r....r.
-00001970: 0000 0072 1300 0000 7214 0000 0072 8c00  ...r....r....r..
-00001980: 0000 e600 0000 7292 0000 007a 1153 7061  ......r....z.Spa
-00001990: 7273 654d 6174 7269 782e 796c 696d 6301  rseMatrix.ylimc.
-000019a0: 0000 0000 0000 0000 0000 0003 0000 0002  ................
-000019b0: 0000 0043 0000 0072 9000 0000 7240 0000  ...C...r....r@..
-000019c0: 00a9 0172 8f00 0000 2903 7288 0000 0072  ...r....).r....r
-000019d0: 3d00 0000 7291 0000 0072 1300 0000 7213  =...r....r....r.
-000019e0: 0000 0072 1400 0000 723d 0000 00eb 0000  ...r....r=......
-000019f0: 0072 9200 0000 7a12 5370 6172 7365 4d61  .r....z.SparseMa
-00001a00: 7472 6978 2e77 6964 7468 6301 0000 0000  trix.widthc.....
-00001a10: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
-00001a20: 0000 0072 9300 0000 7240 0000 0072 9400  ...r....r@...r..
-00001a30: 0000 2903 7288 0000 0072 9100 0000 723e  ..).r....r....r>
-00001a40: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
-00001a50: 0000 723e 0000 00f0 0000 0072 9200 0000  ..r>.......r....
-00001a60: 7a13 5370 6172 7365 4d61 7472 6978 2e68  z.SparseMatrix.h
-00001a70: 6569 6768 7463 0100 0000 0000 0000 0000  eightc..........
-00001a80: 0000 0100 0000 0300 0000 0300 0000 730e  ..............s.
-00001a90: 0000 0074 0074 0183 00a0 02a1 0083 0153  ...t.t.........S
-00001aa0: 0072 4000 0000 2903 7285 0000 00da 0573  .r@...).r......s
-00001ab0: 7570 6572 da04 636f 7079 2901 7288 0000  uper..copy).r...
-00001ac0: 00a9 01da 095f 5f63 6c61 7373 5f5f 7213  .....__class__r.
-00001ad0: 0000 0072 1400 0000 7296 0000 00f5 0000  ...r....r.......
-00001ae0: 0073 0200 0000 0e01 7a11 5370 6172 7365  .s......z.Sparse
-00001af0: 4d61 7472 6978 2e63 6f70 7929 0272 0f00  Matrix.copy).r..
-00001b00: 0000 7285 0000 0029 10da 085f 5f6e 616d  ..r....)...__nam
-00001b10: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00001b20: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
-00001b30: 5f64 6f63 5f5f 7281 0000 0072 7100 0000  _doc__r....rq...
-00001b40: da05 4c69 6d69 74da 0870 726f 7065 7274  ..Limit..propert
-00001b50: 7972 8d00 0000 728f 0000 0072 8b00 0000  yr....r....r....
-00001b60: 728c 0000 0072 3d00 0000 723e 0000 0072  r....r=...r>...r
-00001b70: 9600 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
-00001b80: 6c5f 5f72 1300 0000 7213 0000 0072 9700  l__r....r....r..
-00001b90: 0000 7214 0000 0072 8500 0000 c400 0000  ..r....r........
-00001ba0: 7320 0000 0008 0004 0114 0502 0218 0102  s ..............
-00001bb0: 0a14 0102 0910 0102 0410 0102 0410 0102  ................
-00001bc0: 0410 0116 0472 8500 0000 46da 0173 6306  .....r....F..sc.
-00001bd0: 0000 0000 0000 0000 0000 0007 0000 0005  ................
-00001be0: 0000 0043 0000 0073 1e00 0000 7c03 a000  ...C...s....|...
-00001bf0: 7c00 7c05 7c04 a103 7d06 7c01 a001 7c06  |.|.|...}.|...|.
-00001c00: 7c02 a102 0100 6400 5300 7240 0000 0029  |.....d.S.r@...)
-00001c10: 02da 0672 656e 6465 7272 5500 0000 2907  ...renderrU...).
-00001c20: 72a0 0000 0072 3200 0000 da08 706f 7369  r....r2.....posi
-00001c30: 7469 6f6e da04 666f 6e74 7238 0000 00da  tion..fontr8....
-00001c40: 0961 6e74 6961 6c69 6173 da0b 7465 7874  .antialias..text
-00001c50: 5f62 6974 6d61 7072 1300 0000 7213 0000  _bitmapr....r...
-00001c60: 0072 1400 0000 da09 6472 6177 5f74 6578  .r......draw_tex
-00001c70: 74f9 0000 0073 0400 0000 0e01 1001 72a6  t....s........r.
-00001c80: 0000 0029 0172 2500 0000 7240 0000 0029  ...).r%...r@...)
-00001c90: 024e 7243 0000 0029 0172 0100 0000 2901  .NrC...).r....).
-00001ca0: 4629 2b72 7700 0000 da04 656e 756d da0b  F)+rw.....enum..
-00001cb0: 636f 6c6c 6563 7469 6f6e 7372 0200 0000  collectionsr....
-00001cc0: da04 6d61 7468 7204 0000 00da 0674 7970  ..mathr......typ
-00001cd0: 696e 6772 0500 0000 7206 0000 0072 0700  ingr....r....r..
-00001ce0: 0000 724a 0000 0072 2800 0000 da0e 7079  ..rJ...r(.....py
-00001cf0: 6761 6d65 2e73 7572 6661 6365 7208 0000  game.surfacer...
-00001d00: 00da 1872 6f62 696e 6761 6d65 2e6f 626a  ...robingame.obj
-00001d10: 6563 7473 2e65 6e74 6974 7972 0900 0000  ects.entityr....
-00001d20: 720a 0000 00da 0462 6f6f 6c72 1500 0000  r......boolr....
-00001d30: 7220 0000 0072 2400 0000 7235 0000 0072  r ...r$...r5...r
-00001d40: 3f00 0000 7242 0000 0072 5300 0000 7257  ?...rB...rS...rW
-00001d50: 0000 0072 4800 0000 7247 0000 0072 6300  ...rH...rG...rc.
-00001d60: 0000 7269 0000 0072 7000 0000 7276 0000  ..ri...rp...rv..
-00001d70: 0072 7900 0000 727b 0000 0072 8000 0000  .ry...r{...r....
-00001d80: 7284 0000 0072 8100 0000 7271 0000 00da  r....r....rq....
-00001d90: 0543 6f6f 7264 da04 6469 6374 7285 0000  .Coord..dictr...
-00001da0: 00da 0373 7472 72a6 0000 0072 1300 0000  ...strr....r....
-00001db0: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-00001dc0: 083c 6d6f 6475 6c65 3e01 0000 0073 4000  .<module>....s@.
-00001dd0: 0000 0800 0801 0c01 0c01 1401 0802 0801  ................
-00001de0: 0c01 0403 0c01 0e02 1603 0811 0807 0a11  ................
-00001df0: 0a12 0e0c 0a05 0a09 080d 080b 080c 0a0e  ................
-00001e00: 0807 0805 0808 0807 1604 0805 0c04 1003  ................
-00001e10: 1835                                     .5
+00000110: 640d 651c 651d 651d 6602 1900 6602 6425  d.e.e.e.f...f.d%
+00000120: 6426 8404 5a1e 643d 6427 6428 8401 5a1f  d&..Z.d=d'd(..Z.
+00000130: 6429 642a 8400 5a20 642b 642c 8400 5a21  d)d*..Z d+d,..Z!
+00000140: 642d 642e 8400 5a22 642f 6430 8400 5a23  d-d...Z"d/d0..Z#
+00000150: 6431 6508 6509 6509 6602 1900 6602 6432  d1e.e.e.f...f.d2
+00000160: 6433 8404 5a24 6434 6435 8400 5a25 651c  d3..Z$d4d5..Z%e.
+00000170: 651d 651d 6602 1900 5a26 4700 6436 6437  e.e.f...Z&G.d6d7
+00000180: 8400 6437 6527 8303 5a28 6440 6439 6529  ..d7e'..Z(d@d9e)
+00000190: 6419 650d 6604 643a 643b 8405 5a2a 6401  d.e.f.d:d;..Z*d.
+000001a0: 5300 2941 e900 0000 004e 2901 da0a 6e61  S.)A.....N)...na
+000001b0: 6d65 6474 7570 6c65 a901 da03 7369 6e29  medtuple....sin)
+000001c0: 03da 0d54 5950 455f 4348 4543 4b49 4e47  ...TYPE_CHECKING
+000001d0: da05 5475 706c 65da 0341 6e79 2901 da07  ..Tuple..Any)...
+000001e0: 5375 7266 6163 6529 01da 0645 6e74 6974  Surface)...Entit
+000001f0: 79da 0550 6f69 6e74 da01 78da 0179 da07  y..Point..x..y..
+00000200: 656e 7469 7479 3172 0900 0000 da07 656e  entity1r......en
+00000210: 7469 7479 32da 0672 6574 7572 6e63 0200  tity2..returnc..
+00000220: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00000230: 0000 4300 0000 730e 0000 007c 006a 00a0  ..C...s....|.j..
+00000240: 017c 016a 02a1 0153 0029 0161 c702 0000  .|.j...S.).a....
+00000250: 4465 7465 726d 696e 6520 7768 6574 6865  Determine whethe
+00000260: 7220 656e 7469 7479 3120 6973 2074 6f75  r entity1 is tou
+00000270: 6368 696e 6720 656e 7469 7479 322e 2054  ching entity2. T
+00000280: 6869 7320 6675 6e63 7469 6f6e 2069 7320  his function is 
+00000290: 6469 7265 6374 696f 6e61 6c20 6279 0a20  directional by. 
+000002a0: 2020 2064 6573 6967 6e2d 2d2d 692e 652e     design---i.e.
+000002b0: 2069 7420 6368 6563 6b73 2077 6865 7468   it checks wheth
+000002c0: 6572 0a20 2020 2020 2020 2028 6129 2065  er.        (a) e
+000002d0: 6e74 6974 7931 2e74 6f75 6368 626f 7820  ntity1.touchbox 
+000002e0: 636f 6c6c 6964 6573 2077 6974 6820 656e  collides with en
+000002f0: 7469 7479 322e 7265 6374 0a20 2020 2020  tity2.rect.     
+00000300: 2020 2069 7420 646f 6573 202a 6e6f 742a     it does *not*
+00000310: 2063 6865 636b 2077 6865 7468 6572 0a20   check whether. 
+00000320: 2020 2020 2020 2028 6229 2065 6e74 6974         (b) entit
+00000330: 7932 2e74 6f75 6368 626f 7820 636f 6c6c  y2.touchbox coll
+00000340: 6964 6573 2077 6974 6820 656e 7469 7479  ides with entity
+00000350: 312e 7265 6374 2e0a 0a20 2020 2054 6869  1.rect...    Thi
+00000360: 7320 6973 2062 6563 6175 7365 2069 6e20  s is because in 
+00000370: 6d6f 7374 2063 6173 6573 2074 6865 2065  most cases the e
+00000380: 6e74 6974 6965 7320 7769 6c6c 2068 6176  ntities will hav
+00000390: 6520 746f 7563 6862 6f78 6573 2077 6974  e touchboxes wit
+000003a0: 6820 7468 6520 7361 6d65 2077 6964 7468  h the same width
+000003b0: 0a20 2020 2062 7566 6665 722e 2049 6620  .    buffer. If 
+000003c0: 7468 6973 2069 7320 7468 6520 6361 7365  this is the case
+000003d0: 2074 6865 6e20 2861 2920 6361 6e6e 6f74   then (a) cannot
+000003e0: 2062 6520 7472 7565 2077 6974 686f 7574   be true without
+000003f0: 2028 6229 2061 6c73 6f20 6265 696e 6720   (b) also being 
+00000400: 7472 7565 2c0a 2020 2020 616e 6420 7765  true,.    and we
+00000410: 206e 6565 646e 2774 2062 6f74 6865 7220   needn't bother 
+00000420: 646f 696e 6720 626f 7468 2063 616c 6375  doing both calcu
+00000430: 6c61 7469 6f6e 732e 0a0a 2020 2020 416c  lations...    Al
+00000440: 736f 2c20 4920 7761 6e74 2074 6f20 616c  so, I want to al
+00000450: 6c6f 7720 666f 7220 7468 6520 706f 7373  low for the poss
+00000460: 6962 696c 6974 7920 6f66 2075 6e65 7175  ibility of unequ
+00000470: 616c 2074 6f75 6368 626f 7820 6275 6666  al touchbox buff
+00000480: 6572 2077 6964 7468 733b 2069 6e0a 2020  er widths; in.  
+00000490: 2020 7468 6973 2063 6173 652c 2074 6865    this case, the
+000004a0: 206f 7264 6572 202a 7769 6c6c 2a20 6d61   order *will* ma
+000004b0: 7474 6572 2e20 5468 6520 656e 7469 7479  tter. The entity
+000004c0: 2077 6974 6820 7468 6520 6c61 7267 6572   with the larger
+000004d0: 2074 6f75 6368 626f 7820 6275 6666 6572   touchbox buffer
+000004e0: 2077 696c 6c0a 2020 2020 2274 6f75 6368   will.    "touch
+000004f0: 2220 7468 6520 6f74 6865 7220 656e 7469  " the other enti
+00000500: 7479 2c20 6275 7420 6e6f 7420 7669 6365  ty, but not vice
+00000510: 2076 6572 7361 2e29 03da 0874 6f75 6368   versa.)...touch
+00000520: 626f 78da 0b63 6f6c 6c69 6465 7265 6374  box..colliderect
+00000530: da04 7265 6374 2902 720d 0000 0072 0e00  ..rect).r....r..
+00000540: 0000 a900 7213 0000 00fa 2d2f 686f 6d65  ....r.....-/home
+00000550: 2f72 6f62 696e 2f63 6f64 652f 726f 6269  /robin/code/robi
+00000560: 6e67 616d 652f 726f 6269 6e67 616d 652f  ngame/robingame/
+00000570: 7574 696c 732e 7079 da08 746f 7563 6869  utils.py..touchi
+00000580: 6e67 1200 0000 7302 0000 000e 0e72 1500  ng....s......r..
+00000590: 0000 6302 0000 0000 0000 0000 0000 0004  ..c.............
+000005a0: 0000 0004 0000 0043 0000 0073 5000 0000  .......C...sP...
+000005b0: 7400 7c00 6a01 6a02 7c01 6a01 6a02 8302  t.|.j.j.|.j.j...
+000005c0: 7403 7c00 6a01 6a04 7c01 6a01 6a04 8302  t.|.j.j.|.j.j...
+000005d0: 1800 7d02 7400 7c00 6a01 6a05 7c01 6a01  ..}.t.|.j.j.|.j.
+000005e0: 6a05 8302 7403 7c00 6a01 6a06 7c01 6a01  j...t.|.j.j.|.j.
+000005f0: 6a06 8302 1800 7d03 7c02 7c03 6602 5300  j.....}.|.|.f.S.
+00000600: 2901 7a32 4765 7420 7468 6520 7820 616e  ).z2Get the x an
+00000610: 6420 7920 6f76 6572 6c61 7020 6265 7477  d y overlap betw
+00000620: 6565 6e20 6f62 6a31 2061 6e64 206f 626a  een obj1 and obj
+00000630: 322e 7265 6374 2907 da03 6d69 6e72 1200  2.rect)...minr..
+00000640: 0000 da05 7269 6768 74da 036d 6178 da04  ....right..max..
+00000650: 6c65 6674 da06 626f 7474 6f6d da03 746f  left..bottom..to
+00000660: 7029 04da 046f 626a 31da 046f 626a 32da  p)...obj1..obj2.
+00000670: 0978 5f6f 7665 726c 6170 da09 795f 6f76  .x_overlap..y_ov
+00000680: 6572 6c61 7072 1300 0000 7213 0000 0072  erlapr....r....r
+00000690: 1400 0000 da1b 6765 745f 6f76 6572 6c61  ......get_overla
+000006a0: 705f 6265 7477 6565 6e5f 6f62 6a65 6374  p_between_object
+000006b0: 7323 0000 0073 0600 0000 2402 2401 0801  s#...s....$.$...
+000006c0: 7220 0000 0063 0200 0000 0000 0000 0000  r ...c..........
+000006d0: 0000 0400 0000 0300 0000 4300 0000 7376  ..........C...sv
+000006e0: 0000 0074 007c 007c 0183 025c 027d 027d  ...t.|.|...\.}.}
+000006f0: 037c 027c 036b 0472 237c 006a 016a 027c  .|.|.k.r#|.j.j.|
+00000700: 016a 016a 026b 0572 1b7c 016a 036a 047c  .j.j.k.r.|.j.j.|
+00000710: 006a 035f 0564 0153 007c 016a 036a 057c  .j._.d.S.|.j.j.|
+00000720: 006a 035f 0464 0153 007c 006a 016a 067c  .j._.d.S.|.j.j.|
+00000730: 016a 016a 066b 0572 337c 016a 036a 077c  .j.j.k.r3|.j.j.|
+00000740: 006a 035f 0864 0153 007c 016a 036a 087c  .j._.d.S.|.j.j.|
+00000750: 006a 035f 0764 0153 0029 027a 3b4d 6f76  .j._.d.S.).z;Mov
+00000760: 6520 6d6f 7661 626c 655f 6f62 6a65 6374  e movable_object
+00000770: 206f 7574 7369 6465 2062 6f75 6e64 6172   outside boundar
+00000780: 6965 7320 6f66 2069 6d6d 6f76 6162 6c65  ies of immovable
+00000790: 5f6f 626a 6563 742e 4e29 0972 2000 0000  _object.N).r ...
+000007a0: da08 6365 6e74 726f 6964 720c 0000 0072  ..centroidr....r
+000007b0: 1200 0000 721a 0000 0072 1b00 0000 720b  ....r....r....r.
+000007c0: 0000 0072 1700 0000 7219 0000 0029 04da  ...r....r....)..
+000007d0: 0e6d 6f76 6162 6c65 5f6f 626a 6563 74da  .movable_object.
+000007e0: 1069 6d6d 6f76 6162 6c65 5f6f 626a 6563  .immovable_objec
+000007f0: 7472 1e00 0000 721f 0000 0072 1300 0000  tr....r....r....
+00000800: 7213 0000 0072 1400 0000 da0a 756e 5f6f  r....r......un_o
+00000810: 7665 726c 6170 2a00 0000 7310 0000 000e  verlap*...s.....
+00000820: 0208 0110 0110 0110 0210 0210 0110 0272  ...............r
+00000830: 2400 0000 e97f 0000 0063 0200 0000 0000  $........c......
+00000840: 0000 0000 0000 0600 0000 0600 0000 4300  ..............C.
+00000850: 0000 73b4 0000 0074 006a 01a0 027c 00a0  ..s....t.j...|..
+00000860: 03a1 00a1 017d 027c 00a0 04a1 007d 037c  .....}.|.....}.|
+00000870: 0372 3374 057c 00a0 06a1 0083 0144 005d  .r3t.|.......D.]
+00000880: 1c7d 0474 057c 00a0 07a1 0083 0144 005d  .}.t.|.......D.]
+00000890: 137d 057c 00a0 087c 057c 0466 02a1 017c  .}.|...|.|.f...|
+000008a0: 036b 0372 2f7c 02a0 097c 057c 0466 0264  .k.r/|...|.|.f.d
+000008b0: 01a1 0201 0071 1c71 147c 0253 0074 057c  .....q.q.|.S.t.|
+000008c0: 00a0 06a1 0083 0144 005d 1e7d 0474 057c  .......D.].}.t.|
+000008d0: 00a0 07a1 0083 0144 005d 157d 057c 00a0  .......D.].}.|..
+000008e0: 087c 057c 0466 02a1 0164 0219 007c 016b  .|.|.f...d...|.k
+000008f0: 0472 567c 02a0 097c 057c 0466 0264 01a1  .rV|...|.|.f.d..
+00000900: 0201 0071 4171 397c 0253 0029 034e e901  ...qAq9|.S.).N..
+00000910: 0000 00e9 0300 0000 290a da06 7079 6761  ........)...pyga
+00000920: 6d65 da04 6d61 736b da04 4d61 736b da08  me..mask..Mask..
+00000930: 6765 745f 7369 7a65 da0c 6765 745f 636f  get_size..get_co
+00000940: 6c6f 726b 6579 da05 7261 6e67 65da 0a67  lorkey..range..g
+00000950: 6574 5f68 6569 6768 74da 0967 6574 5f77  et_height..get_w
+00000960: 6964 7468 da06 6765 745f 6174 da06 7365  idth..get_at..se
+00000970: 745f 6174 2906 da07 7375 7266 6163 65da  t_at)...surface.
+00000980: 0974 6872 6573 686f 6c64 7229 0000 00da  .thresholdr)....
+00000990: 036b 6579 720c 0000 0072 0b00 0000 7213  .keyr....r....r.
+000009a0: 0000 0072 1300 0000 7214 0000 00da 0f6d  ...r....r......m
+000009b0: 6173 6b46 726f 6d53 7572 6661 6365 3b00  askFromSurface;.
+000009c0: 0000 7322 0000 0010 0308 0104 0110 0110  ..s"............
+000009d0: 0112 0110 0102 8002 fe04 0810 fc10 0116  ................
+000009e0: 0110 0102 8002 fe04 0372 3500 0000 6302  .........r5...c.
+000009f0: 0000 0000 0000 0000 0000 0007 0000 0006  ................
+00000a00: 0000 0043 0000 0073 7a00 0000 7c01 7204  ...C...sz...|.r.
+00000a10: 7c01 6e05 7400 6a01 6a02 6401 1900 7d01  |.n.t.j.j.d...}.
+00000a20: 7c00 a003 a100 5c02 7d02 7d03 7400 a004  |.....\.}.}.t...
+00000a30: 7c02 7c03 6602 a101 a005 a100 7d04 7c04  |.|.f.......}.|.
+00000a40: a006 6402 a101 0100 7407 7c03 8301 4400  ..d.....t.|...D.
+00000a50: 5d18 7d05 7407 7c02 8301 4400 5d11 7d06  ].}.t.|...D.].}.
+00000a60: 7c00 a008 7c06 7c05 6602 a101 7239 7c04  |...|.|.f...r9|.
+00000a70: a009 7c06 7c05 6602 7c01 a102 0100 7128  ..|.|.f.|.....q(
+00000a80: 7122 7c04 5300 2903 4eda 076d 6167 656e  q"|.S.).N..magen
+00000a90: 7461 a904 7201 0000 0072 0100 0000 7201  ta..r....r....r.
+00000aa0: 0000 0072 0100 0000 290a 7228 0000 00da  ...r....).r(....
+00000ab0: 0563 6f6c 6f72 da09 5448 4543 4f4c 4f52  .color..THECOLOR
+00000ac0: 5372 2b00 0000 7208 0000 00da 0d63 6f6e  Sr+...r......con
+00000ad0: 7665 7274 5f61 6c70 6861 da04 6669 6c6c  vert_alpha..fill
+00000ae0: 722d 0000 0072 3000 0000 7231 0000 0029  r-...r0...r1...)
+00000af0: 0772 2900 0000 da09 7365 745f 636f 6c6f  .r).....set_colo
+00000b00: 72da 0577 6964 7468 da06 6865 6967 6874  r..width..height
+00000b10: 7232 0000 0072 0c00 0000 720b 0000 0072  r2...r....r....r
+00000b20: 1300 0000 7213 0000 0072 1400 0000 da0f  ....r....r......
+00000b30: 6d61 736b 5f74 6f5f 7375 7266 6163 654d  mask_to_surfaceM
+00000b40: 0000 0073 1600 0000 1401 0c01 1201 0a01  ...s............
+00000b50: 0c01 0c01 0e01 1001 0280 02fe 0403 723f  ..............r?
+00000b60: 0000 0072 3200 0000 6301 0000 0000 0000  ...r2...c.......
+00000b70: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
+00000b80: 0073 1000 0000 7400 7c00 8301 7d01 7c01  .s....t.|...}.|.
+00000b90: a001 a100 5300 a901 4e29 0272 3500 0000  ....S...N).r5...
+00000ba0: da07 6f75 746c 696e 6529 0272 3200 0000  ..outline).r2...
+00000bb0: 7229 0000 0072 1300 0000 7213 0000 0072  r)...r....r....r
+00000bc0: 1400 0000 da0d 6f75 746c 696e 655f 696d  ......outline_im
+00000bd0: 6167 6559 0000 0073 0400 0000 0801 0801  ageY...s........
+00000be0: 7242 0000 00e9 3200 0000 6305 0000 0000  rB....2...c.....
+00000bf0: 0000 0000 0000 0007 0000 0006 0000 0043  ...............C
+00000c00: 0000 0073 4a00 0000 7400 7c04 7c04 6401  ...sJ...t.|.|.d.
+00000c10: 1a00 7c04 6402 1a00 8303 7d05 7401 7c02  ..|.d.....}.t.|.
+00000c20: 8301 7d06 7c05 a002 7c06 a101 7d05 7c05  ..}.|...|...}.|.
+00000c30: 7403 a004 7c01 a101 3700 7d05 7405 6a06  t...|...7.}.t.j.
+00000c40: a007 7c00 7c03 7c05 6403 a104 0100 6404  ..|.|.|.d.....d.
+00000c50: 5300 2905 7a1c 616e 676c 6520 6e65 6564  S.).z.angle need
+00000c60: 7320 746f 2062 6520 696e 2064 6567 7265  s to be in degre
+00000c70: 6573 e90a 0000 00e9 0400 0000 e902 0000  es..............
+00000c80: 004e 2908 da0c 6172 726f 775f 636f 6f72  .N)...arrow_coor
+00000c90: 6473 da0f 726f 7461 7469 6f6e 5f6d 6174  ds..rotation_mat
+00000ca0: 7269 78da 0364 6f74 da05 6e75 6d70 79da  rix..dot..numpy.
+00000cb0: 0561 7272 6179 7228 0000 00da 0464 7261  .arrayr(.....dra
+00000cc0: 77da 0770 6f6c 7967 6f6e 2907 7232 0000  w..polygon).r2..
+00000cd0: 00da 066f 7269 6769 6eda 0961 6e67 6c65  ...origin..angle
+00000ce0: 5f64 6567 7238 0000 00da 066c 656e 6774  _degr8.....lengt
+00000cf0: 68da 0861 7272 6f77 5f78 79da 0172 7213  h..arrow_xy..rr.
+00000d00: 0000 0072 1300 0000 7214 0000 00da 0a64  ...r....r......d
+00000d10: 7261 775f 6172 726f 775e 0000 0073 0a00  raw_arrow^...s..
+00000d20: 0000 1402 0801 0a01 0e01 1601 7253 0000  ............rS..
+00000d30: 0063 0400 0000 0000 0000 0000 0000 0500  .c..............
+00000d40: 0000 0600 0000 4300 0000 7346 0000 0074  ......C...sF...t
+00000d50: 00a0 017c 00a0 02a1 007c 00a0 03a1 0066  ...|.....|.....f
+00000d60: 02a1 01a0 04a1 007d 047c 04a0 0564 01a1  .......}.|...d..
+00000d70: 0101 0074 006a 06a0 077c 047c 017c 027c  ...t.j...|.|.|.|
+00000d80: 03a1 0401 007c 00a0 087c 0464 02a1 0201  .....|...|.d....
+00000d90: 0064 0053 0029 034e 7237 0000 00a9 0272  .d.S.).Nr7.....r
+00000da0: 0100 0000 7201 0000 0029 0972 2800 0000  ....r....).r(...
+00000db0: 7208 0000 0072 2f00 0000 722e 0000 0072  r....r/...r....r
+00000dc0: 3a00 0000 723b 0000 0072 4c00 0000 7212  :...r;...rL...r.
+00000dd0: 0000 00da 0462 6c69 7429 0572 3200 0000  .....blit).r2...
+00000de0: 7238 0000 0072 1200 0000 723d 0000 00da  r8...r....r=....
+00000df0: 1273 7572 6661 6365 5f77 6974 685f 616c  .surface_with_al
+00000e00: 7068 6172 1300 0000 7213 0000 0072 1400  phar....r....r..
+00000e10: 0000 da09 6472 6177 5f72 6563 7467 0000  ....draw_rectg..
+00000e20: 0073 0800 0000 1a02 0a01 1202 1002 7257  .s............rW
+00000e30: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000e40: 0300 0000 0700 0000 4300 0000 733e 0000  ........C...s>..
+00000e50: 0074 00a0 017c 00a1 017d 0174 00a0 0274  .t...|...}.t...t
+00000e60: 00a0 037c 01a1 0174 00a0 047c 01a1 010b  ...|...t...|....
+00000e70: 0066 0274 00a0 047c 01a1 0174 00a0 037c  .f.t...|...t...|
+00000e80: 01a1 0166 0267 02a1 017d 027c 0253 0072  ...f.g...}.|.S.r
+00000e90: 4000 0000 2905 724a 0000 00da 0764 6567  @...).rJ.....deg
+00000ea0: 3272 6164 724b 0000 00da 0363 6f73 7204  2radrK.....cosr.
+00000eb0: 0000 0029 0372 4f00 0000 da09 616e 676c  ...).rO.....angl
+00000ec0: 655f 7261 6472 4800 0000 7213 0000 0072  e_radrH...r....r
+00000ed0: 1300 0000 7214 0000 0072 4800 0000 7400  ....r....rH...t.
+00000ee0: 0000 730e 0000 000a 0104 0114 0212 0102  ..s.............
+00000ef0: fe04 ff04 0672 4800 0000 6303 0000 0000  .....rH...c.....
+00000f00: 0000 0000 0000 0003 0000 0008 0000 0043  ...............C
+00000f10: 0000 0073 2e00 0000 7400 a001 6401 7c00  ...s....t...d.|.
+00000f20: 6402 6602 7c00 7c02 1800 7c01 6602 7c00  d.f.|.|...|.f.|.
+00000f30: 7c02 1800 7c01 0b00 6602 7c00 6402 6602  |...|...f.|.d.f.
+00000f40: 6705 a101 5300 2903 4e72 5400 0000 7201  g...S.).NrT...r.
+00000f50: 0000 0029 0272 4a00 0000 724b 0000 0029  ...).rJ...rK...)
+00000f60: 0372 5000 0000 723d 0000 00da 0b68 6561  .rP...r=.....hea
+00000f70: 645f 6c65 6e67 7468 7213 0000 0072 1300  d_lengthr....r..
+00000f80: 0000 7214 0000 0072 4700 0000 7f00 0000  ..r....rG.......
+00000f90: 7310 0000 0004 0102 0206 010a 010c 0106  s...............
+00000fa0: 0102 fb04 ff72 4700 0000 6301 0000 0000  .....rG...c.....
+00000fb0: 0000 0000 0000 0006 0000 0003 0000 0043  ...............C
+00000fc0: 0000 0073 5200 0000 6401 7d01 6401 7d02  ...sR...d.}.d.}.
+00000fd0: 7400 7c00 8301 4400 5d1c 5c02 7d03 7d04  t.|...D.].\.}.}.
+00000fe0: 7c03 6401 6b02 7212 7c04 7d05 7c04 721a  |.d.k.r.|.}.|.r.
+00000ff0: 7c05 731a 7c01 6402 3700 7d01 7c04 7322  |.s.|.d.7.}.|.s"
+00001000: 7c05 7222 7c02 6402 3700 7d02 7c04 7d05  |.r"|.d.7.}.|.}.
+00001010: 7108 7c01 7c02 6602 5300 2903 4e72 0100  q.|.|.f.S.).Nr..
+00001020: 0000 7226 0000 0029 01da 0965 6e75 6d65  ..r&...)...enume
+00001030: 7261 7465 2906 da06 7661 6c75 6573 da0c  rate)...values..
+00001040: 7269 7369 6e67 5f65 6467 6573 da0d 6661  rising_edges..fa
+00001050: 6c6c 696e 675f 6564 6765 73da 0269 69da  lling_edges..ii.
+00001060: 0576 616c 7565 da0e 7072 6576 696f 7573  .value..previous
+00001070: 5f76 616c 7565 7213 0000 0072 1300 0000  _valuer....r....
+00001080: 7214 0000 00da 0b63 6f75 6e74 5f65 6467  r......count_edg
+00001090: 6573 8b00 0000 7316 0000 0004 0104 0110  es....s.........
+000010a0: 0108 0104 0108 0108 0108 0108 0106 0108  ................
+000010b0: 0172 6300 0000 6305 0000 0000 0000 0000  .rc...c.........
+000010c0: 0000 0007 0000 0004 0000 0043 0000 0073  ...........C...s
+000010d0: 3800 0000 7c04 7204 7c04 6e01 7400 7d04  8...|.r.|.n.t.}.
+000010e0: 7c02 7c01 1800 6401 1b00 7d05 7c02 7c01  |.|...d...}.|.|.
+000010f0: 1700 6401 1b00 7d06 7c05 7c04 7c00 7c03  ..d...}.|.|.|.|.
+00001100: 1400 8301 1400 7c06 1700 5300 2902 4e72  ......|...S.).Nr
+00001110: 4600 0000 7203 0000 0029 07da 0474 6963  F...r....)...tic
+00001120: 6b72 1600 0000 7218 0000 00da 0466 7265  kr....r......fre
+00001130: 71da 0466 756e 63da 0141 da01 4272 1300  q..func..A..Br..
+00001140: 0000 7213 0000 0072 1400 0000 da0d 7075  ..r....r......pu
+00001150: 6c73 696e 675f 7661 6c75 6599 0000 0073  lsing_value....s
+00001160: 0800 0000 0c01 0c01 0c01 1401 7269 0000  ............ri..
+00001170: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
+00001180: 0000 0400 0000 4300 0000 731c 0000 0074  ......C...s....t
+00001190: 006a 01a0 02a1 005c 027d 017d 027c 006a  .j.....\.}.}.|.j
+000011a0: 03a0 047c 017c 02a1 0253 0072 4000 0000  ...|.|...S.r@...
+000011b0: 2905 7228 0000 00da 056d 6f75 7365 da07  ).r(.....mouse..
+000011c0: 6765 745f 706f 7372 1200 0000 da0c 636f  get_posr......co
+000011d0: 6c6c 6964 6570 6f69 6e74 2903 da07 656c  llidepoint)...el
+000011e0: 656d 656e 74da 076d 6f75 7365 5f78 da07  ement..mouse_x..
+000011f0: 6d6f 7573 655f 7972 1300 0000 7213 0000  mouse_yr....r...
+00001200: 0072 1400 0000 da13 6d6f 7573 655f 686f  .r......mouse_ho
+00001210: 7665 7269 6e67 5f6f 7665 72a0 0000 0073  vering_over....s
+00001220: 0400 0000 0e01 0e01 7270 0000 0063 0200  ........rp...c..
+00001230: 0000 0000 0000 0000 0000 0300 0000 0600  ................
+00001240: 0000 4300 0000 7340 0000 0074 007c 0083  ..C...s@...t.|..
+00001250: 017d 0074 017c 0064 0114 007c 0064 0114  .}.t.|.d...|.d..
+00001260: 0066 0283 017d 0274 026a 03a0 047c 027c  .f...}.t.j...|.|
+00001270: 017c 007c 0066 027c 00a1 0401 007c 02a0  .|.|.f.|.....|..
+00001280: 0564 02a1 0101 007c 0253 0029 034e 7246  .d.....|.S.).NrF
+00001290: 0000 0029 0372 0100 0000 7201 0000 0072  ...).r....r....r
+000012a0: 0100 0000 2906 da03 696e 7472 0800 0000  ....)...intr....
+000012b0: 7228 0000 0072 4c00 0000 da06 6369 7263  r(...rL.....circ
+000012c0: 6c65 da0c 7365 745f 636f 6c6f 726b 6579  le..set_colorkey
+000012d0: 2903 da06 7261 6469 7573 7238 0000 00da  )...radiusr8....
+000012e0: 0473 7572 6672 1300 0000 7213 0000 0072  .surfr....r....r
+000012f0: 1400 0000 da0b 6369 7263 6c65 5f73 7572  ......circle_sur
+00001300: 66a5 0000 0073 0a00 0000 0801 1401 1601  f....s..........
+00001310: 0a01 0401 7276 0000 0063 0200 0000 0000  ....rv...c......
+00001320: 0000 0000 0000 0400 0000 0300 0000 4300  ..............C.
+00001330: 0000 7328 0000 007c 007c 016b 0073 064a  ..s(...|.|.k.s.J
+00001340: 0082 017c 017c 0018 007d 027c 0074 00a0  ...|.|...}.|.t..
+00001350: 00a1 007c 0214 0017 007d 037c 0353 0072  ...|.....}.|.S.r
+00001360: 4000 0000 2901 da06 7261 6e64 6f6d 2904  @...)...random).
+00001370: 7216 0000 0072 1800 0000 da06 7370 7265  r....r......spre
+00001380: 6164 7261 0000 0072 1300 0000 7213 0000  adra...r....r...
+00001390: 0072 1400 0000 da0c 7261 6e64 6f6d 5f66  .r......random_f
+000013a0: 6c6f 6174 ad00 0000 7308 0000 000c 0108  loat....s.......
+000013b0: 0110 0104 0172 7900 0000 6302 0000 0000  .....ry...c.....
+000013c0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+000013d0: 0000 0073 0c00 0000 7400 a001 7c00 7c01  ...s....t...|.|.
+000013e0: a102 5300 7240 0000 0029 0272 7700 0000  ..S.r@...).rw...
+000013f0: da07 7261 6e64 696e 7429 0272 1600 0000  ..randint).r....
+00001400: 7218 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
+00001410: 1400 0000 da0a 7261 6e64 6f6d 5f69 6e74  ......random_int
+00001420: b400 0000 f302 0000 000c 0172 7b00 0000  ...........r{...
+00001430: da07 6265 7477 6565 6e63 0200 0000 0000  ..betweenc......
+00001440: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
+00001450: 0000 7318 0000 007c 015c 027d 027d 0374  ..s....|.\.}.}.t
+00001460: 007c 0274 017c 007c 0383 0283 0253 0072  .|.t.|.|.....S.r
+00001470: 4000 0000 2902 7218 0000 0072 1600 0000  @...).r....r....
+00001480: 2904 7261 0000 0072 7d00 0000 da04 5f6d  ).ra...r}....._m
+00001490: 696e da04 5f6d 6178 7213 0000 0072 1300  in.._maxr....r..
+000014a0: 0000 7214 0000 00da 0b6c 696d 6974 5f76  ..r......limit_v
+000014b0: 616c 7565 b800 0000 7304 0000 0008 0110  alue....s.......
+000014c0: 0172 8000 0000 6301 0000 0000 0000 0000  .r....c.........
+000014d0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+000014e0: 0c00 0000 7400 7401 7c00 8e00 8301 5300  ....t.t.|.....S.
+000014f0: 7240 0000 0029 02da 0574 7570 6c65 da03  r@...)...tuple..
+00001500: 7a69 7029 01da 067a 6970 7065 6472 1300  zip)...zippedr..
+00001510: 0000 7213 0000 0072 1400 0000 da05 756e  ..r....r......un
+00001520: 7a69 70bd 0000 0072 7c00 0000 7284 0000  zip....r|...r...
+00001530: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00001540: 0000 0500 0000 0000 0000 73ae 0000 0065  ..........s....e
+00001550: 005a 0164 005a 0264 015a 0365 0465 0565  .Z.d.Z.d.Z.e.e.e
+00001560: 0566 0219 0065 0464 0219 0042 005a 0665  .f...e.d...B.Z.e
+00001570: 0764 0365 0465 0665 0666 0219 0066 0264  .d.e.e.e.f...f.d
+00001580: 0464 0584 0483 015a 0865 0764 0365 0565  .d.....Z.e.d.e.e
+00001590: 0566 0266 0264 0664 0784 0483 015a 0965  .f.f.d.d.....Z.e
+000015a0: 0764 0365 0666 0264 0864 0984 0483 015a  .d.e.f.d.d.....Z
+000015b0: 0a65 0764 0365 0666 0264 0a64 0b84 0483  .e.d.e.f.d.d....
+000015c0: 015a 0b65 0764 0365 0566 0264 0c64 0d84  .Z.e.d.e.f.d.d..
+000015d0: 0483 015a 0c65 0764 0365 0566 0264 0e64  ...Z.e.d.e.f.d.d
+000015e0: 0f84 0483 015a 0d64 1287 0066 0164 1064  .....Z.d...f.d.d
+000015f0: 1184 0c5a 0e87 0004 005a 0f53 0029 13da  ...Z.....Z.S.)..
+00001600: 0c53 7061 7273 654d 6174 7269 787a b80a  .SparseMatrixz..
+00001610: 2020 2020 4469 6374 696f 6e61 7279 206f      Dictionary o
+00001620: 6620 7468 6520 666f 726d 207b 2878 2c20  f the form {(x, 
+00001630: 7929 3a20 7661 6c75 657d 2e20 4361 6e20  y): value}. Can 
+00001640: 6265 2075 7365 6420 746f 2073 696d 756c  be used to simul
+00001650: 6174 6520 616e 2069 6e66 696e 6974 6520  ate an infinite 
+00001660: 6772 6964 2e0a 2020 2020 4561 6368 2065  grid..    Each e
+00001670: 6e74 7279 2072 6570 7265 7365 6e74 7320  ntry represents 
+00001680: 6120 6365 6c6c 2077 6974 6820 7769 6474  a cell with widt
+00001690: 6820 616e 6420 6865 6967 6874 206f 6620  h and height of 
+000016a0: 3120 2869 2e65 2e20 4e4f 5420 6120 6469  1 (i.e. NOT a di
+000016b0: 6d65 6e73 696f 6e6c 6573 7320 706f 696e  mensionless poin
+000016c0: 7429 0a20 2020 20a9 024e 4e72 0f00 0000  t).    ..NNr....
+000016d0: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
+000016e0: 0003 0000 0043 0000 0073 4c00 0000 7c00  .....C...sL...|.
+000016f0: 721e 7400 7c00 a001 a100 8301 5c02 7d01  r.t.|.......\.}.
+00001700: 7d02 7402 7c01 8301 7403 7c01 8301 6602  }.t.|...t.|...f.
+00001710: 7d03 7402 7c02 8301 7403 7c02 8301 6602  }.t.|...t.|...f.
+00001720: 7d04 7c03 7c04 6602 5300 6401 0400 7d03  }.|.|.f.S.d...}.
+00001730: 7d04 7c03 7c04 6602 5300 2902 7a29 5468  }.|.|.f.S.).z)Th
+00001740: 6520 6d69 6e20 616e 6420 6d61 7820 782f  e min and max x/
+00001750: 7920 636f 6f72 6473 206f 6620 616c 6c20  y coords of all 
+00001760: 656e 7472 6965 7372 8600 0000 2904 7284  entriesr....).r.
+00001770: 0000 00da 046b 6579 7372 1600 0000 7218  .....keysr....r.
+00001780: 0000 0029 05da 0473 656c 66da 0278 73da  ...)...self..xs.
+00001790: 0279 73da 0478 6c69 6dda 0479 6c69 6d72  .ys..xlim..ylimr
+000017a0: 1300 0000 7213 0000 0072 1400 0000 da06  ....r....r......
+000017b0: 6c69 6d69 7473 cc00 0000 730e 0000 0004  limits....s.....
+000017c0: 0310 0110 0110 0108 0308 ff08 017a 1353  .............z.S
+000017d0: 7061 7273 654d 6174 7269 782e 6c69 6d69  parseMatrix.limi
+000017e0: 7473 6301 0000 0000 0000 0000 0000 0005  tsc.............
+000017f0: 0000 0003 0000 0043 0000 0073 4e00 0000  .......C...sN...
+00001800: 7c00 721f 7c00 6a00 5c02 7d01 7d02 7c01  |.r.|.j.\.}.}.|.
+00001810: 6401 1900 7c01 6402 1900 1800 6401 1700  d...|.d.....d...
+00001820: 7d03 7c02 6401 1900 7c02 6402 1900 1800  }.|.d...|.d.....
+00001830: 6401 1700 7d04 7c03 7c04 6602 5300 6402  d...}.|.|.f.S.d.
+00001840: 0400 7d03 7d04 7c03 7c04 6602 5300 2903  ..}.}.|.|.f.S.).
+00001850: 4e72 2600 0000 7201 0000 00a9 0172 8d00  Nr&...r......r..
+00001860: 0000 2905 7288 0000 0072 8b00 0000 728c  ..).r....r....r.
+00001870: 0000 0072 3d00 0000 723e 0000 0072 1300  ...r=...r>...r..
+00001880: 0000 7213 0000 0072 1400 0000 da04 7369  ..r....r......si
+00001890: 7a65 d700 0000 730e 0000 0004 020a 0114  ze....s.........
+000018a0: 0114 0108 0308 ff08 017a 1153 7061 7273  .........z.Spars
+000018b0: 654d 6174 7269 782e 7369 7a65 6301 0000  eMatrix.sizec...
+000018c0: 0000 0000 0000 0000 0003 0000 0002 0000  ................
+000018d0: 0043 0000 00f3 0e00 0000 7c00 6a00 5c02  .C........|.j.\.
+000018e0: 7d01 7d02 7c01 5300 7240 0000 0072 8e00  }.}.|.S.r@...r..
+000018f0: 0000 2903 7288 0000 0072 8b00 0000 da01  ..).r....r......
+00001900: 5f72 1300 0000 7213 0000 0072 1400 0000  _r....r....r....
+00001910: 728b 0000 00e1 0000 00f3 0400 0000 0a02  r...............
+00001920: 0401 7a11 5370 6172 7365 4d61 7472 6978  ..z.SparseMatrix
+00001930: 2e78 6c69 6d63 0100 0000 0000 0000 0000  .xlimc..........
+00001940: 0000 0300 0000 0200 0000 4300 0000 f30e  ..........C.....
+00001950: 0000 007c 006a 005c 027d 017d 027c 0253  ...|.j.\.}.}.|.S
+00001960: 0072 4000 0000 728e 0000 0029 0372 8800  .r@...r....).r..
+00001970: 0000 7291 0000 0072 8c00 0000 7213 0000  ..r....r....r...
+00001980: 0072 1300 0000 7214 0000 0072 8c00 0000  .r....r....r....
+00001990: e600 0000 7292 0000 007a 1153 7061 7273  ....r....z.Spars
+000019a0: 654d 6174 7269 782e 796c 696d 6301 0000  eMatrix.ylimc...
+000019b0: 0000 0000 0000 0000 0003 0000 0002 0000  ................
+000019c0: 0043 0000 0072 9000 0000 7240 0000 00a9  .C...r....r@....
+000019d0: 0172 8f00 0000 2903 7288 0000 0072 3d00  .r....).r....r=.
+000019e0: 0000 7291 0000 0072 1300 0000 7213 0000  ..r....r....r...
+000019f0: 0072 1400 0000 723d 0000 00eb 0000 0072  .r....r=.......r
+00001a00: 9200 0000 7a12 5370 6172 7365 4d61 7472  ....z.SparseMatr
+00001a10: 6978 2e77 6964 7468 6301 0000 0000 0000  ix.widthc.......
+00001a20: 0000 0000 0003 0000 0002 0000 0043 0000  .............C..
+00001a30: 0072 9300 0000 7240 0000 0072 9400 0000  .r....r@...r....
+00001a40: 2903 7288 0000 0072 9100 0000 723e 0000  ).r....r....r>..
+00001a50: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
+00001a60: 723e 0000 00f0 0000 0072 9200 0000 7a13  r>.......r....z.
+00001a70: 5370 6172 7365 4d61 7472 6978 2e68 6569  SparseMatrix.hei
+00001a80: 6768 7463 0100 0000 0000 0000 0000 0000  ghtc............
+00001a90: 0100 0000 0300 0000 0300 0000 730e 0000  ............s...
+00001aa0: 0074 0074 0183 00a0 02a1 0083 0153 0072  .t.t.........S.r
+00001ab0: 4000 0000 2903 7285 0000 00da 0573 7570  @...).r......sup
+00001ac0: 6572 da04 636f 7079 2901 7288 0000 00a9  er..copy).r.....
+00001ad0: 01da 095f 5f63 6c61 7373 5f5f 7213 0000  ...__class__r...
+00001ae0: 0072 1400 0000 7296 0000 00f5 0000 0073  .r....r........s
+00001af0: 0200 0000 0e01 7a11 5370 6172 7365 4d61  ......z.SparseMa
+00001b00: 7472 6978 2e63 6f70 7929 0272 0f00 0000  trix.copy).r....
+00001b10: 7285 0000 0029 10da 085f 5f6e 616d 655f  r....)...__name_
+00001b20: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00001b30: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
+00001b40: 6f63 5f5f 7281 0000 0072 7100 0000 da05  oc__r....rq.....
+00001b50: 4c69 6d69 74da 0870 726f 7065 7274 7972  Limit..propertyr
+00001b60: 8d00 0000 728f 0000 0072 8b00 0000 728c  ....r....r....r.
+00001b70: 0000 0072 3d00 0000 723e 0000 0072 9600  ...r=...r>...r..
+00001b80: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
+00001b90: 5f72 1300 0000 7213 0000 0072 9700 0000  _r....r....r....
+00001ba0: 7214 0000 0072 8500 0000 c400 0000 7320  r....r........s 
+00001bb0: 0000 0008 0004 0114 0502 0218 0102 0a14  ................
+00001bc0: 0102 0910 0102 0410 0102 0410 0102 0410  ................
+00001bd0: 0116 0472 8500 0000 46da 0173 6306 0000  ...r....F..sc...
+00001be0: 0000 0000 0000 0000 0007 0000 0005 0000  ................
+00001bf0: 0043 0000 0073 1e00 0000 7c03 a000 7c00  .C...s....|...|.
+00001c00: 7c05 7c04 a103 7d06 7c01 a001 7c06 7c02  |.|...}.|...|.|.
+00001c10: a102 0100 6400 5300 7240 0000 0029 02da  ....d.S.r@...)..
+00001c20: 0672 656e 6465 7272 5500 0000 2907 72a0  .renderrU...).r.
+00001c30: 0000 0072 3200 0000 da08 706f 7369 7469  ...r2.....positi
+00001c40: 6f6e da04 666f 6e74 7238 0000 00da 0961  on..fontr8.....a
+00001c50: 6e74 6961 6c69 6173 da0b 7465 7874 5f62  ntialias..text_b
+00001c60: 6974 6d61 7072 1300 0000 7213 0000 0072  itmapr....r....r
+00001c70: 1400 0000 da09 6472 6177 5f74 6578 74f9  ......draw_text.
+00001c80: 0000 0073 0400 0000 0e01 1001 72a6 0000  ...s........r...
+00001c90: 0029 0172 2500 0000 7240 0000 0029 024e  .).r%...r@...).N
+00001ca0: 7243 0000 0029 0172 0100 0000 2901 4629  rC...).r....).F)
+00001cb0: 2b72 7700 0000 da04 656e 756d da0b 636f  +rw.....enum..co
+00001cc0: 6c6c 6563 7469 6f6e 7372 0200 0000 da04  llectionsr......
+00001cd0: 6d61 7468 7204 0000 00da 0674 7970 696e  mathr......typin
+00001ce0: 6772 0500 0000 7206 0000 0072 0700 0000  gr....r....r....
+00001cf0: 724a 0000 0072 2800 0000 da0e 7079 6761  rJ...r(.....pyga
+00001d00: 6d65 2e73 7572 6661 6365 7208 0000 00da  me.surfacer.....
+00001d10: 1872 6f62 696e 6761 6d65 2e6f 626a 6563  .robingame.objec
+00001d20: 7473 2e65 6e74 6974 7972 0900 0000 720a  ts.entityr....r.
+00001d30: 0000 00da 0462 6f6f 6c72 1500 0000 7220  .....boolr....r 
+00001d40: 0000 0072 2400 0000 7235 0000 0072 3f00  ...r$...r5...r?.
+00001d50: 0000 7242 0000 0072 5300 0000 7257 0000  ..rB...rS...rW..
+00001d60: 0072 4800 0000 7247 0000 0072 8100 0000  .rH...rG...r....
+00001d70: 7271 0000 0072 6300 0000 7269 0000 0072  rq...rc...ri...r
+00001d80: 7000 0000 7276 0000 0072 7900 0000 727b  p...rv...ry...r{
+00001d90: 0000 0072 8000 0000 7284 0000 00da 0543  ...r....r......C
+00001da0: 6f6f 7264 da04 6469 6374 7285 0000 00da  oord..dictr.....
+00001db0: 0373 7472 72a6 0000 0072 1300 0000 7213  .strr....r....r.
+00001dc0: 0000 0072 1300 0000 7214 0000 00da 083c  ...r....r......<
+00001dd0: 6d6f 6475 6c65 3e01 0000 0073 4000 0000  module>....s@...
+00001de0: 0800 0801 0c01 0c01 1401 0802 0801 0c01  ................
+00001df0: 0403 0c01 0e02 1603 0811 0807 0a11 0a12  ................
+00001e00: 0e0c 0a05 0a09 080d 080b 160c 0a0e 0807  ................
+00001e10: 0805 0808 0807 1604 0805 0c04 1003 1835  ...............5
```

### Comparing `robingame-0.1.0/robingame/animation.py` & `robingame-1.0.1/robingame/animation.py`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/examples/gui_examples/__pycache__/coloured_button_effects.cpython-310.pyc` & `robingame-1.0.1/robingame/examples/gui_examples/__pycache__/coloured_button_effects.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/examples/gui_examples/assets/button-up.aseprite` & `robingame-1.0.1/robingame/examples/gui_examples/assets/button-up.aseprite`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/examples/gui_examples/assets/flashybutton.aseprite` & `robingame-1.0.1/robingame/examples/gui_examples/assets/flashybutton.aseprite`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/examples/gui_examples/assets/flashybutton.png` & `robingame-1.0.1/robingame/examples/gui_examples/assets/flashybutton.png`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/examples/gui_examples/coloured_button_effects.py` & `robingame-1.0.1/robingame/examples/gui_examples/coloured_button_effects.py`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/examples/gui_examples/complicated_on_press_hook.py` & `robingame-1.0.1/robingame/examples/gui_examples/complicated_on_press_hook.py`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/examples/gui_examples/on_press_event.py` & `robingame-1.0.1/robingame/examples/gui_examples/on_press_event.py`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/examples/particle_example.py` & `robingame-1.0.1/robingame/examples/particle_example.py`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/gui/__pycache__/button.cpython-310.pyc` & `robingame-1.0.1/robingame/gui/__pycache__/button.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/gui/__pycache__/menu.cpython-310.pyc` & `robingame-1.0.1/robingame/gui/__pycache__/menu.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/gui/button.py` & `robingame-1.0.1/robingame/gui/button.py`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/gui/menu.py` & `robingame-1.0.1/robingame/gui/menu.py`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/image/utils.py` & `robingame-1.0.1/robingame/image/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,22 +5,40 @@
 import pygame
 from pygame import Surface
 
 from robingame.utils import limit_value
 
 
 def init_display() -> Surface:
+    """
+    Make sure the pygame display is initialised (required for loading images).
+    If the display already exists, return it. If not, generate a new 1x1 pixel display.
+
+    Returns:
+        the pygame display
+    """
     if not pygame.display.get_init():
         pygame.display.init()
         return pygame.display.set_mode((1, 1))
     else:
         return pygame.display.get_surface()
 
 
-def load_image(filename, colorkey=None) -> Surface:
+def load_image(filename: str | Path, colorkey: Color | int = None) -> Surface:
+    """
+    Load an image. Abstracts away some of the pygame pitfalls.
+
+    Args:
+        filename: path to the image file
+        colorkey: sets the color to treat as transparent (like the green in greenscreen).
+            if `-1` is passed, then the color of the top-left pixel will be used.
+
+    Returns:
+        the loaded image
+    """
     init_display()
     try:
         image = pygame.image.load(filename)
     except pygame.error:
         print("Unable to load image:", filename)
         raise
 
@@ -32,49 +50,85 @@
         image.set_colorkey(colorkey, pygame.RLEACCEL)
 
     image = image.convert_alpha()
     return image
 
 
 def not_empty(surface: Surface) -> bool:
-    """Check if a surface has any non-zero pixels. `Surface.get_bounding_rect()` returns the
+    """
+    Check if a surface has any non-zero pixels. `Surface.get_bounding_rect()` returns the
     smallest rectangle on the surface containing data. If the surface is empty, it will return
-    Rect(0, 0, 0, 0), for which `any` returns False"""
+    Rect(0, 0, 0, 0), for which `any` returns False.
+    """
     return any(surface.get_bounding_rect())
 
 
 def empty_image(*args, **kwargs) -> Surface:
+    """
+    Generate an empty Surface with `.convert_alpha()` already called.
+
+    Returns:
+        an empty Surface
+    """
     img = Surface(*args, **kwargs).convert_alpha()
     img.fill((0, 0, 0, 0))
     return img
 
 
 def relative_folder(current_file: str, folder: str) -> Path:
     return Path(current_file).parent.absolute() / folder
 
 
-def pad_alpha(colour_tuple):
+def pad_alpha(colour_tuple: Color | tuple) -> Color:
+    """
+    Add the 4th (alpha) channel to a length 3 color tuple.
+    By default it sets the new alpha channel to full opacity (255).
+
+    Args:
+        colour_tuple:
+
+    Returns:
+        a colour
+    """
     if len(colour_tuple) == 3:
         # if no alpha channel supplied, assume it's full opacity
         return (*colour_tuple, 255)
     elif len(colour_tuple) == 4:
         return colour_tuple
     else:
         raise Exception("bogus colour, man")
 
 
-def brighten_color(color: Color, amount: int) -> Color:
+def brighten_color(color: Color | tuple, amount: int) -> Color:
+    """
+    Increase all channels to brighten a colour.
+    Does not allow values greater than 255.
+
+    Args:
+        color: the input colour
+        amount: how much to increase each channel
+
+    Returns:
+        the output colour
+    """
     color = Color(color)
     r = limit_value(color.r + amount, between=(0, 255))
     g = limit_value(color.g + amount, between=(0, 255))
     b = limit_value(color.b + amount, between=(0, 255))
     return Color(r, g, b, color.a)
 
 
 def brighten(image: Surface, amount: int):
+    """
+    Use `brighten_color` to brighten all pixels in an image by `amount`. \
+
+    Args:
+        image: the input image
+        amount: how much to increase brightness
+    """
     width, height = image.get_size()
     # surface.copy() inherits surface's colorkey; preserving transparency
     new_image = image.copy()
 
     # iterate over all the pixels in the old surface, and write a pixel to the new surface in the
     # corresponding position. If the colour of the present pixel has an entry in the
     # color_mapping dict, then write the new colour instead of the old one.
@@ -86,34 +140,72 @@
                 new_image.set_at((x, y), pygame.Color(*new_color))
             else:
                 new_image.set_at((x, y), pygame.Color(*color))
 
     return new_image
 
 
-def scale_image(image: Surface, scale: float):
-    x_scale = image.get_rect().width * scale
-    y_scale = image.get_rect().height * scale
-    image = pygame.transform.scale(image, (x_scale, y_scale))
+def scale_image(image: Surface, scale: float) -> Surface:
+    """
+    Return a scaled copy of an image.
+
+    Args:
+        image: input image
+        scale: factor by which to scale image
+
+    Returns:
+        output image
+    """
+    width, height = image.get_rect().size
+    image = pygame.transform.scale(image, (width * scale, height * scale))
     return image
 
 
 def scale_images(images: [Surface], scale: float) -> [Surface]:
+    """
+    Apply `scale_image` to a list of images.
+    """
     return [scale_image(image, scale) for image in images]
 
 
-def flip_image(image: Surface, flip_x=False, flip_y=False):
+def flip_image(image: Surface, flip_x: bool = False, flip_y: bool = False) -> Surface:
+    """
+    Return a flipped copy of an image.
+
+    Args:
+        image: input image
+        flip_x: flip horizontally
+        flip_y: flip vertically
+
+    Returns:
+        output image
+    """
     return pygame.transform.flip(image, bool(flip_x), bool(flip_y))
 
 
-def flip_images(images: [Surface], flip_x=False, flip_y=False):
+def flip_images(images: [Surface], flip_x: bool = False, flip_y: bool = False):
+    """
+    Apply `flip_image` to a list of images.
+    """
     return [flip_image(image, flip_x, flip_y) for image in images]
 
 
-def recolor_image(surface: Surface, color_mapping: dict) -> [Surface]:
+def recolor_image(surface: Surface, color_mapping: dict) -> Surface:
+    """
+    Return a recolored copy of an image.
+
+    Args:
+        surface: input image
+        color_mapping: dictionary of old colors (keys) to new colors (values).
+            Unfortunately they have to be RGB tuples, not pygame Colors, because Color is an
+            unhashable type...
+
+    Returns:
+        output image
+    """
     # make sure the colourmap has alpha channel on all colours
     color_mapping = {pad_alpha(k): pad_alpha(v) for k, v in color_mapping.items()}
     width, height = surface.get_size()
     # surface.copy() inherits surface's colorkey; preserving transparency
     new_surface = surface.copy()
 
     # iterate over all the pixels in the old surface, and write a pixel to the new surface in the
@@ -128,32 +220,45 @@
             else:
                 new_surface.set_at((x, y), pygame.Color(*color))
 
     return new_surface
 
 
 def recolor_images(images: [Surface], colormap: dict) -> [Surface]:
+    """
+    Apply `recolor_image` to a list of images.
+    """
     return [recolor_image(image, colormap) for image in images]
 
 
 def load_spritesheet(
     filename: Path | str,
     image_size: (int, int) = None,
-    colorkey=None,
+    colorkey: Color = None,
     num_images: int = 0,
 ) -> [Surface]:
-    """Load the image file. Don't call this until pygame.display has been initiated. Split
-    the spritesheet into images and return a list of images.
+    """
+    Load the image file. Don't call this until pygame.display has been initiated. Split the
+    spritesheet into images and return a list of images.
 
     If image_size is None, load the whole spritesheet as one sprite.
+
+    Args:
+        filename: path to the spritesheet file
+        image_size: size of the individual frames of the spritesheet (in pixels)
+        colorkey: used to set transparency (see `load_image`)
+        num_images: can be used to limit the number of frames loaded (default = load all)
+
+    Returns:
+        a list of images
     """
     filename = Path(filename)
     if not filename.exists():
         raise FileNotFoundError(f"Couldn't find {filename}")
-    sheet = load_image(filename.as_posix(), colorkey)
+    sheet = load_image(filename=filename.as_posix(), colorkey=colorkey)
 
     if image_size:
         width, height = image_size
         num_horizontal = sheet.get_rect().width // width
         num_vertical = sheet.get_rect().height // height
         rects = [
             pygame.Rect((width * i, height * j, width, height))
@@ -165,19 +270,33 @@
         if num_images:
             images = images[:num_images]
     else:
         images = [sheet]
     return images
 
 
-def load_image_sequence(filename: Path | str, colorkey=None, num_images: int = 0) -> [Surface]:
-    """Load a sequence of images."""
-    filename = Path(filename)
-    parent_folder = filename.parent
-    pattern = filename.stem
-    files = glob.glob(f"{parent_folder}/{pattern}*")
+def load_image_sequence(
+    pattern: Path | str,
+    colorkey: Color = None,
+    num_images: int = 0,
+) -> [Surface]:
+    """
+    Load a sequence of images.
+
+    Args:
+        pattern: glob pattern for the image sequence. E.g. if your folder of image contains
+            `"example1.png", "example2.png"`, etc, then your pattern should be `"example*.png"`
+        colorkey: used to recolor images (see `load_image`)
+        num_images: used to limit how many images are loaded (default = load all images that
+            match the pattern)
+
+    Returns:
+        a list of images
+    """
+    pattern = Path(pattern).as_posix()
+    files = glob.glob(pattern)
     if not files:
-        raise FileNotFoundError(f"Couldn't find {filename}")
+        raise FileNotFoundError(f"Couldn't find any images matching pattern '{pattern}'")
     images = [load_image(file, colorkey) for file in files]
     if num_images:
         images = images[:num_images]
     return images
```

### Comparing `robingame-0.1.0/robingame/input/__pycache__/event.cpython-310.pyc` & `robingame-1.0.1/robingame/input/__pycache__/event.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 14 09:02:00 2023 UTC, .py size: 1623 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,141 +1,160 @@
-00000000: 6f0d 0d0a 0000 0000 88a3 6064 5706 0000  o.........`dW...
+00000000: 6f0d 0d0a 0000 0000 0e1d b464 9e07 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 5a06 6400 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
-00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
-00000070: 0100 650b 8300 0100 4700 6406 6407 8400  ..e.....G.d.d...
-00000080: 6407 8302 5a0c 6403 5300 2908 e900 0000  d...Z.d.S.).....
+00000060: 6d09 5a0a 0100 6400 6405 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
+00000070: 0100 650c 8300 0100 4700 6406 6407 8400  ..e.....G.d.d...
+00000080: 6407 8302 5a0d 6403 5300 2908 e900 0000  d...Z.d.S.).....
 00000090: 0029 03da 0964 6174 6163 6c61 7373 da0c  .)...dataclass..
 000000a0: 6973 5f64 6174 6163 6c61 7373 da06 6173  is_dataclass..as
 000000b0: 6469 6374 2901 da05 556e 696f 6e4e 2902  dict)...UnionN).
 000000c0: da09 4576 656e 7454 7970 65da 0545 7665  ..EventType..Eve
 000000d0: 6e74 2901 da0c 696e 6974 5f64 6973 706c  nt)...init_displ
 000000e0: 6179 6300 0000 0000 0000 0000 0000 0000  ayc.............
-000000f0: 0000 0005 0000 0040 0000 0073 5200 0000  .......@...sR...
+000000f0: 0000 0005 0000 0040 0000 0073 6600 0000  .......@...sf...
 00000100: 6500 5a01 6400 5a02 6401 5a03 6700 5a04  e.Z.d.Z.d.Z.g.Z.
 00000110: 6505 6402 6506 6507 6403 6602 1900 6602  e.d.e.e.d.f...f.
 00000120: 6404 6405 8404 8301 5a08 6505 6406 6407  d.d.....Z.e.d.d.
-00000130: 8400 8301 5a09 6505 6408 6409 8400 8301  ....Z.e.d.d.....
-00000140: 5a0a 6505 640a 640b 8400 8301 5a0b 640c  Z.e.d.d.....Z.d.
-00000150: 5300 290d da0a 4576 656e 7451 7565 7565  S.)...EventQueue
-00000160: 7a70 5079 6761 6d65 2773 2070 7967 616d  zpPygame's pygam
-00000170: 652e 6576 656e 742e 6765 7428 2920 6765  e.event.get() ge
-00000180: 7473 2074 6865 2065 7665 6e74 7320 696e  ts the events in
-00000190: 2074 6865 2071 7565 7565 2c20 6275 7420   the queue, but 
-000001a0: 616c 736f 2065 6d70 7469 6573 2074 6865  also empties the
-000001b0: 2071 7565 7565 2e20 5468 6973 0a20 2020   queue. This.   
-000001c0: 2063 6c61 7373 2073 6f6c 7665 7320 7468   class solves th
-000001d0: 6174 da05 6576 656e 7472 0200 0000 6302  at..eventr....c.
-000001e0: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-000001f0: 0000 0043 0000 0073 2e00 0000 7400 7c01  ...C...s....t.|.
-00000200: 8301 720f 7401 7c01 6a02 6601 6900 7403  ..r.t.|.j.f.i.t.
-00000210: 7c01 8301 a401 8e01 7d01 7404 6a05 a006  |.......}.t.j...
-00000220: 7c01 a101 0100 6401 5300 2902 6121 0100  |.....d.S.).a!..
-00000230: 000a 2020 2020 2020 2020 4164 6420 7468  ..        Add th
-00000240: 6520 6576 656e 7420 746f 2070 7967 616d  e event to pygam
-00000250: 6527 7320 6576 656e 7420 7175 6575 652c  e's event queue,
-00000260: 2077 6865 7265 2069 7420 7769 6c6c 2073   where it will s
-00000270: 7461 7920 756e 7469 6c20 7468 6520 2e75  tay until the .u
-00000280: 7064 6174 6528 2920 6d65 7468 6f64 0a20  pdate() method. 
-00000290: 2020 2020 2020 2069 7320 6361 6c6c 6564         is called
-000002a0: 2074 6f20 6c6f 6164 2069 7420 696e 746f   to load it into
-000002b0: 2063 6c73 2e65 7665 6e74 732e 0a0a 2020   cls.events...  
-000002c0: 2020 2020 2020 5468 6973 2070 7265 7665        This preve
-000002d0: 6e74 7320 7261 6365 2063 6f6e 6469 7469  nts race conditi
-000002e0: 6f6e 7320 2f20 6f72 6465 7220 6465 7065  ons / order depe
-000002f0: 6e64 656e 6379 2077 6865 7265 2061 6e20  ndency where an 
-00000300: 6576 656e 7420 6973 2061 6464 6564 2074  event is added t
-00000310: 6f20 7468 6520 6576 656e 740a 2020 2020  o the event.    
-00000320: 2020 2020 7175 6575 6520 616e 6420 7072      queue and pr
-00000330: 6f63 6573 7365 6420 696e 2074 6865 2073  ocessed in the s
-00000340: 616d 6520 7469 636b 2e0a 2020 2020 2020  ame tick..      
-00000350: 2020 4e29 0772 0300 0000 7207 0000 00da    N).r....r.....
-00000360: 0474 7970 6572 0400 0000 da06 7079 6761  .typer......pyga
-00000370: 6d65 720a 0000 00da 0470 6f73 7429 02da  mer......post)..
-00000380: 0363 6c73 720a 0000 00a9 0072 0f00 0000  .clsr......r....
-00000390: fa33 2f68 6f6d 652f 726f 6269 6e2f 636f  .3/home/robin/co
-000003a0: 6465 2f72 6f62 696e 6761 6d65 2f72 6f62  de/robingame/rob
-000003b0: 696e 6761 6d65 2f69 6e70 7574 2f65 7665  ingame/input/eve
-000003c0: 6e74 2e70 79da 0361 6464 1400 0000 7306  nt.py..add....s.
-000003d0: 0000 0008 0916 0110 017a 0e45 7665 6e74  .........z.Event
-000003e0: 5175 6575 652e 6164 6463 0100 0000 0000  Queue.addc......
-000003f0: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00000400: 0000 7310 0000 0074 006a 01a0 02a1 007c  ..s....t.j.....|
-00000410: 005f 0364 0153 0029 027a 7a0a 2020 2020  ._.d.S.).zz.    
-00000420: 2020 2020 5265 6164 2061 6c6c 2074 6865      Read all the
-00000430: 2065 7665 6e74 7320 6672 6f6d 2070 7967   events from pyg
-00000440: 616d 6527 7320 6576 656e 7420 7175 6575  ame's event queu
-00000450: 6520 696e 746f 2063 6c73 2e65 7665 6e74  e into cls.event
-00000460: 730a 2020 2020 2020 2020 2861 6c73 6f20  s.        (also 
-00000470: 636c 6561 7273 2070 7967 616d 6527 7320  clears pygame's 
-00000480: 6576 656e 7420 7175 6575 6529 0a20 2020  event queue).   
-00000490: 2020 2020 204e 2904 720c 0000 0072 0a00       N).r....r..
-000004a0: 0000 da03 6765 74da 0665 7665 6e74 7329  ....get..events)
-000004b0: 0172 0e00 0000 720f 0000 0072 0f00 0000  .r....r....r....
-000004c0: 7210 0000 00da 0675 7064 6174 6521 0000  r......update!..
-000004d0: 0073 0200 0000 1006 7a11 4576 656e 7451  .s......z.EventQ
-000004e0: 7565 7565 2e75 7064 6174 6563 0100 0000  ueue.updatec....
-000004f0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000500: 0b00 0000 7314 0000 0087 0066 0164 0164  ....s......f.d.d
-00000510: 0284 087c 006a 0044 0083 0153 0029 034e  ...|.j.D...S.).N
-00000520: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000530: 0006 0000 0013 0000 0073 2a00 0000 6700  .........s*...g.
-00000540: 7c00 5d11 8900 7400 8700 6601 6400 6401  |.]...t...f.d.d.
-00000550: 8408 8801 a001 a100 4400 8301 8301 7202  ........D.....r.
-00000560: 8800 9102 7102 5300 2902 6301 0000 0000  ....q.S.).c.....
-00000570: 0000 0000 0000 0003 0000 0005 0000 0033  ...............3
-00000580: 0000 0073 2400 0000 8100 7c00 5d0d 5c02  ...s$.....|.].\.
-00000590: 7d01 7d02 7400 8800 7c01 6400 8303 7c02  }.}.t...|.d...|.
-000005a0: 6b02 5600 0100 7102 6400 5300 2901 4e29  k.V...q.d.S.).N)
-000005b0: 01da 0767 6574 6174 7472 2903 da02 2e30  ...getattr)....0
-000005c0: da09 6174 7472 6962 7574 65da 0576 616c  ..attribute..val
-000005d0: 7565 a901 720a 0000 0072 0f00 0000 7210  ue..r....r....r.
-000005e0: 0000 00da 093c 6765 6e65 7870 723e 2e00  .....<genexpr>..
-000005f0: 0000 7304 0000 0002 8022 007a 2f45 7665  ..s......".z/Eve
-00000600: 6e74 5175 6575 652e 6669 6c74 6572 2e3c  ntQueue.filter.<
-00000610: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00000620: 703e 2e3c 6765 6e65 7870 723e 2902 da03  p>.<genexpr>)...
-00000630: 616c 6cda 0569 7465 6d73 2901 7216 0000  all..items).r...
-00000640: 00a9 01da 066b 7761 7267 7372 1900 0000  .....kwargsr....
-00000650: 7210 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
-00000660: 3e2b 0000 0073 0c00 0000 0600 0202 1801  >+...s..........
-00000670: 02fd 0201 06ff 7a25 4576 656e 7451 7565  ......z%EventQue
-00000680: 7565 2e66 696c 7465 722e 3c6c 6f63 616c  ue.filter.<local
-00000690: 733e 2e3c 6c69 7374 636f 6d70 3e29 0172  s>.<listcomp>).r
-000006a0: 1300 0000 a902 720e 0000 0072 1e00 0000  ......r....r....
-000006b0: 720f 0000 0072 1d00 0000 7210 0000 00da  r....r....r.....
-000006c0: 0666 696c 7465 7229 0000 0073 0600 0000  .filter)...s....
-000006d0: 0a02 0402 06fe 7a11 4576 656e 7451 7565  ......z.EventQue
-000006e0: 7565 2e66 696c 7465 7263 0100 0000 0000  ue.filterc......
-000006f0: 0000 0000 0000 0200 0000 0800 0000 4b00  ..............K.
-00000700: 0000 732c 0000 007a 0b7c 006a 0064 0269  ..s,...z.|.j.d.i
-00000710: 007c 01a4 018e 0164 0119 0057 0053 0004  .|.....d...W.S..
-00000720: 0074 0179 1501 0001 0001 0059 0064 0053  .t.y.......Y.d.S
-00000730: 0077 0029 034e 7201 0000 0072 0f00 0000  .w.).Nr....r....
-00000740: 2902 7221 0000 00da 0a49 6e64 6578 4572  ).r!.....IndexEr
-00000750: 726f 7272 2000 0000 720f 0000 0072 0f00  rorr ...r....r..
-00000760: 0000 7210 0000 0072 1200 0000 3100 0000  ..r....r....1...
-00000770: 730a 0000 0002 0216 010c 0106 0102 ff7a  s..............z
-00000780: 0e45 7665 6e74 5175 6575 652e 6765 744e  .EventQueue.getN
-00000790: 290c da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-000007a0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000007b0: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
-000007c0: 1300 0000 da0b 636c 6173 736d 6574 686f  ......classmetho
-000007d0: 6472 0500 0000 7206 0000 0072 1100 0000  dr....r....r....
-000007e0: 7214 0000 0072 2100 0000 7212 0000 0072  r....r!...r....r
-000007f0: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-00000800: 0000 0072 0900 0000 0c00 0000 7316 0000  ...r........s...
-00000810: 0008 0004 0104 0502 0218 0102 0c0a 0102  ................
-00000820: 070a 0102 070e 0172 0900 0000 290d da0b  .......r....)...
-00000830: 6461 7461 636c 6173 7365 7372 0200 0000  dataclassesr....
-00000840: 7203 0000 0072 0400 0000 da06 7479 7069  r....r......typi
-00000850: 6e67 7205 0000 0072 0c00 0000 da0c 7079  ngr....r......py
-00000860: 6761 6d65 2e65 7665 6e74 7206 0000 0072  game.eventr....r
-00000870: 0700 0000 da0f 726f 6269 6e67 616d 652e  ......robingame.
-00000880: 696d 6167 6572 0800 0000 7209 0000 0072  imager....r....r
-00000890: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-000008a0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000008b0: 0073 0e00 0000 1400 0c01 0802 1001 0c02  .s..............
-000008c0: 0602 1203                                ....
+00000130: 8400 8301 5a09 6505 6408 650a 6507 1900  ....Z.e.d.e.e...
+00000140: 6602 6409 640a 8404 8301 5a0b 6505 6408  f.d.d.....Z.e.d.
+00000150: 6507 640b 4200 6602 640c 640d 8404 8301  e.d.B.f.d.d.....
+00000160: 5a0c 640b 5300 290e da0a 4576 656e 7451  Z.d.S.)...EventQ
+00000170: 7565 7565 7abf 0a20 2020 2050 7967 616d  ueuez..    Pygam
+00000180: 6527 7320 7079 6761 6d65 2e65 7665 6e74  e's pygame.event
+00000190: 2e67 6574 2829 2065 6d70 7469 6573 2074  .get() empties t
+000001a0: 6865 2071 7565 7565 2c20 7768 6963 6820  he queue, which 
+000001b0: 6d61 6b65 7320 6974 2069 6d70 6f73 7369  makes it impossi
+000001c0: 626c 6520 746f 206c 6973 7465 6e20 746f  ble to listen to
+000001d0: 2065 7665 6e74 730a 2020 2020 696e 206d   events.    in m
+000001e0: 6f72 6520 7468 616e 206f 6e65 206c 6f63  ore than one loc
+000001f0: 6174 696f 6e2e 2054 6869 7320 636c 6173  ation. This clas
+00000200: 7320 736f 6c76 6573 2074 6861 7420 7769  s solves that wi
+00000210: 7468 2061 2073 6f72 7420 6f66 2073 696e  th a sort of sin
+00000220: 676c 6574 6f6e 2061 7070 726f 6163 682e  gleton approach.
+00000230: 0a20 2020 20da 0565 7665 6e74 7202 0000  .    ..eventr...
+00000240: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+00000250: 0000 0500 0000 4300 0000 732e 0000 0074  ......C...s....t
+00000260: 007c 0183 0172 0f74 017c 016a 0266 0169  .|...r.t.|.j.f.i
+00000270: 0074 037c 0183 01a4 018e 017d 0174 046a  .t.|.......}.t.j
+00000280: 05a0 067c 01a1 0101 0064 0153 0029 0261  ...|.....d.S.).a
+00000290: dd01 0000 0a20 2020 2020 2020 2041 6464  .....        Add
+000002a0: 2074 6865 2065 7665 6e74 2074 6f20 7079   the event to py
+000002b0: 6761 6d65 2773 2065 7665 6e74 2071 7565  game's event que
+000002c0: 7565 2c20 7768 6572 6520 6974 2077 696c  ue, where it wil
+000002d0: 6c20 7374 6179 2075 6e74 696c 2074 6865  l stay until the
+000002e0: 202e 7570 6461 7465 2829 206d 6574 686f   .update() metho
+000002f0: 640a 2020 2020 2020 2020 6973 2063 616c  d.        is cal
+00000300: 6c65 6420 746f 206c 6f61 6420 6974 2069  led to load it i
+00000310: 6e74 6f20 636c 732e 6576 656e 7473 2e0a  nto cls.events..
+00000320: 0a20 2020 2020 2020 2054 6869 7320 7072  .        This pr
+00000330: 6576 656e 7473 2072 6163 6520 636f 6e64  events race cond
+00000340: 6974 696f 6e73 202f 206f 7264 6572 2064  itions / order d
+00000350: 6570 656e 6465 6e63 7920 7768 6572 6520  ependency where 
+00000360: 616e 2065 7665 6e74 2069 7320 6164 6465  an event is adde
+00000370: 6420 746f 2074 6865 2065 7665 6e74 0a20  d to the event. 
+00000380: 2020 2020 2020 2071 7565 7565 2061 6e64         queue and
+00000390: 2070 726f 6365 7373 6564 2069 6e20 7468   processed in th
+000003a0: 6520 7361 6d65 2074 6963 6b2e 0a0a 2020  e same tick...  
+000003b0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+000003c0: 2020 2020 2020 2020 6576 656e 743a 206f          event: o
+000003d0: 626a 6563 7420 7265 7072 6573 656e 7469  bject representi
+000003e0: 6e67 2074 6865 2065 7665 6e74 2e0a 2020  ng the event..  
+000003f0: 2020 2020 2020 2020 2020 2020 2020 4361                Ca
+00000400: 6e20 6265 2061 2060 7079 6761 6d65 2e45  n be a `pygame.E
+00000410: 7665 6e74 602c 206f 7220 6120 6461 7461  vent`, or a data
+00000420: 636c 6173 7320 7769 7468 0a20 2020 2020  class with.     
+00000430: 2020 2020 2020 2020 2020 2061 7474 7269             attri
+00000440: 6275 7465 2060 7479 7065 203d 2070 7967  bute `type = pyg
+00000450: 616d 652e 6576 656e 742e 6375 7374 6f6d  ame.event.custom
+00000460: 5f74 7970 6528 2960 0a20 2020 2020 2020  _type()`.       
+00000470: 204e 2907 7203 0000 00da 0b50 7967 616d   N).r......Pygam
+00000480: 6545 7665 6e74 da04 7479 7065 7204 0000  eEvent..typer...
+00000490: 00da 0670 7967 616d 6572 0a00 0000 da04  ...pygamer......
+000004a0: 706f 7374 2902 da03 636c 7372 0a00 0000  post)...clsr....
+000004b0: a900 7210 0000 00fa 332f 686f 6d65 2f72  ..r.....3/home/r
+000004c0: 6f62 696e 2f63 6f64 652f 726f 6269 6e67  obin/code/robing
+000004d0: 616d 652f 726f 6269 6e67 616d 652f 696e  ame/robingame/in
+000004e0: 7075 742f 6576 656e 742e 7079 da03 6164  put/event.py..ad
+000004f0: 6416 0000 0073 0600 0000 080e 1601 1001  d....s..........
+00000500: 7a0e 4576 656e 7451 7565 7565 2e61 6464  z.EventQueue.add
+00000510: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000520: 0002 0000 0043 0000 0073 1000 0000 7400  .....C...s....t.
+00000530: 6a01 a002 a100 7c00 5f03 6401 5300 2902  j.....|._.d.S.).
+00000540: 7a7a 0a20 2020 2020 2020 2052 6561 6420  zz.        Read 
+00000550: 616c 6c20 7468 6520 6576 656e 7473 2066  all the events f
+00000560: 726f 6d20 7079 6761 6d65 2773 2065 7665  rom pygame's eve
+00000570: 6e74 2071 7565 7565 2069 6e74 6f20 636c  nt queue into cl
+00000580: 732e 6576 656e 7473 0a20 2020 2020 2020  s.events.       
+00000590: 2028 616c 736f 2063 6c65 6172 7320 7079   (also clears py
+000005a0: 6761 6d65 2773 2065 7665 6e74 2071 7565  game's event que
+000005b0: 7565 290a 2020 2020 2020 2020 4e29 0472  ue).        N).r
+000005c0: 0d00 0000 720a 0000 00da 0367 6574 da06  ....r......get..
+000005d0: 6576 656e 7473 2901 720f 0000 0072 1000  events).r....r..
+000005e0: 0000 7210 0000 0072 1100 0000 da06 7570  ..r....r......up
+000005f0: 6461 7465 2800 0000 7302 0000 0010 067a  date(...s......z
+00000600: 1145 7665 6e74 5175 6575 652e 7570 6461  .EventQueue.upda
+00000610: 7465 da06 7265 7475 726e 6301 0000 0000  te..returnc.....
+00000620: 0000 0000 0000 0002 0000 0003 0000 000b  ................
+00000630: 0000 0073 1400 0000 8700 6601 6401 6402  ...s......f.d.d.
+00000640: 8408 7c00 6a00 4400 8301 5300 2903 4e63  ..|.j.D...S.).Nc
+00000650: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000660: 0600 0000 1300 0000 732a 0000 0067 007c  ........s*...g.|
+00000670: 005d 1189 0074 0087 0066 0164 0064 0184  .]...t...f.d.d..
+00000680: 0888 01a0 01a1 0044 0083 0183 0172 0288  .......D.....r..
+00000690: 0091 0271 0253 0029 0263 0100 0000 0000  ...q.S.).c......
+000006a0: 0000 0000 0000 0300 0000 0500 0000 3300  ..............3.
+000006b0: 0000 7324 0000 0081 007c 005d 0d5c 027d  ..s$.....|.].\.}
+000006c0: 017d 0274 0088 007c 0164 0083 037c 026b  .}.t...|.d...|.k
+000006d0: 0256 0001 0071 0264 0053 0029 014e 2901  .V...q.d.S.).N).
+000006e0: da07 6765 7461 7474 7229 03da 022e 30da  ..getattr)....0.
+000006f0: 0961 7474 7269 6275 7465 da05 7661 6c75  .attribute..valu
+00000700: 65a9 0172 0a00 0000 7210 0000 0072 1100  e..r....r....r..
+00000710: 0000 da09 3c67 656e 6578 7072 3e35 0000  ....<genexpr>5..
+00000720: 0073 0400 0000 0280 2200 7a2f 4576 656e  .s......".z/Even
+00000730: 7451 7565 7565 2e66 696c 7465 722e 3c6c  tQueue.filter.<l
+00000740: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00000750: 3e2e 3c67 656e 6578 7072 3e29 02da 0361  >.<genexpr>)...a
+00000760: 6c6c da05 6974 656d 7329 0172 1800 0000  ll..items).r....
+00000770: a901 da06 6b77 6172 6773 721b 0000 0072  ....kwargsr....r
+00000780: 1100 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
+00000790: 3200 0000 730c 0000 0006 0002 0218 0102  2...s...........
+000007a0: fd02 0106 ff7a 2545 7665 6e74 5175 6575  .....z%EventQueu
+000007b0: 652e 6669 6c74 6572 2e3c 6c6f 6361 6c73  e.filter.<locals
+000007c0: 3e2e 3c6c 6973 7463 6f6d 703e 2901 7214  >.<listcomp>).r.
+000007d0: 0000 00a9 0272 0f00 0000 7220 0000 0072  .....r....r ...r
+000007e0: 1000 0000 721f 0000 0072 1100 0000 da06  ....r....r......
+000007f0: 6669 6c74 6572 3000 0000 7306 0000 000a  filter0...s.....
+00000800: 0204 0206 fe7a 1145 7665 6e74 5175 6575  .....z.EventQueu
+00000810: 652e 6669 6c74 6572 4e63 0100 0000 0000  e.filterNc......
+00000820: 0000 0000 0000 0200 0000 0800 0000 4b00  ..............K.
+00000830: 0000 732c 0000 007a 0b7c 006a 0064 0269  ..s,...z.|.j.d.i
+00000840: 007c 01a4 018e 0164 0119 0057 0053 0004  .|.....d...W.S..
+00000850: 0074 0179 1501 0001 0001 0059 0064 0053  .t.y.......Y.d.S
+00000860: 0077 0029 034e 7201 0000 0072 1000 0000  .w.).Nr....r....
+00000870: 2902 7223 0000 00da 0a49 6e64 6578 4572  ).r#.....IndexEr
+00000880: 726f 7272 2200 0000 7210 0000 0072 1000  rorr"...r....r..
+00000890: 0000 7211 0000 0072 1300 0000 3800 0000  ..r....r....8...
+000008a0: 730a 0000 0002 0216 010c 0106 0102 ff7a  s..............z
+000008b0: 0e45 7665 6e74 5175 6575 652e 6765 7429  .EventQueue.get)
+000008c0: 0dda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+000008d0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+000008e0: 616d 655f 5fda 075f 5f64 6f63 5f5f 7214  ame__..__doc__r.
+000008f0: 0000 00da 0b63 6c61 7373 6d65 7468 6f64  .....classmethod
+00000900: 7205 0000 0072 0600 0000 7212 0000 0072  r....r....r....r
+00000910: 1500 0000 da04 6c69 7374 7223 0000 0072  ......listr#...r
+00000920: 1300 0000 7210 0000 0072 1000 0000 7210  ....r....r....r.
+00000930: 0000 0072 1100 0000 7209 0000 000c 0000  ...r....r.......
+00000940: 0073 1600 0000 0800 0401 0407 0202 1801  .s..............
+00000950: 0211 0a01 0207 1401 0207 1801 7209 0000  ............r...
+00000960: 0029 0eda 0b64 6174 6163 6c61 7373 6573  .)...dataclasses
+00000970: 7202 0000 0072 0300 0000 7204 0000 00da  r....r....r.....
+00000980: 0674 7970 696e 6772 0500 0000 720d 0000  .typingr....r...
+00000990: 00da 0c70 7967 616d 652e 6576 656e 7472  ...pygame.eventr
+000009a0: 0600 0000 7207 0000 0072 0b00 0000 da0f  ....r....r......
+000009b0: 726f 6269 6e67 616d 652e 696d 6167 6572  robingame.imager
+000009c0: 0800 0000 7209 0000 0072 1000 0000 7210  ....r....r....r.
+000009d0: 0000 0072 1000 0000 7211 0000 00da 083c  ...r....r......<
+000009e0: 6d6f 6475 6c65 3e01 0000 0073 0e00 0000  module>....s....
+000009f0: 1400 0c01 0802 1001 0c02 0602 1203       ..............
```

### Comparing `robingame-0.1.0/robingame/input/__pycache__/gamecube.cpython-310.pyc` & `robingame-1.0.1/robingame/input/__pycache__/gamecube.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/input/__pycache__/keyboard.cpython-310.pyc` & `robingame-1.0.1/robingame/input/__pycache__/keyboard.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 14 09:02:00 2023 UTC, .py size: 278 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,67 @@
-00000000: 6f0d 0d0a 0000 0000 88a3 6064 1601 0000  o.........`d....
+00000000: 6f0d 0d0a 0000 0000 0e1d b464 0402 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6502 8303  ..G.d.d...d.e...
 00000050: 5a03 6401 5300 2905 e900 0000 004e 2901  Z.d.S.)......N).
 00000060: da0a 496e 7075 7451 7565 7565 6300 0000  ..InputQueuec...
 00000070: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00000080: 0040 0000 0073 1e00 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000090: 5a02 6401 6503 6504 1900 6602 6402 6403  Z.d.e.e...f.d.d.
-000000a0: 8404 5a05 6404 5300 2905 da12 4b65 7962  ..Z.d.S.)...Keyb
-000000b0: 6f61 7264 496e 7075 7451 7565 7565 da06  oardInputQueue..
-000000c0: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
-000000d0: 0000 0001 0000 0005 0000 0003 0000 0073  ...............s
-000000e0: 2800 0000 7400 6a01 a002 a100 8900 7403  (...t.j.......t.
-000000f0: 8700 6601 6401 6402 8408 7404 7405 8800  ..f.d.d...t.t...
-00000100: 8301 8301 4400 8301 8301 5300 2903 4e63  ....D.....S.).Nc
-00000110: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000120: 0300 0000 3300 0000 7318 0000 0081 007c  ....3...s......|
-00000130: 005d 077d 0188 007c 0119 0056 0001 0071  .].}...|...V...q
-00000140: 0264 0053 0029 014e a900 2902 da02 2e30  .d.S.).N..)....0
-00000150: da02 6969 a901 da10 7363 616e 636f 6465  ..ii....scancode
-00000160: 5f77 7261 7070 6572 7205 0000 00fa 362f  _wrapperr.....6/
-00000170: 686f 6d65 2f72 6f62 696e 2f63 6f64 652f  home/robin/code/
-00000180: 726f 6269 6e67 616d 652f 726f 6269 6e67  robingame/robing
-00000190: 616d 652f 696e 7075 742f 6b65 7962 6f61  ame/input/keyboa
-000001a0: 7264 2e70 79da 093c 6765 6e65 7870 723e  rd.py..<genexpr>
-000001b0: 0900 0000 7304 0000 0002 8016 007a 344b  ....s........z4K
-000001c0: 6579 626f 6172 6449 6e70 7574 5175 6575  eyboardInputQueu
-000001d0: 652e 6765 745f 6e65 775f 7661 6c75 6573  e.get_new_values
-000001e0: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-000001f0: 7072 3e29 06da 0670 7967 616d 65da 036b  pr>)...pygame..k
-00000200: 6579 da0b 6765 745f 7072 6573 7365 64da  ey..get_pressed.
-00000210: 0574 7570 6c65 da05 7261 6e67 65da 036c  .tuple..range..l
-00000220: 656e 2901 da04 7365 6c66 7205 0000 0072  en)...selfr....r
-00000230: 0800 0000 720a 0000 00da 0e67 6574 5f6e  ....r......get_n
-00000240: 6577 5f76 616c 7565 7307 0000 0073 0400  ew_values....s..
-00000250: 0000 0a01 1e01 7a21 4b65 7962 6f61 7264  ......z!Keyboard
-00000260: 496e 7075 7451 7565 7565 2e67 6574 5f6e  InputQueue.get_n
-00000270: 6577 5f76 616c 7565 734e 2906 da08 5f5f  ew_valuesN)...__
-00000280: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000290: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-000002a0: 720f 0000 00da 0369 6e74 7213 0000 0072  r......intr....r
-000002b0: 0500 0000 7205 0000 0072 0500 0000 720a  ....r....r....r.
-000002c0: 0000 0072 0300 0000 0600 0000 7304 0000  ...r........s...
-000002d0: 0008 0016 0172 0300 0000 2904 720c 0000  .....r....).r...
-000002e0: 00da 1572 6f62 696e 6761 6d65 2e69 6e70  ...robingame.inp
-000002f0: 7574 2e71 7565 7565 7202 0000 0072 0300  ut.queuer....r..
-00000300: 0000 7205 0000 0072 0500 0000 7205 0000  ..r....r....r...
-00000310: 0072 0a00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000320: 0100 0000 7306 0000 0008 000c 0214 03    ....s..........
+00000080: 0040 0000 0073 2200 0000 6500 5a01 6400  .@...s"...e.Z.d.
+00000090: 5a02 6401 5a03 6402 6504 6505 1900 6602  Z.d.Z.d.e.e...f.
+000000a0: 6403 6404 8404 5a06 6405 5300 2906 da12  d.d...Z.d.S.)...
+000000b0: 4b65 7962 6f61 7264 496e 7075 7451 7565  KeyboardInputQue
+000000c0: 7565 7ae2 0a20 2020 2054 7261 636b 7320  uez..    Tracks 
+000000d0: 7468 6520 6869 7374 6f72 7920 6f66 2074  the history of t
+000000e0: 6865 206b 6579 626f 6172 6420 696e 7075  he keyboard inpu
+000000f0: 7420 6368 616e 6e65 6c73 2e0a 0a20 2020  t channels...   
+00000100: 2045 7861 6d70 6c65 3a0a 2020 2020 2020   Example:.      
+00000110: 2020 6060 600a 2020 2020 2020 2020 6b65    ```.        ke
+00000120: 7962 6f61 7264 5f68 616e 646c 6572 203d  yboard_handler =
+00000130: 204b 6579 626f 6172 6449 6e70 7574 5175   KeyboardInputQu
+00000140: 6575 6528 290a 2020 2020 2020 2020 6966  eue().        if
+00000150: 206b 6579 626f 6172 645f 6861 6e64 6c65   keyboard_handle
+00000160: 722e 6973 5f70 7265 7373 6564 2870 7967  r.is_pressed(pyg
+00000170: 616d 652e 4b5f 4553 4329 3a0a 2020 2020  ame.K_ESC):.    
+00000180: 2020 2020 2020 2020 7079 6761 6d65 2e71          pygame.q
+00000190: 7569 7428 290a 2020 2020 2020 2020 6060  uit().        ``
+000001a0: 600a 2020 2020 da06 7265 7475 726e 6301  `.    ..returnc.
+000001b0: 0000 0000 0000 0000 0000 0001 0000 0005  ................
+000001c0: 0000 0003 0000 0073 2800 0000 7400 6a01  .......s(...t.j.
+000001d0: a002 a100 8900 7403 8700 6601 6401 6402  ......t...f.d.d.
+000001e0: 8408 7404 7405 8800 8301 8301 4400 8301  ..t.t.......D...
+000001f0: 8301 5300 2903 4e63 0100 0000 0000 0000  ..S.).Nc........
+00000200: 0000 0000 0200 0000 0300 0000 3300 0000  ............3...
+00000210: 7318 0000 0081 007c 005d 077d 0188 007c  s......|.].}...|
+00000220: 0119 0056 0001 0071 0264 0053 0029 014e  ...V...q.d.S.).N
+00000230: a900 2902 da02 2e30 da02 6969 a901 da10  ..)....0..ii....
+00000240: 7363 616e 636f 6465 5f77 7261 7070 6572  scancode_wrapper
+00000250: 7205 0000 00fa 362f 686f 6d65 2f72 6f62  r.....6/home/rob
+00000260: 696e 2f63 6f64 652f 726f 6269 6e67 616d  in/code/robingam
+00000270: 652f 726f 6269 6e67 616d 652f 696e 7075  e/robingame/inpu
+00000280: 742f 6b65 7962 6f61 7264 2e70 79da 093c  t/keyboard.py..<
+00000290: 6765 6e65 7870 723e 1400 0000 7304 0000  genexpr>....s...
+000002a0: 0002 8016 007a 344b 6579 626f 6172 6449  .....z4KeyboardI
+000002b0: 6e70 7574 5175 6575 652e 6765 745f 6e65  nputQueue.get_ne
+000002c0: 775f 7661 6c75 6573 2e3c 6c6f 6361 6c73  w_values.<locals
+000002d0: 3e2e 3c67 656e 6578 7072 3e29 06da 0670  >.<genexpr>)...p
+000002e0: 7967 616d 65da 036b 6579 da0b 6765 745f  ygame..key..get_
+000002f0: 7072 6573 7365 64da 0574 7570 6c65 da05  pressed..tuple..
+00000300: 7261 6e67 65da 036c 656e 2901 da04 7365  range..len)...se
+00000310: 6c66 7205 0000 0072 0800 0000 720a 0000  lfr....r....r...
+00000320: 00da 0e67 6574 5f6e 6577 5f76 616c 7565  ...get_new_value
+00000330: 7312 0000 0073 0400 0000 0a01 1e01 7a21  s....s........z!
+00000340: 4b65 7962 6f61 7264 496e 7075 7451 7565  KeyboardInputQue
+00000350: 7565 2e67 6574 5f6e 6577 5f76 616c 7565  ue.get_new_value
+00000360: 734e 2907 da08 5f5f 6e61 6d65 5f5f da0a  sN)...__name__..
+00000370: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000380: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+00000390: 5f72 0f00 0000 da03 696e 7472 1300 0000  _r......intr....
+000003a0: 7205 0000 0072 0500 0000 7205 0000 0072  r....r....r....r
+000003b0: 0a00 0000 7203 0000 0006 0000 0073 0600  ....r........s..
+000003c0: 0000 0800 0401 160b 7203 0000 0029 0472  ........r....).r
+000003d0: 0c00 0000 da15 726f 6269 6e67 616d 652e  ......robingame.
+000003e0: 696e 7075 742e 7175 6575 6572 0200 0000  input.queuer....
+000003f0: 7203 0000 0072 0500 0000 7205 0000 0072  r....r....r....r
+00000400: 0500 0000 720a 0000 00da 083c 6d6f 6475  ....r......<modu
+00000410: 6c65 3e01 0000 0073 0600 0000 0800 0c02  le>....s........
+00000420: 1403                                     ..
```

### Comparing `robingame-0.1.0/robingame/input/__pycache__/queue.cpython-310.pyc` & `robingame-1.0.1/robingame/input/__pycache__/queue.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 14 09:02:00 2023 UTC, .py size: 3194 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,267 +1,343 @@
-00000000: 6f0d 0d0a 0000 0000 88a3 6064 7a0c 0000  o.........`dz...
+00000000: 6f0d 0d0a 0000 0000 0e1d b464 aa12 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
+00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
-00000050: 6504 8303 5a05 4700 6405 6406 8400 6406  e...Z.G.d.d...d.
-00000060: 6501 8303 5a06 6407 5300 2908 e900 0000  e...Z.d.S.).....
-00000070: 0029 01da 0564 6571 7565 2901 da0b 636f  .)...deque)...co
-00000080: 756e 745f 6564 6765 7363 0000 0000 0000  unt_edgesc......
-00000090: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-000000a0: 0000 731e 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-000000b0: 015a 0364 0265 0466 0264 0364 0484 045a  .Z.d.e.f.d.d...Z
-000000c0: 0564 0553 0029 06da 0545 6d70 7479 7a82  .d.S.)...Emptyz.
-000000d0: 4d6f 636b 2074 7570 6c65 206f 6620 302f  Mock tuple of 0/
-000000e0: 3173 2074 6861 7420 616c 7761 7973 2072  1s that always r
-000000f0: 6574 7572 6e73 2061 2030 206e 6f20 6d61  eturns a 0 no ma
-00000100: 7474 6572 2074 6865 2069 6e64 6578 2e20  tter the index. 
-00000110: 5468 6973 2069 7320 7573 6564 2074 6f0a  This is used to.
-00000120: 2020 2020 7370 6f6f 6620 616e 2065 6d70      spoof an emp
-00000130: 7479 2070 7967 616d 652e 6b65 792e 6765  ty pygame.key.ge
-00000140: 745f 7072 6573 7365 6428 2920 7475 706c  t_pressed() tupl
-00000150: 652e da06 7265 7475 726e 6301 0000 0000  e...returnc.....
-00000160: 0000 0000 0000 0003 0000 0001 0000 004f  ...............O
-00000170: 0000 0073 0400 0000 6401 5300 2902 4e72  ...s....d.S.).Nr
-00000180: 0100 0000 a900 2903 da04 7365 6c66 da04  ......)...self..
-00000190: 6172 6773 da06 6b77 6172 6773 7206 0000  args..kwargsr...
-000001a0: 0072 0600 0000 fa33 2f68 6f6d 652f 726f  .r.....3/home/ro
-000001b0: 6269 6e2f 636f 6465 2f72 6f62 696e 6761  bin/code/robinga
-000001c0: 6d65 2f72 6f62 696e 6761 6d65 2f69 6e70  me/robingame/inp
-000001d0: 7574 2f71 7565 7565 2e70 79da 0b5f 5f67  ut/queue.py..__g
-000001e0: 6574 6974 656d 5f5f 0a00 0000 7302 0000  etitem__....s...
-000001f0: 0004 017a 1145 6d70 7479 2e5f 5f67 6574  ...z.Empty.__get
-00000200: 6974 656d 5f5f 4e29 06da 085f 5f6e 616d  item__N)...__nam
-00000210: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000220: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
-00000230: 5f64 6f63 5f5f da03 696e 7472 0b00 0000  _doc__..intr....
-00000240: 7206 0000 0072 0600 0000 7206 0000 0072  r....r....r....r
-00000250: 0a00 0000 7204 0000 0006 0000 0073 0600  ....r........s..
-00000260: 0000 0800 0401 1203 7204 0000 0063 0000  ........r....c..
-00000270: 0000 0000 0000 0000 0000 0000 0000 0400  ................
-00000280: 0000 0000 0000 73b4 0000 0065 005a 0164  ......s....e.Z.d
-00000290: 005a 0264 015a 0364 1c87 0066 0164 0364  .Z.d.Z.d...f.d.d
-000002a0: 0484 095a 0464 0565 0565 0619 0066 0264  ...Z.d.e.e...f.d
-000002b0: 0664 0784 045a 0764 0864 0984 005a 0864  .d...Z.d.d...Z.d
-000002c0: 0565 0565 0619 0066 0264 0a64 0b84 045a  .e.e...f.d.d...Z
-000002d0: 0964 0565 0565 0619 0066 0264 0c64 0d84  .d.e.e...f.d.d..
-000002e0: 045a 0a64 0565 0565 0619 0066 0264 0e64  .Z.d.e.e...f.d.d
-000002f0: 0f84 045a 0b64 0565 0666 0264 1064 1184  ...Z.d.e.f.d.d..
-00000300: 045a 0c64 0565 0666 0264 1264 1384 045a  .Z.d.e.f.d.d...Z
-00000310: 0d64 0565 0666 0264 1464 1584 045a 0e64  .d.e.f.d.d...Z.d
-00000320: 1664 1784 005a 0f64 1864 1984 005a 1064  .d...Z.d.d...Z.d
-00000330: 1a64 1b84 005a 1187 0004 005a 1253 0029  .d...Z.....Z.S.)
-00000340: 1dda 0a49 6e70 7574 5175 6575 657a c10a  ...InputQueuez..
-00000350: 2020 2020 5072 6f76 6964 6573 2061 6464      Provides add
-00000360: 6974 696f 6e61 6c20 6675 6e63 7469 6f6e  itional function
-00000370: 616c 6974 7920 6265 796f 6e64 2070 7967  ality beyond pyg
-00000380: 616d 652e 6b65 792e 6765 745f 7072 6573  ame.key.get_pres
-00000390: 7365 6428 292e 0a20 2020 202d 204d 6169  sed()..    - Mai
-000003a0: 6e74 6169 6e73 2061 2062 7566 6665 7220  ntains a buffer 
-000003b0: 6f66 2074 6865 206c 6173 7420 6665 7720  of the last few 
-000003c0: 696e 7075 7473 0a20 2020 202d 2043 616c  inputs.    - Cal
-000003d0: 6375 6c61 7465 7320 7768 6963 6820 6b65  culates which ke
-000003e0: 7973 2068 6176 6520 6265 656e 2070 7265  ys have been pre
-000003f0: 7373 6564 2061 6e64 2072 656c 6561 7365  ssed and release
-00000400: 6420 7468 6973 2074 6963 6b0a 2020 2020  d this tick.    
-00000410: e905 0000 0063 0200 0000 0000 0000 0000  .....c..........
-00000420: 0000 0200 0000 0300 0000 0300 0000 7312  ..............s.
-00000430: 0000 0074 0083 006a 017c 0164 018d 0101  ...t...j.|.d....
-00000440: 0064 0053 0029 024e 2901 da06 6d61 786c  .d.S.).N)...maxl
-00000450: 656e 2902 da05 7375 7065 72da 085f 5f69  en)...super..__i
-00000460: 6e69 745f 5f29 0272 0700 0000 da0c 7175  nit__).r......qu
-00000470: 6575 655f 6c65 6e67 7468 a901 da09 5f5f  eue_length....__
-00000480: 636c 6173 735f 5f72 0600 0000 720a 0000  class__r....r...
-00000490: 0072 1500 0000 1500 0000 f302 0000 0012  .r..............
-000004a0: 017a 1349 6e70 7574 5175 6575 652e 5f5f  .z.InputQueue.__
-000004b0: 696e 6974 5f5f 7205 0000 0063 0100 0000  init__r....c....
-000004c0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-000004d0: 4300 0000 7304 0000 0074 0082 0129 017a  C...s....t...).z
-000004e0: 5e53 7562 636c 6173 7365 7320 7368 6f75  ^Subclasses shou
-000004f0: 6c64 2069 6d70 6c65 6d65 6e74 2074 6869  ld implement thi
-00000500: 732e 2049 7420 7368 6f75 6c64 2062 6520  s. It should be 
-00000510: 736f 6d65 7468 696e 6720 6c69 6b65 0a20  something like. 
-00000520: 2020 2020 2020 2070 7967 616d 652e 6b65         pygame.ke
-00000530: 792e 6765 745f 7072 6573 7365 6428 2929  y.get_pressed())
-00000540: 01da 134e 6f74 496d 706c 656d 656e 7465  ...NotImplemente
-00000550: 6445 7272 6f72 a901 7207 0000 0072 0600  dError..r....r..
-00000560: 0000 7206 0000 0072 0a00 0000 da0e 6765  ..r....r......ge
-00000570: 745f 6e65 775f 7661 6c75 6573 1800 0000  t_new_values....
-00000580: 7302 0000 0004 037a 1949 6e70 7574 5175  s......z.InputQu
-00000590: 6575 652e 6765 745f 6e65 775f 7661 6c75  eue.get_new_valu
-000005a0: 6573 6301 0000 0000 0000 0000 0000 0001  esc.............
-000005b0: 0000 0004 0000 0043 0000 0073 1200 0000  .......C...s....
-000005c0: 7c00 a000 7c00 a001 a100 a101 0100 6400  |...|.........d.
-000005d0: 5300 a901 4e29 02da 0661 7070 656e 6472  S...N)...appendr
-000005e0: 1c00 0000 721b 0000 0072 0600 0000 7206  ....r....r....r.
-000005f0: 0000 0072 0a00 0000 da0f 7265 6164 5f6e  ...r......read_n
-00000600: 6577 5f69 6e70 7574 731d 0000 0072 1900  ew_inputs....r..
-00000610: 0000 7a1a 496e 7075 7451 7565 7565 2e72  ..z.InputQueue.r
-00000620: 6561 645f 6e65 775f 696e 7075 7473 6301  ead_new_inputsc.
-00000630: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00000640: 0000 0043 0000 0073 1a00 0000 7400 7c00  ...C...s....t.|.
-00000650: 8301 6401 6b04 720a 7c00 6402 1900 5300  ..d.k.r.|.d...S.
-00000660: 7401 8300 5300 2903 7a2d 5265 7475 726e  t...S.).z-Return
-00000670: 2074 6865 206b 6579 7320 7768 6963 6820   the keys which 
-00000680: 6172 6520 6375 7272 656e 746c 7920 6865  are currently he
-00000690: 6c64 2064 6f77 6e72 0100 0000 e9ff ffff  ld downr........
-000006a0: ff29 02da 036c 656e 7204 0000 0072 1b00  .)...lenr....r..
-000006b0: 0000 7206 0000 0072 0600 0000 720a 0000  ..r....r....r...
-000006c0: 00da 0867 6574 5f64 6f77 6e20 0000 0073  ...get_down ...s
-000006d0: 0200 0000 1a02 7a13 496e 7075 7451 7565  ......z.InputQue
-000006e0: 7565 2e67 6574 5f64 6f77 6e63 0100 0000  ue.get_downc....
-000006f0: 0000 0000 0000 0000 0100 0000 0800 0000  ................
-00000700: 0300 0000 f34e 0000 007a 1a7c 0064 0119  .....N...z.|.d..
-00000710: 0089 007c 0064 0219 0089 0174 0087 0087  ...|.d.....t....
-00000720: 0166 0264 0364 0484 0874 0174 0288 0083  .f.d.d...t.t....
-00000730: 0188 0183 0244 0083 0183 0157 0053 0004  .....D.....W.S..
-00000740: 0074 0379 2601 0001 0001 0074 0483 0006  .t.y&......t....
-00000750: 0059 0053 0077 0029 057a 7252 6574 7572  .Y.S.w.).zrRetur
-00000760: 6e20 7468 6520 6b65 7973 2074 6861 7420  n the keys that 
-00000770: 6861 7665 206a 7573 7420 6265 656e 2070  have just been p
-00000780: 7265 7373 6564 2d2d 2d69 2e65 2e20 7468  ressed---i.e. th
-00000790: 6f73 6520 7468 6174 2061 7265 2064 6f77  ose that are dow
-000007a0: 6e20 7468 6973 2074 6963 6b20 6275 740a  n this tick but.
-000007b0: 2020 2020 2020 2020 6e6f 7420 7468 6520          not the 
-000007c0: 7072 6576 696f 7573 2074 6963 6b72 2000  previous tickr .
-000007d0: 0000 e9fe ffff ff63 0100 0000 0000 0000  .......c........
-000007e0: 0000 0000 0400 0000 0400 0000 3300 0000  ............3...
-000007f0: 732e 0000 0081 007c 005d 125c 025c 027d  s......|.].\.\.}
-00000800: 017d 027d 0374 0088 007c 0119 006f 1188  .}.}.t...|...o..
-00000810: 017c 0119 000c 0083 0156 0001 0071 0264  .|.......V...q.d
-00000820: 0053 0072 1d00 0000 a901 7210 0000 00a9  .S.r......r.....
-00000830: 04da 022e 30da 0169 da01 63da 0170 a902  ....0..i..c..p..
-00000840: da07 6375 7272 656e 74da 0870 7265 7669  ..current..previ
-00000850: 6f75 7372 0600 0000 720a 0000 00da 093c  ousr....r......<
-00000860: 6765 6e65 7870 723e 2d00 0000 f30a 0000  genexpr>-.......
-00000870: 0002 8004 000a 0214 ff0a ff7a 2949 6e70  ...........z)Inp
-00000880: 7574 5175 6575 652e 6765 745f 7072 6573  utQueue.get_pres
-00000890: 7365 642e 3c6c 6f63 616c 733e 2e3c 6765  sed.<locals>.<ge
-000008a0: 6e65 7870 723e a905 da05 7475 706c 65da  nexpr>....tuple.
-000008b0: 037a 6970 da09 656e 756d 6572 6174 65da  .zip..enumerate.
-000008c0: 0a49 6e64 6578 4572 726f 7272 0400 0000  .IndexErrorr....
-000008d0: 721b 0000 0072 0600 0000 722b 0000 0072  r....r....r+...r
-000008e0: 0a00 0000 da0b 6765 745f 7072 6573 7365  ......get_presse
-000008f0: 6424 0000 0073 1200 0000 0203 0801 0801  d$...s..........
-00000900: 0e04 0c02 0afe 0c04 0a01 02ff 7a16 496e  ............z.In
-00000910: 7075 7451 7565 7565 2e67 6574 5f70 7265  putQueue.get_pre
-00000920: 7373 6564 6301 0000 0000 0000 0000 0000  ssedc...........
-00000930: 0001 0000 0008 0000 0003 0000 0072 2300  .............r#.
-00000940: 0000 2905 7a7e 5265 7475 726e 2074 6865  ..).z~Return the
-00000950: 206b 6579 7320 7468 6174 2068 6176 6520   keys that have 
-00000960: 6a75 7374 2062 6565 6e20 7265 6c65 6173  just been releas
-00000970: 6564 2d2d 2d69 2e65 2e20 7468 6f73 6520  ed---i.e. those 
-00000980: 7468 6174 2061 7265 206e 6f74 2064 6f77  that are not dow
-00000990: 6e20 7468 6973 0a20 2020 2020 2020 2074  n this.        t
-000009a0: 6963 6b2c 2062 7574 2077 6572 6520 646f  ick, but were do
-000009b0: 776e 2074 6865 2070 7265 7669 6f75 7320  wn the previous 
-000009c0: 7469 636b 7220 0000 0072 2400 0000 6301  tickr ...r$...c.
-000009d0: 0000 0000 0000 0000 0000 0004 0000 0004  ................
-000009e0: 0000 0033 0000 0073 2e00 0000 8100 7c00  ...3...s......|.
-000009f0: 5d12 5c02 5c02 7d01 7d02 7d03 7400 8801  ].\.\.}.}.}.t...
-00000a00: 7c01 1900 6f11 8800 7c01 1900 0c00 8301  |...o...|.......
-00000a10: 5600 0100 7102 6400 5300 721d 0000 0072  V...q.d.S.r....r
-00000a20: 2500 0000 7226 0000 0072 2b00 0000 7206  %...r&...r+...r.
-00000a30: 0000 0072 0a00 0000 722e 0000 003a 0000  ...r....r....:..
-00000a40: 0072 2f00 0000 7a2a 496e 7075 7451 7565  .r/...z*InputQue
-00000a50: 7565 2e67 6574 5f72 656c 6561 7365 642e  ue.get_released.
-00000a60: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
-00000a70: 723e 7230 0000 0072 1b00 0000 7206 0000  r>r0...r....r...
-00000a80: 0072 2b00 0000 720a 0000 00da 0c67 6574  .r+...r......get
-00000a90: 5f72 656c 6561 7365 6434 0000 0073 1200  _released4...s..
-00000aa0: 0000 0203 0801 0801 0e01 0c02 0afe 0c04  ................
-00000ab0: 0a01 02ff 7a17 496e 7075 7451 7565 7565  ....z.InputQueue
-00000ac0: 2e67 6574 5f72 656c 6561 7365 6463 0200  .get_releasedc..
-00000ad0: 0000 0000 0000 0000 0000 0300 0000 0200  ................
-00000ae0: 0000 4300 0000 f310 0000 007c 00a0 00a1  ..C........|....
-00000af0: 007d 027c 027c 0119 0053 0029 017a 2943  .}.|.|...S.).z)C
-00000b00: 6865 636b 2069 6620 6120 6b65 7920 6861  heck if a key ha
-00000b10: 7320 6265 656e 2070 7265 7373 6564 2074  s been pressed t
-00000b20: 6869 7320 7469 636b 2901 7235 0000 00a9  his tick).r5....
-00000b30: 0372 0700 0000 da03 6b65 79da 046b 6579  .r......key..key
-00000b40: 7372 0600 0000 7206 0000 0072 0a00 0000  sr....r....r....
-00000b50: da0a 6973 5f70 7265 7373 6564 4100 0000  ..is_pressedA...
-00000b60: f304 0000 0008 0208 017a 1549 6e70 7574  .........z.Input
-00000b70: 5175 6575 652e 6973 5f70 7265 7373 6564  Queue.is_pressed
-00000b80: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-00000b90: 0002 0000 0043 0000 0072 3700 0000 2901  .....C...r7...).
-00000ba0: 7a25 4368 6563 6b20 6966 2061 206b 6579  z%Check if a key
-00000bb0: 2069 7320 6375 7272 656e 746c 7920 6865   is currently he
-00000bc0: 6c64 2064 6f77 6e29 0172 2200 0000 7238  ld down).r"...r8
-00000bd0: 0000 0072 0600 0000 7206 0000 0072 0a00  ...r....r....r..
-00000be0: 0000 da07 6973 5f64 6f77 6e46 0000 0072  ....is_downF...r
-00000bf0: 3c00 0000 7a12 496e 7075 7451 7565 7565  <...z.InputQueue
-00000c00: 2e69 735f 646f 776e 6302 0000 0000 0000  .is_downc.......
-00000c10: 0000 0000 0003 0000 0002 0000 0043 0000  .............C..
-00000c20: 0072 3700 0000 2901 7a2a 4368 6563 6b20  .r7...).z*Check 
-00000c30: 6966 2061 206b 6579 2068 6173 2062 6565  if a key has bee
-00000c40: 6e20 7265 6c65 6173 6564 2074 6869 7320  n released this 
-00000c50: 7469 636b 2901 7236 0000 0072 3800 0000  tick).r6...r8...
-00000c60: 7206 0000 0072 0600 0000 720a 0000 00da  r....r....r.....
-00000c70: 0b69 735f 7265 6c65 6173 6564 4b00 0000  .is_releasedK...
-00000c80: 723c 0000 007a 1649 6e70 7574 5175 6575  r<...z.InputQueu
-00000c90: 652e 6973 5f72 656c 6561 7365 6463 0300  e.is_releasedc..
-00000ca0: 0000 0000 0000 0000 0000 0500 0000 0300  ................
-00000cb0: 0000 0300 0000 732c 0000 0074 007c 0083  ......s,...t.|..
-00000cc0: 017c 020b 0064 0185 0219 007d 0387 0066  .|...d.....}...f
-00000cd0: 0164 0264 0384 087c 0344 0083 017d 0474  .d.d...|.D...}.t
-00000ce0: 017c 0483 0153 0029 047a 4643 6f75 6e74  .|...S.).zFCount
-00000cf0: 2074 6865 2072 6973 696e 6720 616e 6420   the rising and 
-00000d00: 6661 6c6c 696e 6720 6564 6765 732e 2043  falling edges. C
-00000d10: 616e 2062 6520 7573 6564 2074 6f20 6465  an be used to de
-00000d20: 7465 6374 2070 6173 7420 696e 7075 7473  tect past inputs
-00000d30: 2e4e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
-00000d40: 0000 0004 0000 0013 0000 0073 1400 0000  ...........s....
-00000d50: 6700 7c00 5d06 7d01 7c01 8800 1900 9102  g.|.].}.|.......
-00000d60: 7102 5300 7206 0000 0072 0600 0000 2902  q.S.r....r....).
-00000d70: 7227 0000 00da 056c 6179 6572 a901 7239  r'.....layer..r9
-00000d80: 0000 0072 0600 0000 720a 0000 00da 0a3c  ...r....r......<
-00000d90: 6c69 7374 636f 6d70 3e53 0000 0073 0200  listcomp>S...s..
-00000da0: 0000 1400 7a2e 496e 7075 7451 7565 7565  ....z.InputQueue
-00000db0: 2e62 7566 6665 7265 645f 696e 7075 7473  .buffered_inputs
-00000dc0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00000dd0: 6f6d 703e 2902 da04 6c69 7374 7203 0000  omp>)...listr...
-00000de0: 0029 0572 0700 0000 7239 0000 00da 0d62  .).r....r9.....b
-00000df0: 7566 6665 725f 6c65 6e67 7468 da06 6275  uffer_length..bu
-00000e00: 6666 6572 da06 7661 6c75 6573 7206 0000  ffer..valuesr...
-00000e10: 0072 4000 0000 720a 0000 00da 0f62 7566  .r@...r......buf
-00000e20: 6665 7265 645f 696e 7075 7473 5000 0000  fered_inputsP...
-00000e30: 7306 0000 0012 0212 0108 017a 1a49 6e70  s..........z.Inp
-00000e40: 7574 5175 6575 652e 6275 6666 6572 6564  utQueue.buffered
-00000e50: 5f69 6e70 7574 7363 0300 0000 0000 0000  _inputsc........
-00000e60: 0000 0000 0500 0000 0400 0000 4300 0000  ............C...
-00000e70: 7314 0000 007c 00a0 007c 017c 02a1 025c  s....|...|.|...\
-00000e80: 027d 037d 047c 0353 0072 1d00 0000 a901  .}.}.|.S.r......
-00000e90: 7246 0000 00a9 0572 0700 0000 7239 0000  rF.....r....r9..
-00000ea0: 0072 4300 0000 da06 7269 7369 6e67 da07  .rC.....rising..
-00000eb0: 6661 6c6c 696e 6772 0600 0000 7206 0000  fallingr....r...
-00000ec0: 0072 0a00 0000 da10 6275 6666 6572 6564  .r......buffered
-00000ed0: 5f70 7265 7373 6573 5600 0000 f304 0000  _pressesV.......
-00000ee0: 0010 0104 017a 1b49 6e70 7574 5175 6575  .....z.InputQueu
-00000ef0: 652e 6275 6666 6572 6564 5f70 7265 7373  e.buffered_press
-00000f00: 6573 6303 0000 0000 0000 0000 0000 0005  esc.............
-00000f10: 0000 0004 0000 0043 0000 0073 1400 0000  .......C...s....
-00000f20: 7c00 a000 7c01 7c02 a102 5c02 7d03 7d04  |...|.|...\.}.}.
-00000f30: 7c04 5300 721d 0000 0072 4700 0000 7248  |.S.r....rG...rH
-00000f40: 0000 0072 0600 0000 7206 0000 0072 0a00  ...r....r....r..
-00000f50: 0000 da11 6275 6666 6572 6564 5f72 656c  ....buffered_rel
-00000f60: 6561 7365 735a 0000 0072 4c00 0000 7a1c  easesZ...rL...z.
-00000f70: 496e 7075 7451 7565 7565 2e62 7566 6665  InputQueue.buffe
-00000f80: 7265 645f 7265 6c65 6173 6573 2901 7212  red_releases).r.
-00000f90: 0000 0029 1372 0c00 0000 720d 0000 0072  ...).r....r....r
-00000fa0: 0e00 0000 720f 0000 0072 1500 0000 7231  ....r....r....r1
-00000fb0: 0000 0072 1000 0000 721c 0000 0072 1f00  ...r....r....r..
-00000fc0: 0000 7222 0000 0072 3500 0000 7236 0000  ..r"...r5...r6..
-00000fd0: 0072 3b00 0000 723d 0000 0072 3e00 0000  .r;...r=...r>...
-00000fe0: 7246 0000 0072 4b00 0000 724d 0000 00da  rF...rK...rM....
-00000ff0: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7206  .__classcell__r.
-00001000: 0000 0072 0600 0000 7217 0000 0072 0a00  ...r....r....r..
-00001010: 0000 7211 0000 000e 0000 0073 1c00 0000  ..r........s....
-00001020: 0800 0401 0e06 1203 0805 1203 1204 1210  ................
-00001030: 0e0d 0e05 0e05 0805 0806 1004 7211 0000  ............r...
-00001040: 004e 2907 da0b 636f 6c6c 6563 7469 6f6e  .N)...collection
-00001050: 7372 0200 0000 da0f 726f 6269 6e67 616d  sr......robingam
-00001060: 652e 7574 696c 7372 0300 0000 7231 0000  e.utilsr....r1..
-00001070: 0072 0400 0000 7211 0000 0072 0600 0000  .r....r....r....
-00001080: 7206 0000 0072 0600 0000 720a 0000 00da  r....r....r.....
-00001090: 083c 6d6f 6475 6c65 3e01 0000 0073 0800  .<module>....s..
-000010a0: 0000 0c00 0c02 1003 1408                 ..........
+00000040: 6d03 5a03 0100 6504 6505 4200 5a06 6507  m.Z...e.e.B.Z.e.
+00000050: 6506 6403 6602 1900 5a08 4700 6404 6405  e.d.f...Z.G.d.d.
+00000060: 8400 6405 6507 8303 5a09 4700 6406 6407  ..d.e...Z.G.d.d.
+00000070: 8400 6407 6501 8303 5a0a 6408 5300 2909  ..d.e...Z.d.S.).
+00000080: e900 0000 0029 01da 0564 6571 7565 2901  .....)...deque).
+00000090: da0b 636f 756e 745f 6564 6765 732e 6300  ..count_edges.c.
+000000a0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+000000b0: 0000 0040 0000 0073 1e00 0000 6500 5a01  ...@...s....e.Z.
+000000c0: 6400 5a02 6401 5a03 6402 6504 6602 6403  d.Z.d.Z.d.e.f.d.
+000000d0: 6404 8404 5a05 6405 5300 2906 da05 456d  d...Z.d.S.)...Em
+000000e0: 7074 797a 8c0a 2020 2020 4d6f 636b 2074  ptyz..    Mock t
+000000f0: 7570 6c65 206f 6620 302f 3173 2074 6861  uple of 0/1s tha
+00000100: 7420 616c 7761 7973 2072 6574 7572 6e73  t always returns
+00000110: 2061 2030 206e 6f20 6d61 7474 6572 2074   a 0 no matter t
+00000120: 6865 2069 6e64 6578 2e20 5468 6973 2069  he index. This i
+00000130: 7320 7573 6564 2074 6f0a 2020 2020 7370  s used to.    sp
+00000140: 6f6f 6620 616e 2065 6d70 7479 2070 7967  oof an empty pyg
+00000150: 616d 652e 6b65 792e 6765 745f 7072 6573  ame.key.get_pres
+00000160: 7365 6428 2920 7475 706c 652e 0a20 2020  sed() tuple..   
+00000170: 20da 0672 6574 7572 6e63 0100 0000 0000   ..returnc......
+00000180: 0000 0000 0000 0300 0000 0100 0000 4f00  ..............O.
+00000190: 0000 7304 0000 0064 0153 0029 024e 7201  ..s....d.S.).Nr.
+000001a0: 0000 00a9 0029 03da 0473 656c 66da 0461  .....)...self..a
+000001b0: 7267 73da 066b 7761 7267 7372 0600 0000  rgs..kwargsr....
+000001c0: 7206 0000 00fa 332f 686f 6d65 2f72 6f62  r.....3/home/rob
+000001d0: 696e 2f63 6f64 652f 726f 6269 6e67 616d  in/code/robingam
+000001e0: 652f 726f 6269 6e67 616d 652f 696e 7075  e/robingame/inpu
+000001f0: 742f 7175 6575 652e 7079 da0b 5f5f 6765  t/queue.py..__ge
+00000200: 7469 7465 6d5f 5f15 0000 0073 0200 0000  titem__....s....
+00000210: 0401 7a11 456d 7074 792e 5f5f 6765 7469  ..z.Empty.__geti
+00000220: 7465 6d5f 5f4e 2906 da08 5f5f 6e61 6d65  tem__N)...__name
+00000230: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000240: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
+00000250: 646f 635f 5fda 0369 6e74 720b 0000 0072  doc__..intr....r
+00000260: 0600 0000 7206 0000 0072 0600 0000 720a  ....r....r....r.
+00000270: 0000 0072 0400 0000 0f00 0000 7306 0000  ...r........s...
+00000280: 0008 0004 0112 0572 0400 0000 6300 0000  .......r....c...
+00000290: 0000 0000 0000 0000 0000 0000 0008 0000  ................
+000002a0: 0000 0000 0073 ba00 0000 6500 5a01 6400  .....s....e.Z.d.
+000002b0: 5a02 6401 5a03 641e 8700 6601 6403 6404  Z.d.Z.d...f.d.d.
+000002c0: 8409 5a04 6405 6505 6602 6406 6407 8404  ..Z.d.e.f.d.d...
+000002d0: 5a06 6408 6409 8400 5a07 6405 6505 6602  Z.d.d...Z.d.e.f.
+000002e0: 640a 640b 8404 5a08 6405 6505 6602 640c  d.d...Z.d.e.f.d.
+000002f0: 640d 8404 5a09 6405 6505 6602 640e 640f  d...Z.d.e.f.d.d.
+00000300: 8404 5a0a 6405 650b 6602 6410 6411 8404  ..Z.d.e.f.d.d...
+00000310: 5a0c 6405 650b 6602 6412 6413 8404 5a0d  Z.d.e.f.d.d...Z.
+00000320: 6405 650b 6602 6414 6415 8404 5a0e 6416  d.e.f.d.d...Z.d.
+00000330: 650b 6417 650b 6405 650f 650b 650b 6602  e.d.e.d.e.e.e.f.
+00000340: 1900 6606 6418 6419 8404 5a10 641a 641b  ..f.d.d...Z.d.d.
+00000350: 8400 5a11 641c 641d 8400 5a12 8700 0400  ..Z.d.d...Z.....
+00000360: 5a13 5300 291f da0a 496e 7075 7451 7565  Z.S.)...InputQue
+00000370: 7565 615c 0100 000a 2020 2020 5072 6f76  uea\....    Prov
+00000380: 6964 6573 2061 6464 6974 696f 6e61 6c20  ides additional 
+00000390: 6675 6e63 7469 6f6e 616c 6974 7920 6265  functionality be
+000003a0: 796f 6e64 2070 7967 616d 652e 6b65 792e  yond pygame.key.
+000003b0: 6765 745f 7072 6573 7365 6428 292e 0a20  get_pressed().. 
+000003c0: 2020 2043 6f6e 7461 696e 7320 6120 7365     Contains a se
+000003d0: 7269 6573 206f 6620 4368 616e 6e65 6c54  ries of ChannelT
+000003e0: 7570 6c65 7320 7768 6963 6820 7265 7072  uples which repr
+000003f0: 6573 656e 7420 7468 6520 7374 6174 6520  esent the state 
+00000400: 6869 7374 6f72 7920 6f66 2074 6865 2069  history of the i
+00000410: 6e70 7574 2064 6576 6963 650a 2020 2020  nput device.    
+00000420: 7468 6174 2074 6869 7320 7175 6575 6520  that this queue 
+00000430: 6973 2074 7261 636b 696e 672e 0a20 2020  is tracking..   
+00000440: 2054 6869 7320 696e 7075 7420 6869 7374   This input hist
+00000450: 6f72 7920 616c 6c6f 7773 2075 7320 746f  ory allows us to
+00000460: 2074 7261 636b 2077 6869 6368 206b 6579   track which key
+00000470: 7320 6861 7665 2062 6565 6e20 7072 6573  s have been pres
+00000480: 7365 6420 616e 6420 7265 6c65 6173 6564  sed and released
+00000490: 2074 6869 7320 7469 636b 2e0a 0a20 2020   this tick...   
+000004a0: 2053 7562 636c 6173 7365 7320 7368 6f75   Subclasses shou
+000004b0: 6c64 2069 6d70 6c65 6d65 6e74 2060 6765  ld implement `ge
+000004c0: 745f 6e65 775f 7661 6c75 6573 602e 0a20  t_new_values`.. 
+000004d0: 2020 20e9 0500 0000 6302 0000 0000 0000     .....c.......
+000004e0: 0000 0000 0002 0000 0003 0000 0003 0000  ................
+000004f0: 0073 1200 0000 7400 8300 6a01 7c01 6401  .s....t...j.|.d.
+00000500: 8d01 0100 6400 5300 2902 4e29 01da 066d  ....d.S.).N)...m
+00000510: 6178 6c65 6e29 02da 0573 7570 6572 da08  axlen)...super..
+00000520: 5f5f 696e 6974 5f5f 2902 7207 0000 00da  __init__).r.....
+00000530: 0c71 7565 7565 5f6c 656e 6774 68a9 01da  .queue_length...
+00000540: 095f 5f63 6c61 7373 5f5f 7206 0000 0072  .__class__r....r
+00000550: 0a00 0000 7215 0000 0023 0000 00f3 0200  ....r....#......
+00000560: 0000 1201 7a13 496e 7075 7451 7565 7565  ....z.InputQueue
+00000570: 2e5f 5f69 6e69 745f 5f72 0500 0000 6301  .__init__r....c.
+00000580: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000590: 0000 0043 0000 0073 0400 0000 7400 8201  ...C...s....t...
+000005a0: 2901 7ad1 0a20 2020 2020 2020 2053 7562  ).z..        Sub
+000005b0: 636c 6173 7365 7320 7368 6f75 6c64 2069  classes should i
+000005c0: 6d70 6c65 6d65 6e74 2074 6869 732e 0a20  mplement this.. 
+000005d0: 2020 2020 2020 2049 7420 7368 6f75 6c64         It should
+000005e0: 2062 6520 736f 6d65 7468 696e 6720 6c69   be something li
+000005f0: 6b65 2070 7967 616d 652e 6b65 792e 6765  ke pygame.key.ge
+00000600: 745f 7072 6573 7365 6428 292e 0a0a 2020  t_pressed()...  
+00000610: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00000620: 2020 2020 2020 2020 2020 2061 2074 7570             a tup
+00000630: 6c65 206f 6620 696e 7465 6765 7273 2072  le of integers r
+00000640: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
+00000650: 7374 6174 6573 206f 6620 7468 6520 696e  states of the in
+00000660: 7075 7420 6368 616e 6e65 6c73 0a20 2020  put channels.   
+00000670: 2020 2020 2029 01da 134e 6f74 496d 706c       )...NotImpl
+00000680: 656d 656e 7465 6445 7272 6f72 a901 7207  ementedError..r.
+00000690: 0000 0072 0600 0000 7206 0000 0072 0a00  ...r....r....r..
+000006a0: 0000 da0e 6765 745f 6e65 775f 7661 6c75  ....get_new_valu
+000006b0: 6573 2600 0000 7302 0000 0004 087a 1949  es&...s......z.I
+000006c0: 6e70 7574 5175 6575 652e 6765 745f 6e65  nputQueue.get_ne
+000006d0: 775f 7661 6c75 6573 6301 0000 0000 0000  w_valuesc.......
+000006e0: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+000006f0: 0073 1200 0000 7c00 a000 7c00 a001 a100  .s....|...|.....
+00000700: a101 0100 6400 5300 a901 4e29 02da 0661  ....d.S...N)...a
+00000710: 7070 656e 6472 1c00 0000 721b 0000 0072  ppendr....r....r
+00000720: 0600 0000 7206 0000 0072 0a00 0000 da0f  ....r....r......
+00000730: 7265 6164 5f6e 6577 5f69 6e70 7574 7330  read_new_inputs0
+00000740: 0000 0072 1900 0000 7a1a 496e 7075 7451  ...r....z.InputQ
+00000750: 7565 7565 2e72 6561 645f 6e65 775f 696e  ueue.read_new_in
+00000760: 7075 7473 6301 0000 0000 0000 0000 0000  putsc...........
+00000770: 0001 0000 0002 0000 0043 0000 0073 1a00  .........C...s..
+00000780: 0000 7400 7c00 8301 6401 6b04 720a 7c00  ..t.|...d.k.r.|.
+00000790: 6402 1900 5300 7401 8300 5300 2903 7aa6  d...S.t...S.).z.
+000007a0: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
+000007b0: 7468 6520 6b65 7973 2077 6869 6368 2061  the keys which a
+000007c0: 7265 2063 7572 7265 6e74 6c79 2068 656c  re currently hel
+000007d0: 6420 646f 776e 2e0a 0a20 2020 2020 2020  d down...       
+000007e0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+000007f0: 2020 2020 2020 6120 7475 706c 6520 6f66        a tuple of
+00000800: 2076 616c 7565 7320 666f 7220 6561 6368   values for each
+00000810: 2069 6e70 7574 2063 6861 6e6e 656c 2e20   input channel. 
+00000820: 3020 3d20 6e6f 7420 646f 776e 2e20 4e6f  0 = not down. No
+00000830: 6e7a 6572 6f20 3d20 646f 776e 2e0a 2020  nzero = down..  
+00000840: 2020 2020 2020 7201 0000 00e9 ffff ffff        r.........
+00000850: 2902 da03 6c65 6e72 0400 0000 721b 0000  )...lenr....r...
+00000860: 0072 0600 0000 7206 0000 0072 0a00 0000  .r....r....r....
+00000870: da08 6765 745f 646f 776e 3300 0000 7302  ..get_down3...s.
+00000880: 0000 001a 077a 1349 6e70 7574 5175 6575  .....z.InputQueu
+00000890: 652e 6765 745f 646f 776e 6301 0000 0000  e.get_downc.....
+000008a0: 0000 0000 0000 0001 0000 0008 0000 0003  ................
+000008b0: 0000 00f3 4e00 0000 7a1a 7c00 6401 1900  ....N...z.|.d...
+000008c0: 8900 7c00 6402 1900 8901 7400 8700 8701  ..|.d.....t.....
+000008d0: 6602 6403 6404 8408 7401 7402 8800 8301  f.d.d...t.t.....
+000008e0: 8801 8302 4400 8301 8301 5700 5300 0400  ....D.....W.S...
+000008f0: 7403 7926 0100 0100 0100 7404 8300 0600  t.y&......t.....
+00000900: 5900 5300 7700 2905 7aea 0a20 2020 2020  Y.S.w.).z..     
+00000910: 2020 2052 6574 7572 6e20 7468 6520 6b65     Return the ke
+00000920: 7973 2074 6861 7420 6861 7665 206a 7573  ys that have jus
+00000930: 7420 6265 656e 2070 7265 7373 6564 0a20  t been pressed. 
+00000940: 2020 2020 2020 2069 2e65 2e20 7468 6f73         i.e. thos
+00000950: 6520 7468 6174 2061 7265 2064 6f77 6e20  e that are down 
+00000960: 7468 6973 2074 6963 6b20 6275 7420 6e6f  this tick but no
+00000970: 7420 7468 6520 7072 6576 696f 7573 2074  t the previous t
+00000980: 6963 6b0a 0a20 2020 2020 2020 2052 6574  ick..        Ret
+00000990: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+000009a0: 2020 6120 7475 706c 6520 6f66 2069 6e74    a tuple of int
+000009b0: 6567 6572 7320 666f 7220 6561 6368 2069  egers for each i
+000009c0: 6e70 7574 2063 6861 6e6e 656c 2e20 3120  nput channel. 1 
+000009d0: 3d20 7072 6573 7365 642c 2030 203d 206e  = pressed, 0 = n
+000009e0: 6f74 2070 7265 7373 6564 2e0a 2020 2020  ot pressed..    
+000009f0: 2020 2020 7220 0000 00e9 feff ffff 6301      r ........c.
+00000a00: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+00000a10: 0000 0033 0000 0073 2e00 0000 8100 7c00  ...3...s......|.
+00000a20: 5d12 5c02 5c02 7d01 7d02 7d03 7400 8800  ].\.\.}.}.}.t...
+00000a30: 7c01 1900 6f11 8801 7c01 1900 0c00 8301  |...o...|.......
+00000a40: 5600 0100 7102 6400 5300 721d 0000 00a9  V...q.d.S.r.....
+00000a50: 0172 1000 0000 a904 da02 2e30 da01 69da  .r.........0..i.
+00000a60: 0163 da01 70a9 02da 0763 7572 7265 6e74  .c..p....current
+00000a70: da08 7072 6576 696f 7573 7206 0000 0072  ..previousr....r
+00000a80: 0a00 0000 da09 3c67 656e 6578 7072 3e4a  ......<genexpr>J
+00000a90: 0000 00f3 0a00 0000 0280 0400 0a02 14ff  ................
+00000aa0: 0aff 7a29 496e 7075 7451 7565 7565 2e67  ..z)InputQueue.g
+00000ab0: 6574 5f70 7265 7373 6564 2e3c 6c6f 6361  et_pressed.<loca
+00000ac0: 6c73 3e2e 3c67 656e 6578 7072 3ea9 05da  ls>.<genexpr>...
+00000ad0: 0574 7570 6c65 da03 7a69 70da 0965 6e75  .tuple..zip..enu
+00000ae0: 6d65 7261 7465 da0a 496e 6465 7845 7272  merate..IndexErr
+00000af0: 6f72 7204 0000 0072 1b00 0000 7206 0000  orr....r....r...
+00000b00: 0072 2b00 0000 720a 0000 00da 0b67 6574  .r+...r......get
+00000b10: 5f70 7265 7373 6564 3c00 0000 7312 0000  _pressed<...s...
+00000b20: 0002 0808 0108 010e 040c 020a fe0c 040a  ................
+00000b30: 0102 ff7a 1649 6e70 7574 5175 6575 652e  ...z.InputQueue.
+00000b40: 6765 745f 7072 6573 7365 6463 0100 0000  get_pressedc....
+00000b50: 0000 0000 0000 0000 0100 0000 0800 0000  ................
+00000b60: 0300 0000 7223 0000 0029 057a f90a 2020  ....r#...).z..  
+00000b70: 2020 2020 2020 5265 7475 726e 2074 6865        Return the
+00000b80: 206b 6579 7320 7468 6174 2068 6176 6520   keys that have 
+00000b90: 6a75 7374 2062 6565 6e20 7265 6c65 6173  just been releas
+00000ba0: 6564 0a20 2020 2020 2020 2069 2e65 2e20  ed.        i.e. 
+00000bb0: 7468 6f73 6520 7468 6174 2061 7265 206e  those that are n
+00000bc0: 6f74 2064 6f77 6e20 7468 6973 2074 6963  ot down this tic
+00000bd0: 6b2c 2062 7574 2077 6572 6520 646f 776e  k, but were down
+00000be0: 2074 6865 2070 7265 7669 6f75 7320 7469   the previous ti
+00000bf0: 636b 2e0a 0a20 2020 2020 2020 2052 6574  ck...        Ret
+00000c00: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00000c10: 2020 6120 7475 706c 6520 6f66 2069 6e74    a tuple of int
+00000c20: 6567 6572 7320 666f 7220 6561 6368 2069  egers for each i
+00000c30: 6e70 7574 2063 6861 6e6e 656c 2e20 3120  nput channel. 1 
+00000c40: 3d20 7265 6c65 6173 6564 2c20 3020 3d20  = released, 0 = 
+00000c50: 6e6f 7420 7265 6c65 6173 6564 2e0a 2020  not released..  
+00000c60: 2020 2020 2020 7220 0000 0072 2400 0000        r ...r$...
+00000c70: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
+00000c80: 0004 0000 0033 0000 0073 2e00 0000 8100  .....3...s......
+00000c90: 7c00 5d12 5c02 5c02 7d01 7d02 7d03 7400  |.].\.\.}.}.}.t.
+00000ca0: 8801 7c01 1900 6f11 8800 7c01 1900 0c00  ..|...o...|.....
+00000cb0: 8301 5600 0100 7102 6400 5300 721d 0000  ..V...q.d.S.r...
+00000cc0: 0072 2500 0000 7226 0000 0072 2b00 0000  .r%...r&...r+...
+00000cd0: 7206 0000 0072 0a00 0000 722e 0000 005c  r....r....r....\
+00000ce0: 0000 0072 2f00 0000 7a2a 496e 7075 7451  ...r/...z*InputQ
+00000cf0: 7565 7565 2e67 6574 5f72 656c 6561 7365  ueue.get_release
+00000d00: 642e 3c6c 6f63 616c 733e 2e3c 6765 6e65  d.<locals>.<gene
+00000d10: 7870 723e 7230 0000 0072 1b00 0000 7206  xpr>r0...r....r.
+00000d20: 0000 0072 2b00 0000 720a 0000 00da 0c67  ...r+...r......g
+00000d30: 6574 5f72 656c 6561 7365 6451 0000 0073  et_releasedQ...s
+00000d40: 1200 0000 0208 0801 0801 0e01 0c02 0afe  ................
+00000d50: 0c04 0a01 02ff 7a17 496e 7075 7451 7565  ......z.InputQue
+00000d60: 7565 2e67 6574 5f72 656c 6561 7365 6463  ue.get_releasedc
+00000d70: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00000d80: 0200 0000 4300 0000 f310 0000 007c 00a0  ....C........|..
+00000d90: 00a1 007d 027c 027c 0119 0053 0029 017a  ...}.|.|...S.).z
+00000da0: 730a 2020 2020 2020 2020 4368 6563 6b20  s.        Check 
+00000db0: 6966 2061 206b 6579 2068 6173 2062 6565  if a key has bee
+00000dc0: 6e20 7072 6573 7365 6420 7468 6973 2074  n pressed this t
+00000dd0: 6963 6b0a 0a20 2020 2020 2020 2052 6574  ick..        Ret
+00000de0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00000df0: 2020 3120 6966 2070 7265 7373 6564 3b20    1 if pressed; 
+00000e00: 3020 6f74 6865 7277 6973 650a 2020 2020  0 otherwise.    
+00000e10: 2020 2020 2901 7235 0000 00a9 0372 0700      ).r5.....r..
+00000e20: 0000 da03 6b65 79da 046b 6579 7372 0600  ....key..keysr..
+00000e30: 0000 7206 0000 0072 0a00 0000 da0a 6973  ..r....r......is
+00000e40: 5f70 7265 7373 6564 6300 0000 f304 0000  _pressedc.......
+00000e50: 0008 0708 017a 1549 6e70 7574 5175 6575  .....z.InputQueu
+00000e60: 652e 6973 5f70 7265 7373 6564 6302 0000  e.is_pressedc...
+00000e70: 0000 0000 0000 0000 0003 0000 0002 0000  ................
+00000e80: 0043 0000 0072 3700 0000 2901 7a6c 0a20  .C...r7...).zl. 
+00000e90: 2020 2020 2020 2043 6865 636b 2069 6620         Check if 
+00000ea0: 6120 6b65 7920 6973 2063 7572 7265 6e74  a key is current
+00000eb0: 6c79 2068 656c 6420 646f 776e 0a0a 2020  ly held down..  
+00000ec0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00000ed0: 2020 2020 2020 2020 2020 2031 2069 6620             1 if 
+00000ee0: 646f 776e 3b20 3020 6f74 6865 7277 6973  down; 0 otherwis
+00000ef0: 650a 2020 2020 2020 2020 2901 7222 0000  e.        ).r"..
+00000f00: 0072 3800 0000 7206 0000 0072 0600 0000  .r8...r....r....
+00000f10: 720a 0000 00da 0769 735f 646f 776e 6d00  r......is_downm.
+00000f20: 0000 723c 0000 007a 1249 6e70 7574 5175  ..r<...z.InputQu
+00000f30: 6575 652e 6973 5f64 6f77 6e63 0200 0000  eue.is_downc....
+00000f40: 0000 0000 0000 0000 0300 0000 0200 0000  ................
+00000f50: 4300 0000 7237 0000 0029 017a 750a 2020  C...r7...).zu.  
+00000f60: 2020 2020 2020 4368 6563 6b20 6966 2061        Check if a
+00000f70: 206b 6579 2068 6173 2062 6565 6e20 7265   key has been re
+00000f80: 6c65 6173 6564 2074 6869 7320 7469 636b  leased this tick
+00000f90: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00000fa0: 733a 0a20 2020 2020 2020 2020 2020 2031  s:.            1
+00000fb0: 2069 6620 7265 6c65 6173 6564 3b20 3020   if released; 0 
+00000fc0: 6f74 6865 7277 6973 650a 2020 2020 2020  otherwise.      
+00000fd0: 2020 2901 7236 0000 0072 3800 0000 7206    ).r6...r8...r.
+00000fe0: 0000 0072 0600 0000 720a 0000 00da 0b69  ...r....r......i
+00000ff0: 735f 7265 6c65 6173 6564 7700 0000 723c  s_releasedw...r<
+00001000: 0000 007a 1649 6e70 7574 5175 6575 652e  ...z.InputQueue.
+00001010: 6973 5f72 656c 6561 7365 6472 3900 0000  is_releasedr9...
+00001020: da0d 6275 6666 6572 5f6c 656e 6774 6863  ..buffer_lengthc
+00001030: 0300 0000 0000 0000 0000 0000 0500 0000  ................
+00001040: 0300 0000 0300 0000 732c 0000 0074 007c  ........s,...t.|
+00001050: 0083 017c 020b 0064 0185 0219 007d 0387  ...|...d.....}..
+00001060: 0066 0164 0264 0384 087c 0344 0083 017d  .f.d.d...|.D...}
+00001070: 0474 017c 0483 0153 0029 0461 4f01 0000  .t.|...S.).aO...
+00001080: 0a20 2020 2020 2020 2043 6f75 6e74 2074  .        Count t
+00001090: 6865 2072 6973 696e 6720 616e 6420 6661  he rising and fa
+000010a0: 6c6c 696e 6720 6564 6765 732e 2043 616e  lling edges. Can
+000010b0: 2062 6520 7573 6564 2074 6f20 6465 7465   be used to dete
+000010c0: 6374 2070 6173 7420 696e 7075 7473 2e0a  ct past inputs..
+000010d0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+000010e0: 2020 2020 2020 2020 2020 206b 6579 3a20             key: 
+000010f0: 6964 656e 7469 6669 6572 206f 6620 7468  identifier of th
+00001100: 6520 696e 7075 7420 6368 616e 6e65 6c0a  e input channel.
+00001110: 2020 2020 2020 2020 2020 2020 6275 6666              buff
+00001120: 6572 5f6c 656e 6774 683a 2068 6f77 206d  er_length: how m
+00001130: 616e 7920 7061 7374 2069 7465 7261 7469  any past iterati
+00001140: 6f6e 7320 746f 2063 6f6e 7369 6465 720a  ons to consider.
+00001150: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00001160: 3a0a 2020 2020 2020 2020 2020 2020 6e75  :.            nu
+00001170: 6d62 6572 206f 6620 7469 6d65 7320 7468  mber of times th
+00001180: 6520 696e 7075 7420 6368 616e 6e65 6c20  e input channel 
+00001190: 6861 7320 6265 656e 2070 7265 7373 6564  has been pressed
+000011a0: 2061 6e64 2072 656c 6561 7365 6420 6f76   and released ov
+000011b0: 6572 2074 6865 2060 6275 6666 6572 5f6c  er the `buffer_l
+000011c0: 656e 6774 6860 0a20 2020 2020 2020 204e  ength`.        N
+000011d0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000011e0: 0004 0000 0013 0000 0073 1400 0000 6700  .........s....g.
+000011f0: 7c00 5d06 7d01 7c01 8800 1900 9102 7102  |.].}.|.......q.
+00001200: 5300 7206 0000 0072 0600 0000 2902 7227  S.r....r....).r'
+00001210: 0000 00da 056c 6179 6572 a901 7239 0000  .....layer..r9..
+00001220: 0072 0600 0000 720a 0000 00da 0a3c 6c69  .r....r......<li
+00001230: 7374 636f 6d70 3e8d 0000 0073 0200 0000  stcomp>....s....
+00001240: 1400 7a2e 496e 7075 7451 7565 7565 2e62  ..z.InputQueue.b
+00001250: 7566 6665 7265 645f 696e 7075 7473 2e3c  uffered_inputs.<
+00001260: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00001270: 703e 2902 da04 6c69 7374 7203 0000 0029  p>)...listr....)
+00001280: 0572 0700 0000 7239 0000 0072 3f00 0000  .r....r9...r?...
+00001290: da06 6275 6666 6572 da06 7661 6c75 6573  ..buffer..values
+000012a0: 7206 0000 0072 4100 0000 720a 0000 00da  r....rA...r.....
+000012b0: 0f62 7566 6665 7265 645f 696e 7075 7473  .buffered_inputs
+000012c0: 8100 0000 7306 0000 0012 0b12 0108 017a  ....s..........z
+000012d0: 1a49 6e70 7574 5175 6575 652e 6275 6666  .InputQueue.buff
+000012e0: 6572 6564 5f69 6e70 7574 7363 0300 0000  ered_inputsc....
+000012f0: 0000 0000 0000 0000 0500 0000 0400 0000  ................
+00001300: 4300 0000 7314 0000 007c 00a0 007c 017c  C...s....|...|.|
+00001310: 02a1 025c 027d 037d 047c 0353 0072 1d00  ...\.}.}.|.S.r..
+00001320: 0000 a901 7246 0000 00a9 0572 0700 0000  ....rF.....r....
+00001330: 7239 0000 0072 3f00 0000 da06 7269 7369  r9...r?.....risi
+00001340: 6e67 da07 6661 6c6c 696e 6772 0600 0000  ng..fallingr....
+00001350: 7206 0000 0072 0a00 0000 da10 6275 6666  r....r......buff
+00001360: 6572 6564 5f70 7265 7373 6573 9000 0000  ered_presses....
+00001370: f304 0000 0010 0104 017a 1b49 6e70 7574  .........z.Input
+00001380: 5175 6575 652e 6275 6666 6572 6564 5f70  Queue.buffered_p
+00001390: 7265 7373 6573 6303 0000 0000 0000 0000  ressesc.........
+000013a0: 0000 0005 0000 0004 0000 0043 0000 0073  ...........C...s
+000013b0: 1400 0000 7c00 a000 7c01 7c02 a102 5c02  ....|...|.|...\.
+000013c0: 7d03 7d04 7c04 5300 721d 0000 0072 4700  }.}.|.S.r....rG.
+000013d0: 0000 7248 0000 0072 0600 0000 7206 0000  ..rH...r....r...
+000013e0: 0072 0a00 0000 da11 6275 6666 6572 6564  .r......buffered
+000013f0: 5f72 656c 6561 7365 7394 0000 0072 4c00  _releases....rL.
+00001400: 0000 7a1c 496e 7075 7451 7565 7565 2e62  ..z.InputQueue.b
+00001410: 7566 6665 7265 645f 7265 6c65 6173 6573  uffered_releases
+00001420: 2901 7212 0000 0029 1472 0c00 0000 720d  ).r....).r....r.
+00001430: 0000 0072 0e00 0000 720f 0000 0072 1500  ...r....r....r..
+00001440: 0000 da0c 4368 616e 6e65 6c54 7570 6c65  ....ChannelTuple
+00001450: 721c 0000 0072 1f00 0000 7222 0000 0072  r....r....r"...r
+00001460: 3500 0000 7236 0000 0072 1000 0000 723b  5...r6...r....r;
+00001470: 0000 0072 3d00 0000 723e 0000 0072 3100  ...r=...r>...r1.
+00001480: 0000 7246 0000 0072 4b00 0000 724d 0000  ..rF...rK...rM..
+00001490: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
+000014a0: 7206 0000 0072 0600 0000 7217 0000 0072  r....r....r....r
+000014b0: 0a00 0000 7211 0000 0019 0000 0073 1c00  ....r........s..
+000014c0: 0000 0800 0401 0e09 0e03 080a 0e03 0e09  ................
+000014d0: 0e15 0e12 0e0a 0e0a 1e0a 080f 1004 7211  ..............r.
+000014e0: 0000 004e 290b da0b 636f 6c6c 6563 7469  ...N)...collecti
+000014f0: 6f6e 7372 0200 0000 da0f 726f 6269 6e67  onsr......robing
+00001500: 616d 652e 7574 696c 7372 0300 0000 7210  ame.utilsr....r.
+00001510: 0000 00da 0566 6c6f 6174 da0c 496e 7075  .....float..Inpu
+00001520: 7443 6861 6e6e 656c 7231 0000 0072 4e00  tChannelr1...rN.
+00001530: 0000 7204 0000 0072 1100 0000 7206 0000  ..r....r....r...
+00001540: 0072 0600 0000 7206 0000 0072 0a00 0000  .r....r....r....
+00001550: da08 3c6d 6f64 756c 653e 0100 0000 730c  ..<module>....s.
+00001560: 0000 000c 000c 0208 050c 0410 0314 0a    ...............
```

### Comparing `robingame-0.1.0/robingame/input/event.py` & `robingame-1.0.1/robingame/input/event.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 from dataclasses import dataclass, is_dataclass, asdict
 from typing import Union
 
 import pygame
-from pygame.event import EventType, Event
+from pygame.event import EventType, Event as PygameEvent
 
 from robingame.image import init_display
 
 init_display()
 
 
 class EventQueue:
-    """Pygame's pygame.event.get() gets the events in the queue, but also empties the queue. This
-    class solves that"""
+    """
+    Pygame's pygame.event.get() empties the queue, which makes it impossible to listen to events
+    in more than one location. This class solves that with a sort of singleton approach.
+    """
 
     # this is intentional. I want to store the events on the class. Only one game will be active
     # at once, so we'll never need more than one instance of this class.
     events = []
 
     @classmethod
     def add(cls, event: Union[EventType, "dataclass"]):
         """
         Add the event to pygame's event queue, where it will stay until the .update() method
         is called to load it into cls.events.
 
         This prevents race conditions / order dependency where an event is added to the event
         queue and processed in the same tick.
+
+        Args:
+            event: object representing the event.
+                Can be a `pygame.Event`, or a dataclass with
+                attribute `type = pygame.event.custom_type()`
         """
         if is_dataclass(event):
-            event = Event(event.type, **asdict(event))
+            event = PygameEvent(event.type, **asdict(event))
         pygame.event.post(event)
 
     @classmethod
     def update(cls):
         """
         Read all the events from pygame's event queue into cls.events
         (also clears pygame's event queue)
         """
         cls.events = pygame.event.get()
 
     @classmethod
-    def filter(cls, **kwargs):
+    def filter(cls, **kwargs) -> list[EventType]:
         return [
             event
             for event in cls.events
             if all(getattr(event, attribute, None) == value for attribute, value in kwargs.items())
         ]
 
     @classmethod
-    def get(cls, **kwargs):
+    def get(cls, **kwargs) -> EventType | None:
         try:
             return cls.filter(**kwargs)[0]
         except IndexError:
             return None
```

### Comparing `robingame-0.1.0/robingame/input/gamecube.py` & `robingame-1.0.1/robingame/input/gamecube.py`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/input/queue.py` & `robingame-1.0.1/robingame/objects/game.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,99 @@
-from collections import deque
+import sys
 
-from robingame.utils import count_edges
+import pygame
+from pygame.color import Color
+from pygame.surface import Surface
 
+from robingame.input import EventQueue
+from robingame.objects.entity import Entity
+from robingame.objects.helpers import FpsTracker
 
-class Empty(tuple):
-    """Mock tuple of 0/1s that always returns a 0 no matter the index. This is used to
-    spoof an empty pygame.key.get_pressed() tuple."""
 
-    def __getitem__(self, *args, **kwargs) -> int:
-        return 0
+class Game(Entity):
+    """
+    Special case of Entity; it is at the very top of the object tree.
 
+    Handles much of the pygame boilerplate setup, including:
 
-class InputQueue(deque):
-    """
-    Provides additional functionality beyond pygame.key.get_pressed().
-    - Maintains a buffer of the last few inputs
-    - Calculates which keys have been pressed and released this tick
+    - initialising the display
+    - setting up and running the main game loop.
+    - doing `clock.tick()` every iteration and enforcing the framerate
+    - filling the screen with `self.screen_color` every iteration
+    - updating the EventQueue with new events
+    - maintaining the FPS tracker (and drawing it in debug mode)
     """
 
-    def __init__(self, queue_length=5):
-        super().__init__(maxlen=queue_length)
-
-    def get_new_values(self) -> tuple[int]:
-        """Subclasses should implement this. It should be something like
-        pygame.key.get_pressed()"""
-        raise NotImplementedError
-
-    def read_new_inputs(self):
-        self.append(self.get_new_values())
-
-    def get_down(self) -> tuple[int]:
-        """Return the keys which are currently held down"""
-        return self[-1] if len(self) > 0 else Empty()
-
-    def get_pressed(self) -> tuple[int]:
-        """Return the keys that have just been pressed---i.e. those that are down this tick but
-        not the previous tick"""
-        try:
-            current = self[-1]
-            previous = self[-2]
-            # we HAVE to use the __getattr__ method of the ScancodeWrapper
-            # here. Using for/in to iterate over it gives erroneous results!
-            # That's why I'm using the index to get the values.
-            return tuple(
-                int(current[i] and not previous[i])
-                for (i, c), p in zip(enumerate(current), previous)
-            )
-        except IndexError:
-            return Empty()
-
-    def get_released(self) -> tuple[int]:
-        """Return the keys that have just been released---i.e. those that are not down this
-        tick, but were down the previous tick"""
-        try:
-            current = self[-1]
-            previous = self[-2]
-            return tuple(
-                int(previous[i] and not current[i])
-                for (i, c), p in zip(enumerate(current), previous)
-            )
-        except IndexError:
-            return Empty()
-
-    def is_pressed(self, key) -> int:
-        """Check if a key has been pressed this tick"""
-        keys = self.get_pressed()
-        return keys[key]
-
-    def is_down(self, key) -> int:
-        """Check if a key is currently held down"""
-        keys = self.get_down()
-        return keys[key]
-
-    def is_released(self, key) -> int:
-        """Check if a key has been released this tick"""
-        keys = self.get_released()
-        return keys[key]
-
-    def buffered_inputs(self, key, buffer_length):
-        """Count the rising and falling edges. Can be used to detect past inputs."""
-        buffer = list(self)[-buffer_length:]
-        values = [layer[key] for layer in buffer]
-        return count_edges(values)
-
-    def buffered_presses(self, key, buffer_length):
-        rising, falling = self.buffered_inputs(key, buffer_length)
-        return rising
-
-    def buffered_releases(self, key, buffer_length):
-        rising, falling = self.buffered_inputs(key, buffer_length)
-        return falling
+    fps: int = 60
+    window_width: int = 500
+    window_height: int = 500
+    window_caption: str = "Game"
+    screen_color = Color("black")
+    debug: bool = False  # draw / print debug info?
+    running: bool  # is the main game loop running
+
+    def __init__(self):
+        """
+        Handles a lot of the boilerplate pygame setup.
+        Creates the display (`self.window`).
+        """
+        super().__init__()
+        pygame.init()
+        self.fps_tracker = FpsTracker()
+        self.window = pygame.display.set_mode((self.window_width, self.window_height))
+        pygame.display.set_caption(self.window_caption)
+        self.clock = pygame.time.Clock()
+
+    def main(self):
+        """
+        Contains the main game loop.
+        Calls `self._update()` and `self._draw()` on every iteration of the game loop.
+        """
+        self.running = True
+        while self.running:
+            self._update()
+            self._draw(self.window, debug=self.debug)
+        pygame.quit()
+        sys.exit()
+
+    def read_inputs(self):
+        """
+        Called by `self._update()`, before `super().update()` updates the children.
+
+        Any code that polls external joysticks/controllers should go here.
+        """
+
+        # I've put this in a separate method because I don't like the idea of putting the inputs
+        # in the same list as other child groups. The order might get ruined, or a subclass might
+        # overwrite the list. It's crucial that the inputs are read before updating.
+        EventQueue.update()
+        for event in EventQueue.events:
+            if event.type == pygame.QUIT:
+                pygame.quit()
+                sys.exit()
+            if event.type == pygame.KEYDOWN and event.key == pygame.K_F1:
+                self.debug = not self.debug
+
+    def print_debug_info(self):
+        """
+        Override this if you want to print any debug info.
+        """
+        pass
+
+    def _update(self):
+        """
+        1. read inputs
+        2. update
+        """
+        self.read_inputs()
+        if self.debug:
+            self.print_debug_info()
+        self.update()
+        self.fps_tracker.update()
+        if self.fps:
+            self.clock.tick(self.fps)
+
+    def _draw(self, surface: Surface, debug: bool = False):
+        surface.fill(self.screen_color)  # clear the screen
+        self.draw(surface, debug)
+        self.fps_tracker.draw(surface, debug)
+        pygame.display.update()  # print to screen
```

### Comparing `robingame-0.1.0/robingame/input/visualization.py` & `robingame-1.0.1/robingame/input/visualization.py`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/objects/__pycache__/entity.cpython-310.pyc` & `robingame-1.0.1/robingame/objects/__pycache__/entity.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jul  5 13:47:52 2023 UTC, .py size: 2755 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8874 a564 c30a 0000  o........t.d....
+00000000: 6f0d 0d0a 0000 0000 b1c6 b364 330d 0000  o..........d3...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a03 6400 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6404 6c05 6d06 5a06 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 6503 6a07 6a08 8303  d.d...d.e.j.j...
 00000070: 5a09 6402 5300 2907 e900 0000 0029 02da  Z.d.S.)......)..
@@ -17,173 +17,228 @@
 00000100: 650b 6508 1900 6602 8700 6601 640a 640b  e.e...f...f.d.d.
 00000110: 840d 5a0c 640c 640d 8400 5a0d 641b 640f  ..Z.d.d...Z.d.d.
 00000120: 650e 6410 650f 6604 6411 6412 8405 5a10  e.d.e.f.d.d...Z.
 00000130: 8700 6601 6413 6414 8408 5a11 6512 6415  ..f.d.d...Z.e.d.
 00000140: 6416 8400 8301 5a13 6513 6a14 6417 6416  d.....Z.e.j.d.d.
 00000150: 8400 8301 5a13 6418 6419 8400 5a15 8700  ....Z.d.d...Z...
 00000160: 0400 5a16 5300 291c da06 456e 7469 7479  ..Z.S.)...Entity
-00000170: 7571 0300 000a 2020 2020 4669 6e69 7465  uq....    Finite
+00000170: 758e 0300 000a 2020 2020 4669 6e69 7465  u.....    Finite
 00000180: 2053 7461 7465 204d 6163 6869 6e65 3a0a   State Machine:.
-00000190: 2020 2020 2d20 7365 6c66 2e73 7461 7465      - self.state
-000001a0: 2069 7320 6578 6563 7574 6564 2065 7665   is executed eve
-000001b0: 7279 2074 6963 6b0a 2020 2020 2d20 7365  ry tick.    - se
-000001c0: 6c66 2e74 6963 6b20 6973 2069 6e63 7265  lf.tick is incre
-000001d0: 6d65 6e74 6564 2065 7665 7279 2074 696d  mented every tim
-000001e0: 6520 7468 6520 6d61 696e 2067 616d 6520  e the main game 
-000001f0: 6c6f 6f70 2065 7865 6375 7465 730a 2020  loop executes.  
-00000200: 2020 2d20 7768 656e 2073 656c 662e 7374    - when self.st
-00000210: 6174 6520 6368 616e 6765 732c 2073 656c  ate changes, sel
-00000220: 662e 7469 636b 2069 7320 7365 7420 746f  f.tick is set to
-00000230: 2030 2c20 736f 2079 6f75 2063 616e 2074   0, so you can t
-00000240: 7261 636b 2068 6f77 206c 6f6e 6720 7468  rack how long th
-00000250: 6520 656e 7469 7479 2068 6173 0a20 2020  e entity has.   
-00000260: 2020 2062 6565 6e20 696e 2069 7473 2063     been in its c
-00000270: 7572 7265 6e74 2073 7461 7465 0a0a 2020  urrent state..  
-00000280: 2020 4869 6572 6172 6368 6963 616c 2073    Hierarchical s
-00000290: 7472 7563 7475 7265 3a0a 2020 2020 2d20  tructure:.    - 
-000002a0: 456e 7469 7469 6573 2063 616e 2062 6520  Entities can be 
-000002b0: 6164 6465 6420 746f 2047 726f 7570 7320  added to Groups 
-000002c0: 746f 2063 7265 6174 6520 6120 6869 6572  to create a hier
-000002d0: 6172 6368 6963 616c 2073 7472 7563 7475  archical structu
-000002e0: 7265 0a20 2020 202d 2054 6865 206f 7264  re.    - The ord
-000002f0: 6572 206f 6620 6772 6f75 7073 2069 6e20  er of groups in 
-00000300: 7468 6520 2e63 6869 6c64 5f67 726f 7570  the .child_group
-00000310: 7320 6174 7472 6962 7574 6520 6465 7465  s attribute dete
-00000320: 726d 696e 6573 2074 6865 2064 7261 7720  rmines the draw 
-00000330: 6f72 6465 723b 2069 7427 7320 6261 7369  order; it's basi
-00000340: 6361 6c6c 790a 2020 2020 2020 7468 6520  cally.      the 
-00000350: 6c61 7965 7273 0a0a 2020 2020 4578 616d  layers..    Exam
-00000360: 706c 6520 6761 6d65 2073 7472 7563 7475  ple game structu
-00000370: 7265 3a0a 2020 2020 4761 6d65 3a20 456e  re:.    Game: En
-00000380: 7469 7479 0a20 2020 20e2 9494 e294 80e2  tity.    .......
-00000390: 9480 2073 6365 6e65 733a 2047 726f 7570  .. scenes: Group
-000003a0: 0a20 2020 2020 2020 20e2 9494 e294 80e2  .        .......
-000003b0: 9480 204d 6169 6e4d 656e 753a 2045 6e74  .. MainMenu: Ent
-000003c0: 6974 790a 2020 2020 2020 2020 2020 2020  ity.            
-000003d0: e294 9ce2 9480 e294 8020 6275 7474 6f6e  ......... button
-000003e0: 733a 2047 726f 7570 0a20 2020 2020 2020  s: Group.       
-000003f0: 2020 2020 20e2 9482 2020 20e2 949c e294       ...   .....
-00000400: 80e2 9480 2042 7574 746f 6e3a 2045 6e74  .... Button: Ent
-00000410: 6974 790a 2020 2020 2020 2020 2020 2020  ity.            
-00000420: e294 8220 2020 e294 9ce2 9480 e294 8020  ...   ......... 
-00000430: 4275 7474 6f6e 3a20 456e 7469 7479 0a20  Button: Entity. 
-00000440: 2020 2020 2020 2020 2020 20e2 9482 2020             ...  
-00000450: 20e2 9494 e294 80e2 9480 2042 7574 746f   ......... Butto
-00000460: 6e3a 2045 6e74 6974 790a 2020 2020 2020  n: Entity.      
-00000470: 2020 2020 2020 e294 94e2 9480 e294 8020        ......... 
-00000480: 736c 6964 6572 733a 2047 726f 7570 0a20  sliders: Group. 
-00000490: 2020 2020 2020 2020 2020 2020 2020 20e2                 .
-000004a0: 949c e294 80e2 9480 2053 6c69 6465 723a  ........ Slider:
-000004b0: 2045 6e74 6974 790a 2020 2020 2020 2020   Entity.        
-000004c0: 2020 2020 2020 2020 e294 94e2 9480 e294          ........
-000004d0: 8020 536c 6964 6572 3a20 456e 7469 7479  . Slider: Entity
-000004e0: 0a0a 2020 2020 6300 0000 0000 0000 0000  ..    c.........
-000004f0: 0000 0002 0000 0001 0000 004f 0000 0073  ...........O...s
-00000500: 0400 0000 6400 5300 a901 4ea9 0029 02da  ....d.S...N..)..
-00000510: 0461 7267 73da 066b 7761 7267 7372 0800  .args..kwargsr..
-00000520: 0000 7208 0000 00fa 362f 686f 6d65 2f72  ..r.....6/home/r
-00000530: 6f62 696e 2f63 6f64 652f 726f 6269 6e67  obin/code/robing
-00000540: 616d 652f 726f 6269 6e67 616d 652f 6f62  ame/robingame/ob
-00000550: 6a65 6374 732f 656e 7469 7479 2e70 79da  jects/entity.py.
-00000560: 083c 6c61 6d62 6461 3e24 0000 0073 0200  .<lambda>$...s..
-00000570: 0000 0400 7a0f 456e 7469 7479 2e3c 6c61  ....z.Entity.<la
-00000580: 6d62 6461 3eda 065f 7374 6174 65da 0c63  mbda>.._state..c
-00000590: 6869 6c64 5f67 726f 7570 7372 0100 0000  hild_groupsr....
-000005a0: da04 7469 636b 7208 0000 00da 0667 726f  ..tickr......gro
-000005b0: 7570 7363 0200 0000 0000 0000 0000 0000  upsc............
-000005c0: 0200 0000 0200 0000 0300 0000 7316 0000  ............s...
-000005d0: 0074 0083 006a 017c 018e 0001 0067 007c  .t...j.|.....g.|
-000005e0: 005f 0264 0053 0072 0700 0000 2903 da05  ._.d.S.r....)...
-000005f0: 7375 7065 72da 085f 5f69 6e69 745f 5f72  super..__init__r
-00000600: 0e00 0000 2902 da04 7365 6c66 7210 0000  ....)...selfr...
-00000610: 00a9 01da 095f 5f63 6c61 7373 5f5f 7208  .....__class__r.
-00000620: 0000 0072 0b00 0000 7212 0000 0028 0000  ...r....r....(..
-00000630: 0073 0400 0000 0c01 0a01 7a0f 456e 7469  .s........z.Enti
-00000640: 7479 2e5f 5f69 6e69 745f 5f63 0100 0000  ty.__init__c....
-00000650: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000660: 4300 0000 732e 0000 007c 00a0 00a1 0001  C...s....|......
-00000670: 007c 006a 0144 005d 067d 017c 01a0 02a1  .|.j.D.].}.|....
-00000680: 0001 0071 077c 0004 006a 0364 0137 0002  ...q.|...j.d.7..
-00000690: 005f 0364 0053 0029 024e e901 0000 0029  ._.d.S.).N.....)
-000006a0: 04da 0573 7461 7465 720e 0000 00da 0675  ...stater......u
-000006b0: 7064 6174 6572 0f00 0000 a902 7213 0000  pdater......r...
-000006c0: 00da 0567 726f 7570 7208 0000 0072 0800  ...groupr....r..
-000006d0: 0000 720b 0000 0072 1800 0000 2c00 0000  ..r....r....,...
-000006e0: 7308 0000 0008 010a 030a 0112 017a 0d45  s............z.E
-000006f0: 6e74 6974 792e 7570 6461 7465 46da 0773  ntity.updateF..s
-00000700: 7572 6661 6365 da05 6465 6275 6763 0300  urface..debugc..
-00000710: 0000 0000 0000 0000 0000 0400 0000 0500  ................
-00000720: 0000 4300 0000 731c 0000 007c 006a 0044  ..C...s....|.j.D
-00000730: 005d 087d 037c 03a0 017c 017c 02a1 0201  .].}.|...|.|....
-00000740: 0071 0364 0053 0072 0700 0000 2902 720e  .q.d.S.r....).r.
-00000750: 0000 00da 0464 7261 7729 0472 1300 0000  .....draw).r....
-00000760: 721b 0000 0072 1c00 0000 721a 0000 0072  r....r....r....r
-00000770: 0800 0000 7208 0000 0072 0b00 0000 721d  ....r....r....r.
-00000780: 0000 0034 0000 0073 0600 0000 0a03 0e01  ...4...s........
-00000790: 04ff 7a0b 456e 7469 7479 2e64 7261 7763  ..z.Entity.drawc
-000007a0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000007b0: 0300 0000 0300 0000 7322 0000 007c 006a  ........s"...|.j
-000007c0: 0044 005d 067d 017c 01a0 01a1 0001 0071  .D.].}.|.......q
-000007d0: 0374 0283 00a0 01a1 0001 0064 0153 0029  .t.........d.S.)
-000007e0: 027a 2f52 656d 6f76 6573 2073 656c 6620  .z/Removes self 
-000007f0: 6672 6f6d 2061 6c6c 2067 726f 7570 7320  from all groups 
-00000800: 6974 2069 7320 6120 6d65 6d62 6572 206f  it is a member o
-00000810: 662e 4e29 0372 0e00 0000 da04 6b69 6c6c  f.N).r......kill
-00000820: 7211 0000 0072 1900 0000 7214 0000 0072  r....r....r....r
-00000830: 0800 0000 720b 0000 0072 1e00 0000 3a00  ....r....r....:.
-00000840: 0000 7306 0000 000a 020a 010e 017a 0b45  ..s..........z.E
-00000850: 6e74 6974 792e 6b69 6c6c 6301 0000 0000  ntity.killc.....
-00000860: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00000870: 0000 0073 0600 0000 7c00 6a00 5300 7207  ...s....|.j.S.r.
-00000880: 0000 0029 0172 0d00 0000 a901 7213 0000  ...).r......r...
-00000890: 0072 0800 0000 7208 0000 0072 0b00 0000  .r....r....r....
-000008a0: 7217 0000 0040 0000 0073 0200 0000 0602  r....@...s......
-000008b0: 7a0c 456e 7469 7479 2e73 7461 7465 6302  z.Entity.statec.
-000008c0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-000008d0: 0000 0043 0000 0073 1000 0000 7c01 7c00  ...C...s....|.|.
-000008e0: 5f00 6401 7c00 5f01 6402 5300 2903 7a69  _.d.|._.d.S.).zi
-000008f0: 0a20 2020 2020 2020 2052 6573 6574 2073  .        Reset s
-00000900: 656c 662e 7469 636b 2077 6865 6e20 7374  elf.tick when st
-00000910: 6174 6520 6368 616e 6765 7320 736f 2077  ate changes so w
-00000920: 6520 6b6e 6f77 2068 6f77 206c 6f6e 6720  e know how long 
-00000930: 7765 2776 6520 6265 656e 2069 6e20 7468  we've been in th
-00000940: 6520 6375 7272 656e 7420 7374 6174 652e  e current state.
-00000950: 0a20 2020 2020 2020 2072 0100 0000 4e29  .        r....N)
-00000960: 0272 0d00 0000 720f 0000 0029 0272 1300  .r....r....).r..
-00000970: 0000 da09 6e65 775f 7374 6174 6572 0800  ....new_stater..
-00000980: 0000 7208 0000 0072 0b00 0000 7217 0000  ..r....r....r...
-00000990: 0044 0000 0073 0400 0000 0605 0a01 6301  .D...s........c.
-000009a0: 0000 0000 0000 0000 0000 0001 0000 0005  ................
-000009b0: 0000 0043 0000 0073 1c00 0000 6401 7c00  ...C...s....d.|.
-000009c0: 6a00 6a01 9b00 6402 7402 7c00 6a03 8301  j.j...d.t.|.j...
-000009d0: 9b00 6403 9d05 5300 2904 4efa 013c 7a0b  ..d...S.).N..<z.
-000009e0: 2045 6e74 6974 7928 696e 207a 0920 6772   Entity(in z. gr
-000009f0: 6f75 7073 293e 2904 7215 0000 00da 085f  oups)>).r......_
-00000a00: 5f6e 616d 655f 5fda 036c 656e da0a 5f53  _name__..len.._S
-00000a10: 7072 6974 655f 5f67 721f 0000 0072 0800  prite__gr....r..
-00000a20: 0000 7208 0000 0072 0b00 0000 da08 5f5f  ..r....r......__
-00000a30: 7265 7072 5f5f 4c00 0000 7302 0000 001c  repr__L...s.....
-00000a40: 027a 0f45 6e74 6974 792e 5f5f 7265 7072  .z.Entity.__repr
-00000a50: 5f5f 2901 7208 0000 0029 0146 2917 7222  __).r....).F).r"
-00000a60: 0000 00da 0a5f 5f6d 6f64 756c 655f 5fda  .....__module__.
-00000a70: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
-00000a80: 5f64 6f63 5f5f 720d 0000 0072 0200 0000  _doc__r....r....
-00000a90: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
-00000aa0: 5fda 046c 6973 7472 0500 0000 720f 0000  _..listr....r...
-00000ab0: 00da 0369 6e74 7203 0000 0072 1200 0000  ...intr....r....
-00000ac0: 7218 0000 0072 0400 0000 da04 626f 6f6c  r....r......bool
-00000ad0: 721d 0000 0072 1e00 0000 da08 7072 6f70  r....r......prop
-00000ae0: 6572 7479 7217 0000 00da 0673 6574 7465  ertyr......sette
-00000af0: 7272 2500 0000 da0d 5f5f 636c 6173 7363  rr%.....__classc
-00000b00: 656c 6c5f 5f72 0800 0000 7208 0000 0072  ell__r....r....r
-00000b10: 1400 0000 720b 0000 0072 0600 0000 0900  ....r....r......
-00000b20: 0000 731c 0000 000a 0004 0110 1a0c 010c  ..s.............
-00000b30: 0118 0208 0414 080c 0602 060a 0104 030a  ................
-00000b40: 0110 0772 0600 0000 290a da06 7479 7069  ...r....)...typi
-00000b50: 6e67 7202 0000 0072 0300 0000 da06 7079  ngr....r......py
-00000b60: 6761 6d65 7204 0000 00da 1772 6f62 696e  gamer......robin
-00000b70: 6761 6d65 2e6f 626a 6563 7473 2e67 726f  game.objects.gro
-00000b80: 7570 7205 0000 00da 0673 7072 6974 65da  upr......sprite.
-00000b90: 0653 7072 6974 6572 0600 0000 7208 0000  .Spriter....r...
-00000ba0: 0072 0800 0000 7208 0000 0072 0b00 0000  .r....r....r....
-00000bb0: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
-00000bc0: 0000 0010 0008 020c 010c 0218 03         .............
+00000190: 0a20 2020 202d 2060 7365 6c66 2e73 7461  .    - `self.sta
+000001a0: 7465 6020 6973 2065 7865 6375 7465 6420  te` is executed 
+000001b0: 6576 6572 7920 7469 636b 0a20 2020 202d  every tick.    -
+000001c0: 2060 7365 6c66 2e74 6963 6b60 2069 7320   `self.tick` is 
+000001d0: 696e 6372 656d 656e 7465 6420 6576 6572  incremented ever
+000001e0: 7920 7469 6d65 2074 6865 206d 6169 6e20  y time the main 
+000001f0: 6761 6d65 206c 6f6f 7020 6578 6563 7574  game loop execut
+00000200: 6573 0a20 2020 202d 2077 6865 6e20 6073  es.    - when `s
+00000210: 656c 662e 7374 6174 6560 2063 6861 6e67  elf.state` chang
+00000220: 6573 2c20 6073 656c 662e 7469 636b 6020  es, `self.tick` 
+00000230: 6973 2073 6574 2074 6f20 302c 2073 6f20  is set to 0, so 
+00000240: 796f 7520 6361 6e20 7472 6163 6b20 686f  you can track ho
+00000250: 7720 6c6f 6e67 2074 6865 2065 6e74 6974  w long the entit
+00000260: 7920 6861 730a 2020 2020 2020 6265 656e  y has.      been
+00000270: 2069 6e20 6974 7320 6375 7272 656e 7420   in its current 
+00000280: 7374 6174 650a 0a20 2020 2048 6965 7261  state..    Hiera
+00000290: 7263 6869 6361 6c20 7374 7275 6374 7572  rchical structur
+000002a0: 653a 0a0a 2020 2020 2d20 6045 6e74 6974  e:..    - `Entit
+000002b0: 6965 7360 2063 616e 2062 6520 6164 6465  ies` can be adde
+000002c0: 6420 746f 2060 4772 6f75 7073 6020 746f  d to `Groups` to
+000002d0: 2063 7265 6174 6520 6120 6869 6572 6172   create a hierar
+000002e0: 6368 6963 616c 2073 7472 7563 7475 7265  chical structure
+000002f0: 0a20 2020 202d 2054 6865 206f 7264 6572  .    - The order
+00000300: 206f 6620 6772 6f75 7073 2069 6e20 7468   of groups in th
+00000310: 6520 2e63 6869 6c64 5f67 726f 7570 7320  e .child_groups 
+00000320: 6174 7472 6962 7574 6520 6465 7465 726d  attribute determ
+00000330: 696e 6573 2074 6865 2064 7261 7720 6f72  ines the draw or
+00000340: 6465 723b 2069 7427 7320 6261 7369 6361  der; it's basica
+00000350: 6c6c 790a 2020 2020 2020 7468 6520 6c61  lly.      the la
+00000360: 7965 7273 0a0a 2020 2020 4578 616d 706c  yers..    Exampl
+00000370: 6520 6761 6d65 2073 7472 7563 7475 7265  e game structure
+00000380: 3a0a 2020 2020 6060 600a 2020 2020 4761  :.    ```.    Ga
+00000390: 6d65 3a20 456e 7469 7479 0a20 2020 20e2  me: Entity.    .
+000003a0: 9494 e294 80e2 9480 2073 6365 6e65 733a  ........ scenes:
+000003b0: 2047 726f 7570 0a20 2020 2020 2020 20e2   Group.        .
+000003c0: 9494 e294 80e2 9480 204d 6169 6e4d 656e  ........ MainMen
+000003d0: 753a 2045 6e74 6974 790a 2020 2020 2020  u: Entity.      
+000003e0: 2020 2020 2020 e294 9ce2 9480 e294 8020        ......... 
+000003f0: 6275 7474 6f6e 733a 2047 726f 7570 0a20  buttons: Group. 
+00000400: 2020 2020 2020 2020 2020 20e2 9482 2020             ...  
+00000410: 20e2 949c e294 80e2 9480 2042 7574 746f   ......... Butto
+00000420: 6e3a 2045 6e74 6974 790a 2020 2020 2020  n: Entity.      
+00000430: 2020 2020 2020 e294 8220 2020 e294 9ce2        ...   ....
+00000440: 9480 e294 8020 4275 7474 6f6e 3a20 456e  ..... Button: En
+00000450: 7469 7479 0a20 2020 2020 2020 2020 2020  tity.           
+00000460: 20e2 9482 2020 20e2 9494 e294 80e2 9480   ...   .........
+00000470: 2042 7574 746f 6e3a 2045 6e74 6974 790a   Button: Entity.
+00000480: 2020 2020 2020 2020 2020 2020 e294 94e2              ....
+00000490: 9480 e294 8020 736c 6964 6572 733a 2047  ..... sliders: G
+000004a0: 726f 7570 0a20 2020 2020 2020 2020 2020  roup.           
+000004b0: 2020 2020 20e2 949c e294 80e2 9480 2053       ......... S
+000004c0: 6c69 6465 723a 2045 6e74 6974 790a 2020  lider: Entity.  
+000004d0: 2020 2020 2020 2020 2020 2020 2020 e294                ..
+000004e0: 94e2 9480 e294 8020 536c 6964 6572 3a20  ....... Slider: 
+000004f0: 456e 7469 7479 0a20 2020 2060 6060 0a20  Entity.    ```. 
+00000500: 2020 2063 0000 0000 0000 0000 0000 0000     c............
+00000510: 0200 0000 0100 0000 4f00 0000 7304 0000  ........O...s...
+00000520: 0064 0053 00a9 014e a900 2902 da04 6172  .d.S...N..)...ar
+00000530: 6773 da06 6b77 6172 6773 7208 0000 0072  gs..kwargsr....r
+00000540: 0800 0000 fa36 2f68 6f6d 652f 726f 6269  .....6/home/robi
+00000550: 6e2f 636f 6465 2f72 6f62 696e 6761 6d65  n/code/robingame
+00000560: 2f72 6f62 696e 6761 6d65 2f6f 626a 6563  /robingame/objec
+00000570: 7473 2f65 6e74 6974 792e 7079 da08 3c6c  ts/entity.py..<l
+00000580: 616d 6264 613e 2700 0000 7302 0000 0004  ambda>'...s.....
+00000590: 007a 0f45 6e74 6974 792e 3c6c 616d 6264  .z.Entity.<lambd
+000005a0: 613e da06 5f73 7461 7465 da0c 6368 696c  a>.._state..chil
+000005b0: 645f 6772 6f75 7073 7201 0000 00da 0474  d_groupsr......t
+000005c0: 6963 6b72 0800 0000 da06 6772 6f75 7073  ickr......groups
+000005d0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+000005e0: 0002 0000 0003 0000 0073 1600 0000 7400  .........s....t.
+000005f0: 8300 6a01 7c01 8e00 0100 6700 7c00 5f02  ..j.|.....g.|._.
+00000600: 6400 5300 7207 0000 0029 03da 0573 7570  d.S.r....)...sup
+00000610: 6572 da08 5f5f 696e 6974 5f5f 720e 0000  er..__init__r...
+00000620: 0029 02da 0473 656c 6672 1000 0000 a901  .)...selfr......
+00000630: da09 5f5f 636c 6173 735f 5f72 0800 0000  ..__class__r....
+00000640: 720b 0000 0072 1200 0000 2b00 0000 7304  r....r....+...s.
+00000650: 0000 000c 010a 017a 0f45 6e74 6974 792e  .......z.Entity.
+00000660: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
+00000670: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00000680: 0073 2e00 0000 7c00 a000 a100 0100 7c00  .s....|.......|.
+00000690: 6a01 4400 5d06 7d01 7c01 a002 a100 0100  j.D.].}.|.......
+000006a0: 7107 7c00 0400 6a03 6401 3700 0200 5f03  q.|...j.d.7..._.
+000006b0: 6402 5300 2903 610f 0200 000a 2020 2020  d.S.).a.....    
+000006c0: 2020 2020 4578 6563 7574 6520 6073 656c      Execute `sel
+000006d0: 662e 7374 6174 6560 2e0a 0a20 2020 2020  f.state`...     
+000006e0: 2020 2043 616c 6c20 602e 7570 6461 7465     Call `.update
+000006f0: 2829 6020 6f6e 2061 6c6c 2063 6869 6c64  ()` on all child
+00000700: 2067 726f 7570 732e 2054 6869 7320 616c   groups. This al
+00000710: 6c6f 7773 2074 6865 2065 6e74 6972 6520  lows the entire 
+00000720: 7472 6565 206f 6620 6f62 6a65 6374 7320  tree of objects 
+00000730: 746f 2075 7064 6174 6520 6279 0a20 2020  to update by.   
+00000740: 2020 2020 206f 6e6c 7920 6361 6c6c 696e       only callin
+00000750: 6720 7468 6520 602e 7570 6461 7465 2829  g the `.update()
+00000760: 6020 6d65 7468 6f64 206f 6620 7468 6520  ` method of the 
+00000770: 726f 6f74 206f 626a 6563 742e 0a0a 2020  root object...  
+00000780: 2020 2020 2020 5375 6263 6c61 7373 6573        Subclasses
+00000790: 2063 616e 206f 7665 7272 6964 6520 7468   can override th
+000007a0: 6973 206d 6574 686f 6420 746f 2070 726f  is method to pro
+000007b0: 7669 6465 2073 7562 636c 6173 732d 7370  vide subclass-sp
+000007c0: 6563 6966 6963 2062 6568 6176 696f 7572  ecific behaviour
+000007d0: 2e20 486f 7765 7665 722c 0a20 2020 2020  . However,.     
+000007e0: 2020 2069 7427 7320 6765 6e65 7261 6c6c     it's generall
+000007f0: 7920 6120 6265 7474 6572 2069 6465 6120  y a better idea 
+00000800: 746f 2077 7269 7465 2073 7461 7465 2066  to write state f
+00000810: 756e 6374 696f 6e73 2061 6e64 2061 6c6c  unctions and all
+00000820: 6f77 2074 6865 2045 6e74 6974 7927 7320  ow the Entity's 
+00000830: 4669 6e69 7465 2053 7461 7465 0a20 2020  Finite State.   
+00000840: 2020 2020 204d 6163 6869 6e65 206d 6563       Machine mec
+00000850: 6861 6e69 736d 2074 6f20 6578 6563 7574  hanism to execut
+00000860: 6520 7468 656d 2e0a 0a20 2020 2020 2020  e them...       
+00000870: 2049 6e63 7265 6d65 6e74 2060 7365 6c66   Increment `self
+00000880: 2e74 6963 6b60 2074 6f20 6b65 6570 2074  .tick` to keep t
+00000890: 7261 636b 206f 6620 686f 7720 6c6f 6e67  rack of how long
+000008a0: 2077 6527 7665 2062 6565 6e20 696e 2074   we've been in t
+000008b0: 6865 2063 7572 7265 6e74 2073 7461 7465  he current state
+000008c0: 2e0a 2020 2020 2020 2020 e901 0000 004e  ..        .....N
+000008d0: 2904 da05 7374 6174 6572 0e00 0000 da06  )...stater......
+000008e0: 7570 6461 7465 720f 0000 00a9 0272 1300  updater......r..
+000008f0: 0000 da05 6772 6f75 7072 0800 0000 7208  ....groupr....r.
+00000900: 0000 0072 0b00 0000 7218 0000 002f 0000  ...r....r..../..
+00000910: 0073 0800 0000 080d 0a01 0a01 1201 7a0d  .s............z.
+00000920: 456e 7469 7479 2e75 7064 6174 6546 da07  Entity.updateF..
+00000930: 7375 7266 6163 65da 0564 6562 7567 6303  surface..debugc.
+00000940: 0000 0000 0000 0000 0000 0004 0000 0005  ................
+00000950: 0000 0043 0000 0073 1c00 0000 7c00 6a00  ...C...s....|.j.
+00000960: 4400 5d08 7d03 7c03 a001 7c01 7c02 a102  D.].}.|...|.|...
+00000970: 0100 7103 6401 5300 2902 612d 0100 000a  ..q.d.S.).a-....
+00000980: 2020 2020 2020 2020 4472 6177 2061 6c6c          Draw all
+00000990: 2063 6869 6c64 2067 726f 7570 732e 2054   child groups. T
+000009a0: 6869 7320 616c 6c6f 7773 2074 6865 2065  his allows the e
+000009b0: 6e74 6972 6520 7472 6565 206f 6620 6f62  ntire tree of ob
+000009c0: 6a65 6374 7320 746f 2064 7261 7720 6279  jects to draw by
+000009d0: 206f 6e6c 7920 6361 6c6c 696e 6720 7468   only calling th
+000009e0: 650a 2020 2020 2020 2020 2e64 7261 7728  e.        .draw(
+000009f0: 2920 6d65 7468 6f64 206f 6620 7468 6520  ) method of the 
+00000a00: 726f 6f74 206f 626a 6563 742e 0a0a 0a20  root object.... 
+00000a10: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00000a20: 2020 2020 2020 2020 2073 7572 6661 6365           surface
+00000a30: 3a20 7468 6520 7375 7266 6163 6520 2875  : the surface (u
+00000a40: 7375 616c 6c79 2074 6865 2073 6372 6565  sually the scree
+00000a50: 6e29 206f 6e20 7768 6963 6820 746f 2064  n) on which to d
+00000a60: 7261 7720 7365 6c66 0a20 2020 2020 2020  raw self.       
+00000a70: 2020 2020 2064 6562 7567 3a20 6966 2054       debug: if T
+00000a80: 7275 652c 2064 7261 7720 6578 7472 6120  rue, draw extra 
+00000a90: 7374 7566 6620 666f 7220 6465 6275 6767  stuff for debugg
+00000aa0: 696e 670a 2020 2020 2020 2020 4e29 0272  ing.        N).r
+00000ab0: 0e00 0000 da04 6472 6177 2904 7213 0000  ......draw).r...
+00000ac0: 0072 1b00 0000 721c 0000 0072 1a00 0000  .r....r....r....
+00000ad0: 7208 0000 0072 0800 0000 720b 0000 0072  r....r....r....r
+00000ae0: 1d00 0000 4100 0000 7306 0000 000a 0a0e  ....A...s.......
+00000af0: 0104 ff7a 0b45 6e74 6974 792e 6472 6177  ...z.Entity.draw
+00000b00: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000b10: 0003 0000 0003 0000 0073 2200 0000 7c00  .........s"...|.
+00000b20: 6a00 4400 5d06 7d01 7c01 a001 a100 0100  j.D.].}.|.......
+00000b30: 7103 7402 8300 a001 a100 0100 6401 5300  q.t.........d.S.
+00000b40: 2902 7a1d 5265 6d6f 7665 7320 7365 6c66  ).z.Removes self
+00000b50: 2066 726f 6d20 616c 6c20 6772 6f75 7073   from all groups
+00000b60: 2e4e 2903 720e 0000 00da 046b 696c 6c72  .N).r......killr
+00000b70: 1100 0000 7219 0000 0072 1400 0000 7208  ....r....r....r.
+00000b80: 0000 0072 0b00 0000 721e 0000 004e 0000  ...r....r....N..
+00000b90: 0073 0600 0000 0a02 0a01 0e01 7a0b 456e  .s..........z.En
+00000ba0: 7469 7479 2e6b 696c 6c63 0100 0000 0000  tity.killc......
+00000bb0: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00000bc0: 0000 7306 0000 007c 006a 0053 0029 017a  ..s....|.j.S.).z
+00000bd0: 2345 7865 6375 7465 2074 6865 2063 7572  #Execute the cur
+00000be0: 7265 6e74 2073 7461 7465 2066 756e 6374  rent state funct
+00000bf0: 696f 6e2e 2901 720d 0000 00a9 0172 1300  ion.).r......r..
+00000c00: 0000 7208 0000 0072 0800 0000 720b 0000  ..r....r....r...
+00000c10: 0072 1700 0000 5400 0000 7302 0000 0006  .r....T...s.....
+00000c20: 037a 0c45 6e74 6974 792e 7374 6174 6563  .z.Entity.statec
+00000c30: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000c40: 0200 0000 4300 0000 7310 0000 007c 017c  ....C...s....|.|
+00000c50: 005f 0064 017c 005f 0164 0253 0029 037a  ._.d.|._.d.S.).z
+00000c60: 690a 2020 2020 2020 2020 5265 7365 7420  i.        Reset 
+00000c70: 7365 6c66 2e74 6963 6b20 7768 656e 2073  self.tick when s
+00000c80: 7461 7465 2063 6861 6e67 6573 2073 6f20  tate changes so 
+00000c90: 7765 206b 6e6f 7720 686f 7720 6c6f 6e67  we know how long
+00000ca0: 2077 6527 7665 2062 6565 6e20 696e 2074   we've been in t
+00000cb0: 6865 2063 7572 7265 6e74 2073 7461 7465  he current state
+00000cc0: 2e0a 2020 2020 2020 2020 7201 0000 004e  ..        r....N
+00000cd0: 2902 720d 0000 0072 0f00 0000 2902 7213  ).r....r....).r.
+00000ce0: 0000 00da 096e 6577 5f73 7461 7465 7208  .....new_stater.
+00000cf0: 0000 0072 0800 0000 720b 0000 0072 1700  ...r....r....r..
+00000d00: 0000 5900 0000 7304 0000 0006 050a 0163  ..Y...s........c
+00000d10: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000d20: 0500 0000 4300 0000 731c 0000 0064 017c  ....C...s....d.|
+00000d30: 006a 006a 019b 0064 0274 027c 006a 0383  .j.j...d.t.|.j..
+00000d40: 019b 0064 039d 0553 0029 044e fa01 3c7a  ...d...S.).N..<z
+00000d50: 0b20 456e 7469 7479 2869 6e20 7a09 2067  . Entity(in z. g
+00000d60: 726f 7570 7329 3e29 0472 1500 0000 da08  roups)>).r......
+00000d70: 5f5f 6e61 6d65 5f5f da03 6c65 6eda 0a5f  __name__..len.._
+00000d80: 5370 7269 7465 5f5f 6772 1f00 0000 7208  Sprite__gr....r.
+00000d90: 0000 0072 0800 0000 720b 0000 00da 085f  ...r....r......_
+00000da0: 5f72 6570 725f 5f61 0000 0073 0200 0000  _repr__a...s....
+00000db0: 1c02 7a0f 456e 7469 7479 2e5f 5f72 6570  ..z.Entity.__rep
+00000dc0: 725f 5f29 0172 0800 0000 2901 4629 1772  r__).r....).F).r
+00000dd0: 2200 0000 da0a 5f5f 6d6f 6475 6c65 5f5f  ".....__module__
+00000de0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
+00000df0: 5f5f 646f 635f 5f72 0d00 0000 7202 0000  __doc__r....r...
+00000e00: 00da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  ...__annotations
+00000e10: 5f5f da04 6c69 7374 7205 0000 0072 0f00  __..listr....r..
+00000e20: 0000 da03 696e 7472 0300 0000 7212 0000  ....intr....r...
+00000e30: 0072 1800 0000 7204 0000 00da 0462 6f6f  .r....r......boo
+00000e40: 6c72 1d00 0000 721e 0000 00da 0870 726f  lr....r......pro
+00000e50: 7065 7274 7972 1700 0000 da06 7365 7474  pertyr......sett
+00000e60: 6572 7225 0000 00da 0d5f 5f63 6c61 7373  err%.....__class
+00000e70: 6365 6c6c 5f5f 7208 0000 0072 0800 0000  cell__r....r....
+00000e80: 7214 0000 0072 0b00 0000 7206 0000 0009  r....r....r.....
+00000e90: 0000 0073 1c00 0000 0a00 0401 101d 0c01  ...s............
+00000ea0: 0c01 1802 0804 1412 0c0d 0206 0a01 0404  ................
+00000eb0: 0a01 1007 7206 0000 0029 0ada 0674 7970  ....r....)...typ
+00000ec0: 696e 6772 0200 0000 7203 0000 00da 0670  ingr....r......p
+00000ed0: 7967 616d 6572 0400 0000 da17 726f 6269  ygamer......robi
+00000ee0: 6e67 616d 652e 6f62 6a65 6374 732e 6772  ngame.objects.gr
+00000ef0: 6f75 7072 0500 0000 da06 7370 7269 7465  oupr......sprite
+00000f00: da06 5370 7269 7465 7206 0000 0072 0800  ..Spriter....r..
+00000f10: 0000 7208 0000 0072 0800 0000 720b 0000  ..r....r....r...
+00000f20: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000f30: 0a00 0000 1000 0802 0c01 0c02 1803       ..............
```

### Comparing `robingame-0.1.0/robingame/objects/__pycache__/game.cpython-310.pyc` & `robingame-1.0.1/robingame/objects/__pycache__/game.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jul  5 13:47:52 2023 UTC, .py size: 2526 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,187 +1,208 @@
-00000000: 6f0d 0d0a 0000 0000 8874 a564 de09 0000  o........t.d....
+00000000: 6f0d 0d0a 0000 0000 7bcd b364 740c 0000  o.......{..dt...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
+00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
-00000070: 0100 6400 6406 6c0b 6d0c 5a0c 0100 4700  ..d.d.l.m.Z...G.
-00000080: 6407 6408 8400 6408 6509 8303 5a0d 6401  d.d...d.e...Z.d.
-00000090: 5300 2909 e900 0000 004e 2901 da05 436f  S.)......N)...Co
-000000a0: 6c6f 7229 01da 0753 7572 6661 6365 2901  lor)...Surface).
-000000b0: da0a 4576 656e 7451 7565 7565 2902 da06  ..EventQueue)...
-000000c0: 456e 7469 7479 da05 4772 6f75 7029 01da  Entity..Group)..
-000000d0: 0a46 7073 5472 6163 6b65 7263 0000 0000  .FpsTrackerc....
-000000e0: 0000 0000 0000 0000 0000 0000 0500 0000  ................
-000000f0: 0000 0000 73a2 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
-00000100: 0255 0064 015a 0364 025a 0465 0565 0664  .U.d.Z.d.Z.e.e.d
-00000110: 033c 0064 045a 0765 0565 0664 053c 0064  .<.d.Z.e.e.d.<.d
-00000120: 045a 0865 0565 0664 063c 0064 005a 0965  .Z.e.e.d.<.d.Z.e
-00000130: 0a65 0664 073c 0065 0b64 0883 015a 0c64  .e.d.<.e.d...Z.d
-00000140: 095a 0d65 0e65 0664 0a3c 0065 0e65 0664  .Z.e.e.d.<.e.e.d
-00000150: 0b3c 0087 0066 0164 0c64 0d84 085a 0f64  .<...f.d.d...Z.d
-00000160: 0e64 0f84 005a 1064 1064 1184 005a 1164  .d...Z.d.d...Z.d
-00000170: 1264 1384 005a 1264 1464 1584 005a 1364  .d...Z.d.d...Z.d
-00000180: 1964 1665 1464 0a65 0e66 0464 1764 1884  .d.e.d.e.f.d.d..
-00000190: 055a 1587 0004 005a 1653 0029 1ada 0447  .Z.....Z.S.)...G
-000001a0: 616d 657a 820a 2020 2020 5370 6563 6961  amez..    Specia
-000001b0: 6c20 6361 7365 206f 6620 456e 7469 7479  l case of Entity
-000001c0: 3b20 6974 2069 7320 6174 2074 6865 2076  ; it is at the v
-000001d0: 6572 7920 746f 7020 6f66 2074 6865 206f  ery top of the o
-000001e0: 626a 6563 7420 7472 6565 2e0a 2020 2020  bject tree..    
-000001f0: 4861 6e64 6c65 7320 7365 7474 696e 6720  Handles setting 
-00000200: 7570 2061 6e64 2072 756e 6e69 6e67 2074  up and running t
-00000210: 6865 206d 6169 6e20 6761 6d65 206c 6f6f  he main game loo
-00000220: 702e 0a20 2020 20e9 3c00 0000 da03 6670  p..    .<.....fp
-00000230: 7369 f401 0000 da0c 7769 6e64 6f77 5f77  si......window_w
-00000240: 6964 7468 da0d 7769 6e64 6f77 5f68 6569  idth..window_hei
-00000250: 6768 74da 0e77 696e 646f 775f 6361 7074  ght..window_capt
-00000260: 696f 6eda 0562 6c61 636b 46da 0564 6562  ion..blackF..deb
-00000270: 7567 da07 7275 6e6e 696e 6763 0100 0000  ug..runningc....
-00000280: 0000 0000 0000 0000 0100 0000 0400 0000  ................
-00000290: 0300 0000 734e 0000 0074 0083 00a0 01a1  ....sN...t......
-000002a0: 0001 0074 02a0 03a1 0001 0074 0483 007c  ...t.......t...|
-000002b0: 005f 0574 026a 06a0 077c 006a 087c 006a  ._.t.j...|.j.|.j
-000002c0: 0966 02a1 017c 005f 0a74 026a 06a0 0b7c  .f...|._.t.j...|
-000002d0: 006a 0ca1 0101 0074 026a 0da0 0ea1 007c  .j.....t.j.....|
-000002e0: 005f 0f64 0053 00a9 014e 2910 da05 7375  ._.d.S...N)...su
-000002f0: 7065 72da 085f 5f69 6e69 745f 5fda 0670  per..__init__..p
-00000300: 7967 616d 65da 0469 6e69 7472 0700 0000  ygame..initr....
-00000310: da0b 6670 735f 7472 6163 6b65 72da 0764  ..fps_tracker..d
-00000320: 6973 706c 6179 da08 7365 745f 6d6f 6465  isplay..set_mode
-00000330: 720b 0000 0072 0c00 0000 da06 7769 6e64  r....r......wind
-00000340: 6f77 da0b 7365 745f 6361 7074 696f 6e72  ow..set_captionr
-00000350: 0d00 0000 da04 7469 6d65 da05 436c 6f63  ......time..Cloc
-00000360: 6bda 0563 6c6f 636b a901 da04 7365 6c66  k..clock....self
-00000370: a901 da09 5f5f 636c 6173 735f 5fa9 00fa  ....__class__...
-00000380: 342f 686f 6d65 2f72 6f62 696e 2f63 6f64  4/home/robin/cod
-00000390: 652f 726f 6269 6e67 616d 652f 726f 6269  e/robingame/robi
-000003a0: 6e67 616d 652f 6f62 6a65 6374 732f 6761  ngame/objects/ga
-000003b0: 6d65 2e70 7972 1300 0000 1a00 0000 730c  me.pyr........s.
-000003c0: 0000 000a 0108 0108 0116 010e 0110 017a  ...............z
-000003d0: 0d47 616d 652e 5f5f 696e 6974 5f5f 6301  .Game.__init__c.
-000003e0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-000003f0: 0000 0043 0000 0073 4000 0000 6401 7c00  ...C...s@...d.|.
-00000400: 5f00 7c00 6a00 7216 7c00 a001 a100 0100  _.|.j.r.|.......
-00000410: 7c00 6a02 7c00 6a03 7c00 6a04 6402 8d02  |.j.|.j.|.j.d...
-00000420: 0100 7c00 6a00 7306 7405 a006 a100 0100  ..|.j.s.t.......
-00000430: 7407 a008 a100 0100 6403 5300 2904 7aae  t.......d.S.).z.
-00000440: 0a20 2020 2020 2020 2054 6869 7320 6973  .        This is
-00000450: 2074 6865 206f 7574 6572 6d6f 7374 2067   the outermost g
-00000460: 616d 6520 6675 6e63 7469 6f6e 2077 6869  ame function whi
-00000470: 6368 2072 756e 7320 6f6e 6365 2e20 4974  ch runs once. It
-00000480: 2063 6f6e 7461 696e 7320 7468 6520 6f75   contains the ou
-00000490: 7465 726d 6f73 7420 6761 6d65 206c 6f6f  termost game loo
-000004a0: 702e 0a20 2020 2020 2020 2048 6572 6527  p..        Here'
-000004b0: 7320 7768 6572 6520 796f 7520 7368 6f75  s where you shou
-000004c0: 6c64 2070 7574 2079 6f75 7220 6d61 696e  ld put your main
-000004d0: 2065 7665 6e74 2073 7461 7465 206d 6163   event state mac
-000004e0: 6869 6e65 2e0a 2020 2020 2020 2020 5429  hine..        T)
-000004f0: 0172 0f00 0000 4e29 0972 1000 0000 da07  .r....N).r......
-00000500: 5f75 7064 6174 65da 055f 6472 6177 7219  _update.._drawr.
-00000510: 0000 0072 0f00 0000 7214 0000 00da 0471  ...r....r......q
-00000520: 7569 74da 0373 7973 da04 6578 6974 721e  uit..sys..exitr.
-00000530: 0000 0072 2200 0000 7222 0000 0072 2300  ...r"...r"...r#.
-00000540: 0000 da04 6d61 696e 2200 0000 730e 0000  ....main"...s...
-00000550: 0006 0506 0108 0112 0106 fe08 030c 017a  ...............z
-00000560: 0947 616d 652e 6d61 696e 6301 0000 0000  .Game.mainc.....
-00000570: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
-00000580: 0000 0073 5600 0000 7400 a001 a100 0100  ...sV...t.......
-00000590: 7400 6a02 4400 5d21 7d01 7c01 6a03 7404  t.j.D.]!}.|.j.t.
-000005a0: 6a05 6b02 7217 7404 a006 a100 0100 7407  j.k.r.t.......t.
-000005b0: a008 a100 0100 7c01 6a03 7404 6a09 6b02  ......|.j.t.j.k.
-000005c0: 7228 7c01 6a0a 7404 6a0b 6b02 7228 7c00  r(|.j.t.j.k.r(|.
-000005d0: 6a0c 0c00 7c00 5f0c 7107 6401 5300 2902  j...|._.q.d.S.).
-000005e0: 611b 0100 000a 2020 2020 2020 2020 4927  a.....        I'
-000005f0: 7665 2070 7574 2074 6869 7320 696e 2061  ve put this in a
-00000600: 2073 6570 6172 6174 6520 6d65 7468 6f64   separate method
-00000610: 2062 6563 6175 7365 2049 2064 6f6e 2774   because I don't
-00000620: 206c 696b 6520 7468 6520 6964 6561 206f   like the idea o
-00000630: 6620 7075 7474 696e 6720 7468 6520 696e  f putting the in
-00000640: 7075 7473 2069 6e0a 2020 2020 2020 2020  puts in.        
-00000650: 7468 6520 7361 6d65 206c 6973 7420 6173  the same list as
-00000660: 206f 7468 6572 2063 6869 6c64 2067 726f   other child gro
-00000670: 7570 732e 2054 6865 206f 7264 6572 206d  ups. The order m
-00000680: 6967 6874 2067 6574 2072 7569 6e65 642c  ight get ruined,
-00000690: 206f 7220 6120 7375 6263 6c61 7373 206d   or a subclass m
-000006a0: 6967 6874 0a20 2020 2020 2020 206f 7665  ight.        ove
-000006b0: 7277 7269 7465 2074 6865 206c 6973 742e  rwrite the list.
-000006c0: 2049 7427 7320 6372 7563 6961 6c20 7468   It's crucial th
-000006d0: 6174 2074 6865 2069 6e70 7574 7320 6172  at the inputs ar
-000006e0: 6520 7265 6164 2062 6566 6f72 6520 7570  e read before up
-000006f0: 6461 7469 6e67 2e0a 2020 2020 2020 2020  dating..        
-00000700: 4e29 0d72 0400 0000 da06 7570 6461 7465  N).r......update
-00000710: da06 6576 656e 7473 da04 7479 7065 7214  ..events..typer.
-00000720: 0000 00da 0451 5549 5472 2600 0000 7227  .....QUITr&...r'
-00000730: 0000 0072 2800 0000 da07 4b45 5944 4f57  ...r(.....KEYDOW
-00000740: 4eda 036b 6579 da04 4b5f 4631 720f 0000  N..key..K_F1r...
-00000750: 0029 0272 1f00 0000 da05 6576 656e 7472  .).r......eventr
-00000760: 2200 0000 7222 0000 0072 2300 0000 da0b  "...r"...r#.....
-00000770: 7265 6164 5f69 6e70 7574 732e 0000 0073  read_inputs....s
-00000780: 1200 0000 0806 0a01 0c01 0801 0801 1801  ................
-00000790: 0a01 0280 04fb 7a10 4761 6d65 2e72 6561  ......z.Game.rea
-000007a0: 645f 696e 7075 7473 6301 0000 0000 0000  d_inputsc.......
-000007b0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-000007c0: 0073 0400 0000 6400 5300 7211 0000 0072  .s....d.S.r....r
-000007d0: 2200 0000 721e 0000 0072 2200 0000 7222  "...r....r"...r"
-000007e0: 0000 0072 2300 0000 da10 7072 696e 745f  ...r#.....print_
-000007f0: 6465 6275 675f 696e 666f 3c00 0000 7302  debug_info<...s.
-00000800: 0000 0004 017a 1547 616d 652e 7072 696e  .....z.Game.prin
-00000810: 745f 6465 6275 675f 696e 666f 6301 0000  t_debug_infoc...
-00000820: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00000830: 0043 0000 0073 4400 0000 7c00 a000 a100  .C...sD...|.....
-00000840: 0100 7c00 6a01 720b 7c00 a002 a100 0100  ..|.j.r.|.......
-00000850: 7c00 a003 a100 0100 7c00 6a04 a003 a100  |.......|.j.....
-00000860: 0100 7c00 6a05 7220 7c00 6a06 a007 7c00  ..|.j.r |.j...|.
-00000870: 6a05 a101 0100 6401 5300 6401 5300 2902  j.....d.S.d.S.).
-00000880: 7a32 0a20 2020 2020 2020 2031 2e20 7265  z2.        1. re
-00000890: 6164 2069 6e70 7574 730a 2020 2020 2020  ad inputs.      
-000008a0: 2020 322e 2075 7064 6174 650a 2020 2020    2. update.    
-000008b0: 2020 2020 4e29 0872 3200 0000 720f 0000      N).r2...r...
-000008c0: 0072 3300 0000 722a 0000 0072 1600 0000  .r3...r*...r....
-000008d0: 720a 0000 0072 1d00 0000 da04 7469 636b  r....r......tick
-000008e0: 721e 0000 0072 2200 0000 7222 0000 0072  r....r"...r"...r
-000008f0: 2300 0000 7224 0000 003f 0000 0073 1000  #...r$...?...s..
-00000900: 0000 0805 0601 0801 0801 0a01 0601 1201  ................
-00000910: 04ff 7a0c 4761 6d65 2e5f 7570 6461 7465  ..z.Game._update
-00000920: da07 7375 7266 6163 6563 0300 0000 0000  ..surfacec......
-00000930: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-00000940: 0000 7334 0000 007c 01a0 007c 006a 01a1  ..s4...|...|.j..
-00000950: 0101 007c 00a0 027c 017c 02a1 0201 007c  ...|...|.|.....|
-00000960: 006a 03a0 027c 017c 02a1 0201 0074 046a  .j...|.|.....t.j
-00000970: 05a0 06a1 0001 0064 0053 0072 1100 0000  .......d.S.r....
-00000980: 2907 da04 6669 6c6c da0c 7363 7265 656e  )...fill..screen
-00000990: 5f63 6f6c 6f72 da04 6472 6177 7216 0000  _color..drawr...
-000009a0: 0072 1400 0000 7217 0000 0072 2a00 0000  .r....r....r*...
-000009b0: 2903 721f 0000 0072 3500 0000 720f 0000  ).r....r5...r...
-000009c0: 0072 2200 0000 7222 0000 0072 2300 0000  .r"...r"...r#...
-000009d0: 7225 0000 004c 0000 0073 0800 0000 0c01  r%...L...s......
-000009e0: 0c01 0e01 0e01 7a0a 4761 6d65 2e5f 6472  ......z.Game._dr
-000009f0: 6177 2901 4629 17da 085f 5f6e 616d 655f  aw).F)...__name_
-00000a00: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000a10: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
-00000a20: 6f63 5f5f 720a 0000 00da 0369 6e74 da0f  oc__r......int..
-00000a30: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5f72  __annotations__r
-00000a40: 0b00 0000 720c 0000 0072 0d00 0000 da03  ....r....r......
-00000a50: 7374 7272 0200 0000 7237 0000 0072 0f00  strr....r7...r..
-00000a60: 0000 da04 626f 6f6c 7213 0000 0072 2900  ....boolr....r).
-00000a70: 0000 7232 0000 0072 3300 0000 7224 0000  ..r2...r3...r$..
-00000a80: 0072 0300 0000 7225 0000 00da 0d5f 5f63  .r....r%.....__c
-00000a90: 6c61 7373 6365 6c6c 5f5f 7222 0000 0072  lasscell__r"...r
-00000aa0: 2200 0000 7220 0000 0072 2300 0000 7208  "...r ...r#...r.
-00000ab0: 0000 000c 0000 0073 1e00 0000 0a00 0401  .......s........
-00000ac0: 0c05 0c01 0c01 0c01 0801 0c01 0801 0c02  ................
-00000ad0: 0808 080c 080e 0803 1c0d 7208 0000 0029  ..........r....)
-00000ae0: 0e72 2700 0000 7214 0000 00da 0c70 7967  .r'...r......pyg
-00000af0: 616d 652e 636f 6c6f 7272 0200 0000 da0e  ame.colorr......
-00000b00: 7079 6761 6d65 2e73 7572 6661 6365 7203  pygame.surfacer.
-00000b10: 0000 00da 0f72 6f62 696e 6761 6d65 2e69  .....robingame.i
-00000b20: 6e70 7574 7204 0000 00da 1872 6f62 696e  nputr......robin
-00000b30: 6761 6d65 2e6f 626a 6563 7473 2e65 6e74  game.objects.ent
-00000b40: 6974 7972 0500 0000 7206 0000 00da 1972  ityr....r......r
-00000b50: 6f62 696e 6761 6d65 2e6f 626a 6563 7473  obingame.objects
-00000b60: 2e68 656c 7065 7273 7207 0000 0072 0800  .helpersr....r..
-00000b70: 0000 7222 0000 0072 2200 0000 7222 0000  ..r"...r"...r"..
-00000b80: 0072 2300 0000 da08 3c6d 6f64 756c 653e  .r#.....<module>
-00000b90: 0100 0000 7310 0000 0008 0008 020c 010c  ....s...........
-00000ba0: 010c 0210 010c 0114 03                   .........
+00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
+00000070: 6406 6c0a 6d0b 5a0b 0100 4700 6407 6408  d.l.m.Z...G.d.d.
+00000080: 8400 6408 6509 8303 5a0c 6401 5300 2909  ..d.e...Z.d.S.).
+00000090: e900 0000 004e 2901 da05 436f 6c6f 7229  .....N)...Color)
+000000a0: 01da 0753 7572 6661 6365 2901 da0a 4576  ...Surface)...Ev
+000000b0: 656e 7451 7565 7565 2901 da06 456e 7469  entQueue)...Enti
+000000c0: 7479 2901 da0a 4670 7354 7261 636b 6572  ty)...FpsTracker
+000000d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000000e0: 0005 0000 0000 0000 0073 a200 0000 6500  .........s....e.
+000000f0: 5a01 6400 5a02 5500 6401 5a03 6402 5a04  Z.d.Z.U.d.Z.d.Z.
+00000100: 6505 6506 6403 3c00 6404 5a07 6505 6506  e.e.d.<.d.Z.e.e.
+00000110: 6405 3c00 6404 5a08 6505 6506 6406 3c00  d.<.d.Z.e.e.d.<.
+00000120: 6400 5a09 650a 6506 6407 3c00 650b 6408  d.Z.e.e.d.<.e.d.
+00000130: 8301 5a0c 6409 5a0d 650e 6506 640a 3c00  ..Z.d.Z.e.e.d.<.
+00000140: 650e 6506 640b 3c00 8700 6601 640c 640d  e.e.d.<...f.d.d.
+00000150: 8408 5a0f 640e 640f 8400 5a10 6410 6411  ..Z.d.d...Z.d.d.
+00000160: 8400 5a11 6412 6413 8400 5a12 6414 6415  ..Z.d.d...Z.d.d.
+00000170: 8400 5a13 6419 6416 6514 640a 650e 6604  ..Z.d.d.e.d.e.f.
+00000180: 6417 6418 8405 5a15 8700 0400 5a16 5300  d.d...Z.....Z.S.
+00000190: 291a da04 4761 6d65 61d2 0100 000a 2020  )...Gamea.....  
+000001a0: 2020 5370 6563 6961 6c20 6361 7365 206f    Special case o
+000001b0: 6620 456e 7469 7479 3b20 6974 2069 7320  f Entity; it is 
+000001c0: 6174 2074 6865 2076 6572 7920 746f 7020  at the very top 
+000001d0: 6f66 2074 6865 206f 626a 6563 7420 7472  of the object tr
+000001e0: 6565 2e0a 0a20 2020 2048 616e 646c 6573  ee...    Handles
+000001f0: 206d 7563 6820 6f66 2074 6865 2070 7967   much of the pyg
+00000200: 616d 6520 626f 696c 6572 706c 6174 6520  ame boilerplate 
+00000210: 7365 7475 702c 2069 6e63 6c75 6469 6e67  setup, including
+00000220: 3a0a 0a20 2020 202d 2069 6e69 7469 616c  :..    - initial
+00000230: 6973 696e 6720 7468 6520 6469 7370 6c61  ising the displa
+00000240: 790a 2020 2020 2d20 7365 7474 696e 6720  y.    - setting 
+00000250: 7570 2061 6e64 2072 756e 6e69 6e67 2074  up and running t
+00000260: 6865 206d 6169 6e20 6761 6d65 206c 6f6f  he main game loo
+00000270: 702e 0a20 2020 202d 2064 6f69 6e67 2060  p..    - doing `
+00000280: 636c 6f63 6b2e 7469 636b 2829 6020 6576  clock.tick()` ev
+00000290: 6572 7920 6974 6572 6174 696f 6e20 616e  ery iteration an
+000002a0: 6420 656e 666f 7263 696e 6720 7468 6520  d enforcing the 
+000002b0: 6672 616d 6572 6174 650a 2020 2020 2d20  framerate.    - 
+000002c0: 6669 6c6c 696e 6720 7468 6520 7363 7265  filling the scre
+000002d0: 656e 2077 6974 6820 6073 656c 662e 7363  en with `self.sc
+000002e0: 7265 656e 5f63 6f6c 6f72 6020 6576 6572  reen_color` ever
+000002f0: 7920 6974 6572 6174 696f 6e0a 2020 2020  y iteration.    
+00000300: 2d20 7570 6461 7469 6e67 2074 6865 2045  - updating the E
+00000310: 7665 6e74 5175 6575 6520 7769 7468 206e  ventQueue with n
+00000320: 6577 2065 7665 6e74 730a 2020 2020 2d20  ew events.    - 
+00000330: 6d61 696e 7461 696e 696e 6720 7468 6520  maintaining the 
+00000340: 4650 5320 7472 6163 6b65 7220 2861 6e64  FPS tracker (and
+00000350: 2064 7261 7769 6e67 2069 7420 696e 2064   drawing it in d
+00000360: 6562 7567 206d 6f64 6529 0a20 2020 20e9  ebug mode).    .
+00000370: 3c00 0000 da03 6670 7369 f401 0000 da0c  <.....fpsi......
+00000380: 7769 6e64 6f77 5f77 6964 7468 da0d 7769  window_width..wi
+00000390: 6e64 6f77 5f68 6569 6768 74da 0e77 696e  ndow_height..win
+000003a0: 646f 775f 6361 7074 696f 6eda 0562 6c61  dow_caption..bla
+000003b0: 636b 46da 0564 6562 7567 da07 7275 6e6e  ckF..debug..runn
+000003c0: 696e 6763 0100 0000 0000 0000 0000 0000  ingc............
+000003d0: 0100 0000 0400 0000 0300 0000 734e 0000  ............sN..
+000003e0: 0074 0083 00a0 01a1 0001 0074 02a0 03a1  .t.........t....
+000003f0: 0001 0074 0483 007c 005f 0574 026a 06a0  ...t...|._.t.j..
+00000400: 077c 006a 087c 006a 0966 02a1 017c 005f  .|.j.|.j.f...|._
+00000410: 0a74 026a 06a0 0b7c 006a 0ca1 0101 0074  .t.j...|.j.....t
+00000420: 026a 0da0 0ea1 007c 005f 0f64 0153 0029  .j.....|._.d.S.)
+00000430: 027a 6d0a 2020 2020 2020 2020 4861 6e64  .zm.        Hand
+00000440: 6c65 7320 6120 6c6f 7420 6f66 2074 6865  les a lot of the
+00000450: 2062 6f69 6c65 7270 6c61 7465 2070 7967   boilerplate pyg
+00000460: 616d 6520 7365 7475 702e 0a20 2020 2020  ame setup..     
+00000470: 2020 2043 7265 6174 6573 2074 6865 2064     Creates the d
+00000480: 6973 706c 6179 2028 6073 656c 662e 7769  isplay (`self.wi
+00000490: 6e64 6f77 6029 2e0a 2020 2020 2020 2020  ndow`)..        
+000004a0: 4e29 10da 0573 7570 6572 da08 5f5f 696e  N)...super..__in
+000004b0: 6974 5f5f da06 7079 6761 6d65 da04 696e  it__..pygame..in
+000004c0: 6974 7206 0000 00da 0b66 7073 5f74 7261  itr......fps_tra
+000004d0: 636b 6572 da07 6469 7370 6c61 79da 0873  cker..display..s
+000004e0: 6574 5f6d 6f64 6572 0a00 0000 720b 0000  et_moder....r...
+000004f0: 00da 0677 696e 646f 77da 0b73 6574 5f63  ...window..set_c
+00000500: 6170 7469 6f6e 720c 0000 00da 0474 696d  aptionr......tim
+00000510: 65da 0543 6c6f 636b da05 636c 6f63 6ba9  e..Clock..clock.
+00000520: 01da 0473 656c 66a9 01da 095f 5f63 6c61  ...self....__cla
+00000530: 7373 5f5f a900 fa34 2f68 6f6d 652f 726f  ss__...4/home/ro
+00000540: 6269 6e2f 636f 6465 2f72 6f62 696e 6761  bin/code/robinga
+00000550: 6d65 2f72 6f62 696e 6761 6d65 2f6f 626a  me/robingame/obj
+00000560: 6563 7473 2f67 616d 652e 7079 7211 0000  ects/game.pyr...
+00000570: 0022 0000 0073 0c00 0000 0a05 0801 0801  ."...s..........
+00000580: 1601 0e01 1001 7a0d 4761 6d65 2e5f 5f69  ......z.Game.__i
+00000590: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+000005a0: 0000 0100 0000 0400 0000 4300 0000 7340  ..........C...s@
+000005b0: 0000 0064 017c 005f 007c 006a 0072 167c  ...d.|._.|.j.r.|
+000005c0: 00a0 01a1 0001 007c 006a 027c 006a 037c  .......|.j.|.j.|
+000005d0: 006a 0464 028d 0201 007c 006a 0073 0674  .j.d.....|.j.s.t
+000005e0: 05a0 06a1 0001 0074 07a0 08a1 0001 0064  .......t.......d
+000005f0: 0353 0029 047a 850a 2020 2020 2020 2020  .S.).z..        
+00000600: 436f 6e74 6169 6e73 2074 6865 206d 6169  Contains the mai
+00000610: 6e20 6761 6d65 206c 6f6f 702e 0a20 2020  n game loop..   
+00000620: 2020 2020 2043 616c 6c73 2060 7365 6c66       Calls `self
+00000630: 2e5f 7570 6461 7465 2829 6020 616e 6420  ._update()` and 
+00000640: 6073 656c 662e 5f64 7261 7728 2960 206f  `self._draw()` o
+00000650: 6e20 6576 6572 7920 6974 6572 6174 696f  n every iteratio
+00000660: 6e20 6f66 2074 6865 2067 616d 6520 6c6f  n of the game lo
+00000670: 6f70 2e0a 2020 2020 2020 2020 5429 0172  op..        T).r
+00000680: 0e00 0000 4e29 0972 0f00 0000 da07 5f75  ....N).r......_u
+00000690: 7064 6174 65da 055f 6472 6177 7217 0000  pdate.._drawr...
+000006a0: 0072 0e00 0000 7212 0000 00da 0471 7569  .r....r......qui
+000006b0: 74da 0373 7973 da04 6578 6974 721c 0000  t..sys..exitr...
+000006c0: 0072 2000 0000 7220 0000 0072 2100 0000  .r ...r ...r!...
+000006d0: da04 6d61 696e 2e00 0000 730e 0000 0006  ..main....s.....
+000006e0: 0506 0108 0112 0106 fe08 030c 017a 0947  .............z.G
+000006f0: 616d 652e 6d61 696e 6301 0000 0000 0000  ame.mainc.......
+00000700: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00000710: 0073 5600 0000 7400 a001 a100 0100 7400  .sV...t.......t.
+00000720: 6a02 4400 5d21 7d01 7c01 6a03 7404 6a05  j.D.]!}.|.j.t.j.
+00000730: 6b02 7217 7404 a006 a100 0100 7407 a008  k.r.t.......t...
+00000740: a100 0100 7c01 6a03 7404 6a09 6b02 7228  ....|.j.t.j.k.r(
+00000750: 7c01 6a0a 7404 6a0b 6b02 7228 7c00 6a0c  |.j.t.j.k.r(|.j.
+00000760: 0c00 7c00 5f0c 7107 6401 5300 2902 7aa9  ..|._.q.d.S.).z.
+00000770: 0a20 2020 2020 2020 2043 616c 6c65 6420  .        Called 
+00000780: 6279 2060 7365 6c66 2e5f 7570 6461 7465  by `self._update
+00000790: 2829 602c 2062 6566 6f72 6520 6073 7570  ()`, before `sup
+000007a0: 6572 2829 2e75 7064 6174 6528 2960 2075  er().update()` u
+000007b0: 7064 6174 6573 2074 6865 2063 6869 6c64  pdates the child
+000007c0: 7265 6e2e 0a0a 2020 2020 2020 2020 416e  ren...        An
+000007d0: 7920 636f 6465 2074 6861 7420 706f 6c6c  y code that poll
+000007e0: 7320 6578 7465 726e 616c 206a 6f79 7374  s external joyst
+000007f0: 6963 6b73 2f63 6f6e 7472 6f6c 6c65 7273  icks/controllers
+00000800: 2073 686f 756c 6420 676f 2068 6572 652e   should go here.
+00000810: 0a20 2020 2020 2020 204e 290d 7204 0000  .        N).r...
+00000820: 00da 0675 7064 6174 65da 0665 7665 6e74  ...update..event
+00000830: 73da 0474 7970 6572 1200 0000 da04 5155  s..typer......QU
+00000840: 4954 7224 0000 0072 2500 0000 7226 0000  ITr$...r%...r&..
+00000850: 00da 074b 4559 444f 574e da03 6b65 79da  ...KEYDOWN..key.
+00000860: 044b 5f46 3172 0e00 0000 2902 721d 0000  .K_F1r....).r...
+00000870: 00da 0565 7665 6e74 7220 0000 0072 2000  ...eventr ...r .
+00000880: 0000 7221 0000 00da 0b72 6561 645f 696e  ..r!.....read_in
+00000890: 7075 7473 3a00 0000 7312 0000 0008 0a0a  puts:...s.......
+000008a0: 010c 0108 0108 0118 010a 0102 8004 fb7a  ...............z
+000008b0: 1047 616d 652e 7265 6164 5f69 6e70 7574  .Game.read_input
+000008c0: 7363 0100 0000 0000 0000 0000 0000 0100  sc..............
+000008d0: 0000 0100 0000 4300 0000 7304 0000 0064  ......C...s....d
+000008e0: 0153 0029 027a 440a 2020 2020 2020 2020  .S.).zD.        
+000008f0: 4f76 6572 7269 6465 2074 6869 7320 6966  Override this if
+00000900: 2079 6f75 2077 616e 7420 746f 2070 7269   you want to pri
+00000910: 6e74 2061 6e79 2064 6562 7567 2069 6e66  nt any debug inf
+00000920: 6f2e 0a20 2020 2020 2020 204e 7220 0000  o..        Nr ..
+00000930: 0072 1c00 0000 7220 0000 0072 2000 0000  .r....r ...r ...
+00000940: 7221 0000 00da 1070 7269 6e74 5f64 6562  r!.....print_deb
+00000950: 7567 5f69 6e66 6f4c 0000 0073 0200 0000  ug_infoL...s....
+00000960: 0404 7a15 4761 6d65 2e70 7269 6e74 5f64  ..z.Game.print_d
+00000970: 6562 7567 5f69 6e66 6f63 0100 0000 0000  ebug_infoc......
+00000980: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00000990: 0000 7344 0000 007c 00a0 00a1 0001 007c  ..sD...|.......|
+000009a0: 006a 0172 0b7c 00a0 02a1 0001 007c 00a0  .j.r.|.......|..
+000009b0: 03a1 0001 007c 006a 04a0 03a1 0001 007c  .....|.j.......|
+000009c0: 006a 0572 207c 006a 06a0 077c 006a 05a1  .j.r |.j...|.j..
+000009d0: 0101 0064 0153 0064 0153 0029 027a 320a  ...d.S.d.S.).z2.
+000009e0: 2020 2020 2020 2020 312e 2072 6561 6420          1. read 
+000009f0: 696e 7075 7473 0a20 2020 2020 2020 2032  inputs.        2
+00000a00: 2e20 7570 6461 7465 0a20 2020 2020 2020  . update.       
+00000a10: 204e 2908 7230 0000 0072 0e00 0000 7231   N).r0...r....r1
+00000a20: 0000 0072 2800 0000 7214 0000 0072 0900  ...r(...r....r..
+00000a30: 0000 721b 0000 00da 0474 6963 6b72 1c00  ..r......tickr..
+00000a40: 0000 7220 0000 0072 2000 0000 7221 0000  ..r ...r ...r!..
+00000a50: 0072 2200 0000 5200 0000 7310 0000 0008  .r"...R...s.....
+00000a60: 0506 0108 0108 010a 0106 0112 0104 ff7a  ...............z
+00000a70: 0c47 616d 652e 5f75 7064 6174 65da 0773  .Game._update..s
+00000a80: 7572 6661 6365 6303 0000 0000 0000 0000  urfacec.........
+00000a90: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
+00000aa0: 3400 0000 7c01 a000 7c00 6a01 a101 0100  4...|...|.j.....
+00000ab0: 7c00 a002 7c01 7c02 a102 0100 7c00 6a03  |...|.|.....|.j.
+00000ac0: a002 7c01 7c02 a102 0100 7404 6a05 a006  ..|.|.....t.j...
+00000ad0: a100 0100 6400 5300 2901 4e29 07da 0466  ....d.S.).N)...f
+00000ae0: 696c 6cda 0c73 6372 6565 6e5f 636f 6c6f  ill..screen_colo
+00000af0: 72da 0464 7261 7772 1400 0000 7212 0000  r..drawr....r...
+00000b00: 0072 1500 0000 7228 0000 0029 0372 1d00  .r....r(...).r..
+00000b10: 0000 7233 0000 0072 0e00 0000 7220 0000  ..r3...r....r ..
+00000b20: 0072 2000 0000 7221 0000 0072 2300 0000  .r ...r!...r#...
+00000b30: 5f00 0000 7308 0000 000c 010c 010e 010e  _...s...........
+00000b40: 017a 0a47 616d 652e 5f64 7261 7729 0146  .z.Game._draw).F
+00000b50: 2917 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000b60: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000b70: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
+00000b80: 0900 0000 da03 696e 74da 0f5f 5f61 6e6e  ......int..__ann
+00000b90: 6f74 6174 696f 6e73 5f5f 720a 0000 0072  otations__r....r
+00000ba0: 0b00 0000 720c 0000 00da 0373 7472 7202  ....r......strr.
+00000bb0: 0000 0072 3500 0000 720e 0000 00da 0462  ...r5...r......b
+00000bc0: 6f6f 6c72 1100 0000 7227 0000 0072 3000  oolr....r'...r0.
+00000bd0: 0000 7231 0000 0072 2200 0000 7203 0000  ..r1...r"...r...
+00000be0: 0072 2300 0000 da0d 5f5f 636c 6173 7363  .r#.....__classc
+00000bf0: 656c 6c5f 5f72 2000 0000 7220 0000 0072  ell__r ...r ...r
+00000c00: 1e00 0000 7221 0000 0072 0700 0000 0c00  ....r!...r......
+00000c10: 0000 731e 0000 000a 0004 010c 0d0c 010c  ..s.............
+00000c20: 010c 0108 010c 0108 010c 0208 0c08 0c08  ................
+00000c30: 1208 061c 0d72 0700 0000 290d 7225 0000  .....r....).r%..
+00000c40: 0072 1200 0000 da0c 7079 6761 6d65 2e63  .r......pygame.c
+00000c50: 6f6c 6f72 7202 0000 00da 0e70 7967 616d  olorr......pygam
+00000c60: 652e 7375 7266 6163 6572 0300 0000 da0f  e.surfacer......
+00000c70: 726f 6269 6e67 616d 652e 696e 7075 7472  robingame.inputr
+00000c80: 0400 0000 da18 726f 6269 6e67 616d 652e  ......robingame.
+00000c90: 6f62 6a65 6374 732e 656e 7469 7479 7205  objects.entityr.
+00000ca0: 0000 00da 1972 6f62 696e 6761 6d65 2e6f  .....robingame.o
+00000cb0: 626a 6563 7473 2e68 656c 7065 7273 7206  bjects.helpersr.
+00000cc0: 0000 0072 0700 0000 7220 0000 0072 2000  ...r....r ...r .
+00000cd0: 0000 7220 0000 0072 2100 0000 da08 3c6d  ..r ...r!.....<m
+00000ce0: 6f64 756c 653e 0100 0000 7310 0000 0008  odule>....s.....
+00000cf0: 0008 020c 010c 010c 020c 010c 0114 03    ...............
```

### Comparing `robingame-0.1.0/robingame/objects/__pycache__/group.cpython-310.pyc` & `robingame-1.0.1/robingame/objects/__pycache__/group.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jul  5 13:47:52 2023 UTC, .py size: 1098 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8874 a564 4a04 0000  o........t.dJ...
+00000000: 6f0d 0d0a 0000 0000 b3c8 b364 1405 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6502 7212 6400 6403 6c03 6d04 5a04  ..e.r.d.d.l.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 6500 6a05  ..G.d.d...d.e.j.
 00000060: 6a06 8303 5a06 6401 5300 2906 e900 0000  j...Z.d.S.).....
 00000070: 004e 2901 da0d 5459 5045 5f43 4845 434b  .N)...TYPE_CHECK
@@ -10,96 +10,107 @@
 00000090: 0000 0000 0000 0000 0000 0000 0000 0500  ................
 000000a0: 0000 0000 0000 734c 0000 0065 005a 0164  ......sL...e.Z.d
 000000b0: 005a 0264 015a 0364 1187 0066 0164 0664  .Z.d.Z.d...f.d.d
 000000c0: 0784 0c5a 0487 0066 0164 0864 0984 085a  ...Z...f.d.d...Z
 000000d0: 0564 1264 0b65 066a 0764 0c65 0866 0464  .d.d.e.j.d.e.f.d
 000000e0: 0d64 0e84 055a 0964 0f64 1084 005a 0a87  .d...Z.d.d...Z..
 000000f0: 0004 005a 0b53 0029 13da 0547 726f 7570  ...Z.S.)...Group
-00000100: 7a26 436f 6e74 6169 6e65 7220 666f 7220  z&Container for 
-00000110: 6d75 6c74 6970 6c65 2045 6e74 6974 7920  multiple Entity 
-00000120: 6f62 6a65 6374 732e da08 656e 7469 7469  objects...entiti
-00000130: 6573 7203 0000 00da 0672 6574 7572 6e4e  esr......returnN
-00000140: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000150: 0002 0000 0007 0000 0073 1000 0000 7400  .........s....t.
-00000160: 8300 6a01 7c01 8e00 0100 6401 5300 2902  ..j.|.....d.S.).
-00000170: 7a4c 4f6e 6c79 206f 7665 7272 6964 696e  zLOnly overridin
-00000180: 6720 7468 6973 2062 6563 6175 7365 2070  g this because p
-00000190: 7967 616d 6527 7320 7479 7069 6e67 2077  ygame's typing w
-000001a0: 6173 206d 616b 696e 6720 7468 6520 6c69  as making the li
-000001b0: 6e74 6572 2063 6f6d 706c 6169 6e2e 4e29  nter complain.N)
-000001c0: 02da 0573 7570 6572 da03 6164 6429 02da  ...super..add)..
-000001d0: 0473 656c 6672 0500 0000 a901 da09 5f5f  .selfr........__
-000001e0: 636c 6173 735f 5fa9 00fa 352f 686f 6d65  class__...5/home
-000001f0: 2f72 6f62 696e 2f63 6f64 652f 726f 6269  /robin/code/robi
-00000200: 6e67 616d 652f 726f 6269 6e67 616d 652f  ngame/robingame/
-00000210: 6f62 6a65 6374 732f 6772 6f75 702e 7079  objects/group.py
-00000220: 7208 0000 000b 0000 0073 0200 0000 1002  r........s......
-00000230: 7a09 4772 6f75 702e 6164 6463 0100 0000  z.Group.addc....
-00000240: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00000250: 0700 0000 7310 0000 0074 0083 006a 017c  ....s....t...j.|
-00000260: 018e 0001 0064 0053 0029 014e 2902 7207  .....d.S.).N).r.
-00000270: 0000 00da 0675 7064 6174 6529 0272 0900  .....update).r..
-00000280: 0000 da04 6172 6773 720a 0000 0072 0c00  ....argsr....r..
-00000290: 0000 720d 0000 0072 0e00 0000 0f00 0000  ..r....r........
-000002a0: 7302 0000 0010 017a 0c47 726f 7570 2e75  s......z.Group.u
-000002b0: 7064 6174 6546 da07 7375 7266 6163 65da  pdateF..surface.
-000002c0: 0564 6562 7567 6303 0000 0000 0000 0000  .debugc.........
-000002d0: 0000 0005 0000 0005 0000 0043 0000 0073  ...........C...s
-000002e0: 2800 0000 7c00 a000 a100 7d03 7c03 4400  (...|.....}.|.D.
-000002f0: 5d08 7d04 7c04 a001 7c01 7c02 a102 0100  ].}.|...|.|.....
-00000300: 7106 6700 7c00 5f02 6401 5300 2902 7adf  q.g.|._.d.S.).z.
-00000310: 0a20 2020 2020 2020 2044 7261 7773 2061  .        Draws a
-00000320: 6c6c 206f 6620 7468 6520 6d65 6d62 6572  ll of the member
-00000330: 2073 7072 6974 6573 206f 6e74 6f20 7468   sprites onto th
-00000340: 6520 6769 7665 6e20 7375 7266 6163 652e  e given surface.
-00000350: 0a20 2020 2020 2020 2044 6966 6665 7265  .        Differe
-00000360: 6e74 2066 726f 6d20 7079 6761 6d65 2773  nt from pygame's
-00000370: 2047 726f 7570 2e64 7261 7720 696e 2074   Group.draw in t
-00000380: 6861 7420 6974 2063 616c 6c73 2074 6865  hat it calls the
-00000390: 2045 6e74 6974 792e 6472 6177 2829 206d   Entity.draw() m
-000003a0: 6574 686f 6420 696e 7374 6561 6420 6f66  ethod instead of
-000003b0: 0a20 2020 2020 2020 206a 7573 7420 626c  .        just bl
-000003c0: 6974 7469 6e67 2074 6865 2045 6e74 6974  itting the Entit
-000003d0: 792e 696d 6167 6520 746f 2074 6865 2073  y.image to the s
-000003e0: 6372 6565 6e2e 0a20 2020 2020 2020 204e  creen..        N
-000003f0: 2903 da07 7370 7269 7465 73da 0464 7261  )...sprites..dra
-00000400: 77da 0b6c 6f73 7473 7072 6974 6573 2905  w..lostsprites).
-00000410: 7209 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
-00000420: 0500 0000 da06 656e 7469 7479 720c 0000  ......entityr...
-00000430: 0072 0c00 0000 720d 0000 0072 1300 0000  .r....r....r....
-00000440: 1200 0000 7308 0000 0008 0608 010e 010a  ....s...........
-00000450: 017a 0a47 726f 7570 2e64 7261 7763 0100  .z.Group.drawc..
-00000460: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00000470: 0000 4300 0000 7316 0000 007c 0044 005d  ..C...s....|.D.]
-00000480: 067d 017c 01a0 00a1 0001 0071 0264 0153  .}.|.......q.d.S
-00000490: 0029 027a 890a 2020 2020 2020 2020 4b69  .).z..        Ki
-000004a0: 6c6c 2061 6c6c 2074 6865 2073 7072 6974  ll all the sprit
-000004b0: 6573 2069 6e20 7468 6973 2067 726f 7570  es in this group
-000004c0: 2e20 5468 6973 2069 7320 6469 6666 6572  . This is differ
-000004d0: 656e 7420 6672 6f6d 202e 656d 7074 7928  ent from .empty(
-000004e0: 292e 0a20 2020 2020 2020 2044 6f65 7320  )..        Does 
-000004f0: 6e6f 7420 6b69 6c6c 2074 6865 2073 7072  not kill the spr
-00000500: 6974 6573 2069 6e20 6f74 6865 7220 6772  ites in other gr
-00000510: 6f75 7073 2e0a 2020 2020 2020 2020 4e29  oups..        N)
-00000520: 01da 046b 696c 6c29 0272 0900 0000 da06  ...kill).r......
-00000530: 7370 7269 7465 720c 0000 0072 0c00 0000  spriter....r....
-00000540: 720d 0000 0072 1600 0000 1d00 0000 7306  r....r........s.
-00000550: 0000 0008 050a 0104 ff7a 0a47 726f 7570  .........z.Group
-00000560: 2e6b 696c 6c29 0472 0500 0000 7203 0000  .kill).r....r...
-00000570: 0072 0600 0000 4e29 0146 290c da08 5f5f  .r....N).F)...__
-00000580: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000590: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-000005a0: da07 5f5f 646f 635f 5f72 0800 0000 720e  ..__doc__r....r.
-000005b0: 0000 00da 0670 7967 616d 65da 0753 7572  .....pygame..Sur
-000005c0: 6661 6365 da04 626f 6f6c 7213 0000 0072  face..boolr....r
-000005d0: 1600 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
-000005e0: 6c5f 5f72 0c00 0000 720c 0000 0072 0a00  l__r....r....r..
-000005f0: 0000 720d 0000 0072 0400 0000 0800 0000  ..r....r........
-00000600: 730c 0000 0008 0004 010e 020c 0416 0310  s...............
-00000610: 0b72 0400 0000 2907 721c 0000 00da 0674  .r....).r......t
-00000620: 7970 696e 6772 0200 0000 da18 726f 6269  ypingr......robi
-00000630: 6e67 616d 652e 6f62 6a65 6374 732e 656e  ngame.objects.en
-00000640: 7469 7479 7203 0000 0072 1700 0000 7204  tityr....r....r.
-00000650: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
-00000660: 0000 720d 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000670: 3e01 0000 0073 0a00 0000 0800 0c01 0402  >....s..........
-00000680: 0c01 1803                                ....
+00000100: 7a20 436f 6e74 6169 6e65 7220 666f 7220  z Container for 
+00000110: 6d75 6c74 6970 6c65 2045 6e74 6974 6965  multiple Entitie
+00000120: 732e da08 656e 7469 7469 6573 7203 0000  s...entitiesr...
+00000130: 00da 0672 6574 7572 6e4e 6301 0000 0000  ...returnNc.....
+00000140: 0000 0000 0000 0002 0000 0002 0000 0007  ................
+00000150: 0000 00f3 1000 0000 7400 8300 6a01 7c01  ........t...j.|.
+00000160: 8e00 0100 6401 5300 2902 7a95 0a20 2020  ....d.S.).z..   
+00000170: 2020 2020 2044 6f65 7320 7468 6520 7361       Does the sa
+00000180: 6d65 2074 6869 6e67 2061 7320 7079 6761  me thing as pyga
+00000190: 6d65 2773 2060 4772 6f75 702e 6164 6428  me's `Group.add(
+000001a0: 2960 2e0a 2020 2020 2020 2020 4f6e 6c79  )`..        Only
+000001b0: 206f 7665 7272 6964 696e 6720 7468 6973   overriding this
+000001c0: 2062 6563 6175 7365 2070 7967 616d 6527   because pygame'
+000001d0: 7320 7479 7069 6e67 2077 6173 206d 616b  s typing was mak
+000001e0: 696e 6720 7468 6520 6c69 6e74 6572 2063  ing the linter c
+000001f0: 6f6d 706c 6169 6e2e 0a20 2020 2020 2020  omplain..       
+00000200: 204e 2902 da05 7375 7065 72da 0361 6464   N)...super..add
+00000210: 2902 da04 7365 6c66 7205 0000 00a9 01da  )...selfr.......
+00000220: 095f 5f63 6c61 7373 5f5f a900 fa35 2f68  .__class__...5/h
+00000230: 6f6d 652f 726f 6269 6e2f 636f 6465 2f72  ome/robin/code/r
+00000240: 6f62 696e 6761 6d65 2f72 6f62 696e 6761  obingame/robinga
+00000250: 6d65 2f6f 626a 6563 7473 2f67 726f 7570  me/objects/group
+00000260: 2e70 7972 0900 0000 0b00 0000 7302 0000  .pyr........s...
+00000270: 0010 057a 0947 726f 7570 2e61 6464 6301  ...z.Group.addc.
+00000280: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+00000290: 0000 0007 0000 0072 0700 0000 2902 7a3a  .......r....).z:
+000002a0: 0a20 2020 2020 2020 2043 616c 6c20 602e  .        Call `.
+000002b0: 7570 6461 7465 2829 6020 6f6e 2061 6c6c  update()` on all
+000002c0: 206d 656d 6265 7220 456e 7469 7469 6573   member Entities
+000002d0: 2e0a 2020 2020 2020 2020 4e29 0272 0800  ..        N).r..
+000002e0: 0000 da06 7570 6461 7465 2902 720a 0000  ....update).r...
+000002f0: 00da 0461 7267 7372 0b00 0000 720d 0000  ...argsr....r...
+00000300: 0072 0e00 0000 720f 0000 0012 0000 0073  .r....r........s
+00000310: 0200 0000 1004 7a0c 4772 6f75 702e 7570  ......z.Group.up
+00000320: 6461 7465 46da 0773 7572 6661 6365 da05  dateF..surface..
+00000330: 6465 6275 6763 0300 0000 0000 0000 0000  debugc..........
+00000340: 0000 0500 0000 0500 0000 4300 0000 7328  ..........C...s(
+00000350: 0000 007c 00a0 00a1 007d 037c 0344 005d  ...|.....}.|.D.]
+00000360: 087d 047c 04a0 017c 017c 02a1 0201 0071  .}.|...|.|.....q
+00000370: 0667 007c 005f 0264 0153 0029 0261 3301  .g.|._.d.S.).a3.
+00000380: 0000 0a20 2020 2020 2020 2043 616c 6c20  ...        Call 
+00000390: 602e 6472 6177 2873 7572 6661 6365 2c20  `.draw(surface, 
+000003a0: 6465 6275 6729 6020 6f6e 2061 6c6c 206d  debug)` on all m
+000003b0: 656d 6265 7220 456e 7469 7469 6573 2e0a  ember Entities..
+000003c0: 0a20 2020 2020 2020 2054 6869 7320 6973  .        This is
+000003d0: 2064 6966 6665 7265 6e74 2066 726f 6d20   different from 
+000003e0: 7079 6761 6d65 2773 2060 4772 6f75 702e  pygame's `Group.
+000003f0: 6472 6177 2829 6020 696e 2074 6861 7420  draw()` in that 
+00000400: 6974 2063 616c 6c73 2074 6865 2060 456e  it calls the `En
+00000410: 7469 7479 2e64 7261 7728 2960 206d 6574  tity.draw()` met
+00000420: 686f 640a 2020 2020 2020 2020 2874 6875  hod.        (thu
+00000430: 7320 616c 6c6f 7769 6e67 2074 6865 2045  s allowing the E
+00000440: 6e74 6974 7920 746f 2064 6563 6964 6520  ntity to decide 
+00000450: 686f 7720 746f 2064 7261 7720 6974 7365  how to draw itse
+00000460: 6c66 2920 696e 7374 6561 6420 6f66 206a  lf) instead of j
+00000470: 7573 7420 626c 6974 7469 6e67 2074 6865  ust blitting the
+00000480: 0a20 2020 2020 2020 2045 6e74 6974 7927  .        Entity'
+00000490: 7320 602e 696d 6167 6560 206f 6e74 6f20  s `.image` onto 
+000004a0: 7468 6520 7375 7266 6163 652e 0a20 2020  the surface..   
+000004b0: 2020 2020 204e 2903 da07 7370 7269 7465       N)...sprite
+000004c0: 73da 0464 7261 77da 0b6c 6f73 7473 7072  s..draw..lostspr
+000004d0: 6974 6573 2905 720a 0000 0072 1100 0000  ites).r....r....
+000004e0: 7212 0000 0072 0500 0000 da06 656e 7469  r....r......enti
+000004f0: 7479 720d 0000 0072 0d00 0000 720e 0000  tyr....r....r...
+00000500: 0072 1400 0000 1800 0000 7308 0000 0008  .r........s.....
+00000510: 0808 010e 010a 017a 0a47 726f 7570 2e64  .......z.Group.d
+00000520: 7261 7763 0100 0000 0000 0000 0000 0000  rawc............
+00000530: 0200 0000 0300 0000 4300 0000 7316 0000  ........C...s...
+00000540: 007c 0044 005d 067d 017c 01a0 00a1 0001  .|.D.].}.|......
+00000550: 0071 0264 0153 0029 027a 730a 2020 2020  .q.d.S.).zs.    
+00000560: 2020 2020 4361 6c6c 2060 2e6b 696c 6c28      Call `.kill(
+00000570: 2960 206f 6e20 616c 6c20 7468 6520 656e  )` on all the en
+00000580: 7469 7469 6573 2069 6e20 7468 6973 2067  tities in this g
+00000590: 726f 7570 2e0a 2020 2020 2020 2020 5468  roup..        Th
+000005a0: 6973 2069 7320 6469 6666 6572 656e 7420  is is different 
+000005b0: 6672 6f6d 2060 4772 6f75 702e 656d 7074  from `Group.empt
+000005c0: 7928 2960 2e0a 2020 2020 2020 2020 4e29  y()`..        N)
+000005d0: 01da 046b 696c 6c29 0272 0a00 0000 7216  ...kill).r....r.
+000005e0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+000005f0: 0000 7217 0000 0025 0000 0073 0600 0000  ..r....%...s....
+00000600: 0805 0a01 04ff 7a0a 4772 6f75 702e 6b69  ......z.Group.ki
+00000610: 6c6c 2904 7205 0000 0072 0300 0000 7206  ll).r....r....r.
+00000620: 0000 004e 2901 4629 0cda 085f 5f6e 616d  ...N).F)...__nam
+00000630: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000640: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
+00000650: 5f64 6f63 5f5f 7209 0000 0072 0f00 0000  _doc__r....r....
+00000660: da06 7079 6761 6d65 da07 5375 7266 6163  ..pygame..Surfac
+00000670: 65da 0462 6f6f 6c72 1400 0000 7217 0000  e..boolr....r...
+00000680: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
+00000690: 720d 0000 0072 0d00 0000 720b 0000 0072  r....r....r....r
+000006a0: 0e00 0000 7204 0000 0008 0000 0073 0c00  ....r........s..
+000006b0: 0000 0800 0401 0e02 0c07 1606 100d 7204  ..............r.
+000006c0: 0000 0029 0772 1c00 0000 da06 7479 7069  ...).r......typi
+000006d0: 6e67 7202 0000 00da 1872 6f62 696e 6761  ngr......robinga
+000006e0: 6d65 2e6f 626a 6563 7473 2e65 6e74 6974  me.objects.entit
+000006f0: 7972 0300 0000 da06 7370 7269 7465 7204  yr......spriter.
+00000700: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
+00000710: 0000 720e 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000720: 3e01 0000 0073 0a00 0000 0800 0c01 0402  >....s..........
+00000730: 0c01 1803                                ....
```

### Comparing `robingame-0.1.0/robingame/objects/__pycache__/helpers.cpython-310.pyc` & `robingame-1.0.1/robingame/objects/__pycache__/helpers.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jul  5 13:47:52 2023 UTC, .py size: 1188 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8874 a564 a404 0000  o........t.d....
+00000000: 6f0d 0d0a 0000 0000 0d1d b464 a904 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6407 6408 8400 6408 6508 8303  ..G.d.d...d.e...
@@ -13,95 +13,95 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0005  ................
 000000d0: 0000 0000 0000 0073 5200 0000 6500 5a01  .......sR...e.Z.
 000000e0: 6400 5a02 5500 6401 5a03 6402 5a04 6505  d.Z.U.d.Z.d.Z.e.
 000000f0: 6a06 5a07 6508 6509 6403 3c00 640f 8700  j.Z.e.e.d.<.d...
 00000100: 6601 6406 6407 840c 5a0a 6408 6409 8400  f.d.d...Z.d.d...
 00000110: 5a0b 6410 640b 650c 640c 650d 6604 640d  Z.d.d.e.d.e.f.d.
 00000120: 640e 8405 5a0e 8700 0400 5a0f 5300 2911  d...Z.....Z.S.).
-00000130: da0a 4670 7354 7261 636b 6572 7a45 4469  ..FpsTrackerzEDi
-00000140: 7370 6c61 7973 2061 206c 6974 746c 6520  splays a little 
-00000150: 6e75 6d62 6572 2069 6e20 7468 6520 746f  number in the to
-00000160: 7020 7269 6768 7420 6f66 2074 6865 2077  p right of the w
-00000170: 696e 646f 7720 6966 2064 6562 7567 3d54  indow if debug=T
-00000180: 7275 65e9 3c00 0000 da03 6670 73da 0672  rue.<.....fps..r
-00000190: 6574 7572 6e4e 6301 0000 0000 0000 0000  eturnNc.........
-000001a0: 0000 0002 0000 0003 0000 0007 0000 0073  ...............s
-000001b0: 1e00 0000 7400 8300 6a01 7c01 8e00 0100  ....t...j.|.....
-000001c0: 7402 7c00 6a03 6401 8d01 7c00 5f04 6400  t.|.j.d...|._.d.
-000001d0: 5300 2902 4e29 01da 066d 6178 6c65 6e29  S.).N)...maxlen)
-000001e0: 05da 0573 7570 6572 da08 5f5f 696e 6974  ...super..__init
-000001f0: 5f5f 7202 0000 00da 0d62 7566 6665 725f  __r......buffer_
-00000200: 6c65 6e67 7468 da05 7175 6575 6529 02da  length..queue)..
-00000210: 0473 656c 66da 0667 726f 7570 73a9 01da  .self..groups...
-00000220: 095f 5f63 6c61 7373 5f5f a900 fa37 2f68  .__class__...7/h
-00000230: 6f6d 652f 726f 6269 6e2f 636f 6465 2f72  ome/robin/code/r
-00000240: 6f62 696e 6761 6d65 2f72 6f62 696e 6761  obingame/robinga
-00000250: 6d65 2f6f 626a 6563 7473 2f68 656c 7065  me/objects/helpe
-00000260: 7273 2e70 7972 0d00 0000 1200 0000 7304  rs.pyr........s.
-00000270: 0000 000c 0112 017a 1346 7073 5472 6163  .......z.FpsTrac
-00000280: 6b65 722e 5f5f 696e 6974 5f5f 6301 0000  ker.__init__c...
-00000290: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-000002a0: 0043 0000 0073 4a00 0000 7400 a001 a100  .C...sJ...t.....
-000002b0: 7d01 7c00 6a02 a003 7c01 a101 0100 7c00  }.|.j...|.....|.
-000002c0: 6a02 6401 1900 7c00 6a02 6402 1900 1800  j.d...|.j.d.....
-000002d0: 7d02 7c02 7220 7404 7c00 6a05 7c02 1b00  }.|.r t.|.j.|...
-000002e0: 8301 7c00 5f06 6400 5300 6402 7c00 5f06  ..|._.d.S.d.|._.
-000002f0: 6400 5300 2903 4ee9 ffff ffff 7201 0000  d.S.).N.....r...
-00000300: 0029 07da 0474 696d 65da 0c70 6572 665f  .)...time..perf_
-00000310: 636f 756e 7465 7272 0f00 0000 da06 6170  counterr......ap
-00000320: 7065 6e64 da03 696e 7472 0e00 0000 7209  pend..intr....r.
-00000330: 0000 0029 0372 1000 0000 da01 74da 0773  ...).r......t..s
-00000340: 6563 6f6e 6473 7214 0000 0072 1400 0000  econdsr....r....
-00000350: 7215 0000 00da 0675 7064 6174 6516 0000  r......update...
-00000360: 0073 0800 0000 0801 0c01 1401 2201 7a11  .s..........".z.
-00000370: 4670 7354 7261 636b 6572 2e75 7064 6174  FpsTracker.updat
-00000380: 6546 da07 7375 7266 6163 65da 0564 6562  eF..surface..deb
-00000390: 7567 6303 0000 0000 0000 0000 0000 0007  ugc.............
-000003a0: 0000 0007 0000 0043 0000 0073 8800 0000  .......C...s....
-000003b0: 7c02 7242 6401 7d03 6402 7c03 1400 7d04  |.rBd.}.d.|...}.
-000003c0: 7400 7c04 7c04 6403 1a00 6602 8301 7d05  t.|.|.d...f...}.
-000003d0: 7c05 a001 7402 6404 8301 a101 0100 7c00  |...t.d.......|.
-000003e0: 6a03 6a04 7c05 6405 7c00 6a05 9b00 9d02  j.j.|.d.|.j.....
-000003f0: 7c04 6406 7c03 6407 8d05 0100 7c05 a006  |.d.|.d.....|...
-00000400: a100 7d06 7c01 a006 a100 6a07 6408 1800  ..}.|.....j.d...
-00000410: 7c06 5f07 7c01 a006 a100 6a08 6408 1700  |._.|.....j.d...
-00000420: 7c06 5f08 7c01 a009 7c05 7c06 a102 0100  |._.|...|.|.....
-00000430: 6400 5300 6400 5300 2909 4ee9 0200 0000  d.S.d.S.).N.....
-00000440: e932 0000 00e9 0400 0000 da05 7768 6974  .2..........whit
-00000450: 657a 0546 5053 3a20 7201 0000 0029 03da  ez.FPS: r....)..
-00000460: 0477 7261 70da 0561 6c69 676e da05 7363  .wrap..align..sc
-00000470: 616c 65e9 0a00 0000 290a 7204 0000 00da  ale.....).r.....
-00000480: 0466 696c 6c72 0300 0000 da04 666f 6e74  .fillr......font
-00000490: da06 7265 6e64 6572 7209 0000 00da 0867  ..renderr......g
-000004a0: 6574 5f72 6563 74da 0572 6967 6874 da03  et_rect..right..
-000004b0: 746f 70da 0462 6c69 7429 0772 1000 0000  top..blit).r....
-000004c0: 721e 0000 0072 1f00 0000 7226 0000 00da  r....r....r&....
-000004d0: 0577 6964 7468 da04 7375 7266 da04 7265  .width..surf..re
-000004e0: 6374 7214 0000 0072 1400 0000 7215 0000  ctr....r....r...
-000004f0: 00da 0464 7261 771c 0000 0073 1600 0000  ...draw....s....
-00000500: 0401 0401 0801 1001 0e01 1e01 0801 1001  ................
-00000510: 1001 1001 04f7 7a0f 4670 7354 7261 636b  ......z.FpsTrack
-00000520: 6572 2e64 7261 7729 0272 0a00 0000 4e29  er.draw).r....N)
-00000530: 0146 2910 da08 5f5f 6e61 6d65 5f5f da0a  .F)...__name__..
-00000540: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000550: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-00000560: 5f72 0e00 0000 7206 0000 00da 0f63 656c  _r....r......cel
-00000570: 6c70 686f 6e65 5f62 6c61 636b 7229 0000  lphone_blackr)..
-00000580: 0072 1a00 0000 da0f 5f5f 616e 6e6f 7461  .r......__annota
-00000590: 7469 6f6e 735f 5f72 0d00 0000 721d 0000  tions__r....r...
-000005a0: 0072 0400 0000 da04 626f 6f6c 7232 0000  .r......boolr2..
-000005b0: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-000005c0: 7214 0000 0072 1400 0000 7212 0000 0072  r....r....r....r
-000005d0: 1500 0000 7207 0000 000b 0000 0073 1000  ....r........s..
-000005e0: 0000 0a00 0401 0402 0601 0801 0e02 0804  ................
-000005f0: 1c06 7207 0000 0029 0c72 1700 0000 da0b  ..r....).r......
-00000600: 636f 6c6c 6563 7469 6f6e 7372 0200 0000  collectionsr....
-00000610: da0c 7079 6761 6d65 2e63 6f6c 6f72 7203  ..pygame.colorr.
-00000620: 0000 00da 0e70 7967 616d 652e 7375 7266  .....pygame.surf
-00000630: 6163 6572 0400 0000 da18 726f 6269 6e67  acer......robing
-00000640: 616d 652e 6f62 6a65 6374 732e 656e 7469  ame.objects.enti
-00000650: 7479 7205 0000 00da 1372 6f62 696e 6761  tyr......robinga
-00000660: 6d65 2e74 6578 742e 666f 6e74 7206 0000  me.text.fontr...
-00000670: 0072 0700 0000 7214 0000 0072 1400 0000  .r....r....r....
-00000680: 7214 0000 0072 1500 0000 da08 3c6d 6f64  r....r......<mod
-00000690: 756c 653e 0100 0000 730e 0000 0008 000c  ule>....s.......
-000006a0: 010c 020c 010c 020c 0114 03              ...........
+00000130: da0a 4670 7354 7261 636b 6572 7a4f 0a20  ..FpsTrackerzO. 
+00000140: 2020 2044 6973 706c 6179 7320 6120 6c69     Displays a li
+00000150: 7474 6c65 206e 756d 6265 7220 696e 2074  ttle number in t
+00000160: 6865 2074 6f70 2072 6967 6874 206f 6620  he top right of 
+00000170: 7468 6520 7769 6e64 6f77 2069 6620 6465  the window if de
+00000180: 6275 673d 5472 7565 0a20 2020 20e9 3c00  bug=True.    .<.
+00000190: 0000 da03 6670 73da 0672 6574 7572 6e4e  ....fps..returnN
+000001a0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000001b0: 0003 0000 0007 0000 0073 1e00 0000 7400  .........s....t.
+000001c0: 8300 6a01 7c01 8e00 0100 7402 7c00 6a03  ..j.|.....t.|.j.
+000001d0: 6401 8d01 7c00 5f04 6400 5300 2902 4e29  d...|._.d.S.).N)
+000001e0: 01da 066d 6178 6c65 6e29 05da 0573 7570  ...maxlen)...sup
+000001f0: 6572 da08 5f5f 696e 6974 5f5f 7202 0000  er..__init__r...
+00000200: 00da 0d62 7566 6665 725f 6c65 6e67 7468  ...buffer_length
+00000210: da05 7175 6575 6529 02da 0473 656c 66da  ..queue)...self.
+00000220: 0667 726f 7570 73a9 01da 095f 5f63 6c61  .groups....__cla
+00000230: 7373 5f5f a900 fa37 2f68 6f6d 652f 726f  ss__...7/home/ro
+00000240: 6269 6e2f 636f 6465 2f72 6f62 696e 6761  bin/code/robinga
+00000250: 6d65 2f72 6f62 696e 6761 6d65 2f6f 626a  me/robingame/obj
+00000260: 6563 7473 2f68 656c 7065 7273 2e70 7972  ects/helpers.pyr
+00000270: 0d00 0000 1400 0000 7304 0000 000c 0112  ........s.......
+00000280: 017a 1346 7073 5472 6163 6b65 722e 5f5f  .z.FpsTracker.__
+00000290: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+000002a0: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
+000002b0: 4a00 0000 7400 a001 a100 7d01 7c00 6a02  J...t.....}.|.j.
+000002c0: a003 7c01 a101 0100 7c00 6a02 6401 1900  ..|.....|.j.d...
+000002d0: 7c00 6a02 6402 1900 1800 7d02 7c02 7220  |.j.d.....}.|.r 
+000002e0: 7404 7c00 6a05 7c02 1b00 8301 7c00 5f06  t.|.j.|.....|._.
+000002f0: 6400 5300 6402 7c00 5f06 6400 5300 2903  d.S.d.|._.d.S.).
+00000300: 4ee9 ffff ffff 7201 0000 0029 07da 0474  N.....r....)...t
+00000310: 696d 65da 0c70 6572 665f 636f 756e 7465  ime..perf_counte
+00000320: 7272 0f00 0000 da06 6170 7065 6e64 da03  rr......append..
+00000330: 696e 7472 0e00 0000 7209 0000 0029 0372  intr....r....).r
+00000340: 1000 0000 da01 74da 0773 6563 6f6e 6473  ......t..seconds
+00000350: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+00000360: 0675 7064 6174 6518 0000 0073 0800 0000  .update....s....
+00000370: 0801 0c01 1401 2201 7a11 4670 7354 7261  ......".z.FpsTra
+00000380: 636b 6572 2e75 7064 6174 6546 da07 7375  cker.updateF..su
+00000390: 7266 6163 65da 0564 6562 7567 6303 0000  rface..debugc...
+000003a0: 0000 0000 0000 0000 0007 0000 0007 0000  ................
+000003b0: 0043 0000 0073 8800 0000 7c02 7242 6401  .C...s....|.rBd.
+000003c0: 7d03 6402 7c03 1400 7d04 7400 7c04 7c04  }.d.|...}.t.|.|.
+000003d0: 6403 1a00 6602 8301 7d05 7c05 a001 7402  d...f...}.|...t.
+000003e0: 6404 8301 a101 0100 7c00 6a03 6a04 7c05  d.......|.j.j.|.
+000003f0: 6405 7c00 6a05 9b00 9d02 7c04 6406 7c03  d.|.j.....|.d.|.
+00000400: 6407 8d05 0100 7c05 a006 a100 7d06 7c01  d.....|.....}.|.
+00000410: a006 a100 6a07 6408 1800 7c06 5f07 7c01  ....j.d...|._.|.
+00000420: a006 a100 6a08 6408 1700 7c06 5f08 7c01  ....j.d...|._.|.
+00000430: a009 7c05 7c06 a102 0100 6400 5300 6400  ..|.|.....d.S.d.
+00000440: 5300 2909 4ee9 0200 0000 e932 0000 00e9  S.).N......2....
+00000450: 0400 0000 da05 7768 6974 657a 0546 5053  ......whitez.FPS
+00000460: 3a20 7201 0000 0029 03da 0477 7261 70da  : r....)...wrap.
+00000470: 0561 6c69 676e da05 7363 616c 65e9 0a00  .align..scale...
+00000480: 0000 290a 7204 0000 00da 0466 696c 6c72  ..).r......fillr
+00000490: 0300 0000 da04 666f 6e74 da06 7265 6e64  ......font..rend
+000004a0: 6572 7209 0000 00da 0867 6574 5f72 6563  err......get_rec
+000004b0: 74da 0572 6967 6874 da03 746f 70da 0462  t..right..top..b
+000004c0: 6c69 7429 0772 1000 0000 721e 0000 0072  lit).r....r....r
+000004d0: 1f00 0000 7226 0000 00da 0577 6964 7468  ....r&.....width
+000004e0: da04 7375 7266 da04 7265 6374 7214 0000  ..surf..rectr...
+000004f0: 0072 1400 0000 7215 0000 00da 0464 7261  .r....r......dra
+00000500: 771e 0000 0073 1600 0000 0401 0401 0801  w....s..........
+00000510: 1001 0e01 1e01 0801 1001 1001 1001 04f7  ................
+00000520: 7a0f 4670 7354 7261 636b 6572 2e64 7261  z.FpsTracker.dra
+00000530: 7729 0272 0a00 0000 4e29 0146 2910 da08  w).r....N).F)...
+00000540: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000550: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000560: 5f5f da07 5f5f 646f 635f 5f72 0e00 0000  __..__doc__r....
+00000570: 7206 0000 00da 0f63 656c 6c70 686f 6e65  r......cellphone
+00000580: 5f62 6c61 636b 7229 0000 0072 1a00 0000  _blackr)...r....
+00000590: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
+000005a0: 5f72 0d00 0000 721d 0000 0072 0400 0000  _r....r....r....
+000005b0: da04 626f 6f6c 7232 0000 00da 0d5f 5f63  ..boolr2.....__c
+000005c0: 6c61 7373 6365 6c6c 5f5f 7214 0000 0072  lasscell__r....r
+000005d0: 1400 0000 7212 0000 0072 1500 0000 7207  ....r....r....r.
+000005e0: 0000 000b 0000 0073 1000 0000 0a00 0401  .......s........
+000005f0: 0404 0601 0801 0e02 0804 1c06 7207 0000  ............r...
+00000600: 0029 0c72 1700 0000 da0b 636f 6c6c 6563  .).r......collec
+00000610: 7469 6f6e 7372 0200 0000 da0c 7079 6761  tionsr......pyga
+00000620: 6d65 2e63 6f6c 6f72 7203 0000 00da 0e70  me.colorr......p
+00000630: 7967 616d 652e 7375 7266 6163 6572 0400  ygame.surfacer..
+00000640: 0000 da18 726f 6269 6e67 616d 652e 6f62  ....robingame.ob
+00000650: 6a65 6374 732e 656e 7469 7479 7205 0000  jects.entityr...
+00000660: 00da 0e72 6f62 696e 6761 6d65 2e74 6578  ...robingame.tex
+00000670: 7472 0600 0000 7207 0000 0072 1400 0000  tr....r....r....
+00000680: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+00000690: 083c 6d6f 6475 6c65 3e01 0000 0073 0e00  .<module>....s..
+000006a0: 0000 0800 0c01 0c02 0c01 0c02 0c01 1403  ................
```

### Comparing `robingame-0.1.0/robingame/objects/__pycache__/particles.cpython-310.pyc` & `robingame-1.0.1/robingame/objects/__pycache__/particles.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/objects/entity.py` & `robingame-1.0.1/robingame/objects/entity.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,68 +5,89 @@
 
 from robingame.objects.group import Group
 
 
 class Entity(pygame.sprite.Sprite):
     """
     Finite State Machine:
-    - self.state is executed every tick
-    - self.tick is incremented every time the main game loop executes
-    - when self.state changes, self.tick is set to 0, so you can track how long the entity has
+
+    - `self.state` is executed every tick
+    - `self.tick` is incremented every time the main game loop executes
+    - when `self.state` changes, `self.tick` is set to 0, so you can track how long the entity has
       been in its current state
 
     Hierarchical structure:
-    - Entities can be added to Groups to create a hierarchical structure
+
+    - `Entities` can be added to `Groups` to create a hierarchical structure
     - The order of groups in the .child_groups attribute determines the draw order; it's basically
       the layers
 
     Example game structure:
+    ```
     Game: Entity
     └── scenes: Group
         └── MainMenu: Entity
             ├── buttons: Group
             │   ├── Button: Entity
             │   ├── Button: Entity
             │   └── Button: Entity
             └── sliders: Group
                 ├── Slider: Entity
                 └── Slider: Entity
-
+    ```
     """
 
     _state: Callable = lambda *args, **kwargs: None  # default state: do nothing
     child_groups: list[Group]  # groups of child Entities belonging to this entity
     tick: int = 0  # number of game loop iterations elapsed in the current state
 
     def __init__(self, groups: Iterable[Group] = ()):
         super().__init__(*groups)
         self.child_groups = []
 
     def update(self):
+        """
+        Execute `self.state`.
+
+        Call `.update()` on all child groups. This allows the entire tree of objects to update by
+        only calling the `.update()` method of the root object.
+
+        Subclasses can override this method to provide subclass-specific behaviour. However,
+        it's generally a better idea to write state functions and allow the Entity's Finite State
+        Machine mechanism to execute them.
+
+        Increment `self.tick` to keep track of how long we've been in the current state.
+        """
         self.state()  # execute current state function
-        # update all child groups. This allows the entire tree of objects to update by only
-        # calling the .update() method of the root object
         for group in self.child_groups:
             group.update()
         self.tick += 1  # increment tick to keep track of how long we've been in the current state
 
     def draw(self, surface: Surface, debug: bool = False):
-        # draw all child groups. This allows the entire tree of objects to draw by only calling
-        # the .draw() method of the root object.
+        """
+        Draw all child groups. This allows the entire tree of objects to draw by only calling the
+        .draw() method of the root object.
+
+
+        Args:
+            surface: the surface (usually the screen) on which to draw self
+            debug: if True, draw extra stuff for debugging
+        """
         for group in self.child_groups:
             group.draw(surface, debug)
 
     def kill(self):
-        """Removes self from all groups it is a member of."""
+        """Removes self from all groups."""
         for group in self.child_groups:
             group.kill()
         super().kill()
 
     @property
     def state(self):
+        """Execute the current state function."""
         return self._state
 
     @state.setter
     def state(self, new_state):
         """
         Reset self.tick when state changes so we know how long we've been in the current state.
         """
```

### Comparing `robingame-0.1.0/robingame/objects/group.py` & `robingame-1.0.1/robingame/objects/group.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,34 +2,42 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from robingame.objects.entity import Entity
 
 
 class Group(pygame.sprite.Group):
-    """Container for multiple Entity objects."""
+    """Container for multiple Entities."""
 
     def add(self, *entities: "Entity") -> None:
-        """Only overriding this because pygame's typing was making the linter complain."""
+        """
+        Does the same thing as pygame's `Group.add()`.
+        Only overriding this because pygame's typing was making the linter complain.
+        """
         super().add(*entities)
 
     def update(self, *args):
+        """
+        Call `.update()` on all member Entities.
+        """
         super().update(*args)
 
     def draw(self, surface: pygame.Surface, debug: bool = False):
         """
-        Draws all of the member sprites onto the given surface.
-        Different from pygame's Group.draw in that it calls the Entity.draw() method instead of
-        just blitting the Entity.image to the screen.
+        Call `.draw(surface, debug)` on all member Entities.
+
+        This is different from pygame's `Group.draw()` in that it calls the `Entity.draw()` method
+        (thus allowing the Entity to decide how to draw itself) instead of just blitting the
+        Entity's `.image` onto the surface.
         """
         entities = self.sprites()
         for entity in entities:
             entity.draw(surface, debug)
         self.lostsprites = []
 
     def kill(self):
         """
-        Kill all the sprites in this group. This is different from .empty().
-        Does not kill the sprites in other groups.
+        Call `.kill()` on all the entities in this group.
+        This is different from `Group.empty()`.
         """
-        for sprite in self:
-            sprite.kill()
+        for entity in self:
+            entity.kill()
```

### Comparing `robingame-0.1.0/robingame/objects/helpers.py` & `robingame-1.0.1/robingame/objects/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import time
 from collections import deque
 
 from pygame.color import Color
 from pygame.surface import Surface
 
 from robingame.objects.entity import Entity
-from robingame.text.font import fonts
+from robingame.text import fonts
 
 
 class FpsTracker(Entity):
-    """Displays a little number in the top right of the window if debug=True"""
+    """
+    Displays a little number in the top right of the window if debug=True
+    """
 
     buffer_length = 60
     font = fonts.cellphone_black
     fps: int
 
     def __init__(self, *groups) -> None:
         super().__init__(*groups)
```

### Comparing `robingame-0.1.0/robingame/objects/particles.py` & `robingame-1.0.1/robingame/objects/particles.py`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/recording.py` & `robingame-1.0.1/robingame/recording.py`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/sound.py` & `robingame-1.0.1/robingame/sound.py`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/text/assets/cellphone-black.png` & `robingame-1.0.1/robingame/text/assets/cellphone-black.png`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/text/assets/cellphone-white.png` & `robingame-1.0.1/robingame/text/assets/cellphone-white.png`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/text/assets/test_font.aseprite` & `robingame-1.0.1/robingame/text/assets/test_font.aseprite`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/text/assets/test_font.png` & `robingame-1.0.1/robingame/text/assets/test_font.png`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/robingame/text/font/__pycache__/fonts.cpython-310.pyc` & `robingame-1.0.1/robingame/text/__pycache__/fonts.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 29 14:47:25 2023 UTC, .py size: 1415 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,67 @@
-00000000: 6f0d 0d0a 0000 0000 7d99 9d64 8705 0000  o.......}..d....
+00000000: 6f0d 0d0a 0000 0000 0d1d b464 8005 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0009 0000 0040 0000 0073 ee00 0000 6400  .....@...s....d.
+00000020: 0009 0000 0040 0000 0073 ec00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6504 8300 5a07  d.l.m.Z...e...Z.
-00000060: 6502 6508 8301 6a09 6a09 6405 1b00 5a0a  e.e...j.j.d...Z.
-00000070: 6506 650a 6406 1b00 6407 6500 6a0b 6500  e.e.d...d.e.j.e.
-00000080: 6a0c 1700 6408 1700 6409 640a 640b 640c  j...d...d.d.d.d.
-00000090: 8d06 5a0d 6506 650a 640d 1b00 640e 640f  ..Z.e.e.d...d.d.
-000000a0: 6500 6a0b 1700 6410 1700 6500 6a0c 1700  e.j...d...e.j...
-000000b0: 6411 1700 640a 6412 6409 6413 6414 8d07  d...d.d.d.d.d...
-000000c0: 5a0e 6506 650a 6415 1b00 640e 640f 6500  Z.e.e.d...d.d.e.
-000000d0: 6a0b 1700 6410 1700 6500 6a0c 1700 6411  j...d...e.j...d.
-000000e0: 1700 640a 6412 6409 6413 6414 8d07 5a0f  ..d.d.d.d.d...Z.
-000000f0: 6506 650a 6415 1b00 640e 640f 6500 6a0b  e.e.d...d.d.e.j.
-00000100: 1700 6410 1700 6500 6a0c 1700 6411 1700  ..d...e.j...d...
-00000110: 6412 6416 8d04 5a10 6401 5300 2917 e900  d.d...Z.d.S.)...
-00000120: 0000 004e 2901 da04 5061 7468 2901 da0c  ...N)...Path)...
-00000130: 696e 6974 5f64 6973 706c 6179 2901 da04  init_display)...
-00000140: 466f 6e74 da06 6173 7365 7473 7a0d 7465  Font..assetsz.te
-00000150: 7374 5f66 6f6e 742e 706e 6729 02e9 1000  st_font.png)....
-00000160: 0000 7206 0000 007a 2b31 3233 3435 3637  ..r....z+1234567
-00000170: 3839 302d 3d21 4023 2425 5e26 2a28 295f  890-=!@#$%^&*()_
-00000180: 2b5b 5d5c 3b27 2c2e 2f7b 7d7c 3a5c 223c  +[]\;',./{}|:\"<
-00000190: 3e3f 7e60 54e9 0100 0000 e908 0000 0029  >?~`T..........)
-000001a0: 06da 0866 696c 656e 616d 65da 0a69 6d61  ...filename..ima
-000001b0: 6765 5f73 697a 65da 076c 6574 7465 7273  ge_size..letters
-000001c0: da04 7472 696d da04 7870 6164 da0b 7370  ..trim..xpad..sp
-000001d0: 6163 655f 7769 6474 687a 1363 656c 6c70  ace_widthz.cellp
-000001e0: 686f 6e65 2d62 6c61 636b 2e70 6e67 2902  hone-black.png).
-000001f0: e907 0000 00e9 0900 0000 7a20 2122 2324  ..........z !"#$
-00000200: 2526 2728 292a 2b2c 2d2e 2f30 3132 3334  %&'()*+,-./01234
-00000210: 3536 3738 393a 3b3c 3d3e 3f40 7a06 5b5c  56789:;<=>?@z.[\
-00000220: 5d5e 5f60 7a04 7b7c 7d7e e9ff ffff ffe9  ]^_`z.{|}~......
-00000230: 0400 0000 2907 7209 0000 0072 0a00 0000  ....).r....r....
-00000240: 720b 0000 0072 0d00 0000 da08 636f 6c6f  r....r......colo
-00000250: 726b 6579 720c 0000 0072 0e00 0000 7a13  rkeyr....r....z.
-00000260: 6365 6c6c 7068 6f6e 652d 7768 6974 652e  cellphone-white.
-00000270: 706e 6729 0472 0900 0000 720a 0000 0072  png).r....r....r
-00000280: 0b00 0000 7213 0000 0029 11da 0673 7472  ....r....)...str
-00000290: 696e 67da 0770 6174 686c 6962 7202 0000  ing..pathlibr...
-000002a0: 00da 0f72 6f62 696e 6761 6d65 2e69 6d61  ...robingame.ima
-000002b0: 6765 7203 0000 00da 1372 6f62 696e 6761  ger......robinga
-000002c0: 6d65 2e74 6578 742e 666f 6e74 7204 0000  me.text.fontr...
-000002d0: 00da 0677 696e 646f 77da 085f 5f66 696c  ...window..__fil
-000002e0: 655f 5fda 0670 6172 656e 7472 0500 0000  e__..parentr....
-000002f0: da0f 6173 6369 695f 7570 7065 7263 6173  ..ascii_uppercas
-00000300: 65da 0f61 7363 6969 5f6c 6f77 6572 6361  e..ascii_lowerca
-00000310: 7365 da09 7465 7374 5f66 6f6e 74da 0f63  se..test_font..c
-00000320: 656c 6c70 686f 6e65 5f62 6c61 636b da0f  ellphone_black..
-00000330: 6365 6c6c 7068 6f6e 655f 7768 6974 65da  cellphone_white.
-00000340: 1463 656c 6c70 686f 6e65 5f77 6869 7465  .cellphone_white
-00000350: 5f6d 6f6e 6fa9 0072 2100 0000 7221 0000  _mono..r!...r!..
-00000360: 00fa 372f 686f 6d65 2f72 6f62 696e 2f63  ..7/home/robin/c
-00000370: 6f64 652f 726f 6269 6e67 616d 652f 726f  ode/robingame/ro
-00000380: 6269 6e67 616d 652f 7465 7874 2f66 6f6e  bingame/text/fon
-00000390: 742f 666f 6e74 732e 7079 da08 3c6d 6f64  t/fonts.py..<mod
-000003a0: 756c 653e 0100 0000 7384 0000 0008 000c  ule>....s.......
-000003b0: 010c 020c 0106 0210 0202 0206 0102 0104  ................
-000003c0: 0204 0102 ff02 0202 fe02 0402 0102 0106  ................
-000003d0: f602 0d06 0102 0102 0204 0102 ff02 0202  ................
-000003e0: fe04 0302 fd02 0402 fc02 0602 0102 0102  ................
-000003f0: 0106 f302 0f06 0102 0102 0204 0102 ff02  ................
-00000400: 0202 fe04 0302 fd02 0402 fc02 0602 0102  ................
-00000410: 0102 0106 f302 0f06 0102 0102 0204 0102  ................
-00000420: ff02 0202 fe04 0302 fd02 0402 fc02 060a  ................
-00000430: f6                                       .
+00000060: 6502 6508 8301 6a09 6405 1b00 5a0a 6506  e.e...j.d...Z.e.
+00000070: 650a 6406 1b00 6407 6500 6a0b 6500 6a0c  e.d...d.e.j.e.j.
+00000080: 1700 6408 1700 6409 640a 640b 640c 8d06  ..d...d.d.d.d...
+00000090: 5a0d 6506 650a 640d 1b00 640e 640f 6500  Z.e.e.d...d.d.e.
+000000a0: 6a0b 1700 6410 1700 6500 6a0c 1700 6411  j...d...e.j...d.
+000000b0: 1700 640a 6412 6409 6413 6414 8d07 5a0e  ..d.d.d.d.d...Z.
+000000c0: 6506 650a 6415 1b00 640e 640f 6500 6a0b  e.e.d...d.d.e.j.
+000000d0: 1700 6410 1700 6500 6a0c 1700 6411 1700  ..d...e.j...d...
+000000e0: 640a 6412 6409 6413 6414 8d07 5a0f 6506  d.d.d.d.d...Z.e.
+000000f0: 650a 6415 1b00 640e 640f 6500 6a0b 1700  e.d...d.d.e.j...
+00000100: 6410 1700 6500 6a0c 1700 6411 1700 6412  d...e.j...d...d.
+00000110: 6416 8d04 5a10 6401 5300 2917 e900 0000  d...Z.d.S.).....
+00000120: 004e 2901 da04 5061 7468 2901 da0c 696e  .N)...Path)...in
+00000130: 6974 5f64 6973 706c 6179 2901 da04 466f  it_display)...Fo
+00000140: 6e74 da06 6173 7365 7473 7a0d 7465 7374  nt..assetsz.test
+00000150: 5f66 6f6e 742e 706e 6729 02e9 1000 0000  _font.png)......
+00000160: 7206 0000 007a 2b31 3233 3435 3637 3839  r....z+123456789
+00000170: 302d 3d21 4023 2425 5e26 2a28 295f 2b5b  0-=!@#$%^&*()_+[
+00000180: 5d5c 3b27 2c2e 2f7b 7d7c 3a5c 223c 3e3f  ]\;',./{}|:\"<>?
+00000190: 7e60 54e9 0100 0000 e908 0000 0029 06da  ~`T..........)..
+000001a0: 0866 696c 656e 616d 65da 0a69 6d61 6765  .filename..image
+000001b0: 5f73 697a 65da 076c 6574 7465 7273 da04  _size..letters..
+000001c0: 7472 696d da04 7870 6164 da0b 7370 6163  trim..xpad..spac
+000001d0: 655f 7769 6474 687a 1363 656c 6c70 686f  e_widthz.cellpho
+000001e0: 6e65 2d62 6c61 636b 2e70 6e67 2902 e907  ne-black.png)...
+000001f0: 0000 00e9 0900 0000 7a20 2122 2324 2526  ........z !"#$%&
+00000200: 2728 292a 2b2c 2d2e 2f30 3132 3334 3536  '()*+,-./0123456
+00000210: 3738 393a 3b3c 3d3e 3f40 7a06 5b5c 5d5e  789:;<=>?@z.[\]^
+00000220: 5f60 7a04 7b7c 7d7e e9ff ffff ffe9 0400  _`z.{|}~........
+00000230: 0000 2907 7209 0000 0072 0a00 0000 720b  ..).r....r....r.
+00000240: 0000 0072 0d00 0000 da08 636f 6c6f 726b  ...r......colork
+00000250: 6579 720c 0000 0072 0e00 0000 7a13 6365  eyr....r....z.ce
+00000260: 6c6c 7068 6f6e 652d 7768 6974 652e 706e  llphone-white.pn
+00000270: 6729 0472 0900 0000 720a 0000 0072 0b00  g).r....r....r..
+00000280: 0000 7213 0000 0029 11da 0673 7472 696e  ..r....)...strin
+00000290: 67da 0770 6174 686c 6962 7202 0000 00da  g..pathlibr.....
+000002a0: 0f72 6f62 696e 6761 6d65 2e69 6d61 6765  .robingame.image
+000002b0: 7203 0000 00da 1372 6f62 696e 6761 6d65  r......robingame
+000002c0: 2e74 6578 742e 666f 6e74 7204 0000 00da  .text.fontr.....
+000002d0: 0677 696e 646f 77da 085f 5f66 696c 655f  .window..__file_
+000002e0: 5fda 0670 6172 656e 7472 0500 0000 da0f  _..parentr......
+000002f0: 6173 6369 695f 7570 7065 7263 6173 65da  ascii_uppercase.
+00000300: 0f61 7363 6969 5f6c 6f77 6572 6361 7365  .ascii_lowercase
+00000310: da09 7465 7374 5f66 6f6e 74da 0f63 656c  ..test_font..cel
+00000320: 6c70 686f 6e65 5f62 6c61 636b da0f 6365  lphone_black..ce
+00000330: 6c6c 7068 6f6e 655f 7768 6974 65da 1463  llphone_white..c
+00000340: 656c 6c70 686f 6e65 5f77 6869 7465 5f6d  ellphone_white_m
+00000350: 6f6e 6fa9 0072 2100 0000 7221 0000 00fa  ono..r!...r!....
+00000360: 322f 686f 6d65 2f72 6f62 696e 2f63 6f64  2/home/robin/cod
+00000370: 652f 726f 6269 6e67 616d 652f 726f 6269  e/robingame/robi
+00000380: 6e67 616d 652f 7465 7874 2f66 6f6e 7473  ngame/text/fonts
+00000390: 2e70 79da 083c 6d6f 6475 6c65 3e01 0000  .py..<module>...
+000003a0: 0073 8400 0000 0800 0c01 0c02 0c01 0602  .s..............
+000003b0: 0e02 0202 0601 0201 0402 0401 02ff 0202  ................
+000003c0: 02fe 0204 0201 0201 06f6 020d 0601 0201  ................
+000003d0: 0202 0401 02ff 0202 02fe 0403 02fd 0204  ................
+000003e0: 02fc 0206 0201 0201 0201 06f3 020f 0601  ................
+000003f0: 0201 0202 0401 02ff 0202 02fe 0403 02fd  ................
+00000400: 0204 02fc 0206 0201 0201 0201 06f3 020f  ................
+00000410: 0601 0201 0202 0401 02ff 0202 02fe 0403  ................
+00000420: 02fd 0204 02fc 0206 0af6                 ..........
```

### Comparing `robingame-0.1.0/robingame/text/font/font_sandbox.py` & `robingame-1.0.1/robingame/examples/font_sandbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pygame.draw
 from pygame.color import Color
 from pygame.surface import Surface
 
 from robingame.objects import Game
-from robingame.text.font import fonts
+from robingame.text import fonts
 
 snippet = """
  1space
   2space
 Ook    in 
 de     spelling 
 van    sommige andere talen wordt de umlaut gebruikt, bijvoorbeeld in verwante
```

### Comparing `robingame-0.1.0/robingame/text/font/fonts.py` & `robingame-1.0.1/robingame/text/fonts.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from robingame.image import init_display
 from robingame.text.font import Font
 
 window = init_display()
 
-assets = Path(__file__).parent.parent / "assets"
+assets = Path(__file__).parent / "assets"
 
 test_font = Font(
     filename=assets / "test_font.png",
     image_size=(16, 16),
     letters=(
         string.ascii_uppercase
         + string.ascii_lowercase
```

### Comparing `robingame-0.1.0/robingame/utils.py` & `robingame-1.0.1/robingame/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             (length - head_length, width),
             (length - head_length, -width),
             (length, 0),
         ]
     )
 
 
-def count_edges(values):
+def count_edges(values) -> tuple[int, int]:
     rising_edges = 0
     falling_edges = 0
     for ii, value in enumerate(values):
         if ii == 0:
             previous_value = value
         if value and not previous_value:
             rising_edges += 1
```

### Comparing `robingame-0.1.0/robingame.egg-info/SOURCES.txt` & `robingame-1.0.1/robingame.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 robingame/__init__.py
 robingame/animation.py
 robingame/recording.py
 robingame/sound.py
 robingame/utils.py
 robingame.egg-info/PKG-INFO
 robingame.egg-info/SOURCES.txt
 robingame.egg-info/dependency_links.txt
 robingame.egg-info/requires.txt
 robingame.egg-info/top_level.txt
 robingame/__pycache__/__init__.cpython-310.pyc
 robingame/__pycache__/animation.cpython-310.pyc
 robingame/__pycache__/utils.cpython-310.pyc
 robingame/examples/__init__.py
+robingame/examples/font_sandbox.py
+robingame/examples/hello_world.py
 robingame/examples/particle_example.py
 robingame/examples/__pycache__/__init__.cpython-310.pyc
 robingame/examples/gui_examples/__init__.py
 robingame/examples/gui_examples/coloured_button_effects.py
 robingame/examples/gui_examples/complicated_on_press_hook.py
 robingame/examples/gui_examples/on_press_event.py
 robingame/examples/gui_examples/__pycache__/__init__.cpython-310.pyc
@@ -34,18 +35,18 @@
 robingame/gui/__init__.py
 robingame/gui/button.py
 robingame/gui/menu.py
 robingame/gui/__pycache__/__init__.cpython-310.pyc
 robingame/gui/__pycache__/button.cpython-310.pyc
 robingame/gui/__pycache__/menu.cpython-310.pyc
 robingame/image/__init__.py
-robingame/image/classes.py
+robingame/image/sprite_animation.py
 robingame/image/utils.py
 robingame/image/__pycache__/__init__.cpython-310.pyc
-robingame/image/__pycache__/classes.cpython-310.pyc
+robingame/image/__pycache__/sprite_animation.cpython-310.pyc
 robingame/image/__pycache__/utils.cpython-310.pyc
 robingame/input/__init__.py
 robingame/input/event.py
 robingame/input/gamecube.py
 robingame/input/keyboard.py
 robingame/input/queue.py
 robingame/input/visualization.py
@@ -64,27 +65,24 @@
 robingame/objects/__pycache__/entity.cpython-310.pyc
 robingame/objects/__pycache__/game.cpython-310.pyc
 robingame/objects/__pycache__/group.cpython-310.pyc
 robingame/objects/__pycache__/helpers.cpython-310.pyc
 robingame/objects/__pycache__/particles.cpython-310.pyc
 robingame/text/__init__.py
 robingame/text/exceptions.py
+robingame/text/font.py
+robingame/text/fonts.py
 robingame/text/__pycache__/__init__.cpython-310.pyc
 robingame/text/__pycache__/exceptions.cpython-310.pyc
+robingame/text/__pycache__/font.cpython-310.pyc
+robingame/text/__pycache__/fonts.cpython-310.pyc
 robingame/text/assets/__init__.py
 robingame/text/assets/cellphone-black.png
 robingame/text/assets/cellphone-white.png
 robingame/text/assets/test_font.aseprite
 robingame/text/assets/test_font.png
-robingame/text/font/__init__.py
-robingame/text/font/classes.py
-robingame/text/font/font_sandbox.py
-robingame/text/font/fonts.py
-robingame/text/font/__pycache__/__init__.cpython-310.pyc
-robingame/text/font/__pycache__/classes.cpython-310.pyc
-robingame/text/font/__pycache__/fonts.cpython-310.pyc
 tests/test_animation.py
 tests/test_event.py
 tests/test_image.py
 tests/test_inputs.py
 tests/test_text.py
 tests/test_utils.py
```

### Comparing `robingame-0.1.0/tests/test_event.py` & `robingame-1.0.1/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/tests/test_image.py` & `robingame-1.0.1/tests/test_image.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from robingame.image import (
     SpriteAnimation,
     load_spritesheet,
     load_image_sequence,
     load_image,
     relative_folder,
     brighten_color,
+    flip_image,
+    utils,
 )
 
 mocks = relative_folder(__file__, "mocks")
 
 
 @pytest.mark.parametrize(
     "num_images, expected_len",
@@ -31,28 +33,28 @@
     with pytest.raises(FileNotFoundError) as e:
         load_spritesheet(filename="foo/bar.png", image_size=(1, 1))
     assert str(e.value) == "Couldn't find foo/bar.png"
 
 
 def test_load_image_sequence_not_found():
     with pytest.raises(FileNotFoundError) as e:
-        load_image_sequence(filename="foo/bar")
-    assert str(e.value) == "Couldn't find foo/bar"
+        load_image_sequence(pattern="foo/bar*.png")
+    assert str(e.value) == "Couldn't find any images matching pattern 'foo/bar*.png'"
 
 
 @pytest.mark.parametrize(
     "num_images, expected_len",
     [
         (None, 3),
         (2, 2),
     ],
 )
 def test_load_image_sequence(num_images, expected_len):
     filename = mocks / "123_series.png"
-    images = load_image_sequence(filename=filename, num_images=num_images)
+    images = load_image_sequence(pattern=mocks / "123_series*.png", num_images=num_images)
     assert len(images) == expected_len
     assert isinstance(images[0], Surface)
 
 
 def test_can_instantiate_empty_spriteanimation():
     """images=None by default and it shouldn't try to flip/recolor/scale"""
     SpriteAnimation()
@@ -63,16 +65,16 @@
     anim = SpriteAnimation.from_spritesheet(filename=filename, image_size=(64, 64))
     assert isinstance(anim, SpriteAnimation)
     assert len(anim.images) == 3
     assert isinstance(anim.images[0], Surface)
 
 
 def test_spriteanimation_from_image_sequence():
-    filename = mocks / "123_series.png"
-    anim = SpriteAnimation.from_image_sequence(filename=filename)
+    pattern = mocks / "123_series*.png"
+    anim = SpriteAnimation.from_image_sequence(pattern=pattern)
     assert isinstance(anim, SpriteAnimation)
     assert len(anim.images) == 3
     assert isinstance(anim.images[0], Surface)
 
 
 def test_spriteanimation_from_image():
     filename = mocks / "123_spritesheet.png"
@@ -225,7 +227,34 @@
     assert x == 7
     assert y == 2
     assert w == 2
     assert h == 2
 
     new = image.subsurface(image.get_bounding_rect())
     assert new.get_rect() == (0, 0, 2, 2)
+
+
+def test_scale_image():
+    image = Surface((2, 2))
+    image.fill(Color("white"))
+    image.set_at((0, 0), Color("red"))
+    new_image = utils.scale_image(image, 2)
+    assert new_image.get_size() == (4, 4)
+    assert new_image is not image  # should be a copy
+
+
+def test_flip_image():
+    image = Surface((2, 2))
+    image.fill(Color("white"))
+    image.set_at((0, 0), Color("red"))
+    new_image = utils.flip_image(image, flip_x=True, flip_y=True)
+    assert new_image.get_at((1, 1)) == Color("red")
+    assert new_image is not image  # should be a copy
+
+
+def test_recolor_image():
+    image = Surface((2, 2))
+    image.fill(Color("white"))
+    image.set_at((0, 0), Color("red"))
+    new_image = utils.recolor_image(image, color_mapping={(255, 0, 0): (0, 255, 0)})
+    assert new_image.get_at((0, 0)) == Color("green")
+    assert new_image is not image  # should be a copy
```

### Comparing `robingame-0.1.0/tests/test_inputs.py` & `robingame-1.0.1/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/tests/test_text.py` & `robingame-1.0.1/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `robingame-0.1.0/tests/test_utils.py` & `robingame-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

