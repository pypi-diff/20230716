# Comparing `tmp/Coquille-1.0.2.tar.gz` & `tmp/Coquille-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Coquille-1.0.2.tar", last modified: Sat Jul 15 11:38:19 2023, max compression
+gzip compressed data, was "Coquille-1.1.1.tar", last modified: Sun Jul 16 09:04:01 2023, max compression
```

## Comparing `Coquille-1.0.2.tar` & `Coquille-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-15 11:38:19.067735 Coquille-1.0.2/
--rw-r--r--   0 qexat     (1000) qexat     (1001)     1813 2023-07-14 10:50:09.000000 Coquille-1.0.2/.gitignore
--rw-r--r--   0 qexat     (1000) qexat     (1001)      551 2023-07-14 10:50:09.000000 Coquille-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 qexat     (1000) qexat     (1001)     1062 2023-07-14 10:50:09.000000 Coquille-1.0.2/LICENSE
--rw-r--r--   0 qexat     (1000) qexat     (1001)     4842 2023-07-15 11:38:19.067735 Coquille-1.0.2/PKG-INFO
--rw-r--r--   0 qexat     (1000) qexat     (1001)     3086 2023-07-14 10:50:09.000000 Coquille-1.0.2/README.md
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-15 11:38:19.057735 Coquille-1.0.2/examples/
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-15 11:38:19.061068 Coquille-1.0.2/examples/coquille_context/
--rw-r--r--   0 qexat     (1000) qexat     (1001)      437 2023-07-14 10:50:09.000000 Coquille-1.0.2/examples/coquille_context/__main__.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)    31985 2023-07-14 10:50:09.000000 Coquille-1.0.2/examples/coquille_context/screenshot.png
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-15 11:38:19.064401 Coquille-1.0.2/examples/coquille_write/
--rw-r--r--   0 qexat     (1000) qexat     (1001)      436 2023-07-14 10:50:09.000000 Coquille-1.0.2/examples/coquille_write/__main__.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)       45 2023-07-14 10:50:09.000000 Coquille-1.0.2/examples/coquille_write/output.txt
--rw-r--r--   0 qexat     (1000) qexat     (1001)    44980 2023-07-14 10:50:09.000000 Coquille-1.0.2/examples/coquille_write/screenshot.png
--rw-r--r--   0 qexat     (1000) qexat     (1001)      698 2023-07-15 11:32:25.000000 Coquille-1.0.2/pyproject.toml
--rw-r--r--   0 qexat     (1000) qexat     (1001)       38 2023-07-15 11:38:19.071068 Coquille-1.0.2/setup.cfg
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-15 11:38:19.057735 Coquille-1.0.2/src/
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-15 11:38:19.064401 Coquille-1.0.2/src/Coquille.egg-info/
--rw-r--r--   0 qexat     (1000) qexat     (1001)     4842 2023-07-15 11:38:19.000000 Coquille-1.0.2/src/Coquille.egg-info/PKG-INFO
--rw-r--r--   0 qexat     (1000) qexat     (1001)      601 2023-07-15 11:38:19.000000 Coquille-1.0.2/src/Coquille.egg-info/SOURCES.txt
--rw-r--r--   0 qexat     (1000) qexat     (1001)        1 2023-07-15 11:38:19.000000 Coquille-1.0.2/src/Coquille.egg-info/dependency_links.txt
--rw-r--r--   0 qexat     (1000) qexat     (1001)       35 2023-07-15 11:38:19.000000 Coquille-1.0.2/src/Coquille.egg-info/requires.txt
--rw-r--r--   0 qexat     (1000) qexat     (1001)        9 2023-07-15 11:38:19.000000 Coquille-1.0.2/src/Coquille.egg-info/top_level.txt
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-15 11:38:19.067735 Coquille-1.0.2/src/coquille/
--rw-r--r--   0 qexat     (1000) qexat     (1001)       32 2023-07-14 10:50:09.000000 Coquille-1.0.2/src/coquille/__init__.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)     6335 2023-07-15 11:32:17.000000 Coquille-1.0.2/src/coquille/coquille.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)    10596 2023-07-14 10:50:09.000000 Coquille-1.0.2/src/coquille/sequences.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)      340 2023-07-14 10:50:09.000000 Coquille-1.0.2/src/coquille/typeshed.py
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-15 11:38:19.067735 Coquille-1.0.2/tests/
--rw-r--r--   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:50:09.000000 Coquille-1.0.2/tests/__init__.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)     1081 2023-07-14 10:50:09.000000 Coquille-1.0.2/tests/coquille_test.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)     4219 2023-07-14 10:50:09.000000 Coquille-1.0.2/tests/sequences_test.py
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:04:01.549366 Coquille-1.1.1/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     1813 2023-07-14 10:50:09.000000 Coquille-1.1.1/.gitignore
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      551 2023-07-14 10:50:09.000000 Coquille-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     1062 2023-07-14 10:50:09.000000 Coquille-1.1.1/LICENSE
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     5241 2023-07-16 09:04:01.549366 Coquille-1.1.1/PKG-INFO
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     3485 2023-07-16 09:02:18.000000 Coquille-1.1.1/README.md
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:04:01.539365 Coquille-1.1.1/examples/
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:04:01.542698 Coquille-1.1.1/examples/coquille_context/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      437 2023-07-14 10:50:09.000000 Coquille-1.1.1/examples/coquille_context/__main__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)    60903 2023-07-16 09:02:18.000000 Coquille-1.1.1/examples/coquille_context/screenshot.png
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:04:01.542698 Coquille-1.1.1/examples/coquille_write/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      196 2023-07-16 09:02:18.000000 Coquille-1.1.1/examples/coquille_write/__main__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)    39301 2023-07-16 09:02:18.000000 Coquille-1.1.1/examples/coquille_write/screenshot.png
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:04:01.546032 Coquille-1.1.1/examples/write/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      406 2023-07-16 09:02:18.000000 Coquille-1.1.1/examples/write/__main__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       45 2023-07-16 09:02:18.000000 Coquille-1.1.1/examples/write/output.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)    75317 2023-07-16 09:02:18.000000 Coquille-1.1.1/examples/write/screenshot.png
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      698 2023-07-16 09:02:43.000000 Coquille-1.1.1/pyproject.toml
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       38 2023-07-16 09:04:01.549366 Coquille-1.1.1/setup.cfg
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:04:01.539365 Coquille-1.1.1/src/
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:04:01.546032 Coquille-1.1.1/src/Coquille.egg-info/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     5241 2023-07-16 09:04:01.000000 Coquille-1.1.1/src/Coquille.egg-info/PKG-INFO
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      649 2023-07-16 09:04:01.000000 Coquille-1.1.1/src/Coquille.egg-info/SOURCES.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)        1 2023-07-16 09:04:01.000000 Coquille-1.1.1/src/Coquille.egg-info/dependency_links.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       35 2023-07-16 09:04:01.000000 Coquille-1.1.1/src/Coquille.egg-info/requires.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)        9 2023-07-16 09:04:01.000000 Coquille-1.1.1/src/Coquille.egg-info/top_level.txt
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:04:01.546032 Coquille-1.1.1/src/coquille/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       32 2023-07-14 10:50:09.000000 Coquille-1.1.1/src/coquille/__init__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     7667 2023-07-16 09:02:18.000000 Coquille-1.1.1/src/coquille/coquille.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)    10596 2023-07-14 10:50:09.000000 Coquille-1.1.1/src/coquille/sequences.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      392 2023-07-16 08:43:00.000000 Coquille-1.1.1/src/coquille/typeshed.py
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:04:01.546032 Coquille-1.1.1/tests/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:50:09.000000 Coquille-1.1.1/tests/__init__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     1081 2023-07-16 08:32:37.000000 Coquille-1.1.1/tests/coquille_test.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     4219 2023-07-14 10:50:09.000000 Coquille-1.1.1/tests/sequences_test.py
```

### Comparing `Coquille-1.0.2/.gitignore` & `Coquille-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.2/.pre-commit-config.yaml` & `Coquille-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.2/LICENSE` & `Coquille-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.2/PKG-INFO` & `Coquille-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Coquille
-Version: 1.0.2
+Version: 1.1.1
 Summary: Coquille is a library that wraps terminal escape sequences as convenient functions.
 Author: Qexat
 License: MIT License
         
         Copyright (c) 2023 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -97,26 +97,43 @@
 print("Oh, we are back to normal now...")
 ```
 
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_context/screenshot.png)
 
 Source code: [examples/coquille_context/](https://github.com/qexat/Coquille/blob/main/examples/coquille_context/__main__.py)
 
-### Coquille.write()
+### write()
 
 ```py
