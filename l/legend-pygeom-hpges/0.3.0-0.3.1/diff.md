# Comparing `tmp/legend_pygeom_hpges-0.3.0.tar.gz` & `tmp/legend_pygeom_hpges-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legend_pygeom_hpges-0.3.0.tar", last modified: Sun Jun 11 12:13:35 2023, max compression
+gzip compressed data, was "legend_pygeom_hpges-0.3.1.tar", last modified: Sun Jul 16 09:22:42 2023, max compression
```

## Comparing `legend_pygeom_hpges-0.3.0.tar` & `legend_pygeom_hpges-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:13:35.412088 legend_pygeom_hpges-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-11 12:13:35.412088 legend_pygeom_hpges-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-11 12:13:35.412088 legend_pygeom_hpges-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:13:35.408088 legend_pygeom_hpges-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:13:35.408088 legend_pygeom_hpges-0.3.0/src/legend_pygeom_hpges.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-11 12:13:35.000000 legend_pygeom_hpges-0.3.0/src/legend_pygeom_hpges.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-11 12:13:35.000000 legend_pygeom_hpges-0.3.0/src/legend_pygeom_hpges.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 12:13:35.000000 legend_pygeom_hpges-0.3.0/src/legend_pygeom_hpges.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 12:13:35.000000 legend_pygeom_hpges-0.3.0/src/legend_pygeom_hpges.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-11 12:13:35.000000 legend_pygeom_hpges-0.3.0/src/legend_pygeom_hpges.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 12:13:35.000000 legend_pygeom_hpges-0.3.0/src/legend_pygeom_hpges.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:13:35.412088 legend_pygeom_hpges-0.3.0/src/legendhpges/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 12:13:35.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/bege.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/invcoax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/make_hpge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/ppc.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/semicoax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:13:35.412088 legend_pygeom_hpges-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/tests/test_det_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:22:42.809105 legend_pygeom_hpges-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-16 09:22:42.809105 legend_pygeom_hpges-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-16 09:22:42.809105 legend_pygeom_hpges-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:22:42.801105 legend_pygeom_hpges-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:22:42.805105 legend_pygeom_hpges-0.3.1/src/legend_pygeom_hpges.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-16 09:22:42.000000 legend_pygeom_hpges-0.3.1/src/legend_pygeom_hpges.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-16 09:22:42.000000 legend_pygeom_hpges-0.3.1/src/legend_pygeom_hpges.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 09:22:42.000000 legend_pygeom_hpges-0.3.1/src/legend_pygeom_hpges.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 09:22:42.000000 legend_pygeom_hpges-0.3.1/src/legend_pygeom_hpges.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-16 09:22:42.000000 legend_pygeom_hpges-0.3.1/src/legend_pygeom_hpges.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-16 09:22:42.000000 legend_pygeom_hpges-0.3.1/src/legend_pygeom_hpges.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:22:42.809105 legend_pygeom_hpges-0.3.1/src/legendhpges/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/src/legendhpges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-16 09:22:42.000000 legend_pygeom_hpges-0.3.1/src/legendhpges/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/src/legendhpges/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/src/legendhpges/bege.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/src/legendhpges/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/src/legendhpges/invcoax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/src/legendhpges/make_hpge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/src/legendhpges/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/src/legendhpges/p00664b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/src/legendhpges/ppc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/src/legendhpges/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/src/legendhpges/semicoax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/src/legendhpges/v02160a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/src/legendhpges/v02162b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/src/legendhpges/v07646a.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:22:42.809105 legend_pygeom_hpges-0.3.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:22:42.809105 legend_pygeom_hpges-0.3.1/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/tests/configs/P00664B.json
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/tests/configs/V02160A.json
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/tests/configs/V02162B.json
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/tests/configs/V07646A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/tests/test_det_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-16 09:22:33.000000 legend_pygeom_hpges-0.3.1/tests/test_materials.py
```

### Comparing `legend_pygeom_hpges-0.3.0/LICENSE` & `legend_pygeom_hpges-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.3.0/PKG-INFO` & `legend_pygeom_hpges-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_pygeom_hpges
-Version: 0.3.0
+Version: 0.3.1
 Summary: Geometry management for LEGEND HPGE detectors
 Home-page: https://github.com/legend-exp/legend-pygeom-hpges
 Author: Luigi Pertoldi
 Author-email: gipert@pm.me
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 1 - Planning
```

### Comparing `legend_pygeom_hpges-0.3.0/README.md` & `legend_pygeom_hpges-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.3.0/setup.cfg` & `legend_pygeom_hpges-0.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/legend-exp/legend-pygeom-hpges
 author = Luigi Pertoldi
 author_email = gipert@pm.me
 maintainer = The LEGEND Collaboration
 license = GPL-3.0
