# Comparing `tmp/xdas-0.1b1.tar.gz` & `tmp/xdas-0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdas-0.1b1.tar", last modified: Wed Jun 28 14:23:15 2023, max compression
+gzip compressed data, was "xdas-0.1b2.tar", last modified: Sun Jul 16 15:01:44 2023, max compression
```

## Comparing `xdas-0.1b1.tar` & `xdas-0.1b2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-06-28 14:23:15.893174 xdas-0.1b1/
--rw-r--r--   0 trabatto   (502) staff       (20)    35149 2023-01-26 16:18:03.000000 xdas-0.1b1/LICENSE.md
--rw-r--r--   0 trabatto   (502) staff       (20)      200 2023-06-28 14:23:15.893026 xdas-0.1b1/PKG-INFO
--rw-r--r--   0 trabatto   (502) staff       (20)      664 2023-06-13 10:17:32.000000 xdas-0.1b1/README.md
--rw-r--r--   0 trabatto   (502) staff       (20)      602 2023-06-28 14:19:21.000000 xdas-0.1b1/pyproject.toml
--rw-r--r--   0 trabatto   (502) staff       (20)       38 2023-06-28 14:23:15.893248 xdas-0.1b1/setup.cfg
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-06-28 14:23:15.890513 xdas-0.1b1/tests/
--rw-r--r--   0 trabatto   (502) staff       (20)    10709 2023-06-13 09:50:51.000000 xdas-0.1b1/tests/test_coordinates.py
--rw-r--r--   0 trabatto   (502) staff       (20)     1353 2023-06-28 14:18:52.000000 xdas-0.1b1/tests/test_core.py
--rw-r--r--   0 trabatto   (502) staff       (20)     1550 2023-06-13 09:50:51.000000 xdas-0.1b1/tests/test_database.py
--rw-r--r--   0 trabatto   (502) staff       (20)     2356 2023-06-28 14:18:52.000000 xdas-0.1b1/tests/test_processing.py
--rw-r--r--   0 trabatto   (502) staff       (20)     2289 2023-06-28 14:18:52.000000 xdas-0.1b1/tests/test_signal.py
--rw-r--r--   0 trabatto   (502) staff       (20)     2069 2023-06-28 14:18:52.000000 xdas-0.1b1/tests/test_virtual.py
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-06-28 14:23:15.891454 xdas-0.1b1/xdas/
--rw-r--r--   0 trabatto   (502) staff       (20)      179 2023-06-27 07:52:45.000000 xdas-0.1b1/xdas/__init__.py
--rw-r--r--   0 trabatto   (502) staff       (20)    11805 2023-06-13 09:50:51.000000 xdas-0.1b1/xdas/coordinates.py
--rw-r--r--   0 trabatto   (502) staff       (20)     4459 2023-06-28 14:18:52.000000 xdas-0.1b1/xdas/core.py
--rw-r--r--   0 trabatto   (502) staff       (20)    12260 2023-06-13 09:50:51.000000 xdas-0.1b1/xdas/database.py
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-06-28 14:23:15.892823 xdas-0.1b1/xdas/io/
--rw-r--r--   0 trabatto   (502) staff       (20)        0 2022-12-29 11:57:28.000000 xdas-0.1b1/xdas/io/__init__.py
--rw-r--r--   0 trabatto   (502) staff       (20)      677 2023-06-28 14:18:52.000000 xdas-0.1b1/xdas/io/asn.py
--rw-r--r--   0 trabatto   (502) staff       (20)     3691 2023-06-13 09:50:51.000000 xdas-0.1b1/xdas/io/febus.py
--rw-r--r--   0 trabatto   (502) staff       (20)     9268 2023-06-28 14:18:52.000000 xdas-0.1b1/xdas/processing.py
--rw-r--r--   0 trabatto   (502) staff       (20)     3308 2023-06-28 14:18:52.000000 xdas-0.1b1/xdas/signal.py
--rw-r--r--   0 trabatto   (502) staff       (20)     3666 2023-06-28 14:18:52.000000 xdas-0.1b1/xdas/virtual.py
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-06-28 14:23:15.892161 xdas-0.1b1/xdas.egg-info/
--rw-r--r--   0 trabatto   (502) staff       (20)      200 2023-06-28 14:23:15.000000 xdas-0.1b1/xdas.egg-info/PKG-INFO
--rw-r--r--   0 trabatto   (502) staff       (20)      479 2023-06-28 14:23:15.000000 xdas-0.1b1/xdas.egg-info/SOURCES.txt
--rw-r--r--   0 trabatto   (502) staff       (20)        1 2023-06-28 14:23:15.000000 xdas-0.1b1/xdas.egg-info/dependency_links.txt
--rw-r--r--   0 trabatto   (502) staff       (20)      170 2023-06-28 14:23:15.000000 xdas-0.1b1/xdas.egg-info/requires.txt
--rw-r--r--   0 trabatto   (502) staff       (20)        5 2023-06-28 14:23:15.000000 xdas-0.1b1/xdas.egg-info/top_level.txt
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-07-16 15:01:44.556594 xdas-0.1b2/
+-rw-r--r--   0 trabatto   (502) staff       (20)    35149 2023-01-26 16:18:03.000000 xdas-0.1b2/LICENSE.md
+-rw-r--r--   0 trabatto   (502) staff       (20)      200 2023-07-16 15:01:44.556439 xdas-0.1b2/PKG-INFO
+-rw-r--r--   0 trabatto   (502) staff       (20)      664 2023-06-13 10:17:32.000000 xdas-0.1b2/README.md
+-rw-r--r--   0 trabatto   (502) staff       (20)      602 2023-07-16 14:29:25.000000 xdas-0.1b2/pyproject.toml
+-rw-r--r--   0 trabatto   (502) staff       (20)       38 2023-07-16 15:01:44.556633 xdas-0.1b2/setup.cfg
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-07-16 15:01:44.553653 xdas-0.1b2/tests/
+-rw-r--r--   0 trabatto   (502) staff       (20)    10709 2023-06-13 09:50:51.000000 xdas-0.1b2/tests/test_coordinates.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     1345 2023-07-16 14:29:25.000000 xdas-0.1b2/tests/test_core.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     1754 2023-07-16 14:29:25.000000 xdas-0.1b2/tests/test_database.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     3017 2023-07-16 14:29:25.000000 xdas-0.1b2/tests/test_processing.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     2289 2023-06-28 14:18:52.000000 xdas-0.1b2/tests/test_signal.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     2069 2023-06-28 14:18:52.000000 xdas-0.1b2/tests/test_virtual.py
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-07-16 15:01:44.554833 xdas-0.1b2/xdas/
+-rw-r--r--   0 trabatto   (502) staff       (20)      216 2023-07-16 14:29:25.000000 xdas-0.1b2/xdas/__init__.py
+-rw-r--r--   0 trabatto   (502) staff       (20)    12128 2023-07-16 14:29:25.000000 xdas-0.1b2/xdas/coordinates.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     5177 2023-07-16 14:29:25.000000 xdas-0.1b2/xdas/core.py
+-rw-r--r--   0 trabatto   (502) staff       (20)    12502 2023-07-16 14:29:25.000000 xdas-0.1b2/xdas/database.py
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-07-16 15:01:44.556130 xdas-0.1b2/xdas/io/
+-rw-r--r--   0 trabatto   (502) staff       (20)        0 2022-12-29 11:57:28.000000 xdas-0.1b2/xdas/io/__init__.py
+-rw-r--r--   0 trabatto   (502) staff       (20)      677 2023-06-28 14:18:52.000000 xdas-0.1b2/xdas/io/asn.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     3691 2023-06-13 09:50:51.000000 xdas-0.1b2/xdas/io/febus.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     9506 2023-07-16 14:29:25.000000 xdas-0.1b2/xdas/processing.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     6127 2023-07-16 14:29:25.000000 xdas-0.1b2/xdas/signal.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     3666 2023-06-28 14:18:52.000000 xdas-0.1b2/xdas/virtual.py
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-07-16 15:01:44.555705 xdas-0.1b2/xdas.egg-info/
+-rw-r--r--   0 trabatto   (502) staff       (20)      200 2023-07-16 15:01:44.000000 xdas-0.1b2/xdas.egg-info/PKG-INFO
+-rw-r--r--   0 trabatto   (502) staff       (20)      479 2023-07-16 15:01:44.000000 xdas-0.1b2/xdas.egg-info/SOURCES.txt
+-rw-r--r--   0 trabatto   (502) staff       (20)        1 2023-07-16 15:01:44.000000 xdas-0.1b2/xdas.egg-info/dependency_links.txt
+-rw-r--r--   0 trabatto   (502) staff       (20)      170 2023-07-16 15:01:44.000000 xdas-0.1b2/xdas.egg-info/requires.txt
+-rw-r--r--   0 trabatto   (502) staff       (20)        5 2023-07-16 15:01:44.000000 xdas-0.1b2/xdas.egg-info/top_level.txt
```

### Comparing `xdas-0.1b1/LICENSE.md` & `xdas-0.1b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xdas-0.1b1/README.md` & `xdas-0.1b2/README.md`

 * *Files identical despite different names*

### Comparing `xdas-0.1b1/pyproject.toml` & `xdas-0.1b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xdas"
-version = "0.1b1"
+version = "0.1b2"
 authors = [
     {name = "Alister Trabattoni", email = "alister.trabattoni@gmail.com"},
 ]
 dependencies = [
     "dask",
     "h5py",
     "netcdf4",
```

### Comparing `xdas-0.1b1/tests/test_coordinates.py` & `xdas-0.1b2/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `xdas-0.1b1/tests/test_processing.py` & `xdas-0.1b2/tests/test_processing.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,73 @@
+import tempfile
+
 import dask.array as da
 import numpy as np
 import scipy.signal as sp
 
 from xdas.core import Coordinate, Database
-from xdas.processing import LFilter, SignalProcessingChain, SOSFilter
+from xdas.processing import ChunkWriter, LFilter, SignalProcessingChain, SOSFilter
+from xdas.virtual import DataLayout
 
 
 class TestProcessing:
-    def test_processing(self):
+    def generate(self):
         fs = 125
         ks = 1 / 10
         data = da.random.normal(size=(1000, 100))
         time = Coordinate([0, data.shape[0] - 1], [0.0, (data.shape[0] - 1) / fs])
         distance = Coordinate([0, data.shape[1] - 1], [0.0, (data.shape[1] - 1) / ks])
-        xarr = Database(data, {"time": time, "distance": distance})
+        return Database(data, {"time": time, "distance": distance})
+
+    def test_lfilter(self):
+        db = self.generate()
         b, a = sp.iirfilter(4, 0.5, btype="lowpass")
         lfilter = LFilter(b, a, "time")
-        result_direct = lfilter(xarr)
+        result_direct = lfilter(db)
         chunk_size = 100
         lfilter.reset()
-        result_chunks = xarr.copy()
-        for k in range(xarr.shape[0] // chunk_size):
+        result_chunks = db.copy()
+        for k in range(db.shape[0] // chunk_size):
             query = {"time": slice(k * chunk_size, (k + 1) * chunk_size)}
-            result_chunks[query] = lfilter(xarr[query]).data
+            result_chunks[query] = lfilter(db[query]).data
         lfilter.reset()
         chain = SignalProcessingChain([lfilter])
-        out = chain.process(xarr, "time", chunk_size, parallel=False)
+        out = chain.process(db, "time", chunk_size, parallel=False)
         lfilter.reset()
         assert chain.filters[0].zi == None
-        out_parallel = chain.process(xarr, "time", chunk_size, parallel=True)
+        out_parallel = chain.process(db, "time", chunk_size, parallel=True)
         assert np.allclose(result_chunks.data, result_direct.data)
         assert np.allclose(out.data, result_direct.data)
         assert np.allclose(out_parallel.data, result_direct.data)
 
+    def test_sosfilter(self):
+        db = self.generate()
         sos = sp.iirfilter(4, 0.5, btype="lowpass", output="sos")
         sosfilter = SOSFilter(sos, "time")
-        result_direct = sosfilter(xarr)
+        result_direct = sosfilter(db)
         chunk_size = 100
         sosfilter.reset()
-        result_chunks = xarr.copy()
-        for k in range(xarr.shape[0] // chunk_size):
+        result_chunks = db.copy()
+        for k in range(db.shape[0] // chunk_size):
             query = {"time": slice(k * chunk_size, (k + 1) * chunk_size)}
-            result_chunks[query] = sosfilter(xarr[query]).data
+            result_chunks[query] = sosfilter(db[query]).data
         sosfilter.reset()
         chain = SignalProcessingChain([sosfilter])
-        out = chain.process(xarr, "time", chunk_size, parallel=False)
+        out = chain.process(db, "time", chunk_size, parallel=False)
         sosfilter.reset()
         assert chain.filters[0].zi == None
-        out_parallel = chain.process(xarr, "time", chunk_size, parallel=True)
+        out_parallel = chain.process(db, "time", chunk_size, parallel=True)
         assert np.allclose(result_chunks.data, result_direct.data)
         assert np.allclose(out.data, result_direct.data)
         assert np.allclose(out_parallel.data, result_direct.data)
+
+    def test_chunkwriter(self):
+        db = self.generate()
+        with tempfile.TemporaryDirectory() as tmpdirname:
+            path = tmpdirname + "/test"
+            chain = SignalProcessingChain([ChunkWriter(path)])
+            out = chain.process(db, "time", 100)
+            assert np.array_equal(db.values, out.values)
+            print(out["time"].tie_indices)
+            print(out["time"].tie_values)
+            assert db.coords == out.coords
+            assert isinstance(out.data, DataLayout)
```

### Comparing `xdas-0.1b1/tests/test_signal.py` & `xdas-0.1b2/tests/test_signal.py`

 * *Files identical despite different names*

### Comparing `xdas-0.1b1/tests/test_virtual.py` & `xdas-0.1b2/tests/test_virtual.py`

 * *Files identical despite different names*

### Comparing `xdas-0.1b1/xdas/coordinates.py` & `xdas-0.1b2/xdas/coordinates.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,20 @@
 
     def to_index(self, item):
         if isinstance(item, slice):
             return self.get_index_slice(item)
         else:
             return self.get_index(item)
 
-    def simplify(self, tolerance):
+    def simplify(self, tolerance=None):
+        if tolerance is None:
+            if np.issubdtype(self.dtype, np.datetime64):
+                tolerance = np.timedelta64(0, "us")
+            else:
+                tolerance = 0.0
         tie_indices, tie_values = douglas_peucker(
             self.tie_indices, self.tie_values, tolerance
         )
         return self.__class__(tie_indices, tie_values)
 
     def get_discontinuities(self):
         (indices,) = np.nonzero(np.diff(self.tie_indices) == 1)
@@ -275,14 +280,18 @@
             {
                 self.tie_indices[index]: self.tie_values[index],
                 self.tie_indices[index + 1]: self.tie_values[index + 1],
             }
             for index in indices
         ]
 
