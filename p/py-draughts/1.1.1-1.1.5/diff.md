# Comparing `tmp/py-draughts-1.1.1.tar.gz` & `tmp/py-draughts-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-1.1.1.tar", last modified: Sun Jul 16 18:50:13 2023, max compression
+gzip compressed data, was "py-draughts-1.1.5.tar", last modified: Sun Jul 16 20:29:20 2023, max compression
```

## Comparing `py-draughts-1.1.1.tar` & `py-draughts-1.1.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 18:50:13.498782 py-draughts-1.1.1/
--rw-rw-rw-   0        0        0    35823 2023-07-11 12:53:30.000000 py-draughts-1.1.1/LICENSE
--rw-rw-rw-   0        0        0       43 2023-07-16 09:45:04.000000 py-draughts-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5364 2023-07-16 18:50:13.497783 py-draughts-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3944 2023-07-16 18:48:02.000000 py-draughts-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 18:50:13.469775 py-draughts-1.1.1/draughts/
--rw-rw-rw-   0        0        0     1585 2023-07-16 18:50:04.000000 py-draughts-1.1.1/draughts/__init__.py
--rw-rw-rw-   0        0        0     3666 2023-07-16 18:41:37.000000 py-draughts-1.1.1/draughts/american.py
--rw-rw-rw-   0        0        0    12410 2023-07-16 18:41:54.000000 py-draughts-1.1.1/draughts/base.py
--rw-rw-rw-   0        0        0     3489 2023-07-16 18:17:38.000000 py-draughts-1.1.1/draughts/engine.py
--rw-rw-rw-   0        0        0      671 2023-07-16 18:11:48.000000 py-draughts-1.1.1/draughts/models.py
--rw-rw-rw-   0        0        0     4147 2023-07-16 18:11:26.000000 py-draughts-1.1.1/draughts/move.py
--rw-rw-rw-   0        0        0     5300 2023-07-16 18:11:04.000000 py-draughts-1.1.1/draughts/server.py
--rw-rw-rw-   0        0        0     7366 2023-07-16 18:41:03.000000 py-draughts-1.1.1/draughts/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-16 18:50:13.440779 py-draughts-1.1.1/draughts/static/
-drwxrwxrwx   0        0        0        0 2023-07-16 18:50:13.471777 py-draughts-1.1.1/draughts/static/css/
--rw-rw-rw-   0        0        0     3873 2023-07-16 09:45:04.000000 py-draughts-1.1.1/draughts/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-07-16 18:50:13.473777 py-draughts-1.1.1/draughts/static/js/
--rw-rw-rw-   0        0        0     6118 2023-07-16 09:50:41.000000 py-draughts-1.1.1/draughts/static/js/script.js
-drwxrwxrwx   0        0        0        0 2023-07-16 18:50:13.476776 py-draughts-1.1.1/draughts/templates/
--rw-rw-rw-   0        0        0     1860 2023-07-11 16:32:17.000000 py-draughts-1.1.1/draughts/templates/base.html
--rw-rw-rw-   0        0        0     2882 2023-07-16 09:45:04.000000 py-draughts-1.1.1/draughts/templates/index.html
--rw-rw-rw-   0        0        0     1973 2023-07-16 10:59:23.000000 py-draughts-1.1.1/draughts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-16 18:50:13.492776 py-draughts-1.1.1/py_draughts.egg-info/
--rw-rw-rw-   0        0        0     5364 2023-07-16 18:50:13.000000 py-draughts-1.1.1/py_draughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-07-16 18:50:13.000000 py-draughts-1.1.1/py_draughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 18:50:13.000000 py-draughts-1.1.1/py_draughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-16 18:50:13.000000 py-draughts-1.1.1/py_draughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-16 18:50:13.000000 py-draughts-1.1.1/py_draughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 17:26:06.000000 py-draughts-1.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 18:50:13.498782 py-draughts-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1908 2023-07-16 09:45:04.000000 py-draughts-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 18:50:13.496783 py-draughts-1.1.1/test/
--rw-rw-rw-   0        0        0     1104 2023-07-16 18:39:54.000000 py-draughts-1.1.1/test/test_american_board.py
--rw-rw-rw-   0        0        0     2376 2023-07-16 09:45:04.000000 py-draughts-1.1.1/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-16 20:29:20.352927 py-draughts-1.1.5/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 12:53:30.000000 py-draughts-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-16 09:45:04.000000 py-draughts-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     5226 2023-07-16 20:29:20.351925 py-draughts-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3806 2023-07-16 18:55:32.000000 py-draughts-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 20:29:20.323356 py-draughts-1.1.5/draughts/
+-rw-rw-rw-   0        0        0     1585 2023-07-16 20:29:03.000000 py-draughts-1.1.5/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3666 2023-07-16 18:41:37.000000 py-draughts-1.1.5/draughts/american.py
+-rw-rw-rw-   0        0        0    12410 2023-07-16 18:41:54.000000 py-draughts-1.1.5/draughts/base.py
+-rw-rw-rw-   0        0        0     3663 2023-07-16 18:55:10.000000 py-draughts-1.1.5/draughts/engine.py
+-rw-rw-rw-   0        0        0      671 2023-07-16 18:11:48.000000 py-draughts-1.1.5/draughts/models.py
+-rw-rw-rw-   0        0        0     4147 2023-07-16 18:11:26.000000 py-draughts-1.1.5/draughts/move.py
+-rw-rw-rw-   0        0        0     5300 2023-07-16 18:11:04.000000 py-draughts-1.1.5/draughts/server.py
+-rw-rw-rw-   0        0        0     8033 2023-07-16 20:18:47.000000 py-draughts-1.1.5/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-16 20:29:20.288272 py-draughts-1.1.5/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-16 20:29:20.324356 py-draughts-1.1.5/draughts/static/css/
+-rw-rw-rw-   0        0        0     3873 2023-07-16 09:45:04.000000 py-draughts-1.1.5/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-16 20:29:20.326356 py-draughts-1.1.5/draughts/static/js/
+-rw-rw-rw-   0        0        0     6118 2023-07-16 09:50:41.000000 py-draughts-1.1.5/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-16 20:29:20.331877 py-draughts-1.1.5/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-11 16:32:17.000000 py-draughts-1.1.5/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2882 2023-07-16 09:45:04.000000 py-draughts-1.1.5/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     1973 2023-07-16 10:59:23.000000 py-draughts-1.1.5/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 20:29:20.346408 py-draughts-1.1.5/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     5226 2023-07-16 20:29:20.000000 py-draughts-1.1.5/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-07-16 20:29:20.000000 py-draughts-1.1.5/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 20:29:20.000000 py-draughts-1.1.5/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-16 20:29:20.000000 py-draughts-1.1.5/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 20:29:20.000000 py-draughts-1.1.5/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2023-07-16 19:28:37.000000 py-draughts-1.1.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 20:29:20.352927 py-draughts-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1908 2023-07-16 09:45:04.000000 py-draughts-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 20:29:20.349926 py-draughts-1.1.5/test/
+-rw-rw-rw-   0        0        0     1104 2023-07-16 18:39:54.000000 py-draughts-1.1.5/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2376 2023-07-16 09:45:04.000000 py-draughts-1.1.5/test/test_board.py
```

### Comparing `py-draughts-1.1.1/LICENSE` & `py-draughts-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.1/PKG-INFO` & `py-draughts-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.1.1
+Version: 1.1.5
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/py-draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
@@ -149,19 +149,14 @@
 ```
 
 _It is as simple as that!_
 
 <img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/a7d67a8a-a325-437e-90b5-ba443d1b0874" width="800" />
 
 
-
-### testing best moves finding methods:
-
-[Example](https://github.com/michalskibinski109/py-draughts/blob/main/examples/engine.py)
-
 ## Contributing
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
 ## Bibliography
 
 1. [Notation](https://en.wikipedia.org/wiki/Portable_Draughts_Notation)
```