-license_file = LICENSE
 license_files = LICENSE
 classifiers = 
 	Development Status :: 1 - Planning
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `legend_pygeom_hpges-0.3.0/src/legend_pygeom_hpges.egg-info/PKG-INFO` & `legend_pygeom_hpges-0.3.1/src/legend_pygeom_hpges.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend-pygeom-hpges
-Version: 0.3.0
+Version: 0.3.1
 Summary: Geometry management for LEGEND HPGE detectors
 Home-page: https://github.com/legend-exp/legend-pygeom-hpges
 Author: Luigi Pertoldi
 Author-email: gipert@pm.me
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 1 - Planning
```

### Comparing `legend_pygeom_hpges-0.3.0/src/legendhpges/base.py` & `legend_pygeom_hpges-0.3.1/src/legendhpges/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import math
 from abc import ABC, abstractmethod
 
 from legendmeta.jsondb import AttrsDict
 from pint import Quantity
 from pyg4ometry import geant4
 
-from .materials import enriched_germanium
+from .materials import natural_germanium
 from .registry import default_g4_registry
 from .registry import default_units_registry as u
 
 
 class HPGe(ABC, geant4.LogicalVolume):
     """An High-Purity Germanium detector.
 
@@ -31,15 +31,15 @@
     """
 
     def __init__(
         self,
         metadata: str | dict | AttrsDict,
         name: str = None,
         registry: geant4.Registry = default_g4_registry,
-        material: geant4.MaterialCompound = enriched_germanium,
+        material: geant4.MaterialCompound = natural_germanium,
     ) -> None:
         if registry is None:
             raise ValueError("registry cannot be None")
 
         if metadata is None:
             raise ValueError("metadata cannot be None")
 
@@ -51,27 +51,43 @@
             self.metadata = AttrsDict(metadata)
 
         if name is None:
             self.name = self.metadata.name
         else:
             self.name = name
 
-        # return ordered r,z lists, default unit [mm]
-        r, z = self._decode_polycone_coord()
+        self.registry = registry
 
-        # build generic polycone, and logical volume, default [mm]
-        ic_solid = geant4.solid.GenericPolycone(
-            self.name, 0, 2 * math.pi, r, z, registry
-        )
-
-        super().__init__(ic_solid, material, self.name, registry)
+        # build logical volume, default [mm]
+        super().__init__(self._g4_solid(), material, self.name, self.registry)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.metadata})"
 
+    def _g4_solid(self) -> geant4.solid.SolidBase:
+        """Build (by default) a :class:`pyg4ometry.solid.GenericPolycone` instance from the (r, z) information.
+
+        Returns
+        -------
+        g4_solid
+            A derived class of :class:`pyg4ometry.solid.SolidBase` to be used to construct the logical volume.
+
+        Note
+        ----
+            Detectors with a special geometry can have this method overridden in their class definition.
+        """
+        # return ordered r,z lists, default unit [mm]
+        r, z = self._decode_polycone_coord()
+
+        # build generic polycone, default [mm]
+        g4_solid = geant4.solid.GenericPolycone(
+            self.name, 0, 2 * math.pi, r, z, self.registry
+        )
+        return g4_solid
+
     @abstractmethod
     def _decode_polycone_coord(self) -> tuple[list[float], list[float]]:
         """Decode shape information from geometry dictionary into (r, z) coordinates.
 
         Suitable for building a :class:`G4GenericPolycone`.
 
         Returns
```

### Comparing `legend_pygeom_hpges-0.3.0/src/legendhpges/bege.py` & `legend_pygeom_hpges-0.3.1/src/legendhpges/bege.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.3.0/src/legendhpges/draw.py` & `legend_pygeom_hpges-0.3.1/src/legendhpges/draw.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 from __future__ import annotations
 
+import logging
+
 import matplotlib.pyplot as plt
 from pyg4ometry.visualisation import VtkViewer
 
 from .base import HPGe
+from .p00664b import P00664B
+from .v02160a import V02160A
 
 
-def plot_profile(hpge: HPGe, axes: plt.Axes = None, **kwargs) -> (plt.Figure, plt.Axes):
+def plot_profile(
+    hpge: HPGe, axes: plt.Axes = None, **kwargs
+) -> tuple[plt.Figure, plt.Axes]:
     """Plot the HPGe profile with :mod:`matplotlib`.
 
     Parameters
     ----------
     hpge
         detector.
     axes
         pre-existing axes where the profile will be plotted.
     **kwargs
         any keyword argument supported by :func:`matplotlib.pyplot.plot`.
 
     """
     # data
-    r = hpge.solid.pR
-    z = hpge.solid.pZ
+    if isinstance(hpge, (V02160A, P00664B)):
+        r = hpge.solid.obj1.pR
+        z = hpge.solid.obj1.pZ
+        logging.warning("The detector profile is that of the solid without cut")
+    else:
+        r = hpge.solid.pR
+        z = hpge.solid.pZ
+
     x = r + [-x for x in reversed(r)]
     y = z + list(reversed(z))
 
     colors = plt.rcParams["axes.prop_cycle"].by_key()["color"]
 
     fig = None
     if axes is None:
```

### Comparing `legend_pygeom_hpges-0.3.0/src/legendhpges/invcoax.py` & `legend_pygeom_hpges-0.3.1/src/legendhpges/invcoax.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,18 +87,23 @@
                 c.height_in_mm,
                 c.height_in_mm - c.taper.borehole.height_in_mm,
             ]
         else:
             r += [c.borehole.radius_in_mm]
             z += [c.height_in_mm]
 
-        r += [
-            c.borehole.radius_in_mm,
-            0,
-        ]
+        if c.taper.borehole.height_in_mm != c.borehole.depth_in_mm:
+            r += [
+                c.borehole.radius_in_mm,
+                0,
+            ]
+
+            z += [
+                c.height_in_mm - c.borehole.depth_in_mm,
+                c.height_in_mm - c.borehole.depth_in_mm,
+            ]
+        else:
+            r += [0]
 
-        z += [
-            c.height_in_mm - c.borehole.depth_in_mm,
-            c.height_in_mm - c.borehole.depth_in_mm,
-        ]
+            z += [c.height_in_mm - c.borehole.depth_in_mm]
 
         return r, z
```

### Comparing `legend_pygeom_hpges-0.3.0/src/legendhpges/make_hpge.py` & `legend_pygeom_hpges-0.3.1/src/legendhpges/make_hpge.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,26 +3,30 @@
 import json
 
 from legendmeta.jsondb import AttrsDict
 from pyg4ometry import geant4
 
 from .bege import BEGe
 from .invcoax import InvertedCoax
-from .materials import _enriched_germanium
+from .materials import make_enriched_germanium
+from .p00664b import P00664B
 from .ppc import PPC
 from .registry import default_g4_registry
 from .semicoax import SemiCoax
+from .v02160a import V02160A
+from .v02162b import V02162B
+from .v07646a import V07646A
 
 
 def make_hpge(
     metadata: str | dict | AttrsDict,
     registry: geant4.Registry = default_g4_registry,
     **kwargs,
 ) -> geant4.LogicalVolume:
-    """Costructing an HPGe detector logical volume based on the detector metadata.
+    """Construct an HPGe detector logical volume based on the detector metadata.
 
     Parameters
     ----------
     metadata
         LEGEND HPGe configuration metadata file containing
         detector static properties.
     registry
@@ -40,32 +44,52 @@
         material
             pyg4ometry Geant4 material for the detector.
 
     Examples
     --------
         >>> gedet = make_hpge(metadata, registry)
 
-        >>> make_hpge(metadata, registry, name = "my_det", material = my_material)
+        >>> gedet = make_hpge(metadata, registry, name = "my_det", material = my_material)
 
     """
     if not isinstance(metadata, (dict, AttrsDict)):
         with open(metadata) as jfile:
             gedet_meta = AttrsDict(json.load(jfile))
     else:
         gedet_meta = AttrsDict(metadata)
 
