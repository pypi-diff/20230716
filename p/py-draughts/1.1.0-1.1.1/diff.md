# Comparing `tmp/py-draughts-1.1.0.tar.gz` & `tmp/py-draughts-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-1.1.0.tar", last modified: Sun Jul 16 11:01:45 2023, max compression
+gzip compressed data, was "py-draughts-1.1.1.tar", last modified: Sun Jul 16 18:50:13 2023, max compression
```

## Comparing `py-draughts-1.1.0.tar` & `py-draughts-1.1.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 11:01:45.754629 py-draughts-1.1.0/
--rw-rw-rw-   0        0        0    35823 2023-07-11 12:53:30.000000 py-draughts-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       43 2023-07-16 09:45:04.000000 py-draughts-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6410 2023-07-16 11:01:45.753631 py-draughts-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4990 2023-07-16 11:00:54.000000 py-draughts-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 11:01:45.731631 py-draughts-1.1.0/draughts/
--rw-rw-rw-   0        0        0     1585 2023-07-16 11:01:19.000000 py-draughts-1.1.0/draughts/__init__.py
--rw-rw-rw-   0        0        0     3803 2023-07-16 10:59:23.000000 py-draughts-1.1.0/draughts/american.py
--rw-rw-rw-   0        0        0    12281 2023-07-16 10:59:05.000000 py-draughts-1.1.0/draughts/base.py
--rw-rw-rw-   0        0        0      671 2023-07-16 09:45:04.000000 py-draughts-1.1.0/draughts/models.py
--rw-rw-rw-   0        0        0     4150 2023-07-16 11:00:50.000000 py-draughts-1.1.0/draughts/move.py
--rw-rw-rw-   0        0        0     5310 2023-07-16 10:59:19.000000 py-draughts-1.1.0/draughts/server.py
--rw-rw-rw-   0        0        0     5635 2023-07-16 11:00:50.000000 py-draughts-1.1.0/draughts/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-16 11:01:45.692888 py-draughts-1.1.0/draughts/static/
-drwxrwxrwx   0        0        0        0 2023-07-16 11:01:45.732630 py-draughts-1.1.0/draughts/static/css/
--rw-rw-rw-   0        0        0     3873 2023-07-16 09:45:04.000000 py-draughts-1.1.0/draughts/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-07-16 11:01:45.734632 py-draughts-1.1.0/draughts/static/js/
--rw-rw-rw-   0        0        0     6118 2023-07-16 09:50:41.000000 py-draughts-1.1.0/draughts/static/js/script.js
-drwxrwxrwx   0        0        0        0 2023-07-16 11:01:45.737630 py-draughts-1.1.0/draughts/templates/
--rw-rw-rw-   0        0        0     1860 2023-07-11 16:32:17.000000 py-draughts-1.1.0/draughts/templates/base.html
--rw-rw-rw-   0        0        0     2882 2023-07-16 09:45:04.000000 py-draughts-1.1.0/draughts/templates/index.html
--rw-rw-rw-   0        0        0     1973 2023-07-16 10:59:23.000000 py-draughts-1.1.0/draughts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-16 11:01:45.749628 py-draughts-1.1.0/py_draughts.egg-info/
--rw-rw-rw-   0        0        0     6410 2023-07-16 11:01:45.000000 py-draughts-1.1.0/py_draughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-07-16 11:01:45.000000 py-draughts-1.1.0/py_draughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 11:01:45.000000 py-draughts-1.1.0/py_draughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-16 11:01:45.000000 py-draughts-1.1.0/py_draughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-16 11:01:45.000000 py-draughts-1.1.0/py_draughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 17:26:06.000000 py-draughts-1.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 11:01:45.754629 py-draughts-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1908 2023-07-16 09:45:04.000000 py-draughts-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 11:01:45.752631 py-draughts-1.1.0/test/
--rw-rw-rw-   0        0        0     1123 2023-07-16 10:55:42.000000 py-draughts-1.1.0/test/test_american_board.py
--rw-rw-rw-   0        0        0     2376 2023-07-16 09:45:04.000000 py-draughts-1.1.0/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:50:13.498782 py-draughts-1.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 12:53:30.000000 py-draughts-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-16 09:45:04.000000 py-draughts-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5364 2023-07-16 18:50:13.497783 py-draughts-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3944 2023-07-16 18:48:02.000000 py-draughts-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 18:50:13.469775 py-draughts-1.1.1/draughts/
+-rw-rw-rw-   0        0        0     1585 2023-07-16 18:50:04.000000 py-draughts-1.1.1/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3666 2023-07-16 18:41:37.000000 py-draughts-1.1.1/draughts/american.py
+-rw-rw-rw-   0        0        0    12410 2023-07-16 18:41:54.000000 py-draughts-1.1.1/draughts/base.py
+-rw-rw-rw-   0        0        0     3489 2023-07-16 18:17:38.000000 py-draughts-1.1.1/draughts/engine.py
+-rw-rw-rw-   0        0        0      671 2023-07-16 18:11:48.000000 py-draughts-1.1.1/draughts/models.py
+-rw-rw-rw-   0        0        0     4147 2023-07-16 18:11:26.000000 py-draughts-1.1.1/draughts/move.py
+-rw-rw-rw-   0        0        0     5300 2023-07-16 18:11:04.000000 py-draughts-1.1.1/draughts/server.py
+-rw-rw-rw-   0        0        0     7366 2023-07-16 18:41:03.000000 py-draughts-1.1.1/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:50:13.440779 py-draughts-1.1.1/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-16 18:50:13.471777 py-draughts-1.1.1/draughts/static/css/
+-rw-rw-rw-   0        0        0     3873 2023-07-16 09:45:04.000000 py-draughts-1.1.1/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-16 18:50:13.473777 py-draughts-1.1.1/draughts/static/js/
+-rw-rw-rw-   0        0        0     6118 2023-07-16 09:50:41.000000 py-draughts-1.1.1/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-16 18:50:13.476776 py-draughts-1.1.1/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-11 16:32:17.000000 py-draughts-1.1.1/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2882 2023-07-16 09:45:04.000000 py-draughts-1.1.1/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     1973 2023-07-16 10:59:23.000000 py-draughts-1.1.1/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:50:13.492776 py-draughts-1.1.1/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     5364 2023-07-16 18:50:13.000000 py-draughts-1.1.1/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-07-16 18:50:13.000000 py-draughts-1.1.1/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 18:50:13.000000 py-draughts-1.1.1/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-16 18:50:13.000000 py-draughts-1.1.1/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 18:50:13.000000 py-draughts-1.1.1/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 17:26:06.000000 py-draughts-1.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 18:50:13.498782 py-draughts-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1908 2023-07-16 09:45:04.000000 py-draughts-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:50:13.496783 py-draughts-1.1.1/test/
+-rw-rw-rw-   0        0        0     1104 2023-07-16 18:39:54.000000 py-draughts-1.1.1/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2376 2023-07-16 09:45:04.000000 py-draughts-1.1.1/test/test_board.py
```

### Comparing `py-draughts-1.1.0/LICENSE` & `py-draughts-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.0/PKG-INFO` & `py-draughts-1.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.1.0
+Version: 1.1.1
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/py-draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
@@ -39,140 +39,123 @@
 
 ## Installation
 
 ```bash
 pip install py-draughts
 ```
 
