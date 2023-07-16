# Comparing `tmp/cshogi-0.6.0.tar.gz` & `tmp/cshogi-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cshogi-0.6.0.tar", last modified: Tue Jul 11 14:57:14 2023, max compression
+gzip compressed data, was "cshogi-0.6.1.tar", last modified: Sun Jul 16 15:49:55 2023, max compression
```

## Comparing `cshogi-0.6.0.tar` & `cshogi-0.6.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 14:57:14.303723 cshogi-0.6.0/
--rw-rw-rw-   0        0        0    35823 2023-07-11 14:56:37.000000 cshogi-0.6.0/LICENSE
--rw-rw-rw-   0        0        0      358 2023-07-11 14:57:14.303723 cshogi-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     5135 2023-07-11 14:56:37.000000 cshogi-0.6.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-11 14:57:14.288086 cshogi-0.6.0/cshogi/
--rw-rw-rw-   0        0        0     2774 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/CSA.py
--rw-rw-rw-   0        0        0    18556 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/KI2.py
--rw-rw-rw-   0        0        0    19549 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/KIF.py
--rw-rw-rw-   0        0        0     2988 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/PGN.py
--rw-rw-rw-   0        0        0       27 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/__init__.py
--rw-rw-rw-   0        0        0    33413 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/_cshogi.pyx
--rw-rw-rw-   0        0        0    25971 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-11 14:57:14.303723 cshogi-0.6.0/cshogi/dlshogi/
--rw-rw-rw-   0        0        0      327 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/dlshogi/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/elo.py
-drwxrwxrwx   0        0        0        0 2023-07-11 14:57:14.303723 cshogi-0.6.0/cshogi/gym_shogi/
--rw-rw-rw-   0        0        0      132 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/gym_shogi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 14:57:14.303723 cshogi-0.6.0/cshogi/gym_shogi/envs/
--rw-rw-rw-   0        0        0      118 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/gym_shogi/envs/__init__.py
--rw-rw-rw-   0        0        0     2259 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/gym_shogi/envs/shogi_env.pyx
--rw-rw-rw-   0        0        0      755 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/gym_shogi/envs/shogi_vec_env.pyx
-drwxrwxrwx   0        0        0        0 2023-07-11 14:57:14.303723 cshogi-0.6.0/cshogi/usi/
--rw-rw-rw-   0        0        0    10531 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/usi/Engine.py
--rw-rw-rw-   0        0        0       26 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/usi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 14:57:14.303723 cshogi-0.6.0/cshogi/web/
--rw-rw-rw-   0        0        0    13662 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/web/app.py
-drwxrwxrwx   0        0        0        0 2023-07-11 14:57:14.303723 cshogi-0.6.0/cshogi/web/static/
--rw-rw-rw-   0        0        0    13931 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/web/static/board.js
-drwxrwxrwx   0        0        0        0 2023-07-11 14:57:14.303723 cshogi-0.6.0/cshogi/web/templates/
--rw-rw-rw-   0        0        0    17362 2023-07-11 14:56:37.000000 cshogi-0.6.0/cshogi/web/templates/board.html
-drwxrwxrwx   0        0        0        0 2023-07-11 14:57:14.288086 cshogi-0.6.0/cshogi.egg-info/
--rw-rw-rw-   0        0        0      358 2023-07-11 14:57:14.000000 cshogi-0.6.0/cshogi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      787 2023-07-11 14:57:14.000000 cshogi-0.6.0/cshogi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 14:57:14.000000 cshogi-0.6.0/cshogi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 14:57:14.000000 cshogi-0.6.0/cshogi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 14:57:14.303723 cshogi-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     2040 2023-07-11 14:56:37.000000 cshogi-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 14:57:14.303723 cshogi-0.6.0/src/
--rw-rw-rw-   0        0        0     8208 2023-07-11 14:56:37.000000 cshogi-0.6.0/src/bitboard.cpp
--rw-rw-rw-   0        0        0     3267 2023-07-11 14:56:37.000000 cshogi-0.6.0/src/book.cpp
--rw-rw-rw-   0        0        0     1350 2023-07-11 14:56:37.000000 cshogi-0.6.0/src/common.cpp
--rw-rw-rw-   0        0        0    28484 2023-07-11 14:56:37.000000 cshogi-0.6.0/src/dfpn.cpp
--rw-rw-rw-   0        0        0    50568 2023-07-11 14:56:37.000000 cshogi-0.6.0/src/generateMoves.cpp
--rw-rw-rw-   0        0        0     1789 2023-07-11 14:56:37.000000 cshogi-0.6.0/src/hand.cpp
--rw-rw-rw-   0        0        0    19051 2023-07-11 14:56:37.000000 cshogi-0.6.0/src/init.cpp
--rw-rw-rw-   0        0        0     6937 2023-07-11 14:56:37.000000 cshogi-0.6.0/src/mate.cpp
--rw-rw-rw-   0        0        0     2163 2023-07-11 14:56:37.000000 cshogi-0.6.0/src/move.cpp
--rw-rw-rw-   0        0        0     1172 2023-07-11 14:56:37.000000 cshogi-0.6.0/src/mt64bit.cpp
--rw-rw-rw-   0        0        0   174059 2023-07-11 14:56:37.000000 cshogi-0.6.0/src/position.cpp
--rw-rw-rw-   0        0        0     3308 2023-07-11 14:56:37.000000 cshogi-0.6.0/src/search.cpp
--rw-rw-rw-   0        0        0     1416 2023-07-11 14:56:37.000000 cshogi-0.6.0/src/square.cpp
--rw-rw-rw-   0        0        0     6627 2023-07-11 14:56:37.000000 cshogi-0.6.0/src/usi.cpp
-drwxrwxrwx   0        0        0        0 2023-07-11 14:57:14.303723 cshogi-0.6.0/test/
--rw-rw-rw-   0        0        0      824 2023-07-11 14:56:37.000000 cshogi-0.6.0/test/test_usi_engine.py
+drwxrwxrwx   0        0        0        0 2023-07-16 15:49:55.131825 cshogi-0.6.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-16 15:49:10.000000 cshogi-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0      358 2023-07-16 15:49:55.131825 cshogi-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5135 2023-07-16 15:49:10.000000 cshogi-0.6.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-16 15:49:55.116199 cshogi-0.6.1/cshogi/
+-rw-rw-rw-   0        0        0     2774 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/CSA.py
+-rw-rw-rw-   0        0        0    18556 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/KI2.py
+-rw-rw-rw-   0        0        0    19549 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/KIF.py
+-rw-rw-rw-   0        0        0     2988 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/PGN.py
+-rw-rw-rw-   0        0        0       27 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/__init__.py
+-rw-rw-rw-   0        0        0    33413 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/_cshogi.pyx
+-rw-rw-rw-   0        0        0    25971 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-16 15:49:55.116199 cshogi-0.6.1/cshogi/dlshogi/
+-rw-rw-rw-   0        0        0      327 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/dlshogi/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/elo.py
+drwxrwxrwx   0        0        0        0 2023-07-16 15:49:55.116199 cshogi-0.6.1/cshogi/gym_shogi/
+-rw-rw-rw-   0        0        0      132 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/gym_shogi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 15:49:55.116199 cshogi-0.6.1/cshogi/gym_shogi/envs/
+-rw-rw-rw-   0        0        0      118 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/gym_shogi/envs/__init__.py
+-rw-rw-rw-   0        0        0     2259 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/gym_shogi/envs/shogi_env.pyx
+-rw-rw-rw-   0        0        0      755 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/gym_shogi/envs/shogi_vec_env.pyx
+drwxrwxrwx   0        0        0        0 2023-07-16 15:49:55.116199 cshogi-0.6.1/cshogi/usi/
+-rw-rw-rw-   0        0        0    10526 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/usi/Engine.py
+-rw-rw-rw-   0        0        0       26 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/usi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 15:49:55.116199 cshogi-0.6.1/cshogi/web/
+-rw-rw-rw-   0        0        0    13662 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/web/app.py
+drwxrwxrwx   0        0        0        0 2023-07-16 15:49:55.116199 cshogi-0.6.1/cshogi/web/static/
+-rw-rw-rw-   0        0        0    13931 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/web/static/board.js
+drwxrwxrwx   0        0        0        0 2023-07-16 15:49:55.116199 cshogi-0.6.1/cshogi/web/templates/
+-rw-rw-rw-   0        0        0    17362 2023-07-16 15:49:10.000000 cshogi-0.6.1/cshogi/web/templates/board.html
+drwxrwxrwx   0        0        0        0 2023-07-16 15:49:55.116199 cshogi-0.6.1/cshogi.egg-info/
+-rw-rw-rw-   0        0        0      358 2023-07-16 15:49:54.000000 cshogi-0.6.1/cshogi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      787 2023-07-16 15:49:55.000000 cshogi-0.6.1/cshogi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 15:49:54.000000 cshogi-0.6.1/cshogi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 15:49:54.000000 cshogi-0.6.1/cshogi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 15:49:55.131825 cshogi-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     2040 2023-07-16 15:49:10.000000 cshogi-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 15:49:55.131825 cshogi-0.6.1/src/
+-rw-rw-rw-   0        0        0     8208 2023-07-16 15:49:10.000000 cshogi-0.6.1/src/bitboard.cpp
+-rw-rw-rw-   0        0        0     3267 2023-07-16 15:49:10.000000 cshogi-0.6.1/src/book.cpp
+-rw-rw-rw-   0        0        0     1350 2023-07-16 15:49:10.000000 cshogi-0.6.1/src/common.cpp
+-rw-rw-rw-   0        0        0    28484 2023-07-16 15:49:10.000000 cshogi-0.6.1/src/dfpn.cpp
+-rw-rw-rw-   0        0        0    50568 2023-07-16 15:49:10.000000 cshogi-0.6.1/src/generateMoves.cpp
+-rw-rw-rw-   0        0        0     1789 2023-07-16 15:49:10.000000 cshogi-0.6.1/src/hand.cpp
+-rw-rw-rw-   0        0        0    19051 2023-07-16 15:49:10.000000 cshogi-0.6.1/src/init.cpp
+-rw-rw-rw-   0        0        0     6937 2023-07-16 15:49:10.000000 cshogi-0.6.1/src/mate.cpp
+-rw-rw-rw-   0        0        0     2163 2023-07-16 15:49:10.000000 cshogi-0.6.1/src/move.cpp
+-rw-rw-rw-   0        0        0     1172 2023-07-16 15:49:10.000000 cshogi-0.6.1/src/mt64bit.cpp
+-rw-rw-rw-   0        0        0   174059 2023-07-16 15:49:10.000000 cshogi-0.6.1/src/position.cpp
+-rw-rw-rw-   0        0        0     3308 2023-07-16 15:49:10.000000 cshogi-0.6.1/src/search.cpp
+-rw-rw-rw-   0        0        0     1416 2023-07-16 15:49:10.000000 cshogi-0.6.1/src/square.cpp
+-rw-rw-rw-   0        0        0     6627 2023-07-16 15:49:10.000000 cshogi-0.6.1/src/usi.cpp
+drwxrwxrwx   0        0        0        0 2023-07-16 15:49:55.131825 cshogi-0.6.1/test/
+-rw-rw-rw-   0        0        0      824 2023-07-16 15:49:10.000000 cshogi-0.6.1/test/test_usi_engine.py
```

### Comparing `cshogi-0.6.0/LICENSE` & `cshogi-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/README.rst` & `cshogi-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/cshogi/CSA.py` & `cshogi-0.6.1/cshogi/CSA.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/cshogi/KI2.py` & `cshogi-0.6.1/cshogi/KI2.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/cshogi/KIF.py` & `cshogi-0.6.1/cshogi/KIF.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/cshogi/PGN.py` & `cshogi-0.6.1/cshogi/PGN.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/cshogi/_cshogi.pyx` & `cshogi-0.6.1/cshogi/_cshogi.pyx`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/cshogi/cli.py` & `cshogi-0.6.1/cshogi/cli.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/cshogi/elo.py` & `cshogi-0.6.1/cshogi/elo.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/cshogi/gym_shogi/envs/shogi_env.pyx` & `cshogi-0.6.1/cshogi/gym_shogi/envs/shogi_env.pyx`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/cshogi/gym_shogi/envs/shogi_vec_env.pyx` & `cshogi-0.6.1/cshogi/gym_shogi/envs/shogi_vec_env.pyx`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/cshogi/usi/Engine.py` & `cshogi-0.6.1/cshogi/usi/Engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def __init__(self, mate_score=100000, listner=None):
         self.__info = {}
         self.__listner = listner
         self.__mate_score = mate_score
         self.__bestmove = None
 
     @staticmethod
-    def _split_info(m: re.Match[str]) -> dict:
+    def _split_info(m: re.Match) -> dict:
         items = (m[1] + m[4]).split(' ')
         info_dict = {}
         for name, value in zip(items[::2], items[1::2]):
             info_dict[name] = int(value)
         if m[2] == 'cp':
             info_dict['score'] = 'cp'
             info_dict['cp'] = int(m[3])
```