-    kwargs.setdefault("material", _enriched_germanium(gedet_meta.production.enrichment))
-    kwargs.setdefault("name", gedet_meta.name)
+    material = kwargs.get("material")
+    name = kwargs.get("name")
+
+    if material is None:
+        if gedet_meta.production.enrichment is None:
+            raise ValueError("The enrichment argument in the metadata is None.")
+        kwargs["material"] = make_enriched_germanium(gedet_meta.production.enrichment)
+
+    if name is None:
+        if gedet_meta.name is None:
+            raise ValueError("The name of the detector in the metadata is None.")
+        kwargs["name"] = gedet_meta.name
 
     if gedet_meta.type == "ppc":
-        gedet = PPC(metadata, registry=registry, **kwargs)
+        if gedet_meta.name == "P00664B":
+            gedet = P00664B(gedet_meta, registry=registry, **kwargs)
+        else:
+            gedet = PPC(gedet_meta, registry=registry, **kwargs)
 
     elif gedet_meta.type == "bege":
-        gedet = BEGe(metadata, registry=registry, **kwargs)
+        gedet = BEGe(gedet_meta, registry=registry, **kwargs)
 
     elif gedet_meta.type == "icpc":
-        gedet = InvertedCoax(metadata, registry=registry, **kwargs)
+        if gedet_meta.name == "V07646A":
+            gedet = V07646A(gedet_meta, registry=registry, **kwargs)
+        elif gedet_meta.name == "V02160A":
+            gedet = V02160A(gedet_meta, registry=registry, **kwargs)
+        elif gedet_meta.name == "V02162B":
+            gedet = V02162B(gedet_meta, registry=registry, **kwargs)
+        else:
+            gedet = InvertedCoax(gedet_meta, registry=registry, **kwargs)
 
     elif gedet_meta.type == "coax":
-        gedet = SemiCoax(metadata, registry=registry, **kwargs)
+        gedet = SemiCoax(gedet_meta, registry=registry, **kwargs)
 
     return gedet
```

### Comparing `legend_pygeom_hpges-0.3.0/src/legendhpges/ppc.py` & `legend_pygeom_hpges-0.3.1/src/legendhpges/ppc.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.3.0/src/legendhpges/semicoax.py` & `legend_pygeom_hpges-0.3.1/src/legendhpges/semicoax.py`

 * *Files identical despite different names*