-## Key features
-1. Provides beautiful web interface for testing your engine/playing against AI.
-2. Supports multiple variants of the game (with different board size). `standard`, `american` etc.
-3. Follows international draughts standards. like `fen` `pdn` etc.
-4. Allows to easily create new variants of the game. by extending the `Board` class.
-5. Accurate documentation generated from code.
-
-
 
 ### [Documentation](https://michalskibinski109.github.io/py-draughts/)
 
-## Usage
-
-
+## Key features
 
-#### Displays simple ascii board
+-  Displays simple ascii board for different variants of the game.
 
 ```python
->>> from draughts import get_board
->>> board = get_board("standard")
-Board initialized with shape (10, 10). (base.py:108)
+>>> board = get_board('standard', "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
 >>> board
- . b . b . b . b . b
- b . b . b . b . b .
- . b . b . b . b . b
+ . . . . . B . w . .
  . . . . . . . . . .
+ . w . . . . . . . .
  . . . . . . . . . .
- . . . . . . . . . .
- . . . . . . . . . .
- w . w . w . w . w .
- . w . w . w . w . w
- w . w . w . w . w .
+ . b . . . . . . . .
+ . . b . w . . . . .
+ . w . b . W . W . .
+ . . . . w . . . w .
+ . W . . . w . W . w
+ W . w . . . . . . .
+
+>>> board = get_board("american")
+>>> board
+ . b . b . b . b
+ b . b . b . b .
+ . b . b . b . b
+ . . . . . . . .
+ . . . . . . . .
+ w . w . w . w .
+ . w . w . w . w
+ w . w . w . w .
+
 ```
 