### Comparing `cshogi-0.6.0/cshogi/web/app.py` & `cshogi-0.6.1/cshogi/web/app.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/cshogi/web/static/board.js` & `cshogi-0.6.1/cshogi/web/static/board.js`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/cshogi/web/templates/board.html` & `cshogi-0.6.1/cshogi/web/templates/board.html`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/cshogi.egg-info/SOURCES.txt` & `cshogi-0.6.1/cshogi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/setup.py` & `cshogi-0.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     Extension('cshogi.gym_shogi.envs.shogi_vec_env',
         ['cshogi/gym_shogi/envs/shogi_vec_env.pyx'],
         language='c++'),
 ]
 
 setup(
     name='cshogi',
-    version='0.6.0',
+    version='0.6.1',
     packages=['cshogi', 'cshogi.usi', 'cshogi.gym_shogi', 'cshogi.gym_shogi.envs', 'cshogi.dlshogi', 'cshogi.web', 'cshogi.web.templates', 'cshogi.web.static'],
     package_data={'cshogi.web.templates': ['*'], 'cshogi.web.static': ['*']},
     ext_modules=ext_modules,
     cmdclass={'build_ext': my_build_ext},
     author='Tadao Yamaoka',
     url='https://github.com/TadaoYamaoka/cshogi',
     description = 'A fast Python shogi library',
```

### Comparing `cshogi-0.6.0/src/bitboard.cpp` & `cshogi-0.6.1/src/bitboard.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/src/book.cpp` & `cshogi-0.6.1/src/book.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/src/common.cpp` & `cshogi-0.6.1/src/common.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/src/dfpn.cpp` & `cshogi-0.6.1/src/dfpn.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/src/generateMoves.cpp` & `cshogi-0.6.1/src/generateMoves.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/src/hand.cpp` & `cshogi-0.6.1/src/hand.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/src/init.cpp` & `cshogi-0.6.1/src/init.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/src/mate.cpp` & `cshogi-0.6.1/src/mate.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/src/move.cpp` & `cshogi-0.6.1/src/move.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/src/mt64bit.cpp` & `cshogi-0.6.1/src/mt64bit.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/src/position.cpp` & `cshogi-0.6.1/src/position.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/src/search.cpp` & `cshogi-0.6.1/src/search.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/src/square.cpp` & `cshogi-0.6.1/src/square.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/src/usi.cpp` & `cshogi-0.6.1/src/usi.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.6.0/test/test_usi_engine.py` & `cshogi-0.6.1/test/test_usi_engine.py`

 * *Files identical despite different names*