+    @classmethod
+    def from_array(cls, arr, tolerance=None):
+        return cls(np.arange(len(arr)), arr).simplify(tolerance)
+
 
 class ScaleOffset:
     def __init__(self, scale, offset):
         self.scale = scale
         self.offset = offset
 
     def __eq__(self, other):
```

### Comparing `xdas-0.1b1/xdas/core.py` & `xdas-0.1b2/xdas/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from concurrent.futures import ProcessPoolExecutor, as_completed
 from glob import glob
 
 import numpy as np
+import xarray as xr
 from tqdm import tqdm
 
 from .coordinates import Coordinate
 from .database import Database, DataCollection
-from .virtual import DataLayout
+from .virtual import DataLayout, DataSource
 
 
 def open_mfdatabase(paths, engine="netcdf", tolerance=np.timedelta64(0, "us")):
     """
     Open a multiple file database.
 
     Parameters
@@ -42,47 +43,49 @@
             future.result()
             for future in tqdm(
                 as_completed(futures),
                 total=len(futures),
                 desc="Fetching metadata from files",
             )
         ]
-    return concatenate(dbs, tolerance=tolerance, virtual=True)
+    return concatenate(dbs, tolerance=tolerance)
 
 
-def concatenate(dbs, dim="time", tolerance=None, virtual=False):
+def concatenate(dbs, dim="time", tolerance=None, virtual=None):
     """
     Concatenate several databases along a given dimension.
 
     Parameters
     ----------
     dbs : list
         List of databases to concatenate.
     dim : str
         The dimension along which concatenate.
     tolerance : float of timedelta64, optional
         The tolerance to consider that the end of a file is continuous with beginning of
         the following, zero by default.
     virtual : bool, optional
         Whether to create a virtual dataset. It requires that all concatenated
