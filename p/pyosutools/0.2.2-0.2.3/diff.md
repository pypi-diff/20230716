# Comparing `tmp/pyosutools-0.2.2.tar.gz` & `tmp/pyosutools-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyosutools-0.2.2.tar", last modified: Sun Jul  9 22:08:31 2023, max compression
+gzip compressed data, was "pyosutools-0.2.3.tar", last modified: Sun Jul 16 17:21:17 2023, max compression
```

## Comparing `pyosutools-0.2.2.tar` & `pyosutools-0.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:08:31.790630 pyosutools-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-09 22:08:16.000000 pyosutools-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-09 22:08:31.790630 pyosutools-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 22:08:16.000000 pyosutools-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:08:31.790630 pyosutools-0.2.2/pyosutools/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:08:31.790630 pyosutools-0.2.2/pyosutools/beatmaps/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/beatmaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/beatmaps/beatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/beatmaps/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:08:31.790630 pyosutools-0.2.2/pyosutools/db/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/db/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/db/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/db/osu.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/db/presence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/db/scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyosutools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:08:31.790630 pyosutools-0.2.2/pyosutools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-09 22:08:31.000000 pyosutools-0.2.2/pyosutools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-09 22:08:31.000000 pyosutools-0.2.2/pyosutools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 22:08:31.000000 pyosutools-0.2.2/pyosutools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-09 22:08:31.000000 pyosutools-0.2.2/pyosutools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 22:08:31.000000 pyosutools-0.2.2/pyosutools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-09 22:08:16.000000 pyosutools-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 22:08:31.790630 pyosutools-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:21:17.441890 pyosutools-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-16 17:21:06.000000 pyosutools-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-16 17:21:17.441890 pyosutools-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:21:06.000000 pyosutools-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:21:17.441890 pyosutools-0.2.3/pyosutools/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:21:17.441890 pyosutools-0.2.3/pyosutools/beatmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/beatmaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/beatmaps/beatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/beatmaps/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:21:17.441890 pyosutools-0.2.3/pyosutools/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/db/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/db/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/db/osu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/db/presence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/db/scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyosutools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:21:17.441890 pyosutools-0.2.3/pyosutools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-16 17:21:17.000000 pyosutools-0.2.3/pyosutools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-16 17:21:17.000000 pyosutools-0.2.3/pyosutools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:21:17.000000 pyosutools-0.2.3/pyosutools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 17:21:17.000000 pyosutools-0.2.3/pyosutools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 17:21:17.000000 pyosutools-0.2.3/pyosutools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-16 17:21:06.000000 pyosutools-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 17:21:17.441890 pyosutools-0.2.3/setup.cfg
```

### Comparing `pyosutools-0.2.2/LICENSE` & `pyosutools-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.2/PKG-INFO` & `pyosutools-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyosutools
-Version: 0.2.2
+Version: 0.2.3
 Summary: Parsing osu! files for easier usage
 Author-email: OlegSuperBro <olegrakovic323@gmail.com>
 Project-URL: Homepage, https://github.com/OlegSuperBro/pyosutools
 Project-URL: Bug Tracker, https://github.com/OlegSuperBro/pyosutools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyosutools-0.2.2/pyosutools/beatmaps/beatmap.py` & `pyosutools-0.2.3/pyosutools/beatmaps/beatmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import List, Tuple, Union
 
 from pyosutools.beatmaps.datatypes import (GeneralSettings, EditorSettings, Metadata, Difficulty,
                                            BaseEvent, TimingPoint, ComboColors, BaseHitObject, HitObjectType,
                                            EventType, BackgroundEvent, BreakEvent, VideoEvent,
                                            CircleObject, ManiaHoldObject, SliderObject, SpinnerObject,
                                            SliderType, CurvePoint, HitSound, HitSample)
-from pyosutools.utils import is_int
+from pyosutools.utils import is_number, as_number, is_int
 
 
 @dataclass
 class Beatmap:
     version: int
     general_settings: GeneralSettings
     editor_settings: EditorSettings
@@ -196,32 +196,32 @@
             header = _Parser.check_header(line)
             if header is not None:
                 curr_header = header
                 continue
 
             if curr_header == "General":
                 key, value = _Parser.parse_line_with_key(line)
-                general_dict[key] = int(value) if is_int(value) else value
+                general_dict[key] = as_number(value) if is_number(value) else value
                 continue
 
             elif curr_header == "Editor":
                 key, value = _Parser.parse_line_with_key(line)