-#### Make and undo moves
+- Make and undo moves
 
 ```python
->>> board.push_from_str("37-32")
->>> board.push_from_str("14-19")
->>> board.push_from_str("32-28")
->>> board.push_from_str("19-23")
+>>> board.push_uci("37-32")
 >>> board.pop() # undo last move
->>> board.push_from_str("19-23")
->>> board.push_from_str("28x19")
->>> board
- . b . b . b . b . b
- b . b . b . b . b .
- . b . b . b . . . b
- . . . . . . w . . .
- . . . . . . . . . .
- . . . . . . . . . .
- . . . . . . . . . .
- w . . . w . w . w .
- . w . w . w . w . w
- w . w . w . w . w .
+Move: 37->32
 ```
 
-#### Generate legal moves and validate moves
+- detects draws and wins
+
+```python
+>>> board.game_over
+False
+>>> board.is_threefold_repetition
+False
+```
+- Validate and generate moves
 
 ```python
->>> board.push_from_str("10x42")
-Move: 10->42 is correct, but not legal in given position.
- Legal moves are: [Move: 36->31, Move: 37->32, Move: 37->31, Move: 38->33, Move: 38->32, Move: 39->34, Move: 39->33, Move: 40->35, Move: 40->34]
+>>> board.push_uci("10x42")
+Move: 37->32 is correct, but not legal in given position.
+Legal moves are: [Move: 28->37, Move: 31->22]
 
 >>> list(board.legal_moves)
-[Move: 36->31, Move: 37->32, Move: 37->31, Move: 38->33, Move: 38->32, Move: 39->34, Move: 39->33, Move: 40->35, Move: 40->34]
+[Move: 28->37, Move: 31->22]
 ```
 
-#### Generate fen string and load board from fen string
-
+- Reads and writes fen strings
 
 ```python
->>> board =get_board('standard', "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
-Board initialized with shape (10, 10). (base.py:109)
->>> board.push_from_str("28-37")
+>>> board = get_board('standard', "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
 >>> board.fen
-'[FEN "B:W4,11,31,K33,K34,37,38,40,K41,43,K44,45,K46,47:BK3,21,27"]'
+'[FEN "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32"]'
 ```
-#### American checkers
+- Has simple engine
 
 ```python
->>> from draughts import get_board
->>> board = get_board("american")
-Board initialized with shape (8, 8). (base.py:108)
->>> board
- . b . b . b . b
- b . b . b . b .
- . b . b . b . b
- . . . . . . . .
- . . . . . . . .
- w . w . w . w .
- . w . w . w . w
- w . w . w . w .
+>>> from draughts.engine import AlphaBetaEngine
+>>> engine = AlphaBetaEngine(depth=5)
+>>> engine.get_best_move(board, with_evaluation=True)
+Move: 28->37, 3.0
 ```
 
-
 ## UI
 
 1. Allows to play against AI.
 2. Allows to play vs another player. (on the same computer)
 3. Allows to test and find bugs in your engine.
 
 ```python
-from draughts.server import Server
-Server().run()
+python -m draughts.server
 ```
 
 #### Use for testing your engine.
 
+
+
 _Example with simplest possible engine._
 
