# Comparing `tmp/terminal_in_colors-0.1.0.tar.gz` & `tmp/terminal_in_colors-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_in_colors-0.1.0.tar", max compression
+gzip compressed data, was "terminal_in_colors-0.1.1.tar", max compression
```

## Comparing `terminal_in_colors-0.1.0.tar` & `terminal_in_colors-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-07-14 14:19:04.692727 terminal_in_colors-0.1.0/LICENSE
--rw-r--r--   0        0        0      981 2023-07-14 16:10:24.055806 terminal_in_colors-0.1.0/README.md
--rw-r--r--   0        0        0      851 2023-07-14 16:27:44.723542 terminal_in_colors-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     9947 2023-07-14 15:15:56.733777 terminal_in_colors-0.1.0/terminal_in_colors/ColorTerminal.py
--rw-r--r--   0        0        0      222 2023-07-14 14:21:57.206266 terminal_in_colors-0.1.0/terminal_in_colors/__init__.py
--rw-r--r--   0        0        0     5690 2023-07-14 14:21:01.486902 terminal_in_colors-0.1.0/terminal_in_colors/info_colors.py
--rw-r--r--   0        0        0     1823 1970-01-01 00:00:00.000000 terminal_in_colors-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-14 14:19:04.692727 terminal_in_colors-0.1.1/LICENSE
+-rw-r--r--   0        0        0      995 2023-07-16 15:14:37.545461 terminal_in_colors-0.1.1/README.md
+-rw-r--r--   0        0        0      851 2023-07-16 15:14:44.972528 terminal_in_colors-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9947 2023-07-14 15:15:56.733777 terminal_in_colors-0.1.1/terminal_in_colors/ColorTerminal.py
+-rw-r--r--   0        0        0      222 2023-07-14 14:21:57.206266 terminal_in_colors-0.1.1/terminal_in_colors/__init__.py
+-rw-r--r--   0        0        0     5690 2023-07-14 14:21:01.486902 terminal_in_colors-0.1.1/terminal_in_colors/info_colors.py
+-rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 terminal_in_colors-0.1.1/PKG-INFO
```

### Comparing `terminal_in_colors-0.1.0/LICENSE` & `terminal_in_colors-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal_in_colors-0.1.0/README.md` & `terminal_in_colors-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # terminal-in-colors
 
 Give color to your terminal, using 256 colors or RGB, use bold, italic, underline, among others, in a simple and uncomplicated way.
 
+![](img.png)
+
 
 # Instalation
 
 You can install simply using a command, thank *PyPi*.
 
 ```bash
 $ pip install termina-in-colors
```

### Comparing `terminal_in_colors-0.1.0/pyproject.toml` & `terminal_in_colors-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "terminal-in-colors"
-version = "0.1.0"
+version = "0.1.1"
 description = "Your terminal in colors :D"
 authors = ["kurotom <55354389+kurotom@users.noreply.github.com>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/kurotom/terminal-in-colors.git"
 documentation = "https://kurotom.github.io/terminal_in_colors/"
 keywords = ["colors", "terminal", "color", "console"]
```

### Comparing `terminal_in_colors-0.1.0/terminal_in_colors/ColorTerminal.py` & `terminal_in_colors-0.1.1/terminal_in_colors/ColorTerminal.py`

 * *Files identical despite different names*

### Comparing `terminal_in_colors-0.1.0/terminal_in_colors/info_colors.py` & `terminal_in_colors-0.1.1/terminal_in_colors/info_colors.py`

 * *Files identical despite different names*

### Comparing `terminal_in_colors-0.1.0/PKG-INFO` & `terminal_in_colors-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-in-colors
-Version: 0.1.0
+Version: 0.1.1
 Summary: Your terminal in colors :D
 Home-page: https://github.com/kurotom/terminal-in-colors.git
 License: LGPL-3.0-or-later
 Keywords: colors,terminal,color,console
 Author: kurotom
 Author-email: 55354389+kurotom@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
@@ -17,14 +17,16 @@
 Project-URL: Repository, https://github.com/kurotom/terminal-in-colors.git
 Description-Content-Type: text/markdown
 
 # terminal-in-colors
 
 Give color to your terminal, using 256 colors or RGB, use bold, italic, underline, among others, in a simple and uncomplicated way.
 
+![](img.png)
+
 
 # Instalation
 
 You can install simply using a command, thank *PyPi*.
 
 ```bash
 $ pip install termina-in-colors
```