### Comparing `py-draughts-1.1.1/README.md` & `py-draughts-1.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -120,19 +120,14 @@
 ```
 
 _It is as simple as that!_
 
 <img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/a7d67a8a-a325-437e-90b5-ba443d1b0874" width="800" />
 
 
-
-### testing best moves finding methods:
-
-[Example](https://github.com/michalskibinski109/py-draughts/blob/main/examples/engine.py)
-
 ## Contributing
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
 ## Bibliography
 
 1. [Notation](https://en.wikipedia.org/wiki/Portable_Draughts_Notation)
```

### Comparing `py-draughts-1.1.1/draughts/__init__.py` & `py-draughts-1.1.5/draughts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 A draughts library with advenced (customizable) WEB UI move generation and validation,
 PDN parsing and writing. Supports multiple variants of game.
 """
 
 from typing import Literal
 
-__version__ = "1.1.1"
+__version__ = "1.1.5"
 __author__ = "Michał Skibiński"
 
 
 def get_board(variant: Literal["standard", "american"], fen: str = None):
     """
     Board factory method.
     - ``standard`` - standard draughts board
```

### Comparing `py-draughts-1.1.1/draughts/american.py` & `py-draughts-1.1.5/draughts/american.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.1/draughts/base.py` & `py-draughts-1.1.5/draughts/base.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.1/draughts/engine.py` & `py-draughts-1.1.5/draughts/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,20 +28,24 @@
     *Alpha-beta puring is a minimax algorithm with optimization. Algorithm
     will not inspect nodes that are worse than already inspected nodes.
     Additionaly, this engine will inspect capture moves first.
     Usually, those moves are better than non-capture moves.*
     """
 
     def __init__(self, depth):
+        """
+        ``depth`` - how many moves will be inspected by engine.
+        Bigger depth means better moves, but also longer calculation time.
+        """
         self.depth = depth
         self.inspected_nodes = 0
 
     def evaluate(self, board: Board):
         """