-        databases are virtual.
+        databases are virtual. By default tries to create a virtual dataset if possible.
 
     Returns
     -------
     Database
         The concatenated database.
     """
     dbs = sorted(dbs, key=lambda db: db[dim][0])
     axis = dbs[0].get_axis_num(dim)
     dims = dbs[0].dims
     dtype = dbs[0].dtype
     shape = tuple(
         sum([db.shape[a] for db in dbs]) if a == axis else dbs[0].shape[a]
         for a in range(len(dims))
     )
+    if virtual is None:
+        virtual = all(isinstance(db.data, DataSource) for db in dbs)
     if virtual:
         data = DataLayout(shape, dtype)
     else:
         data = np.zeros(shape, dtype)
     idx = 0
     tie_indices = []
     tie_values = []
@@ -94,21 +97,15 @@
             data[selection] = db.data.vsource
         else:
             data[selection] = db.values
         tie_indices.extend(idx + db[dim].tie_indices)
         tie_values.extend(db[dim].tie_values)
         idx += db.shape[axis]
     coord = Coordinate(tie_indices, tie_values)
-    if tolerance is None:
-        if np.issubdtype(dbs[0][dim].dtype, np.datetime64):
-            tolerance = np.timedelta64(0, "us")
-        else:
-            tolerance = 0.0
-    if not tolerance == 0:
-        coord = coord.simplify(tolerance)
+    coord = coord.simplify(tolerance)
     coords = dbs[0].coords
     coords[dim] = coord
     return Database(data, coords)
 
 
 def open_database(fname, group=None, engine="netcdf", **kwargs):
     """
