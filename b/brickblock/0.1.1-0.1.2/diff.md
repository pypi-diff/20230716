# Comparing `tmp/brickblock-0.1.1.tar.gz` & `tmp/brickblock-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brickblock-0.1.1.tar", max compression
+gzip compressed data, was "brickblock-0.1.2.tar", max compression
```

## Comparing `brickblock-0.1.1.tar` & `brickblock-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0    35823 2023-07-11 16:43:32.128481 brickblock-0.1.1/LICENSE
--rw-r--r--   0        0        0     2419 2023-07-12 12:20:04.956839 brickblock-0.1.1/README.md
--rw-r--r--   0        0        0       30 2023-07-12 12:12:23.190399 brickblock-0.1.1/brickblock/__init__.py
--rw-r--r--   0        0        0    17417 2023-07-12 12:12:23.182553 brickblock-0.1.1/brickblock/space.py
--rw-r--r--   0        0        0      446 2023-07-12 12:23:28.976727 brickblock-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2989 1970-01-01 00:00:00.000000 brickblock-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-07-15 07:40:33.964780 brickblock-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1383 2023-07-16 13:36:26.400650 brickblock-0.1.2/README.md
+-rw-r--r--   0        0        0       31 2023-07-15 12:28:30.690454 brickblock-0.1.2/brickblock/__init__.py
+-rw-r--r--   0        0        0    11331 2023-07-16 12:20:34.521456 brickblock-0.1.2/brickblock/objects.py
+-rw-r--r--   0        0        0     6835 2023-07-16 16:48:31.304526 brickblock-0.1.2/brickblock/space.py
+-rw-r--r--   0        0        0      535 2023-07-16 16:57:19.256623 brickblock-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 brickblock-0.1.2/setup.py
+-rw-r--r--   0        0        0     2075 1970-01-01 00:00:00.000000 brickblock-0.1.2/PKG-INFO
```

### Comparing `brickblock-0.1.1/LICENSE` & `brickblock-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brickblock-0.1.1/PKG-INFO` & `brickblock-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,40 @@
 Metadata-Version: 2.1
 Name: brickblock
-Version: 0.1.1
+Version: 0.1.2
 Summary: A fun visualisation library for those that like boxes
+Home-page: https://github.com/danielsoutar/brickblock
 Author: Daniel Soutar
 Author-email: danielsoutar144@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: pytest (>=7.4.0,<8.0.0)
+Project-URL: Repository, https://github.com/danielsoutar/brickblock
 Description-Content-Type: text/markdown
 
 # Brickblock: A fun visualisation library for those that like boxes
 
-This is a small library that uses blocks in matplotlib's visually appealing 3D extension - and aims to be the 'seaborn of matplotlib-3D', if you will.
+This is a small library that uses blocks in matplotlib's visually appealing 3D extension - and aims to be the 'seaborn of matplotlib-3D'.
 
 ## Core abstractions
 
-At the centre of BrickBlock is the `Space`. A `Space` contains objects, and when a user wants a visualisation, they render the current state of the `Space` - the rendered state is known as a `Scene`.
+At the centre of Brickblock is the `Space`. A `Space` represents a 3D cartesian coordinate space. It contains objects, and when a user wants a visualisation, they render the current state of the `Space` - the rendered state is known as a `Scene`.
 
-Currently there is one object used for composing visualisations in BrickBlock: the `Cube`. `Cube` objects can be added into the `Space` with a degree of control over their visual presentation: transparency, colour, line widths.
+There are objects used for composing visualisations in Brickblock, such as the `Cube`. `Cube` objects can be added into the `Space` with a degree of control over their visual presentation: transparency, colour, line widths.
 
-BrickBlock also supports `Transition`s and `Transform`s:
+Having these abstractions allows programmers to more easily create animated 3D visualisations, like GIFs. You define a `Space`, adding and mutating objects to evolve the state, and the `Scene` objects are persisted to enable sequences of images for use in GIFs.
 
-* A `Transform` is simply any change to the space like adding one or more `Cube` objects. It does not produce a `Scene`. These are useful when you are just iteratively building up to a complex `Scene`.
-* A `Transition`, by contrast, is a transform between two `Scene`s. These are useful for generating sequences of `Scene`s - the `Space` will keep track of its state over time, as well as which states are `Scene`s. A `Transition` can be defined by one or more `Transform`s.
+## Contributing
 
-Having these abstractions allows programmers to create animated visualisations like GIFs. You define a `Space`, using `Transform`s and `Transition`s to evolve the state, and the `Scene` objects are persisted to enable sequences of images for use in GIFs.
-
-```python
-import brickblock as bb
-
-
-# Let's start with adding a few objects to our space!
-cuboid_base = np.array((0, 0, 0))
-cuboid_dims = np.array((4, 3, 4))
-cuboid_opts = {'color': None, 'alpha': 0}
-input_cube = bb.Cuboid(base, cuboid_dims, **cuboid_opts)
-
-filter_base = np.array((0, 0, 1))
-filter_dims = np.array((3, 3, 3))
-filter_opts = {'color': (1., 1., 0.5), 'alpha': 0.3, 'linewidths': 0.3}
-filter_cube = bb.Cube(filter_base, filter_dims, **filter_opts)
-
-s = bb.Space()
-# Add a 4x3x4 rectangular cuboid to the space.
-s = bb.add_transform(s, input_cube)
-# Add a 3x3x3 filter to the space with a single cube.
-s = bb.add_transform(s, filter_cube)
-
-# Render the state as a scene and use in a plot-like way...
-fig, ax = bb.render(s)
-# Or take a snapshot to indicate that this is a scene...
-state_history = bb.snapshot(s)
-# Do more stuff...
-# And then when you're ready, generate a GIF-like output...
-gif_filename = bb.stream(s, "gif", path_to_file))
-```
+Contributions are more than welcome! There is a very rough TODO in `todo.md` that outlines both short- and long-term goals for the library. However, there are some rules:
+
+* Always follow the [code of conduct](CODE_OF_CONDUCT.md)
+* All the tests should be passing with your change
+* Explain your change (PR template coming soon)
+* Add relevant tests and docstrings
+* Format your changes with `black`
```

