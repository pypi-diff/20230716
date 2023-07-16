# Comparing `tmp/py-draughts-1.0.6.tar.gz` & `tmp/py-draughts-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-1.0.6.tar", last modified: Sat Jul 15 07:09:42 2023, max compression
+gzip compressed data, was "py-draughts-1.1.0.tar", last modified: Sun Jul 16 11:01:45 2023, max compression
```

## Comparing `py-draughts-1.0.6.tar` & `py-draughts-1.1.0.tar`

### file list

```diff
@@ -1,36 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.866606 py-draughts-1.0.6/
--rw-rw-rw-   0        0        0    35823 2023-07-13 22:43:03.000000 py-draughts-1.0.6/LICENSE
--rw-rw-rw-   0        0        0       43 2023-07-13 22:43:03.000000 py-draughts-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     6258 2023-07-15 07:09:42.866606 py-draughts-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4841 2023-07-13 22:43:03.000000 py-draughts-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.754490 py-draughts-1.0.6/draughts/
--rw-rw-rw-   0        0        0      964 2023-07-15 07:09:12.000000 py-draughts-1.0.6/draughts/__init__.py
--rw-rw-rw-   0        0        0     3838 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/american.py
--rw-rw-rw-   0        0        0    11486 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/base.py
--rw-rw-rw-   0        0        0      671 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/models.py
--rw-rw-rw-   0        0        0     4197 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/move.py
--rw-rw-rw-   0        0        0     5323 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/server.py
--rw-rw-rw-   0        0        0     5989 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.653457 py-draughts-1.0.6/draughts/static/
-drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.762530 py-draughts-1.0.6/draughts/static/css/
--rw-rw-rw-   0        0        0     3873 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.777042 py-draughts-1.0.6/draughts/static/img/
--rw-rw-rw-   0        0        0     1386 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/static/img/crown-icon.svg
-drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.786608 py-draughts-1.0.6/draughts/static/js/
--rw-rw-rw-   0        0        0     5993 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/static/js/script.js
-drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.810607 py-draughts-1.0.6/draughts/templates/
--rw-rw-rw-   0        0        0     1860 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/templates/base.html
--rw-rw-rw-   0        0        0     2860 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/templates/index.html
--rw-rw-rw-   0        0        0     1973 2023-07-13 22:43:03.000000 py-draughts-1.0.6/draughts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.842609 py-draughts-1.0.6/py_draughts.egg-info/
--rw-rw-rw-   0        0        0     6258 2023-07-15 07:09:42.000000 py-draughts-1.0.6/py_draughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2023-07-15 07:09:42.000000 py-draughts-1.0.6/py_draughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 07:09:42.000000 py-draughts-1.0.6/py_draughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-15 07:09:42.000000 py-draughts-1.0.6/py_draughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-15 07:09:42.000000 py-draughts-1.0.6/py_draughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 22:43:03.000000 py-draughts-1.0.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 07:09:42.866606 py-draughts-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2001 2023-07-15 07:08:11.000000 py-draughts-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 07:09:42.866606 py-draughts-1.0.6/test/
--rw-rw-rw-   0        0        0     1123 2023-07-13 22:43:03.000000 py-draughts-1.0.6/test/test_american_board.py
--rw-rw-rw-   0        0        0     2376 2023-07-13 22:43:03.000000 py-draughts-1.0.6/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:01:45.754629 py-draughts-1.1.0/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 12:53:30.000000 py-draughts-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-16 09:45:04.000000 py-draughts-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6410 2023-07-16 11:01:45.753631 py-draughts-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4990 2023-07-16 11:00:54.000000 py-draughts-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 11:01:45.731631 py-draughts-1.1.0/draughts/
+-rw-rw-rw-   0        0        0     1585 2023-07-16 11:01:19.000000 py-draughts-1.1.0/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3803 2023-07-16 10:59:23.000000 py-draughts-1.1.0/draughts/american.py
+-rw-rw-rw-   0        0        0    12281 2023-07-16 10:59:05.000000 py-draughts-1.1.0/draughts/base.py
+-rw-rw-rw-   0        0        0      671 2023-07-16 09:45:04.000000 py-draughts-1.1.0/draughts/models.py
+-rw-rw-rw-   0        0        0     4150 2023-07-16 11:00:50.000000 py-draughts-1.1.0/draughts/move.py
+-rw-rw-rw-   0        0        0     5310 2023-07-16 10:59:19.000000 py-draughts-1.1.0/draughts/server.py
+-rw-rw-rw-   0        0        0     5635 2023-07-16 11:00:50.000000 py-draughts-1.1.0/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:01:45.692888 py-draughts-1.1.0/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-16 11:01:45.732630 py-draughts-1.1.0/draughts/static/css/
+-rw-rw-rw-   0        0        0     3873 2023-07-16 09:45:04.000000 py-draughts-1.1.0/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-16 11:01:45.734632 py-draughts-1.1.0/draughts/static/js/
+-rw-rw-rw-   0        0        0     6118 2023-07-16 09:50:41.000000 py-draughts-1.1.0/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-16 11:01:45.737630 py-draughts-1.1.0/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-11 16:32:17.000000 py-draughts-1.1.0/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2882 2023-07-16 09:45:04.000000 py-draughts-1.1.0/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     1973 2023-07-16 10:59:23.000000 py-draughts-1.1.0/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:01:45.749628 py-draughts-1.1.0/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     6410 2023-07-16 11:01:45.000000 py-draughts-1.1.0/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-07-16 11:01:45.000000 py-draughts-1.1.0/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 11:01:45.000000 py-draughts-1.1.0/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-16 11:01:45.000000 py-draughts-1.1.0/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 11:01:45.000000 py-draughts-1.1.0/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 17:26:06.000000 py-draughts-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 11:01:45.754629 py-draughts-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1908 2023-07-16 09:45:04.000000 py-draughts-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:01:45.752631 py-draughts-1.1.0/test/
+-rw-rw-rw-   0        0        0     1123 2023-07-16 10:55:42.000000 py-draughts-1.1.0/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2376 2023-07-16 09:45:04.000000 py-draughts-1.1.0/test/test_board.py
```

### Comparing `py-draughts-1.0.6/LICENSE` & `py-draughts-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.6/PKG-INFO` & `py-draughts-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.0.6
+Version: 1.1.0
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
-Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
+Project-URL: Documentation, https://michalskibinski109.github.io/py-draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -19,23 +19,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py-draughts
 
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/py-draughts)
+[![Downloads](https://static.pepy.tech/personalized-badge/py-draughts?period=month&units=none&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/py-draughts)
 
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
 ## Installation
 
@@ -57,16 +57,16 @@
 ## Usage
 
 
 
 #### Displays simple ascii board
 
 ```python
->>> from draughts.standard import Board
->>> board = Board()
+>>> from draughts import get_board
+>>> board = get_board("standard")
 Board initialized with shape (10, 10). (base.py:108)
 >>> board
  . b . b . b . b . b
  b . b . b . b . b .
  . b . b . b . b . b
  . . . . . . . . . .
  . . . . . . . . . .
@@ -111,25 +111,25 @@
 [Move: 36->31, Move: 37->32, Move: 37->31, Move: 38->33, Move: 38->32, Move: 39->34, Move: 39->33, Move: 40->35, Move: 40->34]
 ```
 
 #### Generate fen string and load board from fen string
 
 
 ```python
->>> board =Board.from_fen("W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
+>>> board =get_board('standard', "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
 Board initialized with shape (10, 10). (base.py:109)
 >>> board.push_from_str("28-37")
 >>> board.fen
 '[FEN "B:W4,11,31,K33,K34,37,38,40,K41,43,K44,45,K46,47:BK3,21,27"]'
 ```
 #### American checkers
 
 ```python
->>> from draughts.american import Board
->>> board = Board()
+>>> from draughts import get_board
+>>> board = get_board("american")
 Board initialized with shape (8, 8). (base.py:108)
 >>> board
  . b . b . b . b
  b . b . b . b .
  . b . b . b . b
  . . . . . . . .
  . . . . . . . .
```

### Comparing `py-draughts-1.0.6/README.md` & `py-draughts-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # py-draughts
 
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/py-draughts)
+[![Downloads](https://static.pepy.tech/personalized-badge/py-draughts?period=month&units=none&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/py-draughts)
 
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
 ## Installation
 
@@ -28,16 +28,16 @@
 ## Usage
 
 
 
 #### Displays simple ascii board
 
 ```python
->>> from draughts.standard import Board
->>> board = Board()
+>>> from draughts import get_board
+>>> board = get_board("standard")
 Board initialized with shape (10, 10). (base.py:108)
 >>> board
  . b . b . b . b . b
  b . b . b . b . b .
  . b . b . b . b . b
  . . . . . . . . . .
  . . . . . . . . . .
@@ -82,25 +82,25 @@
 [Move: 36->31, Move: 37->32, Move: 37->31, Move: 38->33, Move: 38->32, Move: 39->34, Move: 39->33, Move: 40->35, Move: 40->34]
 ```
 
 #### Generate fen string and load board from fen string
 
 
 ```python
->>> board =Board.from_fen("W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
+>>> board =get_board('standard', "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
 Board initialized with shape (10, 10). (base.py:109)
 >>> board.push_from_str("28-37")
 >>> board.fen
 '[FEN "B:W4,11,31,K33,K34,37,38,40,K41,43,K44,45,K46,47:BK3,21,27"]'
 ```
 #### American checkers
 
 ```python
->>> from draughts.american import Board
->>> board = Board()
+>>> from draughts import get_board
+>>> board = get_board("american")
 Board initialized with shape (8, 8). (base.py:108)
 >>> board
  . b . b . b . b
  b . b . b . b .
  . b . b . b . b
  . . . . . . . .
  . . . . . . . .
```

### Comparing `py-draughts-1.0.6/draughts/american.py` & `py-draughts-1.1.0/draughts/american.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 from typing import Generator
 
 import numpy as np
+
 from draughts.base import BaseBoard
 from draughts.models import Color, Figure
 from draughts.move import Move
-from draughts.utils import logger
-
 
 # fmt: off
 SQUARES = [B8, D8, F8, H8,
         A7, C7, E7, G7,
         B6, D6, F6, H6,
         A5, C5, E5, G5,
         B4, D4, F4, H4,
```

### Comparing `py-draughts-1.0.6/draughts/base.py` & `py-draughts-1.1.0/draughts/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 # documentation in rst format
 """
 
 """
 
 from __future__ import annotations
 
+import re
 from abc import ABC
 from typing import Generator
-from collections import defaultdict
+
 import numpy as np
-import re
 
 from draughts.models import ENTITY_REPR, Color, Figure, SquareT
 from draughts.move import Move
-from draughts.utils import (
-    logger,
-    get_king_pseudo_legal_moves,
-    get_man_pseudo_legal_moves,
-)
+from draughts.utils import logger
 
 # fmt: off
 SQUARES = [_, B8, D8, F8, H8,
         A7, C7, E7, G7,
         B6, D6, F6, H6,
         A5, C5, E5, G5,
         B4, D4, F4, H4,
@@ -62,14 +58,16 @@
 
     GAME_TYPE = -1
     """
     PDN game type. See `PDN specification <https://en.wikipedia.org/wiki/Portable_Draughts_Notation>`_.
     """
     VARIANT_NAME = "Abstract variant"
     STARTING_POSITION = np.array([1] * 12 + [0] * 8 + [-1] * 12, dtype=np.int8)
+    row_idx = {val: val // 5 for val in range(len(STARTING_POSITION))}
+    col_idx = {val: val % 10 for val in range(len(STARTING_POSITION))}
     STARTING_COLOR = Color.WHITE
     """
     Starting color. ``Color.WHITE`` or ``Color.BLACK``.
     """
 
     PSEUDO_LEGAL_KING_MOVES = None
     """
@@ -124,25 +122,30 @@
 
     @property
     def position(self) -> np.ndarray:
         """Returns board position."""
         return self._pos
 
     @property
-    def game_over(self) -> bool:
-        """Returns ``True`` if the game is over."""
-        # check if threefold repetition
-        if len(self._moves_stack) >= 8:
+    def is_threefold_repetition(self) -> bool:
+        if len(self._moves_stack) >= 9:
             if (
                 self._moves_stack[-1].square_list
                 == self._moves_stack[-5].square_list
                 == self._moves_stack[-9].square_list
             ):
                 return True
-        return not bool(list(self.legal_moves))
+        return False
+
+    @property
+    def game_over(self) -> bool:
+        """Returns ``True`` if the game is over."""
+        # check if threefold repetition
+
+        return self.is_threefold_repetition or not bool(list(self.legal_moves))
 
     def push(self, move: Move, is_finished: bool = True) -> None:
         """Pushes a move to the board.
         Automatically promotes a piece if it reaches the last row.
 
         If ``is_finished`` is set to ``True``, the turn is switched. This parameter is used only
         for generating legal moves.
@@ -233,38 +236,54 @@
     @classmethod
     def from_fen(cls, fen: str) -> BaseBoard:
         """
         Creates a board from a FEN string by using regular expressions.
         """
         fen = fen.upper()
         re_turn = re.compile(r"[WB]:")
+        re_premove = re.compile(r"(G[0-9]+|P[0-9]+)(,|)")
+        re_prefix = re.compile(r"[WB]:[WB]:[WB]:")
         re_white = re.compile(r"W[0-9K,]+")
         re_black = re.compile(r"B[0-9K,]+")
-        turn = re_turn.search(fen).group(0)[0]
-        white = re_white.search(fen).group(0).replace("W", "")
-        black = re_black.search(fen).group(0).replace("B", "")
+        # remove premoves from fen
+        # remove first 2 letters from prefix
+        fen = re_premove.sub("", fen)
+        prefix = re_prefix.search(fen)
+        if prefix:
+            prefix = prefix.group(0)
+            fen = fen.replace(prefix, prefix[2:])
+        try:
+            turn = re_turn.search(fen).group(0)[0]
+            white = re_white.search(fen).group(0).replace("W", "")
+            black = re_black.search(fen).group(0).replace("B", "")
+        except AttributeError as e:
+            raise AttributeError(f"Invalid FEN: {fen} \n {e}")
+        logger.debug(f"turn: {turn}, white: {white}, black: {black}")
         cls.STARTING_POSITION = np.zeros(cls.STARTING_POSITION.shape, dtype=np.int8)
         if len(turn) != 1 or (len(white) == 0 and len(black) == 0):
-            raise ValueError(f"Wrong FEN: {fen}")
-        cls.__populate_from_list(white.split(","), Color.WHITE)
-        cls.__populate_from_list(black.split(","), Color.BLACK)
+            raise ValueError(f"Invalid FEN: {fen}")
+        try:
+            cls.__populate_from_list(white.split(","), Color.WHITE)
+            cls.__populate_from_list(black.split(","), Color.BLACK)
+        except ValueError as e:
+            logger.error(f"Invalid FEN: {fen} \n {e}")
         cls.turn = Color.WHITE if turn == "W" else Color.BLACK
         return cls(starting_position=cls.STARTING_POSITION)
 
     @classmethod
     def __populate_from_list(cls, fen_list: list[str], color: Color) -> None:
         board_range = range(1, cls.STARTING_POSITION.shape[0] + 1)
         for sq in fen_list:
             if sq.isdigit() and int(sq) in board_range:
                 cls.STARTING_POSITION[int(sq) - 1] = color.value
             elif sq.startswith("K") and sq[1:].isdigit() and int(sq[1:]) in board_range:
                 cls.STARTING_POSITION[int(sq[1:]) - 1] = color.value * Figure.KING.value
             else:
                 raise ValueError(
-                    f"Wrong FEN: invalid square value: {sq} for board with length\
+                    f"invalid square value: {sq} for board with length\
                         {cls.STARTING_POSITION.shape[0]}"
                 )
 
     @classmethod
     @property
     def info(cls) -> str:
         board_size = int(np.sqrt(cls.STARTING_POSITION.shape[0]))
@@ -314,17 +333,16 @@
     def __getitem__(self, key: SquareT) -> Figure:
         return self.position[key]
 
 
 if __name__ == "__main__":
     # board = BaseBoard(BaseBoard.STARTING_POSITION)
     # print(board)
-    BaseBoard.from_fen(
-        '[FEN "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32"]'
-    )
+    board = BaseBoard.from_fen("W:W:WG23:BP12,K19,K28")
+    print(board)
     BaseBoard.from_fen("W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
 
 # print(board.info)
 #     m1 = Move([C3, B4])
 #     board.push(m1)
 
 #     m2 = Move([B6, A5])
```

### Comparing `py-draughts-1.0.6/draughts/models.py` & `py-draughts-1.1.0/draughts/models.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.6/draughts/move.py` & `py-draughts-1.1.0/draughts/move.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 
-from typing import Generator, NewType
+from typing import Generator
 
-import numpy as np
-
-from draughts.models import Color, Figure, SquareT
+from draughts.models import Figure
 
 
 class Move:
     """Move representation.
     End user should never interact with this class directly.
 
     As we can read on wikipedia:
```

### Comparing `py-draughts-1.0.6/draughts/server.py` & `py-draughts-1.1.0/draughts/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+import json
+from collections import defaultdict
+from pathlib import Path
+from typing import Literal
+
 import numpy as np
 import uvicorn
-from fastapi import FastAPI, Request, APIRouter, BackgroundTasks
+from fastapi import APIRouter, FastAPI, Request
 from fastapi.responses import RedirectResponse
-import json
 from fastapi.staticfiles import StaticFiles
 from fastapi.templating import Jinja2Templates
+from pydantic import BaseModel, Field
+
 from draughts import __version__
 from draughts.base import BaseBoard, Color
-from typing import Literal
-from collections import defaultdict
-from pathlib import Path
-from pydantic import BaseModel, Field
 from draughts.standard import Board
 
 
 class PositionResponse(BaseModel):
     position: list = Field(description="Current board position")
     history: list = Field(description="History of moves")
     turn: Literal["white", "black"] = Field(description="Current turn")
```

### Comparing `py-draughts-1.0.6/draughts/standard.py` & `py-draughts-1.1.0/draughts/standard.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,16 @@
 from __future__ import annotations
 
-"""
-**Board for Standard (international) checkers.**
-*Still in development.*
-"""
-
-from typing import Generator
-
 import numpy as np
-from collections import defaultdict
+
 from draughts.base import BaseBoard
-from draughts.models import Color, Figure
+from draughts.models import Figure
 from draughts.move import Move
-from draughts.utils import (
-    logger,
-    get_king_pseudo_legal_moves,
-    get_man_pseudo_legal_moves,
-)
-
+from draughts.utils import (get_king_pseudo_legal_moves,
+                            get_man_pseudo_legal_moves)
 
 # fmt: off
 SQUARES=  [ B10, D10, F10, H10, J10,
             A9, C9, E9, G9, I9,
             B8, D8, F8, H8, J8, 
             A7, C7, E7, G7, I7,
             B6, D6, F6, H6, J6,
@@ -42,16 +31,14 @@
      - Any piece can capture backwards and forwards
      - Capture is mandatory
      - King can move along the diagonal any number of squares
     """
 
     GAME_TYPE = 20
     STARTING_POSITION = np.array([1] * 15 + [0] * 20 + [-1] * 15, dtype=np.int8)
-    row_idx = {val: val // 5 for val in range(len(STARTING_POSITION))}
-    col_idx = {val: val % 10 for val in range(len(STARTING_POSITION))}
     PSEUDO_LEGAL_KING_MOVES = get_king_pseudo_legal_moves(len(STARTING_POSITION))
     PSEUDO_LEGAL_MAN_MOVES = get_man_pseudo_legal_moves(len(STARTING_POSITION))
 
     def __init__(self, starting_position=STARTING_POSITION) -> None:
         super().__init__(starting_position)
 
     @property
@@ -144,13 +131,11 @@
         if is_capture_mandatory:
             moves = [move for move in moves if len(move.captured_list) > 0]
         return moves
 
 
 if __name__ == "__main__":
     board = Board()
-    from pprint import pprint
 
-    Board.from_fen(
-        '[FEN "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32"]'
-    )
+    b = Board.from_fen("B:B:WG8,18,24,28,34,37,42,44,49:B2,10,12,15,25,26")
+    print(b)
     Board.from_fen("W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
```

### Comparing `py-draughts-1.0.6/draughts/static/css/style.css` & `py-draughts-1.1.0/draughts/static/css/style.css`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.6/draughts/static/js/script.js` & `py-draughts-1.1.0/draughts/static/js/script.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -148,14 +148,20 @@
             if (tiles[i].innerText - 1 == element) {
                 $(tiles[i]).addClass("higlight");
             }
         }
     });
 };
 
+async function autoPlay() {
+    setInterval(() => {
+        makeBestMove();
+    }, 700);
+}
+
 const updatehistory = () => {
     let tbody = $("#historyTableBody");
     tbody.empty();
     if (!historyData) return;
     for (let i = 0; i < historyData.length; i++) {
         if (!historyData[i][2]) historyData[i][2] = "-";
         tbody.append(
@@ -213,8 +219,9 @@
     boardArray = await getPosition();
     init(boardArray);
     upadateBoard();
     $("#makeMove").click(makeBestMove);
     $("#popBtn").click(pop);
     $("#randomPos").click(getRandomPos);
     $("#copyFen").click(getFen);
+    $("#autoPlay").click(autoPlay);
 });
```

### Comparing `py-draughts-1.0.6/draughts/templates/base.html` & `py-draughts-1.1.0/draughts/templates/base.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.6/draughts/templates/index.html` & `py-draughts-1.1.0/draughts/templates/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -24,25 +24,26 @@
         <!-- game settings -->
         <hr class="col-12 bg-secondary" />
         <div class="col-12">
           <p class="display-6">Game control</p>
         </div>
         <button id="makeMove" class="col-12 btn btn-custom mt-3">
           Make engine move
-          <hr />
-          <code>Calls method provided on server `__init__`</code>
         </button>
 
         <button id="popBtn" class="col-12 btn btn-custom mt-3">Undo</button>
         <button id="randomPos" class="col-12 btn btn-custom mt-3">
           Set random position
         </button>
         <button id="copyFen" class="col-12 btn btn-custom mt-3">
           Copy FEN <small>to clipboard</small>
         </button>
+        <button id="autoPlay" class="col-12 btn btn-custom mt-3">
+          Auto play
+        </button>
       </div>
     </div>
     <div class="col-6 h-100">
       <div
         id="board"
         class="board"
         crown_icon="{{ url_for('static', path='img/crown-icon.svg') }}"
```

#### html2text {}

```diff
@@ -2,18 +2,16 @@
 ****** Settings ******
 
 ===============================================================================
 Game type
 American_(8x8) Standard_(10x10) Your_own_board_._._.
 ===============================================================================
 Game control
- Make engine move
-===============================================================================
-Calls method provided on server `__init__`  Undo  Set random position   Copy
-FEN to clipboard
+ Make engine move  Undo  Set random position   Copy FEN to clipboard   Auto
+play
 {% for i in range(size) %}
 {% endfor %}
 ****** Game info ******
 ===============================================================================
 Turn: White
 Move history
 Nr White Black
```

### Comparing `py-draughts-1.0.6/draughts/utils.py` & `py-draughts-1.1.0/draughts/utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from easy_logs import get_logger
 import numpy as np
+from easy_logs import get_logger
 
 logger = get_logger(lvl=10)
 
 
 def _get_all_squares_at_the_diagonal(square: int, position_length: int) -> list[int]:
     """
     [[up-right],  [up-left],[down-right], [down-left]]
```

### Comparing `py-draughts-1.0.6/py_draughts.egg-info/PKG-INFO` & `py-draughts-1.1.0/py_draughts.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.0.6
+Version: 1.1.0
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
-Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
+Project-URL: Documentation, https://michalskibinski109.github.io/py-draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -19,23 +19,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py-draughts
 
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/py-draughts)
+[![Downloads](https://static.pepy.tech/personalized-badge/py-draughts?period=month&units=none&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/py-draughts)
 
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
 ## Installation
 
@@ -57,16 +57,16 @@
 ## Usage
 
 
 
 #### Displays simple ascii board
 
 ```python
->>> from draughts.standard import Board
->>> board = Board()
+>>> from draughts import get_board
+>>> board = get_board("standard")
 Board initialized with shape (10, 10). (base.py:108)
 >>> board
  . b . b . b . b . b
  b . b . b . b . b .
  . b . b . b . b . b
  . . . . . . . . . .
  . . . . . . . . . .
@@ -111,25 +111,25 @@
 [Move: 36->31, Move: 37->32, Move: 37->31, Move: 38->33, Move: 38->32, Move: 39->34, Move: 39->33, Move: 40->35, Move: 40->34]
 ```
 
 #### Generate fen string and load board from fen string
 
 
 ```python
->>> board =Board.from_fen("W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
+>>> board =get_board('standard', "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
 Board initialized with shape (10, 10). (base.py:109)
 >>> board.push_from_str("28-37")
 >>> board.fen
 '[FEN "B:W4,11,31,K33,K34,37,38,40,K41,43,K44,45,K46,47:BK3,21,27"]'
 ```
 #### American checkers
 
 ```python
->>> from draughts.american import Board
->>> board = Board()
+>>> from draughts import get_board
+>>> board = get_board("american")
 Board initialized with shape (8, 8). (base.py:108)
 >>> board
  . b . b . b . b
  b . b . b . b .
  . b . b . b . b
  . . . . . . . .
  . . . . . . . .
```

### Comparing `py-draughts-1.0.6/py_draughts.egg-info/SOURCES.txt` & `py-draughts-1.1.0/py_draughts.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 draughts/base.py
 draughts/models.py
 draughts/move.py
 draughts/server.py
 draughts/standard.py
 draughts/utils.py
 draughts/static/css/style.css
-draughts/static/img/crown-icon.svg
 draughts/static/js/script.js
 draughts/templates/base.html
 draughts/templates/index.html
 py_draughts.egg-info/PKG-INFO
 py_draughts.egg-info/SOURCES.txt
 py_draughts.egg-info/dependency_links.txt
 py_draughts.egg-info/requires.txt
```

### Comparing `py-draughts-1.0.6/setup.py` & `py-draughts-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,31 +9,24 @@
 
 with open(this_directory / "requirements.txt") as f:
     requirements = f.read().splitlines()
 
 
 setuptools.setup(
     name="py-draughts",
+    install_requires=requirements,
     version=__version__,
     author="Michał Skibiński",
     author_email="mskibinski109@gmail.com",
     description=__doc__.replace("\n", " ").strip(),
     long_description=long_description,
     # rst
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
-    package_data={
-        "draughts": [
-            "static/js/*",
-            "static/css/*",
-            "templates/*",
-            "static/img/*",
-        ]
-    },
-    install_requires=requirements,
+    package_data={"draughts": ["static/js/*", "static/css/*", "templates/*"]},
     license="GPL-3.0+",
     keywords=" draughts, checkers, AI mini-max, game, board",
     url="https://github.com/michalskibinski109/draughts",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
@@ -47,11 +40,11 @@
         "Programming Language :: Python :: 3.11",
         "Topic :: Games/Entertainment :: Board Games",
         "Topic :: Games/Entertainment :: Turn Based Strategy",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Typing :: Typed",
     ],
     project_urls={
-        "Documentation": "https://michalskibinski109.github.io/draughts/index.html",
+        "Documentation": "https://michalskibinski109.github.io/py-draughts/index.html",
     },
-    python_requires=">=3.8",
+    python_requires=">=3.7",
 )
```

### Comparing `py-draughts-1.0.6/test/test_american_board.py` & `py-draughts-1.1.0/test/test_american_board.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pytest
 
 import draughts.american as checkers
-from draughts.american import Board, Move, Color
+from draughts.american import Board, Color, Move
 from draughts.models import Figure
 
 
 class TestAmericanBoard:
     @pytest.fixture(autouse=True)
     def setup(self):
         self.board = Board()
```

### Comparing `py-draughts-1.0.6/test/test_board.py` & `py-draughts-1.1.0/test/test_board.py`

 * *Files identical despite different names*