-from coquille import Coquille
+from coquille import write
 from coquille.sequences import bold, fg_blue, fg_magenta, italic
 
 print("Hello World!")
 
-Coquille.write("Hello World, but in magenta and italic!", fg_magenta, italic)
+write("Hello World, but in magenta and italic!", fg_magenta, italic)
+
+with open("examples/write/output.txt", "w") as my_file:
+    write("A pretty Hello World in a file!", fg_blue, bold, file=my_file)
+
+```
+
+![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/write/screenshot.png)
+
+Source code: [examples/write/](https://github.com/qexat/Coquille/blob/main/examples/write/__main__.py)
+
+### Coquille.write()
+
+```py
+from coquille import Coquille
+from coquille.sequences import fg_truecolor
+
+print("Normal Hello World!")
 
-with open("examples/coquille_write/output.txt", "w") as my_file:
-    Coquille.write("A pretty Hello World in a file!", fg_blue, bold, file=my_file)
+coquille = Coquille.new(fg_truecolor(128, 255, 0))
+coquille.write("Colorful Hello World!")
 
 ```
 
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_write/screenshot.png)
 
 Source code: [examples/coquille_write/](https://github.com/qexat/Coquille/blob/main/examples/coquille_write/__main__.py)
```

### Comparing `Coquille-1.0.2/README.md` & `Coquille-1.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -60,26 +60,43 @@
 print("Oh, we are back to normal now...")
 ```
 
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_context/screenshot.png)
 
 Source code: [examples/coquille_context/](https://github.com/qexat/Coquille/blob/main/examples/coquille_context/__main__.py)
 
-### Coquille.write()
+### write()
 
 ```py
