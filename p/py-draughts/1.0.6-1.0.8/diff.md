# Comparing `tmp/py-draughts-1.0.6.tar.gz` & `tmp/py-draughts-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-1.0.6.tar", last modified: Sat Jul 15 07:09:42 2023, max compression
+gzip compressed data, was "py-draughts-1.0.8.tar", last modified: Sun Jul 16 08:54:30 2023, max compression
```

## Comparing `py-draughts-1.0.6.tar` & `py-draughts-1.0.8.tar`

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
+drwxrwxrwx   0        0        0        0 2023-07-16 08:54:30.763805 py-draughts-1.0.8/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 18:56:31.000000 py-draughts-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-16 08:41:45.000000 py-draughts-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     6279 2023-07-16 08:54:30.762805 py-draughts-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4859 2023-07-16 08:41:11.000000 py-draughts-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 08:54:30.731804 py-draughts-1.0.8/draughts/
+-rw-rw-rw-   0        0        0     1479 2023-07-16 08:54:18.000000 py-draughts-1.0.8/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3838 2023-07-13 18:02:36.000000 py-draughts-1.0.8/draughts/american.py
+-rw-rw-rw-   0        0        0    12250 2023-07-16 08:39:17.000000 py-draughts-1.0.8/draughts/base.py
+-rw-rw-rw-   0        0        0      671 2023-07-13 17:34:05.000000 py-draughts-1.0.8/draughts/models.py
+-rw-rw-rw-   0        0        0     4197 2023-07-13 18:10:29.000000 py-draughts-1.0.8/draughts/move.py
+-rw-rw-rw-   0        0        0     5323 2023-07-13 19:34:18.000000 py-draughts-1.0.8/draughts/server.py
+-rw-rw-rw-   0        0        0     5971 2023-07-16 08:39:17.000000 py-draughts-1.0.8/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:54:30.676290 py-draughts-1.0.8/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-16 08:54:30.733806 py-draughts-1.0.8/draughts/static/css/
+-rw-rw-rw-   0        0        0     3873 2023-07-13 16:31:38.000000 py-draughts-1.0.8/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-16 08:54:30.736807 py-draughts-1.0.8/draughts/static/js/
+-rw-rw-rw-   0        0        0     5993 2023-07-13 18:16:53.000000 py-draughts-1.0.8/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-16 08:54:30.743805 py-draughts-1.0.8/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-13 13:19:03.000000 py-draughts-1.0.8/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2860 2023-07-13 18:13:53.000000 py-draughts-1.0.8/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     2001 2023-07-16 08:39:17.000000 py-draughts-1.0.8/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:54:30.753805 py-draughts-1.0.8/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     6279 2023-07-16 08:54:30.000000 py-draughts-1.0.8/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-07-16 08:54:30.000000 py-draughts-1.0.8/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 08:54:30.000000 py-draughts-1.0.8/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-16 08:54:30.000000 py-draughts-1.0.8/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 08:54:30.000000 py-draughts-1.0.8/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 18:56:31.000000 py-draughts-1.0.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 08:54:30.763805 py-draughts-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1908 2023-07-16 08:44:01.000000 py-draughts-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:54:30.759806 py-draughts-1.0.8/test/
+-rw-rw-rw-   0        0        0     1123 2023-07-13 17:33:45.000000 py-draughts-1.0.8/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2376 2023-07-13 17:33:45.000000 py-draughts-1.0.8/test/test_board.py
```

### Comparing `py-draughts-1.0.6/LICENSE` & `py-draughts-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.6/PKG-INFO` & `py-draughts-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.0.6
+Version: 1.0.8
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
@@ -19,15 +19,15 @@
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
@@ -120,16 +120,16 @@
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

### Comparing `py-draughts-1.0.6/README.md` & `py-draughts-1.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
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
@@ -91,16 +91,16 @@
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

### Comparing `py-draughts-1.0.6/draughts/american.py` & `py-draughts-1.0.8/draughts/american.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.6/draughts/base.py` & `py-draughts-1.0.8/draughts/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -124,25 +124,30 @@
 
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
@@ -233,38 +238,54 @@
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
@@ -314,17 +335,16 @@
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

### Comparing `py-draughts-1.0.6/draughts/models.py` & `py-draughts-1.0.8/draughts/models.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.6/draughts/move.py` & `py-draughts-1.0.8/draughts/move.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.6/draughts/server.py` & `py-draughts-1.0.8/draughts/server.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.6/draughts/standard.py` & `py-draughts-1.0.8/draughts/standard.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,11 +146,10 @@
         return moves
 
 
 if __name__ == "__main__":
     board = Board()
     from pprint import pprint
 
-    Board.from_fen(
-        '[FEN "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32"]'
-    )
+    b = Board.from_fen("B:B:WG8,18,24,28,34,37,42,44,49:B2,10,12,15,25,26")
+    print(b)
     Board.from_fen("W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
```

### Comparing `py-draughts-1.0.6/draughts/static/css/style.css` & `py-draughts-1.0.8/draughts/static/css/style.css`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.6/draughts/static/js/script.js` & `py-draughts-1.0.8/draughts/static/js/script.js`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.6/draughts/templates/base.html` & `py-draughts-1.0.8/draughts/templates/base.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.6/draughts/templates/index.html` & `py-draughts-1.0.8/draughts/templates/index.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.6/draughts/utils.py` & `py-draughts-1.0.8/draughts/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Literal
 from easy_logs import get_logger
 import numpy as np
 
 logger = get_logger(lvl=10)
 
 
 def _get_all_squares_at_the_diagonal(square: int, position_length: int) -> list[int]:
```

### Comparing `py-draughts-1.0.6/py_draughts.egg-info/PKG-INFO` & `py-draughts-1.0.8/py_draughts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.0.6
+Version: 1.0.8
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
@@ -19,15 +19,15 @@
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
@@ -120,16 +120,16 @@
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

### Comparing `py-draughts-1.0.6/py_draughts.egg-info/SOURCES.txt` & `py-draughts-1.0.8/py_draughts.egg-info/SOURCES.txt`

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

### Comparing `py-draughts-1.0.6/setup.py` & `py-draughts-1.0.8/setup.py`

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

### Comparing `py-draughts-1.0.6/test/test_american_board.py` & `py-draughts-1.0.8/test/test_american_board.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.6/test/test_board.py` & `py-draughts-1.0.8/test/test_board.py`

 * *Files identical despite different names*

