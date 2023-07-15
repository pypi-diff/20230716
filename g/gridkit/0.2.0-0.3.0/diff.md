# Comparing `tmp/gridkit-0.2.0.tar.gz` & `tmp/gridkit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridkit-0.2.0.tar", last modified: Sun Jul  9 22:22:54 2023, max compression
+gzip compressed data, was "gridkit-0.3.0.tar", last modified: Sat Jul 15 23:12:29 2023, max compression
```

## Comparing `gridkit-0.2.0.tar` & `gridkit-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:22:54.888889 gridkit-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-09 22:22:46.000000 gridkit-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-09 22:22:54.888889 gridkit-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-09 22:22:46.000000 gridkit-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:22:54.888889 gridkit-0.2.0/gridkit/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-09 22:22:46.000000 gridkit-0.2.0/gridkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-09 22:22:46.000000 gridkit-0.2.0/gridkit/_statistical_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-07-09 22:22:46.000000 gridkit-0.2.0/gridkit/base_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    20746 2023-07-09 22:22:46.000000 gridkit-0.2.0/gridkit/bounded_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-09 22:22:46.000000 gridkit-0.2.0/gridkit/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    27996 2023-07-09 22:22:46.000000 gridkit-0.2.0/gridkit/hex_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-09 22:22:46.000000 gridkit-0.2.0/gridkit/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    27382 2023-07-09 22:22:46.000000 gridkit-0.2.0/gridkit/rect_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 22:22:54.000000 gridkit-0.2.0/gridkit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:22:54.888889 gridkit-0.2.0/gridkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-09 22:22:54.000000 gridkit-0.2.0/gridkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-09 22:22:54.000000 gridkit-0.2.0/gridkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 22:22:54.000000 gridkit-0.2.0/gridkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-09 22:22:54.000000 gridkit-0.2.0/gridkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 22:22:54.000000 gridkit-0.2.0/gridkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 22:22:54.888889 gridkit-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-09 22:22:46.000000 gridkit-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:12:29.421086 gridkit-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 23:12:18.000000 gridkit-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-15 23:12:29.421086 gridkit-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-15 23:12:18.000000 gridkit-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:12:29.417086 gridkit-0.3.0/gridkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-15 23:12:18.000000 gridkit-0.3.0/gridkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-15 23:12:18.000000 gridkit-0.3.0/gridkit/_statistical_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16385 2023-07-15 23:12:18.000000 gridkit-0.3.0/gridkit/base_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26823 2023-07-15 23:12:18.000000 gridkit-0.3.0/gridkit/bounded_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-15 23:12:18.000000 gridkit-0.3.0/gridkit/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32572 2023-07-15 23:12:18.000000 gridkit-0.3.0/gridkit/hex_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-15 23:12:18.000000 gridkit-0.3.0/gridkit/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26464 2023-07-15 23:12:18.000000 gridkit-0.3.0/gridkit/rect_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 23:12:29.000000 gridkit-0.3.0/gridkit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 23:12:29.421086 gridkit-0.3.0/gridkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-15 23:12:29.000000 gridkit-0.3.0/gridkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-15 23:12:29.000000 gridkit-0.3.0/gridkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 23:12:29.000000 gridkit-0.3.0/gridkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-15 23:12:29.000000 gridkit-0.3.0/gridkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 23:12:29.000000 gridkit-0.3.0/gridkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 23:12:29.421086 gridkit-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-15 23:12:18.000000 gridkit-0.3.0/setup.py
```

### Comparing `gridkit-0.2.0/LICENSE.txt` & `gridkit-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gridkit-0.2.0/README.md` & `gridkit-0.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 GridKit
 =======
 
 GridKit is a tool to work with grids on a high abstraction level.
 
