# Comparing `tmp/lichesspy-5.0.2.tar.gz` & `tmp/lichesspy-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lichesspy-5.0.2.tar", last modified: Sun Jul 16 13:52:42 2023, max compression
+gzip compressed data, was "lichesspy-5.0.3.tar", last modified: Sun Jul 16 14:16:03 2023, max compression
```

## Comparing `lichesspy-5.0.2.tar` & `lichesspy-5.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:52:42.116107 lichesspy-5.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-16 13:52:31.000000 lichesspy-5.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-16 13:52:42.116107 lichesspy-5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-16 13:52:31.000000 lichesspy-5.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:52:42.116107 lichesspy-5.0.2/lichesspy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 13:52:31.000000 lichesspy-5.0.2/lichesspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-07-16 13:52:31.000000 lichesspy-5.0.2/lichesspy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-16 13:52:31.000000 lichesspy-5.0.2/lichesspy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-16 13:52:31.000000 lichesspy-5.0.2/lichesspy/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-16 13:52:31.000000 lichesspy-5.0.2/lichesspy/pgn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:52:42.116107 lichesspy-5.0.2/lichesspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-16 13:52:42.000000 lichesspy-5.0.2/lichesspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-16 13:52:42.000000 lichesspy-5.0.2/lichesspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 13:52:42.000000 lichesspy-5.0.2/lichesspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-16 13:52:42.000000 lichesspy-5.0.2/lichesspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-16 13:52:42.000000 lichesspy-5.0.2/lichesspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 13:52:42.116107 lichesspy-5.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-16 13:52:31.000000 lichesspy-5.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:16:03.442761 lichesspy-5.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-16 14:15:53.000000 lichesspy-5.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-16 14:16:03.442761 lichesspy-5.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-16 14:15:53.000000 lichesspy-5.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:16:03.438761 lichesspy-5.0.3/lichesspy/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-16 14:15:53.000000 lichesspy-5.0.3/lichesspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-07-16 14:15:53.000000 lichesspy-5.0.3/lichesspy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-16 14:15:53.000000 lichesspy-5.0.3/lichesspy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-16 14:15:53.000000 lichesspy-5.0.3/lichesspy/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-16 14:15:53.000000 lichesspy-5.0.3/lichesspy/pgn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 14:16:03.442761 lichesspy-5.0.3/lichesspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-16 14:16:03.000000 lichesspy-5.0.3/lichesspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-16 14:16:03.000000 lichesspy-5.0.3/lichesspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 14:16:03.000000 lichesspy-5.0.3/lichesspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-16 14:16:03.000000 lichesspy-5.0.3/lichesspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-16 14:16:03.000000 lichesspy-5.0.3/lichesspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 14:16:03.442761 lichesspy-5.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-16 14:15:53.000000 lichesspy-5.0.3/setup.py
```

### Comparing `lichesspy-5.0.2/LICENSE` & `lichesspy-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lichesspy-5.0.2/PKG-INFO` & `lichesspy-5.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lichesspy
-Version: 5.0.2
+Version: 5.0.3
 Summary: Python wrapper for lichess
 Home-page: https://github.com/Liffecs/lichesspy
 Author: Liffecs
 Author-email: Liffecs@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lichesspy-5.0.2/README.md` & `lichesspy-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lichesspy-5.0.2/lichesspy/api.py` & `lichesspy-5.0.3/lichesspy/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+""""
+ File: api.py
+ Package: lichesspy
+ Author: Liffecs
+ Created: 01.12.2021
+ Modified: 16.07.2023
+ Version: 5.0.3
+"""
+
+
 def users_by_ids(ids, **kwargs):
     """Wrapper for the `POST /api/users <https://github.com/ornicar/lila#post-apiusers-fetch-many-users-by-id>`_ endpoint.
     Returns a generator that splits the IDs into multiple requests as needed.
 
     Note: Use :data:`~lichesspy.api.users_status` when possible, since it is cheaper and not rate-limited.
 
     >>> users = lichesspy.api.users_by_ids(['thibault', 'cyanfish'])
```

### Comparing `lichesspy-5.0.2/lichesspy/format.py` & `lichesspy-5.0.3/lichesspy/format.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,20 @@
-from six import StringIO
+""""
+ File: format.py
+ Package: lichesspy
+ Author: Liffecs
+ Created: 01.12.2021
+ Modified: 16.07.2023
+ Version: 5.0.3
+"""
+
 import json
 
+from six import StringIO
+
 GAME_STREAM_OBJECT = "game_stream"
 STREAM_OBJECT = "stream"
 GAME_OBJECT = "game"
 PUBLIC_API_OBJECT = "public_api"
 MOBILE_API_OBJECT = "mobile_api"
```

### Comparing `lichesspy-5.0.2/lichesspy/pgn.py` & `lichesspy-5.0.3/lichesspy/pgn.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,16 @@
+""""
+ File: api.py
+ Package: lichesspy
+ Author: Liffecs
+ Created: 01.12.2021
+ Modified: 16.07.2023
+ Version: 5.0.3
 """
-PGN Functions
-"""
+
 import re
 
 
 def parse_pgn(pgn_string):
     """Parse a PGN string and return a list of games as dictionaries."""
     games = []
     pgn_blocks = _extract_pgn_blocks(pgn_string)
@@ -18,15 +24,15 @@
     """Extract PGN blocks from a PGN string."""
     pgn_blocks = re.split(r"\s*\n\n", pgn_string)
     pgn_blocks = [block.strip() for block in pgn_blocks if block.strip()]
     return pgn_blocks
 
 
 def _parse_pgn_block(pgn_block):
-    """Parse a PGN block and return a game as a dictionary."""
+    """Parse a PGN block and return a game as a dictionary."    ""
     game = {}
     tags, moves = pgn_block.split("\n\n", maxsplit=1)
     game["tags"] = _parse_pgn_tags(tags)
     game["moves"] = _parse_pgn_moves(moves)
     return game
```

### Comparing `lichesspy-5.0.2/lichesspy.egg-info/PKG-INFO` & `lichesspy-5.0.3/lichesspy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lichesspy
-Version: 5.0.2
+Version: 5.0.3
 Summary: Python wrapper for lichess
 Home-page: https://github.com/Liffecs/lichesspy
 Author: Liffecs
 Author-email: Liffecs@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lichesspy-5.0.2/setup.py` & `lichesspy-5.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     with open("README.md") as file_content:
         readme = file_content.read()
     return readme
 
 
 setuptools.setup(
     name="lichesspy",
-    version="5.0.2",
+    version="5.0.3",
     author="Liffecs",
     author_email="Liffecs@gmail.com",
     description="Python wrapper for lichess",
     long_description=def_readme(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/Liffecs/lichesspy",
```