@@ -155,7 +152,39 @@
 
     Returns
     -------
     DataCollection
         The opened DataCollection.
     """
     return DataCollection.from_netcdf(fname, **kwargs)
+
+
+def asdatabase(obj, tolerance=None):
+    """
+    Try to convert given object to a database.
+
+    Only support Database or DataArray as input.
+
+    Parameters
+    ----------
+    obj : object
+        The objected to convert
+    tolerance : float or datetime64, optional
+        For dense coordinates, tolerance error for interpolation representation, by
+        default zero.
+
+    Returns
+    -------
+    Database
+        The object converted to a Database. Data is not copied.
+
+    Raises
+    ------
+    ValueError
+        _description_
+    """
+    if isinstance(obj, Database):
+        return obj
+    elif isinstance(obj, xr.DataArray):
+        return Database.from_xarray(obj, tolerance)
+    else:
+        raise ValueError("Cannot convert to database.")
```

### Comparing `xdas-0.1b1/xdas/database.py` & `xdas-0.1b2/xdas/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -254,14 +254,21 @@
             data=self.__array__(),
             coords={dim: self.coords[dim].__array__() for dim in self.coords},
             dims=self.dims,
             name=self.name,
             attrs=self.attrs,
         )
 
+    @classmethod
+    def from_xarray(cls, da, tolerance=None):
+        coords = {
+            dim: Coordinate.from_array(da[dim].values, tolerance) for dim in da.dims
+        }
+        return cls(da.data, coords, da.dims, da.name, da.attrs)
+
     def to_netcdf(self, fname, group=None, virtual=False, **kwargs):
         """
         Write Database contents to a netCDF file.
 
         Parameters
         ----------
         fname : str