-        Evaluation function for given board.
+        Simple evaluation function for given board.
         """
         return -board._pos.sum()
 
     def get_best_move(
         self, board: Board = None, with_evaluation: bool = False
     ) -> tuple:
         self.inspected_nodes = 0
```

### Comparing `py-draughts-1.1.1/draughts/models.py` & `py-draughts-1.1.5/draughts/models.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.1/draughts/move.py` & `py-draughts-1.1.5/draughts/move.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.1/draughts/server.py` & `py-draughts-1.1.5/draughts/server.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.1/draughts/standard.py` & `py-draughts-1.1.5/draughts/standard.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,34 +24,36 @@
             A1, C1, E1, G1, I1] = range(50)
 # fmt: on
 
 
 class Board(BaseBoard):
     """
     **Board for Standard (international) checkers.**
-     Game rules:
 
-     - Board size: 10x10
-     - Any piece can capture backwards and forwards
-     - Capture is mandatory
-     - King can move along the diagonal any number of squares
-
-     **Winning and drawing**
-     - A player wins the game when the opponent no longer has any valid moves.
-        This can be either because all of the player's pieces have been captured,
-        or because they are all blocked and thus have no more squares available.
-     - If the same position appears on the board for the third time,
-        with the same side to move, the game is considered drawn by threefold repetition.
-     - The game is drawn when both players make 25 consecutive king moves without capturing.
-        When one player has only a king left, and the other player three pieces including at least
-        one king (three kings, two kings and a man, or one king and two men),
-        the game is drawn after both players made 16 moves.
-     - When one player has only a king left, and the other player two pieces
-        or less including at least one king (one king, two kings, or one king and a man),
-        the game is drawn after both players made 5 moves.
+    Game rules:
+
+    - Board size: 10x10
+    - Any piece can capture backwards and forwards
+    - Capture is mandatory
+    - King can move along the diagonal any number of squares
+
+    **Winning and drawing**
+
+    - A player wins the game when the opponent no longer has any valid moves.
+    This can be either because all of the player's pieces have been captured,
+    or because they are all blocked and thus have no more squares available.
+    - If the same position appears on the board for the third time,
+    with the same side to move, the game is considered drawn by threefold repetition.
+    - The game is drawn when both players make 25 consecutive king moves without capturing.
+    When one player has only a king left, and the other player three pieces including at least
+    one king (three kings, two kings and a man, or one king and two men),
+    the game is drawn after both players made 16 moves.
+    - When one player has only a king left, and the other player two pieces
+    or less including at least one king (one king, two kings, or one king and a man),
+    the game is drawn after both players made 5 moves.
 
     """
 
     GAME_TYPE = 20
     STARTING_POSITION = np.array([1] * 15 + [0] * 20 + [-1] * 15, dtype=np.int8)
     PSEUDO_LEGAL_KING_MOVES = get_king_pseudo_legal_moves(len(STARTING_POSITION))
     PSEUDO_LEGAL_MAN_MOVES = get_man_pseudo_legal_moves(len(STARTING_POSITION))
@@ -61,30 +63,53 @@
     def __init__(self, starting_position=STARTING_POSITION) -> None:
         super().__init__(starting_position)
 
     @property
     def is_draw(self) -> bool:
         return (
             self.is_threefold_repetition
+            or self.is_5_moves_rule
+            or self.is_16_moves_rule
             or self.is_25_moves_rule
-            # or self.is_16_moves_rule # TODO  to be implemented
-            # or self.is_5_moves_rule  # TODO to be implemented
         )
 
     @property
     def is_25_moves_rule(self) -> bool:
         if len(self._moves_stack) < 25:
             return False
         for move in self._moves_stack[-25:]:
             if move.captured_list:
                 return False
         logger.debug("25 moves rule")
         return True
 
     @property
+    def is_16_moves_rule(self) -> bool:
+        if len(self._moves_stack) < 16:
+            return False
+        for move in self._moves_stack[-16:]:
+            if move.captured_list or move.is_promotion:
+                return False
+        logger.debug("16 moves rule")
+        return True
+
+    @property
+    def is_5_moves_rule(self) -> bool:
+        # if count of pieces is not 3 or 4
+        if len(self._pos[self._pos != Figure.EMPTY]) > 4:
+            return False
+        if len(self._moves_stack) < 5:
+            return False
+        for move in self._moves_stack[-5:]:
+            if move.captured_list or move.is_promotion:
+                return False
+        logger.debug("5 moves rule")
+        return True
+
+    @property
     def legal_moves(self) -> list[Move]:
         all_moves = []
         is_capture_mandatory = False
         squares_list = np.transpose(np.nonzero(self._pos * self.turn.value > 0))
         for square in squares_list.flatten():
             moves = self._legal_moves_from(square, is_capture_mandatory)
             # if not is_capture_mandatory and any( # TODO this should optimize the search
```

### Comparing `py-draughts-1.1.1/draughts/static/css/style.css` & `py-draughts-1.1.5/draughts/static/css/style.css`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.1/draughts/static/js/script.js` & `py-draughts-1.1.5/draughts/static/js/script.js`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.1/draughts/templates/base.html` & `py-draughts-1.1.5/draughts/templates/base.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.1/draughts/templates/index.html` & `py-draughts-1.1.5/draughts/templates/index.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.1/draughts/utils.py` & `py-draughts-1.1.5/draughts/utils.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.1/py_draughts.egg-info/PKG-INFO` & `py-draughts-1.1.5/py_draughts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.1.1
+Version: 1.1.5
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/py-draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
@@ -149,19 +149,14 @@
 ```
 
 _It is as simple as that!_
 
 <img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/a7d67a8a-a325-437e-90b5-ba443d1b0874" width="800" />
 
 
-
-### testing best moves finding methods:
-
-[Example](https://github.com/michalskibinski109/py-draughts/blob/main/examples/engine.py)
-
 ## Contributing
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
 ## Bibliography
 
 1. [Notation](https://en.wikipedia.org/wiki/Portable_Draughts_Notation)
```

### Comparing `py-draughts-1.1.1/py_draughts.egg-info/SOURCES.txt` & `py-draughts-1.1.5/py_draughts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.1/setup.py` & `py-draughts-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.1/test/test_american_board.py` & `py-draughts-1.1.5/test/test_american_board.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.1/test/test_board.py` & `py-draughts-1.1.5/test/test_board.py`

 * *Files identical despite different names*

