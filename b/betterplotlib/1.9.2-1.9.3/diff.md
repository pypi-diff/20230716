# Comparing `tmp/betterplotlib-1.9.2.tar.gz` & `tmp/betterplotlib-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterplotlib-1.9.2.tar", last modified: Tue Dec  6 22:39:14 2022, max compression
+gzip compressed data, was "betterplotlib-1.9.3.tar", last modified: Tue Dec  6 22:59:55 2022, max compression
```

## Comparing `betterplotlib-1.9.2.tar` & `betterplotlib-1.9.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 22:39:14.532092 betterplotlib-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-06 22:39:03.000000 betterplotlib-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2022-12-06 22:39:14.528092 betterplotlib-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2022-12-06 22:39:03.000000 betterplotlib-1.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 22:39:14.528092 betterplotlib-1.9.2/betterplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2022-12-06 22:39:03.000000 betterplotlib-1.9.2/betterplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2022-12-06 22:39:03.000000 betterplotlib-1.9.2/betterplotlib/_generate_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    62525 2022-12-06 22:39:03.000000 betterplotlib-1.9.2/betterplotlib/_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)   101756 2022-12-06 22:39:03.000000 betterplotlib-1.9.2/betterplotlib/axes_bpl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2022-12-06 22:39:03.000000 betterplotlib-1.9.2/betterplotlib/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2022-12-06 22:39:03.000000 betterplotlib-1.9.2/betterplotlib/manage_axes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2022-12-06 22:39:03.000000 betterplotlib-1.9.2/betterplotlib/styles.py
--rw-r--r--   0 runner    (1001) docker     (123)    29613 2022-12-06 22:39:03.000000 betterplotlib-1.9.2/betterplotlib/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2022-12-06 22:39:03.000000 betterplotlib-1.9.2/betterplotlib/type_checking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 22:39:14.528092 betterplotlib-1.9.2/betterplotlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2022-12-06 22:39:14.000000 betterplotlib-1.9.2/betterplotlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2022-12-06 22:39:14.000000 betterplotlib-1.9.2/betterplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 22:39:14.000000 betterplotlib-1.9.2/betterplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-06 22:39:14.000000 betterplotlib-1.9.2/betterplotlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-06 22:39:14.000000 betterplotlib-1.9.2/betterplotlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      950 2022-12-06 22:39:03.000000 betterplotlib-1.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-06 22:39:14.532092 betterplotlib-1.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 22:59:55.981494 betterplotlib-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-06 22:59:48.000000 betterplotlib-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2022-12-06 22:59:55.981494 betterplotlib-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2022-12-06 22:59:48.000000 betterplotlib-1.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 22:59:55.981494 betterplotlib-1.9.3/betterplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2022-12-06 22:59:48.000000 betterplotlib-1.9.3/betterplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2022-12-06 22:59:48.000000 betterplotlib-1.9.3/betterplotlib/_generate_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62525 2022-12-06 22:59:48.000000 betterplotlib-1.9.3/betterplotlib/_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101643 2022-12-06 22:59:48.000000 betterplotlib-1.9.3/betterplotlib/axes_bpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2022-12-06 22:59:48.000000 betterplotlib-1.9.3/betterplotlib/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2022-12-06 22:59:48.000000 betterplotlib-1.9.3/betterplotlib/manage_axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2022-12-06 22:59:48.000000 betterplotlib-1.9.3/betterplotlib/styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29613 2022-12-06 22:59:48.000000 betterplotlib-1.9.3/betterplotlib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2022-12-06 22:59:48.000000 betterplotlib-1.9.3/betterplotlib/type_checking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 22:59:55.981494 betterplotlib-1.9.3/betterplotlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2022-12-06 22:59:55.000000 betterplotlib-1.9.3/betterplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2022-12-06 22:59:55.000000 betterplotlib-1.9.3/betterplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 22:59:55.000000 betterplotlib-1.9.3/betterplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-06 22:59:55.000000 betterplotlib-1.9.3/betterplotlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-06 22:59:55.000000 betterplotlib-1.9.3/betterplotlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2022-12-06 22:59:48.000000 betterplotlib-1.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-06 22:59:55.981494 betterplotlib-1.9.3/setup.cfg
```

### Comparing `betterplotlib-1.9.2/LICENSE` & `betterplotlib-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `betterplotlib-1.9.2/PKG-INFO` & `betterplotlib-1.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterplotlib
-Version: 1.9.2
+Version: 1.9.3
 Summary: Some wrappers for matplotlib to make plotting easier and nicer.
 Author-email: Gillen Brown <gillenbrown@gmail.com>
 License: MIT License
         
         Copyright (c) 2016 Gillen Brown
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `betterplotlib-1.9.2/betterplotlib/_generate_interface.py` & `betterplotlib-1.9.3/betterplotlib/_generate_interface.py`

 * *Files identical despite different names*

### Comparing `betterplotlib-1.9.2/betterplotlib/_interface.py` & `betterplotlib-1.9.3/betterplotlib/_interface.py`

 * *Files identical despite different names*

### Comparing `betterplotlib-1.9.2/betterplotlib/axes_bpl.py` & `betterplotlib-1.9.3/betterplotlib/axes_bpl.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,18 +207,16 @@
                 bpl.scatter(x + dx, y + dx)
             bpl.equal_scale()
 
         """
         # put x and y in args if they're not already there
         if len(args) == 0:
             args = kwargs.pop("x"), kwargs.pop("y")
-        # get the color, if it hasn't already been set. I don't need to do this
-        # in mpl 2.0 technically, but I do it anyway so I can use this color
-        # for the invisible label below.
-        if "color" not in kwargs and "c" not in kwargs:
+        # get the color, if it hasn't already been set
+        if "color" not in kwargs and "c" not in kwargs and "facecolor" not in kwargs:
             # get the default color cycle, and get the next color.
             kwargs["c"] = next(self._get_lines.prop_cycler)["color"]
 
         # set other parameters, if they haven't been set already
         # I use setdefault to do that, which puts the values in if they don't
         # already exist, but won't overwrite anything.
         # use the function we defined to get the proper alpha value.
```

### Comparing `betterplotlib-1.9.2/betterplotlib/colors.py` & `betterplotlib-1.9.3/betterplotlib/colors.py`

 * *Files identical despite different names*

### Comparing `betterplotlib-1.9.2/betterplotlib/manage_axes.py` & `betterplotlib-1.9.3/betterplotlib/manage_axes.py`

 * *Files identical despite different names*

### Comparing `betterplotlib-1.9.2/betterplotlib/styles.py` & `betterplotlib-1.9.3/betterplotlib/styles.py`

 * *Files identical despite different names*

### Comparing `betterplotlib-1.9.2/betterplotlib/tools.py` & `betterplotlib-1.9.3/betterplotlib/tools.py`

 * *Files identical despite different names*

### Comparing `betterplotlib-1.9.2/betterplotlib/type_checking.py` & `betterplotlib-1.9.3/betterplotlib/type_checking.py`

 * *Files identical despite different names*

### Comparing `betterplotlib-1.9.2/betterplotlib.egg-info/PKG-INFO` & `betterplotlib-1.9.3/betterplotlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterplotlib
-Version: 1.9.2
+Version: 1.9.3
 Summary: Some wrappers for matplotlib to make plotting easier and nicer.
 Author-email: Gillen Brown <gillenbrown@gmail.com>
 License: MIT License
         
         Copyright (c) 2016 Gillen Brown
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `betterplotlib-1.9.2/pyproject.toml` & `betterplotlib-1.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["betterplotlib"]
 
 [project]
 name = "betterplotlib"
-version = "1.9.2"
+version = "1.9.3"
 description = "Some wrappers for matplotlib to make plotting easier and nicer."
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     {name = "Gillen Brown", email="gillenbrown@gmail.com"},
 ]
 keywords = ["plotting", "matplotlib"]
```