```

### Comparing `xdas-0.1b1/xdas/io/asn.py` & `xdas-0.1b2/xdas/io/asn.py`

 * *Files identical despite different names*

### Comparing `xdas-0.1b1/xdas/io/febus.py` & `xdas-0.1b2/xdas/io/febus.py`

 * *Files identical despite different names*

### Comparing `xdas-0.1b1/xdas/processing.py` & `xdas-0.1b2/xdas/processing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from concurrent.futures import FIRST_COMPLETED, ThreadPoolExecutor, wait
 
 import numpy as np
 import scipy.signal as sp
 
-from xdas.core import concatenate
+from .core import concatenate, open_database
 
 
 class SignalProcessingChain:
     """
     Chain of processing unit to apply to a Database.
 
     Parameters
@@ -16,16 +16,16 @@
         The chain of filters to apply. The filters can have some state memory to ensure
         continuity when repeatedly applied to consecutive chunks.
     """
 
     def __init__(self, filters):
         self.filters = filters
 
-    def __call__(self, xarr):
-        out = xarr
+    def __call__(self, db):
+        out = db
         for filter in self.filters:
             out = filter(out)
         return out
 
     def process(self, db, dim, chunk_size, parallel=True):
         """
         Process a Database by chunk along a given dimension.
@@ -35,15 +35,15 @@
         db : Database
             The Database to process.
         dim : str
             Name of the the dimension along which to process the Database.
         chunk_size : int
             The number of samples per chunk.
         parallel : bool, optional
-            Whether to use multiprocessing to improve performance, by default True.
+            Whether to use multithreading to improve performance, by default True.
 
         Returns
         -------
         Database
             The processed Database.
         """
         div, mod = divmod(db.sizes[dim], chunk_size)