+
+
 ```python
->>> server = Server(get_best_move_method=lambda board: np.random.choice(list(board.legal_moves)))
+>>> get_best_mv = lambda board: np.random.choice(list(board.legal_moves))
+>>> server = Server(get_best_move_method=get_best_mv)
 >>> server.run()
 INFO:     Started server process [1617]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 ```
 
 _It is as simple as that!_
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/b5b3c1fe-3e08-4114-b73b-2b136e3c1c9b" width="800" />
-
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/a7d67a8a-a325-437e-90b5-ba443d1b0874" width="800" />
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/4deead2a-adf1-4a7a-9422-c8da43f31a53" width="800" />
 
 
 ### testing best moves finding methods:
 
 [Example](https://github.com/michalskibinski109/py-draughts/blob/main/examples/engine.py)
 
 ## Contributing
```

### Comparing `py-draughts-1.1.0/README.md` & `py-draughts-1.1.1/py_draughts.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: py-draughts
+Version: 1.1.1
+Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
+Home-page: https://github.com/michalskibinski109/draughts
+Author: Michał Skibiński
+Author-email: mskibinski109@gmail.com
+License: GPL-3.0+
+Project-URL: Documentation, https://michalskibinski109.github.io/py-draughts/index.html
+Keywords: draughts,checkers,AI mini-max,game,board
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Games/Entertainment :: Board Games
+Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # py-draughts
 
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
 [![Downloads](https://static.pepy.tech/personalized-badge/py-draughts?period=month&units=none&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/py-draughts)
 
 
@@ -10,140 +39,123 @@
 
 ## Installation
 
 ```bash
 pip install py-draughts
 ```
 
-## Key features
-1. Provides beautiful web interface for testing your engine/playing against AI.
-2. Supports multiple variants of the game (with different board size). `standard`, `american` etc.
-3. Follows international draughts standards. like `fen` `pdn` etc.
-4. Allows to easily create new variants of the game. by extending the `Board` class.
-5. Accurate documentation generated from code.
-
-
 
 ### [Documentation](https://michalskibinski109.github.io/py-draughts/)
 
-## Usage
-
-
+## Key features
 
-#### Displays simple ascii board
+-  Displays simple ascii board for different variants of the game.
 
 ```python
->>> from draughts import get_board
->>> board = get_board("standard")
-Board initialized with shape (10, 10). (base.py:108)
+>>> board = get_board('standard', "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
 >>> board
- . b . b . b . b . b
- b . b . b . b . b .
- . b . b . b . b . b
- . . . . . . . . . .
- . . . . . . . . . .
+ . . . . . B . w . .
  . . . . . . . . . .
+ . w . . . . . . . .
  . . . . . . . . . .
- w . w . w . w . w .
- . w . w . w . w . w
- w . w . w . w . w .
+ . b . . . . . . . .
+ . . b . w . . . . .
+ . w . b . W . W . .
+ . . . . w . . . w .
+ . W . . . w . W . w
+ W . w . . . . . . .
+
+>>> board = get_board("american")
+>>> board
+ . b . b . b . b
+ b . b . b . b .
+ . b . b . b . b
+ . . . . . . . .
+ . . . . . . . .
+ w . w . w . w .
+ . w . w . w . w
+ w . w . w . w .
+
 ```
 
-#### Make and undo moves
+- Make and undo moves
 
 ```python
->>> board.push_from_str("37-32")
->>> board.push_from_str("14-19")
->>> board.push_from_str("32-28")
->>> board.push_from_str("19-23")
+>>> board.push_uci("37-32")
 >>> board.pop() # undo last move
->>> board.push_from_str("19-23")
->>> board.push_from_str("28x19")
->>> board
- . b . b . b . b . b
- b . b . b . b . b .
- . b . b . b . . . b
- . . . . . . w . . .
- . . . . . . . . . .
- . . . . . . . . . .
- . . . . . . . . . .
- w . . . w . w . w .
- . w . w . w . w . w
- w . w . w . w . w .
+Move: 37->32
 ```
 
-#### Generate legal moves and validate moves
+- detects draws and wins
+
+```python
+>>> board.game_over
+False
+>>> board.is_threefold_repetition
+False
+```
+- Validate and generate moves
 
 ```python
->>> board.push_from_str("10x42")
-Move: 10->42 is correct, but not legal in given position.
- Legal moves are: [Move: 36->31, Move: 37->32, Move: 37->31, Move: 38->33, Move: 38->32, Move: 39->34, Move: 39->33, Move: 40->35, Move: 40->34]
+>>> board.push_uci("10x42")
+Move: 37->32 is correct, but not legal in given position.
+Legal moves are: [Move: 28->37, Move: 31->22]
 
 >>> list(board.legal_moves)
-[Move: 36->31, Move: 37->32, Move: 37->31, Move: 38->33, Move: 38->32, Move: 39->34, Move: 39->33, Move: 40->35, Move: 40->34]
+[Move: 28->37, Move: 31->22]
 ```
 
-#### Generate fen string and load board from fen string
-
+- Reads and writes fen strings
 
 ```python
->>> board =get_board('standard', "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
-Board initialized with shape (10, 10). (base.py:109)
->>> board.push_from_str("28-37")
+>>> board = get_board('standard', "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
 >>> board.fen
-'[FEN "B:W4,11,31,K33,K34,37,38,40,K41,43,K44,45,K46,47:BK3,21,27"]'
+'[FEN "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32"]'
 ```
-#### American checkers
+- Has simple engine
 
 ```python
->>> from draughts import get_board
->>> board = get_board("american")
-Board initialized with shape (8, 8). (base.py:108)
->>> board
- . b . b . b . b
- b . b . b . b .
- . b . b . b . b
- . . . . . . . .
- . . . . . . . .
- w . w . w . w .
- . w . w . w . w
- w . w . w . w .
+>>> from draughts.engine import AlphaBetaEngine
+>>> engine = AlphaBetaEngine(depth=5)
+>>> engine.get_best_move(board, with_evaluation=True)
+Move: 28->37, 3.0
 ```
 
-
 ## UI
 
 1. Allows to play against AI.
 2. Allows to play vs another player. (on the same computer)
 3. Allows to test and find bugs in your engine.
 
 ```python
-from draughts.server import Server
-Server().run()
+python -m draughts.server
 ```
 
 #### Use for testing your engine.
 
+
+
 _Example with simplest possible engine._
 
+
+
 ```python
->>> server = Server(get_best_move_method=lambda board: np.random.choice(list(board.legal_moves)))
+>>> get_best_mv = lambda board: np.random.choice(list(board.legal_moves))
+>>> server = Server(get_best_move_method=get_best_mv)
 >>> server.run()
 INFO:     Started server process [1617]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 ```
 
 _It is as simple as that!_
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/b5b3c1fe-3e08-4114-b73b-2b136e3c1c9b" width="800" />
-
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/a7d67a8a-a325-437e-90b5-ba443d1b0874" width="800" />
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/4deead2a-adf1-4a7a-9422-c8da43f31a53" width="800" />
 
 
 ### testing best moves finding methods:
 
 [Example](https://github.com/michalskibinski109/py-draughts/blob/main/examples/engine.py)
 
 ## Contributing
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `py-draughts-1.1.0/draughts/__init__.py` & `py-draughts-1.1.1/draughts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 A draughts library with advenced (customizable) WEB UI move generation and validation,
 PDN parsing and writing. Supports multiple variants of game.
 """
 
 from typing import Literal
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 __author__ = "Michał Skibiński"
 
 
 def get_board(variant: Literal["standard", "american"], fen: str = None):
     """
     Board factory method.
     - ``standard`` - standard draughts board
```

### Comparing `py-draughts-1.1.0/draughts/american.py` & `py-draughts-1.1.1/draughts/american.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,36 +30,41 @@
      - Only the king can capture backwards
      - Capture - choose any
     """
 
     GAME_TYPE = 23
     STARTING_POSITION = np.array([1] * 12 + [0] * 8 + [-1] * 12, dtype=np.int8)
     VARIANT_NAME = "American checkers"
+    ROW_IDX = {val: val // 4 for val in range(len(STARTING_POSITION))}
+    COL_IDX = {val: val % 8 for val in range(len(STARTING_POSITION))}
+
     size = int(np.sqrt(len(STARTING_POSITION) * 2))
-    row_idx = {val: val // 4 for val in range(len(STARTING_POSITION))}
-    col_idx = {val: val % 8 for val in range(len(STARTING_POSITION))}
 
     def __init__(self, starting_position=STARTING_POSITION) -> None:
         super().__init__(starting_position)
 
     @property
+    def is_draw(self) -> bool:
+        return self.is_threefold_repetition
+
+    @property
     def legal_moves(self) -> Generator[Move, None, None]:
         if self.turn == Color.BLACK:
             squares_list = np.transpose(np.nonzero(self._pos > 0))
         else:
             squares_list = np.transpose(np.nonzero(self._pos < 0))
         for square in squares_list.flatten():
             moves = self._legal_moves_from(square)
             for move in moves:
                 yield move
 
     def _legal_moves_from(
         self, square: int, is_after_capture=False
     ) -> Generator[Move, None, None]:
-        row = self.row_idx[square]
+        row = self.ROW_IDX[square]
         moves = []
         odd = bool(row % 2 != 0 and self.turn == Color.BLACK) or (
             row % 2 == 0 and self.turn == Color.WHITE
         )
         is_king = bool(self[square] == self.turn.value * Figure.KING)
         # is_king = False  # DEBUG
         for mv_offset, cap_offset, dir in [
@@ -70,22 +75,22 @@
             (5 - (not odd), 9, -self.turn.value),
         ]:
             move_sq = square + mv_offset * (dir)
             capture_sq = square + cap_offset * (dir)
 
             if (
                 0 <= move_sq < len(self._pos)
-                and row + 1 * (dir) == self.row_idx[move_sq]
+                and row + 1 * (dir) == self.ROW_IDX[move_sq]
                 and self[move_sq] == 0
                 and not is_after_capture
             ):
                 moves.append(Move([square, move_sq]))
             elif (
                 0 <= capture_sq < len(self._pos)
-                and row + 2 * (dir) == self.row_idx[capture_sq]
+                and row + 2 * (dir) == self.ROW_IDX[capture_sq]
                 and self[capture_sq] == 0
                 and self[move_sq] * self.turn.value < 0
             ):
                 move = Move(
                     [square, capture_sq],
                     captured_list=[move_sq],
                     captured_entities=[self[move_sq]],
@@ -96,23 +101,15 @@
                 self.pop(False)
 
         return moves
 
 
 if __name__ == "__main__":
     board = Board()
-    print(list(board.legal_moves))
-    # board.push_from_str("12-16")
-    # board.push_from_str("12-16")
-    # board.push_from_str("23-18")
-    # board.push_from_str("16-23")
-    # print(board.pop())
-    print(board)
-    # while True:
-    #     moves = board.legal_moves
-    #     move = np.random.choice(list(moves))
-    #     board.push(move)
-    #     print(move)
-    #     print(board)
-    #     from time import sleep
+    from draughts.server import Server
 
-    #     sleep(2)
+    Server(board).run()
+    moves = ["24-20", "11-16", "20x11", "7x16"]
+    for m in moves:
+        board.push_uci(m)
+        print(board)
+        print(list(board.legal_moves))
```

### Comparing `py-draughts-1.1.0/draughts/base.py` & `py-draughts-1.1.1/draughts/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-# documentation in rst format
-"""
-
-"""
-
 from __future__ import annotations
 
 import re
-from abc import ABC
+from abc import ABC, abstractproperty
 from typing import Generator
 
 import numpy as np
 
-from draughts.models import ENTITY_REPR, Color, Figure, SquareT
+from draughts.models import FIGURE_REPR, Color, Figure, SquareT
 from draughts.move import Move
 from draughts.utils import logger
 
 # fmt: off
 SQUARES = [_, B8, D8, F8, H8,
         A7, C7, E7, G7,
         B6, D6, F6, H6,
@@ -58,16 +53,25 @@
 
     GAME_TYPE = -1
     """
     PDN game type. See `PDN specification <https://en.wikipedia.org/wiki/Portable_Draughts_Notation>`_.
     """
     VARIANT_NAME = "Abstract variant"
     STARTING_POSITION = np.array([1] * 12 + [0] * 8 + [-1] * 12, dtype=np.int8)
-    row_idx = {val: val // 5 for val in range(len(STARTING_POSITION))}
-    col_idx = {val: val % 10 for val in range(len(STARTING_POSITION))}
+    ROW_IDX = ...
+    """ 
+    Dictionary of row indexes for every square. Generated only on module import. 
+    Used to calculate legal moves.
+    """
+
+    COL_IDX = ...
+    """
+    Same as ``ROW_IDX`` but for columns.
+    """
+
     STARTING_COLOR = Color.WHITE
     """
     Starting color. ``Color.WHITE`` or ``Color.BLACK``.
     """
 
     PSEUDO_LEGAL_KING_MOVES = None
     """
@@ -133,19 +137,23 @@
                 == self._moves_stack[-5].square_list
                 == self._moves_stack[-9].square_list
             ):
                 return True
         return False
 
     @property
+    def is_draw(self) -> bool:
+        raise NotImplementedError
+
+    @property
     def game_over(self) -> bool:
         """Returns ``True`` if the game is over."""
         # check if threefold repetition
 
-        return self.is_threefold_repetition or not bool(list(self.legal_moves))
+        return self.is_draw or not bool(list(self.legal_moves))
 
     def push(self, move: Move, is_finished: bool = True) -> None:
         """Pushes a move to the board.
         Automatically promotes a piece if it reaches the last row.
 
         If ``is_finished`` is set to ``True``, the turn is switched. This parameter is used only
         for generating legal moves.
@@ -187,23 +195,23 @@
         self._pos[src], self._pos[tg] = self._pos[tg], self._pos[src]
         for sq, entity in zip(move.captured_list, move.captured_entities):
             self._pos[sq] = entity  # Dangerous line
         if is_finished:
             self.turn = Color.WHITE if self.turn == Color.BLACK else Color.BLACK
         return move
 
-    def push_from_str(self, str_move: str) -> None:
+    def push_uci(self, str_move: str) -> None:
         """
         Allows to push a move from a string.
 
         * Converts string to ``Move`` object
         * calls ``BaseBoard.push`` method
         """
         try:
-            move = Move.from_string(str_move, self.legal_moves)
+            move = Move.from_uci(str_move, self.legal_moves)
         except ValueError as e:
             logger.error(f"{e} \n {str(self)}")
             raise e
         self.push(move)
 
     @property
     def fen(self):
@@ -318,15 +326,15 @@
 
     def __repr__(self) -> str:
         board = ""
         position = self.friendly_form
         for i in range(self.shape[0]):
             # board += f"{'-' * (self.shape[0]*4 + 1) }\n|"
             for j in range(self.shape[0]):
-                board += f" {ENTITY_REPR[position[i*self.shape[0] + j]]}"
+                board += f" {FIGURE_REPR[position[i*self.shape[0] + j]]}"
             board += "\n"
         return board
 
     def __iter__(self) -> Generator[Figure, None, None]:
         for sq in self.position:
             yield sq
```

### Comparing `py-draughts-1.1.0/draughts/models.py` & `py-draughts-1.1.1/draughts/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,14 @@
     WHITE_KING = Color.WHITE.value * 2
     WHITE_MAN = Color.WHITE.value
     KING = 2
     MAN = 1
     EMPTY = 0
 
 
-ENTITY_REPR = {
+FIGURE_REPR = {
     Figure.BLACK_MAN: "b",
     Figure.WHITE_MAN: "w",
     Figure.EMPTY: ".",
     Figure.BLACK_KING: "B",
     Figure.WHITE_KING: "W",
 }
```

### Comparing `py-draughts-1.1.0/draughts/move.py` & `py-draughts-1.1.1/draughts/move.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         return Move(
             self.square_list + other.square_list[1:],
             self.captured_list + other.captured_list,
             self.captured_entities + other.captured_entities,
         )
 
     @classmethod
-    def from_string(cls, move: str, legal_moves: Generator) -> Move:
+    def from_uci(cls, move: str, legal_moves: Generator) -> Move:
         """
 
         Converts string representation of move to ``Move`` object.
         This is generic method, so it can be used for any board size. Therefore,
         For different context different move object will be generated.
         Also we need to pass legal moves, to understand given move and check if it is legal.
```

### Comparing `py-draughts-1.1.0/draughts/server.py` & `py-draughts-1.1.1/draughts/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     def get_best_move(self, request: Request) -> PositionResponse:
         move = self.get_best_move_method(self.board)
         self.board.push(move)
         return self.position_json
 
     def move(self, request: Request, source: str, target: str) -> PositionResponse:
         move_str = f"{source}-{target}"
-        self.board.push_from_str(move_str)
+        self.board.push_uci(move_str)
         return self.position_json
 
     def pop(self, request: Request) -> PositionResponse:
         self.board.pop()
         return self.position_json
 
     def index(self, request: Request):
@@ -136,13 +136,12 @@
         )
 
     def run(self, **kwargs):
         uvicorn.run(self.APP, **kwargs)
 
 
 if __name__ == "__main__":
-    from draughts.standard import Board
+    from draughts.engine import AlphaBetaEngine
 
-    server = Server(
-        get_best_move_method=lambda board: np.random.choice(list(board.legal_moves)),
-    )
+    engine = AlphaBetaEngine(depth=5)
+    server = Server(get_best_move_method=engine.get_best_move)
     server.run()
```

### Comparing `py-draughts-1.1.0/draughts/static/css/style.css` & `py-draughts-1.1.1/draughts/static/css/style.css`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.0/draughts/static/js/script.js` & `py-draughts-1.1.1/draughts/static/js/script.js`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.0/draughts/templates/base.html` & `py-draughts-1.1.1/draughts/templates/base.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.0/draughts/templates/index.html` & `py-draughts-1.1.1/draughts/templates/index.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.0/draughts/utils.py` & `py-draughts-1.1.1/draughts/utils.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.0/py_draughts.egg-info/SOURCES.txt` & `py-draughts-1.1.1/py_draughts.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 draughts/__init__.py
 draughts/american.py
 draughts/base.py
+draughts/engine.py
 draughts/models.py
 draughts/move.py
 draughts/server.py
 draughts/standard.py
 draughts/utils.py
 draughts/static/css/style.css
 draughts/static/js/script.js
```

### Comparing `py-draughts-1.1.0/setup.py` & `py-draughts-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.0/test/test_american_board.py` & `py-draughts-1.1.1/test/test_american_board.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,25 +11,25 @@
     def setup(self):
         self.board = Board()
         yield
         del self.board
 
     def test_move_from_str_method(self):
         legal_moves = self.board.legal_moves
-        m1 = Move.from_string("24-20", legal_moves)
+        m1 = Move.from_uci("24-20", legal_moves)
         assert m1 == Move([checkers.G3, checkers.H4])
 
         with pytest.raises(ValueError):
-            Move.from_string("25-20", [])
+            Move.from_uci("25-20", [])
 
     def test_push_from_string(self):
-        m1 = Move.from_string("24-20", self.board.legal_moves)
-        self.board.push_from_str("24-20")
+        m1 = Move.from_uci("24-20", self.board.legal_moves)
+        self.board.push_uci("24-20")
         assert self.board.turn == Color.BLACK
         assert self.board.pop() == m1
         assert np.array_equal(self.board.position, Board.STARTING_POSITION)
 
     def test_capture(self):
         moves = ["24-20", "11-16", "20x11", "7x16"]
         for m in moves:
-            self.board.push_from_str(m)
+            self.board.push_uci(m)
         assert self.board[checkers.F6] == Figure.EMPTY.value
```

### Comparing `py-draughts-1.1.0/test/test_board.py` & `py-draughts-1.1.1/test/test_board.py`

 * *Files identical despite different names*