-from coquille import Coquille
+from coquille import write
 from coquille.sequences import bold, fg_blue, fg_magenta, italic
 
 print("Hello World!")
 
-Coquille.write("Hello World, but in magenta and italic!", fg_magenta, italic)
+write("Hello World, but in magenta and italic!", fg_magenta, italic)
+
+with open("examples/write/output.txt", "w") as my_file:
+    write("A pretty Hello World in a file!", fg_blue, bold, file=my_file)
+
+```
+
+![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/write/screenshot.png)
+
+Source code: [examples/write/](https://github.com/qexat/Coquille/blob/main/examples/write/__main__.py)
+
+### Coquille.write()
+
+```py
+from coquille import Coquille
+from coquille.sequences import fg_truecolor
+
+print("Normal Hello World!")
 
-with open("examples/coquille_write/output.txt", "w") as my_file:
-    Coquille.write("A pretty Hello World in a file!", fg_blue, bold, file=my_file)
+coquille = Coquille.new(fg_truecolor(128, 255, 0))
+coquille.write("Colorful Hello World!")
 
 ```
 
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_write/screenshot.png)
 
 Source code: [examples/coquille_write/](https://github.com/qexat/Coquille/blob/main/examples/coquille_write/__main__.py)
```

### Comparing `Coquille-1.0.2/pyproject.toml` & `Coquille-1.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Coquille"
-version = "1.0.2"
+version = "1.1.1"
 authors = [{ name = "Qexat" }]
 description = "Coquille is a library that wraps terminal escape sequences as convenient functions."
 readme = "README.md"
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `Coquille-1.0.2/src/Coquille.egg-info/PKG-INFO` & `Coquille-1.1.1/src/Coquille.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Coquille
-Version: 1.0.2
+Version: 1.1.1
 Summary: Coquille is a library that wraps terminal escape sequences as convenient functions.
 Author: Qexat
 License: MIT License
         
         Copyright (c) 2023 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -97,26 +97,43 @@
 print("Oh, we are back to normal now...")
 ```
 
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_context/screenshot.png)
 
 Source code: [examples/coquille_context/](https://github.com/qexat/Coquille/blob/main/examples/coquille_context/__main__.py)
 
-### Coquille.write()
+### write()
 
 ```py
-from coquille import Coquille
+from coquille import write
 from coquille.sequences import bold, fg_blue, fg_magenta, italic
 
 print("Hello World!")
 
-Coquille.write("Hello World, but in magenta and italic!", fg_magenta, italic)
+write("Hello World, but in magenta and italic!", fg_magenta, italic)
+
+with open("examples/write/output.txt", "w") as my_file:
+    write("A pretty Hello World in a file!", fg_blue, bold, file=my_file)
+
+```
+
+![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/write/screenshot.png)
+
+Source code: [examples/write/](https://github.com/qexat/Coquille/blob/main/examples/write/__main__.py)
+
+### Coquille.write()
+
+```py
+from coquille import Coquille
+from coquille.sequences import fg_truecolor
+
+print("Normal Hello World!")
 
-with open("examples/coquille_write/output.txt", "w") as my_file:
-    Coquille.write("A pretty Hello World in a file!", fg_blue, bold, file=my_file)
+coquille = Coquille.new(fg_truecolor(128, 255, 0))
+coquille.write("Colorful Hello World!")
 
 ```
 
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_write/screenshot.png)
 
 Source code: [examples/coquille_write/](https://github.com/qexat/Coquille/blob/main/examples/coquille_write/__main__.py)
```

### Comparing `Coquille-1.0.2/src/Coquille.egg-info/SOURCES.txt` & `Coquille-1.1.1/src/Coquille.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 .pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
 examples/coquille_context/__main__.py
 examples/coquille_context/screenshot.png
 examples/coquille_write/__main__.py
-examples/coquille_write/output.txt
 examples/coquille_write/screenshot.png
+examples/write/__main__.py
+examples/write/output.txt
+examples/write/screenshot.png
 src/Coquille.egg-info/PKG-INFO
 src/Coquille.egg-info/SOURCES.txt
 src/Coquille.egg-info/dependency_links.txt
 src/Coquille.egg-info/requires.txt
 src/Coquille.egg-info/top_level.txt
 src/coquille/__init__.py
 src/coquille/coquille.py
```

### Comparing `Coquille-1.0.2/src/coquille/coquille.py` & `Coquille-1.1.1/src/coquille/coquille.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # pyright: reportUnusedCallResult = false
 from __future__ import annotations
 
 import sys
+from abc import abstractmethod
 from collections.abc import Callable
 from dataclasses import dataclass
 from typing import overload
+from typing import Protocol
 from typing import TYPE_CHECKING
 
 from coquille.sequences import EscapeSequence
 from coquille.sequences import soft_reset
 
 __all__ = ["apply", "Coquille", "EscapeSequence", "prepare", "write"]
 
@@ -84,42 +86,32 @@
     """
 
     string: EscapeSequence = prepare(sequence, *args, **kwargs)
     target = file or sys.stdout
     target.write(string)
 
 
-class _ContextCoquille:
-    __slots__ = ("__sequences", "__file")  # private slots
+class CoquilleLike(Protocol):
+    sequences: list[EscapeSequence]
+    file: SupportsWrite[str] | None
 
-    def __init__(
+    @abstractmethod
+    def print(
         self,
-        sequences: list[EscapeSequence],
-        file: SupportsWrite[str] | None,
+        *values: object,
+        sep: str | None = None,
+        end: str | None = "\n",
     ) -> None:
-        self.__sequences = sequences
-        self.__file = file
-
-    @property
-    def sequences(self) -> list[EscapeSequence]:
-        """
-        Read-only ; the base sequences that were applied at the
-        beginning of the `with` block. They are reset when the
-        block ends.
-        """
+        pass
 
-        return self.__sequences
 
-    @property
-    def file(self) -> SupportsWrite[str] | None:
-        """
-        Read-only ; the file where the sequences are printed in.
-        """
-
-        return self.__file
+@dataclass(slots=True)
+class _ContextCoquille:
+    sequences: list[EscapeSequence]
+    file: SupportsWrite[str] | None
 
     def apply(self, sequence: EscapeSequence) -> None:
         """
         Apply an escape sequence in the context manager of a Coquille
         in live.
 
         It is not added to the base `coquille.sequences`, but will still
@@ -149,15 +141,15 @@
         ```py
         >>> with Coquille.new(bold, fg_red, file=sys.stderr) as coquille:
         ...     # same as: print("My pretty error message", file=coquille.file)
         ...     coquille.print("My pretty error message")
         ```
         """
 
-        print(*values, sep=sep, end=end, file=self.file)
+        Coquille.print(self, *values, sep=sep, end=end)
 
 
 @dataclass(slots=True)
 class Coquille:
     sequences: list[EscapeSequence]
     file: SupportsWrite[str] | None
 
@@ -183,54 +175,74 @@
     ) -> Self:
         """
         Convenient constructor for a Coquille.
         """
 
         return cls(list(sequences), file)
 
-    @staticmethod
+    def print(
+        self: CoquilleLike,
+        *values: object,
+        sep: str | None = " ",
+        end: str | None = "\n",
+    ) -> None:
+        """
+        Convenient function to print in the same file as the coquille's one.
+
+        ## Example
+
+        ```py
+        >>> my_coquille = Coquille.new(bold, fg_red, file=sys.stderr)
+        >>> # same as: print("My pretty error message", file=my_coquille.file)
+        >>> my_coquille.print("My pretty error message")
+        ```
+        """
+
+        for sequence in self.sequences:
+            apply(sequence, self.file)
+
+        print(*values, sep=sep, end=end, file=self.file)
+        apply(soft_reset)
+
     def write(
+        self,
         text: str,
-        *sequences: EscapeSequence,
         end: str | None = "\n",
-        file: SupportsWrite[str] | None = None,
     ) -> None:
         """
-        A function relatively similar to built-in `print`, but with
-        support of escape sequences that are prepended to the printed
-        text.
+        A function relatively similar to built-in `print`.
+        It is the same as naked `write`, but it uses the coquille's
+        registered sequences.
 
         Example:
         ```py
+        >>> from coquille import Coquille
         >>> from coquille.sequences import fg_magenta, italic
-        >>> Coquille.write("Hello World!", fg_magenta, italic)
+        >>> my_coquille = Coquille.new(fg_magenta, italic)
+        >>> my_coquille.write("Hello World!")
         Hello World!
         ```
         Here, "Hello World!" is printed in italic and magenta, but this
         cannot be reproduced exactly in docstrings.
 
-        The previous example is roughly the same as doing:
+        The previous example is roughly equivalent to:
         ```py
         >>> print("\x1b[35m", end="")
         >>> print("\x1b[3m", end="")
         >>> print("Hello World!")
         >>> print("\x1b[!p", end="")
         ```
 
         Note that the soft reset sequence is used rather than SGR reset `x1b[0m`,
         because the range of allowed escape sequences is larger than SGR.
         """
 
-        for sequence in sequences:
-            apply(sequence, file)
+        self.print(text, end=end)
 
-        print(text, end=end, file=file)
-        apply(soft_reset)
-
-    def __enter__(self):
+    def __enter__(self) -> _ContextCoquille:
         """
         Set up a context for a Coquille.
 
         The returned object is actually of a different type ;
         this is for convenience, allowing to have methods that
         only make sense inside the `with` block, such as `coquille.reset()`.
         """
@@ -246,8 +258,44 @@
 
         Soft reset the escape sequences applied since then.
         """
 
         apply(soft_reset, self.file)
 
 
-write = Coquille.write
+def write(
+    text: str,
+    *sequences: EscapeSequence,
+    end: str | None = "\n",
+    file: SupportsWrite[str] | None = None,
+) -> None:
+    """
+    A function relatively similar to built-in `print`, but with
+    support of escape sequences that are prepended to the printed
+    text.
+
+    Example:
+    ```py
+    >>> from coquille.sequences import fg_magenta, italic
+    >>> Coquille.write("Hello World!", fg_magenta, italic)
+    Hello World!
+    ```
+    Here, "Hello World!" is printed in italic and magenta, but this
+    cannot be reproduced exactly in docstrings.
+
+    The previous example is roughly the same as doing:
+    ```py
+    >>> print("\x1b[35m", end="")
+    >>> print("\x1b[3m", end="")
+    >>> print("Hello World!")
+    >>> print("\x1b[!p", end="")
+    ```
+
+    Note that the soft reset sequence is used rather than SGR reset `x1b[0m`,
+    because the range of allowed escape sequences is larger than SGR.
+    """
+
+    for sequence in sequences:
+        apply(sequence, file)
+
+    print(text, end=end, file=file)
+    apply(soft_reset)
```

### Comparing `Coquille-1.0.2/src/coquille/sequences.py` & `Coquille-1.1.1/src/coquille/sequences.py`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.2/tests/coquille_test.py` & `Coquille-1.1.1/tests/coquille_test.py`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.2/tests/sequences_test.py` & `Coquille-1.1.1/tests/sequences_test.py`

 * *Files identical despite different names*