@@ -107,15 +107,15 @@
                 done, _ = wait(self.futures, return_when=FIRST_COMPLETED)
                 for future in done:
                     task = self.futures.pop(future)
                     self.buffer[task["chunk"]] = future.result()
                     next_tasks = self.get_next_tasks(task)
                     for next_task in next_tasks:
                         self.submit_task(next_task)
-                print("Number of futures:", len(self.futures))
+                # print("Number of futures:", len(self.futures))
         return list(self.buffer.values())
 
     def submit_task(self, task):
         """
         Submit a task.
 
         Parameters
@@ -129,15 +129,15 @@
         future
             The future related to the submitted task.
         """
         filter = self.filters[task["filter"]]
         chunk = self.buffer[task["chunk"]]
         future = self.executor.submit(filter, chunk)
         self.futures[future] = task
-        print("New task:", task)
+        # print("New task:", task)
         return future
 
     def get_next_tasks(self, task):
         """
         Given a finished task, gives the two new available possible tasks: applying the
         same filter on the next chunk and applying the next filter to the same chunk.
 
@@ -247,37 +247,37 @@
 
     def __init__(self, sos, dim):
         self.sos = sos
         self.dim = dim
         self.zi = None
         self.axis = None
 
-    def __call__(self, xarr):
+    def __call__(self, db):
         if (self.zi is None) or (self.axis is None):
-            self.initialize(xarr)
-        data, self.zi = sp.sosfilt(self.sos, xarr, axis=self.axis, zi=self.zi)
-        return xarr.copy(data=data)
+            self.initialize(db)
+        data, self.zi = sp.sosfilt(self.sos, db, axis=self.axis, zi=self.zi)
+        return db.copy(data=data)
 
-    def initialize(self, xarr):
+    def initialize(self, db):
         """
         Initialize the filter state.
 
         Parameters
         ----------
         db : Database
             Some sample of the kind of database to process to get the correct axis
             number.
         """
-        self.axis = xarr.get_axis_num(self.dim)
+        self.axis = db.get_axis_num(self.dim)
         zi = sp.sosfilt_zi(self.sos)
-        ndim = len(xarr.shape)
+        ndim = len(db.shape)
         n_sections = zi.shape[0]
         s = [n_sections] + [2 if k == self.axis else 1 for k in range(ndim)]
         zi = zi.reshape(s)
-        s = [n_sections] + [2 if k == self.axis else xarr.shape[k] for k in range(ndim)]
+        s = [n_sections] + [2 if k == self.axis else db.shape[k] for k in range(ndim)]
         zi = np.broadcast_to(zi, s)
         self.zi = zi
 
     def reset(self):
         """
         Reset state of the filter for a fresh start.
         """
@@ -290,24 +290,41 @@
         self.q = q
         self.dim = dim
 
     def __call__(self, db):
         return db[{self.dim: slice(None, None, self.q)}]
 
 
-class Writter(SignalProcessingUnit):
-    def __init__(self, fname, duration=np.timedelta64(1, "m")):
-        self.fname = fname
-        self.duration = duration
-        self.buffer = None
-
-    def __call__(self, xarr):
-        if self.buffer is None:
-            self.buffer = xarr
-        else:
-            self.buffer = concatenate([self.buffer, xarr])
-        if self.buffer["time"][-1] - self.buffer["time"][-1] > self.duration:
-            self.buffer.sel(
-                time=slice(
-                    None,
-                )
-            )
+class ChunkWriter(SignalProcessingUnit):
+    """
+    Write to disk chunk by chunk.
+
+    Parameters
+    ----------
+    path : str
+        Path were to store the chunks. The number of the chunk will be prepended.
+    """
+
+    def __init__(self, path):
+        self.path = path
+        self.chunk = None
+
+    def __call__(self, db):
+        if self.chunk is None:
+            self.initialize(db)
+        self.chunk += 1
+        postfix = f"_{self.chunk:06d}.nc"
+        fname = self.path + postfix
+        db.to_netcdf(fname)
+        return open_database(fname)
+
+    def initialize(self, db):
+        """
+        Initialize the chunk numbering to zero.
+        """
+        self.chunk = 0
+
+    def reset(self):
+        """
+        Reset the chunk numbering.
+        """
+        self.chunk = None
```

### Comparing `xdas-0.1b1/xdas/virtual.py` & `xdas-0.1b2/xdas/virtual.py`

 * *Files identical despite different names*