-                editor_dict[key] = int(value) if is_int(value) else value
+                editor_dict[key] = as_number(value) if is_number(value) else value
                 continue
 
             elif curr_header == "Metadata":
                 key, value = _Parser.parse_line_with_key(line)
                 key = key.replace("i_d", "id")
-                metadata_dict[key] = int(value) if is_int(value) else value
+                metadata_dict[key] = as_number(value) if is_number(value) else value
                 continue
 
             elif curr_header == "Difficulty":
                 key, value = _Parser.parse_line_with_key(line)
                 key = key.replace("h_p", "hp")
-                difficulty_dict[key] = int(value) if is_int(value) else value
+                difficulty_dict[key] = as_number(value) if is_number(value) else value
                 continue
 
             elif curr_header == "Events":
                 values = _Parser.parse_line_without_key(line)
 
                 event = _Parser.parse_event(values)
                 if event is not None:
```

### Comparing `pyosutools-0.2.2/pyosutools/beatmaps/datatypes.py` & `pyosutools-0.2.3/pyosutools/beatmaps/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.2/pyosutools/datatypes.py` & `pyosutools-0.2.3/pyosutools/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.2/pyosutools/db/collection.py` & `pyosutools-0.2.3/pyosutools/db/collection.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.2/pyosutools/db/datatypes.py` & `pyosutools-0.2.3/pyosutools/db/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.2/pyosutools/db/osu.py` & `pyosutools-0.2.3/pyosutools/db/osu.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.2/pyosutools/db/presence.py` & `pyosutools-0.2.3/pyosutools/db/presence.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.2/pyosutools/db/scores.py` & `pyosutools-0.2.3/pyosutools/db/scores.py`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.2/pyosutools/utils.py` & `pyosutools-0.2.3/pyosutools/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import struct
 import datetime
 
+from typing import Union
+
 
 # PART OF CODE COPIED FROM https://github.com/jaasonw/osu-db-tools
 def read_bool(buffer) -> bool:
     return struct.unpack("<?", buffer.read(1))[0]
 
 
 def read_ubyte(buffer) -> int:
@@ -57,15 +59,15 @@
         # https://en.wikipedia.org/wiki/LEB128
         while True:
             byte = read_ubyte(buffer)
             strlen |= ((byte & 0x7F) << shift)
             if (byte & (1 << 7)) == 0:
                 break
             shift += 7
-    return (struct.unpack("<" + str(strlen) + "s", buffer.read(strlen))[0]).decode(encoding)
+    return struct.unpack(f"<{str(strlen)}s", buffer.read(strlen))[0].decode(encoding)
 # PART OF CODE COPIED FROM https://github.com/jaasonw/osu-db-tools
 
 
 def read_datetime(buffer) -> datetime.datetime:
     ticks = read_ulong(buffer)
     if ticks >= 621355968000000000:
         return datetime.datetime.fromtimestamp((ticks-621355968000000000)/10_000_000, tz=datetime.timezone.utc)
@@ -75,7 +77,24 @@
 
 def is_int(text) -> bool:
     try:
         assert int(text) == float(text)
     except (ValueError, AssertionError):
         return False
     return True
+
+
+def is_number(text) -> bool:
+    try:
+        float(text)
+    except (ValueError):
+        return False
+    return True
+
+
+def as_number(number) -> Union[int, float]:
+    if is_int(number):
+        return int(number)
+    elif is_number(number):
+        return float(number)
+    else:
+        raise ValueError(f"could not convert '{type(number)}' to number: {number}")
```

### Comparing `pyosutools-0.2.2/pyosutools.egg-info/PKG-INFO` & `pyosutools-0.2.3/pyosutools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyosutools
-Version: 0.2.2
+Version: 0.2.3
 Summary: Parsing osu! files for easier usage
 Author-email: OlegSuperBro <olegrakovic323@gmail.com>
 Project-URL: Homepage, https://github.com/OlegSuperBro/pyosutools
 Project-URL: Bug Tracker, https://github.com/OlegSuperBro/pyosutools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyosutools-0.2.2/pyosutools.egg-info/SOURCES.txt` & `pyosutools-0.2.3/pyosutools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyosutools-0.2.2/pyproject.toml` & `pyosutools-0.2.3/pyproject.toml`

 * *Files identical despite different names*