-[![Downloads](https://static.pepy.tech/personalized-badge/gridkit?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/gridkit)
-[![Downloads](https://badge.fury.io/py/gridkit.svg)](https://pypi.org/project/gridkit/)
+[![download stats: PePy](https://static.pepy.tech/personalized-badge/gridkit?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/gridkit)
+[![codecov](https://codecov.io/gh/tmillenaar/GridKit/branch/main/graph/badge.svg?token=23BKSMAHM1)](https://codecov.io/gh/tmillenaar/GridKit)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI](https://badge.fury.io/py/gridkit.svg)](https://pypi.org/project/gridkit/)
 
 Documentation
 =============
 Find the docs on [GitHub Pages](https://tmillenaar.github.io/GridKit).
 
 Examples
 ========
```

### Comparing `gridkit-0.2.0/gridkit/_statistical_functions.py` & `gridkit-0.3.0/gridkit/_statistical_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,74 @@
 import numpy
+
 from gridkit.errors import AlignmentError
 
+
 def _total_bounds(left_bounds, right_bounds):
     return (
         min(left_bounds[0], right_bounds[0]),
         min(left_bounds[1], right_bounds[1]),
         max(left_bounds[2], right_bounds[2]),
         max(left_bounds[3], right_bounds[3]),
     )
 
+
 def total_bounds(grids):
     if len(grids) == 1:
         return grids[0].bounds
 
-    combined_bounds =  grids[0].bounds
+    combined_bounds = grids[0].bounds
     for grid in grids[1:]:
         combined_bounds = _total_bounds(combined_bounds, grid.bounds)
     return combined_bounds
 
+
 def _empty_combined_grid(grids, value=numpy.nan):
     reference = grids[0]
     if not all([grid.is_aligned_with(reference)[0] for grid in grids[1:]]):
-        raise AlignmentError("Not all grids are aligned. Please `resample` all grids on the same grid.")
+        raise AlignmentError(
+            "Not all grids are aligned. Please `resample` all grids on the same grid."
+        )
 
     combined_bounds = total_bounds(grids)
-    combined_data = numpy.full( # data shape is y,x
+    combined_data = numpy.full(  # data shape is y,x
         (
-            round((combined_bounds[3]-combined_bounds[1])/reference.dy),
-            round((combined_bounds[2]-combined_bounds[0])/reference.dx)
+            round((combined_bounds[3] - combined_bounds[1]) / reference.dy),
+            round((combined_bounds[2] - combined_bounds[0]) / reference.dx),
         ),
         value,
-        dtype=float # Fixme: don't hardcode dtype. This if workaround for working with NaNs
+        dtype=float,  # Fixme: don't hardcode dtype. This if workaround for working with NaNs
     )
 
     return reference.__class__(combined_data, bounds=combined_bounds, crs=reference.crs)
 
+
 def count(grids):
     empty_grid = _empty_combined_grid(grids, value=0)
     combined_grid = empty_grid.copy()
     for grid in grids:
         if grid.nodata_value is None:
             value_ids = combined_grid.cells_in_bounds(grid.bounds)[0]
         else:
             value_ids = grid != grid.nodata_value
         numpy_ids = combined_grid.grid_id_to_numpy_id(value_ids.T)
         combined_grid._data[numpy_ids] += 1
     return combined_grid
 
+
 def sum(grids):
     empty_grid = _empty_combined_grid(grids, value=numpy.nan)
     combined_grid = empty_grid.copy()
-    for grid in grids: # add zero instead of NaN where there is coverage to allow adding
+    for (
+        grid
+    ) in grids:  # add zero instead of NaN where there is coverage to allow adding
         combined_grid.assign(0, bounds=grid.bounds, in_place=True)
-    empty_grid = _empty_combined_grid(grids, value=0) # TODO: add `replace` function
-    for grid in grids: # add the values
-        combined_grid += empty_grid.assign(grid.data, bounds=grid.bounds, in_place=False)
+    empty_grid = _empty_combined_grid(grids, value=0)  # TODO: add `replace` function
+    for grid in grids:  # add the values
+        combined_grid += empty_grid.assign(
+            grid.data, bounds=grid.bounds, in_place=False
+        )
     return combined_grid
 
+
 def mean(grids):
     return sum(grids) / count(grids)
```

### Comparing `gridkit-0.2.0/gridkit/base_grid.py` & `gridkit-0.3.0/gridkit/base_grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import abc
-import scipy
-import numpy
 import functools
-from pyproj import CRS, Transformer
-import shapely
-from collections.abc import Iterable
 import warnings
+from collections.abc import Iterable
 
-class BaseGrid(metaclass=abc.ABCMeta):
+import numpy
+import scipy
+import shapely
+from pyproj import CRS, Transformer
 
-    def __init__(self, offset=(0,0), crs=None):
 
+class BaseGrid(metaclass=abc.ABCMeta):
+    def __init__(self, offset=(0, 0), crs=None):
         # limit offset to be positive and max 1 cell-size
         offset_x, offset_y = offset[0], offset[1]
         offset_x = offset_x % self.dx
         offset_y = offset_y % self.dy
         self._offset = (offset_x, offset_y)
 
         # set the CRS using crs.setter
@@ -58,18 +58,19 @@
         pass
 
     @abc.abstractmethod
     def cells_near_point(self) -> float:
         pass
 
     @abc.abstractmethod
-    def relative_neighbours(self, depth=1, connect_corners=False, include_selected=False):
+    def relative_neighbours(
+        self, depth=1, connect_corners=False, include_selected=False
+    ):
         pass
 
-
     def neighbours(self, index, depth=1, connect_corners=False, include_selected=False):
         """The indices of the neighbouring cells.
         The argument 'depth' can be used to include cells from further away.
 
         Parameters
         ----------
         index: :class:`numpy.ndarray`
@@ -111,26 +112,31 @@
         --------
         :py:meth:`.RectGrid.relative_neighbours`
         :py:meth:`.HexGrid.relative_neighbours`
         """
         if not isinstance(index, numpy.ndarray):
             index = numpy.array(index)
 
-        neighbours = self.relative_neighbours(depth=depth, connect_corners=connect_corners, include_selected=include_selected, index=index)
+        neighbours = self.relative_neighbours(
+            depth=depth,
+            connect_corners=connect_corners,
+            include_selected=include_selected,
+            index=index,
+        )
 
         if len(index.shape) == 1:
             return neighbours + index
 
         # neighbours = numpy.repeat(neighbours[:, numpy.newaxis], len(index), axis=1)
         neighbours = numpy.swapaxes(neighbours, 0, 1)
         neighbours = neighbours + index
         return numpy.swapaxes(neighbours, 0, 1)
 
     @abc.abstractmethod
-    def cell_at_point(self, point: numpy.ndarray) -> tuple: 
+    def cell_at_point(self, point: numpy.ndarray) -> tuple:
         """Determine the ID of the cell in which `point` falls.
 
         Parameters
         ----------
         point: :class:`tuple`
             The coordinates of the point to which to match the cell
 
@@ -138,15 +144,17 @@
         -------
         :class:`tuple`
             The ID of the cell in (x,y)
         """
         pass
 
     @abc.abstractmethod
-    def cell_corners(self, index: numpy.ndarray, as_poly: bool = False) -> numpy.ndarray:
+    def cell_corners(
+        self, index: numpy.ndarray, as_poly: bool = False
+    ) -> numpy.ndarray:
         """Determine the corners of the cells as specified by `index`.
 
         Parameters
         ----------
         index: :class:`numpy.ndarray`
             The indices of the cells of interest. Each id contains an `x` and `y` value.
         as_poly: :class:`bool`
@@ -160,59 +168,63 @@
         pass
 
     @abc.abstractmethod
     def is_aligned_with(self, other):
         pass
 
     def to_crs(self, crs, resample_method="nearest"):
-        """Transforms the 
+        """Transforms the
 
         The ``crs`` attribute on the current GeometryArray must
         be set.  Either ``crs`` or ``epsg`` may be specified for output.
         This method will transform all points in all objects.  It has no notion
         or projecting entire geometries.  All segments joining points are
         assumed to be lines in the current projection, not geodesics.  Objects
         crossing the dateline (or other projection boundary) will have
         undesirable behavior.
-        
+
         Parameters
         ----------
         crs :class:`pyproj.CRS`
             The value can be anything accepted
             by :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
             such as an epsg integer (eg 4326), an authority string (eg "EPSG:4326") or a WKT string.
 
         Returns
         -------
-        
+
         """
         if self.crs is None:
             raise ValueError(
                 "Cannot transform naive grids.  "
                 "Please set a crs on the object first."
             )
-        
+
         crs = CRS.from_user_input(crs)
 
         # skip if the input CRS and output CRS are the exact same
         if self.crs.is_exact_same(crs):
             return self
 
         transformer = Transformer.from_crs(self.crs, crs, always_xy=True)
 
         new_offset = transformer.transform(*self.offset)
         point_start = transformer.transform(0, 0)
         point_end = transformer.transform(self.dx, self.dy)
         new_dx, new_dy = [end - start for (end, start) in zip(point_end, point_start)]
 
-        return self.parent_grid_class(dx=abs(new_dx), dy=abs(new_dy), offset=new_offset, crs=crs)
+        return self.parent_grid_class(
+            dx=abs(new_dx), dy=abs(new_dy), offset=new_offset, crs=crs
+        )
 
     @property
     def parent_grid(self):
-        return self.parent_grid_class(dx=self.dx, dy=self.dy, offset=self.offset, crs=self.crs)
+        return self.parent_grid_class(
+            dx=self.dx, dy=self.dy, offset=self.offset, crs=self.crs
+        )
 
     @abc.abstractproperty
     def parent_grid_class(self):
         pass
 
     def rotate(self) -> float:
         raise NotImplementedError()
@@ -226,25 +238,26 @@
     def to_vector_file(self) -> float:
         raise NotImplementedError()
 
     def aggregate(self) -> float:
         pass
 
     def are_bounds_aligned(self, bounds, separate=False):
-        is_aligned = lambda val, cellsize: numpy.isclose(val, 0) or numpy.isclose(val, cellsize)
+        is_aligned = lambda val, cellsize: numpy.isclose(val, 0) or numpy.isclose(
+            val, cellsize
+        )
         per_axis = (
-            is_aligned((bounds[0] - self.offset[0]) % self.dx, self.dx), # left
-            is_aligned((bounds[1] - self.offset[1]) % self.dy, self.dy), # bottom
-            is_aligned((bounds[2] - self.offset[0]) % self.dx, self.dx), # right
-            is_aligned((bounds[3] - self.offset[1]) % self.dy, self.dy)  # top
+            is_aligned((bounds[0] - self.offset[0]) % self.dx, self.dx),  # left
+            is_aligned((bounds[1] - self.offset[1]) % self.dy, self.dy),  # bottom
+            is_aligned((bounds[2] - self.offset[0]) % self.dx, self.dx),  # right
+            is_aligned((bounds[3] - self.offset[1]) % self.dy, self.dy),  # top
         )
         return per_axis if separate else numpy.all(per_axis)
 
     def align_bounds(self, bounds, mode="expand"):
-        
         if self.are_bounds_aligned(bounds):
             return bounds
 
         if mode == "expand":
             left_rounded = numpy.floor((bounds[0] - self.offset[0]) / self.dx)
             bottom_rounded = numpy.floor((bounds[1] - self.offset[1]) / self.dy)
             right_rounded = numpy.ceil((bounds[2] - self.offset[0]) / self.dx)
@@ -256,16 +269,18 @@
             top_rounded = numpy.floor((bounds[3] - self.offset[1]) / self.dy)
         elif mode == "nearest":
             left_rounded = round((bounds[0] - self.offset[0]) / self.dx)
             bottom_rounded = round((bounds[1] - self.offset[1]) / self.dy)
             right_rounded = round((bounds[2] - self.offset[0]) / self.dx)
             top_rounded = round((bounds[3] - self.offset[1]) / self.dy)
         else:
-            raise ValueError(f"mode = '{mode}' is not supported. Supported modes: ('expand', 'contract', 'nearest')")
-        
+            raise ValueError(
+                f"mode = '{mode}' is not supported. Supported modes: ('expand', 'contract', 'nearest')"
+            )
+
         return (
             left_rounded * self.dx + self.offset[0],
             bottom_rounded * self.dy + self.offset[1],
             right_rounded * self.dx + self.offset[0],
             top_rounded * self.dy + self.offset[1],
         )
 
@@ -282,35 +297,40 @@
                         yield geom
                 except:
                     yield geometry
 
         for geom in _geom_iterator():
             if isinstance(geom, shapely.geometry.Point):
                 if not suppress_point_warning:
-                    warnings.warn("Point type geometry detected. It is more efficient to use `cell_at_point` than to use `intersect_geometries` when dealing with points")
-                    suppress_point_warning=True # Only warn once per function call
+                    warnings.warn(
+                        "Point type geometry detected. It is more efficient to use `cell_at_point` than to use `intersect_geometries` when dealing with points"
+                    )
+                    suppress_point_warning = True  # Only warn once per function call
             geom_bounds = self.align_bounds(geom.bounds, mode="expand")
-            geom_bounds = ( # buffer bounds to be on the safe side
+            geom_bounds = (  # buffer bounds to be on the safe side
                 geom_bounds[0] - self.dx,
                 geom_bounds[1] - self.dy,
                 geom_bounds[2] + self.dx,
                 geom_bounds[3] + self.dy,
             )
             cells_in_bounds = self.cells_in_bounds(geom_bounds)[0]
-            if len(cells_in_bounds) == 0: # happens only if point or line lies on an edge
-                geom = geom.buffer(min(self.dx, self.dy) / 10) # buffer may never reach further then a single cell size
+            if (
+                len(cells_in_bounds) == 0
+            ):  # happens only if point or line lies on an edge
+                geom = geom.buffer(
+                    min(self.dx, self.dy) / 10
+                )  # buffer may never reach further then a single cell size
                 geom_bounds = self.align_bounds(geom.bounds, mode="expand")
                 cells_in_bounds = self.cells_in_bounds(geom_bounds)[0]
 
             cell_shapes = self.to_shapely(cells_in_bounds)
             mask = [geom.intersects(cell) for cell in cell_shapes]
             intersecting_cells.extend(cells_in_bounds[mask])
         return numpy.unique(intersecting_cells, axis=0)
 
-
     def to_shapely(self, index, as_multipolygon: bool = False):
         """Represent the cells as Shapely Polygons
 
         Parameters
         ----------
         index: :class:`numpy.ndarray`
             The indices of the cells to convert to Shapely Polygons
@@ -325,65 +345,89 @@
         index = numpy.array(index)
         if len(index.shape) == 1:
             index = numpy.expand_dims(index, 0)
         vertices = self.cell_corners(index)
         polygons = [shapely.geometry.Polygon(cell) for cell in vertices]
         return shapely.geometry.MultiPolygon(polygons) if as_multipolygon else polygons
 
-
-    def interp_from_points(self, points, values, method="linear", nodata_value=numpy.nan):
+    def interp_from_points(
+        self, points, values, method="linear", nodata_value=numpy.nan
+    ):
         """Interpolate the cells containing nodata, if they are inside the convex hull of cells that do contain data.
 
+        This function turns any set of points at arbitrary location into a regularly spaced :class:`.BoundedGrid`
+        that has the properties of the current :class:`.BaseGrid` (``self``).
+        :meth:`.BoundedGrid.interpolate` works in the other direction, where a values on a :class:`.BoundedGrid`
+        are sampled in order to obtain values at arbitrary location.
+
+        .. Note ::
+            This function is significantly slower than :meth:`.BoundedGrid.interpolate`
+
         Parameters
         ----------
         point: :class:`numpy.ndarray`
             A 2d numpy array containing the points in the form [[x1,y1], [x2,y2]]
         values: :class:`numpy.ndarray`
             The values corresponding to the supplied `points`, used as input for interpolation
         method: :class:`str`
             The interpolation method to be used. Options are ("nearest", "linear", "cubic"). Default: "linear".
 
         Returns
         -------
-        :class:`~gridkit.bounded_grid.BoundedGrid`
+        :class:`.BoundedGrid`
             A Bounded version of the supplied grid where the data is interpolated between the supplied points.
+
+        See also
+        --------
+        :py:meth:`.BoundedGrid.resample`
+        :py:meth:`.BoundedGrid.interpolate`
         """
         points = numpy.array(points)
         values = numpy.array(values)
 
         method_lut = dict(
-            nearest = scipy.interpolate.NearestNDInterpolator,
-            linear = functools.partial(scipy.interpolate.LinearNDInterpolator, fill_value=nodata_value),
-            cubic = functools.partial(scipy.interpolate.CloughTocher2DInterpolator, fill_value=nodata_value),
+            nearest=scipy.interpolate.NearestNDInterpolator,
+            linear=functools.partial(
+                scipy.interpolate.LinearNDInterpolator, fill_value=nodata_value
+            ),
+            cubic=functools.partial(
+                scipy.interpolate.CloughTocher2DInterpolator, fill_value=nodata_value
+            ),
         )
 
         if method not in method_lut:
-            raise ValueError(f"Method '{method}' is not supported. Supported methods: {method_lut.keys()}")
+            raise ValueError(
+                f"Method '{method}' is not supported. Supported methods: {method_lut.keys()}"
+            )
 
         coords = points.T
         bounds = (
             min(coords[0]),
             min(coords[1]),
             max(coords[0]),
             max(coords[1]),
         )
         aligned_bounds = self.align_bounds(bounds, mode="expand")
         ids, shape = self.cells_in_bounds(aligned_bounds)
-        interp_values = numpy.full(shape=shape, fill_value = nodata_value, dtype=values.dtype)
+        interp_values = numpy.full(
+            shape=shape, fill_value=nodata_value, dtype=values.dtype
+        )
 
         interp_func = method_lut[method]
         nodata_mask = values == nodata_value
 
         interpolator = interp_func(
             points[~nodata_mask],
             values[~nodata_mask],
         )
         centroids = self.centroid(ids)
 
         interp_values.ravel()[:] = interpolator(centroids)
         grid_kwargs = dict(
-            data=interp_values, bounds=aligned_bounds, crs=self.crs, nodata_value=nodata_value
+            data=interp_values,
+            bounds=aligned_bounds,
+            crs=self.crs,
+            nodata_value=nodata_value,
         )
         if hasattr(self, "_shape"):
             grid_kwargs["shape"] = self._shape
         return self.bounded_cls(**grid_kwargs)
-
```

### Comparing `gridkit-0.2.0/gridkit/bounded_grid.py` & `gridkit-0.3.0/gridkit/bounded_grid.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,44 @@
+import abc
+import functools
+import operator
+import warnings
 from multiprocessing.sharedctypes import Value
+from typing import Literal
+
 import numpy
 import scipy
-import operator
-import abc
-import warnings
-import functools
+from pyproj import Transformer
 
 import gridkit
 from gridkit.base_grid import BaseGrid
-from gridkit.errors import IntersectionError, AlignmentError
+from gridkit.errors import AlignmentError, IntersectionError
+
 
 class _BoundedGridMeta(type):
     """metaclass of the Raster class"""
 
     def __new__(cls, name, bases, namespace):
-
         # operators with a nan-base
         for op, as_idx in (
             (operator.mul, False),
             (operator.truediv, False),
             (operator.floordiv, False),
             (operator.pow, False),
             (operator.mod, False),
             (operator.ge, True),
             (operator.le, True),
             (operator.gt, True),
             (operator.lt, True),
         ):
             opname = "__{}__".format(op.__name__)
             opname_reversed = "__r{}__".format(op.__name__)
-            normal_op, reverse_op = cls._gen_operator(op, base_value=numpy.nan, as_idx=as_idx)
+            normal_op, reverse_op = cls._gen_operator(
+                op, base_value=numpy.nan, as_idx=as_idx
+            )
             namespace[opname] = normal_op
             namespace[opname_reversed] = reverse_op
 
         # treat equals and not-equals as special cases to acommodate NaNs
         op = functools.partial(numpy.isclose, equal_nan=True)
         normal_op, reverse_op = cls._gen_operator(op, base_value=numpy.nan, as_idx=True)
         namespace["__eq__"] = normal_op
@@ -91,167 +96,214 @@
         Raises
         ------
         NotImplementedError
             For grids of different sizes
         """
 
         def _grid_op(left, right, op, base_value):
-
             if not isinstance(right, BoundedGrid):
                 data = op(left._data, right)
                 if left.nodata_value is not None:
                     mask = left._data == left.nodata_value
                     data[mask] = left.nodata_value
                 return left.__class__(data, bounds=left.bounds, crs=left.crs)
 
             if not left.intersects(right):
-                raise AlignmentError("Operation not allowed on grids that do not overlap.") # TODO rethink errors. Do we want an out of bounds error?
-            
+                raise AlignmentError(
+                    "Operation not allowed on grids that do not overlap."
+                )  # TODO rethink errors. Do we want an out of bounds error?
+
             aligned, reason = left.is_aligned_with(right)
             if not aligned:
                 raise AlignmentError(f"Grids are not aligned. {reason}")
 
             # determine the dtype and nodata_value for the new grid, based on numpy casting rules
             def dominant_dtype_and_nodata_value(*grids):
                 dtypes = [grid._data.dtype for grid in grids]
                 dtype = numpy.result_type(*dtypes)
-                
+
                 nodata_values = [grid.nodata_value for grid in grids]
                 if all([val == nodata_values[0] for val in nodata_values]):
                     nodata_value = nodata_values[0]
                 elif all([val is not None for val in nodata_values]):
                     nodata_value = nodata_values[0]
-                    warnings.warn(f"Two grids have different `nodata_value`s: {nodata_values}. Using {nodata_value} for the resulting grid.")
+                    warnings.warn(
+                        f"Two grids have different `nodata_value`s: {nodata_values}. Using {nodata_value} for the resulting grid."
+                    )
                 elif all([val is None for val in nodata_values]):
                     nodata_value = None
-                    warnings.warn(f"No `nodata_value` was set on any of the grids. Any potential nodata gaps are filled with `{dtype.type(0)}`. Set a nodata_value by assigning a value to grid.nodata_value.")
-                else: # one but not all grids have a nodata_value set
+                    warnings.warn(
+                        f"No `nodata_value` was set on any of the grids. Any potential nodata gaps are filled with `{dtype.type(0)}`. Set a nodata_value by assigning a value to grid.nodata_value."
+                    )
+                else:  # one but not all grids have a nodata_value set
                     for val in nodata_values:
                         if val is not None:
                             nodata_value = val
                             break
                     else:
-                        raise ValueError("Oops, something unexpected went wrong when determining the new nodata_value. To resolve this you could try setting the `nodata_value` attribute of your grids.")
+                        raise ValueError(
+                            "Oops, something unexpected went wrong when determining the new nodata_value. To resolve this you could try setting the `nodata_value` attribute of your grids."
+                        )
                 return dtype, nodata_value
+
             dtype, nodata_value = dominant_dtype_and_nodata_value(left, right)
-            
+
             # create combined grid, spanning both inputs
             combined_bounds = left.combined_bounds(right)
             combined_data = numpy.full(
-                ( # data shape is y,x
-                    round((combined_bounds[3]-combined_bounds[1])/left.dy),
-                    round((combined_bounds[2]-combined_bounds[0])/left.dx)
+                (  # data shape is y,x
+                    round((combined_bounds[3] - combined_bounds[1]) / left.dy),
+                    round((combined_bounds[2] - combined_bounds[0]) / left.dx),
                 ),
                 fill_value=dtype.type(0) if nodata_value is None else nodata_value,
                 dtype=dtype,
             )
-            combined_grid = left.__class__(combined_data, bounds=combined_bounds, crs=left.crs, nodata_value=nodata_value)
+            combined_grid = left.__class__(
+                combined_data,
+                bounds=combined_bounds,
+                crs=left.crs,
+                nodata_value=nodata_value,
+            )
 
             shared_bounds = left.shared_bounds(right)
             left_shared = left.crop(shared_bounds)
             right_shared = right.crop(shared_bounds)
 
-            left_data = numpy.ma.masked_array(left_shared._data, left_shared.data==left_shared.nodata_value, dtype=dtype)
-            right_data = numpy.ma.masked_array(right_shared._data, right_shared.data==right_shared.nodata_value, dtype=dtype)
+            left_data = numpy.ma.masked_array(
+                left_shared._data,
+                left_shared.data == left_shared.nodata_value,
+                dtype=dtype,
+            )
+            right_data = numpy.ma.masked_array(
+                right_shared._data,
+                right_shared.data == right_shared.nodata_value,
+                dtype=dtype,
+            )
 
             result = op(left_data, right_data)
 
             # assign data of `left` to combined_grid
             left_data = left._data.astype(dtype)
             if left.nodata_value is not None:
                 left_data[left._data == left.nodata_value] = nodata_value
-            combined_grid.assign(left_data, bounds=left.bounds, in_place=True, assign_nodata=False)
+            combined_grid.assign(
+                left_data, bounds=left.bounds, in_place=True, assign_nodata=False
+            )
 
             # assign data of `right` to combined_grid
             right_data = right._data.astype(dtype)
             if right.nodata_value is not None:
                 right_data[right._data == right.nodata_value] = nodata_value
-            combined_grid.assign(right_data, bounds=right.bounds, in_place=True, assign_nodata=False)
+            combined_grid.assign(
+                right_data, bounds=right.bounds, in_place=True, assign_nodata=False
+            )
 
             # overwrite shared area in combined_grid with the combined results
             count = gridkit.count([left, right])
             shared_mask = count == 2
             shared_mask_np = combined_grid.grid_id_to_numpy_id(shared_mask.T)
             result = op(left.value(shared_mask), right.value(shared_mask))
-            combined_grid = combined_grid.astype(numpy.result_type(combined_grid._data.dtype, result.dtype)) # when dividing the dtype changes
-            combined_grid._data[shared_mask_np] = result # TODO: find more elegant way of updating data with grid ids as mask
+            combined_grid = combined_grid.astype(
+                numpy.result_type(combined_grid._data.dtype, result.dtype)
+            )  # when dividing the dtype changes
+            combined_grid._data[
+                shared_mask_np
+            ] = result  # TODO: find more elegant way of updating data with grid ids as mask
 
             return combined_grid
 
         def normal_op(left, right):
             if not isinstance(right, BoundedGrid):
                 data = op(left._data, right)
                 if left.nodata_value is not None:
                     nodata_np_id = numpy.where(left._data == left.nodata_value)
                     data[nodata_np_id] = left.nodata_value
                 grid = left.update(data)
             else:
                 grid = _grid_op(left, right, op, base_value=base_value)
-            return left._mask_to_index(grid._data) if as_idx else grid #TODO: left._mask_to_index(data) works if as_idx is true
+            return (
+                left._mask_to_index(grid._data) if as_idx else grid
+            )  # TODO: left._mask_to_index(data) works if as_idx is true
 
         def reverse_op(left, right):
             if not isinstance(right, BoundedGrid):
                 data = op(right, left._data)
                 if left.nodata_value is not None:
                     nodata_np_id = numpy.where(left._data == left.nodata_value)
                     data[nodata_np_id] = left.nodata_value
                 grid = left.update(data)
             else:
                 grid = _grid_op(left, right, op, base_value=base_value)
-            return grid._mask_to_index(grid._data) if as_idx else grid #TODO: left._mask_to_index(data) works if as_idx is true
+            return (
+                grid._mask_to_index(grid._data) if as_idx else grid
+            )  # TODO: left._mask_to_index(data) works if as_idx is true
 
         return normal_op, reverse_op
 
     @staticmethod
     def _gen_reduce_operator(op, as_idx=False):
         def internal(self, *args, **kwargs):
-
             data = self._data
             if not self.nodata_value is None:
-                data = numpy.ma.masked_array(data, numpy.isclose(data, self.nodata_value, equal_nan=True))
+                data = numpy.ma.masked_array(
+                    data, numpy.isclose(data, self.nodata_value, equal_nan=True)
+                )
             result = op(data, *args, **kwargs)
 
             if not as_idx:
                 return result
 
             # since `as_idx`=True, assume result is the id corresponding to the raveled array
             # TODO: put lines below in function self.numpy_id_to_grid_id or similar. Think of raveled vs xy input
             np_id_x = int(result % self.width)
             np_id_y = int(numpy.floor(result / self.width))
             left_top = self.corners[0]
-            left_top_id = self.cell_at_point(left_top + [self.dx / 2, - self.dy / 2])
+            left_top_id = self.cell_at_point(left_top + [self.dx / 2, -self.dy / 2])
             index = left_top_id + [np_id_x, -np_id_y]
             return index
 
         return internal
 
+
 class _AbstractBoundedGridMeta(abc.ABCMeta, _BoundedGridMeta):
     """Class that enables usage of the :class:`~gridkit.bounded_grid._BoundedGridMeta` metaclass despite using ABCMeta as metaclass for the parent class."""
-    pass
 
-class BoundedGrid(metaclass=_AbstractBoundedGridMeta):
+    pass
 
-    def __init__(self, data: numpy.ndarray, *args, bounds: tuple, nodata_value=None, prevent_copy: bool=False, **kwargs) -> None:
 
+class BoundedGrid(metaclass=_AbstractBoundedGridMeta):
+    def __init__(
+        self,
+        data: numpy.ndarray,
+        *args,
+        bounds: tuple,
+        nodata_value=None,
+        prevent_copy: bool = False,
+        **kwargs,
+    ) -> None:
         self._data = data if prevent_copy else data.copy()
         self._bounds = bounds
         self.nodata_value = nodata_value
         super(BoundedGrid, self).__init__(*args, **kwargs)
 
     @property
     def data(self):
         return self._data
 
     @data.setter
     def data(self, data):
         new_data = numpy.array(data)
         if new_data.dtype.name == "object":
-            raise TypeError(f"Data cannot be interpreted as a numpy.ndarray, got {type(data)}")
+            raise TypeError(
+                f"Data cannot be interpreted as a numpy.ndarray, got {type(data)}"
+            )
         if new_data.shape != self.data.shape:
-            raise ValueError(f"Cannot set data that is different in size. Expected a shape of {self.data.shape}, got {new_data.shape}.")
+            raise ValueError(
+                f"Cannot set data that is different in size. Expected a shape of {self.data.shape}, got {new_data.shape}."
+            )
         self._data = data
 
     def __array__(self, dtype=None):
         if dtype:
             return self.data.astype(dtype)
         return self.data
 
@@ -259,22 +311,24 @@
     def dtype(self):
         return self._data.dtype
 
     def astype(self, dtype):
         return self.update(new_data=self._data.astype(dtype))
 
     def update(self, new_data, bounds=None, crs=None, nodata_value=None):
-        #TODO figure out how to update dx, dy, origin
+        # TODO figure out how to update dx, dy, origin
         if not bounds:
             bounds = self.bounds
         if not crs:
             crs = self.crs
         if not nodata_value:
             nodata_value = self.nodata_value
-        return self.__class__(new_data, bounds=bounds, crs=crs, nodata_value=nodata_value)
+        return self.__class__(
+            new_data, bounds=bounds, crs=crs, nodata_value=nodata_value
+        )
 
     def copy(self):
         return self.update(self.data)
 
     @property
     def bounds(self) -> tuple:
         """Raster Bounds
@@ -297,20 +351,22 @@
         """
         b = self._bounds
         return (b[0], b[2], b[1], b[3])
 
     @property
     def corners(self):
         b = self.bounds
-        return numpy.array([
-            [b[0], b[3]], # left-top
-            [b[2], b[3]], # right-top
-            [b[2], b[1]], # right-bottom
-            [b[0], b[1]], # left-bottom
-        ])
+        return numpy.array(
+            [
+                [b[0], b[3]],  # left-top
+                [b[2], b[3]],  # right-top
+                [b[2], b[1]],  # right-bottom
+                [b[0], b[1]],  # left-bottom
+            ]
+        )
 
     @property
     def width(self):
         """Raster width
 
         Returns
         -------
@@ -342,35 +398,40 @@
         -------
         :class:`int`
             The total number of cells in the grid
         """
         return self.height * self.width
 
     def intersects(self, other):
-        other_bounds = other.bounds if isinstance(other, BaseGrid) else other # Allow for both grid objects and bounds
+        other_bounds = (
+            other.bounds if isinstance(other, BaseGrid) else other
+        )  # Allow for both grid objects and bounds
         return not (
             self.bounds[0] >= other_bounds[2]
             or self.bounds[2] <= other_bounds[0]
             or self.bounds[1] >= other_bounds[3]
             or self.bounds[3] <= other_bounds[1]
         )
 
     def _mask_to_index(self, mask):
-
         if not self._data.shape == mask.shape:
-            raise ValueError(f"Mask shape {mask.shape} does not match data shape {self._data.shape}")
+            raise ValueError(
+                f"Mask shape {mask.shape} does not match data shape {self._data.shape}"
+            )
 
         ids, shape = self.cells_in_bounds(self.bounds)
         ids = ids.reshape([*shape, 2])
         return ids[mask]
 
     def shared_bounds(self, other):
         other_bounds = other.bounds if isinstance(other, BaseGrid) else other
         if not self.intersects(other):
-            raise IntersectionError(f"Grid with bounds {self.bounds} does not intersect with grid with bounds {other_bounds}.")
+            raise IntersectionError(
+                f"Grid with bounds {self.bounds} does not intersect with grid with bounds {other_bounds}."
+            )
         return (
             max(self.bounds[0], other_bounds[0]),
             max(self.bounds[1], other_bounds[1]),
             min(self.bounds[2], other_bounds[2]),
             min(self.bounds[3], other_bounds[3]),
         )
 
@@ -397,73 +458,85 @@
 
     @abc.abstractmethod
     def grid_id_to_numpy_id(self, index):
         pass
 
     @property
     def indices(self):
-        """Return the indices within the bounds of the data"""       
+        """Return the indices within the bounds of the data"""
         return self.cells_in_bounds(self.bounds)[0]
 
-    def assign(self, data, *, anchor=None, bounds=None, in_place=True, assign_nodata=True):
+    def assign(
+        self, data, *, anchor=None, bounds=None, in_place=True, assign_nodata=True
+    ):
         if not any([anchor, bounds]):
-            raise ValueError("Please supply either an 'anchor' or 'bounds' keyword to position the data in the grid.")
+            raise ValueError(
+                "Please supply either an 'anchor' or 'bounds' keyword to position the data in the grid."
+            )
         new_data = self.data if in_place else self.data.copy()
 
         if bounds:
             slice_y, slice_x = self._data_slice_from_bounds(bounds)
             crop = new_data[slice_y, slice_x]
             if not assign_nodata:
                 mask = data != self.nodata_value
                 crop[mask] = data[mask]
             else:
                 crop[:] = data
-        elif anchor: # a corner or center
+        elif anchor:  # a corner or center
             raise NotImplementedError()
         else:
             raise ValueError("Please supply one of: {anchor, bounds}")
 
         return self.__class__(new_data, bounds=self.bounds, crs=self.crs)
 
-    def value(self, index, oob_value = None):
+    def value(self, index, oob_value=None):
         """Return the value at the given cell index"""
 
-        # Convert grid-ids into numpy-ids
-        # Note: the (0,0) id for numpy refers to the top-left
         index = numpy.array(index)
-        index = index[numpy.newaxis, :] if len(index.shape) == 1  else index
-        left_top = self.corners[0]
-        left_top_id = self.cell_at_point(left_top + [self.dx / 2, - self.dy / 2])[:,numpy.newaxis]
-        index = index.T # TODO: maybe always work with xy axis first
-        np_id = numpy.empty_like(index)
-        np_id[0] = index[0] - left_top_id[0]
-        np_id[1] = left_top_id[1] - index[1]
+        index = index[numpy.newaxis, :] if len(index.shape) == 1 else index
+        index = index.T  # TODO: maybe always work with xy axis first
+
+        # Convert grid-ids into numpy-ids
+        np_id = numpy.stack(self.grid_id_to_numpy_id(index)[::-1])
 
         # Identify any id outside the bounds
         oob_mask = numpy.where(np_id[0] >= self._data.shape[1])
         oob_mask += numpy.where(np_id[0] < 0)
         oob_mask += numpy.where(np_id[1] >= self._data.shape[0])
         oob_mask += numpy.where(np_id[1] < 0)
         oob_mask = numpy.hstack(oob_mask)
 
-        if numpy.any(oob_mask): # make sure we know what nodata value to set if ids are out of bounds
+        if numpy.any(
+            oob_mask
+        ):  # make sure we know what nodata value to set if ids are out of bounds
             if oob_value is None and self.nodata_value is None:
-                raise ValueError("Some indices do not have data. Please remove these ids, set a 'nodata_value' or supply an 'oob_value'.")
+                raise ValueError(
+                    "Some indices do not have data. Please remove these ids, set a 'nodata_value' or supply an 'oob_value'."
+                )
             oob_value = oob_value if oob_value else self.nodata_value
         else:
-            oob_value = oob_value if oob_value else 0 # the oob_value does not matter if no ids are out of bounds
+            oob_value = (
+                oob_value if oob_value else 0
+            )  # the oob_value does not matter if no ids are out of bounds
 
         # Return array's `dtype` needs to be float instead of integer if an id falls outside of bounds
         # For NaNs don't make sense as integer
-        if numpy.any(oob_mask) and not numpy.isfinite(oob_value) and not numpy.issubdtype(self._data.dtype, float):
-            print(f"Warning: dtype `{self._data.dtype}` might not support an `oob_value` of `{oob_value}`.")
+        if (
+            numpy.any(oob_mask)
+            and not numpy.isfinite(oob_value)
+            and not numpy.issubdtype(self._data.dtype, float)
+        ):
+            print(
+                f"Warning: dtype `{self._data.dtype}` might not support an `oob_value` of `{oob_value}`."
+            )
 
         values = numpy.full(np_id.shape[1], oob_value, dtype=self._data.dtype)
 
-        sample_mask = numpy.ones_like(values, dtype='bool')
+        sample_mask = numpy.ones_like(values, dtype="bool")
         sample_mask[oob_mask] = False
 
         np_id = np_id[:, sample_mask]
         values[sample_mask] = self._data[np_id[1], np_id[0]]
 
         return values
 
@@ -489,24 +562,30 @@
 
         Returns
         -------
         :class:`tuple`
             A copy of the grid with interpolated values.
         """
         method_lut = dict(
-            nearest = scipy.interpolate.NearestNDInterpolator,
-            linear = functools.partial(scipy.interpolate.LinearNDInterpolator, fill_value=self.nodata_value),
-            cubic = scipy.interpolate.CloughTocher2DInterpolator,
+            nearest=scipy.interpolate.NearestNDInterpolator,
+            linear=functools.partial(
+                scipy.interpolate.LinearNDInterpolator, fill_value=self.nodata_value
+            ),
+            cubic=scipy.interpolate.CloughTocher2DInterpolator,
         )
 
         if self.nodata_value is None:
-            raise ValueError(f"Cannot interpolate nodata values if attribute 'nodata_value' is not set.")
+            raise ValueError(
+                f"Cannot interpolate nodata values if attribute 'nodata_value' is not set."
+            )
 
         if method not in method_lut:
-            raise ValueError(f"Method '{method}' is not supported. Supported methods: {method_lut.keys()}")
+            raise ValueError(
+                f"Method '{method}' is not supported. Supported methods: {method_lut.keys()}"
+            )
 
         if not in_place:
             self = self.copy()
 
         interp_func = method_lut[method]
         values = self.data.ravel()
         nodata_mask = values == self.nodata_value
@@ -515,7 +594,124 @@
             points[~nodata_mask],
             values[~nodata_mask],
         )
         filled_values = interpolator(points[nodata_mask])
         self.data.ravel()[nodata_mask] = filled_values
         return self
 
+    def interpolate(self, sample_points, method="nearest"):
+        """Interpolate the value at the location of ``sample_points``.
+
+        Points that are outside of the bounds of the data are assigned `self.nodata_value`, or 'NaN' if no nodata value is set.
+
+        Parameters
+        ----------
+        sample_points: :class:`numpy.ndarray`
+            The coordinates of the points at which to sample the data
+        method: :class:`str`, `'nearest', 'bilinear'`, optional
+            The interpolation method used to determine the value at the supplied `sample_points`.
+            Supported methods:
+            - "nearest", for nearest neigbour interpolation, effectively sampling the value of the data cell containing the point
+            - "bilinear", linear interpolation using the four cells surrounding the point
+            Default: "nearest"
+
+        Returns
+        -------
+        :class:`numpy.ndarray`
+            The interpolated values at the supplied points
+
+        See also
+        --------
+        :py:meth:`.BoundedGrid.resample`
+        :py:meth:`.BaseGrid.interp_from_points`
+        """
+        if method == "nearest":
+            new_ids = self.cell_at_point(sample_points)
+            return self.value(new_ids)
+        elif method == "bilinear" or method == "linear":
+            return self._bilinear_interpolation(sample_points)
+        raise ValueError(f"Resampling method '{method}' is not supported.")
+
+    def resample(self, alignment_grid, method="nearest"):
+        """Resample the grid onto another grid.
+        This will take the locations of the grid cells of the other grid (here called ``alignment_grid``)
+        and determine the value on these location based on the values of the original grid (``self``).
+
+        The steps are as follows:
+         1. Transform the bounds of the original data to the CRS of the alignment grid (if not already the same)
+            No transformation is done if any of the grids has no CRS set.
+         2. Find the cells of the alignment grid within these transformed bounds
+         3. Find the cells of the original grid that are nearby each of the centroids of the cells found in 2.
+            How many nearby cells are selected depends on the selected ``method``
+         4. Interpolate the values using the supplied ``method`` at each of the centroids of the alignment grid cells selected in 2.
+         5. Create a new bounded grid using the attributes of the alignment grid
+
+        Parameters
+        ----------
+        alignment_grid: :class:`BaseGrid`
+            The grid with the desired attributes on which to resample.
+
+        method: :class:`str`, `'nearest', 'bilinear'`, optional
+            The interpolation method used to determine the value at the supplied `sample_points`.
+            Supported methods:
+            - "nearest", for nearest neigbour interpolation, effectively sampling the value of the data cell containing the point
+            - "bilinear", linear interpolation using the four cells surrounding the point
+            Default: "nearest"
+
+        Returns
+        -------
+        :class:`.BoundedGrid`
+            The interpolated values at the supplied points
+
+        See also
+        --------
+        :py:meth:`.BoundedGrid.interpolate`
+        :py:meth:`.BaseGrid.interp_from_points`
+        """
+        if self.crs is None or alignment_grid.crs is None:
+            warnings.warn(
+                "`crs` not set for one or both grids. Assuming both grids have an identical CRS."
+            )
+            different_crs = False
+        else:
+            different_crs = not self.crs.is_exact_same(alignment_grid.crs)
+
+        # make sure the bounds align with the grid
+        if different_crs:
+            transformer = Transformer.from_crs(
+                self.crs, alignment_grid.crs, always_xy=True
+            )
+            bounds = transformer.transform_bounds(*self.bounds)
+        else:
+            bounds = self.bounds
+
+        # Align using "contract" for we cannot sample outside of the original bounds
+        new_bounds = alignment_grid.align_bounds(bounds, mode="contract")
+
+        new_ids, new_shape = alignment_grid.cells_in_bounds(bounds=new_bounds)
+
+        new_points = alignment_grid.centroid(new_ids)
+
+        if different_crs:
+            transformer = Transformer.from_crs(
+                alignment_grid.crs, self.crs, always_xy=True
+            )
+            transformed_points = transformer.transform(*new_points.T)
+            new_points = numpy.vstack(transformed_points).T
+
+        value = self.interpolate(new_points, method=method)
+        value = value.reshape(new_shape)
+
+        nodata_value = self.nodata_value if self.nodata_value is not None else numpy.nan
+
+        grid_kwargs = dict(
+            data=value,
+            bounds=new_bounds,
+            crs=alignment_grid.crs,
+            nodata_value=nodata_value,
+        )
+        if hasattr(alignment_grid, "_shape"):
+            grid_kwargs["shape"] = alignment_grid._shape
+
+        new_grid = alignment_grid.bounded_cls(**grid_kwargs)
+
+        return new_grid
```

### Comparing `gridkit-0.2.0/gridkit/hex_grid.py` & `gridkit-0.3.0/gridkit/rect_grid.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,198 +1,150 @@
-from gridkit.base_grid import BaseGrid
-from gridkit.bounded_grid import BoundedGrid
-from gridkit.rect_grid import RectGrid
-from gridkit.errors import IntersectionError, AlignmentError
+import warnings
 
 import numpy
-import warnings
+import scipy
 from pyproj import CRS, Transformer
 
-class HexGrid(BaseGrid):
+from gridkit.base_grid import BaseGrid
+from gridkit.bounded_grid import BoundedGrid
+from gridkit.errors import AlignmentError, IntersectionError
 
-    def __init__(self, *args, size, shape="pointy", **kwargs):
-        
-        self._size = size
-        self._radius = size / 3**0.5
-        
-        if shape == "pointy":
-            self._dx = size
-            self._dy = 3/2 * self._radius
-        elif shape == "flat":
-            self._dy = size
-            self._dx = 3/2 * self._radius
-        else:
-            raise ValueError(f"A HexGrid's `shape` can either be 'pointy' or 'flat', got '{shape}'")
-        
-        self._shape = shape
-        self.bounded_cls = BoundedHexGrid
-        super(HexGrid, self).__init__(*args, **kwargs)
+
+class RectGrid(BaseGrid):
+    def __init__(self, *args, dx, dy, **kwargs):
+        self.__dx = dx
+        self.__dy = dy
+        self.bounded_cls = BoundedRectGrid
+        super(RectGrid, self).__init__(*args, **kwargs)
 
     @property
     def dx(self) -> float:
-        """The spacing between cell centers in x-direction
-        """
-        return self._dx
+        """The cellsize in x-direction"""
+        return self.__dx
 
     @property
     def dy(self) -> float:
-        """The spacing between cell centers in y-direction
-        """
-        return self._dy
-    
-    @property
-    def r(self) -> float:
-        """The radius of the cell. The radius is defined to be the distance from the cell center to a cell corner.
-        """
-        return self._radius
-    
-    @property
-    def shape(self) -> str:
-        """The shape of the grid as supplied when initiating the class.
-        This can be either "flat" or "pointy" referring to the top of the cells.
-        """
-        return self._shape
+        """The cellsize in y-direction"""
+        return self.__dy
 
-    @property
-    def size(self) -> float:
-        """The size of the cell as supplied when initiating the class.
-        This is the same as dx for a flat grid and the same as dy for a pointy grid.
-        """
-        return self._size
-    
-    def relative_neighbours(self, depth=1, *, index, include_selected=False, connect_corners=False) -> numpy.ndarray:
+    def relative_neighbours(
+        self, depth=1, connect_corners=False, include_selected=False, index=None
+    ):
         """The relative indices of the neighbouring cells.
 
         Parameters
         ----------
         depth: :class:`int` Default: 1
             Determines the number of neighbours that are returned.
             If `depth=1` the direct neighbours are returned.
             If `depth=2` the direct neighbours are returned, as well as the neighbours of these neighbours.
             `depth=3` returns yet another layer of neighbours, and so forth.
-        index: :class:`numpy.ndarray`
-            The index of the cell of which the relative neighbours are desired.
-            This is mostly relevant because in hexagonal grids the neighbouring indices differ
-            when dealing with odd or even indices.
         include_selected: :class:`bool` Default: False
             Whether to include the specified cell in the return array.
             Even though the specified cell can never be a neighbour of itself,
             this can be useful when for example a weighted average of the neighbours is desired
             in which case the cell itself often should also be included.
         connect_corners: :class:`bool` Default: False
             Whether to consider cells that touch corners but not sides as neighbours.
-            This is not relevant in hexagonal grids. It does nothing here.
-            See :py:meth:`.RectGrid.relative_neighbours`
+            If `connect_corners` is True, the 4 cells directly touching the cell are considered neighbours.
+            If `connect_corners` is True, the 8 cells surrounding the cell are considered neighbours.
+            This escalates in combination with `depth` where indices in a square shape around the cell are returned
+            when `connect_corners` is True, and indices in a diamond shape around the cell are returned when `connect_corners` is False.
+        index: :class:`numpy.ndarray`
+            The index is mostly relevant for hexagonal grids.
+            For a square grid the relative neighbours are independent on the location on the grid.
+            Here it is only used for the return length.
+            If 10 cells are supplied to `index`, the relative neighbours are returned 10 times.
+            This is to keep a consistent api between the two classes.
 
 
         Examples
         --------
         The direct neighbours of a cell can be returned by using depth=1, which is the default.
-        For hexagonal grids, the relative indices of the neighbours differs depending on the index.
-        There are two cases, neighbour indices for even colums and neighbour indices for odd columns,
-        in the case of a grid 'pointy' shape.
-        This works on rows if the grid has a 'flat' shape.
+        For square grids, the number of returned neighbours depends on whether `connect_corners` is True or False:
 
         .. code-block:: python
 
-            >>> from gridkit.hex_grid import HexGrid
-            >>> grid = HexGrid(size=3)
-            >>> grid.relative_neighbours(index=[0,0])
-            array([[-1,  1],
-                   [ 0,  1],
+            >>> from gridkit.rect_grid import RectGrid
+            >>> grid = RectGrid(dx=2, dy=3)
+            >>> grid.relative_neighbours()
+            array([[ 0,  1],
                    [-1,  0],
                    [ 1,  0],
-                   [-1, -1],
                    [ 0, -1]])
-            >>> grid.relative_neighbours(index=[0,1])
-            array([[ 0,  1],
+            >>> grid.relative_neighbours(connect_corners=True)
+            array([[-1,  1],
+                   [ 0,  1],
                    [ 1,  1],
                    [-1,  0],
                    [ 1,  0],
+                   [-1, -1],
                    [ 0, -1],
                    [ 1, -1]])
 
         ..
 
         By specifying `depth` we can include indirect neighbours from further away.
-        The number of neighbours increases with depth by a factor of `depth*6`.
-        So the 3rd element in the list will be `1*6 + 2*6 + 3*6 = 36`.
+        The number of neighbours increases with depth by a factor of `depth*4` or `depth*8` depending on `connect_corners` being True or False.
+        So the 3rd element in the list will be `1*4 + 2*4 + 3*4 = 24` if `connect_corners` is False.
+        And it will be `1*8 + 2*8 + 3*8 = 48` if `connect_corners` is True.
 
         .. code-block:: python
 
-            >>> [len(grid.relative_neighbours(index=[0,0], depth=depth)) for depth in range(1,5)]
-            [6, 18, 36, 60]
+            >>> [len(grid.relative_neighbours(depth=depth)) for depth in range(1,5)]
+            [4, 12, 24, 36]
+            >>> [len(grid.relative_neighbours(depth=depth, connect_corners=True)) for depth in range(1,5)]
+            [8, 24, 48, 80]
 
         ..
 
         The specified cell can be included if `include_selected` is set to True:
 
         .. code-block:: python
 
-            >>> grid.relative_neighbours(index=[0,0], include_selected=True)
-            array([[-1,  1],
-                   [ 0,  1],
+            >>> grid.relative_neighbours(include_selected=True)
+            array([[ 0,  1],
                    [-1,  0],
                    [ 0,  0],
                    [ 1,  0],
-                   [-1, -1],
                    [ 0, -1]])
 
         ..
 
         See also
         --------
         :py:meth:`.BaseGrid.neighbours`
-        :py:meth:`.RectGrid.relative_neighbours`
+        :py:meth:`.HexGrid.relative_neighbours`
         """
 
         if depth < 1:
             raise ValueError("'depth' cannot be lower than 1")
-        
-        index = numpy.array(index)
-        if len(index.shape) == 1:
-            index = index[numpy.newaxis]
-
-        nr_neighbours = sum(6*numpy.arange(1, depth+1)) + 1 # Add 1 for the first cell
-        nr_indices= len(index)
-        neighbours = numpy.empty((nr_indices, nr_neighbours, 2), dtype=int)
-        start_slice = 0
-        rows = range(depth, -1, -1)
-
-        # create top half of selection
-        for i, row in enumerate(rows): # loop from top row to bottom row
-            row_length = depth + i + 1
-            row_slice = slice(start_slice, start_slice+row_length)
-            max_val = int(numpy.floor(row_length/2))
-            if self._shape == "pointy":
-                pointy_axis = 1
-                flat_axis = 0
-            elif self._shape == "flat":
-                pointy_axis = 0
-                flat_axis = 1
-
-            if (i % 2 == 0) == (depth % 2 == 0):
-                neighbours[:, row_slice, flat_axis] = range(-max_val, max_val+1)
-            else:
-                odd_mask = index[:, pointy_axis] % 2 != 0
-                neighbours[odd_mask, row_slice, flat_axis] = range(-max_val+1, max_val+1)
-                neighbours[~odd_mask, row_slice, flat_axis] = range(-max_val, max_val)
-            neighbours[:, row_slice, pointy_axis] = row
-            start_slice += row_length
-
-        # mirror top half to bottom half (leaving the center row be)
-        neighbours[:, start_slice:] = neighbours[:, 0:start_slice - row_length][::-1]
-        neighbours[:, start_slice:, pointy_axis] *= -1
+
+        neighbours = numpy.empty(((2 * depth + 1) ** 2, 2), dtype=int)
+
+        relative_ids_1d = numpy.arange(-depth, depth + 1)
+        relative_x, relative_y = numpy.meshgrid(relative_ids_1d, relative_ids_1d[::-1])
+        neighbours[:, 0], neighbours[:, 1] = numpy.ravel(relative_x), numpy.ravel(
+            relative_y
+        )
+
+        if not connect_corners:
+            mask = abs(numpy.multiply(*neighbours.T)) < depth
+            neighbours = neighbours[mask]
 
         if include_selected is False:
-            center_cell = int(numpy.floor(neighbours.shape[1]/2))
-            neighbours = numpy.delete(neighbours, center_cell, 1)
+            center_cell = int(numpy.floor(len(neighbours) / 2))
+            neighbours = numpy.delete(neighbours, center_cell, 0)
 
-        return neighbours if len(neighbours) > 1 else neighbours[0]
+        if index is not None:
+            index = numpy.array(index)
+            if len(index.shape) == 2:
+                neighbours = numpy.repeat(neighbours[numpy.newaxis], len(index), axis=0)
 
+        return neighbours
 
     def centroid(self, index=None):
         """Coordinates at the center of the cell(s) specified by `index`.
 
         .. Warning ::
             The two values that make up an `index` are expected to be integers, and will be cast as such.
 
@@ -212,15 +164,15 @@
         Raises
         ------
         ValueError
             No `index` parameter was supplied. `index` can only be `None` in classes that contain data.
 
         Examples
         --------
-        Cell centers of single index are returned as an array with one dimention: 
+        Cell centers of single index are returned as an array with one dimention:
 
         .. code-block:: python
 
             >>> grid = RectGrid(dx=4, dy=1)
             >>> grid.centroid((0, 0))
             array([2. , 0.5])
             >>> grid.centroid((-1, -1))
@@ -250,32 +202,27 @@
             >>> grid.centroid((0, 0))
             array([3., 1.])
 
         ..
 
 
         """
-        
+
         if index is None:
-            raise ValueError("For grids that do not contain data, argument `index` is to be supplied to method `centroid`.")
+            raise ValueError(
+                "For grids that do not contain data, argument `index` is to be supplied to method `centroid`."
+            )
         index = numpy.array(index, dtype="int").T
         centroids = numpy.empty_like(index, dtype=float)
         centroids[0] = index[0] * self.dx + (self.dx / 2) + self.offset[0]
         centroids[1] = index[1] * self.dy + (self.dy / 2) + self.offset[1]
-
-        if self._shape == "pointy":
-            offset_rows = index[1] % 2 == 1
-            centroids[0, offset_rows] += self.dx/2
-        elif self._shape == "flat":
-            offset_rows = index[0] % 2 == 1
-            centroids[1, offset_rows] += self.dy/2
         return centroids.T
 
     def cells_near_point(self, point):
-        """Nearest 3 cells around a point.
+        """Nearest 4 cells around a point.
         This includes the cell the point is contained within,
         as well as two direct neighbours of this cell and one diagonal neighbor.
         What neigbors of the containing are slected, depends on where in the cell the point is located.
 
         Args
         ----
         point: :class"`tuple`
@@ -290,67 +237,81 @@
             If a single point is supplied, the four indices are returned as 1d arrays of length 2.
             If multiple points are supplied, the four indices are returned as Nx2 ndarrays.
 
         Examples
         --------
         Nearby cell indices are returned as a tuple:
 
+        .. code-block:: python
 
-        """
-        cell = self.cell_at_point(point)
-        centroid = self.centroid(cell)
-        distance_vector = point - centroid
-        azimuth = numpy.arctan2(*distance_vector.T) * 180 / numpy.pi
-
-        if len(cell.shape) == 1:
-            cell = numpy.expand_dims(cell, axis=0)
-
-        if self._shape == "flat":
-            inconsistent_axis = 0 # TODO: Make consistent and inconsisten axis a property of self
-            consistent_axis = 1
-            az_ranges = [(0,60), (60,120), (120,180), (-180,-120), (-120,-60), (-60,0)]
-            shift_odd_cells = [1, slice(1,3), 2, 1, slice(1,3), 2]
-            nearby_cells_relative_idx = [
-                [[1,0],[0,1]],
-                [[1,-1],[1,0]],
-                [[0,-1],[1,-1]],
-                [[-1,-1],[0,-1]],
-                [[-1,0],[-1,-1]],
-                [[0,1],[-1,0]],
-            ]
-        elif self._shape == "pointy":
-            inconsistent_axis = 1
-            consistent_axis = 0
-            azimuth += 30 # it is easier to work with ranges starting at 0 rather than -30
-            az_ranges = [(0,60), (60,120), (120,180), (180,210), (-120,-60), (-60,0)]
-            shift_odd_cells = [slice(1,3), 1, 2, slice(1,3), 1, 2]
-            nearby_cells_relative_idx = [
-                [[-1,1], [0,1]],
-                [[0,1],[1,0]],
-                [[1,0],[0,-1]],
-                [[0,-1],[-1,-1]],
-                [[-1,-1],[-1,0]],
-                [[-1,0],[-1,1]],
-            ]
-        else:
-            raise AttributeError(f"Unrecognized grid shape {self._shape}")
+            >>> grid = RectGrid(dx=4, dy=1)
+            >>> grid.cells_near_point((0, 0))
+            (array([-1,  0]), array([0, 0]), array([-1, -1]), array([ 0, -1]))
+            >>> grid.cells_near_point((3, 0.75))
+            (array([0, 1]), array([1, 1]), array([0, 0]), array([1, 0]))
+
+        ..
+
+        If multiple points are supplied, a tuple with ndarrays is returned:
+
+        .. code-block:: python
+
+            >>> points = [(0, 0), (3, 0.75), (3, 0)]
+            >>> nearby_cells = grid.cells_near_point(points)
+            >>> from pprint import pprint # used for output readability purposes only
+            >>> pprint(nearby_cells)
+            (array([[-1,  0],
+                   [ 0,  1],
+                   [ 0,  0]]),
+             array([[0, 0],
+                   [1, 1],
+                   [1, 0]]),
+             array([[-1, -1],
+                   [ 0,  0],
+                   [ 0, -1]]),
+             array([[ 0, -1],
+                   [ 1,  0],
+                   [ 1, -1]]))
+
+        ..
 
-        nearby_cells = numpy.repeat(numpy.expand_dims(cell, axis=0), 3, axis=0) # shape: neighbours(3), points(n), xy(2)
-        odd_cells_mask = cell[:, inconsistent_axis] % 2 == 1
-        
-        for az_range, shift_odd, cells in zip(az_ranges, shift_odd_cells, nearby_cells_relative_idx):
-            mask = numpy.logical_and(azimuth > az_range[0], azimuth <= az_range[1])
-            nearby_cells[1, mask] += cells[0]
-            nearby_cells[2, mask] += cells[1]
-            mask_odd = numpy.logical_and(mask, odd_cells_mask)
-            nearby_cells[shift_odd, mask_odd, consistent_axis] += 1
+        """
 
-        nearby_cells = numpy.swapaxes(nearby_cells, 0, 1)
-        return nearby_cells[0] if len(nearby_cells) == 1 else nearby_cells
+        # Split each cell into 4 quadrants in order to identify what 3 neigbors to select
+        new_grid = RectGrid(dx=self.dx / 2, dy=self.dy / 2, offset=self.offset)
+        ids = new_grid.cell_at_point(point).T
+        left_top_mask = numpy.logical_and(ids[0] % 2 == 0, ids[1] % 2 == 1)
+        right_top_mask = numpy.logical_and(ids[0] % 2 == 1, ids[1] % 2 == 1)
+        right_bottom_mask = numpy.logical_and(ids[0] % 2 == 1, ids[1] % 2 == 0)
+        left_bottom_mask = numpy.logical_and(ids[0] % 2 == 0, ids[1] % 2 == 0)
+
+        # obtain the bottom-left cell based on selected quadrant
+        base_ids = numpy.empty_like(ids, dtype="int")
+        # bottom-left if point in upper-right quadrant
+        base_ids[:, right_top_mask] = numpy.floor(ids[:, right_top_mask] / 2)
+        # bottom-left if point in bottom-right quadrant
+        base_ids[:, right_bottom_mask] = numpy.floor(ids[:, right_bottom_mask] / 2)
+        base_ids[1, right_bottom_mask] -= 1
+        # bottom-left if point in bottom-left quadrant
+        base_ids[:, left_bottom_mask] = numpy.floor(ids[:, left_bottom_mask] / 2)
+        base_ids[:, left_bottom_mask] -= 1
+        # bottom-left if point in upper-left qudrant
+        base_ids[:, left_top_mask] = numpy.floor(ids[:, left_top_mask] / 2)
+        base_ids[0, left_top_mask] -= 1
+
+        # use the bottom-left cell to determine the other three
+        bl_ids = base_ids.copy()
+        br_ids = base_ids.copy()
+        br_ids[0] += 1
+        tr_ids = base_ids.copy()
+        tr_ids += 1
+        tl_ids = base_ids.copy()
+        tl_ids[1] += 1
 
+        return tl_ids.T, tr_ids.T, bl_ids.T, br_ids.T
 
     def cell_at_point(self, point):
         """Index of the cell containing the supplied point(s).
 
         Parameters
         ----
         point: :class:`tuple`
@@ -361,321 +322,367 @@
         Returns
         -------
         :class:`numpy.ndarray`
             The index of the cell containing the point(s).
             If a single point is supplied, the index is returned as a 1d array of length 2.
             If multiple points are supplied, the indices are returned as Nx2 ndarrays.
 
-        """       
-        point = numpy.array(point)
-        point = numpy.expand_dims(point, axis=0).T if len(point.shape) == 1 else point.T
-
-        # approach adapted after https://stackoverflow.com/a/7714148
-        if self._shape == "pointy":
-            flat_axis = 0
-            pointy_axis = 1
-            flat_stepsize = self.dx
-            pointy_stepsize = self.dy
-        elif self._shape == "flat":
-            flat_axis = 1
-            pointy_axis = 0
-            flat_stepsize = self.dy
-            pointy_stepsize = self.dx
-        else:
-            raise ValueError(f"A HexGrid's `shape` can either be 'pointy' or 'flat', got '{self._shape}'")
+        Examples
+        --------
+
+        .. code-block:: python
+
+            >>> grid = RectGrid(dx=4, dy=1)
+            >>> grid.cell_at_point((1, 0))
+            array([0, 0])
+
+        ..
 
-        ids_pointy = numpy.floor((point[pointy_axis] - self.offset[pointy_axis] - self.r / 4) / pointy_stepsize)
-        even = ids_pointy % 2 == 0
-        ids_flat = numpy.empty_like(ids_pointy)
-        ids_flat[~even] = numpy.floor((point[flat_axis][~even] - self.offset[flat_axis] - flat_stepsize/2) / flat_stepsize)
-        ids_flat[even] = numpy.floor((point[flat_axis][even] - self.offset[flat_axis]) / flat_stepsize)
-        
-        # Finetune ambiguous points
-        # Points at the top of the cell can be in this cell or in the cell to the top right or top left
-        rel_loc_y = ((point[pointy_axis] - self.offset[pointy_axis] - self.r / 4) % pointy_stepsize) + self.r / 4
-        rel_loc_x = ((point[flat_axis] - self.offset[flat_axis]) % flat_stepsize)
-        top_left_even = rel_loc_x / (flat_stepsize / self.r) < (rel_loc_y - self.r * 5/4)
-        top_right_even = (self.r * 1.25 - rel_loc_y) <= (rel_loc_x - flat_stepsize) / (flat_stepsize / self.r)
-        top_right_odd = (rel_loc_x - flat_stepsize / 2) / (flat_stepsize / self.r) <= (rel_loc_y - self.r * 5/4)
-        top_right_odd &= rel_loc_x >= flat_stepsize / 2
-        top_left_odd = (self.r * 1.25 - rel_loc_y) < (rel_loc_x - flat_stepsize / 2) / (flat_stepsize / self.r)
-        top_left_odd &= rel_loc_x < flat_stepsize / 2
-
-        ids_pointy[top_left_even & even] += 1
-        ids_pointy[top_right_even & even] += 1
-        ids_pointy[top_left_odd & ~even] += 1
-        ids_pointy[top_right_odd & ~even] += 1
-
-        ids_flat[top_left_even & even] -= 1
-        ids_flat[top_left_odd & ~even] += 1
+        Offsets, shift the grid with respect to the coordinate system,
+        and thus can influnce what cell contains the point:
 
-        if self._shape == "pointy":
-            result = numpy.array([ids_flat, ids_pointy], dtype="int").T
+        .. code-block:: python
+
+            >>> grid = RectGrid(dx=4, dy=1, offset=(2,0))
+            >>> grid.cell_at_point((1, 0))
+            array([-1,  0])
+
+        ..
 
-        elif self._shape == "flat":
-            result = numpy.array([ids_pointy, ids_flat], dtype="int").T
+        Multiple points can be specified as a list of points or an ndarray:
+
+        .. code-block:: python
+
+            >>> grid = RectGrid(dx=4, dy=1)
+            >>> points = [(3, 0), (-0.5, -0.5), (5, 0)]
+            >>> grid.cell_at_point(points)
+            array([[ 0,  0],
+                   [-1, -1],
+                   [ 1,  0]])
+            >>> points = numpy.array(points)
+            >>> grid.cell_at_point(points)
+            array([[ 0,  0],
+                   [-1, -1],
+                   [ 1,  0]])
 
-        return result[0] if len(result) == 1 else result
+        ..
 
+        """
+        point = numpy.array(point).T
+        ids_x = numpy.floor((point[0] - self.offset[0]) / self.dx)
+        ids_y = numpy.floor((point[1] - self.offset[1]) / self.dy)
+        return numpy.array([ids_x, ids_y], dtype="int").T
 
     def cell_corners(self, index: numpy.ndarray = None) -> numpy.ndarray:
         """Return corners in (cells, corners, xy)"""
         if index is None:
-            raise ValueError("For grids that do not contain data, argument `index` is to be supplied to method `corners`.")
+            raise ValueError(
+                "For grids that do not contain data, argument `index` is to be supplied to method `corners`."
+            )
         centroids = self.centroid(index).T
-        
+
         if len(centroids.shape) == 1:
-            corners = numpy.empty((6,2))
+            corners = numpy.empty((4, 2))
         else:
-            corners = numpy.empty((6,2,centroids.shape[1]))
+            corners = numpy.empty((4, 2, centroids.shape[1]))
 
-        for i in range(6):
-            angle_deg = 60 * i - 30 if self._shape == "pointy" else 60 * i
-            angle_rad = numpy.pi / 180 * angle_deg
-            corners[i, 0] = centroids[0] + self.r * numpy.cos(angle_rad)
-            corners[i, 1] = centroids[1] + self.r * numpy.sin(angle_rad)
+        corners[0, 0] = centroids[0] - self.dx / 2
+        corners[0, 1] = centroids[1] - self.dy / 2
+        corners[1, 0] = centroids[0] + self.dx / 2
+        corners[1, 1] = centroids[1] - self.dy / 2
+        corners[2, 0] = centroids[0] + self.dx / 2
+        corners[2, 1] = centroids[1] + self.dy / 2
+        corners[3, 0] = centroids[0] - self.dx / 2
+        corners[3, 1] = centroids[1] + self.dy / 2
 
         # swap from (corners, xy, cells) to (cells, corners, xy)
         if len(centroids.shape) > 1:
             corners = numpy.moveaxis(corners, 2, 0)
 
         return corners
 
-
     def is_aligned_with(self, other):
-        if not isinstance(other, BaseGrid):
-            raise ValueError(f"Expected a (child of) BaseGrid, got {type(other)}")
+        if not isinstance(other, RectGrid):
+            raise ValueError(f"Expected a RectGrid, got {type(other)}")
         aligned = True
         reason = ""
         reasons = []
 
-        if not isinstance(other.parent_grid_class, self.parent_grid_class):
-            aligned = False
-            return False, f"Grid type is not the same. This is a {self.parent_grid_class}, the other is a {other.parent_grid_class}"
-
-        if (self.crs is None and other.crs is None):
+        if self.crs is None and other.crs is None:
             pass
         elif self.crs is None:
             aligned = False
             reasons.append("CRS")
         elif not self.crs.is_exact_same(other.crs):
             aligned = False
             reasons.append("CRS")
 
         if not numpy.isclose(self.dx, other.dx) or not numpy.isclose(self.dy, other.dy):
             aligned = False
             reasons.append("cellsize")
 
-        if not all(numpy.isclose(self.offset, other.offset, atol=1e-7)): # FIXME: atol if 1e-7 is a bandaid. It seems the offset depends slightly depending on the bounds after resampling on grid
+        if not all(
+            numpy.isclose(self.offset, other.offset, atol=1e-7)
+        ):  # FIXME: atol if 1e-7 is a bandaid. It seems the offset depends slightly depending on the bounds after resampling on grid
             aligned = False
             reasons.append("offset")
 
-        reason = f"The following attributes are not the same: {reasons}" if reasons else reason
+        reason = (
+            f"The following attributes are not the same: {reasons}"
+            if reasons
+            else reason
+        )
         return aligned, reason
 
-
     def cells_in_bounds(self, bounds):
-        """Cells contained within a bounding box.
-
+        """
         Parameters
         ----------
         bounds: :class:`tuple`
-            The bounding box in which to find the cells in (min_x, min_y, max_x, max_y)
+        align_mode: :class:`str`
+            Specifies when to consider a cell included in the bounds. Options:
+             - contains
+               select cells fully contained in the specified bounds
+             - contains_center
+               select cells of which the center is contained in the specified bounds
+             - intersects
+               select cells partially or fully contained in the specified bounds
         """
-        # TODO: Simplify function. Conceptually hard to follow and not very DRY
+
         if not self.are_bounds_aligned(bounds):
-            raise ValueError(f"supplied bounds '{bounds}' are not aligned with the grid lines. Consider calling 'align_bounds' first.")
+            raise ValueError(
+                f"supplied bounds '{bounds}' are not aligned with the grid lines. Consider calling 'align_bounds' first."
+            )
 
         if not self.are_bounds_aligned(bounds):
             bounds = self.align_bounds(bounds, mode="expand")
 
         # get coordinates of two diagonally opposing corner-cells
-        left_top = (bounds[0] + self.dx / 4, bounds[3] - self.dy / 4)
-        left_bottom = (bounds[0] + self.dx / 4, bounds[1] + self.dy / 4)
-        right_top = (bounds[2] - self.dx / 4, bounds[3] - self.dy / 4)
-        right_bottom = (bounds[2] - self.dx / 4, bounds[1] + self.dy / 4)
+        left_top = (bounds[0] + self.dx / 2, bounds[3] - self.dy / 2)
+        right_bottom = (bounds[2] - self.dx / 2, bounds[1] + self.dy / 2)
 
         # translate the coordinates of the corner cells into indices
-        left_top_id, left_bottom_id, right_top_id, right_bottom_id = self.cell_at_point([left_top, left_bottom, right_top, right_bottom])
-
-        if self._shape == "pointy":
-            nr_cells_flat = round(((bounds[2] - bounds[0]) / self.dx))
-        elif self._shape == "flat":
-            nr_cells_flat = round(((bounds[3] - bounds[1]) / self.dy))
-
-        ids_x = numpy.arange(left_bottom_id[0] - 2, right_top_id[0] + 2)
-        ids_y = numpy.arange(left_bottom_id[1] - 2, right_top_id[1] + 2)
-        ids_x_full, ids_y_full = numpy.meshgrid(ids_x, ids_y, indexing="xy")
-        ids = numpy.vstack([ids_x_full.ravel(), ids_y_full.ravel()]).T
-        
-        # determine what cells are outside of bounding box
-        centroids = self.centroid(ids).T
-        error_margin = numpy.finfo(numpy.float32).eps # expect problems with machine precision since some cells are on the bounds by design
-        oob_mask = centroids[0] < (bounds[0] - error_margin)
-        oob_mask |= centroids[1] < (bounds[1] - error_margin)
-        oob_mask |= centroids[0] >= (bounds[2] - error_margin)
-        oob_mask |= centroids[1] >= (bounds[3] - error_margin)
+        left_top_id, right_bottom_id = self.cell_at_point([left_top, right_bottom])
 
-        ids = ids[~oob_mask]
+        # turn minimum and maximum indices into fully arranged array
+        # TODO: think about dtype. 64 is too large. Should this be exposed? Or automated based on id range?
+        ids_y = numpy.arange(
+            left_top_id[1], right_bottom_id[1] - 1, -1, dtype="int32"
+        )  # y-axis goes from top to bottom (high to low), hence step size is -1
+        ids_x = list(range(left_top_id[0], right_bottom_id[0] + 1))
+
+        # TODO: only return ids_y and ids_x without fully filled grid
+        shape = (len(ids_y), len(ids_x))
+        ids = numpy.empty((2, numpy.multiply(*shape)), dtype="int32")
+        ids[0] = ids_x * len(ids_y)
+        # ids[1] = numpy.tile(ids_y[::-1], len(ids_x)) # invert y for ids are calculated from origin, not form the top of the bounding box
+        ids[1] = numpy.repeat(ids_y, len(ids_x))
 
-        shape = (int(numpy.ceil(ids.shape[0] / nr_cells_flat)), nr_cells_flat) if nr_cells_flat != 0 else (0, 0)
-        return ids, shape
+        return ids.T, shape
 
     @property
     def parent_grid_class(self):
-        return HexGrid
+        return RectGrid
 
 
-class BoundedHexGrid(BoundedGrid, HexGrid):
-
-    def __init__(self, data, *args, bounds, shape="flat", **kwargs):
-        if bounds[2] <= bounds [0] or bounds[3] <= bounds[1]:
-            raise ValueError(f"Incerrect bounds. Minimum value exceeds maximum value for bounds {bounds}")
-
-        if shape == "pointy":
-            dx = (bounds[2] - bounds[0]) / data.shape[1]
-            dy = (bounds[3] - bounds[1]) / data.shape[0]
-            size = dx
-            if not numpy.isclose(size / 2, dy / 3**0.5):
-                raise ValueError("The supplied data cannot be covered by hexagons with sides of equal length.")
-        elif shape == "flat":
-            dx = (bounds[2] - bounds[0]) / data.shape[0]
-            dy = (bounds[3] - bounds[1]) / data.shape[1]
-            size = dy
-            if not numpy.isclose(size / 2, dx / 3**0.5):
-                raise ValueError("The supplied data cannot be covered by hexagons with sides of equal length.")
+class BoundedRectGrid(BoundedGrid, RectGrid):
+    def __init__(self, data, *args, bounds, **kwargs):
+        if bounds[2] <= bounds[0] or bounds[3] <= bounds[1]:
+            raise ValueError(
+                f"Incerrect bounds. Minimum value exceeds maximum value for bounds {bounds}"
+            )
+        dx = (bounds[2] - bounds[0]) / data.shape[1]
+        dy = (bounds[3] - bounds[1]) / data.shape[0]
 
         offset_x = bounds[0] % dx
         offset_y = bounds[1] % dy
         offset_x = dx - offset_x if offset_x < 0 else offset_x
         offset_y = dy - offset_y if offset_y < 0 else offset_y
         offset = (
-            0 if numpy.isclose(offset_x, dx) else offset_x, 
-            0 if numpy.isclose(offset_y, dy) else offset_y
+            0 if numpy.isclose(offset_x, dx) else offset_x,
+            0 if numpy.isclose(offset_y, dy) else offset_y,
+        )
+        super(BoundedRectGrid, self).__init__(
+            data, *args, dx=dx, dy=dy, bounds=bounds, offset=offset, **kwargs
         )
-        super(BoundedHexGrid, self).__init__(data, *args, size=size, bounds=bounds, offset=offset, shape=shape, **kwargs)
-
-        if not self.are_bounds_aligned(bounds):
-            raise AlignmentError("Something went wrong, the supplied bounds are not aligned with the resulting grid.")
 
     @property
     def nr_cells(self):
         return (self.width, self.height)
 
     @property
     def lon(self):
         """Array of long values
 
         Returns
         -------
         :class:`numpy.ndarray`
             1D-Array of size `width`, containing the longitudinal values from left to right
         """
-        return numpy.linspace(self.bounds[0] + self.dx / 2, self.bounds[2] - self.dx / 2, self.width)
+        return numpy.linspace(
+            self.bounds[0] + self.dx / 2, self.bounds[2] - self.dx / 2, self.width
+        )
 
     @property
     def lat(self):
         """Array of lat values
 
         Returns
         -------
         :class:`numpy.ndarray`
             1D-Array of size `height`, containing the latitudinal values from top to bottom
         """
-        return numpy.linspace(self.bounds[3] - self.dy / 2, self.bounds[1] + self.dy / 2, self.height)
+        return numpy.linspace(
+            self.bounds[3] - self.dy / 2, self.bounds[1] + self.dy / 2, self.height
+        )
+
+    def centroid(self, index=None):
+        """Centroids of all cells
+
+        Returns
+        -------
+        :class:`numpy.ndarray`
+            Multidimensional array containing the longitude and latitude of the center of each cell respectively,
+            in (width, height, lonlat)
+        """
+        if index is not None:
+            return super(BoundedRectGrid, self).centroid(index=index)
+        # get grid in shape (latlon, width, height)
+        latlon = numpy.meshgrid(self.lon, self.lat, sparse=False, indexing="xy")
+
+        # return grid in shape (width, height, lonlat)
+        return numpy.array([latlon[0].ravel(), latlon[1].ravel()]).T
 
     def intersecting_cells(self, other):
         raise NotImplementedError()
 
     def crop(self, new_bounds, bounds_crs=None, buffer_cells=0):
-
         if bounds_crs is not None:
             bounds_crs = CRS.from_user_input(bounds_crs)
             transformer = Transformer.from_crs(bounds_crs, self.crs, always_xy=True)
             new_bounds = transformer.transform_bounds(*new_bounds)
 
         if not self.intersects(new_bounds):
-            raise IntersectionError(f"Cannot crop grid with bounds {self.bounds} to {new_bounds} for they do not intersect.")
+            raise IntersectionError(
+                f"Cannot crop grid with bounds {self.bounds} to {new_bounds} for they do not intersect."
+            )
         new_bounds = self.shared_bounds(new_bounds)
 
         new_bounds = self.align_bounds(new_bounds, mode="contract")
         slice_y, slice_x = self._data_slice_from_bounds(new_bounds)
         if buffer_cells:
             slice_x = slice(slice_x.start - buffer_cells, slice_x.stop + buffer_cells)
             slice_y = slice(slice_y.start - buffer_cells, slice_y.stop + buffer_cells)
             new_bounds = (
                 new_bounds[0] - buffer_cells * self.dx,
                 new_bounds[1] - buffer_cells * self.dy,
                 new_bounds[2] + buffer_cells * self.dx,
                 new_bounds[3] + buffer_cells * self.dy,
             )
         # cropped_data = numpy.flipud(numpy.flipud(self._data)[slice_y, slice_x]) # TODO: fix this blasted flipping. The raster should not be stored upside down maybe
-        cropped_data = self._data[slice_y, slice_x] #Fixme: seems to be flipped?
+        cropped_data = self._data[slice_y, slice_x]  # Fixme: seems to be flipped?
         # cropped_data = self._data[slice_x, slice_y]
         return self.update(cropped_data, bounds=new_bounds)
 
     def _data_slice_from_bounds(self, bounds):
-
         if not self.are_bounds_aligned(bounds):
-            raise ValueError(f"Cannot create slice from unaligned bounds {tuple(bounds)}")
+            raise ValueError(
+                f"Cannot create slice from unaligned bounds {tuple(bounds)}"
+            )
 
         difference_left = round(abs((self.bounds[0] - bounds[0]) / self.dx))
         difference_right = round(abs((self.bounds[2] - bounds[2]) / self.dx))
         slice_x = slice(
             difference_left,
-            self.width - difference_right, # add one for upper bound of slice is exclusive
+            self.width
+            - difference_right,  # add one for upper bound of slice is exclusive
         )
 
         difference_bottom = round(abs((self.bounds[1] - bounds[1]) / self.dy))
         difference_top = round(abs((self.bounds[3] - bounds[3]) / self.dy))
         slice_y = slice(
             difference_top,
-            self.height - difference_bottom, # add one for upper bound of slice is exclusive
+            self.height
+            - difference_bottom,  # add one for upper bound of slice is exclusive
         )
 
         return slice_y, slice_x
 
     def cell_corners(self, index: numpy.ndarray = None) -> numpy.ndarray:
         if index is None:
             index = self.indices()
-        return super(BoundedHexGrid, self).cell_corners(index=index)
+        return super(BoundedRectGrid, self).cell_corners(index=index)
 
     def to_shapely(self, index=None, as_multipolygon: bool = False):
-        """Refer to :meth:`.BaseGrid.to_shapely`
+        """Refer to parent method :meth:`.BaseGrid.to_shapely`
 
-        Difference with :meth:`.BaseGrid.to_shapely`:
-            `index` is optional. 
+        Difference with parent method:
+            `index` is optional.
             If `index` is None (default) the cells containing data are used as the `index` argument.
 
         See also
         --------
         :meth:`.BaseGrid.to_shapely`
-        :meth:`.BoundedRectGrid.to_shapely`
+        :meth:`.BoundedHexGrid.to_shapely`
         """
         if index is None:
             index = self.indices
         return super().to_shapely(index, as_multipolygon)
 
-    def resample(self, alignment_grid, method="nearest"):
-        raise NotImplementedError()
+    def _bilinear_interpolation(self, sample_points):
+        """Interpolate the value at the location of `sample_points` by doing a bilinear interpolation
+        using the 4 cells around the point.
+
+        Parameters
+        ----------
+        sample_points: :class:`numpy.ndarray`
+            The coordinates of the points at which to sample the data
+
+        Returns
+        -------
+        :class:`numpy.ndarray`
+            The interpolated values at the supplied points
+
+        See also
+        --------
+        :py:meth:`.RectGrid.cell_at_point`
+        """
+        nodata_value = self.nodata_value if self.nodata_value is not None else numpy.nan
+        tl_ids, tr_ids, bl_ids, br_ids = self.cells_near_point(sample_points)
+
+        tl_val = self.value(tl_ids, oob_value=nodata_value)
+        tr_val = self.value(tr_ids, oob_value=nodata_value)
+        bl_val = self.value(bl_ids, oob_value=nodata_value)
+        br_val = self.value(br_ids, oob_value=nodata_value)
+
+        # determine relative location of new point between old cell centers in x and y directions
+        abs_diff = sample_points - self.centroid(bl_ids)
+        x_diff = abs_diff[:, 0] / self.dx
+        y_diff = abs_diff[:, 1] / self.dy
+
+        top_val = tl_val + (tr_val - tl_val) * x_diff
+        bot_val = bl_val + (br_val - bl_val) * x_diff
+        values = bot_val + (top_val - bot_val) * y_diff
+
+        # TODO: remove rows and cols with nans around the edge after bilinear
+        return values
 
     def to_crs(self, crs, resample_method="nearest"):
-        new_inf_grid = super(BoundedHexGrid, self).to_crs(crs, resample_method=resample_method)
+        new_inf_grid = super(BoundedRectGrid, self).to_crs(
+            crs, resample_method=resample_method
+        )
         return self.resample(new_inf_grid, method=resample_method)
 
     def numpy_id_to_grid_id(self, np_index):
-        raise NotImplementedError()
         centroid_topleft = (self.bounds[0] + self.dx / 2, self.bounds[3] - self.dy / 2)
         index_topleft = self.cell_at_point(centroid_topleft)
         return (index_topleft[0] + np_index[1], index_topleft[1] - np_index[0])
 
     def grid_id_to_numpy_id(self, index):
-        raise NotImplementedError()
         centroid_topleft = (self.bounds[0] + self.dx / 2, self.bounds[3] - self.dy / 2)
         index_topleft = self.cell_at_point(centroid_topleft)
         return (index_topleft[1] - index[1], index[0] - index_topleft[0])
 
     def interp_nodata(self, *args, **kwargs):
         """Please refer to :func:`~gridkit.bounded_grid.BoundedGrid.interp_nodata`."""
         # Fixme: in the case of a rectangular grid, a performance improvement can be obtained by using scipy.interpolate.interpn
-        return super(BoundedHexGrid, self).interp_nodata(*args, **kwargs)
-
+        return super(BoundedRectGrid, self).interp_nodata(*args, **kwargs)
```

### Comparing `gridkit-0.2.0/gridkit/io.py` & `gridkit-0.3.0/gridkit/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from gridkit.rect_grid import BoundedRectGrid
-import rasterio
 import numpy
+import rasterio
 from pyproj import CRS, Transformer
 
+from gridkit.rect_grid import BoundedRectGrid
+
 
 def read_geotiff(path, bands=1, bounds=None, bounds_crs=None, border_buffer=0):
     """Read data from a GeoTIFF
 
     Returns
     -------
     :class:`~gridkit.rect_grid.BoundedRectGrid`
@@ -23,43 +24,46 @@
             if bounds_crs is not None:
                 bounds_crs = CRS.from_user_input(bounds_crs)
                 transformer = Transformer.from_crs(bounds_crs, crs, always_xy=True)
                 bounds = transformer.transform_bounds(*bounds)
             top, left = raster_file.index(bounds[0], bounds[3])
             bottom, right = raster_file.index(bounds[2], bounds[1])
 
-            if border_buffer: # note rasterio slices from top to bottom
+            if border_buffer:  # note rasterio slices from top to bottom
                 left -= border_buffer
                 right += border_buffer
                 top -= border_buffer
                 bottom += border_buffer
 
             # Create a window from the indices
             window = rasterio.windows.Window.from_slices((top, bottom), (left, right))
-            bounds = rasterio.windows.bounds(window, raster_file.transform) # update the bounds to those of the window
+            bounds = rasterio.windows.bounds(
+                window, raster_file.transform
+            )  # update the bounds to those of the window
         else:
             window = None
             b = raster_file.bounds if bounds is None else bounds
             bounds = (b.left, b.bottom, b.right, b.top)
 
-        data = raster_file.read(bands, window=window)        
+        data = raster_file.read(bands, window=window)
         nodata = raster_file.nodata
 
     grid = BoundedRectGrid(data, bounds=bounds, crs=crs, nodata_value=nodata)
     return grid
 
+
 def write_raster(grid, path):
     transform = rasterio.transform.from_bounds(*grid.bounds, grid.width, grid.height)
     with rasterio.open(
         path,
         "w",
         driver="GTiff",
         height=grid.height,
         width=grid.width,
-        count=1, # nr bands
+        count=1,  # nr bands
         dtype=grid._data.dtype,
         crs=grid.crs,
         nodata=grid.nodata_value,
         transform=transform,
     ) as dst:
         dst.write(numpy.expand_dims(grid._data.copy(), 0))
     return path
```

### Comparing `gridkit-0.2.0/gridkit/rect_grid.py` & `gridkit-0.3.0/gridkit/hex_grid.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,147 +1,202 @@
-from gridkit.base_grid import BaseGrid
-from gridkit.bounded_grid import BoundedGrid
-from gridkit.errors import IntersectionError, AlignmentError
+import warnings
 
-import scipy
 import numpy
-import warnings
 from pyproj import CRS, Transformer
 
-class RectGrid(BaseGrid):
+from gridkit.base_grid import BaseGrid
+from gridkit.bounded_grid import BoundedGrid
+from gridkit.errors import AlignmentError, IntersectionError
+from gridkit.rect_grid import RectGrid
+
+
+class HexGrid(BaseGrid):
+    def __init__(self, *args, size, shape="pointy", **kwargs):
+        self._size = size
+        self._radius = size / 3**0.5
+
+        if shape == "pointy":
+            self._dx = size
+            self._dy = 3 / 2 * self._radius
+        elif shape == "flat":
+            self._dy = size
+            self._dx = 3 / 2 * self._radius
+        else:
+            raise ValueError(
+                f"A HexGrid's `shape` can either be 'pointy' or 'flat', got '{shape}'"
+            )
 
-    def __init__(self, *args, dx, dy, **kwargs):
-        self.__dx = dx
-        self.__dy = dy
-        self.bounded_cls = BoundedRectGrid
-        super(RectGrid, self).__init__(*args, **kwargs)
+        self._shape = shape
+        self.bounded_cls = BoundedHexGrid
+        super(HexGrid, self).__init__(*args, **kwargs)
 
     @property
     def dx(self) -> float:
-        """The cellsize in x-direction
-        """
-        return self.__dx
+        """The spacing between cell centers in x-direction"""
+        return self._dx
 
     @property
     def dy(self) -> float:
-        """The cellsize in y-direction
+        """The spacing between cell centers in y-direction"""
+        return self._dy
+
+    @property
+    def r(self) -> float:
+        """The radius of the cell. The radius is defined to be the distance from the cell center to a cell corner."""
+        return self._radius
+
+    @property
+    def shape(self) -> str:
+        """The shape of the grid as supplied when initiating the class.
+        This can be either "flat" or "pointy" referring to the top of the cells.
         """
-        return self.__dy
+        return self._shape
 
-    def relative_neighbours(self, depth=1, connect_corners=False, include_selected=False, index=None):
+    @property
+    def size(self) -> float:
+        """The size of the cell as supplied when initiating the class.
+        This is the same as dx for a flat grid and the same as dy for a pointy grid.
+        """
+        return self._size
+
+    def relative_neighbours(
+        self, depth=1, *, index, include_selected=False, connect_corners=False
+    ) -> numpy.ndarray:
         """The relative indices of the neighbouring cells.
 
         Parameters
         ----------
         depth: :class:`int` Default: 1
             Determines the number of neighbours that are returned.
             If `depth=1` the direct neighbours are returned.
             If `depth=2` the direct neighbours are returned, as well as the neighbours of these neighbours.
             `depth=3` returns yet another layer of neighbours, and so forth.
+        index: :class:`numpy.ndarray`
+            The index of the cell of which the relative neighbours are desired.
+            This is mostly relevant because in hexagonal grids the neighbouring indices differ
+            when dealing with odd or even indices.
         include_selected: :class:`bool` Default: False
             Whether to include the specified cell in the return array.
             Even though the specified cell can never be a neighbour of itself,
             this can be useful when for example a weighted average of the neighbours is desired
             in which case the cell itself often should also be included.
         connect_corners: :class:`bool` Default: False
             Whether to consider cells that touch corners but not sides as neighbours.
-            If `connect_corners` is True, the 4 cells directly touching the cell are considered neighbours.
-            If `connect_corners` is True, the 8 cells surrounding the cell are considered neighbours.
-            This escalates in combination with `depth` where indices in a square shape around the cell are returned
-            when `connect_corners` is True, and indices in a diamond shape around the cell are returned when `connect_corners` is False.
-        index: :class:`numpy.ndarray`
-            The index is mostly relevant for hexagonal grids.
-            For a square grid the relative neighbours are independent on the location on the grid.
-            Here it is only used for the return length.
-            If 10 cells are supplied to `index`, the relative neighbours are returned 10 times.
-            This is to keep a consistent api between the two classes.
+            This is not relevant in hexagonal grids. It does nothing here.
+            See :py:meth:`.RectGrid.relative_neighbours`
 
 
         Examples
         --------
         The direct neighbours of a cell can be returned by using depth=1, which is the default.
-        For square grids, the number of returned neighbours depends on whether `connect_corners` is True or False:
-        
+        For hexagonal grids, the relative indices of the neighbours differs depending on the index.
+        There are two cases, neighbour indices for even colums and neighbour indices for odd columns,
+        in the case of a grid 'pointy' shape.
+        This works on rows if the grid has a 'flat' shape.
+
         .. code-block:: python
 
-            >>> from gridkit.rect_grid import RectGrid
-            >>> grid = RectGrid(dx=2, dy=3)
-            >>> grid.relative_neighbours()
-            array([[ 0,  1],
+            >>> from gridkit.hex_grid import HexGrid
+            >>> grid = HexGrid(size=3)
+            >>> grid.relative_neighbours(index=[0,0])
+            array([[-1,  1],
+                   [ 0,  1],
                    [-1,  0],
                    [ 1,  0],
+                   [-1, -1],
                    [ 0, -1]])
-            >>> grid.relative_neighbours(connect_corners=True)
-            array([[-1,  1],
-                   [ 0,  1],
+            >>> grid.relative_neighbours(index=[0,1])
+            array([[ 0,  1],
                    [ 1,  1],
                    [-1,  0],
                    [ 1,  0],
-                   [-1, -1],
                    [ 0, -1],
                    [ 1, -1]])
 
         ..
 
         By specifying `depth` we can include indirect neighbours from further away.
-        The number of neighbours increases with depth by a factor of `depth*4` or `depth*8` depending on `connect_corners` being True or False.
-        So the 3rd element in the list will be `1*4 + 2*4 + 3*4 = 24` if `connect_corners` is False.
-        And it will be `1*8 + 2*8 + 3*8 = 48` if `connect_corners` is True.
+        The number of neighbours increases with depth by a factor of `depth*6`.
+        So the 3rd element in the list will be `1*6 + 2*6 + 3*6 = 36`.
 
         .. code-block:: python
 
-            >>> [len(grid.relative_neighbours(depth=depth)) for depth in range(1,5)]
-            [4, 12, 24, 36]
-            >>> [len(grid.relative_neighbours(depth=depth, connect_corners=True)) for depth in range(1,5)]
-            [8, 24, 48, 80]
+            >>> [len(grid.relative_neighbours(index=[0,0], depth=depth)) for depth in range(1,5)]
+            [6, 18, 36, 60]
 
         ..
 
         The specified cell can be included if `include_selected` is set to True:
 
         .. code-block:: python
 
-            >>> grid.relative_neighbours(include_selected=True)
-            array([[ 0,  1],
+            >>> grid.relative_neighbours(index=[0,0], include_selected=True)
+            array([[-1,  1],
+                   [ 0,  1],
                    [-1,  0],
                    [ 0,  0],
                    [ 1,  0],
+                   [-1, -1],
                    [ 0, -1]])
 
         ..
 
         See also
         --------
         :py:meth:`.BaseGrid.neighbours`
-        :py:meth:`.HexGrid.relative_neighbours`
+        :py:meth:`.RectGrid.relative_neighbours`
         """
 
         if depth < 1:
             raise ValueError("'depth' cannot be lower than 1")
 
-        neighbours = numpy.empty(((2*depth+1)**2, 2), dtype=int)
-
-        relative_ids_1d = numpy.arange(-depth, depth+1)
-        relative_x, relative_y = numpy.meshgrid(relative_ids_1d, relative_ids_1d[::-1])
-        neighbours[:,0], neighbours[:,1] = numpy.ravel(relative_x), numpy.ravel(relative_y)
-
-        if not connect_corners:
-            mask = abs(numpy.multiply(*neighbours.T)) < depth
-            neighbours = neighbours[mask]
+        index = numpy.array(index)
+        if len(index.shape) == 1:
+            index = index[numpy.newaxis]
+
+        nr_neighbours = (
+            sum(6 * numpy.arange(1, depth + 1)) + 1
+        )  # Add 1 for the first cell
+        nr_indices = len(index)
+        neighbours = numpy.empty((nr_indices, nr_neighbours, 2), dtype=int)
+        start_slice = 0
+        rows = range(depth, -1, -1)
+
+        # create top half of selection
+        for i, row in enumerate(rows):  # loop from top row to bottom row
+            row_length = depth + i + 1
+            row_slice = slice(start_slice, start_slice + row_length)
+            max_val = int(numpy.floor(row_length / 2))
+            if self._shape == "pointy":
+                pointy_axis = 1
+                flat_axis = 0
+            elif self._shape == "flat":
+                pointy_axis = 0
+                flat_axis = 1
+
+            if (i % 2 == 0) == (depth % 2 == 0):
+                neighbours[:, row_slice, flat_axis] = range(-max_val, max_val + 1)
+            else:
+                odd_mask = index[:, pointy_axis] % 2 != 0
+                neighbours[odd_mask, row_slice, flat_axis] = range(
+                    -max_val + 1, max_val + 1
+                )
+                neighbours[~odd_mask, row_slice, flat_axis] = range(-max_val, max_val)
+            neighbours[:, row_slice, pointy_axis] = row
+            start_slice += row_length
+
+        # mirror top half to bottom half (leaving the center row be)
+        neighbours[:, start_slice:] = neighbours[:, 0 : start_slice - row_length][::-1]
+        neighbours[:, start_slice:, pointy_axis] *= -1
 
         if include_selected is False:
-            center_cell = int(numpy.floor(len(neighbours)/2))
-            neighbours = numpy.delete(neighbours, center_cell, 0)
+            center_cell = int(numpy.floor(neighbours.shape[1] / 2))
+            neighbours = numpy.delete(neighbours, center_cell, 1)
 
-        if index is not None:
-            index = numpy.array(index)
-            if len(index.shape) == 2:
-                neighbours = numpy.repeat(neighbours[numpy.newaxis], len(index), axis=0)
-
-        return neighbours
+        return neighbours if len(neighbours) > 1 else neighbours[0]
 
     def centroid(self, index=None):
         """Coordinates at the center of the cell(s) specified by `index`.
 
         .. Warning ::
             The two values that make up an `index` are expected to be integers, and will be cast as such.
 
@@ -161,15 +216,15 @@
         Raises
         ------
         ValueError
             No `index` parameter was supplied. `index` can only be `None` in classes that contain data.
 
         Examples
         --------
-        Cell centers of single index are returned as an array with one dimention: 
+        Cell centers of single index are returned as an array with one dimention:
 
         .. code-block:: python
 
             >>> grid = RectGrid(dx=4, dy=1)
             >>> grid.centroid((0, 0))
             array([2. , 0.5])
             >>> grid.centroid((-1, -1))
@@ -199,25 +254,34 @@
             >>> grid.centroid((0, 0))
             array([3., 1.])
 
         ..
 
 
         """
-        
+
         if index is None:
-            raise ValueError("For grids that do not contain data, argument `index` is to be supplied to method `centroid`.")
+            raise ValueError(
+                "For grids that do not contain data, argument `index` is to be supplied to method `centroid`."
+            )
         index = numpy.array(index, dtype="int").T
         centroids = numpy.empty_like(index, dtype=float)
         centroids[0] = index[0] * self.dx + (self.dx / 2) + self.offset[0]
         centroids[1] = index[1] * self.dy + (self.dy / 2) + self.offset[1]
+
+        if self._shape == "pointy":
+            offset_rows = index[1] % 2 == 1
+            centroids[0, offset_rows] += self.dx / 2
+        elif self._shape == "flat":
+            offset_rows = index[0] % 2 == 1
+            centroids[1, offset_rows] += self.dy / 2
         return centroids.T
 
     def cells_near_point(self, point):
-        """Nearest 4 cells around a point.
+        """Nearest 3 cells around a point.
         This includes the cell the point is contained within,
         as well as two direct neighbours of this cell and one diagonal neighbor.
         What neigbors of the containing are slected, depends on where in the cell the point is located.
 
         Args
         ----
         point: :class"`tuple`
@@ -232,86 +296,80 @@
             If a single point is supplied, the four indices are returned as 1d arrays of length 2.
             If multiple points are supplied, the four indices are returned as Nx2 ndarrays.
 
         Examples
         --------
         Nearby cell indices are returned as a tuple:
 
-        .. code-block:: python
-
-            >>> grid = RectGrid(dx=4, dy=1)
-            >>> grid.cells_near_point((0, 0))
-            (array([-1,  0]), array([0, 0]), array([-1, -1]), array([ 0, -1]))
-            >>> grid.cells_near_point((3, 0.75))
-            (array([0, 1]), array([1, 1]), array([0, 0]), array([1, 0]))
-
-        ..
-
-        If multiple points are supplied, a tuple with ndarrays is returned:
-
-        .. code-block:: python
-
-            >>> points = [(0, 0), (3, 0.75), (3, 0)]
-            >>> nearby_cells = grid.cells_near_point(points)
-            >>> from pprint import pprint # used for output readability purposes only
-            >>> pprint(nearby_cells)
-            (array([[-1,  0],
-                   [ 0,  1],
-                   [ 0,  0]]),
-             array([[0, 0],
-                   [1, 1],
-                   [1, 0]]),
-             array([[-1, -1],
-                   [ 0,  0],
-                   [ 0, -1]]),
-             array([[ 0, -1],
-                   [ 1,  0],
-                   [ 1, -1]]))
-
-        ..
 
         """
+        cell = self.cell_at_point(point)
+        centroid = self.centroid(cell)
+        distance_vector = point - centroid
+        azimuth = numpy.arctan2(*distance_vector.T) * 180 / numpy.pi
+        # FIXME: if there is one point, azimuth is a float in which we cannot use a mask. Make the check more elegant
+        point = numpy.array(point)
+        if len(point.shape) == 1:
+            azimuth = numpy.array([azimuth])
+
+        if len(cell.shape) == 1:
+            cell = numpy.expand_dims(cell, axis=0)
+        az_ranges = [(0, 60), (60, 120), (120, 180), (180, 240), (240, 300), (300, 360)]
+        if self._shape == "flat":
+            inconsistent_axis = (
+                0  # TODO: Make consistent and inconsisten axis a property of self
+            )
+            consistent_axis = 1
+            shift_odd_cells = [1, slice(1, 3), 2, 1, slice(1, 3), 2]
+            nearby_cells_relative_idx = [
+                [[1, 0], [0, 1]],
+                [[1, -1], [1, 0]],
+                [[0, -1], [1, -1]],
+                [[-1, -1], [0, -1]],
+                [[-1, 0], [-1, -1]],
+                [[0, 1], [-1, 0]],
+            ]
+        elif self._shape == "pointy":
+            inconsistent_axis = 1
+            consistent_axis = 0
+            azimuth += (
+                30  # it is easier to work with ranges starting at 0 rather than -30
+            )
+            shift_odd_cells = [slice(1, 3), 1, 2, slice(1, 3), 1, 2]
+            nearby_cells_relative_idx = [
+                [[-1, 1], [0, 1]],
+                [[0, 1], [1, 0]],
+                [[1, 0], [0, -1]],
+                [[0, -1], [-1, -1]],
+                [[-1, -1], [-1, 0]],
+                [[-1, 0], [-1, 1]],
+            ]
+        else:
+            raise AttributeError(f"Unrecognized grid shape {self._shape}")
 
-        # Split each cell into 4 quadrants in order to identify what 3 neigbors to select
-        new_grid = RectGrid(
-            dx = self.dx/2,
-            dy = self.dy/2,
-            offset = self.offset
-        )
-        ids = new_grid.cell_at_point(point).T
-        left_top_mask = numpy.logical_and(ids[0] % 2 == 0, ids[1] % 2 == 1)
-        right_top_mask = numpy.logical_and(ids[0] % 2 == 1, ids[1] % 2 == 1)
-        right_bottom_mask = numpy.logical_and(ids[0] % 2 == 1, ids[1] % 2 == 0)
-        left_bottom_mask = numpy.logical_and(ids[0] % 2 == 0, ids[1] % 2 == 0)
-
-        # obtain the bottom-left cell based on selected quadrant
-        base_ids = numpy.empty_like(ids, dtype="int")
-        # bottom-left if point in upper-right quadrant
-        base_ids[:,right_top_mask] = numpy.floor(ids[:,right_top_mask] / 2)
-        # bottom-left if point in bottom-right quadrant
-        base_ids[:,right_bottom_mask] = numpy.floor(ids[:,right_bottom_mask] / 2)
-        base_ids[1,right_bottom_mask] -= 1
-        # bottom-left if point in bottom-left quadrant
-        base_ids[:,left_bottom_mask] = numpy.floor(ids[:,left_bottom_mask] / 2)
-        base_ids[:,left_bottom_mask] -= 1
-        # bottom-left if point in upper-left qudrant
-        base_ids[:,left_top_mask] = numpy.floor(ids[:,left_top_mask] / 2)
-        base_ids[0,left_top_mask] -= 1
-
-        # use the bottom-left cell to determine the other three
-        bl_ids = base_ids.copy()
-        br_ids = base_ids.copy()
-        br_ids[0] += 1
-        tr_ids = base_ids.copy()
-        tr_ids += 1
-        tl_ids = base_ids.copy()
-        tl_ids[1] += 1
-            
-        return tl_ids.T, tr_ids.T, bl_ids.T, br_ids.T
+        nearby_cells = numpy.repeat(
+            numpy.expand_dims(cell, axis=0), 3, axis=0
+        )  # shape: neighbours(3), points(n), xy(2)
+        odd_cells_mask = cell[:, inconsistent_axis] % 2 == 1
+
+        # make sure azimuth is inbetween 0 and 360, and not between -180 and 180
+        azimuth[azimuth <= 0] += 360
+        azimuth[azimuth > 360] -= 360
+
+        for az_range, shift_odd, cells in zip(
+            az_ranges, shift_odd_cells, nearby_cells_relative_idx
+        ):
+            mask = numpy.logical_and(azimuth > az_range[0], azimuth <= az_range[1])
+            nearby_cells[1, mask] += cells[0]
+            nearby_cells[2, mask] += cells[1]
+            mask_odd = numpy.logical_and(mask, odd_cells_mask)
+            nearby_cells[shift_odd, mask_odd, consistent_axis] += 1
 
+        nearby_cells = numpy.swapaxes(nearby_cells, 0, 1)
+        return nearby_cells[0] if len(nearby_cells) == 1 else nearby_cells
 
     def cell_at_point(self, point):
         """Index of the cell containing the supplied point(s).
 
         Parameters
         ----
         point: :class:`tuple`
@@ -322,370 +380,463 @@
         Returns
         -------
         :class:`numpy.ndarray`
             The index of the cell containing the point(s).
             If a single point is supplied, the index is returned as a 1d array of length 2.
             If multiple points are supplied, the indices are returned as Nx2 ndarrays.
 
-        Examples
-        --------
-
-        .. code-block:: python
-
-            >>> grid = RectGrid(dx=4, dy=1)
-            >>> grid.cell_at_point((1, 0))
-            array([0, 0])
-
-        ..
-
-        Offsets, shift the grid with respect to the coordinate system,
-        and thus can influnce what cell contains the point:
+        """
+        point = numpy.array(point)
+        point = numpy.expand_dims(point, axis=0).T if len(point.shape) == 1 else point.T
 
-        .. code-block:: python
+        # approach adapted after https://stackoverflow.com/a/7714148
+        if self._shape == "pointy":
+            flat_axis = 0
+            pointy_axis = 1
+            flat_stepsize = self.dx
+            pointy_stepsize = self.dy
+        elif self._shape == "flat":
+            flat_axis = 1
+            pointy_axis = 0
+            flat_stepsize = self.dy
+            pointy_stepsize = self.dx
+        else:
+            raise ValueError(
+                f"A HexGrid's `shape` can either be 'pointy' or 'flat', got '{self._shape}'"
+            )
 
-            >>> grid = RectGrid(dx=4, dy=1, offset=(2,0))
-            >>> grid.cell_at_point((1, 0))
-            array([-1,  0])
+        ids_pointy = numpy.floor(
+            (point[pointy_axis] - self.offset[pointy_axis] - self.r / 4)
+            / pointy_stepsize
+        )
+        even = ids_pointy % 2 == 0
+        ids_flat = numpy.empty_like(ids_pointy)
+        ids_flat[~even] = numpy.floor(
+            (point[flat_axis][~even] - self.offset[flat_axis] - flat_stepsize / 2)
+            / flat_stepsize
+        )
+        ids_flat[even] = numpy.floor(
+            (point[flat_axis][even] - self.offset[flat_axis]) / flat_stepsize
+        )
 
-        ..
+        # Finetune ambiguous points
+        # Points at the top of the cell can be in this cell or in the cell to the top right or top left
+        rel_loc_y = (
+            (point[pointy_axis] - self.offset[pointy_axis] - self.r / 4)
+            % pointy_stepsize
+        ) + self.r / 4
+        rel_loc_x = (point[flat_axis] - self.offset[flat_axis]) % flat_stepsize
+        top_left_even = rel_loc_x / (flat_stepsize / self.r) < (
+            rel_loc_y - self.r * 5 / 4
+        )
+        top_right_even = (self.r * 1.25 - rel_loc_y) <= (rel_loc_x - flat_stepsize) / (
+            flat_stepsize / self.r
+        )
+        top_right_odd = (rel_loc_x - flat_stepsize / 2) / (flat_stepsize / self.r) <= (
+            rel_loc_y - self.r * 5 / 4
+        )
+        top_right_odd &= rel_loc_x >= flat_stepsize / 2
+        top_left_odd = (self.r * 1.25 - rel_loc_y) < (rel_loc_x - flat_stepsize / 2) / (
+            flat_stepsize / self.r
+        )
+        top_left_odd &= rel_loc_x < flat_stepsize / 2
 
-        Multiple points can be specified as a list of points or an ndarray:
+        ids_pointy[top_left_even & even] += 1
+        ids_pointy[top_right_even & even] += 1
+        ids_pointy[top_left_odd & ~even] += 1
+        ids_pointy[top_right_odd & ~even] += 1
 
-        .. code-block:: python
+        ids_flat[top_left_even & even] -= 1
+        ids_flat[top_left_odd & ~even] += 1
 
-            >>> grid = RectGrid(dx=4, dy=1)
-            >>> points = [(3, 0), (-0.5, -0.5), (5, 0)]
-            >>> grid.cell_at_point(points)
-            array([[ 0,  0],
-                   [-1, -1],
-                   [ 1,  0]])
-            >>> points = numpy.array(points)
-            >>> grid.cell_at_point(points)
-            array([[ 0,  0],
-                   [-1, -1],
-                   [ 1,  0]])
+        if self._shape == "pointy":
+            result = numpy.array([ids_flat, ids_pointy], dtype="int").T
 
-        ..
+        elif self._shape == "flat":
+            result = numpy.array([ids_pointy, ids_flat], dtype="int").T
 
-        """
-        point = numpy.array(point).T
-        ids_x = numpy.floor((point[0] - self.offset[0]) / self.dx)
-        ids_y = numpy.floor((point[1] - self.offset[1]) / self.dy)
-        return numpy.array([ids_x, ids_y], dtype="int").T
+        return result[0] if len(result) == 1 else result
 
     def cell_corners(self, index: numpy.ndarray = None) -> numpy.ndarray:
         """Return corners in (cells, corners, xy)"""
         if index is None:
-            raise ValueError("For grids that do not contain data, argument `index` is to be supplied to method `corners`.")
+            raise ValueError(
+                "For grids that do not contain data, argument `index` is to be supplied to method `corners`."
+            )
         centroids = self.centroid(index).T
-        
+
         if len(centroids.shape) == 1:
-            corners = numpy.empty((4,2))
+            corners = numpy.empty((6, 2))
         else:
-            corners = numpy.empty((4,2,centroids.shape[1]))
+            corners = numpy.empty((6, 2, centroids.shape[1]))
 
-        corners[0,0] = centroids[0] - self.dx / 2
-        corners[0,1] = centroids[1] - self.dy / 2
-        corners[1,0] = centroids[0] + self.dx / 2
-        corners[1,1] = centroids[1] - self.dy / 2
-        corners[2,0] = centroids[0] + self.dx / 2
-        corners[2,1] = centroids[1] + self.dy / 2
-        corners[3,0] = centroids[0] - self.dx / 2
-        corners[3,1] = centroids[1] + self.dy / 2
+        for i in range(6):
+            angle_deg = 60 * i - 30 if self._shape == "pointy" else 60 * i
+            angle_rad = numpy.pi / 180 * angle_deg
+            corners[i, 0] = centroids[0] + self.r * numpy.cos(angle_rad)
+            corners[i, 1] = centroids[1] + self.r * numpy.sin(angle_rad)
 
         # swap from (corners, xy, cells) to (cells, corners, xy)
         if len(centroids.shape) > 1:
             corners = numpy.moveaxis(corners, 2, 0)
 
         return corners
 
-
     def is_aligned_with(self, other):
-        if not isinstance(other, RectGrid):
-            raise ValueError(f"Expected a RectGrid, got {type(other)}")
+        if not isinstance(other, BaseGrid):
+            raise ValueError(f"Expected a (child of) BaseGrid, got {type(other)}")
         aligned = True
         reason = ""
         reasons = []
-        
-        if (self.crs is None and other.crs is None):
+
+        if not isinstance(other.parent_grid_class, self.parent_grid_class):
+            aligned = False
+            return (
+                False,
+                f"Grid type is not the same. This is a {self.parent_grid_class}, the other is a {other.parent_grid_class}",
+            )
+
+        if self.crs is None and other.crs is None:
             pass
         elif self.crs is None:
             aligned = False
             reasons.append("CRS")
         elif not self.crs.is_exact_same(other.crs):
             aligned = False
             reasons.append("CRS")
 
         if not numpy.isclose(self.dx, other.dx) or not numpy.isclose(self.dy, other.dy):
             aligned = False
             reasons.append("cellsize")
 
-        if not all(numpy.isclose(self.offset, other.offset, atol=1e-7)): # FIXME: atol if 1e-7 is a bandaid. It seems the offset depends slightly depending on the bounds after resampling on grid
+        if not all(
+            numpy.isclose(self.offset, other.offset, atol=1e-7)
+        ):  # FIXME: atol if 1e-7 is a bandaid. It seems the offset depends slightly depending on the bounds after resampling on grid
             aligned = False
             reasons.append("offset")
 
-        reason = f"The following attributes are not the same: {reasons}" if reasons else reason
+        reason = (
+            f"The following attributes are not the same: {reasons}"
+            if reasons
+            else reason
+        )
         return aligned, reason
 
-
     def cells_in_bounds(self, bounds):
-        """
+        """Cells contained within a bounding box.
+
         Parameters
         ----------
         bounds: :class:`tuple`
-        align_mode: :class:`str`
-            Specifies when to consider a cell included in the bounds. Options:
-             - contains
-               select cells fully contained in the specified bounds
-             - contains_center
-               select cells of which the center is contained in the specified bounds
-             - intersects
-               select cells partially or fully contained in the specified bounds
+            The bounding box in which to find the cells in (min_x, min_y, max_x, max_y)
         """
-
+        # TODO: Simplify function. Conceptually hard to follow and not very DRY
         if not self.are_bounds_aligned(bounds):
-            raise ValueError(f"supplied bounds '{bounds}' are not aligned with the grid lines. Consider calling 'align_bounds' first.")
+            raise ValueError(
+                f"supplied bounds '{bounds}' are not aligned with the grid lines. Consider calling 'align_bounds' first."
+            )
 
         if not self.are_bounds_aligned(bounds):
             bounds = self.align_bounds(bounds, mode="expand")
 
         # get coordinates of two diagonally opposing corner-cells
-        left_top = (bounds[0] + self.dx / 2, bounds[3] - self.dy / 2)
-        right_bottom = (bounds[2] - self.dx / 2, bounds[1] + self.dy / 2)
+        left_top = (bounds[0] + self.dx / 4, bounds[3] - self.dy / 4)
+        left_bottom = (bounds[0] + self.dx / 4, bounds[1] + self.dy / 4)
+        right_top = (bounds[2] - self.dx / 4, bounds[3] - self.dy / 4)
+        right_bottom = (bounds[2] - self.dx / 4, bounds[1] + self.dy / 4)
 
         # translate the coordinates of the corner cells into indices
-        left_top_id, right_bottom_id = self.cell_at_point([left_top, right_bottom])
-
-        # turn minimum and maximum indices into fully arranged array
-        # TODO: think about dtype. 64 is too large. Should this be exposed? Or automated based on id range?
-        ids_y = numpy.arange(left_top_id[1], right_bottom_id[1]-1, -1, dtype="int32") # y-axis goes from top to bottom (high to low), hence step size is -1
-        ids_x = list(range(left_top_id[0], right_bottom_id[0]+1))
-
-        # TODO: only return ids_y and ids_x without fully filled grid
-        shape = (len(ids_y), len(ids_x))
-        ids = numpy.empty((2, numpy.multiply(*shape)), dtype="int32")
-        ids[0] = ids_x * len(ids_y)
-        # ids[1] = numpy.tile(ids_y[::-1], len(ids_x)) # invert y for ids are calculated from origin, not form the top of the bounding box
-        ids[1] = numpy.repeat(ids_y, len(ids_x))
+        left_top_id, left_bottom_id, right_top_id, right_bottom_id = self.cell_at_point(
+            [left_top, left_bottom, right_top, right_bottom]
+        )
 
-        return ids.T, shape
+        if self._shape == "pointy":
+            nr_cells_flat = round(((bounds[2] - bounds[0]) / self.dx))
+        elif self._shape == "flat":
+            nr_cells_flat = round(((bounds[3] - bounds[1]) / self.dy))
+
+        ids_x = numpy.arange(left_bottom_id[0] - 2, right_top_id[0] + 2)
+        ids_y = numpy.arange(left_bottom_id[1] - 2, right_top_id[1] + 2)
+        if self._shape == "flat":
+            ids_x_full, ids_y_full = numpy.meshgrid(ids_x, ids_y, indexing="ij")
+            ids_y_full = numpy.fliplr(ids_y_full)
+        else:
+            ids_x_full, ids_y_full = numpy.meshgrid(ids_x, ids_y, indexing="xy")
+            ids_y_full = numpy.flipud(ids_y_full)
+        ids = numpy.vstack([ids_x_full.ravel(), ids_y_full.ravel()]).T
+
+        # determine what cells are outside of bounding box
+        centroids = self.centroid(ids).T
+        error_margin = numpy.finfo(
+            numpy.float32
+        ).eps  # expect problems with machine precision since some cells are on the bounds by design
+        oob_mask = centroids[0] < (bounds[0] - error_margin)
+        oob_mask |= centroids[1] < (bounds[1] - error_margin)
+        oob_mask |= centroids[0] >= (bounds[2] - error_margin)
+        oob_mask |= centroids[1] >= (bounds[3] - error_margin)
+
+        ids = ids[~oob_mask]
+
+        shape = (
+            (int(numpy.ceil(ids.shape[0] / nr_cells_flat)), nr_cells_flat)
+            if nr_cells_flat != 0
+            else (0, 0)
+        )
+        return ids, shape
 
     @property
     def parent_grid_class(self):
-        return RectGrid
+        return HexGrid
 
 
-class BoundedRectGrid(BoundedGrid, RectGrid):
+class BoundedHexGrid(BoundedGrid, HexGrid):
+    def __init__(self, data, *args, bounds, shape="flat", **kwargs):
+        if bounds[2] <= bounds[0] or bounds[3] <= bounds[1]:
+            raise ValueError(
+                f"Incerrect bounds. Minimum value exceeds maximum value for bounds {bounds}"
+            )
 
-    def __init__(self, data, *args, bounds, **kwargs):
-        if bounds[2] <= bounds [0] or bounds[3] <= bounds[1]:
-            raise ValueError(f"Incerrect bounds. Minimum value exceeds maximum value for bounds {bounds}")
-        dx = (bounds[2] - bounds[0]) / data.shape[1]
-        dy = (bounds[3] - bounds[1]) / data.shape[0]
+        if shape == "pointy":
+            dx = (bounds[2] - bounds[0]) / data.shape[1]
+            dy = (bounds[3] - bounds[1]) / data.shape[0]
+            size = dx
+            if not numpy.isclose(size / 2, dy / 3**0.5):
+                raise ValueError(
+                    "The supplied data cannot be covered by hexagons with sides of equal length."
+                )
+        elif shape == "flat":
+            dx = (bounds[2] - bounds[0]) / data.shape[0]
+            dy = (bounds[3] - bounds[1]) / data.shape[1]
+            size = dy
+            if not numpy.isclose(size / 2, dx / 3**0.5):
+                raise ValueError(
+                    "The supplied data cannot be covered by hexagons with sides of equal length."
+                )
 
         offset_x = bounds[0] % dx
         offset_y = bounds[1] % dy
         offset_x = dx - offset_x if offset_x < 0 else offset_x
         offset_y = dy - offset_y if offset_y < 0 else offset_y
         offset = (
-            0 if numpy.isclose(offset_x, dx) else offset_x, 
-            0 if numpy.isclose(offset_y, dy) else offset_y
+            0 if numpy.isclose(offset_x, dx) else offset_x,
+            0 if numpy.isclose(offset_y, dy) else offset_y,
+        )
+        super(BoundedHexGrid, self).__init__(
+            data, *args, size=size, bounds=bounds, offset=offset, shape=shape, **kwargs
         )
-        super(BoundedRectGrid, self).__init__(data, *args, dx=dx, dy=dy, bounds=bounds, offset=offset, **kwargs)
+
+        if not self.are_bounds_aligned(bounds):
+            raise AlignmentError(
+                "Something went wrong, the supplied bounds are not aligned with the resulting grid."
+            )
 
     @property
     def nr_cells(self):
         return (self.width, self.height)
 
     @property
     def lon(self):
         """Array of long values
 
         Returns
         -------
         :class:`numpy.ndarray`
             1D-Array of size `width`, containing the longitudinal values from left to right
         """
-        return numpy.linspace(self.bounds[0] + self.dx / 2, self.bounds[2] - self.dx / 2, self.width)
+        return numpy.linspace(
+            self.bounds[0] + self.dx / 2, self.bounds[2] - self.dx / 2, self.width
+        )
 
     @property
     def lat(self):
         """Array of lat values
 
         Returns
         -------
         :class:`numpy.ndarray`
             1D-Array of size `height`, containing the latitudinal values from top to bottom
         """
-        return numpy.linspace(self.bounds[3] - self.dy / 2, self.bounds[1] + self.dy / 2, self.height)
-
-    def centroid(self, index=None):
-        """Centroids of all cells
-
-        Returns
-        -------
-        :class:`numpy.ndarray`
-            Multidimensional array containing the longitude and latitude of the center of each cell respectively,
-            in (width, height, lonlat)
-        """
-        if index is not None:
-            return super(BoundedRectGrid, self).centroid(index=index)
-        # get grid in shape (latlon, width, height)
-        latlon = numpy.meshgrid(self.lon, self.lat, sparse=False, indexing="xy")
-
-        # return grid in shape (width, height, lonlat)
-        return numpy.array([latlon[0].ravel(),latlon[1].ravel()]).T
+        return numpy.linspace(
+            self.bounds[3] - self.dy / 2, self.bounds[1] + self.dy / 2, self.height
+        )
 
     def intersecting_cells(self, other):
         raise NotImplementedError()
 
     def crop(self, new_bounds, bounds_crs=None, buffer_cells=0):
-
         if bounds_crs is not None:
             bounds_crs = CRS.from_user_input(bounds_crs)
             transformer = Transformer.from_crs(bounds_crs, self.crs, always_xy=True)
             new_bounds = transformer.transform_bounds(*new_bounds)
 
         if not self.intersects(new_bounds):
-            raise IntersectionError(f"Cannot crop grid with bounds {self.bounds} to {new_bounds} for they do not intersect.")
+            raise IntersectionError(
+                f"Cannot crop grid with bounds {self.bounds} to {new_bounds} for they do not intersect."
+            )
         new_bounds = self.shared_bounds(new_bounds)
 
         new_bounds = self.align_bounds(new_bounds, mode="contract")
         slice_y, slice_x = self._data_slice_from_bounds(new_bounds)
         if buffer_cells:
             slice_x = slice(slice_x.start - buffer_cells, slice_x.stop + buffer_cells)
             slice_y = slice(slice_y.start - buffer_cells, slice_y.stop + buffer_cells)
             new_bounds = (
                 new_bounds[0] - buffer_cells * self.dx,
                 new_bounds[1] - buffer_cells * self.dy,
                 new_bounds[2] + buffer_cells * self.dx,
                 new_bounds[3] + buffer_cells * self.dy,
             )
         # cropped_data = numpy.flipud(numpy.flipud(self._data)[slice_y, slice_x]) # TODO: fix this blasted flipping. The raster should not be stored upside down maybe
-        cropped_data = self._data[slice_y, slice_x] #Fixme: seems to be flipped?
+        cropped_data = self._data[slice_y, slice_x]  # Fixme: seems to be flipped?
         # cropped_data = self._data[slice_x, slice_y]
         return self.update(cropped_data, bounds=new_bounds)
 
     def _data_slice_from_bounds(self, bounds):
-
         if not self.are_bounds_aligned(bounds):
-            raise ValueError(f"Cannot create slice from unaligned bounds {tuple(bounds)}")
+            raise ValueError(
+                f"Cannot create slice from unaligned bounds {tuple(bounds)}"
+            )
 
         difference_left = round(abs((self.bounds[0] - bounds[0]) / self.dx))
         difference_right = round(abs((self.bounds[2] - bounds[2]) / self.dx))
         slice_x = slice(
             difference_left,
-            self.width - difference_right, # add one for upper bound of slice is exclusive
+            self.width
+            - difference_right,  # add one for upper bound of slice is exclusive
         )
 
         difference_bottom = round(abs((self.bounds[1] - bounds[1]) / self.dy))
         difference_top = round(abs((self.bounds[3] - bounds[3]) / self.dy))
         slice_y = slice(
             difference_top,
-            self.height - difference_bottom, # add one for upper bound of slice is exclusive
+            self.height
+            - difference_bottom,  # add one for upper bound of slice is exclusive
         )
 
         return slice_y, slice_x
 
     def cell_corners(self, index: numpy.ndarray = None) -> numpy.ndarray:
         if index is None:
             index = self.indices()
-        return super(BoundedRectGrid, self).cell_corners(index=index)
-    
+        return super(BoundedHexGrid, self).cell_corners(index=index)
+
     def to_shapely(self, index=None, as_multipolygon: bool = False):
-        """Refer to parent method :meth:`.BaseGrid.to_shapely`
+        """Refer to :meth:`.BaseGrid.to_shapely`
 
-        Difference with parent method:
-            `index` is optional. 
+        Difference with :meth:`.BaseGrid.to_shapely`:
+            `index` is optional.
             If `index` is None (default) the cells containing data are used as the `index` argument.
-        
+
         See also
         --------
         :meth:`.BaseGrid.to_shapely`
-        :meth:`.BoundedHexGrid.to_shapely`
+        :meth:`.BoundedRectGrid.to_shapely`
         """
         if index is None:
             index = self.indices
         return super().to_shapely(index, as_multipolygon)
 
-    def resample(self, alignment_grid, method="nearest"):
-        if self.crs is None or alignment_grid.crs is None:
-            warnings.warn("`crs` not set for one or both grids. Assuming both grids have an identical CRS.")
-            different_crs = False
-        else:
-            different_crs = not self.crs.is_exact_same(alignment_grid.crs)
-
-        # make sure the bounds align with the grid
-        if different_crs:
-            transformer = Transformer.from_crs(self.crs, alignment_grid.crs, always_xy=True)
-            bounds = transformer.transform_bounds(*self.bounds)
-        else:
-            bounds = self.bounds
-
-        # Align using "contract" for we cannot sample outside of the original bounds
-        new_bounds = alignment_grid.align_bounds(bounds, mode="contract")
-
-        new_ids, new_shape = alignment_grid.cells_in_bounds(bounds=new_bounds)
-
-        new_points = alignment_grid.centroid(new_ids)
-
-        if different_crs:
-            transformer = Transformer.from_crs(alignment_grid.crs, self.crs, always_xy=True)
-            transformed_points = transformer.transform(*new_points.T)
-            new_points = numpy.vstack(transformed_points).T
-
-        nodata_value = self.nodata_value if self.nodata_value is not None else numpy.nan
-        if method == "nearest":
-            new_ids = self.cell_at_point(new_points)
-            value = self.value(new_ids)
-        elif method == "bilinear":
-            tl_ids, tr_ids, bl_ids, br_ids = self.cells_near_point(new_points)
-
-            tl_val = self.value(tl_ids, oob_value=nodata_value)
-            tr_val = self.value(tr_ids, oob_value=nodata_value)
-            bl_val = self.value(bl_ids, oob_value=nodata_value)
-            br_val = self.value(br_ids, oob_value=nodata_value)
-
-            # determine relative location of new point between old cell centers in x and y directions
-            abs_diff = (new_points - self.centroid(bl_ids))
-            x_diff = abs_diff[:,0] / self.dx
-            y_diff = abs_diff[:,1] / self.dy
-
-            top_val = tl_val + (tr_val - tl_val) * x_diff
-            bot_val = bl_val + (br_val - bl_val) * x_diff
-            value = bot_val + (top_val - bot_val) * y_diff
+    def _bilinear_interpolation(self, sample_points):
+        """Interpolate the value at the location of `sample_points` by doing a bilinear interpolation
+        using the 4 cells around the point.
 
-            # TODO: remove rows and cols with nans around the edge after bilinear
-        else:
-            raise ValueError(f"Resampling method '{method}' is not supported.")
+        Parameters
+        ----------
+        sample_points: :class:`numpy.ndarray`
+            The coordinates of the points at which to sample the data
 
-        value = value.reshape(new_shape)
+        Returns
+        -------
+        :class:`numpy.ndarray`
+            The interpolated values at the supplied points
 
-        grid_kwargs = dict(
-            data=value, bounds=new_bounds, crs=alignment_grid.crs, nodata_value=nodata_value
-        )
-        if hasattr(alignment_grid, "_shape"):
-            grid_kwargs["shape"] = alignment_grid._shape
+        See also
+        --------
+        :py:meth:`.RectGrid.cell_at_point`
+        """
 
-        new_grid = alignment_grid.bounded_cls(**grid_kwargs)
+        # FIXME: speed up (numba)
+        def get_weight(point, p1, p2, p3):
+            def _project(point, line_points):
+                """Project 'point' onto a line drawn between 'line_points[0]' and 'line_points[1]'
+                Credits to https://stackoverflow.com/a/61343727/22128453
+                """
+                # distance between line_points[0] and line_points[1]
+                line_length = numpy.sum((line_points[0] - line_points[1]) ** 2)
+
+                # project point on line extension connecting line_points[0] and line_points[1]
+                t = (
+                    numpy.sum(
+                        (point - line_points[0]) * (line_points[1] - line_points[0])
+                    )
+                    / line_length
+                )
+
+                return line_points[0] + t * (line_points[1] - line_points[0])
+
+            side_length = numpy.linalg.norm(p1 - p2)
+            dd = p2 + (p2 - p3) / 2
+            if numpy.linalg.norm(dd - p1) > side_length:
+                dd = p2 - (p2 - p3) / 2
+            ad = dd - p1
+
+            projected = _project(point - p1, [p3 - p1, p2 - p1])
+            return numpy.linalg.norm((projected - (point - p1)) / numpy.linalg.norm(ad))
+
+        all_nearby_cells = self.cells_near_point(
+            sample_points
+        )  # (points, nearby_cells, xy)
+        values = numpy.empty(len(sample_points))
+        for idx, (point, nearby_cells) in enumerate(
+            zip(sample_points, all_nearby_cells)
+        ):
+            nearby_centroids = self.centroid(nearby_cells)
+            p1, p2, p3 = nearby_centroids
+            weights = numpy.array(
+                [
+                    get_weight(point, p1, p2, p3),
+                    get_weight(point, p2, p1, p3),
+                    get_weight(point, p3, p2, p1),
+                ]
+            )
+            values[idx] = numpy.sum(weights * self.value(nearby_cells))
 
-        return new_grid
+        # TODO: remove rows and cols with nans around the edge after bilinear
+        return values
 
     def to_crs(self, crs, resample_method="nearest"):
-        new_inf_grid = super(BoundedRectGrid, self).to_crs(crs, resample_method=resample_method)
+        new_inf_grid = super(BoundedHexGrid, self).to_crs(
+            crs, resample_method=resample_method
+        )
         return self.resample(new_inf_grid, method=resample_method)
 
     def numpy_id_to_grid_id(self, np_index):
+        raise NotImplementedError()
         centroid_topleft = (self.bounds[0] + self.dx / 2, self.bounds[3] - self.dy / 2)
         index_topleft = self.cell_at_point(centroid_topleft)
         return (index_topleft[0] + np_index[1], index_topleft[1] - np_index[0])
 
     def grid_id_to_numpy_id(self, index):
+        if self._shape == "pointy":
+            offset_rows = index[1] % 2 == 1
+            index[0, offset_rows] += 1
+        elif self._shape == "flat":
+            offset_rows = index[0] % 2 == 1
+            index[1, offset_rows] += 1
+
         centroid_topleft = (self.bounds[0] + self.dx / 2, self.bounds[3] - self.dy / 2)
         index_topleft = self.cell_at_point(centroid_topleft)
-        return (index_topleft[1] - index[1], index[0] - index_topleft[0])
+        if self._shape == "pointy":
+            np_id = (index_topleft[1] - index[1], index[0] - index_topleft[0])
+        elif self._shape == "flat":
+            np_id = ((index[0] - index_topleft[0]), (index_topleft[1] - index[1]))
+        return np_id
 
     def interp_nodata(self, *args, **kwargs):
         """Please refer to :func:`~gridkit.bounded_grid.BoundedGrid.interp_nodata`."""
         # Fixme: in the case of a rectangular grid, a performance improvement can be obtained by using scipy.interpolate.interpn
-        return super(BoundedRectGrid, self).interp_nodata(*args, **kwargs)
+        return super(BoundedHexGrid, self).interp_nodata(*args, **kwargs)
 
+    def centroid(self, index=None):
+        if index is None:
+            index = self.indices
+        return super(BoundedHexGrid, self).centroid(index)
```

### Comparing `gridkit-0.2.0/setup.py` & `gridkit-0.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 with open("requirements.txt") as file:
     install_requires = file.read()
 
 tests_require = [
     "black",
     "geopandas",
+    "pytest-cov",
     "pytest-pylint",
     "pytest-black",
     "pylint",
     "pre-commit",
 ]
 
 docs_require = [
```

